# Comparing `tmp/delayed_image-0.2.6-py3-none-any.whl.zip` & `tmp/delayed_image-0.2.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 70620 bytes, number of entries: 13
--rw-r--r--  2.0 unx    15467 b- defN 23-Mar-16 17:17 delayed_image/__init__.py
--rw-r--r--  2.0 unx    59717 b- defN 23-Mar-16 17:17 delayed_image/channel_spec.py
--rw-r--r--  2.0 unx    13066 b- defN 23-Mar-16 17:17 delayed_image/delayed_base.py
--rw-r--r--  2.0 unx    13590 b- defN 23-Mar-16 17:17 delayed_image/delayed_leafs.py
--rw-r--r--  2.0 unx    99022 b- defN 23-Mar-16 17:17 delayed_image/delayed_nodes.py
--rw-r--r--  2.0 unx      900 b- defN 23-Mar-16 17:17 delayed_image/demo.py
--rw-r--r--  2.0 unx    33248 b- defN 23-Mar-16 17:17 delayed_image/helpers.py
--rw-r--r--  2.0 unx    26144 b- defN 23-Mar-16 17:17 delayed_image/lazy_loaders.py
--rw-r--r--  2.0 unx    22206 b- defN 23-Mar-16 17:17 delayed_image/sensorchan_spec.py
--rw-r--r--  2.0 unx    26380 b- defN 23-Mar-16 17:17 delayed_image-0.2.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-16 17:17 delayed_image-0.2.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Mar-16 17:17 delayed_image-0.2.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1092 b- defN 23-Mar-16 17:17 delayed_image-0.2.6.dist-info/RECORD
-13 files, 310938 bytes uncompressed, 68808 bytes compressed:  77.9%
+Zip file size: 73023 bytes, number of entries: 13
+-rw-r--r--  2.0 unx    15467 b- defN 23-May-02 19:30 delayed_image/__init__.py
+-rw-r--r--  2.0 unx    61766 b- defN 23-May-02 19:30 delayed_image/channel_spec.py
+-rw-r--r--  2.0 unx    13085 b- defN 23-May-02 19:30 delayed_image/delayed_base.py
+-rw-r--r--  2.0 unx    13590 b- defN 23-May-02 19:30 delayed_image/delayed_leafs.py
+-rw-r--r--  2.0 unx    99022 b- defN 23-May-02 19:30 delayed_image/delayed_nodes.py
+-rw-r--r--  2.0 unx      900 b- defN 23-May-02 19:30 delayed_image/demo.py
+-rw-r--r--  2.0 unx    33248 b- defN 23-May-02 19:30 delayed_image/helpers.py
+-rw-r--r--  2.0 unx    26215 b- defN 23-May-02 19:30 delayed_image/lazy_loaders.py
+-rw-r--r--  2.0 unx    22747 b- defN 23-May-02 19:30 delayed_image/sensorchan_spec.py
+-rw-r--r--  2.0 unx    30203 b- defN 23-May-02 19:31 delayed_image-0.2.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-02 19:31 delayed_image-0.2.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-May-02 19:31 delayed_image-0.2.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1092 b- defN 23-May-02 19:31 delayed_image-0.2.7.dist-info/RECORD
+13 files, 317441 bytes uncompressed, 71211 bytes compressed:  77.6%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: delayed_image/lazy_loaders.py
 Comment: 
 
 Filename: delayed_image/sensorchan_spec.py
 Comment: 
 
-Filename: delayed_image-0.2.6.dist-info/METADATA
+Filename: delayed_image-0.2.7.dist-info/METADATA
 Comment: 
 
-Filename: delayed_image-0.2.6.dist-info/WHEEL
+Filename: delayed_image-0.2.7.dist-info/WHEEL
 Comment: 
 
-Filename: delayed_image-0.2.6.dist-info/top_level.txt
+Filename: delayed_image-0.2.7.dist-info/top_level.txt
 Comment: 
 
-Filename: delayed_image-0.2.6.dist-info/RECORD
+Filename: delayed_image-0.2.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## delayed_image/__init__.py

