# Comparing `tmp/pypreql-nlp-0.0.8.tar.gz` & `tmp/pypreql-nlp-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypreql-nlp-0.0.8.tar", last modified: Mon May 22 03:26:30 2023, max compression
+gzip compressed data, was "pypreql-nlp-0.0.9.tar", last modified: Tue May 23 01:06:48 2023, max compression
```

## Comparing `pypreql-nlp-0.0.8.tar` & `pypreql-nlp-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:26:30.087298 pypreql-nlp-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-22 03:26:30.087298 pypreql-nlp-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-22 03:26:07.000000 pypreql-nlp-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:26:30.087298 pypreql-nlp-0.0.8/preql_nlp/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-22 03:26:07.000000 pypreql-nlp-0.0.8/preql_nlp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:26:30.087298 pypreql-nlp-0.0.8/preql_nlp/cache_providers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 03:26:07.000000 pypreql-nlp-0.0.8/preql_nlp/cache_providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-22 03:26:07.000000 pypreql-nlp-0.0.8/preql_nlp/cache_providers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-22 03:26:07.000000 pypreql-nlp-0.0.8/preql_nlp/cache_providers/local_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-22 03:26:07.000000 pypreql-nlp-0.0.8/preql_nlp/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-22 03:26:07.000000 pypreql-nlp-0.0.8/preql_nlp/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-05-22 03:26:07.000000 pypreql-nlp-0.0.8/preql_nlp/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-22 03:26:07.000000 pypreql-nlp-0.0.8/preql_nlp/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-22 03:26:07.000000 pypreql-nlp-0.0.8/preql_nlp/monkeypatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:26:30.087298 pypreql-nlp-0.0.8/preql_nlp/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-22 03:26:07.000000 pypreql-nlp-0.0.8/preql_nlp/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10653 2023-05-22 03:26:07.000000 pypreql-nlp-0.0.8/preql_nlp/prompts/prompt_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-22 03:26:07.000000 pypreql-nlp-0.0.8/preql_nlp/prompts/prompt_final_concepts.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-05-22 03:26:07.000000 pypreql-nlp-0.0.8/preql_nlp/prompts/prompt_query_semantic_groupings.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-22 03:26:07.000000 pypreql-nlp-0.0.8/preql_nlp/prompts/prompt_refine_filter.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-22 03:26:07.000000 pypreql-nlp-0.0.8/preql_nlp/prompts/prompt_semantic_to_tokens.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-22 03:26:07.000000 pypreql-nlp-0.0.8/preql_nlp/tokenization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:26:30.087298 pypreql-nlp-0.0.8/pypreql_nlp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-22 03:26:30.000000 pypreql-nlp-0.0.8/pypreql_nlp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-22 03:26:30.000000 pypreql-nlp-0.0.8/pypreql_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 03:26:30.000000 pypreql-nlp-0.0.8/pypreql_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-22 03:26:30.000000 pypreql-nlp-0.0.8/pypreql_nlp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-22 03:26:30.000000 pypreql-nlp-0.0.8/pypreql_nlp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-22 03:26:07.000000 pypreql-nlp-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 03:26:30.087298 pypreql-nlp-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-22 03:26:07.000000 pypreql-nlp-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:06:48.181039 pypreql-nlp-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-23 01:06:48.181039 pypreql-nlp-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-23 01:06:34.000000 pypreql-nlp-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:06:48.181039 pypreql-nlp-0.0.9/preql_nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-23 01:06:34.000000 pypreql-nlp-0.0.9/preql_nlp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:06:48.181039 pypreql-nlp-0.0.9/preql_nlp/cache_providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:06:34.000000 pypreql-nlp-0.0.9/preql_nlp/cache_providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-23 01:06:34.000000 pypreql-nlp-0.0.9/preql_nlp/cache_providers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-23 01:06:34.000000 pypreql-nlp-0.0.9/preql_nlp/cache_providers/local_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-23 01:06:34.000000 pypreql-nlp-0.0.9/preql_nlp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-23 01:06:34.000000 pypreql-nlp-0.0.9/preql_nlp/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9803 2023-05-23 01:06:34.000000 pypreql-nlp-0.0.9/preql_nlp/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-23 01:06:34.000000 pypreql-nlp-0.0.9/preql_nlp/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-23 01:06:34.000000 pypreql-nlp-0.0.9/preql_nlp/monkeypatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:06:48.181039 pypreql-nlp-0.0.9/preql_nlp/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-23 01:06:34.000000 pypreql-nlp-0.0.9/preql_nlp/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11868 2023-05-23 01:06:34.000000 pypreql-nlp-0.0.9/preql_nlp/prompts/prompt_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-05-23 01:06:34.000000 pypreql-nlp-0.0.9/preql_nlp/prompts/prompt_final_concepts.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-05-23 01:06:34.000000 pypreql-nlp-0.0.9/preql_nlp/prompts/prompt_final_concepts_v2.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-05-23 01:06:34.000000 pypreql-nlp-0.0.9/preql_nlp/prompts/prompt_query_semantic_groupings.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-23 01:06:34.000000 pypreql-nlp-0.0.9/preql_nlp/prompts/prompt_refine_filter.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-23 01:06:34.000000 pypreql-nlp-0.0.9/preql_nlp/prompts/prompt_semantic_to_tokens.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-23 01:06:34.000000 pypreql-nlp-0.0.9/preql_nlp/tokenization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:06:48.181039 pypreql-nlp-0.0.9/pypreql_nlp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-23 01:06:48.000000 pypreql-nlp-0.0.9/pypreql_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-23 01:06:48.000000 pypreql-nlp-0.0.9/pypreql_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 01:06:48.000000 pypreql-nlp-0.0.9/pypreql_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-23 01:06:48.000000 pypreql-nlp-0.0.9/pypreql_nlp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-23 01:06:48.000000 pypreql-nlp-0.0.9/pypreql_nlp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-23 01:06:34.000000 pypreql-nlp-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 01:06:48.181039 pypreql-nlp-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-23 01:06:34.000000 pypreql-nlp-0.0.9/setup.py
```

### Comparing `pypreql-nlp-0.0.8/PKG-INFO` & `pypreql-nlp-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypreql-nlp
-Version: 0.0.8
+Version: 0.0.9
 Summary: NLP interface for pypreql.
 Home-page: 
 Author: 
 Author-email: pypreql-community@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pypreql-nlp-0.0.8/README.md` & `pypreql-nlp-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pypreql-nlp-0.0.8/preql_nlp/cache_providers/local_sqlite.py` & `pypreql-nlp-0.0.9/preql_nlp/cache_providers/local_sqlite.py`

 * *Files identical despite different names*

### Comparing `pypreql-nlp-0.0.8/preql_nlp/helpers.py` & `pypreql-nlp-0.0.9/preql_nlp/helpers.py`

 * *Files identical despite different names*

### Comparing `pypreql-nlp-0.0.8/preql_nlp/main.py` & `pypreql-nlp-0.0.9/preql_nlp/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,23 +15,23 @@
     WhereClause,
     unique,
 )
 from preql.core.query_processor import process_query_v2
 
 from preql_nlp.constants import DEFAULT_LIMIT, logger
 from preql_nlp.models import (
-    ConceptSelectionResponse,
     FilterResult,
     FinalFilterResult,
     FinalOrderResult,
     InitialParseResponse,
     IntermediateParseResults,
     OrderResult,
     # TokenInputs,
     SemanticTokenResponse,
+    FinalParseResponse
 )
 from preql_nlp.prompts import (
     FilterRefinementCase,
     SelectionPromptCase,
     SemanticExtractionPromptCase,
     SemanticToTokensPromptCase,
     run_prompt,
@@ -46,43 +46,45 @@
         return x.concept
     elif isinstance(x, OrderResult):
         return x.concept
     raise ValueError
 
 
 def tokenize_phrases(
-    phrase_list: List[str], tokens: List[str], session_uuid, log_info: bool
+    purpose:str, phrase_list: List[str], tokens: List[str], session_uuid, log_info: bool
 ) -> SemanticTokenResponse:
     phrase_tokens: SemanticTokenResponse = run_prompt(  # type: ignore
-        SemanticToTokensPromptCase(phrases=phrase_list, tokens=tokens),
+        SemanticToTokensPromptCase(phrases=phrase_list, tokens=tokens, purpose=purpose),
         debug=True,
         session_uuid=session_uuid,
         log_info=log_info,
     )
     phrase_tokens.__root__ = [
         x for x in phrase_tokens.__root__ if x.phrase in phrase_list
     ]
     return phrase_tokens
 
 
 def concept_names_from_token_response(
-    phrase_tokens: SemanticTokenResponse, concepts: dict[str, Concept]
+    phrase_tokens: SemanticTokenResponse, concepts: dict[str, Concept],
+    token_universe:list | None
 ) -> list[str]:
-    token_universe = []
+    token_universe_internal = token_universe or []
     output: list[str] = []
 
     for mapping in phrase_tokens:
-        token_universe += mapping.tokens
+        token_universe_internal += mapping.tokens
+    token_universe_internal = list(set(token_universe_internal))
     for mapping in phrase_tokens:
         found = False
         concepts_str_matches = tokens_to_concept(
             mapping.tokens,
             [c for c in concepts.keys()],
-            limits=5,
-            universe=token_universe,
+            limits=10,
+            universe=token_universe_internal,
         )
         if concepts_str_matches:
             logger.info(f"For phrase {mapping.phrase} got {concepts_str_matches}")
             output += concepts_str_matches
             found = True
             break
         if not found:
@@ -113,16 +115,15 @@
 ) -> IntermediateParseResults:
     # the core logic flow
 
     # DETERMINSTIC: setup logging
     # LLM: semantic extraction
     # LLM: tokenization of all strings (reduce search space over all concepts)
     # DETERMINISTIC: concept candidates from tokens (map reduced search space to candidates)
