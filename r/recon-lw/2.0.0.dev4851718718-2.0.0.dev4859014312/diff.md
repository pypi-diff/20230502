# Comparing `tmp/recon_lw-2.0.0.dev4851718718.tar.gz` & `tmp/recon_lw-2.0.0.dev4859014312.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev4851718718.tar", last modified: Mon May  1 14:10:47 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev4859014312.tar", last modified: Tue May  2 08:10:58 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev4851718718.tar` & `recon_lw-2.0.0.dev4859014312.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:10:47.000000 recon_lw-2.0.0.dev4851718718/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-01 14:10:05.000000 recon_lw-2.0.0.dev4851718718/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-01 14:10:47.000000 recon_lw-2.0.0.dev4851718718/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-01 14:10:05.000000 recon_lw-2.0.0.dev4851718718/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-01 14:10:28.000000 recon_lw-2.0.0.dev4851718718/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:10:47.000000 recon_lw-2.0.0.dev4851718718/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1877 2023-05-01 14:10:05.000000 recon_lw-2.0.0.dev4851718718/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     2748 2023-05-01 14:10:05.000000 recon_lw-2.0.0.dev4851718718/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-01 14:10:05.000000 recon_lw-2.0.0.dev4851718718/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13016 2023-05-01 14:10:05.000000 recon_lw-2.0.0.dev4851718718/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    20885 2023-05-01 14:10:05.000000 recon_lw-2.0.0.dev4851718718/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    14809 2023-05-01 14:10:05.000000 recon_lw-2.0.0.dev4851718718/recon_lw/recon_ob_cross_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:10:47.000000 recon_lw-2.0.0.dev4851718718/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-01 14:10:47.000000 recon_lw-2.0.0.dev4851718718/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      374 2023-05-01 14:10:47.000000 recon_lw-2.0.0.dev4851718718/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-01 14:10:47.000000 recon_lw-2.0.0.dev4851718718/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-01 14:10:47.000000 recon_lw-2.0.0.dev4851718718/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-01 14:10:47.000000 recon_lw-2.0.0.dev4851718718/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-01 14:10:05.000000 recon_lw-2.0.0.dev4851718718/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-01 14:10:47.000000 recon_lw-2.0.0.dev4851718718/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-01 14:10:05.000000 recon_lw-2.0.0.dev4851718718/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 08:10:58.000000 recon_lw-2.0.0.dev4859014312/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-02 08:10:32.000000 recon_lw-2.0.0.dev4859014312/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-02 08:10:58.000000 recon_lw-2.0.0.dev4859014312/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-02 08:10:32.000000 recon_lw-2.0.0.dev4859014312/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-02 08:10:39.000000 recon_lw-2.0.0.dev4859014312/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 08:10:58.000000 recon_lw-2.0.0.dev4859014312/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1877 2023-05-02 08:10:32.000000 recon_lw-2.0.0.dev4859014312/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2748 2023-05-02 08:10:32.000000 recon_lw-2.0.0.dev4859014312/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-02 08:10:32.000000 recon_lw-2.0.0.dev4859014312/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13016 2023-05-02 08:10:32.000000 recon_lw-2.0.0.dev4859014312/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21293 2023-05-02 08:10:32.000000 recon_lw-2.0.0.dev4859014312/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14809 2023-05-02 08:10:32.000000 recon_lw-2.0.0.dev4859014312/recon_lw/recon_ob_cross_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 08:10:58.000000 recon_lw-2.0.0.dev4859014312/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-02 08:10:58.000000 recon_lw-2.0.0.dev4859014312/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      396 2023-05-02 08:10:58.000000 recon_lw-2.0.0.dev4859014312/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-02 08:10:58.000000 recon_lw-2.0.0.dev4859014312/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-02 08:10:58.000000 recon_lw-2.0.0.dev4859014312/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-02 08:10:58.000000 recon_lw-2.0.0.dev4859014312/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-02 08:10:32.000000 recon_lw-2.0.0.dev4859014312/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-02 08:10:58.000000 recon_lw-2.0.0.dev4859014312/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-02 08:10:32.000000 recon_lw-2.0.0.dev4859014312/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 08:10:58.000000 recon_lw-2.0.0.dev4859014312/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-05-02 08:10:32.000000 recon_lw-2.0.0.dev4859014312/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev4851718718/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev4859014312/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4851718718/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev4859014312/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4851718718/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev4859014312/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4851718718/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev4859014312/recon_lw/recon_ob.py`

 * *Files 12% similar despite different names*

