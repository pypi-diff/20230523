# Comparing `tmp/Publ-0.7.8.tar.gz` & `tmp/Publ-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Publ-0.7.8.tar", last modified: Wed Mar 23 20:20:58 2022, max compression
+gzip compressed data, was "Publ-0.7.9.tar", max compression
```

## Comparing `Publ-0.7.8.tar` & `Publ-0.7.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1088 2019-06-21 05:13:42.230894 Publ-0.7.8/LICENSE
--rw-r--r--   0        0        0     3462 2022-03-22 05:52:37.639949 Publ-0.7.8/README.md
--rwxr-xr-x   0        0        0      419 2022-03-22 05:52:37.640703 Publ-0.7.8/publ/__init__.py
--rw-r--r--   0        0        0       38 2022-03-23 20:18:58.342575 Publ-0.7.8/publ/__version__.py
--rw-r--r--   0        0        0     1463 2022-03-22 05:52:37.640872 Publ-0.7.8/publ/caching.py
--rw-r--r--   0        0        0     1306 2021-08-31 05:29:49.808458 Publ-0.7.8/publ/cards.py
--rw-r--r--   0        0        0    11439 2022-03-22 05:52:37.640987 Publ-0.7.8/publ/category.py
--rw-r--r--   0        0        0     5831 2022-03-22 05:52:37.641102 Publ-0.7.8/publ/cli.py
--rw-r--r--   0        0        0     2188 2022-03-22 05:52:37.641325 Publ-0.7.8/publ/config.py
--rw-r--r--   0        0        0     8259 2022-03-22 17:50:16.539192 Publ-0.7.8/publ/default_template/_admin.html
--rw-r--r--   0        0        0      373 2019-07-26 04:06:18.138581 Publ-0.7.8/publ/default_template/error.html
--rw-r--r--   0        0        0      370 2019-08-20 02:21:22.113803 Publ-0.7.8/publ/default_template/logout.html
--rw-r--r--   0        0        0    39704 2022-03-23 20:18:43.927585 Publ-0.7.8/publ/entry.py
--rw-r--r--   0        0        0    13216 2022-03-22 05:52:37.641778 Publ-0.7.8/publ/flask_wrapper.py
--rw-r--r--   0        0        0     7830 2022-03-22 05:52:37.641895 Publ-0.7.8/publ/html_entry.py
--rw-r--r--   0        0        0     8467 2022-03-22 05:52:37.642012 Publ-0.7.8/publ/image/__init__.py
--rw-r--r--   0        0        0     2899 2021-08-31 05:29:49.810060 Publ-0.7.8/publ/image/external.py
--rw-r--r--   0        0        0     7088 2022-03-22 05:52:37.642121 Publ-0.7.8/publ/image/image.py
--rw-r--r--   0        0        0    19392 2022-03-22 05:52:37.642292 Publ-0.7.8/publ/image/local.py
--rw-r--r--   0        0        0    11540 2022-03-22 05:52:37.642426 Publ-0.7.8/publ/index.py
--rw-r--r--   0        0        0     2103 2020-06-06 18:28:53.576145 Publ-0.7.8/publ/links.py
--rw-r--r--   0        0        0      901 2020-05-26 07:58:42.864566 Publ-0.7.8/publ/maintenance.py
--rw-r--r--   0        0        0    23982 2022-03-22 05:52:37.642594 Publ-0.7.8/publ/markdown.py
--rw-r--r--   0        0        0     7591 2022-03-22 17:50:16.539564 Publ-0.7.8/publ/model.py
--rw-r--r--   0        0        0     5350 2022-03-22 05:52:37.642976 Publ-0.7.8/publ/path_alias.py
--rw-r--r--   0        0        0    11612 2022-03-22 05:52:37.643120 Publ-0.7.8/publ/queries.py
--rw-r--r--   0        0        0    19380 2022-03-22 05:52:37.643284 Publ-0.7.8/publ/rendering.py
--rw-r--r--   0        0        0     6308 2022-03-22 05:52:37.643408 Publ-0.7.8/publ/search.py
--rw-r--r--   0        0        0     3650 2022-03-22 05:52:37.643516 Publ-0.7.8/publ/template.py
--rw-r--r--   0        0        0     8074 2022-03-22 20:22:26.343054 Publ-0.7.8/publ/tokens.py
--rw-r--r--   0        0        0     9822 2022-03-23 20:18:43.927982 Publ-0.7.8/publ/user.py
--rw-r--r--   0        0        0    19138 2022-03-22 20:22:26.343817 Publ-0.7.8/publ/utils.py
--rw-r--r--   0        0        0    18646 2022-03-22 05:52:37.644138 Publ-0.7.8/publ/view.py
--rw-r--r--   0        0        0      934 2022-03-23 20:18:53.183874 Publ-0.7.8/pyproject.toml
--rw-r--r--   0        0        0     4523 2022-03-23 20:20:58.989391 Publ-0.7.8/setup.py
--rw-r--r--   0        0        0     4532 2022-03-23 20:20:58.989721 Publ-0.7.8/PKG-INFO
+-rw-r--r--   0        0        0     1088 2018-04-06 06:14:16.000000 Publ-0.7.9/LICENSE
+-rw-r--r--   0        0        0     3462 2021-10-31 23:18:20.366078 Publ-0.7.9/README.md
+-rwxr-xr-x   0        0        0      419 2021-10-31 21:04:31.803187 Publ-0.7.9/publ/__init__.py
+-rw-r--r--   0        0        0       38 2022-04-29 00:33:04.019822 Publ-0.7.9/publ/__version__.py
+-rw-r--r--   0        0        0     1463 2021-10-08 03:02:31.667808 Publ-0.7.9/publ/caching.py
+-rw-r--r--   0        0        0     1306 2021-08-14 06:12:36.570975 Publ-0.7.9/publ/cards.py
+-rw-r--r--   0        0        0    11439 2021-10-31 21:04:31.803399 Publ-0.7.9/publ/category.py
+-rw-r--r--   0        0        0     5831 2021-10-31 21:08:08.745625 Publ-0.7.9/publ/cli.py
+-rw-r--r--   0        0        0     2188 2022-03-20 19:26:16.167179 Publ-0.7.9/publ/config.py
+-rw-r--r--   0        0        0     8259 2022-03-26 05:17:44.195369 Publ-0.7.9/publ/default_template/_admin.html
+-rw-r--r--   0        0        0      373 2019-10-25 19:56:11.000000 Publ-0.7.9/publ/default_template/error.html
+-rw-r--r--   0        0        0      370 2019-08-09 07:36:36.000000 Publ-0.7.9/publ/default_template/logout.html
+-rw-r--r--   0        0        0    39704 2022-03-26 05:17:44.195637 Publ-0.7.9/publ/entry.py
+-rw-r--r--   0        0        0    13216 2022-03-20 19:26:16.167610 Publ-0.7.9/publ/flask_wrapper.py
+-rw-r--r--   0        0        0     7830 2022-03-20 19:45:30.764038 Publ-0.7.9/publ/html_entry.py
+-rw-r--r--   0        0        0     8467 2021-10-06 18:10:21.076884 Publ-0.7.9/publ/image/__init__.py
+-rw-r--r--   0        0        0     2899 2021-06-17 16:44:56.711479 Publ-0.7.9/publ/image/external.py
+-rw-r--r--   0        0        0     7088 2021-10-08 03:02:31.669005 Publ-0.7.9/publ/image/image.py
+-rw-r--r--   0        0        0    19392 2021-10-06 18:10:21.077387 Publ-0.7.9/publ/image/local.py
+-rw-r--r--   0        0        0    11540 2021-10-31 21:04:31.805135 Publ-0.7.9/publ/index.py
+-rw-r--r--   0        0        0     2103 2020-06-04 05:17:08.000000 Publ-0.7.9/publ/links.py
+-rw-r--r--   0        0        0      901 2020-05-17 07:20:49.000000 Publ-0.7.9/publ/maintenance.py
+-rw-r--r--   0        0        0    23991 2022-04-29 00:34:18.692020 Publ-0.7.9/publ/markdown.py
+-rw-r--r--   0        0        0     7591 2022-03-26 05:17:44.195880 Publ-0.7.9/publ/model.py
+-rw-r--r--   0        0        0     5350 2021-10-31 21:04:31.805313 Publ-0.7.9/publ/path_alias.py
+-rw-r--r--   0        0        0    11612 2021-10-08 04:04:15.449308 Publ-0.7.9/publ/queries.py
+-rw-r--r--   0        0        0    19380 2021-10-31 21:04:31.805626 Publ-0.7.9/publ/rendering.py
+-rw-r--r--   0        0        0     6308 2021-10-08 03:03:37.476073 Publ-0.7.9/publ/search.py
+-rw-r--r--   0        0        0     3650 2021-09-08 18:33:36.855379 Publ-0.7.9/publ/template.py
+-rw-r--r--   0        0        0     8074 2022-03-26 05:17:44.196022 Publ-0.7.9/publ/tokens.py
+-rw-r--r--   0        0        0     9822 2022-03-26 05:17:44.196181 Publ-0.7.9/publ/user.py
+-rw-r--r--   0        0        0    19138 2022-03-26 05:17:44.196370 Publ-0.7.9/publ/utils.py
+-rw-r--r--   0        0        0    18646 2021-10-31 21:04:31.806750 Publ-0.7.9/publ/view.py
+-rw-r--r--   0        0        0      934 2022-04-29 00:32:57.340425 Publ-0.7.9/pyproject.toml
+-rw-r--r--   0        0        0     4523 2022-04-29 00:35:40.003783 Publ-0.7.9/setup.py
+-rw-r--r--   0        0        0     4583 2022-04-29 00:35:40.004054 Publ-0.7.9/PKG-INFO
```

### Comparing `Publ-0.7.8/LICENSE` & `Publ-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Publ-0.7.8/README.md` & `Publ-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `Publ-0.7.8/publ/caching.py` & `Publ-0.7.9/publ/caching.py`

 * *Files identical despite different names*

