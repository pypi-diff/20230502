# Comparing `tmp/napari-sam-0.3.8.tar.gz` & `tmp/napari-sam-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-sam-0.3.8.tar", last modified: Mon Apr 17 14:11:09 2023, max compression
+gzip compressed data, was "napari-sam-0.3.9.tar", last modified: Tue Apr 18 08:56:21 2023, max compression
```

## Comparing `napari-sam-0.3.8.tar` & `napari-sam-0.3.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:09.857162 napari-sam-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-17 14:10:51.000000 napari-sam-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-17 14:10:51.000000 napari-sam-0.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-04-17 14:11:09.857162 napari-sam-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-04-17 14:10:51.000000 napari-sam-0.3.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-17 14:10:51.000000 napari-sam-0.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-17 14:11:09.857162 napari-sam-0.3.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:09.853162 napari-sam-0.3.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:09.857162 napari-sam-0.3.8/src/napari_sam/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-17 14:10:51.000000 napari-sam-0.3.8/src/napari_sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39534 2023-04-17 14:10:51.000000 napari-sam-0.3.8/src/napari_sam/_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-17 14:10:51.000000 napari-sam-0.3.8/src/napari_sam/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-17 14:10:51.000000 napari-sam-0.3.8/src/napari_sam/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:09.857162 napari-sam-0.3.8/src/napari_sam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-04-17 14:11:09.000000 napari-sam-0.3.8/src/napari_sam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-17 14:11:09.000000 napari-sam-0.3.8/src/napari_sam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 14:11:09.000000 napari-sam-0.3.8/src/napari_sam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-17 14:11:09.000000 napari-sam-0.3.8/src/napari_sam.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-17 14:11:09.000000 napari-sam-0.3.8/src/napari_sam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-17 14:11:09.000000 napari-sam-0.3.8/src/napari_sam.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:56:21.862763 napari-sam-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-18 08:56:04.000000 napari-sam-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-18 08:56:04.000000 napari-sam-0.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-04-18 08:56:21.862763 napari-sam-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-04-18 08:56:04.000000 napari-sam-0.3.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-18 08:56:04.000000 napari-sam-0.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-18 08:56:21.862763 napari-sam-0.3.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:56:21.858762 napari-sam-0.3.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:56:21.862763 napari-sam-0.3.9/src/napari_sam/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-18 08:56:04.000000 napari-sam-0.3.9/src/napari_sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38882 2023-04-18 08:56:04.000000 napari-sam-0.3.9/src/napari_sam/_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-18 08:56:04.000000 napari-sam-0.3.9/src/napari_sam/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-18 08:56:04.000000 napari-sam-0.3.9/src/napari_sam/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:56:21.862763 napari-sam-0.3.9/src/napari_sam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-04-18 08:56:21.000000 napari-sam-0.3.9/src/napari_sam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-18 08:56:21.000000 napari-sam-0.3.9/src/napari_sam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:56:21.000000 napari-sam-0.3.9/src/napari_sam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-18 08:56:21.000000 napari-sam-0.3.9/src/napari_sam.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-18 08:56:21.000000 napari-sam-0.3.9/src/napari_sam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-18 08:56:21.000000 napari-sam-0.3.9/src/napari_sam.egg-info/top_level.txt
```

### Comparing `napari-sam-0.3.8/LICENSE` & `napari-sam-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-sam-0.3.8/PKG-INFO` & `napari-sam-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-sam
-Version: 0.3.8
+Version: 0.3.9
 Summary: Segment anything with Meta AI's new SAM model!
 Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: napari-sam Version: 0.3.8 Summary: Segment anything
+Metadata-Version: 2.1 Name: napari-sam Version: 0.3.9 Summary: Segment anything
 with Meta AI's new SAM model! Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski Author-email: karol.gotkowski@dkfz.de License: Apache-
 2.0 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
 Project-URL: Source Code, https://github.com/MIC-DKFZ/napari-sam Project-URL:
 User Support, https://github.com/MIC-DKFZ/napari-sam/issues Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Framework :: napari Classifier:
```

### Comparing `napari-sam-0.3.8/README.md` & `napari-sam-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `napari-sam-0.3.8/setup.cfg` & `napari-sam-0.3.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-sam-0.3.8/src/napari_sam/_widget.py` & `napari-sam-0.3.9/src/napari_sam/_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -502,36 +502,37 @@
         self.label_layer.data = self.label_layer.data
 
     def on_contrast_limits_change(self):
         print("Contrast limit change")
         self.set_image()
 
     def set_image(self):
-        image = np.asarray(self.image_layer.data)
         if self.image_layer.ndim == 2:
+            image = np.asarray(self.image_layer.data)
             if not self.image_layer.rgb:
                 image = np.stack((image,)*3, axis=-1)  # Expand to 3-channel image
             image = image[..., :3]  # Remove a potential alpha channel
             self.sam_predictor.set_image(image)
             self.sam_features = self.sam_predictor.features
         elif self.image_layer.ndim == 3:
             l_creating_features= QLabel("Creating SAM image embedding:")
             self.layout().addWidget(l_creating_features)
             progress_bar = QProgressBar(self)
-            progress_bar.setMaximum(image.shape[0])
+            progress_bar.setMaximum(self.image_layer.data.shape[0])
             progress_bar.setValue(0)
             self.layout().addWidget(progress_bar)
-            if not self.image_layer.rgb:
-                image = np.stack((image,) * 3, axis=-1)  # Expand to 3-channel image
-            image = image[..., :3]  # Remove a potential alpha channel
-            contrast_limits = self.image_layer.contrast_limits
-            image = normalize(image, source_limits=contrast_limits, target_limits=(0, 255)).astype(np.uint8)
             self.sam_features = []
-            for index in tqdm(range(image.shape[0]), desc="Creating SAM image embedding"):
-                self.sam_predictor.set_image(image[index, :, :, :])
+            for index in tqdm(range(self.image_layer.data.shape[0]), desc="Creating SAM image embedding"):
+                image_slice = np.asarray(self.image_layer.data[index, ...])
+                if not self.image_layer.rgb:
+                    image_slice = np.stack((image_slice,) * 3, axis=-1)  # Expand to 3-channel image
+                image_slice = image_slice[..., :3]  # Remove a potential alpha channel
+                contrast_limits = self.image_layer.contrast_limits
+                image_slice = normalize(image_slice, source_limits=contrast_limits, target_limits=(0, 255)).astype(np.uint8)
+                self.sam_predictor.set_image(image_slice)
                 self.sam_features.append(self.sam_predictor.features)
                 progress_bar.setValue(index+1)
                 QApplication.processEvents()
                 progress_bar.deleteLater()
                 l_creating_features.deleteLater()
         else:
             raise RuntimeError("Only 2D and 3D images are supported.")
@@ -609,28 +610,14 @@
                 point_labels=np.asarray(group_labels),
                 mask_input=self.sam_logits[x_coord],
                 multimask_output=False,
             )
             prediction_yz = prediction_yz[0]
             prediction[x_coord, :, :] = prediction_yz
             predicted_slices = x_coord
-
-            # for x_coord, group_points in groups.items():
-            #     group_labels = [labels[np.argwhere(np.all(points == point, axis=1)).flatten()[0]] for point in group_points]
-            #     group_points = [point[1:] for point in group_points]
-            #     self.sam_predictor.features = self.sam_features[x_coord]
-            #     prediction_yz, _, _ = self.sam_predictor.predict(
-            #         point_coords=np.flip(group_points, axis=-1),
-            #         point_labels=np.asarray(group_labels),
-            #         mask_input=self.sam_logits,
-            #         multimask_output=False,
-            #     )
-            #     prediction_yz = prediction_yz[0]
-            #     prediction[x_coord, :, :] = prediction_yz
-            sam_logits = None  # TODO: Use sam_logits
         # elif self.image_layer.ndim == 3:
         #     z_coords = np.unique(points[:, 2])
         #     groups = {x_coord: list(points[points[:, 2] == x_coord]) for x_coord in z_coords}  # Group points if they are on the same image slice
         #     image_point_proposals, image_label_proposals = [], []
         #
         #     for x_coord, group_points in groups.items():
         #         group_labels = [labels[np.argwhere(np.all(points == point, axis=1)).flatten()[0]] for point in group_points]
```

### Comparing `napari-sam-0.3.8/src/napari_sam/utils.py` & `napari-sam-0.3.9/src/napari_sam/utils.py`

 * *Files identical despite different names*

### Comparing `napari-sam-0.3.8/src/napari_sam.egg-info/PKG-INFO` & `napari-sam-0.3.9/src/napari_sam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-sam
-Version: 0.3.8
+Version: 0.3.9
 Summary: Segment anything with Meta AI's new SAM model!
 Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: napari-sam Version: 0.3.8 Summary: Segment anything
+Metadata-Version: 2.1 Name: napari-sam Version: 0.3.9 Summary: Segment anything
 with Meta AI's new SAM model! Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski Author-email: karol.gotkowski@dkfz.de License: Apache-
 2.0 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
 Project-URL: Source Code, https://github.com/MIC-DKFZ/napari-sam Project-URL:
 User Support, https://github.com/MIC-DKFZ/napari-sam/issues Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Framework :: napari Classifier:
```

