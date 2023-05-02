# Comparing `tmp/visualtest_python-1.3.1-py3-none-any.whl.zip` & `tmp/visualtest_python-1.3.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 20523 bytes, number of entries: 11
--rw-r--r--  2.0 unx     1129 b- defN 23-Apr-27 18:10 sbvt/__init__.py
+Zip file size: 20590 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     1129 b- defN 23-May-01 23:30 sbvt/__init__.py
 -rw-r--r--  2.0 unx     9114 b- defN 23-Apr-26 16:54 sbvt/api.py
--rw-r--r--  2.0 unx    34618 b- defN 23-Apr-26 16:54 sbvt/browser.py
+-rw-r--r--  2.0 unx    35178 b- defN 23-May-01 22:54 sbvt/browser.py
 -rw-r--r--  2.0 unx     5981 b- defN 22-Sep-26 14:39 sbvt/imagetools.py
 -rw-r--r--  2.0 unx      548 b- defN 22-Sep-26 14:39 sbvt/timer.py
--rw-r--r--  2.0 unx    11191 b- defN 23-Apr-27 18:10 sbvt/visualtest.py
--rw-r--r--  2.0 unx     1073 b- defN 23-Apr-27 18:21 visualtest_python-1.3.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     3876 b- defN 23-Apr-27 18:21 visualtest_python-1.3.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-27 18:21 visualtest_python-1.3.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Apr-27 18:21 visualtest_python-1.3.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      869 b- defN 23-Apr-27 18:21 visualtest_python-1.3.1.dist-info/RECORD
-11 files, 68496 bytes uncompressed, 19065 bytes compressed:  72.2%
+-rw-r--r--  2.0 unx    11283 b- defN 23-May-01 22:55 sbvt/visualtest.py
+-rw-r--r--  2.0 unx     1073 b- defN 23-May-02 18:15 visualtest_python-1.3.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3876 b- defN 23-May-02 18:15 visualtest_python-1.3.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-02 18:15 visualtest_python-1.3.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-May-02 18:15 visualtest_python-1.3.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      869 b- defN 23-May-02 18:15 visualtest_python-1.3.2.dist-info/RECORD
+11 files, 69148 bytes uncompressed, 19132 bytes compressed:  72.3%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: sbvt/timer.py
 Comment: 
 
 Filename: sbvt/visualtest.py
 Comment: 
 
-Filename: visualtest_python-1.3.1.dist-info/LICENSE
+Filename: visualtest_python-1.3.2.dist-info/LICENSE
 Comment: 
 
-Filename: visualtest_python-1.3.1.dist-info/METADATA
+Filename: visualtest_python-1.3.2.dist-info/METADATA
 Comment: 
 
-Filename: visualtest_python-1.3.1.dist-info/WHEEL
+Filename: visualtest_python-1.3.2.dist-info/WHEEL
 Comment: 
 
-Filename: visualtest_python-1.3.1.dist-info/top_level.txt
+Filename: visualtest_python-1.3.2.dist-info/top_level.txt
 Comment: 
 
-Filename: visualtest_python-1.3.1.dist-info/RECORD
+Filename: visualtest_python-1.3.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sbvt/__init__.py

```diff
@@ -1,14 +1,14 @@
 import logging
 import os.path
 
 # this import statement is here for context.py in tests folder
 from .visualtest import VisualTest
 
-__version__ = '1.3.1'
+__version__ = '1.3.2'
 
 logPath = 'logs'
 if not os.path.exists(logPath):
     os.makedirs(logPath)
 
 # By generating a new logger as 'vt' we don't affect global logging from other packages
 # Each logger created in our package should be a child by prefacing with 'vt.childname'
```

## sbvt/browser.py

