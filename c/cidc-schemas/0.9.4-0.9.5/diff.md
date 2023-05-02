# Comparing `tmp/cidc_schemas-0.9.4.tar.gz` & `tmp/cidc_schemas-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cidc_schemas-0.9.4.tar", last modified: Fri Nov  1 13:52:42 2019, max compression
+gzip compressed data, was "dist/cidc_schemas-0.9.5.tar", last modified: Mon Nov  4 20:30:16 2019, max compression
```

## Comparing `cidc_schemas-0.9.4.tar` & `cidc_schemas-0.9.5.tar`

### file list

```diff
@@ -1,147 +1,149 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-01 13:52:42.000000 cidc_schemas-0.9.4/
--rw-rw-r--   0 travis    (2000) travis    (2000)      314 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)      253 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     3577 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/CONTRIBUTING.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      617 2019-11-01 13:52:42.000000 cidc_schemas-0.9.4/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      165 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/AUTHORS.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-01 13:52:42.000000 cidc_schemas-0.9.4/cidc_schemas.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)      617 2019-11-01 13:52:42.000000 cidc_schemas-0.9.4/cidc_schemas.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-11-01 13:52:42.000000 cidc_schemas-0.9.4/cidc_schemas.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       13 2019-11-01 13:52:42.000000 cidc_schemas-0.9.4/cidc_schemas.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-11-01 13:52:42.000000 cidc_schemas-0.9.4/cidc_schemas.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)     5185 2019-11-01 13:52:42.000000 cidc_schemas-0.9.4/cidc_schemas.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      254 2019-11-01 13:52:42.000000 cidc_schemas-0.9.4/cidc_schemas.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       56 2019-11-01 13:52:42.000000 cidc_schemas-0.9.4/cidc_schemas.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     8991 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      395 2019-11-01 13:52:42.000000 cidc_schemas-0.9.4/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)       89 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/HISTORY.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1072 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/LICENSE
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-01 13:52:42.000000 cidc_schemas-0.9.4/cidc_schemas/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4773 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/util.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11521 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/template.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10892 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/template_reader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10395 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/template_writer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34223 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/prism.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      380 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/constants.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4835 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/cli.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      880 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/unprism.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15077 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/json_validation.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      162 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-01 13:52:42.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3349 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/shipping_core.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-01 13:52:42.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/assays/
--rw-rw-r--   0 travis    (2000) travis    (2000)      753 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/assays/micsss_assay.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-01 13:52:42.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/
--rw-rw-r--   0 travis    (2000) travis    (2000)      642 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/composite_image.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-01 13:52:42.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/cytof/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1408 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/cytof/cytof_analysis.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     3275 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/cytof/cytof_entry.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      457 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/cytof/cytof_input.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1051 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/cytof/cytof_antibody.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      790 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/fastq_pair_and_mapping.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      368 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/local_file.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1321 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/ngs_assay_core.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1600 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/image.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      965 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/imaging_data.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1469 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/mif_antibody.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      726 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/ihc_antibodies.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1201 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/mapping.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-01 13:52:42.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/imaging/
--rw-rw-r--   0 travis    (2000) travis    (2000)      792 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/imaging/micsss_input.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1099 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/imaging/mif_input.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      618 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/imaging/mif_entry.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      663 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/imaging/micsss_entry.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     2513 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/imaging/ihc_entry.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      664 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/imaging/ihc_input.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      441 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/assay_core.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-01 13:52:42.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/olink/
--rw-rw-r--   0 travis    (2000) travis    (2000)      613 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/olink/olink_combined.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1918 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/olink/olink_entry.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      592 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/olink/olink_input.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      343 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/germline.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     2925 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/micsss_antibody.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      526 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/alignment.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      423 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/somatic.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-01 13:52:42.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/ngs/
--rw-rw-r--   0 travis    (2000) travis    (2000)      638 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/ngs/wes_assay_record.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      569 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/ngs/wes_output.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      262 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/ngs/rna_input.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      863 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/ngs/rna_expression_entry.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1475 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/ngs/ngs_assay_record.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      583 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/ngs/wes_export.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1045 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/antibody.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1711 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/available_assays.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1097 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/assays/wes_assay.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      781 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/assays/ihc_assay.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1019 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/assays/cytof_assay.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      732 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/assays/mif_assay.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      864 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/assays/olink_assay.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1497 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/assays/rna_expression_assay.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1790 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/clinical_trial.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-01 13:52:42.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/artifacts/
--rw-rw-r--   0 travis    (2000) travis    (2000)      408 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/artifacts/artifact_fastq.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      437 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/artifacts/artifact_text.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      400 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/artifacts/artifact_bam.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      432 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/artifacts/artifact_fcs.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      963 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/artifacts/artifact_npx.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      400 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/artifacts/artifact_maf.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      984 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/artifacts/artifact_image.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      445 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/artifacts/artifact_binary.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      816 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/artifacts/artifact_csv.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      439 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/artifacts/artifact_xlsx.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     2564 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/artifacts/artifact_core.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      432 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/artifacts/artifact_zip.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      400 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/artifacts/artifact_vcf.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      817 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/user.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-01 13:52:42.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/templates/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-01 13:52:42.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/templates/metadata/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5490 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/templates/metadata/olink_template.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     7852 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/templates/metadata/cytof_template.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     4330 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/templates/metadata/wes_template.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     6865 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/templates/metadata/ihc_template.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-01 13:52:42.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/templates/manifests/
--rw-rw-r--   0 travis    (2000) travis    (2000)    13964 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/templates/manifests/plasma_template.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    14688 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/templates/manifests/pbmc_template.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    12386 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/sample.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     2937 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/participant.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     2452 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/cidc_schemas/schemas/aliquot.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1449 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-01 13:52:42.000000 cidc_schemas-0.9.4/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4587 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/tests/test_trial_core.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    43862 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/tests/test_prism.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      341 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/tests/constants.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-01 13:52:42.000000 cidc_schemas-0.9.4/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11605 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/tests/data/pbmc_shipping.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    23365 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/tests/data/date_examples.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)     8987 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/tests/data/tiny_manifest.xlsx
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-01 13:52:42.000000 cidc_schemas-0.9.4/tests/data/clinicaltrial_examples/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11510 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/tests/data/clinicaltrial_examples/CT_1PA_multiWES.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     2037 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/tests/data/clinicaltrial_examples/CT_minimal.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    15284 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/tests/data/clinicaltrial_examples/CT_1.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    19126 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/tests/data/pbmc_invalid.xlsx
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-01 13:52:42.000000 cidc_schemas-0.9.4/tests/data/olink/
--rw-rw-r--   0 travis    (2000) travis    (2000)    21276 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/tests/data/olink/olink_assay_combined.xlsx
--rw-rw-r--   0 travis    (2000) travis    (2000)    17905 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/tests/data/olink/olink_assay_1_NPX.xlsx
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-01 13:52:42.000000 cidc_schemas-0.9.4/tests/data/schemas/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-01 13:52:42.000000 cidc_schemas-0.9.4/tests/data/schemas/d1/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-01 13:52:42.000000 cidc_schemas-0.9.4/tests/data/schemas/d1/d2/
--rw-rw-r--   0 travis    (2000) travis    (2000)      141 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/tests/data/schemas/d1/d2/2.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      127 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/tests/data/schemas/d1/3.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      127 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/tests/data/schemas/c.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      138 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/tests/data/schemas/a.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      138 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/tests/data/schemas/b.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      144 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/tests/data/schemas/1.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      951 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/tests/test_template_writer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      779 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/tests/test_schemas.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15291 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/tests/test_assays.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3381 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/tests/test_templates.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6741 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/tests/test_template_reader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3483 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/tests/test_util.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4144 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/tests/test_artifacts.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10936 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/tests/test_json_validation.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      754 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/tests/test_generate_docs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1676 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/tests/test_clinicaltrial_examples.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1361 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/tests/conftest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3794 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/tests/test_template.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1407 2019-11-01 13:50:59.000000 cidc_schemas-0.9.4/tests/test_unprism.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-04 20:30:16.000000 cidc_schemas-0.9.5/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      314 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)      253 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3577 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/CONTRIBUTING.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      617 2019-11-04 20:30:16.000000 cidc_schemas-0.9.5/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      165 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/AUTHORS.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-04 20:30:16.000000 cidc_schemas-0.9.5/cidc_schemas.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      617 2019-11-04 20:30:16.000000 cidc_schemas-0.9.5/cidc_schemas.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-11-04 20:30:16.000000 cidc_schemas-0.9.5/cidc_schemas.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       13 2019-11-04 20:30:16.000000 cidc_schemas-0.9.5/cidc_schemas.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-11-04 20:30:16.000000 cidc_schemas-0.9.5/cidc_schemas.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5254 2019-11-04 20:30:16.000000 cidc_schemas-0.9.5/cidc_schemas.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      254 2019-11-04 20:30:16.000000 cidc_schemas-0.9.5/cidc_schemas.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       56 2019-11-04 20:30:16.000000 cidc_schemas-0.9.5/cidc_schemas.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8991 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      395 2019-11-04 20:30:16.000000 cidc_schemas-0.9.5/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)       89 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/HISTORY.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1072 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/LICENSE
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-04 20:30:16.000000 cidc_schemas-0.9.5/cidc_schemas/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4773 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/util.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11521 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/template.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10892 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/template_reader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10395 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/template_writer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34284 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/prism.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      380 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/constants.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4835 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/cli.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      880 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/unprism.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15077 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/json_validation.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      162 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-04 20:30:16.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3349 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/shipping_core.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-04 20:30:16.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/assays/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      753 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/assays/micsss_assay.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-04 20:30:16.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      642 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/composite_image.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-04 20:30:16.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/cytof/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1410 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/cytof/cytof_analysis.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3275 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/cytof/cytof_entry.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      457 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/cytof/cytof_input.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1051 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/cytof/cytof_antibody.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      790 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/fastq_pair_and_mapping.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      368 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/local_file.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1321 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/ngs_assay_core.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1600 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/image.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      965 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/imaging_data.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1469 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/mif_antibody.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      726 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/ihc_antibodies.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1201 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/mapping.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-04 20:30:16.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/imaging/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      792 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/imaging/micsss_input.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1099 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/imaging/mif_input.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      618 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/imaging/mif_entry.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      663 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/imaging/micsss_entry.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2513 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/imaging/ihc_entry.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      664 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/imaging/ihc_input.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      441 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/assay_core.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-04 20:30:16.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/olink/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      613 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/olink/olink_combined.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1918 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/olink/olink_entry.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      592 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/olink/olink_input.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      343 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/germline.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2925 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/micsss_antibody.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      526 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/alignment.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      423 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/somatic.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-04 20:30:16.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/ngs/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      638 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/ngs/wes_assay_record.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      569 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/ngs/wes_output.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      262 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/ngs/rna_input.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      863 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/ngs/rna_expression_entry.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1475 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/ngs/ngs_assay_record.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      583 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/ngs/wes_export.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1045 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/antibody.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1784 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/available_assays.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1097 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/assays/wes_assay.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      781 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/assays/ihc_assay.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1190 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/assays/cytof_assay.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      732 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/assays/mif_assay.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      864 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/assays/olink_assay.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1497 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/assays/rna_expression_assay.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1790 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/clinical_trial.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-04 20:30:16.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/artifacts/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      408 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/artifacts/artifact_fastq.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      437 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/artifacts/artifact_text.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      400 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/artifacts/artifact_bam.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      432 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/artifacts/artifact_fcs.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      963 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/artifacts/artifact_npx.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      400 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/artifacts/artifact_maf.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      984 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/artifacts/artifact_image.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      445 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/artifacts/artifact_binary.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      816 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/artifacts/artifact_csv.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      439 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/artifacts/artifact_xlsx.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2564 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/artifacts/artifact_core.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      432 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/artifacts/artifact_zip.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      400 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/artifacts/artifact_vcf.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      817 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/user.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-04 20:30:16.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/templates/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-04 20:30:16.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/templates/metadata/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5490 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/templates/metadata/olink_template.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8057 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/templates/metadata/cytof_template.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4330 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/templates/metadata/wes_template.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6865 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/templates/metadata/ihc_template.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-04 20:30:16.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/templates/analyses/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5025 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/templates/analyses/cytof_analysis_template.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-04 20:30:16.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/templates/manifests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13964 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/templates/manifests/plasma_template.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14688 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/templates/manifests/pbmc_template.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12386 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/sample.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2937 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/participant.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2452 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/cidc_schemas/schemas/aliquot.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1449 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-04 20:30:16.000000 cidc_schemas-0.9.5/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4587 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/tests/test_trial_core.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    44778 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/tests/test_prism.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      341 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/tests/constants.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-04 20:30:16.000000 cidc_schemas-0.9.5/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11605 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/tests/data/pbmc_shipping.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23365 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/tests/data/date_examples.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8987 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/tests/data/tiny_manifest.xlsx
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-04 20:30:16.000000 cidc_schemas-0.9.5/tests/data/clinicaltrial_examples/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11510 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/tests/data/clinicaltrial_examples/CT_1PA_multiWES.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2037 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/tests/data/clinicaltrial_examples/CT_minimal.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15284 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/tests/data/clinicaltrial_examples/CT_1.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19126 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/tests/data/pbmc_invalid.xlsx
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-04 20:30:16.000000 cidc_schemas-0.9.5/tests/data/olink/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21276 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/tests/data/olink/olink_assay_combined.xlsx
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17905 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/tests/data/olink/olink_assay_1_NPX.xlsx
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-04 20:30:16.000000 cidc_schemas-0.9.5/tests/data/schemas/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-04 20:30:16.000000 cidc_schemas-0.9.5/tests/data/schemas/d1/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-04 20:30:16.000000 cidc_schemas-0.9.5/tests/data/schemas/d1/d2/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      141 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/tests/data/schemas/d1/d2/2.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      127 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/tests/data/schemas/d1/3.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      127 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/tests/data/schemas/c.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      138 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/tests/data/schemas/a.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      138 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/tests/data/schemas/b.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      144 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/tests/data/schemas/1.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      951 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/tests/test_template_writer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      779 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/tests/test_schemas.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15324 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/tests/test_assays.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3381 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/tests/test_templates.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6741 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/tests/test_template_reader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3483 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/tests/test_util.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4144 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/tests/test_artifacts.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10936 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/tests/test_json_validation.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      754 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/tests/test_generate_docs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1676 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/tests/test_clinicaltrial_examples.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1361 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/tests/conftest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3794 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/tests/test_template.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1407 2019-11-04 20:28:34.000000 cidc_schemas-0.9.5/tests/test_unprism.py
```

### Comparing `cidc_schemas-0.9.4/CONTRIBUTING.rst` & `cidc_schemas-0.9.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/PKG-INFO` & `cidc_schemas-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: cidc_schemas
-Version: 0.9.4
+Version: 0.9.5
 Summary: The CIDC data model and tools for working with it.
 Home-page: https://github.com/CIMAC-CIDC/schemas
 Author: James Lindsay
 Author-email: jlindsay@jimmy.harvard.edu
 License: MIT license
 Description: UNKNOWN
 Keywords: cidc_schemas
