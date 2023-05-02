# Comparing `tmp/felupe-7.4.0.tar.gz` & `tmp/felupe-7.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "felupe-7.4.0.tar", last modified: Sat Apr 29 20:25:36 2023, max compression
+gzip compressed data, was "felupe-7.4.1.tar", last modified: Tue May  2 21:52:01 2023, max compression
```

## Comparing `felupe-7.4.0.tar` & `felupe-7.4.1.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:25:36.394801 felupe-7.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35081 2023-04-29 20:25:21.000000 felupe-7.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    50152 2023-04-29 20:25:36.394801 felupe-7.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8369 2023-04-29 20:25:21.000000 felupe-7.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-29 20:25:21.000000 felupe-7.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 20:25:36.394801 felupe-7.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:25:36.382801 felupe-7.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:25:36.382801 felupe-7.4.0/src/felupe/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:25:36.382801 felupe-7.4.0/src/felupe/_assembly/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/_assembly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/_assembly/_axi.py
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/_assembly/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23268 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/_assembly/_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/_assembly/_mixed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:25:36.382801 felupe-7.4.0/src/felupe/_basis/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/_basis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/_basis/_basis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:25:36.386801 felupe-7.4.0/src/felupe/_field/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/_field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/_field/_axi.py
--rw-r--r--   0 runner    (1001) docker     (123)     9409 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/_field/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/_field/_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/_field/_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/_field/_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/_field/_planestrain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:25:36.386801 felupe-7.4.0/src/felupe/constitution/
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/constitution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/constitution/_kinematics.py
--rw-r--r--   0 runner    (1001) docker     (123)    17327 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/constitution/_mixed.py
--rw-r--r--   0 runner    (1001) docker     (123)     9596 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/constitution/_models_hyperelasticity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/constitution/_models_hyperelasticity_ad.py
--rw-r--r--   0 runner    (1001) docker     (123)    17201 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/constitution/_models_linear_elasticity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/constitution/_models_pseudo_elasticity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/constitution/_user_materials.py
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/constitution/_user_materials_hyperelastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/constitution/_user_materials_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:25:36.386801 felupe-7.4.0/src/felupe/dof/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/dof/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/dof/_boundary.py
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/dof/_loadcase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/dof/_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:25:36.386801 felupe-7.4.0/src/felupe/element/
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/element/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/element/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13451 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/element/_hexahedron.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/element/_lagrange.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/element/_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     9632 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/element/_quad.py
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/element/_tetra.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/element/_triangle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:25:36.386801 felupe-7.4.0/src/felupe/math/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/math/_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/math/_math.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/math/_spatial.py
--rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/math/_tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:25:36.390801 felupe-7.4.0/src/felupe/mechanics/
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/mechanics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/mechanics/_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/mechanics/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/mechanics/_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/mechanics/_multipoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/mechanics/_pointload.py
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/mechanics/_solidbody.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/mechanics/_solidbody_gravity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7118 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/mechanics/_solidbody_incompressible.py
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/mechanics/_solidbody_pressure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/mechanics/_step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:25:36.390801 felupe-7.4.0/src/felupe/mesh/
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/mesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/mesh/_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     8857 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/mesh/_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/mesh/_discrete_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/mesh/_dual.py
--rw-r--r--   0 runner    (1001) docker     (123)     7004 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/mesh/_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/mesh/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/mesh/_line_rectangle_cube.py
--rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/mesh/_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/mesh/_read.py
--rw-r--r--   0 runner    (1001) docker     (123)    15579 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/mesh/_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:25:36.390801 felupe-7.4.0/src/felupe/quadrature/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/quadrature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/quadrature/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/quadrature/_gausslegendre.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/quadrature/_tetra.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/quadrature/_triangle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:25:36.390801 felupe-7.4.0/src/felupe/region/
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/region/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12824 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/region/_boundary.py
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/region/_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/region/_templates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:25:36.390801 felupe-7.4.0/src/felupe/solve/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/solve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/solve/_solve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:25:36.394801 felupe-7.4.0/src/felupe/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/tools/_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/tools/_newton.py
--rw-r--r--   0 runner    (1001) docker     (123)    11962 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/tools/_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/tools/_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/tools/_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/tools/_save.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-29 20:25:21.000000 felupe-7.4.0/src/felupe/tools/_solve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:25:36.382801 felupe-7.4.0/src/felupe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    50152 2023-04-29 20:25:36.000000 felupe-7.4.0/src/felupe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-04-29 20:25:36.000000 felupe-7.4.0/src/felupe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 20:25:36.000000 felupe-7.4.0/src/felupe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-29 20:25:36.000000 felupe-7.4.0/src/felupe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-29 20:25:36.000000 felupe-7.4.0/src/felupe.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:25:36.394801 felupe-7.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-04-29 20:25:21.000000 felupe-7.4.0/tests/test_basis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-29 20:25:21.000000 felupe-7.4.0/tests/test_bilinearform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-29 20:25:21.000000 felupe-7.4.0/tests/test_composite.py
--rw-r--r--   0 runner    (1001) docker     (123)    12252 2023-04-29 20:25:21.000000 felupe-7.4.0/tests/test_constitution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-04-29 20:25:21.000000 felupe-7.4.0/tests/test_dof.py
--rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-04-29 20:25:21.000000 felupe-7.4.0/tests/test_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-04-29 20:25:21.000000 felupe-7.4.0/tests/test_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-04-29 20:25:21.000000 felupe-7.4.0/tests/test_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-04-29 20:25:21.000000 felupe-7.4.0/tests/test_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-04-29 20:25:21.000000 felupe-7.4.0/tests/test_math.py
--rw-r--r--   0 runner    (1001) docker     (123)    12303 2023-04-29 20:25:21.000000 felupe-7.4.0/tests/test_mechanics.py
--rw-r--r--   0 runner    (1001) docker     (123)    11591 2023-04-29 20:25:21.000000 felupe-7.4.0/tests/test_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-04-29 20:25:21.000000 felupe-7.4.0/tests/test_mpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-04-29 20:25:21.000000 felupe-7.4.0/tests/test_planestrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-04-29 20:25:21.000000 felupe-7.4.0/tests/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-04-29 20:25:21.000000 felupe-7.4.0/tests/test_quadrature.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-04-29 20:25:21.000000 felupe-7.4.0/tests/test_readme.py
--rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-04-29 20:25:21.000000 felupe-7.4.0/tests/test_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-29 20:25:21.000000 felupe-7.4.0/tests/test_solve.py
--rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-04-29 20:25:21.000000 felupe-7.4.0/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:52:01.849577 felupe-7.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35081 2023-05-02 21:51:49.000000 felupe-7.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    50264 2023-05-02 21:52:01.849577 felupe-7.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-05-02 21:51:49.000000 felupe-7.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-02 21:51:49.000000 felupe-7.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 21:52:01.849577 felupe-7.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:52:01.833577 felupe-7.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:52:01.837577 felupe-7.4.1/src/felupe/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:52:01.837577 felupe-7.4.1/src/felupe/_assembly/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/_assembly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/_assembly/_axi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/_assembly/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23268 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/_assembly/_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/_assembly/_mixed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:52:01.837577 felupe-7.4.1/src/felupe/_basis/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/_basis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/_basis/_basis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:52:01.837577 felupe-7.4.1/src/felupe/_field/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/_field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/_field/_axi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9409 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/_field/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/_field/_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/_field/_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/_field/_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/_field/_planestrain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:52:01.837577 felupe-7.4.1/src/felupe/constitution/
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/constitution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/constitution/_kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17327 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/constitution/_mixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9596 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/constitution/_models_hyperelasticity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/constitution/_models_hyperelasticity_ad.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17201 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/constitution/_models_linear_elasticity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/constitution/_models_pseudo_elasticity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/constitution/_user_materials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/constitution/_user_materials_hyperelastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/constitution/_user_materials_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:52:01.837577 felupe-7.4.1/src/felupe/dof/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/dof/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/dof/_boundary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/dof/_loadcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/dof/_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:52:01.841577 felupe-7.4.1/src/felupe/element/
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/element/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/element/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13451 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/element/_hexahedron.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/element/_lagrange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/element/_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9632 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/element/_quad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/element/_tetra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/element/_triangle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:52:01.841577 felupe-7.4.1/src/felupe/math/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/math/_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/math/_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/math/_spatial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/math/_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:52:01.841577 felupe-7.4.1/src/felupe/mechanics/
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/mechanics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/mechanics/_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/mechanics/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/mechanics/_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/mechanics/_multipoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/mechanics/_pointload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/mechanics/_solidbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/mechanics/_solidbody_gravity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7118 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/mechanics/_solidbody_incompressible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/mechanics/_solidbody_pressure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/mechanics/_step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:52:01.841577 felupe-7.4.1/src/felupe/mesh/
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/mesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/mesh/_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8857 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/mesh/_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/mesh/_discrete_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/mesh/_dual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7004 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/mesh/_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/mesh/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/mesh/_line_rectangle_cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/mesh/_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/mesh/_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15579 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/mesh/_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:52:01.841577 felupe-7.4.1/src/felupe/quadrature/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/quadrature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/quadrature/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/quadrature/_gausslegendre.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/quadrature/_tetra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/quadrature/_triangle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:52:01.845577 felupe-7.4.1/src/felupe/region/
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/region/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12824 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/region/_boundary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/region/_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/region/_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:52:01.845577 felupe-7.4.1/src/felupe/solve/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/solve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/solve/_solve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:52:01.845577 felupe-7.4.1/src/felupe/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/tools/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/tools/_newton.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11962 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/tools/_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/tools/_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/tools/_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/tools/_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/tools/_solve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:52:01.837577 felupe-7.4.1/src/felupe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    50264 2023-05-02 21:52:01.000000 felupe-7.4.1/src/felupe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-05-02 21:52:01.000000 felupe-7.4.1/src/felupe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:52:01.000000 felupe-7.4.1/src/felupe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-02 21:52:01.000000 felupe-7.4.1/src/felupe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-02 21:52:01.000000 felupe-7.4.1/src/felupe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:52:01.845577 felupe-7.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-02 21:51:49.000000 felupe-7.4.1/tests/test_basis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-02 21:51:49.000000 felupe-7.4.1/tests/test_bilinearform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-02 21:51:49.000000 felupe-7.4.1/tests/test_composite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12252 2023-05-02 21:51:49.000000 felupe-7.4.1/tests/test_constitution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-05-02 21:51:49.000000 felupe-7.4.1/tests/test_dof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-05-02 21:51:49.000000 felupe-7.4.1/tests/test_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-05-02 21:51:49.000000 felupe-7.4.1/tests/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-05-02 21:51:49.000000 felupe-7.4.1/tests/test_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-05-02 21:51:49.000000 felupe-7.4.1/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-05-02 21:51:49.000000 felupe-7.4.1/tests/test_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12303 2023-05-02 21:51:49.000000 felupe-7.4.1/tests/test_mechanics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11591 2023-05-02 21:51:49.000000 felupe-7.4.1/tests/test_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-05-02 21:51:49.000000 felupe-7.4.1/tests/test_mpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-05-02 21:51:49.000000 felupe-7.4.1/tests/test_planestrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-05-02 21:51:49.000000 felupe-7.4.1/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-05-02 21:51:49.000000 felupe-7.4.1/tests/test_quadrature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-02 21:51:49.000000 felupe-7.4.1/tests/test_readme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-05-02 21:51:49.000000 felupe-7.4.1/tests/test_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-02 21:51:49.000000 felupe-7.4.1/tests/test_solve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-05-02 21:51:49.000000 felupe-7.4.1/tests/test_tools.py
```

### Comparing `felupe-7.4.0/LICENSE` & `felupe-7.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/PKG-INFO` & `felupe-7.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: felupe
-Version: 7.4.0
+Version: 7.4.1
 Summary: Finite Element Analysis
 Author: Andreas Dutzler
 Author-email: a.dutzler@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -701,22 +701,26 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: all
 License-File: LICENSE
 
 <p align="center">
