# Comparing `tmp/tksheet-6.0.3.tar.gz` & `tmp/tksheet-6.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tksheet-6.0.3.tar", last modified: Sun Apr 30 15:35:43 2023, max compression
+gzip compressed data, was "tksheet-6.0.4.tar", last modified: Tue May  2 09:21:47 2023, max compression
```

## Comparing `tksheet-6.0.3.tar` & `tksheet-6.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 15:35:43.047748 tksheet-6.0.3/
--rw-rw-rw-   0        0        0     1101 2023-04-13 09:47:22.000000 tksheet-6.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     3003 2023-04-30 15:35:43.047748 tksheet-6.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2353 2023-04-29 12:52:53.000000 tksheet-6.0.3/README.md
--rw-rw-rw-   0        0        0       86 2023-04-30 15:35:43.047748 tksheet-6.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1025 2023-04-26 17:49:39.000000 tksheet-6.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-30 15:35:43.032125 tksheet-6.0.3/tksheet/
--rw-rw-rw-   0        0        0      351 2023-04-13 08:55:45.000000 tksheet-6.0.3/tksheet/__init__.py
--rw-rw-rw-   0        0        0   165005 2023-04-30 15:29:07.000000 tksheet-6.0.3/tksheet/_tksheet.py
--rw-rw-rw-   0        0        0   103939 2023-04-30 14:48:10.000000 tksheet-6.0.3/tksheet/_tksheet_column_headers.py
--rw-rw-rw-   0        0        0    10233 2023-04-24 07:09:26.000000 tksheet-6.0.3/tksheet/_tksheet_formatters.py
--rw-rw-rw-   0        0        0   321463 2023-04-30 11:33:25.000000 tksheet-6.0.3/tksheet/_tksheet_main_table.py
--rw-rw-rw-   0        0        0    14797 2023-04-30 11:47:18.000000 tksheet-6.0.3/tksheet/_tksheet_other_classes.py
--rw-rw-rw-   0        0        0   102184 2023-04-30 08:50:43.000000 tksheet-6.0.3/tksheet/_tksheet_row_index.py
--rw-rw-rw-   0        0        0     5646 2023-04-29 16:37:13.000000 tksheet-6.0.3/tksheet/_tksheet_top_left_rectangle.py
--rw-rw-rw-   0        0        0    52360 2023-04-30 11:47:39.000000 tksheet-6.0.3/tksheet/_tksheet_vars.py
-drwxrwxrwx   0        0        0        0 2023-04-30 15:35:43.047748 tksheet-6.0.3/tksheet.egg-info/
--rw-rw-rw-   0        0        0     3003 2023-04-30 15:35:43.000000 tksheet-6.0.3/tksheet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2023-04-30 15:35:43.000000 tksheet-6.0.3/tksheet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 15:35:43.000000 tksheet-6.0.3/tksheet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-30 15:35:43.000000 tksheet-6.0.3/tksheet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 09:21:47.752989 tksheet-6.0.4/
+-rw-rw-rw-   0        0        0     1101 2023-04-13 09:47:22.000000 tksheet-6.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     3003 2023-05-02 09:21:47.752989 tksheet-6.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2353 2023-04-29 12:52:53.000000 tksheet-6.0.4/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-02 09:21:47.753991 tksheet-6.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1025 2023-05-02 07:35:47.000000 tksheet-6.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:21:47.748987 tksheet-6.0.4/tksheet/
+-rw-rw-rw-   0        0        0      351 2023-04-13 08:55:45.000000 tksheet-6.0.4/tksheet/__init__.py
+-rw-rw-rw-   0        0        0   165045 2023-05-02 09:00:05.000000 tksheet-6.0.4/tksheet/_tksheet.py
+-rw-rw-rw-   0        0        0   104398 2023-05-02 09:01:02.000000 tksheet-6.0.4/tksheet/_tksheet_column_headers.py
+-rw-rw-rw-   0        0        0    10233 2023-05-02 08:49:43.000000 tksheet-6.0.4/tksheet/_tksheet_formatters.py
+-rw-rw-rw-   0        0        0   311455 2023-05-02 09:00:57.000000 tksheet-6.0.4/tksheet/_tksheet_main_table.py
+-rw-rw-rw-   0        0        0    14797 2023-04-30 11:47:18.000000 tksheet-6.0.4/tksheet/_tksheet_other_classes.py
+-rw-rw-rw-   0        0        0   102583 2023-05-02 09:01:05.000000 tksheet-6.0.4/tksheet/_tksheet_row_index.py
+-rw-rw-rw-   0        0        0     5651 2023-05-02 07:44:31.000000 tksheet-6.0.4/tksheet/_tksheet_top_left_rectangle.py
+-rw-rw-rw-   0        0        0    52380 2023-05-02 08:58:51.000000 tksheet-6.0.4/tksheet/_tksheet_vars.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:21:47.752989 tksheet-6.0.4/tksheet.egg-info/
+-rw-rw-rw-   0        0        0     3003 2023-05-02 09:21:47.000000 tksheet-6.0.4/tksheet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2023-05-02 09:21:47.000000 tksheet-6.0.4/tksheet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 09:21:47.000000 tksheet-6.0.4/tksheet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-02 09:21:47.000000 tksheet-6.0.4/tksheet.egg-info/top_level.txt
```

### Comparing `tksheet-6.0.3/LICENSE.txt` & `tksheet-6.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tksheet-6.0.3/PKG-INFO` & `tksheet-6.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tksheet
-Version: 6.0.3
+Version: 6.0.4
 Summary: Tkinter table / sheet widget
 Home-page: https://github.com/ragardner/tksheet
-Download-URL: https://github.com/ragardner/tksheet/archive/6.0.3.tar.gz
+Download-URL: https://github.com/ragardner/tksheet/archive/6.0.4.tar.gz
 Author: ragardner
 Author-email: github@ragardner.simplelogin.com
 License: MIT
 Keywords: tkinter,table,widget,sheet,grid,tk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `tksheet-6.0.3/README.md` & `tksheet-6.0.4/README.md`

 * *Files identical despite different names*

### Comparing `tksheet-6.0.3/setup.py` & `tksheet-6.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding = 'utf-8') as f:
     long_description = f.read()
 
 setup(
   name = 'tksheet',
   packages = ['tksheet'],
-  version = '6.0.3',
+  version = '6.0.4',
   python_requires = '>=3.6',
   license = 'MIT',
   description = 'Tkinter table / sheet widget',
   long_description = long_description,
   long_description_content_type = 'text/markdown',
   author = 'ragardner',
   author_email = 'github@ragardner.simplelogin.com',
   url = 'https://github.com/ragardner/tksheet',
-  download_url = 'https://github.com/ragardner/tksheet/archive/6.0.3.tar.gz',
+  download_url = 'https://github.com/ragardner/tksheet/archive/6.0.4.tar.gz',
   keywords = ['tkinter', 'table', 'widget', 'sheet', 'grid', 'tk'],
   install_requires = [],
   classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License'
```

### Comparing `tksheet-6.0.3/tksheet/_tksheet.py` & `tksheet-6.0.4/tksheet/_tksheet.py`

 * *Files 1% similar despite different names*

```diff
@@ -294,23 +294,23 @@
                     self.set_options(**{k: v})
         if set_all_heights_and_widths:
             self.set_all_cell_sizes_to_text()
         if startup_select is not None:
             try:
                 if startup_select[-1] == "cells":
                     self.MT.create_selected(*startup_select)
-                    self.MT.create_current(startup_select[0], startup_select[1], type_ = "cell", inside = True)
+                    self.MT.set_currently_selected(startup_select[0], startup_select[1], type_ = "cell", inside = True)
                     self.see(startup_select[0], startup_select[1])
                 elif startup_select[-1] == "rows":
                     self.MT.create_selected(startup_select[0], 0, startup_select[1], len(self.MT.col_positions) - 1, "rows")
-                    self.MT.create_current(startup_select[0], 0, type_ = "row", inside = True)
+                    self.MT.set_currently_selected(startup_select[0], 0, type_ = "row", inside = True)
                     self.see(startup_select[0], 0)
                 elif startup_select[-1] in ("cols", "columns"):
                     self.MT.create_selected(0, startup_select[0], len(self.MT.row_positions) - 1, startup_select[1], "columns")
-                    self.MT.create_current(0, startup_select[0], type_ = "column", inside = True)
+                    self.MT.set_currently_selected(0, startup_select[0], type_ = "column", inside = True)
                     self.see(0, startup_select[0])
             except:
                 pass
         self.refresh()
         if startup_focus:
             self.MT.focus_set()
             
@@ -614,16 +614,16 @@
                 if binding == "ctrl_row_select":
                     self.RI.ctrl_selection_binding_func = func
                 if binding == "ctrl_column_select":
                     self.CH.ctrl_selection_binding_func = func
                 if binding == "deselect":
                     self.MT.deselection_binding_func = func
 
-    def emit_modified_event(self, data = {}):
-        self.event_generate("<<SheetModified>>", data = data)
+    def emit_event(self, event, data = {}):
+        self.event_generate(event, data = data)
 
     def bind_event(self, sequence, func, add = None):
         widget = self
         def _substitute(*args):
             e = lambda: None 
             e.data = eval(args[0])
             e.widget = widget
@@ -1208,18 +1208,18 @@
         self.MT.deselect(r = row, c = column, cell = cell, redraw = False)
 
     # (row, column, type_) e.g. (0, 0, "column") as a named tuple
     def get_currently_selected(self):
         return self.MT.currently_selected()
 
     def set_currently_selected(self, row, column, type_ = "cell", selection_binding = True):
-        self.MT.create_current(r = row,
-                               c = column,
-                               type_ = type_,
-                               inside = True if self.MT.cell_selected(row, column) else False)
+        self.MT.set_currently_selected(r = row,
+                                       c = column,
+                                       type_ = type_,
+                                       inside = True if self.MT.cell_selected(row, column) else False)
         if selection_binding and self.MT.selection_binding_func is not None:
             self.MT.selection_binding_func(SelectCellEvent("select_cell", row, column))
 
     def get_selected_rows(self, get_cells = False, get_cells_as_rows = False, return_tuple = False):
         if return_tuple:
             return tuple(self.MT.get_selected_rows(get_cells = get_cells, get_cells_as_rows = get_cells_as_rows))
         else:
```

### Comparing `tksheet-6.0.3/tksheet/_tksheet_column_headers.py` & `tksheet-6.0.4/tksheet/_tksheet_column_headers.py`

 * *Files 0% similar despite different names*

```diff
@@ -220,14 +220,16 @@
                 if not c_selected and self.col_selection_enabled:
                     self.add_selection(c, set_as_current = True)
                     self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
                     if self.ctrl_selection_binding_func is not None:
                         self.ctrl_selection_binding_func(SelectionBoxEvent("ctrl_select_columns", (c, c + 1)))
                 elif c_selected:
                     self.dragged_col = DraggedRowColumn(dragged = c, to_move = get_seq_without_gaps_at_index(sorted(self.MT.get_selected_cols()), c))
+        elif not self.MT.ctrl_select_enabled:
+            self.b1_press(event)
                     
     def ctrl_shift_b1_press(self, event):
         self.mouseclick_outside_editor_or_dropdown_all_canvases()
         x = event.x
         c = self.MT.identify_col(x = x)
         if (self.drag_and_drop_enabled or self.col_selection_enabled) and self.MT.ctrl_select_enabled and self.rsz_h is None and self.rsz_w is None:
             if c < len(self.MT.col_positions) - 1:
@@ -247,14 +249,16 @@
                         self.add_selection(c, set_as_current = True)
                         func_event = (c, )
                     self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
                     if self.ctrl_selection_binding_func is not None:
                         self.ctrl_selection_binding_func(SelectionBoxEvent("ctrl_select_columns", func_event))
                 elif c_selected:
                     self.dragged_col = DraggedRowColumn(dragged = c, to_move = get_seq_without_gaps_at_index(sorted(self.MT.get_selected_cols()), c))
+        elif not self.MT.ctrl_select_enabled:
+            self.shift_b1_press(event)
 
     def shift_b1_press(self, event):
         self.mouseclick_outside_editor_or_dropdown_all_canvases()
         x = event.x
         c = self.MT.identify_col(x = x)
         if (self.drag_and_drop_enabled or self.col_selection_enabled) and self.rsz_h is None and self.rsz_w is None:
             if c < len(self.MT.col_positions) - 1:
@@ -490,14 +494,16 @@
                         self.being_drawn_rect = rect
                         if self.drag_selection_binding_func is not None:
                             self.drag_selection_binding_func(SelectionBoxEvent("drag_select_columns", func_event))
                 if self.scroll_if_event_offscreen(event):
                     need_redraw = True
             if need_redraw:
                 self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = False)
+        elif not self.MT.ctrl_select_enabled:
+            self.b1_motion(event)
                 
     def drag_and_drop_motion(self, event):
         x = event.x
         wend = self.winfo_width()
         xcheck = self.xview()
         if x >= wend - 0 and len(xcheck) > 1 and xcheck[1] < 1:
             if x >= wend + 15:
@@ -640,15 +646,15 @@
                     if self.MT.undo_enabled:
                         self.MT.undo_storage.append(zlib.compress(pickle.dumps(("move_cols",
                                                                                 orig_selected,
                                                                                 new_selected))))
                     self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
                     if self.ch_extra_end_drag_drop_func is not None:
                         self.ch_extra_end_drag_drop_func(EndDragDropEvent("end_column_header_drag_drop", orig_selected, new_selected, int(c)))
-                    self.parentframe.emit_modified_event()
+                    self.parentframe.emit_event("<<SheetModified>>")
         elif self.b1_pressed_loc is not None and self.rsz_w is None and self.rsz_h is None:
             c = self.MT.identify_col(x = event.x)
             if c is not None and c < len(self.MT.col_positions) - 1 and c == self.b1_pressed_loc and self.b1_pressed_loc != self.closed_dropdown:
                 datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
                 canvasx = self.canvasx(event.x)
                 if self.event_over_dropdown(c, datacn, event, canvasx) or self.event_over_checkbox(c, datacn, event, canvasx):
                     self.open_cell(event)
@@ -676,48 +682,39 @@
                     del self.cell_options[c]['readonly']
         else:
             for c in columns_:
                 if c not in self.cell_options:
                     self.cell_options[c] = {}
                 self.cell_options[c]['readonly'] = True
 
-    def select_col(self, c, redraw = False, keep_other_selections = False):
-        if not keep_other_selections:
-            self.MT.delete_selection_rects()
-        self.MT.create_current(0, c, type_ = "column", inside = True)
-        self.MT.create_selected(0, c, len(self.MT.row_positions) - 1, c + 1, "columns")
-        if redraw:
-            self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
-        if self.selection_binding_func is not None:
-            self.selection_binding_func(SelectColumnEvent("select_column", int(c)))
-
     def toggle_select_col(self, column, add_selection = True, redraw = True, run_binding_func = True, set_as_current = True):
         if add_selection:
             if self.MT.col_selected(column):
                 self.MT.deselect(c = column, redraw = redraw)
             else:
                 self.add_selection(c = column, redraw = redraw, run_binding_func = run_binding_func, set_as_current = set_as_current)
         else:
             if self.MT.col_selected(column):
                 self.MT.deselect(c = column, redraw = redraw)
             else:
                 self.select_col(column, redraw = redraw)
+                
+    def select_col(self, c, redraw = False):
+        self.MT.delete_selection_rects()
+        self.MT.create_selected(0, c, len(self.MT.row_positions) - 1, c + 1, "columns")
+        self.MT.set_currently_selected(0, c, type_ = "column")
+        if redraw:
+            self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
+        if self.selection_binding_func is not None:
+            self.selection_binding_func(SelectColumnEvent("select_column", int(c)))
 
     def add_selection(self, c, redraw = False, run_binding_func = True, set_as_current = True):
         c = int(c)
         if set_as_current:
-            create_new_sel = False
-            current = self.MT.get_tags_of_current()
-            if current:
-                if current[0] == "Current_Outside":
-                    create_new_sel = True
-            self.MT.create_current(0, c, type_ = "column", inside = True)
-            if create_new_sel:
-                r1, c1, r2, c2 = tuple(int(e) for e in current[1].split("_") if e)
-                self.MT.create_selected(r1, c1, r2, c2, current[2] + "s")
+            self.MT.set_currently_selected(0, c, type_ = "column")
         self.MT.create_selected(0, c, len(self.MT.row_positions) - 1, c + 1, "columns")
         if redraw:
             self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
         if self.selection_binding_func is not None and run_binding_func:
             self.selection_binding_func(("select_column", int(c)))
             
     def get_cell_dimensions(self, datacn):
