# Comparing `tmp/pysdl2-dll-2.26.2.tar.gz` & `tmp/pysdl2-dll-2.26.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysdl2-dll-2.26.2.tar", last modified: Sun Jan  8 17:52:33 2023, max compression
+gzip compressed data, was "pysdl2-dll-2.26.5.tar", last modified: Tue May  2 14:17:28 2023, max compression
```

## Comparing `pysdl2-dll-2.26.2.tar` & `pysdl2-dll-2.26.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-08 17:52:33.059845 pysdl2-dll-2.26.2/
--rw-r--r--   0 root         (0) root         (0)    16725 2023-01-08 17:52:32.000000 pysdl2-dll-2.26.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       34 2023-01-08 17:52:32.000000 pysdl2-dll-2.26.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4526 2023-01-08 17:52:33.059845 pysdl2-dll-2.26.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3733 2023-01-08 17:52:32.000000 pysdl2-dll-2.26.2/README.md
--rw-r--r--   0 root         (0) root         (0)    19001 2023-01-08 17:52:32.000000 pysdl2-dll-2.26.2/getdlls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-08 17:52:33.058845 pysdl2-dll-2.26.2/pysdl2_dll.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4526 2023-01-08 17:52:33.000000 pysdl2-dll-2.26.2/pysdl2_dll.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      236 2023-01-08 17:52:33.000000 pysdl2-dll-2.26.2/pysdl2_dll.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-08 17:52:33.000000 pysdl2-dll-2.26.2/pysdl2_dll.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-01-08 17:52:33.000000 pysdl2-dll-2.26.2/pysdl2_dll.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-08 17:52:33.059845 pysdl2-dll-2.26.2/sdl2dll/
--rw-r--r--   0 root         (0) root         (0)      419 2023-01-08 17:52:32.000000 pysdl2-dll-2.26.2/sdl2dll/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2567 2023-01-08 17:52:32.000000 pysdl2-dll-2.26.2/sdl2dll/initcheck.py
--rw-r--r--   0 root         (0) root         (0)      116 2023-01-08 17:52:33.060845 pysdl2-dll-2.26.2/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     2532 2023-01-08 17:52:32.000000 pysdl2-dll-2.26.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:17:28.111384 pysdl2-dll-2.26.5/
+-rw-r--r--   0 root         (0) root         (0)    16725 2023-05-02 14:17:26.000000 pysdl2-dll-2.26.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       34 2023-05-02 14:17:26.000000 pysdl2-dll-2.26.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4322 2023-05-02 14:17:28.111384 pysdl2-dll-2.26.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3529 2023-05-02 14:17:26.000000 pysdl2-dll-2.26.5/README.md
+-rw-r--r--   0 root         (0) root         (0)    19001 2023-05-02 14:17:26.000000 pysdl2-dll-2.26.5/getdlls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:17:28.110384 pysdl2-dll-2.26.5/pysdl2_dll.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4322 2023-05-02 14:17:28.000000 pysdl2-dll-2.26.5/pysdl2_dll.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      236 2023-05-02 14:17:28.000000 pysdl2-dll-2.26.5/pysdl2_dll.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 14:17:28.000000 pysdl2-dll-2.26.5/pysdl2_dll.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-02 14:17:28.000000 pysdl2-dll-2.26.5/pysdl2_dll.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:17:28.111384 pysdl2-dll-2.26.5/sdl2dll/
+-rw-r--r--   0 root         (0) root         (0)      419 2023-05-02 14:17:26.000000 pysdl2-dll-2.26.5/sdl2dll/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2567 2023-05-02 14:17:26.000000 pysdl2-dll-2.26.5/sdl2dll/initcheck.py
+-rw-r--r--   0 root         (0) root         (0)      116 2023-05-02 14:17:28.111384 pysdl2-dll-2.26.5/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     2534 2023-05-02 14:17:26.000000 pysdl2-dll-2.26.5/setup.py
```

### Comparing `pysdl2-dll-2.26.2/LICENSE` & `pysdl2-dll-2.26.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pysdl2-dll-2.26.2/PKG-INFO` & `pysdl2-dll-2.26.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysdl2-dll
-Version: 2.26.2
+Version: 2.26.5
 Summary: Pre-built SDL2 binaries for PySDL2
 Home-page: https://github.com/a-hurst/pysdl2-dll
 Author: Austin Hurst
 Author-email: mynameisaustinhurst@gmail.com
 License: Mozilla Public License Version 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -28,15 +28,17 @@
 
 It uses the official SDL2, SDL2\_mixer, SDL2\_ttf, and SDL2\_image binaries for macOS and Windows, as well as [unofficial SDL2\_gfx binaries](https://github.com/a-hurst/sdl2gfx-builds) for the same platforms. For Linux, the SDL2 binaries and their dependencies are all built from source using the official Python [manylinux](https://github.com/pypa/manylinux) images for maximum compatibility.
 
 The latest release includes the following versions of the SDL2 binaries:
 
 SDL2 | SDL2\_ttf | SDL2\_mixer | SDL2\_image | SDL2\_gfx
 --- | --- | --- | --- | ---
-2.26.2 | 2.20.0 | 2.6.0 | 2.6.0 | 1.0.4
+2.26.5 | 2.20.0 | 2.6.0 | 2.6.0 | 1.0.4
+
+Note that the mixer and image libraries are pinned at their current versions until their next major release due to a regression in the macOS binaries.
 
 
 ## Installation
 
 You can install the latest version of pysdl2-dll via pip:
 
 ```bash
@@ -44,15 +46,15 @@
 ```
 
 
 ## Requirements
 
 At present, the following platforms are supported:
 
-* macOS (10.9+, 64-bit x86)
+* macOS (10.11+, 64-bit x86)
 * macOS (11.0+, 64-bit ARM)
 * Windows (32-bit x86)
 * Windows (64-bit x86)
 * Linux (32-bit x86)
 * Linux (64-bit x86)
 * Linux (64-bit ARM)
 
@@ -65,19 +67,17 @@
 ```
 
 Because the wheels are not built against any specfic version of Python, pysdl2-dll supports all versions and implementations of Python that are supported by PySDL2.
 
 
 ### Linux Requirements
 
-There are currently two versions the Linux wheels: "legacy" wheels based on the `manylinux2014` standard (for 32-bit and 64-bit x86), and "modern" wheels based on the `manylinux_2_24` standard (for 64-bit x86 and 64-bit ARM only). The `manylinux_2_24` SDL2 binaries require a more recent version of Linux, but offer dynamic support for additional features such as Wayland windowing, Pipewire/sndio/JACK audio, and OpenGL ES v1 rendering.
-
-You must have pip 19.3 or newer to install the `manylinux2014` wheels, and pip 20.3 or newer to install the `manylinux_2_24` wheels. Distributions that use musl C instead of glibc (e.g. Alpine Linux) are not supported.
+There are currently two versions the Linux wheels: "legacy" wheels based on the `manylinux2014` standard (for 32-bit and 64-bit x86), and "modern" wheels based on the `manylinux_2_28` standard (for 64-bit x86 and 64-bit ARM only). The `manylinux_2_28` SDL2 binaries require a more recent version of Linux, but offer dynamic support for additional features such as native Wayland windowing, Pipewire audio, and Vulkan rendering.
 
-**Note**: pysdl2-dll is currently not built with libdecor support, meaning that native Wayland (non-XWayland) window decorations will be unavailable when using these binaries (see issue #9 for details). Given that SDL2 defaults to using XWayland this shouldn't be an issue for most users, but suggestions and/or PRs to fix the issue are welcome!
+You must have pip 19.3 or newer to install the `manylinux2014` wheels, and pip 20.3 or newer to install the `manylinux_2_28` wheels. Distributions that use musl C instead of glibc (e.g. Alpine Linux) are not supported.
 
 
 ## Usage
 
 If you are using PySDL2 0.9.7 or later, you don't need to do anything special to use the pysdl2-dll binaries in your project: PySDL2 will load them automatically (and print a message indicating such) if they are available. For older versions of PySDL2, you will need to import this module manually in your scripts (`import sdl2dll`) before PySDL2 is imported.
 
 To override pysdl2-dll and use a different set of binaries, you can set the `PYSDL2_DLL_PATH` environment variable to the path of the folder containing the binaries you want to use instead, or alternatively set it to "system" to force PySDL2 to use the system install of SDL2 if available (e.g. SDL2 installed with `brew` on macOS).
```

### Comparing `pysdl2-dll-2.26.2/README.md` & `pysdl2-dll-2.26.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 
 It uses the official SDL2, SDL2\_mixer, SDL2\_ttf, and SDL2\_image binaries for macOS and Windows, as well as [unofficial SDL2\_gfx binaries](https://github.com/a-hurst/sdl2gfx-builds) for the same platforms. For Linux, the SDL2 binaries and their dependencies are all built from source using the official Python [manylinux](https://github.com/pypa/manylinux) images for maximum compatibility.
 
 The latest release includes the following versions of the SDL2 binaries:
 
 SDL2 | SDL2\_ttf | SDL2\_mixer | SDL2\_image | SDL2\_gfx
 --- | --- | --- | --- | ---
-2.26.2 | 2.20.0 | 2.6.0 | 2.6.0 | 1.0.4
+2.26.5 | 2.20.0 | 2.6.0 | 2.6.0 | 1.0.4
+
+Note that the mixer and image libraries are pinned at their current versions until their next major release due to a regression in the macOS binaries.
 
 
 ## Installation
 
 You can install the latest version of pysdl2-dll via pip:
 
 ```bash
@@ -23,15 +25,15 @@
 ```
 
 
 ## Requirements
 
 At present, the following platforms are supported:
 
-* macOS (10.9+, 64-bit x86)
+* macOS (10.11+, 64-bit x86)
 * macOS (11.0+, 64-bit ARM)
 * Windows (32-bit x86)
 * Windows (64-bit x86)
 * Linux (32-bit x86)
 * Linux (64-bit x86)
 * Linux (64-bit ARM)
 
@@ -44,19 +46,17 @@
 ```
 
 Because the wheels are not built against any specfic version of Python, pysdl2-dll supports all versions and implementations of Python that are supported by PySDL2.
 
 
 ### Linux Requirements
 
-There are currently two versions the Linux wheels: "legacy" wheels based on the `manylinux2014` standard (for 32-bit and 64-bit x86), and "modern" wheels based on the `manylinux_2_24` standard (for 64-bit x86 and 64-bit ARM only). The `manylinux_2_24` SDL2 binaries require a more recent version of Linux, but offer dynamic support for additional features such as Wayland windowing, Pipewire/sndio/JACK audio, and OpenGL ES v1 rendering.
-
-You must have pip 19.3 or newer to install the `manylinux2014` wheels, and pip 20.3 or newer to install the `manylinux_2_24` wheels. Distributions that use musl C instead of glibc (e.g. Alpine Linux) are not supported.
+There are currently two versions the Linux wheels: "legacy" wheels based on the `manylinux2014` standard (for 32-bit and 64-bit x86), and "modern" wheels based on the `manylinux_2_28` standard (for 64-bit x86 and 64-bit ARM only). The `manylinux_2_28` SDL2 binaries require a more recent version of Linux, but offer dynamic support for additional features such as native Wayland windowing, Pipewire audio, and Vulkan rendering.
 
-**Note**: pysdl2-dll is currently not built with libdecor support, meaning that native Wayland (non-XWayland) window decorations will be unavailable when using these binaries (see issue #9 for details). Given that SDL2 defaults to using XWayland this shouldn't be an issue for most users, but suggestions and/or PRs to fix the issue are welcome!
+You must have pip 19.3 or newer to install the `manylinux2014` wheels, and pip 20.3 or newer to install the `manylinux_2_28` wheels. Distributions that use musl C instead of glibc (e.g. Alpine Linux) are not supported.
 
 
 ## Usage
 
 If you are using PySDL2 0.9.7 or later, you don't need to do anything special to use the pysdl2-dll binaries in your project: PySDL2 will load them automatically (and print a message indicating such) if they are available. For older versions of PySDL2, you will need to import this module manually in your scripts (`import sdl2dll`) before PySDL2 is imported.
 
 To override pysdl2-dll and use a different set of binaries, you can set the `PYSDL2_DLL_PATH` environment variable to the path of the folder containing the binaries you want to use instead, or alternatively set it to "system" to force PySDL2 to use the system install of SDL2 if available (e.g. SDL2 installed with `brew` on macOS).
```

### Comparing `pysdl2-dll-2.26.2/getdlls.py` & `pysdl2-dll-2.26.5/getdlls.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 except ImportError:
     from urllib2 import urlopen # Python 2
 
 
 libraries = ['SDL2', 'SDL2_mixer', 'SDL2_ttf', 'SDL2_image', 'SDL2_gfx']
 
 libversions = {
-    'SDL2': '2.26.2',
+    'SDL2': '2.26.5',
     'SDL2_mixer': '2.6.0',
     'SDL2_ttf': '2.20.0',
     'SDL2_image': '2.6.0',
     'SDL2_gfx': '1.0.4'
 }
 
 url_fmt = 'https://github.com/libsdl-org/SDL{LIB}/releases/download/release-{0}/SDL2{LIB}-{0}{1}'
```

### Comparing `pysdl2-dll-2.26.2/pysdl2_dll.egg-info/PKG-INFO` & `pysdl2-dll-2.26.5/pysdl2_dll.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysdl2-dll
-Version: 2.26.2
+Version: 2.26.5
 Summary: Pre-built SDL2 binaries for PySDL2
 Home-page: https://github.com/a-hurst/pysdl2-dll
 Author: Austin Hurst
 Author-email: mynameisaustinhurst@gmail.com
 License: Mozilla Public License Version 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -28,15 +28,17 @@
 
 It uses the official SDL2, SDL2\_mixer, SDL2\_ttf, and SDL2\_image binaries for macOS and Windows, as well as [unofficial SDL2\_gfx binaries](https://github.com/a-hurst/sdl2gfx-builds) for the same platforms. For Linux, the SDL2 binaries and their dependencies are all built from source using the official Python [manylinux](https://github.com/pypa/manylinux) images for maximum compatibility.
 
 The latest release includes the following versions of the SDL2 binaries:
 
 SDL2 | SDL2\_ttf | SDL2\_mixer | SDL2\_image | SDL2\_gfx
 --- | --- | --- | --- | ---
-2.26.2 | 2.20.0 | 2.6.0 | 2.6.0 | 1.0.4
+2.26.5 | 2.20.0 | 2.6.0 | 2.6.0 | 1.0.4
+
+Note that the mixer and image libraries are pinned at their current versions until their next major release due to a regression in the macOS binaries.
 
 
 ## Installation
 
 You can install the latest version of pysdl2-dll via pip:
 
 ```bash
@@ -44,15 +46,15 @@
 ```
 
 
 ## Requirements
 
 At present, the following platforms are supported:
 
-* macOS (10.9+, 64-bit x86)
+* macOS (10.11+, 64-bit x86)
 * macOS (11.0+, 64-bit ARM)
 * Windows (32-bit x86)
 * Windows (64-bit x86)
 * Linux (32-bit x86)
 * Linux (64-bit x86)
 * Linux (64-bit ARM)
 
@@ -65,19 +67,17 @@
 ```
 
 Because the wheels are not built against any specfic version of Python, pysdl2-dll supports all versions and implementations of Python that are supported by PySDL2.
 
 
 ### Linux Requirements
 
-There are currently two versions the Linux wheels: "legacy" wheels based on the `manylinux2014` standard (for 32-bit and 64-bit x86), and "modern" wheels based on the `manylinux_2_24` standard (for 64-bit x86 and 64-bit ARM only). The `manylinux_2_24` SDL2 binaries require a more recent version of Linux, but offer dynamic support for additional features such as Wayland windowing, Pipewire/sndio/JACK audio, and OpenGL ES v1 rendering.
-
-You must have pip 19.3 or newer to install the `manylinux2014` wheels, and pip 20.3 or newer to install the `manylinux_2_24` wheels. Distributions that use musl C instead of glibc (e.g. Alpine Linux) are not supported.
+There are currently two versions the Linux wheels: "legacy" wheels based on the `manylinux2014` standard (for 32-bit and 64-bit x86), and "modern" wheels based on the `manylinux_2_28` standard (for 64-bit x86 and 64-bit ARM only). The `manylinux_2_28` SDL2 binaries require a more recent version of Linux, but offer dynamic support for additional features such as native Wayland windowing, Pipewire audio, and Vulkan rendering.
 
-**Note**: pysdl2-dll is currently not built with libdecor support, meaning that native Wayland (non-XWayland) window decorations will be unavailable when using these binaries (see issue #9 for details). Given that SDL2 defaults to using XWayland this shouldn't be an issue for most users, but suggestions and/or PRs to fix the issue are welcome!
+You must have pip 19.3 or newer to install the `manylinux2014` wheels, and pip 20.3 or newer to install the `manylinux_2_28` wheels. Distributions that use musl C instead of glibc (e.g. Alpine Linux) are not supported.
 
 
 ## Usage
 
 If you are using PySDL2 0.9.7 or later, you don't need to do anything special to use the pysdl2-dll binaries in your project: PySDL2 will load them automatically (and print a message indicating such) if they are available. For older versions of PySDL2, you will need to import this module manually in your scripts (`import sdl2dll`) before PySDL2 is imported.
 
 To override pysdl2-dll and use a different set of binaries, you can set the `PYSDL2_DLL_PATH` environment variable to the path of the folder containing the binaries you want to use instead, or alternatively set it to "system" to force PySDL2 to use the system install of SDL2 if available (e.g. SDL2 installed with `brew` on macOS).
```

### Comparing `pysdl2-dll-2.26.2/sdl2dll/initcheck.py` & `pysdl2-dll-2.26.5/sdl2dll/initcheck.py`

 * *Files identical despite different names*

### Comparing `pysdl2-dll-2.26.2/setup.py` & `pysdl2-dll-2.26.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,17 +32,17 @@
 try:
     from wheel.bdist_wheel import bdist_wheel
 
     class bdist_wheel_half_pure(bdist_wheel):
 
         def get_tag(self):
             if 'macosx' in platform:
-                system = 'macosx_10_9_universal2'
+                system = 'macosx_10_11_universal2'
                 if os.getenv('MACOS_LEGACY_WHEEL'):
-                    system = 'macosx_10_9_x86_64'
+                    system = 'macosx_10_11_x86_64'
             elif platform in ['win32', 'win-amd64']:
                 system = platform.replace('-', '_')
             elif 'manylinux' in platform:
                 arch = get_platform().split('-')[-1]
                 system = '_'.join([platform, arch])
             else:
                 system = 'any'
@@ -57,15 +57,15 @@
 # Install the package
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
 	name='pysdl2-dll',
-	version='2.26.2',
+	version='2.26.5',
 	author='Austin Hurst',
 	author_email='mynameisaustinhurst@gmail.com',
     license='Mozilla Public License Version 2.0',
     description='Pre-built SDL2 binaries for PySDL2',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/a-hurst/pysdl2-dll',
```

