# Comparing `tmp/superpowered-sdk-0.1.4.tar.gz` & `tmp/superpowered-sdk-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superpowered-sdk-0.1.4.tar", last modified: Mon May 22 18:08:50 2023, max compression
+gzip compressed data, was "superpowered-sdk-0.1.5.tar", last modified: Tue May 23 06:02:00 2023, max compression
```

## Comparing `superpowered-sdk-0.1.4.tar` & `superpowered-sdk-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxr-xr-x   0 justinclark   (501) staff       (20)        0 2023-05-22 18:08:50.577150 superpowered-sdk-0.1.4/
--rw-r--r--   0 justinclark   (501) staff       (20)     6636 2023-05-22 18:08:50.576850 superpowered-sdk-0.1.4/PKG-INFO
--rw-r--r--   0 justinclark   (501) staff       (20)     5136 2023-05-19 14:21:49.000000 superpowered-sdk-0.1.4/README.md
--rw-r--r--   0 justinclark   (501) staff       (20)       38 2023-05-22 18:08:50.577257 superpowered-sdk-0.1.4/setup.cfg
--rw-r--r--   0 justinclark   (501) staff       (20)     2277 2023-05-22 18:07:56.000000 superpowered-sdk-0.1.4/setup.py
-drwxr-xr-x   0 justinclark   (501) staff       (20)        0 2023-05-22 18:08:50.574272 superpowered-sdk-0.1.4/superpowered/
--rw-r--r--   0 justinclark   (501) staff       (20)      892 2023-05-22 17:50:01.000000 superpowered-sdk-0.1.4/superpowered/__init__.py
--rw-r--r--   0 justinclark   (501) staff       (20)     4045 2023-05-22 18:08:50.000000 superpowered-sdk-0.1.4/superpowered/errors.json
--rw-r--r--   0 justinclark   (501) staff       (20)     1301 2023-05-18 20:08:04.000000 superpowered-sdk-0.1.4/superpowered/exceptions.py
--rw-r--r--   0 justinclark   (501) staff       (20)    11202 2023-05-22 17:50:01.000000 superpowered-sdk-0.1.4/superpowered/superpowered.py
-drwxr-xr-x   0 justinclark   (501) staff       (20)        0 2023-05-22 18:08:50.576377 superpowered-sdk-0.1.4/superpowered_sdk.egg-info/
--rw-r--r--   0 justinclark   (501) staff       (20)     6636 2023-05-22 18:08:50.000000 superpowered-sdk-0.1.4/superpowered_sdk.egg-info/PKG-INFO
--rw-r--r--   0 justinclark   (501) staff       (20)      323 2023-05-22 18:08:50.000000 superpowered-sdk-0.1.4/superpowered_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 justinclark   (501) staff       (20)        1 2023-05-22 18:08:50.000000 superpowered-sdk-0.1.4/superpowered_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 justinclark   (501) staff       (20)       17 2023-05-22 18:08:50.000000 superpowered-sdk-0.1.4/superpowered_sdk.egg-info/requires.txt
--rw-r--r--   0 justinclark   (501) staff       (20)       13 2023-05-22 18:08:50.000000 superpowered-sdk-0.1.4/superpowered_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:02:00.145100 superpowered-sdk-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-05-23 06:02:00.145100 superpowered-sdk-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-05-23 06:01:46.000000 superpowered-sdk-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 06:02:00.145100 superpowered-sdk-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-23 06:01:46.000000 superpowered-sdk-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:02:00.145100 superpowered-sdk-0.1.5/superpowered/
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-23 06:01:46.000000 superpowered-sdk-0.1.5/superpowered/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-23 06:01:46.000000 superpowered-sdk-0.1.5/superpowered/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11449 2023-05-23 06:01:46.000000 superpowered-sdk-0.1.5/superpowered/superpowered.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:02:00.145100 superpowered-sdk-0.1.5/superpowered_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-05-23 06:01:59.000000 superpowered-sdk-0.1.5/superpowered_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-23 06:02:00.000000 superpowered-sdk-0.1.5/superpowered_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 06:01:59.000000 superpowered-sdk-0.1.5/superpowered_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-23 06:01:59.000000 superpowered-sdk-0.1.5/superpowered_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-23 06:01:59.000000 superpowered-sdk-0.1.5/superpowered_sdk.egg-info/top_level.txt
```

### Comparing `superpowered-sdk-0.1.4/PKG-INFO` & `superpowered-sdk-0.1.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,7 @@
-Metadata-Version: 2.1
-Name: superpowered-sdk
-Version: 0.1.4
-Summary: Superpowered AI SDK
-Home-page: https://superpowered.ai
-Author: superpowered
-Author-email: justin@superpowered.ai
-License: Proprietary License
-Project-URL: Homepage, https://superpowered.ai
-Project-URL: Documentation, https://superpowered.ai/docs
-Project-URL: Contact, https://superpowered.ai/contact/
-Project-URL: End-User License Agreement, https://superpowered.ai/api-user-agreement/
-Keywords: Superpowered AI Knowledge base as a service for LLM applications
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Environment :: Other Environment
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: System Administrators
-Classifier: License :: Other/Proprietary License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Database
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 # This is the official Superpowered AI Python SDK
 
 ## Installation
 
 `pip install superpowered-sdk`
 
 _Note_: To create API keys, please login to the Superpowered AI dashboard and click the "Account" tab on the left navigation.
