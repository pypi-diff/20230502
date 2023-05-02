# Comparing `tmp/checkontap-0.1a5.tar.gz` & `tmp/checkontap-0.1a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkontap-0.1a5.tar", last modified: Wed Apr 26 14:34:00 2023, max compression
+gzip compressed data, was "checkontap-0.1a6.tar", last modified: Tue May  2 15:04:01 2023, max compression
```

## Comparing `checkontap-0.1a5.tar` & `checkontap-0.1a6.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0      223 2023-03-23 09:02:45.881436 checkontap-0.1a5/README.md
--rw-r--r--   0        0        0      926 2023-03-22 16:30:38.341339 checkontap-0.1a5/checkontap/__init__.py
--rw-r--r--   0        0        0     3431 2023-03-23 14:53:12.575066 checkontap-0.1a5/checkontap/cli.py
--rw-r--r--   0        0        0      756 2023-03-22 16:09:15.025609 checkontap-0.1a5/checkontap/ontapcmd/__init__.py
--rw-r--r--   0        0        0     2227 2023-04-21 14:48:25.623996 checkontap-0.1a5/checkontap/ontapcmd/about.py
--rw-r--r--   0        0        0     6945 2023-04-21 14:48:51.992608 checkontap-0.1a5/checkontap/ontapcmd/aggregateusage.py
--rw-r--r--   0        0        0     2886 2023-04-26 14:31:12.533831 checkontap-0.1a5/checkontap/ontapcmd/clusterhealth.py
--rw-r--r--   0        0        0     7694 2023-04-21 14:49:13.743682 checkontap-0.1a5/checkontap/ontapcmd/diskhealth.py
--rw-r--r--   0        0        0     4509 2023-04-21 14:49:23.573489 checkontap-0.1a5/checkontap/ontapcmd/hardwarehealth.py
--rw-r--r--   0        0        0     3875 2023-04-24 12:40:05.504428 checkontap-0.1a5/checkontap/ontapcmd/interfacehealth.py
--rw-r--r--   0        0        0     4994 2023-04-21 14:49:47.394778 checkontap-0.1a5/checkontap/ontapcmd/lunusage.py
--rw-r--r--   0        0        0     5079 2023-04-21 14:49:57.522947 checkontap-0.1a5/checkontap/ontapcmd/volumehealth.py
--rw-r--r--   0        0        0     8463 2023-04-26 12:55:43.724726 checkontap-0.1a5/checkontap/ontapcmd/volumeusage.py
--rw-r--r--   0        0        0      757 2023-03-22 16:09:25.201105 checkontap-0.1a5/checkontap/tools/__init__.py
--rw-r--r--   0        0        0     9565 2023-04-26 13:06:26.630474 checkontap-0.1a5/checkontap/tools/cli.py
--rw-r--r--   0        0        0     3108 2023-04-24 12:07:20.737893 checkontap-0.1a5/checkontap/tools/helper.py
--rw-r--r--   0        0        0      857 2023-04-26 14:32:23.061640 checkontap-0.1a5/pyproject.toml
--rw-r--r--   0        0        0      893 1970-01-01 00:00:00.000000 checkontap-0.1a5/PKG-INFO
+-rw-r--r--   0        0        0      223 2023-03-23 09:02:45.881436 checkontap-0.1a6/README.md
+-rw-r--r--   0        0        0      926 2023-03-22 16:30:38.341339 checkontap-0.1a6/checkontap/__init__.py
+-rw-r--r--   0        0        0     3431 2023-03-23 14:53:12.575066 checkontap-0.1a6/checkontap/cli.py
+-rw-r--r--   0        0        0      756 2023-03-22 16:09:15.025609 checkontap-0.1a6/checkontap/ontapcmd/__init__.py
+-rw-r--r--   0        0        0     2227 2023-04-21 14:48:25.623996 checkontap-0.1a6/checkontap/ontapcmd/about.py
+-rw-r--r--   0        0        0     7033 2023-04-28 13:18:56.743322 checkontap-0.1a6/checkontap/ontapcmd/aggregateusage.py
+-rw-r--r--   0        0        0     4641 2023-04-27 15:24:18.383341 checkontap-0.1a6/checkontap/ontapcmd/clusterhealth.py
+-rw-r--r--   0        0        0     7694 2023-04-21 14:49:13.743682 checkontap-0.1a6/checkontap/ontapcmd/diskhealth.py
+-rw-r--r--   0        0        0     4509 2023-04-21 14:49:23.573489 checkontap-0.1a6/checkontap/ontapcmd/hardwarehealth.py
+-rw-r--r--   0        0        0     3878 2023-04-27 14:42:48.878279 checkontap-0.1a6/checkontap/ontapcmd/interfacehealth.py
+-rw-r--r--   0        0        0     4994 2023-04-21 14:49:47.394778 checkontap-0.1a6/checkontap/ontapcmd/lunusage.py
+-rw-r--r--   0        0        0     4298 2023-05-02 15:00:56.886969 checkontap-0.1a6/checkontap/ontapcmd/porthealth.py
+-rw-r--r--   0        0        0     7239 2023-04-28 14:49:04.694080 checkontap-0.1a6/checkontap/ontapcmd/ports.py
+-rw-r--r--   0        0        0     5079 2023-04-21 14:49:57.522947 checkontap-0.1a6/checkontap/ontapcmd/volumehealth.py
+-rw-r--r--   0        0        0     8463 2023-04-26 12:55:43.724726 checkontap-0.1a6/checkontap/ontapcmd/volumeusage.py
+-rw-r--r--   0        0        0      757 2023-03-22 16:09:25.201105 checkontap-0.1a6/checkontap/tools/__init__.py
+-rw-r--r--   0        0        0    10030 2023-04-28 13:08:45.930194 checkontap-0.1a6/checkontap/tools/cli.py
+-rw-r--r--   0        0        0     3918 2023-04-28 12:56:43.397643 checkontap-0.1a6/checkontap/tools/helper.py
+-rw-r--r--   0        0        0      857 2023-05-02 15:01:41.029050 checkontap-0.1a6/pyproject.toml
+-rw-r--r--   0        0        0      893 1970-01-01 00:00:00.000000 checkontap-0.1a6/PKG-INFO
```

### Comparing `checkontap-0.1a5/checkontap/__init__.py` & `checkontap-0.1a6/checkontap/__init__.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a5/checkontap/cli.py` & `checkontap-0.1a6/checkontap/cli.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a5/checkontap/ontapcmd/__init__.py` & `checkontap-0.1a6/checkontap/ontapcmd/__init__.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a5/checkontap/ontapcmd/about.py` & `checkontap-0.1a6/checkontap/ontapcmd/about.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a5/checkontap/ontapcmd/aggregateusage.py` & `checkontap-0.1a6/checkontap/ontapcmd/aggregateusage.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,152 +11,151 @@
 #    but WITHOUT ANY WARRANTY; without even the implied warranty of
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU Affero General Public License for more details.
 #
 #    You should have received a copy of the GNU Affero General Public License
 #    along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-from monplugin import Check,Status
