# Comparing `tmp/pore-c-py-2.0.3.tar.gz` & `tmp/pore-c-py-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pore-c-py-2.0.3.tar", last modified: Wed Apr  5 14:16:42 2023, max compression
+gzip compressed data, was "pore-c-py-2.0.4.tar", last modified: Tue May  2 16:24:31 2023, max compression
```

## Comparing `pore-c-py-2.0.3.tar` & `pore-c-py-2.0.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 14:16:42.727204 pore-c-py-2.0.3/
--rw-rw-rw-   0 root         (0) root         (0)    15820 2023-04-05 14:14:31.000000 pore-c-py-2.0.3/LICENSE.md
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-04-05 14:14:31.000000 pore-c-py-2.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1157 2023-04-05 14:16:42.723204 pore-c-py-2.0.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      895 2023-04-05 14:14:31.000000 pore-c-py-2.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 14:16:42.723204 pore-c-py-2.0.3/pore_c_py/
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-04-05 14:14:31.000000 pore-c-py-2.0.3/pore_c_py/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6323 2023-04-05 14:14:31.000000 pore-c-py-2.0.3/pore_c_py/align_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     2748 2023-04-05 14:14:31.000000 pore-c-py-2.0.3/pore_c_py/annotate.py
--rw-rw-rw-   0 root         (0) root         (0)     4907 2023-04-05 14:14:31.000000 pore-c-py-2.0.3/pore_c_py/digest.py
--rw-rw-rw-   0 root         (0) root         (0)    15382 2023-04-05 14:14:31.000000 pore-c-py-2.0.3/pore_c_py/main.py
--rw-rw-rw-   0 root         (0) root         (0)     3739 2023-04-05 14:14:31.000000 pore-c-py-2.0.3/pore_c_py/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     4087 2023-04-05 14:14:31.000000 pore-c-py-2.0.3/pore_c_py/writers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 14:16:42.723204 pore-c-py-2.0.3/pore_c_py.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1157 2023-04-05 14:16:42.000000 pore-c-py-2.0.3/pore_c_py.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      549 2023-04-05 14:16:42.000000 pore-c-py-2.0.3/pore_c_py.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-05 14:16:42.000000 pore-c-py-2.0.3/pore_c_py.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       54 2023-04-05 14:16:42.000000 pore-c-py-2.0.3/pore_c_py.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-05 14:16:27.000000 pore-c-py-2.0.3/pore_c_py.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       46 2023-04-05 14:16:42.000000 pore-c-py-2.0.3/pore_c_py.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-05 14:16:42.000000 pore-c-py-2.0.3/pore_c_py.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       93 2023-04-05 14:14:31.000000 pore-c-py-2.0.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-05 14:16:42.727204 pore-c-py-2.0.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1930 2023-04-05 14:14:31.000000 pore-c-py-2.0.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 14:16:42.723204 pore-c-py-2.0.3/tests/
--rw-rw-rw-   0 root         (0) root         (0)     8939 2023-04-05 14:14:31.000000 pore-c-py-2.0.3/tests/test_align_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     6972 2023-04-05 14:14:31.000000 pore-c-py-2.0.3/tests/test_annotate.py
--rw-rw-rw-   0 root         (0) root         (0)      561 2023-04-05 14:14:31.000000 pore-c-py-2.0.3/tests/test_digest.py
--rw-rw-rw-   0 root         (0) root         (0)      946 2023-04-05 14:14:31.000000 pore-c-py-2.0.3/tests/test_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2786 2023-04-05 14:14:31.000000 pore-c-py-2.0.3/tests/test_writers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 16:24:31.830572 pore-c-py-2.0.4/
+-rw-rw-rw-   0 root         (0) root         (0)    15820 2023-05-02 16:20:43.000000 pore-c-py-2.0.4/LICENSE.md
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-05-02 16:20:43.000000 pore-c-py-2.0.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1157 2023-05-02 16:24:31.830572 pore-c-py-2.0.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      895 2023-05-02 16:20:43.000000 pore-c-py-2.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 16:24:31.826572 pore-c-py-2.0.4/pore_c_py/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-05-02 16:20:43.000000 pore-c-py-2.0.4/pore_c_py/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6413 2023-05-02 16:20:43.000000 pore-c-py-2.0.4/pore_c_py/align_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     2748 2023-05-02 16:20:43.000000 pore-c-py-2.0.4/pore_c_py/annotate.py
+-rw-rw-rw-   0 root         (0) root         (0)     5759 2023-05-02 16:20:43.000000 pore-c-py-2.0.4/pore_c_py/digest.py
+-rw-rw-rw-   0 root         (0) root         (0)    15382 2023-05-02 16:20:43.000000 pore-c-py-2.0.4/pore_c_py/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     3739 2023-05-02 16:20:43.000000 pore-c-py-2.0.4/pore_c_py/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4087 2023-05-02 16:20:43.000000 pore-c-py-2.0.4/pore_c_py/writers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 16:24:31.826572 pore-c-py-2.0.4/pore_c_py.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1157 2023-05-02 16:24:31.000000 pore-c-py-2.0.4/pore_c_py.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      549 2023-05-02 16:24:31.000000 pore-c-py-2.0.4/pore_c_py.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 16:24:31.000000 pore-c-py-2.0.4/pore_c_py.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       54 2023-05-02 16:24:31.000000 pore-c-py-2.0.4/pore_c_py.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 16:24:16.000000 pore-c-py-2.0.4/pore_c_py.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       46 2023-05-02 16:24:31.000000 pore-c-py-2.0.4/pore_c_py.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-02 16:24:31.000000 pore-c-py-2.0.4/pore_c_py.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       93 2023-05-02 16:20:43.000000 pore-c-py-2.0.4/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-02 16:24:31.830572 pore-c-py-2.0.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1930 2023-05-02 16:20:43.000000 pore-c-py-2.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 16:24:31.830572 pore-c-py-2.0.4/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     9082 2023-05-02 16:20:43.000000 pore-c-py-2.0.4/tests/test_align_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     6972 2023-05-02 16:20:43.000000 pore-c-py-2.0.4/tests/test_annotate.py
+-rw-rw-rw-   0 root         (0) root         (0)     4646 2023-05-02 16:20:43.000000 pore-c-py-2.0.4/tests/test_digest.py
+-rw-rw-rw-   0 root         (0) root         (0)      946 2023-05-02 16:20:43.000000 pore-c-py-2.0.4/tests/test_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2786 2023-05-02 16:20:43.000000 pore-c-py-2.0.4/tests/test_writers.py
```

### Comparing `pore-c-py-2.0.3/LICENSE.md` & `pore-c-py-2.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pore-c-py-2.0.3/PKG-INFO` & `pore-c-py-2.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pore-c-py
-Version: 2.0.3
+Version: 2.0.4
 Summary: Analyse Pore-C data.
 Home-page: https://github.com/epi2me-labs/pore-c-py
 Author: epi2melabs
 Author-email: epi2melabs@nanoporetech.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `pore-c-py-2.0.3/README.md` & `pore-c-py-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pore-c-py-2.0.3/pore_c_py/align_tools.py` & `pore-c-py-2.0.4/pore_c_py/align_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,16 +159,18 @@
     distance = genomic_distance(align1, align2)
     return distance <= tol
 
 
 def group_colinear(
         aligns: List[pysam.AlignedSegment], tol=0):
     """Group alignments into co-linear blocks."""
-    if len(aligns) < 2:
-        return [list(range(len(aligns)))]
+    if len(aligns) == 0:
+        return []  # an empty list of blocks
+    elif len(aligns) == 1:
+        return [aligns]  # one block with single alignment
     res = []
     block = []
     last = aligns[0]
     block = [last]
     for aln in aligns[1:]:
         if is_colinear(last, aln, tol=tol):
             block.append(aln)
```

