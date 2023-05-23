# Comparing `tmp/aqme-1.4.7.tar.gz` & `tmp/aqme-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aqme-1.4.7.tar", last modified: Mon Mar 13 12:59:14 2023, max compression
+gzip compressed data, was "aqme-1.5.0.tar", last modified: Tue May 23 11:31:27 2023, max compression
```

## Comparing `aqme-1.4.7.tar` & `aqme-1.5.0.tar`

### file list

```diff
@@ -1,38 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-03-13 12:59:14.528638 aqme-1.4.7/
--rw-rw-rw-   0        0        0     1086 2022-09-14 16:11:15.000000 aqme-1.4.7/LICENSE
--rw-rw-rw-   0        0        0     1056 2023-03-13 12:59:14.528638 aqme-1.4.7/PKG-INFO
--rw-rw-rw-   0        0        0     3419 2023-03-06 16:00:20.000000 aqme-1.4.7/README.md
-drwxrwxrwx   0        0        0        0 2023-03-13 12:59:14.510461 aqme-1.4.7/aqme/
--rw-rw-rw-   0        0        0        0 2022-09-14 16:11:15.000000 aqme-1.4.7/aqme/__init__.py
--rw-rw-rw-   0        0        0      628 2022-09-14 16:11:15.000000 aqme-1.4.7/aqme/__main__.py
--rw-rw-rw-   0        0        0     9459 2023-03-12 12:43:38.000000 aqme-1.4.7/aqme/aqme.py
--rw-rw-rw-   0        0        0     3482 2023-03-12 12:38:19.000000 aqme-1.4.7/aqme/argument_parser.py
--rw-rw-rw-   0        0        0    24153 2023-03-13 11:07:05.000000 aqme-1.4.7/aqme/cmin.py
--rw-rw-rw-   0        0        0     1503 2022-12-10 12:38:42.000000 aqme-1.4.7/aqme/cmin_utils.py
-drwxrwxrwx   0        0        0        0 2023-03-13 12:59:14.521545 aqme-1.4.7/aqme/csearch/
--rw-rw-rw-   0        0        0       37 2022-12-06 18:50:02.000000 aqme-1.4.7/aqme/csearch/__init__.py
--rw-rw-rw-   0        0        0    49275 2023-03-13 11:06:52.000000 aqme-1.4.7/aqme/csearch/base.py
--rw-rw-rw-   0        0        0    23535 2023-03-13 11:14:52.000000 aqme-1.4.7/aqme/csearch/crest.py
--rw-rw-rw-   0        0        0     8237 2023-01-31 07:17:56.000000 aqme-1.4.7/aqme/csearch/fullmonte.py
--rw-rw-rw-   0        0        0    15621 2023-02-05 12:34:12.000000 aqme-1.4.7/aqme/csearch/templates.py
--rw-rw-rw-   0        0        0    16237 2023-03-05 16:43:21.000000 aqme-1.4.7/aqme/csearch/utils.py
--rw-rw-rw-   0        0        0    20614 2022-12-09 18:04:27.000000 aqme-1.4.7/aqme/filter.py
--rw-rw-rw-   0        0        0    41206 2023-03-13 11:57:22.000000 aqme-1.4.7/aqme/qcorr.py
--rw-rw-rw-   0        0        0    24886 2023-03-12 08:17:09.000000 aqme-1.4.7/aqme/qcorr_utils.py
--rw-rw-rw-   0        0        0    20306 2023-03-04 14:49:26.000000 aqme-1.4.7/aqme/qdescp.py
--rw-rw-rw-   0        0        0    16003 2023-02-06 12:40:14.000000 aqme-1.4.7/aqme/qdescp_utils.py
--rw-rw-rw-   0        0        0    19518 2023-03-13 07:06:58.000000 aqme-1.4.7/aqme/qprep.py
-drwxrwxrwx   0        0        0        0 2023-03-13 12:59:14.526550 aqme-1.4.7/aqme/templates/
--rw-rw-rw-   0        0        0      354 2022-09-14 16:11:15.000000 aqme-1.4.7/aqme/templates/template-2.sdf
--rw-rw-rw-   0        0        0      448 2022-09-14 16:11:15.000000 aqme-1.4.7/aqme/templates/template-3.sdf
--rw-rw-rw-   0        0        0      640 2022-09-14 16:11:15.000000 aqme-1.4.7/aqme/templates/template-4-and-5.sdf
--rw-rw-rw-   0        0        0    26662 2023-03-13 12:57:33.000000 aqme-1.4.7/aqme/utils.py
--rw-rw-rw-   0        0        0     4473 2022-12-09 17:37:46.000000 aqme-1.4.7/aqme/vismol.py
-drwxrwxrwx   0        0        0        0 2023-03-13 12:59:14.518660 aqme-1.4.7/aqme.egg-info/
--rw-rw-rw-   0        0        0     1056 2023-03-13 12:59:13.000000 aqme-1.4.7/aqme.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      644 2023-03-13 12:59:14.000000 aqme-1.4.7/aqme.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-13 12:59:13.000000 aqme-1.4.7/aqme.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       92 2023-03-13 12:59:14.000000 aqme-1.4.7/aqme.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-03-13 12:59:14.000000 aqme-1.4.7/aqme.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      118 2023-03-13 12:59:14.528638 aqme-1.4.7/setup.cfg
--rw-rw-rw-   0        0        0     1863 2023-03-13 12:57:39.000000 aqme-1.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 11:31:27.245301 aqme-1.5.0/
+-rw-rw-rw-   0        0        0     1086 2022-09-14 16:11:15.000000 aqme-1.5.0/LICENSE
+-rw-rw-rw-   0        0        0     1035 2023-05-23 11:31:27.245301 aqme-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3419 2023-03-06 16:00:20.000000 aqme-1.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 11:31:27.211067 aqme-1.5.0/aqme/
+-rw-rw-rw-   0        0        0        0 2022-09-14 16:11:15.000000 aqme-1.5.0/aqme/__init__.py
+-rw-rw-rw-   0        0        0      628 2022-09-14 16:11:15.000000 aqme-1.5.0/aqme/__main__.py
+-rw-rw-rw-   0        0        0     9791 2023-05-01 11:11:50.000000 aqme-1.5.0/aqme/aqme.py
+-rw-rw-rw-   0        0        0     3586 2023-05-01 11:11:41.000000 aqme-1.5.0/aqme/argument_parser.py
+-rw-rw-rw-   0        0        0    24365 2023-04-30 17:05:33.000000 aqme-1.5.0/aqme/cmin.py
+-rw-rw-rw-   0        0        0     1503 2022-12-10 12:38:42.000000 aqme-1.5.0/aqme/cmin_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-23 11:31:27.232044 aqme-1.5.0/aqme/csearch/
+-rw-rw-rw-   0        0        0       37 2022-12-06 18:50:02.000000 aqme-1.5.0/aqme/csearch/__init__.py
+-rw-rw-rw-   0        0        0    49308 2023-03-15 18:15:42.000000 aqme-1.5.0/aqme/csearch/base.py
+-rw-rw-rw-   0        0        0    24815 2023-03-16 10:06:51.000000 aqme-1.5.0/aqme/csearch/crest.py
+-rw-rw-rw-   0        0        0     8237 2023-01-31 07:17:56.000000 aqme-1.5.0/aqme/csearch/fullmonte.py
+-rw-rw-rw-   0        0        0    15621 2023-02-05 12:34:12.000000 aqme-1.5.0/aqme/csearch/templates.py
+-rw-rw-rw-   0        0        0    16736 2023-04-30 17:05:33.000000 aqme-1.5.0/aqme/csearch/utils.py
+-rw-rw-rw-   0        0        0    20614 2022-12-09 18:04:27.000000 aqme-1.5.0/aqme/filter.py
+-rw-rw-rw-   0        0        0    41399 2023-04-30 17:08:10.000000 aqme-1.5.0/aqme/qcorr.py
+-rw-rw-rw-   0        0        0    24886 2023-03-12 08:17:09.000000 aqme-1.5.0/aqme/qcorr_utils.py
+-rw-rw-rw-   0        0        0    26177 2023-05-01 14:27:23.000000 aqme-1.5.0/aqme/qdescp.py
+-rw-rw-rw-   0        0        0    15665 2023-05-01 14:25:40.000000 aqme-1.5.0/aqme/qdescp_utils.py
+-rw-rw-rw-   0        0        0    20608 2023-04-30 17:08:42.000000 aqme-1.5.0/aqme/qprep.py
+drwxrwxrwx   0        0        0        0 2023-05-23 11:31:27.234456 aqme-1.5.0/aqme/templates/
+-rw-rw-rw-   0        0        0      354 2022-09-14 16:11:15.000000 aqme-1.5.0/aqme/templates/template-2.sdf
+-rw-rw-rw-   0        0        0      448 2022-09-14 16:11:15.000000 aqme-1.5.0/aqme/templates/template-3.sdf
+-rw-rw-rw-   0        0        0      640 2022-09-14 16:11:15.000000 aqme-1.5.0/aqme/templates/template-4-and-5.sdf
+-rw-rw-rw-   0        0        0    27517 2023-05-01 11:04:52.000000 aqme-1.5.0/aqme/utils.py
+-rw-rw-rw-   0        0        0     4486 2023-04-30 17:05:33.000000 aqme-1.5.0/aqme/vismol.py
+drwxrwxrwx   0        0        0        0 2023-05-23 11:31:27.215276 aqme-1.5.0/aqme.egg-info/
+-rw-rw-rw-   0        0        0     1035 2023-05-23 11:31:26.000000 aqme-1.5.0/aqme.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      746 2023-05-23 11:31:27.000000 aqme-1.5.0/aqme.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 11:31:26.000000 aqme-1.5.0/aqme.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       99 2023-05-23 11:31:26.000000 aqme-1.5.0/aqme.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-23 11:31:26.000000 aqme-1.5.0/aqme.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      118 2023-05-23 11:31:27.245301 aqme-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1882 2023-05-23 11:26:58.000000 aqme-1.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 11:31:27.245301 aqme-1.5.0/tests/
+-rw-rw-rw-   0        0        0     2948 2023-04-30 17:05:33.000000 aqme-1.5.0/tests/test_cmin.py
+-rw-rw-rw-   0        0        0    28035 2023-03-06 09:24:52.000000 aqme-1.5.0/tests/test_csearch.py
+-rw-rw-rw-   0        0        0    34526 2023-03-18 10:55:19.000000 aqme-1.5.0/tests/test_qcorr.py
+-rw-rw-rw-   0        0        0     7360 2023-03-06 09:24:03.000000 aqme-1.5.0/tests/test_qdescp.py
+-rw-rw-rw-   0        0        0    19952 2023-03-13 07:06:58.000000 aqme-1.5.0/tests/test_qprep.py
```

### Comparing `aqme-1.4.7/LICENSE` & `aqme-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aqme-1.4.7/PKG-INFO` & `aqme-1.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: aqme
-Version: 1.4.7
+Version: 1.5.0
 Summary: Automated Quantum Mechanical Environments
 Home-page: https://github.com/jvalegre/aqme
