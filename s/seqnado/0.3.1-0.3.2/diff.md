# Comparing `tmp/seqnado-0.3.1.tar.gz` & `tmp/seqnado-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqnado-0.3.1.tar", last modified: Fri Mar 31 12:28:36 2023, max compression
+gzip compressed data, was "seqnado-0.3.2.tar", last modified: Fri Mar 31 13:37:37 2023, max compression
```

## Comparing `seqnado-0.3.1.tar` & `seqnado-0.3.2.tar`

### file list

```diff
@@ -1,46 +1,108 @@
-drwxr-xr-x   0 catherine   (501) staff       (20)        0 2023-03-31 12:28:36.695345 seqnado-0.3.1/
--rw-r--r--   0 catherine   (501) staff       (20)    35129 2023-03-31 12:20:22.000000 seqnado-0.3.1/LICENSE
--rw-r--r--   0 catherine   (501) staff       (20)      113 2023-03-31 12:20:52.000000 seqnado-0.3.1/MANIFEST.in
--rw-r--r--   0 catherine   (501) staff       (20)      311 2023-03-31 12:28:36.695409 seqnado-0.3.1/PKG-INFO
--rw-r--r--   0 catherine   (501) staff       (20)     7580 2023-03-31 12:20:52.000000 seqnado-0.3.1/README.md
--rw-r--r--   0 catherine   (501) staff       (20)      108 2023-03-31 12:20:22.000000 seqnado-0.3.1/pyproject.toml
-drwxr-xr-x   0 catherine   (501) staff       (20)        0 2023-03-31 12:28:36.690633 seqnado-0.3.1/seqnado/
--rw-r--r--   0 catherine   (501) staff       (20)        0 2023-03-31 12:20:52.000000 seqnado-0.3.1/seqnado/__init__.py
--rw-r--r--   0 catherine   (501) staff       (20)     2938 2023-03-31 12:20:52.000000 seqnado-0.3.1/seqnado/cli.py
--rw-r--r--   0 catherine   (501) staff       (20)     6180 2023-03-31 12:20:52.000000 seqnado-0.3.1/seqnado/utils.py
--rw-r--r--   0 catherine   (501) staff       (20)     5059 2023-03-31 12:20:52.000000 seqnado-0.3.1/seqnado/utils_chipseq.py
-drwxr-xr-x   0 catherine   (501) staff       (20)        0 2023-03-31 12:28:36.692240 seqnado-0.3.1/seqnado/workflow/
-drwxr-xr-x   0 catherine   (501) staff       (20)        0 2023-03-31 12:28:36.694648 seqnado-0.3.1/seqnado/workflow/rules/
--rw-r--r--   0 catherine   (501) staff       (20)     1575 2023-03-31 12:20:52.000000 seqnado-0.3.1/seqnado/workflow/rules/align.smk
--rw-r--r--   0 catherine   (501) staff       (20)     1163 2023-03-31 12:20:52.000000 seqnado-0.3.1/seqnado/workflow/rules/align_rna.smk
--rw-r--r--   0 catherine   (501) staff       (20)      848 2023-03-31 12:20:52.000000 seqnado-0.3.1/seqnado/workflow/rules/alignment_counts.smk
--rw-r--r--   0 catherine   (501) staff       (20)     2901 2023-03-31 12:20:52.000000 seqnado-0.3.1/seqnado/workflow/rules/alignment_post_processing.smk
--rw-r--r--   0 catherine   (501) staff       (20)     1573 2023-03-31 12:20:52.000000 seqnado-0.3.1/seqnado/workflow/rules/custom_genome.smk
--rw-r--r--   0 catherine   (501) staff       (20)      946 2023-03-31 12:20:52.000000 seqnado-0.3.1/seqnado/workflow/rules/fastq_trim.smk
--rw-r--r--   0 catherine   (501) staff       (20)     1007 2023-03-31 12:20:52.000000 seqnado-0.3.1/seqnado/workflow/rules/heatmap.smk
--rw-r--r--   0 catherine   (501) staff       (20)     1608 2023-03-31 12:20:52.000000 seqnado-0.3.1/seqnado/workflow/rules/hub.smk
--rw-r--r--   0 catherine   (501) staff       (20)      713 2023-03-31 12:20:52.000000 seqnado-0.3.1/seqnado/workflow/rules/hub_rna.smk
--rw-r--r--   0 catherine   (501) staff       (20)     4671 2023-03-31 12:20:52.000000 seqnado-0.3.1/seqnado/workflow/rules/peak_call.smk
--rw-r--r--   0 catherine   (501) staff       (20)     2038 2023-03-31 12:20:52.000000 seqnado-0.3.1/seqnado/workflow/rules/pileup.smk
--rw-r--r--   0 catherine   (501) staff       (20)     1085 2023-03-31 12:20:52.000000 seqnado-0.3.1/seqnado/workflow/rules/pileup_rna.smk
--rw-r--r--   0 catherine   (501) staff       (20)     2650 2023-03-31 12:20:52.000000 seqnado-0.3.1/seqnado/workflow/rules/qc.smk
--rwxr-xr-x   0 catherine   (501) staff       (20)     2428 2023-03-31 12:20:52.000000 seqnado-0.3.1/seqnado/workflow/rules/variant.smk
--rw-r--r--   0 catherine   (501) staff       (20)     2606 2023-03-31 12:20:52.000000 seqnado-0.3.1/seqnado/workflow/snakefile_atac
--rw-r--r--   0 catherine   (501) staff       (20)      116 2023-03-31 12:20:52.000000 seqnado-0.3.1/seqnado/workflow/snakefile_build_index
--rw-r--r--   0 catherine   (501) staff       (20)     3011 2023-03-31 12:20:52.000000 seqnado-0.3.1/seqnado/workflow/snakefile_chip
--rw-r--r--   0 catherine   (501) staff       (20)     2478 2023-03-31 12:20:52.000000 seqnado-0.3.1/seqnado/workflow/snakefile_rna
--rwxr-xr-x   0 catherine   (501) staff       (20)     2151 2023-03-31 12:20:52.000000 seqnado-0.3.1/seqnado/workflow/snakefile_snp
-drwxr-xr-x   0 catherine   (501) staff       (20)        0 2023-03-31 12:28:36.691568 seqnado-0.3.1/seqnado.egg-info/
--rw-r--r--   0 catherine   (501) staff       (20)      311 2023-03-31 12:28:36.000000 seqnado-0.3.1/seqnado.egg-info/PKG-INFO
--rw-r--r--   0 catherine   (501) staff       (20)     1100 2023-03-31 12:28:36.000000 seqnado-0.3.1/seqnado.egg-info/SOURCES.txt
--rw-r--r--   0 catherine   (501) staff       (20)        1 2023-03-31 12:28:36.000000 seqnado-0.3.1/seqnado.egg-info/dependency_links.txt
--rw-r--r--   0 catherine   (501) staff       (20)      133 2023-03-31 12:28:36.000000 seqnado-0.3.1/seqnado.egg-info/entry_points.txt
--rw-r--r--   0 catherine   (501) staff       (20)        1 2023-03-31 12:22:14.000000 seqnado-0.3.1/seqnado.egg-info/not-zip-safe
--rw-r--r--   0 catherine   (501) staff       (20)       70 2023-03-31 12:28:36.000000 seqnado-0.3.1/seqnado.egg-info/requires.txt
--rw-r--r--   0 catherine   (501) staff       (20)        8 2023-03-31 12:28:36.000000 seqnado-0.3.1/seqnado.egg-info/top_level.txt
--rw-r--r--   0 catherine   (501) staff       (20)      703 2023-03-31 12:28:36.695716 seqnado-0.3.1/setup.cfg
--rw-r--r--   0 catherine   (501) staff       (20)       38 2023-03-31 12:20:22.000000 seqnado-0.3.1/setup.py
-drwxr-xr-x   0 catherine   (501) staff       (20)        0 2023-03-31 12:28:36.695139 seqnado-0.3.1/tests/
--rw-r--r--   0 catherine   (501) staff       (20)     3863 2023-03-31 12:20:52.000000 seqnado-0.3.1/tests/test_atac.py
--rw-r--r--   0 catherine   (501) staff       (20)     3862 2023-03-31 12:20:52.000000 seqnado-0.3.1/tests/test_chip.py
--rw-r--r--   0 catherine   (501) staff       (20)     4180 2023-03-31 12:20:52.000000 seqnado-0.3.1/tests/test_rna.py
+drwxr-xr-x   0 catherine   (501) staff       (20)        0 2023-03-31 13:37:37.646715 seqnado-0.3.2/
+drwxr-xr-x   0 catherine   (501) staff       (20)        0 2023-03-31 13:37:37.632312 seqnado-0.3.2/.github/
+drwxr-xr-x   0 catherine   (501) staff       (20)        0 2023-03-31 13:37:37.635954 seqnado-0.3.2/.github/workflows/
+-rw-r--r--   0 catherine   (501) staff       (20)     1541 2023-03-31 12:20:22.000000 seqnado-0.3.2/.github/workflows/test_pipelines.yml
+-rw-r--r--   0 catherine   (501) staff       (20)     1178 2023-03-31 12:20:52.000000 seqnado-0.3.2/.pre-commit-config.yaml
+-rw-r--r--   0 catherine   (501) staff       (20)    35129 2023-03-31 12:20:22.000000 seqnado-0.3.2/LICENSE
+-rw-r--r--   0 catherine   (501) staff       (20)      159 2023-03-31 13:35:24.000000 seqnado-0.3.2/MANIFEST.in
+-rw-r--r--   0 catherine   (501) staff       (20)      311 2023-03-31 13:37:37.646771 seqnado-0.3.2/PKG-INFO
+-rw-r--r--   0 catherine   (501) staff       (20)     7580 2023-03-31 12:20:52.000000 seqnado-0.3.2/README.md
+drwxr-xr-x   0 catherine   (501) staff       (20)        0 2023-03-31 13:37:37.636406 seqnado-0.3.2/config/
+-rw-r--r--   0 catherine   (501) staff       (20)     3291 2023-03-31 12:20:52.000000 seqnado-0.3.2/config/config_atac.yml
+-rw-r--r--   0 catherine   (501) staff       (20)     3511 2023-03-31 12:20:52.000000 seqnado-0.3.2/config/config_chip.yml
+-rw-r--r--   0 catherine   (501) staff       (20)     3185 2023-03-31 12:20:52.000000 seqnado-0.3.2/config/config_rna.yml
+-rw-r--r--   0 catherine   (501) staff       (20)      479 2023-03-31 12:20:52.000000 seqnado-0.3.2/environment.yml
+-rw-r--r--   0 catherine   (501) staff       (20)      108 2023-03-31 12:20:22.000000 seqnado-0.3.2/pyproject.toml
+drwxr-xr-x   0 catherine   (501) staff       (20)        0 2023-03-31 13:37:37.637141 seqnado-0.3.2/seqnado/
+-rw-r--r--   0 catherine   (501) staff       (20)        0 2023-03-31 12:20:52.000000 seqnado-0.3.2/seqnado/__init__.py
+-rw-r--r--   0 catherine   (501) staff       (20)     2938 2023-03-31 12:20:52.000000 seqnado-0.3.2/seqnado/cli.py
+drwxr-xr-x   0 catherine   (501) staff       (20)        0 2023-03-31 13:37:37.633625 seqnado-0.3.2/seqnado/data/
+drwxr-xr-x   0 catherine   (501) staff       (20)        0 2023-03-31 13:37:37.633395 seqnado-0.3.2/seqnado/data/cookiecutter_config/
+drwxr-xr-x   0 catherine   (501) staff       (20)        0 2023-03-31 13:37:37.632835 seqnado-0.3.2/seqnado/data/cookiecutter_config/config_atac/
+drwxr-xr-x   0 catherine   (501) staff       (20)        0 2023-03-31 13:37:37.638530 seqnado-0.3.2/seqnado/data/cookiecutter_config/config_atac/hooks/
+-rw-r--r--   0 catherine   (501) staff       (20)        0 2023-03-31 12:20:52.000000 seqnado-0.3.2/seqnado/data/cookiecutter_config/config_atac/hooks/generate_samplesheet.py
+drwxr-xr-x   0 catherine   (501) staff       (20)        0 2023-03-31 13:37:37.638692 seqnado-0.3.2/seqnado/data/cookiecutter_config/config_atac/{{cookiecutter.date}}_{{cookiecutter.project_id}}/
+-rw-r--r--   0 catherine   (501) staff       (20)     1663 2023-03-31 12:20:52.000000 seqnado-0.3.2/seqnado/data/cookiecutter_config/config_atac/{{cookiecutter.date}}_{{cookiecutter.project_id}}/config_atac.yml
+drwxr-xr-x   0 catherine   (501) staff       (20)        0 2023-03-31 13:37:37.633042 seqnado-0.3.2/seqnado/data/cookiecutter_config/config_chip/
+drwxr-xr-x   0 catherine   (501) staff       (20)        0 2023-03-31 13:37:37.638873 seqnado-0.3.2/seqnado/data/cookiecutter_config/config_chip/hooks/
+-rw-r--r--   0 catherine   (501) staff       (20)        0 2023-03-31 12:20:52.000000 seqnado-0.3.2/seqnado/data/cookiecutter_config/config_chip/hooks/generate_samplesheet.py
+drwxr-xr-x   0 catherine   (501) staff       (20)        0 2023-03-31 13:37:37.639020 seqnado-0.3.2/seqnado/data/cookiecutter_config/config_chip/{{cookiecutter.date}}_{{cookiecutter.project_id}}/
+-rw-r--r--   0 catherine   (501) staff       (20)     1731 2023-03-31 12:20:52.000000 seqnado-0.3.2/seqnado/data/cookiecutter_config/config_chip/{{cookiecutter.date}}_{{cookiecutter.project_id}}/config_chip.yml
+drwxr-xr-x   0 catherine   (501) staff       (20)        0 2023-03-31 13:37:37.633280 seqnado-0.3.2/seqnado/data/cookiecutter_config/config_rna/
+drwxr-xr-x   0 catherine   (501) staff       (20)        0 2023-03-31 13:37:37.639193 seqnado-0.3.2/seqnado/data/cookiecutter_config/config_rna/hooks/
+-rw-r--r--   0 catherine   (501) staff       (20)        0 2023-03-31 12:20:52.000000 seqnado-0.3.2/seqnado/data/cookiecutter_config/config_rna/hooks/generate_samplesheet.py
+drwxr-xr-x   0 catherine   (501) staff       (20)        0 2023-03-31 13:37:37.639333 seqnado-0.3.2/seqnado/data/cookiecutter_config/config_rna/{{cookiecutter.date}}_{{cookiecutter.project_id}}/
+-rw-r--r--   0 catherine   (501) staff       (20)     1549 2023-03-31 13:32:14.000000 seqnado-0.3.2/seqnado/data/cookiecutter_config/config_rna/{{cookiecutter.date}}_{{cookiecutter.project_id}}/config_rna.yml
+drwxr-xr-x   0 catherine   (501) staff       (20)        0 2023-03-31 13:37:37.633543 seqnado-0.3.2/seqnado/data/cookiecutter_config/config_snp/
+drwxr-xr-x   0 catherine   (501) staff       (20)        0 2023-03-31 13:37:37.639498 seqnado-0.3.2/seqnado/data/cookiecutter_config/config_snp/hooks/
+-rw-r--r--   0 catherine   (501) staff       (20)        0 2023-03-31 12:20:52.000000 seqnado-0.3.2/seqnado/data/cookiecutter_config/config_snp/hooks/generate_samplesheet.py
+drwxr-xr-x   0 catherine   (501) staff       (20)        0 2023-03-31 13:37:37.639722 seqnado-0.3.2/seqnado/data/cookiecutter_config/config_snp/{{cookiecutter.date}}_{{cookiecutter.project_id}}/
+-rw-r--r--   0 catherine   (501) staff       (20)      904 2023-03-31 12:20:52.000000 seqnado-0.3.2/seqnado/data/cookiecutter_config/config_snp/{{cookiecutter.date}}_{{cookiecutter.project_id}}/config_snp.yml
+drwxr-xr-x   0 catherine   (501) staff       (20)        0 2023-03-31 13:37:37.633744 seqnado-0.3.2/seqnado/data/profiles/
+drwxr-xr-x   0 catherine   (501) staff       (20)        0 2023-03-31 13:37:37.639942 seqnado-0.3.2/seqnado/data/profiles/profile_drmaa_singularity/
+-rw-r--r--   0 catherine   (501) staff       (20)      280 2023-03-31 12:20:52.000000 seqnado-0.3.2/seqnado/data/profiles/profile_drmaa_singularity/config.yaml
+drwxr-xr-x   0 catherine   (501) staff       (20)        0 2023-03-31 13:37:37.640178 seqnado-0.3.2/seqnado/data/profiles/profile_singularity/
+-rw-r--r--   0 catherine   (501) staff       (20)      189 2023-03-31 12:20:52.000000 seqnado-0.3.2/seqnado/data/profiles/profile_singularity/config.yaml
+-rw-r--r--   0 catherine   (501) staff       (20)     6180 2023-03-31 12:20:52.000000 seqnado-0.3.2/seqnado/utils.py
+-rw-r--r--   0 catherine   (501) staff       (20)     5059 2023-03-31 12:20:52.000000 seqnado-0.3.2/seqnado/utils_chipseq.py
+drwxr-xr-x   0 catherine   (501) staff       (20)        0 2023-03-31 13:37:37.641087 seqnado-0.3.2/seqnado/workflow/
+drwxr-xr-x   0 catherine   (501) staff       (20)        0 2023-03-31 13:37:37.641238 seqnado-0.3.2/seqnado/workflow/envs/
+-rw-r--r--   0 catherine   (501) staff       (20)      538 2023-03-31 12:20:52.000000 seqnado-0.3.2/seqnado/workflow/envs/environment.yml
+drwxr-xr-x   0 catherine   (501) staff       (20)        0 2023-03-31 13:37:37.634085 seqnado-0.3.2/seqnado/workflow/envs/profiles/
+drwxr-xr-x   0 catherine   (501) staff       (20)        0 2023-03-31 13:37:37.641391 seqnado-0.3.2/seqnado/workflow/envs/profiles/profile_drmaa_singularity/
+-rw-r--r--   0 catherine   (501) staff       (20)      317 2023-03-31 12:20:52.000000 seqnado-0.3.2/seqnado/workflow/envs/profiles/profile_drmaa_singularity/config.yaml
+drwxr-xr-x   0 catherine   (501) staff       (20)        0 2023-03-31 13:37:37.641558 seqnado-0.3.2/seqnado/workflow/envs/profiles/profile_singularity/
+-rw-r--r--   0 catherine   (501) staff       (20)      178 2023-03-31 12:20:52.000000 seqnado-0.3.2/seqnado/workflow/envs/profiles/profile_singularity/config.yaml
+drwxr-xr-x   0 catherine   (501) staff       (20)        0 2023-03-31 13:37:37.644052 seqnado-0.3.2/seqnado/workflow/rules/
+-rw-r--r--   0 catherine   (501) staff       (20)     1575 2023-03-31 12:20:52.000000 seqnado-0.3.2/seqnado/workflow/rules/align.smk
+-rw-r--r--   0 catherine   (501) staff       (20)     1163 2023-03-31 12:20:52.000000 seqnado-0.3.2/seqnado/workflow/rules/align_rna.smk
+-rw-r--r--   0 catherine   (501) staff       (20)      848 2023-03-31 12:20:52.000000 seqnado-0.3.2/seqnado/workflow/rules/alignment_counts.smk
+-rw-r--r--   0 catherine   (501) staff       (20)     2901 2023-03-31 12:20:52.000000 seqnado-0.3.2/seqnado/workflow/rules/alignment_post_processing.smk
+-rw-r--r--   0 catherine   (501) staff       (20)     1573 2023-03-31 12:20:52.000000 seqnado-0.3.2/seqnado/workflow/rules/custom_genome.smk
+-rw-r--r--   0 catherine   (501) staff       (20)      555 2023-03-31 13:32:14.000000 seqnado-0.3.2/seqnado/workflow/rules/deseq2_rna.smk
+-rw-r--r--   0 catherine   (501) staff       (20)      946 2023-03-31 12:20:52.000000 seqnado-0.3.2/seqnado/workflow/rules/fastq_trim.smk
+-rw-r--r--   0 catherine   (501) staff       (20)     1007 2023-03-31 12:20:52.000000 seqnado-0.3.2/seqnado/workflow/rules/heatmap.smk
+-rw-r--r--   0 catherine   (501) staff       (20)     1608 2023-03-31 12:20:52.000000 seqnado-0.3.2/seqnado/workflow/rules/hub.smk
+-rw-r--r--   0 catherine   (501) staff       (20)      713 2023-03-31 12:20:52.000000 seqnado-0.3.2/seqnado/workflow/rules/hub_rna.smk
+-rw-r--r--   0 catherine   (501) staff       (20)     4671 2023-03-31 12:20:52.000000 seqnado-0.3.2/seqnado/workflow/rules/peak_call.smk
+-rw-r--r--   0 catherine   (501) staff       (20)     2038 2023-03-31 12:20:52.000000 seqnado-0.3.2/seqnado/workflow/rules/pileup.smk
+-rw-r--r--   0 catherine   (501) staff       (20)     1085 2023-03-31 12:20:52.000000 seqnado-0.3.2/seqnado/workflow/rules/pileup_rna.smk
+-rw-r--r--   0 catherine   (501) staff       (20)     2650 2023-03-31 12:20:52.000000 seqnado-0.3.2/seqnado/workflow/rules/qc.smk
+-rwxr-xr-x   0 catherine   (501) staff       (20)     2432 2023-03-31 13:34:48.000000 seqnado-0.3.2/seqnado/workflow/rules/variant.smk
+drwxr-xr-x   0 catherine   (501) staff       (20)        0 2023-03-31 13:37:37.645034 seqnado-0.3.2/seqnado/workflow/scripts/
+-rw-r--r--   0 catherine   (501) staff       (20)     1561 2023-03-31 12:20:52.000000 seqnado-0.3.2/seqnado/workflow/scripts/create_hub_genomics.py
+-rw-r--r--   0 catherine   (501) staff       (20)     1448 2023-03-31 12:20:52.000000 seqnado-0.3.2/seqnado/workflow/scripts/create_hub_transcriptomics.py
+-rw-r--r--   0 catherine   (501) staff       (20)      708 2023-03-31 12:20:52.000000 seqnado-0.3.2/seqnado/workflow/scripts/remove_blacklist.py
+-rw-r--r--   0 catherine   (501) staff       (20)     1055 2023-03-31 12:20:52.000000 seqnado-0.3.2/seqnado/workflow/scripts/remove_duplicates.py
+-rw-r--r--   0 catherine   (501) staff       (20)      830 2023-03-31 12:20:52.000000 seqnado-0.3.2/seqnado/workflow/scripts/shift_alignments.py
+-rw-r--r--   0 catherine   (501) staff       (20)     2606 2023-03-31 12:20:52.000000 seqnado-0.3.2/seqnado/workflow/snakefile_atac
+-rw-r--r--   0 catherine   (501) staff       (20)      116 2023-03-31 12:20:52.000000 seqnado-0.3.2/seqnado/workflow/snakefile_build_index
+-rw-r--r--   0 catherine   (501) staff       (20)     3011 2023-03-31 12:20:52.000000 seqnado-0.3.2/seqnado/workflow/snakefile_chip
+-rw-r--r--   0 catherine   (501) staff       (20)     2581 2023-03-31 13:32:14.000000 seqnado-0.3.2/seqnado/workflow/snakefile_rna
+-rwxr-xr-x   0 catherine   (501) staff       (20)     2151 2023-03-31 12:20:52.000000 seqnado-0.3.2/seqnado/workflow/snakefile_snp
+drwxr-xr-x   0 catherine   (501) staff       (20)        0 2023-03-31 13:37:37.638318 seqnado-0.3.2/seqnado.egg-info/
+-rw-r--r--   0 catherine   (501) staff       (20)      311 2023-03-31 13:37:37.000000 seqnado-0.3.2/seqnado.egg-info/PKG-INFO
+-rw-r--r--   0 catherine   (501) staff       (20)     2809 2023-03-31 13:37:37.000000 seqnado-0.3.2/seqnado.egg-info/SOURCES.txt
+-rw-r--r--   0 catherine   (501) staff       (20)        1 2023-03-31 13:37:37.000000 seqnado-0.3.2/seqnado.egg-info/dependency_links.txt
+-rw-r--r--   0 catherine   (501) staff       (20)      133 2023-03-31 13:37:37.000000 seqnado-0.3.2/seqnado.egg-info/entry_points.txt
+-rw-r--r--   0 catherine   (501) staff       (20)        1 2023-03-31 12:22:14.000000 seqnado-0.3.2/seqnado.egg-info/not-zip-safe
+-rw-r--r--   0 catherine   (501) staff       (20)       70 2023-03-31 13:37:37.000000 seqnado-0.3.2/seqnado.egg-info/requires.txt
+-rw-r--r--   0 catherine   (501) staff       (20)        8 2023-03-31 13:37:37.000000 seqnado-0.3.2/seqnado.egg-info/top_level.txt
+-rw-r--r--   0 catherine   (501) staff       (20)      703 2023-03-31 13:37:37.647055 seqnado-0.3.2/setup.cfg
+-rw-r--r--   0 catherine   (501) staff       (20)       38 2023-03-31 12:20:22.000000 seqnado-0.3.2/setup.py
+-rw-r--r--   0 catherine   (501) staff       (20)       92 2023-03-31 12:20:22.000000 seqnado-0.3.2/testing.yml
+drwxr-xr-x   0 catherine   (501) staff       (20)        0 2023-03-31 13:37:37.645467 seqnado-0.3.2/tests/
+drwxr-xr-x   0 catherine   (501) staff       (20)        0 2023-03-31 13:37:37.634429 seqnado-0.3.2/tests/data/
+drwxr-xr-x   0 catherine   (501) staff       (20)        0 2023-03-31 13:37:37.645885 seqnado-0.3.2/tests/data/config/
+-rw-r--r--   0 catherine   (501) staff       (20)     3293 2023-03-31 12:20:52.000000 seqnado-0.3.2/tests/data/config/config_atac.yml
+-rw-r--r--   0 catherine   (501) staff       (20)     3513 2023-03-31 12:20:52.000000 seqnado-0.3.2/tests/data/config/config_chip.yml
+-rw-r--r--   0 catherine   (501) staff       (20)     3057 2023-03-31 12:20:52.000000 seqnado-0.3.2/tests/data/config/config_rna.yml
+drwxr-xr-x   0 catherine   (501) staff       (20)        0 2023-03-31 13:37:37.646587 seqnado-0.3.2/tests/old/
+-rw-r--r--   0 catherine   (501) staff       (20)     1955 2023-03-31 12:20:52.000000 seqnado-0.3.2/tests/old/old_test_atac.py
+-rw-r--r--   0 catherine   (501) staff       (20)     1940 2023-03-31 12:20:52.000000 seqnado-0.3.2/tests/old/old_test_chip_paired.py
+-rw-r--r--   0 catherine   (501) staff       (20)     1942 2023-03-31 12:20:52.000000 seqnado-0.3.2/tests/old/old_test_chip_single.py
+-rw-r--r--   0 catherine   (501) staff       (20)     2295 2023-03-31 12:20:52.000000 seqnado-0.3.2/tests/old/old_test_rna.py
+-rw-r--r--   0 catherine   (501) staff       (20)     2541 2023-03-31 12:20:22.000000 seqnado-0.3.2/tests/old/old_test_smk_chip.py
+-rw-r--r--   0 catherine   (501) staff       (20)     3863 2023-03-31 12:20:52.000000 seqnado-0.3.2/tests/test_atac.py
+-rw-r--r--   0 catherine   (501) staff       (20)     3862 2023-03-31 12:20:52.000000 seqnado-0.3.2/tests/test_chip.py
+-rw-r--r--   0 catherine   (501) staff       (20)     4180 2023-03-31 12:20:52.000000 seqnado-0.3.2/tests/test_rna.py
```

### Comparing `seqnado-0.3.1/LICENSE` & `seqnado-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `seqnado-0.3.1/README.md` & `seqnado-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `seqnado-0.3.1/seqnado/cli.py` & `seqnado-0.3.2/seqnado/cli.py`

 * *Files identical despite different names*

### Comparing `seqnado-0.3.1/seqnado/utils.py` & `seqnado-0.3.2/seqnado/utils.py`

 * *Files identical despite different names*

### Comparing `seqnado-0.3.1/seqnado/utils_chipseq.py` & `seqnado-0.3.2/seqnado/utils_chipseq.py`

 * *Files identical despite different names*

### Comparing `seqnado-0.3.1/seqnado/workflow/rules/align.smk` & `seqnado-0.3.2/seqnado/workflow/rules/align.smk`

 * *Files identical despite different names*

### Comparing `seqnado-0.3.1/seqnado/workflow/rules/align_rna.smk` & `seqnado-0.3.2/seqnado/workflow/rules/align_rna.smk`

 * *Files identical despite different names*

### Comparing `seqnado-0.3.1/seqnado/workflow/rules/alignment_counts.smk` & `seqnado-0.3.2/seqnado/workflow/rules/alignment_counts.smk`

 * *Files identical despite different names*

### Comparing `seqnado-0.3.1/seqnado/workflow/rules/alignment_post_processing.smk` & `seqnado-0.3.2/seqnado/workflow/rules/alignment_post_processing.smk`

 * *Files identical despite different names*

### Comparing `seqnado-0.3.1/seqnado/workflow/rules/custom_genome.smk` & `seqnado-0.3.2/seqnado/workflow/rules/custom_genome.smk`

 * *Files identical despite different names*

### Comparing `seqnado-0.3.1/seqnado/workflow/rules/fastq_trim.smk` & `seqnado-0.3.2/seqnado/workflow/rules/fastq_trim.smk`

 * *Files identical despite different names*

### Comparing `seqnado-0.3.1/seqnado/workflow/rules/heatmap.smk` & `seqnado-0.3.2/seqnado/workflow/rules/heatmap.smk`

 * *Files identical despite different names*

### Comparing `seqnado-0.3.1/seqnado/workflow/rules/hub.smk` & `seqnado-0.3.2/seqnado/workflow/rules/hub.smk`

 * *Files identical despite different names*

### Comparing `seqnado-0.3.1/seqnado/workflow/rules/hub_rna.smk` & `seqnado-0.3.2/seqnado/workflow/rules/hub_rna.smk`

 * *Files identical despite different names*

### Comparing `seqnado-0.3.1/seqnado/workflow/rules/peak_call.smk` & `seqnado-0.3.2/seqnado/workflow/rules/peak_call.smk`

 * *Files identical despite different names*

### Comparing `seqnado-0.3.1/seqnado/workflow/rules/pileup.smk` & `seqnado-0.3.2/seqnado/workflow/rules/pileup.smk`

 * *Files identical despite different names*

### Comparing `seqnado-0.3.1/seqnado/workflow/rules/pileup_rna.smk` & `seqnado-0.3.2/seqnado/workflow/rules/pileup_rna.smk`

 * *Files identical despite different names*

### Comparing `seqnado-0.3.1/seqnado/workflow/rules/qc.smk` & `seqnado-0.3.2/seqnado/workflow/rules/qc.smk`

 * *Files identical despite different names*

### Comparing `seqnado-0.3.1/seqnado/workflow/rules/variant.smk` & `seqnado-0.3.2/seqnado/workflow/rules/variant.smk`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         fasta = config["genome"]["fasta"],
         faidx = config["genome"]["fasta_index"],
     resources:
         mem_mb=1024 * 10,
     threads: config["bcftools"]["threads"]
     log:
         "seqnado_output/logs/variant/bcftools/{sample}.log",
-    shell: "bcftools mpileup --threads {threads} -Ou -f {params.fasta} {input} | bcftools call --threads {threads} -mv -Oz -o {output.vcf} > {log} 2>&1"
+    shell: "bcftools mpileup --threads {threads} -Ou -f {params.fasta} {input.bam} | bcftools call --threads {threads} -mv -Oz -o {output.vcf} > {log} 2>&1"
 
 rule bcftools_split_multiallelic:
     input:
         vcf = rules.bcftools_call_snp.output.vcf,
     output:
         vcf = "seqnado_output/variant/{sample}_splitmultiallelic.vcf.gz",
     shell: "bcftools norm -m -any {input.vcf} -o {output.vcf} -Oz"
```

