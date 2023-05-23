# Comparing `tmp/PyComplexHeatmap-1.4.4.tar.gz` & `tmp/PyComplexHeatmap-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyComplexHeatmap-1.4.4.tar", last modified: Tue May 16 22:08:13 2023, max compression
+gzip compressed data, was "PyComplexHeatmap-1.5.0.tar", last modified: Tue May 23 20:51:27 2023, max compression
```

## Comparing `PyComplexHeatmap-1.4.4.tar` & `PyComplexHeatmap-1.5.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 wding      (503) staff       (20)        0 2023-05-16 22:08:13.526768 PyComplexHeatmap-1.4.4/
--rw-r--r--   0 wding      (503) staff       (20)     1067 2023-05-16 21:30:04.000000 PyComplexHeatmap-1.4.4/LICENSE
--rw-r--r--   0 wding      (503) staff       (20)      105 2023-05-16 21:30:04.000000 PyComplexHeatmap-1.4.4/MANIFEST.in
--rw-r--r--   0 wding      (503) staff       (20)    11704 2023-05-16 22:08:13.526173 PyComplexHeatmap-1.4.4/PKG-INFO
-drwxr-xr-x   0 wding      (503) staff       (20)        0 2023-05-16 22:08:13.523139 PyComplexHeatmap-1.4.4/PyComplexHeatmap/
--rw-r--r--   0 wding      (503) staff       (20)      387 2023-05-16 22:07:22.000000 PyComplexHeatmap-1.4.4/PyComplexHeatmap/__init__.py
--rw-r--r--   0 wding      (503) staff       (20)    65962 2023-05-16 21:46:47.000000 PyComplexHeatmap-1.4.4/PyComplexHeatmap/annotations.py
--rw-r--r--   0 wding      (503) staff       (20)    75705 2023-05-16 21:58:54.000000 PyComplexHeatmap-1.4.4/PyComplexHeatmap/clustermap.py
--rw-r--r--   0 wding      (503) staff       (20)     5430 2023-05-15 19:27:29.000000 PyComplexHeatmap-1.4.4/PyComplexHeatmap/colors.py
--rw-r--r--   0 wding      (503) staff       (20)    21247 2023-05-08 23:39:01.000000 PyComplexHeatmap-1.4.4/PyComplexHeatmap/dotHeatmap.py
--rw-r--r--   0 wding      (503) staff       (20)     6766 2023-05-08 23:39:01.000000 PyComplexHeatmap-1.4.4/PyComplexHeatmap/example.py
--rw-r--r--   0 wding      (503) staff       (20)    17814 2023-05-08 23:39:01.000000 PyComplexHeatmap-1.4.4/PyComplexHeatmap/oncoPrint.py
--rw-r--r--   0 wding      (503) staff       (20)     6753 2023-05-08 23:39:01.000000 PyComplexHeatmap-1.4.4/PyComplexHeatmap/tools.py
--rw-r--r--   0 wding      (503) staff       (20)    27686 2023-05-16 18:20:55.000000 PyComplexHeatmap-1.4.4/PyComplexHeatmap/utils.py
-drwxr-xr-x   0 wding      (503) staff       (20)        0 2023-05-16 22:08:13.525571 PyComplexHeatmap-1.4.4/PyComplexHeatmap.egg-info/
--rw-r--r--   0 wding      (503) staff       (20)    11704 2023-05-16 22:08:13.000000 PyComplexHeatmap-1.4.4/PyComplexHeatmap.egg-info/PKG-INFO
--rw-r--r--   0 wding      (503) staff       (20)      473 2023-05-16 22:08:13.000000 PyComplexHeatmap-1.4.4/PyComplexHeatmap.egg-info/SOURCES.txt
--rw-r--r--   0 wding      (503) staff       (20)        1 2023-05-16 22:08:13.000000 PyComplexHeatmap-1.4.4/PyComplexHeatmap.egg-info/dependency_links.txt
--rw-r--r--   0 wding      (503) staff       (20)       17 2023-05-16 22:08:13.000000 PyComplexHeatmap-1.4.4/PyComplexHeatmap.egg-info/top_level.txt
--rw-r--r--   0 wding      (503) staff       (20)    11095 2023-05-16 21:30:04.000000 PyComplexHeatmap-1.4.4/README.md
--rw-r--r--   0 wding      (503) staff       (20)      672 2023-05-16 22:07:30.000000 PyComplexHeatmap-1.4.4/pyproject.toml
--rw-r--r--   0 wding      (503) staff       (20)       38 2023-05-16 22:08:13.527031 PyComplexHeatmap-1.4.4/setup.cfg
--rw-r--r--   0 wding      (503) staff       (20)     1044 2023-05-16 22:07:36.000000 PyComplexHeatmap-1.4.4/setup.py
+drwxr-xr-x   0 wding      (503) staff       (20)        0 2023-05-23 20:51:27.917675 PyComplexHeatmap-1.5.0/
+-rw-r--r--   0 wding      (503) staff       (20)     1067 2023-05-16 21:30:04.000000 PyComplexHeatmap-1.5.0/LICENSE
+-rw-r--r--   0 wding      (503) staff       (20)      105 2023-05-16 21:30:04.000000 PyComplexHeatmap-1.5.0/MANIFEST.in
+-rw-r--r--   0 wding      (503) staff       (20)    11704 2023-05-23 20:51:27.917290 PyComplexHeatmap-1.5.0/PKG-INFO
+drwxr-xr-x   0 wding      (503) staff       (20)        0 2023-05-23 20:51:27.914965 PyComplexHeatmap-1.5.0/PyComplexHeatmap/
+-rw-r--r--   0 wding      (503) staff       (20)      387 2023-05-23 20:49:55.000000 PyComplexHeatmap-1.5.0/PyComplexHeatmap/__init__.py
+-rw-r--r--   0 wding      (503) staff       (20)    66115 2023-05-16 22:49:47.000000 PyComplexHeatmap-1.5.0/PyComplexHeatmap/annotations.py
+-rw-r--r--   0 wding      (503) staff       (20)    75856 2023-05-23 20:30:33.000000 PyComplexHeatmap-1.5.0/PyComplexHeatmap/clustermap.py
+-rw-r--r--   0 wding      (503) staff       (20)     5430 2023-05-15 19:27:29.000000 PyComplexHeatmap-1.5.0/PyComplexHeatmap/colors.py
+-rw-r--r--   0 wding      (503) staff       (20)    21247 2023-05-08 23:39:01.000000 PyComplexHeatmap-1.5.0/PyComplexHeatmap/dotHeatmap.py
+-rw-r--r--   0 wding      (503) staff       (20)     6766 2023-05-08 23:39:01.000000 PyComplexHeatmap-1.5.0/PyComplexHeatmap/example.py
+-rw-r--r--   0 wding      (503) staff       (20)    17848 2023-05-17 00:12:40.000000 PyComplexHeatmap-1.5.0/PyComplexHeatmap/oncoPrint.py
+-rw-r--r--   0 wding      (503) staff       (20)     6753 2023-05-08 23:39:01.000000 PyComplexHeatmap-1.5.0/PyComplexHeatmap/tools.py
+-rw-r--r--   0 wding      (503) staff       (20)    28823 2023-05-23 20:47:26.000000 PyComplexHeatmap-1.5.0/PyComplexHeatmap/utils.py
+drwxr-xr-x   0 wding      (503) staff       (20)        0 2023-05-23 20:51:27.916757 PyComplexHeatmap-1.5.0/PyComplexHeatmap.egg-info/
+-rw-r--r--   0 wding      (503) staff       (20)    11704 2023-05-23 20:51:27.000000 PyComplexHeatmap-1.5.0/PyComplexHeatmap.egg-info/PKG-INFO
+-rw-r--r--   0 wding      (503) staff       (20)      473 2023-05-23 20:51:27.000000 PyComplexHeatmap-1.5.0/PyComplexHeatmap.egg-info/SOURCES.txt
+-rw-r--r--   0 wding      (503) staff       (20)        1 2023-05-23 20:51:27.000000 PyComplexHeatmap-1.5.0/PyComplexHeatmap.egg-info/dependency_links.txt
+-rw-r--r--   0 wding      (503) staff       (20)       17 2023-05-23 20:51:27.000000 PyComplexHeatmap-1.5.0/PyComplexHeatmap.egg-info/top_level.txt
+-rw-r--r--   0 wding      (503) staff       (20)    11095 2023-05-16 21:30:04.000000 PyComplexHeatmap-1.5.0/README.md
+-rw-r--r--   0 wding      (503) staff       (20)      672 2023-05-23 20:50:06.000000 PyComplexHeatmap-1.5.0/pyproject.toml
+-rw-r--r--   0 wding      (503) staff       (20)       38 2023-05-23 20:51:27.917773 PyComplexHeatmap-1.5.0/setup.cfg
+-rw-r--r--   0 wding      (503) staff       (20)     1044 2023-05-23 20:50:15.000000 PyComplexHeatmap-1.5.0/setup.py
```

### Comparing `PyComplexHeatmap-1.4.4/LICENSE` & `PyComplexHeatmap-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.4.4/PKG-INFO` & `PyComplexHeatmap-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyComplexHeatmap
-Version: 1.4.4
+Version: 1.5.0
 Summary: A python package to plot complex heatmap
 Home-page: https://github.com/DingWB/PyComplexHeatmap
 Author: Wubin Ding
 Author-email: Wubin Ding <ding.wu.bin.gm@gmail.com>
 Project-URL: Homepage, https://github.com/DingWB/PyComplexHeatmap
 Project-URL: Bug Tracker, https://github.com/DingWB/PyComplexHeatmap/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PyComplexHeatmap-1.4.4/PyComplexHeatmap/annotations.py` & `PyComplexHeatmap-1.5.0/PyComplexHeatmap/annotations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1220,15 +1220,18 @@
                 vmax = np.nanmax(array)
                 vmin = np.nanmin(array)
                 legend_kws.setdefault('vmin', round(vmin, 2))
                 legend_kws.setdefault('vmax', round(vmax, 2))
                 self.legend_list.append([annotation.cmap, annotation.label, legend_kws, 4,'cmap'])
         if len(self.legend_list) > 1:
             self.legend_list = sorted(self.legend_list, key=lambda x: x[3])
