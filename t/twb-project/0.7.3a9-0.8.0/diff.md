# Comparing `tmp/twb_project-0.7.3a9.tar.gz` & `tmp/twb_project-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twb_project-0.7.3a9.tar", max compression
+gzip compressed data, was "twb_project-0.8.0.tar", max compression
```

## Comparing `twb_project-0.7.3a9.tar` & `twb_project-0.8.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rw-r--r--   0        0        0    18092 2023-02-26 13:10:42.136159 twb_project-0.7.3a9/LICENSE
--rw-r--r--   0        0        0     1547 2023-02-27 01:45:34.838817 twb_project-0.7.3a9/README.md
--rw-r--r--   0        0        0      762 2023-04-19 17:36:55.924904 twb_project-0.7.3a9/pyproject.toml
--rw-r--r--   0        0        0      201 2023-03-26 05:00:17.199386 twb_project-0.7.3a9/twb/__init__.py
--rw-r--r--   0        0        0      788 2023-02-26 15:18:15.849792 twb_project-0.7.3a9/twb/bip.py
--rw-r--r--   0        0        0    17389 2023-04-19 17:36:30.165883 twb_project-0.7.3a9/twb/builder.py
--rw-r--r--   0        0        0     4614 2023-03-26 18:02:08.247223 twb_project-0.7.3a9/twb/decompressor.py
--rw-r--r--   0        0        0     9493 2023-03-26 18:01:42.380403 twb_project-0.7.3a9/twb/downloader.py
--rw-r--r--   0        0        0     3607 2023-03-26 19:24:30.197127 twb_project-0.7.3a9/twb/logger.py
--rw-r--r--   0        0        0      546 2023-03-26 05:47:24.185465 twb_project-0.7.3a9/twb/modifier.py
--rw-r--r--   0        0        0     9101 2023-04-19 03:52:12.830673 twb_project-0.7.3a9/twb/parallelization.py
--rw-r--r--   0        0        0    11680 2023-04-19 06:20:11.392642 twb_project-0.7.3a9/twb/reader.py
--rw-r--r--   0        0        0     6161 2023-04-19 04:03:30.303243 twb_project-0.7.3a9/twb/utils.py
--rw-r--r--   0        0        0     2437 1970-01-01 00:00:00.000000 twb_project-0.7.3a9/setup.py
--rw-r--r--   0        0        0     2592 1970-01-01 00:00:00.000000 twb_project-0.7.3a9/PKG-INFO
+-rw-r--r--   0        0        0    18092 2023-02-26 13:10:42.136159 twb_project-0.8.0/LICENSE
+-rw-r--r--   0        0        0     1547 2023-02-27 01:45:34.838817 twb_project-0.8.0/README.md
+-rw-r--r--   0        0        0      760 2023-05-02 05:53:55.856803 twb_project-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      218 2023-05-02 04:53:16.027176 twb_project-0.8.0/twb/__init__.py
+-rw-r--r--   0        0        0      788 2023-02-26 15:18:15.849792 twb_project-0.8.0/twb/bip.py
+-rw-r--r--   0        0        0    17118 2023-04-20 02:58:09.579621 twb_project-0.8.0/twb/builder.py
+-rw-r--r--   0        0        0     4614 2023-03-26 18:02:08.247223 twb_project-0.8.0/twb/decompressor.py
+-rw-r--r--   0        0        0     9493 2023-03-26 18:01:42.380403 twb_project-0.8.0/twb/downloader.py
+-rw-r--r--   0        0        0     3794 2023-04-20 07:59:01.227219 twb_project-0.8.0/twb/logger.py
+-rw-r--r--   0        0        0     1605 2023-05-02 05:31:50.969415 twb_project-0.8.0/twb/logger_init.py
+-rw-r--r--   0        0        0    10620 2023-05-02 05:58:56.480996 twb_project-0.8.0/twb/modifier.py
+-rw-r--r--   0        0        0     9161 2023-04-20 02:54:12.926181 twb_project-0.8.0/twb/parallelization.py
+-rw-r--r--   0        0        0     5527 2023-05-02 04:49:02.953589 twb_project-0.8.0/twb/reader.py
+-rw-r--r--   0        0        0     6203 2023-04-20 00:32:02.529127 twb_project-0.8.0/twb/utils.py
+-rw-r--r--   0        0        0     3417 2023-05-02 05:44:59.869020 twb_project-0.8.0/twb/warehouse.py
+-rw-r--r--   0        0        0     2435 1970-01-01 00:00:00.000000 twb_project-0.8.0/setup.py
+-rw-r--r--   0        0        0     2590 1970-01-01 00:00:00.000000 twb_project-0.8.0/PKG-INFO
```

### Comparing `twb_project-0.7.3a9/LICENSE` & `twb_project-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `twb_project-0.7.3a9/README.md` & `twb_project-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `twb_project-0.7.3a9/pyproject.toml` & `twb_project-0.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "twb-project"
-version = "0.7.3a9"
+version = "0.8.0"
 description = "An unified tool for the research in extracting information from Wikipedia Edit History chunk."
 authors = ["Lingxi Li <hi@lingxi.li>"]
 license = "GNU GPL"
 readme = "README.md"
 packages = [
     { include = "twb" },
 ]
