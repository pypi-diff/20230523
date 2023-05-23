# Comparing `tmp/xarrayaita-0.2.6-py3-none-any.whl.zip` & `tmp/xarrayaita-0.2.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 28568 bytes, number of entries: 13
+Zip file size: 29049 bytes, number of entries: 13
 -rw-r--r--  2.0 unx      263 b- defN 23-Apr-18 08:38 xarrayaita/__init__.py
 -rw-r--r--  2.0 unx     1347 b- defN 22-Sep-27 07:28 xarrayaita/aita.py
--rw-r--r--  2.0 unx     4898 b- defN 22-Sep-27 07:28 xarrayaita/aita_export.py
+-rw-r--r--  2.0 unx     6863 b- defN 23-May-23 13:51 xarrayaita/aita_export.py
 -rw-r--r--  2.0 unx     6679 b- defN 22-Sep-27 07:28 xarrayaita/aita_geom.py
 -rw-r--r--  2.0 unx    16005 b- defN 22-Sep-27 07:28 xarrayaita/aita_interactive_nb.py
 -rw-r--r--  2.0 unx      975 b- defN 22-Nov-17 13:24 xarrayaita/aita_plot.py
 -rw-r--r--  2.0 unx    12164 b- defN 22-Sep-27 07:28 xarrayaita/aita_processing.py
 -rw-r--r--  2.0 unx     6899 b- defN 23-Apr-18 08:37 xarrayaita/loadData_aita.py
--rw-r--r--  2.0 unx    35149 b- defN 23-Apr-18 08:46 xarrayaita-0.2.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     1072 b- defN 23-Apr-18 08:46 xarrayaita-0.2.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-18 08:46 xarrayaita-0.2.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Apr-18 08:46 xarrayaita-0.2.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1058 b- defN 23-Apr-18 08:46 xarrayaita-0.2.6.dist-info/RECORD
-13 files, 86612 bytes uncompressed, 26810 bytes compressed:  69.0%
+-rw-r--r--  2.0 unx    35149 b- defN 23-May-23 14:01 xarrayaita-0.2.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1053 b- defN 23-May-23 14:01 xarrayaita-0.2.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-23 14:01 xarrayaita-0.2.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-May-23 14:01 xarrayaita-0.2.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1058 b- defN 23-May-23 14:01 xarrayaita-0.2.7.dist-info/RECORD
+13 files, 88558 bytes uncompressed, 27291 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: xarrayaita/aita_processing.py
 Comment: 
 
 Filename: xarrayaita/loadData_aita.py
 Comment: 
 
-Filename: xarrayaita-0.2.6.dist-info/LICENSE
+Filename: xarrayaita-0.2.7.dist-info/LICENSE
 Comment: 
 
-Filename: xarrayaita-0.2.6.dist-info/METADATA
+Filename: xarrayaita-0.2.7.dist-info/METADATA
 Comment: 
 
-Filename: xarrayaita-0.2.6.dist-info/WHEEL
+Filename: xarrayaita-0.2.7.dist-info/WHEEL
 Comment: 
 
-Filename: xarrayaita-0.2.6.dist-info/top_level.txt
+Filename: xarrayaita-0.2.7.dist-info/top_level.txt
 Comment: 
 
-Filename: xarrayaita-0.2.6.dist-info/RECORD
+Filename: xarrayaita-0.2.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xarrayaita/aita_export.py

```diff
@@ -14,24 +14,26 @@
 from IPython import get_ipython
 if get_ipython().__class__.__name__ == 'ZMQInteractiveShell':
     from tqdm.notebook import tqdm
 else:
     from tqdm import tqdm
 
 
-def craft(self, nameId, res=0, m3d=0):
+def craft(self, nameId, res=0, m3d=0,tesr=False):
     '''
     Export 'vtk' file and the phase file. 
 
     :param res: resolution for the vtk export
     :type res: float
     :param nameId: name of manipulation
     :type nameTd: string
     :param m3d: 0 for 2 dimensional data, 1 for 3 dimensional data
     :type m3d: int
+    :param tesr: export tesr file compatible with neper
+    :type tesr: bool
     '''
     zoom = self._obj.step_size/res
 
     # Copy and compute mean grain
     ds = self._obj.copy()
     ds['orientation_mg'] = ds.aita.mean_grain()
     # Remove hole in grainId
@@ -117,16 +119,80 @@
             phi2 = float(np.random.rand(1)*2*np.pi)
             if np.isnan(phi1):
                 phi1 = float(np.random.rand(1)*2*np.pi)
                 phi = float(np.random.rand(1)*2*np.pi)
             phase_out.write(str(i) + '          0              ' +
                             str(phi1) + ' ' + str(phi) + ' ' + str(phi2) + '\n')
     phase_out.close()
+    # ----------------------------------------------------
+    # Export tesr file if needed
+    if tesr:
+        micro=np.loadtxt(nameId+'_micro.vtk',skiprows=10)
+
+        a_file = open(nameId+'_micro.vtk')
+        for position, line in enumerate(a_file):
+            if position==4:
+                ss=np.int32(line.split()[1:])
+            if position==6:
+                dim=np.float64(line.split()[1])
+                break
+
+
+        uni_g=np.unique(micro.flatten())
+
+        im=np.moveaxis(micro,0,-1)
+
+        micro2=np.zeros(np.shape(im))
+
+        k=1
+        for ig in uni_g:
+            id=np.where(im==ig)
+            micro2[id]=k
+            k=k+1
+
+
+        new_mi=np.transpose(micro2).flatten()
+
+        tesr_out=open(nameId+'_micro.tesr','w')
+        tesr_out.write('***tesr\n')
+        tesr_out.write(' **format\n')
+        tesr_out.write('   2.1\n')
+        tesr_out.write(' **general\n')
+
+        if m3d==0:
+            tesr_out.write('   2\n')
+            tesr_out.write('   '+str(ss[0])+' '+str(ss[1])+'\n')
+            tesr_out.write('   '+str(dim)+' '+str(dim)+'\n')
+        else:
+            tesr_out.write('   3\n')
+            tesr_out.write('   '+str(ss[0])+' '+str(ss[1])+' '+str(ss[2])+'\n')
+            tesr_out.write('   '+str(dim)+' '+str(dim)+' '+str(dim)+'\n')
+
+        tesr_out.write(' **cell\n')
+        tesr_out.write('   '+str(len(uni_g))+'\n')
+        tesr_out.write('  *id\n')
+        tesr_out.write('  ')
+        for ig in range(len(uni_g)):
+            tesr_out.write(' '+str(int(ig+1)))
+        tesr_out.write('\n')
+
+        tesr_out.write(' **data\n')
+        tesr_out.write('   ascii\n')
+        for i in range(len(new_mi)):
+            tesr_out.write(str(int(new_mi[i])))
+            if np.mod(i+1,ss[0])==0:
+                tesr_out.write('\n')
+            else:
+                tesr_out.write(' ')
 
-# ----------------------------------------------------
+
+        tesr_out.write('\n')
+        tesr_out.write('***end')
+
+        tesr_out.close()
 
 
 def save(self, path):
     """
     Save xarray craft data using pickle
 
     :param path: path to save pickle file
```