-        self.label_max_width = max([ann.get_max_label_width() for ann in self.annotations])
+        if self.label_side == 'right':
+            self.label_max_width = max([ann.get_max_label_width() for ann in self.annotations])
+        else:
+            self.label_max_width = max([ann.get_ticklabel_width() for ann in self.annotations])
         # self.label_max_height = max([ann.ax.yaxis.label.get_window_extent().height for ann in self.annotations])
 
     def plot_annotations(self, ax=None, subplot_spec=None, idxs=None,
                          wspace=None, hspace=None):
         """
         Plot annotations
```

### Comparing `PyComplexHeatmap-1.4.4/PyComplexHeatmap/clustermap.py` & `PyComplexHeatmap-1.5.0/PyComplexHeatmap/clustermap.py`

 * *Files 0% similar despite different names*

```diff
@@ -789,16 +789,16 @@
     plot_legend :bool
         True or False, whether to plot legend, if False, legends can be plot with
         ClusterMapPlotter.plot_legends()
     legend_anchor :str
         ax_heatmap or ax, the ax to which legend anchor.
     legend_gap :float
         the columns gap between different legends.
-    legend_width: float
-        width of the legend, default is 4.5[mm]
+    legend_width: float [mm]
+        width of the legend, default is None (infer from data automatically)
     legend_hpad: float
         Horizonal space between the heatmap and legend, default is 2 [mm].
     legend_vpad: float
         Vertical space between the top of legend_anchor and legend, default is 5 [mm].
     legend_side :str
         right of left.
     cmap :str
@@ -826,15 +826,15 @@
                  row_cluster=True, col_cluster=True, row_cluster_method='average', row_cluster_metric='correlation',
                  col_cluster_method='average', col_cluster_metric='correlation',
                  show_rownames=False, show_colnames=False, row_names_side='right', col_names_side='bottom',
                  row_dendrogram=False, col_dendrogram=False, row_dendrogram_size=10, col_dendrogram_size=10,
                  row_split=None, col_split=None, dendrogram_kws=None, tree_kws=None,
                  row_split_order=None, col_split_order=None, row_split_gap=0.5, col_split_gap=0.2, mask=None,
                  subplot_gap=1, legend=True, legend_kws=None, plot=True, plot_legend=True,
-                 legend_anchor='auto', legend_gap=7, legend_width=4.5, legend_hpad=2, legend_vpad=5,
+                 legend_anchor='auto', legend_gap=7, legend_width=None, legend_hpad=1, legend_vpad=5,
                  legend_side='right', cmap='jet', label=None, xticklabels_kws=None, yticklabels_kws=None,
                  rasterized=False, legend_delta_x=None, verbose=1, **kwargs):
         self.kwargs = kwargs if not kwargs is None else {}
         self.data2d = self.format_data(data, mask, z_score, standard_scale)
         self.verbose=verbose
         self._define_kws(xticklabels_kws, yticklabels_kws)
         self.top_annotation = top_annotation
@@ -1336,23 +1336,25 @@
         # self.ax_heatmap.tick_params(axis='both', which='both',
         #                             left=False, right=False, top=False, bottom=False)
         self.yticklabels = []
         self.xticklabels = []
         if (self.show_rownames and self.left_annotation is None and not self.row_dendrogram) \
                 and ((not self.right_annotation is None) or (
                 self.right_annotation is None and self.row_names_side == 'left')):  # tick left
+            self.row_names_side='left'
             self.yticklabels_kws.setdefault('labelrotation', 0)
             for i in range(self.heatmap_axes.shape[0]):
                 self.heatmap_axes[i, 0].yaxis.set_visible(True)
                 self.heatmap_axes[i, 0].tick_params(axis='y', which='both', left=False, labelleft=True)
                 self.heatmap_axes[i, 0].yaxis.set_tick_params(**self.yticklabels_kws)  # **self.ticklabels_kws
                 plt.setp(self.heatmap_axes[i, 0].get_yticklabels(), rotation_mode='anchor',
                          ha='right', va='center')
                 self.yticklabels.extend(self.heatmap_axes[i, 0].get_yticklabels())
         elif self.show_rownames and self.right_annotation is None:  # tick right
+            self.row_names_side = 'right'
             self.yticklabels_kws.setdefault('labelrotation', 0)
             for i in range(self.heatmap_axes.shape[0]):
                 self.heatmap_axes[i, -1].yaxis.tick_right()  # set_ticks_position('right')
                 self.heatmap_axes[i, -1].yaxis.set_visible(True)
                 self.heatmap_axes[i, -1].tick_params(axis='y', which='both', right=False, labelright=True)
                 self.heatmap_axes[i, -1].yaxis.set_tick_params(**self.yticklabels_kws)
                 plt.setp(self.heatmap_axes[i, -1].get_yticklabels(), rotation_mode='anchor',
@@ -1402,19 +1404,19 @@
         if self.legend:
             vmax = self.kwargs.get('vmax', np.nanmax(self.data2d[self.data2d != np.inf]))
             vmin = self.kwargs.get('vmin', np.nanmin(self.data2d[self.data2d != -np.inf]))
             self.legend_kws.setdefault('vmin', round(vmin, 2))
             self.legend_kws.setdefault('vmax', round(vmax, 2))
             self.legend_list.append([self.cmap, self.label, self.legend_kws, 4,'cmap'])
             heatmap_label_max_width = max([label.get_window_extent().width for label in self.yticklabels]) if len(
-                self.yticklabels) > 0 else 0
+                self.yticklabels) > 0 and self.row_names_side=='right' else 0
             # heatmap_label_max_height = max([label.get_window_extent().height for label in self.yticklabels]) if len(
             #     self.yticklabels) > 0 else 0
             if heatmap_label_max_width >= self.label_max_width or self.legend_anchor == 'ax_heatmap':
-                self.label_max_width = heatmap_label_max_width * 1.1
+                self.label_max_width = heatmap_label_max_width #* 1.1
             if len(self.legend_list) > 1:
                 self.legend_list = sorted(self.legend_list, key=lambda x: x[3])
 
     def plot_legends(self, ax=None):
         if self.verbose >= 1:
             print("Plotting legends..")
         if len(self.legend_list) > 0:
@@ -1501,15 +1503,15 @@
         matplotlib.figure.Figure.set_figwidth(fig, width)  # convert mm to inches
 
     def post_processing(self):
         pass
 # =============================================================================
 def composite(cmlist=None, main=0, ax=None, axis=1, row_gap=15, col_gap=15,
               legend_side='right', legend_gap=5, legend_y=0.8, legend_hpad=None,
-              legend_width=4.5):
+              legend_width=None):
     """
     Assemble multiple ClusterMapPlotter objects vertically or horizontally together.
 
     Parameters
     ----------
     cmlist: list
         a list of ClusterMapPlotter (with plot=False).
