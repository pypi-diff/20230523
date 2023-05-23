# Comparing `tmp/prompt-generator-0.2.1.tar.gz` & `tmp/prompt-generator-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompt-generator-0.2.1.tar", last modified: Sun May 21 18:32:12 2023, max compression
+gzip compressed data, was "prompt-generator-0.3.0.tar", last modified: Tue May 23 18:22:37 2023, max compression
```

## Comparing `prompt-generator-0.2.1.tar` & `prompt-generator-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:32:12.002254 prompt-generator-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-21 18:32:00.000000 prompt-generator-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-05-21 18:32:11.998254 prompt-generator-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-21 18:32:00.000000 prompt-generator-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-21 18:32:00.000000 prompt-generator-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 18:32:12.002254 prompt-generator-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:32:11.998254 prompt-generator-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:32:11.998254 prompt-generator-0.2.1/src/directory_structure/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-21 18:32:00.000000 prompt-generator-0.2.1/src/directory_structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-21 18:32:00.000000 prompt-generator-0.2.1/src/directory_structure/get_directory_structure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:32:11.998254 prompt-generator-0.2.1/src/markdown_parser/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-21 18:32:00.000000 prompt-generator-0.2.1/src/markdown_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-05-21 18:32:00.000000 prompt-generator-0.2.1/src/markdown_parser/parse_md.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:32:11.998254 prompt-generator-0.2.1/src/print_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-21 18:32:00.000000 prompt-generator-0.2.1/src/print_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-21 18:32:00.000000 prompt-generator-0.2.1/src/print_utils/print_color.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-21 18:32:00.000000 prompt-generator-0.2.1/src/print_utils/print_result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:32:11.998254 prompt-generator-0.2.1/src/prompt_generator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-05-21 18:32:11.000000 prompt-generator-0.2.1/src/prompt_generator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-21 18:32:11.000000 prompt-generator-0.2.1/src/prompt_generator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 18:32:11.000000 prompt-generator-0.2.1/src/prompt_generator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-21 18:32:11.000000 prompt-generator-0.2.1/src/prompt_generator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-21 18:32:11.000000 prompt-generator-0.2.1/src/prompt_generator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-21 18:32:11.000000 prompt-generator-0.2.1/src/prompt_generator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:22:37.472587 prompt-generator-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-23 18:22:21.000000 prompt-generator-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-05-23 18:22:37.472587 prompt-generator-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-23 18:22:21.000000 prompt-generator-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-23 18:22:21.000000 prompt-generator-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 18:22:37.472587 prompt-generator-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:22:37.468586 prompt-generator-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:22:37.468586 prompt-generator-0.3.0/src/directory_structure/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-23 18:22:21.000000 prompt-generator-0.3.0/src/directory_structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-23 18:22:21.000000 prompt-generator-0.3.0/src/directory_structure/get_directory_structure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:22:37.468586 prompt-generator-0.3.0/src/docs_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-23 18:22:21.000000 prompt-generator-0.3.0/src/docs_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-23 18:22:21.000000 prompt-generator-0.3.0/src/docs_generator/generate_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:22:37.472587 prompt-generator-0.3.0/src/file_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-23 18:22:21.000000 prompt-generator-0.3.0/src/file_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-23 18:22:21.000000 prompt-generator-0.3.0/src/file_utils/get_code_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-23 18:22:21.000000 prompt-generator-0.3.0/src/file_utils/get_dir_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-23 18:22:21.000000 prompt-generator-0.3.0/src/file_utils/load_gitignore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-23 18:22:21.000000 prompt-generator-0.3.0/src/file_utils/read_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:22:37.472587 prompt-generator-0.3.0/src/input_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-23 18:22:21.000000 prompt-generator-0.3.0/src/input_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-23 18:22:21.000000 prompt-generator-0.3.0/src/input_utils/input_color.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:22:37.472587 prompt-generator-0.3.0/src/markdown_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-23 18:22:21.000000 prompt-generator-0.3.0/src/markdown_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-05-23 18:22:21.000000 prompt-generator-0.3.0/src/markdown_parser/parse_md.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:22:37.472587 prompt-generator-0.3.0/src/print_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-23 18:22:21.000000 prompt-generator-0.3.0/src/print_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-23 18:22:21.000000 prompt-generator-0.3.0/src/print_utils/print_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-23 18:22:21.000000 prompt-generator-0.3.0/src/print_utils/print_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:22:37.472587 prompt-generator-0.3.0/src/prompt_generator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-05-23 18:22:37.000000 prompt-generator-0.3.0/src/prompt_generator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-23 18:22:37.000000 prompt-generator-0.3.0/src/prompt_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 18:22:37.000000 prompt-generator-0.3.0/src/prompt_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-23 18:22:37.000000 prompt-generator-0.3.0/src/prompt_generator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-23 18:22:37.000000 prompt-generator-0.3.0/src/prompt_generator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-23 18:22:37.000000 prompt-generator-0.3.0/src/prompt_generator.egg-info/top_level.txt
```

### Comparing `prompt-generator-0.2.1/LICENSE` & `prompt-generator-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prompt-generator-0.2.1/PKG-INFO` & `prompt-generator-0.3.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompt-generator
-Version: 0.2.1
+Version: 0.3.0
 Summary: Prompt Generator is a flexible and user-friendly package that offers customizable scripts for generating effective and context-aware prompts. These prompts can be used to guide the writing, improvement, and debugging of code.
 Author: Vincenzo Cascone
 License: MIT License
         
         Copyright (c) 2023 Vince
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -44,14 +44,31 @@
 
 ```bash
 pip install prompt-generator
 ```
 
 ## Features
 
