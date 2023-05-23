# Comparing `tmp/surv_ai-0.1.6.tar.gz` & `tmp/surv_ai-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "surv_ai-0.1.6.tar", max compression
+gzip compressed data, was "surv_ai-0.1.7.tar", max compression
```

## Comparing `surv_ai-0.1.6.tar` & `surv_ai-0.1.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1056 2023-05-19 03:25:36.438871 surv_ai-0.1.6/LICENSE
--rw-r--r--   0        0        0    21349 2023-05-23 12:53:10.344514 surv_ai-0.1.6/README.md
--rw-r--r--   0        0        0     1447 2023-05-23 12:53:49.203158 surv_ai-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1301 2023-05-22 19:00:12.464186 surv_ai-0.1.6/surv_ai/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 02:57:50.211881 surv_ai-0.1.6/surv_ai/core/__init__.py
--rw-r--r--   0        0        0     1667 2023-05-22 16:09:44.534005 surv_ai-0.1.6/surv_ai/core/agent.py
--rw-r--r--   0        0        0        0 2023-05-09 03:57:54.724106 surv_ai-0.1.6/surv_ai/core/agents/__init__.py
--rw-r--r--   0        0        0     1608 2023-05-22 15:04:42.549505 surv_ai-0.1.6/surv_ai/core/agents/binary.py
--rw-r--r--   0        0        0     6979 2023-05-22 15:18:19.376795 surv_ai-0.1.6/surv_ai/core/agents/reasoning.py
--rw-r--r--   0        0        0     1857 2023-05-22 19:00:12.464474 surv_ai-0.1.6/surv_ai/core/interfaces.py
--rw-r--r--   0        0        0     1279 2023-05-22 16:09:44.531688 surv_ai-0.1.6/surv_ai/core/model.py
--rw-r--r--   0        0        0     4722 2023-05-22 19:00:12.464239 surv_ai-0.1.6/surv_ai/core/survey.py
--rw-r--r--   0        0        0        0 2023-04-16 19:43:12.303158 surv_ai-0.1.6/surv_ai/lib/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 03:24:33.757534 surv_ai-0.1.6/surv_ai/lib/conversation/__init__.py
--rw-r--r--   0        0        0     1065 2023-05-22 15:04:42.565319 surv_ai-0.1.6/surv_ai/lib/conversation/conversation.py
--rw-r--r--   0        0        0      409 2023-05-21 02:50:40.891526 surv_ai-0.1.6/surv_ai/lib/conversation/interfaces.py
--rw-r--r--   0        0        0       53 2023-05-08 03:25:52.022148 surv_ai-0.1.6/surv_ai/lib/knowledge_store/__init__.py
--rw-r--r--   0        0        0      693 2023-05-22 15:04:42.556450 surv_ai-0.1.6/surv_ai/lib/knowledge_store/interfaces.py
--rw-r--r--   0        0        0     1486 2023-05-22 15:04:42.581390 surv_ai-0.1.6/surv_ai/lib/knowledge_store/local.py
--rw-r--r--   0        0        0        0 2023-04-16 19:53:58.086455 surv_ai-0.1.6/surv_ai/lib/llm/__init__.py
--rw-r--r--   0        0        0     3755 2023-05-22 16:07:39.753305 surv_ai-0.1.6/surv_ai/lib/llm/anthropic.py
--rw-r--r--   0        0        0     4261 2023-05-22 16:07:57.537852 surv_ai-0.1.6/surv_ai/lib/llm/gpt.py
--rw-r--r--   0        0        0      432 2023-05-22 15:04:42.564655 surv_ai-0.1.6/surv_ai/lib/llm/interfaces.py
--rw-r--r--   0        0        0     2005 2023-05-23 04:29:11.574974 surv_ai-0.1.6/surv_ai/lib/log.py
--rw-r--r--   0        0        0        0 2023-04-16 23:16:14.406022 surv_ai-0.1.6/surv_ai/lib/tools/__init__.py
--rw-r--r--   0        0        0      656 2023-05-22 19:00:03.447356 surv_ai-0.1.6/surv_ai/lib/tools/interfaces.py
--rw-r--r--   0        0        0        0 2023-04-16 23:16:30.843990 surv_ai-0.1.6/surv_ai/lib/tools/query/__init__.py
--rw-r--r--   0        0        0     7047 2023-05-22 16:09:44.603986 surv_ai-0.1.6/surv_ai/lib/tools/query/google_custom_search.py
--rw-r--r--   0        0        0      219 2023-05-19 05:42:04.105413 surv_ai-0.1.6/surv_ai/lib/tools/query/interfaces.py
--rw-r--r--   0        0        0     5918 2023-05-22 16:09:44.606441 surv_ai-0.1.6/surv_ai/lib/tools/query/wikipedia.py
--rw-r--r--   0        0        0     2924 2023-05-22 19:00:12.464217 surv_ai-0.1.6/surv_ai/lib/tools/tool_belt.py
--rw-r--r--   0        0        0    22699 1970-01-01 00:00:00.000000 surv_ai-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-05-19 03:25:36.438871 surv_ai-0.1.7/LICENSE
+-rw-r--r--   0        0        0    21369 2023-05-23 13:32:11.427446 surv_ai-0.1.7/README.md
+-rw-r--r--   0        0        0     1447 2023-05-23 13:32:23.220510 surv_ai-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1301 2023-05-22 19:00:12.464186 surv_ai-0.1.7/surv_ai/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 02:57:50.211881 surv_ai-0.1.7/surv_ai/core/__init__.py
+-rw-r--r--   0        0        0     1667 2023-05-22 16:09:44.534005 surv_ai-0.1.7/surv_ai/core/agent.py
+-rw-r--r--   0        0        0        0 2023-05-09 03:57:54.724106 surv_ai-0.1.7/surv_ai/core/agents/__init__.py
+-rw-r--r--   0        0        0     1608 2023-05-22 15:04:42.549505 surv_ai-0.1.7/surv_ai/core/agents/binary.py
+-rw-r--r--   0        0        0     6979 2023-05-22 15:18:19.376795 surv_ai-0.1.7/surv_ai/core/agents/reasoning.py
+-rw-r--r--   0        0        0     1857 2023-05-22 19:00:12.464474 surv_ai-0.1.7/surv_ai/core/interfaces.py
+-rw-r--r--   0        0        0     1279 2023-05-22 16:09:44.531688 surv_ai-0.1.7/surv_ai/core/model.py
+-rw-r--r--   0        0        0     4723 2023-05-23 12:58:41.819687 surv_ai-0.1.7/surv_ai/core/survey.py
+-rw-r--r--   0        0        0        0 2023-04-16 19:43:12.303158 surv_ai-0.1.7/surv_ai/lib/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 03:24:33.757534 surv_ai-0.1.7/surv_ai/lib/conversation/__init__.py
+-rw-r--r--   0        0        0     1065 2023-05-22 15:04:42.565319 surv_ai-0.1.7/surv_ai/lib/conversation/conversation.py
+-rw-r--r--   0        0        0      409 2023-05-21 02:50:40.891526 surv_ai-0.1.7/surv_ai/lib/conversation/interfaces.py
+-rw-r--r--   0        0        0       53 2023-05-08 03:25:52.022148 surv_ai-0.1.7/surv_ai/lib/knowledge_store/__init__.py
+-rw-r--r--   0        0        0      693 2023-05-22 15:04:42.556450 surv_ai-0.1.7/surv_ai/lib/knowledge_store/interfaces.py
+-rw-r--r--   0        0        0     1486 2023-05-22 15:04:42.581390 surv_ai-0.1.7/surv_ai/lib/knowledge_store/local.py
+-rw-r--r--   0        0        0        0 2023-04-16 19:53:58.086455 surv_ai-0.1.7/surv_ai/lib/llm/__init__.py
+-rw-r--r--   0        0        0     3755 2023-05-22 16:07:39.753305 surv_ai-0.1.7/surv_ai/lib/llm/anthropic.py
+-rw-r--r--   0        0        0     4261 2023-05-22 16:07:57.537852 surv_ai-0.1.7/surv_ai/lib/llm/gpt.py
+-rw-r--r--   0        0        0      432 2023-05-22 15:04:42.564655 surv_ai-0.1.7/surv_ai/lib/llm/interfaces.py
+-rw-r--r--   0        0        0     2005 2023-05-23 04:29:11.574974 surv_ai-0.1.7/surv_ai/lib/log.py
+-rw-r--r--   0        0        0        0 2023-04-16 23:16:14.406022 surv_ai-0.1.7/surv_ai/lib/tools/__init__.py
+-rw-r--r--   0        0        0      656 2023-05-22 19:00:03.447356 surv_ai-0.1.7/surv_ai/lib/tools/interfaces.py
+-rw-r--r--   0        0        0        0 2023-04-16 23:16:30.843990 surv_ai-0.1.7/surv_ai/lib/tools/query/__init__.py
+-rw-r--r--   0        0        0     7047 2023-05-22 16:09:44.603986 surv_ai-0.1.7/surv_ai/lib/tools/query/google_custom_search.py
+-rw-r--r--   0        0        0      219 2023-05-19 05:42:04.105413 surv_ai-0.1.7/surv_ai/lib/tools/query/interfaces.py
+-rw-r--r--   0        0        0     5918 2023-05-22 16:09:44.606441 surv_ai-0.1.7/surv_ai/lib/tools/query/wikipedia.py
+-rw-r--r--   0        0        0     2924 2023-05-22 19:00:12.464217 surv_ai-0.1.7/surv_ai/lib/tools/tool_belt.py
+-rw-r--r--   0        0        0    22719 1970-01-01 00:00:00.000000 surv_ai-0.1.7/PKG-INFO
```

### Comparing `surv_ai-0.1.6/LICENSE` & `surv_ai-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.6/README.md` & `surv_ai-0.1.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # 🕵 Multi-agent modeling with large language models 
 <!-- [![PyPi](https://img.shields.io/badge/Official%20Website-agpt.co-blue?style=flat&logo=world&logoColor=white)](https://agpt.co) -->
 [![PyPi](https://shields.io/pypi/v/surv-ai)](https://pypi.org/project/surv-ai/)
-[![PyPi](https://shields.io/pyversions/surv-ai)](https://pypi.org/project/surv-ai/)
+[![PyPi](https://shields.io/pypi/pyversions/surv-ai)](https://pypi.org/project/surv-ai/)
 [![Unit Tests](https://shields.io/github/actions/workflow/status/DanielBalsam/surv_ai/.github/workflows/ci.yaml?branch=main)](https://github.com/DanielBalsam/surv_ai/actions/workflows/ci.yaml)
 [![GitHub Repo stars](https://img.shields.io/github/stars/DanielBalsam/surv_ai?style=social)](https://github.com/DanielBalsam/surv_ai/stargazers)
 
 
 **`surv_ai` is a large language model framework designed for multi-agent modeling. This allows large-language models to be used as engines to power research into predictive modeling, bias analysis, and other forms of comparative analysis.**
 
 ![](https://raw.githubusercontent.com/DanielBalsam/surv_ai/main/examples/midterms_2022.png)
 
 **Multi-agent modeling** involves generating statistical models based on the actions of multiple agents. In our case, these models are crafted by agents querying and processing text from a comprehensive data corpus. The agents then reason with the information extracted to produce a data point.
 
 Given the stochastic nature of large language models, individual data points may vary. However, if a sufficient number of agents are employed, the generated models can effectively support comparative analysis.
 
 They key idea here was inspired by the [technique of bagging (bootstrap aggregating) in classical ensemble classifiers.](https://en.wikipedia.org/wiki/Bootstrap_aggregating) The basic idea is that if you have a lot of weak learners with only limited information - in aggregate those weak learners can produce much higher quality results than a single weak learner with maximum information (or a bunch a weak learners with maximum information).
 
-This technique appears to work better when each agent has access to a very limited subset information even when using language models with larger context windows.
+This technique appears to work better when each agent has access to a limited subset of the total information even when using language models with larger context windows.
 
 The abstraction in this repository capable of producing a multi-agent data point is known as a `Survey`. A `Survey` takes a statement as input and returns the percentage of agents that agreed with it.
 
 A more complex abstraction, called a `Model`, enables the variation of input parameters into a `Survey` to create a nuanced multi-agent model.
 
 The data points produced serve as sentiment analysis against a text corpus, making them susceptible to the biases of both the large language models and the corpus itself. However, if the data source provided is quality - then the model produced can be high quality as well.
 
@@ -56,15 +56,15 @@
 class Survey:
     def __init__(
         self,
         client: LargeLanguageModelClientInterface,
         tool_belt: ToolBeltInterface,
         n_agents=10,
         max_concurrency=10,
-        max_knowledge_per_agent=5,
+        max_knowledge_per_agent=10,
     ):
         ...
 
     async def conduct(self, hypothesis: str) -> SurveyResponse:
         ...
 ```
 
@@ -100,15 +100,15 @@
 
 Let's start by establishing the system's ability to figure out if information is true.
 
 ```
 from surv_ai import (
     GPTClient,
     Survey,
-    ToolBelt,
+    ToolBelt,x
     GoogleCustomSearchTool,
     Knowledge
 )
 
 client = GPTClient(os.environ["OPEN_AI_API_KEY"])
 
 survey = Survey(
@@ -122,15 +122,14 @@
                 os.environ["GOOGLE_SEARCH_ENGINE_ID"],
                 start_date="2023-01-01",
                 end_date="2023-05-01",
                 n_pages=10,
             )
         ]
     ),
-    max_knowledge_per_agent=3,
     n_agents=10,
     base_knowledge=[
         Knowledge(
             text="It is currently 2023/05/01, all the articles are from 2023.",
             source="Additional context",
         ),
     ],
@@ -220,15 +219,14 @@
 model = Model(
     Survey,
     parameters=[
         SurveyParameter(
             independent_variable=range[1],
             parameters={
                 "n_agents": 100,
-                "max_knowledge_per_agent": 1,
                 "max_concurrency": 10,
                 "tool_belt": ToolBelt(
                     client,
                     [
                         GoogleCustomSearchTool(
                             client,
                             os.environ["GOOGLE_API_KEY"],
@@ -255,15 +253,16 @@
     "Democrats are favored to maintain control of the Senate in the 2022 November Midterm elections.",
 )
 ```
 
 When compared with a leading model in political opinion polling, our model is presented as follows:
 
 ![](https://raw.githubusercontent.com/DanielBalsam/surv_ai/main/examples/midterms_2022.png)
-*In this example, the agents crawled websites such as nytimes.com, wsj.com, abcnews.com, cnn.com, bloomberg.com, foxnews.com, economist.com, washingtonpost.com, and nbcnews.com.*
+
+*In this example, the agents crawled websites such as nytimes.com, wsj.com, abcnews.com, cnn.com, bloomberg.com, foxnews.com, economist.com, washingtonpost.com, and nbcnews.com. [FiveThirtyEight data can be found here.](https://projects.fivethirtyeight.com/2022-election-forecast/senate/)*
 
 Pretty cool! Another example could involve plotting sentiments about the economy and using fluctuations in the yield curve as a benchmark for accuracy.
 
 ```
 from surv_ai import (
     GPTClient,
     Model,
@@ -288,15 +287,14 @@
 model = Model(
     Survey,
     parameters=[
         SurveyParameter(
             independent_variable=range[1],
             parameters={
                 "n_agents": 100,
-                "max_knowledge_per_agent": 1,
                 "max_concurrency": 5,
                 "tool_belt": ToolBelt(
                     client,
                     [
                         GoogleCustomSearchTool(
                             client,
                             os.environ["GOOGLE_API_KEY"],
@@ -323,15 +321,16 @@
     "The United States economy looks like it is heading for a recession.",
 )
 ```
 
 This gives us the following graph:
 
 ![](https://raw.githubusercontent.com/DanielBalsam/surv_ai/main/examples/yield_spread.png)
-*In this example, the agents crawled websites such as nytimes.com, wsj.com, abcnews.com, cnn.com, bloomberg.com, foxnews.com, economist.com, washingtonpost.com, and nbcnews.com. Please note that it is the complement of multi-agent model that is plotted.*
+
+*In this example, the agents crawled websites such as nytimes.com, wsj.com, abcnews.com, cnn.com, bloomberg.com, foxnews.com, economist.com, washingtonpost.com, and nbcnews.com. Please note that it is the complement of multi-agent model that is plotted. [Yield spread data can be found here.](https://www.longtermtrends.net/us-treasury-yield-curve/)*
 
 ### Measuring bias in a data corpus
 
 A promising application of this technique is observing bias within a text corpus. For instance, we could create a model that uses different news sites as its independent variable to explore how the agents' conclusions might vary based on the data source utilized.
 
 ```
 from surv_ai import (
@@ -369,15 +368,14 @@
                             start_date="2023-05-01",
                             end_date="2023-06-01",
                             only_include_sources=[source]
                         )
                     ]
                 ),
                 "n_agents": 100,
-                "max_knowledge_per_agent": 3,
                 "base_knowledge": [
                     Knowledge(
                         text=f"It is currently 2023-06-01. The included articles were published between 2023-05-01 and 2023-06-01",
                         source="Additional context",
                     ),
                 ],
             }
@@ -389,14 +387,15 @@
     "Republicans are responsible for the impending debt ceiling crisis."
 )
 ```
 
 This provides us with a scatter plot representing the above-mentioned news sources:
 
 ![](https://raw.githubusercontent.com/DanielBalsam/surv_ai/main/examples/debt_ceiling.png)
+
 *In this example, for each news site the agents looked only at articles published in May of 2023. Omitted publications did not have enough articles on the topic published to get reliable results.*
 
 ### Measuring biases in different large language models
 
 Another promising method for measuring bias involves comparing biases across various large language models, provided they all receive identical input parameters.
 
 ```
@@ -432,15 +431,14 @@
                             end_date="2023-06-01",
                             max_concurrency=3,
                         )
                     ]
                 ),
                 "n_agents": 100,
                 "max_concurrency": 3,
-                "max_knowledge_per_agent": 3,
                 "base_knowledge": [
                     Knowledge(
                         text=f"It is currently 2023-06-01. The included articles were published between 2023-01-01 and 2023-06-01",
                         source="Additional context",
                     ),
                 ],
             }
@@ -452,14 +450,15 @@
     "OpenAI has been irresponsible in their handling of AI technology."
 )
 ```
 
 When we compare this statement between Anthropic and OpenAI's models, the resulting scatter plot appears as follows:
 
 ![](https://raw.githubusercontent.com/DanielBalsam/surv_ai/main/examples/openai.png)
+
 *In this example, the agents crawled websites such as nytimes.com, wsj.com, abcnews.com, cnn.com, bloomberg.com, foxnews.com, economist.com, washingtonpost.com, and nbcnews.com for articles published in the first half of 2023.*
 
 
 ## 🧠 Tips 
 
 Ultimately, a `Survey` is powered by a Large Language Model (LLM), which means that the survey hypothesis might require tuning, much like the general need to tune prompts. Here are some insights on crafting hypotheses.
 
@@ -489,15 +488,14 @@
                 os.environ["GOOGLE_SEARCH_ENGINE_ID"],
                 start_date="2023-01-01",
                 end_date="2023-05-01",
                 n_pages=10,
             )
         ]
     ),
-    max_knowledge_per_agent=3,
     n_agents=10,
     base_knowledge=[
         Knowledge(
             text="It is currently 2023/05/01, all the articles are from 2023.",
             source="Additional context",
         ),
     ],
@@ -557,13 +555,14 @@
 ## 📈 Next steps 
 
 A few directions I plan to explore with this project include:
 
 1. I'm considering transitioning the core Large Language Model (LLM) interaction code to take advantage of Microsoft's Guidance framework.
 2. I aim to further refine the agent code to improve decision-making across a wide variety of problems. I'm particularly interested in exploring Tree of Thought Prompting to see the outcomes it generates.
 3. I plan to incorporate clients with more instruction-tuned and reinforcement-learned LLMs.
-4. One feature that would be exciting would be the ability to easily fit a machine learning model against a multi-agent model. This could allow projection of the multi-agent models.
+4. One feature that would be exciting would be the ability to easily fit a machine learning model against a multi-agent model. This could allow projection with the multi-agent models.
+5. More documentation and use guides!
 
 
 ## 🤝 Contribute 
 
 If you'd like to contribute then please reach out!
```

### Comparing `surv_ai-0.1.6/pyproject.toml` & `surv_ai-0.1.7/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "surv_ai"
-version = "0.1.6"
+version = "0.1.7"
 description = "A framework for multi-agent modeling using large language models"
 authors = ["Daniel Balsam <daniel.balsam@survai.org>"]
 license = "MIT"
 readme = "README.md"
 keywords=[
     "ai",
     "artificial intelligence",
```

### Comparing `surv_ai-0.1.6/surv_ai/__init__.py` & `surv_ai-0.1.7/surv_ai/__init__.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.6/surv_ai/core/agent.py` & `surv_ai-0.1.7/surv_ai/core/agent.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.6/surv_ai/core/agents/binary.py` & `surv_ai-0.1.7/surv_ai/core/agents/binary.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.6/surv_ai/core/agents/reasoning.py` & `surv_ai-0.1.7/surv_ai/core/agents/reasoning.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.6/surv_ai/core/interfaces.py` & `surv_ai-0.1.7/surv_ai/core/interfaces.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.6/surv_ai/core/model.py` & `surv_ai-0.1.7/surv_ai/core/model.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.6/surv_ai/core/survey.py` & `surv_ai-0.1.7/surv_ai/core/survey.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 class Survey(SurveyInterface):
     def __init__(
         self,
         client: LargeLanguageModelClientInterface,
         tool_belt: ToolBeltInterface,
         n_agents=10,
         max_concurrency=10,
-        max_knowledge_per_agent=5,
+        max_knowledge_per_agent=10,
         base_knowledge: Optional[list[Knowledge]] = None,
     ):
         self.client = client
         self.tool_belt = tool_belt
 
         self.n_agents = n_agents
         self.max_concurrency = max_concurrency
```

### Comparing `surv_ai-0.1.6/surv_ai/lib/conversation/conversation.py` & `surv_ai-0.1.7/surv_ai/lib/conversation/conversation.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.6/surv_ai/lib/knowledge_store/interfaces.py` & `surv_ai-0.1.7/surv_ai/lib/knowledge_store/interfaces.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.6/surv_ai/lib/knowledge_store/local.py` & `surv_ai-0.1.7/surv_ai/lib/knowledge_store/local.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.6/surv_ai/lib/llm/anthropic.py` & `surv_ai-0.1.7/surv_ai/lib/llm/anthropic.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.6/surv_ai/lib/llm/gpt.py` & `surv_ai-0.1.7/surv_ai/lib/llm/gpt.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.6/surv_ai/lib/log.py` & `surv_ai-0.1.7/surv_ai/lib/log.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.6/surv_ai/lib/tools/interfaces.py` & `surv_ai-0.1.7/surv_ai/lib/tools/interfaces.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.6/surv_ai/lib/tools/query/google_custom_search.py` & `surv_ai-0.1.7/surv_ai/lib/tools/query/google_custom_search.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.6/surv_ai/lib/tools/query/wikipedia.py` & `surv_ai-0.1.7/surv_ai/lib/tools/query/wikipedia.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.6/surv_ai/lib/tools/tool_belt.py` & `surv_ai-0.1.7/surv_ai/lib/tools/tool_belt.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.6/PKG-INFO` & `surv_ai-0.1.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surv-ai
-Version: 0.1.6
+Version: 0.1.7
 Summary: A framework for multi-agent modeling using large language models
 Home-page: https://github.com/DanielBalsam/surv_ai
 License: MIT
 Keywords: ai,artificial intelligence,data science,statistics,models,llm,agents,survai,surv_ai,survey,multi-agent,large language model,artificial intelligence,machine learning,natural language processing,nlp,sentiment analysis
 Author: Daniel Balsam
 Author-email: daniel.balsam@survai.org
 Requires-Python: >=3.9,<4.0
@@ -25,30 +25,30 @@
 Project-URL: Documentation, https://github.com/DanielBalsam/surv_ai/blob/main/README.md
 Project-URL: Repository, https://github.com/DanielBalsam/surv_ai
 Description-Content-Type: text/markdown
 
 # 🕵 Multi-agent modeling with large language models 
 <!-- [![PyPi](https://img.shields.io/badge/Official%20Website-agpt.co-blue?style=flat&logo=world&logoColor=white)](https://agpt.co) -->
 [![PyPi](https://shields.io/pypi/v/surv-ai)](https://pypi.org/project/surv-ai/)
-[![PyPi](https://shields.io/pyversions/surv-ai)](https://pypi.org/project/surv-ai/)
+[![PyPi](https://shields.io/pypi/pyversions/surv-ai)](https://pypi.org/project/surv-ai/)
 [![Unit Tests](https://shields.io/github/actions/workflow/status/DanielBalsam/surv_ai/.github/workflows/ci.yaml?branch=main)](https://github.com/DanielBalsam/surv_ai/actions/workflows/ci.yaml)
 [![GitHub Repo stars](https://img.shields.io/github/stars/DanielBalsam/surv_ai?style=social)](https://github.com/DanielBalsam/surv_ai/stargazers)
 
 
 **`surv_ai` is a large language model framework designed for multi-agent modeling. This allows large-language models to be used as engines to power research into predictive modeling, bias analysis, and other forms of comparative analysis.**
 
 ![](https://raw.githubusercontent.com/DanielBalsam/surv_ai/main/examples/midterms_2022.png)
 
 **Multi-agent modeling** involves generating statistical models based on the actions of multiple agents. In our case, these models are crafted by agents querying and processing text from a comprehensive data corpus. The agents then reason with the information extracted to produce a data point.
 
 Given the stochastic nature of large language models, individual data points may vary. However, if a sufficient number of agents are employed, the generated models can effectively support comparative analysis.
 
 They key idea here was inspired by the [technique of bagging (bootstrap aggregating) in classical ensemble classifiers.](https://en.wikipedia.org/wiki/Bootstrap_aggregating) The basic idea is that if you have a lot of weak learners with only limited information - in aggregate those weak learners can produce much higher quality results than a single weak learner with maximum information (or a bunch a weak learners with maximum information).
 
-This technique appears to work better when each agent has access to a very limited subset information even when using language models with larger context windows.
+This technique appears to work better when each agent has access to a limited subset of the total information even when using language models with larger context windows.
 
 The abstraction in this repository capable of producing a multi-agent data point is known as a `Survey`. A `Survey` takes a statement as input and returns the percentage of agents that agreed with it.
 
 A more complex abstraction, called a `Model`, enables the variation of input parameters into a `Survey` to create a nuanced multi-agent model.
 
 The data points produced serve as sentiment analysis against a text corpus, making them susceptible to the biases of both the large language models and the corpus itself. However, if the data source provided is quality - then the model produced can be high quality as well.
 
@@ -84,15 +84,15 @@
 class Survey:
     def __init__(
         self,
         client: LargeLanguageModelClientInterface,
         tool_belt: ToolBeltInterface,
         n_agents=10,
         max_concurrency=10,
-        max_knowledge_per_agent=5,
+        max_knowledge_per_agent=10,
     ):
         ...
 
     async def conduct(self, hypothesis: str) -> SurveyResponse:
         ...
 ```
 
@@ -128,15 +128,15 @@
 
 Let's start by establishing the system's ability to figure out if information is true.
 
 ```
 from surv_ai import (
     GPTClient,
     Survey,
-    ToolBelt,
+    ToolBelt,x
     GoogleCustomSearchTool,
     Knowledge
 )
 
 client = GPTClient(os.environ["OPEN_AI_API_KEY"])
 
 survey = Survey(
@@ -150,15 +150,14 @@
                 os.environ["GOOGLE_SEARCH_ENGINE_ID"],
                 start_date="2023-01-01",
                 end_date="2023-05-01",
                 n_pages=10,
             )
         ]
     ),
-    max_knowledge_per_agent=3,
     n_agents=10,
     base_knowledge=[
         Knowledge(
             text="It is currently 2023/05/01, all the articles are from 2023.",
             source="Additional context",
         ),
     ],
@@ -248,15 +247,14 @@
 model = Model(
     Survey,
     parameters=[
         SurveyParameter(
             independent_variable=range[1],
             parameters={
                 "n_agents": 100,
-                "max_knowledge_per_agent": 1,
                 "max_concurrency": 10,
                 "tool_belt": ToolBelt(
                     client,
                     [
                         GoogleCustomSearchTool(
                             client,
                             os.environ["GOOGLE_API_KEY"],
@@ -283,15 +281,16 @@
     "Democrats are favored to maintain control of the Senate in the 2022 November Midterm elections.",
 )
 ```
 
 When compared with a leading model in political opinion polling, our model is presented as follows:
 
 ![](https://raw.githubusercontent.com/DanielBalsam/surv_ai/main/examples/midterms_2022.png)
-*In this example, the agents crawled websites such as nytimes.com, wsj.com, abcnews.com, cnn.com, bloomberg.com, foxnews.com, economist.com, washingtonpost.com, and nbcnews.com.*
+
+*In this example, the agents crawled websites such as nytimes.com, wsj.com, abcnews.com, cnn.com, bloomberg.com, foxnews.com, economist.com, washingtonpost.com, and nbcnews.com. [FiveThirtyEight data can be found here.](https://projects.fivethirtyeight.com/2022-election-forecast/senate/)*
 
 Pretty cool! Another example could involve plotting sentiments about the economy and using fluctuations in the yield curve as a benchmark for accuracy.
 
 ```
 from surv_ai import (
     GPTClient,
     Model,
@@ -316,15 +315,14 @@
 model = Model(
     Survey,
     parameters=[
         SurveyParameter(
             independent_variable=range[1],
             parameters={
                 "n_agents": 100,
-                "max_knowledge_per_agent": 1,
                 "max_concurrency": 5,
                 "tool_belt": ToolBelt(
                     client,
                     [
                         GoogleCustomSearchTool(
                             client,
                             os.environ["GOOGLE_API_KEY"],
@@ -351,15 +349,16 @@
     "The United States economy looks like it is heading for a recession.",
 )
 ```
 
 This gives us the following graph:
 
 ![](https://raw.githubusercontent.com/DanielBalsam/surv_ai/main/examples/yield_spread.png)
-*In this example, the agents crawled websites such as nytimes.com, wsj.com, abcnews.com, cnn.com, bloomberg.com, foxnews.com, economist.com, washingtonpost.com, and nbcnews.com. Please note that it is the complement of multi-agent model that is plotted.*
+
+*In this example, the agents crawled websites such as nytimes.com, wsj.com, abcnews.com, cnn.com, bloomberg.com, foxnews.com, economist.com, washingtonpost.com, and nbcnews.com. Please note that it is the complement of multi-agent model that is plotted. [Yield spread data can be found here.](https://www.longtermtrends.net/us-treasury-yield-curve/)*
 
 ### Measuring bias in a data corpus
 
 A promising application of this technique is observing bias within a text corpus. For instance, we could create a model that uses different news sites as its independent variable to explore how the agents' conclusions might vary based on the data source utilized.
 
 ```
 from surv_ai import (
@@ -397,15 +396,14 @@
                             start_date="2023-05-01",
                             end_date="2023-06-01",
                             only_include_sources=[source]
                         )
                     ]
                 ),
                 "n_agents": 100,
-                "max_knowledge_per_agent": 3,
                 "base_knowledge": [
                     Knowledge(
                         text=f"It is currently 2023-06-01. The included articles were published between 2023-05-01 and 2023-06-01",
                         source="Additional context",
                     ),
                 ],
             }
@@ -417,14 +415,15 @@
     "Republicans are responsible for the impending debt ceiling crisis."
 )
 ```
 
 This provides us with a scatter plot representing the above-mentioned news sources:
 
 ![](https://raw.githubusercontent.com/DanielBalsam/surv_ai/main/examples/debt_ceiling.png)
+
 *In this example, for each news site the agents looked only at articles published in May of 2023. Omitted publications did not have enough articles on the topic published to get reliable results.*
 
 ### Measuring biases in different large language models
 
 Another promising method for measuring bias involves comparing biases across various large language models, provided they all receive identical input parameters.
 
 ```
@@ -460,15 +459,14 @@
                             end_date="2023-06-01",
                             max_concurrency=3,
                         )
                     ]
                 ),
                 "n_agents": 100,
                 "max_concurrency": 3,
-                "max_knowledge_per_agent": 3,
                 "base_knowledge": [
                     Knowledge(
                         text=f"It is currently 2023-06-01. The included articles were published between 2023-01-01 and 2023-06-01",
                         source="Additional context",
                     ),
                 ],
             }
@@ -480,14 +478,15 @@
     "OpenAI has been irresponsible in their handling of AI technology."
 )
 ```
 
 When we compare this statement between Anthropic and OpenAI's models, the resulting scatter plot appears as follows:
 
 ![](https://raw.githubusercontent.com/DanielBalsam/surv_ai/main/examples/openai.png)
+
 *In this example, the agents crawled websites such as nytimes.com, wsj.com, abcnews.com, cnn.com, bloomberg.com, foxnews.com, economist.com, washingtonpost.com, and nbcnews.com for articles published in the first half of 2023.*
 
 
 ## 🧠 Tips 
 
 Ultimately, a `Survey` is powered by a Large Language Model (LLM), which means that the survey hypothesis might require tuning, much like the general need to tune prompts. Here are some insights on crafting hypotheses.
 
@@ -517,15 +516,14 @@
                 os.environ["GOOGLE_SEARCH_ENGINE_ID"],
                 start_date="2023-01-01",
                 end_date="2023-05-01",
                 n_pages=10,
             )
         ]
     ),
-    max_knowledge_per_agent=3,
     n_agents=10,
     base_knowledge=[
         Knowledge(
             text="It is currently 2023/05/01, all the articles are from 2023.",
             source="Additional context",
         ),
     ],
@@ -585,14 +583,15 @@
 ## 📈 Next steps 
 
 A few directions I plan to explore with this project include:
 
 1. I'm considering transitioning the core Large Language Model (LLM) interaction code to take advantage of Microsoft's Guidance framework.
 2. I aim to further refine the agent code to improve decision-making across a wide variety of problems. I'm particularly interested in exploring Tree of Thought Prompting to see the outcomes it generates.
 3. I plan to incorporate clients with more instruction-tuned and reinforcement-learned LLMs.
-4. One feature that would be exciting would be the ability to easily fit a machine learning model against a multi-agent model. This could allow projection of the multi-agent models.
+4. One feature that would be exciting would be the ability to easily fit a machine learning model against a multi-agent model. This could allow projection with the multi-agent models.
+5. More documentation and use guides!
 
 
 ## 🤝 Contribute 
 
 If you'd like to contribute then please reach out!
```

