# Comparing `tmp/neopolitan-0.1.3.tar.gz` & `tmp/neopolitan-0.1.4.tar.gz`

## Comparing `neopolitan-0.1.3.tar` & `neopolitan-0.1.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 neopolitan-0.1.3/.pylintrc
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 neopolitan-0.1.3/Notes.md
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 neopolitan-0.1.3/pytest.ini
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 neopolitan-0.1.3/requirements.txt
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 neopolitan-0.1.3/.github/workflows/python-package.yml
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 neopolitan-0.1.3/.vscode/settings.json
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 neopolitan-0.1.3/neopolitan/ReadMe.md
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 neopolitan-0.1.3/neopolitan/__init__.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 neopolitan-0.1.3/neopolitan/const.py
--rw-r--r--   0        0        0     5715 2020-02-02 00:00:00.000000 neopolitan-0.1.3/neopolitan/neop.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 neopolitan-0.1.3/neopolitan/os_detection.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 neopolitan-0.1.3/neopolitan/testboardrunner.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 neopolitan-0.1.3/neopolitan/board_functions/__init__.py
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 neopolitan-0.1.3/neopolitan/board_functions/board.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 neopolitan-0.1.3/neopolitan/board_functions/board_data.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 neopolitan-0.1.3/neopolitan/board_functions/colors.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 neopolitan-0.1.3/neopolitan/display/__init__.py
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 neopolitan-0.1.3/neopolitan/display/abstract_board_display.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 neopolitan-0.1.3/neopolitan/display/abstract_display.py
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 neopolitan-0.1.3/neopolitan/display/graphical_board_display.py
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 neopolitan-0.1.3/neopolitan/display/graphical_display.py
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 neopolitan-0.1.3/neopolitan/display/hardware_board_display.py
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 neopolitan-0.1.3/neopolitan/display/hardware_display.py
--rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 neopolitan-0.1.3/neopolitan/writing/ReadMe.md
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 neopolitan-0.1.3/neopolitan/writing/__init__.py
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 neopolitan-0.1.3/neopolitan/writing/data_transformation.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 neopolitan-0.1.3/neopolitan/writing/groups_8.py
--rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 neopolitan-0.1.3/neopolitan/writing/letters_8.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 neopolitan-0.1.3/tests/ReadMe.md
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 neopolitan-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 neopolitan-0.1.3/tests/board_test.py
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 neopolitan-0.1.3/tests/data_transformation_test.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 neopolitan-0.1.3/tests/flip_test.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 neopolitan-0.1.3/tests/groups_test.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 neopolitan-0.1.3/tests/process_board_data_test.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 neopolitan-0.1.3/visual_tests/__init__.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 neopolitan-0.1.3/visual_tests/demo_test.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 neopolitan-0.1.3/visual_tests/main_test.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 neopolitan-0.1.3/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 neopolitan-0.1.3/LICENSE
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 neopolitan-0.1.3/README.md
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 neopolitan-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 neopolitan-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 neopolitan-0.1.4/.pylintrc
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 neopolitan-0.1.4/Notes.md
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 neopolitan-0.1.4/pytest.ini
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 neopolitan-0.1.4/requirements.txt
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 neopolitan-0.1.4/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 neopolitan-0.1.4/.vscode/settings.json
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 neopolitan-0.1.4/neopolitan/ReadMe.md
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 neopolitan-0.1.4/neopolitan/__init__.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 neopolitan-0.1.4/neopolitan/const.py
+-rw-r--r--   0        0        0     6192 2020-02-02 00:00:00.000000 neopolitan-0.1.4/neopolitan/neop.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 neopolitan-0.1.4/neopolitan/os_detection.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 neopolitan-0.1.4/neopolitan/testboardrunner.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 neopolitan-0.1.4/neopolitan/board_functions/__init__.py
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 neopolitan-0.1.4/neopolitan/board_functions/board.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 neopolitan-0.1.4/neopolitan/board_functions/board_data.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 neopolitan-0.1.4/neopolitan/board_functions/colors.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 neopolitan-0.1.4/neopolitan/display/__init__.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 neopolitan-0.1.4/neopolitan/display/abstract_board_display.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 neopolitan-0.1.4/neopolitan/display/abstract_display.py
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 neopolitan-0.1.4/neopolitan/display/graphical_board_display.py
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 neopolitan-0.1.4/neopolitan/display/graphical_display.py
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 neopolitan-0.1.4/neopolitan/display/hardware_board_display.py
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 neopolitan-0.1.4/neopolitan/display/hardware_display.py
+-rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 neopolitan-0.1.4/neopolitan/writing/ReadMe.md
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 neopolitan-0.1.4/neopolitan/writing/__init__.py
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 neopolitan-0.1.4/neopolitan/writing/data_transformation.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 neopolitan-0.1.4/neopolitan/writing/groups_8.py
+-rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 neopolitan-0.1.4/neopolitan/writing/letters_8.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 neopolitan-0.1.4/tests/ReadMe.md
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 neopolitan-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 neopolitan-0.1.4/tests/board_test.py
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 neopolitan-0.1.4/tests/data_transformation_test.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 neopolitan-0.1.4/tests/flip_test.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 neopolitan-0.1.4/tests/groups_test.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 neopolitan-0.1.4/tests/process_board_data_test.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 neopolitan-0.1.4/visual_tests/__init__.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 neopolitan-0.1.4/visual_tests/demo_test.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 neopolitan-0.1.4/visual_tests/main_test.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 neopolitan-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 neopolitan-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 neopolitan-0.1.4/README.md
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 neopolitan-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 neopolitan-0.1.4/PKG-INFO
```

### Comparing `neopolitan-0.1.3/.github/workflows/python-package.yml` & `neopolitan-0.1.4/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.3/neopolitan/ReadMe.md` & `neopolitan-0.1.4/neopolitan/ReadMe.md`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.3/neopolitan/neop.py` & `neopolitan-0.1.4/neopolitan/neop.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,43 @@
 """Main application function"""
 
 # pylint: disable=fixme
 # pylint: disable=too-many-nested-blocks
 # pylint: disable=too-many-statements
 # pylint: disable=too-many-branches
 # pylint: disable=import-outside-toplevel
+# pylint: disable=logging-fstring-interpolation
 # ToDo: fix this
 
 # todo: only import pygame if on graphical
 
 import getopt
 import sys
 import time
+import logging
+import datetime
 
 from neopolitan.board_functions.board import Board
 # from board_functions.colors import OFF, ON
 from neopolitan.board_functions.board_data import default_board_data
 from neopolitan.writing.data_transformation import str_to_data
 from neopolitan.os_detection import on_pi
 # pylint: disable=wildcard-import
 from neopolitan.const import *
 
+def initialize_logger():
+    """Set up the log file"""
+    filename = 'neopolitan/logs/' + str(datetime.datetime.now()) + '.txt'
+    logging.basicConfig(filename=filename, encoding='utf=8', level=logging.DEBUG)
 
 def main(events=None):
     """Make a very simple display"""
 
+    initialize_logger()
+
     board_data = process_arguments()
 
     width = WIDTH
     height = HEIGHT
     size = width*height
     board = None
     display = None
@@ -48,24 +57,24 @@
     board.set_data(str_to_data(board_data.message))
 
     while not display.should_exit:
         # process events
         # todo: make better
         while events and not events.empty():
             event = events.get()
-            print('event:', event)
+            logging.info(f'event: {event}')
             event_list = event.split()
             first = event_list[0]
             if first == 'exit':
                 return
             if first == 'say':
-                print('e:', event)
+                logging.info(f'e: {event}')
                 message = event_list[1]
                 board.set_data(str_to_data(message))
-                print('set message:', message)
+                logging.info(f'set message: {message}')
             else: # try board data events
                 board_data = process_board_data_events(board_data, event_list)
             # todo: error handling
         display.loop()
         if board_data.scroll_speed:
             board.scroll(wrap=board_data.should_wrap)
 
@@ -86,76 +95,76 @@
         if len(args[0]) > 0:
             for arg, val in args[0]:
                 if arg in ('-m', '--message'):
                     board_data.message = val
                 elif arg in ('-g', '--graphical'):
                     if val == 'True':
                         if on_pi():
-                            print('This code cannot be run in graphical mode on a Raspberry Pi,'\
+                            logging.warning('This code cannot be run in graphical mode on a Raspberry Pi,'\
                                 ' setting graphical to False')
                             board_data.graphical = False
                         else:
                             board_data.graphical = True
                     elif val == 'False':
                         if not on_pi():
-                            print('This code cannot be run in hardware mode when not run'\
+                            logging.warning('This code cannot be run in hardware mode when not run'\
                             ' on a Raspberry Pi, setting graphical to True')
                             board_data.graphical = True
                         else:
                             board_data.graphical = False
                     else:
-                        print('Could not parse "graphical" argument:', val)
+                        logging.warning(f'Could not parse "graphical" argument: {val}')
                 elif arg in ('-s', 'scroll'):
                     if val in ('slow', 'medium', 'fast'):
                         board_data.scroll_speed = val
                         if val == 'slow':
                             board_data.scroll_wait = SCROLL_FAST
                         elif val == 'medium':
                             board_data.scroll_wait = SCROLL_MED
                         else: # fast
                             board_data.scroll_wait = SCROLL_SLOW
                     else:
-                        print('Invalid scroll speed:', val)
+                        logging.warning(f'Invalid scroll speed: {val}')
                 elif arg in ('-w', 'wrap'):
                     if val == 'True':
                         board_data.should_wrap = True
                     elif val == 'False':
                         board_data.should_wrap = False
                     else:
-                        print('Could not parse "wrap" argument:', val)
-        print('message set to:', board_data.message)
-        print('graphical set to:', board_data.graphical)
-        print(f'scroll speed set to: {board_data.scroll_speed} ({board_data.scroll_wait})')
-        print('wrap set to:', board_data.should_wrap)
+                        logging.warning(f'Could not parse "wrap" argument: {val}')
+        logging.info(f'message set to: {board_data.message}')
+        logging.info(f'graphical set to: {board_data.graphical}')
+        logging.info(f'scroll speed set to: {board_data.scroll_speed} ({board_data.scroll_wait})')
+        logging.info(f'wrap set to: {board_data.should_wrap}')
 
     except getopt.error as err:
-        print('getopt error:', str(err))
+        logging.error(f'getopt error: {err}')
 
     return board_data
 
 def process_board_data_events(board_data, event_list):
     """Manipulate board data according to events"""
 
     first = event_list[0]
     if first == 'speed':
         speed = event_list[1]
         if speed == 'slow':
             board_data.scroll_slow()
-            print('set speed: slow')
+            logging.info('set speed: slow')
         elif speed == 'medium':
             board_data.scroll_medium()
-            print('set speed: medium')
+            logging.info('set speed: medium')
         elif speed == 'fast':
             board_data.scroll_fast()
-            print('set speed: fast')
+            logging.info('set speed: fast')
         else:
             try:
                 speed = float(speed)
                 board_data.set_scroll_wait(speed)
-                print('set speed: ', speed)
+                logging.info(f'set speed: {speed}')
             except ValueError:
-                print('Cannot parse speed: ', speed)
+                logging.warning(f'Cannot parse speed: {speed}')
 
     return board_data
 
 if __name__ == '__main__':
     main()
```

