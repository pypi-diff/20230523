# Comparing `tmp/factscore-0.1.2.tar.gz` & `tmp/factscore-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "factscore-0.1.2.tar", max compression
+gzip compressed data, was "factscore-0.1.3.tar", max compression
```

## Comparing `factscore-0.1.2.tar` & `factscore-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     2907 2023-05-23 16:05:08.735586 factscore-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-05-23 14:51:37.783672 factscore-0.1.2/factscore/__init__.py
--rw-r--r--   0        0        0    16718 2023-05-23 14:51:37.783672 factscore-0.1.2/factscore/atomic_facts.py
--rw-r--r--   0        0        0     2967 2023-05-23 14:51:37.783672 factscore-0.1.2/factscore/clm.py
--rw-r--r--   0        0        0     1993 2023-05-23 16:02:14.263382 factscore-0.1.2/factscore/download_data.py
--rw-r--r--   0        0        0    10158 2023-05-23 16:02:34.590940 factscore-0.1.2/factscore/factscorer.py
--rw-r--r--   0        0        0     1762 2023-05-23 14:51:37.783672 factscore-0.1.2/factscore/lm.py
--rw-r--r--   0        0        0     7133 2023-05-23 14:51:37.783672 factscore-0.1.2/factscore/npm.py
--rw-r--r--   0        0        0     3953 2023-05-23 14:51:37.783672 factscore-0.1.2/factscore/openai_lm.py
--rw-r--r--   0        0        0     7536 2023-05-23 14:51:37.783672 factscore-0.1.2/factscore/retrieval.py
--rw-r--r--   0        0        0     4774 2023-05-23 14:51:37.783672 factscore-0.1.2/factscore/utils.py
--rw-r--r--   0        0        0      798 2023-05-23 16:04:23.608568 factscore-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3991 1970-01-01 00:00:00.000000 factscore-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     4099 2023-05-23 19:36:36.423724 factscore-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-23 14:51:37.783672 factscore-0.1.3/factscore/__init__.py
+-rw-r--r--   0        0        0    15249 2023-05-23 19:22:54.093599 factscore-0.1.3/factscore/atomic_facts.py
+-rw-r--r--   0        0        0     2967 2023-05-23 14:51:37.783672 factscore-0.1.3/factscore/clm.py
+-rw-r--r--   0        0        0     2360 2023-05-23 19:26:26.996972 factscore-0.1.3/factscore/download_data.py
+-rw-r--r--   0        0        0    10241 2023-05-23 19:39:46.119599 factscore-0.1.3/factscore/factscorer.py
+-rw-r--r--   0        0        0     1706 2023-05-23 19:09:54.010548 factscore-0.1.3/factscore/lm.py
+-rw-r--r--   0        0        0     7105 2023-05-23 19:37:35.506439 factscore-0.1.3/factscore/npm.py
+-rw-r--r--   0        0        0     3956 2023-05-23 19:20:40.884494 factscore-0.1.3/factscore/openai_lm.py
+-rw-r--r--   0        0        0     7747 2023-05-23 19:31:41.778130 factscore-0.1.3/factscore/retrieval.py
+-rw-r--r--   0        0        0     4774 2023-05-23 14:51:37.783672 factscore-0.1.3/factscore/utils.py
+-rw-r--r--   0        0        0      813 2023-05-23 19:44:18.229683 factscore-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5220 1970-01-01 00:00:00.000000 factscore-0.1.3/PKG-INFO
```

### Comparing `factscore-0.1.2/factscore/atomic_facts.py` & `factscore-0.1.3/factscore/atomic_facts.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,39 @@
 import json
 import numpy as np
 import re
 import functools
 import string
 import spacy
 import sys
-from tqdm import tqdm
+import nltk
 import openai
 from rank_bm25 import BM25Okapi
 import os
 import time
 from nltk.tokenize import sent_tokenize
 
+from factscore.openai_lm import OpenAIModel
+
+nltk.download("punkt")
+
 
 class AtomicFactGenerator(object):
