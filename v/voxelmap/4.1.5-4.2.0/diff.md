# Comparing `tmp/voxelmap-4.1.5.tar.gz` & `tmp/voxelmap-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voxelmap-4.1.5.tar", max compression
+gzip compressed data, was "voxelmap-4.2.0.tar", max compression
```

## Comparing `voxelmap-4.1.5.tar` & `voxelmap-4.2.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1073 2023-01-14 04:48:56.741276 voxelmap-4.1.5/LICENSE
--rw-r--r--   0        0        0     1762 2023-03-28 06:03:09.266535 voxelmap-4.1.5/README.md
--rw-r--r--   0        0        0      590 2023-05-01 19:59:24.554165 voxelmap-4.1.5/pyproject.toml
--rw-r--r--   0        0        0       59 2023-04-02 23:36:39.545755 voxelmap-4.1.5/voxelmap/__init__.py
--rw-r--r--   0        0        0    21518 2023-05-01 01:42:22.585166 voxelmap-4.1.5/voxelmap/annex.py
--rwxr-xr-x   0        0        0    28849 2023-05-01 01:44:24.008146 voxelmap-4.1.5/voxelmap/jotunn.py
--rw-r--r--   0        0        0     2746 1970-01-01 00:00:00.000000 voxelmap-4.1.5/setup.py
--rw-r--r--   0        0        0     2800 1970-01-01 00:00:00.000000 voxelmap-4.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-01-14 04:48:56.741276 voxelmap-4.2.0/LICENSE
+-rw-r--r--   0        0        0     1762 2023-03-28 06:03:09.266535 voxelmap-4.2.0/README.md
+-rw-r--r--   0        0        0      590 2023-05-01 23:49:48.096334 voxelmap-4.2.0/pyproject.toml
+-rw-r--r--   0        0        0       87 2023-05-01 21:53:23.971994 voxelmap-4.2.0/voxelmap/__init__.py
+-rw-r--r--   0        0        0    18090 2023-05-01 23:31:17.709032 voxelmap-4.2.0/voxelmap/annex.py
+-rw-r--r--   0        0        0     3469 2023-05-01 22:00:09.289822 voxelmap-4.2.0/voxelmap/legacy.py
+-rwxr-xr-x   0        0        0    29202 2023-05-01 23:31:20.000989 voxelmap-4.2.0/voxelmap/main.py
+-rw-r--r--   0        0        0     2746 1970-01-01 00:00:00.000000 voxelmap-4.2.0/setup.py
+-rw-r--r--   0        0        0     2800 1970-01-01 00:00:00.000000 voxelmap-4.2.0/PKG-INFO
```

### Comparing `voxelmap-4.1.5/LICENSE` & `voxelmap-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `voxelmap-4.1.5/README.md` & `voxelmap-4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `voxelmap-4.1.5/pyproject.toml` & `voxelmap-4.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "voxelmap"
-version = "4.1.5"
+version = "4.2.0"
 description = "A Python library for making voxel and 3D models from NumPy arrays."
 authors = ["andrewrgarcia <garcia.gtr@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
```

### Comparing `voxelmap-4.1.5/voxelmap/annex.py` & `voxelmap-4.2.0/voxelmap/annex.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 
 def findclosest(array, value): 
     'adapted from: https://www.geeksforgeeks.org/python-find-closest-number-to-k-in-given-list/'      
     idx = (np.abs(array - value)).argmin()
     return idx
 
 
-
 def set_axes_radius(ax, origin, radius):
     '''set_axes_radius and set_axes_equal * * * Credit:
     Mateen Ulhaq (answered Jun 3 '18 at 7:55)
     https://stackoverflow.com/questions/13685386/matplotlib-equal-unit-length-with-equal-aspect-ratio-z-axis-is-not-equal-to'''
     ax.set_xlim3d([origin[0] - radius, origin[0] + radius])
     ax.set_ylim3d([origin[1] - radius, origin[1] + radius])
     ax.set_zlim3d([origin[2] - radius, origin[2] + radius])
@@ -58,21 +57,40 @@
         ax.get_zlim3d(),
     ])
 
     origin = np.mean(limits, axis=1)
     radius = 0.5 * np.max(np.abs(limits[:, 1] - limits[:, 0]))
     set_axes_radius(ax, origin, radius)
 