### Comparing `neopolitan-0.1.3/neopolitan/testboardrunner.py` & `neopolitan-0.1.4/neopolitan/testboardrunner.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,12 +17,10 @@
 
     Thread(target=add_to_queue, args=(events, 'speed fast', 1,)).start()
     Thread(target=add_to_queue, args=(events, 'speed 1.0', 2,)).start()
     Thread(target=add_to_queue, args=(events, 'speed banana', 3,)).start()
     Thread(target=add_to_queue, args=(events, 'say abcdefg', 5,)).start()
     Thread(target=add_to_queue, args=(events, 'exit', 8,)).start()
 
-    # todo: 'off' event
-
-    # t.join() # no difference
+    t.join() # no difference
 
 runner()
```

### Comparing `neopolitan-0.1.3/neopolitan/board_functions/board.py` & `neopolitan-0.1.4/neopolitan/board_functions/board.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """LED board data"""
 
 # pylint: disable=fixme
+import logging
 from neopolitan.board_functions.colors import ON, OFF
 
 class Board:
     """Represents the colors for a board"""
 
     # pylint: disable=pointless-string-statement
     """
@@ -33,15 +34,15 @@
             data = data[0:self.size]
         self.data = data
 
     def turn_on(self, idx, color=ON):
         """Set the color of a given idx (default=white)"""
         if idx >= len(self.data):
             # pylint: disable=consider-using-f-string
-            print('index {0} out of bounds: size = {1}'.format(idx, self.size))
+            logging.warning('index {0} out of bounds: size = {1}'.format(idx, self.size))
             return
         self.data[idx] = color
 
     def turn_off(self, idx):
         """'Turn off' a given idx (set to None)"""
         # todo: what about with led board?
         self.data[idx] = OFF
```

### Comparing `neopolitan-0.1.3/neopolitan/board_functions/board_data.py` & `neopolitan-0.1.4/neopolitan/board_functions/board_data.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.3/neopolitan/display/graphical_board_display.py` & `neopolitan-0.1.4/neopolitan/display/graphical_board_display.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Draws a board"""
 
 import pygame