```

### Comparing `twb_project-0.7.3a9/twb/bip.py` & `twb_project-0.8.0/twb/bip.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.7.3a9/twb/builder.py` & `twb_project-0.8.0/twb/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from .logger import universal_logger_init, twb_logger, cleanup_logger
 from .utils import get_file_list, compress_zstd, get_memory_consumption, cleanup_dir, get_curr_version, \
     prepare_output_dir, COMPRESSION_EXTENSION
 from .bip import BlockInteriorProcessor, DefaultBIP
 from .parallelization import RDSProcessManager, RDSProcessController
 
-_DEFAULT_REVISIONS_PER_BLOCK = 300000
+_DEFAULT_REVISIONS_PER_BLOCK = 1000000
 _DEFAULT_START_INDEX = 0
 _DEFAULT_NUM_PROC = 1
 _DEFAULT_LOG_LEVEL = logging.DEBUG
 
 
 class Builder:
     """
@@ -233,15 +233,17 @@
     # Second try block, catching issues during processing (XML parsing, etc).
     try:
         def get_new_output_path():
             """
             Get the path of the next output file.
             """
             nonlocal controller, compression_target_dir
+            controller.logdebug('Ready to declare index (cp).')
             curr_index = str(controller.declare_index()).zfill(8)  # 8 digits in total for scalability.
+            controller.logdebug('Done declaring index (cp).')
             return os.path.join(compression_target_dir, f'block_{curr_index}.jsonl')
 
         compression_target_dir = compression_temp_dir if should_compress else output_dir
 
         total_article_count = 0
         total_block_count = 1
         total_revision_count = 0
@@ -251,18 +253,20 @@
         all_memory_usage_records = []
         curr_output_path = get_new_output_path()
 
         def _super_callback(article: dict):
             """
             The super callback for the XML parser. It will be called recursively for each article.
             """
+            controller.logdebug('_super_callback() calling.')
+
             nonlocal total_article_count, total_block_count, total_revision_count
             nonlocal revision_count, memory_usage_records, all_memory_usage_records, curr_output_path
 
-            controller.logdebug('_super_callback() called.')
+            controller.logdebug('_super_callback() started.')
 
             # If previous batch is full, store the max memory usage and reset the counters.
             if revision_count >= revisions_per_block:
                 # Store the max memory usage in previous batch.
                 all_memory_usage_records.append(max(memory_usage_records))
                 # Update the block count.
                 total_block_count += 1
@@ -295,15 +299,15 @@
             controller.logdebug(f'Memory: {memory_usage_records[-1]} MB')
 
         controller.logdebug(f'Big parsing loop started. (revisions_per_block={revisions_per_block})')
 
         # We store articles into JSONL files in a streaming manner, along the way of parsing XML files.
         # Therefore, we don't have to keep all the results in the memory, which is a huge problem.
         for path in decompressed_files:
-            _parse_xml(path=path, processor=block_interior_processor, super_callback=_super_callback)
+            _parse_xml(xml_path=path, processor=block_interior_processor, super_callback=_super_callback)
 
         controller.logdebug('Big parsing loop done.')
 
         if len(memory_usage_records) > 0:
             all_memory_usage_records.append(max(memory_usage_records))
 
         controller.logdebug(f'Parsing done. {total_article_count} articles processed.',
@@ -337,63 +341,51 @@
         very_end_time = time.time()
         total_execution_duration = very_end_time - very_start_time
         controller.loginfo(f'File done: {archive_filename}. (Duration: {total_execution_duration:.2f}s)')
 
         controller.unregister()
 
 
-def _xml_parser_callback(path, item, processor: BlockInteriorProcessor, super_callback: Callable[[dict], None]):
+def _parse_xml(xml_path: str, processor: BlockInteriorProcessor, super_callback: Callable[[dict], None]):
     """
-    The callback function for the XML parser.
-    :param path: the path of the current item
-    :param item: children dictionary
+    Parse the XML file into a list of JSON objects.
+    :param xml_path: the path of the XML file
     :param processor: the interior processor for blocks
