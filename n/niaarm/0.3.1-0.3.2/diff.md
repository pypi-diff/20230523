# Comparing `tmp/niaarm-0.3.1.tar.gz` & `tmp/niaarm-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "niaarm-0.3.1.tar", max compression
+gzip compressed data, was "niaarm-0.3.2.tar", max compression
```

## Comparing `niaarm-0.3.1.tar` & `niaarm-0.3.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     9405 2023-02-14 19:43:42.843226 niaarm-0.3.1/CHANGELOG.md
--rw-r--r--   0        0        0     1095 2023-02-14 19:43:42.843226 niaarm-0.3.1/LICENSE
--rw-r--r--   0        0        0    12607 2023-02-14 19:43:42.843226 niaarm-0.3.1/README.md
--rw-r--r--   0        0        0      396 2023-02-14 19:43:42.846226 niaarm-0.3.1/niaarm/__init__.py
--rw-r--r--   0        0        0       88 2023-02-14 19:43:42.846226 niaarm-0.3.1/niaarm/__main__.py
--rw-r--r--   0        0        0     6633 2023-02-14 19:43:42.846226 niaarm-0.3.1/niaarm/cli.py
--rw-r--r--   0        0        0     4055 2023-02-14 19:43:42.846226 niaarm-0.3.1/niaarm/dataset.py
--rw-r--r--   0        0        0     1305 2023-02-14 19:43:42.846226 niaarm-0.3.1/niaarm/feature.py
--rw-r--r--   0        0        0     4457 2023-02-14 19:43:42.846226 niaarm-0.3.1/niaarm/mine.py
--rw-r--r--   0        0        0     6614 2023-02-14 19:43:42.846226 niaarm-0.3.1/niaarm/niaarm.py
--rw-r--r--   0        0        0     2490 2023-02-14 19:43:42.846226 niaarm-0.3.1/niaarm/preprocessing.py
--rw-r--r--   0        0        0    12829 2023-02-14 19:43:42.846226 niaarm-0.3.1/niaarm/rule.py
--rw-r--r--   0        0        0     3699 2023-02-14 19:43:42.846226 niaarm-0.3.1/niaarm/rule_list.py
--rw-r--r--   0        0        0    11840 2023-02-14 19:43:42.846226 niaarm-0.3.1/niaarm/text.py
--rw-r--r--   0        0        0     3777 2023-02-14 19:43:42.846226 niaarm-0.3.1/niaarm/visualize.py
--rw-r--r--   0        0        0     1522 2023-02-14 19:43:42.846226 niaarm-0.3.1/niaarm.1
--rw-r--r--   0        0        0     1129 2023-02-14 19:43:42.848226 niaarm-0.3.1/pyproject.toml
--rw-r--r--   0        0        0    14251 2023-02-14 19:43:51.547946 niaarm-0.3.1/setup.py
--rw-r--r--   0        0        0    13767 2023-02-14 19:43:51.548768 niaarm-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11629 2023-05-23 13:00:36.137068 niaarm-0.3.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1095 2023-05-23 13:00:36.137068 niaarm-0.3.2/LICENSE
+-rw-r--r--   0        0        0    12607 2023-05-23 13:00:36.137068 niaarm-0.3.2/README.md
+-rw-r--r--   0        0        0      396 2023-05-23 13:00:36.142068 niaarm-0.3.2/niaarm/__init__.py
+-rw-r--r--   0        0        0       88 2023-05-23 13:00:36.142068 niaarm-0.3.2/niaarm/__main__.py
+-rw-r--r--   0        0        0     6633 2023-05-23 13:00:36.142068 niaarm-0.3.2/niaarm/cli.py
+-rw-r--r--   0        0        0     4055 2023-05-23 13:00:36.142068 niaarm-0.3.2/niaarm/dataset.py
+-rw-r--r--   0        0        0     1305 2023-05-23 13:00:36.142068 niaarm-0.3.2/niaarm/feature.py
+-rw-r--r--   0        0        0     4457 2023-05-23 13:00:36.142068 niaarm-0.3.2/niaarm/mine.py
+-rw-r--r--   0        0        0     6614 2023-05-23 13:00:36.142068 niaarm-0.3.2/niaarm/niaarm.py
+-rw-r--r--   0        0        0     2490 2023-05-23 13:00:36.142068 niaarm-0.3.2/niaarm/preprocessing.py
+-rw-r--r--   0        0        0    12829 2023-05-23 13:00:36.142068 niaarm-0.3.2/niaarm/rule.py
+-rw-r--r--   0        0        0     3765 2023-05-23 13:00:36.142068 niaarm-0.3.2/niaarm/rule_list.py
+-rw-r--r--   0        0        0    11840 2023-05-23 13:00:36.142068 niaarm-0.3.2/niaarm/text.py
+-rw-r--r--   0        0        0     3777 2023-05-23 13:00:36.143068 niaarm-0.3.2/niaarm/visualize.py
+-rw-r--r--   0        0        0     1542 2023-05-23 13:00:36.142068 niaarm-0.3.2/niaarm.1
+-rw-r--r--   0        0        0     1359 2023-05-23 13:00:36.146068 niaarm-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0    14286 2023-05-23 13:00:55.692140 niaarm-0.3.2/setup.py
+-rw-r--r--   0        0        0    13988 2023-05-23 13:00:55.693674 niaarm-0.3.2/PKG-INFO
```

### Comparing `niaarm-0.3.1/CHANGELOG.md` & `niaarm-0.3.2/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,59 @@
 # Changelog
 
