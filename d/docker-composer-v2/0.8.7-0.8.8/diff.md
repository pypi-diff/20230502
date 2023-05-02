# Comparing `tmp/docker_composer_v2-0.8.7.tar.gz` & `tmp/docker_composer_v2-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker_composer_v2-0.8.7.tar", max compression
+gzip compressed data, was "docker_composer_v2-0.8.8.tar", max compression
```

## Comparing `docker_composer_v2-0.8.7.tar` & `docker_composer_v2-0.8.8.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rwxr-xr-x   0        0        0    11358 2023-04-19 22:25:00.981589 docker_composer_v2-0.8.7/LICENSE.txt
--rwxr-xr-x   0        0        0     2356 2023-04-19 22:25:00.981589 docker_composer_v2-0.8.7/README.md
--rwxr-xr-x   0        0        0     1492 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/pyproject.toml
--rwxr-xr-x   0        0        0       60 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/__init__.py
--rwxr-xr-x   0        0        0        0 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/_utils/__init__.py
--rwxr-xr-x   0        0        0     4482 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/_utils/argument.py
--rwxr-xr-x   0        0        0     7763 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/_utils/generate_class.py
--rwxr-xr-x   0        0        0     3997 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/base.py
--rwxr-xr-x   0        0        0        0 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/py.typed
--rw-r--r--   0        0        0     1159 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/build.py
--rw-r--r--   0        0        0     1515 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/config.py
--rw-r--r--   0        0        0      932 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/cp.py
--rw-r--r--   0        0        0     1235 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/create.py
--rw-r--r--   0        0        0     1057 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/down.py
--rw-r--r--   0        0        0      615 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/events.py
--rw-r--r--   0        0        0     1245 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/exec.py
--rw-r--r--   0        0        0      704 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/images.py
--rw-r--r--   0        0        0      743 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/kill.py
--rw-r--r--   0        0        0     1166 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/logs.py
--rw-r--r--   0        0        0      808 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/ls.py
--rw-r--r--   0        0        0      470 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/pause.py
--rw-r--r--   0        0        0      683 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/port.py
--rw-r--r--   0        0        0     1078 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/ps.py
--rw-r--r--   0        0        0      878 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/pull.py
--rw-r--r--   0        0        0      835 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/push.py
--rw-r--r--   0        0        0      696 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/restart.py
--rw-r--r--   0        0        0     1021 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/rm.py
--rw-r--r--   0        0        0     2120 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/run.py
--rw-r--r--   0        0        0      470 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/start.py
--rw-r--r--   0        0        0      571 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/stop.py
--rw-r--r--   0        0        0      480 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/top.py
--rw-r--r--   0        0        0      478 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/unpause.py
--rw-r--r--   0        0        0     2988 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/up.py
--rw-r--r--   0        0        0      676 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/version.py
--rw-r--r--   0        0        0    26076 2023-04-19 22:25:00.985589 docker_composer_v2-0.8.7/src/docker_composer_v2/runner/root.py
--rw-r--r--   0        0        0     3713 1970-01-01 00:00:00.000000 docker_composer_v2-0.8.7/PKG-INFO
+-rwxr-xr-x   0        0        0    11358 2023-05-02 15:46:44.710162 docker_composer_v2-0.8.8/LICENSE.txt
+-rwxr-xr-x   0        0        0     2356 2023-05-02 15:46:44.710162 docker_composer_v2-0.8.8/README.md
+-rwxr-xr-x   0        0        0     1492 2023-05-02 15:46:44.710162 docker_composer_v2-0.8.8/pyproject.toml
+-rwxr-xr-x   0        0        0       60 2023-05-02 15:46:44.710162 docker_composer_v2-0.8.8/src/docker_composer_v2/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-05-02 15:46:44.710162 docker_composer_v2-0.8.8/src/docker_composer_v2/_utils/__init__.py
+-rwxr-xr-x   0        0        0     4934 2023-05-02 15:46:44.710162 docker_composer_v2-0.8.8/src/docker_composer_v2/_utils/argument.py
+-rwxr-xr-x   0        0        0     8003 2023-05-02 15:46:44.710162 docker_composer_v2-0.8.8/src/docker_composer_v2/_utils/generate_class.py
+-rwxr-xr-x   0        0        0     3997 2023-05-02 15:46:44.710162 docker_composer_v2-0.8.8/src/docker_composer_v2/base.py
+-rwxr-xr-x   0        0        0        0 2023-05-02 15:46:44.710162 docker_composer_v2-0.8.8/src/docker_composer_v2/py.typed
+-rw-r--r--   0        0        0     1261 2023-05-02 15:46:44.714162 docker_composer_v2-0.8.8/src/docker_composer_v2/runner/cmd/build.py
+-rw-r--r--   0        0        0     1839 2023-05-02 15:46:44.714162 docker_composer_v2-0.8.8/src/docker_composer_v2/runner/cmd/config.py
+-rw-r--r--   0        0        0      951 2023-05-02 15:46:44.714162 docker_composer_v2-0.8.8/src/docker_composer_v2/runner/cmd/cp.py
+-rw-r--r--   0        0        0     1456 2023-05-02 15:46:44.714162 docker_composer_v2-0.8.8/src/docker_composer_v2/runner/cmd/create.py
+-rw-r--r--   0        0        0     1070 2023-05-02 15:46:44.714162 docker_composer_v2-0.8.8/src/docker_composer_v2/runner/cmd/down.py
+-rw-r--r--   0        0        0      615 2023-05-02 15:46:44.714162 docker_composer_v2-0.8.8/src/docker_composer_v2/runner/cmd/events.py
+-rw-r--r--   0        0        0     1281 2023-05-02 15:46:44.714162 docker_composer_v2-0.8.8/src/docker_composer_v2/runner/cmd/exec.py
+-rw-r--r--   0        0        0      704 2023-05-02 15:46:44.714162 docker_composer_v2-0.8.8/src/docker_composer_v2/runner/cmd/images.py
+-rw-r--r--   0        0        0      743 2023-05-02 15:46:44.714162 docker_composer_v2-0.8.8/src/docker_composer_v2/runner/cmd/kill.py
+-rw-r--r--   0        0        0     1292 2023-05-02 15:46:44.714162 docker_composer_v2-0.8.8/src/docker_composer_v2/runner/cmd/logs.py
+-rw-r--r--   0        0        0      844 2023-05-02 15:46:44.714162 docker_composer_v2-0.8.8/src/docker_composer_v2/runner/cmd/ls.py
+-rw-r--r--   0        0        0      470 2023-05-02 15:46:44.714162 docker_composer_v2-0.8.8/src/docker_composer_v2/runner/cmd/pause.py
+-rw-r--r--   0        0        0      701 2023-05-02 15:46:44.714162 docker_composer_v2-0.8.8/src/docker_composer_v2/runner/cmd/port.py
+-rw-r--r--   0        0        0     1153 2023-05-02 15:46:44.714162 docker_composer_v2-0.8.8/src/docker_composer_v2/runner/cmd/ps.py
+-rw-r--r--   0        0        0      978 2023-05-02 15:46:44.714162 docker_composer_v2-0.8.8/src/docker_composer_v2/runner/cmd/pull.py
+-rw-r--r--   0        0        0      877 2023-05-02 15:46:44.714162 docker_composer_v2-0.8.8/src/docker_composer_v2/runner/cmd/push.py
+-rw-r--r--   0        0        0      696 2023-05-02 15:46:44.714162 docker_composer_v2-0.8.8/src/docker_composer_v2/runner/cmd/restart.py
+-rw-r--r--   0        0        0     1021 2023-05-02 15:46:44.714162 docker_composer_v2-0.8.8/src/docker_composer_v2/runner/cmd/rm.py
+-rw-r--r--   0        0        0     2374 2023-05-02 15:46:44.714162 docker_composer_v2-0.8.8/src/docker_composer_v2/runner/cmd/run.py
+-rw-r--r--   0        0        0      470 2023-05-02 15:46:44.714162 docker_composer_v2-0.8.8/src/docker_composer_v2/runner/cmd/start.py
+-rw-r--r--   0        0        0      571 2023-05-02 15:46:44.714162 docker_composer_v2-0.8.8/src/docker_composer_v2/runner/cmd/stop.py
+-rw-r--r--   0        0        0      480 2023-05-02 15:46:44.718162 docker_composer_v2-0.8.8/src/docker_composer_v2/runner/cmd/top.py
+-rw-r--r--   0        0        0      478 2023-05-02 15:46:44.718162 docker_composer_v2-0.8.8/src/docker_composer_v2/runner/cmd/unpause.py
+-rw-r--r--   0        0        0     3562 2023-05-02 15:46:44.718162 docker_composer_v2-0.8.8/src/docker_composer_v2/runner/cmd/up.py
+-rw-r--r--   0        0        0      716 2023-05-02 15:46:44.718162 docker_composer_v2-0.8.8/src/docker_composer_v2/runner/cmd/version.py
+-rw-r--r--   0        0        0    28404 2023-05-02 15:46:44.718162 docker_composer_v2-0.8.8/src/docker_composer_v2/runner/root.py
+-rw-r--r--   0        0        0     3713 1970-01-01 00:00:00.000000 docker_composer_v2-0.8.8/PKG-INFO
```

### Comparing `docker_composer_v2-0.8.7/LICENSE.txt` & `docker_composer_v2-0.8.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.7/README.md` & `docker_composer_v2-0.8.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 ## Install
 ```shell script
 pip install docker-composer-v2
 ```
 
 ## Usage