```

### Comparing `cidc_schemas-0.9.4/cidc_schemas.egg-info/PKG-INFO` & `cidc_schemas-0.9.5/cidc_schemas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: cidc-schemas
-Version: 0.9.4
+Version: 0.9.5
 Summary: The CIDC data model and tools for working with it.
 Home-page: https://github.com/CIMAC-CIDC/schemas
 Author: James Lindsay
 Author-email: jlindsay@jimmy.harvard.edu
 License: MIT license
 Description: UNKNOWN
 Keywords: cidc_schemas
```

### Comparing `cidc_schemas-0.9.4/cidc_schemas.egg-info/SOURCES.txt` & `cidc_schemas-0.9.5/cidc_schemas.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,15 @@
 cidc_schemas/schemas/assays/components/ngs/rna_input.json
 cidc_schemas/schemas/assays/components/ngs/wes_assay_record.json
 cidc_schemas/schemas/assays/components/ngs/wes_export.json
 cidc_schemas/schemas/assays/components/ngs/wes_output.json
 cidc_schemas/schemas/assays/components/olink/olink_combined.json
 cidc_schemas/schemas/assays/components/olink/olink_entry.json
 cidc_schemas/schemas/assays/components/olink/olink_input.json
+cidc_schemas/schemas/templates/analyses/cytof_analysis_template.json
 cidc_schemas/schemas/templates/manifests/pbmc_template.json
 cidc_schemas/schemas/templates/manifests/plasma_template.json
 cidc_schemas/schemas/templates/metadata/cytof_template.json
 cidc_schemas/schemas/templates/metadata/ihc_template.json
 cidc_schemas/schemas/templates/metadata/olink_template.json
 cidc_schemas/schemas/templates/metadata/wes_template.json
 tests/__init__.py