-    def __init__(self, key_path, demon_dir, model_name=None, gpt3_cache_dir=None):
+    def __init__(self, key_path, demon_dir, model_name=None, gpt3_cache_file=None):
 
         self.model = model_name
         if model_name:
             self.preprocess_fn = functools.partial(preprocess_fn, model=model_name)
         else:
             self.preprocess_fn = None
         self.nlp = spacy.load("en_core_web_sm")
-        self.key_path = key_path
         self.is_bio = True
         self.demon_path = os.path.join(demon_dir, "demons.json" if self.is_bio else "demons_complex.json")
-        if gpt3_cache_dir is not None:
-            self.gpt3_cache_path = os.path.join(gpt3_cache_dir, "{}_{}_additional.json".format("bio" if self.is_bio else "complex", model_name))
-        else:
-            self.gpt3_cache_path = None
 
-        # load api key
-        with open(key_path, 'r') as f:
-            api_key = f.readline()
-        openai.api_key = api_key.strip()
+        self.openai_lm = OpenAIModel("InstructGPT", cache_file=gpt3_cache_file, key_path=key_path)
 
         # get the demos
         with open(self.demon_path, 'r') as f:
             self.demons = json.load(f)
 
         tokenized_corpus = [doc.split(" ") for doc in self.demons.keys()]
         self.bm25 = BM25Okapi(tokenized_corpus)
@@ -101,15 +97,14 @@
 
     def get_init_atomic_facts_from_sentence(self, sentences):
         is_bio = self.is_bio
         demons = self.demons
 
         k = 1 if is_bio else 0
         n = 7 if is_bio else 8
-        batch_size = 8
 
         prompts = []
         prompt_to_sent = {}
         atoms = {}
         for sentence in sentences:
             if sentence in atoms:
                 continue
@@ -127,19 +122,18 @@
                 for fact in demons[match]:
                     prompt = prompt + "- {}\n".format(fact)
                 prompt = prompt + "\n"
             prompt = prompt + "Please breakdown the following sentence into independent facts: {}\n".format(sentence)
             prompts.append(prompt)
             prompt_to_sent[prompt] = sentence
 
-        for i in range(0, len(prompts), batch_size):
-            response = call_gpt3(prompts[i: i+batch_size])
-            for j in range(len(response["choices"])):
-                atoms[prompt_to_sent[prompts[i+j]]] = text_to_sentences(response["choices"][j]["text"])
-            
+        for prompt in prompts:
+            output, _ = self.openai_lm.generate(prompt)
+            atoms[prompt_to_sent[prompt]] = text_to_sentences(output)
+
         for key, value in demons.items():
             if key not in atoms:
                 atoms[key] = value
 
         return atoms
 
 
@@ -155,51 +149,26 @@
         if is_invalid_ppl(output):
             return None
         paragraphs = []
         for para in output.split("\n\n"):
             if is_invalid_paragraph_ppl(para):
                 break
             paragraphs.append(para.strip())
-        
+
         if len(paragraphs) == 0:
             return None
 
     elif model in ["mpt-7b", "stablelm-alpha-7b"]:
         if not "sorry" in generation and not "provide" in generation.split(" "):
             paragraphs = [para.strip() for para in generation.split("\n") if len(para.strip()) > 0]
 
     else:
         paragraphs = [para.strip() for para in generation.split("\n") if len(para.strip()) > 0]
-    
-    return paragraphs
-
 
-def call_gpt3(prompt, model_name="text-davinci-003", max_len=512, temp=0.7, num_log_probs=0, echo=False):
-    # call GPT-3 API until result is provided and then return it
-    response = None
-    received = False
-
-    while not received:
-        try:
-            response = openai.Completion.create(model=model_name,
-                                                prompt=prompt,
-                                                max_tokens=max_len,
-                                                temperature=temp,
-                                                logprobs=num_log_probs,
-                                                echo=echo)
-            received = True
-        except:
-            error = sys.exc_info()[0]
-            if error == openai.error.InvalidRequestError:
-                # something is wrong: e.g. prompt too long
-                print(f"InvalidRequestError\nPrompt passed in:\n\n{prompt}\n\n")
-                assert False
-            print("API error:", error)
-            time.sleep(1)
-    return response
+    return paragraphs
 
 def best_demos(query, bm25, demons_sents, k):
     tokenized_query = query.split(" ")
     top_machings = bm25.get_top_n(tokenized_query, demons_sents, k)
     return top_machings
 
 
