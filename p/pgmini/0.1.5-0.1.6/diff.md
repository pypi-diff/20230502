# Comparing `tmp/pgmini-0.1.5.tar.gz` & `tmp/pgmini-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgmini-0.1.5.tar", max compression
+gzip compressed data, was "pgmini-0.1.6.tar", max compression
```

## Comparing `pgmini-0.1.5.tar` & `pgmini-0.1.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1461 2023-02-19 07:19:37.209313 pgmini-0.1.5/LICENSE
--rw-r--r--   0        0        0     7773 2023-04-03 05:59:48.504852 pgmini-0.1.5/README.md
--rw-r--r--   0        0        0     2259 2023-05-01 05:08:31.710026 pgmini-0.1.5/pgmini/__init__.py
--rw-r--r--   0        0        0      614 2023-02-24 08:44:04.617355 pgmini-0.1.5/pgmini/alias.py
--rw-r--r--   0        0        0      811 2023-05-01 05:08:02.585539 pgmini-0.1.5/pgmini/array.py
--rw-r--r--   0        0        0     1861 2023-05-01 05:08:02.603966 pgmini-0.1.5/pgmini/case.py
--rw-r--r--   0        0        0      946 2023-05-01 05:08:50.018185 pgmini-0.1.5/pgmini/cast.py
--rw-r--r--   0        0        0     1670 2023-05-01 05:08:02.579642 pgmini-0.1.5/pgmini/column.py
--rw-r--r--   0        0        0     1547 2023-05-01 05:08:02.600431 pgmini-0.1.5/pgmini/delete.py
--rw-r--r--   0        0        0      272 2023-02-23 06:15:18.337495 pgmini-0.1.5/pgmini/distinct.py
--rw-r--r--   0        0        0     4365 2023-05-01 05:08:02.612565 pgmini-0.1.5/pgmini/func.py
--rw-r--r--   0        0        0     6743 2023-05-01 05:08:02.596689 pgmini-0.1.5/pgmini/insert.py
--rw-r--r--   0        0        0     2025 2023-05-01 05:08:02.588339 pgmini-0.1.5/pgmini/literal.py
--rw-r--r--   0        0        0     2010 2023-02-27 06:30:22.659219 pgmini-0.1.5/pgmini/marks.py
--rw-r--r--   0        0        0     2687 2023-02-23 06:15:18.320773 pgmini-0.1.5/pgmini/operation.py
--rw-r--r--   0        0        0     6954 2023-05-01 05:08:16.877681 pgmini-0.1.5/pgmini/operations.py
--rw-r--r--   0        0        0     2850 2023-05-01 05:08:02.582903 pgmini-0.1.5/pgmini/operators.py
--rw-r--r--   0        0        0     1616 2023-02-24 08:44:04.622843 pgmini-0.1.5/pgmini/order_by.py
--rw-r--r--   0        0        0     1184 2023-05-01 05:01:36.361544 pgmini-0.1.5/pgmini/param.py
--rw-r--r--   0        0        0     9462 2023-05-01 05:08:02.592762 pgmini-0.1.5/pgmini/select.py
--rw-r--r--   0        0        0     1718 2023-05-01 05:08:02.571006 pgmini-0.1.5/pgmini/subquery.py
--rw-r--r--   0        0        0     1134 2023-02-23 09:40:15.343020 pgmini-0.1.5/pgmini/table.py
--rw-r--r--   0        0        0     2583 2023-05-01 05:08:02.615662 pgmini-0.1.5/pgmini/update.py
--rw-r--r--   0        0        0     2896 2023-05-01 05:08:02.607073 pgmini-0.1.5/pgmini/utils.py
--rw-r--r--   0        0        0      901 2023-05-01 05:08:41.372640 pgmini-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     8815 1970-01-01 00:00:00.000000 pgmini-0.1.5/setup.py
--rw-r--r--   0        0        0     8238 1970-01-01 00:00:00.000000 pgmini-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1461 2023-02-19 07:19:37.209313 pgmini-0.1.6/LICENSE
+-rw-r--r--   0        0        0     7773 2023-04-03 05:59:48.504852 pgmini-0.1.6/README.md
+-rw-r--r--   0        0        0     2259 2023-05-02 12:44:45.058854 pgmini-0.1.6/pgmini/__init__.py
+-rw-r--r--   0        0        0      614 2023-02-24 08:44:04.617355 pgmini-0.1.6/pgmini/alias.py
+-rw-r--r--   0        0        0      811 2023-05-01 05:08:02.585539 pgmini-0.1.6/pgmini/array.py
+-rw-r--r--   0        0        0     1861 2023-05-01 05:08:02.603966 pgmini-0.1.6/pgmini/case.py
+-rw-r--r--   0        0        0      946 2023-05-01 05:08:50.018185 pgmini-0.1.6/pgmini/cast.py
+-rw-r--r--   0        0        0     1670 2023-05-01 05:08:02.579642 pgmini-0.1.6/pgmini/column.py
+-rw-r--r--   0        0        0     1547 2023-05-01 05:08:02.600431 pgmini-0.1.6/pgmini/delete.py
+-rw-r--r--   0        0        0      272 2023-02-23 06:15:18.337495 pgmini-0.1.6/pgmini/distinct.py
+-rw-r--r--   0        0        0     4365 2023-05-01 05:08:02.612565 pgmini-0.1.6/pgmini/func.py
+-rw-r--r--   0        0        0     6743 2023-05-01 05:08:02.596689 pgmini-0.1.6/pgmini/insert.py
+-rw-r--r--   0        0        0     2025 2023-05-01 05:08:02.588339 pgmini-0.1.6/pgmini/literal.py
+-rw-r--r--   0        0        0     2010 2023-02-27 06:30:22.659219 pgmini-0.1.6/pgmini/marks.py
+-rw-r--r--   0        0        0     2950 2023-05-02 12:32:18.326618 pgmini-0.1.6/pgmini/operation.py
+-rw-r--r--   0        0        0     8233 2023-05-02 12:45:39.641005 pgmini-0.1.6/pgmini/operations.py
+-rw-r--r--   0        0        0     2850 2023-05-01 05:08:02.582903 pgmini-0.1.6/pgmini/operators.py
+-rw-r--r--   0        0        0     1616 2023-02-24 08:44:04.622843 pgmini-0.1.6/pgmini/order_by.py
+-rw-r--r--   0        0        0     1184 2023-05-01 05:01:36.361544 pgmini-0.1.6/pgmini/param.py
+-rw-r--r--   0        0        0     9462 2023-05-01 05:08:02.592762 pgmini-0.1.6/pgmini/select.py
+-rw-r--r--   0        0        0     1718 2023-05-01 05:08:02.571006 pgmini-0.1.6/pgmini/subquery.py
+-rw-r--r--   0        0        0     1134 2023-02-23 09:40:15.343020 pgmini-0.1.6/pgmini/table.py
+-rw-r--r--   0        0        0     2583 2023-05-01 05:08:02.615662 pgmini-0.1.6/pgmini/update.py
+-rw-r--r--   0        0        0     2896 2023-05-01 05:08:02.607073 pgmini-0.1.6/pgmini/utils.py
+-rw-r--r--   0        0        0      901 2023-05-02 12:44:50.639051 pgmini-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     8815 1970-01-01 00:00:00.000000 pgmini-0.1.6/setup.py
+-rw-r--r--   0        0        0     8238 1970-01-01 00:00:00.000000 pgmini-0.1.6/PKG-INFO
```

### Comparing `pgmini-0.1.5/LICENSE` & `pgmini-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pgmini-0.1.5/README.md` & `pgmini-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pgmini-0.1.5/pgmini/__init__.py` & `pgmini-0.1.6/pgmini/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     CTX_DISABLE_TABLE_IN_COLUMN,
     CTX_FORCE_CAST_BRACKETS,
     CTX_TABLES,
     CompileABC,
 )
 
 
