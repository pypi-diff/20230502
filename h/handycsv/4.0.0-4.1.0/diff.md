# Comparing `tmp/handycsv-4.0.0.tar.gz` & `tmp/handycsv-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/nic/dev/handycsv/dist/tmpfk6oam7r/handycsv-4.0.0.tar", last modified: Thu Mar 25 20:52:34 2021, max compression
+gzip compressed data, was "handycsv-4.1.0.tar", last modified: Tue May  2 05:00:42 2023, max compression
```

## Comparing `handycsv-4.0.0.tar` & `handycsv-4.1.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-x---   0 nic       (1000) nic       (1000)        0 2021-03-25 20:52:34.159558 handycsv-4.0.0/
--rw-r-----   0 nic       (1000) nic       (1000)      234 2021-03-25 20:52:34.159558 handycsv-4.0.0/PKG-INFO
--rw-r-----   0 nic       (1000) nic       (1000)       79 2021-03-25 20:49:50.000000 handycsv-4.0.0/README.md
-drwxr-x---   0 nic       (1000) nic       (1000)        0 2021-03-25 20:52:34.159558 handycsv-4.0.0/handycsv/
--rw-r-----   0 nic       (1000) nic       (1000)     1719 2021-03-25 20:50:03.000000 handycsv-4.0.0/handycsv/__init__.py
--rw-r-----   0 nic       (1000) nic       (1000)     6645 2021-03-25 20:50:20.000000 handycsv-4.0.0/handycsv/column_stats.py
--rw-r-----   0 nic       (1000) nic       (1000)    10700 2021-03-25 20:48:20.000000 handycsv-4.0.0/handycsv/csv.py
--rw-r-----   0 nic       (1000) nic       (1000)     8619 2021-03-25 20:50:12.000000 handycsv-4.0.0/handycsv/grid_stats.py
-drwxr-x---   0 nic       (1000) nic       (1000)        0 2021-03-25 20:52:34.159558 handycsv-4.0.0/handycsv.egg-info/
--rw-r-----   0 nic       (1000) nic       (1000)      234 2021-03-25 20:52:34.000000 handycsv-4.0.0/handycsv.egg-info/PKG-INFO
--rw-r-----   0 nic       (1000) nic       (1000)      296 2021-03-25 20:52:34.000000 handycsv-4.0.0/handycsv.egg-info/SOURCES.txt
--rw-r-----   0 nic       (1000) nic       (1000)        1 2021-03-25 20:52:34.000000 handycsv-4.0.0/handycsv.egg-info/dependency_links.txt
--rw-r-----   0 nic       (1000) nic       (1000)        9 2021-03-25 20:52:34.000000 handycsv-4.0.0/handycsv.egg-info/top_level.txt
--rw-r-----   0 nic       (1000) nic       (1000)       38 2021-03-25 20:52:34.159558 handycsv-4.0.0/setup.cfg
--rw-r-----   0 nic       (1000) nic       (1000)     2473 2021-03-25 20:51:28.000000 handycsv-4.0.0/setup.py
-drwxr-x---   0 nic       (1000) nic       (1000)        0 2021-03-25 20:52:34.159558 handycsv-4.0.0/test/
--rw-r-----   0 nic       (1000) nic       (1000)     4215 2021-03-25 20:49:19.000000 handycsv-4.0.0/test/test_columnstats.py
--rw-r-----   0 nic       (1000) nic       (1000)    13733 2021-03-25 20:49:19.000000 handycsv-4.0.0/test/test_csv.py
--rw-r-----   0 nic       (1000) nic       (1000)     6377 2021-03-25 20:49:19.000000 handycsv-4.0.0/test/test_gridstats.py
+drwxr-x---   0 nic       (1000) nic       (1000)        0 2023-05-02 05:00:42.370126 handycsv-4.1.0/
+-rw-r-----   0 nic       (1000) nic       (1000)     1525 2023-05-02 02:28:44.000000 handycsv-4.1.0/LICENSE
+-rw-r-----   0 nic       (1000) nic       (1000)      131 2023-05-02 02:28:44.000000 handycsv-4.1.0/NOTICE
+-rw-r-----   0 nic       (1000) nic       (1000)      238 2023-05-02 05:00:42.370126 handycsv-4.1.0/PKG-INFO
+-rw-r-----   0 nic       (1000) nic       (1000)       79 2023-05-02 02:28:44.000000 handycsv-4.1.0/README.md
+drwxr-x---   0 nic       (1000) nic       (1000)        0 2023-05-02 05:00:42.370126 handycsv-4.1.0/handycsv/
+-rw-r-----   0 nic       (1000) nic       (1000)     1719 2023-05-02 04:58:54.000000 handycsv-4.1.0/handycsv/__init__.py
+-rw-r-----   0 nic       (1000) nic       (1000)     7010 2023-05-02 04:57:39.000000 handycsv-4.1.0/handycsv/column_stats.py
+-rw-r-----   0 nic       (1000) nic       (1000)    11533 2023-05-02 04:30:57.000000 handycsv-4.1.0/handycsv/csv.py
+-rw-r-----   0 nic       (1000) nic       (1000)    10029 2023-05-02 04:52:54.000000 handycsv-4.1.0/handycsv/grid_stats.py
+drwxr-x---   0 nic       (1000) nic       (1000)        0 2023-05-02 05:00:42.370126 handycsv-4.1.0/handycsv.egg-info/
+-rw-r-----   0 nic       (1000) nic       (1000)      238 2023-05-02 05:00:42.000000 handycsv-4.1.0/handycsv.egg-info/PKG-INFO
+-rw-r-----   0 nic       (1000) nic       (1000)      311 2023-05-02 05:00:42.000000 handycsv-4.1.0/handycsv.egg-info/SOURCES.txt
+-rw-r-----   0 nic       (1000) nic       (1000)        1 2023-05-02 05:00:42.000000 handycsv-4.1.0/handycsv.egg-info/dependency_links.txt
+-rw-r-----   0 nic       (1000) nic       (1000)        9 2023-05-02 05:00:42.000000 handycsv-4.1.0/handycsv.egg-info/top_level.txt
+-rw-r-----   0 nic       (1000) nic       (1000)       38 2023-05-02 05:00:42.370126 handycsv-4.1.0/setup.cfg
+-rw-r-----   0 nic       (1000) nic       (1000)     2473 2023-05-02 02:28:44.000000 handycsv-4.1.0/setup.py
+drwxr-x---   0 nic       (1000) nic       (1000)        0 2023-05-02 05:00:42.370126 handycsv-4.1.0/test/
+-rw-r-----   0 nic       (1000) nic       (1000)     4541 2023-05-02 04:58:28.000000 handycsv-4.1.0/test/test_columnstats.py
+-rw-r-----   0 nic       (1000) nic       (1000)    15035 2023-05-02 04:32:57.000000 handycsv-4.1.0/test/test_csv.py
+-rw-r-----   0 nic       (1000) nic       (1000)     7784 2023-05-02 04:54:07.000000 handycsv-4.1.0/test/test_gridstats.py
```

### Comparing `handycsv-4.0.0/handycsv/__init__.py` & `handycsv-4.1.0/handycsv/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,8 +29,8 @@
  * POSSIBILITY OF SUCH DAMAGE.
 """
 
 from .column_stats import ColumnStats
 from .csv import Csv
 from .grid_stats import GridStats
 
-__version__ = '4.0.0'
+__version__ = '4.1.0'
```

### Comparing `handycsv-4.0.0/handycsv/column_stats.py` & `handycsv-4.1.0/handycsv/column_stats.py`

 * *Files 4% similar despite different names*

```diff
@@ -197,14 +197,28 @@
     try:
       row_index = self.row_index[row]
     except KeyError:
       raise IndexError('row={0} doesn\'t exist'.format(row))
     self.csv.remove_row(row_index)
     self.__init_row_info()
 
+  def add_row(self, name, value, index):
+    """
+    This adds the specified row.
+
+    Args:
+      name (str)    : the name of the row
+      value (value) : the value of the row
+    """
+    if name in self.row_names():
+      raise ValueError(f'row {name} already exists')
+    new_row = [name, value]
+    self.csv.add_row(new_row, index)
+    self.__init_row_info()
+
   def filter_rows(self, regex, invert=False):
     """
     This filter the data into a subset. It removes rows wherein the value
     matches the specified regular expression. If invert is False only the
     matching rows will be retained. If invert is True only the non matching
     rows will be retained.
