# Comparing `tmp/phic-2.0.8-py3-none-any.whl.zip` & `tmp/phic-2.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 22907 bytes, number of entries: 8
+Zip file size: 22897 bytes, number of entries: 8
 -rw-r--r--  2.0 unx        1 b- defN 21-Oct-18 05:22 src/__init__.py
--rw-rw-r--  2.0 unx    44842 b- defN 22-Aug-25 01:36 src/phic2.py
--rw-r--r--  2.0 unx    35149 b- defN 22-Aug-25 01:41 phic-2.0.8.dist-info/LICENSE
--rw-rw-r--  2.0 unx    11388 b- defN 22-Aug-25 01:41 phic-2.0.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Aug-25 01:41 phic-2.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       39 b- defN 22-Aug-25 01:41 phic-2.0.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        4 b- defN 22-Aug-25 01:41 phic-2.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      603 b- defN 22-Aug-25 01:41 phic-2.0.8.dist-info/RECORD
-8 files, 92118 bytes uncompressed, 21861 bytes compressed:  76.3%
+-rw-rw-r--  2.0 unx    44730 b- defN 22-Sep-07 06:11 src/phic2.py
+-rw-r--r--  2.0 unx    35149 b- defN 22-Sep-07 06:16 phic-2.0.9.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    11388 b- defN 22-Sep-07 06:16 phic-2.0.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 22-Sep-07 06:16 phic-2.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       39 b- defN 22-Sep-07 06:16 phic-2.0.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        4 b- defN 22-Sep-07 06:16 phic-2.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      603 b- defN 22-Sep-07 06:16 phic-2.0.9.dist-info/RECORD
+8 files, 92006 bytes uncompressed, 21851 bytes compressed:  76.3%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: src/__init__.py
 Comment: 
 
 Filename: src/phic2.py
 Comment: 
 
-Filename: phic-2.0.8.dist-info/LICENSE
+Filename: phic-2.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: phic-2.0.8.dist-info/METADATA
+Filename: phic-2.0.9.dist-info/METADATA
 Comment: 
 
-Filename: phic-2.0.8.dist-info/WHEEL
+Filename: phic-2.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: phic-2.0.8.dist-info/entry_points.txt
+Filename: phic-2.0.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: phic-2.0.8.dist-info/top_level.txt
+Filename: phic-2.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: phic-2.0.8.dist-info/RECORD
+Filename: phic-2.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## src/phic2.py

```diff
@@ -781,19 +781,17 @@
     ax.spines["top"].set_color("none")
     ax.spines["bottom"].set_color("none")
     plt.tick_params(labelbottom=0, bottom=0, labelleft=1)
 
     plt.savefig(FILE_FIG_SPECTRUM_ABS)
     plt.close()
     # ----------------------------------------------------------------------------------------------
-    np.savetxt(FILE_OUT_SPECTRUM_STORAGE, np.flipud(
-        J_storage[START:END, :]), fmt="%e")
-    np.savetxt(FILE_OUT_SPECTRUM_LOSS, np.flipud(
-        J_loss[START:END, :]), fmt="%e")
-    np.savetxt(FILE_OUT_SPECTRUM_ABS, np.flipud(J_abs[START:END, :]), fmt="%e")
+    np.savetxt(FILE_OUT_SPECTRUM_STORAGE, J_storage[START:END, :]), fmt="%e")
+    np.savetxt(FILE_OUT_SPECTRUM_LOSS, J_loss[START:END, :], fmt="%e")
+    np.savetxt(FILE_OUT_SPECTRUM_ABS, J_abs[START:END, :], fmt="%e")
 # --------------------------------------------------------------------------------------------------
 
 
 @cli.command()
 @click.option("--name", "NAME", required=True,
               help="Target directory name")
 @click.option("--upper", "UPPER", type=int, default=1,
@@ -929,19 +927,17 @@
     ax.spines["top"].set_color("none")
     ax.spines["bottom"].set_color("none")
     plt.tick_params(labelbottom=0, bottom=0, labelleft=1)
 
     plt.savefig(FILE_FIG_SPECTRUM_ABS)
     plt.close()
     # ----------------------------------------------------------------------------------------------
-    np.savetxt(FILE_OUT_SPECTRUM_STORAGE, np.flipud(
-        G_storage[START:END, :]), fmt="%e")
-    np.savetxt(FILE_OUT_SPECTRUM_LOSS, np.flipud(
-        G_loss[START:END, :]), fmt="%e")
-    np.savetxt(FILE_OUT_SPECTRUM_ABS, np.flipud(G_abs[START:END, :]), fmt="%e")
+    np.savetxt(FILE_OUT_SPECTRUM_STORAGE, G_storage[START:END, :], fmt="%e")
+    np.savetxt(FILE_OUT_SPECTRUM_LOSS, G_loss[START:END, :], fmt="%e")
+    np.savetxt(FILE_OUT_SPECTRUM_ABS, G_abs[START:END, :], fmt="%e")
 # --------------------------------------------------------------------------------------------------
 
 
 @cli.command()
 @click.option("--name", "NAME", required=True,
               help="Target directory name")
 @click.option("--upper", "UPPER", type=int, default=1,
@@ -1000,13 +996,13 @@
     ax.spines["top"].set_color("none")
     ax.spines["bottom"].set_color("none")
     plt.tick_params(labelbottom=0, bottom=0, labelleft=1)
 
     plt.savefig(FILE_FIG_SPECTRUM)
     plt.close()
     # ----------------------------------------------------------------------------------------------
-    np.savetxt(FILE_OUT_SPECTRUM, np.flipud(tan[START:END, :]), fmt="%e")
+    np.savetxt(FILE_OUT_SPECTRUM, tan[START:END, :], fmt="%e")
 # --------------------------------------------------------------------------------------------------
 
 
 if __name__ == '__main__':
     cli()
```

## Comparing `phic-2.0.8.dist-info/LICENSE` & `phic-2.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `phic-2.0.8.dist-info/METADATA` & `phic-2.0.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phic
-Version: 2.0.8
+Version: 2.0.9
 Summary: Polymer dynamics deciphered from Hi-C data
 Home-page: https://github.com/soyashinkai/PHi-C2
 Author: Soya SHINKAI
 Author-email: soya.shinkai@riken.jp
 License: GPL-3.0
 Keywords: biophysics,bioinformatics,genomics,Hi-C,polymer modeling,polymer dynamics,rheology
 Classifier: Programming Language :: Python :: 3
```

