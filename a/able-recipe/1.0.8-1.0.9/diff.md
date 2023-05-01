# Comparing `tmp/able_recipe-1.0.8.tar.gz` & `tmp/able_recipe-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/able_recipe-1.0.8.tar", last modified: Sun Aug 15 20:36:00 2021, max compression
+gzip compressed data, was "dist/able_recipe-1.0.9.tar", last modified: Wed Dec 15 19:12:16 2021, max compression
```

## Comparing `able_recipe-1.0.8.tar` & `able_recipe-1.0.9.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-15 20:36:00.000000 able_recipe-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1159 2021-08-15 20:35:46.000000 able_recipe-1.0.8/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2021-08-15 20:35:46.000000 able_recipe-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       90 2021-08-15 20:35:46.000000 able_recipe-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3503 2021-08-15 20:36:00.000000 able_recipe-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2189 2021-08-15 20:35:46.000000 able_recipe-1.0.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-15 20:36:00.000000 able_recipe-1.0.8/able/
--rw-r--r--   0 runner    (1001) docker     (121)     1895 2021-08-15 20:35:46.000000 able_recipe-1.0.8/able/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10840 2021-08-15 20:35:46.000000 able_recipe-1.0.8/able/advertising.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-15 20:36:00.000000 able_recipe-1.0.8/able/android/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-15 20:35:46.000000 able_recipe-1.0.8/able/android/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5439 2021-08-15 20:35:46.000000 able_recipe-1.0.8/able/android/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (121)     6024 2021-08-15 20:35:46.000000 able_recipe-1.0.8/able/android/jni.py
--rw-r--r--   0 runner    (1001) docker     (121)    10646 2021-08-15 20:35:46.000000 able_recipe-1.0.8/able/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (121)     2217 2021-08-15 20:35:46.000000 able_recipe-1.0.8/able/queue.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-15 20:36:00.000000 able_recipe-1.0.8/able/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-15 20:36:00.000000 able_recipe-1.0.8/able/src/org/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-15 20:36:00.000000 able_recipe-1.0.8/able/src/org/able/
--rw-r--r--   0 runner    (1001) docker     (121)    10587 2021-08-15 20:35:46.000000 able_recipe-1.0.8/able/src/org/able/BLE.java
--rw-r--r--   0 runner    (1001) docker     (121)     2834 2021-08-15 20:35:46.000000 able_recipe-1.0.8/able/src/org/able/BLEAdvertiser.java
--rw-r--r--   0 runner    (1001) docker     (121)     1215 2021-08-15 20:35:46.000000 able_recipe-1.0.8/able/src/org/able/PythonBluetooth.java
--rw-r--r--   0 runner    (1001) docker     (121)      671 2021-08-15 20:35:46.000000 able_recipe-1.0.8/able/src/org/able/PythonBluetoothAdvertiser.java
--rw-r--r--   0 runner    (1001) docker     (121)     2277 2021-08-15 20:35:46.000000 able_recipe-1.0.8/able/structures.py
--rw-r--r--   0 runner    (1001) docker     (121)      946 2021-08-15 20:35:46.000000 able_recipe-1.0.8/able/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-08-15 20:35:46.000000 able_recipe-1.0.8/able/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-15 20:36:00.000000 able_recipe-1.0.8/able_recipe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3503 2021-08-15 20:36:00.000000 able_recipe-1.0.8/able_recipe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      570 2021-08-15 20:36:00.000000 able_recipe-1.0.8/able_recipe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-15 20:36:00.000000 able_recipe-1.0.8/able_recipe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-15 20:36:00.000000 able_recipe-1.0.8/able_recipe.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        5 2021-08-15 20:36:00.000000 able_recipe-1.0.8/able_recipe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-08-15 20:36:00.000000 able_recipe-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2828 2021-08-15 20:35:46.000000 able_recipe-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 19:12:16.000000 able_recipe-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1417 2021-12-15 19:12:07.000000 able_recipe-1.0.9/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1071 2021-12-15 19:12:07.000000 able_recipe-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       90 2021-12-15 19:12:07.000000 able_recipe-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     3501 2021-12-15 19:12:16.000000 able_recipe-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2187 2021-12-15 19:12:07.000000 able_recipe-1.0.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 19:12:16.000000 able_recipe-1.0.9/able/
+-rw-r--r--   0 runner    (1001) docker     (121)     1895 2021-12-15 19:12:07.000000 able_recipe-1.0.9/able/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10840 2021-12-15 19:12:07.000000 able_recipe-1.0.9/able/advertising.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 19:12:16.000000 able_recipe-1.0.9/able/android/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-15 19:12:07.000000 able_recipe-1.0.9/able/android/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5869 2021-12-15 19:12:07.000000 able_recipe-1.0.9/able/android/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6411 2021-12-15 19:12:07.000000 able_recipe-1.0.9/able/android/jni.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11136 2021-12-15 19:12:07.000000 able_recipe-1.0.9/able/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7843 2021-12-15 19:12:07.000000 able_recipe-1.0.9/able/filters.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2217 2021-12-15 19:12:07.000000 able_recipe-1.0.9/able/queue.py
+-rw-r--r--   0 runner    (1001) docker     (121)      690 2021-12-15 19:12:07.000000 able_recipe-1.0.9/able/scan_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 19:12:16.000000 able_recipe-1.0.9/able/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 19:12:16.000000 able_recipe-1.0.9/able/src/org/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 19:12:16.000000 able_recipe-1.0.9/able/src/org/able/
+-rw-r--r--   0 runner    (1001) docker     (121)    11891 2021-12-15 19:12:07.000000 able_recipe-1.0.9/able/src/org/able/BLE.java
+-rw-r--r--   0 runner    (1001) docker     (121)     2834 2021-12-15 19:12:07.000000 able_recipe-1.0.9/able/src/org/able/BLEAdvertiser.java
+-rw-r--r--   0 runner    (1001) docker     (121)     1188 2021-12-15 19:12:07.000000 able_recipe-1.0.9/able/src/org/able/PythonBluetooth.java
+-rw-r--r--   0 runner    (1001) docker     (121)      671 2021-12-15 19:12:07.000000 able_recipe-1.0.9/able/src/org/able/PythonBluetoothAdvertiser.java
+-rw-r--r--   0 runner    (1001) docker     (121)     2277 2021-12-15 19:12:07.000000 able_recipe-1.0.9/able/structures.py
+-rw-r--r--   0 runner    (1001) docker     (121)      946 2021-12-15 19:12:07.000000 able_recipe-1.0.9/able/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2021-12-15 19:12:08.000000 able_recipe-1.0.9/able/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 19:12:16.000000 able_recipe-1.0.9/able_recipe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3501 2021-12-15 19:12:16.000000 able_recipe-1.0.9/able_recipe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      608 2021-12-15 19:12:16.000000 able_recipe-1.0.9/able_recipe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-15 19:12:16.000000 able_recipe-1.0.9/able_recipe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-15 19:12:16.000000 able_recipe-1.0.9/able_recipe.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2021-12-15 19:12:16.000000 able_recipe-1.0.9/able_recipe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-15 19:12:16.000000 able_recipe-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2828 2021-12-15 19:12:07.000000 able_recipe-1.0.9/setup.py
```

### Comparing `able_recipe-1.0.8/CHANGELOG.rst` & `able_recipe-1.0.9/CHANGELOG.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changelog
 =========
 