-    :return: True if the parsing should continue, False otherwise
+    :return: the list of parsed results
     """
-    tag_name = path[-1][0]
-    item_type = type(item)
-
-    # If the item is a page, we don't need to process it.
-    if tag_name != 'page':
-        return True
-
-    # If the item is not a dictionary, it means that the item is a leaf node, and we don't expect it to be a block.
-    if item_type is not dict:
-        return True
+    def _inner_callback(path, item):
+        nonlocal super_callback
 
-    logging.debug(f'Start callback: <{tag_name}>.')
+        tag_name = path[-1][0]
+        item_type = type(item)
 
-    # processed_item = processor.parse(tag=tag_name, meta={}, tree=item)
+        # If the item is a page, we don't need to process it.
+        if tag_name != 'page':
+            return True
 
-    # If the item is not None, it means that the item is a block and we should append it to the results.
-    # if processed_item is not None:
-    #     pass
+        # If the item is not a dictionary, it means that the item is a leaf node, and we don't expect it to be a block.
+        if item_type is not dict:
+            return True
 
-    super_callback(item)
+        logging.debug(f'Memory: {get_memory_consumption()} MB')
 
-    logging.debug(f'Callback done: <{tag_name}>.')
-
-    return True
+        logging.debug(f'Start callback: <{tag_name}>.')
+        super_callback(item)
+        logging.debug(f'Callback done: <{tag_name}>.')
 
+        return True
 
-def _parse_xml(path: str, processor: BlockInteriorProcessor, super_callback: Callable[[dict], None]):
-    """
-    Parse the XML file into a list of JSON objects.
-    :param path: the path of the XML file
-    :param processor: the interior processor for blocks
-    :return: the list of parsed results
-    """
-    with open(path, 'rb') as xml_file:
+    with open(xml_path, 'rb') as xml_file:
         xmltodict.parse(
             xml_file,
             item_depth=processor.read_depth,
-            item_callback=lambda x, y: _xml_parser_callback(x, y, processor, super_callback)
+            item_callback=_inner_callback,
         )
 
-        logging.debug(f'Parsing done: {path}')
+        logging.debug(f'Parsing done: {xml_path}')
 
 
 def _store_article_to_jsonl(article: dict, output_path: str):
     """
     Store the blocks to a JSONL file.
     :param article: the article to store
     :param output_path: the path to store the JSONL file
```

### Comparing `twb_project-0.7.3a9/twb/decompressor.py` & `twb_project-0.8.0/twb/decompressor.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.7.3a9/twb/downloader.py` & `twb_project-0.8.0/twb/downloader.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.7.3a9/twb/logger.py` & `twb_project-0.8.0/twb/logger.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,26 +5,28 @@
 from typing import Union
 
 
 _log_format = "[%(asctime)s (%(process)d) %(levelname)s] %(message)s"
 _formatter = logging.Formatter(_log_format)
 
 
-def _get_logger_stream_handler() -> logging.StreamHandler:
+def _get_logger_stream_handler(log_level: int) -> logging.StreamHandler:
     stream_handler = logging.StreamHandler()
     stream_handler.setFormatter(_formatter)
+    stream_handler.setLevel(log_level)
     return stream_handler
 
 
-def _get_logger_file_handler(log_name: str, log_dir: str) -> Union[logging.FileHandler, None]:
+def _get_logger_file_handler(log_name: str, log_dir: str, log_level: int) -> Union[logging.FileHandler, None]:
     if log_dir is not None:
         os.makedirs(log_dir, exist_ok=True)
         log_path = os.path.join(log_dir, f'{log_name}.log')
         file_handler = logging.FileHandler(filename=log_path, mode='a')
         file_handler.setFormatter(_formatter)
+        file_handler.setLevel(log_level)
         return file_handler
     return None
 
 
 def cleanup_logger(log_name: str, log_dir: str):
     if log_dir is not None and os.path.exists(log_dir):
         log_file_path = os.path.join(log_dir, f'{log_name}.log')
@@ -37,34 +39,34 @@
 
 
 def _cleanup_logger_handlers(logger: logging.Logger):
     while logger.hasHandlers():
         logger.removeHandler(logger.handlers[0])
 
 
-def universal_logger_init(log_name: str, log_dir: str, log_level: int = logging.DEBUG):
-    stream_handler = _get_logger_stream_handler()
-    file_handler = _get_logger_file_handler(log_name=log_name, log_dir=log_dir)
+def universal_logger_init(log_name: str, log_dir: str, log_level: int = logging.INFO):
+    stream_handler = _get_logger_stream_handler(log_level=log_level)
+    file_handler = _get_logger_file_handler(log_name=log_name, log_dir=log_dir, log_level=log_level)
 
     logger = logging.getLogger()
 
     # Clean up any existing handlers in default logger.
     _cleanup_logger_handlers(logger)
 
     logger.setLevel(log_level)
     logger.addHandler(stream_handler)
     if file_handler is not None:
         logger.addHandler(file_handler)
 
 
-def mp_logger_init(log_name: str, log_dir: str, log_level: int = logging.DEBUG) -> (QueueListener, mp.Queue):
+def mp_logger_init(log_name: str, log_dir: str, log_level: int = logging.INFO) -> (QueueListener, mp.Queue):
     q = mp.Queue()
 
-    stream_handler = _get_logger_stream_handler()
-    file_handler = _get_logger_file_handler(log_name=log_name, log_dir=log_dir)
+    stream_handler = _get_logger_stream_handler(log_level=log_level)
+    file_handler = _get_logger_file_handler(log_name=log_name, log_dir=log_dir, log_level=log_level)
 
     if file_handler is not None:
         ql = QueueListener(q, stream_handler, file_handler)
     else:
         ql = QueueListener(q, stream_handler)
     ql.start()
 
