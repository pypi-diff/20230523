# Comparing `tmp/named-1.1.0.tar.gz` & `tmp/named-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "named-1.1.0.tar", max compression
+gzip compressed data, was "named-1.2.0.tar", max compression
```

## Comparing `named-1.1.0.tar` & `named-1.2.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1092 2022-11-07 13:58:12.159378 named-1.1.0/LICENSE
--rw-r--r--   0        0        0     3056 2022-11-07 13:58:12.159378 named-1.1.0/README.md
--rw-r--r--   0        0        0      938 2022-11-07 13:58:12.159378 named-1.1.0/named/__init__.py
--rw-r--r--   0        0        0        0 2022-11-07 13:58:12.159378 named-1.1.0/named/py.typed
--rw-r--r--   0        0        0     1233 2022-11-07 13:58:12.159378 named-1.1.0/named/typing.py
--rw-r--r--   0        0        0     2952 2022-11-07 13:58:12.159378 named-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     3782 1970-01-01 00:00:00.000000 named-1.1.0/setup.py
--rw-r--r--   0        0        0     4176 1970-01-01 00:00:00.000000 named-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-05-23 21:52:52.063806 named-1.2.0/LICENSE
+-rw-r--r--   0        0        0     3056 2023-05-23 21:52:52.063806 named-1.2.0/README.md
+-rw-r--r--   0        0        0     1242 2023-05-23 21:52:52.063806 named-1.2.0/named/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 21:52:52.063806 named-1.2.0/named/py.typed
+-rw-r--r--   0        0        0     2646 2023-05-23 21:52:52.063806 named-1.2.0/named/typing.py
+-rw-r--r--   0        0        0     3099 2023-05-23 21:52:52.063806 named-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4176 1970-01-01 00:00:00.000000 named-1.2.0/PKG-INFO
```

### Comparing `named-1.1.0/LICENSE` & `named-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `named-1.1.0/README.md` & `named-1.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 $ poetry add named
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-named = "^1.1.0"
+named = "^1.2.0"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.named]
 git = "https://github.com/nekitdev/named.git"
```

### Comparing `named-1.1.0/named/typing.py` & `named-1.2.0/named/typing.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,38 @@
 from builtins import hasattr as has_attribute
 from typing import Any
 
 from typing_extensions import Protocol, TypeGuard, runtime_checkable
 
-__all__ = ("NAME", "Named", "get_name", "get_type_name", "is_named")
+__all__ = (
+    # named
+    "NAME",
+    "Named",
+    "get_name",
+    "get_type_name",
+    "has_name",
+    "is_named",
+    # moduled
+    "MODULE",
+    "Moduled",
+    "get_module",
+    "get_type_module",
+    "has_module",
+    "is_moduled",
+)
 
 
 NAME = "__name__"
 """The literal `__name__` string."""
 
 
 @runtime_checkable
 class Named(Protocol):
     """The named protocol for types that contain the `__name__` attribute."""
+
     __name__: str
 
 
 def get_name(item: Named) -> str:
     """Fetches the `__name__` of the [`Named`][named.typing.Named] `item`.
 
     Arguments:
@@ -46,7 +62,62 @@
     Arguments:
         item: The item to check.
 
     Returns:
         Whether the item implements the [`Named`][named.typing.Named] protocol.
     """
     return has_attribute(item, NAME)