@@ -773,15 +770,15 @@
                 for datacn in iterable:
                     txt = self.MT.get_valid_cell_data_as_str(datarn, datacn, get_displayed = True)
                     if txt:
                         qconf(qtxtm, text = txt)
                         b = qbbox(qtxtm)
                         h = b[3] - b[1] + 5
                     else:
-                        h = self.default_header_height
+                        h = self.MT.default_header_height
                     if h < self.MT.min_header_height:
                         h = int(self.MT.min_header_height)
                     elif h > self.MT.max_header_height:
                         h = int(self.MT.max_header_height)
                     if h > new_height:
                         new_height = h
         space_bot = self.MT.get_space_bot(0)
@@ -882,25 +879,25 @@
                     del self.cell_options[c]['align']
         else:
             for c in cols:
                 if c not in self.cell_options:
                     self.cell_options[c] = {}
                 self.cell_options[c]['align'] = align
 
-    def redraw_highlight_get_text_fg(self, fc, sc, c, c_2, c_3, selected_cols, selected_rows, actual_selected_cols, datacn):
+    def redraw_highlight_get_text_fg(self, fc, sc, c, c_2, c_3, selections, datacn):
         redrawn = False
         kwargs = self.get_cell_kwargs(datacn, key = 'highlight')
         if kwargs:
             if kwargs[0] is not None:
                 c_1 = kwargs[0] if kwargs[0].startswith("#") else Color_Map_[kwargs[0]]
-            if c in actual_selected_cols:
+            if 'columns' in selections and c in selections['columns']:
                 tf = self.header_selected_columns_fg if kwargs[1] is None or self.MT.display_selected_fg_over_highlights else kwargs[1]
                 if kwargs[0] is not None:
                     fill = f"#{int((int(c_1[1:3], 16) + int(c_3[1:3], 16)) / 2):02X}" + f"{int((int(c_1[3:5], 16) + int(c_3[3:5], 16)) / 2):02X}" + f"{int((int(c_1[5:], 16) + int(c_3[5:], 16)) / 2):02X}"
-            elif (c in selected_cols or selected_rows):
+            elif 'cells' in selections and c in selections['cells']:
                 tf = self.header_selected_cells_fg if kwargs[1] is None or self.MT.display_selected_fg_over_highlights else kwargs[1]
                 if kwargs[0] is not None:
                     fill = f"#{int((int(c_1[1:3], 16) + int(c_2[1:3], 16)) / 2):02X}" + f"{int((int(c_1[3:5], 16) + int(c_2[3:5], 16)) / 2):02X}" + f"{int((int(c_1[5:], 16) + int(c_2[5:], 16)) / 2):02X}"
             else:
                 tf = self.header_fg if kwargs[1] is None else kwargs[1]
                 if kwargs[0] is not None:
                     fill = kwargs[0]
@@ -909,17 +906,17 @@
                                                 0,
                                                 sc,
                                                 self.current_height - 1,
                                                 fill = fill,
                                                 outline = self.header_fg if self.get_cell_kwargs(datacn, key = 'dropdown') and self.MT.show_dropdown_borders else "",
                                                 tag = "hi")
         elif not kwargs:
-            if c in actual_selected_cols:
+            if 'columns' in selections and c in selections['columns']:
                 tf = self.header_selected_columns_fg
-            elif c in selected_cols or selected_rows:
+            elif 'cells' in selections and c in selections['cells']:
                 tf = self.header_selected_cells_fg
             else:
                 tf = self.header_fg
         return tf, redrawn
             
     def redraw_highlight(self, x1, y1, x2, y2, fill, outline, tag):
         config = (fill, outline)
@@ -1038,15 +1035,15 @@
                 else:
                     self.itemconfig(t, fill = fill, outline = outline, tag = tag, state = "normal")
                 self.lift(t)
             else:
                 t = self.create_polygon(points, fill = fill, outline = outline, tag = tag, smooth = True)
             self.disp_checkbox[t] = True
 
-    def redraw_grid_and_text(self, last_col_line_pos, scrollpos_left, x_stop, start_col, end_col, scrollpos_right, selected_cols, selected_rows, actual_selected_cols, col_pos_exists):
+    def redraw_grid_and_text(self, last_col_line_pos, scrollpos_left, x_stop, start_col, end_col, scrollpos_right, col_pos_exists):
         try:
             self.configure(scrollregion = (0,
                                            0,
                                            last_col_line_pos + self.MT.empty_horizontal,
                                            self.current_height))
         except:
             return
@@ -1092,20 +1089,21 @@
                                    self.MT.col_positions[c + 1] if len(self.MT.col_positions) - 1 > c else draw_x, -1])
                 if points:
                     self.redraw_gridline(points = points, fill = self.header_grid_fg, width = 1, tag = "v")
         top = self.canvasy(0)
         c_2 = self.header_selected_cells_bg if self.header_selected_cells_bg.startswith("#") else Color_Map_[self.header_selected_cells_bg]
         c_3 = self.header_selected_columns_bg if self.header_selected_columns_bg.startswith("#") else Color_Map_[self.header_selected_columns_bg]
         font = self.MT.header_font
+        selections = self.get_redraw_selections(start_col, end_col)
         for c in range(start_col, end_col - 1):
             draw_y = self.MT.header_fl_ins
             cleftgridln = self.MT.col_positions[c]
             crightgridln = self.MT.col_positions[c + 1]
             datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
-            fill, dd_drawn = self.redraw_highlight_get_text_fg(cleftgridln, crightgridln, c, c_2, c_3, selected_cols, selected_rows, actual_selected_cols, datacn)
+            fill, dd_drawn = self.redraw_highlight_get_text_fg(cleftgridln, crightgridln, c, c_2, c_3, selections, datacn)
 
             if datacn in self.cell_options and 'align' in self.cell_options[datacn]:
                 align = self.cell_options[datacn]['align']
             else:
                 align = self.align
             
             kwargs = self.get_cell_kwargs(datacn, key = 'dropdown')
@@ -1183,23 +1181,25 @@
                             iid, showing = self.hidd_text[k].pop()
                             cc1, cc2 = self.coords(iid)
                             if (int(cc1) == int(draw_x) and
                                 int(cc2) == int(draw_y)):
                                 option = 0 if showing else 2
                             else:
                                 option = 1 if showing else 3
+                            self.tag_raise(iid)
                         elif self.hidd_text:
                             k = next(iter(self.hidd_text))
                             iid, showing = self.hidd_text[k].pop()
                             cc1, cc2 = self.coords(iid)
                             if (int(cc1) == int(draw_x) and
                                 int(cc2) == int(draw_y)):
                                 option = 2 if showing else 3
                             else:
                                 option = 3
+                            self.tag_raise(iid)
                         else:
                             iid, showing, option = self.create_text(draw_x, draw_y, text = txt, fill = fill, font = font, anchor = align, tag = "t"), 1, 4
                         if option in (1, 3):
                             self.coords(iid, draw_x, draw_y)
                         if option in (2, 3):
                             if showing:
                                 self.itemconfig(iid, text = txt, fill = fill, font = font, anchor = align)
@@ -1239,15 +1239,14 @@
                                 self.coords(iid, draw_x, draw_y)
                             self.disp_text[config._replace(txt = txt)].add(DrawnItem(iid = iid, showing = True))
                         else:
                             self.disp_text[config].add(DrawnItem(iid = iid, showing = True))
                     draw_y += self.MT.header_xtra_lines_increment
                     if draw_y - 1 > self.current_height:
                         break
-        self.tag_raise("t")
         for cfg, set_ in self.hidd_text.items():
             for namedtup in tuple(set_):
                 if namedtup.showing:
                     self.itemconfig(namedtup.iid, state = "hidden")
                     self.hidd_text[cfg].discard(namedtup)
                     self.hidd_text[cfg].add(namedtup._replace(showing = False))
         for cfg, set_ in self.hidd_high.items():
@@ -1265,14 +1264,26 @@
                 self.itemconfig(t, state = "hidden")
                 self.hidd_dropdown[t] = False
         for t, sh in self.hidd_checkbox.items():
             if sh:
                 self.itemconfig(t, state = "hidden")
                 self.hidd_checkbox[t] = False
                 
+    def get_redraw_selections(self, startc, endc):
+        d = defaultdict(list)
+        for item in chain(self.find_withtag("cells"), self.find_withtag("columns")):
+            tags = self.gettags(item)
+            d[tags[0]].append(tuple(int(e) for e in tags[1].split("_") if e))
+        d2 = {}
+        if 'cells' in d:
+            d2['cells'] = {c for c in range(startc, endc) for r1, c1, r2, c2 in d['cells'] if c1 <= c and c2 > c}
+        if 'columns' in d:
+            d2['columns'] = {c for c in range(startc, endc) for r1, c1, r2, c2 in d['columns'] if c1 <= c and c2 > c}
+        return d2
+                
     def open_cell(self, event = None, ignore_existing_editor = False):
         if not self.MT.anything_selected()  or (not ignore_existing_editor and self.text_editor_id is not None):
             return
         currently_selected = self.MT.currently_selected()
         if not currently_selected:
             return
         x1 = int(currently_selected[1])
@@ -1339,15 +1350,14 @@
             else:
                 text = text if isinstance(text, str) else f"{text}"
         text = "" if text is None else text
         if self.MT.cell_auto_resize_enabled:
             if self.height_resizing_enabled:
                 self.set_height_of_header_to_text(text)
             self.set_col_width_run_binding(c)
-        self.select_col(c = c, keep_other_selections = True)
         
         if c == self.text_editor_loc and self.text_editor is not None:
             self.text_editor.set_text(self.text_editor.get() + "" if not isinstance(text, str) else text)
             return
         if self.text_editor is not None:
             self.destroy_text_editor()
         if see:
@@ -1535,15 +1545,15 @@
                 self.set_cell_data(datacn = datacn, value = value)
         if cell_resize and self.MT.cell_auto_resize_enabled:
             if self.height_resizing_enabled:
                 self.set_height_of_header_to_text(self.get_valid_cell_data_as_str(datacn, fix = False))
             self.set_col_width_run_binding(c)
         if redraw:
             self.MT.refresh()
-        self.parentframe.emit_modified_event()
+        self.parentframe.emit_event("<<SheetModified>>")
     
     def set_cell_data(self, datacn = None, value = ""):
         if isinstance(self.MT._headers, int):
             self.MT.set_cell_data(datarn = self.MT._headers, datacn = datacn, value = value)
         else:
             self.fix_header(datacn)
             if self.get_cell_kwargs(datacn, key = 'checkbox'):
```

### Comparing `tksheet-6.0.3/tksheet/_tksheet_formatters.py` & `tksheet-6.0.4/tksheet/_tksheet_formatters.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.0.3/tksheet/_tksheet_main_table.py` & `tksheet-6.0.4/tksheet/_tksheet_main_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -387,31 +387,28 @@
                 self.itemconfig(t, state = "hidden")
                 self.hidd_ctrl_outline[t] = False
 
     def get_ctrl_x_c_boxes(self):
         currently_selected = self.currently_selected()
         boxes = {}
         if currently_selected.type_ in ("cell", "column"):
-            for item in chain(self.find_withtag("CellSelectFill"), self.find_withtag("Current_Outside"), self.find_withtag("ColSelectFill")):
+            for item in chain(self.find_withtag("cells"), self.find_withtag("columns")):
                 alltags = self.gettags(item)
-                if alltags[0] == "CellSelectFill" or alltags[0] == "Current_Outside":
-                    boxes[tuple(int(e) for e in alltags[1].split("_") if e)] = "cells"
-                elif alltags[0] == "ColSelectFill":
-                    boxes[tuple(int(e) for e in alltags[1].split("_") if e)] = "columns"
+                boxes[tuple(int(e) for e in alltags[1].split("_") if e)] = alltags[0]
             maxrows = 0
             for r1, c1, r2, c2 in boxes:
                 if r2 - r1 > maxrows:
                     maxrows = r2 - r1
             curr_box = self.find_last_selected_box_with_current_from_boxes(currently_selected, boxes)
             for box in tuple(boxes):
                 if box[2] - box[0] < maxrows and box != curr_box:
                     del boxes[box]
             return boxes, maxrows
         else:
-            for item in self.find_withtag("RowSelectFill"):
+            for item in self.find_withtag("rows"):
                 boxes[tuple(int(e) for e in self.gettags(item)[1].split("_") if e)] = "rows"
             return boxes
 
     def ctrl_c(self, event = None):
         currently_selected = self.currently_selected()
         if currently_selected:
             s = io.StringIO()
@@ -538,15 +535,15 @@
         self.clipboard_append(s.getvalue())
         self.update_idletasks()
         self.refresh()
         for r1, c1, r2, c2 in boxes:
             self.show_ctrl_outline(canvas = "table", start_cell = (c1, r1), end_cell = (c2, r2))
         if self.extra_end_ctrl_x_func is not None:
             self.extra_end_ctrl_x_func(CtrlKeyEvent("end_ctrl_x", boxes, currently_selected, rows))
-        self.parentframe.emit_modified_event()
+        self.parentframe.emit_event("<<SheetModified>>")
 
     def find_last_selected_box_with_current(self, currently_selected):
         if currently_selected.type_ in ("cell", "column"):
             boxes, maxrows = self.get_ctrl_x_c_boxes()
         else:
             boxes = self.get_ctrl_x_c_boxes()
         return self.find_last_selected_box_with_current_from_boxes(currently_selected, boxes)
@@ -665,36 +662,31 @@
         if changes and self.undo_enabled:
             self.undo_storage.append(zlib.compress(pickle.dumps(("edit_cells_paste",
                                                                  undo_storage,
                                                                  {(selected_r, selected_c, selected_r + numrows, selected_c + numcols): "cells"}, # boxes
                                                                  currently_selected,
                                                                  added_rows_cols))))
         self.create_selected(selected_r, selected_c, selected_r + numrows, selected_c + numcols, "cells")
-        self.create_current(selected_r, selected_c, type_ = "cell", inside = True if numrows > 1 or numcols > 1 else False)
+        self.set_currently_selected(selected_r, selected_c, type_ = "cell")
         self.see(r = selected_r, c = selected_c, keep_yscroll = False, keep_xscroll = False, bottom_right_corner = False, check_cell_visibility = True, redraw = False)
         self.refresh()
         if self.extra_end_ctrl_v_func is not None:
             self.extra_end_ctrl_v_func(PasteEvent("end_ctrl_v", currently_selected, rows))
-        self.parentframe.emit_modified_event()
+        self.parentframe.emit_event("<<SheetModified>>")
 
     def delete_key(self, event = None):
         if not self.anything_selected():
             return
         currently_selected = self.currently_selected()
         undo_storage = {}
         boxes = {}
-        for item in chain(self.find_withtag("CellSelectFill"), self.find_withtag("RowSelectFill"), self.find_withtag("ColSelectFill"), self.find_withtag("Current_Outside")):
+        for item in chain(self.find_withtag("cells"), self.find_withtag("rows"), self.find_withtag("columns")):
             alltags = self.gettags(item)
             box = tuple(int(e) for e in alltags[1].split("_") if e)
-            if alltags[0] in ("CellSelectFill", "Current_Outside"):
-                boxes[box] = "cells"
-            elif alltags[0] == "ColSelectFill":
-                boxes[box] = "columns"
-            elif alltags[0] == "RowSelectFill":
-                boxes[box] = "rows"
+            boxes[box] = alltags[0]
         if self.extra_begin_delete_key_func is not None:
             try:
                 self.extra_begin_delete_key_func(CtrlKeyEvent("begin_delete_key", boxes, currently_selected, tuple()))
             except:
                 return
         changes = 0
         for r1, c1, r2, c2 in boxes:
@@ -708,15 +700,15 @@
                         self.set_cell_data(datarn, datacn, "")
                         changes += 1
         if self.extra_end_delete_key_func is not None:
             self.extra_end_delete_key_func(CtrlKeyEvent("end_delete_key", boxes, currently_selected, undo_storage))
         if changes and self.undo_enabled:
             self.undo_storage.append(zlib.compress(pickle.dumps(("edit_cells", undo_storage, boxes, currently_selected))))
         self.refresh()