-    # LLM: final selection of concepts (final get the concept result we want)
-    # DETERMINISTIC: map phrases to final concepts
+    # LLM: final selection of concepts and mapping to output roles
     # LLM: enrich filter values
     # DETERMINISTIC: return results
 
     # DETERMINISTIC: setup logging
     session_uuid = uuid.uuid4()
     env_concepts = input_environment.concepts
 
@@ -133,79 +134,84 @@
         log_info=log_info,
         session_uuid=session_uuid,
     )
 
     # LLM: tokenization of all strings (reduce search space over all concepts)
     concept_candidates = []
     global_phrase_token_map = {}
+    token_response_mapping:dict[str, SemanticTokenResponse] = {}
     for semantic_category, valid_purposes in {
         "metrics": [Purpose.METRIC],
         "dimensions": [Purpose.KEY, Purpose.PROPERTY, Purpose.CONSTANT],
         "filtering": list(Purpose),
         "order": list(Purpose),
     }.items():
         category_tokens = build_token_list_by_purpose(env_concepts, valid_purposes)
         local_phrases = [
             get_phrase_from_x(x) for x in getattr(parsed, semantic_category)
         ]
         # skip if we have no relevant phrases
         if not local_phrases:
             continue
         token_mapping = tokenize_phrases(
-            local_phrases, category_tokens, log_info=log_info, session_uuid=session_uuid
+            semantic_category, local_phrases, category_tokens, log_info=log_info, session_uuid=session_uuid
         )
