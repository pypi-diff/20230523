# Comparing `tmp/hkkang_utils-0.1.9.tar.gz` & `tmp/hkkang_utils-0.1.90.tar.gz`

## Comparing `hkkang_utils-0.1.9.tar` & `hkkang_utils-0.1.90.tar`

### file list

```diff
@@ -1,18 +1,39 @@
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 hkkang_utils-0.1.9/.vscode/settings.json
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 hkkang_utils-0.1.9/src/hkkang_utils/__init__.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 hkkang_utils-0.1.9/src/hkkang_utils/file.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 hkkang_utils-0.1.9/src/hkkang_utils/list.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 hkkang_utils-0.1.9/src/hkkang_utils/misc.py
--rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 hkkang_utils-0.1.9/src/hkkang_utils/sql.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 hkkang_utils-0.1.9/src/hkkang_utils/string.py
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 hkkang_utils-0.1.9/src/hkkang_utils/tensor.py
--rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 hkkang_utils-0.1.9/tests/test_file.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 hkkang_utils-0.1.9/tests/test_list.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hkkang_utils-0.1.9/tests/test_sql.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 hkkang_utils-0.1.9/tests/test_string.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 hkkang_utils-0.1.9/tests/test_tensor.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 hkkang_utils-0.1.9/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 hkkang_utils-0.1.9/LICENSE
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 hkkang_utils-0.1.9/README.md
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 hkkang_utils-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 hkkang_utils-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 hkkang_utils-0.1.90/.github/workflows/deploy_doc.yml
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 hkkang_utils-0.1.90/.github/workflows/unittest.yml
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 hkkang_utils-0.1.90/.vscode/settings.json
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 hkkang_utils-0.1.90/src/hkkang_utils/__init__.py
+-rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 hkkang_utils-0.1.90/src/hkkang_utils/concurrent.py
+-rw-r--r--   0        0        0     6525 2020-02-02 00:00:00.000000 hkkang_utils-0.1.90/src/hkkang_utils/file.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 hkkang_utils-0.1.90/src/hkkang_utils/io.py
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 hkkang_utils-0.1.90/src/hkkang_utils/list.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 hkkang_utils-0.1.90/src/hkkang_utils/logger.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 hkkang_utils-0.1.90/src/hkkang_utils/metrics.py
+-rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 hkkang_utils-0.1.90/src/hkkang_utils/misc.py
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 hkkang_utils-0.1.90/src/hkkang_utils/ml.py
+-rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 hkkang_utils-0.1.90/src/hkkang_utils/pattern.py
+-rw-r--r--   0        0        0     4669 2020-02-02 00:00:00.000000 hkkang_utils-0.1.90/src/hkkang_utils/pg.py
+-rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 hkkang_utils-0.1.90/src/hkkang_utils/slack.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 hkkang_utils-0.1.90/src/hkkang_utils/socket.py
+-rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 hkkang_utils-0.1.90/src/hkkang_utils/sql.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 hkkang_utils-0.1.90/src/hkkang_utils/string.py
+-rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 hkkang_utils-0.1.90/src/hkkang_utils/tensor.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 hkkang_utils-0.1.90/src/hkkang_utils/testing.py
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 hkkang_utils-0.1.90/src/hkkang_utils/time.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hkkang_utils-0.1.90/tests/__init__.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 hkkang_utils-0.1.90/tests/test_concurrent.py
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 hkkang_utils-0.1.90/tests/test_design.py
+-rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 hkkang_utils-0.1.90/tests/test_file.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 hkkang_utils-0.1.90/tests/test_io.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 hkkang_utils-0.1.90/tests/test_list.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 hkkang_utils-0.1.90/tests/test_metrics.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 hkkang_utils-0.1.90/tests/test_misc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hkkang_utils-0.1.90/tests/test_sql.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 hkkang_utils-0.1.90/tests/test_string.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 hkkang_utils-0.1.90/tests/test_tensor.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 hkkang_utils-0.1.90/tests/test_testing.py
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 hkkang_utils-0.1.90/tests/test_time.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 hkkang_utils-0.1.90/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 hkkang_utils-0.1.90/LICENSE
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 hkkang_utils-0.1.90/README.md
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 hkkang_utils-0.1.90/pyproject.toml
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 hkkang_utils-0.1.90/PKG-INFO
```

### Comparing `hkkang_utils-0.1.9/src/hkkang_utils/sql.py` & `hkkang_utils-0.1.90/src/hkkang_utils/sql.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.9/tests/test_file.py` & `hkkang_utils-0.1.90/tests/test_file.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,73 +8,131 @@
 
 
 class testing_environment:
     def __init__(self, dir_name=None, num_files=10, extension=".txt"):
         self.dir_name = dir_name if dir_name else self._generate_random_string()
         self.num_files = num_files
         self.extension = extension
-        self.file_names = [self._generate_random_string()+extension for _ in range(num_files)]
-    
+        self.file_names = [
+            self._generate_random_string() + extension for _ in range(num_files)
+        ]
+
     @property
     def dummpy_dict_data(self):
         return {"key": "value"}
