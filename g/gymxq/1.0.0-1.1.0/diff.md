# Comparing `tmp/gymxq-1.0.0.tar.gz` & `tmp/gymxq-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gymxq-1.0.0.tar", last modified: Thu Apr 27 08:34:38 2023, max compression
+gzip compressed data, was "gymxq-1.1.0.tar", last modified: Tue May  2 20:15:25 2023, max compression
```

## Comparing `gymxq-1.0.0.tar` & `gymxq-1.1.0.tar`

### file list

```diff
@@ -1,41 +1,40 @@
-drwxr-xr-x   0 ldf       (1000) ldf       (1000)        0 2023-04-27 08:34:38.376167 gymxq-1.0.0/
--rw-r--r--   0 ldf       (1000) ldf       (1000)     1060 2023-02-22 19:35:09.000000 gymxq-1.0.0/LICENSE
--rw-r--r--   0 ldf       (1000) ldf       (1000)       59 2023-03-06 02:50:57.000000 gymxq-1.0.0/MANIFEST.in
--rw-r--r--   0 ldf       (1000) ldf       (1000)      161 2023-04-27 08:34:38.376167 gymxq-1.0.0/PKG-INFO
--rw-r--r--   0 ldf       (1000) ldf       (1000)     2285 2023-03-01 07:45:02.000000 gymxq-1.0.0/README.md
-drwxr-xr-x   0 ldf       (1000) ldf       (1000)        0 2023-04-27 08:34:38.376167 gymxq-1.0.0/gymxq/
--rw-r--r--   0 ldf       (1000) ldf       (1000)      357 2023-03-08 05:54:44.000000 gymxq-1.0.0/gymxq/__init__.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)      671 2023-03-08 05:55:03.000000 gymxq-1.0.0/gymxq/constants.py
-drwxr-xr-x   0 ldf       (1000) ldf       (1000)        0 2023-04-27 08:34:38.376167 gymxq-1.0.0/gymxq/envs/
--rw-r--r--   0 ldf       (1000) ldf       (1000)       42 2023-03-01 08:26:31.000000 gymxq-1.0.0/gymxq/envs/__init__.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)     6645 2023-03-27 03:04:58.000000 gymxq-1.0.0/gymxq/envs/game.py
--rw-r--r--   0 ldf       (1000) ldf       (1000)    19398 2023-03-27 03:07:41.000000 gymxq-1.0.0/gymxq/envs/xiangqi.py
-drwxr-xr-x   0 ldf       (1000) ldf       (1000)        0 2023-04-27 08:34:38.376167 gymxq-1.0.0/gymxq/resources/
--rw-r--r--   0 ldf       (1000) ldf       (1000)     5593 2023-02-22 19:35:09.000000 gymxq-1.0.0/gymxq/resources/bA.png
--rw-r--r--   0 ldf       (1000) ldf       (1000)     6473 2023-02-22 19:35:09.000000 gymxq-1.0.0/gymxq/resources/bB.png
--rw-r--r--   0 ldf       (1000) ldf       (1000)     6637 2023-02-22 19:35:09.000000 gymxq-1.0.0/gymxq/resources/bC.png
--rw-r--r--   0 ldf       (1000) ldf       (1000)     6754 2023-02-22 19:35:09.000000 gymxq-1.0.0/gymxq/resources/bK.png
--rw-r--r--   0 ldf       (1000) ldf       (1000)     6393 2023-02-22 19:35:09.000000 gymxq-1.0.0/gymxq/resources/bN.png
--rw-r--r--   0 ldf       (1000) ldf       (1000)     6162 2023-02-22 19:35:09.000000 gymxq-1.0.0/gymxq/resources/bP.png
--rw-r--r--   0 ldf       (1000) ldf       (1000)     6191 2023-02-22 19:35:09.000000 gymxq-1.0.0/gymxq/resources/bR.png
--rw-r--r--   0 ldf       (1000) ldf       (1000)    33967 2023-02-22 19:35:09.000000 gymxq-1.0.0/gymxq/resources/board540x600.png
--rw-r--r--   0 ldf       (1000) ldf       (1000)      182 2023-02-22 19:35:09.000000 gymxq-1.0.0/gymxq/resources/cross.png
--rw-r--r--   0 ldf       (1000) ldf       (1000)      457 2023-02-22 19:35:09.000000 gymxq-1.0.0/gymxq/resources/frame.png
--rw-r--r--   0 ldf       (1000) ldf       (1000)     4286 2023-02-22 19:35:09.000000 gymxq-1.0.0/gymxq/resources/icon.ico
--rw-r--r--   0 ldf       (1000) ldf       (1000)     5677 2023-02-22 19:35:09.000000 gymxq-1.0.0/gymxq/resources/rA.png
--rw-r--r--   0 ldf       (1000) ldf       (1000)     5989 2023-02-22 19:35:09.000000 gymxq-1.0.0/gymxq/resources/rB.png
--rw-r--r--   0 ldf       (1000) ldf       (1000)     6313 2023-02-22 19:35:09.000000 gymxq-1.0.0/gymxq/resources/rC.png
--rw-r--r--   0 ldf       (1000) ldf       (1000)     6012 2023-02-22 19:35:09.000000 gymxq-1.0.0/gymxq/resources/rK.png
--rw-r--r--   0 ldf       (1000) ldf       (1000)     6217 2023-02-22 19:35:09.000000 gymxq-1.0.0/gymxq/resources/rN.png
--rw-r--r--   0 ldf       (1000) ldf       (1000)     5790 2023-02-22 19:35:09.000000 gymxq-1.0.0/gymxq/resources/rP.png
--rw-r--r--   0 ldf       (1000) ldf       (1000)     6031 2023-02-22 19:35:09.000000 gymxq-1.0.0/gymxq/resources/rR.png
--rw-r--r--   0 ldf       (1000) ldf       (1000)     1871 2023-02-22 19:35:09.000000 gymxq-1.0.0/gymxq/resources/right.png
--rw-r--r--   0 ldf       (1000) ldf       (1000)    12345 2023-03-08 06:49:07.000000 gymxq-1.0.0/gymxq/utils.py
-drwxr-xr-x   0 ldf       (1000) ldf       (1000)        0 2023-04-27 08:34:38.376167 gymxq-1.0.0/gymxq.egg-info/
--rw-r--r--   0 ldf       (1000) ldf       (1000)      161 2023-04-27 08:34:38.000000 gymxq-1.0.0/gymxq.egg-info/PKG-INFO
--rw-r--r--   0 ldf       (1000) ldf       (1000)      756 2023-04-27 08:34:38.000000 gymxq-1.0.0/gymxq.egg-info/SOURCES.txt
--rw-r--r--   0 ldf       (1000) ldf       (1000)        1 2023-04-27 08:34:38.000000 gymxq-1.0.0/gymxq.egg-info/dependency_links.txt
--rw-r--r--   0 ldf       (1000) ldf       (1000)       91 2023-04-27 08:34:38.000000 gymxq-1.0.0/gymxq.egg-info/requires.txt
--rw-r--r--   0 ldf       (1000) ldf       (1000)        6 2023-04-27 08:34:38.000000 gymxq-1.0.0/gymxq.egg-info/top_level.txt
--rw-r--r--   0 ldf       (1000) ldf       (1000)       38 2023-04-27 08:34:38.376167 gymxq-1.0.0/setup.cfg
--rw-r--r--   0 ldf       (1000) ldf       (1000)      626 2023-04-27 08:34:30.000000 gymxq-1.0.0/setup.py
+drwxr-xr-x   0 ldf       (1000) ldf       (1000)        0 2023-05-02 20:15:25.362167 gymxq-1.1.0/
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     1060 2023-02-22 19:35:09.000000 gymxq-1.1.0/LICENSE
+-rw-r--r--   0 ldf       (1000) ldf       (1000)       59 2023-03-06 02:50:57.000000 gymxq-1.1.0/MANIFEST.in
+-rw-r--r--   0 ldf       (1000) ldf       (1000)      161 2023-05-02 20:15:25.352167 gymxq-1.1.0/PKG-INFO
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     2285 2023-03-01 07:45:02.000000 gymxq-1.1.0/README.md
+drwxr-xr-x   0 ldf       (1000) ldf       (1000)        0 2023-05-02 20:15:25.352167 gymxq-1.1.0/gymxq/
+-rw-r--r--   0 ldf       (1000) ldf       (1000)      357 2023-03-08 05:54:44.000000 gymxq-1.1.0/gymxq/__init__.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)      671 2023-03-08 05:55:03.000000 gymxq-1.1.0/gymxq/constants.py
+drwxr-xr-x   0 ldf       (1000) ldf       (1000)        0 2023-05-02 20:15:25.352167 gymxq-1.1.0/gymxq/envs/
+-rw-r--r--   0 ldf       (1000) ldf       (1000)       42 2023-03-01 08:26:31.000000 gymxq-1.1.0/gymxq/envs/__init__.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     6645 2023-04-29 07:22:39.000000 gymxq-1.1.0/gymxq/envs/game.py
+-rw-r--r--   0 ldf       (1000) ldf       (1000)    19398 2023-03-27 03:07:41.000000 gymxq-1.1.0/gymxq/envs/xiangqi.py
+drwxr-xr-x   0 ldf       (1000) ldf       (1000)        0 2023-05-02 20:15:25.352167 gymxq-1.1.0/gymxq/resources/
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     4297 2023-05-02 19:34:39.000000 gymxq-1.1.0/gymxq/resources/bA.png
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     5408 2023-05-02 19:40:47.000000 gymxq-1.1.0/gymxq/resources/bB.png
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     5242 2023-05-02 19:38:31.000000 gymxq-1.1.0/gymxq/resources/bC.png
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     5410 2023-05-02 19:42:19.000000 gymxq-1.1.0/gymxq/resources/bK.png
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     5117 2023-05-02 19:43:43.000000 gymxq-1.1.0/gymxq/resources/bN.png
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     4843 2023-05-02 19:45:36.000000 gymxq-1.1.0/gymxq/resources/bP.png
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     4895 2023-05-02 19:44:43.000000 gymxq-1.1.0/gymxq/resources/bR.png
+-rw-r--r--   0 ldf       (1000) ldf       (1000)    41692 2023-05-02 19:36:39.000000 gymxq-1.1.0/gymxq/resources/board540x600.png
+-rw-r--r--   0 ldf       (1000) ldf       (1000)      182 2023-05-02 19:47:07.000000 gymxq-1.1.0/gymxq/resources/cross.png
+-rw-r--r--   0 ldf       (1000) ldf       (1000)      457 2023-05-02 19:47:08.000000 gymxq-1.1.0/gymxq/resources/frame.png
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     4286 2023-05-02 19:48:03.000000 gymxq-1.1.0/gymxq/resources/icon.ico
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     4640 2023-05-02 19:35:10.000000 gymxq-1.1.0/gymxq/resources/rA.png
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     4960 2023-05-02 19:41:46.000000 gymxq-1.1.0/gymxq/resources/rB.png
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     5311 2023-05-02 19:39:28.000000 gymxq-1.1.0/gymxq/resources/rC.png
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     4923 2023-05-02 19:43:03.000000 gymxq-1.1.0/gymxq/resources/rK.png
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     5295 2023-05-02 19:44:06.000000 gymxq-1.1.0/gymxq/resources/rN.png
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     4891 2023-05-02 19:45:56.000000 gymxq-1.1.0/gymxq/resources/rP.png
+-rw-r--r--   0 ldf       (1000) ldf       (1000)     5228 2023-05-02 19:45:07.000000 gymxq-1.1.0/gymxq/resources/rR.png
+-rw-r--r--   0 ldf       (1000) ldf       (1000)    12345 2023-04-29 07:22:39.000000 gymxq-1.1.0/gymxq/utils.py
+drwxr-xr-x   0 ldf       (1000) ldf       (1000)        0 2023-05-02 20:15:25.352167 gymxq-1.1.0/gymxq.egg-info/
+-rw-r--r--   0 ldf       (1000) ldf       (1000)      161 2023-05-02 20:15:25.000000 gymxq-1.1.0/gymxq.egg-info/PKG-INFO
+-rw-r--r--   0 ldf       (1000) ldf       (1000)      730 2023-05-02 20:15:25.000000 gymxq-1.1.0/gymxq.egg-info/SOURCES.txt
+-rw-r--r--   0 ldf       (1000) ldf       (1000)        1 2023-05-02 20:15:25.000000 gymxq-1.1.0/gymxq.egg-info/dependency_links.txt
+-rw-r--r--   0 ldf       (1000) ldf       (1000)       91 2023-05-02 20:15:25.000000 gymxq-1.1.0/gymxq.egg-info/requires.txt
+-rw-r--r--   0 ldf       (1000) ldf       (1000)        6 2023-05-02 20:15:25.000000 gymxq-1.1.0/gymxq.egg-info/top_level.txt
+-rw-r--r--   0 ldf       (1000) ldf       (1000)       38 2023-05-02 20:15:25.362167 gymxq-1.1.0/setup.cfg
+-rw-r--r--   0 ldf       (1000) ldf       (1000)      626 2023-05-02 20:15:05.000000 gymxq-1.1.0/setup.py
```

### Comparing `gymxq-1.0.0/LICENSE` & `gymxq-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gymxq-1.0.0/README.md` & `gymxq-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `gymxq-1.0.0/gymxq/constants.py` & `gymxq-1.1.0/gymxq/constants.py`

 * *Files identical despite different names*

