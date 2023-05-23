# Comparing `tmp/qrImageIndexerGUI-0.3.1.tar.gz` & `tmp/qrImageIndexerGUI-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qrImageIndexerGUI-0.3.1.tar", last modified: Sun Mar 26 06:35:04 2023, max compression
+gzip compressed data, was "qrImageIndexerGUI-0.3.2.tar", last modified: Tue May 23 07:24:42 2023, max compression
```

## Comparing `qrImageIndexerGUI-0.3.1.tar` & `qrImageIndexerGUI-0.3.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 06:35:04.084470 qrImageIndexerGUI-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-03-26 06:34:53.000000 qrImageIndexerGUI-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-03-26 06:35:04.084470 qrImageIndexerGUI-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-03-26 06:34:53.000000 qrImageIndexerGUI-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-03-26 06:34:53.000000 qrImageIndexerGUI-0.3.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 06:35:04.080470 qrImageIndexerGUI-0.3.1/qrImageIndexerGUI/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-26 06:34:53.000000 qrImageIndexerGUI-0.3.1/qrImageIndexerGUI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-03-26 06:34:53.000000 qrImageIndexerGUI-0.3.1/qrImageIndexerGUI/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-03-26 06:34:53.000000 qrImageIndexerGUI-0.3.1/qrImageIndexerGUI/generate_qr_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     8551 2023-03-26 06:34:53.000000 qrImageIndexerGUI-0.3.1/qrImageIndexerGUI/image_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-03-26 06:34:53.000000 qrImageIndexerGUI-0.3.1/qrImageIndexerGUI/launch_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-03-26 06:34:53.000000 qrImageIndexerGUI-0.3.1/qrImageIndexerGUI/sort_images_window.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 06:35:04.080470 qrImageIndexerGUI-0.3.1/qrImageIndexerGUI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-03-26 06:35:04.000000 qrImageIndexerGUI-0.3.1/qrImageIndexerGUI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-03-26 06:35:04.000000 qrImageIndexerGUI-0.3.1/qrImageIndexerGUI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 06:35:04.000000 qrImageIndexerGUI-0.3.1/qrImageIndexerGUI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-26 06:35:04.000000 qrImageIndexerGUI-0.3.1/qrImageIndexerGUI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-26 06:35:04.000000 qrImageIndexerGUI-0.3.1/qrImageIndexerGUI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-26 06:35:04.084470 qrImageIndexerGUI-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-26 06:34:53.000000 qrImageIndexerGUI-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 06:35:04.084470 qrImageIndexerGUI-0.3.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-03-26 06:34:53.000000 qrImageIndexerGUI-0.3.1/test/test_generate_qr_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-03-26 06:34:53.000000 qrImageIndexerGUI-0.3.1/test/test_sort_images_window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:24:42.651871 qrImageIndexerGUI-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-23 07:24:24.000000 qrImageIndexerGUI-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-05-23 07:24:42.651871 qrImageIndexerGUI-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-05-23 07:24:24.000000 qrImageIndexerGUI-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-23 07:24:24.000000 qrImageIndexerGUI-0.3.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:24:42.647871 qrImageIndexerGUI-0.3.2/qrImageIndexerGUI/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-23 07:24:24.000000 qrImageIndexerGUI-0.3.2/qrImageIndexerGUI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-23 07:24:24.000000 qrImageIndexerGUI-0.3.2/qrImageIndexerGUI/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-05-23 07:24:24.000000 qrImageIndexerGUI-0.3.2/qrImageIndexerGUI/generate_qr_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8551 2023-05-23 07:24:24.000000 qrImageIndexerGUI-0.3.2/qrImageIndexerGUI/image_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-23 07:24:24.000000 qrImageIndexerGUI-0.3.2/qrImageIndexerGUI/launch_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-05-23 07:24:24.000000 qrImageIndexerGUI-0.3.2/qrImageIndexerGUI/sort_images_window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:24:42.647871 qrImageIndexerGUI-0.3.2/qrImageIndexerGUI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-05-23 07:24:42.000000 qrImageIndexerGUI-0.3.2/qrImageIndexerGUI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-23 07:24:42.000000 qrImageIndexerGUI-0.3.2/qrImageIndexerGUI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 07:24:42.000000 qrImageIndexerGUI-0.3.2/qrImageIndexerGUI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-23 07:24:42.000000 qrImageIndexerGUI-0.3.2/qrImageIndexerGUI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-23 07:24:42.000000 qrImageIndexerGUI-0.3.2/qrImageIndexerGUI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 07:24:42.651871 qrImageIndexerGUI-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-23 07:24:24.000000 qrImageIndexerGUI-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:24:42.651871 qrImageIndexerGUI-0.3.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     8040 2023-05-23 07:24:24.000000 qrImageIndexerGUI-0.3.2/test/test_generate_qr_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5837 2023-05-23 07:24:24.000000 qrImageIndexerGUI-0.3.2/test/test_sort_images_window.py
```

### Comparing `qrImageIndexerGUI-0.3.1/LICENSE` & `qrImageIndexerGUI-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qrImageIndexerGUI-0.3.1/PKG-INFO` & `qrImageIndexerGUI-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qrImageIndexerGUI
-Version: 0.3.1
+Version: 0.3.2
 Summary: GUI interface for tool for indexing images with QR codes
 Author-email: Jonathan Pecar <jonathan.pecar@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 jonpecar
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `qrImageIndexerGUI-0.3.1/README.md` & `qrImageIndexerGUI-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `qrImageIndexerGUI-0.3.1/pyproject.toml` & `qrImageIndexerGUI-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "qrImageIndexerGUI"
-version = "0.3.1"
+version = "0.3.2"
 description = "GUI interface for tool for indexing images with QR codes"
 readme = "README.md"
 authors = [{name = "Jonathan Pecar", email = "jonathan.pecar@gmail.com"}]
 license = { file = "LICENSE"}
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["sorter", "qrcode", "photosorter"]
 dependencies = [
-        "qrImageIndexer>=0.7.3",
+        "qrImageIndexer>=0.7.4",
         "PyMuPDF",
         "pillow",
         "natsort",
         "customtkinter>=5.0.3"
 ]
 requires-python = ">=3.7"
 [project.optional-dependencies]
 dev = ["pytest", "bumpver", "setuptools", "pytest-mock"]
 
 [project.urls]
 Homepage = "https://github.com/jonpecar/qrCodeImageSorterGUI"
 [tool.bumpver]
