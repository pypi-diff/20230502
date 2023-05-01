# Comparing `tmp/vecdb-0.0.1.tar.gz` & `tmp/vecdb-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vecdb-0.0.1.tar", last modified: Wed Apr 26 06:52:51 2023, max compression
+gzip compressed data, was "vecdb-0.0.3.tar", last modified: Mon May  1 23:40:11 2023, max compression
```

## Comparing `vecdb-0.0.1.tar` & `vecdb-0.0.3.tar`

### file list

```diff
@@ -1,31 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 06:52:51.432372 vecdb-0.0.1/
--rw-rw-rw-   0        0        0    11547 2022-10-04 01:13:53.000000 vecdb-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      255 2023-04-26 06:52:51.431872 vecdb-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       92 2023-04-26 04:22:14.000000 vecdb-0.0.1/README.md
--rw-rw-rw-   0        0        0      134 2023-04-20 03:26:54.000000 vecdb-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-26 06:52:51.432372 vecdb-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      851 2023-04-26 06:11:34.000000 vecdb-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-26 06:52:51.404346 vecdb-0.0.1/vecdb/
--rw-rw-rw-   0        0        0       23 2023-04-26 06:11:34.000000 vecdb-0.0.1/vecdb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 06:52:51.426366 vecdb-0.0.1/vecdb/api/
--rw-rw-rw-   0        0        0        0 2023-04-26 05:04:38.000000 vecdb-0.0.1/vecdb/api/__init__.py
--rw-rw-rw-   0        0        0    30859 2023-04-26 05:56:25.000000 vecdb-0.0.1/vecdb/api/api.py
--rw-rw-rw-   0        0        0      131 2023-04-26 06:11:34.000000 vecdb-0.0.1/vecdb/api/helpers.py
--rw-rw-rw-   0        0        0     3315 2023-04-26 06:04:39.000000 vecdb-0.0.1/vecdb/api/local.py
-drwxrwxrwx   0        0        0        0 2023-04-26 06:52:51.428872 vecdb-0.0.1/vecdb/collections/
--rw-rw-rw-   0        0        0        0 2023-04-26 05:04:38.000000 vecdb-0.0.1/vecdb/collections/__init__.py
--rw-rw-rw-   0        0        0    11665 2023-04-26 06:08:36.000000 vecdb-0.0.1/vecdb/collections/dataset.py
--rw-rw-rw-   0        0        0    15627 2023-04-26 06:07:39.000000 vecdb-0.0.1/vecdb/collections/field.py
--rw-rw-rw-   0        0        0      157 2023-04-26 05:57:14.000000 vecdb-0.0.1/vecdb/constants.py
--rw-rw-rw-   0        0        0       43 2023-04-26 05:56:56.000000 vecdb-0.0.1/vecdb/errors.py
--rw-rw-rw-   0        0        0      600 2023-04-26 05:06:00.000000 vecdb-0.0.1/vecdb/types.py
-drwxrwxrwx   0        0        0        0 2023-04-26 06:52:51.430873 vecdb-0.0.1/vecdb/utils/
--rw-rw-rw-   0        0        0        0 2023-04-26 05:04:38.000000 vecdb-0.0.1/vecdb/utils/__init__.py
--rw-rw-rw-   0        0        0    14602 2023-04-26 06:11:31.000000 vecdb-0.0.1/vecdb/utils/document.py
--rw-rw-rw-   0        0        0     3355 2023-04-26 06:11:05.000000 vecdb-0.0.1/vecdb/utils/json_encoder.py
-drwxrwxrwx   0        0        0        0 2023-04-26 06:52:51.419862 vecdb-0.0.1/vecdb.egg-info/
--rw-rw-rw-   0        0        0      255 2023-04-26 06:52:51.000000 vecdb-0.0.1/vecdb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      494 2023-04-26 06:52:51.000000 vecdb-0.0.1/vecdb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 06:52:51.000000 vecdb-0.0.1/vecdb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      236 2023-04-26 06:52:51.000000 vecdb-0.0.1/vecdb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-26 06:52:51.000000 vecdb-0.0.1/vecdb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:40:11.199694 vecdb-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-05-01 23:39:43.000000 vecdb-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-01 23:40:11.199694 vecdb-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-01 23:39:43.000000 vecdb-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-01 23:39:43.000000 vecdb-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 23:40:11.203694 vecdb-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-01 23:39:43.000000 vecdb-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:40:11.195694 vecdb-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:39:43.000000 vecdb-0.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-05-01 23:39:43.000000 vecdb-0.0.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:40:11.195694 vecdb-0.0.3/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:39:43.000000 vecdb-0.0.3/tests/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:40:11.195694 vecdb-0.0.3/tests/core/test_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:39:43.000000 vecdb-0.0.3/tests/core/test_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-01 23:39:43.000000 vecdb-0.0.3/tests/core/test_api/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-01 23:39:43.000000 vecdb-0.0.3/tests/core/test_api/test_endpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:40:11.195694 vecdb-0.0.3/tests/core/test_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:39:43.000000 vecdb-0.0.3/tests/core/test_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-05-01 23:39:43.000000 vecdb-0.0.3/tests/core/test_dataset/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-01 23:39:43.000000 vecdb-0.0.3/tests/core/test_dataset/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-01 23:39:43.000000 vecdb-0.0.3/tests/test_connection_retry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:40:11.199694 vecdb-0.0.3/vecdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-01 23:39:43.000000 vecdb-0.0.3/vecdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:40:11.199694 vecdb-0.0.3/vecdb/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:39:43.000000 vecdb-0.0.3/vecdb/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16922 2023-05-01 23:39:43.000000 vecdb-0.0.3/vecdb/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-01 23:39:43.000000 vecdb-0.0.3/vecdb/api/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-01 23:39:43.000000 vecdb-0.0.3/vecdb/api/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:40:11.199694 vecdb-0.0.3/vecdb/collections/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:39:43.000000 vecdb-0.0.3/vecdb/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11102 2023-05-01 23:39:43.000000 vecdb-0.0.3/vecdb/collections/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-05-01 23:39:43.000000 vecdb-0.0.3/vecdb/collections/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-01 23:39:43.000000 vecdb-0.0.3/vecdb/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-01 23:39:43.000000 vecdb-0.0.3/vecdb/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-01 23:39:43.000000 vecdb-0.0.3/vecdb/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:40:11.199694 vecdb-0.0.3/vecdb/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:39:43.000000 vecdb-0.0.3/vecdb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14246 2023-05-01 23:39:43.000000 vecdb-0.0.3/vecdb/utils/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-05-01 23:39:43.000000 vecdb-0.0.3/vecdb/utils/example_documents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-01 23:39:43.000000 vecdb-0.0.3/vecdb/utils/json_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:40:11.199694 vecdb-0.0.3/vecdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-01 23:40:11.000000 vecdb-0.0.3/vecdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-01 23:40:11.000000 vecdb-0.0.3/vecdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 23:40:11.000000 vecdb-0.0.3/vecdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-01 23:40:11.000000 vecdb-0.0.3/vecdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-01 23:40:11.000000 vecdb-0.0.3/vecdb.egg-info/top_level.txt
```

### Comparing `vecdb-0.0.1/LICENSE` & `vecdb-0.0.3/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright 2022 Onsearch Pty LTD
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright 2022 Onsearch Pty LTD
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `vecdb-0.0.1/setup.py` & `vecdb-0.0.3/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,22 @@
-from setuptools import find_packages, setup
-
-from vecdb import __version__
-
-requirements = ["tqdm>=4.49.0", "requests>=2.0.0", "pandas>=1.5.0", "pydantic>=1.10.2"]
-
-core_test_requirements = ["pytest", "pytest-xdist", "pytest-cov"]
-
-example_test_requirements = core_test_requirements + ["torch", "scikit-learn>=0.20.0", "transformers[torch]==4.18.0"]
-
-chunk_requirements = ["fuzzysearch==0.7.3"]
-
-setup(
-    name="vecdb",
-    version=__version__,
-    url="https://relevanceai.com.au/",
-    author="Relevance AI",
-    author_email="dev@tryrelevance.com",
-    packages=find_packages(),
-    setup_requires=["wheel"],
-    install_requires=requirements,
-    package_data={"": ["*.ini"]},
-    extras_require=dict(
-        core_tests=core_test_requirements, example_tests=example_test_requirements, chunk=chunk_requirements
-    ),
-)
+from setuptools import find_packages, setup
+
+from vecdb import __version__
+
+requirements = ["tqdm>=4.49.0", "requests>=2.0.0", "pandas>=1.5.0", "pydantic>=1.10.2"]
+
+test_requirements = ["pytest", "pytest-xdist", "pytest-cov"]
+
+chunk_requirements = ["fuzzysearch==0.7.3"]
+
+setup(
+    name="vecdb",
+    version=__version__,
+    url="https://relevanceai.com.au/",
+    author="Relevance AI",
+    author_email="dev@tryrelevance.com",
+    packages=find_packages(),
+    setup_requires=["wheel"],
+    install_requires=requirements,
+    package_data={"": ["*.ini"]},
+    extras_require=dict(tests=test_requirements, chunk=chunk_requirements),
+)
```

