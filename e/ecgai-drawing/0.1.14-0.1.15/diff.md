# Comparing `tmp/ecgai_drawing-0.1.14.tar.gz` & `tmp/ecgai_drawing-0.1.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecgai_drawing-0.1.14.tar", max compression
+gzip compressed data, was "ecgai_drawing-0.1.15.tar", max compression
```

## Comparing `ecgai_drawing-0.1.14.tar` & `ecgai_drawing-0.1.15.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1010 2023-05-22 20:24:04.828234 ecgai_drawing-0.1.14/pyproject.toml
--rw-r--r--   0        0        0       78 2023-05-22 20:24:04.832234 ecgai_drawing-0.1.14/src/ecgai_drawing/__init__.py
--rw-r--r--   0        0        0     5709 2023-05-22 20:24:04.832234 ecgai_drawing-0.1.14/src/ecgai_drawing/create_ecg_plot.py
--rw-r--r--   0        0        0     5993 2023-05-22 20:24:04.832234 ecgai_drawing-0.1.14/src/ecgai_drawing/ecg_grid_plotter.py
--rw-r--r--   0        0        0      988 2023-05-22 20:24:04.832234 ecgai_drawing-0.1.14/src/ecgai_drawing/ecg_plot_image.py
--rw-r--r--   0        0        0    13186 2023-05-22 20:24:04.832234 ecgai_drawing-0.1.14/src/ecgai_drawing/ecg_plotter.py
--rw-r--r--   0        0        0        0 2023-05-22 20:24:04.832234 ecgai_drawing-0.1.14/src/ecgai_drawing/enums/__init__.py
--rw-r--r--   0        0        0      178 2023-05-22 20:24:04.832234 ecgai_drawing-0.1.14/src/ecgai_drawing/enums/artifact.py
--rw-r--r--   0        0        0      481 2023-05-22 20:24:04.832234 ecgai_drawing-0.1.14/src/ecgai_drawing/enums/color_style.py
--rw-r--r--   0        0        0      563 2023-05-22 20:24:04.832234 ecgai_drawing-0.1.14/src/ecgai_drawing/enums/ecg_lead_name.py
--rw-r--r--   0        0        0      676 2023-05-22 20:24:04.832234 ecgai_drawing-0.1.14/src/ecgai_drawing/enums/enum_ordered_base.py
--rw-r--r--   0        0        0      105 2023-05-22 20:24:04.832234 ecgai_drawing-0.1.14/src/ecgai_drawing/enums/show_grid.py
--rw-r--r--   0        0        0  1010336 2023-05-22 20:24:04.836234 ecgai_drawing-0.1.14/src/ecgai_drawing/grid_images/bw_six_x_two.png
--rw-r--r--   0        0        0   862301 2023-05-22 20:24:04.836234 ecgai_drawing-0.1.14/src/ecgai_drawing/grid_images/colour_six_x_two.png
--rw-r--r--   0        0        0    11934 2023-05-22 20:24:04.836234 ecgai_drawing-0.1.14/src/ecgai_drawing/images.py
--rw-r--r--   0        0        0        0 2023-05-22 20:24:04.836234 ecgai_drawing-0.1.14/src/ecgai_drawing/models/__init__.py
--rw-r--r--   0        0        0      812 2023-05-22 20:24:04.836234 ecgai_drawing-0.1.14/src/ecgai_drawing/models/ecg_lead.py
--rw-r--r--   0        0        0      647 2023-05-22 20:24:04.836234 ecgai_drawing-0.1.14/src/ecgai_drawing/models/ecg_leads.py
--rw-r--r--   0        0        0      851 2023-05-22 20:24:04.836234 ecgai_drawing-0.1.14/src/ecgai_drawing/models/model_base.py
--rw-r--r--   0        0        0      677 1970-01-01 00:00:00.000000 ecgai_drawing-0.1.14/PKG-INFO
+-rw-r--r--   0        0        0     1010 2023-05-23 13:32:16.646997 ecgai_drawing-0.1.15/pyproject.toml
+-rw-r--r--   0        0        0       78 2023-05-23 13:32:16.646997 ecgai_drawing-0.1.15/src/ecgai_drawing/__init__.py
+-rw-r--r--   0        0        0     5709 2023-05-23 13:32:16.646997 ecgai_drawing-0.1.15/src/ecgai_drawing/create_ecg_plot.py
+-rw-r--r--   0        0        0     5993 2023-05-23 13:32:16.646997 ecgai_drawing-0.1.15/src/ecgai_drawing/ecg_grid_plotter.py
+-rw-r--r--   0        0        0      988 2023-05-23 13:32:16.646997 ecgai_drawing-0.1.15/src/ecgai_drawing/ecg_plot_image.py
+-rw-r--r--   0        0        0    13186 2023-05-23 13:32:16.646997 ecgai_drawing-0.1.15/src/ecgai_drawing/ecg_plotter.py
+-rw-r--r--   0        0        0        0 2023-05-23 13:32:16.646997 ecgai_drawing-0.1.15/src/ecgai_drawing/enums/__init__.py
+-rw-r--r--   0        0        0      178 2023-05-23 13:32:16.646997 ecgai_drawing-0.1.15/src/ecgai_drawing/enums/artifact.py
+-rw-r--r--   0        0        0      481 2023-05-23 13:32:16.646997 ecgai_drawing-0.1.15/src/ecgai_drawing/enums/color_style.py
+-rw-r--r--   0        0        0      563 2023-05-23 13:32:16.646997 ecgai_drawing-0.1.15/src/ecgai_drawing/enums/ecg_lead_name.py
+-rw-r--r--   0        0        0      676 2023-05-23 13:32:16.646997 ecgai_drawing-0.1.15/src/ecgai_drawing/enums/enum_ordered_base.py
+-rw-r--r--   0        0        0      105 2023-05-23 13:32:16.646997 ecgai_drawing-0.1.15/src/ecgai_drawing/enums/show_grid.py
+-rw-r--r--   0        0        0  1010336 2023-05-23 13:32:16.650997 ecgai_drawing-0.1.15/src/ecgai_drawing/grid_images/bw_six_x_two.png
+-rw-r--r--   0        0        0   862301 2023-05-23 13:32:16.654996 ecgai_drawing-0.1.15/src/ecgai_drawing/grid_images/colour_six_x_two.png
+-rw-r--r--   0        0        0    11934 2023-05-23 13:32:16.654996 ecgai_drawing-0.1.15/src/ecgai_drawing/images.py
+-rw-r--r--   0        0        0        0 2023-05-23 13:32:16.654996 ecgai_drawing-0.1.15/src/ecgai_drawing/models/__init__.py
+-rw-r--r--   0        0        0      812 2023-05-23 13:32:16.654996 ecgai_drawing-0.1.15/src/ecgai_drawing/models/ecg_lead.py
+-rw-r--r--   0        0        0      647 2023-05-23 13:32:16.654996 ecgai_drawing-0.1.15/src/ecgai_drawing/models/ecg_leads.py
+-rw-r--r--   0        0        0      851 2023-05-23 13:32:16.654996 ecgai_drawing-0.1.15/src/ecgai_drawing/models/model_base.py
+-rw-r--r--   0        0        0      677 1970-01-01 00:00:00.000000 ecgai_drawing-0.1.15/PKG-INFO
```

### Comparing `ecgai_drawing-0.1.14/pyproject.toml` & `ecgai_drawing-0.1.15/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "ecgai-drawing"
-version = "0.1.14"
+version = "0.1.15"
 description = ""
 authors = ["RobC <rob.clapham@gmail.com>"]
 
 [tool.poetry.dependencies]
 #TODO change poetry version to <4.0, currently required by scipy
 python = "^3.9,<3.12"
 numpy = "^1.23.2"
 aenum = "^3.1.11"
 pydantic = "^1.9.2"
 matplotlib = "^3.5.3"