+        token_response_mapping[semantic_category] = token_mapping
 
-        for item in token_mapping:
+    # DETERMINISTIC
+    token_universe = set()
+    for key, token_mapping_pass_one in token_response_mapping.items():
+        for mapping in token_mapping_pass_one:
+            for t in mapping.tokens:
+                token_universe.add(t)
+    token_universe_list = list(token_universe)
+
+    # for key, debug in token_response_mapping.items():
+    #     print(key)
+    #     print(debug)
+    # raise ValueError('eel')
+
+    for key, token_mapping_pass_two in token_response_mapping.items():
+        for item in token_mapping_pass_two:
             if not all([x in category_tokens] for x in item.tokens):
                 invalid = [x for x in item.tokens if x not in category_tokens]
                 raise ValueError(
                     f"Phrase {item.phrase} return invalid tokens {invalid}"
                 )
             global_phrase_token_map[item.phrase] = item.tokens
         concept_candidates += concept_names_from_token_response(
-            token_mapping, env_concepts
+            token_mapping_pass_two, env_concepts, token_universe=token_universe_list
         )
 
+
     # DETERMINISTIC: concept candidates from tokens (map reduced search space to candidates)
-    selections: ConceptSelectionResponse = run_prompt(  # type: ignore
+    selections: FinalParseResponse = run_prompt(  # type: ignore
         SelectionPromptCase(concept_names=concept_candidates, question=input_text),
         debug=debug,
         session_uuid=session_uuid,
         log_info=log_info,
     )
-    selected_concepts = list(set(selections.matches))
-
-    for selection in selected_concepts:
-        if selection not in env_concepts:
-            raise ValueError(
-                f"Returned concept {selection} that does not actually exist in environment!"
-            )
+    selected_concepts = list(set(selections.selection))
 
-    # DETERMINISTIC: map phrases to final concepts
-    phrase_to_concept_map: dict[str, Concept] = {}
-    for key, tokens in global_phrase_token_map.items():
-        mapped = tokens_to_concept(concepts=selected_concepts, tokens=tokens, limits=1)
-        if mapped:
-            phrase_to_concept_map[key] = env_concepts[mapped[0]]
 
     final_ordering = [
         FinalOrderResult(
-            concept=phrase_to_concept_map[order.concept], order=order.order
+            concept=env_concepts[order.concept], order=order.order
         )
-        for order in parsed.order
-        if phrase_to_concept_map[order.concept]
+        for order in selections.order
+
     ]
 
     final_filters_pre = [
         FinalFilterResult(
-            concept=phrase_to_concept_map[filter.concept],
+            concept=env_concepts[filter.concept],
             operator=filter.operator,
             values=filter.values,
         )
-        for filter in parsed.filtering
+        for filter in selections.filtering
     ]
 
     # LLM: enrich filter values
     for item in final_filters_pre:
         enrich_filter(item, log_info=log_info, session_uuid=session_uuid)
     # DETERMINISTIC: return results
     return IntermediateParseResults(
```

### Comparing `pypreql-nlp-0.0.8/preql_nlp/models.py` & `pypreql-nlp-0.0.9/preql_nlp/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,14 +37,22 @@
     @property
     def selection(self)->list[str]:
         filtering = [f.concept for f in self.filtering]
         order = [x.concept for x in self.order]
         return list(set(self.metrics + self.dimensions + filtering + order))
 
 
+class FinalParseResponse(BaseModel):
+    """The result of the initial parse"""
+    selection:list[str]
+    limit:int
+    order:list[OrderResult]
+    filtering:list[FilterResult]
+
+
 class IntermediateParseResults(BaseModel):
     select: list[Concept]
     limit: int
     order: list[FinalOrderResult]
     filtering:list[FinalFilterResult]
```

### Comparing `pypreql-nlp-0.0.8/preql_nlp/monkeypatch.py` & `pypreql-nlp-0.0.9/preql_nlp/monkeypatch.py`

 * *Files identical despite different names*

### Comparing `pypreql-nlp-0.0.8/preql_nlp/prompts/prompt_executor.py` & `pypreql-nlp-0.0.9/preql_nlp/prompts/prompt_executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 # to return a score between 0 and 1
 from preql_nlp.constants import logger
 from preql_nlp.models import (
     InitialParseResponse,
     ConceptSelectionResponse,
     SemanticTokenResponse,
     FilterRefinementResponse,
+    FinalParseResponse
+
 )
 from preql_nlp.cache_providers.base import BaseCache
 from preql_nlp.cache_providers.local_sqlite import SqlliteCache
 from preql_nlp.helpers import retry_with_exponential_backoff
 from pydantic import BaseModel, ValidationError
 from typing import List, Optional, Callable, Union, Type, overload
 import uuid
@@ -68,14 +70,15 @@
             prompt_executor_kwargs={"stopword": PROMPT_STOPWORD},
         )
         self._prompt_hash = str(uuid.uuid4())
         self.parsed = None
         self.fail_on_parse_error = fail_on_parse_error
         self.retry_prompt = "User: That response was incorrectly formatted. Please return the same content as the first response with formatting fixed (eg. valid JSON) to conform with original request. System:\n"
         self.stash: BaseCache = SqlliteCache()
+        self.has_rerun = False
 
     @classmethod
     def parse_response(cls, response: str):
         return cls.parse_model.parse_raw(response.split(cls.stopword)[0])
 
     # def get_prompt_executor(self):
     #     from langchain.chat_models import ChatOpenAI
@@ -88,54 +91,57 @@
 
     @retry_with_exponential_backoff
     def execute_prompt(self, prompt_str, skip_cache: bool = False):
         # if we already have a local result
         # skip hitting remote
         # TODO: make the cache provider pluggable and injected
         hash_val = gen_hash(self, self.attributes_used_for_hash)
-        resp = self.stash.retrieve(hash_val)
-        if resp and not skip_cache:
-            self.response = resp
-            return self.response
+        if not skip_cache:
+            resp = self.stash.retrieve(hash_val)
+            if resp:
+                self.response = resp
+                return self.response
         self.response = self.prompt_executor(prompt_str)
         self.stash.store(hash_val, self.category, self.response)
         return self.response
 
     def get_extra_template_context(self):
         return {"stopword": self.stopword}
 
     def rerun(self):
         self.prompt = self.prompt + self.response + "\n" + self.retry_prompt
+        self.has_rerun = True
         self.execute_prompt(self.prompt, skip_cache=True)
 
+
     def post_run(self):
         try:
             self.parsed = self.parse_response(self.response)
         except ValidationError as e:
-            self.rerun()
-            try:
-                self.parsed = self.parse_response(self.response)
-            except ValidationError:
-                print(self.render())
-                print("was unable to parse response using ", str(self.parse_model))
-                print(self.response)
-                if self.fail_on_parse_error:
-                    raise e
+            if not self.has_rerun:
+                self.rerun()
+                return self.post_run()
+            print(self.render())
+            print("was unable to parse response using ", str(self.parse_model))
+            print(self.response)
+            if self.fail_on_parse_error:
+                raise e
 
+    
     def render(
         self,
     ):
         return self.template.render(**self.jinja_context)
 
 
 class SemanticExtractionPromptCase(BasePreqlPromptCase):
     template = templates.get_template("prompt_query_semantic_groupings.jinja2")
     parse_model = InitialParseResponse
 
-    attributes_used_for_hash = {"category", "question", "template"}
+    attributes_used_for_hash = {"category", "question", "template",}
 
     def __init__(
         self,
         question: str,
         evaluators: Optional[Union[Callable, List[Callable]]] = None,
     ):
         self.question = question
@@ -145,67 +151,92 @@
         return {**super().get_extra_template_context(), "question": self.question}
 
 
 class SemanticToTokensPromptCase(BasePreqlPromptCase):
     template = templates.get_template("prompt_semantic_to_tokens.jinja2")
     parse_model = SemanticTokenResponse
 
-    attributes_used_for_hash = {"tokens", "phrases", "category", "template"}
+    attributes_used_for_hash = {"tokens", "phrases", "category", "template", "purpose",}
 
     def __init__(
         self,
+        purpose:str,
         tokens: List[str],
         phrases: List[str],
         evaluators: Optional[Union[Callable, List[Callable]]] = None,
-    ):
+    ):  
+        tokens = [token for token in tokens if token]
         self.tokens = sorted(tokens)