### Comparing `Publ-0.7.8/publ/cards.py` & `Publ-0.7.9/publ/cards.py`

 * *Files identical despite different names*

### Comparing `Publ-0.7.8/publ/category.py` & `Publ-0.7.9/publ/category.py`

 * *Files identical despite different names*

### Comparing `Publ-0.7.8/publ/cli.py` & `Publ-0.7.9/publ/cli.py`

 * *Files identical despite different names*

### Comparing `Publ-0.7.8/publ/config.py` & `Publ-0.7.9/publ/config.py`

 * *Files identical despite different names*

### Comparing `Publ-0.7.8/publ/default_template/_admin.html` & `Publ-0.7.9/publ/default_template/_admin.html`

 * *Files identical despite different names*

### Comparing `Publ-0.7.8/publ/entry.py` & `Publ-0.7.9/publ/entry.py`

 * *Files identical despite different names*

### Comparing `Publ-0.7.8/publ/flask_wrapper.py` & `Publ-0.7.9/publ/flask_wrapper.py`

 * *Files identical despite different names*

### Comparing `Publ-0.7.8/publ/html_entry.py` & `Publ-0.7.9/publ/html_entry.py`

 * *Files identical despite different names*

### Comparing `Publ-0.7.8/publ/image/__init__.py` & `Publ-0.7.9/publ/image/__init__.py`

 * *Files identical despite different names*