+
+
+has_name = is_named
+"""An alias of [`is_named`][named.typing.is_named]."""
+
+
+MODULE = "__module__"
+"""The literal `__module__` string."""
+
+
+@runtime_checkable
+class Moduled(Protocol):
+    """The moduled protocol for types that contain the `__module__` attribute."""
+
+    __module__: str
+
+
+def get_module(item: Moduled) -> str:
+    """Fetches the `__module__` of the [`Moduled`][named.typing.Moduled] `item`.
+
+    Arguments:
+        item: The item to fetch the module of.
+
+    Returns:
+        The module of the item.
+    """
+    return item.__module__
+
+
+def get_type_module(item: Any) -> str:
+    """Fetches the `__module__` of the `item` type.
+
+    Arguments:
+        item: The item to fetch the type module of.
+
+    Returns:
+        The module of the item type.
+    """
+    return get_module(type(item))  # type: ignore
+
+
+def is_moduled(item: Any) -> TypeGuard[Moduled]:
+    """Checks if the `item` implements the [`Moduled`][named.typing.Moduled] protocol.
+
+    Arguments:
+        item: The item to check.
+
+    Returns:
+        Whether the item implements the [`Moduled`][named.typing.Moduled] protocol.
+    """
+    return has_attribute(item, MODULE)
+
+
+has_module = is_moduled
+"""An alias of [`is_moduled`][named.typing.is_moduled]."""
```

### Comparing `named-1.1.0/pyproject.toml` & `named-1.2.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "named"
-version = "1.1.0"
+version = "1.2.0"
 description = "Named types."
 authors = ["nekitdev"]
 license = "MIT"
 
 readme = "README.md"
 
 homepage = "https://github.com/nekitdev/named"
@@ -27,56 +27,64 @@
 Issues = "https://github.com/nekitdev/named/issues"
 
 [[tool.poetry.packages]]
 include = "named"
 
 [tool.poetry.dependencies]
 python = ">= 3.7"
-typing-extensions = ">= 4.3.0"
+typing-extensions = ">= 4.5.0"
 
 [tool.poetry.group.format]
 optional = true
 
 [tool.poetry.group.format.dependencies]
-black = "22.8.0"
+black = "23.3.0"
+flake8-pyproject = "1.2.3"
+
+[tool.poetry.group.format.dependencies.flake8]
+version = "6.0.0"
+python = ">= 3.8.1"
 
 [tool.poetry.group.format.dependencies.isort]
-version = "5.10.1"
-python = "^3.7"
+version = "5.12.0"
+python = ">= 3.8"
 
 [tool.poetry.group.check]
 optional = true
 
 [tool.poetry.group.check.dependencies]
-mypy = "0.982"
+mypy = "1.3.0"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
-pytest = "7.1.3"
-pytest-cov = "3.0.0"
+pytest = "7.3.1"
+pytest-cov = "4.0.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-mkdocs = "1.3.1"
-mkdocs-material = "8.5.3"
+mkdocs = "1.4.3"
+mkdocs-material = "9.1.14"
 
 [tool.poetry.group.docs.dependencies.mkdocstrings]
-version = "0.19.0"
+version = "0.21.2"
 extras = ["python"]
 
 [tool.poetry.group.dev.dependencies]
-changelogging = "1.0.0"
+changelogging = "1.3.0"
 
 [tool.black]
 line_length = 100
 
+[tool.flake8]
+max_line_length = 100
+
 [tool.isort]
 line_length = 100
 profile = "black"
 
 [tool.pytest.ini_options]
 addopts = "--cov named"
 testpaths = ["tests"]
@@ -87,15 +95,15 @@
 [tool.coverage.report]
 ignore_errors = true
 exclude_lines = [
     "pragma: never",
     "pragma: no cover",
     "if TYPE_CHECKING",
     "@overload",
-    "@abstractmethod",
+    "@required",
     "raise NotImplementedError",
     "raise AssertionError",
     "def __repr__",
 ]
 
 [tool.coverage.html]
 directory = "coverage"
@@ -123,15 +131,15 @@
 warn_unreachable = true
 
 warn_redundant_casts = true
 warn_unused_ignores = false  # compatibility
 
 [tool.changelogging]
 name = "named"
-version = "1.1.0"
+version = "1.2.0"
 url = "https://github.com/nekitdev/named"
 directory = "changes"
 output = "CHANGELOG.md"
 
 start_string = "<!-- changelogging: start -->"
 
 title_format = "{version} ({date})"
@@ -140,9 +148,9 @@
 bullet = "-"
 wrap = true
 wrap_size = 100
 
 display = ["feature", "change", "fix", "security", "deprecation", "removal", "internal"]
 
 [build-system]
