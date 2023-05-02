# Comparing `tmp/fake-bpy-module-latest-20230430.tar.gz` & `tmp/fake-bpy-module-latest-20230501.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fake-bpy-module-latest-20230430.tar", last modified: Sun Apr 30 06:21:34 2023, max compression
+gzip compressed data, was "dist/fake-bpy-module-latest-20230501.tar", last modified: Mon May  1 06:23:05 2023, max compression
```

## Comparing `fake-bpy-module-latest-20230430.tar` & `fake-bpy-module-latest-20230501.tar`

### file list

```diff
@@ -1,352 +1,352 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/
--rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-04-30 06:21:33.000000 fake-bpy-module-latest-20230430/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-30 06:19:34.000000 fake-bpy-module-latest-20230430/addon_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-30 06:21:31.000000 fake-bpy-module-latest-20230430/animsys_refactor.py
--rw-r--r--   0 runner    (1001) docker     (123)    31249 2023-04-30 06:19:30.000000 fake-bpy-module-latest-20230430/aud.py
--rw-r--r--   0 runner    (1001) docker     (123)   116266 2023-04-30 06:19:27.000000 fake-bpy-module-latest-20230430/bgl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/bl_app_override/
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-30 06:19:34.000000 fake-bpy-module-latest-20230430/bl_app_override/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-30 06:19:34.000000 fake-bpy-module-latest-20230430/bl_app_override/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/bl_app_override/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-30 06:21:31.000000 fake-bpy-module-latest-20230430/bl_app_template_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/bl_console_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-30 06:21:31.000000 fake-bpy-module-latest-20230430/bl_console_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/bl_console_utils/autocomplete/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-30 06:21:31.000000 fake-bpy-module-latest-20230430/bl_console_utils/autocomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-30 06:21:31.000000 fake-bpy-module-latest-20230430/bl_console_utils/autocomplete/complete_calltip.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-30 06:21:31.000000 fake-bpy-module-latest-20230430/bl_console_utils/autocomplete/complete_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-30 06:21:31.000000 fake-bpy-module-latest-20230430/bl_console_utils/autocomplete/complete_namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-30 06:21:31.000000 fake-bpy-module-latest-20230430/bl_console_utils/autocomplete/intellisense.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/bl_console_utils/autocomplete/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/bl_console_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/bl_i18n_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-30 06:19:34.000000 fake-bpy-module-latest-20230430/bl_i18n_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-30 06:19:34.000000 fake-bpy-module-latest-20230430/bl_i18n_utils/bl_extract_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-30 06:19:34.000000 fake-bpy-module-latest-20230430/bl_i18n_utils/merge_po.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/bl_i18n_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-30 06:19:34.000000 fake-bpy-module-latest-20230430/bl_i18n_utils/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-30 06:19:34.000000 fake-bpy-module-latest-20230430/bl_i18n_utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-30 06:19:34.000000 fake-bpy-module-latest-20230430/bl_i18n_utils/utils_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-30 06:19:34.000000 fake-bpy-module-latest-20230430/bl_i18n_utils/utils_languages_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-30 06:19:34.000000 fake-bpy-module-latest-20230430/bl_i18n_utils/utils_rtl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/bl_keymap_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-30 06:21:31.000000 fake-bpy-module-latest-20230430/bl_keymap_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-30 06:21:31.000000 fake-bpy-module-latest-20230430/bl_keymap_utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-30 06:21:31.000000 fake-bpy-module-latest-20230430/bl_keymap_utils/keymap_from_toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-30 06:21:31.000000 fake-bpy-module-latest-20230430/bl_keymap_utils/keymap_hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-30 06:21:31.000000 fake-bpy-module-latest-20230430/bl_keymap_utils/platform_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/bl_keymap_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-30 06:21:31.000000 fake-bpy-module-latest-20230430/bl_keymap_utils/versioning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-30 06:19:33.000000 fake-bpy-module-latest-20230430/bl_math.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/bl_operators/
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-30 06:19:34.000000 fake-bpy-module-latest-20230430/bl_operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-30 06:19:40.000000 fake-bpy-module-latest-20230430/bl_operators/add_mesh_torus.py
--rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-04-30 06:19:39.000000 fake-bpy-module-latest-20230430/bl_operators/anim.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-04-30 06:19:39.000000 fake-bpy-module-latest-20230430/bl_operators/assets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/bl_operators/bmesh/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-30 06:19:37.000000 fake-bpy-module-latest-20230430/bl_operators/bmesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-30 06:19:37.000000 fake-bpy-module-latest-20230430/bl_operators/bmesh/find_adjacent.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/bl_operators/bmesh/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22556 2023-04-30 06:19:39.000000 fake-bpy-module-latest-20230430/bl_operators/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-04-30 06:19:35.000000 fake-bpy-module-latest-20230430/bl_operators/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-04-30 06:19:35.000000 fake-bpy-module-latest-20230430/bl_operators/constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-04-30 06:19:39.000000 fake-bpy-module-latest-20230430/bl_operators/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-04-30 06:19:37.000000 fake-bpy-module-latest-20230430/bl_operators/freestyle.py
--rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-04-30 06:19:39.000000 fake-bpy-module-latest-20230430/bl_operators/geometry_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-04-30 06:19:35.000000 fake-bpy-module-latest-20230430/bl_operators/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-04-30 06:19:37.000000 fake-bpy-module-latest-20230430/bl_operators/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-04-30 06:19:35.000000 fake-bpy-module-latest-20230430/bl_operators/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    38053 2023-04-30 06:19:37.000000 fake-bpy-module-latest-20230430/bl_operators/object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-30 06:19:39.000000 fake-bpy-module-latest-20230430/bl_operators/object_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-04-30 06:19:38.000000 fake-bpy-module-latest-20230430/bl_operators/object_quick_effects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-30 06:19:38.000000 fake-bpy-module-latest-20230430/bl_operators/object_randomize_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    42973 2023-04-30 06:19:34.000000 fake-bpy-module-latest-20230430/bl_operators/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/bl_operators/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-04-30 06:19:38.000000 fake-bpy-module-latest-20230430/bl_operators/rigidbody.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-30 06:19:35.000000 fake-bpy-module-latest-20230430/bl_operators/screen_play_rendered_anim.py
--rw-r--r--   0 runner    (1001) docker     (123)    12099 2023-04-30 06:19:37.000000 fake-bpy-module-latest-20230430/bl_operators/sequencer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-30 06:19:39.000000 fake-bpy-module-latest-20230430/bl_operators/spreadsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    56119 2023-04-30 06:19:38.000000 fake-bpy-module-latest-20230430/bl_operators/userpref.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-04-30 06:19:39.000000 fake-bpy-module-latest-20230430/bl_operators/uvcalc_follow_active.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-04-30 06:19:39.000000 fake-bpy-module-latest-20230430/bl_operators/uvcalc_lightmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-04-30 06:19:39.000000 fake-bpy-module-latest-20230430/bl_operators/uvcalc_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-30 06:19:37.000000 fake-bpy-module-latest-20230430/bl_operators/vertexpaint_dirt.py
--rw-r--r--   0 runner    (1001) docker     (123)    11529 2023-04-30 06:19:39.000000 fake-bpy-module-latest-20230430/bl_operators/view3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    97916 2023-04-30 06:19:36.000000 fake-bpy-module-latest-20230430/bl_operators/wm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/bl_previews_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-30 06:19:40.000000 fake-bpy-module-latest-20230430/bl_previews_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-30 06:19:40.000000 fake-bpy-module-latest-20230430/bl_previews_utils/bl_previews_render.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/bl_previews_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/bl_rna_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-30 06:21:31.000000 fake-bpy-module-latest-20230430/bl_rna_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-30 06:21:31.000000 fake-bpy-module-latest-20230430/bl_rna_utils/data_path.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/bl_rna_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/bl_ui/
--rw-r--r--   0 runner    (1001) docker     (123)    10201 2023-04-30 06:19:41.000000 fake-bpy-module-latest-20230430/bl_ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-04-30 06:20:29.000000 fake-bpy-module-latest-20230430/bl_ui/generic_ui_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-30 06:21:29.000000 fake-bpy-module-latest-20230430/bl_ui/node_add_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)   108259 2023-04-30 06:19:55.000000 fake-bpy-module-latest-20230430/bl_ui/node_add_menu_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-30 06:20:40.000000 fake-bpy-module-latest-20230430/bl_ui/properties_animviz.py
--rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-04-30 06:19:48.000000 fake-bpy-module-latest-20230430/bl_ui/properties_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)   385296 2023-04-30 06:20:14.000000 fake-bpy-module-latest-20230430/bl_ui/properties_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)    25330 2023-04-30 06:19:48.000000 fake-bpy-module-latest-20230430/bl_ui/properties_data_armature.py
--rw-r--r--   0 runner    (1001) docker     (123)    22602 2023-04-30 06:20:39.000000 fake-bpy-module-latest-20230430/bl_ui/properties_data_bone.py
--rw-r--r--   0 runner    (1001) docker     (123)    36945 2023-04-30 06:19:43.000000 fake-bpy-module-latest-20230430/bl_ui/properties_data_camera.py
--rw-r--r--   0 runner    (1001) docker     (123)    38857 2023-04-30 06:20:41.000000 fake-bpy-module-latest-20230430/bl_ui/properties_data_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)    15423 2023-04-30 06:20:29.000000 fake-bpy-module-latest-20230430/bl_ui/properties_data_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-04-30 06:20:37.000000 fake-bpy-module-latest-20230430/bl_ui/properties_data_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)    46403 2023-04-30 06:20:39.000000 fake-bpy-module-latest-20230430/bl_ui/properties_data_gpencil.py
--rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-04-30 06:20:41.000000 fake-bpy-module-latest-20230430/bl_ui/properties_data_lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-04-30 06:20:15.000000 fake-bpy-module-latest-20230430/bl_ui/properties_data_light.py
--rw-r--r--   0 runner    (1001) docker     (123)    12933 2023-04-30 06:20:27.000000 fake-bpy-module-latest-20230430/bl_ui/properties_data_lightprobe.py
--rw-r--r--   0 runner    (1001) docker     (123)    57510 2023-04-30 06:20:28.000000 fake-bpy-module-latest-20230430/bl_ui/properties_data_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-04-30 06:19:58.000000 fake-bpy-module-latest-20230430/bl_ui/properties_data_metaball.py
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-04-30 06:20:28.000000 fake-bpy-module-latest-20230430/bl_ui/properties_data_modifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    13050 2023-04-30 06:19:58.000000 fake-bpy-module-latest-20230430/bl_ui/properties_data_pointcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-30 06:20:29.000000 fake-bpy-module-latest-20230430/bl_ui/properties_data_shaderfx.py
--rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-04-30 06:20:38.000000 fake-bpy-module-latest-20230430/bl_ui/properties_data_speaker.py
--rw-r--r--   0 runner    (1001) docker     (123)    20178 2023-04-30 06:20:39.000000 fake-bpy-module-latest-20230430/bl_ui/properties_data_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    66640 2023-04-30 06:21:31.000000 fake-bpy-module-latest-20230430/bl_ui/properties_freestyle.py
--rw-r--r--   0 runner    (1001) docker     (123)    32219 2023-04-30 06:19:57.000000 fake-bpy-module-latest-20230430/bl_ui/properties_grease_pencil_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-04-30 06:21:31.000000 fake-bpy-module-latest-20230430/bl_ui/properties_mask_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    30514 2023-04-30 06:20:42.000000 fake-bpy-module-latest-20230430/bl_ui/properties_material.py
--rw-r--r--   0 runner    (1001) docker     (123)    25892 2023-04-30 06:20:29.000000 fake-bpy-module-latest-20230430/bl_ui/properties_material_gpencil.py
--rw-r--r--   0 runner    (1001) docker     (123)    35174 2023-04-30 06:20:40.000000 fake-bpy-module-latest-20230430/bl_ui/properties_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    46745 2023-04-30 06:19:43.000000 fake-bpy-module-latest-20230430/bl_ui/properties_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-04-30 06:20:38.000000 fake-bpy-module-latest-20230430/bl_ui/properties_paint_common.py
--rw-r--r--   0 runner    (1001) docker     (123)   133597 2023-04-30 06:20:26.000000 fake-bpy-module-latest-20230430/bl_ui/properties_particle.py
--rw-r--r--   0 runner    (1001) docker     (123)    36563 2023-04-30 06:20:23.000000 fake-bpy-module-latest-20230430/bl_ui/properties_physics_cloth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-30 06:20:28.000000 fake-bpy-module-latest-20230430/bl_ui/properties_physics_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    67584 2023-04-30 06:21:29.000000 fake-bpy-module-latest-20230430/bl_ui/properties_physics_dynamicpaint.py
--rw-r--r--   0 runner    (1001) docker     (123)    27217 2023-04-30 06:20:38.000000 fake-bpy-module-latest-20230430/bl_ui/properties_physics_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    91307 2023-04-30 06:19:42.000000 fake-bpy-module-latest-20230430/bl_ui/properties_physics_fluid.py
--rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-04-30 06:20:14.000000 fake-bpy-module-latest-20230430/bl_ui/properties_physics_rigidbody.py
--rw-r--r--   0 runner    (1001) docker     (123)    33547 2023-04-30 06:19:58.000000 fake-bpy-module-latest-20230430/bl_ui/properties_physics_rigidbody_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)    39030 2023-04-30 06:21:31.000000 fake-bpy-module-latest-20230430/bl_ui/properties_physics_softbody.py
--rw-r--r--   0 runner    (1001) docker     (123)    89468 2023-04-30 06:20:32.000000 fake-bpy-module-latest-20230430/bl_ui/properties_render.py
--rw-r--r--   0 runner    (1001) docker     (123)    32886 2023-04-30 06:21:30.000000 fake-bpy-module-latest-20230430/bl_ui/properties_scene.py
--rw-r--r--   0 runner    (1001) docker     (123)    66952 2023-04-30 06:20:33.000000 fake-bpy-module-latest-20230430/bl_ui/properties_texture.py
--rw-r--r--   0 runner    (1001) docker     (123)    37695 2023-04-30 06:20:27.000000 fake-bpy-module-latest-20230430/bl_ui/properties_view_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-04-30 06:21:31.000000 fake-bpy-module-latest-20230430/bl_ui/properties_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-04-30 06:19:42.000000 fake-bpy-module-latest-20230430/bl_ui/properties_world.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/bl_ui/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   174521 2023-04-30 06:19:48.000000 fake-bpy-module-latest-20230430/bl_ui/space_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)    15218 2023-04-30 06:20:31.000000 fake-bpy-module-latest-20230430/bl_ui/space_console.py
--rw-r--r--   0 runner    (1001) docker     (123)    62595 2023-04-30 06:20:41.000000 fake-bpy-module-latest-20230430/bl_ui/space_dopesheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    71853 2023-04-30 06:19:56.000000 fake-bpy-module-latest-20230430/bl_ui/space_filebrowser.py
--rw-r--r--   0 runner    (1001) docker     (123)    43433 2023-04-30 06:20:29.000000 fake-bpy-module-latest-20230430/bl_ui/space_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)   187053 2023-04-30 06:19:52.000000 fake-bpy-module-latest-20230430/bl_ui/space_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    15172 2023-04-30 06:20:30.000000 fake-bpy-module-latest-20230430/bl_ui/space_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    38361 2023-04-30 06:19:58.000000 fake-bpy-module-latest-20230430/bl_ui/space_nla.py
--rw-r--r--   0 runner    (1001) docker     (123)    65582 2023-04-30 06:19:44.000000 fake-bpy-module-latest-20230430/bl_ui/space_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    35830 2023-04-30 06:20:30.000000 fake-bpy-module-latest-20230430/bl_ui/space_outliner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-04-30 06:20:15.000000 fake-bpy-module-latest-20230430/bl_ui/space_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)   182398 2023-04-30 06:20:37.000000 fake-bpy-module-latest-20230430/bl_ui/space_sequencer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-04-30 06:20:14.000000 fake-bpy-module-latest-20230430/bl_ui/space_spreadsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-30 06:20:30.000000 fake-bpy-module-latest-20230430/bl_ui/space_statusbar.py
--rw-r--r--   0 runner    (1001) docker     (123)    40008 2023-04-30 06:20:15.000000 fake-bpy-module-latest-20230430/bl_ui/space_text.py
--rw-r--r--   0 runner    (1001) docker     (123)    18254 2023-04-30 06:21:29.000000 fake-bpy-module-latest-20230430/bl_ui/space_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-04-30 06:20:14.000000 fake-bpy-module-latest-20230430/bl_ui/space_toolsystem_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    21583 2023-04-30 06:20:42.000000 fake-bpy-module-latest-20230430/bl_ui/space_toolsystem_toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)    65863 2023-04-30 06:19:53.000000 fake-bpy-module-latest-20230430/bl_ui/space_topbar.py
--rw-r--r--   0 runner    (1001) docker     (123)   209844 2023-04-30 06:20:03.000000 fake-bpy-module-latest-20230430/bl_ui/space_userpref.py
--rw-r--r--   0 runner    (1001) docker     (123)   611242 2023-04-30 06:21:28.000000 fake-bpy-module-latest-20230430/bl_ui/space_view3d.py
--rw-r--r--   0 runner    (1001) docker     (123)   237261 2023-04-30 06:20:23.000000 fake-bpy-module-latest-20230430/bl_ui/space_view3d_toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-30 06:20:28.000000 fake-bpy-module-latest-20230430/bl_ui/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/bl_ui_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-30 06:19:34.000000 fake-bpy-module-latest-20230430/bl_ui_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-30 06:19:34.000000 fake-bpy-module-latest-20230430/bl_ui_utils/bug_report_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-30 06:19:34.000000 fake-bpy-module-latest-20230430/bl_ui_utils/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/bl_ui_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-30 06:19:34.000000 fake-bpy-module-latest-20230430/blend_render_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-04-30 06:19:27.000000 fake-bpy-module-latest-20230430/blf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/bmesh/
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-30 06:19:30.000000 fake-bpy-module-latest-20230430/bmesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-30 06:19:30.000000 fake-bpy-module-latest-20230430/bmesh/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    77491 2023-04-30 06:19:33.000000 fake-bpy-module-latest-20230430/bmesh/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/bmesh/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    37270 2023-04-30 06:19:30.000000 fake-bpy-module-latest-20230430/bmesh/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-04-30 06:19:30.000000 fake-bpy-module-latest-20230430/bmesh/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/bpy/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/bpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/bpy/app/
--rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-04-30 06:19:25.000000 fake-bpy-module-latest-20230430/bpy/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-04-30 06:19:25.000000 fake-bpy-module-latest-20230430/bpy/app/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-30 06:19:25.000000 fake-bpy-module-latest-20230430/bpy/app/icons.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/bpy/app/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-30 06:19:25.000000 fake-bpy-module-latest-20230430/bpy/app/timers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-04-30 06:19:25.000000 fake-bpy-module-latest-20230430/bpy/app/translations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-30 06:19:24.000000 fake-bpy-module-latest-20230430/bpy/msgbus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/bpy/ops/
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-30 06:18:43.000000 fake-bpy-module-latest-20230430/bpy/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27608 2023-04-30 06:18:57.000000 fake-bpy-module-latest-20230430/bpy/ops/action.py
--rw-r--r--   0 runner    (1001) docker     (123)    35270 2023-04-30 06:19:20.000000 fake-bpy-module-latest-20230430/bpy/ops/anim.py
--rw-r--r--   0 runner    (1001) docker     (123)    25130 2023-04-30 06:18:44.000000 fake-bpy-module-latest-20230430/bpy/ops/armature.py
--rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-04-30 06:19:21.000000 fake-bpy-module-latest-20230430/bpy/ops/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-04-30 06:18:44.000000 fake-bpy-module-latest-20230430/bpy/ops/boid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-04-30 06:18:53.000000 fake-bpy-module-latest-20230430/bpy/ops/brush.py
--rw-r--r--   0 runner    (1001) docker     (123)    12217 2023-04-30 06:19:04.000000 fake-bpy-module-latest-20230430/bpy/ops/buttons.py
--rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-04-30 06:19:10.000000 fake-bpy-module-latest-20230430/bpy/ops/cachefile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-04-30 06:19:05.000000 fake-bpy-module-latest-20230430/bpy/ops/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)    70010 2023-04-30 06:19:22.000000 fake-bpy-module-latest-20230430/bpy/ops/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-30 06:18:44.000000 fake-bpy-module-latest-20230430/bpy/ops/cloth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-30 06:19:15.000000 fake-bpy-module-latest-20230430/bpy/ops/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    12767 2023-04-30 06:19:13.000000 fake-bpy-module-latest-20230430/bpy/ops/console.py
--rw-r--r--   0 runner    (1001) docker     (123)    17809 2023-04-30 06:19:19.000000 fake-bpy-module-latest-20230430/bpy/ops/constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)    40490 2023-04-30 06:18:57.000000 fake-bpy-module-latest-20230430/bpy/ops/curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-04-30 06:19:03.000000 fake-bpy-module-latest-20230430/bpy/ops/curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-04-30 06:19:04.000000 fake-bpy-module-latest-20230430/bpy/ops/cycles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-30 06:18:52.000000 fake-bpy-module-latest-20230430/bpy/ops/dpaint.py
--rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-04-30 06:18:55.000000 fake-bpy-module-latest-20230430/bpy/ops/ed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-30 06:18:54.000000 fake-bpy-module-latest-20230430/bpy/ops/export_anim.py
--rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-04-30 06:19:24.000000 fake-bpy-module-latest-20230430/bpy/ops/export_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    40642 2023-04-30 06:19:12.000000 fake-bpy-module-latest-20230430/bpy/ops/export_scene.py
--rw-r--r--   0 runner    (1001) docker     (123)    30339 2023-04-30 06:19:24.000000 fake-bpy-module-latest-20230430/bpy/ops/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-04-30 06:19:07.000000 fake-bpy-module-latest-20230430/bpy/ops/fluid.py
--rw-r--r--   0 runner    (1001) docker     (123)    21051 2023-04-30 06:19:15.000000 fake-bpy-module-latest-20230430/bpy/ops/font.py
--rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-04-30 06:18:45.000000 fake-bpy-module-latest-20230430/bpy/ops/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-30 06:19:04.000000 fake-bpy-module-latest-20230430/bpy/ops/gizmogroup.py
--rw-r--r--   0 runner    (1001) docker     (123)   132520 2023-04-30 06:18:52.000000 fake-bpy-module-latest-20230430/bpy/ops/gpencil.py
--rw-r--r--   0 runner    (1001) docker     (123)    49736 2023-04-30 06:19:10.000000 fake-bpy-module-latest-20230430/bpy/ops/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    53280 2023-04-30 06:19:13.000000 fake-bpy-module-latest-20230430/bpy/ops/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-30 06:19:05.000000 fake-bpy-module-latest-20230430/bpy/ops/import_anim.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-30 06:19:05.000000 fake-bpy-module-latest-20230430/bpy/ops/import_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-04-30 06:19:16.000000 fake-bpy-module-latest-20230430/bpy/ops/import_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    14471 2023-04-30 06:18:55.000000 fake-bpy-module-latest-20230430/bpy/ops/import_scene.py
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-04-30 06:19:04.000000 fake-bpy-module-latest-20230430/bpy/ops/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-04-30 06:18:43.000000 fake-bpy-module-latest-20230430/bpy/ops/lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-04-30 06:18:53.000000 fake-bpy-module-latest-20230430/bpy/ops/marker.py
--rw-r--r--   0 runner    (1001) docker     (123)    26986 2023-04-30 06:19:15.000000 fake-bpy-module-latest-20230430/bpy/ops/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-30 06:18:57.000000 fake-bpy-module-latest-20230430/bpy/ops/material.py
--rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-04-30 06:19:04.000000 fake-bpy-module-latest-20230430/bpy/ops/mball.py
--rw-r--r--   0 runner    (1001) docker     (123)   182898 2023-04-30 06:19:19.000000 fake-bpy-module-latest-20230430/bpy/ops/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    28495 2023-04-30 06:19:16.000000 fake-bpy-module-latest-20230430/bpy/ops/nla.py
--rw-r--r--   0 runner    (1001) docker     (123)    67349 2023-04-30 06:19:15.000000 fake-bpy-module-latest-20230430/bpy/ops/node.py
--rw-r--r--   0 runner    (1001) docker     (123)   220624 2023-04-30 06:18:50.000000 fake-bpy-module-latest-20230430/bpy/ops/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    44201 2023-04-30 06:19:05.000000 fake-bpy-module-latest-20230430/bpy/ops/outliner.py
--rw-r--r--   0 runner    (1001) docker     (123)    43251 2023-04-30 06:18:45.000000 fake-bpy-module-latest-20230430/bpy/ops/paint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-04-30 06:19:03.000000 fake-bpy-module-latest-20230430/bpy/ops/paintcurve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-04-30 06:19:09.000000 fake-bpy-module-latest-20230430/bpy/ops/palette.py
--rw-r--r--   0 runner    (1001) docker     (123)    22863 2023-04-30 06:19:05.000000 fake-bpy-module-latest-20230430/bpy/ops/particle.py
--rw-r--r--   0 runner    (1001) docker     (123)    39857 2023-04-30 06:18:54.000000 fake-bpy-module-latest-20230430/bpy/ops/pose.py
--rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-04-30 06:19:16.000000 fake-bpy-module-latest-20230430/bpy/ops/poselib.py
--rw-r--r--   0 runner    (1001) docker     (123)    32388 2023-04-30 06:18:53.000000 fake-bpy-module-latest-20230430/bpy/ops/preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-04-30 06:19:09.000000 fake-bpy-module-latest-20230430/bpy/ops/ptcache.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/bpy/ops/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-04-30 06:19:16.000000 fake-bpy-module-latest-20230430/bpy/ops/render.py
--rw-r--r--   0 runner    (1001) docker     (123)    10108 2023-04-30 06:18:53.000000 fake-bpy-module-latest-20230430/bpy/ops/rigidbody.py
--rw-r--r--   0 runner    (1001) docker     (123)    25220 2023-04-30 06:18:44.000000 fake-bpy-module-latest-20230430/bpy/ops/scene.py
--rw-r--r--   0 runner    (1001) docker     (123)    31884 2023-04-30 06:19:24.000000 fake-bpy-module-latest-20230430/bpy/ops/screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-30 06:19:15.000000 fake-bpy-module-latest-20230430/bpy/ops/script.py
--rw-r--r--   0 runner    (1001) docker     (123)    46533 2023-04-30 06:18:56.000000 fake-bpy-module-latest-20230430/bpy/ops/sculpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-04-30 06:19:15.000000 fake-bpy-module-latest-20230430/bpy/ops/sculpt_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)    93839 2023-04-30 06:19:07.000000 fake-bpy-module-latest-20230430/bpy/ops/sequencer.py
--rw-r--r--   0 runner    (1001) docker     (123)    19928 2023-04-30 06:19:07.000000 fake-bpy-module-latest-20230430/bpy/ops/sound.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-30 06:18:58.000000 fake-bpy-module-latest-20230430/bpy/ops/spreadsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-04-30 06:19:21.000000 fake-bpy-module-latest-20230430/bpy/ops/surface.py
--rw-r--r--   0 runner    (1001) docker     (123)    30944 2023-04-30 06:18:54.000000 fake-bpy-module-latest-20230430/bpy/ops/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-04-30 06:18:54.000000 fake-bpy-module-latest-20230430/bpy/ops/texture.py
--rw-r--r--   0 runner    (1001) docker     (123)    70511 2023-04-30 06:19:09.000000 fake-bpy-module-latest-20230430/bpy/ops/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    19257 2023-04-30 06:19:24.000000 fake-bpy-module-latest-20230430/bpy/ops/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-04-30 06:18:53.000000 fake-bpy-module-latest-20230430/bpy/ops/uilist.py
--rw-r--r--   0 runner    (1001) docker     (123)    56321 2023-04-30 06:19:23.000000 fake-bpy-module-latest-20230430/bpy/ops/uv.py
--rw-r--r--   0 runner    (1001) docker     (123)    12023 2023-04-30 06:19:09.000000 fake-bpy-module-latest-20230430/bpy/ops/view2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    56515 2023-04-30 06:19:21.000000 fake-bpy-module-latest-20230430/bpy/ops/view3d.py
--rw-r--r--   0 runner    (1001) docker     (123)   245716 2023-04-30 06:19:03.000000 fake-bpy-module-latest-20230430/bpy/ops/wm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-04-30 06:19:15.000000 fake-bpy-module-latest-20230430/bpy/ops/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-30 06:19:19.000000 fake-bpy-module-latest-20230430/bpy/ops/world.py
--rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-04-30 06:19:25.000000 fake-bpy-module-latest-20230430/bpy/path.py
--rw-r--r--   0 runner    (1001) docker     (123)    27445 2023-04-30 06:19:25.000000 fake-bpy-module-latest-20230430/bpy/props.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/bpy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)  3488183 2023-04-30 06:18:43.000000 fake-bpy-module-latest-20230430/bpy/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/bpy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-04-30 06:19:25.000000 fake-bpy-module-latest-20230430/bpy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-04-30 06:19:25.000000 fake-bpy-module-latest-20230430/bpy/utils/previews.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/bpy/utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-04-30 06:19:25.000000 fake-bpy-module-latest-20230430/bpy/utils/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/bpy_extras/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-30 06:19:30.000000 fake-bpy-module-latest-20230430/bpy_extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-04-30 06:19:30.000000 fake-bpy-module-latest-20230430/bpy_extras/anim_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-30 06:19:30.000000 fake-bpy-module-latest-20230430/bpy_extras/asset_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-30 06:19:30.000000 fake-bpy-module-latest-20230430/bpy_extras/bmesh_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-30 06:19:30.000000 fake-bpy-module-latest-20230430/bpy_extras/id_map_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-30 06:19:30.000000 fake-bpy-module-latest-20230430/bpy_extras/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-04-30 06:19:30.000000 fake-bpy-module-latest-20230430/bpy_extras/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-30 06:19:30.000000 fake-bpy-module-latest-20230430/bpy_extras/keyconfig_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-04-30 06:19:30.000000 fake-bpy-module-latest-20230430/bpy_extras/mesh_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-04-30 06:19:30.000000 fake-bpy-module-latest-20230430/bpy_extras/node_shader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-30 06:19:30.000000 fake-bpy-module-latest-20230430/bpy_extras/node_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-04-30 06:19:30.000000 fake-bpy-module-latest-20230430/bpy_extras/object_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/bpy_extras/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-04-30 06:19:30.000000 fake-bpy-module-latest-20230430/bpy_extras/view3d_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/bpy_extras/wm_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-30 06:19:30.000000 fake-bpy-module-latest-20230430/bpy_extras/wm_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-30 06:19:30.000000 fake-bpy-module-latest-20230430/bpy_extras/wm_utils/progress_report.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/bpy_extras/wm_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-30 06:19:40.000000 fake-bpy-module-latest-20230430/bpy_restrict_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    54167 2023-04-30 06:19:40.000000 fake-bpy-module-latest-20230430/bpy_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-30 06:19:34.000000 fake-bpy-module-latest-20230430/console_python.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-30 06:19:40.000000 fake-bpy-module-latest-20230430/console_shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/fake_bpy_module_latest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/fake_bpy_module_latest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7720 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/fake_bpy_module_latest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/fake_bpy_module_latest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/fake_bpy_module_latest.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/fake_bpy_module_latest.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/freestyle/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-30 06:19:28.000000 fake-bpy-module-latest-20230430/freestyle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-04-30 06:19:30.000000 fake-bpy-module-latest-20230430/freestyle/chainingiterators.py
--rw-r--r--   0 runner    (1001) docker     (123)    47908 2023-04-30 06:19:30.000000 fake-bpy-module-latest-20230430/freestyle/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13232 2023-04-30 06:19:30.000000 fake-bpy-module-latest-20230430/freestyle/predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/freestyle/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23737 2023-04-30 06:19:30.000000 fake-bpy-module-latest-20230430/freestyle/shaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    86403 2023-04-30 06:19:29.000000 fake-bpy-module-latest-20230430/freestyle/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/freestyle/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-04-30 06:19:29.000000 fake-bpy-module-latest-20230430/freestyle/utils/ContextFunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-04-30 06:19:29.000000 fake-bpy-module-latest-20230430/freestyle/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/freestyle/utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/gpu/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-30 06:19:28.000000 fake-bpy-module-latest-20230430/gpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-04-30 06:19:28.000000 fake-bpy-module-latest-20230430/gpu/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-30 06:19:28.000000 fake-bpy-module-latest-20230430/gpu/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-30 06:19:28.000000 fake-bpy-module-latest-20230430/gpu/platform.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/gpu/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-30 06:19:28.000000 fake-bpy-module-latest-20230430/gpu/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-30 06:19:28.000000 fake-bpy-module-latest-20230430/gpu/shader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-04-30 06:19:28.000000 fake-bpy-module-latest-20230430/gpu/state.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-30 06:19:28.000000 fake-bpy-module-latest-20230430/gpu/texture.py
--rw-r--r--   0 runner    (1001) docker     (123)    26992 2023-04-30 06:19:28.000000 fake-bpy-module-latest-20230430/gpu/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/gpu_extras/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-30 06:19:28.000000 fake-bpy-module-latest-20230430/gpu_extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-30 06:19:28.000000 fake-bpy-module-latest-20230430/gpu_extras/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-04-30 06:19:28.000000 fake-bpy-module-latest-20230430/gpu_extras/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/gpu_extras/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-30 06:21:33.000000 fake-bpy-module-latest-20230430/graphviz_export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/idprop/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-30 06:19:33.000000 fake-bpy-module-latest-20230430/idprop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/idprop/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-30 06:19:33.000000 fake-bpy-module-latest-20230430/idprop/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/imbuf/
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-30 06:19:33.000000 fake-bpy-module-latest-20230430/imbuf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/imbuf/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-30 06:19:33.000000 fake-bpy-module-latest-20230430/imbuf/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    48637 2023-04-30 06:19:34.000000 fake-bpy-module-latest-20230430/keyingsets_builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-30 06:19:40.000000 fake-bpy-module-latest-20230430/keyingsets_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/mathutils/
--rw-r--r--   0 runner    (1001) docker     (123)    86215 2023-04-30 06:19:28.000000 fake-bpy-module-latest-20230430/mathutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-04-30 06:19:28.000000 fake-bpy-module-latest-20230430/mathutils/bvhtree.py
--rw-r--r--   0 runner    (1001) docker     (123)    22187 2023-04-30 06:19:28.000000 fake-bpy-module-latest-20230430/mathutils/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-30 06:19:28.000000 fake-bpy-module-latest-20230430/mathutils/interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-04-30 06:19:28.000000 fake-bpy-module-latest-20230430/mathutils/kdtree.py
--rw-r--r--   0 runner    (1001) docker     (123)    13248 2023-04-30 06:19:28.000000 fake-bpy-module-latest-20230430/mathutils/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/mathutils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-30 06:19:34.000000 fake-bpy-module-latest-20230430/nodeitems_builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-30 06:19:34.000000 fake-bpy-module-latest-20230430/nodeitems_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-04-30 06:21:33.000000 fake-bpy-module-latest-20230430/rna_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-30 06:19:33.000000 fake-bpy-module-latest-20230430/rna_keymap_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-30 06:19:34.000000 fake-bpy-module-latest-20230430/rna_prop_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-30 06:19:34.000000 fake-bpy-module-latest-20230430/rna_xml.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-04-30 06:21:33.000000 fake-bpy-module-latest-20230430/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-30 06:21:33.000000 fake-bpy-module-latest-20230430/sys_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:23:05.000000 fake-bpy-module-latest-20230501/
+-rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-05-01 06:23:05.000000 fake-bpy-module-latest-20230501/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-05-01 06:23:04.000000 fake-bpy-module-latest-20230501/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-01 06:23:03.000000 fake-bpy-module-latest-20230501/addon_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-01 06:21:11.000000 fake-bpy-module-latest-20230501/animsys_refactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31249 2023-05-01 06:21:01.000000 fake-bpy-module-latest-20230501/aud.py
+-rw-r--r--   0 runner    (1001) docker     (123)   116266 2023-05-01 06:20:58.000000 fake-bpy-module-latest-20230501/bgl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:23:05.000000 fake-bpy-module-latest-20230501/bl_app_override/
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-01 06:23:03.000000 fake-bpy-module-latest-20230501/bl_app_override/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-01 06:23:03.000000 fake-bpy-module-latest-20230501/bl_app_override/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 06:13:39.000000 fake-bpy-module-latest-20230501/bl_app_override/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-01 06:21:11.000000 fake-bpy-module-latest-20230501/bl_app_template_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:23:05.000000 fake-bpy-module-latest-20230501/bl_console_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-01 06:23:03.000000 fake-bpy-module-latest-20230501/bl_console_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:23:05.000000 fake-bpy-module-latest-20230501/bl_console_utils/autocomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-01 06:23:03.000000 fake-bpy-module-latest-20230501/bl_console_utils/autocomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-01 06:23:03.000000 fake-bpy-module-latest-20230501/bl_console_utils/autocomplete/complete_calltip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-01 06:23:03.000000 fake-bpy-module-latest-20230501/bl_console_utils/autocomplete/complete_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-01 06:23:03.000000 fake-bpy-module-latest-20230501/bl_console_utils/autocomplete/complete_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-01 06:23:03.000000 fake-bpy-module-latest-20230501/bl_console_utils/autocomplete/intellisense.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 06:13:39.000000 fake-bpy-module-latest-20230501/bl_console_utils/autocomplete/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 06:13:39.000000 fake-bpy-module-latest-20230501/bl_console_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:23:05.000000 fake-bpy-module-latest-20230501/bl_i18n_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-01 06:21:05.000000 fake-bpy-module-latest-20230501/bl_i18n_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-01 06:21:05.000000 fake-bpy-module-latest-20230501/bl_i18n_utils/bl_extract_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-01 06:21:05.000000 fake-bpy-module-latest-20230501/bl_i18n_utils/merge_po.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 06:13:39.000000 fake-bpy-module-latest-20230501/bl_i18n_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-01 06:21:05.000000 fake-bpy-module-latest-20230501/bl_i18n_utils/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-05-01 06:21:05.000000 fake-bpy-module-latest-20230501/bl_i18n_utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-01 06:21:05.000000 fake-bpy-module-latest-20230501/bl_i18n_utils/utils_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-01 06:21:05.000000 fake-bpy-module-latest-20230501/bl_i18n_utils/utils_languages_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-01 06:21:05.000000 fake-bpy-module-latest-20230501/bl_i18n_utils/utils_rtl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:23:05.000000 fake-bpy-module-latest-20230501/bl_keymap_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-01 06:21:11.000000 fake-bpy-module-latest-20230501/bl_keymap_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-01 06:21:11.000000 fake-bpy-module-latest-20230501/bl_keymap_utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-01 06:21:11.000000 fake-bpy-module-latest-20230501/bl_keymap_utils/keymap_from_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-01 06:21:11.000000 fake-bpy-module-latest-20230501/bl_keymap_utils/keymap_hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-01 06:21:11.000000 fake-bpy-module-latest-20230501/bl_keymap_utils/platform_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 06:13:39.000000 fake-bpy-module-latest-20230501/bl_keymap_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-01 06:21:11.000000 fake-bpy-module-latest-20230501/bl_keymap_utils/versioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-01 06:21:05.000000 fake-bpy-module-latest-20230501/bl_math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:23:05.000000 fake-bpy-module-latest-20230501/bl_operators/
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-01 06:21:05.000000 fake-bpy-module-latest-20230501/bl_operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-05-01 06:21:05.000000 fake-bpy-module-latest-20230501/bl_operators/add_mesh_torus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-05-01 06:21:05.000000 fake-bpy-module-latest-20230501/bl_operators/anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-05-01 06:21:06.000000 fake-bpy-module-latest-20230501/bl_operators/assets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:23:05.000000 fake-bpy-module-latest-20230501/bl_operators/bmesh/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-01 06:21:09.000000 fake-bpy-module-latest-20230501/bl_operators/bmesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-01 06:21:09.000000 fake-bpy-module-latest-20230501/bl_operators/bmesh/find_adjacent.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 06:13:39.000000 fake-bpy-module-latest-20230501/bl_operators/bmesh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22556 2023-05-01 06:21:10.000000 fake-bpy-module-latest-20230501/bl_operators/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-05-01 06:21:09.000000 fake-bpy-module-latest-20230501/bl_operators/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-05-01 06:21:05.000000 fake-bpy-module-latest-20230501/bl_operators/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-05-01 06:21:10.000000 fake-bpy-module-latest-20230501/bl_operators/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-05-01 06:21:06.000000 fake-bpy-module-latest-20230501/bl_operators/freestyle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-05-01 06:21:09.000000 fake-bpy-module-latest-20230501/bl_operators/geometry_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-05-01 06:21:06.000000 fake-bpy-module-latest-20230501/bl_operators/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-05-01 06:21:08.000000 fake-bpy-module-latest-20230501/bl_operators/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-05-01 06:21:06.000000 fake-bpy-module-latest-20230501/bl_operators/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38122 2023-05-01 06:21:06.000000 fake-bpy-module-latest-20230501/bl_operators/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-05-01 06:21:10.000000 fake-bpy-module-latest-20230501/bl_operators/object_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-05-01 06:21:06.000000 fake-bpy-module-latest-20230501/bl_operators/object_quick_effects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-05-01 06:21:05.000000 fake-bpy-module-latest-20230501/bl_operators/object_randomize_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42973 2023-05-01 06:21:10.000000 fake-bpy-module-latest-20230501/bl_operators/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 06:13:39.000000 fake-bpy-module-latest-20230501/bl_operators/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-05-01 06:21:11.000000 fake-bpy-module-latest-20230501/bl_operators/rigidbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-01 06:21:05.000000 fake-bpy-module-latest-20230501/bl_operators/screen_play_rendered_anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12099 2023-05-01 06:21:05.000000 fake-bpy-module-latest-20230501/bl_operators/sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-01 06:21:10.000000 fake-bpy-module-latest-20230501/bl_operators/spreadsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56119 2023-05-01 06:21:07.000000 fake-bpy-module-latest-20230501/bl_operators/userpref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-05-01 06:21:07.000000 fake-bpy-module-latest-20230501/bl_operators/uvcalc_follow_active.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-05-01 06:21:05.000000 fake-bpy-module-latest-20230501/bl_operators/uvcalc_lightmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-05-01 06:21:06.000000 fake-bpy-module-latest-20230501/bl_operators/uvcalc_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-01 06:21:05.000000 fake-bpy-module-latest-20230501/bl_operators/vertexpaint_dirt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11529 2023-05-01 06:21:06.000000 fake-bpy-module-latest-20230501/bl_operators/view3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97916 2023-05-01 06:21:09.000000 fake-bpy-module-latest-20230501/bl_operators/wm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:23:05.000000 fake-bpy-module-latest-20230501/bl_previews_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-01 06:21:11.000000 fake-bpy-module-latest-20230501/bl_previews_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-01 06:21:11.000000 fake-bpy-module-latest-20230501/bl_previews_utils/bl_previews_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 06:13:39.000000 fake-bpy-module-latest-20230501/bl_previews_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:23:05.000000 fake-bpy-module-latest-20230501/bl_rna_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-01 06:23:03.000000 fake-bpy-module-latest-20230501/bl_rna_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-01 06:23:03.000000 fake-bpy-module-latest-20230501/bl_rna_utils/data_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 06:13:39.000000 fake-bpy-module-latest-20230501/bl_rna_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:23:05.000000 fake-bpy-module-latest-20230501/bl_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)    10201 2023-05-01 06:21:11.000000 fake-bpy-module-latest-20230501/bl_ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-05-01 06:22:18.000000 fake-bpy-module-latest-20230501/bl_ui/generic_ui_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-01 06:22:14.000000 fake-bpy-module-latest-20230501/bl_ui/node_add_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)   108259 2023-05-01 06:22:24.000000 fake-bpy-module-latest-20230501/bl_ui/node_add_menu_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-01 06:22:12.000000 fake-bpy-module-latest-20230501/bl_ui/properties_animviz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-05-01 06:22:17.000000 fake-bpy-module-latest-20230501/bl_ui/properties_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)   385296 2023-05-01 06:22:36.000000 fake-bpy-module-latest-20230501/bl_ui/properties_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25330 2023-05-01 06:22:52.000000 fake-bpy-module-latest-20230501/bl_ui/properties_data_armature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22602 2023-05-01 06:22:18.000000 fake-bpy-module-latest-20230501/bl_ui/properties_data_bone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36945 2023-05-01 06:22:13.000000 fake-bpy-module-latest-20230501/bl_ui/properties_data_camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38857 2023-05-01 06:22:17.000000 fake-bpy-module-latest-20230501/bl_ui/properties_data_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15423 2023-05-01 06:22:51.000000 fake-bpy-module-latest-20230501/bl_ui/properties_data_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-05-01 06:22:17.000000 fake-bpy-module-latest-20230501/bl_ui/properties_data_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46403 2023-05-01 06:22:53.000000 fake-bpy-module-latest-20230501/bl_ui/properties_data_gpencil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-05-01 06:21:11.000000 fake-bpy-module-latest-20230501/bl_ui/properties_data_lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-05-01 06:22:18.000000 fake-bpy-module-latest-20230501/bl_ui/properties_data_light.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12933 2023-05-01 06:22:18.000000 fake-bpy-module-latest-20230501/bl_ui/properties_data_lightprobe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57510 2023-05-01 06:22:44.000000 fake-bpy-module-latest-20230501/bl_ui/properties_data_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-05-01 06:22:44.000000 fake-bpy-module-latest-20230501/bl_ui/properties_data_metaball.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-05-01 06:22:44.000000 fake-bpy-module-latest-20230501/bl_ui/properties_data_modifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13050 2023-05-01 06:23:02.000000 fake-bpy-module-latest-20230501/bl_ui/properties_data_pointcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-05-01 06:22:12.000000 fake-bpy-module-latest-20230501/bl_ui/properties_data_shaderfx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-05-01 06:22:04.000000 fake-bpy-module-latest-20230501/bl_ui/properties_data_speaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20178 2023-05-01 06:22:17.000000 fake-bpy-module-latest-20230501/bl_ui/properties_data_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66640 2023-05-01 06:22:07.000000 fake-bpy-module-latest-20230501/bl_ui/properties_freestyle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32219 2023-05-01 06:22:56.000000 fake-bpy-module-latest-20230501/bl_ui/properties_grease_pencil_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-05-01 06:22:08.000000 fake-bpy-module-latest-20230501/bl_ui/properties_mask_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30514 2023-05-01 06:22:12.000000 fake-bpy-module-latest-20230501/bl_ui/properties_material.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25892 2023-05-01 06:22:17.000000 fake-bpy-module-latest-20230501/bl_ui/properties_material_gpencil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35174 2023-05-01 06:23:02.000000 fake-bpy-module-latest-20230501/bl_ui/properties_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46745 2023-05-01 06:22:15.000000 fake-bpy-module-latest-20230501/bl_ui/properties_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-05-01 06:22:53.000000 fake-bpy-module-latest-20230501/bl_ui/properties_paint_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)   133597 2023-05-01 06:22:49.000000 fake-bpy-module-latest-20230501/bl_ui/properties_particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36563 2023-05-01 06:22:16.000000 fake-bpy-module-latest-20230501/bl_ui/properties_physics_cloth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-01 06:22:12.000000 fake-bpy-module-latest-20230501/bl_ui/properties_physics_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67584 2023-05-01 06:21:17.000000 fake-bpy-module-latest-20230501/bl_ui/properties_physics_dynamicpaint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27217 2023-05-01 06:22:06.000000 fake-bpy-module-latest-20230501/bl_ui/properties_physics_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91307 2023-05-01 06:22:51.000000 fake-bpy-module-latest-20230501/bl_ui/properties_physics_fluid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-05-01 06:22:04.000000 fake-bpy-module-latest-20230501/bl_ui/properties_physics_rigidbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33547 2023-05-01 06:22:45.000000 fake-bpy-module-latest-20230501/bl_ui/properties_physics_rigidbody_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39030 2023-05-01 06:22:05.000000 fake-bpy-module-latest-20230501/bl_ui/properties_physics_softbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89468 2023-05-01 06:22:55.000000 fake-bpy-module-latest-20230501/bl_ui/properties_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32886 2023-05-01 06:22:14.000000 fake-bpy-module-latest-20230501/bl_ui/properties_scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66952 2023-05-01 06:22:15.000000 fake-bpy-module-latest-20230501/bl_ui/properties_texture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37695 2023-05-01 06:22:06.000000 fake-bpy-module-latest-20230501/bl_ui/properties_view_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-05-01 06:23:02.000000 fake-bpy-module-latest-20230501/bl_ui/properties_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-05-01 06:23:02.000000 fake-bpy-module-latest-20230501/bl_ui/properties_world.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 06:13:39.000000 fake-bpy-module-latest-20230501/bl_ui/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   174521 2023-05-01 06:22:59.000000 fake-bpy-module-latest-20230501/bl_ui/space_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15218 2023-05-01 06:22:53.000000 fake-bpy-module-latest-20230501/bl_ui/space_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62595 2023-05-01 06:22:52.000000 fake-bpy-module-latest-20230501/bl_ui/space_dopesheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71853 2023-05-01 06:22:25.000000 fake-bpy-module-latest-20230501/bl_ui/space_filebrowser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43433 2023-05-01 06:23:00.000000 fake-bpy-module-latest-20230501/bl_ui/space_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)   187053 2023-05-01 06:22:12.000000 fake-bpy-module-latest-20230501/bl_ui/space_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15172 2023-05-01 06:22:03.000000 fake-bpy-module-latest-20230501/bl_ui/space_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38361 2023-05-01 06:23:03.000000 fake-bpy-module-latest-20230501/bl_ui/space_nla.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65582 2023-05-01 06:23:02.000000 fake-bpy-module-latest-20230501/bl_ui/space_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35830 2023-05-01 06:23:00.000000 fake-bpy-module-latest-20230501/bl_ui/space_outliner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-05-01 06:22:53.000000 fake-bpy-module-latest-20230501/bl_ui/space_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)   182398 2023-05-01 06:22:22.000000 fake-bpy-module-latest-20230501/bl_ui/space_sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-05-01 06:22:07.000000 fake-bpy-module-latest-20230501/bl_ui/space_spreadsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-05-01 06:22:16.000000 fake-bpy-module-latest-20230501/bl_ui/space_statusbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40008 2023-05-01 06:22:08.000000 fake-bpy-module-latest-20230501/bl_ui/space_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18254 2023-05-01 06:22:59.000000 fake-bpy-module-latest-20230501/bl_ui/space_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-05-01 06:22:17.000000 fake-bpy-module-latest-20230501/bl_ui/space_toolsystem_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21583 2023-05-01 06:22:04.000000 fake-bpy-module-latest-20230501/bl_ui/space_toolsystem_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65863 2023-05-01 06:22:46.000000 fake-bpy-module-latest-20230501/bl_ui/space_topbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)   209844 2023-05-01 06:21:16.000000 fake-bpy-module-latest-20230501/bl_ui/space_userpref.py
+-rw-r--r--   0 runner    (1001) docker     (123)   611242 2023-05-01 06:22:03.000000 fake-bpy-module-latest-20230501/bl_ui/space_view3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)   237261 2023-05-01 06:22:44.000000 fake-bpy-module-latest-20230501/bl_ui/space_view3d_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-01 06:22:52.000000 fake-bpy-module-latest-20230501/bl_ui/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:23:05.000000 fake-bpy-module-latest-20230501/bl_ui_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-01 06:23:03.000000 fake-bpy-module-latest-20230501/bl_ui_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-01 06:23:03.000000 fake-bpy-module-latest-20230501/bl_ui_utils/bug_report_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-01 06:23:03.000000 fake-bpy-module-latest-20230501/bl_ui_utils/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 06:13:39.000000 fake-bpy-module-latest-20230501/bl_ui_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-01 06:21:11.000000 fake-bpy-module-latest-20230501/blend_render_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-05-01 06:20:58.000000 fake-bpy-module-latest-20230501/blf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:23:05.000000 fake-bpy-module-latest-20230501/bmesh/
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-01 06:21:01.000000 fake-bpy-module-latest-20230501/bmesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-01 06:21:02.000000 fake-bpy-module-latest-20230501/bmesh/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77491 2023-05-01 06:21:05.000000 fake-bpy-module-latest-20230501/bmesh/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 06:13:39.000000 fake-bpy-module-latest-20230501/bmesh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    37270 2023-05-01 06:21:02.000000 fake-bpy-module-latest-20230501/bmesh/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-05-01 06:21:02.000000 fake-bpy-module-latest-20230501/bmesh/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:23:05.000000 fake-bpy-module-latest-20230501/bpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-01 06:13:39.000000 fake-bpy-module-latest-20230501/bpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:23:05.000000 fake-bpy-module-latest-20230501/bpy/app/
+-rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-05-01 06:20:56.000000 fake-bpy-module-latest-20230501/bpy/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-05-01 06:20:56.000000 fake-bpy-module-latest-20230501/bpy/app/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-01 06:20:56.000000 fake-bpy-module-latest-20230501/bpy/app/icons.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 06:13:39.000000 fake-bpy-module-latest-20230501/bpy/app/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-01 06:20:56.000000 fake-bpy-module-latest-20230501/bpy/app/timers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-05-01 06:20:56.000000 fake-bpy-module-latest-20230501/bpy/app/translations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-01 06:20:57.000000 fake-bpy-module-latest-20230501/bpy/msgbus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:23:05.000000 fake-bpy-module-latest-20230501/bpy/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-01 06:20:15.000000 fake-bpy-module-latest-20230501/bpy/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27608 2023-05-01 06:20:31.000000 fake-bpy-module-latest-20230501/bpy/ops/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35270 2023-05-01 06:20:42.000000 fake-bpy-module-latest-20230501/bpy/ops/anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25130 2023-05-01 06:20:54.000000 fake-bpy-module-latest-20230501/bpy/ops/armature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-05-01 06:20:48.000000 fake-bpy-module-latest-20230501/bpy/ops/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-05-01 06:20:49.000000 fake-bpy-module-latest-20230501/bpy/ops/boid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-05-01 06:20:39.000000 fake-bpy-module-latest-20230501/bpy/ops/brush.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12217 2023-05-01 06:20:15.000000 fake-bpy-module-latest-20230501/bpy/ops/buttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-05-01 06:20:21.000000 fake-bpy-module-latest-20230501/bpy/ops/cachefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-05-01 06:20:53.000000 fake-bpy-module-latest-20230501/bpy/ops/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70010 2023-05-01 06:20:36.000000 fake-bpy-module-latest-20230501/bpy/ops/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-01 06:20:34.000000 fake-bpy-module-latest-20230501/bpy/ops/cloth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-05-01 06:20:53.000000 fake-bpy-module-latest-20230501/bpy/ops/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12767 2023-05-01 06:20:56.000000 fake-bpy-module-latest-20230501/bpy/ops/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17809 2023-05-01 06:20:55.000000 fake-bpy-module-latest-20230501/bpy/ops/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40490 2023-05-01 06:20:34.000000 fake-bpy-module-latest-20230501/bpy/ops/curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-05-01 06:20:31.000000 fake-bpy-module-latest-20230501/bpy/ops/curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-05-01 06:20:41.000000 fake-bpy-module-latest-20230501/bpy/ops/cycles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-05-01 06:20:22.000000 fake-bpy-module-latest-20230501/bpy/ops/dpaint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-05-01 06:20:35.000000 fake-bpy-module-latest-20230501/bpy/ops/ed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-05-01 06:20:38.000000 fake-bpy-module-latest-20230501/bpy/ops/export_anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-05-01 06:20:41.000000 fake-bpy-module-latest-20230501/bpy/ops/export_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40642 2023-05-01 06:20:52.000000 fake-bpy-module-latest-20230501/bpy/ops/export_scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30339 2023-05-01 06:20:17.000000 fake-bpy-module-latest-20230501/bpy/ops/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-05-01 06:20:27.000000 fake-bpy-module-latest-20230501/bpy/ops/fluid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21051 2023-05-01 06:20:55.000000 fake-bpy-module-latest-20230501/bpy/ops/font.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-05-01 06:20:41.000000 fake-bpy-module-latest-20230501/bpy/ops/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-01 06:20:41.000000 fake-bpy-module-latest-20230501/bpy/ops/gizmogroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)   132520 2023-05-01 06:20:51.000000 fake-bpy-module-latest-20230501/bpy/ops/gpencil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49736 2023-05-01 06:20:54.000000 fake-bpy-module-latest-20230501/bpy/ops/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53280 2023-05-01 06:20:32.000000 fake-bpy-module-latest-20230501/bpy/ops/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-01 06:20:48.000000 fake-bpy-module-latest-20230501/bpy/ops/import_anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-01 06:20:53.000000 fake-bpy-module-latest-20230501/bpy/ops/import_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-05-01 06:20:21.000000 fake-bpy-module-latest-20230501/bpy/ops/import_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14471 2023-05-01 06:20:40.000000 fake-bpy-module-latest-20230501/bpy/ops/import_scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-05-01 06:20:56.000000 fake-bpy-module-latest-20230501/bpy/ops/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-05-01 06:20:56.000000 fake-bpy-module-latest-20230501/bpy/ops/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-05-01 06:20:38.000000 fake-bpy-module-latest-20230501/bpy/ops/marker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26986 2023-05-01 06:20:34.000000 fake-bpy-module-latest-20230501/bpy/ops/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-01 06:20:48.000000 fake-bpy-module-latest-20230501/bpy/ops/material.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-05-01 06:20:53.000000 fake-bpy-module-latest-20230501/bpy/ops/mball.py
+-rw-r--r--   0 runner    (1001) docker     (123)   182898 2023-05-01 06:20:30.000000 fake-bpy-module-latest-20230501/bpy/ops/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28495 2023-05-01 06:20:56.000000 fake-bpy-module-latest-20230501/bpy/ops/nla.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67349 2023-05-01 06:20:17.000000 fake-bpy-module-latest-20230501/bpy/ops/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)   220626 2023-05-01 06:20:27.000000 fake-bpy-module-latest-20230501/bpy/ops/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44201 2023-05-01 06:20:39.000000 fake-bpy-module-latest-20230501/bpy/ops/outliner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43251 2023-05-01 06:20:22.000000 fake-bpy-module-latest-20230501/bpy/ops/paint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-01 06:20:34.000000 fake-bpy-module-latest-20230501/bpy/ops/paintcurve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-05-01 06:20:53.000000 fake-bpy-module-latest-20230501/bpy/ops/palette.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22863 2023-05-01 06:20:21.000000 fake-bpy-module-latest-20230501/bpy/ops/particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39857 2023-05-01 06:20:36.000000 fake-bpy-module-latest-20230501/bpy/ops/pose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-05-01 06:20:53.000000 fake-bpy-module-latest-20230501/bpy/ops/poselib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32388 2023-05-01 06:20:55.000000 fake-bpy-module-latest-20230501/bpy/ops/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-05-01 06:20:48.000000 fake-bpy-module-latest-20230501/bpy/ops/ptcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 06:13:39.000000 fake-bpy-module-latest-20230501/bpy/ops/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-05-01 06:20:49.000000 fake-bpy-module-latest-20230501/bpy/ops/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10108 2023-05-01 06:20:22.000000 fake-bpy-module-latest-20230501/bpy/ops/rigidbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25220 2023-05-01 06:20:22.000000 fake-bpy-module-latest-20230501/bpy/ops/scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31884 2023-05-01 06:20:16.000000 fake-bpy-module-latest-20230501/bpy/ops/screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-01 06:20:28.000000 fake-bpy-module-latest-20230501/bpy/ops/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46533 2023-05-01 06:20:33.000000 fake-bpy-module-latest-20230501/bpy/ops/sculpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-05-01 06:20:34.000000 fake-bpy-module-latest-20230501/bpy/ops/sculpt_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93840 2023-05-01 06:20:24.000000 fake-bpy-module-latest-20230501/bpy/ops/sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19928 2023-05-01 06:20:48.000000 fake-bpy-module-latest-20230501/bpy/ops/sound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-01 06:20:41.000000 fake-bpy-module-latest-20230501/bpy/ops/spreadsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-05-01 06:20:41.000000 fake-bpy-module-latest-20230501/bpy/ops/surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30944 2023-05-01 06:20:39.000000 fake-bpy-module-latest-20230501/bpy/ops/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-01 06:20:56.000000 fake-bpy-module-latest-20230501/bpy/ops/texture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70511 2023-05-01 06:20:21.000000 fake-bpy-module-latest-20230501/bpy/ops/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19257 2023-05-01 06:20:41.000000 fake-bpy-module-latest-20230501/bpy/ops/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-05-01 06:20:38.000000 fake-bpy-module-latest-20230501/bpy/ops/uilist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56321 2023-05-01 06:20:38.000000 fake-bpy-module-latest-20230501/bpy/ops/uv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12023 2023-05-01 06:20:41.000000 fake-bpy-module-latest-20230501/bpy/ops/view2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56515 2023-05-01 06:20:38.000000 fake-bpy-module-latest-20230501/bpy/ops/view3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)   245716 2023-05-01 06:20:48.000000 fake-bpy-module-latest-20230501/bpy/ops/wm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-05-01 06:20:15.000000 fake-bpy-module-latest-20230501/bpy/ops/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-01 06:20:48.000000 fake-bpy-module-latest-20230501/bpy/ops/world.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-05-01 06:20:57.000000 fake-bpy-module-latest-20230501/bpy/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27445 2023-05-01 06:20:57.000000 fake-bpy-module-latest-20230501/bpy/props.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 06:13:39.000000 fake-bpy-module-latest-20230501/bpy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)  3488183 2023-05-01 06:20:15.000000 fake-bpy-module-latest-20230501/bpy/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:23:05.000000 fake-bpy-module-latest-20230501/bpy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-05-01 06:20:56.000000 fake-bpy-module-latest-20230501/bpy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-01 06:20:56.000000 fake-bpy-module-latest-20230501/bpy/utils/previews.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 06:13:39.000000 fake-bpy-module-latest-20230501/bpy/utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-01 06:20:57.000000 fake-bpy-module-latest-20230501/bpy/utils/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:23:05.000000 fake-bpy-module-latest-20230501/bpy_extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-01 06:21:01.000000 fake-bpy-module-latest-20230501/bpy_extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-01 06:21:01.000000 fake-bpy-module-latest-20230501/bpy_extras/anim_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-01 06:21:01.000000 fake-bpy-module-latest-20230501/bpy_extras/asset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-01 06:21:01.000000 fake-bpy-module-latest-20230501/bpy_extras/bmesh_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-01 06:21:01.000000 fake-bpy-module-latest-20230501/bpy_extras/id_map_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-01 06:21:01.000000 fake-bpy-module-latest-20230501/bpy_extras/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-05-01 06:21:01.000000 fake-bpy-module-latest-20230501/bpy_extras/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-01 06:21:01.000000 fake-bpy-module-latest-20230501/bpy_extras/keyconfig_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-01 06:21:01.000000 fake-bpy-module-latest-20230501/bpy_extras/mesh_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-05-01 06:21:01.000000 fake-bpy-module-latest-20230501/bpy_extras/node_shader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-01 06:21:01.000000 fake-bpy-module-latest-20230501/bpy_extras/node_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-05-01 06:21:01.000000 fake-bpy-module-latest-20230501/bpy_extras/object_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 06:13:39.000000 fake-bpy-module-latest-20230501/bpy_extras/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-05-01 06:21:01.000000 fake-bpy-module-latest-20230501/bpy_extras/view3d_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:23:05.000000 fake-bpy-module-latest-20230501/bpy_extras/wm_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-01 06:21:01.000000 fake-bpy-module-latest-20230501/bpy_extras/wm_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-01 06:21:01.000000 fake-bpy-module-latest-20230501/bpy_extras/wm_utils/progress_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 06:13:39.000000 fake-bpy-module-latest-20230501/bpy_extras/wm_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-01 06:21:11.000000 fake-bpy-module-latest-20230501/bpy_restrict_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54167 2023-05-01 06:21:11.000000 fake-bpy-module-latest-20230501/bpy_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-01 06:21:05.000000 fake-bpy-module-latest-20230501/console_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-01 06:23:03.000000 fake-bpy-module-latest-20230501/console_shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:23:05.000000 fake-bpy-module-latest-20230501/fake_bpy_module_latest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-05-01 06:23:05.000000 fake-bpy-module-latest-20230501/fake_bpy_module_latest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7720 2023-05-01 06:23:05.000000 fake-bpy-module-latest-20230501/fake_bpy_module_latest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 06:23:05.000000 fake-bpy-module-latest-20230501/fake_bpy_module_latest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 06:23:05.000000 fake-bpy-module-latest-20230501/fake_bpy_module_latest.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-01 06:23:05.000000 fake-bpy-module-latest-20230501/fake_bpy_module_latest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:23:05.000000 fake-bpy-module-latest-20230501/freestyle/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-01 06:21:00.000000 fake-bpy-module-latest-20230501/freestyle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-05-01 06:21:01.000000 fake-bpy-module-latest-20230501/freestyle/chainingiterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47908 2023-05-01 06:21:01.000000 fake-bpy-module-latest-20230501/freestyle/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13232 2023-05-01 06:21:01.000000 fake-bpy-module-latest-20230501/freestyle/predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 06:13:39.000000 fake-bpy-module-latest-20230501/freestyle/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23737 2023-05-01 06:21:01.000000 fake-bpy-module-latest-20230501/freestyle/shaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86403 2023-05-01 06:21:01.000000 fake-bpy-module-latest-20230501/freestyle/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:23:05.000000 fake-bpy-module-latest-20230501/freestyle/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-01 06:21:01.000000 fake-bpy-module-latest-20230501/freestyle/utils/ContextFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-05-01 06:21:01.000000 fake-bpy-module-latest-20230501/freestyle/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 06:13:39.000000 fake-bpy-module-latest-20230501/freestyle/utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:23:05.000000 fake-bpy-module-latest-20230501/gpu/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-01 06:21:00.000000 fake-bpy-module-latest-20230501/gpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-05-01 06:21:00.000000 fake-bpy-module-latest-20230501/gpu/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-01 06:21:00.000000 fake-bpy-module-latest-20230501/gpu/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-01 06:21:00.000000 fake-bpy-module-latest-20230501/gpu/platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 06:13:39.000000 fake-bpy-module-latest-20230501/gpu/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-01 06:21:00.000000 fake-bpy-module-latest-20230501/gpu/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-01 06:21:00.000000 fake-bpy-module-latest-20230501/gpu/shader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-05-01 06:21:00.000000 fake-bpy-module-latest-20230501/gpu/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-01 06:21:00.000000 fake-bpy-module-latest-20230501/gpu/texture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26992 2023-05-01 06:21:00.000000 fake-bpy-module-latest-20230501/gpu/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:23:05.000000 fake-bpy-module-latest-20230501/gpu_extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-01 06:21:00.000000 fake-bpy-module-latest-20230501/gpu_extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-01 06:21:00.000000 fake-bpy-module-latest-20230501/gpu_extras/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-01 06:21:00.000000 fake-bpy-module-latest-20230501/gpu_extras/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 06:13:39.000000 fake-bpy-module-latest-20230501/gpu_extras/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-01 06:21:11.000000 fake-bpy-module-latest-20230501/graphviz_export.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:23:05.000000 fake-bpy-module-latest-20230501/idprop/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-01 06:21:05.000000 fake-bpy-module-latest-20230501/idprop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 06:13:39.000000 fake-bpy-module-latest-20230501/idprop/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-01 06:21:05.000000 fake-bpy-module-latest-20230501/idprop/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:23:05.000000 fake-bpy-module-latest-20230501/imbuf/
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-01 06:21:05.000000 fake-bpy-module-latest-20230501/imbuf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 06:13:39.000000 fake-bpy-module-latest-20230501/imbuf/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-01 06:21:05.000000 fake-bpy-module-latest-20230501/imbuf/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48637 2023-05-01 06:23:03.000000 fake-bpy-module-latest-20230501/keyingsets_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-01 06:23:03.000000 fake-bpy-module-latest-20230501/keyingsets_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:23:05.000000 fake-bpy-module-latest-20230501/mathutils/
+-rw-r--r--   0 runner    (1001) docker     (123)    86215 2023-05-01 06:21:00.000000 fake-bpy-module-latest-20230501/mathutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-05-01 06:21:00.000000 fake-bpy-module-latest-20230501/mathutils/bvhtree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22187 2023-05-01 06:21:00.000000 fake-bpy-module-latest-20230501/mathutils/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-01 06:21:00.000000 fake-bpy-module-latest-20230501/mathutils/interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-01 06:21:00.000000 fake-bpy-module-latest-20230501/mathutils/kdtree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13248 2023-05-01 06:21:00.000000 fake-bpy-module-latest-20230501/mathutils/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 06:13:39.000000 fake-bpy-module-latest-20230501/mathutils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-01 06:23:03.000000 fake-bpy-module-latest-20230501/nodeitems_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-01 06:21:11.000000 fake-bpy-module-latest-20230501/nodeitems_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-05-01 06:21:11.000000 fake-bpy-module-latest-20230501/rna_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-01 06:21:11.000000 fake-bpy-module-latest-20230501/rna_keymap_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-01 06:23:03.000000 fake-bpy-module-latest-20230501/rna_prop_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-01 06:23:03.000000 fake-bpy-module-latest-20230501/rna_xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 06:23:05.000000 fake-bpy-module-latest-20230501/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-05-01 06:23:04.000000 fake-bpy-module-latest-20230501/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-01 06:21:11.000000 fake-bpy-module-latest-20230501/sys_info.py
```

### Comparing `fake-bpy-module-latest-20230430/PKG-INFO` & `fake-bpy-module-latest-20230501/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: fake-bpy-module-latest
-Version: 20230430
+Version: 20230501
 Summary: Collection of the fake Blender Python API module for the code completion.
 Home-page: https://github.com/nutti/fake-bpy-module
 Author: nutti
 Author-email: nutti.metro@gmail.com
 Maintainer: nutti
 Maintainer-email: nutti.metro@gmail.com
 License: MIT
