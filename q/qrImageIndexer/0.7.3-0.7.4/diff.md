# Comparing `tmp/qrImageIndexer-0.7.3.tar.gz` & `tmp/qrImageIndexer-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qrImageIndexer-0.7.3.tar", last modified: Tue Sep 27 23:40:53 2022, max compression
+gzip compressed data, was "qrImageIndexer-0.7.4.tar", last modified: Tue May 23 06:40:16 2023, max compression
```

## Comparing `qrImageIndexer-0.7.3.tar` & `qrImageIndexer-0.7.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 23:40:53.456009 qrImageIndexer-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-09-27 23:40:42.000000 qrImageIndexer-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     8562 2022-09-27 23:40:53.456009 qrImageIndexer-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6798 2022-09-27 23:40:42.000000 qrImageIndexer-0.7.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1202 2022-09-27 23:40:42.000000 qrImageIndexer-0.7.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 23:40:53.452009 qrImageIndexer-0.7.3/qrImageIndexer/
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-09-27 23:40:42.000000 qrImageIndexer-0.7.3/qrImageIndexer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3441 2022-09-27 23:40:42.000000 qrImageIndexer-0.7.3/qrImageIndexer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      602 2022-09-27 23:40:42.000000 qrImageIndexer-0.7.3/qrImageIndexer/generate_qr_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)    10200 2022-09-27 23:40:42.000000 qrImageIndexer-0.7.3/qrImageIndexer/photo_sorter.py
--rw-r--r--   0 runner    (1001) docker     (121)     8100 2022-09-27 23:40:42.000000 qrImageIndexer-0.7.3/qrImageIndexer/qr_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)     4728 2022-09-27 23:40:42.000000 qrImageIndexer-0.7.3/qrImageIndexer/write_pdf_fpf2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 23:40:53.452009 qrImageIndexer-0.7.3/qrImageIndexer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8562 2022-09-27 23:40:53.000000 qrImageIndexer-0.7.3/qrImageIndexer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      526 2022-09-27 23:40:53.000000 qrImageIndexer-0.7.3/qrImageIndexer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-27 23:40:53.000000 qrImageIndexer-0.7.3/qrImageIndexer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-09-27 23:40:53.000000 qrImageIndexer-0.7.3/qrImageIndexer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-09-27 23:40:53.000000 qrImageIndexer-0.7.3/qrImageIndexer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-27 23:40:53.456009 qrImageIndexer-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-09-27 23:40:42.000000 qrImageIndexer-0.7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 23:40:53.456009 qrImageIndexer-0.7.3/test/
--rw-r--r--   0 runner    (1001) docker     (121)     2889 2022-09-27 23:40:42.000000 qrImageIndexer-0.7.3/test/test_pdf_build_fpdf2.py
--rw-r--r--   0 runner    (1001) docker     (121)     6333 2022-09-27 23:40:42.000000 qrImageIndexer-0.7.3/test/test_photo_sorter.py
--rw-r--r--   0 runner    (1001) docker     (121)     8981 2022-09-27 23:40:42.000000 qrImageIndexer-0.7.3/test/test_qr_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2937 2022-09-27 23:40:42.000000 qrImageIndexer-0.7.3/test/test_qr_pdf_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:40:16.720028 qrImageIndexer-0.7.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-23 06:40:03.000000 qrImageIndexer-0.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-05-23 06:40:16.720028 qrImageIndexer-0.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-05-23 06:40:03.000000 qrImageIndexer-0.7.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-23 06:40:03.000000 qrImageIndexer-0.7.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:40:16.716028 qrImageIndexer-0.7.4/qrImageIndexer/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-23 06:40:03.000000 qrImageIndexer-0.7.4/qrImageIndexer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-05-23 06:40:03.000000 qrImageIndexer-0.7.4/qrImageIndexer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-23 06:40:03.000000 qrImageIndexer-0.7.4/qrImageIndexer/generate_qr_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10661 2023-05-23 06:40:03.000000 qrImageIndexer-0.7.4/qrImageIndexer/photo_sorter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8100 2023-05-23 06:40:03.000000 qrImageIndexer-0.7.4/qrImageIndexer/qr_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-05-23 06:40:03.000000 qrImageIndexer-0.7.4/qrImageIndexer/write_pdf_fpf2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:40:16.720028 qrImageIndexer-0.7.4/qrImageIndexer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-05-23 06:40:16.000000 qrImageIndexer-0.7.4/qrImageIndexer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-23 06:40:16.000000 qrImageIndexer-0.7.4/qrImageIndexer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 06:40:16.000000 qrImageIndexer-0.7.4/qrImageIndexer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-23 06:40:16.000000 qrImageIndexer-0.7.4/qrImageIndexer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-23 06:40:16.000000 qrImageIndexer-0.7.4/qrImageIndexer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 06:40:16.720028 qrImageIndexer-0.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-23 06:40:03.000000 qrImageIndexer-0.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:40:16.720028 qrImageIndexer-0.7.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-23 06:40:03.000000 qrImageIndexer-0.7.4/test/test_pdf_build_fpdf2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7695 2023-05-23 06:40:03.000000 qrImageIndexer-0.7.4/test/test_photo_sorter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8981 2023-05-23 06:40:03.000000 qrImageIndexer-0.7.4/test/test_qr_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-05-23 06:40:03.000000 qrImageIndexer-0.7.4/test/test_qr_pdf_wrapper.py
```

### Comparing `qrImageIndexer-0.7.3/LICENSE` & `qrImageIndexer-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qrImageIndexer-0.7.3/PKG-INFO` & `qrImageIndexer-0.7.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qrImageIndexer
-Version: 0.7.3
+Version: 0.7.4
 Summary: Tool for indexing images with QR codes
 Author-email: Jonathan Pecar <jonathan.pecar@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Jonathan Pecar
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -71,15 +71,15 @@
 As the tool is targetting images, any files which are not images will be copied into the
 directory `non_image_files/` under the target output directory.
 #### Files Before Index Image
 If there are images which appear before the first QR-containing image will be copied into
 the directory `unsorted/`.
 
 ### Example Input Images