@@ -285,15 +254,15 @@
 
     verbs = ["born.", " appointed.", " characterized.", " described.", " known.", " member.", " advocate.", "served.", "elected."]
     permitted_verbs = ["founding member."]
 
     atomic_facts = []
     new_atomic_facts = []
     new_para_breaks = []
-    
+
     for i, (sent, facts) in enumerate(_atomic_facts):
         sent = sent.strip()
         if len(sent.split())==1 and i not in para_breaks and i > 0:
             assert i not in para_breaks
             atomic_facts[-1][0] += " " + sent
             atomic_facts[-1][1] += facts
         else:
@@ -316,32 +285,32 @@
             if len(new_entities) > 0:
                 do_pass = False
                 for new_ent in new_entities:
                     pre_ent = None
                     for ent in entities:
                         if ent.startswith(new_ent):
                             pre_ent = ent
-                            break			
+                            break
                     if pre_ent is None:
                         do_pass = True
                         break
                     fact = fact.replace(new_ent, pre_ent)
                     covered_entities.add(pre_ent)
                 if do_pass:
                     continue
             if fact in new_facts:
                 continue
             new_facts.append(fact)
         try:
             assert entities==covered_entities
         except Exception:
             new_facts = facts # there is a bug in spacy entity linker, so just go with the previous facts
-        
+
         new_atomic_facts.append((sent, new_facts))
-    
+
     return new_atomic_facts, new_para_breaks
 
 def is_integer(s):
     try:
         s = int(s)
         return True
     except Exception:
```

### Comparing `factscore-0.1.2/factscore/clm.py` & `factscore-0.1.3/factscore/clm.py`

 * *Files identical despite different names*

### Comparing `factscore-0.1.2/factscore/download_data.py` & `factscore-0.1.3/factscore/download_data.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import argparse
 import os
 import subprocess
 
 
-def download_file(_id, dest):
-    if os.path.exists(dest):
+def download_file(_id, dest, cache_dir):
+    if os.path.exists(dest) or os.path.exists(os.path.join(cache_dir, dest)):
+        print ("[Already exists] Skipping", dest)
+        print ("If you want to download the file in another location, please specify a different path")
+        return
+
+    if os.path.exists(dest.replace(".zip", "")) or os.path.exists(os.path.join(cache_dir, dest.replace(".zip", ""))):
         print ("[Already exists] Skipping", dest)
         print ("If you want to download the file in another location, please specify a different path")
         return
 
     if "/" in dest:
         dest_dir = "/".join(dest.split("/")[:-1])
         if not os.path.isdir(dest_dir):
@@ -33,18 +38,18 @@
         ret_code = subprocess.run([command], shell=True)
         if ret_code.returncode != 0:
             print("Unzip {} ... [Failed]".format(dest))
         else:
             print("Unzip {} ... [Success]".format(dest))
 
 if __name__ == '__main__':
-    download_file("1IseEAflk1qqV0z64eM60Fs3dTgnbgiyt", "demos.zip")
-    download_file("1pUhBqQnrK9ZlgGdpP8LfPaG27yQRSIeT", "original_generation.zip")
-    download_file("1mekls6OGOKLmt7gYtHs0WGf5oTamTNat", "enwiki-20230401.db")
-
     cache_dir = ".cache/factscore"
     if not os.path.exists(cache_dir):
         os.makedirs(cache_dir)
 
+    download_file("1IseEAflk1qqV0z64eM60Fs3dTgnbgiyt", "demos.zip", cache_dir)
+    download_file("1enz1PxwxeMr4FRF9dtpCPXaZQCBejuVF", "data.zip", cache_dir)
+    download_file("1mekls6OGOKLmt7gYtHs0WGf5oTamTNat", "enwiki-20230401.db", cache_dir)
+
     # move the files to the cache directory
     subprocess.run(["mv demos %s" % cache_dir], shell=True)