-requires = ["poetry-core >= 1.3.2"]
+requires = ["poetry-core >= 1.5.2"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `named-1.1.0/setup.py` & `named-1.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,152 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: named
+Version: 1.2.0
+Summary: Named types.
+Home-page: https://github.com/nekitdev/named
+License: MIT
+Keywords: python,named,name
+Author: nekitdev
+Requires-Python: >=3.7
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Utilities
+Classifier: Typing :: Typed
+Requires-Dist: typing-extensions (>=4.5.0)
+Project-URL: Documentation, https://nekitdev.github.io/named
+Project-URL: Discord, https://nekit.dev/discord
+Project-URL: Funding, https://patreon.com/nekitdev
+Project-URL: Issues, https://github.com/nekitdev/named/issues
+Project-URL: Repository, https://github.com/nekitdev/named
+Description-Content-Type: text/markdown
 
-packages = \
-['named']
+# `named`
 
-package_data = \
-{'': ['*']}
+[![License][License Badge]][License]
+[![Version][Version Badge]][Package]
+[![Downloads][Downloads Badge]][Package]
+[![Discord][Discord Badge]][Discord]
 
-install_requires = \
-['typing-extensions>=4.3.0']
-
-setup_kwargs = {
-    'name': 'named',
-    'version': '1.1.0',
-    'description': 'Named types.',
-    'long_description': '# `named`\n\n[![License][License Badge]][License]\n[![Version][Version Badge]][Package]\n[![Downloads][Downloads Badge]][Package]\n[![Discord][Discord Badge]][Discord]\n\n[![Documentation][Documentation Badge]][Documentation]\n[![Check][Check Badge]][Actions]\n[![Test][Test Badge]][Actions]\n[![Coverage][Coverage Badge]][Coverage]\n\n> *Named types.*\n\n## Installing\n\n**Python 3.7 or above is required.**\n\n### pip\n\nInstalling the library with `pip` is quite simple:\n\n```console\n$ pip install named\n```\n\nAlternatively, the library can be installed from source:\n\n```console\n$ git clone https://github.com/nekitdev/named.git\n$ cd named\n$ python -m pip install .\n```\n\n### poetry\n\nYou can add `named` as a dependency with the following command:\n\n```console\n$ poetry add named\n```\n\nOr by directly specifying it in the configuration like so:\n\n```toml\n[tool.poetry.dependencies]\nnamed = "^1.1.0"\n```\n\nAlternatively, you can add it directly from the source:\n\n```toml\n[tool.poetry.dependencies.named]\ngit = "https://github.com/nekitdev/named.git"\n```\n\n## Example\n\n```python\n>>> from named import get_name, get_type_name, is_named\n>>> print(is_named(int))\nTrue\n>>> print(get_name(int))\nint\n>>> print(is_named(42))\nFalse\n>>> print(get_type_name(42))\nint\n```\n\n## Documentation\n\nYou can find the documentation [here][Documentation].\n\n## Support\n\nIf you need support with the library, you can send an [email][Email]\nor refer to the official [Discord server][Discord].\n\n## Changelog\n\nYou can find the changelog [here][Changelog].\n\n## Security Policy\n\nYou can find the Security Policy of `named` [here][Security].\n\n## Contributing\n\nIf you are interested in contributing to `named`, make sure to take a look at the\n[Contributing Guide][Contributing Guide], as well as the [Code of Conduct][Code of Conduct].\n\n## License\n\n`named` is licensed under the MIT License terms. See [License][License] for details.\n\n[Email]: mailto:support@nekit.dev\n\n[Discord]: https://nekit.dev/discord\n\n[Actions]: https://github.com/nekitdev/named/actions\n\n[Changelog]: https://github.com/nekitdev/named/blob/main/CHANGELOG.md\n[Code of Conduct]: https://github.com/nekitdev/named/blob/main/CODE_OF_CONDUCT.md\n[Contributing Guide]: https://github.com/nekitdev/named/blob/main/CONTRIBUTING.md\n[Security]: https://github.com/nekitdev/named/blob/main/SECURITY.md\n\n[License]: https://github.com/nekitdev/named/blob/main/LICENSE\n\n[Package]: https://pypi.org/project/named\n[Coverage]: https://codecov.io/gh/nekitdev/named\n[Documentation]: https://nekitdev.github.io/named\n\n[Discord Badge]: https://img.shields.io/badge/chat-discord-5865f2\n[License Badge]: https://img.shields.io/pypi/l/named\n[Version Badge]: https://img.shields.io/pypi/v/named\n[Downloads Badge]: https://img.shields.io/pypi/dm/named\n\n[Documentation Badge]: https://github.com/nekitdev/named/workflows/docs/badge.svg\n[Check Badge]: https://github.com/nekitdev/named/workflows/check/badge.svg\n[Test Badge]: https://github.com/nekitdev/named/workflows/test/badge.svg\n[Coverage Badge]: https://codecov.io/gh/nekitdev/named/branch/main/graph/badge.svg\n',
-    'author': 'nekitdev',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/nekitdev/named',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7',
-}
+[![Documentation][Documentation Badge]][Documentation]
+[![Check][Check Badge]][Actions]
+[![Test][Test Badge]][Actions]
+[![Coverage][Coverage Badge]][Coverage]
 