-        self.parentframe.emit_modified_event()
+        self.parentframe.emit_event("<<SheetModified>>")
             
     def move_columns_adjust_options_dict(self, col, to_move_min, num_cols, move_data = True, create_selections = True, index_type = "displayed"):
         c = int(col)
         to_move_max = to_move_min + num_cols
         to_del = to_move_max + num_cols
         orig_selected = list(range(to_move_min, to_move_min + num_cols))
         if index_type == "displayed":
@@ -739,15 +731,15 @@
                 if create_selections and index_type == "displayed":
                     self.create_selected(0, c, len(self.row_positions) - 1, c + num_cols, "columns")
             else:
                 new_selected = tuple(range(c + 1 - num_cols, c + 1))
                 if create_selections and index_type == "displayed":
                     self.create_selected(0, c + 1 - num_cols, len(self.row_positions) - 1, c + 1, "columns")
         if create_selections and index_type == "displayed":
-            self.create_current(0, int(new_selected[0]), type_ = "column", inside = True)
+            self.set_currently_selected(0, int(new_selected[0]), type_ = "column")
         newcolsdct = {t1: t2 for t1, t2 in zip(orig_selected, new_selected)}
         if self.all_columns_displayed or index_type != "displayed":
             dispset = {}
             if to_move_min > c:
                 self.CH.cell_options = {
                     newcolsdct[k] if k in newcolsdct else
                     k + num_cols if k < to_move_min and k >= c else
@@ -884,15 +876,15 @@
                 if create_selections and index_type == "displayed":
                     self.create_selected(r, 0, r + num_rows, len(self.col_positions) - 1, "rows")
             else:
                 new_selected = tuple(range(r + 1 - num_rows, r + 1))
                 if create_selections and index_type == "displayed":
                     self.create_selected(r + 1 - num_rows, 0, r + 1, len(self.col_positions) - 1, "rows")
         if create_selections and index_type == "displayed":
-            self.create_current(int(new_selected[0]), 0, type_ = "row", inside = True)
+            self.set_currently_selected(int(new_selected[0]), 0, type_ = "row")
         newrowsdct = {t1: t2 for t1, t2 in zip(orig_selected, new_selected)}
         if self.all_rows_displayed or index_type != "displayed":
             dispset = {}
             if to_move_min > r:
                 self.RI.cell_options = {
                     newrowsdct[k] if k in newrowsdct else
                     k + num_rows if k < to_move_min and k >= r else
@@ -1010,21 +1002,21 @@
             except:
                 return
         self.undo_storage.pop()
         if undo_storage[0] in ("edit_header", ):
             for c, v in undo_storage[1].items():
                 self._headers[c] = v
             self.reselect_from_get_boxes(undo_storage[2])
-            self.create_current(0, undo_storage[3][1], type_ = "column", inside = True)
+            self.set_currently_selected(0, undo_storage[3][1], type_ = "column")
             
         if undo_storage[0] in ("edit_index", ):
             for r, v in undo_storage[1].items():
                 self._row_index[r] = v
             self.reselect_from_get_boxes(undo_storage[2])
-            self.create_current(0, undo_storage[3][1], type_ = "row", inside = True)
+            self.set_currently_selected(0, undo_storage[3][1], type_ = "row")
                         
         if undo_storage[0] in ("edit_cells", "edit_cells_paste"):
             for (datarn, datacn), v in undo_storage[1].items():
                 self.set_cell_data(datarn, datacn, v)
             start_row = float("inf")
             start_col = float("inf")
             if undo_storage[0] == "edit_cells_paste" and self.expand_sheet_if_paste_too_big:
@@ -1038,20 +1030,19 @@
                     self.del_col_positions(len(self.col_positions) - 1 - quick_added_cols, quick_added_cols)
                     for rn in range(len(self.data)):
                         self.data[rn][:] = self.data[rn][:-quick_added_cols]
                     if not self.all_columns_displayed:
                         self.displayed_columns[:] = self.displayed_columns[:-quick_added_cols]
             self.reselect_from_get_boxes(undo_storage[2])
             if undo_storage[3]:
-                self.create_current(undo_storage[3].row,
-                                    undo_storage[3].column, 
-                                    type_ = undo_storage[3].type_, 
-                                    inside = True if self.cell_selected(undo_storage[3].row, undo_storage[3].column) else False)
+                self.set_currently_selected(undo_storage[3].row,
+                                            undo_storage[3].column, 
+                                            type_ = undo_storage[3].type_)
             elif start_row < len(self.row_positions) - 1 and start_col < len(self.col_positions) - 1:
-                self.create_current(start_row, start_col, type_ = "cell", inside = True if self.cell_selected(start_row, start_col) else False)
+                self.set_currently_selected(start_row, start_col, type_ = "cell")
             if start_row < len(self.row_positions) - 1 and start_col < len(self.col_positions) - 1:
                 self.see(r = start_row, c = start_col, keep_yscroll = False, keep_xscroll = False, bottom_right_corner = False, check_cell_visibility = True, redraw = False)
         
         elif undo_storage[0] == "move_cols":
             c = undo_storage[1][0]
             to_move_min = undo_storage[2][0]
             totalcols = len(undo_storage[2])
@@ -1072,27 +1063,22 @@
             self.displayed_rows = undo_storage[1]['displayed_rows']
             self.data[undo_storage[1]['data_row_num']:undo_storage[1]['data_row_num'] + undo_storage[1]['numrows']] = []
             try:
                 self._row_index[undo_storage[1]['data_row_num']:undo_storage[1]['data_row_num'] + undo_storage[1]['numrows']] = []
             except:
                 pass
             self.del_row_positions(undo_storage[1]['sheet_row_num'],
-                                    undo_storage[1]['numrows'],
-                                    deselect_all = False)
-            for r in range(undo_storage[1]['sheet_row_num'],
-                            undo_storage[1]['sheet_row_num'] + undo_storage[1]['numrows']):
-                if r in self.row_options:
-                    del self.row_options[r]
-                if r in self.RI.cell_options:
-                    del self.RI.cell_options[r]
+                                   undo_storage[1]['numrows'],
+                                   deselect_all = False)
+            to_del = set(range(undo_storage[1]['sheet_row_num'], undo_storage[1]['sheet_row_num'] + undo_storage[1]['numrows']))
             numrows = undo_storage[1]['numrows']
             idx = undo_storage[1]['sheet_row_num'] + undo_storage[1]['numrows']
-            self.cell_options = {(rn if rn < idx else rn - numrows, cn): t2 for (rn, cn), t2 in self.cell_options.items()}
-            self.row_options = {rn if rn < idx else rn - numrows: t for rn, t in self.row_options.items()}
-            self.RI.cell_options = {rn if rn < idx else rn - numrows: t for rn, t in self.RI.cell_options.items()}
+            self.cell_options = {(rn if rn < idx else rn - numrows, cn): t2 for (rn, cn), t2 in self.cell_options.items() if rn not in to_del}
+            self.row_options = {rn if rn < idx else rn - numrows: t for rn, t in self.row_options.items() if rn not in to_del}
+            self.RI.cell_options = {rn if rn < idx else rn - numrows: t for rn, t in self.RI.cell_options.items() if rn not in to_del}
             if len(self.row_positions) > 1:
                 start_row = undo_storage[1]['sheet_row_num'] if undo_storage[1]['sheet_row_num'] < len(self.row_positions) - 1 else undo_storage[1]['sheet_row_num'] - 1
                 self.RI.select_row(start_row)
                 self.see(r = start_row, c = 0, keep_yscroll = False, keep_xscroll = False, bottom_right_corner = False, check_cell_visibility = True, redraw = False)
                 
         elif undo_storage[0] == "insert_cols":
             self.displayed_columns = undo_storage[1]['displayed_columns']
@@ -1101,27 +1087,22 @@
             for rn in range(len(self.data)):
                 self.data[rn][qx:qx + qnum] = []
             try:
                 self._headers[qx:qx + qnum] = []
             except:
                 pass
             self.del_col_positions(undo_storage[1]['sheet_col_num'],
-                                    undo_storage[1]['numcols'],
-                                    deselect_all = False)
-            for c in range(undo_storage[1]['sheet_col_num'],
-                           undo_storage[1]['sheet_col_num'] + undo_storage[1]['numcols']):
-                if c in self.col_options:
-                    del self.col_options[c]
-                if c in self.CH.cell_options:
-                    del self.CH.cell_options[c]
+                                   undo_storage[1]['numcols'],
+                                   deselect_all = False)
+            to_del = set(range(undo_storage[1]['sheet_col_num'], undo_storage[1]['sheet_col_num'] + undo_storage[1]['numcols']))
             numcols = undo_storage[1]['numcols']
             idx = undo_storage[1]['sheet_col_num'] + undo_storage[1]['numcols']
-            self.cell_options = {(rn, cn if cn < idx else cn - numcols): t2 for (rn, cn), t2 in self.cell_options.items()}
-            self.col_options = {cn if cn < idx else cn - numcols: t for cn, t in self.col_options.items()}
-            self.CH.cell_options = {cn if cn < idx else cn - numcols: t for cn, t in self.CH.cell_options.items()}
+            self.cell_options = {(rn, cn if cn < idx else cn - numcols): t2 for (rn, cn), t2 in self.cell_options.items() if cn not in to_del}
+            self.col_options = {cn if cn < idx else cn - numcols: t for cn, t in self.col_options.items() if cn not in to_del}
+            self.CH.cell_options = {cn if cn < idx else cn - numcols: t for cn, t in self.CH.cell_options.items() if cn not in to_del}
             if len(self.col_positions) > 1:
                 start_col = undo_storage[1]['sheet_col_num'] if undo_storage[1]['sheet_col_num'] < len(self.col_positions) - 1 else undo_storage[1]['sheet_col_num'] - 1
                 self.CH.select_col(start_col)
                 self.see(r = 0, c = start_col, keep_yscroll = False, keep_xscroll = False, bottom_right_corner = False, check_cell_visibility = True, redraw = False)
                 
         elif undo_storage[0] == "delete_rows":
             self.displayed_rows = undo_storage[1]['displayed_rows']
@@ -1157,15 +1138,15 @@
                     self._headers.insert(cn, v)
                 except:
                     continue
             self.reselect_from_get_boxes(undo_storage[1]['selection_boxes'])
         self.refresh()
         if self.extra_end_ctrl_z_func is not None:
             self.extra_end_ctrl_z_func(UndoEvent("end_ctrl_z", undo_storage[0], undo_storage))
-        self.parentframe.emit_modified_event()
+        self.parentframe.emit_event("<<SheetModified>>")
 
     def bind_arrowkeys(self, keys: dict = {}):
         for canvas in (self, self.parentframe, self.CH, self.RI, self.TL):
             for k, func in keys.items():
                 canvas.bind(f"<{arrowkey_bindings_helper[k.lower()]}>", func)
 
     def unbind_arrowkeys(self, keys: dict = {}):
@@ -1263,56 +1244,36 @@
         return False
 
     def select_all(self, redraw = True, run_binding_func = True):
         currently_selected = self.currently_selected()
         self.deselect("all")
         if len(self.row_positions) > 1 and len(self.col_positions) > 1:
             if currently_selected:
-                self.create_current(currently_selected.row, currently_selected.column, type_ = "cell", inside = True)
+                self.set_currently_selected(currently_selected.row, currently_selected.column, type_ = "cell")
             else:
-                self.create_current(0, 0, type_ = "cell", inside = True)
+                self.set_currently_selected(0, 0, type_ = "cell")
             self.create_selected(0, 0, len(self.row_positions) - 1, len(self.col_positions) - 1)
             if redraw:
                 self.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
             if self.select_all_binding_func is not None and run_binding_func:
                 self.select_all_binding_func(SelectionBoxEvent("select_all_cells", (0, 0, len(self.row_positions) - 1, len(self.col_positions) - 1)))
 
-    def select_cell(self, r, c, redraw = False, keep_other_selections = False):
-        r = int(r)
-        c = int(c)
-        if keep_other_selections:
-            inside = self.cell_selected(r, c)
-        else:
-            inside = False
-            self.delete_selection_rects()
-        self.create_current(r, c, type_ = "cell", inside = inside)
+    def select_cell(self, r, c, redraw = False):
+        self.delete_selection_rects()
+        self.create_selected(r, c, r + 1, c + 1, state = "hidden")
+        self.set_currently_selected(r, c, type_ = "cell")
         if redraw:
             self.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
         if self.selection_binding_func is not None:
             self.selection_binding_func(SelectCellEvent("select_cell", r, c))
 
     def add_selection(self, r, c, redraw = False, run_binding_func = True, set_as_current = False):
-        r = int(r)
-        c = int(c)
+        self.create_selected(r, c, r + 1, c + 1, state = "hidden")
         if set_as_current:
-            items = self.find_withtag("Current_Outside")
-            if items:
-                alltags = self.gettags(items[0])
-                if alltags[2] == "cell":
-                    r1, c1, r2, c2 = tuple(int(e) for e in alltags[1].split("_") if e)
-                    add_sel = (r1, c1)
-                else:
-                    add_sel = tuple()
-            else:
-                add_sel = tuple()
-            self.create_current(r, c, type_ = "cell", inside = self.cell_selected(r, c))
-            if add_sel:
-                self.add_selection(add_sel[0], add_sel[1], redraw = False, run_binding_func = False, set_as_current = False)
-        else:
-            self.create_selected(r, c, r + 1, c + 1)
+            self.set_currently_selected(r, c, type_ = "cell")
         if redraw:
             self.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
         if self.selection_binding_func is not None and run_binding_func:
             self.selection_binding_func(SelectCellEvent("select_cell", r, c))
 
     def toggle_select_cell(self, row, column, add_selection = True, redraw = True, run_binding_func = True, set_as_current = True):
         if add_selection:
@@ -1417,48 +1378,48 @@
 
     def deselect(self, r = None, c = None, cell = None, redraw = True):
         deselected = tuple()
         deleted_boxes = {}
         if r == "all":
             deselected = ("deselect_all", self.delete_selection_rects())
         elif r == "allrows":
-            for item in self.find_withtag("RowSelectFill"):
+            for item in self.find_withtag("rows"):
                 alltags = self.gettags(item)
                 if alltags:
                     r1, c1, r2, c2 = tuple(int(e) for e in alltags[1].split("_") if e)
                     deleted_boxes[r1, c1, r2, c2] = "rows"
                     self.delete(alltags[1])
                     self.RI.delete(alltags[1])
                     self.CH.delete(alltags[1])
             current = self.currently_selected()
             if current and current.type_ == "row":
                 deleted_boxes[tuple(int(e) for e in self.get_tags_of_current()[1].split("_") if e)] = "cell"
                 self.delete_current()
             deselected = ("deselect_all_rows", deleted_boxes)
         elif r == "allcols":
-            for item in self.find_withtag("ColSelectFill"):
+            for item in self.find_withtag("columns"):
                 alltags = self.gettags(item)
                 if alltags:
                     r1, c1, r2, c2 = tuple(int(e) for e in alltags[1].split("_") if e)
                     deleted_boxes[r1, c1, r2, c2] = "columns"
                     self.delete(alltags[1])
                     self.RI.delete(alltags[1])
                     self.CH.delete(alltags[1])
             current = self.currently_selected()
             if current and current.type_ == "column":
                 deleted_boxes[tuple(int(e) for e in self.get_tags_of_current()[1].split("_") if e)] = "cell"
                 self.delete_current()
             deselected = ("deselect_all_cols", deleted_boxes)
         elif r is not None and c is None and cell is None:
-            current = self.find_withtag("Current_Inside") + self.find_withtag("Current_Outside")
+            current = self.find_withtag("currently")
             current_tags = self.gettags(current[0]) if current else tuple()
             if current:
                 curr_r1, curr_c1, curr_r2, curr_c2 = tuple(int(e) for e in current_tags[1].split("_") if e)
             reset_current = False
-            for item in self.find_withtag("RowSelectFill"):
+            for item in self.find_withtag("rows"):
                 alltags = self.gettags(item)
                 if alltags:
                     r1, c1, r2, c2 = tuple(int(e) for e in alltags[1].split("_") if e)
                     if r >= r1 and r < r2:
                         self.delete(f"{r1}_{c1}_{r2}_{c2}")
                         self.RI.delete(f"{r1}_{c1}_{r2}_{c2}")
                         self.CH.delete(f"{r1}_{c1}_{r2}_{c2}")
@@ -1467,20 +1428,20 @@
                         deleted_boxes[curr_r1, curr_c1, curr_r2, curr_c2] = "cell"
                     deleted_boxes[r1, c1, r2, c2] = "rows"
             if reset_current:
                 self.delete_current()
                 self.set_current_to_last()
             deselected = ("deselect_row", deleted_boxes)
         elif c is not None and r is None and cell is None:
-            current = self.find_withtag("Current_Inside") + self.find_withtag("Current_Outside")
+            current = self.find_withtag("currently")
             current_tags = self.gettags(current[0]) if current else tuple()
             if current:
                 curr_r1, curr_c1, curr_r2, curr_c2 = tuple(int(e) for e in current_tags[1].split("_") if e)
             reset_current = False
-            for item in self.find_withtag("ColSelectFill"):
+            for item in self.find_withtag("columns"):
                 alltags = self.gettags(item)
                 if alltags:
                     r1, c1, r2, c2 = tuple(int(e) for e in alltags[1].split("_") if e)
                     if c >= c1 and c < c2:
                         self.delete(f"{r1}_{c1}_{r2}_{c2}")
                         self.RI.delete(f"{r1}_{c1}_{r2}_{c2}")
                         self.CH.delete(f"{r1}_{c1}_{r2}_{c2}")
@@ -1492,19 +1453,18 @@
                 self.delete_current()
                 self.set_current_to_last()
             deselected = ("deselect_column", deleted_boxes)
         elif (r is not None and c is not None and cell is None) or cell is not None:
             set_curr = False
             if cell is not None:
                 r, c = cell[0], cell[1]
-            for item in chain(self.find_withtag("CellSelectFill"),
-                              self.find_withtag("RowSelectFill"),
-                              self.find_withtag("ColSelectFill"),
-                              self.find_withtag("Current_Outside"),
-                              self.find_withtag("Current_Inside")):
+            for item in chain(self.find_withtag("cells"),
+                              self.find_withtag("rows"),
+                              self.find_withtag("columns"),
+                              self.find_withtag("currently")):
                 alltags = self.gettags(item)
                 if alltags:
                     r1, c1, r2, c2 = tuple(int(e) for e in alltags[1].split("_") if e)
                     if (r >= r1 and
                         c >= c1 and
                         r < r2 and
                         c < c2):
@@ -2130,15 +2090,14 @@
             self.edit_bindings(True)
             self.rc_delete_column_enabled = True
             self.rc_delete_row_enabled = True
             self.rc_insert_column_enabled = True
             self.rc_insert_row_enabled = True
             self.rc_popup_menus_enabled = True
             self.rc_select_enabled = True
-            self.ctrl_select_enabled = True
             self.TL.rh_state()
             self.TL.rw_state()
         elif binding in ("single", "single_selection_mode", "single_select"):
             self.single_selection_enabled = True
             self.toggle_selection_enabled = False
         elif binding in ("toggle", "toggle_selection_mode", "toggle_select"):
             self.toggle_selection_enabled = True
@@ -2465,14 +2424,16 @@
             if rowsel < len(self.row_positions) - 1 and colsel < len(self.col_positions) - 1:
                 currently_selected = self.currently_selected()
                 if not currently_selected or currently_selected.row != rowsel or currently_selected.column != colsel:
                     self.add_selection(rowsel, colsel, set_as_current = True)
                 self.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True, redraw_table = True)
                 if self.ctrl_selection_binding_func is not None:
                     self.ctrl_selection_binding_func(SelectionBoxEvent("ctrl_select_cells", (rowsel, colsel, rowsel + 1, colsel + 1)))
+        elif not self.ctrl_select_enabled:
+            self.b1_press(event)
                     
     def ctrl_shift_b1_press(self, event = None):
         self.mouseclick_outside_editor_or_dropdown_all_canvases()
         self.focus_set()
         if self.ctrl_select_enabled and self.drag_selection_enabled and all(v is None for v in (self.RI.rsz_h, self.RI.rsz_w, self.CH.rsz_h, self.CH.rsz_w)):
             self.b1_pressed_loc = None
             rowsel = int(self.identify_row(y = event.y))
@@ -2493,14 +2454,16 @@
                     self.create_selected(*last_selected)
                 else:
                     self.add_selection(rowsel, colsel, set_as_current = True)
                     last_selected = (rowsel, colsel, rowsel + 1, colsel + 1)
                 self.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True, redraw_table = True)
                 if self.shift_selection_binding_func is not None:
                     self.shift_selection_binding_func(SelectionBoxEvent("shift_select_cells", last_selected))
+        elif not self.ctrl_select_enabled:
+            self.shift_b1_press(event)
 
     def shift_b1_press(self, event = None):
         self.mouseclick_outside_editor_or_dropdown_all_canvases()
         self.focus_set()
         if self.drag_selection_enabled and all(v is None for v in (self.RI.rsz_h, self.RI.rsz_w, self.CH.rsz_h, self.CH.rsz_w)):
             self.b1_pressed_loc = None
             rowsel = int(self.identify_row(y = event.y))
@@ -2515,18 +2478,18 @@
                         self.create_selected(min_r, min_c, rowsel + 1, colsel + 1)
                     elif rowsel >= min_r and min_c >= colsel:
                         self.create_selected(min_r, colsel, rowsel + 1, min_c + 1)
                     elif min_r >= rowsel and colsel >= min_c:
                         self.create_selected(rowsel, min_c, min_r + 1, colsel + 1)
                     elif min_r >= rowsel and min_c >= colsel:
                         self.create_selected(rowsel, colsel, min_r + 1, min_c + 1)
-                    last_selected = tuple(int(e) for e in self.gettags(self.find_withtag("CellSelectFill"))[1].split("_") if e)
+                    last_selected = tuple(int(e) for e in self.gettags(self.find_withtag("cells"))[1].split("_") if e)
                 else:
                     self.select_cell(rowsel, colsel, redraw = False)
-                    last_selected = tuple(int(e) for e in self.gettags(self.find_withtag("Current_Outside"))[1].split("_") if e)
+                    last_selected = tuple(int(e) for e in self.gettags(self.find_withtag("currently"))[1].split("_") if e)
                 self.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True, redraw_table = True)
                 if self.shift_selection_binding_func is not None:
                     self.shift_selection_binding_func(SelectionBoxEvent("shift_select_cells", last_selected))
                     
     def get_b1_motion_rect(self, start_row, start_col, end_row, end_col):
         if (end_row >= start_row and 
             end_col >= start_col and
@@ -2620,14 +2583,16 @@
                     if self.drag_selection_binding_func is not None:
                         self.drag_selection_binding_func(SelectionBoxEvent("drag_select_cells", rect[:-1]))
                     need_redraw = True
             if self.scroll_if_event_offscreen(event):
                 need_redraw = True
             if need_redraw:
                 self.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True, redraw_table = True)
+        elif not self.ctrl_select_enabled:
+            self.b1_motion(event)
 
     def b1_release(self, event = None):
         if self.being_drawn_rect is not None and (self.being_drawn_rect[2] - self.being_drawn_rect[0] > 1 or self.being_drawn_rect[3] - self.being_drawn_rect[1] > 1):
             self.delete_selected(*self.being_drawn_rect)
             to_sel = tuple(self.being_drawn_rect)
             self.being_drawn_rect = None
             self.create_selected(*to_sel)
@@ -3290,24 +3255,24 @@
                                      deselect_all = False)
             self.data.append(self.get_empty_row_seq(0, end = data_ins_col + numcols, start = data_ins_col, c_ops = False))
         else:
             end = data_ins_col + numcols
             for rn in range(len(self.data)):
                 self.data[rn][data_ins_col:data_ins_col] = self.get_empty_row_seq(rn, end, data_ins_col, c_ops = False)
         self.create_selected(0, displayed_ins_col, len(self.row_positions) - 1, displayed_ins_col + numcols, "columns")
-        self.create_current(0, displayed_ins_col, "column", inside = True)
+        self.set_currently_selected(0, displayed_ins_col, "column")
         if self.undo_enabled:
             self.undo_storage.append(zlib.compress(pickle.dumps(("insert_cols", {"data_col_num": data_ins_col,
                                                                                  "displayed_columns": saved_displayed_columns,
                                                                                  "sheet_col_num": displayed_ins_col,
                                                                                  "numcols": numcols}))))
         self.refresh()
         if self.extra_end_insert_cols_rc_func is not None:
             self.extra_end_insert_cols_rc_func(InsertEvent("end_insert_columns", data_ins_col, displayed_ins_col, numcols))
-        self.parentframe.emit_modified_event()
+        self.parentframe.emit_event("<<SheetModified>>")
 
     def insert_rows_rc(self, event = None):
         if self.anything_selected(exclude_columns = True, exclude_cells = True):
             selrows = self.get_selected_rows()
             numrows = len(selrows)
             displayed_ins_row = min(selrows) if event == "above" else max(selrows) + 1
             if self.all_rows_displayed:
@@ -3364,24 +3329,24 @@
                                      width = None,
                                      deselect_all = False)
             self.data.append(self.get_empty_row_seq(0, end = data_ins_row + numrows, start = data_ins_row, r_ops = False))
         else:
             total_data_cols = self.total_data_cols()
             self.data[data_ins_row:data_ins_row] = [self.get_empty_row_seq(rn, total_data_cols, r_ops = False) for rn in range(data_ins_row, data_ins_row + numrows)]
         self.create_selected(displayed_ins_row, 0, displayed_ins_row + numrows, len(self.col_positions) - 1, "rows")
-        self.create_current(displayed_ins_row, 0, "row", inside = True)
+        self.set_currently_selected(displayed_ins_row, 0, "row")
         if self.undo_enabled:
             self.undo_storage.append(zlib.compress(pickle.dumps(("insert_rows", {"data_row_num": data_ins_row,
                                                                                  "displayed_rows": saved_displayed_rows,
                                                                                  "sheet_row_num": displayed_ins_row,
                                                                                  "numrows": numrows}))))
         self.refresh()
         if self.extra_end_insert_rows_rc_func is not None:
             self.extra_end_insert_rows_rc_func(InsertEvent("end_insert_rows", data_ins_row, displayed_ins_row, numrows))
-        self.parentframe.emit_modified_event()
+        self.parentframe.emit_event("<<SheetModified>>")
 
     def del_cols_rc(self, event = None):
         seld_cols = sorted(self.get_selected_cols())
         if not seld_cols:
             return
         if self.extra_begin_del_cols_rc_func is not None:
             try:
@@ -3435,15 +3400,15 @@
         if not self.all_columns_displayed:
             self.displayed_columns = [c for c in self.displayed_columns if c not in seldset]
             for c in sorted(seldset):
                 self.displayed_columns = [dc if c > dc else dc - 1 for dc in self.displayed_columns]
         self.refresh()
         if self.extra_end_del_cols_rc_func is not None:
             self.extra_end_del_cols_rc_func(DeleteRowColumnEvent("end_delete_columns", seld_cols))
-        self.parentframe.emit_modified_event()
+        self.parentframe.emit_event("<<SheetModified>>")
 
     def del_rows_rc(self, event = None):
         seld_rows = sorted(self.get_selected_rows())
         if not seld_rows:
             return
         if self.extra_begin_del_rows_rc_func is not None:
             try:
@@ -3486,15 +3451,15 @@
         self.row_options = {rn if rn < idx else rn - numrows: t for rn, t in self.row_options.items() if rn not in seldset}
         self.RI.cell_options = {rn if rn < idx else rn - numrows: t for rn, t in self.RI.cell_options.items() if rn not in seldset}
         self.deselect("allrows", redraw = False)
         self.set_current_to_last()
         self.refresh()
         if self.extra_end_del_rows_rc_func is not None:
             self.extra_end_del_rows_rc_func(DeleteRowColumnEvent("end_delete_rows", seld_rows))
-        self.parentframe.emit_modified_event()
+        self.parentframe.emit_event("<<SheetModified>>")
 
     def move_row_position(self, idx1, idx2):
         if not len(self.row_positions) <= 2:
             if idx1 < idx2:
                 height = self.row_positions[idx1 + 1] - self.row_positions[idx1]
                 self.row_positions.insert(idx2 + 1, self.row_positions.pop(idx1 + 1))
                 for i in range(idx1 + 1, idx2 + 1):
@@ -3686,47 +3651,47 @@
     def get_visible_columns(self, x1, x2):
         start_col = bisect.bisect_left(self.col_positions, x1)
         end_col = bisect.bisect_right(self.col_positions, x2)
         if not x2 >= self.col_positions[-1]:
             end_col += 1
         return start_col, end_col
 
-    def redraw_highlight_get_text_fg(self, r, c, fc, fr, sc, sr, c_2_, c_3_, c_4_, selected_cells, actual_selected_rows, actual_selected_cols, datarn, datacn, can_width):
+    def redraw_highlight_get_text_fg(self, r, c, fc, fr, sc, sr, c_2_, c_3_, c_4_, selections, datarn, datacn, can_width):
         redrawn = False
         kwargs = self.get_cell_kwargs(datarn, datacn, key = 'highlight')
         if kwargs:
             if kwargs[0] is not None:
                 c_1 = kwargs[0] if kwargs[0].startswith("#") else Color_Map_[kwargs[0]]
-            if (r, c) in selected_cells:
+            if 'cells' in selections and (r, c) in selections['cells']:
                 tf = self.table_selected_cells_fg if kwargs[1] is None or self.display_selected_fg_over_highlights else kwargs[1]
                 if kwargs[0] is not None:
                     fill = f"#{int((int(c_1[1:3], 16) + c_2_[0]) / 2):02X}" + f"{int((int(c_1[3:5], 16) + c_2_[1]) / 2):02X}" + f"{int((int(c_1[5:], 16) + c_2_[2]) / 2):02X}"
-            elif r in actual_selected_rows:
+            elif 'rows' in selections and r in selections['rows']:
                 tf = self.table_selected_rows_fg if kwargs[1] is None or self.display_selected_fg_over_highlights else kwargs[1]
                 if kwargs[0] is not None:
                     fill = f"#{int((int(c_1[1:3], 16) + c_4_[0]) / 2):02X}" + f"{int((int(c_1[3:5], 16) + c_4_[1]) / 2):02X}" + f"{int((int(c_1[5:], 16) + c_4_[2]) / 2):02X}"
-            elif c in actual_selected_cols:
+            elif 'columns' in selections and c in selections['columns']:
                 tf = self.table_selected_columns_fg if kwargs[1] is None or self.display_selected_fg_over_highlights else kwargs[1]
                 if kwargs[0] is not None:
                     fill = f"#{int((int(c_1[1:3], 16) + c_3_[0]) / 2):02X}" + f"{int((int(c_1[3:5], 16) + c_3_[1]) / 2):02X}" + f"{int((int(c_1[5:], 16) + c_3_[2]) / 2):02X}"
             else:
                 tf = self.table_fg if kwargs[1] is None else kwargs[1]
                 if kwargs[0] is not None:
                     fill = kwargs[0]
             if kwargs[0] is not None:
                 redrawn = self.redraw_highlight(fc + 1, fr + 1, sc, sr, fill = fill, 
                                                 outline = self.table_fg if self.get_cell_kwargs(datarn, datacn, key = 'dropdown') and self.show_dropdown_borders else "", 
                                                 tag = "hi",
                                                 can_width = can_width if (len(kwargs) > 2 and kwargs[2]) else None)
         elif not kwargs:
-            if (r, c) in selected_cells:
+            if 'cells' in selections and (r, c) in selections['cells']:
                 tf = self.table_selected_cells_fg
-            elif r in actual_selected_rows:
+            elif 'rows' in selections and r in selections['rows']:
                 tf = self.table_selected_rows_fg
-            elif c in actual_selected_cols:
+            elif 'columns' in selections and c in selections['columns']:
                 tf = self.table_selected_columns_fg
             else:
                 tf = self.table_fg
         return tf, redrawn
 
     def redraw_highlight(self, x1, y1, x2, y2, fill, outline, tag, can_width = None, pc = None):
         config = (fill, outline)
@@ -3861,18 +3826,15 @@
 
     def main_table_redraw_grid_and_text(self, redraw_header = False, redraw_row_index = False, redraw_table = True):
         last_col_line_pos = self.col_positions[-1] + 1
         last_row_line_pos = self.row_positions[-1] + 1
         try:
             can_width = self.winfo_width()
             can_height = self.winfo_height()
-            self.configure(scrollregion = (0,
-                                           0,
-                                           last_col_line_pos + self.empty_horizontal,
-                                           last_row_line_pos + self.empty_vertical))
+            self.configure(scrollregion = (0, 0, last_col_line_pos + self.empty_horizontal, last_row_line_pos + self.empty_vertical))
         except:
             return
         if can_width >= last_col_line_pos + self.empty_horizontal and self.parentframe.xscroll_showing:
             self.parentframe.xscroll.grid_forget()
             self.parentframe.xscroll_showing = False
         elif can_width < last_col_line_pos + self.empty_horizontal and not self.parentframe.xscroll_showing and not self.parentframe.xscroll_disabled and can_height > 45:
             self.parentframe.xscroll.grid(row = 2, column = 0, columnspan = 2, sticky = "nswe")