-    subprocess.run(["mv enwiki-20230401.db %s" % cache_dir], shell=True)
+    subprocess.run(["mv enwiki-20230401.db %s" % cache_dir], shell=True)
```

### Comparing `factscore-0.1.2/factscore/factscorer.py` & `factscore-0.1.3/factscore/factscorer.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,19 +21,22 @@
         assert model_name in ["retrieval+llama", "retrieval+llama+npm", "retrieval+ChatGPT", "npm", "retrieval+ChatGPT+npm"]
         self.model_name = model_name
 
         self.db = {}
         self.retrieval = {}
         self.npm = {}
         self.batch_size = batch_size # batch size for retrieval
+        self.openai_key = openai_key
 
         self.cache_dir = cache_dir
         if not os.path.exists(cache_dir):
             os.makedirs(cache_dir)
 
+        self.af_generator = None
+
         if "llama" in model_name:
             self.lm = CLM("inst-llama-7B",
                           model_dir=os.path.join(cache_dir, "inst-llama-7B"),
                           cache_file=os.path.join(cache_dir, "inst-llama-7B.pkl"))
         elif "ChatGPT" in model_name:
             self.lm = OpenAIModel("ChatGPT",
                                   cache_file=os.path.join(cache_dir, "ChatGPT.pkl"),
@@ -50,14 +53,15 @@
         for k, v in self.retrieval.items():
             v.save_cache()
 
     def register_knowledge_source(self, name="enwiki-20230401", db_path=None, data_path=None):
         assert name not in self.retrieval, f"{name} already registered"
         if db_path is None:
             db_path = os.path.join(self.cache_dir, f"{name}.db")
+
         if data_path is None:
             data_path = os.path.join(self.cache_dir, f"{name}.jsonl")
 
         cache_path = os.path.join(self.cache_dir, f"retrieval-{name}.json")
         embed_cache_path = os.path.join(self.cache_dir, f"retrieval-{name}.pkl")
 
         self.db[name] = DocDB(db_path=db_path, data_path=data_path)
@@ -68,15 +72,15 @@
             self.npm[name] = NPM(Retrieval(self.db[name], cache_path, embed_cache_path, "bm25"),
                                  "npm-single",
                                  cache_file=os.path.join(self.cache_dir, f"npm-{name}.pkl"))
 
     def get_score(self,
                   topics,
                   generations,
-                  atomic_facts,
+                  atomic_facts=None,
                   knowledge_source=None,
                   return_atomic_facts=False,
                   return_individual_decisions=False,
                   verbose=False):
 
         if knowledge_source is None:
             # use the default one (enwiki-20230401)
@@ -89,29 +93,50 @@
         if type(topics)==len(generations)==str:
             topics = [topics]
             generations = [generations]
         else:
             assert type(topics)==type(generations)==list, "`topics` and `generations` should be lists."
             assert len(topics)==len(generations), "`topics` and `generations` should have the same length"
 
-        assert len(topics)==len(atomic_facts), "`topics` and `atomic_facts` should have the same length"
+        if atomic_facts is not None:
+            assert len(topics)==len(atomic_facts), "`topics` and `atomic_facts` should have the same length"
+        else:
+            if self.af_generator is None:
+                self.af_generator = AtomicFactGenerator(key_path=self.openai_key,
+                                                        demon_dir=os.path.join(self.cache_dir, "demos"),
+                                                        gpt3_cache_file=os.path.join(self.cache_dir, "InstructGPT.pkl"))
+
+            if verbose:
+                topics = tqdm(topics)
+
+            new_topics, new_generations, new_atomic_facts = [], [], []
+            for topic, gen in zip(topics, generations):
+                curr_afs, _ = self.af_generator.run(gen)
+                curr_afs = [fact for _, facts in curr_afs for fact in facts]
+                if len(curr_afs)==0:
+                    # abstain from answering
+                    continue
+                new_topics.append(topic)
+                new_generations.append(gen)
+                new_atomic_facts.append(curr_afs)
+            topics, generations, atomic_facts = new_topics, new_generations, new_atomic_facts
 
         if verbose:
             topics = tqdm(topics)
 
         scores = []
         decisions = []
         for topic, generation, facts in zip(topics, generations, atomic_facts):
             decision = self._get_score(topic, generation, facts, knowledge_source)
             score = np.mean([d["is_supported"] for d in decision])
             decisions.append(decision)
             scores.append(score)
 
         if return_atomic_facts:
-            return np.mean(scores), [[d["atom"] for d in ds] for ds in decisions]
+            return np.mean(scores), atomic_facts
 
         if return_individual_decisions:
             return np.mean(scores), decisions
 
         return np.mean(scores)
 
     def _get_score(self, topic, generation, atomic_facts, knowledge_source):
@@ -123,15 +148,14 @@
                 definition = "Answer the question about {} based on the given context.\n\n".format(topic)
                 context = ""
                 for psg_idx, psg in enumerate(reversed(passages)):
                     context += "Title: {}\nText: {}\n\n".format(psg["title"], psg["text"].replace("<s>", "").replace("</s>", ""))
                 definition += context.strip()
                 if not definition[-1] in string.punctuation:
                     definition += "."
-                assert atom.endswith("."), atom
                 prompt = "{}\n\nInput: {} True or False?\nOutput:".format(definition.strip(), atom.strip())
                 output = self.lm.generate(prompt)
 
                 if type(output[1])==np.ndarray:
                     # when logits are available
                     logits = np.array(output[1])
                     assert logits.shape[0] in [32000, 32001]
@@ -164,77 +188,54 @@
         return decisions
 
 if __name__ == '__main__':
 
     parser = argparse.ArgumentParser()
     parser.add_argument('--data_path',
                         type=str,
-                        default="data/src-light/bio_PerplexityAI_v0.1.jsonl")
+                        default="data/labeled/InstructGPT.jsonl")
     parser.add_argument('--model_name',
                         type=str,
                         default="retrieval+ChatGPT")
     parser.add_argument('--openai_key',
                         type=str,
                         default="api.key")
     parser.add_argument('--cache_dir',
                         type=str,
                         default=".cache/factscore/")
