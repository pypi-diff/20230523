# Comparing `tmp/clinlp-0.1.0.tar.gz` & `tmp/clinlp-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clinlp-0.1.0.tar", max compression
+gzip compressed data, was "clinlp-0.1.1.tar", max compression
```

## Comparing `clinlp-0.1.0.tar` & `clinlp-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0    35149 2023-05-23 13:34:48.119725 clinlp-0.1.0/LICENSE
--rw-r--r--   0        0        0     7783 2023-05-23 13:34:48.119725 clinlp-0.1.0/README.md
--rw-r--r--   0        0        0       54 2023-05-23 13:34:48.119725 clinlp-0.1.0/clinlp/__init__.py
--rw-r--r--   0        0        0      250 2023-05-23 13:34:48.119725 clinlp-0.1.0/clinlp/component/__init__.py
--rw-r--r--   0        0        0    10789 2023-05-23 13:34:48.119725 clinlp-0.1.0/clinlp/component/qualifier.py
--rw-r--r--   0        0        0     2308 2023-05-23 13:34:48.119725 clinlp-0.1.0/clinlp/component/sentencizer.py
--rw-r--r--   0        0        0     7698 2023-05-23 13:34:48.119725 clinlp-0.1.0/clinlp/language.py
--rw-r--r--   0        0        0    24443 2023-05-23 13:34:48.119725 clinlp-0.1.0/clinlp/resources/psynlp_context_rules.json
--rw-r--r--   0        0        0      450 2023-05-23 13:34:48.119725 clinlp-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     8244 1970-01-01 00:00:00.000000 clinlp-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-06 13:37:40.385218 clinlp-0.1.1/LICENSE
+-rw-r--r--   0        0        0     8381 2023-05-23 14:07:16.856255 clinlp-0.1.1/README.md
+-rw-r--r--   0        0        0       54 2023-05-23 13:53:46.196466 clinlp-0.1.1/clinlp/__init__.py
+-rw-r--r--   0        0        0      250 2023-05-23 11:18:41.641635 clinlp-0.1.1/clinlp/component/__init__.py
+-rw-r--r--   0        0        0    10757 2023-05-23 14:07:16.856623 clinlp-0.1.1/clinlp/component/qualifier.py
+-rw-r--r--   0        0        0     2308 2023-05-23 11:18:41.641955 clinlp-0.1.1/clinlp/component/sentencizer.py
+-rw-r--r--   0        0        0     7698 2023-05-23 13:20:57.844906 clinlp-0.1.1/clinlp/language.py
+-rw-r--r--   0        0        0        0 2023-05-23 14:07:16.856699 clinlp-0.1.1/clinlp/resources/__init__.py
+-rw-r--r--   0        0        0    24443 2023-05-23 13:32:24.283263 clinlp-0.1.1/clinlp/resources/psynlp_context_rules.json
+-rw-r--r--   0        0        0      547 2023-05-23 14:09:46.872858 clinlp-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     9475 1970-01-01 00:00:00.000000 clinlp-0.1.1/setup.py
+-rw-r--r--   0        0        0     8939 1970-01-01 00:00:00.000000 clinlp-0.1.1/PKG-INFO
```

### Comparing `clinlp-0.1.0/LICENSE` & `clinlp-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clinlp-0.1.0/README.md` & `clinlp-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -32,32 +32,54 @@
 nlp.add_pipe('clinlp_sentencizer')
 
 # Entities
 ruler = nlp.add_pipe('entity_ruler')
 
 terms = {
     'covid_19_symptomen': [
-        'verkouden', 'neusverkouden', 'loopneus', 'niezen', 
-        'keelpijn', 'hoesten', 'benauwd', 'kortademig', 'verhoging', 
+        'verkoudheid', 'neusverkoudheid', 'loopneus', 'niezen', 'vermoeidheid',
+        'keelpijn', 'hoesten', 'benauwdheid', 'kortademigheid', 'verhoging', 
+        'koorts', 'verlies van reuk', 'verlies van smaak'
+    ]
+}
+
+for term_description, terms in terms.items():
+    ruler.add_patterns([{'label': term_description, 'pattern': term} for term in terms])
+import clinlp
+import spacy
+
+nlp = spacy.blank("clinlp")
+
+# Sentences
+nlp.add_pipe('clinlp_sentencizer')
+
+# Entities
+ruler = nlp.add_pipe('entity_ruler')
+
+terms = {
+    'covid_19_symptomen': [
+        'verkoudheid', 'neusverkoudheid', 'loopneus', 'niezen', 'vermoeidheid',
+        'keelpijn', 'hoesten', 'benauwdheid', 'kortademigheid', 'verhoging', 
         'koorts', 'verlies van reuk', 'verlies van smaak'
     ]
 }
 
 for term_description, terms in terms.items():
     ruler.add_patterns([{'label': term_description, 'pattern': term} for term in terms])
 
 # Qualifiers
 nlp.add_pipe('clinlp_context_matcher')
 
 text = (
-    "Patiente bij mij gezien op spreekuur, omdat zij vorige maand pneumonitis heeft "
-    "gehad. Zij had geen last meer van kortademigheid, wel was er nog sprake van "
-    "hoesten, geen afname vermoeidheid."
+    "Patiente bij mij gezien op spreekuur, omdat zij vorige maand verlies van "
+    "reuk na covid infectie aangaf. Zij had geen last meer van kortademigheid, "
+    "wel was er nog sprake van hoesten, geen afname vermoeidheid."
 )
 