@@ -74,15 +76,15 @@
     logger.addHandler(stream_handler)
     if file_handler is not None:
         logger.addHandler(file_handler)
 
     return ql, q
 
 
-def mp_child_logger_init(q: mp.Queue, log_level: int = logging.DEBUG):
+def mp_child_logger_init(q: mp.Queue, log_level: int = logging.INFO):
     qh = QueueHandler(q)
     logger = logging.getLogger()
 
     # Clean up any existing handlers in subprocess default logger.
     _cleanup_logger_handlers(logger)
 
     logger.setLevel(log_level)
```

### Comparing `twb_project-0.7.3a9/twb/parallelization.py` & `twb_project-0.8.0/twb/parallelization.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,25 +9,26 @@
 
 # ========== Global Variables for cross-process communication ==========
 
 
 global _parallel_lock, _logger_lock, _curr_index, _curr_count, _pid_map, _active_pids
 
 
-def _init_worker(q, inner_parallel_lock, inner_logger_lock, inner_curr_index, inner_curr_count, pid_map, active_pids):
+def _init_worker(q, inner_parallel_lock, inner_logger_lock, inner_curr_index, inner_curr_count, pid_map, active_pids,
+                 log_level):
     global _parallel_lock, _logger_lock, _curr_index, _curr_count, _pid_map, _active_pids
     _parallel_lock = inner_parallel_lock
     _logger_lock = inner_logger_lock
     _curr_index = inner_curr_index
     _curr_count = inner_curr_count
     _pid_map = pid_map
     _active_pids = active_pids
 
     # Initialize the logger within the sub-process.
-    mp_child_logger_init(q)
+    mp_child_logger_init(q, log_level=log_level)
 
     # Log the initialization of the process.
     twb_logger.debug('Process initialized.')
 
 
 # ========== RDS Process Controller ==========
 