+    parser.add_argument('--use_atomic_facts',
+                        action="store_true")
+    parser.add_argument('--verbose',
+                        action="store_true")
+    parser.add_argument('--n_samples',
+                        type=int,
+                        default=None)
+
     args = parser.parse_args()
 
-    def extract_topic(dp):
-        key_to_use = "prompt" if "prompt" in dp else "input"
-        assert dp[key_to_use].startswith("Question: Tell me a bio of "), dp[key_to_use]
-        topic = dp[key_to_use].split("\n")[0].split("Tell me a bio of")[-1].strip()
-        assert topic.endswith(".")
-        return topic[:-1]
-
-    fs = FactScorer(model_name=args.model_name, cache_dir=args.cache_dir, openai_key=args.openai_key)
-    af_generator = AtomicFactGenerator(key_path=args.openai_key, demon_dir=os.path.join(args.cache_dir, "demos"))
-
-    topics = []
-    generations = []
-    atomic_facts = []
+    fs = FactScorer(args.model_name, args.cache_dir, args.openai_key)
 
     tot = 0
-    with open(args.data_path, "r") as f:
-        for line in tqdm(f, desc="Getting atomic facts..."):
-            tot += 1
+    topics, generations, atomic_facts = [], [], []
+    with open(args.data_path) as f:
+        for line in f:
             dp = json.loads(line)
