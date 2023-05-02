# Comparing `tmp/bandplot-0.1.3.1-py3-none-any.whl.zip` & `tmp/bandplot-0.1.3.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 9274 bytes, number of entries: 9
--rwxrwxrwx  2.0 unx       26 b- defN 23-Mar-30 18:56 bandplot/__init__.py
--rwxrwxrwx  2.0 unx    27604 b- defN 23-Mar-05 05:05 bandplot/plots.py
--rwxrwxrwx  2.0 unx     5809 b- defN 23-Mar-10 00:34 bandplot/readdata.py
--rwxrwxrwx  2.0 unx    15274 b- defN 23-Apr-15 22:51 bandplot/wrapper.py
--rwxrwxrwx  2.0 unx     2901 b- defN 23-Apr-15 23:02 bandplot-0.1.3.1.dist-info/METADATA
--rwxrwxrwx  2.0 unx       92 b- defN 23-Apr-15 23:02 bandplot-0.1.3.1.dist-info/WHEEL
--rwxrwxrwx  2.0 unx       86 b- defN 23-Apr-15 23:02 bandplot-0.1.3.1.dist-info/entry_points.txt
--rwxrwxrwx  2.0 unx        9 b- defN 23-Apr-15 23:02 bandplot-0.1.3.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      711 b- defN 23-Apr-15 23:02 bandplot-0.1.3.1.dist-info/RECORD
-9 files, 52512 bytes uncompressed, 8050 bytes compressed:  84.7%
+Zip file size: 9279 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx       26 b- defN 23-May-02 18:19 bandplot/__init__.py
+-rw-rw-r--  2.0 unx    27604 b- defN 23-May-02 18:19 bandplot/plots.py
+-rw-rw-r--  2.0 unx     5809 b- defN 23-May-02 18:19 bandplot/readdata.py
+-rw-rw-r--  2.0 unx    15274 b- defN 23-May-02 18:19 bandplot/wrapper.py
+-rw-rw-r--  2.0 unx     2901 b- defN 23-May-02 18:19 bandplot-0.1.3.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-02 18:19 bandplot-0.1.3.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       86 b- defN 23-May-02 18:19 bandplot-0.1.3.2.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        9 b- defN 23-May-02 18:19 bandplot-0.1.3.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      711 b- defN 23-May-02 18:19 bandplot-0.1.3.2.dist-info/RECORD
+9 files, 52512 bytes uncompressed, 8055 bytes compressed:  84.7%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: bandplot/readdata.py
 Comment: 
 
 Filename: bandplot/wrapper.py
 Comment: 
 
-Filename: bandplot-0.1.3.1.dist-info/METADATA
+Filename: bandplot-0.1.3.2.dist-info/METADATA
 Comment: 
 
-Filename: bandplot-0.1.3.1.dist-info/WHEEL
+Filename: bandplot-0.1.3.2.dist-info/WHEEL
 Comment: 
 
-Filename: bandplot-0.1.3.1.dist-info/entry_points.txt
+Filename: bandplot-0.1.3.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: bandplot-0.1.3.1.dist-info/top_level.txt
+Filename: bandplot-0.1.3.2.dist-info/top_level.txt
 Comment: 
 
-Filename: bandplot-0.1.3.1.dist-info/RECORD
+Filename: bandplot-0.1.3.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bandplot/__init__.py

```diff
@@ -1,3 +1,3 @@
 
-__version__ = "0.1.3.1"
+__version__ = "0.1.3.2"
```

## bandplot/wrapper.py