+1.0.9
+-----
+
+* Switched from deprecated scanning method `BluetoothAdapter.startLeScan` to `BluetoothLeScanner.startScan`
+* Added support for BLE scanning settings: `able.scan_settings` module
+* Added support for BLE scanning filters: `able.filters` module
+
+
 1.0.8
 -----
 
 * Added support to use `able` in Android services
 * Added decorators:
 
   - `able.require_bluetooth_enabled`: to call `BluetoothDispatcher` method when bluetooth adapter becomes ready
```

### Comparing `able_recipe-1.0.8/LICENSE` & `able_recipe-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `able_recipe-1.0.8/PKG-INFO` & `able_recipe-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: able_recipe
-Version: 1.0.8
+Version: 1.0.9
 Summary: Bluetooth Low Energy for Android
 Home-page: https://github.com/b3b/able
 Author: b3b
 Author-email: ash.b3b@gmail.com
 License: MIT
 Project-URL: Changelog, https://github.com/b3b/able/blob/master/CHANGELOG.rst
 Description: Android Bluetooth Low Energy
@@ -67,15 +67,15 @@
         
             `andfmart <https://github.com/andfmart>`_
             `andreamerello <https://github.com/andreamerello>`_
             `datmaniac95  <https://github.com/datmaniac95>`_
             `dgatf <https://github.com/dgatf>`_
             `dwmoffatt <https://github.com/dwmoffatt>`_
             `Enkumicahel <https://github.com/Enkumicahel>`_
