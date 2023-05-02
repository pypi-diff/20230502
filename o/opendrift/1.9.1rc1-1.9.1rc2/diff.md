# Comparing `tmp/opendrift-1.9.1rc1.tar.gz` & `tmp/opendrift-1.9.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opendrift-1.9.1rc1.tar", max compression
+gzip compressed data, was "opendrift-1.9.1rc2.tar", max compression
```

## Comparing `opendrift-1.9.1rc1.tar` & `opendrift-1.9.1rc2.tar`

### file list

```diff
@@ -1,188 +1,188 @@
--rw-r--r--   0        0        0    18092 2020-02-04 12:59:28.094781 opendrift-1.9.1rc1/LICENSE
--rw-r--r--   0        0        0     7293 2022-01-03 13:34:45.420795 opendrift-1.9.1rc1/opendrift/__init__.py
--rw-r--r--   0        0        0     1954 2021-03-05 15:37:49.611897 opendrift-1.9.1rc1/opendrift/elements/__init__.py
--rw-r--r--   0        0        0    10641 2021-03-05 15:37:49.615897 opendrift-1.9.1rc1/opendrift/elements/elements.py
--rw-r--r--   0        0        0     1030 2021-03-05 15:37:49.615897 opendrift-1.9.1rc1/opendrift/elements/passivetracer.py
--rw-r--r--   0        0        0      226 2022-03-14 11:12:16.165241 opendrift-1.9.1rc1/opendrift/errors.py
--rw-r--r--   0        0        0        0 2020-02-04 12:59:28.938787 opendrift-1.9.1rc1/opendrift/export/__init__.py
--rw-r--r--   0        0        0    16786 2022-01-03 08:32:44.609576 opendrift-1.9.1rc1/opendrift/export/io_netcdf.py
--rw-r--r--   0        0        0    16526 2020-02-04 12:59:28.930787 opendrift-1.9.1rc1/opendrift/models/OBJECTPROP.DAT
--rw-r--r--   0        0        0       32 2021-03-05 15:37:49.615897 opendrift-1.9.1rc1/opendrift/models/__init__.py
--rw-r--r--   0        0        0   240307 2022-08-25 10:29:50.032354 opendrift-1.9.1rc1/opendrift/models/basemodel.py
--rw-r--r--   0        0        0   120412 2022-09-06 09:12:17.126755 opendrift-1.9.1rc1/opendrift/models/chemicaldrift.py
--rw-r--r--   0        0        0      658 2022-06-02 16:46:38.860396 opendrift-1.9.1rc1/opendrift/models/eulerdrift/__init__.py
--rw-r--r--   0        0        0      325 2022-06-02 16:46:38.860396 opendrift-1.9.1rc1/opendrift/models/eulerdrift/diff.py
--rw-r--r--   0        0        0     3149 2022-07-16 14:34:16.703808 opendrift-1.9.1rc1/opendrift/models/eulerdrift/grid.py
--rw-r--r--   0        0        0      343 2022-06-02 16:46:38.860396 opendrift-1.9.1rc1/opendrift/models/eulerdrift/interp.py
--rw-r--r--   0        0        0     2396 2022-06-02 16:46:38.860396 opendrift-1.9.1rc1/opendrift/models/eulerdrift/readers.py
--rw-r--r--   0        0        0     7655 2022-06-02 16:46:38.860396 opendrift-1.9.1rc1/opendrift/models/eulerdrift/simulation.py
--rw-r--r--   0        0        0      948 2022-06-02 16:46:38.860396 opendrift-1.9.1rc1/opendrift/models/eulerdrift/srs.py
--rw-r--r--   0        0        0    11394 2022-01-03 08:32:44.613576 opendrift-1.9.1rc1/opendrift/models/larvalfish.py
--rw-r--r--   0        0        0    19700 2022-01-13 08:10:13.973543 opendrift-1.9.1rc1/opendrift/models/leeway.py
--rw-r--r--   0        0        0    12134 2021-03-05 15:37:49.615897 opendrift-1.9.1rc1/opendrift/models/model_template.py
--rw-r--r--   0        0        0    37666 2022-07-16 14:09:51.724350 opendrift-1.9.1rc1/opendrift/models/oceandrift.py
--rw-r--r--   0        0        0    13406 2021-03-05 15:37:49.619897 opendrift-1.9.1rc1/opendrift/models/openberg.py
--rw-r--r--   0        0        0       23 2022-01-03 13:34:45.424795 opendrift-1.9.1rc1/opendrift/models/openoil/__init__.py
--rw-r--r--   0        0        0      371 2022-01-03 13:34:45.424795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/README.md
--rw-r--r--   0        0        0      928 2022-01-31 13:18:42.337403 opendrift-1.9.1rc1/opendrift/models/openoil/adios/__init__.py
--rw-r--r--   0        0        0      256 2022-01-03 13:34:45.424795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/computation/__init__.py
--rw-r--r--   0        0        0     7477 2022-01-03 13:34:45.424795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/computation/estimations.py
--rw-r--r--   0        0        0    17896 2022-01-03 13:34:45.424795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/computation/gnome_oil.py
--rw-r--r--   0        0        0    14868 2022-01-03 13:34:45.424795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/computation/physical_properties.py
--rwxr-xr-x   0        0        0     1172 2022-01-03 13:34:45.424795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/csv_to_json.py
--rw-r--r--   0        0        0     2840 2022-01-03 13:34:45.424795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/dirjs.py
--rw-r--r--   0        0        0    12064 2022-01-03 13:34:45.424795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03128.json
--rw-r--r--   0        0        0    12782 2022-03-14 11:12:16.169241 opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03129.json
--rw-r--r--   0        0        0    14059 2022-03-14 11:12:16.169241 opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03130.json
--rw-r--r--   0        0        0    11629 2022-01-03 13:34:45.424795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03131.json
--rw-r--r--   0        0        0    11658 2022-03-14 11:12:16.169241 opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03132.json
--rw-r--r--   0        0        0    11366 2022-03-14 11:12:16.169241 opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03133.json
--rw-r--r--   0        0        0    10656 2022-03-14 11:12:16.169241 opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03134.json
--rw-r--r--   0        0        0    11729 2022-03-14 11:12:16.169241 opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03135.json
--rw-r--r--   0        0        0    12628 2022-01-03 13:34:45.424795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03136.json
--rw-r--r--   0        0        0    12498 2022-01-03 13:34:45.424795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03137.json
--rw-r--r--   0        0        0    12175 2022-01-03 13:34:45.424795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03138.json
--rw-r--r--   0        0        0    11693 2022-01-03 13:34:45.424795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03139.json
--rw-r--r--   0        0        0    11616 2022-01-03 13:34:45.424795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03140.json
--rw-r--r--   0        0        0     9372 2022-01-03 13:34:45.424795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03141.json
--rw-r--r--   0        0        0    11545 2022-03-14 11:12:16.169241 opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03142.json
--rw-r--r--   0        0        0    11132 2022-03-14 11:12:16.169241 opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03143.json
--rw-r--r--   0        0        0    12184 2022-03-14 11:12:16.169241 opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03144.json
--rw-r--r--   0        0        0    11276 2022-01-03 13:34:45.428795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03145.json
--rw-r--r--   0        0        0    11729 2022-01-31 13:18:42.337403 opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03146.json
--rw-r--r--   0        0        0    12834 2022-03-14 11:12:16.169241 opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03147.json
--rw-r--r--   0        0        0    15136 2022-03-14 11:12:16.169241 opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03148.json
--rw-r--r--   0        0        0    13753 2022-03-14 11:12:16.169241 opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03149.json
--rw-r--r--   0        0        0    16359 2022-03-14 11:12:16.169241 opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03150.json
--rw-r--r--   0        0        0    14551 2022-03-14 11:12:16.169241 opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03151.json
--rw-r--r--   0        0        0    10815 2022-03-14 11:12:16.169241 opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03152.json
--rw-r--r--   0        0        0    10974 2022-03-14 11:12:16.169241 opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03153.json
--rw-r--r--   0        0        0    15843 2022-01-03 13:34:45.428795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD04000.json
--rw-r--r--   0        0        0    17688 2022-01-03 13:34:45.428795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD04001.json
--rw-r--r--   0        0        0    16375 2022-01-03 13:34:45.428795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD04002.json
--rw-r--r--   0        0        0     6987 2022-01-03 13:34:45.428795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD04003.json
--rw-r--r--   0        0        0     7748 2022-01-03 13:34:45.428795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD04004.json
--rw-r--r--   0        0        0    11360 2022-01-03 13:34:45.428795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD04006.json
--rw-r--r--   0        0        0    13012 2022-01-03 13:34:45.428795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD04007.json
--rw-r--r--   0        0        0    11363 2022-01-03 13:34:45.428795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD04008.json
--rw-r--r--   0        0        0    12614 2022-01-03 13:34:45.428795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD04009.json
--rw-r--r--   0        0        0    14255 2022-01-03 13:34:45.428795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD04010.json
--rw-r--r--   0        0        0    14094 2022-01-03 13:34:45.428795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD04011.json
--rw-r--r--   0        0        0    14088 2022-01-03 13:34:45.428795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD04012.json
--rw-r--r--   0        0        0    14094 2022-01-03 13:34:45.428795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD04013.json
--rw-r--r--   0        0        0     5106 2022-01-03 13:34:45.428795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD04014.json
--rw-r--r--   0        0        0        0 2022-01-03 13:34:45.428795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/__init__.py
--rwxr-xr-x   0        0        0       56 2022-03-14 11:12:16.169241 opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/clean_lines.bash
--rw-r--r--   0        0        0    14224 2022-03-14 11:12:16.169241 opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/oillibnorway.csv
--rw-r--r--   0        0        0    12953 2022-01-03 13:34:45.428795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/oillibtest.csv
--rw-r--r--   0        0        0    15737 2022-09-06 09:12:17.126755 opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/templates/parse_oil_pdf.py
--rw-r--r--   0        0        0     2377 2022-01-03 13:34:45.428795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/harvest_oils.py
--rw-r--r--   0        0        0        0 2022-01-03 13:34:45.428795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/__init__.py
--rw-r--r--   0        0        0      740 2022-01-03 13:34:45.428795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/common/__init__.py
--rw-r--r--   0        0        0      876 2022-01-03 13:34:45.428795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/common/enum_types.py
--rw-r--r--   0        0        0      350 2022-01-03 13:34:45.428795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/common/label.py
--rw-r--r--   0        0        0    12121 2022-01-03 13:34:45.428795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/common/measurement.py
--rw-r--r--   0        0        0     1972 2022-01-03 13:34:45.428795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/common/sara.py
--rw-r--r--   0        0        0      144 2022-01-03 13:34:45.428795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/common/synonym.py
--rw-r--r--   0        0        0     5957 2022-01-03 13:34:45.428795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/common/utilities.py
--rw-r--r--   0        0        0     3546 2022-01-03 13:34:45.428795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/common/validators.py
--rw-r--r--   0        0        0        0 2022-01-03 13:34:45.428795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/__init__.py
--rw-r--r--   0        0        0      567 2022-01-03 13:34:45.428795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/bulk_composition.py
--rw-r--r--   0        0        0      558 2022-01-03 13:34:45.428795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/ccme.py
--rw-r--r--   0        0        0      723 2022-01-03 13:34:45.428795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/cleanup/__init__.py
--rw-r--r--   0        0        0    14087 2022-01-03 13:34:45.428795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/cleanup/add_labels.py
--rw-r--r--   0        0        0      926 2022-01-03 13:34:45.428795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/cleanup/cleanup.py
--rw-r--r--   0        0        0     2805 2022-01-03 13:34:45.432795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/cleanup/density.py
--rw-r--r--   0        0        0     1825 2022-01-03 13:34:45.432795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/cleanup/distillation.py
--rw-r--r--   0        0        0     5946 2022-01-03 13:34:45.432795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/completeness.py
--rw-r--r--   0        0        0     1194 2022-01-03 13:34:45.432795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/compound.py
--rw-r--r--   0        0        0     3020 2022-01-03 13:34:45.432795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/distillation.py
--rw-r--r--   0        0        0      727 2022-01-03 13:34:45.432795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/environmental_behavior.py
--rw-r--r--   0        0        0      672 2022-01-03 13:34:45.432795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/ests_fractions.py
--rw-r--r--   0        0        0      698 2022-01-03 13:34:45.432795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/industry_property.py
--rw-r--r--   0        0        0     2014 2022-01-03 13:34:45.432795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/location_coordinates.py
--rw-r--r--   0        0        0     2193 2022-01-03 13:34:45.432795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/metadata.py
--rw-r--r--   0        0        0     5876 2022-01-03 13:34:45.432795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/oil.py
--rw-r--r--   0        0        0     4273 2022-01-03 13:34:45.432795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/physical_properties.py
--rw-r--r--   0        0        0     2661 2022-01-03 13:34:45.432795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/product_type.py
--rw-r--r--   0        0        0     2092 2022-01-03 13:34:45.432795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/product_types_and_labels.csv
--rw-r--r--   0        0        0     2391 2022-01-03 13:34:45.432795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/properties.py
--rw-r--r--   0        0        0     1109 2022-01-03 13:34:45.432795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/review_status.py
--rw-r--r--   0        0        0     3692 2022-01-03 13:34:45.432795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/sample.py
--rw-r--r--   0        0        0      502 2022-01-03 13:34:45.432795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/sara.py
--rw-r--r--   0        0        0        6 2022-01-03 13:34:45.432795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/validation/__init__.py
--rw-r--r--   0        0        0      943 2022-01-03 13:34:45.432795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/validation/errors.py
--rw-r--r--   0        0        0     1180 2022-01-03 13:34:45.432795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/validation/validate.py
--rw-r--r--   0        0        0      879 2022-01-03 13:34:45.432795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/validation/warnings.py
--rw-r--r--   0        0        0      726 2022-01-03 13:34:45.432795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/values.py
--rw-r--r--   0        0        0     1793 2022-01-03 13:34:45.432795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/version.py
--rw-r--r--   0        0        0     2640 2022-01-03 13:34:45.432795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/version_update.py
--rw-r--r--   0        0        0      741 2022-01-03 13:34:45.432795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/versions.py
--rw-r--r--   0        0        0     4676 2022-01-03 13:34:45.432795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/oil.py
--rw-r--r--   0        0        0   442560 2022-01-03 13:34:45.432795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/oils.xz
--rw-r--r--   0        0        0        0 2022-01-03 13:34:45.432795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/util/__init__.py
--rw-r--r--   0        0        0    13382 2022-01-03 13:34:45.432795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/util/estimations.py
--rw-r--r--   0        0        0     3507 2022-01-03 13:34:45.432795 opendrift-1.9.1rc1/opendrift/models/openoil/adios/util/many_many.py
--rw-r--r--   0        0        0     1418 2022-01-03 13:34:45.432795 opendrift-1.9.1rc1/opendrift/models/openoil/noaa_oil_weathering.py
--rw-r--r--   0        0        0    74753 2022-08-19 13:17:11.790014 opendrift-1.9.1rc1/opendrift/models/openoil/openoil.py
--rw-r--r--   0        0        0     7525 2022-01-03 08:32:44.613576 opendrift-1.9.1rc1/opendrift/models/pelagicegg.py
--rw-r--r--   0        0        0    40791 2022-01-31 13:18:42.337403 opendrift-1.9.1rc1/opendrift/models/physics_methods.py
--rw-r--r--   0        0        0     4114 2022-01-03 08:32:44.613576 opendrift-1.9.1rc1/opendrift/models/plastdrift.py
--rw-r--r--   0        0        0    73052 2022-03-14 11:12:16.169241 opendrift-1.9.1rc1/opendrift/models/radionuclides.py
--rw-r--r--   0        0        0     1535 2021-03-05 15:37:49.619897 opendrift-1.9.1rc1/opendrift/models/seaicedrift.py
--rw-r--r--   0        0        0    19003 2022-01-03 08:32:44.613576 opendrift-1.9.1rc1/opendrift/models/sealice.py
--rw-r--r--   0        0        0     4382 2022-01-03 08:32:44.613576 opendrift-1.9.1rc1/opendrift/models/sedimentdrift.py
--rw-r--r--   0        0        0    16188 2022-03-14 11:12:16.169241 opendrift-1.9.1rc1/opendrift/models/shipdrift.py
--rw-r--r--   0        0        0     2786 2020-02-04 12:59:28.930787 opendrift-1.9.1rc1/opendrift/models/wforce.dat
--rw-r--r--   0        0        0     1401 2021-10-15 06:07:51.948992 opendrift-1.9.1rc1/opendrift/models/windblow.py
--rw-r--r--   0        0        0     2873 2022-01-03 08:32:44.613576 opendrift-1.9.1rc1/opendrift/readers/__init__.py
--rw-r--r--   0        0        0    18608 2022-08-17 09:16:24.928658 opendrift-1.9.1rc1/opendrift/readers/basereader/__init__.py
--rw-r--r--   0        0        0     1608 2021-06-09 07:33:51.628938 opendrift-1.9.1rc1/opendrift/readers/basereader/consts.py
--rw-r--r--   0        0        0     1531 2021-03-05 15:37:49.623897 opendrift-1.9.1rc1/opendrift/readers/basereader/continuous.py
--rw-r--r--   0        0        0      335 2021-03-05 15:37:49.623897 opendrift-1.9.1rc1/opendrift/readers/basereader/fakeproj.py
--rw-r--r--   0        0        0    24363 2022-08-17 09:16:22.304652 opendrift-1.9.1rc1/opendrift/readers/basereader/structured.py
--rw-r--r--   0        0        0     5699 2021-05-28 07:34:17.640297 opendrift-1.9.1rc1/opendrift/readers/basereader/unstructured.py
--rw-r--r--   0        0        0    33873 2022-08-25 10:25:48.412419 opendrift-1.9.1rc1/opendrift/readers/basereader/variables.py
--rw-r--r--   0        0        0       66 2021-03-05 15:37:49.623897 opendrift-1.9.1rc1/opendrift/readers/interpolation/__init__.py
--rw-r--r--   0        0        0     7876 2022-04-19 13:39:31.757022 opendrift-1.9.1rc1/opendrift/readers/interpolation/interpolators.py
--rw-r--r--   0        0        0     6500 2021-03-05 15:37:49.623897 opendrift-1.9.1rc1/opendrift/readers/interpolation/structured.py
--rw-r--r--   0        0        0       77 2022-08-17 09:16:24.928658 opendrift-1.9.1rc1/opendrift/readers/operators/__init__.py
--rw-r--r--   0        0        0      613 2022-08-25 10:31:54.484385 opendrift-1.9.1rc1/opendrift/readers/operators/filter.py
--rw-r--r--   0        0        0     1775 2022-08-25 10:33:47.844422 opendrift-1.9.1rc1/opendrift/readers/operators/numops.py
--rw-r--r--   0        0        0     1562 2022-08-17 10:18:16.319417 opendrift-1.9.1rc1/opendrift/readers/operators/ops.py
--rw-r--r--   0        0        0     2015 2022-08-25 10:29:50.032354 opendrift-1.9.1rc1/opendrift/readers/operators/readerops.py
--rw-r--r--   0        0        0     2722 2021-03-05 15:37:49.623897 opendrift-1.9.1rc1/opendrift/readers/reader_ArtificialOceanEddy.py
--rw-r--r--   0        0        0    26777 2022-04-19 13:39:31.757022 opendrift-1.9.1rc1/opendrift/readers/reader_ROMS_native.py
--rw-r--r--   0        0        0     1912 2022-08-09 11:26:36.990944 opendrift-1.9.1rc1/opendrift/readers/reader_constant.py
--rw-r--r--   0        0        0     1675 2021-03-05 15:37:49.623897 opendrift-1.9.1rc1/opendrift/readers/reader_constant_2d.py
--rw-r--r--   0        0        0     5362 2021-03-05 15:37:49.623897 opendrift-1.9.1rc1/opendrift/readers/reader_current_from_drifter.py
--rw-r--r--   0        0        0     3659 2021-03-05 15:37:49.623897 opendrift-1.9.1rc1/opendrift/readers/reader_current_from_track.py
--rw-r--r--   0        0        0     2696 2021-03-05 15:37:49.627897 opendrift-1.9.1rc1/opendrift/readers/reader_double_gyre.py
--rw-r--r--   0        0        0     8823 2022-03-16 09:34:05.975572 opendrift-1.9.1rc1/opendrift/readers/reader_global_landmask.py
--rw-r--r--   0        0        0     8109 2021-03-05 15:37:49.627897 opendrift-1.9.1rc1/opendrift/readers/reader_grib.py
--rw-r--r--   0        0        0     5015 2021-09-14 13:39:37.970333 opendrift-1.9.1rc1/opendrift/readers/reader_grib2.py
--rw-r--r--   0        0        0     2420 2021-03-05 15:37:49.627897 opendrift-1.9.1rc1/opendrift/readers/reader_lazy.py
--rw-r--r--   0        0        0    22804 2022-07-16 14:09:51.724350 opendrift-1.9.1rc1/opendrift/readers/reader_netCDF_CF_generic.py
--rw-r--r--   0        0        0    15090 2021-10-15 06:08:42.877054 opendrift-1.9.1rc1/opendrift/readers/reader_netCDF_CF_unstructured.py
--rw-r--r--   0        0        0     1973 2021-03-05 15:37:49.627897 opendrift-1.9.1rc1/opendrift/readers/reader_oscillating.py
--rwxr-xr-x   0        0        0    52697 2022-01-03 08:32:44.613576 opendrift-1.9.1rc1/opendrift/readers/reader_schism_native.py
--rw-r--r--   0        0        0     4100 2021-10-15 06:08:42.877054 opendrift-1.9.1rc1/opendrift/readers/reader_shape.py
--rw-r--r--   0        0        0    12289 2022-01-03 08:32:44.613576 opendrift-1.9.1rc1/opendrift/readers/reader_telemac_selafin.py
--rw-r--r--   0        0        0     2474 2021-03-05 15:37:49.627897 opendrift-1.9.1rc1/opendrift/readers/reader_timeseries.py
--rw-r--r--   0        0        0        0 2020-02-04 12:59:28.886786 opendrift-1.9.1rc1/opendrift/readers/roppy/__init__.py
--rw-r--r--   0        0        0    10784 2021-03-05 15:37:49.627897 opendrift-1.9.1rc1/opendrift/readers/roppy/depth.py
--rw-r--r--   0        0        0     7678 2021-05-28 07:34:14.960298 opendrift-1.9.1rc1/opendrift/readers/unstructured/shyfem.py
--rw-r--r--   0        0        0     1522 2022-04-19 13:39:31.757022 opendrift-1.9.1rc1/opendrift/scripts/data_sources.txt
--rw-r--r--   0        0        0      565 2022-01-03 08:32:44.613576 opendrift-1.9.1rc1/opendrift/scripts/data_sources_historical.txt
--rwxr-xr-x   0        0        0     3845 2022-03-14 11:12:16.169241 opendrift-1.9.1rc1/opendrift/scripts/hodograph.py
--rwxr-xr-x   0        0        0      322 2021-03-05 15:37:49.627897 opendrift-1.9.1rc1/opendrift/scripts/mp4_to_gif.bash
--rwxr-xr-x   0        0        0     1875 2021-03-05 15:37:49.631897 opendrift-1.9.1rc1/opendrift/scripts/opendrift_animate.py
--rwxr-xr-x   0        0        0     1761 2021-03-05 15:37:49.631897 opendrift-1.9.1rc1/opendrift/scripts/opendrift_animate_profile.py
--rwxr-xr-x   0        0        0    34073 2022-03-14 11:12:16.169241 opendrift-1.9.1rc1/opendrift/scripts/opendrift_gui.py
--rwxr-xr-x   0        0        0     1351 2021-03-05 15:37:49.631897 opendrift-1.9.1rc1/opendrift/scripts/opendrift_plot.py
--rwxr-xr-x   0        0        0     4497 2021-05-28 07:34:14.960298 opendrift-1.9.1rc1/opendrift/scripts/readerinfo.py
--rw-r--r--   0        0        0      933 2021-03-05 15:37:49.631897 opendrift-1.9.1rc1/opendrift/timer.py
--rw-r--r--   0        0        0      606 2022-04-19 13:39:31.757022 opendrift-1.9.1rc1/opendrift/version.py
--rw-r--r--   0        0        0      998 2022-09-06 09:48:58.069565 opendrift-1.9.1rc1/pyproject.toml
--rw-r--r--   0        0        0     1900 2022-09-06 09:49:05.885599 opendrift-1.9.1rc1/setup.py
--rw-r--r--   0        0        0     1197 2022-09-06 09:49:05.886035 opendrift-1.9.1rc1/PKG-INFO
+-rw-r--r--   0        0        0    18092 2022-09-12 19:23:58.277039 opendrift-1.9.1rc2/LICENSE
+-rw-r--r--   0        0        0     7293 2022-09-12 19:23:58.285039 opendrift-1.9.1rc2/opendrift/__init__.py
+-rw-r--r--   0        0        0     1954 2022-09-12 19:23:58.285039 opendrift-1.9.1rc2/opendrift/elements/__init__.py
+-rw-r--r--   0        0        0    10641 2022-09-12 19:23:58.285039 opendrift-1.9.1rc2/opendrift/elements/elements.py
+-rw-r--r--   0        0        0     1030 2022-09-12 19:23:58.285039 opendrift-1.9.1rc2/opendrift/elements/passivetracer.py
+-rw-r--r--   0        0        0      226 2022-09-12 19:23:58.285039 opendrift-1.9.1rc2/opendrift/errors.py
+-rw-r--r--   0        0        0        0 2022-09-12 19:23:58.285039 opendrift-1.9.1rc2/opendrift/export/__init__.py
+-rw-r--r--   0        0        0    16786 2022-09-12 19:23:58.285039 opendrift-1.9.1rc2/opendrift/export/io_netcdf.py
+-rw-r--r--   0        0        0    16526 2022-09-12 19:23:58.285039 opendrift-1.9.1rc2/opendrift/models/OBJECTPROP.DAT
+-rw-r--r--   0        0        0       32 2022-09-12 19:23:58.285039 opendrift-1.9.1rc2/opendrift/models/__init__.py
+-rw-r--r--   0        0        0   240307 2022-09-12 19:23:58.289039 opendrift-1.9.1rc2/opendrift/models/basemodel.py
+-rw-r--r--   0        0        0   120412 2022-09-12 19:23:58.289039 opendrift-1.9.1rc2/opendrift/models/chemicaldrift.py
+-rw-r--r--   0        0        0      658 2022-09-12 19:23:58.289039 opendrift-1.9.1rc2/opendrift/models/eulerdrift/__init__.py
+-rw-r--r--   0        0        0      325 2022-09-12 19:23:58.289039 opendrift-1.9.1rc2/opendrift/models/eulerdrift/diff.py
+-rw-r--r--   0        0        0     3149 2022-09-12 19:23:58.289039 opendrift-1.9.1rc2/opendrift/models/eulerdrift/grid.py
+-rw-r--r--   0        0        0      343 2022-09-12 19:23:58.289039 opendrift-1.9.1rc2/opendrift/models/eulerdrift/interp.py
+-rw-r--r--   0        0        0     2396 2022-09-12 19:23:58.289039 opendrift-1.9.1rc2/opendrift/models/eulerdrift/readers.py
+-rw-r--r--   0        0        0     7655 2022-09-12 19:23:58.289039 opendrift-1.9.1rc2/opendrift/models/eulerdrift/simulation.py
+-rw-r--r--   0        0        0      948 2022-09-12 19:23:58.289039 opendrift-1.9.1rc2/opendrift/models/eulerdrift/srs.py
+-rw-r--r--   0        0        0    11394 2022-09-12 19:23:58.289039 opendrift-1.9.1rc2/opendrift/models/larvalfish.py
+-rw-r--r--   0        0        0    19700 2022-09-12 19:23:58.289039 opendrift-1.9.1rc2/opendrift/models/leeway.py
+-rw-r--r--   0        0        0    12134 2022-09-12 19:23:58.289039 opendrift-1.9.1rc2/opendrift/models/model_template.py
+-rw-r--r--   0        0        0    37666 2022-09-12 19:23:58.289039 opendrift-1.9.1rc2/opendrift/models/oceandrift.py
+-rw-r--r--   0        0        0    13406 2022-09-12 19:23:58.289039 opendrift-1.9.1rc2/opendrift/models/openberg.py
+-rw-r--r--   0        0        0       23 2022-09-12 19:23:58.289039 opendrift-1.9.1rc2/opendrift/models/openoil/__init__.py
+-rw-r--r--   0        0        0      371 2022-09-12 19:23:58.289039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/README.md
+-rw-r--r--   0        0        0      928 2022-09-12 19:23:58.289039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/__init__.py
+-rw-r--r--   0        0        0      256 2022-09-12 19:23:58.289039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/computation/__init__.py
+-rw-r--r--   0        0        0     7477 2022-09-12 19:23:58.289039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/computation/estimations.py
+-rw-r--r--   0        0        0    17896 2022-09-12 19:23:58.289039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/computation/gnome_oil.py
+-rw-r--r--   0        0        0    14868 2022-09-12 19:23:58.289039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/computation/physical_properties.py
+-rwxr-xr-x   0        0        0     1172 2022-09-12 19:23:58.289039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/csv_to_json.py
+-rw-r--r--   0        0        0     2840 2022-09-12 19:23:58.289039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/dirjs.py
+-rw-r--r--   0        0        0    12064 2022-09-12 19:23:58.289039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03128.json
+-rw-r--r--   0        0        0    12782 2022-09-12 19:23:58.289039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03129.json
+-rw-r--r--   0        0        0    14059 2022-09-12 19:23:58.289039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03130.json
+-rw-r--r--   0        0        0    11629 2022-09-12 19:23:58.289039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03131.json
+-rw-r--r--   0        0        0    11658 2022-09-12 19:23:58.289039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03132.json
+-rw-r--r--   0        0        0    11366 2022-09-12 19:23:58.289039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03133.json
+-rw-r--r--   0        0        0    10656 2022-09-12 19:23:58.289039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03134.json
+-rw-r--r--   0        0        0    11729 2022-09-12 19:23:58.289039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03135.json
+-rw-r--r--   0        0        0    12628 2022-09-12 19:23:58.289039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03136.json
+-rw-r--r--   0        0        0    12498 2022-09-12 19:23:58.289039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03137.json
+-rw-r--r--   0        0        0    12175 2022-09-12 19:23:58.289039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03138.json
+-rw-r--r--   0        0        0    11693 2022-09-12 19:23:58.289039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03139.json
+-rw-r--r--   0        0        0    11616 2022-09-12 19:23:58.289039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03140.json
+-rw-r--r--   0        0        0     9372 2022-09-12 19:23:58.289039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03141.json
+-rw-r--r--   0        0        0    11545 2022-09-12 19:23:58.289039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03142.json
+-rw-r--r--   0        0        0    11132 2022-09-12 19:23:58.289039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03143.json
+-rw-r--r--   0        0        0    12184 2022-09-12 19:23:58.289039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03144.json
+-rw-r--r--   0        0        0    11276 2022-09-12 19:23:58.289039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03145.json
+-rw-r--r--   0        0        0    11729 2022-09-12 19:23:58.289039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03146.json
+-rw-r--r--   0        0        0    12834 2022-09-12 19:23:58.289039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03147.json
+-rw-r--r--   0        0        0    15136 2022-09-12 19:23:58.289039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03148.json
+-rw-r--r--   0        0        0    13753 2022-09-12 19:23:58.289039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03149.json
+-rw-r--r--   0        0        0    16359 2022-09-12 19:23:58.289039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03150.json
+-rw-r--r--   0        0        0    14551 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03151.json
+-rw-r--r--   0        0        0    10815 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03152.json
+-rw-r--r--   0        0        0    10974 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03153.json
+-rw-r--r--   0        0        0    15843 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD04000.json
+-rw-r--r--   0        0        0    17688 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD04001.json
+-rw-r--r--   0        0        0    16375 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD04002.json
+-rw-r--r--   0        0        0     6987 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD04003.json
+-rw-r--r--   0        0        0     7748 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD04004.json
+-rw-r--r--   0        0        0    11360 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD04006.json
+-rw-r--r--   0        0        0    13012 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD04007.json
+-rw-r--r--   0        0        0    11363 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD04008.json
+-rw-r--r--   0        0        0    12614 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD04009.json
+-rw-r--r--   0        0        0    14255 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD04010.json
+-rw-r--r--   0        0        0    14094 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD04011.json
+-rw-r--r--   0        0        0    14088 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD04012.json
+-rw-r--r--   0        0        0    14094 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD04013.json
+-rw-r--r--   0        0        0     5106 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD04014.json
+-rw-r--r--   0        0        0        0 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/__init__.py
+-rwxr-xr-x   0        0        0       56 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/clean_lines.bash
+-rw-r--r--   0        0        0    14224 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/oillibnorway.csv
+-rw-r--r--   0        0        0    12953 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/oillibtest.csv
+-rw-r--r--   0        0        0    15737 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/templates/parse_oil_pdf.py
+-rw-r--r--   0        0        0     2377 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/harvest_oils.py
+-rw-r--r--   0        0        0        0 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/__init__.py
+-rw-r--r--   0        0        0      740 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/common/__init__.py
+-rw-r--r--   0        0        0      876 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/common/enum_types.py
+-rw-r--r--   0        0        0      350 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/common/label.py
+-rw-r--r--   0        0        0    12121 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/common/measurement.py
+-rw-r--r--   0        0        0     1972 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/common/sara.py
+-rw-r--r--   0        0        0      144 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/common/synonym.py
+-rw-r--r--   0        0        0     5957 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/common/utilities.py
+-rw-r--r--   0        0        0     3546 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/common/validators.py
+-rw-r--r--   0        0        0        0 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/__init__.py
+-rw-r--r--   0        0        0      567 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/bulk_composition.py
+-rw-r--r--   0        0        0      558 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/ccme.py
+-rw-r--r--   0        0        0      723 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/cleanup/__init__.py
+-rw-r--r--   0        0        0    14087 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/cleanup/add_labels.py
+-rw-r--r--   0        0        0      926 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/cleanup/cleanup.py
+-rw-r--r--   0        0        0     2805 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/cleanup/density.py
+-rw-r--r--   0        0        0     1825 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/cleanup/distillation.py
+-rw-r--r--   0        0        0     5946 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/completeness.py
+-rw-r--r--   0        0        0     1194 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/compound.py
+-rw-r--r--   0        0        0     3020 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/distillation.py
+-rw-r--r--   0        0        0      727 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/environmental_behavior.py
+-rw-r--r--   0        0        0      672 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/ests_fractions.py
+-rw-r--r--   0        0        0      698 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/industry_property.py
+-rw-r--r--   0        0        0     2014 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/location_coordinates.py
+-rw-r--r--   0        0        0     2193 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/metadata.py
+-rw-r--r--   0        0        0     5876 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/oil.py
+-rw-r--r--   0        0        0     4273 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/physical_properties.py
+-rw-r--r--   0        0        0     2661 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/product_type.py
+-rw-r--r--   0        0        0     2092 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/product_types_and_labels.csv
+-rw-r--r--   0        0        0     2391 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/properties.py
+-rw-r--r--   0        0        0     1109 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/review_status.py
+-rw-r--r--   0        0        0     3692 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/sample.py
+-rw-r--r--   0        0        0      502 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/sara.py
+-rw-r--r--   0        0        0        6 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/validation/__init__.py
+-rw-r--r--   0        0        0      943 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/validation/errors.py
+-rw-r--r--   0        0        0     1180 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/validation/validate.py
+-rw-r--r--   0        0        0      879 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/validation/warnings.py
+-rw-r--r--   0        0        0      726 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/values.py
+-rw-r--r--   0        0        0     1793 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/version.py
+-rw-r--r--   0        0        0     2640 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/version_update.py
+-rw-r--r--   0        0        0      741 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/versions.py
+-rw-r--r--   0        0        0     4676 2022-09-12 19:23:58.293039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/oil.py
+-rw-r--r--   0        0        0   442560 2022-09-12 19:23:58.297039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/oils.xz
+-rw-r--r--   0        0        0        0 2022-09-12 19:23:58.297039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/util/__init__.py
+-rw-r--r--   0        0        0    13382 2022-09-12 19:23:58.297039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/util/estimations.py
+-rw-r--r--   0        0        0     3507 2022-09-12 19:23:58.297039 opendrift-1.9.1rc2/opendrift/models/openoil/adios/util/many_many.py
+-rw-r--r--   0        0        0     1418 2022-09-12 19:23:58.297039 opendrift-1.9.1rc2/opendrift/models/openoil/noaa_oil_weathering.py
+-rw-r--r--   0        0        0    74753 2022-09-12 19:23:58.297039 opendrift-1.9.1rc2/opendrift/models/openoil/openoil.py
+-rw-r--r--   0        0        0     7525 2022-09-12 19:23:58.297039 opendrift-1.9.1rc2/opendrift/models/pelagicegg.py
+-rw-r--r--   0        0        0    40791 2022-09-12 19:23:58.297039 opendrift-1.9.1rc2/opendrift/models/physics_methods.py
+-rw-r--r--   0        0        0     4114 2022-09-12 19:23:58.297039 opendrift-1.9.1rc2/opendrift/models/plastdrift.py
+-rw-r--r--   0        0        0    73052 2022-09-12 19:23:58.297039 opendrift-1.9.1rc2/opendrift/models/radionuclides.py
+-rw-r--r--   0        0        0     1535 2022-09-12 19:23:58.297039 opendrift-1.9.1rc2/opendrift/models/seaicedrift.py
+-rw-r--r--   0        0        0    19003 2022-09-12 19:23:58.297039 opendrift-1.9.1rc2/opendrift/models/sealice.py
+-rw-r--r--   0        0        0     4382 2022-09-12 19:23:58.297039 opendrift-1.9.1rc2/opendrift/models/sedimentdrift.py
+-rw-r--r--   0        0        0    16188 2022-09-12 19:23:58.297039 opendrift-1.9.1rc2/opendrift/models/shipdrift.py
+-rw-r--r--   0        0        0     2786 2022-09-12 19:23:58.297039 opendrift-1.9.1rc2/opendrift/models/wforce.dat
+-rw-r--r--   0        0        0     1401 2022-09-12 19:23:58.297039 opendrift-1.9.1rc2/opendrift/models/windblow.py
+-rw-r--r--   0        0        0     2873 2022-09-12 19:23:58.297039 opendrift-1.9.1rc2/opendrift/readers/__init__.py
+-rw-r--r--   0        0        0    18608 2022-09-12 19:23:58.297039 opendrift-1.9.1rc2/opendrift/readers/basereader/__init__.py
+-rw-r--r--   0        0        0     1608 2022-09-12 19:23:58.297039 opendrift-1.9.1rc2/opendrift/readers/basereader/consts.py
+-rw-r--r--   0        0        0     1531 2022-09-12 19:23:58.297039 opendrift-1.9.1rc2/opendrift/readers/basereader/continuous.py
+-rw-r--r--   0        0        0      335 2022-09-12 19:23:58.297039 opendrift-1.9.1rc2/opendrift/readers/basereader/fakeproj.py
+-rw-r--r--   0        0        0    24363 2022-09-12 19:23:58.297039 opendrift-1.9.1rc2/opendrift/readers/basereader/structured.py
+-rw-r--r--   0        0        0     5699 2022-09-12 19:23:58.297039 opendrift-1.9.1rc2/opendrift/readers/basereader/unstructured.py
+-rw-r--r--   0        0        0    33873 2022-09-12 19:23:58.297039 opendrift-1.9.1rc2/opendrift/readers/basereader/variables.py
+-rw-r--r--   0        0        0       66 2022-09-12 19:23:58.297039 opendrift-1.9.1rc2/opendrift/readers/interpolation/__init__.py
+-rw-r--r--   0        0        0     7876 2022-09-12 19:23:58.297039 opendrift-1.9.1rc2/opendrift/readers/interpolation/interpolators.py
+-rw-r--r--   0        0        0     6500 2022-09-12 19:23:58.297039 opendrift-1.9.1rc2/opendrift/readers/interpolation/structured.py
+-rw-r--r--   0        0        0       77 2022-09-12 19:23:58.297039 opendrift-1.9.1rc2/opendrift/readers/operators/__init__.py
+-rw-r--r--   0        0        0      613 2022-09-12 19:23:58.297039 opendrift-1.9.1rc2/opendrift/readers/operators/filter.py
+-rw-r--r--   0        0        0     1775 2022-09-12 19:23:58.297039 opendrift-1.9.1rc2/opendrift/readers/operators/numops.py
+-rw-r--r--   0        0        0     1562 2022-09-12 19:23:58.297039 opendrift-1.9.1rc2/opendrift/readers/operators/ops.py
+-rw-r--r--   0        0        0     2015 2022-09-12 19:23:58.297039 opendrift-1.9.1rc2/opendrift/readers/operators/readerops.py
+-rw-r--r--   0        0        0     2722 2022-09-12 19:23:58.297039 opendrift-1.9.1rc2/opendrift/readers/reader_ArtificialOceanEddy.py
+-rw-r--r--   0        0        0    26777 2022-09-12 19:23:58.301039 opendrift-1.9.1rc2/opendrift/readers/reader_ROMS_native.py
+-rw-r--r--   0        0        0     1912 2022-09-12 19:23:58.301039 opendrift-1.9.1rc2/opendrift/readers/reader_constant.py
+-rw-r--r--   0        0        0     1675 2022-09-12 19:23:58.301039 opendrift-1.9.1rc2/opendrift/readers/reader_constant_2d.py
+-rw-r--r--   0        0        0     5362 2022-09-12 19:23:58.301039 opendrift-1.9.1rc2/opendrift/readers/reader_current_from_drifter.py
+-rw-r--r--   0        0        0     3659 2022-09-12 19:23:58.301039 opendrift-1.9.1rc2/opendrift/readers/reader_current_from_track.py
+-rw-r--r--   0        0        0     2696 2022-09-12 19:23:58.301039 opendrift-1.9.1rc2/opendrift/readers/reader_double_gyre.py
+-rw-r--r--   0        0        0     8823 2022-09-12 19:23:58.301039 opendrift-1.9.1rc2/opendrift/readers/reader_global_landmask.py
+-rw-r--r--   0        0        0     8109 2022-09-12 19:23:58.301039 opendrift-1.9.1rc2/opendrift/readers/reader_grib.py
+-rw-r--r--   0        0        0     5015 2022-09-12 19:23:58.301039 opendrift-1.9.1rc2/opendrift/readers/reader_grib2.py
+-rw-r--r--   0        0        0     2420 2022-09-12 19:23:58.301039 opendrift-1.9.1rc2/opendrift/readers/reader_lazy.py
+-rw-r--r--   0        0        0    22804 2022-09-12 19:23:58.301039 opendrift-1.9.1rc2/opendrift/readers/reader_netCDF_CF_generic.py
+-rw-r--r--   0        0        0    15090 2022-09-12 19:23:58.301039 opendrift-1.9.1rc2/opendrift/readers/reader_netCDF_CF_unstructured.py
+-rw-r--r--   0        0        0     1973 2022-09-12 19:23:58.301039 opendrift-1.9.1rc2/opendrift/readers/reader_oscillating.py
+-rwxr-xr-x   0        0        0    52697 2022-09-12 19:23:58.301039 opendrift-1.9.1rc2/opendrift/readers/reader_schism_native.py
+-rw-r--r--   0        0        0     4100 2022-09-12 19:23:58.301039 opendrift-1.9.1rc2/opendrift/readers/reader_shape.py
+-rw-r--r--   0        0        0    12289 2022-09-12 19:23:58.301039 opendrift-1.9.1rc2/opendrift/readers/reader_telemac_selafin.py
+-rw-r--r--   0        0        0     2474 2022-09-12 19:23:58.301039 opendrift-1.9.1rc2/opendrift/readers/reader_timeseries.py
+-rw-r--r--   0        0        0        0 2022-09-12 19:23:58.301039 opendrift-1.9.1rc2/opendrift/readers/roppy/__init__.py
+-rw-r--r--   0        0        0    10784 2022-09-12 19:23:58.301039 opendrift-1.9.1rc2/opendrift/readers/roppy/depth.py
+-rw-r--r--   0        0        0     7678 2022-09-12 19:23:58.301039 opendrift-1.9.1rc2/opendrift/readers/unstructured/shyfem.py
+-rw-r--r--   0        0        0     1522 2022-09-12 19:23:58.301039 opendrift-1.9.1rc2/opendrift/scripts/data_sources.txt
+-rw-r--r--   0        0        0      565 2022-09-12 19:23:58.301039 opendrift-1.9.1rc2/opendrift/scripts/data_sources_historical.txt
+-rwxr-xr-x   0        0        0     3831 2022-09-12 19:23:58.301039 opendrift-1.9.1rc2/opendrift/scripts/hodograph.py
+-rwxr-xr-x   0        0        0      322 2022-09-12 19:23:58.301039 opendrift-1.9.1rc2/opendrift/scripts/mp4_to_gif.bash
+-rwxr-xr-x   0        0        0     1898 2022-09-12 19:23:58.301039 opendrift-1.9.1rc2/opendrift/scripts/opendrift_animate.py
+-rwxr-xr-x   0        0        0     1761 2022-09-12 19:23:58.301039 opendrift-1.9.1rc2/opendrift/scripts/opendrift_animate_profile.py
+-rwxr-xr-x   0        0        0    34018 2022-09-12 19:23:58.301039 opendrift-1.9.1rc2/opendrift/scripts/opendrift_gui.py
+-rwxr-xr-x   0        0        0     1371 2022-09-12 19:23:58.301039 opendrift-1.9.1rc2/opendrift/scripts/opendrift_plot.py
+-rwxr-xr-x   0        0        0     4522 2022-09-12 19:23:58.301039 opendrift-1.9.1rc2/opendrift/scripts/readerinfo.py
+-rw-r--r--   0        0        0      933 2022-09-12 19:23:58.301039 opendrift-1.9.1rc2/opendrift/timer.py
+-rw-r--r--   0        0        0      609 2022-09-12 19:23:58.301039 opendrift-1.9.1rc2/opendrift/version.py
+-rw-r--r--   0        0        0     2464 2022-09-12 19:23:58.301039 opendrift-1.9.1rc2/pyproject.toml
+-rw-r--r--   0        0        0     2365 1970-01-01 00:00:00.000000 opendrift-1.9.1rc2/setup.py
+-rw-r--r--   0        0        0     1260 1970-01-01 00:00:00.000000 opendrift-1.9.1rc2/PKG-INFO
```

### Comparing `opendrift-1.9.1rc1/LICENSE` & `opendrift-1.9.1rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/__init__.py` & `opendrift-1.9.1rc2/opendrift/__init__.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/elements/__init__.py` & `opendrift-1.9.1rc2/opendrift/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/elements/elements.py` & `opendrift-1.9.1rc2/opendrift/elements/elements.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/elements/passivetracer.py` & `opendrift-1.9.1rc2/opendrift/elements/passivetracer.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/export/io_netcdf.py` & `opendrift-1.9.1rc2/opendrift/export/io_netcdf.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/OBJECTPROP.DAT` & `opendrift-1.9.1rc2/opendrift/models/OBJECTPROP.DAT`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/basemodel.py` & `opendrift-1.9.1rc2/opendrift/models/basemodel.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/chemicaldrift.py` & `opendrift-1.9.1rc2/opendrift/models/chemicaldrift.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/eulerdrift/__init__.py` & `opendrift-1.9.1rc2/opendrift/models/eulerdrift/__init__.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/eulerdrift/grid.py` & `opendrift-1.9.1rc2/opendrift/models/eulerdrift/grid.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/eulerdrift/readers.py` & `opendrift-1.9.1rc2/opendrift/models/eulerdrift/readers.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/eulerdrift/simulation.py` & `opendrift-1.9.1rc2/opendrift/models/eulerdrift/simulation.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/eulerdrift/srs.py` & `opendrift-1.9.1rc2/opendrift/models/eulerdrift/srs.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/larvalfish.py` & `opendrift-1.9.1rc2/opendrift/models/larvalfish.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/leeway.py` & `opendrift-1.9.1rc2/opendrift/models/leeway.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/model_template.py` & `opendrift-1.9.1rc2/opendrift/models/model_template.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/oceandrift.py` & `opendrift-1.9.1rc2/opendrift/models/oceandrift.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openberg.py` & `opendrift-1.9.1rc2/opendrift/models/openberg.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/__init__.py` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/__init__.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/computation/estimations.py` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/computation/estimations.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/computation/gnome_oil.py` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/computation/gnome_oil.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/computation/physical_properties.py` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/computation/physical_properties.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/csv_to_json.py` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/csv_to_json.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/dirjs.py` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/dirjs.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03128.json` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03128.json`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03129.json` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03129.json`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03130.json` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03130.json`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03131.json` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03131.json`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03132.json` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03132.json`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03133.json` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03133.json`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03134.json` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03134.json`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03135.json` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03135.json`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03136.json` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03136.json`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03137.json` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03137.json`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03138.json` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03138.json`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03139.json` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03139.json`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03140.json` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03140.json`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03141.json` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03141.json`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03142.json` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03142.json`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03143.json` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03143.json`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03144.json` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03144.json`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03145.json` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03145.json`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03146.json` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03146.json`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03147.json` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03147.json`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03148.json` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03148.json`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03149.json` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03149.json`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03150.json` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03150.json`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03151.json` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03151.json`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03152.json` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03152.json`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD03153.json` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD03153.json`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD04000.json` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD04000.json`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD04001.json` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD04001.json`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD04002.json` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD04002.json`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD04003.json` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD04003.json`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD04004.json` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD04004.json`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD04006.json` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD04006.json`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD04007.json` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD04007.json`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD04008.json` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD04008.json`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD04009.json` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD04009.json`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD04010.json` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD04010.json`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD04011.json` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD04011.json`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD04012.json` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD04012.json`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD04013.json` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD04013.json`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/AD04014.json` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/AD04014.json`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/oillibnorway.csv` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/oillibnorway.csv`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/oillibtest.csv` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/oillibtest.csv`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/extra_oils/templates/parse_oil_pdf.py` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/extra_oils/templates/parse_oil_pdf.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/harvest_oils.py` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/harvest_oils.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/common/__init__.py` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/common/__init__.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/common/enum_types.py` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/common/enum_types.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/common/measurement.py` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/common/measurement.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/common/sara.py` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/common/sara.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/common/utilities.py` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/common/utilities.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/common/validators.py` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/common/validators.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/bulk_composition.py` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/bulk_composition.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/ccme.py` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/ccme.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/cleanup/__init__.py` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/cleanup/__init__.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/cleanup/add_labels.py` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/cleanup/add_labels.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/cleanup/cleanup.py` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/cleanup/cleanup.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/cleanup/density.py` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/cleanup/density.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/cleanup/distillation.py` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/cleanup/distillation.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/completeness.py` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/completeness.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/compound.py` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/compound.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/distillation.py` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/distillation.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/environmental_behavior.py` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/environmental_behavior.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/ests_fractions.py` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/ests_fractions.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/industry_property.py` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/industry_property.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/location_coordinates.py` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/location_coordinates.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/metadata.py` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/metadata.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/oil.py` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/oil.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/physical_properties.py` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/physical_properties.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/product_type.py` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/product_type.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/product_types_and_labels.csv` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/product_types_and_labels.csv`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/properties.py` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/properties.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/review_status.py` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/review_status.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/sample.py` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/sample.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/validation/errors.py` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/validation/errors.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/validation/validate.py` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/validation/validate.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/validation/warnings.py` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/validation/warnings.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/values.py` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/values.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/version.py` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/version.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/version_update.py` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/version_update.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/models/oil/versions.py` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/models/oil/versions.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/oil.py` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/oil.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/oils.xz` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/oils.xz`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/util/estimations.py` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/util/estimations.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/adios/util/many_many.py` & `opendrift-1.9.1rc2/opendrift/models/openoil/adios/util/many_many.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/noaa_oil_weathering.py` & `opendrift-1.9.1rc2/opendrift/models/openoil/noaa_oil_weathering.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/openoil/openoil.py` & `opendrift-1.9.1rc2/opendrift/models/openoil/openoil.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/pelagicegg.py` & `opendrift-1.9.1rc2/opendrift/models/pelagicegg.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/physics_methods.py` & `opendrift-1.9.1rc2/opendrift/models/physics_methods.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/plastdrift.py` & `opendrift-1.9.1rc2/opendrift/models/plastdrift.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/radionuclides.py` & `opendrift-1.9.1rc2/opendrift/models/radionuclides.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/seaicedrift.py` & `opendrift-1.9.1rc2/opendrift/models/seaicedrift.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/sealice.py` & `opendrift-1.9.1rc2/opendrift/models/sealice.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/sedimentdrift.py` & `opendrift-1.9.1rc2/opendrift/models/sedimentdrift.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/shipdrift.py` & `opendrift-1.9.1rc2/opendrift/models/shipdrift.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/wforce.dat` & `opendrift-1.9.1rc2/opendrift/models/wforce.dat`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/models/windblow.py` & `opendrift-1.9.1rc2/opendrift/models/windblow.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/readers/__init__.py` & `opendrift-1.9.1rc2/opendrift/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/readers/basereader/__init__.py` & `opendrift-1.9.1rc2/opendrift/readers/basereader/__init__.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/readers/basereader/consts.py` & `opendrift-1.9.1rc2/opendrift/readers/basereader/consts.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/readers/basereader/continuous.py` & `opendrift-1.9.1rc2/opendrift/readers/basereader/continuous.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/readers/basereader/structured.py` & `opendrift-1.9.1rc2/opendrift/readers/basereader/structured.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/readers/basereader/unstructured.py` & `opendrift-1.9.1rc2/opendrift/readers/basereader/unstructured.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/readers/basereader/variables.py` & `opendrift-1.9.1rc2/opendrift/readers/basereader/variables.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/readers/interpolation/interpolators.py` & `opendrift-1.9.1rc2/opendrift/readers/interpolation/interpolators.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/readers/interpolation/structured.py` & `opendrift-1.9.1rc2/opendrift/readers/interpolation/structured.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/readers/operators/filter.py` & `opendrift-1.9.1rc2/opendrift/readers/operators/filter.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/readers/operators/numops.py` & `opendrift-1.9.1rc2/opendrift/readers/operators/numops.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/readers/operators/ops.py` & `opendrift-1.9.1rc2/opendrift/readers/operators/ops.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/readers/operators/readerops.py` & `opendrift-1.9.1rc2/opendrift/readers/operators/readerops.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/readers/reader_ArtificialOceanEddy.py` & `opendrift-1.9.1rc2/opendrift/readers/reader_ArtificialOceanEddy.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/readers/reader_ROMS_native.py` & `opendrift-1.9.1rc2/opendrift/readers/reader_ROMS_native.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/readers/reader_constant.py` & `opendrift-1.9.1rc2/opendrift/readers/reader_constant.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/readers/reader_constant_2d.py` & `opendrift-1.9.1rc2/opendrift/readers/reader_constant_2d.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/readers/reader_current_from_drifter.py` & `opendrift-1.9.1rc2/opendrift/readers/reader_current_from_drifter.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/readers/reader_current_from_track.py` & `opendrift-1.9.1rc2/opendrift/readers/reader_current_from_track.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/readers/reader_double_gyre.py` & `opendrift-1.9.1rc2/opendrift/readers/reader_double_gyre.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/readers/reader_global_landmask.py` & `opendrift-1.9.1rc2/opendrift/readers/reader_global_landmask.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/readers/reader_grib.py` & `opendrift-1.9.1rc2/opendrift/readers/reader_grib.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/readers/reader_grib2.py` & `opendrift-1.9.1rc2/opendrift/readers/reader_grib2.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/readers/reader_lazy.py` & `opendrift-1.9.1rc2/opendrift/readers/reader_lazy.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/readers/reader_netCDF_CF_generic.py` & `opendrift-1.9.1rc2/opendrift/readers/reader_netCDF_CF_generic.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/readers/reader_netCDF_CF_unstructured.py` & `opendrift-1.9.1rc2/opendrift/readers/reader_netCDF_CF_unstructured.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/readers/reader_oscillating.py` & `opendrift-1.9.1rc2/opendrift/readers/reader_oscillating.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/readers/reader_schism_native.py` & `opendrift-1.9.1rc2/opendrift/readers/reader_schism_native.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/readers/reader_shape.py` & `opendrift-1.9.1rc2/opendrift/readers/reader_shape.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/readers/reader_telemac_selafin.py` & `opendrift-1.9.1rc2/opendrift/readers/reader_telemac_selafin.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/readers/reader_timeseries.py` & `opendrift-1.9.1rc2/opendrift/readers/reader_timeseries.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/readers/roppy/depth.py` & `opendrift-1.9.1rc2/opendrift/readers/roppy/depth.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/readers/unstructured/shyfem.py` & `opendrift-1.9.1rc2/opendrift/readers/unstructured/shyfem.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/scripts/data_sources.txt` & `opendrift-1.9.1rc2/opendrift/scripts/data_sources.txt`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/scripts/data_sources_historical.txt` & `opendrift-1.9.1rc2/opendrift/scripts/data_sources_historical.txt`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/scripts/hodograph.py` & `opendrift-1.9.1rc2/opendrift/scripts/hodograph.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 #!/usr/bin/env python
 #
 # This file is part of OpenDrift.
