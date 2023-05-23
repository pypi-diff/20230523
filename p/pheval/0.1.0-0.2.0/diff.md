# Comparing `tmp/pheval-0.1.0.tar.gz` & `tmp/pheval-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pheval-0.1.0.tar", max compression
+gzip compressed data, was "pheval-0.2.0.tar", max compression
```

## Comparing `pheval-0.1.0.tar` & `pheval-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,40 @@
--rw-r--r--   0        0        0    11357 2022-12-06 11:15:27.113772 pheval-0.1.0/LICENSE
--rw-r--r--   0        0        0      751 2022-12-06 11:15:27.113772 pheval-0.1.0/README.md
--rw-r--r--   0        0        0      721 2022-12-06 11:15:27.113772 pheval-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       44 2022-12-06 11:15:27.117772 pheval-0.1.0/src/pheval/__init__.py
--rw-r--r--   0        0        0      970 2022-12-06 11:15:27.117772 pheval-0.1.0/src/pheval/cli.py
--rw-r--r--   0        0        0     1851 2022-12-06 11:15:27.117772 pheval-0.1.0/src/pheval/cli_pheval.py
--rw-r--r--   0        0        0      606 2022-12-06 11:15:27.117772 pheval-0.1.0/src/pheval/cli_pheval_utils.py
--rw-r--r--   0        0        0     1241 2022-12-06 11:15:27.117772 pheval-0.1.0/src/pheval/implementations/__init__.py
--rw-r--r--   0        0        0        0 2022-12-06 11:15:27.117772 pheval-0.1.0/src/pheval/runners/__init__.py
--rw-r--r--   0        0        0      942 2022-12-06 11:15:27.117772 pheval-0.1.0/src/pheval/runners/runner.py
--rw-r--r--   0        0        0       77 2022-12-06 11:15:27.117772 pheval-0.1.0/src/pheval/utils.py
--rw-r--r--   0        0        0     1727 1970-01-01 00:00:00.000000 pheval-0.1.0/setup.py
--rw-r--r--   0        0        0     1360 1970-01-01 00:00:00.000000 pheval-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-23 18:26:15.086397 pheval-0.2.0/LICENSE
+-rw-r--r--   0        0        0      751 2023-05-23 18:26:15.086397 pheval-0.2.0/README.md
+-rw-r--r--   0        0        0     1457 2023-05-23 18:26:15.090397 pheval-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-23 18:26:15.090397 pheval-0.2.0/src/pheval/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 18:26:15.090397 pheval-0.2.0/src/pheval/analyse/__init__.py
+-rw-r--r--   0        0        0    24825 2023-05-23 18:26:15.090397 pheval-0.2.0/src/pheval/analyse/analysis.py
+-rw-r--r--   0        0        0    14483 2023-05-23 18:26:15.090397 pheval-0.2.0/src/pheval/analyse/generate_plots.py
+-rw-r--r--   0        0        0     7266 2023-05-23 18:26:15.090397 pheval-0.2.0/src/pheval/analyse/generate_summary_outputs.py
+-rw-r--r--   0        0        0     1933 2023-05-23 18:26:15.090397 pheval-0.2.0/src/pheval/analyse/rank_stats.py
+-rw-r--r--   0        0        0     1412 2023-05-23 18:26:15.090397 pheval-0.2.0/src/pheval/cli.py
+-rw-r--r--   0        0        0     2423 2023-05-23 18:26:15.090397 pheval-0.2.0/src/pheval/cli_pheval.py
+-rw-r--r--   0        0        0     7307 2023-05-23 18:26:15.090397 pheval-0.2.0/src/pheval/cli_pheval_utils.py
+-rw-r--r--   0        0        0     1030 2023-05-23 18:26:15.090397 pheval-0.2.0/src/pheval/config_parser.py
+-rw-r--r--   0        0        0       45 2023-05-23 18:26:15.090397 pheval-0.2.0/src/pheval/constants.py
+-rw-r--r--   0        0        0     1227 2023-05-23 18:26:15.090397 pheval-0.2.0/src/pheval/implementations/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 18:26:15.090397 pheval-0.2.0/src/pheval/post_processing/__init__.py
+-rw-r--r--   0        0        0     7244 2023-05-23 18:26:15.090397 pheval-0.2.0/src/pheval/post_processing/post_processing.py
+-rw-r--r--   0        0        0        0 2023-05-23 18:26:15.090397 pheval-0.2.0/src/pheval/prepare/__init__.py
+-rw-r--r--   0        0        0     6920 2023-05-23 18:26:15.090397 pheval-0.2.0/src/pheval/prepare/create_noisy_phenopackets.py
+-rw-r--r--   0        0        0    12988 2023-05-23 18:26:15.090397 pheval-0.2.0/src/pheval/prepare/create_spiked_vcf.py
+-rw-r--r--   0        0        0     1719 2023-05-23 18:26:15.090397 pheval-0.2.0/src/pheval/prepare/custom_exceptions.py
+-rw-r--r--   0        0        0     2252 2023-05-23 18:26:15.090397 pheval-0.2.0/src/pheval/prepare/update_phenopacket.py
+-rw-r--r--   0        0        0      547 2023-05-23 18:26:15.090397 pheval-0.2.0/src/pheval/resources/alternate_ouputs/CADA_results.txt
+-rw-r--r--   0        0        0     1508 2023-05-23 18:26:15.090397 pheval-0.2.0/src/pheval/resources/alternate_ouputs/DeepPVP_results.txt
+-rw-r--r--   0        0        0     9845 2023-05-23 18:26:15.090397 pheval-0.2.0/src/pheval/resources/alternate_ouputs/OVA_results.txt
+-rw-r--r--   0        0        0    14148 2023-05-23 18:26:15.090397 pheval-0.2.0/src/pheval/resources/alternate_ouputs/Phen2Gene_results.json
+-rw-r--r--   0        0        0      594 2023-05-23 18:26:15.090397 pheval-0.2.0/src/pheval/resources/alternate_ouputs/Phenolyzer_results.txt
+-rw-r--r--   0        0        0   431068 2023-05-23 18:26:15.094397 pheval-0.2.0/src/pheval/resources/alternate_ouputs/lirical_results.tsv
+-rw-r--r--   0        0        0      714 2023-05-23 18:26:15.094397 pheval-0.2.0/src/pheval/resources/alternate_ouputs/svanna_results.tsv
+-rw-r--r--   0        0        0 16274884 2023-05-23 18:26:15.170398 pheval-0.2.0/src/pheval/resources/hgnc_complete_set_2022-10-01.txt
+-rw-r--r--   0        0        0      919 2023-05-23 18:26:15.170398 pheval-0.2.0/src/pheval/run_metadata.py
+-rw-r--r--   0        0        0        0 2023-05-23 18:26:15.170398 pheval-0.2.0/src/pheval/runners/__init__.py
+-rw-r--r--   0        0        0     3774 2023-05-23 18:26:15.170398 pheval-0.2.0/src/pheval/runners/runner.py
+-rw-r--r--   0        0        0        0 2023-05-23 18:26:15.170398 pheval-0.2.0/src/pheval/utils/__init__.py
+-rw-r--r--   0        0        0     3192 2023-05-23 18:26:15.170398 pheval-0.2.0/src/pheval/utils/docs_gen.py
+-rwxr-xr-x   0        0        0      477 2023-05-23 18:26:15.170398 pheval-0.2.0/src/pheval/utils/docs_gen.sh
+-rw-r--r--   0        0        0     3068 2023-05-23 18:26:15.170398 pheval-0.2.0/src/pheval/utils/file_utils.py
+-rw-r--r--   0        0        0    14245 2023-05-23 18:26:15.170398 pheval-0.2.0/src/pheval/utils/phenopacket_utils.py
+-rw-r--r--   0        0        0     6150 2023-05-23 18:26:15.170398 pheval-0.2.0/src/pheval/utils/semsim_utils.py
+-rw-r--r--   0        0        0     1688 1970-01-01 00:00:00.000000 pheval-0.2.0/PKG-INFO
```

### Comparing `pheval-0.1.0/LICENSE` & `pheval-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pheval-0.1.0/README.md` & `pheval-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pheval-0.1.0/src/pheval/cli_pheval.py` & `pheval-0.2.0/src/pheval/cli_pheval.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,68 +1,93 @@
 """
 Monarch Initiative
 """