-            `FalkorDev <https://github.com/FalkorDev>`_
+            `HelaFaye <https://github.com/HelaFaye>`_
             `jacklinquan <https://github.com/jacklinquan>`_
             `juasiepo <https://github.com/juasiepo>`_
             `PapoKarlo <https://github.com/PapoKarlo>`_
             `RoberWare <https://github.com/RoberWare>`_
             `sooko_io <https://github.com/sooko>`_
         
 Keywords: android ble bluetooth kivy
```

### Comparing `able_recipe-1.0.8/README.rst` & `able_recipe-1.0.9/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -58,13 +58,13 @@
 
     `andfmart <https://github.com/andfmart>`_
     `andreamerello <https://github.com/andreamerello>`_
     `datmaniac95  <https://github.com/datmaniac95>`_
     `dgatf <https://github.com/dgatf>`_
     `dwmoffatt <https://github.com/dwmoffatt>`_
     `Enkumicahel <https://github.com/Enkumicahel>`_
-    `FalkorDev <https://github.com/FalkorDev>`_
+    `HelaFaye <https://github.com/HelaFaye>`_
     `jacklinquan <https://github.com/jacklinquan>`_
     `juasiepo <https://github.com/juasiepo>`_
     `PapoKarlo <https://github.com/PapoKarlo>`_
     `RoberWare <https://github.com/RoberWare>`_
     `sooko_io <https://github.com/sooko>`_
```

### Comparing `able_recipe-1.0.8/able/__init__.py` & `able_recipe-1.0.9/able/__init__.py`

 * *Files identical despite different names*

### Comparing `able_recipe-1.0.8/able/advertising.py` & `able_recipe-1.0.9/able/advertising.py`

 * *Files identical despite different names*

### Comparing `able_recipe-1.0.8/able/android/dispatcher.py` & `able_recipe-1.0.9/able/android/dispatcher.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,17 @@
     request_permission,
 )
 from jnius import autoclass
 from kivy.logger import Logger
 
 from able.android.jni import PythonBluetooth
 from able.dispatcher import BluetoothDispatcherBase
+from able.scan_settings import ScanSettingsBuilder
 
+ArrayList = autoclass('java.util.ArrayList')
 
 Activity = autoclass('android.app.Activity')
 BLE = autoclass('org.able.BLE')
 
 BluetoothAdapter = autoclass('android.bluetooth.BluetoothAdapter')
 BluetoothDevice = autoclass('android.bluetooth.BluetoothDevice')
 BluetoothGattDescriptor = autoclass('android.bluetooth.BluetoothGattDescriptor')
@@ -85,16 +87,25 @@
 
     def _request_runtime_permissions(self):
         request_permission(Permission.ACCESS_FINE_LOCATION,
                            self.on_runtime_permissions)
 
     @require_bluetooth_enabled
     @require_runtime_permissions
-    def start_scan(self):
-        self._ble.startScan(self.enable_ble_code)
+    def start_scan(self, filters=None, settings=None):
+        filters_array = ArrayList()
+        for f in filters or []:
+            filters_array.add(f.build())
+        if not settings:
+            settings = ScanSettingsBuilder()
+        try:
+            settings = settings.build()
+        except AttributeError:
+            pass
+        self._ble.startScan(self.enable_ble_code, filters_array, settings)
 
     def stop_scan(self):
         self._ble.stopScan()
 
     @require_bluetooth_enabled
     def connect_by_device_address(self, address: str):
         address = address.upper()