-# 
+#
 # OpenDrift is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, version 2
-# 
+#
 # OpenDrift is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
-# 
+#
 # You should have received a copy of the GNU General Public License
 # along with OpenDrift.  If not, see <https://www.gnu.org/licenses/>.
-# 
+#
 # Copyright 2015, Knut-Frode Dagestad, MET Norway
 
 
 # Utility script to display contents of a netCDF CF-compliant
 # file or URL containing driver data suitable for opendrift
 #
 # Knut-Frode Dagestad, 19 Feb 2015
@@ -35,15 +35,15 @@
     from opendrift.readers import reader_netCDF_CF_generic
     from opendrift.readers import reader_ROMS_native
     readers = [reader_netCDF_CF_generic, reader_ROMS_native]
 except ImportError: # development
     sys.exit('Please add opendrift folder to your PYTHONPATH.')
 
 
-if __name__ == '__main__':
+def main():
     parser = argparse.ArgumentParser()
     parser.add_argument('filename',
                         help='<URL or netCDF filename>')
     parser.add_argument('lon', help='longitude in degrees')
     parser.add_argument('lat', help='longitude in degrees')
     parser.add_argument('time', help='YYYYMMDDHHMM')
     parser.add_argument('-e', action='store_true',
@@ -61,29 +61,29 @@
             if args.e is True:
                 print(me)
                 import traceback
                 print(traceback.format_exc())
                 print('---------------------------------------')
             print('...not applicable.')
 
-    if not 'r' in locals():            
+    if not 'r' in locals():
         sys.exit('No readers applicable for ' + args.filename)
 
     time = datetime.strptime(args.time, '%Y%m%d%H%M')
     lon = np.atleast_1d(args.lon)
     lat = np.atleast_1d(args.lat)
 
     x, y = r.lonlat2xy(lon, lat)
     r.buffer = 3
     i=3; j=3  # center of block
 
     uv = r.get_variables(['x_sea_water_velocity', 'y_sea_water_velocity',
                          'sea_floor_depth_below_sea_level'],
                          time, x, y, r.z)
-                       
+
     u_comp = uv['x_sea_water_velocity'][:,i,j]
     v_comp = uv['y_sea_water_velocity'][:,i,j]
     depth = uv['sea_floor_depth_below_sea_level'][i,j]
     u_comp = u_comp[0:sum(~u_comp.mask)]
     v_comp = v_comp[0:sum(~v_comp.mask)]
 
     u_rot, v_rot = r.rotate_vectors(x, y, u_comp, v_comp,
@@ -103,7 +103,11 @@
     plt.xlabel('East component [m/s]')
     textstr = u'%s UTC\n%.3fN\N{DEGREE SIGN}, %.3fE\N{DEGREE SIGN}' % \
              (time, float(args.lat), float(args.lon))
     ax.text(0.05, 0.95, textstr, transform=ax.transAxes, fontsize=14,
             verticalalignment='top',
             bbox=dict(boxstyle='round', facecolor='wheat', alpha=0.5))
     plt.show()
+
+if __name__ == '__main__':
+    main()
+
```

### Comparing `opendrift-1.9.1rc1/opendrift/scripts/opendrift_animate.py` & `opendrift-1.9.1rc2/opendrift/scripts/opendrift_animate.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # 
 # Copyright 2015, Knut-Frode Dagestad, MET Norway
 
 import argparse
 import numpy as np
 import opendrift
 
-if __name__ == '__main__':
+def main():
     parser = argparse.ArgumentParser()
     parser.add_argument('filename1',
                         help='<OpenDrift filename (netCDF) of first file>')
     parser.add_argument(dest='filename2', nargs='?',
                         help='<OpenDrift filename (netCDF) of second file>')
     parser.add_argument('-b', dest='buffer',
                         default=1.0,
@@ -45,7 +45,10 @@
     else:
         o2 = opendrift.open(args.filename2)
         print(o2)
 
         # Animate and compare the two runs
         o1.animation(compare=o2, legend=[args.filename1, args.filename2],
                      filename=args.outfile, color=args.color)
+
+if __name__ == '__main__':
+   main()
```

### Comparing `opendrift-1.9.1rc1/opendrift/scripts/opendrift_animate_profile.py` & `opendrift-1.9.1rc2/opendrift/scripts/opendrift_animate_profile.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/scripts/opendrift_gui.py` & `opendrift-1.9.1rc2/opendrift/scripts/opendrift_gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -367,15 +367,15 @@
                                      '../../docs/opendrift_logo.png'))
             panel = tk.Label(self.seed, image=img)
             panel.image = img
             panel.grid(row=0, column=0)
         except Exception as e:
             print(e)
             pass # Could not display logo
- 
+
         ##########
         # RUN
         ##########
         tk.Button(self.seed, text=startbutton, bg='green',
                   command=self.run_opendrift).grid(row=80, column=1,
                                               sticky=tk.W, pady=4)
 
@@ -440,16 +440,16 @@
                 )
         elif command == 'saveconcfile':
             self.o.guipp_saveconcfile(filename=homefolder+'/conc_radio.nc')
         elif command == 'plotconc':
             zlayer = [-1]
             time   = None
             specie = ['LMM']