+import logging
 from neopolitan.display.abstract_board_display import BoardDisplay
 from neopolitan.const import WIDTH, HEIGHT
 # from board import Board
 
 class GraphicalBoardDisplay(BoardDisplay):
     """Draws board data"""
     width = 0
@@ -22,15 +23,15 @@
     # pylint: disable=arguments-differ
     def draw_board(self, screen, space, size):
         """Draw all the 'lights' in the board"""
         assert self.board, 'No board assigned'
 
         for i in range(self.width * self.height):
             if i >= len(self.board.data):
-                print("index", i, "outside of data array bounds")
+                logging.warning(f'index {i} outside of data array bounds')
                 return
             color = self.board.data[i]
             row = self.get_row(i)
             col = self.get_col(i)
 
             if not self.board.data[i]:
                 continue
```

### Comparing `neopolitan-0.1.3/neopolitan/display/graphical_display.py` & `neopolitan-0.1.4/neopolitan/display/graphical_display.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.3/neopolitan/display/hardware_board_display.py` & `neopolitan-0.1.4/neopolitan/display/hardware_board_display.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Interacts with the LED board"""
 
+import logging
 from neopolitan.display.abstract_board_display import BoardDisplay
 from neopolitan.const import WIDTH, HEIGHT
 
 class HardwareBoardDisplay(BoardDisplay):
     """Draws board data"""
 
     def __init__(self, board, pixels, size=WIDTH*HEIGHT):
@@ -20,15 +21,15 @@
         """Sets all the LEDs in accordance with the current data"""
         assert self.board, 'No board assigned'
 
         flipped_data = HardwareBoardDisplay.flip(self.board.data, HEIGHT)
 
         for i in range(self.size):
             if i >= len(self.board.data):
-                print("index", i, "outside of data array bounds")
+                logging.warning(f'index {i} outside of data array bounds')
                 return
             self.pixels[i] = flipped_data[i]
 
     # pylint: disable=no-self-argument
     def flip(data, height=HEIGHT, start_at_first=False):
         """
         Handles flipping alternate 'rows' so that data appears as expected;