```

### Comparing `fake-bpy-module-latest-20230430/README.rst` & `fake-bpy-module-latest-20230501/README.rst`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/addon_utils.py` & `fake-bpy-module-latest-20230501/addon_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/animsys_refactor.py` & `fake-bpy-module-latest-20230501/animsys_refactor.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/aud.py` & `fake-bpy-module-latest-20230501/aud.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bgl.py` & `fake-bpy-module-latest-20230501/bgl.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_app_override/helpers.py` & `fake-bpy-module-latest-20230501/bl_app_override/helpers.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_i18n_utils/bl_extract_messages.py` & `fake-bpy-module-latest-20230501/bl_i18n_utils/bl_extract_messages.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_i18n_utils/settings.py` & `fake-bpy-module-latest-20230501/bl_i18n_utils/settings.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_i18n_utils/utils.py` & `fake-bpy-module-latest-20230501/bl_i18n_utils/utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_keymap_utils/io.py` & `fake-bpy-module-latest-20230501/bl_keymap_utils/io.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_math.py` & `fake-bpy-module-latest-20230501/bl_math.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_operators/__init__.py` & `fake-bpy-module-latest-20230501/bl_operators/__init__.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 import sys
 import typing
-from . import presets
-from . import console
-from . import image
-from . import node
-from . import screen_play_rendered_anim
-from . import constraint
-from . import wm
-from . import freestyle
-from . import bmesh
-from . import mesh
 from . import sequencer
-from . import vertexpaint_dirt
-from . import object
-from . import rigidbody
+from . import add_mesh_torus
 from . import object_randomize_transform
-from . import userpref
-from . import object_quick_effects
-from . import clip
+from . import vertexpaint_dirt
+from . import constraint
 from . import uvcalc_lightmap
-from . import spreadsheet
-from . import file
-from . import assets
-from . import geometry_nodes
+from . import screen_play_rendered_anim
+from . import anim
+from . import object
+from . import freestyle
+from . import node
+from . import image
 from . import view3d
+from . import assets
+from . import object_quick_effects
 from . import uvcalc_transform
+from . import userpref
 from . import uvcalc_follow_active
-from . import anim
+from . import mesh
+from . import wm
+from . import geometry_nodes
+from . import bmesh
+from . import console
+from . import clip
 from . import object_align
-from . import add_mesh_torus
+from . import presets
+from . import file
+from . import spreadsheet
+from . import rigidbody
 
 GenericType = typing.TypeVar("GenericType")
 
 
 def register():
     '''
```

