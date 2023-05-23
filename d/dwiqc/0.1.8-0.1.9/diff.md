# Comparing `tmp/dwiqc-0.1.8-py2.py3-none-any.whl.zip` & `tmp/dwiqc-0.1.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 21805 bytes, number of entries: 20
+Zip file size: 21814 bytes, number of entries: 20
 -rw-r--r--  2.0 unx      225 b- defN 23-May-19 16:11 dwiqc/__init__.py
--rw-r--r--  2.0 unx      247 b- defN 23-May-23 11:28 dwiqc/__version__.py
+-rw-r--r--  2.0 unx      247 b- defN 23-May-23 13:22 dwiqc/__version__.py
 -rw-r--r--  2.0 unx       62 b- defN 23-May-19 16:11 dwiqc/cli/__init__.py
 -rw-r--r--  2.0 unx     6651 b- defN 23-May-19 16:11 dwiqc/cli/get.py
 -rw-r--r--  2.0 unx     5273 b- defN 23-May-19 16:11 dwiqc/cli/process.py
 -rw-r--r--  2.0 unx      160 b- defN 23-May-19 16:11 dwiqc/config/__init__.py
 -rw-r--r--  2.0 unx      274 b- defN 23-May-19 16:11 dwiqc/config/dwiqc.yaml
 -rw-r--r--  2.0 unx       98 b- defN 23-May-19 16:11 dwiqc/state/__init__.py
 -rw-r--r--  2.0 unx     1892 b- defN 23-May-19 16:11 dwiqc/tasks/__init__.py
--rw-r--r--  2.0 unx     8639 b- defN 23-May-22 18:04 dwiqc/tasks/prequal.py
+-rw-r--r--  2.0 unx     8696 b- defN 23-May-23 13:17 dwiqc/tasks/prequal.py
 -rw-r--r--  2.0 unx     4209 b- defN 23-May-22 17:12 dwiqc/tasks/prequal_EQ.py
 -rw-r--r--  2.0 unx     6193 b- defN 23-May-23 11:24 dwiqc/tasks/qsiprep.py
 -rw-r--r--  2.0 unx     3782 b- defN 23-May-19 16:11 dwiqc/tasks/qsiprep_EQ.py
--rw-r--r--  2.0 unx    13839 b- defN 23-May-19 16:11 dwiqc/xnat/__init__.py
--rwxr-xr-x  2.0 unx     3889 b- defN 23-May-23 11:29 dwiqc-0.1.8.data/scripts/dwiQC.py
--rw-r--r--  2.0 unx     1541 b- defN 23-May-23 11:29 dwiqc-0.1.8.dist-info/LICENSE
--rw-r--r--  2.0 unx      411 b- defN 23-May-23 11:29 dwiqc-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-23 11:29 dwiqc-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-May-23 11:29 dwiqc-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1559 b- defN 23-May-23 11:29 dwiqc-0.1.8.dist-info/RECORD
-20 files, 59060 bytes uncompressed, 19293 bytes compressed:  67.3%
+-rw-r--r--  2.0 unx    13810 b- defN 23-May-23 12:53 dwiqc/xnat/__init__.py
+-rwxr-xr-x  2.0 unx     3889 b- defN 23-May-23 13:23 dwiqc-0.1.9.data/scripts/dwiQC.py
+-rw-r--r--  2.0 unx     1541 b- defN 23-May-23 13:23 dwiqc-0.1.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx      388 b- defN 23-May-23 13:23 dwiqc-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-23 13:23 dwiqc-0.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-May-23 13:23 dwiqc-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1559 b- defN 23-May-23 13:23 dwiqc-0.1.9.dist-info/RECORD
+20 files, 59065 bytes uncompressed, 19302 bytes compressed:  67.3%
```

## zipnote {}

```diff
@@ -36,26 +36,26 @@
 
 Filename: dwiqc/tasks/qsiprep_EQ.py
 Comment: 
 
 Filename: dwiqc/xnat/__init__.py
 Comment: 
 
-Filename: dwiqc-0.1.8.data/scripts/dwiQC.py
+Filename: dwiqc-0.1.9.data/scripts/dwiQC.py
 Comment: 
 
-Filename: dwiqc-0.1.8.dist-info/LICENSE
+Filename: dwiqc-0.1.9.dist-info/LICENSE
 Comment: 
 
-Filename: dwiqc-0.1.8.dist-info/METADATA
+Filename: dwiqc-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: dwiqc-0.1.8.dist-info/WHEEL
+Filename: dwiqc-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: dwiqc-0.1.8.dist-info/top_level.txt
+Filename: dwiqc-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: dwiqc-0.1.8.dist-info/RECORD
+Filename: dwiqc-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dwiqc/__version__.py

```diff
@@ -1,6 +1,6 @@
 __title__ = 'dwiqc'
 __description__ = 'Quality Assurance Pipeline for Diffusion MR Data'
 __url__ = 'https://github.com/harvard-nrg/dwiqc'
-__version__ = '0.1.8'
+__version__ = '0.1.9'
 __author__ = 'Neuroinformatics Research Group'
 __author_email__ = 'info@neuroinfo.org'
```

## dwiqc/tasks/prequal.py

