# Comparing `tmp/elegantmotd-0.2.4.tar.gz` & `tmp/elegantmotd-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elegantmotd-0.2.4.tar", max compression
+gzip compressed data, was "elegantmotd-0.2.5.tar", max compression
```

## Comparing `elegantmotd-0.2.4.tar` & `elegantmotd-0.2.5.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0      785 2023-04-24 12:41:45.364385 elegantmotd-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     1674 2023-04-24 12:37:35.609096 elegantmotd-0.2.4/README.md
--rw-r--r--   0        0        0        0 2023-04-24 09:50:20.677486 elegantmotd-0.2.4/src/elegantmotd/__init__.py
--rw-r--r--   0        0        0      212 2023-04-24 08:04:35.982872 elegantmotd-0.2.4/src/elegantmotd/constants.py
--rw-r--r--   0        0        0      845 2023-04-24 09:50:20.670118 elegantmotd-0.2.4/src/elegantmotd/cpu.py
--rw-r--r--   0        0        0     1068 2023-04-24 08:04:35.982872 elegantmotd-0.2.4/src/elegantmotd/disk.py
--rw-r--r--   0        0        0      308 2023-04-24 08:04:35.982872 elegantmotd-0.2.4/src/elegantmotd/load.py
--rw-r--r--   0        0        0      379 2023-04-24 08:04:35.982872 elegantmotd-0.2.4/src/elegantmotd/loggedinusers.py
--rw-r--r--   0        0        0     1468 2023-04-24 08:04:35.982872 elegantmotd-0.2.4/src/elegantmotd/memory.py
--rw-r--r--   0        0        0     2198 2023-04-24 12:12:35.623458 elegantmotd-0.2.4/src/elegantmotd/motd.py
--rw-r--r--   0        0        0      519 2023-04-24 08:04:35.986528 elegantmotd-0.2.4/src/elegantmotd/network.py
--rw-r--r--   0        0        0      291 2023-04-24 08:04:35.987213 elegantmotd-0.2.4/src/elegantmotd/process.py
--rw-r--r--   0        0        0      345 2023-04-24 08:04:35.987213 elegantmotd-0.2.4/src/elegantmotd/sysinfo.py
--rw-r--r--   0        0        0     1455 2023-04-24 08:04:35.987770 elegantmotd-0.2.4/src/elegantmotd/temperature.py
--rw-r--r--   0        0        0     2656 1970-01-01 00:00:00.000000 elegantmotd-0.2.4/setup.py
--rw-r--r--   0        0        0     2444 1970-01-01 00:00:00.000000 elegantmotd-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1607 2023-05-02 17:18:20.672993 elegantmotd-0.2.5/README.md
+-rw-r--r--   0        0        0      760 2023-05-02 18:26:28.872815 elegantmotd-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-02 17:59:59.267653 elegantmotd-0.2.5/src/elegantmotd/__init__.py
+-rw-r--r--   0        0        0      200 2023-05-02 17:18:20.672993 elegantmotd-0.2.5/src/elegantmotd/constants.py
+-rw-r--r--   0        0        0      819 2023-05-02 18:18:23.387757 elegantmotd-0.2.5/src/elegantmotd/cpu.py
+-rw-r--r--   0        0        0     1036 2023-05-02 18:07:36.104712 elegantmotd-0.2.5/src/elegantmotd/disk.py
+-rw-r--r--   0        0        0      294 2023-05-02 18:07:36.120712 elegantmotd-0.2.5/src/elegantmotd/load.py
+-rw-r--r--   0        0        0      365 2023-05-02 18:07:36.104712 elegantmotd-0.2.5/src/elegantmotd/loggedinusers.py
+-rw-r--r--   0        0        0     1429 2023-05-02 18:07:36.132712 elegantmotd-0.2.5/src/elegantmotd/memory.py
+-rw-r--r--   0        0        0     2126 2023-05-02 18:14:12.401738 elegantmotd-0.2.5/src/elegantmotd/motd.py
+-rw-r--r--   0        0        0      500 2023-05-02 18:07:36.116712 elegantmotd-0.2.5/src/elegantmotd/network.py
+-rw-r--r--   0        0        0      279 2023-05-02 18:18:23.387757 elegantmotd-0.2.5/src/elegantmotd/process.py
+-rw-r--r--   0        0        0      286 2023-05-02 18:19:32.351205 elegantmotd-0.2.5/src/elegantmotd/sysinfo.py
+-rw-r--r--   0        0        0     1414 2023-05-02 18:07:36.112712 elegantmotd-0.2.5/src/elegantmotd/temperature.py
+-rw-r--r--   0        0        0     2444 1970-01-01 00:00:00.000000 elegantmotd-0.2.5/PKG-INFO
```

### Comparing `elegantmotd-0.2.4/pyproject.toml` & `elegantmotd-0.2.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-[tool.poetry]
-name = "elegantmotd"
-version = "0.2.4"
-authors = ["Emerick Biron <emerick.biron@gmail.com>"]
-readme = "README.md"
-description = "A visually appealing and informative Message of the Day (MOTD) generator for Linux systems."
-homepage = "https://github.com/emerick-biron/elegantmotd"
-repository = "https://github.com/emerick-biron/elegantmotd.git"
-keywords = ["motd", "system", "information", "console", "dashboard"]
-license = "MIT"
-packages = [{ include = "elegantmotd", from = "src" }]
-
-[tool.poetry.dependencies]
-python = "^3.10"
-rich = "^13.3.4"
-psutil = "^5.9.5"
-netifaces = "^0.11.0"
-art = "^5.9"
-
-[tool.poetry.scripts]
-elegantmotd="elegantmotd.motd:display"
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "elegantmotd"
+version = "0.2.5"
+authors = ["Emerick Biron <emerick.biron@gmail.com>"]
+readme = "README.md"
+description = "A visually appealing and informative Message of the Day (MOTD) generator for Linux systems."
+homepage = "https://github.com/emerick-biron/elegantmotd"
+repository = "https://github.com/emerick-biron/elegantmotd.git"
+keywords = ["motd", "system", "information", "console", "dashboard"]
+license = "MIT"
+packages = [{ include = "elegantmotd", from = "src" }]
+
+[tool.poetry.dependencies]
+python = "^3.10"
+rich = "^13.3.4"
+psutil = "^5.9.5"
+netifaces = "^0.11.0"
+art = "^5.9"
+
+[tool.poetry.scripts]
+elegantmotd="elegantmotd.motd:display"
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `elegantmotd-0.2.4/README.md` & `elegantmotd-0.2.5/README.md`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-# ElegantMOTD
-
-ElegantMOTD is a Python-based Message of the Day (MOTD) generator for displaying system information in a visually
-appealing and informative manner. It works on Linux systems and provides details such as system load, disk usage, memory
-usage, swap usage, temperature, network interfaces, CPU usage, and more.
-
-## Features
-
-- Rich, colorful text-based output.
-- Displays various system information.
-- Customizable display options.
-- Easy to use and integrate into your system.
-
-## Installation
-- Clone this repository:
-```bash
-git clone https://github.com/yourusername/elegantmotd.git
-cd elegantmotd
-```
-- Create a virtual environment and activate it:
-
-```bash
-python3 -m venv venv
-source venv/bin/activate
-```
-
-- Install the required dependencies:
-```bash
-poetry build 
-```
-
-## Usage
-
-To display the Message of the Day, run the following command:
-
-```bash
-elegantmotd
-```
-
-## Output
-
-![Output](resources/output.png)
-
-## Customization
-
-You can customize the output by modifying the `motd.py` file and adding or removing system information modules as per your preference. The available modules are:
-
-- Load
-- Disk
-- Memory
-- Temperature
-- Process
-- LoggedInUsers
-- Network
-- CPU
-
-To add or remove a module, simply add or remove the corresponding import statement and the respective class instance from the `sysinfos` list in the `display()` function.
-
-## Contributing
-
-Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
-
-Please make sure to update tests as appropriate.
-
-## License
-
-[MIT](https://choosealicense.com/licenses/mit/)
+# ElegantMOTD
+
+ElegantMOTD is a Python-based Message of the Day (MOTD) generator for displaying system information in a visually
+appealing and informative manner. It works on Linux systems and provides details such as system load, disk usage, memory
+usage, swap usage, temperature, network interfaces, CPU usage, and more.
+
+## Features
+
+- Rich, colorful text-based output.
+- Displays various system information.
+- Customizable display options.
+- Easy to use and integrate into your system.
+
+## Installation
+- Clone this repository:
+```bash
+git clone https://github.com/yourusername/elegantmotd.git
+cd elegantmotd
+```
+- Create a virtual environment and activate it:
+
+```bash
+python3 -m venv venv
+source venv/bin/activate
+```
+
+- Install the required dependencies:
+```bash
+poetry build 
+```
+
+## Usage
+
+To display the Message of the Day, run the following command:
+
+```bash
+elegantmotd
+```
+
+## Output
+
+![Output](resources/output.png)
+
+## Customization
+
+You can customize the output by modifying the `motd.py` file and adding or removing system information modules as per your preference. The available modules are:
+
+- Load
+- Disk
+- Memory
+- Temperature
+- Process
+- LoggedInUsers
+- Network
+- CPU
+
+To add or remove a module, simply add or remove the corresponding import statement and the respective class instance from the `sysinfos` list in the `display()` function.
+
+## Contributing
+
+Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
+
+Please make sure to update tests as appropriate.
+
+## License
+
+[MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `elegantmotd-0.2.4/src/elegantmotd/cpu.py` & `elegantmotd-0.2.5/src/elegantmotd/cpu.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from typing import Dict
-
-import psutil
-from rich.console import RenderableType
-from rich.progress import Progress, BarColumn, TaskProgressColumn
-
-from .constants import GREEN, RED, ORANGE, YELLOW
-from .sysinfo import SysInfo
-
-
-class CPU(SysInfo):
-    def _get_infos(self) -> Dict[RenderableType, RenderableType]:
-        cpu_percent = psutil.cpu_percent()
-        color = (
-            GREEN if cpu_percent < 25
-            else YELLOW if cpu_percent < 50
-            else ORANGE if cpu_percent < 75
-            else RED
-        )
-        progress = Progress(
-            BarColumn(complete_style=color, bar_width=10, finished_style=RED),
-            TaskProgressColumn()
-        )
-        progress.add_task("cpu_percent", total=100, completed=round(cpu_percent))
-        infos = {"CPU": progress}
-        return infos
+from typing import Dict
+
+import psutil
+from rich.console import RenderableType
+from rich.progress import Progress, BarColumn, TaskProgressColumn
+
+from .constants import GREEN, RED, ORANGE, YELLOW
+from .sysinfo import SysInfo
+
+
+class CPU(SysInfo):
+    def _get_infos(self) -> Dict[RenderableType, RenderableType]:
+        cpu_percent = psutil.cpu_percent()
+        color = (
+            GREEN if cpu_percent < 25
+            else YELLOW if cpu_percent < 50
+            else ORANGE if cpu_percent < 75
+            else RED
+        )
+        progress = Progress(
+            BarColumn(complete_style=color, bar_width=10, finished_style=RED),
+            TaskProgressColumn()
+        )
+        progress.add_task("cpu_percent", total=100, completed=round(cpu_percent))
+        infos = {"CPU": progress}
+        return infos
```

### Comparing `elegantmotd-0.2.4/src/elegantmotd/disk.py` & `elegantmotd-0.2.5/src/elegantmotd/disk.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-import shutil
-from typing import Dict
-
-from rich.console import RenderableType
-from rich.progress import Progress, BarColumn, TaskProgressColumn, TextColumn
-
-from .constants import GB, GREEN, YELLOW, ORANGE, RED
-from .sysinfo import SysInfo
-
-
-class Disk(SysInfo):
-    def _get_infos(self) -> Dict[RenderableType, RenderableType]:
-        disk_usage = shutil.disk_usage('/')
-        total_space = f"{round(disk_usage.total / GB, 2)}GB"
-        usage_percent = round((disk_usage.used / disk_usage.total * 100), 1)
-        color = (
-            GREEN if usage_percent < 25
-            else YELLOW if usage_percent < 50
-            else ORANGE if usage_percent < 75
-            else RED
-        )
-
-        progress = Progress(
-            BarColumn(complete_style=color, bar_width=10, finished_style=RED),
-            TaskProgressColumn(),
-            TextColumn(f" of {total_space}")
-        )
-        progress.add_task("progress", total=100, completed=round(usage_percent))
-
-        infos = {"Usage of /": progress}
-
-        return infos
+import shutil
+from typing import Dict
+
+from rich.console import RenderableType
+from rich.progress import Progress, BarColumn, TaskProgressColumn, TextColumn
+
+from .constants import GB, GREEN, YELLOW, ORANGE, RED
+from .sysinfo import SysInfo
+
+
+class Disk(SysInfo):
+    def _get_infos(self) -> Dict[RenderableType, RenderableType]:
+        disk_usage = shutil.disk_usage('/')
+        total_space = f"{round(disk_usage.total / GB, 2)}GB"
+        usage_percent = round((disk_usage.used / disk_usage.total * 100), 1)
+        color = (
+            GREEN if usage_percent < 25
+            else YELLOW if usage_percent < 50
+            else ORANGE if usage_percent < 75
+            else RED
+        )
+
+        progress = Progress(
+            BarColumn(complete_style=color, bar_width=10, finished_style=RED),
+            TaskProgressColumn(),
+            TextColumn(f" of {total_space}")
+        )
+        progress.add_task("progress", total=100, completed=round(usage_percent))
+
+        infos = {"Usage of /": progress}
+
+        return infos
```

### Comparing `elegantmotd-0.2.4/src/elegantmotd/memory.py` & `elegantmotd-0.2.5/src/elegantmotd/memory.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from typing import Dict
-
-import psutil
-from rich.console import RenderableType
-from rich.progress import Progress, BarColumn, TaskProgressColumn, TextColumn
-
-from .constants import GB, GREEN, YELLOW, ORANGE, RED
-from .sysinfo import SysInfo
-
-
-class Memory(SysInfo):
-    def _get_infos(self) -> Dict[RenderableType, RenderableType]:
-        memory_usage = psutil.virtual_memory()
-        memory_progress, memory_usage_percent = self.__get_process(memory_usage)
-        memory_progress.add_task("memory_progress", total=100, completed=round(memory_usage_percent))
-
-        swap_usage = psutil.swap_memory()
-        swap_progress, swap_usage_percent = self.__get_process(swap_usage)
-        swap_progress.add_task("swap_progress", total=100, completed=round(swap_usage_percent))
-
-        infos = {"Memory usage": memory_progress, "Swap usage": swap_progress}
-        return infos
-
-    @staticmethod
-    def __get_process(usage):
-        total_space = f"{round(usage[0] / GB, 2)}GB"
-        usage_percent = usage[2]
-        color = (
-            GREEN if usage_percent < 25
-            else YELLOW if usage_percent < 50
-            else ORANGE if usage_percent < 75
-            else RED
-        )
-        progress = Progress(
-            BarColumn(complete_style=color, bar_width=10, finished_style=RED),
-            TaskProgressColumn(),
-            TextColumn(f" of {total_space}")
-        )
-        return progress, usage_percent
+from typing import Dict
+
+import psutil
+from rich.console import RenderableType
+from rich.progress import Progress, BarColumn, TaskProgressColumn, TextColumn
+
+from .constants import GB, GREEN, YELLOW, ORANGE, RED
+from .sysinfo import SysInfo
+
+
+class Memory(SysInfo):
+    def _get_infos(self) -> Dict[RenderableType, RenderableType]:
+        memory_usage = psutil.virtual_memory()
+        memory_progress, memory_usage_percent = self.__get_process(memory_usage)
+        memory_progress.add_task("memory_progress", total=100, completed=round(memory_usage_percent))
+
+        swap_usage = psutil.swap_memory()
+        swap_progress, swap_usage_percent = self.__get_process(swap_usage)
+        swap_progress.add_task("swap_progress", total=100, completed=round(swap_usage_percent))
+
+        infos = {"Memory usage": memory_progress, "Swap usage": swap_progress}
+        return infos
+
+    @staticmethod
+    def __get_process(usage):
+        total_space = f"{round(usage[0] / GB, 2)}GB"
+        usage_percent = usage[2]
+        color = (
+            GREEN if usage_percent < 25
+            else YELLOW if usage_percent < 50
+            else ORANGE if usage_percent < 75
+            else RED
+        )
+        progress = Progress(
+            BarColumn(complete_style=color, bar_width=10, finished_style=RED),
+            TaskProgressColumn(),
+            TextColumn(f" of {total_space}")
+        )
+        return progress, usage_percent
```

### Comparing `elegantmotd-0.2.4/PKG-INFO` & `elegantmotd-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elegantmotd
-Version: 0.2.4
+Version: 0.2.5
 Summary: A visually appealing and informative Message of the Day (MOTD) generator for Linux systems.
 Home-page: https://github.com/emerick-biron/elegantmotd
 License: MIT
 Keywords: motd,system,information,console,dashboard
 Author: Emerick Biron
 Author-email: emerick.biron@gmail.com
 Requires-Python: >=3.10,<4.0
```

