# Comparing `tmp/tab2neo-1.2.1.0.tar.gz` & `tmp/tab2neo-1.2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tab2neo-1.2.1.0.tar", last modified: Fri Feb  3 07:09:47 2023, max compression
+gzip compressed data, was "tab2neo-1.2.5.0.tar", last modified: Tue May 23 08:45:54 2023, max compression
```

## Comparing `tab2neo-1.2.1.0.tar` & `tab2neo-1.2.5.0.tar`

### file list

```diff
@@ -1,34 +1,37 @@
-drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-02-03 07:09:47.127519 tab2neo-1.2.1.0/
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    11357 2023-01-27 10:16:08.000000 tab2neo-1.2.1.0/LICENSE
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    13246 2023-02-03 07:09:47.127519 tab2neo-1.2.1.0/PKG-INFO
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     1218 2023-01-27 10:16:08.000000 tab2neo-1.2.1.0/README.md
-drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-02-03 07:09:47.123520 tab2neo-1.2.1.0/data_loaders/
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)      241 2023-01-27 10:16:08.000000 tab2neo-1.2.1.0/data_loaders/__init__.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     3584 2023-01-27 10:16:08.000000 tab2neo-1.2.1.0/data_loaders/azure_data_loader.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    18791 2023-01-27 10:16:08.000000 tab2neo-1.2.1.0/data_loaders/file_data_loader.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     1492 2023-01-27 10:16:08.000000 tab2neo-1.2.1.0/data_loaders/hive_data_loader.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     1157 2023-01-27 10:16:08.000000 tab2neo-1.2.1.0/data_loaders/sql_server_data_loader.py
-drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-02-03 07:09:47.123520 tab2neo-1.2.1.0/data_providers/
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       54 2023-01-27 10:16:08.000000 tab2neo-1.2.1.0/data_providers/__init__.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    10233 2023-01-27 10:16:08.000000 tab2neo-1.2.1.0/data_providers/data_provider.py
-drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-02-03 07:09:47.123520 tab2neo-1.2.1.0/logger/
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)        0 2023-01-27 10:16:08.000000 tab2neo-1.2.1.0/logger/__init__.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     1192 2023-01-27 10:16:08.000000 tab2neo-1.2.1.0/logger/logger.py
-drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-02-03 07:09:47.123520 tab2neo-1.2.1.0/model_appliers/
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       53 2023-01-27 10:16:08.000000 tab2neo-1.2.1.0/model_appliers/__init__.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    29100 2023-01-27 10:16:08.000000 tab2neo-1.2.1.0/model_appliers/model_applier.py
-drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-02-03 07:09:47.127519 tab2neo-1.2.1.0/model_managers/
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       53 2023-01-27 10:16:08.000000 tab2neo-1.2.1.0/model_managers/__init__.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    53913 2023-02-03 07:08:34.000000 tab2neo-1.2.1.0/model_managers/model_manager.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)      103 2023-01-27 10:16:08.000000 tab2neo-1.2.1.0/pyproject.toml
-drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-02-03 07:09:47.127519 tab2neo-1.2.1.0/query_builders/
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       53 2023-01-27 10:16:08.000000 tab2neo-1.2.1.0/query_builders/__init__.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    32478 2023-01-27 10:16:08.000000 tab2neo-1.2.1.0/query_builders/query_builder.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       38 2023-02-03 07:09:47.127519 tab2neo-1.2.1.0/setup.cfg
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     2282 2023-02-03 07:08:34.000000 tab2neo-1.2.1.0/setup.py
-drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-02-03 07:09:47.127519 tab2neo-1.2.1.0/tab2neo.egg-info/
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    13246 2023-02-03 07:09:47.000000 tab2neo-1.2.1.0/tab2neo.egg-info/PKG-INFO
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)      631 2023-02-03 07:09:47.000000 tab2neo-1.2.1.0/tab2neo.egg-info/SOURCES.txt
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)        1 2023-02-03 07:09:47.000000 tab2neo-1.2.1.0/tab2neo.egg-info/dependency_links.txt
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)      544 2023-02-03 07:09:47.000000 tab2neo-1.2.1.0/tab2neo.egg-info/requires.txt
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       80 2023-02-03 07:09:47.000000 tab2neo-1.2.1.0/tab2neo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 08:45:54.514190 tab2neo-1.2.5.0/
+-rw-rw-rw-   0        0        0    11558 2023-04-11 17:18:19.000000 tab2neo-1.2.5.0/LICENSE
+-rw-rw-rw-   0        0        0    19117 2023-05-23 08:45:54.512195 tab2neo-1.2.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5544 2023-05-22 13:56:28.000000 tab2neo-1.2.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 08:45:53.094202 tab2neo-1.2.5.0/data_loaders/
+-rw-rw-rw-   0        0        0      245 2023-04-11 17:18:19.000000 tab2neo-1.2.5.0/data_loaders/__init__.py
+-rw-rw-rw-   0        0        0     3477 2023-04-11 17:18:19.000000 tab2neo-1.2.5.0/data_loaders/azure_data_loader.py
+-rw-rw-rw-   0        0        0    19213 2023-05-09 11:46:26.000000 tab2neo-1.2.5.0/data_loaders/file_data_loader.py
+-rw-rw-rw-   0        0        0     1535 2023-04-11 17:18:19.000000 tab2neo-1.2.5.0/data_loaders/hive_data_loader.py
+-rw-rw-rw-   0        0        0     1186 2023-04-11 17:18:19.000000 tab2neo-1.2.5.0/data_loaders/sql_server_data_loader.py
+drwxrwxrwx   0        0        0        0 2023-05-23 08:45:53.429194 tab2neo-1.2.5.0/data_providers/
+-rw-rw-rw-   0        0        0       55 2023-04-11 17:18:19.000000 tab2neo-1.2.5.0/data_providers/__init__.py
+-rw-rw-rw-   0        0        0    11225 2023-05-22 13:56:28.000000 tab2neo-1.2.5.0/data_providers/data_provider.py
+drwxrwxrwx   0        0        0        0 2023-05-23 08:45:53.518205 tab2neo-1.2.5.0/logger/
+-rw-rw-rw-   0        0        0        0 2023-04-11 17:18:20.000000 tab2neo-1.2.5.0/logger/__init__.py
+-rw-rw-rw-   0        0        0     1258 2023-04-11 17:18:20.000000 tab2neo-1.2.5.0/logger/logger.py
+drwxrwxrwx   0        0        0        0 2023-05-23 08:45:53.574189 tab2neo-1.2.5.0/model_appliers/
+-rw-rw-rw-   0        0        0       53 2023-04-11 17:18:20.000000 tab2neo-1.2.5.0/model_appliers/__init__.py
+-rw-rw-rw-   0        0        0    29922 2023-05-22 13:56:28.000000 tab2neo-1.2.5.0/model_appliers/model_applier.py
+drwxrwxrwx   0        0        0        0 2023-05-23 08:45:53.742196 tab2neo-1.2.5.0/model_managers/
+-rw-rw-rw-   0        0        0       53 2023-04-11 17:18:20.000000 tab2neo-1.2.5.0/model_managers/__init__.py
+-rw-rw-rw-   0        0        0    56933 2023-05-09 11:46:26.000000 tab2neo-1.2.5.0/model_managers/model_manager.py
+-rw-rw-rw-   0        0        0    55497 2023-04-11 17:22:12.000000 tab2neo-1.2.5.0/model_managers/temp.py
+-rw-rw-rw-   0        0        0      108 2023-04-11 17:18:20.000000 tab2neo-1.2.5.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-23 08:45:54.079204 tab2neo-1.2.5.0/query_builders/
+-rw-rw-rw-   0        0        0       53 2023-04-11 17:18:20.000000 tab2neo-1.2.5.0/query_builders/__init__.py
+-rw-rw-rw-   0        0        0    41633 2023-05-09 11:46:26.000000 tab2neo-1.2.5.0/query_builders/query_builder.py
+-rw-rw-rw-   0        0        0       42 2023-05-23 08:45:54.514190 tab2neo-1.2.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     2340 2023-05-09 11:46:26.000000 tab2neo-1.2.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 08:45:54.493201 tab2neo-1.2.5.0/tab2neo.egg-info/
+-rw-rw-rw-   0        0        0    19117 2023-05-23 08:45:51.000000 tab2neo-1.2.5.0/tab2neo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      689 2023-05-23 08:45:52.000000 tab2neo-1.2.5.0/tab2neo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 08:45:51.000000 tab2neo-1.2.5.0/tab2neo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      544 2023-05-23 08:45:51.000000 tab2neo-1.2.5.0/tab2neo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       80 2023-05-23 08:45:51.000000 tab2neo-1.2.5.0/tab2neo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 08:45:54.509200 tab2neo-1.2.5.0/tests/
+-rw-rw-rw-   0        0        0     8029 2023-04-11 17:18:20.000000 tab2neo-1.2.5.0/tests/test_comparison_utilities.py
```

### Comparing `tab2neo-1.2.1.0/LICENSE` & `tab2neo-1.2.5.0/LICENSE`

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
-   Copyright [yyyy] [name of copyright owner]
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
+   Copyright [yyyy] [name of copyright owner]
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

### Comparing `tab2neo-1.2.1.0/data_loaders/azure_data_loader.py` & `tab2neo-1.2.5.0/data_loaders/azure_data_loader.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,78 +1,76 @@
-from data_loaders import FileDataLoader
-import os
-from azure.storage.filedatalake import DataLakeServiceClient
-from azure.identity import ClientSecretCredential
-
-
-class AzureDataLoader(FileDataLoader):
-    """
-    Assumes the following environmental variables to be defined with credentials to access Azure blob storage:
-    AZ_CONTAINER, AZ_TENANT, AZ_CLIENT, AZ_CLIENT_SECRET;
-    AZ_FILESYSTEM also needs to be set.
-    Load data into Neo4j from Azure blob storage, with support for input formats: rda, xpt, sas7bdat and xls, xlsx
-    All functions available in FileDataLoader are available here as well
-    """
-
-    def __init__(self, temp_folder=None, domain_dict=None, *args, **kwargs):
-        """
-        :param temp_folder: temporary folder where files from Azure would be downloaded to
-                            (files by default deleted after operation completed)
-        :param domain_dict: dictionary with file names as keys, and domain to be assigned as values
-                            (e.g. {'dm_xyz.sas7bdat': 'DM', 'ae_xyz.sas7bdat': 'AE'} )
-        :param verbose: bool - to print or not to print exec details
-        :param debug: bool - to print or not to print details for debugging (e.g. cypher queries to be submitted)
-        :param args: other arguments
-        :param kwargs: other keyword arguments
-        """
-        super().__init__(domain_dict=domain_dict, *args, **kwargs)
-        self.temp_folder = temp_folder if temp_folder is not None else 'temp'
-
-        # Create the temp folder, if it doesn't already exist
-        if not os.path.exists(self.temp_folder):
-            os.makedirs(self.temp_folder)
-
-        # Set up connection details to the Azure data lake
-        self.service = DataLakeServiceClient(
-            account_url=f"https://{os.environ.get('AZ_CONTAINER')}.dfs.core.windows.net/",
-            credential=ClientSecretCredential(tenant_id=os.environ.get("AZ_TENANT"),
-                                              client_id=os.environ.get("AZ_CLIENT"),
-                                              client_secret=os.environ.get("AZ_CLIENT_SECRET"))
-        )
-
-        self.fs = self.service.get_file_system_client(file_system=os.environ.get("AZ_FILESYSTEM"))
-
-    def listdir(self, path: str) -> [str]:
-        """
-        Lists all files (full path) in a directory on Azure blob storage
-
-        :param path: A list of strings
-                     # EXAMPLE of list item: "rd/space/test_compound/trial_01/testing_01/sdtm/vs.sas7bdat"
-        """
-        return [path.name for path in self.fs.get_paths(path=path)]
-
-    def read_file(self, folder: str, filename: str, clean_up=True, *args, **kwargs):
-        """
-        Downloads file from Azure blob storage into a temporary folder {self.temp_folder},
-        calls FileDataLoader.read_file against it and returns the result
-
-        :param folder:
-        :param filename:
-        :param clean_up: Flag indicating whether to delete the temporary files
-        :param args:
-        :param kwargs:
-        :return:
-        """
-        directory_client = self.fs.get_directory_client(folder)
-        file_client = directory_client.get_file_client(filename)
-        download = file_client.download_file()
-
-        local_file = open(os.path.join(self.temp_folder, filename), 'wb')
-        downloaded_bytes = download.readall()
-        local_file.write(downloaded_bytes)
-        local_file.close()
-
-        res = super().read_file(self.temp_folder, filename, *args, **kwargs)
-        if clean_up:
-            os.remove(os.path.join(self.temp_folder, filename))
-
-        return res
+from data_loaders import FileDataLoader
+import os
+from azure.storage.filedatalake import DataLakeServiceClient
+from azure.identity import ClientSecretCredential
+
+
+class AzureDataLoader(FileDataLoader):
+    """
+    Assumes the following environmental variables to be defined with credentials to access Azure blob storage:
+    AZ_CONTAINER, AZ_TENANT, AZ_CLIENT, AZ_CLIENT_SECRET;
+    AZ_FILESYSTEM also needs to be set.
+    Load data into Neo4j from Azure blob storage, with support for input formats: rda, xpt, sas7bdat and xls, xlsx
+    All functions available in FileDataLoader are available here as well
+    """
+
+    def __init__(self, temp_folder=None, domain_dict=None, *args, **kwargs):
+        """
+        :param temp_folder: temporary folder where files from Azure would be downloaded to
+                            (files by default deleted after operation completed)
+        :param domain_dict: dictionary with file names as keys, and domain to be assigned as values
+                            (e.g. {'dm_xyz.sas7bdat': 'DM', 'ae_xyz.sas7bdat': 'AE'} )
+        :param args: other arguments
+        :param kwargs: other keyword arguments
+        """
+        super().__init__(domain_dict=domain_dict, *args, **kwargs)
+        self.temp_folder = temp_folder if temp_folder is not None else 'temp'
+
+        # Create the temp folder, if it doesn't already exist
+        if not os.path.exists(self.temp_folder):
+            os.makedirs(self.temp_folder)
+
+        # Set up connection details to the Azure data lake
+        self.service = DataLakeServiceClient(
+            account_url=f"https://{os.environ.get('AZ_CONTAINER')}.dfs.core.windows.net/",
+            credential=ClientSecretCredential(tenant_id=os.environ.get("AZ_TENANT"),
+                                              client_id=os.environ.get("AZ_CLIENT"),
+                                              client_secret=os.environ.get("AZ_CLIENT_SECRET"))
+        )
+
+        self.fs = self.service.get_file_system_client(file_system=os.environ.get("AZ_FILESYSTEM"))
+
+    def listdir(self, path: str) -> [str]:
+        """
+        Lists all files (full path) in a directory on Azure blob storage
+
+        :param path: A list of strings
+                     # EXAMPLE of list item: "rd/space/test_compound/trial_01/testing_01/sdtm/vs.sas7bdat"
+        """
+        return [path.name for path in self.fs.get_paths(path=path)]
+
+    def read_file(self, folder: str, filename: str, clean_up=True, *args, **kwargs):
+        """
+        Downloads file from Azure blob storage into a temporary folder {self.temp_folder},
+        calls FileDataLoader.read_file against it and returns the result
+
+        :param folder:
+        :param filename:
+        :param clean_up: Flag indicating whether to delete the temporary files
+        :param args:
+        :param kwargs:
+        :return:
+        """
+        directory_client = self.fs.get_directory_client(folder)
+        file_client = directory_client.get_file_client(filename)
+        download = file_client.download_file()
+
+        local_file = open(os.path.join(self.temp_folder, filename), 'wb')
+        downloaded_bytes = download.readall()
+        local_file.write(downloaded_bytes)
+        local_file.close()
+
+        res = super().read_file(self.temp_folder, filename, *args, **kwargs)
+        if clean_up:
+            os.remove(os.path.join(self.temp_folder, filename))
+
+        return res
```

### Comparing `tab2neo-1.2.1.0/data_loaders/file_data_loader.py` & `tab2neo-1.2.5.0/data_loaders/file_data_loader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,369 +1,370 @@
-import neointerface
-import pandas as pd
-import re
-import pyreadstat       # A library that was open-sourced by Roche
-import pyreadr          # Used for the RDA format
-import os
-
-
-class FileDataLoader(neointerface.NeoInterface):
-    """
-    Load data into Neo4j, with support for the following input formats:
-            rda, xpt, sas7bdat, xls, xlsx
-    A goal is to harmonize those formats.
-    """
-
-    def __init__(self, domain_dict = None, *args, **kwargs):
-        """
-        :param domain_dict: dictionary with file names as keys and domain to be assigned as values
-                            (e.g. {'dm_xyz.sas7bdat': 'DM', 'ae_xyz.sas7bdat': 'AE'} )
-        :param verbose: bool - to print or not to print exec details
-        :param debug: bool - to print or not to print details for debugging (e.g. cypher queries to be submitted)
-        :param args: other arguments
-        :param kwargs: other keyword arguments
-        """
-        self.domain_dict = domain_dict
-        super().__init__(*args, **kwargs)
-
-
-    def read_file(self, folder:str, filename:str, sheet_name=0, query=None, metadataonly = False, test_run = False,
-                  colcharsbl =r'[^A-Za-z0-9_]+'):
-        """
-        Read in an external file as a Pandas data frame.
-        Can read in file types: rda, xpt, sas7bdat, xls, csv
-        It can OPTIONALLY only retrieve the metadata from the source file.
-
-        Note: nothing is actually loaded into Neo4j
-
-        It returns a Pandas data frame, and the metadata.
-
-        In case of error (such as an unsupported file format), an Exception is raised.
-
-        :param folder:          Name of directory where the file to load resides
-        :param filename:        Name (exclusive of path) of file to load
-        :param sheet_name       Only for xls and xlsx - name of the sheet to load
-        :param query            If not None apply a df.query on the dataframe being read
-        :param metadataonly:    If True then only the folder, filename, and column names are imported
-        :param test_run:        If True, only read the first 100 rows (Not applicable if the flag metadataonly is True)
-        :param colcharsbl:      The column names of the input files are renamed in such a way that the symbols
-                                    specified by the regex pattern are excluded
-                                    (e.g. for cleaning special characters in the colnames of excel files)
-                                    EXAMPLE: r'[^A-Za-z0-9_]+' will only keep A-Z, a-z, 0-9 and the underscore
-                                    TODO: Perhaps default it to None, and if not None, then apply it
-                                          regardless of the file extension (currently, only applied to Excel files)
-
-        :return:                 The pair (Pandas data frame, metadata)
-                                    EXAMPLE of the Pandas data frame:
-                                              STUDYID     SITEID   ...    BIRTHDATE
-                                        0    mid987650  214356.0   ...   1983-06-30
-                                        1    mid987650  214356.0   ...   1956-06-30
-
-                                    EXAMPLE of a value for meta:
-                                        {'column_names': ['STUDYID', 'SITEID', 'BIRTHDATE']}
-        """
-        assert query is None or isinstance(query, str)
-
-        ext = filename.split(".")[-1]               # Extract the filename extension (e.g. "rda")
-
-        # Special processing for the various file formats we support
-        # Set df to the Pandas dataframe, and meta to the dictionary {'column_names' : LIST_OF_COLUMN_NAMES_IN_DATA}
-        if ext in ["sas7bdat"]:
-            df, meta = pyreadstat.read_sas7bdat(os.path.join(folder, filename), metadataonly = metadataonly)
-            meta = meta.__dict__
-        elif ext in ["xpt"]:
-            df, meta = pyreadstat.read_xport(os.path.join(folder, filename), metadataonly = metadataonly)
-            meta = meta.__dict__
-        elif ext in ["rda"]:
-            r_result = pyreadr.read_r(os.path.join(folder, filename))
-            name, df = r_result.popitem(last=False)
-            meta = {'column_names': list(df.columns)}
-            if metadataonly:
-                df = pd.DataFrame(columns = df.columns)
-        elif ext in ["xls", "xlsx"]:
-            if ext == "xls":
-                df = pd.read_excel(os.path.join(folder, filename), sheet_name=sheet_name)
-            elif ext == "xlsx":
-                df = pd.read_excel(os.path.join(folder, filename), engine='openpyxl', sheet_name=sheet_name)
-            df.columns = [re.sub(colcharsbl, '', re.sub(r'\s', '_', s)) for s in df.columns] #TODO: maybe apply to ALL data types
-            meta = {'column_names': list(df.columns)}
-            if metadataonly:
-                df = pd.DataFrame(columns = df.columns)
-        elif ext in ["csv"]:
-            # Todo: N.B CDISC Library provides csv files where values are quoted (i.e. "variabel 1","Another variable")
-            #  Therefore option quotechar is used, which means that " will not appear in data.
-            #  Have not tested or thought of scenarios what would happen if values are not quoted
-            df = pd.read_csv(os.path.join(folder, filename), quotechar='"')
-            meta = {'column_names': list(df.columns)}
-            if metadataonly:
-                df = pd.DataFrame(columns = df.columns)
-        else:
-            raise Exception(f"Unsupported file format - unrecognized filename extension: {ext}")
-
-        # EXAMPLE of a value for meta:
-        #   {'column_names': ['STUDYID', 'SITEID', 'AGE']}
-
-        if test_run:
-            df = df.head(100)   # Only use the first 100 rows
-
-        # since pandas sets missing strings to float NaN we actively replace na with ''
-        col_obj = [col for col in df.columns if df[col].dtype == 'object']
-        df[col_obj] = df[col_obj].fillna(value='')
-
-        if query:
-            df = df.query(query)
-
-        return (df, meta)
-
-
-    def load_file(self, folder:str, filename:str, sheet_name=0, query=None, metadataonly = False, dataonly = False, test_run = False,
-                        load_to_neo = True, colcharsbl =r'[^A-Za-z0-9_]+'):
-        """
-        Read in an external file as a Pandas data frame.
-
-        Can read in file types: rda, xpt, sas7bdat, xls, csv
-        It can OPTIONALLY only retrieve the metadata from the source file.
-        It OPTIONALLY loads into Neo4j the metadata (creating 3 node labels: `Source Data Folder`, `Source Data Table`, `Source Data Column`),
-                and, if imported, the data (creating nodes with the label `Source Data Row`,
-                                            and also adding an extra field named `_domain_` to store the domain.)
-                Whenever data is loaded to Neo4j, the following relationships are also created:
-                    1) `Source Data Folder` -[:HAS_TABLE]-> `Source Data Table`
-                    2) `Source Data Table` -[:HAS_COLUMN]-> to all `Source Data Column` nodes
-                    3) 'Source Data Table' -[:HAS_DATA]-> to all 'Source Data Row' nodes
-
-        "DOMAIN" - term used for the capitalized version of the basename of the datafile, for provenance information
-
-        It returns a Pandas data frame.
-
-        In case of error (such as an unsupported file format), an Exception is raised.
-
-        :param folder:          Name of directory where the file to load resides
-        :param filename:        Name (exclusive of path) of file to load
-        :param sheet_name       Only for xls and xlsx - name of the sheet to load
-        :param query:           A parameter to be passed to read_file
-        :param metadataonly:    If True then only the folder, filename, and column names are imported
-        :param dataonly:
-        :param test_run:        If True, only read the first 100 rows (Not applicable if the flag metadataonly is True)
-        :param load_to_neo:     If True then data (INCL. metadata) is loaded into Neo4j nodes with `Source Data Row` labels
-        :param colcharsbl:      The column names of the input files are renamed in such a way that the symbols
-                                    specified by the regex pattern are excluded
-                                    (e.g. for cleaning special characters in the colnames of excel files)
-                                    EXAMPLE: r'[^A-Za-z0-9_]+' will only keep A-Z, a-z, 0-9 and the underscore
-                                    TODO: Perhaps default it to None, and if not None, then apply it
-                                          regardless of the file extension (currently, only applied to Excel files)
-
-        :return:                 A Pandas data frame.  EXAMPLE:
-                                             STUDYID    SITEID    USUBJID  ...        TRTETM   BRTHDT      BRTHDTC
-                                        0    mid987650  214356.0  987650.000001  ...  33420.0  1983-06-30  1983.0
-                                        1    mid987650  214356.0  987650.000002  ...  33420.0  1956-06-30  1956.0
-        """
-        (df, meta) = self.read_file(folder=folder, filename=filename, sheet_name=sheet_name, query=query, metadataonly=metadataonly,
-                                    test_run=test_run, colcharsbl=colcharsbl)
-
-        fn = ".".join(filename.split(".")[:-1])     # The filename excluding the dot and the extension suffix
-        ext = filename.split(".")[-1]
-
-        if ext in ["xls", "xlsx"] and isinstance(sheet_name, str):
-            domain = f"{fn}.{sheet_name}".upper()
-        else:
-            domain = fn.upper()
-            
-        if self.domain_dict:
-            if filename in self.domain_dict.keys():
-                domain = self.domain_dict[filename]
-
-        # If the dataframe isn't empty, and it was requested to load the data into Neo4j,
-        #       create nodes with the label `Source Data Row`
-        if not df.empty and not metadataonly:
-            # Timestamp data formats are not supported in neo4j as parameters to the query; therefore, changing to str
-            # This does not cause trouble with SDTM data as dates are stored as str ther,e but would cause problems with
-            # raw and ADaM data
-            # TODO: get rid of this temporary workaround
-            for i, dtype in enumerate(df.dtypes):
-                if not dtype in ['O', 'float64', 'int64']:
-                    df[df.columns[i]] = df[df.columns[i]].astype(str)
-
-            # loading data
-            # df = df.assign(_filename_ = filename)
-            df = df.assign(_domain_=domain)  # Add new column, to keep track of the data provenance
-            df = df.assign(_filename_=filename)  # Add new column, to keep track of the data provenance
-            df = df.assign(_folder_=folder)  # Add new column, to keep track of the data provenance
-            if load_to_neo:
-                self.load_df(df=df, label="Source Data Row", merge=False)
-                # self.load_df_clean_nan()
-
-        # If the meta dictionary contains, as expected, the key 'column_names',
-        #       and if the data (and metadata) is to be loaded into Neo4j,
-        #       then handle the loading of the metadata
-        if not dataonly:
-            if 'column_names' in meta.keys() and load_to_neo:
-                self.load_file_metadata(folder, filename, meta['column_names'], domain)
-
-        # Create the 'HAS_DATA' relationships between the 'Source Data Table' node and all the 'Source Data Row' nodes
-        self.link_nodes_on_matching_property_value(label1='Source Data Table', label2='Source Data Row',
-                                                prop_name='_domain_', prop_value=domain,
-                                                rel='HAS_DATA')
-        return df
-
-    # #TODO: to be moved to NeoInterface.load_df ?
-    # def load_df_clean_nan(self, label = "Source Data Row"):
-    #     q = f"""
-    #     MATCH (sdrl:{label})
-    #     WITH
-    #     """
-    #     if self.debug:
-    #         print("        Query : ", q)
-    #         print("        Query parameters: ", params)
-    #     self.query(q)
-
-    def load_file_metadata(self, folder:str, filename:str, columns: [str], domain = None) -> None:
-        """
-        It creates Neo4j nodes, to be used for metadata, with the following labels:
-            `Source Data Folder`, `Source Data Table`, `Source Data Column`,
-            and relationships HAS_TABLE and HAS_COLUMN among them
-
-        :param folder:      Name of directory where the file resides
-        :param filename:    Name (exclusive of path) of the file
-        :param columns:     List of field names
-        :param domain:      A string indicating a "data domain" (e.g. the name of the file with the original data)
-        :return:            None
-        """
-        q = f"""
-            MERGE (sdf:`Source Data Folder`{{_folder_:$folder}})                                 
-            MERGE (sdf)-[:HAS_TABLE]->(sdt:`Source Data Table`{{_folder_:$folder, _domain_:$domain, _filename_:$filename}})
-            WITH * UNWIND $columns as columnname
-            MERGE (sdt)-[:HAS_COLUMN]->(sdc:`Source Data Column`{{_folder_:$folder, _domain_:$domain, _columnname_:columnname}})
-            WITH DISTINCT sdf, sdt           
-            MATCH (sdr:`Source Data Row`{{_folder_:$folder, _domain_:$domain}}), (sdt)
-            MERGE (sdr)<-[:HAS_DATA]-(sdt)           
-        """
-        params = {'folder':folder, 'filename': filename, 'columns': columns, 'domain': domain}
-        res = self.query(q, params)
-        if self.debug:
-            print("        Query : ", q)
-            print("        Query parameters: ", params)
-
-
-    def load_folder(self, folder="", only_files=None, metadataonly = False, test_run = False):
-        """
-        Loop over all files in the folder, and load them as detailed in load_file()
-
-        :param folder:
-        :param only_files:
-        :param metadataonly:
-        :param test_run:
-        :return:
-        """
-        if not only_files:
-            only_files = []
-        self.load_df(df=pd.DataFrame([{'_folder_': folder}]), label="Source Data Folder", merge=True,
-                     primary_key='_folder_')
-        for filename in os.listdir(folder):
-            # if only_files is empty list, then loads all files
-            if (not only_files) or filename in only_files:
-                if self.verbose:
-                    print(f"Loading {filename}")
-                self.load_file(folder, filename, metadataonly = metadataonly, test_run = test_run)
-
-    def delete_source_data(self):
-        """
-        Deletes all (Non-reshaped) data
-        :return:
-        """
-        q = """
-        MATCH (sd)
-        WHERE sd:`Source Data Folder` OR sd:`Source Data Row` OR sd:`Source Data Table` OR sd:`Source Data Column`
-        DETACH DELETE sd
-        """
-        self.query(q)
-
-    def delete_file_data(self, folder: str, domain: str):
-        q = f"""
-                MATCH (folder:`Source Data Folder`{{_folder_:$folder}}),                           
-                (folder)-[:HAS_TABLE]->(file:`Source Data Table`{{_domain_:$domain}}),               
-                (file)-[:HAS_COLUMN]->(column:`Source Data Column`)
-                DETACH DELETE column
-                WITH DISTINCT folder, file
-                MATCH (file)-[:HAS_DATA]->(sdr:`Source Data Row`)
-                DETACH DELETE sdr
-                WITH DISTINCT folder, file
-                DETACH DELETE file
-                WITH DISTINCT folder
-                OPTIONAL MATCH (folder)-[r:HAS_TABLE]->()
-                WITH DISTINCT folder, count(r) as cnt
-                CALL apoc.do.when(
-                	cnt = 0,
-                	'DELETE $folder',
-                	'RETURN "keep"',
-                	{{folder: folder}}
-                ) 
-                YIELD value RETURN value
-            """
-        self.query(q, {'folder': folder, 'domain': domain})
-
-
-    def load_file_distinct_values_for_columns(self, folder: str, filename: str, column_list: list, test_run = False):
-        """
-        To be used when one doesn't want to load all the data,
-        but just distinct items in a column (stored w/ a relationship to its property)
-
-        This operation sits in-between the models and the data loading.
-
-        :param folder:
-        :param filename:
-        :param column_list:
-        :param test_run:
-        :return:
-        """
-        df = self.load_file(folder, filename, metadataonly = False, load_to_neo= False, test_run = test_run)
-        for column, property_id in column_list:
-            values = [x for x in set(df[column]) if not x is None]
-            q = """             
-            MATCH (property) 
-            WHERE id(property) = $property_id
-            WITH *, $values as values UNWIND values as value
-            MERGE (property)-[:HAS_PROPERTY_VALUE]->(:PropertyValue{value:value})
-            """
-            self.query(q, {'property_id': property_id, 'values': values})
-
-    @staticmethod
-    def convert_datetime_columns(df: pd.DataFrame, date_format: str, datetime_col_regex='^.*DTM$',
-                                 date_col_regex='^.*DT$'):
-        """
-        Convert columns in df that match dtcol_regex from SAS integer dates to pandas Timestamps (equivalent to python
-        datetimes).
-        :param df: input df
-        :param date_format: String of date format to convert from. E.g. 'sas', 'unix'
-        :param datetime_col_regex: regex for datetime columns
-        :param date_col_regex: regex for date columns
-        :return: modified df
-        """
-
-        assert date_format.lower() in ['sas', 'unix'], f"Unsupported date_format {date_format}"
-
-        # setup regex column matching for datetime/date columns
-        r_datetime = re.compile(pattern=datetime_col_regex)
-        date_time_cols = list(filter(r_datetime.match, df.columns))
-        r_date = re.compile(pattern=date_col_regex)
-        date_cols = list(filter(r_date.match, df.columns))
-
-        if date_format.lower() == 'sas':
-            # setup conversion function for sas datetimes/dates
-            def f(x, unit):
-                return pd.to_timedelta(x, unit=unit) + pd.Timestamp(year=1960, month=1, day=1)
-
-        if date_format.lower() == 'unix':
-            # setup conversion function for unix datetimes/dates
-            def f(x, unit):
-                return pd.to_datetime(x, unit=unit)
-
-        for col in date_time_cols:
-            # for all datetime columns convert using unit='s' (seconds)
-            df[col] = df[col].apply(
-                lambda x: f(x, 's'))
-
-        for col in date_cols:
-            # for all date columns convert using unit='D' (days)
-            df[col] = df[col].apply(
-                lambda x: f(x, 'D'))
-
-        return df
+import neointerface
+import pandas as pd
+import re
+import pyreadstat       # A library that was open-sourced by Roche
+import pyreadr          # Used for the RDA format
+import os
+from logger.logger import logger
+
+
+class FileDataLoader(neointerface.NeoInterface):
+    """
+    Load data into Neo4j, with support for the following input formats:
+            rda, xpt, sas7bdat, xls, xlsx
+    A goal is to harmonize those formats.
+    """
+
+    def __init__(self, domain_dict = None, *args, **kwargs):
+        """
+        :param domain_dict: dictionary with file names as keys and domain to be assigned as values
+                            (e.g. {'dm_xyz.sas7bdat': 'DM', 'ae_xyz.sas7bdat': 'AE'} )
+        :param verbose:     Flag indicating whether ANY logs will be displayed
+        :param debug:       Flag indicating whether logs will be in debug or info mode
+        :param args:        other arguments
+        :param kwargs:      other keyword arguments
+        """
+        self.domain_dict = domain_dict
+        super().__init__(*args, **kwargs)
+
+
+    def read_file(self, folder:str, filename:str, sheet_name=0, query=None, metadataonly = False, test_run = False,
+                  colcharsbl =r'[^A-Za-z0-9_]+'):
+        """
+        Read in an external file as a Pandas data frame.
+        Can read in file types: rda, xpt, sas7bdat, xls, csv
+        It can OPTIONALLY only retrieve the metadata from the source file.
+
+        Note: nothing is actually loaded into Neo4j
+
+        It returns a Pandas data frame, and the metadata.
+
+        In case of error (such as an unsupported file format), an Exception is raised.
+
+        :param folder:          Name of directory where the file to load resides
+        :param filename:        Name (exclusive of path) of file to load
+        :param sheet_name       Only for xls and xlsx - name of the sheet to load
+        :param query            If not None apply a df.query on the dataframe being read
+        :param metadataonly:    If True then only the folder, filename, and column names are imported
+        :param test_run:        If True, only read the first 100 rows (Not applicable if the flag metadataonly is True)
+        :param colcharsbl:      The column names of the input files are renamed in such a way that the symbols
+                                    specified by the regex pattern are excluded
+                                    (e.g. for cleaning special characters in the colnames of excel files)
+                                    EXAMPLE: r'[^A-Za-z0-9_]+' will only keep A-Z, a-z, 0-9 and the underscore
+                                    TODO: Perhaps default it to None, and if not None, then apply it
+                                          regardless of the file extension (currently, only applied to Excel files)
+
+        :return:                 The pair (Pandas data frame, metadata)
+                                    EXAMPLE of the Pandas data frame:
+                                              STUDYID     SITEID   ...    BIRTHDATE
+                                        0    mid987650  214356.0   ...   1983-06-30
+                                        1    mid987650  214356.0   ...   1956-06-30
+
+                                    EXAMPLE of a value for meta:
+                                        {'column_names': ['STUDYID', 'SITEID', 'BIRTHDATE']}
+        """
+        assert query is None or isinstance(query, str)
+
+        ext = filename.split(".")[-1]               # Extract the filename extension (e.g. "rda")
+
+        # Special processing for the various file formats we support
+        # Set df to the Pandas dataframe, and meta to the dictionary {'column_names' : LIST_OF_COLUMN_NAMES_IN_DATA}
+        if ext in ["sas7bdat"]:
+            df, meta = pyreadstat.read_sas7bdat(os.path.join(folder, filename), metadataonly = metadataonly)
+            meta = meta.__dict__
+        elif ext in ["xpt"]:
+            df, meta = pyreadstat.read_xport(os.path.join(folder, filename), metadataonly = metadataonly)
+            meta = meta.__dict__
+        elif ext in ["rda"]:
+            r_result = pyreadr.read_r(os.path.join(folder, filename))
+            name, df = r_result.popitem(last=False)
+            meta = {'column_names': list(df.columns)}
+            if metadataonly:
+                df = pd.DataFrame(columns = df.columns)
+        elif ext in ["xls", "xlsx"]:
+            if ext == "xls":
+                df = pd.read_excel(os.path.join(folder, filename), sheet_name=sheet_name)
+            elif ext == "xlsx":
+                df = pd.read_excel(os.path.join(folder, filename), engine='openpyxl', sheet_name=sheet_name)
+            df.columns = [re.sub(colcharsbl, '', re.sub(r'\s', '_', s)) for s in df.columns] #TODO: maybe apply to ALL data types
+            meta = {'column_names': list(df.columns)}
+            if metadataonly:
+                df = pd.DataFrame(columns = df.columns)
+        elif ext in ["csv"]:
+            # Todo: N.B CDISC Library provides csv files where values are quoted (i.e. "variabel 1","Another variable")
+            #  Therefore option quotechar is used, which means that " will not appear in data.
+            #  Have not tested or thought of scenarios what would happen if values are not quoted
+            df = pd.read_csv(os.path.join(folder, filename), quotechar='"')
+            meta = {'column_names': list(df.columns)}
+            if metadataonly:
+                df = pd.DataFrame(columns = df.columns)
+        else:
+            raise Exception(f"Unsupported file format - unrecognized filename extension: {ext}")
+
+        # EXAMPLE of a value for meta:
+        #   {'column_names': ['STUDYID', 'SITEID', 'AGE']}
+
+        if test_run:
+            df = df.head(100)   # Only use the first 100 rows
+
+        # since pandas sets missing strings to float NaN we actively replace na with ''
+        col_obj = [col for col in df.columns if df[col].dtype == 'object']
+        df[col_obj] = df[col_obj].fillna(value='')
+
+        if query:
+            df = df.query(query)
+
+        return (df, meta)
+
+
+    def load_file(self, folder:str, filename:str, sheet_name=0, query=None, metadataonly = False, dataonly = False, test_run = False,
+                        load_to_neo = True, colcharsbl =r'[^A-Za-z0-9_]+'):
+        """
+        Read in an external file as a Pandas data frame.
+
+        Can read in file types: rda, xpt, sas7bdat, xls, csv
+        It can OPTIONALLY only retrieve the metadata from the source file.
+        It OPTIONALLY loads into Neo4j the metadata (creating 3 node labels: `Source Data Folder`, `Source Data Table`, `Source Data Column`),
+                and, if imported, the data (creating nodes with the label `Source Data Row`,
+                                            and also adding an extra field named `_domain_` to store the domain.)
+                Whenever data is loaded to Neo4j, the following relationships are also created:
+                    1) `Source Data Folder` -[:HAS_TABLE]-> `Source Data Table`
+                    2) `Source Data Table` -[:HAS_COLUMN]-> to all `Source Data Column` nodes
+                    3) 'Source Data Table' -[:HAS_DATA]-> to all 'Source Data Row' nodes
+
+        "DOMAIN" - term used for the capitalized version of the basename of the datafile, for provenance information
+
+        It returns a Pandas data frame.
+
+        In case of error (such as an unsupported file format), an Exception is raised.
+
+        :param folder:          Name of directory where the file to load resides
+        :param filename:        Name (exclusive of path) of file to load
+        :param sheet_name       Only for xls and xlsx - name of the sheet to load
+        :param query:           A parameter to be passed to read_file
+        :param metadataonly:    If True then only the folder, filename, and column names are imported
+        :param dataonly:
+        :param test_run:        If True, only read the first 100 rows (Not applicable if the flag metadataonly is True)
+        :param load_to_neo:     If True then data (INCL. metadata) is loaded into Neo4j nodes with `Source Data Row` labels
+        :param colcharsbl:      The column names of the input files are renamed in such a way that the symbols
+                                    specified by the regex pattern are excluded
+                                    (e.g. for cleaning special characters in the colnames of excel files)
+                                    EXAMPLE: r'[^A-Za-z0-9_]+' will only keep A-Z, a-z, 0-9 and the underscore
+                                    TODO: Perhaps default it to None, and if not None, then apply it
+                                          regardless of the file extension (currently, only applied to Excel files)
+
+        :return:                 A Pandas data frame.  EXAMPLE:
+                                             STUDYID    SITEID    USUBJID  ...        TRTETM   BRTHDT      BRTHDTC
+                                        0    mid987650  214356.0  987650.000001  ...  33420.0  1983-06-30  1983.0
+                                        1    mid987650  214356.0  987650.000002  ...  33420.0  1956-06-30  1956.0
+        """
+        (df, meta) = self.read_file(folder=folder, filename=filename, sheet_name=sheet_name, query=query, metadataonly=metadataonly,
+                                    test_run=test_run, colcharsbl=colcharsbl)
+
+        fn = ".".join(filename.split(".")[:-1])     # The filename excluding the dot and the extension suffix
+        ext = filename.split(".")[-1]
+
+        if ext in ["xls", "xlsx"] and isinstance(sheet_name, str):
+            domain = f"{fn}.{sheet_name}".upper()
+        else:
+            domain = fn.upper()
+            
+        if self.domain_dict:
+            if filename in self.domain_dict.keys():
+                domain = self.domain_dict[filename]
+
+        # If the dataframe isn't empty, and it was requested to load the data into Neo4j,
+        #       create nodes with the label `Source Data Row`
+        if not df.empty and not metadataonly:
+            # Timestamp data formats are not supported in neo4j as parameters to the query; therefore, changing to str
+            # This does not cause trouble with SDTM data as dates are stored as str ther,e but would cause problems with
+            # raw and ADaM data
+            # TODO: get rid of this temporary workaround
+            for i, dtype in enumerate(df.dtypes):
+                if not dtype in ['O', 'float64', 'int64']:
+                    df[df.columns[i]] = df[df.columns[i]].astype(str)
+
+            # loading data
+            # df = df.assign(_filename_ = filename)
+            df = df.assign(_domain_=domain)  # Add new column, to keep track of the data provenance
+            df = df.assign(_filename_=filename)  # Add new column, to keep track of the data provenance
+            df = df.assign(_folder_=folder)  # Add new column, to keep track of the data provenance
+            if load_to_neo:
+                self.load_df(df=df, label="Source Data Row", merge=False)
+                # self.load_df_clean_nan()
+
+        # If the meta dictionary contains, as expected, the key 'column_names',
+        #       and if the data (and metadata) is to be loaded into Neo4j,
+        #       then handle the loading of the metadata
+        if not dataonly:
+            if 'column_names' in meta.keys() and load_to_neo:
+                self.load_file_metadata(folder, filename, meta['column_names'], domain)
+
+        # Create the 'HAS_DATA' relationships between the 'Source Data Table' node and all the 'Source Data Row' nodes
+        self.link_nodes_on_matching_property_value(label1='Source Data Table', label2='Source Data Row',
+                                                prop_name='_domain_', prop_value=domain,
+                                                rel='HAS_DATA')
+        return df
+
+    # #TODO: to be moved to NeoInterface.load_df ?
+    # def load_df_clean_nan(self, label = "Source Data Row"):
+    #     q = f"""
+    #     MATCH (sdrl:{label})
+    #     WITH
+    #     """
+    #     if self.debug:
+    #         print("        Query : ", q)
+    #         print("        Query parameters: ", params)
+    #     self.query(q)
+
+    def load_file_metadata(self, folder:str, filename:str, columns: [str], domain = None) -> None:
+        """
+        It creates Neo4j nodes, to be used for metadata, with the following labels:
+            `Source Data Folder`, `Source Data Table`, `Source Data Column`,
+            and relationships HAS_TABLE and HAS_COLUMN among them
+
+        :param folder:      Name of directory where the file resides
+        :param filename:    Name (exclusive of path) of the file
+        :param columns:     List of field names
+        :param domain:      A string indicating a "data domain" (e.g. the name of the file with the original data)
+        :return:            None
+        """
+        q = f"""
+            MERGE (sdf:`Source Data Folder`{{_folder_:$folder}})                                 
+            MERGE (sdf)-[:HAS_TABLE]->(sdt:`Source Data Table`{{_folder_:$folder, _domain_:$domain, _filename_:$filename}})
+            WITH * UNWIND $columns as columnname
+            MERGE (sdt)-[:HAS_COLUMN]->(sdc:`Source Data Column`{{_folder_:$folder, _domain_:$domain, _columnname_:columnname}})
+            WITH DISTINCT sdf, sdt           
+            MATCH (sdr:`Source Data Row`{{_folder_:$folder, _domain_:$domain}}), (sdt)
+            MERGE (sdr)<-[:HAS_DATA]-(sdt)           
+        """
+        params = {'folder':folder, 'filename': filename, 'columns': columns, 'domain': domain}
+        res = self.query(q, params)
+        if self.verbose:
+            logger.debug(f"        Query : {q}")
+            logger.debug(f"        Query parameters: {params}")
+
+
+    def load_folder(self, folder="", only_files=None, metadataonly = False, test_run = False):
+        """
+        Loop over all files in the folder, and load them as detailed in load_file()
+
+        :param folder:
+        :param only_files:
+        :param metadataonly:
+        :param test_run:
+        :return:
+        """
+        if not only_files:
+            only_files = []
+        self.load_df(df=pd.DataFrame([{'_folder_': folder}]), label="Source Data Folder", merge=True,
+                     primary_key='_folder_')
+        for filename in os.listdir(folder):
+            # if only_files is empty list, then loads all files
+            if (not only_files) or filename in only_files:
+                if self.verbose:
+                    logger.info(f"Loading {filename}")
+                self.load_file(folder, filename, metadataonly = metadataonly, test_run = test_run)
+
+    def delete_source_data(self):
+        """
+        Deletes all (Non-reshaped) data
+        :return:
+        """
+        q = """
+        MATCH (sd)
+        WHERE sd:`Source Data Folder` OR sd:`Source Data Row` OR sd:`Source Data Table` OR sd:`Source Data Column`
+        DETACH DELETE sd
+        """
+        self.query(q)
+
+    def delete_file_data(self, folder: str, domain: str):
+        q = f"""
+                MATCH (folder:`Source Data Folder`{{_folder_:$folder}}),                           
+                (folder)-[:HAS_TABLE]->(file:`Source Data Table`{{_domain_:$domain}}),               
+                (file)-[:HAS_COLUMN]->(column:`Source Data Column`)
+                DETACH DELETE column
+                WITH DISTINCT folder, file
+                MATCH (file)-[:HAS_DATA]->(sdr:`Source Data Row`)
+                DETACH DELETE sdr
+                WITH DISTINCT folder, file
+                DETACH DELETE file
+                WITH DISTINCT folder
+                OPTIONAL MATCH (folder)-[r:HAS_TABLE]->()
+                WITH DISTINCT folder, count(r) as cnt
+                CALL apoc.do.when(
+                	cnt = 0,
+                	'DELETE $folder',
+                	'RETURN "keep"',
+                	{{folder: folder}}
+                ) 
+                YIELD value RETURN value
+            """
+        self.query(q, {'folder': folder, 'domain': domain})
+
+
+    def load_file_distinct_values_for_columns(self, folder: str, filename: str, column_list: list, test_run = False):
+        """
+        To be used when one doesn't want to load all the data,
+        but just distinct items in a column (stored w/ a relationship to its property)
+
+        This operation sits in-between the models and the data loading.
+
+        :param folder:
+        :param filename:
+        :param column_list:
+        :param test_run:
+        :return:
+        """
+        df = self.load_file(folder, filename, metadataonly = False, load_to_neo= False, test_run = test_run)
+        for column, property_id in column_list:
+            values = [x for x in set(df[column]) if not x is None]
+            q = """             
+            MATCH (property) 
+            WHERE id(property) = $property_id
+            WITH *, $values as values UNWIND values as value
+            MERGE (property)-[:HAS_PROPERTY_VALUE]->(:PropertyValue{value:value})
+            """
+            self.query(q, {'property_id': property_id, 'values': values})
+
+    @staticmethod
+    def convert_datetime_columns(df: pd.DataFrame, date_format: str, datetime_col_regex='^.*DTM$',
+                                 date_col_regex='^.*DT$'):
+        """
+        Convert columns in df that match dtcol_regex from SAS integer dates to pandas Timestamps (equivalent to python
+        datetimes).
+        :param df: input df
+        :param date_format: String of date format to convert from. E.g. 'sas', 'unix'
+        :param datetime_col_regex: regex for datetime columns
+        :param date_col_regex: regex for date columns
+        :return: modified df
+        """
+
+        assert date_format.lower() in ['sas', 'unix'], f"Unsupported date_format {date_format}"
+
+        # setup regex column matching for datetime/date columns
+        r_datetime = re.compile(pattern=datetime_col_regex)
+        date_time_cols = list(filter(r_datetime.match, df.columns))
+        r_date = re.compile(pattern=date_col_regex)
+        date_cols = list(filter(r_date.match, df.columns))
+
+        if date_format.lower() == 'sas':
+            # setup conversion function for sas datetimes/dates
+            def f(x, unit):
+                return pd.to_timedelta(x, unit=unit) + pd.Timestamp(year=1960, month=1, day=1)
+
+        if date_format.lower() == 'unix':
+            # setup conversion function for unix datetimes/dates
+            def f(x, unit):
+                return pd.to_datetime(x, unit=unit)
+
+        for col in date_time_cols:
+            # for all datetime columns convert using unit='s' (seconds)
+            df[col] = df[col].apply(
+                lambda x: f(x, 's'))
+
+        for col in date_cols:
+            # for all date columns convert using unit='D' (days)
+            df[col] = df[col].apply(
+                lambda x: f(x, 'D'))
+
+        return df
```

### Comparing `tab2neo-1.2.1.0/data_loaders/sql_server_data_loader.py` & `tab2neo-1.2.5.0/data_loaders/sql_server_data_loader.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-import neointerface
-import os
-import pandas as pd
-
-class SQLServerDataLoader(neointerface.NeoInterface):
-    def __init__(self,
-                 sqldburl = os.environ.get("SQL_SERVER"),
-                 sqldbname = os.environ.get("SQL_DATABASE"),
-                 sqluser = os.environ.get("SQL_USER_ID"),
-                 sqlpassword = os.environ.get("SQL_PASSWORD"),
-                 *args, **kwargs):
-        self.sqldbname = sqldbname
-        self.sqluser = sqluser
-        self._sqlpassword = sqlpassword
-        self._con = f"jdbc:sqlserver://{sqldburl};databaseName={self.sqldbname};user={self.sqluser};password={self._sqlpassword};"
-        super().__init__(*args, **kwargs)
-        if self.autoconnect:
-            self.query("call db.clearQueryCaches()")
-
-    def sql_query(self, sqlq:str):
-        q = "CALL apoc.load.jdbc($con, $sqlq) YIELD row RETURN row"
-        params = {
-            "sqlq": sqlq,
-            "con": self._con
-        }
-        return pd.DataFrame([x['row'] for x in self.query(q, params)])
-
-    def sql_get_tables(self):
-        tables_df = self.sql_query("SELECT * FROM information_schema.tables;")
+import neointerface
+import os
+import pandas as pd
+
+class SQLServerDataLoader(neointerface.NeoInterface):
+    def __init__(self,
+                 sqldburl = os.environ.get("SQL_SERVER"),
+                 sqldbname = os.environ.get("SQL_DATABASE"),
+                 sqluser = os.environ.get("SQL_USER_ID"),
+                 sqlpassword = os.environ.get("SQL_PASSWORD"),
+                 *args, **kwargs):
+        self.sqldbname = sqldbname
+        self.sqluser = sqluser
+        self._sqlpassword = sqlpassword
+        self._con = f"jdbc:sqlserver://{sqldburl};databaseName={self.sqldbname};user={self.sqluser};password={self._sqlpassword};"
+        super().__init__(*args, **kwargs)
+        if self.autoconnect:
+            self.query("call db.clearQueryCaches()")
+
+    def sql_query(self, sqlq:str):
+        q = "CALL apoc.load.jdbc($con, $sqlq) YIELD row RETURN row"
+        params = {
+            "sqlq": sqlq,
+            "con": self._con
+        }
+        return pd.DataFrame([x['row'] for x in self.query(q, params)])
+
+    def sql_get_tables(self):
+        tables_df = self.sql_query("SELECT * FROM information_schema.tables;")
         return tables_df