-            gen = ""
-            facts = []
-            if "response" in dp and dp["response"] is not None:
-                # v0.1 files which have human written atomic facts
-                response = dp["response"]
-                for sent_idx, sent_dp in enumerate(response["fact_data"]):
-                    gen += sent_dp["orig_sentence"] + " "
-                    facts += sent_dp["orig_facts"]
-                topics.append(extract_topic(dp))
-                generations.append(gen)
-
-            elif "output" in dp and dp["output"] is not None:
-                # TODO: is processing para breaks critical for correct FactScore?
-                atomic_facts, para_breaks = af_generator.run(dp["output"])
-                for sent, afs in atomic_facts:
-                    gen += sent + " "
-                    facts.extend(afs)
-                topics.append(extract_topic(dp))
-
-            if facts:
-                for i, fact in enumerate(facts):
-                    # this should be manually fixed before releasing the data
-                    if not fact.endswith("."):
-                        facts[i] += "."
-
-                atomic_facts.append(facts)
-
-            if "ChatGPT" in args.model_name and tot == 100:
+            tot += 1
+            if args.use_atomic_facts:
+                assert "annotations" in dp, "You can specify `--use_atomic_facts` only when atomic facts are available in the input data already."
+                if dp["annotations"] is None:
+                    continue
+                topics.append(dp["topic"])
+                generations.append(dp["output"])
+                atomic_facts.append([atom["text"] for sent in dp["annotations"] for atom in sent["model-atomic-facts"]])
+            else:
+                topics.append(dp["topic"])
+                generations.append(dp["output"])
+            if args.n_samples is not None and tot==args.n_samples:
                 break
 
-    score, decisions = fs.get_score(topics,
-                                    generations,
-                                    atomic_facts=atomic_facts,
-                                    return_individual_decisions=True,
-                                    verbose=True)
-    print ("%s\t%.1f" % (args.model_name, 100*score))
-
+    score = fs.get_score(topics=topics, generations=generations, atomic_facts=atomic_facts if args.use_atomic_facts else None, verbose=args.verbose)
+    print (score)
     fs.save_cache()
 
+
+
```

### Comparing `factscore-0.1.2/factscore/lm.py` & `factscore-0.1.3/factscore/lm.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,23 +15,23 @@
 
     def generate(self, prompt, sample_idx=0, max_sequence_length=2048, max_output_length=128, verbose=False):
         prompt = prompt.strip() # it's important not to end with a whitespace
         cache_key = f"{prompt}_{sample_idx}"
 
         if cache_key in self.cache_dict:
             return self.cache_dict[cache_key]
-        
+
         if self.model is None:
             self.load_model()
-        
+
         if prompt.endswith(" True or False?\nAnswer:"):
             generated = self._generate(prompt, max_sequence_length=max_sequence_length, max_output_length=1)
         else:
             generated = self._generate(prompt, max_sequence_length=max_sequence_length, max_output_length=max_output_length)
-        
+
         self.cache_dict[cache_key] = generated
         self.add_n += 1
         return generated
 
     def save_cache(self):
         if self.add_n == 0:
             return
@@ -40,15 +40,14 @@
         for k, v in self.load_cache().items():
             self.cache_dict[k] = v
 
         with open(self.cache_file, "wb") as f:
             pickle.dump(self.cache_dict, f)
 
     def load_cache(self):
-        print (self.cache_file)
         if os.path.exists(self.cache_file):
             with open(self.cache_file, "rb") as f:
                 cache = pickle.load(f)
         else:
             cache = {}
         return cache
```

### Comparing `factscore-0.1.2/factscore/npm.py` & `factscore-0.1.3/factscore/npm.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,30 +13,30 @@
 class NPM(LM):
 
     def __init__(self, bm25, model_name, cache_file):
         assert model_name.startswith("npm")
         self.bm25 = bm25
         self.model_name = model_name
         self.model = None
-        
+
         self.tokenizer = AutoTokenizer.from_pretrained("facebook/" + self.model_name)
         self.mask_id = self.tokenizer.mask_token_id
-        
+
         with open("roberta_stopwords.txt", "r") as f:
             self.stopwords = set()
             for line in f:
                 self.stopwords.add(int(line.strip()))
-        
+
         super().__init__(cache_file=cache_file)
 
     def load_model(self):
         self.model = AutoModelForMaskedLM.from_pretrained("facebook/" + self.model_name)
         self.model.cuda()
         self.model.eval()
