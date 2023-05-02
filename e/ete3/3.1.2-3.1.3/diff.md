# Comparing `tmp/ete3-3.1.2.tar.gz` & `tmp/ete3-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ete3-3.1.2.tar", last modified: Sun Aug 30 07:08:33 2020, max compression
+gzip compressed data, was "ete3-3.1.3.tar", last modified: Tue May  2 09:36:15 2023, max compression
```

## Comparing `ete3-3.1.2.tar` & `ete3-3.1.3.tar`

### file list

```diff
@@ -1,763 +1,763 @@
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      652 2020-08-30 07:08:26.000000 ete3-3.1.2/THANKS.rst
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      286 2020-08-30 07:08:26.000000 ete3-3.1.2/MANIFEST.in
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       38 2020-08-30 07:08:33.000000 ete3-3.1.2/setup.cfg
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2052 2020-08-30 07:08:33.000000 ete3-3.1.2/PKG-INFO
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/examples/
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/examples/clustering/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     3942 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/clustering/clustering_tree.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    38844 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/clustering/diauxic.array
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    15682 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/clustering/diauxic.nw
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1589 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/clustering/cluster_visualization.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2402 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/clustering/bubbles_validation.py
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/examples/nexml/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      329 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/nexml/nexml.xml
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1006 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/nexml/nexml_from_scratch.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     3531 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/nexml/tolweb.xml
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1029 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/nexml/nexml_annotated_trees.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     3162 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/nexml/taxa.xml
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     5195 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/nexml/trees.xml
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2129 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/nexml/nexml_parser.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    23870 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/nexml/characters.xml
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1960 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/nexml/phenoscape.xml
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    14324 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/nexml/timetree.xml
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     3771 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/nexml/02_dogfish_no_taxrefs.xml
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2058 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/nexml/meta_taxa.xml
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/examples/general/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2767 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/general/fish.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      726 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/general/genes_tree.nh
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     3212 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/general/get_midpoint_outgroup.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     4971 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/general/custom_tree_visualization.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1652 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/general/rooting_trees.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1115 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/general/chimp.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     4130 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/general/dog.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     3503 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/general/human.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1044 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/general/tree_traverse.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      541 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/general/custom_tree_traversing.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1036 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/general/getting_leaves.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      517 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/general/render_tree_images.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2768 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/general/remove_and_delete_nodes.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2464 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/general/get_distances_between_nodes.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      710 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/general/tree_basis.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1228 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/general/prune_tree.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1176 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/general/get_common_ancestor.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2124 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/general/add_features.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      589 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/general/label_nodes.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1887 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/general/copy_and_paste_trees.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      687 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/general/iterators.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     3971 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/general/fly.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1964 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/general/rooting_subtrees.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      749 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/general/byoperand_search.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      346 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/general/write_newick.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1735 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/general/create_trees_from_scratch.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)   103821 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/general/random_tree.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1324 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/general/mouse.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      517 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/general/search_nodes.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      420 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/general/read_newick.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2067 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/general/nhx_format.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      819 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/general/custom_search.py
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/examples/evol/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      869 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/test_hist.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      571 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/7_slr.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2184 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/2_sites_model.py
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/examples/evol/data/
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/examples/evol/data/L_example/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1258 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/L_example/alignment_L_measuring_evol.fasta
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      130 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/L_example/measuring_L_tree.nw
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/examples/evol/data/S_example/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       72 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/measuring_S_tree.nw
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1378 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/alignment_S_measuring_evol.fasta
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/examples/evol/data/S_example/paml/
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/examples/evol/data/S_example/paml/M1/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      143 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/M1/2NG.t
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       71 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/M1/tree
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    12125 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/M1/out
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      254 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/M1/4fold.nuc
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      143 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/M1/2NG.dS
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       79 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/M1/rst1
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      595 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/M1/tmp.ctl
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     4586 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/M1/lnf
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     3429 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/M1/rst
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      143 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/M1/2NG.dN
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       11 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/M1/rub
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1112 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/M1/algn
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/examples/evol/data/S_example/paml/fb/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      143 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/fb/2NG.t
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       71 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/fb/tree
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    12631 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/fb/out
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      254 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/fb/4fold.nuc
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      143 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/fb/2NG.dS
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     4657 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/fb/rst1
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      601 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/fb/tmp.ctl
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     4586 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/fb/lnf
--rw-rw-r--   0 huerta    (1000) huerta    (1000)   217002 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/fb/rst
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      143 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/fb/2NG.dN
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       11 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/fb/rub
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1112 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/fb/algn
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/examples/evol/data/S_example/paml/bsA1/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      143 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/bsA1/2NG.t
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       74 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/bsA1/tree
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    11769 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/bsA1/out
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      254 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/bsA1/4fold.nuc
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      143 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/bsA1/2NG.dS
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       85 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/bsA1/rst1
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      598 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/bsA1/tmp.ctl
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     4586 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/bsA1/lnf
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     4345 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/bsA1/rst
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      143 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/bsA1/2NG.dN
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       11 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/bsA1/rub
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1112 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/bsA1/algn
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/examples/evol/data/S_example/paml/M2/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      143 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/M2/2NG.t
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       71 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/M2/tree
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    12297 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/M2/out
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      254 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/M2/4fold.nuc
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      143 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/M2/2NG.dS
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       93 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/M2/rst1
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      591 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/M2/tmp.ctl
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     4681 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/M2/lnf
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     9821 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/M2/rst
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      143 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/M2/2NG.dN
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       11 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/M2/rub
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1112 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/M2/algn
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/examples/evol/data/S_example/paml/bsA/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      143 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/bsA/2NG.t
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       74 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/bsA/tree
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    12965 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/bsA/out
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      254 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/bsA/4fold.nuc
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      143 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/bsA/2NG.dS
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       91 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/bsA/rst1
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      600 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/bsA/tmp.ctl
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     4586 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/bsA/lnf
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     8374 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/bsA/rst
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      143 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/bsA/2NG.dN
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       11 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/bsA/rub
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1112 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/S_example/paml/bsA/algn
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/examples/evol/data/CladeModelCD/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      212 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/CladeModelCD/ECP_EDN_15.nw
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     7789 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/CladeModelCD/ECP_EDN_15.fasta
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/examples/evol/data/protamine/
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/slr/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/slr/2NG.t
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2027 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/slr/tree
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       83 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/slr/slr.ctl
--rw-rw-r--   0 huerta    (1000) huerta    (1000)   169966 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/slr/fb.out
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2064 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/slr/4fold.nuc
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/slr/2NG.dS
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        1 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/slr/rst1
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      478 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/slr/tmp.ctl
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    54234 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/slr/lnf
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/slr/2NG.dN
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       59 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/slr/rst.fb
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       11 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/slr/rub
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    21148 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/slr/algn
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      483 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/slr/tree.slr
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2026 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/tree.nw
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M0/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    40255 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M0/2NG.t
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2026 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M0/tree
--rw-rw-r--   0 huerta    (1000) huerta    (1000)   265562 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M0/out
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2064 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M0/4fold.nuc
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    40255 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M0/2NG.dS
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1211 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M0/rst1
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      424 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M0/tmp.ctl
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    54234 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M0/lnf
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       59 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M0/rst
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    40255 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M0/2NG.dN
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       11 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M0/rub
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    21148 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M0/algn
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M1/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M1/2NG.t
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2027 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M1/tree
--rw-rw-r--   0 huerta    (1000) huerta    (1000)   153567 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M1/M1.out
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2064 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M1/4fold.nuc
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M1/2NG.dS
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        1 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M1/rst1
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      428 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M1/tmp.ctl
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    54234 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M1/lnf
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2716 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M1/rst
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M1/2NG.dN
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       11 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M1/rub
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    21148 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M1/algn
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M8/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M8/2NG.t
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2027 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M8/tree
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2064 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M8/4fold.nuc
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M8/2NG.dS
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        1 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M8/rst1
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      428 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M8/tmp.ctl
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    54234 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M8/lnf
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    16616 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M8/rst
--rw-rw-r--   0 huerta    (1000) huerta    (1000)   155459 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M8/M8.out
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M8/2NG.dN
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       11 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M8/rub
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    21148 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M8/algn
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/fb/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/fb/2NG.t
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2027 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/fb/tree
--rw-rw-r--   0 huerta    (1000) huerta    (1000)   169966 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/fb/fb.out
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2064 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/fb/4fold.nuc
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/fb/2NG.dS
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        1 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/fb/rst1
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      478 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/fb/tmp.ctl
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    54234 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/fb/lnf
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/fb/2NG.dN
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       59 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/fb/rst.fb
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       11 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/fb/rub
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    21148 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/fb/algn
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M7/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M7/2NG.t
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2027 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M7/tree
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2064 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M7/4fold.nuc
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M7/2NG.dS
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        1 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M7/rst1
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      428 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M7/tmp.ctl
--rw-rw-r--   0 huerta    (1000) huerta    (1000)   153770 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M7/M7.out
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    54234 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M7/lnf
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     7022 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M7/rst
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M7/2NG.dN
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       11 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M7/rub
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    21148 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M7/algn
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M2/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M2/2NG.t
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2027 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M2/tree
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2064 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M2/4fold.nuc
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M2/2NG.dS
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        1 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M2/rst1
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      428 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M2/tmp.ctl
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    54234 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M2/lnf
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     8072 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M2/rst
--rw-rw-r--   0 huerta    (1000) huerta    (1000)   155576 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M2/M2.out
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M2/2NG.dN
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       11 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M2/rub
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    21148 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M2/algn
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    21140 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/data/protamine/PRM1/alignments.fasta_ali
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2804 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/4_branch_models.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1795 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/1_freeratio.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     7098 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/measuring_evolution_trees.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1902 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/5_branchsite_cladetest.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1456 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/test_protamine.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1312 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/6_ancestral_sequence.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      295 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/README
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2423 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/evol/3_branchsite_test.py
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/examples/phyloxml/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    38619 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/phyloxml/apaf.xml
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2062 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/phyloxml/example1.xml
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    14908 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/phyloxml/example3.xml
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    15291 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/phyloxml/phyloxml_examples.xml
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     3201 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/phyloxml/phyloxml_from_scratch.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)   564207 2020-08-30 07:08:27.000000 ete3-3.1.2/examples/phyloxml/tol_life_on_earth.xml.bz2
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      651 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/phyloxml/phyloxml_parser.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)   645989 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/phyloxml/ncbi_taxonomy_metazoa.xml.bz2
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1969 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/phyloxml/example2.xml
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     7233 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/phyloxml/multiple_supports.xml
--rw-rw-r--   0 huerta    (1000) huerta    (1000)   113544 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/phyloxml/bcl_2.xml
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/examples/treeview/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    10303 2020-08-30 07:08:27.000000 ete3-3.1.2/examples/treeview/node_style.png
--rwxrwxr-x   0 huerta    (1000) huerta    (1000)     1626 2020-08-30 07:08:27.000000 ete3-3.1.2/examples/treeview/face_grid.py
--rwxrwxr-x   0 huerta    (1000) huerta    (1000)     2039 2020-08-30 07:08:27.000000 ete3-3.1.2/examples/treeview/node_style.py
--rwxrwxr-x   0 huerta    (1000) huerta    (1000)     4012 2020-08-30 07:08:27.000000 ete3-3.1.2/examples/treeview/face_positions.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    16453 2020-08-30 07:08:27.000000 ete3-3.1.2/examples/treeview/seq_motif_faces.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    33022 2020-08-30 07:08:27.000000 ete3-3.1.2/examples/treeview/barcharts.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)   112579 2020-08-30 07:08:27.000000 ete3-3.1.2/examples/treeview/bubble_map.png
--rwxrwxr-x   0 huerta    (1000) huerta    (1000)     4141 2020-08-30 07:08:27.000000 ete3-3.1.2/examples/treeview/item_faces.py
--rwxrwxr-x   0 huerta    (1000) huerta    (1000)     1196 2020-08-30 07:08:27.000000 ete3-3.1.2/examples/treeview/node_background.py
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/examples/treeview/img_faces/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2767 2020-08-30 07:08:27.000000 ete3-3.1.2/examples/treeview/img_faces/fish.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    60235 2020-08-30 07:08:27.000000 ete3-3.1.2/examples/treeview/img_faces/img_faces.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1115 2020-08-30 07:08:27.000000 ete3-3.1.2/examples/treeview/img_faces/chimp.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     4130 2020-08-30 07:08:27.000000 ete3-3.1.2/examples/treeview/img_faces/dog.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     3503 2020-08-30 07:08:27.000000 ete3-3.1.2/examples/treeview/img_faces/human.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     3971 2020-08-30 07:08:27.000000 ete3-3.1.2/examples/treeview/img_faces/fly.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1324 2020-08-30 07:08:27.000000 ete3-3.1.2/examples/treeview/img_faces/mouse.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     5156 2020-08-30 07:08:27.000000 ete3-3.1.2/examples/treeview/img_faces/img_faces.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    35247 2020-08-30 07:08:27.000000 ete3-3.1.2/examples/treeview/item_faces.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)   289006 2020-08-30 07:08:27.000000 ete3-3.1.2/examples/treeview/float_piechart.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)   118000 2020-08-30 07:08:27.000000 ete3-3.1.2/examples/treeview/tree_faces.png
--rwxrwxr-x   0 huerta    (1000) huerta    (1000)     1357 2020-08-30 07:08:27.000000 ete3-3.1.2/examples/treeview/tree_faces.py
--rwxrwxr-x   0 huerta    (1000) huerta    (1000)     3714 2020-08-30 07:08:27.000000 ete3-3.1.2/examples/treeview/seq_motif_faces.py
--rwxrwxr-x   0 huerta    (1000) huerta    (1000)     1433 2020-08-30 07:08:27.000000 ete3-3.1.2/examples/treeview/barchart_and_piechart_faces.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    97444 2020-08-30 07:08:27.000000 ete3-3.1.2/examples/treeview/seqmotif.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    10961 2020-08-30 07:08:27.000000 ete3-3.1.2/examples/treeview/new_seq_face.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    33631 2020-08-30 07:08:27.000000 ete3-3.1.2/examples/treeview/rotated_faces.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    51805 2020-08-30 07:08:27.000000 ete3-3.1.2/examples/treeview/node_background.png
--rwxrwxr-x   0 huerta    (1000) huerta    (1000)      800 2020-08-30 07:08:27.000000 ete3-3.1.2/examples/treeview/face_rotation.py
--rwxrwxr-x   0 huerta    (1000) huerta    (1000)     1355 2020-08-30 07:08:27.000000 ete3-3.1.2/examples/treeview/bubble_map.py
--rwxrwxr-x   0 huerta    (1000) huerta    (1000)      840 2020-08-30 07:08:27.000000 ete3-3.1.2/examples/treeview/floating_piecharts.py
--rwxrwxr-x   0 huerta    (1000) huerta    (1000)     3818 2020-08-30 07:08:27.000000 ete3-3.1.2/examples/treeview/random_draw.py
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/examples/phylogenies/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    48918 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/phylogenies/phylotree.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     3112 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/phylogenies/link_sequences_to_phylogenies.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2863 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/phylogenies/dating_evolutionary_events.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1430 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/phylogenies/phylotree_visualization.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     3204 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/phylogenies/species_aware_phylogenies.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     3426 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/phylogenies/tree_reconciliation.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     3020 2020-08-30 07:08:26.000000 ete3-3.1.2/examples/phylogenies/orthology_and_paralogy_prediction.py
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/examples/webplugin/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    31079 2020-08-30 07:08:27.000000 ete3-3.1.2/examples/webplugin/jquery-ui-1.8.4.custom.min.js
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     7364 2020-08-30 07:08:27.000000 ete3-3.1.2/examples/webplugin/loader.gif
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1467 2020-08-30 07:08:27.000000 ete3-3.1.2/examples/webplugin/icon_cancel_search.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      735 2020-08-30 07:08:27.000000 ete3-3.1.2/examples/webplugin/close.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1947 2020-08-30 07:08:27.000000 ete3-3.1.2/examples/webplugin/webplugin_example.html
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1637 2020-08-30 07:08:27.000000 ete3-3.1.2/examples/webplugin/ete.css
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/examples/webplugin/wsgi/
--rwxrwxr-x   0 huerta    (1000) huerta    (1000)    22378 2020-08-30 07:08:27.000000 ete3-3.1.2/examples/webplugin/wsgi/webplugin_example.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1143 2020-08-30 07:08:27.000000 ete3-3.1.2/examples/webplugin/icon_tools.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    72174 2020-08-30 07:08:27.000000 ete3-3.1.2/examples/webplugin/jquery-1.4.2.min.js
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1661 2020-08-30 07:08:27.000000 ete3-3.1.2/examples/webplugin/icon_attachment.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1481 2020-08-30 07:08:27.000000 ete3-3.1.2/examples/webplugin/icon_search.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1238 2020-08-30 07:08:27.000000 ete3-3.1.2/examples/webplugin/README
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2252 2020-08-30 07:08:27.000000 ete3-3.1.2/examples/webplugin/ete.js
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        5 2020-08-30 07:08:26.000000 ete3-3.1.2/VERSION
--rwxrwxr-x   0 huerta    (1000) huerta    (1000)     5838 2020-08-30 07:08:27.000000 ete3-3.1.2/setup.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      522 2020-08-30 07:08:26.000000 ete3-3.1.2/CITATION.txt
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     3167 2020-08-30 07:08:26.000000 ete3-3.1.2/README.rst
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3.egg-info/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2052 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3.egg-info/PKG-INFO
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        5 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3.egg-info/top_level.txt
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       46 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3.egg-info/entry_points.txt
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        1 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3.egg-info/dependency_links.txt
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    27329 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3.egg-info/SOURCES.txt
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3/
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3/clustering/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1542 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/clustering/__init__.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     6288 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/clustering/clustvalidation.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     8555 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/clustering/clustertree.py
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3/ncbi_taxonomy/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1509 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/ncbi_taxonomy/__init__.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    32938 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/ncbi_taxonomy/ncbiquery.py
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3/ncbi_taxonomy/SQLite-Levenshtein/
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3/ncbi_taxonomy/SQLite-Levenshtein/src/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1603 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/ncbi_taxonomy/SQLite-Levenshtein/src/levenshtein.c
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      156 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/ncbi_taxonomy/SQLite-Levenshtein/Makefile
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3/ncbi_taxonomy/SQLite-Levenshtein/tests/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1801 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/ncbi_taxonomy/SQLite-Levenshtein/tests/levenshtein-test.sql
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      550 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/ncbi_taxonomy/SQLite-Levenshtein/tests/README
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       19 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/ncbi_taxonomy/SQLite-Levenshtein/.gitignore
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      271 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/ncbi_taxonomy/SQLite-Levenshtein/EXAMPLE
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      116 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/ncbi_taxonomy/SQLite-Levenshtein/README
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2422 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/__init__.py
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3/nexml/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     3264 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/nexml/__init__.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)   749400 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/nexml/_nexml.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     7101 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/nexml/_nexml_tree.py
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3/tools/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    15107 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_maptrees.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1445 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/__init__.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     4841 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_annotate.py
--rwxrwxr-x   0 huerta    (1000) huerta    (1000)    48239 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build.py
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3/tools/ete_build_lib/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     3540 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build_lib/getch.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     8342 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build_lib/visualize.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1445 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build_lib/__init__.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    18183 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build_lib/configcheck.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    10439 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build_lib/ordereddict.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     5978 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build_lib/sge.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    23315 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build_lib/master_task.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    16370 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build_lib/interface.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2724 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build_lib/logger.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    15996 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build_lib/db.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    28022 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build_lib/scheduler.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    88890 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build_lib/configobj.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     4295 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build_lib/curses_gui.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2131 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build_lib/errors.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    47320 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build_lib/validate.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    20613 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build_lib/utils.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     7168 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build_lib/apps.py
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3/tools/ete_build_lib/task/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    11871 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build_lib/task/concat_alg.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      648 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build_lib/task/__init__.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     6445 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build_lib/task/prottest2.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    10549 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build_lib/task/merger.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     6215 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build_lib/task/prottest.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2908 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build_lib/task/iqtree.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     9329 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build_lib/task/meta_aligner.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     4158 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build_lib/task/trimal.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     3066 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build_lib/task/msf.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2956 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build_lib/task/muscle.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1474 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build_lib/task/dummyalg.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    22121 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build_lib/task/cog_creator.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     3670 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build_lib/task/fasttree.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     3233 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build_lib/task/clustalo.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     3039 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build_lib/task/dialigntx.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2783 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build_lib/task/dummytree.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    11401 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build_lib/task/raxml.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2976 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build_lib/task/mafft.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     4331 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build_lib/task/uhire.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1526 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build_lib/task/tcoffee.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    10555 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build_lib/task/cog_selector.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     4092 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build_lib/task/jmodeltest.py
--rwxrwxr-x   0 huerta    (1000) huerta    (1000)     2413 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build_lib/task/pmodeltest.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     5739 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build_lib/task/phyml.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    11038 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build_lib/seqio.py
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3/tools/ete_build_lib/workflow/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1445 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build_lib/workflow/__init__.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    12687 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build_lib/workflow/supermatrix.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    20533 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build_lib/workflow/genetree.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    25825 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build_lib/workflow/common.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     8498 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build_lib/master_job.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    24626 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_view.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2089 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_split.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     8118 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_compare.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     4959 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_mod.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1713 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_expand.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     8531 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_ncbiquery.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    42798 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_evol.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    21605 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_build.cfg
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2246 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_extract.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     8266 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/common.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1324 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/utils.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2038 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_generate.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2344 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete_upgrade_tools.py
--rwxrwxr-x   0 huerta    (1000) huerta    (1000)     9846 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/tools/ete.py
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3/evol/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1801 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/evol/__init__.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    20476 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/evol/control.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    23604 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/evol/evoltree.py
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3/evol/parser/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1630 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/evol/parser/__init__.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    13344 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/evol/parser/codemlparser.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     3177 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/evol/parser/slrparser.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    15173 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/evol/model.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    12335 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/evol/utils.py
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3/phyloxml/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2456 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/phyloxml/__init__.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)   190180 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/phyloxml/_phyloxml.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     5845 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/phyloxml/_phyloxml_tree.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       73 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/version.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     4478 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/_ph.py
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3/treeview/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     4416 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/image_properties.ui
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1080 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/fit_region.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1284 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/zoom_in.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1553 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/__init__.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      751 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/filesave.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    15598 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/qt4_circular_render.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    10462 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/node_gui_actions.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2224 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/templates.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      867 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/ete_icon.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    35658 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/qt4_gui.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      583 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/force_topo.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1241 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/zoom_out.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     4263 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/search_dialog.ui
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      887 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/y_reduce.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)   114778 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/ete_resources_rc.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      962 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/fileopen.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     4969 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/drawer.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1639 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/search.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    28623 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/main.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      651 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/show_support.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     9590 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/layouts.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2521 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/_open_newick.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     5316 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/show_newick.ui
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      797 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/show_newick.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      920 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/x_reduce.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      491 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/show_names.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     5029 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/qt.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    15043 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/_mainwindow.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1500 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/fit_tree.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      760 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/ete_resources.qrc
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     4231 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/_about.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      838 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/y_expand.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    10717 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/ete_qt4app.ui
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      904 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/x_expand.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2279 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/about.ui
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     5756 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/ete_logo.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    14711 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/qt4_face_render.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1308 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/export_pdf.png
--rwxrwxr-x   0 huerta    (1000) huerta    (1000)      351 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/qt4_compile_resources.sh
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     6196 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/_show_newick.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     5120 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/_search_dialog.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    41790 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/svg_colors.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    88202 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/faces.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1808 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/clean_search.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     7271 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/_show_codeml.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      454 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/show_dist.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      773 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/open_newick.ui
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    44533 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/qt4_render.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     3872 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/treeview/qt4_rect_render.py
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3/test/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      210 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_all.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2131 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_xml_parsers.py
--rwxrwxr-x   0 huerta    (1000) huerta    (1000)     3550 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_circle_label.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/__init__.py
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3/test/test_issue258/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    83547 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_issue258/issue258.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2289 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_arraytable.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2203 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_ete_evol.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    17082 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_phylotree.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     9669 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_evol.py
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3/test/ete_evol_data/
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3/test/ete_evol_data/L_example/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1258 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/L_example/alignment_L_measuring_evol.fasta
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      130 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/L_example/measuring_L_tree.nw
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       72 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/tree.nw
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/M1/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      143 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/M1/2NG.t
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       71 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/M1/tree
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    12125 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/M1/out
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      254 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/M1/4fold.nuc
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      143 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/M1/2NG.dS
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       79 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/M1/rst1
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      595 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/M1/tmp.ctl
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     4586 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/M1/lnf
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     3429 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/M1/rst
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      143 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/M1/2NG.dN
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       11 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/M1/rub
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1112 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/M1/algn
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/fb/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      143 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/fb/2NG.t
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       71 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/fb/tree
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    12631 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/fb/out
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      254 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/fb/4fold.nuc
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      143 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/fb/2NG.dS
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     4657 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/fb/rst1
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      601 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/fb/tmp.ctl
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     4586 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/fb/lnf
--rw-rw-r--   0 huerta    (1000) huerta    (1000)   217002 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/fb/rst
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      143 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/fb/2NG.dN
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       11 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/fb/rub
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1112 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/fb/algn
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/bsA1/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      143 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/bsA1/2NG.t
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       74 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/bsA1/tree
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    11769 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/bsA1/out
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      254 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/bsA1/4fold.nuc
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      143 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/bsA1/2NG.dS
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       85 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/bsA1/rst1
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      598 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/bsA1/tmp.ctl
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     4586 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/bsA1/lnf
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     4345 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/bsA1/rst
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      143 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/bsA1/2NG.dN
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       11 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/bsA1/rub
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1112 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/bsA1/algn
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/M2/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      143 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/M2/2NG.t
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       71 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/M2/tree
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    12297 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/M2/out
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      254 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/M2/4fold.nuc
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      143 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/M2/2NG.dS
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       93 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/M2/rst1
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      591 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/M2/tmp.ctl
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     4681 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/M2/lnf
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     9821 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/M2/rst
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      143 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/M2/2NG.dN
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       11 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/M2/rub
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1112 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/M2/algn
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/bsA/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      143 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/bsA/2NG.t
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       74 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/bsA/tree
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    12965 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/bsA/out
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      254 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/bsA/4fold.nuc
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      143 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/bsA/2NG.dS
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       91 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/bsA/rst1
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      600 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/bsA/tmp.ctl
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     4586 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/bsA/lnf
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     8374 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/bsA/rst
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      143 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/bsA/2NG.dN
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       11 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/bsA/rub
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1112 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/bsA/algn
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1378 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/S_example/ali.fasta
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3/test/ete_evol_data/XS_example/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       35 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/XS_example/tree.nw
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       96 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/XS_example/ali.fasta
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3/test/ete_evol_data/CladeModelCD/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      212 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/CladeModelCD/ECP_EDN_15.nw
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     7789 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/CladeModelCD/ECP_EDN_15.fasta
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/slr/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/slr/2NG.t
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2027 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/slr/tree
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       83 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/slr/slr.ctl
--rw-rw-r--   0 huerta    (1000) huerta    (1000)   169966 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/slr/fb.out
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2064 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/slr/4fold.nuc
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/slr/2NG.dS
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        1 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/slr/rst1
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      478 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/slr/tmp.ctl
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    54234 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/slr/lnf
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/slr/2NG.dN
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       59 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/slr/rst.fb
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       11 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/slr/rub
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    21148 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/slr/algn
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      483 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/slr/tree.slr
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2026 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/tree.nw
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M0/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    40255 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M0/2NG.t
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2026 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M0/tree
--rw-rw-r--   0 huerta    (1000) huerta    (1000)   265562 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M0/out
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2064 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M0/4fold.nuc
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    40255 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M0/2NG.dS
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1211 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M0/rst1
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      424 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M0/tmp.ctl
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    54234 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M0/lnf
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       59 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M0/rst
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    40255 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M0/2NG.dN
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       11 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M0/rub
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    21148 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M0/algn
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M1/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M1/2NG.t
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2027 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M1/tree
--rw-rw-r--   0 huerta    (1000) huerta    (1000)   153567 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M1/M1.out
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2064 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M1/4fold.nuc
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M1/2NG.dS
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        1 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M1/rst1
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      428 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M1/tmp.ctl
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    54234 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M1/lnf
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2716 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M1/rst
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M1/2NG.dN
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       11 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M1/rub
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    21148 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M1/algn
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M8/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M8/2NG.t
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2027 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M8/tree
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2064 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M8/4fold.nuc
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M8/2NG.dS
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        1 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M8/rst1
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      428 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M8/tmp.ctl
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    54234 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M8/lnf
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    16616 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M8/rst
--rw-rw-r--   0 huerta    (1000) huerta    (1000)   155459 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M8/M8.out
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M8/2NG.dN
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       11 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M8/rub
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    21148 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M8/algn
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/fb/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/fb/2NG.t
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2027 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/fb/tree
--rw-rw-r--   0 huerta    (1000) huerta    (1000)   169966 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/fb/fb.out
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2064 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/fb/4fold.nuc
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/fb/2NG.dS
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        1 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/fb/rst1
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      478 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/fb/tmp.ctl
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    54234 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/fb/lnf
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/fb/2NG.dN
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       59 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/fb/rst.fb
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       11 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/fb/rub
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    21148 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/fb/algn
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M7/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M7/2NG.t
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2027 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M7/tree
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2064 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M7/4fold.nuc
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M7/2NG.dS
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        1 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M7/rst1
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      428 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M7/tmp.ctl
--rw-rw-r--   0 huerta    (1000) huerta    (1000)   153770 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M7/M7.out
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    54234 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M7/lnf
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     7022 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M7/rst
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M7/2NG.dN
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       11 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M7/rub
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    21148 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M7/algn
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M2/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M2/2NG.t
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2027 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M2/tree
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2064 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M2/4fold.nuc
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M2/2NG.dS
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        1 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M2/rst1
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      428 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M2/tmp.ctl
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    54234 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M2/lnf
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     8072 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M2/rst
--rw-rw-r--   0 huerta    (1000) huerta    (1000)   155576 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M2/M2.out
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M2/2NG.dN
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       11 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M2/rub
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    21148 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M2/algn
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    21140 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/alignments.fasta_ali
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     3778 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_seqgroup.py
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3/test/test_treeview/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2767 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_treeview/fish.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    60235 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_treeview/img_faces.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_treeview/__init__.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    10303 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_treeview/node_style.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     5093 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_treeview/test_all_treeview.py
--rwxrwxr-x   0 huerta    (1000) huerta    (1000)     1625 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_treeview/face_grid.py
--rwxrwxr-x   0 huerta    (1000) huerta    (1000)     2038 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_treeview/node_style.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1115 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_treeview/chimp.png
--rwxrwxr-x   0 huerta    (1000) huerta    (1000)     4011 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_treeview/face_positions.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)   163991 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_treeview/seq_motif_faces.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     4130 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_treeview/dog.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     3503 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_treeview/human.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    33022 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_treeview/barcharts.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)   174830 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_treeview/motifs.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)   112579 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_treeview/bubble_map.png
--rwxrwxr-x   0 huerta    (1000) huerta    (1000)     4163 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_treeview/item_faces.py
--rwxrwxr-x   0 huerta    (1000) huerta    (1000)     1195 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_treeview/node_background.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    35247 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_treeview/item_faces.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)   289006 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_treeview/float_piechart.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)   118000 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_treeview/tree_faces.png
--rwxrwxr-x   0 huerta    (1000) huerta    (1000)     1356 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_treeview/tree_faces.py
--rwxrwxr-x   0 huerta    (1000) huerta    (1000)     2300 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_treeview/seq_motif_faces.py
--rwxrwxr-x   0 huerta    (1000) huerta    (1000)     1370 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_treeview/barchart_and_piechart_faces.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    97444 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_treeview/seqmotif.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     5696 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_treeview/new_seq_face.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     3971 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_treeview/fly.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1429 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_treeview/phylotree_visualization.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    33631 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_treeview/rotated_faces.png
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    51805 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_treeview/node_background.png
--rwxrwxr-x   0 huerta    (1000) huerta    (1000)      799 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_treeview/face_rotation.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1324 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_treeview/mouse.png
--rwxrwxr-x   0 huerta    (1000) huerta    (1000)     1354 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_treeview/bubble_map.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     5155 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_treeview/img_faces.py
--rwxrwxr-x   0 huerta    (1000) huerta    (1000)      839 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_treeview/floating_piecharts.py
--rwxrwxr-x   0 huerta    (1000) huerta    (1000)     3814 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_treeview/random_draw.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    79064 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_tree.py
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3/test/test_ete_build/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)       63 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_ete_build/__init__.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      964 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_ete_build/cog_seqs.nt.fa
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      145 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_ete_build/fake_alg1.fa
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     3346 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_ete_build/P53.fa
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      127 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_ete_build/fake_cogs.tsv
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     3902 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_ete_build/test_manual_alg.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     7574 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_ete_build/NUP62.nt.fa
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      125 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_ete_build/fake_alg3.fa
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     3392 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_ete_build/P53.alg.fa
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      355 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_ete_build/fake_alg2.nt.fa
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2624 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_ete_build/test_sptree.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      284 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_ete_build/fake_alg3.nt.fa
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     3425 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_ete_build/test_modeltest.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2610 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_ete_build/NUP62.aa.fa
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      243 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_ete_build/__main__.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      428 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_ete_build/cog_seqs.fa
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      325 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_ete_build/fake_alg1.nt.fa
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1451 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_ete_build/test_genetree.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      155 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_ete_build/fake_alg2.fa
--rw-rw-r--   0 huerta    (1000) huerta    (1000)      463 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_api.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1484 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_interop.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     5601 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_ncbiquery.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    51563 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/datasets.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1017 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/test/test_clustertree.py
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3/parser/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1446 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/parser/__init__.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    20803 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/parser/newick.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     8130 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/parser/phylip.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     4449 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/parser/fasta.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     6363 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/parser/paml.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     5184 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/parser/text_arraytable.py
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3/orthoxml/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1509 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/orthoxml/__init__.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    85296 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/orthoxml/_orthoxml.py
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3/phylo/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1587 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/phylo/__init__.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    30595 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/phylo/phylotree.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     8169 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/phylo/reconciliation.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2573 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/phylo/evolevents.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     9007 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/phylo/spoverlap.py
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3/phylomedb/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     2411 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/phylomedb/__init__.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    26457 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/phylomedb/phylomeDB.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    61120 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/phylomedb/phylomeDB3.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     6080 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/citation.py
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3/coretype/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     9020 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/coretype/arraytable.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1446 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/coretype/__init__.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    97974 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/coretype/tree.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     6037 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/coretype/seqgroup.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     7913 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/utils.py
-drwxrwxr-x   0 huerta    (1000) huerta    (1000)        0 2020-08-30 07:08:33.000000 ete3-3.1.2/ete3/webplugin/
--rw-rw-r--   0 huerta    (1000) huerta    (1000)     1445 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/webplugin/__init__.py
--rwxrwxr-x   0 huerta    (1000) huerta    (1000)    15146 2020-08-30 07:08:26.000000 ete3-3.1.2/ete3/webplugin/webapp.py
--rw-rw-r--   0 huerta    (1000) huerta    (1000)    35147 2020-08-30 07:08:26.000000 ete3-3.1.2/LICENSE
--rwxrwxr-x   0 huerta    (1000) huerta    (1000)    10376 2020-08-30 07:08:27.000000 ete3-3.1.2/ez_setup.py
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.708094 ete3-3.1.3/
+-rw-r--r--   0 jaime      (501) staff       (20)      522 2023-05-02 08:57:16.000000 ete3-3.1.3/CITATION.txt
+-rw-r--r--   0 jaime      (501) staff       (20)    35147 2022-02-23 15:57:28.000000 ete3-3.1.3/LICENSE
+-rw-r--r--   0 jaime      (501) staff       (20)      286 2022-02-23 15:57:28.000000 ete3-3.1.3/MANIFEST.in
+-rw-r--r--   0 jaime      (501) staff       (20)     2062 2023-05-02 09:36:15.707619 ete3-3.1.3/PKG-INFO
+-rw-r--r--   0 jaime      (501) staff       (20)     3167 2023-05-02 08:57:16.000000 ete3-3.1.3/README.rst
+-rw-r--r--   0 jaime      (501) staff       (20)      652 2022-02-23 15:57:28.000000 ete3-3.1.3/THANKS.rst
+-rw-r--r--   0 jaime      (501) staff       (20)        5 2023-05-02 09:01:39.000000 ete3-3.1.3/VERSION
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.274228 ete3-3.1.3/ete3/
+-rw-r--r--   0 jaime      (501) staff       (20)     2422 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/__init__.py
+-rw-r--r--   0 jaime      (501) staff       (20)     4478 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/_ph.py
+-rw-r--r--   0 jaime      (501) staff       (20)     6080 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/citation.py
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.279327 ete3-3.1.3/ete3/clustering/
+-rw-r--r--   0 jaime      (501) staff       (20)     1542 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/clustering/__init__.py
+-rw-r--r--   0 jaime      (501) staff       (20)     8555 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/clustering/clustertree.py
+-rw-r--r--   0 jaime      (501) staff       (20)     6288 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/clustering/clustvalidation.py
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.281471 ete3-3.1.3/ete3/coretype/
+-rw-r--r--   0 jaime      (501) staff       (20)     1446 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/coretype/__init__.py
+-rw-r--r--   0 jaime      (501) staff       (20)     9020 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/coretype/arraytable.py
+-rw-r--r--   0 jaime      (501) staff       (20)     6037 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/coretype/seqgroup.py
+-rw-r--r--   0 jaime      (501) staff       (20)    97981 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/coretype/tree.py
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.284598 ete3-3.1.3/ete3/evol/
+-rw-r--r--   0 jaime      (501) staff       (20)     1801 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/evol/__init__.py
+-rw-r--r--   0 jaime      (501) staff       (20)    20476 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/evol/control.py
+-rw-r--r--   0 jaime      (501) staff       (20)    23623 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/evol/evoltree.py
+-rw-r--r--   0 jaime      (501) staff       (20)    15124 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/evol/model.py
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.286378 ete3-3.1.3/ete3/evol/parser/
+-rw-r--r--   0 jaime      (501) staff       (20)     1630 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/evol/parser/__init__.py
+-rw-r--r--   0 jaime      (501) staff       (20)    13338 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/evol/parser/codemlparser.py
+-rw-r--r--   0 jaime      (501) staff       (20)     3177 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/evol/parser/slrparser.py
+-rw-r--r--   0 jaime      (501) staff       (20)    12335 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/evol/utils.py
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.287700 ete3-3.1.3/ete3/ncbi_taxonomy/
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.290465 ete3-3.1.3/ete3/ncbi_taxonomy/SQLite-Levenshtein/
+-rw-r--r--   0 jaime      (501) staff       (20)       19 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/ncbi_taxonomy/SQLite-Levenshtein/.gitignore
+-rw-r--r--   0 jaime      (501) staff       (20)      271 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/ncbi_taxonomy/SQLite-Levenshtein/EXAMPLE
+-rw-r--r--   0 jaime      (501) staff       (20)      156 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/ncbi_taxonomy/SQLite-Levenshtein/Makefile
+-rw-r--r--   0 jaime      (501) staff       (20)      116 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/ncbi_taxonomy/SQLite-Levenshtein/README
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.291210 ete3-3.1.3/ete3/ncbi_taxonomy/SQLite-Levenshtein/src/
+-rw-r--r--   0 jaime      (501) staff       (20)     1603 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/ncbi_taxonomy/SQLite-Levenshtein/src/levenshtein.c
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.292443 ete3-3.1.3/ete3/ncbi_taxonomy/SQLite-Levenshtein/tests/
+-rw-r--r--   0 jaime      (501) staff       (20)      550 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/ncbi_taxonomy/SQLite-Levenshtein/tests/README
+-rw-r--r--   0 jaime      (501) staff       (20)     1801 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/ncbi_taxonomy/SQLite-Levenshtein/tests/levenshtein-test.sql
+-rw-r--r--   0 jaime      (501) staff       (20)     1509 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/ncbi_taxonomy/__init__.py
+-rw-r--r--   0 jaime      (501) staff       (20)    32987 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/ncbi_taxonomy/ncbiquery.py
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.295718 ete3-3.1.3/ete3/nexml/
+-rw-r--r--   0 jaime      (501) staff       (20)     3264 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/nexml/__init__.py
+-rw-r--r--   0 jaime      (501) staff       (20)   749400 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/nexml/_nexml.py
+-rw-r--r--   0 jaime      (501) staff       (20)     7101 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/nexml/_nexml_tree.py
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.297031 ete3-3.1.3/ete3/orthoxml/
+-rw-r--r--   0 jaime      (501) staff       (20)     1509 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/orthoxml/__init__.py
+-rw-r--r--   0 jaime      (501) staff       (20)    84921 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/orthoxml/_orthoxml.py
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.300767 ete3-3.1.3/ete3/parser/
+-rw-r--r--   0 jaime      (501) staff       (20)     1446 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/parser/__init__.py
+-rw-r--r--   0 jaime      (501) staff       (20)     4449 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/parser/fasta.py
+-rw-r--r--   0 jaime      (501) staff       (20)    20803 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/parser/newick.py
+-rw-r--r--   0 jaime      (501) staff       (20)     6363 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/parser/paml.py
+-rw-r--r--   0 jaime      (501) staff       (20)     8130 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/parser/phylip.py
+-rw-r--r--   0 jaime      (501) staff       (20)     5184 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/parser/text_arraytable.py
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.303512 ete3-3.1.3/ete3/phylo/
+-rw-r--r--   0 jaime      (501) staff       (20)     1587 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/phylo/__init__.py
+-rw-r--r--   0 jaime      (501) staff       (20)     2573 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/phylo/evolevents.py
+-rw-r--r--   0 jaime      (501) staff       (20)    30595 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/phylo/phylotree.py
+-rw-r--r--   0 jaime      (501) staff       (20)     8169 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/phylo/reconciliation.py
+-rw-r--r--   0 jaime      (501) staff       (20)     9007 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/phylo/spoverlap.py
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.305341 ete3-3.1.3/ete3/phylomedb/
+-rw-r--r--   0 jaime      (501) staff       (20)     2411 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/phylomedb/__init__.py
+-rw-r--r--   0 jaime      (501) staff       (20)    26457 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/phylomedb/phylomeDB.py
+-rw-r--r--   0 jaime      (501) staff       (20)    61120 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/phylomedb/phylomeDB3.py
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.307292 ete3-3.1.3/ete3/phyloxml/
+-rw-r--r--   0 jaime      (501) staff       (20)     2456 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/phyloxml/__init__.py
+-rw-r--r--   0 jaime      (501) staff       (20)   190180 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/phyloxml/_phyloxml.py
+-rw-r--r--   0 jaime      (501) staff       (20)     5845 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/phyloxml/_phyloxml_tree.py
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.315854 ete3-3.1.3/ete3/test/
+-rw-r--r--   0 jaime      (501) staff       (20)        0 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/__init__.py
+-rw-r--r--   0 jaime      (501) staff       (20)    51563 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/datasets.py
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.253539 ete3-3.1.3/ete3/test/ete_evol_data/
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.317052 ete3-3.1.3/ete3/test/ete_evol_data/CladeModelCD/
+-rw-r--r--   0 jaime      (501) staff       (20)     7789 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/CladeModelCD/ECP_EDN_15.fasta
+-rw-r--r--   0 jaime      (501) staff       (20)      212 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/CladeModelCD/ECP_EDN_15.nw
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.318353 ete3-3.1.3/ete3/test/ete_evol_data/L_example/
+-rw-r--r--   0 jaime      (501) staff       (20)     1258 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/L_example/alignment_L_measuring_evol.fasta
+-rw-r--r--   0 jaime      (501) staff       (20)      130 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/L_example/measuring_L_tree.nw
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.319722 ete3-3.1.3/ete3/test/ete_evol_data/S_example/
+-rw-r--r--   0 jaime      (501) staff       (20)     1378 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/ali.fasta
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.252971 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.326195 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/M1/
+-rw-r--r--   0 jaime      (501) staff       (20)      143 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/M1/2NG.dN
+-rw-r--r--   0 jaime      (501) staff       (20)      143 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/M1/2NG.dS
+-rw-r--r--   0 jaime      (501) staff       (20)      143 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/M1/2NG.t
+-rw-r--r--   0 jaime      (501) staff       (20)      254 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/M1/4fold.nuc
+-rw-r--r--   0 jaime      (501) staff       (20)     1112 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/M1/algn
+-rw-r--r--   0 jaime      (501) staff       (20)     4586 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/M1/lnf
+-rw-r--r--   0 jaime      (501) staff       (20)    12125 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/M1/out
+-rw-r--r--   0 jaime      (501) staff       (20)     3429 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/M1/rst
+-rw-r--r--   0 jaime      (501) staff       (20)       79 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/M1/rst1
+-rw-r--r--   0 jaime      (501) staff       (20)       11 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/M1/rub
+-rw-r--r--   0 jaime      (501) staff       (20)      595 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/M1/tmp.ctl
+-rw-r--r--   0 jaime      (501) staff       (20)       71 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/M1/tree
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.333444 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/M2/
+-rw-r--r--   0 jaime      (501) staff       (20)      143 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/M2/2NG.dN
+-rw-r--r--   0 jaime      (501) staff       (20)      143 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/M2/2NG.dS
+-rw-r--r--   0 jaime      (501) staff       (20)      143 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/M2/2NG.t
+-rw-r--r--   0 jaime      (501) staff       (20)      254 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/M2/4fold.nuc
+-rw-r--r--   0 jaime      (501) staff       (20)     1112 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/M2/algn
+-rw-r--r--   0 jaime      (501) staff       (20)     4681 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/M2/lnf
+-rw-r--r--   0 jaime      (501) staff       (20)    12297 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/M2/out
+-rw-r--r--   0 jaime      (501) staff       (20)     9821 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/M2/rst
+-rw-r--r--   0 jaime      (501) staff       (20)       93 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/M2/rst1
+-rw-r--r--   0 jaime      (501) staff       (20)       11 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/M2/rub
+-rw-r--r--   0 jaime      (501) staff       (20)      591 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/M2/tmp.ctl
+-rw-r--r--   0 jaime      (501) staff       (20)       71 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/M2/tree
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.340986 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/bsA/
+-rw-r--r--   0 jaime      (501) staff       (20)      143 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/bsA/2NG.dN
+-rw-r--r--   0 jaime      (501) staff       (20)      143 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/bsA/2NG.dS
+-rw-r--r--   0 jaime      (501) staff       (20)      143 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/bsA/2NG.t
+-rw-r--r--   0 jaime      (501) staff       (20)      254 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/bsA/4fold.nuc
+-rw-r--r--   0 jaime      (501) staff       (20)     1112 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/bsA/algn
+-rw-r--r--   0 jaime      (501) staff       (20)     4586 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/bsA/lnf
+-rw-r--r--   0 jaime      (501) staff       (20)    12965 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/bsA/out
+-rw-r--r--   0 jaime      (501) staff       (20)     8374 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/bsA/rst
+-rw-r--r--   0 jaime      (501) staff       (20)       91 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/bsA/rst1
+-rw-r--r--   0 jaime      (501) staff       (20)       11 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/bsA/rub
+-rw-r--r--   0 jaime      (501) staff       (20)      600 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/bsA/tmp.ctl
+-rw-r--r--   0 jaime      (501) staff       (20)       74 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/bsA/tree
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.349387 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/bsA1/
+-rw-r--r--   0 jaime      (501) staff       (20)      143 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/bsA1/2NG.dN
+-rw-r--r--   0 jaime      (501) staff       (20)      143 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/bsA1/2NG.dS
+-rw-r--r--   0 jaime      (501) staff       (20)      143 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/bsA1/2NG.t
+-rw-r--r--   0 jaime      (501) staff       (20)      254 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/bsA1/4fold.nuc
+-rw-r--r--   0 jaime      (501) staff       (20)     1112 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/bsA1/algn
+-rw-r--r--   0 jaime      (501) staff       (20)     4586 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/bsA1/lnf
+-rw-r--r--   0 jaime      (501) staff       (20)    11769 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/bsA1/out
+-rw-r--r--   0 jaime      (501) staff       (20)     4345 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/bsA1/rst
+-rw-r--r--   0 jaime      (501) staff       (20)       85 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/bsA1/rst1
+-rw-r--r--   0 jaime      (501) staff       (20)       11 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/bsA1/rub
+-rw-r--r--   0 jaime      (501) staff       (20)      598 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/bsA1/tmp.ctl
+-rw-r--r--   0 jaime      (501) staff       (20)       74 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/bsA1/tree
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.357083 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/fb/
+-rw-r--r--   0 jaime      (501) staff       (20)      143 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/fb/2NG.dN
+-rw-r--r--   0 jaime      (501) staff       (20)      143 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/fb/2NG.dS
+-rw-r--r--   0 jaime      (501) staff       (20)      143 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/fb/2NG.t
+-rw-r--r--   0 jaime      (501) staff       (20)      254 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/fb/4fold.nuc
+-rw-r--r--   0 jaime      (501) staff       (20)     1112 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/fb/algn
+-rw-r--r--   0 jaime      (501) staff       (20)     4586 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/fb/lnf
+-rw-r--r--   0 jaime      (501) staff       (20)    12631 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/fb/out
+-rw-r--r--   0 jaime      (501) staff       (20)   217002 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/fb/rst
+-rw-r--r--   0 jaime      (501) staff       (20)     4657 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/fb/rst1
+-rw-r--r--   0 jaime      (501) staff       (20)       11 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/fb/rub
+-rw-r--r--   0 jaime      (501) staff       (20)      601 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/fb/tmp.ctl
+-rw-r--r--   0 jaime      (501) staff       (20)       71 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/fb/tree
+-rw-r--r--   0 jaime      (501) staff       (20)       72 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/S_example/tree.nw
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.358060 ete3-3.1.3/ete3/test/ete_evol_data/XS_example/
+-rw-r--r--   0 jaime      (501) staff       (20)       96 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/XS_example/ali.fasta
+-rw-r--r--   0 jaime      (501) staff       (20)       35 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/XS_example/tree.nw
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.253701 ete3-3.1.3/ete3/test/ete_evol_data/protamine/
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.360415 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/
+-rw-r--r--   0 jaime      (501) staff       (20)    21140 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/alignments.fasta_ali
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.255592 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.369800 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M0/
+-rw-r--r--   0 jaime      (501) staff       (20)    40255 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M0/2NG.dN
+-rw-r--r--   0 jaime      (501) staff       (20)    40255 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M0/2NG.dS
+-rw-r--r--   0 jaime      (501) staff       (20)    40255 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M0/2NG.t
+-rw-r--r--   0 jaime      (501) staff       (20)     2064 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M0/4fold.nuc
+-rw-r--r--   0 jaime      (501) staff       (20)    21148 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M0/algn
+-rw-r--r--   0 jaime      (501) staff       (20)    54234 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M0/lnf
+-rw-r--r--   0 jaime      (501) staff       (20)   265562 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M0/out
+-rw-r--r--   0 jaime      (501) staff       (20)       59 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M0/rst
+-rw-r--r--   0 jaime      (501) staff       (20)     1211 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M0/rst1
+-rw-r--r--   0 jaime      (501) staff       (20)       11 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M0/rub
+-rw-r--r--   0 jaime      (501) staff       (20)      424 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M0/tmp.ctl
+-rw-r--r--   0 jaime      (501) staff       (20)     2026 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M0/tree
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.376067 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M1/
+-rw-r--r--   0 jaime      (501) staff       (20)        0 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M1/2NG.dN
+-rw-r--r--   0 jaime      (501) staff       (20)        0 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M1/2NG.dS
+-rw-r--r--   0 jaime      (501) staff       (20)        0 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M1/2NG.t
+-rw-r--r--   0 jaime      (501) staff       (20)     2064 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M1/4fold.nuc
+-rw-r--r--   0 jaime      (501) staff       (20)   153567 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M1/M1.out
+-rw-r--r--   0 jaime      (501) staff       (20)    21148 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M1/algn
+-rw-r--r--   0 jaime      (501) staff       (20)    54234 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M1/lnf
+-rw-r--r--   0 jaime      (501) staff       (20)     2716 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M1/rst
+-rw-r--r--   0 jaime      (501) staff       (20)        1 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M1/rst1
+-rw-r--r--   0 jaime      (501) staff       (20)       11 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M1/rub
+-rw-r--r--   0 jaime      (501) staff       (20)      428 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M1/tmp.ctl
+-rw-r--r--   0 jaime      (501) staff       (20)     2027 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M1/tree
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.383169 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M2/
+-rw-r--r--   0 jaime      (501) staff       (20)        0 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M2/2NG.dN
+-rw-r--r--   0 jaime      (501) staff       (20)        0 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M2/2NG.dS
+-rw-r--r--   0 jaime      (501) staff       (20)        0 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M2/2NG.t
+-rw-r--r--   0 jaime      (501) staff       (20)     2064 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M2/4fold.nuc
+-rw-r--r--   0 jaime      (501) staff       (20)   155576 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M2/M2.out
+-rw-r--r--   0 jaime      (501) staff       (20)    21148 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M2/algn
+-rw-r--r--   0 jaime      (501) staff       (20)    54234 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M2/lnf
+-rw-r--r--   0 jaime      (501) staff       (20)     8072 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M2/rst
+-rw-r--r--   0 jaime      (501) staff       (20)        1 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M2/rst1
+-rw-r--r--   0 jaime      (501) staff       (20)       11 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M2/rub
+-rw-r--r--   0 jaime      (501) staff       (20)      428 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M2/tmp.ctl
+-rw-r--r--   0 jaime      (501) staff       (20)     2027 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M2/tree
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.392322 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M7/
+-rw-r--r--   0 jaime      (501) staff       (20)        0 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M7/2NG.dN
+-rw-r--r--   0 jaime      (501) staff       (20)        0 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M7/2NG.dS
+-rw-r--r--   0 jaime      (501) staff       (20)        0 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M7/2NG.t
+-rw-r--r--   0 jaime      (501) staff       (20)     2064 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M7/4fold.nuc
+-rw-r--r--   0 jaime      (501) staff       (20)   153770 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M7/M7.out
+-rw-r--r--   0 jaime      (501) staff       (20)    21148 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M7/algn
+-rw-r--r--   0 jaime      (501) staff       (20)    54234 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M7/lnf
+-rw-r--r--   0 jaime      (501) staff       (20)     7022 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M7/rst
+-rw-r--r--   0 jaime      (501) staff       (20)        1 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M7/rst1
+-rw-r--r--   0 jaime      (501) staff       (20)       11 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M7/rub
+-rw-r--r--   0 jaime      (501) staff       (20)      428 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M7/tmp.ctl
+-rw-r--r--   0 jaime      (501) staff       (20)     2027 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M7/tree
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.401618 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M8/
+-rw-r--r--   0 jaime      (501) staff       (20)        0 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M8/2NG.dN
+-rw-r--r--   0 jaime      (501) staff       (20)        0 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M8/2NG.dS
+-rw-r--r--   0 jaime      (501) staff       (20)        0 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M8/2NG.t
+-rw-r--r--   0 jaime      (501) staff       (20)     2064 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M8/4fold.nuc
+-rw-r--r--   0 jaime      (501) staff       (20)   155459 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M8/M8.out
+-rw-r--r--   0 jaime      (501) staff       (20)    21148 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M8/algn
+-rw-r--r--   0 jaime      (501) staff       (20)    54234 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M8/lnf
+-rw-r--r--   0 jaime      (501) staff       (20)    16616 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M8/rst
+-rw-r--r--   0 jaime      (501) staff       (20)        1 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M8/rst1
+-rw-r--r--   0 jaime      (501) staff       (20)       11 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M8/rub
+-rw-r--r--   0 jaime      (501) staff       (20)      428 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M8/tmp.ctl
+-rw-r--r--   0 jaime      (501) staff       (20)     2027 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M8/tree
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.412598 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/fb/
+-rw-r--r--   0 jaime      (501) staff       (20)        0 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/fb/2NG.dN
+-rw-r--r--   0 jaime      (501) staff       (20)        0 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/fb/2NG.dS
+-rw-r--r--   0 jaime      (501) staff       (20)        0 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/fb/2NG.t
+-rw-r--r--   0 jaime      (501) staff       (20)     2064 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/fb/4fold.nuc
+-rw-r--r--   0 jaime      (501) staff       (20)    21148 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/fb/algn
+-rw-r--r--   0 jaime      (501) staff       (20)   169966 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/fb/fb.out
+-rw-r--r--   0 jaime      (501) staff       (20)    54234 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/fb/lnf
+-rw-r--r--   0 jaime      (501) staff       (20)       59 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/fb/rst.fb
+-rw-r--r--   0 jaime      (501) staff       (20)        1 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/fb/rst1
+-rw-r--r--   0 jaime      (501) staff       (20)       11 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/fb/rub
+-rw-r--r--   0 jaime      (501) staff       (20)      478 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/fb/tmp.ctl
+-rw-r--r--   0 jaime      (501) staff       (20)     2027 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/fb/tree
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.422236 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/slr/
+-rw-r--r--   0 jaime      (501) staff       (20)        0 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/slr/2NG.dN
+-rw-r--r--   0 jaime      (501) staff       (20)        0 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/slr/2NG.dS
+-rw-r--r--   0 jaime      (501) staff       (20)        0 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/slr/2NG.t
+-rw-r--r--   0 jaime      (501) staff       (20)     2064 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/slr/4fold.nuc
+-rw-r--r--   0 jaime      (501) staff       (20)    21148 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/slr/algn
+-rw-r--r--   0 jaime      (501) staff       (20)   169966 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/slr/fb.out
+-rw-r--r--   0 jaime      (501) staff       (20)    54234 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/slr/lnf
+-rw-r--r--   0 jaime      (501) staff       (20)       59 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/slr/rst.fb
+-rw-r--r--   0 jaime      (501) staff       (20)        1 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/slr/rst1
+-rw-r--r--   0 jaime      (501) staff       (20)       11 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/slr/rub
+-rw-r--r--   0 jaime      (501) staff       (20)       83 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/slr/slr.ctl
+-rw-r--r--   0 jaime      (501) staff       (20)      478 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/slr/tmp.ctl
+-rw-r--r--   0 jaime      (501) staff       (20)     2027 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/slr/tree
+-rw-r--r--   0 jaime      (501) staff       (20)      483 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/slr/tree.slr
+-rw-r--r--   0 jaime      (501) staff       (20)     2026 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/tree.nw
+-rw-r--r--   0 jaime      (501) staff       (20)      210 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_all.py
+-rw-r--r--   0 jaime      (501) staff       (20)      463 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_api.py
+-rw-r--r--   0 jaime      (501) staff       (20)     2289 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_arraytable.py
+-rwxr-xr-x   0 jaime      (501) staff       (20)     3550 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_circle_label.py
+-rw-r--r--   0 jaime      (501) staff       (20)     1017 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_clustertree.py
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.433737 ete3-3.1.3/ete3/test/test_ete_build/
+-rw-r--r--   0 jaime      (501) staff       (20)     2610 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_ete_build/NUP62.aa.fa
+-rw-r--r--   0 jaime      (501) staff       (20)     7574 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_ete_build/NUP62.nt.fa
+-rw-r--r--   0 jaime      (501) staff       (20)     3392 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_ete_build/P53.alg.fa
+-rw-r--r--   0 jaime      (501) staff       (20)     3346 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_ete_build/P53.fa
+-rw-r--r--   0 jaime      (501) staff       (20)       63 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_ete_build/__init__.py
+-rw-r--r--   0 jaime      (501) staff       (20)      243 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_ete_build/__main__.py
+-rw-r--r--   0 jaime      (501) staff       (20)      428 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_ete_build/cog_seqs.fa
+-rw-r--r--   0 jaime      (501) staff       (20)      964 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_ete_build/cog_seqs.nt.fa
+-rw-r--r--   0 jaime      (501) staff       (20)      145 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_ete_build/fake_alg1.fa
+-rw-r--r--   0 jaime      (501) staff       (20)      325 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_ete_build/fake_alg1.nt.fa
+-rw-r--r--   0 jaime      (501) staff       (20)      155 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_ete_build/fake_alg2.fa
+-rw-r--r--   0 jaime      (501) staff       (20)      355 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_ete_build/fake_alg2.nt.fa
+-rw-r--r--   0 jaime      (501) staff       (20)      125 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_ete_build/fake_alg3.fa
+-rw-r--r--   0 jaime      (501) staff       (20)      284 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_ete_build/fake_alg3.nt.fa
+-rw-r--r--   0 jaime      (501) staff       (20)      127 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_ete_build/fake_cogs.tsv
+-rw-r--r--   0 jaime      (501) staff       (20)     1451 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_ete_build/test_genetree.py
+-rw-r--r--   0 jaime      (501) staff       (20)     3902 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_ete_build/test_manual_alg.py
+-rw-r--r--   0 jaime      (501) staff       (20)     3425 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_ete_build/test_modeltest.py
+-rw-r--r--   0 jaime      (501) staff       (20)     2624 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_ete_build/test_sptree.py
+-rw-r--r--   0 jaime      (501) staff       (20)     2203 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_ete_evol.py
+-rw-r--r--   0 jaime      (501) staff       (20)     9669 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_evol.py
+-rw-r--r--   0 jaime      (501) staff       (20)     1484 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_interop.py
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.434329 ete3-3.1.3/ete3/test/test_issue258/
+-rw-r--r--   0 jaime      (501) staff       (20)    83547 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_issue258/issue258.py
+-rw-r--r--   0 jaime      (501) staff       (20)     5646 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_ncbiquery.py
+-rw-r--r--   0 jaime      (501) staff       (20)    17082 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_phylotree.py
+-rw-r--r--   0 jaime      (501) staff       (20)     3778 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_seqgroup.py
+-rw-r--r--   0 jaime      (501) staff       (20)    79064 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_tree.py
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.457525 ete3-3.1.3/ete3/test/test_treeview/
+-rw-r--r--   0 jaime      (501) staff       (20)        0 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_treeview/__init__.py
+-rwxr-xr-x   0 jaime      (501) staff       (20)     1378 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_treeview/barchart_and_piechart_faces.py
+-rw-r--r--   0 jaime      (501) staff       (20)    33022 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_treeview/barcharts.png
+-rw-r--r--   0 jaime      (501) staff       (20)   112579 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_treeview/bubble_map.png
+-rwxr-xr-x   0 jaime      (501) staff       (20)     1354 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_treeview/bubble_map.py
+-rw-r--r--   0 jaime      (501) staff       (20)     1115 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_treeview/chimp.png
+-rw-r--r--   0 jaime      (501) staff       (20)     4130 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_treeview/dog.png
+-rwxr-xr-x   0 jaime      (501) staff       (20)     1625 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_treeview/face_grid.py
+-rwxr-xr-x   0 jaime      (501) staff       (20)     4011 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_treeview/face_positions.py
+-rwxr-xr-x   0 jaime      (501) staff       (20)      799 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_treeview/face_rotation.py
+-rw-r--r--   0 jaime      (501) staff       (20)     2767 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_treeview/fish.png
+-rw-r--r--   0 jaime      (501) staff       (20)   289006 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_treeview/float_piechart.png
+-rwxr-xr-x   0 jaime      (501) staff       (20)      839 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_treeview/floating_piecharts.py
+-rw-r--r--   0 jaime      (501) staff       (20)     3971 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_treeview/fly.png
+-rw-r--r--   0 jaime      (501) staff       (20)     3503 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_treeview/human.png
+-rw-r--r--   0 jaime      (501) staff       (20)    60235 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_treeview/img_faces.png
+-rw-r--r--   0 jaime      (501) staff       (20)     5155 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_treeview/img_faces.py
+-rw-r--r--   0 jaime      (501) staff       (20)    35247 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_treeview/item_faces.png
+-rwxr-xr-x   0 jaime      (501) staff       (20)     4163 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_treeview/item_faces.py
+-rw-r--r--   0 jaime      (501) staff       (20)   174830 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_treeview/motifs.png
+-rw-r--r--   0 jaime      (501) staff       (20)     1324 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_treeview/mouse.png
+-rw-r--r--   0 jaime      (501) staff       (20)     5696 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_treeview/new_seq_face.py
+-rw-r--r--   0 jaime      (501) staff       (20)    51805 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_treeview/node_background.png
+-rwxr-xr-x   0 jaime      (501) staff       (20)     1195 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_treeview/node_background.py
+-rw-r--r--   0 jaime      (501) staff       (20)    10303 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_treeview/node_style.png
+-rwxr-xr-x   0 jaime      (501) staff       (20)     2038 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_treeview/node_style.py
+-rw-r--r--   0 jaime      (501) staff       (20)     1429 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_treeview/phylotree_visualization.py
+-rwxr-xr-x   0 jaime      (501) staff       (20)     3814 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_treeview/random_draw.py
+-rw-r--r--   0 jaime      (501) staff       (20)    33631 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_treeview/rotated_faces.png
+-rw-r--r--   0 jaime      (501) staff       (20)   163991 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_treeview/seq_motif_faces.png
+-rwxr-xr-x   0 jaime      (501) staff       (20)     2300 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_treeview/seq_motif_faces.py
+-rw-r--r--   0 jaime      (501) staff       (20)    97444 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_treeview/seqmotif.png
+-rw-r--r--   0 jaime      (501) staff       (20)     5093 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_treeview/test_all_treeview.py
+-rw-r--r--   0 jaime      (501) staff       (20)   118000 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_treeview/tree_faces.png
+-rwxr-xr-x   0 jaime      (501) staff       (20)     1356 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_treeview/tree_faces.py
+-rw-r--r--   0 jaime      (501) staff       (20)     2131 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/test/test_xml_parsers.py
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.467568 ete3-3.1.3/ete3/tools/
+-rw-r--r--   0 jaime      (501) staff       (20)     1445 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/__init__.py
+-rw-r--r--   0 jaime      (501) staff       (20)     8266 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/common.py
+-rwxr-xr-x   0 jaime      (501) staff       (20)     9846 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete.py
+-rw-r--r--   0 jaime      (501) staff       (20)     4841 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_annotate.py
+-rw-r--r--   0 jaime      (501) staff       (20)    21605 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build.cfg
+-rwxr-xr-x   0 jaime      (501) staff       (20)    48239 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build.py
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.478141 ete3-3.1.3/ete3/tools/ete_build_lib/
+-rw-r--r--   0 jaime      (501) staff       (20)     1445 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build_lib/__init__.py
+-rw-r--r--   0 jaime      (501) staff       (20)     7168 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build_lib/apps.py
+-rw-r--r--   0 jaime      (501) staff       (20)    18183 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build_lib/configcheck.py
+-rw-r--r--   0 jaime      (501) staff       (20)    88890 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build_lib/configobj.py
+-rw-r--r--   0 jaime      (501) staff       (20)     4295 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build_lib/curses_gui.py
+-rw-r--r--   0 jaime      (501) staff       (20)    15996 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build_lib/db.py
+-rw-r--r--   0 jaime      (501) staff       (20)     2131 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build_lib/errors.py
+-rw-r--r--   0 jaime      (501) staff       (20)     3540 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build_lib/getch.py
+-rw-r--r--   0 jaime      (501) staff       (20)    16370 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build_lib/interface.py
+-rw-r--r--   0 jaime      (501) staff       (20)     2724 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build_lib/logger.py
+-rw-r--r--   0 jaime      (501) staff       (20)     8498 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build_lib/master_job.py
+-rw-r--r--   0 jaime      (501) staff       (20)    23315 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build_lib/master_task.py
+-rw-r--r--   0 jaime      (501) staff       (20)    10439 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build_lib/ordereddict.py
+-rw-r--r--   0 jaime      (501) staff       (20)    28022 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build_lib/scheduler.py
+-rw-r--r--   0 jaime      (501) staff       (20)    11038 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build_lib/seqio.py
+-rw-r--r--   0 jaime      (501) staff       (20)     5978 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build_lib/sge.py
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.502870 ete3-3.1.3/ete3/tools/ete_build_lib/task/
+-rw-r--r--   0 jaime      (501) staff       (20)      648 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build_lib/task/__init__.py
+-rw-r--r--   0 jaime      (501) staff       (20)     3233 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build_lib/task/clustalo.py
+-rw-r--r--   0 jaime      (501) staff       (20)    22121 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build_lib/task/cog_creator.py
+-rw-r--r--   0 jaime      (501) staff       (20)    10555 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build_lib/task/cog_selector.py
+-rw-r--r--   0 jaime      (501) staff       (20)    11871 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build_lib/task/concat_alg.py
+-rw-r--r--   0 jaime      (501) staff       (20)     3039 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build_lib/task/dialigntx.py
+-rw-r--r--   0 jaime      (501) staff       (20)     1474 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build_lib/task/dummyalg.py
+-rw-r--r--   0 jaime      (501) staff       (20)     2783 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build_lib/task/dummytree.py
+-rw-r--r--   0 jaime      (501) staff       (20)     3670 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build_lib/task/fasttree.py
+-rw-r--r--   0 jaime      (501) staff       (20)     2908 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build_lib/task/iqtree.py
+-rw-r--r--   0 jaime      (501) staff       (20)     4092 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build_lib/task/jmodeltest.py
+-rw-r--r--   0 jaime      (501) staff       (20)     2976 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build_lib/task/mafft.py
+-rw-r--r--   0 jaime      (501) staff       (20)    10549 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build_lib/task/merger.py
+-rw-r--r--   0 jaime      (501) staff       (20)     9329 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build_lib/task/meta_aligner.py
+-rw-r--r--   0 jaime      (501) staff       (20)     3066 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build_lib/task/msf.py
+-rw-r--r--   0 jaime      (501) staff       (20)     2956 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build_lib/task/muscle.py
+-rw-r--r--   0 jaime      (501) staff       (20)     5739 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build_lib/task/phyml.py
+-rwxr-xr-x   0 jaime      (501) staff       (20)     2413 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build_lib/task/pmodeltest.py
+-rw-r--r--   0 jaime      (501) staff       (20)     6215 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build_lib/task/prottest.py
+-rw-r--r--   0 jaime      (501) staff       (20)     6445 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build_lib/task/prottest2.py
+-rw-r--r--   0 jaime      (501) staff       (20)    11401 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build_lib/task/raxml.py
+-rw-r--r--   0 jaime      (501) staff       (20)     1526 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build_lib/task/tcoffee.py
+-rw-r--r--   0 jaime      (501) staff       (20)     4158 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build_lib/task/trimal.py
+-rw-r--r--   0 jaime      (501) staff       (20)     4331 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build_lib/task/uhire.py
+-rw-r--r--   0 jaime      (501) staff       (20)    20613 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build_lib/utils.py
+-rw-r--r--   0 jaime      (501) staff       (20)    47320 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build_lib/validate.py
+-rw-r--r--   0 jaime      (501) staff       (20)     8342 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build_lib/visualize.py
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.506895 ete3-3.1.3/ete3/tools/ete_build_lib/workflow/
+-rw-r--r--   0 jaime      (501) staff       (20)     1445 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build_lib/workflow/__init__.py
+-rw-r--r--   0 jaime      (501) staff       (20)    25825 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build_lib/workflow/common.py
+-rw-r--r--   0 jaime      (501) staff       (20)    20533 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build_lib/workflow/genetree.py
+-rw-r--r--   0 jaime      (501) staff       (20)    12687 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_build_lib/workflow/supermatrix.py
+-rw-r--r--   0 jaime      (501) staff       (20)     8118 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_compare.py
+-rw-r--r--   0 jaime      (501) staff       (20)    42798 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_evol.py
+-rw-r--r--   0 jaime      (501) staff       (20)     1713 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_expand.py
+-rw-r--r--   0 jaime      (501) staff       (20)     2246 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_extract.py
+-rw-r--r--   0 jaime      (501) staff       (20)     2038 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_generate.py
+-rw-r--r--   0 jaime      (501) staff       (20)    15107 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_maptrees.py
+-rw-r--r--   0 jaime      (501) staff       (20)     4959 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_mod.py
+-rw-r--r--   0 jaime      (501) staff       (20)     8531 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_ncbiquery.py
+-rw-r--r--   0 jaime      (501) staff       (20)     2089 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_split.py
+-rw-r--r--   0 jaime      (501) staff       (20)     2344 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_upgrade_tools.py
+-rw-r--r--   0 jaime      (501) staff       (20)    24626 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/ete_view.py
+-rw-r--r--   0 jaime      (501) staff       (20)     1324 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/tools/utils.py
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.547027 ete3-3.1.3/ete3/treeview/
+-rw-r--r--   0 jaime      (501) staff       (20)     1553 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/__init__.py
+-rw-r--r--   0 jaime      (501) staff       (20)     4231 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/_about.py
+-rw-r--r--   0 jaime      (501) staff       (20)    15043 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/_mainwindow.py
+-rw-r--r--   0 jaime      (501) staff       (20)     2521 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/_open_newick.py
+-rw-r--r--   0 jaime      (501) staff       (20)     5120 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/_search_dialog.py
+-rw-r--r--   0 jaime      (501) staff       (20)     7271 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/_show_codeml.py
+-rw-r--r--   0 jaime      (501) staff       (20)     6196 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/_show_newick.py
+-rw-r--r--   0 jaime      (501) staff       (20)     2279 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/about.ui
+-rw-r--r--   0 jaime      (501) staff       (20)     1808 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/clean_search.png
+-rw-r--r--   0 jaime      (501) staff       (20)     4969 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/drawer.py
+-rw-r--r--   0 jaime      (501) staff       (20)      867 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/ete_icon.png
+-rw-r--r--   0 jaime      (501) staff       (20)     5756 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/ete_logo.png
+-rw-r--r--   0 jaime      (501) staff       (20)    10717 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/ete_qt4app.ui
+-rw-r--r--   0 jaime      (501) staff       (20)      760 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/ete_resources.qrc
+-rw-r--r--   0 jaime      (501) staff       (20)   114778 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/ete_resources_rc.py
+-rw-r--r--   0 jaime      (501) staff       (20)     1308 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/export_pdf.png
+-rw-r--r--   0 jaime      (501) staff       (20)    90930 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/faces.py
+-rw-r--r--   0 jaime      (501) staff       (20)      962 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/fileopen.png
+-rw-r--r--   0 jaime      (501) staff       (20)      751 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/filesave.png
+-rw-r--r--   0 jaime      (501) staff       (20)     1080 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/fit_region.png
+-rw-r--r--   0 jaime      (501) staff       (20)     1500 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/fit_tree.png
+-rw-r--r--   0 jaime      (501) staff       (20)      583 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/force_topo.png
+-rw-r--r--   0 jaime      (501) staff       (20)     4416 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/image_properties.ui
+-rw-r--r--   0 jaime      (501) staff       (20)     9590 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/layouts.py
+-rw-r--r--   0 jaime      (501) staff       (20)    28679 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/main.py
+-rw-r--r--   0 jaime      (501) staff       (20)    10462 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/node_gui_actions.py
+-rw-r--r--   0 jaime      (501) staff       (20)      773 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/open_newick.ui
+-rw-r--r--   0 jaime      (501) staff       (20)     5299 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/qt.py
+-rw-r--r--   0 jaime      (501) staff       (20)    15598 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/qt4_circular_render.py
+-rwxr-xr-x   0 jaime      (501) staff       (20)      351 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/qt4_compile_resources.sh
+-rw-r--r--   0 jaime      (501) staff       (20)    14711 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/qt4_face_render.py
+-rw-r--r--   0 jaime      (501) staff       (20)    35376 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/qt4_gui.py
+-rw-r--r--   0 jaime      (501) staff       (20)     3872 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/qt4_rect_render.py
+-rw-r--r--   0 jaime      (501) staff       (20)    44533 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/qt4_render.py
+-rw-r--r--   0 jaime      (501) staff       (20)     1639 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/search.png
+-rw-r--r--   0 jaime      (501) staff       (20)     4263 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/search_dialog.ui
+-rw-r--r--   0 jaime      (501) staff       (20)      454 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/show_dist.png
+-rw-r--r--   0 jaime      (501) staff       (20)      491 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/show_names.png
+-rw-r--r--   0 jaime      (501) staff       (20)      797 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/show_newick.png
+-rw-r--r--   0 jaime      (501) staff       (20)     5316 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/show_newick.ui
+-rw-r--r--   0 jaime      (501) staff       (20)      651 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/show_support.png
+-rw-r--r--   0 jaime      (501) staff       (20)    41790 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/svg_colors.py
+-rw-r--r--   0 jaime      (501) staff       (20)     2224 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/templates.py
+-rw-r--r--   0 jaime      (501) staff       (20)      904 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/x_expand.png
+-rw-r--r--   0 jaime      (501) staff       (20)      920 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/x_reduce.png
+-rw-r--r--   0 jaime      (501) staff       (20)      838 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/y_expand.png
+-rw-r--r--   0 jaime      (501) staff       (20)      887 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/y_reduce.png
+-rw-r--r--   0 jaime      (501) staff       (20)     1284 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/zoom_in.png
+-rw-r--r--   0 jaime      (501) staff       (20)     1241 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/treeview/zoom_out.png
+-rw-r--r--   0 jaime      (501) staff       (20)     7913 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/utils.py
+-rw-r--r--   0 jaime      (501) staff       (20)       73 2023-05-02 09:01:39.000000 ete3-3.1.3/ete3/version.py
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.548014 ete3-3.1.3/ete3/webplugin/
+-rw-r--r--   0 jaime      (501) staff       (20)     1445 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/webplugin/__init__.py
+-rwxr-xr-x   0 jaime      (501) staff       (20)    15146 2023-05-02 08:57:17.000000 ete3-3.1.3/ete3/webplugin/webapp.py
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.277490 ete3-3.1.3/ete3.egg-info/
+-rw-r--r--   0 jaime      (501) staff       (20)     2062 2023-05-02 09:36:15.000000 ete3-3.1.3/ete3.egg-info/PKG-INFO
+-rw-r--r--   0 jaime      (501) staff       (20)    27329 2023-05-02 09:36:15.000000 ete3-3.1.3/ete3.egg-info/SOURCES.txt
+-rw-r--r--   0 jaime      (501) staff       (20)        1 2023-05-02 09:36:15.000000 ete3-3.1.3/ete3.egg-info/dependency_links.txt
+-rw-r--r--   0 jaime      (501) staff       (20)       45 2023-05-02 09:36:15.000000 ete3-3.1.3/ete3.egg-info/entry_points.txt
+-rw-r--r--   0 jaime      (501) staff       (20)        5 2023-05-02 09:36:15.000000 ete3-3.1.3/ete3.egg-info/top_level.txt
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.267576 ete3-3.1.3/examples/
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.550514 ete3-3.1.3/examples/clustering/
+-rw-r--r--   0 jaime      (501) staff       (20)     2402 2022-02-23 15:57:28.000000 ete3-3.1.3/examples/clustering/bubbles_validation.py
+-rw-r--r--   0 jaime      (501) staff       (20)     1589 2022-02-23 15:57:28.000000 ete3-3.1.3/examples/clustering/cluster_visualization.py
+-rw-r--r--   0 jaime      (501) staff       (20)     3942 2022-02-23 15:57:28.000000 ete3-3.1.3/examples/clustering/clustering_tree.py
+-rw-r--r--   0 jaime      (501) staff       (20)    38844 2022-02-23 15:57:28.000000 ete3-3.1.3/examples/clustering/diauxic.array
+-rw-r--r--   0 jaime      (501) staff       (20)    15682 2022-02-23 15:57:28.000000 ete3-3.1.3/examples/clustering/diauxic.nw
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.555734 ete3-3.1.3/examples/evol/
+-rw-r--r--   0 jaime      (501) staff       (20)     1795 2022-02-23 15:57:28.000000 ete3-3.1.3/examples/evol/1_freeratio.py
+-rw-r--r--   0 jaime      (501) staff       (20)     2184 2022-02-23 15:57:28.000000 ete3-3.1.3/examples/evol/2_sites_model.py
+-rw-r--r--   0 jaime      (501) staff       (20)     2423 2022-02-23 15:57:28.000000 ete3-3.1.3/examples/evol/3_branchsite_test.py
+-rw-r--r--   0 jaime      (501) staff       (20)     2804 2022-02-23 15:57:28.000000 ete3-3.1.3/examples/evol/4_branch_models.py
+-rw-r--r--   0 jaime      (501) staff       (20)     1902 2022-02-23 15:57:28.000000 ete3-3.1.3/examples/evol/5_branchsite_cladetest.py
+-rw-r--r--   0 jaime      (501) staff       (20)     1312 2022-02-23 15:57:28.000000 ete3-3.1.3/examples/evol/6_ancestral_sequence.py
+-rw-r--r--   0 jaime      (501) staff       (20)      571 2022-02-23 15:57:28.000000 ete3-3.1.3/examples/evol/7_slr.py
+-rw-r--r--   0 jaime      (501) staff       (20)      295 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/README
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.263276 ete3-3.1.3/examples/evol/data/
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.556933 ete3-3.1.3/examples/evol/data/CladeModelCD/
+-rw-r--r--   0 jaime      (501) staff       (20)     7789 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/CladeModelCD/ECP_EDN_15.fasta
+-rw-r--r--   0 jaime      (501) staff       (20)      212 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/CladeModelCD/ECP_EDN_15.nw
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.558414 ete3-3.1.3/examples/evol/data/L_example/
+-rw-r--r--   0 jaime      (501) staff       (20)     1258 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/L_example/alignment_L_measuring_evol.fasta
+-rw-r--r--   0 jaime      (501) staff       (20)      130 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/L_example/measuring_L_tree.nw
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.559527 ete3-3.1.3/examples/evol/data/S_example/
+-rw-r--r--   0 jaime      (501) staff       (20)     1378 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/alignment_S_measuring_evol.fasta
+-rw-r--r--   0 jaime      (501) staff       (20)       72 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/measuring_S_tree.nw
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.262898 ete3-3.1.3/examples/evol/data/S_example/paml/
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.566258 ete3-3.1.3/examples/evol/data/S_example/paml/M1/
+-rw-r--r--   0 jaime      (501) staff       (20)      143 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/M1/2NG.dN
+-rw-r--r--   0 jaime      (501) staff       (20)      143 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/M1/2NG.dS
+-rw-r--r--   0 jaime      (501) staff       (20)      143 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/M1/2NG.t
+-rw-r--r--   0 jaime      (501) staff       (20)      254 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/M1/4fold.nuc
+-rw-r--r--   0 jaime      (501) staff       (20)     1112 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/M1/algn
+-rw-r--r--   0 jaime      (501) staff       (20)     4586 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/M1/lnf
+-rw-r--r--   0 jaime      (501) staff       (20)    12125 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/M1/out
+-rw-r--r--   0 jaime      (501) staff       (20)     3429 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/M1/rst
+-rw-r--r--   0 jaime      (501) staff       (20)       79 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/M1/rst1
+-rw-r--r--   0 jaime      (501) staff       (20)       11 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/M1/rub
+-rw-r--r--   0 jaime      (501) staff       (20)      595 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/M1/tmp.ctl
+-rw-r--r--   0 jaime      (501) staff       (20)       71 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/M1/tree
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.572345 ete3-3.1.3/examples/evol/data/S_example/paml/M2/
+-rw-r--r--   0 jaime      (501) staff       (20)      143 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/M2/2NG.dN
+-rw-r--r--   0 jaime      (501) staff       (20)      143 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/M2/2NG.dS
+-rw-r--r--   0 jaime      (501) staff       (20)      143 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/M2/2NG.t
+-rw-r--r--   0 jaime      (501) staff       (20)      254 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/M2/4fold.nuc
+-rw-r--r--   0 jaime      (501) staff       (20)     1112 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/M2/algn
+-rw-r--r--   0 jaime      (501) staff       (20)     4681 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/M2/lnf
+-rw-r--r--   0 jaime      (501) staff       (20)    12297 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/M2/out
+-rw-r--r--   0 jaime      (501) staff       (20)     9821 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/M2/rst
+-rw-r--r--   0 jaime      (501) staff       (20)       93 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/M2/rst1
+-rw-r--r--   0 jaime      (501) staff       (20)       11 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/M2/rub
+-rw-r--r--   0 jaime      (501) staff       (20)      591 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/M2/tmp.ctl
+-rw-r--r--   0 jaime      (501) staff       (20)       71 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/M2/tree
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.578399 ete3-3.1.3/examples/evol/data/S_example/paml/bsA/
+-rw-r--r--   0 jaime      (501) staff       (20)      143 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/bsA/2NG.dN
+-rw-r--r--   0 jaime      (501) staff       (20)      143 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/bsA/2NG.dS
+-rw-r--r--   0 jaime      (501) staff       (20)      143 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/bsA/2NG.t
+-rw-r--r--   0 jaime      (501) staff       (20)      254 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/bsA/4fold.nuc
+-rw-r--r--   0 jaime      (501) staff       (20)     1112 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/bsA/algn
+-rw-r--r--   0 jaime      (501) staff       (20)     4586 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/bsA/lnf
+-rw-r--r--   0 jaime      (501) staff       (20)    12965 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/bsA/out
+-rw-r--r--   0 jaime      (501) staff       (20)     8374 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/bsA/rst
+-rw-r--r--   0 jaime      (501) staff       (20)       91 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/bsA/rst1
+-rw-r--r--   0 jaime      (501) staff       (20)       11 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/bsA/rub
+-rw-r--r--   0 jaime      (501) staff       (20)      600 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/bsA/tmp.ctl
+-rw-r--r--   0 jaime      (501) staff       (20)       74 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/bsA/tree
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.583510 ete3-3.1.3/examples/evol/data/S_example/paml/bsA1/
+-rw-r--r--   0 jaime      (501) staff       (20)      143 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/bsA1/2NG.dN
+-rw-r--r--   0 jaime      (501) staff       (20)      143 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/bsA1/2NG.dS
+-rw-r--r--   0 jaime      (501) staff       (20)      143 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/bsA1/2NG.t
+-rw-r--r--   0 jaime      (501) staff       (20)      254 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/bsA1/4fold.nuc
+-rw-r--r--   0 jaime      (501) staff       (20)     1112 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/bsA1/algn
+-rw-r--r--   0 jaime      (501) staff       (20)     4586 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/bsA1/lnf
+-rw-r--r--   0 jaime      (501) staff       (20)    11769 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/bsA1/out
+-rw-r--r--   0 jaime      (501) staff       (20)     4345 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/bsA1/rst
+-rw-r--r--   0 jaime      (501) staff       (20)       85 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/bsA1/rst1
+-rw-r--r--   0 jaime      (501) staff       (20)       11 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/bsA1/rub
+-rw-r--r--   0 jaime      (501) staff       (20)      598 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/bsA1/tmp.ctl
+-rw-r--r--   0 jaime      (501) staff       (20)       74 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/bsA1/tree
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.589855 ete3-3.1.3/examples/evol/data/S_example/paml/fb/
+-rw-r--r--   0 jaime      (501) staff       (20)      143 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/fb/2NG.dN
+-rw-r--r--   0 jaime      (501) staff       (20)      143 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/fb/2NG.dS
+-rw-r--r--   0 jaime      (501) staff       (20)      143 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/fb/2NG.t
+-rw-r--r--   0 jaime      (501) staff       (20)      254 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/fb/4fold.nuc
+-rw-r--r--   0 jaime      (501) staff       (20)     1112 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/fb/algn
+-rw-r--r--   0 jaime      (501) staff       (20)     4586 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/fb/lnf
+-rw-r--r--   0 jaime      (501) staff       (20)    12631 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/fb/out
+-rw-r--r--   0 jaime      (501) staff       (20)   217002 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/fb/rst
+-rw-r--r--   0 jaime      (501) staff       (20)     4657 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/fb/rst1
+-rw-r--r--   0 jaime      (501) staff       (20)       11 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/fb/rub
+-rw-r--r--   0 jaime      (501) staff       (20)      601 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/fb/tmp.ctl
+-rw-r--r--   0 jaime      (501) staff       (20)       71 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/S_example/paml/fb/tree
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.263474 ete3-3.1.3/examples/evol/data/protamine/
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.591141 ete3-3.1.3/examples/evol/data/protamine/PRM1/
+-rw-r--r--   0 jaime      (501) staff       (20)    21140 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/alignments.fasta_ali
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.265270 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.601158 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M0/
+-rw-r--r--   0 jaime      (501) staff       (20)    40255 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M0/2NG.dN
+-rw-r--r--   0 jaime      (501) staff       (20)    40255 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M0/2NG.dS
+-rw-r--r--   0 jaime      (501) staff       (20)    40255 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M0/2NG.t
+-rw-r--r--   0 jaime      (501) staff       (20)     2064 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M0/4fold.nuc
+-rw-r--r--   0 jaime      (501) staff       (20)    21148 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M0/algn
+-rw-r--r--   0 jaime      (501) staff       (20)    54234 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M0/lnf
+-rw-r--r--   0 jaime      (501) staff       (20)   265562 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M0/out
+-rw-r--r--   0 jaime      (501) staff       (20)       59 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M0/rst
+-rw-r--r--   0 jaime      (501) staff       (20)     1211 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M0/rst1
+-rw-r--r--   0 jaime      (501) staff       (20)       11 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M0/rub
+-rw-r--r--   0 jaime      (501) staff       (20)      424 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M0/tmp.ctl
+-rw-r--r--   0 jaime      (501) staff       (20)     2026 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M0/tree
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.608415 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M1/
+-rw-r--r--   0 jaime      (501) staff       (20)        0 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M1/2NG.dN
+-rw-r--r--   0 jaime      (501) staff       (20)        0 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M1/2NG.dS
+-rw-r--r--   0 jaime      (501) staff       (20)        0 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M1/2NG.t
+-rw-r--r--   0 jaime      (501) staff       (20)     2064 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M1/4fold.nuc
+-rw-r--r--   0 jaime      (501) staff       (20)   153567 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M1/M1.out
+-rw-r--r--   0 jaime      (501) staff       (20)    21148 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M1/algn
+-rw-r--r--   0 jaime      (501) staff       (20)    54234 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M1/lnf
+-rw-r--r--   0 jaime      (501) staff       (20)     2716 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M1/rst
+-rw-r--r--   0 jaime      (501) staff       (20)        1 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M1/rst1
+-rw-r--r--   0 jaime      (501) staff       (20)       11 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M1/rub
+-rw-r--r--   0 jaime      (501) staff       (20)      428 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M1/tmp.ctl
+-rw-r--r--   0 jaime      (501) staff       (20)     2027 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M1/tree
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.615199 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M2/
+-rw-r--r--   0 jaime      (501) staff       (20)        0 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M2/2NG.dN
+-rw-r--r--   0 jaime      (501) staff       (20)        0 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M2/2NG.dS
+-rw-r--r--   0 jaime      (501) staff       (20)        0 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M2/2NG.t
+-rw-r--r--   0 jaime      (501) staff       (20)     2064 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M2/4fold.nuc
+-rw-r--r--   0 jaime      (501) staff       (20)   155576 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M2/M2.out
+-rw-r--r--   0 jaime      (501) staff       (20)    21148 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M2/algn
+-rw-r--r--   0 jaime      (501) staff       (20)    54234 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M2/lnf
+-rw-r--r--   0 jaime      (501) staff       (20)     8072 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M2/rst
+-rw-r--r--   0 jaime      (501) staff       (20)        1 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M2/rst1
+-rw-r--r--   0 jaime      (501) staff       (20)       11 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M2/rub
+-rw-r--r--   0 jaime      (501) staff       (20)      428 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M2/tmp.ctl
+-rw-r--r--   0 jaime      (501) staff       (20)     2027 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M2/tree
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.622378 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M7/
+-rw-r--r--   0 jaime      (501) staff       (20)        0 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M7/2NG.dN
+-rw-r--r--   0 jaime      (501) staff       (20)        0 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M7/2NG.dS
+-rw-r--r--   0 jaime      (501) staff       (20)        0 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M7/2NG.t
+-rw-r--r--   0 jaime      (501) staff       (20)     2064 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M7/4fold.nuc
+-rw-r--r--   0 jaime      (501) staff       (20)   153770 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M7/M7.out
+-rw-r--r--   0 jaime      (501) staff       (20)    21148 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M7/algn
+-rw-r--r--   0 jaime      (501) staff       (20)    54234 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M7/lnf
+-rw-r--r--   0 jaime      (501) staff       (20)     7022 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M7/rst
+-rw-r--r--   0 jaime      (501) staff       (20)        1 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M7/rst1
+-rw-r--r--   0 jaime      (501) staff       (20)       11 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M7/rub
+-rw-r--r--   0 jaime      (501) staff       (20)      428 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M7/tmp.ctl
+-rw-r--r--   0 jaime      (501) staff       (20)     2027 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M7/tree
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.630013 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M8/
+-rw-r--r--   0 jaime      (501) staff       (20)        0 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M8/2NG.dN
+-rw-r--r--   0 jaime      (501) staff       (20)        0 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M8/2NG.dS
+-rw-r--r--   0 jaime      (501) staff       (20)        0 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M8/2NG.t
+-rw-r--r--   0 jaime      (501) staff       (20)     2064 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M8/4fold.nuc
+-rw-r--r--   0 jaime      (501) staff       (20)   155459 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M8/M8.out
+-rw-r--r--   0 jaime      (501) staff       (20)    21148 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M8/algn
+-rw-r--r--   0 jaime      (501) staff       (20)    54234 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M8/lnf
+-rw-r--r--   0 jaime      (501) staff       (20)    16616 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M8/rst
+-rw-r--r--   0 jaime      (501) staff       (20)        1 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M8/rst1
+-rw-r--r--   0 jaime      (501) staff       (20)       11 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M8/rub
+-rw-r--r--   0 jaime      (501) staff       (20)      428 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M8/tmp.ctl
+-rw-r--r--   0 jaime      (501) staff       (20)     2027 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M8/tree
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.637254 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/fb/
+-rw-r--r--   0 jaime      (501) staff       (20)        0 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/fb/2NG.dN
+-rw-r--r--   0 jaime      (501) staff       (20)        0 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/fb/2NG.dS
+-rw-r--r--   0 jaime      (501) staff       (20)        0 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/fb/2NG.t
+-rw-r--r--   0 jaime      (501) staff       (20)     2064 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/fb/4fold.nuc
+-rw-r--r--   0 jaime      (501) staff       (20)    21148 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/fb/algn
+-rw-r--r--   0 jaime      (501) staff       (20)   169966 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/fb/fb.out
+-rw-r--r--   0 jaime      (501) staff       (20)    54234 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/fb/lnf
+-rw-r--r--   0 jaime      (501) staff       (20)       59 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/fb/rst.fb
+-rw-r--r--   0 jaime      (501) staff       (20)        1 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/fb/rst1
+-rw-r--r--   0 jaime      (501) staff       (20)       11 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/fb/rub
+-rw-r--r--   0 jaime      (501) staff       (20)      478 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/fb/tmp.ctl
+-rw-r--r--   0 jaime      (501) staff       (20)     2027 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/fb/tree
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.645472 ete3-3.1.3/examples/evol/data/protamine/PRM1/slr/
+-rw-r--r--   0 jaime      (501) staff       (20)        0 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/slr/2NG.dN
+-rw-r--r--   0 jaime      (501) staff       (20)        0 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/slr/2NG.dS
+-rw-r--r--   0 jaime      (501) staff       (20)        0 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/slr/2NG.t
+-rw-r--r--   0 jaime      (501) staff       (20)     2064 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/slr/4fold.nuc
+-rw-r--r--   0 jaime      (501) staff       (20)    21148 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/slr/algn
+-rw-r--r--   0 jaime      (501) staff       (20)   169966 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/slr/fb.out
+-rw-r--r--   0 jaime      (501) staff       (20)    54234 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/slr/lnf
+-rw-r--r--   0 jaime      (501) staff       (20)       59 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/slr/rst.fb
+-rw-r--r--   0 jaime      (501) staff       (20)        1 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/slr/rst1
+-rw-r--r--   0 jaime      (501) staff       (20)       11 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/slr/rub
+-rw-r--r--   0 jaime      (501) staff       (20)       83 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/slr/slr.ctl
+-rw-r--r--   0 jaime      (501) staff       (20)      478 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/slr/tmp.ctl
+-rw-r--r--   0 jaime      (501) staff       (20)     2027 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/slr/tree
+-rw-r--r--   0 jaime      (501) staff       (20)      483 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/slr/tree.slr
+-rw-r--r--   0 jaime      (501) staff       (20)     2026 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/evol/data/protamine/PRM1/tree.nw
+-rw-r--r--   0 jaime      (501) staff       (20)     7098 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/evol/measuring_evolution_trees.py
+-rw-r--r--   0 jaime      (501) staff       (20)      869 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/evol/test_hist.py
+-rw-r--r--   0 jaime      (501) staff       (20)     1456 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/evol/test_protamine.py
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.663452 ete3-3.1.3/examples/general/
+-rw-r--r--   0 jaime      (501) staff       (20)     2124 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/general/add_features.py
+-rw-r--r--   0 jaime      (501) staff       (20)      749 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/general/byoperand_search.py
+-rw-r--r--   0 jaime      (501) staff       (20)     1115 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/general/chimp.png
+-rw-r--r--   0 jaime      (501) staff       (20)     1887 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/general/copy_and_paste_trees.py
+-rw-r--r--   0 jaime      (501) staff       (20)     1735 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/general/create_trees_from_scratch.py
+-rw-r--r--   0 jaime      (501) staff       (20)      819 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/general/custom_search.py
+-rw-r--r--   0 jaime      (501) staff       (20)      541 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/general/custom_tree_traversing.py
+-rw-r--r--   0 jaime      (501) staff       (20)     4971 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/general/custom_tree_visualization.py
+-rw-r--r--   0 jaime      (501) staff       (20)     4130 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/general/dog.png
+-rw-r--r--   0 jaime      (501) staff       (20)     2767 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/general/fish.png
+-rw-r--r--   0 jaime      (501) staff       (20)     3971 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/general/fly.png
+-rw-r--r--   0 jaime      (501) staff       (20)      726 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/general/genes_tree.nh
+-rw-r--r--   0 jaime      (501) staff       (20)     1176 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/general/get_common_ancestor.py
+-rw-r--r--   0 jaime      (501) staff       (20)     2464 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/general/get_distances_between_nodes.py
+-rw-r--r--   0 jaime      (501) staff       (20)     3212 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/general/get_midpoint_outgroup.py
+-rw-r--r--   0 jaime      (501) staff       (20)     1036 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/general/getting_leaves.py
+-rw-r--r--   0 jaime      (501) staff       (20)     3503 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/general/human.png
+-rw-r--r--   0 jaime      (501) staff       (20)      687 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/general/iterators.py
+-rw-r--r--   0 jaime      (501) staff       (20)      589 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/general/label_nodes.py
+-rw-r--r--   0 jaime      (501) staff       (20)     1324 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/general/mouse.png
+-rw-r--r--   0 jaime      (501) staff       (20)     2067 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/general/nhx_format.py
+-rw-r--r--   0 jaime      (501) staff       (20)     1228 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/general/prune_tree.py
+-rw-r--r--   0 jaime      (501) staff       (20)   103821 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/general/random_tree.png
+-rw-r--r--   0 jaime      (501) staff       (20)      420 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/general/read_newick.py
+-rw-r--r--   0 jaime      (501) staff       (20)     2768 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/general/remove_and_delete_nodes.py
+-rw-r--r--   0 jaime      (501) staff       (20)      517 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/general/render_tree_images.py
+-rw-r--r--   0 jaime      (501) staff       (20)     1964 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/general/rooting_subtrees.py
+-rw-r--r--   0 jaime      (501) staff       (20)     1652 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/general/rooting_trees.py
+-rw-r--r--   0 jaime      (501) staff       (20)      517 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/general/search_nodes.py
+-rw-r--r--   0 jaime      (501) staff       (20)      710 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/general/tree_basis.py
+-rw-r--r--   0 jaime      (501) staff       (20)     1044 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/general/tree_traverse.py
+-rw-r--r--   0 jaime      (501) staff       (20)      346 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/general/write_newick.py
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.669280 ete3-3.1.3/examples/nexml/
+-rw-r--r--   0 jaime      (501) staff       (20)     3771 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/nexml/02_dogfish_no_taxrefs.xml
+-rw-r--r--   0 jaime      (501) staff       (20)    23870 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/nexml/characters.xml
+-rw-r--r--   0 jaime      (501) staff       (20)     2058 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/nexml/meta_taxa.xml
+-rw-r--r--   0 jaime      (501) staff       (20)      329 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/nexml/nexml.xml
+-rw-r--r--   0 jaime      (501) staff       (20)     1029 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/nexml/nexml_annotated_trees.py
+-rw-r--r--   0 jaime      (501) staff       (20)     1006 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/nexml/nexml_from_scratch.py
+-rw-r--r--   0 jaime      (501) staff       (20)     2129 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/nexml/nexml_parser.py
+-rw-r--r--   0 jaime      (501) staff       (20)     1960 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/nexml/phenoscape.xml
+-rw-r--r--   0 jaime      (501) staff       (20)     3162 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/nexml/taxa.xml
+-rw-r--r--   0 jaime      (501) staff       (20)    14324 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/nexml/timetree.xml
+-rw-r--r--   0 jaime      (501) staff       (20)     3531 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/nexml/tolweb.xml
+-rw-r--r--   0 jaime      (501) staff       (20)     5195 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/nexml/trees.xml
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.672318 ete3-3.1.3/examples/phylogenies/
+-rw-r--r--   0 jaime      (501) staff       (20)     2863 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/phylogenies/dating_evolutionary_events.py
+-rw-r--r--   0 jaime      (501) staff       (20)     3112 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/phylogenies/link_sequences_to_phylogenies.py
+-rw-r--r--   0 jaime      (501) staff       (20)     3020 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/phylogenies/orthology_and_paralogy_prediction.py
+-rw-r--r--   0 jaime      (501) staff       (20)    48918 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/phylogenies/phylotree.png
+-rw-r--r--   0 jaime      (501) staff       (20)     1430 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/phylogenies/phylotree_visualization.py
+-rw-r--r--   0 jaime      (501) staff       (20)     3204 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/phylogenies/species_aware_phylogenies.py
+-rw-r--r--   0 jaime      (501) staff       (20)     3426 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/phylogenies/tree_reconciliation.py
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.679437 ete3-3.1.3/examples/phyloxml/
+-rw-r--r--   0 jaime      (501) staff       (20)    38619 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/phyloxml/apaf.xml
+-rw-r--r--   0 jaime      (501) staff       (20)   113544 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/phyloxml/bcl_2.xml
+-rw-r--r--   0 jaime      (501) staff       (20)     2062 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/phyloxml/example1.xml
+-rw-r--r--   0 jaime      (501) staff       (20)     1969 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/phyloxml/example2.xml
+-rw-r--r--   0 jaime      (501) staff       (20)    14908 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/phyloxml/example3.xml
+-rw-r--r--   0 jaime      (501) staff       (20)     7233 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/phyloxml/multiple_supports.xml
+-rw-r--r--   0 jaime      (501) staff       (20)   645989 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/phyloxml/ncbi_taxonomy_metazoa.xml.bz2
+-rw-r--r--   0 jaime      (501) staff       (20)    15291 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/phyloxml/phyloxml_examples.xml
+-rw-r--r--   0 jaime      (501) staff       (20)     3201 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/phyloxml/phyloxml_from_scratch.py
+-rw-r--r--   0 jaime      (501) staff       (20)      651 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/phyloxml/phyloxml_parser.py
+-rw-r--r--   0 jaime      (501) staff       (20)   564207 2023-05-02 08:57:17.000000 ete3-3.1.3/examples/phyloxml/tol_life_on_earth.xml.bz2
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.694847 ete3-3.1.3/examples/treeview/
+-rwxr-xr-x   0 jaime      (501) staff       (20)     1433 2023-05-01 16:21:57.000000 ete3-3.1.3/examples/treeview/barchart_and_piechart_faces.py
+-rw-r--r--   0 jaime      (501) staff       (20)    33022 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/treeview/barcharts.png
+-rw-r--r--   0 jaime      (501) staff       (20)   112579 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/treeview/bubble_map.png
+-rwxr-xr-x   0 jaime      (501) staff       (20)     1355 2023-05-01 16:21:57.000000 ete3-3.1.3/examples/treeview/bubble_map.py
+-rwxr-xr-x   0 jaime      (501) staff       (20)     1626 2023-05-01 16:21:57.000000 ete3-3.1.3/examples/treeview/face_grid.py
+-rwxr-xr-x   0 jaime      (501) staff       (20)     4012 2023-05-01 16:21:57.000000 ete3-3.1.3/examples/treeview/face_positions.py
+-rwxr-xr-x   0 jaime      (501) staff       (20)      800 2023-05-01 16:21:57.000000 ete3-3.1.3/examples/treeview/face_rotation.py
+-rw-r--r--   0 jaime      (501) staff       (20)   289006 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/treeview/float_piechart.png
+-rwxr-xr-x   0 jaime      (501) staff       (20)      840 2023-05-01 16:21:57.000000 ete3-3.1.3/examples/treeview/floating_piecharts.py
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.699507 ete3-3.1.3/examples/treeview/img_faces/
+-rw-r--r--   0 jaime      (501) staff       (20)     1115 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/treeview/img_faces/chimp.png
+-rw-r--r--   0 jaime      (501) staff       (20)     4130 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/treeview/img_faces/dog.png
+-rw-r--r--   0 jaime      (501) staff       (20)     2767 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/treeview/img_faces/fish.png
+-rw-r--r--   0 jaime      (501) staff       (20)     3971 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/treeview/img_faces/fly.png
+-rw-r--r--   0 jaime      (501) staff       (20)     3503 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/treeview/img_faces/human.png
+-rw-r--r--   0 jaime      (501) staff       (20)    60235 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/treeview/img_faces/img_faces.png
+-rw-r--r--   0 jaime      (501) staff       (20)     5156 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/treeview/img_faces/img_faces.py
+-rw-r--r--   0 jaime      (501) staff       (20)     1324 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/treeview/img_faces/mouse.png
+-rw-r--r--   0 jaime      (501) staff       (20)    35247 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/treeview/item_faces.png
+-rwxr-xr-x   0 jaime      (501) staff       (20)     4141 2023-05-01 16:21:57.000000 ete3-3.1.3/examples/treeview/item_faces.py
+-rw-r--r--   0 jaime      (501) staff       (20)    10961 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/treeview/new_seq_face.py
+-rw-r--r--   0 jaime      (501) staff       (20)    51805 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/treeview/node_background.png
+-rwxr-xr-x   0 jaime      (501) staff       (20)     1196 2023-05-01 16:21:57.000000 ete3-3.1.3/examples/treeview/node_background.py
+-rw-r--r--   0 jaime      (501) staff       (20)    10303 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/treeview/node_style.png
+-rwxr-xr-x   0 jaime      (501) staff       (20)     2039 2023-05-01 16:21:57.000000 ete3-3.1.3/examples/treeview/node_style.py
+-rwxr-xr-x   0 jaime      (501) staff       (20)     3818 2023-05-01 16:21:57.000000 ete3-3.1.3/examples/treeview/random_draw.py
+-rw-r--r--   0 jaime      (501) staff       (20)    33631 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/treeview/rotated_faces.png
+-rw-r--r--   0 jaime      (501) staff       (20)    16453 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/treeview/seq_motif_faces.png
+-rwxr-xr-x   0 jaime      (501) staff       (20)     3714 2023-05-01 16:21:57.000000 ete3-3.1.3/examples/treeview/seq_motif_faces.py
+-rw-r--r--   0 jaime      (501) staff       (20)    97444 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/treeview/seqmotif.png
+-rw-r--r--   0 jaime      (501) staff       (20)   118000 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/treeview/tree_faces.png
+-rwxr-xr-x   0 jaime      (501) staff       (20)     1357 2023-05-01 16:21:57.000000 ete3-3.1.3/examples/treeview/tree_faces.py
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.706185 ete3-3.1.3/examples/webplugin/
+-rw-r--r--   0 jaime      (501) staff       (20)     1238 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/webplugin/README
+-rw-r--r--   0 jaime      (501) staff       (20)      735 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/webplugin/close.png
+-rw-r--r--   0 jaime      (501) staff       (20)     1637 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/webplugin/ete.css
+-rw-r--r--   0 jaime      (501) staff       (20)     2252 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/webplugin/ete.js
+-rw-r--r--   0 jaime      (501) staff       (20)     1661 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/webplugin/icon_attachment.png
+-rw-r--r--   0 jaime      (501) staff       (20)     1467 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/webplugin/icon_cancel_search.png
+-rw-r--r--   0 jaime      (501) staff       (20)     1481 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/webplugin/icon_search.png
+-rw-r--r--   0 jaime      (501) staff       (20)     1143 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/webplugin/icon_tools.png
+-rw-r--r--   0 jaime      (501) staff       (20)    72174 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/webplugin/jquery-1.4.2.min.js
+-rw-r--r--   0 jaime      (501) staff       (20)    31079 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/webplugin/jquery-ui-1.8.4.custom.min.js
+-rw-r--r--   0 jaime      (501) staff       (20)     7364 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/webplugin/loader.gif
+-rw-r--r--   0 jaime      (501) staff       (20)     1947 2022-02-23 15:57:29.000000 ete3-3.1.3/examples/webplugin/webplugin_example.html
+drwxr-xr-x   0 jaime      (501) staff       (20)        0 2023-05-02 09:36:15.706838 ete3-3.1.3/examples/webplugin/wsgi/
+-rwxr-xr-x   0 jaime      (501) staff       (20)    22378 2023-05-01 16:21:57.000000 ete3-3.1.3/examples/webplugin/wsgi/webplugin_example.py
+-rwxr-xr-x   0 jaime      (501) staff       (20)    10376 2023-05-01 16:21:57.000000 ete3-3.1.3/ez_setup.py
+-rw-r--r--   0 jaime      (501) staff       (20)       38 2023-05-02 09:36:15.708244 ete3-3.1.3/setup.cfg
+-rwxr-xr-x   0 jaime      (501) staff       (20)     3893 2023-05-02 09:36:02.000000 ete3-3.1.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ete3-3.1.2/THANKS.rst` & `ete3-3.1.3/THANKS.rst`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/PKG-INFO` & `ete3-3.1.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,20 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: ete3
-Version: 3.1.2
+Version: 3.1.3
 Summary: A Python Environment for (phylogenetic) Tree Exploration
 Home-page: http://etetoolkit.org
+Download-URL: http://etetoolkit.org/static/releases/ete3/
 Author: Jaime Huerta-Cepas
 Author-email: jhcepas@gmail.com
 Maintainer: Jaime Huerta-Cepas
 Maintainer-email: huerta@embl.de
 License: GPLv3
-Download-URL: http://etetoolkit.org/static/releases/ete3/
-Description: 
-        The Environment for Tree Exploration (ETE) is a Python programming
-        toolkit that assists in the recontruction, manipulation, analysis and
-        visualization of phylogenetic trees (although clustering trees or any
-        other tree-like data structure are also supported).
-        
-        ETE is currently developed as a tool for researchers working in
-        phylogenetics and genomics. If you use ETE for a published work,
-        please cite:
-        
-        ::
-        
-           Jaime Huerta-Cepas, François Serra and Peer Bork. "ETE 3: Reconstruction,
-           analysis and visualization of phylogenomic data."  Mol Biol Evol (2016) doi:
-           10.1093/molbev/msw046
-        
-        Visit http://etetoolkit.org for more info.
-        
+Project-URL: Documentation, http://etetoolkit.org/docs/latest/tutorial/index.html
+Project-URL: Source, https://github.com/etetoolkit/ete
 Keywords: tree,tree reconstruction,tree visualization,tree comparison,phylogeny,phylogenetics,phylogenomics
 Platform: OS Independent
 Classifier: Development Status :: 6 - Mature
 Classifier: Environment :: Console
 Classifier: Environment :: X11 Applications :: Qt
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
@@ -42,7 +26,26 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires: six
 Provides: ete3
+License-File: LICENSE
+
+
+The Environment for Tree Exploration (ETE) is a Python programming
+toolkit that assists in the recontruction, manipulation, analysis and
+visualization of phylogenetic trees (although clustering trees or any
+other tree-like data structure are also supported).
+
+ETE is currently developed as a tool for researchers working in
+phylogenetics and genomics. If you use ETE for a published work,
+please cite:
+
+::
+
+   Jaime Huerta-Cepas, François Serra and Peer Bork. "ETE 3: Reconstruction,
+   analysis and visualization of phylogenomic data."  Mol Biol Evol (2016) doi:
+   10.1093/molbev/msw046
+
+Visit http://etetoolkit.org for more info.
```

