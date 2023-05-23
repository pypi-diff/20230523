# Comparing `tmp/synth_mapping_helper-1.2.1.tar.gz` & `tmp/synth_mapping_helper-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synth_mapping_helper-1.2.1.tar", last modified: Mon Apr 24 21:32:41 2023, max compression
+gzip compressed data, was "synth_mapping_helper-1.2.2.tar", last modified: Tue May 23 20:11:02 2023, max compression
```

## Comparing `synth_mapping_helper-1.2.1.tar` & `synth_mapping_helper-1.2.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:32:41.060683 synth_mapping_helper-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-24 21:32:30.000000 synth_mapping_helper-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-24 21:32:30.000000 synth_mapping_helper-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-04-24 21:32:41.060683 synth_mapping_helper-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-04-24 21:32:30.000000 synth_mapping_helper-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-24 21:32:30.000000 synth_mapping_helper-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-24 21:32:41.060683 synth_mapping_helper-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-24 21:32:30.000000 synth_mapping_helper-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:32:41.056683 synth_mapping_helper-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:32:41.060683 synth_mapping_helper-1.2.1/src/synth_mapping_helper/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-24 21:32:30.000000 synth_mapping_helper-1.2.1/src/synth_mapping_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27126 2023-04-24 21:32:30.000000 synth_mapping_helper-1.2.1/src/synth_mapping_helper/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    27963 2023-04-24 21:32:30.000000 synth_mapping_helper-1.2.1/src/synth_mapping_helper/companion.py
--rw-r--r--   0 runner    (1001) docker     (123)    14572 2023-04-24 21:32:30.000000 synth_mapping_helper-1.2.1/src/synth_mapping_helper/finalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-04-24 21:32:30.000000 synth_mapping_helper-1.2.1/src/synth_mapping_helper/movement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-24 21:32:30.000000 synth_mapping_helper-1.2.1/src/synth_mapping_helper/pattern_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-04-24 21:32:30.000000 synth_mapping_helper-1.2.1/src/synth_mapping_helper/rails.py
--rw-r--r--   0 runner    (1001) docker     (123)    16429 2023-04-24 21:32:30.000000 synth_mapping_helper-1.2.1/src/synth_mapping_helper/synth_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-04-24 21:32:30.000000 synth_mapping_helper-1.2.1/src/synth_mapping_helper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:32:41.060683 synth_mapping_helper-1.2.1/src/synth_mapping_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-04-24 21:32:41.000000 synth_mapping_helper-1.2.1/src/synth_mapping_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-24 21:32:41.000000 synth_mapping_helper-1.2.1/src/synth_mapping_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 21:32:41.000000 synth_mapping_helper-1.2.1/src/synth_mapping_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-24 21:32:41.000000 synth_mapping_helper-1.2.1/src/synth_mapping_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-24 21:32:41.000000 synth_mapping_helper-1.2.1/src/synth_mapping_helper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:32:41.060683 synth_mapping_helper-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-24 21:32:30.000000 synth_mapping_helper-1.2.1/tests/test_synth_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:11:02.772779 synth_mapping_helper-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-23 20:10:50.000000 synth_mapping_helper-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-23 20:10:50.000000 synth_mapping_helper-1.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-05-23 20:11:02.772779 synth_mapping_helper-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-05-23 20:10:50.000000 synth_mapping_helper-1.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-23 20:10:50.000000 synth_mapping_helper-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-23 20:11:02.772779 synth_mapping_helper-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-23 20:10:50.000000 synth_mapping_helper-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:11:02.768779 synth_mapping_helper-1.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:11:02.768779 synth_mapping_helper-1.2.2/src/synth_mapping_helper/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-23 20:10:50.000000 synth_mapping_helper-1.2.2/src/synth_mapping_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27126 2023-05-23 20:10:50.000000 synth_mapping_helper-1.2.2/src/synth_mapping_helper/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28072 2023-05-23 20:10:50.000000 synth_mapping_helper-1.2.2/src/synth_mapping_helper/companion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14572 2023-05-23 20:10:50.000000 synth_mapping_helper-1.2.2/src/synth_mapping_helper/finalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-05-23 20:10:50.000000 synth_mapping_helper-1.2.2/src/synth_mapping_helper/movement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-23 20:10:50.000000 synth_mapping_helper-1.2.2/src/synth_mapping_helper/pattern_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-05-23 20:10:50.000000 synth_mapping_helper-1.2.2/src/synth_mapping_helper/rails.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16429 2023-05-23 20:10:50.000000 synth_mapping_helper-1.2.2/src/synth_mapping_helper/synth_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-23 20:10:50.000000 synth_mapping_helper-1.2.2/src/synth_mapping_helper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:11:02.768779 synth_mapping_helper-1.2.2/src/synth_mapping_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-05-23 20:11:02.000000 synth_mapping_helper-1.2.2/src/synth_mapping_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-23 20:11:02.000000 synth_mapping_helper-1.2.2/src/synth_mapping_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 20:11:02.000000 synth_mapping_helper-1.2.2/src/synth_mapping_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-23 20:11:02.000000 synth_mapping_helper-1.2.2/src/synth_mapping_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-23 20:11:02.000000 synth_mapping_helper-1.2.2/src/synth_mapping_helper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:11:02.772779 synth_mapping_helper-1.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-23 20:10:50.000000 synth_mapping_helper-1.2.2/tests/test_synth_format.py
```

### Comparing `synth_mapping_helper-1.2.1/LICENSE` & `synth_mapping_helper-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.2.1/PKG-INFO` & `synth_mapping_helper-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synth_mapping_helper
-Version: 1.2.1
+Version: 1.2.2
 Summary: Toolbox for manipulating the JSON-Format used by Synth Riders Beatmap Editor in the clipboard
 Home-page: https://github.com/adosikas/synth_mapping_helper
 Author: adosikas
 Author-email: 
 Project-URL: Documentation, https://github.com/adosikas/synth_mapping_helper
 Project-URL: Bug Reports, https://github.com/adosikas/synth_mapping_helper
 Project-URL: Source Code, https://github.com/adosikas/synth_mapping_helper