### Comparing `fake-bpy-module-latest-20230430/bl_operators/add_mesh_torus.py` & `fake-bpy-module-latest-20230501/bl_operators/add_mesh_torus.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_operators/anim.py` & `fake-bpy-module-latest-20230501/bl_operators/anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_operators/assets.py` & `fake-bpy-module-latest-20230501/bl_operators/assets.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_operators/bmesh/find_adjacent.py` & `fake-bpy-module-latest-20230501/bl_operators/bmesh/find_adjacent.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_operators/clip.py` & `fake-bpy-module-latest-20230501/bl_operators/clip.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_operators/console.py` & `fake-bpy-module-latest-20230501/bl_operators/console.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_operators/constraint.py` & `fake-bpy-module-latest-20230501/bl_operators/constraint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_operators/file.py` & `fake-bpy-module-latest-20230501/bl_operators/file.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_operators/freestyle.py` & `fake-bpy-module-latest-20230501/bl_operators/freestyle.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_operators/geometry_nodes.py` & `fake-bpy-module-latest-20230501/bl_operators/geometry_nodes.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_operators/image.py` & `fake-bpy-module-latest-20230501/bl_operators/image.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_operators/mesh.py` & `fake-bpy-module-latest-20230501/bl_operators/mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_operators/node.py` & `fake-bpy-module-latest-20230501/bl_operators/node.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_operators/object.py` & `fake-bpy-module-latest-20230501/bl_operators/object.py`

 * *Files 0% similar despite different names*

```diff
@@ -865,14 +865,20 @@
 
     def path_resolve(self):
         ''' 
 
         '''
         pass
 
+    def poll(self, context):
+        ''' 
+
+        '''
+        pass
+
     def poll_message_set(self):
         ''' 
 
         '''
         pass
 
     def pop(self):
```

### Comparing `fake-bpy-module-latest-20230430/bl_operators/object_align.py` & `fake-bpy-module-latest-20230501/bl_operators/object_align.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_operators/object_quick_effects.py` & `fake-bpy-module-latest-20230501/bl_operators/object_quick_effects.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_operators/object_randomize_transform.py` & `fake-bpy-module-latest-20230501/bl_operators/object_randomize_transform.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_operators/presets.py` & `fake-bpy-module-latest-20230501/bl_operators/presets.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_operators/rigidbody.py` & `fake-bpy-module-latest-20230501/bl_operators/rigidbody.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_operators/screen_play_rendered_anim.py` & `fake-bpy-module-latest-20230501/bl_operators/screen_play_rendered_anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_operators/sequencer.py` & `fake-bpy-module-latest-20230501/bl_operators/sequencer.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_operators/spreadsheet.py` & `fake-bpy-module-latest-20230501/bl_operators/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_operators/userpref.py` & `fake-bpy-module-latest-20230501/bl_operators/userpref.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_operators/uvcalc_follow_active.py` & `fake-bpy-module-latest-20230501/bl_operators/uvcalc_follow_active.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_operators/uvcalc_lightmap.py` & `fake-bpy-module-latest-20230501/bl_operators/uvcalc_lightmap.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_operators/uvcalc_transform.py` & `fake-bpy-module-latest-20230501/bl_operators/uvcalc_transform.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_operators/vertexpaint_dirt.py` & `fake-bpy-module-latest-20230501/bl_operators/vertexpaint_dirt.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_operators/view3d.py` & `fake-bpy-module-latest-20230501/bl_operators/view3d.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_operators/wm.py` & `fake-bpy-module-latest-20230501/bl_operators/wm.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_previews_utils/bl_previews_render.py` & `fake-bpy-module-latest-20230501/bl_previews_utils/bl_previews_render.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/__init__.py` & `fake-bpy-module-latest-20230501/bl_ui/__init__.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,80 +1,80 @@
 import sys
 import typing
 import bpy_types
 