### Comparing `ete3-3.1.2/examples/clustering/clustering_tree.py` & `ete3-3.1.3/examples/clustering/clustering_tree.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/clustering/diauxic.array` & `ete3-3.1.3/examples/clustering/diauxic.array`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/clustering/diauxic.nw` & `ete3-3.1.3/examples/clustering/diauxic.nw`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/clustering/cluster_visualization.py` & `ete3-3.1.3/examples/clustering/cluster_visualization.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/clustering/bubbles_validation.py` & `ete3-3.1.3/examples/clustering/bubbles_validation.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/nexml/nexml_from_scratch.py` & `ete3-3.1.3/examples/nexml/nexml_from_scratch.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/nexml/tolweb.xml` & `ete3-3.1.3/examples/nexml/tolweb.xml`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/nexml/nexml_annotated_trees.py` & `ete3-3.1.3/examples/nexml/nexml_annotated_trees.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/nexml/taxa.xml` & `ete3-3.1.3/examples/nexml/taxa.xml`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/nexml/trees.xml` & `ete3-3.1.3/examples/nexml/trees.xml`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/nexml/nexml_parser.py` & `ete3-3.1.3/examples/nexml/nexml_parser.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/nexml/characters.xml` & `ete3-3.1.3/examples/nexml/characters.xml`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/nexml/phenoscape.xml` & `ete3-3.1.3/examples/nexml/phenoscape.xml`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/nexml/timetree.xml` & `ete3-3.1.3/examples/nexml/timetree.xml`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/nexml/02_dogfish_no_taxrefs.xml` & `ete3-3.1.3/examples/nexml/02_dogfish_no_taxrefs.xml`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/nexml/meta_taxa.xml` & `ete3-3.1.3/examples/nexml/meta_taxa.xml`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/general/fish.png` & `ete3-3.1.3/ete3/test/test_treeview/fish.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/general/genes_tree.nh` & `ete3-3.1.3/examples/general/genes_tree.nh`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/general/get_midpoint_outgroup.py` & `ete3-3.1.3/examples/general/get_midpoint_outgroup.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/general/custom_tree_visualization.py` & `ete3-3.1.3/examples/general/custom_tree_visualization.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/general/rooting_trees.py` & `ete3-3.1.3/examples/general/rooting_trees.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/general/chimp.png` & `ete3-3.1.3/ete3/test/test_treeview/chimp.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/general/dog.png` & `ete3-3.1.3/ete3/test/test_treeview/dog.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/general/human.png` & `ete3-3.1.3/ete3/test/test_treeview/human.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/general/tree_traverse.py` & `ete3-3.1.3/examples/general/tree_traverse.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/general/custom_tree_traversing.py` & `ete3-3.1.3/examples/general/custom_tree_traversing.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/general/getting_leaves.py` & `ete3-3.1.3/examples/general/getting_leaves.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/general/render_tree_images.py` & `ete3-3.1.3/examples/general/render_tree_images.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/general/remove_and_delete_nodes.py` & `ete3-3.1.3/examples/general/remove_and_delete_nodes.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/general/get_distances_between_nodes.py` & `ete3-3.1.3/examples/general/get_distances_between_nodes.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/general/tree_basis.py` & `ete3-3.1.3/examples/general/tree_basis.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/general/prune_tree.py` & `ete3-3.1.3/examples/general/prune_tree.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/general/get_common_ancestor.py` & `ete3-3.1.3/examples/general/get_common_ancestor.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/general/add_features.py` & `ete3-3.1.3/examples/general/add_features.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/general/label_nodes.py` & `ete3-3.1.3/examples/general/label_nodes.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/general/copy_and_paste_trees.py` & `ete3-3.1.3/examples/general/copy_and_paste_trees.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/general/iterators.py` & `ete3-3.1.3/examples/general/iterators.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/general/fly.png` & `ete3-3.1.3/ete3/test/test_treeview/fly.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/general/rooting_subtrees.py` & `ete3-3.1.3/examples/general/rooting_subtrees.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/general/byoperand_search.py` & `ete3-3.1.3/examples/general/byoperand_search.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/general/create_trees_from_scratch.py` & `ete3-3.1.3/examples/general/create_trees_from_scratch.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/general/random_tree.png` & `ete3-3.1.3/examples/general/random_tree.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/general/mouse.png` & `ete3-3.1.3/ete3/test/test_treeview/mouse.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/general/search_nodes.py` & `ete3-3.1.3/examples/general/search_nodes.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/general/nhx_format.py` & `ete3-3.1.3/examples/general/nhx_format.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/general/custom_search.py` & `ete3-3.1.3/examples/general/custom_search.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/test_hist.py` & `ete3-3.1.3/examples/evol/test_hist.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/7_slr.py` & `ete3-3.1.3/examples/evol/7_slr.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/2_sites_model.py` & `ete3-3.1.3/examples/evol/2_sites_model.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/L_example/alignment_L_measuring_evol.fasta` & `ete3-3.1.3/ete3/test/ete_evol_data/L_example/alignment_L_measuring_evol.fasta`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/S_example/alignment_S_measuring_evol.fasta` & `ete3-3.1.3/ete3/test/ete_evol_data/S_example/ali.fasta`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/S_example/paml/M1/out` & `ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/M1/out`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/S_example/paml/M1/tmp.ctl` & `ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/M1/tmp.ctl`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/S_example/paml/M1/lnf` & `ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/M1/lnf`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/S_example/paml/M1/rst` & `ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/M1/rst`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/S_example/paml/M1/algn` & `ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/M1/algn`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/S_example/paml/fb/out` & `ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/fb/out`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/S_example/paml/fb/rst1` & `ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/fb/rst1`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/S_example/paml/fb/tmp.ctl` & `ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/fb/tmp.ctl`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/S_example/paml/fb/lnf` & `ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/fb/lnf`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/S_example/paml/fb/rst` & `ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/fb/rst`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/S_example/paml/fb/algn` & `ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/M2/algn`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/S_example/paml/bsA1/out` & `ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/bsA1/out`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/S_example/paml/bsA1/tmp.ctl` & `ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/bsA1/tmp.ctl`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/S_example/paml/bsA1/lnf` & `ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/bsA1/lnf`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/S_example/paml/bsA1/rst` & `ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/bsA1/rst`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/S_example/paml/bsA1/algn` & `ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/bsA/algn`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/S_example/paml/M2/out` & `ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/M2/out`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/S_example/paml/M2/tmp.ctl` & `ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/M2/tmp.ctl`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/S_example/paml/M2/lnf` & `ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/M2/lnf`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/S_example/paml/M2/rst` & `ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/M2/rst`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/S_example/paml/M2/algn` & `ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/bsA1/algn`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/S_example/paml/bsA/out` & `ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/bsA/out`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/S_example/paml/bsA/tmp.ctl` & `ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/bsA/tmp.ctl`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/S_example/paml/bsA/lnf` & `ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/bsA/lnf`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/S_example/paml/bsA/rst` & `ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/bsA/rst`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/S_example/paml/bsA/algn` & `ete3-3.1.3/ete3/test/ete_evol_data/S_example/paml/fb/algn`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/CladeModelCD/ECP_EDN_15.fasta` & `ete3-3.1.3/ete3/test/ete_evol_data/CladeModelCD/ECP_EDN_15.fasta`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/protamine/PRM1/slr/tree` & `ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M1/tree`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/protamine/PRM1/slr/fb.out` & `ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/fb/fb.out`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/protamine/PRM1/slr/4fold.nuc` & `ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M1/4fold.nuc`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/protamine/PRM1/slr/lnf` & `ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/fb/lnf`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/protamine/PRM1/slr/algn` & `ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M1/algn`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/protamine/PRM1/tree.nw` & `ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/tree.nw`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M0/2NG.t` & `ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M0/2NG.t`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M0/tree` & `ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M0/tree`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M0/out` & `ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M0/out`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M0/4fold.nuc` & `ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M0/4fold.nuc`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M0/2NG.dS` & `ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M0/2NG.dS`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M0/rst1` & `ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M0/rst1`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M0/lnf` & `ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M0/lnf`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M0/2NG.dN` & `ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M0/2NG.dN`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M0/algn` & `ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M0/algn`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M1/tree` & `ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M2/tree`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M1/M1.out` & `ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M1/M1.out`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M1/4fold.nuc` & `ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M2/4fold.nuc`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M1/lnf` & `ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M1/lnf`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M1/rst` & `ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M1/rst`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M1/algn` & `ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M2/algn`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M8/tree` & `ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M7/tree`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M8/4fold.nuc` & `ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M7/4fold.nuc`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M8/lnf` & `ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M8/lnf`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M8/rst` & `ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M8/rst`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M8/M8.out` & `ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M8/M8.out`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M8/algn` & `ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M7/algn`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/fb/tree` & `ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M8/tree`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/fb/fb.out` & `ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/slr/fb.out`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/fb/4fold.nuc` & `ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M8/4fold.nuc`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/fb/lnf` & `ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/slr/lnf`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/fb/algn` & `ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M8/algn`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M7/tree` & `ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/fb/tree`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M7/4fold.nuc` & `ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/fb/4fold.nuc`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M7/M7.out` & `ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M7/M7.out`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M7/lnf` & `ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M7/lnf`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M7/rst` & `ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M7/rst`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M7/algn` & `ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/fb/algn`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M2/tree` & `ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/slr/tree`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M2/4fold.nuc` & `ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/slr/4fold.nuc`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M2/lnf` & `ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M2/lnf`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M2/rst` & `ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M2/rst`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M2/M2.out` & `ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/paml/M2/M2.out`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/protamine/PRM1/paml/M2/algn` & `ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/slr/algn`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/data/protamine/PRM1/alignments.fasta_ali` & `ete3-3.1.3/ete3/test/ete_evol_data/protamine/PRM1/alignments.fasta_ali`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/4_branch_models.py` & `ete3-3.1.3/examples/evol/4_branch_models.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/1_freeratio.py` & `ete3-3.1.3/examples/evol/1_freeratio.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/measuring_evolution_trees.py` & `ete3-3.1.3/examples/evol/measuring_evolution_trees.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/5_branchsite_cladetest.py` & `ete3-3.1.3/examples/evol/5_branchsite_cladetest.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/test_protamine.py` & `ete3-3.1.3/examples/evol/test_protamine.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/6_ancestral_sequence.py` & `ete3-3.1.3/examples/evol/6_ancestral_sequence.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/evol/3_branchsite_test.py` & `ete3-3.1.3/examples/evol/3_branchsite_test.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/phyloxml/apaf.xml` & `ete3-3.1.3/examples/phyloxml/apaf.xml`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/phyloxml/example1.xml` & `ete3-3.1.3/examples/phyloxml/example1.xml`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/phyloxml/example3.xml` & `ete3-3.1.3/examples/phyloxml/example3.xml`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/phyloxml/phyloxml_examples.xml` & `ete3-3.1.3/examples/phyloxml/phyloxml_examples.xml`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/phyloxml/phyloxml_from_scratch.py` & `ete3-3.1.3/examples/phyloxml/phyloxml_from_scratch.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/phyloxml/tol_life_on_earth.xml.bz2` & `ete3-3.1.3/examples/phyloxml/tol_life_on_earth.xml.bz2`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/phyloxml/phyloxml_parser.py` & `ete3-3.1.3/examples/phyloxml/phyloxml_parser.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/phyloxml/ncbi_taxonomy_metazoa.xml.bz2` & `ete3-3.1.3/examples/phyloxml/ncbi_taxonomy_metazoa.xml.bz2`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/phyloxml/example2.xml` & `ete3-3.1.3/examples/phyloxml/example2.xml`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/phyloxml/multiple_supports.xml` & `ete3-3.1.3/examples/phyloxml/multiple_supports.xml`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/phyloxml/bcl_2.xml` & `ete3-3.1.3/examples/phyloxml/bcl_2.xml`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/treeview/node_style.png` & `ete3-3.1.3/ete3/test/test_treeview/node_style.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/treeview/face_grid.py` & `ete3-3.1.3/examples/treeview/face_grid.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/treeview/node_style.py` & `ete3-3.1.3/examples/treeview/node_style.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/treeview/face_positions.py` & `ete3-3.1.3/examples/treeview/face_positions.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/treeview/seq_motif_faces.png` & `ete3-3.1.3/examples/treeview/seq_motif_faces.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/treeview/barcharts.png` & `ete3-3.1.3/ete3/test/test_treeview/barcharts.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/treeview/bubble_map.png` & `ete3-3.1.3/ete3/test/test_treeview/bubble_map.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/treeview/item_faces.py` & `ete3-3.1.3/examples/treeview/item_faces.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/treeview/node_background.py` & `ete3-3.1.3/examples/treeview/node_background.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/treeview/img_faces/fish.png` & `ete3-3.1.3/examples/general/fish.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/treeview/img_faces/img_faces.png` & `ete3-3.1.3/ete3/test/test_treeview/img_faces.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/treeview/img_faces/chimp.png` & `ete3-3.1.3/examples/general/chimp.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/treeview/img_faces/dog.png` & `ete3-3.1.3/examples/general/dog.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/treeview/img_faces/human.png` & `ete3-3.1.3/examples/general/human.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/treeview/img_faces/fly.png` & `ete3-3.1.3/examples/general/fly.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/treeview/img_faces/mouse.png` & `ete3-3.1.3/examples/general/mouse.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/treeview/img_faces/img_faces.py` & `ete3-3.1.3/examples/treeview/img_faces/img_faces.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/treeview/item_faces.png` & `ete3-3.1.3/ete3/test/test_treeview/item_faces.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/treeview/float_piechart.png` & `ete3-3.1.3/ete3/test/test_treeview/float_piechart.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/treeview/tree_faces.png` & `ete3-3.1.3/ete3/test/test_treeview/tree_faces.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/treeview/tree_faces.py` & `ete3-3.1.3/examples/treeview/tree_faces.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/treeview/seq_motif_faces.py` & `ete3-3.1.3/examples/treeview/seq_motif_faces.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/treeview/barchart_and_piechart_faces.py` & `ete3-3.1.3/examples/treeview/barchart_and_piechart_faces.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/treeview/seqmotif.png` & `ete3-3.1.3/ete3/test/test_treeview/seqmotif.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/treeview/new_seq_face.py` & `ete3-3.1.3/examples/treeview/new_seq_face.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/treeview/rotated_faces.png` & `ete3-3.1.3/ete3/test/test_treeview/rotated_faces.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/treeview/node_background.png` & `ete3-3.1.3/ete3/test/test_treeview/node_background.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/treeview/face_rotation.py` & `ete3-3.1.3/examples/treeview/face_rotation.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/treeview/bubble_map.py` & `ete3-3.1.3/examples/treeview/bubble_map.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/treeview/floating_piecharts.py` & `ete3-3.1.3/examples/treeview/floating_piecharts.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/treeview/random_draw.py` & `ete3-3.1.3/examples/treeview/random_draw.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/phylogenies/phylotree.png` & `ete3-3.1.3/examples/phylogenies/phylotree.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/phylogenies/link_sequences_to_phylogenies.py` & `ete3-3.1.3/examples/phylogenies/link_sequences_to_phylogenies.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/phylogenies/dating_evolutionary_events.py` & `ete3-3.1.3/examples/phylogenies/dating_evolutionary_events.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/phylogenies/phylotree_visualization.py` & `ete3-3.1.3/examples/phylogenies/phylotree_visualization.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/phylogenies/species_aware_phylogenies.py` & `ete3-3.1.3/examples/phylogenies/species_aware_phylogenies.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/phylogenies/tree_reconciliation.py` & `ete3-3.1.3/examples/phylogenies/tree_reconciliation.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/phylogenies/orthology_and_paralogy_prediction.py` & `ete3-3.1.3/examples/phylogenies/orthology_and_paralogy_prediction.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/webplugin/jquery-ui-1.8.4.custom.min.js` & `ete3-3.1.3/examples/webplugin/jquery-ui-1.8.4.custom.min.js`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/webplugin/loader.gif` & `ete3-3.1.3/examples/webplugin/loader.gif`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/webplugin/icon_cancel_search.png` & `ete3-3.1.3/examples/webplugin/icon_cancel_search.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/webplugin/close.png` & `ete3-3.1.3/examples/webplugin/close.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/webplugin/webplugin_example.html` & `ete3-3.1.3/examples/webplugin/webplugin_example.html`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/webplugin/ete.css` & `ete3-3.1.3/examples/webplugin/ete.css`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/webplugin/wsgi/webplugin_example.py` & `ete3-3.1.3/examples/webplugin/wsgi/webplugin_example.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/webplugin/icon_tools.png` & `ete3-3.1.3/examples/webplugin/icon_tools.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/webplugin/jquery-1.4.2.min.js` & `ete3-3.1.3/examples/webplugin/jquery-1.4.2.min.js`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/webplugin/icon_attachment.png` & `ete3-3.1.3/examples/webplugin/icon_attachment.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/webplugin/icon_search.png` & `ete3-3.1.3/examples/webplugin/icon_search.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/webplugin/README` & `ete3-3.1.3/examples/webplugin/README`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/examples/webplugin/ete.js` & `ete3-3.1.3/examples/webplugin/ete.js`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/CITATION.txt` & `ete3-3.1.3/CITATION.txt`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/README.rst` & `ete3-3.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3.egg-info/PKG-INFO` & `ete3-3.1.3/ete3.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,20 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: ete3
-Version: 3.1.2
+Version: 3.1.3
 Summary: A Python Environment for (phylogenetic) Tree Exploration
 Home-page: http://etetoolkit.org
