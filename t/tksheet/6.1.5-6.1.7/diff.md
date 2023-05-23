# Comparing `tmp/tksheet-6.1.5.tar.gz` & `tmp/tksheet-6.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tksheet-6.1.5.tar", last modified: Fri May 19 16:16:43 2023, max compression
+gzip compressed data, was "tksheet-6.1.7.tar", last modified: Tue May 23 08:14:15 2023, max compression
```

## Comparing `tksheet-6.1.5.tar` & `tksheet-6.1.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 16:16:43.617146 tksheet-6.1.5/
--rw-rw-rw-   0        0        0     1101 2023-05-19 10:58:20.000000 tksheet-6.1.5/LICENSE.txt
--rw-rw-rw-   0        0        0     3657 2023-05-19 16:16:43.617146 tksheet-6.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     3007 2023-05-19 10:58:20.000000 tksheet-6.1.5/README.md
--rw-rw-rw-   0        0        0       86 2023-05-19 16:16:43.617146 tksheet-6.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1010 2023-05-19 10:59:33.000000 tksheet-6.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 16:16:43.601509 tksheet-6.1.5/tksheet/
--rw-rw-rw-   0        0        0     1901 2023-05-19 10:58:20.000000 tksheet-6.1.5/tksheet/__init__.py
--rw-rw-rw-   0        0        0   163926 2023-05-19 15:49:40.000000 tksheet-6.1.5/tksheet/_tksheet.py
--rw-rw-rw-   0        0        0   111539 2023-05-19 10:58:20.000000 tksheet-6.1.5/tksheet/_tksheet_column_headers.py
--rw-rw-rw-   0        0        0     8846 2023-05-19 10:58:20.000000 tksheet-6.1.5/tksheet/_tksheet_formatters.py
--rw-rw-rw-   0        0        0   328259 2023-05-19 10:58:20.000000 tksheet-6.1.5/tksheet/_tksheet_main_table.py
--rw-rw-rw-   0        0        0    12695 2023-05-19 10:58:20.000000 tksheet-6.1.5/tksheet/_tksheet_other_classes.py
--rw-rw-rw-   0        0        0   108469 2023-05-19 10:58:20.000000 tksheet-6.1.5/tksheet/_tksheet_row_index.py
--rw-rw-rw-   0        0        0     5746 2023-05-19 10:58:20.000000 tksheet-6.1.5/tksheet/_tksheet_top_left_rectangle.py
--rw-rw-rw-   0        0        0    59987 2023-05-19 10:58:20.000000 tksheet-6.1.5/tksheet/_tksheet_vars.py
-drwxrwxrwx   0        0        0        0 2023-05-19 16:16:43.617146 tksheet-6.1.5/tksheet.egg-info/
--rw-rw-rw-   0        0        0     3657 2023-05-19 16:16:43.000000 tksheet-6.1.5/tksheet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2023-05-19 16:16:43.000000 tksheet-6.1.5/tksheet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 16:16:43.000000 tksheet-6.1.5/tksheet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-19 16:16:43.000000 tksheet-6.1.5/tksheet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 08:14:15.022253 tksheet-6.1.7/
+-rw-rw-rw-   0        0        0     1101 2023-05-23 07:18:56.000000 tksheet-6.1.7/LICENSE.txt
+-rw-rw-rw-   0        0        0     3657 2023-05-23 08:14:15.022253 tksheet-6.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3007 2023-05-23 07:18:56.000000 tksheet-6.1.7/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-23 08:14:15.022253 tksheet-6.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1010 2023-05-23 07:43:27.000000 tksheet-6.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 08:14:15.014748 tksheet-6.1.7/tksheet/
+-rw-rw-rw-   0        0        0     1901 2023-05-23 07:18:56.000000 tksheet-6.1.7/tksheet/__init__.py
+-rw-rw-rw-   0        0        0   163926 2023-05-23 07:18:56.000000 tksheet-6.1.7/tksheet/_tksheet.py
+-rw-rw-rw-   0        0        0   111612 2023-05-23 08:01:56.000000 tksheet-6.1.7/tksheet/_tksheet_column_headers.py
+-rw-rw-rw-   0        0        0     8846 2023-05-23 07:18:56.000000 tksheet-6.1.7/tksheet/_tksheet_formatters.py
+-rw-rw-rw-   0        0        0   329885 2023-05-23 08:10:54.000000 tksheet-6.1.7/tksheet/_tksheet_main_table.py
+-rw-rw-rw-   0        0        0    12695 2023-05-23 07:18:57.000000 tksheet-6.1.7/tksheet/_tksheet_other_classes.py
+-rw-rw-rw-   0        0        0   108542 2023-05-23 08:02:12.000000 tksheet-6.1.7/tksheet/_tksheet_row_index.py
+-rw-rw-rw-   0        0        0     5746 2023-05-23 07:18:57.000000 tksheet-6.1.7/tksheet/_tksheet_top_left_rectangle.py
+-rw-rw-rw-   0        0        0    59987 2023-05-23 07:18:57.000000 tksheet-6.1.7/tksheet/_tksheet_vars.py
+drwxrwxrwx   0        0        0        0 2023-05-23 08:14:15.022253 tksheet-6.1.7/tksheet.egg-info/
+-rw-rw-rw-   0        0        0     3657 2023-05-23 08:14:14.000000 tksheet-6.1.7/tksheet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2023-05-23 08:14:14.000000 tksheet-6.1.7/tksheet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 08:14:14.000000 tksheet-6.1.7/tksheet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-23 08:14:14.000000 tksheet-6.1.7/tksheet.egg-info/top_level.txt
```

### Comparing `tksheet-6.1.5/LICENSE.txt` & `tksheet-6.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.5/PKG-INFO` & `tksheet-6.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tksheet
-Version: 6.1.5
+Version: 6.1.7
 Summary: Tkinter table / sheet widget
 Home-page: https://github.com/ragardner/tksheet