-Download-URL: https://github.com/jvalegre/aqme/archive/refs/tags/1.4.7.tar.gz
+Download-URL: https://github.com/jvalegre/aqme/archive/refs/tags/1.5.0.tar.gz
 Author: Shree Sowndarya S. V., Juan V. Alegre Requena
 Author-email: svss@colostate.edu, jvalegre@unizar.es
 License: MIT
 Keywords: workflows,computational chemistry,conformational sampling,cheminformatics,quantum mechanics,DFT,automated
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Documentation in Read The Docs: https://aqme.readthedocs.io
-
```

### Comparing `aqme-1.4.7/README.md` & `aqme-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `aqme-1.4.7/aqme/__main__.py` & `aqme-1.5.0/aqme/__main__.py`

 * *Files identical despite different names*

### Comparing `aqme-1.4.7/aqme/aqme.py` & `aqme-1.5.0/aqme/aqme.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,14 +166,17 @@
             prefix=args.prefix,
             chk=args.chk,
             mem=args.mem,
             nprocs=args.nprocs,
             gen_atoms=args.gen_atoms,
             bs_gen=args.bs_gen,
             bs_nogen=args.bs_nogen,
+            lowest_only = args.lowest_only,
+            lowest_n = args.lowest_n,
+            e_threshold_qprep= args.e_threshold_qprep,
         )
 
     # QCORR
     if args.qcorr:
         qcorr(
             files=args.files,
             command_line=args.command_line,
@@ -196,14 +199,15 @@
             nprocs=args.nprocs,
             qm_input=args.qm_input,
             qm_end=args.qm_end,
             chk=args.chk,
             gen_atoms=args.gen_atoms,
             bs_gen=args.bs_gen,
             bs_nogen=args.bs_nogen,
+            nodup_check=args.nodup_check,
         )
 
     # QDESCP
     if args.qdescp:
         qdescp(
             w_dir_main=args.w_dir_main,
             destination=args.destination,
@@ -215,12 +219,16 @@
             qdescp_acc=args.qdescp_acc,
             qdescp_solvent=args.qdescp_solvent,
             boltz=args.boltz,
             nmr_atoms=args.nmr_atoms,
             nmr_slope=args.nmr_slope,
             nmr_intercept=args.nmr_intercept,
             nmr_experim=args.nmr_experim,
+            qdescp_atom=args.qdescp_atom,
+            dbstep_r=args.dbstep_r,
+            robert=args.robert,
+            csv_name=args.csv_name
         )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `aqme-1.4.7/aqme/argument_parser.py` & `aqme-1.5.0/aqme/argument_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,16 +65,16 @@
     "qm_input": "",
     "ts_input": "opt=(calcfc,noeigen,ts,maxstep=5)",
     "qm_end": "",
     "gen_atoms": [],
     "bs_nogen": "",
     "bs_gen": "",
     "lowest_only": False,
-    "lowest_n": False,
-    "energy_threshold_for_gaussian": 100.0,
+    "lowest_n": None,
+    "e_threshold_qprep": None,
     "chk": False,
     "w_dir_main": os.getcwd(),
     "files": [],
     "atom_types": [],
     "cartesians": [],
     "dup": True,
     "dup_threshold": 0.0001,
@@ -100,14 +100,19 @@
     "qdescp_acc": 0.2,
     "qdescp_solvent": None,
     "boltz": True,
     "nmr_atoms": [6, 1],  # [C,H]
     "nmr_slope": [-1.0537, -1.0784],  # [C,H]
     "nmr_intercept": [181.7815,31.8723],  # [C,H]
     "nmr_experim": None,
+    "nodup_check": False,
+    "qdescp_atom": None,
+    "dbstep_r": 3.5,
+    "robert": True,
+    "csv_name": None
 }
 
 
 # part for using the options in a script or jupyter notebook
 class options_add:
     pass
```

### Comparing `aqme-1.4.7/aqme/cmin.py` & `aqme-1.5.0/aqme/cmin.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,18 +97,17 @@
 from rdkit.Chem.PropertyMol import PropertyMol
 from progress.bar import IncrementalBar
 from rdkit.Geometry import Point3D
 import pandas as pd
 import time
 from aqme.utils import (
     load_variables,
+    substituted_mol,
     mol_from_sdf_or_mol_or_mol2,
-    add_prefix_suffix,
-    check_files,
-    check_xtb
+    add_prefix_suffix
 )
 from aqme.filter import ewin_filter, pre_E_filter, RMSD_and_E_filter
 from aqme.cmin_utils import creation_of_dup_csv_cmin
 from aqme.csearch.crest import xtb_opt_main
 from aqme.csearch.utils import prepare_com_files
 
 hartree_to_kcal = 627.509
@@ -137,77 +136,70 @@
             if self.args.program.lower() not in ["xtb", "ani"]:
                 cmin_program = False
         if not cmin_program:
             self.args.log.write('\nx  Program not supported for CMIN refinement! Specify: program="xtb" (or "ani")')
             self.args.log.finalize()
             sys.exit()
 
-        try:
-            os.chdir(self.args.w_dir_main)
-        except FileNotFoundError:
-            self.args.w_dir_main = Path(f"{os.getcwd()}/{self.args.w_dir_main}")
-            os.chdir(self.args.w_dir_main)
-
         # retrieves the different files to run in CMIN
-        _ = check_files(self,'cmin')
+        if len(self.args.files) == 0:
+            self.args.log.write('\nx  No files were found! Make sure you use quotation marks if you are using * (i.e. --files "*.sdf")')
+            self.args.log.finalize()
+            sys.exit()
 
         # create the dataframe to store the data
         self.final_dup_data = creation_of_dup_csv_cmin(self.args.program.lower())
 
         bar = IncrementalBar(
             "\no  Number of finished jobs from CMIN", max=len(self.args.files)
         )
 
-        file_format = os.path.basename(Path(self.args.files[0])).split('.')[1]
-        file_dir = os.path.dirname(Path(self.args.files[0]))
-        if file_format.lower() in ['xyz', 'gjf', 'com']:
+        file_format = '.'+os.path.basename(Path(self.args.files[0])).split('.')[1]
+
+        if file_format.lower() in ['.xyz', '.gjf', '.com']:
             for file in self.args.files:
                 prepare_com_files(self.args, file)