+from monplugin import Check,Threshold,Status
 import logging
-from netapp_ontap.resources import Aggregate,Plex 
+from netapp_ontap.resources import Aggregate,Plex
 from netapp_ontap import NetAppRestError
 from ..tools import cli
-from ..tools.helper import setup_connection,item_filter,percent_to,to_percent,bytes_to,to_bytes,severity
+from ..tools.helper import setup_connection,item_filter,severity,bytes_to_uom,uom_to_bytes
 
 __cmd__ = "aggregate-usage"
-description = f"Mode {__cmd__} with -U / --unit % or size description like GB "
+description = f"Mode {__cmd__} with -m / --metric % or size description like used_GB "
 """
 Aggregate({
-    '_links': {'self': {'href': '/api/storage/aggregates/01d71c4b-88d8-43c3-ae33-afa2b64a629d'}}, 
-    'uuid': '01d71c4b-88d8-43c3-ae33-afa2b64a629d', 
+    '_links': {'self': {'href': '/api/storage/aggregates/01d71c4b-88d8-43c3-ae33-afa2b64a629d'}},
+    'uuid': '01d71c4b-88d8-43c3-ae33-afa2b64a629d',
     'space': {
-        'footprint': 139780465348608, 
-        'efficiency': {'ratio': 186.6856716029982, 'logical_used': 24291687892377600, 'savings': 24161567097976004}, 
-        'cloud_storage': {'used': 0}, 
-        'efficiency_without_snapshots': {'ratio': 2.08165380808469, 'logical_used': 252303379914752, 'savings': 131100046807748}, 
+        'footprint': 139780465348608,
+        'efficiency': {'ratio': 186.6856716029982, 'logical_used': 24291687892377600, 'savings': 24161567097976004},
+        'cloud_storage': {'used': 0},
+        'efficiency_without_snapshots': {'ratio': 2.08165380808469, 'logical_used': 252303379914752, 'savings': 131100046807748},
         'block_storage': {
-            'available': 62257396912128, 
-            'full_threshold_percent': 98, 
-            'used': 134769329168384, 
-            'size': 197026726080512, 
+            'available': 62257396912128,
+            'full_threshold_percent': 98,
+            'used': 134769329168384,
+            'size': 197026726080512,
             'inactive_user_data': 0}
-        }, 
+        },
     'name': 'storage.central.acme'})
 Plex({
     'aggregate': {
-        'uuid': '97e37d61-23b0-4917-85c8-ae9d5354bba5', 
-        '_links': {'self': {'href': '/api/storage/aggregates/97e37d61-23b0-4917-85c8-ae9d5354bba5'}}, 
+        'uuid': '97e37d61-23b0-4917-85c8-ae9d5354bba5',
+        '_links': {'self': {'href': '/api/storage/aggregates/97e37d61-23b0-4917-85c8-ae9d5354bba5'}},
         'name': 'aggr1_01'
-        }, 
-    'resync': {'active': False}, 
-    'online': True, 
-    'pool': 'pool0', 
-    'state': 'normal', 
+        },
+    'resync': {'active': False},
+    'online': True,
+    'pool': 'pool0',
+    'state': 'normal',
     'raid_groups': [{
-        'cache_tier': False, 
-        'recomputing_parity': {'active': False}, 
-        'reconstruct': {'active': False}, 
-        'degraded': False, 
+        'cache_tier': False,
+        'recomputing_parity': {'active': False},
+        'reconstruct': {'active': False},
+        'degraded': False,
         'disks': [{
-            'disk': {'name': '1.0.11'}, 
-            'usable_size': 3838499094528, 
-            'state': 'normal', 
-            'type': 'fsas', 
+            'disk': {'name': '1.0.11'},
+            'usable_size': 3838499094528,
+            'state': 'normal',
+            'type': 'fsas',
             'position': 'dparity'
             }, {
             'disk' .....
-            }], 
-        'name': 'rg0'}], 
+            }],
+        'name': 'rg0'}],
     'name': 'plex0'})
 """