```

### Comparing `handycsv-4.0.0/handycsv/csv.py` & `handycsv-4.1.0/handycsv/csv.py`

 * *Files 4% similar despite different names*

```diff
@@ -313,14 +313,44 @@
       if len(self.raw[row]) == 1:
         raise IndexError('row {} only has one element, '
                          'removing the column would make an empty row'
                          .format(row))
     for row in range(self.num_rows()):
       self.raw[row].pop(column)
 
+  def add_row(self, row, index):
+    """
+    This adds a row at the specified index.
+
+    Args:
+      row   ([values]) : the new row contents
+      index (int)      : the new row's index
+    """
+    new_row = []
+    for cell in row:
+      new_row.append(cell)
+    self.raw.insert(index, new_row)
+
+  def add_column(self, column, index):
+    """
+    This adds a column at the specified index.
+
+    Args:
+      column ([values]) : the new column contents
+      index  (int)      : the new column's index
+    """
+    if len(column) != self.num_rows():
+      raise ValueError('The length of column must match the current number of '
+                       'rows')
+    new_col = []
+    for cell in column:
+      new_col.append(cell)
+    for row_index in range(self.num_rows()):
+      self.raw[row_index].insert(index, new_col[row_index])
+
   def is_rectangular(self):
     """
     Return True iff the Csv is rectangular.
     This tests that all rows are equal length
     """
     return len(set(self.row_lengths())) == 1
