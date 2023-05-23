# Comparing `tmp/tree-of-thoughts-0.1.6.tar.gz` & `tmp/tree-of-thoughts-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tree-of-thoughts-0.1.6.tar", last modified: Mon May 22 15:58:09 2023, max compression
+gzip compressed data, was "tree-of-thoughts-0.1.7.tar", last modified: Tue May 23 16:21:34 2023, max compression
```

## Comparing `tree-of-thoughts-0.1.6.tar` & `tree-of-thoughts-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:58:09.751886 tree-of-thoughts-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-22 15:57:58.000000 tree-of-thoughts-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-22 15:58:09.751886 tree-of-thoughts-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-05-22 15:57:58.000000 tree-of-thoughts-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 15:58:09.751886 tree-of-thoughts-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-22 15:57:58.000000 tree-of-thoughts-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:58:09.751886 tree-of-thoughts-0.1.6/tree_of_thoughts/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-22 15:57:58.000000 tree-of-thoughts-0.1.6/tree_of_thoughts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15498 2023-05-22 15:57:58.000000 tree-of-thoughts-0.1.6/tree_of_thoughts/treeofthoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:58:09.751886 tree-of-thoughts-0.1.6/tree_of_thoughts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-22 15:58:09.000000 tree-of-thoughts-0.1.6/tree_of_thoughts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-22 15:58:09.000000 tree-of-thoughts-0.1.6/tree_of_thoughts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 15:58:09.000000 tree-of-thoughts-0.1.6/tree_of_thoughts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-22 15:58:09.000000 tree-of-thoughts-0.1.6/tree_of_thoughts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-22 15:58:09.000000 tree-of-thoughts-0.1.6/tree_of_thoughts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:21:34.960389 tree-of-thoughts-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-23 16:21:22.000000 tree-of-thoughts-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-23 16:21:34.960389 tree-of-thoughts-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13559 2023-05-23 16:21:22.000000 tree-of-thoughts-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 16:21:34.960389 tree-of-thoughts-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-23 16:21:22.000000 tree-of-thoughts-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:21:34.960389 tree-of-thoughts-0.1.7/tree_of_thoughts/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-23 16:21:22.000000 tree-of-thoughts-0.1.7/tree_of_thoughts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18892 2023-05-23 16:21:22.000000 tree-of-thoughts-0.1.7/tree_of_thoughts/treeofthoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:21:34.960389 tree-of-thoughts-0.1.7/tree_of_thoughts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-23 16:21:34.000000 tree-of-thoughts-0.1.7/tree_of_thoughts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-23 16:21:34.000000 tree-of-thoughts-0.1.7/tree_of_thoughts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 16:21:34.000000 tree-of-thoughts-0.1.7/tree_of_thoughts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 16:21:34.000000 tree-of-thoughts-0.1.7/tree_of_thoughts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-23 16:21:34.000000 tree-of-thoughts-0.1.7/tree_of_thoughts.egg-info/top_level.txt
```

### Comparing `tree-of-thoughts-0.1.6/LICENSE` & `tree-of-thoughts-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tree-of-thoughts-0.1.6/PKG-INFO` & `tree-of-thoughts-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-of-thoughts
-Version: 0.1.6
+Version: 0.1.7
 Summary: Tree of Thoughts - Pytorch
 Home-page: https://github.com/kyegomez/tree-of-thoughts
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `tree-of-thoughts-0.1.6/README.md` & `tree-of-thoughts-0.1.7/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # Tree of Thoughts 🌳🌲🌴🌿🍃
 
 ![tree of thoughts banner](tree-of-thoughts.jpeg)
 
 [Paper link](https://arxiv.org/pdf/2305.10601.pdf)
 
-Tree of Thoughts (ToT) is a powerful and flexible algorithm for leveraging pre-trained language models to solve various problems by exploring multiple reasoning paths. It's designed to be plug-and-play, allowing users to easily connect their models and use the Tree of Thoughts method.
+Tree of Thoughts (ToT) is an all-new powerful and flexible algorithm that advances model reasoning by a whopping 70%. This is an plug in and play verision, connect your own models and enjoy superintelligence!
+
+
+Share this repository by clicking on the following buttons 😊 
+
+[![Twitter](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Ftree-of-thoughts)](https://twitter.com/intent/tweet?text=Check%20out%20this%20amazing%20project%20on%20improving%20AI%20reasoning%20-%20Tree%20of%20Thoughts!%20https://github.com/kyegomez/tree-of-thoughts)
+[![LinkedIn](https://img.shields.io/badge/Share-LinkedIn-blue?style=social&logo=linkedin)](https://www.linkedin.com/sharing/share-offsite/?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Ftree-of-thoughts)
 
 # Join Agora, Creators United
 This implementation of Tree of Thoughts is brought to you by Agora, Agora advances Humanity with open source SOTA Multi-Modality AI research! We plan on combating Humanity's grandest root problems like food insecurity, planetary insecurity, and disease, and hopefully death itself.
 
 [Join our Discord and contribute to this project](https://discord.gg/qUtxnK2NMf)
 
 ## Getting started
@@ -22,58 +28,49 @@
 Navigate to the repository folder: ``` cd tree-of-thoughts```
 
 ```pip install openai```
 
 Create a Python script (e.g., example.py) and import the necessary classes:
 
 ``` python