-__version__ = '0.1.5'
+__version__ = '0.1.6'
 __all__ = (
     'And',
     'Array',
     'Case',
     'Delete',
     'Excluded',
     'Exists',
```

### Comparing `pgmini-0.1.5/pgmini/alias.py` & `pgmini-0.1.6/pgmini/alias.py`

 * *Files identical despite different names*

### Comparing `pgmini-0.1.5/pgmini/array.py` & `pgmini-0.1.6/pgmini/array.py`

 * *Files identical despite different names*

### Comparing `pgmini-0.1.5/pgmini/case.py` & `pgmini-0.1.6/pgmini/case.py`

 * *Files identical despite different names*

### Comparing `pgmini-0.1.5/pgmini/cast.py` & `pgmini-0.1.6/pgmini/cast.py`

 * *Files identical despite different names*

### Comparing `pgmini-0.1.5/pgmini/column.py` & `pgmini-0.1.6/pgmini/column.py`

 * *Files identical despite different names*

### Comparing `pgmini-0.1.5/pgmini/delete.py` & `pgmini-0.1.6/pgmini/delete.py`

 * *Files identical despite different names*

### Comparing `pgmini-0.1.5/pgmini/func.py` & `pgmini-0.1.6/pgmini/func.py`

 * *Files identical despite different names*

### Comparing `pgmini-0.1.5/pgmini/insert.py` & `pgmini-0.1.6/pgmini/insert.py`

 * *Files identical despite different names*

### Comparing `pgmini-0.1.5/pgmini/literal.py` & `pgmini-0.1.6/pgmini/literal.py`

 * *Files identical despite different names*

### Comparing `pgmini-0.1.5/pgmini/marks.py` & `pgmini-0.1.6/pgmini/marks.py`

 * *Files identical despite different names*

### Comparing `pgmini-0.1.5/pgmini/operation.py` & `pgmini-0.1.6/pgmini/operation.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,24 @@
         from .operations import OperationMath
         return OperationMath(self, right=other, operator='*')
 
     def __truediv__(self, other):
         from .operations import OperationMath
         return OperationMath(self, right=other, operator='/')
 
+    def __getitem__(self, item: int | slice):
+        from .operations import OperationSlice
+        return OperationSlice(self, right=item)
+
+    def __setitem__(self, item):
+        raise RuntimeError
+
+    def __delitem__(self, key):
+        raise RuntimeError
+
     def Is(self, other):
         from .operations import OperationMath
         return OperationMath(self, right=other, operator='IS')
 
     def IsNot(self, other):
         from .operations import OperationMath
         return OperationMath(self, right=other, operator='IS NOT')
```

### Comparing `pgmini-0.1.5/pgmini/operations.py` & `pgmini-0.1.6/pgmini/operations.py`

 * *Files 12% similar despite different names*

```diff
@@ -121,14 +121,56 @@
             _build(self._right, params),
         )
         if self._marks:
             res = self._marks.build(res)
         return res
 
 