-def arr2crds(array,mult):
+def matrix_toXY(array,mult):
+    """
+    Converts a 2D numpy array into an XYv coordinate matrix where v is the corresponding element in every x-y coordinate.
+
+    Parameters
+    ----------
+    array : np.array(int,int)
+        The 2D numpy array to be converted to an XYv coordinate matrix.
+    mult : int or float
+        The multiplication factor to be applied to the elements in the matrix.
+    """
+
     Z  = np.max(array)
-    # return np.array([ [*i,Z-array[tuple(i)]] for i in np.argwhere(array)])
-    return np.array([ [*i,-mult*array[tuple(i)]] for i in np.argwhere(array)])
+    return np.array([ [*i,mult*array[tuple(i)]] for i in np.argwhere(array)])
 
-def tensor2crds(tensor,mult):
-    # return np.array([ [*i,Z-array[tuple(i)]] for i in np.argwhere(array)])
+def tensor_toXYZ(tensor,mult):
+    """
+    Converts a 3D numpy array (tensor) into an XYZ coordinate matrix.
+
+    Parameters
+    ----------
+    tensor : np.array(int,int,int)
+        The 3D array (tensor) to be converted to XYZ coordinates.
+    mult : int or float
+        The multiplication factor to be applied to all the coordinates.
+    """
     return np.array([ [*i*mult] for i in np.argwhere(tensor)])
 
 
 def resize_array(array, mult=(2,2,2)):
     '''Resizes a three-dimensional array by the three dim factors specified by `mult` tuple. 
     Converts to sparse array of 0s and 1s   
 
@@ -145,16 +163,14 @@
     kernel_level: int
         length scale (size) of random kernels used. The smallest scale (=1) gives the roughest transformation.
     '''
     kernel = np.zeros((kernel_level,kernel_level,kernel_level))
     return random_kernel_convolve(array,kernel,(-1,2))
 
 
-
-
 def load_array(filename):
     '''Loads a pickled numpy array with `filename` name'''
     return pickle.load( open(filename, "rb" ),encoding='latin1')
 
 def save_array(array,filename):
     '''Saves an `array` array with `filename` name using the pickle module'''
     return pickle.dump(array,open(filename,'wb'))
@@ -299,102 +315,16 @@
                     j2,(rand_t0+1)%4+1,j2,\
                     j3,(rand_t0+2)%4+1,j3 
                     ]
 
             f.write("f {}/{}/{} {}/{}/{} {}/{}/{}\n".format(*facestr))
 
 
-def voxelwrite(array, filename = 'voxelmodel.obj'):
-    '''
-    Writes a 3-D voxel model from the provided, third-order (3-D) `array` as an .obj file
-    
-    Parameters
-    ----------
-    array : np.array(int)
-            array of the third-order populated with discrete, non-zero integers which may represent a voxel block type
-    filename : str
-            name of .obj file to save model as. 
-    '''
-
-
-    # vertices diff (diffvs) for cube writing
-    diffvs = np.array([
-        [-0.50, -0.50, 0.00],
-        [-0.50, 0.50, 0.00],
-        [0.50, 0.50, 0.00],
-        [0.50 ,-0.50, 0.00],
-        [-0.50 ,-0.50 ,1.00],
-        [ 0.50, -0.50, 1.00],
-        [0.50, 0.50, 1.00],
-        [-0.50 ,0.50 ,1.00]])
-    
-
-
-    with open(filename, 'w') as f:
-        for coords in np.argwhere(array!=0):
-
-            # z,y,x = coords
-            for dverts in diffvs:
-                # dz,dy,dx = verts
-                
-                posits = (dverts + coords)
-            
-                f.write("v  {:.4f} {:.4f} {:.4f}\n".format(*posits))
-
-
-        block = """
-vt 1.00 0.00 0.00 
-vt 1.00 1.00 0.00
-vt 0.00 1.00 0.00
-vt 0.00 0.00 0.00
-
-vn 0.00 0.00 -1.00
-vn 0.00 0.00 1.00
-vn 0.00 -1.00 0.00
-vn 1.00 0.00 0.00
-vn 0.00 1.00 0.00
-vn -1.00 0.00 0.00
-
-\n"""
-
-
-       
-        f.write("\n"+block)
-
-        f.write("\ng Polyhedral\n\n")
-
-        v_idcs_text = list('123 341 567 785 146 651 437 764 328 873 215 582')
-        v_idcs = np.array([int(i) for i in v_idcs_text if i != ' '])
-
-        for i in range(len(np.argwhere(array!=0))):
-
-            f.write("""
-f {}/1/1 {}/2/1 {}/3/1
-f {}/3/1 {}/4/1 {}/1/1
-f {}/4/2 {}/1/2 {}/2/2
-f {}/2/2 {}/3/2 {}/4/2
-f {}/4/3 {}/1/3 {}/2/3
-f {}/2/3 {}/3/3 {}/4/3
-f {}/4/4 {}/1/4 {}/2/4
-f {}/2/4 {}/3/4 {}/4/4
-f {}/4/5 {}/1/5 {}/2/5
-f {}/2/5 {}/3/5 {}/4/5
-f {}/4/6 {}/1/6 {}/2/6
-f {}/2/6 {}/3/6 {}/4/6
-""".format(*(v_idcs+i+(i*7))))
-            
-            # 0 -> 1
-            # 1 -> 9 
-            # 2 -> 17
-
-
-
 