@@ -3992,22 +3954,22 @@
                 else:
                     self.disp_grid[self.create_line(points, fill = self.table_grid_fg, capstyle = tk.BUTT, joinstyle = tk.ROUND, width = 1, tag = "g")] = True
         if start_row > 0:
             start_row -= 1
         if start_col > 0:
             start_col -= 1
         end_row -= 1
+        selections = self.get_redraw_selections(start_row, end_row, start_col, end_col)
         c_2 = self.table_selected_cells_bg if self.table_selected_cells_bg.startswith("#") else Color_Map_[self.table_selected_cells_bg]
         c_2_ = (int(c_2[1:3], 16), int(c_2[3:5], 16), int(c_2[5:], 16))
         c_3 = self.table_selected_columns_bg if self.table_selected_columns_bg.startswith("#") else Color_Map_[self.table_selected_columns_bg]
         c_3_ = (int(c_3[1:3], 16), int(c_3[3:5], 16), int(c_3[5:], 16))
         c_4 = self.table_selected_rows_bg if self.table_selected_rows_bg.startswith("#") else Color_Map_[self.table_selected_rows_bg]
         c_4_ = (int(c_4[1:3], 16), int(c_4[3:5], 16), int(c_4[5:], 16))
         rows_ = tuple(range(start_row, end_row))
-        selected_cells, selected_rows, selected_cols, actual_selected_rows, actual_selected_cols = self.get_redraw_selections((start_row, start_col, end_row, end_col - 1))
         font = self.table_font
         if redraw_table:
             for c in range(start_col, end_col - 1):
                 for r in rows_:
                     rtopgridln = self.row_positions[r]
                     rbotgridln = self.row_positions[r + 1]
                     if rbotgridln - rtopgridln < self.txt_h:
@@ -4015,15 +3977,15 @@
                     cleftgridln = self.col_positions[c]
                     crightgridln = self.col_positions[c + 1]
                     
                     datarn = r if self.all_rows_displayed else self.displayed_rows[r]
                     datacn = c if self.all_columns_displayed else self.displayed_columns[c]
                     
                     fill, dd_drawn = self.redraw_highlight_get_text_fg(r, c, cleftgridln, rtopgridln, crightgridln, rbotgridln,
-                                                                       c_2_, c_3_, c_4_, selected_cells, actual_selected_rows, actual_selected_cols, 
+                                                                       c_2_, c_3_, c_4_, selections, 
                                                                        datarn, datacn, can_width)
                     align = self.get_cell_kwargs(datarn, datacn, key = 'align')
                     if align:
                         align = align
                     else:
                         align = self.align
                     kwargs = self.get_cell_kwargs(datarn, datacn, key = 'dropdown')
@@ -4103,23 +4065,25 @@
                                     iid, showing = self.hidd_text[k].pop()
                                     cc1, cc2 = self.coords(iid)
                                     if (int(cc1) == int(draw_x) and
                                         int(cc2) == int(draw_y)):
                                         option = 0 if showing else 2
                                     else:
                                         option = 1 if showing else 3
+                                    self.tag_raise(iid)
                                 elif self.hidd_text:
                                     k = next(iter(self.hidd_text))
                                     iid, showing = self.hidd_text[k].pop()
                                     cc1, cc2 = self.coords(iid)
                                     if (int(cc1) == int(draw_x) and
                                         int(cc2) == int(draw_y)):
                                         option = 2 if showing else 3
                                     else:
                                         option = 3
+                                    self.tag_raise(iid)
                                 else:
                                     iid, showing, option = self.create_text(draw_x, draw_y, text = txt, fill = fill, font = font, anchor = align, tag = "t"), 1, 4
                                 if option in (1, 3):
                                     self.coords(iid, draw_x, draw_y)
                                 if option in (2, 3):
                                     if showing:
                                         self.itemconfig(iid, text = txt, fill = fill, font = font, anchor = align)
@@ -4160,15 +4124,14 @@
                                     self.disp_text[config._replace(txt = txt)].add(DrawnItem(iid = iid, showing = True))
                                 else:
                                     self.disp_text[config].add(DrawnItem(iid = iid, showing = True))
                                 draw_y += self.xtra_lines_increment
                                 if draw_y + self.half_txt_h - 1 > rbotgridln:
                                     break
         if redraw_table:
-            self.tag_raise("t")
             for cfg, set_ in self.hidd_text.items():
                 for namedtup in tuple(set_):
                     if namedtup.showing:
                         self.itemconfig(namedtup.iid, state = "hidden")
                         self.hidd_text[cfg].discard(namedtup)
                         self.hidd_text[cfg].add(namedtup._replace(showing = False))
             for cfg, set_ in self.hidd_high.items():
@@ -4186,151 +4149,142 @@
                     self.itemconfig(t, state = "hidden")
                     self.hidd_dropdown[t] = False
             for t, sh in self.hidd_checkbox.items():
                 if sh:
                     self.itemconfig(t, state = "hidden")
                     self.hidd_checkbox[t] = False
             if self.show_selected_cells_border:
-                self.tag_raise("CellSelectBorder")
-                self.tag_raise("Current_Inside")
-                self.tag_raise("Current_Outside")
-                self.tag_raise("RowSelectBorder")
-                self.tag_raise("ColSelectBorder")
+                self.tag_raise("cellsbd")
+                self.tag_raise("currently")
+                self.tag_raise("rowsbd")
+                self.tag_raise("columnsbd")
         if redraw_header and self.show_header:
-            self.CH.redraw_grid_and_text(last_col_line_pos, scrollpos_left, x_stop, start_col, end_col, scrollpos_right, selected_cols, actual_selected_rows, actual_selected_cols, col_pos_exists)
+            self.CH.redraw_grid_and_text(last_col_line_pos, scrollpos_left, x_stop, start_col, end_col, scrollpos_right, col_pos_exists)
         if redraw_row_index and self.show_index:
-            self.RI.redraw_grid_and_text(last_row_line_pos, scrollpos_top, y_stop, start_row, end_row + 1, scrollpos_bot, selected_rows, actual_selected_cols, actual_selected_rows, row_pos_exists)
+            self.RI.redraw_grid_and_text(last_row_line_pos, scrollpos_top, y_stop, start_row, end_row + 1, scrollpos_bot, row_pos_exists)
+        self.parentframe.emit_event("<<SheetRedrawn>>")
         return True
 
     def get_all_selection_items(self):
-        return sorted(self.find_withtag("CellSelectFill") + self.find_withtag("RowSelectFill") + self.find_withtag("ColSelectFill") + self.find_withtag("Current_Inside") + self.find_withtag("Current_Outside"))
+        return sorted(self.find_withtag("cells") + self.find_withtag("rows") + self.find_withtag("columns") + self.find_withtag("currently"))
 
     def get_boxes(self, include_current = True):
         boxes = {}
         for item in self.get_all_selection_items():
             alltags = self.gettags(item)
-            if alltags[0] == "CellSelectFill":
+            if alltags[0] == "cells":
                 boxes[tuple(int(e) for e in alltags[1].split("_") if e)] = "cells"
-            elif alltags[0] == "RowSelectFill":
+            elif alltags[0] == "rows":
                 boxes[tuple(int(e) for e in alltags[1].split("_") if e)] = "rows"
-            elif alltags[0] == "ColSelectFill":
+            elif alltags[0] == "columns":
                 boxes[tuple(int(e) for e in alltags[1].split("_") if e)] = "columns"
-            elif include_current and alltags[0] == "Current_Inside":
-                boxes[tuple(int(e) for e in alltags[1].split("_") if e)] = f"{alltags[2]}_inside"
-            elif include_current and alltags[0] == "Current_Outside":
-                boxes[tuple(int(e) for e in alltags[1].split("_") if e)] = f"{alltags[2]}_outside"
+            elif include_current and alltags[0] == "currently":
+                boxes[tuple(int(e) for e in alltags[1].split("_") if e)] = f"{alltags[2]}"
         return boxes
 
     def reselect_from_get_boxes(self, boxes):
         for (r1, c1, r2, c2), v in boxes.items():
             if r2 < len(self.row_positions) and c2 < len(self.col_positions):
                 if v == "cells":
                     self.create_selected(r1, c1, r2, c2, "cells")
                 elif v == "rows":
                     self.create_selected(r1, c1, r2, c2, "rows")
                 elif v == "columns":
                     self.create_selected(r1, c1, r2, c2, "columns")
-                elif v in ("cell_inside", "cell_outside", "row_inside", "row_outside", "col_outside", "col_inside"): #currently selected
-                    x = v.split("_")
-                    self.create_current(r1, c1, type_ = x[0], inside = True if x[1] == "inside" else False)
+                elif v in ("cell", "row", "column"): #currently selected
+                    self.set_currently_selected(r1, c1, type_ = v)
                 
     def delete_selected(self, r1 = None, c1 = None, r2 = None, c2 = None, type_ = None):
         deleted_boxes = {}
         tags_to_del = set()
         box1 = (r1, c1, r2, c2)
         for s in self.get_selection_tags_from_type(type_):
             for item in self.find_withtag(s):
                 alltags = self.gettags(item)
                 if alltags:
                     box2 = tuple(int(e) for e in alltags[1].split("_") if e)
                     if box1 == box2:
                         tags_to_del.add(alltags)
-                        deleted_boxes[box2] = "cells" if alltags[0].startswith("Cell") else "rows" if alltags[0].startswith("Row") else "columns"
+                        deleted_boxes[box2] = "cells" if alltags[0].startswith("cell") else "rows" if alltags[0].startswith("row") else "columns"
                         self.delete(item)
         for canvas in (self.RI, self.CH):
             for item in canvas.find_withtag(s):
                 if canvas.gettags(item) in tags_to_del:
                     canvas.delete(item)
 
     def get_selection_tags_from_type(self, type_):
         if type_ == "cells":
-            return {"CellSelectFill", "CellSelectBorder"}
+            return {"cells", "cellsbd"}
         if type_ == "rows":
-            return {"RowSelectFill", "RowSelectBorder"}
+            return {"rows", "rowsbd"}
         elif type_ == "columns":
-            return {"ColSelectFill", "ColSelectBorder"}
+            return {"columns", "columnsbd"}
         else:
-            return {"CellSelectFill", "CellSelectBorder", "RowSelectFill", "RowSelectBorder", "ColSelectFill", "ColSelectBorder"}             
+            return {"cells", "cellsbd", "rows", "rowsbd", "columns", "columnsbd"}             
 
     def delete_selection_rects(self, cells = True, rows = True, cols = True, delete_current = True):
         deleted_boxes = {}
         if cells:
-            for item in self.find_withtag("CellSelectFill"):
+            for item in self.find_withtag("cells"):
                 alltags = self.gettags(item)
                 if alltags:
                     deleted_boxes[tuple(int(e) for e in alltags[1].split("_") if e)] = "cells"
-            self.delete("CellSelectFill", "CellSelectBorder")
-            self.RI.delete("CellSelectFill", "CellSelectBorder")
-            self.CH.delete("CellSelectFill", "CellSelectBorder")
+            self.delete("cells", "cellsbd")
+            self.RI.delete("cells", "cellsbd")
+            self.CH.delete("cells", "cellsbd")
         if rows:
-            for item in self.find_withtag("RowSelectFill"):
+            for item in self.find_withtag("rows"):
                 alltags = self.gettags(item)
                 if alltags:
                     deleted_boxes[tuple(int(e) for e in alltags[1].split("_") if e)] = "rows"
-            self.delete("RowSelectFill", "RowSelectBorder")
-            self.RI.delete("RowSelectFill", "RowSelectBorder")
-            self.CH.delete("RowSelectFill", "RowSelectBorder")
+            self.delete("rows", "rowsbd")
+            self.RI.delete("rows", "rowsbd")
+            self.CH.delete("rows", "rowsbd")
         if cols:
-            for item in self.find_withtag("ColSelectFill"):
+            for item in self.find_withtag("columns"):
                 alltags = self.gettags(item)
                 if alltags:
                     deleted_boxes[tuple(int(e) for e in alltags[1].split("_") if e)] = "columns"
-            self.delete("ColSelectFill", "ColSelectBorder")
-            self.RI.delete("ColSelectFill", "ColSelectBorder")
-            self.CH.delete("ColSelectFill", "ColSelectBorder")
+            self.delete("columns", "columnsbd")
+            self.RI.delete("columns", "columnsbd")
+            self.CH.delete("columns", "columnsbd")
         if delete_current:
-            for item in chain(self.find_withtag("Current_Inside"), self.find_withtag("Current_Outside")):
-                alltags = self.gettags(item)
-                if alltags:
-                    deleted_boxes[tuple(int(e) for e in alltags[1].split("_") if e)] = "cells"
-            self.delete("Current_Inside", "Current_Outside")
-            self.RI.delete("Current_Inside", "Current_Outside")
-            self.CH.delete("Current_Inside", "Current_Outside")
+            self.delete("currently")
+            self.RI.delete("currently")
+            self.CH.delete("currently")
         return deleted_boxes
 
     def currently_selected(self):
-        items = self.find_withtag("Current_Inside") + self.find_withtag("Current_Outside")
+        items = self.find_withtag("currently")
         if not items:
             return tuple()
         alltags = self.gettags(items[0])
         box = tuple(int(e) for e in alltags[1].split("_") if e)
         return CurrentlySelectedClass(box[0], box[1], alltags[2])
 
     def get_tags_of_current(self):
-        items = self.find_withtag("Current_Inside") + self.find_withtag("Current_Outside")
+        items = self.find_withtag("currently")
         if items:
             return self.gettags(items[0])
         else:
             return tuple()
 
-    def create_current(self, r, c, type_ = "cell", inside = False): # cell, column or row
+    def set_currently_selected(self, r, c, type_ = "cell"): # cell, column or row
         r1, c1, r2, c2 = r, c, r + 1, c + 1
-        self.delete("Current_Inside", "Current_Outside")
-        self.RI.delete("Current_Inside", "Current_Outside")
-        self.CH.delete("Current_Inside", "Current_Outside")
+        self.delete("currently")
+        self.RI.delete("currently")
+        self.CH.delete("currently")
         if self.col_positions == [0]:
             c1 = 0
             c2 = 0
         if self.row_positions == [0]:
             r1 = 0
             r2 = 0
-        if inside:
-            tagr = ("Current_Inside", f"{r1}_{c1}_{r2}_{c2}", type_)
-        else:
-            tagr = ("Current_Outside", f"{r1}_{c1}_{r2}_{c2}", type_)
+        tagr = ("currently", f"{r1}_{c1}_{r2}_{c2}", type_)
+        tag_index_header = ("cells", f"{r1}_{c1}_{r2}_{c2}")
         if type_ == "cell":
             outline = self.table_selected_cells_border_fg
         elif type_ == "row":
             outline = self.table_selected_rows_border_fg
         elif type_ == "column":
             outline = self.table_selected_columns_border_fg
         if self.show_selected_cells_border:
@@ -4345,264 +4299,157 @@
                                       fill = self.table_selected_cells_bg,
                                       outline = "",
                                       tags = tagr)
             self.tag_lower(b)
         ri = self.RI.create_rectangle(0, self.row_positions[r1], self.RI.current_width - 1, self.row_positions[r2],
                                       fill = self.RI.index_selected_cells_bg,
                                       outline = "",
-                                      tags = tagr)
+                                      tags = tag_index_header)
         ch = self.CH.create_rectangle(self.col_positions[c1], 0, self.col_positions[c2], self.CH.current_height - 1,
                                       fill = self.CH.header_selected_cells_bg,
                                       outline = "",
-                                      tags = tagr)
+                                      tags = tag_index_header)
         self.RI.tag_lower(ri)
         self.CH.tag_lower(ch)
         return b
 
     def set_current_to_last(self):
         if not self.currently_selected():
-            items = sorted(self.find_withtag("CellSelectFill") + self.find_withtag("RowSelectFill") + self.find_withtag("ColSelectFill"))
+            items = sorted(self.find_withtag("cells") + self.find_withtag("rows") + self.find_withtag("columns"))
             if items:
                 last = self.gettags(items[-1])
                 r1, c1, r2, c2 = tuple(int(e) for e in last[1].split("_") if e)
