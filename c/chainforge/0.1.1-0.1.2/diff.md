# Comparing `tmp/chainforge-0.1.1.tar.gz` & `tmp/chainforge-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainforge-0.1.1.tar", last modified: Mon May 22 17:32:43 2023, max compression
+gzip compressed data, was "chainforge-0.1.2.tar", last modified: Tue May 23 19:13:32 2023, max compression
```

## Comparing `chainforge-0.1.1.tar` & `chainforge-0.1.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 ianarawjo   (501) staff       (20)        0 2023-05-22 17:32:43.694374 chainforge-0.1.1/
--rw-r--r--   0 ianarawjo   (501) staff       (20)     1067 2023-04-11 20:15:11.000000 chainforge-0.1.1/LICENSE.md
--rw-r--r--   0 ianarawjo   (501) staff       (20)       35 2023-05-18 04:19:30.000000 chainforge-0.1.1/MANIFEST.in
--rw-r--r--   0 ianarawjo   (501) staff       (20)      576 2023-05-22 17:32:43.693880 chainforge-0.1.1/PKG-INFO
--rw-r--r--   0 ianarawjo   (501) staff       (20)     8269 2023-05-22 17:16:36.000000 chainforge-0.1.1/README.md
-drwxr-xr-x   0 ianarawjo   (501) staff       (20)        0 2023-05-22 17:32:43.660346 chainforge-0.1.1/chainforge/
--rw-r--r--   0 ianarawjo   (501) staff       (20)       22 2023-05-18 04:19:30.000000 chainforge-0.1.1/chainforge/__init__.py
--rw-r--r--   0 ianarawjo   (501) staff       (20)     4801 2023-05-18 04:19:30.000000 chainforge-0.1.1/chainforge/app.py
--rw-r--r--   0 ianarawjo   (501) staff       (20)    30116 2023-05-22 16:23:48.000000 chainforge-0.1.1/chainforge/flask_app.py
-drwxr-xr-x   0 ianarawjo   (501) staff       (20)        0 2023-05-22 17:32:43.666773 chainforge-0.1.1/chainforge/promptengine/
--rw-r--r--   0 ianarawjo   (501) staff       (20)        1 2023-05-18 04:19:30.000000 chainforge-0.1.1/chainforge/promptengine/__init__.py
-drwxr-xr-x   0 ianarawjo   (501) staff       (20)        0 2023-05-22 17:32:43.668134 chainforge-0.1.1/chainforge/promptengine/dalaipy/
--rw-r--r--   0 ianarawjo   (501) staff       (20)       43 2023-05-18 04:19:30.000000 chainforge-0.1.1/chainforge/promptengine/dalaipy/__init__.py
--rw-r--r--   0 ianarawjo   (501) staff       (20)     4002 2023-05-18 04:19:30.000000 chainforge-0.1.1/chainforge/promptengine/dalaipy/main.py
--rw-r--r--   0 ianarawjo   (501) staff       (20)     1972 2023-05-20 01:57:45.000000 chainforge-0.1.1/chainforge/promptengine/models.py
--rw-r--r--   0 ianarawjo   (501) staff       (20)    10245 2023-05-20 02:13:24.000000 chainforge-0.1.1/chainforge/promptengine/query.py
--rw-r--r--   0 ianarawjo   (501) staff       (20)     7161 2023-05-19 20:09:20.000000 chainforge-0.1.1/chainforge/promptengine/template.py
--rw-r--r--   0 ianarawjo   (501) staff       (20)    12861 2023-05-21 13:44:51.000000 chainforge-0.1.1/chainforge/promptengine/utils.py
-drwxr-xr-x   0 ianarawjo   (501) staff       (20)        0 2023-05-22 17:32:43.656686 chainforge-0.1.1/chainforge/react-server/
-drwxr-xr-x   0 ianarawjo   (501) staff       (20)        0 2023-05-22 17:32:43.671946 chainforge-0.1.1/chainforge/react-server/build/
--rw-r--r--   0 ianarawjo   (501) staff       (20)     6148 2023-05-22 17:32:01.000000 chainforge-0.1.1/chainforge/react-server/build/.DS_Store
--rw-r--r--   0 ianarawjo   (501) staff       (20)      517 2023-05-22 17:31:52.000000 chainforge-0.1.1/chainforge/react-server/build/asset-manifest.json
--rw-r--r--   0 ianarawjo   (501) staff       (20)    17470 2023-05-22 17:30:47.000000 chainforge-0.1.1/chainforge/react-server/build/favicon.ico
--rw-r--r--   0 ianarawjo   (501) staff       (20)      645 2023-05-22 17:31:52.000000 chainforge-0.1.1/chainforge/react-server/build/index.html
--rw-r--r--   0 ianarawjo   (501) staff       (20)    18595 2023-05-22 17:30:47.000000 chainforge-0.1.1/chainforge/react-server/build/logo192.png
--rw-r--r--   0 ianarawjo   (501) staff       (20)    18375 2023-05-22 17:30:47.000000 chainforge-0.1.1/chainforge/react-server/build/logo512.png
--rw-r--r--   0 ianarawjo   (501) staff       (20)      492 2023-05-22 17:30:47.000000 chainforge-0.1.1/chainforge/react-server/build/manifest.json
--rw-r--r--   0 ianarawjo   (501) staff       (20)       67 2023-05-22 17:30:47.000000 chainforge-0.1.1/chainforge/react-server/build/robots.txt
-drwxr-xr-x   0 ianarawjo   (501) staff       (20)        0 2023-05-22 17:32:43.673619 chainforge-0.1.1/chainforge/react-server/build/static/
-drwxr-xr-x   0 ianarawjo   (501) staff       (20)        0 2023-05-22 17:32:43.674632 chainforge-0.1.1/chainforge/react-server/build/static/css/
--rw-r--r--   0 ianarawjo   (501) staff       (20)     9920 2023-05-22 17:31:52.000000 chainforge-0.1.1/chainforge/react-server/build/static/css/main.1e595843.css
--rw-r--r--   0 ianarawjo   (501) staff       (20)    19973 2023-05-22 17:31:52.000000 chainforge-0.1.1/chainforge/react-server/build/static/css/main.1e595843.css.map
--rw-r--r--   0 ianarawjo   (501) staff       (20)    17470 2023-05-22 17:30:47.000000 chainforge-0.1.1/chainforge/react-server/build/static/favicon.ico
-drwxr-xr-x   0 ianarawjo   (501) staff       (20)        0 2023-05-22 17:32:43.684282 chainforge-0.1.1/chainforge/react-server/build/static/js/
--rw-r--r--   0 ianarawjo   (501) staff       (20)     4603 2023-05-22 17:31:52.000000 chainforge-0.1.1/chainforge/react-server/build/static/js/787.4c72bb55.chunk.js
--rw-r--r--   0 ianarawjo   (501) staff       (20)    10592 2023-05-22 17:31:52.000000 chainforge-0.1.1/chainforge/react-server/build/static/js/787.4c72bb55.chunk.js.map
--rw-r--r--   0 ianarawjo   (501) staff       (20)  5257931 2023-05-22 17:31:52.000000 chainforge-0.1.1/chainforge/react-server/build/static/js/main.8fcca0e8.js
--rw-r--r--   0 ianarawjo   (501) staff       (20)     6168 2023-05-22 17:31:52.000000 chainforge-0.1.1/chainforge/react-server/build/static/js/main.8fcca0e8.js.LICENSE.txt
--rw-r--r--   0 ianarawjo   (501) staff       (20)  6176695 2023-05-22 17:31:52.000000 chainforge-0.1.1/chainforge/react-server/build/static/js/main.8fcca0e8.js.map
--rw-r--r--   0 ianarawjo   (501) staff       (20)    18595 2023-05-22 17:30:47.000000 chainforge-0.1.1/chainforge/react-server/build/static/logo192.png
--rw-r--r--   0 ianarawjo   (501) staff       (20)    18375 2023-05-22 17:30:47.000000 chainforge-0.1.1/chainforge/react-server/build/static/logo512.png
--rw-r--r--   0 ianarawjo   (501) staff       (20)      492 2023-05-22 17:30:47.000000 chainforge-0.1.1/chainforge/react-server/build/static/manifest.json
-drwxr-xr-x   0 ianarawjo   (501) staff       (20)        0 2023-05-22 17:32:43.663102 chainforge-0.1.1/chainforge.egg-info/
--rw-r--r--   0 ianarawjo   (501) staff       (20)      576 2023-05-22 17:32:43.000000 chainforge-0.1.1/chainforge.egg-info/PKG-INFO
--rw-r--r--   0 ianarawjo   (501) staff       (20)     1545 2023-05-22 17:32:43.000000 chainforge-0.1.1/chainforge.egg-info/SOURCES.txt
--rw-r--r--   0 ianarawjo   (501) staff       (20)        1 2023-05-22 17:32:43.000000 chainforge-0.1.1/chainforge.egg-info/dependency_links.txt
--rw-r--r--   0 ianarawjo   (501) staff       (20)       51 2023-05-22 17:32:43.000000 chainforge-0.1.1/chainforge.egg-info/entry_points.txt
--rw-r--r--   0 ianarawjo   (501) staff       (20)      110 2023-05-22 17:32:43.000000 chainforge-0.1.1/chainforge.egg-info/requires.txt
--rw-r--r--   0 ianarawjo   (501) staff       (20)       11 2023-05-22 17:32:43.000000 chainforge-0.1.1/chainforge.egg-info/top_level.txt
--rw-r--r--   0 ianarawjo   (501) staff       (20)       38 2023-05-22 17:32:43.694540 chainforge-0.1.1/setup.cfg
--rw-r--r--   0 ianarawjo   (501) staff       (20)     1098 2023-05-22 17:18:56.000000 chainforge-0.1.1/setup.py
+drwxr-xr-x   0 ianarawjo   (501) staff       (20)        0 2023-05-23 19:13:32.360008 chainforge-0.1.2/
+-rw-r--r--   0 ianarawjo   (501) staff       (20)     1067 2023-04-11 20:15:11.000000 chainforge-0.1.2/LICENSE.md
+-rw-r--r--   0 ianarawjo   (501) staff       (20)       53 2023-05-23 19:05:23.000000 chainforge-0.1.2/MANIFEST.in
+-rw-r--r--   0 ianarawjo   (501) staff       (20)     8952 2023-05-23 19:13:32.359056 chainforge-0.1.2/PKG-INFO
+-rw-r--r--   0 ianarawjo   (501) staff       (20)     8269 2023-05-23 18:29:50.000000 chainforge-0.1.2/README.md
+drwxr-xr-x   0 ianarawjo   (501) staff       (20)        0 2023-05-23 19:13:32.323786 chainforge-0.1.2/chainforge/
+-rw-r--r--   0 ianarawjo   (501) staff       (20)       22 2023-05-18 04:19:30.000000 chainforge-0.1.2/chainforge/__init__.py
+-rw-r--r--   0 ianarawjo   (501) staff       (20)     4801 2023-05-18 04:19:30.000000 chainforge-0.1.2/chainforge/app.py
+-rw-r--r--   0 ianarawjo   (501) staff       (20)    30302 2023-05-23 18:52:35.000000 chainforge-0.1.2/chainforge/flask_app.py
+drwxr-xr-x   0 ianarawjo   (501) staff       (20)        0 2023-05-23 19:13:32.331569 chainforge-0.1.2/chainforge/promptengine/
+-rw-r--r--   0 ianarawjo   (501) staff       (20)        1 2023-05-18 04:19:30.000000 chainforge-0.1.2/chainforge/promptengine/__init__.py
+drwxr-xr-x   0 ianarawjo   (501) staff       (20)        0 2023-05-23 19:13:32.332985 chainforge-0.1.2/chainforge/promptengine/dalaipy/
+-rw-r--r--   0 ianarawjo   (501) staff       (20)       43 2023-05-18 04:19:30.000000 chainforge-0.1.2/chainforge/promptengine/dalaipy/__init__.py
+-rw-r--r--   0 ianarawjo   (501) staff       (20)     4002 2023-05-18 04:19:30.000000 chainforge-0.1.2/chainforge/promptengine/dalaipy/main.py
+-rw-r--r--   0 ianarawjo   (501) staff       (20)     1972 2023-05-20 01:57:45.000000 chainforge-0.1.2/chainforge/promptengine/models.py
+-rw-r--r--   0 ianarawjo   (501) staff       (20)    10245 2023-05-20 02:13:24.000000 chainforge-0.1.2/chainforge/promptengine/query.py
+-rw-r--r--   0 ianarawjo   (501) staff       (20)     7161 2023-05-19 20:09:20.000000 chainforge-0.1.2/chainforge/promptengine/template.py
+-rw-r--r--   0 ianarawjo   (501) staff       (20)    13095 2023-05-23 18:28:08.000000 chainforge-0.1.2/chainforge/promptengine/utils.py
+drwxr-xr-x   0 ianarawjo   (501) staff       (20)        0 2023-05-23 19:13:32.319727 chainforge-0.1.2/chainforge/react-server/
+drwxr-xr-x   0 ianarawjo   (501) staff       (20)        0 2023-05-23 19:13:32.337527 chainforge-0.1.2/chainforge/react-server/build/
+-rw-r--r--   0 ianarawjo   (501) staff       (20)     6148 2023-05-23 19:13:08.000000 chainforge-0.1.2/chainforge/react-server/build/.DS_Store
+-rw-r--r--   0 ianarawjo   (501) staff       (20)      517 2023-05-23 19:12:50.000000 chainforge-0.1.2/chainforge/react-server/build/asset-manifest.json
+-rw-r--r--   0 ianarawjo   (501) staff       (20)    17470 2023-05-23 19:11:40.000000 chainforge-0.1.2/chainforge/react-server/build/favicon.ico
+-rw-r--r--   0 ianarawjo   (501) staff       (20)      645 2023-05-23 19:12:50.000000 chainforge-0.1.2/chainforge/react-server/build/index.html
+-rw-r--r--   0 ianarawjo   (501) staff       (20)    18595 2023-05-23 19:11:40.000000 chainforge-0.1.2/chainforge/react-server/build/logo192.png
+-rw-r--r--   0 ianarawjo   (501) staff       (20)    18375 2023-05-23 19:11:40.000000 chainforge-0.1.2/chainforge/react-server/build/logo512.png
+-rw-r--r--   0 ianarawjo   (501) staff       (20)      492 2023-05-23 19:11:40.000000 chainforge-0.1.2/chainforge/react-server/build/manifest.json
+-rw-r--r--   0 ianarawjo   (501) staff       (20)       67 2023-05-23 19:11:40.000000 chainforge-0.1.2/chainforge/react-server/build/robots.txt
+drwxr-xr-x   0 ianarawjo   (501) staff       (20)        0 2023-05-23 19:13:32.339266 chainforge-0.1.2/chainforge/react-server/build/static/
+drwxr-xr-x   0 ianarawjo   (501) staff       (20)        0 2023-05-23 19:13:32.339940 chainforge-0.1.2/chainforge/react-server/build/static/css/
+-rw-r--r--   0 ianarawjo   (501) staff       (20)     9920 2023-05-23 19:12:50.000000 chainforge-0.1.2/chainforge/react-server/build/static/css/main.1e595843.css
+-rw-r--r--   0 ianarawjo   (501) staff       (20)    19973 2023-05-23 19:12:50.000000 chainforge-0.1.2/chainforge/react-server/build/static/css/main.1e595843.css.map
+-rw-r--r--   0 ianarawjo   (501) staff       (20)    17470 2023-05-23 19:11:40.000000 chainforge-0.1.2/chainforge/react-server/build/static/favicon.ico
+drwxr-xr-x   0 ianarawjo   (501) staff       (20)        0 2023-05-23 19:13:32.348194 chainforge-0.1.2/chainforge/react-server/build/static/js/
+-rw-r--r--   0 ianarawjo   (501) staff       (20)     4603 2023-05-23 19:12:50.000000 chainforge-0.1.2/chainforge/react-server/build/static/js/787.4c72bb55.chunk.js
+-rw-r--r--   0 ianarawjo   (501) staff       (20)    10592 2023-05-23 19:12:50.000000 chainforge-0.1.2/chainforge/react-server/build/static/js/787.4c72bb55.chunk.js.map
+-rw-r--r--   0 ianarawjo   (501) staff       (20)  5257931 2023-05-23 19:12:50.000000 chainforge-0.1.2/chainforge/react-server/build/static/js/main.8fcca0e8.js
+-rw-r--r--   0 ianarawjo   (501) staff       (20)     6168 2023-05-23 19:12:50.000000 chainforge-0.1.2/chainforge/react-server/build/static/js/main.8fcca0e8.js.LICENSE.txt
+-rw-r--r--   0 ianarawjo   (501) staff       (20)  6176695 2023-05-23 19:12:50.000000 chainforge-0.1.2/chainforge/react-server/build/static/js/main.8fcca0e8.js.map
+-rw-r--r--   0 ianarawjo   (501) staff       (20)    18595 2023-05-23 19:11:40.000000 chainforge-0.1.2/chainforge/react-server/build/static/logo192.png
+-rw-r--r--   0 ianarawjo   (501) staff       (20)    18375 2023-05-23 19:11:40.000000 chainforge-0.1.2/chainforge/react-server/build/static/logo512.png
+-rw-r--r--   0 ianarawjo   (501) staff       (20)      492 2023-05-23 19:11:40.000000 chainforge-0.1.2/chainforge/react-server/build/static/manifest.json
+drwxr-xr-x   0 ianarawjo   (501) staff       (20)        0 2023-05-23 19:13:32.326817 chainforge-0.1.2/chainforge.egg-info/
+-rw-r--r--   0 ianarawjo   (501) staff       (20)     8952 2023-05-23 19:13:32.000000 chainforge-0.1.2/chainforge.egg-info/PKG-INFO
+-rw-r--r--   0 ianarawjo   (501) staff       (20)     1545 2023-05-23 19:13:32.000000 chainforge-0.1.2/chainforge.egg-info/SOURCES.txt
+-rw-r--r--   0 ianarawjo   (501) staff       (20)        1 2023-05-23 19:13:32.000000 chainforge-0.1.2/chainforge.egg-info/dependency_links.txt
+-rw-r--r--   0 ianarawjo   (501) staff       (20)       51 2023-05-23 19:13:32.000000 chainforge-0.1.2/chainforge.egg-info/entry_points.txt
+-rw-r--r--   0 ianarawjo   (501) staff       (20)      153 2023-05-23 19:13:32.000000 chainforge-0.1.2/chainforge.egg-info/requires.txt
+-rw-r--r--   0 ianarawjo   (501) staff       (20)       11 2023-05-23 19:13:32.000000 chainforge-0.1.2/chainforge.egg-info/top_level.txt
+-rw-r--r--   0 ianarawjo   (501) staff       (20)       38 2023-05-23 19:13:32.360289 chainforge-0.1.2/setup.cfg
+-rw-r--r--   0 ianarawjo   (501) staff       (20)     1406 2023-05-23 19:10:42.000000 chainforge-0.1.2/setup.py
```

### Comparing `chainforge-0.1.1/LICENSE.md` & `chainforge-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `chainforge-0.1.1/README.md` & `chainforge-0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # ⛓️🛠️ ChainForge
 **An open-source visual programming environment for battle-testing prompts to LLMs.**
 
-<img width="1599" alt="prompt-injection-test" src="https://github.com/ianarawjo/ChainForge/assets/5251713/f6366269-39e9-472d-afc3-5e09c513ccfa">
+<img width="1599" alt="prompt-injection-test" src="https://github.com/ianarawjo/ChainForge/assets/5251713/83757804-4288-4fc2-b28d-fd0826bae6a1">
 
 ChainForge is a data flow prompt engineering environment for analyzing and evaluating LLM responses. It is geared towards early-stage, quick-and-dirty exploration of prompts and response quality that goes beyond ad-hoc chatting with individual LLMs. With ChainForge, you can: 
  - Query multiple LLMs at once to test prompt ideas and variations quickly and effectively. 
  - Compare response quality across prompt permutations and across models to choose the best prompt and model for your use case. 
  - Setup an evaluation metric (scoring function) and immediately visualize results across prompts, prompt parameters, and models. 
 
 **This is an open alpha of Chainforge.** Functionality is powerful but limited. We currently support OpenAI models GPT3.5 and GPT4, Anthropic's Claude, Google PaLM2 (text-bison), and Alpaca 7B (through [Dalai](https://github.com/cocktailpeanut/dalai)) at default settings. Visualization nodes support numeric and boolean evaluation metrics. Try it and let us know what you'd like to see in the future! :)
@@ -31,15 +31,15 @@
 You can set your API keys by clicking the Settings icon in the top-right corner. If you prefer to not worry about this everytime you open ChainForge, we recommend that save your OpenAI, Anthropic, and/or Google PaLM API keys to your local environment. For more details, see the [Installation Guide](https://github.com/ianarawjo/ChainForge/blob/main/INSTALL_GUIDE.md).
 
 ## Example evaluation flows
 
 In the `examples/` folder, we've prepared a couple example flows to give you a sense of what's possible with Chainforge.
 Click the Import button in the top of the screen and select one. Here is `basic_comparison.cforge`, plotting the length of responses across different models and arguments for the prompt parameter `{game}`:
 
-<img width="1593" alt="basic-compare" src="https://github.com/ianarawjo/ChainForge/assets/5251713/e15bd13c-ea6b-4934-be7f-b8081339c8d5">
+<img width="1593" alt="basic-compare" src="https://github.com/ianarawjo/ChainForge/assets/5251713/43c87ab7-aabd-41ba-8d9b-e7e9ebe25c75">
 
 For more details about features and available nodes, check out the [User Guide](https://github.com/ianarawjo/ChainForge/blob/main/GUIDE.md).
 
 # Features
 
 A key goal of ChainForge is facilitating **comparison** and **evaluation** of prompts and models, and (in the near future) prompt chains. Basic features are:
 - **Prompt permutations**: Setup a prompt template and feed it variations of input variables. ChainForge will prompt all selected LLMs with all possible permutations of the input prompt, so that you can get a better sense of prompt quality. You can also chain prompt templates at arbitrary depth (e.g., to compare templates).
```