+Download-URL: http://etetoolkit.org/static/releases/ete3/
 Author: Jaime Huerta-Cepas
 Author-email: jhcepas@gmail.com
 Maintainer: Jaime Huerta-Cepas
 Maintainer-email: huerta@embl.de
 License: GPLv3
-Download-URL: http://etetoolkit.org/static/releases/ete3/
-Description: 
-        The Environment for Tree Exploration (ETE) is a Python programming
-        toolkit that assists in the recontruction, manipulation, analysis and
-        visualization of phylogenetic trees (although clustering trees or any
-        other tree-like data structure are also supported).
-        
-        ETE is currently developed as a tool for researchers working in
-        phylogenetics and genomics. If you use ETE for a published work,
-        please cite:
-        
-        ::
-        
-           Jaime Huerta-Cepas, François Serra and Peer Bork. "ETE 3: Reconstruction,
-           analysis and visualization of phylogenomic data."  Mol Biol Evol (2016) doi:
-           10.1093/molbev/msw046
-        
-        Visit http://etetoolkit.org for more info.
-        
+Project-URL: Documentation, http://etetoolkit.org/docs/latest/tutorial/index.html
+Project-URL: Source, https://github.com/etetoolkit/ete
 Keywords: tree,tree reconstruction,tree visualization,tree comparison,phylogeny,phylogenetics,phylogenomics
 Platform: OS Independent
 Classifier: Development Status :: 6 - Mature
 Classifier: Environment :: Console
 Classifier: Environment :: X11 Applications :: Qt
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
@@ -42,7 +26,26 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires: six
 Provides: ete3
