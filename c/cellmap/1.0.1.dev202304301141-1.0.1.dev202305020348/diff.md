# Comparing `tmp/cellmap-1.0.1.dev202304301141-py3-none-any.whl.zip` & `tmp/cellmap-1.0.1.dev202305020348-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 19734 bytes, number of entries: 5
+Zip file size: 19828 bytes, number of entries: 5
 -rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 cellmap/__init__.py
--rw-r--r--  2.0 unx   112821 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
--rw-r--r--  2.0 unx     1869 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304301141.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304301141.dist-info/WHEEL
-?rw-r--r--  2.0 unx      405 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304301141.dist-info/RECORD
-5 files, 115235 bytes uncompressed, 18980 bytes compressed:  83.5%
+-rw-r--r--  2.0 unx   113385 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
+-rw-r--r--  2.0 unx     1869 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202305020348.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202305020348.dist-info/WHEEL
+?rw-r--r--  2.0 unx      405 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202305020348.dist-info/RECORD
+5 files, 115799 bytes uncompressed, 19074 bytes compressed:  83.5%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: cellmap/__init__.py
 Comment: 
 
 Filename: cellmap/cellmap.py
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304301141.dist-info/METADATA
+Filename: cellmap-1.0.1.dev202305020348.dist-info/METADATA
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304301141.dist-info/WHEEL
+Filename: cellmap-1.0.1.dev202305020348.dist-info/WHEEL
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304301141.dist-info/RECORD
+Filename: cellmap-1.0.1.dev202305020348.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cellmap/cellmap.py

```diff
@@ -1903,15 +1903,15 @@
                         ax1 = fig.add_subplot(grid[0:2,0:12])
                         ax2 = fig.add_subplot(grid[2:10,0:8])
                         ax3 = fig.add_subplot(grid[2:10,8:14])
                         update(t,name_i_,name_j_,max_val_,lim,i,j,k)
                         filename_ = '%s_%03d.%s' % (filename,t,save_type)
                         fig.savefig(filename_, bbox_inches='tight')
                         plt.close()
-                    matplotlib.use('TkAgg')
+                    matplotlib.use('module://matplotlib_inline.backend_inline')
                     
 
 def culc_bifurcation_diagram(
         adata,
         source_cluster,
         target_clusters,
         path_key = 'path',
@@ -2336,26 +2336,29 @@
             # annotations=annotations
         )
 
         fig = go.Figure(data=data_, layout=layout)
         pio.show(fig)
 
 
-def find_DEG_time(
+def key_gene_dynamics(
         adata,
         source_cluster,
         target_clusters,
         time,
         n_genes = 10,
         threshold_min = 1,
         path_key = 'path',
         exp_key = None,
         gene_dynamics_key = 'gene_dynamics',
         n_div = 100,
         fontsize_label = 10,
+        save = False,
+        save_dir = None,
+        save_filename = 'key_gene_dynamics',
     ):
 
     if gene_dynamics_key not in adata.uns.keys():
         culc_gene_dynamics(adata, source_cluster, target_clusters, path_key=path_key, exp_key=exp_key, gene_dynamics_key=gene_dynamics_key, n_div=n_div)
 
     idx_t_n_ = np.arange(n_div+1)[(np.linspace(0,1,n_div+1) <= time)]
     idx_t_p_ = np.arange(n_div+1)[(np.linspace(0,1,n_div+1) >= time)]
@@ -2400,8 +2403,13 @@
                 ax.axvline(time,color='r',zorder=1)
                 ax.text(time,0.95,str(time)+' ',color='r',zorder=1,va='top',ha='right',transform=ax.transAxes)
                 ax.set_xlim([0,1])
                 ax.set_xticks(vlines)
                 ax.set_xticklabels(vline_labels,fontsize=fontsize_label)
                 ax.spines['top'].set_visible(False)
                 ax.spines['right'].set_visible(False)
+                if save:
+                    filename = '%s' % (save_filename) if save_dir == None else '%s/%s' % (save_dir,save_filename)
+                    filename += target_clusters[i] + '_' + target_clusters[j]
+                    filename += '_{}'.format(round(time, len(str(n_div)))) + '_' + '%02d_' % (i_+1) + adata.var.index[idx_max_][diff_order_[i_]]
+                    fig.savefig(filename+'.png', bbox_inches='tight')
     display(out_pd_)
```

## Comparing `cellmap-1.0.1.dev202304301141.dist-info/METADATA` & `cellmap-1.0.1.dev202305020348.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmap
-Version: 1.0.1.dev202304301141
+Version: 1.0.1.dev202305020348
 Summary: CellMap - RNA landscape inference method
 Home-page: https://github.com/yusuke-imoto-lab/CellMap
 Author: Yusuke Imoto
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