```

### Comparing `able_recipe-1.0.8/able/android/jni.py` & `able_recipe-1.0.9/able/android/jni.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,18 +13,31 @@
         self.dispatcher = dispatcher
 
     @java_method('(Ljava/lang/String;)V')
     def on_error(self, msg):
         Logger.debug("on_error")
         self.dispatcher.dispatch('on_error', msg)
 
-    @java_method('(Landroid/bluetooth/BluetoothDevice;I[B)V')
-    def on_device(self, device, rssi, record):
-        self.dispatcher.dispatch('on_device', device, rssi,
-                                 Advertisement(record))
+    @java_method('(Landroid/bluetooth/le/ScanResult;)V')
+    def on_scan_result(self, result):
+        device = result.getDevice()  # type: android.bluetooth.BluetoothDevice
+        record = result.getScanRecord()  # type: android.bluetooth.le.ScanRecord
+        if record:
+            self.dispatcher.dispatch(
+                'on_device',
+                device,
+                result.getRssi(),
+                Advertisement(record.getBytes())
+            )
+        else:
+            Logger.warning(
+                "Scan result for device without the scan record: %s",
+                device
+            )
+
 
     @java_method('(Z)V')
     def on_scan_started(self, success):
         Logger.debug("on_scan_started")
         self.dispatcher.dispatch('on_scan_started', success)
 
     @java_method('()V')
```

### Comparing `able_recipe-1.0.8/able/dispatcher.py` & `able_recipe-1.0.9/able/dispatcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-from typing import Optional
+from typing import List, Optional
 
 from kivy.event import EventDispatcher
 from kivy.logger import Logger
 
 from able import WriteType
+from able.filters import Filter
 from able.queue import BLEQueue, ble_task, ble_task_done
 from able.utils import force_convertible_to_java_array
+from able.scan_settings import ScanSettingsBuilder
 
 
 class BLEError(object):
     """raise Exception on attribute access
     """
 
     def __init__(self, msg):
@@ -100,21 +102,30 @@
 
     def set_queue_timeout(self, timeout):
         """Change the BLE operations queue timeout
         """
         self.queue_timeout = timeout
         self.queue.set_timeout(timeout)
 
-    def start_scan(self):
+    def start_scan(
+            self,
+            filters: Optional[List[Filter]]=None,
+            settings: Optional[ScanSettingsBuilder]=None
+    ):
         """Start a scan for devices.
         Ask for runtime permission to access location.
         Start a system activity that allows the user to turn on Bluetooth,
         if Bluetooth is not enabled.
         The status of the scan start are reported with
         :func:`scan_started <on_scan_started>` event.
+
+        :param filters: list of filters to restrict scan results.
+                        Advertising record is considered matching the filters
+                        if it matches any of the :class:`able.filters.Filter` in the list.
+        :param settings: scan settings
         """
         pass
 
     def stop_scan(self):
         """Stop the ongoing scan for devices.
         """
         pass
```

### Comparing `able_recipe-1.0.8/able/queue.py` & `able_recipe-1.0.9/able/queue.py`

 * *Files identical despite different names*

### Comparing `able_recipe-1.0.8/able/src/org/able/BLE.java` & `able_recipe-1.0.9/able/src/org/able/BLE.java`

 * *Files 5% similar despite different names*

```diff
@@ -9,27 +9,35 @@
 import android.bluetooth.BluetoothDevice;
 import android.bluetooth.BluetoothProfile;
 import android.bluetooth.BluetoothGatt;
 import android.bluetooth.BluetoothGattCallback;
 import android.bluetooth.BluetoothGattCharacteristic;
 import android.bluetooth.BluetoothGattDescriptor;
 import android.bluetooth.BluetoothGattService;