+@attrs.frozen(eq=False)
+class OperationSlice(Operation):
+    _right: Any = attrs.field(alias='right', default=_NOT_SET)
+
+    def _build(self, params: list | dict) -> str:
+        if alias := extract_alias(self):
+            return alias
+
+        expr = '%s[%s]' % (
+            _wrap_operation_member(self._left),
+            _wrap_operation_member(self._right),
+        )
+        part1 = _build(self._left, params)
+        if (
+            self._left._marks is not None
+            and self._left._marks.cast is not None
+            and not RE_PARENTHESIZED.fullmatch(part1)
+        ):
+            part1 = '(%s)' % part1
+
+        if isinstance(self._right, slice):
+            part2 = '%s:%s' % (
+                (
+                    ''
+                    if self._right.start is None
+                    else _build(_convert_right(self._right.start), params)
+                ),
+                (
+                    ''
+                    if self._right.stop is None
+                    else _build(_convert_right(self._right.stop), params)
+                ),
+            )
+        else:
+            part2 = _build(_convert_right(self._right), params)
+
+        res = expr % (part1, part2)
+        if self._marks:
+            res = self._marks.build(res)
+        return res
+
+
 def _convert_items(value):
     from .select import Select
 
     if isinstance(value, ITERABLES):
         if not value:
             raise ValueError
         value = tuple(prepare_column(i) for i in value)