+- ### Generate Docs
+
+  This script generates a prompt that can be used to make the AI write documentation
+  for the project. When executed, it will first ask for some info about the project, such as the name, description, root
+  path. Optionally you can provide the path to config files such as pyproject.toml for a python project or
+  package.json for a node project. The same can be done with particularly relevant files. This will allow the AI to have
+  a better understanding of the project and generate more accurate documentation.
+
+  To utilize it, use the following command in your terminal:
+
+    ```bash
+    generate_docs
+    ```
+
+  Upon successful execution, the resultant prompt will be displayed in your terminal and copied to your clipboard for
+  immediate use or future reference.
+
 - ### Markdown Parser
 
   The Markdown Parser is a robust utility specifically designed to parse markdown files. It works by replacing all
   hyperlinks within a Markdown document with the actual content of the linked files. This function proves extremely
   useful if you maintain a collection of prompt files written in Markdown format, and these files contain references to
   other project documents.
```

### Comparing `prompt-generator-0.2.1/README.md` & `prompt-generator-0.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,31 @@
 
 ```bash
 pip install prompt-generator
 ```
 
 ## Features
 
+- ### Generate Docs
+
+  This script generates a prompt that can be used to make the AI write documentation
+  for the project. When executed, it will first ask for some info about the project, such as the name, description, root
+  path. Optionally you can provide the path to config files such as pyproject.toml for a python project or
+  package.json for a node project. The same can be done with particularly relevant files. This will allow the AI to have
+  a better understanding of the project and generate more accurate documentation.
+
+  To utilize it, use the following command in your terminal:
+
+    ```bash
+    generate_docs
+    ```
+
+  Upon successful execution, the resultant prompt will be displayed in your terminal and copied to your clipboard for
+  immediate use or future reference.
+
 - ### Markdown Parser
 
   The Markdown Parser is a robust utility specifically designed to parse markdown files. It works by replacing all
   hyperlinks within a Markdown document with the actual content of the linked files. This function proves extremely
   useful if you maintain a collection of prompt files written in Markdown format, and these files contain references to
   other project documents.
