# Comparing `tmp/parameterspace-0.9.0.tar.gz` & `tmp/parameterspace-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parameterspace-0.9.0.tar", max compression
+gzip compressed data, was "parameterspace-0.9.1.tar", max compression
```

## Comparing `parameterspace-0.9.0.tar` & `parameterspace-0.9.1.tar`

### file list

```diff
@@ -1,29 +1,28 @@
--rw-r--r--   0        0        0    11482 2023-02-22 09:47:52.000000 parameterspace-0.9.0/LICENSE
--rw-r--r--   0        0        0     4563 2023-02-22 09:47:52.000000 parameterspace-0.9.0/README.md
--rw-r--r--   0        0        0      444 2023-02-22 09:47:52.000000 parameterspace-0.9.0/parameterspace/__init__.py
--rw-r--r--   0        0        0     1552 2023-02-22 09:47:52.000000 parameterspace-0.9.0/parameterspace/base.py
--rw-r--r--   0        0        0     4708 2023-02-22 09:47:52.000000 parameterspace-0.9.0/parameterspace/condition.py
--rw-r--r--   0        0        0     7778 2023-02-22 09:47:52.000000 parameterspace-0.9.0/parameterspace/configspace_utils.py
--rw-r--r--   0        0        0      590 2023-02-22 09:47:52.000000 parameterspace-0.9.0/parameterspace/parameters/__init__.py
--rw-r--r--   0        0        0     7043 2023-02-22 09:47:52.000000 parameterspace-0.9.0/parameterspace/parameters/base.py
--rw-r--r--   0        0        0     2261 2023-02-22 09:47:52.000000 parameterspace-0.9.0/parameterspace/parameters/categorical.py
--rw-r--r--   0        0        0     2853 2023-02-22 09:47:52.000000 parameterspace-0.9.0/parameterspace/parameters/continuous.py
--rw-r--r--   0        0        0     3008 2023-02-22 09:47:52.000000 parameterspace-0.9.0/parameterspace/parameters/integer.py
--rw-r--r--   0        0        0     2163 2023-02-22 09:47:52.000000 parameterspace-0.9.0/parameterspace/parameters/ordinal.py
--rw-r--r--   0        0        0    20212 2023-02-22 09:47:52.000000 parameterspace-0.9.0/parameterspace/parameterspace.py
--rw-r--r--   0        0        0      425 2023-02-22 09:47:52.000000 parameterspace-0.9.0/parameterspace/priors/__init__.py
--rw-r--r--   0        0        0     2489 2023-02-22 09:47:52.000000 parameterspace-0.9.0/parameterspace/priors/base.py
--rw-r--r--   0        0        0     1322 2023-02-22 09:47:52.000000 parameterspace-0.9.0/parameterspace/priors/beta.py
--rw-r--r--   0        0        0     2833 2023-02-22 09:47:52.000000 parameterspace-0.9.0/parameterspace/priors/categorical.py
--rw-r--r--   0        0        0     1523 2023-02-22 09:47:52.000000 parameterspace-0.9.0/parameterspace/priors/truncated_normal.py
--rw-r--r--   0        0        0     1391 2023-02-22 09:47:52.000000 parameterspace-0.9.0/parameterspace/priors/uniform.py
--rw-r--r--   0        0        0        0 2023-02-22 09:47:52.000000 parameterspace-0.9.0/parameterspace/py.typed
--rw-r--r--   0        0        0      454 2023-02-22 09:47:52.000000 parameterspace-0.9.0/parameterspace/transformations/__init__.py
--rw-r--r--   0        0        0     2966 2023-02-22 09:47:52.000000 parameterspace-0.9.0/parameterspace/transformations/base.py
--rw-r--r--   0        0        0     1839 2023-02-22 09:47:52.000000 parameterspace-0.9.0/parameterspace/transformations/categorical.py
--rw-r--r--   0        0        0     3324 2023-02-22 09:47:52.000000 parameterspace-0.9.0/parameterspace/transformations/log_zero_one.py
--rw-r--r--   0        0        0     2229 2023-02-22 09:47:52.000000 parameterspace-0.9.0/parameterspace/transformations/zero_one.py
--rw-r--r--   0        0        0     3499 2023-02-22 09:47:52.000000 parameterspace-0.9.0/parameterspace/utils.py
--rw-r--r--   0        0        0     3005 2023-02-22 09:47:52.000000 parameterspace-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     5518 1970-01-01 00:00:00.000000 parameterspace-0.9.0/setup.py
--rw-r--r--   0        0        0     5574 1970-01-01 00:00:00.000000 parameterspace-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0    11482 2023-05-23 11:01:28.000000 parameterspace-0.9.1/LICENSE
+-rw-r--r--   0        0        0     4563 2023-05-23 11:01:28.000000 parameterspace-0.9.1/README.md
+-rw-r--r--   0        0        0      444 2023-05-23 11:01:28.000000 parameterspace-0.9.1/parameterspace/__init__.py
+-rw-r--r--   0        0        0     1552 2023-05-23 11:01:28.000000 parameterspace-0.9.1/parameterspace/base.py
+-rw-r--r--   0        0        0     4708 2023-05-23 11:01:28.000000 parameterspace-0.9.1/parameterspace/condition.py
+-rw-r--r--   0        0        0     7778 2023-05-23 11:01:28.000000 parameterspace-0.9.1/parameterspace/configspace_utils.py
+-rw-r--r--   0        0        0      590 2023-05-23 11:01:28.000000 parameterspace-0.9.1/parameterspace/parameters/__init__.py
+-rw-r--r--   0        0        0     7043 2023-05-23 11:01:28.000000 parameterspace-0.9.1/parameterspace/parameters/base.py
+-rw-r--r--   0        0        0     2261 2023-05-23 11:01:28.000000 parameterspace-0.9.1/parameterspace/parameters/categorical.py
+-rw-r--r--   0        0        0     2853 2023-05-23 11:01:28.000000 parameterspace-0.9.1/parameterspace/parameters/continuous.py
+-rw-r--r--   0        0        0     3008 2023-05-23 11:01:28.000000 parameterspace-0.9.1/parameterspace/parameters/integer.py
+-rw-r--r--   0        0        0     2163 2023-05-23 11:01:28.000000 parameterspace-0.9.1/parameterspace/parameters/ordinal.py
+-rw-r--r--   0        0        0    20580 2023-05-23 11:01:28.000000 parameterspace-0.9.1/parameterspace/parameterspace.py
+-rw-r--r--   0        0        0      425 2023-05-23 11:01:28.000000 parameterspace-0.9.1/parameterspace/priors/__init__.py
+-rw-r--r--   0        0        0     2489 2023-05-23 11:01:28.000000 parameterspace-0.9.1/parameterspace/priors/base.py
+-rw-r--r--   0        0        0     1322 2023-05-23 11:01:28.000000 parameterspace-0.9.1/parameterspace/priors/beta.py
+-rw-r--r--   0        0        0     2833 2023-05-23 11:01:28.000000 parameterspace-0.9.1/parameterspace/priors/categorical.py
+-rw-r--r--   0        0        0     1523 2023-05-23 11:01:28.000000 parameterspace-0.9.1/parameterspace/priors/truncated_normal.py
+-rw-r--r--   0        0        0     1391 2023-05-23 11:01:28.000000 parameterspace-0.9.1/parameterspace/priors/uniform.py
+-rw-r--r--   0        0        0        0 2023-05-23 11:01:28.000000 parameterspace-0.9.1/parameterspace/py.typed
+-rw-r--r--   0        0        0      454 2023-05-23 11:01:28.000000 parameterspace-0.9.1/parameterspace/transformations/__init__.py
+-rw-r--r--   0        0        0     2966 2023-05-23 11:01:28.000000 parameterspace-0.9.1/parameterspace/transformations/base.py
+-rw-r--r--   0        0        0     1839 2023-05-23 11:01:28.000000 parameterspace-0.9.1/parameterspace/transformations/categorical.py
+-rw-r--r--   0        0        0     3324 2023-05-23 11:01:28.000000 parameterspace-0.9.1/parameterspace/transformations/log_zero_one.py
+-rw-r--r--   0        0        0     2229 2023-05-23 11:01:28.000000 parameterspace-0.9.1/parameterspace/transformations/zero_one.py
+-rw-r--r--   0        0        0     3499 2023-05-23 11:01:28.000000 parameterspace-0.9.1/parameterspace/utils.py
+-rw-r--r--   0        0        0     3005 2023-05-23 11:01:28.000000 parameterspace-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     5375 1970-01-01 00:00:00.000000 parameterspace-0.9.1/PKG-INFO
```

### Comparing `parameterspace-0.9.0/LICENSE` & `parameterspace-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `parameterspace-0.9.0/README.md` & `parameterspace-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `parameterspace-0.9.0/parameterspace/base.py` & `parameterspace-0.9.1/parameterspace/base.py`

 * *Files identical despite different names*

### Comparing `parameterspace-0.9.0/parameterspace/condition.py` & `parameterspace-0.9.1/parameterspace/condition.py`

 * *Files identical despite different names*

### Comparing `parameterspace-0.9.0/parameterspace/configspace_utils.py` & `parameterspace-0.9.1/parameterspace/configspace_utils.py`

 * *Files identical despite different names*

### Comparing `parameterspace-0.9.0/parameterspace/parameters/__init__.py` & `parameterspace-0.9.1/parameterspace/parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `parameterspace-0.9.0/parameterspace/parameters/base.py` & `parameterspace-0.9.1/parameterspace/parameters/base.py`

 * *Files identical despite different names*