-current_version = "0.3.1"
+current_version = "0.3.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `qrImageIndexerGUI-0.3.1/qrImageIndexerGUI/generate_qr_window.py` & `qrImageIndexerGUI-0.3.2/qrImageIndexerGUI/generate_qr_window.py`

 * *Files 16% similar despite different names*

```diff
@@ -143,14 +143,24 @@
             # bg=self.cget('fg_color')[1] if ctk.get_appearance_mode() == 'Dark' else self.cget('fg_color')[0])
         self.doc_viewer.pack(fill=tk.BOTH, expand=True, side=tk.TOP,
                             padx=FRAME_PAD_PX, pady=FRAME_PAD_PX)
 
         self.update_pdf_sample() #Update the PDF here so that it will contain the sample text and use all the default settings
 
     def save_pdf(self):
+        if self.has_invalid_path_chars():
+            proceed = messagebox.askyesno('Found Invalid File Characters', 
+                                             "One or more of the following characters were found in your text:"
+                                              + " '<', '>', ':', '\"', '|', '\\', '/', '?', '*'. "
+                                              + "These are not valid characters for file paths in Windows." 
+                                              + " If you proceed these will be removed when sorting the images"
+                                              + " except for '\\' and '/' which will create new folders." 
+                                              + "\n\nDo you wish to proceed?")
+            if not proceed: return
+        
         file = filedialog.asksaveasfile(mode='wb', confirmoverwrite=True, defaultextension='.pdf',
                                         filetypes=[['PDF Files', '*.pdf']])
         pdf = self.generate_pdf()
         pdf.output(file)
         file.close()
         messagebox.showinfo("File Saved", "File successfully saved.")
 
@@ -162,8 +172,14 @@
         text = self.enter_txt.get("1.0", tk.END)
         text = text.split('\n')
         data = load_lines(text)
         prefix = ''
         if check_states['use_prefix']:
             prefix = self.opt_frame.get_prefix()
         return generate_qr_pdf(data, check_states['qr_headings'], check_states['repeat_headings'],
-                                check_states['sliceable'], prefix)
+                                check_states['sliceable'], prefix)
+    
+    def has_invalid_path_chars(self) -> bool:
+        invalid_chars_windows = ['<', '>', ':', '"', '|', '\\', '/', '?', '*']
+        text = self.enter_txt.get("1.0", tk.END)
+        has_invalid_chars = [char in text for char in invalid_chars_windows]
+        return True in has_invalid_chars
```

