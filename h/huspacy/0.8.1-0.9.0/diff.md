# Comparing `tmp/huspacy-0.8.1-py3-none-any.whl.zip` & `tmp/huspacy-0.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 92285 bytes, number of entries: 17
--rw-r--r--  2.0 unx     3889 b- defN 80-Jan-01 00:00 huspacy/__init__.py
+Zip file size: 92314 bytes, number of entries: 17
+-rw-r--r--  2.0 unx     3973 b- defN 80-Jan-01 00:00 huspacy/__init__.py
 -rw-r--r--  2.0 unx      102 b- defN 80-Jan-01 00:00 huspacy/components/__init__.py
 -rw-r--r--  2.0 unx    17063 b- defN 80-Jan-01 00:00 huspacy/components/edit_tree_lemmatizer.py
 -rw-r--r--  2.0 unx     3237 b- defN 80-Jan-01 00:00 huspacy/components/lemma_postprocessing.py
 -rw-r--r--  2.0 unx     5077 b- defN 80-Jan-01 00:00 huspacy/components/lookup_lemmatizer.py
 -rw-r--r--  2.0 unx       60 b- defN 80-Jan-01 00:00 huspacy/extra/__init__.py
 -rw-r--r--  2.0 unx     1635 b- defN 80-Jan-01 00:00 huspacy/extra/roman_num_converter.py
 -rw-r--r--  2.0 unx     2059 b- defN 80-Jan-01 00:00 huspacy/extra/sentencizer.py
 -rw-r--r--  2.0 unx       44 b- defN 80-Jan-01 00:00 huspacy/integrations/__init__.py
 -rw-r--r--  2.0 unx     2413 b- defN 80-Jan-01 00:00 huspacy/integrations/nerpp.py
 -rw-r--r--  2.0 unx     4063 b- defN 80-Jan-01 00:00 huspacy/integrations/sentiment.py
 -rw-r--r--  2.0 unx   541963 b- defN 80-Jan-01 00:00 huspacy/resources/poltext_sentiment.json
 -rw-r--r--  2.0 unx   791334 b- defN 80-Jan-01 00:00 huspacy/resources/precognox_sentiment.json
 -rw-r--r--  2.0 unx     2103 b- defN 80-Jan-01 00:00 huspacy/utils.py
--rw-r--r--  2.0 unx    12182 b- defN 80-Jan-01 00:00 huspacy-0.8.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 huspacy-0.8.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1458 b- defN 16-Jan-01 00:00 huspacy-0.8.1.dist-info/RECORD
-17 files, 1388770 bytes uncompressed, 89883 bytes compressed:  93.5%
+?rw-r--r--  2.0 unx       88 b- defN 16-Jan-01 00:00 huspacy-0.9.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx    12245 b- defN 16-Jan-01 00:00 huspacy-0.9.0.dist-info/METADATA
+?rw-r--r--  2.0 unx     1458 b- defN 16-Jan-01 00:00 huspacy-0.9.0.dist-info/RECORD
+17 files, 1388917 bytes uncompressed, 89912 bytes compressed:  93.5%
```

## zipnote {}

```diff
@@ -36,17 +36,17 @@
 
 Filename: huspacy/resources/precognox_sentiment.json
 Comment: 
 
 Filename: huspacy/utils.py
 Comment: 
 
-Filename: huspacy-0.8.1.dist-info/METADATA
+Filename: huspacy-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: huspacy-0.8.1.dist-info/WHEEL
+Filename: huspacy-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: huspacy-0.8.1.dist-info/RECORD
+Filename: huspacy-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## huspacy/__init__.py