```diff
@@ -230,15 +230,15 @@
     >>> stack = kwimage.stack_images(tostack_rows, axis=0, bg_value=(5, 100, 10), pad=10)
     >>> kwplot.imshow(stack, title='notice how the "undone all" crops are shifted to the right' + chr(10) + 'such that they align with the original image')
     >>> kwplot.show_if_requested()
 
 """
 
 
-__version__ = '0.2.6'
+__version__ = '0.2.7'
 __author__ = 'Jon Crall'
 __author_email__ = 'jon.crall@kitware.com'
 
 
 __mkinit__ = """
 mkinit -m delayed_image
 """
```

## delayed_image/channel_spec.py

```diff
@@ -263,15 +263,15 @@
         """
         Addition operator is overloaded to late fusion
         """
         if other == 0:
             return self
         return other + self
 
-    def path_sanitize(self, maxlen=None):
+    def path_sanitize(self, maxlen=128):
         """
         Clean up the channel spec so it can be used in a pathname.
 
         Args:
             maxlen (int):
                 if specified, and the name is longer than this length, it is
                 shortened. Must be 8 or greater.
@@ -293,22 +293,15 @@
         Example:
             >>> import delayed_image
             >>> print(delayed_image.ChannelSpec.coerce('foo.0:3').normalize().path_sanitize(24))
             foo.0_foo.1_foo.2
             >>> print(delayed_image.ChannelSpec.coerce('foo.0:256').normalize().path_sanitize(24))
             tuuxtfnrsvdhezkdndysxo_256
         """
-        spec = self.spec
-        pname = spec.replace('|', '_').replace(':', '-')
-        if maxlen is not None and len(pname) > maxlen:
-            # prevent long names for docker (limit is 242 chars)
-            num_bands = self.numel()
-            hashlen = maxlen - 2
-            hashlen = max(8, hashlen)
-            pname = '{}_{}'.format(ub.hash_data(pname, base='abc')[0:hashlen], num_bands)
+        pname = _path_sanitize_v2(self.spec, maxlen=maxlen, hash_suffix=self.numel)
         return pname
 
 
 class FusedChannelSpec(BaseChannelSpec):
     """
     A specific type of channel spec with only one early fused stream.
 
@@ -699,16 +692,22 @@
     to_list = as_list
 
     def as_path(self):
         """
         Returns a string suitable for use in a path.
 
         Note, this may no longer be a valid channel spec
+
+        Example:
+            >>> from delayed_image.channel_spec import *  # NOQA
+            >>> self = FusedChannelSpec.coerce('b1|Z:3|b2|b3|rgb')
+            >>> self.as_path()
+            b1_Z..3_b2_b3_rgb
         """
-        return self.spec.replace('|', '_')
+        return self.path_sanitize()
 
     def __set__(self):
         return self.as_set()
 
     def difference(self, other):
         """
         Set difference
@@ -1100,16 +1099,22 @@
         return ub.peek(parsed.values())
 
     def as_path(self):
         """
         Returns a string suitable for use in a path.
 
         Note, this may no longer be a valid channel spec
+
+        Example:
+            >>> from delayed_image.channel_spec import *
+            >>> self = ChannelSpec('rgb|disparity,flowx|r|flowy')
+            >>> self.as_path()
+            rgb_disparity,flowx_r_flowy
         """
-        return self.spec.replace('|', '_')
+        return self.path_sanitize()
 
     def difference(self, other):
         """
         Set difference. Remove all instances of other channels from
         this set of channels.
 
         Example:
@@ -1696,14 +1701,68 @@
     if CHECK_ERRORS:
         if '.' in root or ':' in root:
             raise ValueError('invalid slice syntax: {}'.format(v))
 
     return root, start, stop, step
 
 
+def _path_sanitize_v2(path, maxlen=128, hash_suffix=None):
+    """
+    Clean input text so it can be used as a path.
+
+    Args:
+        path (str): the path name to santaize
+        maxlen (int | None):
+            if specified, and the name is longer than this length, it is
+            shortened. Must be 8 or greater.
+        hash_suffix (str | None | callable):
+            if specified, add an extra suffix to the name if it was hashed.
+            Can also be a callable.
+
+    Returns:
+        str: path suitable for usage in a filename
+
+    Example:
+        >>> from delayed_image.channel_spec import _path_sanitize_v2
+        >>> print(_path_sanitize_v2('a chan with space|bar|baz'))
+        a chan with space_bar_baz
+        >>> print(_path_sanitize_v2('dont|use<these>chars:in?a*path.'))
+        dont_use-LT-these-GT-chars..in_Q_a_S_path._
+        >>> print(_path_sanitize_v2('dont|use<these>chars:in?a*path.', maxlen=8))
+        iderkhwc
+    """
+    # https://stackoverflow.com/questions/1976007/what-characters-are-forbidden-in-windows-and-linux-directory-names
+    illegal_character_mapping = {
+        '|': '_',
+        '<': '-LT-',
+        '>': '-GT-',
+        ':': '..',
+        '?': '_Q_',
+        '*': '_S_',
+    }
+    new_name = path
+    for k, v in illegal_character_mapping.items():
+        new_name = new_name.replace(k, v)
+    if new_name.endswith(('.', ' ')):
+        # filenames cannot end with a dot or space.
+        new_name = new_name + '_'
+    if maxlen is not None and len(new_name) > maxlen:
+        # prevent long names for docker (limit is 242 chars)
+        hashlen = maxlen - 2
+        hashlen = max(8, hashlen)
+        hashstr = ub.hash_data(new_name, base='abc')[0:hashlen]
+        if hash_suffix is not None:
+            if callable(hash_suffix):
+                hash_suffix = hash_suffix()
+            new_name = '{}_{}'.format(hashstr, hash_suffix)
+        else:
+            new_name = hashstr
+    return new_name
+
+
 def oset_insert(self, index, obj):
     """
     Ignore:
         self = ub.oset()
         oset_insert(self, 0, 'a')
         oset_insert(self, 0, 'b')
         oset_insert(self, 0, 'c')
```

