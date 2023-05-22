# Comparing `tmp/fukkatsu-0.0.1.tar.gz` & `tmp/fukkatsu-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fukkatsu-0.0.1.tar", last modified: Thu May 18 15:23:34 2023, max compression
+gzip compressed data, was "fukkatsu-0.0.2.tar", last modified: Mon May 22 22:35:32 2023, max compression
```

## Comparing `fukkatsu-0.0.1.tar` & `fukkatsu-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 15:23:34.950851 fukkatsu-0.0.1/
--rw-rw-rw-   0        0        0      110 2023-05-18 14:26:28.000000 fukkatsu-0.0.1/CHANGELOG.md
--rw-rw-rw-   0        0        0     1089 2023-04-28 00:39:24.000000 fukkatsu-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       58 2022-10-31 01:25:26.000000 fukkatsu-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     8460 2023-05-18 15:23:34.942798 fukkatsu-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     7819 2023-05-18 15:09:15.000000 fukkatsu-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 15:23:34.868578 fukkatsu-0.0.1/fukkatsu/
--rw-rw-rw-   0        0        0     3977 2023-05-18 15:09:53.000000 fukkatsu-0.0.1/fukkatsu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 15:23:34.915498 fukkatsu-0.0.1/fukkatsu/memory/
--rw-rw-rw-   0        0        0       73 2023-04-29 00:45:59.000000 fukkatsu-0.0.1/fukkatsu/memory/__init__.py
--rw-rw-rw-   0        0        0       22 2023-04-29 00:22:51.000000 fukkatsu-0.0.1/fukkatsu/memory/long.py
--rw-rw-rw-   0        0        0       23 2023-04-29 00:47:35.000000 fukkatsu-0.0.1/fukkatsu/memory/short.py
-drwxrwxrwx   0        0        0        0 2023-05-18 15:23:34.938222 fukkatsu-0.0.1/fukkatsu/utils/
--rw-rw-rw-   0        0        0      110 2023-05-18 05:17:09.000000 fukkatsu-0.0.1/fukkatsu/utils/__init__.py
--rw-rw-rw-   0        0        0     1013 2023-05-17 19:31:17.000000 fukkatsu-0.0.1/fukkatsu/utils/helper.py
--rw-rw-rw-   0        0        0     1459 2023-05-18 05:17:11.000000 fukkatsu-0.0.1/fukkatsu/utils/medic.py
--rw-rw-rw-   0        0        0      864 2023-05-18 05:17:09.000000 fukkatsu-0.0.1/fukkatsu/utils/prompt.py
-drwxrwxrwx   0        0        0        0 2023-05-18 15:23:34.899870 fukkatsu-0.0.1/fukkatsu.egg-info/
--rw-rw-rw-   0        0        0     8460 2023-05-18 15:23:34.000000 fukkatsu-0.0.1/fukkatsu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      409 2023-05-18 15:23:34.000000 fukkatsu-0.0.1/fukkatsu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 15:23:34.000000 fukkatsu-0.0.1/fukkatsu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-05-18 15:23:34.000000 fukkatsu-0.0.1/fukkatsu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-18 15:23:34.000000 fukkatsu-0.0.1/fukkatsu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 15:23:34.958827 fukkatsu-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1086 2023-05-18 05:36:01.000000 fukkatsu-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 22:35:32.320587 fukkatsu-0.0.2/
+-rw-rw-rw-   0        0        0      377 2023-05-22 21:56:00.000000 fukkatsu-0.0.2/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1089 2023-04-28 00:39:24.000000 fukkatsu-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       58 2022-10-31 01:25:26.000000 fukkatsu-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     9618 2023-05-22 22:35:32.304972 fukkatsu-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8977 2023-05-22 22:17:18.000000 fukkatsu-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 22:35:32.195587 fukkatsu-0.0.2/fukkatsu/
+-rw-rw-rw-   0        0        0     6790 2023-05-22 22:11:23.000000 fukkatsu-0.0.2/fukkatsu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 22:35:32.258082 fukkatsu-0.0.2/fukkatsu/memory/
+-rw-rw-rw-   0        0        0       75 2023-05-20 04:07:03.000000 fukkatsu-0.0.2/fukkatsu/memory/__init__.py
+-rw-rw-rw-   0        0        0      663 2023-05-20 04:07:01.000000 fukkatsu-0.0.2/fukkatsu/memory/manage.py
+-rw-rw-rw-   0        0        0       23 2023-05-20 04:07:01.000000 fukkatsu-0.0.2/fukkatsu/memory/short.py
+drwxrwxrwx   0        0        0        0 2023-05-22 22:35:32.289340 fukkatsu-0.0.2/fukkatsu/utils/
+-rw-rw-rw-   0        0        0      110 2023-05-18 05:17:09.000000 fukkatsu-0.0.2/fukkatsu/utils/__init__.py
+-rw-rw-rw-   0        0        0     2573 2023-05-22 21:23:31.000000 fukkatsu-0.0.2/fukkatsu/utils/helper.py
+-rw-rw-rw-   0        0        0     2241 2023-05-22 22:11:23.000000 fukkatsu-0.0.2/fukkatsu/utils/medic.py
+-rw-rw-rw-   0        0        0     1583 2023-05-20 04:08:40.000000 fukkatsu-0.0.2/fukkatsu/utils/prompt.py
+drwxrwxrwx   0        0        0        0 2023-05-22 22:35:32.242463 fukkatsu-0.0.2/fukkatsu.egg-info/
+-rw-rw-rw-   0        0        0     9618 2023-05-22 22:35:31.000000 fukkatsu-0.0.2/fukkatsu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      411 2023-05-22 22:35:31.000000 fukkatsu-0.0.2/fukkatsu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 22:35:31.000000 fukkatsu-0.0.2/fukkatsu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-05-22 22:35:31.000000 fukkatsu-0.0.2/fukkatsu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-22 22:35:31.000000 fukkatsu-0.0.2/fukkatsu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 22:35:32.320587 fukkatsu-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1086 2023-05-19 01:33:19.000000 fukkatsu-0.0.2/setup.py
```

### Comparing `fukkatsu-0.0.1/LICENSE` & `fukkatsu-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fukkatsu-0.0.1/PKG-INFO` & `fukkatsu-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fukkatsu
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python library for runtime LLM supported code corrections.
 Home-page: https://github.com/maxmekiska/fukkatsu
 Author: Maximilian Mekiska
 Author-email: maxmekiska@gmail.com
 Keywords: machinelearning,llm,runtime,codecorrection
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -45,14 +45,15 @@
 
 
 Here is a representation of what I am trying to do: https://giphy.com/gifs/tire-kNRqJCLOe6ri8/fullscreen 
 
 
 This concept currently only applies to interpreted languages such as Python and not to compiled languages such as C++. The very nature of interpreted languages allows us to dynamically change the code during runtime.
 