### Comparing `chainforge-0.1.1/chainforge/app.py` & `chainforge-0.1.2/chainforge/app.py`

 * *Files identical despite different names*

### Comparing `chainforge-0.1.1/chainforge/flask_app.py` & `chainforge-0.1.2/chainforge/flask_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,14 +227,17 @@
                 'items': flat_eval_res
             }
         })
     
     return ret
 
 def load_all_cached_responses(cache_ids):
+    # Create a cache dir if it doesn't exist:
+    create_dir_if_not_exists(CACHE_DIR)
+
     if not isinstance(cache_ids, list):
         cache_ids = [cache_ids]
     
     # Load all responses with the given ID:
     all_cache_files = get_files_at_dir(CACHE_DIR)
     responses = []
     for cache_id in cache_ids:
@@ -353,15 +356,15 @@
         POST'd data should be in the form: 
         {
             'id': str  # a unique ID to refer to this information. Used when cache'ing responses. 
             'llm': str | list  # a string or list of strings specifying the LLM(s) to query
             'params': dict  # an optional dict of any other params to set when querying the LLMs, like 'temperature', 'n' (num of responses per prompt), etc.
             'prompt': str  # the prompt template, with any {{}} vars
             'vars': dict  # a dict of the template variables to fill the prompt template with, by name. For each var, can be single values or a list; in the latter, all permutations are passed. (Pass empty dict if no vars.)
-            'api_keys': dict  # (optional) a dict of {api_name: api_key} pairs. Supported keys: OpenAI, Anthropic.
+            'api_keys': dict  # (optional) a dict of {api_name: api_key} pairs. Supported key names: OpenAI, Anthropic, Google
             'no_cache': bool (optional)  # delete any cache'd responses for 'id' (always call the LLM fresh)
         }
     """
     data = request.get_json()
 
     # Check that all required info is here:
     if not set(data.keys()).issuperset({'llm', 'prompt', 'vars', 'id'}):
@@ -699,14 +702,17 @@
     data = request.get_json()
     if 'files' not in data:
         return jsonify({'result': False, 'error': 'Missing files parameter to importData.'})
     elif not isinstance(data['files'], dict):
         typeof_files = data['files']
         return jsonify({'result': False, 'error': f'Files parameter in importData should be a dict, but is of type {typeof_files}.'})
 
+    # Create a cache dir if it doesn't exist:
+    create_dir_if_not_exists(CACHE_DIR)
+
     # Verify filenames, data, and access permissions to write to cache
     for filename in data['files']:
         # Verify filepath
         cache_filepath = os.path.join(CACHE_DIR, filename)
         if not is_valid_filepath(cache_filepath):
             return jsonify({'result': False, 'error': f'Invalid filepath: {cache_filepath}'})
```

### Comparing `chainforge-0.1.1/chainforge/promptengine/dalaipy/main.py` & `chainforge-0.1.2/chainforge/promptengine/dalaipy/main.py`

 * *Files identical despite different names*

### Comparing `chainforge-0.1.1/chainforge/promptengine/models.py` & `chainforge-0.1.2/chainforge/promptengine/models.py`

 * *Files identical despite different names*

### Comparing `chainforge-0.1.1/chainforge/promptengine/query.py` & `chainforge-0.1.2/chainforge/promptengine/query.py`

 * *Files identical despite different names*

### Comparing `chainforge-0.1.1/chainforge/promptengine/template.py` & `chainforge-0.1.2/chainforge/promptengine/template.py`

 * *Files identical despite different names*

### Comparing `chainforge-0.1.1/chainforge/promptengine/utils.py` & `chainforge-0.1.2/chainforge/promptengine/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         "n": n,
         "temperature": temperature,
     }
     try:
         response = await openai.ChatCompletion.acreate(**query)
     except Exception as e:
         if (isinstance(e, openai.error.AuthenticationError)):
-            raise Exception("Could not authenticate to OpenAI. Double-check your API key.")
+            raise Exception("Could not authenticate to OpenAI. Double-check that your API key is set in Settings or in your local Python environment.")
         raise e
     return query, response
 
 async def call_anthropic(prompt: str, model: LLM, n: int = 1, temperature: float= 1.0,
                         custom_prompt_wrapper: Union[Callable[[str], str], None]=None,
                         max_tokens_to_sample=1024,
                         stop_sequences: Union[List[str], str]=["\n\nHuman:"],
@@ -88,15 +88,15 @@
             - stop_sequences: A list of strings upon which to stop generating. Defaults to ["\n\nHuman:"], the cue for the next turn in the dialog agent.
             - async_mode: Evaluation access to Claude limits calls to 1 at a time, meaning we can't take advantage of async.
                           If you want to send all 'n' requests at once, you can set async_mode to True.
 
         NOTE: It is recommended to set an environment variable ANTHROPIC_API_KEY with your Anthropic API key
     """
     if ANTHROPIC_API_KEY is None:
-        raise Exception("Could not find an API key for Anthropic models.")
+        raise Exception("Could not find an API key for Anthropic models. Double-check that your API key is set in Settings or in your local Python environment.")
 
     import anthropic
     client = anthropic.Client(ANTHROPIC_API_KEY)
 
     # Format query
     query = {
         'model': model.value,
@@ -129,15 +129,15 @@
                            async_mode=False,
                            **params) -> Tuple[Dict, Dict]:
     """
         Calls a Google PaLM model. 
         Returns raw query and response JSON dicts.
     """
     if GOOGLE_PALM_API_KEY is None:
-        raise Exception("Could not find an API key for Google PaLM models.")
+        raise Exception("Could not find an API key for Google PaLM models. Double-check that your API key is set in Settings or in your local Python environment.")
 
     import google.generativeai as palm
     palm.configure(api_key=GOOGLE_PALM_API_KEY)
 
     query = {
         'model': f"models/{model.value}",
         'prompt': prompt,
```

### Comparing `chainforge-0.1.1/chainforge/react-server/build/.DS_Store` & `chainforge-0.1.2/chainforge/react-server/build/.DS_Store`

 * *Files 20% similar despite different names*

```diff
@@ -36,16 +36,16 @@
 00000230: d701 0203 0405 0607 0809 0908 090d 095d  ...............]
 00000240: 5368 6f77 5374 6174 7573 4261 725b 5368  ShowStatusBar[Sh
 00000250: 6f77 5061 7468 6261 725b 5368 6f77 546f  owPathbar[ShowTo
 00000260: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
 00000270: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
 00000280: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
 00000290: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
-000002a0: 7208 0909 0809 5f10 187b 7b37 3230 2c20  r....._..{{720, 
-000002b0: 3134 347d 2c20 7b39 3831 2c20 3631 357d  144}, {981, 615}
+000002a0: 7208 0909 0809 5f10 187b 7b34 3936 2c20  r....._..{{496, 
+000002b0: 3135 337d 2c20 7b39 3831 2c20 3631 357d  153}, {981, 615}
 000002c0: 7d09 0817 2531 3d49 606d 797a 7b7c 7d7e  }...%1=I`myz{|}~
 000002d0: 9900 0000 0000 0001 0100 0000 0000 0000  ................
 000002e0: 0f00 0000 0000 0000 0000 0000 0000 0000  ................
 000002f0: 9a00 0000 0600 7300 7400 6100 7400 6900  ......s.t.a.t.i.
 00000300: 6376 5372 6e6c 6f6e 6700 0000 0100 0000  cvSrnlong.......
 00000310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000320: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `chainforge-0.1.1/chainforge/react-server/build/asset-manifest.json` & `chainforge-0.1.2/chainforge/react-server/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `chainforge-0.1.1/chainforge/react-server/build/favicon.ico` & `chainforge-0.1.2/chainforge/react-server/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `chainforge-0.1.1/chainforge/react-server/build/index.html` & `chainforge-0.1.2/chainforge/react-server/build/index.html`

 * *Files identical despite different names*

### Comparing `chainforge-0.1.1/chainforge/react-server/build/logo192.png` & `chainforge-0.1.2/chainforge/react-server/build/logo192.png`

 * *Files identical despite different names*

### Comparing `chainforge-0.1.1/chainforge/react-server/build/logo512.png` & `chainforge-0.1.2/chainforge/react-server/build/logo512.png`

 * *Files identical despite different names*

### Comparing `chainforge-0.1.1/chainforge/react-server/build/static/css/main.1e595843.css` & `chainforge-0.1.2/chainforge/react-server/build/static/css/main.1e595843.css`

 * *Files identical despite different names*

### Comparing `chainforge-0.1.1/chainforge/react-server/build/static/css/main.1e595843.css.map` & `chainforge-0.1.2/chainforge/react-server/build/static/css/main.1e595843.css.map`

 * *Files identical despite different names*

### Comparing `chainforge-0.1.1/chainforge/react-server/build/static/favicon.ico` & `chainforge-0.1.2/chainforge/react-server/build/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `chainforge-0.1.1/chainforge/react-server/build/static/js/787.4c72bb55.chunk.js` & `chainforge-0.1.2/chainforge/react-server/build/static/js/787.4c72bb55.chunk.js`

 * *Files identical despite different names*

### Comparing `chainforge-0.1.1/chainforge/react-server/build/static/js/787.4c72bb55.chunk.js.map` & `chainforge-0.1.2/chainforge/react-server/build/static/js/787.4c72bb55.chunk.js.map`

 * *Files identical despite different names*

### Comparing `chainforge-0.1.1/chainforge/react-server/build/static/js/main.8fcca0e8.js` & `chainforge-0.1.2/chainforge/react-server/build/static/js/main.8fcca0e8.js`

 * *Files identical despite different names*

### Comparing `chainforge-0.1.1/chainforge/react-server/build/static/js/main.8fcca0e8.js.LICENSE.txt` & `chainforge-0.1.2/chainforge/react-server/build/static/js/main.8fcca0e8.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chainforge-0.1.1/chainforge/react-server/build/static/js/main.8fcca0e8.js.map` & `chainforge-0.1.2/chainforge/react-server/build/static/js/main.8fcca0e8.js.map`

 * *Files identical despite different names*

### Comparing `chainforge-0.1.1/chainforge/react-server/build/static/logo192.png` & `chainforge-0.1.2/chainforge/react-server/build/static/logo192.png`

 * *Files identical despite different names*

### Comparing `chainforge-0.1.1/chainforge/react-server/build/static/logo512.png` & `chainforge-0.1.2/chainforge/react-server/build/static/logo512.png`

 * *Files identical despite different names*

### Comparing `chainforge-0.1.1/chainforge.egg-info/SOURCES.txt` & `chainforge-0.1.2/chainforge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chainforge-0.1.1/setup.py` & `chainforge-0.1.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,37 @@
 from setuptools import setup, find_packages
 
+def readme():
+    with open('README.md') as f:
+        return f.read()
+
 setup(
     name='chainforge',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),
     author="Ian Arawjo",
     description="A Visual Programming Environment for Prompt Engineering",
+    long_description=readme(),
+    long_description_content_type='text/markdown',
+    keywords='prompt engineering LLM response evaluation',
+    license="MIT",
     url="https://github.com/ianarawjo/ChainForge/",
     install_requires=[
         # Package dependencies
+        "flask>=2.2.3",
         "flask[async]",
         "flask_cors",
         "flask_socketio",
-        "openai",
         "python-socketio",
-        "dalaipy>=2.0.2",
         "gevent-websocket",
         "urllib3==1.26.6",
+        "openai",
+        "anthropic",
+        "google-generativeai",
+        "dalaipy>=2.0.2",
     ],
     entry_points={
         'console_scripts': [
             'chainforge = chainforge.app:main',
         ],
     },
     classifiers=[
```

