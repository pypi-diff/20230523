# Comparing `tmp/vector_vault-0.2.8.tar.gz` & `tmp/vector_vault-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-0.2.8.tar", last modified: Mon May 22 19:51:41 2023, max compression
+gzip compressed data, was "vector_vault-0.2.9.tar", last modified: Tue May 23 05:35:24 2023, max compression
```

## Comparing `vector_vault-0.2.8.tar` & `vector_vault-0.2.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-22 19:51:41.308486 vector_vault-0.2.8/
--rw-r--r--   0 johnrood   (501) staff       (20)      688 2023-05-20 04:34:30.000000 vector_vault-0.2.8/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    11737 2023-05-22 19:51:41.308290 vector_vault-0.2.8/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    10985 2023-05-21 05:47:01.000000 vector_vault-0.2.8/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-22 19:51:41.308529 vector_vault-0.2.8/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1066 2023-05-22 19:49:44.000000 vector_vault-0.2.8/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-22 19:51:41.306506 vector_vault-0.2.8/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    11737 2023-05-22 19:51:41.000000 vector_vault-0.2.8/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      384 2023-05-22 19:51:41.000000 vector_vault-0.2.8/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-22 19:51:41.000000 vector_vault-0.2.8/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-05-22 19:51:41.000000 vector_vault-0.2.8/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-05-22 19:51:41.000000 vector_vault-0.2.8/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-22 19:51:41.308075 vector_vault-0.2.8/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      675 2023-05-21 06:23:38.000000 vector_vault-0.2.8/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)     5165 2023-05-22 19:44:52.000000 vector_vault-0.2.8/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3380 2023-05-22 19:00:54.000000 vector_vault-0.2.8/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1824 2023-05-22 19:13:17.000000 vector_vault-0.2.8/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-0.2.8/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1542 2023-05-22 19:15:18.000000 vector_vault-0.2.8/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)    17191 2023-05-22 19:49:38.000000 vector_vault-0.2.8/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-0.2.8/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-23 05:35:24.041313 vector_vault-0.2.9/
+-rw-r--r--   0 johnrood   (501) staff       (20)      688 2023-05-20 04:34:30.000000 vector_vault-0.2.9/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    11808 2023-05-23 05:35:24.041143 vector_vault-0.2.9/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    11056 2023-05-22 19:56:00.000000 vector_vault-0.2.9/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-23 05:35:24.041350 vector_vault-0.2.9/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1066 2023-05-22 21:42:21.000000 vector_vault-0.2.9/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-23 05:35:24.038889 vector_vault-0.2.9/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    11808 2023-05-23 05:35:24.000000 vector_vault-0.2.9/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      384 2023-05-23 05:35:24.000000 vector_vault-0.2.9/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-23 05:35:24.000000 vector_vault-0.2.9/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-05-23 05:35:24.000000 vector_vault-0.2.9/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-05-23 05:35:24.000000 vector_vault-0.2.9/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-23 05:35:24.040837 vector_vault-0.2.9/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      675 2023-05-21 06:23:38.000000 vector_vault-0.2.9/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     5163 2023-05-22 21:46:43.000000 vector_vault-0.2.9/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3380 2023-05-22 19:00:54.000000 vector_vault-0.2.9/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1824 2023-05-22 19:13:17.000000 vector_vault-0.2.9/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-0.2.9/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1542 2023-05-22 19:15:18.000000 vector_vault-0.2.9/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    17191 2023-05-22 19:49:38.000000 vector_vault-0.2.9/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-0.2.9/vectorvault/wrap.py
```

### Comparing `vector_vault-0.2.8/LICENSE` & `vector_vault-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-0.2.8/PKG-INFO` & `vector_vault-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 0.2.8
+Version: 0.2.9
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -48,14 +48,19 @@
 `get_chat` : Retrieves a response from OpenAI's ChatGPT for a given input text, with support for handling conversation history, summarizing responses, and retrieving context-based responses by accessing similar references in the vault
 
 
 <br>
 <br>
 
 ## Basic usage:
+Install VectorVault:
+```
+pip install vector-vault
+```
+Use VectorVault:
 ```
 from vectorvault import Vault
 
 # Create an instance of the Vault class - a new vault will be created if name does not exist
 vault = Vault(user='your_user_id', api_key='your_api_key', vault='name_of_your_vault)
 
 # Some text data we want to store
```

### Comparing `vector_vault-0.2.8/README.md` & `vector_vault-0.2.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,19 @@
 `get_chat` : Retrieves a response from OpenAI's ChatGPT for a given input text, with support for handling conversation history, summarizing responses, and retrieving context-based responses by accessing similar references in the vault
 
 
 <br>
 <br>
 
 ## Basic usage:
+Install VectorVault:
+```
+pip install vector-vault
+```
+Use VectorVault:
 ```
 from vectorvault import Vault
 
 # Create an instance of the Vault class - a new vault will be created if name does not exist
 vault = Vault(user='your_user_id', api_key='your_api_key', vault='name_of_your_vault)
 
 # Some text data we want to store
```

### Comparing `vector_vault-0.2.8/setup.py` & `vector_vault-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="0.2.8",
+    version="0.2.9",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-0.2.8/vector_vault.egg-info/PKG-INFO` & `vector_vault-0.2.9/vector_vault.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 0.2.8
+Version: 0.2.9
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -48,14 +48,19 @@
 `get_chat` : Retrieves a response from OpenAI's ChatGPT for a given input text, with support for handling conversation history, summarizing responses, and retrieving context-based responses by accessing similar references in the vault
 
 
 <br>
 <br>
 
 ## Basic usage:
+Install VectorVault:
+```
+pip install vector-vault
+```
+Use VectorVault:
 ```
 from vectorvault import Vault
 
 # Create an instance of the Vault class - a new vault will be created if name does not exist
 vault = Vault(user='your_user_id', api_key='your_api_key', vault='name_of_your_vault)
 
 # Some text data we want to store
```

### Comparing `vector_vault-0.2.8/vectorvault/__init__.py` & `vector_vault-0.2.9/vectorvault/__init__.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.2.8/vectorvault/ai.py` & `vector_vault-0.2.9/vectorvault/ai.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 # herein are proprietary to Vector Vault
 # and its suppliers and may be covered by U.S. and Foreign Patents,
 # patents in process, and are protected by trade secret or copyright law.
 # Dissemination of this information or reproduction of this material
 # is strictly forbidden unless prior written permission is obtained
 # from Vector Vault.
 
-
 import openai
 import tiktoken
 
 class AI:
     def __init__(self) -> None:
         pass
 
@@ -47,15 +46,15 @@
             # The API responds with a 'choices' array containing the 'message' object.
         return response['choices'][0]['message']['content']
     
     # This function returns a ChatGPT completion based contextual input
     def llm_w_context(self, user_input, context, history=None, model='gpt-3.5-turbo'):
         prompt_template = """
         Use the following pieces of context to answer the question at the end. 
-        Answer as if you were the modern voice of the context. Make sure to not just repeat what is referenced. Don't preface, and at the end, don't give any warnings.
+        Answer as if you were the modern voice of the context. Make sure to not just repeat what is referenced. Don't preface, and don't give any warnings at the end.
 
         {context}
 
         Question: {question}
 
         (answer the question directly. Most importantly, make your answer interesting, engaging, and helpful) 
         Answer:"""
```

### Comparing `vector_vault-0.2.8/vectorvault/cloudmanager.py` & `vector_vault-0.2.9/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.2.8/vectorvault/creds.py` & `vector_vault-0.2.9/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.2.8/vectorvault/download.py` & `vector_vault-0.2.9/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.2.8/vectorvault/itemize.py` & `vector_vault-0.2.9/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.2.8/vectorvault/vault.py` & `vector_vault-0.2.9/vectorvault/vault.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.2.8/vectorvault/wrap.py` & `vector_vault-0.2.9/vectorvault/wrap.py`

 * *Files identical despite different names*