+        self.purpose = purpose
         # we need to ensure that we always have a list
         # for chat-gpt to understand the prompt properly
         # pad out the inputs with a random phrase
         self.phrases = sorted(phrases + ["democratic elections"])
         super().__init__(category="semantic_to_tokens", evaluators=evaluators)
 
     def get_extra_template_context(self):
         return {
             **super().get_extra_template_context(),
+            "purpose": self.purpose,
             "tokens": ", ".join([f'"{c}"' for c in self.tokens if c]),
             "phrase_str": ", ".join([f'"{c}"' for c in self.phrases]),
         }
 
 
 class SelectionPromptCase(BasePreqlPromptCase):
-    template = templates.get_template("prompt_final_concepts.jinja2")
-    parse_model = ConceptSelectionResponse
+    template = templates.get_template("prompt_final_concepts_v2.jinja2")
+    parse_model = FinalParseResponse
 
-    attributes_used_for_hash = {"question", "concept_names", "category", "template"}
+    attributes_used_for_hash = {"question", "concept_names", "category", "template",}
 
     def __init__(
         self,
         question: str,
         concept_names: List[str],
         evaluators: Optional[Union[Callable, List[Callable]]] = None,
     ):
         self.question = question
         self.concept_names = sorted(list(set(concept_names)), key=lambda x: x)
         super().__init__(evaluators=evaluators, category="selection")
         self.execution.score = None
