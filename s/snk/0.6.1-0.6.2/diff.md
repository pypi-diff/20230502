# Comparing `tmp/snk-0.6.1.tar.gz` & `tmp/snk-0.6.2.tar.gz`

## Comparing `snk-0.6.1.tar` & `snk-0.6.2.tar`

### file list

```diff
@@ -1,42 +1,44 @@
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 snk-0.6.1/Dockerfile
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 snk-0.6.1/mkdocs.yml
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 snk-0.6.1/.github/workflows/mkdocs.yml
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 snk-0.6.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 snk-0.6.1/.github/workflows/tests.yml
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 snk-0.6.1/docs/CNAME
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 snk-0.6.1/docs/index.md
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 snk-0.6.1/docs/reference/cli.md
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 snk-0.6.1/docs/reference/errors.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snk-0.6.1/docs/reference/main.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snk-0.6.1/docs/reference/nest.md
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 snk-0.6.1/snk/__about__.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 snk-0.6.1/snk/__init__.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 snk-0.6.1/snk/errors.py
--rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 snk-0.6.1/snk/main.py
--rw-r--r--   0        0        0    14897 2020-02-02 00:00:00.000000 snk-0.6.1/snk/nest.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 snk-0.6.1/snk/cli/__init__.py
--rw-r--r--   0        0        0    14687 2020-02-02 00:00:00.000000 snk-0.6.1/snk/cli/cli.py
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 snk-0.6.1/snk/cli/config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snk-0.6.1/snk/cli/options.py
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 snk-0.6.1/snk/cli/pipeline.py
--rw-r--r--   0        0        0     8485 2020-02-02 00:00:00.000000 snk-0.6.1/snk/cli/utils.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 snk-0.6.1/tests/.DS_Store
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snk-0.6.1/tests/__init__.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 snk-0.6.1/tests/conftest.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 snk-0.6.1/tests/test_nest.py
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 snk-0.6.1/tests/test_pipline_cli.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 snk-0.6.1/tests/test_snk.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 snk-0.6.1/tests/utils.py
--rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 snk-0.6.1/tests/data/artic_v4.1.bed
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 snk-0.6.1/tests/data/config.yaml
--rw-r--r--   0        0        0   242003 2020-02-02 00:00:00.000000 snk-0.6.1/tests/data/cov.fasta
--rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 snk-0.6.1/tests/data/bin/snk-basic-pipeline
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 snk-0.6.1/tests/data/pipeline/.snk
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 snk-0.6.1/tests/data/pipeline/Snakefile
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 snk-0.6.1/tests/data/pipeline/config.yaml
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 snk-0.6.1/tests/data/pipeline/profiles/base/config.yaml
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 snk-0.6.1/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 snk-0.6.1/LICENSE.txt
--rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 snk-0.6.1/README.md
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 snk-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 snk-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 snk-0.6.2/Dockerfile
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 snk-0.6.2/mkdocs.yml
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 snk-0.6.2/.github/workflows/mkdocs.yml
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 snk-0.6.2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 snk-0.6.2/.github/workflows/tests.yml
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 snk-0.6.2/docs/CNAME
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 snk-0.6.2/docs/index.md
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 snk-0.6.2/docs/reference/cli.md
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 snk-0.6.2/docs/reference/errors.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snk-0.6.2/docs/reference/main.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snk-0.6.2/docs/reference/nest.md
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 snk-0.6.2/snk/__about__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 snk-0.6.2/snk/__init__.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 snk-0.6.2/snk/errors.py
+-rw-r--r--   0        0        0     5549 2020-02-02 00:00:00.000000 snk-0.6.2/snk/main.py
+-rw-r--r--   0        0        0    15537 2020-02-02 00:00:00.000000 snk-0.6.2/snk/nest.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 snk-0.6.2/snk/cli/__init__.py
+-rw-r--r--   0        0        0    16338 2020-02-02 00:00:00.000000 snk-0.6.2/snk/cli/cli.py
+-rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 snk-0.6.2/snk/cli/config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snk-0.6.2/snk/cli/options.py
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 snk-0.6.2/snk/cli/pipeline.py
+-rw-r--r--   0        0        0     8630 2020-02-02 00:00:00.000000 snk-0.6.2/snk/cli/utils.py
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 snk-0.6.2/tests/.DS_Store
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snk-0.6.2/tests/__init__.py
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 snk-0.6.2/tests/conftest.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 snk-0.6.2/tests/test_nest.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 snk-0.6.2/tests/test_pipline_cli.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 snk-0.6.2/tests/test_snk.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 snk-0.6.2/tests/utils.py
+-rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 snk-0.6.2/tests/data/artic_v4.1.bed
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 snk-0.6.2/tests/data/config.yaml
+-rw-r--r--   0        0        0   242003 2020-02-02 00:00:00.000000 snk-0.6.2/tests/data/cov.fasta
+-rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 snk-0.6.2/tests/data/bin/snk-basic-pipeline
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 snk-0.6.2/tests/data/pipeline/.snk
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 snk-0.6.2/tests/data/pipeline/cli.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 snk-0.6.2/tests/data/pipeline/config.yaml
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 snk-0.6.2/tests/data/pipeline/workflow/Snakefile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snk-0.6.2/tests/data/pipeline/workflow/envs/base.yml
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 snk-0.6.2/tests/data/pipeline/workflow/profiles/base/config.yaml
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 snk-0.6.2/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 snk-0.6.2/LICENSE.txt
+-rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 snk-0.6.2/README.md
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 snk-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 snk-0.6.2/PKG-INFO
```

### Comparing `snk-0.6.1/mkdocs.yml` & `snk-0.6.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `snk-0.6.1/.github/workflows/publish.yml` & `snk-0.6.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `snk-0.6.1/.github/workflows/tests.yml` & `snk-0.6.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `snk-0.6.1/docs/index.md` & `snk-0.6.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `snk-0.6.1/snk/main.py` & `snk-0.6.2/snk/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from .errors import PipelineExistsError, PipelineNotFoundError
 
 app = typer.Typer()
 
 SNK_HOME = None
 SNK_BIN = None
 
