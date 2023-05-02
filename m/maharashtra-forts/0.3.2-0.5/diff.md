# Comparing `tmp/maharashtra-forts-0.3.2.macosx-10.9-x86_64.tar.gz` & `tmp/maharashtra-forts-0.5.macosx-10.9-x86_64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maharashtra-forts-0.3.2.macosx-10.9-x86_64.tar", last modified: Tue May  2 12:00:57 2023, max compression
+gzip compressed data, was "maharashtra-forts-0.5.macosx-10.9-x86_64.tar", last modified: Tue May  2 12:09:05 2023, max compression
```

## Comparing `maharashtra-forts-0.3.2.macosx-10.9-x86_64.tar` & `maharashtra-forts-0.5.macosx-10.9-x86_64.tar`

### file list

```diff
@@ -1,26 +1,85 @@
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:00:57.544891 ./
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:00:57.544948 ./Library/
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:00:57.545002 ./Library/Frameworks/
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:00:57.545055 ./Library/Frameworks/Python.framework/
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:00:57.545111 ./Library/Frameworks/Python.framework/Versions/
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:00:57.545165 ./Library/Frameworks/Python.framework/Versions/3.8/
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:00:57.545218 ./Library/Frameworks/Python.framework/Versions/3.8/lib/
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:00:57.545273 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:00:57.558908 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:00:57.547723 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra-forts/
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-04-18 18:22:46.000000 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra-forts/__init__.py
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:00:57.548954 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra-forts/__pycache__/
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)      198 2023-05-02 12:00:57.548874 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra-forts/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)      591 2023-05-02 12:00:57.548537 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra-forts/__pycache__/get_forts.cpython-38.pyc
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)      487 2023-05-02 07:41:41.000000 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra-forts/get_forts.py
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:00:57.549180 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:09:05.055403 ./
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:09:05.055455 ./Library/
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:09:05.055511 ./Library/Frameworks/
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:09:05.055564 ./Library/Frameworks/Python.framework/
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:09:05.055616 ./Library/Frameworks/Python.framework/Versions/
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:09:05.055668 ./Library/Frameworks/Python.framework/Versions/3.8/
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:09:05.055726 ./Library/Frameworks/Python.framework/Versions/3.8/lib/
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:09:05.055781 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:09:05.082368 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:09:05.062068 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/
 -rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-04-18 18:22:46.000000 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/__init__.py
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:00:57.549599 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/__pycache__/
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)      198 2023-05-02 12:00:57.549546 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)      591 2023-05-02 12:00:57.549294 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/__pycache__/get_forts.cpython-38.pyc
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:09:05.062460 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/__pycache__/
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      198 2023-05-02 12:09:05.062412 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      591 2023-05-02 12:09:05.062175 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/__pycache__/get_forts.cpython-38.pyc
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:09:05.062566 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/forts/
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 06:48:51.000000 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/forts/__init__.py
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:09:05.065042 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/forts/__pycache__/
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      204 2023-05-02 12:09:05.063663 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/forts/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      217 2023-05-02 12:09:05.064985 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/forts/__pycache__/harishchandragad_fort.cpython-38.pyc
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      208 2023-05-02 12:09:05.063478 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/forts/__pycache__/lohagad_fort.cpython-38.pyc
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      210 2023-05-02 12:09:05.064257 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/forts/__pycache__/pratapgad_fort.cpython-38.pyc
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      209 2023-05-02 12:09:05.063102 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/forts/__pycache__/purandar_fort.cpython-38.pyc
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      207 2023-05-02 12:09:05.064542 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/forts/__pycache__/raigad_fort.cpython-38.pyc
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      207 2023-05-02 12:09:05.063290 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/forts/__pycache__/rajgad_fort.cpython-38.pyc
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      209 2023-05-02 12:09:05.062908 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/forts/__pycache__/shivneri_fort.cpython-38.pyc
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      209 2023-05-02 12:09:05.062674 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/forts/__pycache__/sinhagad_fort.cpython-38.pyc
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      207 2023-05-02 12:09:05.064776 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/forts/__pycache__/tikona_fort.cpython-38.pyc
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      206 2023-05-02 12:09:05.063964 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/forts/__pycache__/torna_fort.cpython-38.pyc
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/forts/harishchandragad_fort.py
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/forts/lohagad_fort.py
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/forts/pratapgad_fort.py
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/forts/purandar_fort.py
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/forts/raigad_fort.py
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/forts/rajgad_fort.py
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/forts/shivneri_fort.py
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/forts/sinhagad_fort.py
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/forts/tikona_fort.py
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/forts/torna_fort.py
 -rw-r--r--   0 rahulbhoyar   (501) staff       (20)      487 2023-05-02 07:41:41.000000 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/get_forts.py
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:00:57.563251 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts-0.3.2-py3.8.egg-info/
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)     2386 2023-05-02 12:00:57.557086 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts-0.3.2-py3.8.egg-info/PKG-INFO
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)      243 2023-05-02 12:00:57.558763 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts-0.3.2-py3.8.egg-info/SOURCES.txt
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)        1 2023-05-02 12:00:57.557224 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts-0.3.2-py3.8.egg-info/dependency_links.txt
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)       18 2023-05-02 12:00:57.557389 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts-0.3.2-py3.8.egg-info/top_level.txt
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:09:05.083385 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts-0.5-py3.8.egg-info/
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      189 2023-05-02 12:09:05.079135 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts-0.5-py3.8.egg-info/PKG-INFO
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)     1085 2023-05-02 12:09:05.082239 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts-0.5-py3.8.egg-info/SOURCES.txt
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)        1 2023-05-02 12:09:05.079248 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts-0.5-py3.8.egg-info/dependency_links.txt
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)       20 2023-05-02 12:09:05.079366 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts-0.5-py3.8.egg-info/entry_points.txt
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)       23 2023-05-02 12:09:05.079492 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts-0.5-py3.8.egg-info/top_level.txt
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:09:05.072211 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/venv/
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-04-18 18:28:09.000000 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/venv/__init__.py
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:09:05.072370 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/venv/__pycache__/
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      185 2023-05-02 12:09:05.072311 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/venv/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:09:05.065958 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/venv/bin/
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-04-18 18:28:09.000000 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/venv/bin/__init__.py
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:09:05.071845 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/venv/bin/__pycache__/
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      189 2023-05-02 12:09:05.066657 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/venv/bin/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      572 2023-05-02 12:09:05.071225 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/venv/bin/__pycache__/rst2html.cpython-38.pyc
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      694 2023-05-02 12:09:05.069221 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/venv/bin/__pycache__/rst2html4.cpython-38.pyc
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      631 2023-05-02 12:09:05.069624 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/venv/bin/__pycache__/rst2html5.cpython-38.pyc
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      705 2023-05-02 12:09:05.066419 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/venv/bin/__pycache__/rst2latex.cpython-38.pyc
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      664 2023-05-02 12:09:05.071493 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/venv/bin/__pycache__/rst2man.cpython-38.pyc
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      718 2023-05-02 12:09:05.070340 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/venv/bin/__pycache__/rst2odt.cpython-38.pyc
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)     1647 2023-05-02 12:09:05.068780 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/venv/bin/__pycache__/rst2odt_prepstyles.cpython-38.pyc
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      578 2023-05-02 12:09:05.070672 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/venv/bin/__pycache__/rst2pseudoxml.cpython-38.pyc
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      617 2023-05-02 12:09:05.070976 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/venv/bin/__pycache__/rst2s5.cpython-38.pyc
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      791 2023-05-02 12:09:05.066100 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/venv/bin/__pycache__/rst2xetex.cpython-38.pyc
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      580 2023-05-02 12:09:05.069917 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/venv/bin/__pycache__/rst2xml.cpython-38.pyc
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      640 2023-05-02 12:09:05.071783 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/venv/bin/__pycache__/rstpep2html.cpython-38.pyc
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      664 2023-04-18 18:33:46.000000 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/venv/bin/rst2html.py
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      786 2023-04-18 18:33:46.000000 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/venv/bin/rst2html4.py
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)     1131 2023-04-18 18:33:46.000000 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/venv/bin/rst2html5.py
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      863 2023-04-18 18:33:46.000000 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/venv/bin/rst2latex.py
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      686 2023-04-18 18:33:46.000000 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/venv/bin/rst2man.py
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      852 2023-04-18 18:33:46.000000 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/venv/bin/rst2odt.py
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)     1790 2023-04-18 18:33:46.000000 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/venv/bin/rst2odt_prepstyles.py
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      671 2023-04-18 18:33:46.000000 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/venv/bin/rst2pseudoxml.py
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      707 2023-04-18 18:33:46.000000 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/venv/bin/rst2s5.py
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      943 2023-04-18 18:33:46.000000 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/venv/bin/rst2xetex.py
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      672 2023-04-18 18:33:46.000000 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/venv/bin/rst2xml.py
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      740 2023-04-18 18:33:46.000000 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/venv/bin/rstpep2html.py
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:09:05.071968 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/venv/include/
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-04-18 18:28:09.000000 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/venv/include/__init__.py
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:09:05.072110 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/venv/include/__pycache__/
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      193 2023-05-02 12:09:05.072059 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/venv/include/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:09:05.072488 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/venv/lib/
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-04-18 18:28:09.000000 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/venv/lib/__init__.py
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:09:05.072672 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/venv/lib/__pycache__/
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      189 2023-05-02 12:09:05.072603 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/venv/lib/__pycache__/__init__.cpython-38.pyc
```