### Comparing `gymxq-1.0.0/gymxq/envs/game.py` & `gymxq-1.1.0/gymxq/envs/game.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import sys
 from typing import List, Optional
 
 import numpy as np
-import xqcpp
+import cppxq
 from ..constants import (
     NUM_ROW,
     NUM_COL,
     NUM_PIECE,
     NUM_HISTORY,
     MAX_NUM_NO_EAT,
     NUM_ACTIONS,
@@ -15,15 +15,15 @@
     RED_PLAYER,
     BLACK_PLAYER,
 )
 from ..utils import move_to_coordinate, make_last_move_qipu
 
 
 def get_init_board(init_fen: Optional[str], use_rule: bool):
-    board = xqcpp.XqBoard()
+    board = cppxq.XqBoard()
     board.reset()
     # 设置移动类型判断规则
     board.set_use_rule_flag(use_rule)
     include_no_eat_ = False
     if init_fen:
         fs = init_fen.split(" ")
         assert len(fs) <= 6, "空格分隔列表数量必须小于6"
@@ -75,27 +75,27 @@
 
         Args:
             action (int): 移动编码 [0,2085]
 
         Returns:
             str: 4位整数代表的移动字符串
         """
-        return xqcpp.a2m(action)
+        return cppxq.a2m(action)
 
     @staticmethod
     def move_string_to_action(move: str) -> int:
         """移动字符串转换为移动编码
 
         Args:
             move (str): 4位整数代表的移动字符串
 
         Returns:
             int: 移动编码
         """
-        return xqcpp.m2a(move)
+        return cppxq.m2a(move)
 
     def get_fen(self):
         """棋盘状态fen字符串
 
         Returns:
             str: fen字符串
         """
@@ -136,16 +136,16 @@
         # next batch
         self.continuous_uneaten_history.append(self.board.no_eat())
         self.to_play_id_history.append(self.player_id_)
         self.legal_actions_history.append(self.board.legal_actions())
 
     def step(self, action):
         if action not in self.legal_actions_history[-1]:
-            legal_moves = [xqcpp.a2m(a) for a in self.legal_actions_history[-1]]
-            to_move = xqcpp.a2m(action)
+            legal_moves = [cppxq.a2m(a) for a in self.legal_actions_history[-1]]
+            to_move = cppxq.a2m(action)
             raise RuntimeError("非法走子。合法移动={}，选中={}".format(legal_moves, to_move))
 
         self.board.move(action)
         self.steps += 1
         # 走子后更新done状态
         termination = self.board.is_finished()
```

### Comparing `gymxq-1.0.0/gymxq/envs/xiangqi.py` & `gymxq-1.1.0/gymxq/envs/xiangqi.py`

 * *Files identical despite different names*

### Comparing `gymxq-1.0.0/gymxq/resources/icon.ico` & `gymxq-1.1.0/gymxq/resources/icon.ico`

 * *Files identical despite different names*

### Comparing `gymxq-1.0.0/gymxq/utils.py` & `gymxq-1.1.0/gymxq/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from contextlib import closing
 from io import StringIO
 from typing import List, Optional
 
 # import pygame
 import six
 import termcolor
-import xqcpp
+import cppxq
 
 from .constants import (
     BLACK_PLAYER,
     BOARD_NUM_PROMPT,
     NUM_COL,
     NUM_ROW,
     PIECE_HEIGHT,
@@ -105,20 +105,20 @@
     if bold:
         attr.append(six.u("1"))
     attrs = six.u(";").join(attr)
     return six.u("\x1b[%sm%s\x1b[0m") % (attrs, string)
 
 
 def render_board_to_text(
-    board: xqcpp.XqBoard, last_move: Optional[str] = None, title: Optional[str] = None
+    board: cppxq.XqBoard, last_move: Optional[str] = None, title: Optional[str] = None
 ):
     """棋盘文本表达
 
     Args:
-        board (xqcpp.XqBoard): 棋盘实例
+        board (cppxq.XqBoard): 棋盘实例
         last_move (Optional[str], optional): 最后移动字符串. Defaults to None.
         title (Optional[str], optional): 标题. Defaults to None.
     Note:
         0.5 ms 速度更快
     """
     outfile = StringIO()
     # outfile = sys.stdout
@@ -163,20 +163,20 @@
     attrs = []
     if bold:
         attrs.append("bold")
     return termcolor.colored(string, color, attrs=attrs)
 
 
 def render_board_to_text_v2(
-    board: xqcpp.XqBoard, last_move: Optional[str] = None, title: Optional[str] = None
+    board: cppxq.XqBoard, last_move: Optional[str] = None, title: Optional[str] = None
 ):
     """棋盘文本表达
 
     Args:
-        board (xqcpp.XqBoard): 棋盘实例
+        board (cppxq.XqBoard): 棋盘实例
         last_move (Optional[str], optional): 最后移动字符串. Defaults to None.
         title (Optional[str], optional): 标题. Defaults to None.
     Note:
         1 ms 慢
     """
     # outfile = StringIO()
     outfile = sys.stdout
@@ -317,15 +317,15 @@
     elif piece.color_id == BLACK_PLAYER:
         if piece.y < y0:
             return "进"
         elif piece.y > y0:
             return "退"
 
 
-def make_last_move_qipu(board: xqcpp.XqBoard, move: str):
+def make_last_move_qipu(board: cppxq.XqBoard, move: str):
     record = ""
     x0, y0, x1, y1 = move_to_coordinate(move)
     piece = board.get_piece(x1, y1)
     assert piece.color_name in ("红", "黑"), "棋子不得为空"
     sames = _get_in_same_col_ys(board, piece, x0)
     # 不存在重叠时或帅、士、象、马棋子移动时
     if len(sames) <= 1 or piece.piece_id in (2, 3, 5, 7):
```

### Comparing `gymxq-1.0.0/gymxq.egg-info/SOURCES.txt` & `gymxq-1.1.0/gymxq.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -26,9 +26,8 @@
 gymxq/resources/icon.ico
 gymxq/resources/rA.png
 gymxq/resources/rB.png
 gymxq/resources/rC.png
 gymxq/resources/rK.png
 gymxq/resources/rN.png
 gymxq/resources/rP.png
-gymxq/resources/rR.png
-gymxq/resources/right.png
+gymxq/resources/rR.png
```

### Comparing `gymxq-1.0.0/setup.py` & `gymxq-1.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # from setuptools import setup, find_packages
 from setuptools import setup
 
 setup(
     name="gymxq",
-    version="1.0.0",
+    version="1.1.0",
     long_description="""
     gymnasium like Chinese xiangqi single agent reinforcement learning environment
     """,
     # packages=find_packages(
     #     # All keyword arguments below are optional:
     #     exclude=["tests", "assets", "report.html"],  # empty by default
     # ),
     include_package_data=True,
     install_requires=[
-        "xqcpp>=1.0.0",
+        "cppxq>=1.0.0",
         "gymnasium>=0.27.0",
         "pygame>=2.1.2",
         "moviepy>=1.0.3",
         "termcolor>=2.2.0",
         "pytest>=7.1.3",
     ],
 )
```