```

### Comparing `synth_mapping_helper-1.2.1/README.md` & `synth_mapping_helper-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.2.1/setup.py` & `synth_mapping_helper-1.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.2.1/src/synth_mapping_helper/cli.py` & `synth_mapping_helper-1.2.2/src/synth_mapping_helper/cli.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.2.1/src/synth_mapping_helper/companion.py` & `synth_mapping_helper-1.2.2/src/synth_mapping_helper/companion.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 DEFAULT_OUTPUT_FILE = Path("output.synth")  # inside working directory
 DEFAULT_BACKUP_DIR = Path("smh_backup")  # inside working directory
 
 DEFAULT_VELOCITY_WINDOW = utils.SecondFloat(0.5)  # half a second gap breaks up velocity / acceleration calculations
 DEFAULT_INTERPOLATION = 1/16
 DEFAULT_VEL_LIMIT = 100
-DEFAULT_ACC_LIMIT = 1000
+DEFAULT_ACC_LIMIT = 2000
 DEFAULT_HEATMAP_BIN_COUNT = 3
 DEFAULT_HEATMAP_NORM_POWER = 0.6
 
 DEFAULT_WINDOW_WIDTH = 1600
 DEFAULT_WINDOW_HEIGHT = 900
 DEFAULT_MENU_SIZE = 100
 
@@ -236,15 +236,15 @@
 def plot_notes(options, fig, infile: SynthFile, data: DataContainer, prepared_data, **kwargs):
     axs = fig.subplots(4, sharex=True)
     axs[-1].set_xlabel("beats")
     plot_bookmarks(infile.bookmarks, axs)
 
     ax_x, ax_y, ax_vel, ax_acc = axs
     ax_x.set_ylabel("X-Position (sq)")
-    ax_x.set_ylim((-8,8))
+    ax_x.set_ylim((8,-8))
     ax_x.set_yticks(range(-8,8+1), (str(t) if not t%2 else "" for t in range(-8,8+1)))
     ax_x.grid(True)
 
     ax_y.set_ylabel("Y-Position (sq)")
     ax_y.set_ylim((-6,6))
     ax_y.set_yticks(range(-6,6+1), (str(t) if not t%2 else "" for t in range(-6,6+1)))
     ax_y.grid(True)
@@ -360,14 +360,15 @@
             bins=[int(17 * options.heatmap_bin_count),int(13 * options.heatmap_bin_count)], range=[[-8,8],[-6,6]],
             cmap=("Reds", "Blues", "Greens", "Oranges")[t],
             density=False, norm=PowerNorm(options.heatmap_norm_power),
         )
         avg = np.nanmean(pos, axis=0)
         axs[t].plot(avg[0], avg[1], marker="x", color="white", markeredgecolor="black", markersize=10)
         axs[t].grid(True)
+        axs[t].text((-7,7,7,-7)[t], (-5,-5,5,5)[t], len(getattr(data, note_type)), ha="center", va="center")
 
 def show_warnings(options, fig, infile: SynthFile, data: DataContainer, prepared_data, platform: str):
     ax = fig.subplots(1)
     ax.set_axis_off()
     ax.table(loc="top", colWidths=(1/20, 19/20), cellLoc="left", rowLabels=["123 5/6"], cellText=[["note:left", "placeholder, ie extreme peak in acceleration"]])
 
 TABS = [
```

### Comparing `synth_mapping_helper-1.2.1/src/synth_mapping_helper/finalize.py` & `synth_mapping_helper-1.2.2/src/synth_mapping_helper/finalize.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.2.1/src/synth_mapping_helper/movement.py` & `synth_mapping_helper-1.2.2/src/synth_mapping_helper/movement.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.2.1/src/synth_mapping_helper/pattern_generation.py` & `synth_mapping_helper-1.2.2/src/synth_mapping_helper/pattern_generation.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.2.1/src/synth_mapping_helper/rails.py` & `synth_mapping_helper-1.2.2/src/synth_mapping_helper/rails.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.2.1/src/synth_mapping_helper/synth_format.py` & `synth_mapping_helper-1.2.2/src/synth_mapping_helper/synth_format.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.2.1/src/synth_mapping_helper/utils.py` & `synth_mapping_helper-1.2.2/src/synth_mapping_helper/utils.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.2.1/src/synth_mapping_helper.egg-info/PKG-INFO` & `synth_mapping_helper-1.2.2/src/synth_mapping_helper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synth-mapping-helper
-Version: 1.2.1
+Version: 1.2.2
 Summary: Toolbox for manipulating the JSON-Format used by Synth Riders Beatmap Editor in the clipboard
 Home-page: https://github.com/adosikas/synth_mapping_helper
 Author: adosikas
 Author-email: 
 Project-URL: Documentation, https://github.com/adosikas/synth_mapping_helper
 Project-URL: Bug Reports, https://github.com/adosikas/synth_mapping_helper
 Project-URL: Source Code, https://github.com/adosikas/synth_mapping_helper
```

### Comparing `synth_mapping_helper-1.2.1/src/synth_mapping_helper.egg-info/SOURCES.txt` & `synth_mapping_helper-1.2.2/src/synth_mapping_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

