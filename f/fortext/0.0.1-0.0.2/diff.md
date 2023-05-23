# Comparing `tmp/fortext-0.0.1.tar.gz` & `tmp/fortext-0.0.2.tar.gz`

## Comparing `fortext-0.0.1.tar` & `fortext-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 fortext-0.0.1/requirements.txt
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 fortext-0.0.1/src/fortext/__init__.py
--rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 fortext-0.0.1/src/fortext/ansi.py
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 fortext-0.0.1/src/fortext/style.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 fortext-0.0.1/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 fortext-0.0.1/LICENSE
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 fortext-0.0.1/README.md
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 fortext-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 fortext-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 fortext-0.0.2/requirements.txt
+-rw-r--r--   0        0        0     4427 2020-02-02 00:00:00.000000 fortext-0.0.2/img/syntax_highlighting.png
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 fortext-0.0.2/src/fortext/__init__.py
+-rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 fortext-0.0.2/src/fortext/ansi.py
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 fortext-0.0.2/src/fortext/style.py
+-rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 fortext-0.0.2/src/fortext/syntax.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 fortext-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 fortext-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 fortext-0.0.2/README.md
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 fortext-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 fortext-0.0.2/PKG-INFO
```

### Comparing `fortext-0.0.1/src/fortext/ansi.py` & `fortext-0.0.2/src/fortext/ansi.py`

 * *Files identical despite different names*

### Comparing `fortext-0.0.1/src/fortext/style.py` & `fortext-0.0.2/src/fortext/style.py`

 * *Files identical despite different names*

### Comparing `fortext-0.0.1/.gitignore` & `fortext-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `fortext-0.0.1/LICENSE` & `fortext-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fortext-0.0.1/README.md` & `fortext-0.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -4,35 +4,37 @@
 ## Table of Contents
 
 * [Table of Contents](#table-of-contents)
 * [Getting Started](#getting-started)
   * [Prerequisites](#prerequisites)
   * [Installation](#installation)
 * [Usage](#usage)
+  * [Text styling](#text-styling)
+  * [Syntax highlighting](#syntax-highlighting)
 
 
 
 ## Getting Started
 
 ### Prerequisites
 * Install or update the [pip](https://pip.pypa.io/en/stable/) package manager.
   ```sh
   python3 -m pip install --upgrade pip
   ```
 
 * It's also recommended to use a [virtual environment](https://docs.python.org/3/library/venv.html).
   * Linux / MacOS
     ```bash
-    python3 -m venv venv-name
+    python3 -m venv <venv-name>
     source venv/bin/activate
     ```
   * Windows
     ```bash
-    python3 -m venv venv-name
-    venv/Scripts/activate
+    python3 -m venv <venv-name>
+    <venv-name>/Scripts/activate
     ```
 
 ### Installation
 
 Use pip to install `fortext`.
 
 ```bash
@@ -42,18 +44,29 @@
 Install the required dependencies as listed on [requirements.txt](./requirements.txt).
 ```shell
 python3 -m pip install -r requirements.txt
 ```
 
 ## Usage
 
+### Text styling
+
 ```python
 print(style('Hi, human.', fg='#ff0000'))
 print(style('RGB tuple or list also works.', fg=(0, 255, 0)))
 print(style('You can also use predefined colors.', bg=Bg.BLACK))
 print(style('Want to be bold?.', frmt=[Frmt.BOLD]))
 
 print(
     style('Want to go all in?',
           fg='#ff0000', bg=Bg.BLACK,
           frmt=[Frmt.BOLD, Frmt.UNDERLINE, Frmt.ITALIC]))
 ```
+
+### Syntax highlighting
+
+```python
+print(highlight({'somekey': 'somevalue', 'anotherkey': [12.4, True, 23]}))
+```
+Output:
+
+![syntax highlighting example output](./img/syntax_highlighting.png)
```

### Comparing `fortext-0.0.1/pyproject.toml` & `fortext-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fortext"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="4MBL" },
 ]
 description = "Text stylizer for Python. Mainly useful for CLI output."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.11"
```

### Comparing `fortext-0.0.1/PKG-INFO` & `fortext-0.0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortext
-Version: 0.0.1
+Version: 0.0.2
 Summary: Text stylizer for Python. Mainly useful for CLI output.
 Project-URL: Homepage, https://github.com/4MBL/fortext
 Project-URL: Bug Tracker, https://github.com/4MBL/fortext/issues
 Author: 4MBL
 License: MIT License
         
         Copyright (c) 2023 4MBL
@@ -39,35 +39,37 @@
 ## Table of Contents
 
 * [Table of Contents](#table-of-contents)
 * [Getting Started](#getting-started)
   * [Prerequisites](#prerequisites)
   * [Installation](#installation)
 * [Usage](#usage)
+  * [Text styling](#text-styling)
+  * [Syntax highlighting](#syntax-highlighting)
 
 
 
 ## Getting Started
 
 ### Prerequisites
 * Install or update the [pip](https://pip.pypa.io/en/stable/) package manager.
   ```sh
   python3 -m pip install --upgrade pip
   ```
 
 * It's also recommended to use a [virtual environment](https://docs.python.org/3/library/venv.html).
   * Linux / MacOS
     ```bash
-    python3 -m venv venv-name
+    python3 -m venv <venv-name>
     source venv/bin/activate
     ```
   * Windows
     ```bash
-    python3 -m venv venv-name
-    venv/Scripts/activate
+    python3 -m venv <venv-name>
+    <venv-name>/Scripts/activate
     ```
 
 ### Installation
 
 Use pip to install `fortext`.
 
 ```bash
@@ -77,18 +79,29 @@
 Install the required dependencies as listed on [requirements.txt](./requirements.txt).
 ```shell
 python3 -m pip install -r requirements.txt
 ```
 
 ## Usage
 
+### Text styling
+
 ```python
 print(style('Hi, human.', fg='#ff0000'))
 print(style('RGB tuple or list also works.', fg=(0, 255, 0)))
 print(style('You can also use predefined colors.', bg=Bg.BLACK))
 print(style('Want to be bold?.', frmt=[Frmt.BOLD]))
 
 print(
     style('Want to go all in?',
           fg='#ff0000', bg=Bg.BLACK,
           frmt=[Frmt.BOLD, Frmt.UNDERLINE, Frmt.ITALIC]))
 ```
+
+### Syntax highlighting
+
+```python
+print(highlight({'somekey': 'somevalue', 'anotherkey': [12.4, True, 23]}))
+```
+Output:
+
+![syntax highlighting example output](./img/syntax_highlighting.png)
```