-from . import properties_physics_fluid
-from . import properties_world
-from . import properties_output
+from . import properties_data_lattice
+from . import space_userpref
+from . import properties_physics_dynamicpaint
+from . import space_view3d
+from . import space_info
+from . import space_toolsystem_toolbar
+from . import properties_data_speaker
+from . import properties_physics_rigidbody
+from . import properties_physics_softbody
+from . import properties_view_layer
+from . import properties_physics_field
+from . import properties_freestyle
+from . import space_spreadsheet
+from . import properties_mask_common
+from . import space_text
+from . import space_image
+from . import properties_material
+from . import properties_physics_common
+from . import properties_data_shaderfx
+from . import properties_animviz
 from . import properties_data_camera
-from . import space_node
-from . import space_clip
+from . import properties_scene
+from . import node_add_menu
+from . import properties_texture
+from . import properties_output
+from . import properties_physics_cloth
+from . import space_statusbar
+from . import properties_material_gpencil
 from . import properties_collection
-from . import properties_data_armature
-from . import space_image
-from . import space_topbar
+from . import properties_data_empty
+from . import properties_data_curve
+from . import properties_data_volume
+from . import space_toolsystem_common
+from . import properties_data_bone
+from . import properties_data_lightprobe
+from . import generic_ui_list
+from . import properties_data_light
+from . import space_sequencer
 from . import node_add_menu_geometry
 from . import space_filebrowser
-from . import properties_grease_pencil_common
-from . import space_nla
-from . import properties_physics_rigidbody_constraint
-from . import properties_data_pointcloud
-from . import properties_data_metaball
-from . import space_userpref
 from . import properties_constraint
-from . import space_toolsystem_common
-from . import space_spreadsheet
-from . import properties_physics_rigidbody
-from . import space_properties
-from . import properties_data_light
-from . import space_text
 from . import space_view3d_toolbar
-from . import properties_physics_cloth
-from . import properties_particle
-from . import properties_view_layer
-from . import properties_data_lightprobe
-from . import properties_data_mesh
-from . import utils
 from . import properties_data_modifier
-from . import properties_physics_common
-from . import space_graph
+from . import properties_data_mesh
+from . import properties_data_metaball
+from . import properties_physics_rigidbody_constraint
+from . import space_topbar
+from . import properties_particle
+from . import properties_physics_fluid
 from . import properties_data_curves
-from . import properties_material_gpencil
-from . import generic_ui_list
-from . import properties_data_shaderfx
-from . import space_outliner
-from . import space_info
-from . import space_statusbar
+from . import space_dopesheet
+from . import utils
+from . import properties_data_armature
+from . import properties_data_gpencil
+from . import properties_paint_common
 from . import space_console
+from . import space_properties
 from . import properties_render
-from . import properties_texture
-from . import space_sequencer
-from . import properties_data_empty
-from . import properties_physics_field
-from . import properties_paint_common
-from . import properties_data_speaker
-from . import properties_data_gpencil
-from . import properties_data_bone
-from . import properties_data_volume
-from . import properties_object
-from . import properties_animviz
-from . import properties_data_curve
-from . import properties_data_lattice
-from . import space_dopesheet
-from . import space_toolsystem_toolbar
-from . import properties_material
-from . import space_view3d
+from . import properties_grease_pencil_common
+from . import space_clip
 from . import space_time
-from . import node_add_menu
-from . import properties_physics_dynamicpaint
-from . import properties_scene
-from . import properties_freestyle
-from . import properties_mask_common
-from . import properties_physics_softbody
+from . import space_graph
+from . import space_outliner
+from . import space_node
+from . import properties_data_pointcloud
 from . import properties_workspace
+from . import properties_object
+from . import properties_world
+from . import space_nla
 
 GenericType = typing.TypeVar("GenericType")
 
 
 class UI_MT_button_context_menu(bpy_types.Menu, bpy_types._GenericUI):
     bl_idname = None
     ''' '''
```

### Comparing `fake-bpy-module-latest-20230430/bl_ui/generic_ui_list.py` & `fake-bpy-module-latest-20230501/bl_ui/generic_ui_list.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/node_add_menu_geometry.py` & `fake-bpy-module-latest-20230501/bl_ui/node_add_menu_geometry.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/properties_animviz.py` & `fake-bpy-module-latest-20230501/bl_ui/properties_animviz.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/properties_collection.py` & `fake-bpy-module-latest-20230501/bl_ui/properties_collection.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/properties_constraint.py` & `fake-bpy-module-latest-20230501/bl_ui/properties_constraint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/properties_data_armature.py` & `fake-bpy-module-latest-20230501/bl_ui/properties_data_armature.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/properties_data_bone.py` & `fake-bpy-module-latest-20230501/bl_ui/properties_data_bone.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/properties_data_camera.py` & `fake-bpy-module-latest-20230501/bl_ui/properties_data_camera.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/properties_data_curve.py` & `fake-bpy-module-latest-20230501/bl_ui/properties_data_curve.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/properties_data_curves.py` & `fake-bpy-module-latest-20230501/bl_ui/properties_data_curves.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/properties_data_empty.py` & `fake-bpy-module-latest-20230501/bl_ui/properties_data_empty.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/properties_data_gpencil.py` & `fake-bpy-module-latest-20230501/bl_ui/properties_data_gpencil.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/properties_data_lattice.py` & `fake-bpy-module-latest-20230501/bl_ui/properties_data_lattice.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/properties_data_light.py` & `fake-bpy-module-latest-20230501/bl_ui/properties_data_light.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/properties_data_lightprobe.py` & `fake-bpy-module-latest-20230501/bl_ui/properties_data_lightprobe.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/properties_data_mesh.py` & `fake-bpy-module-latest-20230501/bl_ui/properties_data_mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/properties_data_metaball.py` & `fake-bpy-module-latest-20230501/bl_ui/properties_data_metaball.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/properties_data_modifier.py` & `fake-bpy-module-latest-20230501/bl_ui/properties_data_modifier.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/properties_data_pointcloud.py` & `fake-bpy-module-latest-20230501/bl_ui/properties_data_pointcloud.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/properties_data_shaderfx.py` & `fake-bpy-module-latest-20230501/bl_ui/properties_data_shaderfx.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/properties_data_speaker.py` & `fake-bpy-module-latest-20230501/bl_ui/properties_data_speaker.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/properties_data_volume.py` & `fake-bpy-module-latest-20230501/bl_ui/properties_data_volume.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/properties_freestyle.py` & `fake-bpy-module-latest-20230501/bl_ui/properties_freestyle.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/properties_grease_pencil_common.py` & `fake-bpy-module-latest-20230501/bl_ui/properties_grease_pencil_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/properties_mask_common.py` & `fake-bpy-module-latest-20230501/bl_ui/properties_mask_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/properties_material.py` & `fake-bpy-module-latest-20230501/bl_ui/properties_material.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/properties_material_gpencil.py` & `fake-bpy-module-latest-20230501/bl_ui/properties_material_gpencil.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/properties_object.py` & `fake-bpy-module-latest-20230501/bl_ui/properties_object.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/properties_output.py` & `fake-bpy-module-latest-20230501/bl_ui/properties_output.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/properties_paint_common.py` & `fake-bpy-module-latest-20230501/bl_ui/properties_paint_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/properties_particle.py` & `fake-bpy-module-latest-20230501/bl_ui/properties_particle.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/properties_physics_cloth.py` & `fake-bpy-module-latest-20230501/bl_ui/properties_physics_cloth.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/properties_physics_common.py` & `fake-bpy-module-latest-20230501/bl_ui/properties_physics_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/properties_physics_dynamicpaint.py` & `fake-bpy-module-latest-20230501/bl_ui/properties_physics_dynamicpaint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/properties_physics_field.py` & `fake-bpy-module-latest-20230501/bl_ui/properties_physics_field.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/properties_physics_fluid.py` & `fake-bpy-module-latest-20230501/bl_ui/properties_physics_fluid.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/properties_physics_rigidbody.py` & `fake-bpy-module-latest-20230501/bl_ui/properties_physics_rigidbody.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/properties_physics_rigidbody_constraint.py` & `fake-bpy-module-latest-20230501/bl_ui/properties_physics_rigidbody_constraint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/properties_physics_softbody.py` & `fake-bpy-module-latest-20230501/bl_ui/properties_physics_softbody.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/properties_render.py` & `fake-bpy-module-latest-20230501/bl_ui/properties_render.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/properties_scene.py` & `fake-bpy-module-latest-20230501/bl_ui/properties_scene.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/properties_texture.py` & `fake-bpy-module-latest-20230501/bl_ui/properties_texture.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/properties_view_layer.py` & `fake-bpy-module-latest-20230501/bl_ui/properties_view_layer.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/properties_workspace.py` & `fake-bpy-module-latest-20230501/bl_ui/properties_workspace.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/properties_world.py` & `fake-bpy-module-latest-20230501/bl_ui/properties_world.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/space_clip.py` & `fake-bpy-module-latest-20230501/bl_ui/space_clip.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/space_console.py` & `fake-bpy-module-latest-20230501/bl_ui/space_console.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/space_dopesheet.py` & `fake-bpy-module-latest-20230501/bl_ui/space_dopesheet.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/space_filebrowser.py` & `fake-bpy-module-latest-20230501/bl_ui/space_filebrowser.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/space_graph.py` & `fake-bpy-module-latest-20230501/bl_ui/space_graph.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/space_image.py` & `fake-bpy-module-latest-20230501/bl_ui/space_image.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/space_info.py` & `fake-bpy-module-latest-20230501/bl_ui/space_info.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/space_nla.py` & `fake-bpy-module-latest-20230501/bl_ui/space_nla.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/space_node.py` & `fake-bpy-module-latest-20230501/bl_ui/space_node.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/space_outliner.py` & `fake-bpy-module-latest-20230501/bl_ui/space_outliner.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/space_properties.py` & `fake-bpy-module-latest-20230501/bl_ui/space_properties.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/space_sequencer.py` & `fake-bpy-module-latest-20230501/bl_ui/space_sequencer.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/space_spreadsheet.py` & `fake-bpy-module-latest-20230501/bl_ui/space_spreadsheet.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/space_statusbar.py` & `fake-bpy-module-latest-20230501/bl_ui/space_statusbar.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/space_text.py` & `fake-bpy-module-latest-20230501/bl_ui/space_text.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/space_time.py` & `fake-bpy-module-latest-20230501/bl_ui/space_time.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/space_toolsystem_common.py` & `fake-bpy-module-latest-20230501/bl_ui/space_toolsystem_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/space_toolsystem_toolbar.py` & `fake-bpy-module-latest-20230501/bl_ui/space_toolsystem_toolbar.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/space_topbar.py` & `fake-bpy-module-latest-20230501/bl_ui/space_topbar.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/space_userpref.py` & `fake-bpy-module-latest-20230501/bl_ui/space_userpref.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/space_view3d.py` & `fake-bpy-module-latest-20230501/bl_ui/space_view3d.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/space_view3d_toolbar.py` & `fake-bpy-module-latest-20230501/bl_ui/space_view3d_toolbar.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bl_ui/utils.py` & `fake-bpy-module-latest-20230501/bl_ui/utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/blf.py` & `fake-bpy-module-latest-20230501/blf.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bmesh/__init__.py` & `fake-bpy-module-latest-20230501/bmesh/__init__.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bmesh/geometry.py` & `fake-bpy-module-latest-20230501/bmesh/geometry.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bmesh/ops.py` & `fake-bpy-module-latest-20230501/bmesh/ops.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bmesh/types.py` & `fake-bpy-module-latest-20230501/bmesh/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bmesh/utils.py` & `fake-bpy-module-latest-20230501/bmesh/utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/app/__init__.py` & `fake-bpy-module-latest-20230501/bpy/app/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 import typing
 from . import handlers
-from . import translations
-from . import icons
 from . import timers
+from . import icons
+from . import translations
 
 GenericType = typing.TypeVar("GenericType")
 
 
 def is_job_running(job_type: typing.Optional[str]) -> typing.Any:
     ''' Check whether a job of the given type is running.
```

### Comparing `fake-bpy-module-latest-20230430/bpy/app/handlers.py` & `fake-bpy-module-latest-20230501/bpy/app/handlers.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/app/icons.py` & `fake-bpy-module-latest-20230501/bpy/app/icons.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/app/timers.py` & `fake-bpy-module-latest-20230501/bpy/app/timers.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/app/translations.py` & `fake-bpy-module-latest-20230501/bpy/app/translations.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/msgbus.py` & `fake-bpy-module-latest-20230501/bpy/msgbus.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/__init__.py` & `fake-bpy-module-latest-20230501/bpy/ops/__init__.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,79 +1,79 @@
 import sys
 import typing
-from . import lattice
-from . import armature
-from . import cloth
-from . import boid
+from . import buttons
+from . import workspace
+from . import screen
+from . import node
+from . import file
+from . import transform
+from . import particle
+from . import cachefile
+from . import import_mesh
+from . import rigidbody
 from . import scene
 from . import paint
-from . import geometry
-from . import object
-from . import gpencil
 from . import dpaint
-from . import marker
-from . import brush
-from . import uilist
-from . import preferences
-from . import rigidbody
+from . import sequencer
+from . import object
+from . import fluid
+from . import script
+from . import mesh
+from . import action
+from . import curves
+from . import image
+from . import sculpt
+from . import curve
+from . import sculpt_curves
+from . import mask
+from . import cloth
+from . import paintcurve
+from . import ed
+from . import clip
 from . import pose
-from . import text
+from . import view3d
 from . import export_anim
-from . import texture
-from . import ed
+from . import uilist
+from . import uv
+from . import marker
+from . import text
+from . import brush
+from . import outliner
 from . import import_scene
-from . import sculpt
-from . import curve
-from . import action
-from . import material
+from . import ui
 from . import spreadsheet
-from . import wm
-from . import paintcurve
-from . import curves
-from . import buttons
-from . import mball
-from . import gizmogroup
-from . import info
+from . import surface
+from . import geometry
 from . import cycles
-from . import particle
-from . import outliner
-from . import camera
-from . import import_anim
-from . import import_curve
-from . import sequencer
-from . import sound
-from . import fluid
-from . import transform
 from . import view2d
-from . import palette
+from . import gizmogroup
+from . import export_mesh
+from . import anim
+from . import wm
 from . import ptcache
-from . import cachefile
-from . import graph
+from . import material
+from . import world
+from . import asset
+from . import import_anim
+from . import sound
+from . import render
+from . import boid
+from . import gpencil
 from . import export_scene
-from . import image
-from . import console
-from . import node
-from . import sculpt_curves
-from . import script
-from . import mask
-from . import font
-from . import workspace
+from . import mball
+from . import import_curve
+from . import palette
 from . import collection
+from . import camera
 from . import poselib
-from . import nla
-from . import render
-from . import import_mesh
-from . import mesh
+from . import graph
+from . import armature
+from . import font
 from . import constraint
-from . import world
-from . import anim
-from . import view3d
-from . import asset
-from . import surface
-from . import clip
-from . import uv
-from . import ui
-from . import export_mesh
-from . import file
-from . import screen
+from . import preferences
+from . import info
+from . import nla
+from . import console
+from . import texture
+from . import lattice
 
 GenericType = typing.TypeVar("GenericType")
```

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/action.py` & `fake-bpy-module-latest-20230501/bpy/ops/action.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/anim.py` & `fake-bpy-module-latest-20230501/bpy/ops/anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/armature.py` & `fake-bpy-module-latest-20230501/bpy/ops/armature.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/asset.py` & `fake-bpy-module-latest-20230501/bpy/ops/asset.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/boid.py` & `fake-bpy-module-latest-20230501/bpy/ops/boid.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/brush.py` & `fake-bpy-module-latest-20230501/bpy/ops/brush.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/buttons.py` & `fake-bpy-module-latest-20230501/bpy/ops/buttons.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/cachefile.py` & `fake-bpy-module-latest-20230501/bpy/ops/cachefile.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/camera.py` & `fake-bpy-module-latest-20230501/bpy/ops/camera.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/clip.py` & `fake-bpy-module-latest-20230501/bpy/ops/clip.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/cloth.py` & `fake-bpy-module-latest-20230501/bpy/ops/cloth.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/collection.py` & `fake-bpy-module-latest-20230501/bpy/ops/collection.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/console.py` & `fake-bpy-module-latest-20230501/bpy/ops/console.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/constraint.py` & `fake-bpy-module-latest-20230501/bpy/ops/constraint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/curve.py` & `fake-bpy-module-latest-20230501/bpy/ops/curve.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/curves.py` & `fake-bpy-module-latest-20230501/bpy/ops/curves.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/cycles.py` & `fake-bpy-module-latest-20230501/bpy/ops/cycles.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/dpaint.py` & `fake-bpy-module-latest-20230501/bpy/ops/dpaint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/ed.py` & `fake-bpy-module-latest-20230501/bpy/ops/ed.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/export_anim.py` & `fake-bpy-module-latest-20230501/bpy/ops/export_anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/export_mesh.py` & `fake-bpy-module-latest-20230501/bpy/ops/export_mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/export_scene.py` & `fake-bpy-module-latest-20230501/bpy/ops/export_scene.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/file.py` & `fake-bpy-module-latest-20230501/bpy/ops/file.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/fluid.py` & `fake-bpy-module-latest-20230501/bpy/ops/fluid.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/font.py` & `fake-bpy-module-latest-20230501/bpy/ops/font.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/geometry.py` & `fake-bpy-module-latest-20230501/bpy/ops/geometry.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/gizmogroup.py` & `fake-bpy-module-latest-20230501/bpy/ops/gizmogroup.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/gpencil.py` & `fake-bpy-module-latest-20230501/bpy/ops/gpencil.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/graph.py` & `fake-bpy-module-latest-20230501/bpy/ops/graph.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/image.py` & `fake-bpy-module-latest-20230501/bpy/ops/image.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/import_anim.py` & `fake-bpy-module-latest-20230501/bpy/ops/import_anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/import_curve.py` & `fake-bpy-module-latest-20230501/bpy/ops/import_curve.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/import_mesh.py` & `fake-bpy-module-latest-20230501/bpy/ops/import_mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/import_scene.py` & `fake-bpy-module-latest-20230501/bpy/ops/import_scene.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/info.py` & `fake-bpy-module-latest-20230501/bpy/ops/info.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/lattice.py` & `fake-bpy-module-latest-20230501/bpy/ops/lattice.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/marker.py` & `fake-bpy-module-latest-20230501/bpy/ops/marker.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/mask.py` & `fake-bpy-module-latest-20230501/bpy/ops/mask.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/material.py` & `fake-bpy-module-latest-20230501/bpy/ops/material.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/mball.py` & `fake-bpy-module-latest-20230501/bpy/ops/mball.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/mesh.py` & `fake-bpy-module-latest-20230501/bpy/ops/mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/nla.py` & `fake-bpy-module-latest-20230501/bpy/ops/nla.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/node.py` & `fake-bpy-module-latest-20230501/bpy/ops/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -615,15 +615,15 @@
 
 
 def gltf_settings_node_operator(
         override_context: typing.Union[typing.
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None):
-    ''' Add a node to the active tree for glTF export :File: `addons/io_scene_gltf2/blender/com/gltf2_blender_ui.py\:29 <https://projects.blender.org/blender/blender-addons/addons/io_scene_gltf2/blender/com/gltf2_blender_ui.py#L29>`__
+    ''' Add a node to the active tree for glTF export :File: `addons/io_scene_gltf2/blender/com/gltf2_blender_ui.py\:32 <https://projects.blender.org/blender/blender-addons/addons/io_scene_gltf2/blender/com/gltf2_blender_ui.py#L32>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -955,30 +955,30 @@
 
 
 def new_geometry_node_group_assign(
         override_context: typing.Union[typing.
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None):
-    ''' Create a new geometry node group and assign it to the active modifier :File: `startup/bl_operators/geometry_nodes.py\:233 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/geometry_nodes.py#L233>`__
+    ''' Create a new geometry node group and assign it to the active modifier :File: `startup/bl_operators/geometry_nodes.py\:234 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/geometry_nodes.py#L234>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
 
 
 def new_geometry_nodes_modifier(
         override_context: typing.Union[typing.
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None):
-    ''' Create a new modifier with a new geometry node group :File: `startup/bl_operators/geometry_nodes.py\:210 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/geometry_nodes.py#L210>`__
+    ''' Create a new modifier with a new geometry node group :File: `startup/bl_operators/geometry_nodes.py\:211 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/geometry_nodes.py#L211>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
```

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/object.py` & `fake-bpy-module-latest-20230501/bpy/ops/object.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
     pass
 
 
 def anim_transforms_to_deltas(override_context: typing.
                               Union[typing.Dict, 'bpy.types.Context'] = None,
                               execution_context: typing.Union[str, int] = None,
                               undo: typing.Optional[bool] = None):
-    ''' Convert object animation for normal transforms to delta transforms :File: `startup/bl_operators/object.py\:771 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L771>`__
+    ''' Convert object animation for normal transforms to delta transforms :File: `startup/bl_operators/object.py\:776 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L776>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -157,15 +157,15 @@
         override_context: typing.Union[typing.
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None,
         *,
         process_data: typing.Union[bool, typing.Any] = True,
         process_bones: typing.Union[bool, typing.Any] = True):
-    ''' Assign the current values of custom properties as their defaults, for use as part of the rest pose state in NLA track mixing :File: `startup/bl_operators/object.py\:995 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L995>`__
+    ''' Assign the current values of custom properties as their defaults, for use as part of the rest pose state in NLA track mixing :File: `startup/bl_operators/object.py\:1000 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L1000>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param process_data: Process data properties
     :type process_data: typing.Union[bool, typing.Any]
     :param process_bones: Process bone properties
@@ -1234,15 +1234,15 @@
 
 
 def geometry_nodes_move_to_nodes(
         override_context: typing.Union[typing.
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None):
-    ''' Move inputs and outputs from in the modifier to a new node group :File: `startup/bl_operators/geometry_nodes.py\:113 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/geometry_nodes.py#L113>`__
+    ''' Move inputs and outputs from in the modifier to a new node group :File: `startup/bl_operators/geometry_nodes.py\:114 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/geometry_nodes.py#L114>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -1476,15 +1476,15 @@
     pass
 
 
 def hide_render_clear_all(override_context: typing.
                           Union[typing.Dict, 'bpy.types.Context'] = None,
                           execution_context: typing.Union[str, int] = None,
                           undo: typing.Optional[bool] = None):
-    ''' Reveal all render objects by setting the hide render flag :File: `startup/bl_operators/object.py\:678 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L678>`__
+    ''' Reveal all render objects by setting the hide render flag :File: `startup/bl_operators/object.py\:683 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L683>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -1649,58 +1649,58 @@
 
 
 def instance_offset_from_cursor(
         override_context: typing.Union[typing.
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None):
-    ''' Set offset used for collection instances based on cursor position :File: `startup/bl_operators/object.py\:856 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L856>`__
+    ''' Set offset used for collection instances based on cursor position :File: `startup/bl_operators/object.py\:861 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L861>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
 
 
 def instance_offset_from_object(
         override_context: typing.Union[typing.
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None):
-    ''' Set offset used for collection instances based on the active object position :File: `startup/bl_operators/object.py\:888 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L888>`__
+    ''' Set offset used for collection instances based on the active object position :File: `startup/bl_operators/object.py\:893 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L893>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
 
 
 def instance_offset_to_cursor(override_context: typing.
                               Union[typing.Dict, 'bpy.types.Context'] = None,
                               execution_context: typing.Union[str, int] = None,
                               undo: typing.Optional[bool] = None):
-    ''' Set cursor position to the offset used for collection instances :File: `startup/bl_operators/object.py\:871 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L871>`__
+    ''' Set cursor position to the offset used for collection instances :File: `startup/bl_operators/object.py\:876 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L876>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
 
 
 def isolate_type_render(override_context: typing.
                         Union[typing.Dict, 'bpy.types.Context'] = None,
                         execution_context: typing.Union[str, int] = None,
                         undo: typing.Optional[bool] = None):
-    ''' Hide unselected render objects of same type as active by setting the hide render flag :File: `startup/bl_operators/object.py\:658 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L658>`__
+    ''' Hide unselected render objects of same type as active by setting the hide render flag :File: `startup/bl_operators/object.py\:663 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L663>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -1956,15 +1956,15 @@
                           execution_context: typing.Union[str, int] = None,
                           undo: typing.Optional[bool] = None,
                           *,
                           filepath: typing.Union[str, typing.Any] = "",
                           filter_image: typing.Union[bool, typing.Any] = True,
                           filter_folder: typing.Union[bool, typing.Any] = True,
                           view_align: typing.Union[bool, typing.Any] = True):
-    ''' Add a reference image into the background behind objects :File: `startup/bl_operators/object.py\:919 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L919>`__
+    ''' Add a reference image into the background behind objects :File: `startup/bl_operators/object.py\:924 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L924>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param filepath: filepath
     :type filepath: typing.Union[str, typing.Any]
     :param filter_image: filter_image
@@ -1983,15 +1983,15 @@
                          execution_context: typing.Union[str, int] = None,
                          undo: typing.Optional[bool] = None,
                          *,
                          filepath: typing.Union[str, typing.Any] = "",
                          filter_image: typing.Union[bool, typing.Any] = True,
                          filter_folder: typing.Union[bool, typing.Any] = True,
                          view_align: typing.Union[bool, typing.Any] = True):
-    ''' Add a reference image into the scene between objects :File: `startup/bl_operators/object.py\:919 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L919>`__
+    ''' Add a reference image into the scene between objects :File: `startup/bl_operators/object.py\:924 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L924>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param filepath: filepath
     :type filepath: typing.Union[str, typing.Any]
     :param filter_image: filter_image
@@ -4146,15 +4146,15 @@
 def transforms_to_deltas(override_context: typing.
                          Union[typing.Dict, 'bpy.types.Context'] = None,
                          execution_context: typing.Union[str, int] = None,
                          undo: typing.Optional[bool] = None,
                          *,
                          mode: typing.Optional[typing.Any] = 'ALL',
                          reset_values: typing.Union[bool, typing.Any] = True):
-    ''' Convert normal object transforms to delta transforms, any existing delta transforms will be included as well :File: `startup/bl_operators/object.py\:713 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L713>`__
+    ''' Convert normal object transforms to delta transforms, any existing delta transforms will be included as well :File: `startup/bl_operators/object.py\:718 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/object.py#L718>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param mode: Mode, Which transforms to transfer * ``ALL`` All Transforms -- Transfer location, rotation, and scale transforms. * ``LOC`` Location -- Transfer location transforms only. * ``ROT`` Rotation -- Transfer rotation transforms only. * ``SCALE`` Scale -- Transfer scale transforms only.
     :type mode: typing.Optional[typing.Any]
     :param reset_values: Reset Values, Clear transform values after transferring to deltas
```

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/outliner.py` & `fake-bpy-module-latest-20230501/bpy/ops/outliner.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/paint.py` & `fake-bpy-module-latest-20230501/bpy/ops/paint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/paintcurve.py` & `fake-bpy-module-latest-20230501/bpy/ops/paintcurve.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/palette.py` & `fake-bpy-module-latest-20230501/bpy/ops/palette.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/particle.py` & `fake-bpy-module-latest-20230501/bpy/ops/particle.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/pose.py` & `fake-bpy-module-latest-20230501/bpy/ops/pose.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/poselib.py` & `fake-bpy-module-latest-20230501/bpy/ops/poselib.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/preferences.py` & `fake-bpy-module-latest-20230501/bpy/ops/preferences.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/ptcache.py` & `fake-bpy-module-latest-20230501/bpy/ops/ptcache.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/render.py` & `fake-bpy-module-latest-20230501/bpy/ops/render.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/rigidbody.py` & `fake-bpy-module-latest-20230501/bpy/ops/rigidbody.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/scene.py` & `fake-bpy-module-latest-20230501/bpy/ops/scene.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/screen.py` & `fake-bpy-module-latest-20230501/bpy/ops/screen.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/script.py` & `fake-bpy-module-latest-20230501/bpy/ops/script.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/sculpt.py` & `fake-bpy-module-latest-20230501/bpy/ops/sculpt.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/sculpt_curves.py` & `fake-bpy-module-latest-20230501/bpy/ops/sculpt_curves.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/sequencer.py` & `fake-bpy-module-latest-20230501/bpy/ops/sequencer.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,15 +220,15 @@
 
 def delete(override_context: typing.Union[typing.
                                           Dict, 'bpy.types.Context'] = None,
            execution_context: typing.Union[str, int] = None,
            undo: typing.Optional[bool] = None,
            *,
            delete_data: typing.Union[bool, typing.Any] = False):
-    ''' Erase selected strips from the sequencer
+    ''' Delete selected strips from the sequencer
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param delete_data: Delete Data, After removing the Strip, delete the associated data also
     :type delete_data: typing.Union[bool, typing.Any]
     '''