-from tree_of_thoughts import OpenAILanguageModel, CustomLanguageModel, TreeofThoughts, OptimizedOpenAILanguageModel, OptimizedTreeofThoughts
+from tree_of_thoughts.treeofthoughts import OpenAILanguageModel, CustomLanguageModel, TreeofThoughts, OptimizedOpenAILanguageModel, OptimizedTreeofThoughts
 
-#v1
-model = OpenAILanguageModel('api key')
-
-#v2 parallel execution, caching, adaptive temperature
-model = OptimizedOpenAILanguageModel('api key')
+use_v2 = False
+api_key=""
+api_base= "" # leave it blank if you simply use default openai api url
+
+if not use_v2:
+    #v1
+    model = OpenAILanguageModel(api_key=api_key, api_base=api_base)
+else:
+    #v2 parallel execution, caching, adaptive temperature
+    model = OptimizedOpenAILanguageModel(api_key=api_key, api_base=api_base)
 
 #choose search algorithm('BFS' or 'DFS')
 search_algorithm = "BFS"
 
 #cot or propose
 strategy="cot"
 
 # value or vote
 evaluation_strategy = "value"
 
-#create an instance of the tree of thoughts class v1
-tree_of_thoughts = TreeofThoughts(model, search_algorithm)
-
-#or v2 -> dynamic beam width -< adjust the beam width [b] dynamically based on the search depth quality of the generated thoughts
-tree_of_thoughts= OptimizedTreeofThoughts(model, search_algorithm)
-
-input_problem = "What are next generation reasoning methods for Large Language Models"
-k = 5
-T = 3
-b = 5
-vth = 0.5
-
-# # Optimal nominal values for the stopping conditions
+if not use_v2:
+    #create an instance of the tree of thoughts class v1
+    tree_of_thoughts = TreeofThoughts(model, search_algorithm)
+else:
+    #or v2 -> dynamic beam width -< adjust the beam width [b] dynamically based on the search depth quality of the generated thoughts
+    tree_of_thoughts= OptimizedTreeofThoughts(model, search_algorithm)
 
-# confidence = 0.9 #HIGH QUALITY SOLIUTION FOUND
-
-# max_iterations = 5 # MAX ITERATIONS 10
-
-# convergence_threshold = 0.01 #Convergence Check: Monitor the change in evaluation values between consecutive iterations. If the change in evaluation values is below a certain threshold for a specified number of consecutive iterations, the algorithm can stop and return the solution.
-
-# convergence_count = 5
-
-#call the solve method with the input problem and other params
-solution = tree_of_thoughts.solve(input_problem, k, T, b, vth)
+input_problem = "use 4 numbers and basic arithmetic operations (+-*/) to obtain 24"
+    
+solution = tree_of_thoughts.solve(input_problem)
 
-#use the solution in env
-print(f"solution: {solution}")
+#use the solution in your production environment
+print(f'solution {solution}')
 
 
 ```
 
 Or Integrate your own custom language model:
 
 ```python
@@ -168,35 +165,31 @@
 
 
 # Contributing
 This algorithm is still infant yet it's potential remains unimaginable, let's advance the reasoning of AI's together under this banner.
 
 # Share With Your Network
 