-The main class is `docker_compose_v2r.DockerCompose`. Its parameters are
+The main class is `docker_composer_v2.DockerCompose`. Its parameters are
 all options from `docker compose`.
 
 Each `docker compose` subcommand has a corresponding function, e.g. 
 `DockerCompose.run` or `DockerCompose.scale`. Their arguments again mirror 
 the options of the corresponding command.
 
 The resulting object has a `call` function.
```

### Comparing `docker_composer_v2-0.8.7/pyproject.toml` & `docker_composer_v2-0.8.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "docker-composer-v2"
-version = "0.8.7"
+version = "0.8.8"
 description = "Use `docker compose` from within Python. This is a branch forked from https://github.com/schollm/docker-composer to support Docker Compose V2."
 authors = ["Micha <schollm-git@gmx.com>", "Jensen <jensen@kairosaerospace.com>"]
 readme = "README.md"
 homepage = "https://github.com/jensenkairos/docker-composer-v2"
 repository = "https://github.com/jensenkairos/docker-composer-v2"
 license = "Apache-2.0"
 packages = [
```

### Comparing `docker_composer_v2-0.8.7/src/docker_composer_v2/_utils/argument.py` & `docker_composer_v2-0.8.8/src/docker_composer_v2/_utils/argument.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,47 +49,59 @@
         return self.type_desc == OPTION
 
     @staticmethod
     def from_line(line: str) -> "Argument":
         if "  " in line:
             return _from_line_has_sep(line)
 
+        logger.info("from_line: " + line)
         words = iter(line.split())
         has_more = True
         while has_more:
             arg, default_str, has_more = _parse_arg(next(words))
-        type_desc = next(words)
+
         type_from_default = _get_type_name_from_default(default_str)
+        try:
+            type_desc = next(words)
+        except StopIteration:
+            type_desc = type_from_default
         desc = " ".join(words)
         if type_desc[1:].islower() and "=" not in type_desc:
             desc = f"{type_desc} {desc}"
             type_desc = type_from_default
 
         type_ = _get_type(type_from_default if default_str else type_desc)
         return Argument(arg, type_desc, type_, desc, default_str)
 
 
 def _collect_arguments(arguments: Iterable[str]) -> Iterator[str]:
-    """Combine argument lines to obtain one line per argument"""
+    """
+    Combine argument lines to obtain one line per argument
+        -d, --detach               Detached mode: Run containers in the background,
+        --no-color                 Produce monochrome output.
+    """
     res = ""
     for arg in arguments:
-        if res and arg[:6].strip().startswith("-"):
+        logger.info("arg.strip(): " + arg)
+        if res and arg[:10].strip().startswith("-"):
+            logger.info("single parsed line: " + res.strip())
             yield res.strip()
             res = ""
         res += f"\n   {arg.strip()}"
     if res:
         yield res.strip()
 
 
 def parse_dc_argument(lines: List[str]) -> List[Argument]:
     """
     Parse arguments from lines of `docker compose` specifications
     :param lines: Lines of the Options sections from `docker compose --help`.
     :return: List of arguments
     """
+    logger.info("parse dc argument lines: " + str(lines))
     iter_lines = _collect_arguments(lines)
     return [Argument.from_line(line) for line in iter_lines if "--version" not in line]
 
 
 def _get_type(type_name) -> Type:
     res = _TYPE_CONVERSIONS.get(type_name, None)
     if res is None:
```

### Comparing `docker_composer_v2-0.8.7/src/docker_composer_v2/_utils/generate_class.py` & `docker_composer_v2-0.8.8/src/docker_composer_v2/_utils/generate_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,17 @@
             parts[part].append(line)
     return parts
 
 
 def parse_help(msg: str) -> Tuple[Mapping[str, List[str]], List[Argument]]:
     """Helper function, get sections and arguments from docker-compose <cmd> --help text"""
     sections = collect_help_lines(msg)
+    logger.info('sections["options"]' + str(sections["options"]))
     arguments = parse_dc_argument(sections["options"])
+    logger.info("parsed arguments: " + str(arguments))
     return sections, arguments
 
 
 def _flatten(lists: Iterable[list]):
     """Flatten an iterable of lists"""
     return reduce(add, lists, [])
 
@@ -158,18 +160,21 @@
 def generate_class(class_name: str, cmd: str, level=0) -> str:
     docker_lines = get_help_message(cmd)
     nl = level + 4
     sections, arguments = parse_help(docker_lines)
     cmd_fns = ""
     add_imports: Set[str] = set()
     if "commands" in sections:
-        logger.info("Found commands in section {}", cmd)
-        for cmd_fn, add_import in get_def_commands(sections):
-            cmd_fns += cmd_fn
-            add_imports = add_imports.union(add_import)
+        try:
+            logger.info("Found commands in section {}", cmd)
+            for cmd_fn, add_import in get_def_commands(sections):
+                cmd_fns += cmd_fn
+                add_imports = add_imports.union(add_import)
+        except:  # catching the exception
+            logger.error("StopIteration error")
     args: List[str] = _flatten(list(type_arg(arg)) for arg in arguments)
 
     # List of argument that are options only
     options = ", ".join([f'"{arg.arg}"' for arg in arguments if arg.is_option])
     if options:
         options = options + ","
     new_line = "\n"
```

### Comparing `docker_composer_v2-0.8.7/src/docker_composer_v2/base.py` & `docker_composer_v2-0.8.8/src/docker_composer_v2/base.py`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/build.py` & `docker_composer_v2-0.8.8/src/docker_composer_v2/runner/cmd/port.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,33 +5,23 @@
 
 import attr
 
 from docker_composer_v2.base import DockerBaseRunner
 
 
 @attr.s(auto_attribs=True)
-class DockerComposeBuild(DockerBaseRunner):
+class DockerComposePort(DockerBaseRunner):
     """
 
-    Usage:  docker compose build [OPTIONS] [SERVICE...]
+    Usage:  docker compose port [OPTIONS] SERVICE PRIVATE_PORT
 
-    Build or rebuild services
+    Print the public port for a port binding.
 
     """
 
-    build_arg: Optional[str] = None
-    """Set build-time variables for services.
-       --no-cache                Do not use cache when building the image
-       --progress string         Set type of progress output (auto, tty,
-       plain, quiet) (default "auto")
-       --pull                    Always attempt to pull a newer version of
-       the image.
-       --push                    Push service images."""
-    quiet: Optional[bool] = None
-    """Don't print anything to STDOUT
-       --ssh string              Set SSH authentications used when
-       building service images. (use 'default'
-       for using your default SSH Agent)"""
-    _cmd: str = "build"
-    _options: List[str] = [
-        "quiet",
-    ]
+    index: Optional[int] = None
+    """index of the container if service has multiple
+       replicas (default 1)"""
+    protocol: Optional[str] = None
+    """tcp or udp (default "tcp")"""
+    _cmd: str = "port"
+    _options: List[str] = []
```

### Comparing `docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/cp.py` & `docker_composer_v2-0.8.8/src/docker_composer_v2/runner/cmd/cp.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,16 @@
     Copy files/folders between a service container and the local filesystem
 
     """
 
     archive: Optional[bool] = None
     """Archive mode (copy all uid/gid information)"""
     follow_link: Optional[bool] = None
-    """Always follow symbol link in SRC_PATH
-       --index int     Index of the container if there are multiple
+    """Always follow symbol link in SRC_PATH"""
+    index: Optional[int] = None
+    """Index of the container if there are multiple
        instances of a service ."""
     _cmd: str = "cp"
     _options: List[str] = [
         "archive",
         "follow_link",
     ]
```

### Comparing `docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/down.py` & `docker_composer_v2-0.8.8/src/docker_composer_v2/runner/cmd/down.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,16 +16,17 @@
 
     Stop and remove containers, networks
 
     """
 
     remove_orphans: Optional[bool] = None
     """Remove containers for services not defined in
-       the Compose file.
-       --rmi string        Remove images used by services. "local" remove
+       the Compose file."""
+    rmi: Optional[str] = None
+    """Remove images used by services. "local" remove
        only images that don't have a custom tag
        ("local"|"all")"""
     timeout: Optional[int] = None
     """Specify a shutdown timeout in seconds (default 10)"""
     volumes: Optional[str] = None
     """Remove named volumes declared in the volumes
        section of the Compose file and anonymous
```

### Comparing `docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/events.py` & `docker_composer_v2-0.8.8/src/docker_composer_v2/runner/cmd/events.py`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/images.py` & `docker_composer_v2-0.8.8/src/docker_composer_v2/runner/cmd/images.py`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/kill.py` & `docker_composer_v2-0.8.8/src/docker_composer_v2/runner/cmd/kill.py`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/logs.py` & `docker_composer_v2-0.8.8/src/docker_composer_v2/runner/cmd/pull.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,36 +5,32 @@
 
 import attr
 
 from docker_composer_v2.base import DockerBaseRunner
 
 
 @attr.s(auto_attribs=True)
-class DockerComposeLogs(DockerBaseRunner):
+class DockerComposePull(DockerBaseRunner):
     """
 
-    Usage:  docker compose logs [OPTIONS] [SERVICE...]
+    Usage:  docker compose pull [OPTIONS] [SERVICE...]
 
-    View output from containers
+    Pull service images
 
     """
 
-    follow: Optional[bool] = None
-    """Follow log output.
-       --no-color        Produce monochrome output.
-       --no-log-prefix   Don't print prefix in logs.
-       --since string    Show logs since timestamp (e.g.
-       2013-01-02T13:23:37Z) or relative (e.g. 42m for
-       42 minutes)"""
-    tail: Optional[str] = None
-    """Number of lines to show from the end of the logs
-       for each container. (default "all")"""
-    timestamps: Optional[bool] = None
-    """Show timestamps.
-       --until string    Show logs before a timestamp (e.g.
-       2013-01-02T13:23:37Z) or relative (e.g. 42m for
-       42 minutes)"""
-    _cmd: str = "logs"
+    ignore_buildable: Optional[bool] = None
+    """Ignore images that can be built."""
+    ignore_pull_failures: Optional[bool] = None
+    """Pull what it can and ignores images with
+       pull failures."""
+    include_deps: Optional[bool] = None
+    """Also pull services declared as dependencies."""
+    quiet: Optional[bool] = None
+    """Pull without printing progress information."""
+    _cmd: str = "pull"
     _options: List[str] = [
-        "follow",
-        "timestamps",
+        "ignore_buildable",
+        "ignore_pull_failures",
+        "include_deps",
+        "quiet",
     ]
```

### Comparing `docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/ls.py` & `docker_composer_v2-0.8.8/src/docker_composer_v2/runner/cmd/ls.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,17 +15,19 @@
     Usage:  docker compose ls [OPTIONS]
 
     List running compose projects
 
     """
 
     all: Optional[bool] = None
-    """Show all stopped Compose projects
-       --filter filter   Filter output based on conditions provided.
-       --format string   Format the output. Values: [table | json].
+    """Show all stopped Compose projects"""
+    filter: Optional[str] = None
+    """Filter output based on conditions provided."""
+    format: Optional[str] = None
+    """Format the output. Values: [table | json].
        (default "table")"""
     quiet: Optional[bool] = None
     """Only display IDs."""
     _cmd: str = "ls"
     _options: List[str] = [
         "all",
         "quiet",
```

### Comparing `docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/port.py` & `docker_composer_v2-0.8.8/src/docker_composer_v2/runner/cmd/restart.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,22 +5,24 @@
 
 import attr
 
 from docker_composer_v2.base import DockerBaseRunner
 
 
 @attr.s(auto_attribs=True)
-class DockerComposePort(DockerBaseRunner):
+class DockerComposeRestart(DockerBaseRunner):
     """
 
-    Usage:  docker compose port [OPTIONS] SERVICE PRIVATE_PORT
+    Usage:  docker compose restart [OPTIONS] [SERVICE...]
 
-    Print the public port for a port binding.
+    Restart service containers
 
     """
 
-    index: Optional[int] = None
-    """index of the container if service has multiple
-       replicas (default 1)
-       --protocol string   tcp or udp (default "tcp")"""
-    _cmd: str = "port"
-    _options: List[str] = []
+    no_deps: Optional[bool] = None
+    """Don't restart dependent services."""
+    timeout: Optional[int] = None
+    """Specify a shutdown timeout in seconds (default 10)"""
+    _cmd: str = "restart"
+    _options: List[str] = [
+        "no_deps",
+    ]
```

### Comparing `docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/ps.py` & `docker_composer_v2-0.8.8/src/docker_composer_v2/runner/cmd/ps.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,23 +16,28 @@
 
     List containers
 
     """
 
     all: Optional[bool] = None
     """Show all stopped containers (including those
-       created by the run command)
-       --filter string        Filter services by a property (supported
-       filters: status).
-       --format string        Format the output. Values: [table | json]
+       created by the run command)"""
+    filter: Optional[str] = None
+    """Filter services by a property (supported
+       filters: status)."""
+    format: Optional[str] = None
+    """Format the output. Values: [table | json]
        (default "table")"""
     quiet: Optional[bool] = None
-    """Only display IDs
-       --services             Display services
-       --status stringArray   Filter services by status. Values: [paused |
+    """Only display IDs"""
+    services: Optional[bool] = None
+    """Display services"""
+    status: Optional[str] = None
+    """Filter services by status. Values: [paused |
        restarting | removing | running | dead |
        created | exited]"""
     _cmd: str = "ps"
     _options: List[str] = [
         "all",
         "quiet",
+        "services",
     ]
```

### Comparing `docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/push.py` & `docker_composer_v2-0.8.8/src/docker_composer_v2/runner/cmd/push.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,17 +16,19 @@
 
     Push service images
 
     """
 
     ignore_push_failures: Optional[bool] = None
     """Push what it can and ignores images with
-       push failures
-       --include-deps           Also push images of services declared as
+       push failures"""
+    include_deps: Optional[bool] = None
+    """Also push images of services declared as
        dependencies"""
     quiet: Optional[bool] = None
     """Push without printing progress information"""
     _cmd: str = "push"
     _options: List[str] = [
         "ignore_push_failures",
+        "include_deps",
         "quiet",
     ]
```

### Comparing `docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/restart.py` & `docker_composer_v2-0.8.8/src/docker_composer_v2/runner/cmd/stop.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,24 +5,20 @@
 
 import attr
 
 from docker_composer_v2.base import DockerBaseRunner
 
 
 @attr.s(auto_attribs=True)
-class DockerComposeRestart(DockerBaseRunner):
+class DockerComposeStop(DockerBaseRunner):
     """
 
-    Usage:  docker compose restart [OPTIONS] [SERVICE...]
+    Usage:  docker compose stop [OPTIONS] [SERVICE...]
 
-    Restart service containers
+    Stop services
 
     """
 
-    no_deps: Optional[bool] = None
-    """Don't restart dependent services."""
     timeout: Optional[int] = None
     """Specify a shutdown timeout in seconds (default 10)"""
-    _cmd: str = "restart"
-    _options: List[str] = [
-        "no_deps",
-    ]
+    _cmd: str = "stop"
+    _options: List[str] = []
```

### Comparing `docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/rm.py` & `docker_composer_v2-0.8.8/src/docker_composer_v2/runner/cmd/rm.py`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/run.py` & `docker_composer_v2-0.8.8/src/docker_composer_v2/runner/cmd/create.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,57 +5,43 @@
 
 import attr
 
 from docker_composer_v2.base import DockerBaseRunner
 
 
 @attr.s(auto_attribs=True)
-class DockerComposeRun(DockerBaseRunner):
+class DockerComposeCreate(DockerBaseRunner):
     """
 
-    Usage:  docker compose run [OPTIONS] SERVICE [COMMAND] [ARGS...]
+    Usage:  docker compose create [OPTIONS] [SERVICE...]
 
-    Run a one-off command on a service.
+    Creates containers for a service.
 
     """
 
     build: Optional[bool] = None
-    """Build image before starting container."""
-    detach: Optional[bool] = None
-    """Run container in background and print
-       container ID
-       --entrypoint string     Override the entrypoint of the image"""
-    env: Optional[str] = None
-    """Set environment variables"""
-    interactive: Optional[bool] = None
-    """Keep STDIN open even if not attached.
-       (default true)"""
-    label: Optional[str] = None
-    """Add or override a label
-       --name string           Assign a name to the container"""
-    no_TTY: Optional[bool] = None
-    """Disable pseudo-TTY allocation (default:
-       auto-detected). (default true)
-       --no-deps               Don't start linked services."""
-    publish: Optional[str] = None
-    """Publish a container's port(s) to the host.
-       --quiet-pull            Pull without printing progress information.
-       --remove-orphans        Remove containers for services not defined
-       in the Compose file.
-       --rm                    Automatically remove the container when it exits
-       --service-ports         Run command with the service's ports
-       enabled and mapped to the host.
-       --use-aliases           Use the service's network useAliases in the
-       network(s) the container connects to."""
-    user: Optional[str] = None
-    """Run as specified username or uid"""
-    volume: Optional[str] = None
-    """Bind mount a volume."""
-    workdir: Optional[str] = None
-    """Working directory inside the container"""
-    _cmd: str = "run"
+    """Build images before starting containers."""
+    force_recreate: Optional[bool] = None
+    """Recreate containers even if their configuration
+       and image haven't changed."""
+    no_build: Optional[bool] = None
+    """Don't build an image, even if it's missing."""
+    no_recreate: Optional[bool] = None
+    """If containers already exist, don't recreate
+       them. Incompatible with --force-recreate."""
+    pull: Optional[str] = None
+    """Pull image before running
+       ("always"|"missing"|"never") (default "missing")"""
+    remove_orphans: Optional[bool] = None
+    """Remove containers for services not defined in
+       the Compose file."""
+    scale: Optional[str] = None
+    """Scale SERVICE to NUM instances. Overrides the
+       scale setting in the Compose file if present."""
+    _cmd: str = "create"
     _options: List[str] = [
         "build",
-        "detach",
-        "interactive",
-        "no_TTY",
+        "force_recreate",
+        "no_build",
+        "no_recreate",
+        "remove_orphans",
     ]
```

### Comparing `docker_composer_v2-0.8.7/src/docker_composer_v2/runner/cmd/stop.py` & `docker_composer_v2-0.8.8/src/docker_composer_v2/runner/cmd/version.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,20 +5,25 @@
 
 import attr
 
 from docker_composer_v2.base import DockerBaseRunner
 
 
 @attr.s(auto_attribs=True)
-class DockerComposeStop(DockerBaseRunner):
+class DockerComposeVersion(DockerBaseRunner):
     """
 
-    Usage:  docker compose stop [OPTIONS] [SERVICE...]
+    Usage:  docker compose version [OPTIONS]
 
-    Stop services
+    Show the Docker Compose version information
 
     """
 
-    timeout: Optional[int] = None
-    """Specify a shutdown timeout in seconds (default 10)"""
-    _cmd: str = "stop"
-    _options: List[str] = []
+    format: Optional[str] = None
+    """Format the output. Values: [pretty | json].
+       (Default: pretty)"""
+    short: Optional[bool] = None
+    """Shows only Compose's version number."""
+    _cmd: str = "version"
+    _options: List[str] = [
+        "short",
+    ]
```

### Comparing `docker_composer_v2-0.8.7/src/docker_composer_v2/runner/root.py` & `docker_composer_v2-0.8.8/src/docker_composer_v2/runner/root.py`

 * *Files 27% similar despite different names*

```diff
@@ -42,160 +42,194 @@
     Docker Compose
 
     """
 
     ansi: Optional[str] = None
     """Control when to print ANSI control
        characters ("never"|"always"|"auto")
-       (default "auto")
-       --compatibility              Run compose in backward compatibility mode
-       --env-file stringArray       Specify an alternate environment file."""
+       (default "auto")"""
+    compatibility: Optional[bool] = None
+    """Run compose in backward compatibility mode"""
+    env_file: Optional[str] = None
+    """Specify an alternate environment file."""
     file: Optional[str] = None
-    """Compose configuration files
-       --parallel int               Control max parallelism, -1 for
-       unlimited (default -1)
-       --profile stringArray        Specify a profile to enable
-       --project-directory string   Specify an alternate working directory
+    """Compose configuration files"""
+    parallel: Optional[int] = None
+    """Control max parallelism, -1 for
+       unlimited (default -1)"""
+    profile: Optional[str] = None
+    """Specify a profile to enable"""
+    project_directory: Optional[str] = None
+    """Specify an alternate working directory
        (default: the path of the, first
        specified, Compose file)"""
     project_name: Optional[str] = None
     """Project name"""
     _cmd: str = ""
-    _options: List[str] = []
+    _options: List[str] = [
+        "compatibility",
+    ]
 
     def build(
-        self, build_arg: Optional[str] = None, quiet: Optional[bool] = None
+        self,
+        build_arg: Optional[str] = None,
+        no_cache: Optional[bool] = None,
+        progress: Optional[str] = None,
+        pull: Optional[bool] = None,
+        push: Optional[bool] = None,
+        quiet: Optional[bool] = None,
+        ssh: Optional[str] = None,
     ) -> docker_composer_v2.runner.cmd.build.DockerComposeBuild:
         """
 
         Usage:  docker compose build [OPTIONS] [SERVICE...]
 
         Build or rebuild services
 
 
         :param build_arg: Set build-time variables for services.
-           --no-cache                Do not use cache when building the image
-           --progress string         Set type of progress output (auto, tty,
+        :param no_cache: Do not use cache when building the image
+        :param progress: Set type of progress output (auto, tty,
            plain, quiet) (default "auto")
-           --pull                    Always attempt to pull a newer version of
+        :param pull: Always attempt to pull a newer version of
            the image.
-           --push                    Push service images.
+        :param push: Push service images.
         :param quiet: Don't print anything to STDOUT
-           --ssh string              Set SSH authentications used when
+        :param ssh: Set SSH authentications used when
            building service images. (use 'default'
            for using your default SSH Agent)
         """
         runner = docker_composer_v2.runner.cmd.build.DockerComposeBuild(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def config(
         self,
         format: Optional[str] = None,
+        hash: Optional[str] = None,
+        images: Optional[bool] = None,
+        no_consistency: Optional[bool] = None,
+        no_interpolate: Optional[bool] = None,
+        no_normalize: Optional[bool] = None,
         output: Optional[str] = None,
+        profiles: Optional[bool] = None,
         quiet: Optional[bool] = None,
+        resolve_image_digests: Optional[bool] = None,
+        services: Optional[bool] = None,
+        volumes: Optional[bool] = None,
     ) -> docker_composer_v2.runner.cmd.config.DockerComposeConfig:
         """
 
         Usage:  docker compose config [OPTIONS] [SERVICE...]
 
         Parse, resolve and render compose file in canonical format
 
 
         :param format: Format the output. Values: [yaml | json]
            (default "yaml")
-           --hash string             Print the service config hash, one per line.
-           --images                  Print the image names, one per line.
-           --no-consistency          Don't check model consistency - warning:
+        :param hash: Print the service config hash, one per line.
+        :param images: Print the image names, one per line.
+        :param no_consistency: Don't check model consistency - warning:
            may produce invalid Compose output
-           --no-interpolate          Don't interpolate environment variables.
-           --no-normalize            Don't normalize compose model.
+        :param no_interpolate: Don't interpolate environment variables.
+        :param no_normalize: Don't normalize compose model.
         :param output: Save to file (default to stdout)
-           --profiles                Print the profile names, one per line.
+        :param profiles: Print the profile names, one per line.
         :param quiet: Only validate the configuration, don't
            print anything.
-           --resolve-image-digests   Pin image tags to digests.
-           --services                Print the service names, one per line.
-           --volumes                 Print the volume names, one per line.
+        :param resolve_image_digests: Pin image tags to digests.
+        :param services: Print the service names, one per line.
+        :param volumes: Print the volume names, one per line.
         """
         runner = docker_composer_v2.runner.cmd.config.DockerComposeConfig(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def cp(
-        self, archive: Optional[bool] = None, follow_link: Optional[bool] = None
+        self,
+        archive: Optional[bool] = None,
+        follow_link: Optional[bool] = None,
+        index: Optional[int] = None,
     ) -> docker_composer_v2.runner.cmd.cp.DockerComposeCp:
         """
 
         Usage:  docker compose cp [OPTIONS] SERVICE:SRC_PATH DEST_PATH|-
                 docker compose cp [OPTIONS] SRC_PATH|- SERVICE:DEST_PATH
 
         Copy files/folders between a service container and the local filesystem
 
 
         :param archive: Archive mode (copy all uid/gid information)
         :param follow_link: Always follow symbol link in SRC_PATH
-           --index int     Index of the container if there are multiple
+        :param index: Index of the container if there are multiple
            instances of a service .
         """
         runner = docker_composer_v2.runner.cmd.cp.DockerComposeCp(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def create(
-        self, build: Optional[bool] = None
+        self,
+        build: Optional[bool] = None,
+        force_recreate: Optional[bool] = None,
+        no_build: Optional[bool] = None,
+        no_recreate: Optional[bool] = None,
+        pull: Optional[str] = None,
+        remove_orphans: Optional[bool] = None,
+        scale: Optional[str] = None,
     ) -> docker_composer_v2.runner.cmd.create.DockerComposeCreate:
         """
 
         Usage:  docker compose create [OPTIONS] [SERVICE...]
 
         Creates containers for a service.
 
 
         :param build: Build images before starting containers.
-           --force-recreate   Recreate containers even if their configuration
+        :param force_recreate: Recreate containers even if their configuration
            and image haven't changed.
-           --no-build         Don't build an image, even if it's missing.
-           --no-recreate      If containers already exist, don't recreate
+        :param no_build: Don't build an image, even if it's missing.
+        :param no_recreate: If containers already exist, don't recreate
            them. Incompatible with --force-recreate.
-           --pull string      Pull image before running
+        :param pull: Pull image before running
            ("always"|"missing"|"never") (default "missing")
-           --remove-orphans   Remove containers for services not defined in
+        :param remove_orphans: Remove containers for services not defined in
            the Compose file.
-           --scale scale      Scale SERVICE to NUM instances. Overrides the
+        :param scale: Scale SERVICE to NUM instances. Overrides the
            scale setting in the Compose file if present.
         """
         runner = docker_composer_v2.runner.cmd.create.DockerComposeCreate(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def down(
         self,
         remove_orphans: Optional[bool] = None,
+        rmi: Optional[str] = None,
         timeout: Optional[int] = None,
         volumes: Optional[str] = None,
     ) -> docker_composer_v2.runner.cmd.down.DockerComposeDown:
         """
 
         Usage:  docker compose down [OPTIONS]
 
         Stop and remove containers, networks
 
 
         :param remove_orphans: Remove containers for services not defined in
            the Compose file.
-           --rmi string        Remove images used by services. "local" remove
+        :param rmi: Remove images used by services. "local" remove
            only images that don't have a custom tag
            ("local"|"all")
         :param timeout: Specify a shutdown timeout in seconds (default 10)
         :param volumes: Remove named volumes declared in the volumes
            section of the Compose file and anonymous
            volumes attached to containers.
         """
@@ -223,35 +257,37 @@
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def exec(
         self,
         detach: Optional[bool] = None,
         env: Optional[str] = None,
+        index: Optional[int] = None,
         no_TTY: Optional[str] = None,
+        privileged: Optional[bool] = None,
         user: Optional[str] = None,
         workdir: Optional[str] = None,
     ) -> docker_composer_v2.runner.cmd.exec.DockerComposeExec:
         """
 
         Usage:  docker compose exec [OPTIONS] SERVICE COMMAND [ARGS...]
 
         Execute a command in a running container.
 
 
         :param detach: Detached mode: Run command in the
            background.
         :param env: Set environment variables
-           --index int                    index of the container if there are
+        :param index: index of the container if there are
            multiple instances of a service
            [default: 1]. (default 1)
         :param no_TTY: Disable pseudo-TTY allocation. By
            default docker compose exec
            allocates a TTY. (default true)
-           --privileged                   Give extended privileges to the process.
+        :param privileged: Give extended privileges to the process.
         :param user: Run the command as this user.
         :param workdir: Path to workdir directory for this
            command.
         """
         runner = docker_composer_v2.runner.cmd.exec.DockerComposeExec(
             **{k: v for k, v in locals().items() if k != "self"}
         )
@@ -297,56 +333,64 @@
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def logs(
         self,
         follow: Optional[bool] = None,
+        no_color: Optional[bool] = None,
+        no_log_prefix: Optional[bool] = None,
+        since: Optional[str] = None,
         tail: Optional[str] = None,
         timestamps: Optional[bool] = None,
+        until: Optional[str] = None,
     ) -> docker_composer_v2.runner.cmd.logs.DockerComposeLogs:
         """
 
         Usage:  docker compose logs [OPTIONS] [SERVICE...]
 
         View output from containers
 
 
         :param follow: Follow log output.
-           --no-color        Produce monochrome output.
-           --no-log-prefix   Don't print prefix in logs.
-           --since string    Show logs since timestamp (e.g.
+        :param no_color: Produce monochrome output.
+        :param no_log_prefix: Don't print prefix in logs.
+        :param since: Show logs since timestamp (e.g.
            2013-01-02T13:23:37Z) or relative (e.g. 42m for
            42 minutes)
         :param tail: Number of lines to show from the end of the logs
            for each container. (default "all")
         :param timestamps: Show timestamps.
-           --until string    Show logs before a timestamp (e.g.
+        :param until: Show logs before a timestamp (e.g.
            2013-01-02T13:23:37Z) or relative (e.g. 42m for
            42 minutes)
         """
         runner = docker_composer_v2.runner.cmd.logs.DockerComposeLogs(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def ls(
-        self, all: Optional[bool] = None, quiet: Optional[bool] = None
+        self,
+        all: Optional[bool] = None,
+        filter: Optional[str] = None,
+        format: Optional[str] = None,
+        quiet: Optional[bool] = None,
     ) -> docker_composer_v2.runner.cmd.ls.DockerComposeLs:
         """
 
         Usage:  docker compose ls [OPTIONS]
 
         List running compose projects
 
 
         :param all: Show all stopped Compose projects
-           --filter filter   Filter output based on conditions provided.
-           --format string   Format the output. Values: [table | json].
+        :param filter: Filter output based on conditions provided.
+        :param format: Format the output. Values: [table | json].
            (default "table")
         :param quiet: Only display IDs.
         """
         runner = docker_composer_v2.runner.cmd.ls.DockerComposeLs(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
@@ -367,96 +411,109 @@
         runner = docker_composer_v2.runner.cmd.pause.DockerComposePause(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def port(
-        self, index: Optional[int] = None
+        self, index: Optional[int] = None, protocol: Optional[str] = None
     ) -> docker_composer_v2.runner.cmd.port.DockerComposePort:
         """
 
         Usage:  docker compose port [OPTIONS] SERVICE PRIVATE_PORT
 
         Print the public port for a port binding.
 
 
         :param index: index of the container if service has multiple
            replicas (default 1)
-           --protocol string   tcp or udp (default "tcp")
+        :param protocol: tcp or udp (default "tcp")
         """
         runner = docker_composer_v2.runner.cmd.port.DockerComposePort(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def ps(
-        self, all: Optional[bool] = None, quiet: Optional[bool] = None
+        self,
+        all: Optional[bool] = None,
+        filter: Optional[str] = None,
+        format: Optional[str] = None,
+        quiet: Optional[bool] = None,
+        services: Optional[bool] = None,
+        status: Optional[str] = None,
     ) -> docker_composer_v2.runner.cmd.ps.DockerComposePs:
         """
 
         Usage:  docker compose ps [OPTIONS] [SERVICE...]
 
         List containers
 
 
         :param all: Show all stopped containers (including those
            created by the run command)
-           --filter string        Filter services by a property (supported
+        :param filter: Filter services by a property (supported
            filters: status).
-           --format string        Format the output. Values: [table | json]
+        :param format: Format the output. Values: [table | json]
            (default "table")
         :param quiet: Only display IDs
-           --services             Display services
-           --status stringArray   Filter services by status. Values: [paused |
+        :param services: Display services
+        :param status: Filter services by status. Values: [paused |
            restarting | removing | running | dead |
            created | exited]
         """
         runner = docker_composer_v2.runner.cmd.ps.DockerComposePs(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def pull(
-        self, ignore_buildable: Optional[bool] = None, quiet: Optional[bool] = None
+        self,
+        ignore_buildable: Optional[bool] = None,
+        ignore_pull_failures: Optional[bool] = None,
+        include_deps: Optional[bool] = None,
+        quiet: Optional[bool] = None,
     ) -> docker_composer_v2.runner.cmd.pull.DockerComposePull:
         """
 
         Usage:  docker compose pull [OPTIONS] [SERVICE...]
 
         Pull service images
 
 
         :param ignore_buildable: Ignore images that can be built.
-           --ignore-pull-failures   Pull what it can and ignores images with
+        :param ignore_pull_failures: Pull what it can and ignores images with
            pull failures.
-           --include-deps           Also pull services declared as dependencies.
+        :param include_deps: Also pull services declared as dependencies.
         :param quiet: Pull without printing progress information.
         """
         runner = docker_composer_v2.runner.cmd.pull.DockerComposePull(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def push(
-        self, ignore_push_failures: Optional[bool] = None, quiet: Optional[bool] = None
+        self,
+        ignore_push_failures: Optional[bool] = None,
+        include_deps: Optional[bool] = None,
+        quiet: Optional[bool] = None,
     ) -> docker_composer_v2.runner.cmd.push.DockerComposePush:
         """
 
         Usage:  docker compose push [OPTIONS] [SERVICE...]
 
         Push service images
 
 
         :param ignore_push_failures: Push what it can and ignores images with
            push failures
-           --include-deps           Also push images of services declared as
+        :param include_deps: Also push images of services declared as
            dependencies
         :param quiet: Push without printing progress information
         """
         runner = docker_composer_v2.runner.cmd.push.DockerComposePush(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
@@ -509,50 +566,58 @@
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def run(
         self,
         build: Optional[bool] = None,
         detach: Optional[bool] = None,
+        entrypoint: Optional[str] = None,
         env: Optional[str] = None,
         interactive: Optional[bool] = None,
         label: Optional[str] = None,
+        name: Optional[str] = None,
         no_TTY: Optional[bool] = None,
+        no_deps: Optional[bool] = None,
         publish: Optional[str] = None,
+        quiet_pull: Optional[bool] = None,
+        remove_orphans: Optional[bool] = None,
+        rm: Optional[bool] = None,
+        service_ports: Optional[bool] = None,
+        use_aliases: Optional[bool] = None,
         user: Optional[str] = None,
         volume: Optional[str] = None,
         workdir: Optional[str] = None,
     ) -> docker_composer_v2.runner.cmd.run.DockerComposeRun:
         """
 
         Usage:  docker compose run [OPTIONS] SERVICE [COMMAND] [ARGS...]
 
         Run a one-off command on a service.
 
 
         :param build: Build image before starting container.
         :param detach: Run container in background and print
            container ID
-           --entrypoint string     Override the entrypoint of the image
+        :param entrypoint: Override the entrypoint of the image
         :param env: Set environment variables
         :param interactive: Keep STDIN open even if not attached.
            (default true)
         :param label: Add or override a label
-           --name string           Assign a name to the container
+        :param name: Assign a name to the container
         :param no_TTY: Disable pseudo-TTY allocation (default:
            auto-detected). (default true)
-           --no-deps               Don't start linked services.
+        :param no_deps: Don't start linked services.
         :param publish: Publish a container's port(s) to the host.
-           --quiet-pull            Pull without printing progress information.
-           --remove-orphans        Remove containers for services not defined
+        :param quiet_pull: Pull without printing progress information.
+        :param remove_orphans: Remove containers for services not defined
            in the Compose file.
-           --rm                    Automatically remove the container when it exits
-           --service-ports         Run command with the service's ports
+        :param rm: Automatically remove the container when it exits
+        :param service_ports: Run command with the service's ports
            enabled and mapped to the host.
-           --use-aliases           Use the service's network useAliases in the
+        :param use_aliases: Use the service's network useAliases in the
            network(s) the container connects to.
         :param user: Run as specified username or uid
         :param volume: Bind mount a volume.
         :param workdir: Working directory inside the container
         """
         runner = docker_composer_v2.runner.cmd.run.DockerComposeRun(
             **{k: v for k, v in locals().items() if k != "self"}
@@ -631,89 +696,109 @@
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def up(
         self,
         abort_on_container_exit: Optional[bool] = None,
+        always_recreate_deps: Optional[bool] = None,
+        attach: Optional[str] = None,
+        attach_dependencies: Optional[bool] = None,
+        build: Optional[bool] = None,
         detach: Optional[bool] = None,
+        exit_code_from: Optional[str] = None,
+        force_recreate: Optional[bool] = None,
+        no_attach: Optional[str] = None,
+        no_build: Optional[bool] = None,
+        no_color: Optional[bool] = None,
+        no_deps: Optional[bool] = None,
+        no_log_prefix: Optional[bool] = None,
+        no_recreate: Optional[bool] = None,
+        no_start: Optional[bool] = None,
+        pull: Optional[str] = None,
+        quiet_pull: Optional[bool] = None,
+        remove_orphans: Optional[bool] = None,
         renew_anon_volumes: Optional[bool] = None,
+        scale: Optional[str] = None,
+        timestamps: Optional[bool] = None,
+        wait: Optional[bool] = None,
+        wait_timeout: Optional[int] = None,
         waitTimeout: Optional[int] = None,
     ) -> docker_composer_v2.runner.cmd.up.DockerComposeUp:
         """
 
         Usage:  docker compose up [OPTIONS] [SERVICE...]
 
         Create and start containers
 
 
         :param abort_on_container_exit: Stops all containers if any container
            was stopped. Incompatible with -d
-           --always-recreate-deps      Recreate dependent containers.
+        :param always_recreate_deps: Recreate dependent containers.
            Incompatible with --no-recreate.
-           --attach stringArray        Attach to service output.
-           --attach-dependencies       Attach to dependent containers.
-           --build                     Build images before starting containers.
+        :param attach: Attach to service output.
+        :param attach_dependencies: Attach to dependent containers.
+        :param build: Build images before starting containers.
         :param detach: Detached mode: Run containers in the
            background
-           --exit-code-from string     Return the exit code of the selected
+        :param exit_code_from: Return the exit code of the selected
            service container. Implies
            --abort-on-container-exit
-           --force-recreate            Recreate containers even if their
+        :param force_recreate: Recreate containers even if their
            configuration and image haven't changed.
-           --no-attach stringArray     Don't attach to specified service.
-           --no-build                  Don't build an image, even if it's missing.
-           --no-color                  Produce monochrome output.
-           --no-deps                   Don't start linked services.
-           --no-log-prefix             Don't print prefix in logs.
-           --no-recreate               If containers already exist, don't
+        :param no_attach: Don't attach to specified service.
+        :param no_build: Don't build an image, even if it's missing.
+        :param no_color: Produce monochrome output.
+        :param no_deps: Don't start linked services.
+        :param no_log_prefix: Don't print prefix in logs.
+        :param no_recreate: If containers already exist, don't
            recreate them. Incompatible with
            --force-recreate.
-           --no-start                  Don't start the services after creating
+        :param no_start: Don't start the services after creating
            them.
-           --pull string               Pull image before running
+        :param pull: Pull image before running
            ("always"|"missing"|"never") (default
            "missing")
-           --quiet-pull                Pull without printing progress information.
-           --remove-orphans            Remove containers for services not
+        :param quiet_pull: Pull without printing progress information.
+        :param remove_orphans: Remove containers for services not
            defined in the Compose file.
         :param renew_anon_volumes: Recreate anonymous volumes instead of
            retrieving data from the previous
            containers.
-           --scale scale               Scale SERVICE to NUM instances.
+        :param scale: Scale SERVICE to NUM instances.
            Overrides the scale setting in the
            Compose file if present.
-           --timestamps                Show timestamps.
-           --wait                      Wait for services to be
+        :param timestamps: Show timestamps.
+        :param wait: Wait for services to be
            running|healthy. Implies detached mode.
-           --wait-timeout int          timeout waiting for application to be
+        :param wait_timeout: timeout waiting for application to be
            running|healthy.
         :param waitTimeout: Use this waitTimeout in seconds for
            container shutdown when attached or
            when containers are already running.
            (default 10)
         """
         runner = docker_composer_v2.runner.cmd.up.DockerComposeUp(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
 
     def version(
-        self, format: Optional[str] = None
+        self, format: Optional[str] = None, short: Optional[bool] = None
     ) -> docker_composer_v2.runner.cmd.version.DockerComposeVersion:
         """
 
         Usage:  docker compose version [OPTIONS]
 
         Show the Docker Compose version information
 
 
         :param format: Format the output. Values: [pretty | json].
            (Default: pretty)
-           --short           Shows only Compose's version number.
+        :param short: Shows only Compose's version number.
         """
         runner = docker_composer_v2.runner.cmd.version.DockerComposeVersion(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
```

### Comparing `docker_composer_v2-0.8.7/PKG-INFO` & `docker_composer_v2-0.8.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-composer-v2
-Version: 0.8.7
+Version: 0.8.8
 Summary: Use `docker compose` from within Python. This is a branch forked from https://github.com/schollm/docker-composer to support Docker Compose V2.
 Home-page: https://github.com/jensenkairos/docker-composer-v2
 License: Apache-2.0
 Author: Micha
 Author-email: schollm-git@gmx.com
 Requires-Python: >=3.6,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -40,15 +40,15 @@
 
 ## Install
 ```shell script
 pip install docker-composer-v2
 ```
 
 ## Usage
-The main class is `docker_compose_v2r.DockerCompose`. Its parameters are
+The main class is `docker_composer_v2.DockerCompose`. Its parameters are
 all options from `docker compose`.
 
 Each `docker compose` subcommand has a corresponding function, e.g. 
 `DockerCompose.run` or `DockerCompose.scale`. Their arguments again mirror 
 the options of the corresponding command.
 
 The resulting object has a `call` function.
```