```

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/sound.py` & `fake-bpy-module-latest-20230501/bpy/ops/sound.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/spreadsheet.py` & `fake-bpy-module-latest-20230501/bpy/ops/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/surface.py` & `fake-bpy-module-latest-20230501/bpy/ops/surface.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/text.py` & `fake-bpy-module-latest-20230501/bpy/ops/text.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/texture.py` & `fake-bpy-module-latest-20230501/bpy/ops/texture.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/transform.py` & `fake-bpy-module-latest-20230501/bpy/ops/transform.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/ui.py` & `fake-bpy-module-latest-20230501/bpy/ops/ui.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/uilist.py` & `fake-bpy-module-latest-20230501/bpy/ops/uilist.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
                Union[typing.Dict, 'bpy.types.Context'] = None,
                execution_context: typing.Union[str, int] = None,
                undo: typing.Optional[bool] = None,
                *,
                list_path: typing.Union[str, typing.Any] = "",
                active_index_path: typing.Union[str, typing.Any] = "",
                direction: typing.Optional[typing.Any] = 'UP'):
-    ''' Move an entry in the list up or down :File: `startup/bl_ui/generic_ui_list.py\:234 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_ui/generic_ui_list.py#L234>`__
+    ''' Move an entry in the list up or down :File: `startup/bl_ui/generic_ui_list.py\:236 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_ui/generic_ui_list.py#L236>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param list_path: list_path
     :type list_path: typing.Union[str, typing.Any]
     :param active_index_path: active_index_path
```

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/uv.py` & `fake-bpy-module-latest-20230501/bpy/ops/uv.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/view2d.py` & `fake-bpy-module-latest-20230501/bpy/ops/view2d.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/view3d.py` & `fake-bpy-module-latest-20230501/bpy/ops/view3d.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/wm.py` & `fake-bpy-module-latest-20230501/bpy/ops/wm.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/workspace.py` & `fake-bpy-module-latest-20230501/bpy/ops/workspace.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/ops/world.py` & `fake-bpy-module-latest-20230501/bpy/ops/world.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/path.py` & `fake-bpy-module-latest-20230501/bpy/path.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/props.py` & `fake-bpy-module-latest-20230501/bpy/props.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/types.py` & `fake-bpy-module-latest-20230501/bpy/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,173 +1,173 @@
 00000000: 696d 706f 7274 2073 7973 0a69 6d70 6f72  import sys.impor
 00000010: 7420 7479 7069 6e67 0a69 6d70 6f72 7420  t typing.import 
 00000020: 6d61 7468 7574 696c 730a 696d 706f 7274  mathutils.import
 00000030: 2062 7079 0a69 6d70 6f72 7420 626c 5f75   bpy.import bl_u
-00000040: 692e 7072 6f70 6572 7469 6573 5f70 6879  i.properties_phy
-00000050: 7369 6373 5f66 6c75 6964 0a69 6d70 6f72  sics_fluid.impor
-00000060: 7420 626c 5f6f 7065 7261 746f 7273 2e70  t bl_operators.p
-00000070: 7265 7365 7473 0a69 6d70 6f72 7420 626c  resets.import bl
-00000080: 5f75 692e 7072 6f70 6572 7469 6573 5f77  _ui.properties_w
-00000090: 6f72 6c64 0a69 6d70 6f72 7420 626c 5f75  orld.import bl_u
-000000a0: 692e 7072 6f70 6572 7469 6573 5f6f 7574  i.properties_out
-000000b0: 7075 740a 696d 706f 7274 2062 6c5f 7569  put.import bl_ui
-000000c0: 2e70 726f 7065 7274 6965 735f 6461 7461  .properties_data
-000000d0: 5f63 616d 6572 610a 696d 706f 7274 2062  _camera.import b
-000000e0: 6c5f 7569 2e73 7061 6365 5f6e 6f64 650a  l_ui.space_node.
-000000f0: 696d 706f 7274 2062 6c5f 7569 2e73 7061  import bl_ui.spa
-00000100: 6365 5f63 6c69 700a 696d 706f 7274 2062  ce_clip.import b
-00000110: 6c5f 6f70 6572 6174 6f72 732e 6e6f 6465  l_operators.node
-00000120: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
-00000130: 6f70 6572 7469 6573 5f63 6f6c 6c65 6374  operties_collect
-00000140: 696f 6e0a 696d 706f 7274 2062 6c5f 7569  ion.import bl_ui
-00000150: 2e70 726f 7065 7274 6965 735f 6461 7461  .properties_data
-00000160: 5f61 726d 6174 7572 650a 696d 706f 7274  _armature.import
-00000170: 2062 6c5f 7569 2e73 7061 6365 5f69 6d61   bl_ui.space_ima
-00000180: 6765 0a69 6d70 6f72 7420 626c 5f75 692e  ge.import bl_ui.
-00000190: 7370 6163 655f 746f 7062 6172 0a69 6d70  space_topbar.imp
-000001a0: 6f72 7420 626c 5f75 692e 6e6f 6465 5f61  ort bl_ui.node_a
-000001b0: 6464 5f6d 656e 755f 6765 6f6d 6574 7279  dd_menu_geometry
-000001c0: 0a69 6d70 6f72 7420 626c 5f6f 7065 7261  .import bl_opera
-000001d0: 746f 7273 2e63 6f6e 7374 7261 696e 740a  tors.constraint.
-000001e0: 696d 706f 7274 2062 6c5f 7569 2e73 7061  import bl_ui.spa
-000001f0: 6365 5f66 696c 6562 726f 7773 6572 0a69  ce_filebrowser.i
-00000200: 6d70 6f72 7420 626c 5f6f 7065 7261 746f  mport bl_operato
-00000210: 7273 2e77 6d0a 696d 706f 7274 2062 6c5f  rs.wm.import bl_
-00000220: 7569 2e70 726f 7065 7274 6965 735f 6772  ui.properties_gr
-00000230: 6561 7365 5f70 656e 6369 6c5f 636f 6d6d  ease_pencil_comm
-00000240: 6f6e 0a69 6d70 6f72 7420 626c 5f75 692e  on.import bl_ui.
-00000250: 7370 6163 655f 6e6c 610a 696d 706f 7274  space_nla.import
-00000260: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
-00000270: 735f 7068 7973 6963 735f 7269 6769 6462  s_physics_rigidb
-00000280: 6f64 795f 636f 6e73 7472 6169 6e74 0a69  ody_constraint.i
-00000290: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
-000002a0: 6572 7469 6573 5f64 6174 615f 706f 696e  erties_data_poin
-000002b0: 7463 6c6f 7564 0a69 6d70 6f72 7420 626c  tcloud.import bl
-000002c0: 5f75 692e 7072 6f70 6572 7469 6573 5f64  _ui.properties_d
-000002d0: 6174 615f 6d65 7461 6261 6c6c 0a69 6d70  ata_metaball.imp
-000002e0: 6f72 7420 626c 5f75 692e 7370 6163 655f  ort bl_ui.space_
-000002f0: 7573 6572 7072 6566 0a69 6d70 6f72 7420  userpref.import 
-00000300: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
-00000310: 5f63 6f6e 7374 7261 696e 740a 696d 706f  _constraint.impo
-00000320: 7274 2062 6c5f 6f70 6572 6174 6f72 732e  rt bl_operators.
-00000330: 6672 6565 7374 796c 650a 696d 706f 7274  freestyle.import
-00000340: 2062 6c5f 7569 2e73 7061 6365 5f74 6f6f   bl_ui.space_too
-00000350: 6c73 7973 7465 6d5f 636f 6d6d 6f6e 0a69  lsystem_common.i
-00000360: 6d70 6f72 7420 626c 5f75 692e 7370 6163  mport bl_ui.spac
-00000370: 655f 7370 7265 6164 7368 6565 740a 696d  e_spreadsheet.im
-00000380: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
-00000390: 7274 6965 735f 7068 7973 6963 735f 7269  rties_physics_ri
-000003a0: 6769 6462 6f64 790a 696d 706f 7274 2062  gidbody.import b
-000003b0: 6c5f 7569 2e73 7061 6365 5f70 726f 7065  l_ui.space_prope
-000003c0: 7274 6965 730a 696d 706f 7274 2062 6c5f  rties.import bl_
-000003d0: 7569 2e70 726f 7065 7274 6965 735f 6461  ui.properties_da
-000003e0: 7461 5f6c 6967 6874 0a69 6d70 6f72 7420  ta_light.import 
-000003f0: 626c 5f75 692e 7370 6163 655f 7465 7874  bl_ui.space_text
-00000400: 0a69 6d70 6f72 7420 626c 5f75 692e 7370  .import bl_ui.sp
-00000410: 6163 655f 7669 6577 3364 5f74 6f6f 6c62  ace_view3d_toolb
-00000420: 6172 0a69 6d70 6f72 7420 626c 5f75 692e  ar.import bl_ui.
-00000430: 7072 6f70 6572 7469 6573 5f70 6879 7369  properties_physi
-00000440: 6373 5f63 6c6f 7468 0a69 6d70 6f72 7420  cs_cloth.import 
-00000450: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
-00000460: 5f70 6172 7469 636c 650a 696d 706f 7274  _particle.import
-00000470: 2062 6c5f 6f70 6572 6174 6f72 732e 6f62   bl_operators.ob
-00000480: 6a65 6374 0a69 6d70 6f72 7420 626c 5f75  ject.import bl_u
-00000490: 692e 7072 6f70 6572 7469 6573 5f76 6965  i.properties_vie
-000004a0: 775f 6c61 7965 720a 696d 706f 7274 2062  w_layer.import b
-000004b0: 6c5f 6f70 6572 6174 6f72 732e 7573 6572  l_operators.user
-000004c0: 7072 6566 0a69 6d70 6f72 7420 626c 5f75  pref.import bl_u
-000004d0: 692e 7072 6f70 6572 7469 6573 5f64 6174  i.properties_dat
-000004e0: 615f 6c69 6768 7470 726f 6265 0a69 6d70  a_lightprobe.imp
-000004f0: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
-00000500: 7469 6573 5f64 6174 615f 6d65 7368 0a69  ties_data_mesh.i
-00000510: 6d70 6f72 7420 626c 5f75 690a 696d 706f  mport bl_ui.impo
-00000520: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
-00000530: 6965 735f 6461 7461 5f6d 6f64 6966 6965  ies_data_modifie
-00000540: 720a 696d 706f 7274 2062 6c5f 7569 2e70  r.import bl_ui.p
-00000550: 726f 7065 7274 6965 735f 7068 7973 6963  roperties_physic
-00000560: 735f 636f 6d6d 6f6e 0a69 6d70 6f72 7420  s_common.import 
-00000570: 626c 5f75 692e 7370 6163 655f 6772 6170  bl_ui.space_grap
-00000580: 680a 696d 706f 7274 2062 6c5f 7569 2e70  h.import bl_ui.p
-00000590: 726f 7065 7274 6965 735f 6461 7461 5f63  roperties_data_c
-000005a0: 7572 7665 730a 696d 706f 7274 2062 6c5f  urves.import bl_
-000005b0: 6f70 6572 6174 6f72 732e 636c 6970 0a69  operators.clip.i
-000005c0: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
-000005d0: 6572 7469 6573 5f6d 6174 6572 6961 6c5f  erties_material_
-000005e0: 6770 656e 6369 6c0a 696d 706f 7274 2062  gpencil.import b
-000005f0: 6c5f 7569 2e67 656e 6572 6963 5f75 695f  l_ui.generic_ui_
-00000600: 6c69 7374 0a69 6d70 6f72 7420 626c 5f75  list.import bl_u
-00000610: 692e 7072 6f70 6572 7469 6573 5f64 6174  i.properties_dat
-00000620: 615f 7368 6164 6572 6678 0a69 6d70 6f72  a_shaderfx.impor
-00000630: 7420 626c 5f6f 7065 7261 746f 7273 2e73  t bl_operators.s
-00000640: 7072 6561 6473 6865 6574 0a69 6d70 6f72  preadsheet.impor
-00000650: 7420 626c 5f75 692e 7370 6163 655f 6f75  t bl_ui.space_ou
-00000660: 746c 696e 6572 0a69 6d70 6f72 7420 626c  tliner.import bl
-00000670: 5f75 692e 7370 6163 655f 696e 666f 0a69  _ui.space_info.i
-00000680: 6d70 6f72 7420 626c 5f75 692e 7370 6163  mport bl_ui.spac
-00000690: 655f 7374 6174 7573 6261 720a 696d 706f  e_statusbar.impo
-000006a0: 7274 2062 6c5f 7569 2e73 7061 6365 5f63  rt bl_ui.space_c
-000006b0: 6f6e 736f 6c65 0a69 6d70 6f72 7420 626c  onsole.import bl
-000006c0: 5f75 692e 7072 6f70 6572 7469 6573 5f72  _ui.properties_r
-000006d0: 656e 6465 720a 696d 706f 7274 2062 6c5f  ender.import bl_
-000006e0: 7569 2e70 726f 7065 7274 6965 735f 7465  ui.properties_te
-000006f0: 7874 7572 650a 696d 706f 7274 2062 6c5f  xture.import bl_
-00000700: 7569 2e73 7061 6365 5f73 6571 7565 6e63  ui.space_sequenc
-00000710: 6572 0a69 6d70 6f72 7420 626c 5f75 692e  er.import bl_ui.
-00000720: 7072 6f70 6572 7469 6573 5f64 6174 615f  properties_data_
-00000730: 656d 7074 790a 696d 706f 7274 2062 6c5f  empty.import bl_
-00000740: 6f70 6572 6174 6f72 732e 6669 6c65 0a69  operators.file.i
-00000750: 6d70 6f72 7420 626c 5f6f 7065 7261 746f  mport bl_operato
-00000760: 7273 2e61 7373 6574 730a 696d 706f 7274  rs.assets.import
-00000770: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
-00000780: 735f 7068 7973 6963 735f 6669 656c 640a  s_physics_field.
-00000790: 696d 706f 7274 2062 6c5f 6f70 6572 6174  import bl_operat
-000007a0: 6f72 732e 7669 6577 3364 0a69 6d70 6f72  ors.view3d.impor
-000007b0: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
-000007c0: 6573 5f70 6169 6e74 5f63 6f6d 6d6f 6e0a  es_paint_common.
-000007d0: 696d 706f 7274 2062 6c5f 7569 2e70 726f  import bl_ui.pro
-000007e0: 7065 7274 6965 735f 6461 7461 5f73 7065  perties_data_spe
-000007f0: 616b 6572 0a69 6d70 6f72 7420 626c 5f75  aker.import bl_u
-00000800: 692e 7072 6f70 6572 7469 6573 5f64 6174  i.properties_dat
-00000810: 615f 6770 656e 6369 6c0a 696d 706f 7274  a_gpencil.import
-00000820: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
-00000830: 735f 6461 7461 5f62 6f6e 650a 696d 706f  s_data_bone.impo
-00000840: 7274 2062 6c5f 6f70 6572 6174 6f72 732e  rt bl_operators.
-00000850: 616e 696d 0a69 6d70 6f72 7420 626c 5f75  anim.import bl_u
-00000860: 692e 7072 6f70 6572 7469 6573 5f64 6174  i.properties_dat
-00000870: 615f 766f 6c75 6d65 0a69 6d70 6f72 7420  a_volume.import 
-00000880: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
-00000890: 5f6f 626a 6563 740a 696d 706f 7274 2062  _object.import b
-000008a0: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
-000008b0: 6461 7461 5f63 7572 7665 0a69 6d70 6f72  data_curve.impor
-000008c0: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
-000008d0: 6573 5f64 6174 615f 6c61 7474 6963 650a  es_data_lattice.
-000008e0: 696d 706f 7274 2062 6c5f 7569 2e73 7061  import bl_ui.spa
-000008f0: 6365 5f64 6f70 6573 6865 6574 0a69 6d70  ce_dopesheet.imp
-00000900: 6f72 7420 626c 5f75 692e 7370 6163 655f  ort bl_ui.space_
-00000910: 746f 6f6c 7379 7374 656d 5f74 6f6f 6c62  toolsystem_toolb
-00000920: 6172 0a69 6d70 6f72 7420 626c 5f75 692e  ar.import bl_ui.
-00000930: 7072 6f70 6572 7469 6573 5f6d 6174 6572  properties_mater
-00000940: 6961 6c0a 696d 706f 7274 2062 6c5f 7569  ial.import bl_ui
-00000950: 2e73 7061 6365 5f76 6965 7733 640a 696d  .space_view3d.im
-00000960: 706f 7274 2062 6c5f 7569 2e73 7061 6365  port bl_ui.space
-00000970: 5f74 696d 650a 696d 706f 7274 2062 6c5f  _time.import bl_
-00000980: 7569 2e70 726f 7065 7274 6965 735f 7068  ui.properties_ph
-00000990: 7973 6963 735f 6479 6e61 6d69 6370 6169  ysics_dynamicpai
-000009a0: 6e74 0a69 6d70 6f72 7420 626c 5f75 692e  nt.import bl_ui.
-000009b0: 7072 6f70 6572 7469 6573 5f73 6365 6e65  properties_scene
-000009c0: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
-000009d0: 6f70 6572 7469 6573 5f66 7265 6573 7479  operties_freesty
-000009e0: 6c65 0a69 6d70 6f72 7420 626c 5f75 692e  le.import bl_ui.
-000009f0: 7072 6f70 6572 7469 6573 5f6d 6173 6b5f  properties_mask_
-00000a00: 636f 6d6d 6f6e 0a69 6d70 6f72 7420 626c  common.import bl
-00000a10: 5f75 692e 7072 6f70 6572 7469 6573 5f70  _ui.properties_p
-00000a20: 6879 7369 6373 5f73 6f66 7462 6f64 790a  hysics_softbody.
-00000a30: 696d 706f 7274 2062 6c5f 7569 2e70 726f  import bl_ui.pro
-00000a40: 7065 7274 6965 735f 776f 726b 7370 6163  perties_workspac
-00000a50: 650a 0a47 656e 6572 6963 5479 7065 203d  e..GenericType =
+00000040: 692e 7072 6f70 6572 7469 6573 5f64 6174  i.properties_dat
+00000050: 615f 6c61 7474 6963 650a 696d 706f 7274  a_lattice.import
+00000060: 2062 6c5f 7569 2e73 7061 6365 5f75 7365   bl_ui.space_use
+00000070: 7270 7265 660a 696d 706f 7274 2062 6c5f  rpref.import bl_
+00000080: 7569 2e70 726f 7065 7274 6965 735f 7068  ui.properties_ph
+00000090: 7973 6963 735f 6479 6e61 6d69 6370 6169  ysics_dynamicpai
+000000a0: 6e74 0a69 6d70 6f72 7420 626c 5f75 692e  nt.import bl_ui.
+000000b0: 7370 6163 655f 7669 6577 3364 0a69 6d70  space_view3d.imp
+000000c0: 6f72 7420 626c 5f75 692e 7370 6163 655f  ort bl_ui.space_
+000000d0: 696e 666f 0a69 6d70 6f72 7420 626c 5f75  info.import bl_u
+000000e0: 692e 7370 6163 655f 746f 6f6c 7379 7374  i.space_toolsyst
+000000f0: 656d 5f74 6f6f 6c62 6172 0a69 6d70 6f72  em_toolbar.impor
+00000100: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
+00000110: 6573 5f64 6174 615f 7370 6561 6b65 720a  es_data_speaker.
+00000120: 696d 706f 7274 2062 6c5f 7569 2e70 726f  import bl_ui.pro
+00000130: 7065 7274 6965 735f 7068 7973 6963 735f  perties_physics_
+00000140: 7269 6769 6462 6f64 790a 696d 706f 7274  rigidbody.import
+00000150: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
+00000160: 735f 7068 7973 6963 735f 736f 6674 626f  s_physics_softbo
+00000170: 6479 0a69 6d70 6f72 7420 626c 5f75 692e  dy.import bl_ui.
+00000180: 7072 6f70 6572 7469 6573 5f76 6965 775f  properties_view_
+00000190: 6c61 7965 720a 696d 706f 7274 2062 6c5f  layer.import bl_
+000001a0: 7569 2e70 726f 7065 7274 6965 735f 7068  ui.properties_ph
+000001b0: 7973 6963 735f 6669 656c 640a 696d 706f  ysics_field.impo
+000001c0: 7274 2062 6c5f 6f70 6572 6174 6f72 732e  rt bl_operators.
+000001d0: 636f 6e73 7472 6169 6e74 0a69 6d70 6f72  constraint.impor
+000001e0: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
+000001f0: 6573 5f66 7265 6573 7479 6c65 0a69 6d70  es_freestyle.imp
+00000200: 6f72 7420 626c 5f75 692e 7370 6163 655f  ort bl_ui.space_
+00000210: 7370 7265 6164 7368 6565 740a 696d 706f  spreadsheet.impo
+00000220: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
+00000230: 6965 735f 6d61 736b 5f63 6f6d 6d6f 6e0a  ies_mask_common.
+00000240: 696d 706f 7274 2062 6c5f 7569 2e73 7061  import bl_ui.spa
+00000250: 6365 5f74 6578 740a 696d 706f 7274 2062  ce_text.import b
+00000260: 6c5f 7569 2e73 7061 6365 5f69 6d61 6765  l_ui.space_image
+00000270: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
+00000280: 6f70 6572 7469 6573 5f6d 6174 6572 6961  operties_materia
+00000290: 6c0a 696d 706f 7274 2062 6c5f 7569 2e70  l.import bl_ui.p
+000002a0: 726f 7065 7274 6965 735f 7068 7973 6963  roperties_physic
+000002b0: 735f 636f 6d6d 6f6e 0a69 6d70 6f72 7420  s_common.import 
+000002c0: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
+000002d0: 5f64 6174 615f 7368 6164 6572 6678 0a69  _data_shaderfx.i
+000002e0: 6d70 6f72 7420 626c 5f6f 7065 7261 746f  mport bl_operato
+000002f0: 7273 2e61 6e69 6d0a 696d 706f 7274 2062  rs.anim.import b
+00000300: 6c5f 6f70 6572 6174 6f72 732e 6f62 6a65  l_operators.obje
+00000310: 6374 0a69 6d70 6f72 7420 626c 5f75 692e  ct.import bl_ui.
+00000320: 7072 6f70 6572 7469 6573 5f64 6174 615f  properties_data_
+00000330: 6361 6d65 7261 0a69 6d70 6f72 7420 626c  camera.import bl
+00000340: 5f6f 7065 7261 746f 7273 2e66 7265 6573  _operators.frees
+00000350: 7479 6c65 0a69 6d70 6f72 7420 626c 5f6f  tyle.import bl_o
+00000360: 7065 7261 746f 7273 2e6e 6f64 650a 696d  perators.node.im
+00000370: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
+00000380: 7274 6965 735f 7363 656e 650a 696d 706f  rties_scene.impo
+00000390: 7274 2062 6c5f 6f70 6572 6174 6f72 732e  rt bl_operators.
+000003a0: 7669 6577 3364 0a69 6d70 6f72 7420 626c  view3d.import bl
+000003b0: 5f6f 7065 7261 746f 7273 2e61 7373 6574  _operators.asset
+000003c0: 730a 696d 706f 7274 2062 6c5f 7569 2e70  s.import bl_ui.p
+000003d0: 726f 7065 7274 6965 735f 7465 7874 7572  roperties_textur
+000003e0: 650a 696d 706f 7274 2062 6c5f 7569 2e70  e.import bl_ui.p
+000003f0: 726f 7065 7274 6965 735f 6f75 7470 7574  roperties_output
+00000400: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
+00000410: 6f70 6572 7469 6573 5f70 6879 7369 6373  operties_physics
+00000420: 5f63 6c6f 7468 0a69 6d70 6f72 7420 626c  _cloth.import bl
+00000430: 5f75 692e 7370 6163 655f 7374 6174 7573  _ui.space_status
+00000440: 6261 720a 696d 706f 7274 2062 6c5f 7569  bar.import bl_ui
+00000450: 2e70 726f 7065 7274 6965 735f 6d61 7465  .properties_mate
+00000460: 7269 616c 5f67 7065 6e63 696c 0a69 6d70  rial_gpencil.imp
+00000470: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
+00000480: 7469 6573 5f63 6f6c 6c65 6374 696f 6e0a  ties_collection.
+00000490: 696d 706f 7274 2062 6c5f 7569 2e70 726f  import bl_ui.pro
+000004a0: 7065 7274 6965 735f 6461 7461 5f65 6d70  perties_data_emp
+000004b0: 7479 0a69 6d70 6f72 7420 626c 5f75 692e  ty.import bl_ui.
+000004c0: 7072 6f70 6572 7469 6573 5f64 6174 615f  properties_data_
+000004d0: 6375 7276 650a 696d 706f 7274 2062 6c5f  curve.import bl_
+000004e0: 7569 2e70 726f 7065 7274 6965 735f 6461  ui.properties_da
+000004f0: 7461 5f76 6f6c 756d 650a 696d 706f 7274  ta_volume.import
+00000500: 2062 6c5f 7569 2e73 7061 6365 5f74 6f6f   bl_ui.space_too
+00000510: 6c73 7973 7465 6d5f 636f 6d6d 6f6e 0a69  lsystem_common.i
+00000520: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
+00000530: 6572 7469 6573 5f64 6174 615f 626f 6e65  erties_data_bone
+00000540: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
+00000550: 6f70 6572 7469 6573 5f64 6174 615f 6c69  operties_data_li
+00000560: 6768 7470 726f 6265 0a69 6d70 6f72 7420  ghtprobe.import 
+00000570: 626c 5f75 692e 6765 6e65 7269 635f 7569  bl_ui.generic_ui
+00000580: 5f6c 6973 740a 696d 706f 7274 2062 6c5f  _list.import bl_
+00000590: 7569 2e70 726f 7065 7274 6965 735f 6461  ui.properties_da
+000005a0: 7461 5f6c 6967 6874 0a69 6d70 6f72 7420  ta_light.import 
+000005b0: 626c 5f75 692e 7370 6163 655f 7365 7175  bl_ui.space_sequ
+000005c0: 656e 6365 720a 696d 706f 7274 2062 6c5f  encer.import bl_
+000005d0: 7569 2e6e 6f64 655f 6164 645f 6d65 6e75  ui.node_add_menu
+000005e0: 5f67 656f 6d65 7472 790a 696d 706f 7274  _geometry.import
+000005f0: 2062 6c5f 6f70 6572 6174 6f72 732e 7573   bl_operators.us
+00000600: 6572 7072 6566 0a69 6d70 6f72 7420 626c  erpref.import bl
+00000610: 5f6f 7065 7261 746f 7273 2e77 6d0a 696d  _operators.wm.im
+00000620: 706f 7274 2062 6c5f 7569 2e73 7061 6365  port bl_ui.space
+00000630: 5f66 696c 6562 726f 7773 6572 0a69 6d70  _filebrowser.imp
+00000640: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
+00000650: 7469 6573 5f63 6f6e 7374 7261 696e 740a  ties_constraint.
+00000660: 696d 706f 7274 2062 6c5f 7569 2e73 7061  import bl_ui.spa
+00000670: 6365 5f76 6965 7733 645f 746f 6f6c 6261  ce_view3d_toolba
+00000680: 720a 696d 706f 7274 2062 6c5f 7569 2e70  r.import bl_ui.p
+00000690: 726f 7065 7274 6965 735f 6461 7461 5f6d  roperties_data_m
+000006a0: 6f64 6966 6965 720a 696d 706f 7274 2062  odifier.import b
+000006b0: 6c5f 7569 0a69 6d70 6f72 7420 626c 5f75  l_ui.import bl_u
+000006c0: 692e 7072 6f70 6572 7469 6573 5f64 6174  i.properties_dat
+000006d0: 615f 6d65 7368 0a69 6d70 6f72 7420 626c  a_mesh.import bl
+000006e0: 5f75 692e 7072 6f70 6572 7469 6573 5f64  _ui.properties_d
+000006f0: 6174 615f 6d65 7461 6261 6c6c 0a69 6d70  ata_metaball.imp
+00000700: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
+00000710: 7469 6573 5f70 6879 7369 6373 5f72 6967  ties_physics_rig
+00000720: 6964 626f 6479 5f63 6f6e 7374 7261 696e  idbody_constrain
+00000730: 740a 696d 706f 7274 2062 6c5f 7569 2e73  t.import bl_ui.s
+00000740: 7061 6365 5f74 6f70 6261 720a 696d 706f  pace_topbar.impo
+00000750: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
+00000760: 6965 735f 7061 7274 6963 6c65 0a69 6d70  ies_particle.imp
+00000770: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
+00000780: 7469 6573 5f70 6879 7369 6373 5f66 6c75  ties_physics_flu
+00000790: 6964 0a69 6d70 6f72 7420 626c 5f75 692e  id.import bl_ui.
+000007a0: 7072 6f70 6572 7469 6573 5f64 6174 615f  properties_data_
+000007b0: 6375 7276 6573 0a69 6d70 6f72 7420 626c  curves.import bl
+000007c0: 5f6f 7065 7261 746f 7273 2e63 6c69 700a  _operators.clip.
+000007d0: 696d 706f 7274 2062 6c5f 7569 2e73 7061  import bl_ui.spa
+000007e0: 6365 5f64 6f70 6573 6865 6574 0a69 6d70  ce_dopesheet.imp
+000007f0: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
+00000800: 7469 6573 5f64 6174 615f 6172 6d61 7475  ties_data_armatu
+00000810: 7265 0a69 6d70 6f72 7420 626c 5f75 692e  re.import bl_ui.
+00000820: 7072 6f70 6572 7469 6573 5f64 6174 615f  properties_data_
+00000830: 6770 656e 6369 6c0a 696d 706f 7274 2062  gpencil.import b
+00000840: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
+00000850: 7061 696e 745f 636f 6d6d 6f6e 0a69 6d70  paint_common.imp
+00000860: 6f72 7420 626c 5f75 692e 7370 6163 655f  ort bl_ui.space_
+00000870: 636f 6e73 6f6c 650a 696d 706f 7274 2062  console.import b
+00000880: 6c5f 7569 2e73 7061 6365 5f70 726f 7065  l_ui.space_prope
+00000890: 7274 6965 730a 696d 706f 7274 2062 6c5f  rties.import bl_
+000008a0: 6f70 6572 6174 6f72 732e 7072 6573 6574  operators.preset
+000008b0: 730a 696d 706f 7274 2062 6c5f 7569 2e70  s.import bl_ui.p
+000008c0: 726f 7065 7274 6965 735f 7265 6e64 6572  roperties_render
+000008d0: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
+000008e0: 6f70 6572 7469 6573 5f67 7265 6173 655f  operties_grease_
+000008f0: 7065 6e63 696c 5f63 6f6d 6d6f 6e0a 696d  pencil_common.im
+00000900: 706f 7274 2062 6c5f 7569 2e73 7061 6365  port bl_ui.space
+00000910: 5f63 6c69 700a 696d 706f 7274 2062 6c5f  _clip.import bl_
+00000920: 7569 2e73 7061 6365 5f74 696d 650a 696d  ui.space_time.im
+00000930: 706f 7274 2062 6c5f 7569 2e73 7061 6365  port bl_ui.space
+00000940: 5f67 7261 7068 0a69 6d70 6f72 7420 626c  _graph.import bl
+00000950: 5f75 692e 7370 6163 655f 6f75 746c 696e  _ui.space_outlin
+00000960: 6572 0a69 6d70 6f72 7420 626c 5f75 692e  er.import bl_ui.
+00000970: 7370 6163 655f 6e6f 6465 0a69 6d70 6f72  space_node.impor
+00000980: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
+00000990: 6573 5f64 6174 615f 706f 696e 7463 6c6f  es_data_pointclo
+000009a0: 7564 0a69 6d70 6f72 7420 626c 5f75 692e  ud.import bl_ui.
+000009b0: 7072 6f70 6572 7469 6573 5f77 6f72 6b73  properties_works
+000009c0: 7061 6365 0a69 6d70 6f72 7420 626c 5f75  pace.import bl_u
+000009d0: 692e 7072 6f70 6572 7469 6573 5f6f 626a  i.properties_obj
+000009e0: 6563 740a 696d 706f 7274 2062 6c5f 6f70  ect.import bl_op
+000009f0: 6572 6174 6f72 732e 6669 6c65 0a69 6d70  erators.file.imp
+00000a00: 6f72 7420 626c 5f6f 7065 7261 746f 7273  ort bl_operators
+00000a10: 2e73 7072 6561 6473 6865 6574 0a69 6d70  .spreadsheet.imp
+00000a20: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
+00000a30: 7469 6573 5f77 6f72 6c64 0a69 6d70 6f72  ties_world.impor
+00000a40: 7420 626c 5f75 692e 7370 6163 655f 6e6c  t bl_ui.space_nl
+00000a50: 610a 0a47 656e 6572 6963 5479 7065 203d  a..GenericType =
 00000a60: 2074 7970 696e 672e 5479 7065 5661 7228   typing.TypeVar(
 00000a70: 2247 656e 6572 6963 5479 7065 2229 0a0a  "GenericType")..
 00000a80: 0a63 6c61 7373 2062 7079 5f73 7472 7563  .class bpy_struc
 00000a90: 743a 0a20 2020 2027 2727 2062 7569 6c74  t:.    ''' built
 00000aa0: 2d69 6e20 6261 7365 2063 6c61 7373 2066  -in base class f
 00000ab0: 6f72 2061 6c6c 2063 6c61 7373 6573 2069  or all classes i
 00000ac0: 6e20 6270 792e 7479 7065 732e 0a20 2020  n bpy.types..   
