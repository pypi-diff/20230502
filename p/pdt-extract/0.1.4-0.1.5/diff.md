# Comparing `tmp/pdt_extract-0.1.4-py3-none-any.whl.zip` & `tmp/pdt_extract-0.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 10635 bytes, number of entries: 8
+Zip file size: 10693 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat    11413 b- defN 23-Apr-25 23:53 pdt_canny.py
--rw-rw-rw-  2.0 fat       74 b- defN 23-Apr-26 19:26 pdt_extract/__init__.py
--rw-rw-rw-  2.0 fat     5714 b- defN 23-Apr-28 19:45 pdt_extract/feature_extract.py
--rw-rw-rw-  2.0 fat    11582 b- defN 23-Apr-28 15:55 pdt_extract/pdt_extract.py
--rw-rw-rw-  2.0 fat      662 b- defN 23-Apr-28 19:48 pdt_extract-0.1.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-28 19:48 pdt_extract-0.1.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-Apr-28 19:48 pdt_extract-0.1.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      632 b- defN 23-Apr-28 19:48 pdt_extract-0.1.4.dist-info/RECORD
-8 files, 30181 bytes uncompressed, 9535 bytes compressed:  68.4%
+-rw-rw-rw-  2.0 fat      136 b- defN 23-May-02 13:45 pdt_extract/__init__.py
+-rw-rw-rw-  2.0 fat     5716 b- defN 23-Apr-28 23:10 pdt_extract/feature_extract.py
+-rw-rw-rw-  2.0 fat    11583 b- defN 23-May-02 13:36 pdt_extract/pdt_extract.py
+-rw-rw-rw-  2.0 fat      662 b- defN 23-May-02 13:46 pdt_extract-0.1.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-02 13:46 pdt_extract-0.1.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-May-02 13:46 pdt_extract-0.1.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      633 b- defN 23-May-02 13:46 pdt_extract-0.1.5.dist-info/RECORD
+8 files, 30247 bytes uncompressed, 9593 bytes compressed:  68.3%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: pdt_extract/feature_extract.py
 Comment: 
 
 Filename: pdt_extract/pdt_extract.py
 Comment: 
 
-Filename: pdt_extract-0.1.4.dist-info/METADATA
+Filename: pdt_extract-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: pdt_extract-0.1.4.dist-info/WHEEL
+Filename: pdt_extract-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: pdt_extract-0.1.4.dist-info/top_level.txt
+Filename: pdt_extract-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: pdt_extract-0.1.4.dist-info/RECORD
+Filename: pdt_extract-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pdt_extract/__init__.py

```diff
@@ -1,2 +1,3 @@
 from pdt_extract.pdt_extract import DropProfile
-__all__ = ['DropProfile']
+from feature_extract import FeatureExtract
+__all__ = ['DropProfile', 'FeatureExtract']
```

## pdt_extract/feature_extract.py

```diff
@@ -34,35 +34,34 @@
         self.y = y
 
         self.capillary_radius = self.x[-1]
         self.drop_height = self.y[0]
         self.equator_radius = self.find_equator_radius()
         self.s_radius = self.find_s_radius()
         self.apex_radius = self.find_apex_radius()
+        # Normalize to dimensionless ratio to apex radius
         self.feature_set = {
-            "Apex radius": self.apex_radius,
-            "Equator radius": self.equator_radius / self.apex_radius,
-            "S_radius": self.s_radius / self.apex_radius,
+            "Drop height": self.drop_height / self.apex_radius,
             "Capillary radius": self.capillary_radius / self.apex_radius,
-            "Drop height": self.drop_height / self.apex_radius
+            "R-s": self.s_radius / self.apex_radius,
+            "R-e": self.equator_radius / self.apex_radius,
         }
-        print(f"Apex radius: {self.apex_radius }")
-        print(f"Equator radius: {self.equator_radius },"
-              f"S radius: {self.s_radius },"
-              f"Capillary radius: {self.capillary_radius},"
+        print(f"Apex radius (Pixels): {self.apex_radius }")
+        print(f"Equator radius: {self.equator_radius }\n"
+              f"S radius: {self.s_radius }\n"
+              f"Capillary radius: {self.capillary_radius}\n"
               f"Drop Height: {self.drop_height }")
 
     def average_x(self, i: int, n: int) -> int:
         s = 0
         for j in range(i-n, i+n+1):
             s = s + self.x[j]
         return s / (2 * n + 1)
 
     def recursive_equator_radius(self, i, n):
-        global r_e
         # use recursive approach: start from apex, continue until x decreases
         # at i-th point we average x of x-n to x+n to suppress noise
         # compare x-i_th vs x_i+t_th until it decreases to find equator
         if self.average_x(i, n) < self.average_x(i+1, n) and i <= len(self.x) - n-3:
             i += 1
             output = self.recursive_equator_radius(i, n)
             if output:
@@ -130,13 +129,13 @@
 
         return r_0[-1]
 
     # Find maximum (bulge) x value from 70% of profile
     def find_equator_radius(self):
         split = int(len(self.x) * 0.7)
 
-        # Slice the first 70% of the list and find the maximum value
+        # Slice the first 70% of the list from bottom and find the maximum value
         return max(self.x[:split])
 
     # Find radius at point X = [2 * equator_radius] between capillary and equator
     def find_s_radius(self):
         return self.x[-2 * int(self.equator_radius)]
```

