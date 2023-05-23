# Comparing `tmp/ScriptCollection-3.3.92-py3-none-any.whl.zip` & `tmp/ScriptCollection-3.3.93-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 57600 bytes, number of entries: 14
+Zip file size: 57992 bytes, number of entries: 14
 -rw-rw-rw-  2.0 fat    18064 b- defN 23-Mar-05 15:39 ScriptCollection/Executables.py
 -rw-rw-rw-  2.0 fat    34139 b- defN 23-May-20 16:21 ScriptCollection/GeneralUtilities.py
 -rw-rw-rw-  2.0 fat     1937 b- defN 22-Aug-30 21:59 ScriptCollection/ProgramRunnerBase.py
 -rw-rw-rw-  2.0 fat     6273 b- defN 22-Oct-16 19:55 ScriptCollection/ProgramRunnerEpew.py
 -rw-rw-rw-  2.0 fat     3023 b- defN 22-Aug-30 21:59 ScriptCollection/ProgramRunnerPopen.py
--rw-rw-rw-  2.0 fat    86233 b- defN 23-May-20 18:53 ScriptCollection/ScriptCollectionCore.py
--rw-rw-rw-  2.0 fat   129034 b- defN 23-May-20 18:20 ScriptCollection/TasksForCommonProjectStructure.py
+-rw-rw-rw-  2.0 fat    86233 b- defN 23-May-23 21:53 ScriptCollection/ScriptCollectionCore.py
+-rw-rw-rw-  2.0 fat   130752 b- defN 23-May-23 21:53 ScriptCollection/TasksForCommonProjectStructure.py
 -rw-rw-rw-  2.0 fat     7918 b- defN 22-Aug-30 21:59 ScriptCollection/UpdateCertificates.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Aug-29 05:45 ScriptCollection/__init__.py
--rw-rw-rw-  2.0 fat     7864 b- defN 23-May-20 18:54 ScriptCollection-3.3.92.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-20 18:54 ScriptCollection-3.3.92.dist-info/WHEEL
--rw-rw-rw-  2.0 fat     1968 b- defN 23-May-20 18:54 ScriptCollection-3.3.92.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       17 b- defN 23-May-20 18:54 ScriptCollection-3.3.92.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1295 b- defN 23-May-20 18:54 ScriptCollection-3.3.92.dist-info/RECORD
-14 files, 297857 bytes uncompressed, 55408 bytes compressed:  81.4%
+-rw-rw-rw-  2.0 fat     7864 b- defN 23-May-23 21:54 ScriptCollection-3.3.93.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-23 21:54 ScriptCollection-3.3.93.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat     1968 b- defN 23-May-23 21:54 ScriptCollection-3.3.93.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       17 b- defN 23-May-23 21:54 ScriptCollection-3.3.93.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1295 b- defN 23-May-23 21:54 ScriptCollection-3.3.93.dist-info/RECORD
+14 files, 299575 bytes uncompressed, 55800 bytes compressed:  81.4%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: ScriptCollection/UpdateCertificates.py
 Comment: 
 
 Filename: ScriptCollection/__init__.py
 Comment: 
 
-Filename: ScriptCollection-3.3.92.dist-info/METADATA
+Filename: ScriptCollection-3.3.93.dist-info/METADATA
 Comment: 
 
-Filename: ScriptCollection-3.3.92.dist-info/WHEEL
+Filename: ScriptCollection-3.3.93.dist-info/WHEEL
 Comment: 
 
-Filename: ScriptCollection-3.3.92.dist-info/entry_points.txt
+Filename: ScriptCollection-3.3.93.dist-info/entry_points.txt
 Comment: 
 
-Filename: ScriptCollection-3.3.92.dist-info/top_level.txt
+Filename: ScriptCollection-3.3.93.dist-info/top_level.txt
 Comment: 
 
-Filename: ScriptCollection-3.3.92.dist-info/RECORD
+Filename: ScriptCollection-3.3.93.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ScriptCollection/ScriptCollectionCore.py

