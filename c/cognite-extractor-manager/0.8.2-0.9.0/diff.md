# Comparing `tmp/cognite_extractor_manager-0.8.2.tar.gz` & `tmp/cognite_extractor_manager-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_extractor_manager-0.8.2.tar", max compression
+gzip compressed data, was "cognite_extractor_manager-0.9.0.tar", max compression
```

## Comparing `cognite_extractor_manager-0.8.2.tar` & `cognite_extractor_manager-0.9.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    10173 2023-05-15 12:27:07.293851 cognite_extractor_manager-0.8.2/LICENSE
--rw-r--r--   0        0        0     3816 2023-05-15 12:27:07.293851 cognite_extractor_manager-0.8.2/README.md
--rw-r--r--   0        0        0      607 2023-05-15 12:27:07.293851 cognite_extractor_manager-0.8.2/cognite/extractorutils/cogex/__init__.py
--rw-r--r--   0        0        0     3049 2023-05-15 12:27:07.293851 cognite_extractor_manager-0.8.2/cognite/extractorutils/cogex/__main__.py
--rw-r--r--   0        0        0      294 2023-05-15 12:27:07.293851 cognite_extractor_manager-0.8.2/cognite/extractorutils/cogex/_common.py
--rw-r--r--   0        0        0     5298 2023-05-15 12:27:07.293851 cognite_extractor_manager-0.8.2/cognite/extractorutils/cogex/build.py
--rw-r--r--   0        0        0     4701 2023-05-15 12:27:07.293851 cognite_extractor_manager-0.8.2/cognite/extractorutils/cogex/docker.py
--rw-r--r--   0        0        0    10553 2023-05-15 12:27:07.293851 cognite_extractor_manager-0.8.2/cognite/extractorutils/cogex/initialize.py
--rw-r--r--   0        0        0     1830 2023-05-15 12:27:07.293851 cognite_extractor_manager-0.8.2/cognite/extractorutils/cogex/io.py
--rw-r--r--   0        0        0     2334 2023-05-15 12:27:07.293851 cognite_extractor_manager-0.8.2/pyproject.toml
--rw-r--r--   0        0        0     4532 1970-01-01 00:00:00.000000 cognite_extractor_manager-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0    10173 2023-05-23 08:29:23.462868 cognite_extractor_manager-0.9.0/LICENSE
+-rw-r--r--   0        0        0     5652 2023-05-23 08:29:23.462868 cognite_extractor_manager-0.9.0/README.md
+-rw-r--r--   0        0        0      607 2023-05-23 08:29:23.462868 cognite_extractor_manager-0.9.0/cognite/extractorutils/cogex/__init__.py
+-rw-r--r--   0        0        0     3049 2023-05-23 08:29:23.466868 cognite_extractor_manager-0.9.0/cognite/extractorutils/cogex/__main__.py
+-rw-r--r--   0        0        0      294 2023-05-23 08:29:23.466868 cognite_extractor_manager-0.9.0/cognite/extractorutils/cogex/_common.py
+-rw-r--r--   0        0        0     5298 2023-05-23 08:29:23.466868 cognite_extractor_manager-0.9.0/cognite/extractorutils/cogex/build.py
+-rw-r--r--   0        0        0     4701 2023-05-23 08:29:23.466868 cognite_extractor_manager-0.9.0/cognite/extractorutils/cogex/docker.py
+-rw-r--r--   0        0        0    10553 2023-05-23 08:29:23.466868 cognite_extractor_manager-0.9.0/cognite/extractorutils/cogex/initialize.py
+-rw-r--r--   0        0        0     1830 2023-05-23 08:29:23.466868 cognite_extractor_manager-0.9.0/cognite/extractorutils/cogex/io.py
+-rw-r--r--   0        0        0     2341 2023-05-23 08:29:23.466868 cognite_extractor_manager-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     6407 1970-01-01 00:00:00.000000 cognite_extractor_manager-0.9.0/PKG-INFO
```

### Comparing `cognite_extractor_manager-0.8.2/LICENSE` & `cognite_extractor_manager-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_extractor_manager-0.8.2/cognite/extractorutils/cogex/__init__.py` & `cognite_extractor_manager-0.9.0/cognite/extractorutils/cogex/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-__version__ = "0.8.2"
+__version__ = "0.9.0"
```

### Comparing `cognite_extractor_manager-0.8.2/cognite/extractorutils/cogex/__main__.py` & `cognite_extractor_manager-0.9.0/cognite/extractorutils/cogex/__main__.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_manager-0.8.2/cognite/extractorutils/cogex/build.py` & `cognite_extractor_manager-0.9.0/cognite/extractorutils/cogex/build.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_manager-0.8.2/cognite/extractorutils/cogex/docker.py` & `cognite_extractor_manager-0.9.0/cognite/extractorutils/cogex/docker.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_manager-0.8.2/cognite/extractorutils/cogex/initialize.py` & `cognite_extractor_manager-0.9.0/cognite/extractorutils/cogex/initialize.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_manager-0.8.2/cognite/extractorutils/cogex/io.py` & `cognite_extractor_manager-0.9.0/cognite/extractorutils/cogex/io.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_manager-0.8.2/pyproject.toml` & `cognite_extractor_manager-0.9.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-extractor-manager"
-version = "0.8.2"
+version = "0.9.0"
 description = "A project manager for Python based extractors"
 authors = ["Mathias Lohne <mathias.lohne@cognite.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 packages = [
     { include="cognite", from="." },
@@ -43,25 +43,25 @@
 disallow_untyped_defs = true
 follow_imports = "normal"
 namespace_packages = true
 explicit_package_bases = true
 show_error_codes = true
 
 [tool.poetry.dependencies]
-python = "^3.8.0"
+python = ">=3.8.0,<3.12"
 termcolor = "^2.0.0"
 requests = "^2.26.0"
 toml = "^0.10.2"
+pyinstaller = "^5.0"
 
 [tool.poetry.group.dev.dependencies]
 twine = "^4.0.0"
 pre-commit = "^3.0.0"
-pyinstaller = "^4.0"
 black = "^23.3.0"
-ruff = "^0.0.265"
+ruff = "^0.0.267"
 mypy = "^1.2.0"
 types-requests = "^2.30.0.0"
 types-toml = "^0.10.8.6"
 
 
 [tool.poetry.scripts]
 cogex = "cognite.extractorutils.cogex.__main__:main"
```

### Comparing `cognite_extractor_manager-0.8.2/PKG-INFO` & `cognite_extractor_manager-0.9.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: cognite-extractor-manager
-Version: 0.8.2
-Summary: A project manager for Python based extractors
-License: Apache-2.0
-Author: Mathias Lohne
-Author-email: mathias.lohne@cognite.com
-Requires-Python: >=3.8.0,<4.0.0
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: requests (>=2.26.0,<3.0.0)
-Requires-Dist: termcolor (>=2.0.0,<3.0.0)
-Requires-Dist: toml (>=0.10.2,<0.11.0)
-Description-Content-Type: text/markdown
-
 # `cogex`
 
 `cogex` is a tool for managing extractors for Cognite Data Fusion written in Python. It provides
 utilities for initializing a new extractor project and building self-contained executables of Python
 based extractors.
 
 
@@ -78,25 +59,84 @@
 `cogex` will install all of these, and automatically run them on every commit. If you for some
 reason need to perform a commit despite one of these failing, you can run `git commit --no-verify`,
 although this is not recommended.
 
 
 ### Build and package an extractor project
 
+#### Packaging a binary of your extractor
+
 It is not always an option to rely on a Python installation at the machine your extractor will be
 deployed at. For those scenarios it is useful to package the extractor, including its dependencies
 and the Python runtime, into a single self-contained executable. To do this, run
 
 ```bash
 cogex build
 ```
 
 This will create a new executable (for the operating system you ran `cogex build` from) in the
 `dist` directory.
 
+#### Making docker images
+
+To build a docker image, you first need to add a `[tools.cogex.docker]` section to your pyproject
+file. The required fields are
+
+ * `tags`: A list of tags to tag the resulting image with. These support some simple templating, if
+   you include `{version}` in your tag, it will be replaced with the current version of the
+   extractor.
+ * If your `[tool.poetry.scripts]` includes multiple entries, you need to specify which one to use
+   in the docker image with the `entrypoint` field
+
+In addition, you have some additional fields:
+
+ * `base-image`: Which base image to use. By default, the `debian-slim` based python image for the
+   python version currently running with be chosen.
+ * `install-dir` if you want to specify where in the image the extractor should be installed
+ * `preamble` which can contain additional dockerimage statements to run in the beginning of the
+   dockerfile.
+
+Minimal example:
+
+``` toml
+[tool.cogex.docker]
+tags = ["cognite/my-extractor:{version}"]
+```
+
+Larger example (from the DB Extractor):
+
+``` toml
+[tool.cogex.docker]
+base-image = "python:3.10"
+preamble = """
+RUN apt-get update \
+    && apt-get dist-upgrade -y dirmngr gnupg gnupg-l10n gnupg-utils gpg gpg-agent gpg-wks-client gpg-wks-server \
+    && gpgconf gpgsm gpgv libssl-dev libssl1.1 openssl
+RUN apt-get install -y apt-utils build-essential
+RUN apt-get install -y unixodbc-dev unixodbc
+"""
+tags = [
+    "eu.gcr.io/cognite-registry/db-extractor-base:latest",
+    "eu.gcr.io/cognite-registry/db-extractor-base:{version}",
+    "cognite/db-extractor-base:{version}",
+]
+```
+
+You can now build and tag docker images with
+
+``` commandline
+cogex build --dockerimage
+```
+
+If you just want to see the generated dockerfile, instead run
+
+``` commandline
+cogex build --dockerfile
+```
+
 
 ### Creating a new version of your extractor
 
 To keep track of which version of the code base is running at a given deployment it is very useful
 to version your extractor. When releasing a new version, run
 
 ```bash
@@ -113,8 +153,7 @@
  * `minor` for new features or bigger improvements that __doesn't__ break compatability
  * `major` for new feature or improvements that breaks compatability with previous versions, in
    other words for those scenarios where the new version is not a drop-in replacement for an old
    version. For example:
    - When adding a new required config field
    - When removing a config field
    - When changing defaults in a way that could break existing deployments
-
```