## delayed_image/delayed_base.py

```diff
@@ -119,15 +119,15 @@
         while stack:
             parent, item = stack.pop()
             yield parent, item
             for child in item.children():
                 stack.append((item, child))
 
     @profile
-    def _leafs(self):
+    def leafs(self):
         """
         Iterates over all leafs in the tree.
 
         Yields:
             Tuple[DelayedOperation] :
         """
         # Might be useful in _set_nested_params or other functions that
@@ -138,14 +138,16 @@
             children = list(item.children())
             if children:
                 for child in item.children():
                     stack.append(child)
             else:
                 yield item
 
+    _leafs = leafs
+
     @profile
     def _leaf_paths(self):
         """
         Builds all independent paths to leafs.
 
         Yields:
             Tuple[DelayedOperation, DelayedOperation]:
```

## delayed_image/lazy_loaders.py

```diff
@@ -353,15 +353,15 @@
     Example:
         >>> # See if we can reproduce the INTERLEAVE bug
 
         data = np.random.rand(128, 128, 64)
         import kwimage
         import ubelt as ub
         from os.path import join
-        dpath = ub.ensure_app_cache_dir('delayed_image/tests/reader')
+        dpath = ub.Path.appdir('delayed_image/tests/reader').ensuredir()
         fpath = join(dpath, 'foo.tiff')
         kwimage.imwrite(fpath, data, backend='skimage')
         recon1 = kwimage.imread(fpath)
         recon1.shape
 
         self = LazyGDalFrameFile(fpath)
         self.shape
@@ -431,15 +431,15 @@
 
     @classmethod
     def demo(cls, key='astro', dsize=None):
         """
         Ignore:
             >>> self = LazyGDalFrameFile.demo(dsize=(6600, 4400))
         """
-        cache_dpath = ub.ensure_app_cache_dir('delayed_image/demo')
+        cache_dpath = ub.Path.appdir('delayed_image/demo').ensuredir()
         fpath = join(cache_dpath, key + '.cog.tiff')
         depends = ub.odict(dsize=dsize)
         stamp = ub.CacheStamp(fname=key, depends=depends, dpath=cache_dpath,
                               product=[fpath])
         if stamp.expired():
             img = kwimage.grab_test_image(key, dsize=dsize)
             kwimage.imwrite(fpath, img, backend='gdal')
@@ -595,14 +595,16 @@
         ds = self._ds
         height, width, C = self.shape
 
         if 1:
             INTERLEAVE = ds.GetMetadata('IMAGE_STRUCTURE').get('INTERLEAVE', '')
             if INTERLEAVE == 'BAND':
                 if len(ds.GetSubDatasets()) > 0:
+                    import xdev
+                    xdev.embed()
                     raise NotImplementedError('Cannot handle interleaved files yet')
 
         if not ub.iterable(index):
             index = [index]
         else:
             index = list(index)
```

