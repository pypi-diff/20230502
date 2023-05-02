# Comparing `tmp/skelly_synchronize-2023.5.1008.tar.gz` & `tmp/skelly_synchronize-2023.5.1009.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skelly_synchronize-2023.5.1008.tar", last modified: Mon May  1 17:12:27 2023, max compression
+gzip compressed data, was "skelly_synchronize-2023.5.1009.tar", last modified: Tue May  2 20:29:30 2023, max compression
```

## Comparing `skelly_synchronize-2023.5.1008.tar` & `skelly_synchronize-2023.5.1009.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0       65 2023-05-01 17:12:14.655931 skelly_synchronize-2023.5.1008/.gitattributes
--rw-r--r--   0        0        0      146 2023-05-01 17:12:14.655931 skelly_synchronize-2023.5.1008/.github/workflows/lint-with-black.yml
--rw-r--r--   0        0        0     1087 2023-05-01 17:12:14.655931 skelly_synchronize-2023.5.1008/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml
--rw-r--r--   0        0        0      924 2023-05-01 17:12:14.655931 skelly_synchronize-2023.5.1008/.github/workflows/python-testing.yml
--rw-r--r--   0        0        0     2783 2023-05-01 17:12:14.655931 skelly_synchronize-2023.5.1008/.gitignore
--rw-r--r--   0        0        0    34523 2023-05-01 17:12:14.655931 skelly_synchronize-2023.5.1008/LICENSE
--rw-r--r--   0        0        0     2571 2023-05-01 17:12:14.655931 skelly_synchronize-2023.5.1008/README.md
--rw-r--r--   0        0        0     1600 2023-05-01 17:12:14.655931 skelly_synchronize-2023.5.1008/pyproject.toml
--rw-r--r--   0        0        0      111 2023-05-01 17:12:14.655931 skelly_synchronize-2023.5.1008/requirements.txt
--rw-r--r--   0        0        0       50 2023-05-01 17:12:14.655931 skelly_synchronize-2023.5.1008/setup.py
--rw-r--r--   0        0        0      976 2023-05-01 17:12:14.655931 skelly_synchronize-2023.5.1008/skelly_synchronize/__init__.py
--rw-r--r--   0        0        0      333 2023-05-01 17:12:14.655931 skelly_synchronize-2023.5.1008/skelly_synchronize/__main__.py
--rw-r--r--   0        0        0     1799 2023-05-01 17:12:14.655931 skelly_synchronize-2023.5.1008/skelly_synchronize/gui/skelly_synchronize_gui.py
--rw-r--r--   0        0        0      420 2023-05-01 17:12:14.655931 skelly_synchronize-2023.5.1008/skelly_synchronize/gui/widgets/run_button_widget.py
--rw-r--r--   0        0        0    18610 2023-05-01 17:12:14.659931 skelly_synchronize-2023.5.1008/skelly_synchronize/skelly_synchronize.py
--rw-r--r--   0        0        0        0 2023-05-01 17:12:14.659931 skelly_synchronize-2023.5.1008/skelly_synchronize/system/__init__.py
--rw-r--r--   0        0        0     1479 2023-05-01 17:12:14.659931 skelly_synchronize-2023.5.1008/skelly_synchronize/system/default_paths.py
--rw-r--r--   0        0        0     1402 2023-05-01 17:12:14.659931 skelly_synchronize-2023.5.1008/skelly_synchronize/system/logging_configuration.py
--rw-r--r--   0        0        0     1449 2023-05-01 17:12:14.659931 skelly_synchronize-2023.5.1008/skelly_synchronize/tests/test_trim_single_video_deffcode.py
--rw-r--r--   0        0        0     1018 2023-05-01 17:12:14.659931 skelly_synchronize-2023.5.1008/skelly_synchronize/tests/unit_tests.py
--rw-r--r--   0        0        0      577 2023-05-01 17:12:14.659931 skelly_synchronize-2023.5.1008/skelly_synchronize/tests/utilities/check_list_values_are_equal.py
--rw-r--r--   0        0        0      262 2023-05-01 17:12:14.659931 skelly_synchronize-2023.5.1008/skelly_synchronize/tests/utilities/find_frame_count_of_video.py
--rw-r--r--   0        0        0     1263 2023-05-01 17:12:14.659931 skelly_synchronize-2023.5.1008/skelly_synchronize/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py
--rw-r--r--   0        0        0     2048 2023-05-01 17:12:14.659931 skelly_synchronize-2023.5.1008/skelly_synchronize/utils/check_if_video_has_reversed_metadata.py
--rw-r--r--   0        0        0     1340 2023-05-01 17:12:14.659931 skelly_synchronize-2023.5.1008/skelly_synchronize/utils/get_video_files.py
--rw-r--r--   0        0        0     1871 2023-05-01 17:12:14.659931 skelly_synchronize-2023.5.1008/skelly_synchronize/utils/path_handling_utilities.py
--rw-r--r--   0        0        0     3438 1970-01-01 00:00:00.000000 skelly_synchronize-2023.5.1008/PKG-INFO
+-rw-r--r--   0        0        0       65 2023-05-02 20:29:14.965668 skelly_synchronize-2023.5.1009/.gitattributes
+-rw-r--r--   0        0        0      146 2023-05-02 20:29:14.965668 skelly_synchronize-2023.5.1009/.github/workflows/lint-with-black.yml
+-rw-r--r--   0        0        0     1087 2023-05-02 20:29:14.965668 skelly_synchronize-2023.5.1009/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml
+-rw-r--r--   0        0        0      924 2023-05-02 20:29:14.965668 skelly_synchronize-2023.5.1009/.github/workflows/python-testing.yml
+-rw-r--r--   0        0        0     2783 2023-05-02 20:29:14.965668 skelly_synchronize-2023.5.1009/.gitignore
+-rw-r--r--   0        0        0    34523 2023-05-02 20:29:14.965668 skelly_synchronize-2023.5.1009/LICENSE
+-rw-r--r--   0        0        0     2571 2023-05-02 20:29:14.965668 skelly_synchronize-2023.5.1009/README.md
+-rw-r--r--   0        0        0     1600 2023-05-02 20:29:14.965668 skelly_synchronize-2023.5.1009/pyproject.toml
+-rw-r--r--   0        0        0      111 2023-05-02 20:29:14.965668 skelly_synchronize-2023.5.1009/requirements.txt
+-rw-r--r--   0        0        0       50 2023-05-02 20:29:14.965668 skelly_synchronize-2023.5.1009/setup.py
+-rw-r--r--   0        0        0      976 2023-05-02 20:29:14.965668 skelly_synchronize-2023.5.1009/skelly_synchronize/__init__.py
+-rw-r--r--   0        0        0      333 2023-05-02 20:29:14.965668 skelly_synchronize-2023.5.1009/skelly_synchronize/__main__.py
+-rw-r--r--   0        0        0     1799 2023-05-02 20:29:14.965668 skelly_synchronize-2023.5.1009/skelly_synchronize/gui/skelly_synchronize_gui.py
+-rw-r--r--   0        0        0      420 2023-05-02 20:29:14.965668 skelly_synchronize-2023.5.1009/skelly_synchronize/gui/widgets/run_button_widget.py
+-rw-r--r--   0        0        0    18727 2023-05-02 20:29:14.965668 skelly_synchronize-2023.5.1009/skelly_synchronize/skelly_synchronize.py
+-rw-r--r--   0        0        0        0 2023-05-02 20:29:14.965668 skelly_synchronize-2023.5.1009/skelly_synchronize/system/__init__.py
+-rw-r--r--   0        0        0     1479 2023-05-02 20:29:14.965668 skelly_synchronize-2023.5.1009/skelly_synchronize/system/default_paths.py
+-rw-r--r--   0        0        0     1402 2023-05-02 20:29:14.965668 skelly_synchronize-2023.5.1009/skelly_synchronize/system/logging_configuration.py
+-rw-r--r--   0        0        0     1449 2023-05-02 20:29:14.965668 skelly_synchronize-2023.5.1009/skelly_synchronize/tests/test_trim_single_video_deffcode.py
+-rw-r--r--   0        0        0     1018 2023-05-02 20:29:14.965668 skelly_synchronize-2023.5.1009/skelly_synchronize/tests/unit_tests.py
+-rw-r--r--   0        0        0      577 2023-05-02 20:29:14.965668 skelly_synchronize-2023.5.1009/skelly_synchronize/tests/utilities/check_list_values_are_equal.py
+-rw-r--r--   0        0        0      262 2023-05-02 20:29:14.965668 skelly_synchronize-2023.5.1009/skelly_synchronize/tests/utilities/find_frame_count_of_video.py
+-rw-r--r--   0        0        0     1263 2023-05-02 20:29:14.969669 skelly_synchronize-2023.5.1009/skelly_synchronize/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py
+-rw-r--r--   0        0        0     2048 2023-05-02 20:29:14.969669 skelly_synchronize-2023.5.1009/skelly_synchronize/utils/check_if_video_has_reversed_metadata.py
+-rw-r--r--   0        0        0     1340 2023-05-02 20:29:14.969669 skelly_synchronize-2023.5.1009/skelly_synchronize/utils/get_video_files.py
+-rw-r--r--   0        0        0     1871 2023-05-02 20:29:14.969669 skelly_synchronize-2023.5.1009/skelly_synchronize/utils/path_handling_utilities.py
+-rw-r--r--   0        0        0     3438 1970-01-01 00:00:00.000000 skelly_synchronize-2023.5.1009/PKG-INFO
```

### Comparing `skelly_synchronize-2023.5.1008/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml` & `skelly_synchronize-2023.5.1009/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1008/.github/workflows/python-testing.yml` & `skelly_synchronize-2023.5.1009/.github/workflows/python-testing.yml`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1008/.gitignore` & `skelly_synchronize-2023.5.1009/.gitignore`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1008/LICENSE` & `skelly_synchronize-2023.5.1009/LICENSE`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1008/README.md` & `skelly_synchronize-2023.5.1009/README.md`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1008/pyproject.toml` & `skelly_synchronize-2023.5.1009/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [tool.bumpver] #bump the version by entering `bumpver update` in the terminal
-current_version = "v2023.05.1008"
+current_version = "v2023.05.1009"
 version_pattern = "vYYYY.0M.BUILD[-TAG]"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `skelly_synchronize-2023.5.1008/skelly_synchronize/__init__.py` & `skelly_synchronize-2023.5.1009/skelly_synchronize/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Top-level package for basic_template_repo."""
 
 __package_name__ = "skelly_synchronize"
-__version__ = "v2023.05.1008"
+__version__ = "v2023.05.1009"
 
 __author__ = """Philip Queen"""
 __email__ = "info@freemocap.org"
 __repo_owner_github_user_name__ = "freemocap"
 __repo_url__ = (
     f"https://github.com/{__repo_owner_github_user_name__}/{__package_name__}/"
 )
```