+License-File: LICENSE
+
+
+The Environment for Tree Exploration (ETE) is a Python programming
+toolkit that assists in the recontruction, manipulation, analysis and
+visualization of phylogenetic trees (although clustering trees or any
+other tree-like data structure are also supported).
+
+ETE is currently developed as a tool for researchers working in
+phylogenetics and genomics. If you use ETE for a published work,
+please cite:
+
+::
+
+   Jaime Huerta-Cepas, François Serra and Peer Bork. "ETE 3: Reconstruction,
+   analysis and visualization of phylogenomic data."  Mol Biol Evol (2016) doi:
+   10.1093/molbev/msw046
+
+Visit http://etetoolkit.org for more info.
```

### Comparing `ete3-3.1.2/ete3.egg-info/SOURCES.txt` & `ete3-3.1.3/ete3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/clustering/__init__.py` & `ete3-3.1.3/ete3/clustering/__init__.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/clustering/clustvalidation.py` & `ete3-3.1.3/ete3/clustering/clustvalidation.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/clustering/clustertree.py` & `ete3-3.1.3/ete3/clustering/clustertree.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/ncbi_taxonomy/__init__.py` & `ete3-3.1.3/ete3/ncbi_taxonomy/__init__.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/ncbi_taxonomy/ncbiquery.py` & `ete3-3.1.3/ete3/ncbi_taxonomy/ncbiquery.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,35 +93,35 @@
 class NCBITaxa(object):
     """
     versionadded: 2.3
 
     Provides a local transparent connector to the NCBI taxonomy database.
     """
 