### Comparing `pore-c-py-2.0.3/pore_c_py/annotate.py` & `pore-c-py-2.0.4/pore_c_py/annotate.py`

 * *Files identical despite different names*

### Comparing `pore-c-py-2.0.3/pore_c_py/digest.py` & `pore-c-py-2.0.4/pore_c_py/digest.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,69 +2,68 @@
 import copy
 
 from Bio import Restriction
 from Bio.Seq import Seq
 
 from pore_c_py import utils
 
+
 logger = utils.get_named_logger("Digest")
 
 
-def get_subread(align, start, end):
-    """Get sub read."""
+def get_subread_modified_bases(align, start, end):
+    """Get modified bases subread.
+
+    :param align: pysam.AlignedSegment.
+    :param start: start coordinate to trim to.
+    :param end: exclusive end co-ordinate.
+    """
+    mm_str, ml_str = "", ""
+    base_indices = {}
     seq = align.query_sequence[start:end]
-    if align.query_qualities:
-        qual = align.query_qualities[start:end]
-    else:
-        qual = None
-    if align.modified_bases:
-        mm_str, ml_str = "", ""
-        base_indices = {}
-        for mod_key, mod_data in align.modified_bases.items():
-            # find the modifications that overlap the subread
-            idx = [
-                x for x in range(len(mod_data)) if
-                start <= mod_data[x][0] < end]
-            if not idx:  # no mods in this subread
-                continue
-            try:
-                canonical_base, strand, skip_scheme, mod_type = mod_key
-            except ValueError:
-                canonical_base, strand, mod_type = mod_key
-                skip_scheme = ""
-
-            canonical_base = mod_key[0]
-            # find the positions of that canonical base in the subread
-            if canonical_base not in base_indices:
-                base_indices[canonical_base] = [
-                    x for x, b in enumerate(seq) if b.upper() == canonical_base
-                ]
-
-            base_offsets, probs = zip(*[mod_data[_] for _ in idx])
-            deltas = []
-            counter = 0
-            for seq_idx in base_indices[canonical_base]:
-                orig_idx = seq_idx + start
-                if orig_idx in base_offsets:  # is modified
-                    deltas.append(str(counter))
-                    counter = 0
-                else:
-                    counter += 1
-            assert len(deltas) == len(probs)
+    for mod_key, mod_data in align.modified_bases.items():
+        # find the modifications that overlap the subread
+        idx = [
+            x for x in range(len(mod_data)) if
+            start <= mod_data[x][0] < end]
+        probs_dic = dict(mod_data)
+        if not idx:  # no mod bases (of this type) in the subread
+            continue
+        try:
+            canonical_base, strand, skip_scheme, mod_type = mod_key
+        except ValueError:
+            canonical_base, strand, mod_type = mod_key
+            skip_scheme = ""
+        if canonical_base == "N":
+            base_indices[canonical_base] = list(range(len(seq)))
+        elif canonical_base not in base_indices:
+            base_indices[canonical_base] = [
+                x for x, b in enumerate(seq) if b.upper() == canonical_base
+            ]
+        base_offsets, probs = zip(*[mod_data[i] for i in idx])
+        strand = "+" if strand == 0 else "-"
+        deltas = []
+        counter = 0
+        probs = []
+        for seq_idx in base_indices[canonical_base]:
+            orig_idx = seq_idx + start
+            if orig_idx in base_offsets:  # is modified
+                probs += [probs_dic[orig_idx]]
+                deltas.append(str(counter))
+                counter = 0
+            else:
+                counter += 1
+            deltas_formatted = ','.join(deltas)
             prob_str = ",".join(map(str, probs))
