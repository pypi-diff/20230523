# Comparing `tmp/poetry-relax-0.1.1.tar.gz` & `tmp/poetry-relax-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry-relax-0.1.1.tar", max compression
+gzip compressed data, was "poetry-relax-0.1.2.tar", max compression
```

## Comparing `poetry-relax-0.1.1.tar` & `poetry-relax-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1070 2023-03-24 05:40:27.765564 poetry-relax-0.1.1/LICENSE
--rw-r--r--   0        0        0     6544 2023-03-24 05:40:27.765564 poetry-relax-0.1.1/README.md
--rw-r--r--   0        0        0     1411 2023-03-24 05:41:07.519975 poetry-relax-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      434 2023-03-24 05:40:27.765564 poetry-relax-0.1.1/src/poetry_relax/__init__.py
--rw-r--r--   0        0        0     7225 2023-03-24 05:40:27.765564 poetry-relax-0.1.1/src/poetry_relax/_core.py
--rw-r--r--   0        0        0     7830 2023-03-24 05:40:27.765564 poetry-relax-0.1.1/src/poetry_relax/command.py
--rw-r--r--   0        0        0        0 2023-03-24 05:40:27.765564 poetry-relax-0.1.1/src/poetry_relax/py.typed
--rw-r--r--   0        0        0     7532 1970-01-01 00:00:00.000000 poetry-relax-0.1.1/setup.py
--rw-r--r--   0        0        0     7940 1970-01-01 00:00:00.000000 poetry-relax-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-23 15:47:55.953304 poetry-relax-0.1.2/LICENSE
+-rw-r--r--   0        0        0     6496 2023-05-23 15:47:55.953304 poetry-relax-0.1.2/README.md
+-rw-r--r--   0        0        0     1411 2023-05-23 15:48:35.935095 poetry-relax-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      434 2023-05-23 15:47:55.953304 poetry-relax-0.1.2/src/poetry_relax/__init__.py
+-rw-r--r--   0        0        0     7559 2023-05-23 15:47:55.953304 poetry-relax-0.1.2/src/poetry_relax/_core.py
+-rw-r--r--   0        0        0     7830 2023-05-23 15:47:55.953304 poetry-relax-0.1.2/src/poetry_relax/command.py
+-rw-r--r--   0        0        0        0 2023-05-23 15:47:55.953304 poetry-relax-0.1.2/src/poetry_relax/py.typed
+-rw-r--r--   0        0        0     7484 1970-01-01 00:00:00.000000 poetry-relax-0.1.2/setup.py
+-rw-r--r--   0        0        0     7892 1970-01-01 00:00:00.000000 poetry-relax-0.1.2/PKG-INFO
```

### Comparing `poetry-relax-0.1.1/LICENSE` & `poetry-relax-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry-relax-0.1.1/README.md` & `poetry-relax-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
 > Does this plugin remove upper constraints I've added?
 
 This plugin will only relax constraints specified with a caret (`^`). Upper constraints added with `<` and `<=` will not be changed.
 
 > Is this plugin stable?
 