+## [0.3.1](https://github.com/firefly-cpp/NiaARM/tree/0.3.1) (2023-02-14)
+
+[Full Changelog](https://github.com/firefly-cpp/NiaARM/compare/0.3.0...0.3.1)
+
+**Merged pull requests:**
+
+- squashing refactor [\#86](https://github.com/firefly-cpp/NiaARM/pull/86) ([zStupan](https://github.com/zStupan))
+
+## [0.3.0](https://github.com/firefly-cpp/NiaARM/tree/0.3.0) (2023-02-12)
+
+[Full Changelog](https://github.com/firefly-cpp/NiaARM/compare/0.2.4...0.3.0)
+
+**Closed issues:**
+
+- Lift metric problem [\#82](https://github.com/firefly-cpp/NiaARM/issues/82)
+- Mining association rules the hard way \(example\) [\#80](https://github.com/firefly-cpp/NiaARM/issues/80)
+- Add Fedora/Arch linux badges [\#79](https://github.com/firefly-cpp/NiaARM/issues/79)
+
+**Merged pull requests:**
+
+- Add data squashing [\#85](https://github.com/firefly-cpp/NiaARM/pull/85) ([zStupan](https://github.com/zStupan))
+
+## [0.2.4](https://github.com/firefly-cpp/NiaARM/tree/0.2.4) (2022-12-23)
+
+[Full Changelog](https://github.com/firefly-cpp/NiaARM/compare/0.2.3...0.2.4)
+
+**Closed issues:**
+
+- New example [\#64](https://github.com/firefly-cpp/NiaARM/issues/64)
+- Test for text mining is missing [\#63](https://github.com/firefly-cpp/NiaARM/issues/63)
+
+**Merged pull requests:**
+
+- Update text mining [\#78](https://github.com/firefly-cpp/NiaARM/pull/78) ([zStupan](https://github.com/zStupan))
+- Add rule example [\#77](https://github.com/firefly-cpp/NiaARM/pull/77) ([zStupan](https://github.com/zStupan))
+
+## [0.2.3](https://github.com/firefly-cpp/NiaARM/tree/0.2.3) (2022-12-17)
+
+[Full Changelog](https://github.com/firefly-cpp/NiaARM/compare/0.2.2...0.2.3)
+
+**Closed issues:**
+
+- Prepare CITATION.cff file for JOSS paper [\#75](https://github.com/firefly-cpp/NiaARM/issues/75)
+
+**Merged pull requests:**
+
+- Bump certifi from 2022.5.18.1 to 2022.12.7 [\#76](https://github.com/firefly-cpp/NiaARM/pull/76) ([dependabot[bot]](https://github.com/apps/dependabot))
+- Bump joblib from 1.1.0 to 1.2.0 [\#74](https://github.com/firefly-cpp/NiaARM/pull/74) ([dependabot[bot]](https://github.com/apps/dependabot))
+- Bump pillow from 9.1.1 to 9.3.0 [\#73](https://github.com/firefly-cpp/NiaARM/pull/73) ([dependabot[bot]](https://github.com/apps/dependabot))
+
 ## [0.2.2](https://github.com/firefly-cpp/NiaARM/tree/0.2.2) (2022-10-15)
 
 [Full Changelog](https://github.com/firefly-cpp/NiaARM/compare/0.2.1...0.2.2)
 
 **Closed issues:**
 
 - Add man page for CLI [\#71](https://github.com/firefly-cpp/NiaARM/issues/71)
```

### Comparing `niaarm-0.3.1/LICENSE` & `niaarm-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `niaarm-0.3.1/README.md` & `niaarm-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `niaarm-0.3.1/niaarm/cli.py` & `niaarm-0.3.2/niaarm/cli.py`

 * *Files identical despite different names*

### Comparing `niaarm-0.3.1/niaarm/dataset.py` & `niaarm-0.3.2/niaarm/dataset.py`

 * *Files identical despite different names*

### Comparing `niaarm-0.3.1/niaarm/feature.py` & `niaarm-0.3.2/niaarm/feature.py`

 * *Files identical despite different names*

### Comparing `niaarm-0.3.1/niaarm/mine.py` & `niaarm-0.3.2/niaarm/mine.py`

 * *Files identical despite different names*

### Comparing `niaarm-0.3.1/niaarm/niaarm.py` & `niaarm-0.3.2/niaarm/niaarm.py`

 * *Files identical despite different names*

### Comparing `niaarm-0.3.1/niaarm/preprocessing.py` & `niaarm-0.3.2/niaarm/preprocessing.py`

 * *Files identical despite different names*

### Comparing `niaarm-0.3.1/niaarm/rule.py` & `niaarm-0.3.2/niaarm/rule.py`

 * *Files identical despite different names*

### Comparing `niaarm-0.3.1/niaarm/rule_list.py` & `niaarm-0.3.2/niaarm/rule_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,14 +93,17 @@
 
             for rule in self.data:
                 writer.writerow(
                     [rule.antecedent, rule.consequent, rule.fitness] + [getattr(rule, metric) for metric in metrics])
         print(f"Rules exported to {filename}")
 
     def __str__(self):
+        if not self:  # if list is empty
+            return '[]'
+
         string = f'STATS:\n' \
                  f'Total rules: {len(self)}\n' \
                  f'Average fitness: {self.mean("fitness")}\n' \
                  f'Average support: {self.mean("support")}\n' \
                  f'Average confidence: {self.mean("confidence")}\n' \
                  f'Average lift: {self.mean("lift")}\n' \
                  f'Average coverage: {self.mean("coverage")}\n' \
```

### Comparing `niaarm-0.3.1/niaarm/text.py` & `niaarm-0.3.2/niaarm/text.py`

 * *Files identical despite different names*

### Comparing `niaarm-0.3.1/niaarm/visualize.py` & `niaarm-0.3.2/niaarm/visualize.py`

 * *Files identical despite different names*

### Comparing `niaarm-0.3.1/niaarm.1` & `niaarm-0.3.2/niaarm.1`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 .TH NIAARM "1" "October 2022" "" "User Commands"
 .SH NAME
 .B niaarm
-\(en perform ARM, output mined rules as csv, get mined rules\(cq statistics
+\(en perform Association Rule Mining, output mined rules as csv, get mined rules\(cq statistics
 .SH SYNOPSIS
 .B niaarm
 .RB [ \-h ]
 .RB [ \-v ]
 .B \-i\ \fIINPUT_FILE
 .RB [ \-o\ \fIOUTPUT_FILE ]
 .B \-a\ \fIALGORITHM
```

### Comparing `niaarm-0.3.1/pyproject.toml` & `niaarm-0.3.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 [tool.poetry]
 name = "niaarm"
-version = "0.3.1"
+version = "0.3.2"
 description = "A minimalistic framework for numerical association rule mining"
 authors = ["Žiga Stupan <ziga.stupan1@student.um.si>", "Iztok Fister Jr. <iztok@iztok-jr-fister.eu>"]
+keywords = ['association rule mining', 'data science', 'numerical association rule mining', 'preprocessing', 'visualization']
+homepage = "https://github.com/firefly-cpp/NiaARM"
+repository = "https://github.com/firefly-cpp/NiaARM"
 readme = "README.md"
 
 include = [
     { path="LICENSE", format="sdist" },
     { path="CHANGELOG.md", format="sdist" },
     { path="niaarm.1", format="sdist" },
 ]
```

### Comparing `niaarm-0.3.1/setup.py` & `niaarm-0.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,22 +20,22 @@
           'sphinxcontrib-bibtex>=2.4.1,<3.0.0']}
 
 entry_points = \
 {'console_scripts': ['niaarm = niaarm.cli:main']}
 
 setup_kwargs = {
     'name': 'niaarm',
-    'version': '0.3.1',
+    'version': '0.3.2',
     'description': 'A minimalistic framework for numerical association rule mining',
     'long_description': '<p align="center">\n  <img alt="logo" width="300" src="https://raw.githubusercontent.com/firefly-cpp/NiaARM/main/.github/images/logo.png">\n</p>\n\n---\n\n# NiaARM - A minimalistic framework for Numerical Association Rule Mining\n\n---\n[![PyPI Version](https://img.shields.io/pypi/v/niaarm.svg)](https://pypi.python.org/pypi/niaarm)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/niaarm.svg)\n![PyPI - Downloads](https://img.shields.io/pypi/dm/niaarm.svg)\n[![Downloads](https://pepy.tech/badge/niaarm)](https://pepy.tech/project/niaarm)\n[![GitHub license](https://img.shields.io/github/license/firefly-cpp/niaarm.svg)](https://github.com/firefly-cpp/NiaARM/blob/main/LICENSE)\n![GitHub commit activity](https://img.shields.io/github/commit-activity/w/firefly-cpp/niaarm.svg)\n[![Average time to resolve an issue](http://isitmaintained.com/badge/resolution/firefly-cpp/niaarm.svg)](http://isitmaintained.com/project/firefly-cpp/niaarm "Average time to resolve an issue")\n[![Fedora package](https://img.shields.io/fedora/v/python3-niaarm?color=blue&label=Fedora%20Linux&logo=fedora)](https://src.fedoraproject.org/rpms/python-niaarm)\n[![AUR package](https://img.shields.io/aur/version/python-niaarm?color=blue&label=Arch%20Linux&logo=arch-linux)](https://aur.archlinux.org/packages/python-niaarm)\n[![DOI](https://joss.theoj.org/papers/10.21105/joss.04448/status.svg)](https://doi.org/10.21105/joss.04448)\n\n\nNiaARM is a framework for Association Rule Mining based on nature-inspired algorithms for optimization. The framework is written fully in Python and runs on all platforms. NiaARM allows users to preprocess the data in a transaction database automatically, to search for association rules and provide a pretty output of the rules found. This framework also supports integral and real-valued types of attributes besides the categorical ones. Mining the association rules is defined as an optimization problem, and solved using the nature-inspired algorithms that come from the related framework called [NiaPy](https://github.com/NiaOrg/NiaPy).\n\n* **Documentation:** https://niaarm.readthedocs.io/en/latest/\n* **Tested OS:** Windows, Ubuntu, Fedora, Alpine, Arch, macOS. **However, that does not mean it does not work on others**\n\n## Detailed insights\nThe current version includes (but is not limited to) the following functions:\n\n- loading datasets in CSV format,\n- preprocessing of data,\n- searching for association rules,\n- providing output of mined association rules,\n- generating statistics about mined association rules,\n- visualization of association rules,\n- association rule text mining (experimental).\n\n## Installation\n\n### pip\n\nInstall NiaARM with pip:\n\n```sh\npip install niaarm\n```\n\nTo install NiaARM on Alpine Linux, please enable Community repository and use:\n\n```sh\n$ apk add py3-niaarm\n```\n\nTo install NiaARM on Arch Linux, please use an [AUR helper](https://wiki.archlinux.org/title/AUR_helpers):\n\n```sh\n$ yay -Syyu python-niaarm\n```\n\nTo install NiaARM on Fedora, use:\n\n```sh\n$ dnf install python3-niaarm\n```\n\n## Usage\n\n### Loading data\n\nIn NiaARM, data loading is done via the `Dataset` class. There are two options for loading data:\n\n#### Option 1: From a pandas DataFrame (recommended)\n\n```python\nimport pandas as pd\nfrom niaarm import Dataset\n\n\ndf = pd.read_csv(\'datasets/Abalone.csv\')\n# preprocess data...\ndata = Dataset(df)\nprint(data) # printing the dataset will generate a feature report\n```\n\n#### Option 2: From CSV file directly\n\n```python\nfrom niaarm import Dataset\n\n\ndata = Dataset(\'datasets/Abalone.csv\')\nprint(data)\n```\n\n### Data Squashing\n\nOptionally, a preprocessing technique, called data squashing [5], can be applied. This will significantly reduce the number of transactions, while providing similar results to the original dataset.\n\n```python\nfrom niaarm import Dataset, squash\n\ndataset = Dataset(\'datasets/Abalone.csv\')\nsquashed = squash(dataset, threshold=0.9, similarity=\'euclidean\')\nprint(squashed)\n```\n\n### Mining association rules the easy way (recommended)\n\nAssociation rule mining can be easily performed using the `get_rules` function:\n\n```python\nfrom niaarm import Dataset, get_rules\nfrom niapy.algorithms.basic import DifferentialEvolution\n\ndata = Dataset("datasets/Abalone.csv")\n\nalgo = DifferentialEvolution(population_size=50, differential_weight=0.5, crossover_probability=0.9)\nmetrics = (\'support\', \'confidence\')\n\nrules, run_time = get_rules(data, algo, metrics, max_iters=30, logging=True)\n\nprint(rules) # Prints basic stats about the mined rules\nprint(f\'Run Time: {run_time}\')\nrules.to_csv(\'output.csv\')\n```\n\n### Mining association rules the hard way\n\nThe above example can be also be implemented using a more low level interface,\nwith the `NiaARM` class directly:\n\n```python\nfrom niaarm import NiaARM, Dataset\nfrom niapy.algorithms.basic import DifferentialEvolution\nfrom niapy.task import Task, OptimizationType\n\n\ndata = Dataset("datasets/Abalone.csv")\n\n# Create a problem:::\n# dimension represents the dimension of the problem;\n# features represent the list of features, while transactions depicts the list of transactions\n# metrics is a sequence of metrics to be taken into account when computing the fitness;\n# you can also pass in a dict of the shape {\'metric_name\': <weight of metric in range [0, 1]>};\n# when passing a sequence, the weights default to 1.\nproblem = NiaARM(data.dimension, data.features, data.transactions, metrics=(\'support\', \'confidence\'), logging=True)\n\n# build niapy task\ntask = Task(problem=problem, max_iters=30, optimization_type=OptimizationType.MAXIMIZATION)\n\n# use Differential Evolution (DE) algorithm from the NiaPy library\n# see full list of available algorithms: https://github.com/NiaOrg/NiaPy/blob/master/Algorithms.md\nalgo = DifferentialEvolution(population_size=50, differential_weight=0.5, crossover_probability=0.9)\n\n# run algorithm\nbest = algo.run(task=task)\n\n# sort rules\nproblem.rules.sort()\n\n# export all rules to csv\nproblem.rules.to_csv(\'output.csv\')\n```\n\n### Visualization\n\nThe framework currently supports the hill slopes visualization method presented in [4]. More visualization methods are planned\nto be implemented in future releases.\n\n```python\nfrom matplotlib import pyplot as plt\nfrom niaarm import Dataset, get_rules\nfrom niaarm.visualize import hill_slopes\n\ndataset = Dataset(\'datasets/Abalone.csv\')\nmetrics = (\'support\', \'confidence\')\nrules, _ = get_rules(dataset, \'DifferentialEvolution\', metrics, max_evals=1000, seed=1234)\nsome_rule = rules[150]\nhill_slopes(some_rule, dataset.transactions)\nplt.show()\n```\n\n<p>\n    <img alt="logo" src="https://raw.githubusercontent.com/firefly-cpp/NiaARM/main/.github/images/hill_slopes.png">\n</p>\n\n\n### Text Mining (Experimental)\n\nAn experimental implementation of association rule text mining using nature-inspired algorithms, based on ideas from [5]\nis also provided. The `niaarm.text` module contains the `Corpus` and `Document` classes for loading and preprocessing corpora,\na `TextRule` class, representing a text rule, and the `NiaARTM` class, implementing association rule text mining\nas a continuous optimization problem. The `get_text_rules` function, equivalent to `get_rules`, but for text mining, was also\nadded to the `niaarm.mine` module.\n\n```python\nimport pandas as pd\nfrom niaarm.text import Corpus\nfrom niaarm.mine import get_text_rules\nfrom niapy.algorithms.basic import ParticleSwarmOptimization\n\ndf = pd.read_json(\'datasets/text/artm_test_dataset.json\', orient=\'records\')\ndocuments = df[\'text\'].tolist()\ncorpus = Corpus.from_list(documents)\n\nalgorithm = ParticleSwarmOptimization(population_size=200, seed=123)\nmetrics = (\'support\', \'confidence\', \'aws\')\nrules, time = get_text_rules(corpus, max_terms=5, algorithm=algorithm, metrics=metrics, max_evals=10000, logging=True)\n\nif len(rules):\n    print(rules)\n    print(f\'Run time: {time:.2f}s\')\n    rules.to_csv(\'output.csv\')\nelse:\n    print(\'No rules generated\')\n    print(f\'Run time: {time:.2f}s\')\n```\n\n**Note:** You may need to download stopwords and the punkt tokenizer from nltk by running `import nltk; nltk.download(\'stopwords\'); nltk.download(\'punkt\')`.\n\nFor a full list of examples see the [examples folder](https://github.com/firefly-cpp/NiaARM/tree/main/examples)\nin the GitHub repository.\n\n### Command line interface\n\nWe provide a simple command line interface, which allows you to easily\nmine association rules on any input dataset, output them to a csv file and/or perform\na simple statistical analysis on them.\n\n```shell\nniaarm -h\n```\n\n```\nusage: niaarm [-h] [-v] -i INPUT_FILE [-o OUTPUT_FILE] -a ALGORITHM [-s SEED]\n              [--max-evals MAX_EVALS] [--max-iters MAX_ITERS] --metrics\n              METRICS [METRICS ...] [--weights WEIGHTS [WEIGHTS ...]] [--log]\n              [--show-stats]\n\nPerform ARM, output mined rules as csv, get mined rules\' statistics\n\noptions:\n  -h, --help            show this help message and exit\n  -v, --version         show program\'s version number and exit\n  -i INPUT_FILE, --input-file INPUT_FILE\n                        Input file containing a csv dataset\n  -o OUTPUT_FILE, --output-file OUTPUT_FILE\n                        Output file for mined rules\n  -a ALGORITHM, --algorithm ALGORITHM\n                        Algorithm to use (niapy class name, e.g.\n                        DifferentialEvolution)\n  -s SEED, --seed SEED  Seed for the algorithm\'s random number generator\n  --max-evals MAX_EVALS\n                        Maximum number of fitness function evaluations\n  --max-iters MAX_ITERS\n                        Maximum number of iterations\n  --metrics METRICS [METRICS ...]\n                        Metrics to use in the fitness function.\n  --weights WEIGHTS [WEIGHTS ...]\n                        Weights in range [0, 1] corresponding to --metrics\n  --log                 Enable logging of fitness improvements\n  --show-stats          Display stats about mined rules\n```\nNote: The CLI script can also run as a python module (`python -m niaarm ...`)\n\n## Reference Papers:\n\nIdeas are based on the following research papers:\n\n[1] I. Fister Jr., A. Iglesias, A. Gálvez, J. Del Ser, E. Osaba, I Fister. [Differential evolution for association rule mining using categorical and numerical attributes](http://www.iztok-jr-fister.eu/static/publications/231.pdf) In: Intelligent data engineering and automated learning - IDEAL 2018, pp. 79-88, 2018.\n\n[2] I. Fister Jr., V. Podgorelec, I. Fister. [Improved Nature-Inspired Algorithms for Numeric Association Rule Mining](https://link.springer.com/chapter/10.1007/978-3-030-68154-8_19). In: Vasant P., Zelinka I., Weber GW. (eds) Intelligent Computing and Optimization. ICO 2020. Advances in Intelligent Systems and Computing, vol 1324. Springer, Cham.\n\n[3] I. Fister Jr., I. Fister [A brief overview of swarm intelligence-based algorithms for numerical association rule mining](https://arxiv.org/abs/2010.15524). arXiv preprint arXiv:2010.15524 (2020).\n\n[4] Fister, I. et al. (2020). [Visualization of Numerical Association Rules by Hill Slopes](http://www.iztok-jr-fister.eu/static/publications/280.pdf).\n    In: Analide, C., Novais, P., Camacho, D., Yin, H. (eds) Intelligent Data Engineering and Automated Learning – IDEAL 2020.\n    IDEAL 2020. Lecture Notes in Computer Science(), vol 12489. Springer, Cham. https://doi.org/10.1007/978-3-030-62362-3_10\n\n[5] I. Fister, S. Deb, I. Fister, [Population-based metaheuristics for Association Rule Text Mining](http://www.iztok-jr-fister.eu/static/publications/260.pdf),\n    In: Proceedings of the 2020 4th International Conference on Intelligent Systems, Metaheuristics & Swarm Intelligence,\n    New York, NY, USA, mar. 2020, pp. 19–23. doi: [10.1145/3396474.3396493](https://dl.acm.org/doi/10.1145/3396474.3396493).\n\n[6] I. Fister, I. Fister Jr., D. Novak and D. Verber, [Data squashing as preprocessing in association rule mining](https://iztok-jr-fister.eu/static/publications/300.pdf), 2022 IEEE Symposium Series on Computational Intelligence (SSCI), Singapore, Singapore, 2022, pp. 1720-1725, doi: [10.1109/SSCI51031.2022.10022240](https://doi.org/10.1109/SSCI51031.2022.10022240).\n\n## License\n\nThis package is distributed under the MIT License. This license can be found online at <http://www.opensource.org/licenses/MIT>.\n\n## Disclaimer\n\nThis framework is provided as-is, and there are no guarantees that it fits your purposes or that it is bug-free. Use it at your own risk!\n\n## Cite us\n\nStupan, Ž., & Fister Jr., I. (2022). [NiaARM: A minimalistic framework for Numerical Association Rule Mining](https://www.theoj.org/joss-papers/joss.04448/10.21105.joss.04448.pdf). Journal of Open Source Software, 7(77), 4448.\n',
     'author': 'Žiga Stupan',
     'author_email': 'ziga.stupan1@student.um.si',
     'maintainer': None,
     'maintainer_email': None,
-    'url': None,
+    'url': 'https://github.com/firefly-cpp/NiaARM',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'entry_points': entry_points,
     'python_requires': '>=3.7,<4.0',
 }
```

### Comparing `niaarm-0.3.1/PKG-INFO` & `niaarm-0.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.1
 Name: niaarm
-Version: 0.3.1
+Version: 0.3.2
 Summary: A minimalistic framework for numerical association rule mining
+Home-page: https://github.com/firefly-cpp/NiaARM
+Keywords: association rule mining,data science,numerical association rule mining,preprocessing,visualization
 Author: Žiga Stupan
 Author-email: ziga.stupan1@student.um.si
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -16,14 +18,15 @@
 Requires-Dist: nltk (>=3.7,<4.0)
 Requires-Dist: numpy (>=1.21.5,<2.0.0); python_version >= "3.7" and python_version < "3.11"
 Requires-Dist: numpy (>=1.22.3,<2.0.0); python_version >= "3.11" and python_version < "4.0"
 Requires-Dist: pandas (>=1.3.5,<2.0.0); python_full_version >= "3.7.1" and python_version < "3.8"
 Requires-Dist: pandas (>=1.4.0,<2.0.0); python_version >= "3.8" and python_version < "4.0"
 Requires-Dist: sphinx-rtd-theme (>=1.0.0,<2.0.0); extra == "docs"
 Requires-Dist: sphinxcontrib-bibtex (>=2.4.1,<3.0.0); extra == "docs"
+Project-URL: Repository, https://github.com/firefly-cpp/NiaARM
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img alt="logo" width="300" src="https://raw.githubusercontent.com/firefly-cpp/NiaARM/main/.github/images/logo.png">
 </p>
 
 ---
```