-
-def MarchingMesh(array, out_file='model.obj', level=0, spacing=(1., 1., 1.), gradient_direction='descent', step_size=1, allow_degenerate=True, method='lewiner', mask=None, plot=False, figsize=(4.8,4.8) ):
+def MarchingMesh(array, out_file='scene.obj', level=0, spacing=(1., 1., 1.), gradient_direction='descent', step_size=1, allow_degenerate=True, method='lewiner', mask=None, plot=False, figsize=(4.8,4.8) ):
     '''
     Marching cubes on sparse 3-D integer `voxelmap` arrays (GLOBAL)
 
     Parameters
     -------------
     array: np.array((int/float,int/float,int/float))
         3-D array for which to run the marching cubes algorithm   
@@ -429,36 +359,18 @@
 
     'write wavefront .obj file for generated mesh'
     writeobj_MC(out_file, verts, faces, normals, values)
 
     # Display resulting triangular mesh using Matplotlib. This can also be done
     # with mayavi (see skimage.measure.marching_cubes_lewiner docstring).
     if plot:
-        # fig = plt.figure(figsize=figsize)
-        # ax = fig.add_subplot(111, projection='3d')
-
-        # # Fancy indexing: `verts[faces]` to generate a collection of triangles
-        # print(verts[faces-1])
-        # mesh = Poly3DCollection(verts[faces-1])
-        # mesh.set_edgecolor('k')
-        # ax.add_collection3d(mesh)
-
-        # def maxmin(arr): return np.min(arr), np.max(arr)
-
-        # ax.set_xlim(*maxmin(verts.T[0]))  
-        # ax.set_ylim(*maxmin(verts.T[1])) 
-        # ax.set_zlim(*maxmin(verts.T[2])) 
-
-        # plt.tight_layout()
-        # plt.show()
-
         MeshView(out_file)
 
 
-def MeshView(objfile='model.obj',color='black',alpha=0.5,wireframe=False,wireframe_color='white',background_color='#ffffff', viewport = [1024, 768]):
+def MeshView(objfile='scene.obj',color='black',alpha=1,wireframe=True,wireframe_color='white',background_color='#cccccc', viewport = [1024, 768]):
     '''
     Triangulated mesh view with PyVista (GLOBAL)
     
     Parameters
     --------------
     objfile: string
         .obj file to process with MeshView [in GLOBAL function only]
@@ -484,40 +396,15 @@
     my_theme.background = background_color
 
 
     mesh = pyvista.read(objfile)
     mesh.plot(theme=my_theme,opacity=alpha,window_size = viewport)
     
 