-This plugin is brand new! Poetry just added their plugin system recently. Efforts will be made to avoid changes in behavior, but it'll be valuable to gather feedback on this plugin in its early stages before releasing a stable version. However, the test suite is thorough and common cases should be well covered.
+This plugin is tested against multiple versions of Poetry and has an integration focused test suite. It is safe to use this in production, though it is recommend to pin versions. Breaking changes will be avoided unless infeasible due to upstream changes in Poetry.
 
 > Will this plugin drop the upper bound on Python itself?
 
 Believe it or not, this is an even more contentious subset of this issue as Poetry will not allow packages with no upper bound on Python to exist alongside those that include one. This basically means that we cannot relax this requirement without breaking the vast majority of use-cases. For this reason, we cannot relax `python^3` at this time. See [the post on the Poetry discussion board](https://github.com/python-poetry/poetry/discussions/3757#discussioncomment-435345) for more details.
 
 ## Contributing
```

### Comparing `poetry-relax-0.1.1/pyproject.toml` & `poetry-relax-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-relax"
-version = "0.1.1"
+version = "0.1.2"
 repository = "https://github.com/madkinsz/poetry-relax"
 description = "Plugin for Poetry to relax upper version pins"
 authors = ["Zanie <contact@zanie.dev>"]
 readme = "README.md"
 keywords = ["poetry", "plugin", "versioning", "version"]
 packages = [{ include = "poetry_relax", from = "src" }]
 classifiers = [
```

### Comparing `poetry-relax-0.1.1/src/poetry_relax/_core.py` & `poetry-relax-0.1.2/src/poetry_relax/_core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,32 @@
 """
 Core utilities for the `poetry relax` functionality.
 """
 import contextlib
 import functools
 import re
+import sys
 from copy import copy
 from typing import TYPE_CHECKING, Any, Callable, Iterable, Optional
 
-import pkg_resources
+import packaging.version
 
-if pkg_resources.get_distribution("poetry").version.startswith("1.2."):
+if sys.version_info < (3, 8):  # Python 3.7 support
+    import pkg_resources
+
+    POETRY_VERSION = packaging.version.Version(
+        pkg_resources.get_distribution("poetry").version
+    )
+else:
+    import importlib.metadata as importlib_metadata
+
+    POETRY_VERSION = packaging.version.Version(importlib_metadata.version("poetry"))
+
+
+if POETRY_VERSION < packaging.version.Version("1.3.0"):
     from poetry.core.semver.version_range import VersionRange
 else:
     from poetry.core.constraints.version import VersionRange
 
 from poetry.core.packages.dependency_group import MAIN_GROUP
 
 if TYPE_CHECKING:
```

### Comparing `poetry-relax-0.1.1/src/poetry_relax/command.py` & `poetry-relax-0.1.2/src/poetry_relax/command.py`

 * *Files identical despite different names*

### Comparing `poetry-relax-0.1.1/setup.py` & `poetry-relax-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 ['poetry>=1.2']
 
 entry_points = \
 {'poetry.application.plugin': ['relax = poetry_relax:RelaxPlugin']}
 
 setup_kwargs = {
     'name': 'poetry-relax',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'Plugin for Poetry to relax upper version pins',
-    'long_description': "# poetry-relax\n\nA [Poetry](https://github.com/python-poetry/poetry) plugin to relax dependency versions when publishing libraries. Relax your project's dependencies from `foobar^2.0.0` to `foobar>=2.0.0`.\n\nBy default, Poetry uses caret constraints which would limit `foobar` versions to `<3.0`.\n**poetry-relax**  removes these upper version bounds, allowing dependencies to be upgraded.\n\nRemoving upper version bounds is important when publishing libraries.\nWhen searching for versions of dependencies to install, the resolver (e.g. `pip`) must respect the bounds your library specifies.\nWhen a new version of the dependency is released, consumers of your library _cannot_ install it unless a new version of your library is also released.\n\nIt is not feasible to release patches for every previous version of most libraries, which forces users to use the most recent version of the library or be stuck without the new version of the dependency.\nWhen many libraries contain upper version bounds, the dependencies can easily become _unsolvable_ — where libraries have incompatible dependency version requirements.\nBy removing upper version bounds from your library, control is returned to the user.\n\nPoetry's default behavior is to include upper version bounds. Many people have spoken up against this style of dependency management in the Python ecosystem, including members of the Python core development team. See [the bottom of the readme](#references) for links and additional context.\n\nSince the Poetry project will not allow this behavior to be configured, maintainers have resorted to manual editing of dependency constraints after adding. **poetry-relax** aims to automate and simplify this process.\n\n**poetry-relax** provides:\n- Automated removal of upper bound constraints specified with `^`\n- Safety check if package requirements are still solvable after relaxing constraints\n- Upgrade of dependencies after relaxing constraints\n- Update of the lock file without upgrading dependencies\n- Limit dependency relaxation to specific dependency groups\n- Retention of intentional upper bounds indicating true incompatibilities\n- CLI messages designed to match Poetry's output\n\n## Installation\n\nThe plugin must be installed in Poetry's environment. This requires use of the  `self` subcommand.\n\n```bash\n$ poetry self add poetry-relax\n```\n\n## Usage\n\nRelax constraints for which Poetry set an upper version:\n\n```bash\n$ poetry relax\n```\n\nRelax constraints and check that they are resolvable without performing upgrades:\n\n```bash\n$ poetry relax --check\n```\n\nRelax constraints and upgrade packages:\n\n```bash\n$ poetry relax --update\n```\n\nRelax constraints and update the lock file without upgrading packages:\n\n```bash\n$ poetry relax --lock\n```\n\nPreview the changes `poetry relax` would make without modifying the project:\n\n```bash\n$ poetry relax --dry-run\n```\n\n## Examples\n\nThe behavior of Poetry is quite reasonable for local development! `poetry relax` is most useful when used in CI/CD pipelines.\n\n### Relaxing requirements before publishing\n\nRun `poetry relax` before building and publishing a package.\n\nSee it at work in [the release workflow for this project](https://github.com/madkinsz/poetry-relax/blob/main/.github/workflows/release.yaml).\n\n\n### Relaxing requirements for testing\n\nRun `poetry relax --update` before tests to test against the newest possible versions of packages.\n\nSee it at work in [the test workflow for this project](https://github.com/madkinsz/poetry-relax/blob/main/.github/workflows/test.yaml).\n\n## Frequently asked questions\n\n> Can this plugin change the behavior of `poetry add` to relax constraints?\n\nNot at this time. The Poetry project states that plugins must not alter the behavior of core Poetry commands. If this behavior would be useful for you, please chime in [on the tracking issue](https://github.com/madkinsz/poetry-relax/issues/5).\n\n> Does this plugin remove upper constraints I've added?\n\nThis plugin will only relax constraints specified with a caret (`^`). Upper constraints added with `<` and `<=` will not be changed.\n\n> Is this plugin stable?\n\nThis plugin is brand new! Poetry just added their plugin system recently. Efforts will be made to avoid changes in behavior, but it'll be valuable to gather feedback on this plugin in its early stages before releasing a stable version. However, the test suite is thorough and common cases should be well covered.\n\n> Will this plugin drop the upper bound on Python itself?\n\nBelieve it or not, this is an even more contentious subset of this issue as Poetry will not allow packages with no upper bound on Python to exist alongside those that include one. This basically means that we cannot relax this requirement without breaking the vast majority of use-cases. For this reason, we cannot relax `python^3` at this time. See [the post on the Poetry discussion board](https://github.com/python-poetry/poetry/discussions/3757#discussioncomment-435345) for more details.\n\n## Contributing\n\nThis project is managed with Poetry. Here are the basics for getting started.\n\nClone the repository:\n```bash\n$ git clone https://github.com/madkinsz/poetry-relax.git\n$ cd poetry-relax\n```\n\nInstall packages:\n```bash\n$ poetry install\n```\n\nRun the test suite:\n```bash\n$ pytest tests\n```\n\nRun linters before opening pull requests:\n```bash\n$ ./bin/lint check .\n$ ./bin/lint fix .\n```\n\n## References\n\nThere's a lot to read on this topic! It's contentious and causing a lot of problems for maintainers and users.\n\nThe following blog posts by Henry Schreiner are quite comprehensive:\n- [Should You Use Upper Bound Version Constraints?](https://iscinumpy.dev/post/bound-version-constraints/)\n- [Poetry Versions](https://iscinumpy.dev/post/poetry-versions/)\n\nContent from some members of the Python core developer team:\n- [Semantic Versioning Will Not Save You](https://hynek.me/articles/semver-will-not-save-you/)\n- [Why I don't like SemVer anymore](https://snarky.ca/why-i-dont-like-semver/)\n- [Version numbers: how to use them?](https://bernat.tech/posts/version-numbers/)\n- [Versioning Software](https://caremad.io/posts/2016/02/versioning-software/)\n\nDiscussion and issues in the Poetry project:\n- [Please stop pinning to major versions by default, especially for Python itself](https://github.com/python-poetry/poetry/issues/3747)\n- [Change default dependency constraint from ^ to >=](https://github.com/python-poetry/poetry/issues/3427)\n- [Developers should be able to turn off dependency upper-bound calculations](https://github.com/python-poetry/poetry/issues/2731)\n",
+    'long_description': "# poetry-relax\n\nA [Poetry](https://github.com/python-poetry/poetry) plugin to relax dependency versions when publishing libraries. Relax your project's dependencies from `foobar^2.0.0` to `foobar>=2.0.0`.\n\nBy default, Poetry uses caret constraints which would limit `foobar` versions to `<3.0`.\n**poetry-relax**  removes these upper version bounds, allowing dependencies to be upgraded.\n\nRemoving upper version bounds is important when publishing libraries.\nWhen searching for versions of dependencies to install, the resolver (e.g. `pip`) must respect the bounds your library specifies.\nWhen a new version of the dependency is released, consumers of your library _cannot_ install it unless a new version of your library is also released.\n\nIt is not feasible to release patches for every previous version of most libraries, which forces users to use the most recent version of the library or be stuck without the new version of the dependency.\nWhen many libraries contain upper version bounds, the dependencies can easily become _unsolvable_ — where libraries have incompatible dependency version requirements.\nBy removing upper version bounds from your library, control is returned to the user.\n\nPoetry's default behavior is to include upper version bounds. Many people have spoken up against this style of dependency management in the Python ecosystem, including members of the Python core development team. See [the bottom of the readme](#references) for links and additional context.\n\nSince the Poetry project will not allow this behavior to be configured, maintainers have resorted to manual editing of dependency constraints after adding. **poetry-relax** aims to automate and simplify this process.\n\n**poetry-relax** provides:\n- Automated removal of upper bound constraints specified with `^`\n- Safety check if package requirements are still solvable after relaxing constraints\n- Upgrade of dependencies after relaxing constraints\n- Update of the lock file without upgrading dependencies\n- Limit dependency relaxation to specific dependency groups\n- Retention of intentional upper bounds indicating true incompatibilities\n- CLI messages designed to match Poetry's output\n\n## Installation\n\nThe plugin must be installed in Poetry's environment. This requires use of the  `self` subcommand.\n\n```bash\n$ poetry self add poetry-relax\n```\n\n## Usage\n\nRelax constraints for which Poetry set an upper version:\n\n```bash\n$ poetry relax\n```\n\nRelax constraints and check that they are resolvable without performing upgrades:\n\n```bash\n$ poetry relax --check\n```\n\nRelax constraints and upgrade packages:\n\n```bash\n$ poetry relax --update\n```\n\nRelax constraints and update the lock file without upgrading packages:\n\n```bash\n$ poetry relax --lock\n```\n\nPreview the changes `poetry relax` would make without modifying the project:\n\n```bash\n$ poetry relax --dry-run\n```\n\n## Examples\n\nThe behavior of Poetry is quite reasonable for local development! `poetry relax` is most useful when used in CI/CD pipelines.\n\n### Relaxing requirements before publishing\n\nRun `poetry relax` before building and publishing a package.\n\nSee it at work in [the release workflow for this project](https://github.com/madkinsz/poetry-relax/blob/main/.github/workflows/release.yaml).\n\n\n### Relaxing requirements for testing\n\nRun `poetry relax --update` before tests to test against the newest possible versions of packages.\n\nSee it at work in [the test workflow for this project](https://github.com/madkinsz/poetry-relax/blob/main/.github/workflows/test.yaml).\n\n## Frequently asked questions\n\n> Can this plugin change the behavior of `poetry add` to relax constraints?\n\nNot at this time. The Poetry project states that plugins must not alter the behavior of core Poetry commands. If this behavior would be useful for you, please chime in [on the tracking issue](https://github.com/madkinsz/poetry-relax/issues/5).\n\n> Does this plugin remove upper constraints I've added?\n\nThis plugin will only relax constraints specified with a caret (`^`). Upper constraints added with `<` and `<=` will not be changed.\n\n> Is this plugin stable?\n\nThis plugin is tested against multiple versions of Poetry and has an integration focused test suite. It is safe to use this in production, though it is recommend to pin versions. Breaking changes will be avoided unless infeasible due to upstream changes in Poetry.\n\n> Will this plugin drop the upper bound on Python itself?\n\nBelieve it or not, this is an even more contentious subset of this issue as Poetry will not allow packages with no upper bound on Python to exist alongside those that include one. This basically means that we cannot relax this requirement without breaking the vast majority of use-cases. For this reason, we cannot relax `python^3` at this time. See [the post on the Poetry discussion board](https://github.com/python-poetry/poetry/discussions/3757#discussioncomment-435345) for more details.\n\n## Contributing\n\nThis project is managed with Poetry. Here are the basics for getting started.\n\nClone the repository:\n```bash\n$ git clone https://github.com/madkinsz/poetry-relax.git\n$ cd poetry-relax\n```\n\nInstall packages:\n```bash\n$ poetry install\n```\n\nRun the test suite:\n```bash\n$ pytest tests\n```\n\nRun linters before opening pull requests:\n```bash\n$ ./bin/lint check .\n$ ./bin/lint fix .\n```\n\n## References\n\nThere's a lot to read on this topic! It's contentious and causing a lot of problems for maintainers and users.\n\nThe following blog posts by Henry Schreiner are quite comprehensive:\n- [Should You Use Upper Bound Version Constraints?](https://iscinumpy.dev/post/bound-version-constraints/)\n- [Poetry Versions](https://iscinumpy.dev/post/poetry-versions/)\n\nContent from some members of the Python core developer team:\n- [Semantic Versioning Will Not Save You](https://hynek.me/articles/semver-will-not-save-you/)\n- [Why I don't like SemVer anymore](https://snarky.ca/why-i-dont-like-semver/)\n- [Version numbers: how to use them?](https://bernat.tech/posts/version-numbers/)\n- [Versioning Software](https://caremad.io/posts/2016/02/versioning-software/)\n\nDiscussion and issues in the Poetry project:\n- [Please stop pinning to major versions by default, especially for Python itself](https://github.com/python-poetry/poetry/issues/3747)\n- [Change default dependency constraint from ^ to >=](https://github.com/python-poetry/poetry/issues/3427)\n- [Developers should be able to turn off dependency upper-bound calculations](https://github.com/python-poetry/poetry/issues/2731)\n",
     'author': 'Zanie',
     'author_email': 'contact@zanie.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/madkinsz/poetry-relax',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `poetry-relax-0.1.1/PKG-INFO` & `poetry-relax-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-relax
-Version: 0.1.1
+Version: 0.1.2
 Summary: Plugin for Poetry to relax upper version pins
 Home-page: https://github.com/madkinsz/poetry-relax
 Keywords: poetry,plugin,versioning,version
 Author: Zanie
 Author-email: contact@zanie.dev
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -125,15 +125,15 @@
 
 > Does this plugin remove upper constraints I've added?
 
 This plugin will only relax constraints specified with a caret (`^`). Upper constraints added with `<` and `<=` will not be changed.
 
 > Is this plugin stable?
 
-This plugin is brand new! Poetry just added their plugin system recently. Efforts will be made to avoid changes in behavior, but it'll be valuable to gather feedback on this plugin in its early stages before releasing a stable version. However, the test suite is thorough and common cases should be well covered.
+This plugin is tested against multiple versions of Poetry and has an integration focused test suite. It is safe to use this in production, though it is recommend to pin versions. Breaking changes will be avoided unless infeasible due to upstream changes in Poetry.
 
 > Will this plugin drop the upper bound on Python itself?
 
 Believe it or not, this is an even more contentious subset of this issue as Poetry will not allow packages with no upper bound on Python to exist alongside those that include one. This basically means that we cannot relax this requirement without breaking the vast majority of use-cases. For this reason, we cannot relax `python^3` at this time. See [the post on the Poetry discussion board](https://github.com/python-poetry/poetry/discussions/3757#discussioncomment-435345) for more details.
 
 ## Contributing
```

