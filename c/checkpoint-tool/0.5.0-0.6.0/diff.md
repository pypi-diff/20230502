# Comparing `tmp/checkpoint_tool-0.5.0.tar.gz` & `tmp/checkpoint_tool-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkpoint_tool-0.5.0.tar", max compression
+gzip compressed data, was "checkpoint_tool-0.6.0.tar", max compression
```

## Comparing `checkpoint_tool-0.5.0.tar` & `checkpoint_tool-0.6.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     4391 2023-04-29 13:31:23.891521 checkpoint_tool-0.5.0/README.md
--rw-r--r--   0        0        0    21944 2023-04-30 12:26:06.634930 checkpoint_tool-0.5.0/checkpoint.py
--rw-r--r--   0        0        0      679 2023-04-30 12:28:21.280430 checkpoint_tool-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     5245 1970-01-01 00:00:00.000000 checkpoint_tool-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     5113 2023-05-02 05:40:25.984486 checkpoint_tool-0.6.0/README.md
+-rw-r--r--   0        0        0    23405 2023-05-02 05:49:00.896816 checkpoint_tool-0.6.0/checkpoint.py
+-rw-r--r--   0        0        0      679 2023-05-02 05:53:00.536869 checkpoint_tool-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     5967 1970-01-01 00:00:00.000000 checkpoint_tool-0.6.0/PKG-INFO
```

### Comparing `checkpoint_tool-0.5.0/README.md` & `checkpoint_tool-0.6.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: checkpoint-tool
+Version: 0.6.0
+Summary: A lightweight workflow management tool written in pure Python
+Home-page: https://github.com/koheimiya/checkpoint
+License: MIT
+Author: Kohei Miyaguchi
+Author-email: koheimiyaguchi@gmail.com
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: cloudpickle (>=2.2.1,<3.0.0)
+Requires-Dist: diskcache (>=5.6.1,<6.0.0)
+Requires-Dist: networkx (>=3.1,<4.0)
+Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
+Project-URL: Repository, https://github.com/koheimiya/checkpoint
+Description-Content-Type: text/markdown
+
 # Checkpoint-tool
 
 A lightweight workflow management tool written in pure Python.
 
 Internally, it depends on `DiskCache`, `cloudpickle` `networkx` and `concurrent.futures`.
 
 
@@ -63,68 +85,101 @@
 # Delete all the cache associated with `choose`,
 # equivalent to `rm -r {$CP_CACHE_DIR:-./.cache}/checkpoint/{module_name}.choose`.
 choose.clear()            
 ```
 
 ### Advanced IO
 
-More complex inputs can be used as long as it is JSON serializable:
+More complex inputs can be passed as long as it is JSON serializable:
 ```python
 @task
-def task1(**param1):
+def f1(**param1):
     ...
 
 @task
-def task2(**param2):
+def f2(**param2):
     ...
 
 @task
-def task3(json_params):
-    @requires(task1(**json_params['param1']))
-    @requires(task2(**json_params['param2']))
-    def __(result1, result2):
+def f3(json_params):
+    @requires(f1(**json_params['param1']))
+    @requires(f2(**json_params['param2']))
+    def __(obj1, obj2):
         ...
     return __
 
-result = task3({'param1': { ... }, 'param2': { ... }}).run()
+result = f3({'param1': { ... }, 'param2': { ... }}).run()
 ```
 
-Task dependencies can be specified with lists and dicts:
+Even more complex inputs can be passed as `task`s:
 ```python
+from checkpoint import Task
+
+Dataset = ...  # Some complex data structure
+Model = ...    # Some complex data structure
+
 @task
-def task3(json_params):
-    @requires([task1(p) for p in json_params['my_param_list']])
-    @requires({k: task2(p) for k, p in json_params['my_param_dict'].items()})
-    def __(result_list, result_dict):
+def load_dataset():
+    def __() -> Dataset:
         ...
     return __
 
-result = task3({'my_param_list': [ ... ], 'my_param_dict': { ... }}).run()
+@task
+def train_model(dataset_task: Task[Dataset]):
+    @requires(dataset_task)
+    def __(dataset) -> Model:
+        ...
+    return __
+    
+@task
+def score_model(dataset_task: Task[Dataset], model_task: Task[Model]):
+    @requires(dataset_task)
+    @requires(model_task)
+    def __(dataset, model) -> float:
+        ...
+    return __
+
+
+dataset_task = load_dataset()
+model_task = train_model(dataset)
+score_task = score_model(dataset, model)
+print(score_task.run())
+```
+
+Task dependencies can be specified with lists and dicts:
+```python
+@task
+def summarize_scores(scores_tasks: dict[str, Task[float]]):
+
+    @requires(score_tasks)
+    def __(score_dict):
+        ...
+    return __
 ```
 
 Large outputs can be stored with compression via `zlib`:
 ```python
 @task(compress_level=-1)