+from pathlib import Path
 
 import click
 
 from pheval.implementations import get_implementation_resolver
+from pheval.utils.file_utils import write_metadata
 
 
 @click.command()
 @click.option(
-    "--inputdir",
+    "--input-dir",
     "-i",
     metavar="INPUTDIR",
     required=True,
     help="The input directory (relative path: e.g exomiser-13.11)",
+    type=Path,
 )
 @click.option(
-    "--testdatadir",
+    "--testdata-dir",
     "-t",
     metavar="TESTDATA",
     required=True,
     help="The input directory (relative path: e.g ./data)",
+    type=Path,
 )
 @click.option(
     "--runner",
     "-r",
     metavar="RUNNER",
     required=True,
     help="Runner implementation (e.g exomiser-13.11)",
 )
 @click.option(
-    "--tmpdir",
+    "--tmp-dir",
     "-m",
     metavar="TMPDIR",
     required=False,
     help="The path of the temporary directory (optional)",
+    type=Path,
 )
 @click.option(
-    "--outputdir",
+    "--output-dir",
     "-o",
     metavar="OUTPUTDIR",
     required=True,
     help="The path of the output directory",
+    type=Path,
 )
 @click.option(
     "--config",
     "-c",
     metavar="CONFIG",
     required=False,
     help="The path of the configuration file (optional e.g config.yaml)",
+    type=Path,
 )