```diff
@@ -174,15 +174,15 @@
     parser.add_argument('-i', "--input",      type=str,             default="BAND.dat", help="plot figure from .dat file, default BAND.dat")
     parser.add_argument('-o', "--output",     type=str,             default="BAND.png", help="plot figure filename, default BAND.png")
     parser.add_argument('-l', "--labels",     type=str.upper,       nargs='+', default=[], help='labels for high-symmetry points, such as X S Y K M')
     parser.add_argument('-d', "--dos",        type=str,             help="plot Phonon DOS from .dat file")
     parser.add_argument('-x', "--horizontal", type=float,           nargs=2, help="Phonon density of states range")
     parser.add_argument('-n', "--exchange",   action='store_true',  help="exchange the x and y axes of Phonon DOS")
     parser.add_argument('-e', "--elements",   type=str,             nargs='+', default=[], help="PDOS labels")
-    parser.add_argument('-r', "--wratios",    type=float,           default=0.5, help='width ratio for DOS subplot, default 0.5')
+    parser.add_argument('-p', "--wratios",    type=float,           default=0.5, help='width ratio for DOS subplot, default 0.5')
     parser.add_argument('-z', "--fill",       action='store_true',  help='fill a shaded region between PDOS and axis')
     parser.add_argument('-f', "--font",       type=str,             default='STIXGeneral', help="font to use")
 
     args = parser.parse_args()
 
     labels = [re.sub("'|‘|’", '′', re.sub('"|“|”', '″', re.sub('^GA[A-Z]+$|^G$', 'Γ', i))) for i in args.labels]
     elements = [re.sub("'|‘|’", '′', re.sub('"|“|”', '″', i)) for i in args.elements]
```

## Comparing `bandplot-0.1.3.1.dist-info/METADATA` & `bandplot-0.1.3.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bandplot
-Version: 0.1.3.1
+Version: 0.1.3.2
 Summary: Band structure, DOS or phonon band structure plot from vaspkit or phonopy result.
 Home-page: https://github.com/lkccrr/bandplot
 Author: kan
 Author-email: luokan@hrbeu.edu.cn
 License: MIT
 Keywords: DFT VASP DOS band plot Phonon
 Platform: Unix
```

## Comparing `bandplot-0.1.3.1.dist-info/RECORD` & `bandplot-0.1.3.2.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-bandplot/__init__.py,sha256=no8qvZvMjtJ5okO4f624fs8-dW0NIACrU6SrSEX8gpo,26
+bandplot/__init__.py,sha256=RA5qSpUhadirp4I_SZgIfQERJtJssx2PSGw3t1fRUiY,26
 bandplot/plots.py,sha256=EEhITz9cZKxhfe9DOmoIWGOAyXrJqoz6_dk_utYaPyI,27604
 bandplot/readdata.py,sha256=perJzlojUpEHArzro_gM-oh1wMRuNyAOOC1z1cvORPE,5809
-bandplot/wrapper.py,sha256=UsF4iX_RchDrHMyQpAEi9mrFnUJgXayRDE-QlvXu2YE,15274
-bandplot-0.1.3.1.dist-info/METADATA,sha256=4u3UWBeGyiyij9UooBsJQr81BvrvvBwTyOWtIn5tPvY,2901
-bandplot-0.1.3.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-bandplot-0.1.3.1.dist-info/entry_points.txt,sha256=1iTM_knGcHWOG7xxwvloJo_nbjS8WKTPOHP_HIKQr7k,86
-bandplot-0.1.3.1.dist-info/top_level.txt,sha256=SMQlf9lMS_nlhnQduityQVcU231XkEEvM7Z0n9gB0JE,9
-bandplot-0.1.3.1.dist-info/RECORD,,
+bandplot/wrapper.py,sha256=keKK2jbbiandVI2hyhb2Gcp2-OJZ6qhtghEyRR53WHQ,15274
+bandplot-0.1.3.2.dist-info/METADATA,sha256=bENd7GJWrvICIHAj7gQSt-jlwKCCq78iwFQW9EucyeA,2901
+bandplot-0.1.3.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+bandplot-0.1.3.2.dist-info/entry_points.txt,sha256=1iTM_knGcHWOG7xxwvloJo_nbjS8WKTPOHP_HIKQr7k,86
+bandplot-0.1.3.2.dist-info/top_level.txt,sha256=SMQlf9lMS_nlhnQduityQVcU231XkEEvM7Z0n9gB0JE,9
+bandplot-0.1.3.2.dist-info/RECORD,,
```