```

### Comparing `handycsv-4.0.0/handycsv/grid_stats.py` & `handycsv-4.1.0/handycsv/grid_stats.py`

 * *Files 11% similar despite different names*

```diff
@@ -252,18 +252,68 @@
 
     Args:
       row (str) : the row identifier
     """
     try:
       row_index = self.row_index[row]
     except KeyError:
-      raise IndexError('row={0} doesn\'t exist'.format(row))
+      raise IndexError(f'row={row} doesn\'t exist')
     self.csv.remove_row(row_index)
     self.__init_row_info()
 
+  def remove_column(self, column):
+    """
+    This removes the specified column.
+
+    Args
+      column (str) : the column identifier
+    """
+    try:
+      column_index = self.column_index[column]
+    except KeyError:
+      raise IndexError(f'column={column} doesn\'t exist')
+    self.csv.remove_column(column_index)
+    self.__init_column_info()
+
+  def add_row(self, name, columns, index):
+    """
+    This adds a new row the the grid.
+
+    Args:
+      name    (str)      : the name of the row
+      columns ([values]) : dict of column values
+      index   (int)      : placement of row
+    """
+    if name in self.row_names():
+      raise ValueError(f'row {name} already exists')
+    new_row = [name]
+    for column in self.column_names():
+      new_row.append(columns[column])
+    self.csv.add_row(new_row, index + 1)
+    self.__init_row_info()
+    self.__init_column_info()
+
+  def add_column(self, name, rows, index):
+    """
+    This adds a new columns the the grid.
+
+    Args:
+      name  (str)      : the name of the colu,n
+      rows  ([values]) : dict of row values
+      index (int)      : placement of column
+    """
+    if name in self.column_names():
+      raise ValueError(f'column {name} already exists')
+    new_column = [name]
+    for row in self.row_names():
+      new_column.append(rows[row])
+    self.csv.add_column(new_column, index + 1)
+    self.__init_row_info()
+    self.__init_column_info()
+
   def filter_rows(self, column, regex, invert=False):
     """
     This filter the data into a subset. It removes rows wherein the value of the
     identified column matches the specified regular expression. If invert is
     False only the matching rows will be retained. If invert is True only the
     non matching rows will be retained.
```

### Comparing `handycsv-4.0.0/setup.py` & `handycsv-4.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `handycsv-4.0.0/test/test_columnstats.py` & `handycsv-4.1.0/test/test_columnstats.py`

 * *Files 9% similar despite different names*

```diff
@@ -115,7 +115,15 @@
       self.assertEqual(stats, newstats)
 
       os.remove(csvfile1)
 
     skeleton = handycsv.ColumnStats.create(['-', 'd', 'e', 'f'])
     stats = handycsv.ColumnStats.load(text)
     self.assertEqual(skeleton.row_names(), stats.row_names())
+
+    skeleton = handycsv.ColumnStats.create(['-', 'd', 'e', 'g', 'f'])
+    stats = handycsv.ColumnStats.load(text)
+    stats.add_row('g', 7, 3)
+    self.assertEqual(skeleton.row_names(), stats.row_names())
+    self.assertEqual(stats.get('g'), 7)
+    self.assertEqual(stats.get('e'), 3)
+    self.assertEqual(stats.get('f'), 6)
```

### Comparing `handycsv-4.0.0/test/test_csv.py` & `handycsv-4.1.0/test/test_csv.py`

 * *Files 6% similar despite different names*