```

### Comparing `tab2neo-1.2.1.0/data_providers/data_provider.py` & `tab2neo-1.2.5.0/data_providers/data_provider.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,240 +1,253 @@
-import logging
-import pandas as pd
-from neointerface import NeoInterface
-from logger.logger import logger
-from model_managers import ModelManager
-from query_builders.query_builder import QueryBuilder
-
-logger.setLevel(logging.INFO)
-
-
-class DataProvider(NeoInterface):
-    """
-    Version 2
-    To use the data already in the database (such as the data after the transformations with ModelApplier v2),
-    for various purposes - such as to feed the User Interface.
-    """
-    OCLASS_MARKER = '**'
-
-    def __init__(self, *args, **kwargs):
-        self.qb = QueryBuilder()
-        self.mm = ModelManager(*args, **kwargs)
-        super().__init__(*args, **kwargs)
-        if self.verbose:
-            print(f"---------------- {self.__class__} initialized -------------------")
-
-    def check_schema(self, labels: list, rels: list):
-        for label in labels:
-            q = "MATCH " + self.qb.generate_1match_schema_check(label=label) + " RETURN *"
-            res = self.query(q)
-            assert res, f"Class {label} not found in the schema"
-        for rel in rels:
-            q1, params1 = self.qb.generate_1rel_schema_check(rel, subclass_dir=">")
-            q1 = "MATCH " + q1 + " RETURN * LIMIT 1"
-            res1 = self.query(q1, params1)
-            q2, params2 = self.qb.generate_1rel_schema_check(rel, subclass_dir="<")
-            q2 = "MATCH " + q2 + " RETURN * LIMIT 1"
-            res2 = self.query(q2, params2)
-            assert res1 or res2, f"Relationship {rel} not found in the schema"
-
-    def get_data(self, labels: list, rels: list = None, where_map=None, return_nodeid=False):
-        """
-        A typical get_data_generic call with nodes with multiple parameters and repeating property names btw labels
-        :return: pd.DataFrame
-        """
-        self.get_data_generic(
-            labels=labels,
-            rels=rels,
-            infer_rels=False,
-            where_map=where_map,
-            allow_unrelated_subgraphs=False,
-            use_shortlabel=False,
-            return_nodeid=return_nodeid,
-            return_propname=True,
-            check_schema=False,
-            limit=None,
-            return_q_and_dict=False)
-
-    def get_data_cld(self,
-                     labels: list,
-                     rels: list = None,
-                     where_map=None,
-                     where_rel_map=None,
-                     return_nodeid=True,
-                     return_termorder=False,
-                     return_class_uris=False):
-        """
-        A typical get_data_generic call for CLD project:
-            Class-Relationship schema is used and shortlabel is used as the
-            1 property per class named rdfs:label
-        output df column names
-        :return: pd.DataFrame, str, dict
-        """
-        return self.get_data_generic(
-            labels=labels,
-            rels=rels,
-            infer_rels=True,
-            where_map=where_map,
-            where_rel_map=where_rel_map,
-            allow_unrelated_subgraphs=False,
-            use_shortlabel=True,
-            return_nodeid=return_nodeid,
-            return_propname=False,
-            return_termorder=return_termorder,
-            return_class_uris=return_class_uris,
-            only_props=["rdfs:label"],
-            check_schema=False,
-            limit=None,
-            return_q_and_dict=True)
-
-    def get_data_generic(
-            self,
-            labels: list,
-            rels: list = None,  # [{'from':<label1>, 'to':<label2>, 'type':<type>}, ...]
-            labels_to_pack=None,  # {'label1': 'label1_def', 'label2': 'label2_def', 'label3': [term1, term2, ...], ...}
-            infer_rels=False,
-            where_map=None,
-            where_rel_map=None,
-            allow_unrelated_subgraphs: bool = False,
-            use_shortlabel: bool = False,
-            use_rel_labels: bool = True,
-            # use_rel_labels only active when use_shortlabel == True; the short_label of the [:TO] class is updated with the one in Relationship.short_label
-            return_nodeid: bool = True,
-            return_propname: bool = True,
-            return_termorder: bool = False,
-            only_props: list = None,  # to return only specified properties. If None - return all
-            return_disjoint: bool = False,  # to return dict with Class as key and distinct values as values set to True
-            return_class_uris: bool = False,  # to return dict with Class as key and distinct values as values set to True
-            check_schema=False,
-            limit=None,
-            return_q_and_dict=False
-    ):
-        if only_props:
-            if isinstance(only_props, str):
-                only_props = [only_props]
-        assert len(labels) > 0 or len(rels) > 0
-        if rels:
-            for rel in rels:
-                assert isinstance(rel, dict)
-                for key in ['from', 'to']:
-                    assert isinstance(rel.get(key), str) and len(rel.get(key)) > 0
-        # #making sure all labels from the rels are in labels
-        labels = self.qb.enrich_labels_from_rels(labels=labels, rels=rels, oclass_marker=self.OCLASS_MARKER)
-        # #creating a list of labels without an optional match sign (**)
-        labels_clean = []
-        for label in labels:
-            assert isinstance(label, str)
-            if label.endswith(self.OCLASS_MARKER):
-                labels_clean.append(label[:-len(self.OCLASS_MARKER)])
-            else:
-                labels_clean.append(label)
-        # #empty where_map if None
-        if not where_map:
-            where_map = {}
-        if not where_rel_map:
-            where_rel_map = {}
-        # #infer rels from the schema if rels are not provided and infer_rels parameter is True
-
-        if not rels:
-            if infer_rels:
-                rels = self.mm.infer_rels(labels=labels, oclass_marker=self.OCLASS_MARKER)
-            else:
-                rels = []
-        # #filling the rel.type with the default relationship type (HAS_ ...)
-        rels = self.mm.gen_default_reltypes_list(rels)
-        # #checking that the requested Class and Relationship nodes exist in the schema
-        if check_schema:
-            self.check_schema(labels=labels_clean, rels=rels)
-        # #checking that there are not unrelated subgraphse if allow_unrelated_subgraphs set to True
-        if not allow_unrelated_subgraphs:
-            assert self.qb.check_connectedness(labels=labels_clean, rels=rels), \
-                f"Diconnected subgraphs found in {(labels_clean, rels)}"
-        # #building queries to run against the database
-        q_res, q, params = None, None, None
-        q_body_list = []
-        if only_props:
-            params = {'only_props': only_props}
-        else:
-            params = {}
-        # #if any labels are marked for optional match - separately generating a query for each MATCH statement
-        for i, (_labels, _rels) in enumerate(
-                self.qb.split_out_optional(labels=labels, rels=rels, oclass_marker=self.OCLASS_MARKER)):
-            # schema check for each subquery:
-            if not allow_unrelated_subgraphs:
-                assert self.qb.check_connectedness(labels=_labels, rels=_rels), \
-                    f"Diconnected subgraphs found in {(_labels, _rels)}"
-
-            # building sub-query
-            _where_map = {k: i for k, i in where_map.items() if k in _labels}
-            _where_rel_map = {k: i for k, i in where_rel_map.items() if k in _labels}
-            # TODO: validate the insides of where_rel_map only contain labels in _labels
-
-            if use_shortlabel:
-                _labels, _rels, _labels_to_pack, _where_map, _where_rel_map = self.mm.translate_to_shortlabel(
-                    _labels,
-                    _rels,
-                    labels_to_pack,
-                    _where_map,
-                    _where_rel_map,
-                    use_rel_labels=use_rel_labels
-                )
-            # ------------------------------ QUERY BUILD ------------------------------------#
-            (_q_body, _params) = self.qb.generate_query_body(
-                labels=_labels,
-                rels=_rels,
-                match=("MATCH" if i == 0 else "OPTIONAL MATCH"),
-                where_map=_where_map,
-                where_rel_map=_where_rel_map
-            )
-            q_body_list.append(_q_body)
-            params = {**params, **_params}
-
-        q_body = "\n".join(q_body_list)
-        if use_shortlabel:
-            translated = self.mm.translate_to_shortlabel(labels_clean, rels, labels_to_pack, {},
-                                                         use_rel_labels=use_rel_labels)
-            labels_clean = [dct['short_label'] for dct in translated[0]]
-            rels = translated[1]
-            labels_to_pack = translated[2]
-
-        # print(f'Labels to Pack (get_data_generic): {labels_to_pack}')
-
-        q_call = "\n" + self.qb.generate_call(
-            labels=labels_clean,
-            rels=rels,
-            labels_to_pack=labels_to_pack,
-            only_props=only_props
-        )
-
-        q_with = "\n" + self.qb.generate_with(
-            labels=labels_clean,
-            labels_to_pack=labels_to_pack,
-            only_props=only_props
-        )
-
-        q_return = "\n" + self.qb.generate_return(
-            labels=labels_clean,
-            labels_to_pack=labels_to_pack,
-            return_nodeid=return_nodeid,
-            return_propname=return_propname,
-            return_termorder=return_termorder,
-            return_class_uris=return_class_uris,
-            only_props=only_props,
-            return_disjoint=return_disjoint
-        )
-        q_limit = (f" LIMIT {str(limit)}" if limit else "")
-        q = q_body + q_call + q_with + q_return + q_limit
-        # ------------------------------ QUERY RUN ------------------------------------#
-        if self.verbose:
-            logger.info(f"QUERY: {q}")
-            logger.info(f"PARAMS: {params}")
-        q_res = self.query(q, params)
-        if return_disjoint:
-            res = q_res
-        else:
-            res = pd.DataFrame([r['all'] for r in q_res])
-        # TODO: rename rdfs:label to short_label of each class
-        if return_q_and_dict:
-            return res, q, params
-        else:
-            return res
+import logging
+import pandas as pd
+from neointerface import NeoInterface
+from logger.logger import logger
+from model_managers import ModelManager
+from query_builders.query_builder import QueryBuilder
+
+
+class DataProvider(NeoInterface):
+    """
+    Version 2
+    To use the data already in the database (such as the data after the transformations with ModelApplier v2),
+    for various purposes - such as to feed the User Interface.
+    """
+    OCLASS_MARKER = '**'
+
+    def __init__(self, *args, **kwargs):
+        self.qb = QueryBuilder()
+        self.mm = ModelManager(*args, **kwargs)
+        super().__init__(*args, **kwargs)
+        if self.verbose:
+            logger.info(f"---------------- {self.__class__} initialized -------------------")
+
+    def check_schema(self, labels: list, rels: list):
+        for label in labels:
+            q = "MATCH " + self.qb.generate_1match_schema_check(label=label) + " RETURN *"
+            res = self.query(q)
+            assert res, f"Class {label} not found in the schema"
+        for rel in rels:
+            q1, params1 = self.qb.generate_1rel_schema_check(rel, subclass_dir=">")
+            q1 = "MATCH " + q1 + " RETURN * LIMIT 1"
+            res1 = self.query(q1, params1)
+            q2, params2 = self.qb.generate_1rel_schema_check(rel, subclass_dir="<")
+            q2 = "MATCH " + q2 + " RETURN * LIMIT 1"
+            res2 = self.query(q2, params2)
+            assert res1 or res2, f"Relationship {rel} not found in the schema"
+
+    def get_data(self, labels: list, rels: list = None, where_map=None, return_nodeid=False):
+        """
+        A typical get_data_generic call with nodes with multiple parameters and repeating property names btw labels
+        :return: pd.DataFrame
+        """
+        return self.get_data_generic(
+            labels=labels,
+            rels=rels,
+            infer_rels=False,
+            where_map=where_map,
+            allow_unrelated_subgraphs=False,
+            use_shortlabel=False,
+            return_nodeid=return_nodeid,
+            return_propname=True,
+            check_schema=False,
+            limit=None,
+            return_q_and_dict=False)
+
+    def get_data_cld(self,
+                     labels: list,
+                     rels: list = None,
+                     where_map=None,
+                     where_rel_map=None,
+                     return_nodeid=True,
+                     return_termorder=False,
+                     return_class_uris=False):
+        """
+        A typical get_data_generic call for CLD project:
+            Class-Relationship schema is used and shortlabel is used as the
+            1 property per class named rdfs:label
+        output df column names
+        :return: pd.DataFrame, str, dict
+        """
+        return self.get_data_generic(
+            labels=labels,
+            rels=rels,
+            infer_rels=True,
+            where_map=where_map,
+            where_rel_map=where_rel_map,
+            allow_unrelated_subgraphs=False,
+            use_shortlabel=True,
+            return_nodeid=return_nodeid,
+            return_propname=False,
+            return_termorder=return_termorder,
+            return_class_uris=return_class_uris,
+            only_props=["rdfs:label"],
+            check_schema=False,
+            limit=None,
+            return_q_and_dict=True)
+
+    def get_data_generic(
+            self,
+            labels: list,
+            rels: list = None,  # [{'from':<label1>, 'to':<label2>, 'type':<type>}, ...]
+            labels_to_pack=None,  # {'label1': 'label1_def', 'label2': 'label2_def', 'label3': [term1, term2, ...], ...}
+            infer_rels=False,
+            where_map=None,
+            where_rel_map=None,
+            allow_unrelated_subgraphs: bool = False,
+            use_shortlabel: bool = False,
+            use_rel_labels: bool = True,
+            # use_rel_labels only active when use_shortlabel == True; the short_label of the [:TO] class is updated with the one in Relationship.short_label
+            return_nodeid: bool = True,
+            return_propname: bool = True,
+            return_termorder: bool = False,
+            only_props: list = None,  # to return only specified properties. If None - return all
+            return_disjoint: bool = False,  # to return dict with Class as key and distinct values as values set to True
+            return_class_uris: bool = False,  # to return dict with Class as key and distinct values as values set to True
+            check_schema=False,
+            limit=None,
+            return_q_and_dict=False,
+            pivot: bool = False
+    ):
+        if only_props:
+            if isinstance(only_props, str):
+                only_props = [only_props]
+        assert len(labels) > 0 or len(rels) > 0
+        if rels:
+            for rel in rels:
+                assert isinstance(rel, dict)
+                for key in ['from', 'to']:
+                    assert isinstance(rel.get(key), str) and len(rel.get(key)) > 0
+        # #making sure all labels from the rels are in labels
+        labels = self.qb.enrich_labels_from_rels(labels=labels, rels=rels, oclass_marker=self.OCLASS_MARKER)
+        # #creating a list of labels without an optional match sign (**)
+        labels_clean = []
+        for label in labels:
+            assert isinstance(label, str)
+            if label.endswith(self.OCLASS_MARKER):
+                labels_clean.append(label[:-len(self.OCLASS_MARKER)])
+            else:
+                labels_clean.append(label)
+        # #empty where_map if None
+        if not where_map:
+            where_map = {}
+        if not where_rel_map:
+            where_rel_map = {}
+        # #infer rels from the schema if rels are not provided and infer_rels parameter is True
+
+        if not rels:
+            if infer_rels:
+                rels = self.mm.infer_rels(labels=labels, oclass_marker=self.OCLASS_MARKER)
+            else:
+                rels = []
+        # #filling the rel.type with the default relationship type (HAS_ ...)
+        rels = self.mm.gen_default_reltypes_list(rels)
+        # #checking that the requested Class and Relationship nodes exist in the schema
+        if check_schema:
+            self.check_schema(labels=labels_clean, rels=rels)
+        # #checking that there are not unrelated subgraphse if allow_unrelated_subgraphs set to True
+        if not allow_unrelated_subgraphs:
+            assert self.qb.check_connectedness(labels=labels_clean, rels=rels), \
+                f"Diconnected subgraphs found in {(labels_clean, rels)}"
+        # #building queries to run against the database
+        q_res, q, params = None, None, None
+        q_body_list = []
+        if only_props:
+            params = {'only_props': only_props}
+        else:
+            params = {}
+        # #if any labels are marked for optional match - separately generating a query for each MATCH statement
+        for i, (_labels, _rels) in enumerate(
+                self.qb.split_out_optional(labels=labels, rels=rels, oclass_marker=self.OCLASS_MARKER)):
+            # schema check for each subquery:
+            if not allow_unrelated_subgraphs:
+                assert self.qb.check_connectedness(labels=_labels, rels=_rels), \
+                    f"Diconnected subgraphs found in {(_labels, _rels)}"
+
+            # building sub-query
+            _where_map = {k: i for k, i in where_map.items() if k in _labels}
+            _where_rel_map = {k: i for k, i in where_rel_map.items() if k in _labels}
+            # TODO: validate the insides of where_rel_map only contain labels in _labels
+
+            if use_shortlabel:
+                _labels, _rels, _labels_to_pack, _where_map, _where_rel_map = self.mm.translate_to_shortlabel(
+                    _labels,
+                    _rels,
+                    labels_to_pack,
+                    _where_map,
+                    _where_rel_map,
+                    use_rel_labels=use_rel_labels
+                )
+            # ------------------------------ QUERY BUILD ------------------------------------#
+            (_q_body, _params) = self.qb.generate_query_body(
+                labels=_labels,
+                rels=_rels,
+                match=("MATCH" if i == 0 else "OPTIONAL MATCH"),
+                where_map=_where_map,
+                where_rel_map=_where_rel_map
+            )
+            q_body_list.append(_q_body)
+            params = {**params, **_params}
+
+        q_body = "\n".join(q_body_list)
+        if use_shortlabel:
+            translated = self.mm.translate_to_shortlabel(labels_clean, rels, labels_to_pack, {},
+                                                         use_rel_labels=use_rel_labels)
+            labels_clean = [dct['short_label'] for dct in translated[0]]
+            rels = translated[1]
+            labels_to_pack = translated[2]
+
+        # print(f'Labels to Pack (get_data_generic): {labels_to_pack}')
+
+        q_call = "\n" + self.qb.generate_call(
+            labels=labels_clean,
+            rels=rels,
+            labels_to_pack=labels_to_pack,
+            only_props=only_props
+        )
+
+        q_with = "\n" + self.qb.generate_with(
+            labels=labels_clean,
+            labels_to_pack=labels_to_pack,
+            only_props=only_props,
+            return_nodeid=return_nodeid
+        )
+
+        q_return = "\n" + self.qb.generate_return(
+            labels=labels_clean,
+            labels_to_pack=labels_to_pack,
+            return_nodeid=return_nodeid,
+            return_propname=return_propname,
+            return_termorder=return_termorder,
+            return_class_uris=return_class_uris,
+            only_props=only_props,
+            return_disjoint=return_disjoint
+        )
+        q_limit = (f" LIMIT {str(limit)}" if limit else "")
+        q = q_body + q_call + q_with + q_return + q_limit
+        # ------------------------------ QUERY RUN ------------------------------------#
+        if self.verbose:
+            logger.debug(f"QUERY: {q}")
+            logger.debug(f"PARAMS: {params}")
+        q_res = self.query(q, params)
+        if return_disjoint:
+            res = q_res
+        else:
+            res = pd.DataFrame([r['all'] for r in q_res])
+        # TODO: rename rdfs:label to short_label of each class
+        # pivot dictionaries if labels_to_pack not none
+        if pivot:
+            if labels_to_pack:
+            #code to pivot tables
+                for label in labels_to_pack:
+                    
+                    res = res.drop(label,1).join(pd.DataFrame.from_dict(getattr(res,label).to_dict(), 
+                                                            orient='index'))
+                    if return_nodeid:
+                        id_label = "_id_"+label
+                        res = res.drop(id_label,1).join(pd.DataFrame.from_dict(getattr(res,id_label).to_dict(), 
+                                                            orient='index').add_prefix("_id_"))
+
+        if return_q_and_dict:
+            return res, q, params
+        else:
+            return res
```

### Comparing `tab2neo-1.2.1.0/logger/logger.py` & `tab2neo-1.2.5.0/logger/logger.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,41 @@
-"""
-Custom logger. Level INFO by default, can be changed to DEBUG if CLD is ran with --debug option.
-"""
-
-import logging
-import os
-import colorlog
-from pathlib import Path
-from time import gmtime, strftime
-
-now = strftime("%Y-%m-%d_%H-%M-%S", gmtime())
-
-logger = logging.getLogger("cld")
-logger.setLevel(logging.INFO)
-
-Path(os.path.join("logs", "logger")).mkdir(parents=True, exist_ok=True)
-file_handler = logging.FileHandler(os.path.join("logs", "logger", f"main_{now}.log"))
-
-file_handler.setFormatter(logging.Formatter("%(asctime)s    %(levelname)s    %(message)s"))
-file_handler.setLevel(logging.DEBUG)
-logger.addHandler(file_handler)
-
-stream_handler = colorlog.StreamHandler()
-stream_handler.setFormatter(
-    colorlog.ColoredFormatter(
-        "%(log_color)s%(asctime)s    %(name)s    %(levelname)s    %(message)s",
-        log_colors={
-            "DEBUG": "white",
-            "INFO": "white",
-            "WARNING": "yellow",
-            "ERROR": "red",
-            "CRITICAL": "red,bg_white",
-        },
-    )
-)
-
-logger.addHandler(file_handler)
-logger.addHandler(stream_handler)
-
-logger.info("-------------------------------   Loaded CLD Logger    -------------------------------")
+"""
+Custom logger. Level INFO by default, can be changed to DEBUG if CLD is ran with --debug option.
+"""
+
+import logging
+from time import gmtime, strftime
+
+
+class CustomFormatter(logging.Formatter):
+
+    grey = "\x1b[30;20m"
+    yellow = "\x1b[33;20m"
+    blue = "\x1b[36;20m"
+    red = "\x1b[31;20m"
+    bold_red = "\x1b[31;1m"
+    reset = "\x1b[0m"
+    format = "%(asctime)s    %(name)s    %(levelname)s    %(message)s (%(filename)s:%(lineno)d)"
+
+    FORMATS = {
+        logging.DEBUG: blue + format + reset,
+        logging.INFO: grey + format + reset,
+        logging.WARNING: yellow + format + reset,
+        logging.ERROR: red + format + reset,
+        logging.CRITICAL: bold_red + format + reset
+    }
+
+    def format(self, record):
+        log_fmt = self.FORMATS.get(record.levelno)
+        formatter = logging.Formatter(log_fmt, datefmt='%Y-%m-%d %I:%M:%S')
+        return formatter.format(record)
+
+
+now = strftime("%Y-%m-%d_%H-%M-%S", gmtime())
+
+logger = logging.getLogger("tab2neo")
+logger.setLevel(logging.INFO)
+ch = logging.StreamHandler()
+ch.setFormatter(CustomFormatter())
+logger.addHandler(ch)
+
+logger.info("-------------------------------   Loaded tab2neo Logger    -------------------------------")
```

### Comparing `tab2neo-1.2.1.0/model_managers/model_manager.py` & `tab2neo-1.2.5.0/model_managers/model_manager.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,1113 +1,1141 @@
-import os
-from neointerface import NeoInterface
-from typing import List
-import pandas as pd
-
-
-class ModelManager(NeoInterface):
-    """
-    Python class to manage metadata nodes (such as nodes with label Class, Relationship, Term) along with relationships between them
-    as well as to return information about them
-    """
-    URI_MAP = {
-        "Class": {"properties": ["label"]},
-        "Property": {"properties": ["Class.label", "label"]},
-        "Relationship": {"properties": ["relationship_type"],
-                         "neighbours": [
-                             {"label": "Class", "relationship": "FROM", "property": "label"},
-                             {"label": "Class", "relationship": "TO", "property": "label"},
-                         ]},
-        "Term": {"properties": ["Codelist Code", "Term Code"]},
-        "Method": {"properties": ["parent_id", "id"]},
-    }
-    SCD = 50  # SUBCLASS_OF allowed Depth
-    RDFSLABEL = "rdfs:label"
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        if self.verbose:
-            print(f"---------------- {self.__class__} initialized -------------------")
-
-    def gen_default_reltype(self, to_label: str) -> str:
-        """
-        Default relationship type name is generated from the label of the :TO Class
-        """
-        return f'{to_label}'
-
-    def gen_default_reltypes_list(self, rels: list) -> [{}]:
-        """
-        Updates list of dicts with relationships {'from':...,'to':...,'type':...}
-        replacing 'type':None with default relationship type
-        """
-        return [{**rel, **{'type': (rel['type'] if rel['type'] else self.gen_default_reltype(rel['to']))}}
-                for rel in rels
-                ]
-
-    def create_class(self, classes, merge=True, merge_on: List[str]=None) -> [list]:
-        """
-        :param classes:  List of string labels or a list of property dictionaries to give to the new class(es)
-                         created. For example:
-                         classes = ['class1', 'class2' ...] OR classes = [{"label": 'class1'}, {"label": 'class2'] ...]
-                         Will both result in the creation of two new classes with labels class1 and class2 respectively.
-        :param merge:    boolean - if True use MERGE statement to create nodes to avoid duplicate classes
-                             TODO: address question "would we want to ever allow multiple classes with the same name??"
-        :param merge_on: Optional list of property names MERGED on when classes is a list of property dictionaries. This
-                         can be used to selectively rename certain properties on an existing node rather than
-                         creating a new one, For example:
-
-                            With classes = [{'label': 'class1', 'type': 'new_type'}] and merge on = ['label']
-                            If a class node with 'label' = 'class1' already exists with 'type' = 'old_type' rather
-                            than creating a new node 'class1' will be updated with 'type' = 'new_type'
-
-                         When not merge_on is not set the default behaviour is to merge on all properties.
-        :return:         A list of lists that contain a single dictionary with keys 'label', 'neo4j_id' and 'neo4j_labels'
-                         EXAMPLE: [ [{'label': 'A', 'neo4j_id': 0, 'neo4j_labels': ['Class']}],
-                                    [{'label': 'B', 'neo4j_id': 1, 'neo4j_labels': ['Class']}]
-                                  ]
-        """
-
-        # Maintain backwards compatibility:
-        if type(classes) == str:
-            classes = [classes]
-
-        assert type(classes) == list, "Classes must be a list"
-        assert type(merge) == bool, "Merge must be a bool"
-        if merge_on:
-            assert merge, "Merge_on requires merge = true"
-
-        if type(classes[0]) == str:
-            # Note class_item is the result of unwinding $classes, which in this case is a list of string labels.
-            apoc_action = f"""
-                CALL apoc.{'merge' if merge else 'create'}.node(
-                    ['Class'], {{label: class_item}}{', {}, {}' if merge else ''}
-                ) YIELD node
-            """
-        elif type(classes[0]) == dict:
-            # Note class_item is the result of unwinding $classes, which in this case is a list of property
-            # dictionaries. So a new node would be created/merged with that given dictionary.
-            if not merge_on:
-                apoc_action = f"""
-                    CALL apoc.{'merge' if merge else 'create'}.node(
-                        ['Class'], class_item{', {}, {}' if merge else ''}
-                    ) YIELD node
-                """
-            else:
-                ident_props = f'{{`{merge_on[0]}`: class_item["{merge_on[0]}"]'
-                for prop in merge_on[1:]:
-                    ident_props += f', `{prop}`: class_item["{prop}"]'
-                ident_props += '}'
-
-                apoc_action = f"""
-                    CALL apoc.merge.node(
-                        ['Class'], {ident_props}, class_item, class_item
-                    ) YIELD node
-                """
-                # Example resulting apoc_action format(merge):
-                # With ident props = ['label'] the resulting action would be:
-                # CALL apoc.merge.node(
-                #   ['Class'], {`label`: class_item[`label`]}, class_item, class_item
-                # ) YIELD node
-                # Which matches on 'label then sets the properties to class_item
-        else:
-            raise AssertionError('Classes must be a list of strings or dict')
-
-        q = f"""
-        WITH $classes as classes 
-        UNWIND classes as class_item 
-        {apoc_action}
-        RETURN node as class
-        ORDER by node
-        """
-
-        params = {'classes': classes}
-
-        if self.debug:
-            print(f"""
-            query: {q}
-            parameters: {params}
-            """)
-
-        return self.query(q, params, return_type='neo4j.Result')
-
-    def delete_class(self, values: list, identifier='label'):
-        """
-        Deletes a class and any associated relationships or controlled terminology
-        :param values: list of class labels or property values (if identifier is changed) to match classes for removal
-        :param identifier: Class property to use in combination with values for identification.
-        :return:
-        """
-        # TODO: address the issue of invalid Methods linked to the deleted entities.
-        q = f"""
-        MATCH (class:Class)
-        WHERE class[$identifier] in $values
-        OPTIONAL MATCH (class)-[:HAS_CONTROLLED_TERM]->(term:Term)
-        OPTIONAL MATCH (class)-[:TO|FROM]-(rel:Relationship)
-        DETACH DELETE class, term, rel
-        """
-        params = {'values': values, 'identifier': identifier}
-
-        return self.query(q, params, return_type='neo4j.Result')
-
-    def get_missing_classes(self, values: list, identifier='label'):
-        """
-        Samples a list of class property values to determine if a set of classes are missing from the database.
-        :param values: List of property values eg: [class1, class2]
-        :param identifier: Property name to be used when identifying classes eg: 'label'
-        :return: A list of any values not found in neo4j.
-        """
-
-        q = f"""
-        MATCH (c:Class)
-        WHERE c.{identifier} in $values
-        RETURN collect(c.{identifier}) as existing
-        """
-        params = {'values': values}
-        existing_classes = self.query(q, params)[0].get('existing')
-
-        missing_classes = set(values) - set(existing_classes)
-        return missing_classes
-
-    def set_short_label(self, label: str, short_label: str) -> None:
-        "One the class with :Class{label:{label}} - sets property 'short_label value to the provided"
-        q = """
-        MATCH (c:Class)
-        WHERE c.label = $label
-        SET c.short_label = $short_label
-        """
-        params = {'label': label, 'short_label': short_label}
-        self.query(q, params)
-
-    def create_related_classes_from_list(self, rel_list: [[str, str, str]], identifier='label') -> [str]:
-        """
-        Create `Class` and `Relationship` nodes between them, as specified by rel_list
-
-        Given a list of relationship triplets, perform 2 operations:
-        1)  Identify all the unique names, and create new nodes labeled "Class",
-            each new node has one of the unique names stored in an attribute named "label"
-        2)  Adds <-[:FROM]-(:Relationship{relationship_type:'...'})-[:TO]-> relationships to pairs of the newly-created nodes,
-            as specified by the triplets in the elements of rel_list
-
-        EXAMPLE:  if rel_list is  [  ["Study", "Site", "Site],  ["Study", "Subject", "Subject]  ]
-                  then 3 new `Class`-labeled nodes will be created, with "label" attributes respectively
-                  valued "Study", "Site" and "Subject",
-                  plus <-[:FROM]-(:Relationship{relationship_type:'Site'})-[:TO]-> relationship from "Study" to "Site",
-                  and <-[:FROM]-(:Relationship{relationship_type:'Subject'})-[:TO]-> relationship from "Study" to "Subject"
-
-        :param rel_list: A list of 3-element lists, indicating a relationship among nodes of type `Class`
-                         EXAMPLE:   [
-                                        ["Study", "Site", "Site'],
-                                        ["Study", "Subject", "Subject"],
-                                        ["Subject", "Race", "Race"]
-                                    ]
-        :param identifier: String class property used to identify to & from classes
-        :return: List of all the class names; repeated ones are taken out
-        """
-
-        # Identify all the unique class names in inner elements of rel_list
-        class_set = set()  # Empty set
-        for rel in rel_list:
-            # [:2] in order to get only the first two items (classes) out of rel_list; [2] is the relationship type
-            class_set = class_set.union(rel[:2])  # The Set Union operation will avoid duplicates
-
-        class_list = sorted(list(class_set))  # Convert the final set back to list
-
-        self.create_relationship(rel_list, identifier, match_classes=False)
-
-        return class_list
-
-    def create_relationship(self, rel_list: List[List[str]], identifier='label', match_classes=True) -> [str]:
-        """
-        Create relationship nodes between two specified classes as defined in rel_list.
-        For example:
-            With rel_list = [ ['class1', 'class2', 'example'] ]
-            A new relationship node will be created between nodes with "label", as specified by the
-            identifier, 'class1' and 'class2' with a relationship_type property = 'example'.
-            This relationship node also includes 'FROM.Class.label' and 'TO.Class.label' properties
-            regardless of the class identifier.
-        Note if no relationship type is included a default is generated via gen_default_reltype() 
-        :param rel_list: A list of relationships represented as lists
-        :param identifier: String class property used to identify to & from classes
-        :param match_classes: Boolean, If false classes are merged rather than matched which will create them
-                              if they do not already exist.
-        :return: A list of created relationships = rel_list if all relationships were created successfully
-        """
-
-        q = f"""
-        UNWIND $rels as rel
-        WITH rel[0] as from_identity, rel[1] as to_identity, rel[2] as rel_type
-        {'MATCH' if match_classes else 'MERGE'} (from:Class {{`{identifier}`:from_identity}})
-        {'MATCH' if match_classes else 'MERGE'} (to:Class {{`{identifier}`:to_identity}})   
-        MERGE (from)<-[:FROM]-(rel_node:Relationship{{relationship_type:rel_type}})-[:TO]->(to)
-        SET rel_node.`FROM.Class.label` = from.label
-        SET rel_node.`TO.Class.label` = to.label
-        RETURN collect([from.`{identifier}`, to.`{identifier}`, rel_node.relationship_type]) as rels
-        """
-
-        res = self.query(q, {
-            "rels": [(r if len(r) == 3 else r + [self.gen_default_reltype(to_label=r[1])]) for r in rel_list]
-        })
-        if res:
-            return res[0].get('rels')
-        else:
-            return []
-
-    def delete_relationship(self, rel_list: [[str, str, str]], identifier='label'):
-        """
-        Deletes specified relationships between classes.
-        :param rel_list: List of relationships to be deleted in the following format:
-                         [from class prop value, to class prop value, relationship type]
-                         For example: With identifier = 'label' and
-                         rel_list = [['class1', 'class2', 'Example'], ...]
-                         Relationships of type "Example" between classes with labels = 'class1' and 'class2'
-                         would be deleted.
-        :param identifier: String class property to be used when identifying classes.
-        :return:
-        """
-
-        q = f"""
-        UNWIND $rels as rel
-        WITH rel[0] as from, rel[1] as to, rel[2] as type
-        MATCH (:Class{{`{identifier}`:from}})<-[:FROM]-(rel:Relationship {{relationship_type:type}})-[:TO]->(:Class{{`{identifier}`:to}})
-        DETACH DELETE rel
-        """
-        params = {"rels": rel_list}
-        return self.query(q, params, return_type='neo4j.Result')
-
-    def get_all_classes(self) -> [str]:
-        ""
-        return [c['Class'] for c in self.get_all_classes_with_nodeids()]
-
-    def get_all_classes_with_nodeids(self, include_id=False, sort=True) -> [dict]:
-        """
-        Get all the existing Class names, optionally including their Neo4j ID, and optionally sorted
-        :param include_id:  If True, also include the Neo4j ID's
-        :param sort:        If True, sort the results by name
-        :return:            A list of dictionaries, with keys "Class" (for the name) and "_id_Class"
-                            EXAMPLE, with include_id=False:
-                                [{'Class': 'car'}, {'Class': 'boat'}]
-                            EXAMPLE, with include_id=True:
-                                [{'Class': 'car', "_id_Class": 88}, {'Class': 'boat', "_id_Class": 91}]
-        """
-        q = '''
-            MATCH (class:Class)
-            RETURN class.label as Class, class.short_label as short_label
-            '''
-
-        if include_id:
-            q += " , id(class) as _id_Class "
-
-        if sort:
-            q += " ORDER BY class.label"
-
-        return self.query(q)
-
-    def get_all_classes_props(self, props: [str]) -> [dict]:
-        """
-        Retrieve a list of property values for all classes.
-        :param props: List of properties ro retrieve ie ['label', ...]
-        :return: A list of dictionaries, with keys equal to the specified property name
-                            EXAMPLE, with props=['prop1', 'prop2]:
-                                [{'prop1': 'value', 'prop2': 'value'}, ...]
-        """
-        assert len(props) > 0, 'Must specify at least one property to return!'
-        assert len(props) == len(set(props)), 'Specified props must not contain duplicates!'
-
-        q_return = f"RETURN c.`{props[0]}` as `{props[0]}`"
-        if len(props) != 1:
-            for prop in props[1:]:
-                q_return += f", c.`{prop}` as `{prop}`"
-
-        q = f"""
-        MATCH (c:Class)
-        {q_return}
-        """
-
-        return self.query(q)
-
-    def get_rels_where(self, where_clause=None, return_prop="label") -> [{}]:
-        """
-        Returns a list of dictionaries representing relationships between all classes or a subset of classes and/or
-        relationships if filtered with a cypher where clause.
-        :param where_clause: Optional string cypher where clause, For example:
-                             `WHERE from_class.short_label IS NOT NULL` - Only relationships from_classes with a short_label
-        :param return_prop: Property to identify class in returned relationships. For example with
-                            return prop = "label", relationships will be in the format:
-                            {from: from_class.label, to: to_class.label, type: rel.relationship_type}
-        :return: A list of dicts representing relationships eg:
-                            [{from: from_class.label, to: to_class.label, type: rel.relationship_type}, ...]
-        """
-
-        q = f"""
-        MATCH (from_class:Class)<-[:FROM]-(rel:Relationship)-[:TO]->(to_class:Class)
-        {where_clause if where_clause else ""}
-        RETURN {{from: from_class.`{return_prop}`, to: to_class.`{return_prop}`, type: rel.relationship_type}} as rel   
-        """
-        res = self.query(q)
-        return [x['rel'] for x in res]
-
-    def get_rels_from_labels(self, labels: list) -> [{}]:
-        """
-        Returns all the relationships (according to the schema) from the nodes with specified labels
-        including the relationships of parent and child classes
-        """
-        q = f"""
-        MATCH 
-            (c1:Class)<-[:SUBCLASS_OF*0..{str(self.SCD)}]-(c1low:Class)
-        WHERE 
-            c1.label in $labels AND
-            NOT EXISTS ( (c1low)<-[:SUBCLASS_OF]-(:Class) )
-        WITH c1low
-        MATCH 
-            path1 = (c1high:Class)<-[:SUBCLASS_OF*0..{str(self.SCD)}]-(c1low:Class)
-        WHERE             
-            NOT EXISTS ( (:Class)<-[:SUBCLASS_OF]-(c1high) )
-        WITH nodes(path1) as col1
-        UNWIND col1 as c1       
-        MATCH (x)<-[f:FROM]-(rr:Relationship)-[t:TO]->(y)
-        WHERE x = c1 or y = c1
-        RETURN {{from: x.label, to: y.label, type: rr.relationship_type}} as rel            
-        ORDER BY rel['from'], rel['to'], rel['type']
-        """
-        params = {'labels': labels}
-        res = self.query(q, params)
-        return [x['rel'] for x in res]
-
-    def get_labels_from_rels_list(self, rels_list: list) -> [str]:
-        "Returns all the class labels from a list of relationships in the form {'from':...,'to':...,'type':...}"
-        labels = []
-        for rel in rels_list:
-            for key in ['from', 'to']:
-                if rel.get(key) not in labels:
-                    labels.append(rel.get(key))
-        return labels
-
-    def get_rels_btw2(self, label1: str, label2: str, identifier='label'):
-        """
-        Returns all the relationships (according to the schema) between classes with identifier properties equal to
-        {label1} and {label2} including the relationships of parent and child classes.
-        """
-        q = f"""
-        MATCH 
-            (c1:Class)<-[:SUBCLASS_OF*0..{str(self.SCD)}]-(c1low:Class),
-            (c2:Class)<-[:SUBCLASS_OF*0..{str(self.SCD)}]-(c2low:Class)
-        WHERE 
-            c1.`{identifier}` = $label1 AND c2.`{identifier}` = $label2 AND
-            NOT EXISTS ( (c1low)<-[:SUBCLASS_OF]-(:Class) ) AND
-            NOT EXISTS ( (c2low)<-[:SUBCLASS_OF]-(:Class) ) 
-        WITH c1low, c2low
-        MATCH 
-            path1 = (c1high:Class)<-[:SUBCLASS_OF*0..{str(self.SCD)}]-(c1low:Class),
-            path2 = (c2high:Class)<-[:SUBCLASS_OF*0..{str(self.SCD)}]-(c2low:Class)
-        WHERE             
-            NOT EXISTS ( (:Class)<-[:SUBCLASS_OF]-(c1high) ) AND
-            NOT EXISTS ( (:Class)<-[:SUBCLASS_OF]-(c2high) ) 
-        WITH nodes(path1) as col1, nodes(path2) as col2
-        UNWIND col1 as c1
-        UNWIND col2 as c2
-        WITH c1, c2
-        MATCH (x)<-[f:FROM]-(rr:Relationship)-[t:TO]->(y)
-        WHERE (x = c1 and y = c2) or (y = c1 and x = c2) 
-        RETURN {{from: x.`{identifier}`, to: y.`{identifier}`, type: rr.relationship_type}} as rel            
-        ORDER BY rel['from'], rel['to'], rel['type']
-        """
-        params = {'label1': label1, 'label2': label2}
-        res = self.query(q, params)
-        return [x['rel'] for x in res]
-
-    def infer_rels(self, labels: list, oclass_marker: str = "**", impute_relationship_type: bool = True):
-        """
-        Infers most appropriate relationship type (if exists) between each pair of $labels
-        for generating cypher query according to the schema
-        """
-        q = f"""
-        MATCH (a:Class), (b:Class)
-        WHERE a.label in $labels and b.label in $labels 
-        AND (
-                ( EXISTS ( (a)-[:SUBCLASS_OF*0..{str(
-            self.SCD)}]->()<-[:FROM]-(:Relationship)-[:TO]->()<-[:SUBCLASS_OF*0..{str(self.SCD)}]-(b) ) )
-                OR
-                ( EXISTS ( (a)<-[:SUBCLASS_OF*0..{str(
-            self.SCD)}]-()<-[:FROM]-(:Relationship)-[:TO]->()-[:SUBCLASS_OF*0..{str(self.SCD)}]->(b) ) )
-            )
-        OPTIONAL MATCH 
-            p1 = (a)-[:SUBCLASS_OF*0..{str(
-            self.SCD)}]->()<-[:FROM]-(r1:Relationship)-[:TO]->(crt_to1)<-[:SUBCLASS_OF*0..{str(self.SCD)}]-(b)
-        OPTIONAL MATCH
-            p2 = (a)<-[:SUBCLASS_OF*0..{str(
-            self.SCD)}]-()<-[:FROM]-(r2:Relationship)-[:TO]->(crt_to2)-[:SUBCLASS_OF*0..{str(self.SCD)}]->(b)
-        WITH a, b, 
-            collect(distinct {{
-                path: p1, 
-                rel_type: 
-                    CASE WHEN r1.relationship_type is NULL and $impute_relationship_type THEN 
-                        crt_to1.label
-                    ELSE
-                        r1.relationship_type
-                    END,   
-                short_label: r1.short_label, 
-                tag: 'p1'
-            }})
-            +
-            collect({{
-                path: p2, 
-                rel_type: 
-                    CASE WHEN r2.relationship_type is NULL THEN 
-                        crt_to2.label
-                    ELSE
-                        r2.relationship_type
-                    END,   
-                short_label: r2.short_label,               
-                tag: 'p2'
-            }})
-            as coll
-        UNWIND coll as map
-        WITH a, b, map, size(nodes(map['path'])) as sz 
-        WHERE not map['path'] is NULL
-        WITH *
-        ORDER BY map['tag'], sz //Here we prioritizing paths with SUBCLASS > over paths with < SUBCLASS rel. and then prioritize shorter paths  
-        WITH a, b, collect(map) as coll //ideally we should always have only 1 path for each pair, but allowing here for >1
-        WITH a, b, coll[0] as map        
-        //WITH apoc.map.mergeList(
-        //    [{{from: a.label, to: b.label, type: map['rel_type']}}] +
-        //        CASE WHEN short_label in keys(a) THEN [{{from_tag: a.short_label}}] ELSE [] END +
-        //        CASE WHEN short_label in keys(b) THEN [{{to_tag: b.short_label}}] ELSE [] END
-        //) as rel
-        WITH {{from: a.label, to: b.label, type: map['rel_type'], short_label: map['short_label']}} as rel
-        WITH *
-        ORDER BY rel['from'], rel['to'], rel['type']        
-        RETURN rel
-        """
-        olabels = [label for label in labels if label.endswith(oclass_marker)]
-        params = {
-            'labels': [(label[:-(len(oclass_marker))] if label in olabels else label) for label in labels],
-            'impute_relationship_type': impute_relationship_type
-        }
-        res = self.query(q, params)
-        rels = []
-        for r in res:
-            dct = r['rel']
-            if dct.get('from') in olabels or dct.get('to') in olabels:
-                dct['optional'] = True
-            rels.append(dct)
-        return rels
-
-    def translate_to_shortlabel(self, labels: list, rels: list, labels_to_pack, where_map: dict = None,
-                                where_rel_map: dict = None, use_rel_labels=True):
-        if not where_map:
-            where_map = {}
-        if not where_rel_map:
-            where_rel_map = {}
-
-        q = """
-        MATCH (c:Class)
-        WHERE c.label in $labels
-        RETURN apoc.map.fromPairs(collect([
-            c.label,
-            CASE WHEN 'short_label' in keys(c) THEN  
-                c.short_label
-            ELSE
-                c.label
-            END
-        ])) as map
-        """
-        params = {'labels': list(set(labels + [rel.get('from') for rel in rels] + [rel.get('to') for rel in rels]))}
-        assert labels_to_pack is None or isinstance(labels_to_pack, dict)
-        if labels_to_pack is not None:
-            labels_lst = []
-            for key, value in labels_to_pack.items():
-                assert isinstance(value,
-                                  (str, list)), f'Value in labels_to_pack is not string or list. It was: {type(value)}'
-                labels_lst.append(key)
-                if isinstance(value, str):
-                    labels_lst.append(value)
-                elif isinstance(value, list):
-                    labels_lst.extend(value)
-            params['labels'].extend(labels_lst)
-        # print(f'PARAMS: {params}')
-
-        res = self.query(q, params)
-        map = res[0]['map']
-        if use_rel_labels:
-            for rel in rels:
-                if rel.get('short_label'):
-                    map[rel['to']] = rel.get('short_label')
-        if not labels:
-            labels = []
-        labels = [{'label': label, 'short_label': map[label]} for label in labels]
-        if not rels:
-            rels = []
-        rels = [{**rel, **{'from': map[rel['from']], 'to': map[rel['to']]}} for rel in rels]
-
-        if labels_to_pack is not None:
-            mapped_labels_to_pack = {}
-            # print(f'MAP: {map}')
-            for key, value in labels_to_pack.items():
-                assert isinstance(value,
-                                  (str, list)), f'Value in labels_to_pack is not string or list. It was: {type(value)}'
-                if isinstance(value, str):
-                    mapped_labels_to_pack[map[key]] = map[value]
-                elif isinstance(value, list):
-                    # print(f'KEY: {key}')
-                    # print(f'VALUE: {value}')
-                    assert key in map.keys(), f'{key} was not found as a key in {map}'
-                    assert (True if i in map.keys() else False for i in
-                            value), f'a value from {value} was not found as a key in {map}'
-                    mapped_labels_to_pack[map[key]] = [map[i] for i in value]
-                    # convert the fromclass/coreclass label to short label only
-                    # leave the label as it needs to be long format for the generate_call function
-            labels_to_pack = mapped_labels_to_pack
-
-        if not where_map:
-            where_map = {}
-        where_map = {map[key]: item for key, item in where_map.items()}
-        where_rel_map = {map[key]: item for key, item in where_rel_map.items()}
-        return labels, rels, labels_to_pack, where_map, where_rel_map
-
-    @staticmethod
-    def arrows_dict_uri_dict_enrich(dct: dict, uri_map: dict):
-
-        def _gen_new_prop_name(neighbour: dict):
-            assert len({"label", "relationship", "property"}.intersection(neighbour.keys())) == 3
-            return f"{neighbour['relationship']}.{neighbour['label']}.{neighbour['property']}"
-
-        def _get_neighbour_id(nd: dict, neighbour: dict):
-            assert len({"label", "relationship", "property"}.intersection(neighbour.keys())) == 3
-            for rel in dct['relationships']:
-                if nd["id"] in [rel["toId"]] and rel["type"] == neighbour["relationship"]:
-                    return rel["fromId"]
-                elif nd["id"] in [rel["fromId"]] and rel["type"] == neighbour["relationship"]:
-                    return rel["toId"]
-            return None
-
-        def _get_neighbour_value(nd: dict, neighbour: dict):
-            neighbour_id = _get_neighbour_id(nd, neighbour)
-            for nd in dct['nodes']:
-                if nd['id'] == neighbour_id:
-                    return nd['properties'].get(neighbour["property"])
-
-        def _enrich_node(nd: dict, neighbour: str):
-            value = _get_neighbour_value(nd, neighbour)
-            return {**nd, **{"properties": {**nd["properties"], **{_gen_new_prop_name(neighbour): value}}}}
-
-        merge_on = {}
-        for key, item in uri_map.items():
-            merge_on[key] = item.get("properties").copy()
-            if not merge_on[key]:
-                merge_on[key] = []
-            if item.get('neighbours'):
-                for n in item['neighbours']:
-                    new_nodes = []
-                    for nd in dct['nodes']:
-                        if key in nd['labels']:
-                            new_nodes.append(_enrich_node(nd, n))
-                        else:
-                            new_nodes.append(nd)
-                    dct = {**dct, **{"nodes": new_nodes}}
-                    merge_on[key].append(_gen_new_prop_name(n))
-        return dct, merge_on
-
-    def create_ct(self, controlled_terminology: dict, identifier='label', order_terms=True, merge_on=None):
-        """
-        Creates :Term nodes and links them to a specified class with a [:HAS_CONTROLLED_TERM] relationship.
-        If order terms is True, an ascending Order property will be assigned to terms in the order they are created
-        accounting for the order of existing terms (if any) and [:NEXT] relationships between terms following this order.
-        For example:
-            With identifier = 'label' and controlled_terminology =
-            {
-                'class1': [{'term_label': 'term1'}, {'term_label': 'term2'}],
-                'class2': [{'term_label': 'term3'}]
-            }
-            3 new term nodes with 'term_label' properties equal to 'term1', 'term2' and 'term3' would be
-            created. The class with 'label' = 'class1' would then be linked by [:HAS_CONTROLLED_TERM]
-            relationships to 'term1' and 'term2' and similarly 'class2' would be linked to 'term3'
-
-        :param controlled_terminology: A dictionary of classes and terms eg: {'class1': [{prop1: value, prop2: value}, ...]}
-        :param identifier: String, property used when identifying classes to assign terms.
-        :param order_terms: Bool, if true order properties and next relationships will be created between terms.
-        :param merge_on: Optional List[string] term properties to merge on to prevent duplication
-        :return: neo4j result object.
-        """
-        ident_props = None
-        missing = self.get_missing_classes(list(controlled_terminology.keys()), identifier)
-        assert not missing, f'Cannot create controlled terminology for nonexistent classes: {missing}'
-
-        if merge_on:
-            ident_props = f'{{`{merge_on[0]}`: term_props["{merge_on[0]}"]'
-            for prop in merge_on[1:]:
-                ident_props += f', `{prop}`: term_props["{prop}"]'
-            ident_props += '}'
-
-        # Create terms
-        q1 = f"""
-        UNWIND KEYS($terminology) as class_label
-        MATCH (class:Class {{{identifier}: class_label}})
-        WITH class, class_label
-        UNWIND $terminology[class_label] as term_props
-        CALL apoc.merge.node(['Term'], {f"{ident_props}, term_props, term_props" if ident_props else 'term_props, {}, {}'}) YIELD node
-        CALL apoc.create.addLabels([node], [class.label]) YIELD node as term
-        MERGE (class)-[:HAS_CONTROLLED_TERM]->(term)
-        """
-        res1 = self.query(q1, {'terminology': controlled_terminology}, return_type='neo4j.Result')
-
-        if order_terms:
-            # Create order property on new terms
-            q2 = f"""
-            UNWIND $labels as class_label
-            MATCH (c:Class{{{identifier}: class_label}})
-            OPTIONAL MATCH (c)-[:HAS_CONTROLLED_TERM]->(term:Term)
-            WITH c, MAX(term.Order) as term_order
-            WITH c, CASE WHEN term_order IS NULL THEN 1 ELSE term_order + 1 END as term_order
-    
-            MATCH (c)-[:HAS_CONTROLLED_TERM]->(t1:Term)
-            WHERE t1.Order is NULL
-            WITH c, term_order, t1 order by t1.`Codelist Code`, t1.`Term Code` 
-            WITH c, collect(t1) as terms_to_order, term_order
-            WITH *, apoc.coll.zip(terms_to_order, range(term_order, term_order + size(terms_to_order))) as pairs
-            UNWIND pairs as pair
-            WITH pair[0] as term_node, pair[1] as new_order, c, terms_to_order
-            SET term_node.Order = new_order
-            return c, terms_to_order
-            """
-            self.query(q2, {'labels': list(controlled_terminology.keys())})
-
-            # Create next rel between terms
-            q3 = f"""
-            UNWIND $labels as class_label
-            MATCH (c:Class{{{identifier}: class_label}})-[:HAS_CONTROLLED_TERM]->(t:Term)
-            WITH c,t ORDER BY c.label, t.Order ASC
-            WITH c, COLLECT(t) AS terms
-            FOREACH (n IN RANGE(0, SIZE(terms)-2) |
-                FOREACH (prev IN [terms[n]] |
-                    FOREACH (next IN [terms[n+1]] |
-                        MERGE (prev)-[:NEXT]->(next))))
-            """
-            self.query(q3, {'labels': list(controlled_terminology.keys())})
-
-        return res1
-
-    def get_class_ct(self, class_: str, ct_prop_name='rdfs:label'):
-        q = """
-        MATCH (c:Class) 
-        WHERE c.label = $class_
-        OPTIONAL MATCH (c)-[:HAS_CONTROLLED_TERM]->(t:Term)
-        RETURN collect(DISTINCT t[$ct_prop_name]) as coll
-        """
-        params = {'class_': class_, 'ct_prop_name': ct_prop_name}
-        res = self.query(q, params)
-        if res:
-            return res[0]['coll']
-        else:
-            return []
-
-    def get_class_ct_map(self, classes: list, ct_props: list = None, identifier='label'):
-        """
-        Return controlled terminology for a given list of classes.
-        :param classes: list of class labels of class.identifier property values if using custom identifier
-                        for example: with identifier = 'short_label', classes = ['shortlabel1', 'shortlabel2']
-        :param ct_props: list of controlled terminology props to collect eg:
-                         ['label', 'Codelist Code', 'Order']
-                         defaults to ['rdfs:label']
-        :param identifier: string used when identifying classes
-        :return: Dictionary of classes and found controlled terminology for example:
-                 with classes = ['class1', 'class2'] and ct_props = ['label'] a typical result might be:
-                {'class1': [{'label': 'term1'}, {'label': 'term2'}], 'class2': [{{'label': 'term3'}}]}
-                Where 'class1' has two terms labeled 'term1' and 'term2' and 'class2' has one term labeled 'term3'
-        """
-
-        if ct_props is None:
-            ct_props = ['rdfs:label']
-        elif type(ct_props) == str:
-            ct_props = [ct_props]
-
-        prop_collection = f'["{ct_props[0]}", term.`{ct_props[0]}`]'
-        if len(ct_props) != 1:
-            for prop in ct_props[1:]:
-                prop_collection += f', ["{prop}", term.`{prop}`]'
-
-        q = f"""
-        UNWIND $classes as class
-        MATCH (c:Class)-[:HAS_CONTROLLED_TERM]->(term:Term)
-        WHERE c.`{identifier}` = class
-        WITH c, collect(apoc.map.fromPairs([{prop_collection}])) as terms
-        RETURN apoc.map.setKey({{}}, c.`{identifier}`, terms) as ct
-        """
-
-        params = {'classes': classes}
-        res = self.query(q, params)
-
-        data = {}
-        if res:
-            for term_dict in res:
-                # Flattened result {class.identifer:[[term.ct_props[0], ...], [term.ct_props[0], ...]]}
-                data.update(term_dict.get('ct'))
-        return data
-
-    def delete_ct(self, controlled_terminology: dict, ct_props: list, identifier='label'):
-        """
-        Deletes part of class specific controlled terminology.
-        :param controlled_terminology: Dictionary of key: class identity - value: list of class specific term property
-                                       values to delete. For example:
-                                       with ct_props = ['Codelist Code'] controlled terminology might be:
-                                      {'class1':[['code1'], ['code2']], class1':[['code2']]}
-                                      Note these property values must align with the keys defined in term_props!
-        :param ct_props: List of property names that define property values in a controlled terminology term,
-                         For example:
-                            With controlled terminology = {'class1':[['code1'], ['code2']], class1':[['code2']]}
-                            ct_props would be ['Codelist Code'] indicating that we intending to delete terms
-                            for 'class1' and 'class2' using 'Codelist Code' property value.
-        :param identifier: string, property used to identify class
-        :return: neo4j result object.
-        """
-        # TODO: Resolving [:NEXT] rel when deleting CT
-
-        where_clause = f't.`{ct_props[0]}` = term_props[0]'
-        for count, prop in enumerate(ct_props[1:], start=1):
-            where_clause += f' AND t.`{prop}` = term_props[{count}]'
-
-        q = f"""
-        UNWIND KEYS($terminology) as class_label
-        MATCH (c:Class)
-        WHERE c.`{identifier}` = class_label
-        UNWIND $terminology[class_label] as term_props
-        MATCH (c)-[:HAS_CONTROLLED_TERM]-(t:Term)
-        WHERE {where_clause}
-        DETACH DELETE t
-        """
-
-        return self.query(q, {'terminology': controlled_terminology}, return_type='neo4j.Result')
-
-    def get_all_ct(self, term_props: list, class_prop='label', derived_only=False):
-        """
-        Returns a list of dictionaries containing specified props for all controlled terminology.
-        Example:
-            With term_props = ['rdfs:label'] and class_prop = ['label'] the return format would be:
-            [{'label': class1, 'rdfs:label': 'term1'}, {'label': class1, 'rdfs:label': 'term2'},
-            {'label': class2, 'rdfs:label': 'term1'} ...]
-            Repeated for all CT.
-        :param term_props: Term properties to return eg: ['rdfs:label', 'Codelist Code']
-        :param class_prop: Class property used to identify controlled terminology class
-                            :param derived_only:
-        :param derived_only: Bool, optional filter for classes where class.derived = 'true'.
-        :return: List of dictionaries, see example above.
-        """
-        # TODO: consider converting to format similar to get_class_ct_map? ie {'class.label': [{'rdfs:label': 'term1'}]}
-        assert len(term_props) >= 1, 'Must include at least 1 term_prop'
-        assert class_prop not in term_props, 'Class prop cannot be in term props'
-
-        term_return = f'term.`{term_props[0]}` as `{term_props[0]}`'
-        for prop in term_props[1:]:
-            term_return += f', term.`{prop}` as `{prop}`'
-
-        q = f"""
-        MATCH (c:Class)-[:HAS_CONTROLLED_TERM]->(term:Term)
-        {'WHERE c.derived = "true"' if derived_only else ''}
-        RETURN c.`{class_prop}` as `{class_prop}`, {term_return}
-        """
-        return self.query(q)
-
-    def create_same_as_ct(self, same_as_terms: List[dict], term_identifiers: List[str], identifier='label'):
-        """
-        Creates a [:SAME_AS] relationship between two terms. For example:
-            With term_identifiers = ['Codelist Code', 'Term Code']
-            and same_as_terms = [
-                {'from_class': 'class1', 'to_class': 'class2', # Class identifiers
-                 'from_codelist_code': 'code_1', 'from_term_code': 'code_2', # Term 1 identifier
-                 'to_codelist_code: 'code_3', 'to_term_code': 'code_4' # Term 2 identifier
-                }
-            ]
-            A same as relationship would be created from a term of 'class1' with properties:
-            `Codelist Code` = code_1 and `Term Code` = 'code_2' to the corresponding term for 'class2'.
-
-            Note term identifiers in a same_as_terms dictionaries must be lowercase, use underscores instead of spaces
-            and be prefixed with from_ or to_ a property listed in term_identifiers.
-
-        :param same_as_terms: List of dictionaries defining same as terms between classes.
-        :param term_identifiers: List of strings with term properties that guarantee uniqueness
-        :param identifier: string class property used when matching classes
-        :return: neo4j result object
-        """
-
-        where_clause = f"WHERE c1.`{identifier}` = new_term['from_class'] AND c2.`{identifier}` = new_term['to_class']"
-        for term_prop in term_identifiers:
-            clean_prop = term_prop.lower().replace(' ', '_')
-            where_clause += f" AND t1.`{term_prop}` = new_term['from_{clean_prop}']"
-            where_clause += f" AND t2.`{term_prop}` = new_term['to_{clean_prop}']"
-
-        q = f"""
-        UNWIND $same_as_terms as new_term
-        MATCH (c1:Class)-[:HAS_CONTROLLED_TERM]-(t1:Term)
-        MATCH (c2:Class)-[:HAS_CONTROLLED_TERM]-(t2:Term)
-        {where_clause}
-        MERGE (t1)-[:SAME_AS]->(t2)
-        """
-        return self.query(q, {'same_as_terms': same_as_terms}, return_type='neo4j.Result')
-
-    def remove_same_as_ct(self, same_as_terms: List[dict], term_identifiers: List[str], identifier='label'):
-        """
-        Removes a [:SAME_AS] relationship between two terms, see "create_same_as_ct()" for format information.
-
-        :param same_as_terms: List of dictionaries defining same as terms between classes.
-        :param term_identifiers: List of strings with term properties that guarantee uniqueness
-        :param identifier: string class property used when matching classes
-        :return: neo4j result object
-        """
-
-        where_clause = f"WHERE c1.`{identifier}` = new_term['from_class'] AND c2.`{identifier}` = new_term['to_class']"
-        for term_prop in term_identifiers:
-            clean_prop = term_prop.lower().replace(' ', '_')
-            where_clause += f"AND t1.`{term_prop}` = new_term['from_{clean_prop}']"
-            where_clause += f"AND t2.`{term_prop}` = new_term['to_{clean_prop}']"
-
-        q = f"""
-        UNWIND $same_as_terms as new_term
-        MATCH (c1:Class)-[:HAS_CONTROLLED_TERM]->(t1:Term)-[rel:SAME_AS]->(t2:Term)<-[:HAS_CONTROLLED_TERM]-(c2:Class)
-        {where_clause}
-        DETACH DELETE rel
-        """
-
-        return self.query(q, {'same_as_terms': same_as_terms}, return_type='neo4j.Result')
-
-    def propagate_rels_to_parent_class(self):
-        if self.verbose:
-            print("Copying Relationships to 'parent' Classes where (child)-[:SUBCLASS_OF]->(parent)")
-        self.query("""
-        MATCH (c:Class)<-[r1:TO|FROM]-(r:Relationship)-[r2:TO|FROM]-(target:Class), (c)-[:SUBCLASS_OF*1..50]->(source:Class)
-        WHERE type(r1) <> type(r2)
-        WITH *,
-        "
-            WITH $source as source, $target as target
-            MERGE (source)<-[:`"+type(r1)+"`]-(:Relationship{relationship_type:$type})-[:`"+type(r2)+"`]->(target)
-            RETURN count(*)
-        " as q, 
-        {type: r.relationship_type, source: source , target: target} as params
-        CALL apoc.cypher.doIt(q, params) YIELD value
-        RETURN value, q, params         
-        """)
-
-    def remove_unmapped_classes(self):
-        q = """
-        MATCH (c:Class)
-        WHERE NOT EXISTS (
-            ()-[:MAPS_TO_CLASS]->()-[:SUBCLASS_OF*0..50]->(c)
-        )
-        OPTIONAL MATCH (c)<-[:TO|FROM]-(r:Relationship)
-        REMOVE r:Relationship
-        REMOVE c:Class
-        """
-        self.query(q)
-
-    def remove_auxilary_term_labels(self):
-        """
-        To be used after reshaping - additional labels from Terms that have not been extracted from data are removed
-        :return:
-        """
-        q = """
-        MATCH (x:Term) 
-        WHERE not exists ( (x)-[:FROM_DATA]->() )
-        WITH x, labels(x) as coll
-        UNWIND coll as lbl
-        WITH *
-        WHERE NOT lbl in ["Term", "Class"]
-        CALL apoc.cypher.doIt(
-        'WITH x REMOVE x:`'+lbl+'`',
-        {x:x}
-        ) yield value
-        RETURN value
-        """
-        self.query(q)
-
-    def export_model_ttl(self, folder: str, filename: str, include_mappings=False):
-        uri_map1 = {
-            "Data Extraction Standard": {"properties": "_tag_"},
-            "Source Data Folder": {"properties": "_folder_"},
-            "Source Data Table": {"properties": "_domain_"},
-            "Source Data Column": {"properties": ["_domain_", "_columnname_"]}
-        }
-        uri_map2 = {key: item
-                    for key, item in ModelManager.URI_MAP.items()
-                    if key in ["Class", "Property", "Relationship"]}
-
-        if include_mappings:
-            self.rdf_generate_uri({**uri_map1, **uri_map2})
-            rdf = self.rdf_get_subgraph(
-                """
-                MATCH (n:Class)
-                call apoc.path.expand(n, 
-                    'SUBCLASS_OF|HAS_CONTROLLED_TERM>|<MAPS_TO_CLASS|<HAS_COLUMN|<HAS_TABLE|<TO|<FROM', 
-                    '+Class|+Term|+Relationship|+Data Extraction Standard|+Source Data Folder|+Source Data Table|+Source Data Column', 
-                    0, 1 ) yield path
-                RETURN path
-                """
-            )
-        else:
-            self.rdf_generate_uri(uri_map2)
-            rdf = self.rdf_get_subgraph(
-                """
-                MATCH (n:Class)
-                call apoc.path.expand(n, 'SUBCLASS_OF|HAS_CONTROLLED_TERM|<TO|<FROM', '+Class|+Relationship|+Term', 0, 1 ) yield path
-                RETURN path
-                """
-            )
-        rdf_file_path = os.path.join(folder, filename)
-        with open(rdf_file_path, "w") as file:
-            file.write(rdf)
-
-    def create_custom_mappings_from_dict(self, groupings = None) -> None:
-        """
-        Function to support MethodApplier(mode="schema_PROPERTY")
-
-        Create a set of nodes labeled "Class", all taken from the groupings dictionary; their names are
-            stored in an attribute named "label".  EXAMPLES: "Study", "Site", "Race", "Adverse Event".
-
-        Also, create a set of nodes labeled "Property"; likewise, their names are
-            stored in an attribute named "label".  EXAMPLES: "RACE", "RACEN", "SITEID".
-
-        In addition, create relationships named "HAS_PROPERTY", from each of the "Class" nodes to the appropriate
-            "Property" nodes.   EXAMPLE:  The "Race" node (labeled "Class") links to the "RACE", "RACEN" nodes
-            (labeled "Property")
-
-        Finally,  create relationships named "MAPS_TO_PROPERTY", from `Source Data Column` nodes to `Property` nodes.
-            These relationships are created based on matches between the "_columnname_" attribute on `Source Data Column` nodes
-            and entries in the lists contained in groupings (e.g., "RACEN"); in some cases, further restrictions are applied,
-            requiring the `Source Data Column` node to be linked to a particular `Source Data Table` node.
-
-        :param groupings:   A dictionary.  The keys are either "*" (meaning no `Source Data Table` restriction)
-                                           or the name of a specific `Source Data Table`.
-                                           The values are dictionaries such as {"Race": ["RACE", "RACEN"]}
-        :return:            None
-        """
-        if not groupings:
-            groupings = {}
-
-        # Loop over all the keys/values of the groupings dictionary
-        for table, groupping in groupings.items():
-            # EXAMPLES of table:  "ADSL" or "*" (the star indicates "all tables")
-            # groupping is a dictionary with entries such as  "Race": ["RACE", "RACEN"]
-
-            # Define the Cypher query, which depends on the value of the "table" variable in the outer loop;
-            #       for examples of how the query shapes up, see below (inside inner loop)
-            q = f"""                    
-                MERGE (class:Class {{label:$class}})
-                WITH * UNWIND $properties as property
-                MERGE (class)-[:HAS_PROPERTY]->(p:Property {{label:property}})
-                WITH *
-                MATCH (sdc:`Source Data Column` {{_columnname_:property}})
-                {
-                "" if table == "*" else "<-[:HAS_COLUMN]-(sdt:`Source Data Table` {_domain_:$table})"
-                }                     
-                MERGE (sdc)-[:MAPS_TO_PROPERTY]->(p)
-                """
-
-            for class_, properties in groupping.items():
-                # EXAMPLE of class_ : "Race"
-                # EXAMPLE of properties: ["RACE", "RACEN"]
-
-                params = {"table":table, "class": class_, "properties": properties}
-                self.query(q, params)
-
-                # EXAMPLE1 of query (involving a specific table, such as "ADSL")
-                """
-                    MERGE (class:Class {label:$class})
-                    WITH * UNWIND $properties as property
-                    MERGE (class)-[:HAS_PROPERTY]->(p:Property {label:property})
-                    WITH *
-                    MATCH (sdc:`Source Data Column` {_columnname_:property})
-                    <-[:HAS_COLUMN]-(sdt:`Source Data Table` {_domain_:$table})                     
-                    MERGE (sdc)-[:MAPS_TO_PROPERTY]->(p)
-                """
-
-                # EXAMPLE2 of query (involving any table, indicated by the "*" value of the table variable)
-                """
-                    MERGE (class:Class {label:$class})
-                    WITH * UNWIND $properties as property
-                    MERGE (class)-[:HAS_PROPERTY]->(p:Property {label:property})
-                    WITH *
-                    MATCH (sdc:`Source Data Column` {_columnname_:property})                     
-                    MERGE (sdc)-[:MAPS_TO_PROPERTY]->(p)
-                """
-                # EXAMPLE of params: {'table': 'ADSL', 'class': 'Race', 'properties': ['RACE', 'RACEN']}
-
-    def create_custom_rels_from_list(self, rels: [[str, str]], create_if_absent = False) -> None:
-        """
-        Adds "CLASS_RELATES_TO" relationships to pairs of nodes with "Class" label,
-        based on the list passed as the argument "rels".
-        Matches occur based on node attributes named "label".
-        Optionally, create the Class nodes if needed.
-        To create just a single relationship, see create_class_relationship()
-
-        NOTE: this is a more general version of the method create_related_classes_from_list()
-
-        :param rels:    A list of 2-element lists, indicating a relationship among nodes of type `Class`
-                        EXAMPLE:   [
-                                        ["Study", "Site"],
-                                        ["Study", "Subject"],
-                                        ["Subject", "Race"]
-                                   ]
-        :param create_if_absent: If True, the Class nodes specified in the argument "rel" get created as needed;
-                                        otherwise, no relationships get created whenever their start or end class is missing
-        :return:                 None
-        """
-        if rels is None or rels == []:
-            return      # There's nothing to do
-
-        if create_if_absent:
-            q = f"""            
-                UNWIND $rels as rel
-                WITH rel[0] as left, rel[1] as right      
-                WHERE apoc.meta.type(left) = apoc.meta.type(right) = 'STRING'  
-                MERGE (ln:Class {{label:left}})
-                MERGE (rn:Class {{label:right}})   
-                MERGE (ln)-[:CLASS_RELATES_TO]->(rn)   
-                """
-        else:   # The Class nodes MUST be present, or no relationship gets created
-            q = f"""            
-                UNWIND $rels as rel
-                WITH rel[0] as left, rel[1] as right    
-                WHERE apoc.meta.type(left) = apoc.meta.type(right) = 'STRING'      
-                MATCH (ln:Class {{label:left}}), (rn:Class {{label:right}})    
-                MERGE (ln)-[:CLASS_RELATES_TO]->(rn)   
-                """
-
-        params = {"rels": rels}
-        self.query(q, params)
-
-    def create_model_from_data(
-            self,
-            data_label: str = "Source Data Row",
-            data_table_label: str = "Source Data Table",
-            domain_property: str = "_domain_",
-            no_domain_label: str = "Thing",
-            data_column_label: str = "Source Data Column",
-            columnname_property: str = "_columnname_",
-            exclude_properties: list = None,
-    ):
-        """
-        Creates Class and Relationship nodes to represent a trivial schema to reshape data ingested e.g. with
-        FileDataLoader - Tables loaded into nodes one row to one node, column names used as property names.
-
-        data_labels: labels of the nodes where loaded data is stored (mm with use OR btw labels to fetch data nodes)
-        domain_property: property where the name of the table/domain can be found
-        """
-        if exclude_properties is None:
-            exclude_properties = ["_filename_", "_folder_"]
-        q = f"""
-        MATCH (data:`{data_label}`)<-[:HAS_DATA]-(dt:`{data_table_label}`)        
-        WITH distinct dt, dt._domain_ as domain, keys(data) as ks
-        WITH *, CASE WHEN domain IS NULL THEN $no_domain_label ELSE domain END as domain
-        WITH dt, domain, [k in ks WHERE NOT k IN $exclude_properties] as ks
-        WITH dt, domain, apoc.coll.flatten(apoc.coll.toSet(ks)) as ks
-        MERGE (c:Class{{label: domain, short_label: domain, create: True}})
-        MERGE (dt)-[:MAPS_TO_CLASS]->(c)
-        WITH *
-        UNWIND ks as k
-        MATCH (dt)-[:HAS_COLUMN]->(col:`{data_column_label}`)
-        WHERE col.`{columnname_property}` = k
-        MERGE (c2:Class{{label: k, short_label: k}})        
-        MERGE (c)<-[:FROM]-(r:Relationship{{relationship_type: k}})-[:TO]->(c2)
-        MERGE (col)-[:MAPS_TO_CLASS]->(c2)        
-        """
-        params = {
-            "exclude_properties": exclude_properties + [domain_property],
-            "no_domain_label": no_domain_label
-        }
+import os
+from neointerface import NeoInterface
+from typing import List
+import pandas as pd
+import numpy as np
+from logger.logger import logger
+
+
+class ModelManager(NeoInterface):
+    """
+    Python class to manage metadata nodes (such as nodes with label Class, Relationship, Term) along with relationships between them
+    as well as to return information about them
+    """
+    URI_MAP = {
+        "Class": {"properties": ["label"]},
+        "Property": {"properties": ["Class.label", "label"]},
+        "Relationship": {"properties": ["relationship_type"],
+                         "neighbours": [
+                             {"label": "Class", "relationship": "FROM", "property": "label"},
+                             {"label": "Class", "relationship": "TO", "property": "label"},
+                         ]},
+        "Term": {"properties": ["Codelist Code", "Term Code"]},
+        "Method": {"properties": ["parent_id", "id"]},
+    }
+    SCD = 50  # SUBCLASS_OF allowed Depth
+    RDFSLABEL = "rdfs:label"
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        if self.verbose:
+            logger.info(f"---------------- {self.__class__} initialized -------------------")
+
+    def gen_default_reltype(self, to_label: str) -> str:
+        """
+        Default relationship type name is generated from the label of the :TO Class
+        """
+        return f'{to_label}'
+
+    def gen_default_reltypes_list(self, rels: list) -> [{}]:
+        """
+        Updates list of dicts with relationships {'from':...,'to':...,'type':...}
+        replacing 'type':None with default relationship type
+        """
+        return [{**rel, **{'type': (rel['type'] if rel['type'] else self.gen_default_reltype(rel['to']))}}
+                for rel in rels
+                ]
+
+    def create_class(self, classes, merge=True, merge_on: List[str]=None) -> [list]:
+        """
+        :param classes:  List of string labels or a list of property dictionaries to give to the new class(es)
+                         created. For example:
+                         classes = ['class1', 'class2' ...] OR classes = [{"label": 'class1'}, {"label": 'class2'] ...]
+                         Will both result in the creation of two new classes with labels class1 and class2 respectively.
+        :param merge:    boolean - if True use MERGE statement to create nodes to avoid duplicate classes
+                             TODO: address question "would we want to ever allow multiple classes with the same name??"
+        :param merge_on: Optional list of property names MERGED on when classes is a list of property dictionaries. This
+                         can be used to selectively rename certain properties on an existing node rather than
+                         creating a new one, For example:
+
+                            With classes = [{'label': 'class1', 'type': 'new_type'}] and merge on = ['label']
+                            If a class node with 'label' = 'class1' already exists with 'type' = 'old_type' rather
+                            than creating a new node 'class1' will be updated with 'type' = 'new_type'
+
+                         When not merge_on is not set the default behaviour is to merge on all properties.
+        :return:         A list of lists that contain a single dictionary with keys 'label', 'neo4j_id' and 'neo4j_labels'
+                         EXAMPLE: [ [{'label': 'A', 'neo4j_id': 0, 'neo4j_labels': ['Class']}],
+                                    [{'label': 'B', 'neo4j_id': 1, 'neo4j_labels': ['Class']}]
+                                  ]
+        """
+
+        # Maintain backwards compatibility:
+        if type(classes) == str:
+            classes = [classes]
+
+        assert type(classes) == list, "Classes must be a list"
+        assert type(merge) == bool, "Merge must be a bool"
+        if merge_on:
+            assert merge, "Merge_on requires merge = true"
+
+        if type(classes[0]) == str:
+            # Note class_item is the result of unwinding $classes, which in this case is a list of string labels.
+            apoc_action = f"""
+                CALL apoc.{'merge' if merge else 'create'}.node(
+                    ['Class'], {{label: class_item}}{', {}, {}' if merge else ''}
+                ) YIELD node
+            """
+        elif type(classes[0]) == dict:
+            # Note class_item is the result of unwinding $classes, which in this case is a list of property
+            # dictionaries. So a new node would be created/merged with that given dictionary.
+            if not merge_on:
+                apoc_action = f"""
+                    CALL apoc.{'merge' if merge else 'create'}.node(
+                        ['Class'], class_item{', {}, {}' if merge else ''}
+                    ) YIELD node
+                """
+            else:
+                ident_props = f'{{`{merge_on[0]}`: class_item["{merge_on[0]}"]'
+                for prop in merge_on[1:]:
+                    ident_props += f', `{prop}`: class_item["{prop}"]'
+                ident_props += '}'
+
+                apoc_action = f"""
+                    CALL apoc.merge.node(
+                        ['Class'], {ident_props}, class_item, class_item
+                    ) YIELD node
+                """
+                # Example resulting apoc_action format(merge):
+                # With ident props = ['label'] the resulting action would be:
+                # CALL apoc.merge.node(
+                #   ['Class'], {`label`: class_item[`label`]}, class_item, class_item
+                # ) YIELD node
+                # Which matches on 'label then sets the properties to class_item
+        else:
+            raise AssertionError('Classes must be a list of strings or dict')
+
+        q = f"""
+        WITH $classes as classes 
+        UNWIND classes as class_item 
+        {apoc_action}
+        RETURN node as class
+        ORDER by node
+        """
+
+        params = {'classes': classes}
+
+        if self.verbose:
+            logger.debug(f"""
+            query: {q}
+            parameters: {params}
+            """)
+
+        return self.query(q, params, return_type='neo4j.Result')
+
+    def delete_class(self, values: list, identifier='label'):
+        """
+        Deletes a class and any associated relationships or controlled terminology
+        :param values: list of class labels or property values (if identifier is changed) to match classes for removal
+        :param identifier: Class property to use in combination with values for identification.
+        :return:
+        """
+        # TODO: address the issue of invalid Methods linked to the deleted entities.
+        q = f"""
+        MATCH (class:Class)
+        WHERE class[$identifier] in $values
+        OPTIONAL MATCH (class)-[:HAS_CONTROLLED_TERM]->(term:Term)
+        OPTIONAL MATCH (class)-[:TO|FROM]-(rel:Relationship)
+        DETACH DELETE class, term, rel
+        """
+        params = {'values': values, 'identifier': identifier}
+
+        return self.query(q, params, return_type='neo4j.Result')
+
+    def get_missing_classes(self, values: list, identifier='label'):
+        """
+        Samples a list of class property values to determine if a set of classes are missing from the database.
+        :param values: List of property values eg: [class1, class2]
+        :param identifier: Property name to be used when identifying classes eg: 'label'
+        :return: A list of any values not found in neo4j.
+        """
+
+        q = f"""
+        MATCH (c:Class)
+        WHERE c.{identifier} in $values
+        RETURN collect(c.{identifier}) as existing
+        """
+        params = {'values': values}
+        existing_classes = self.query(q, params)[0].get('existing')
+
+        missing_classes = set(values) - set(existing_classes)
+        return missing_classes
+
+    def set_short_label(self, label: str, short_label: str) -> None:
+        "One the class with :Class{label:{label}} - sets property 'short_label value to the provided"
+        q = """
+        MATCH (c:Class)
+        WHERE c.label = $label
+        SET c.short_label = $short_label
+        """
+        params = {'label': label, 'short_label': short_label}
+        self.query(q, params)
+
+    def create_related_classes_from_list(self, rel_list: [[str, str, str]], identifier='label') -> [str]:
+        """
+        Create `Class` and `Relationship` nodes between them, as specified by rel_list
+
+        Given a list of relationship triplets, perform 2 operations:
+        1)  Identify all the unique names, and create new nodes labeled "Class",
+            each new node has one of the unique names stored in an attribute named "label"
+        2)  Adds <-[:FROM]-(:Relationship{relationship_type:'...'})-[:TO]-> relationships to pairs of the newly-created nodes,
+            as specified by the triplets in the elements of rel_list
+
+        EXAMPLE:  if rel_list is  [  ["Study", "Site", "Site],  ["Study", "Subject", "Subject]  ]
+                  then 3 new `Class`-labeled nodes will be created, with "label" attributes respectively
+                  valued "Study", "Site" and "Subject",
+                  plus <-[:FROM]-(:Relationship{relationship_type:'Site'})-[:TO]-> relationship from "Study" to "Site",
+                  and <-[:FROM]-(:Relationship{relationship_type:'Subject'})-[:TO]-> relationship from "Study" to "Subject"
+
+        :param rel_list: A list of 3-element lists, indicating a relationship among nodes of type `Class`
+                         EXAMPLE:   [
+                                        ["Study", "Site", "Site'],
+                                        ["Study", "Subject", "Subject"],
+                                        ["Subject", "Race", "Race"]
+                                    ]
+        :param identifier: String class property used to identify to & from classes
+        :return: List of all the class names; repeated ones are taken out
+        """
+
+        # Identify all the unique class names in inner elements of rel_list
+        class_set = set()  # Empty set
+        for rel in rel_list:
+            # [:2] in order to get only the first two items (classes) out of rel_list; [2] is the relationship type
+            class_set = class_set.union(rel[:2])  # The Set Union operation will avoid duplicates
+
+        class_list = sorted(list(class_set))  # Convert the final set back to list
+
+        self.create_relationship(rel_list, identifier, match_classes=False)
+
+        return class_list
+
+    def create_relationship(self, rel_list: List[List[str]], identifier='label', match_classes=True) -> [str]:
+        """
+        Create relationship nodes between two specified classes as defined in rel_list.
+        For example:
+        1.  With rel_list = [ ['class1', 'class2', 'example'] ]
+            A new relationship node will be created between nodes with "label", as specified by the
+            identifier, 'class1' and 'class2' with a relationship_type property = 'example'.
+            This relationship node also includes 'FROM.Class.label' and 'TO.Class.label' properties
+            regardless of the class identifier.
+
+        2.  With rel_list = [ ['class1', 'class2', 'example','false'] ]
+            A new relationship node will be created between nodes with "label", as specified by the
+            identifier, 'class1' and 'class2' with a relationship_type property = 'example' and optional_relationship = 'false'.
+            This relationship node also includes 'FROM.Class.label' and 'TO.Class.label' properties
+            regardless of the class identifier.
+        Note if no relationship type is included in example-1, a default is generated via gen_default_reltype() 
+        and if no relationship type is included in example-2, optional_relationship would be considered as relationship type 
+        and optional relationship would be ignored
+        :param rel_list: A list of relationships represented as lists
+        :param identifier: String class property used to identify to & from classes
+        :param match_classes: Boolean, If false classes are merged rather than matched which will create them
+                              if they do not already exist.
+        :return: A list of created relationships = rel_list if all relationships were created successfully
+        """
+
+        q = f"""
+        UNWIND $rels as rel
+        CALL apoc.do.when(size(rel)<=3,
+        "WITH rel[0] as from_identity, rel[1] as to_identity, rel[2] as rel_type
+        {'MATCH' if match_classes else 'MERGE'} (from:Class {{`{identifier}`:from_identity}})
+        {'MATCH' if match_classes else 'MERGE'} (to:Class {{`{identifier}`:to_identity}})   
+        MERGE (from)<-[:FROM]-(rel_node:Relationship{{relationship_type:rel_type}})-[:TO]->(to)
+        SET rel_node.`FROM.Class.label` = from.label
+        SET rel_node.`TO.Class.label` = to.label
+        RETURN collect([from.`{identifier}`, to.`{identifier}`, rel_node.relationship_type]) as rels", 
+        "WITH rel[0] as from_identity, rel[1] as to_identity, rel[2] as rel_type, rel[3] as optional
+        {'MATCH' if match_classes else 'MERGE'} (from:Class {{`{identifier}`:from_identity}})
+        {'MATCH' if match_classes else 'MERGE'} (to:Class {{`{identifier}`:to_identity}})   
+        MERGE (from)<-[:FROM]-(rel_node:Relationship{{relationship_type:rel_type, relationship_optional:optional}})-[:TO]->(to)
+        SET rel_node.`FROM.Class.label` = from.label
+        SET rel_node.`TO.Class.label` = to.label
+        RETURN collect([from.`{identifier}`, to.`{identifier}`, rel_node.relationship_type, rel_node.relationship_optional]) as rels
+        ",
+        {{rel:rel}})
+        YIELD value
+        RETURN collect(value.rels) as rels
+        """
+
+        res = self.query(q, {
+            "rels": [(r if len(r)>=3 else r + [self.gen_default_reltype(to_label=r[1])]) for r in rel_list]
+        })
+
+        if res:
+            result = [np.array(i).flatten().tolist() for i in res[0].get('rels')]
+            return result
+        else:
+            return []
+
+    def delete_relationship(self, rel_list: [[str, str, str]], identifier='label'):
+        """
+        Deletes specified relationships between classes.
+        :param rel_list: List of relationships to be deleted in the following format:
+                         [from class prop value, to class prop value, relationship type]
+                         For example: With identifier = 'label' and
+                         rel_list = [['class1', 'class2', 'Example'], ...]
+                         Relationships of type "Example" between classes with labels = 'class1' and 'class2'
+                         would be deleted.
+        :param identifier: String class property to be used when identifying classes.
+        :return:
+        """
+
+        q = f"""
+        UNWIND $rels as rel
+        WITH rel[0] as from, rel[1] as to, rel[2] as type
+        MATCH (:Class{{`{identifier}`:from}})<-[:FROM]-(rel:Relationship {{relationship_type:type}})-[:TO]->(:Class{{`{identifier}`:to}})
+        DETACH DELETE rel
+        """
+        params = {"rels": rel_list}
+        return self.query(q, params, return_type='neo4j.Result')
+
+    def get_all_classes(self) -> [str]:
+        ""
+        return [c['Class'] for c in self.get_all_classes_with_nodeids()]
+
+    def get_all_classes_with_nodeids(self, include_id=False, sort=True) -> [dict]:
+        """
+        Get all the existing Class names, optionally including their Neo4j ID, and optionally sorted
+        :param include_id:  If True, also include the Neo4j ID's
+        :param sort:        If True, sort the results by name
+        :return:            A list of dictionaries, with keys "Class" (for the name) and "_id_Class"
+                            EXAMPLE, with include_id=False:
+                                [{'Class': 'car'}, {'Class': 'boat'}]
+                            EXAMPLE, with include_id=True:
+                                [{'Class': 'car', "_id_Class": 88}, {'Class': 'boat', "_id_Class": 91}]
+        """
+        q = '''
+            MATCH (class:Class)
+            RETURN class.label as Class, class.short_label as short_label
+            '''
+
+        if include_id:
+            q += " , id(class) as _id_Class "
+
+        if sort:
+            q += " ORDER BY class.label"
+
+        return self.query(q)
+
+    def get_all_classes_props(self, props: [str]) -> [dict]:
+        """
+        Retrieve a list of property values for all classes.
+        :param props: List of properties ro retrieve ie ['label', ...]
+        :return: A list of dictionaries, with keys equal to the specified property name
+                            EXAMPLE, with props=['prop1', 'prop2]:
+                                [{'prop1': 'value', 'prop2': 'value'}, ...]
+        """
+        assert len(props) > 0, 'Must specify at least one property to return!'
+        assert len(props) == len(set(props)), 'Specified props must not contain duplicates!'
+
+        q_return = f"RETURN c.`{props[0]}` as `{props[0]}`"
+        if len(props) != 1:
+            for prop in props[1:]:
+                q_return += f", c.`{prop}` as `{prop}`"
+
+        q = f"""
+        MATCH (c:Class)
+        {q_return}
+        """
+
+        return self.query(q)
+
+    def get_rels_where(self, where_clause=None, return_prop="label") -> [{}]:
+        """
+        Returns a list of dictionaries representing relationships between all classes or a subset of classes and/or
+        relationships if filtered with a cypher where clause.
+        :param where_clause: Optional string cypher where clause, For example:
+                             `WHERE from_class.short_label IS NOT NULL` - Only relationships from_classes with a short_label
+        :param return_prop: Property to identify class in returned relationships. For example with
+                            return prop = "label", relationships will be in the format:
+                            {from: from_class.label, to: to_class.label, type: rel.relationship_type, optional: rel.relationship_optional}
+        :return: A list of dicts representing relationships eg:
+                            [{from: from_class.label, to: to_class.label, type: rel.relationship_type, optional: rel.relationship_optional}, ...]
+        """
+
+        q = f"""
+        MATCH (from_class:Class)<-[:FROM]-(rel:Relationship)-[:TO]->(to_class:Class)
+        {where_clause if where_clause else ""}
+        RETURN {{from: from_class.`{return_prop}`, to: to_class.`{return_prop}`, type: rel.relationship_type, optional: rel.relationship_optional}} as rel   
+        """
+        res = self.query(q)
+        return [x['rel'] for x in res]
+
+    def get_rels_from_labels(self, labels: list) -> [{}]:
+        """
+        Returns all the relationships (according to the schema) from the nodes with specified labels
+        including the relationships of parent and child classes
+        """
+        q = f"""
+        MATCH 
+            (c1:Class)<-[:SUBCLASS_OF*0..{str(self.SCD)}]-(c1low:Class)
+        WHERE 
+            c1.label in $labels AND
+            NOT EXISTS ( (c1low)<-[:SUBCLASS_OF]-(:Class) )
+        WITH c1low
+        MATCH 
+            path1 = (c1high:Class)<-[:SUBCLASS_OF*0..{str(self.SCD)}]-(c1low:Class)
+        WHERE             
+            NOT EXISTS ( (:Class)<-[:SUBCLASS_OF]-(c1high) )
+        WITH nodes(path1) as col1
+        UNWIND col1 as c1       
+        MATCH (x)<-[f:FROM]-(rr:Relationship)-[t:TO]->(y)
+        WHERE x = c1 or y = c1
+        RETURN {{from: x.label, to: y.label, type: rr.relationship_type, optional: rr.relationship_optional}} as rel            
+        ORDER BY rel['from'], rel['to'], rel['type']
+        """
+        params = {'labels': labels}
+        res = self.query(q, params)
+        return [x['rel'] for x in res]
+
+    def get_labels_from_rels_list(self, rels_list: list) -> [str]:
+        "Returns all the class labels from a list of relationships in the form {'from':...,'to':...,'type':...}"
+        labels = []
+        for rel in rels_list:
+            for key in ['from', 'to']:
+                if rel.get(key) not in labels:
+                    labels.append(rel.get(key))
+        return labels
+
+    def get_rels_btw2(self, label1: str, label2: str, identifier='label'):
+        """
+        Returns all the relationships (according to the schema) between classes with identifier properties equal to
+        {label1} and {label2} including the relationships of parent and child classes.
+        """
+        q = f"""
+        MATCH 
+            (c1:Class)<-[:SUBCLASS_OF*0..{str(self.SCD)}]-(c1low:Class),
+            (c2:Class)<-[:SUBCLASS_OF*0..{str(self.SCD)}]-(c2low:Class)
+        WHERE 
+            c1.`{identifier}` = $label1 AND c2.`{identifier}` = $label2 AND
+            NOT EXISTS ( (c1low)<-[:SUBCLASS_OF]-(:Class) ) AND
+            NOT EXISTS ( (c2low)<-[:SUBCLASS_OF]-(:Class) ) 
+        WITH c1low, c2low
+        MATCH 
+            path1 = (c1high:Class)<-[:SUBCLASS_OF*0..{str(self.SCD)}]-(c1low:Class),
+            path2 = (c2high:Class)<-[:SUBCLASS_OF*0..{str(self.SCD)}]-(c2low:Class)
+        WHERE             
+            NOT EXISTS ( (:Class)<-[:SUBCLASS_OF]-(c1high) ) AND
+            NOT EXISTS ( (:Class)<-[:SUBCLASS_OF]-(c2high) ) 
+        WITH nodes(path1) as col1, nodes(path2) as col2
+        UNWIND col1 as c1
+        UNWIND col2 as c2
+        WITH c1, c2
+        MATCH (x)<-[f:FROM]-(rr:Relationship)-[t:TO]->(y)
+        WHERE (x = c1 and y = c2) or (y = c1 and x = c2) 
+        RETURN {{from: x.`{identifier}`, to: y.`{identifier}`, type: rr.relationship_type}} as rel            
+        ORDER BY rel['from'], rel['to'], rel['type']
+        """
+        params = {'label1': label1, 'label2': label2}
+        res = self.query(q, params)
+        return [x['rel'] for x in res]
+
+    def infer_rels(self, labels: list, oclass_marker: str = "**", impute_relationship_type: bool = True):
+        """
+        Infers most appropriate relationship type (if exists) between each pair of $labels
+        for generating cypher query according to the schema
+        """
+        q = f"""
+        MATCH (a:Class), (b:Class)
+        WHERE a.label in $labels and b.label in $labels 
+        AND (
+                ( EXISTS ( (a)-[:SUBCLASS_OF*0..{str(
+            self.SCD)}]->()<-[:FROM]-(:Relationship)-[:TO]->()<-[:SUBCLASS_OF*0..{str(self.SCD)}]-(b) ) )
+                OR
+                ( EXISTS ( (a)<-[:SUBCLASS_OF*0..{str(
+            self.SCD)}]-()<-[:FROM]-(:Relationship)-[:TO]->()-[:SUBCLASS_OF*0..{str(self.SCD)}]->(b) ) )
+            )
+        OPTIONAL MATCH 
+            p1 = (a)-[:SUBCLASS_OF*0..{str(
+            self.SCD)}]->()<-[:FROM]-(r1:Relationship)-[:TO]->(crt_to1)<-[:SUBCLASS_OF*0..{str(self.SCD)}]-(b)
+        OPTIONAL MATCH
+            p2 = (a)<-[:SUBCLASS_OF*0..{str(
+            self.SCD)}]-()<-[:FROM]-(r2:Relationship)-[:TO]->(crt_to2)-[:SUBCLASS_OF*0..{str(self.SCD)}]->(b)
+        WITH a, b, 
+            collect(distinct {{
+                path: p1, 
+                rel_type: 
+                    CASE WHEN r1.relationship_type is NULL and $impute_relationship_type THEN 
+                        crt_to1.label
+                    ELSE
+                        r1.relationship_type
+                    END,   
+                short_label: r1.short_label, 
+                tag: 'p1'
+            }})
+            +
+            collect({{
+                path: p2, 
+                rel_type: 
+                    CASE WHEN r2.relationship_type is NULL THEN 
+                        crt_to2.label
+                    ELSE
+                        r2.relationship_type
+                    END,   
+                short_label: r2.short_label,               
+                tag: 'p2'
+            }})
+            as coll
+        UNWIND coll as map
+        WITH a, b, map, size(nodes(map['path'])) as sz 
+        WHERE not map['path'] is NULL
+        WITH *
+        ORDER BY map['tag'], sz //Here we prioritizing paths with SUBCLASS > over paths with < SUBCLASS rel. and then prioritize shorter paths  
+        WITH a, b, collect(map) as coll //ideally we should always have only 1 path for each pair, but allowing here for >1
+        WITH a, b, coll[0] as map        
+        //WITH apoc.map.mergeList(
+        //    [{{from: a.label, to: b.label, type: map['rel_type']}}] +
+        //        CASE WHEN short_label in keys(a) THEN [{{from_tag: a.short_label}}] ELSE [] END +
+        //        CASE WHEN short_label in keys(b) THEN [{{to_tag: b.short_label}}] ELSE [] END
+        //) as rel
+        WITH {{from: a.label, to: b.label, type: map['rel_type'], short_label: map['short_label']}} as rel
+        WITH *
+        ORDER BY rel['from'], rel['to'], rel['type']        
+        RETURN rel
+        """
+        olabels = [label for label in labels if label.endswith(oclass_marker)]
+        params = {
+            'labels': [(label[:-(len(oclass_marker))] if label in olabels else label) for label in labels],
+            'impute_relationship_type': impute_relationship_type
+        }
+        res = self.query(q, params)
+        rels = []
+        for r in res:
+            dct = r['rel']
+            if dct.get('from') in olabels or dct.get('to') in olabels:
+                dct['optional'] = True
+            rels.append(dct)
+        return rels
+
+    def translate_to_shortlabel(self, labels: list, rels: list, labels_to_pack, where_map: dict = None,
+                                where_rel_map: dict = None, use_rel_labels=True):
+        if not where_map:
+            where_map = {}
+        if not where_rel_map:
+            where_rel_map = {}
+
+        q = """
+        MATCH (c:Class)
+        WHERE c.label in $labels
+        RETURN apoc.map.fromPairs(collect([
+            c.label,
+            CASE WHEN 'short_label' in keys(c) THEN  
+                c.short_label
+            ELSE
+                c.label
+            END
+        ])) as map
+        """
+        params = {'labels': list(set(labels + [rel.get('from') for rel in rels] + [rel.get('to') for rel in rels]))}
+        assert labels_to_pack is None or isinstance(labels_to_pack, dict)
+        if labels_to_pack is not None:
+            labels_lst = []
+            for key, value in labels_to_pack.items():
+                assert isinstance(value,
+                                  (str, list)), f'Value in labels_to_pack is not string or list. It was: {type(value)}'
+                labels_lst.append(key)
+                if isinstance(value, str):
+                    labels_lst.append(value)
+                elif isinstance(value, list):
+                    labels_lst.extend(value)
+            params['labels'].extend(labels_lst)
+        # print(f'PARAMS: {params}')
+
+        res = self.query(q, params)
+        map = res[0]['map']
+        if use_rel_labels:
+            for rel in rels:
+                if rel.get('short_label'):
+                    map[rel['to']] = rel.get('short_label')
+        if not labels:
+            labels = []
+        labels = [{'label': label, 'short_label': map[label]} for label in labels]
+        if not rels:
+            rels = []
+        rels = [{**rel, **{'from': map[rel['from']], 'to': map[rel['to']]}} for rel in rels]
+
+        if labels_to_pack is not None:
+            mapped_labels_to_pack = {}
+            # print(f'MAP: {map}')
+            for key, value in labels_to_pack.items():
+                assert isinstance(value,
+                                  (str, list)), f'Value in labels_to_pack is not string or list. It was: {type(value)}'
+                if isinstance(value, str):
+                    mapped_labels_to_pack[map[key]] = map[value]
+                elif isinstance(value, list):
+                    # print(f'KEY: {key}')
+                    # print(f'VALUE: {value}')
+                    assert key in map.keys(), f'{key} was not found as a key in {map}'
+                    assert (True if i in map.keys() else False for i in
+                            value), f'a value from {value} was not found as a key in {map}'
+                    mapped_labels_to_pack[map[key]] = [map[i] for i in value]
+                    # convert the fromclass/coreclass label to short label only
+                    # leave the label as it needs to be long format for the generate_call function
+            labels_to_pack = mapped_labels_to_pack
+
+        if not where_map:
+            where_map = {}
+        where_map = {map[key]: item for key, item in where_map.items()}
+        where_rel_map = {map[key]: item for key, item in where_rel_map.items()}
+        return labels, rels, labels_to_pack, where_map, where_rel_map
+
+    @staticmethod
+    def arrows_dict_uri_dict_enrich(dct: dict, uri_map: dict):
+
+        def _gen_new_prop_name(neighbour: dict):
+            assert len({"label", "relationship", "property"}.intersection(neighbour.keys())) == 3
+            return f"{neighbour['relationship']}.{neighbour['label']}.{neighbour['property']}"
+
+        def _get_neighbour_id(nd: dict, neighbour: dict):
+            assert len({"label", "relationship", "property"}.intersection(neighbour.keys())) == 3
+            for rel in dct['relationships']:
+                if nd["id"] in [rel["toId"]] and rel["type"] == neighbour["relationship"]:
+                    return rel["fromId"]
+                elif nd["id"] in [rel["fromId"]] and rel["type"] == neighbour["relationship"]:
+                    return rel["toId"]
+            return None
+
+        def _get_neighbour_value(nd: dict, neighbour: dict):
+            neighbour_id = _get_neighbour_id(nd, neighbour)
+            for nd in dct['nodes']:
+                if nd['id'] == neighbour_id:
+                    return nd['properties'].get(neighbour["property"])
+
+        def _enrich_node(nd: dict, neighbour: str):
+            value = _get_neighbour_value(nd, neighbour)
+            return {**nd, **{"properties": {**nd["properties"], **{_gen_new_prop_name(neighbour): value}}}}
+
+        merge_on = {}
+        for key, item in uri_map.items():
+            merge_on[key] = item.get("properties").copy()
+            if not merge_on[key]:
+                merge_on[key] = []
+            if item.get('neighbours'):
+                for n in item['neighbours']:
+                    new_nodes = []
+                    for nd in dct['nodes']:
+                        if key in nd['labels']:
+                            new_nodes.append(_enrich_node(nd, n))
+                        else:
+                            new_nodes.append(nd)
+                    dct = {**dct, **{"nodes": new_nodes}}
+                    merge_on[key].append(_gen_new_prop_name(n))
+        return dct, merge_on
+
+    def create_ct(self, controlled_terminology: dict, identifier='label', order_terms=True, merge_on=None):
+        """
+        Creates :Term nodes and links them to a specified class with a [:HAS_CONTROLLED_TERM] relationship.
+        If order terms is True, an ascending Order property will be assigned to terms in the order they are created
+        accounting for the order of existing terms (if any) and [:NEXT] relationships between terms following this order.
+        For example:
+            With identifier = 'label' and controlled_terminology =
+            {
+                'class1': [{'term_label': 'term1'}, {'term_label': 'term2'}],
+                'class2': [{'term_label': 'term3'}]
+            }
+            3 new term nodes with 'term_label' properties equal to 'term1', 'term2' and 'term3' would be
+            created. The class with 'label' = 'class1' would then be linked by [:HAS_CONTROLLED_TERM]
+            relationships to 'term1' and 'term2' and similarly 'class2' would be linked to 'term3'
+
+        :param controlled_terminology: A dictionary of classes and terms eg: {'class1': [{prop1: value, prop2: value}, ...]}
+        :param identifier: String, property used when identifying classes to assign terms.
+        :param order_terms: Bool, if true order properties and next relationships will be created between terms.
+        :param merge_on: Optional List[string] term properties to merge on to prevent duplication
+        :return: neo4j result object.
+        """
+        ident_props = None
+        missing = self.get_missing_classes(list(controlled_terminology.keys()), identifier)
+        assert not missing, f'Cannot create controlled terminology for nonexistent classes: {missing}'
+
+        if merge_on:
+            ident_props = f'{{`{merge_on[0]}`: term_props["{merge_on[0]}"]'
+            for prop in merge_on[1:]:
+                ident_props += f', `{prop}`: term_props["{prop}"]'
+            ident_props += '}'
+
+        # Create terms
+        q1 = f"""
+        UNWIND KEYS($terminology) as class_label
+        MATCH (class:Class {{{identifier}: class_label}})
+        WITH class, class_label
+        UNWIND $terminology[class_label] as term_props
+        CALL apoc.merge.node(['Term'], {f"{ident_props}, term_props, term_props" if ident_props else 'term_props, {}, {}'}) YIELD node
+        CALL apoc.create.addLabels([node], [class.label]) YIELD node as term
+        MERGE (class)-[:HAS_CONTROLLED_TERM]->(term)
+        """
+        res1 = self.query(q1, {'terminology': controlled_terminology}, return_type='neo4j.Result')
+
+        if order_terms:
+            # Create order property on new terms
+            q2 = f"""
+            UNWIND $labels as class_label
+            MATCH (c:Class{{{identifier}: class_label}})
+            OPTIONAL MATCH (c)-[:HAS_CONTROLLED_TERM]->(term:Term)
+            WITH c, MAX(term.Order) as term_order
+            WITH c, CASE WHEN term_order IS NULL THEN 1 ELSE term_order + 1 END as term_order
+    
+            MATCH (c)-[:HAS_CONTROLLED_TERM]->(t1:Term)
+            WHERE t1.Order is NULL
+            WITH c, term_order, t1 order by t1.`Codelist Code`, t1.`Term Code` 
+            WITH c, collect(t1) as terms_to_order, term_order
+            WITH *, apoc.coll.zip(terms_to_order, range(term_order, term_order + size(terms_to_order))) as pairs
+            UNWIND pairs as pair
+            WITH pair[0] as term_node, pair[1] as new_order, c, terms_to_order
+            SET term_node.Order = new_order
+            return c, terms_to_order
+            """
+            self.query(q2, {'labels': list(controlled_terminology.keys())})
+
+            # Create next rel between terms
+            q3 = f"""
+            UNWIND $labels as class_label
+            MATCH (c:Class{{{identifier}: class_label}})-[:HAS_CONTROLLED_TERM]->(t:Term)
+            WITH c,t ORDER BY c.label, t.Order ASC
+            WITH c, COLLECT(t) AS terms
+            FOREACH (n IN RANGE(0, SIZE(terms)-2) |
+                FOREACH (prev IN [terms[n]] |
+                    FOREACH (next IN [terms[n+1]] |
+                        MERGE (prev)-[:NEXT]->(next))))
+            """
+            self.query(q3, {'labels': list(controlled_terminology.keys())})
+
+        return res1
+
+    def get_class_ct(self, class_: str, ct_prop_name='rdfs:label'):
+        q = """
+        MATCH (c:Class) 
+        WHERE c.label = $class_
+        OPTIONAL MATCH (c)-[:HAS_CONTROLLED_TERM]->(t:Term)
+        RETURN collect(DISTINCT t[$ct_prop_name]) as coll
+        """
+        params = {'class_': class_, 'ct_prop_name': ct_prop_name}
+        res = self.query(q, params)
+        if res:
+            return res[0]['coll']
+        else:
+            return []
+
+    def get_class_ct_map(self, classes: list, ct_props: list = None, identifier='label'):
+        """
+        Return controlled terminology for a given list of classes.
+        :param classes: list of class labels of class.identifier property values if using custom identifier
+                        for example: with identifier = 'short_label', classes = ['shortlabel1', 'shortlabel2']
+        :param ct_props: list of controlled terminology props to collect eg:
+                         ['label', 'Codelist Code', 'Order']
+                         defaults to ['rdfs:label']
+        :param identifier: string used when identifying classes
+        :return: Dictionary of classes and found controlled terminology for example:
+                 with classes = ['class1', 'class2'] and ct_props = ['label'] a typical result might be:
+                {'class1': [{'label': 'term1'}, {'label': 'term2'}], 'class2': [{{'label': 'term3'}}]}
+                Where 'class1' has two terms labeled 'term1' and 'term2' and 'class2' has one term labeled 'term3'
+        """
+
+        if ct_props is None:
+            ct_props = ['rdfs:label']
+        elif type(ct_props) == str:
+            ct_props = [ct_props]
+
+        prop_collection = f'["{ct_props[0]}", term.`{ct_props[0]}`]'
+        if len(ct_props) != 1:
+            for prop in ct_props[1:]:
+                prop_collection += f', ["{prop}", term.`{prop}`]'
+
+        q = f"""
+        UNWIND $classes as class
+        MATCH (c:Class)-[:HAS_CONTROLLED_TERM]->(term:Term)
+        WHERE c.`{identifier}` = class
+        WITH c, collect(apoc.map.fromPairs([{prop_collection}])) as terms
+        RETURN apoc.map.setKey({{}}, c.`{identifier}`, terms) as ct
+        """
+
+        params = {'classes': classes}
+        res = self.query(q, params)
+
+        data = {}
+        if res:
+            for term_dict in res:
+                # Flattened result {class.identifer:[[term.ct_props[0], ...], [term.ct_props[0], ...]]}
+                data.update(term_dict.get('ct'))
+        return data
+
+    def delete_ct(self, controlled_terminology: dict, ct_props: list, identifier='label'):
+        """
+        Deletes part of class specific controlled terminology.
+        :param controlled_terminology: Dictionary of key: class identity - value: list of class specific term property
+                                       values to delete. For example:
+                                       with ct_props = ['Codelist Code'] controlled terminology might be:
+                                      {'class1':[['code1'], ['code2']], class1':[['code2']]}
+                                      Note these property values must align with the keys defined in term_props!
+        :param ct_props: List of property names that define property values in a controlled terminology term,
+                         For example:
+                            With controlled terminology = {'class1':[['code1'], ['code2']], class1':[['code2']]}
+                            ct_props would be ['Codelist Code'] indicating that we intending to delete terms
+                            for 'class1' and 'class2' using 'Codelist Code' property value.
+        :param identifier: string, property used to identify class
+        :return: neo4j result object.
+        """
+        # TODO: Resolving [:NEXT] rel when deleting CT
+
+        where_clause = f't.`{ct_props[0]}` = term_props[0]'
+        for count, prop in enumerate(ct_props[1:], start=1):
+            where_clause += f' AND t.`{prop}` = term_props[{count}]'
+
+        q = f"""
+        UNWIND KEYS($terminology) as class_label
+        MATCH (c:Class)
+        WHERE c.`{identifier}` = class_label
+        UNWIND $terminology[class_label] as term_props
+        MATCH (c)-[:HAS_CONTROLLED_TERM]-(t:Term)
+        WHERE {where_clause}
+        DETACH DELETE t
+        """
+
+        return self.query(q, {'terminology': controlled_terminology}, return_type='neo4j.Result')
+
+    def get_all_ct(self, term_props: list, class_prop='label', derived_only=False):
+        """
+        Returns a list of dictionaries containing specified props for all controlled terminology.
+        Example:
+            With term_props = ['rdfs:label'] and class_prop = ['label'] the return format would be:
+            [{'label': class1, 'rdfs:label': 'term1'}, {'label': class1, 'rdfs:label': 'term2'},
+            {'label': class2, 'rdfs:label': 'term1'} ...]
+            Repeated for all CT.
+        :param term_props: Term properties to return eg: ['rdfs:label', 'Codelist Code']
+        :param class_prop: Class property used to identify controlled terminology class
+                            :param derived_only:
+        :param derived_only: Bool, optional filter for classes where class.derived = 'true'.
+        :return: List of dictionaries, see example above.
+        """
+        # TODO: consider converting to format similar to get_class_ct_map? ie {'class.label': [{'rdfs:label': 'term1'}]}
+        assert len(term_props) >= 1, 'Must include at least 1 term_prop'
+        assert class_prop not in term_props, 'Class prop cannot be in term props'
+
+        term_return = f'term.`{term_props[0]}` as `{term_props[0]}`'
+        for prop in term_props[1:]:
+            term_return += f', term.`{prop}` as `{prop}`'
+
+        q = f"""
+        MATCH (c:Class)-[:HAS_CONTROLLED_TERM]->(term:Term)
+        {'WHERE c.derived = "true"' if derived_only else ''}
+        RETURN c.`{class_prop}` as `{class_prop}`, {term_return}
+        """
+        return self.query(q)
+
+    def create_same_as_ct(self, same_as_terms: List[dict], term_identifiers: List[str], identifier='label'):
+        """
+        Creates a [:SAME_AS] relationship between two terms. For example:
+            With term_identifiers = ['Codelist Code', 'Term Code']
+            and same_as_terms = [
+                {'from_class': 'class1', 'to_class': 'class2', # Class identifiers
+                 'from_codelist_code': 'code_1', 'from_term_code': 'code_2', # Term 1 identifier
+                 'to_codelist_code: 'code_3', 'to_term_code': 'code_4' # Term 2 identifier
+                }
+            ]
+            A same as relationship would be created from a term of 'class1' with properties:
+            `Codelist Code` = code_1 and `Term Code` = 'code_2' to the corresponding term for 'class2'.
+
+            Note term identifiers in a same_as_terms dictionaries must be lowercase, use underscores instead of spaces
+            and be prefixed with from_ or to_ a property listed in term_identifiers.
+
+        :param same_as_terms: List of dictionaries defining same as terms between classes.
+        :param term_identifiers: List of strings with term properties that guarantee uniqueness
+        :param identifier: string class property used when matching classes
+        :return: neo4j result object
+        """
+
+        where_clause = f"WHERE c1.`{identifier}` = new_term['from_class'] AND c2.`{identifier}` = new_term['to_class']"
+        for term_prop in term_identifiers:
+            clean_prop = term_prop.lower().replace(' ', '_')
+            where_clause += f" AND t1.`{term_prop}` = new_term['from_{clean_prop}']"
+            where_clause += f" AND t2.`{term_prop}` = new_term['to_{clean_prop}']"
+
+        q = f"""
+        UNWIND $same_as_terms as new_term
+        MATCH (c1:Class)-[:HAS_CONTROLLED_TERM]-(t1:Term)
+        MATCH (c2:Class)-[:HAS_CONTROLLED_TERM]-(t2:Term)
+        {where_clause}
+        MERGE (t1)-[:SAME_AS]->(t2)
+        """
+        return self.query(q, {'same_as_terms': same_as_terms}, return_type='neo4j.Result')
+
+    def remove_same_as_ct(self, same_as_terms: List[dict], term_identifiers: List[str], identifier='label'):
+        """
+        Removes a [:SAME_AS] relationship between two terms, see "create_same_as_ct()" for format information.
+
+        :param same_as_terms: List of dictionaries defining same as terms between classes.
+        :param term_identifiers: List of strings with term properties that guarantee uniqueness
+        :param identifier: string class property used when matching classes
+        :return: neo4j result object
+        """
+
+        where_clause = f"WHERE c1.`{identifier}` = new_term['from_class'] AND c2.`{identifier}` = new_term['to_class']"
+        for term_prop in term_identifiers:
+            clean_prop = term_prop.lower().replace(' ', '_')
+            where_clause += f"AND t1.`{term_prop}` = new_term['from_{clean_prop}']"
+            where_clause += f"AND t2.`{term_prop}` = new_term['to_{clean_prop}']"
+
+        q = f"""
+        UNWIND $same_as_terms as new_term
+        MATCH (c1:Class)-[:HAS_CONTROLLED_TERM]->(t1:Term)-[rel:SAME_AS]->(t2:Term)<-[:HAS_CONTROLLED_TERM]-(c2:Class)
+        {where_clause}
+        DETACH DELETE rel
+        """
+
+        return self.query(q, {'same_as_terms': same_as_terms}, return_type='neo4j.Result')
+
+    def propagate_rels_to_parent_class(self):
+        if self.verbose:
+            logger.info("Copying Relationships to 'parent' Classes where (child)-[:SUBCLASS_OF]->(parent)")
+        self.query("""
+        MATCH (c:Class)<-[r1:TO|FROM]-(r:Relationship)-[r2:TO|FROM]-(target:Class), (c)-[:SUBCLASS_OF*1..50]->(source:Class)
+        WHERE type(r1) <> type(r2)
+        WITH *,
+        "
+            WITH $source as source, $target as target
+            MERGE (source)<-[:`"+type(r1)+"`]-(:Relationship{relationship_type:$type})-[:`"+type(r2)+"`]->(target)
+            RETURN count(*)
+        " as q, 
+        {type: r.relationship_type, source: source , target: target} as params
+        CALL apoc.cypher.doIt(q, params) YIELD value
+        RETURN value, q, params         
+        """)
+
+    def remove_unmapped_classes(self):
+        if self.verbose:
+            logger.info("Removing Unmapped Classes")
+        q = """
+        MATCH (c:Class)
+        WHERE NOT EXISTS (
+            ()-[:MAPS_TO_CLASS]->()-[:SUBCLASS_OF*0..50]->(c)
+        )
+        OPTIONAL MATCH (c)<-[:TO|FROM]-(r:Relationship)
+        REMOVE r:Relationship
+        REMOVE c:Class
+        """
+        self.query(q)
+
+    def remove_auxilary_term_labels(self):
+        if self.verbose:
+            logger.info("Removing Auxilary Term Labels")
+        """
+        To be used after reshaping - additional labels from Terms that have not been extracted from data are removed
+        :return:
+        """
+        q = """
+        MATCH (x:Term) 
+        WHERE not exists ( (x)-[:FROM_DATA]->() )
+        WITH x, labels(x) as coll
+        UNWIND coll as lbl
+        WITH *
+        WHERE NOT lbl in ["Term", "Class"]
+        CALL apoc.cypher.doIt(
+        'WITH x REMOVE x:`'+lbl+'`',
+        {x:x}
+        ) yield value
+        RETURN value
+        """
+        self.query(q)
+
+    def export_model_ttl(self, folder: str, filename: str, include_mappings=False):
+        uri_map1 = {
+            "Data Extraction Standard": {"properties": "_tag_"},
+            "Source Data Folder": {"properties": "_folder_"},
+            "Source Data Table": {"properties": "_domain_"},
+            "Source Data Column": {"properties": ["_domain_", "_columnname_"]}
+        }
+        uri_map2 = {key: item
+                    for key, item in ModelManager.URI_MAP.items()
+                    if key in ["Class", "Property", "Relationship"]}
+
+        if include_mappings:
+            self.rdf_generate_uri({**uri_map1, **uri_map2})
+            rdf = self.rdf_get_subgraph(
+                """
+                MATCH (n:Class)
+                call apoc.path.expand(n, 
+                    'SUBCLASS_OF|HAS_CONTROLLED_TERM>|<MAPS_TO_CLASS|<HAS_COLUMN|<HAS_TABLE|<TO|<FROM', 
+                    '+Class|+Term|+Relationship|+Data Extraction Standard|+Source Data Folder|+Source Data Table|+Source Data Column', 
+                    0, 1 ) yield path
+                RETURN path
+                """
+            )
+        else:
+            self.rdf_generate_uri(uri_map2)
+            rdf = self.rdf_get_subgraph(
+                """
+                MATCH (n:Class)
+                call apoc.path.expand(n, 'SUBCLASS_OF|HAS_CONTROLLED_TERM|<TO|<FROM', '+Class|+Relationship|+Term', 0, 1 ) yield path
+                RETURN path
+                """
+            )
+        rdf_file_path = os.path.join(folder, filename)
+        with open(rdf_file_path, "w") as file:
+            file.write(rdf)
+
+    def create_custom_mappings_from_dict(self, groupings = None) -> None:
+        """
+        Function to support MethodApplier(mode="schema_PROPERTY")
+
+        Create a set of nodes labeled "Class", all taken from the groupings dictionary; their names are
+            stored in an attribute named "label".  EXAMPLES: "Study", "Site", "Race", "Adverse Event".
+
+        Also, create a set of nodes labeled "Property"; likewise, their names are
+            stored in an attribute named "label".  EXAMPLES: "RACE", "RACEN", "SITEID".
+
+        In addition, create relationships named "HAS_PROPERTY", from each of the "Class" nodes to the appropriate
+            "Property" nodes.   EXAMPLE:  The "Race" node (labeled "Class") links to the "RACE", "RACEN" nodes
+            (labeled "Property")
+
+        Finally,  create relationships named "MAPS_TO_PROPERTY", from `Source Data Column` nodes to `Property` nodes.
+            These relationships are created based on matches between the "_columnname_" attribute on `Source Data Column` nodes
+            and entries in the lists contained in groupings (e.g., "RACEN"); in some cases, further restrictions are applied,
+            requiring the `Source Data Column` node to be linked to a particular `Source Data Table` node.
+
+        :param groupings:   A dictionary.  The keys are either "*" (meaning no `Source Data Table` restriction)
+                                           or the name of a specific `Source Data Table`.
+                                           The values are dictionaries such as {"Race": ["RACE", "RACEN"]}
+        :return:            None
+        """
+        if not groupings:
+            groupings = {}
+
+        # Loop over all the keys/values of the groupings dictionary
+        for table, groupping in groupings.items():
+            # EXAMPLES of table:  "ADSL" or "*" (the star indicates "all tables")
+            # groupping is a dictionary with entries such as  "Race": ["RACE", "RACEN"]
+
+            # Define the Cypher query, which depends on the value of the "table" variable in the outer loop;
+            #       for examples of how the query shapes up, see below (inside inner loop)
+            q = f"""                    
+                MERGE (class:Class {{label:$class}})
+                WITH * UNWIND $properties as property
+                MERGE (class)-[:HAS_PROPERTY]->(p:Property {{label:property}})
+                WITH *
+                MATCH (sdc:`Source Data Column` {{_columnname_:property}})
+                {
+                "" if table == "*" else "<-[:HAS_COLUMN]-(sdt:`Source Data Table` {_domain_:$table})"
+                }                     
+                MERGE (sdc)-[:MAPS_TO_PROPERTY]->(p)
+                """
+
+            for class_, properties in groupping.items():
+                # EXAMPLE of class_ : "Race"
+                # EXAMPLE of properties: ["RACE", "RACEN"]
+
+                params = {"table":table, "class": class_, "properties": properties}
+                self.query(q, params)
+
+                # EXAMPLE1 of query (involving a specific table, such as "ADSL")
+                """
+                    MERGE (class:Class {label:$class})
+                    WITH * UNWIND $properties as property
+                    MERGE (class)-[:HAS_PROPERTY]->(p:Property {label:property})
+                    WITH *
+                    MATCH (sdc:`Source Data Column` {_columnname_:property})
+                    <-[:HAS_COLUMN]-(sdt:`Source Data Table` {_domain_:$table})                     
+                    MERGE (sdc)-[:MAPS_TO_PROPERTY]->(p)
+                """
+
+                # EXAMPLE2 of query (involving any table, indicated by the "*" value of the table variable)
+                """
+                    MERGE (class:Class {label:$class})
+                    WITH * UNWIND $properties as property
+                    MERGE (class)-[:HAS_PROPERTY]->(p:Property {label:property})
+                    WITH *
+                    MATCH (sdc:`Source Data Column` {_columnname_:property})                     
+                    MERGE (sdc)-[:MAPS_TO_PROPERTY]->(p)
+                """
+                # EXAMPLE of params: {'table': 'ADSL', 'class': 'Race', 'properties': ['RACE', 'RACEN']}
+
+    def create_custom_rels_from_list(self, rels: [[str, str]], create_if_absent = False) -> None:
+        """
+        Adds "CLASS_RELATES_TO" relationships to pairs of nodes with "Class" label,
+        based on the list passed as the argument "rels".
+        Matches occur based on node attributes named "label".
+        Optionally, create the Class nodes if needed.
+        To create just a single relationship, see create_class_relationship()
+
+        NOTE: this is a more general version of the method create_related_classes_from_list()
+
+        :param rels:    A list of 2-element lists, indicating a relationship among nodes of type `Class`
+                        EXAMPLE:   [
+                                        ["Study", "Site"],
+                                        ["Study", "Subject"],
+                                        ["Subject", "Race"]
+                                   ]
+        :param create_if_absent: If True, the Class nodes specified in the argument "rel" get created as needed;
+                                        otherwise, no relationships get created whenever their start or end class is missing
+        :return:                 None
+        """
+        if rels is None or rels == []:
+            return      # There's nothing to do
+
+        if create_if_absent:
+            q = f"""            
+                UNWIND $rels as rel
+                WITH rel[0] as left, rel[1] as right      
+                WHERE apoc.meta.type(left) = apoc.meta.type(right) = 'STRING'  
+                MERGE (ln:Class {{label:left}})
+                MERGE (rn:Class {{label:right}})   
+                MERGE (ln)-[:CLASS_RELATES_TO]->(rn)   
+                """
+        else:   # The Class nodes MUST be present, or no relationship gets created
+            q = f"""            
+                UNWIND $rels as rel
+                WITH rel[0] as left, rel[1] as right    
+                WHERE apoc.meta.type(left) = apoc.meta.type(right) = 'STRING'      
+                MATCH (ln:Class {{label:left}}), (rn:Class {{label:right}})    
+                MERGE (ln)-[:CLASS_RELATES_TO]->(rn)   
+                """
+
+        params = {"rels": rels}
+        self.query(q, params)
+
+    def create_model_from_data(
+            self,
+            data_label: str = "Source Data Row",
+            data_table_label: str = "Source Data Table",
+            domain_property: str = "_domain_",
+            no_domain_label: str = "Thing",
+            data_column_label: str = "Source Data Column",
+            columnname_property: str = "_columnname_",
+            exclude_properties: list = None,
+    ):
+        """
+        Creates Class and Relationship nodes to represent a trivial schema to reshape data ingested e.g. with
+        FileDataLoader - Tables loaded into nodes one row to one node, column names used as property names.
+
+        data_labels: labels of the nodes where loaded data is stored (mm with use OR btw labels to fetch data nodes)
+        domain_property: property where the name of the table/domain can be found
+        """
+        if exclude_properties is None:
+            exclude_properties = ["_filename_", "_folder_"]
+        q = f"""
+        MATCH (data:`{data_label}`)<-[:HAS_DATA]-(dt:`{data_table_label}`)        
+        WITH distinct dt, dt._domain_ as domain, keys(data) as ks
+        WITH *, CASE WHEN domain IS NULL THEN $no_domain_label ELSE domain END as domain
+        WITH dt, domain, [k in ks WHERE NOT k IN $exclude_properties] as ks
+        WITH dt, domain, apoc.coll.flatten(apoc.coll.toSet(ks)) as ks
+        MERGE (c:Class{{label: domain, short_label: domain, create: True}})
+        MERGE (dt)-[:MAPS_TO_CLASS]->(c)
+        WITH *
+        UNWIND ks as k
+        MATCH (dt)-[:HAS_COLUMN]->(col:`{data_column_label}`)
+        WHERE col.`{columnname_property}` = k
+        MERGE (c2:Class{{label: k, short_label: k}})        
+        MERGE (c)<-[:FROM]-(r:Relationship{{relationship_type: k}})-[:TO]->(c2)
+        MERGE (col)-[:MAPS_TO_CLASS]->(c2)        
+        """
+        params = {
+            "exclude_properties": exclude_properties + [domain_property],
+            "no_domain_label": no_domain_label
+        }
         self.query(q, params)