-            self.o.guipp_plotandsaveconc(filename=homefolder+'/conc_radio.nc', 
-                                         outfilename=homefolder+'/radio_plots/RadioConc', 
+            self.o.guipp_plotandsaveconc(filename=homefolder+'/conc_radio.nc',
+                                         outfilename=homefolder+'/radio_plots/RadioConc',
                                          zlayers=zlayer, time=time, specie=specie )
         elif command == 'showanimationprofile':
             self.o.guipp_showanimationprofile()
 
 
 
     def validate_config(self, value_if_allowed, prior_value, key):
@@ -472,15 +472,15 @@
             print('Setting: %s -> %s', (key, value_if_allowed))
             self.o.set_config(key, value_if_allowed)
             return True
         except:
             return False
 
     def set_model(self, model, rebuild_gui=True):
-        
+
         # Creating simulation object (self.o) of chosen model class
         print('Setting model: ' + model)
         if model in self.extra_args:
             extra_args = self.extra_args[model]
         else:
             extra_args = {}
         self.o = self.opendrift_models[model](**extra_args)
@@ -585,15 +585,15 @@
             varlabel = i.split(':')[-1]
             if i in self.o.ElementType.variables.keys():
                 if 'units' in self.o.ElementType.variables[i].keys():
                     units = self.o.ElementType.variables[i]['units']
                     if units == '1':
                         units = 'fraction'
                     varlabel = '%s [%s]' % (varlabel, units)
-        
+
             self.seed_input_label[i] = tk.Label(self.seed_frame,
                                                 text=varlabel + '\t')
             self.seed_input_label[i].grid(row=num, column=0)
             CreateToolTip(self.seed_input_label[i], text=sc[i]['description'])
             actual_val = self.o.get_config(i)
             if sc[i]['type'] == 'enum':
                 self.seed_input_var[i] = tk.StringVar()
@@ -685,15 +685,15 @@
     def run_opendrift(self):
         sys.stdout.write('running OpenDrift')
 
         # Creating fresh instance of the current model, but keeping config
         adjusted_config = self.o._config
         self.set_model(self.modelname, rebuild_gui=False)
         self.o._config = adjusted_config
-    
+
         try:
             self.budgetbutton.destroy()
         except Exception as e:
             print(e)
             pass
         month = int(self.months.index(self.monthvar.get()) + 1)
         start_time = datetime(int(self.yearvar.get()), month,
@@ -754,23 +754,23 @@
 
         self.simulationname = 'opendrift_' + self.model.get() + \
             self.o.start_time.strftime('_%Y%m%d_%H%M')
 
         # Starting simulation run
         self.o.run(steps=duration, **extra_args)
         print(self.o)
-        
+
         try:
             os.chmod(extra_args['outfile'], 0o666)
         except:
             pass
-        
+
         # Model-specific post processing
         self.o.gui_postproc()
-        
+
 
         self.results.destroy()
         self.results = tk.Frame(self.seed, bd=2,
                                relief=tk.FLAT, padx=5, pady=0)
         self.results.grid(row=70, column=3, columnspan=1, sticky='ew')
         tk.Button(self.results, text='Show animation',
                   command=lambda: self.handle_result(
@@ -788,41 +788,44 @@
             tk.Button(self.results, text='Save oil budget',
                       command=lambda: self.handle_result(
                         'saveoilbudget')).grid(row=50, column=1)
             tk.Button(self.results, text='Show oil budget',
                       command=lambda: self.handle_result(
                         'showoilbudget')).grid(row=60, column=1)
 
-        
+
         if self.model.get() =='RadionuclideDrift':
             tk.Button(self.results, text='Show animation specie',
                       command=lambda: self.handle_result(
-                          'showanimationspecie')).grid(row=30, column=2) 
+                          'showanimationspecie')).grid(row=30, column=2)
             tk.Button(self.results, text='Save animation specie',
                       command=lambda: self.handle_result(
-                          'saveanimationspecie')).grid(row=40, column=2) 
+                          'saveanimationspecie')).grid(row=40, column=2)
             tk.Button(self.results, text='Animation profile',
                       command=lambda: self.handle_result(
-                          'showanimationprofile')).grid(row=10, column=2) 
+                          'showanimationprofile')).grid(row=10, column=2)
 #             tk.Button(self.results, text='Save conc file',
 #                       command=lambda: self.handle_result(