-def large_output_task(*args, **kwargs):
+def large_output_task():
     ...
 ```
 
 ### Data directories
 
-Use `@requires_directory` decorator to create a fresh directory dedicated to each task. The contents of the directory are cleared at each task call and persist until `clear`ed.
+Use `TaskDirectory` to create a fresh directory dedicated to each task. The contents of the directory are cleared at each task call and persist until the task is `clear`ed.
 ```python
 from pathlib import Path
-from checkpoint import requires_directory
+from checkpoint import TaskDirectory
 
 @task
 def train_model(...):
 
     # Passing a new directory at
     # `{$CP_CACHE_DIR:-./.cache}/checkpoint/{module_name}.{function_name}/data/{cryptic_task_id}`
-    @requires_directory
+    @requires(TaskDirectory())
     def __(path: Path) -> str:
         ...
         model_path = str(path / 'model.bin')
         model.save(model_path)
         return model_path
 
     return __
@@ -143,25 +198,38 @@
 # Limit the number of parallel workers
 my_task().run(executor=ProcessPoolExecutor(max_workers=2))
 
 # Thread-based parallelism
 my_task().run(executor=ThreadPoolExecutor())
 ```
 
-One can also control the concurrency at a task level:
+One can also control the concurrency at a task/queue level:
 ```python
-@task(max_concurrency=2)
-def resource_intensive_task(*args, **kwargs):
+# Task-level concurrency limit
+my_task().run(rate_limit={my_task.queue: 2})
+
+# Queue-level concurrency limit
+@task(queue='gpu')
+def task_using_gpu():
+    ...
+
+@task(queue='gpu')
+def another_task_using_gpu():
     ...
+
+# ...
+some_downstream_task.run(rate_limit={'gpu': 1})
+
 ```
 
 ### Commandline tool
 We can use checkpoint-tool from commandline like `python -m checkpoint path/to/taskfile.py`, where `taskfile.py` defines the `main` task as follows:
 ```python
 # taskfile.py
 
 @task
 def main():
     ...
 ```
 The command runs the `main` task and stores the cache right next to `taskfile.py` as `.cache/checkpoint/...`.
 Please refer to `python -m checkpoint --help` for more info.
+
```

### Comparing `checkpoint_tool-0.5.0/checkpoint.py` & `checkpoint_tool-0.6.0/checkpoint.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """ A lightweight workflow management tool written in pure Python.
 