```

### Comparing `tab2neo-1.2.1.0/setup.py` & `tab2neo-1.2.5.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-import setuptools
-import os
-
-with open("README.md", "r") as fh:
-    long_description = fh.read()
-
-def read_text(file_name: str):
-    return open(os.path.join(file_name)).read()
-
-with open('requirements.txt') as f:
-    requirements = f.read().splitlines()
-
-required = []
-dependency_links = []
-
-# Do not add to required lines pointing to Git repositories
-EGG_MARK = '#egg='
-for line in requirements:
-    if line.startswith('-e git:') or line.startswith('-e git+') or \
-            line.startswith('git:') or line.startswith('git+'):
-        if EGG_MARK in line:
-            package_name = line[line.find(EGG_MARK) + len(EGG_MARK):]
-            required.append(package_name)
-            dependency_links.append(line)
-        else:
-            print('Dependency to a git repository should have the format:')
-            print('git+ssh://git@github.com/xxxxx/xxxxxx#egg=package_name')
-    else:
-        required.append(line)
-
-setuptools.setup(
-    name="tab2neo",                         # This is the name of the package
-    version="1.2.1.0",                      # Release.Major Feature.Minor Feature.Bug Fix
-    author="Alexey Kuznetsov",              # Full name of the author
-    description="Clinical Linked Data: High-level Python classes to load, model and reshape tabular data imported into Neo4j database",
-    long_description=long_description,      # Long description read from the the readme file
-    long_description_content_type="text/markdown",
-    packages=setuptools.find_packages(include=[
-        "logger",
-        "analysis_metadata",
-        "derivation_method",
-        "data_loaders",
-        "data_providers",
-        "model_appliers",
-        "model_managers",
-        "query_builders",
-        "method_appliers"
-    ]),    # List of all python modules to be installed
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "Operating System :: OS Independent",
-    ],                                      # Information to filter the project on PyPi website
-    license=read_text("LICENSE"),
-    python_requires='>=3.6',                # Minimum version requirement of the package
-    # package_dir={'':''},                  # Directory of the source code of the package
-    install_requires=required,
-    dependency_links=dependency_links
-)
+import setuptools
+import os
+
+with open("README.md", "r") as fh:
+    long_description = fh.read()
+
+def read_text(file_name: str):
+    return open(os.path.join(file_name)).read()
+
+with open('requirements.txt') as f:
+    requirements = f.read().splitlines()
+
+required = []
+dependency_links = []
+
+# Do not add to required lines pointing to Git repositories
+EGG_MARK = '#egg='
+for line in requirements:
+    if line.startswith('-e git:') or line.startswith('-e git+') or \
+            line.startswith('git:') or line.startswith('git+'):
+        if EGG_MARK in line:
+            package_name = line[line.find(EGG_MARK) + len(EGG_MARK):]
+            required.append(package_name)
+            dependency_links.append(line)
+        else:
+            print('Dependency to a git repository should have the format:')
+            print('git+ssh://git@github.com/xxxxx/xxxxxx#egg=package_name')
+    else:
+        required.append(line)
+
+setuptools.setup(
+    name="tab2neo",                         # This is the name of the package
+    version="1.2.5.0",                      # Release.Major Feature.Minor Feature.Bug Fix
+    author="Alexey Kuznetsov",              # Full name of the author
+    description="Clinical Linked Data: High-level Python classes to load, model and reshape tabular data imported into Neo4j database",
+    long_description=long_description,      # Long description read from the the readme file
+    long_description_content_type="text/markdown",
+    packages=setuptools.find_packages(include=[
+        "logger",
+        "analysis_metadata",
+        "derivation_method",
+        "data_loaders",
+        "data_providers",
+        "model_appliers",
+        "model_managers",
+        "query_builders",
+        "method_appliers"
+    ]),    # List of all python modules to be installed
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "Operating System :: OS Independent",
+    ],                                      # Information to filter the project on PyPi website
+    license=read_text("LICENSE"),
+    python_requires='>=3.6',                # Minimum version requirement of the package
+    # package_dir={'':''},                  # Directory of the source code of the package
+    install_requires=required,
+    dependency_links=dependency_links
+)
```

### Comparing `tab2neo-1.2.1.0/tab2neo.egg-info/SOURCES.txt` & `tab2neo-1.2.5.0/tab2neo.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 data_providers/data_provider.py
 logger/__init__.py
 logger/logger.py
 model_appliers/__init__.py
 model_appliers/model_applier.py
 model_managers/__init__.py
 model_managers/model_manager.py
+model_managers/temp.py
 query_builders/__init__.py
 query_builders/query_builder.py
 tab2neo.egg-info/PKG-INFO
 tab2neo.egg-info/SOURCES.txt
 tab2neo.egg-info/dependency_links.txt
 tab2neo.egg-info/requires.txt
-tab2neo.egg-info/top_level.txt
+tab2neo.egg-info/top_level.txt
+tests/test_comparison_utilities.py
```

### Comparing `tab2neo-1.2.1.0/tab2neo.egg-info/requires.txt` & `tab2neo-1.2.5.0/tab2neo.egg-info/requires.txt`

 * *Files identical despite different names*