@@ -23163,16 +23163,16 @@
 0005a7a0: 3a20 2745 7665 6e74 272c 0a20 2020 2020  : 'Event',.     
 0005a7b0: 2020 2020 2020 2020 2074 7765 616b 3a20           tweak: 
 0005a7c0: 7479 7069 6e67 2e55 6e69 6f6e 5b74 7970  typing.Union[typ
 0005a7d0: 696e 672e 5365 745b 7374 725d 2c20 7479  ing.Set[str], ty
 0005a7e0: 7069 6e67 2e53 6574 5b69 6e74 5d5d 0a20  ping.Set[int]]. 
 0005a7f0: 2020 2020 2020 2020 2020 2020 2029 202d               ) -
 0005a800: 3e20 7479 7069 6e67 2e55 6e69 6f6e 5b74  > typing.Union[t
-0005a810: 7970 696e 672e 5365 745b 7374 725d 2c20  yping.Set[str], 
-0005a820: 7479 7069 6e67 2e53 6574 5b69 6e74 5d5d  typing.Set[int]]
+0005a810: 7970 696e 672e 5365 745b 696e 745d 2c20  yping.Set[int], 
+0005a820: 7479 7069 6e67 2e53 6574 5b73 7472 5d5d  typing.Set[str]]
 0005a830: 3a0a 2020 2020 2020 2020 2727 2720 0a0a  :.        ''' ..
 0005a840: 2020 2020 2020 2020 3a70 6172 616d 2063          :param c
 0005a850: 6f6e 7465 7874 3a20 0a20 2020 2020 2020  ontext: .       
 0005a860: 203a 7479 7065 2063 6f6e 7465 7874 3a20   :type context: 
 0005a870: 2743 6f6e 7465 7874 270a 2020 2020 2020  'Context'.      
 0005a880: 2020 3a70 6172 616d 2065 7665 6e74 3a20    :param event: 
 0005a890: 0a20 2020 2020 2020 203a 7479 7065 2065  .        :type e
@@ -23181,42 +23181,42 @@
 0005a8c0: 616b 3a20 5477 6561 6b0a 2020 2020 2020  ak: Tweak.      
 0005a8d0: 2020 3a74 7970 6520 7477 6561 6b3a 2074    :type tweak: t
 0005a8e0: 7970 696e 672e 556e 696f 6e5b 7479 7069  yping.Union[typi
 0005a8f0: 6e67 2e53 6574 5b73 7472 5d2c 2074 7970  ng.Set[str], typ
 0005a900: 696e 672e 5365 745b 696e 745d 5d0a 2020  ing.Set[int]].  
 0005a910: 2020 2020 2020 3a72 7479 7065 3a20 7479        :rtype: ty
 0005a920: 7069 6e67 2e55 6e69 6f6e 5b74 7970 696e  ping.Union[typin
-0005a930: 672e 5365 745b 7374 725d 2c20 7479 7069  g.Set[str], typi
-0005a940: 6e67 2e53 6574 5b69 6e74 5d5d 0a20 2020  ng.Set[int]].   
+0005a930: 672e 5365 745b 696e 745d 2c20 7479 7069  g.Set[int], typi
+0005a940: 6e67 2e53 6574 5b73 7472 5d5d 0a20 2020  ng.Set[str]].   
 0005a950: 2020 2020 203a 7265 7475 726e 3a20 7265       :return: re
 0005a960: 7375 6c74 0a20 2020 2020 2020 2027 2727  sult.        '''
 0005a970: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
 0005a980: 2020 2064 6566 2073 6574 7570 2873 656c     def setup(sel
 0005a990: 6629 3a0a 2020 2020 2020 2020 2727 2720  f):.        ''' 
 0005a9a0: 0a0a 2020 2020 2020 2020 2727 270a 2020  ..        '''.  
 0005a9b0: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
 0005a9c0: 6465 6620 696e 766f 6b65 2873 656c 662c  def invoke(self,
 0005a9d0: 2063 6f6e 7465 7874 3a20 2743 6f6e 7465   context: 'Conte
 0005a9e0: 7874 272c 2065 7665 6e74 3a20 2745 7665  xt', event: 'Eve
 0005a9f0: 6e74 270a 2020 2020 2020 2020 2020 2020  nt'.            
 0005aa00: 2020 2029 202d 3e20 7479 7069 6e67 2e55     ) -> typing.U
 0005aa10: 6e69 6f6e 5b74 7970 696e 672e 5365 745b  nion[typing.Set[
-0005aa20: 7374 725d 2c20 7479 7069 6e67 2e53 6574  str], typing.Set
-0005aa30: 5b69 6e74 5d5d 3a0a 2020 2020 2020 2020  [int]]:.        
+0005aa20: 696e 745d 2c20 7479 7069 6e67 2e53 6574  int], typing.Set
+0005aa30: 5b73 7472 5d5d 3a0a 2020 2020 2020 2020  [str]]:.        
 0005aa40: 2727 2720 0a0a 2020 2020 2020 2020 3a70  ''' ..        :p
 0005aa50: 6172 616d 2063 6f6e 7465 7874 3a20 0a20  aram context: . 
 0005aa60: 2020 2020 2020 203a 7479 7065 2063 6f6e         :type con
 0005aa70: 7465 7874 3a20 2743 6f6e 7465 7874 270a  text: 'Context'.
 0005aa80: 2020 2020 2020 2020 3a70 6172 616d 2065          :param e
 0005aa90: 7665 6e74 3a20 0a20 2020 2020 2020 203a  vent: .        :
 0005aaa0: 7479 7065 2065 7665 6e74 3a20 2745 7665  type event: 'Eve
 0005aab0: 6e74 270a 2020 2020 2020 2020 3a72 7479  nt'.        :rty
 0005aac0: 7065 3a20 7479 7069 6e67 2e55 6e69 6f6e  pe: typing.Union
-0005aad0: 5b74 7970 696e 672e 5365 745b 7374 725d  [typing.Set[str]
-0005aae0: 2c20 7479 7069 6e67 2e53 6574 5b69 6e74  , typing.Set[int
+0005aad0: 5b74 7970 696e 672e 5365 745b 696e 745d  [typing.Set[int]
+0005aae0: 2c20 7479 7069 6e67 2e53 6574 5b73 7472  , typing.Set[str
 0005aaf0: 5d5d 0a20 2020 2020 2020 203a 7265 7475  ]].        :retu
 0005ab00: 726e 3a20 7265 7375 6c74 0a20 2020 2020  rn: result.     
 0005ab10: 2020 2027 2727 0a20 2020 2020 2020 2070     '''.        p
 0005ab20: 6173 730a 0a20 2020 2064 6566 2065 7869  ass..    def exi
 0005ab30: 7428 7365 6c66 2c20 636f 6e74 6578 743a  t(self, context:
 0005ab40: 2027 436f 6e74 6578 7427 2c20 6361 6e63   'Context', canc
 0005ab50: 656c 3a20 7479 7069 6e67 2e4f 7074 696f  el: typing.Optio
@@ -27339,24 +27339,24 @@
 0006aca0: 6e5b 7374 722c 2074 7970 696e 672e 416e  n[str, typing.An
 0006acb0: 795d 203d 204e 6f6e 650a 2020 2020 2727  y] = None.    ''
 0006acc0: 2720 0a0a 2020 2020 3a74 7970 653a 2074  ' ..    :type: t
 0006acd0: 7970 696e 672e 556e 696f 6e5b 7374 722c  yping.Union[str,
 0006ace0: 2074 7970 696e 672e 416e 795d 0a20 2020   typing.Any].   
 0006acf0: 2027 2727 0a0a 2020 2020 626c 5f6f 7074   '''..    bl_opt
 0006ad00: 696f 6e73 3a20 7479 7069 6e67 2e55 6e69  ions: typing.Uni
-0006ad10: 6f6e 5b74 7970 696e 672e 5365 745b 7374  on[typing.Set[st
-0006ad20: 725d 2c20 7479 7069 6e67 2e53 6574 5b69  r], typing.Set[i
-0006ad30: 6e74 5d5d 203d 204e 6f6e 650a 2020 2020  nt]] = None.    
+0006ad10: 6f6e 5b74 7970 696e 672e 5365 745b 696e  on[typing.Set[in
+0006ad20: 745d 2c20 7479 7069 6e67 2e53 6574 5b73  t], typing.Set[s
+0006ad30: 7472 5d5d 203d 204e 6f6e 650a 2020 2020  tr]] = None.    
 0006ad40: 2727 2720 4b65 7969 6e67 2053 6574 206f  ''' Keying Set o
 0006ad50: 7074 696f 6e73 2074 6f20 7573 6520 7768  ptions to use wh
 0006ad60: 656e 2069 6e73 6572 7469 6e67 206b 6579  en inserting key
 0006ad70: 6672 616d 6573 0a0a 2020 2020 3a74 7970  frames..    :typ
 0006ad80: 653a 2074 7970 696e 672e 556e 696f 6e5b  e: typing.Union[
-0006ad90: 7479 7069 6e67 2e53 6574 5b73 7472 5d2c  typing.Set[str],
-0006ada0: 2074 7970 696e 672e 5365 745b 696e 745d   typing.Set[int]
+0006ad90: 7479 7069 6e67 2e53 6574 5b69 6e74 5d2c  typing.Set[int],
+0006ada0: 2074 7970 696e 672e 5365 745b 7374 725d   typing.Set[str]
 0006adb0: 5d0a 2020 2020 2727 270a 0a20 2020 2064  ].    '''..    d
 0006adc0: 6566 2070 6f6c 6c28 7365 6c66 2c20 636f  ef poll(self, co
 0006add0: 6e74 6578 743a 2074 7970 696e 672e 4f70  ntext: typing.Op
 0006ade0: 7469 6f6e 616c 5b27 436f 6e74 6578 7427  tional['Context'
 0006adf0: 5d29 3a0a 2020 2020 2020 2020 2727 2720  ]):.        ''' 
 0006ae00: 5465 7374 2069 6620 4b65 7969 6e67 2053  Test if Keying S
 0006ae10: 6574 2063 616e 2062 6520 7573 6564 206f  et can be used o
@@ -28100,23 +28100,23 @@
 0006dc30: 7479 7069 6e67 2e41 6e79 5d20 3d20 4e6f  typing.Any] = No
 0006dc40: 6e65 0a20 2020 2027 2727 200a 0a20 2020  ne.    ''' ..   
 0006dc50: 203a 7479 7065 3a20 7479 7069 6e67 2e55   :type: typing.U
 0006dc60: 6e69 6f6e 5b73 7472 2c20 7479 7069 6e67  nion[str, typing
 0006dc70: 2e41 6e79 5d0a 2020 2020 2727 270a 0a20  .Any].    '''.. 
 0006dc80: 2020 2062 6c5f 6f70 7469 6f6e 733a 2074     bl_options: t
 0006dc90: 7970 696e 672e 556e 696f 6e5b 7479 7069  yping.Union[typi
-0006dca0: 6e67 2e53 6574 5b73 7472 5d2c 2074 7970  ng.Set[str], typ
-0006dcb0: 696e 672e 5365 745b 696e 745d 5d20 3d20  ing.Set[int]] = 
+0006dca0: 6e67 2e53 6574 5b69 6e74 5d2c 2074 7970  ng.Set[int], typ
+0006dcb0: 696e 672e 5365 745b 7374 725d 5d20 3d20  ing.Set[str]] = 
 0006dcc0: 4e6f 6e65 0a20 2020 2027 2727 204f 7074  None.    ''' Opt
 0006dcd0: 696f 6e73 2066 6f72 2074 6869 7320 6f70  ions for this op
 0006dce0: 6572 6174 6f72 2074 7970 650a 0a20 2020  erator type..   
 0006dcf0: 203a 7479 7065 3a20 7479 7069 6e67 2e55   :type: typing.U
 0006dd00: 6e69 6f6e 5b74 7970 696e 672e 5365 745b  nion[typing.Set[
-0006dd10: 7374 725d 2c20 7479 7069 6e67 2e53 6574  str], typing.Set
-0006dd20: 5b69 6e74 5d5d 0a20 2020 2027 2727 0a0a  [int]].    '''..
+0006dd10: 696e 745d 2c20 7479 7069 6e67 2e53 6574  int], typing.Set
+0006dd20: 5b73 7472 5d5d 0a20 2020 2027 2727 0a0a  [str]].    '''..
 0006dd30: 2020 2020 626c 5f74 7261 6e73 6c61 7469      bl_translati
 0006dd40: 6f6e 5f63 6f6e 7465 7874 3a20 7479 7069  on_context: typi
 0006dd50: 6e67 2e55 6e69 6f6e 5b73 7472 2c20 7479  ng.Union[str, ty
 0006dd60: 7069 6e67 2e41 6e79 5d20 3d20 4e6f 6e65  ping.Any] = None
 0006dd70: 0a20 2020 2027 2727 200a 0a20 2020 203a  .    ''' ..    :
 0006dd80: 7479 7065 3a20 7479 7069 6e67 2e55 6e69  type: typing.Uni
 0006dd90: 6f6e 5b73 7472 2c20 7479 7069 6e67 2e41  on[str, typing.A
@@ -28151,27 +28151,27 @@
 0006df60: 5072 6f70 6572 7469 6573 2720 3d20 4e6f  Properties' = No
 0006df70: 6e65 0a20 2020 2027 2727 200a 0a20 2020  ne.    ''' ..   
 0006df80: 203a 7479 7065 3a20 274f 7065 7261 746f   :type: 'Operato
 0006df90: 7250 726f 7065 7274 6965 7327 0a20 2020  rProperties'.   
 0006dfa0: 2027 2727 0a0a 2020 2020 6465 6620 7265   '''..    def re
 0006dfb0: 706f 7274 2873 656c 662c 2074 7970 653a  port(self, type:
 0006dfc0: 2074 7970 696e 672e 556e 696f 6e5b 7479   typing.Union[ty
-0006dfd0: 7069 6e67 2e53 6574 5b73 7472 5d2c 2074  ping.Set[str], t
-0006dfe0: 7970 696e 672e 5365 745b 696e 745d 5d2c  yping.Set[int]],
+0006dfd0: 7069 6e67 2e53 6574 5b69 6e74 5d2c 2074  ping.Set[int], t
+0006dfe0: 7970 696e 672e 5365 745b 7374 725d 5d2c  yping.Set[str]],
 0006dff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0006e000: 6d65 7373 6167 653a 2074 7970 696e 672e  message: typing.
 0006e010: 556e 696f 6e5b 7374 722c 2074 7970 696e  Union[str, typin
 0006e020: 672e 416e 795d 293a 0a20 2020 2020 2020  g.Any]):.       
 0006e030: 2027 2727 2072 6570 6f72 740a 0a20 2020   ''' report..   
 0006e040: 2020 2020 203a 7061 7261 6d20 7479 7065       :param type
 0006e050: 3a20 5479 7065 0a20 2020 2020 2020 203a  : Type.        :
 0006e060: 7479 7065 2074 7970 653a 2074 7970 696e  type type: typin
 0006e070: 672e 556e 696f 6e5b 7479 7069 6e67 2e53  g.Union[typing.S
-0006e080: 6574 5b73 7472 5d2c 2074 7970 696e 672e  et[str], typing.
-0006e090: 5365 745b 696e 745d 5d0a 2020 2020 2020  Set[int]].      
+0006e080: 6574 5b69 6e74 5d2c 2074 7970 696e 672e  et[int], typing.
+0006e090: 5365 745b 7374 725d 5d0a 2020 2020 2020  Set[str]].      
 0006e0a0: 2020 3a70 6172 616d 206d 6573 7361 6765    :param message
 0006e0b0: 3a20 5265 706f 7274 204d 6573 7361 6765  : Report Message
 0006e0c0: 0a20 2020 2020 2020 203a 7479 7065 206d  .        :type m
 0006e0d0: 6573 7361 6765 3a20 7479 7069 6e67 2e55  essage: typing.U
 0006e0e0: 6e69 6f6e 5b73 7472 2c20 7479 7069 6e67  nion[str, typing
 0006e0f0: 2e41 6e79 5d0a 2020 2020 2020 2020 2727  .Any].        ''
 0006e100: 270a 2020 2020 2020 2020 7061 7373 0a0a  '.        pass..
@@ -37222,23 +37222,23 @@
 00091650: 6f6e 5b73 7472 2c20 7479 7069 6e67 2e41  on[str, typing.A
 00091660: 6e79 5d20 3d20 4e6f 6e65 0a20 2020 2027  ny] = None.    '
 00091670: 2727 200a 0a20 2020 203a 7479 7065 3a20  '' ..    :type: 
 00091680: 7479 7069 6e67 2e55 6e69 6f6e 5b73 7472  typing.Union[str
 00091690: 2c20 7479 7069 6e67 2e41 6e79 5d0a 2020  , typing.Any].  
 000916a0: 2020 2727 270a 0a20 2020 2062 6c5f 6f70    '''..    bl_op
 000916b0: 7469 6f6e 733a 2074 7970 696e 672e 556e  tions: typing.Un