```diff
@@ -259,15 +259,18 @@
 
 
 	# build the prequal sbatch command and create job
 
 	def build(self):
 		self.add_intended_for()
 		cwd = os.getcwd()
+		print(self._tempdir)
 		os.chdir(self._tempdir)
+		print(os.getcwd())
+		sys.exit()
 		os.chdir(cwd)
 		inputs_dir = f'{self._tempdir}/INPUTS/'
 		self.copy_inputs(inputs_dir)
 		self._command = [
 			'selfie',
 			'--lock',
 			'--output-file', self._prov,
```

## dwiqc/xnat/__init__.py

```diff
@@ -7,15 +7,14 @@
 import json
 import lxml
 import shutil
 import zipfile
 import logging
 import numpy as np
 from lxml import etree
-from anatqc.bids import BIDS
 from bids import BIDSLayout
 
 logger = logging.getLogger(__name__)
 
 EDDY_METRICS = [
     'Average_SNR_b0', 'Average_CNR_b500','Average_CNR_b1000', 'Average_CNR_b2000', 
     'Average_CNR_b3000', 'Average_abs_motion_mm', 'Average_rel_motion_mm', 'Average_x_translation_mm',
```

## Comparing `dwiqc-0.1.8.data/scripts/dwiQC.py` & `dwiqc-0.1.9.data/scripts/dwiQC.py`

 * *Files identical despite different names*

## Comparing `dwiqc-0.1.8.dist-info/LICENSE` & `dwiqc-0.1.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dwiqc-0.1.8.dist-info/RECORD` & `dwiqc-0.1.9.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 dwiqc/__init__.py,sha256=MZJhUZKhHHoZ2w_GeoFCITk1m_0ASdRw_ZaeDixFEPU,225
-dwiqc/__version__.py,sha256=AFgFyRC_s-GU0o83hx5AukoI-CFOT-T6_JOzloH3plI,247
+dwiqc/__version__.py,sha256=s0Ubik8_58WTORo_NGEJ5QXWgfZgTdyq_fUnySJkR2U,247
 dwiqc/cli/__init__.py,sha256=zGIm7lrjh3wA191D-VjQBZNjSlspFUx148VwDNQGaTk,62
 dwiqc/cli/get.py,sha256=6ixaBdwEgY_GXh8L-_3QDY4MEsNqSJgXle_mxW99mlk,6651
 dwiqc/cli/process.py,sha256=X4eUXf-jRuOR_3cVQ0FfcDXmNPVQzILH35uGAtz9upE,5273
 dwiqc/config/__init__.py,sha256=k_w5JzoJN_7R7eI_sIJxHA4FQQHs0_KGf-6jsbG4Xs8,160
 dwiqc/config/dwiqc.yaml,sha256=x8gKMFZyChdzvNX3GthRe0eWvyKDDL5itXo0kLWVfd0,274
 dwiqc/state/__init__.py,sha256=NaRifw26bI3F1J9BqeLa-KLSzEPq2m_UNhMbXdmPdh4,98
 dwiqc/tasks/__init__.py,sha256=LnlN7iYjpqiBic2ihFrM-_h7m8FD_N7Beh7UIwKyGZ8,1892
-dwiqc/tasks/prequal.py,sha256=DcZH8kYTaJ5jGM5niR2U-RUMSgu9C0HMvcEmEbHj5AA,8639
+dwiqc/tasks/prequal.py,sha256=vbjvACbD4kNSQScpYC_cYf20SyUVhve-hqo6Y_bazo4,8696
 dwiqc/tasks/prequal_EQ.py,sha256=PWmlo8u_D5qM1lyXdmT7iq865JL6xoPM0JHGEwzRnes,4209
 dwiqc/tasks/qsiprep.py,sha256=2HAmLSSXyKRUuYmok9EEmoPaSo8_7LoCAU-JGfudeiY,6193
 dwiqc/tasks/qsiprep_EQ.py,sha256=JWildptHsuyJVj7ZYMFlWWYvsAIszJpWk1a0m05JM-Q,3782
-dwiqc/xnat/__init__.py,sha256=PyJJtcfxf71c9x1LwdCem2bT_2MNuqhRmb0uLTfoGgs,13839
-dwiqc-0.1.8.data/scripts/dwiQC.py,sha256=OkI1WZqnUIqS4DWSt-pSm01taEv3m_aNmqSJUM50N_U,3889
-dwiqc-0.1.8.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
-dwiqc-0.1.8.dist-info/METADATA,sha256=dxxF4Y0IG2t8IpiANgsGs8KRHAhh1qlCP1pMU3ocbEk,411
-dwiqc-0.1.8.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-dwiqc-0.1.8.dist-info/top_level.txt,sha256=omH7pmKt7fzFyiNkTPDLX4yyBccoge5Saqc9rgyu0Wk,6
-dwiqc-0.1.8.dist-info/RECORD,,
+dwiqc/xnat/__init__.py,sha256=8jjaZO_5JlUhiSHNsmDr59HsfOS-uZAunSQuLPUXb1g,13810
+dwiqc-0.1.9.data/scripts/dwiQC.py,sha256=OkI1WZqnUIqS4DWSt-pSm01taEv3m_aNmqSJUM50N_U,3889
+dwiqc-0.1.9.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
+dwiqc-0.1.9.dist-info/METADATA,sha256=xaGdhumZ8S4f0eMWQZ50M-BaaZxBXhDplwqpUHubiPs,388
+dwiqc-0.1.9.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+dwiqc-0.1.9.dist-info/top_level.txt,sha256=omH7pmKt7fzFyiNkTPDLX4yyBccoge5Saqc9rgyu0Wk,6
+dwiqc-0.1.9.dist-info/RECORD,,
```