```

### Comparing `PyComplexHeatmap-1.4.4/PyComplexHeatmap/colors.py` & `PyComplexHeatmap-1.5.0/PyComplexHeatmap/colors.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.4.4/PyComplexHeatmap/dotHeatmap.py` & `PyComplexHeatmap-1.5.0/PyComplexHeatmap/dotHeatmap.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.4.4/PyComplexHeatmap/example.py` & `PyComplexHeatmap-1.5.0/PyComplexHeatmap/example.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.4.4/PyComplexHeatmap/oncoPrint.py` & `PyComplexHeatmap-1.5.0/PyComplexHeatmap/oncoPrint.py`

 * *Files 1% similar despite different names*

```diff
@@ -347,17 +347,17 @@
                 # print(annotation.label_max_width,self.label_max_width)
                 if annotation.label_max_width > self.label_max_width:
                     self.label_max_width = annotation.label_max_width
         if self.legend:
             self.legend_list.append(
                 [self.color_dict, self.label, self.color_legend_kws, len(self.color_dict), 'color_dict'])
             heatmap_label_max_width = max([label.get_window_extent().width for label in self.yticklabels]) if len(
-                self.yticklabels) > 0 else 0
+                self.yticklabels) > 0 and self.row_names_side=='right' else 0
             if heatmap_label_max_width >= self.label_max_width or self.legend_anchor == 'ax_heatmap':