-            if file_format.lower() in ['gjf', 'com']:
-                files_temp_extra = glob.glob(f'{file_dir}/*.xyz')
-            files_cmin = glob.glob(f'{file_dir}/*.sdf')
-        elif file_format.lower() == 'pdb':
+            if file_format.lower() in ['.gjf', '.com']:
+                files_temp_extra = glob.glob('*.xyz')
+            files_cmin = glob.glob('*.sdf')
+        elif file_format.lower() == '.pdb':
             for file in self.args.files:
                 command_pdb = [
                     "obabel",
                     "-ipdb",
                     f"{file}",
                     "-osdf",
                     f"-O{file.split('.pdb')[0]}.sdf",
                 ]
                 subprocess.run(
                     command_pdb,
                     stdout=subprocess.DEVNULL,
                     stderr=subprocess.DEVNULL,
                 )
-            files_cmin = glob.glob(f'{file_dir}/*.sdf')
-        elif file_format.lower() == 'sdf':
+            files_cmin = glob.glob('*.sdf')
+        elif file_format.lower() == '.sdf':
             files_cmin = self.args.files
         else:
             self.args.log.write(f"\nx  The input format {file_format} is not supported for CMIN refinement! Formats allowed: SDF, XYZ, COM, GJF and PDB")
             self.args.log.finalize()
             sys.exit()
 
         for file in files_cmin:
             # load jobs for cmin minimization
             self.mols, self.name = self.load_jobs(file)
             self.name = add_prefix_suffix(self.name, self.args)
 
             self.args.log.write(f"\n\n   ----- {self.name} -----")
 
             if self.args.destination is None:
-                self.cmin_folder = Path(self.args.w_dir_main).joinpath(
-                    f"CMIN"
-                )
+                self.cmin_folder = self.args.initial_dir.joinpath("CMIN")
+            elif self.args.initial_dir.joinpath(self.args.destination).exists():
+                self.cmin_folder = Path(self.args.initial_dir.joinpath(self.args.destination))
             else:
-                if self.args.initial_dir.as_posix() in f"{self.args.destination}":
-                    self.cmin_folder = Path(self.args.destination)
-                else:
-                    self.cmin_folder = Path(self.args.initial_dir).joinpath(
-                    self.args.destination)
+                self.cmin_folder = Path(self.args.destination)
 
             self.cmin_folder.mkdir(exist_ok=True, parents=True)
 
             self.cmin_all_file = self.cmin_folder.joinpath(
                 f"{self.name}_{self.args.program.lower()}_all_confs{self.args.output}"
             )
             self.sdwriterall = Chem.SDWriter(str(self.cmin_all_file))
@@ -230,32 +222,33 @@
         self.final_dup_data.to_csv(cmin_csv_file, index=False)
 
         elapsed_time = round(time.time() - start_time_overall, 2)
         self.args.log.write(f"\nTime CMIN: {elapsed_time} seconds\n")
         self.args.log.finalize()
 
         # delete extra temporary files created when using XYZ, GJF, COM and PDB files
-        if file_format.lower() in ['xyz', 'gjf', 'com', 'pdb']:
-            if file_format.lower() in ['gjf', 'com']:
+        if file_format.lower() in ['.xyz', '.gjf', '.com', '.pdb']:
+            if file_format.lower() in ['.gjf', '.com']:
                 files_cmin = files_cmin + files_temp_extra
             for temp_file in files_cmin:
                 os.remove(temp_file)
 
         # this is added to avoid path problems in jupyter notebooks
         os.chdir(self.args.initial_dir)
 
     def load_jobs(self, file):
 
         # read SDF files
         try:
-            inmols = mol_from_sdf_or_mol_or_mol2(file, 'cmin')
+            inmols = mol_from_sdf_or_mol_or_mol2(file, 'cmin', self.args)
         except OSError:
             file_path = Path(self.args.initial_dir).joinpath(file)
             file_path = file_path.as_posix()
-            inmols = mol_from_sdf_or_mol_or_mol2(file_path, 'cmin')
+            inmols = mol_from_sdf_or_mol_or_mol2(file_path, 'cmin', self.args)
+
         name_mol = os.path.basename(file).split(".sdf")[0]
 
         return inmols, name_mol
 
     def compute_cmin(self, file):
 
         dup_data = creation_of_dup_csv_cmin(self.args.program.lower())
@@ -272,20 +265,18 @@
             elif self.args.mult is not None:
                 self.args.log.write("\nx  Multiplicity is automatically calculated for ANI methods, do not use the mult option!")
                 self.args.log.finalize()
                 sys.exit()
             charge,mult,final_mult,dup_data = self.charge_mult_cmin(dup_data, dup_data_idx)
 
         elif self.args.program.lower() == "xtb":
-            # checks if xTB is installed
-            _ = self.get_cmin_model()
             # sets charge and mult
-            file_format = os.path.basename(Path(file)).split('.')[1]
+            file_format = os.path.splitext(file)[1]
             charge_input, mult_input, final_mult = None, None, None
-            if file_format.lower() == 'sdf':
+            if file_format.lower() == '.sdf':
                 if self.args.charge is None or self.args.mult is None:
                     # read charge and mult from SDF if possible (i.e. charge/mult of SDFs created with CSEARCH)
                     with open(file, "r") as F:
                         lines = F.readlines()
                     charge_found, mult_found = False, False
                     for i, line in enumerate(lines):
                         if line.find(">  <Real charge>") > -1:
@@ -319,15 +310,17 @@
                     mol, energy, cmin_valid = self.ani_optimize(mol,charge,mult)
                 # xTB calculations use the xTB program directly
                 elif self.args.program.lower() == "xtb":
                     # for contrained optimizations
                     complex_ts = False
                     if len(self.args.constraints_atoms) >= 1 or len(self.args.constraints_dist) >= 1 or len(self.args.constraints_angle) >= 1 or len(self.args.constraints_dihedral) >= 1:
                         complex_ts = True
-                    name_init = str(open(file, "r").readlines()[0].strip())
+                    # name_init = str(open(file, "r").readlines()[0].strip())
+                    name_init = mol.GetProp('_Name')
+                    # print(name_init)
                     mol, energy, cmin_valid = xtb_opt_main(
                         f'{self.name}_conf_{i}',
                         dup_data,
                         dup_data_idx,
                         self,
                         charge,
                         mult,
@@ -428,15 +421,15 @@
                 os.remove(file)
 
         return dup_data
 
     # xTB AND ANI MAIN OPTIMIZATION PROCESS
     def ani_optimize(self, mol, charge, mult):
 
-        # Attempts ANI imports and exits if the programs are not installed
+        # Attempts ANI/xTB imports and exits if the programs are not installed
         try:
             import torch
             import warnings
             warnings.filterwarnings('ignore')
 
         except ModuleNotFoundError:
             self.args.log.write("x  Torch-related modules are not installed! You can install these modules with 'pip install torch torchvision torchani'")
@@ -524,15 +517,23 @@
                 self.args.log.write("x  Torchani is not installed! You can install the program with 'pip install torchani'")
                 self.args.log.finalize()
                 sys.exit()
 
             model = getattr(torchani.models,self.args.ani_method)()
 
         elif self.args.program.lower() == "xtb":
-            _ = check_xtb(self)
+            try:
+                subprocess.run(
+                    ["xtb", "-h"], stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL
+                )
+            except FileNotFoundError:
+                self.args.log.write("x  xTB is not installed (CREST cannot be used)! You can install the program with 'conda install -c conda-forge xtb'")
+                self.args.log.finalize()
+                sys.exit()
+    
             model = None
 
         return model
 
     # write SDF files for xTB and ANI
     def write_confs(self, conformers, selectedcids, log):
         if len(conformers) > 0:
```

### Comparing `aqme-1.4.7/aqme/cmin_utils.py` & `aqme-1.5.0/aqme/cmin_utils.py`

 * *Files identical despite different names*

### Comparing `aqme-1.4.7/aqme/csearch/base.py` & `aqme-1.5.0/aqme/csearch/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -417,14 +417,15 @@
                 constraints_angle,
                 constraints_dihedral,
                 complex_ts
             ) = smi_to_mol(
                 smi,
                 self.args.program.lower(),
                 self.args.log,
+                self.args.seed,
                 constraints_atoms,
                 constraints_dist,
                 constraints_angle,
                 constraints_dihedral,
             )
             if mol is None:
                 self.args.log.write(f"\nx  Failed to convert the provided SMILES ({smi}) to an RDkit Mol object! Please check the starting smiles.")
```

### Comparing `aqme-1.4.7/aqme/csearch/crest.py` & `aqme-1.5.0/aqme/csearch/crest.py`

 * *Files 3% similar despite different names*

```diff
@@ -164,15 +164,21 @@
         except FileNotFoundError:
             os.rename(str(dat_dir) + "/xtblast.xyz", xyzoutxtb1)
 
         # remove files that might interfere in subsequent calculations (i.e. wrong electron readings)
         for file in glob.glob('*') + glob.glob('*.*') + glob.glob('.*'):
             if os.path.exists(file):
                 if file.find('_xtb2') == -1 and file.find('_xtb1') == -1 and file.find('.out') == -1:
-                    os.remove(file)
+                    try:
+                        os.remove(file)
+                    except IsADirectoryError:
+                        try:
+                            shutil.rmtree(file)
+                        except OSError: # this avoids problems when running AQME in HPCs
+                            pass
 
         if constrained_opt:
             xyzoutxtb2 = str(dat_dir) + "/" + name_no_path + "_xtb2.xyz"
             # xTB optimization with the user-defined constraints
             _ = create_xcontrol(
                 self.args,
                 list(constraints_atoms),
@@ -498,41 +504,55 @@
         xcontrol_file.close()
 
     return constrained_sampling
 
 
 def nci_ts_mol(
     smi,
+    log,
+    seed,
     constraints_atoms,
     constraints_dist,
     constraints_angle,
     constraints_dihedral,
 ):
+    using_const = None
     if constraints_atoms is not None:
+        using_const = constraints_atoms
         constraints_atoms = [[float(y) for y in x] for x in constraints_atoms]
+        constraints_atoms = np.array(constraints_atoms)
     if constraints_dist is not None:
+        using_const = constraints_dist
         constraints_dist = [[float(y) for y in x] for x in constraints_dist]
         constraints_dist = np.array(constraints_dist)
     if constraints_angle is not None:
+        using_const = constraints_angle
         constraints_angle = [[float(y) for y in x] for x in constraints_angle]
         constraints_angle = np.array(constraints_angle)
     if constraints_dihedral is not None:
+        using_const = constraints_dihedral
         constraints_dihedral = [[float(y) for y in x] for x in constraints_dihedral]
         constraints_dihedral = np.array(constraints_dihedral)
 
+    if using_const is not None:
+        for smi_part in smi:
+            if ':' not in smi_part or '[' not in smi_part:
+                log.write(f"\nx  Constraints were specified {using_const} but atoms might not be mapped in the SMILES input!")
+                break
+
     molsH = []
     mols = []
     for m in smi:
         mols.append(Chem.MolFromSmiles(m))
         molsH.append(Chem.AddHs(Chem.MolFromSmiles(m)))
 
     for m in molsH:
-        Chem.EmbedMultipleConfs(m, numConfs=1)
+        Chem.EmbedMultipleConfs(m, numConfs=1, randomSeed=seed)
     for m in mols:
-        Chem.EmbedMultipleConfs(m, numConfs=1)
+        Chem.EmbedMultipleConfs(m, numConfs=1, randomSeed=seed)
 
     coord = [0.0, 0.0, 5.0]
     molH = molsH[0]
     for _, fragment in enumerate(molsH[1:]):
         offset_3d = Geometry.Point3D(coord[0], coord[1], coord[2])
         molH = Chem.CombineMols(molH, fragment, offset_3d)
         coord[1] += 5
@@ -543,15 +563,23 @@
     for _, fragment in enumerate(mols[1:]):
         offset_3d = Geometry.Point3D(coord[0], coord[1], coord[2])
         mol = Chem.CombineMols(mol, fragment, offset_3d)
         coord[1] += 5
         Chem.SanitizeMol(mol)
     mol = Chem.AddHs(mol)
 
-    mol = Chem.ConstrainedEmbed(mol, molH)
+    try:
+        mol = Chem.ConstrainedEmbed(mol, molH, randomseed=seed)
+    except ValueError: # removingH in the core (molH) avoids problems related to RDKit embedding
+        molH = Chem.RemoveHs(molH)
+        try:
+            mol = Chem.ConstrainedEmbed(mol, molH, randomseed=seed)
+        except ValueError:
+            log.write(f"\nx  Constrained optimization failed due to an embedding problem with RDKit that could not be fixed!")
+            pass
 
     atom_map = []
     for atom in mol.GetAtoms():
         atom_map.append(atom.GetAtomMapNum())
 
     max_map = max(atom_map)
     for a in mol.GetAtoms():
```

### Comparing `aqme-1.4.7/aqme/csearch/fullmonte.py` & `aqme-1.5.0/aqme/csearch/fullmonte.py`

 * *Files identical despite different names*

### Comparing `aqme-1.4.7/aqme/csearch/templates.py` & `aqme-1.5.0/aqme/csearch/templates.py`

 * *Files identical despite different names*

### Comparing `aqme-1.4.7/aqme/csearch/utils.py` & `aqme-1.5.0/aqme/csearch/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -293,23 +293,37 @@
 
 def prepare_com_files(args, csearch_file):
     job_inputs = []
 
     filename = os.path.basename(csearch_file)
     if filename.split('.')[1] in ["gjf", "com"]:
         xyz_file, _, _ = com_2_xyz(csearch_file)
-        _, charge, mult = get_info_input(csearch_file)
+        if args.charge is None:
+            _, charge, _ = get_info_input(csearch_file)
+        else:
+            charge = args.charge
+        if args.mult is None:
+            _, _, mult = get_info_input(csearch_file)
+        else:
+            mult = args.mult
     else:
         xyz_file = csearch_file
-        charge, mult = read_xyz_charge_mult(xyz_file)
+        if args.charge is None:
+            charge, _ = read_xyz_charge_mult(csearch_file)
+        else:
+            charge = args.charge
+        if args.mult is None:
+            _, mult = read_xyz_charge_mult(csearch_file)
+        else:
+            mult = args.mult
     _ = xyz_2_sdf(xyz_file)
 
     sdffile = f'{os.path.dirname(csearch_file)}/{filename.split(".")[0]}.sdf'
 
-    suppl, _, _, _ = mol_from_sdf_or_mol_or_mol2(sdffile, "csearch")
+    suppl, _, _, _ = mol_from_sdf_or_mol_or_mol2(sdffile, "csearch", args)
 
     name = filename.split('.')[0]
     name = add_prefix_suffix(name, args)
 
     obj = (
         suppl[0],
         name,
@@ -343,15 +357,17 @@
     os.remove(sdffile)
     return job_inputs
 
 
 def prepare_sdf_files(args, csearch_file):
     filename = os.path.basename(csearch_file)
     sdffile = f'{os.path.dirname(csearch_file)}/{filename}'
-    suppl, charges, mults, IDs = mol_from_sdf_or_mol_or_mol2(sdffile, "csearch")
+
+    suppl, charges, mults, IDs = mol_from_sdf_or_mol_or_mol2(sdffile, "csearch", args)
+
     if sdffile.split('.')[0] in ['mol','mol2']:
         os.remove(f'{sdffile.split(".")[0]}.sdf')
 
     job_inputs = []
     for mol, charge, mult, name in zip(suppl, charges, mults, IDs):
         name = add_prefix_suffix(name, args)
         obj = (
@@ -473,14 +489,15 @@
     return uniqmatches
 
 
 def smi_to_mol(
     smi,
     program,
     log,
+    seed,
     constraints_atoms,
     constraints_dist,
     constraints_angle,
     constraints_dihedral,
 ):
 
     complex_ts = False
@@ -500,14 +517,16 @@
             mol,
             constraints_atoms,
             constraints_dist,
             constraints_angle,
             constraints_dihedral,
         ) = nci_ts_mol(
             smi,
+            log,
+            seed,
             constraints_atoms,
             constraints_dist,
             constraints_angle,
             constraints_dihedral,
         )
         complex_ts = True
```

### Comparing `aqme-1.4.7/aqme/filter.py` & `aqme-1.5.0/aqme/filter.py`

 * *Files identical despite different names*

### Comparing `aqme-1.4.7/aqme/qcorr.py` & `aqme-1.5.0/aqme/qcorr.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,14 +46,16 @@
       Folder containing the initial input files to check for isomerization
    vdwfrac : float, default=0.50
       Fraction of the summed VDW radii that constitutes a bond between two atoms 
       in the isomerization filter
    covfrac : float, default=1.10
       Fraction of the summed covalent radii that constitutes a bond between two 
       atoms in the isomerization filter
+   nodup_check : bool, default=False
+      If True, the duplicate filter is disabled
       
 .. note::
 
    New input files are generated through the QPREP module and, therefore, all 
    QPREP arguments can be used when calling QCORR and will overwrite default 
    options. For example, if the user specifies qm_input='wb97xd/def2svp', 
    all the new input files generated to fix issues will contain this keywords 
@@ -423,29 +425,30 @@
                 duplicate_data["RO_constant"].append(ro_json)
 
         atom_types, cartesians = cclib_atoms_coords(cclib_data)
         dup_off = None
         if errortype == "none":
             E_dup, H_dup, G_dup, ro_dup, errortype = get_cclib_params(cclib_data, errortype)
 
-            # detects if this calculation is a duplicate
-            for i, _ in enumerate(duplicate_data["Energies"]):
-                E_diff = abs(E_dup - duplicate_data["Energies"][i])
-                H_diff = abs(H_dup - duplicate_data["Enthalpies"][i])
-                G_diff = abs(G_dup - duplicate_data["Gibbs"][i])
-                if (ro_dup is not None) and (
-                    duplicate_data["RO_constant"][i] is not None
-                ):
-                    ro_diff = np.linalg.norm(
-                        np.array(ro_dup) - np.array(duplicate_data["RO_constant"][i])
-                    )
-                if max([E_diff, H_diff, G_diff]) < abs(float(self.args.dup_threshold)):
-                    if (ro_dup is not None) and (ro_diff < self.args.ro_threshold):
-                        errortype = "duplicate_calc"
-                        dup_off = duplicate_data["File"][i]
+            if self.args.nodup_check==False:
+                # detects if this calculation is a duplicate
+                for i, _ in enumerate(duplicate_data["Energies"]):
+                    E_diff = abs(E_dup - duplicate_data["Energies"][i])
+                    H_diff = abs(H_dup - duplicate_data["Enthalpies"][i])
+                    G_diff = abs(G_dup - duplicate_data["Gibbs"][i])
+                    if (ro_dup is not None) and (
+                        duplicate_data["RO_constant"][i] is not None
+                    ):
+                        ro_diff = np.linalg.norm(
+                            np.array(ro_dup) - np.array(duplicate_data["RO_constant"][i])
+                        )
+                    if max([E_diff, H_diff, G_diff]) < abs(float(self.args.dup_threshold)):
+                        if (ro_dup is not None) and (ro_diff < self.args.ro_threshold):
+                            errortype = "duplicate_calc"
+                            dup_off = duplicate_data["File"][i]
 
         if errortype == "none":
             duplicate_data["File"].append(file_name)
             duplicate_data["Energies"].append(E_dup)
             duplicate_data["Enthalpies"].append(H_dup)
             duplicate_data["Gibbs"].append(G_dup)
             duplicate_data["RO_constant"].append(ro_dup)
```

### Comparing `aqme-1.4.7/aqme/qcorr_utils.py` & `aqme-1.5.0/aqme/qcorr_utils.py`

 * *Files identical despite different names*

### Comparing `aqme-1.4.7/aqme/qdescp.py` & `aqme-1.5.0/aqme/qdescp.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,16 +7,22 @@
 
    w_dir_main : str, default=os.getcwd()
       Working directory
    destination : str, default=None,
       Directory to create the JSON file(s)
    program : str, default=None
       Program required to create the new descriptors. Current options: 'xtb', 'nmr'
+   qdescp_atom : str, default=None
+      Type of atom to calculate atomic properties (i.e., qdescp_atom='P' to 
+      study the properties of phosphorus atoms in monodentate phosphines)
+   robert : bool, default=True
+      Creates a database ready to use in an AQME-ROBERT machine learning workflow,
+      combining the input CSV with SMILES/code_name and the calculated xTB/DBSTEP descriptors
 
-XTB descriptors
+xTB descriptors
 +++++++++++++++
 
    files : list of str, default=''
       Filenames of SDF/PDB/XYZ files to calculate xTB descriptors. If \*.sdf 
       (or other strings that are not lists such as \*.pdb) are specified, 
       the program will look for all the SDF files in the working directory 
       through glob.glob(\*.sdf)
@@ -32,14 +38,20 @@
       Temperature required for the xTB property calculations
    qdescp_acc : float, default=0.2
       Accuracy required for the xTB property calculations 
    boltz : bool, default=True
       Calculation of Boltzmann averaged xTB properties and addition of RDKit 
       molecular descriptors
 
+DBSTEP descriptors
+++++++++++++++
+
+   dbstep_r : float, default=3.5
+      Radius used in the DBSTEP calculations (in A)
+
 NMR simulation
 ++++++++++++++
 
    files : list of str, default=''
       Filenames of LOG files to retrieve NMR shifts from Gaussian calculations 
       (\*.log can be used to include all the log files in the working directory)
    boltz : bool, default=True
@@ -77,23 +89,24 @@
 import json
 import shutil
 import numpy as np
 from progress.bar import IncrementalBar
 import pandas as pd
 from rdkit import Chem
 from pathlib import Path
+import dbstep.Dbstep as db
 from aqme.utils import (
     load_variables,
     read_xyz_charge_mult,
     mol_from_sdf_or_mol_or_mol2,
     run_command,
     check_files
 )
 from aqme.qdescp_utils import (
-    get_boltz_avg_properties_xtb,
+    get_boltz_props,
     read_fod,
     read_json,
     read_xtb,
     read_wbo,
     read_gfn1,
     read_fukui
 )
@@ -128,34 +141,46 @@
                 qdescp_program = False
         if not qdescp_program:
             self.args.log.write("\nx  Program not supported for QDESCP descriptor generation! Specify: program='xtb' (or nmr)")
             self.args.log.finalize()
             sys.exit()
 
         if self.args.program.lower() == "xtb":
-            self.gather_files_and_run(destination)
+            mol_prop = ["total energy","HOMO-LUMO gap/eV","electronic energy","Dipole module/D",
+                "Total charge","HOMO","LUMO","Fermi-level/eV","Total dispersion C6",
+                "Total dispersion C8","Total polarizability alpha","Total FOD"]
+            atom_prop = ["partial charges","mulliken charges","cm5 charges","FUKUI+","FUKUI-",
+                "FUKUIrad","s proportion","p proportion","d proportion","Coordination numbers",
+                "Dispersion coefficient C6","Polarizability alpha","FOD","FOD s proportion",
+                "FOD p proportion","FOD d proportion",'DBSTEP_Vbur']
+            self.gather_files_and_run(destination,atom_prop)
+
+        elif self.args.program.lower() == "nmr":
+            mol_prop = None
+            atom_prop = ["NMR Chemical Shifts"]
 
         if self.args.boltz == "False":
             self.args.boltz = False
         elif self.args.boltz == "True":
             self.args.boltz = True
+
+        qdescp_csv = "QDESCP_boltz_descriptors.csv"
         if self.args.boltz:
+            self.args.log.write('\no  Running RDKit and collecting molecular properties')
             boltz_dir = Path(f"{destination}/boltz")
             boltz_dir.mkdir(exist_ok=True, parents=True)
             if self.args.program.lower() == "xtb":
                 for file in self.args.files:
                     mol = Chem.SDMolSupplier(file, removeHs=False)[0]
                     name = file.replace("/", "\\").split("\\")[-1].split(".")[0]
                     json_files = glob.glob(
                         str(destination) + "/" + name + "_conf_*.json"
                     )
-                    get_boltz_avg_properties_xtb(
-                        json_files, name, boltz_dir, "xtb", self, None, None, None, None, mol
-                    )
-                self.write_csv_boltz_data(destination)
+                    get_boltz_props(json_files, name, boltz_dir, "xtb", self, mol_prop, atom_prop, mol=mol)
+                self.write_csv_boltz_data(destination,qdescp_csv)
 
             elif self.args.program.lower() == "nmr":
                 if self.args.files[0].split('.')[1].lower() not in ["json"]:
                     self.args.log.write(f"\nx  The format used ({self.args.files[0].split('.')[1].lower()}) is not compatible with QDESCP with NMR! Formats accepted: json")
                     self.args.log.finalize()
                     sys.exit()
 
@@ -163,46 +188,74 @@
                     name = file.replace("/", "\\").split("\\")[-1].split("_conf")[0]
                     json_files = glob.glob(
                         str(os.path.dirname(os.path.abspath(file)))
                         + "/"
                         + name
                         + "_conf_*.json"
                     )
-                    get_boltz_avg_properties_xtb(
+                    get_boltz_props(
                         json_files,
                         name,
                         boltz_dir,
                         "nmr",
                         self,
+                        mol_prop,
+                        atom_prop,
                         self.args.nmr_atoms,
                         self.args.nmr_slope,
                         self.args.nmr_intercept,
                         self.args.nmr_experim,
                     )
 
+        if self.args.robert == "False":
+            self.args.robert = False
+        if self.args.robert:
+            if self.args.csv_name is None:
+                self.args.log.write(f"\n-  The input csv_name with SMILES and code_name is missing. A combined database for AQME-ROBERT workflows will not be created.")
+            elif not Path(f"{self.args.csv_name}").exists():
+                self.args.log.write(f"\nx  The input csv_name provided ({self.args.csv_name}) is not valid. A combined database for AQME-ROBERT workflows will not be created.")
+            else:
+                combined_df = pd.DataFrame()
+                qdescp_df = pd.read_csv(qdescp_csv)
+                input_df = pd.read_csv(self.args.csv_name)
+                if 'code_name' not in input_df.columns:
+                    self.args.log.write(f"\nx  The input csv_name provided ({self.args.csv_name}) does not contain the code_name column. A combined database for AQME-ROBERT workflows will not be created.")
+                elif 'SMILES' in input_df.columns or 'smiles' in input_df.columns or 'Smiles' in input_df.columns:
+                    path_json = os.path.dirname(Path(qdescp_df['Name'][0]))
+                    for i,input_name in enumerate(input_df['code_name']):
+                        # match the entries of the two databases using the entry name
+                        qdescp_col = input_df.loc[i].to_frame().T.reset_index(drop=True) # transposed, reset index
+                        input_col = qdescp_df.loc[(qdescp_df['Name'] == f'{path_json}/{input_name}_rdkit_boltz') | (qdescp_df['Name'] == f'{path_json}/{input_name}_boltz')]
+                        input_col = input_col.drop(['Name'], axis=1).reset_index(drop=True)
+                        combined_row = pd.concat([qdescp_col,input_col], axis=1)
+                        combined_df = combined_df.append(combined_row, ignore_index=True)
+                    _ = combined_df.to_csv(f'AQME-ROBERT_{self.args.csv_name}', index = None, header=True)
+                    self.args.log.write(f"o  The AQME-ROBERT_{self.args.csv_name} file containing the database ready for the AQME-ROBERT workflow was successfully created in {self.args.initial_dir}")
+                else:
+                    self.args.log.write(f"\nx  The input csv_name provided ({self.args.csv_name}) does not contain the SMILES column. A combined database for AQME-ROBERT workflows will not be created.")
+
         elapsed_time = round(time.time() - start_time_overall, 2)
         self.args.log.write(f"\nTime QDESCP: {elapsed_time} seconds\n")
         self.args.log.finalize()
 
-    def write_csv_boltz_data(self, destination):
+    def write_csv_boltz_data(self, destination, qdescp_csv):
         boltz_json_files = glob.glob(str(destination) + "/boltz/*.json")
         dfs = []  # an empty list to store the data frames
         for file in boltz_json_files:
             data = pd.read_json(file, lines=True)  # read data frame from json file
             data["Name"] = file.split(".json")[0]
             dfs.append(data)  # append the data frame to the list
 
         temp = pd.concat(
             dfs, ignore_index=True
         )  # concatenate all the data frames in the list.
-        qdescp_csv = "QDESCP_boltz_descriptors.csv"
         temp.to_csv(qdescp_csv, index=False)
-        self.args.log.write(f"o  The {qdescp_csv} file containing Boltzmann weighted xTB and RDKit descriptors was successfully created in {self.args.initial_dir}")
+        self.args.log.write(f"o  The {qdescp_csv} file containing Boltzmann weighted xTB, DBSTEP and RDKit descriptors was successfully created in {self.args.initial_dir}")
 
-    def gather_files_and_run(self, destination):
+    def gather_files_and_run(self, destination, atom_prop):
         bar = IncrementalBar(
             "\no  Number of finished jobs from QDESCP", max=len(self.args.files)
         )
         # write input files
         if self.args.files[0].split('.')[1].lower() not in ["sdf", "xyz", "pdb"]:
             self.args.log.write(f"\nx  The format used ({self.args.files[0].split('.')[1].lower()}) is not compatible with QDESCP with xTB! Formats accepted: sdf, xyz, pdb")
             self.args.log.finalize()
@@ -259,23 +312,23 @@
                         command_sdf,
                         stdout=subprocess.DEVNULL,
                         stderr=subprocess.DEVNULL,
                     )
 
             if file.split(".")[1].lower() in ["sdf", "pdb"]:
                 if self.args.charge is None:
-                    _, charges, _, _ = mol_from_sdf_or_mol_or_mol2(file, "csearch")
+                    _, charges, _, _ = mol_from_sdf_or_mol_or_mol2(file, "csearch", self.args)
                 else:
                     charges = [self.args.charge] * len(
                         glob.glob(
                             f"{os.path.dirname(os.path.abspath(file))}/{name}_conf_*.xyz"
                         )
                     )
                 if self.args.mult is None:
-                    _, _, mults, _ = mol_from_sdf_or_mol_or_mol2(file, "csearch")
+                    _, _, mults, _ = mol_from_sdf_or_mol_or_mol2(file, "csearch", self.args)
                 else:
                     mults = [self.args.mult] * len(
                         glob.glob(
                             f"{os.path.dirname(os.path.abspath(file))}/{name}_conf_*.xyz"
                         )
                     )
 
@@ -286,16 +339,17 @@
                 ):
                     xyz_files.append(f)
                     xyz_charges.append(charges[count])
                     xyz_mults.append(mults[count])
 
             for xyz_file, charge, mult in zip(xyz_files, xyz_charges, xyz_mults):
                 name = os.path.basename(xyz_file.split(".")[0])
+                self.args.log.write(f"\n   Running xTB and collecting properties")
                 self.run_sp_xtb(xyz_file, charge, mult, name, destination)
-                self.collect_xtb_properties()
+                self.collect_xtb_properties(atom_prop)
                 self.cleanup(name, destination)
             bar.next()
         bar.finish()
 
     def run_sp_xtb(self, xyz_file, charge, mult, name, destination):
         """
         Runs single point xTB calculations to collect properties
@@ -404,15 +458,15 @@
         if self.args.qdescp_solvent is not None:
             command4.append("--alpb")
             command4.append(f"{self.args.qdescp_solvent}")
         run_command(command4, self.xtb_fod)
 
         os.chdir(self.args.initial_dir)
 
-    def collect_xtb_properties(self):
+    def collect_xtb_properties(self,atom_prop):
         """
         Collects all xTB properties from the files and puts them in a JSON file
         """
 
         (
             energy,
             total_charge,
@@ -449,14 +503,15 @@
         for i, bond in enumerate(bonds):
             wbo_matrix[(bond[0] - 1)][(bond[1] - 1)] = wbos[i]
             wbo_matrix[(bond[1] - 1)][(bond[0] - 1)] = wbos[i]
 
         """
 		Now add xTB descriptors to existing json files.
 		"""
+
         json_data = read_json(self.xtb_json)
         json_data["Dipole module/D"] = dipole_module
         json_data["Total charge"] = total_charge
         json_data["Transition dipole module/D"] = transition_dipole_moment
         json_data["HOMO"] = homo
         json_data["LUMO"] = lumo
         json_data["HOMO occupancy"] = homo_occ
@@ -486,20 +541,55 @@
         json_data["FOD s proportion"] = s_prop_fod
         json_data["FOD p proportion"] = p_prop_fod
         json_data["FOD d proportion"] = d_prop_fod
 
         with open(self.xtb_xyz, "r") as f:
             inputs = f.readlines()
 
-        coordinates = [
-            inputs[i].strip().split()[1:] for i in range(2, int(inputs[0].strip()) + 2)
-        ]
-
+        coordinates = [inputs[i].strip().split()[1:] for i in range(2, int(inputs[0].strip()) + 2)]
         json_data["coordinates"] = coordinates
 
+        
+        if self.args.qdescp_atom is not None:
+            idx_dbstep, idx_xtb = None, None
+
+            # calculate DBSTEP descriptors
+            self.args.log.write(f"\n   Running DBSTEP and collecting properties")
+
+            hit_at = 0
+            for i,line in enumerate(inputs):
+                if i > 2:
+                    if line.split()[0] == self.args.qdescp_atom:
+                        hit_at += 1
+                        idx_dbstep = i-1 # DBSTEP starts from index 1 (i.e. first atom has idx 1)
+                        idx_xtb = i-2
+
+            if hit_at > 1:
+                self.args.log.write(f'WARNING! More than one {self.args.qdescp_atom} were found, using {self.args.qdescp_atom} with index {idx_dbstep}.')
+
+            if idx_dbstep is not None:
+                # calculates buried volume to the type of atom selected
+                try:
+                    dbstep_obj = db.dbstep(self.xtb_xyz,atom1=idx_dbstep,r=float(self.args.dbstep_r),commandline=True,verbose=False,volume=True)  
+                    json_data['DBSTEP_Vbur'] = float(dbstep_obj.bur_vol)
+                except TypeError:
+                    self.args.log.write(f'WARNING! DBSTEP is not working correctly, DBSTEP properties will not be calculated.')
+                    json_data['DBSTEP_Vbur'] = 'NaN'
+
+                # selects xTB atom properties
+                for prop in atom_prop:
+                    if prop != 'DBSTEP_Vbur': # already set the value of the atom instead of a list of values
+                        json_data[prop] = json_data[prop][idx_xtb]
+
+            else:
+                self.args.log.write(f'WARNING! No {self.args.qdescp_atom} atoms were found, using NaN as the value.')
+                json_data['DBSTEP_Vbur'] = 'NaN'
+                for prop in atom_prop:
+                    json_data[prop] = 'NaN'
+
         with open(self.xtb_json, "w") as outfile:
             json.dump(json_data, outfile)
 
     def cleanup(self, name, destination):
         final_json = str(destination) + "/" + name + ".json"
         shutil.move(self.xtb_json, final_json)
         # delete xTB files that does not contain useful data
```

### Comparing `aqme-1.4.7/aqme/qdescp_utils.py` & `aqme-1.5.0/aqme/qdescp_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import json
 import sys
 import numpy as np
 import pandas as pd
 import ast
 import math
 import rdkit
+import warnings
+warnings.filterwarnings('ignore')
 
 GAS_CONSTANT = 8.3144621  # J / K / mol
 J_TO_AU = 4.184 * 627.509541 * 1000.0  # UNIT CONVERSION
 T = 298.15
 
 
 def get_boltz(energy):
@@ -30,78 +32,42 @@
     for e in energ:
         weight = math.exp(-e * J_TO_AU / GAS_CONSTANT / T) / boltz_sum
         weights.append(weight)
 
     return weights
 
 
-def get_boltz_avg_properties_xtb(
+def get_boltz_props(
     json_files,
     name,
     boltz_dir,
     type,
     self,
+    mol_prop,
+    atom_prop,
     nmr_atoms=None,
     nmr_slope=None,
     nmr_intercept=None,
     nmr_experim=None,
     mol=None,
 ):
     """
     Retrieves the properties from json files and gives Boltzmann averaged properties
     """
 
-    if type == "xtb":
-        mol_prop = [
-            "total energy",
-            "HOMO-LUMO gap/eV",
-            "electronic energy",
-            "Dipole module/D",
-            "Total charge",
-            "HOMO",
-            "LUMO",
-            "Fermi-level/eV",
-            "Total dispersion C6",
-            "Total dispersion C8",
-            "Total polarizability alpha",
-            "Total FOD",
-        ]
-        atom_prop = [
-            "dipole",
-            "partial charges",
-            "mulliken charges",
-            "cm5 charges",
-            "FUKUI+",
-            "FUKUI-",
-            "FUKUIrad",
-            "s proportion",
-            "p proportion",
-            "d proportion",
-            "Coordination numbers",
-            "Dispersion coefficient C6",
-            "Polarizability alpha",
-            "FOD",
-            "FOD s proportion",
-            "FOD p proportion",
-            "FOD d proportion",
-        ]
-    elif type == "nmr":
-        atom_prop = [
-            "NMR Chemical Shifts",
-        ]
+    if type == "nmr":
         if nmr_experim is not None:
             try:
                 exp_data = pd.read_csv(nmr_experim)
             except:
                 self.args.log.write(f'\nx  The CSV file with experimental NMR shifts specified ({nmr_experim}) was not found!')
                 self.args.log.finalize()
                 sys.exit()
 
     energy = []
-
     for k, json_file in enumerate(json_files):
         json_data = read_json(json_file)
         if type == "xtb":
             energy.append(json_data["total energy"])
         elif type == "nmr":
             energy.append(json_data["optimization"]["scf"]["scf energies"][-1])
 
@@ -122,19 +88,24 @@
     boltz = get_boltz(energy)
 
     avg_json_data = {}
     for prop in atom_prop:
         prop_list = []
         for json_file in json_files:
             json_data = read_json(json_file)
+            if self.args.qdescp_atom is None:
+                json_data['DBSTEP_Vbur'] = 'NaN'
             if type == "xtb":
                 prop_list.append(json_data[prop])
             if type == "nmr":
                 prop_list.append(json_data["properties"]["NMR"][prop].values())
-        avg_prop = average_prop_atom(boltz, prop_list)
+        if self.args.qdescp_atom is None:
+            avg_prop = average_prop_atom(boltz, prop_list)
+        else:
+            avg_prop = average_prop_mol(boltz, prop_list)
 
         if type == "nmr":
             dictavgprop = {}
             for i, key in enumerate(json_data["properties"]["NMR"][prop].keys()):
                 dictavgprop[key] = avg_prop[i]
             avg_json_data[prop] = dictavgprop
 
@@ -150,26 +121,31 @@
                     exp_data["experimental_ppm"] - exp_data["boltz_avg"]
                 )
                 qdescp_nmr = nmr_experim.split(".csv")[0] + "_predicted.csv"
                 exp_data.round(2).to_csv(qdescp_nmr, index=False)
                 self.args.log.write(f"o  The {qdescp_nmr} file containing Boltzmann weighted NMR shifts was successfully created in {self.args.initial_dir}")
 
         elif type == "xtb":
-            avg_json_data[prop] = avg_prop.tolist()
+            if self.args.qdescp_atom is not None or avg_prop == 'NaN':
+                avg_json_data[prop] = avg_prop
+            else:
+                avg_json_data[prop] = avg_prop.tolist()                
 
     if type == "xtb":
         for prop in mol_prop:
             prop_list = []
             for json_file in json_files:
                 json_data = read_json(json_file)
                 prop_list.append(json_data[prop])
             avg_prop = average_prop_mol(boltz, prop_list)
             avg_json_data[prop] = avg_prop
 
     final_boltz_file = str(boltz_dir) + "/" + name + "_boltz.json"
+    
+    # calculate RDKit descriptors
     if mol is not None:
         avg_json_data = get_rdkit_properties(avg_json_data, mol)
     with open(final_boltz_file, "w") as outfile:
         json.dump(avg_json_data, outfile)
 
 
 def get_chemical_shifts(json_data, nmr_atoms, nmr_slope, nmr_intercept):
@@ -207,26 +183,35 @@
 def average_prop_atom(weights, prop):
     """
     Returns Boltzmann averaged atomic properties
     """
 
     boltz_avg = []
     for i, p in enumerate(prop):
+        if p == 'NaN':
+            boltz_avg = 'NaN'
+            break
         boltz_avg.append([number * weights[i] for number in p])
-    boltz_res = np.sum(boltz_avg, 0)
+    if boltz_avg == 'NaN':
+        boltz_res = 'NaN'
+    else:
+        boltz_res = np.sum(boltz_avg, 0)
     return boltz_res
 
 
 def average_prop_mol(weights, prop):
     """
     Returns Boltzmann averaged molecular properties
     """
 
     boltz_avg = 0.0
     for i, p in enumerate(prop):
+        if p == 'NaN':
+            boltz_avg = 'NaN'
+            break
         boltz_avg += p * weights[i]
     return boltz_avg
 
 
 def get_rdkit_properties(avg_json_data, mol):
     """
     Calculates RDKit molecular descriptors
```

### Comparing `aqme-1.4.7/aqme/qprep.py` & `aqme-1.5.0/aqme/qprep.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,14 +37,21 @@
       Number of processors used in the QM calculations
    gen_atoms : list of str, default=[]
       Atoms included in the gen(ECP) basis set (i.e. ['I','Pd'])
    bs_gen : str, default=''
       Basis set used for gen(ECP) atoms (i.e. 'def2svp')
    bs_nogen : str, default=''
       Basis set used for non gen(ECP) atoms in gen(ECP) calculations (i.e. '6-31G*')
+   lowest_only : bool, default=False
+      Only create input for the conformer with lowest energy of the SDF file
+   lowest_n : int, default=None
+      Only create inputs for the n conformers with lowest energy of the SDF file
+   e_threshold_qprep : float, default=None
+      Only create inputs for conformers below the energy threshold (to the lowest conformer)
+      of the SDF file
 """
 ######################################################.
 #        This file stores the QPREP class            #
 ######################################################.
 
 import os
 import subprocess
@@ -127,15 +134,22 @@
                 sdf_files = []
                 if file_format.lower() == "xyz":
                     # separate the parent XYZ file into individual XYZ files
                     xyzall_2_xyz(file, f"{self.args.w_dir_main}/{name}")
                     for conf_file in glob.glob(
                         f"{self.args.w_dir_main}/{name}_conf_*.xyz"
                     ):
-                        charge_xyz, mult_xyz = read_xyz_charge_mult(conf_file)
+                        if self.args.charge is None:
+                            charge_xyz, _ = read_xyz_charge_mult(conf_file)
+                        else:
+                            charge_xyz = self.args.charge
+                        if self.args.mult is None:
+                            _, mult_xyz = read_xyz_charge_mult(conf_file)
+                        else:
+                            mult_xyz = self.args.mult
                         # generate SDF files from XYZ with Openbabel
                         command_xyz = [
                             "obabel",
                             "-ixyz",
                             conf_file,
                             "-osdf",
                             f"-O{conf_file.split('.xyz')[0]}.sdf",
@@ -212,15 +226,24 @@
             elapsed_time = round(time.time() - start_time_overall, 2)
             self.args.log.write(f"\nTime QPREP: {elapsed_time} seconds\n")
             self.args.log.finalize()
 
     def sdf_2_com(self, sdf_file, destination, file_format):
         sdf_name = os.path.basename(sdf_file).split(".")[0]
         # get atom types, atomic coordinates, charge and multiplicity of all the mols in the SDF file
-        mols = mol_from_sdf_or_mol_or_mol2(sdf_file, "qprep")
+
+        low_check = None
+        if self.args.lowest_only == True:
+            low_check='lowest_only'
+        if self.args.lowest_n is not None:
+            low_check=int(self.args.lowest_n)
+        if self.args.e_threshold_qprep is not None:
+            low_check=float(self.args.e_threshold_qprep)
+        mols = mol_from_sdf_or_mol_or_mol2(sdf_file, "qprep", self.args, low_check=low_check)
+
         for i, mol in enumerate(mols):
             (
                 atom_types,
                 cartesians,
                 charge,
                 mult,
                 _,
```

### Comparing `aqme-1.4.7/aqme/templates/template-4-and-5.sdf` & `aqme-1.5.0/aqme/templates/template-4-and-5.sdf`

 * *Files identical despite different names*

### Comparing `aqme-1.4.7/aqme/utils.py` & `aqme-1.5.0/aqme/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from aqme.argument_parser import set_options, var_dict
 from rdkit import RDLogger
 
 GAS_CONSTANT = 8.3144621  # J / K / mol
 J_TO_AU = 4.184 * 627.509541 * 1000.0  # UNIT CONVERSION
 T = 298.15
 
-aqme_version = "1.4.8"
+aqme_version = "1.5.0"
 time_run = time.strftime("%Y/%m/%d %H:%M:%S", time.localtime())
 aqme_ref = f"AQME v {aqme_version}, Alegre-Requena, J. V.; Sowndarya, S.; Perez-Soto, R.; Alturaifi, T.; Paton, R. AQME: Automated Quantum Mechanical Environments for Researchers and Educators. Wiley Interdiscip. Rev. Comput. Mol. Sci. 2023, DOI: 10.1002/wcms.1663."
 
 RDLogger.DisableLog("rdApp.*")
 
 
 def run_command(command, outfile):
@@ -329,16 +329,17 @@
         "qprep",
         "qcorr",
         "qdescp",
         "vismol",
         "heavyonly",
         "cregen",
         "lowest_only",
-        "lowest_n",
         "chk",
+        "nodup_check",
+        "robert"
     ]
 
     for arg in var_dict:
         if arg in bool_args:
             available_args.append(f"{arg}")
         else:
             available_args.append(f"{arg} =")
@@ -378,15 +379,15 @@
                                 value = value.replace('[',']').replace(',',']').split(']')
                                 while('' in value):
                                     value.remove('')
                 kwargs[arg_name] = value
 
     # Second, load all the default variables as an "add_option" object
     args = load_variables(kwargs, "command")
-
+    
     return args
 
 
 def load_variables(kwargs, aqme_module, create_dat=True):
     """
     Load default and user-defined variables
     """
@@ -609,38 +610,53 @@
 
     charge_xyz, mult_xyz = None, None
     # read charge and mult from xyz files
     with open(file, "r") as F:
         lines = F.readlines()
     for line in lines:
         for keyword in line.strip().split():
-            if keyword.lower().find("charge") > -1:
+            if keyword.lower().find("charge=") > -1:
                 charge_xyz = int(keyword.split("=")[1])
-            elif keyword.lower().find("mult") > -1:
+            elif keyword.lower().find("mult=") > -1:
                 mult_xyz = int(keyword.split("=")[1])
             elif charge_xyz is not None and mult_xyz is not None:
                 break
 
     if charge_xyz is None:
         charge_xyz = 0
     if mult_xyz is None:
         mult_xyz = 1
 
     return charge_xyz, mult_xyz
 
 
-def mol_from_sdf_or_mol_or_mol2(input_file, module):
+def mol_from_sdf_or_mol_or_mol2(input_file, module, args, low_check=None):
+
     """
     mol object from SDF, MOL or MOL2 files
     """
-
     if module in ["qprep","cmin"]:
         # using sanitize=False to avoid reading problems
         mols = Chem.SDMolSupplier(input_file, removeHs=False, sanitize=False)
-        return mols
+        if low_check=='lowest_only':
+            return [mols[0]]
+        elif isinstance(low_check, int):
+            check_n = min(len(mols),low_check)
+            n_mols = []
+            for i in range(check_n):
+                n_mols.append(mols[i])
+            return n_mols
+        elif isinstance(low_check, float):
+            n_mols = []
+            for i in range(len(mols)):
+                if abs(float(mols[i].GetProp('Energy')) - float(mols[0].GetProp('Energy'))) < low_check: # kcal/mol
+                    n_mols.append(mols[i])
+            return n_mols
+        else:
+            return mols
 
     elif module == "csearch":
 
         # using sanitize=True in this case, which is recommended for RDKit calculations
         filename = os.path.splitext(input_file)[0]
         extension = os.path.splitext(input_file)[1]
 
@@ -685,18 +701,23 @@
         if len(IDs) == 0:
             if len(suppl) > 1:
                 for i in range(len(suppl)):
                     IDs.append(f"{filename}_{i+1}")
             else:
                 IDs.append(filename)
 
-        if len(charges) == 0:
+        if args.charge is not None:
+            for i, mol in enumerate(mols):
+                charges.append(args.charge)
+        elif len(charges) == 0:
             for i, mol in enumerate(mols):
                 charges.append(Chem.GetFormalCharge(mol))
-        if len(mults) == 0:
+        if args.mult is not None:
+            mults.append(args.mult)
+        elif len(mults) == 0:
             for i, mol in enumerate(mols):
                 NumRadicalElectrons = 0
                 for Atom in mol.GetAtoms():
                     NumRadicalElectrons += Atom.GetNumRadicalElectrons()
                 TotalElectronicSpin = NumRadicalElectrons / 2
                 mult = int((2 * TotalElectronicSpin) + 1)
                 mults.append(mult)
```

### Comparing `aqme-1.4.7/aqme/vismol.py` & `aqme-1.5.0/aqme/vismol.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,16 @@
                         stderr=subprocess.DEVNULL,
                     )
                     sdf_files.append(f"{name}.sdf")
                 else:
                     sdf_files.append(file)
 
             for sdf_file in sdf_files:
-                self.confs = mol_from_sdf_or_mol_or_mol2(sdf_file, "qprep")
+                self.confs = mol_from_sdf_or_mol_or_mol2(sdf_file, "qprep", self.args)
+
                 interact(
                     self.style_selector,
                     idx=ipywidgets.IntSlider(min=0, max=len(self.confs) - 1, step=1),
                     s=ipywidgets.Dropdown(
                         options=["line", "stick", "sphere"],
                         value="line",
                         description="Style:",
```

### Comparing `aqme-1.4.7/aqme.egg-info/PKG-INFO` & `aqme-1.5.0/aqme.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: aqme
-Version: 1.4.7
+Version: 1.5.0
 Summary: Automated Quantum Mechanical Environments
 Home-page: https://github.com/jvalegre/aqme
-Download-URL: https://github.com/jvalegre/aqme/archive/refs/tags/1.4.7.tar.gz
+Download-URL: https://github.com/jvalegre/aqme/archive/refs/tags/1.5.0.tar.gz
 Author: Shree Sowndarya S. V., Juan V. Alegre Requena
 Author-email: svss@colostate.edu, jvalegre@unizar.es
 License: MIT
 Keywords: workflows,computational chemistry,conformational sampling,cheminformatics,quantum mechanics,DFT,automated
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Documentation in Read The Docs: https://aqme.readthedocs.io
-
```

### Comparing `aqme-1.4.7/aqme.egg-info/SOURCES.txt` & `aqme-1.5.0/aqme.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -25,8 +25,13 @@
 aqme/csearch/base.py
 aqme/csearch/crest.py
 aqme/csearch/fullmonte.py
 aqme/csearch/templates.py
 aqme/csearch/utils.py
 aqme/templates/template-2.sdf
 aqme/templates/template-3.sdf
-aqme/templates/template-4-and-5.sdf
+aqme/templates/template-4-and-5.sdf
+tests/test_cmin.py
+tests/test_csearch.py
+tests/test_qcorr.py
+tests/test_qdescp.py
+tests/test_qprep.py
```

### Comparing `aqme-1.4.7/setup.py` & `aqme-1.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from setuptools import setup, find_packages
-version = "1.4.7"
+version = "1.5.0"
 setup(
     name="aqme",
     packages=find_packages(exclude=["tests"]),
     package_data={"aqme": ["templates/*"]},
     version=version,
     license="MIT",
     description="Automated Quantum Mechanical Environments",
@@ -40,12 +40,13 @@
         "numpy",
         "cclib",
         "matplotlib",
         "seaborn",
         "cffi",
         "goodvibes",
         "py3Dmol",
-        "ipywidgets"
+        "ipywidgets",
+        "dbstep"
     ],
     python_requires=">=3.0",
     include_package_data=True,
 )
```