+Furthermore, fukkatsu introduces a method to enhance ordinary functions with the power of LLMs. By decorating ordinary functions with natural language prompts, they can now dynamically adapt to unforeseen inputs.
 
 ## MVP
 
 <details>
   <summary>Expand</summary>
   <br>
 
@@ -209,7 +210,31 @@
 ```
 
 ```
 1002
 1002
 ```
 </details>
+
+
+## fukkatsu 0.0.2
+
+<details>
+  <summary>Expand</summary>
+  <br>
+
+The `mutate` decorator introduces a new way to enhance ordinary functions dynamically via the power of LLMs, enabling them to adapt to specific inputs. It provides users with the ability to extend the capabilities of functions through natural language prompts. Additionally, the decorator can be further extended using the `resurrect` decorator. The `mutate` decorator enables users to program and account for cases that are challenging or impossible to anticipate.
+
+```python
+@resurrect(lives=1)
+@mutate(request= "Check the inputs closely. Given the inputs, make sure that the function is able to handle different formats if neccessary")
+def my_mutated_function(file_path: str) -> pd.DataFrame():
+    """
+    function to read files and output a dataframes.
+    """
+    pd.read_csv(file_path)
+    
+my_mutated_function("test_file.xlsx")
+```
+
+
+</details>
```

### Comparing `fukkatsu-0.0.1/README.md` & `fukkatsu-0.0.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
 
 Here is a representation of what I am trying to do: https://giphy.com/gifs/tire-kNRqJCLOe6ri8/fullscreen 
 
 
 This concept currently only applies to interpreted languages such as Python and not to compiled languages such as C++. The very nature of interpreted languages allows us to dynamically change the code during runtime.
 
+Furthermore, fukkatsu introduces a method to enhance ordinary functions with the power of LLMs. By decorating ordinary functions with natural language prompts, they can now dynamically adapt to unforeseen inputs.
 
 ## MVP
 
 <details>
   <summary>Expand</summary>
   <br>
 
@@ -192,8 +193,32 @@
         return result + 1000
 ```
 
 ```
 1002
 1002
 ```
+</details>
+
+
+## fukkatsu 0.0.2
+
+<details>
+  <summary>Expand</summary>
+  <br>
+
+The `mutate` decorator introduces a new way to enhance ordinary functions dynamically via the power of LLMs, enabling them to adapt to specific inputs. It provides users with the ability to extend the capabilities of functions through natural language prompts. Additionally, the decorator can be further extended using the `resurrect` decorator. The `mutate` decorator enables users to program and account for cases that are challenging or impossible to anticipate.
+
+```python
+@resurrect(lives=1)
+@mutate(request= "Check the inputs closely. Given the inputs, make sure that the function is able to handle different formats if neccessary")
+def my_mutated_function(file_path: str) -> pd.DataFrame():
+    """
+    function to read files and output a dataframes.
+    """
+    pd.read_csv(file_path)
+    
+my_mutated_function("test_file.xlsx")
+```
+
+
 </details>
```