## pdt_extract/pdt_extract.py

```diff
@@ -81,15 +81,15 @@
 
         # Create ordered set of X and Y coordinates along edge profile
         indices = np.where(final_image == 255)
         x = np.flip(indices[1])
         y = np.flip(indices[0])
         # Extract and save profile features to feature list
         features = FeatureExtract(x, y)
-        features.feature_set["image"] = filename
+        #features.feature_set["image"] = filename
         self.feature_list.append(features.feature_set)
         show_image(final_image)
 
         fft_profile(final_image)
         if save:
             imageio.imwrite(filename, np.uint8(final_image))
         else:
```

## Comparing `pdt_extract-0.1.4.dist-info/METADATA` & `pdt_extract-0.1.5.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdt-extract
-Version: 0.1.4
+Version: 0.1.5
 Summary: Perform edge profile and characteristic feature extraction from images of pendant drops
 Home-page: https://github.com/DmitriLyalikov/pdt-canny-edge-detector
 Author: Dmitri Lyalikov
 Author-email: Dlyalikov01@manhattan.edu
 Classifier: Intended Audience :: Science/Research
 Description-Content-Type: text/markdown
 Requires-Dist: imageio
```

## Comparing `pdt_extract-0.1.4.dist-info/RECORD` & `pdt_extract-0.1.5.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 pdt_canny.py,sha256=H9B7o4vPiWQoMjiu6J8d5uIk2FHaCQNmWz0NMTOuF3Y,11413
-pdt_extract/__init__.py,sha256=4lNIpyPWiCe7y_Ksf3ZEb9qB0D7WJ1FMJGDwY0Qywjg,74
-pdt_extract/feature_extract.py,sha256=w-aKaQ2Mm0U3ITQ8Ygro1IlrSDxi2n_2Zyy5FVea0b8,5714
-pdt_extract/pdt_extract.py,sha256=nPiGN4Y8G8Mm2nJghk2qdeQ5mpi3bQzWPinW2KjBHbo,11582
-pdt_extract-0.1.4.dist-info/METADATA,sha256=1DaEGpF6olHaFsXi-IeRWS9GudNz27eVoobf6blndRI,662
-pdt_extract-0.1.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pdt_extract-0.1.4.dist-info/top_level.txt,sha256=QCEOHNPwd72hz8668WATwVkOuYdskgLisqco3A-kRSQ,12
-pdt_extract-0.1.4.dist-info/RECORD,,
+pdt_extract/__init__.py,sha256=Rrbng7A3AgRRnkEZxVNjpQrgwkbf0ktT9DHLcrhndks,136
+pdt_extract/feature_extract.py,sha256=gsBApWn69007cWyjqczPfDfZYcEftdKcsAfO9VXTkJs,5716
+pdt_extract/pdt_extract.py,sha256=lkMw_Dhdd8Ue3R82M8ZaKlvUo3FeL_IYVLjauAZrVJA,11583
+pdt_extract-0.1.5.dist-info/METADATA,sha256=TSvU5cAwlDPRsBvRKDRm0e4RMq4CpsOmWdBbYgaoJ1o,662
+pdt_extract-0.1.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pdt_extract-0.1.5.dist-info/top_level.txt,sha256=QCEOHNPwd72hz8668WATwVkOuYdskgLisqco3A-kRSQ,12
+pdt_extract-0.1.5.dist-info/RECORD,,
```