+# fmt: off
 @app.callback(context_settings={"help_option_names": ["-h", "--help"]})
 def callback(
     home: Optional[Path] = typer.Option(
             None, 
             envvar="SNK_HOME", 
             dir_okay=True, 
             file_okay=False, 
@@ -45,110 +46,128 @@
  \b
  \n
  Snakemake pipeline management system
     """
     global SNK_BIN, SNK_HOME
     SNK_BIN = bin
     SNK_HOME = home
-    
+# fmt: on
 
 
 @app.command()
 def install(
-        pipeline: str = typer.Argument(
-            ..., help="Path, URL or Github name (user/repo) of the pipeline to install."
-        ),
-        name: Optional[str] = typer.Option(
-            None, 
-            help="Rename the pipeline (this name will be used to call the CLI.)"
-        ),
-        tag: Optional[str] = typer.Option(
-            None,
-            "--tag",
-            "-t",
-            help="Tag (version) of the pipeline to install. Can specify a branch name, or tag. If None the latest commit will be installed."
-        ),
-        config: Optional[Path] = typer.Option(
-            None, 
-            help="Specify a non-standard config location."
-        ),
-        resource: Optional[List[Path]] = typer.Option(
-            [], 
-            help="Specify a resource required to run the pipeline (copied to working dir at runtime)."
-        ),
-        editable: Optional[bool] = typer.Option(False, '--editable', '-e', help="Force uninstall without asking."),
-    ):
+    pipeline: str = typer.Argument(
+        ..., help="Path, URL or Github name (user/repo) of the pipeline to install."
+    ),
+    name: Optional[str] = typer.Option(
+        None, help="Rename the pipeline (this name will be used to call the CLI.)"
+    ),
+    tag: Optional[str] = typer.Option(
+        None,
+        "--tag",
+        "-t",
+        help="Tag (version) of the pipeline to install. Can specify a branch name, or tag. If None the latest commit will be installed.",
+    ),
+    config: Optional[Path] = typer.Option(
+        None, help="Specify a non-standard config location."
+    ),
+    resource: Optional[List[Path]] = typer.Option(
+        [],
+        help="Specify a resource required to run the pipeline (copied to working dir at runtime).",
+    ),
+    force: Optional[bool] = typer.Option(
+        False, "--force", "-f", help="Force install (overwrites existing installs)."
+    ),
+    editable: Optional[bool] = typer.Option(
+        False, "--editable", "-e", help="Whether to install the pipeline in editable mode."
+    ),
+):
     """
     Install a pipeline.
     """
+    global SNK_BIN, SNK_HOME
     nest = Nest(snk_home=SNK_HOME, bin_dir=SNK_BIN)
     if not nest.bin_dir_in_path():
         bin_dir_yellow = typer.style(nest.bin_dir, fg=typer.colors.YELLOW, bold=False)
         typer.echo(f"Please add SNK_BIN to your $PATH: {bin_dir_yellow}")
-    if not Path(pipeline).exists() and not pipeline.startswith('http'):
+    if not Path(pipeline).exists() and not pipeline.startswith("http"):
         pipeline = f"https://github.com/{pipeline}.git"
     try:
-        installed_pipeline = nest.install(pipeline, editable=editable, name=name, tag=tag, config=config, resources=resource)
+        installed_pipeline = nest.install(
+            pipeline,
+            editable=editable,
+            name=name,
+            tag=tag,
+            config=config,
+            resources=resource,
+            force=force
+        )
     except PipelineExistsError as e:
-        typer.secho(e, fg='red')
+        typer.secho(e, fg="red")
         raise typer.Exit()
     except PipelineNotFoundError as e:
-        typer.secho(e, fg='red')
+        typer.secho(e, fg="red")
         raise typer.Exit()
     v = installed_pipeline.version
-    v = v if v else 'latest'
-    typer.secho(f"Successfully installed {installed_pipeline.name} ({v})!", fg='green')
+    v = v if v else "latest"
+    typer.secho(f"Successfully installed {installed_pipeline.name} ({v})!", fg="green")
 
 
 @app.command()
 def uninstall(
-        name: str = typer.Argument(..., help="Name of the pipeline to uninstall."),
-        force: Optional[bool] = typer.Option(False, '--force', '-f', help="Force uninstall without asking."),
-    ):
+    name: str = typer.Argument(..., help="Name of the pipeline to uninstall."),
+    force: Optional[bool] = typer.Option(
+        False, "--force", "-f", help="Force uninstall without asking."
+    ),
+):
     """
     Uninstall a pipeline.
     """
+    global SNK_BIN, SNK_HOME
     nest = Nest(snk_home=SNK_HOME, bin_dir=SNK_BIN)
     try:
         uninstalled = nest.uninstall(name, force=force)
     except PipelineNotFoundError as e:
-        typer.secho(e, fg='red')
+        typer.secho(e, fg="red")
         raise typer.Exit(1)
     if uninstalled:
-        typer.secho(f"Successfully uninstalled {name}!", fg='green')
-        
+        typer.secho(f"Successfully uninstalled {name}!", fg="green")
+
 
 # @app.command()
 # def update():
 #     """
 #     Update a pipeline.
 #     """
 #     raise NotImplementedError
 
 
 @app.command()
 def list():
     """
     List the installed pipelines.
     """
-    nest = Nest()
+    global SNK_BIN, SNK_HOME
+    nest = Nest(snk_home=SNK_HOME, bin_dir=SNK_BIN)
     try:
         pipelines = nest.pipelines
     except FileNotFoundError:
         pipelines = []
-    pipeline_dir_yellow = typer.style(nest.pipelines_dir, fg=typer.colors.YELLOW, bold=False)
+    pipeline_dir_yellow = typer.style(
+        nest.pipelines_dir, fg=typer.colors.YELLOW, bold=False
+    )
     typer.echo(f"Found {len(pipelines)} pipelines in {pipeline_dir_yellow}")
     for pipeline in pipelines:
         v = pipeline.version
-        v = v if v else 'latest'
+        v = v if v else "latest"
         typer.echo(f"- {pipeline.name} ({v})")
 
 
 # @app.command()
-# def run(        
+# def run(
 #         pipeline: str = typer.Argument(
 #             ..., help="URL or Github name (user/repo) of the pipeline to install."
 #         ),
 #     ):
 #     """
 #     Run the pipeline in a temporary environment.
 #     """
@@ -158,8 +177,8 @@
 # def annotations(config: Path):
 #     """Generate annotations defaults from config file"""
 #     raise NotImplementedError
 
 # @app.command()
 # def create(name: str):
 #     """Create a default project that can be installed with snk"""
-#     raise NotImplementedError
+#     raise NotImplementedError
```

### Comparing `snk-0.6.1/snk/nest.py` & `snk-0.6.2/snk/nest.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,19 @@
 import stat
 import inspect
 import os
 from typing import List
 import shutil
 import yaml
 
-from .errors import PipelineExistsError, PipelineNotFoundError, InvalidPipelineRepositoryError
+from .errors import (
+    PipelineExistsError,
+    PipelineNotFoundError,
+    InvalidPipelineRepositoryError,
+)
 from .cli.config import SnkConfig
 from .cli.pipeline import Pipeline
 
 
 class Nest:
     """
     Initializes a Nest object.
@@ -32,59 +36,70 @@
           snk_home (Path, optional): The path to the SNK home directory. Defaults to None.
           bin_dir (Path, optional): The path to the bin directory. Defaults to None.
         Side Effects:
           Creates the SNK home and bin directories if they do not exist.
         Examples:
           >>> nest = Nest()
         """
-        self.python_interpreter_path = Path(sys.executable) # needs to be the same python that has snk
-        
+        self.python_interpreter_path = Path(
+            sys.executable
+        )  # needs to be the same python that has snk
+
         if not snk_home:
             home_path = self.python_interpreter_path.parent.parent
             if not os.access(home_path, os.W_OK):
-                user_home_path = Path('~').expanduser()
-                snk_home = user_home_path / ".local" / 'snk'
+                user_home_path = Path("~").expanduser()
+                snk_home = user_home_path / ".local" / "snk"
             else:
-                snk_home = home_path / 'snk'
+                snk_home = home_path / "snk"
 
         if not bin_dir:
             bin_dir = self.python_interpreter_path.parent
             if not os.access(bin_dir, os.W_OK):
-                user_home_path = Path('~').expanduser()
-                bin_dir = user_home_path / ".local" / 'bin'
+                user_home_path = Path("~").expanduser()
+                bin_dir = user_home_path / ".local" / "bin"
 
         self.snk_home = Path(snk_home).absolute()
         self.pipelines_dir = self.snk_home / "pipelines"
         self.bin_dir = Path(bin_dir).absolute()
-        
+
         # Create dirs
         self.snk_home.mkdir(parents=True, exist_ok=True)
         self.pipelines_dir.mkdir(parents=True, exist_ok=True)
         self.bin_dir.mkdir(parents=True, exist_ok=True)
 
     def bin_dir_in_path(self) -> bool:
-        path_dirs = os.environ['PATH'].split(os.pathsep)
+        path_dirs = os.environ["PATH"].split(os.pathsep)
         return str(self.bin_dir) in path_dirs
 
     def _check_repo_url_format(self, repo: str):
         """
         Checks that the given repo URL is valid.
         Args:
           repo (str): The URL of the repo.
         Raises:
           InvalidPipelineRepositoryError: If the repo URL is not valid.
         Examples:
           >>> nest._check_repo_url_format('https://github.com/example/repo.git')
         """
-        if not repo.startswith('http'):
-            raise InvalidPipelineRepositoryError('Repo url must start with http')
-        if not repo.endswith('.git'):
-            raise InvalidPipelineRepositoryError('Repo url must end in .git')
-
-    def install(self, pipeline: str, editable = False, name = None, tag = None, config: Path = None, force = False, resources=[]) -> Pipeline:
+        if not repo.startswith("http"):
+            raise InvalidPipelineRepositoryError("Repo url must start with http")
+        if not repo.endswith(".git"):
+            raise InvalidPipelineRepositoryError("Repo url must end in .git")
+
+    def install(
+        self,
+        pipeline: str,
+        editable=False,
+        name=None,
+        tag=None,
+        config: Path = None,
+        force=False,
+        resources=[],
+    ) -> Pipeline:
         """
         Installs a Snakemake pipeline as a CLI.
         Args:
           pipeline (str): The URL of the repo or the path to the local pipeline.
           editable (bool, optional): Whether to install the pipeline in editable mode. Defaults to False.
           name (str, optional): The name of the pipeline. Defaults to None.
           tag (str, optional): The tag of the pipeline. Defaults to None.
@@ -92,101 +107,113 @@
           force (bool, optional): Whether to force the installation. Defaults to False.
           resources (list, optional): A list of additional resources to copy. Defaults to [].
         Returns:
           Pipeline: The installed pipeline.
         Examples:
           >>> nest.install('https://github.com/example/repo.git', name='example', tag='v1.0.0')
         """
+        def handle_force_installation(name: str):
+            try:
+                self.uninstall(name=name, force=True)
+            except PipelineNotFoundError:
+                pass
+
         if name in [p.name for p in self.pipelines]:
             raise ValueError("")
         try:
             self._check_repo_url_format(pipeline)
             if not name:
                 name = self._get_name_from_git_url(pipeline)
-            self._check_pipeline_name_available(name)
+            if not force:
+                self._check_pipeline_name_available(name)
+            else:
+                handle_force_installation(name)
             path = self.download(pipeline, name, tag_name=tag)
         except InvalidPipelineRepositoryError:
             pipeline = Path(pipeline)
-            if pipeline.suffix == '.snk':
+            if pipeline.suffix == ".snk":
                 pipeline = pipeline.parent
             if not name:
                 name = pipeline.name
-            self._check_pipeline_name_available(name)
+            if not force:
+                self._check_pipeline_name_available(name)
+            else:
+                handle_force_installation(name)
             path = self.local(pipeline, name, editable)
         try:
             pipeline = Pipeline(path=path)
             pipeline_executable = self.create_package(pipeline.path)
             self.link_pipeline_executable_to_bin(pipeline_executable)
             if config:
                 self.copy_nonstandard_config(pipeline.path, config)
             if resources:
                 self.additional_resources(pipeline.path, resources)
             self._confirm_installation(name)
         except Exception as e:
-            # remove any half completed steps 
+            # remove any half completed steps
             to_remove = self.get_paths_to_delete(name)
             self.delete_paths(to_remove)
             raise e
         return pipeline
-    
+
     def additional_resources(self, pipeline_dir: Path, resources: List[Path]):
         """
         Modify the .snk file so that resources will be copied at runtime.
         Args:
           pipeline_dir (Path): The path to the pipeline directory.
           resources (List[Path]): A list of additional resources to copy.
         Examples:
           >>> nest.additional_resources(Path('/path/to/pipeline'), [Path('/path/to/resource1'), Path('/path/to/resource2')])
         """
         # validate_resources(resources)
-        snk_config = SnkConfig.from_path(pipeline_dir / '.snk')
+        snk_config = SnkConfig.from_path(pipeline_dir / ".snk")
         snk_config.resources += [r for r in resources if r not in snk_config.resources]
-        snk_config.to_yaml(pipeline_dir / '.snk')
+        snk_config.to_yaml(pipeline_dir / ".snk")
 
     def copy_nonstandard_config(self, pipeline_dir: Path, config_path: Path):
         """
         Copy a nonstandard config file to the pipeline directory.
         Args:
           pipeline_dir (Path): The path to the pipeline directory.
           config_path (Path): The path to the config file.
         Examples:
           >>> nest.copy_nonstandard_config(Path('/path/to/pipeline'), Path('/path/to/config.yaml'))
         """
-        config_dir = pipeline_dir / 'config'
+        config_dir = pipeline_dir / "config"
         config_dir.mkdir()
-        shutil.copyfile(pipeline_dir / config_path, config_dir / 'config.yaml')
+        shutil.copyfile(pipeline_dir / config_path, config_dir / "config.yaml")
 
     def get_paths_to_delete(self, pipeline_name: str) -> List[Path]:
         """
         Get the paths to delete when uninstalling a pipeline.
         Args:
           pipeline_name (str): The name of the pipeline.
         Returns:
           List[Path]: A list of paths to delete.
         Examples:
           >>> nest.get_paths_to_delete('example')
           [Path('/path/to/pipelines/example'), Path('/path/to/bin/example')]
         """
         to_delete = []
-        
-        # remove repo 
+
+        # remove repo
         pipeline_dir = self.pipelines_dir / pipeline_name
         if pipeline_dir.exists() and pipeline_dir.is_dir():
             to_delete.append(pipeline_dir)
         elif pipeline_dir.is_symlink():
             to_delete.append(pipeline_dir)
         else:
-            raise PipelineNotFoundError(f'Could not find pipeline: {pipeline_name}')
+            raise PipelineNotFoundError(f"Could not find pipeline: {pipeline_name}")
 
         # remove link
         pipeline_bin_executable = self.bin_dir / pipeline_name
         if pipeline_bin_executable.exists() and pipeline_bin_executable.is_symlink():
             if str(pipeline_dir) in str(os.readlink(pipeline_bin_executable)):
                 to_delete.append(pipeline_bin_executable)
-        
+
         return to_delete
 
     def delete_paths(self, files: List[Path]):
         """
         Delete the given paths.
         Args:
           files (List[Path]): A list of paths to delete.
@@ -199,15 +226,17 @@
         # i.e. if it is a symlink read the link and check
         for path in files:
             if path.is_symlink():
                 print("Unlinking:", path)
                 path.unlink()
             elif path.is_dir():
                 print("Deleting:", path)
-                assert str(self.snk_home) in str(path), "Cannot delete folders outside of SNK_HOME"
+                assert str(self.snk_home) in str(
+                    path
+                ), "Cannot delete folders outside of SNK_HOME"
                 shutil.rmtree(path)
             else:
                 raise TypeError("Invalid file type")
 
     def uninstall(self, name: str, force: bool = False) -> bool:
         """
         Uninstalls a pipeline.
@@ -225,136 +254,147 @@
             proceed = True
         else:
             print(f"Uninstalling {name}")
             print("  Would remove:")
             for p in to_remove:
                 print(f"    {p}{'/*' if p.is_dir() else ''}")
             ans = input("Proceed (Y/n)? ")
-            proceed = ans.lower() in ['y', 'yes']
+            proceed = ans.lower() in ["y", "yes"]
         if not proceed:
             return False
         self.delete_paths(to_remove)
-        return True 
+        return True
 
     def _check_pipeline_name_available(self, name: str):
         if name in os.listdir(self.pipelines_dir):
-            raise PipelineExistsError(f"Pipeline '{name}' already exists in {self.pipelines_dir}")
+            raise PipelineExistsError(
+                f"Pipeline '{name}' already exists in {self.pipelines_dir}"
+            )
         if name in os.listdir(self.bin_dir):
-            raise PipelineExistsError(f"Pipeline '{name}' already exists in {self.bin_dir}")
+            raise PipelineExistsError(
+                f"Pipeline '{name}' already exists in {self.bin_dir}"
+            )
 
     def _confirm_installation(self, name: str):
         """
         Confirms that the installation was successful.
         Args:
           name (str): The name of the pipeline.
         Examples:
           >>> nest._confirm_installation('example')
         """
         pipeline_dir = self.pipelines_dir / name
         assert pipeline_dir.exists()
-        pipelines = [p.name.split('.')[0] for p in self.bin_dir.glob('*')]
+        pipelines = [p.name.split(".")[0] for p in self.bin_dir.glob("*")]
         assert name in pipelines
 
     def _get_name_from_git_url(self, git_url: str):
         """
         Gets the name of the pipeline from the git URL.
         Args:
           git_url (str): The URL of the git repository.
         Returns:
           str: The name of the pipeline.
         """
-        return git_url.split('/')[-1].split('.')[0]
+        return git_url.split("/")[-1].split(".")[0]
 
     @property
     def pipelines(self):
-        return [Pipeline(pipeline_dir.absolute()) for pipeline_dir in self.pipelines_dir.glob('*')]
+        return [
+            Pipeline(pipeline_dir.absolute())
+            for pipeline_dir in self.pipelines_dir.glob("*")
+        ]
 
     def download(self, repo_url: str, name: str, tag_name: str = None) -> Path:
         """
         Downloads a file from a given URL.
         Args:
           url (str): The URL of the file to download.
         Returns:
           None
         Side Effects:
           Downloads the file from the given URL.
         Examples:
           >>> Nest.download('https://example.com/file.txt')
           None
         """
-        location  = self.pipelines_dir / name
-        options = ['--depth 1', '--single-branch']
+        location = self.pipelines_dir / name
+        options = ["--depth 1", "--single-branch"]
         if tag_name:
-            options.append(f'--branch {tag_name}')
+            options.append(f"--branch {tag_name}")
         try:
             repo = Repo.clone_from(repo_url, location, multi_options=options)
             repo.git.checkout(tag_name)
         except GitCommandError as e:
             if "destination path" in e.stderr:
-                raise PipelineExistsError(f"Pipeline '{name}' already exists in {self.pipelines_dir}")
+                raise PipelineExistsError(
+                    f"Pipeline '{name}' already exists in {self.pipelines_dir}"
+                )
             elif f"Remote branch {tag_name}" in e.stderr:
                 raise PipelineNotFoundError(f"Pipeline tag '{tag_name}' not found")
             elif "not found" in e.stderr:
-                raise PipelineNotFoundError(f"Pipeline repository '{repo_url}' not found")
+                raise PipelineNotFoundError(
+                    f"Pipeline repository '{repo_url}' not found"
+                )
             raise e
         return location
-    
+
     def local(self, path: Path, name: str, editable=False) -> Path:
-        location  = self.pipelines_dir / name
+        location = self.pipelines_dir / name
         if editable:
             os.symlink(path.absolute(), location, target_is_directory=True)
             return location
         shutil.copytree(path, location)
         try:
             Repo(location)
         except InvalidGitRepositoryError:
             Repo.init(location, mkdir=False)
         return location
-        
-
 
     def create_package(self, pipeline_dir: Path) -> Path:
         """
         Creates a package in the local environment.
         Args:
           package_name (str): The name of the package to create.
         Returns:
           None
         Side Effects:
           Creates a package in the local environment.
         Examples:
           >>> Nest.create_package('my_package')
         """
         self.validate_SnakeMake_repo(pipeline_dir)
-        
-        template = inspect.cleandoc(f"""
+
+        template = inspect.cleandoc(
+            f"""
             #!/bin/sh
             '''exec' "{self.python_interpreter_path}" "$0" "$@"
             ' '''
             # -*- coding: utf-8 -*-
             import re
             import sys
             from snk import create_cli
             if __name__ == "__main__":
                 sys.argv[0] = re.sub(r'(-script\.pyw|\.exe)?$', '', sys.argv[0])
                 sys.exit(create_cli("{pipeline_dir}"))
                 
-        """)
+        """
+        )
 
-        pipeline_bin_dir = pipeline_dir / 'bin'
+        pipeline_bin_dir = pipeline_dir / "bin"
         pipeline_bin_dir.mkdir(exist_ok=True)
 
         name = pipeline_dir.name
 
-        if sys.platform.startswith('win'):
-            name += '.exe'
-        
+        if sys.platform.startswith("win"):
+            name += ".exe"
+
         pipeline_executable = pipeline_bin_dir / name
 
-        with open(pipeline_executable, 'w') as f:
+        with open(pipeline_executable, "w") as f:
             f.write(template)
 
         pipeline_executable.chmod(pipeline_executable.stat().st_mode | stat.S_IEXEC)
 
         return pipeline_executable
 
     def link_pipeline_executable_to_bin(self, pipeline_executable_path: Path):
@@ -381,8 +421,8 @@
         Returns:
           bool: True if the repository is valid, False otherwise.
         Examples:
           >>> Nest.validate_SnakeMake_repo('/path/to/repo')
           True
         """
         print("Skipping validation!")
-        pass
+        pass
```

### Comparing `snk-0.6.1/snk/cli/cli.py` & `snk-0.6.2/snk/cli/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import inspect
 import sys
 import typer
 from pathlib import Path
 from typing import Optional, List, Callable
 from datetime import datetime
 import subprocess
 import shutil
@@ -10,74 +11,110 @@
 
 import snakemake
 from rich.console import Console
 from rich.syntax import Syntax
 from art import text2art
 
 
-
-from .config import SnkConfig, get_config_from_pipeline_dir, load_pipeline_snakemake_config
+from .config import (
+    SnkConfig,
+    get_config_from_pipeline_dir,
+    load_pipeline_snakemake_config,
+)
 from .utils import add_dynamic_options, build_dynamic_cli_options, parse_config_args
 from .pipeline import Pipeline
 
 
 class CLI:
     """
     Constructor for the CLI class.
     Args:
       pipeline_dir_path (Path): Path to the pipeline directory.
     Side Effects:
       Initializes the CLI class.
     Examples:
       >>> CLI(Path('/path/to/pipeline'))
     """
-    def __init__(self, pipeline_dir_path: Path) -> None:
+
+    def __init__(self, pipeline_dir_path: Path = None) -> None:
+        if not pipeline_dir_path:
+            # get the calling frame (the frame of the function that called this function)
+            calling_frame = inspect.currentframe().f_back
+            # get the file path from the calling frame
+            pipeline_dir_path = Path(calling_frame.f_globals['__file__'])
+        if pipeline_dir_path.is_file():
+            pipeline_dir_path = pipeline_dir_path.parent
         self.pipeline = Pipeline(path=pipeline_dir_path)
         self.app = typer.Typer()
         self.snakemake_config = load_pipeline_snakemake_config(pipeline_dir_path)
-        self.snk_config: SnkConfig = SnkConfig.from_path(pipeline_dir_path / '.snk')
+        self.snk_config: SnkConfig = SnkConfig.from_path(pipeline_dir_path / ".snk")
         self.options = build_dynamic_cli_options(self.snakemake_config, self.snk_config)
         self.snakefile = self._find_snakefile()
-        self.conda_prefix_dir = pipeline_dir_path / '.conda'
+        self.conda_prefix_dir = pipeline_dir_path / ".conda"
         self.name = self.pipeline.name
+        self.verbose = False
+
         def _print_pipline_version(ctx: typer.Context, value: bool):
             if value:
                 typer.echo(self.pipeline.version)
                 raise typer.Exit()
 
         def _print_pipline_path(ctx: typer.Context, value: bool):
             if value:
                 typer.echo(self.pipeline.path)
                 raise typer.Exit()
 
         def callback(
-            ctx: typer.Context, 
-            version: Optional[bool] = typer.Option(None, '-v', '--version', help="Show the pipeline version.", is_eager=True, callback=_print_pipline_version, show_default=False),
-            path: Optional[bool] = typer.Option(None, '-p', '--path', help="Show the pipeline path.", is_eager=True, callback=_print_pipline_path, show_default=False)
+            ctx: typer.Context,
+            version: Optional[bool] = typer.Option(
+                None,
+                "-v",
+                "--version",
+                help="Show the pipeline version.",
+                is_eager=True,
+                callback=_print_pipline_version,
+                show_default=False,
+            ),
+            path: Optional[bool] = typer.Option(
+                None,
+                "-p",
+                "--path",
+                help="Show the pipeline path.",
+                is_eager=True,
+                callback=_print_pipline_path,
+                show_default=False,
+            ),
         ):
             if ctx.invoked_subcommand is None:
-                typer.echo(f'{ctx.get_help()}')
+                typer.echo(f"{ctx.get_help()}")
+
         # dynamically create the logo
         callback.__doc__ = f"{self.create_logo()}"
 
-        # registration 
-        self.register_callback(callback, invoke_without_command=True, context_settings={"help_option_names": ["-h", "--help"]})
-        self.register_command(self.info, help="Display information about current pipeline install.")
+        # registration
+        self.register_callback(
+            callback,
+            invoke_without_command=True,
+            context_settings={"help_option_names": ["-h", "--help"]},
+        )
+        self.register_command(
+            self.info, help="Display information about current pipeline install."
+        )
         self.register_command(self.config, help="Access the pipeline configuration.")
         self.register_command(self.env, help="Access the pipeline conda environments.")
         self.register_command(self.profile, help="Access the pipeline profiles.")
         # self.register_command(self.script, help="Access the pipeline scripts.")
         self.register_command(
-            add_dynamic_options(self.options)(self.run), 
-            help="Run the dynamically generated pipeline CLI.\n\nAll unrecognized arguments are passed onto Snakemake.", 
+            add_dynamic_options(self.options)(self.run),
+            help="Run the dynamically generated pipeline CLI.\n\nAll unrecognized arguments are passed onto Snakemake.",
             context_settings={
-                "allow_extra_args": True, 
-                "ignore_unknown_options": True, 
-                "help_option_names": ["-h", "--help"]
-            }
+                "allow_extra_args": True,
+                "ignore_unknown_options": True,
+                "help_option_names": ["-h", "--help"],
+            },
         )
 
     def __call__(self):
         """
         Invoke the CLI.
         Side Effects:
           Invokes the CLI.
@@ -116,44 +153,44 @@
         Args:
           font (str): The font to use for the logo.
         Returns:
           str: The logo.
         Examples:
           >>> CLI.create_logo()
         """
-        logo = text2art(self.name, font=font)        
-        doc  = f"""\b{logo}\bA Snakemake pipeline CLI generated with snk"""
+        logo = text2art(self.name, font=font)
+        doc = f"""\b{logo}\bA Snakemake pipeline CLI generated with snk"""
         return doc
 
     def _print_snakemake_help(value: bool):
         """
         Print the snakemake help and exit.
         Args:
           value (bool): If True, print the snakemake help and exit.
         Side Effects:
           Prints the snakemake help and exits.
         Examples:
           >>> CLI._print_snakemake_help(True)
         """
         if value:
             snakemake.main("-h")
-    
+
     def _find_snakefile(self):
         """
         Search possible snakefile locations.
         Returns:
           Path: The path to the snakefile.
         Examples:
           >>> CLI._find_snakefile()
         """
         for path in snakemake.SNAKEFILE_CHOICES:
             if (self.pipeline.path / path).exists():
-                return self.pipeline.path / path 
+                return self.pipeline.path / path
         raise FileNotFoundError("Snakefile not found!")
-    
+
     @contextmanager
     def copy_resources(self, resources: List[Path], cleanup: bool):
         """
         Copy resources to the current working directory.
         Args:
           resources (List[Path]): A list of paths to the resources to copy.
           cleanup (bool): If True, the resources will be removed after the function exits.
@@ -178,50 +215,102 @@
                 shutil.rmtree(resource)
             else:
                 os.remove(resource)
 
         try:
             for resource in resources:
                 abs_path = self.pipeline.path / resource
-                destination = Path('.') / resource.name
-                if not destination.exists(): 
+                destination = Path(".") / resource.name
+                if not destination.exists():
                     # make sure you don't delete files that are already there...
                     copy_resource(abs_path, destination)
                     copied_resources.append(destination)
                 else:
-                    typer.secho(
-                        f"Resource {resource.name} already exists... Skipping!", 
-                        fg=typer.colors.YELLOW
-                    )
+                    raise FileExistsError(f"Resource '{resource.name}' already exists!")
 
             yield
         finally:
             if not cleanup:
-                return 
+                return
             for copied_resource in copied_resources:
                 if copied_resource.exists():
+                    if self.verbose:
+                        typer.secho(
+                            f"Deleting '{resource.name}' resource...",
+                            fg=typer.colors.YELLOW,
+                        )
                     remove_resource(copied_resource)
 
     def run(
-            self,
-            ctx: typer.Context,
-            target: str = typer.Argument(None, help="File to generate. If None will run the pipeline 'all' rule."),
-            configfile: Path = typer.Option(None, help="Path to snakemake config file. Overrides existing config and defaults.", exists=True, dir_okay=False),
-            resource: List[Path] = typer.Option([], "--resource", "-r", help="Additional resources to copy to workdir at run time."),
-            profile: Optional[str] = typer.Option(None, "--profile", "-p", help=f"Name of profile to use for configuring Snakemake.",),
-            force: bool = typer.Option(False, "--force", "-f", help="Force the execution of the selected target or the first rule regardless of already created output."),
-            lock: bool = typer.Option(False, "--lock", "-l", help="Lock the working directory."),
-            keep_resources: bool = typer.Option(False, "--keep-resources", "-R", help="Keep resources after pipeline completes."),
-            keep_snakemake: bool = typer.Option(False, "--keep-snakemake", "-S", help="Keep .snakemake folder after pipeline completes."),
-            cores: int = typer.Option(None, "--cores", "-c", help="Set the number of cores to use. If None will use all cores."),
-            verbose: Optional[bool] = typer.Option(False, "--verbose", "-v", help="Run pipeline in verbose mode.",),
-            help_snakemake: Optional[bool] = typer.Option(
-                False, "--help-snakemake", "-hs", help="Print the snakemake help and exit.", is_eager=True, callback=_print_snakemake_help, show_default=False
-            ),
-        ):
+        self,
+        ctx: typer.Context,
+        target: str = typer.Argument(
+            None, help="File to generate. If None will run the pipeline 'all' rule."
+        ),
+        configfile: Path = typer.Option(
+            None,
+            help="Path to snakemake config file. Overrides existing config and defaults.",
+            exists=True,
+            dir_okay=False,
+        ),
+        resource: List[Path] = typer.Option(
+            [],
+            "--resource",
+            "-r",
+            help="Additional resources to copy to workdir at run time (relative to pipeline directory).",
+        ),
+        profile: Optional[str] = typer.Option(
+            None,
+            "--profile",
+            "-p",
+            help="Name of profile to use for configuring Snakemake.",
+        ),
+        force: bool = typer.Option(
+            False,
+            "--force",
+            "-f",
+            help="Force the execution of pipeline regardless of already created output.",
+        ),
+        lock: bool = typer.Option(
+            False, "--lock", "-l", help="Lock the working directory."
+        ),
+        keep_resources: bool = typer.Option(
+            False,
+            "--keep-resources",
+            "-R",
+            help="Keep resources after pipeline completes.",
+        ),
+        keep_snakemake: bool = typer.Option(
+            False,
+            "--keep-snakemake",
+            "-S",
+            help="Keep .snakemake folder after pipeline completes.",
+        ),
+        cores: int = typer.Option(
+            None,
+            "--cores",
+            "-c",
+            help="Set the number of cores to use. If None will use all cores.",
+        ),
+        verbose: Optional[bool] = typer.Option(
+            False,
+            "--verbose",
+            "-v",
+            help="Run pipeline in verbose mode.",
+        ),
+        help_snakemake: Optional[bool] = typer.Option(
+            False,
+            "--help-snakemake",
+            "-hs",
+            help="Print the snakemake help and exit.",
+            is_eager=True,
+            callback=_print_snakemake_help,
+            show_default=False,
+        ),
+    ):
         """
         Run the pipeline.
         Args:
           target (str): File to generate. If None will run the pipeline 'all' rule.
           configfile (Path): Path to snakemake config file. Overrides existing config and defaults.
           resource (List[Path]): Additional resources to copy to workdir at run time.
           keep_resources (bool): Keep resources.
@@ -230,149 +319,166 @@
           verbose (bool): Run pipeline in verbose mode.
           help_snakemake (bool): Print the snakemake help and exit.
         Side Effects:
           Runs the pipeline.
         Examples:
           >>> CLI.run(target='my_target', configfile=Path('/path/to/config.yaml'), resource=[Path('/path/to/resource')], verbose=True)
         """
+        self.verbose = verbose
         args = []
         if not cores:
-            cores = 'all'
-        args.extend([
-            "--use-conda",
-            f"--conda-prefix={self.conda_prefix_dir}",
-            f"--cores={cores}",
-        ])
+            cores = "all"
+        args.extend(
+            [
+                "--use-conda",
+                f"--conda-prefix={self.conda_prefix_dir}",
+                f"--cores={cores}",
+            ]
+        )
         if not self.snakefile.exists():
-            raise ValueError('Could not find Snakefile') # this should occur at install
+            raise ValueError("Could not find Snakefile")  # this should occur at install
         else:
             args.append(f"--snakefile={self.snakefile}")
-        
+
         if not configfile:
             configfile = get_config_from_pipeline_dir(self.pipeline.path)
         args.append(f"--configfile={configfile}")
 
         if profile:
-          found_profile = [p for p in self.pipeline.profiles if profile==p.name]
-          if found_profile:
-              profile = found_profile[0]
-          args.append(f"--profile={profile}")
-        
+            found_profile = [p for p in self.pipeline.profiles if profile == p.name]
+            if found_profile:
+                profile = found_profile[0]
+            args.append(f"--profile={profile}")
+
         # Set up conda frontend
         mamba_found = True
         try:
             subprocess.run(["mamba", "--version"], capture_output=True, check=True)
         except (subprocess.CalledProcessError, FileNotFoundError):
-            typer.secho("Mamba not found! Install for speed up.", fg=typer.colors.YELLOW)
+            typer.secho(
+                "Mamba not found! Install for speed up.", fg=typer.colors.YELLOW
+            )
             mamba_found = False
         if not mamba_found:
             args.append("--conda-frontend=conda")
-        
+
         typer.echo(self.create_logo())
         typer.echo()
 
         if verbose:
             args.insert(0, "--verbose")
 
         if force:
-            args.append("--force")
+            args.append("--forceall")
 
         if not lock:
             args.append("--nolock")
-            
+
         if target:
             args.append(target)
-        targets_and_or_snakemake, config_dict_list = parse_config_args(ctx.args, options=self.options)
+        targets_and_or_snakemake, config_dict_list = parse_config_args(
+            ctx.args, options=self.options
+        )
 
         args.extend(targets_and_or_snakemake)
 
-        configs = [f"{list(c.keys())[0]}={list(c.values())[0]}" for c in config_dict_list]
+        configs = [
+            f"{list(c.keys())[0]}={list(c.values())[0]}" for c in config_dict_list
+        ]
         if configs:
             args.extend(["--config", *configs])
         if verbose:
             typer.secho(f"snakemake {' '.join(args)}\n", fg=typer.colors.MAGENTA)
-        
+
         self.snk_config.add_resources(resource, self.pipeline.path)
-        
+
         with self.copy_resources(self.snk_config.resources, cleanup=not keep_resources):
             try:
-              status = 0
-              snakemake.main(args)
+                snakemake.main(args)
             except SystemExit as e:
-                status = e
+                status = int(str(e))
+                if status:
+                    sys.exit(status)
         if not keep_snakemake and Path(".snakemake").exists():
             if verbose:
-              typer.secho("Deleting .snakemake folder", fg="yellow")
+                typer.secho("Deleting '.snakemake' folder...", fg="yellow")
             shutil.rmtree(".snakemake")
-        sys.exit(status)
 
     def info(self):
         """
         Display information about current pipeline install.
         Returns:
           str: A JSON string containing information about the current pipeline install.
         Examples:
           >>> CLI.info()
         """
         import json
+
         info_dict = {}
-        info_dict['name'] = self.pipeline.path.name
-        info_dict['version'] = self.pipeline.version
-        info_dict['pipeline_dir_path'] = str(self.pipeline.path)
+        info_dict["name"] = self.pipeline.path.name
+        info_dict["version"] = self.pipeline.version
+        info_dict["pipeline_dir_path"] = str(self.pipeline.path)
         typer.echo(json.dumps(info_dict, indent=2))
 
     def config(self):
         """
         Access the pipeline configuration.
         Side Effects:
           Prints the pipeline configuration.
         Examples:
           >>> CLI.config()
         """
         config_path = get_config_from_pipeline_dir(self.pipeline.path)
         if not config_path:
-            typer.secho("Could not find config...", fg='red')
+            typer.secho("Could not find config...", fg="red")
             raise typer.Exit(1)
         with open(config_path) as f:
             code = f.read()
-            syntax = Syntax(code, 'yaml')
+            syntax = Syntax(code, "yaml")
             console = Console()
             console.print(syntax)
-    
 
     def env(
         self,
         name: str = typer.Argument(None, help="The name of the environment."),
     ):
         """
         Access the pipeline conda environments.
         Args:
           name (str): The name of the environment.
         Examples:
           >>> CLI.env(name='my_env')
         """
-        environments_dir_yellow = typer.style(self.pipeline.path / 'envs', fg=typer.colors.YELLOW)
-        typer.echo(f"Found {len(self.pipeline.environments)} environments in {environments_dir_yellow}")
+        environments_dir_yellow = typer.style(
+            self.pipeline.path / "envs", fg=typer.colors.YELLOW
+        )
+        typer.echo(
+            f"Found {len(self.pipeline.environments)} environments in {environments_dir_yellow}"
+        )
         for env in self.pipeline.environments:
             typer.echo(f"- {env}")
-    
+
     def profile(
         self,
         name: str = typer.Argument(None, help="The name of the profile."),
     ):
-        profiles_dir_yellow = typer.style(self.pipeline.path / 'profiles', fg=typer.colors.YELLOW)
-        typer.echo(f"Found {len(self.pipeline.profiles)} profiles in {profiles_dir_yellow}")
+        profiles_dir_yellow = typer.style(
+            self.pipeline.path / "profiles", fg=typer.colors.YELLOW
+        )
+        typer.echo(
+            f"Found {len(self.pipeline.profiles)} profiles in {profiles_dir_yellow}"
+        )
         for profile in self.pipeline.profiles:
             typer.echo(f"- {profile.name}")
 
     # def script(
     #     self,
     #     name: Optional[str] = typer.Argument(None)
     # ):
     #     """
     #     Access the pipeline scripts.
     #     Args:
     #       name (str): The name of the script.
     #     Examples:
     #       >>> CLI.script(name='my_script')
     #     """
-    #     raise NotImplementedError
+    #     raise NotImplementedError
```

### Comparing `snk-0.6.1/snk/cli/config.py` & `snk-0.6.2/snk/cli/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,53 @@
 from pathlib import Path
 from typing import List
 import snakemake
 from dataclasses import dataclass, field
 
 import yaml
 
+
 @dataclass
 class SnkConfig:
     """
     SNK config holds dynamic cli config and option annotations.
     """
+
     resources: List[Path] = field(default_factory=list)
     annotations: dict = field(default_factory=dict)
 
     @classmethod
     def from_path(cls, snk_config_path: Path):
         """
         Load and validate SNK config from .snk file.
         """
         if snk_config_path.exists():
             snk_config_dict = snakemake.load_configfile(snk_config_path)
             snk_config = cls(**snk_config_dict)
-            snk_config.resources = [snk_config_path.parent / resource for resource in snk_config.resources]
+            snk_config.resources = [
+                snk_config_path.parent / resource for resource in snk_config.resources
+            ]
             snk_config.validate_resources(snk_config.resources)
             return snk_config
         return cls()
-    
+
     def validate_resources(self, resources):
         """
         Validate resources.
         Args:
             resources (List[Path]): List of resources to validate.
         Raises:
             FileNotFoundError: If a resource is not found.
         Notes:
             This function does not modify the resources list.
         """
         for resource in resources:
-            assert resource.exists(), FileNotFoundError(f"Could not find resource: {resource}")
+            assert resource.exists(), FileNotFoundError(
+                f"Could not find resource: {resource}"
+            )
 
     def add_resources(self, resources: List[Path], pipeline_dir_path: Path = None):
         processed = []
         for resource in resources:
             if pipeline_dir_path and not resource.is_absolute():
                 resource = pipeline_dir_path / resource
             processed.append(resource)
@@ -54,29 +60,32 @@
         Args:
             path (Path): Path to write the YAML file to.
         Returns:
             None
         Side Effects:
             Writes the SNK config to the specified path.
         """
-        with open(path, 'w') as f:
+        with open(path, "w") as f:
             yaml.dump(vars(self), f)
-                             
-    
+
 
 def get_config_from_pipeline_dir(pipeline_dir_path: Path):
     """Search possible config locations"""
-    for path in [Path('config') / 'config.yaml', Path('config') / 'config.yml', 'config.yaml', 'config.yml']:
+    for path in [
+        Path("config") / "config.yaml",
+        Path("config") / "config.yml",
+        "config.yaml",
+        "config.yml",
+    ]:
         if (pipeline_dir_path / path).exists():
-            return pipeline_dir_path / path 
+            return pipeline_dir_path / path
     return None
 
 
-
 def load_pipeline_snakemake_config(pipeline_dir_path: Path):
     """
     Load snakemake config.
     """
     pipeline_config_path = get_config_from_pipeline_dir(pipeline_dir_path)
-    if not pipeline_config_path.exists():
-        return []
+    if not pipeline_config_path or not pipeline_config_path.exists():
+        return {}
     return snakemake.load_configfile(pipeline_config_path)
```

### Comparing `snk-0.6.1/snk/cli/pipeline.py` & `snk-0.6.2/snk/cli/pipeline.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,70 +1,85 @@
 from pathlib import Path
 import sys
+from typing import Optional
 from git import Repo, GitCommandError, InvalidGitRepositoryError
 
+
 class Pipeline:
     """
     Represents a pipeline.
     Attributes:
       path (Path): The path to the pipeline.
       repo (Repo): The git repository of the pipeline.
       name (str): The name of the pipeline.
     """
-    def __init__(self, path:Path) -> None:
+
+    def __init__(self, path: Path) -> None:
         """
         Initializes a Pipeline object.
         Args:
             path (Path): The path to the pipeline.
         Returns:
             None
         Notes:
             Initializes the `repo` and `name` attributes.
         """
         self.path = path
-        if path.is_symlink(): # editable mode 
+        if path.is_symlink():  # editable mode
             self.repo = None
         else:
-            self.repo = Repo(path)
+            try:
+                self.repo = Repo(path)
+            except InvalidGitRepositoryError:
+                self.repo = None
         self.name = self.path.name
-    
+
     @property
     def version(self):
         """
         Gets the version of the pipeline.
         Returns:
             str: The version of the pipeline, or None if no version is found.
         """
         try:
             # TODO: default to commit
-            version = self.repo.git.describe(['--tags','--exact-match']) 
+            version = self.repo.git.describe(["--tags", "--exact-match"])
         except Exception:
             version = None
         return version
 
     @property
     def executable(self):
         """
         Gets the executable of the pipeline.
         Returns:
             Path: The path to the pipeline executable.
         """
-        pipeline_bin_dir = self.path / 'bin'
+        pipeline_bin_dir = self.path / "bin"
         name = self.name
-        if sys.platform.startswith('win'):
-            name += '.exe'
+        if sys.platform.startswith("win"):
+            name += ".exe"
         return pipeline_bin_dir / name
-        
+
+    def _find_folder(self, name) -> Optional[Path]:
+        """Search for folder"""
+        if (self.path / name).exists():
+            return self.path / name
+        if (self.path / "workflow" / name).exists():
+            return self.path / "workflow" / name
+        return None
+
     @property
     def profiles(self):
-        pipeline_profile_dir = self.path / 'profiles'
-        if not pipeline_profile_dir.exists():
-            return []
-        return [p for p in pipeline_profile_dir.glob("*") if p.is_dir()]
-        
+        pipeline_profile_dir = self._find_folder("profiles")
+        if pipeline_profile_dir:
+            return [p for p in pipeline_profile_dir.glob("*") if p.is_dir()]
+        return []
+
     @property
     def environments(self):
-        pipeline_environments_dir = self.path / 'envs'
-        if not pipeline_environments_dir.exists():
-            return []
-        return [e for e in pipeline_environments_dir.glob("*.ya?ml")]
-        
+        pipeline_environments_dir = self._find_folder("envs")
+        if pipeline_environments_dir:
+            return [e for e in pipeline_environments_dir.glob("*.yaml")] + [
+                e for e in pipeline_environments_dir.glob("*.yml")
+            ]
+        return []
```

### Comparing `snk-0.6.1/snk/cli/utils.py` & `snk-0.6.2/snk/cli/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,50 +3,57 @@
 from makefun import wraps
 from pathlib import Path
 from .config import SnkConfig
 from datetime import datetime
 import typer
 import sys
 import collections  # MutableMapping import hack
+
 if sys.version_info.major == 3 and sys.version_info.minor >= 10:
     from collections.abc import MutableMapping
 else:
     from collections import MutableMapping
 
 
 types = {
-    'int': int,
-    'integer': int,
-    'str': str,
-    'string': str,
-    'path': Path,
-    'bool': bool,
-    'boolean': bool,
-    'list': List[str],
-    'list[path]': List[Path],
-    'list[int]': List[int],
+    "int": int,
+    "integer": int,
+    "str": str,
+    "string": str,
+    "path": Path,
+    "bool": bool,
+    "boolean": bool,
+    "list": List[str],
+    "list[path]": List[Path],
+    "list[int]": List[int],
 }
 
+
 def create_cli_parameter(option):
     """
     Creates a parameter for a CLI option.
     Args:
       option (dict): A dictionary containing the option's name, type, required status, default value, and help message.
     Returns:
       Parameter: A parameter object for the CLI option.
     Examples:
       >>> option = {'name': 'foo', 'type': 'int', 'required': True, 'default': 0, 'help': 'A number'}
       >>> create_cli_parameter(option)
       Parameter('foo', kind=Parameter.POSITIONAL_OR_KEYWORD, default=typer.Option(..., help='[CONFIG] A number'), annotation=int)
     """
     return Parameter(
-        option['name'], 
-        kind=Parameter.POSITIONAL_OR_KEYWORD, 
-        default=typer.Option(... if option['required'] else option['default'], help=f"[CONFIG] {option['help']}"), 
-        annotation=types.get(option['type'].lower(), str))
+        option["name"],
+        kind=Parameter.POSITIONAL_OR_KEYWORD,
+        default=typer.Option(
+            ... if option["required"] else option["default"],
+            help=f"[CONFIG] {option['help']}",
+        ),
+        annotation=types.get(option["type"].lower(), str),
+    )
+
 
 def add_dynamic_options(options: List[dict]):
     """
     Decorator to add dynamic options to a function.
     Args:
       options (List[dict]): A list of dictionaries containing the option's name, type, required status, default value, and help message.
     Returns:
@@ -54,48 +61,54 @@
     Examples:
       >>> @add_dynamic_options([{'name': 'foo', 'type': 'int', 'required': True, 'default': 0, 'help': 'A number'}])
       ... def my_func(ctx):
       ...     pass
       >>> my_func
       <function my_func at 0x7f8f9f9f9f90>
     """
+
     def inner(func: Callable):
         """
         Wraps a function with dynamic options.
         """
         func_sig = signature(func)
         params = list(func_sig.parameters.values())
         for op in options[::-1]:
             params.insert(1, create_cli_parameter(op))
         new_sig = func_sig.replace(parameters=params)
+
         @wraps(func, new_sig=new_sig)
         def func_wrapper(*args, **kwargs):
             """
             Wraps a function with dynamic options.
             Args:
                 *args: Variable length argument list.
                 **kwargs: Arbitrary keyword arguments.
             Returns:
                 Callable: A wrapped function with the dynamic options added.
             Notes:
                 This function is used as an inner function in the `add_dynamic_options` decorator.
             """
-            if kwargs['configfile']:
+            if kwargs["configfile"]:
                 # need to check if kwargs in options have changed
                 # parse the new configfile and update the defautls
                 raise NotImplementedError
             for op in options:
-                kwargs['ctx'].args.extend([f"--{op['name']}", kwargs[op['name']]])
-            kwargs= {k:v for k,v in kwargs.items() if k in func_sig.parameters.keys()}
+                kwargs["ctx"].args.extend([f"--{op['name']}", kwargs[op["name"]]])
+            kwargs = {
+                k: v for k, v in kwargs.items() if k in func_sig.parameters.keys()
+            }
             return func(*args, **kwargs)
+
         return func_wrapper
+
     return inner
 
 
-def flatten(d, parent_key='', sep=':'):
+def flatten(d, parent_key="", sep=":"):
     """
     Flattens a nested dictionary.
     Args:
       d (dict): The dictionary to flatten.
       parent_key (str, optional): The parent key of the dictionary. Defaults to ''.
       sep (str, optional): The separator to use between keys. Defaults to ':'.
     Returns:
@@ -126,14 +139,15 @@
     for part in parts[:-1]:
         current_dict = current_dict.setdefault(part, {})
 
     current_dict[parts[-1]] = value
 
     return result_dict
 
+
 def serialise(d):
     """
     Serialises a data structure into a string.
     Args:
       d (any): The data structure to serialise.
     Returns:
       any: The serialised data structure.
@@ -150,47 +164,50 @@
     if isinstance(d, dict):
         for k, v in d.items():
             d.update({k: serialise(v)})
 
     # return anything else, like a string or number
     return d
 
+
 def parse_config_args(args: List[str], options):
     """
     Parses a list of arguments and a list of options.
     Args:
       args (List[str]): A list of arguments.
       options (List[dict]): A list of options.
     Returns:
       (List[str], List[dict]): A tuple of parsed arguments and config.
     Examples:
       >>> parse_config_args(['-name', 'John', '-age', '20'], [{'name': 'name', 'default': '', 'help': '', 'type': 'str', 'required': True}, {'name': 'age', 'default': '', 'help': '', 'type': 'int', 'required': True}])
       (['John', '20'], [{'name': 'name', 'John'}, {'age': 20}])
     """
-    names = [op['name'] for op in options]
+    names = [op["name"] for op in options]
     config = []
     parsed = []
-    flag=None
+    flag = None
     for arg in args:
         if flag:
-            name = flag.lstrip('-')
-            op = next(op for op in options if op['name'] == name)
-            if op['default'] == serialise(arg):
+            name = flag.lstrip("-")
+            op = next(op for op in options if op["name"] == name)
+            if op["default"] == serialise(arg):
                 # skip args that don't change
-                flag=None
+                flag = None
                 continue
-            if ":" in op['original_key']:
-                samkemake_format_config = convert_key_to_snakemake_format(op['original_key'], arg)
+            if ":" in op["original_key"]:
+                samkemake_format_config = convert_key_to_snakemake_format(
+                    op["original_key"], arg
+                )
                 name = list(samkemake_format_config.keys())[0]
                 arg = samkemake_format_config[name]
             # config.append(f'{name}={serialise(arg)}')
             config.append({name: serialise(arg)})
-            flag=None
+            flag = None
             continue
-        if arg.startswith('-') and arg.lstrip('-') in names:
+        if arg.startswith("-") and arg.lstrip("-") in names:
             flag = arg
             continue
         parsed.append(arg)
     return parsed, config
 
 
 def build_dynamic_cli_options(snakemake_config, snk_config: SnkConfig):
@@ -205,26 +222,28 @@
       >>> build_dynamic_cli_options({'name': 'John', 'age': 20}, {'annotations': {'name:name': 'name', 'name:help': '', 'name:type': 'str', 'name:required': True, 'age:name': 'age', 'age:help': '', 'age:type': 'int', 'age:required': True}})
       [{'name': 'name', 'original_key': 'name', 'default': 'John', 'help': '', 'type': 'str', 'required': True}, {'name': 'age', 'original_key': 'age', 'default': 20, 'help': '', 'type': 'int', 'required': True}]
     """
     flat_config = flatten(snakemake_config)
     options = []
     flat_snk_annotations = flatten(snk_config.annotations)
     for op in flat_config:
-        name = flat_snk_annotations.get(f"{op}:name", op.replace(':', '_'))
+        name = flat_snk_annotations.get(f"{op}:name", op.replace(":", "_"))
         help = flat_snk_annotations.get(f"{op}:help", "")
-        # TODO be smarter here 
-        # look up the List type e.g. if type == list then check the frist index type 
+        # TODO be smarter here
+        # look up the List type e.g. if type == list then check the frist index type
         # also can probably just pass the type around instead of the string?
-        param_type = flat_snk_annotations.get(f"{op}:type", f"{type(flat_config[op]).__name__}")  # TODO refactor 
+        param_type = flat_snk_annotations.get(
+            f"{op}:type", f"{type(flat_config[op]).__name__}"
+        )  # TODO refactor
         required = flat_snk_annotations.get(f"{op}:required", False)
         options.append(
             {
-                'name':name.replace('-', '_'),
-                'original_key': op,
-                'default': flat_config[op],
-                'help': help,
-                'type': param_type,
-                'required': required
+                "name": name.replace("-", "_"),
+                "original_key": op,
+                "default": flat_config[op],
+                "help": help,
+                "type": param_type,
+                "required": required,
             }
         )
     # TODO: find annotations missing from config and add them to options
     return options
```

### Comparing `snk-0.6.1/tests/.DS_Store` & `snk-0.6.2/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `snk-0.6.1/tests/conftest.py` & `snk-0.6.2/tests/conftest.py`

 * *Files 18% similar despite different names*

```diff
@@ -24,8 +24,21 @@
 def basic_runner(tmp_path_factory):
     nest = Nest(tmp_path_factory.mktemp("snk"), tmp_path_factory.mktemp("bin"))
     basic_pipeline = nest.install('https://github.com/Wytamma/snk-basic-pipeline.git')
     expected = nest.pipelines_dir / 'snk-basic-pipeline'
     assert expected.exists()
     print(basic_pipeline.executable)
     runner = CLIRunner([basic_pipeline.executable])
-    return runner
+    return runner
+
+@pytest.fixture()
+def local_pipeline(tmp_path_factory):
+    path = Path(tmp_path_factory.mktemp("snk"))
+    (path / 'home').mkdir()
+    (path / 'bin').mkdir()
+    nest = Nest(path / 'home', path / 'bin')
+    print(nest.bin_dir)
+    print(nest.snk_home)
+    local_pipeline = nest.install("tests/data/pipeline")
+    expected = nest.pipelines_dir / 'pipeline'
+    assert expected.exists()
+    return local_pipeline
```

### Comparing `snk-0.6.1/tests/test_nest.py` & `snk-0.6.2/tests/test_nest.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.1/tests/test_pipline_cli.py` & `snk-0.6.2/tests/test_pipline_cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,32 +4,35 @@
 import pytest
 
 def test_flatten(example_config: Path):
     config = snakemake.load_configfile(example_config)
     flat_config = flatten(config)
     assert flat_config['diffexp:contrasts:A-vs-B'] == ['A', 'B']
 
-def test_install(basic_runner):
-    res = basic_runner(['--help'])
-    assert 'snk-basic-pipeline' in res.stdout
-
-def test_info(basic_runner):
-    res = basic_runner(['info'])
-    assert 'snk-basic-pipeline' in res.stdout, res.stderr
-    assert 'version' in res.stdout
-    assert 'pipeline_dir_path' in res.stdout
 
 @pytest.mark.parametrize("key, value, expected", [
     ("a:b:c", 42, {"a": {"b": {"c": 42}}}),
     ("x:y:z", "hello", {"x": {"y": {"z": "hello"}}}),
     ("d:e", [1, 2, 3], {"d": {"e": [1, 2, 3]}}),
     ("h", "world", {"h": "world"}),
 ])
 def test_convert_key_to_snakemake_format(key, value, expected):
     assert convert_key_to_snakemake_format(key, value) == expected
 
+def test_installation(basic_runner):
+    res = basic_runner(['--help'])
+    assert 'snk-basic-pipeline' in res.stdout
+
+def test_info(basic_runner):
+    res = basic_runner(['info'])
+    assert 'snk-basic-pipeline' in res.stdout, res.stderr
+    assert 'version' in res.stdout
+    assert 'pipeline_dir_path' in res.stdout
+
+def test_run(basic_runner):
+    res = basic_runner(['run', '-h'])
+    assert 'snk-basic-pipeline' in res.stdout, res.stderr
+    assert 'samples' in res.stdout
+    assert 'genome' in res.stdout
+    res = basic_runner(['run'])
+
 
-# def test_run(basic_runner):
-#     res = basic_runner(['info'])
-#     assert 'snk-basic-pipeline' in res.stdout, res.stderr
-#     assert 'version' in res.stdout
-#     assert 'pipeline_dir_path' in res.stdout
```

### Comparing `snk-0.6.1/tests/utils.py` & `snk-0.6.2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.1/tests/data/artic_v4.1.bed` & `snk-0.6.2/tests/data/artic_v4.1.bed`

 * *Files identical despite different names*

### Comparing `snk-0.6.1/tests/data/config.yaml` & `snk-0.6.2/tests/data/config.yaml`

 * *Files identical despite different names*

### Comparing `snk-0.6.1/tests/data/cov.fasta` & `snk-0.6.2/tests/data/cov.fasta`

 * *Files identical despite different names*

### Comparing `snk-0.6.1/LICENSE.txt` & `snk-0.6.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snk-0.6.1/README.md` & `snk-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `snk-0.6.1/pyproject.toml` & `snk-0.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `snk-0.6.1/PKG-INFO` & `snk-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snk
-Version: 0.6.1
+Version: 0.6.2
 Project-URL: Documentation, https://github.com/wytamma/snk#readme
 Project-URL: Issues, https://github.com/wytamma/snk/issues
 Project-URL: Source, https://github.com/wytamma/snk
 Author-email: Wytamma Wirth <wytamma.wirth@me.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