### Comparing `seqnado-0.3.1/seqnado/workflow/snakefile_atac` & `seqnado-0.3.2/seqnado/workflow/snakefile_atac`

 * *Files identical despite different names*

### Comparing `seqnado-0.3.1/seqnado/workflow/snakefile_chip` & `seqnado-0.3.2/seqnado/workflow/snakefile_chip`

 * *Files identical despite different names*

### Comparing `seqnado-0.3.1/seqnado/workflow/snakefile_rna` & `seqnado-0.3.2/seqnado/workflow/snakefile_rna`

 * *Files 5% similar despite different names*

```diff
@@ -33,39 +33,40 @@
 
 include: "rules/qc.smk"
 include: "rules/fastq_trim.smk"
 include: "rules/align_rna.smk"
 include: "rules/alignment_post_processing.smk"
 include: "rules/alignment_counts.smk"
 include: "rules/pileup_rna.smk"
+include: "rules/deseq2_rna.smk"
 include: "rules/hub_rna.smk"
 
 
 rule all:
     input:
         mutiqc_full="seqnado_output/qc/full_qc_report.html",
         read_counts = "seqnado_output/feature_counts/read_counts.tsv",
-
+        deseq2=f"DESeq2_{config['DESeq2']['project_id']}.html",
         bams=expand(
             "seqnado_output/aligned/{sample}.bam",
             sample=SAMPLE_NAMES,
         ),
 
         pileups=expand(
             "seqnado_output/bigwigs/{method}/{sample}_{strand}.bigWig",
             sample=SAMPLE_NAMES,
             method=PILEUP_METHODS,
             strand=["plus", "minus"]
         ),
-
         hub=os.path.join(
             config["ucsc_hub_details"]["directory"],
             f"{config['ucsc_hub_details']['name']}.hub.txt",
         ),
 
+        
 
 onsuccess:
     slurm_files = glob.glob("slurm-*.out")
     sps_files = glob.glob("sps-*")
 
     for fn in [*slurm_files, *sps_files]:
         try:
```

### Comparing `seqnado-0.3.1/seqnado/workflow/snakefile_snp` & `seqnado-0.3.2/seqnado/workflow/snakefile_snp`

 * *Files identical despite different names*

### Comparing `seqnado-0.3.1/setup.cfg` & `seqnado-0.3.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = seqnado
-version = 0.3.1
+version = 0.3.2
 author = asmith
 author_email = alastair.smith@ndcls.ox.ac.uk
 description = Pipelines for ATAC-seq, ChIP-seq and RNA-seq analysis
 readme = "README.md"
 license = GNU GENERAL PUBLIC LICENSE Version 3
 license_file = LICENSE
 url = https://github.com/alsmith151/seqnado
```

### Comparing `seqnado-0.3.1/tests/test_atac.py` & `seqnado-0.3.2/tests/test_atac.py`

 * *Files identical despite different names*

### Comparing `seqnado-0.3.1/tests/test_chip.py` & `seqnado-0.3.2/tests/test_chip.py`

 * *Files identical despite different names*

### Comparing `seqnado-0.3.1/tests/test_rna.py` & `seqnado-0.3.2/tests/test_rna.py`

 * *Files identical despite different names*