+        self.retries = 0
 
     def get_extra_template_context(self):
         return {
             **super().get_extra_template_context(),
             "concept_string": ", ".join([f'"{c}"' for c in self.concept_names]),
-            "question": self.question,
+            "question": self.question
         }
+    
+    def post_run(self):
+        super().post_run()
+
+        selected_concepts:List[str] = self.parsed.selection
+        for item in self.parsed.filtering:
+            selected_concepts.append(item.concept)
+        for item in self.parsed.order:
+            selected_concepts.append(item.concept)
+
+        for selection in selected_concepts:
+            if selection not in self.concept_names:
+                self.retries +=1
+                retry_prompt = f'User: Return value {selection} was not provided by me, please return a new answer with only concepts I provided.\nSystem: '
+                self.prompt = self.prompt + self.response + "\n" + retry_prompt
+                if self.retries<4:
+                    self.execute_prompt(self.prompt, skip_cache=True)
+                    self.post_run()
+                else:
+                    raise ValueError(f"LLM returned concept {selection} that do not exist ininput names, cannot progress - returned {self.parsed}")
 
 
 class FilterRefinementCase(BasePreqlPromptCase):
     template = templates.get_template("prompt_refine_filter.jinja2")
     parse_model = FilterRefinementResponse
 
-    attributes_used_for_hash = {"values", "description", "template"}
+    attributes_used_for_hash = {"values", "description", "template",}
 
     def __init__(
         self,
         values: list[str],
         description: str,
         evaluators: Optional[Union[Callable, List[Callable]]] = None,
     ):