-def run(inputdir, testdatadir, runner, tmpdir, outputdir, config) -> None:
+@click.option(
+    "--version",
+    "-v",
+    required=False,
+    help="Version of the tool implementation.",
+    type=str,
+)
+def run(
+    input_dir: Path,
+    testdata_dir: Path,
+    runner: str,
+    tmp_dir: Path,
+    output_dir: Path,
+    config: Path,
+    version: str,
+) -> None:
     """PhEval Runner Command Line Interface
-
     Args:
-        inputdir (Click.Path): The input directory (relative path: e.g exomiser-13.11)
-        testdatadir (Click.Path): The input directory (relative path: e.g ./data
+        input_dir (Path): The input directory (relative path: e.g exomiser-13.11)
+        testdata_dir (Path): The input directory (relative path: e.g ./data
         runner (str): Runner implementation (e.g exomiser-13.11)
-        tmpdir (Click.Path): The path of the temporary directory (optional)
-        outputdir (Click.Path): The path of the output directory
-        config (Click.Path): The path of the configuration file (optional e.g config.yaml)
+        tmp_dir (Path): The path of the temporary directory (optional)
+        output_dir (Path): The path of the output directory
+        config (Path): The path of the configuration file (optional e.g., config.yaml)
+        version (str): The version of the tool implementation
     """
     runner_class = get_implementation_resolver().lookup(runner)
-    runner_instance = runner_class(inputdir, testdatadir, tmpdir, outputdir, config)
+    runner_instance = runner_class(input_dir, testdata_dir, tmp_dir, output_dir, config, version)
+    runner_instance.build_output_directory_structure()
     runner_instance.prepare()
     runner_instance.run()
     runner_instance.post_process()
+    run_metadata = runner_instance.construct_meta_data()
+    write_metadata(output_dir, run_metadata)
```

### Comparing `pheval-0.1.0/src/pheval/implementations/__init__.py` & `pheval-0.2.0/src/pheval/implementations/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 @cache
 def get_implementation_resolver() -> ClassResolver[PhEvalRunner]:
     """get_implementation_resolver
 
     Returns:
         ClassResolver[PhEvalRunner]: _description_
     """
-    implementation_resolver: ClassResolver[
-        PhEvalRunner
-    ] = ClassResolver.from_subclasses(
+    implementation_resolver: ClassResolver[PhEvalRunner] = ClassResolver.from_subclasses(
         PhEvalRunner,
         suffix="Implementation",
     )
 
     # implementation_resolver.synonyms.update(
     #     {
     #         "exomiser": DefaultPhEvalRunner,
```

### Comparing `pheval-0.1.0/PKG-INFO` & `pheval-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 Metadata-Version: 2.1
 Name: pheval
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
-Author: Nico Matentzoglu
-Author-email: nicolas.matentzoglu@gmail.com
-Requires-Python: >=3.9
+Author: Yasemin Bridges
+Author-email: y.bridges@qmul.ac.uk
+Requires-Python: >=3.9,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: class-resolver (>=0.3.10,<0.4.0)
 Requires-Dist: click (>=8.1.3)
 Requires-Dist: deprecation (>=2.1.0)
+Requires-Dist: google (>=3.0.0,<4.0.0)
 Requires-Dist: jaydebeapi (>=1.2.3)
+Requires-Dist: matplotlib (>=3.7.0,<4.0.0)
+Requires-Dist: oaklib (>=0.1.55,<0.2.0)
 Requires-Dist: pandas (>=1.5.1)
+Requires-Dist: phenopackets (>=2.0.2,<3.0.0)
+Requires-Dist: plotly (>=5.13.0,<6.0.0)
+Requires-Dist: pyaml (>=21.10.1,<22.0.0)
+Requires-Dist: pyserde (>=0.9.8,<0.10.0)
+Requires-Dist: seaborn (>=0.12.2,<0.13.0)
 Requires-Dist: tqdm (>=4.64.1)
 Description-Content-Type: text/markdown
 
 # PhEval - Phenotypic Inference Evaluation Framework
 
 There is currently no empirical framework to evaluate the performance of phenotype matching and prioritization tools, much needed to guide tuning for cross species inference. Many algorithms are evaluated using simulations, which may fail to capture real-world scenarios. This gap presents a number of problems: it is difficult to optimize algorithms if we do not know which choices lead to better results; performance may be sensitive to factors that are subject to change, such as ontology structure or annotation completeness. We will develop a modular Phenotypic Inference Evaluation Framework, PhEval and use it to optimize our own algorithms, as well as deliver it as a community resource.
```