-  <img src="https://raw.githubusercontent.com/adtzlr/felupe/main/docs/_static/logo_light.svg" height="100px"/> <a href="https://felupe.readthedocs.io/en/latest/examples/rubberspring.html"><img src="https://user-images.githubusercontent.com/5793153/230604246-5a416081-6777-4f33-afdf-efdb51338722.png" height="100px"/></a> <a href="https://felupe.readthedocs.io/en/latest/examples/platewithhole.html"><img src="https://user-images.githubusercontent.com/5793153/230604587-42e3e339-e08c-4cc8-8000-f7046a8d95df.png" height="100px"/></a>
+  <a href="https://felupe.readthedocs.io/en/latest/?badge=latest"><img src="https://user-images.githubusercontent.com/5793153/235789118-eb03eb25-2556-401d-8a0f-580f37e72f8d.png" height="80px"/></a>
   <p align="center">Finite Element Analysis.</p>
 </p>
 
 [![PyPI version shields.io](https://img.shields.io/pypi/v/felupe.svg)](https://pypi.python.org/pypi/felupe/) [![Documentation Status](https://readthedocs.org/projects/felupe/badge/?version=latest)](https://felupe.readthedocs.io/en/latest/?badge=latest) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) ![Made with love in Graz (Austria)](https://img.shields.io/badge/Made%20with%20%E2%9D%A4%EF%B8%8F%20in-Graz%20(Austria)-0c674a) [![codecov](https://codecov.io/gh/adtzlr/felupe/branch/main/graph/badge.svg?token=J2QP6Y6LVH)](https://codecov.io/gh/adtzlr/felupe) [![DOI](https://zenodo.org/badge/360657894.svg)](https://zenodo.org/badge/latestdoi/360657894) ![Codestyle black](https://img.shields.io/badge/code%20style-black-black) ![GitHub Repo stars](https://img.shields.io/github/stars/adtzlr/felupe?logo=github) ![PyPI - Downloads](https://img.shields.io/pypi/dm/felupe) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/adtzlr/felupe-web/main?labpath=notebooks/binder/01_Getting-Started.ipynb) [![lite-badge](https://jupyterlite.rtfd.io/en/latest/_static/badge.svg)](https://adtzlr.github.io/felupe-web/lab?path=01_Getting-Started.ipynb) <a target="_blank" href="https://colab.research.google.com/github/adtzlr/felupe-web/blob/main/notebooks/colab/01_Getting-Started.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
 
 FElupe is a Python 3.7+ 🐍 finite element analysis package 📦 focussing on the formulation and numerical solution of nonlinear problems in continuum mechanics 🔧 of solid bodies 🚂. Its name is a combination of FE (finite element) and the german word *Lupe* 🔍 (magnifying glass) as a synonym for getting an insight 📖 how a finite element analysis code 🧮 looks like under the hood 🕳️.
 
+<p align="center">
+  <a href="https://felupe.readthedocs.io/en/latest/examples/rubberspring.html"><img src="https://user-images.githubusercontent.com/5793153/230604246-5a416081-6777-4f33-afdf-efdb51338722.png" height="70px"/></a> <a href="https://felupe.readthedocs.io/en/latest/examples/platewithhole.html"><img src="https://user-images.githubusercontent.com/5793153/230604587-42e3e339-e08c-4cc8-8000-f7046a8d95df.png" height="70px"/></a>
+</p>
+
 # Installation
 Install Python, fire up 🔥 a terminal and run 🏃
 
 ```shell
 pip install felupe[all]
 ```
```

### Comparing `felupe-7.4.0/README.md` & `felupe-7.4.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 <p align="center">
-  <img src="https://raw.githubusercontent.com/adtzlr/felupe/main/docs/_static/logo_light.svg" height="100px"/> <a href="https://felupe.readthedocs.io/en/latest/examples/rubberspring.html"><img src="https://user-images.githubusercontent.com/5793153/230604246-5a416081-6777-4f33-afdf-efdb51338722.png" height="100px"/></a> <a href="https://felupe.readthedocs.io/en/latest/examples/platewithhole.html"><img src="https://user-images.githubusercontent.com/5793153/230604587-42e3e339-e08c-4cc8-8000-f7046a8d95df.png" height="100px"/></a>
+  <a href="https://felupe.readthedocs.io/en/latest/?badge=latest"><img src="https://user-images.githubusercontent.com/5793153/235789118-eb03eb25-2556-401d-8a0f-580f37e72f8d.png" height="80px"/></a>
   <p align="center">Finite Element Analysis.</p>
 </p>
 
 [![PyPI version shields.io](https://img.shields.io/pypi/v/felupe.svg)](https://pypi.python.org/pypi/felupe/) [![Documentation Status](https://readthedocs.org/projects/felupe/badge/?version=latest)](https://felupe.readthedocs.io/en/latest/?badge=latest) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) ![Made with love in Graz (Austria)](https://img.shields.io/badge/Made%20with%20%E2%9D%A4%EF%B8%8F%20in-Graz%20(Austria)-0c674a) [![codecov](https://codecov.io/gh/adtzlr/felupe/branch/main/graph/badge.svg?token=J2QP6Y6LVH)](https://codecov.io/gh/adtzlr/felupe) [![DOI](https://zenodo.org/badge/360657894.svg)](https://zenodo.org/badge/latestdoi/360657894) ![Codestyle black](https://img.shields.io/badge/code%20style-black-black) ![GitHub Repo stars](https://img.shields.io/github/stars/adtzlr/felupe?logo=github) ![PyPI - Downloads](https://img.shields.io/pypi/dm/felupe) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/adtzlr/felupe-web/main?labpath=notebooks/binder/01_Getting-Started.ipynb) [![lite-badge](https://jupyterlite.rtfd.io/en/latest/_static/badge.svg)](https://adtzlr.github.io/felupe-web/lab?path=01_Getting-Started.ipynb) <a target="_blank" href="https://colab.research.google.com/github/adtzlr/felupe-web/blob/main/notebooks/colab/01_Getting-Started.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
 
 FElupe is a Python 3.7+ 🐍 finite element analysis package 📦 focussing on the formulation and numerical solution of nonlinear problems in continuum mechanics 🔧 of solid bodies 🚂. Its name is a combination of FE (finite element) and the german word *Lupe* 🔍 (magnifying glass) as a synonym for getting an insight 📖 how a finite element analysis code 🧮 looks like under the hood 🕳️.
 
+<p align="center">
+  <a href="https://felupe.readthedocs.io/en/latest/examples/rubberspring.html"><img src="https://user-images.githubusercontent.com/5793153/230604246-5a416081-6777-4f33-afdf-efdb51338722.png" height="70px"/></a> <a href="https://felupe.readthedocs.io/en/latest/examples/platewithhole.html"><img src="https://user-images.githubusercontent.com/5793153/230604587-42e3e339-e08c-4cc8-8000-f7046a8d95df.png" height="70px"/></a>
+</p>
+
 # Installation
 Install Python, fire up 🔥 a terminal and run 🏃
 
 ```shell
 pip install felupe[all]
 ```
```

#### html2text {}

```diff
@@ -1,12 +1,9 @@
-      [https://raw.githubusercontent.com/adtzlr/felupe/main/docs/_static/
- logo_light.svg] [https://user-images.githubusercontent.com/5793153/230604246-
-           5a416081-6777-4f33-afdf-efdb51338722.png] [https://user-
-    images.githubusercontent.com/5793153/230604587-42e3e339-e08c-4cc8-8000-
-                               f7046a8d95df.png]
+  [https://user-images.githubusercontent.com/5793153/235789118-eb03eb25-2556-
+                          401d-8a0f-580f37e72f8d.png]
                            Finite Element Analysis.
 [![PyPI version shields.io](https://img.shields.io/pypi/v/felupe.svg)](https://
 pypi.python.org/pypi/felupe/) [![Documentation Status](https://readthedocs.org/
 projects/felupe/badge/?version=latest)](https://felupe.readthedocs.io/en/
 latest/?badge=latest) [![License: GPL v3](https://img.shields.io/badge/License-
 GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) ![Made with love in Graz
 (Austria)](https://img.shields.io/badge/Made%20with%20%E2%9D%A4%EF%B8%8F%20in-
@@ -21,60 +18,63 @@
 Started.ipynb) [![lite-badge](https://jupyterlite.rtfd.io/en/latest/_static/
 badge.svg)](https://adtzlr.github.io/felupe-web/lab?path=01_Getting-
 Started.ipynb) [Open_In_Colab] FElupe is a Python 3.7+ ð finite element
 analysis package ð¦ focussing on the formulation and numerical solution of
 nonlinear problems in continuum mechanics ð§ of solid bodies ð. Its name
 is a combination of FE (finite element) and the german word *Lupe* ð
 (magnifying glass) as a synonym for getting an insight ð how a finite
-element analysis code ð§® looks like under the hood ð³ï¸. # Installation
-Install Python, fire up ð¥ a terminal and run ð ```shell pip install
-felupe[all] ``` where `[all]` installs all optional dependencies. FElupe has
-minimal dependencies, all available at PyPI supporting all platforms. * `numpy`
-for array operations * `scipy` for sparse matrices * `tensortrax` for automatic
-differentiation In order to make use of all features of FElupe
-ðð°ððð, it is suggested to install all optional dependencies. *
-`einsumt` for parallel assembly * `h5py` for XDMF result files * `matplotlib`
-for plotting graphs * `meshio` for mesh-related I/O * `pyvista` for interactive
-visualizations * `tqdm` for showing progress bars during job evaluation #
-Getting Started This tutorial covers the essential high-level parts of creating
-and solving problems with FElupe. As an introductory example ð¨âð«, a
-quarter model of a solid cube with hyperelastic material behaviour is subjected
-to a uniaxial elongation applied at a clamped end-face. First, letâs import
-FElupe and create a meshed cube out of hexahedron cells with a given number of
-points per axis. A numeric region, pre-defined for hexahedrons, is created on
-the mesh. A vector-valued displacement field is initiated on the region. Next,
-a field container is created on top of this field. A uniaxial load case is
-applied on the displacement field stored inside the field container. This
-involves setting up symmetry planes as well as the absolute value of the
-prescribed displacement at the mesh-points on the right-end face of the cube.
-The right-end face is *clamped* ð ï¸: only displacements in direction *x*
-are allowed. The dict of boundary conditions for this pre-defined load case are
-returned as `boundaries` and the partitioned degrees of freedom as well as the
-external displacements are stored within the returned dict `loadcase`. An
-isotropic pseudo-elastic Ogden-Roxburgh Mullins-softening model formulation in
-combination with an isotropic hyperelastic Neo-Hookean material formulation is
-applied on the displacement field of a nearly-incompressible solid body. A step
-generates the consecutive substep-movements of a given boundary condition. The
-step is further added to a list of steps of a job ð©âð» (here, a
-characteristic-curve ð job is used). During evaluation â³, each substep of
-each step is solved by an iterative Newton-Rhapson procedure âï¸. The
-solution is exported after each completed substep as a time-series â XDMF
-file. Finally, the result of the last completed substep is plotted. For more
-details beside this high-level code snippet, please have a look at the ð
-[documentation](https://felupe.readthedocs.io/en/latest/?badge=latest).
-```python import felupe as fem # create a hexahedron-region on a cube mesh =
-fem.Cube(n=6) region = fem.RegionHexahedron(mesh) # add a field container (with
-a vector-valued displacement field) field = fem.FieldContainer([fem.Field
-(region, dim=3)]) # apply a uniaxial elongation on the cube boundaries,
-loadcase = fem.dof.uniaxial(field, clamped=True) # define the constitutive
-material behaviour # and create a nearly-incompressible (u,p,J - formulation)
-solid body umat = fem.OgdenRoxburgh(material=fem.NeoHooke(mu=1), r=3, m=1,
-beta=0) solid = fem.SolidBodyNearlyIncompressible(umat, field, bulk=5000) #
-prepare a step with substeps move = fem.math.linsteps([0, 1, 0, 1, 2, 1],
-num=5) step = fem.Step(items=[solid], ramp={boundaries["move"]: move},
+element analysis code ð§® looks like under the hood ð³ï¸.
+  [https://user-images.githubusercontent.com/5793153/230604246-5a416081-6777-
+4f33-afdf-efdb51338722.png] [https://user-images.githubusercontent.com/5793153/
+              230604587-42e3e339-e08c-4cc8-8000-f7046a8d95df.png]
+# Installation Install Python, fire up ð¥ a terminal and run ð ```shell
+pip install felupe[all] ``` where `[all]` installs all optional dependencies.
+FElupe has minimal dependencies, all available at PyPI supporting all
+platforms. * `numpy` for array operations * `scipy` for sparse matrices *
+`tensortrax` for automatic differentiation In order to make use of all features
+of FElupe ðð°ððð, it is suggested to install all optional
+dependencies. * `einsumt` for parallel assembly * `h5py` for XDMF result files
+* `matplotlib` for plotting graphs * `meshio` for mesh-related I/O * `pyvista`
+for interactive visualizations * `tqdm` for showing progress bars during job
+evaluation # Getting Started This tutorial covers the essential high-level
+parts of creating and solving problems with FElupe. As an introductory example
+ð¨âð«, a quarter model of a solid cube with hyperelastic material
+behaviour is subjected to a uniaxial elongation applied at a clamped end-face.
+First, letâs import FElupe and create a meshed cube out of hexahedron cells
+with a given number of points per axis. A numeric region, pre-defined for
+hexahedrons, is created on the mesh. A vector-valued displacement field is
+initiated on the region. Next, a field container is created on top of this
+field. A uniaxial load case is applied on the displacement field stored inside
+the field container. This involves setting up symmetry planes as well as the
+absolute value of the prescribed displacement at the mesh-points on the right-
+end face of the cube. The right-end face is *clamped* ð ï¸: only
+displacements in direction *x* are allowed. The dict of boundary conditions for
+this pre-defined load case are returned as `boundaries` and the partitioned
+degrees of freedom as well as the external displacements are stored within the
+returned dict `loadcase`. An isotropic pseudo-elastic Ogden-Roxburgh Mullins-
+softening model formulation in combination with an isotropic hyperelastic Neo-
+Hookean material formulation is applied on the displacement field of a nearly-
+incompressible solid body. A step generates the consecutive substep-movements
+of a given boundary condition. The step is further added to a list of steps of
+a job ð©âð» (here, a characteristic-curve ð job is used). During
+evaluation â³, each substep of each step is solved by an iterative Newton-
+Rhapson procedure âï¸. The solution is exported after each completed substep
+as a time-series â XDMF file. Finally, the result of the last completed
+substep is plotted. For more details beside this high-level code snippet,
+please have a look at the ð [documentation](https://felupe.readthedocs.io/
+en/latest/?badge=latest). ```python import felupe as fem # create a hexahedron-
+region on a cube mesh = fem.Cube(n=6) region = fem.RegionHexahedron(mesh) # add
+a field container (with a vector-valued displacement field) field =
+fem.FieldContainer([fem.Field(region, dim=3)]) # apply a uniaxial elongation on
+the cube boundaries, loadcase = fem.dof.uniaxial(field, clamped=True) # define
+the constitutive material behaviour # and create a nearly-incompressible (u,p,J
+- formulation) solid body umat = fem.OgdenRoxburgh(material=fem.NeoHooke(mu=1),
+r=3, m=1, beta=0) solid = fem.SolidBodyNearlyIncompressible(umat, field,
+bulk=5000) # prepare a step with substeps move = fem.math.linsteps([0, 1, 0, 1,
+2, 1], num=5) step = fem.Step(items=[solid], ramp={boundaries["move"]: move},
 boundaries=boundaries) # add the step to a job, evaluate all substeps and
 create a plot job = fem.CharacteristicCurve(steps=[step], boundary=boundaries
 ["move"]) job.evaluate(filename="result.xdmf") fig, ax = job.plot
 ( xlabel="Displacement $u$ in mm $\longrightarrow$", ylabel="Normal Force $F$
 in N $\longrightarrow$", ) # visualize the results view = fem.View(field)
 view.plot("Principal Values of Logarithmic Strain").show() ``` ![curve](https:/
 /user-images.githubusercontent.com/5793153/234382805-d9a56108-9dd7-4f57-a029-
```

### Comparing `felupe-7.4.0/pyproject.toml` & `felupe-7.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/__init__.py` & `felupe-7.4.1/src/felupe/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/_assembly/_axi.py` & `felupe-7.4.1/src/felupe/_assembly/_axi.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/_assembly/_base.py` & `felupe-7.4.1/src/felupe/_assembly/_base.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/_assembly/_form.py` & `felupe-7.4.1/src/felupe/_assembly/_form.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/_assembly/_mixed.py` & `felupe-7.4.1/src/felupe/_assembly/_mixed.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/_basis/_basis.py` & `felupe-7.4.1/src/felupe/_basis/_basis.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/_field/_axi.py` & `felupe-7.4.1/src/felupe/_field/_axi.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/_field/_base.py` & `felupe-7.4.1/src/felupe/_field/_base.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/_field/_container.py` & `felupe-7.4.1/src/felupe/_field/_container.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/_field/_fields.py` & `felupe-7.4.1/src/felupe/_field/_fields.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/_field/_indices.py` & `felupe-7.4.1/src/felupe/_field/_indices.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/_field/_planestrain.py` & `felupe-7.4.1/src/felupe/_field/_planestrain.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/constitution/__init__.py` & `felupe-7.4.1/src/felupe/constitution/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/constitution/_kinematics.py` & `felupe-7.4.1/src/felupe/constitution/_kinematics.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/constitution/_mixed.py` & `felupe-7.4.1/src/felupe/constitution/_mixed.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/constitution/_models_hyperelasticity.py` & `felupe-7.4.1/src/felupe/constitution/_models_hyperelasticity.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/constitution/_models_hyperelasticity_ad.py` & `felupe-7.4.1/src/felupe/constitution/_models_hyperelasticity_ad.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/constitution/_models_linear_elasticity.py` & `felupe-7.4.1/src/felupe/constitution/_models_linear_elasticity.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/constitution/_models_pseudo_elasticity.py` & `felupe-7.4.1/src/felupe/constitution/_models_pseudo_elasticity.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/constitution/_user_materials.py` & `felupe-7.4.1/src/felupe/constitution/_user_materials.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/constitution/_user_materials_hyperelastic.py` & `felupe-7.4.1/src/felupe/constitution/_user_materials_hyperelastic.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/constitution/_user_materials_models.py` & `felupe-7.4.1/src/felupe/constitution/_user_materials_models.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/dof/_boundary.py` & `felupe-7.4.1/src/felupe/dof/_boundary.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/dof/_loadcase.py` & `felupe-7.4.1/src/felupe/dof/_loadcase.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/dof/_tools.py` & `felupe-7.4.1/src/felupe/dof/_tools.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/element/__init__.py` & `felupe-7.4.1/src/felupe/element/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/element/_base.py` & `felupe-7.4.1/src/felupe/element/_base.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/element/_hexahedron.py` & `felupe-7.4.1/src/felupe/element/_hexahedron.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/element/_lagrange.py` & `felupe-7.4.1/src/felupe/element/_lagrange.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/element/_line.py` & `felupe-7.4.1/src/felupe/element/_line.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/element/_quad.py` & `felupe-7.4.1/src/felupe/element/_quad.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/element/_tetra.py` & `felupe-7.4.1/src/felupe/element/_tetra.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/element/_triangle.py` & `felupe-7.4.1/src/felupe/element/_triangle.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/math/__init__.py` & `felupe-7.4.1/src/felupe/math/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/math/_field.py` & `felupe-7.4.1/src/felupe/math/_field.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/math/_math.py` & `felupe-7.4.1/src/felupe/math/_math.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/math/_spatial.py` & `felupe-7.4.1/src/felupe/math/_spatial.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/math/_tensor.py` & `felupe-7.4.1/src/felupe/math/_tensor.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/mechanics/__init__.py` & `felupe-7.4.1/src/felupe/mechanics/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/mechanics/_curve.py` & `felupe-7.4.1/src/felupe/mechanics/_curve.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/mechanics/_helpers.py` & `felupe-7.4.1/src/felupe/mechanics/_helpers.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/mechanics/_job.py` & `felupe-7.4.1/src/felupe/mechanics/_job.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/mechanics/_multipoint.py` & `felupe-7.4.1/src/felupe/mechanics/_multipoint.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/mechanics/_pointload.py` & `felupe-7.4.1/src/felupe/mechanics/_pointload.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/mechanics/_solidbody.py` & `felupe-7.4.1/src/felupe/mechanics/_solidbody.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/mechanics/_solidbody_gravity.py` & `felupe-7.4.1/src/felupe/mechanics/_solidbody_gravity.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/mechanics/_solidbody_incompressible.py` & `felupe-7.4.1/src/felupe/mechanics/_solidbody_incompressible.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/mechanics/_solidbody_pressure.py` & `felupe-7.4.1/src/felupe/mechanics/_solidbody_pressure.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/mechanics/_step.py` & `felupe-7.4.1/src/felupe/mechanics/_step.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/mesh/__init__.py` & `felupe-7.4.1/src/felupe/mesh/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/mesh/_container.py` & `felupe-7.4.1/src/felupe/mesh/_container.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/mesh/_convert.py` & `felupe-7.4.1/src/felupe/mesh/_convert.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/mesh/_discrete_geometry.py` & `felupe-7.4.1/src/felupe/mesh/_discrete_geometry.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/mesh/_dual.py` & `felupe-7.4.1/src/felupe/mesh/_dual.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/mesh/_geometry.py` & `felupe-7.4.1/src/felupe/mesh/_geometry.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/mesh/_helpers.py` & `felupe-7.4.1/src/felupe/mesh/_helpers.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/mesh/_line_rectangle_cube.py` & `felupe-7.4.1/src/felupe/mesh/_line_rectangle_cube.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/mesh/_mesh.py` & `felupe-7.4.1/src/felupe/mesh/_mesh.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/mesh/_read.py` & `felupe-7.4.1/src/felupe/mesh/_read.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/mesh/_tools.py` & `felupe-7.4.1/src/felupe/mesh/_tools.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/quadrature/_base.py` & `felupe-7.4.1/src/felupe/quadrature/_base.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/quadrature/_gausslegendre.py` & `felupe-7.4.1/src/felupe/quadrature/_gausslegendre.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/quadrature/_tetra.py` & `felupe-7.4.1/src/felupe/quadrature/_tetra.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/quadrature/_triangle.py` & `felupe-7.4.1/src/felupe/quadrature/_triangle.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/region/__init__.py` & `felupe-7.4.1/src/felupe/region/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/region/_boundary.py` & `felupe-7.4.1/src/felupe/region/_boundary.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/region/_region.py` & `felupe-7.4.1/src/felupe/region/_region.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/region/_templates.py` & `felupe-7.4.1/src/felupe/region/_templates.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/solve/_solve.py` & `felupe-7.4.1/src/felupe/solve/_solve.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/tools/__init__.py` & `felupe-7.4.1/src/felupe/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/tools/_misc.py` & `felupe-7.4.1/src/felupe/tools/_misc.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/tools/_newton.py` & `felupe-7.4.1/src/felupe/tools/_newton.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/tools/_plot.py` & `felupe-7.4.1/src/felupe/tools/_plot.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/tools/_post.py` & `felupe-7.4.1/src/felupe/tools/_post.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/tools/_project.py` & `felupe-7.4.1/src/felupe/tools/_project.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/tools/_save.py` & `felupe-7.4.1/src/felupe/tools/_save.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe/tools/_solve.py` & `felupe-7.4.1/src/felupe/tools/_solve.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/src/felupe.egg-info/PKG-INFO` & `felupe-7.4.1/src/felupe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: felupe
-Version: 7.4.0
+Version: 7.4.1
 Summary: Finite Element Analysis
 Author: Andreas Dutzler
 Author-email: a.dutzler@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -701,22 +701,26 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: all
 License-File: LICENSE
 
 <p align="center">
-  <img src="https://raw.githubusercontent.com/adtzlr/felupe/main/docs/_static/logo_light.svg" height="100px"/> <a href="https://felupe.readthedocs.io/en/latest/examples/rubberspring.html"><img src="https://user-images.githubusercontent.com/5793153/230604246-5a416081-6777-4f33-afdf-efdb51338722.png" height="100px"/></a> <a href="https://felupe.readthedocs.io/en/latest/examples/platewithhole.html"><img src="https://user-images.githubusercontent.com/5793153/230604587-42e3e339-e08c-4cc8-8000-f7046a8d95df.png" height="100px"/></a>
+  <a href="https://felupe.readthedocs.io/en/latest/?badge=latest"><img src="https://user-images.githubusercontent.com/5793153/235789118-eb03eb25-2556-401d-8a0f-580f37e72f8d.png" height="80px"/></a>
   <p align="center">Finite Element Analysis.</p>
 </p>
 
 [![PyPI version shields.io](https://img.shields.io/pypi/v/felupe.svg)](https://pypi.python.org/pypi/felupe/) [![Documentation Status](https://readthedocs.org/projects/felupe/badge/?version=latest)](https://felupe.readthedocs.io/en/latest/?badge=latest) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) ![Made with love in Graz (Austria)](https://img.shields.io/badge/Made%20with%20%E2%9D%A4%EF%B8%8F%20in-Graz%20(Austria)-0c674a) [![codecov](https://codecov.io/gh/adtzlr/felupe/branch/main/graph/badge.svg?token=J2QP6Y6LVH)](https://codecov.io/gh/adtzlr/felupe) [![DOI](https://zenodo.org/badge/360657894.svg)](https://zenodo.org/badge/latestdoi/360657894) ![Codestyle black](https://img.shields.io/badge/code%20style-black-black) ![GitHub Repo stars](https://img.shields.io/github/stars/adtzlr/felupe?logo=github) ![PyPI - Downloads](https://img.shields.io/pypi/dm/felupe) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/adtzlr/felupe-web/main?labpath=notebooks/binder/01_Getting-Started.ipynb) [![lite-badge](https://jupyterlite.rtfd.io/en/latest/_static/badge.svg)](https://adtzlr.github.io/felupe-web/lab?path=01_Getting-Started.ipynb) <a target="_blank" href="https://colab.research.google.com/github/adtzlr/felupe-web/blob/main/notebooks/colab/01_Getting-Started.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
 
 FElupe is a Python 3.7+ 🐍 finite element analysis package 📦 focussing on the formulation and numerical solution of nonlinear problems in continuum mechanics 🔧 of solid bodies 🚂. Its name is a combination of FE (finite element) and the german word *Lupe* 🔍 (magnifying glass) as a synonym for getting an insight 📖 how a finite element analysis code 🧮 looks like under the hood 🕳️.
 
+<p align="center">
+  <a href="https://felupe.readthedocs.io/en/latest/examples/rubberspring.html"><img src="https://user-images.githubusercontent.com/5793153/230604246-5a416081-6777-4f33-afdf-efdb51338722.png" height="70px"/></a> <a href="https://felupe.readthedocs.io/en/latest/examples/platewithhole.html"><img src="https://user-images.githubusercontent.com/5793153/230604587-42e3e339-e08c-4cc8-8000-f7046a8d95df.png" height="70px"/></a>
+</p>
+
 # Installation
 Install Python, fire up 🔥 a terminal and run 🏃
 
 ```shell
 pip install felupe[all]
 ```
```

### Comparing `felupe-7.4.0/src/felupe.egg-info/SOURCES.txt` & `felupe-7.4.1/src/felupe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/tests/test_basis.py` & `felupe-7.4.1/tests/test_basis.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/tests/test_bilinearform.py` & `felupe-7.4.1/tests/test_bilinearform.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/tests/test_composite.py` & `felupe-7.4.1/tests/test_composite.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/tests/test_constitution.py` & `felupe-7.4.1/tests/test_constitution.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/tests/test_dof.py` & `felupe-7.4.1/tests/test_dof.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/tests/test_element.py` & `felupe-7.4.1/tests/test_element.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/tests/test_field.py` & `felupe-7.4.1/tests/test_field.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/tests/test_form.py` & `felupe-7.4.1/tests/test_form.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/tests/test_job.py` & `felupe-7.4.1/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/tests/test_math.py` & `felupe-7.4.1/tests/test_math.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/tests/test_mechanics.py` & `felupe-7.4.1/tests/test_mechanics.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/tests/test_mesh.py` & `felupe-7.4.1/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/tests/test_mpc.py` & `felupe-7.4.1/tests/test_mpc.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/tests/test_planestrain.py` & `felupe-7.4.1/tests/test_planestrain.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/tests/test_plot.py` & `felupe-7.4.1/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/tests/test_quadrature.py` & `felupe-7.4.1/tests/test_quadrature.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/tests/test_readme.py` & `felupe-7.4.1/tests/test_readme.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/tests/test_region.py` & `felupe-7.4.1/tests/test_region.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/tests/test_solve.py` & `felupe-7.4.1/tests/test_solve.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.0/tests/test_tools.py` & `felupe-7.4.1/tests/test_tools.py`

 * *Files identical despite different names*