-    def __init__(self, dbfile=None, taxdump_file=None):
+    def __init__(self, dbfile=None, taxdump_file=None, update=True):
 
         if not dbfile:
             self.dbfile = DEFAULT_TAXADB
         else:
             self.dbfile = dbfile
 
         if taxdump_file:
             self.update_taxonomy_database(taxdump_file)
 
-        if dbfile is None and not os.path.exists(self.dbfile):
+        if dbfile != DEFAULT_TAXADB and not os.path.exists(self.dbfile):
             print('NCBI database not present yet (first time used?)', file=sys.stderr)
             self.update_taxonomy_database(taxdump_file)
 
         if not os.path.exists(self.dbfile):
             raise ValueError("Cannot open taxonomy database: %s" % self.dbfile)
 
         self.db = None
         self._connect()
 
-        if not is_taxadb_up_to_date(self.dbfile):
+        if not is_taxadb_up_to_date(self.dbfile) and update:
             print('NCBI database format is outdated. Upgrading', file=sys.stderr)
             self.update_taxonomy_database(taxdump_file)
 
     def update_taxonomy_database(self, taxdump_file=None):
         """Updates the ncbi taxonomy database by downloading and parsing the latest
         taxdump.tar.gz file from the NCBI FTP site (via HTTP).
 
@@ -367,15 +367,15 @@
         if rank_limit or collapse_subspecies or return_tree:
             tree = self.get_topology(list(descendants.keys()), intermediate_nodes=intermediate_nodes, collapse_subspecies=collapse_subspecies, rank_limit=rank_limit)
             if return_tree:
                 return tree
             elif intermediate_nodes:
                 return list(map(int, [n.name for n in tree.get_descendants()]))
             else:
-                return map(int, [n.name for n in tree])
+                return list(map(int, [n.name for n in tree]))
 
         elif intermediate_nodes:
             return [tid for tid, count in six.iteritems(descendants)]
         else:
             return [tid for tid, count in six.iteritems(descendants) if count == 1]
 
     def get_topology(self, taxids, intermediate_nodes=False, rank_limit=None, collapse_subspecies=False, annotate=True):
@@ -406,19 +406,19 @@
             descendants = {}
             found = 0
             nodes = {}
             hit = 0
             visited = set()
             start = prepostorder.index(root_taxid)
             try:
-            	end = prepostorder.index(root_taxid, start+1)
-            	subtree = prepostorder[start:end+1]
+                end = prepostorder.index(root_taxid, start+1)
+                subtree = prepostorder[start:end+1]
             except ValueError:
                 # If root taxid is not found in postorder, must be a tip node
-            	subtree = [root_taxid]
+                subtree = [root_taxid]
             leaves = set([v for v, count in Counter(subtree).items() if count == 1])
             nodes[root_taxid] = PhyloTree(name=str(root_taxid))
             current_parent = nodes[root_taxid]
             for tid in subtree:
                 if tid in visited:
                     current_parent = nodes[tid].up
                 else:
```

### Comparing `ete3-3.1.2/ete3/ncbi_taxonomy/SQLite-Levenshtein/src/levenshtein.c` & `ete3-3.1.3/ete3/ncbi_taxonomy/SQLite-Levenshtein/src/levenshtein.c`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/ncbi_taxonomy/SQLite-Levenshtein/tests/levenshtein-test.sql` & `ete3-3.1.3/ete3/ncbi_taxonomy/SQLite-Levenshtein/tests/levenshtein-test.sql`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/ncbi_taxonomy/SQLite-Levenshtein/tests/README` & `ete3-3.1.3/ete3/ncbi_taxonomy/SQLite-Levenshtein/tests/README`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/__init__.py` & `ete3-3.1.3/ete3/__init__.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/nexml/__init__.py` & `ete3-3.1.3/ete3/nexml/__init__.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/nexml/_nexml.py` & `ete3-3.1.3/ete3/nexml/_nexml.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/nexml/_nexml_tree.py` & `ete3-3.1.3/ete3/nexml/_nexml_tree.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_maptrees.py` & `ete3-3.1.3/ete3/tools/ete_maptrees.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/__init__.py` & `ete3-3.1.3/ete3/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_annotate.py` & `ete3-3.1.3/ete3/tools/ete_annotate.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build.py` & `ete3-3.1.3/ete3/tools/ete_build.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build_lib/getch.py` & `ete3-3.1.3/ete3/tools/ete_build_lib/getch.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build_lib/visualize.py` & `ete3-3.1.3/ete3/tools/ete_build_lib/visualize.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build_lib/__init__.py` & `ete3-3.1.3/ete3/tools/ete_build_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build_lib/configcheck.py` & `ete3-3.1.3/ete3/tools/ete_build_lib/configcheck.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build_lib/ordereddict.py` & `ete3-3.1.3/ete3/tools/ete_build_lib/ordereddict.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build_lib/sge.py` & `ete3-3.1.3/ete3/tools/ete_build_lib/sge.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build_lib/master_task.py` & `ete3-3.1.3/ete3/tools/ete_build_lib/master_task.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build_lib/interface.py` & `ete3-3.1.3/ete3/tools/ete_build_lib/interface.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build_lib/logger.py` & `ete3-3.1.3/ete3/tools/ete_build_lib/logger.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build_lib/db.py` & `ete3-3.1.3/ete3/tools/ete_build_lib/db.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build_lib/scheduler.py` & `ete3-3.1.3/ete3/tools/ete_build_lib/scheduler.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build_lib/configobj.py` & `ete3-3.1.3/ete3/tools/ete_build_lib/configobj.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build_lib/curses_gui.py` & `ete3-3.1.3/ete3/tools/ete_build_lib/curses_gui.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build_lib/errors.py` & `ete3-3.1.3/ete3/tools/ete_build_lib/errors.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build_lib/validate.py` & `ete3-3.1.3/ete3/tools/ete_build_lib/validate.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build_lib/utils.py` & `ete3-3.1.3/ete3/tools/ete_build_lib/utils.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build_lib/apps.py` & `ete3-3.1.3/ete3/tools/ete_build_lib/apps.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build_lib/task/concat_alg.py` & `ete3-3.1.3/ete3/tools/ete_build_lib/task/concat_alg.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build_lib/task/__init__.py` & `ete3-3.1.3/ete3/tools/ete_build_lib/task/__init__.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build_lib/task/prottest2.py` & `ete3-3.1.3/ete3/tools/ete_build_lib/task/prottest2.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build_lib/task/merger.py` & `ete3-3.1.3/ete3/tools/ete_build_lib/task/merger.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build_lib/task/prottest.py` & `ete3-3.1.3/ete3/tools/ete_build_lib/task/prottest.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build_lib/task/iqtree.py` & `ete3-3.1.3/ete3/tools/ete_build_lib/task/iqtree.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build_lib/task/meta_aligner.py` & `ete3-3.1.3/ete3/tools/ete_build_lib/task/meta_aligner.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build_lib/task/trimal.py` & `ete3-3.1.3/ete3/tools/ete_build_lib/task/trimal.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build_lib/task/msf.py` & `ete3-3.1.3/ete3/tools/ete_build_lib/task/msf.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build_lib/task/muscle.py` & `ete3-3.1.3/ete3/tools/ete_build_lib/task/muscle.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build_lib/task/dummyalg.py` & `ete3-3.1.3/ete3/tools/ete_build_lib/task/dummyalg.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build_lib/task/cog_creator.py` & `ete3-3.1.3/ete3/tools/ete_build_lib/task/cog_creator.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build_lib/task/fasttree.py` & `ete3-3.1.3/ete3/tools/ete_build_lib/task/fasttree.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build_lib/task/clustalo.py` & `ete3-3.1.3/ete3/tools/ete_build_lib/task/clustalo.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build_lib/task/dialigntx.py` & `ete3-3.1.3/ete3/tools/ete_build_lib/task/dialigntx.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build_lib/task/dummytree.py` & `ete3-3.1.3/ete3/tools/ete_build_lib/task/dummytree.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build_lib/task/raxml.py` & `ete3-3.1.3/ete3/tools/ete_build_lib/task/raxml.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build_lib/task/mafft.py` & `ete3-3.1.3/ete3/tools/ete_build_lib/task/mafft.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build_lib/task/uhire.py` & `ete3-3.1.3/ete3/tools/ete_build_lib/task/uhire.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build_lib/task/tcoffee.py` & `ete3-3.1.3/ete3/tools/ete_build_lib/task/tcoffee.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build_lib/task/cog_selector.py` & `ete3-3.1.3/ete3/tools/ete_build_lib/task/cog_selector.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build_lib/task/jmodeltest.py` & `ete3-3.1.3/ete3/tools/ete_build_lib/task/jmodeltest.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build_lib/task/pmodeltest.py` & `ete3-3.1.3/ete3/tools/ete_build_lib/task/pmodeltest.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build_lib/task/phyml.py` & `ete3-3.1.3/ete3/tools/ete_build_lib/task/phyml.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build_lib/seqio.py` & `ete3-3.1.3/ete3/tools/ete_build_lib/seqio.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build_lib/workflow/__init__.py` & `ete3-3.1.3/ete3/tools/ete_build_lib/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build_lib/workflow/supermatrix.py` & `ete3-3.1.3/ete3/tools/ete_build_lib/workflow/supermatrix.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build_lib/workflow/genetree.py` & `ete3-3.1.3/ete3/tools/ete_build_lib/workflow/genetree.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build_lib/workflow/common.py` & `ete3-3.1.3/ete3/tools/ete_build_lib/workflow/common.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build_lib/master_job.py` & `ete3-3.1.3/ete3/tools/ete_build_lib/master_job.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_view.py` & `ete3-3.1.3/ete3/tools/ete_view.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_split.py` & `ete3-3.1.3/ete3/tools/ete_split.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_compare.py` & `ete3-3.1.3/ete3/tools/ete_compare.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_mod.py` & `ete3-3.1.3/ete3/tools/ete_mod.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_expand.py` & `ete3-3.1.3/ete3/tools/ete_expand.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_ncbiquery.py` & `ete3-3.1.3/ete3/tools/ete_ncbiquery.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_evol.py` & `ete3-3.1.3/ete3/tools/ete_evol.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_build.cfg` & `ete3-3.1.3/ete3/tools/ete_build.cfg`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_extract.py` & `ete3-3.1.3/ete3/tools/ete_extract.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/common.py` & `ete3-3.1.3/ete3/tools/common.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/utils.py` & `ete3-3.1.3/ete3/tools/utils.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_generate.py` & `ete3-3.1.3/ete3/tools/ete_generate.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete_upgrade_tools.py` & `ete3-3.1.3/ete3/tools/ete_upgrade_tools.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/tools/ete.py` & `ete3-3.1.3/ete3/tools/ete.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/evol/__init__.py` & `ete3-3.1.3/ete3/evol/__init__.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/evol/control.py` & `ete3-3.1.3/ete3/evol/control.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/evol/evoltree.py` & `ete3-3.1.3/ete3/evol/evoltree.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,20 +40,28 @@
 """
 this module defines the EvolNode dataytype to manage evolutionary
 variables and integrate them within phylogenetic trees. It inheritates
 the coretype PhyloNode and add some speciall features to the the node
 instances.
 """
 from __future__ import absolute_import
+from ..tools.utils import which
+from .utils import translate
+from .model import Model, PARAMS, AVAIL
+from ..parser.newick import write_newick
+from .. import PhyloNode, SeqGroup
+from warnings import warn
+import sys
+import os
 from six.moves import map
 
-__author__     = "Francois-Jose Serra"
-__email__      = "francois@barrabin.org"
-__licence__    = "GPLv3"
-__version__    = "0.0"
+__author__ = "Francois-Jose Serra"
+__email__ = "francois@barrabin.org"
+__licence__ = "GPLv3"
+__version__ = "0.0"
 __references__ = '''
 Yang, Z., Nielsen, R., Goldman, N., & Pedersen, A. M. 2000.
     Codon-substitution models for heterogeneous selection pressure at amino acid sites.
     Genetics 155: 431-49.
     Retrieved from http://www.pubmedcentral.nih.gov/articlerender.fcgi?artid=1461088&tool=pmcentrez&rendertype=abstract
 Yang, Z., & Nielsen, R. 2002.
     Codon-substitution models for detecting molecular adaptation at individual sites along specific lineages.
@@ -69,44 +77,38 @@
     Retrieved from http://www.ncbi.nlm.nih.gov/pubmed/16107592
 Yang, Z. 2007.
     PAML 4: phylogenetic analysis by maximum likelihood.
     Molecular biology and evolution 24: 1586-91.
     Retrieved from http://www.ncbi.nlm.nih.gov/pubmed/17483113
 '''
 
-import os
-import sys
-from warnings import warn
 
-from .. import PhyloNode, SeqGroup
-from ..parser.newick import write_newick
-from .model import Model, PARAMS, AVAIL
-from .utils import translate
-from ..tools.utils import which
 try:
     from scipy.stats import chi2
-    chi_high = lambda x, y: 1 - chi2.cdf(x, y)
+    def chi_high(x, y): return 1 - chi2.cdf(x, y)
 except ImportError:
     from .utils import chi_high
 
 try:
     from ..treeview import TreeStyle
 except ImportError:
     TREEVIEW = False
 else:
     TREEVIEW = True
 
 __all__ = ["EvolNode", "EvolTree"]
 
+
 def _parse_species(name):
     '''
     just to return specie name from fasta description
     '''
     return name[:3]
 
+
 class EvolNode(PhyloNode):
     """ Re-implementation of the standart TreeNode instance. It adds
     attributes and methods to work with phylogentic trees.
 
     :argument newick: path to tree in newick format, can also be a string
     :argument alignment: path to alignment, can also be a string.
     :argument fasta alg_format: alignment format.