## delayed_image/sensorchan_spec.py

```diff
@@ -45,25 +45,25 @@
     // A channel code can just be an ID, or it can have a getitem
     // style syntax with a scalar or slice as an argument
     chan_code : chan_single | chan_getslice_0b | chan_getslice_ab | chan_getitem
 
     // Fused channels are an ordered sequence of channel codes (without sensors)
     fused : chan_code ("|" chan_code)*
 
-    // A channel only part can be a fused channel or a sequence
-    channel_rhs : fused | fused_seq
-
     // Channels can be specified in a sequence but must contain parens
     fused_seq : "(" fused ("," fused)* ")"
 
     // Sensors can be specified in a sequence but must contain parens
     sensor_seq : "(" IDEN ("," IDEN)* "):"
 
     sensor_lhs : (IDEN ":") | (sensor_seq)
 
+    // A channel only part can be a fused channel or a sequence
+    channel_rhs : fused | fused_seq
+
     sensor_chan : sensor_lhs channel_rhs?
 
     nosensor_chan : channel_rhs
 
     stream_item : sensor_chan | nosensor_chan
 
     // A stream is an unordered sequence of fused channels, that can
@@ -73,14 +73,41 @@
 
     %import common.DIGIT
     %import common.LETTER
     %import common.INT
     ''')
 
 
+"""
+TODO: add the concept of an exclusive or operator with left hand priority. The
+idea is that we can specify a code that will use the one fused channel spec if
+it is available, but if it is not, it will fall back to the next one. E.G.
+
+
+WV:((red|green|blue)^(pan))
+
+(L8,S2,WV,WV1):((red|green|blue)^(pan))
+
+
+Possible Production Rules:
+
+    fused : chan_code ("|" chan_code)*
+    fused_seq : "(" fused ("," fused)* ")"
+
+
+
+Maybe also include that on the sensor side?
+
+Use WV:r|g|b if we have it otherwise use S2:r|g|b
+
+(WV^S2)(r|g|b)
+
+"""
+
+
 class SensorSpec(ub.NiceRepr):
     """
     A simple wrapper for sensors in case we want to do anything fancy with them
     later. For now they are just a string.
     """
     def __init__(self, spec):
         self.spec = spec
```

## Comparing `delayed_image-0.2.6.dist-info/METADATA` & `delayed_image-0.2.7.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delayed-image
-Version: 0.2.6
+Version: 0.2.7
 Summary: The delayed_image module
 Author: Jon Crall
 Author-email: jon.crall@kitware.com
 License: Apache 2
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -33,26 +33,24 @@
 Provides-Extra: all
 Requires-Dist: kwarray ; extra == 'all'
 Requires-Dist: kwimage ; extra == 'all'
 Requires-Dist: ubelt ; extra == 'all'
 Requires-Dist: affine ; extra == 'all'
 Requires-Dist: xdoctest ; extra == 'all'
 Requires-Dist: pytest-timeout ; extra == 'all'