```diff
@@ -8,18 +8,19 @@
 from huspacy.utils import run_command
 
 __URL = "https://huggingface.co/huspacy/{model_name}/resolve/{version}/{model_name}-any-py3-none-any.whl"
 __DEFAULT_VERSION = "main"
 __DEFAULT_MODEL = "hu_core_news_lg"
 
 __AVAILABLE_MODELS: Dict[str, List[str]] = {
-    "hu_core_news_lg": ["3.2.1", "3.2.2", "3.3.0", "3.3.1", "3.4.0", "3.4.1", "3.4.2", "3.4.3", "3.4.4", "3.5.0", "3.5.1"],
-    "hu_core_news_md": ["3.4.1", "3.4.2", "3.5.0", "3.5.1"],
-    "hu_core_news_trf": ["3.2.0", "3.2.1", "3.2.2", "3.2.3", "3.2.4", "3.4.0", "3.5.1"],
-    "hu_core_news_trf_xl": ["3.4.0", "3.5.1"],
+    "hu_core_news_lg": ["3.2.1", "3.2.2", "3.3.0", "3.3.1", "3.4.0", "3.4.1", "3.4.2", "3.4.3", "3.4.4", "3.5.0",
+                        "3.5.1", "3.5.2"],
+    "hu_core_news_md": ["3.4.1", "3.4.2", "3.5.0", "3.5.1", "3.5.2"],
+    "hu_core_news_trf": ["3.2.0", "3.2.1", "3.2.2", "3.2.3", "3.2.4", "3.4.0", "3.5.1", "3.5.2"],
+    "hu_core_news_trf_xl": ["3.4.0", "3.5.1", "3.5.2"],
 }
 
 
 def get_valid_models(spacy_version: Optional[str] = None) -> Dict[str, List[str]]:
     """
     Returns valid model names and versions for the given spacy version
 
@@ -51,32 +52,32 @@
         model_version (str): model version, if not provided it defaults to the latest version ("main")
 
     Returns:
         None
     """
     assert model_name in __AVAILABLE_MODELS, f"{model_name} is not a valid model name"
     assert (
-        model_version == "main" or model_version in __AVAILABLE_MODELS[model_name]
+            model_version == "main" or model_version in __AVAILABLE_MODELS[model_name]
     ), f"{model_version} is not a valid version for {model_name}"
 
     if model_version != __DEFAULT_VERSION:
         model_version = "v" + model_version
 
     download_url = __URL.format(version=model_version, model_name=model_name)
     cmd = [sys.executable, "-m", "pip", "install"] + [download_url]
     run_command(cmd)
 
 
 # noinspection PyDefaultArgument,PyUnresolvedReferences
 def load(
-    name: Union[str, Path] = __DEFAULT_MODEL,
-    vocab: Union["Vocab", bool] = True,
-    disable: Optional[Iterable[str]] = None,
-    exclude: Optional[Iterable[str]] = None,
-    config: Union[Dict[str, Any], "Config", None] = None,
+        name: Union[str, Path] = __DEFAULT_MODEL,
+        vocab: Union["Vocab", bool] = True,
+        disable: Optional[Iterable[str]] = None,
+        exclude: Optional[Iterable[str]] = None,
+        config: Union[Dict[str, Any], "Config", None] = None,
 ) -> "Language":
     """Loads a HuSpaCy model.
 
     Args:
         name (str): model name, if not provided it defaults to `hu_core_news_lg`
         vocab (Vocab): A Vocab object. If True, a vocab is created.
         disable (Iterable[str]): Names of pipeline components to disable. Disabled pipes will be loaded, but they
```

## Comparing `huspacy-0.8.1.dist-info/METADATA` & `huspacy-0.9.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huspacy
-Version: 0.8.1
+Version: 0.9.0
 Summary: HuSpaCy: industrial strength Hungarian natural language processing
 Home-page: https://github.com/huspacy/huspacy
 License: Apache-2.0
 Keywords: nlp,huspacy,Hungarian,text processing,text processing,language processing,text mining,tokenization,sentence boundary detection,sbd,sentence splitting,pos tagging,tagging,lemmatization,ner,named entity recognition,parsing,word embeddings,word vectors,spacy,spacy model
 Author: SzegedAI, MILAB
 Author-email: gyorgy@orosz.link
 Maintainer: György Orosz
@@ -26,20 +26,22 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: Linguistic
+Provides-Extra: np
 Provides-Extra: trf
-Requires-Dist: importlib_resources ; python_version < "3.9"
+Requires-Dist: benepar (==0.2.0); extra == "np"
+Requires-Dist: importlib_resources; python_version < "3.9"
 Requires-Dist: packaging (>=21.3,<22.0)
