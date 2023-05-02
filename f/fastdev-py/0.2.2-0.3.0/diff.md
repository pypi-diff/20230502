# Comparing `tmp/fastdev-py-0.2.2.tar.gz` & `tmp/fastdev-py-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastdev-py-0.2.2.tar", last modified: Mon May  1 03:25:47 2023, max compression
+gzip compressed data, was "fastdev-py-0.3.0.tar", last modified: Tue May  2 02:12:20 2023, max compression
```

## Comparing `fastdev-py-0.2.2.tar` & `fastdev-py-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      677 2023-05-01 03:25:34.935001 fastdev-py-0.2.2/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0      748 2023-05-01 03:25:34.935001 fastdev-py-0.2.2/.github/workflows/pypitest-publish.yml
--rw-r--r--   0        0        0      856 2023-05-01 03:25:34.935001 fastdev-py-0.2.2/.gitignore
--rw-r--r--   0        0        0       51 2023-05-01 03:25:34.935001 fastdev-py-0.2.2/license.md
--rw-r--r--   0        0        0     1231 2023-05-01 03:25:34.935001 fastdev-py-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      302 2023-05-01 03:25:34.935001 fastdev-py-0.2.2/readme.md
--rw-r--r--   0        0        0      154 2023-05-01 03:25:34.935001 fastdev-py-0.2.2/src/fastdev/__init__.py
--rw-r--r--   0        0        0      584 2023-05-01 03:25:34.935001 fastdev-py-0.2.2/src/fastdev/__main__.py
--rw-r--r--   0        0        0    11496 2023-05-01 03:25:34.935001 fastdev-py-0.2.2/src/fastdev/builders/deno_lts_esbuild.ts
--rw-r--r--   0        0        0     1015 2023-05-01 03:25:34.935001 fastdev-py-0.2.2/src/fastdev/config.py
--rw-r--r--   0        0        0     1848 2023-05-01 03:25:34.935001 fastdev-py-0.2.2/src/fastdev/fs_serving.py
--rw-r--r--   0        0        0     8133 2023-05-01 03:25:34.935001 fastdev-py-0.2.2/src/fastdev/preprocessor/temp.py.bak
--rw-r--r--   0        0        0     2508 2023-05-01 03:25:34.935001 fastdev-py-0.2.2/src/fastdev/router.py
--rw-r--r--   0        0        0     1364 2023-05-01 03:25:34.935001 fastdev-py-0.2.2/src/fastdev/ts_serving.py
--rw-r--r--   0        0        0     1463 2023-05-01 03:25:34.935001 fastdev-py-0.2.2/src/fastdev/utils.py
--rw-r--r--   0        0        0      313 2023-05-01 03:25:34.935001 fastdev-py-0.2.2/tests/1/hello.ts
--rw-r--r--   0        0        0       40 2023-05-01 03:25:34.935001 fastdev-py-0.2.2/tests/1/temp.ts
--rw-r--r--   0        0        0      741 1970-01-01 00:00:00.000000 fastdev-py-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      677 2023-05-02 02:12:04.636442 fastdev-py-0.3.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0      748 2023-05-02 02:12:04.636442 fastdev-py-0.3.0/.github/workflows/pypitest-publish.yml
+-rw-r--r--   0        0        0      856 2023-05-02 02:12:04.636442 fastdev-py-0.3.0/.gitignore
+-rw-r--r--   0        0        0       51 2023-05-02 02:12:04.636442 fastdev-py-0.3.0/license.md
+-rw-r--r--   0        0        0     1231 2023-05-02 02:12:04.636442 fastdev-py-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      302 2023-05-02 02:12:04.636442 fastdev-py-0.3.0/readme.md
+-rw-r--r--   0        0        0      154 2023-05-02 02:12:04.636442 fastdev-py-0.3.0/src/fastdev/__init__.py
+-rw-r--r--   0        0        0      584 2023-05-02 02:12:04.636442 fastdev-py-0.3.0/src/fastdev/__main__.py
+-rw-r--r--   0        0        0    11496 2023-05-02 02:12:04.636442 fastdev-py-0.3.0/src/fastdev/builders/deno_lts_esbuild.ts
+-rw-r--r--   0        0        0     1015 2023-05-02 02:12:04.636442 fastdev-py-0.3.0/src/fastdev/config.py
+-rw-r--r--   0        0        0     1701 2023-05-02 02:12:04.636442 fastdev-py-0.3.0/src/fastdev/fs_serving.py
+-rw-r--r--   0        0        0     8133 2023-05-02 02:12:04.636442 fastdev-py-0.3.0/src/fastdev/preprocessor/temp.py.bak
+-rw-r--r--   0        0        0     4405 2023-05-02 02:12:04.636442 fastdev-py-0.3.0/src/fastdev/router.py
+-rw-r--r--   0        0        0     1410 2023-05-02 02:12:04.636442 fastdev-py-0.3.0/src/fastdev/ts_serving.py
+-rw-r--r--   0        0        0     1463 2023-05-02 02:12:04.636442 fastdev-py-0.3.0/src/fastdev/utils.py
+-rw-r--r--   0        0        0      313 2023-05-02 02:12:04.636442 fastdev-py-0.3.0/tests/1/hello.ts
+-rw-r--r--   0        0        0       40 2023-05-02 02:12:04.636442 fastdev-py-0.3.0/tests/1/temp.ts
+-rw-r--r--   0        0        0      741 1970-01-01 00:00:00.000000 fastdev-py-0.3.0/PKG-INFO
```

### Comparing `fastdev-py-0.2.2/.github/workflows/pypi-publish.yml` & `fastdev-py-0.3.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `fastdev-py-0.2.2/.github/workflows/pypitest-publish.yml` & `fastdev-py-0.3.0/.github/workflows/pypitest-publish.yml`

 * *Files identical despite different names*