-000916c0: 696f 6e5b 7479 7069 6e67 2e53 6574 5b73  ion[typing.Set[s
-000916d0: 7472 5d2c 2074 7970 696e 672e 5365 745b  tr], typing.Set[
-000916e0: 696e 745d 5d20 3d20 4e6f 6e65 0a20 2020  int]] = None.   
+000916c0: 696f 6e5b 7479 7069 6e67 2e53 6574 5b69  ion[typing.Set[i
+000916d0: 6e74 5d2c 2074 7970 696e 672e 5365 745b  nt], typing.Set[
+000916e0: 7374 725d 5d20 3d20 4e6f 6e65 0a20 2020  str]] = None.   
 000916f0: 2027 2727 204f 7074 696f 6e73 2066 6f72   ''' Options for
 00091700: 2074 6869 7320 6f70 6572 6174 6f72 2074   this operator t
 00091710: 7970 650a 0a20 2020 203a 7479 7065 3a20  ype..    :type: 
 00091720: 7479 7069 6e67 2e55 6e69 6f6e 5b74 7970  typing.Union[typ
-00091730: 696e 672e 5365 745b 7374 725d 2c20 7479  ing.Set[str], ty
-00091740: 7069 6e67 2e53 6574 5b69 6e74 5d5d 0a20  ping.Set[int]]. 
+00091730: 696e 672e 5365 745b 696e 745d 2c20 7479  ing.Set[int], ty
+00091740: 7069 6e67 2e53 6574 5b73 7472 5d5d 0a20  ping.Set[str]]. 
 00091750: 2020 2027 2727 0a0a 2020 2020 626c 5f74     '''..    bl_t
 00091760: 7261 6e73 6c61 7469 6f6e 5f63 6f6e 7465  ranslation_conte
 00091770: 7874 3a20 7479 7069 6e67 2e55 6e69 6f6e  xt: typing.Union
 00091780: 5b73 7472 2c20 7479 7069 6e67 2e41 6e79  [str, typing.Any
 00091790: 5d20 3d20 4e6f 6e65 0a20 2020 2027 2727  ] = None.    '''
 000917a0: 200a 0a20 2020 203a 7479 7065 3a20 7479   ..    :type: ty
 000917b0: 7069 6e67 2e55 6e69 6f6e 5b73 7472 2c20  ping.Union[str, 
@@ -37305,27 +37305,27 @@
 00091b80: 7065 7274 7920 7768 656e 2065 7870 616e  perty when expan
 00091b90: 6469 6e67 2061 6e20 6f70 6572 6174 6f72  ding an operator
 00091ba0: 2069 6e74 6f20 6120 6d65 6e75 2e0a 0a20   into a menu... 
 00091bb0: 2020 203a 7479 7065 3a20 7374 720a 2020     :type: str.  
 00091bc0: 2020 2727 270a 0a20 2020 2064 6566 2072    '''..    def r
 00091bd0: 6570 6f72 7428 7365 6c66 2c20 7479 7065  eport(self, type
 00091be0: 3a20 7479 7069 6e67 2e55 6e69 6f6e 5b74  : typing.Union[t
-00091bf0: 7970 696e 672e 5365 745b 7374 725d 2c20  yping.Set[str], 
-00091c00: 7479 7069 6e67 2e53 6574 5b69 6e74 5d5d  typing.Set[int]]
+00091bf0: 7970 696e 672e 5365 745b 696e 745d 2c20  yping.Set[int], 
+00091c00: 7479 7069 6e67 2e53 6574 5b73 7472 5d5d  typing.Set[str]]
 00091c10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
 00091c20: 206d 6573 7361 6765 3a20 7479 7069 6e67   message: typing
 00091c30: 2e55 6e69 6f6e 5b73 7472 2c20 7479 7069  .Union[str, typi
 00091c40: 6e67 2e41 6e79 5d29 3a0a 2020 2020 2020  ng.Any]):.      
 00091c50: 2020 2727 2720 7265 706f 7274 0a0a 2020    ''' report..  
 00091c60: 2020 2020 2020 3a70 6172 616d 2074 7970        :param typ
 00091c70: 653a 2054 7970 650a 2020 2020 2020 2020  e: Type.        
 00091c80: 3a74 7970 6520 7479 7065 3a20 7479 7069  :type type: typi
 00091c90: 6e67 2e55 6e69 6f6e 5b74 7970 696e 672e  ng.Union[typing.
-00091ca0: 5365 745b 7374 725d 2c20 7479 7069 6e67  Set[str], typing
-00091cb0: 2e53 6574 5b69 6e74 5d5d 0a20 2020 2020  .Set[int]].     
+00091ca0: 5365 745b 696e 745d 2c20 7479 7069 6e67  Set[int], typing
+00091cb0: 2e53 6574 5b73 7472 5d5d 0a20 2020 2020  .Set[str]].     
 00091cc0: 2020 203a 7061 7261 6d20 6d65 7373 6167     :param messag
 00091cd0: 653a 2052 6570 6f72 7420 4d65 7373 6167  e: Report Messag
 00091ce0: 650a 2020 2020 2020 2020 3a74 7970 6520  e.        :type 
 00091cf0: 6d65 7373 6167 653a 2074 7970 696e 672e  message: typing.
 00091d00: 556e 696f 6e5b 7374 722c 2074 7970 696e  Union[str, typin
 00091d10: 672e 416e 795d 0a20 2020 2020 2020 2027  g.Any].        '
 00091d20: 2727 0a20 2020 2020 2020 2070 6173 730a  ''.        pass.
@@ -37350,26 +37350,26 @@
 00091e50: 436f 6e74 6578 7427 0a20 2020 2020 2020  Context'.       
 00091e60: 2027 2727 0a20 2020 2020 2020 2070 6173   '''.        pas
 00091e70: 730a 0a20 2020 2064 6566 2065 7865 6375  s..    def execu
 00091e80: 7465 2873 656c 662c 2063 6f6e 7465 7874  te(self, context
 00091e90: 3a20 2743 6f6e 7465 7874 270a 2020 2020  : 'Context'.    
 00091ea0: 2020 2020 2020 2020 2020 2020 2920 2d3e              ) ->
 00091eb0: 2074 7970 696e 672e 556e 696f 6e5b 7479   typing.Union[ty
-00091ec0: 7069 6e67 2e53 6574 5b73 7472 5d2c 2074  ping.Set[str], t
-00091ed0: 7970 696e 672e 5365 745b 696e 745d 5d3a  yping.Set[int]]:
+00091ec0: 7069 6e67 2e53 6574 5b69 6e74 5d2c 2074  ping.Set[int], t
+00091ed0: 7970 696e 672e 5365 745b 7374 725d 5d3a  yping.Set[str]]:
 00091ee0: 0a20 2020 2020 2020 2027 2727 2045 7865  .        ''' Exe
 00091ef0: 6375 7465 2074 6865 206f 7065 7261 746f  cute the operato
 00091f00: 720a 0a20 2020 2020 2020 203a 7061 7261  r..        :para
 00091f10: 6d20 636f 6e74 6578 743a 200a 2020 2020  m context: .    
 00091f20: 2020 2020 3a74 7970 6520 636f 6e74 6578      :type contex
 00091f30: 743a 2027 436f 6e74 6578 7427 0a20 2020  t: 'Context'.   
 00091f40: 2020 2020 203a 7274 7970 653a 2074 7970       :rtype: typ
 00091f50: 696e 672e 556e 696f 6e5b 7479 7069 6e67  ing.Union[typing
-00091f60: 2e53 6574 5b73 7472 5d2c 2074 7970 696e  .Set[str], typin
-00091f70: 672e 5365 745b 696e 745d 5d0a 2020 2020  g.Set[int]].    
+00091f60: 2e53 6574 5b69 6e74 5d2c 2074 7970 696e  .Set[int], typin
+00091f70: 672e 5365 745b 7374 725d 5d0a 2020 2020  g.Set[str]].    
 00091f80: 2020 2020 3a72 6574 7572 6e3a 2072 6573      :return: res
 00091f90: 756c 740a 2020 2020 2020 2020 2727 270a  ult.        '''.
 00091fa0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
 00091fb0: 2020 6465 6620 6368 6563 6b28 7365 6c66    def check(self
 00091fc0: 2c20 636f 6e74 6578 743a 2027 436f 6e74  , context: 'Cont
 00091fd0: 6578 7427 2920 2d3e 2062 6f6f 6c3a 0a20  ext') -> bool:. 
 00091fe0: 2020 2020 2020 2027 2727 2043 6865 636b         ''' Check
@@ -37387,53 +37387,53 @@
 000920a0: 2027 2727 0a20 2020 2020 2020 2070 6173   '''.        pas
 000920b0: 730a 0a20 2020 2064 6566 2069 6e76 6f6b  s..    def invok
 000920c0: 6528 7365 6c66 2c20 636f 6e74 6578 743a  e(self, context:
 000920d0: 2027 436f 6e74 6578 7427 2c20 6576 656e   'Context', even
 000920e0: 743a 2027 4576 656e 7427 0a20 2020 2020  t: 'Event'.     
 000920f0: 2020 2020 2020 2020 2020 2920 2d3e 2074            ) -> t
 00092100: 7970 696e 672e 556e 696f 6e5b 7479 7069  yping.Union[typi
-00092110: 6e67 2e53 6574 5b73 7472 5d2c 2074 7970  ng.Set[str], typ
-00092120: 696e 672e 5365 745b 696e 745d 5d3a 0a20  ing.Set[int]]:. 
+00092110: 6e67 2e53 6574 5b69 6e74 5d2c 2074 7970  ng.Set[int], typ
+00092120: 696e 672e 5365 745b 7374 725d 5d3a 0a20  ing.Set[str]]:. 
 00092130: 2020 2020 2020 2027 2727 2049 6e76 6f6b         ''' Invok
 00092140: 6520 7468 6520 6f70 6572 6174 6f72 0a0a  e the operator..
 00092150: 2020 2020 2020 2020 3a70 6172 616d 2063          :param c
 00092160: 6f6e 7465 7874 3a20 0a20 2020 2020 2020  ontext: .       
 00092170: 203a 7479 7065 2063 6f6e 7465 7874 3a20   :type context: 
 00092180: 2743 6f6e 7465 7874 270a 2020 2020 2020  'Context'.      
 00092190: 2020 3a70 6172 616d 2065 7665 6e74 3a20    :param event: 
 000921a0: 0a20 2020 2020 2020 203a 7479 7065 2065  .        :type e
 000921b0: 7665 6e74 3a20 2745 7665 6e74 270a 2020  vent: 'Event'.  
 000921c0: 2020 2020 2020 3a72 7479 7065 3a20 7479        :rtype: ty
 000921d0: 7069 6e67 2e55 6e69 6f6e 5b74 7970 696e  ping.Union[typin
-000921e0: 672e 5365 745b 7374 725d 2c20 7479 7069  g.Set[str], typi
-000921f0: 6e67 2e53 6574 5b69 6e74 5d5d 0a20 2020  ng.Set[int]].   
+000921e0: 672e 5365 745b 696e 745d 2c20 7479 7069  g.Set[int], typi
+000921f0: 6e67 2e53 6574 5b73 7472 5d5d 0a20 2020  ng.Set[str]].   
 00092200: 2020 2020 203a 7265 7475 726e 3a20 7265       :return: re
 00092210: 7375 6c74 0a20 2020 2020 2020 2027 2727  sult.        '''
 00092220: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
 00092230: 2020 2064 6566 206d 6f64 616c 2873 656c     def modal(sel
 00092240: 662c 2063 6f6e 7465 7874 3a20 2743 6f6e  f, context: 'Con
 00092250: 7465 7874 272c 2065 7665 6e74 3a20 2745  text', event: 'E
 00092260: 7665 6e74 270a 2020 2020 2020 2020 2020  vent'.          
 00092270: 2020 2020 2920 2d3e 2074 7970 696e 672e      ) -> typing.
 00092280: 556e 696f 6e5b 7479 7069 6e67 2e53 6574  Union[typing.Set
-00092290: 5b73 7472 5d2c 2074 7970 696e 672e 5365  [str], typing.Se
-000922a0: 745b 696e 745d 5d3a 0a20 2020 2020 2020  t[int]]:.       
+00092290: 5b69 6e74 5d2c 2074 7970 696e 672e 5365  [int], typing.Se
+000922a0: 745b 7374 725d 5d3a 0a20 2020 2020 2020  t[str]]:.       
 000922b0: 2027 2727 204d 6f64 616c 206f 7065 7261   ''' Modal opera
 000922c0: 746f 7220 6675 6e63 7469 6f6e 0a0a 2020  tor function..  
 000922d0: 2020 2020 2020 3a70 6172 616d 2063 6f6e        :param con
 000922e0: 7465 7874 3a20 0a20 2020 2020 2020 203a  text: .        :
 000922f0: 7479 7065 2063 6f6e 7465 7874 3a20 2743  type context: 'C
 00092300: 6f6e 7465 7874 270a 2020 2020 2020 2020  ontext'.        
 00092310: 3a70 6172 616d 2065 7665 6e74 3a20 0a20  :param event: . 
 00092320: 2020 2020 2020 203a 7479 7065 2065 7665         :type eve
 00092330: 6e74 3a20 2745 7665 6e74 270a 2020 2020  nt: 'Event'.    
 00092340: 2020 2020 3a72 7479 7065 3a20 7479 7069      :rtype: typi
 00092350: 6e67 2e55 6e69 6f6e 5b74 7970 696e 672e  ng.Union[typing.
-00092360: 5365 745b 7374 725d 2c20 7479 7069 6e67  Set[str], typing
-00092370: 2e53 6574 5b69 6e74 5d5d 0a20 2020 2020  .Set[int]].     
+00092360: 5365 745b 696e 745d 2c20 7479 7069 6e67  Set[int], typing
+00092370: 2e53 6574 5b73 7472 5d5d 0a20 2020 2020  .Set[str]].     
 00092380: 2020 203a 7265 7475 726e 3a20 7265 7375     :return: resu
 00092390: 6c74 0a20 2020 2020 2020 2027 2727 0a20  lt.        '''. 
 000923a0: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
 000923b0: 2064 6566 2064 7261 7728 7365 6c66 2c20   def draw(self, 
 000923c0: 636f 6e74 6578 743a 2027 436f 6e74 6578  context: 'Contex
 000923d0: 7427 293a 0a20 2020 2020 2020 2027 2727  t'):.        '''
 000923e0: 2044 7261 7720 6675 6e63 7469 6f6e 2066   Draw function f
@@ -47082,29 +47082,29 @@
 000b7e90: 2020 203a 7479 7065 206d 656d 6f72 795f     :type memory_
 000b7ea0: 7065 616b 3a20 7479 7069 6e67 2e4f 7074  peak: typing.Opt
 000b7eb0: 696f 6e61 6c5b 7479 7069 6e67 2e41 6e79  ional[typing.Any
 000b7ec0: 5d0a 2020 2020 2020 2020 2727 270a 2020  ].        '''.  
 000b7ed0: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
 000b7ee0: 6465 6620 7265 706f 7274 2873 656c 662c  def report(self,
 000b7ef0: 2074 7970 653a 2074 7970 696e 672e 556e   type: typing.Un
-000b7f00: 696f 6e5b 7479 7069 6e67 2e53 6574 5b73  ion[typing.Set[s
-000b7f10: 7472 5d2c 2074 7970 696e 672e 5365 745b  tr], typing.Set[
-000b7f20: 696e 745d 5d2c 0a20 2020 2020 2020 2020  int]],.         
+000b7f00: 696f 6e5b 7479 7069 6e67 2e53 6574 5b69  ion[typing.Set[i
+000b7f10: 6e74 5d2c 2074 7970 696e 672e 5365 745b  nt], typing.Set[
+000b7f20: 7374 725d 5d2c 0a20 2020 2020 2020 2020  str]],.         
 000b7f30: 2020 2020 2020 6d65 7373 6167 653a 2074        message: t
 000b7f40: 7970 696e 672e 556e 696f 6e5b 7374 722c  yping.Union[str,
 000b7f50: 2074 7970 696e 672e 416e 795d 293a 0a20   typing.Any]):. 
 000b7f60: 2020 2020 2020 2027 2727 2052 6570 6f72         ''' Repor
 000b7f70: 7420 696e 666f 2c20 7761 726e 696e 6720  t info, warning 
 000b7f80: 6f72 2065 7272 6f72 206d 6573 7361 6765  or error message
 000b7f90: 730a 0a20 2020 2020 2020 203a 7061 7261  s..        :para
 000b7fa0: 6d20 7479 7065 3a20 5479 7065 0a20 2020  m type: Type.   
 000b7fb0: 2020 2020 203a 7479 7065 2074 7970 653a       :type type:
 000b7fc0: 2074 7970 696e 672e 556e 696f 6e5b 7479   typing.Union[ty
-000b7fd0: 7069 6e67 2e53 6574 5b73 7472 5d2c 2074  ping.Set[str], t
-000b7fe0: 7970 696e 672e 5365 745b 696e 745d 5d0a  yping.Set[int]].
+000b7fd0: 7069 6e67 2e53 6574 5b69 6e74 5d2c 2074  ping.Set[int], t
+000b7fe0: 7970 696e 672e 5365 745b 7374 725d 5d0a  yping.Set[str]].
 000b7ff0: 2020 2020 2020 2020 3a70 6172 616d 206d          :param m
 000b8000: 6573 7361 6765 3a20 5265 706f 7274 204d  essage: Report M
 000b8010: 6573 7361 6765 0a20 2020 2020 2020 203a  essage.        :
 000b8020: 7479 7065 206d 6573 7361 6765 3a20 7479  type message: ty
 000b8030: 7069 6e67 2e55 6e69 6f6e 5b73 7472 2c20  ping.Union[str, 
 000b8040: 7479 7069 6e67 2e41 6e79 5d0a 2020 2020  typing.Any].    
 000b8050: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
@@ -66601,23 +66601,23 @@
 00104280: 2066 6163 6573 2077 6974 6820 7468 6520   faces with the 
 00104290: 6375 7272 656e 746c 7920 6469 7370 6c61  currently displa
 001042a0: 7965 6420 696d 6167 6520 6173 7369 676e  yed image assign
 001042b0: 6564 0a0a 2020 2020 3a74 7970 653a 2062  ed..    :type: b
 001042c0: 6f6f 6c0a 2020 2020 2727 270a 0a20 2020  ool.    '''..   
 001042d0: 2073 6e61 705f 656c 656d 656e 7473 3a20   snap_elements: 
 001042e0: 7479 7069 6e67 2e55 6e69 6f6e 5b74 7970  typing.Union[typ
-001042f0: 696e 672e 5365 745b 7374 725d 2c20 7479  ing.Set[str], ty
-00104300: 7069 6e67 2e53 6574 5b69 6e74 5d5d 203d  ping.Set[int]] =
+001042f0: 696e 672e 5365 745b 696e 745d 2c20 7479  ing.Set[int], ty
+00104300: 7069 6e67 2e53 6574 5b73 7472 5d5d 203d  ping.Set[str]] =
 00104310: 204e 6f6e 650a 2020 2020 2727 2720 5479   None.    ''' Ty
 00104320: 7065 206f 6620 656c 656d 656e 7420 746f  pe of element to
 00104330: 2073 6e61 7020 746f 0a0a 2020 2020 3a74   snap to..    :t
 00104340: 7970 653a 2074 7970 696e 672e 556e 696f  ype: typing.Unio
-00104350: 6e5b 7479 7069 6e67 2e53 6574 5b73 7472  n[typing.Set[str
-00104360: 5d2c 2074 7970 696e 672e 5365 745b 696e  ], typing.Set[in
-00104370: 745d 5d0a 2020 2020 2727 270a 0a20 2020  t]].    '''..   
+00104350: 6e5b 7479 7069 6e67 2e53 6574 5b69 6e74  n[typing.Set[int
+00104360: 5d2c 2074 7970 696e 672e 5365 745b 7374  ], typing.Set[st
+00104370: 725d 5d0a 2020 2020 2727 270a 0a20 2020  r]].    '''..   
 00104380: 2073 6e61 705f 6661 6365 5f6e 6561 7265   snap_face_neare
 00104390: 7374 5f73 7465 7073 3a20 696e 7420 3d20  st_steps: int = 
 001043a0: 4e6f 6e65 0a20 2020 2027 2727 204e 756d  None.    ''' Num
 001043b0: 6265 7220 6f66 2073 7465 7073 2074 6f20  ber of steps to 
 001043c0: 6272 6561 6b20 7472 616e 7366 6f72 6d61  break transforma
 001043d0: 7469 6f6e 2069 6e74 6f20 666f 7220 6661  tion into for fa
 001043e0: 6365 206e 6561 7265 7374 2073 6e61 7070  ce nearest snapp
@@ -108240,16 +108240,16 @@
 001a6cf0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
 001a6d00: 2020 2020 2020 2020 2020 2020 2020 6576                ev
 001a6d10: 656e 743a 2074 7970 696e 672e 4f70 7469  ent: typing.Opti
 001a6d20: 6f6e 616c 5b27 4576 656e 7427 5d0a 2020  onal['Event'].  
 001a6d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 001a6d40: 2020 2020 2020 2020 2029 202d 3e20 7479           ) -> ty
 001a6d50: 7069 6e67 2e55 6e69 6f6e 5b74 7970 696e  ping.Union[typin
-001a6d60: 672e 5365 745b 7374 725d 2c20 7479 7069  g.Set[str], typi
-001a6d70: 6e67 2e53 6574 5b69 6e74 5d5d 3a0a 2020  ng.Set[int]]:.  
+001a6d60: 672e 5365 745b 696e 745d 2c20 7479 7069  g.Set[int], typi
+001a6d70: 6e67 2e53 6574 5b73 7472 5d5d 3a0a 2020  ng.Set[str]]:.  
 001a6d80: 2020 2020 2020 2727 2720 4f70 6572 6174        ''' Operat
 001a6d90: 6f72 2070 6f70 7570 2069 6e76 6f6b 6520  or popup invoke 
 001a6da0: 2873 686f 7720 6f70 6572 6174 6f72 2070  (show operator p
 001a6db0: 726f 7065 7274 6965 7320 616e 6420 6578  roperties and ex
 001a6dc0: 6563 7574 6520 6974 2061 7574 6f6d 6174  ecute it automat
 001a6dd0: 6963 616c 6c79 206f 6e20 6368 616e 6765  ically on change
 001a6de0: 7329 0a0a 2020 2020 2020 2020 3a70 6172  s)..        :par