## Comparing `xarrayaita-0.2.6.dist-info/LICENSE` & `xarrayaita-0.2.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `xarrayaita-0.2.6.dist-info/METADATA` & `xarrayaita-0.2.7.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: xarrayaita
-Version: 0.2.6
+Version: 0.2.7
 Summary: Tools to work on output from AITA
 Home-page: https://gricad-gitlab.univ-grenoble-alpes.fr/mecaiceige/tools/lib_python/xarray_aita
 Author: Thomas Chauve
 Author-email: thomas.chauve@univ-grenoble-alpes.fr
 License: GPL-3.0
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 License-File: LICENSE
 Requires-Dist: xarray
@@ -29,8 +28,7 @@
 Requires-Dist: jupyterlab
 Requires-Dist: xarrayuvecs
 Provides-Extra: docs
 Requires-Dist: sphinx ; extra == 'docs'
 Requires-Dist: sphinx-rtd-theme ; extra == 'docs'
 
 Tools to work on output from AITA
-
```

## Comparing `xarrayaita-0.2.6.dist-info/RECORD` & `xarrayaita-0.2.7.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 xarrayaita/__init__.py,sha256=yn2X2skf4ihNjaMVMh3Bdj606_xKP5Yzt7eRY5XNfNY,263
 xarrayaita/aita.py,sha256=brGzqVA5fufWG-tsLyIOdGunj1DdrTDhakZG-B73Cg8,1347
-xarrayaita/aita_export.py,sha256=H0eEgeIgNY-tZHJ_syo2xqX_6k-Jn0T3pYEaYSRbK9k,4898
+xarrayaita/aita_export.py,sha256=xtAn2WE3dpw9BfLdYY0Ih6RjGD2ofmUdUlKmR5wlWs0,6863
 xarrayaita/aita_geom.py,sha256=olZffQqAaNH8Vhrb-aR_3EdCUXjkCEL3v7nkYPuLXD4,6679
 xarrayaita/aita_interactive_nb.py,sha256=roYRhc_PfrMSsoHeSd1xhZ30W99RYsURjTorZ2PXYds,16005
 xarrayaita/aita_plot.py,sha256=sitVEzjxFNgchlM93RckdWPNQT-nikDENv07nyKrEcA,975
 xarrayaita/aita_processing.py,sha256=LyrSR0tsTZ7Mj6n5hutEeXjFNpmeh5XDcyljZr7wC-w,12164
 xarrayaita/loadData_aita.py,sha256=nspH4OIKTiU6dAvnh-rdpi60Cvw1ZyxYeIusxBOCVxw,6899
-xarrayaita-0.2.6.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-xarrayaita-0.2.6.dist-info/METADATA,sha256=I5f6o-89g5jpjvS_HYcesPoR43icYOUfWPbOvuOkxTA,1072
-xarrayaita-0.2.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-xarrayaita-0.2.6.dist-info/top_level.txt,sha256=Ohg9Yo4Ya3hbXoW4drW0ZIPQBb94aXXWy8SgHsfeFI4,11
-xarrayaita-0.2.6.dist-info/RECORD,,
+xarrayaita-0.2.7.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+xarrayaita-0.2.7.dist-info/METADATA,sha256=-B_dgKNdPW38yGIAN6sufRvtBxzm0RwQGtGaaAWGKSg,1053
+xarrayaita-0.2.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+xarrayaita-0.2.7.dist-info/top_level.txt,sha256=Ohg9Yo4Ya3hbXoW4drW0ZIPQBb94aXXWy8SgHsfeFI4,11
+xarrayaita-0.2.7.dist-info/RECORD,,
```