```diff
@@ -21,15 +21,15 @@
 from PyPDF2 import PdfFileMerger
 from .GeneralUtilities import GeneralUtilities
 from .ProgramRunnerBase import ProgramRunnerBase
 from .ProgramRunnerPopen import ProgramRunnerPopen
 from .ProgramRunnerEpew import ProgramRunnerEpew, CustomEpewArgument
 
 
-version = "3.3.92"
+version = "3.3.93"
 __version__ = version
 
 
 class ScriptCollectionCore:
 
     # The purpose of this property is to use it when testing your code which uses scriptcollection for external program-calls.
     # Do not change this value for productive environments.
```

## ScriptCollection/TasksForCommonProjectStructure.py

```diff
@@ -1,17 +1,19 @@
 from datetime import datetime
 from graphlib import TopologicalSorter
 import os
 from pathlib import Path
+from functools import cmp_to_key
 import shutil
 import re
 import urllib.request
 import zipfile
 import json
 import configparser
+from packaging import version
 import xmlschema
 from OpenSSL import crypto
 from lxml import etree
 from .GeneralUtilities import GeneralUtilities
 from .ScriptCollectionCore import ScriptCollectionCore
 from .ProgramRunnerEpew import ProgramRunnerEpew
 
@@ -209,18 +211,22 @@
         sc = ScriptCollectionCore()
         folder = os.path.dirname(os.path.realpath(buildscript_file))
         codeunit_folder = GeneralUtilities.resolve_relative_path("../..", folder)
         result = sc.run_program_argsasarray("git", ["ls-tree", "-r", "HEAD", "--name-only"], codeunit_folder)
         files = [f for f in result[1].split('\n') if len(f) > 0]
         for file in files:
             full_source_file = os.path.join(codeunit_folder, file)
-            target_file = os.path.join(codeunit_folder, "Other", "Artifacts", "SourceCode", file)
-            target_folder = os.path.dirname(target_file)
-            GeneralUtilities.ensure_directory_exists(target_folder)
-            shutil.copyfile(full_source_file, target_file)
+            if os.path.isfile(full_source_file):
+                # Reson of isdir-check:
+                # Prevent trying to copy files which are not exist.
+                # Otherwise exceptions occurr because uncommitted deletions of files will result in an error here.
+                target_file = os.path.join(codeunit_folder, "Other", "Artifacts", "SourceCode", file)
+                target_folder = os.path.dirname(target_file)
+                GeneralUtilities.ensure_directory_exists(target_folder)
+                shutil.copyfile(full_source_file, target_file)
 
     @GeneralUtilities.check_arguments
     def standardized_tasks_build_for_python_codeunit(self, buildscript_file: str, verbosity: int, targetenvironmenttype: str, commandline_arguments: list[str]):
         self.copy_source_files_to_output_directory(buildscript_file)
         codeunitname: str = Path(os.path.dirname(buildscript_file)).parent.parent.name
         verbosity = TasksForCommonProjectStructure.get_verbosity_from_commandline_arguments(commandline_arguments,  verbosity)
         codeunit_folder = str(Path(os.path.dirname(buildscript_file)).parent.parent.absolute())
@@ -827,14 +833,15 @@
   </head>
 
   <body>
     <h1>{title}</h1>
     <hr/>
     Available reference-content for {codeunitname}:<br>
     {repo_url_html}<br>
+    <!--TODO add artefacts-link: <a href="./x">Artefacts</a><br>-->
     <a href="./Reference/index.html">Reference</a><br>
     <a href="./DiffReport/DiffReport.html">Diff-report</a><br>
     {coverage_report_link}
   </body>
 
 </html>
 """
@@ -883,20 +890,45 @@
             self.__export_codeunit_reference_content_to_reference_repository("Latest", True, reference_folder, information.repository,
                                                                              codeunitname, information.projectname, codeunit_version, information.public_repository_url,
                                                                              information.target_branch_name)
 
             # Generate reference
             self.__generate_entire_reference(information.projectname, project_version, reference_folder)
 
+    @staticmethod
+    @GeneralUtilities.check_arguments
+    def _internal_sort_reference_folder(folder1: str, folder2: str) -> int:
+        """Returns a value greater than 0 if and only if folder1 has a base-folder-name with a with a higher version than the base-folder-name of folder2.
+        Returns a value lower than 0 if and only if folder1 has a base-folder-name with a with a lower version than the base-folder-name of folder2.
+        Returns 0 if both values are equal."""
+        if (folder1 == folder2):
+            return 0
+
+        version_identifier_1 = os.path.basename(folder1)
+        if version_identifier_1 == "Latest":
+            return -1
+        version_identifier_1 = version_identifier_1[1:]
+
+        version_identifier_2 = os.path.basename(folder2)
+        if version_identifier_2 == "Latest":
+            return 1
+        version_identifier_2 = version_identifier_2[1:]
+
+        if version.parse(version_identifier_1) < version.parse(version_identifier_2):
+            return -1
+        elif version.parse(version_identifier_1) > version.parse(version_identifier_2):
+            return 1
+        else:
+            return 0
+
     @GeneralUtilities.check_arguments
     def __generate_entire_reference(self, projectname: str, project_version: str, reference_folder: str) -> None:
-        all_available_version_identifier_folders_of_reference = list(
-            folder for folder in GeneralUtilities.get_direct_folders_of_folder(reference_folder))
-        all_available_version_identifier_folders_of_reference.reverse()  # move newer versions above
-        all_available_version_identifier_folders_of_reference.insert(0, all_available_version_identifier_folders_of_reference.pop())  # move latest version to the top
+        all_available_version_identifier_folders_of_reference: list[str] = list(folder for folder in GeneralUtilities.get_direct_folders_of_folder(reference_folder))
+        all_available_version_identifier_folders_of_reference = sorted(all_available_version_identifier_folders_of_reference,
+                                                                       key=cmp_to_key(TasksForCommonProjectStructure._internal_sort_reference_folder))
         reference_versions_html_lines = []
         reference_versions_html_lines.append('    <hr/>')
         for all_available_version_identifier_folder_of_reference in all_available_version_identifier_folders_of_reference:
             version_identifier_of_project = os.path.basename(all_available_version_identifier_folder_of_reference)
             if version_identifier_of_project == "Latest":
                 latest_version_hint = f" (v{project_version})"
             else:
@@ -1127,35 +1159,35 @@
         sbom_folder = os.path.join(artifacts_folder, "BOM")
         codeunitversion = self.get_version_of_codeunit(os.path.join(codeunit_folder, f"{codeunitname}.codeunit.xml"))
         GeneralUtilities.ensure_directory_exists(sbom_folder)
         self.__sc.run_program_argsasarray("docker", ["sbom", "--format", "cyclonedx", f"{codeunitname_lower}:{codeunitversion}",
                                                      "--output", f"{codeunitname}.{codeunitversion}.sbom.xml"], sbom_folder, verbosity=verbosity, print_errors_as_information=True)
 
     @GeneralUtilities.check_arguments
-    def push_docker_build_artifact(self, push_artifacts_file: str, registry: str, product_name: str, codeunitname: str,
+    def push_docker_build_artifact(self, push_artifacts_file: str, registry: str, project_name: str, codeunitname: str,
                                    verbosity: int, push_readme: bool, commandline_arguments: list[str], repository_folder_name: str):
         folder_of_this_file = os.path.dirname(push_artifacts_file)
         verbosity = TasksForCommonProjectStructure.get_verbosity_from_commandline_arguments(commandline_arguments, verbosity)
         repository_folder = GeneralUtilities.resolve_relative_path(f"..{os.path.sep}..{os.path.sep}Submodules{os.path.sep}{repository_folder_name}", folder_of_this_file)
         codeunit_folder = os.path.join(repository_folder, codeunitname)
         artifacts_folder = self.get_artifacts_folder(repository_folder, codeunitname)
         applicationimage_folder = os.path.join(artifacts_folder, "BuildResult_OCIImage")
         sc = ScriptCollectionCore()
         image_file = sc.find_file_by_extension(applicationimage_folder, "tar")
         image_filename = os.path.basename(image_file)
-        version = self.get_version_of_codeunit(os.path.join(codeunit_folder, f"{codeunitname}.codeunit.xml"))
+        codeunit_version = self.get_version_of_codeunit(os.path.join(codeunit_folder, f"{codeunitname}.codeunit.xml"))
         image_tag_name = codeunitname.lower()
         repo = f"{registry}/{image_tag_name}"
         image_latest = f"{repo}:latest"
-        image_version = f"{repo}:{version}"
+        image_version = f"{repo}:{codeunit_version}"
         GeneralUtilities.write_message_to_stdout("Load image...")
         sc.run_program("docker", f"load --input {image_filename}", applicationimage_folder, verbosity=verbosity)
         GeneralUtilities.write_message_to_stdout("Tag image...")
-        sc.run_program("docker", f"tag {image_tag_name}:{version} {image_latest}", verbosity=verbosity)
-        sc.run_program("docker", f"tag {image_tag_name}:{version} {image_version}", verbosity=verbosity)
+        sc.run_program("docker", f"tag {image_tag_name}:{codeunit_version} {image_latest}", verbosity=verbosity)
+        sc.run_program("docker", f"tag {image_tag_name}:{codeunit_version} {image_version}", verbosity=verbosity)
         GeneralUtilities.write_message_to_stdout("Push image...")
         sc.run_program("docker", f"push {image_latest}", verbosity=verbosity)
         sc.run_program("docker", f"push {image_version}", verbosity=verbosity)
         if push_readme:
             sc.run_program("docker", f"pushrm {repo}", codeunit_folder, verbosity=verbosity)
 
     @GeneralUtilities.check_arguments
@@ -1302,17 +1334,17 @@
     @GeneralUtilities.check_arguments
     def get_version_of_project(self, repository_folder: str):
         return ScriptCollectionCore().get_semver_version_from_gitversion(repository_folder)
 
     @GeneralUtilities.check_arguments
     def replace_common_variables_in_nuspec_file(self, codeunit_folder: str):
         codeunit_name = os.path.basename(codeunit_folder)
-        version = self.get_version_of_codeunit_folder(codeunit_folder)
+        codeunit_version = self.get_version_of_codeunit_folder(codeunit_folder)
         nuspec_file = os.path.join(codeunit_folder, "Other", "Build", f"{codeunit_name}.nuspec")
-        self.__sc.replace_version_in_nuspec_file(nuspec_file, version)
+        self.__sc.replace_version_in_nuspec_file(nuspec_file, codeunit_version)
 
     @GeneralUtilities.check_arguments
     def standardized_tasks_build_for_node_project(self, build_script_file: str, build_environment_target_type: str,
                                                   verbosity: int, commandline_arguments: list[str]):
         # TODO use unused parameter
         self.copy_source_files_to_output_directory(build_script_file)
         sc = ScriptCollectionCore()
@@ -1483,25 +1515,25 @@
     def generate_openapi_file(self, buildscript_file: str, runtime: str, verbosity: int, commandline_arguments: list[str],
                               swagger_document_name: str = "APISpecification") -> None:
         codeunitname = os.path.basename(str(Path(os.path.dirname(buildscript_file)).parent.parent.absolute()))
         repository_folder = str(Path(os.path.dirname(buildscript_file)).parent.parent.parent.absolute())
         artifacts_folder = os.path.join(repository_folder, codeunitname, "Other", "Artifacts")
         GeneralUtilities.ensure_directory_exists(os.path.join(artifacts_folder, "APISpecification"))
         verbosity = self.get_verbosity_from_commandline_arguments(commandline_arguments, verbosity)
-        version = self.get_version_of_codeunit_folder(os.path.join(repository_folder, codeunitname))
-        self.__sc.run_program("swagger", f"tofile --output APISpecification\\{codeunitname}.v{version}.api.json" +
+        codeunit_version = self.get_version_of_codeunit_folder(os.path.join(repository_folder, codeunitname))
+        self.__sc.run_program("swagger", f"tofile --output APISpecification\\{codeunitname}.v{codeunit_version}.api.json" +
                               f" BuildResult_DotNet_{runtime}\\{codeunitname}.dll {swagger_document_name}",
                               artifacts_folder, verbosity=verbosity)
 
     @GeneralUtilities.check_arguments
-    def replace_version_in_packagejson_file(self, packagejson_file: str, version: str):
+    def replace_version_in_packagejson_file(self, packagejson_file: str, codeunit_version: str):
         encoding = "utf-8"
         with open(packagejson_file, encoding=encoding) as f:
             data = json.load(f)
-        data['version'] = version
+        data['version'] = codeunit_version
         with open(packagejson_file, 'w', encoding=encoding) as f:
             json.dump(data, f, indent=2)
 
     @GeneralUtilities.check_arguments
     def build_dependent_code_units(self, repo_folder: str, codeunit_name: str, verbosity: int, target_environmenttype: str,
                                    additional_arguments_file: str) -> None:
         codeunit_file = os.path.join(repo_folder, codeunit_name, codeunit_name + ".codeunit.xml")
@@ -1814,28 +1846,28 @@
         execution_result = self.__sc.run_program(
             "python", f"GenerateReference.py{additional_arguments_g}{general_argument}", reference_folder, verbosity=verbosity_for_executed_programs, throw_exception_if_exitcode_is_not_zero=False)
         if execution_result[0] != 0:
             raise ValueError(f"GenerateReference.py resulted in exitcode {execution_result[0]}. StdOut: '{execution_result[1]}' StdOut: '{execution_result[2]}'")
         self.verify_artifact_exists(codeunit_folder, dict[str, bool]({"Reference": True}))
 
         artifactsinformation_file = os.path.join(artifacts_folder, f"{codeunit_name}.artifactsinformation.xml")
-        version = self.get_version_of_codeunit(codeunit_file)
+        codeunit_version = self.get_version_of_codeunit(codeunit_file)
         GeneralUtilities.ensure_file_exists(artifactsinformation_file)
         artifacts_list = []
         for artifact_folder in GeneralUtilities.get_direct_folders_of_folder(artifacts_folder):
             artifact_name = os.path.basename(artifact_folder)
             artifacts_list.append(f"        <cps:artifact>{artifact_name}<cps:artifact>")
         artifacts = '\n'.join(artifacts_list)
         moment = GeneralUtilities.datetime_to_string(now)
         # TODO implement usage of self.reference_latest_version_of_xsd_when_generating_xml
         GeneralUtilities.write_text_to_file(artifactsinformation_file, f"""<?xml version="1.0" encoding="UTF-8" ?>
 <cps:artifactsinformation xmlns:cps="https://projects.aniondev.de/PublicProjects/Common/ProjectTemplates/-/tree/main/Conventions/RepositoryStructure/CommonProjectStructure" artifactsinformationspecificationversion="1.0.0"
     xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="https://raw.githubusercontent.com/anionDev/ProjectTemplates/main/Templates/Conventions/RepositoryStructure/CommonProjectStructure/artifactsinformation.xsd">
     <cps:name>{codeunit_name}</cps:name>
-    <cps:version>{version}</cps:version>
+    <cps:version>{codeunit_version}</cps:version>
     <cps:timestamp>{moment}</cps:timestamp>
     <cps:targetenvironmenttype>{target_environmenttype}</cps:targetenvironmenttype>
     <cps:artifacts>
 {artifacts}
     </cps:artifacts>
 </cps:artifactsinformation>""")
         # TODO validate artifactsinformation_file against xsd
```