+import android.bluetooth.le.BluetoothLeScanner;
+import android.bluetooth.le.ScanCallback;
+import android.bluetooth.le.ScanResult;
+
+import android.bluetooth.le.ScanFilter;
+import android.bluetooth.le.ScanSettings;
+
 import android.os.Handler;
 import android.util.Log;
 import java.util.List;
 import org.kivy.android.PythonActivity;
 import org.kivy.android.PythonService;
 import org.able.PythonBluetooth;
 
 
 public class BLE {
         private String TAG = "BLE-python";
         private PythonBluetooth mPython;
         private Context mContext;
         private BluetoothAdapter mBluetoothAdapter;
+        private BluetoothLeScanner mBluetoothLeScanner;
         private BluetoothGatt mBluetoothGatt;
         private List<BluetoothGattService> mBluetoothGattServices;
         private boolean mScanning;
         private boolean mIsServiceContext = false;
 
         public void showError(final String msg) {
                 Log.e(TAG, msg);
@@ -78,54 +86,76 @@
                 return mBluetoothAdapter;
         }
 
         public BluetoothGatt getGatt() {
                 return mBluetoothGatt;
         }
 
-        public void startScan(int EnableBtCode) {
+        public void startScan(int EnableBtCode,
+                              List<ScanFilter> filters,
+                              ScanSettings settings) {
                 Log.d(TAG, "startScan");
                 BluetoothAdapter adapter = getAdapter(EnableBtCode);
                 if (adapter != null) {
                     Log.d(TAG, "BLE adapter is ready for scan");
-                    if (adapter.startLeScan(mLeScanCallback)) {
-                            Log.d(TAG, "BLE scan started successfully");
-                            mScanning = true;
-                            mPython.on_scan_started(true);
+                    if (mBluetoothLeScanner == null) {
+                            mBluetoothLeScanner = adapter.getBluetoothLeScanner();
+                    }
+                    if (mBluetoothLeScanner != null) {
+                            mScanning = false;
+                            mBluetoothLeScanner.startScan(filters, settings, mScanCallback);
                     } else {
-                            Log.d(TAG, "BLE scan not started");
+                            showError("Could not get BLE Scanner object.");
                             mPython.on_scan_started(false);
                     }
                 }
         }
 
         public void stopScan() {
-                if (mScanning == true) {
+                if (mBluetoothLeScanner != null) {
                         Log.d(TAG, "stopScan");
-                        mScanning = false;
-                        mBluetoothAdapter.stopLeScan(mLeScanCallback);
-                        mPython.on_scan_completed();
+                        mBluetoothLeScanner.stopScan(mScanCallback);
+                        if (mScanning) {
+                                mScanning = false;
+                                mPython.on_scan_completed();
+                        }
                 }
         }
 
-        private BluetoothAdapter.LeScanCallback mLeScanCallback =
-                new BluetoothAdapter.LeScanCallback() {
+        private final ScanCallback mScanCallback =
+                new ScanCallback() {
                         @Override
-                        public void onLeScan(final BluetoothDevice device, final int rssi, final byte[] scanRecord) {
+                        public void onScanResult(final int callbackType, final ScanResult result) {
+                                if (!mScanning) {
+                                        mScanning = true;
+                                        Log.d(TAG, "BLE scan started successfully");
+                                        mPython.on_scan_started(true);
+                                }
                                 if (mIsServiceContext) {
-                                        mPython.on_device(device, rssi, scanRecord);
+                                        mPython.on_scan_result(result);
                                         return;
                                 }
                                 PythonActivity.mActivity.runOnUiThread(new Runnable() {
                                                 @Override
                                                 public void run() {
-                                                        mPython.on_device(device, rssi, scanRecord);
+                                                        mPython.on_scan_result(result);
                                                 }
                                         });
                         }
+
+                        @Override
+                        public void onBatchScanResults(List<ScanResult> results) {
+                                Log.d(TAG, "onBatchScanResults");
+                        }
+
+                        @Override
+                        public void onScanFailed(int errorCode) {
+                                Log.e(TAG, "BLE Scan failed, error code:" + errorCode);
+                                mPython.on_scan_started(false);
+                        }
                 };
 
         public void connectGatt(BluetoothDevice device) {
                 Log.d(TAG, "connectGatt");
                 if (mBluetoothGatt == null) {
                         mBluetoothGatt = device.connectGatt(mContext, false, mGattCallback, BluetoothDevice.TRANSPORT_LE);
                 }
```

### Comparing `able_recipe-1.0.8/able/src/org/able/BLEAdvertiser.java` & `able_recipe-1.0.9/able/src/org/able/BLEAdvertiser.java`

 * *Files identical despite different names*

### Comparing `able_recipe-1.0.8/able/src/org/able/PythonBluetooth.java` & `able_recipe-1.0.9/able/src/org/able/PythonBluetooth.java`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 package org.able;
 
 import java.util.List;
-import android.bluetooth.BluetoothDevice;
 import android.bluetooth.BluetoothGattService;
 import android.bluetooth.BluetoothGattCharacteristic;
 import android.bluetooth.BluetoothGattDescriptor;
+import android.bluetooth.le.ScanResult;
 
 interface PythonBluetooth
 {
         public void on_error(String msg);
-        public void on_device(BluetoothDevice device, int rssi, byte[] record);
         public void on_scan_started(boolean success);
+        public void on_scan_result(ScanResult result);
         public void on_scan_completed();
         public void on_services(int status, List<BluetoothGattService> services);
         public void on_characteristic_changed(BluetoothGattCharacteristic characteristic);
         public void on_characteristic_read(BluetoothGattCharacteristic characteristic, int status);
         public void on_characteristic_write(BluetoothGattCharacteristic characteristic, int status);
         public void on_descriptor_read(BluetoothGattDescriptor descriptor, int status);
         public void on_descriptor_write(BluetoothGattDescriptor descriptor, int status);
```

### Comparing `able_recipe-1.0.8/able/src/org/able/PythonBluetoothAdvertiser.java` & `able_recipe-1.0.9/able/src/org/able/PythonBluetoothAdvertiser.java`

 * *Files identical despite different names*

### Comparing `able_recipe-1.0.8/able/structures.py` & `able_recipe-1.0.9/able/structures.py`

 * *Files identical despite different names*

### Comparing `able_recipe-1.0.8/able/utils.py` & `able_recipe-1.0.9/able/utils.py`

 * *Files identical despite different names*

### Comparing `able_recipe-1.0.8/able_recipe.egg-info/PKG-INFO` & `able_recipe-1.0.9/able_recipe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: able-recipe
-Version: 1.0.8
+Version: 1.0.9
 Summary: Bluetooth Low Energy for Android
 Home-page: https://github.com/b3b/able
 Author: b3b
 Author-email: ash.b3b@gmail.com
 License: MIT
 Project-URL: Changelog, https://github.com/b3b/able/blob/master/CHANGELOG.rst
 Description: Android Bluetooth Low Energy
@@ -67,15 +67,15 @@
         
             `andfmart <https://github.com/andfmart>`_
             `andreamerello <https://github.com/andreamerello>`_
             `datmaniac95  <https://github.com/datmaniac95>`_
             `dgatf <https://github.com/dgatf>`_
             `dwmoffatt <https://github.com/dwmoffatt>`_
             `Enkumicahel <https://github.com/Enkumicahel>`_
-            `FalkorDev <https://github.com/FalkorDev>`_
+            `HelaFaye <https://github.com/HelaFaye>`_
             `jacklinquan <https://github.com/jacklinquan>`_
             `juasiepo <https://github.com/juasiepo>`_
             `PapoKarlo <https://github.com/PapoKarlo>`_
             `RoberWare <https://github.com/RoberWare>`_
             `sooko_io <https://github.com/sooko>`_
         
 Keywords: android ble bluetooth kivy
```

### Comparing `able_recipe-1.0.8/able_recipe.egg-info/SOURCES.txt` & `able_recipe-1.0.9/able_recipe.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 LICENSE
 MANIFEST.in
 README.rst
 setup.py
 able/__init__.py
 able/advertising.py
 able/dispatcher.py
+able/filters.py
 able/queue.py
+able/scan_settings.py
 able/structures.py
 able/utils.py
 able/version.py
 able/android/__init__.py
 able/android/dispatcher.py
 able/android/jni.py
 able/src/org/able/BLE.java
```

### Comparing `able_recipe-1.0.8/setup.py` & `able_recipe-1.0.9/setup.py`

 * *Files identical despite different names*