-![Example directory of input images](docs\images\example_sort.png)
+![Example directory of input images](https://user-images.githubusercontent.com/65805625/192940631-be5f5bc7-c23e-4eed-8610-0a8752c1f950.png)
 
 ## Installation
 ---
 
 The package is available on PyPi and can be installed with the following command:
 
 ```pip install qrImageIndexer```
@@ -91,19 +91,19 @@
 ---
 
 ### Tool Command Line Arguments
 ---
 
 To use the tool run the command:
 
-```python -m qr_image_indexer```
+```python -m qrImageIndexer```
 
 Command line useage is as per below:
 ```
-usage: __main__.py [-h] [-g INPUT_TEXT_FILE OUTPUT_PDF | -s INPUT_DIR OUTPUT_DIR] [--pdf-type SORT_TYPE] [-q] [-r] [-p STRING_PREFIX] [-v]
+usage: qrImageIndexer [-h] [-g INPUT_TEXT_FILE OUTPUT_PDF | -s INPUT_DIR OUTPUT_DIR] [--pdf-type SORT_TYPE] [-q] [-r] [-p STRING_PREFIX] [-v]
 
 options:
   -h, --help            show this help message and exit
   -g INPUT_TEXT_FILE OUTPUT_PDF, --generate-pdf INPUT_TEXT_FILE OUTPUT_PDF
                         Generate a PDF of QR codes from a given text file. Specify
   -s INPUT_DIR OUTPUT_DIR, --sort-photos INPUT_DIR OUTPUT_DIR
                         Sort photos based on QR codes found in photos. Once a QR code is found all photos will be sorted into the directory indicated by the code until subsequent codes found
@@ -126,15 +126,15 @@
 
 #### PDF Format
 ---
 
 For ease of use it is recommended to use the `--pdf-type sliceable` option, which will allow, when printed single-sided, for the QR codes to be easily sliced
 and stacked for use in-order.
 
-![](docs/images/example_linear_sliceable.png)
+![Demonstration of Linear Slicing](https://user-images.githubusercontent.com/65805625/192940658-6ce1837c-b5d2-46ab-bb6c-876ee1d9eb53.png)
 
 #### File Format
 ---
 
 Expected input file format is as a tab indented list. Each level of indentation is considered a child tested below the preceeding level. When photos are sorted
 these nested elements will form the file paths. **Additional file formats could easily be added
 and may be a good first issue for anyone who wishes to contribute.** An example input file is shown below:
@@ -169,21 +169,21 @@
 Using the option `-v` for any operations will provide verbose status output to the command line.
 
 #### Generating PDF Document
 ---
 
 Assuming that the above demo file is saved as `demo.txt` the following command would generate a PDF with repeated headings and qr codes for each line in a sliceable format, with the prefix `{image}`:
 
-```python -m qr_image_indexer -g demo.txt demo.pdf -r -q --pdf-type sliceable -p "{image}"```
+```python -m qrImageIndexer -g demo.txt demo.pdf -r -q --pdf-type sliceable -p "{image}"```
 
 #### Sorting Images
 ---
 
 After taking photos, these images could then be sorted into a folder called `outputs\` from a folder called `inputs\` as shown below:
 
-```python -m qr_image_indexer -s inputs\ outputs\ -p "{image}"```
+```python -m qrImageIndexer -s inputs\ outputs\ -p "{image}"```
 
 ## Future Features
 ---
 
 Currently the module is command line only. In future this will be expanded to include a GUI
 which will simplify the generation of QR codes and the scanning of images for users.
```

### Comparing `qrImageIndexer-0.7.3/README.md` & `qrImageIndexer-0.7.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 As the tool is targetting images, any files which are not images will be copied into the
 directory `non_image_files/` under the target output directory.
 #### Files Before Index Image
 If there are images which appear before the first QR-containing image will be copied into
 the directory `unsorted/`.
 
 ### Example Input Images
-![Example directory of input images](docs\images\example_sort.png)
+![Example directory of input images](https://user-images.githubusercontent.com/65805625/192940631-be5f5bc7-c23e-4eed-8610-0a8752c1f950.png)
 
 ## Installation
 ---
 
 The package is available on PyPi and can be installed with the following command:
 
 ```pip install qrImageIndexer```
@@ -54,19 +54,19 @@
 ---
 
 ### Tool Command Line Arguments
 ---
 
 To use the tool run the command:
 
-```python -m qr_image_indexer```
+```python -m qrImageIndexer```
 
 Command line useage is as per below:
 ```
-usage: __main__.py [-h] [-g INPUT_TEXT_FILE OUTPUT_PDF | -s INPUT_DIR OUTPUT_DIR] [--pdf-type SORT_TYPE] [-q] [-r] [-p STRING_PREFIX] [-v]
+usage: qrImageIndexer [-h] [-g INPUT_TEXT_FILE OUTPUT_PDF | -s INPUT_DIR OUTPUT_DIR] [--pdf-type SORT_TYPE] [-q] [-r] [-p STRING_PREFIX] [-v]
 
 options:
   -h, --help            show this help message and exit
   -g INPUT_TEXT_FILE OUTPUT_PDF, --generate-pdf INPUT_TEXT_FILE OUTPUT_PDF
                         Generate a PDF of QR codes from a given text file. Specify
   -s INPUT_DIR OUTPUT_DIR, --sort-photos INPUT_DIR OUTPUT_DIR
                         Sort photos based on QR codes found in photos. Once a QR code is found all photos will be sorted into the directory indicated by the code until subsequent codes found
@@ -89,15 +89,15 @@
 
 #### PDF Format
 ---
 
 For ease of use it is recommended to use the `--pdf-type sliceable` option, which will allow, when printed single-sided, for the QR codes to be easily sliced
 and stacked for use in-order.
 
-![](docs/images/example_linear_sliceable.png)
+![Demonstration of Linear Slicing](https://user-images.githubusercontent.com/65805625/192940658-6ce1837c-b5d2-46ab-bb6c-876ee1d9eb53.png)
 
 #### File Format
 ---
 
 Expected input file format is as a tab indented list. Each level of indentation is considered a child tested below the preceeding level. When photos are sorted
 these nested elements will form the file paths. **Additional file formats could easily be added
 and may be a good first issue for anyone who wishes to contribute.** An example input file is shown below:
@@ -132,21 +132,21 @@
 Using the option `-v` for any operations will provide verbose status output to the command line.
 
 #### Generating PDF Document
 ---
 
 Assuming that the above demo file is saved as `demo.txt` the following command would generate a PDF with repeated headings and qr codes for each line in a sliceable format, with the prefix `{image}`:
 
-```python -m qr_image_indexer -g demo.txt demo.pdf -r -q --pdf-type sliceable -p "{image}"```
+```python -m qrImageIndexer -g demo.txt demo.pdf -r -q --pdf-type sliceable -p "{image}"```
 
 #### Sorting Images
 ---
 
 After taking photos, these images could then be sorted into a folder called `outputs\` from a folder called `inputs\` as shown below:
 
-```python -m qr_image_indexer -s inputs\ outputs\ -p "{image}"```
+```python -m qrImageIndexer -s inputs\ outputs\ -p "{image}"```
 
 ## Future Features
 ---
 
 Currently the module is command line only. In future this will be expanded to include a GUI
 which will simplify the generation of QR codes and the scanning of images for users.
```

### Comparing `qrImageIndexer-0.7.3/pyproject.toml` & `qrImageIndexer-0.7.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "qrImageIndexer"
-version = "0.7.3"
+version = "0.7.4"
 description = "Tool for indexing images with QR codes"
 readme = "README.md"
 authors = [{name = "Jonathan Pecar", email = "jonathan.pecar@gmail.com"}]
 license = { file = "LICENSE"}
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -27,15 +27,15 @@
 requires-python = ">=3.6"
 [project.optional-dependencies]
 dev = ["pytest", "bumpver", "setuptools"]
 
 [project.urls]
 Homepage = "https://github.com/jonpecar/qrCodeImageSorter"
 [tool.bumpver]
-current_version = "0.7.3"
+current_version = "0.7.4"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `qrImageIndexer-0.7.3/qrImageIndexer/__main__.py` & `qrImageIndexer-0.7.4/qrImageIndexer/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,14 +23,17 @@
     # parser.add_argument('-b', '--use-binarization', help='Search for QR codes with binarized images. May take up to twice as long but can sometimes find QR codes that would otherwise not be detected.',
     #     action='store_true')
 
     parser.add_argument('-p', '--string-prefix', help='Specify a prefix for use in the generated QR codes to differentiate from codes that might also end up in photos')
 
     parser.add_argument('-v', '--verbose', help='Turn progress text to terminal on or off',
             action='store_true')
+    
+    parser.add_argument('-d', '--datestamp', help='Use file modified time to sort the incoming images instead of file name',
+            action='store_true')
 
     args = parser.parse_args()
 
     string_header = ''
     if args.string_prefix:
         string_header = args.string_prefix
 
@@ -61,15 +64,15 @@
     if args.sort_photos:
         input = args.sort_photos[0]
         output = args.sort_photos[1]
 
         if verbose:
             print('Sorting from: ' + input + ', to : ' + output)
 
-        found_dirs = sort_directory(input, output, string_header, args.verbose, True)
+        found_dirs = sort_directory(input, output, string_header, args.verbose, True, order_by_date=args.datestamp)
 
         if verbose:
             print('Found directories from images:')
             [print(x) for x in found_dirs]
```

### Comparing `qrImageIndexer-0.7.3/qrImageIndexer/generate_qr_wrapper.py` & `qrImageIndexer-0.7.4/qrImageIndexer/generate_qr_wrapper.py`

 * *Files identical despite different names*

### Comparing `qrImageIndexer-0.7.3/qrImageIndexer/photo_sorter.py` & `qrImageIndexer-0.7.4/qrImageIndexer/photo_sorter.py`

 * *Files 4% similar despite different names*

```diff
@@ -183,15 +183,20 @@
     images = os.listdir(input_dir)
     image_paths = [os.path.join(input_dir, x) for x in images]
     
     image_paths = remove_non_images(image_paths, verbose, non_image_dir)
     return image_paths
 
 
-def sort_directory(input_dir : str, output_dir : str, string_header : str = '', verbose : bool = False, binarization : bool = False) -> List[str]:
+def sort_directory(input_dir : str,
+                   output_dir : str, 
+                   string_header : str = '', 
+                   verbose : bool = False, 
+                   binarization : bool = False, 
+                   order_by_date : bool = False) -> List[str]:
     """
         Takes all images in a directory and sorts them by QR codes found in the images. Any
         images which are found before the first QR code will go into an "unsorted" folder in the directory.
 
         Parameters:
             input_dir: input directory containing photos as a string
             output_dir: target directory for photos, will be created if does not exist
@@ -211,20 +216,24 @@
 
     if verbose:
         print('Scanning images for QR codes')
     results = get_qr_for_files(image_paths, string_header=string_header, verbose=verbose, binarization=binarization)
     os.makedirs(output_dir, exist_ok=True)
 
 
-    found_directories = sort_directory_exisitng_results(results, input_dir, output_dir, verbose)
+    found_directories = sort_directory_exisitng_results(results, input_dir, output_dir, verbose, order_by_date=order_by_date)
 
     found_directories.sort()
     return found_directories
 
-def sort_directory_exisitng_results(results : Dict[str, str], input_dir : str, output_dir : str, verbose : bool = False) -> List[str]:
+def sort_directory_exisitng_results(results : Dict[str, str], 
+                                    input_dir : str, 
+                                    output_dir : str, 
+                                    verbose : bool = False,
+                                    order_by_date : bool = False) -> List[str]:
     """
         Takes results from the QR code scanning and uses that information to sort the images. Function separated from
         above for better integration with GUI code.
 
         Parameters:
             results: Dictionary of results including image path and QR code result
             input_dir: input directory containing photos as string
@@ -234,14 +243,19 @@
         Returns:
             List[str] of all paths found in QR codes
     """
     found_directories = []
     non_image_dir = os.path.join(output_dir, 'non_image_files')
     image_paths = get_image_paths(input_dir, non_image_dir, verbose)
 
+    if order_by_date:
+        image_paths.sort(key=lambda path: os.path.getmtime(path))
+    else:
+        image_paths.sort()
+
     if verbose:
         print('Sorting image files')
     current_path = os.path.join(output_dir, 'unsorted')
     for image_path in tqdm.tqdm(image_paths) if verbose else image_paths:
         _, image = os.path.split(image_path)
         qr_string = ''
         if image_path in results:
```

### Comparing `qrImageIndexer-0.7.3/qrImageIndexer/qr_generator.py` & `qrImageIndexer-0.7.4/qrImageIndexer/qr_generator.py`

 * *Files identical despite different names*

### Comparing `qrImageIndexer-0.7.3/qrImageIndexer/write_pdf_fpf2.py` & `qrImageIndexer-0.7.4/qrImageIndexer/write_pdf_fpf2.py`

 * *Files identical despite different names*

### Comparing `qrImageIndexer-0.7.3/qrImageIndexer.egg-info/PKG-INFO` & `qrImageIndexer-0.7.4/qrImageIndexer.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qrImageIndexer
-Version: 0.7.3
+Version: 0.7.4
 Summary: Tool for indexing images with QR codes
 Author-email: Jonathan Pecar <jonathan.pecar@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Jonathan Pecar
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -71,15 +71,15 @@
 As the tool is targetting images, any files which are not images will be copied into the
 directory `non_image_files/` under the target output directory.
 #### Files Before Index Image
 If there are images which appear before the first QR-containing image will be copied into
 the directory `unsorted/`.
 
 ### Example Input Images
-![Example directory of input images](docs\images\example_sort.png)
+![Example directory of input images](https://user-images.githubusercontent.com/65805625/192940631-be5f5bc7-c23e-4eed-8610-0a8752c1f950.png)
 
 ## Installation
 ---
 
 The package is available on PyPi and can be installed with the following command:
 
 ```pip install qrImageIndexer```
@@ -91,19 +91,19 @@
 ---
 
 ### Tool Command Line Arguments
 ---
 
 To use the tool run the command:
 
-```python -m qr_image_indexer```
+```python -m qrImageIndexer```
 
 Command line useage is as per below:
 ```
-usage: __main__.py [-h] [-g INPUT_TEXT_FILE OUTPUT_PDF | -s INPUT_DIR OUTPUT_DIR] [--pdf-type SORT_TYPE] [-q] [-r] [-p STRING_PREFIX] [-v]
+usage: qrImageIndexer [-h] [-g INPUT_TEXT_FILE OUTPUT_PDF | -s INPUT_DIR OUTPUT_DIR] [--pdf-type SORT_TYPE] [-q] [-r] [-p STRING_PREFIX] [-v]
 
 options:
   -h, --help            show this help message and exit
   -g INPUT_TEXT_FILE OUTPUT_PDF, --generate-pdf INPUT_TEXT_FILE OUTPUT_PDF
                         Generate a PDF of QR codes from a given text file. Specify
   -s INPUT_DIR OUTPUT_DIR, --sort-photos INPUT_DIR OUTPUT_DIR
                         Sort photos based on QR codes found in photos. Once a QR code is found all photos will be sorted into the directory indicated by the code until subsequent codes found
@@ -126,15 +126,15 @@
 
 #### PDF Format
 ---
 
 For ease of use it is recommended to use the `--pdf-type sliceable` option, which will allow, when printed single-sided, for the QR codes to be easily sliced
 and stacked for use in-order.
 
-![](docs/images/example_linear_sliceable.png)
+![Demonstration of Linear Slicing](https://user-images.githubusercontent.com/65805625/192940658-6ce1837c-b5d2-46ab-bb6c-876ee1d9eb53.png)
 
 #### File Format
 ---
 
 Expected input file format is as a tab indented list. Each level of indentation is considered a child tested below the preceeding level. When photos are sorted
 these nested elements will form the file paths. **Additional file formats could easily be added
 and may be a good first issue for anyone who wishes to contribute.** An example input file is shown below:
@@ -169,21 +169,21 @@
 Using the option `-v` for any operations will provide verbose status output to the command line.
 
 #### Generating PDF Document
 ---
 
 Assuming that the above demo file is saved as `demo.txt` the following command would generate a PDF with repeated headings and qr codes for each line in a sliceable format, with the prefix `{image}`:
 
-```python -m qr_image_indexer -g demo.txt demo.pdf -r -q --pdf-type sliceable -p "{image}"```
+```python -m qrImageIndexer -g demo.txt demo.pdf -r -q --pdf-type sliceable -p "{image}"```
 
 #### Sorting Images
 ---
 
 After taking photos, these images could then be sorted into a folder called `outputs\` from a folder called `inputs\` as shown below:
 
-```python -m qr_image_indexer -s inputs\ outputs\ -p "{image}"```
+```python -m qrImageIndexer -s inputs\ outputs\ -p "{image}"```
 
 ## Future Features
 ---
 
 Currently the module is command line only. In future this will be expanded to include a GUI
 which will simplify the generation of QR codes and the scanning of images for users.
```

### Comparing `qrImageIndexer-0.7.3/qrImageIndexer.egg-info/SOURCES.txt` & `qrImageIndexer-0.7.4/qrImageIndexer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qrImageIndexer-0.7.3/test/test_pdf_build_fpdf2.py` & `qrImageIndexer-0.7.4/test/test_pdf_build_fpdf2.py`

 * *Files identical despite different names*

### Comparing `qrImageIndexer-0.7.3/test/test_photo_sorter.py` & `qrImageIndexer-0.7.4/test/test_photo_sorter.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from os import listdir
 from qrImageIndexer import photo_sorter, qr_generator
 import pathlib
 import os
+import time
 from typing import Dict
+from PIL import Image, ImageMode
 
 def generate_image(tmp_path : pathlib.Path, string : str, filename : str = 'test') -> str:
     '''
         Generates a temporary image and returns the path to the image
         as a string.
 
         Arguments:
@@ -136,21 +138,57 @@
     qr_strings = [r'Test1\subTest', r'Test1', r'Test2', r'Test?']
     inputs = tmp_path/'inputs'
     outputs = tmp_path/'outputs'
     outputs.mkdir()
     inputs.mkdir()
     for i in range(len(qr_strings)):
         image = qr_generator.build_qr(qr_strings[i])
-        image.save(inputs / (str(i) + '.png'))
+        image.save(inputs / f'{i}_a.png')
 
+        blank_image = Image.new('RGB', (100,100))
+        blank_image.save(inputs / f'{i}_b.png')
 
     found_dirs = photo_sorter.sort_directory(inputs.as_posix(), outputs.as_posix())
 
     assert found_dirs == [r'Test1', r'Test1\subTest', r'Test2', r'Test_']
 
     for i in range(len(qr_strings)):
         path = outputs/photo_sorter.sanitise_path(qr_strings[i])
         filecount = 0
         for filename in os.listdir(path.as_posix()):
             if os.path.isfile(path/filename): filecount += 1
-        assert filecount == 1
-        assert os.listdir(path.as_posix())[0] == (str(i) + '.png')
+        assert filecount == 2
+        assert f'{i}_a.png' in os.listdir(path.as_posix())
+        assert f'{i}_b.png' in os.listdir(path.as_posix())
+
+def test_qr_sorting_by_date(tmp_path : pathlib.Path):
+    qr_strings = [r'Test1\subTest', r'Test1', r'Test2', r'Test?']
+    inputs = tmp_path/'inputs'
+    outputs = tmp_path/'outputs'
+    outputs.mkdir()
+    inputs.mkdir()
+    for i in range(len(qr_strings)):
+        image = qr_generator.build_qr(qr_strings[i])
+        image.save(inputs / (str(i) + '.png'))
+
+        time.sleep(0.01)
+        #Need to make sure it doesn't write too fast or they can have the same timestamp
+
+        blank_image = Image.new('RGB', (100,100))
+        blank_image.save(inputs / f'#{i}.png')
+
+        time.sleep(0.01)
+
+
+    found_dirs = photo_sorter.sort_directory(inputs.as_posix(), outputs.as_posix(), order_by_date=True)
+
+    assert found_dirs == [r'Test1', r'Test1\subTest', r'Test2', r'Test_']
+
+    for i in range(len(qr_strings)):
+        path = outputs/photo_sorter.sanitise_path(qr_strings[i])
+        filecount = 0
+        for filename in os.listdir(path.as_posix()):
+            if os.path.isfile(path/filename): filecount += 1
+        assert filecount == 2
+        assert (str(i) + '.png') in os.listdir(path.as_posix())
+        assert f'#{i}.png' in os.listdir(path.as_posix())
+
```

### Comparing `qrImageIndexer-0.7.3/test/test_qr_generator.py` & `qrImageIndexer-0.7.4/test/test_qr_generator.py`

 * *Files identical despite different names*

### Comparing `qrImageIndexer-0.7.3/test/test_qr_pdf_wrapper.py` & `qrImageIndexer-0.7.4/test/test_qr_pdf_wrapper.py`

 * *Files identical despite different names*