-                if last[0] == "CellSelectFill":
-                    return self.gettags(self.create_current(r1, c1, "cell", inside = True))
-                elif last[0] == "RowSelectFill":
-                    return self.gettags(self.create_current(r1, c1, "row", inside = True))
-                elif last[0] == "ColSelectFill":
-                    return self.gettags(self.create_current(r1, c1, "column", inside = True))
+                if last[0] == "cells":
+                    return self.gettags(self.set_currently_selected(r1, c1, "cell"))
+                elif last[0] == "rows":
+                    return self.gettags(self.set_currently_selected(r1, c1, "row"))
+                elif last[0] == "columns":
+                    return self.gettags(self.set_currently_selected(r1, c1, "column"))
         return tuple()
    
     def delete_current(self):
-        self.delete("Current_Inside", "Current_Outside")
-        self.RI.delete("Current_Inside", "Current_Outside")
-        self.CH.delete("Current_Inside", "Current_Outside")
+        self.delete("currently")
+        self.RI.delete("currently")
+        self.CH.delete("currently")
             
-    def create_selected(self, r1 = None, c1 = None, r2 = None, c2 = None, type_ = "cells", taglower = True):
-        currently_selected = self.currently_selected()
-        if currently_selected and currently_selected.type_ == "cell":
-            if (currently_selected.row >= r1 and
-                currently_selected.column >= c1 and
-                currently_selected.row < r2 and
-                currently_selected.column < c2):
-                self.create_current(currently_selected.row, currently_selected.column, type_ = "cell", inside = True)
+    def create_selected(self, r1 = None, c1 = None, r2 = None, c2 = None, type_ = "cells", taglower = True, state = "normal"):
+        self.itemconfig("cells", state = "normal")
         if type_ == "cells":
-            tagr = ("CellSelectFill", f"{r1}_{c1}_{r2}_{c2}")
-            tagb = ("CellSelectBorder", f"{r1}_{c1}_{r2}_{c2}")
-            taglower = "CellSelectFill"
+            tagr = ("cells", f"{r1}_{c1}_{r2}_{c2}")
+            tagb = ("cellsbd", f"{r1}_{c1}_{r2}_{c2}")
             mt_bg = self.table_selected_cells_bg
             mt_border_col = self.table_selected_cells_border_fg
         elif type_ == "rows":
-            tagr = ("RowSelectFill", f"{r1}_{c1}_{r2}_{c2}")
-            tagb = ("RowSelectBorder", f"{r1}_{c1}_{r2}_{c2}")
-            taglower = "RowSelectFill"
+            tagr = ("rows", f"{r1}_{c1}_{r2}_{c2}")
+            tagb = ("rowsbd", f"{r1}_{c1}_{r2}_{c2}")
+            tag_index_header = ("cells", f"{r1}_{c1}_{r2}_{c2}")
             mt_bg = self.table_selected_rows_bg
             mt_border_col = self.table_selected_rows_border_fg
         elif type_ == "columns":
-            tagr = ("ColSelectFill", f"{r1}_{c1}_{r2}_{c2}")
-            tagb = ("ColSelectBorder", f"{r1}_{c1}_{r2}_{c2}")
-            taglower = "ColSelectFill"
+            tagr = ("columns", f"{r1}_{c1}_{r2}_{c2}")
+            tagb = ("columnsbd", f"{r1}_{c1}_{r2}_{c2}")
+            tag_index_header = ("cells", f"{r1}_{c1}_{r2}_{c2}")
             mt_bg = self.table_selected_columns_bg
             mt_border_col = self.table_selected_columns_border_fg
         self.last_selected = (r1, c1, r2, c2, type_)
+        ch_tags = tag_index_header if type_ == "rows" else tagr
+        ri_tags = tag_index_header if type_ == "columns" else tagr
         r = self.create_rectangle(self.col_positions[c1],
                                   self.row_positions[r1],
                                   self.canvasx(self.winfo_width()) if self.selected_rows_to_end_of_window else self.col_positions[c2],
                                   self.row_positions[r2],
                                   fill = mt_bg,
                                   outline = "",
+                                  state = state,
                                   tags = tagr)
-        
         self.RI.create_rectangle(0,
                                  self.row_positions[r1],
                                  self.RI.current_width - 1,
                                  self.row_positions[r2],
                                  fill = self.RI.index_selected_rows_bg if type_ == "rows" else self.RI.index_selected_cells_bg,
                                  outline = "",
-                                 tags = tagr)
+                                 tags = ri_tags)
         self.CH.create_rectangle(self.col_positions[c1],
                                  0,
                                  self.col_positions[c2],
                                  self.CH.current_height - 1,
                                  fill = self.CH.header_selected_columns_bg if type_ == "columns" else self.CH.header_selected_cells_bg,
                                  outline = "",
-                                 tags = tagr)
+                                 tags = ch_tags)
         if self.show_selected_cells_border and ((self.being_drawn_rect is None and self.RI.being_drawn_rect is None and self.CH.being_drawn_rect is None) or len(self.anything_selected()) > 1):
             b = self.create_rectangle(self.col_positions[c1], self.row_positions[r1], self.col_positions[c2], self.row_positions[r2],
                                       fill = "",
                                       outline = mt_border_col,
                                       tags = tagb)
         else:
             b = None
         if taglower:
-            self.tag_lower(taglower)
-            self.RI.tag_lower(taglower)
-            self.CH.tag_lower(taglower)
-            self.RI.tag_lower("Current_Inside")
-            self.RI.tag_lower("Current_Outside")
-            self.RI.tag_lower("CellSelectFill")
-            self.CH.tag_lower("Current_Inside")
-            self.CH.tag_lower("Current_Outside")
-            self.CH.tag_lower("CellSelectFill")
+            self.tag_lower("rows")
+            self.RI.tag_lower("rows")
+            self.tag_lower("columns")
+            self.CH.tag_lower("columns")
+            self.tag_lower("cells")
+            self.RI.tag_lower("cells")
+            self.CH.tag_lower("cells")
         return r, b
 
     def recreate_all_selection_boxes(self):
-        for item in chain(self.find_withtag("CellSelectFill"),
-                          self.find_withtag("RowSelectFill"),
-                          self.find_withtag("ColSelectFill"),
-                          self.find_withtag("Current_Inside"),
-                          self.find_withtag("Current_Outside")):
-            full_tags = self.gettags(item)
-            if full_tags:
-                type_ = full_tags[0]
-                r1, c1, r2, c2 = tuple(int(e) for e in full_tags[1].split("_") if e)
+        for item in chain(self.find_withtag("cells"),
+                          self.find_withtag("rows"),
+                          self.find_withtag("columns"),
+                          self.find_withtag("currently")):
+            tags = self.gettags(item)
+            if tags:
+                r1, c1, r2, c2 = tuple(int(e) for e in tags[1].split("_") if e)
                 self.delete(f"{r1}_{c1}_{r2}_{c2}")
                 self.RI.delete(f"{r1}_{c1}_{r2}_{c2}")
                 self.CH.delete(f"{r1}_{c1}_{r2}_{c2}")
                 if r1 >= len(self.row_positions) - 1 or c1 >= len(self.col_positions) - 1:
                     continue
                 if r2 > len(self.row_positions) - 1:
                     r2 = len(self.row_positions) - 1
                 if c2 > len(self.col_positions) - 1:
                     c2 = len(self.col_positions) - 1
-                if type_.startswith("CellSelect"):
-                    self.create_selected(r1, c1, r2, c2, "cells")
-                elif type_.startswith("RowSelect"):
-                    self.create_selected(r1, c1, r2, c2, "rows")
-                elif type_.startswith("ColSelect"):
-                    self.create_selected(r1, c1, r2, c2, "columns")
-                elif type_.startswith("Current"):
-                    if type_ == "Current_Inside":
-                        self.create_current(r1, c1, full_tags[2], inside = True)
-                    elif type_ == "Current_Outside":
-                        self.create_current(r1, c1, full_tags[2], inside = False)
-        self.tag_lower("RowSelectFill")
-        self.RI.tag_lower("RowSelectFill")
-        self.CH.tag_lower("RowSelectFill")
-        self.tag_lower("ColSelectFill")
-        self.RI.tag_lower("ColSelectFill")
-        self.CH.tag_lower("ColSelectFill")
-        self.tag_lower("CellSelectFill")
-        self.RI.tag_lower("CellSelectFill")
-        self.CH.tag_lower("CellSelectFill")
-        self.RI.tag_lower("Current_Inside")
-        self.RI.tag_lower("Current_Outside")
-        self.CH.tag_lower("Current_Inside")
-        self.CH.tag_lower("Current_Outside")
-        if not self.show_selected_cells_border:
-            self.tag_lower("Current_Outside")
-
-    def get_redraw_selections(self, within_range):
-        scells = set()
-        srows = set()
-        scols = set()
-        ac_srows = set()
-        ac_scols = set()
-        within_r1 = within_range[0]
-        within_c1 = within_range[1]
-        within_r2 = within_range[2]
-        within_c2 = within_range[3]
-        for item in self.find_withtag("RowSelectFill"):
-            r1, c1, r2, c2 = tuple(int(e) for e in self.gettags(item)[1].split("_") if e)
-            if (r1 >= within_r1 or
-                r2 <= within_r2) or (within_r1 >= r1 and within_r2 <= r2):
-                if r1 > within_r1:
-                    start_row = r1
-                else:
-                    start_row = within_r1
-                if r2 < within_r2:
-                    end_row = r2
-                else:
-                    end_row = within_r2
-                srows.update(set(range(start_row, end_row)))
-                ac_srows.update(set(range(start_row, end_row)))
-        for item in chain(self.find_withtag("Current_Outside"), self.find_withtag("Current_Inside")):
-            r1, c1, r2, c2 = tuple(int(e) for e in self.gettags(item)[1].split("_") if e)
-            if (r1 >= within_r1 or
-                r2 <= within_r2):
-                if r1 > within_r1:
-                    start_row = r1
-                else:
-                    start_row = within_r1
-                if r2 < within_r2:
-                    end_row = r2
-                else:
-                    end_row = within_r2
-                srows.update(set(range(start_row, end_row)))
-        for item in self.find_withtag("ColSelectFill"): 
-            r1, c1, r2, c2 = tuple(int(e) for e in self.gettags(item)[1].split("_") if e)
-            if (c1 >= within_c1 or
-                c2 <= within_c2) or (within_c1 >= c1 and within_c2 <= c2):
-                if c1 > within_c1:
-                    start_col = c1
-                else:
-                    start_col = within_c1
-                if c2 < within_c2:
-                    end_col = c2
-                else:
-                    end_col = within_c2
-                scols.update(set(range(start_col, end_col)))
-                ac_scols.update(set(range(start_col, end_col)))
-        for item in self.find_withtag("Current_Outside"):
-            r1, c1, r2, c2 = tuple(int(e) for e in self.gettags(item)[1].split("_") if e)
-            if (c1 >= within_c1 or
-                c2 <= within_c2):
-                if c1 > within_c1:
-                    start_col = c1
+                if tags[0] == "currently":
+                    self.set_currently_selected(r1, c1, tags[2])
                 else:
-                    start_col = within_c1
-                if c2 < within_c2:
-                    end_col = c2
-                else:
-                    end_col = within_c2
-                scols.update(set(range(start_col, end_col)))
+                    self.create_selected(r1, c1, r2, c2, tags[0])
+        self.tag_lower("rows")
+        self.RI.tag_lower("rows")
+        self.tag_lower("columns")
+        self.CH.tag_lower("columns")
+        self.tag_lower("cells")
+        self.RI.tag_lower("cells")
+        self.CH.tag_lower("cells")
         if not self.show_selected_cells_border:
-            iterable = chain(self.find_withtag("CellSelectFill"), self.find_withtag("Current_Outside"))
-        else:
-            iterable = self.find_withtag("CellSelectFill")
-        for item in iterable:
+            self.tag_lower("currently")
+    
+    def get_redraw_selections(self, startr, endr, startc, endc):
+        d = defaultdict(list)
+        for item in chain(self.find_withtag("cells"), self.find_withtag("rows"), self.find_withtag("columns")):
             tags = self.gettags(item)
-            r1, c1, r2, c2 = tuple(int(e) for e in tags[1].split("_") if e)
-            if (r1 >= within_r1 or
-                c1 >= within_c1 or
-                r2 <= within_r2 or
-                c2 <= within_c2) or (within_c1 >= c1 and within_c2 <= c2) or (within_r1 >= r1 and within_r2 <= r2):
-                if r1 > within_r1:
-                    start_row = r1
-                else:
-                    start_row = within_r1
-                if c1 > within_c1:
-                    start_col = c1
-                else:
-                    start_col = within_c1
-                if r2 < within_r2:
-                    end_row = r2
-                else:
-                    end_row = within_r2
-                if c2 < within_c2:
-                    end_col = c2
-                else:
-                    end_col = within_c2
-                colsr = tuple(range(start_col, end_col))
-                rowsr = tuple(range(start_row, end_row))
-                scells.update(set(product(rowsr, colsr)))
-                srows.update(set(range(start_row, end_row)))
-                scols.update(set(range(start_col, end_col)))
-        return scells, srows, scols, ac_srows, ac_scols
+            d[tags[0]].append(tuple(int(e) for e in tags[1].split("_") if e))
+        d2 = {}
+        if 'cells' in d:
+            d2['cells'] = {(r, c) for r in range(startr, endr) for c in range(startc, endc) for r1, c1, r2, c2 in d['cells'] if r1 <= r and c1 <= c and r2 > r and c2 > c}
+        if 'rows' in d:
+            d2['rows'] = {r for r in range(startr, endr) for r1, c1, r2, c2 in d['rows'] if r1 <= r and r2 > r}
+        if 'columns' in d:
+            d2['columns'] = {c for c in range(startc, endc) for r1, c1, r2, c2 in d['columns'] if c1 <= c and c2 > c}
+        return d2
 
     def get_selected_min_max(self):
         min_x = float("inf")
         min_y = float("inf")
         max_x = 0
         max_y = 0
-        for item in chain(self.find_withtag("CellSelectFill"),
-                          self.find_withtag("RowSelectFill"),
-                          self.find_withtag("ColSelectFill"),
-                          self.find_withtag("Current_Inside"),
-                          self.find_withtag("Current_Outside")):
+        for item in chain(self.find_withtag("cells"),
+                          self.find_withtag("rows"),
+                          self.find_withtag("columns"),
+                          self.find_withtag("currently")):
             r1, c1, r2, c2 = tuple(int(e) for e in self.gettags(item)[1].split("_") if e)
             if r1 < min_y:
                 min_y = r1
             if c1 < min_x:
                 min_x = c1
             if r2 > max_y:
                 max_y = r2
@@ -4616,21 +4463,21 @@
     def get_selected_rows(self, get_cells = False, within_range = None, get_cells_as_rows = False):
         s = set()
         if within_range is not None:
             within_r1 = within_range[0]
             within_r2 = within_range[1]
         if get_cells:
             if within_range is None:
-                for item in self.find_withtag("RowSelectFill"):
+                for item in self.find_withtag("rows"):
                     r1, c1, r2, c2 = tuple(int(e) for e in self.gettags(item)[1].split("_") if e)
                     s.update(set(product(range(r1, r2), range(0, len(self.col_positions) - 1))))
                 if get_cells_as_rows:
                     s.update(self.get_selected_cells())
             else:
-                for item in self.find_withtag("RowSelectFill"):
+                for item in self.find_withtag("rows"):
                     r1, c1, r2, c2 = tuple(int(e) for e in self.gettags(item)[1].split("_") if e)
                     if (r1 >= within_r1 or
                         r2 <= within_r2):
                         if r1 > within_r1:
                             start_row = r1
                         else:
                             start_row = within_r1
@@ -4639,21 +4486,21 @@
                         else:
                             end_row = within_r2
                         s.update(set(product(range(start_row, end_row), range(0, len(self.col_positions) - 1))))
                 if get_cells_as_rows:
                     s.update(self.get_selected_cells(within_range = (within_r1, 0, within_r2, len(self.col_positions) - 1)))
         else:
             if within_range is None:
-                for item in self.find_withtag("RowSelectFill"):
+                for item in self.find_withtag("rows"):
                     r1, c1, r2, c2 = tuple(int(e) for e in self.gettags(item)[1].split("_") if e)
                     s.update(set(range(r1, r2)))
                 if get_cells_as_rows:
                     s.update(set(tup[0] for tup in self.get_selected_cells()))
             else:
-                for item in self.find_withtag("RowSelectFill"):
+                for item in self.find_withtag("rows"):
                     r1, c1, r2, c2 = tuple(int(e) for e in self.gettags(item)[1].split("_") if e)
                     if (r1 >= within_r1 or
                         r2 <= within_r2):
                         if r1 > within_r1:
                             start_row = r1
                         else:
                             start_row = within_r1
@@ -4669,21 +4516,21 @@
     def get_selected_cols(self, get_cells = False, within_range = None, get_cells_as_cols = False):
         s = set()
         if within_range is not None:
             within_c1 = within_range[0]
             within_c2 = within_range[1]
         if get_cells:
             if within_range is None:
-                for item in self.find_withtag("ColSelectFill"):
+                for item in self.find_withtag("columns"):
                     r1, c1, r2, c2 = tuple(int(e) for e in self.gettags(item)[1].split("_") if e)
                     s.update(set(product(range(c1, c2), range(0, len(self.row_positions) - 1))))
                 if get_cells_as_cols:
                     s.update(self.get_selected_cells())
             else:
-                for item in self.find_withtag("ColSelectFill"):
+                for item in self.find_withtag("columns"):
                     r1, c1, r2, c2 = tuple(int(e) for e in self.gettags(item)[1].split("_") if e)
                     if (c1 >= within_c1 or
                         c2 <= within_c2):
                         if c1 > within_c1:
                             start_col = c1
                         else:
                             start_col = within_c1
@@ -4692,21 +4539,21 @@
                         else:
                             end_col = within_c2
                         s.update(set(product(range(start_col, end_col), range(0, len(self.row_positions) - 1))))
                 if get_cells_as_cols:
                     s.update(self.get_selected_cells(within_range = (0, within_c1, len(self.row_positions) - 1, within_c2)))
         else:
             if within_range is None:
-                for item in self.find_withtag("ColSelectFill"):
+                for item in self.find_withtag("columns"):
                     r1, c1, r2, c2 = tuple(int(e) for e in self.gettags(item)[1].split("_") if e)
                     s.update(set(range(c1, c2)))
                 if get_cells_as_cols:
                     s.update(set(tup[1] for tup in self.get_selected_cells()))
             else:
-                for item in self.find_withtag("ColSelectFill"):
+                for item in self.find_withtag("columns"):
                     r1, c1, r2, c2 = tuple(int(e) for e in self.gettags(item)[1].split("_") if e)
                     if (c1 >= within_c1 or
                         c2 <= within_c2):
                         if c1 > within_c1:
                             start_col = c1
                         else:
                             start_col = within_c1
@@ -4723,21 +4570,21 @@
         s = set()
         if within_range is not None:
             within_r1 = within_range[0]
             within_c1 = within_range[1]
             within_r2 = within_range[2]
             within_c2 = within_range[3]
         if get_cols and get_rows:
-            iterable = chain(self.find_withtag("CellSelectFill"), self.find_withtag("RowSelectFill"), self.find_withtag("ColSelectFill"), self.find_withtag("Current_Outside"))
+            iterable = chain(self.find_withtag("cells"), self.find_withtag("rows"), self.find_withtag("columns"))
         elif get_rows and not get_cols:
-            iterable = chain(self.find_withtag("CellSelectFill"), self.find_withtag("RowSelectFill"), self.find_withtag("Current_Outside"))
+            iterable = chain(self.find_withtag("cells"), self.find_withtag("rows"))
         elif get_cols and not get_rows:
-            iterable = chain(self.find_withtag("CellSelectFill"), self.find_withtag("ColSelectFill"), self.find_withtag("Current_Outside"))
+            iterable = chain(self.find_withtag("cells"), self.find_withtag("columns"))
         else:
-            iterable = chain(self.find_withtag("CellSelectFill"), self.find_withtag("Current_Outside"))
+            iterable = chain(self.find_withtag("cells"))
         if within_range is None:
             for item in iterable:
                 r1, c1, r2, c2 = tuple(int(e) for e in self.gettags(item)[1].split("_") if e)
                 s.update(set(product(range(r1, r2), range(c1, c2))))
         else:
             for item in iterable:
                 r1, c1, r2, c2 = tuple(int(e) for e in self.gettags(item)[1].split("_") if e)
@@ -4761,99 +4608,93 @@
                         end_col = c2
                     else:
                         end_col = within_c2
                     s.update(set(product(range(start_row, end_row), range(start_col, end_col))))
         return s
 
     def get_all_selection_boxes(self):
-        return tuple(tuple(int(e) for e in self.gettags(item)[1].split("_") if e) for item in chain(self.find_withtag("CellSelectFill"),
-                                                                                                    self.find_withtag("RowSelectFill"),
-                                                                                                    self.find_withtag("ColSelectFill"),
-                                                                                                    self.find_withtag("Current_Outside")))
+        return tuple(tuple(int(e) for e in self.gettags(item)[1].split("_") if e) for item in chain(self.find_withtag("cells"),
+                                                                                                    self.find_withtag("rows"),
+                                                                                                    self.find_withtag("columns")))
 
     def get_all_selection_boxes_with_types(self):
         boxes = []
-        for item in sorted(self.find_withtag("CellSelectFill") + self.find_withtag("RowSelectFill") + self.find_withtag("ColSelectFill") + self.find_withtag("Current_Outside")):
+        for item in sorted(self.find_withtag("cells") + self.find_withtag("rows") + self.find_withtag("columns")):
             tags = self.gettags(item)
-            if tags:
-                if tags[0].startswith(("Cell", "Current")):
-                    boxes.append((tuple(int(e) for e in tags[1].split("_") if e), "cells"))
-                elif tags[0].startswith("Row"):
-                    boxes.append((tuple(int(e) for e in tags[1].split("_") if e), "rows"))
-                elif tags[0].startswith("Col"):
-                    boxes.append((tuple(int(e) for e in tags[1].split("_") if e), "columns"))
+            boxes.append((tuple(int(e) for e in tags[1].split("_") if e), tags[0]))
         return boxes
 
     def all_selected(self):
         for r1, c1, r2, c2 in self.get_all_selection_boxes():
             if not r1 and not c1 and r2 == len(self.row_positions) - 1 and c2 == len(self.col_positions) - 1:
                 return True
         return False
     
+    # don't have to use "currently" because you can't have a current without a selection box
     def cell_selected(self, r, c, inc_cols = False, inc_rows = False):
         if not isinstance(r, int) or not isinstance(c, int):
             return False
         if not inc_cols and not inc_rows:
-            iterable = chain(self.find_withtag("CellSelectFill"), self.find_withtag("Current_Inside"), self.find_withtag("Current_Outside"))
+            iterable = self.find_withtag("cells")
         elif inc_cols and not inc_rows:
-            iterable = chain(self.find_withtag("ColSelectFill"), self.find_withtag("CellSelectFill"), self.find_withtag("Current_Inside"), self.find_withtag("Current_Outside"))
+            iterable = chain(self.find_withtag("columns"), self.find_withtag("cells"))
         elif not inc_cols and inc_rows:
-            iterable = chain(self.find_withtag("RowSelectFill"), self.find_withtag("CellSelectFill"), self.find_withtag("Current_Inside"), self.find_withtag("Current_Outside"))
+            iterable = chain(self.find_withtag("rows"), self.find_withtag("cells"))
         elif inc_cols and inc_rows:
-            iterable = chain(self.find_withtag("RowSelectFill"), self.find_withtag("ColSelectFill"), self.find_withtag("CellSelectFill"), self.find_withtag("Current_Inside"), self.find_withtag("Current_Outside"))
+            iterable = chain(self.find_withtag("rows"), self.find_withtag("columns"), self.find_withtag("cells"))
         for item in iterable:
             r1, c1, r2, c2 = tuple(int(e) for e in self.gettags(item)[1].split("_") if e)
             if r1 <= r and c1 <= c and r2 > r and c2 > c:
                 return True
         return False
 
     def col_selected(self, c):
         if not isinstance(c, int):
             return False
-        for item in self.find_withtag("ColSelectFill"):
+        for item in self.find_withtag("columns"):
             r1, c1, r2, c2 = tuple(int(e) for e in self.gettags(item)[1].split("_") if e)
             if c1 <= c and c2 > c:
                 return True
         return False
 
     def row_selected(self, r):
         if not isinstance(r, int):
             return False
-        for item in self.find_withtag("RowSelectFill"):
+        for item in self.find_withtag("rows"):
             r1, c1, r2, c2 = tuple(int(e) for e in self.gettags(item)[1].split("_") if e)
             if r1 <= r and r2 > r:
                 return True
         return False
 
     def anything_selected(self, exclude_columns = False, exclude_rows = False, exclude_cells = False):
         if exclude_columns and exclude_rows and not exclude_cells:
-            return self.find_withtag("CellSelectFill") + self.find_withtag("Current_Outside")
+            return self.find_withtag("cells")
         elif exclude_columns and exclude_cells and not exclude_rows:
-            return self.find_withtag("RowSelectFill")
+            return self.find_withtag("rows")
         elif exclude_rows and exclude_cells and not exclude_columns:
-            return self.find_withtag("ColSelectFill")
+            return self.find_withtag("columns")
             
         elif exclude_columns and not exclude_rows and not exclude_cells:
-            return self.find_withtag("CellSelectFill") + self.find_withtag("RowSelectFill") + self.find_withtag("Current_Outside")
+            return self.find_withtag("cells") + self.find_withtag("rows")
         elif exclude_rows and not exclude_columns and not exclude_cells:
-            return self.find_withtag("CellSelectFill") + self.find_withtag("ColSelectFill") + self.find_withtag("Current_Outside")
+            return self.find_withtag("cells") + self.find_withtag("columns")
 
         elif exclude_cells and not exclude_columns and not exclude_rows:
-            return self.find_withtag("RowSelectFill") + self.find_withtag("ColSelectFill")
+            return self.find_withtag("rows") + self.find_withtag("columns")
             
         elif not exclude_columns and not exclude_rows and not exclude_cells:
-            return self.find_withtag("CellSelectFill") + self.find_withtag("RowSelectFill") + self.find_withtag("ColSelectFill") + self.find_withtag("Current_Outside")
+            return self.find_withtag("cells") + self.find_withtag("rows") + self.find_withtag("columns")
         return tuple()
 
     def hide_current(self):
-        for item in chain(self.find_withtag("Current_Inside"), self.find_withtag("Current_Outside")):
+        for item in self.find_withtag("currently"):
             self.itemconfig(item, state = "hidden")
 
     def show_current(self):
-        for item in chain(self.find_withtag("Current_Inside"), self.find_withtag("Current_Outside")):
+        for item in self.find_withtag("currently"):
             self.itemconfig(item, state = "normal")
 
     def open_cell(self, event = None, ignore_existing_editor = False):
         if not self.anything_selected() or (not ignore_existing_editor and self.text_editor_id is not None):
             return
         currently_selected = self.currently_selected()
         if not currently_selected:
@@ -4936,16 +4777,14 @@
             if text is None:
                 return False
             else:
                 text = text if isinstance(text, str) else f"{text}"
         text = "" if text is None else text
         if self.cell_auto_resize_enabled:
             self.set_cell_size_to_text(r, c, only_set_if_too_small = True, redraw = True, run_binding = True)
-        if not self.currently_selected():
-            self.select_cell(r = r, c = c, keep_other_selections = True)
             
         if (r, c) == self.text_editor_loc and self.text_editor is not None:
             self.text_editor.set_text(self.text_editor.get() + "" if not isinstance(text, str) else text)
             return
         if self.text_editor is not None:
             self.destroy_text_editor()
         if see:
@@ -5129,15 +4968,15 @@
                             new_c = c + 1
                             moved = True
                         if not moved:
                             if r + 1 == r2:
                                 new_r = r1
                             elif numrows > 1:
                                 new_r = r + 1
-                    self.create_current(new_r, new_c, type_ = currently_selected.type_, inside = True)
+                    self.set_currently_selected(new_r, new_c, type_ = currently_selected.type_)
                     self.see(new_r, new_c, keep_xscroll = False, bottom_right_corner = True, check_cell_visibility = True)
         self.close_dropdown_window(r, c)
         if recreate:
             self.recreate_all_selection_boxes()
         if redraw:
             self.refresh()
         if editor_info is not None and len(editor_info) >= 3 and editor_info[2] != "FocusOut":
@@ -5166,15 +5005,15 @@
                 new_c = c + 1
                 moved = True
             if not moved:
                 if r + 1 == r2:
                     new_r = r1
                 elif numrows > 1:
                     new_r = r + 1
-        self.create_current(new_r, new_c, type_ = currently_selected.type_, inside = True)
+        self.set_currently_selected(new_r, new_c, type_ = currently_selected.type_)
         self.see(new_r, new_c, keep_xscroll = False, bottom_right_corner = True, check_cell_visibility = True)
         return "break"
 
     #internal event use
     def set_cell_data_undo(self, r = 0, c = 0, datarn = None, datacn = None, value = "", undo = True, cell_resize = True, redraw = True, check_input_valid = True):
         if datacn is None:
             datacn = c if self.all_columns_displayed else self.displayed_columns[c]
@@ -5185,15 +5024,15 @@
                 self.undo_storage.append(zlib.compress(pickle.dumps(("edit_cells",
                                                                     {(datarn, datacn): self.get_cell_data(datarn, datacn)},
                                                                     self.get_boxes(include_current = False),
                                                                     self.currently_selected()))))
             self.set_cell_data(datarn, datacn, value)
         if cell_resize and self.cell_auto_resize_enabled:
             self.set_cell_size_to_text(r, c, only_set_if_too_small = True, redraw = redraw, run_binding = True)
-        self.parentframe.emit_modified_event()
+        self.parentframe.emit_event("<<SheetModified>>")
         return True
     
     def set_cell_data(self, datarn, datacn, value, kwargs = {}, expand_sheet = True):
         if expand_sheet:
             if datarn >= len(self.data):
                 self.fix_data_len(datarn, datacn)
             elif datacn >= len(self.data[datarn]):
```

### Comparing `tksheet-6.0.3/tksheet/_tksheet_other_classes.py` & `tksheet-6.0.4/tksheet/_tksheet_other_classes.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.0.3/tksheet/_tksheet_row_index.py` & `tksheet-6.0.4/tksheet/_tksheet_row_index.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,14 +197,16 @@
                 if not r_selected and self.row_selection_enabled:
                     self.add_selection(r, set_as_current = True)
                     self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
                     if self.ctrl_selection_binding_func is not None:
                         self.ctrl_selection_binding_func(SelectionBoxEvent("ctrl_select_rows", (r, r + 1)))
                 elif r_selected:
                     self.dragged_row = DraggedRowColumn(dragged = r, to_move = get_seq_without_gaps_at_index(sorted(self.MT.get_selected_rows()), r))
+        elif not self.MT.ctrl_select_enabled:
+            self.b1_press(event)
                     
     def ctrl_shift_b1_press(self, event):
         self.mouseclick_outside_editor_or_dropdown_all_canvases()
         y = event.y
         r = self.MT.identify_row(y = y)
         if (self.drag_and_drop_enabled or self.row_selection_enabled) and self.MT.ctrl_select_enabled and self.rsz_h is None and self.rsz_w is None:
             if r < len(self.MT.row_positions) - 1:
@@ -224,14 +226,16 @@
                         self.add_selection(r, set_as_current = True)
                         func_event = (r, )
                     self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
                     if self.ctrl_selection_binding_func is not None:
                         self.ctrl_selection_binding_func(SelectionBoxEvent("ctrl_select_rows", func_event))
                 elif r_selected:
                     self.dragged_row = DraggedRowColumn(dragged = r, to_move = get_seq_without_gaps_at_index(sorted(self.MT.get_selected_rows()), r))
+        elif not self.MT.ctrl_select_enabled:
+            self.shift_b1_press(event)
 
     def shift_b1_press(self, event):
         self.mouseclick_outside_editor_or_dropdown_all_canvases()
         y = event.y
         r = self.MT.identify_row(y = y)
         if (self.drag_and_drop_enabled or self.row_selection_enabled) and self.rsz_h is None and self.rsz_w is None:
             if r < len(self.MT.row_positions) - 1:
@@ -473,14 +477,16 @@
                         self.being_drawn_rect = rect
                         if self.drag_selection_binding_func is not None:
                             self.drag_selection_binding_func(SelectionBoxEvent("drag_select_rows", func_event))
             if self.scroll_if_event_offscreen(event):
                 need_redraw = True
             if need_redraw:
                 self.MT.main_table_redraw_grid_and_text(redraw_header = False, redraw_row_index = True)