### Comparing `fastdev-py-0.2.2/.gitignore` & `fastdev-py-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fastdev-py-0.2.2/pyproject.toml` & `fastdev-py-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "fastdev-py"
-version = "0.2.2"
+version = "0.3.0"
 description = "FastAPI development server that JIT preprocess TS, TSX, SCSS, etc... files."
 readme = "readme.md"
 requires-python = ">=3.11"
 license = { file = "license.md" }
 authors = [{ name = "Omar Azmi" }]
 dependencies = ["fastapi"]
 keywords = [
```

### Comparing `fastdev-py-0.2.2/src/fastdev/__main__.py` & `fastdev-py-0.3.0/src/fastdev/__main__.py`

 * *Files identical despite different names*

### Comparing `fastdev-py-0.2.2/src/fastdev/builders/deno_lts_esbuild.ts` & `fastdev-py-0.3.0/src/fastdev/builders/deno_lts_esbuild.ts`

 * *Files identical despite different names*

### Comparing `fastdev-py-0.2.2/src/fastdev/config.py` & `fastdev-py-0.3.0/src/fastdev/config.py`

 * *Files identical despite different names*

### Comparing `fastdev-py-0.2.2/src/fastdev/fs_serving.py` & `fastdev-py-0.3.0/src/fastdev/fs_serving.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 from pathlib import Path
-from fastapi.responses import (
-	FileResponse, HTMLResponse, PlainTextResponse, RedirectResponse,
-)
+from fastapi.responses import FileResponse, HTMLResponse, PlainTextResponse
 from .config import SWD
 from .utils import qoute
 
 
 async def serve_file(file: Path):
 	if not file.is_file():
 		return PlainTextResponse(f"the following file was not found:\n\t{file}", status_code=404)
@@ -14,30 +12,27 @@
 	if mime is None:
 		mime = "application/octet-stream"
 	return FileResponse(file, media_type=mime)
 	"""
 	return FileResponse(file)
 
 
-async def serve_dir(directory: Path):
+async def serve_dir(directory: Path, base_dir: Path = SWD):
+	# TODO add docstring and include: base_dir must be absolute
+	directory = directory.absolute()
 	if not directory.is_dir():
 		return PlainTextResponse(
 			f"the following directory was not found:\n\t{directory}",
 			status_code=404
 		)
-	directory_index = directory.joinpath("./index.html")
-	if directory_index.is_file():
-		index_html_url = "/" + str(directory_index.relative_to(SWD).as_posix())
-		print(f"index.html found. redirecting to:\n\t{index_html_url}")
-		return RedirectResponse(index_html_url)
-	dir_head = directory.relative_to(SWD)
+	dir_head = directory.relative_to(base_dir).as_posix()
 	dir_links: dict[str, str] = dict()  # key: href_path, value: title
 	dir_links["./.."] = ".."
 	for subpath in directory.iterdir():
-		rel_subpath = subpath.relative_to(directory)
+		rel_subpath = subpath.relative_to(directory).as_posix()
 		prefix = "./"
 		suffix = "" if subpath.is_file() else "/"
 		href = prefix + str(rel_subpath) + suffix
 		title = str(rel_subpath) + suffix
 		dir_links[href] = title
 	dir_links_html_li: list[str] = [f"""
 	<li><a href={qoute(href)}>{title}</a></li>
```

#### html2text {}

```diff
@@ -1,26 +1,25 @@
-from pathlib import Path from fastapi.responses import ( FileResponse,
-HTMLResponse, PlainTextResponse, RedirectResponse, ) from .config import SWD
-from .utils import qoute async def serve_file(file: Path): if not file.is_file
-(): return PlainTextResponse(f"the following file was not found:\n\t{file}",
+from pathlib import Path from fastapi.responses import FileResponse,
+HTMLResponse, PlainTextResponse from .config import SWD from .utils import
+qoute async def serve_file(file: Path): if not file.is_file(): return
+PlainTextResponse(f"the following file was not found:\n\t{file}",
 status_code=404) """ fastapi takes care of custom mime types when they're added
 to the built-in `mintypes` library mime, _ = mimetypes.guess_type(file) if mime
 is None: mime = "application/octet-stream" return FileResponse(file,
 media_type=mime) """ return FileResponse(file) async def serve_dir(directory:
-Path): if not directory.is_dir(): return PlainTextResponse( f"the following
-directory was not found:\n\t{directory}", status_code=404 ) directory_index =
-directory.joinpath("./index.html") if directory_index.is_file(): index_html_url
-= "/" + str(directory_index.relative_to(SWD).as_posix()) print(f"index.html
-found. redirecting to:\n\t{index_html_url}") return RedirectResponse
-(index_html_url) dir_head = directory.relative_to(SWD) dir_links: dict[str,
-str] = dict() # key: href_path, value: title dir_links["./.."] = ".." for
-subpath in directory.iterdir(): rel_subpath = subpath.relative_to(directory)
-prefix = "./" suffix = "" if subpath.is_file() else "/" href = prefix + str
-(rel_subpath) + suffix title = str(rel_subpath) + suffix dir_links[href] =
-title dir_links_html_li: list[str] = [f"""
+Path, base_dir: Path = SWD): # TODO add docstring and include: base_dir must be
+absolute directory = directory.absolute() if not directory.is_dir(): return
+PlainTextResponse( f"the following directory was not found:\n\t{directory}",
+status_code=404 ) dir_head = directory.relative_to(base_dir).as_posix()
+dir_links: dict[str, str] = dict() # key: href_path, value: title dir_links
+["./.."] = ".." for subpath in directory.iterdir(): rel_subpath =
+subpath.relative_to(directory).as_posix() prefix = "./" suffix = "" if
+subpath.is_file() else "/" href = prefix + str(rel_subpath) + suffix title =
+str(rel_subpath) + suffix dir_links[href] = title dir_links_html_li: list[str]
+= [f"""
 {title}
 """ for href, title in dir_links.items()] html = f"""
 ****** Directory listing for: {qoute(dir_head)} ******
 ===============================================================================
     * {"".join(dir_links_html_li)}
 ===============================================================================
 """ return HTMLResponse(html)
```

### Comparing `fastdev-py-0.2.2/src/fastdev/preprocessor/temp.py.bak` & `fastdev-py-0.3.0/src/fastdev/preprocessor/temp.py.bak`

 * *Files identical despite different names*

### Comparing `fastdev-py-0.2.2/src/fastdev/ts_serving.py` & `fastdev-py-0.3.0/src/fastdev/ts_serving.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from asyncio import Future
+from pathlib import Path
 from subprocess import Popen
 from urllib.parse import urljoin
 from fastapi.responses import PlainTextResponse, Response
 from .config import SWD, ESBuildConfig, ModDir, Port
 from .utils import post_data, qoute
 
 BUILD_SERVER_PORT = 3000  # the port on which `deno_lts_esbuild.ts` listens for build requests
@@ -10,26 +11,26 @@
 build_server_path = ModDir.joinpath("./builders/deno_lts_esbuild.ts")
 build_server_callback_path = "/build_server_loaded"
 build_server_callback = f"http://localhost:{Port}{build_server_callback_path}"
 build_server_url = f"http://localhost:{BUILD_SERVER_PORT}"
 build_server_process = Popen(f"deno run -A {qoute(build_server_path)} --port={BUILD_SERVER_PORT} --callback={qoute(build_server_callback)}", cwd=SWD)
 
 
-async def serve_ts(url_path: str):
+async def serve_ts(file: Path):
 	await build_server_loaded_promise
-	# file_abspath = SWD.joinpath(url_path)
+	file_abspath = file.absolute().relative_to(SWD).as_posix()
 	output_js_response = post_data(
 		urljoin(build_server_url, "compile"),
-		{**ESBuildConfig, "path": url_path},
+		{**ESBuildConfig, "path": str(file_abspath)},
 		timeout=50_000,
 		headers={"content-type": "application/json"},
 	)
 	if output_js_response is None:
 		return PlainTextResponse(
-			f"failed to transpile and bundle the requested file:\n\t{url_path}",
+			f"failed to transpile and bundle the requested file:\n\t{file}",
 			status_code=503
 		)
 	return Response(
 		output_js_response["content"],
 		status_code=output_js_response["status_code"],
 		media_type="text/javascript"
 	)
```

### Comparing `fastdev-py-0.2.2/src/fastdev/utils.py` & `fastdev-py-0.3.0/src/fastdev/utils.py`

 * *Files identical despite different names*

### Comparing `fastdev-py-0.2.2/PKG-INFO` & `fastdev-py-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastdev-py
-Version: 0.2.2
+Version: 0.3.0
 Summary: FastAPI development server that JIT preprocess TS, TSX, SCSS, etc... files.
 Keywords: devserver,dev-server,devtools,sever,liveserver,live-server
 Author: Omar Azmi
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: fastapi
 Project-URL: Homepage, https://github.com/omar-azmi/fastdev_py
```