```

### Comparing `pypreql-nlp-0.0.8/preql_nlp/prompts/prompt_final_concepts.jinja2` & `pypreql-nlp-0.0.9/preql_nlp/prompts/prompt_final_concepts.jinja2`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 System: You are a helpful AI that selects the most relevant matching concepts to answer a question from a provided list.
 
 Guidelines:
-* you can assume the user will always provide a list of phrases
-* you can assume the user will always provide a question
+* the user will always provide a list of phrases
+* the user will always provide a question
+* the user may provide some filters they wish to use
 * only return concepts provided by the user
 * concepts are dot seperated and in quotes, e.g. "sales" or "product.revenue"
 * return the concepts that together best match the user question
 * reason about each match step by step, e.g. "first match the concept 'product' to the word 'product' in the question, then match the concept 'revenue' to the word 'revenue' in the question, and together these enable aggregating revenue by year"
 The output should be a VALID JSON blob with the following keys and values:
 * matches: a list of concepts from the user provided list that together best match the 
 * reasoning: a string explaining your step by step reasoning for the matches
+* final_filters: the filters remapped to the restricted concepts
 
-User: concepts: ["product.color", "order.state", "order.year", "order.revenue.sum", "order.revenue.avg", "product.name", "order.month", "order.day", "product.manufacturer"] question: "what color products were the top sellers by revenue in 2024?"]
+User: concepts: ["product.color", "order.state", "order.year", "order.revenue.sum", "order.revenue.avg", "product.name", "order.month", "order.day", "product.manufacturer"] question: "what color products were the top sellers by revenue in 2024?"
 System:
 {% raw %}{"matches": ["product.color", "order.revenue.sum", "order.year" ],
-"reasoning": "product.color matches the user request for product colors, and order revenue sum would enable aggregating revenue to the color to determine the top. Order year is required to filter to 2024." }
-User: concepts: ["product.color", "order.state", "order.year", "order.revenue.sum", "order.revenue.avg", "product.name", "order.month", "order.day", "product.manufacturer"] question: "What are the sales by state?"
-System:
+final_filters:[{"order.year": "2024"}],
+"reasoning": "product.color matches the user request for product colors, and order revenue sum would enable aggregating revenue to the color to determine the top. Order year is required to filter to 2024." }{% endraw %}
+User: concepts: ["product.color", "order.state", "order.year", "order.revenue.sum", "order.revenue.avg", "product.name", "order.month", "order.day", "product.manufacturer"] question: "What are the sales by state? No filtering."
+System:{% raw %}
 {"matches": ["order.state", "order.revenue.sum"],
-"reasoning": "order.state is the best match for state when looking at revenue, and order.revenue.sum would enable aggregating revenue." }
-User: concepts: ["product.color", "order.state", "order.year", "order.revenue.sum", "order.revenue.avg", "product.name", "order.month", "order.day", "product.manufacturer"]  question: "What are the average sales by state?"
-System:
+"final_filters": [],
+"reasoning": "order.state is the best match for state when looking at revenue, and order.revenue.sum would enable aggregating revenue." }{% endraw %}
+User: concepts: ["product.color", "order.state", "order.year", "order.revenue.sum", "order.revenue.avg", "product.name", "order.month", "order.day", "product.manufacturer"]  question: "What are the average sales by state? No filtering."
+System:{% raw %}
 {"matches": ["order.state", "order.revenue.avg"],
+"final_filters": [],
 "reasoning": "order.state is the best match for state, and order.revenue.avg references the average of revenue for an order, which is conceptually closest to sales." }{% endraw %}
-User: concepts: [{{ concept_string }}] question: "{{ question }}"
+User: concepts: [{{ concept_string }}] question: "{{ question }}" {%if filtering%}Filter by {{filtering}}{% else %}No filtering{% endif%}
 System:
```