-TODO:
-    - Task change detection
-        - via variable-anonymized AST
-    - Priority-based scheduling
+Key features:
+    - Intuitive and flexible task graph creation with small boilerblates.
+    - Automatic cache/data management (source code change detection, cache/data dependency tracking).
+    - Task queue with rate limits.
+
+Limitations:
+    - No priority-based scheduling.
 """
 from __future__ import annotations
 from typing import Callable, ClassVar, Generic, NewType, TypeVar, Any, cast, overload
 from typing_extensions import ParamSpec, Concatenate, Self
 from collections import defaultdict
 from dataclasses import dataclass
 from datetime import datetime
 from pathlib import Path
 from concurrent.futures import ProcessPoolExecutor, Future, ThreadPoolExecutor, wait, FIRST_COMPLETED, Executor
 from functools import wraps
-import importlib.util
 import ast
 import os
 import sys
 import logging
 import inspect
 import json
 import base64
@@ -59,15 +61,18 @@
 
 
 Json = NewType('Json', str)
 
 
 K = TypeVar('K')
 T = TypeVar('T')
+S = TypeVar('S')
+U = TypeVar('U')
 P = ParamSpec('P')
+Q = ParamSpec('Q')
 R = TypeVar('R', covariant=True)
 D = TypeVar('D')
 
 
 Serializer = tuple[Callable[[Any], bytes], Callable[[bytes], Any]]
 DEFAULT_SERIALIZER: Serializer = (cloudpickle.dumps, cloudpickle.loads)
 
@@ -192,15 +197,16 @@
 
     def to_tuple(self) -> TaskKey:
         return self.task_factory.get_db_name(), self.key
 
     @property
     def arg_id(self) -> str:
         _, arg_str = self.to_tuple()
-        return base64.urlsafe_b64encode(arg_str.encode()).decode().replace('=', '')
+        id_ = base64.urlsafe_b64encode(zlib.compress(arg_str.encode(), level=9)).decode().replace('=', '')
+        return os.path.join(*[id_[i:i+255] for i in range(0, len(id_), 255)])
 
     @property
     def directory(self) -> Path:
         return Path(self.task_factory.db.data_directory) / self.arg_id
 
     def clear(self) -> None:
         db = self.task_factory.db
@@ -215,61 +221,67 @@
             return None
 
     def get_result(self) -> R:
         db = self.task_factory.db
         return db.load(self.key)
 
     def load_content(self, loader: RunnerFactory[[], R]) -> Task[R]:
-        is_root = not self._register
+        # is_root = not self._register
 
         key = self.to_tuple()
         runner = self._register.get(key, None)
         if runner is None:
             runner = loader()
             self._register[key] = runner
         task = Task(task_factory=self.task_factory, key=self.key, runner=runner)
 
-        if is_root:
-            self._register.clear()
+        # if is_root:
+        #     self._register.clear()
         return task
 
 
 @dataclass(frozen=True)
 class Task(TaskSkeleton[R]):
     """ Runner with cache """
     runner: Runner[R]
 
     def set_result(self) -> None:
         db = self.task_factory.db
         out = self.runner()
         db.save(self.key, out)
 
-    def run(self, *, executor: Executor | None = None, max_workers: int | None = None) -> R:
-        return self.run_with_info(executor=executor, max_workers=max_workers)[0]
+    def run(
+            self, *,
+            executor: Executor | None = None,
+            max_workers: int | None = None,
+            rate_limits: dict[str, int] | None = None
+            ) -> R:
+        return self.run_with_info(executor=executor, max_workers=max_workers, rate_limits=rate_limits)[0]
 
     def run_with_info(
             self, *,
             executor: Executor | None = None,
             max_workers: int | None = None,
+            rate_limits: dict[str, int] | None = None,
             dump_generations: bool = False
             ) -> tuple[R, dict[str, Any]]:
         graph = TaskGraph.build_from(self)
         if executor is None:
             executor = Context.get_executor(max_workers=max_workers)
         else:
             assert max_workers is None
-        info = run_task_graph(graph=graph, executor=executor, dump_generations=dump_generations)
+        info = run_task_graph(graph=graph, executor=executor, rate_limits=rate_limits, dump_graphs=dump_generations)
         return self.get_result(), info
 
 
 @dataclass
 class TaskFactory(Generic[P, R]):
     runner_factory: RunnerFactory[P, R]
     db: Database
-    max_concurrency: int | None
+    queue: str
     source_timestamp: datetime
 
     def get_db_name(self) -> str:
         return self.db.name
 
     def clear(self) -> None:
         self.db.clear()
@@ -279,39 +291,40 @@
         dummy = TaskSkeleton(task_factory=self, key=key)
         return dummy.load_content(loader=lambda: self.runner_factory(*args, **kwargs))
 
 
 @overload
 def task(fn: RunnerFactory[P, R]) -> TaskFactory[P, R]: ...
 @overload
-def task(*, compress_level: int = 0, max_concurrency: int | None = None) -> Callable[[RunnerFactory[P, R]], TaskFactory[P, R]]: ...
+def task(*, compress_level: int = 0, queue: str | None = None) -> Callable[[RunnerFactory[P, R]], TaskFactory[P, R]]: ...
 def task(*args, **kwargs) -> Any:
     if args:
         fn, = args
         return _task()(fn)
     else:
         return _task(**kwargs)
 
 
 def _task(
-        *, compress_level: int = 0, max_concurrency: int | None = None
+        *, compress_level: int = 0, queue: str | None = None
         ) -> Callable[[RunnerFactory[P, R]], TaskFactory[P, R]]:
     """ Convert a runner factory into a task factory. """
 
     def decorator(fn: RunnerFactory[P, R]) -> TaskFactory[P, R]:
         name = _serialize_function(fn)
         db = Database.make(name=name, compress_level=compress_level)
+        _queue = f'<{name}>' if queue is None else queue
 
         source = inspect.getsource(fn)
         formatted_source = ast.unparse(ast.parse(source))
         source_timestamp = db.update_source_if_necessary(formatted_source)
 
         return wraps(fn)(TaskFactory(
             runner_factory=fn, db=db,
-            max_concurrency=max_concurrency,
+            queue=_queue,
             source_timestamp=source_timestamp
             ))
     return decorator
 
 
 def _serialize_function(fn: Callable[..., Any]) -> str:
     return f'{fn.__module__}.{fn.__qualname__}'
@@ -321,133 +334,142 @@
     params = inspect.signature(fn).bind(*args, **kwargs)
     params.apply_defaults()
     return params.arguments
 
 
 def _serialize_arguments(fn: Callable[P, Any], *args: P.args, **kwargs: P.kwargs) -> Json:
     arguments = _normalize_arguments(fn, *args, **kwargs)
-    return cast(Json, json.dumps(arguments, separators=(',', ':'), sort_keys=True))
+    return cast(Json, json.dumps(arguments, separators=(',', ':'), sort_keys=True, cls=CustomJSONEncoder))
+
+
+class CustomJSONEncoder(json.JSONEncoder):
+    def default(self, o):
+        if isinstance(o, Task):
+            return {'__task__': o.to_tuple()}
+        else:
+            # Let the base class default method raise the TypeError
+            return super().default(o)
 
 
 AnyTask = Task[Any]
-Connector = Callable[[Callable[Concatenate[T, P], R]], Callable[P, R]]  # Takes (T, *P) -> R and return P -> R
 
 
-@overload
-def requires(task: Task[T]) -> Connector[T, P, R]: ...
-@overload
-def requires(task: list[Task[T]]) -> Connector[list[T], P, R]: ...
-@overload
-def requires(task: dict[K, Task[T]]) -> Connector[dict[K, T], P, R]: ...
-def requires(task: AnyTask | list[AnyTask] | dict[Any, AnyTask]) -> Any:
-    """ Register a task dependency """
-    if isinstance(task, Task):
-        return requires_single(task)
-    elif isinstance(task, list):
-        return requires_list(task)
-    elif isinstance(task, dict):
-        return requires_dict(task)
+def get_prerequisite_tasks(task: AnyTask) -> list[AnyTask]:
+    if isinstance(task.runner, PartialRunner):
+        task.runner.set_directory(task.directory)
+        return task.runner.get_tasks()
     else:
-        raise TypeError(task)
+        return []
 
 
-@dataclass(frozen=True)
-class Connected(Generic[T, P, R]):
-    """ Connect a task to a function. """
-    pre_task: Task[T]
-    fn: Callable[Concatenate[T, P], R]
-
-    def __call__(self, *args: P.args, **kwargs: P.kwargs) -> R:
-        x = self.pre_task.get_result()
-        return self.fn(x, *args, **kwargs)
-
-    def get_prerequisites(self) -> list[AnyTask]:
-        return [self.pre_task]
-
-
-def requires_single(task: Task[T]) -> Connector[T, P, R]:
-    """ Register a task dependency """
-    def decorator(fn: Callable[Concatenate[T, P], R]) -> Callable[P, R]:
-        return Connected(task, fn)
-    return decorator
+@dataclass
+class TaskDirectory:
+    path: Path | None = None
 
+    def get_path_prepared(self) -> Path:
+        assert self.path is not None, 'Should never happens.'
+        if self.path.exists():
+            shutil.rmtree(self.path)
+        self.path.mkdir()
+        return self.path
 
-@dataclass(frozen=True)
-class ListConnected(Generic[T, P, R]):
-    """ Connect a list of tasks to a function. """
-    pre_tasks: list[Task[T]]
-    fn: Callable[Concatenate[list[T], P], R]
-
-    def __call__(self, *args: P.args, **kwargs: P.kwargs) -> R:
-        xs = [task.get_result() for task in self.pre_tasks]
-        return self.fn(xs, *args, **kwargs)
-
-    def get_prerequisites(self) -> list[AnyTask]:
-        return self.pre_tasks
-
-
-def requires_list(tasks: list[Task[T]]) -> Connector[list[T], P, R]:
-    """ Register a task dependency """
-    def decorator(fn: Callable[Concatenate[list[T], P], R]) -> Callable[P, R]:
-        return ListConnected(tasks, fn)
-    return decorator
 
+@dataclass
+class TaskArgs(Generic[P]):
+    args: list[AnyTask | list[AnyTask] | dict[Any, AnyTask] | TaskDirectory]
+
+    def __call__(self, fn: Callable[P, T]) -> T:
+        args: list[Any] = []
+        for a in self.args:
+            if isinstance(a, Task):
+                args.append(a.get_result())
+            elif isinstance(a, list):
+                args.append([ai.get_result() for ai in a])
+            elif isinstance(a, dict):
+                args.append({k: v.get_result() for k, v in a.items()})
+            elif isinstance(a, TaskDirectory):
+                args.append(a.get_path_prepared())
+            else:
+                raise TypeError(a)
+        return fn(*args)  # type: ignore
 
-@dataclass(frozen=True)
-class DictConnected(Generic[K, T, P, R]):
-    """ Connect a dict of tasks to a function. """
-    pre_tasks: dict[K, Task[T]]
-    fn: Callable[Concatenate[dict[K, T], P], R]
-
-    def __call__(self, *args: P.args, **kwargs: P.kwargs) -> R:
-        xs = {k: task.get_result() for k, task in self.pre_tasks.items()}
-        return self.fn(xs, *args, **kwargs)
-
-    def get_prerequisites(self) -> list[AnyTask]:
-        return list(self.pre_tasks.values())
-
-
-def requires_dict(tasks: dict[K, Task[T]]) -> Connector[dict[K, T], P, R]:
-    """ Register a task dependency """
-    def decorator(fn: Callable[Concatenate[dict[K, T], P], R]) -> Callable[P, R]:
-        return DictConnected(tasks, fn)
-    return decorator
+    def get_tasks(self) -> list[AnyTask]:
+        tasks: list[AnyTask] = []
+        for a in self.args:
+            if isinstance(a, Task):
+                tasks.append(a)
+            elif isinstance(a, list):
+                tasks.extend(a)
+            elif isinstance(a, dict):
+                tasks.extend(a.values())
+        return tasks
+
+    def set_directory(self, path: Path) -> None:
+        placeholders = [a for a in self.args if isinstance(a, TaskDirectory)]
+        for ph in placeholders:
+            ph.path = path
+
+    @overload
+    def cons(self, task: Task[S]) -> TaskArgs[Concatenate[S, P]]: ...
+    @overload
+    def cons(self, task: list[Task[S]]) -> TaskArgs[Concatenate[list[S], P]]: ...
+    @overload
+    def cons(self, task: dict[K, Task[S]]) -> TaskArgs[Concatenate[dict[K, S], P]]: ...
+    def cons(self, task: Any) -> TaskArgs[...]:
+        return TaskArgs(args=[task, *self.args])
+
+    @classmethod
+    def empty(cls) -> TaskArgs[[]]:
+        return TaskArgs([])
 
 
 @dataclass
-class RequiresDirectory(Generic[P, R]):
-    fn: Callable[Concatenate[Path, P], R]
-    directory: Path | None = None
+class PartialRunner(Generic[P, Q, T]):
+    cont: TaskArgs[P]
+    fn: Callable[Q, T]
 
-    def __call__(self, *args: P.args, **kwargs: P.kwargs) -> R:
-        assert self.directory is not None, 'Directory not set. Bug?'
-        if self.directory.exists():
-            shutil.rmtree(self.directory)
-        self.directory.mkdir()
-        return self.fn(self.directory, *args, **kwargs)
+    @classmethod
+    def init(cls, fn: Callable[Q, T]) -> PartialRunner[[], Q, T]:
+        return PartialRunner(cont=TaskArgs.empty(), fn=fn)
+
+    def __call__(self: PartialRunner[P, P, T]) -> T:
+        return self.cont(self.fn)
 
     def set_directory(self, path: Path) -> None:
-        self.directory = path
+        self.cont.set_directory(path)
 
+    def get_tasks(self) -> list[AnyTask]:
+        return self.cont.get_tasks()
 
-def requires_directory(fn: Callable[Concatenate[Path, P], R]) -> Callable[P, R]:
-    """ Create fresh directory dedicated to the task """
-    return RequiresDirectory(fn)
 
+@dataclass
+class requires(Generic[S]):
+    task: S
 
-def get_prerequisite_tasks(task: AnyTask) -> list[AnyTask]:
-    deps: list[Task[Any]] = []
-    task_fn = task.runner
-    while isinstance(task_fn, (Connected, ListConnected, DictConnected, RequiresDirectory)):
-        if isinstance(task_fn, (Connected, ListConnected, DictConnected)):
-            deps.extend(task_fn.get_prerequisites())
+    @overload
+    def __call__(self: requires[Task[U]], f: Callable[Q, T]) -> PartialRunner[[U], Q, T]: ...
+    @overload
+    def __call__(self: requires[list[Task[U]]], f: Callable[Q, T]) -> PartialRunner[[list[U]], Q, T]: ...
+    @overload
+    def __call__(self: requires[dict[K, Task[U]]], f: Callable[Q, T]) -> PartialRunner[[dict[K, U]], Q, T]: ...
+    @overload
+    def __call__(self: requires[TaskDirectory], f: Callable[Q, T]) -> PartialRunner[[Path], Q, T]: ...
+    @overload
+    def __call__(self: requires[Task[U]], f: PartialRunner[P, Q, T]) -> PartialRunner[Concatenate[U, P], Q, T]: ...
+    @overload
+    def __call__(self: requires[list[Task[U]]], f: PartialRunner[P, Q, T]) -> PartialRunner[Concatenate[list[U], P], Q, T]: ...
+    @overload
+    def __call__(self: requires[dict[K, Task[U]]], f: PartialRunner[P, Q, T]) -> PartialRunner[Concatenate[dict[K, U], P], Q, T]: ...
+    @overload
+    def __call__(self: requires[TaskDirectory], f: PartialRunner[P, Q, T]) -> PartialRunner[Concatenate[Path, P], Q, T]: ...
+    def __call__(self: requires[Any], f: Callable[Q, T] | PartialRunner[P, Q, T]) -> PartialRunner[[Any], Q, T] | PartialRunner[Concatenate[Any, P], Q, T]:
+        if isinstance(f, PartialRunner):
+            return PartialRunner(cont=f.cont.cons(self.task), fn=f.fn)
         else:
-            task_fn.set_directory(task.directory)
-        task_fn = task_fn.fn
-    return deps
+            return PartialRunner(TaskArgs.empty().cons(self.task), f)
 
 
 @dataclass
 class TaskGraph:
     G: nx.DiGraph
 
     @classmethod
@@ -504,154 +526,156 @@
         TR = nx.transitive_reduction(self.G)
         TR.add_nodes_from(self.G.nodes(data=True))
         self.G = TR
 
     def get_task_factories(self) -> dict[str, TaskFactory[..., Any]]:
         return dict((path, attr['task'].task_factory) for (path, _), attr in self.G.nodes.items())
 
-    def get_initial_tasks(self) -> list[TaskKey]:
-        return [x for x in self.G if self.G.in_degree(x) == 0]
+    def get_initial_tasks(self) -> dict[str, list[TaskKey]]:
+        leaves = [x for x in self.G if self.G.in_degree(x) == 0]
+        return self._group_by_queue(leaves)
+
+    def _group_by_queue(self, nodes: list[TaskKey]) -> dict[str, list[TaskKey]]:
+        out = defaultdict(list)
+        for x in nodes:
+            out[self.get_task(x).task_factory.queue].append(x)
+        return out
 
-    def pop_with_new_leaves(self, x: TaskKey, disallow_non_leaf: bool = True) -> list[TaskKey]:
+    def pop_with_new_leaves(self, x: TaskKey, disallow_non_leaf: bool = True) -> dict[str, list[TaskKey]]:
         if disallow_non_leaf:
             assert not list(self.G.predecessors(x))
 
         new_leaves: list[TaskKey] = []
         for y in self.G.successors(x):
             if self.G.in_degree(y) == 1:
                 new_leaves.append(y)
 
         self.G.remove_node(x)
-        return new_leaves
+        return self._group_by_queue(new_leaves)
 
-    def get_grouped_nodes(self) -> dict[str, list[Json]]:
+    def get_nodes_by_task(self) -> dict[str, list[Json]]:
         out: dict[str, list[Json]] = defaultdict(list)
         for x in self.G:
             path, args = x
             out[path].append(args)
         return dict(out)
 
 
-def _group_nodes_by_db(tasks: list[TaskKey]) -> dict[str, list[TaskKey]]:
-    out = defaultdict(list)
-    for x in tasks:
-        db, _ = x
-        out[db].append(x)
-    return dict(out)
-
-
-def run_task_graph(graph: TaskGraph, executor: Executor, dump_generations: bool = False) -> dict[str, Any]:
+def run_task_graph(
+        graph: TaskGraph,
+        executor: Executor,
+        rate_limits: dict[str, int] | None = None,
+        dump_graphs: bool = False,
+        ) -> dict[str, Any]:
     """ Consume task graph concurrently.
     """
-    stats = {k: len(args) for k, args in graph.get_grouped_nodes().items()}
+    stats = {k: len(args) for k, args in graph.get_nodes_by_task().items()}
     LOGGER.info(f'Following tasks will be called: {stats}')
     info = {'stats': stats, 'generations': []}
 
     # Read concurrency budgets
-    budgets: dict[str, int] = {}
-    occupied: dict[str, int] = {}
-    for path, fac in graph.get_task_factories().items():
-        mc = fac.max_concurrency
-        if mc is not None:
-            budgets[path] = mc
-            occupied[path] = 0
+    if rate_limits is None:
+        rate_limits = {}
+    occupied = {k: 0 for k in rate_limits}
 
     # Execute tasks
-    standby = _group_nodes_by_db(graph.get_initial_tasks())
-    in_process: set[Future[TaskKey]] = set()
+    standby = graph.get_initial_tasks()
+    in_process: set[Future[tuple[str, TaskKey]]] = set()
     with executor as executor:
         while standby or in_process:
             # Log some stats
             LOGGER.info(
                     f'nodes: {graph.size}, '
                     f'standby: {len(standby)}, '
                     f'in_process: {len(in_process)}'
                     )
-            if dump_generations:
-                info['generations'].append(graph.get_grouped_nodes())
+            if dump_graphs:
+                info['generations'].append(graph.get_nodes_by_task())
 
             # Submit all leaf tasks
             leftover: dict[str, list[TaskKey]] = {}
-            for path, keys in standby.items():
-                if path in budgets:
-                    free = budgets[path] - occupied[path]
+            for queue, keys in standby.items():
+                if queue in rate_limits:
+                    free = rate_limits[queue] - occupied[queue]
                     to_submit, to_hold = keys[:free], keys[free:]
-                    occupied[path] += len(to_submit)
+                    occupied[queue] += len(to_submit)
                     if to_hold:
-                        leftover[path] = to_hold
+                        leftover[queue] = to_hold
                 else:
                     to_submit = keys
 
                 for key in to_submit:
-                    future = executor.submit(_run_task, cloudpickle.dumps(graph.get_task(key)))
+                    future = executor.submit(_run_task, queue, cloudpickle.dumps(graph.get_task(key)))
                     in_process.add(future)
 
             # Wait for the first tasks to complete
             done, in_process = wait(in_process, return_when=FIRST_COMPLETED)
 
             # Update graph
             standby = defaultdict(list, leftover)
             for done_future in done:
-                x_done = done_future.result()
+                queue_done, x_done = done_future.result()
 
                 # Update occupied
-                path = x_done[0]
-                if path in occupied:
-                    occupied[path] -= 1
-                    assert occupied[path] >= 0
+                if queue_done in occupied:
+                    occupied[queue_done] -= 1
+                    assert occupied[queue_done] >= 0
 
                 # Remove node from graph
                 ys = graph.pop_with_new_leaves(x_done)
 
                 # Update standby
-                for y in ys:
-                    standby[y[0]].append(y)
+                for queue, task in ys.items():
+                    standby[queue].extend(task)
 
     # Sanity check
     assert graph.size == 0, f'Graph is not empty. Should not happen.'
     assert all(n == 0 for n in occupied.values()), 'Incorrect task count. Should not happen.'
     return info
 
 
-def _run_task(task_data: bytes) -> tuple[str, Json]:
+def _run_task(queue: str, task_data: bytes) -> tuple[str, TaskKey]:  # queue, (dbname, key)
     task = cloudpickle.loads(task_data)
     assert isinstance(task, Task)
     task.set_result()
-    return task.to_tuple()
+    return queue, task.to_tuple()
 
 
 @click.command
 @click.argument('taskfile', type=Path)
 @click.option('-e', '--entrypoint', default='main', help='Task name for entrypoint.')
 @click.option('-t', '--exec-type', type=click.Choice(['process', 'thread']), default='process')
 @click.option('-w', '--max-workers', type=int, default=-1)
 @click.option('--cache-dir', type=Path, default=None)
+@click.option('--rate-limits', type=json.loads, default=None, help='JSON dictionary for rate_limits.')
 @click.option('-D', '--detect-source-change', is_flag=True, help='Automatically discard the cache per task once the source code (AST) is changed.')
-def main(taskfile: Path, entrypoint: str, exec_type: str, max_workers: int, cache_dir: Path | None, detect_source_change: bool):
+def main(taskfile: Path, entrypoint: str, exec_type: str, max_workers: int, cache_dir: Path | None, rate_limits: dict[str, Any] | None, detect_source_change: bool):
     # Set arguments as environment variables
     os.environ['CP_EXECUTOR'] = exec_type
     os.environ['CP_MAX_WORKERS'] = str(max_workers)
     os.environ['CP_CACHE_DIR'] = str(taskfile.parent / '.cache') if cache_dir is None else str(cache_dir)
     os.environ['CP_DETECT_SOURCE_CHANGE'] = str(int(detect_source_change))
 
     # Run script as module
     module_name = taskfile.with_suffix('').name
-    spec = importlib.util.spec_from_file_location(module_name, taskfile)
-    assert spec is not None
-    assert spec.loader is not None
-    module = importlib.util.module_from_spec(spec)
-    sys.modules[module_name] = module
-    spec.loader.exec_module(module)
+    sys.path.append(str(taskfile.parent))
+    module = __import__(module_name)
+    # import importlib.util
+    # spec = importlib.util.spec_from_file_location(module_name, taskfile)
+    # assert spec is not None
+    # assert spec.loader is not None
+    # module = importlib.util.module_from_spec(spec)
+    # sys.modules[module_name] = module
+    # spec.loader.exec_module(module)
 
     # Run the main task
     entrypoint_fn = getattr(module, entrypoint)
     assert type(entrypoint_fn).__name__ == TaskFactory.__name__, \
             f'Taskfile `{taskfile}` should contain a task(factory) `{entrypoint}`, but found `{entrypoint_fn}`.'
     entrypoint_fn = cast(TaskFactory, entrypoint_fn)
     task = entrypoint_fn()
-    task.run()
-    print(task.directory)
+    print(task.run(rate_limits=rate_limits))
     return 0
 
 
 if __name__ == '__main__':
     sys.exit(main())
```

### Comparing `checkpoint_tool-0.5.0/pyproject.toml` & `checkpoint_tool-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "checkpoint-tool"
-version = "0.5.0"
+version = "0.6.0"
 description = "A lightweight workflow management tool written in pure Python"
 authors = ["Kohei Miyaguchi <koheimiyaguchi@gmail.com>"]
 license = "MIT License"
 homepage = "https://github.com/koheimiya/checkpoint"
 repository = "https://github.com/koheimiya/checkpoint"
 readme = "README.md"
 packages = [{include = "checkpoint.py"}]
```

### Comparing `checkpoint_tool-0.5.0/PKG-INFO` & `checkpoint_tool-0.6.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: checkpoint-tool
-Version: 0.5.0
-Summary: A lightweight workflow management tool written in pure Python
-Home-page: https://github.com/koheimiya/checkpoint
-License: MIT
-Author: Kohei Miyaguchi
-Author-email: koheimiyaguchi@gmail.com
-Requires-Python: >=3.9,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: cloudpickle (>=2.2.1,<3.0.0)
-Requires-Dist: diskcache (>=5.6.1,<6.0.0)
-Requires-Dist: networkx (>=3.1,<4.0)
-Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
-Project-URL: Repository, https://github.com/koheimiya/checkpoint
-Description-Content-Type: text/markdown
-
 # Checkpoint-tool
 
 A lightweight workflow management tool written in pure Python.
 
 Internally, it depends on `DiskCache`, `cloudpickle` `networkx` and `concurrent.futures`.
 
 
@@ -85,68 +63,101 @@
 # Delete all the cache associated with `choose`,
 # equivalent to `rm -r {$CP_CACHE_DIR:-./.cache}/checkpoint/{module_name}.choose`.
 choose.clear()            
 ```
 
 ### Advanced IO
 
-More complex inputs can be used as long as it is JSON serializable:
+More complex inputs can be passed as long as it is JSON serializable:
 ```python
 @task
-def task1(**param1):
+def f1(**param1):
     ...
 
 @task
-def task2(**param2):
+def f2(**param2):
     ...
 
 @task
-def task3(json_params):
-    @requires(task1(**json_params['param1']))
-    @requires(task2(**json_params['param2']))
-    def __(result1, result2):
+def f3(json_params):
+    @requires(f1(**json_params['param1']))
+    @requires(f2(**json_params['param2']))
+    def __(obj1, obj2):
         ...
     return __
 
-result = task3({'param1': { ... }, 'param2': { ... }}).run()
+result = f3({'param1': { ... }, 'param2': { ... }}).run()
 ```
 
-Task dependencies can be specified with lists and dicts:
+Even more complex inputs can be passed as `task`s:
 ```python
+from checkpoint import Task
+
+Dataset = ...  # Some complex data structure
+Model = ...    # Some complex data structure
+
 @task
-def task3(json_params):
-    @requires([task1(p) for p in json_params['my_param_list']])
-    @requires({k: task2(p) for k, p in json_params['my_param_dict'].items()})
-    def __(result_list, result_dict):
+def load_dataset():
+    def __() -> Dataset:
         ...
     return __
 
-result = task3({'my_param_list': [ ... ], 'my_param_dict': { ... }}).run()
+@task
+def train_model(dataset_task: Task[Dataset]):
+    @requires(dataset_task)
+    def __(dataset) -> Model:
+        ...
+    return __
+    
+@task
+def score_model(dataset_task: Task[Dataset], model_task: Task[Model]):
+    @requires(dataset_task)
+    @requires(model_task)
+    def __(dataset, model) -> float:
+        ...
+    return __
+
+
+dataset_task = load_dataset()
+model_task = train_model(dataset)
+score_task = score_model(dataset, model)
+print(score_task.run())
+```
+
+Task dependencies can be specified with lists and dicts:
+```python
+@task
+def summarize_scores(scores_tasks: dict[str, Task[float]]):
+
+    @requires(score_tasks)
+    def __(score_dict):
+        ...
+    return __
 ```
 
 Large outputs can be stored with compression via `zlib`:
 ```python
 @task(compress_level=-1)
-def large_output_task(*args, **kwargs):
+def large_output_task():
     ...
 ```
 
 ### Data directories
 
-Use `@requires_directory` decorator to create a fresh directory dedicated to each task. The contents of the directory are cleared at each task call and persist until `clear`ed.
+Use `TaskDirectory` to create a fresh directory dedicated to each task. The contents of the directory are cleared at each task call and persist until the task is `clear`ed.
 ```python
 from pathlib import Path
-from checkpoint import requires_directory
+from checkpoint import TaskDirectory
 
 @task
 def train_model(...):
 
     # Passing a new directory at
     # `{$CP_CACHE_DIR:-./.cache}/checkpoint/{module_name}.{function_name}/data/{cryptic_task_id}`
-    @requires_directory
+    @requires(TaskDirectory())
     def __(path: Path) -> str:
         ...
         model_path = str(path / 'model.bin')
         model.save(model_path)
         return model_path
 
     return __
@@ -165,26 +176,37 @@
 # Limit the number of parallel workers
 my_task().run(executor=ProcessPoolExecutor(max_workers=2))
 
 # Thread-based parallelism
 my_task().run(executor=ThreadPoolExecutor())
 ```
 
-One can also control the concurrency at a task level:
+One can also control the concurrency at a task/queue level:
 ```python
-@task(max_concurrency=2)
-def resource_intensive_task(*args, **kwargs):
+# Task-level concurrency limit
+my_task().run(rate_limit={my_task.queue: 2})
+
+# Queue-level concurrency limit
+@task(queue='gpu')
+def task_using_gpu():
+    ...
+
+@task(queue='gpu')
+def another_task_using_gpu():
     ...
+
+# ...
+some_downstream_task.run(rate_limit={'gpu': 1})
+
 ```
 
 ### Commandline tool
 We can use checkpoint-tool from commandline like `python -m checkpoint path/to/taskfile.py`, where `taskfile.py` defines the `main` task as follows:
 ```python
 # taskfile.py
 
 @task
 def main():
     ...
 ```
 The command runs the `main` task and stores the cache right next to `taskfile.py` as `.cache/checkpoint/...`.
 Please refer to `python -m checkpoint --help` for more info.
-
```