```

### Comparing `cidc_schemas-0.9.4/README.md` & `cidc_schemas-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/LICENSE` & `cidc_schemas-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/util.py` & `cidc_schemas-0.9.5/cidc_schemas/util.py`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/template.py` & `cidc_schemas-0.9.5/cidc_schemas/template.py`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/template_reader.py` & `cidc_schemas-0.9.5/cidc_schemas/template_reader.py`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/template_writer.py` & `cidc_schemas-0.9.5/cidc_schemas/template_writer.py`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/prism.py` & `cidc_schemas-0.9.5/cidc_schemas/prism.py`

 * *Files 0% similar despite different names*

```diff
@@ -235,15 +235,16 @@
                         fields_found.append(another_result)
 
     return fields_found
 
 
 SUPPORTED_ASSAYS = ["wes", "olink", "cytof", "ihc"]
 SUPPORTED_MANIFESTS = ["pbmc", "plasma"]
-SUPPORTED_TEMPLATES = SUPPORTED_ASSAYS + SUPPORTED_MANIFESTS
+SUPPORTED_ANALYSES = ["cytof_analysis"]
+SUPPORTED_TEMPLATES = SUPPORTED_ASSAYS + SUPPORTED_MANIFESTS + SUPPORTED_ANALYSES
 
 LocalFileUploadEntry = namedtuple('LocalFileUploadEntry',
                                   ["local_path", "gs_key", "upload_placeholder", "metadata_availability"])
 
 
 def _process_property(
         key: str,
```

### Comparing `cidc_schemas-0.9.4/cidc_schemas/cli.py` & `cidc_schemas-0.9.5/cidc_schemas/cli.py`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/unprism.py` & `cidc_schemas-0.9.5/cidc_schemas/unprism.py`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/json_validation.py` & `cidc_schemas-0.9.5/cidc_schemas/json_validation.py`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/shipping_core.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/shipping_core.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/assays/micsss_assay.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/assays/micsss_assay.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/composite_image.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/composite_image.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/cytof/cytof_analysis.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/cytof/cytof_analysis.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'$id'": "'cytof_analysis'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "$id": "cytof_output",
+    "$id": "cytof_analysis",
     "$schema": "http://json-schema.org/draft-07/schema#",
     "description": "Output files generated from the CyTOF assay: FCS file with enumerations for compartment, assignment and profiling cell labels; 3 CSV keys for mapping from respective enumeration indices to the cell labels; 3 CSV files providing cell count information for each of the cell labels; Analysis.zip and Results.zip containing a variety of R scripts, figures, tables and charts with QC and other information.",
     "properties": {
         "assignment": {
             "$ref": "artifacts/artifact_csv.json"
         },
         "astrolabe_analysis": {
```

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/cytof/cytof_entry.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/cytof/cytof_entry.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/cytof/cytof_antibody.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/cytof/cytof_antibody.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/fastq_pair_and_mapping.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/fastq_pair_and_mapping.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/ngs_assay_core.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/ngs_assay_core.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/image.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/image.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/imaging_data.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/imaging_data.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/mif_antibody.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/mif_antibody.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/ihc_antibodies.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/ihc_antibodies.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/mapping.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/mapping.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/imaging/micsss_input.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/imaging/micsss_input.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/imaging/mif_input.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/imaging/mif_input.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/imaging/mif_entry.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/imaging/mif_entry.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/imaging/micsss_entry.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/imaging/micsss_entry.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/imaging/ihc_entry.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/imaging/ihc_entry.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/imaging/ihc_input.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/imaging/ihc_input.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/olink/olink_combined.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/olink/olink_combined.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/olink/olink_entry.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/olink/olink_entry.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/olink/olink_input.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/olink/olink_input.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/micsss_antibody.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/micsss_antibody.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/alignment.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/alignment.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/ngs/wes_assay_record.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/ngs/wes_assay_record.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/ngs/wes_output.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/ngs/wes_output.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/ngs/rna_expression_entry.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/ngs/rna_expression_entry.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/ngs/ngs_assay_record.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/ngs/ngs_assay_record.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/ngs/wes_export.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/ngs/wes_export.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/antibody.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/antibody.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/assays/components/available_assays.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/assays/components/available_assays.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9982142857142856%*

 * *Differences: {"'properties'": "{'cytof': {'mergeStrategy': 'arrayMergeById', 'mergeOptions': "*

 * *                 "OrderedDict([('idRef', 'assay_run_id')])}}"}*

```diff
@@ -5,15 +5,18 @@
     "mergeStrategy": "objectMerge",
     "properties": {
         "cytof": {
             "description": "Base information about the acquisition and analysis of CyTOF data.",
             "items": {
                 "$ref": "assays/cytof_assay.json"
             },
-            "mergeStrategy": "append",
+            "mergeOptions": {
+                "idRef": "assay_run_id"
+            },
+            "mergeStrategy": "arrayMergeById",
             "type": "array"
         },
         "ihc": {
             "description": "Immunohistochemical analysis.",
             "items": {
                 "$ref": "assays/ihc_assay.json"
             },
```

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/assays/wes_assay.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/assays/wes_assay.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/assays/ihc_assay.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/assays/ihc_assay.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/assays/mif_assay.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/assays/mif_assay.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/assays/olink_assay.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/assays/olink_assay.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/assays/rna_expression_assay.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/assays/rna_expression_assay.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/clinical_trial.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/clinical_trial.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/artifacts/artifact_npx.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/artifacts/artifact_npx.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/artifacts/artifact_image.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/artifacts/artifact_image.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/artifacts/artifact_csv.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/artifacts/artifact_csv.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/artifacts/artifact_core.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/artifacts/artifact_core.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/user.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/user.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/templates/metadata/olink_template.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/templates/metadata/olink_template.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/templates/metadata/cytof_template.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/templates/metadata/cytof_template.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999702380952381%*

 * *Differences: {"'properties'": "{'worksheets': {'Acquisition and Preprocessing': {'preamble_rows': {'assay run "*

 * *                 "id': OrderedDict([('merge_pointer', '/assay_run_id'), ('type_ref', "*

 * *                 "'assays/cytof_assay.json#properties/assay_run_id')])}}}}"}*

```diff
@@ -78,14 +78,18 @@
                     }
                 },
                 "preamble_rows": {
                     "assay creator": {
                         "merge_pointer": "0/assay_creator",
                         "type_ref": "assays/components/assay_core.json#properties/assay_creator"
                     },
+                    "assay run id": {
+                        "merge_pointer": "/assay_run_id",
+                        "type_ref": "assays/cytof_assay.json#properties/assay_run_id"
+                    },
                     "instrument": {
                         "merge_pointer": "0/instrument",
                         "type_ref": "assays/components/cytof/cytof_entry.json#properties/instrument"
                     },
                     "panel name": {
                         "merge_pointer": "0/panel_name",
                         "type_ref": "assays/components/cytof/cytof_entry.json#properties/panel_name"
```

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/templates/metadata/wes_template.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/templates/metadata/wes_template.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/templates/metadata/ihc_template.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/templates/metadata/ihc_template.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/templates/manifests/plasma_template.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/templates/manifests/plasma_template.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/templates/manifests/pbmc_template.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/templates/manifests/pbmc_template.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/sample.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/sample.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/participant.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/participant.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/cidc_schemas/schemas/aliquot.json` & `cidc_schemas-0.9.5/cidc_schemas/schemas/aliquot.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/setup.py` & `cidc_schemas-0.9.5/setup.py`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/tests/test_trial_core.py` & `cidc_schemas-0.9.5/tests/test_trial_core.py`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/tests/test_prism.py` & `cidc_schemas-0.9.5/tests/test_prism.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,29 +16,28 @@
 
 
 from .constants import TEST_DATA_DIR
 
 from cidc_schemas import prism
 from cidc_schemas.prism import prismify, merge_artifact, \
     merge_clinical_trial_metadata, InvalidMergeTargetException, \
-    SUPPORTED_ASSAYS, SUPPORTED_MANIFESTS, SUPPORTED_TEMPLATES, \
+    SUPPORTED_ASSAYS, SUPPORTED_MANIFESTS, SUPPORTED_TEMPLATES, SUPPORTED_ANALYSES, \
     PROTOCOL_ID_FIELD_NAME, parse_npx, merge_artifact_extra_metadata, \
     PRISM_MERGE_STRATEGIES, PRISM_PRISMIFY_STRATEGIES, ThrowOnCollision, \
     MergeCollisionException
 
 from cidc_schemas.json_validation import load_and_validate_schema, InDocRefNotFoundError
 from cidc_schemas.template import Template
 from cidc_schemas.template_writer import RowType
 from cidc_schemas.template_reader import XlTemplateReader
 
 from .constants import ROOT_DIR, SCHEMA_DIR, TEMPLATE_EXAMPLES_DIR, TEST_DATA_DIR
 from .test_templates import template_set
 from .test_assays import ARTIFACT_OBJ
 
-
 def prismify_test_set(filter = None):
     yielded = False
 
     for template, xlsx_path in template_set():
         if filter and not template.type in filter:
             continue
         xlsx, errors = XlTemplateReader.from_excel(xlsx_path)
@@ -328,22 +327,14 @@
     if template.type not in SUPPORTED_ASSAYS:
         return
 
     # turn into object.
     ct, file_maps, errs = prismify(xlsx, template)
     assert 0 == len(errs)
 
-    if template.type == 'cytof':
-        assert "CYTOF_TEST1" == ct[PROTOCOL_ID_FIELD_NAME]
-        ct[PROTOCOL_ID_FIELD_NAME] = 'test_prism_trial_id'
-
-    if template.type == 'ihc':
-        assert "ihc_test_trial" == ct[PROTOCOL_ID_FIELD_NAME]
-        ct[PROTOCOL_ID_FIELD_NAME] = 'test_prism_trial_id'
-
     if template.type in SUPPORTED_ASSAYS:
         # olink is different - is will never have array of assay "runs" - only one
         if template.type != 'olink':
             assert len(ct['assays'][template.type]) == 1
 
     elif template.type in SUPPORTED_MANIFESTS:
         assert not ct.get('assays'), "Assay created during manifest prismify"
@@ -363,24 +354,21 @@
 
     if template.type in SUPPORTED_ASSAYS :
         assert merged[PROTOCOL_ID_FIELD_NAME] == "test_prism_trial_id"
     else:
         assert TEST_PRISM_TRIAL[PROTOCOL_ID_FIELD_NAME] == merged[PROTOCOL_ID_FIELD_NAME]
 
 
-@pytest.mark.parametrize('template, xlsx_path', template_set())
-def test_unsupported_prismify(template, xlsx_path):
-
-    # skipp supported
-    if template.type in SUPPORTED_TEMPLATES:
-        return
-
-    with pytest.raises(NotImplementedError):
-        prismify(xlsx_path, schema_path)
+def test_unsupported_prismify():
+    """Check that prism raises a non-implemented error for unsupported template types."""
+    mock_template = MagicMock()
+    mock_template.type = 'some-unsupported-type'
 
+    with pytest.raises(NotImplementedError, match="'some-unsupported-type' is not supported"):
+        prismify(None, mock_template)
 
 
 @pytest.mark.parametrize('xlsx, template', prismify_test_set())
 def test_filepath_gen(xlsx, template):
 
     # TODO: every other assay
     if template.type not in SUPPORTED_ASSAYS:
@@ -726,22 +714,19 @@
     if template.type in SUPPORTED_MANIFESTS:
         assert len(prism_patch['shipments']) == 1
 
         assert prism_patch['participants'][0]['samples'][0]["cimac_id"][:7].startswith(
                 prism_patch['participants'][0]['cimac_participant_id'])
 
         if template.type == 'pbmc':
-            assert (prism_patch['shipments'][0]['manifest_id']) == "TEST123_pbmc"
-
             assert len(prism_patch['participants']) == 2
             assert len(prism_patch['participants'][0]['samples']) == 3
             assert len(prism_patch['participants'][1]['samples']) == 3
 
         elif template.type == 'plasma':
-            assert (prism_patch['shipments'][0]['manifest_id']) == "TEST123_plasma"
             assert len(prism_patch['participants']) == 2
             assert len(prism_patch['participants'][0]['samples']) == 3
             assert 'aliquots' not in prism_patch['participants'][0]['samples'][0]
 
         else: 
             assert False, f'add {template.type} specific asserts'
 
@@ -765,20 +750,34 @@
 
         else:
             raise NotImplementedError(f"no support in test for this template.type {template.type}")
 
     for f in file_maps:
         assert f'{template.type}/' in f.gs_key, f"No {template.type} template.type found"
 
-    # And we need set PROTOCOL_ID_FIELD_NAME to be the same for testing
     original_ct = copy.deepcopy(TEST_PRISM_TRIAL) 
 
-    # so we can merge
-    original_ct[PROTOCOL_ID_FIELD_NAME] = prism_patch[PROTOCOL_ID_FIELD_NAME]
-    
+    if template.type in SUPPORTED_ANALYSES:
+        # we can't merge analysis info unless an associated initial assay upload exists
+        # in the clinical trial object, so we add an initial assay upload below:
+
+        if template.type == 'cytof_analysis':
+            # simulate an initial cytof upload by prismifying the initial cytof template object,
+            # and merging it with clinical trial object
+            cytof_input_xlsx_path = os.path.join(TEMPLATE_EXAMPLES_DIR, 'cytof_template.xlsx')
+            cytof_input_xlsx, _ = XlTemplateReader.from_excel(cytof_input_xlsx_path)
+            cytof_input_template = Template.from_type('cytof')
+            cytof_input_patch, _, _ = prismify(cytof_input_xlsx, cytof_input_template)
+
+            original_ct, errs = merge_clinical_trial_metadata(cytof_input_patch, original_ct)
+            assert len(errs) == 0
+
+        else:
+            raise NotImplementedError(f"no support in test for this template.type {template.type}")
+
     # "prismify" provides only a patch so we need to merge it into a "full" ct
     full_after_prism, errs = merge_clinical_trial_metadata(prism_patch, original_ct)
     assert not errs
 
     # Assert we still have a good clinical trial object, so we can save it.
     validator.validate(full_after_prism)
 
@@ -831,14 +830,17 @@
     elif template.type in SUPPORTED_MANIFESTS:
         assert len(merged_gs_keys) == 0
 
     elif template.type == 'cytof':
         # TODO: This will need ot be updated when we accept a list of source fcs files
         assert len(merged_gs_keys) == 6
 
+    elif template.type == 'cytof_analysis':
+        assert len(merged_gs_keys) == 9  # 9 output files
+
     else:
         assert False, f"add {template.type} assay specific asserts"
 
     for file_map_entry in file_maps:
         assert len((full_ct | grep(fmap_entry.gs_key))['matched_values']) == 1 # each gs_url only once
 
     # olink is special - it's not an array
@@ -854,14 +856,18 @@
 
     elif template.type in SUPPORTED_MANIFESTS:
         assert full_ct["assays"] == original_ct["assays"]
 
     elif template.type == 'cytof':
         assert len(full_ct['assays'][template.type]) == 1
 
+    elif template.type == 'cytof_analysis':
+        # the original cytof upload had 2 records, hence after analysis, this too has 2 records
+        assert len(full_ct['assays']['cytof'][0]['records']) == 2, "More records than expected"
+
     else:
         assert False, f"add {template.type} assay specific asserts"
 
     dd = DeepDiff(full_after_prism, full_ct)
 
     if template.type=='wes':
 
@@ -884,14 +890,18 @@
 
     elif template.type in SUPPORTED_MANIFESTS:
         assert len(dd) == 0, "Unexpected CT changes"
 
     elif template.type == 'cytof':
         assert len(dd['dictionary_item_added']) == 7*6, "Unexpected CT changes"
 
+    elif template.type == 'cytof_analysis':
+        # 7 artifact attributes * 9 files
+        assert len(dd['dictionary_item_added']) == 7*9, "Unexpected CT changes"
+
     else:
         assert False, f"add {template.type} assay specific asserts"
 
 
 def test_merge_stuff():
 
     obj1 = {'_preamble_obj': 'copy_for:cytof:Antibody Information:row_0', 'cytof_antibodies': [{'_data_obj': 'cytof:Antibody Information:row_0', 'antibody': 'CD8', 'clone': 'C8/144b', 'company': 'DAKO', 'cat_num': 'C8-ABC', 'lot_num': '3983272', 'isotope': '146Nd', 'dilution': '100X', 'stain_type': 'Surface Stain'}]}
```

### Comparing `cidc_schemas-0.9.4/tests/data/pbmc_shipping.xlsx` & `cidc_schemas-0.9.5/tests/data/pbmc_shipping.xlsx`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/tests/data/date_examples.xlsx` & `cidc_schemas-0.9.5/tests/data/date_examples.xlsx`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/tests/data/tiny_manifest.xlsx` & `cidc_schemas-0.9.5/tests/data/tiny_manifest.xlsx`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/tests/data/clinicaltrial_examples/CT_1PA_multiWES.json` & `cidc_schemas-0.9.5/tests/data/clinicaltrial_examples/CT_1PA_multiWES.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/tests/data/clinicaltrial_examples/CT_minimal.json` & `cidc_schemas-0.9.5/tests/data/clinicaltrial_examples/CT_minimal.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/tests/data/clinicaltrial_examples/CT_1.json` & `cidc_schemas-0.9.5/tests/data/clinicaltrial_examples/CT_1.json`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/tests/data/pbmc_invalid.xlsx` & `cidc_schemas-0.9.5/tests/data/pbmc_invalid.xlsx`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/tests/data/olink/olink_assay_combined.xlsx` & `cidc_schemas-0.9.5/tests/data/olink/olink_assay_combined.xlsx`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/tests/data/olink/olink_assay_1_NPX.xlsx` & `cidc_schemas-0.9.5/tests/data/olink/olink_assay_1_NPX.xlsx`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/tests/test_template_writer.py` & `cidc_schemas-0.9.5/tests/test_template_writer.py`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/tests/test_schemas.py` & `cidc_schemas-0.9.5/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/tests/test_assays.py` & `cidc_schemas-0.9.5/tests/test_assays.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,14 +223,15 @@
             "isotope": "dummy",
             "dilution": "dummy",
             "stain_type": "Intracellular",
             "usage": "Used"
         }
     ]
     cytof_panel = {
+        "assay_run_id": "run_1",
         "panel_name": "DFCI default",
         "cytof_antibodies": antibodies
     }
 
     obj = {**ASSAY_CORE, **cytof_platform, **cytof_panel}    # merge three dictionaries
 
     # create the cytof object
```

### Comparing `cidc_schemas-0.9.4/tests/test_templates.py` & `cidc_schemas-0.9.5/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/tests/test_template_reader.py` & `cidc_schemas-0.9.5/tests/test_template_reader.py`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/tests/test_util.py` & `cidc_schemas-0.9.5/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/tests/test_artifacts.py` & `cidc_schemas-0.9.5/tests/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/tests/test_json_validation.py` & `cidc_schemas-0.9.5/tests/test_json_validation.py`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/tests/test_generate_docs.py` & `cidc_schemas-0.9.5/tests/test_generate_docs.py`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/tests/test_clinicaltrial_examples.py` & `cidc_schemas-0.9.5/tests/test_clinicaltrial_examples.py`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/tests/conftest.py` & `cidc_schemas-0.9.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/tests/test_template.py` & `cidc_schemas-0.9.5/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `cidc_schemas-0.9.4/tests/test_unprism.py` & `cidc_schemas-0.9.5/tests/test_unprism.py`

 * *Files identical despite different names*