### Comparing `Publ-0.7.8/publ/image/external.py` & `Publ-0.7.9/publ/image/external.py`

 * *Files identical despite different names*

### Comparing `Publ-0.7.8/publ/image/image.py` & `Publ-0.7.9/publ/image/image.py`

 * *Files identical despite different names*

### Comparing `Publ-0.7.8/publ/image/local.py` & `Publ-0.7.9/publ/image/local.py`

 * *Files identical despite different names*

### Comparing `Publ-0.7.8/publ/index.py` & `Publ-0.7.9/publ/index.py`

 * *Files identical despite different names*

### Comparing `Publ-0.7.8/publ/links.py` & `Publ-0.7.9/publ/links.py`

 * *Files identical despite different names*

### Comparing `Publ-0.7.8/publ/maintenance.py` & `Publ-0.7.9/publ/maintenance.py`

 * *Files identical despite different names*

### Comparing `Publ-0.7.8/publ/markdown.py` & `Publ-0.7.9/publ/markdown.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,18 +84,18 @@
                  line_id_prefix: str,
                  link_base: typing.Union[str, bool],
                  *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.line_id_prefix = line_id_prefix
         self.link_base = link_base
 
-    def wrap(self, source, outfile):
+    def wrap(self, source, outfile=None):
         """ called by pygments """
         # pylint:disable=unused-argument