### Comparing `fukkatsu-0.0.1/fukkatsu/utils/medic.py` & `fukkatsu-0.0.2/fukkatsu/utils/medic.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
 
 import openai
 
-from fukkatsu.utils.prompt import ADDITIONAL, CONTEXT, OUTPUT_CONSTRAINTS
+from fukkatsu.utils.prompt import (ADDITIONAL, CONTEXT, CONTEXT_MUTATE,
+                                   OUTPUT_CONSTRAINTS,
+                                   OUTPUT_CONSTRAINTS_MUTATE)
 
 try:
     openai.api_key = os.environ.get("OPENAI_API_KEY")
     print("OPENAI_API_KEY found in environment variables.")
 except:
     print("OPENAI_API_KEY not found in environment variables.")
     raise Exception("OPENAI_API_KEY not found in environment variables.")
@@ -39,7 +41,29 @@
         stop=None,
         temperature=0.1,
     )
 
     corrected_function = response["choices"][0]["message"]["content"].strip()
 
     return corrected_function
+
+
+def enhance(inputs: str, target_function: str, request: str = "") -> str:
+    set_prompt = (
+        f"{CONTEXT_MUTATE}\n\n{target_function}\n\nThe function received the following inputs:\n\n"
+        f"{inputs}\n\nThe user requests the following:\n{request}\n{OUTPUT_CONSTRAINTS_MUTATE}"
+    )
+
+    response = openai.ChatCompletion.create(
+        model=MODEL,
+        messages=[
+            {"role": "system", "content": set_prompt},
+        ],
+        max_tokens=1024,
+        n=1,
+        stop=None,
+        temperature=0.1,
+    )
+
+    mutated_function = response["choices"][0]["message"]["content"].strip()
+
+    return mutated_function
```

### Comparing `fukkatsu-0.0.1/fukkatsu.egg-info/PKG-INFO` & `fukkatsu-0.0.2/fukkatsu.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fukkatsu
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python library for runtime LLM supported code corrections.
 Home-page: https://github.com/maxmekiska/fukkatsu
 Author: Maximilian Mekiska
 Author-email: maxmekiska@gmail.com
 Keywords: machinelearning,llm,runtime,codecorrection
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -45,14 +45,15 @@
 
 
 Here is a representation of what I am trying to do: https://giphy.com/gifs/tire-kNRqJCLOe6ri8/fullscreen 
 
 
 This concept currently only applies to interpreted languages such as Python and not to compiled languages such as C++. The very nature of interpreted languages allows us to dynamically change the code during runtime.
 
+Furthermore, fukkatsu introduces a method to enhance ordinary functions with the power of LLMs. By decorating ordinary functions with natural language prompts, they can now dynamically adapt to unforeseen inputs.
 
 ## MVP
 
 <details>
   <summary>Expand</summary>
   <br>
 
@@ -209,7 +210,31 @@
 ```
 
 ```
 1002
 1002
 ```
 </details>
+
+
+## fukkatsu 0.0.2
+
+<details>
+  <summary>Expand</summary>
+  <br>
+
+The `mutate` decorator introduces a new way to enhance ordinary functions dynamically via the power of LLMs, enabling them to adapt to specific inputs. It provides users with the ability to extend the capabilities of functions through natural language prompts. Additionally, the decorator can be further extended using the `resurrect` decorator. The `mutate` decorator enables users to program and account for cases that are challenging or impossible to anticipate.
+
+```python
+@resurrect(lives=1)
+@mutate(request= "Check the inputs closely. Given the inputs, make sure that the function is able to handle different formats if neccessary")
+def my_mutated_function(file_path: str) -> pd.DataFrame():
+    """
+    function to read files and output a dataframes.
+    """
+    pd.read_csv(file_path)
+    
+my_mutated_function("test_file.xlsx")
+```
+
+
+</details>
```

### Comparing `fukkatsu-0.0.1/setup.py` & `fukkatsu-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     author="Maximilian Mekiska",
     author_email="maxmekiska@gmail.com",
     url="https://github.com/maxmekiska/fukkatsu",
     description="A python library for runtime LLM supported code corrections.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     name="fukkatsu",
-    version="0.0.1",
+    version="0.0.2",
     packages=find_packages(include=["fukkatsu", "fukkatsu.*"]),
     install_requires=[
         "setuptools >= 41.0.0",
         "openai >= 0.27.5, <= 0.28",
     ],
     classifiers=[
         "Programming Language :: Python :: 3.8",
```