-            strand = "+" if strand == 0 else "-"
-            mm_str += (
+        mm_str += (
                 f"{canonical_base}{strand}{mod_type}{skip_scheme}"
-                f",{','.join(deltas)};"
+                f",{deltas_formatted};"
             )
-            ml_str += f"{canonical_base},{prob_str};"
-    else:
-        mm_str, ml_str = None, None
-
-    return seq, qual, mm_str, ml_str
+        ml_str += f"{prob_str},"
+    return mm_str, ml_str
 
 
 def splits_to_intervals(positions, length):
     """Split to intervals."""
     if len(positions) == 0:
         return [(0, length)]
     prefix, suffix = [], []
@@ -84,53 +83,81 @@
     if enz.cut_twice():
         raise NotImplementedError(
             f"Enzyme cuts twice, not currently supported: {enzyme}"
         )
     return enz
 
 
-def get_concatemer_seqs(input_file, enzyme, remove_tags):
+def digest_sequence(align, enzyme, tags_remove=None):
+    """Digest sequence."""
+    # the move tag massively bloats files, and we don't care for
+    # it or handle it in trimming, so force its removal by default.
+    if tags_remove is None:
+        tags_remove = {'mv'}
+
+    concatemer_id = align.query_name
+    cut_points = [x - 1 for x in enzyme.search(Seq(align.query_sequence))]
+    read_length = len(align.query_sequence)
+    num_digits = len(str(read_length))
+    intervals = splits_to_intervals(cut_points, read_length)
+    num_intervals = len(intervals)
+
+    for idx, (start, end) in enumerate(intervals):
+        read = copy.copy(align)
+        # trim the sequence and quality
+        seq = align.query_sequence[start:end]
+        qual = None
+        if align.query_qualities:
+            qual = align.query_qualities[start:end]
+        read.query_sequence = seq
+        read.query_qualities = qual
+        # deal with mods, upgrading tag from interim to approved spec
+        if ('Mm' in tags_remove) or ('MM' in tags_remove):
+            # Setting to None effectively deletes,
+            # or does nothing if not present
+            for tag in ('Mm', 'Ml', 'MM', 'ML'):
+                read.set_tag(tag, None)
+        else:
+            mm, ml = get_subread_modified_bases(align, start, end)
+            for tag in ('Mm', 'Ml'):
+                read.set_tag(tag, None)
+            read.set_tag("MM", mm)
+            read.set_tag("ML", ml)
+        # lexograpically sortable monomer ID
+        read.query_name = \
+            f"{concatemer_id}:{start:0{num_digits}d}:{end:0{num_digits}d}"
+        read.set_tag(
+            utils.MONOMER_DATA_TAG,
+            [start, end, read_length, idx, num_intervals])
+        utils.MonomerData.set_monomer_data(
+                read, start, end, read_length, idx, num_intervals)
+        read.set_tag(utils.CONCATEMER_ID_TAG, concatemer_id, "Z")
+        yield read
+
+
+def get_concatemer_seqs(input_file, enzyme, remove_tags=None):
     """Digest concatemers in to unaligned monomers.
 
-    :param input_file: The input BAM or Fastq file.
+    :param input_file: pysam.AlignmentFile input
     :param enzyme: Name of the digestion enzyme used in sample preperation
     :param remove_tags: Comma seperated list of additional
                         tags to remove from file
 
     Concatemers are split with chosen digestion enzyme in to monomers.
     Monomers are tagged with unique monomer id and concatemer info.
     """
     logger.info(f"Digesting unaligned sequences from {input_file}")
     n_concatemers = 0
     n_monomers = 0
     enzyme = get_enzyme(enzyme)
-    tags_remove = {"Ml", "ML", "Mm", "MM", "mv"}
+    tags_remove = {"mv"}
     if remove_tags:
         tags_remove.update(set(remove_tags))
     for align in input_file.fetch(until_eof=True):
         n_concatemers += 1
-        concatemer_id = align.query_name
-        cut_points = [x - 1 for x in enzyme.search(Seq(align.query_sequence))]
-        read_length = len(align.query_sequence)
-        num_digits = len(str(read_length))
-        intervals = splits_to_intervals(cut_points, read_length)
-        num_intervals = len(intervals)
-        for idx, (start, end) in enumerate(intervals):
+        reads = digest_sequence(
+            align, enzyme, tags_remove)
+        for read in reads:
             n_monomers += 1
-            read = copy.copy(align)
-            seq, qual, mm_str, ml_str = get_subread(
-                align=align, start=start, end=end)
-            for item in tags_remove:
-                read.set_tag(item, None)
-            read.query_sequence = seq
-            read.query_qualities = qual
-            # lexograpically sortable monomer ID
-            read.query_name = \
-                f"{concatemer_id}:{start:0{num_digits}d}:{end:0{num_digits}d}"
-            utils.MonomerData.set_monomer_data(
-                read, start, end, read_length, idx, num_intervals)
-            read.set_tag(utils.CONCATEMER_ID_TAG, concatemer_id, "Z")
-            read.set_tag("MM", mm_str)
-            read.set_tag("ML", ml_str)
             yield read
-
-    logger.info(f"Found {n_monomers} monomers in {n_concatemers} concatemers.")
+    logger.info(
+        f"Found {n_monomers} monomers in {n_concatemers} concatemers.")
```

### Comparing `pore-c-py-2.0.3/pore_c_py/main.py` & `pore-c-py-2.0.4/pore_c_py/main.py`

 * *Files identical despite different names*

### Comparing `pore-c-py-2.0.3/pore_c_py/utils.py` & `pore-c-py-2.0.4/pore_c_py/utils.py`

 * *Files identical despite different names*

### Comparing `pore-c-py-2.0.3/pore_c_py/writers.py` & `pore-c-py-2.0.4/pore_c_py/writers.py`

 * *Files identical despite different names*

### Comparing `pore-c-py-2.0.3/pore_c_py.egg-info/PKG-INFO` & `pore-c-py-2.0.4/pore_c_py.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pore-c-py
-Version: 2.0.3
+Version: 2.0.4
 Summary: Analyse Pore-C data.
 Home-page: https://github.com/epi2me-labs/pore-c-py
 Author: epi2melabs
 Author-email: epi2melabs@nanoporetech.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `pore-c-py-2.0.3/pore_c_py.egg-info/SOURCES.txt` & `pore-c-py-2.0.4/pore_c_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pore-c-py-2.0.3/setup.py` & `pore-c-py-2.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `pore-c-py-2.0.3/tests/test_align_tools.py` & `pore-c-py-2.0.4/tests/test_align_tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Tests to align_tools."""
 import pysam
 import pytest
 
 from pore_c_py import align_tools
 
-HEADER = pysam.AlignmentHeader.from_references(
-    ["chr1", "chr2"], [1000, 2000])
 
+HEADER = pysam.AlignmentHeader.from_references(
+    ["chr1", "chr2", "*"], [1000, 2000, 3000])
 
 def align_from_tuple(t):
     """Align from tuple."""
     rec = pysam.AlignedSegment(header=HEADER)
-    rec.reference_id = ["chr1", "chr2"].index(t[0])
+    rec.reference_id = ["chr1", "chr2", "*"].index(t[0])
     rec.reference_start = t[1]
     rec.query_sequence = "A" * (t[2] - t[1])
     rec.cigartuples = [(pysam.CMATCH, (t[2] - t[1]))]
     rec.flag = 0
     if t[3] == "-":
         rec.flag |= pysam.FREVERSE
     if t[3] == ".":
@@ -58,14 +58,22 @@
         [
             [("chr1", 0, 8, "+"), ("chr1", 8, 9, "."), ("chr1", 20, 30, "+")],
             [[0], [1], [2]],
         ],
         [
             [("chr1", 0, 8, "+"), ("chr1", 8, 9, ".")],
             [[0], [1]],
+        ],
+        [
+            [("chr1", 0, 8, "+")],
+            [[0]],
+        ],
+        [
+            [],
+            []
         ]
     ],
 )
 def test_group_colinear(aligns, expected):
     """Test group colinear."""
     alns = [align_from_tuple(t) for t in aligns]
     exp = list()
```

### Comparing `pore-c-py-2.0.3/tests/test_annotate.py` & `pore-c-py-2.0.4/tests/test_annotate.py`

 * *Files identical despite different names*

### Comparing `pore-c-py-2.0.3/tests/test_utils.py` & `pore-c-py-2.0.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pore-c-py-2.0.3/tests/test_writers.py` & `pore-c-py-2.0.4/tests/test_writers.py`

 * *Files identical despite different names*