### Comparing `skelly_synchronize-2023.5.1008/skelly_synchronize/gui/skelly_synchronize_gui.py` & `skelly_synchronize-2023.5.1009/skelly_synchronize/gui/skelly_synchronize_gui.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1008/skelly_synchronize/skelly_synchronize.py` & `skelly_synchronize-2023.5.1009/skelly_synchronize/skelly_synchronize.py`

 * *Files 1% similar despite different names*

```diff
@@ -462,20 +462,23 @@
     )
 
     synchronize = VideoSynchronize()
     synchronize.synchronize(
         session_folder_path=session_folder_path,
         video_file_list=video_file_list,
     )
+    synchronized_video_folder_path = synchronize.synchronized_folder_path
 
     # end performance timer
     end_timer = time.time()
 
     # calculate and display elapsed processing time
     elapsed_time = end_timer - start_timer
     logging.info(f"Elapsed processing time in seconds: {elapsed_time}")
 
+    return synchronized_video_folder_path
+
 
 if __name__ == "__main__":
     raw_video_folder_path = Path("path/to/your/folder/of/raw/videos")
     file_type = "MP4"
     synchronize_videos(raw_video_folder_path=raw_video_folder_path, file_type=file_type)
```

### Comparing `skelly_synchronize-2023.5.1008/skelly_synchronize/system/default_paths.py` & `skelly_synchronize-2023.5.1009/skelly_synchronize/system/default_paths.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1008/skelly_synchronize/system/logging_configuration.py` & `skelly_synchronize-2023.5.1009/skelly_synchronize/system/logging_configuration.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1008/skelly_synchronize/tests/test_trim_single_video_deffcode.py` & `skelly_synchronize-2023.5.1009/skelly_synchronize/tests/test_trim_single_video_deffcode.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1008/skelly_synchronize/tests/unit_tests.py` & `skelly_synchronize-2023.5.1009/skelly_synchronize/tests/unit_tests.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1008/skelly_synchronize/tests/utilities/check_list_values_are_equal.py` & `skelly_synchronize-2023.5.1009/skelly_synchronize/tests/utilities/check_list_values_are_equal.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1008/skelly_synchronize/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py` & `skelly_synchronize-2023.5.1009/skelly_synchronize/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1008/skelly_synchronize/utils/check_if_video_has_reversed_metadata.py` & `skelly_synchronize-2023.5.1009/skelly_synchronize/utils/check_if_video_has_reversed_metadata.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1008/skelly_synchronize/utils/get_video_files.py` & `skelly_synchronize-2023.5.1009/skelly_synchronize/utils/get_video_files.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1008/skelly_synchronize/utils/path_handling_utilities.py` & `skelly_synchronize-2023.5.1009/skelly_synchronize/utils/path_handling_utilities.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1008/PKG-INFO` & `skelly_synchronize-2023.5.1009/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skelly_synchronize
-Version: 2023.5.1008
+Version: 2023.5.1009
 Summary: Basic template of a python repository
 Keywords: basic,template,python,repository
 Author-email: skelly_synchronize <info@freemocap.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python
```