-        return self._wrap_code(source)
+        return self._wrap_pre(self._wrap_code(source))
 
     def _wrap_code(self, source):
         line_number = 0
         for i, line in source:
             if i == 1:
                 line_number += 1
                 line_id = f"{self.line_id_prefix}L{line_number}"
@@ -594,16 +594,15 @@
     def listitem(content, is_ordered, is_block):
         """ Just add the * back on """
         # pylint: disable=unused-argument
         if not is_ordered:
             return '* ' + content
         raise ValueError("Not sure how we got here")
 
-    @staticmethod
-    def header(content, level):
+    def header(self, content, level):
         """ Passthrough """
         # pylint: disable=unused-argument
         return content
 
 
 def render_title(text, markup=True, smartquotes=True, markdown_extensions=None):
     """ Convert a Markdown title to HTML """
```

### Comparing `Publ-0.7.8/publ/model.py` & `Publ-0.7.9/publ/model.py`

 * *Files identical despite different names*

### Comparing `Publ-0.7.8/publ/path_alias.py` & `Publ-0.7.9/publ/path_alias.py`

 * *Files identical despite different names*

### Comparing `Publ-0.7.8/publ/queries.py` & `Publ-0.7.9/publ/queries.py`

 * *Files identical despite different names*

### Comparing `Publ-0.7.8/publ/rendering.py` & `Publ-0.7.9/publ/rendering.py`

 * *Files identical despite different names*

### Comparing `Publ-0.7.8/publ/search.py` & `Publ-0.7.9/publ/search.py`

 * *Files identical despite different names*

### Comparing `Publ-0.7.8/publ/template.py` & `Publ-0.7.9/publ/template.py`

 * *Files identical despite different names*

### Comparing `Publ-0.7.8/publ/tokens.py` & `Publ-0.7.9/publ/tokens.py`

 * *Files identical despite different names*

### Comparing `Publ-0.7.8/publ/user.py` & `Publ-0.7.9/publ/user.py`

 * *Files identical despite different names*

### Comparing `Publ-0.7.8/publ/utils.py` & `Publ-0.7.9/publ/utils.py`

 * *Files identical despite different names*

### Comparing `Publ-0.7.8/publ/view.py` & `Publ-0.7.9/publ/view.py`

 * *Files identical despite different names*

### Comparing `Publ-0.7.8/pyproject.toml` & `Publ-0.7.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Publ"
-version = "0.7.8"
+version = "0.7.9"
 description = "A flexible web-based publishing framework"
 authors = ["fluffy <fluffy@beesbuzz.biz>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/PlaidWeb/Publ"
 homepage = "https://publ.plaidweb.site/"
```

### Comparing `Publ-0.7.8/setup.py` & `Publ-0.7.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  'awesome-slugify>=1.6.5,<2.0.0',
  'misaka>=2.1.1,<3.0.0',
  'pony>=0.7.14,<0.8.0',
  'watchdog>=1.0.2,<2.0.0']
 
 setup_kwargs = {
     'name': 'publ',
-    'version': '0.7.8',
+    'version': '0.7.9',
     'description': 'A flexible web-based publishing framework',
     'long_description': "# Publ\n\nA personal publishing platform. Like a static publishing system, only dynamic.\n\n## Motivation\n\nI make a lot of different things — comics, music, art, code, games — and none of\nthe existing content management systems I found quite satisfied my use cases.\nEither they don't allow enough flexibility in the sorts of content that they can\nprovide, or the complexity in managing the content makes it more complicated than\nsimply hand-authoring a site.\n\nI wanted to bring the best of the classic static web to a more dynamic\npublishing system; scheduled posts, private posts, category-based templates, and\nbuilt-in support for image renditions (including thumbnails, high-DPI support,\nand image galleries). And I want to do it all using simple Markdown files\norganized in a sensible file hierarchy.\n\n## Basic tenets\n\n* Containerized web app that's deployable with little friction (hopefully)\n* Do one thing (present heterogeneous content), do it well (hopefully)\n* Use external tools for site content editing\n* Be CDN-friendly\n* High-DPI images and image sets as first-class citizens\n* Interoperate with everything that's open for interoperation (especially [IndieWeb](http://indieweb.org))\n\n## See it in action\n\nThe main demonstration site is at https://beesbuzz.biz/ — it is of course a\nwork in progress! The documentation site for Publ itself (which is also a work in progress) lives at https://publ.plaidweb.site/\n\n## Operating requirements\n\nI am designing this to work in any WSGI-capable environment with a supported\nversion of Python. This means that it will, for example, be deployable on any\nshared hosting which has Passenger support (such as Dreamhost), as well as on\nHeroku, Google AppEngine, S3, or any other simple containerized deployment\ntarget.\n\nThe file system is the ground truth for all site data, and while it does use a\ndatabase as a content index, the actual choice of database doesn't matter all\nthat much. A typical deployment will use SQLite, but MySQL, Postgres, Oracle,\nand Cockroach are also supported.\n\n## Developing Publ\n\nIn order to develop Publ itself, you'll need to install its dependencies; see\nthe [getting started\nguide](http://publ.plaidweb.site/manual/328-Getting-started) for more\ninformation. In particular, make sure you have compatible versions of\n[Python](https://python.org/) and [Poetry](https://python-poetry.org/)\ninstalled, and, if on Windows, you'll probably need to install the [Visual C++\nbuild tools](https://visualstudio.microsoft.com/downloads/).\n\nAs far as developing Publ itself goes, cloning this repository and running\n`./runTests.sh` (Linux/macOS/etc.) or `wintests.cmd` (Windows) should get you up\nand running. The runtime manual test suite site lives in `tests/` (with the\nactual site content in `content/`, `templates/` and `static/`).\n\nFor developing CLI functionality, you'll have to override the `FLASK_APP`\nenvironment variable to be `test_app.py`.\n\n## Additional resources\n\nThe [Publ-site](https://github.com/PlaidWeb/Publ-site) repository stores all of\nthe templates, site content, and configuration for the [Publ\nsite](https://publ.plaidweb.site).\n\nThe\n[Publ-templates-beesbuzz.biz](https://github.com/PlaidWeb/Publ-templates-beesbuzz.biz)\nrepository provides a stripped-down sample site based on [my personal\nhomepage](https://beesbuzz.biz).\n\n## Authors\n\nIn order of first contribution:\n\n* [fluffy](https://github.com/fluffy-critter)\n* [karinassuni](https://github.com/karinassuni)\n",
     'author': 'fluffy',
     'author_email': 'fluffy@beesbuzz.biz',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://publ.plaidweb.site/',
```

### Comparing `Publ-0.7.8/PKG-INFO` & `Publ-0.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: publ
-Version: 0.7.8
+Version: 0.7.9
 Summary: A flexible web-based publishing framework
 Home-page: https://publ.plaidweb.site/
 License: MIT
 Author: fluffy
 Author-email: fluffy@beesbuzz.biz
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Flask (>=2.0.0,<3.0.0)
 Requires-Dist: Flask-Caching (>=1.9.0,<2.0.0)
 Requires-Dist: Pillow (>=9.0.0,<10.0.0)
 Requires-Dist: Pygments (>=2.7.3,<3.0.0)
```