```

### Comparing `prompt-generator-0.2.1/pyproject.toml` & `prompt-generator-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "prompt-generator"
-version = "0.2.1"
+version = "0.3.0"
 description = "Prompt Generator is a flexible and user-friendly package that offers customizable scripts for generating effective and context-aware prompts. These prompts can be used to guide the writing, improvement, and debugging of code."
 readme = "README.md"
 requires-python = ">=3.6"
 authors = [
     { name = "Vincenzo Cascone" },
 ]
 license = { file = "LICENSE" }
@@ -21,11 +21,12 @@
     "pyperclip",
     "pathspec",
 ]
 
 [project.scripts]
 parse_md = "markdown_parser:main"
 get_directory_structure = "directory_structure:main"
+generate_docs = "docs_generator:main"
 
 [project.urls]
 repository = "https://github.com/vincenzocascone/prompt-generator"
```

### Comparing `prompt-generator-0.2.1/src/markdown_parser/parse_md.py` & `prompt-generator-0.3.0/src/markdown_parser/parse_md.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,13 @@
 import argparse
 import os
 import re
 
-from print_utils import print_result, print_color, TerminalColor
-
-
-def read_file(file_path):
-    """Reads a file and returns its content."""
-    try:
-        with open(file_path, 'r', encoding='utf-8') as file:
-            return file.read()
-    except IOError:
-        print_color(f"Failed to open {file_path}", TerminalColor.WARNING)
+from file_utils import read_file, get_code_block
+from print_utils import print_result
 
 
 def parse_links(content, base_path):
     """Parses links within the content."""
     links = re.findall(r'\[(.*?)]\((.*?)\)', content)
 
     for text, file_path in links:
@@ -26,24 +18,23 @@
                 content, text, file_path, full_file_path)
 
     return content
 
 
 def replace_link_with_content(content, text, file_path, full_file_path):
     """Replaces link with its corresponding content."""
-    file_content = read_file(full_file_path)
     _, file_extension = os.path.splitext(full_file_path)
 
     if file_extension == '.md':
         file_content = parse_content(full_file_path)
         content = content.replace(
             f'[{text}]({file_path})', f'{file_content}')
     else:
         content = content.replace(
-            f'[{text}]({file_path})', f'```{file_extension[1:]}\n{file_content}\n```')
+            f'[{text}]({file_path})', get_code_block(full_file_path))
 
     return content
 
 
 def parse_content(md_file_path):
     """Parses a markdown file, replacing links with the content of the linked files."""
     content = read_file(md_file_path)
```

### Comparing `prompt-generator-0.2.1/src/prompt_generator.egg-info/PKG-INFO` & `prompt-generator-0.3.0/src/prompt_generator.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompt-generator
-Version: 0.2.1
+Version: 0.3.0
 Summary: Prompt Generator is a flexible and user-friendly package that offers customizable scripts for generating effective and context-aware prompts. These prompts can be used to guide the writing, improvement, and debugging of code.
 Author: Vincenzo Cascone
 License: MIT License
         
         Copyright (c) 2023 Vince
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -44,14 +44,31 @@
 
 ```bash
 pip install prompt-generator
 ```
 
 ## Features
 
+- ### Generate Docs
+
+  This script generates a prompt that can be used to make the AI write documentation
+  for the project. When executed, it will first ask for some info about the project, such as the name, description, root
+  path. Optionally you can provide the path to config files such as pyproject.toml for a python project or
+  package.json for a node project. The same can be done with particularly relevant files. This will allow the AI to have
+  a better understanding of the project and generate more accurate documentation.
+
+  To utilize it, use the following command in your terminal:
+
+    ```bash
+    generate_docs
+    ```
+
+  Upon successful execution, the resultant prompt will be displayed in your terminal and copied to your clipboard for
+  immediate use or future reference.
+
 - ### Markdown Parser
 
   The Markdown Parser is a robust utility specifically designed to parse markdown files. It works by replacing all
   hyperlinks within a Markdown document with the actual content of the linked files. This function proves extremely
   useful if you maintain a collection of prompt files written in Markdown format, and these files contain references to
   other project documents.
```