+
 def run():
     parser = cli.Parser()
     parser.set_description(description)
     parser.add_required_arguments(cli.Argument.WARNING,cli.Argument.CRITICAL)
     parser.add_optional_arguments(cli.Argument.EXCLUDE,
                                   cli.Argument.INCLUDE,
-                                  cli.Argument.UNIT)
+                                  cli.Argument.METRIC)
     args = parser.get_args()
     # Setup module logging
     logger = logging.getLogger(__name__)
     logger.disabled = True
     if args.verbose:
         for log_name, log_obj in logging.Logger.manager.loggerDict.items():
             log_obj.disabled = False
             logging.getLogger(log_name).setLevel(severity(args.verbose))
 
-    check = Check()
-
-    check.set_threshold(
-        warning=args.warning,
-        critical=args.critical
-    )
-
+    check = Check(threshold = Threshold(args.warning or None, args.critical or None))
     setup_connection(args.host, args.api_user, args.api_pass)
 
     try:
         aggr_count = Aggregate.count_collection()
         logger.debug(f"found {aggr_count} Aggregates")
         if aggr_count == 0:
             check.exit(Status.UNKNOWN, "no aggregates found")
 
         for aggr in Aggregate.get_collection():
             aggr.get(fields="space,uuid")
             if (args.exclude or args.include) and item_filter(args,aggr.name):