-Requires-Dist: codecov ; extra == 'all'
 Requires-Dist: lark-cython ; extra == 'all'
 Requires-Dist: lark ; extra == 'all'
 Requires-Dist: xarray ; extra == 'all'
 Provides-Extra: all-strict
 Requires-Dist: kwarray (==0.6.0) ; extra == 'all-strict'
 Requires-Dist: kwimage (==0.9.7) ; extra == 'all-strict'
 Requires-Dist: ubelt (==1.2.1) ; extra == 'all-strict'
 Requires-Dist: affine (==2.3.1) ; extra == 'all-strict'
 Requires-Dist: xdoctest (==0.14.0) ; extra == 'all-strict'
 Requires-Dist: pytest-timeout (==1.4.2) ; extra == 'all-strict'
-Requires-Dist: codecov (==2.0.15) ; extra == 'all-strict'
 Requires-Dist: lark-cython (==0.0.12) ; extra == 'all-strict'
 Requires-Dist: lark (==1.1.2) ; extra == 'all-strict'
 Requires-Dist: xarray (==0.16.0) ; extra == 'all-strict'
 Requires-Dist: coverage (==4.5) ; (python_version < "2.7" and python_version >= "2.6") and extra == 'all-strict'
 Requires-Dist: pytest (<=4.6.11,==4.6.0) ; (python_version < "2.8.0" and python_version >= "2.7.0") and extra == 'all-strict'
 Requires-Dist: pytest-cov (==2.8.1) ; (python_version < "2.8.0" and python_version >= "2.7.0") and extra == 'all-strict'
 Requires-Dist: numpy (==1.19.3) ; (python_version < "3.10" and python_version >= "3.9") and extra == 'all-strict'
@@ -165,19 +163,17 @@
 Requires-Dist: numpy (==1.19.2) ; (python_version < "3.8" and python_version >= "3.7") and extra == 'runtime-strict'
 Requires-Dist: numpy (==1.19.2) ; (python_version < "3.9" and python_version >= "3.8") and extra == 'runtime-strict'
 Requires-Dist: numpy (==1.23.2) ; (python_version >= "3.11") and extra == 'runtime-strict'
 Requires-Dist: networkx (==2.7) ; (python_version >= "3.8") and extra == 'runtime-strict'
 Provides-Extra: tests
 Requires-Dist: xdoctest ; extra == 'tests'
 Requires-Dist: pytest-timeout ; extra == 'tests'
-Requires-Dist: codecov ; extra == 'tests'
 Provides-Extra: tests-strict
 Requires-Dist: xdoctest (==0.14.0) ; extra == 'tests-strict'
 Requires-Dist: pytest-timeout (==1.4.2) ; extra == 'tests-strict'
-Requires-Dist: codecov (==2.0.15) ; extra == 'tests-strict'
 Requires-Dist: coverage (==4.5) ; (python_version < "2.7" and python_version >= "2.6") and extra == 'tests-strict'
 Requires-Dist: pytest (<=4.6.11,==4.6.0) ; (python_version < "2.8.0" and python_version >= "2.7.0") and extra == 'tests-strict'
 Requires-Dist: pytest-cov (==2.8.1) ; (python_version < "2.8.0" and python_version >= "2.7.0") and extra == 'tests-strict'
 Requires-Dist: coverage (==5.3.1) ; (python_version < "3.10" and python_version >= "3.9") and extra == 'tests-strict'
 Requires-Dist: pytest (==4.6.0) ; (python_version < "3.10.0" and python_version >= "3.7.0") and extra == 'tests-strict'
 Requires-Dist: coverage (==5.3.1) ; (python_version < "3.4" and python_version >= "2.7") and extra == 'tests-strict'
 Requires-Dist: coverage (==4.3.4) ; (python_version < "3.5" and python_version >= "3.4") and extra == 'tests-strict'
@@ -230,15 +226,15 @@
 it detects a scaling operation. This is **much** faster than the naive way of
 accomplishing these operations, and **much** easier than having to remember to
 do everything in the right order yourself.
 
 Note: GDAL is optional, but recommended. Precompiled GDAL wheels are available
 on Kitware's `large image wheel repository <https://girder.github.io/large_image_wheels/>`__.
 Use ``pip install gdal -f https://girder.github.io/large_image_wheels/`` 