-#                           'saveconcfile')).grid(row=20, column=2) 
+#                           'saveconcfile')).grid(row=20, column=2)
             tk.Button(self.results, text='Plot conc',
                       command=lambda: self.handle_result(
-                          'plotconc')).grid(row=20, column=2) 
+                          'plotconc')).grid(row=20, column=2)
+
+
 
-        
-        
         if self.has_diana is True:
             diana_filename = self.dianadir + self.simulationname + '.nc'
             self.o.write_netcdf_density_map(diana_filename)
             tk.Button(self.results, text='Show in Diana',
                       command=lambda: os.system('diana &')
                       ).grid(row=80, column=1)
-                      
+
             try:
                 os.chmod(diana_filename, 0o666)
             except:
                 pass
 
+def main():
+    OpenDriftGUI().mainloop()
+
 if __name__ == '__main__':
     OpenDriftGUI().mainloop()
```

### Comparing `opendrift-1.9.1rc1/opendrift/scripts/opendrift_plot.py` & `opendrift-1.9.1rc2/opendrift/scripts/opendrift_plot.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 #!/usr/bin/env python
 #
 # This file is part of OpenDrift.
-# 
+#
 # OpenDrift is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, version 2
-# 
+#
 # OpenDrift is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
-# 
+#
 # You should have received a copy of the GNU General Public License
 # along with OpenDrift.  If not, see <https://www.gnu.org/licenses/>.