-We are excited about the potential of the Tree of Thoughts project and we hope you are too! If you like this project, we'd greatly appreciate it if you could share it with your friends, colleagues, and social network. Every share helps us reach more people, get more feedback, and continue improving the project.
-
 You can easily share this repository by clicking on the following buttons:
 
 [![Twitter](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Ftree-of-thoughts)](https://twitter.com/intent/tweet?text=Check%20out%20this%20amazing%20project%20on%20improving%20AI%20reasoning%20-%20Tree%20of%20Thoughts!%20https://github.com/kyegomez/tree-of-thoughts)
 [![LinkedIn](https://img.shields.io/badge/Share-LinkedIn-blue?style=social&logo=linkedin)](https://www.linkedin.com/sharing/share-offsite/?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Ftree-of-thoughts)
 
 For Instagram, while it doesn't directly support sharing of web links, you can share the screenshot of our project and the link in your caption or bio. You can download the project screenshot by clicking the image below:
 
 [![Tree of Thoughts](https://github.com/kyegomez/tree-of-thoughts/raw/main/tree-of-thoughts.jpeg)](https://github.com/kyegomez/tree-of-thoughts/raw/main/tree-of-thoughts.jpeg)
 
 We greatly appreciate any help in spreading the word about our project. Thank you for your support!
 
 
 ## Roadmap
 
-Provide ready to use generate thoughts function -- done
-
-Provide ready to use evaluate states function -- done
+now:
+Generate suite of evaluations used in the paper testing AI agents with other reasoning methods like COT and self consistency and run them in parallel to conduct evaluation experiments.
 
-now
 Implement a more sophisticated prompt engineering strategy to guide the model's reasoning process more effectively.
 
 Make TreeofThoughts class completely customizable with a config yml file with params like
 chatbot:
     type: "openai"
     max_context_length: 8000
     include_chat_history_in_query: false
@@ -242,14 +235,59 @@
 3. Develop a method for combining different modalities in the search tree, allowing the algorithm to reason across different data types.
 4. Implement and test the multi-modal Tree of Thoughts algorithm with various problems and datasets.
 5. Optimize the algorithm for performance and resource usage, ensuring it scales well with large multi-modal datasets.
 6. Publish the results and gather feedback from the community to further improve the multi-modal Tree of Thoughts algorithm.
 
 Join us on this exciting journey to advance the Tree of Thoughts algorithm to multi-modality superintelligence! 🚀
 
+# The Compiler
+
+[Utilizing Tree of Thoughts for optimal program synthesis](https://github.com/kyegomez/the-compiler)
+
+![the compiler banner](https://github.com/kyegomez/the-compiler/raw/main/the-compiler.png)
+
+Welcome to _The Compiler_, a novel child project under the Tree of Thoughts (ToT) paradigm. This project is crafted with the intent of making autonomous programming not just a reality, but an effortless task for you. 
+
+In essence, _The Compiler_ allows you to "grow" any program you can dream of. By providing a high-level specification of the product you would like, you can sit back and let _The Compiler_ do the heavy lifting. 
+
+## Overview 
+
+_The Compiler_ leverages the ToT framework and large language models (LLMs) to handle the programming process, from abstract specifications to a working program. 
+
+Here's a basic breakdown of the workflow:
+
+1. **Input**: You provide an abstract specification for the product you would like.
+2. **Unit Tests Generation**: We use an LLM on ToT to produce a suite of unit tests for the code.
+3. **Run ToT**: We run the Tree of Thoughts LLM on the given specification, using the generated unit tests as the evaluation score.
+4. **Output**: Ready to use program!
+
+## Architecture
+
+The Compiler, leveraging the Tree of Thoughts paradigm, consists of several primary components, including the Specification Parser, Thought Decomposer, Thought Generator, State Evaluator, and the Search Algorithm. 
+
+1. **Specification Parser**: This interprets your high-level input specifications and translates them into a format that the Thought Decomposer can understand and work with.
+
+2. **Thought Decomposer**: This component breaks down the programming problem into manageable "thoughts" or steps.
+
+3. **Thought Generator**: It generates potential thoughts or steps from the current state using two strategies, either sampling thoughts independently or proposing thoughts sequentially.
+
+4. **State Evaluator**: It evaluates the progress of different states towards solving the programming problem, acting as a heuristic for the Search Algorithm.
+
+5. **Search Algorithm**: This module determines which states to keep exploring and in which order. It employs either Breadth-First Search (BFS) or Depth-First Search (DFS), depending on the nature of the problem.
+
+## Share The Compiler
+
+If you find this project exciting and think others might benefit from it, feel free to share it. Use the buttons below to share it on various social media platforms:
+
+- [Share on Twitter](http://twitter.com/share?text=Check%20out%20The%20Compiler%20project%20on%20GitHub!%20It%20allows%20you%20to%20autonomously%20create%20programs%20using%20abstract%20specifications.&url=https://github.com/kyegomez/the-compiler)
+- [Share on LinkedIn](http://www.linkedin.com/shareArticle?mini=true&url=https://github.com/kyegomez/the-compiler&title=The%20Compiler%20Project&summary=This%20project%20is%20a%20revolution%20in%20autonomous%20programming!%20Check%20it%20out%20on%20GitHub.)
+- [Share on Facebook](http://www.facebook.com/sharer.php?u=https://github.com/kyegomez/the-compiler)
+
+Let's revolutionize the world of programming together with _The Compiler_!
+
 
 
 # Acknowledgements
 
 Thanks to: Shunyu Yao Princeton University, Dian Yu Google DeepMind, Jeffrey Zhao, Google DeepMind, Izhak Shafran Google DeepMind, Thomas L. Griffiths, Princeton University, Yuan Cao Google DeepMind, Karthik Narasimha, Princeton University for sharing this amazing work with the world!
 
-And, thanks to Phil Wang or Lucidrains for inspiring me to devote myself to open source AI Research
+And, thanks to Phil Wang or Lucidrains for inspiring me to devote myself to open source AI Research
```

### Comparing `tree-of-thoughts-0.1.6/setup.py` & `tree-of-thoughts-0.1.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'tree-of-thoughts',
   packages = find_packages(exclude=[]),
-  version = '0.1.6',
+  version = '0.1.7',
   license='MIT',
   description = 'Tree of Thoughts - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/tree-of-thoughts',
   keywords = [
     'artificial intelligence',
     'deep learning',
     'optimizers',
     "Prompt Engineering"
   ],
   install_requires=[
-    'torch>=1.6'
+    'openai'
   ],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3.6',
   ],
-)
+)
```

### Comparing `tree-of-thoughts-0.1.6/tree_of_thoughts/treeofthoughts.py` & `tree-of-thoughts-0.1.7/tree_of_thoughts/treeofthoughts.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import concurrent.futures
 from abc import ABC, abstractmethod
 import openai
+import os
+import re
 import time
 
-
 class AbstractLanguageModel(ABC):
     @abstractmethod
     def generate_thoughts(self, state, k):
         pass
 
     @abstractmethod
     def evaluate_states(self, states):
@@ -22,82 +23,153 @@
         #implement the thought generation logic using self.model
         pass
 
     def evaluate_states(self, states):
         #implement state evaluation logic using self.model
         pass
 class OpenAILanguageModel(AbstractLanguageModel):
-    def __init__(self, api_key, strategy="cot", evaluation_strategy="value"):
-        openai.api_key = api_key
+    def __init__(self, api_key, strategy="cot", evaluation_strategy="value", api_base="", api_model="", enable_ReAct_prompting=True):
+        if api_key == "" or api_key == None:
+            api_key = os.environ.get("OPENAI_API_KEY", "")
+        if api_key != "":
+            openai.api_key = api_key
+        else:
+            raise Exception("Please provide OpenAI API key")
+
+        if api_base == ""or api_base == None:
+            api_base = os.environ.get("OPENAI_API_BASE", "")  # if not set, use the default base path of "https://api.openai.com/v1"
+        if api_base != "":
+            # e.g. https://api.openai.com/v1/ or your custom url
+            openai.api_base = api_base
+            print(f'Using custom api_base {api_base}')
+            
+        if api_model == "" or api_model == None:
+            api_model = os.environ.get("OPENAI_API_MODEL", "")
+        if api_model != "":
+            self.api_model = api_model
+        else:
+            self.api_model = "text-davinci-003"
+        print(f'Using api_model {self.api_model}')
+
+        self.use_chat_api = 'gpt' in self.api_model
+
+        # reference : https://www.promptingguide.ai/techniques/react
+        self.ReAct_prompt = ''
+        if enable_ReAct_prompting:
+            self.ReAct_prompt = "Write down your observations in format 'Observation:xxxx', then write down your thoughts in format 'Thoughts:xxxx'."
+        
         self.strategy = strategy
         self.evaluation_strategy = evaluation_strategy
 
+    def openai_api_call_handler(self, prompt, max_tokens, temperature, k=1, stop=None):
+        while True:
+            try:
+                if self.use_chat_api:
+                    messages = [
+                        {
+                            "role": "user",
+                            "content": prompt
+                        }
+                    ]
+                    response = openai.ChatCompletion.create(
+                        model=self.api_model,
+                        messages=messages,
+                        max_tokens=max_tokens,
+                        temperature=temperature,
+                    )
+                else:
+                    response = openai.Completion.create(
+                        engine=self.api_model,
+                        prompt=prompt,
+                        n=k,
+                        max_tokens=max_tokens,
+                        stop=stop,
+                        temperature=temperature,
+                    )
+                return response
+            except openai.error.RateLimitError as e:
+                sleep_duratoin = os.environ.get("OPENAI_RATE_TIMEOUT", 30)
+                print(f'{str(e)}, sleep for {sleep_duratoin}s, set it by env OPENAI_RATE_TIMEOUT')
+                time.sleep(sleep_duratoin)
+
+    def openai_choice2text_handler(self, choice):
+        if self.use_chat_api:
+            text = choice['message']['content']
+        else:
+            text = choice.text.strip()
+        return text
+
     def generate_thoughts(self, state, k):
         state_text = ' '.join(state)
         
-        prompt = f"Given the current state of reasoning: '{state_text}', generate {k} coherent thoughts to continue the reasoning process:"
-        response = openai.Completion.create(
-            engine="text-davinci-003",
-            prompt=prompt,
-            n=k,
-            max_tokens=50,
-            stop=None,
-            temperature=0.5,
-        )
-        thoughts = [choice.text.strip() for choice in response.choices]
+        prompt = f"Given the current state of reasoning: '{state_text}', generate {1} coherent thoughts to continue the reasoning process:"
+        prompt += self.ReAct_prompt
+        if self.use_chat_api:
+            new_prompt_success = False
+            """
+            # Try prompt and parse in a single shot to save tokens (but if we fail, we end up spending more tokens)
+            new_prompt = prompt + "Thought string should be output in a format that can be parsed into python array in format [xxx,xxx,xxx]"
+            response = self.openai_api_call_handler(new_prompt, 100 * k, 0.5, 1)
+            text = self.openai_choice2text_handler(response.choices[0])
+            re_parse = re.search(r'\[(.*?)\]', text)
+            if re_parse:
+                thoughts_str = re_parse.group(1)
+                if thoughts_str:
+                    thoughts = thoughts_str.split(',')
+                    new_prompt_success = len(thoughts) == k 
+                    if not new_prompt_success:
+                        print(f"Fall back to multi-prompt for chat-completion due to parse fail {text}")
+
+            """
+            if not new_prompt_success:
+                thoughts = []
+                for _ in range(k):
+                    response = self.openai_api_call_handler(prompt, 50, 0.5, k)
+                    text = self.openai_choice2text_handler(response.choices[0])
+                    thoughts += [text]
+            
+        else:
+            response = self.openai_api_call_handler(prompt, 50, 0.5, k)
+            thoughts = [self.openai_choice2text_handler(choice) for choice in response.choices]
         # print(thoughts)
         print(f"Generated thoughts: {thoughts}")
         return thoughts
 
     def evaluate_states(self, states):
         if self.evaluation_strategy == 'value':
             state_values = {}
             for state in states:
                 state_text = ' '.join(state)
-                prompt = f"Given the current state of reasoning: '{state_text}', evaluate its value as a float between 0 and 1:"
-                response = openai.Completion.create(
-                    engine="text-davinci-003",
-                    prompt=prompt,
-                    n=1,
-                    max_tokens=10,
-                    stop=None,
-                    temperature=1,
-                )
+                prompt = f"Given the current state of reasoning: '{state_text}', evaluate its value as a float between 0 and 1, and NOTHING ELSE:"
+                response = self.openai_api_call_handler(prompt, 10, 1)
                 try:
-                    value_text = response.choices[0].text.strip()
+                    value_text = self.openai_choice2text_handler(response.choices[0])
                     print(f"Value text {value_text}")
-                    value = float(response.choices[0].text.strip())
+                    value = float(value_text)
                     print(f"value: {value}")
                 except ValueError:
                     value = 0  # Assign a default value if the conversion fails
                 state_values[state] = value
             return state_values
 
         elif self.evaluation_strategy == 'vote':
             states_text = '\n'.join([' '.join(state) for state in states])
-            prompt = f"Given the following states of reasoning, vote for the best state:\n{states_text}\n\nVote:"
-            response = openai.Completion.create(
-                engine="text-davinci-003",
-                prompt=prompt,
-                n=1,
-                max_tokens=50,
-                stop=None,
-                temperature=1,
-            )
-            best_state_text = response.choices[0].text.strip()
+            prompt = f"Given the following states of reasoning, vote for the best state:\n{states_text}\n\nVote, and NOTHING ELSE:"
+            response = self.openai_api_call_handler(prompt, 50, 1)
+            best_state_text = self.openai_choice2text_handler(response.choices[0])
             print(f"Best state text: {best_state_text}")
             best_state = tuple(best_state_text.split())
             return {state: 1 if state == best_state else 0 for state in states}
 
         else:
             raise ValueError("Invalid evaluation strategy. Choose 'value' or 'vote'.")
 
 class OptimizedOpenAILanguageModel(OpenAILanguageModel):
-    def __init__(self, api_key, strategy="cot", evaluation_strategy="value", cache_enabled=True):
-        super().__init__(api_key, strategy, evaluation_strategy)
+    def __init__(self, api_key, strategy="cot", evaluation_strategy="value", cache_enabled=True, api_base="", api_model="", enable_ReAct_prompting=True):
+        super().__init__(api_key, strategy, evaluation_strategy, api_base, api_model, enable_ReAct_prompting)
         self.cache_enabled = cache_enabled
         self.thought_cache = {}
         self.state_evaluation_cache = {}
 
     def parallel_generate_thoughts(self, states, k):
         with concurrent.futures.ThreadPoolExecutor() as executor:
             thoughts = list(executor.map(lambda state: self.generate_thoughts(state, k), states))
@@ -211,82 +283,70 @@
             return False
 
         dfs(x, 1)
         return max(output, key=lambda x: x[1]) if output else None
 
 
 class OptimizedTreeofThoughts(TreeofThoughts):
-    def solve(self, x, k, T, b, vth, timeout=None, confidence_threshold=0.9, max_iterations=10, convergence_threshold=0.1, convergence_count=5):
+    def solve(self, x, k=5, T=3, b=5, vth=0.5, timeout=None, confidence_threshold=0.9, max_iterations=10, convergence_threshold=0.1, convergence_count=5):
         start_time = time.time()
         if self.search_algorithm == 'BFS':
             while timeout is None or time.time() - start_time < timeout:
                 result = self.tot_bfs(x, k, T, b)
                 if result:
                     return result
         elif self.search_algorithm == 'DFS':
             while timeout is None or time.time() - start_time < timeout:
                 result = self.tot_dfs(x, k, T, vth, confidence_threshold=confidence_threshold, max_iterations=max_iterations, convergence_threshold=convergence_threshold, convergence_count=convergence_count)
                 if result:
                     return result
         else:
             raise ValueError("Invalid search algorithm. Choose 'BFS' or 'DFS'.")
 
-search_algorithm = "DFS"
-strategy = "cot"
-evaluation_strategy="vote"
-
-#create instance
-model = OptimizedOpenAILanguageModel('api key')
-
-
-tree_of_thoughts = OptimizedTreeofThoughts(model, search_algorithm)
-
-
-input_problem = "What are next generation reasoning methods for Large Language Models"
-k = 5
-T = 3
-b = 5
-vth = 0.5
-
-# # Optimal nominal values for the stopping conditions
-
-# confidence = 0.9 #HIGH QUALITY SOLIUTION FOUND
-
-# max_iterations = 5 # MAX ITERATIONS 10
-
-# convergence_threshold = 0.01 #Convergence Check: Monitor the change in evaluation values between consecutive iterations. If the change in evaluation values is below a certain threshold for a specified number of consecutive iterations, the algorithm can stop and return the solution.
-
-# convergence_count = 5
-
-#call the solve method with the input problem and other params
-solution = tree_of_thoughts.solve(input_problem, k, T, b, vth)
-
-#use the solution in yes
-print(f"solution: {solution}")
-
-"""
-should return something like this:
-
-['1. Utilizing reinforcement learning techniques to train large language models can be an effective approach to advancing them.\n2. Developing methods to better incorporate contextual information into large language models can help in their advancement.\n3. Incorpor', '1. Utilizing reinforcement learning techniques to allow for more efficient training of large language models.\n2. Incorporating transfer learning to leverage existing language models for faster and more accurate inference.\n3. Exploring the use of distributed', '1. Identifying and understanding key components of large language models such as natural language processing and machine learning algorithms.\n2. Utilizing methods such as transfer learning to quickly and efficiently train large language models.\n3. Incorporating', '1. Utilizing reinforcement learning techniques to train large language models can be an effective method of advancing them.\n2. Incorporating techniques such as transfer learning and data augmentation can help improve the performance of large language models.', '1. Identifying and understanding the underlying structure of language is essential to advancing large language models.\n2. Developing methods to effectively capture and represent the complexities of language is necessary for the advancement of large language models.\n3. Ut']
-0.8
-0.8
-['4. Analyzing and interpreting large language models to identify areas of improvement.\n5. Utilizing reinforcement learning to enable models to learn from mistakes and further improve accuracy.\n6. Leveraging automated data augmentation techniques to further improve', '4. Experimenting with different architectures and hyperparameters to determine the best model for a given task.\n5. Incorporating techniques such as data augmentation and ensembling to improve the performance of large language models.\n6', '4. Exploring methods to improve the efficiency of large language models such as using distributed computing techniques.\n5. Developing methods to reduce overfitting and improve generalization of large language models.\n6. Incorporating techniques such as', '4. Exploring and utilizing different types of data sets to train large language models.\n5. Developing strategies to optimize the training process and improve the performance of large language models.\n6. Applying advanced techniques such as deep learning', '4. Exploring methods such as reinforcement learning to improve the accuracy and robustness of large language models.\n5. Utilizing data augmentation techniques to increase the amount of training data available to the model.\n6. Incorpor']
-0.8
-0.8
-['7. Developing automated testing frameworks to validate the accuracy of large language models.\n8. Exploring ways to improve the scalability of large language models.\n9. Exploring ways to improve the efficiency of large language models.', '7. Applying methods such as active learning to further refine large language models.\n8. Developing and utilizing techniques such as knowledge distillation to compress large language models.\n9. Incorporating techniques such as semi-supervised', '7. Applying regularization techniques to reduce overfitting and improve generalization of large language models.\n8. Exploring the use of generative adversarial networks to improve the accuracy of large language models.\n9. Applying deep', '7. Developing methods to evaluate the performance of large language models on various tasks.\n8. Applying techniques such as hyperparameter tuning to optimize the performance of large language models.\n9. Utilizing adversarial training to', '7. Developing strategies to ensure large language models are able to generalize to unseen data.\n8. Incorporating methods such as meta-learning to further improve model performance.\n9. Utilizing techniques such as unsuper']
-0.7
-0.7
-['Once the key components of large language models have been identified and understood, the best reasoning methods to advance them include utilizing transfer learning to quickly train them, analyzing and interpreting them to identify areas of improvement, leveraging reinforcement learning to enable them to learn']
-0.7
-0.7
-['Exploring the use of meta-learning to enable models to rapidly adapt to new data and improve accuracy.']
-0.7
-0.7
-['One potential way to further advance large language models is to incorporate automated data augmentation techniques to create more varied datasets to train the models on, as well as leveraging reinforcement learning to enable the models to learn from mistakes and continually improve accuracy.']
-0.7
-0.7
-['By utilizing these methods, we can continue to advance large language models by improving their accuracy and performance. We can also use these methods to identify weaknesses in the models and make modifications to address them. Additionally, these methods can help us to develop']
-0.7
-0.7
-
+if __name__ == '__main__':
+    search_algorithm = "DFS"
+    strategy = "cot"
+    evaluation_strategy="vote"
+    
+    #create instance
+    model = OptimizedOpenAILanguageModel('api key')
+    
+    
+    tree_of_thoughts = OptimizedTreeofThoughts(model, search_algorithm)
+    
+    
+    input_problem = "What are next generation reasoning methods for Large Language Models"
 
-"""
+    
+    solution = tree_of_thoughts.solve(input_problem)
+    
+    #use the solution in yes
+    print(f"solution: {solution}")
+    
+    """
+    should return something like this:
+    
+    ['1. Utilizing reinforcement learning techniques to train large language models can be an effective approach to advancing them.\n2. Developing methods to better incorporate contextual information into large language models can help in their advancement.\n3. Incorpor', '1. Utilizing reinforcement learning techniques to allow for more efficient training of large language models.\n2. Incorporating transfer learning to leverage existing language models for faster and more accurate inference.\n3. Exploring the use of distributed', '1. Identifying and understanding key components of large language models such as natural language processing and machine learning algorithms.\n2. Utilizing methods such as transfer learning to quickly and efficiently train large language models.\n3. Incorporating', '1. Utilizing reinforcement learning techniques to train large language models can be an effective method of advancing them.\n2. Incorporating techniques such as transfer learning and data augmentation can help improve the performance of large language models.', '1. Identifying and understanding the underlying structure of language is essential to advancing large language models.\n2. Developing methods to effectively capture and represent the complexities of language is necessary for the advancement of large language models.\n3. Ut']
+    0.8
+    0.8
+    ['4. Analyzing and interpreting large language models to identify areas of improvement.\n5. Utilizing reinforcement learning to enable models to learn from mistakes and further improve accuracy.\n6. Leveraging automated data augmentation techniques to further improve', '4. Experimenting with different architectures and hyperparameters to determine the best model for a given task.\n5. Incorporating techniques such as data augmentation and ensembling to improve the performance of large language models.\n6', '4. Exploring methods to improve the efficiency of large language models such as using distributed computing techniques.\n5. Developing methods to reduce overfitting and improve generalization of large language models.\n6. Incorporating techniques such as', '4. Exploring and utilizing different types of data sets to train large language models.\n5. Developing strategies to optimize the training process and improve the performance of large language models.\n6. Applying advanced techniques such as deep learning', '4. Exploring methods such as reinforcement learning to improve the accuracy and robustness of large language models.\n5. Utilizing data augmentation techniques to increase the amount of training data available to the model.\n6. Incorpor']
+    0.8
+    0.8
+    ['7. Developing automated testing frameworks to validate the accuracy of large language models.\n8. Exploring ways to improve the scalability of large language models.\n9. Exploring ways to improve the efficiency of large language models.', '7. Applying methods such as active learning to further refine large language models.\n8. Developing and utilizing techniques such as knowledge distillation to compress large language models.\n9. Incorporating techniques such as semi-supervised', '7. Applying regularization techniques to reduce overfitting and improve generalization of large language models.\n8. Exploring the use of generative adversarial networks to improve the accuracy of large language models.\n9. Applying deep', '7. Developing methods to evaluate the performance of large language models on various tasks.\n8. Applying techniques such as hyperparameter tuning to optimize the performance of large language models.\n9. Utilizing adversarial training to', '7. Developing strategies to ensure large language models are able to generalize to unseen data.\n8. Incorporating methods such as meta-learning to further improve model performance.\n9. Utilizing techniques such as unsuper']
+    0.7
+    0.7
+    ['Once the key components of large language models have been identified and understood, the best reasoning methods to advance them include utilizing transfer learning to quickly train them, analyzing and interpreting them to identify areas of improvement, leveraging reinforcement learning to enable them to learn']
+    0.7
+    0.7
+    ['Exploring the use of meta-learning to enable models to rapidly adapt to new data and improve accuracy.']
+    0.7
+    0.7
+    ['One potential way to further advance large language models is to incorporate automated data augmentation techniques to create more varied datasets to train the models on, as well as leveraging reinforcement learning to enable the models to learn from mistakes and continually improve accuracy.']
+    0.7
+    0.7
+    ['By utilizing these methods, we can continue to advance large language models by improving their accuracy and performance. We can also use these methods to identify weaknesses in the models and make modifications to address them. Additionally, these methods can help us to develop']
+    0.7
+    0.7
+    
+    
+    """
+
```

### Comparing `tree-of-thoughts-0.1.6/tree_of_thoughts.egg-info/PKG-INFO` & `tree-of-thoughts-0.1.7/tree_of_thoughts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-of-thoughts
-Version: 0.1.6
+Version: 0.1.7
 Summary: Tree of Thoughts - Pytorch
 Home-page: https://github.com/kyegomez/tree-of-thoughts
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