-                self.label_max_width = heatmap_label_max_width * 1.1
+                self.label_max_width = heatmap_label_max_width #* 1.1
             if len(self.legend_list) > 1:
                 self.legend_list = sorted(self.legend_list, key=lambda x: x[3])
 
     def post_processing(self):
         pass
 
 if __name__ == "__main__":
```

### Comparing `PyComplexHeatmap-1.4.4/PyComplexHeatmap/tools.py` & `PyComplexHeatmap-1.5.0/PyComplexHeatmap/tools.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.4.4/PyComplexHeatmap/utils.py` & `PyComplexHeatmap-1.5.0/PyComplexHeatmap/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         'font.family':['sans serif'], #'serif',
         # 'mathtext.fontset':'dejavuserif',
         'font.sans-serif':['Arial'],
         'pdf.fonttype':42,
 
         # Remove legend frame
         'legend.frameon': True,
+        'legend.fontsize': 10,
 
         # Savefig
         'figure.dpi': 100,
         'savefig.bbox': 'tight',
         'savefig.dpi':300,
         'savefig.pad_inches': 0.05
     }
@@ -545,16 +546,33 @@
             except:
                 pass
     ax.add_artist(Lgd)
     ax.grid(False)
     # print(availabel_height,L.get_window_extent().height)
     return Lgd
 # =============================================================================