-scikit-image = "^0.19.3"
+scikit-image = "^0.20.0"
 scipy = "^1.9.0"
 opencv-python = "^4.6.0"
 timer = "^0.2.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 pre-commit = "^2.20.0"
```

### Comparing `ecgai_drawing-0.1.14/src/ecgai_drawing/create_ecg_plot.py` & `ecgai_drawing-0.1.15/src/ecgai_drawing/create_ecg_plot.py`

 * *Files identical despite different names*

### Comparing `ecgai_drawing-0.1.14/src/ecgai_drawing/ecg_grid_plotter.py` & `ecgai_drawing-0.1.15/src/ecgai_drawing/ecg_grid_plotter.py`

 * *Files identical despite different names*

### Comparing `ecgai_drawing-0.1.14/src/ecgai_drawing/ecg_plot_image.py` & `ecgai_drawing-0.1.15/src/ecgai_drawing/ecg_plot_image.py`

 * *Files identical despite different names*

### Comparing `ecgai_drawing-0.1.14/src/ecgai_drawing/ecg_plotter.py` & `ecgai_drawing-0.1.15/src/ecgai_drawing/ecg_plotter.py`

 * *Files identical despite different names*

### Comparing `ecgai_drawing-0.1.14/src/ecgai_drawing/enums/ecg_lead_name.py` & `ecgai_drawing-0.1.15/src/ecgai_drawing/enums/ecg_lead_name.py`

 * *Files identical despite different names*

### Comparing `ecgai_drawing-0.1.14/src/ecgai_drawing/enums/enum_ordered_base.py` & `ecgai_drawing-0.1.15/src/ecgai_drawing/enums/enum_ordered_base.py`

 * *Files identical despite different names*

### Comparing `ecgai_drawing-0.1.14/src/ecgai_drawing/grid_images/bw_six_x_two.png` & `ecgai_drawing-0.1.15/src/ecgai_drawing/grid_images/bw_six_x_two.png`

 * *Files identical despite different names*

### Comparing `ecgai_drawing-0.1.14/src/ecgai_drawing/grid_images/colour_six_x_two.png` & `ecgai_drawing-0.1.15/src/ecgai_drawing/grid_images/colour_six_x_two.png`

 * *Files identical despite different names*

### Comparing `ecgai_drawing-0.1.14/src/ecgai_drawing/images.py` & `ecgai_drawing-0.1.15/src/ecgai_drawing/images.py`

 * *Files identical despite different names*

### Comparing `ecgai_drawing-0.1.14/src/ecgai_drawing/models/ecg_lead.py` & `ecgai_drawing-0.1.15/src/ecgai_drawing/models/ecg_lead.py`

 * *Files identical despite different names*

### Comparing `ecgai_drawing-0.1.14/src/ecgai_drawing/models/ecg_leads.py` & `ecgai_drawing-0.1.15/src/ecgai_drawing/models/ecg_leads.py`

 * *Files identical despite different names*

### Comparing `ecgai_drawing-0.1.14/src/ecgai_drawing/models/model_base.py` & `ecgai_drawing-0.1.15/src/ecgai_drawing/models/model_base.py`

 * *Files identical despite different names*

### Comparing `ecgai_drawing-0.1.14/PKG-INFO` & `ecgai_drawing-0.1.15/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: ecgai-drawing
-Version: 0.1.14
+Version: 0.1.15
 Summary: 
 Author: RobC
 Author-email: rob.clapham@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aenum (>=3.1.11,<4.0.0)
 Requires-Dist: matplotlib (>=3.5.3,<4.0.0)
 Requires-Dist: numpy (>=1.23.2,<2.0.0)
 Requires-Dist: opencv-python (>=4.6.0,<5.0.0)
 Requires-Dist: pydantic (>=1.9.2,<2.0.0)
-Requires-Dist: scikit-image (>=0.19.3,<0.20.0)
+Requires-Dist: scikit-image (>=0.20.0,<0.21.0)
 Requires-Dist: scipy (>=1.9.0,<2.0.0)
 Requires-Dist: timer (>=0.2.2,<0.3.0)
```

