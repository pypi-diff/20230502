# Comparing `tmp/netswift_cli-0.1.1.tar.gz` & `tmp/netswift_cli-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netswift_cli-0.1.1.tar", max compression
+gzip compressed data, was "netswift_cli-0.1.2.tar", max compression
```

## Comparing `netswift_cli-0.1.1.tar` & `netswift_cli-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      149 2023-05-02 08:35:12.064627 netswift_cli-0.1.1/netswift_cli/README.md
--rw-r--r--   0        0        0    16384 2023-05-02 10:12:39.593378 netswift_cli-0.1.1/netswift_cli/employee_absent.db
--rw-r--r--   0        0        0     5043 2023-05-02 10:13:25.232133 netswift_cli-0.1.1/netswift_cli/netswift_cli.py
--rw-r--r--   0        0        0      861 2023-05-02 08:52:26.285750 netswift_cli-0.1.1/netswift_cli/requirements.txt
--rw-r--r--   0        0        0      418 2023-05-02 10:18:47.277783 netswift_cli-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      591 1970-01-01 00:00:00.000000 netswift_cli-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      149 2023-05-02 08:35:12.064627 netswift_cli-0.1.2/netswift_cli/README.md
+-rw-r--r--   0        0        0    16384 2023-05-02 10:12:39.593378 netswift_cli-0.1.2/netswift_cli/employee_absent.db
+-rw-r--r--   0        0        0     5060 2023-05-02 10:21:40.933802 netswift_cli-0.1.2/netswift_cli/netswift_cli.py
+-rw-r--r--   0        0        0      861 2023-05-02 08:52:26.285750 netswift_cli-0.1.2/netswift_cli/requirements.txt
+-rw-r--r--   0        0        0      418 2023-05-02 10:21:50.732572 netswift_cli-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      591 1970-01-01 00:00:00.000000 netswift_cli-0.1.2/PKG-INFO
```

### Comparing `netswift_cli-0.1.1/netswift_cli/employee_absent.db` & `netswift_cli-0.1.2/netswift_cli/employee_absent.db`

 * *Files identical despite different names*

### Comparing `netswift_cli-0.1.1/netswift_cli/netswift_cli.py` & `netswift_cli-0.1.2/netswift_cli/netswift_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,15 +133,15 @@
         ]
         table_data.append(row)
 
     headers = ["Employee ID", "Name", "Absent Count"]
     typer.echo(tabulate(table_data, headers=headers, tablefmt="pretty"))
 
 @app.command()
-def list_absents(employee_id: str, month: str):
+def list_absents(employee_id: str, month: Optional[str] = None):
     """
     List all employees and their absent
     """
     if not month:
         month = datetime.now().strftime('%B')
     cursor.execute(f"SELECT * FROM absent WHERE employee_id = '{employee_id}' AND date LIKE '%{month}%'")
     absents = cursor.fetchall()
```

### Comparing `netswift_cli-0.1.1/netswift_cli/requirements.txt` & `netswift_cli-0.1.2/netswift_cli/requirements.txt`

 * *Files identical despite different names*

### Comparing `netswift_cli-0.1.1/PKG-INFO` & `netswift_cli-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netswift-cli
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple CLI application to manage NetSwift employee attendance
 Author: Rehmat Alam
 Author-email: rehmat@netswift.pk
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