-def objdraw(array,filename='voxelmodel.obj',color='black',alpha=0.5,wireframe=False,wireframe_color='white',background_color='#ffffff', viewport = [1024, 768]):
-    '''
-    Creates a 3-D voxel model (.obj file) from the provided, third-order (3-D) `array`. It then uses the global method MeshView to draw the .obj file and display it on screen 
-    
-    Parameters
-    ------------------
-    array : np.array(int)
-            array of the third-order populated with discrete, non-zero integers which may represent a voxel block type
-    filename : str
-            name of .obj file to save model as. 
-    objfile: string
-        .obj file to process with MeshView [in GLOBAL function only]
-    wireframe: bool
-        Represent mesh as wireframe instead of solid polyhedron if True (default: False). 
-    color : string / hexadecimal
-        mesh color. default: 'pink'
-    alpha : float
-        opacity transparency range: 0 - 1.0. Default: 0.5
-    background_color : string / hexadecimal
-        color of background. default: 'pink'
-    viewport : (int,int)
-        viewport / screen (width, height) for display window (default: 80% your screen's width & height)
-    '''
-    voxelwrite(array, filename = filename)
-    # MeshView(objfile=filename,wireframe=wireframe,color=color,alpha=alpha,background_color=background_color, viewport = viewport)
-    MeshView(filename,color,alpha,wireframe,wireframe_color,background_color, viewport )
+
 
 def xyz_to_sparse_array(df,hashblocks,spacing=1):
     '''
     Converts a pandas DataFrame df with columns 'x', 'y', 'z', and 'rgb' to a sparse 3D array. The function returns the array and a dictionary `hashblocks` that maps voxel colors to their corresponding index values in the array.
 
     Parameters
     -------------
@@ -562,22 +449,22 @@
                 i for i in hashblocks if hashblocks[i][0] == rgb][0]
         else:
             array[z, y, x] = elems[i][3]
 
     return array, hashblocks
 
 
-def wavefront_to_xyz(filename='model.obj'):
+def wavefront_to_xyz(filename='scene.obj'):
     '''
     Converts a Wavefront .obj file into a df pandas dataframe of vertex coordinates to be represented as a point cloud, where df has columns 'z', 'y', 'x', and 'rgb'. 
 
     Parameters
     ---------------
     filename : str, optional
-        The path and name of the .obj file to be read. Default is 'model.obj'.
+        The path and name of the .obj file to be read. Default is 'scene.obj'.
     '''
 
     # Read the .obj file into a list of strings
     with open(filename) as f:
         lines = f.readlines()
 
     # Initialize an empty list to hold the vertex coordinates
@@ -594,22 +481,22 @@
 
     # Convert the vertices list to a pandas dataframe with headers z, y, x, rgb
     df = pandas.DataFrame(vertices, columns=['z', 'y', 'x', 'rgb'])
 
     return df
 
 
-def objarray(filename='model.obj',spacing=1):
+def objcast(filename='scene.obj',spacing=1):
     '''
     Converts a Wavefront .obj file into a sparse, third-order (3-D) NumPy array to represent a point cloud model.
 
     Parameters
     ---------------
     filename : str 
-        Path to the .obj file. Defaults to 'model.obj'.
+        Path to the .obj file. Defaults to 'scene.obj'.
     spacing : float
         Distance between points in the point cloud. Can be adjusted to create a denser or sparser point cloud. Defaults to 1.
     '''
 
     df = wavefront_to_xyz(filename)
     hashblocks={}
     array, _ = xyz_to_sparse_array(df,hashblocks,spacing)
```

### Comparing `voxelmap-4.1.5/voxelmap/jotunn.py` & `voxelmap-4.2.0/voxelmap/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,29 +21,27 @@
 from scipy import ndimage
 from scipy.spatial import ConvexHull
 
 from voxelmap.annex import *
 
 # from scipy.spatial import Delaunay
 
-
-
 def SectorHull(array, sector_dims, Z_here, Z_there, Y_here, Y_there, X_here, X_there,  
                 num_simplices, rel_depth, color='orange', trace_min=1, plot=True, ax=[]):
     '''SectorHull does ConvexHull on a specific 2-D sector of the selected image
     adapted [ significantly ] from 
     https://stackoverflow.com/questions/27270477/3d-convex-hull-from-point-cloud'''
 
     sector = array[Y_here:Y_there, X_here:X_there] if sector_dims == 2 else \
              array[Z_here:Z_there, Y_here:Y_there, X_here:X_there]
 
 
     if len(np.unique(sector)) > trace_min:
         
-        points = arr2crds(sector, rel_depth) if sector_dims == 2 else tensor2crds(array, rel_depth)
+        points = matrix_toXY(sector, -rel_depth) if sector_dims == 2 else tensor_toXYZ(array, rel_depth)
 
         hull = ConvexHull(points)
 
         if plot=='mpl': 
             for s in hull.simplices:
                 s = np.append(s, s[0])  # Here we cycle back to the first coordinate
                 ax.plot(Y_here+points[s, 1],X_here+points[s, 0], Z_here+points[s, 2], color=color)