+                logger.debug(f"{aggr.name} filtered out and removed from check")
                 aggr_count -= 1
                 continue
-            for plex in Plex.get_collection(aggr.uuid):
-                plex.get(fields="raid_groups")
-                logging.debug(f"Plex {plex.name}\n{plex.__dict__}") 
-                for rg in plex.raid_groups:
-                    if rg.reconstruct.active:
-                        check.add_message(Status.CRITICAL, f"RaidGroup {rg.name} on Plex {plex.name} is reconstructing")
-
-            pctUsage = to_percent(aggr.space.block_storage.size,aggr.space.block_storage.used)
-            unitPerf = {'label': f'{aggr.name}_space',
-                    'value': aggr.space.block_storage.used,
-                    'uom': 'B',
-                    'min': 0,
-                    'max': aggr.space.block_storage.size,
-                    }
-            pctPerf = {
-                'label': f'{aggr.name}_percent',
-                'value': pctUsage,
-                'uom': '%',
-                'min': 0,
-                'max': 100,
-            }
-            if args.unit and '%' in args.unit:
-                pctPerf['threshold'] = check.threshold
-                check.add_perfdata(**pctPerf)
-                unitPerf['warning'] = percent_to(aggr.space.block_storage.size,args.warning)
-                unitPerf['critical'] = percent_to(aggr.space.block_storage.size,args.critical)
-                check.add_perfdata(**unitPerf)
-                check.add_message(
-                    check.threshold.get_status(pctUsage),
-                    f"{aggr.name} (Usage {bytes_to(aggr.space.block_storage.used,'GB')}/{bytes_to(aggr.space.block_storage.size,'GB')}GB {pctUsage}%)"
-                )
-            elif args.unit:
-                unitPerf['warning'] = to_bytes(args.warning,args.unit)
-                unitPerf['critical'] = to_bytes(args.critical,args.unit)
-                check.add_perfdata(**unitPerf)
-                check.add_perfdata(**pctPerf)
-                check.add_message(
-                    check.threshold.get_status(bytes_to(aggr.space.block_storage.used, args.unit)),
-                    f"{aggr.name} (Usage {bytes_to(aggr.space.block_storage.used,args.unit)}/{bytes_to(aggr.space.block_storage.size,args.unit)}{args.unit} {pctUsage}%)"
-                )
-            else:
-                unitPerf['threshold'] = check.threshold
-                check.add_perfdata(**unitPerf)
-                check.add_perfdata(**pctPerf)
-                check.add_message(
-                    check.threshold.get_status(aggr.space.block_storage.used),
-                    f"{aggr.name} (Usage {aggr.space.block_storage.used}/{aggr.space.block_storage.size}B {pctUsage}%)"
-                )
-        (code, message) = check.check_messages(separator='\n  ',allok=f"all {aggr_count} aggregates are fine")
+            logger.debug(f"Aggregate {aggr.name}\n{aggr.__dict__}")
+            
+            plex_count = Plex.count_collection(aggr.uuid)
+            if plex_count != 0:
+                for plex in Plex.get_collection(aggr.uuid):
+                    plex.get(fields="raid_groups")
+                    logging.debug(f"Plex {plex.name}\n{plex.__dict__}")
+                    for rg in plex.raid_groups:
+                        if rg.reconstruct.active:
+                            check.add_message(Status.CRITICAL, f"RaidGroup {rg.name} on Plex {plex.name} is reconstructing")
+    
+            value = {
+                'usage': bytes_to_uom(aggr.space.block_storage.used,'%',aggr.space.block_storage.size),
+                'used': aggr.space.block_storage.used,
+                'free': aggr.space.block_storage.size - aggr.space.block_storage.used,
+                'max': aggr.space.block_storage.size
+                }
+
+            for metric in ['usage','used','free']:
+                opts = {}
+                if metric in args.metric:
+                    typ, uom, *_ = (args.metric.split('_') + ['%' if 'usage' in args.metric else 'B'])
+                    threshold = {}
+                    opts['threshold'] = {}
+                    if '%' in uom:
+                        s = check.threshold.get_status(value['usage'])
+                        out = f"{value[typ] :.2f}%"
+                        if args.warning:
+                            threshold['warning'] = args.warning
+                        if args.critical:
+                            threshold['critical'] = args.critical
+                    else:
+                        s = check.threshold.get_status(bytes_to_uom(value[typ],uom))
+                        if 'free' in typ:
+                            pct = 100 - value['usage']
+                        else:
+                            pct = value['usage']
+
+                        out = f"{bytes_to_uom(value[metric],uom)}{uom} ({pct :.2f} %) "
+                        if args.warning:
+                            threshold['warning'] = str(uom_to_bytes(args.warning,uom))
+                        if args.critical:
+                            threshold['critical'] = str(uom_to_bytes(args.critical,uom))
+                    opts['threshold'] = Threshold(**threshold)
+                    if s != Status.OK:
+                        check.add_message(s, f"{args.metric} on {aggr.name} is: {out}")
+
+                puom = '%' if metric == 'usage' else 'B'
+                check.add_perfmultidata(aggr.name, 'aggregates',  label=metric, value=value[metric], uom=puom, **opts)
+        (code, message) = check.check_messages(separator=' ',allok=f"all {aggr_count} aggregates are fine")
         check.exit(code=code,message=message)
 
     except NetAppRestError as error:
         check.exit(Status.UNKNOWN, "Error => {}".format(error.http_err_response.http_response.text))