+
     @property
     def file_paths(self):
         return [os.path.join(self.dir_name, file_name) for file_name in self.file_names]
-    
+
     # Helper functions
     def _generate_random_string(self, num_chars=10):
         letters = string.ascii_lowercase
-        return ''.join(random.choice(letters) for i in range(num_chars))
-    
+        return "".join(random.choice(letters) for i in range(num_chars))
+
     # Handle directory
     def create_directory(self):
         os.mkdir(self.dir_name)
-        
+
     def remove_directory(self):
         os.rmdir(self.dir_name)
-    
+
     # Handle files
     def create_random_files(self):
         for file_name in self.file_names:
             file_path = os.path.join(self.dir_name, file_name)
-            with open(file_path, 'w') as f:
+            with open(file_path, "w") as f:
                 json.dump(self.dummpy_dict_data, f)
-    
+
     def remove_random_files(self):
         for file_name in self.file_names:
             file_path = os.path.join(self.dir_name, file_name)
             os.remove(file_path)
-    
+
     # Magic methods
     def __enter__(self):
         self.create_directory()
         self.create_random_files()
         return self
-    
+
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.remove_random_files()
         self.remove_directory()
 
 
 class Test_file_utils(unittest.TestCase):
     def __init__(self, *args, **kwargs):
         super(Test_file_utils, self).__init__(*args, **kwargs)
-        
+
     def test_get_files_in_directory(self):
         with testing_environment() as env:
-            retrieved_file_paths = file_utils.get_files_in_directory(env.dir_name)
+            retrieved_file_paths = file_utils.get_files_in_directory(
+                env.dir_name, return_with_dir=True
+            )
             self.assertEqual(len(retrieved_file_paths), env.num_files)
             self.assertSetEqual(set(retrieved_file_paths), set(env.file_paths))
-    
+
     def test_read_json_file(self):
         with testing_environment() as env:
             file_path = os.path.join(env.dir_name, env.file_names[0])
             json_data = file_utils.read_json_file(file_path)
             self.assertEqual(json_data, env.dummpy_dict_data)
-    
+
     def test_get_files_in_all_sub_directories(self):
         pass
 
+    def test_yaml_file_functions(self):
+        yaml_path = "test.yaml"
+        dict_object = {"A": "a", "B": {"C": "c", "D": "d", "E": "e"}}
+        # Write yaml file
+        file_utils.write_yaml_file(dict_object, yaml_path)
+
+        # Read in yaml file
+        yaml_object = file_utils.read_yaml_file(yaml_path)
+
+        # Check if the two objects are the same
+        self.assertEqual(dict_object, yaml_object)
+
+        # Delete yaml file
+        os.remove(yaml_path)
+
+    def test_csv_file_functions(self):
+        header = ["A", "B", "C"]
+        data = [["1", "2", "3"], ["4", "5", "6"]]
+        csv_object_original = [dict(zip(header, row)) for row in data]
+        csv_path = "test.csv"
+        # Write csv file
+        file_utils.write_csv_file(csv_object_original, csv_path)
+
+        # Read in csv file
+        csv_object = file_utils.read_csv_file(csv_path)
+
+        # Check if the two objects are the same
+        self.assertEqual(csv_object_original, csv_object)
+
+        # Delete csv file
+        os.remove(csv_path)
+
+    def test_csv_file_functions_with_process_row(self):
+        def process_row(row):
+            """Convert string to int"""
+            return [int(x) for x in row]
+
+        header = ["A", "B", "C"]
+        data = [[1, 2, 3], [4, 5, 6]]
+        csv_object_original = [dict(zip(header, row)) for row in data]
+        csv_path = "test.csv"
+        # Write csv file
+        file_utils.write_csv_file(csv_object_original, csv_path)
+
+        # Read in csv file
+        csv_object = file_utils.read_csv_file(csv_path, process_row_func=process_row)
+
+        # Check if the two objects are the same
+        self.assertEqual(csv_object_original, csv_object)
+
+        # Delete csv file
+        os.remove(csv_path)
+
 
 if __name__ == "__main__":
-    unittest.main()
+    unittest.main()
```

### Comparing `hkkang_utils-0.1.9/.gitignore` & `hkkang_utils-0.1.90/.gitignore`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.9/LICENSE` & `hkkang_utils-0.1.90/LICENSE`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.9/pyproject.toml` & `hkkang_utils-0.1.90/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "hkkang_utils"
-version = "0.1.9"
+version = "0.1.90"
 authors = [{name="Hyukkyu Kang", email="hyukkyukang@gmail.com"}]
 description = "A collection of useful util functions"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies=[
-    "nltk>=3.7",
-    "numpy>=1.23",
-    "torch>=1.13",
-    "pglast>=3.17"
+    "attrs",
+    "python-dotenv",
+    "nltk",
+    "numpy",
+    "omegaconf",
+    "pglast",
+    "psycopg[binary,pool]",
+    "slack_sdk",
+    "torch",
+    "ujson"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/hyukkyukang/python_utils"
-"Bug Tracker" = "https://github.com/hyukkyukang/python_utils/issues"
+"Bug Tracker" = "https://github.com/hyukkyukang/python_utils/issues"
```