+def cal_legend_width(legend_list):
+    lgd_w=4.5
+    legend_width=0
+    for lgd in legend_list:
+        obj, title, legend_kws, n, lgd_t = lgd
+        if lgd_t=='color_dict':
+            max_text_len=max(len(str(title)),max([len(str(k)) for k in obj]))
+            fontsize = legend_kws.get('fontsize',plt.rcParams['legend.fontsize'])
+            lgd_w=max_text_len * fontsize * 0.65 / 72 / mm2inch #point to inches to mm. in average, width = height * 0.6
+        elif lgd_t=="markers":
+            max_text_len = len(str(title))
+            fontsize = legend_kws.get('fontsize', plt.rcParams['legend.fontsize'])
+            lgd_w = max_text_len * fontsize * 0.65 / 72 / mm2inch
+        if legend_width < lgd_w:
+            legend_width=lgd_w
+    return legend_width
+
 def plot_legend_list(legend_list=None,ax=None,space=0,legend_side='right',
-                     y0=None,gap=2,delta_x=None,legend_width=4.5,legend_vpad=5,
+                     y0=None,gap=2,delta_x=None,legend_width=None,legend_vpad=5,
                      cmap_width=4.5):
     """
     Plot all lengends for a given legend_list.
 
     Parameters
     ----------
     legend_list : a list including [handles(dict) / cmap / markers dict, title, legend_kws, height, legend_type]
@@ -574,115 +592,113 @@
         print("No ax was provided, using plt.gca()")
         ax=plt.gca()
         ax.set_axis_off()
         left=ax.get_position().x0+ax.yaxis.labelpad*2/ax.figure.get_window_extent().width if delta_x is None else ax.get_position().x0+delta_x
     else:
         #labelpad: Spacing in points, pad is the fraction relative to x1.
         pad = (space+ax.yaxis.labelpad*1.2*ax.figure.dpi / 72) / ax.figure.get_window_extent().width if delta_x is None else delta_x #labelpad unit is points
-        # print(space,pad)
         left=ax.get_position().x1 + pad
-        # print(ax.get_position(),space,pad,left)
-    legend_width=legend_width*mm2inch*ax.figure.dpi / ax.figure.get_window_extent().width #mm to px
-    cmap_width = cmap_width * mm2inch * ax.figure.dpi / ax.figure.get_window_extent().width  # mm to px
+    if legend_width is None:
+        legend_width=cal_legend_width(legend_list) + 2.5 #base width for color rectangle is set to 2 mm
+    # print("Estimated legend width: ",legend_width)
+    legend_width=legend_width*mm2inch*ax.figure.dpi / ax.figure.get_window_extent().width #mm to px to fraction
+    cmap_width = cmap_width * mm2inch * ax.figure.dpi / ax.figure.get_window_extent().width  # mm to px to fraction
     if legend_side=='right':
         ax_legend=ax.figure.add_axes([left,ax.get_position().y0,legend_width,ax.get_position().height]) #left, bottom, width, height
-    # print(ax.get_position(),ax_legend.get_position())
     legend_axes=[ax_legend]
     cbars=[]
-    leg_pos = ax_legend.get_position()
+    leg_pos = ax_legend.get_position() #left bototm: x0,y0; top right: x1,y1
+
+    # y is the bottom position of the first legend (from top to the bottom)
     y = leg_pos.y1 - legend_vpad*mm2inch * ax.figure.dpi / ax.figure.get_window_extent().height if y0 is None else y0
-    max_width=0
-    h_gap=round(gap*mm2inch*ax.figure.dpi/ax.figure.get_window_extent().height,2) #2mm height gap between two legends
+    lgd_col_max_width=0 #the maximum width of all legends in one column
+    v_gap=round(gap*mm2inch*ax.figure.dpi/ax.figure.get_window_extent().height,2) #2mm vertically height gap between two legends
     i=0
     while i <= len(legend_list)-1:
-    # for i,legend in enumerate(legend_list):
         obj, title, legend_kws, n, lgd_t = legend_list[i]
-        ax1 = legend_axes[-1]
+        ax1 = legend_axes[-1] #ax for the legend on the right
         ax1.set_axis_off()
-        # print(i,legend_list[i])
         color_text=legend_kws.pop("color_text",True)
         if lgd_t=='cmap': #type(obj)==str: # a cmap, plot colorbar
-            f = (15) * mm2inch * ax.figure.dpi / ax.figure.get_window_extent().height  # 15 mm
+            f = 15 * mm2inch * ax.figure.dpi / ax.figure.get_window_extent().height  # 15 mm
             if y-f < 0: #add a new column of axes to plot legends
-                left_pos=ax1.get_position()
-                pad=(max_width + ax.yaxis.labelpad * 2) / ax.figure.get_window_extent().width
-                ax2=ax.figure.add_axes([left_pos.x1+pad, ax.get_position().y0, cmap_width, ax.get_position().height]) #left_pos.width
+                offset=(lgd_col_max_width + ax.yaxis.labelpad * 2) / ax.figure.get_window_extent().width
+                ax2=ax.figure.add_axes(rect=[ax1.get_position().x0+offset, ax.get_position().y0, cmap_width, ax.get_position().height]) #left_pos.width
                 legend_axes.append(ax2)
                 ax1=legend_axes[-1]
                 ax1.set_axis_off()
                 leg_pos = ax1.get_position()
-                y=leg_pos.y1 if y0 is None else y0
-                max_width = 0
-            y_cax_to_figure=y-f
-            # width=leg_pos.width
-            cax=ax1.figure.add_axes(rect=[leg_pos.x0,y_cax_to_figure,cmap_width,f],
+                y = leg_pos.y1 - legend_vpad * mm2inch * ax.figure.dpi / ax.figure.get_window_extent().height if y0 is None else y0
+                lgd_col_max_width = 0
+
+            cax=ax1.figure.add_axes(rect=[leg_pos.x0,y-f,cmap_width,f],
                                    xmargin=0,ymargin=0) #unit is fractions of figure width and height
             # [i.set_linewidth(0.5) for i in cax.spines.values()]
             cax.figure.subplots_adjust(bottom=0) #wspace=0, hspace=0
             #https://matplotlib.org/stable/api/figure_api.html
             #[left, bottom, width, height],sharex=True,anchor=(0,0),frame_on=False.
             cbar=plot_cmap_legend(ax=ax1,cax=cax,cmap=obj,label=title,label_side=legend_side,kws=legend_kws)
             cbar_width=cbar.ax.get_window_extent().width
             cbars.append(cbar)
-            if cbar_width > max_width:
-                max_width=cbar_width
-            # print(cax.get_position(),cbar.ax.get_position())
+            if cbar_width > lgd_col_max_width:
+                lgd_col_max_width=cbar_width
         elif lgd_t == 'color_dict':
-            # print("color_dict",leg_pos.x0,y)
+            # print(obj, title, legend_kws)
             legend_kws['bbox_to_anchor']=(leg_pos.x0,y) #lower left position of the box.
             #x, y, width, height #kws['bbox_transform'] = ax.figure.transFigure
             # ax1.scatter(leg_pos.x0,y,s=6,color='red',zorder=20,transform=ax1.figure.transFigure)
-            # print("color_dict",ax1.get_position(),leg_pos)
             L = plot_color_dict_legend(D=obj, ax=ax1, title=title, label_side=legend_side,
                                        color_text=color_text, kws=legend_kws)
             if L is None:
                 print("Legend too long, generating a new column..")
-                pad = (max_width + ax.yaxis.labelpad * 2) / ax.figure.get_window_extent().width
+                pad = (lgd_col_max_width + ax.yaxis.labelpad * 2) / ax.figure.get_window_extent().width
                 left_pos = ax1.get_position()
-                ax2 = ax.figure.add_axes([left_pos.x1 + pad, ax.get_position().y0, left_pos.width, ax.get_position().height])
+                ax2 = ax.figure.add_axes([left_pos.x0 + pad, ax.get_position().y0, left_pos.width, ax.get_position().height])
                 legend_axes.append(ax2)
                 ax1 = legend_axes[-1]
                 ax1.set_axis_off()
                 leg_pos = ax1.get_position()
-                y=leg_pos.y1 if y0 is None else y0
+                y = leg_pos.y1 - legend_vpad * mm2inch * ax.figure.dpi / ax.figure.get_window_extent().height if y0 is None else y0
                 legend_kws['bbox_to_anchor'] = (leg_pos.x0, y)
                 L = plot_color_dict_legend(D=obj, ax=ax1, title=title, label_side=legend_side,
                                            color_text=color_text, kws=legend_kws)
-                max_width = 0
+                lgd_col_max_width = 0
             L_width = L.get_window_extent().width
-            if L_width > max_width:
-                max_width = L_width
+            if L_width > lgd_col_max_width:
+                lgd_col_max_width = L_width
             f = L.get_window_extent().height / ax.figure.get_window_extent().height
             cbars.append(L)
         elif lgd_t == 'markers':
             legend_kws['bbox_to_anchor'] = (leg_pos.x0, y)  # lower left position of the box.
             L = plot_marker_legend(obj=obj, ax=ax1, title=title, label_side=legend_side,
                                    color_text=color_text, kws=legend_kws) #obj is a tuple: markers and colors
             if L is None:
                 print("Legend too long, generating a new column..")
-                pad = (max_width + ax.yaxis.labelpad * 2) / ax.figure.get_window_extent().width
+                pad = (lgd_col_max_width + ax.yaxis.labelpad * 2) / ax.figure.get_window_extent().width
                 left_pos = ax1.get_position()
                 ax2 = ax.figure.add_axes(
-                    [left_pos.x1 + pad, ax.get_position().y0, left_pos.width, ax.get_position().height])
+                    [left_pos.x0 + pad, ax.get_position().y0, left_pos.width, ax.get_position().height])
                 legend_axes.append(ax2)
                 ax1 = legend_axes[-1]
                 ax1.set_axis_off()
                 leg_pos = ax1.get_position()
-                y = leg_pos.y1 if y0 is None else y0
+                y = leg_pos.y1 - legend_vpad * mm2inch * ax.figure.dpi / ax.figure.get_window_extent().height if y0 is None else y0
                 legend_kws['bbox_to_anchor'] = (leg_pos.x0, y)
                 L = plot_marker_legend(obj=obj, ax=ax1, title=title, label_side=legend_side,
                                            color_text=color_text, kws=legend_kws)
-                max_width = 0
+                lgd_col_max_width = 0
             L_width = L.get_window_extent().width
-            if L_width > max_width:
-                max_width = L_width
+            if L_width > lgd_col_max_width:
+                lgd_col_max_width = L_width
             f = L.get_window_extent().height / ax.figure.get_window_extent().height
             cbars.append(L)
-        y = y - f - h_gap
+
+        y = y - f - v_gap
         i+=1
+
     if legend_side=='right':
-        boundry=ax1.get_position().y1+max_width / ax.figure.get_window_extent().width
+        boundry=ax1.get_position().y1+lgd_col_max_width / ax.figure.get_window_extent().width
     else:
-        boundry = ax1.get_position().y0 - max_width / ax.figure.get_window_extent().width
+        boundry = ax1.get_position().y0 - lgd_col_max_width / ax.figure.get_window_extent().width
     return legend_axes,cbars,boundry
 # =============================================================================
 set_default_style()
```

### Comparing `PyComplexHeatmap-1.4.4/PyComplexHeatmap.egg-info/PKG-INFO` & `PyComplexHeatmap-1.5.0/PyComplexHeatmap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyComplexHeatmap
-Version: 1.4.4
+Version: 1.5.0
 Summary: A python package to plot complex heatmap
 Home-page: https://github.com/DingWB/PyComplexHeatmap
 Author: Wubin Ding
 Author-email: Wubin Ding <ding.wu.bin.gm@gmail.com>
 Project-URL: Homepage, https://github.com/DingWB/PyComplexHeatmap
 Project-URL: Bug Tracker, https://github.com/DingWB/PyComplexHeatmap/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PyComplexHeatmap-1.4.4/README.md` & `PyComplexHeatmap-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.4.4/pyproject.toml` & `PyComplexHeatmap-1.5.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0","matplotlib>=3.5.1","numpy>=1.20.3","pandas>=1.4.1", "scipy"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PyComplexHeatmap"
-version = "1.4.4"
+version = "1.5.0"
 authors = [
   { name="Wubin Ding", email="ding.wu.bin.gm@gmail.com" },
 ]
 description = "A python package to plot complex heatmap"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

### Comparing `PyComplexHeatmap-1.4.4/setup.py` & `PyComplexHeatmap-1.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 # print(long_description)
 
 #release new version
 setup(
    name='PyComplexHeatmap',
-   version='1.4.4',
+   version='1.5.0',
    description='A Python package to plot complex heatmap',
    # long_description="#PyComplexHeatmap\n##Documentation:https://dingwb.github.io/PyComplexHeatmap/build/html/index.html",
    # long_description_content_type='text/markdown',
    author='Wubin Ding',
    author_email='ding.wu.bin.gm@gmail.com',
    url="https://github.com/DingWB/PyComplexHeatmap",
    packages=['PyComplexHeatmap'], #src
```