-to install gdal from this server. Track status of official gdal wheels `here
+to install GDAL from this server. Track status of official GDAL wheels `here
 <https://github.com/OSGeo/gdal/issues/3060>`__.
 
 
 History
 -------
 
 This module is still in its early days of development and is a port the
@@ -338,21 +334,99 @@
     >>> kwplot.imshow(final0, pnum=(1, 2, 1), fnum=1, title='raw')
     >>> kwplot.imshow(final1, pnum=(1, 2, 2), fnum=1, title='optimized')
 
  
 .. image:: https://i.imgur.com/3SGvxtC.png
 
 
+Native Resolution Sampling
+--------------------------
+
+Consider the case where we have multiple images on disk in different
+resolutions, but they correspond to the same scene (e.g. a satellite image may
+have RGB bands at 10 meter resolution and an infrared band at 30 meter
+resolution), and we want to sample corresponding regions in each image.
+Typically a developer may opt to simply rescale everything to the same
+resolution, so everything corresponds and then just crop out the region.  This
+works but it has the negative effect of incurring resampling artifacts.
+
+Delayed image allows for easy and intuitive "native resolution sampling".  We
+can perform a delayed scale operation to get a "view" of an image as if we
+rescaled all component bands to the same resolution, and then perform a delayed
+crop. Finalizing this delayed operation is exactly the same as the previously
+described case (except that it benefits from delayed image's optimized
+operation reordering). However, we can go further. Because we know about the
+underlying operation graph we can undo the scale component while keeping the
+crop component, which results in loading the corresponding parts of the image
+inside the cropped area, but does not do any resampling. The images on disk can
+differ in more than just resolution, they could also be offset, skewed or
+rotated, and this unwarping procedure will still work. 
+
+The following image illustrates an extreme example of this were we simulate a
+low resolution red band (R), a medium but rotated resolution green band (G),
+and a high but cropped resolution blue (B) band.
+
+.. image:: https://i.imgur.com/fW7Mdo1.png
+
+
+The raw bands on disk are shown in the top row. The second row demonstrates the
+aligned space that we can conceptually think in when performing the crop. The
+blue box defined in this row and is projected to all other images using delayed
+image. The third row shows the result of the naive resampled alignment and
+cropping of the blue box (and also pixel differences between optimized and
+non-optimized finalizations). Lastly the fourth row shows the native sampling where
+each crop corresponds to the same region, but we have removed all scale factors
+(rotation and skew resamplings are still done to align to image corners up to a
+scale factor).
+
+For code details see the doctest in `delayed_image/__init__.py __doc__:2 <https://gitlab.kitware.com/computer-vision/delayed_image/-/blob/main/delayed_image/__init__.py#L115>`_
+
+
 SensorChanSpec
 --------------
 
 Includes the SensorChan spec, which makes handling channels from different
 sensing sources easier.
 
-It has a simple grammar:
+The sensor/channel spec isn't necessary to use delayed image, but it helps ---
+particularly the channel spec --- to be able to semantically label the channels
+when performing delayed load operations.
+
+On a simple level all you need to know to use the basic channel spec is that
+channel names are ``|`` delimited. E.g. ``red|green|blue`` refers to a 3
+channel image. You can use these names to select subsets of channels. Here is
+an example where you load an image, provide it with the semantic labels for
+each channel, and then use them to select a single channel.
+
+.. code:: python
+
+    import delayed_image
+    import kwimage
+    fpath = kwimage.grab_test_image_fpath(overviews=3)
+
+    # When you create a delayed image, you can enrich the image with
+    # information about what channels it contains by specifying the 
+    # channels attribute.
+    delayed = DelayedLoad(fpath, channels='red|green|blue').prepare()
+
+    # You can use this to semantically interact with the channels
+    delayed_g = delayed.take_channels('green')
+    assert delayed_g.shape == (512, 512, 1)
+
+    # Specifying more than one channel works too
+    delayed_rb = delayed.take_channels('blue|red')
+    assert delayed_rb.shape == (512, 512, 2)
+
+
+Much of the Sensor/Channel spec functionality exists for the benefit of other
+projects like `kwcoco <https://gitlab.kitware.com/computer-vision/kwcoco>`_.
+Admittedly, this library isn't the perfect home for the full sensor / channel
+spec, but this is where it currently lives.
+
+The full sensor channel spec has a formal grammar defined in this package.
 
  .. code:: 
 
     // SENSOR_CHAN_GRAMMAR
     ?start: stream
 
     // An identifier can contain spaces