### Comparing `qrImageIndexerGUI-0.3.1/qrImageIndexerGUI/image_grid.py` & `qrImageIndexerGUI-0.3.2/qrImageIndexerGUI/image_grid.py`

 * *Files identical despite different names*

### Comparing `qrImageIndexerGUI-0.3.1/qrImageIndexerGUI/launch_window.py` & `qrImageIndexerGUI-0.3.2/qrImageIndexerGUI/launch_window.py`

 * *Files identical despite different names*

### Comparing `qrImageIndexerGUI-0.3.1/qrImageIndexerGUI/sort_images_window.py` & `qrImageIndexerGUI-0.3.2/qrImageIndexerGUI/sort_images_window.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,22 +38,28 @@
             for image_path, qr_string in pool.imap(func, self.image_files):
                 self.done += 1
                 self.percent = (self.done * 100)//len(self.image_files)
                 if qr_string:
                     self.results[image_path] = qr_string
 
 class ImageCopy(Thread):
-    def __init__(self, scan_results : Dict[str, str], in_directory : str, out_directory : str):
+    def __init__(self, scan_results : Dict[str, str], in_directory : str, out_directory : str, use_date : bool):
         Thread.__init__(self)
         self.scan_results = scan_results
         self.in_directory = in_directory
         self.out_directory = out_directory
+        self.use_date = use_date
 
     def run(self):
-        photo_sorter.sort_directory_exisitng_results(self.scan_results, self.in_directory, self.out_directory, False)
+        photo_sorter.sort_directory_exisitng_results(
+            self.scan_results, 
+            self.in_directory, 
+            self.out_directory, 
+            False, 
+            order_by_date=self.use_date)
 
 class ScanImagesWindow(ctk.CTkToplevel):
     def __init__(self, master, *args, **kwargs):
         ctk.CTkToplevel.__init__(self, master, *args, **kwargs)
         self.geometry("1200x800")
         self.title("Sort Images by QR Codes")
         self.button_frame = ctk.CTkFrame(self)
@@ -112,15 +118,18 @@
         self._save_files(directory)
 
 
 
     def _save_files(self, out_dir: str):
         if os.path.isdir(out_dir):
             self.out_directory = out_dir
-            save_thread = ImageCopy(self.scan_results, self.in_directory, self.out_directory)
+            save_thread = ImageCopy(self.scan_results, 
+                                    self.in_directory, 
+                                    self.out_directory, 
+                                    self.scan_opts.use_dates())
             save_thread.start()
             self.monitor_progress_image_save(save_thread)
 
     def disable_buttons(self):
         """
             Disable buttons while processes running to avoid clash
         """
@@ -174,23 +183,32 @@
     def __init__(self, parent, *args, **kwargs):
         ctk.CTkFrame.__init__(self, parent, *args, **kwargs)
 
         self.has_prefix_chk_var = tk.BooleanVar()
         self.has_prefix_chk = ctk.CTkCheckBox(self, text='QR codes have prefix',
                                             variable=self.has_prefix_chk_var, onvalue=True,
                                             offvalue=False)
+        self.use_dates_chk_var = tk.BooleanVar()
+        self.use_dates_chk = ctk.CTkCheckBox(self, text='Use modified date to order input images',
+                                    variable=self.use_dates_chk_var, onvalue=True,
+                                    offvalue=False)
         self.prefix_frame = ctk.CTkFrame(self)
         self.prefix_label = ctk.CTkLabel(self.prefix_frame, text="Prefix:")
         self.prefix_input = ctk.CTkEntry(self.prefix_frame)
         
         self.has_prefix_chk_var.set(True)
         self.has_prefix_chk.pack(side=tk.TOP, fill=tk.BOTH)
+        self.use_dates_chk_var.set(False)
+        self.use_dates_chk.pack(side=tk.TOP, fill=tk.BOTH)
         self.prefix_frame.pack(side=tk.TOP, fill=tk.BOTH)
         self.prefix_label.pack(side=tk.LEFT, fill=tk.BOTH)
         self.prefix_input.insert(0, r"{image}")
         self.prefix_input.pack(side=tk.RIGHT, fill=tk.BOTH, expand=True)
 
     def get_prefix(self) -> str:
         if self.has_prefix_chk_var.get():
             return self.prefix_input.get()
         else:
-            return ''
+            return ''
+        
+    def use_dates(self) -> bool:
+        return self.use_dates_chk_var.get()
```

### Comparing `qrImageIndexerGUI-0.3.1/qrImageIndexerGUI.egg-info/PKG-INFO` & `qrImageIndexerGUI-0.3.2/qrImageIndexerGUI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qrImageIndexerGUI
-Version: 0.3.1
+Version: 0.3.2
 Summary: GUI interface for tool for indexing images with QR codes
 Author-email: Jonathan Pecar <jonathan.pecar@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 jonpecar
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `qrImageIndexerGUI-0.3.1/qrImageIndexerGUI.egg-info/SOURCES.txt` & `qrImageIndexerGUI-0.3.2/qrImageIndexerGUI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qrImageIndexerGUI-0.3.1/test/test_generate_qr_window.py` & `qrImageIndexerGUI-0.3.2/test/test_generate_qr_window.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 import pytest
 import tkinter as tk
 import customtkinter as ctk
 from qrImageIndexerGUI import generate_qr_window
+import time
 
 # Testing the behaviour of the checkboxes. Probably not the best practice, but wanted to make sure that
 # they are representing the checked state of the appropriate checkboxes
 
 @pytest.fixture
 def options_frame() -> generate_qr_window.OptionsFrame:
     app = ctk.CTk()
     frame = generate_qr_window.OptionsFrame(app)
     yield frame
     app.destroy()
 
+@pytest.fixture
+def generate_qr_frame() -> generate_qr_window.GenerateQRWindow:
+    app = ctk.CTk()
+    frame = generate_qr_window.GenerateQRWindow(app)
+    yield frame
+    app.destroy()
 
 def test_sliceable_checkbox_check(options_frame : generate_qr_window.OptionsFrame):
     options_frame.sort_sliceable_chk.select()
     assert options_frame.get_check_states()['sliceable']
 
 def test_sliceable_checkbox_uncheck(options_frame : generate_qr_window.OptionsFrame):
     options_frame.sort_sliceable_chk.deselect()
@@ -47,14 +54,22 @@
     assert not options_frame.get_check_states()['use_prefix']
 
 def test_get_prefix_option(options_frame : generate_qr_window.OptionsFrame):
     options_frame.prefix_input.delete(0, tk.END)
     options_frame.prefix_input.insert(0, 'prefix')
     assert options_frame.get_prefix() == 'prefix'
 
+def test_check_text_for_invalid_chars_pass_for_valid_chars(generate_qr_frame : generate_qr_window.GenerateQRWindow):
+    generate_qr_frame.enter_txt.insert("1.0", 'These are \nAll valid characters\n7892719312\t-_78473#')
+    assert generate_qr_frame.has_invalid_path_chars() == False
+    
+def test_check_text_for_invalid_chars_fail_for_invalid_chars(generate_qr_frame : generate_qr_window.GenerateQRWindow):
+    generate_qr_frame.enter_txt.insert("1.0", 'Here are some\nInvalid *\nPath chars <')
+    assert generate_qr_frame.has_invalid_path_chars() == True
+
 @pytest.fixture
 def mocked_qr_generate_functions(mocker):
 
     get_check_states = mocker.patch('qrImageIndexerGUI.generate_qr_window.OptionsFrame.get_check_states')
 
     get_prefix = mocker.patch('qrImageIndexerGUI.generate_qr_window.OptionsFrame.get_prefix')
```

### Comparing `qrImageIndexerGUI-0.3.1/test/test_sort_images_window.py` & `qrImageIndexerGUI-0.3.2/test/test_sort_images_window.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,15 +192,15 @@
         'c':789
     }
 
     expect_keys = ['a', 'b', 'c']
     
     assert expect_keys == list(sort_images_window.ScanImagesWindow.sort_results_dict(input).keys())
 
-def test_sort_dict_function_unergdered():
+def test_sort_dict_function_unordered():
     input = {
         'a':123,
         'c':789,
         'b':456
     }
 
     expect_keys = ['a', 'b', 'c']
```