-    
+
     def save_cache(self):
         super().save_cache()
         self.bm25.save_cache()
 
     def tokenize(self, texts, skip_special_tokens=False, padding=True):
         assert type(texts)==list
         all_input_ids = self.tokenizer(texts)["input_ids"]
```

### Comparing `factscore-0.1.2/factscore/openai_lm.py` & `factscore-0.1.3/factscore/openai_lm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from factscore.lm import LM
 import openai
 import sys
 import time
 import os
 import numpy as np
 
+
+
 class OpenAIModel(LM):
 
     def __init__(self, model_name, cache_file=None, key_path="api.key"):
         self.model_name = model_name
         self.key_path = key_path
         self.temp = 0.7
         self.save_interval = 100
@@ -38,15 +40,16 @@
             return output, response
         elif self.model_name == "InstructGPT":
             # Call API
             response = call_GPT3(prompt, temp=self.temp)
             # Get the output from the response
             output = response["choices"][0]["text"]
             return output, response
- 
+
+
 def call_ChatGPT(message, model_name="gpt-3.5-turbo", max_len=1024, temp=0.7):
     # call GPT-3 API until result is provided and then return it
     response = None
     received = False
     num_rate_errors = 0
     while not received:
         try:
@@ -64,14 +67,15 @@
                 print(f"InvalidRequestError\nPrompt passed in:\n\n{message}\n\n")
                 assert False
             
             print("API error: %s (%d). Waiting %dsec" % (error, num_rate_errors, np.power(2, num_rate_errors)))
             time.sleep(np.power(2, num_rate_errors))
     return response
 
+
 def call_GPT3(prompt, model_name="text-davinci-003", max_len=512, temp=0.7, num_log_probs=0, echo=False):
     # call GPT-3 API until result is provided and then return it
     response = None
     received = False
     num_rate_errors = 0
     while not received:
         try:
```

### Comparing `factscore-0.1.2/factscore/retrieval.py` & `factscore-0.1.3/factscore/retrieval.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,18 +95,20 @@
         self.connection.close()
 
     def get_text_from_title(self, title):
         """Fetch the raw text of the doc for 'doc_id'."""
         cursor = self.connection.cursor()
         cursor.execute("SELECT text FROM documents WHERE title = ?", (title,))
         results = cursor.fetchall()
-        results = None if results is None else [r for r in results]
+        results = [r for r in results]
         cursor.close()
-        assert len(results)==1
-        return [{"title": title, "text": para} for para in results[0][0].split(SPECIAL_SEPARATOR)]
+        assert results is not None and len(results)==1, f"`topic` in your data ({title}) is likely to be not a valid title in the DB."
+        results = [{"title": title, "text": para} for para in results[0][0].split(SPECIAL_SEPARATOR)]
+        assert len(results)>0, f"`topic` in your data ({title}) is likely to be not a valid title in the DB."
+        return results
 
 class Retrieval(object):
 
     def __init__(self, db, cache_path, embed_cache_path,
                  retrieval_type="gtr-t5-large", batch_size=None):
         self.db = db
         self.cache_path = cache_path