### Comparing `parameterspace-0.9.0/parameterspace/parameters/categorical.py` & `parameterspace-0.9.1/parameterspace/parameters/categorical.py`

 * *Files identical despite different names*

### Comparing `parameterspace-0.9.0/parameterspace/parameters/continuous.py` & `parameterspace-0.9.1/parameterspace/parameters/continuous.py`

 * *Files identical despite different names*

### Comparing `parameterspace-0.9.0/parameterspace/parameters/integer.py` & `parameterspace-0.9.1/parameterspace/parameters/integer.py`

 * *Files identical despite different names*

### Comparing `parameterspace-0.9.0/parameterspace/parameters/ordinal.py` & `parameterspace-0.9.1/parameterspace/parameters/ordinal.py`

 * *Files identical despite different names*

### Comparing `parameterspace-0.9.0/parameterspace/parameterspace.py` & `parameterspace-0.9.1/parameterspace/parameterspace.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 from parameterspace.base import SearchSpace
 from parameterspace.condition import Condition
 from parameterspace.parameters import (
     CategoricalParameter,
     ContinuousParameter,
     IntegerParameter,
+    OrdinalParameter,
 )
 from parameterspace.parameters.base import BaseParameter
 
 
 # pylint: disable=too-many-public-methods
 class ParameterSpace(SearchSpace):
     """Class representing a parameter space that allows to sampling, converting and
@@ -521,36 +522,45 @@
 
             if isinstance(parameter, IntegerParameter):
                 type_str = "Integer"
                 values_str = f"$[{parameter.bounds[0]}, {parameter.bounds[1]}]$"
                 transformation_str = "Log" if "Log" in transformation_name else ""
                 prior_str = prior_name
 
-            if isinstance(parameter, ContinuousParameter):
+            elif isinstance(parameter, ContinuousParameter):
                 type_str = "Float"
                 prior_str = prior_name
 
                 if "Log" in transformation_name:
                     transformation_str = "Log"
                     lower_bound = num2tex(parameter.bounds[0], precision=2)
                     upper_bound = num2tex(parameter.bounds[1], precision=2)
                     values_str = f"$[{lower_bound}, {upper_bound}]$"
                 else:
                     transformation_str = " "
                     values_str = f"$[{parameter.bounds[0]}, {parameter.bounds[1]}]$"
 
-            if isinstance(parameter, CategoricalParameter):
+            elif isinstance(parameter, CategoricalParameter):
                 type_str = "Categorical"
                 values_str = "[" + ", ".join(parameter.values) + "]"
                 transformation_str = " "
                 prior_probs = parameter._prior.probabilities
                 prior_str = (
                     "[" + ",".join(map(lambda p: f"{p:3.2f}", prior_probs)) + "]"
                 )
 
+            elif isinstance(parameter, OrdinalParameter):
+                type_str = "Ordinal"
+                values_str = "[" + ", ".join(parameter.values) + "]"
+                transformation_str = " "
+                prior_str = prior_name
+
+            else:
+                raise ValueError(f"Unknown parameter type {type(parameter)}")
+
             latex_strs.append(
                 " & ".join(
                     [name_str, type_str, values_str, transformation_str, prior_str]
                 )
                 + "\\\\"
             )
```

### Comparing `parameterspace-0.9.0/parameterspace/priors/base.py` & `parameterspace-0.9.1/parameterspace/priors/base.py`

 * *Files identical despite different names*

### Comparing `parameterspace-0.9.0/parameterspace/priors/beta.py` & `parameterspace-0.9.1/parameterspace/priors/beta.py`

 * *Files identical despite different names*

### Comparing `parameterspace-0.9.0/parameterspace/priors/categorical.py` & `parameterspace-0.9.1/parameterspace/priors/categorical.py`

 * *Files identical despite different names*

### Comparing `parameterspace-0.9.0/parameterspace/priors/truncated_normal.py` & `parameterspace-0.9.1/parameterspace/priors/truncated_normal.py`

 * *Files identical despite different names*

### Comparing `parameterspace-0.9.0/parameterspace/priors/uniform.py` & `parameterspace-0.9.1/parameterspace/priors/uniform.py`

 * *Files identical despite different names*

### Comparing `parameterspace-0.9.0/parameterspace/transformations/base.py` & `parameterspace-0.9.1/parameterspace/transformations/base.py`

 * *Files identical despite different names*

### Comparing `parameterspace-0.9.0/parameterspace/transformations/categorical.py` & `parameterspace-0.9.1/parameterspace/transformations/categorical.py`

 * *Files identical despite different names*

### Comparing `parameterspace-0.9.0/parameterspace/transformations/log_zero_one.py` & `parameterspace-0.9.1/parameterspace/transformations/log_zero_one.py`

 * *Files identical despite different names*

### Comparing `parameterspace-0.9.0/parameterspace/transformations/zero_one.py` & `parameterspace-0.9.1/parameterspace/transformations/zero_one.py`

 * *Files identical despite different names*

### Comparing `parameterspace-0.9.0/parameterspace/utils.py` & `parameterspace-0.9.1/parameterspace/utils.py`

 * *Files identical despite different names*

### Comparing `parameterspace-0.9.0/pyproject.toml` & `parameterspace-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "parameterspace"
-version = "0.9.0"
+version = "0.9.1"
 description = "Parametrized hierarchical spaces with flexible priors and transformations."
 readme = "README.md"
 repository = "https://github.com/boschresearch/parameterspace"
 authors = ["Bosch Center for AI, Robert Bosch GmbH"]
 license = "Apache-2.0"
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `parameterspace-0.9.0/setup.py` & `parameterspace-0.9.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,147 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: parameterspace
+Version: 0.9.1
+Summary: Parametrized hierarchical spaces with flexible priors and transformations.
+Home-page: https://github.com/boschresearch/parameterspace
+License: Apache-2.0
+Author: Bosch Center for AI, Robert Bosch GmbH
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: examples
+Requires-Dist: numpy (>=1.22.0)
+Requires-Dist: scipy (>=1.6.0)
+Project-URL: Repository, https://github.com/boschresearch/parameterspace
+Description-Content-Type: text/markdown
 
-packages = \
-['parameterspace',
- 'parameterspace.parameters',
- 'parameterspace.priors',
- 'parameterspace.transformations']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['numpy>=1.22.0', 'scipy>=1.6.0']
-
-setup_kwargs = {
-    'name': 'parameterspace',
-    'version': '0.9.0',
-    'description': 'Parametrized hierarchical spaces with flexible priors and transformations.',
-    'long_description': '# ParameterSpace\n\n[![Actions Status](https://github.com/boschresearch/parameterspace/workflows/ci-cd-pipeline/badge.svg)](https://github.com/boschresearch/parameterspace/actions)\n[![PyPI - Wheel](https://img.shields.io/pypi/wheel/parameterspace)](https://pypi.org/project/parameterspace/)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/parameterspace)](https://pypi.org/project/parameterspace/)\n[![License: Apache-2.0](https://img.shields.io/github/license/boschresearch/parameterspace)](https://github.com/boschresearch/parameterspace/blob/main/LICENSE)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n**Contents:**\n\n- [About](#about)\n- [Installation](#installation)\n- [Development](#development)\n  - [Prerequisites](#prerequisites)\n  - [Setup environment](#setup-environment)\n  - [Running Tests](#running-tests)\n  - [Building Documentation](#building-documentation)\n- [License](#license)\n\n## About\n\nA package to define parameter spaces consisting of mixed types (continuous, integer,\ncategorical) with conditions and priors. It allows for easy specification of the\nparameters and their dependencies. The `ParameterSpace` object can then be used to\nsample random configurations from the prior and convert any valid configuration\ninto a numerical representation. This numerical representation has the following\nproperties:\n\n- it results in a Numpy `ndarray` of type `float64`\n- transformed representation between 0 and 1 (uniform) including integers, ordinal and\n  categorical parameters\n- inactive parameters are masked as `numpy.nan` values\n\nThis allows to easily use optimizers that expect continuous domains to be used on more\ncomplicated problems because `parameterspace` can convert any numerical vector\nrepresentation inside the unit hypercube into a valid configuration. The function might\nnot be smooth, but for robust methods (like genetic algorithms/evolutionary strategies)\nthis might still be valuable.\n\nThis software is a research prototype. The software is not ready for production use. It\nhas neither been developed nor tested for a specific use case. However, the license\nconditions of the applicable Open Source licenses allow you to adapt the software to\nyour needs. Before using it in a safety relevant setting, make sure that the software\nfulfills your requirements and adjust it according to any applicable safety standards\n(e.g. ISO 26262).\n\n## Documentation\n\n**Visit [boschresearch.github.io/parameterspace](https://boschresearch.github.io/parameterspace/)**\n\n\n## Installation\n\nThe `parameterspace` package can be installed from [pypi.org](https://pypi.org):\n\n```\npip install parameterspace\n```\n\n## Development\n\n### Prerequisites\n\n- Python >= 3.8\n- [Poetry](https://python-poetry.org/docs/#installation)\n\n### Setup environment\n\nTo install the package and its dependencies for development run:\n\n```\npoetry install\n```\n\nOptionally install [pre-commit](https://pre-commit.com) hooks to check code standards\nbefore committing changes:\n\n```\npoetry run pre-commit install\n```\n\n### Running Tests\n\nThe tests are located in the `./tests` folder. The [pytest](https://pytest.org)\nframework is used for running them. To run the tests:\n\n```\npoetry run pytest ./tests\n```\n\n### Building Documentation\n\nTo built documentation run from the repository root:\n\n```\npoetry run mkdocs build --clean\n```\n\nFor serving it locally while working on the documentation run:\n\n```\npoetry run mkdocs serve\n```\n\n## Architectural Decision Records\n\n### Parameter Names\n\n**In the context of** naming parameters and using their name to fix them to constant\nvalues or condition on them via `lambda` expressions,\n**facing that** only valid Python variable names can be used in conditions, and that\nfixing parameters that do not have a valid parameter name can only be done like\n`fix(**{"invalid-variable:name": "const"})`\n**we decided for** requiring all parameter names to be valid Python variable names\n**to achieve** early failure and communication of that convention to avoid surprises\nwhen fixing and using conditions down the line, accepting that this rules out common\nparameter names like `lambda` and might require explicit translation between from and to\ncontexts that require incompatible names (e.g. predefined benchmarks).\n\n## License\n\n`parameterspace` is open-sourced under the Apache-2.0 license. See the\n[LICENSE](LICENSE) file for details.\n\nFor a list of other open source components included in `parameterspace`, see the file\n[3rd-party-licenses.txt](3rd-party-licenses.txt).\n',
-    'author': 'Bosch Center for AI, Robert Bosch GmbH',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/boschresearch/parameterspace',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+# ParameterSpace
 
+[![Actions Status](https://github.com/boschresearch/parameterspace/workflows/ci-cd-pipeline/badge.svg)](https://github.com/boschresearch/parameterspace/actions)
+[![PyPI - Wheel](https://img.shields.io/pypi/wheel/parameterspace)](https://pypi.org/project/parameterspace/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/parameterspace)](https://pypi.org/project/parameterspace/)
+[![License: Apache-2.0](https://img.shields.io/github/license/boschresearch/parameterspace)](https://github.com/boschresearch/parameterspace/blob/main/LICENSE)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+**Contents:**
+
+- [About](#about)
+- [Installation](#installation)
+- [Development](#development)
+  - [Prerequisites](#prerequisites)
+  - [Setup environment](#setup-environment)
+  - [Running Tests](#running-tests)
+  - [Building Documentation](#building-documentation)
+- [License](#license)
+
+## About
+
+A package to define parameter spaces consisting of mixed types (continuous, integer,
+categorical) with conditions and priors. It allows for easy specification of the
+parameters and their dependencies. The `ParameterSpace` object can then be used to
+sample random configurations from the prior and convert any valid configuration
+into a numerical representation. This numerical representation has the following
+properties:
+
+- it results in a Numpy `ndarray` of type `float64`
+- transformed representation between 0 and 1 (uniform) including integers, ordinal and
+  categorical parameters
+- inactive parameters are masked as `numpy.nan` values
+
+This allows to easily use optimizers that expect continuous domains to be used on more
+complicated problems because `parameterspace` can convert any numerical vector
+representation inside the unit hypercube into a valid configuration. The function might
+not be smooth, but for robust methods (like genetic algorithms/evolutionary strategies)
+this might still be valuable.
+
+This software is a research prototype. The software is not ready for production use. It
+has neither been developed nor tested for a specific use case. However, the license
+conditions of the applicable Open Source licenses allow you to adapt the software to
+your needs. Before using it in a safety relevant setting, make sure that the software
+fulfills your requirements and adjust it according to any applicable safety standards
+(e.g. ISO 26262).
+
+## Documentation
+
+**Visit [boschresearch.github.io/parameterspace](https://boschresearch.github.io/parameterspace/)**
+
+
+## Installation
+
+The `parameterspace` package can be installed from [pypi.org](https://pypi.org):
+
+```
+pip install parameterspace
+```
+
+## Development
+
+### Prerequisites
+
+- Python >= 3.8
+- [Poetry](https://python-poetry.org/docs/#installation)
+
+### Setup environment
+
+To install the package and its dependencies for development run:
+
+```
+poetry install
+```
+
+Optionally install [pre-commit](https://pre-commit.com) hooks to check code standards
+before committing changes:
+
+```
+poetry run pre-commit install
+```
+
+### Running Tests
+
+The tests are located in the `./tests` folder. The [pytest](https://pytest.org)
+framework is used for running them. To run the tests:
+
+```
+poetry run pytest ./tests
+```
+
+### Building Documentation
+
+To built documentation run from the repository root:
+
+```
+poetry run mkdocs build --clean
+```
+
+For serving it locally while working on the documentation run:
+
+```
+poetry run mkdocs serve
+```
+
+## Architectural Decision Records
+
+### Parameter Names
+
+**In the context of** naming parameters and using their name to fix them to constant
+values or condition on them via `lambda` expressions,
+**facing that** only valid Python variable names can be used in conditions, and that
+fixing parameters that do not have a valid parameter name can only be done like
+`fix(**{"invalid-variable:name": "const"})`
+**we decided for** requiring all parameter names to be valid Python variable names
+**to achieve** early failure and communication of that convention to avoid surprises
+when fixing and using conditions down the line, accepting that this rules out common
+parameter names like `lambda` and might require explicit translation between from and to
+contexts that require incompatible names (e.g. predefined benchmarks).
+
+## License
+
+`parameterspace` is open-sourced under the Apache-2.0 license. See the
+[LICENSE](LICENSE) file for details.
+
+For a list of other open source components included in `parameterspace`, see the file
+[3rd-party-licenses.txt](3rd-party-licenses.txt).
 
-setup(**setup_kwargs)
```

