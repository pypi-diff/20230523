# Comparing `tmp/gensum-0.1.1.tar.gz` & `tmp/gensum-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gensum-0.1.1.tar", last modified: Tue May 23 05:22:08 2023, max compression
+gzip compressed data, was "gensum-0.1.2.tar", last modified: Tue May 23 05:36:04 2023, max compression
```

## Comparing `gensum-0.1.1.tar` & `gensum-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 abriel     (503) staff       (20)        0 2023-05-23 05:22:08.094605 gensum-0.1.1/
--rw-r--r--   0 abriel     (503) staff       (20)    11357 2023-05-18 19:51:17.000000 gensum-0.1.1/LICENSE
--rw-r--r--   0 abriel     (503) staff       (20)     4700 2023-05-23 05:22:08.094260 gensum-0.1.1/PKG-INFO
--rw-r--r--   0 abriel     (503) staff       (20)     4400 2023-05-23 05:21:24.000000 gensum-0.1.1/README.md
-drwxr-xr-x   0 abriel     (503) staff       (20)        0 2023-05-23 05:22:08.093012 gensum-0.1.1/gensum/
--rw-r--r--   0 abriel     (503) staff       (20)       29 2023-05-19 16:34:03.000000 gensum-0.1.1/gensum/__init__.py
--rw-r--r--   0 abriel     (503) staff       (20)     3561 2023-05-19 16:41:16.000000 gensum-0.1.1/gensum/generator.py
--rw-r--r--   0 abriel     (503) staff       (20)    12726 2023-05-22 22:10:22.000000 gensum-0.1.1/gensum/gensum.py
-drwxr-xr-x   0 abriel     (503) staff       (20)        0 2023-05-23 05:22:08.094042 gensum-0.1.1/gensum.egg-info/
--rw-r--r--   0 abriel     (503) staff       (20)     4700 2023-05-23 05:22:08.000000 gensum-0.1.1/gensum.egg-info/PKG-INFO
--rw-r--r--   0 abriel     (503) staff       (20)      246 2023-05-23 05:22:08.000000 gensum-0.1.1/gensum.egg-info/SOURCES.txt
--rw-r--r--   0 abriel     (503) staff       (20)        1 2023-05-23 05:22:08.000000 gensum-0.1.1/gensum.egg-info/dependency_links.txt
--rw-r--r--   0 abriel     (503) staff       (20)       20 2023-05-23 05:22:08.000000 gensum-0.1.1/gensum.egg-info/requires.txt
--rw-r--r--   0 abriel     (503) staff       (20)        7 2023-05-23 05:22:08.000000 gensum-0.1.1/gensum.egg-info/top_level.txt
--rw-r--r--   0 abriel     (503) staff       (20)      500 2023-05-23 05:21:45.000000 gensum-0.1.1/pyproject.toml
--rw-r--r--   0 abriel     (503) staff       (20)       38 2023-05-23 05:22:08.094656 gensum-0.1.1/setup.cfg
--rw-r--r--   0 abriel     (503) staff       (20)      834 2023-05-23 05:21:52.000000 gensum-0.1.1/setup.py
+drwxr-xr-x   0 abriel     (503) staff       (20)        0 2023-05-23 05:36:04.402031 gensum-0.1.2/
+-rw-r--r--   0 abriel     (503) staff       (20)    11357 2023-05-18 19:51:17.000000 gensum-0.1.2/LICENSE
+-rw-r--r--   0 abriel     (503) staff       (20)     4700 2023-05-23 05:36:04.401847 gensum-0.1.2/PKG-INFO
+-rw-r--r--   0 abriel     (503) staff       (20)     4400 2023-05-23 05:21:24.000000 gensum-0.1.2/README.md
+drwxr-xr-x   0 abriel     (503) staff       (20)        0 2023-05-23 05:36:04.400894 gensum-0.1.2/gensum/
+-rw-r--r--   0 abriel     (503) staff       (20)       29 2023-05-19 16:34:03.000000 gensum-0.1.2/gensum/__init__.py
+-rw-r--r--   0 abriel     (503) staff       (20)    15514 2023-05-23 05:29:46.000000 gensum-0.1.2/gensum/gensum.py
+drwxr-xr-x   0 abriel     (503) staff       (20)        0 2023-05-23 05:36:04.401634 gensum-0.1.2/gensum.egg-info/
+-rw-r--r--   0 abriel     (503) staff       (20)     4700 2023-05-23 05:36:04.000000 gensum-0.1.2/gensum.egg-info/PKG-INFO
+-rw-r--r--   0 abriel     (503) staff       (20)      226 2023-05-23 05:36:04.000000 gensum-0.1.2/gensum.egg-info/SOURCES.txt
+-rw-r--r--   0 abriel     (503) staff       (20)        1 2023-05-23 05:36:04.000000 gensum-0.1.2/gensum.egg-info/dependency_links.txt
+-rw-r--r--   0 abriel     (503) staff       (20)       20 2023-05-23 05:36:04.000000 gensum-0.1.2/gensum.egg-info/requires.txt
+-rw-r--r--   0 abriel     (503) staff       (20)        7 2023-05-23 05:36:04.000000 gensum-0.1.2/gensum.egg-info/top_level.txt
+-rw-r--r--   0 abriel     (503) staff       (20)      500 2023-05-23 05:30:26.000000 gensum-0.1.2/pyproject.toml
+-rw-r--r--   0 abriel     (503) staff       (20)       38 2023-05-23 05:36:04.402077 gensum-0.1.2/setup.cfg
+-rw-r--r--   0 abriel     (503) staff       (20)      834 2023-05-23 05:30:21.000000 gensum-0.1.2/setup.py
```

### Comparing `gensum-0.1.1/LICENSE` & `gensum-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gensum-0.1.1/PKG-INFO` & `gensum-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gensum
-Version: 0.1.1
+Version: 0.1.2
 Summary: Generative Summarization for Data Augmentation
 Home-page: https://github.com/aaronbriel/gensum
 Author: Aaron Briel
 Author-email: aaronbriel@gmail.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gensum-0.1.1/README.md` & `gensum-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `gensum-0.1.1/gensum/gensum.py` & `gensum-0.1.2/gensum/gensum.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,22 +9,23 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import logging
-from multiprocessing import Process
+import os
 import time
-from typing import Callable, Dict, List, Tuple
+from typing import Dict, List, Tuple
 
 import numpy as np
 import pandas as pd
 
-from generator import Generator
+import openai
+
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 
 class Augmentor(object):
     """
@@ -268,14 +269,92 @@
                 count = self.threshold - value_counts[value]
 
             append_counts[value] = count
 
         return append_counts
 
 
+class Generator(object):
+    """
+    Calls specified LMM and underlying model to generate text based on prompt.
+    
+    Parameters:
+        llm (:obj:`string`, `optional`, defaults to 'chatgpt'): The 
+            generative LLM to use for summarization.
+        model (:obj:`string`, `optional`, defaults to 'gpt-3.5-turbo'): The 
+            specific model to use.
+        temperature (:obj:`int`, `optional`, defaults to 0): Determines the 
+            randomness of the generated sequences. Between 0 and 1, where a
+            higher value means the generated sequences will be more random.
+        debug (:obj:`bool`, `optional`, defaults to True): If set, prints 
+            debug to console.
+    """
+    def __init__(
+        self,
+        llm = 'chatgpt',
+        model = 'gpt-3.5-turbo',
+        temperature = 0,
+        debug = True
+    ):
+        self.llm = llm
+        self.model = model
+        self.temperature = temperature
+        self.debug = debug
+        
+        if llm == 'chatgpt':
+            openai.api_key = os.getenv('OPENAI_API_KEY')
+    
+    def generate_summary(self, prompt: str) -> str:
+        """
+        Calls specified LLM and underlying model to generate text based on 
+        prompt.
+        
+        :param prompt (:obj:`string`): Prompt to generate text from.
+        :return: response (:obj:`string`): Generated text.
+        """
+        if self.llm == 'chatgpt':
+            response = self._chatgpt(prompt)
+        else:
+            raise ValueError(f"LLM {self.llm} not yet supported.")
+
+        return response
+    
+    def _chatgpt(self, prompt: str, retry_attempts: int = 3) -> str:
+        """
+        Calls OpenAI's ChatGPT API to generate text based on prompt.
+        
+        :param prompt (:obj:`string`): Prompt to generate text from.
+        :param retry_attempts (:obj:`int`, `optional`, defaults to 3): Number
+            of retry attempts to make if OpenAI fails.
+        :return: response (:obj:`string`): Generated text.
+        """
+        messages = [{"role": "user", "content": prompt}]
+        # OpenAI seems to intermittently fail, so we'll retry a few times
+        attempts = 0
+        wait_time = 1
+        while attempts < retry_attempts:
+            try:
+                response = openai.ChatCompletion.create(
+                    model=self.model,
+                    temperature=self.temperature,
+                    messages=messages
+                )["choices"][0]["message"]["content"]
+                break
+            except (openai.error.RateLimitError, 
+                    openai.error.APIConnectionError) as err:
+                attempts += 1
+                time.sleep(wait_time * attempts)
+                response = ''
+                if self.debug:
+                    logger.warning(f"ERROR: {err}")
+                
+        
+        return response
+
+
 def get_min_max_word_counts(sents: List[str]) -> Tuple[int, int]:
     """
     Gets min and max word counts from list of sentences
     
     :param sents: List of sentences to get min/max word counts from
     :return: Tuple of min and max word counts
     """
```

### Comparing `gensum-0.1.1/gensum.egg-info/PKG-INFO` & `gensum-0.1.2/gensum.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gensum
-Version: 0.1.1
+Version: 0.1.2
 Summary: Generative Summarization for Data Augmentation
 Home-page: https://github.com/aaronbriel/gensum
 Author: Aaron Briel
 Author-email: aaronbriel@gmail.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gensum-0.1.1/setup.py` & `gensum-0.1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.1.1'
+VERSION = '0.1.2'
 PACKAGE_NAME = 'gensum'
 AUTHOR = 'Aaron Briel'
 AUTHOR_EMAIL = 'aaronbriel@gmail.com'
 URL = 'https://github.com/aaronbriel/gensum'
 
 LICENSE = 'Apache License 2.0'
 DESCRIPTION = 'Generative Summarization for Data Augmentation'
```