+> *Named types.*
+
+## Installing
+
+**Python 3.7 or above is required.**
+
+### pip
+
+Installing the library with `pip` is quite simple:
+
+```console
+$ pip install named
+```
+
+Alternatively, the library can be installed from source:
+
+```console
+$ git clone https://github.com/nekitdev/named.git
+$ cd named
+$ python -m pip install .
+```
+
+### poetry
+
+You can add `named` as a dependency with the following command:
+
+```console
+$ poetry add named
+```
+
+Or by directly specifying it in the configuration like so:
+
+```toml
+[tool.poetry.dependencies]
+named = "^1.2.0"
+```
+
+Alternatively, you can add it directly from the source:
+
+```toml
+[tool.poetry.dependencies.named]
+git = "https://github.com/nekitdev/named.git"
+```
+
+## Example
+
+```python
+>>> from named import get_name, get_type_name, is_named
+>>> print(is_named(int))
+True
+>>> print(get_name(int))
+int
+>>> print(is_named(42))
+False
+>>> print(get_type_name(42))
+int
+```
+
+## Documentation
+
+You can find the documentation [here][Documentation].
+
+## Support
+
+If you need support with the library, you can send an [email][Email]
+or refer to the official [Discord server][Discord].
+
+## Changelog
+
+You can find the changelog [here][Changelog].
+
+## Security Policy
+
+You can find the Security Policy of `named` [here][Security].
+
+## Contributing
+
+If you are interested in contributing to `named`, make sure to take a look at the
+[Contributing Guide][Contributing Guide], as well as the [Code of Conduct][Code of Conduct].
+
+## License
+
+`named` is licensed under the MIT License terms. See [License][License] for details.
+
+[Email]: mailto:support@nekit.dev
+
+[Discord]: https://nekit.dev/discord
+
+[Actions]: https://github.com/nekitdev/named/actions
+
+[Changelog]: https://github.com/nekitdev/named/blob/main/CHANGELOG.md
+[Code of Conduct]: https://github.com/nekitdev/named/blob/main/CODE_OF_CONDUCT.md
+[Contributing Guide]: https://github.com/nekitdev/named/blob/main/CONTRIBUTING.md
+[Security]: https://github.com/nekitdev/named/blob/main/SECURITY.md
+
+[License]: https://github.com/nekitdev/named/blob/main/LICENSE
+
+[Package]: https://pypi.org/project/named
+[Coverage]: https://codecov.io/gh/nekitdev/named
+[Documentation]: https://nekitdev.github.io/named
+
+[Discord Badge]: https://img.shields.io/badge/chat-discord-5865f2
+[License Badge]: https://img.shields.io/pypi/l/named
+[Version Badge]: https://img.shields.io/pypi/v/named
+[Downloads Badge]: https://img.shields.io/pypi/dm/named
+
+[Documentation Badge]: https://github.com/nekitdev/named/workflows/docs/badge.svg
+[Check Badge]: https://github.com/nekitdev/named/workflows/check/badge.svg
+[Test Badge]: https://github.com/nekitdev/named/workflows/test/badge.svg
+[Coverage Badge]: https://codecov.io/gh/nekitdev/named/branch/main/graph/badge.svg
 
-setup(**setup_kwargs)
```