+        elif not self.MT.ctrl_select_enabled:
+            self.b1_motion(event)
                 
     def drag_and_drop_motion(self, event):
         y = event.y
         hend = self.winfo_height()
         ycheck = self.yview()
         if y >= hend - 0 and len(ycheck) > 1 and ycheck[1] < 1:
             if y >= hend + 15:
@@ -622,15 +628,15 @@
                     if self.MT.undo_enabled:
                         self.MT.undo_storage.append(zlib.compress(pickle.dumps(("move_rows",
                                                                                 orig_selected,
                                                                                 new_selected))))
                     self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
                     if self.ri_extra_end_drag_drop_func is not None:
                         self.ri_extra_end_drag_drop_func(EndDragDropEvent("end_row_index_drag_drop", orig_selected, new_selected, int(r)))
-                    self.parentframe.emit_modified_event()
+                    self.parentframe.emit_event("<<SheetModified>>")
         elif self.b1_pressed_loc is not None and self.rsz_w is None and self.rsz_h is None:
             r = self.MT.identify_row(y = event.y)
             if r is not None and r < len(self.MT.row_positions) - 1 and r == self.b1_pressed_loc and self.b1_pressed_loc != self.closed_dropdown:
                 datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
                 canvasy = self.canvasy(event.y)
                 if self.event_over_dropdown(r, datarn, event, canvasy) or self.event_over_checkbox(r, datarn, event, canvasy):
                     self.open_cell(event)
@@ -658,48 +664,39 @@
                     del self.cell_options[r]['readonly']
         else:
             for r in rows_:
                 if r not in self.cell_options:
                     self.cell_options[r] = {}
                 self.cell_options[r]['readonly'] = True
 
-    def select_row(self, r, redraw = False, keep_other_selections = False):
-        if not keep_other_selections:
-            self.MT.delete_selection_rects()
-        self.MT.create_selected(r, 0, r + 1, len(self.MT.col_positions) - 1, "rows")
-        self.MT.create_current(r, 0, type_ = "row", inside = True)
-        if redraw:
-            self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
-        if self.selection_binding_func is not None:
-            self.selection_binding_func(SelectRowEvent("select_row", int(r)))
-
     def toggle_select_row(self, row, add_selection = True, redraw = True, run_binding_func = True, set_as_current = True):
         if add_selection:
             if self.MT.row_selected(row):
                 self.MT.deselect(r = row, redraw = redraw)
             else:
                 self.add_selection(r = row, redraw = redraw, run_binding_func = run_binding_func, set_as_current = set_as_current)
         else:
             if self.MT.row_selected(row):
                 self.MT.deselect(r = row, redraw = redraw)
             else:
                 self.select_row(row, redraw = redraw)
+                
+    def select_row(self, r, redraw = False):
+        self.MT.delete_selection_rects()
+        self.MT.create_selected(r, 0, r + 1, len(self.MT.col_positions) - 1, "rows")
+        self.MT.set_currently_selected(r, 0, type_ = "row")
+        if redraw:
+            self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
+        if self.selection_binding_func is not None:
+            self.selection_binding_func(SelectRowEvent("select_row", int(r)))
 
     def add_selection(self, r, redraw = False, run_binding_func = True, set_as_current = True):
         r = int(r)
         if set_as_current:
-            create_new_sel = False
-            current = self.MT.get_tags_of_current()
-            if current:
-                if current[0] == "Current_Outside":
-                    create_new_sel = True
-            self.MT.create_current(r, 0, type_ = "row", inside = True)
-            if create_new_sel:
-                r1, c1, r2, c2 = tuple(int(e) for e in current[1].split("_") if e)
-                self.MT.create_selected(r1, c1, r2, c2, current[2] + "s")
+            self.MT.set_currently_selected(r, 0, type_ = "row")
         self.MT.create_selected(r, 0, r + 1, len(self.MT.col_positions) - 1, "rows")
         if redraw:
             self.MT.main_table_redraw_grid_and_text(redraw_header = False, redraw_row_index = True)
         if self.selection_binding_func is not None and run_binding_func:
             self.selection_binding_func(("select_row", int(r)))
             
     def get_cell_dimensions(self, datarn):
@@ -873,25 +870,25 @@
             elif self.default_index == "both":
                 new_w = self.MT.get_txt_w(f"{end_row + 1} {num2alpha(end_row)}") + 20
                 if self.current_width - new_w > 15 or new_w - self.current_width > 5:
                     self.set_width(new_w, set_TL = True)
                     return True
         return False
 
-    def redraw_highlight_get_text_fg(self, fr, sr, r, c_2, c_3, selected_rows, selected_cols, actual_selected_rows, datarn):
+    def redraw_highlight_get_text_fg(self, fr, sr, r, c_2, c_3, selections, datarn):
         redrawn = False
         kwargs = self.get_cell_kwargs(datarn, key = 'highlight')
         if kwargs:
             if kwargs[0] is not None:
                 c_1 = kwargs[0] if kwargs[0].startswith("#") else Color_Map_[kwargs[0]]
-            if r in actual_selected_rows:
+            if 'rows' in selections and r in selections['rows']:
                 tf = self.index_selected_rows_fg if kwargs[1] is None or self.MT.display_selected_fg_over_highlights else kwargs[1]
                 if kwargs[0] is not None:
                     fill = f"#{int((int(c_1[1:3], 16) + int(c_3[1:3], 16)) / 2):02X}" + f"{int((int(c_1[3:5], 16) + int(c_3[3:5], 16)) / 2):02X}" + f"{int((int(c_1[5:], 16) + int(c_3[5:], 16)) / 2):02X}"
-            elif r in selected_rows or selected_cols:
+            elif 'cells' in selections and r in selections['cells']:
                 tf = self.index_selected_cells_fg if kwargs[1] is None or self.MT.display_selected_fg_over_highlights else kwargs[1]
                 if kwargs[0] is not None:
                     fill = f"#{int((int(c_1[1:3], 16) + int(c_2[1:3], 16)) / 2):02X}" + f"{int((int(c_1[3:5], 16) + int(c_2[3:5], 16)) / 2):02X}" + f"{int((int(c_1[5:], 16) + int(c_2[5:], 16)) / 2):02X}"
             else:
                 tf = self.index_fg if kwargs[1] is None else kwargs[1]
                 if kwargs[0] is not None:
                     fill = kwargs[0]
@@ -900,17 +897,17 @@
                                                 fr + 1,
                                                 self.current_width - 1,
                                                 sr,
                                                 fill = fill,
                                                 outline = self.index_fg if self.get_cell_kwargs(datarn, key = 'dropdown') and self.MT.show_dropdown_borders else "",
                                                 tag = "s")
         elif not kwargs:
-            if r in actual_selected_rows:
+            if 'rows' in selections and r in selections['rows']:
                 tf = self.index_selected_rows_fg
-            elif r in selected_rows or selected_cols:
+            elif 'cells' in selections and r in selections['cells']:
                 tf = self.index_selected_cells_fg
             else:
                 tf = self.index_fg
         return tf, redrawn
 
     def redraw_highlight(self, x1, y1, x2, y2, fill, outline, tag):
         config = (fill, outline)
@@ -1026,15 +1023,15 @@
                 else:
                     self.itemconfig(t, fill = fill, outline = outline, tag = tag, state = "normal")
                 self.lift(t)
             else:
                 t = self.create_polygon(points, fill = fill, outline = outline, tag = tag, smooth = True)
             self.disp_checkbox[t] = True
 
-    def redraw_grid_and_text(self, last_row_line_pos, scrollpos_top, y_stop, start_row, end_row, scrollpos_bot, selected_rows, selected_cols, actual_selected_rows, row_pos_exists):
+    def redraw_grid_and_text(self, last_row_line_pos, scrollpos_top, y_stop, start_row, end_row, scrollpos_bot, row_pos_exists):
         try:
             self.configure(scrollregion = (0,
                                            0,
                                            self.current_width,
                                            last_row_line_pos + self.MT.empty_vertical))
         except:
             return
@@ -1079,21 +1076,22 @@
                                    -1, draw_y,
                                    -1, self.MT.row_positions[r + 1] if len(self.MT.row_positions) - 1 > r else draw_y])
                 if points:
                     self.redraw_gridline(points = points, fill = self.index_grid_fg, width = 1, tag = "h")
         c_2 = self.index_selected_cells_bg if self.index_selected_cells_bg.startswith("#") else Color_Map_[self.index_selected_cells_bg]
         c_3 = self.index_selected_rows_bg if self.index_selected_rows_bg.startswith("#") else Color_Map_[self.index_selected_rows_bg]
         font = self.MT.index_font
+        selections = self.get_redraw_selections(start_row, end_row)
         for r in range(start_row, end_row - 1):
             rtopgridln = self.MT.row_positions[r]
             rbotgridln = self.MT.row_positions[r + 1]
             if rbotgridln - rtopgridln < self.MT.txt_h:
                 continue
             datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
-            fill, dd_drawn = self.redraw_highlight_get_text_fg(rtopgridln, rbotgridln, r, c_2, c_3, selected_rows, selected_cols, actual_selected_rows, datarn)
+            fill, dd_drawn = self.redraw_highlight_get_text_fg(rtopgridln, rbotgridln, r, c_2, c_3, selections, datarn)
             
             if datarn in self.cell_options and 'align' in self.cell_options[datarn]:
                 align = self.cell_options[datarn]['align']
             else:
                 align = self.align
             dropdown_kwargs = self.get_cell_kwargs(datarn, key = 'dropdown')
             if align == "w":
@@ -1173,23 +1171,25 @@
                             iid, showing = self.hidd_text[k].pop()
                             cc1, cc2 = self.coords(iid)
                             if (int(cc1) == int(draw_x) and
                                 int(cc2) == int(draw_y)):
                                 option = 0 if showing else 2
                             else:
                                 option = 1 if showing else 3
+                            self.tag_raise(iid)
                         elif self.hidd_text:
                             k = next(iter(self.hidd_text))
                             iid, showing = self.hidd_text[k].pop()
                             cc1, cc2 = self.coords(iid)
                             if (int(cc1) == int(draw_x) and
                                 int(cc2) == int(draw_y)):
                                 option = 2 if showing else 3
                             else:
                                 option = 3
+                            self.tag_raise(iid)
                         else:
                             iid, showing, option = self.create_text(draw_x, draw_y, text = txt, fill = fill, font = font, anchor = align, tag = "t"), 1, 4
                         if option in (1, 3):
                             self.coords(iid, draw_x, draw_y)
                         if option in (2, 3):
                             if showing:
                                 self.itemconfig(iid, text = txt, fill = fill, font = font, anchor = align)
@@ -1229,15 +1229,14 @@
                                 self.coords(iid, draw_x, draw_y)
                             self.disp_text[config._replace(txt = txt)].add(DrawnItem(iid = iid, showing = True))
                         else:
                             self.disp_text[config].add(DrawnItem(iid = iid, showing = True))
                         draw_y += self.MT.xtra_lines_increment
                         if draw_y + self.MT.half_txt_h - 1 > rbotgridln:
                             break
-        self.tag_raise("t")
         for cfg, set_ in self.hidd_text.items():
             for namedtup in tuple(set_):
                 if namedtup.showing:
                     self.itemconfig(namedtup.iid, state = "hidden")
                     self.hidd_text[cfg].discard(namedtup)
                     self.hidd_text[cfg].add(namedtup._replace(showing = False))
         for cfg, set_ in self.hidd_high.items():
@@ -1254,14 +1253,26 @@
             if sh:
                 self.itemconfig(t, state = "hidden")
                 self.hidd_dropdown[t] = False
         for t, sh in self.hidd_checkbox.items():
             if sh:
                 self.itemconfig(t, state = "hidden")
                 self.hidd_checkbox[t] = False
+    
+    def get_redraw_selections(self, startr, endr):
+        d = defaultdict(list)
+        for item in chain(self.find_withtag("cells"), self.find_withtag("rows")):
+            tags = self.gettags(item)
+            d[tags[0]].append(tuple(int(e) for e in tags[1].split("_") if e))
+        d2 = {}
+        if 'cells' in d:
+            d2['cells'] = {r for r in range(startr, endr) for r1, c1, r2, c2 in d['cells'] if r1 <= r and r2 > r}
+        if 'rows' in d:
+            d2['rows'] = {r for r in range(startr, endr) for r1, c1, r2, c2 in d['rows'] if r1 <= r and r2 > r}
+        return d2
                 
     def open_cell(self, event = None, ignore_existing_editor = False):
         if not self.MT.anything_selected() or (not ignore_existing_editor and self.text_editor_id is not None):
             return
         currently_selected = self.MT.currently_selected()
         if not currently_selected:
             return
@@ -1327,15 +1338,14 @@
             if text is None:
                 return False
             else:
                 text = text if isinstance(text, str) else f"{text}"
         text = "" if text is None else text
         if self.MT.cell_auto_resize_enabled:
             self.set_row_height_run_binding(r)
-        self.select_row(r = r, keep_other_selections = True, redraw = not dropdown)
         
         if r == self.text_editor_loc and self.text_editor is not None:
             self.text_editor.set_text(self.text_editor.get() + "" if not isinstance(text, str) else text)
             return
         if self.text_editor is not None:
             self.destroy_text_editor()
         if see:
@@ -1511,15 +1521,15 @@
                                                                             self.MT.get_boxes(include_current = False),
                                                                             self.MT.currently_selected()))))
                 self.set_cell_data(datarn = datarn, value = value)
         if cell_resize and self.MT.cell_auto_resize_enabled:
             self.set_row_height_run_binding(r, only_set_if_too_small = False)
         if redraw:
             self.MT.refresh()
-        self.parentframe.emit_modified_event()
+        self.parentframe.emit_event("<<SheetModified>>")
 
     def set_cell_data(self, datarn = None, value = ""):
         if isinstance(self.MT._row_index, int):
             self.MT.set_cell_data(datarn = datarn, datacn = self.MT._row_index, value = value)
         else:
             self.fix_index(datarn)
             if self.get_cell_kwargs(datarn, key = 'checkbox'):
```

### Comparing `tksheet-6.0.3/tksheet/_tksheet_top_left_rectangle.py` & `tksheet-6.0.4/tksheet/_tksheet_top_left_rectangle.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,18 +110,18 @@
             if self.MT.select_all_enabled:
                 self.MT.deselect("all")
                 self.MT.select_all()
             else:
                 self.MT.deselect("all")
         elif rect[0] == 1:
             if self.RI.width_resizing_enabled:
-                self.RI.set_width(self.RI.default_index_width, set_TL = True)
+                self.RI.set_width(self.MT.default_index_width, set_TL = True)
         elif rect[0] == 2:
             if self.CH.height_resizing_enabled:
-                self.CH.set_height(self.MT.default_header_h[1], set_TL = True)
+                self.CH.set_height(self.MT.default_header_height[1], set_TL = True)
         self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
         if self.extra_b1_press_func is not None:
             self.extra_b1_press_func(event)
 
     def b1_motion(self, event = None):
         self.focus_set()
         if self.extra_b1_motion_func is not None:
```

### Comparing `tksheet-6.0.3/tksheet/_tksheet_vars.py` & `tksheet-6.0.4/tksheet/_tksheet_vars.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 arrowkey_bindings_helper = {"tab": "Tab",
                             "up": "Up",
                             "right": "Right",
                             "left": "Left",
                             "down": "Down",
                             "prior": "Prior",
                             "next": "Next"}
-emitted_events = {"<<SheetModified>>", }
+emitted_events = {"<<SheetModified>>", "<<SheetRedrawn>>", }
 
 def get_font():
     return ("Calibri", 13 if USER_OS == "darwin" else 11, "normal")
 
 def get_index_font():
     return ('Calibri', 13 if USER_OS == "darwin" else 11, "normal")
```

### Comparing `tksheet-6.0.3/tksheet.egg-info/PKG-INFO` & `tksheet-6.0.4/tksheet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tksheet
-Version: 6.0.3
+Version: 6.0.4
 Summary: Tkinter table / sheet widget
 Home-page: https://github.com/ragardner/tksheet
-Download-URL: https://github.com/ragardner/tksheet/archive/6.0.3.tar.gz
+Download-URL: https://github.com/ragardner/tksheet/archive/6.0.4.tar.gz
 Author: ragardner
 Author-email: github@ragardner.simplelogin.com
 License: MIT
 Keywords: tkinter,table,widget,sheet,grid,tk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