```

### Comparing `neopolitan-0.1.3/neopolitan/display/hardware_display.py` & `neopolitan-0.1.4/neopolitan/display/hardware_display.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.3/neopolitan/writing/ReadMe.md` & `neopolitan-0.1.4/neopolitan/writing/ReadMe.md`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.3/neopolitan/writing/data_transformation.py` & `neopolitan-0.1.4/neopolitan/writing/data_transformation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Takes letters as defined and transforms them into usable data"""
 
 # pylint: disable=fixme
 # Todo: location?
 # todo
 from math import floor
+import logging
 from neopolitan.writing.groups_8 import uppercase, lowercase, symbols, numbers
 from neopolitan.board_functions.colors import ON, OFF
 
 def character_to_symbol(char):
     """Gets the symbol for the character"""
     ascii_val = ord(char)
     # todo: make everything like for symbols?
@@ -18,15 +19,15 @@
         return lowercase[ascii_val-97]
     if 65 <= ascii_val < 91:
         return uppercase[ascii_val-65]
     if 48 <= ascii_val < 58:
         return numbers[ascii_val-48]
     if char in symbols:
         return symbols[char]
-    print("Cannot find char: " + char)
+    logging.warning(f'Cannot find char: {char}')
     return []
 
 def frame_length(sym):
     """Returns the highest multiple of 8 above the largest index in the symbol array.
     This makes it so the frame has the correct length, since it should 'fill' all columns it uses"""
     if sym == 'space':
         return 8*2
```

### Comparing `neopolitan-0.1.3/neopolitan/writing/groups_8.py` & `neopolitan-0.1.4/neopolitan/writing/groups_8.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.3/neopolitan/writing/letters_8.py` & `neopolitan-0.1.4/neopolitan/writing/letters_8.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.3/tests/board_test.py` & `neopolitan-0.1.4/tests/board_test.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.3/tests/data_transformation_test.py` & `neopolitan-0.1.4/tests/data_transformation_test.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.3/tests/flip_test.py` & `neopolitan-0.1.4/tests/flip_test.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.3/tests/groups_test.py` & `neopolitan-0.1.4/tests/groups_test.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.3/tests/process_board_data_test.py` & `neopolitan-0.1.4/tests/process_board_data_test.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.3/.gitignore` & `neopolitan-0.1.4/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+neopolitan/logs/*
+
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
```

### Comparing `neopolitan-0.1.3/LICENSE` & `neopolitan-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.3/README.md` & `neopolitan-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.3/pyproject.toml` & `neopolitan-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "neopolitan"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
     { name = "alyo" },
 ]
 description = "Neopolitan: a library for displaying text on LED boards"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `neopolitan-0.1.3/PKG-INFO` & `neopolitan-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neopolitan
-Version: 0.1.3
+Version: 0.1.4
 Summary: Neopolitan: a library for displaying text on LED boards
 Project-URL: Homepage, https://github.com/alyoshenka/neopolitan
 Author: alyo
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