-    
+    except Exception as error:
+        logger.exception(error)
+
 if __name__ == "__main__":
-    run()
+    run()
```

### Comparing `checkontap-0.1a5/checkontap/ontapcmd/diskhealth.py` & `checkontap-0.1a6/checkontap/ontapcmd/diskhealth.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a5/checkontap/ontapcmd/hardwarehealth.py` & `checkontap-0.1a6/checkontap/ontapcmd/hardwarehealth.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a5/checkontap/ontapcmd/interfacehealth.py` & `checkontap-0.1a6/checkontap/ontapcmd/interfacehealth.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     check = Check()
 
     setup_connection(args.host, args.api_user, args.api_pass)
 
     IpInts = []
     try:
         interface_count = IpInterface.count_collection()
-        logger.info(f"found {interface_count} volumes")
+        logger.info(f"found {interface_count} interfaces")
         if interface_count == 0:
             check.exit(Status.UNKNOWN, "no interfaces found")
 
         for IpInt in IpInterface.get_collection():
             IpInt.get()
             if (args.exclude or args.include) and item_filter(args,IpInt.name):
                 logger.debug(f"exclude interface {IpInt.name}")
```

### Comparing `checkontap-0.1a5/checkontap/ontapcmd/lunusage.py` & `checkontap-0.1a6/checkontap/ontapcmd/lunusage.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a5/checkontap/ontapcmd/volumehealth.py` & `checkontap-0.1a6/checkontap/ontapcmd/volumehealth.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a5/checkontap/ontapcmd/volumeusage.py` & `checkontap-0.1a6/checkontap/ontapcmd/volumeusage.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a5/checkontap/tools/__init__.py` & `checkontap-0.1a6/checkontap/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a5/checkontap/tools/cli.py` & `checkontap-0.1a6/checkontap/tools/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -196,14 +196,25 @@
         'name_or_flags': ['-U', '--unit'],
         'options': {
             'action': 'store',
             'help': 'Unit to deal with',
             'choices': ['%', 'kB', 'MB', 'GB', 'TB', 'PB'],
         }
     }