@@ -108,15 +106,15 @@
         self.make_intensity() if file != '' else None
 
         self.hashblocks = {}        # start with empty voxel-color dictionary
         self.colormap = cm.cool     # default: cool colormap
         self.alphacm = 1            # default: opaque colormap (alpha=1)
 
         # self.file = 'placeholder.txt'
-        self.objfile = 'model.obj'
+        self.objfile = 'scene.obj'
         self.XYZ = []
         self.RGB = []
         self.sparsity = 10.0
         
 
     def resize_intensity(self, res = 1.0, res_interp = cv2.INTER_AREA):
         '''Resize the intensity matrix of the provided image.
@@ -314,16 +312,16 @@
 
         voxels = Model(self.array).build()
 
         ax.voxels(voxels, facecolors=voxcolors, edgecolors=edgecolors)
         set_axes_equal(ax)
         plt.show()
 
-    def draw(self, coloring='none', geometry = 'voxels', scalars='', background_color='#cccccc', wireframe=False, wireframe_color='k', window_size=[1024, 768],voxel_spacing=(1,1,1)):
-        '''Draws voxel model after building it with the provided `array` with PyVista library
+    def draw(self, coloring='none', geometry = 'voxels', scalars='', background_color='#cccccc', wireframe=False, wireframe_color='k', window_size=[1024, 768],voxel_spacing=(1,1,1),show=True):
+        '''Draws voxel model after building it with the provided `array` with PyVista library 
 
         Parameters
         ----------
         coloring: string  
             voxel coloring scheme
                 * 'custom'                      --> colors voxel model based on the provided keys to its array integers, defined in the `hashblocks` variable from the `Model` class
                 * 'custom: #8599A6'             -->  color all voxel types with the #8599A6 hex color (bluish dark gray) and an alpha transparency of 1.0 (default)
@@ -345,17 +343,19 @@
             Represent mesh as wireframe instead of solid polyhedron if True (default: False). 
         wireframe_color: string / hex 
             edges or wireframe colors
         window_size : (float,float)
             defines plot window dimensions. Defaults to [1024, 768], unless set differently in the relevant theme’s window_size property [pyvista.Plotter]
         voxel_spacing : (float,float,float)
             changes voxel spacing by defining length scales of x y and z directions (default:(1,1,1)).
+        show : bool
+            Display Pyvista 3-D render of drawn 3-D model if True (default: True)
         '''
 
-        xx, yy, zz, voxid = arr2crds(self.array, -1).T
+        xx, yy, zz, voxid = matrix_toXY(self.array, 1).T
 
         centers = np.vstack((xx.ravel(), yy.ravel(), zz.ravel())).T
 
         pl = pyvista.Plotter(window_size=window_size)
 
         if background_color != "":
             pl.background_color = background_color
@@ -442,43 +442,52 @@
                 pl.add_mesh(voxel, color=voxel_color, smooth_shading=smooth, opacity=voxel_alpha,show_edges=True if wireframe else False, edge_color=wireframe_color)
             elif coloring == 'none':
                 pl.add_mesh(voxel,smooth_shading=smooth, show_edges=True if wireframe else False, edge_color=wireframe_color)
             else:
                 pl.add_mesh(voxel, scalars=[i for i in range(
                     8)] if scalars == '' else scalars,smooth_shading=smooth, show_edges=True if wireframe else False, edge_color=wireframe_color, cmap=coloring)
 
-        pl.isometric_view_interactive()
-        pl.show(interactive=True)
 
-    def save(self, filename='voxeldata.json'):
+        if show:
+            pl.isometric_view_interactive()
+            pl.show(interactive=True)
+
+        else:
+            return pl
+        
+
+    def save(self, filename='scene.json'):
         '''Save sparse array + color assignments Model data as a dictionary of keys (DOK) JSON file
 
         Parameters
         ----------
         filename: string  
-            name of file (e.g. 'voxeldata.json')
+            name of file (e.g. 'scene.json')
             Data types:
             .json -> voxel data represented as (DOK) JSON file 
             .txt -> voxel data represented x,y,z,rgb matrix in .txt file (see Goxel .txt imports)
         '''
         if filename[-4:] == 'json':
             tojson(filename, self.array, self.hashblocks)
