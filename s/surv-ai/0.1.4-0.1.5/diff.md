# Comparing `tmp/surv_ai-0.1.4.tar.gz` & `tmp/surv_ai-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "surv_ai-0.1.4.tar", max compression
+gzip compressed data, was "surv_ai-0.1.5.tar", max compression
```

## Comparing `surv_ai-0.1.4.tar` & `surv_ai-0.1.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1056 2023-05-19 03:25:36.438871 surv_ai-0.1.4/LICENSE
--rw-r--r--   0        0        0    19579 2023-05-22 19:03:29.144408 surv_ai-0.1.4/README.md
--rw-r--r--   0        0        0     1447 2023-05-22 19:06:24.713187 surv_ai-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1301 2023-05-22 19:00:12.464186 surv_ai-0.1.4/surv_ai/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 02:57:50.211881 surv_ai-0.1.4/surv_ai/core/__init__.py
--rw-r--r--   0        0        0     1667 2023-05-22 16:09:44.534005 surv_ai-0.1.4/surv_ai/core/agent.py
--rw-r--r--   0        0        0        0 2023-05-09 03:57:54.724106 surv_ai-0.1.4/surv_ai/core/agents/__init__.py
--rw-r--r--   0        0        0     1608 2023-05-22 15:04:42.549505 surv_ai-0.1.4/surv_ai/core/agents/binary.py
--rw-r--r--   0        0        0     6979 2023-05-22 15:18:19.376795 surv_ai-0.1.4/surv_ai/core/agents/reasoning.py
--rw-r--r--   0        0        0     1857 2023-05-22 19:00:12.464474 surv_ai-0.1.4/surv_ai/core/interfaces.py
--rw-r--r--   0        0        0     1279 2023-05-22 16:09:44.531688 surv_ai-0.1.4/surv_ai/core/model.py
--rw-r--r--   0        0        0     4722 2023-05-22 19:00:12.464239 surv_ai-0.1.4/surv_ai/core/survey.py
--rw-r--r--   0        0        0        0 2023-04-16 19:43:12.303158 surv_ai-0.1.4/surv_ai/lib/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 03:24:33.757534 surv_ai-0.1.4/surv_ai/lib/conversation/__init__.py
--rw-r--r--   0        0        0     1065 2023-05-22 15:04:42.565319 surv_ai-0.1.4/surv_ai/lib/conversation/conversation.py
--rw-r--r--   0        0        0      409 2023-05-21 02:50:40.891526 surv_ai-0.1.4/surv_ai/lib/conversation/interfaces.py
--rw-r--r--   0        0        0       53 2023-05-08 03:25:52.022148 surv_ai-0.1.4/surv_ai/lib/knowledge_store/__init__.py
--rw-r--r--   0        0        0      693 2023-05-22 15:04:42.556450 surv_ai-0.1.4/surv_ai/lib/knowledge_store/interfaces.py
--rw-r--r--   0        0        0     1486 2023-05-22 15:04:42.581390 surv_ai-0.1.4/surv_ai/lib/knowledge_store/local.py
--rw-r--r--   0        0        0        0 2023-04-16 19:53:58.086455 surv_ai-0.1.4/surv_ai/lib/llm/__init__.py
--rw-r--r--   0        0        0     3755 2023-05-22 16:07:39.753305 surv_ai-0.1.4/surv_ai/lib/llm/anthropic.py
--rw-r--r--   0        0        0     4261 2023-05-22 16:07:57.537852 surv_ai-0.1.4/surv_ai/lib/llm/gpt.py
--rw-r--r--   0        0        0      432 2023-05-22 15:04:42.564655 surv_ai-0.1.4/surv_ai/lib/llm/interfaces.py
--rw-r--r--   0        0        0     1960 2023-05-22 15:04:42.613196 surv_ai-0.1.4/surv_ai/lib/log.py
--rw-r--r--   0        0        0        0 2023-04-16 23:16:14.406022 surv_ai-0.1.4/surv_ai/lib/tools/__init__.py
--rw-r--r--   0        0        0      656 2023-05-22 19:00:03.447356 surv_ai-0.1.4/surv_ai/lib/tools/interfaces.py
--rw-r--r--   0        0        0        0 2023-04-16 23:16:30.843990 surv_ai-0.1.4/surv_ai/lib/tools/query/__init__.py
--rw-r--r--   0        0        0     7047 2023-05-22 16:09:44.603986 surv_ai-0.1.4/surv_ai/lib/tools/query/google_custom_search.py
--rw-r--r--   0        0        0      219 2023-05-19 05:42:04.105413 surv_ai-0.1.4/surv_ai/lib/tools/query/interfaces.py
--rw-r--r--   0        0        0     5918 2023-05-22 16:09:44.606441 surv_ai-0.1.4/surv_ai/lib/tools/query/wikipedia.py
--rw-r--r--   0        0        0     2924 2023-05-22 19:00:12.464217 surv_ai-0.1.4/surv_ai/lib/tools/tool_belt.py
--rw-r--r--   0        0        0    20929 1970-01-01 00:00:00.000000 surv_ai-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-05-19 03:25:36.438871 surv_ai-0.1.5/LICENSE
+-rw-r--r--   0        0        0    19688 2023-05-22 19:30:25.960802 surv_ai-0.1.5/README.md
+-rw-r--r--   0        0        0     1447 2023-05-22 19:34:53.895143 surv_ai-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1301 2023-05-22 19:00:12.464186 surv_ai-0.1.5/surv_ai/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 02:57:50.211881 surv_ai-0.1.5/surv_ai/core/__init__.py
+-rw-r--r--   0        0        0     1667 2023-05-22 16:09:44.534005 surv_ai-0.1.5/surv_ai/core/agent.py
+-rw-r--r--   0        0        0        0 2023-05-09 03:57:54.724106 surv_ai-0.1.5/surv_ai/core/agents/__init__.py
+-rw-r--r--   0        0        0     1608 2023-05-22 15:04:42.549505 surv_ai-0.1.5/surv_ai/core/agents/binary.py
+-rw-r--r--   0        0        0     6979 2023-05-22 15:18:19.376795 surv_ai-0.1.5/surv_ai/core/agents/reasoning.py
+-rw-r--r--   0        0        0     1857 2023-05-22 19:00:12.464474 surv_ai-0.1.5/surv_ai/core/interfaces.py
+-rw-r--r--   0        0        0     1279 2023-05-22 16:09:44.531688 surv_ai-0.1.5/surv_ai/core/model.py
+-rw-r--r--   0        0        0     4722 2023-05-22 19:00:12.464239 surv_ai-0.1.5/surv_ai/core/survey.py
+-rw-r--r--   0        0        0        0 2023-04-16 19:43:12.303158 surv_ai-0.1.5/surv_ai/lib/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 03:24:33.757534 surv_ai-0.1.5/surv_ai/lib/conversation/__init__.py
+-rw-r--r--   0        0        0     1065 2023-05-22 15:04:42.565319 surv_ai-0.1.5/surv_ai/lib/conversation/conversation.py
+-rw-r--r--   0        0        0      409 2023-05-21 02:50:40.891526 surv_ai-0.1.5/surv_ai/lib/conversation/interfaces.py
+-rw-r--r--   0        0        0       53 2023-05-08 03:25:52.022148 surv_ai-0.1.5/surv_ai/lib/knowledge_store/__init__.py
+-rw-r--r--   0        0        0      693 2023-05-22 15:04:42.556450 surv_ai-0.1.5/surv_ai/lib/knowledge_store/interfaces.py
+-rw-r--r--   0        0        0     1486 2023-05-22 15:04:42.581390 surv_ai-0.1.5/surv_ai/lib/knowledge_store/local.py
+-rw-r--r--   0        0        0        0 2023-04-16 19:53:58.086455 surv_ai-0.1.5/surv_ai/lib/llm/__init__.py
+-rw-r--r--   0        0        0     3755 2023-05-22 16:07:39.753305 surv_ai-0.1.5/surv_ai/lib/llm/anthropic.py
+-rw-r--r--   0        0        0     4261 2023-05-22 16:07:57.537852 surv_ai-0.1.5/surv_ai/lib/llm/gpt.py
+-rw-r--r--   0        0        0      432 2023-05-22 15:04:42.564655 surv_ai-0.1.5/surv_ai/lib/llm/interfaces.py
+-rw-r--r--   0        0        0     1960 2023-05-22 15:04:42.613196 surv_ai-0.1.5/surv_ai/lib/log.py
+-rw-r--r--   0        0        0        0 2023-04-16 23:16:14.406022 surv_ai-0.1.5/surv_ai/lib/tools/__init__.py
+-rw-r--r--   0        0        0      656 2023-05-22 19:00:03.447356 surv_ai-0.1.5/surv_ai/lib/tools/interfaces.py
+-rw-r--r--   0        0        0        0 2023-04-16 23:16:30.843990 surv_ai-0.1.5/surv_ai/lib/tools/query/__init__.py
+-rw-r--r--   0        0        0     7047 2023-05-22 16:09:44.603986 surv_ai-0.1.5/surv_ai/lib/tools/query/google_custom_search.py
+-rw-r--r--   0        0        0      219 2023-05-19 05:42:04.105413 surv_ai-0.1.5/surv_ai/lib/tools/query/interfaces.py
+-rw-r--r--   0        0        0     5918 2023-05-22 16:09:44.606441 surv_ai-0.1.5/surv_ai/lib/tools/query/wikipedia.py
+-rw-r--r--   0        0        0     2924 2023-05-22 19:00:12.464217 surv_ai-0.1.5/surv_ai/lib/tools/tool_belt.py
+-rw-r--r--   0        0        0    21038 1970-01-01 00:00:00.000000 surv_ai-0.1.5/PKG-INFO
```

### Comparing `surv_ai-0.1.4/LICENSE` & `surv_ai-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.4/README.md` & `surv_ai-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,56 @@
+Metadata-Version: 2.1
+Name: surv-ai
+Version: 0.1.5
+Summary: A framework for multi-agent modeling using large language models
+Home-page: https://github.com/DanielBalsam/surv_ai
+License: MIT
+Keywords: ai,artificial intelligence,data science,statistics,models,llm,agents,survai,surv_ai,survey,multi-agent,large language model,artificial intelligence,machine learning,natural language processing,nlp,sentiment analysis
+Author: Daniel Balsam
+Author-email: daniel.balsam@survai.org
+Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
+Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
+Requires-Dist: colorama (>=0.4.6,<0.5.0)
+Requires-Dist: exceptiongroup (>=1.1.1,<2.0.0)
+Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Project-URL: Documentation, https://github.com/DanielBalsam/surv_ai/blob/main/README.md
+Project-URL: Repository, https://github.com/DanielBalsam/surv_ai
+Description-Content-Type: text/markdown
+
 # 🕵 Multi-agent modeling with large language models 
 <!-- [![PyPi](https://img.shields.io/badge/Official%20Website-agpt.co-blue?style=flat&logo=world&logoColor=white)](https://agpt.co) -->
 [![Unit Tests](https://shields.io/github/actions/workflow/status/DanielBalsam/surv_ai/.github/workflows/ci.yaml?branch=main)](https://github.com/DanielBalsam/surv_ai/actions/workflows/ci.yaml)
 [![GitHub Repo stars](https://img.shields.io/github/stars/DanielBalsam/surv_ai?style=social)](https://github.com/DanielBalsam/surv_ai/stargazers)
 
 
 **`surv_ai` is a large language model framework designed for multi-agent modeling. This allows large-language models to be used as engines to power research into predictive modeling, bias analysis, and other forms of comparative analysis.**
 
 ![](https://raw.githubusercontent.com/DanielBalsam/surv_ai/main/examples/midterms_2022.png)
 
-**Multi-agent modeling** is the process of using the actions of various agents in order to produce statistical models. In our case, these models are created by having agents query and process text from a robust data corpus, and then "reason" with the information extracted from that text to produce a data point.
+**Multi-agent modeling** involves generating statistical models based on the actions of multiple agents. In our case, these models are crafted by agents querying and processing text from a comprehensive data corpus. The agents then reason with the information extracted to produce a data point.
 
-Given the stochastic nature of large language models, each data point may vary - however if a large enough sample of agents are used, the models that can be produced can be effective for comparative analysis.
+Given the stochastic nature of large language models, individual data points may vary. However, if a sufficient number of agents are employed, the generated models can effectively support comparative analysis.
 
-The abstraction in this repository that is capable of producing a data point is referred to as an `Survey`. A survey takes a statement as an argument and returns a percentage of agents which agreed with the statement.
+The abstraction in this repository capable of producing a data point is known as a `Survey`. A `Survey` takes a statement as input and returns the percentage of agents that agreed with it.
 
-A model that varies with respect to some independent variable a further abstraction called a `Model`, which allows us to vary input parameters into a `Survey` creating a proper multi-agent model.
+A more complex abstraction, called a `Model`, enables the variation of input parameters into a `Survey` to create a nuanced multi-agent model. This abstraction depends on some independent variable.
 
-The data points produced are ultimately end up being a form of sentiment analysis against a corpus of text. This means they are subject to the biases of both the large language models, and the corpus of text itself. 
+The data points produced serve as sentiment analysis against a text corpus, making them susceptible to the biases of both the large language models and the corpus itself.
 
-With further advances in large language models, and AI broadly, multi-agent modeling may continue to prove a useful paradigm for classification and regression models, and may become a valuable extra data point for researchers investigating complex issues with many complex underlying variables.
+As advances in large language models and AI continue, multi-agent modeling may remain a valuable framework for classification and regression models. It also has the potential to become a useful data point for researchers investigating complex issues with numerous underlying variables.
 
 ## 📲 Installation 
 
 Package is available on [PyPi](https://pypi.org/project/surv-ai/): 
 
 ```
 pip install surv-ai
@@ -30,19 +58,19 @@
 
 ## 📻 Contact 
 
 For all inquiries, contact me at: daniel.balsam@survai.org
 
 ## ✅ Responsible use 
 
-Examples below are meant to simply demonstrate the potential use-cases of this framework, and are not to be interpreted as scientifically rigorous.
+The examples provided below are intended merely to illustrate potential applications of this framework; they are not to be considered scientifically rigorous.
 
-While approaches like this have the potential to be used in research and guide decision making, it is important to always use a wide-variety of data points and to take any particular model with a grain of salt.
+Approaches like this have potential in guiding research and decision-making. However, it is crucial to rely on a diverse range of data points and to interpret each model cautiously.
 
-I am always eager for suggestions on how this approach can be further improved.
+I am always open to suggestions for further enhancing this approach.
 
 ## 📝 Basic usage 
 
 The two key abstractions in this repository are a `Survey` and a `Model`. 
 
 Calling `Survey.conduct` with a hypothesis will spin up a number of agents and seed them with some base knowledge. The agents are then asked to to assign a true or false value to the hypothesis provided. 
 
@@ -90,16 +118,14 @@
 [**Anthropic / Claude**](https://console.anthropic.com/docs)
 [**Google Custom Search**](https://developers.google.com/custom-search/v1/overview)
 
 ### Comparing against a ground truth
 
 Let's start by establishing the system's ability to figure out if information is true.
 
-For instance:
-
 ```
 from surv_ai import (
     GPTClient,
     Survey,
     ToolBelt,
     GoogleCustomSearchTool,
     Knowledge
@@ -133,19 +159,19 @@
 )
 
 await survey.conduct(
     "California experienced a significant amount of rainfall this winter.",
 )  # This should always returns high a confidence agreement.
 ```
 
-Running this code should produce an output like: `PollResponse(in_favor=10, against=0, undecided=0, error=0, percent_in_favor=1.0, uncertainty=0.0)`
+Executing this code should yield an output similar to: `SurveyResponse(in_favor=10, against=0, undecided=0, error=0, percent_in_favor=1.0, uncertainty=0.0)`
 
-It's worth noting that every so often, an agent or two may get a simple question like this wrong. That is why we use many agents in these systems - to combat the stochastic nature of LLMs.
+It's important to recognize that occasionally, one or two agents might incorrectly respond to a straightforward question like this. That's why we employ multiple agents in these systems - to counteract the randomness inherent in Large Language Models (LLMs).
 
-Another way to test our hypothesis is to make the opposite assertion and make sure we can the opposite value.
+To further test our hypothesis, we could also assert the contrary position and ensure we obtain the opposite value.
 
 ```
 from surv_ai import (
     GPTClient,
     Survey,
     ToolBelt,
     GoogleCustomSearchTool,
@@ -179,15 +205,15 @@
 )
 
 await survey.conduct(
     "California experienced little rainfall this winter.",
 )  # This should always returns a high confidence disagreement.
 ```
 
-Running this code should produce an output like: `PollResponse(in_favor=0, against=10, undecided=0, error=0, percent_in_favor=0.0, uncertainty=0.0)`
+Executing this code should result in an output similar to: `SurveyResponse(in_favor=0, against=10, undecided=0, error=0, percent_in_favor=0.0, uncertainty=0.0)`
 
 ### Comparing changes in sentiment over time
 
 One thing we can use this tool for is measuring changes in sentiment overtime. GPT's training data ends in late 2021, so one way we can test our models with GPT is by looking at events that happened after GPT's training cutoff.
 
 For instance, we can plot how sentiment regarding the United States' 2022 Midterm Elections evolved in the months leading up to it:
 
@@ -248,20 +274,20 @@
 )
 
 results = await model.build(
     "Democrats are favored to maintain control of the Senate in the 2022 November Midterm elections.",
 )
 ```
 
-Plotted next to a domain leading model in the world of political opinion polling, our model looks like this:
+When compared with a leading model in political opinion polling, our model is presented as follows:
 
 ![](https://raw.githubusercontent.com/DanielBalsam/surv_ai/main/examples/midterms_2022.png)
-*Websites crawled by the agents in this example: nytimes.com, wsj.com, abcnews.com, cnn.com, bloomberg.com, foxnews.com, economist.com, washingtonpost.com, nbcnews.com*
+*In this example, the agents crawled websites such as nytimes.com, wsj.com, abcnews.com, cnn.com, bloomberg.com, foxnews.com, economist.com, washingtonpost.com, and nbcnews.com.*
 
-Pretty neat! Another example would be plotting sentiment regarding the economy and using changes in the Consumer Confidence Index as a ground truth.
+Pretty cool! Another example could involve plotting sentiments about the economy and using fluctuations in the Consumer Confidence Index as a benchmark for accuracy.
 
 ```
 from surv_ai import (
     GPTClient,
     Model,
     ToolBelt,
     GoogleCustomSearchTool,
@@ -319,19 +345,19 @@
     "The United States economy looks like it is heading for a recession.",
 )
 ```
 
 This gives us the following graph:
 
 ![](https://raw.githubusercontent.com/DanielBalsam/surv_ai/main/examples/cci.png)
-*Websites crawled by the agents in this example: nytimes.com, wsj.com, abcnews.com, cnn.com, bloomberg.com, foxnews.com, economist.com, washingtonpost.com, nbcnews.com*
+*In this example, the agents crawled websites such as nytimes.com, wsj.com, abcnews.com, cnn.com, bloomberg.com, foxnews.com, economist.com, washingtonpost.com, and nbcnews.com.*
 
 ### Measuring bias in different data corpuses
 
-One promising use of this technique is to observe bias in a corpus. For instance - we can create a model that uses different news sites as its independent variable, to see how the agents conclusions may differ using that data source.
+A promising application of this technique is observing bias within a text corpus. For instance, we could create a model that uses different news sites as its independent variable to explore how the agents' conclusions might vary based on the data source utilized.
 
 ```
 from surv_ai import (
     GPTClient,
     Model,
     ToolBelt,
     GoogleCustomSearchTool,
@@ -382,21 +408,21 @@
     ],
 )
 results = await model.build(
     "Republicans are responsible for the impending debt ceiling crisis."
 )
 ```
 
-This gives us the following scatter plot for the news sources above:
+This provides us with a scatter plot representing the above-mentioned news sources:
 
 ![](https://raw.githubusercontent.com/DanielBalsam/surv_ai/main/examples/debt_ceiling.png)
 
 ### Measuring biases in different large language models
 
-Another promising bias measurement approach is to compare biases across large language models, otherwise given the same parameters as input.
+Another promising method for measuring bias involves comparing biases across various large language models, provided they all receive identical input parameters.
 
 ```
 from surv_ai import (
     GPTClient,
     AnthropicClient,
     Model,
     ToolBelt,
@@ -444,26 +470,26 @@
     ],
 )
 results = await model.build(
     "OpenAI has been irresponsible in their handling of AI technology."
 )
 ```
 
-Comparing this statement between Claude and OpenAI, we get the following scatter plot:
+When we compare this statement between Anthropic and OpenAI's models, the resulting scatter plot appears as follows:
 
 ![](https://raw.githubusercontent.com/DanielBalsam/surv_ai/main/examples/openai.png)
 
 
 ## 🧠 Tips 
 
-Ultimately a `Survey` is powered by an LLM, and so the survey hypothesis may need to be tuned the same way that prompts more generally need to be tuned. Here are some tips for thinking about how to write hypotheses.
+Ultimately, a `Survey` is powered by a Large Language Model (LLM), which means that the survey hypothesis might require tuning, much like the general need to tune prompts. Here are some insights on crafting hypotheses.
 
-In these systems, often ambiguity in the original hypothesis can lead to strange results. This is often because the agents are interpreting the statement a little too literally, and thus rejecting the exact phrasing of the statement.
+In these systems, any ambiguity in the original hypothesis can lead to unexpected results. This often happens because the agents interpret the statement too literally, thus rejecting the precise phrasing of the statement.
 
-Another helpful trick is to seed base knowledge to the agents which provides additional context to the problem. To revisit an earlier example:
+Another useful tactic involves seeding base knowledge to the agents, which provides extra context to the problem. To revisit a previous example:
 
 ```
 from surv_ai import (
     GPTClient,
     Survey,
     ToolBelt,
     GoogleCustomSearchTool,
@@ -498,26 +524,26 @@
 )
 
 await survey.conduct(
     "California experienced a significant amount of rainfall this winter.",
 )  # This should always returns high a confidence agreement.
 ```
 
-The base knowledge helps keep the agent's on track. As GPT's training data ends in 2021, without the additional prompt GPT may believe it is still 2021 and thus has no way of assessing the validity of the statement.
+The base knowledge assists in keeping the agents on track. As GPT's training data concludes in 2021, without an additional prompt, GPT might assume it's still 2021, which would prevent it from evaluating the statement's validity accurately.
 
-A little trial and error is often necessary, however one way to debug is you can read the output of the agents very easily by setting the log level:
+A bit of trial and error is often necessary, but you can debug more efficiently by reading the output of the agents. This is made possible by setting the log level:
 
 ```
 from lib.log import logger, AgentLogLevel
 
 logger.set_log_level(AgentLogLevel.OUTPUT)  # Output from the agents will be logged
 logger.set_log_level(AgentLogLevel.INTERNAL)  # Agent internal "thoughts" will be logged
 ```
 
-You can also prompt agents directly:
+You may also prompt agents directly:
 
 ```
 from surv_ai import (
     GPTClient,
     ReasoningAgent,
     Knowledge
 )
@@ -534,27 +560,28 @@
 )
 
 agent.prompt("There are multiple ways to teach an agent knowledge.")
 ```
 
 ## 🤩 Inspiration 
 
-This project was inspired by many other cool projects and papers coming out recently. Some of the inspirations for this project are:
+This project was inspired by numerous innovative projects and recent papers. Some of the inspirations for this project include:
 
 1. [Generative Agents: Interactive Simulacra of Human Behavior](https://arxiv.org/abs/2304.03442).
 2. [Large Language Models are Zero-Shot Reasoners](https://arxiv.org/abs/2205.11916)
 3. [AutoGPT](https://github.com/Significant-Gravitas/Auto-GPT)
 
-And the many other researchers and engineers out there helping unlock the power of these models!
+Additionally, thanks go to the multitude of researchers and engineers out there who are contributing to unlocking the power of these models!
 
 ## 📈 Next steps 
 
-A few of the next places I'd like to take this project are:
+A few directions I plan to explore with this project include:
 
-1. I am considering migrating the core LLM interaction code to leverage [Microsoft's Guidance framework](https://github.com/microsoft/guidance).
-2. Continue to refine the agent code to lead to better decision making agents across a wide variety of problems. Very interested in exploring [Tree of Thought Prompting](https://arxiv.org/pdf/2305.10601.pdf) to see what results are yielded there.
-3. Integrations with more instruction-tuned and reinforcement learnt LLMs.
+1. I'm considering transitioning the core Large Language Model (LLM) interaction code to take advantage of Microsoft's Guidance framework.
+2. I aim to further refine the agent code to improve decision-making across a wide variety of problems. I'm particularly interested in exploring Tree of Thought Prompting to see the outcomes it generates.
+3. I plan to incorporate more instruction-tuned and reinforcement-learned LLMs.
 
 
 ## 🤝 Contribute 
 
 If you'd like to contribute then please reach out!
+
```

### Comparing `surv_ai-0.1.4/pyproject.toml` & `surv_ai-0.1.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "surv_ai"
-version = "0.1.4"
+version = "0.1.5"
 description = "A framework for multi-agent modeling using large language models"
 authors = ["Daniel Balsam <daniel.balsam@survai.org>"]
 license = "MIT"
 readme = "README.md"
 keywords=[
     "ai",
     "artificial intelligence",
```

### Comparing `surv_ai-0.1.4/surv_ai/__init__.py` & `surv_ai-0.1.5/surv_ai/__init__.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.4/surv_ai/core/agent.py` & `surv_ai-0.1.5/surv_ai/core/agent.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.4/surv_ai/core/agents/binary.py` & `surv_ai-0.1.5/surv_ai/core/agents/binary.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.4/surv_ai/core/agents/reasoning.py` & `surv_ai-0.1.5/surv_ai/core/agents/reasoning.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.4/surv_ai/core/interfaces.py` & `surv_ai-0.1.5/surv_ai/core/interfaces.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.4/surv_ai/core/model.py` & `surv_ai-0.1.5/surv_ai/core/model.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.4/surv_ai/core/survey.py` & `surv_ai-0.1.5/surv_ai/core/survey.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.4/surv_ai/lib/conversation/conversation.py` & `surv_ai-0.1.5/surv_ai/lib/conversation/conversation.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.4/surv_ai/lib/knowledge_store/interfaces.py` & `surv_ai-0.1.5/surv_ai/lib/knowledge_store/interfaces.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.4/surv_ai/lib/knowledge_store/local.py` & `surv_ai-0.1.5/surv_ai/lib/knowledge_store/local.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.4/surv_ai/lib/llm/anthropic.py` & `surv_ai-0.1.5/surv_ai/lib/llm/anthropic.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.4/surv_ai/lib/llm/gpt.py` & `surv_ai-0.1.5/surv_ai/lib/llm/gpt.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.4/surv_ai/lib/log.py` & `surv_ai-0.1.5/surv_ai/lib/log.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.4/surv_ai/lib/tools/interfaces.py` & `surv_ai-0.1.5/surv_ai/lib/tools/interfaces.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.4/surv_ai/lib/tools/query/google_custom_search.py` & `surv_ai-0.1.5/surv_ai/lib/tools/query/google_custom_search.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.4/surv_ai/lib/tools/query/wikipedia.py` & `surv_ai-0.1.5/surv_ai/lib/tools/query/wikipedia.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.4/surv_ai/lib/tools/tool_belt.py` & `surv_ai-0.1.5/surv_ai/lib/tools/tool_belt.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.4/PKG-INFO` & `surv_ai-0.1.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,28 @@
-Metadata-Version: 2.1
-Name: surv-ai
-Version: 0.1.4
-Summary: A framework for multi-agent modeling using large language models
-Home-page: https://github.com/DanielBalsam/surv_ai
-License: MIT
-Keywords: ai,artificial intelligence,data science,statistics,models,llm,agents,survai,surv_ai,survey,multi-agent,large language model,artificial intelligence,machine learning,natural language processing,nlp,sentiment analysis
-Author: Daniel Balsam
-Author-email: daniel.balsam@survai.org
-Requires-Python: >=3.9,<4.0
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
-Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
-Requires-Dist: colorama (>=0.4.6,<0.5.0)
-Requires-Dist: exceptiongroup (>=1.1.1,<2.0.0)
-Requires-Dist: pydantic (>=1.10.7,<2.0.0)
-Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
-Project-URL: Documentation, https://github.com/DanielBalsam/surv_ai/blob/main/README.md
-Project-URL: Repository, https://github.com/DanielBalsam/surv_ai
-Description-Content-Type: text/markdown
-
 # 🕵 Multi-agent modeling with large language models 
 <!-- [![PyPi](https://img.shields.io/badge/Official%20Website-agpt.co-blue?style=flat&logo=world&logoColor=white)](https://agpt.co) -->
 [![Unit Tests](https://shields.io/github/actions/workflow/status/DanielBalsam/surv_ai/.github/workflows/ci.yaml?branch=main)](https://github.com/DanielBalsam/surv_ai/actions/workflows/ci.yaml)
 [![GitHub Repo stars](https://img.shields.io/github/stars/DanielBalsam/surv_ai?style=social)](https://github.com/DanielBalsam/surv_ai/stargazers)
 
 
 **`surv_ai` is a large language model framework designed for multi-agent modeling. This allows large-language models to be used as engines to power research into predictive modeling, bias analysis, and other forms of comparative analysis.**
 
 ![](https://raw.githubusercontent.com/DanielBalsam/surv_ai/main/examples/midterms_2022.png)
 
-**Multi-agent modeling** is the process of using the actions of various agents in order to produce statistical models. In our case, these models are created by having agents query and process text from a robust data corpus, and then "reason" with the information extracted from that text to produce a data point.
+**Multi-agent modeling** involves generating statistical models based on the actions of multiple agents. In our case, these models are crafted by agents querying and processing text from a comprehensive data corpus. The agents then reason with the information extracted to produce a data point.
 
-Given the stochastic nature of large language models, each data point may vary - however if a large enough sample of agents are used, the models that can be produced can be effective for comparative analysis.
+Given the stochastic nature of large language models, individual data points may vary. However, if a sufficient number of agents are employed, the generated models can effectively support comparative analysis.
 
-The abstraction in this repository that is capable of producing a data point is referred to as an `Survey`. A survey takes a statement as an argument and returns a percentage of agents which agreed with the statement.
+The abstraction in this repository capable of producing a data point is known as a `Survey`. A `Survey` takes a statement as input and returns the percentage of agents that agreed with it.
 
-A model that varies with respect to some independent variable a further abstraction called a `Model`, which allows us to vary input parameters into a `Survey` creating a proper multi-agent model.
+A more complex abstraction, called a `Model`, enables the variation of input parameters into a `Survey` to create a nuanced multi-agent model. This abstraction depends on some independent variable.
 
-The data points produced are ultimately end up being a form of sentiment analysis against a corpus of text. This means they are subject to the biases of both the large language models, and the corpus of text itself. 
+The data points produced serve as sentiment analysis against a text corpus, making them susceptible to the biases of both the large language models and the corpus itself.
 
-With further advances in large language models, and AI broadly, multi-agent modeling may continue to prove a useful paradigm for classification and regression models, and may become a valuable extra data point for researchers investigating complex issues with many complex underlying variables.
+As advances in large language models and AI continue, multi-agent modeling may remain a valuable framework for classification and regression models. It also has the potential to become a useful data point for researchers investigating complex issues with numerous underlying variables.
 
 ## 📲 Installation 
 
 Package is available on [PyPi](https://pypi.org/project/surv-ai/): 
 
 ```
 pip install surv-ai
@@ -58,19 +30,19 @@
 
 ## 📻 Contact 
 
 For all inquiries, contact me at: daniel.balsam@survai.org
 
 ## ✅ Responsible use 
 
-Examples below are meant to simply demonstrate the potential use-cases of this framework, and are not to be interpreted as scientifically rigorous.
+The examples provided below are intended merely to illustrate potential applications of this framework; they are not to be considered scientifically rigorous.
 
-While approaches like this have the potential to be used in research and guide decision making, it is important to always use a wide-variety of data points and to take any particular model with a grain of salt.
+Approaches like this have potential in guiding research and decision-making. However, it is crucial to rely on a diverse range of data points and to interpret each model cautiously.
 
-I am always eager for suggestions on how this approach can be further improved.
+I am always open to suggestions for further enhancing this approach.
 
 ## 📝 Basic usage 
 
 The two key abstractions in this repository are a `Survey` and a `Model`. 
 
 Calling `Survey.conduct` with a hypothesis will spin up a number of agents and seed them with some base knowledge. The agents are then asked to to assign a true or false value to the hypothesis provided. 
 
@@ -118,16 +90,14 @@
 [**Anthropic / Claude**](https://console.anthropic.com/docs)
 [**Google Custom Search**](https://developers.google.com/custom-search/v1/overview)
 
 ### Comparing against a ground truth
 
 Let's start by establishing the system's ability to figure out if information is true.
 
-For instance:
-
 ```
 from surv_ai import (
     GPTClient,
     Survey,
     ToolBelt,
     GoogleCustomSearchTool,
     Knowledge
@@ -161,19 +131,19 @@
 )
 
 await survey.conduct(
     "California experienced a significant amount of rainfall this winter.",
 )  # This should always returns high a confidence agreement.
 ```
 
-Running this code should produce an output like: `PollResponse(in_favor=10, against=0, undecided=0, error=0, percent_in_favor=1.0, uncertainty=0.0)`
+Executing this code should yield an output similar to: `SurveyResponse(in_favor=10, against=0, undecided=0, error=0, percent_in_favor=1.0, uncertainty=0.0)`
 
-It's worth noting that every so often, an agent or two may get a simple question like this wrong. That is why we use many agents in these systems - to combat the stochastic nature of LLMs.
+It's important to recognize that occasionally, one or two agents might incorrectly respond to a straightforward question like this. That's why we employ multiple agents in these systems - to counteract the randomness inherent in Large Language Models (LLMs).
 
-Another way to test our hypothesis is to make the opposite assertion and make sure we can the opposite value.
+To further test our hypothesis, we could also assert the contrary position and ensure we obtain the opposite value.
 
 ```
 from surv_ai import (
     GPTClient,
     Survey,
     ToolBelt,
     GoogleCustomSearchTool,
@@ -207,15 +177,15 @@
 )
 
 await survey.conduct(
     "California experienced little rainfall this winter.",
 )  # This should always returns a high confidence disagreement.
 ```
 
-Running this code should produce an output like: `PollResponse(in_favor=0, against=10, undecided=0, error=0, percent_in_favor=0.0, uncertainty=0.0)`
+Executing this code should result in an output similar to: `SurveyResponse(in_favor=0, against=10, undecided=0, error=0, percent_in_favor=0.0, uncertainty=0.0)`
 
 ### Comparing changes in sentiment over time
 
 One thing we can use this tool for is measuring changes in sentiment overtime. GPT's training data ends in late 2021, so one way we can test our models with GPT is by looking at events that happened after GPT's training cutoff.
 
 For instance, we can plot how sentiment regarding the United States' 2022 Midterm Elections evolved in the months leading up to it:
 
@@ -276,20 +246,20 @@
 )
 
 results = await model.build(
     "Democrats are favored to maintain control of the Senate in the 2022 November Midterm elections.",
 )
 ```
 
-Plotted next to a domain leading model in the world of political opinion polling, our model looks like this:
+When compared with a leading model in political opinion polling, our model is presented as follows:
 
 ![](https://raw.githubusercontent.com/DanielBalsam/surv_ai/main/examples/midterms_2022.png)
-*Websites crawled by the agents in this example: nytimes.com, wsj.com, abcnews.com, cnn.com, bloomberg.com, foxnews.com, economist.com, washingtonpost.com, nbcnews.com*
+*In this example, the agents crawled websites such as nytimes.com, wsj.com, abcnews.com, cnn.com, bloomberg.com, foxnews.com, economist.com, washingtonpost.com, and nbcnews.com.*
 
-Pretty neat! Another example would be plotting sentiment regarding the economy and using changes in the Consumer Confidence Index as a ground truth.
+Pretty cool! Another example could involve plotting sentiments about the economy and using fluctuations in the Consumer Confidence Index as a benchmark for accuracy.
 
 ```
 from surv_ai import (
     GPTClient,
     Model,
     ToolBelt,
     GoogleCustomSearchTool,
@@ -347,19 +317,19 @@
     "The United States economy looks like it is heading for a recession.",
 )
 ```
 
 This gives us the following graph:
 
 ![](https://raw.githubusercontent.com/DanielBalsam/surv_ai/main/examples/cci.png)
-*Websites crawled by the agents in this example: nytimes.com, wsj.com, abcnews.com, cnn.com, bloomberg.com, foxnews.com, economist.com, washingtonpost.com, nbcnews.com*
+*In this example, the agents crawled websites such as nytimes.com, wsj.com, abcnews.com, cnn.com, bloomberg.com, foxnews.com, economist.com, washingtonpost.com, and nbcnews.com.*
 
 ### Measuring bias in different data corpuses
 
-One promising use of this technique is to observe bias in a corpus. For instance - we can create a model that uses different news sites as its independent variable, to see how the agents conclusions may differ using that data source.
+A promising application of this technique is observing bias within a text corpus. For instance, we could create a model that uses different news sites as its independent variable to explore how the agents' conclusions might vary based on the data source utilized.
 
 ```
 from surv_ai import (
     GPTClient,
     Model,
     ToolBelt,
     GoogleCustomSearchTool,
@@ -410,21 +380,21 @@
     ],
 )
 results = await model.build(
     "Republicans are responsible for the impending debt ceiling crisis."
 )
 ```
 
-This gives us the following scatter plot for the news sources above:
+This provides us with a scatter plot representing the above-mentioned news sources:
 
 ![](https://raw.githubusercontent.com/DanielBalsam/surv_ai/main/examples/debt_ceiling.png)
 
 ### Measuring biases in different large language models
 
-Another promising bias measurement approach is to compare biases across large language models, otherwise given the same parameters as input.
+Another promising method for measuring bias involves comparing biases across various large language models, provided they all receive identical input parameters.
 
 ```
 from surv_ai import (
     GPTClient,
     AnthropicClient,
     Model,
     ToolBelt,
@@ -472,26 +442,26 @@
     ],
 )
 results = await model.build(
     "OpenAI has been irresponsible in their handling of AI technology."
 )
 ```
 
-Comparing this statement between Claude and OpenAI, we get the following scatter plot:
+When we compare this statement between Anthropic and OpenAI's models, the resulting scatter plot appears as follows:
 
 ![](https://raw.githubusercontent.com/DanielBalsam/surv_ai/main/examples/openai.png)
 
 
 ## 🧠 Tips 
 
-Ultimately a `Survey` is powered by an LLM, and so the survey hypothesis may need to be tuned the same way that prompts more generally need to be tuned. Here are some tips for thinking about how to write hypotheses.
+Ultimately, a `Survey` is powered by a Large Language Model (LLM), which means that the survey hypothesis might require tuning, much like the general need to tune prompts. Here are some insights on crafting hypotheses.
 
-In these systems, often ambiguity in the original hypothesis can lead to strange results. This is often because the agents are interpreting the statement a little too literally, and thus rejecting the exact phrasing of the statement.
+In these systems, any ambiguity in the original hypothesis can lead to unexpected results. This often happens because the agents interpret the statement too literally, thus rejecting the precise phrasing of the statement.
 
-Another helpful trick is to seed base knowledge to the agents which provides additional context to the problem. To revisit an earlier example:
+Another useful tactic involves seeding base knowledge to the agents, which provides extra context to the problem. To revisit a previous example:
 
 ```
 from surv_ai import (
     GPTClient,
     Survey,
     ToolBelt,
     GoogleCustomSearchTool,
@@ -526,26 +496,26 @@
 )
 
 await survey.conduct(
     "California experienced a significant amount of rainfall this winter.",
 )  # This should always returns high a confidence agreement.
 ```
 
-The base knowledge helps keep the agent's on track. As GPT's training data ends in 2021, without the additional prompt GPT may believe it is still 2021 and thus has no way of assessing the validity of the statement.
+The base knowledge assists in keeping the agents on track. As GPT's training data concludes in 2021, without an additional prompt, GPT might assume it's still 2021, which would prevent it from evaluating the statement's validity accurately.
 
-A little trial and error is often necessary, however one way to debug is you can read the output of the agents very easily by setting the log level:
+A bit of trial and error is often necessary, but you can debug more efficiently by reading the output of the agents. This is made possible by setting the log level:
 
 ```
 from lib.log import logger, AgentLogLevel
 
 logger.set_log_level(AgentLogLevel.OUTPUT)  # Output from the agents will be logged
 logger.set_log_level(AgentLogLevel.INTERNAL)  # Agent internal "thoughts" will be logged
 ```
 
-You can also prompt agents directly:
+You may also prompt agents directly:
 
 ```
 from surv_ai import (
     GPTClient,
     ReasoningAgent,
     Knowledge
 )
@@ -562,28 +532,27 @@
 )
 
 agent.prompt("There are multiple ways to teach an agent knowledge.")
 ```
 
 ## 🤩 Inspiration 
 
-This project was inspired by many other cool projects and papers coming out recently. Some of the inspirations for this project are:
+This project was inspired by numerous innovative projects and recent papers. Some of the inspirations for this project include:
 
 1. [Generative Agents: Interactive Simulacra of Human Behavior](https://arxiv.org/abs/2304.03442).
 2. [Large Language Models are Zero-Shot Reasoners](https://arxiv.org/abs/2205.11916)
 3. [AutoGPT](https://github.com/Significant-Gravitas/Auto-GPT)
 
-And the many other researchers and engineers out there helping unlock the power of these models!
+Additionally, thanks go to the multitude of researchers and engineers out there who are contributing to unlocking the power of these models!
 
 ## 📈 Next steps 
 
-A few of the next places I'd like to take this project are:
+A few directions I plan to explore with this project include:
 
-1. I am considering migrating the core LLM interaction code to leverage [Microsoft's Guidance framework](https://github.com/microsoft/guidance).
-2. Continue to refine the agent code to lead to better decision making agents across a wide variety of problems. Very interested in exploring [Tree of Thought Prompting](https://arxiv.org/pdf/2305.10601.pdf) to see what results are yielded there.
-3. Integrations with more instruction-tuned and reinforcement learnt LLMs.
+1. I'm considering transitioning the core Large Language Model (LLM) interaction code to take advantage of Microsoft's Guidance framework.
+2. I aim to further refine the agent code to improve decision-making across a wide variety of problems. I'm particularly interested in exploring Tree of Thought Prompting to see the outcomes it generates.
+3. I plan to incorporate more instruction-tuned and reinforcement-learned LLMs.
 
 
 ## 🤝 Contribute 
 
 If you'd like to contribute then please reach out!
-
```

