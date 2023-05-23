# Comparing `tmp/jinja2_jsonschema-0.1.0.tar.gz` & `tmp/jinja2_jsonschema-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jinja2_jsonschema-0.1.0.tar", max compression
+gzip compressed data, was "jinja2_jsonschema-0.2.0.tar", max compression
```

## Comparing `jinja2_jsonschema-0.1.0.tar` & `jinja2_jsonschema-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1076 2023-05-17 12:07:26.429957 jinja2_jsonschema-0.1.0/LICENSE
--rw-r--r--   0        0        0     4751 2023-05-17 12:07:26.429957 jinja2_jsonschema-0.1.0/README.md
--rw-r--r--   0        0        0     2309 2023-05-17 12:07:26.429957 jinja2_jsonschema-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       78 2023-05-17 12:07:26.429957 jinja2_jsonschema-0.1.0/src/jinja2_jsonschema/__init__.py
--rw-r--r--   0        0        0      657 2023-05-17 12:07:26.429957 jinja2_jsonschema-0.1.0/src/jinja2_jsonschema/errors.py
--rw-r--r--   0        0        0     4202 2023-05-17 12:07:26.429957 jinja2_jsonschema-0.1.0/src/jinja2_jsonschema/extension.py
--rw-r--r--   0        0        0        0 2023-05-17 12:07:26.429957 jinja2_jsonschema-0.1.0/src/jinja2_jsonschema/py.typed
--rw-r--r--   0        0        0     6128 1970-01-01 00:00:00.000000 jinja2_jsonschema-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-05-23 07:53:56.812785 jinja2_jsonschema-0.2.0/LICENSE
+-rw-r--r--   0        0        0     7095 2023-05-23 07:53:56.812785 jinja2_jsonschema-0.2.0/README.md
+-rw-r--r--   0        0        0     2313 2023-05-23 07:53:56.812785 jinja2_jsonschema-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       78 2023-05-23 07:53:56.812785 jinja2_jsonschema-0.2.0/src/jinja2_jsonschema/__init__.py
+-rw-r--r--   0        0        0      657 2023-05-23 07:53:56.816785 jinja2_jsonschema-0.2.0/src/jinja2_jsonschema/errors.py
+-rw-r--r--   0        0        0     4617 2023-05-23 07:53:56.816785 jinja2_jsonschema-0.2.0/src/jinja2_jsonschema/extension.py
+-rw-r--r--   0        0        0        0 2023-05-23 07:53:56.816785 jinja2_jsonschema-0.2.0/src/jinja2_jsonschema/py.typed
+-rw-r--r--   0        0        0     8222 1970-01-01 00:00:00.000000 jinja2_jsonschema-0.2.0/PKG-INFO
```

### Comparing `jinja2_jsonschema-0.1.0/LICENSE` & `jinja2_jsonschema-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jinja2_jsonschema-0.1.0/README.md` & `jinja2_jsonschema-0.2.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # JSON Schema Validation within Jinja2 Templates
 
 [![CI](https://github.com/copier-org/jinja2-jsonschema/workflows/tests/badge.svg)](https://github.com/copier-org/jinja2-jsonschema/actions?query=branch%3Amain)
 ![Python versions](https://img.shields.io/pypi/pyversions/jinja2-jsonschema?logo=python&logoColor=%23959DA5)
 [![PyPI](https://img.shields.io/pypi/v/jinja2-jsonschema?logo=pypi&logoColor=%23959DA5)](https://pypi.org/project/jinja2-jsonschema)
 [![Code style: Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Linter: Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/charliermarsh/ruff)
+[![Linter: Ruff](https://img.shields.io/badge/-Ruff-261230.svg?labelColor=grey&logo=ruff&logoColor=D7FF64)](https://github.com/charliermarsh/ruff)
 [![Type-checker: mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org)
 
-A [Jinja2 extension][jinja-extensions] providing a [Jinja2 filter][jinja-filter] for validating data against a JSON/YAML schema within [Jinja2][jinja] templates.
+A [Jinja2 extension][jinja-extensions] providing a [Jinja2 filter][jinja-filter] and a [Jinja2 test][jinja-test] for validating data against a JSON/YAML schema within [Jinja2][jinja] templates.
 
 ## Installation
 
 * With [`pip`](https://pip.pypa.io):
 
     ```shell
     pip install jinja2-jsonschema
@@ -45,56 +45,113 @@
 
     # ... or with YAML support
     pipx inject PACKAGE jinja2-jsonschema[yaml]
     ```
 
 ## Usage
 
-The extension provides a Jinja2 filter which receives a schema file path or schema object as input and returns a [`jsonschema.ValidationError`][python-jsonschema-validationerror] object when validation fails and an empty string (`""`) otherwise. The [JSON Schema dialect][jsonschema-dialect] is inferred from the `$schema` field in the JSON Schema document and, when omitted, defaults to the [latest dialect supported by the installed `jsonschema` library][python-jsonschema-features]. Both local and remote schemas are supported including [schema references][jsonschema-ref] and [JSON Pointers][jsonschema-jsonpointer].
+The extension provides:
+
+* A Jinja2 filter which receives a schema file path or schema object as input and returns a [`jsonschema.ValidationError`][python-jsonschema-validationerror] object when validation fails and an empty string (`""`) otherwise.
+* A Jinja2 test which receives a schema file path or schema object as input and returns `False` when validation fails and `True` otherwise.
+
+The [JSON Schema dialect][jsonschema-dialect] is inferred from the `$schema` field in the JSON Schema document and, when omitted, defaults to the [latest dialect supported by the installed `jsonschema` library][python-jsonschema-features]. Both local and remote schemas are supported including [schema references][jsonschema-ref] and [JSON Pointers][jsonschema-jsonpointer].
 
 Local schema files are loaded via a [Jinja2 loader](https://jinja.palletsprojects.com/en/latest/api/#loaders) in which case configuring the Jinja2 environment with a loader is mandatory.
 
-Some example usage of the JSON Schema validation filter is this:
+Some example usage of the JSON Schema validation filter and test is this:
 
 ```python
 from jinja2 import Environment
 from jinja2 import FileSystemLoader
 
 
 env = Environment(
     # Register a loader (only necessary when using local schema files).
     loader=FileSystemLoader("/path/to/templates"),
     # Register the extension.
-    extensions=['jinja2_jsonschema.JsonSchemaExtension'],
+    extensions=["jinja2_jsonschema.JsonSchemaExtension"],
 )
 
 # Example using an inline schema object.
 template = env.from_string("{{ age | jsonschema({'type': 'integer', 'minimum': 0}) }}")
 template.render(age=30)  # OK
 template.render(age=-1)  # ERROR
+template = env.from_string("{{ age is jsonschema({'type': 'integer', 'minimum': 0}) }}")
+template.render(age=30)  # --> `True`
+template.render(age=-1)  # --> `False`
 
 # Example using a local schema file.
 template = env.from_string("{{ age | jsonschema('age.json') }}")
 template.render(age=30)  # OK
 template.render(age=-1)  # ERROR
+template = env.from_string("{{ age is jsonschema('age.json') }}")
+template.render(age=30)  # --> `True`
+template.render(age=-1)  # --> `False`
 
 # Example using a remote schema file.
 template = env.from_string("{{ age | jsonschema('https://example.com/age.json') }}")
 template.render(age=30)  # OK
 template.render(age=-1)  # ERROR
+template = env.from_string("{{ age is jsonschema('https://example.com/age.json') }}")
+template.render(age=30)  # --> `True`
+template.render(age=-1)  # --> `False`
+```
+
+## Usage with Copier
+
+The extension integrates nicely with [Copier][copier], e.g. for validating complex JSON/YAML answers in the Copier questionnaire. For this, add the extension as a [Jinja2 extension in `copier.yml`][copier-jinja-extensions] and use the Jinja2 filter in the `validator` field of a Copier [question][copier-questions]. For instance:
+
+```yaml
+_jinja_extensions:
+  - jinja2_jsonschema.JsonSchemaExtension
+
+complex_question:
+  type: json # or `yaml`
+  validator: "{{ complex_question | jsonschema('schemas/complex.json') }}"
+```
+
+In this example, a local schema file `schemas/complex.json` is used whose path is relative to the template root. To prevent copying schema files to the generated project, they should be either [excluded][copier-exclude]
+
+```diff
++_exclude:
++  - schemas/
+ _jinja_extensions:
+   - jinja2_jsonschema.JsonSchemaExtension
+```
+
+or the project template should be located in a [subdirectory][copier-subdirectory] such as `template/`:
+
+```diff
++_subdirectory_: template
+ _jinja_extensions:
+   - jinja2_jsonschema.JsonSchemaExtension
+```
+
+Finally, template consumers need to install the extension along with Copier. For instance with `pipx`:
+
+```shell
+pipx install copier
+pipx inject copier jinja2-jsonschema
 ```
 
 ## Contributions
 
 Contributions are always welcome via filing [issues](https://github.com/copier-org/jinja2-jsonschema/issues) or submitting [pull requests](https://github.com/copier-org/jinja2-jsonschema/pulls). Please check the [contribution guide][contribution-guide] for more details.
 
-[contribution-guide]: https://https://github.com/copier-org/jinja2-jsonschema/blob/main/CONTRIBUTING.md
+[contribution-guide]: https://github.com/copier-org/jinja2-jsonschema/blob/main/CONTRIBUTING.md
+[copier]: https://github.com/copier-org/copier
+[copier-exclude]: https://copier.readthedocs.io/en/stable/configuring/#exclude
+[copier-jinja-extensions]: https://copier.readthedocs.io/en/stable/configuring/#jinja_extensions
+[copier-questions]: https://copier.readthedocs.io/en/stable/configuring/#questions
+[copier-subdirectory]: https://copier.readthedocs.io/en/stable/configuring/#subdirectory
 [jinja]: https://jinja.palletsprojects.com
 [jinja-extensions]: https://jinja.palletsprojects.com/en/latest/extensions/
 [jinja-filter]: https://jinja.palletsprojects.com/en/latest/templates/#filters
+[jinja-test]: https://jinja.palletsprojects.com/en/latest/templates/#tests
 [jsonschema]: https://json-schema.org
 [jsonschema-dialect]: https://json-schema.org/understanding-json-schema/reference/schema.html#schema
 [jsonschema-ref]: https://json-schema.org/understanding-json-schema/structuring.html#ref
 [jsonschema-jsonpointer]: https://json-schema.org/understanding-json-schema/structuring.html#json-pointer
 [pdm]: https://pdm.fming.dev
 [pip]: https://pip.pypa.io
 [pipx]: https://pypa.github.io/pipx
```

### Comparing `jinja2_jsonschema-0.1.0/pyproject.toml` & `jinja2_jsonschema-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jinja2-jsonschema"
-version = "0.1.0"
+version = "0.2.0"
 description = "JSON/YAML schema validation within Jinja2 templates"
 license = "MIT"
 classifiers = [
   "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
@@ -43,15 +43,15 @@
 
 [tool.poetry.group.test.dependencies]
 pytest = ">=7.3.1"
 pytest-cov = ">=4.0.0"
 
 [tool.poetry.group.typing.dependencies]
 types-jsonschema = ">=4.0.0"
-types-pyyaml = ">=6.0.0"
+types-pyyaml = ">=6.0.12.10"
 typing-extensions = { version = ">=3.7.4", python = "<3.8" }
 
 [tool.black]
 target-version = ["py37"]
 
 [tool.isort]
 profile = "black"
```

### Comparing `jinja2_jsonschema-0.1.0/src/jinja2_jsonschema/errors.py` & `jinja2_jsonschema-0.2.0/src/jinja2_jsonschema/errors.py`

 * *Files identical despite different names*

### Comparing `jinja2_jsonschema-0.1.0/src/jinja2_jsonschema/extension.py` & `jinja2_jsonschema-0.2.0/src/jinja2_jsonschema/extension.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,27 +23,42 @@
     from typing import Literal
 else:  # pragma: no cover
     from typing_extensions import Literal
 
 __all__ = ["JsonSchemaExtension"]
 
 
-class JsonSchemaExtension(Extension):  # pylint: disable=abstract-method
+class JsonSchemaExtension(Extension):
     """Jinja2 extension for using JSON Schema within Jinja2 templates."""
 
     def __init__(self, environment: Environment) -> None:
         super().__init__(environment)
+
+        jsonschema_filter = _JsonSchemaFilter(environment)
+
         if "jsonschema" in environment.filters:
             warn(
                 'A filter named "jsonschema" already exists in the Jinja2 environment',
                 category=RuntimeWarning,
                 stacklevel=2,
             )
         else:
-            environment.filters["jsonschema"] = _JsonSchemaFilter(environment)
+            environment.filters["jsonschema"] = jsonschema_filter
+
+        def jsonschema_test(data: Any, schema: Union[str, _Schema]) -> bool:
+            return not jsonschema_filter(data, schema)
+
+        if "jsonschema" in environment.tests:
+            warn(
+                'A test named "jsonschema" already exists in the Jinja2 environment',
+                category=RuntimeWarning,
+                stacklevel=2,
+            )
+        else:
+            environment.tests["jsonschema"] = jsonschema_test
 
 
 _Schema = Mapping[str, Any]
 
 
 class _JsonSchemaFilter:
     """Jinja2 filter for validating data aginst a JSON Schema document."""
@@ -121,13 +136,13 @@
             raise
         return self._load(raw_schema)
 
     @staticmethod
     def _load(raw_schema: str) -> _Schema:
         schema: _Schema
         try:
-            import yaml  # pylint: disable=import-outside-toplevel
+            import yaml
         except ImportError:
             schema = json.loads(raw_schema)
         else:
             schema = yaml.safe_load(raw_schema)
         return schema
```

### Comparing `jinja2_jsonschema-0.1.0/PKG-INFO` & `jinja2_jsonschema-0.2.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jinja2-jsonschema
-Version: 0.1.0
+Version: 0.2.0
 Summary: JSON/YAML schema validation within Jinja2 templates
 Home-page: https://github.com/copier-org/jinja2-jsonschema
 License: MIT
 Keywords: jinja,jinja2,extension,jsonschema,json,yaml
 Author: Sigurd Spieckermann
 Author-email: sigurd.spieckermann@gmail.com
 Requires-Python: >=3.7.2
@@ -14,37 +14,32 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: yaml
 Requires-Dist: jinja2 (>=3.0.0)
 Requires-Dist: jsonschema (>=4.0.0)
 Requires-Dist: pyyaml (>=6.0.0) ; extra == "yaml"
 Project-URL: Repository, https://github.com/copier-org/jinja2-jsonschema
 Description-Content-Type: text/markdown
 
 # JSON Schema Validation within Jinja2 Templates
 
 [![CI](https://github.com/copier-org/jinja2-jsonschema/workflows/tests/badge.svg)](https://github.com/copier-org/jinja2-jsonschema/actions?query=branch%3Amain)
 ![Python versions](https://img.shields.io/pypi/pyversions/jinja2-jsonschema?logo=python&logoColor=%23959DA5)
 [![PyPI](https://img.shields.io/pypi/v/jinja2-jsonschema?logo=pypi&logoColor=%23959DA5)](https://pypi.org/project/jinja2-jsonschema)
 [![Code style: Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Linter: Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/charliermarsh/ruff)
+[![Linter: Ruff](https://img.shields.io/badge/-Ruff-261230.svg?labelColor=grey&logo=ruff&logoColor=D7FF64)](https://github.com/charliermarsh/ruff)
 [![Type-checker: mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org)
 
-A [Jinja2 extension][jinja-extensions] providing a [Jinja2 filter][jinja-filter] for validating data against a JSON/YAML schema within [Jinja2][jinja] templates.
+A [Jinja2 extension][jinja-extensions] providing a [Jinja2 filter][jinja-filter] and a [Jinja2 test][jinja-test] for validating data against a JSON/YAML schema within [Jinja2][jinja] templates.
 
 ## Installation
 
 * With [`pip`](https://pip.pypa.io):
 
     ```shell
     pip install jinja2-jsonschema
@@ -78,56 +73,113 @@
 
     # ... or with YAML support
     pipx inject PACKAGE jinja2-jsonschema[yaml]
     ```
 
 ## Usage
 
-The extension provides a Jinja2 filter which receives a schema file path or schema object as input and returns a [`jsonschema.ValidationError`][python-jsonschema-validationerror] object when validation fails and an empty string (`""`) otherwise. The [JSON Schema dialect][jsonschema-dialect] is inferred from the `$schema` field in the JSON Schema document and, when omitted, defaults to the [latest dialect supported by the installed `jsonschema` library][python-jsonschema-features]. Both local and remote schemas are supported including [schema references][jsonschema-ref] and [JSON Pointers][jsonschema-jsonpointer].
+The extension provides:
+
+* A Jinja2 filter which receives a schema file path or schema object as input and returns a [`jsonschema.ValidationError`][python-jsonschema-validationerror] object when validation fails and an empty string (`""`) otherwise.
+* A Jinja2 test which receives a schema file path or schema object as input and returns `False` when validation fails and `True` otherwise.
+
+The [JSON Schema dialect][jsonschema-dialect] is inferred from the `$schema` field in the JSON Schema document and, when omitted, defaults to the [latest dialect supported by the installed `jsonschema` library][python-jsonschema-features]. Both local and remote schemas are supported including [schema references][jsonschema-ref] and [JSON Pointers][jsonschema-jsonpointer].
 
 Local schema files are loaded via a [Jinja2 loader](https://jinja.palletsprojects.com/en/latest/api/#loaders) in which case configuring the Jinja2 environment with a loader is mandatory.
 
-Some example usage of the JSON Schema validation filter is this:
+Some example usage of the JSON Schema validation filter and test is this:
 
 ```python
 from jinja2 import Environment
 from jinja2 import FileSystemLoader
 
 
 env = Environment(
     # Register a loader (only necessary when using local schema files).
     loader=FileSystemLoader("/path/to/templates"),
     # Register the extension.
-    extensions=['jinja2_jsonschema.JsonSchemaExtension'],
+    extensions=["jinja2_jsonschema.JsonSchemaExtension"],
 )
 
 # Example using an inline schema object.
 template = env.from_string("{{ age | jsonschema({'type': 'integer', 'minimum': 0}) }}")
 template.render(age=30)  # OK
 template.render(age=-1)  # ERROR
+template = env.from_string("{{ age is jsonschema({'type': 'integer', 'minimum': 0}) }}")
+template.render(age=30)  # --> `True`
+template.render(age=-1)  # --> `False`
 
 # Example using a local schema file.
 template = env.from_string("{{ age | jsonschema('age.json') }}")
 template.render(age=30)  # OK
 template.render(age=-1)  # ERROR
+template = env.from_string("{{ age is jsonschema('age.json') }}")
+template.render(age=30)  # --> `True`
+template.render(age=-1)  # --> `False`
 
 # Example using a remote schema file.
 template = env.from_string("{{ age | jsonschema('https://example.com/age.json') }}")
 template.render(age=30)  # OK
 template.render(age=-1)  # ERROR
+template = env.from_string("{{ age is jsonschema('https://example.com/age.json') }}")
+template.render(age=30)  # --> `True`
+template.render(age=-1)  # --> `False`
+```
+
+## Usage with Copier
+
+The extension integrates nicely with [Copier][copier], e.g. for validating complex JSON/YAML answers in the Copier questionnaire. For this, add the extension as a [Jinja2 extension in `copier.yml`][copier-jinja-extensions] and use the Jinja2 filter in the `validator` field of a Copier [question][copier-questions]. For instance:
+
+```yaml
+_jinja_extensions:
+  - jinja2_jsonschema.JsonSchemaExtension
+
+complex_question:
+  type: json # or `yaml`
+  validator: "{{ complex_question | jsonschema('schemas/complex.json') }}"
+```
+
+In this example, a local schema file `schemas/complex.json` is used whose path is relative to the template root. To prevent copying schema files to the generated project, they should be either [excluded][copier-exclude]
+
+```diff
++_exclude:
++  - schemas/
+ _jinja_extensions:
+   - jinja2_jsonschema.JsonSchemaExtension
+```
+
+or the project template should be located in a [subdirectory][copier-subdirectory] such as `template/`:
+
+```diff
++_subdirectory_: template
+ _jinja_extensions:
+   - jinja2_jsonschema.JsonSchemaExtension
+```
+
+Finally, template consumers need to install the extension along with Copier. For instance with `pipx`:
+
+```shell
+pipx install copier
+pipx inject copier jinja2-jsonschema
 ```
 
 ## Contributions
 
 Contributions are always welcome via filing [issues](https://github.com/copier-org/jinja2-jsonschema/issues) or submitting [pull requests](https://github.com/copier-org/jinja2-jsonschema/pulls). Please check the [contribution guide][contribution-guide] for more details.
 
-[contribution-guide]: https://https://github.com/copier-org/jinja2-jsonschema/blob/main/CONTRIBUTING.md
+[contribution-guide]: https://github.com/copier-org/jinja2-jsonschema/blob/main/CONTRIBUTING.md
+[copier]: https://github.com/copier-org/copier
+[copier-exclude]: https://copier.readthedocs.io/en/stable/configuring/#exclude
+[copier-jinja-extensions]: https://copier.readthedocs.io/en/stable/configuring/#jinja_extensions
+[copier-questions]: https://copier.readthedocs.io/en/stable/configuring/#questions
+[copier-subdirectory]: https://copier.readthedocs.io/en/stable/configuring/#subdirectory
 [jinja]: https://jinja.palletsprojects.com
 [jinja-extensions]: https://jinja.palletsprojects.com/en/latest/extensions/
 [jinja-filter]: https://jinja.palletsprojects.com/en/latest/templates/#filters
+[jinja-test]: https://jinja.palletsprojects.com/en/latest/templates/#tests
 [jsonschema]: https://json-schema.org
 [jsonschema-dialect]: https://json-schema.org/understanding-json-schema/reference/schema.html#schema
 [jsonschema-ref]: https://json-schema.org/understanding-json-schema/structuring.html#ref
 [jsonschema-jsonpointer]: https://json-schema.org/understanding-json-schema/structuring.html#json-pointer
 [pdm]: https://pdm.fming.dev
 [pip]: https://pip.pypa.io
 [pipx]: https://pypa.github.io/pipx
```