```diff
@@ -211,26 +211,26 @@
     flush_sequence_clear_cache(n_processed, rule_settings["sequence_cache"])
 
 
 def init_aggr_seq(order_book: dict) -> None:
     order_book["aggr_seq"] = {"top_v": 0, "top_delta": 0, "limit_v": 0, "limit_delta": 0}
 
 
-def reflect_price_update_in_version(side, price, order_book):
+def reflect_price_update_in_version(side: str, price: float, order_book: dict):
     level = get_price_level(side, price, order_book)
     max_levels = order_book["aggr_max_levels"]
     if level <= max_levels:
         order_book["aggr_seq"]["limit_v"] += 1
         order_book["aggr_seq"]["limit_delta"] = 1
     if level == 1:
         order_book["aggr_seq"]["top_v"] += 1
         order_book["aggr_seq"]["top_delta"] = 1
 
 
-def ob_add_order(order_id, price, size, side, order_book):
+def ob_add_order(order_id: str, price: float, size: int, side: str, order_book: dict) -> tuple:
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
     order_book["aggr_seq"].update({"top_delta": 0, "limit_delta": 0})
 
     if find_order_position(order_id, order_book)[0] is not None:
         return {"error": order_id + " already exists"}, []
     if price not in order_book[side]:
@@ -238,15 +238,15 @@
     else:
         order_book[side][price][order_id] = size
 
     reflect_price_update_in_version(side, price, order_book)
     return {}, [copy.deepcopy(order_book)]
 
 
-def ob_update_order(order_id, price, size, order_book):
+def ob_update_order(order_id: str, price: float, size: int, order_book: dict) -> tuple:
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
     order_book["aggr_seq"].update({"top_delta": 0, "limit_delta": 0})
 
     old_side, old_price, old_size = find_order_position(order_id, order_book)
     if old_side is None:
         return {"error": order_id + " not found"}, []
@@ -268,15 +268,15 @@
         order_book[old_side][price][order_id] = size
         reflect_price_update_in_version(old_side, price, order_book)
         log.append(copy.deepcopy(order_book))
 
     return {}, log
 
 
-def ob_delete_order(order_id, order_book):
+def ob_delete_order(order_id: str, order_book: dict) -> tuple:
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
     order_book["aggr_seq"].update({"top_delta": 0, "limit_delta": 0})
 
     old_side, old_price, old_size = find_order_position(order_id, order_book)
     if old_side is None:
         return {"error": order_id + " not found"}, []
@@ -295,15 +295,15 @@
             log.append(copy.deepcopy(order_book))
     else:
         log.append(copy.deepcopy(order_book))
 
     return {}, log
 
 
-def ob_trade_order(order_id, traded_size, order_book):
+def ob_trade_order(order_id: str, traded_size: int, order_book: dict) -> tuple:
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
     order_book["aggr_seq"].update({"top_delta": 0, "limit_delta": 0})
     old_side, old_price, old_size = find_order_position(order_id, order_book)
     log = []
     if old_side is None:
         return {"error": order_id + " not found"}, []
@@ -326,57 +326,58 @@
     else:
         reflect_price_update_in_version(old_side, old_price, order_book)
         order_book[old_side][old_price][order_id] -= traded_size
         log.append(copy.deepcopy(order_book))
     return {}, log
 
 
-def ob_clean_book(order_book):
+def ob_clean_book(order_book: dict) -> tuple:
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
     order_book["aggr_seq"].update({"top_delta": 0, "limit_delta": 0})
     for side_key in ["ask", "bid"]:
         if side_key in order_book:
             order_book[side_key].clear()
     order_book["aggr_seq"]["limit_delta"] = 1
     order_book["aggr_seq"]["limit_v"] += 1
     order_book["aggr_seq"]["top_delta"] = 1
     order_book["aggr_seq"]["top_v"] += 1
     return {}, [copy.deepcopy(order_book)]
 
 
-def ob_change_status(new_status, order_book):
+def ob_change_status(new_status: str, order_book: dict) -> tuple:
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
     order_book["status"] = new_status
     order_book["aggr_seq"]["limit_delta"] = 1
     order_book["aggr_seq"]["limit_v"] += 1
     order_book["aggr_seq"]["top_delta"] = 1
     order_book["aggr_seq"]["top_v"] += 1
     return {}, [copy.deepcopy(order_book)]
 
 
-def find_order_position(order_id, order_book):
+def find_order_position(order_id: str, order_book: dict) -> tuple:
     for side in ["ask", "bid"]:
         for pr, orders in order_book[side].items():
             if order_id in orders:
                 return side, pr, orders[order_id]
     return None, None, None
 
 
 # levels start with 1 (1,2,......
-def get_price_level(side, p, order_book):
+def get_price_level(side: str, p: float, order_book: dict) -> int:
     if p not in order_book[side]:
         return -1
     levels = list(order_book[side].keys())
     levels.sort()
     return levels.index(p) + 1 if side == "ask" else len(levels) - levels.index(p)
 
 
-def ob_aggr_add_level(side, level, price, real_qty, real_num_orders, impl_qty, impl_num_orders, order_book):
+def ob_aggr_add_level(side: str, level: int, price: float, real_qty: int, real_num_orders: int, impl_qty: int,
+                      impl_num_orders: int, order_book: dict):
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
     order_book["aggr_seq"].update({"top_delta": 0, "limit_delta": 0})
     result_body = {}
     max_levels = order_book["aggr_max_levels"]
     side_key = side + "_aggr"
     new_index = level - 1
@@ -387,19 +388,18 @@
     new_level = {"price": price, "real_qty": real_qty, "real_num_orders": real_num_orders, "impl_qty": impl_qty,
                  "impl_num_orders": impl_num_orders}
     order_book[side_key].insert(new_index, new_level)
     if len(order_book[side_key]) == max_levels + 1:
         order_book[side_key].pop()
     order_book["aggr_seq"]["limit_delta"] = 1
     order_book["aggr_seq"]["limit_v"] += 1
-
     return {}, [copy.deepcopy(order_book)]
 
 
-def ob_aggr_delete_level(side, level, order_book):
+def ob_aggr_delete_level(side: str, level: int, order_book: dict) -> tuple:
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
     order_book["aggr_seq"].update({"top_delta": 0, "limit_delta": 0})
     result_body = {}
     side_key = side + "_aggr"
     del_index = level - 1
     if not 0 <= del_index < len(order_book[side_key]):
@@ -409,15 +409,16 @@
     order_book[side_key].pop(del_index)
 
     order_book["aggr_seq"]["limit_delta"] = 1
     order_book["aggr_seq"]["limit_v"] += 1
     return {}, [copy.deepcopy(order_book)]
 
 
-def ob_aggr_update_level(side, level, price, real_qty, real_num_orders, impl_qty, impl_num_orders, order_book):
+def ob_aggr_update_level(side: str, level: int, price: float, real_qty: int, real_num_orders: int, impl_qty: int,
+                         impl_num_orders: int, order_book: dict) -> tuple:
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
     order_book["aggr_seq"].update({"top_delta": 0, "limit_delta": 0})
     result_body = {}
     max_levels = order_book["aggr_max_levels"]
     side_key = side + "_aggr"
     update_index = level - 1
@@ -430,27 +431,27 @@
     order_book[side_key][update_index].update(upd_level)
     order_book["aggr_seq"]["limit_delta"] = 1
     order_book["aggr_seq"]["limit_v"] += 1
 
     return {}, [copy.deepcopy(order_book)]
 
 
-def ob_aggr_clean_book(order_book):
+def ob_aggr_clean_book(order_book: dict) -> tuple:
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
     order_book["aggr_seq"].update({"top_delta": 0, "limit_delta": 0})
     for side_key in ["ask_aggr", "bid_aggr"]:
         if side_key in order_book:
             order_book[side_key].clear()
     order_book["aggr_seq"]["limit_delta"] = 1
     order_book["aggr_seq"]["limit_v"] += 1
     return {}, [copy.deepcopy(order_book)]
 
 
-def ob_top_clean_book(order_book):
+def ob_top_clean_book(order_book: dict) -> tuple:
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
 
     order_book["ask_price"] = 0
     order_book["ask_real_qty"] = 0
     order_book["ask_impl_qty"] = 0
     order_book["ask_real_n_orders"] = 0
```

### Comparing `recon_lw-2.0.0.dev4851718718/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev4859014312/recon_lw/recon_ob_cross_stream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4851718718/setup.py` & `recon_lw-2.0.0.dev4859014312/setup.py`

 * *Files identical despite different names*