```diff
@@ -481,7 +481,53 @@
     self.assertEqual(csv.pretty(5), exp)
 
     exp = (
       '  hello         89\n'
       '              why?\n'
       '0.33333 1234.10000 bye\n')
     self.assertEqual(csv.pretty(5, True), exp)
+
+  def test_add_row(self):
+    csv = handycsv.Csv([2, 1, 3])
+    csv.set(0, 0, 'd')
+    csv.set(0, 1, 0)
+    csv.set(1, 0, '5')
+    csv.set(2, 0, 'e')
+    csv.set(2, 1, 3)
+    csv.set(2, 2, 4)
+
+    self.assertEqual(csv.num_rows(), 3)
+
+    csv.add_row(['z', 5, 'y', 9], 2)
+
+    self.assertEqual(csv.num_rows(), 4)
+    self.assertEqual(csv.row_lengths(), [2, 1, 4, 3])
+    self.assertEqual(csv.get(2, 0), 'z')
+    self.assertEqual(csv.get(2, 1), 5)
+    self.assertEqual(csv.get(2, 2), 'y')
+    self.assertEqual(csv.get(2, 3), 9)
+    self.assertEqual(csv.get(1, 0), '5')
+    self.assertEqual(csv.get(3, 0), 'e')
+    self.assertEqual(csv.get(3, 1), 3)
+    self.assertEqual(csv.get(3, 2), 4)
+
+  def test_add_column(self):
+    csv = handycsv.Csv([2, 1, 3])
+    csv.set(0, 0, 'd')
+    csv.set(0, 1, 0)
+    csv.set(1, 0, '5')
+    csv.set(2, 0, 'e')
+    csv.set(2, 1, 3)
+    csv.set(2, 2, 4)
+
+    self.assertEqual(csv.num_rows(), 3)
+
+    csv.add_column(['x', 'y', 'z'], 0)
+
+    self.assertEqual(csv.num_rows(), 3)
+    self.assertEqual(csv.row_lengths(), [3, 2, 4])
+    self.assertEqual(csv.get(0, 0), 'x')
+    self.assertEqual(csv.get(1, 0), 'y')
+    self.assertEqual(csv.get(2, 0), 'z')
+    self.assertEqual(csv.get(0, 1), 'd')
+    self.assertEqual(csv.get(1, 1), '5')
+    self.assertEqual(csv.get(2, 1), 'e')
```

### Comparing `handycsv-4.0.0/test/test_gridstats.py` & `handycsv-4.1.0/test/test_gridstats.py`

 * *Files 22% similar despite different names*

```diff
@@ -48,15 +48,15 @@
   k4x4 = [
     ['-', 'a', 'b', 'c'],
     ['d', 0, 1, 2],
     ['e', 3, 4, 5],
     ['f', 6, 7, 8]
   ]
 
-  def test_handy(self):
+  def test_grid(self):
     text = TestGridStats.make_str(TestGridStats.k4x4)
 
     stats = handycsv.GridStats.load(text)
     self.assertEqual(stats.row_names(), ['d', 'e', 'f'])
     self.assertEqual(stats.column_names(), ['a', 'b', 'c'])
     self.assertEqual(stats.get('d', 'c'), 2)
     self.assertEqual(stats.get('f', 'b'), 7)
@@ -165,7 +165,36 @@
       os.remove(csvfile2)
 
     skeleton = handycsv.GridStats.create('-', ['d', 'e', 'f'], ['a', 'b', 'c'])
     stats = handycsv.GridStats.load(text)
     self.assertEqual(skeleton.head(), stats.head())
     self.assertEqual(skeleton.row_names(), stats.row_names())
     self.assertEqual(skeleton.column_names(), stats.column_names())
+
+    skeleton = handycsv.GridStats.create('-', ['d', 'e', 'f'], ['b', 'c'])
+    stats = handycsv.GridStats.load(text)
+    stats.remove_column('a')
+    self.assertEqual(skeleton.head(), stats.head())
+    self.assertEqual(skeleton.row_names(), stats.row_names())
+    self.assertEqual(skeleton.column_names(), stats.column_names())
+
+    stats = handycsv.GridStats.load(text)
+    stats.add_row('g', {'a': 9, 'b': 8, 'c': 7}, 1)
+    skeleton = handycsv.GridStats.create('-', ['d', 'g', 'e', 'f'],
+                                         ['a', 'b', 'c'])
+    self.assertEqual(skeleton.head(), stats.head())
+    self.assertEqual(skeleton.row_names(), stats.row_names())
+    self.assertEqual(skeleton.column_names(), stats.column_names())
+    self.assertEqual(stats.get('g', 'b'), 8)
+    self.assertEqual(stats.get('d', 'b'), 1)
+    self.assertEqual(stats.get('e', 'b'), 4)
+
+    stats = handycsv.GridStats.load(text)
+    stats.add_column('z', {'d': 9, 'e': 8, 'f': 7}, 3)
+    skeleton = handycsv.GridStats.create('-', ['d', 'e', 'f'],
+                                         ['a', 'b', 'c', 'z'])
+    self.assertEqual(skeleton.head(), stats.head())
+    self.assertEqual(skeleton.row_names(), stats.row_names())
+    self.assertEqual(skeleton.column_names(), stats.column_names())
+    self.assertEqual(stats.get('d', 'z'), 9)
+    self.assertEqual(stats.get('d', 'a'), 0)
+    self.assertEqual(stats.get('d', 'c'), 2)
```