@@ -202,15 +203,15 @@
         logger_lock = Lock()
 
         self.manager = manager
 
         self.pool = Pool(
             processes=final_num_proc,
             initializer=_init_worker,
-            initargs=(q, parallel_lock, logger_lock, curr_index, curr_count, pid_map, active_pids)
+            initargs=(q, parallel_lock, logger_lock, curr_index, curr_count, pid_map, active_pids, log_level)
         )
 
     def apply_async(self,
                     executable: RDSProcessExecutable[_R],
                     args: Tuple[Any, ...],  # Typing of this variable might not be correct.
                     use_controller: bool = True,
                     callback: Union[Callable[[_R], None], None] = None,
```

### Comparing `twb_project-0.7.3a9/twb/reader.py` & `twb_project-0.8.0/twb/modifier.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,66 +1,65 @@
 import json
 import logging
 import os
-import uuid
+from functools import partial
+from multiprocessing import Pool
 from typing import Union, List, Tuple
+from abc import ABC, abstractmethod
 import time
 
-from .modifier import Modifier
-from .logger import cleanup_logger, universal_logger_init, twb_logger
-from .parallelization import RDSProcessManager, RDSProcessController
-from .utils import get_file_list, decompress_zstd, prepare_output_dir, get_curr_version, get_line_positions, \
-    cleanup_dir, read_line_in_file, compress_zstd, COMPRESSION_EXTENSION, parse_schema
+from .logger_init import _init_logger_main_process, _init_logger_sub_process, _init_logger_multiprocessing
+from .utils import get_file_list, decompress_zstd, prepare_output_dir, get_curr_version, \
+    cleanup_dir, compress_zstd, COMPRESSION_EXTENSION
+from .warehouse import Warehouse, get_warehouse_filenames
 
 _DEFAULT_NUM_PROC = 1
-_DEFAULT_LOG_LEVEL = logging.DEBUG
+_DEFAULT_LOG_LEVEL = logging.INFO
 
 
-class Reader:
+class ModifierProfile(ABC):
     """
-    The core class to read the generated temporal wikipedia blocks.
-
-    Basic usage:
-
-        import twb
-        reader = twb.Reader()  # Create an instance.
-        reader.preload('./test/sample_data/minimal_sample.xml')  # Preload the files to be processed.
+    The core class to define how to modify the JSON content.
+    """
+    @abstractmethod
+    def block(self, content: dict) -> Union[dict, None]:
+        """
+        Returns a list of batches of URLs to download.
+        :param content: The JSON content to be modified.
+        :return: Modified JSON content. Return None if the content should be removed.
+        """
+        pass
 
-    You must preload the files to be processed before building the blocks.
-    Preload function accepts a path to a file or a directory, and can be called multiple times (for multiple files).
 
+class Modifier:
+    """
     Attributes:
         num_proc (int): The number of processes to use.
-        log_dir (str): The dir to the log file.
         log_level (int): The log level.
         files (list): A list of files to be read.
         modifiers (list): A list of modifiers to be applied.
     """
 
     def __init__(self,
-                 log_dir: Union[str, None] = None,
+                 output_dir: str,
                  num_proc: int = _DEFAULT_NUM_PROC,
                  log_level: int = _DEFAULT_LOG_LEVEL):
         """
-        :param log_dir: the dir to the log file (default: None)
+        :param output_dir: the output directory
         :param num_proc: the number of processes to use (default: 1)
         :param log_level: the log level (default: logging.INFO)
         """
-        self.log_dir = log_dir
+        self.output_dir = output_dir
         self.num_proc = num_proc
         self.log_level = log_level
 
-        self.files = []
-        self.modifiers = []
-
-        # If log dir exists, remove it first.
-        cleanup_logger(log_name='reader', log_dir=log_dir)
+        self.files: List[str] = []
+        self.modifiers: List[ModifierProfile] = []
 
-        # Initialize the logger.
-        universal_logger_init(log_name='reader', log_dir=log_dir, log_level=log_level)
+        _init_logger_main_process(name='modifier', log_level=self.log_level)
 
     def preload(self, path: str):
         """
         Preload the files to be processed.
         It will not actually load to the memory until the build() method is called.
         :param path: the path of a file or a directory
         :raise ValueError: if the path is empty
@@ -68,257 +67,229 @@
         """
         if not path:
             raise ValueError('The path cannot be empty.')
         if not os.path.exists(path):
             raise FileNotFoundError('The path does not exist.')
         self.files.extend(get_file_list(path))
 
-    def glimpse(self) -> Union[Tuple[dict, dict], Tuple[None, None]]:
+    def add_profile(self, profile: ModifierProfile):
         """
-        Take a glimpse of the data.
-        It could still be large if one object contains a lot of information (e.g. many revisions, long article).
+        Map a function to each block.
+        :param profile: the modifier profile to be added
         """
-        if len(self.files) == 0:
-            twb_logger.warning('No file is loaded.')
-            return None
+        self.modifiers.append(profile)
 
-        # Randomly select a file.
-        picked_index = int(uuid.uuid4().int % len(self.files))
-        glimpse_path = self.files[picked_index]
-
-        twb_logger.info(f'Randomly chosen file: {glimpse_path}')
+    def _worker_initializer(self, q):
+        """
+        Initialize the worker process.
+        """
+        # Initialize the logger within the sub-process.
+        _init_logger_sub_process(q, log_level=self.log_level)
 
-        # Prepare the temporary directory for glimpse.
-        glimpse_temp_dir = os.path.join(os.getcwd(), '.glimpse')
-        os.makedirs(glimpse_temp_dir, exist_ok=True)
+    def _process_executor(self, file_path: str):
+        temp_dir = os.path.join(self.output_dir, 'temp')
+        os.makedirs(temp_dir, exist_ok=True)
 
-        twb_logger.info(f'Decompressing...')
+        original_name = os.path.split(file_path)[1]
+        decompressed_name = original_name.replace('.zst', '')
+        decompressed_path = os.path.join(temp_dir, decompressed_name)
 
         # Decompress the file.
-        decompressed_path = _decompress_executor(glimpse_path, glimpse_temp_dir)
-        first_block_text = read_line_in_file(decompressed_path, 0).rstrip('\n')
+        decompress_zstd(file_path, decompressed_path)
 
-        if first_block_text[0] != '{' or first_block_text[-1] != '}':
-            twb_logger.error(f'Invalid starting of block or end of block.')
-            return None, None
+        modified_name = decompressed_name + '.modified'
+        modified_path = os.path.join(temp_dir, modified_name)
 
-        # Read the first block into memory and then delete the decompressed file.
-        first_block = json.loads(first_block_text)
-        cleanup_dir(glimpse_temp_dir)
+        modified_file = open(modified_path, 'w')
 
-        twb_logger.info(f'Glimpse finished.')
+        # Read the file line by line, and apply the modifiers.
+        with open(decompressed_path, 'r') as f:
+            for line in iter(f.readline, ''):
+                block = json.loads(line)
+                for modifier in self.modifiers:
+                    block = modifier.block(block)
+                    if block is None:
+                        break
+                if block is not None:
+                    modified_file.write(json.dumps(block) + '\n')
 
-        return first_block, parse_schema(first_block)
+        modified_file.close()
 
-    def decompress(self, output_dir: str):
-        """
-        Decompress the selected files.
-        :param output_dir: the directory to store the decompressed files
-        """
-        # Log the version.
-        twb_logger.info(f'TWB Package Version: {get_curr_version()}')
+        # Remove the decompressed file.
+        os.remove(decompressed_path)
 
-        # Prepare the output directory.
-        prepare_output_dir(output_dir)
+        return modified_path
 
-        start_time = time.time()
+    def _warehouse_executor(self, file_path: str, assigned_warehouse: str):
+        try:
+            warehouse_filename, warehouse_metadata_filename = get_warehouse_filenames(assigned_warehouse)
+            warehouse_path = os.path.join(self.output_dir, warehouse_filename)
+            # warehouse_metadata_path = os.path.join(self.output_dir, warehouse_metadata_filename)  # TODO.
 
-        pm = RDSProcessManager(
-            log_name='decompress',
-            log_dir=self.log_dir,
-            log_level=self.log_level,
-            num_proc=self.num_proc
-        )
-        for file in self.files:
-            pm.apply_async(
-                executable=_decompress_executor,
-                args=(file, output_dir),
-                use_controller=False
-            )
+            warehouse_file = open(warehouse_path, 'a')
 
-        pm.close()
-        pm.join()
+            # Read the file line by line, and move directly to the warehouse (without last empty line).
+            with open(file_path, 'r') as f:
+                for line in iter(f.readline, ''):
+                    warehouse_file.write(line + '\n')
 
-        end_time = time.time()
-        execution_duration = end_time - start_time
-        twb_logger.info(f'Decompression finished. (Duration: {execution_duration:.2f}s)')
+            warehouse_file.close()
 
-    def add_modifier(self, modifier: Modifier):
-        """
-        Map a function to each block.
-        :param modifier: the modifier to be added
-        """
-        self.modifiers.append(modifier)
+            # Remove the modified file.
+            os.remove(file_path)
+
+        except Exception as e:
+            logging.critical(f'Error occurred when moving the file to the warehouse. {e}')
+
+        return assigned_warehouse
+
+    def _cleanup_executor(self, warehouse_path: str):
+        try:
+            original_file_path = os.path.join(self.output_dir, warehouse_path)
+            if not os.path.exists(original_file_path):
+                logging.critical(f'The file {warehouse_path} [{original_file_path}] does not exist.')
+                return None
+
+            compressed_path = original_file_path + COMPRESSION_EXTENSION
+            compress_zstd(original_file_path, compressed_path)
+            os.remove(original_file_path)
 
-    def build_modification(self, output_dir: str):
+            return compressed_path
+
+        except:
+            logging.critical(f'Error occurred when compressing the file {warehouse_path}.')
+            return None
+
+    def build(self):
         """
         Build the blocks after apply the modifiers.
-        :param output_dir: the directory to store the modified files
         """
         # Log the version.
-        twb_logger.info(f'TWB Package Version: {get_curr_version()}')
+        logging.info(f'Modifier Version: {get_curr_version()}')
+
+        warehouse = Warehouse(
+            output_dir=self.output_dir,
+            max_size=8,
+            compress=True,
+        )
 
         start_time = time.time()
 
         # Prepare the output directory.
-        prepare_output_dir(output_dir)
+        prepare_output_dir(self.output_dir)
 
         curr_count = 0
         total_count = len(self.files)
 
-        global_temp_dir = os.path.join(output_dir, 'temp')
+        global_temp_dir = os.path.join(self.output_dir, 'temp')
         os.makedirs(global_temp_dir, exist_ok=True)
 
-        def _success_callback(*args):
-            pass
-
-        def _error_callback(e):
-            twb_logger.error(f'Error occurred when processing block: {e}')
-
-        for file_path in self.files:
-            twb_logger.info(f'Start: {file_path}')
-
-            file_start_time = time.time()
+        # Initialize multiprocessing logger.
+        ql, q = _init_logger_multiprocessing(log_level=self.log_level)
 
-            # Create temporary directory for this file.
-            temp_id = uuid.uuid4().hex
-            temp_dir = os.path.join(output_dir, 'temp', temp_id)
-            os.makedirs(temp_dir, exist_ok=True)
+        # Tasks is a list of tuples (task_type, args).
+        # Task types: 'process', 'warehouse', 'cleanup'
+        tasks: List[Tuple[str, Tuple]] = []
+
+        available_process_count = self.num_proc
+
+        modification_pool = Pool(
+            processes=self.num_proc,
+            initializer=self._worker_initializer,
+            initargs=(q,)
+        )
 
-            decompression_temp_dir = os.path.join(temp_dir, 'decompression')
-            os.makedirs(decompression_temp_dir, exist_ok=True)
-            compression_temp_dir = os.path.join(temp_dir, 'compression')
-            os.makedirs(compression_temp_dir, exist_ok=True)
+        processed_count = 0
+        finished_count = 0
 
-            # Decompress the file first (this step will not be done in parallel because this is faster).
-            twb_logger.debug(f'Decompressing...')
-            decompressed_path = _decompress_executor(file_path, decompression_temp_dir)
+        def _process_callback(file_path):
+            nonlocal warehouse, available_process_count, processed_count
+            processed_count += 1
 
-            # Compute target path. The target path should be within compression temporary directory.
-            target_filename = os.path.basename(decompressed_path)
-            target_path = os.path.join(compression_temp_dir, target_filename)
+            assigned_warehouse = warehouse.assign_warehouse()
 
-            line_positions = get_line_positions(decompressed_path)
+            logging.info(f'({processed_count / total_count * 100:.2f}% = {processed_count} / {total_count}) | '
+                         f'Processed: {os.path.basename(file_path)} | Warehouse: {assigned_warehouse}')
 
-            twb_logger.info(f'Start modifying {len(line_positions)} blocks...')
+            next_task_type = 'warehouse'
+            next_args = (file_path, assigned_warehouse)
+            tasks.insert(0, (next_task_type, next_args))
 
-            # Get line positions for all files.
-            pm = RDSProcessManager(
-                log_name='reader',
-                log_dir=self.log_dir,
-                log_level=self.log_level,
-                num_proc=self.num_proc
-            )
+            available_process_count += 1
 
-            for line_position in line_positions:
-                pm.apply_async(
-                    executable=_modify_executor,
-                    args=(decompressed_path, line_position, target_path, self.modifiers),
-                    use_controller=True,
-                    callback=_success_callback,
-                    error_callback=_error_callback
-                )
+        def _warehouse_callback(warehouse_basename):
+            nonlocal warehouse, available_process_count, finished_count
 
-            pm.close()
-            pm.join()
+            logging.debug(f'Saved into warehouse: {warehouse_basename}')
 
-            twb_logger.info(f'Finished modifying {len(line_positions)} blocks. Compressing...')
+            cleanup_path = warehouse.release_warehouse(warehouse_basename)
+            if cleanup_path is not None:
+                next_task_type = 'cleanup'
+                next_args = (cleanup_path,)
+                tasks.insert(0, (next_task_type, next_args))
 
-            # Compress the file.
-            output_path = os.path.join(output_dir, os.path.basename(target_path) + COMPRESSION_EXTENSION)
-            compress_zstd(target_path, output_path)
+            finished_count += 1
+            available_process_count += 1
 
-            twb_logger.info(f'Finished compressing. Cleaning up...')
+        def _cleanup_callback(cleanup_path):
+            nonlocal available_process_count
+            logging.info(f'Warehouse packed: {cleanup_path}')
 
-            # Clean up the temporary directory at this step.
-            cleanup_dir(temp_dir)
+            available_process_count += 1
 
-            twb_logger.info(f'Finished cleaning up.')
+        def _success_callback(task_type, file_path):
+            if task_type == 'process':
+                _process_callback(file_path)
+            elif task_type == 'warehouse':
+                _warehouse_callback(file_path)
+            elif task_type == 'cleanup':
+                _cleanup_callback(file_path)
 
-            file_end_time = time.time()
-            file_execution_duration = file_end_time - file_start_time
+        def _error_callback(e):
+            logging.error(f'Error occurred when processing block: {e}')
 
-            twb_logger.info(f'Finished: {file_path} -- (took {file_execution_duration:.2f}s)')
+        # Built-up initial tasks.
+        for curr_file_path in self.files:
+            tasks.append(('process', (curr_file_path,)))
+
+        # Main semaphore loop.
+        while tasks or available_process_count < self.num_proc:
+            if tasks and available_process_count > 0:
+                available_process_count -= 1
+                task_type, args = tasks.pop(0)
+                if task_type == 'process':
+                    file_path, = args
+                    modification_pool.apply_async(
+                        func=self._process_executor,
+                        args=(file_path,),
+                        callback=partial(_success_callback, task_type),
+                        error_callback=_error_callback
+                    )
+                elif task_type == 'warehouse':
+                    file_path, assigned_warehouse = args
+                    modification_pool.apply_async(
+                        func=self._warehouse_executor,
+                        args=(file_path, assigned_warehouse),
+                        callback=partial(_success_callback, task_type),
+                        error_callback=_error_callback
+                    )
+                elif task_type == 'cleanup':
+                    cleanup_path, = args
+                    modification_pool.apply_async(
+                        func=self._cleanup_executor,
+                        args=(cleanup_path,),
+                        callback=partial(_success_callback, task_type),
+                        error_callback=_error_callback
+                    )
+            else:
+                time.sleep(0.1)
 
-            # Log the progress.
-            curr_count += 1
-            twb_logger.info(f'Progress: {curr_count} / {total_count} = ({curr_count / total_count * 100:.2f}%)')
+        logging.debug(f'Semaphore loop finished.')
 
         # Clean up the global temporary directory.
         cleanup_dir(global_temp_dir)
 
         end_time = time.time()
         execution_duration = end_time - start_time
 
         # Log the end of the task.
-        twb_logger.info(f'All done! Finished all files. (took {execution_duration:.2f}s in total)')
-
-
-def _decompress_executor(path: str, output_dir: str) -> str:
-    original_name = os.path.split(path)[1]
-    decompressed_name = original_name.replace('.zst', '')
-    decompressed_path = os.path.join(output_dir, decompressed_name)
-    decompress_zstd(path, decompressed_path)
-    return decompressed_path
-
-
-def _line_position_processor(path: str, output_dir: str):
-    """
-    The processor for the line position process.
-    """
-    temp_id = uuid.uuid4().hex
-
-    temp_dir = os.path.join(output_dir, 'temp', temp_id)
-    os.makedirs(temp_dir, exist_ok=True)
-
-    _decompress_executor(path, temp_dir)
-
-    return path, get_line_positions(path)
-
-
-def _modify_executor(controller: RDSProcessController,
-                     path: str,
-                     position: int,
-                     target_path: str,
-                     modifiers: List[Modifier]):
-    """
-    The executor for the modification process.
-    :param controller: the controller of the process
-    :param path: the path of the file to be processed
-    :param position: the position of the file to be processed
-    :param target_path: the directory to store the modified files
-    :param modifiers: the list of modifiers to be applied
-    """
-    start_time = time.time()
-
-    controller.logdebug(f'Processing block: {position}')
-    block_text = read_line_in_file(path, position).rstrip('\n')
-    if block_text[0] != '{' or block_text[-1] != '}':
-        controller.logerr(f'Invalid starting of block or end of block: {path} @ {position}')
-        return
-
-    # Parse the block from text to JSON.
-    block = json.loads(block_text)
-
-    # Apply the modifiers.
-    for modifier in modifiers:
-        if block is None:
-            break
-        block = modifier.modify(block)
-
-    # We write the output only if the block is not None. Otherwise, we remove this block.
-    if block is not None:
-        with controller.parallel_lock:
-            logging.debug(f'Storing JSONL to {target_path}...')
-            try:
-                with open(target_path, 'a', buffering=1) as f:
-                    f.write(json.dumps(block) + '\n')
-            except Exception as e:
-                controller.logerr(f'Error occurred when writing block to file: {e}')
-            logging.debug(f'Storing JSONL done: {target_path}.')
-    else:
-        controller.logdebug(f'Removed block because of "None": {position}')
-
-    end_time = time.time()
-    execution_duration = end_time - start_time
-
-    controller.logdebug(f'Finished block: {position} -- (took {execution_duration:.2f}s)')
+        logging.info(f'All done! Finished all files. (took {execution_duration:.2f}s in total)')
```

### Comparing `twb_project-0.7.3a9/twb/utils.py` & `twb_project-0.8.0/twb/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 from typing import List, Callable, Union
 import zstandard as zstd
 import py7zr
 import shutil
 import psutil
 from importlib.metadata import version, PackageNotFoundError
+import multiprocessing as mp
 
 from twb.logger import twb_logger
 
 
 def get_curr_version():
     """
     Get the version of the package.
@@ -122,15 +123,15 @@
             else:
                 return space * 2
     else:
         return os.path.getsize(path) * 2
 
 
 def get_memory_consumption() -> int:
-    process = psutil.Process(os.getpid())
+    process = psutil.Process(mp.current_process().pid)
     memory_usage_mb = process.memory_info().rss / 1024 / 1024
     return round(memory_usage_mb, 2)
 
 
 def get_line_positions(path: str):
     """
     Get all line positions in the given file. So that it could be re-used to read the file for a specific line.
```

### Comparing `twb_project-0.7.3a9/setup.py` & `twb_project-0.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'py7zr>=0.20.5,<0.21.0',
  'requests>=2.28.2,<3.0.0',
  'xmltodict>=0.13.0,<0.14.0',
  'zstandard>=0.21.0,<0.22.0']
 
 setup_kwargs = {
     'name': 'twb-project',
-    'version': '0.7.3a9',
+    'version': '0.8.0',
     'description': 'An unified tool for the research in extracting information from Wikipedia Edit History chunk.',
     'long_description': '<img src="https://imagedelivery.net/Dr98IMl5gQ9tPkFM5JRcng/49178640-2f6d-4c23-e56f-a48eca531200/HD" alt="TWB" />\n\n# Temporal Wikipedia Blocks (TWB)\n\nTemporal Wikipedia Blocks (TWB) is a powerful Python package designed to process the extensive edit history of Wikipedia pages into easily manageable and memory-friendly blocks. The package is specifically developed to enable efficient parallelization and composition of these blocks to facilitate faster processing and analysis of large Wikipedia datasets. The original design of this package is to build other Wikipedia-oriented datasets on top of it.\n\nThe package works by dividing the Wikipedia edit history into temporal blocks, which are essentially subsets of the complete dataset that are based on time intervals. These blocks can then be easily processed and analyzed without the need to load the entire dataset into memory.\n\n## Installation\n\nThe package is available on PyPI and can be installed using pip:\n\n```bash\npip install twb-project\n```\n\n## Benefits\n\n- **Efficient**: The package is designed to be memory-friendly and can be easily parallelized to process large datasets.\n- **Fast**: The package is designed to be fast and can be easily optimized to process large datasets.\n- **Flexible**: The package is designed to be flexible and can be easily extended to support other types of blocks.\n- **Composable**: The package is designed to be composable and can be easily combined with other packages to build other datasets.\n\n## Specification\n\n- Default compression method: ZStandard.\n',
     'author': 'Lingxi Li',
     'author_email': 'hi@lingxi.li',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://twb.lingxi.li/',
```

### Comparing `twb_project-0.7.3a9/PKG-INFO` & `twb_project-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twb-project
-Version: 0.7.3a9
+Version: 0.8.0
 Summary: An unified tool for the research in extracting information from Wikipedia Edit History chunk.
 Home-page: https://twb.lingxi.li/
 License: GNU GPL
 Author: Lingxi Li
 Author-email: hi@lingxi.li
 Requires-Python: >=3.8,<4
 Classifier: License :: Other/Proprietary License
```