```diff
@@ -143,21 +143,25 @@
             with open(path.replace('.png','.json'), 'w') as outfile:
                 json.dump(dom, outfile, indent=4)
 
         return dom
 
     def _findElement(self, cssSelector):
         return self._driver.find_element(By.CSS_SELECTOR, cssSelector)
-    
+
+    def _clearIgnoreElements(self):
+        script = 'delete window.sbvt'
+        self._driver.execute_script(script)
+
     def _injectIgnoreElements(self, ignoreElements):
         script = 'window.sbvt = { ignoreElements: %s }' % json.dumps(ignoreElements)
         self._driver.execute_script(script)
 
     def _freezePage(self):
-        self._driver.execute_script(f'return {self._freezePageScript};')
+        return self._driver.execute_script(f'return {self._freezePageScript};')
 
     def _getPageDimensions(self):
         script = """
             return JSON.stringify({
                 "document": {
                     "height": document.documentElement.clientHeight,
                     "width": document.documentElement.clientWidth
@@ -444,19 +448,20 @@
             log.info(f'Taking single screenshot for single page')
 
             pageStopWatch = StopWatch()
             pageStopWatch.start()
             totalPageTime = 0
 
             # freezePage script
+            freezePageResult = None
             if 'freezePage' in options:
                 if options['freezePage']:
-                    self._freezePage()
+                    freezePageResult = self._freezePage()
             else:
-                self._freezePage()
+                freezePageResult = self._freezePage()
 
             file = os.path.join(self.tmpDir, f'0.png')
             self._driver.save_screenshot(file)
 
             if self._cropEachBottom:
                 file = ImageTools.cropBottom(file, self._cropEachBottom)
 
@@ -484,19 +489,20 @@
 
             # handle lazy-loaded content if setting provided
             if 'lazyload' in options:
                 if options['lazyload'] is not None:
                     self._loadLazyContent(totalPages, options['lazyload'])
 
             # freezePage script
+            freezePageResult = None
             if 'freezePage' in options:
                 if options['freezePage']:
-                    self._freezePage()
+                    freezePageResult = self._freezePage()
             else:
-                self._freezePage()
+                freezePageResult = self._freezePage()
 
             # to hide bottom fixed elements, this is a trick that works on most modern browsers
             log.info(f'PREP: Hiding bottom fixed elements: document.body.style.transform="translateY(0)"')
             self._driver.execute_script(f'document.body.style.transform="translateY(0)"')
             time.sleep(0.5) #some browsers need a little time to apply (Safari)
 
             done = False
@@ -645,15 +651,16 @@
                 'width': expectedImageWidth,
                 'height': expectedImageHeight
             },
             'devicePixelRatio': self.devicePixelRatio,
             'reasonStopped': reasonStopped,
             'duration': f'{totalFullpageTime} seconds',
             'averagePageTime': f'{averagePageTime} seconds',
-            'url': self._driver.current_url
+            'url': self._driver.current_url,
+            'freezePageResult': freezePageResult
         }
 
         log.info(f'Result: {result}')
         result['dom'] = self.dom #add dom after logging result
 
         # delete the temp screenshot images used to build fullpage
         if not self._debugImages:
@@ -672,19 +679,20 @@
         self.watch = StopWatch()
         self.watch.start()
 
         # create tmp directory for storing images that will be stitched together
         self._createTmpDir(os.path.dirname(path), 'element')
 
         # freezePage script
+        freezePageResult = None
         if 'freezePage' in options:
             if options['freezePage']:
-                self._freezePage()
+                freezePageResult = self._freezePage()
         else:
-            self._freezePage()
+            freezePageResult = self._freezePage()
 
         # update the dimensions of the browser window and webpage
         self._getPageDimensions()
 
         # selenium.webdriver.firefox.webelement.FirefoxWebElement
         log.debug(f'type of element is {type(options["element"])}')
         log.info(f'Taking element screenshot of element')
@@ -700,15 +708,16 @@
         result = {
             'imagePath': path,
             'imageSize': {
                 'width': imageWidth,
                 'height': imageHeight
             },
             'duration': f'{totalTime} seconds',
-            'url': self._driver.current_url
+            'url': self._driver.current_url,
+            'freezePageResult': freezePageResult
         }
 
         log.info(f'Result: {result}')
         result['dom'] = self.dom #add dom after logging result
 
         if not self._debugImages:
             self._deleteTmpDir()
@@ -727,19 +736,20 @@
         self.watch = StopWatch()
         self.watch.start()
 
         # create tmp directory for storing images that will be stitched together
         self._createTmpDir(os.path.dirname(path), 'viewport')
 
         # freezePage script
+        freezePageResult = None
         if 'freezePage' in options:
             if options['freezePage']:
-                self._freezePage()
+                freezePageResult = self._freezePage()
         else:
-            self._freezePage()
+            freezePageResult = self._freezePage()
 
         # get initial page state for returning to later (must do before hiding scrollbar)
         self._getInitialPageState()
 
         # hide scroll bar for accurate dimensions
         hideScrollBarResult = self._driver.execute_script('return document.body.style.overflow="hidden";')
         log.info(f'PREP: Hide scrollbar result: {hideScrollBarResult}')
@@ -781,15 +791,16 @@
             },
             'expectedSize': {
                 'width': expectedImageWidth,
                 'height': expectedImageHeight
             },
             'devicePixelRatio': self.devicePixelRatio,
             'duration': f'{totalTime} seconds',
-            'url': self._driver.current_url
+            'url': self._driver.current_url,
+            'freezePageResult': freezePageResult
         }
 
         log.info(f'Result: {result}')
         result['dom'] = self.dom #add dom after logging result
 
         if not self._debugImages:
             self._deleteTmpDir()
```

## sbvt/visualtest.py

```diff
@@ -201,14 +201,15 @@
 
         if len(name) > 100:
             raise Exception(f'Name argument cannot be greater than 100 characters')
 
         filePath = os.path.join(self._settings['saveTo'],f'{name}.png')
         imageType = None
 
+        self.browser._clearIgnoreElements() #clear the window from previous ignoredElements
         if 'ignoreElements' in options:
             if not isinstance(options['ignoreElements'], list):
                 raise Exception(f'ignoreElements must be of type "list"')
             if not all(isinstance(item, str) for item in options['ignoreElements']):
                 raise Exception(f'ignoreElements values must all be strings')
             
             elementsNotFound = []
```

## Comparing `visualtest_python-1.3.1.dist-info/LICENSE` & `visualtest_python-1.3.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `visualtest_python-1.3.1.dist-info/METADATA` & `visualtest_python-1.3.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visualtest-python
-Version: 1.3.1
+Version: 1.3.2
 Summary: Python SDK for SmartBear VisualTest via Selenium WebDriver
 Home-page: https://github.com/SmartBear/visualtest-python
 Author: Luke Kende
 Author-email: luke.kende@smartbear.com
 Keywords: visual testing,UI testing,GUI testing,UX testing,screenshots,full page screenshots,image comparisons,regression testing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