+        elif filename[-4:] == '.obj':
+            pl = self.draw(show=False) 
+            pl.export_obj(filename)  
         else:
             toTXT(filename,self.array, self.hashblocks)
 
         return None
     
-    def load(self, filename='voxeldata.json', coords=False):
+    def load(self, filename='scene.json', coords=False):
         '''
         Load to Model object.
 
         Parameters
         ----------
         filename: string (.json or .txt extensions (see above))
-            name of file to be loaded (e.g 'voxeldata.json')
+            name of file to be loaded (e.g 'scene.json')
         coords: bool
             loads and processes self.XYZ, self.RGB, and self.sparsity = 10.0 (see Model class desc above) to Model if True. This boolean overrides filename loader option. 
         '''
         if coords:
             self.importdata(filename='')
         else:
             if filename[-4:] == 'json':
@@ -496,15 +505,15 @@
                     self.array[z, y, x] = data['val'][c]
 
             else:
                 self.importdata(filename)
 
 
 
-    def ImageMap(self,depth=5,out_file='model.obj',plot = False):
+    def ImageMap(self,depth=5,out_file='scene.obj',plot = False):
         '''Map image or 2-D array (matrix) to 3-D array
         
         Parameters
         -----------
         depth : int
             depth in number of voxels (default = 5 voxels)
         out_file : str
@@ -526,23 +535,25 @@
             for i in range(width):
                 pixel_intensity = matrix[j,i]
                 # k = findcrossover(intensities,0,depth-1, pixel_intensity)
                 # model[k-1][j][ i ] = 1
                 k = findclosest(intensities, pixel_intensity)
                 model[k][j][ i ] = 1
 
-        voxelwrite(model, filename =out_file)
+        # voxelwrite(model, filename =out_file)
+        self.array = model
+        self.save(filename=out_file)
         self.objfile = out_file 
 
         if plot:
             self.MeshView()
 
         return model
     
-    def ImageMesh(self, out_file='model.obj', L_sectors = 4, rel_depth = 0.50, trace_min = 1, plot = True, figsize=(4.8,4.8), verbose=False ):
+    def ImageMesh(self, out_file='scene.obj', L_sectors = 4, rel_depth = 0.50, trace_min = 1, plot = True, figsize=(4.8,4.8), verbose=False ):
         '''
         3-D triangulation of 2-D images / 2-D arrays (matrices) with a Convex Hull algorithm (Andrew Garcia, 2022)
 
         Parameters
         ------------
         out_file : str
             name and/or path for Wavefront .obj file output. This is the common format for OpenGL 3-D model files (default: model.obj) 
@@ -639,15 +650,15 @@
         # image in self.file mapped to 3d if self.file image specified else it takes the 3-D array defined in self.array
         array = self.ImageMap(voxel_depth) if self.file != '' else self.array              
 
         MarchingMesh(array, out_file=self.objfile, level=level,spacing=spacing, gradient_direction=gradient_direction, step_size=step_size, allow_degenerate=allow_degenerate, method=method, mask=mask, plot=plot, figsize=figsize)
         
         print('mesh created! saved as {}.'.format(self.objfile))
 