-Download-URL: https://github.com/ragardner/tksheet/archive/6.1.5.tar.gz
+Download-URL: https://github.com/ragardner/tksheet/archive/6.1.7.tar.gz
 Author: ragardner
 Author-email: github@ragardner.simplelogin.com
 License: MIT
 Keywords: tkinter,table,widget,sheet,grid,tk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `tksheet-6.1.5/README.md` & `tksheet-6.1.7/README.md`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.5/setup.py` & `tksheet-6.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding = 'utf-8') as f:
     long_description = f.read()
 
 setup(
   name = 'tksheet',
   packages = ['tksheet'],
-  version = '6.1.5',
+  version = '6.1.7',
   python_requires = '>=3.6',
   license = 'MIT',
   description = 'Tkinter table / sheet widget',
   long_description = long_description,
   long_description_content_type = 'text/markdown',
   author = 'ragardner',
   author_email = 'github@ragardner.simplelogin.com',
   url = 'https://github.com/ragardner/tksheet',
-  download_url = 'https://github.com/ragardner/tksheet/archive/6.1.5.tar.gz',
+  download_url = 'https://github.com/ragardner/tksheet/archive/6.1.7.tar.gz',
   keywords = ['tkinter', 'table', 'widget', 'sheet', 'grid', 'tk'],
   install_requires = [],
   classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License'
```

### Comparing `tksheet-6.1.5/tksheet/__init__.py` & `tksheet-6.1.7/tksheet/__init__.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.5/tksheet/_tksheet.py` & `tksheet-6.1.7/tksheet/_tksheet.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.5/tksheet/_tksheet_column_headers.py` & `tksheet-6.1.7/tksheet/_tksheet_column_headers.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,14 +43,15 @@
             highlightthickness=0,
         )
         self.parentframe = kwargs["parentframe"]
         self.current_height = None  # is set from within MainTable() __init__ or from Sheet parameters
         self.MT = None  # is set from within MainTable() __init__
         self.RI = None  # is set from within MainTable() __init__
         self.TL = None  # is set from within TopLeftRectangle() __init__
+        self.popup_menu_loc = None
         self.extra_begin_edit_cell_func = None
         self.extra_end_edit_cell_func = None
         self.text_editor = None
         self.text_editor_id = None
         self.text_editor_loc = None
         self.centre_alignment_text_mod_indexes = (slice(1, None), slice(None, -1))
         self.c_align_cyc = cycle(self.centre_alignment_text_mod_indexes)
@@ -235,14 +236,15 @@
                     elif self.MT.toggle_selection_enabled and self.MT.rc_select_enabled:
                         self.toggle_select_col(c, redraw=True)
                     if self.MT.rc_popup_menus_enabled:
                         popup_menu = self.ch_rc_popup_menu
         if self.extra_rc_func is not None:
             self.extra_rc_func(event)
         if popup_menu is not None:
+            self.popup_menu_loc = c
             popup_menu.tk_popup(event.x_root, event.y_root)
 
     def ctrl_b1_press(self, event=None):
         self.mouseclick_outside_editor_or_dropdown_all_canvases()
         if (
             (self.drag_and_drop_enabled or self.col_selection_enabled)
             and self.MT.ctrl_select_enabled
```

### Comparing `tksheet-6.1.5/tksheet/_tksheet_formatters.py` & `tksheet-6.1.7/tksheet/_tksheet_formatters.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.5/tksheet/_tksheet_main_table.py` & `tksheet-6.1.7/tksheet/_tksheet_main_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     SelectCellEvent,
     SelectionBoxEvent,
     TextCfg,
     TextEditor,
     UndoEvent,
     get_checkbox_dict,
     get_dropdown_dict,
+    get_seq_without_gaps_at_index,
     is_iterable,
 )
 from ._tksheet_vars import (
     USER_OS,
     Color_Map_,
     arrowkey_bindings_helper,
     ctrl_key,
@@ -4084,18 +4085,33 @@
                 )
             )
         self.refresh()
         if self.extra_end_insert_rows_rc_func is not None:
             self.extra_end_insert_rows_rc_func(InsertEvent("end_insert_rows", data_ins_row, displayed_ins_row, numrows))
         self.parentframe.emit_event("<<SheetModified>>")
 
-    def del_cols_rc(self, event=None):
+    def del_cols_rc(self, event=None, c=None):
         seld_cols = sorted(self.get_selected_cols())
-        if not seld_cols:
+        curr = self.currently_selected()
+        if not seld_cols or not curr:
             return
+        if self.CH.popup_menu_loc is None or self.CH.popup_menu_loc < seld_cols[0] or self.CH.popup_menu_loc > seld_cols[-1]:
+            c = seld_cols[0]
+        else:
+            c = self.CH.popup_menu_loc
+        seld_cols = get_seq_without_gaps_at_index(seld_cols, c)
+        self.deselect("all", redraw=False)
+        self.create_selected(
+                        0,
+                        seld_cols[0],
+                        len(self.row_positions) - 1,
+                        seld_cols[-1] + 1,
+                        "columns",
+                    )
+        self.set_currently_selected(0, seld_cols[0], type_="column")
         seldmax = seld_cols[-1] if self.all_columns_displayed else self.displayed_columns[seld_cols[-1]]
         if self.extra_begin_del_cols_rc_func is not None:
             try:
                 self.extra_begin_del_cols_rc_func(DeleteRowColumnEvent("begin_delete_columns", seld_cols))
             except Exception:
                 return
         seldset = set(seld_cols) if self.all_columns_displayed else set(self.displayed_columns[c] for c in seld_cols)
@@ -4136,41 +4152,54 @@
                 except Exception:
                     continue
         if self.undo_enabled:
             self.undo_storage.append(("delete_cols", undo_storage))
         for c in reversed(seld_cols):
             self.del_col_position(c, deselect_all=False)
         numcols = len(seld_cols)
-
         self.cell_options = {
             (rn, cn if cn < seldmax else cn - numcols): t2
             for (rn, cn), t2 in self.cell_options.items()
             if cn not in seldset
         }
         self.col_options = {
             cn if cn < seldmax else cn - numcols: t for cn, t in self.col_options.items() if cn not in seldset
         }
         self.CH.cell_options = {
             cn if cn < seldmax else cn - numcols: t for cn, t in self.CH.cell_options.items() if cn not in seldset
         }
-        self.deselect("allcols", redraw=False)
-        self.set_current_to_last()
+        self.deselect("all", redraw=False)
         if not self.all_columns_displayed:
             self.displayed_columns = [c for c in self.displayed_columns if c not in seldset]
             for c in sorted(seldset):
                 self.displayed_columns = [dc if c > dc else dc - 1 for dc in self.displayed_columns]
         self.refresh()
         if self.extra_end_del_cols_rc_func is not None:
             self.extra_end_del_cols_rc_func(DeleteRowColumnEvent("end_delete_columns", seld_cols))
         self.parentframe.emit_event("<<SheetModified>>")
 
-    def del_rows_rc(self, event=None):
+    def del_rows_rc(self, event=None, r=None):
         seld_rows = sorted(self.get_selected_rows())
-        if not seld_rows:
+        curr = self.currently_selected()
+        if not seld_rows or not curr:
             return
+        if self.RI.popup_menu_loc is None or self.RI.popup_menu_loc < seld_rows[0] or self.RI.popup_menu_loc > seld_rows[-1]:
+            r = seld_rows[0]
+        else:
+            r = self.RI.popup_menu_loc
+        seld_rows = get_seq_without_gaps_at_index(seld_rows, r)
+        self.deselect("all", redraw=False)
+        self.create_selected(
+                        seld_rows[0],
+                        0,
+                        seld_rows[-1] + 1,
+                        len(self.col_positions) - 1,
+                        "rows",
+                    )
+        self.set_currently_selected(seld_rows[0], 0, type_="row")
         seldmax = seld_rows[-1] if self.all_rows_displayed else self.displayed_rows[seld_rows[-1]]
         if self.extra_begin_del_rows_rc_func is not None:
             try:
                 self.extra_begin_del_rows_rc_func(DeleteRowColumnEvent("begin_delete_rows", seld_rows))
             except Exception:
                 return
         seldset = set(seld_rows) if self.all_rows_displayed else set(self.displayed_rows[r] for r in seld_rows)