### Comparing `vecdb-0.0.1/vecdb/collections/dataset.py` & `vecdb-0.0.3/vecdb/collections/dataset.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,316 +1,325 @@
-import time
-import logging
-
-from json import JSONDecodeError
-from typing import Any, Dict, List, Optional, Union
-
-from vecdb.api import api
-from vecdb.api import helpers
-from vecdb import types
-from vecdb import errors
-
-from vecdb.collections import field
-from vecdb.utils import document
-
-from concurrent.futures import ThreadPoolExecutor
-
-
-logging.basicConfig(level=logging.DEBUG)
-logger = logging.getLogger()
-
-
-class Dataset:
-    def __init__(self, api: api.API, dataset_id: str):
-        self._api = api
-        self._dataset_id = dataset_id
-
-    @property
-    def api(self) -> api.API:
-        return self._api
-
-    @classmethod
-    def from_details(cls: "Dataset", dataset_id: str, token: str) -> "Dataset":
-        return cls(api.API(helpers.process_token(token)), dataset_id)
-
-    @property
-    def token(self):
-        return self.api.credentials.token
-
-    def __getitem__(self, index: str) -> field.Field:
-        if isinstance(index, str):
-            if index.startswith(("_cluster_", "_cluster_otm_")) or "_cluster_id_" in index:
-                return field.ClusterField(dataset=self, field=index)
-            elif "_keyphrase_" in index:
-                return field.KeyphraseField(dataset=self, field=index)
-            else:
-                return field.Field(dataset=self, field=index)
-        else:
-            raise NotImplementedError("index must of type `str` (field in dataset)")
-
-    def __len__(self, *args, **kwargs) -> int:
-        return self.get_documents(1, *args, **kwargs)["count"]
-
-    @property
-    def dataset_id(self) -> str:
-        return self._dataset_id
-
-    @property
-    def schema(self) -> types.Schema:
-        return self.api._get_schema(self._dataset_id)
-
-    def health(self) -> Dict[str, Any]:
-        return self.api._get_health(self._dataset_id)
-
-    def create(self):
-        return self.api._create_dataset(self._dataset_id)
-
-    def delete(self):
-        return self.api._delete_dataset(self._dataset_id)
-
-    def bulk_insert(
-        self,
-        documents: Union[List[document.Document], document.DocumentList],
-        insert_chunksize: int = 20,
-        max_workers: int = 2,
-        **kwargs,
-    ):
-        def chunk_documents_with_kwargs(documents):
-            for i in range(len(documents) // insert_chunksize + 1):
-                yield {"documents": documents[i * insert_chunksize : (i + 1) * insert_chunksize], **kwargs}
-
-        results = {}
-        with ThreadPoolExecutor(max_workers=max_workers) as executor:
-            futures = executor.map(lambda kw: self.insert_documents(**kw), chunk_documents_with_kwargs(documents))
-
-        results = {"inserted": 0, "failed_documents": []}
-        for result in futures:
-            results["inserted"] += result["inserted"]
-            results["failed_documents"] += result["failed_documents"]
-
-        return results
-
-    def insert_documents(
-        self, documents: Union[List[document.Document], document.DocumentList], *args, **kwargs
-    ) -> Dict[str, Any]:
-        if hasattr(documents, "to_json"):
-            documents = documents.to_json()
-        else:
-            for index in range(len(documents)):
-                if hasattr(documents[index], "to_json"):
-                    documents[index] = documents[index].to_json()
-        return self.api._bulk_insert(dataset_id=self._dataset_id, documents=documents, *args, **kwargs)
-
-    def update_documents(
-        self,
-        documents: Union[List[document.Document], document.DocumentList],
-        insert_date: bool = True,
-        ingest_in_background: bool = True,
-        update_schema: bool = True,
-    ) -> Dict[str, Any]:
-        if hasattr(documents, "to_json"):
-            documents = documents.to_json()
-        else:
-            for index in range(len(documents)):
-                if hasattr(documents[index], "to_json"):
-                    documents[index] = documents[index].to_json()
-        return self.api._bulk_update(
-            dataset_id=self._dataset_id,
-            documents=documents,
-            insert_date=insert_date,
-            ingest_in_background=ingest_in_background,
-            update_schema=update_schema,
-        )
-
-    def get_documents(
-        self,
-        page_size: int,
-        filters: Optional[List[types.Filter]] = None,
-        sort: Optional[list] = None,
-        select_fields: Optional[List[str]] = None,
-        include_vector: bool = True,
-        random_state: int = 0,
-        is_random: bool = False,
-        after_id: Optional[List] = None,
-        worker_number: int = 0,
-    ) -> Dict[str, Any]:
-        res = self.api._get_where(
-            dataset_id=self._dataset_id,
-            page_size=page_size,
-            filters=filters,
-            sort=sort,
-            select_fields=select_fields,
-            include_vector=include_vector,
-            random_state=random_state,
-            is_random=is_random,
-            after_id=after_id,
-            worker_number=worker_number,
-        )
-        res["documents"] = document.DocumentList(res["documents"])
-        return res
-
-    def delete_documents(self, filters: Optional[List[types.Filter]]) -> Dict[str, Any]:
-        res = self.api._delete_where(dataset_id=self._dataset_id, filters=filters)
-        return res
-
-    def get_all_documents(
-        self,
-        page_size: int = 64,
-        filters: Optional[List[types.Filter]] = None,
-        select_fields: Optional[List[str]] = None,
-        sort: Optional[list] = None,
-        include_vector: bool = True,
-        random_state: int = 0,
-        is_random: bool = False,
-        after_id: Optional[List] = None,
-        worker_number: int = 0,
-        max_retries: int = 3,
-        retry_delay: int = 2,
-    ) -> Dict[str, Any]:
-        documents = []
-        retry_count = 0
-        while True:
-            try:
-                chunk = self.get_documents(
-                    page_size=page_size,
-                    filters=filters,
-                    select_fields=select_fields,
-                    after_id=after_id,
-                    worker_number=worker_number,
-                    sort=sort,
-                    include_vector=include_vector,
-                    random_state=random_state,
-                    is_random=is_random,
-                )
-            except ConnectionError as e:
-                logger.exception(e)
-                retry_count += 1
-                time.sleep(retry_delay)
-
-                if retry_count >= max_retries:
-                    raise errors.MaxRetriesError("max number of retries exceeded")
-
-            except JSONDecodeError as e:
-                logger.exception(e)
-                retry_count += 1
-                time.sleep(retry_delay)
-
-                if retry_count >= max_retries:
-                    raise errors.MaxRetriesError("max number of retries exceeded")
-
-            else:
-                after_id = chunk["after_id"]
-                if not chunk["documents"]:
-                    break
-                documents += chunk["documents"]
-                retry_count = 0
-
-        res = {}
-        res["documents"] = document.DocumentList(documents)
-        return res
-
-    def len(self, *args, **kwargs):
-        """
-        Get length of dataset, usually used with filters
-        """
-        return self.api._get_where(dataset_id=self._dataset_id, page_size=1, *args, **kwargs)["count"]
-
-    def insert_metadata(self, metadata: Dict[str, Any]):
-        return self.api._update_dataset_metadata(dataset_id=self._dataset_id, metadata=metadata)
-
-    def update_metadata(self, metadata: Dict[str, Any]):
-        old_metadata: dict = self.get_metadata()["results"]
-
-        def merge_dicts(dict1, dict2):
-            """Recursively merges dict2 into dict1"""
-            if not isinstance(dict1, dict) or not isinstance(dict2, dict):
-                return dict2
-            for k in dict2:
-                if k in dict1:
-                    dict1[k] = merge_dicts(dict1[k], dict2[k])
-                else:
-                    dict1[k] = dict2[k]
-            return dict1
-
-        return self.api._update_dataset_metadata(
-            dataset_id=self._dataset_id, metadata=merge_dicts(old_metadata, metadata)
-        )
-
-    def get_metadata(self) -> Dict[str, Any]:
-        return self.api._get_metadata(dataset_id=self._dataset_id)
-
-    def insert_local_medias(self, file_paths: List[str]) -> List[str]:
-        presigned_urls = self.api._get_file_upload_urls(self.dataset_id, files=file_paths)
-        urls = []
-        for index, file_path in enumerate(file_paths):
-            url = presigned_urls["files"][index]["url"]
-            upload_url = presigned_urls["files"][index]["upload_url"]
-            with open(file_path, "rb") as fn_byte:
-                media_content = bytes(fn_byte.read())
-            urls.append(url)
-            response = self.api._upload_media(presigned_url=upload_url, media_content=media_content)
-            assert response.status_code == 200
-        return urls
-
-    def facets(self, fields: List[str], data_interval: str = "monthly", page_size: int = 10000, asc: bool = False):
-        return self.api._facets(
-            dataset_id=self.dataset_id, fields=fields, data_interval=data_interval, page_size=page_size, asc=asc
-        )
-
-    def set_field_children(
-        self,
-        fieldchildren_id: str,
-        field: str,
-        field_children: List[str],
-        metadata: Optional[Dict[str, Any]] = None,
-        recursive: bool = True,
-    ):
-        self.api._set_field_children(
-            dataset_id=self._dataset_id,
-            fieldchildren_id=fieldchildren_id,
-            field=field,
-            field_children=field_children,
-            metadata=metadata,
-        )
-        if recursive:
-            parent_fields = self[field].list_field_parents()
-            for parent_field in parent_fields:
-                self[parent_field].add_field_children(
-                    field_children=field_children, fieldchildren_id=fieldchildren_id, recursive=recursive
-                )
-
-    def list_field_children(self, page: int = 1, page_size: int = 10000, sort=None):
-        return self.api._list_field_children(dataset_id=self._dataset_id, page=page, page_size=page_size, sort=sort)
-
-    def delete_field_children(self, fieldchildren_id: str):
-        return self.api._delete_field_children(dataset_id=self._dataset_id, fieldchildren_id=fieldchildren_id)
-
-    def aggregate(
-        self,
-        page_size: str = 20,
-        page: str = 1,
-        asc: str = False,
-        groupby: List[types.GroupBy] = None,
-        metrics: List[types.Metric] = None,
-        sort: List[Any] = None,
-        dataset_ids: List[str] = None,
-        filters: List[types.Filter] = None,
-    ):
-        return self.api._aggregate(
-            dataset_id=self._dataset_id,
-            page_size=page_size,
-            page=page,
-            asc=asc,
-            aggregation_query=dict(
-                groupby=[] if groupby is None else groupby,
-                metrics=[] if metrics is None else metrics,
-                sort=[] if sort is None else sort,
-            ),
-            dataset_ids=dataset_ids,
-            filters=filters,
-        )
-
-    def get_settings(self):
-        return self.api._get_dataset_settings(self.dataset_id)
-
-    def update_settings(self, settings: Dict[str, Any]):
-        return self.api._upsert_dataset_settings(dataset_id=self.dataset_id, settings=settings)
+import time
+import logging
+
+from json import JSONDecodeError
+from typing import Any, Dict, List, Optional, Union
+
+from vecdb.api import api
+from vecdb.api import helpers
+from vecdb import types
+from vecdb import errors
+
+import vecdb.collections.field
+from vecdb.utils import document
+
+from concurrent.futures import ThreadPoolExecutor
+
+
+# logging.basicConfig(level=logging.DEBUG)
+logger = logging.getLogger()
+
+
+class Dataset:
+    def __init__(self, api: api.API, dataset_id: str):
+        self._api = api
+        self._dataset_id = dataset_id
+
+    @property
+    def api(self) -> api.API:
+        return self._api
+
+    @classmethod
+    def from_details(cls: "Dataset", dataset_id: str, token: str) -> "Dataset":
+        return cls(api.API(helpers.process_token(token)), dataset_id)
+
+    @property
+    def token(self):
+        return self.api.credentials.token
+
+    def __getitem__(self, index: str) -> vecdb.collections.field.Field:
+        if isinstance(index, str):
+            return vecdb.collections.field.Field(dataset=self, field=index)
+        else:
+            raise NotImplementedError("index must of type `str` (field in dataset)")
+
+    def __len__(self, *args, **kwargs) -> int:
+        return self.search(1, *args, **kwargs)["count"]
+
+    @property
+    def dataset_id(self) -> str:
+        return self._dataset_id
+
+    @property
+    def schema(self) -> types.Schema:
+        return self.api._get_schema(self._dataset_id)
+
+    def health(self) -> Dict[str, Any]:
+        return self.api._get_health(self._dataset_id)
+
+    def bulk_insert(
+        self,
+        documents: Union[List[document.Document], document.DocumentList],
+        insert_chunksize: int = 20,
+        max_workers: int = 2,
+        **kwargs,
+    ):
+        def chunk_documents_with_kwargs(documents):
+            for i in range(len(documents) // insert_chunksize + 1):
+                yield {"documents": documents[i * insert_chunksize : (i + 1) * insert_chunksize], **kwargs}
+
+        results = {}
+        with ThreadPoolExecutor(max_workers=max_workers) as executor:
+            futures = executor.map(lambda kw: self.insert(**kw), chunk_documents_with_kwargs(documents))
+
+        results = {"inserted": 0, "failed_documents": []}
+        for result in futures:
+            results["inserted"] += result["inserted"]
+            results["failed_documents"] += result["failed_documents"]
+
+        return results
+
+    def insert(
+        self,
+        documents: Union[List[document.Document], document.DocumentList] = None,
+        ids: List[str] = None,
+        data: List[str] = None,
+        metadata: List[Dict[str, Any]] = None,
+        vector: List[List[float]] = None,
+        encoders: List[types.Encoder] = None,
+        *args,
+        **kwargs,
+    ) -> Dict[str, Any]:
+
+        encoders = [] if encoders is None else encoders
+        if not encoders:
+            encoders += [{"model_name": "all-mpnet-base-v2", "field": "text", "body": "text"}]
+
+        if not documents:
+            assert len(data) == len(metadata)
+            documents = [{"text": d, **md} for d, md in zip(data, metadata)]
+
+            if vector:
+                assert len(vector) == len(data)
+                for index, document in enumerate(documents):
+                    document["text_vector_"] = vector[index]
+
+            if ids:
+                assert len(ids) == len(data)
+                for index, document in enumerate(documents):
+                    document["_id"] = ids[index]
+
+        if hasattr(documents, "to_json"):
+            documents = documents.to_json()
+        else:
+            for index in range(len(documents)):
+                if hasattr(documents[index], "to_json"):
+                    documents[index] = documents[index].to_json()
+
+        return self.api._bulk_insert(
+            dataset_id=self._dataset_id, documents=documents, encoders=encoders, *args, **kwargs
+        )
+
+    def update(
+        self,
+        documents: Union[List[document.Document], document.DocumentList],
+        insert_date: bool = True,
+        ingest_in_background: bool = True,
+        update_schema: bool = True,
+    ) -> Dict[str, Any]:
+        if hasattr(documents, "to_json"):
+            documents = documents.to_json()
+        else:
+            for index in range(len(documents)):
+                if hasattr(documents[index], "to_json"):
+                    documents[index] = documents[index].to_json()
+        return self.api._bulk_update(
+            dataset_id=self._dataset_id,
+            documents=documents,
+            insert_date=insert_date,
+            ingest_in_background=ingest_in_background,
+            update_schema=update_schema,
+        )
+
+    def search(
+        self,
+        page_size: int = None,
+        sort: list = None,
+        filters: List[types.Filter] = None,
+        select_fields: List[str] = None,
+        include_vector: bool = None,
+        after_id: list = None,
+        text: str = None,
+        vector: List[float] = None,
+        field: str = None,
+        model: str = "all-mpnet-base-v2",
+        query: dict = None,
+    ) -> Dict[str, Any]:
+
+        if text or vector:
+            vector_search_query = {}
+
+            vector_search_query["model"] = model
+            if text:
+                vector_search_query["query"] = text
+            if vector:
+                vector_search_query["vector"] = vector
+            if not field:
+                vector_search_query["field"] = "text_vector_"
+
+        elif query:
+            vector_search_query = query
+
+        else:
+            vector_search_query = None
+
+        res = self.api._get_where(
+            dataset_id=self._dataset_id,
+            page_size=page_size,
+            filters=filters,
+            sort=sort,
+            select_fields=select_fields,
+            include_vector=include_vector,
+            after_id=after_id,
+            vector_search_query=vector_search_query,
+        )
+        res["documents"] = document.DocumentList(res["documents"])
+        return res
+
+    def delete(self, filters: Optional[List[types.Filter]] = None, ids: Union[str, list] = None) -> Dict[str, Any]:
+        if not filters:
+            filters = []
+        if ids:
+            if isinstance(ids, str):
+                ids = [ids]
+            filters += self["ids"] == ids
+        res = self.api._delete_where(dataset_id=self._dataset_id, filters=filters)
+        return res
+
+    def get_all(
+        self,
+        page_size: int = 64,
+        filters: Optional[List[types.Filter]] = None,
+        select_fields: Optional[List[str]] = None,
+        sort: Optional[list] = None,
+        include_vector: bool = True,
+        after_id: Optional[List] = None,
+        max_retries: int = 3,
+        retry_delay: int = 2,
+    ) -> Dict[str, Any]:
+        documents = []
+        retry_count = 0
+        while True:
+            try:
+                chunk = self.search(
+                    page_size=page_size,
+                    filters=filters,
+                    select_fields=select_fields,
+                    after_id=after_id,
+                    sort=sort,
+                    include_vector=include_vector,
+                )
+            except ConnectionError as e:
+                logger.exception(e)
+                retry_count += 1
+                time.sleep(retry_delay)
+
+                if retry_count >= max_retries:
+                    raise errors.MaxRetriesError("max number of retries exceeded")
+
+            except JSONDecodeError as e:
+                logger.exception(e)
+                retry_count += 1
+                time.sleep(retry_delay)
+
+                if retry_count >= max_retries:
+                    raise errors.MaxRetriesError("max number of retries exceeded")
+
+            else:
+                after_id = chunk["after_id"]
+                if not chunk["documents"]:
+                    break
+                documents += chunk["documents"]
+                retry_count = 0
+
+        res = {}
+        res["documents"] = document.DocumentList(documents)
+        return res
+
+    def len(self, *args, **kwargs):
+        """
+        Get length of dataset, usually used with filters
+        """
+        return self.api._get_where(dataset_id=self._dataset_id, page_size=1, *args, **kwargs)["count"]
+
+    def insert_metadata(self, metadata: Dict[str, Any]):
+        return self.api._update_dataset_metadata(dataset_id=self._dataset_id, metadata=metadata)
+
+    def update_metadata(self, metadata: Dict[str, Any]):
+        old_metadata: dict = self.get_metadata()["results"]
+
+        def merge_dicts(dict1, dict2):
+            """Recursively merges dict2 into dict1"""
+            if not isinstance(dict1, dict) or not isinstance(dict2, dict):
+                return dict2
+            for k in dict2:
+                if k in dict1:
+                    dict1[k] = merge_dicts(dict1[k], dict2[k])
+                else:
+                    dict1[k] = dict2[k]
+            return dict1
+
+        return self.api._update_dataset_metadata(
+            dataset_id=self._dataset_id, metadata=merge_dicts(old_metadata, metadata)
+        )
+
+    def get_metadata(self) -> Dict[str, Any]:
+        return self.api._get_metadata(dataset_id=self._dataset_id)
+
+    def insert_local_medias(self, file_paths: List[str]) -> List[str]:
+        presigned_urls = self.api._get_file_upload_urls(self.dataset_id, files=file_paths)
+        urls = []
+        for index, file_path in enumerate(file_paths):
+            url = presigned_urls["files"][index]["url"]
+            upload_url = presigned_urls["files"][index]["upload_url"]
+            with open(file_path, "rb") as fn_byte:
+                media_content = bytes(fn_byte.read())
+            urls.append(url)
+            response = self.api._upload_media(presigned_url=upload_url, media_content=media_content)
+            assert response.status_code == 200
+        return urls
+
+    def facets(self, fields: List[str], data_interval: str = "monthly", page_size: int = 10000, asc: bool = False):
+        return self.api._facets(
+            dataset_id=self.dataset_id, fields=fields, data_interval=data_interval, page_size=page_size, asc=asc
+        )
+
+    def aggregate(
+        self,
+        page_size: str = 20,
+        page: str = 1,
+        asc: str = False,
+        groupby: List[types.GroupBy] = None,
+        metrics: List[types.Metric] = None,
+        sort: List[Any] = None,
+        dataset_ids: List[str] = None,
+        filters: List[types.Filter] = None,
+    ):
+        return self.api._aggregate(
+            dataset_id=self._dataset_id,
+            page_size=page_size,
+            page=page,
+            asc=asc,
+            aggregation_query=dict(
+                groupby=[] if groupby is None else groupby,
+                metrics=[] if metrics is None else metrics,
+                sort=[] if sort is None else sort,
+            ),
+            dataset_ids=dataset_ids,
+            filters=filters,
+        )
+
+    def get_settings(self):
+        return self.api._get_dataset_settings(self.dataset_id)
+
+    def update_settings(self, settings: Dict[str, Any]):
+        return self.api._upsert_dataset_settings(dataset_id=self.dataset_id, settings=settings)
```

### Comparing `vecdb-0.0.1/vecdb/utils/json_encoder.py` & `vecdb-0.0.3/vecdb/utils/json_encoder.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,120 +1,120 @@
-"""Json Encoder utility
-
-To invoke JSON encoder:
-
-```
-    from relevanceai import json_encoder
-```
-
-"""
-import math
-import datetime
-import dataclasses
-import collections
-import pandas as pd
-
-from ipaddress import IPv4Address, IPv4Interface, IPv4Network, IPv6Address, IPv6Interface, IPv6Network
-
-from enum import Enum
-from types import GeneratorType
-from uuid import UUID
-from collections import deque
-from pathlib import Path
-from pathlib import PurePath
-from types import GeneratorType
-from enum import Enum
-from typing import Any
-
-from vecdb.utils import document
-
-
-# Taken from pydanitc.json
-ENCODERS_BY_TYPE = {
-    bytes: lambda o: o.decode(),
-    datetime.date: lambda o: o.isoformat(),
-    datetime.datetime: lambda o: o.isoformat(),
-    datetime.time: lambda o: o.isoformat(),
-    datetime.timedelta: lambda td: td.total_seconds(),
-    Enum: lambda o: o.value,
-    frozenset: list,
-    deque: list,
-    GeneratorType: list,
-    IPv4Address: str,
-    IPv4Interface: str,
-    IPv4Network: str,
-    IPv6Address: str,
-    IPv6Interface: str,
-    IPv6Network: str,
-    Path: str,
-    set: list,
-    UUID: str,
-}
-
-
-def json_encoder(obj: Any, force_string: bool = False):
-    """Converts object so it is json serializable
-    If you want to add your own mapping,
-    customize it this way;
-
-    Parameters
-    ------------
-    obj: Any
-        The object to convert
-    force_string: bool
-        If True, forces the object to a string representation. Used mainly for
-        analytics tracking.
-
-    Example
-    --------
-
-    YOu can use our JSON encoder easily.
-    >>> documents = [{"value": np.nan}]
-    >>> client.json_encoder(documents)
-
-    If you want to use FastAPI's json encoder, do this:
-    >>> from fastapi import jsonable_encoder
-    >>> client.json_encoder = jsonable_encoder
-
-    """
-
-    # Loop through iterators and convert
-    if isinstance(obj, (list, set, frozenset, GeneratorType, tuple, collections.deque)):
-        encoded_list = []
-        for item in obj:
-            encoded_list.append(json_encoder(item, force_string=force_string))
-        return encoded_list
-
-    # Loop through dictionaries and convert
-    if isinstance(obj, dict):
-        encoded_dict = {}
-        for key, value in obj.items():
-            encoded_key = json_encoder(key, force_string=force_string)
-            encoded_value = json_encoder(value, force_string=force_string)
-            encoded_dict[encoded_key] = encoded_value
-        return encoded_dict
-
-    # Custom conversions
-    if dataclasses.is_dataclass(obj):
-        return dataclasses.asdict(obj)
-    if isinstance(obj, Enum):
-        return obj.value
-    if isinstance(obj, PurePath):
-        return str(obj)
-    if isinstance(obj, (str, int, type(None))):
-        return obj
-    if isinstance(obj, float):
-        if math.isnan(obj):
-            return None
-        return obj
-    if isinstance(obj, (document.Document, document.DocumentList)):
-        return obj.to_json()
-    if type(obj) in ENCODERS_BY_TYPE:
-        return ENCODERS_BY_TYPE[type(obj)](obj)  # type: ignore
-
-    if force_string:
-        return repr(obj)
-
-    if isinstance(obj, pd.Timestamp):
-        return repr(obj)
-
-    raise ValueError(f"{obj} ({type(obj)}) cannot be converted to JSON format")
+"""Json Encoder utility
+
+To invoke JSON encoder:
+
+```
+    from relevanceai import json_encoder
+```
+
+"""
+import math
+import datetime
+import dataclasses
+import collections
+import pandas as pd
+
+from ipaddress import IPv4Address, IPv4Interface, IPv4Network, IPv6Address, IPv6Interface, IPv6Network
+
+from enum import Enum
+from types import GeneratorType
+from uuid import UUID
+from collections import deque
+from pathlib import Path
+from pathlib import PurePath
+from types import GeneratorType
+from enum import Enum
+from typing import Any
+
+from vecdb.utils import document
+
+
+# Taken from pydanitc.json
+ENCODERS_BY_TYPE = {
+    bytes: lambda o: o.decode(),
+    datetime.date: lambda o: o.isoformat(),
+    datetime.datetime: lambda o: o.isoformat(),
+    datetime.time: lambda o: o.isoformat(),
+    datetime.timedelta: lambda td: td.total_seconds(),
+    Enum: lambda o: o.value,
+    frozenset: list,
+    deque: list,
+    GeneratorType: list,
+    IPv4Address: str,
+    IPv4Interface: str,
+    IPv4Network: str,
+    IPv6Address: str,
+    IPv6Interface: str,
+    IPv6Network: str,
+    Path: str,
+    set: list,
+    UUID: str,
+}
+
+
+def json_encoder(obj: Any, force_string: bool = False):
+    """Converts object so it is json serializable
+    If you want to add your own mapping,
+    customize it this way;
+
+    Parameters
+    ------------
+    obj: Any
+        The object to convert
+    force_string: bool
+        If True, forces the object to a string representation. Used mainly for
+        analytics tracking.
+
+    Example
+    --------
+
+    YOu can use our JSON encoder easily.
+    >>> documents = [{"value": np.nan}]
+    >>> client.json_encoder(documents)
+
+    If you want to use FastAPI's json encoder, do this:
+    >>> from fastapi import jsonable_encoder
+    >>> client.json_encoder = jsonable_encoder
+
+    """
+
+    # Loop through iterators and convert
+    if isinstance(obj, (list, set, frozenset, GeneratorType, tuple, collections.deque)):
+        encoded_list = []
+        for item in obj:
+            encoded_list.append(json_encoder(item, force_string=force_string))
+        return encoded_list
+
+    # Loop through dictionaries and convert
+    if isinstance(obj, dict):
+        encoded_dict = {}
+        for key, value in obj.items():
+            encoded_key = json_encoder(key, force_string=force_string)
+            encoded_value = json_encoder(value, force_string=force_string)
+            encoded_dict[encoded_key] = encoded_value
+        return encoded_dict
+
+    # Custom conversions
+    if dataclasses.is_dataclass(obj):
+        return dataclasses.asdict(obj)
+    if isinstance(obj, Enum):
+        return obj.value
+    if isinstance(obj, PurePath):
+        return str(obj)
+    if isinstance(obj, (str, int, type(None))):
+        return obj
+    if isinstance(obj, float):
+        if math.isnan(obj):
+            return None
+        return obj
+    if isinstance(obj, (document.Document, document.DocumentList)):
+        return obj.to_json()
+    if type(obj) in ENCODERS_BY_TYPE:
+        return ENCODERS_BY_TYPE[type(obj)](obj)  # type: ignore
+
+    if force_string:
+        return repr(obj)
+
+    if isinstance(obj, pd.Timestamp):
+        return repr(obj)
+
+    raise ValueError(f"{obj} ({type(obj)}) cannot be converted to JSON format")
```