```

### Comparing `factscore-0.1.2/factscore/utils.py` & `factscore-0.1.3/factscore/utils.py`

 * *Files identical despite different names*

### Comparing `factscore-0.1.2/pyproject.toml` & `factscore-0.1.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "factscore"
-version = "0.1.2"
+version = "0.1.3"
 description = "FactScore is an automatic evaluation metric for factual precision in long-form text generation. It uses large language models and retrieval to break down generations into atomic facts and then measure the correctness with respect to a knowledge source (like Wikipedia)."
 authors = ["Sewon Min <sewon@cs.washington.edu>", "Kalpesh Krishna <kalpesh@cs.umass.edu>", "Xinxi Lyu <alrope@cs.washington.edu>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7.1"
 torch = "^1.13.0"
 sentence-transformers = "^2.2.2"
 transformers = "^4.29.2"
 openai = "^0.27.7"
 rank-bm25 = "^0.2.2"
 spacy = "^3.5.3"
 pysqlite-binary = "^0.5.0"
-
+nltk = "^3.8.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `factscore-0.1.2/PKG-INFO` & `factscore-0.1.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: factscore
-Version: 0.1.2
+Version: 0.1.3
 Summary: FactScore is an automatic evaluation metric for factual precision in long-form text generation. It uses large language models and retrieval to break down generations into atomic facts and then measure the correctness with respect to a knowledge source (like Wikipedia).
 License: MIT
 Author: Sewon Min
 Author-email: sewon@cs.washington.edu
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: openai (>=0.27.7,<0.28.0)
 Requires-Dist: pysqlite-binary (>=0.5.0,<0.6.0)
 Requires-Dist: rank-bm25 (>=0.2.2,<0.3.0)
 Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0)
 Requires-Dist: spacy (>=3.5.3,<4.0.0)
 Requires-Dist: torch (>=1.13.0,<2.0.0)
 Requires-Dist: transformers (>=4.29.2,<5.0.0)
@@ -53,33 +54,44 @@
 
 ## Running FactScore
 
 ```bash
 python -m factscore.factscorer --data_path {data_path} --model_name {estimator_name} --cache_dir {cache_dir} --openai_key {openai_key}
 ```
 
-- `data_path` can be something like `data/src-light/bio_ChatGPT_v0.2.jsonl` which is in a format we have been using so far. TODO for simplying the format and allowing it to take any topics/generations.
+- `data_path` can be something like `data/unlabeled/InstructGPT.jsonl`. It should be a `.jsonl` format where each line contains `topic` (a topic entity that corresponds to the Wikipedia title) and `output` (a generation from the model).
 - `model_name`: `retrieval+ChatGPT`, `retrieval+ChatGPT+npm`, two more configs (`retrieval+llama`, `retrieval+llama+npm`) coming soon!
 - `cache_dir`: `.cache/factscore` by default.
-- `openai_key`: File containing API Key, needed when ChatGPT is being used.
+- `openai_key`: File containing OpenAI API Key.
+- `use_atomic_facts`: If specified, it uses model-generated atomic facts released as part of our data instead of running the atomic fact generator. You can't specify it if you are running new model generations.
+- `n_samples`: If specified, it runs the model on a subset of the data.
+- `verbose`: If specified, it shows the progress bar.
 
 For example,
 
 ```python
 python -m factscore.factscorer \
-    --data_path original_generation/v0.2/answers_mpt-7b_bio_test_addtional.jsonl \
+    --data_path data/unlabeled/InstructGPT.jsonl \
     --model_name "retrieval+ChatGPT" \
     --cache_dir ".cache/factscore" \
-    --openai_key "api.key"
+    --openai_key "api.key" \
+    --verbose
 ```
 
 It uses `enwiki-20230401` by default, and will download the database from our Google drive.
 
 Instructions to use Instruct-LLAMA-7B or your own LM coming soon!
 
+## To generate outputs from your own LM and evaluate them.
+
+There're two sets of prompt entities, `data/labeled/prompt_entities.txt` (183 entities) and `data/unlabeled/prompt_entities.txt` (500 entities). Each line contains the name of the person (which is also a corresponding Wikipedia title). You can use the labeled version if you want to be compatible with the data under `data/labeled` (Section 3 and Section 4.2 in the paper), and use the unlabeled version if you want to be compatible with the data under `data/unlabeled` (Section 4.3 in the paper).
+
+You can prompt your LM with your own prompt (we used `Question: Tell me a bio of <entity>.`) and create a .jsonl file, where each line has `topic` (entity name, exactly same as the one from `.txt` file) and `output` (generation from LM). This can be fed into `factscore.factscorer` using `--data_path`.
+
+
 ## To use a custom knowledge source.
 You need a `.jsonl` file where each line is a dictionary containing `title` and `text`. `text` can either be a string or a list of strings (e.g., sections).
 
 ```python
 from factscore.factscorer import FactScorer
 
 fs = FactScorer()
```