@@ -108261,16 +108261,16 @@
 001a6e40: 5d0a 2020 2020 2020 2020 3a70 6172 616d  ].        :param
 001a6e50: 2065 7665 6e74 3a20 4576 656e 740a 2020   event: Event.  
 001a6e60: 2020 2020 2020 3a74 7970 6520 6576 656e        :type even
 001a6e70: 743a 2074 7970 696e 672e 4f70 7469 6f6e  t: typing.Option
 001a6e80: 616c 5b27 4576 656e 7427 5d0a 2020 2020  al['Event'].    
 001a6e90: 2020 2020 3a72 7479 7065 3a20 7479 7069      :rtype: typi
 001a6ea0: 6e67 2e55 6e69 6f6e 5b74 7970 696e 672e  ng.Union[typing.
-001a6eb0: 5365 745b 7374 725d 2c20 7479 7069 6e67  Set[str], typing
-001a6ec0: 2e53 6574 5b69 6e74 5d5d 0a20 2020 2020  .Set[int]].     
+001a6eb0: 5365 745b 696e 745d 2c20 7479 7069 6e67  Set[int], typing
+001a6ec0: 2e53 6574 5b73 7472 5d5d 0a20 2020 2020  .Set[str]].     
 001a6ed0: 2020 203a 7265 7475 726e 3a20 7265 7375     :return: resu
 001a6ee0: 6c74 0a20 2020 2020 2020 2027 2727 0a20  lt.        '''. 
 001a6ef0: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
 001a6f00: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
 001a6f10: 2020 6465 6620 696e 766f 6b65 5f70 726f    def invoke_pro
 001a6f20: 7073 5f64 6961 6c6f 6728 0a20 2020 2020  ps_dialog(.     
 001a6f30: 2020 2020 2020 2063 6c73 2c0a 2020 2020         cls,.    
@@ -108278,16 +108278,16 @@
 001a6f50: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
 001a6f60: 6c5b 274f 7065 7261 746f 7227 5d2c 0a20  l['Operator'],. 
 001a6f70: 2020 2020 2020 2020 2020 2077 6964 7468             width
 001a6f80: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
 001a6f90: 6c5b 7479 7069 6e67 2e41 6e79 5d20 3d20  l[typing.Any] = 
 001a6fa0: 3330 300a 2020 2020 2920 2d3e 2074 7970  300.    ) -> typ
 001a6fb0: 696e 672e 556e 696f 6e5b 7479 7069 6e67  ing.Union[typing
-001a6fc0: 2e53 6574 5b73 7472 5d2c 2074 7970 696e  .Set[str], typin
-001a6fd0: 672e 5365 745b 696e 745d 5d3a 0a20 2020  g.Set[int]]:.   
+001a6fc0: 2e53 6574 5b69 6e74 5d2c 2074 7970 696e  .Set[int], typin
+001a6fd0: 672e 5365 745b 7374 725d 5d3a 0a20 2020  g.Set[str]]:.   
 001a6fe0: 2020 2020 2027 2727 204f 7065 7261 746f       ''' Operato
 001a6ff0: 7220 6469 616c 6f67 2028 6e6f 6e2d 6175  r dialog (non-au
 001a7000: 746f 6578 6563 2070 6f70 7570 2920 696e  toexec popup) in
 001a7010: 766f 6b65 2028 7368 6f77 206f 7065 7261  voke (show opera
 001a7020: 746f 7220 7072 6f70 6572 7469 6573 2061  tor properties a
 001a7030: 6e64 206f 6e6c 7920 6578 6563 7574 6520  nd only execute 
 001a7040: 6974 206f 6e20 636c 6963 6b20 6f6e 204f  it on click on O
@@ -108301,16 +108301,16 @@
 001a70c0: 203a 7061 7261 6d20 7769 6474 683a 2057   :param width: W
 001a70d0: 6964 7468 206f 6620 7468 6520 706f 7075  idth of the popu
 001a70e0: 700a 2020 2020 2020 2020 3a74 7970 6520  p.        :type 
 001a70f0: 7769 6474 683a 2074 7970 696e 672e 4f70  width: typing.Op
 001a7100: 7469 6f6e 616c 5b74 7970 696e 672e 416e  tional[typing.An
 001a7110: 795d 0a20 2020 2020 2020 203a 7274 7970  y].        :rtyp
 001a7120: 653a 2074 7970 696e 672e 556e 696f 6e5b  e: typing.Union[
-001a7130: 7479 7069 6e67 2e53 6574 5b73 7472 5d2c  typing.Set[str],
-001a7140: 2074 7970 696e 672e 5365 745b 696e 745d   typing.Set[int]
+001a7130: 7479 7069 6e67 2e53 6574 5b69 6e74 5d2c  typing.Set[int],
+001a7140: 2074 7970 696e 672e 5365 745b 7374 725d   typing.Set[str]
 001a7150: 5d0a 2020 2020 2020 2020 3a72 6574 7572  ].        :retur
 001a7160: 6e3a 2072 6573 756c 740a 2020 2020 2020  n: result.      
 001a7170: 2020 2727 270a 2020 2020 2020 2020 7061    '''.        pa
 001a7180: 7373 0a0a 2020 2020 4063 6c61 7373 6d65  ss..    @classme
 001a7190: 7468 6f64 0a20 2020 2064 6566 2069 6e76  thod.    def inv
 001a71a0: 6f6b 655f 7365 6172 6368 5f70 6f70 7570  oke_search_popup
 001a71b0: 2863 6c73 2c20 6f70 6572 6174 6f72 3a20  (cls, operator: 
@@ -108343,17 +108343,17 @@
 001a7360: 5b27 4f70 6572 6174 6f72 275d 2c0a 2020  ['Operator'],.  
 001a7370: 2020 2020 2020 2020 2020 2020 2020 2020                  
 001a7380: 2020 2077 6964 7468 3a20 7479 7069 6e67     width: typing
 001a7390: 2e4f 7074 696f 6e61 6c5b 7479 7069 6e67  .Optional[typing
 001a73a0: 2e41 6e79 5d20 3d20 3330 300a 2020 2020  .Any] = 300.    
 001a73b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 001a73c0: 2029 202d 3e20 7479 7069 6e67 2e55 6e69   ) -> typing.Uni
-001a73d0: 6f6e 5b74 7970 696e 672e 5365 745b 7374  on[typing.Set[st
-001a73e0: 725d 2c20 7479 7069 6e67 2e53 6574 5b69  r], typing.Set[i
-001a73f0: 6e74 5d5d 3a0a 2020 2020 2020 2020 2727  nt]]:.        ''
+001a73d0: 6f6e 5b74 7970 696e 672e 5365 745b 696e  on[typing.Set[in
+001a73e0: 745d 2c20 7479 7069 6e67 2e53 6574 5b73  t], typing.Set[s
+001a73f0: 7472 5d5d 3a0a 2020 2020 2020 2020 2727  tr]]:.        ''
 001a7400: 2720 4f70 6572 6174 6f72 2070 6f70 7570  ' Operator popup
 001a7410: 2069 6e76 6f6b 6520 286f 6e6c 7920 7368   invoke (only sh
 001a7420: 6f77 7320 6f70 6572 6174 6f72 2773 2070  ows operator's p
 001a7430: 726f 7065 7274 6965 732c 2077 6974 686f  roperties, witho
 001a7440: 7574 2065 7865 6375 7469 6e67 2069 7429  ut executing it)
 001a7450: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
 001a7460: 206f 7065 7261 746f 723a 204f 7065 7261   operator: Opera
@@ -108365,32 +108365,32 @@
 001a74c0: 6964 7468 3a20 5769 6474 6820 6f66 2074  idth: Width of t
 001a74d0: 6865 2070 6f70 7570 0a20 2020 2020 2020  he popup.       
 001a74e0: 203a 7479 7065 2077 6964 7468 3a20 7479   :type width: ty
 001a74f0: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7479  ping.Optional[ty
 001a7500: 7069 6e67 2e41 6e79 5d0a 2020 2020 2020  ping.Any].      
 001a7510: 2020 3a72 7479 7065 3a20 7479 7069 6e67    :rtype: typing
 001a7520: 2e55 6e69 6f6e 5b74 7970 696e 672e 5365  .Union[typing.Se
-001a7530: 745b 7374 725d 2c20 7479 7069 6e67 2e53  t[str], typing.S
-001a7540: 6574 5b69 6e74 5d5d 0a20 2020 2020 2020  et[int]].       
+001a7530: 745b 696e 745d 2c20 7479 7069 6e67 2e53  t[int], typing.S
+001a7540: 6574 5b73 7472 5d5d 0a20 2020 2020 2020  et[str]].       
 001a7550: 203a 7265 7475 726e 3a20 7265 7375 6c74   :return: result
 001a7560: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
 001a7570: 2020 2020 2070 6173 730a 0a20 2020 2040       pass..    @
 001a7580: 636c 6173 736d 6574 686f 640a 2020 2020  classmethod.    
 001a7590: 6465 6620 696e 766f 6b65 5f63 6f6e 6669  def invoke_confi
 001a75a0: 726d 2863 6c73 2c20 6f70 6572 6174 6f72  rm(cls, operator
 001a75b0: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
 001a75c0: 6c5b 274f 7065 7261 746f 7227 5d2c 0a20  l['Operator'],. 
 001a75d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 001a75e0: 2020 2020 2020 6576 656e 743a 2074 7970        event: typ
 001a75f0: 696e 672e 4f70 7469 6f6e 616c 5b27 4576  ing.Optional['Ev
 001a7600: 656e 7427 5d0a 2020 2020 2020 2020 2020  ent'].          
 001a7610: 2020 2020 2020 2020 2020 2020 2029 202d               ) -
 001a7620: 3e20 7479 7069 6e67 2e55 6e69 6f6e 5b74  > typing.Union[t
-001a7630: 7970 696e 672e 5365 745b 7374 725d 2c20  yping.Set[str], 
-001a7640: 7479 7069 6e67 2e53 6574 5b69 6e74 5d5d  typing.Set[int]]
+001a7630: 7970 696e 672e 5365 745b 696e 745d 2c20  yping.Set[int], 
+001a7640: 7479 7069 6e67 2e53 6574 5b73 7472 5d5d  typing.Set[str]]
 001a7650: 3a0a 2020 2020 2020 2020 2727 2720 4f70  :.        ''' Op
 001a7660: 6572 6174 6f72 2063 6f6e 6669 726d 6174  erator confirmat
 001a7670: 696f 6e20 706f 7075 7020 286f 6e6c 7920  ion popup (only 
 001a7680: 746f 206c 6574 2075 7365 7220 636f 6e66  to let user conf
 001a7690: 6972 6d20 7468 6520 6578 6563 7574 696f  irm the executio
 001a76a0: 6e2c 206e 6f20 6f70 6572 6174 6f72 2070  n, no operator p
 001a76b0: 726f 7065 7274 6965 7320 7368 6f77 6e29  roperties shown)
@@ -108403,16 +108403,16 @@
 001a7720: 2020 2020 2020 2020 3a70 6172 616d 2065          :param e
 001a7730: 7665 6e74 3a20 4576 656e 740a 2020 2020  vent: Event.    
 001a7740: 2020 2020 3a74 7970 6520 6576 656e 743a      :type event:
 001a7750: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
 001a7760: 5b27 4576 656e 7427 5d0a 2020 2020 2020  ['Event'].      
 001a7770: 2020 3a72 7479 7065 3a20 7479 7069 6e67    :rtype: typing
 001a7780: 2e55 6e69 6f6e 5b74 7970 696e 672e 5365  .Union[typing.Se
-001a7790: 745b 7374 725d 2c20 7479 7069 6e67 2e53  t[str], typing.S
-001a77a0: 6574 5b69 6e74 5d5d 0a20 2020 2020 2020  et[int]].       
+001a7790: 745b 696e 745d 2c20 7479 7069 6e67 2e53  t[int], typing.S
+001a77a0: 6574 5b73 7472 5d5d 0a20 2020 2020 2020  et[str]].       
 001a77b0: 203a 7265 7475 726e 3a20 7265 7375 6c74   :return: result
 001a77c0: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
 001a77d0: 2020 2020 2070 6173 730a 0a20 2020 2040       pass..    @
 001a77e0: 636c 6173 736d 6574 686f 640a 2020 2020  classmethod.    
 001a77f0: 6465 6620 706f 706d 656e 755f 6265 6769  def popmenu_begi
 001a7800: 6e5f 5f69 6e74 6572 6e61 6c28 636c 732c  n__internal(cls,
 001a7810: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
@@ -114395,22 +114395,22 @@
 001beda0: 6d65 7472 7920 746f 2066 6f72 6d20 706c  metry to form pl
 001bedb0: 616e 6172 2070 6f6c 7967 6f6e 732e 0a0a  anar polygons...
 001bedc0: 2020 2020 3a74 7970 653a 2074 7970 696e      :type: typin
 001bedd0: 672e 556e 696f 6e5b 7374 722c 2069 6e74  g.Union[str, int
 001bede0: 5d0a 2020 2020 2727 270a 0a20 2020 2064  ].    '''..    d
 001bedf0: 656c 696d 6974 3a20 7479 7069 6e67 2e55  elimit: typing.U
 001bee00: 6e69 6f6e 5b74 7970 696e 672e 5365 745b  nion[typing.Set[
-001bee10: 7374 725d 2c20 7479 7069 6e67 2e53 6574  str], typing.Set
-001bee20: 5b69 6e74 5d5d 203d 204e 6f6e 650a 2020  [int]] = None.  
+001bee10: 696e 745d 2c20 7479 7069 6e67 2e53 6574  int], typing.Set
+001bee20: 5b73 7472 5d5d 203d 204e 6f6e 650a 2020  [str]] = None.  
 001bee30: 2020 2727 2720 4c69 6d69 7420 6d65 7267    ''' Limit merg
 001bee40: 696e 6720 6765 6f6d 6574 7279 0a0a 2020  ing geometry..  
 001bee50: 2020 3a74 7970 653a 2074 7970 696e 672e    :type: typing.
 001bee60: 556e 696f 6e5b 7479 7069 6e67 2e53 6574  Union[typing.Set
-001bee70: 5b73 7472 5d2c 2074 7970 696e 672e 5365  [str], typing.Se
-001bee80: 745b 696e 745d 5d0a 2020 2020 2727 270a  t[int]].    '''.
+001bee70: 5b69 6e74 5d2c 2074 7970 696e 672e 5365  [int], typing.Se
+001bee80: 745b 7374 725d 5d0a 2020 2020 2727 270a  t[str]].    '''.
 001bee90: 0a20 2020 2066 6163 655f 636f 756e 743a  .    face_count:
 001beea0: 2069 6e74 203d 204e 6f6e 650a 2020 2020   int = None.    
 001beeb0: 2727 2720 5468 6520 6375 7272 656e 7420  ''' The current 
 001beec0: 6e75 6d62 6572 206f 6620 6661 6365 7320  number of faces 
 001beed0: 696e 2074 6865 2064 6563 696d 6174 6564  in the decimated
 001beee0: 206d 6573 680a 0a20 2020 203a 7479 7065   mesh..    :type
 001beef0: 3a20 696e 740a 2020 2020 2727 270a 0a20  : int.    '''.. 
@@ -115678,21 +115678,21 @@
 001c3dd0: 5061 7468 2074 6f20 6578 7465 726e 616c  Path to external
 001c3de0: 2064 6973 706c 6163 656d 656e 7473 2066   displacements f
 001c3df0: 696c 650a 0a20 2020 203a 7479 7065 3a20  ile..    :type: 
 001c3e00: 7479 7069 6e67 2e55 6e69 6f6e 5b73 7472  typing.Union[str
 001c3e10: 2c20 7479 7069 6e67 2e41 6e79 5d0a 2020  , typing.Any].  
 001c3e20: 2020 2727 270a 0a20 2020 2066 6c69 705f    '''..    flip_
 001c3e30: 6178 6973 3a20 7479 7069 6e67 2e55 6e69  axis: typing.Uni
-001c3e40: 6f6e 5b74 7970 696e 672e 5365 745b 7374  on[typing.Set[st
-001c3e50: 725d 2c20 7479 7069 6e67 2e53 6574 5b69  r], typing.Set[i
-001c3e60: 6e74 5d5d 203d 204e 6f6e 650a 2020 2020  nt]] = None.    
+001c3e40: 6f6e 5b74 7970 696e 672e 5365 745b 696e  on[typing.Set[in
+001c3e50: 745d 2c20 7479 7069 6e67 2e53 6574 5b73  t], typing.Set[s
+001c3e60: 7472 5d5d 203d 204e 6f6e 650a 2020 2020  tr]] = None.    
 001c3e70: 2727 2720 0a0a 2020 2020 3a74 7970 653a  ''' ..    :type:
 001c3e80: 2074 7970 696e 672e 556e 696f 6e5b 7479   typing.Union[ty
-001c3e90: 7069 6e67 2e53 6574 5b73 7472 5d2c 2074  ping.Set[str], t
-001c3ea0: 7970 696e 672e 5365 745b 696e 745d 5d0a  yping.Set[int]].
+001c3e90: 7069 6e67 2e53 6574 5b69 6e74 5d2c 2074  ping.Set[int], t
+001c3ea0: 7970 696e 672e 5365 745b 7374 725d 5d0a  yping.Set[str]].
 001c3eb0: 2020 2020 2727 270a 0a20 2020 2066 6f72      '''..    for
 001c3ec0: 7761 7264 5f61 7869 733a 2074 7970 696e  ward_axis: typin
 001c3ed0: 672e 556e 696f 6e5b 7374 722c 2069 6e74  g.Union[str, int
 001c3ee0: 5d20 3d20 4e6f 6e65 0a20 2020 2027 2727  ] = None.    '''
 001c3ef0: 200a 0a20 2020 203a 7479 7065 3a20 7479   ..    :type: ty
 001c3f00: 7069 6e67 2e55 6e69 6f6e 5b73 7472 2c20  ping.Union[str, 
 001c3f10: 696e 745d 0a20 2020 2027 2727 0a0a 2020  int].    '''..
```

### Comparing `fake-bpy-module-latest-20230430/bpy/utils/__init__.py` & `fake-bpy-module-latest-20230501/bpy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/utils/previews.py` & `fake-bpy-module-latest-20230501/bpy/utils/previews.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy/utils/units.py` & `fake-bpy-module-latest-20230501/bpy/utils/units.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy_extras/anim_utils.py` & `fake-bpy-module-latest-20230501/bpy_extras/anim_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,16 +108,16 @@
     '''
 
     pass
 
 
 def bake_action_objects_iter(
         object_action_pairs: typing.
-        Union['bpy.types.Sequence', 'bpy.types.Action', 'bpy.types.Object'],
+        Union['bpy.types.Action', 'bpy.types.Object', 'bpy.types.Sequence'],
         **kwargs):
     ''' An coroutine that bakes actions for multiple objects.
 
     :param object_action_pairs: Sequence of object action tuples, action is the destination for the baked data. When None a new action will be created.
-    :type object_action_pairs: typing.Union['bpy.types.Sequence', 'bpy.types.Action', 'bpy.types.Object']
+    :type object_action_pairs: typing.Union['bpy.types.Action', 'bpy.types.Object', 'bpy.types.Sequence']
     '''
 
     pass
```

### Comparing `fake-bpy-module-latest-20230430/bpy_extras/image_utils.py` & `fake-bpy-module-latest-20230501/bpy_extras/image_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy_extras/io_utils.py` & `fake-bpy-module-latest-20230501/bpy_extras/io_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy_extras/mesh_utils.py` & `fake-bpy-module-latest-20230501/bpy_extras/mesh_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy_extras/node_shader_utils.py` & `fake-bpy-module-latest-20230501/bpy_extras/node_shader_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy_extras/object_utils.py` & `fake-bpy-module-latest-20230501/bpy_extras/object_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy_extras/view3d_utils.py` & `fake-bpy-module-latest-20230501/bpy_extras/view3d_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy_extras/wm_utils/progress_report.py` & `fake-bpy-module-latest-20230501/bpy_extras/wm_utils/progress_report.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/bpy_types.py` & `fake-bpy-module-latest-20230501/bpy_types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/fake_bpy_module_latest.egg-info/PKG-INFO` & `fake-bpy-module-latest-20230501/fake_bpy_module_latest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: fake-bpy-module-latest
-Version: 20230430
+Version: 20230501
 Summary: Collection of the fake Blender Python API module for the code completion.
 Home-page: https://github.com/nutti/fake-bpy-module
 Author: nutti
 Author-email: nutti.metro@gmail.com
 Maintainer: nutti
 Maintainer-email: nutti.metro@gmail.com
 License: MIT
```

### Comparing `fake-bpy-module-latest-20230430/fake_bpy_module_latest.egg-info/SOURCES.txt` & `fake-bpy-module-latest-20230501/fake_bpy_module_latest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/freestyle/chainingiterators.py` & `fake-bpy-module-latest-20230501/freestyle/chainingiterators.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/freestyle/functions.py` & `fake-bpy-module-latest-20230501/freestyle/functions.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/freestyle/predicates.py` & `fake-bpy-module-latest-20230501/freestyle/predicates.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/freestyle/shaders.py` & `fake-bpy-module-latest-20230501/freestyle/shaders.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/freestyle/types.py` & `fake-bpy-module-latest-20230501/freestyle/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/freestyle/utils/ContextFunctions.py` & `fake-bpy-module-latest-20230501/freestyle/utils/ContextFunctions.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/freestyle/utils/__init__.py` & `fake-bpy-module-latest-20230501/freestyle/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/gpu/capabilities.py` & `fake-bpy-module-latest-20230501/gpu/capabilities.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/gpu/matrix.py` & `fake-bpy-module-latest-20230501/gpu/matrix.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/gpu/platform.py` & `fake-bpy-module-latest-20230501/gpu/platform.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/gpu/shader.py` & `fake-bpy-module-latest-20230501/gpu/shader.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/gpu/state.py` & `fake-bpy-module-latest-20230501/gpu/state.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/gpu/texture.py` & `fake-bpy-module-latest-20230501/gpu/texture.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/gpu/types.py` & `fake-bpy-module-latest-20230501/gpu/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/gpu_extras/batch.py` & `fake-bpy-module-latest-20230501/gpu_extras/batch.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/gpu_extras/presets.py` & `fake-bpy-module-latest-20230501/gpu_extras/presets.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/idprop/types.py` & `fake-bpy-module-latest-20230501/idprop/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/imbuf/__init__.py` & `fake-bpy-module-latest-20230501/imbuf/__init__.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/imbuf/types.py` & `fake-bpy-module-latest-20230501/imbuf/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/keyingsets_builtins.py` & `fake-bpy-module-latest-20230501/keyingsets_builtins.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/keyingsets_utils.py` & `fake-bpy-module-latest-20230501/keyingsets_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/mathutils/__init__.py` & `fake-bpy-module-latest-20230501/mathutils/__init__.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/mathutils/bvhtree.py` & `fake-bpy-module-latest-20230501/mathutils/bvhtree.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/mathutils/geometry.py` & `fake-bpy-module-latest-20230501/mathutils/geometry.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/mathutils/kdtree.py` & `fake-bpy-module-latest-20230501/mathutils/kdtree.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/mathutils/noise.py` & `fake-bpy-module-latest-20230501/mathutils/noise.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/nodeitems_builtins.py` & `fake-bpy-module-latest-20230501/nodeitems_builtins.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/nodeitems_utils.py` & `fake-bpy-module-latest-20230501/nodeitems_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/rna_info.py` & `fake-bpy-module-latest-20230501/rna_info.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/rna_keymap_ui.py` & `fake-bpy-module-latest-20230501/rna_keymap_ui.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/rna_prop_ui.py` & `fake-bpy-module-latest-20230501/rna_prop_ui.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/rna_xml.py` & `fake-bpy-module-latest-20230501/rna_xml.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230430/setup.py` & `fake-bpy-module-latest-20230501/setup.py`

 * *Files identical despite different names*