### Comparing `pypreql-nlp-0.0.8/preql_nlp/prompts/prompt_query_semantic_groupings.jinja2` & `pypreql-nlp-0.0.9/preql_nlp/prompts/prompt_query_semantic_groupings.jinja2`

 * *Files identical despite different names*

### Comparing `pypreql-nlp-0.0.8/preql_nlp/prompts/prompt_refine_filter.jinja2` & `pypreql-nlp-0.0.9/preql_nlp/prompts/prompt_refine_filter.jinja2`

 * *Files identical despite different names*

### Comparing `pypreql-nlp-0.0.8/preql_nlp/prompts/prompt_semantic_to_tokens.jinja2` & `pypreql-nlp-0.0.9/preql_nlp/prompts/prompt_semantic_to_tokens.jinja2`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 System: you are a helpful AI that maps a list of phrases to the most related words from a provided set. Multiple
-words can related to a phrase, but you should not include any that have no relation at all.
+words can related to a phrase, but if there are several similar terms include only the most specific one. If Multiple
+terms are related to the phrase but not similar, include both. If a phrase has no matches, return an empty array.
 
 Guidelines:
-* you can assume the user will always provide a list of phrases
-* you can assume the user will always provide a list of words
+* the user will always provide a list of phrases
+* the user will always provide a list of words
+* the user will provide a purpose for the phrase
 * only return words that appear in the list provided by the user
 * If a phrase has no matches, return an empty array
 The output should be a VALID JSON list. Each JSON list entry should have following keys.
 * phrase, the input phrase
 * tokens, the user provided words that are most related to the phrase