## Comparing `ScriptCollection-3.3.92.dist-info/METADATA` & `ScriptCollection-3.3.93.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ScriptCollection
-Version: 3.3.92
+Version: 3.3.93
 Summary: The ScriptCollection is the place for reusable scripts.
 Home-page: https://github.com/anionDev/ScriptCollection
 Author: Marius Göcke
 Author-email: marius.goecke@gmail.com
 Project-URL: Documentation, https://aniondev.github.io/ScriptCollectionReference/index.html
 Project-URL: Changelog, https://github.com/anionDev/ScriptCollection/tree/main/Other/Resources/Changelog
 Keywords: package release build management
```

## Comparing `ScriptCollection-3.3.92.dist-info/entry_points.txt` & `ScriptCollection-3.3.93.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `ScriptCollection-3.3.92.dist-info/RECORD` & `ScriptCollection-3.3.93.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ScriptCollection/Executables.py,sha256=kXTIX92KLeFuxnYOlsyFs5lkznsxkuoBMVrV3OU7FZU,18064
 ScriptCollection/GeneralUtilities.py,sha256=7-KuXjS_S-oiMcMM9bEDGx8n4RlnGxGpqHdhXhN47I8,34139
 ScriptCollection/ProgramRunnerBase.py,sha256=2kyOuoM3oFjBfLc9Q5t5RTz7Ya2CjUxFtB1rBBDmnjU,1937
 ScriptCollection/ProgramRunnerEpew.py,sha256=ZiBZVMcsphmo49z2BwUwQYXo2uTKXPu33QW3IxCT46E,6273
 ScriptCollection/ProgramRunnerPopen.py,sha256=HOs1QVnXiQtwXy1_xvH79bWBdd0i-2tUyyLloQBvMto,3023
-ScriptCollection/ScriptCollectionCore.py,sha256=441FIJMhdYMpRRCSo223Qtr8G_ffPB6Go_9rq1XPkcg,86233
-ScriptCollection/TasksForCommonProjectStructure.py,sha256=Zg_aBGA5K8oA06l79HYT_Tm7lERE1Ym3JLtqUVyT7ys,129034
+ScriptCollection/ScriptCollectionCore.py,sha256=IoZc3kmwLjrP9QAeTU_clHWwHc3Np816lACKKhNC1F8,86233
+ScriptCollection/TasksForCommonProjectStructure.py,sha256=_R5kBf88cySZE_5q6Cch9eRddwbJrRzsBFTISVXFhr0,130752
 ScriptCollection/UpdateCertificates.py,sha256=Go-JJK-YTi7aBB1phlLxypa8GHkmFHBEPB0_TT9G-bw,7918
 ScriptCollection/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ScriptCollection-3.3.92.dist-info/METADATA,sha256=Y8ligCMf2s3o4k0XqbBkfXMwIMJXaI54VYsHEPYx4qA,7864
-ScriptCollection-3.3.92.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ScriptCollection-3.3.92.dist-info/entry_points.txt,sha256=VIuxVCOpX38lSJUwRRENBNgcGKTIBxQyrCfbJVRHP8g,1968
-ScriptCollection-3.3.92.dist-info/top_level.txt,sha256=hY2hOVH0V0Ce51WB76zKkIWTUNwMUdHo4XDkR2vYVwg,17
-ScriptCollection-3.3.92.dist-info/RECORD,,
+ScriptCollection-3.3.93.dist-info/METADATA,sha256=vKTeuSCESq0cj4EsHBNWMF2f3QgdLXZSpQ4-Dyp6ZwA,7864
+ScriptCollection-3.3.93.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ScriptCollection-3.3.93.dist-info/entry_points.txt,sha256=VIuxVCOpX38lSJUwRRENBNgcGKTIBxQyrCfbJVRHP8g,1968
+ScriptCollection-3.3.93.dist-info/top_level.txt,sha256=hY2hOVH0V0Ce51WB76zKkIWTUNwMUdHo4XDkR2vYVwg,17
+ScriptCollection-3.3.93.dist-info/RECORD,,
```