@@ -114,15 +116,15 @@
     :argument format: type of newick format
     :argument binpath: path to binaries, in case codeml or SLR are not in global path.
 
     """
 
     def __init__(self, newick=None, alignment=None, alg_format="fasta",
                  sp_naming_function=_parse_species, format=0,
-                  binpath='', **kwargs):
+                 binpath='', **kwargs):
         '''
         freebranch: path to find codeml output of freebranch model.
         '''
         # _update names?
         self.workdir = '/tmp/ete3-tmp/'
         if not binpath:
             ete3_path = which("ete3")
@@ -163,19 +165,20 @@
         WARNING: sorted names in same order that sequence
         WARNING: depends on tree topology conformation, not the same after a swap
         activates the function get_descendants_by_pamlid
         '''
         nid = 1
         # check we do not have dupplicated names in tree
         if (len(self)) != len(set(self.get_leaf_names())):
-            duplis = [n for n in self.get_leaf_names() if self.get_leaf_names().count(n)>1]
+            duplis = [n for n in self.get_leaf_names(
+            ) if self.get_leaf_names().count(n) > 1]
             raise Exception('EvolTree require unique names for leaves', duplis)
         # put ids
         for leaf in sorted(self, key=lambda x: x.name):
-            leaf.add_feature ('node_id', nid)
+            leaf.add_feature('node_id', nid)
             nid += 1
         self.add_feature('node_id', nid)
         self._label_internal_nodes([nid])
 
     def get_descendant_by_node_id(self, idname):
         '''
         returns node list corresponding to a given idname
@@ -183,29 +186,28 @@
         try:
             for n in self.iter_descendants():
                 if n.node_id == idname:
                     return n
             if self.node_id == idname:
                 return self
         except AttributeError:
-            warn('Should be first labelled as paml ' + \
+            warn('Should be first labelled as paml ' +
                  '(automatically done when alignemnt is loaded)')
 
     def _write_algn(self, fullpath):
         """
         to write algn in paml format
         """
         seq_group = SeqGroup()
         for n in self:
-            seq_group.id2seq  [n.node_id] = n.nt_sequence
-            seq_group.id2name [n.node_id] = n.name
-            seq_group.name2id [n.name   ] = n.node_id
+            seq_group.id2seq[n.node_id] = n.nt_sequence
+            seq_group.id2name[n.node_id] = n.name
+            seq_group.name2id[n.name] = n.node_id
         seq_group.write(outfile=fullpath, format='paml')
 
-
     def run_model(self, model_name, ctrl_string='', keep=True, **kwargs):
         '''
         To compute evolutionnary models.     e.g.: b_free_lala.vs.lele, will launch one free branch model, and store
         it in "WORK_DIR/b_free_lala.vs.lele" directory
 
         WARNING: this functionality needs to create a working directory in "rep"
 
@@ -222,77 +224,75 @@
         of these models, with continuous omega rates (namely M1a and M2a in the
         PAML user guide).**
 
         :argument model_name: a string like "model-name[.some-secondary-name]" (e.g.: "fb.my_first_try", or just "fb")
                               * model-name is compulsory, is the name of the model (see table above for the full list)
                               * the second part is accessory, it is to avoid over-writing models with the same name.
         :argument ctrl_string: list of parameters that can be used as control file.
+        :argument True keep: links the model to the tree (equivalen of running `EVOL_TREE.link_to_evol_model(MODEL_NAME)`)
         :argument kwargs: extra parameters should be one of: %s.
         '''
         from subprocess import Popen, PIPE
         model_obj = Model(model_name, self, **kwargs)
-        fullpath = os.path.join (self.workdir, model_obj.name)
-        os.system("mkdir -p %s" %fullpath)
+        fullpath = os.path.join(self.workdir, model_obj.name)
+        os.system("mkdir -p %s" % fullpath)
         # write tree file
         self._write_algn(fullpath + '/algn')
         if model_obj.properties['exec'] == 'Slr':
-            self.write(outfile=fullpath+'/tree', format = (11))
+            self.write(outfile=fullpath+'/tree', format=(11))
         else:
             self.write(outfile=fullpath+'/tree',
-                       format = (10 if model_obj.properties['allow_mark'] else 9))
+                       format=(10 if model_obj.properties['allow_mark'] else 9))
         # write algn file
-        ## MODEL MODEL MDE
+        # MODEL MODEL MDE
         if ctrl_string == '':
             ctrl_string = model_obj.get_ctrl_string(fullpath+'/tmp.ctl')
         else:
             open(fullpath+'/tmp.ctl', 'w').write(ctrl_string)
         hlddir = os.getcwd()
         os.chdir(fullpath)
         bin_ = os.path.join(self.execpath, model_obj.properties['exec'])
         try:
-            proc = Popen([bin_, 'tmp.ctl'], stdout=PIPE, stdin=PIPE)
+            proc = Popen([bin_, 'tmp.ctl'], stdout=PIPE,
+                         stdin=PIPE, stderr=PIPE)
         except OSError:
             raise Exception(('ERROR: {} not installed, ' +
                              'or wrong path to binary\n').format(bin_))
-        run, err = proc.communicate(b'\n') # send \n via stdin in case codeml/slr asks something (note on py3, stdin needs bytes)
+        # send \n via stdin in case codeml/slr asks something (note on py3, stdin needs bytes)
+        run, err = proc.communicate(b'\n')
         run = run.decode(sys.stdout.encoding)
 
-        if err is not None:
-            warn("ERROR: codeml not found!!!\n" +
-                 "       define your variable EvolTree.execpath")
-            return 1
-        if 'error' in run or 'Error' in run:
-            warn("ERROR: inside codeml!!\n" + run)
-            return 1
         os.chdir(hlddir)
+        if err:
+            warn("ERROR: inside codeml!!\n" + err)
+            return 1
         if keep:
             setattr(model_obj, 'run', run)
-            self.link_to_evol_model(os.path.join(fullpath,'out'), model_obj)
+            self.link_to_evol_model(os.path.join(fullpath, 'out'), model_obj)
     sep = '\n'
     run_model.__doc__ = run_model.__doc__ % \
-                        (sep.join(['          %-8s   %-27s   %-15s  ' % \
-                                      ('%s' % (x), AVAIL[x]['evol'], AVAIL[x]['typ']) for x in sorted (sorted (AVAIL.keys()), key=lambda x: \
-                                              AVAIL[x]['typ'],
-                                              reverse=True)]),
-                         ', '.join(list(PARAMS.keys())))
-
+        (sep.join(['          %-8s   %-27s   %-15s  ' %
+                   ('%s' % (x), AVAIL[x]['evol'], AVAIL[x]['typ']) for x in sorted(sorted(AVAIL.keys()), key=lambda x:
+                                                                                   AVAIL[x]['typ'],
+                                                                                   reverse=True)]),
+         ', '.join(list(PARAMS.keys())))
 
-    #def test_codon_model(self):
+    # def test_codon_model(self):
     #    for c_frq in range(4):
     #        self.run_model('M0.model_test-'+str(c_frq), CodonFreq=c_frq)
     #    if self.get_most_likely('M0.model_test-1', 'M0.model_test-0') > 0.05:
     #
     #    self.get_most_likely('M0.model_test-2', 'M0.model_test-0')
     #    self.get_most_likely('M0.model_test-3', 'M0.model_test-0')
     #    self.get_most_likely('M0.model_test-2', 'M0.model_test-1')
     #    self.get_most_likely('M0.model_test-3', 'M0.model_test-1')
     #    self.get_most_likely('M0.model_test-3', 'M0.model_test-2')
 
     def link_to_alignment(self, alignment, alg_format="paml",
-                           nucleotides=True, **kwargs):
+                          nucleotides=True, **kwargs):
         '''
         same function as for phyloTree, but translate sequences if nucleotides
         nucleotidic sequence is kept under node.nt_sequence
 
         :argument alignment: path to alignment or string
         :argument alg_format: one of fasta phylip or paml
         :argument True alignment: set to False in case we want to keep it untranslated
@@ -328,29 +328,28 @@
             if histfaces:
                 for hist in histfaces:
                     try:
                         mdl = self.get_evol_model(hist)
                     except AttributeError:
                         warn('model %s not computed' % (hist))
                     if not 'histface' in mdl.properties:
-                        if len(histfaces)>1 and histfaces.index(hist)!=0:
+                        if len(histfaces) > 1 and histfaces.index(hist) != 0:
                             mdl.set_histface(up=False)
                         else:
                             mdl.set_histface()
-                    if mdl.properties ['histface'].up:
+                    if mdl.properties['histface'].up:
                         ts.aligned_header.add_face(
                             mdl.properties['histface'], 1)
                     else:
                         ts.aligned_foot.add_face(
                             mdl.properties['histface'], 1)
             super(EvolTree, self).show(layout=layout, tree_style=ts)
         else:
             raise ValueError("Treeview module is disabled")
 
-
     def render(self, file_name, layout=None, w=None, h=None,
                tree_style=None, header=None, histfaces=None):
         '''
         call super show adding up and down faces
 
         :argument layout: a layout function
         :argument None tree_style: tree_style object
@@ -365,31 +364,30 @@
             if histfaces:
                 for hist in histfaces:
                     try:
                         mdl = self.get_evol_model(hist)
                     except AttributeError:
                         warn('model %s not computed' % (hist))
                     if not 'histface' in mdl.properties:
-                        if len(histfaces)>1 and histfaces.index(hist)!=0:
+                        if len(histfaces) > 1 and histfaces.index(hist) != 0:
                             mdl.set_histface(up=False)
                         else:
                             mdl.set_histface()
-                    if mdl.properties ['histface'].up:
+                    if mdl.properties['histface'].up:
                         ts.aligned_header.add_face(
                             mdl.properties['histface'], 1)
                     else:
                         ts.aligned_foot.add_face(
                             mdl.properties['histface'], 1)
             return super(EvolTree, self).render(file_name, layout=layout,
                                                 tree_style=ts,
                                                 w=w, h=h)
         else:
             raise ValueError("Treeview module is disabled")
 
-
     def mark_tree(self, node_ids, verbose=False, **kargs):
         '''
         function to mark branches on tree in order that paml could interpret it.
         takes a "marks" argument that should be a list of #1,#1,#2
         e.g.:
         ::
 
@@ -397,96 +395,95 @@
 
         :argument node_ids: list of node ids (have a look to node.node_id)
         :argument False verbose: warn if marks do not correspond to codeml standard
         :argument kargs: mainly for the marks key-word which needs a list of marks (marks=['#1', '#2'])
 
         '''
         from re import match
-        node_ids = list(map(int , node_ids))
+        node_ids = list(map(int, node_ids))
         if 'marks' in kargs:
             marks = list(kargs['marks'])
         else:
-            marks = ['#1']*len (node_ids)
+            marks = ['#1']*len(node_ids)
         for node in self.traverse():
             if not hasattr(node, 'node_id'):
                 continue
             if node.node_id in node_ids:
                 if ('.' in marks[node_ids.index(node.node_id)] or
                     match('#[0-9]+',
                           marks[node_ids.index(node.node_id)]) is None) and verbose:
                     warn('WARNING: marks should be "#" sign directly ' +
                          'followed by integer\n' + self.mark_tree.__doc__)
-                node.add_feature('mark', ' '+marks[node_ids.index(node.node_id)])
+                node.add_feature(
+                    'mark', ' '+marks[node_ids.index(node.node_id)])
             elif not 'mark' in node.features:
                 node.add_feature('mark', '')
 
     def link_to_evol_model(self, path, model):
         '''
         link EvolTree to evolutionary model
           * free-branch model ("fb") will append evol values to tree
           * Site models (M0, M1, M2, M7, M8) will give evol values by site
             and likelihood
 
         :argument path: path to outfile containing model computation result
         :argument model: either the name of a model, or a Model object (usually empty)
 
         '''
-        if type(model) == str :
+        if isinstance(model, str):
             model = Model(model, self, path)
         else:
             model._load(path)
         # new entry in _models dict
         while model.name in self._models:
             model.name = model.name.split('__')[0] + str(
                 (int(model.name.split('__')[1]) + 1)
                 if '__' in model.name else 0)
         self._models[model.name] = model
         if not os.path.isfile(path):
             warn("ERROR: not a file: " + path)
             return 1
-        if len(self._models) == 1 and model.properties['exec']=='codeml':
+        if len(self._models) == 1 and model.properties['exec'] == 'codeml':
             self.change_dist_to_evol('bL', model, fill=True)
 
     def get_evol_model(self, modelname):
         '''
         returns one precomputed model
 
         :argument modelname: string of the name of a model object stored
         :returns: Model object
         '''
         try:
             return self._models[modelname]
         except KeyError:
-            warn("Model %s not found." % (modelname))
-
+            Exception("ERROR: Model %s not found." % (modelname))
 
     def write(self, features=None, outfile=None, format=10):
         """
         Inherits from Tree but adds the tenth format, that allows to display marks for CodeML.
         TODO: internal writting format need to be something like 0
         """
         from re import sub
-        if int(format)==11:
+        if int(format) == 11:
             nwk = ' %s 1\n' % (len(self))
-            nwk += sub('\[&&NHX:mark=([ #0-9.]*)\]', r'\1', \
-                       write_newick(self, features=['mark'],format=9))
-        elif int(format)==10:
-            nwk = sub('\[&&NHX:mark=([ #0-9.]*)\]', r'\1', \
-                      write_newick(self, features=['mark'],format=9))
+            nwk += sub('\[&&NHX:mark=([ #0-9.]*)\]', r'\1',
+                       write_newick(self, features=['mark'], format=9))
+        elif int(format) == 10:
+            nwk = sub('\[&&NHX:mark=([ #0-9.]*)\]', r'\1',
+                      write_newick(self, features=['mark'], format=9))
         else:
-            nwk = write_newick(self, features=features,format=format)
+            nwk = write_newick(self, features=features, format=format)
         if outfile is not None:
             open(outfile, "w").write(nwk)
             return nwk
         else:
             return nwk
     write.__doc__ += super(PhyloNode, PhyloNode()).write.__doc__.replace(
         'argument format', 'argument 10 format')
 
-
     def get_most_likely(self, altn, null):
         '''
         Returns pvalue of LRT between alternative model and null model.
 
         usual comparison are:
 
         ============ ======= ===========================================
@@ -526,15 +523,15 @@
         altn = self.get_evol_model(altn)
         null = self.get_evol_model(null)
         if null.np > altn.np:
             warn("first model should be the alternative, change the order")
             return 1.0
         try:
             if hasattr(altn, 'lnL') and hasattr(null, 'lnL'):
-                if  null.lnL - altn.lnL < 0:
+                if null.lnL - altn.lnL < 0:
                     return chi_high(2 * abs(altn.lnL - null.lnL),
                                     float(altn.np - null.np))
                 else:
                     warn("\nWARNING: Likelihood of the alternative model is "
                          "smaller than null's (%f - %f = %f)" % (
                              null.lnL, altn.lnL, null.lnL - altn.lnL) +
                          "\nLarge differences (> 0.1) may indicate mistaken "
@@ -559,12 +556,12 @@
             return
         for node in self.iter_descendants():
             if not evol in model.branches[node.node_id]:
                 continue
             node.dist = model.branches[node.node_id][evol]
             if fill:
                 for e in ['dN', 'dS', 'w', 'bL']:
-                    node.add_feature(e, model.branches [node.node_id][e])
+                    node.add_feature(e, model.branches[node.node_id][e])
 
 
 # cosmetic alias
 EvolTree = EvolNode
```

### Comparing `ete3-3.1.2/ete3/evol/parser/__init__.py` & `ete3-3.1.3/ete3/evol/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/evol/parser/codemlparser.py` & `ete3-3.1.3/ete3/evol/parser/codemlparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,24 +103,24 @@
         # line to list
         line = line.replace(' +- ', ' ')
         line = re.sub ('[()]', '', line.strip()).split()
         # get amino-acid
         sites[typ].setdefault ('aa', []).append (line[1])
         # get site class probability
         probs = []
-        for i in range (k):
+        for i in range(k):
             probs.append (float (line[2+i]))
-            sites [typ].setdefault ('p'+str(i), []).append (float (line[2+i]))
-        sites [typ].setdefault ('pv', []).append (max (probs))
+            sites [typ].setdefault('p' + str(i), []).append(float(line[2+i]))
+        sites [typ].setdefault ('pv', []).append (max(probs))
         # get most likely site class
         classe = int (line [3 + i])
-        sites[typ].setdefault ('class', []).append (classe)
+        sites[typ].setdefault ('class', []).append(classe)
         # if there, get omega and error
         try:
-            sites [typ].setdefault ('w' , []).append (float (line [4 + i]))
+            sites [typ].setdefault('w' , []).append(float (line [4 + i]))
         except IndexError:
             # in this case we are with branch-site A or A1 and we should sum
             # probabilities of categories 2a and 2b
             probs = probs[:-2] + [sum(probs[-2:])]
             sites[typ]['pv'][-1] = max(probs)
             bsa = True
             try:
@@ -214,15 +214,15 @@
     # if we do not have tree, load it
     if model._tree is None:
         from ..evol import EvolTree
         model._tree = EvolTree (re.findall ('\(.*\);', ''.join(all_lines))[2])
         model._tree._label_as_paml()
     # starts parsing
     for i, line in enumerate (all_lines):
-        if line is '\n':
+        if line == '\n':
             continue
         # codon frequency
         if line.startswith('Codon frequencies under model'):
             model.stats ['codonFreq'] = []
             for j in range (16):
                 line = list(map (float, re.findall ('\d\.\d+', all_lines [i+j+1])))
                 model.stats ['codonFreq'] += [line]
```

### Comparing `ete3-3.1.2/ete3/evol/parser/slrparser.py` & `ete3-3.1.3/ete3/evol/parser/slrparser.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/evol/model.py` & `ete3-3.1.3/ete3/evol/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,16 +213,15 @@
             val = 'NEB'
         else:
             val = 'SLR'
         colors = self.colorize_rst(val, col=colors)
         if not 'ylim' in kwargs:
             kwargs['ylim'] = (0, 2)
         if errors:
-            errors = self.sites[val]['se'] if 'se' in self.sites[val]\
-                     else None
+            errors = self.sites[val].get('se', None)
         if TREEVIEW:
             try:
                 hist = SequencePlotFace(self.sites[val]['w'], hlines=hlines,
                                         colors=colors, errors=errors,
                                         ylabel=u'Omega (\u03c9)', kind=kind,
                                         **kwargs)
             except KeyError:
@@ -332,15 +331,15 @@
                             'branch-site models.')
         ps_model = 'positive' in self.properties['evol']
         categories = []
         for pval, curr_class in zip(self.sites[val]['pv'],
                                     self.sites[val]['class']):
             if pval < 0.95:
                 categories.append('NS')
-            elif curr_class != self.n_classes[val] and not ps_model:
+            elif curr_class == self.n_classes[val] and not ps_model:
                 if pval < 0.99:
                     categories.append('RX')
                 else:
                     categories.append('RX+')
             elif curr_class == 1:
                 if pval < 0.99:
                     categories.append('CN')
```

### Comparing `ete3-3.1.2/ete3/evol/utils.py` & `ete3-3.1.3/ete3/evol/utils.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/phyloxml/__init__.py` & `ete3-3.1.3/ete3/phyloxml/__init__.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/phyloxml/_phyloxml.py` & `ete3-3.1.3/ete3/phyloxml/_phyloxml.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/phyloxml/_phyloxml_tree.py` & `ete3-3.1.3/ete3/phyloxml/_phyloxml_tree.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/_ph.py` & `ete3-3.1.3/ete3/_ph.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/treeview/image_properties.ui` & `ete3-3.1.3/ete3/treeview/image_properties.ui`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/treeview/fit_region.png` & `ete3-3.1.3/ete3/treeview/fit_region.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/treeview/zoom_in.png` & `ete3-3.1.3/ete3/treeview/zoom_in.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/treeview/__init__.py` & `ete3-3.1.3/ete3/treeview/__init__.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/treeview/filesave.png` & `ete3-3.1.3/ete3/treeview/filesave.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/treeview/qt4_circular_render.py` & `ete3-3.1.3/ete3/treeview/qt4_circular_render.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/treeview/node_gui_actions.py` & `ete3-3.1.3/ete3/treeview/node_gui_actions.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/treeview/templates.py` & `ete3-3.1.3/ete3/treeview/templates.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/treeview/ete_icon.png` & `ete3-3.1.3/ete3/treeview/ete_icon.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/treeview/qt4_gui.py` & `ete3-3.1.3/ete3/treeview/qt4_gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,25 +68,20 @@
         QGraphicsRectItem.__init__(self, 0, 0, 0, 0)
         if parent:
             self.setParentItem(parent)
 
     def paint(self, p, option, widget):
         p.setPen(self.Color)
         p.setBrush(QBrush(Qt.NoBrush))
-        p.drawRect(self.rect().x(),self.rect().y(),self.rect().width(),self.rect().height())
+        p.drawRect(QRectF(self.rect().x(),self.rect().y(),self.rect().width(),self.rect().height()))
         return
         # Draw info text
         font = QFont("Arial",13)
         text = "%d selected."  % len(self.get_selected_nodes())
         textR = QFontMetrics(font).boundingRect(text)
-        if  self.rect().width() > textR.width() and \
-                self.rect().height() > textR.height()/2 and 0: # OJO !!!!
-            p.setPen(QPen(self.Color))
-            p.setFont(QFont("Arial",13))
-            p.drawText(self.rect().bottomLeft().x(),self.rect().bottomLeft().y(),text)
 
     def get_selected_nodes(self):
         selPath = QPainterPath()
         selPath.addRect(self.rect())
         self.scene().setSelectionArea(selPath)
         return [i.node for i in self.scene().selectedItems()]
 
@@ -165,15 +160,15 @@
         self.searchDialog._conf.setupUi(self.searchDialog)
 
         self.scene.setItemIndexMethod(QGraphicsScene.NoIndex)
 
         # Shows the whole tree by default
         #self.view.fitInView(self.scene.sceneRect(), Qt.KeepAspectRatio)
         splitter.setCollapsible(1, True)
-        splitter.setSizes([self.scene.sceneRect().width(), 10])
+        splitter.setSizes([int(self.scene.sceneRect().width()), 10])
 
         self.view.fitInView(0, 0, self.scene.sceneRect().width(), 200, Qt.KeepAspectRatio)
 
         # Check for updates
         self.check = CheckUpdates()
         #self.check.start()
         #self.connect(self.check, SIGNAL("output(QString)"), self._updatestatus)
```

### Comparing `ete3-3.1.2/ete3/treeview/force_topo.png` & `ete3-3.1.3/ete3/treeview/force_topo.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/treeview/zoom_out.png` & `ete3-3.1.3/ete3/treeview/zoom_out.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/treeview/search_dialog.ui` & `ete3-3.1.3/ete3/treeview/search_dialog.ui`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/treeview/y_reduce.png` & `ete3-3.1.3/ete3/treeview/y_reduce.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/treeview/ete_resources_rc.py` & `ete3-3.1.3/ete3/treeview/ete_resources_rc.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/treeview/fileopen.png` & `ete3-3.1.3/ete3/treeview/fileopen.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/treeview/drawer.py` & `ete3-3.1.3/ete3/treeview/drawer.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/treeview/search.png` & `ete3-3.1.3/ete3/treeview/search.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/treeview/main.py` & `ete3-3.1.3/ete3/treeview/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -403,15 +403,15 @@
     def set_layout_fn(self, layout):
         self._layout_handler = []
         if type(layout) not in set([list, set, tuple, frozenset]):
             layout = [layout]
 
         for ly in layout:
             # Validates layout function
-            if (type(ly) == types.FunctionType or type(ly) == types.MethodType or ly is None):
+            if callable(ly) is True or ly is None:
                 self._layout_handler.append(ly)
             else:
                 from . import layouts
                 try:
                     self._layout_handler.append(getattr(layouts, ly))
                 except Exception as e:
                     print(e)
@@ -678,15 +678,15 @@
         raise Exception("wrong unit format")
 
     x_scale, y_scale = w/main_rect.width(), h/main_rect.height()
 
     if ext == "SVG":
         svg = QSvgGenerator()
         targetRect = QRectF(0, 0, w, h)
-        svg.setSize(QSize(w, h))
+        svg.setSize(QSize(int(w), int(h)))
         svg.setViewBox(targetRect)
         svg.setTitle("Generated with ETE http://etetoolkit.org")
         svg.setDescription("Generated with ETE http://etetoolkit.org")
 
         if imgName == '%%return':
             ba = QByteArray()
             buf = QBuffer(ba)
@@ -699,31 +699,33 @@
         pp.begin(svg)
         scene.render(pp, targetRect, scene.sceneRect(), ratio_mode)
         pp.end()
         if imgName == '%%return':
             compatible_code = str(ba)
             print('from memory')
         else:
-            compatible_code = open(imgName).read()
+            with open(imgName) as f:
+                compatible_code = f.read()
+            
         # Fix a very annoying problem with Radial gradients in
         # inkscape and browsers...
         compatible_code = compatible_code.replace("xml:id=", "id=")
         compatible_code = re.sub('font-size="(\d+)"', 'font-size="\\1pt"', compatible_code)
         compatible_code = compatible_code.replace('\n', ' ')
         compatible_code = re.sub('<g [^>]+>\s*</g>', '', compatible_code)
         # End of fix
         if ipython_inline:
             from IPython.core.display import SVG
             return SVG(compatible_code)
 
         elif imgName == '%%return':
             return x_scale, y_scale, compatible_code
         else:
-            open(imgName, "w").write(compatible_code)
-
+            with open(imgName, "w") as f:
+                f.write(compatible_code)
 
     elif ext == "PDF" or ext == "PS":
         if ext == "PS":
             format = QPrinter.PostScriptFormat
         else:
             format = QPrinter.PdfFormat
 
@@ -745,18 +747,18 @@
         printer.setFullPage(True);
         printer.setOutputFileName(imgName);
         pp = QPainter(printer)
         targetRect =  QRectF(0, 0 , w, h)
         scene.render(pp, targetRect, scene.sceneRect(), ratio_mode)
     else:
         targetRect = QRectF(0, 0, w, h)
-        ii= QImage(w, h, QImage.Format_ARGB32)
+        ii= QImage(int(w), int(h), QImage.Format_ARGB32)
         ii.fill(QColor(Qt.white).rgb())
-        ii.setDotsPerMeterX(dpi / 0.0254) # Convert inches to meters
-        ii.setDotsPerMeterY(dpi / 0.0254)
+        ii.setDotsPerMeterX(int(dpi / 0.0254)) # Convert inches to meters
+        ii.setDotsPerMeterY(int(dpi / 0.0254))
         pp = QPainter(ii)
         pp.setRenderHint(QPainter.Antialiasing)
         pp.setRenderHint(QPainter.TextAntialiasing)
         pp.setRenderHint(QPainter.SmoothPixmapTransform)
 
         scene.render(pp, targetRect, scene.sceneRect(), ratio_mode)
         pp.end()
```

### Comparing `ete3-3.1.2/ete3/treeview/show_support.png` & `ete3-3.1.3/ete3/treeview/show_support.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/treeview/layouts.py` & `ete3-3.1.3/ete3/treeview/layouts.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/treeview/_open_newick.py` & `ete3-3.1.3/ete3/treeview/_open_newick.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/treeview/show_newick.ui` & `ete3-3.1.3/ete3/treeview/show_newick.ui`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/treeview/show_newick.png` & `ete3-3.1.3/ete3/treeview/show_newick.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/treeview/x_reduce.png` & `ete3-3.1.3/ete3/treeview/x_reduce.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/treeview/qt.py` & `ete3-3.1.3/ete3/treeview/qt.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 try:
     from PyQt4 import QtGui, QtCore
-    from PyQt4.QtCore import (Qt, QPointF, QRect, QRectF, QBuffer, QByteArray,
+    from PyQt4.QtCore import (Qt, QPointF, QRect, QLineF, QRectF, QBuffer, QByteArray,
                               QThread, QIODevice, QMetaObject, QModelIndex, QObject, QRegExp, QSize,
                               QSizeF,QVariant )
     from PyQt4.QtGui import (QAction, QApplication, QBrush, QCheckBox, QColor,
                              QColorDialog, QComboBox, QCursor, QDialog,
                              QDialogButtonBox, QFileDialog, QFont,
                              QFontMetrics, QGraphicsEllipseItem, QGraphicsItem,
                              QGraphicsItemGroup, QGraphicsLineItem,
@@ -21,15 +21,21 @@
                              QTextEdit, QToolBar, QTransform, QVBoxLayout,
                              QWidget)
     from PyQt4.QtSvg import QGraphicsSvgItem, QSvgGenerator
     from PyQt4.QtOpenGL import QGLFormat, QGLWidget
 
 except ImportError:
     from PyQt5 import QtGui, QtCore
-    from PyQt5.QtCore import (Qt, QPointF, QRect, QRectF, QBuffer, QByteArray,
+
+    # Fixes incompatibilities due to new overflow checking when converting integers introduced in qt 5.12
+    # https://www.riverbankcomputing.com/static/Docs/PyQt5/incompatibilities.html#pyqt-v5-12
+    import sip
+    sip.enableoverflowchecking(False)
+
+    from PyQt5.QtCore import (Qt, QPointF, QLineF, QRect, QRectF, QBuffer, QByteArray,
                               QThread, QIODevice, QMetaObject, QModelIndex, QObject, QRegExp, QSize,
                               QSizeF,  QVariant) #QString
     from PyQt5.QtSvg import QGraphicsSvgItem, QSvgGenerator
     from PyQt5.QtOpenGL import QGLFormat, QGLWidget
     from PyQt5.QtPrintSupport import QPrinter
     from PyQt5.QtWidgets import (QAction, QApplication, QCheckBox, QWidget,
                                  QColorDialog, QComboBox, QDialog, QDialogButtonBox, QFileDialog,
```

### Comparing `ete3-3.1.2/ete3/treeview/_mainwindow.py` & `ete3-3.1.3/ete3/treeview/_mainwindow.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/treeview/fit_tree.png` & `ete3-3.1.3/ete3/treeview/fit_tree.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/treeview/ete_resources.qrc` & `ete3-3.1.3/ete3/treeview/ete_resources.qrc`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/treeview/_about.py` & `ete3-3.1.3/ete3/treeview/_about.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/treeview/y_expand.png` & `ete3-3.1.3/ete3/treeview/y_expand.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/treeview/ete_qt4app.ui` & `ete3-3.1.3/ete3/treeview/ete_qt4app.ui`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/treeview/x_expand.png` & `ete3-3.1.3/ete3/treeview/x_expand.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/treeview/about.ui` & `ete3-3.1.3/ete3/treeview/about.ui`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/treeview/ete_logo.png` & `ete3-3.1.3/ete3/treeview/ete_logo.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/treeview/qt4_face_render.py` & `ete3-3.1.3/ete3/treeview/qt4_face_render.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,15 +244,15 @@
                 if max_h > h:
                     if f.vt_align == 0:
                         # Vertically on top
                         y_offset = 0
                     elif f.vt_align == 1:
                         # Vertically centered
                         y_offset = (max_h - h) / 2
-                    elif f.hz_align == 2:
+                    elif f.vt_align == 2:
                         # Vertically at bottom
                         y_offset = (max_h - h)
 
                 # Correct cases in which object faces has negative
                 # starting points
                 #obj_rect = obj.boundingRect()
                 #_pos = obj_rect.topLeft()
```

### Comparing `ete3-3.1.2/ete3/treeview/export_pdf.png` & `ete3-3.1.3/ete3/treeview/export_pdf.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/treeview/_show_newick.py` & `ete3-3.1.3/ete3/treeview/_show_newick.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/treeview/_search_dialog.py` & `ete3-3.1.3/ete3/treeview/_search_dialog.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/treeview/svg_colors.py` & `ete3-3.1.3/ete3/treeview/svg_colors.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/treeview/faces.py` & `ete3-3.1.3/ete3/treeview/faces.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,17 +59,17 @@
 from six.moves import map
 from six.moves import range
 from six.moves import zip
 
 from .qt import (QGraphicsRectItem, QGraphicsLineItem,
                  QGraphicsPolygonItem, QGraphicsEllipseItem,
                  QPen, QColor, QBrush, QPolygonF, QFont,
-                 QPixmap, QFontMetrics, QPainter,
+                 QPixmap, QFontMetrics, QPainter, QPainterPath,
                  QRadialGradient, QGraphicsSimpleTextItem, QGraphicsTextItem,
-                 QGraphicsItem, Qt,  QPointF, QRect, QRectF, QGraphicsSvgItem)
+                 QGraphicsItem, Qt, QLineF, QPointF, QRect, QRectF, QGraphicsSvgItem)
 
 from .main import add_face_to_node, _Background, _Border, COLOR_SCHEMES
 
 _aafgcolors = {
     'A':"#000000" ,
     'R':"#000000" ,
     'N':"#000000" ,
@@ -556,27 +556,27 @@
         # Mean and quartiles y positions
         mean_line_y = y + profile_height/2
         line2_y     = mean_line_y + profile_height/4
         line3_y     = mean_line_y - profile_height/4
 
         # Draw axis and scale
         p.setPen(QColor("black"))
-        p.drawRect(x2,y,profile_width, profile_height-1)
+        p.drawRect(QRectF(x2,y,profile_width, profile_height-1))
         p.setFont(QFont("Verdana",8))
-        p.drawText(profile_width,y+10,"%0.3f" %self.max_value)
-        p.drawText(profile_width,y+profile_height,"%0.3f" %self.min_value)
+        p.drawText(QPointF(profile_width,y+10), "%0.3f" %self.max_value)
+        p.drawText(QPointF(profile_width,y+profile_height), "%0.3f" %self.min_value)
 
         dashedPen = QPen(QBrush(QColor("#ddd")), 0)
         dashedPen.setStyle(Qt.DashLine)
 
         # Draw hz grid
         p.setPen(dashedPen)
-        p.drawLine(x2+1, mean_line_y, profile_width-2, mean_line_y )
-        p.drawLine(x2+1, line2_y, profile_width-2, line2_y )
-        p.drawLine(x2+1, line3_y, profile_width-2, line3_y )
+        p.drawLine(QLineF(x2+1, mean_line_y, profile_width-2, mean_line_y ))
+        p.drawLine(QLineF(x2+1, line2_y, profile_width-2, line2_y ))
+        p.drawLine(QLineF(x2+1, line3_y, profile_width-2, line3_y ))
 
 
         # Draw bars
         for pos in range(vlength):
             # first and second X pixel positions
             x1 = x2
             x2 = x1 + x_alpha
@@ -599,25 +599,25 @@
                 customColor = colors[100]
 
             # mean bar high
             mean_y1     = int ( (mean1 - self.min_value) * y_alpha)
 
             # Draw bar border
             p.setPen(QColor("black"))
-            #p.drawRect(x1+2,mean_y1, x_alpha-3, profile_height-mean_y1+1)
+            #p.drawRect(QRectF(x1+2,mean_y1, x_alpha-3, profile_height-mean_y1+1))
             # Fill bar with custom color
-            p.fillRect(x1+3,profile_height-mean_y1, x_alpha-4, mean_y1-1, QBrush(customColor))
+            p.fillRect(QRectF(x1+3,profile_height-mean_y1, x_alpha-4, mean_y1-1), QBrush(customColor))
 
             # Draw error bars
             if dev1 != 0:
                 dev_up_y1   = int((mean1+dev1 - self.min_value) * y_alpha)
                 dev_down_y1 = int((mean1-dev1 - self.min_value) * y_alpha)
-                p.drawLine(x1+x_alpha/2, profile_height-dev_up_y1 ,x1+x_alpha/2, profile_height-dev_down_y1 )
-                p.drawLine(x1-1+x_alpha/2,  profile_height-dev_up_y1, x1+1+x_alpha/2, profile_height-dev_up_y1 )
-                p.drawLine(x1-1+x_alpha/2,  profile_height-dev_down_y1, x1+1+x_alpha/2, profile_height-dev_down_y1 )
+                p.drawLine(QLineF(1+x_alpha/2, profile_height-dev_up_y1 ,x1+x_alpha/2, profile_height-dev_down_y1 ))
+                p.drawLine(QLineF(x1-1+x_alpha/2,  profile_height-dev_up_y1, x1+1+x_alpha/2, profile_height-dev_up_y1 ))
+                p.drawLine(QLineF(x1-1+x_alpha/2,  profile_height-dev_down_y1, x1+1+x_alpha/2, profile_height-dev_down_y1 ))
 
     def draw_centered_bar_profile(self):
         # Calculate vector
         mean_vector  = self.node.profile
         deviation_vector = self.node.deviation
         # If no vector, skip
         if mean_vector is None:
@@ -645,28 +645,28 @@
         # Mean and quartiles y positions
         mean_line_y = y + profile_height/2
         line2_y     = mean_line_y + profile_height/4
         line3_y     = mean_line_y - profile_height/4
 
         # Draw axis and scale
         p.setPen(QColor("black"))
-        p.drawRect(x2,y,profile_width, profile_height-1)
+        p.drawRect(QRectF(x2,y,profile_width), profile_height-1)
         p.setFont(QFont("Verdana",8))
-        p.drawText(profile_width,y+10,"%0.3f" %self.max_value)
-        p.drawText(profile_width,y+profile_height,"%0.3f" %self.min_value)
-        p.drawText(profile_width,mean_line_y,"%0.3f" %self.center_v)
+        p.drawText(QPointF(profile_width,y+10), "%0.3f" %self.max_value)
+        p.drawText(QPointF(profile_width,y+profile_height), "%0.3f" %self.min_value)
+        p.drawText(QPointF(profile_width,mean_line_y), "%0.3f" %self.center_v)
 
         dashedPen = QPen(QBrush(QColor("#ddd")), 0)
         dashedPen.setStyle(Qt.DashLine)
 
         # Draw hz grid
         p.setPen(dashedPen)
-        p.drawLine(x2+1, mean_line_y, profile_width-2, mean_line_y )
-        p.drawLine(x2+1, line2_y, profile_width-2, line2_y )
-        p.drawLine(x2+1, line3_y, profile_width-2, line3_y )
+        p.drawLine(QLineF(x2+1, mean_line_y, profile_width-2, mean_line_y ))
+        p.drawLine(QLineF(x2+1, line2_y, profile_width-2, line2_y ))
+        p.drawLine(QLineF(x2+1, line3_y, profile_width-2, line3_y ))
 
 
         # Draw bars
         for pos in range(vlength):
             # first and second X pixel positions
             x1 = x2
             x2 = x1 + x_alpha
@@ -700,32 +700,32 @@
                 mean_y1 = int(abs((mean1 - self.center_v) * y_alpha_up))
 
             # Draw bar border
             p.setPen(QColor("black"))
             #p.drawRect(x1+2,mean_y1, x_alpha-3, profile_height-mean_y1+1)
             # Fill bar with custom color
             if mean1<self.center_v:
-                p.fillRect(x1+3, mean_line_y, x_alpha-4, mean_y1, QBrush(customColor))
+                p.fillRect(QRectF(x1+3, mean_line_y, x_alpha-4, mean_y1), QBrush(customColor))
             else:
-                p.fillRect(x1+3, mean_line_y-mean_y1, x_alpha-4, mean_y1+1, QBrush(customColor))
+                p.fillRect(QRectF(x1+3, mean_line_y-mean_y1, x_alpha-4, mean_y1+1), QBrush(customColor))
 
             # Draw error bars
             if dev1 != 0:
                 if mean1<self.center_v:
                     dev_up_y1   = int((mean1+dev1 - self.center_v) * y_alpha_down)
                     dev_down_y1 = int((mean1-dev1 - self.center_v) * y_alpha_down)
-                    p.drawLine(x1+x_alpha/2, mean_line_y+dev_up_y1 ,x1+x_alpha/2, mean_line_y+dev_down_y1 )
-                    p.drawLine(x1-1+x_alpha/2, mean_line_y+dev_up_y1 ,x1+1+x_alpha/2, mean_line_y+dev_up_y1 )
-                    p.drawLine(x1-1+x_alpha/2, mean_line_y+dev_down_y1 ,x1+1+x_alpha/2, mean_line_y+dev_down_y1 )
+                    p.drawLine(QLineF(x1+x_alpha/2, mean_line_y+dev_up_y1 ,x1+x_alpha/2, mean_line_y+dev_down_y1 ))
+                    p.drawLine(QLineF(x1-1+x_alpha/2, mean_line_y+dev_up_y1 ,x1+1+x_alpha/2, mean_line_y+dev_up_y1 ))
+                    p.drawLine(QLineF(x1-1+x_alpha/2, mean_line_y+dev_down_y1 ,x1+1+x_alpha/2, mean_line_y+dev_down_y1 ))
                 else:
                     dev_up_y1   = int((mean1+dev1 - self.center_v) * y_alpha_up)
                     dev_down_y1 = int((mean1-dev1 - self.center_v) * y_alpha_up)
-                    p.drawLine(x1+x_alpha/2, mean_line_y-dev_up_y1 ,x1+x_alpha/2, mean_line_y-dev_down_y1 )
-                    p.drawLine(x1-1+x_alpha/2, mean_line_y-dev_up_y1 ,x1+1+x_alpha/2, mean_line_y-dev_up_y1 )
-                    p.drawLine(x1-1+x_alpha/2, mean_line_y-dev_down_y1 ,x1+1+x_alpha/2, mean_line_y-dev_down_y1 )
+                    p.drawLine(QLineF(x1+x_alpha/2, mean_line_y-dev_up_y1 ,x1+x_alpha/2, mean_line_y-dev_down_y1 ))
+                    p.drawLine(QLineF(x1-1+x_alpha/2, mean_line_y-dev_up_y1 ,x1+1+x_alpha/2, mean_line_y-dev_up_y1 ))
+                    p.drawLine(QLineF(x1-1+x_alpha/2, mean_line_y-dev_down_y1 ,x1+1+x_alpha/2, mean_line_y-dev_down_y1 ))
 
     def draw_line_profile(self):
         # Calculate vector
         mean_vector = self.node.profile
         deviation_vector = self.node.deviation
         if mean_vector is None:
             return
@@ -750,43 +750,43 @@
         # Mean and quartiles y positions
         mean_line_y = y + profile_height/2
         line2_y     = mean_line_y + profile_height/4
         line3_y     = mean_line_y - profile_height/4
 
         # Draw axis and scale
         p.setPen(QColor("black"))
-        p.drawRect(x2,y,profile_width, profile_height-1)
+        p.drawRect(QRectF(x2,y,profile_width, profile_height-1))
         p.setFont(QFont("Verdana",8))
-        p.drawText(profile_width,y+10,"%0.3f" %self.max_value)
-        p.drawText(profile_width,y+profile_height,"%0.3f" %self.min_value)
-        p.drawText(profile_width,mean_line_y+5,"%0.3f" %self.center_v)
+        p.drawText(QPointF(profile_width,y+10), "%0.3f" %self.max_value)
+        p.drawText(QPointF(profile_width,y+profile_height), "%0.3f" %self.min_value)
+        p.drawText(QPointF(profile_width,mean_line_y+5), "%0.3f" %self.center_v)
 
         dashedPen = QPen(QBrush(QColor("#ddd")), 0)
         dashedPen.setStyle(Qt.DashLine)
 
         # Draw hz grid
         p.setPen(dashedPen)
-        p.drawLine(x2+1, mean_line_y, profile_width-2, mean_line_y )
-        p.drawLine(x2+1, line2_y, profile_width-2, line2_y )
-        p.drawLine(x2+1, line3_y, profile_width-2, line3_y )
+        p.drawLine(QLineF(x2+1, mean_line_y, profile_width-2, mean_line_y ))
+        p.drawLine(QLineF(x2+1, line2_y, profile_width-2, line2_y ))
+        p.drawLine(QLineF(x2+1, line3_y, profile_width-2, line3_y ))
 
         # Draw lines
         for pos in range(0,vlength-1):
             dev1 =  self.fit_to_scale(mean_vector[pos] + deviation_vector[pos])
             dev2 =  self.fit_to_scale(mean_vector[pos+1] + deviation_vector[pos+1])
             mean1 = self.fit_to_scale(mean_vector[pos])
             mean2 = self.fit_to_scale(mean_vector[pos+1])
             # first and second X pixel positions
             x1 = x2
             x2 = x1 + x_alpha
 
             # Draw vt grid
             if x2 < profile_width:
                 p.setPen(dashedPen)
-                p.drawLine(x2, y+1, x2, profile_height-2)
+                p.drawLine(QLineF(x2, y+1, x2, profile_height-2))
 
             # If nan values, continue
             if not isfinite(mean1) or not isfinite(mean2):
                 continue
 
             # First Y postions for mean
             mean_y1 = (mean1 - self.min_value) * y_alpha
@@ -795,19 +795,19 @@
             if dev1!= 0 and dev2!=0:
                 # First Y postions for deviations
                 dev_y1   = (dev1 - self.min_value) * y_alpha
                 # Second Y postions for deviations
                 dev_y2   = (dev2 - self.min_value) * y_alpha
                 # Draw red deviation lines
                 p.setPen(QColor("red"))
-                p.drawLine(x1, profile_height-dev_y1, x2, profile_height-dev_y2)
-                p.drawLine(x1, profile_height+dev_y1, x2, profile_height+dev_y2)
+                p.drawLine(QLineF(x1, profile_height-dev_y1, x2, profile_height-dev_y2))
+                p.drawLine(QLineF(x1, profile_height+dev_y1, x2, profile_height+dev_y2))
             # Draw blue mean line
             p.setPen(QColor("blue"))
-            p.drawLine(x1, profile_height-mean_y1, x2, profile_height-mean_y2)
+            p.drawLine(QLineF(x1, profile_height-mean_y1, x2, profile_height-mean_y2))
 
 
     def draw_heatmap_profile(self):
         # Calculate vector
         vector = self.node.profile
         deviation = self.node.deviation
         # If no vector, skip
@@ -853,19 +853,19 @@
                 elif mean1<self.center_v:
                     color_index = abs(int(ceil(((self.center_v-mean1)*100)/(self.min_value-self.center_v))))
                     customColor = colors[100 - color_index]
                 else:
                     customColor = colors[100]
 
                 # Fill bar with custom color
-                p.fillRect(x1, y, x_alpha, y_step, QBrush(customColor))
+                p.fillRect(QRectF(x1, y, x_alpha, y_step), QBrush(customColor))
             y+= y_step
             x2 = 0
         p.end()
-        
+
     def fit_to_scale(self,v):
         if v<self.min_value:
             return float(self.min_value)
         elif v>self.max_value:
             return float(self.max_value)
         else:
             return float(v)
@@ -940,16 +940,16 @@
                 letter_brush = QBrush(QColor(self.ntbg.get(letter,"white" )))
                 letter_pen = QPen(QColor(self.ntfg.get(letter, "black")))
             else:
                 letter_brush = QBrush(QColor(self.aabg.get(letter,"white" )))
                 letter_pen = QPen(QColor(self.aafg.get(letter,"black" )))
 
             p.setPen(letter_pen)
-            p.fillRect(x,0,width, height,letter_brush)
-            p.drawText(x, y, letter)
+            p.fillRect(QRectF(x,0,width, height,letter_brush))
+            p.drawText(QPointF(x, y), letter)
             x += float(width)/len(self.seq)
         p.end()
 
 class TreeFace(Face):
     """
     .. versionadded:: 2.1
 