-The full ohutput should be followed by {{stopword}}.
+The full output should be followed by {{stopword}}.
 
 
-User: given the words ["color", "product", "year", "revenue"], find the most relevant words for each phrase in ["product revenue is up", "products with green color", "product revenue by year", "yearly revenue"]
+User: given the words ["color", "product", "year", "revenue", "count"], find the most relevant words for the purpose of creating metrics for each phrase in ["product revenue is up", "products with green color", "product revenue by year", "yearly revenue"]
 System:
 {% raw %}
 [
    {
       "phrase":"product revenue",
       "tokens":[
          "product",
          "revenue"
       ]
    },
    {
       "phrase":"product color",
       "tokens":[
          "product",
-         "color"
+         "color",
+         "count"
       ]
     },
     {
       "phrase":"product revenue by year",
       "tokens":[
          "product",
          "revenue",
@@ -42,27 +45,43 @@
       "phrase":"yearly revenue",
       "tokens":[
          "revenue",
          "year"
       ]
    }   
 ]{% endraw %}{{ stopword }}
-User: given the words ["state", "motto", "taxes", "expenses"], find the most relevant words for each phrase in ["vermont budget shortfall "]
+User: given the words ["state", "motto", "taxes", "expenses"], find the most relevant words for the purpose of filtering for each phrase in ["vermont budget shortfall "]
 System:{% raw %}
 [
    {
       "phrase":"vermont budget shortfall",
       "tokens":[
-         "state",
-         "taxes",
-         "expenses"
+         "state"
+      ]
+   }
+]{% endraw %}{{ stopword }}
+User: given the words ["product", "color", "revenue", "skus"], find the most relevant words for the purpose of grouping data for each phrase in ["products by color", "SKUs by color"]
+System:{% raw %}
+[
+   {
+      "phrase":"products by color",
+      "tokens":[
+         "products",
+         "color"
+      ]
+   },
+      {
+      "phrase":"skus by color",
+      "tokens":[
+         "skus",
+         "color"
       ]
    }
 ]{% endraw %}{{ stopword }}
-User: given the words ["product", "count", "order", "year"], find the most relevant words for each phrase in ["top selling products", "order flow"]
+User: given the words ["product", "count", "order", "year"], find the most relevant words for the purpose of metrics for each phrase in ["top selling products", "order flow"]
 System:{% raw %}
 [
    {
       "phrase":"products sold",
       "tokens":[
          "product",
          "count",
@@ -73,9 +92,9 @@
       "phrase":"orders",
       "tokens":[
          "order",
          "count"
       ]
    }
 ]{% endraw %}{{ stopword }}
-User: Given the words [{{ tokens }}], find the most relevant words for each phrase in [{{ phrase_str }}]
+User: Given the words [{{ tokens }}], find the most relevant words for the purpose of {{purpose}} for each phrase in [{{ phrase_str }}]
 System:
```

### Comparing `pypreql-nlp-0.0.8/preql_nlp/tokenization.py` & `pypreql-nlp-0.0.9/preql_nlp/tokenization.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,30 +41,34 @@
     mappings = {x: split_to_tokens(x) for x in concepts}
     candidates =[x for x in concepts if any(token in mappings[x] for token in tokens)]
     pickings = defaultdict(list)
 
     if not candidates:
         return None
     tiers = set()
-    
+
     for candidate in candidates:
         score  = 0
         candidate_tokens = mappings[candidate]
         # exact match to concept is +2
-        for x in candidate_tokens:
-            if x in tokens:
-                score +=2
+        for x in tokens:
+            if x in candidate_tokens:
+                # print(f'+2 score from token {x} in candidate list')
+                score +=10
         # universe context is + 1
         for y in universe_list:
-            if y in tokens:
+            if y in candidate_tokens:
+                # print(f"+1 score from token {y} in universe")
                 score +=1
         pickings[score].append(candidate)
         tiers.add(score)
     tier_list = sorted(list(tiers), key=lambda x: -x)
     found: List[str] = []
     while len(found) < limits and tier_list:
 
         stier = tier_list.pop(0)
-        candidates = sorted(pickings[stier], key=lambda x: len(x))
+        # sort within list by length ascending, then alphabetical
+        # for consistency
+        candidates = sorted(pickings[stier], key=lambda x: (len(x), x))
         required = limits - len(found)
         found += candidates[:required]
     return found
```

### Comparing `pypreql-nlp-0.0.8/pypreql_nlp.egg-info/PKG-INFO` & `pypreql-nlp-0.0.9/pypreql_nlp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypreql-nlp
-Version: 0.0.8
+Version: 0.0.9
 Summary: NLP interface for pypreql.
 Home-page: 
 Author: 
 Author-email: pypreql-community@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pypreql-nlp-0.0.8/pypreql_nlp.egg-info/SOURCES.txt` & `pypreql-nlp-0.0.9/pypreql_nlp.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 preql_nlp/tokenization.py
 preql_nlp/cache_providers/__init__.py
 preql_nlp/cache_providers/base.py
 preql_nlp/cache_providers/local_sqlite.py
 preql_nlp/prompts/__init__.py
 preql_nlp/prompts/prompt_executor.py
 preql_nlp/prompts/prompt_final_concepts.jinja2
+preql_nlp/prompts/prompt_final_concepts_v2.jinja2
 preql_nlp/prompts/prompt_query_semantic_groupings.jinja2
 preql_nlp/prompts/prompt_refine_filter.jinja2
 preql_nlp/prompts/prompt_semantic_to_tokens.jinja2
 pypreql_nlp.egg-info/PKG-INFO
 pypreql_nlp.egg-info/SOURCES.txt
 pypreql_nlp.egg-info/dependency_links.txt
 pypreql_nlp.egg-info/requires.txt
```

### Comparing `pypreql-nlp-0.0.8/setup.py` & `pypreql-nlp-0.0.9/setup.py`

 * *Files identical despite different names*