```

## Comparing `delayed_image-0.2.6.dist-info/RECORD` & `delayed_image-0.2.7.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-delayed_image/__init__.py,sha256=UDFda6UVqCILtAs8aOl6q5fw2ZG9H_9zKXmdYlCxCY8,15467
-delayed_image/channel_spec.py,sha256=SXiT3QZwSY-nKPCGyPnoeYT9_FlDMImPI3H6QN7cAVs,59717
-delayed_image/delayed_base.py,sha256=vLI4ueIUN1bn8163J1twXlUDNLex6AXnbptkMyBTiCM,13066
+delayed_image/__init__.py,sha256=tPd_p21WTqRzQb9ZMC5_8Z75aq3WyniE63yRa5zza6Q,15467
+delayed_image/channel_spec.py,sha256=6E6iCwo8kLReeBN2Nb0kPH1bzlyHHzSDXTn-V2yc7Co,61766
+delayed_image/delayed_base.py,sha256=NxHKASG-nJT6YUt-FxpJNaMM7a3UIK1j4z2uN0KQDdg,13085
 delayed_image/delayed_leafs.py,sha256=TMFqGTNyEwurtC_9PAG812uTF_zCjnJi0JG0hNOSVqc,13590
 delayed_image/delayed_nodes.py,sha256=F48bc090WCuQ8UJCC2a4oLkrvziDWAau4C-6-MqxEPE,99022
 delayed_image/demo.py,sha256=jQqXRo6cN75vB_D32lnpUXIjCYYk-sKAXF1776GCfI4,900
 delayed_image/helpers.py,sha256=D0eiIo0Blyu0n4D5uiZ3mZP0ESuLnm-6exJV7iTpwzU,33248
-delayed_image/lazy_loaders.py,sha256=oP4oxX4KNDrfAY4vyQiYfBpOcX0sT-TcSBBYZXMJBcw,26144
-delayed_image/sensorchan_spec.py,sha256=LxEpi_6fGjYEAsJLxvV-YcPmxSWt2laLlOFAX7Ji2nU,22206
-delayed_image-0.2.6.dist-info/METADATA,sha256=b94s03786q1euSmmG06ANoEsupXauRwpjkzNfSkjMuo,26380
-delayed_image-0.2.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-delayed_image-0.2.6.dist-info/top_level.txt,sha256=2I0BoRDZ6Gfbdps7YCquLhxb4hLEOuYKZN7L7Rh_jmk,14
-delayed_image-0.2.6.dist-info/RECORD,,
+delayed_image/lazy_loaders.py,sha256=2y6daP6WQikcHYc8JiXqXX7A62acuTd2mKpRz7OlPl8,26215
+delayed_image/sensorchan_spec.py,sha256=Zm0uMxnoFBOswAARF5e4-bSYPakIpfwN_LoduBq-tPU,22747
+delayed_image-0.2.7.dist-info/METADATA,sha256=q3EJ1yiDreRFJVL9I5cW2h70HGIW1dHOmur2v81n-ZY,30203
+delayed_image-0.2.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+delayed_image-0.2.7.dist-info/top_level.txt,sha256=2I0BoRDZ6Gfbdps7YCquLhxb4hLEOuYKZN7L7Rh_jmk,14
+delayed_image-0.2.7.dist-info/RECORD,,
```