-# 
+#
 # Copyright 2015, Knut-Frode Dagestad, MET Norway
 
 import sys
 import argparse
 import numpy as np
 sys.path.append("..")
 
 import opendrift
 
-if __name__ == '__main__':
+def main():
     parser = argparse.ArgumentParser()
     parser.add_argument('filename',
                         help='<OpenDrift output filename (netCDF)>')
     parser.add_argument('-b', dest='buffer',
                         default=0.1,
                         help='Buffer around plot in degrees lon/lat.')
     parser.add_argument('-f', dest='outfile',
@@ -35,7 +35,10 @@
 
     args = parser.parse_args()
 
 
     o = opendrift.open(args.filename)
     print(o)
     o.plot(buffer=float(args.buffer), filename=args.outfile)
+
+if __name__ == '__main__':
+    main()
```

### Comparing `opendrift-1.9.1rc1/opendrift/scripts/readerinfo.py` & `opendrift-1.9.1rc2/opendrift/scripts/readerinfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     except:
         pass
 
 except ImportError: # development
     sys.exit('Please add opendrift folder to your PYTHONPATH.')
 
 
-if __name__ == '__main__':
+def main():
     parser = argparse.ArgumentParser()
     parser.add_argument('filename',
                         help='<URL or netCDF filename>')
     parser.add_argument('-p', dest='variable',
                         default='noplot', nargs='?',
                         help='Plot domain (or variable if given)')
     parser.add_argument('-vmin', dest='vmin',
@@ -117,7 +117,11 @@
                 vmin = float(args.vmin)
             if args.vmax is None:
                 vmax = None
             else:
                 vmax = float(args.vmax)
 
             r.plot(args.variable, vmin=vmin, vmax=vmax)
+
+if __name__ == '__main__':
+    main()
+
```

### Comparing `opendrift-1.9.1rc1/opendrift/timer.py` & `opendrift-1.9.1rc2/opendrift/timer.py`

 * *Files identical despite different names*

### Comparing `opendrift-1.9.1rc1/opendrift/version.py` & `opendrift-1.9.1rc2/opendrift/version.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.9.0"
+__version__ = "1.9.1rc2"
 
 
 def git_describe():
     """
     Return git version if available.
     """
     import os.path
```

### Comparing `opendrift-1.9.1rc1/setup.py` & `opendrift-1.9.1rc2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -34,37 +34,47 @@
  'cmocean>=2.0,<3.0',
  'coloredlogs>=15.0.1,<16.0.0',
  'geojson>=2.5.0,<3.0.0',
  'matplotlib>=3.5',
  'nc-time-axis>=1.4.1,<2.0.0',
  'netCDF4>=1.6',
  'numpy>=1.23',
+ 'pykdtree>=1.3.5,<2.0.0',
  'pynucos>=3',
  'pyproj>=2.3',
  'requests>=2.28.1,<3.0.0',
  'roaring-landmask>=0.5.1',
  'scipy>=1.9',
  'utm>=0.7.0,<0.8.0',
  'xarray>=2022.6.0']
 
 extras_require = \
 {'grib': ['cfgrib>=0.9.10,<0.10.0', 'pygrib>=2.1.4,<3.0.0']}
 
+entry_points = \
+{'console_scripts': ['hodograph = opendrift.scripts.hodograph:main',
+                     'opendrift_animate = '
+                     'opendrift.scripts.opendrift_animate:main',
+                     'opendrift_gui = opendrift.scripts.opendrift_gui:main',
+                     'opendrift_plot = opendrift.scripts.opendrift_plot:main',
+                     'readerinfo = opendrift.scripts.readerinfo:main']}
+
 setup_kwargs = {
     'name': 'opendrift',
-    'version': '1.9.1rc1',
+    'version': '1.9.1rc2',
     'description': 'OpenDrift - a framework for ocean trajectory modeling',
-    'long_description': None,
+    'long_description': 'None',
     'author': 'Knut-Frode Dagestad',
-    'author_email': 'knutfd@met.no>, Gaute Hope <gauteh@met.no',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
+    'author_email': 'knutfd@met.no',
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
-    'python_requires': '>=3.9,<3.12',
+    'entry_points': entry_points,
+    'python_requires': '>=3.8,<3.11',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `opendrift-1.9.1rc1/PKG-INFO` & `opendrift-1.9.1rc2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: opendrift
-Version: 1.9.1rc1
+Version: 1.9.1rc2
 Summary: OpenDrift - a framework for ocean trajectory modeling
 License: GPLv2
 Author: Knut-Frode Dagestad
-Author-email: knutfd@met.no>, Gaute Hope <gauteh@met.no
-Requires-Python: >=3.9,<3.12
+Author-email: knutfd@met.no
+Requires-Python: >=3.8,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: grib
 Requires-Dist: Cartopy (>=0.20)
-Requires-Dist: GDAL (>=3.5.1,<4.0.0)
+Requires-Dist: GDAL (>=3.3.1,<4.0.0)
 Requires-Dist: cfgrib (>=0.9.10,<0.10.0); extra == "grib"
 Requires-Dist: cmocean (>=2.0,<3.0)
 Requires-Dist: coloredlogs (>=15.0.1,<16.0.0)
 Requires-Dist: dask (>=2022.9.0,<2023.0.0)
 Requires-Dist: geojson (>=2.5.0,<3.0.0)
 Requires-Dist: matplotlib (>=3.5)
 Requires-Dist: nc-time-axis (>=1.4.1,<2.0.0)
 Requires-Dist: netCDF4 (>=1.6)
 Requires-Dist: numpy (>=1.23)
 Requires-Dist: pygrib (>=2.1.4,<3.0.0); extra == "grib"
+Requires-Dist: pykdtree (>=1.3.5,<2.0.0)
 Requires-Dist: pynucos (>=3)
 Requires-Dist: pyproj (>=2.3)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: roaring-landmask (>=0.5.1)
 Requires-Dist: scipy (>=1.9)
 Requires-Dist: utm (>=0.7.0,<0.8.0)
 Requires-Dist: xarray (>=2022.6.0)
```