@@ -198,7 +164,17 @@
         '<etc.>'
     ],
     top_k=10,                       # OPTIONAL
     max_chunk_length=500,           # OPTIONAL
     summarize_results=True          # OPTIONAL
 )
 ```
+
+
+
+## Usage Operations
+
+**Get total storage used**
+
+```python
+storage_stats = superpowered.get_total_storage()
+```
```

#### html2text {}

```diff
@@ -1,31 +1,11 @@
-Metadata-Version: 2.1 Name: superpowered-sdk Version: 0.1.4 Summary:
-Superpowered AI SDK Home-page: https://superpowered.ai Author: superpowered
-Author-email: justin@superpowered.ai License: Proprietary License Project-URL:
-Homepage, https://superpowered.ai Project-URL: Documentation, https://
-superpowered.ai/docs Project-URL: Contact, https://superpowered.ai/contact/
-Project-URL: End-User License Agreement, https://superpowered.ai/api-user-
-agreement/ Keywords: Superpowered AI Knowledge base as a service for LLM
-applications Classifier: Development Status :: 4 - Beta Classifier: Environment
-:: Console Classifier: Environment :: Other Environment Classifier: Intended
-Audience :: Developers Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: Science/Research Classifier: Intended Audience
-:: System Administrators Classifier: License :: Other/Proprietary License
-Classifier: Operating System :: OS Independent Classifier: Programming Language
-:: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Topic :: Database Classifier: Topic :: Software
-Development Classifier: Topic :: Software Development :: Libraries Classifier:
-Topic :: Software Development :: Libraries :: Application Frameworks
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6 Description-Content-Type: text/markdown # This is the
-official Superpowered AI Python SDK ## Installation `pip install superpowered-
-sdk` _Note_: To create API keys, please login to the Superpowered AI dashboard
-and click the "Account" tab on the left navigation. ## Knowledge Base
-Operations **Create a knowledge base** ```python kb =
+# This is the official Superpowered AI Python SDK ## Installation `pip install
+superpowered-sdk` _Note_: To create API keys, please login to the Superpowered
+AI dashboard and click the "Account" tab on the left navigation. ## Knowledge
+Base Operations **Create a knowledge base** ```python kb =
 superpowered.create_knowledge_base( title='research-biology',
 description='Papers, podcasts, and articles about biology.', # OPTIONAL
 supp_id='' # OPTIONAL ) # use kb['id'] when uploading documents for this
 knowledge base ``` **Get knowledge base(s)** ```python # list all knowledge
 bases kbs = superpowered.list_knowledge_bases() # returns list of kb objects #
 list knowledge bases that meet criteria kbs = superpowered.list_knowledge_bases
 (supp_id='') # OR kbs = superpowered.list_knowledge_bases
@@ -72,8 +52,9 @@
 web search applications like Google Chrome extensions. ```python # if passages
 are longer than `max_chunk_length`, we will chunk the passages to # make them
 more easily parsable by our model result = superpowered.query_passages
 ( query='What technological advancements do need to construct a dyson sphere?',
 passages=[ '
 , '', '
 >' ], top_k=10, # OPTIONAL max_chunk_length=500, # OPTIONAL
-summarize_results=True # OPTIONAL ) ```
+summarize_results=True # OPTIONAL ) ``` ## Usage Operations **Get total storage
+used** ```python storage_stats = superpowered.get_total_storage() ```
```

### Comparing `superpowered-sdk-0.1.4/setup.py` & `superpowered-sdk-0.1.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 def read(fname):
     with open(os.path.join(os.path.dirname(__file__), fname), "r", encoding="utf-8") as fh:
         return fh.read()
 
 
 # copy errors.json to the package directory
 DIR = os.path.dirname(os.path.abspath(__file__))
-shutil.copy(f'{DIR}/../../errors.json', f'{DIR}/superpowered/errors.json')
+shutil.copy(f'{DIR}/../../errors.json', f'{DIR}/superpowered/errors.json', follow_symlinks=True)
 
 
 setuptools.setup(
     name="superpowered-sdk",
     version=read("VERSION"),
     description="Superpowered AI SDK",
     license="Proprietary License",
```

### Comparing `superpowered-sdk-0.1.4/superpowered/__init__.py` & `superpowered-sdk-0.1.5/superpowered/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from .superpowered import (
     set_api_key,
+    get_total_storage,
     create_knowledge_base,
     list_knowledge_bases,
     get_knowledge_base,
     delete_knowledge_base,
     create_document_via_text,
     create_document_via_url,
     create_document_via_file,
@@ -18,14 +19,15 @@
     set_base_url,
 )
 
 from . import exceptions
 
 __all__ = [
     'set_api_key',
+    'get_total_storage',
     'create_knowledge_base',
     'list_knowledge_bases',
     'get_knowledge_base',
     'delete_knowledge_base',
     'create_document_via_text',
     'create_document_via_url',
     'create_document_via_file',
```

### Comparing `superpowered-sdk-0.1.4/superpowered/exceptions.py` & `superpowered-sdk-0.1.5/superpowered/exceptions.py`

 * *Files identical despite different names*

### Comparing `superpowered-sdk-0.1.4/superpowered/superpowered.py` & `superpowered-sdk-0.1.5/superpowered/superpowered.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,26 @@
     elif not resp.ok:
         print(args)
         raise Exception(resp_json, resp.status_code)
     else:
         return resp_json
 
 
+def get_total_storage():
+    """
+    GET /usage/total_storage
+    """
+    args = {
+        'method': 'GET',
+        'url': f'{get_base_url()}/usage/total_storage',
+        'auth': auth(),
+    }
+    return make_api_call(args)
+
+
 def create_knowledge_base(title: str, description: str = None, supp_id: str = None) -> dict:
     """
     POST /knowledge_bases
     """
     data = {
         'title': title,
     }
@@ -214,15 +226,16 @@
         'Content-MD5': encoded_md5,
     }
     args = {
         'url': resp['temporary_url'],
         'data': file_content,
         'headers': headers,
     }
-    resp = requests.put(**args)
+    with requests.put(**args) as resp:
+        pass
 
     return {'message': 'Successfully uploaded file. Vectorization process will begin shortly.'}
 
 
 def download_file(knowledge_base_id: str, file_name: str, destination_path: str = None) -> bytes:
     """
     POST /knowledge_bases/{knowledge_base_id}/documents/request_signed_file_url
```

### Comparing `superpowered-sdk-0.1.4/superpowered_sdk.egg-info/PKG-INFO` & `superpowered-sdk-0.1.5/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,201 @@
 Metadata-Version: 2.1
 Name: superpowered-sdk
-Version: 0.1.4
+Version: 0.1.5
 Summary: Superpowered AI SDK
 Home-page: https://superpowered.ai
 Author: superpowered
 Author-email: justin@superpowered.ai
 License: Proprietary License
 Project-URL: Homepage, https://superpowered.ai
 Project-URL: Documentation, https://superpowered.ai/docs
 Project-URL: Contact, https://superpowered.ai/contact/
 Project-URL: End-User License Agreement, https://superpowered.ai/api-user-agreement/
+Description: # This is the official Superpowered AI Python SDK
+        
+        ## Installation
+        
+        `pip install superpowered-sdk`
+        
+        _Note_: To create API keys, please login to the Superpowered AI dashboard and click the "Account" tab on the left navigation.
+        
+        
+        ## Knowledge Base Operations
+        
+        **Create a knowledge base**
+        
+        ```python
+        kb = superpowered.create_knowledge_base(
+            title='research-biology',
+            description='Papers, podcasts, and articles about biology.',  # OPTIONAL
+            supp_id='<internal_id>'                                       # OPTIONAL
+        )
+        # use kb['id'] when uploading documents for this knowledge base
+        ```
+        
+        
+        **Get knowledge base(s)**
+        
+        ```python
+        # list all knowledge bases
+        kbs = superpowered.list_knowledge_bases()  # returns list of kb objects
+        
+        # list knowledge bases that meet criteria
+        kbs = superpowered.list_knowledge_bases(supp_id='<internal_id>')
+        # OR
+        kbs = superpowered.list_knowledge_bases(title_begins_with='research-')
+        
+        # get single knowledge base
+        kb = superpowered.get_knowledge_base(kb_id)  # returns a single kb object
+        ```
+        
+        
+        **Delete knowledge base**
+        
+        ```python
+        ok = superpowered.delete_knowledge_base(kb_id)
+        ```
+        
+        
+        
+        ## Document Operations
+        
+        **Create Documents**
+        
+        *NOTE: We currently support `.txt`, `.md`, `.pdf`, `.docx`, `.wav`, `.mp3`, `.m4a` files.*
+        
+        ```python
+        # create a document via plain text
+        superpowered.create_document_via_text(
+            knowledge_base_id=kb_id,
+            content='Observation suggests that people are switching to using ChatGPT '
+                    'to write things for them with almost indecent haste. Most people '
+                    'hate to write as much as they hate math. Way more than admit it. '
+                    'Within a year the median piece of writing could be by AI.',
+            title='pg-twitter-20230509',                                                                        # OPTIONAL
+            link_to_source='https://twitter.com/paulg/status/1655925905527537666?s=42&t=blTOe1mODRIfVwjJvMJ52w' # OPTIONAL
+            description=None,                                                                                   # OPTIONAL
+            supp_id='<internal_id>',                                                                            # OPTIONAL
+        )
+        
+        # create a document via a url
+        superpowered.create_document_via_url(
+            knowledge_base_id=kb_id,
+            url='https://superpoweredai.notion.site/',
+            title=None,                                   # OPTIONAL - scraped from HTML <title> tag if not provided
+            description='Superpowered AI Documentation',  # OPTIONAL
+            supp_id='<internal_id>'                       # OPTIONAL
+        )
+        
+        # create a document via file upload
+        superpowered.create_document_via_file(
+            knowledge_base_id=kb_id,
+            file_path='/path/to/podcast_audio.mp3',
+            description=None,                             # OPTIONAL
+            supp_id=None                                  # OPTIONAL
+        )
+        ```
+        
+        
+        
+        **Get document(s)**
+        
+        ```python
+        # list all documents
+        # NOTE: `content` is not returned with `list_documents()` - only with `get_document()`
+        docs = superpowered.list_documents()
+        
+        # list documents with filter
+        docs = superpowered.list_documents(knowledge_base_id=kb_id, title_begins_with='pg-twitter')
+        # OR
+        docs = superpowered.list_documents(knowledge_base_id=kb_id, link_to_source='https://superpoweredai.notion.site/')
+        # OR
+        docs = superpowered.list_documents(knowledge_base_id=kb_id, supp_id='<internal_id>')
+        # OR
+        docs = superpowered.list_documents(knowledge_base_id=kb_id, vectorization_status='PENDING|IN_PROGRESS|COMPLETE|FAILED')
+        
+        # get individual document by id
+        doc = superpowered.get_document(kb_id, doc_id)
+        ```
+        
+        
+        
+        **Update document**
+        
+        ```python
+        # valid params: title, supp_id, description
+        doc = superpowered.update_document(
+            knowledge_base_id=kb_id,
+            document_id=doc_id,
+            title='patched title',                      # OPTIONAL
+            supp_id='<internal_id>',                    # OPTIONAL
+            description='I am a document about X'       # OPTIONAL
+        )
+        ```
+        
+        
+        
+        **Delete document**
+        
+        ```python
+        ok = superpowered.delete_document(
+            knowledge_base_id=kb_id,
+            document_id=doc_id
+        )
+        ```
+        
+        
+        
+        ## Query Operations
+        
+        **Query knowledge bases**
+        
+        ```python
+        result = superpowered.query_knowledge_bases(
+            knowledge_base_ids=[tweets_kb_id, research_papers_kb_kd, podcasts_kb_id],
+            query='What are some of the biggest hurdles we '
+                  'need to overcome to achieve superintelligence?',
+            top_k=10,                                                                   # OPTIONAL
+            summarize_results=True                                                      # OPTIONAL
+        )
+        ```
+        
+        
+        
+        **Query passages directly without having to create a knowledge base**
+        
+        This functionality is perfect for web search applications like Google Chrome extensions.
+        
+        ```python
+        # if passages are longer than `max_chunk_length`, we will chunk the passages to 
+        # make them more easily parsable by our model
+        result = superpowered.query_passages(
+            query='What technological advancements do need to construct a dyson sphere?',
+            passages=[
+                '<web page content',
+                '<text content>',
+                '<etc.>'
+            ],
+            top_k=10,                       # OPTIONAL
+            max_chunk_length=500,           # OPTIONAL
+            summarize_results=True          # OPTIONAL
+        )
+        ```
+        
+        
+        
+        ## Usage Operations
+        
+        **Get total storage used**
+        
+        ```python
+        storage_stats = superpowered.get_total_storage()
+        ```
 Keywords: Superpowered AI Knowledge base as a service for LLM applications
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
@@ -27,178 +208,7 @@
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-
-# This is the official Superpowered AI Python SDK
-
-## Installation
-
-`pip install superpowered-sdk`
-
-_Note_: To create API keys, please login to the Superpowered AI dashboard and click the "Account" tab on the left navigation.
-
-
-## Knowledge Base Operations
-
-**Create a knowledge base**
-
-```python
-kb = superpowered.create_knowledge_base(
-    title='research-biology',
-    description='Papers, podcasts, and articles about biology.',  # OPTIONAL
-    supp_id='<internal_id>'                                       # OPTIONAL
-)
-# use kb['id'] when uploading documents for this knowledge base
-```
-
-
-**Get knowledge base(s)**
-
-```python
-# list all knowledge bases
-kbs = superpowered.list_knowledge_bases()  # returns list of kb objects
-
-# list knowledge bases that meet criteria
-kbs = superpowered.list_knowledge_bases(supp_id='<internal_id>')
-# OR
-kbs = superpowered.list_knowledge_bases(title_begins_with='research-')
-
-# get single knowledge base
-kb = superpowered.get_knowledge_base(kb_id)  # returns a single kb object
-```
-
-
-**Delete knowledge base**
-
-```python
-ok = superpowered.delete_knowledge_base(kb_id)
-```
-
-
-
-## Document Operations
-
-**Create Documents**
-
-*NOTE: We currently support `.txt`, `.md`, `.pdf`, `.docx`, `.wav`, `.mp3`, `.m4a` files.*
-
-```python
-# create a document via plain text
-superpowered.create_document_via_text(
-    knowledge_base_id=kb_id,
-    content='Observation suggests that people are switching to using ChatGPT '
-            'to write things for them with almost indecent haste. Most people '
-            'hate to write as much as they hate math. Way more than admit it. '
-            'Within a year the median piece of writing could be by AI.',
-    title='pg-twitter-20230509',                                                                        # OPTIONAL
-    link_to_source='https://twitter.com/paulg/status/1655925905527537666?s=42&t=blTOe1mODRIfVwjJvMJ52w' # OPTIONAL
-    description=None,                                                                                   # OPTIONAL
-    supp_id='<internal_id>',                                                                            # OPTIONAL
-)
-
-# create a document via a url
-superpowered.create_document_via_url(
-    knowledge_base_id=kb_id,
-    url='https://superpoweredai.notion.site/',
-    title=None,                                   # OPTIONAL - scraped from HTML <title> tag if not provided
-    description='Superpowered AI Documentation',  # OPTIONAL
-    supp_id='<internal_id>'                       # OPTIONAL
-)
-
-# create a document via file upload
-superpowered.create_document_via_file(
-    knowledge_base_id=kb_id,
-    file_path='/path/to/podcast_audio.mp3',
-    description=None,                             # OPTIONAL
-    supp_id=None                                  # OPTIONAL
-)
-```
-
-
-
-**Get document(s)**
-
-```python
-# list all documents
-# NOTE: `content` is not returned with `list_documents()` - only with `get_document()`
-docs = superpowered.list_documents()
-
-# list documents with filter
-docs = superpowered.list_documents(knowledge_base_id=kb_id, title_begins_with='pg-twitter')
-# OR
-docs = superpowered.list_documents(knowledge_base_id=kb_id, link_to_source='https://superpoweredai.notion.site/')
-# OR
-docs = superpowered.list_documents(knowledge_base_id=kb_id, supp_id='<internal_id>')
-# OR
-docs = superpowered.list_documents(knowledge_base_id=kb_id, vectorization_status='PENDING|IN_PROGRESS|COMPLETE|FAILED')
-
-# get individual document by id
-doc = superpowered.get_document(kb_id, doc_id)
-```
-
-
-
-**Update document**
-
-```python
-# valid params: title, supp_id, description
-doc = superpowered.update_document(
-    knowledge_base_id=kb_id,
-    document_id=doc_id,
-    title='patched title',                      # OPTIONAL
-    supp_id='<internal_id>',                    # OPTIONAL
-    description='I am a document about X'       # OPTIONAL
-)
-```
-
-
-
-**Delete document**
-
-```python
-ok = superpowered.delete_document(
-    knowledge_base_id=kb_id,
-    document_id=doc_id
-)
-```
-
-
-
-## Query Operations
-
-**Query knowledge bases**
-
-```python
-result = superpowered.query_knowledge_bases(
-    knowledge_base_ids=[tweets_kb_id, research_papers_kb_kd, podcasts_kb_id],
-    query='What are some of the biggest hurdles we '
-          'need to overcome to achieve superintelligence?',
-    top_k=10,                                                                   # OPTIONAL
-    summarize_results=True                                                      # OPTIONAL
-)
-```
-
-
-
-**Query passages directly without having to create a knowledge base**
-
-This functionality is perfect for web search applications like Google Chrome extensions.
-
-```python
-# if passages are longer than `max_chunk_length`, we will chunk the passages to 
-# make them more easily parsable by our model
-result = superpowered.query_passages(
-    query='What technological advancements do need to construct a dyson sphere?',
-    passages=[
-        '<web page content',
-        '<text content>',
-        '<etc.>'
-    ],
-    top_k=10,                       # OPTIONAL
-    max_chunk_length=500,           # OPTIONAL
-    summarize_results=True          # OPTIONAL
-)
-```
```

#### html2text {}

```diff
@@ -1,32 +1,18 @@
-Metadata-Version: 2.1 Name: superpowered-sdk Version: 0.1.4 Summary:
+Metadata-Version: 2.1 Name: superpowered-sdk Version: 0.1.5 Summary:
 Superpowered AI SDK Home-page: https://superpowered.ai Author: superpowered
 Author-email: justin@superpowered.ai License: Proprietary License Project-URL:
 Homepage, https://superpowered.ai Project-URL: Documentation, https://
 superpowered.ai/docs Project-URL: Contact, https://superpowered.ai/contact/
 Project-URL: End-User License Agreement, https://superpowered.ai/api-user-
-agreement/ Keywords: Superpowered AI Knowledge base as a service for LLM
-applications Classifier: Development Status :: 4 - Beta Classifier: Environment
-:: Console Classifier: Environment :: Other Environment Classifier: Intended
-Audience :: Developers Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: Science/Research Classifier: Intended Audience
-:: System Administrators Classifier: License :: Other/Proprietary License
-Classifier: Operating System :: OS Independent Classifier: Programming Language
-:: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Topic :: Database Classifier: Topic :: Software
-Development Classifier: Topic :: Software Development :: Libraries Classifier:
-Topic :: Software Development :: Libraries :: Application Frameworks
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6 Description-Content-Type: text/markdown # This is the
-official Superpowered AI Python SDK ## Installation `pip install superpowered-
-sdk` _Note_: To create API keys, please login to the Superpowered AI dashboard
-and click the "Account" tab on the left navigation. ## Knowledge Base
-Operations **Create a knowledge base** ```python kb =
-superpowered.create_knowledge_base( title='research-biology',
+agreement/ Description: # This is the official Superpowered AI Python SDK ##
+Installation `pip install superpowered-sdk` _Note_: To create API keys, please
+login to the Superpowered AI dashboard and click the "Account" tab on the left
+navigation. ## Knowledge Base Operations **Create a knowledge base** ```python
+kb = superpowered.create_knowledge_base( title='research-biology',
 description='Papers, podcasts, and articles about biology.', # OPTIONAL
 supp_id='' # OPTIONAL ) # use kb['id'] when uploading documents for this
 knowledge base ``` **Get knowledge base(s)** ```python # list all knowledge
 bases kbs = superpowered.list_knowledge_bases() # returns list of kb objects #
 list knowledge bases that meet criteria kbs = superpowered.list_knowledge_bases
 (supp_id='') # OR kbs = superpowered.list_knowledge_bases
 (title_begins_with='research-') # get single knowledge base kb =
@@ -72,8 +58,23 @@
 web search applications like Google Chrome extensions. ```python # if passages
 are longer than `max_chunk_length`, we will chunk the passages to # make them
 more easily parsable by our model result = superpowered.query_passages
 ( query='What technological advancements do need to construct a dyson sphere?',
 passages=[ '
 , '', '
 >' ], top_k=10, # OPTIONAL max_chunk_length=500, # OPTIONAL
-summarize_results=True # OPTIONAL ) ```
+summarize_results=True # OPTIONAL ) ``` ## Usage Operations **Get total storage
+used** ```python storage_stats = superpowered.get_total_storage() ``` Keywords:
+Superpowered AI Knowledge base as a service for LLM applications Platform:
+UNKNOWN Classifier: Development Status :: 4 - Beta Classifier: Environment ::
+Console Classifier: Environment :: Other Environment Classifier: Intended
+Audience :: Developers Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: Science/Research Classifier: Intended Audience
+:: System Administrators Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: OS Independent Classifier: Programming Language
+:: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Topic :: Database Classifier: Topic :: Software
+Development Classifier: Topic :: Software Development :: Libraries Classifier:
+Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.6 Description-Content-Type: text/markdown
```