+    METRIC = {
+        'name_or_flags': ['-m', '--metric'],
+        'options': {
+            'action': 'store',
+            'default': 'usage',
+            'help': 'The metric to apply the thresholds on, defaults to `usage`, can be: '
+                    'usage (in percent), free and used. '
+                    'free and used are measured in bytes. You can one of these suffixes: '
+                    'kB, MB, GB for example: free_MB or used_GB'
+        }
+    }
     NAME = {
         'name_or_flags': ['--name'],
         'options': {
             'action': 'append',
             'nargs': '+',
             'help': 'define something',
         }
```

### Comparing `checkontap-0.1a5/checkontap/tools/helper.py` & `checkontap-0.1a6/checkontap/tools/helper.py`

 * *Files 24% similar despite different names*

```diff
@@ -35,14 +35,39 @@
             return(False)
     elif args.include:
         if re.search(args.include,item):
             return(False)
         else:
             return(True)
 
+#
+# uom_to_bytes(20,%,2000) => 400B
+# uom_to_bytes(1024,MB) => 1048576B
+def uom_to_bytes(value, uom, maximum=None, bsize=1024) -> None:
+    a = {'kB' : 1, 'MB': 2, 'GB' : 3, 'TB' : 4, 'PB' : 5, 'EB' : 6 }
+    try:
+        if '%' in uom and maximum:
+            r = round((float(maximum) / 100) * int(value),2)
+        else:
+            r = round(float(value) * (bsize ** a[uom]),3)
+    except Exception as err:
+        return err
+    return(r)
+
+def bytes_to_uom(value, uom, maximum=None, bsize=1024) -> None:
+    a = {'kB' : 1, 'MB': 2, 'GB' : 3, 'TB' : 4, 'PB' : 5, 'EB' : 6 }
+    try:
+        if '%' in uom and maximum:
+            r = (float(value) / int(maximum) ) * 100
+        else:
+            r = round(float(value) / (bsize ** a[uom]),3)
+    except Exception as err:
+        return err
+    return(r)
+
 # Percent returned with 2 decimals
 def to_percent(max,value) -> None:
     try:
         pct = (float(value) / int(max) ) * 100
     except Exception as err:
         return err
     return(round(pct,2))
```

### Comparing `checkontap-0.1a5/pyproject.toml` & `checkontap-0.1a6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 build-backend = "flit_core.buildapi"
 requires = ["flit_core >=3.2,<4"]
 
 [project]
 name = "checkontap"
 readme = "README.md"
 description = "check_ontap monitoring plugin"
-version = "0.1a5"
+version = "0.1a6"
 requires-python = ">= 3.6"
 authors = [
     { name = "Matthias Gallinger", email = "matthias.gallinger@consol.de" }
 ]
 dependencies = [
     "netapp-ontap >= 9.11.1.0",
     "monplugin >= 0.5",
```

### Comparing `checkontap-0.1a5/PKG-INFO` & `checkontap-0.1a6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: checkontap
-Version: 0.1a5
+Version: 0.1a6
 Summary: check_ontap monitoring plugin
 Author-email: Matthias Gallinger <matthias.gallinger@consol.de>
 Requires-Python: >= 3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: System :: Monitoring
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