@@ -4204,28 +4233,30 @@
                 except Exception:
                     continue
         if self.undo_enabled:
             self.undo_storage.append(("delete_rows", undo_storage))
         for r in reversed(seld_rows):
             self.del_row_position(r, deselect_all=False)
         numrows = len(seld_rows)
-
         self.cell_options = {
             (rn if rn < seldmax else rn - numrows, cn): t2
             for (rn, cn), t2 in self.cell_options.items()
             if rn not in seldset
         }
         self.row_options = {
             rn if rn < seldmax else rn - numrows: t for rn, t in self.row_options.items() if rn not in seldset
         }
         self.RI.cell_options = {
             rn if rn < seldmax else rn - numrows: t for rn, t in self.RI.cell_options.items() if rn not in seldset
         }
-        self.deselect("allrows", redraw=False)
-        self.set_current_to_last()
+        self.deselect("all", redraw=False)
+        if not self.all_rows_displayed:
+            self.displayed_rows = [r for r in self.displayed_rows if r not in seldset]
+            for r in sorted(seldset):
+                self.displayed_rows = [dr if r > dr else dr - 1 for dr in self.displayed_rows]
         self.refresh()
         if self.extra_end_del_rows_rc_func is not None:
             self.extra_end_del_rows_rc_func(DeleteRowColumnEvent("end_delete_rows", seld_rows))
         self.parentframe.emit_event("<<SheetModified>>")
 
     def move_row_position(self, idx1, idx2):
         if not len(self.row_positions) <= 2:
```

### Comparing `tksheet-6.1.5/tksheet/_tksheet_other_classes.py` & `tksheet-6.1.7/tksheet/_tksheet_other_classes.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.5/tksheet/_tksheet_row_index.py` & `tksheet-6.1.7/tksheet/_tksheet_row_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,14 +44,15 @@
             background=kwargs["index_bg"],
             highlightthickness=0,
         )
         self.parentframe = kwargs["parentframe"]
         self.MT = None  # is set from within MainTable() __init__
         self.CH = None  # is set from within MainTable() __init__
         self.TL = None  # is set from within TopLeftRectangle() __init__
+        self.popup_menu_loc = None
         self.extra_begin_edit_cell_func = None
         self.extra_end_edit_cell_func = None
         self.text_editor = None
         self.text_editor_id = None
         self.text_editor_loc = None
         self.b1_pressed_loc = None
         self.existing_dropdown_canvas_id = None
@@ -204,14 +205,15 @@
                     elif self.MT.toggle_selection_enabled and self.MT.rc_select_enabled:
                         self.toggle_select_row(r, redraw=True)
                     if self.MT.rc_popup_menus_enabled:
                         popup_menu = self.ri_rc_popup_menu
         if self.extra_rc_func is not None:
             self.extra_rc_func(event)
         if popup_menu is not None:
+            self.popup_menu_loc = r
             popup_menu.tk_popup(event.x_root, event.y_root)
 
     def ctrl_b1_press(self, event=None):
         self.mouseclick_outside_editor_or_dropdown_all_canvases()
         if (
             (self.drag_and_drop_enabled or self.row_selection_enabled)
             and self.MT.ctrl_select_enabled
```

### Comparing `tksheet-6.1.5/tksheet/_tksheet_top_left_rectangle.py` & `tksheet-6.1.7/tksheet/_tksheet_top_left_rectangle.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.5/tksheet/_tksheet_vars.py` & `tksheet-6.1.7/tksheet/_tksheet_vars.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.5/tksheet.egg-info/PKG-INFO` & `tksheet-6.1.7/tksheet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tksheet
-Version: 6.1.5
+Version: 6.1.7
 Summary: Tkinter table / sheet widget
 Home-page: https://github.com/ragardner/tksheet
-Download-URL: https://github.com/ragardner/tksheet/archive/6.1.5.tar.gz
+Download-URL: https://github.com/ragardner/tksheet/archive/6.1.7.tar.gz
 Author: ragardner
 Author-email: github@ragardner.simplelogin.com
 License: MIT
 Keywords: tkinter,table,widget,sheet,grid,tk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