-    def MeshView(self,color='black',alpha=0.5,wireframe=False,wireframe_color='white',background_color='#ffffff', viewport = [1024, 768]):
+    def MeshView(self,color='black',alpha=1,wireframe=True,wireframe_color='white',background_color='#ffffff', viewport = [1024, 768]):
         '''
         Triangulated mesh view with PyVista
 
         Parameters
         --------------
         objfile: string
             .obj file to process with MeshView [in GLOBAL function only]
```

### Comparing `voxelmap-4.1.5/setup.py` & `voxelmap-4.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'scikit-image>=0.19.3,<0.20.0',
  'scipy>=1.10.0,<2.0.0',
  'sphinx-rtd-theme>=1.2.0,<2.0.0',
  'sphinx>=6.1.3,<7.0.0']
 
 setup_kwargs = {
     'name': 'voxelmap',
-    'version': '4.1.5',
+    'version': '4.2.0',
     'description': 'A Python library for making voxel and 3D models from NumPy arrays.',
     'long_description': '# voxelmap\n\n[![License](http://img.shields.io/:license-mit-blue.svg?style=flat-square)](https://raw.githubusercontent.com/andrewrgarcia/voxelmap/main/LICENSE)\n[![Documentation Status](https://readthedocs.org/projects/voxelmap/badge/?version=latest)](https://voxelmap.readthedocs.io/en/latest/?badge=latest)\n\nA Python library for making voxel and three-dimensional models from NumPy arrays. \n\n<a href="https://voxelmap.readthedocs.io/en/latest/">\n<img src="https://github.com/andrewrgarcia/voxelmap/blob/main/voxelmap.svg?raw=true" width="250"></a>\n\n## Installation and Local Usage \n\n```ruby\npip install voxelmap\n```\n\nIt is recommended you run voxelmap using a `virtualenv` virtual environment. To do so, follow the below simple protocol to create the virtual environment, run it, and install the package there:\n\n```ruby \nvirtualenv venv\nsource venv/bin/activate\npip install voxelmap\npython [your-voxelmap-script.py]\n```\nTo exit the virtual environment, simply type `deactivate`. To access it at any other time again, enter with the above `source venv...` command. \n\n## Just starting? Remote Usage with a Colab notebook (click below)\n\n<a href="https://colab.research.google.com/drive/1RMEMgZHlk_tKAzfS4QfXLJV9joDgdh8N?usp=sharing">\n<img src="https://raw.githubusercontent.com/andrewrgarcia/voxelmap/main/docs/img/colaboratory.png" width="500" ></a>\n\n\n## Disclaimer: Use At Your Own Risk\n\nThis program is free software. It comes without any warranty, to the extent permitted by applicable law. You can redistribute it and/or modify it under the terms of the MIT LICENSE, as published by Andrew Garcia. See LICENSE below for more details.\n\n**[MIT license](./LICENSE)** Copyright 2022 © <a href="https://github.com/andrewrgarcia" target="_blank">Andrew Garcia</a>.\n',
     'author': 'andrewrgarcia',
     'author_email': 'garcia.gtr@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['voxelmap']
 package_data = \ {'': ['*']} install_requires = \ ['colorcet>=3.0.1,<4.0.0',
 'matplotlib>=3.6.2,<4.0.0', 'numpy>=1.24.1,<2.0.0', 'opencv-
 python>=4.7.0.68,<5.0.0.0', 'pandas>=1.5.2,<2.0.0', 'pytest>=7.3.1,<8.0.0',
 'pyvista>=0.38.2,<0.39.0', 'scikit-image>=0.19.3,<0.20.0',
 'scipy>=1.10.0,<2.0.0', 'sphinx-rtd-theme>=1.2.0,<2.0.0',
 'sphinx>=6.1.3,<7.0.0'] setup_kwargs = { 'name': 'voxelmap', 'version':
-'4.1.5', 'description': 'A Python library for making voxel and 3D models from
+'4.2.0', 'description': 'A Python library for making voxel and 3D models from
 NumPy arrays.', 'long_description': '# voxelmap\n\n[![License](http://
 img.shields.io/:license-mit-blue.svg?style=flat-square)](https://
 raw.githubusercontent.com/andrewrgarcia/voxelmap/main/LICENSE)\n[!
 [Documentation Status](https://readthedocs.org/projects/voxelmap/badge/
 ?version=latest)](https://voxelmap.readthedocs.io/en/latest/?badge=latest)\n\nA
 Python library for making voxel and three-dimensional models from NumPy arrays.
 \n\n\n[https://github.com/andrewrgarcia/voxelmap/blob/main/
```

### Comparing `voxelmap-4.1.5/PKG-INFO` & `voxelmap-4.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voxelmap
-Version: 4.1.5
+Version: 4.2.0
 Summary: A Python library for making voxel and 3D models from NumPy arrays.
 License: MIT
 Author: andrewrgarcia
 Author-email: garcia.gtr@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: voxelmap Version: 4.1.5 Summary: A Python library
+Metadata-Version: 2.1 Name: voxelmap Version: 4.2.0 Summary: A Python library
 for making voxel and 3D models from NumPy arrays. License: MIT Author:
 andrewrgarcia Author-email: garcia.gtr@gmail.com Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: colorcet (>=3.0.1,<4.0.0) Requires-Dist: matplotlib
```