+
 doc = nlp(text)
 ```
 
 Find information in the doc object:
 
 ```python
 from spacy import displacy
```

### Comparing `clinlp-0.1.0/clinlp/component/qualifier.py` & `clinlp-0.1.1/clinlp/component/qualifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,18 +175,17 @@
         if default_rules is not None:
             self._load_default_rules(default_rules)
 
         if rules:
             self.add_rules(rules)
 
     def _load_default_rules(self, default_rules: str):
-        with importlib.resources.path("clinlp.resources", default_rules) as path:
-            input_json = path
 
-        self.add_rules(parse_rules(input_json))
+        with importlib.resources.path("clinlp.resources", default_rules) as path:
+            self.add_rules(parse_rules(path))
 
     def add_rule(self, rule: ContextRule):
         """
         Add a rule.
         """
         rule_key = f"rule_{len(self.rules)}"
         self.rules[rule_key] = rule
```

### Comparing `clinlp-0.1.0/clinlp/component/sentencizer.py` & `clinlp-0.1.1/clinlp/component/sentencizer.py`

 * *Files identical despite different names*

### Comparing `clinlp-0.1.0/clinlp/language.py` & `clinlp-0.1.1/clinlp/language.py`

 * *Files identical despite different names*

### Comparing `clinlp-0.1.0/clinlp/resources/psynlp_context_rules.json` & `clinlp-0.1.1/clinlp/resources/psynlp_context_rules.json`

 * *Files identical despite different names*

### Comparing `clinlp-0.1.0/PKG-INFO` & `clinlp-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: clinlp
-Version: 0.1.0
-Summary: 
-Author: Your Name
-Author-email: you@example.com
+Version: 0.1.1
+Summary: Performant and production-ready NLP pipelines for clinical text written in Dutch
+Author: UMCU DIT Analytics
+Author-email: analytics@umcutrecht.nl
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: intervaltree (>=3.1.0,<4.0.0)
 Requires-Dist: spacy (>=3.4.4,<4.0.0)
@@ -47,32 +47,54 @@
 nlp.add_pipe('clinlp_sentencizer')
 
 # Entities
 ruler = nlp.add_pipe('entity_ruler')
 
 terms = {
     'covid_19_symptomen': [
-        'verkouden', 'neusverkouden', 'loopneus', 'niezen', 
-        'keelpijn', 'hoesten', 'benauwd', 'kortademig', 'verhoging', 
+        'verkoudheid', 'neusverkoudheid', 'loopneus', 'niezen', 'vermoeidheid',
+        'keelpijn', 'hoesten', 'benauwdheid', 'kortademigheid', 'verhoging', 
+        'koorts', 'verlies van reuk', 'verlies van smaak'
+    ]
+}
+
+for term_description, terms in terms.items():
+    ruler.add_patterns([{'label': term_description, 'pattern': term} for term in terms])
+import clinlp
+import spacy
+
+nlp = spacy.blank("clinlp")
+
+# Sentences
+nlp.add_pipe('clinlp_sentencizer')
+
+# Entities
+ruler = nlp.add_pipe('entity_ruler')
+
+terms = {
+    'covid_19_symptomen': [
+        'verkoudheid', 'neusverkoudheid', 'loopneus', 'niezen', 'vermoeidheid',
+        'keelpijn', 'hoesten', 'benauwdheid', 'kortademigheid', 'verhoging', 
         'koorts', 'verlies van reuk', 'verlies van smaak'
     ]
 }
 
 for term_description, terms in terms.items():
     ruler.add_patterns([{'label': term_description, 'pattern': term} for term in terms])
 
 # Qualifiers
 nlp.add_pipe('clinlp_context_matcher')
 
 text = (
-    "Patiente bij mij gezien op spreekuur, omdat zij vorige maand pneumonitis heeft "
-    "gehad. Zij had geen last meer van kortademigheid, wel was er nog sprake van "
-    "hoesten, geen afname vermoeidheid."
+    "Patiente bij mij gezien op spreekuur, omdat zij vorige maand verlies van "
+    "reuk na covid infectie aangaf. Zij had geen last meer van kortademigheid, "
+    "wel was er nog sprake van hoesten, geen afname vermoeidheid."
 )
 
+
 doc = nlp(text)
 ```
 
 Find information in the doc object:
 
 ```python
 from spacy import displacy
```