-Requires-Dist: spacy-alignments (>=0.8.6,<0.9.0) ; extra == "trf"
-Requires-Dist: torch ; extra == "trf"
-Requires-Dist: transformers (>=4.24.0,<5.0.0) ; extra == "trf"
+Requires-Dist: spacy-alignments (>=0.8.6,<0.9.0); extra == "trf"
+Requires-Dist: torch; extra == "trf"
+Requires-Dist: transformers (>=4.24.0,<5.0.0); extra == "trf"
 Project-URL: Repository, https://github.com/huspacy/huspacy
 Description-Content-Type: text/markdown
 
 
 # 
 
 <div align="center" markdown>
```

## Comparing `huspacy-0.8.1.dist-info/RECORD` & `huspacy-0.9.0.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-huspacy/__init__.py,sha256=dDGxA0L1Na2-vZen2bvxphBYqejHalbKVhgTy4yTfX0,3889
+huspacy/__init__.py,sha256=9Ox7uNShMP7Uz2vTweHuqbKfFwg3Uhkz5ic-hEmPD08,3973
 huspacy/components/__init__.py,sha256=kE9WMudC-GvwZWrNLd2LwEvdpa9KA2R7JOuqHChcC6g,102
 huspacy/components/edit_tree_lemmatizer.py,sha256=iMctOZgo4QOIe54Jwj2jQbxDwGrFJhGFpdsvud2u5us,17063
 huspacy/components/lemma_postprocessing.py,sha256=9IiTanL_rO7P53n-U9ia00ZKzB6hXxQtWTmKs8LvFtk,3237
 huspacy/components/lookup_lemmatizer.py,sha256=BKmWgpUo24U6UXNmyF3rhQlNkB51aBsEY4hxTgtG0qQ,5077
 huspacy/extra/__init__.py,sha256=RK39FEvNpkcxMeflciLuaWM1b2b2EdVaj9ARSjrWLmw,60
 huspacy/extra/roman_num_converter.py,sha256=7ldRR8-uxg6Q6ZxUoJd0Ye3ME6k1s4sFQAXGlVJCJSI,1635
 huspacy/extra/sentencizer.py,sha256=8rDNILh3gwngMoq-srtrQLeLv8kke4BkS4L0MBSaw54,2059
 huspacy/integrations/__init__.py,sha256=7cBtB8nMP3CEm4izgf9JJVEhUq2G1fYtAXL5SuClZ40,44
 huspacy/integrations/nerpp.py,sha256=Wt9cKYMY1lpZ8WwAlWOuGMA--_JDuGxEFYQn9FBlwC4,2413
 huspacy/integrations/sentiment.py,sha256=g-squqWpGYJLqst3gH9_PhdkoQfvgw5GsiO_XFF0sLE,4063
 huspacy/resources/poltext_sentiment.json,sha256=pHx0iDx6Nl9zUuQKkdOB2hH3aXddMn-4wIZOUE9oS-Y,541963
 huspacy/resources/precognox_sentiment.json,sha256=STcuZYUMDFb5rgrcH9r39SsNl36mkG6gzqfsqIPE2TQ,791334
 huspacy/utils.py,sha256=b1-pq2FHw-nJSlFrwg-vTwGnMiWMypRXmyLEzrS90CI,2103
-huspacy-0.8.1.dist-info/METADATA,sha256=OOJUJ16r0TdvFhDy_wM3aI1EUGFtEIgU8aQ7rkTcY5A,12182
-huspacy-0.8.1.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
-huspacy-0.8.1.dist-info/RECORD,,
+huspacy-0.9.0.dist-info/WHEEL,sha256=vxFmldFsRN_Hx10GDvsdv1wroKq8r5Lzvjp6GZ4OO8c,88
+huspacy-0.9.0.dist-info/METADATA,sha256=ChCW4zbzRFeIfbk_rqmrm1ZxbnpPlOyy2iyxCzMbueA,12245
+huspacy-0.9.0.dist-info/RECORD,,
```