```

### Comparing `pgmini-0.1.5/pgmini/operators.py` & `pgmini-0.1.6/pgmini/operators.py`

 * *Files identical despite different names*

### Comparing `pgmini-0.1.5/pgmini/order_by.py` & `pgmini-0.1.6/pgmini/order_by.py`

 * *Files identical despite different names*

### Comparing `pgmini-0.1.5/pgmini/param.py` & `pgmini-0.1.6/pgmini/param.py`

 * *Files identical despite different names*

### Comparing `pgmini-0.1.5/pgmini/select.py` & `pgmini-0.1.6/pgmini/select.py`

 * *Files identical despite different names*

### Comparing `pgmini-0.1.5/pgmini/subquery.py` & `pgmini-0.1.6/pgmini/subquery.py`

 * *Files identical despite different names*

### Comparing `pgmini-0.1.5/pgmini/table.py` & `pgmini-0.1.6/pgmini/table.py`

 * *Files identical despite different names*

### Comparing `pgmini-0.1.5/pgmini/update.py` & `pgmini-0.1.6/pgmini/update.py`

 * *Files identical despite different names*

### Comparing `pgmini-0.1.5/pgmini/utils.py` & `pgmini-0.1.6/pgmini/utils.py`

 * *Files identical despite different names*

### Comparing `pgmini-0.1.5/pyproject.toml` & `pgmini-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pgmini"
-version = "0.1.5"
+version = "0.1.6"
 description = "Build sql for PostgreSQL"
 authors = ["Vitalii Ponomar"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ponomar/pgmini"
 
 [tool.poetry.dependencies]
```

### Comparing `pgmini-0.1.5/setup.py` & `pgmini-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['attrs>=22.2.0']
 
 setup_kwargs = {
     'name': 'pgmini',
-    'version': '0.1.5',
+    'version': '0.1.6',
     'description': 'Build sql for PostgreSQL',
     'long_description': '[![Test & Lint](https://github.com/ponomar/pgmini/actions/workflows/main.yml/badge.svg)](https://github.com/ponomar/pgmini/actions/workflows/main.yml)\n\n## 🇺🇦 What is pgmini? 🇺🇦\n\nIt is the PostgreSQL query builder with next core principles:\n- simple (predictable, without magic)\n- fast\n\nAll object are immutable (thanks to [attrs](https://www.attrs.org) lib).\nPython code as close to SQL structure as possible.\nLibrary doesn\'t try to be everything.\nIt doesn\'t manage connections to postgres, doesn\'t escape params.\nAll this can and should be done with other tools: (asyncpg, psycopg2, postgresql itself etc.).\n\nI\'ve decided to use `PascalCase` methods naming to avoid collisions with python reserved words: \n`From`, `And`, `Or`, `Else`, `With`, `As` etc.\n\n## Examples\n```python\nUser = Table(\'user\')  # dynamic columns\n\nq = Select(User.id, User.name).From(User).Where(User.email == \'test@test.com\')\n\nbuild(q)\n# (\n#     \'SELECT id, name FROM "user" WHERE email = $1\', \n#     [\'test@test.com\'],\n# )\n```\n\nExplicitly defined table schema allows to save filters and methods for further reusing \nand to use IDE code analyzers for smart completions, find usages, bulk refactors etc.  \n```python\nclass RoleSchema(Table):\n    id: int\n    name: str\n    status: str\n    \n    @property\n    def status_active(self):  # can also be decorated with functools.cache\n        return self.status == Literal(\'active\')\n    \n    def name_startswith(self, value: str):\n        return self.name.Like(f\'{value}%\')\n\nRole = RoleSchema(\'role\')\nq = Select(Role.id).From(Role).Where(Role.status_active, Role.name_startswith(\'admin\'))\n\nRoleAlias = Role.As(\'role2\')  # all columns/methods are visible for IDE live inspection as well\nq = (\n    Select(Role.STAR).From(Role)\n    .Where(Not(Exists(\n        Select(1).From(RoleAlias)\n        .Where(RoleAlias.id < Role.id, RoleAlias.status_active)\n    )))\n)\n```\n\n#### WHERE\nWhere takes *args which work like AND operator.\n```python\nt = Table(\'tbl\')\nq = (\n    Select(t.id).From(t)\n    .Where(\n        t.id.Between(10, 20), \n        Or(t.name > \'name\', And(t.status == \'active\', Not(t.id == 15))),\n    )\n)\n# SELECT id FROM tbl WHERE id BETWEEN $1 AND $2 AND (name > $3 OR (status = $4 AND NOT (id = $5)))\n\n# Add filters to existent query\nq2 = q.Where(t.id != 14)\n```\n\n#### JOIN\n```python\nt, t2 = Table(\'tbl\'), Table(\'tbl2\')\n\nsq = Select(t2.name).From(t2).Where(t2.id == t.id).Subquery(\'sq\')\nq = (\n    Select(t.id).From(t)\n    .Join(t2, t2.id == t.id)\n    .LeftJoin(t2, And(t2.id == t.id, t2.status == \'active\'))\n    .JoinLateral(sq, True)\n    .LeftJoinLateral(sq, sq.name != \'test\')\n)\n```\n\n#### PARAMETERS / LITERALS\nBy default, all values are considered as parameters. \nIf you need to cast value or add alias use Param wrapper.\nIf you need to literally insert value into sql use special Literal wrapper, \nbut be very careful - it won\'t be escaped and can lead to SQL injections. \nUse Literal only with data you can 100% trust.\n```python\nt = Table(\'tbl\')\nq = (\n    Select(t.STAR, Param(10).Cast(\'int\').As(\'added\')).From(t)\n    .Where(\n        t.id1 == 1, \n        t.id2 != Param(2).Cast(\'float\'), \n        t.id3 > Literal(3), \n        t.id4 < Literal(4).Cast(\'numeric\'),\n    )\n)\nbuild(q)\n# (\n#     \'SELECT *, $1::int AS added FROM tbl WHERE id1 == $2 AND id2 != $3::float AND id3 > 3 AND id4 < 4::numeric\',\n#     [10, 1, 2],\n# )\n```\n\n#### FUNCTIONS\nThere are `Func` and its `F` alias.\n```python\nt = Table(\'tbl\')\n\nq1 = (\n    Select(\n        F.count(\'*\'), \n        F.count(t.id).Where(t.id > 10, t.id < 20),\n        F.array_agg(t.id).OrderBy(t.id.Desc().NullsLast()).As(\'ids\'),\n    )\n    .From(t)\n)\n\nq2 = Select(t.id, F.row_number().Over(partition_by=t.status, order_by=t.id)).From(t)\n\nf = F.unnest(Literal([1, 2, 3])).As(\'idx\')\nq3 = Select(f.STAR).From(f)\n# SELECT * FROM UNNEST(ARRAY[1, 2, 3]) AS idx\n\nq4 = Select(Case((t.id == 1, \'first\'), (t.id == 2, \'second\'), Else=\'third\').As(\'val\')).From(t)\n\nq5 = Select(Array([t.id, 5, 7])).From(t)\n```\n\n#### ORDER BY / GROUP BY / HAVING / DISTINCT / DISTINCT ON\n```python\nt = Table(\'tbl\')\n\nq1 = Select(t.id.Distinct()).From(t)\n# SELECT DISTINCT id FROM tbl\n\nq2 = Select(t.STAR).From(t).OrderBy(t.id.Desc(), t.name.NullsLast())\n\nq3 = Select(F.count(\'*\')).From(t).GroupBy(t.status).Having(F.count(\'*\') > 10)\n\nq4 = Select(t.id, t.status).From(t).DistinctOn(t.status)\n# SELECT DISTINCT ON (status) id, status FROM tbl\n```\n\n#### OPERATIONS\nBasic math operator are supported out of the box: \n`+`, `-`, `*`, `/`, `>`, `>=`, `<`, `<=`. \nOthers are support as methods:\n```python\nt = Table(\'tbl\')\nq = (\n    Select(\n        t.id + t.id,\n        t.id - 1,\n        t.id * 10,\n        t.id > 15,\n        (t.id == 10).As(\'equals_ten\'),\n        (t.id != 11).As(\'not_equals_eleven\'),\n        Param(10) > 9,\n        (Literal(5) * 3.5).Cast(\'int\'),\n        t.id.Between(1, 2),\n        t.id.In([1, 2, 3]),\n        t.id.NotIn(Select(t.id).From(t).Where(t.id < 10)),\n        t.name.Is(None),\n        t.active.IsNot(False),\n        t.data.Op(\'->>\', \'key\').As(\'value1\'),\n        t.data.Op(\'#>>\', [\'key1\', \'key2\']).As(\'value2\'),\n        t.id.Any(list(range(1_000))),\n        t.name.Like(\'%ABC%\'),\n        t.name.Ilike(\'%abc%\'),\n    )\n    .From(t)\n)\n```\n\n#### INSERT\n```python\nt = Table(\'tbl\')\nq = (\n    Insert(t, columns=(t.name, t.status))\n    .Values(\n        (Param(\'some text\').Cast(\'varchar(10)\'), \'active\'),\n        (\'other text\', Literal(\'deleted\')),\n    )\n    .Returning(t.STAR)\n)\n\nbuild(q)\n# (\n#     "INSERT INTO tbl (name, status) VALUES ($1::varchar(10), $2), ($3, \'deleted\') RETURNING *",\n#     [\'some text\', \'active\', \'other text\'],\n# )\n\n# From select\nq = (\n    Insert(t, columns=(t.name, t.status))\n    .Select(\n        Select(F.concat(t.name, F.random().Cast(\'text\')), t.status)\n        .From(t)\n        .Where(t.id < 100)\n        .Limit(10)\n    )\n    .Returning(t.STAR)\n)\n\n# CTE\nsq = Select(t.STAR).From(t).Where(t.id < 100).Subquery(\'sq\')\nq = (\n    With(sq)\n    .Insert(t, (\'name\', \'status\'))\n    .From(Select(sq.name, sq.status).From(sq))\n)\n\n# Efficient bulk insert from the list of values\nvalues = [(str(i), \'active\') for i in range(1_000)]\nq = (\n    Insert(t, (\'name\', \'status\'))\n    .From(Select(\n        F.unnest(Param([name for name, _ in values]).Cast(\'text[]\')),\n        F.unnest(Param([status for _, status in values]).Cast(\'enum_status[]\')),\n    ))\n)\n```\n\n#### UPDATE / DELETE\n```python\nt = Table(\'stmh\')\nq1 = Update(t).Set({t.name: \'second\'}).Where(t.name == \'first\', t.status == \'active\').Returning(t.id)\nq2 = Delete(t).Where(t.id == 25).Returning(t.id)\n```\n\n#### Subquery / CTE\nAny Select/Insert/Update/Delete has Subquery method.\n```python\nt = Table(\'tbl\')\nsq = Select(t.id).From(t).Where(t.id < 100).Subquery(\'sq\')\n\n# Subquery\nq = Select(sq.id).From(sq).Where(sq.id > 50)\n# SELECT id FROM (SELECT id FROM tbl WHERE id < $1) As sq WHERE id > $2\n\n# CTE\nq = With(sq).Select(sq.id).From(sq).Where(sq.id > 50).Limit(2)\n# WITH sq AS (SELECT id FROM tbl WHERE id < $1) SELECT id FROM sq WHERE id > $2 LIMIT $3\n```\n\n***\n\n### Why not sqlalchemy?\n- too smart (tries to do everything: from connection/session management, to sql generating and params escaping)\n- too complex\n- too slow\n- mutable (on its core)\n\nIt is good for simple projects with simple sql queries. \nBut when your project grows up, your team grows up, sqlalchemy always leads to errors,\nunnecessary complexity, extra time your team need to spend to learn it, find not obvious bugs etc.  \n\n\n### Why not pypika?\nWhile it is much simpler then sqlalchemy, it also requires you to learn their own "sql syntax" which is not always obvious.\nAnd by default it uses parameters as literals, so it can lead to sql injections.\n\n\n***\n\nThe library is inspired by Ukraine🇺🇦 (Kyiv is my home) and its brave and free people🔱.\n\nSlava Ukraini, Heroyam slava!\n',
     'author': 'Vitalii Ponomar',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ponomar/pgmini',
```

### Comparing `pgmini-0.1.5/PKG-INFO` & `pgmini-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgmini
-Version: 0.1.5
+Version: 0.1.6
 Summary: Build sql for PostgreSQL
 Home-page: https://github.com/ponomar/pgmini
 License: MIT
 Author: Vitalii Ponomar
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