@@ -1221,15 +1221,15 @@
         else:
             painter.setPen(QColor(self.line_color))
 
         for i, p in enumerate(self.percents):
             col = self.colors[i]
             painter.setBrush(QBrush(QColor(col)))
             angle_span = (p/100.) * a
-            painter.drawPie(self.rect(), angle_start, angle_span )
+            painter.drawPie(self.rect(), int(angle_start), int(angle_span) )
             angle_start += angle_span
 
 
 class PieChartFace(StaticItemFace):
     """
     .. versionadded:: 2.2
 
@@ -1474,34 +1474,34 @@
         # Mean and quartiles y positions
         mean_line_y = y + (plot_height / 2.0)
         line2_y = mean_line_y + (plot_height/4.0)
         line3_y = mean_line_y - (plot_height/4.0)
 
         if self.draw_border:
             p.setPen(QColor("black"))
-            p.drawRect(x, y + 1, plot_width, plot_height)
+            p.drawRect(QRectF(x, y + 1, plot_width, plot_height))
 
         if self.draw_scale:
             p.setFont(QFont("Verdana", self.scale_fsize))
             font_height = QFontMetrics(p.font()).height()
             max_string = "% 7.2f" %max_value
             min_string = "% 7.2f" %min_value
-            p.drawText(plot_width + margin, font_height-2, max_string)
-            p.drawText(plot_width + margin, plot_height - 2, min_string)
-            p.drawLine(plot_width + margin - 1, 1, plot_width + margin - 1, plot_height+1)
-            p.drawLine(plot_width + margin - 1, 1, plot_width + margin + 2, 1)
-            p.drawLine(plot_width + margin - 1, plot_height+1, plot_width + margin + 2, plot_height+1)
+            p.drawText(QPointF(plot_width + margin, font_height-2), max_string)
+            p.drawText(QPointF(plot_width + margin, plot_height - 2), min_string)
+            p.drawLine(QLineF(plot_width + margin - 1, 1, plot_width + margin - 1, plot_height+1))
+            p.drawLine(QLineF(plot_width + margin - 1, 1, plot_width + margin + 2, 1))
+            p.drawLine(QLineF(plot_width + margin - 1, plot_height+1, plot_width + margin + 2, plot_height+1))
 
         if self.draw_grid:
             dashedPen = QPen(QBrush(QColor("#ddd")), 0)
             dashedPen.setStyle(Qt.DashLine)
             p.setPen(dashedPen)
-            p.drawLine(x+1, mean_line_y, plot_width - 2, mean_line_y)
-            p.drawLine(x+1, line2_y, plot_width - 2, line2_y )
-            p.drawLine(x+1, line3_y, plot_width - 2, line3_y )
+            p.drawLineQLineF((x+1, mean_line_y, plot_width - 2, mean_line_y))
+            p.drawLine(QLineF(x+1, line2_y, plot_width - 2, line2_y ))
+            p.drawLine(QLineF(x+1, line3_y, plot_width - 2, line3_y ))
 
         # Draw bars
         p.setFont(QFont("Verdana", self.label_fsize))
         label_height = self.rect().height() - self.height
         label_width = QFontMetrics(p.font()).height()
         for pos in range(len(values)):
             # first and second X pixel positions
@@ -1511,39 +1511,39 @@
             std =  deviations[pos]
             val = values[pos]
 
             if self.labels:
                 p.save()
                 p.translate(x1, plot_height+2)
                 p.rotate(90)
-                p.drawText(0, -x_alpha, label_height, x_alpha, Qt.AlignVCenter, str(self.labels[pos]))
-                #p.drawRect(0, -x_alpha, label_height, x_alpha)
+                p.drawText(QRectF(0, -x_alpha, label_height, x_alpha), Qt.AlignVCenter, str(self.labels[pos]))
+                #p.drawRect(QRectF(0, -x_alpha, label_height, x_alpha))
                 p.restore()
 
             # If nan value, skip
             if not isfinite(val):
                 continue
 
             color = QColor(colors[pos])
             # mean bar high
             mean_y1     = int((val - min_value) * y_alpha)
             # Draw bar border
             p.setPen(QColor("black"))
 
             # Fill bar with custom color
-            p.fillRect(x1, height - mean_y1, x_alpha, mean_y1, QBrush(color))
+            p.fillRect(QRectF(x1, height - mean_y1, x_alpha, mean_y1), QBrush(color))
 
             # Draw error bars
             if std != 0:
                 dev_up_y1   = int((val + std - min_value) * y_alpha)
                 dev_down_y1 = int((val - std - min_value) * y_alpha)
                 center_x = x1 + (x_alpha / 2)
-                p.drawLine(center_x, plot_height - dev_up_y1, center_x, plot_height - dev_down_y1)
-                p.drawLine(center_x + 1, plot_height - dev_up_y1, center_x -1, plot_height - dev_up_y1)
-                p.drawLine(center_x + 1, plot_height - dev_down_y1, center_x -1, plot_height - dev_down_y1)
+                p.drawLine(QLineF(center_x, plot_height - dev_up_y1, center_x, plot_height - dev_down_y1))
+                p.drawLine(QLineF(center_x + 1, plot_height - dev_up_y1, center_x -1, plot_height - dev_up_y1))
+                p.drawLine(QLineF(center_x + 1, plot_height - dev_down_y1, center_x -1, plot_height - dev_down_y1))
 
 
 
 class QGraphicsTriangleItem(QGraphicsPolygonItem):
     def __init__(self, width, height, orientation=1):
         self.tri = QPolygonF()
         if orientation == 1:
@@ -1613,28 +1613,28 @@
         blackPen = QPen(QColor("black"))
         for letter in self.seq:
             letter = letter.upper()
             if x >= current_pixel:
                 if self.draw_text and self.poswidth >= 8:
                     br = QBrush(QColor(self.bg.get(letter, "white")))
                     p.setPen(blackPen)
-                    p.fillRect(x, 0, self.poswidth, self.posheight, br)
+                    p.fillRect(QRectF(x, 0, self.poswidth, self.posheight), br)
                     qfont.setPixelSize(min(self.posheight, self.poswidth))
                     p.setFont(qfont)
                     p.setBrush(QBrush(QColor("black")))
-                    p.drawText(x, 0, self.poswidth, self.posheight,
+                    p.drawText(QRectF(x, 0, self.poswidth, self.posheight),
                                Qt.AlignCenter |  Qt.AlignVCenter,
                                letter)
                 elif letter == "-" or letter == ".":
                     p.setPen(blackPen)
-                    p.drawLine(x, self.posheight/2, x+self.poswidth, self.posheight/2)
+                    p.drawLine(QLineF(x, self.posheight/2, x+self.poswidth, self.posheight/2))
 
                 else:
                     br = QBrush(QColor(self.bg.get(letter, "white")))
-                    p.fillRect(x, 0, max(1, self.poswidth), self.posheight, br)
+                    p.fillRect(QRectF(x, 0, max(1, self.poswidth), self.posheight), br)
                     #p.setPen(QPen(QColor(self.bg.get(letter, "black"))))
                     #p.drawLine(x, 0, x, self.posheight)
                 current_pixel = int(x)
             x += self.poswidth
 
 
 class TextLabelItem(QGraphicsRectItem):
@@ -2416,7 +2416,72 @@
 
     def _width(self):
         return self.width
 
     def _height(self):
         return self.height
 
+
+class ArrowFace(Face):
+
+    """
+
+    Creates a color-stripped arrow representation for synteny visualization
+
+    :param width: width of the arrow (min of 10)
+    :param height: height of arrow (min of 10)
+    :param strand: defines gene orientation. "-" entails left-oriented arrows
+                   while "+" strand right-oriented arrows.
+    :param colors: array containing values to color stripes
+
+    """
+
+    def __init__(self, width, height, strand, colors):
+        Face.__init__(self)
+        self.width = width
+        self.height = height
+        self.strand = strand
+        self.colors = colors
+
+    def _width(self):
+        return self.width
+
+    def _height(self):
+        return self.height
+
+    def update_items(self):
+        return
+
+    def update_pixmap(self):
+        # Create pixmap
+        self.pixmap = QPixmap(self.width, self.height)
+        self.pixmap.fill(QColor("white"))
+        p = QPainter(self.pixmap)
+
+        # Create pen
+        solidPen = QPen(QBrush(QColor("black")), 0)
+        solidPen.setStyle(Qt.SolidLine)
+        p.setPen(solidPen)
+
+        # Define bands width and arrow height taking padding into account
+        rect_w = (self.width - 10) / len(self.colors)
+        rect_h = self.height - 10
+
+        # Draw each of the color bands and the arrow pointer depending on the
+        # strand (+,right/-,left)
+        for i, color in enumerate(self.colors):
+            if self.strand == "+":
+                p.fillRect(3 + i*rect_w, 5, math.ceil(rect_w), rect_h, QColor(color))
+                if i == (len(self.colors) - 1):
+                    path = QPainterPath()
+                    path.moveTo(3+(i+1)*rect_w, 5)
+                    path.lineTo(7+(i+1)*rect_w, 5+rect_h / 2)
+                    path.lineTo(3+(i+1)*rect_w, 5+rect_h)
+                    p.fillPath(path, QColor(color))
+            elif self.strand == "-":
+                p.fillRect(7 + i*rect_w, 5, math.ceil(rect_w), rect_h, QColor(color))
+                if i == 0:
+                    path = QPainterPath()
+                    path.moveTo(7, 5)
+                    path.lineTo(3, 5+rect_h / 2)
+                    path.lineTo(7, 5+rect_h)
+                    p.fillPath(path, QColor(color))
```

### Comparing `ete3-3.1.2/ete3/treeview/clean_search.png` & `ete3-3.1.3/ete3/treeview/clean_search.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/treeview/_show_codeml.py` & `ete3-3.1.3/ete3/treeview/_show_codeml.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/treeview/open_newick.ui` & `ete3-3.1.3/ete3/treeview/open_newick.ui`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/treeview/qt4_render.py` & `ete3-3.1.3/ete3/treeview/qt4_render.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/treeview/qt4_rect_render.py` & `ete3-3.1.3/ete3/treeview/qt4_rect_render.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_xml_parsers.py` & `ete3-3.1.3/ete3/test/test_xml_parsers.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_circle_label.py` & `ete3-3.1.3/ete3/test/test_circle_label.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_issue258/issue258.py` & `ete3-3.1.3/ete3/test/test_issue258/issue258.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_arraytable.py` & `ete3-3.1.3/ete3/test/test_arraytable.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_ete_evol.py` & `ete3-3.1.3/ete3/test/test_ete_evol.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_phylotree.py` & `ete3-3.1.3/ete3/test/test_phylotree.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_evol.py` & `ete3-3.1.3/ete3/test/test_evol.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/L_example/alignment_L_measuring_evol.fasta` & `ete3-3.1.3/examples/evol/data/L_example/alignment_L_measuring_evol.fasta`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/M1/out` & `ete3-3.1.3/examples/evol/data/S_example/paml/M1/out`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/M1/tmp.ctl` & `ete3-3.1.3/examples/evol/data/S_example/paml/M1/tmp.ctl`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/M1/lnf` & `ete3-3.1.3/examples/evol/data/S_example/paml/M1/lnf`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/M1/rst` & `ete3-3.1.3/examples/evol/data/S_example/paml/M1/rst`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/M1/algn` & `ete3-3.1.3/examples/evol/data/S_example/paml/M1/algn`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/fb/out` & `ete3-3.1.3/examples/evol/data/S_example/paml/fb/out`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/fb/rst1` & `ete3-3.1.3/examples/evol/data/S_example/paml/fb/rst1`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/fb/tmp.ctl` & `ete3-3.1.3/examples/evol/data/S_example/paml/fb/tmp.ctl`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/fb/lnf` & `ete3-3.1.3/examples/evol/data/S_example/paml/fb/lnf`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/fb/rst` & `ete3-3.1.3/examples/evol/data/S_example/paml/fb/rst`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/fb/algn` & `ete3-3.1.3/examples/evol/data/S_example/paml/M2/algn`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/bsA1/out` & `ete3-3.1.3/examples/evol/data/S_example/paml/bsA1/out`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/bsA1/tmp.ctl` & `ete3-3.1.3/examples/evol/data/S_example/paml/bsA1/tmp.ctl`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/bsA1/lnf` & `ete3-3.1.3/examples/evol/data/S_example/paml/bsA1/lnf`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/bsA1/rst` & `ete3-3.1.3/examples/evol/data/S_example/paml/bsA1/rst`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/bsA1/algn` & `ete3-3.1.3/examples/evol/data/S_example/paml/bsA/algn`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/M2/out` & `ete3-3.1.3/examples/evol/data/S_example/paml/M2/out`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/M2/tmp.ctl` & `ete3-3.1.3/examples/evol/data/S_example/paml/M2/tmp.ctl`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/M2/lnf` & `ete3-3.1.3/examples/evol/data/S_example/paml/M2/lnf`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/M2/rst` & `ete3-3.1.3/examples/evol/data/S_example/paml/M2/rst`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/M2/algn` & `ete3-3.1.3/examples/evol/data/S_example/paml/bsA1/algn`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/bsA/out` & `ete3-3.1.3/examples/evol/data/S_example/paml/bsA/out`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/bsA/tmp.ctl` & `ete3-3.1.3/examples/evol/data/S_example/paml/bsA/tmp.ctl`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/bsA/lnf` & `ete3-3.1.3/examples/evol/data/S_example/paml/bsA/lnf`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/bsA/rst` & `ete3-3.1.3/examples/evol/data/S_example/paml/bsA/rst`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/S_example/paml/bsA/algn` & `ete3-3.1.3/examples/evol/data/S_example/paml/fb/algn`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/S_example/ali.fasta` & `ete3-3.1.3/examples/evol/data/S_example/alignment_S_measuring_evol.fasta`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/CladeModelCD/ECP_EDN_15.fasta` & `ete3-3.1.3/examples/evol/data/CladeModelCD/ECP_EDN_15.fasta`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/slr/tree` & `ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M1/tree`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/slr/fb.out` & `ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/fb/fb.out`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/slr/4fold.nuc` & `ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M1/4fold.nuc`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/slr/lnf` & `ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/fb/lnf`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/slr/algn` & `ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M1/algn`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/tree.nw` & `ete3-3.1.3/examples/evol/data/protamine/PRM1/tree.nw`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M0/2NG.t` & `ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M0/2NG.t`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M0/tree` & `ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M0/tree`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M0/out` & `ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M0/out`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M0/4fold.nuc` & `ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M0/4fold.nuc`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M0/2NG.dS` & `ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M0/2NG.dS`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M0/rst1` & `ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M0/rst1`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M0/lnf` & `ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M0/lnf`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M0/2NG.dN` & `ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M0/2NG.dN`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M0/algn` & `ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M0/algn`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M1/tree` & `ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M2/tree`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M1/M1.out` & `ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M1/M1.out`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M1/4fold.nuc` & `ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M2/4fold.nuc`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M1/lnf` & `ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M1/lnf`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M1/rst` & `ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M1/rst`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M1/algn` & `ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M2/algn`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M8/tree` & `ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M7/tree`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M8/4fold.nuc` & `ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M7/4fold.nuc`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M8/lnf` & `ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M8/lnf`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M8/rst` & `ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M8/rst`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M8/M8.out` & `ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M8/M8.out`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M8/algn` & `ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M7/algn`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/fb/tree` & `ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M8/tree`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/fb/fb.out` & `ete3-3.1.3/examples/evol/data/protamine/PRM1/slr/fb.out`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/fb/4fold.nuc` & `ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M8/4fold.nuc`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/fb/lnf` & `ete3-3.1.3/examples/evol/data/protamine/PRM1/slr/lnf`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/fb/algn` & `ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M8/algn`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M7/tree` & `ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/fb/tree`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M7/4fold.nuc` & `ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/fb/4fold.nuc`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M7/M7.out` & `ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M7/M7.out`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M7/lnf` & `ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M7/lnf`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M7/rst` & `ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M7/rst`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M7/algn` & `ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/fb/algn`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M2/tree` & `ete3-3.1.3/examples/evol/data/protamine/PRM1/slr/tree`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M2/4fold.nuc` & `ete3-3.1.3/examples/evol/data/protamine/PRM1/slr/4fold.nuc`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M2/lnf` & `ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M2/lnf`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M2/rst` & `ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M2/rst`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M2/M2.out` & `ete3-3.1.3/examples/evol/data/protamine/PRM1/paml/M2/M2.out`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/paml/M2/algn` & `ete3-3.1.3/examples/evol/data/protamine/PRM1/slr/algn`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/ete_evol_data/protamine/PRM1/alignments.fasta_ali` & `ete3-3.1.3/examples/evol/data/protamine/PRM1/alignments.fasta_ali`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_seqgroup.py` & `ete3-3.1.3/ete3/test/test_seqgroup.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_treeview/fish.png` & `ete3-3.1.3/examples/treeview/img_faces/fish.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_treeview/img_faces.png` & `ete3-3.1.3/examples/treeview/img_faces/img_faces.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_treeview/node_style.png` & `ete3-3.1.3/examples/treeview/node_style.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_treeview/test_all_treeview.py` & `ete3-3.1.3/ete3/test/test_treeview/test_all_treeview.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_treeview/face_grid.py` & `ete3-3.1.3/ete3/test/test_treeview/face_grid.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_treeview/node_style.py` & `ete3-3.1.3/ete3/test/test_treeview/node_style.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_treeview/chimp.png` & `ete3-3.1.3/examples/treeview/img_faces/chimp.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_treeview/face_positions.py` & `ete3-3.1.3/ete3/test/test_treeview/face_positions.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_treeview/seq_motif_faces.png` & `ete3-3.1.3/ete3/test/test_treeview/seq_motif_faces.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_treeview/dog.png` & `ete3-3.1.3/examples/treeview/img_faces/dog.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_treeview/human.png` & `ete3-3.1.3/examples/treeview/img_faces/human.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_treeview/barcharts.png` & `ete3-3.1.3/examples/treeview/barcharts.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_treeview/motifs.png` & `ete3-3.1.3/ete3/test/test_treeview/motifs.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_treeview/bubble_map.png` & `ete3-3.1.3/examples/treeview/bubble_map.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_treeview/item_faces.py` & `ete3-3.1.3/ete3/test/test_treeview/item_faces.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_treeview/node_background.py` & `ete3-3.1.3/ete3/test/test_treeview/node_background.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_treeview/item_faces.png` & `ete3-3.1.3/examples/treeview/item_faces.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_treeview/float_piechart.png` & `ete3-3.1.3/examples/treeview/float_piechart.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_treeview/tree_faces.png` & `ete3-3.1.3/examples/treeview/tree_faces.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_treeview/tree_faces.py` & `ete3-3.1.3/ete3/test/test_treeview/tree_faces.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_treeview/seq_motif_faces.py` & `ete3-3.1.3/ete3/test/test_treeview/seq_motif_faces.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_treeview/barchart_and_piechart_faces.py` & `ete3-3.1.3/ete3/test/test_treeview/barchart_and_piechart_faces.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 import random
 from ... import Tree, faces, TreeStyle, COLOR_SCHEMES
 
-schema_names = COLOR_SCHEMES.keys()
+schema_names = sorted(COLOR_SCHEMES.keys())
 
 def layout(node):
     if node.is_leaf():
         F= faces.PieChartFace([10,10,10,10,10,10,10,10,10,4,6],
                               colors=COLOR_SCHEMES["set3"],
                               width=50, height=50)
         F.border.width = None
```

### Comparing `ete3-3.1.2/ete3/test/test_treeview/seqmotif.png` & `ete3-3.1.3/examples/treeview/seqmotif.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_treeview/new_seq_face.py` & `ete3-3.1.3/ete3/test/test_treeview/new_seq_face.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_treeview/fly.png` & `ete3-3.1.3/examples/treeview/img_faces/fly.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_treeview/phylotree_visualization.py` & `ete3-3.1.3/ete3/test/test_treeview/phylotree_visualization.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_treeview/rotated_faces.png` & `ete3-3.1.3/examples/treeview/rotated_faces.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_treeview/node_background.png` & `ete3-3.1.3/examples/treeview/node_background.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_treeview/face_rotation.py` & `ete3-3.1.3/ete3/test/test_treeview/face_rotation.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_treeview/mouse.png` & `ete3-3.1.3/examples/treeview/img_faces/mouse.png`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_treeview/bubble_map.py` & `ete3-3.1.3/ete3/test/test_treeview/bubble_map.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_treeview/img_faces.py` & `ete3-3.1.3/ete3/test/test_treeview/img_faces.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_treeview/floating_piecharts.py` & `ete3-3.1.3/ete3/test/test_treeview/floating_piecharts.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_treeview/random_draw.py` & `ete3-3.1.3/ete3/test/test_treeview/random_draw.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_tree.py` & `ete3-3.1.3/ete3/test/test_tree.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_ete_build/cog_seqs.nt.fa` & `ete3-3.1.3/ete3/test/test_ete_build/cog_seqs.nt.fa`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_ete_build/P53.fa` & `ete3-3.1.3/ete3/test/test_ete_build/P53.fa`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_ete_build/test_manual_alg.py` & `ete3-3.1.3/ete3/test/test_ete_build/test_manual_alg.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_ete_build/NUP62.nt.fa` & `ete3-3.1.3/ete3/test/test_ete_build/NUP62.nt.fa`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_ete_build/P53.alg.fa` & `ete3-3.1.3/ete3/test/test_ete_build/P53.alg.fa`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_ete_build/test_sptree.py` & `ete3-3.1.3/ete3/test/test_ete_build/test_sptree.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_ete_build/test_modeltest.py` & `ete3-3.1.3/ete3/test/test_ete_build/test_modeltest.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_ete_build/NUP62.aa.fa` & `ete3-3.1.3/ete3/test/test_ete_build/NUP62.aa.fa`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_ete_build/test_genetree.py` & `ete3-3.1.3/ete3/test/test_ete_build/test_genetree.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_interop.py` & `ete3-3.1.3/ete3/test/test_interop.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_ncbiquery.py` & `ete3-3.1.3/ete3/test/test_ncbiquery.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,21 +52,21 @@
 
     name2id = ncbi.get_name_translator(['Bacteria'])
     #self.assertEqual(set(name2id['Bacteria']), set([2, 629395]))
     # Recent versions of NCBI seem to have removed the name Bacteria from 629395
     self.assertEqual(set(name2id['Bacteria']), set([2]))
 
     out = ncbi.get_descendant_taxa("9605", intermediate_nodes=True)
-    #Out[9]: [9606, 63221, 741158, 2665952, 2665953, 1425170]
+    #Out[9]: [9606, 63221, 741158, 2665952, 2665953, 1425170, 2813598, 2813599]
     # New Taxonomies of Homo in NCBI, {2665952: 'environmental samples', 2665953: 'Homo sapiens environmental sample'}
-    self.assertEqual(set(out), set([9606, 63221, 741158, 2665952, 2665953, 1425170]))
+    self.assertEqual(set(out), set([9606, 63221, 741158, 2665952, 2665953, 1425170, 2813598, 2813599]))
     
     out = ncbi.get_descendant_taxa("9605", intermediate_nodes=False)
     #Out[10]: [63221, 741158, 2665953, 1425170]
-    self.assertEqual(set(out), set([63221, 741158, 2665953, 1425170]))
+    self.assertEqual(set(out), set([63221, 741158, 2665953, 1425170, 2813599]))
     
     out = ncbi.get_descendant_taxa("9596", intermediate_nodes=False, rank_limit="species")
     #Out[11]: [9597, 9598]
     self.assertEqual(set(out), set([9597, 9598]))
     
   def test_get_topology(self):
     ncbi = NCBITaxa(dbfile=DATABASE_PATH)
```

### Comparing `ete3-3.1.2/ete3/test/datasets.py` & `ete3-3.1.3/ete3/test/datasets.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/test/test_clustertree.py` & `ete3-3.1.3/ete3/test/test_clustertree.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/parser/__init__.py` & `ete3-3.1.3/ete3/coretype/__init__.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/parser/newick.py` & `ete3-3.1.3/ete3/parser/newick.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/parser/phylip.py` & `ete3-3.1.3/ete3/parser/phylip.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/parser/fasta.py` & `ete3-3.1.3/ete3/parser/fasta.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/parser/paml.py` & `ete3-3.1.3/ete3/parser/paml.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/parser/text_arraytable.py` & `ete3-3.1.3/ete3/parser/text_arraytable.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/orthoxml/__init__.py` & `ete3-3.1.3/ete3/orthoxml/__init__.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/orthoxml/_orthoxml.py` & `ete3-3.1.3/ete3/orthoxml/_orthoxml.py`

 * *Files 1% similar despite different names*

```diff
@@ -443,21 +443,21 @@
             showIndent(outfile, level)
             outfile.write('</%s%s>\n' % (namespace_, name_))
         else:
             outfile.write('/>\n')
     def exportAttributes(self, outfile, level, already_processed, namespace_='ortho:', name_='orthoXML'):
         if self.origin is not None and 'origin' not in already_processed:
             already_processed.append('origin')
-            outfile.write(' origin=%s' % (self.gds_format_string(quote_attrib(self.origin).encode(ExternalEncoding), input_name='origin'), ))
+            outfile.write(' origin=%s' % (self.gds_format_string(quote_attrib(self.origin), input_name='origin'), ))
         if self.version is not None and 'version' not in already_processed:
             already_processed.append('version')
             outfile.write(' version="%s"' % self.gds_format_float(self.version, input_name='version'))
         if self.originVersion is not None and 'originVersion' not in already_processed:
             already_processed.append('originVersion')
-            outfile.write(' originVersion=%s' % (self.gds_format_string(quote_attrib(self.originVersion).encode(ExternalEncoding), input_name='originVersion'), ))
+            outfile.write(' originVersion=%s' % (self.gds_format_string(quote_attrib(self.originVersion), input_name='originVersion'), ))
     def exportChildren(self, outfile, level, namespace_='ortho:', name_='orthoXML', fromsubclass_=False):
         if self.notes:
             self.notes.export(outfile, level, namespace_, name_='notes')
         for species_ in self.species:
             species_.export(outfile, level, namespace_, name_='species')
         if self.scores:
             self.scores.export(outfile, level, namespace_, name_='scores')
@@ -605,15 +605,15 @@
             showIndent(outfile, level)
             outfile.write('</%s%s>\n' % (namespace_, name_))
         else:
             outfile.write('/>\n')
     def exportAttributes(self, outfile, level, already_processed, namespace_='ortho:', name_='species'):
         if self.name is not None and 'name' not in already_processed:
             already_processed.append('name')
-            outfile.write(' name=%s' % (self.gds_format_string(quote_attrib(self.name).encode(ExternalEncoding), input_name='name'), ))
+            outfile.write(' name=%s' % (self.gds_format_string(quote_attrib(self.name), input_name='name'), ))
         if self.NCBITaxId is not None and 'NCBITaxId' not in already_processed:
             already_processed.append('NCBITaxId')
             outfile.write(' NCBITaxId="%s"' % self.gds_format_integer(self.NCBITaxId, input_name='NCBITaxId'))
     def exportChildren(self, outfile, level, namespace_='ortho:', name_='species', fromsubclass_=False):
         for database_ in self.database:
             database_.export(outfile, level, namespace_, name_='database')
         if self.notes:
@@ -736,27 +736,27 @@
             showIndent(outfile, level)
             outfile.write('</%s%s>\n' % (namespace_, name_))
         else:
             outfile.write('/>\n')
     def exportAttributes(self, outfile, level, already_processed, namespace_='ortho:', name_='database'):
         if self.transcriptLink is not None and 'transcriptLink' not in already_processed:
             already_processed.append('transcriptLink')
-            outfile.write(' transcriptLink=%s' % (self.gds_format_string(quote_attrib(self.transcriptLink).encode(ExternalEncoding), input_name='transcriptLink'), ))
+            outfile.write(' transcriptLink=%s' % (self.gds_format_string(quote_attrib(self.transcriptLink), input_name='transcriptLink'), ))
         if self.protLink is not None and 'protLink' not in already_processed:
             already_processed.append('protLink')
-            outfile.write(' protLink=%s' % (self.gds_format_string(quote_attrib(self.protLink).encode(ExternalEncoding), input_name='protLink'), ))
+            outfile.write(' protLink=%s' % (self.gds_format_string(quote_attrib(self.protLink), input_name='protLink'), ))
         if self.geneLink is not None and 'geneLink' not in already_processed:
             already_processed.append('geneLink')
-            outfile.write(' geneLink=%s' % (self.gds_format_string(quote_attrib(self.geneLink).encode(ExternalEncoding), input_name='geneLink'), ))
+            outfile.write(' geneLink=%s' % (self.gds_format_string(quote_attrib(self.geneLink), input_name='geneLink'), ))
         if self.name is not None and 'name' not in already_processed:
             already_processed.append('name')
-            outfile.write(' name=%s' % (self.gds_format_string(quote_attrib(self.name).encode(ExternalEncoding), input_name='name'), ))
+            outfile.write(' name=%s' % (self.gds_format_string(quote_attrib(self.name), input_name='name'), ))
         if self.version is not None and 'version' not in already_processed:
             already_processed.append('version')
-            outfile.write(' version=%s' % (self.gds_format_string(quote_attrib(self.version).encode(ExternalEncoding), input_name='version'), ))
+            outfile.write(' version=%s' % (self.gds_format_string(quote_attrib(self.version), input_name='version'), ))
     def exportChildren(self, outfile, level, namespace_='ortho:', name_='database', fromsubclass_=False):
         if self.genes:
             self.genes.export(outfile, level, namespace_, name_='genes', )
     def hasContent_(self):
         if (
             self.genes is not None
             ):
@@ -958,24 +958,24 @@
             self.exportChildren(outfile, level + 1, namespace_, name_)
             outfile.write('</%s%s>\n' % (namespace_, name_))
         else:
             outfile.write('/>\n')
     def exportAttributes(self, outfile, level, already_processed, namespace_='ortho:', name_='gene'):
         if self.protId is not None and 'protId' not in already_processed:
             already_processed.append('protId')
-            outfile.write(' protId=%s' % (self.gds_format_string(quote_attrib(self.protId).encode(ExternalEncoding), input_name='protId'), ))
+            outfile.write(' protId=%s' % (self.gds_format_string(quote_attrib(self.protId), input_name='protId'), ))
         if self.id is not None and 'id' not in already_processed:
             already_processed.append('id')
             outfile.write(' id="%s"' % self.gds_format_integer(self.id, input_name='id'))
         if self.geneId is not None and 'geneId' not in already_processed:
             already_processed.append('geneId')
-            outfile.write(' geneId=%s' % (self.gds_format_string(quote_attrib(self.geneId).encode(ExternalEncoding), input_name='geneId'), ))
+            outfile.write(' geneId=%s' % (self.gds_format_string(quote_attrib(self.geneId), input_name='geneId'), ))
         if self.transcriptId is not None and 'transcriptId' not in already_processed:
             already_processed.append('transcriptId')
-            outfile.write(' transcriptId=%s' % (self.gds_format_string(quote_attrib(self.transcriptId).encode(ExternalEncoding), input_name='transcriptId'), ))
+            outfile.write(' transcriptId=%s' % (self.gds_format_string(quote_attrib(self.transcriptId), input_name='transcriptId'), ))
     def exportChildren(self, outfile, level, namespace_='ortho:', name_='gene', fromsubclass_=False):
         pass
     def hasContent_(self):
         if (
 
             ):
             return True
@@ -1273,15 +1273,15 @@
             showIndent(outfile, level)
             outfile.write('</%s%s>\n' % (namespace_, name_))
         else:
             outfile.write('/>\n')
     def exportAttributes(self, outfile, level, already_processed, namespace_='ortho:', name_='group'):
         if self.id is not None and 'id' not in already_processed:
             already_processed.append('id')
-            outfile.write(' id=%s' % (self.gds_format_string(quote_attrib(self.id).encode(ExternalEncoding), input_name='id'), ))
+            outfile.write(' id=%s' % (self.gds_format_string(quote_attrib(self.id), input_name='id'), ))
     def exportChildren(self, outfile, level, namespace_='ortho:', name_='group', fromsubclass_=False):
         for score_ in self.score:
             score_.export(outfile, level, namespace_, name_='score')
         for property_ in self.property:
             property_.export(outfile, level, namespace_, name_='property')
         for geneRef_ in self.geneRef:
             geneRef_.export(outfile, level, namespace_, name_='geneRef')
@@ -1572,15 +1572,15 @@
             outfile.write('/>\n')
     def exportAttributes(self, outfile, level, already_processed, namespace_='ortho:', name_='scoreDef'):
         if self.id is not None and 'id' not in already_processed:
             already_processed.append('id')
             outfile.write(' id=%s' % (quote_attrib(self.id), ))
         if self.desc is not None and 'desc' not in already_processed:
             already_processed.append('desc')
-            outfile.write(' desc=%s' % (self.gds_format_string(quote_attrib(self.desc).encode(ExternalEncoding), input_name='desc'), ))
+            outfile.write(' desc=%s' % (self.gds_format_string(quote_attrib(self.desc), input_name='desc'), ))
     def exportChildren(self, outfile, level, namespace_='ortho:', name_='scoreDef', fromsubclass_=False):
         pass
     def hasContent_(self):
         if (
 
             ):
             return True
@@ -1740,18 +1740,18 @@
             self.exportChildren(outfile, level + 1, namespace_, name_)
             outfile.write('</%s%s>\n' % (namespace_, name_))
         else:
             outfile.write('/>\n')
     def exportAttributes(self, outfile, level, already_processed, namespace_='ortho:', name_='property'):
         if self.name is not None and 'name' not in already_processed:
             already_processed.append('name')
-            outfile.write(' name=%s' % (self.gds_format_string(quote_attrib(self.name).encode(ExternalEncoding), input_name='name'), ))
+            outfile.write(' name=%s' % (self.gds_format_string(quote_attrib(self.name), input_name='name'), ))
         if self.value is not None and 'value' not in already_processed:
             already_processed.append('value')
-            outfile.write(' value=%s' % (self.gds_format_string(quote_attrib(self.value).encode(ExternalEncoding), input_name='value'), ))
+            outfile.write(' value=%s' % (self.gds_format_string(quote_attrib(self.value), input_name='value'), ))
     def exportChildren(self, outfile, level, namespace_='ortho:', name_='property', fromsubclass_=False):
         pass
     def hasContent_(self):
         if (
 
             ):
             return True
```

### Comparing `ete3-3.1.2/ete3/phylo/__init__.py` & `ete3-3.1.3/ete3/phylo/__init__.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/phylo/phylotree.py` & `ete3-3.1.3/ete3/phylo/phylotree.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/phylo/reconciliation.py` & `ete3-3.1.3/ete3/phylo/reconciliation.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/phylo/evolevents.py` & `ete3-3.1.3/ete3/phylo/evolevents.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/phylo/spoverlap.py` & `ete3-3.1.3/ete3/phylo/spoverlap.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/phylomedb/__init__.py` & `ete3-3.1.3/ete3/phylomedb/__init__.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/phylomedb/phylomeDB.py` & `ete3-3.1.3/ete3/phylomedb/phylomeDB.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/phylomedb/phylomeDB3.py` & `ete3-3.1.3/ete3/phylomedb/phylomeDB3.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/citation.py` & `ete3-3.1.3/ete3/citation.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/coretype/arraytable.py` & `ete3-3.1.3/ete3/coretype/arraytable.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/coretype/__init__.py` & `ete3-3.1.3/ete3/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/coretype/tree.py` & `ete3-3.1.3/ete3/coretype/tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -1654,15 +1654,15 @@
 
         :param name attr_t1: Compare trees using a custom node
                               attribute as a node name.
 
         :param name attr_t2: Compare trees using a custom node
                               attribute as a node name in target tree.
 
-        :param False attr_t2: If True, consider trees as unrooted.
+        :param False unrooted_trees: If True, consider trees as unrooted.
 
         :param False expand_polytomies: If True, all polytomies in the reference
            and target tree will be expanded into all possible binary
            trees. Robinson-foulds distance will be calculated between all
            tree combinations and the minimum value will be returned.
            See also, :func:`NodeTree.expand_polytomy`.
```

### Comparing `ete3-3.1.2/ete3/coretype/seqgroup.py` & `ete3-3.1.3/ete3/coretype/seqgroup.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/utils.py` & `ete3-3.1.3/ete3/utils.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/webplugin/__init__.py` & `ete3-3.1.3/ete3/webplugin/__init__.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ete3/webplugin/webapp.py` & `ete3-3.1.3/ete3/webplugin/webapp.py`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/LICENSE` & `ete3-3.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ete3-3.1.2/ez_setup.py` & `ete3-3.1.3/ez_setup.py`

 * *Files identical despite different names*

