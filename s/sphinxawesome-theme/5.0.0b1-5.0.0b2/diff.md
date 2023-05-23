# Comparing `tmp/sphinxawesome_theme-5.0.0b1.tar.gz` & `tmp/sphinxawesome_theme-5.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxawesome_theme-5.0.0b1.tar", max compression
+gzip compressed data, was "sphinxawesome_theme-5.0.0b2.tar", max compression
```

## Comparing `sphinxawesome_theme-5.0.0b1.tar` & `sphinxawesome_theme-5.0.0b2.tar`

### file list

```diff
@@ -1,51 +1,50 @@
--rw-r--r--   0        0        0     1066 2023-05-12 16:19:07.291156 sphinxawesome_theme-5.0.0b1/LICENSE
--rw-r--r--   0        0        0     2628 2023-05-12 16:19:07.291156 sphinxawesome_theme-5.0.0b1/README.md
--rw-r--r--   0        0        0     2375 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/pyproject.toml
--rw-r--r--   0        0        0      172 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/README.rst
--rw-r--r--   0        0        0     7050 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/__init__.py
--rw-r--r--   0        0        0     1194 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/breadcrumbs.html
--rw-r--r--   0        0        0     5522 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/deprecated.py
--rw-r--r--   0        0        0     6185 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/docsearch.py
--rw-r--r--   0        0        0     1394 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/footer.html
--rw-r--r--   0        0        0     7631 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/header.html
--rw-r--r--   0        0        0    12730 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/highlighting.py
--rw-r--r--   0        0        0      820 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/icons.py
--rw-r--r--   0        0        0     2133 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/jinja_functions.py
--rw-r--r--   0        0        0     1191 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/jsonimpl.py
--rw-r--r--   0        0        0     5307 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/layout.html
--rw-r--r--   0        0        0     3241 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/logos.py
--rw-r--r--   0        0        0      895 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/page.html
--rw-r--r--   0        0        0     7375 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/postprocess.py
--rw-r--r--   0        0        0     1603 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/prev_next.html
--rw-r--r--   0        0        0      656 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/scrolltop.html
--rw-r--r--   0        0        0      920 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/search.html
--rw-r--r--   0        0        0     1370 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/searchbox.html
--rw-r--r--   0        0        0     2462 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/sidebar.html
--rw-r--r--   0        0        0      416 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/sidebar_main_nav_links.html
--rw-r--r--   0        0        0      256 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/sidebar_toc.html
--rw-r--r--   0        0        0    28348 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/09be83022f2ac2ce16b0.woff
--rw-r--r--   0        0        0    28288 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/0ffeb7a552b36437b54c.woff
--rw-r--r--   0        0        0    22192 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/31f64b9c465158bd6066.woff2
--rw-r--r--   0        0        0    26760 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/44fd0da18fe361a5cc7f.woff
--rw-r--r--   0        0        0    26680 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/46830c334f8112fa510a.woff
--rw-r--r--   0        0        0    25940 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/6f04107ce68d524ebe69.woff
--rw-r--r--   0        0        0    27532 2023-05-12 16:19:07.299156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/ad463ea60cc8b68792f4.woff
--rw-r--r--   0        0        0        0 2023-05-12 16:19:07.299156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/awesome-sphinx-design.31d6cfe0d16ae931b73c.js
--rw-r--r--   0        0        0     1278 2023-05-12 16:19:07.299156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/awesome-sphinx-design.f3507627e0af8330cfa7.css
--rw-r--r--   0        0        0    22228 2023-05-12 16:19:07.299156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/c3b5f43fe4c8f3f1fa21.woff2
--rw-r--r--   0        0        0    21080 2023-05-12 16:19:07.299156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/cfdd43ce3499ca7f900a.woff2
--rw-r--r--   0        0        0    20388 2023-05-12 16:19:07.299156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/d0b41bd1d599bc0a52b7.woff2
--rw-r--r--   0        0        0    19886 2023-05-12 16:19:07.299156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/docsearch.445222223e83896718c6.css
--rw-r--r--   0        0        0   108012 2023-05-12 16:19:07.299156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/docsearch.f1a1a5835ed7a6ab0c85.js
--rw-r--r--   0        0        0      109 2023-05-12 16:19:07.299156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/docsearch.f1a1a5835ed7a6ab0c85.js.LICENSE.txt
--rw-r--r--   0        0        0      704 2023-05-12 16:19:07.299156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/docsearch_config.js_t
--rw-r--r--   0        0        0    20932 2023-05-12 16:19:07.299156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/ec416b97881f4a422686.woff2
--rw-r--r--   0        0        0    21412 2023-05-12 16:19:07.299156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/ff058b7e238adc5cba09.woff2
--rw-r--r--   0        0        0     1590 2023-05-12 16:19:07.299156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/manifest.json
--rw-r--r--   0        0        0    48804 2023-05-12 16:19:07.299156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/theme.a16405b310edf0713aee.css
--rw-r--r--   0        0        0    52713 2023-05-12 16:19:07.299156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/theme.ad172c0f1249198ea036.js
--rw-r--r--   0        0        0       93 2023-05-12 16:19:07.299156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/theme.ad172c0f1249198ea036.js.LICENSE.txt
--rw-r--r--   0        0        0      470 2023-05-12 16:19:07.299156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/theme.conf
--rw-r--r--   0        0        0      357 2023-05-12 16:19:07.299156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/toc.html
--rw-r--r--   0        0        0     2086 2023-05-12 16:19:07.299156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/toc.py
--rw-r--r--   0        0        0     3678 1970-01-01 00:00:00.000000 sphinxawesome_theme-5.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-05-23 10:00:38.530395 sphinxawesome_theme-5.0.0b2/LICENSE
+-rw-r--r--   0        0        0     2421 2023-05-23 10:00:38.530395 sphinxawesome_theme-5.0.0b2/README.md
+-rw-r--r--   0        0        0     2580 2023-05-23 10:00:38.534395 sphinxawesome_theme-5.0.0b2/pyproject.toml
+-rw-r--r--   0        0        0      172 2023-05-23 10:00:38.534395 sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/README.rst
+-rw-r--r--   0        0        0     7050 2023-05-23 10:00:38.534395 sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/__init__.py
+-rw-r--r--   0        0        0     1194 2023-05-23 10:00:38.534395 sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/breadcrumbs.html
+-rw-r--r--   0        0        0     5522 2023-05-23 10:00:38.534395 sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/deprecated.py
+-rw-r--r--   0        0        0     6185 2023-05-23 10:00:38.534395 sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/docsearch.py
+-rw-r--r--   0        0        0     1394 2023-05-23 10:00:38.534395 sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/footer.html
+-rw-r--r--   0        0        0     7631 2023-05-23 10:00:38.534395 sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/header.html
+-rw-r--r--   0        0        0    12728 2023-05-23 10:00:38.534395 sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/highlighting.py
+-rw-r--r--   0        0        0     2133 2023-05-23 10:00:38.534395 sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/jinja_functions.py
+-rw-r--r--   0        0        0     1191 2023-05-23 10:00:38.534395 sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/jsonimpl.py
+-rw-r--r--   0        0        0     5307 2023-05-23 10:00:38.534395 sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/layout.html
+-rw-r--r--   0        0        0     3241 2023-05-23 10:00:38.534395 sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/logos.py
+-rw-r--r--   0        0        0      895 2023-05-23 10:00:38.534395 sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/page.html
+-rw-r--r--   0        0        0     8436 2023-05-23 10:00:38.534395 sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/postprocess.py
+-rw-r--r--   0        0        0     1603 2023-05-23 10:00:38.534395 sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/prev_next.html
+-rw-r--r--   0        0        0      656 2023-05-23 10:00:38.534395 sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/scrolltop.html
+-rw-r--r--   0        0        0      920 2023-05-23 10:00:38.534395 sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/search.html
+-rw-r--r--   0        0        0     1370 2023-05-23 10:00:38.534395 sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/searchbox.html
+-rw-r--r--   0        0        0     2462 2023-05-23 10:00:38.534395 sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/sidebar.html
+-rw-r--r--   0        0        0      416 2023-05-23 10:00:38.534395 sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/sidebar_main_nav_links.html
+-rw-r--r--   0        0        0      256 2023-05-23 10:00:38.534395 sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/sidebar_toc.html
+-rw-r--r--   0        0        0    21420 2023-05-23 10:00:38.534395 sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/static/0ff19efc74e94c856af0.woff2
+-rw-r--r--   0        0        0    27956 2023-05-23 10:00:38.534395 sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/static/26400cae88e50682937d.woff
+-rw-r--r--   0        0        0    21848 2023-05-23 10:00:38.534395 sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/static/2a472f0334546ace60b3.woff2
+-rw-r--r--   0        0        0    27996 2023-05-23 10:00:38.534395 sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/static/3925889378745d0382d0.woff
+-rw-r--r--   0        0        0    20740 2023-05-23 10:00:38.534395 sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/static/4163112e566ed7697acf.woff2
+-rw-r--r--   0        0        0    29556 2023-05-23 10:00:38.534395 sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/static/5b12b1b913a1d0348fc6.woff
+-rw-r--r--   0        0        0    27272 2023-05-23 10:00:38.534395 sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/static/6c1a3008005254946aef.woff
+-rw-r--r--   0        0        0    22668 2023-05-23 10:00:38.534395 sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/static/aef37e2fab43d03531cd.woff2
+-rw-r--r--   0        0        0        0 2023-05-23 10:00:38.534395 sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/static/awesome-sphinx-design.31d6cfe0d16ae931b73c.js
+-rw-r--r--   0        0        0     1278 2023-05-23 10:00:38.534395 sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/static/awesome-sphinx-design.f3507627e0af8330cfa7.css
+-rw-r--r--   0        0        0    29516 2023-05-23 10:00:38.534395 sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/static/b8546ea1646db8ea9c7f.woff
+-rw-r--r--   0        0        0    22592 2023-05-23 10:00:38.534395 sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/static/c10c163dd1c289f11c49.woff2
+-rw-r--r--   0        0        0    19886 2023-05-23 10:00:38.534395 sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/static/docsearch.82e38f6cd0ccc11d77d4.css
+-rw-r--r--   0        0        0   108052 2023-05-23 10:00:38.538396 sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/static/docsearch.8cecda6602174cdd6086.js
+-rw-r--r--   0        0        0      109 2023-05-23 10:00:38.538396 sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/static/docsearch.8cecda6602174cdd6086.js.LICENSE.txt
+-rw-r--r--   0        0        0      704 2023-05-23 10:00:38.538396 sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/static/docsearch_config.js_t
+-rw-r--r--   0        0        0    21356 2023-05-23 10:00:38.538396 sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/static/f4604891b5f1fc1bdbe5.woff2
+-rw-r--r--   0        0        0    28788 2023-05-23 10:00:38.538396 sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/static/f509ddf49c74ded8c0ee.woff
+-rw-r--r--   0        0        0     1590 2023-05-23 10:00:38.538396 sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/static/manifest.json
+-rw-r--r--   0        0        0    49068 2023-05-23 10:00:38.538396 sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/static/theme.871137ef162fc5460fb0.css
+-rw-r--r--   0        0        0    52292 2023-05-23 10:00:38.538396 sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/static/theme.929b2cdd5fa757959a38.js
+-rw-r--r--   0        0        0       93 2023-05-23 10:00:38.538396 sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/static/theme.929b2cdd5fa757959a38.js.LICENSE.txt
+-rw-r--r--   0        0        0      470 2023-05-23 10:00:38.538396 sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/theme.conf
+-rw-r--r--   0        0        0      357 2023-05-23 10:00:38.538396 sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/toc.html
+-rw-r--r--   0        0        0     2086 2023-05-23 10:00:38.538396 sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/toc.py
+-rw-r--r--   0        0        0     3471 1970-01-01 00:00:00.000000 sphinxawesome_theme-5.0.0b2/PKG-INFO
```

### Comparing `sphinxawesome_theme-5.0.0b1/LICENSE` & `sphinxawesome_theme-5.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.0.0b1/README.md` & `sphinxawesome_theme-5.0.0b2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -26,30 +26,19 @@
 
    ```python
    html_theme = "sphinxawesome_theme"
    ```
 
    For more information, see [Add your theme](https://sphinxawesome.xyz/how-to/add/).
 
-1. Optional:
-
-   - If you want to use Algolia DocSearch with this theme,
-     load the bundled extension:
-
-     ```python
-     # conf.py
-     extensions += ["sphinxawesome_theme.docsearch"]
-     ```
-
-   - If you want to use awesome features for highlighting code,
-     load the bundled extension:
+1. Optional: add bundled extensions for more awesome features:
 
      ```python
      # conf.py
-     extensions += ["sphinxawesome_theme.highlighting"]
+     extensions += ["sphinxawesome_theme.docsearch", "sphinxawesome.highlighting"]
      ```
 
 ## Features
 
 With the Awesome Theme, you can build readable, functional, and beautiful documentation websites.
 
 ### Awesome code blocks
```

#### html2text {}

```diff
@@ -3,20 +3,18 @@
  Create beautiful and awesome documentation websites with Sphinx. See how the
                     theme looks like on sphinxawesome.xyz.
 ## Get started 1. Install the theme as a Python package: ```console pip install
 sphinxawesome-theme ``` For more information, see [Install the theme](https://
 sphinxawesome.xyz/how-to/install/). 1. Add `sphinxawesome_theme` as an HTML
 theme in your Sphinx configuration file `conf.py`: ```python html_theme =
 "sphinxawesome_theme" ``` For more information, see [Add your theme](https://
-sphinxawesome.xyz/how-to/add/). 1. Optional: - If you want to use Algolia
-DocSearch with this theme, load the bundled extension: ```python # conf.py
-extensions += ["sphinxawesome_theme.docsearch"] ``` - If you want to use
-awesome features for highlighting code, load the bundled extension: ```python #
-conf.py extensions += ["sphinxawesome_theme.highlighting"] ``` ## Features With
-the Awesome Theme, you can build readable, functional, and beautiful
+sphinxawesome.xyz/how-to/add/). 1. Optional: add bundled extensions for more
+awesome features: ```python # conf.py extensions +=
+["sphinxawesome_theme.docsearch", "sphinxawesome.highlighting"] ``` ## Features
+With the Awesome Theme, you can build readable, functional, and beautiful
 documentation websites. ### Awesome code blocks - Code block have a **Copy**
 button for copying the code. - If you load the bundled
 `sphinxawesome_theme.highlighting`, you can use these additional options in
 your ``code-block`` directives: - `emphasize-added`. Highlight lines that
 should be added to code - `emphasize-removed`. Highlight lines that should be
 removed from the code - `emphasize-text: TEXT`. Highlight _`TEXT`_ in the code
 block to emphasize placeholder text. ### Better headerlinks Clicking the link
```

### Comparing `sphinxawesome_theme-5.0.0b1/pyproject.toml` & `sphinxawesome_theme-5.0.0b2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sphinxawesome-theme"
-version = "5.0.0-beta.1"
+version = "5.0.0-beta.2"
 description = "An awesome theme for the Sphinx documentation generator"
 readme = "README.md"
 authors = ["Kai Welke <kai687@pm.me>"]
 homepage = "https://sphinxawesome.xyz"
 documentation = "https://sphinxawesome.xyz"
 repository = "https://github.com/kai687/sphinxawesome-theme"
 license = "MIT"
@@ -33,19 +33,20 @@
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2"
 pytest-cov = "^4.0"
 coverage = { extras = ["toml"], version = "^7.2" }
 types-docutils = "^0.19.1.6"
 mypy = "^1.0"
+commitizen = "^3.2.2"
 
 [tool.poetry.group.lint.dependencies]
 black = "^23.1"
 pre-commit = "^3.1.1"
-ruff = "^0.0.265"
+ruff = "^0.0.269"
 
 [tool.poetry.group.netlify.dependencies]
 nox = {version = "^2023.4.22", python = "3.8"}
 poetry = {version = "^1.4.2", python = "3.8"}
 pipx = {version = "^1.2.0", python = "3.8"}
 pip = {version = "^23.1.2", python = "3.8"}
 
@@ -83,10 +84,17 @@
 [[tool.mypy.overrides]]
 module = ["pygments.*", "dotenv", "sphinxcontrib.serializinghtml", "nox_poetry", "bs4"]
 ignore_missing_imports = true
 
 [tool.poetry.plugins."sphinx.html_themes"]
 sphinxawesome_theme = "sphinxawesome_theme"
 
+
+[tool.commitizen]
+name = "cz_conventional_commits"
+tag_format = "$major.$minor.$patch$prerelease"
+version_type = "semver"
+version_provider = "poetry"
+update_changelog_on_bump = true
 [build-system]
 requires = ["poetry_core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/__init__.py` & `sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/breadcrumbs.html` & `sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/deprecated.py` & `sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/deprecated.py`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/docsearch.py` & `sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/docsearch.py`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/footer.html` & `sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/footer.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/header.html` & `sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/header.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/highlighting.py` & `sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/highlighting.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,66 +3,77 @@
 This extension extends the Sphinx ``code-block``
 directive with new options:
 
 - ``:emphasize-added:``: highlight added lines
 - ``:emphasize-removed:``: highlight removed lines
 - ``:emphasize-text:``: highlight a single word, such as, a placeholder
 
-To achieve this, this extension must make a few larger changes:
-
-1. Provide a custom Sphinx translator to parse the new code block options.
-2. Provide a new Sphinx directive to pass along these new options to Pygments.
-3. Write a new Pygments HTML formatter and a custom filter to handle these options.
-
-It's entirely possible that there's a simpler way of doing this,
-but I haven't found it.
-
 To load this extension, add:
 
 .. code-block:: python
-   :caption: |conf|
+   :caption: File: conf.py
 
    extensions += ["sphinxawesome_theme.highlighting"]
 
+To achieve this, this extension makes a few larger changes:
+
+1. Provide a new Sphinx directive: ``AwesomeCodeBlock``.
+   This parses the additional options and passes them to the syntax highlighter.
+
+2. Provide a new Pygments HTML formatter ``AwesomeHtmlFormatter``.
+   This handles formatting the lines for added or removed options.
+   This extension changes the output compared to the default Sphinx implementation.
+   For example, each line is wrapped in a ``<span>`` element,
+   and the whole code block is wrapped in a ``<pre><code>..`` element.
+   For highlighted lines, this extension uses ``<mark>``, ``<ins>``, and ``<del>`` elements.
+
+3. Define a new custom Pygments filter ``AwesomePlaceholders``,
+   which wraps each encountered placeholder word in a ``Generic.Emphasized`` token,
+   such that we can style placeholders by CSS.
+
+4. Monkey-patch the ``PygmentsBridge.get_lexer`` method to apply the ``AwesomePlaceholders`` filter,
+   if the option for it is present.
+
+5. Monkey-patch the ``PygmentsBridge.highlight_block`` method to pass the option for highlighting text to the ``get_lexer`` method.
+
 :copyright: Copyright Kai Welke.
 :license: MIT, see LICENSE for details.
 """
 from __future__ import annotations
 
 import re
-from typing import Any, Generator, Pattern, Tuple, Union
+from typing import Any, Generator, Literal, Pattern, Tuple, Union
 
 from docutils import nodes
-from docutils.nodes import Element, Node
+from docutils.nodes import Node
 from docutils.parsers.rst import directives
-from pygments import highlight
 from pygments.filter import Filter
-from pygments.filters import ErrorToken
 from pygments.formatters import HtmlFormatter
+from pygments.lexer import Lexer
 from pygments.token import Generic, _TokenType
 from pygments.util import get_list_opt
 from sphinx.application import Sphinx
-from sphinx.directives.code import CodeBlock, container_wrapper, dedent_lines
+from sphinx.directives.code import CodeBlock
 from sphinx.highlighting import PygmentsBridge
 from sphinx.locale import __
-from sphinx.util import logging, parselinenos, texescape
+from sphinx.util import logging, parselinenos
 
 from . import __version__
 
 logger = logging.getLogger(__name__)
 
 # type alias
 TokenType = Union[_TokenType, int]  # For Python 3.8
 TokenStream = Generator[Tuple[TokenType, str], None, None]
 
 
 def _replace_placeholders(
     ttype: _TokenType, value: str, regex: Pattern[str]
 ) -> TokenStream:
-    """Replace every occurence of `regex` with `Generic.Emph` token."""
+    """Replace every occurence of ``regex`` with ``Generic.Emph`` token."""
     last = 0
     for match in regex.finditer(value):
         start, end = match.start(), match.end()
         if start != last:
             yield ttype, value[last:start]
         yield Generic.Emph, value[start:end]
         last = end
@@ -71,75 +82,88 @@
 
 
 # Without the comment, `mypy` throws a fit:
 # Cannot subclass Filter, is type `Any`
 
 
 class AwesomePlaceholders(Filter):  # type: ignore[misc]
-    """A Pygments filter for marking up placeholder text."""
+    """A Pygments filter for marking up placeholder text.
+
+    You can define the text to highlight with the ``hl_text`` option.
+    To add the filter to a Pygments lexer, use the ``add_filter`` method:
+
+    .. code-block:: python
+
+       f = AwesomePlaceholders(hl_text=TEXT)
+       lexer.add_filter(AwesomePlaceholders(hl_text=TEXT))
+
+    For more information, see the `Pygments documentation <https://pygments.org/docs/quickstart/>`__.
+    """
 
     def __init__(self: AwesomePlaceholders, **options: str) -> None:
-        """Create an instance of the `AwesomePlaceholders` filter."""
+        """Create an instance of the ``AwesomePlaceholders`` filter."""
         Filter.__init__(self, **options)
         placeholders = get_list_opt(options, "hl_text", [])
         self.placeholders_re = re.compile(
             r"|".join([re.escape(x) for x in placeholders if x])
         )
 
     def filter(
         self: AwesomePlaceholders, _lexer: Any, stream: TokenStream
     ) -> TokenStream:
         """Filter on all tokens.
 
-        The `lexer` is required by the parent class.
+        The ``lexer`` instance is required by the parent class, but isn't used here.
         """
         regex = self.placeholders_re
         for ttype, value in stream:
             yield from _replace_placeholders(ttype, value, regex)
 
 
 class AwesomeHtmlFormatter(HtmlFormatter):  # type: ignore
-    """Custom HTML formatter for Pygments.
-
-    Allow highlighting added or removed lines.
-    Similar to emphasizing lines.
+    """Custom Pygments HTML formatter for highlighting added or removed lines.
 
-    In contrast to Pygments, this formatter returns `<mark>` for higlighted lines.
+    The method is similar to handling the ``hl_lines`` option in the regular HtmlFormatter.
     """
 
-    def __init__(self: AwesomeHtmlFormatter, **options: Any) -> None:
-        """Implement `hl_added` and `hl_removed` options."""
-        self.added_lines = set()
-        self.removed_lines = set()
-
-        for lineno in get_list_opt(options, "hl_added", []):
+    def _get_line_numbers(
+        self: AwesomeHtmlFormatter,
+        options: dict[str, Any],
+        which: Literal["hl_added", "hl_removed"],
+    ) -> set[int]:
+        """Get the lines to be added or removed."""
+        line_numbers = set()
+        for lineno in get_list_opt(options, which, []):
             try:
-                self.added_lines.add(int(lineno))
+                line_numbers.add(int(lineno))
             except ValueError:
                 pass
+        return line_numbers
 
-        for lineno in get_list_opt(options, "hl_removed", []):
-            try:
-                self.removed_lines.add(int(lineno))
-            except ValueError:
-                pass
+    def __init__(self: AwesomeHtmlFormatter, **options: Any) -> None:
+        """Implement `hl_added` and `hl_removed` options.
+
+        Also set the ``linespans`` and ``wrapcode`` options of the Pygments HTML formatter to ``True``.
+        """
+        self.added_lines = self._get_line_numbers(options, "hl_added")
+        self.removed_lines = self._get_line_numbers(options, "hl_removed")
 
         # These options aren't compatible with `sphinx.ext.autodoc`
         # options["lineanchors"] = "code"
         options["linespans"] = "line"
         options["wrapcode"] = True
 
         super().__init__(**options)
 
     def _highlight_lines(
         self: AwesomeHtmlFormatter, tokensource: TokenStream
     ) -> TokenStream:
         """Highlight added, removed, and emphasized lines.
 
-        In contrast to Pygments, use `<mark>`, `<ins>`, and `<del>` elements.
+        In contrast to Pygments, use ``<mark>``, ``<ins>``, and ``<del>`` elements.
         """
         for i, (t, value) in enumerate(tokensource):
             if t != 1:
                 yield t, value
             if i + 1 in self.hl_lines:
                 yield 1, "<mark>%s</mark>" % value
             elif i + 1 in self.added_lines:
@@ -181,174 +205,146 @@
             if self.full:
                 source = self._wrap_full(source, outfile)
 
         for _, piece in source:
             outfile.write(piece)
 
 
-def _get_parsed_line_numbers(linespec: str, nlines: int, location: str) -> list[int]:
-    """Get the parsed line numbers for the `emphasize-*` options."""
-    line_numbers = parselinenos(linespec, nlines)
-    if any(i >= nlines for i in line_numbers):
-        logger.warning(
-            __("line number spec is out of range(1-%d): %r") % (nlines, linespec),
-            location=location,
-        )
-    return [x + 1 for x in line_numbers if x < nlines]
-
-
 class AwesomeCodeBlock(CodeBlock):
-    """Add options to highlight added and removed lines to `code-block` directives."""
+    """An extension of the Sphinx ``code-block`` directive to handle additional options.
+
+    - ``:emphasize-added:`` highlight added lines
+    - ``:emphasize-removed:`` highlight removed lines
+    - ``:emphasize-text:`` highlight placeholder text
+
+    The job of the directive is to set the correct options to the ``literal_block`` node,
+    which represents a code block in the parsed reStructuredText tree.
+    When transforming the abstract tree to HTML,
+    Sphinx passes these options to the ``highlight_block`` method,
+    which is a wrapper around Pygments' ``highlight`` method.
+    Handling these options is then a job of the ``AwesomePygmentsBridge``.
+    """
 
     new_options = {
         "emphasize-added": directives.unchanged_required,
         "emphasize-removed": directives.unchanged_required,
         "emphasize-text": directives.unchanged_required,
     }
 
     option_spec = CodeBlock.option_spec
     option_spec.update(new_options)
 
-    def run(self: AwesomeCodeBlock) -> list[Node]:  # noqa
-        """Overwrite method from Sphinx.
-
-        Add ability to highlight added and removed lines.
-        This passes the options to the highlighter.
-        You need a custom pygments formatter.
-
-        Unfortunately, the original method doesn't lend itself to being extended,
-        so I had to copy it.
-        """
+    def _get_line_numbers(
+        self: AwesomeCodeBlock, option: Literal["emphasize-added", "emphasize-removed"]
+    ) -> list[int] | None:
+        """Parse the line numbers for the ``:emphasize-added:`` and ``:emphasize-removed:`` options."""
         document = self.state.document
-        code = "\n".join(self.content)
         location = self.state_machine.get_source_and_line(self.lineno)
         nlines = len(self.content)
+        linespec = self.options.get(option)
 
-        hl_lines = hl_added = hl_removed = None
-        linespec = self.options.get("emphasize-lines")
-        if linespec:
-            try:
-                hl_lines = _get_parsed_line_numbers(linespec, nlines, location)
-            except ValueError as err:
-                return [document.reporter.warning(err, line=self.lineno)]
-
-        linespec = self.options.get("emphasize-added")
-        if linespec:
-            try:
-                hl_added = _get_parsed_line_numbers(linespec, nlines, location)
-            except ValueError as err:
-                return [document.reporter.warning(err, line=self.lineno)]
+        if not linespec:
+            return None
 
-        linespec = self.options.get("emphasize-removed")
-        if linespec:
-            try:
-                hl_removed = _get_parsed_line_numbers(linespec, nlines, location)
-            except ValueError as err:
-                return [document.reporter.warning(err, line=self.lineno)]
-
-        if "dedent" in self.options:
-            lines = code.splitlines(True)
-            lines = dedent_lines(lines, self.options["dedent"], location=location)
-            code = "".join(lines)
-
-        literal: Element = nodes.literal_block(code, code)
-        if "linenos" in self.options or "lineno-start" in self.options:
-            literal["linenos"] = True
-        literal["classes"] += self.options.get("class", [])
-        literal["force"] = "force" in self.options
-        if self.arguments:
-            # highlight language specified
-            literal["language"] = self.arguments[0]
-        else:
-            # no highlight language specified.  Then this directive refers the current
-            # highlight setting via ``highlight`` directive or ``highlight_language``
-            # configuration.
-            literal["language"] = self.env.temp_data.get(
-                "highlight_language", self.config.highlight_language
-            )
-        extra_args = literal["highlight_args"] = {}
-        if hl_lines is not None:
-            extra_args["hl_lines"] = hl_lines
-        if hl_added is not None:
-            extra_args["hl_added"] = hl_added
-        if hl_removed is not None:
-            extra_args["hl_removed"] = hl_removed
-        if "lineno-start" in self.options:
-            extra_args["linenostart"] = self.options["lineno-start"]
-        if "emphasize-text" in self.options:
-            extra_args["hl_text"] = self.options["emphasize-text"]
+        try:
+            line_numbers = parselinenos(linespec, nlines)
+            if any(i >= nlines for i in line_numbers):
+                logger.warning(
+                    __("line number spec is out of range(1-%d): %r")
+                    % (nlines, linespec),
+                    location=location,
+                )
+            return [i + 1 for i in line_numbers if i < nlines]
+        except ValueError as err:
+            return [document.reporter.warning(err, line=self.lineno)]
+
+    def run(self: AwesomeCodeBlock) -> list[Node]:
+        """Handle parsing extra options for highlighting."""
+        literal_nodes = super().run()
+
+        hl_added = self._get_line_numbers("emphasize-added")
+        hl_removed = self._get_line_numbers("emphasize-removed")
+
+        # `literal_nodes` is either `[literal_block]`, or `[caption, literal_block]`
+        for node in literal_nodes:
+            if isinstance(node, nodes.literal_block):
+                extra_args = node.get("highlight_args", {})
+
+                if hl_added is not None:
+                    extra_args["hl_added"] = hl_added
+                if hl_removed is not None:
+                    extra_args["hl_removed"] = hl_removed
+                if "emphasize-text" in self.options:
+                    extra_args["hl_text"] = self.options["emphasize-text"]
+
+        return literal_nodes
+
+
+# These external references are needed, or you'll get a maximum recursion depth error
+pygmentsbridge_get_lexer = PygmentsBridge.get_lexer
+pygmentsbridge_highlight_block = PygmentsBridge.highlight_block
 
-        self.set_source_info(literal)
 
-        caption = self.options.get("caption")
-        if caption:
-            try:
-                literal = container_wrapper(self, literal, caption)
-            except ValueError as exc:
-                return [document.reporter.warning(exc, line=self.lineno)]
-
-        # literal will be note_implicit_target that is linked from caption and numref.
-        # when options['name'] is provided, it should be primary ID.
-        self.add_name(literal)
+class AwesomePygmentsBridge(PygmentsBridge):
+    """Monkey-patch the Pygments methods to handle highlighting placeholder text."""
 
-        return [literal]
+    def get_lexer(
+        self: AwesomePygmentsBridge,
+        source: str,
+        lang: str,
+        opts: dict[str, Any] | None = None,
+        force: bool = False,
+        location: Any = None,
+    ) -> Lexer:
+        """Monkey-patch the ``PygmentsBridge.get_lexer`` method.
 
+        Adds a filter to lexers if the ``hl_text`` option is present.
+        """
+        lexer = pygmentsbridge_get_lexer(self, source, lang, opts, force, location)
 
-class AwesomePygmentsBridge(PygmentsBridge):
-    """Class for monkeypatching."""
+        if opts and "hl_text" in opts:
+            lexer.add_filter(AwesomePlaceholders(hl_text=opts["hl_text"]))
+        return lexer
 
     def highlight_block(
-        self: PygmentsBridge,
+        self: AwesomePygmentsBridge,
         source: str,
         lang: str,
         opts: dict[str, Any] | None = None,
         force: bool = False,
         location: Any = None,
         **kwargs: Any,
     ) -> str:
-        """Repeat this method."""
-        if not isinstance(source, str):
-            source = source.decode()  # type: ignore[unreachable]
+        """Monkey-patch the ``PygmentsBridge.highlight_block`` method.
+
+        This method is called, when Sphinx transforms the abstract document tree
+        to HTML and encounters code blocks.
+        The ``hl_text`` option is passed in the ``kwargs`` dictionary.
+        For the ``get_lexer`` method, we need to pass it in the ``opts`` dictionary.
+        """
+        if opts is None:
+            opts = {}
 
-        lexer = self.get_lexer(source, lang, opts, force, location)
         hl_text = get_list_opt(kwargs, "hl_text", [])
-        if hl_text:
-            lexer.add_filter(AwesomePlaceholders(hl_text=hl_text))
 
-        # highlight via Pygments
-        formatter = self.get_formatter(**kwargs)
-        try:
-            hlsource: str = highlight(source, lexer, formatter)
-        except ErrorToken:
-            # this is most probably not the selected language,
-            # so let it pass unhighlighted
-            if lang == "default":
-                pass  # automatic highlighting failed.
-            else:
-                logger.warning(
-                    __('Could not lex literal_block as "%s". ' "Highlighting skipped."),
-                    lang,
-                    type="misc",
-                    subtype="highlighting_failure",
-                    location=location,
-                )
-            lexer = self.get_lexer(source, "none", opts, force, location)
-            hlsource = highlight(source, lexer, formatter)
+        if hl_text:
+            opts["hl_text"] = hl_text
 
-        if self.dest == "html":
-            return hlsource
-        else:
-            # MEMO: this is done to escape Unicode chars with non-Unicode engines
-            return texescape.hlescape(hlsource, self.latex_engine)
+        return pygmentsbridge_highlight_block(
+            self, source, lang, opts, force, location, **kwargs
+        )
 
 
 def setup(app: Sphinx) -> dict[str, Any]:
     """Set up this internal extension."""
     PygmentsBridge.html_formatter = AwesomeHtmlFormatter
-    PygmentsBridge.highlight_block = AwesomePygmentsBridge.highlight_block  # type: ignore[method-assign]  # noqa
+    PygmentsBridge.get_lexer = AwesomePygmentsBridge.get_lexer  # type: ignore
+    PygmentsBridge.highlight_block = (  # type: ignore
+        AwesomePygmentsBridge.highlight_block  # type: ignore
+    )
     directives.register_directive("code-block", AwesomeCodeBlock)
 
     return {
         "version": __version__,
         "parallel_read_safe": True,
         "parallel_write_safe": True,
     }
```

### Comparing `sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/jinja_functions.py` & `sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/jinja_functions.py`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/jsonimpl.py` & `sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/jsonimpl.py`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/layout.html` & `sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/layout.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/logos.py` & `sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/logos.py`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/page.html` & `sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/page.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/postprocess.py` & `sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/postprocess.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,19 +17,32 @@
 :copyright: Copyright Kai Welke.
 :license: MIT, see LICENSE.
 """
 from __future__ import annotations
 
 import os
 import re
+from dataclasses import dataclass
 
 from bs4 import BeautifulSoup, Comment
 from sphinx.application import Sphinx
 
-from . import icons, logos
+from . import logos
+
+
+@dataclass(frozen=True)
+class Icons:
+    """Icons from Material Design.
+
+    See: https://material.io/resources/icons/
+    """
+
+    external_link: str = '<svg xmlns="http://www.w3.org/2000/svg" height="1em" width="1em" fill="currentColor" stroke="none" viewBox="0 96 960 960"><path d="M188 868q-11-11-11-28t11-28l436-436H400q-17 0-28.5-11.5T360 336q0-17 11.5-28.5T400 296h320q17 0 28.5 11.5T760 336v320q0 17-11.5 28.5T720 696q-17 0-28.5-11.5T680 656V432L244 868q-11 11-28 11t-28-11Z"/></svg>'
+    chevron_right: str = '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="18px" height="18px" stroke="none" fill="currentColor"><path d="M10 6L8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"/></svg>'
+    permalinks_icon: str = '<svg xmlns="http://www.w3.org/2000/svg" height="1em" width="1em" viewBox="0 0 24 24"><path d="M3.9 12c0-1.71 1.39-3.1 3.1-3.1h4V7H7c-2.76 0-5 2.24-5 5s2.24 5 5 5h4v-1.9H7c-1.71 0-3.1-1.39-3.1-3.1zM8 13h8v-2H8v2zm9-6h-4v1.9h4c1.71 0 3.1 1.39 3.1 3.1s-1.39 3.1-3.1 3.1h-4V17h4c2.76 0 5-2.24 5-5s-2.24-5-5-5z"/></svg>'
 
 
 def _get_html_files(outdir: str) -> list[str]:
     """Get a list of HTML files."""
     html_list = []
     for root, _, files in os.walk(outdir):
         html_list.extend(
@@ -61,15 +74,15 @@
                 "button",
                 attrs={"type": "button", "@click.prevent.stop": "expanded = !expanded"},
             )
             label = tree.new_tag("span", attrs={"class": "sr-only"})
             button.append(label)
 
             # create the icon
-            svg = BeautifulSoup(icons.ICONS["chevron_right"], "html.parser").svg
+            svg = BeautifulSoup(Icons.chevron_right, "html.parser").svg
             button.append(svg)
             link.append(button)
 
 
 def _remove_empty_toctree(tree: BeautifulSoup) -> None:
     """Remove empty toctree divs.
 
@@ -115,15 +128,15 @@
 
     The alternative was to copy `visit_reference` in the HTMLTranslator
     and change literally one line.
     """
     for link in tree("a", class_="reference external"):
         link["rel"] = "nofollow noopener"
         # append icon
-        link.append(BeautifulSoup(icons.ICONS["external_link"], "html.parser").svg)
+        link.append(BeautifulSoup(Icons.external_link, "html.parser").svg)
 
 
 def _strip_comments(tree: BeautifulSoup) -> None:
     """Remove HTML comments from documents."""
     comments = tree.find_all(string=lambda text: isinstance(text, Comment))
     for c in comments:
         c.extract()
```

### Comparing `sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/prev_next.html` & `sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/prev_next.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/scrolltop.html` & `sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/scrolltop.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/search.html` & `sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/search.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/searchbox.html` & `sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/searchbox.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/sidebar.html` & `sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/sidebar.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/awesome-sphinx-design.f3507627e0af8330cfa7.css` & `sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/static/awesome-sphinx-design.f3507627e0af8330cfa7.css`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/docsearch.445222223e83896718c6.css` & `sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/static/docsearch.82e38f6cd0ccc11d77d4.css`

 * *Files 0% similar despite different names*

```diff
@@ -1,2 +1,2 @@
-/*! @docsearch/css 3.3.4 | MIT License | © Algolia, Inc. and contributors | https://docsearch.algolia.com */:root{--docsearch-primary-color:#5468ff;--docsearch-text-color:#1c1e21;--docsearch-spacing:12px;--docsearch-icon-stroke-width:1.4;--docsearch-highlight-color:var(--docsearch-primary-color);--docsearch-muted-color:#969faf;--docsearch-container-background:rgba(101,108,133,.8);--docsearch-logo-color:#5468ff;--docsearch-modal-width:560px;--docsearch-modal-height:600px;--docsearch-modal-background:#f5f6f7;--docsearch-modal-shadow:inset 1px 1px 0 0 hsla(0,0%,100%,.5),0 3px 8px 0 #555a64;--docsearch-searchbox-height:56px;--docsearch-searchbox-background:#ebedf0;--docsearch-searchbox-focus-background:#fff;--docsearch-searchbox-shadow:inset 0 0 0 2px var(--docsearch-primary-color);--docsearch-hit-height:56px;--docsearch-hit-color:#444950;--docsearch-hit-active-color:#fff;--docsearch-hit-background:#fff;--docsearch-hit-shadow:0 1px 3px 0 #d4d9e1;--docsearch-key-gradient:linear-gradient(-225deg,#d5dbe4,#f8f8f8);--docsearch-key-shadow:inset 0 -2px 0 0 #cdcde6,inset 0 0 1px 1px #fff,0 1px 2px 1px rgba(30,35,90,.4);--docsearch-footer-height:44px;--docsearch-footer-background:#fff;--docsearch-footer-shadow:0 -1px 0 0 #e0e3e8,0 -3px 6px 0 rgba(69,98,155,.12)}html[data-theme=dark]{--docsearch-text-color:#f5f6f7;--docsearch-container-background:rgba(9,10,17,.8);--docsearch-modal-background:#15172a;--docsearch-modal-shadow:inset 1px 1px 0 0 #2c2e40,0 3px 8px 0 #000309;--docsearch-searchbox-background:#090a11;--docsearch-searchbox-focus-background:#000;--docsearch-hit-color:#bec3c9;--docsearch-hit-shadow:none;--docsearch-hit-background:#090a11;--docsearch-key-gradient:linear-gradient(-26.5deg,#565872,#31355b);--docsearch-key-shadow:inset 0 -2px 0 0 #282d55,inset 0 0 1px 1px #51577d,0 2px 2px 0 rgba(3,4,9,.3);--docsearch-footer-background:#1e2136;--docsearch-footer-shadow:inset 0 1px 0 0 rgba(73,76,106,.5),0 -4px 8px 0 rgba(0,0,0,.2);--docsearch-logo-color:#fff;--docsearch-muted-color:#7f8497}.DocSearch-Button{align-items:center;background:#ebedf0;background:var(--docsearch-searchbox-background);border:0;border-radius:40px;color:#969faf;color:var(--docsearch-muted-color);cursor:pointer;display:flex;font-weight:500;height:36px;justify-content:space-between;margin:0 0 0 16px;padding:0 8px;-webkit-user-select:none;-moz-user-select:none;user-select:none}.DocSearch-Button:active,.DocSearch-Button:focus,.DocSearch-Button:hover{background:#fff;background:var(--docsearch-searchbox-focus-background);box-shadow:inset 0 0 0 2px #5468ff;box-shadow:var(--docsearch-searchbox-shadow);color:#1c1e21;color:var(--docsearch-text-color);outline:none}.DocSearch-Button-Container{align-items:center;display:flex}.DocSearch-Search-Icon{stroke-width:1.6}.DocSearch-Button .DocSearch-Search-Icon{color:#1c1e21;color:var(--docsearch-text-color)}.DocSearch-Button-Placeholder{font-size:1rem;padding:0 12px 0 6px}.DocSearch-Button-Keys{display:flex;min-width:calc(40px + .8em)}.DocSearch-Button-Key{align-items:center;background:linear-gradient(-225deg,#d5dbe4,#f8f8f8);background:var(--docsearch-key-gradient);border:0;border-radius:3px;box-shadow:inset 0 -2px 0 0 #cdcde6,inset 0 0 1px 1px #fff,0 1px 2px 1px rgba(30,35,90,.4);box-shadow:var(--docsearch-key-shadow);color:#969faf;color:var(--docsearch-muted-color);display:flex;height:18px;justify-content:center;margin-right:.4em;padding:0 0 2px;position:relative;top:-1px;width:20px}@media (max-width:768px){.DocSearch-Button-Keys,.DocSearch-Button-Placeholder{display:none}}.DocSearch--active{overflow:hidden!important}.DocSearch-Container,.DocSearch-Container *{box-sizing:border-box}.DocSearch-Container{background-color:rgba(101,108,133,.8);background-color:var(--docsearch-container-background);height:100vh;left:0;position:fixed;top:0;width:100vw;z-index:200}.DocSearch-Container a{-webkit-text-decoration:none;text-decoration:none}.DocSearch-Link{-webkit-appearance:none;-moz-appearance:none;appearance:none;background:none;border:0;color:#5468ff;color:var(--docsearch-highlight-color);cursor:pointer;font:inherit;margin:0;padding:0}.DocSearch-Modal{background:#f5f6f7;background:var(--docsearch-modal-background);border-radius:6px;box-shadow:inset 1px 1px 0 0 hsla(0,0%,100%,.5),0 3px 8px 0 #555a64;box-shadow:var(--docsearch-modal-shadow);flex-direction:column;margin:60px auto auto;max-width:560px;max-width:var(--docsearch-modal-width);position:relative}.DocSearch-SearchBar{display:flex;padding:12px 12px 0;padding:var(--docsearch-spacing) var(--docsearch-spacing) 0}.DocSearch-Form{align-items:center;background:#fff;background:var(--docsearch-searchbox-focus-background);border-radius:4px;box-shadow:inset 0 0 0 2px #5468ff;box-shadow:var(--docsearch-searchbox-shadow);display:flex;height:56px;height:var(--docsearch-searchbox-height);margin:0;padding:0 12px;padding:0 var(--docsearch-spacing);position:relative;width:100%}.DocSearch-Input{-webkit-appearance:none;-moz-appearance:none;appearance:none;background:transparent;border:0;color:#1c1e21;color:var(--docsearch-text-color);flex:1;font:inherit;font-size:1.2em;height:100%;outline:none;padding:0 0 0 8px;width:80%}.DocSearch-Input::-moz-placeholder{color:#969faf;color:var(--docsearch-muted-color);opacity:1}.DocSearch-Input::placeholder{color:#969faf;color:var(--docsearch-muted-color);opacity:1}.DocSearch-Input::-webkit-search-cancel-button,.DocSearch-Input::-webkit-search-decoration,.DocSearch-Input::-webkit-search-results-button,.DocSearch-Input::-webkit-search-results-decoration{display:none}.DocSearch-LoadingIndicator,.DocSearch-MagnifierLabel,.DocSearch-Reset{margin:0;padding:0}.DocSearch-MagnifierLabel,.DocSearch-Reset{align-items:center;color:#5468ff;color:var(--docsearch-highlight-color);display:flex;justify-content:center}.DocSearch-Container--Stalled .DocSearch-MagnifierLabel,.DocSearch-LoadingIndicator{display:none}.DocSearch-Container--Stalled .DocSearch-LoadingIndicator{align-items:center;color:#5468ff;color:var(--docsearch-highlight-color);display:flex;justify-content:center}@media screen and (prefers-reduced-motion:reduce){.DocSearch-Reset{stroke-width:1.4;stroke-width:var(--docsearch-icon-stroke-width);animation:none;-webkit-appearance:none;-moz-appearance:none;appearance:none;background:none;border:0;border-radius:50%;color:var(--docsearch-icon-color);cursor:pointer;right:0}}.DocSearch-Reset{stroke-width:1.4;stroke-width:var(--docsearch-icon-stroke-width);animation:fade-in .1s ease-in forwards;-webkit-appearance:none;-moz-appearance:none;appearance:none;background:none;border:0;border-radius:50%;color:var(--docsearch-icon-color);cursor:pointer;padding:2px;right:0}.DocSearch-Reset[hidden]{display:none}.DocSearch-Reset:hover{color:#5468ff;color:var(--docsearch-highlight-color)}.DocSearch-LoadingIndicator svg,.DocSearch-MagnifierLabel svg{height:24px;width:24px}.DocSearch-Cancel{display:none}.DocSearch-Dropdown{max-height:488px;max-height:calc(var(--docsearch-modal-height) - var(--docsearch-searchbox-height) - var(--docsearch-spacing) - var(--docsearch-footer-height));min-height:12px;min-height:var(--docsearch-spacing);overflow-y:auto;overflow-y:overlay;padding:0 12px;padding:0 var(--docsearch-spacing);scrollbar-color:#969faf #f5f6f7;scrollbar-color:var(--docsearch-muted-color) var(--docsearch-modal-background);scrollbar-width:thin}.DocSearch-Dropdown::-webkit-scrollbar{width:12px}.DocSearch-Dropdown::-webkit-scrollbar-track{background:transparent}.DocSearch-Dropdown::-webkit-scrollbar-thumb{background-color:#969faf;background-color:var(--docsearch-muted-color);border:3px solid #f5f6f7;border:3px solid var(--docsearch-modal-background);border-radius:20px}.DocSearch-Dropdown ul{list-style:none;margin:0;padding:0}.DocSearch-Label{font-size:.75em;line-height:1.6em}.DocSearch-Help,.DocSearch-Label{color:#969faf;color:var(--docsearch-muted-color)}.DocSearch-Help{font-size:.9em;margin:0;-webkit-user-select:none;-moz-user-select:none;user-select:none}.DocSearch-Title{font-size:1.2em}.DocSearch-Logo a{display:flex}.DocSearch-Logo svg{color:#5468ff;color:var(--docsearch-logo-color);margin-left:8px}.DocSearch-Hits:last-of-type{margin-bottom:24px}.DocSearch-Hits mark{background:none;color:#5468ff;color:var(--docsearch-highlight-color)}.DocSearch-HitsFooter{color:#969faf;color:var(--docsearch-muted-color);display:flex;font-size:.85em;justify-content:center;margin-bottom:12px;margin-bottom:var(--docsearch-spacing);padding:12px;padding:var(--docsearch-spacing)}.DocSearch-HitsFooter a{border-bottom:1px solid;color:inherit}.DocSearch-Hit{border-radius:4px;display:flex;padding-bottom:4px;position:relative}@media screen and (prefers-reduced-motion:reduce){.DocSearch-Hit--deleting{transition:none}}.DocSearch-Hit--deleting{opacity:0;transition:all .25s linear}@media screen and (prefers-reduced-motion:reduce){.DocSearch-Hit--favoriting{transition:none}}.DocSearch-Hit--favoriting{transform:scale(0);transform-origin:top center;transition:all .25s linear;transition-delay:.25s}.DocSearch-Hit a{background:#fff;background:var(--docsearch-hit-background);border-radius:4px;box-shadow:0 1px 3px 0 #d4d9e1;box-shadow:var(--docsearch-hit-shadow);display:block;padding-left:12px;padding-left:var(--docsearch-spacing);width:100%}.DocSearch-Hit-source{background:#f5f6f7;background:var(--docsearch-modal-background);color:#5468ff;color:var(--docsearch-highlight-color);font-size:.85em;font-weight:600;line-height:32px;margin:0 -4px;padding:8px 4px 0;position:sticky;top:0;z-index:10}.DocSearch-Hit-Tree{stroke-width:1.4;stroke-width:var(--docsearch-icon-stroke-width);color:#969faf;color:var(--docsearch-muted-color);height:56px;height:var(--docsearch-hit-height);opacity:.5;width:24px}.DocSearch-Hit[aria-selected=true] a{background-color:#5468ff;background-color:var(--docsearch-highlight-color)}.DocSearch-Hit[aria-selected=true] mark{-webkit-text-decoration:underline;text-decoration:underline}.DocSearch-Hit-Container{align-items:center;color:#444950;color:var(--docsearch-hit-color);display:flex;flex-direction:row;height:56px;height:var(--docsearch-hit-height);padding:0 12px 0 0;padding:0 var(--docsearch-spacing) 0 0}.DocSearch-Hit-icon{height:20px;width:20px}.DocSearch-Hit-action,.DocSearch-Hit-icon{stroke-width:1.4;stroke-width:var(--docsearch-icon-stroke-width);color:#969faf;color:var(--docsearch-muted-color)}.DocSearch-Hit-action{align-items:center;display:flex;height:22px;width:22px}.DocSearch-Hit-action svg{display:block;height:18px;width:18px}.DocSearch-Hit-action+.DocSearch-Hit-action{margin-left:6px}.DocSearch-Hit-action-button{-webkit-appearance:none;-moz-appearance:none;appearance:none;background:none;border:0;border-radius:50%;color:inherit;cursor:pointer;padding:2px}svg.DocSearch-Hit-Select-Icon{display:none}.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-Select-Icon{display:block}.DocSearch-Hit-action-button:focus,.DocSearch-Hit-action-button:hover{background:rgba(0,0,0,.2);transition:background-color .1s ease-in}@media screen and (prefers-reduced-motion:reduce){.DocSearch-Hit-action-button:focus,.DocSearch-Hit-action-button:hover{transition:none}}.DocSearch-Hit-action-button:focus path,.DocSearch-Hit-action-button:hover path{fill:#fff}.DocSearch-Hit-content-wrapper{display:flex;flex:1 1 auto;flex-direction:column;font-weight:500;justify-content:center;line-height:1.2em;margin:0 8px;overflow-x:hidden;position:relative;text-overflow:ellipsis;white-space:nowrap;width:80%}.DocSearch-Hit-title{font-size:.9em}.DocSearch-Hit-path{color:#969faf;color:var(--docsearch-muted-color);font-size:.75em}.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-Tree,.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-action,.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-icon,.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-path,.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-text,.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-title,.DocSearch-Hit[aria-selected=true] mark{color:#fff!important;color:var(--docsearch-hit-active-color)!important}@media screen and (prefers-reduced-motion:reduce){.DocSearch-Hit-action-button:focus,.DocSearch-Hit-action-button:hover{background:rgba(0,0,0,.2);transition:none}}.DocSearch-ErrorScreen,.DocSearch-NoResults,.DocSearch-StartScreen{font-size:.9em;margin:0 auto;padding:36px 0;text-align:center;width:80%}.DocSearch-Screen-Icon{color:#969faf;color:var(--docsearch-muted-color);padding-bottom:12px}.DocSearch-NoResults-Prefill-List{display:inline-block;padding-bottom:24px;text-align:left}.DocSearch-NoResults-Prefill-List ul{display:inline-block;padding:8px 0 0}.DocSearch-NoResults-Prefill-List li{list-style-position:inside;list-style-type:"» "}.DocSearch-Prefill{-webkit-appearance:none;-moz-appearance:none;appearance:none;background:none;border:0;border-radius:1em;color:#5468ff;color:var(--docsearch-highlight-color);cursor:pointer;display:inline-block;font-size:1em;font-weight:700;padding:0}.DocSearch-Prefill:focus,.DocSearch-Prefill:hover{outline:none;-webkit-text-decoration:underline;text-decoration:underline}.DocSearch-Footer{align-items:center;background:#fff;background:var(--docsearch-footer-background);border-radius:0 0 8px 8px;box-shadow:0 -1px 0 0 #e0e3e8,0 -3px 6px 0 rgba(69,98,155,.12);box-shadow:var(--docsearch-footer-shadow);display:flex;flex-direction:row-reverse;flex-shrink:0;height:44px;height:var(--docsearch-footer-height);justify-content:space-between;padding:0 12px;padding:0 var(--docsearch-spacing);position:relative;-webkit-user-select:none;-moz-user-select:none;user-select:none;width:100%;z-index:300}.DocSearch-Commands{color:#969faf;color:var(--docsearch-muted-color);display:flex;list-style:none;margin:0;padding:0}.DocSearch-Commands li{align-items:center;display:flex}.DocSearch-Commands li:not(:last-of-type){margin-right:.8em}.DocSearch-Commands-Key{align-items:center;background:linear-gradient(-225deg,#d5dbe4,#f8f8f8);background:var(--docsearch-key-gradient);border:0;border-radius:2px;box-shadow:inset 0 -2px 0 0 #cdcde6,inset 0 0 1px 1px #fff,0 1px 2px 1px rgba(30,35,90,.4);box-shadow:var(--docsearch-key-shadow);color:#969faf;color:var(--docsearch-muted-color);display:flex;height:18px;justify-content:center;margin-right:.4em;padding:0 0 1px;width:20px}@media (max-width:768px){:root{--docsearch-spacing:10px;--docsearch-footer-height:40px}.DocSearch-Dropdown{height:100%}.DocSearch-Container{height:-webkit-fill-available;height:100vh;height:calc(var(--docsearch-vh, 1vh)*100);position:absolute}.DocSearch-Footer{border-radius:0;bottom:0;position:absolute}.DocSearch-Hit-content-wrapper{display:flex;position:relative;width:80%}.DocSearch-Modal{border-radius:0;box-shadow:none;height:-webkit-fill-available;height:100vh;height:calc(var(--docsearch-vh, 1vh)*100);margin:0;max-width:100%;width:100%}.DocSearch-Dropdown{max-height:calc(100vh - 112px);max-height:calc(var(--docsearch-vh, 1vh)*100 - var(--docsearch-searchbox-height) - var(--docsearch-spacing) - var(--docsearch-footer-height))}.DocSearch-Cancel{-webkit-appearance:none;-moz-appearance:none;appearance:none;background:none;border:0;color:#5468ff;color:var(--docsearch-highlight-color);cursor:pointer;display:inline-block;flex:none;font:inherit;font-size:1em;font-weight:500;margin-left:12px;margin-left:var(--docsearch-spacing);outline:none;overflow:hidden;padding:0;-webkit-user-select:none;-moz-user-select:none;user-select:none;white-space:nowrap}.DocSearch-Commands,.DocSearch-Hit-Tree{display:none}}@keyframes fade-in{0%{opacity:0}to{opacity:1}}
+/*! @docsearch/css 3.3.5 | MIT License | © Algolia, Inc. and contributors | https://docsearch.algolia.com */:root{--docsearch-primary-color:#5468ff;--docsearch-text-color:#1c1e21;--docsearch-spacing:12px;--docsearch-icon-stroke-width:1.4;--docsearch-highlight-color:var(--docsearch-primary-color);--docsearch-muted-color:#969faf;--docsearch-container-background:rgba(101,108,133,.8);--docsearch-logo-color:#5468ff;--docsearch-modal-width:560px;--docsearch-modal-height:600px;--docsearch-modal-background:#f5f6f7;--docsearch-modal-shadow:inset 1px 1px 0 0 hsla(0,0%,100%,.5),0 3px 8px 0 #555a64;--docsearch-searchbox-height:56px;--docsearch-searchbox-background:#ebedf0;--docsearch-searchbox-focus-background:#fff;--docsearch-searchbox-shadow:inset 0 0 0 2px var(--docsearch-primary-color);--docsearch-hit-height:56px;--docsearch-hit-color:#444950;--docsearch-hit-active-color:#fff;--docsearch-hit-background:#fff;--docsearch-hit-shadow:0 1px 3px 0 #d4d9e1;--docsearch-key-gradient:linear-gradient(-225deg,#d5dbe4,#f8f8f8);--docsearch-key-shadow:inset 0 -2px 0 0 #cdcde6,inset 0 0 1px 1px #fff,0 1px 2px 1px rgba(30,35,90,.4);--docsearch-footer-height:44px;--docsearch-footer-background:#fff;--docsearch-footer-shadow:0 -1px 0 0 #e0e3e8,0 -3px 6px 0 rgba(69,98,155,.12)}html[data-theme=dark]{--docsearch-text-color:#f5f6f7;--docsearch-container-background:rgba(9,10,17,.8);--docsearch-modal-background:#15172a;--docsearch-modal-shadow:inset 1px 1px 0 0 #2c2e40,0 3px 8px 0 #000309;--docsearch-searchbox-background:#090a11;--docsearch-searchbox-focus-background:#000;--docsearch-hit-color:#bec3c9;--docsearch-hit-shadow:none;--docsearch-hit-background:#090a11;--docsearch-key-gradient:linear-gradient(-26.5deg,#565872,#31355b);--docsearch-key-shadow:inset 0 -2px 0 0 #282d55,inset 0 0 1px 1px #51577d,0 2px 2px 0 rgba(3,4,9,.3);--docsearch-footer-background:#1e2136;--docsearch-footer-shadow:inset 0 1px 0 0 rgba(73,76,106,.5),0 -4px 8px 0 rgba(0,0,0,.2);--docsearch-logo-color:#fff;--docsearch-muted-color:#7f8497}.DocSearch-Button{align-items:center;background:#ebedf0;background:var(--docsearch-searchbox-background);border:0;border-radius:40px;color:#969faf;color:var(--docsearch-muted-color);cursor:pointer;display:flex;font-weight:500;height:36px;justify-content:space-between;margin:0 0 0 16px;padding:0 8px;-webkit-user-select:none;-moz-user-select:none;user-select:none}.DocSearch-Button:active,.DocSearch-Button:focus,.DocSearch-Button:hover{background:#fff;background:var(--docsearch-searchbox-focus-background);box-shadow:inset 0 0 0 2px #5468ff;box-shadow:var(--docsearch-searchbox-shadow);color:#1c1e21;color:var(--docsearch-text-color);outline:none}.DocSearch-Button-Container{align-items:center;display:flex}.DocSearch-Search-Icon{stroke-width:1.6}.DocSearch-Button .DocSearch-Search-Icon{color:#1c1e21;color:var(--docsearch-text-color)}.DocSearch-Button-Placeholder{font-size:1rem;padding:0 12px 0 6px}.DocSearch-Button-Keys{display:flex;min-width:calc(40px + .8em)}.DocSearch-Button-Key{align-items:center;background:linear-gradient(-225deg,#d5dbe4,#f8f8f8);background:var(--docsearch-key-gradient);border:0;border-radius:3px;box-shadow:inset 0 -2px 0 0 #cdcde6,inset 0 0 1px 1px #fff,0 1px 2px 1px rgba(30,35,90,.4);box-shadow:var(--docsearch-key-shadow);color:#969faf;color:var(--docsearch-muted-color);display:flex;height:18px;justify-content:center;margin-right:.4em;padding:0 0 2px;position:relative;top:-1px;width:20px}@media (max-width:768px){.DocSearch-Button-Keys,.DocSearch-Button-Placeholder{display:none}}.DocSearch--active{overflow:hidden!important}.DocSearch-Container,.DocSearch-Container *{box-sizing:border-box}.DocSearch-Container{background-color:rgba(101,108,133,.8);background-color:var(--docsearch-container-background);height:100vh;left:0;position:fixed;top:0;width:100vw;z-index:200}.DocSearch-Container a{-webkit-text-decoration:none;text-decoration:none}.DocSearch-Link{-webkit-appearance:none;-moz-appearance:none;appearance:none;background:none;border:0;color:#5468ff;color:var(--docsearch-highlight-color);cursor:pointer;font:inherit;margin:0;padding:0}.DocSearch-Modal{background:#f5f6f7;background:var(--docsearch-modal-background);border-radius:6px;box-shadow:inset 1px 1px 0 0 hsla(0,0%,100%,.5),0 3px 8px 0 #555a64;box-shadow:var(--docsearch-modal-shadow);flex-direction:column;margin:60px auto auto;max-width:560px;max-width:var(--docsearch-modal-width);position:relative}.DocSearch-SearchBar{display:flex;padding:12px 12px 0;padding:var(--docsearch-spacing) var(--docsearch-spacing) 0}.DocSearch-Form{align-items:center;background:#fff;background:var(--docsearch-searchbox-focus-background);border-radius:4px;box-shadow:inset 0 0 0 2px #5468ff;box-shadow:var(--docsearch-searchbox-shadow);display:flex;height:56px;height:var(--docsearch-searchbox-height);margin:0;padding:0 12px;padding:0 var(--docsearch-spacing);position:relative;width:100%}.DocSearch-Input{-webkit-appearance:none;-moz-appearance:none;appearance:none;background:transparent;border:0;color:#1c1e21;color:var(--docsearch-text-color);flex:1;font:inherit;font-size:1.2em;height:100%;outline:none;padding:0 0 0 8px;width:80%}.DocSearch-Input::-moz-placeholder{color:#969faf;color:var(--docsearch-muted-color);opacity:1}.DocSearch-Input::placeholder{color:#969faf;color:var(--docsearch-muted-color);opacity:1}.DocSearch-Input::-webkit-search-cancel-button,.DocSearch-Input::-webkit-search-decoration,.DocSearch-Input::-webkit-search-results-button,.DocSearch-Input::-webkit-search-results-decoration{display:none}.DocSearch-LoadingIndicator,.DocSearch-MagnifierLabel,.DocSearch-Reset{margin:0;padding:0}.DocSearch-MagnifierLabel,.DocSearch-Reset{align-items:center;color:#5468ff;color:var(--docsearch-highlight-color);display:flex;justify-content:center}.DocSearch-Container--Stalled .DocSearch-MagnifierLabel,.DocSearch-LoadingIndicator{display:none}.DocSearch-Container--Stalled .DocSearch-LoadingIndicator{align-items:center;color:#5468ff;color:var(--docsearch-highlight-color);display:flex;justify-content:center}@media screen and (prefers-reduced-motion:reduce){.DocSearch-Reset{stroke-width:1.4;stroke-width:var(--docsearch-icon-stroke-width);animation:none;-webkit-appearance:none;-moz-appearance:none;appearance:none;background:none;border:0;border-radius:50%;color:var(--docsearch-icon-color);cursor:pointer;right:0}}.DocSearch-Reset{stroke-width:1.4;stroke-width:var(--docsearch-icon-stroke-width);animation:fade-in .1s ease-in forwards;-webkit-appearance:none;-moz-appearance:none;appearance:none;background:none;border:0;border-radius:50%;color:var(--docsearch-icon-color);cursor:pointer;padding:2px;right:0}.DocSearch-Reset[hidden]{display:none}.DocSearch-Reset:hover{color:#5468ff;color:var(--docsearch-highlight-color)}.DocSearch-LoadingIndicator svg,.DocSearch-MagnifierLabel svg{height:24px;width:24px}.DocSearch-Cancel{display:none}.DocSearch-Dropdown{max-height:488px;max-height:calc(var(--docsearch-modal-height) - var(--docsearch-searchbox-height) - var(--docsearch-spacing) - var(--docsearch-footer-height));min-height:12px;min-height:var(--docsearch-spacing);overflow-y:auto;overflow-y:overlay;padding:0 12px;padding:0 var(--docsearch-spacing);scrollbar-color:#969faf #f5f6f7;scrollbar-color:var(--docsearch-muted-color) var(--docsearch-modal-background);scrollbar-width:thin}.DocSearch-Dropdown::-webkit-scrollbar{width:12px}.DocSearch-Dropdown::-webkit-scrollbar-track{background:transparent}.DocSearch-Dropdown::-webkit-scrollbar-thumb{background-color:#969faf;background-color:var(--docsearch-muted-color);border:3px solid #f5f6f7;border:3px solid var(--docsearch-modal-background);border-radius:20px}.DocSearch-Dropdown ul{list-style:none;margin:0;padding:0}.DocSearch-Label{font-size:.75em;line-height:1.6em}.DocSearch-Help,.DocSearch-Label{color:#969faf;color:var(--docsearch-muted-color)}.DocSearch-Help{font-size:.9em;margin:0;-webkit-user-select:none;-moz-user-select:none;user-select:none}.DocSearch-Title{font-size:1.2em}.DocSearch-Logo a{display:flex}.DocSearch-Logo svg{color:#5468ff;color:var(--docsearch-logo-color);margin-left:8px}.DocSearch-Hits:last-of-type{margin-bottom:24px}.DocSearch-Hits mark{background:none;color:#5468ff;color:var(--docsearch-highlight-color)}.DocSearch-HitsFooter{color:#969faf;color:var(--docsearch-muted-color);display:flex;font-size:.85em;justify-content:center;margin-bottom:12px;margin-bottom:var(--docsearch-spacing);padding:12px;padding:var(--docsearch-spacing)}.DocSearch-HitsFooter a{border-bottom:1px solid;color:inherit}.DocSearch-Hit{border-radius:4px;display:flex;padding-bottom:4px;position:relative}@media screen and (prefers-reduced-motion:reduce){.DocSearch-Hit--deleting{transition:none}}.DocSearch-Hit--deleting{opacity:0;transition:all .25s linear}@media screen and (prefers-reduced-motion:reduce){.DocSearch-Hit--favoriting{transition:none}}.DocSearch-Hit--favoriting{transform:scale(0);transform-origin:top center;transition:all .25s linear;transition-delay:.25s}.DocSearch-Hit a{background:#fff;background:var(--docsearch-hit-background);border-radius:4px;box-shadow:0 1px 3px 0 #d4d9e1;box-shadow:var(--docsearch-hit-shadow);display:block;padding-left:12px;padding-left:var(--docsearch-spacing);width:100%}.DocSearch-Hit-source{background:#f5f6f7;background:var(--docsearch-modal-background);color:#5468ff;color:var(--docsearch-highlight-color);font-size:.85em;font-weight:600;line-height:32px;margin:0 -4px;padding:8px 4px 0;position:sticky;top:0;z-index:10}.DocSearch-Hit-Tree{stroke-width:1.4;stroke-width:var(--docsearch-icon-stroke-width);color:#969faf;color:var(--docsearch-muted-color);height:56px;height:var(--docsearch-hit-height);opacity:.5;width:24px}.DocSearch-Hit[aria-selected=true] a{background-color:#5468ff;background-color:var(--docsearch-highlight-color)}.DocSearch-Hit[aria-selected=true] mark{-webkit-text-decoration:underline;text-decoration:underline}.DocSearch-Hit-Container{align-items:center;color:#444950;color:var(--docsearch-hit-color);display:flex;flex-direction:row;height:56px;height:var(--docsearch-hit-height);padding:0 12px 0 0;padding:0 var(--docsearch-spacing) 0 0}.DocSearch-Hit-icon{height:20px;width:20px}.DocSearch-Hit-action,.DocSearch-Hit-icon{stroke-width:1.4;stroke-width:var(--docsearch-icon-stroke-width);color:#969faf;color:var(--docsearch-muted-color)}.DocSearch-Hit-action{align-items:center;display:flex;height:22px;width:22px}.DocSearch-Hit-action svg{display:block;height:18px;width:18px}.DocSearch-Hit-action+.DocSearch-Hit-action{margin-left:6px}.DocSearch-Hit-action-button{-webkit-appearance:none;-moz-appearance:none;appearance:none;background:none;border:0;border-radius:50%;color:inherit;cursor:pointer;padding:2px}svg.DocSearch-Hit-Select-Icon{display:none}.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-Select-Icon{display:block}.DocSearch-Hit-action-button:focus,.DocSearch-Hit-action-button:hover{background:rgba(0,0,0,.2);transition:background-color .1s ease-in}@media screen and (prefers-reduced-motion:reduce){.DocSearch-Hit-action-button:focus,.DocSearch-Hit-action-button:hover{transition:none}}.DocSearch-Hit-action-button:focus path,.DocSearch-Hit-action-button:hover path{fill:#fff}.DocSearch-Hit-content-wrapper{display:flex;flex:1 1 auto;flex-direction:column;font-weight:500;justify-content:center;line-height:1.2em;margin:0 8px;overflow-x:hidden;position:relative;text-overflow:ellipsis;white-space:nowrap;width:80%}.DocSearch-Hit-title{font-size:.9em}.DocSearch-Hit-path{color:#969faf;color:var(--docsearch-muted-color);font-size:.75em}.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-Tree,.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-action,.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-icon,.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-path,.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-text,.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-title,.DocSearch-Hit[aria-selected=true] mark{color:#fff!important;color:var(--docsearch-hit-active-color)!important}@media screen and (prefers-reduced-motion:reduce){.DocSearch-Hit-action-button:focus,.DocSearch-Hit-action-button:hover{background:rgba(0,0,0,.2);transition:none}}.DocSearch-ErrorScreen,.DocSearch-NoResults,.DocSearch-StartScreen{font-size:.9em;margin:0 auto;padding:36px 0;text-align:center;width:80%}.DocSearch-Screen-Icon{color:#969faf;color:var(--docsearch-muted-color);padding-bottom:12px}.DocSearch-NoResults-Prefill-List{display:inline-block;padding-bottom:24px;text-align:left}.DocSearch-NoResults-Prefill-List ul{display:inline-block;padding:8px 0 0}.DocSearch-NoResults-Prefill-List li{list-style-position:inside;list-style-type:"» "}.DocSearch-Prefill{-webkit-appearance:none;-moz-appearance:none;appearance:none;background:none;border:0;border-radius:1em;color:#5468ff;color:var(--docsearch-highlight-color);cursor:pointer;display:inline-block;font-size:1em;font-weight:700;padding:0}.DocSearch-Prefill:focus,.DocSearch-Prefill:hover{outline:none;-webkit-text-decoration:underline;text-decoration:underline}.DocSearch-Footer{align-items:center;background:#fff;background:var(--docsearch-footer-background);border-radius:0 0 8px 8px;box-shadow:0 -1px 0 0 #e0e3e8,0 -3px 6px 0 rgba(69,98,155,.12);box-shadow:var(--docsearch-footer-shadow);display:flex;flex-direction:row-reverse;flex-shrink:0;height:44px;height:var(--docsearch-footer-height);justify-content:space-between;padding:0 12px;padding:0 var(--docsearch-spacing);position:relative;-webkit-user-select:none;-moz-user-select:none;user-select:none;width:100%;z-index:300}.DocSearch-Commands{color:#969faf;color:var(--docsearch-muted-color);display:flex;list-style:none;margin:0;padding:0}.DocSearch-Commands li{align-items:center;display:flex}.DocSearch-Commands li:not(:last-of-type){margin-right:.8em}.DocSearch-Commands-Key{align-items:center;background:linear-gradient(-225deg,#d5dbe4,#f8f8f8);background:var(--docsearch-key-gradient);border:0;border-radius:2px;box-shadow:inset 0 -2px 0 0 #cdcde6,inset 0 0 1px 1px #fff,0 1px 2px 1px rgba(30,35,90,.4);box-shadow:var(--docsearch-key-shadow);color:#969faf;color:var(--docsearch-muted-color);display:flex;height:18px;justify-content:center;margin-right:.4em;padding:0 0 1px;width:20px}@media (max-width:768px){:root{--docsearch-spacing:10px;--docsearch-footer-height:40px}.DocSearch-Dropdown{height:100%}.DocSearch-Container{height:-webkit-fill-available;height:100vh;height:calc(var(--docsearch-vh, 1vh)*100);position:absolute}.DocSearch-Footer{border-radius:0;bottom:0;position:absolute}.DocSearch-Hit-content-wrapper{display:flex;position:relative;width:80%}.DocSearch-Modal{border-radius:0;box-shadow:none;height:-webkit-fill-available;height:100vh;height:calc(var(--docsearch-vh, 1vh)*100);margin:0;max-width:100%;width:100%}.DocSearch-Dropdown{max-height:calc(100vh - 112px);max-height:calc(var(--docsearch-vh, 1vh)*100 - var(--docsearch-searchbox-height) - var(--docsearch-spacing) - var(--docsearch-footer-height))}.DocSearch-Cancel{-webkit-appearance:none;-moz-appearance:none;appearance:none;background:none;border:0;color:#5468ff;color:var(--docsearch-highlight-color);cursor:pointer;display:inline-block;flex:none;font:inherit;font-size:1em;font-weight:500;margin-left:12px;margin-left:var(--docsearch-spacing);outline:none;overflow:hidden;padding:0;-webkit-user-select:none;-moz-user-select:none;user-select:none;white-space:nowrap}.DocSearch-Commands,.DocSearch-Hit-Tree{display:none}}@keyframes fade-in{0%{opacity:0}to{opacity:1}}
 :root{--docsearch-primary-color:hsl(var(--primary));--docsearch-key-gradient:transparent;--docsearch-key-shadow:transparent;--docsearch-text-color:hsl(var(--popover-foreground));--docsearch-modal-width:760px;--docsearch-modal-background:hsl(var(--popover));--docsearch-footer-background:hsl(var(--popover));--docsearch-searchbox-focus-background:hsl(var(--popover));--docsearch-container-background:hsl(var(--background)/0.8);--docsearch-spacing:0.5rem;--docsearch-hit-active-color:hsl(var(--accent-foreground));--docsearch-hit-background:transparent;--docsearch-searchbox-shadow:none;--docsearch-hit-shadow:none;--docsearch-modal-shadow:none;--docsearch-footer-shadow:none}.DocSearch-Button{--tw-ring-offset-color:hsl(var(--background));border-color:hsl(var(--input));border-radius:.5em;border-style:solid;border-width:1px;display:flex;font-size:.875rem;line-height:1.25rem;transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1);width:90%}.DocSearch-Button:hover{--tw-shadow:0 0 transparent;--tw-shadow-colored:0 0 transparent;box-shadow:0 0 transparent,0 0 transparent,0 0 transparent;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow)}.DocSearch-Button:focus,.DocSearch-Button:hover{background-color:hsl(var(--accent));color:hsl(var(--accent-foreground))}.DocSearch-Button:focus-visible{--tw-ring-offset-shadow:var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow:var(--tw-ring-inset) 0 0 0 calc(2px + var(--tw-ring-offset-width)) var(--tw-ring-color);--tw-ring-color:hsl(var(--ring));--tw-ring-offset-width:2px;box-shadow:var(--tw-ring-inset) 0 0 0 2px var(--tw-ring-offset-color),var(--tw-ring-inset) 0 0 0 4px hsl(var(--ring)),0 0 transparent;box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow,0 0 #0000);outline:2px solid transparent;outline-offset:2px}.DocSearch-Button-Placeholder{display:block;font-size:.875rem;font-weight:500;line-height:1.25rem}.DocSearch-Button-Key{background-color:hsl(var(--muted));border-color:hsl(var(--border));border-radius:.25rem;border-style:solid;border-width:1px;color:hsl(var(--muted-foreground));font-size:12px}.DocSearch-Container{--tw-backdrop-blur:blur(4px);-webkit-backdrop-filter:blur(4px) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:blur(4px) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);-webkit-backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);position:fixed}.DocSearch-Modal{border-color:hsl(var(--border));border-radius:var(--radius);border-width:1px}.DocSearch-SearchBar{border-bottom-left-radius:0;border-bottom-right-radius:0;border-bottom-width:1px;border-color:hsl(var(--input));border-top-left-radius:var(--radius);border-top-right-radius:var(--radius);padding:0}.DocSearch-Form{border-bottom-left-radius:0;border-bottom-right-radius:0;border-top-left-radius:var(--radius);border-top-right-radius:var(--radius)}.DocSearch-Cancel{color:hsl(var(--muted-foreground));font-size:.875rem;line-height:1.25rem;padding-left:.5rem;padding-right:.5rem}.DocSearch-MagnifierLabel,.DocSearch-Search-Icon{stroke-width:2;opacity:.5}.DocSearch-Hit-source{color:hsl(var(--muted-foreground))}.DocSearch-Hit,.DocSearch-Hit a{border-radius:calc(var(--radius) - 4px)}.DocSearch-Hit a:focus-visible{outline-offset:-2px}.DocSearch-Hit[aria-selected=true] a{background-color:hsl(var(--accent));color:hsl(var(--accent-foreground))}.DocSearch-Commands{display:none}.DocSearch-Footer{border-color:hsl(var(--border));border-top-width:1px}
```

### Comparing `sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/docsearch.f1a1a5835ed7a6ab0c85.js` & `sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/static/docsearch.8cecda6602174cdd6086.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see docsearch.f1a1a5835ed7a6ab0c85.js.LICENSE.txt */ ! function() {
+/*! For license information please see docsearch.8cecda6602174cdd6086.js.LICENSE.txt */ ! function() {
     "use strict";
 
     function e(e, t) {
         var n = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var r = Object.getOwnPropertySymbols(e);
             t && (r = r.filter((function(t) {
@@ -4397,15 +4397,15 @@
             q = Fe.useRef(null),
             M = Fe.useRef(10),
             H = Fe.useRef("undefined" != typeof window ? window.getSelection().toString().slice(0, 64) : "").current,
             U = Fe.useRef(E || H).current,
             F = function(e, t, n) {
                 return Fe.useMemo((function() {
                     var r = Fr(e, t);
-                    return r.addAlgoliaAgent("docsearch", "3.3.4"), !1 === /docsearch.js \(.*\)/.test(r.transporter.userAgent.value) && r.addAlgoliaAgent("docsearch-react", "3.3.4"), n(r)
+                    return r.addAlgoliaAgent("docsearch", "3.3.5"), !1 === /docsearch.js \(.*\)/.test(r.transporter.userAgent.value) && r.addAlgoliaAgent("docsearch-react", "3.3.5"), n(r)
                 }), [e, t, n])
             }(t, n, b),
             B = Fe.useRef(sr({
                 key: "__DOCSEARCH_FAVORITE_SEARCHES__".concat(r),
                 limit: 10
             })).current,
             V = Fe.useRef(sr({
@@ -4707,15 +4707,16 @@
             var t = e.isOpen,
                 n = e.onOpen,
                 r = e.onClose,
                 o = e.onInput,
                 c = e.searchButtonRef;
             Fe.useEffect((function() {
                 function e(e) {
-                    (27 === e.keyCode && t || "k" === e.key.toLowerCase() && (e.metaKey || e.ctrlKey) || ! function(e) {
+                    var a;
+                    (27 === e.keyCode && t || "k" === (null === (a = e.key) || void 0 === a ? void 0 : a.toLowerCase()) && (e.metaKey || e.ctrlKey) || ! function(e) {
                         var t = e.target,
                             n = t.tagName;
                         return t.isContentEditable || "INPUT" === n || "SELECT" === n || "TEXTAREA" === n
                     }(e) && "/" === e.key && !t) && (e.preventDefault(), t ? r() : document.body.classList.contains("DocSearch--active") || document.body.classList.contains("DocSearch--active") || n()), c && c.current === document.activeElement && o && /[a-zA-Z0-9]/.test(String.fromCharCode(e.keyCode)) && o(e)
                 }
                 return window.addEventListener("keydown", e),
                     function() {
@@ -4740,15 +4741,15 @@
             translations: null == e || null === (n = e.translations) || void 0 === n ? void 0 : n.modal,
             onClose: f
         })), document.body))
     }
     window.docsearch = function(e) {
         Ce(Fe.createElement(Gr, o({}, e, {
             transformSearchClient: function(t) {
-                return t.addAlgoliaAgent("docsearch.js", "3.3.4"), e.transformSearchClient ? e.transformSearchClient(t) : t
+                return t.addAlgoliaAgent("docsearch.js", "3.3.5"), e.transformSearchClient ? e.transformSearchClient(t) : t
             }
         })), function(e) {
             var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : window;
             return "string" == typeof e ? t.document.querySelector(e) : e
         }(e.container, e.environment))
     }
 }();
```

### Comparing `sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/docsearch_config.js_t` & `sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/static/docsearch_config.js_t`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/manifest.json` & `sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/static/manifest.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5789473684210527%*

 * *Differences: {"'_static/docsearch.css'": "'_static/docsearch.82e38f6cd0ccc11d77d4.css'",*

 * * "'_static/docsearch.js'": "'_static/docsearch.8cecda6602174cdd6086.js'",*

 * * "'_static/jetbrains-mono-latin-400-italic.woff'": "'_static/f509ddf49c74ded8c0ee.woff'",*

 * * "'_static/jetbrains-mono-latin-400-italic.woff2'": "'_static/2a472f0334546ace60b3.woff2'",*

 * * "'_static/jetbrains-mono-latin-400-normal.woff'": "'_static/6c1a3008005254946aef.woff'",*

 * * "'_static/jetbrains-mono-latin-400-normal.woff2'": "'_static/4163112e566ed7697acf.woff2'" […]*

```diff
@@ -1,21 +1,21 @@
 {
     "_static/awesome-sphinx-design.css": "_static/awesome-sphinx-design.f3507627e0af8330cfa7.css",
     "_static/awesome-sphinx-design.js": "_static/awesome-sphinx-design.31d6cfe0d16ae931b73c.js",
-    "_static/docsearch.css": "_static/docsearch.445222223e83896718c6.css",
-    "_static/docsearch.js": "_static/docsearch.f1a1a5835ed7a6ab0c85.js",
+    "_static/docsearch.css": "_static/docsearch.82e38f6cd0ccc11d77d4.css",
+    "_static/docsearch.js": "_static/docsearch.8cecda6602174cdd6086.js",
     "_static/docsearch_config.js_t": "_static/docsearch_config.js_t",
-    "_static/jetbrains-mono-latin-400-italic.woff": "_static/ad463ea60cc8b68792f4.woff",
-    "_static/jetbrains-mono-latin-400-italic.woff2": "_static/ff058b7e238adc5cba09.woff2",
-    "_static/jetbrains-mono-latin-400-normal.woff": "_static/6f04107ce68d524ebe69.woff",
-    "_static/jetbrains-mono-latin-400-normal.woff2": "_static/d0b41bd1d599bc0a52b7.woff2",
-    "_static/jetbrains-mono-latin-500-italic.woff": "_static/09be83022f2ac2ce16b0.woff",
-    "_static/jetbrains-mono-latin-500-italic.woff2": "_static/31f64b9c465158bd6066.woff2",
-    "_static/jetbrains-mono-latin-500-normal.woff": "_static/46830c334f8112fa510a.woff",
-    "_static/jetbrains-mono-latin-500-normal.woff2": "_static/ec416b97881f4a422686.woff2",
-    "_static/jetbrains-mono-latin-700-italic.woff": "_static/0ffeb7a552b36437b54c.woff",
-    "_static/jetbrains-mono-latin-700-italic.woff2": "_static/c3b5f43fe4c8f3f1fa21.woff2",
-    "_static/jetbrains-mono-latin-700-normal.woff": "_static/44fd0da18fe361a5cc7f.woff",
-    "_static/jetbrains-mono-latin-700-normal.woff2": "_static/cfdd43ce3499ca7f900a.woff2",
-    "_static/theme.css": "_static/theme.a16405b310edf0713aee.css",
-    "_static/theme.js": "_static/theme.ad172c0f1249198ea036.js"
+    "_static/jetbrains-mono-latin-400-italic.woff": "_static/f509ddf49c74ded8c0ee.woff",
+    "_static/jetbrains-mono-latin-400-italic.woff2": "_static/2a472f0334546ace60b3.woff2",
+    "_static/jetbrains-mono-latin-400-normal.woff": "_static/6c1a3008005254946aef.woff",
+    "_static/jetbrains-mono-latin-400-normal.woff2": "_static/4163112e566ed7697acf.woff2",
+    "_static/jetbrains-mono-latin-500-italic.woff": "_static/5b12b1b913a1d0348fc6.woff",
+    "_static/jetbrains-mono-latin-500-italic.woff2": "_static/c10c163dd1c289f11c49.woff2",
+    "_static/jetbrains-mono-latin-500-normal.woff": "_static/26400cae88e50682937d.woff",
+    "_static/jetbrains-mono-latin-500-normal.woff2": "_static/0ff19efc74e94c856af0.woff2",
+    "_static/jetbrains-mono-latin-700-italic.woff": "_static/b8546ea1646db8ea9c7f.woff",
+    "_static/jetbrains-mono-latin-700-italic.woff2": "_static/aef37e2fab43d03531cd.woff2",
+    "_static/jetbrains-mono-latin-700-normal.woff": "_static/3925889378745d0382d0.woff",
+    "_static/jetbrains-mono-latin-700-normal.woff2": "_static/f4604891b5f1fc1bdbe5.woff2",
+    "_static/theme.css": "_static/theme.871137ef162fc5460fb0.css",
+    "_static/theme.js": "_static/theme.929b2cdd5fa757959a38.js"
 }
```

### Comparing `sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/theme.a16405b310edf0713aee.css` & `sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/static/theme.871137ef162fc5460fb0.css`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 /*! tailwindcss v3.3.2 | MIT License | https://tailwindcss.com*/*,:after,:before{border:0 solid #e5e7eb;box-sizing:border-box}:after,:before{--tw-content:""}html{-webkit-text-size-adjust:100%;font-feature-settings:normal;font-family:ui-sans-serif,system-ui,-apple-system,Segoe UI,Roboto,Ubuntu,Cantarell,Noto Sans,sans-serif,BlinkMacSystemFont,Helvetica Neue,Arial,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji;font-variation-settings:normal;line-height:1.5;-moz-tab-size:4;-o-tab-size:4;tab-size:4}body{line-height:inherit;margin:0}hr{border-top-width:1px;color:inherit;height:0}abbr:where([title]){text-decoration:underline;-webkit-text-decoration:underline dotted;text-decoration:underline dotted}h1,h2,h3,h4,h5,h6{font-size:inherit;font-weight:inherit}a{color:inherit;text-decoration:inherit}b,strong{font-weight:bolder}code,kbd,pre,samp{font-family:JetBrains\ Mono,ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;font-size:1em}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline}sub{bottom:-.25em}sup{top:-.5em}table{border-collapse:collapse;border-color:inherit;text-indent:0}button,input,optgroup,select,textarea{color:inherit;font-family:inherit;font-size:100%;font-weight:inherit;line-height:inherit;margin:0;padding:0}button,select{text-transform:none}[type=button],[type=reset],[type=submit],button{-webkit-appearance:button;background-color:transparent;background-image:none}:-moz-focusring{outline:auto}:-moz-ui-invalid{box-shadow:none}progress{vertical-align:baseline}::-webkit-inner-spin-button,::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}summary{display:list-item}blockquote,dd,dl,figure,h1,h2,h3,h4,h5,h6,hr,p,pre{margin:0}fieldset{margin:0}fieldset,legend{padding:0}menu,ol,ul{list-style:none;margin:0;padding:0}textarea{resize:vertical}input::-moz-placeholder,textarea::-moz-placeholder{color:#9ca3af;opacity:1}input::placeholder,textarea::placeholder{color:#9ca3af;opacity:1}[role=button],button{cursor:pointer}:disabled{cursor:default}audio,canvas,embed,iframe,img,object,svg,video{display:block;vertical-align:middle}img,video{height:auto;max-width:100%}[hidden]{display:none}:root{--background:0 0% 100%;--foreground:222.2 47.4% 11.2%;--muted:210 40% 96.1%;--muted-foreground:215.4 16.3% 46.9%;--popover:0 0% 100%;--popover-foreground:222.2 47.4% 11.2%;--border:214.3 31.8% 91.4%;--input:214.3 31.8% 91.4%;--card:0 0% 100%;--card-foreground:222.2 47.4% 11.2%;--primary:222.2 47.4% 11.2%;--primary-foreground:210 40% 98%;--secondary:210 40% 96.1%;--secondary-foreground:222.2 47.4% 11.2%;--accent:210 40% 96.1%;--accent-foreground:222.2 47.4% 11.2%;--destructive:0 100% 50%;--destructive-foreground:210 40% 98%;--ring:215 20.2% 65.1%;--radius:0.5rem}.dark{--background:224 71% 4%;--foreground:213 31% 91%;--muted:223 47% 11%;--muted-foreground:215.4 16.3% 56.9%;--accent:216 34% 17%;--accent-foreground:210 40% 98%;--popover:224 71% 4%;--popover-foreground:215 20.2% 65.1%;--border:216 34% 17%;--input:216 34% 17%;--card:224 71% 4%;--card-foreground:213 31% 91%;--primary:210 40% 98%;--primary-foreground:222.2 47.4% 1.2%;--secondary:222.2 47.4% 11.2%;--secondary-foreground:210 40% 98%;--destructive:0 63% 31%;--destructive-foreground:210 40% 98%;--ring:216 34% 17%;--radius:0.5rem}*,:after,:before{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgba(59,130,246,.5);--tw-ring-offset-shadow:0 0 transparent;--tw-ring-shadow:0 0 transparent;--tw-shadow:0 0 transparent;--tw-shadow-colored:0 0 transparent;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: }::backdrop{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgba(59,130,246,.5);--tw-ring-offset-shadow:0 0 transparent;--tw-ring-shadow:0 0 transparent;--tw-shadow:0 0 transparent;--tw-shadow-colored:0 0 transparent;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: }.container{margin-left:auto;margin-right:auto;padding-left:2rem;padding-right:2rem;width:100%}@media (min-width:1400px){.container{max-width:1400px}}#content svg{display:inline}#content hr{border-color:#e2e8f0;border-color:hsl(var(--border));margin-bottom:1rem;margin-top:1rem}@media (min-width:768px){#content hr{margin-bottom:1.5rem;margin-top:1.5rem}}#content h1{font-size:2.25rem;font-weight:700;line-height:2.5rem;margin-bottom:.5rem}#content h2{border-bottom-width:1px;border-color:#e2e8f0;border-color:hsl(var(--border));font-size:1.875rem;font-weight:600;line-height:2.25rem;margin-top:3rem;padding-bottom:.5rem}#content h3{font-size:1.5rem;font-weight:600;line-height:2rem;margin-top:2rem}#content .rubric,#content h4{font-size:1.25rem;font-weight:600;line-height:1.75rem;margin-top:2rem}#content section{scroll-margin:5rem}#content section>p{line-height:1.75rem;margin-top:1.5rem}#content section>p.rubric,#content section>p:first-child{margin-top:0}#content section>p.lead{color:#64748b;color:hsl(var(--muted-foreground));font-size:1.125rem;line-height:1.75rem}#content .centered{text-align:center}#content a:not(.toc-backref){color:#0f172a;color:hsl(var(--primary));font-weight:500;text-decoration-line:underline;text-decoration-thickness:from-font;text-underline-offset:4px}#content ul:not(.search){list-style-type:disc;margin-left:1.5rem;margin-top:1.5rem}#content ul:not(.search) p,#content ul:not(.search)>li{margin-top:1.5rem}#content ul:not(.search) ul{margin-top:0}#content ol{list-style-type:decimal;margin-left:1.5rem;margin-top:1.5rem}#content ol ::marker{font-weight:500}#content ol::marker{font-weight:500}#content ol p,#content ol>li{margin-top:1.5rem}#content ol ol{margin-top:0}#content dl{margin-top:1.5rem}#content dl dt:not(.sig){font-weight:500;margin-top:1.5rem}#content dl dt:not(.sig):first-child{margin-bottom:0;margin-top:0}#content dl dd{margin-left:1.5rem}#content dl p{margin-bottom:.5rem;margin-top:.5rem}#content .align-center{margin-left:auto;margin-right:auto;text-align:center}#content .align-right{margin-left:auto;text-align:right}#content img{margin-top:1.5rem}#content figure img{display:inline-block}#content figcaption{color:#64748b;color:hsl(var(--muted-foreground));font-size:.875rem;line-height:1.25rem;margin-bottom:3rem}#content figcaption>*{margin-top:1rem}blockquote{border-left-width:2px;font-style:italic;margin-bottom:1.5rem;margin-top:1.5rem;padding-left:1.5rem}blockquote .attribution{font-style:normal;margin-top:.5rem}table{font-size:.875rem;line-height:1.25rem;margin-bottom:1.5rem;margin-top:1.5rem;width:100%}table caption{color:#64748b;color:hsl(var(--muted-foreground));margin-bottom:1.5rem;text-align:left}table thead{border-bottom-width:1px;border-color:#e2e8f0;border-color:hsl(var(--border))}table th{font-weight:500;padding-bottom:.5rem;padding-left:.5rem;text-align:left}table th:first-child{padding-left:0}.dark table th{font-weight:600}table tbody tr{border-bottom-width:1px;border-color:#e2e8f0;border-color:hsl(var(--border))}table tbody td{padding:.5rem}table tbody td:first-child{padding-left:0}.footnote>.label{float:left;padding-right:.5rem}.footnote>:not(.label){margin-bottom:1.5rem;margin-left:2rem;margin-top:1.5rem}.footnote .footnote-reference,.footnote [role=doc-backlink]{text-decoration-line:none!important}.admonition{background-color:#fff;background-color:hsl(var(--background));border-color:#e2e8f0;border-color:hsl(var(--border));border-radius:.5rem;border-radius:var(--radius);border-width:1px;color:#0f172a;color:hsl(var(--foreground));font-size:.875rem;line-height:1.25rem;margin-bottom:1.5rem;margin-top:1.5rem;padding:1rem}.admonition p:not(.admonition-title){margin-top:.5rem}.admonition .admonition-title{margin-top:0!important}.admonition-title{font-weight:500}.dark .admonition-title{font-weight:600;letter-spacing:.025em}.note{--tw-border-opacity:1;--tw-bg-opacity:1;--tw-text-opacity:1;background-color:#f0f9ff;background-color:rgb(240 249 255/var(--tw-bg-opacity));border-color:#0284c7;border-color:rgb(2 132 199/var(--tw-border-opacity));color:#0c4a6e;color:rgb(12 74 110/var(--tw-text-opacity))}.dark .note{--tw-text-opacity:1;background-color:rgba(96,165,250,.15);color:#e0f2fe;color:rgb(224 242 254/var(--tw-text-opacity))}.hint,.tip{--tw-border-opacity:1;--tw-bg-opacity:1;--tw-text-opacity:1;background-color:#f0fdf4;background-color:rgb(240 253 244/var(--tw-bg-opacity));border-color:#16a34a;border-color:rgb(22 163 74/var(--tw-border-opacity));color:#14532d;color:rgb(20 83 45/var(--tw-text-opacity))}.dark .hint,.dark .tip{--tw-text-opacity:1;background-color:rgba(74,222,128,.15);color:#dcfce7;color:rgb(220 252 231/var(--tw-text-opacity))}.danger,.error{--tw-border-opacity:1;--tw-bg-opacity:1;--tw-text-opacity:1;background-color:#fef2f2;background-color:rgb(254 242 242/var(--tw-bg-opacity));border-color:#dc2626;border-color:rgb(220 38 38/var(--tw-border-opacity));color:#7f1d1d;color:rgb(127 29 29/var(--tw-text-opacity))}.dark .danger,.dark .error{--tw-text-opacity:1;background-color:hsla(0,91%,71%,.15);color:#fee2e2;color:rgb(254 226 226/var(--tw-text-opacity))}.attention,.caution,.important,.warning{--tw-border-opacity:1;--tw-bg-opacity:1;--tw-text-opacity:1;background-color:#fefce8;background-color:rgb(254 252 232/var(--tw-bg-opacity));border-color:#ca8a04;border-color:rgb(202 138 4/var(--tw-border-opacity));color:#713f12;color:rgb(113 63 18/var(--tw-text-opacity))}.dark .attention,.dark .caution,.dark .important,.dark .warning{--tw-text-opacity:1;background-color:rgba(250,204,21,.15);color:#fef9c3;color:rgb(254 249 195/var(--tw-text-opacity))}div.versionadded{--tw-border-opacity:1;border-color:#16a34a;border-color:rgb(22 163 74/var(--tw-border-opacity));border-left-width:3px;font-size:.875rem;line-height:1.25rem;margin-top:1rem;padding:.25rem 1rem}div.versionadded p{margin-top:0!important}div.versionadded p:last-child{margin-bottom:0!important}div.versionadded .versionmodified{--tw-text-opacity:1;color:#14532d;color:rgb(20 83 45/var(--tw-text-opacity));font-weight:500}.dark div.versionadded .versionmodified{--tw-text-opacity:1;color:#22c55e;color:rgb(34 197 94/var(--tw-text-opacity));letter-spacing:.025em}div.versionchanged{--tw-border-opacity:1;border-color:#ca8a04;border-color:rgb(202 138 4/var(--tw-border-opacity));border-left-width:3px;font-size:.875rem;line-height:1.25rem;margin-top:1rem;padding:.25rem 1rem}div.versionchanged p{margin-top:0!important}div.versionchanged p:last-child{margin-bottom:0!important}div.versionchanged .versionmodified{--tw-text-opacity:1;color:#713f12;color:rgb(113 63 18/var(--tw-text-opacity));font-weight:500}.dark div.versionchanged .versionmodified{--tw-text-opacity:1;color:#eab308;color:rgb(234 179 8/var(--tw-text-opacity));letter-spacing:.025em}div.deprecated{--tw-border-opacity:1;border-color:#dc2626;border-color:rgb(220 38 38/var(--tw-border-opacity));border-left-width:3px;font-size:.875rem;line-height:1.25rem;margin-top:1rem;padding:.25rem 1rem}div.deprecated p{margin-top:0!important}div.deprecated p:last-child{margin-bottom:0!important}div.deprecated .versionmodified{--tw-text-opacity:1;color:#7f1d1d;color:rgb(127 29 29/var(--tw-text-opacity));font-weight:500}.dark div.deprecated .versionmodified{--tw-text-opacity:1;color:#f87171;color:rgb(248 113 113/var(--tw-text-opacity));letter-spacing:.025em}.highlight{background-color:transparent;position:relative}.highlight:hover .copy{opacity:1}.literal-block-wrapper{border-color:#e2e8f0;border-color:hsl(var(--border));border-radius:.5rem;border-radius:var(--radius);border-width:1px;margin-left:0;margin-right:0;margin-top:1.5rem;max-width:none;padding-left:0;padding-right:0}.literal-block-wrapper pre{border-radius:0;border-style:none;margin-top:0}.literal-block-wrapper .code-block-caption{border-bottom-width:1px;border-color:#e2e8f0;border-color:hsl(var(--border));border-top-left-radius:.5rem;border-top-left-radius:var(--radius);border-top-right-radius:.5rem;border-top-right-radius:var(--radius);color:#64748b;color:hsl(var(--muted-foreground));font-size:.875rem;letter-spacing:.025em;line-height:1.25rem;padding:.5rem 1rem}code{background-color:#f1f5f9;background-color:hsl(var(--muted));border-radius:.25rem;font-family:JetBrains\ Mono,ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;font-size:.875rem;line-height:1.25rem;padding:.2rem .3rem;position:relative;white-space:nowrap}code .ge,code em{color:#0f172a;color:hsl(var(--accent-foreground));font-weight:700;letter-spacing:.025em}pre{border-color:#e2e8f0;border-color:hsl(var(--border));border-radius:.5rem;border-radius:var(--radius);border-width:1px;font-size:.875rem;line-height:1.25rem;margin-top:1.5rem;overflow-x:auto;padding-bottom:1rem;padding-top:1rem}pre[data-theme=dark]{background-color:#fff;background-color:hsl(var(--background))}pre[data-theme=light]{--tw-bg-opacity:1;background-color:#fff;background-color:rgb(255 255 255/var(--tw-bg-opacity))}pre.literal-block{padding-left:1rem;padding-right:1rem}pre code{background-color:transparent;padding:0;white-space:pre}pre code>[id^=line-]{display:block;padding-left:1rem;padding-right:1rem}pre code [id^=line-]:has(.gd),pre code [id^=line-]:has(.gi),pre code [id^=line-]:has(del),pre code [id^=line-]:has(ins),pre code [id^=line-]:has(mark){padding-left:0;padding-right:0}pre code [id^=line-] del,pre code [id^=line-] ins,pre code [id^=line-] mark{display:block;padding-left:1rem;padding-right:1rem;position:relative}pre code [id^=line-] mark{--tw-shadow:2px 0 currentColor inset;--tw-shadow-colored:inset 2px 0 var(--tw-shadow-color);background-color:#f1f5f9;background-color:hsl(var(--muted));box-shadow:0 0 transparent,0 0 transparent,inset 2px 0 currentColor;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow);color:inherit}.dark pre code [id^=line-] mark{--tw-bg-opacity:1;--tw-shadow:3px 0 currentColor inset;--tw-shadow-colored:inset 3px 0 var(--tw-shadow-color);background-color:#334155;background-color:rgb(51 65 85/var(--tw-bg-opacity));box-shadow:0 0 transparent,0 0 transparent,inset 3px 0 currentColor;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow)}pre code [id^=line-] ins{--tw-text-opacity:1;background-color:rgba(34,197,94,.3);color:#14532d;color:rgb(20 83 45/var(--tw-text-opacity));text-decoration-line:none}pre code [id^=line-] ins:before{--tw-content:"\002b";content:"\002b";content:var(--tw-content);left:2px;position:absolute}.dark pre code [id^=line-] ins{--tw-bg-opacity:1;--tw-text-opacity:1;color:#bbf7d0;color:rgb(187 247 208/var(--tw-text-opacity))}pre code [id^=line-] del{--tw-text-opacity:1;background-color:rgba(239,68,68,.3);color:#7f1d1d;color:rgb(127 29 29/var(--tw-text-opacity));text-decoration-line:none}pre code [id^=line-] del:before{--tw-content:"\2212";content:"\2212";content:var(--tw-content);left:2px;position:absolute}.dark pre code [id^=line-] del{--tw-bg-opacity:1;--tw-text-opacity:1;color:#fecaca;color:rgb(254 202 202/var(--tw-text-opacity))}pre .linenos{padding-left:0;padding-right:1rem;-webkit-user-select:none;-moz-user-select:none;user-select:none}.highlight-diff .gi{--tw-text-opacity:1;background-color:rgba(34,197,94,.3);color:#14532d;color:rgb(20 83 45/var(--tw-text-opacity));display:inline-block;padding-left:1rem;padding-right:1rem;width:100%}.dark .highlight-diff .gi{--tw-bg-opacity:1;--tw-text-opacity:1;color:#bbf7d0;color:rgb(187 247 208/var(--tw-text-opacity))}.highlight-diff .gd{--tw-text-opacity:1;background-color:rgba(239,68,68,.3);color:#7f1d1d;color:rgb(127 29 29/var(--tw-text-opacity));display:inline-block;padding-left:1rem;padding-right:1rem;width:100%}.dark .highlight-diff .gd{--tw-bg-opacity:1;--tw-text-opacity:1;color:#bbf7d0;color:rgb(187 247 208/var(--tw-text-opacity))}.guilabel,.menuselection{border-color:#e2e8f0;border-color:hsl(var(--border));border-radius:calc(.5rem - 4px);border-radius:calc(var(--radius) - 4px);border-width:1px;color:#0f172a;color:hsl(var(--accent-foreground));font-weight:500;padding:1px .5rem}#content kbd:not(.compound){background-color:#f1f5f9;background-color:hsl(var(--muted));border-radius:.25rem;border-width:1px;font-size:.875rem;font-weight:500;letter-spacing:.025em;line-height:1.25rem;padding:1px .25rem}.sig{font-family:JetBrains\ Mono,ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;font-weight:700;scroll-margin:5rem}.sig-name{color:#0f172a;color:hsl(var(--accent-foreground))}em.property{color:#64748b;color:hsl(var(--muted-foreground))}.option .sig-prename{font-style:italic}.viewcode-link{color:#64748b;color:hsl(var(--muted-foreground));float:right}.option-list kbd{background-color:transparent!important;border-style:none!important;font-size:1em!important;font-weight:700!important}.headerlink{align-items:center;display:inline-flex;margin-left:.25rem;position:relative;vertical-align:middle}.headerlink:after{-webkit-font-smoothing:subpixel-antialiased;word-wrap:break-word;--tw-bg-opacity:0.75;background-color:#f1f5f9;background-color:hsl(var(--muted));border-radius:calc(.5rem - 4px);border-radius:calc(var(--radius) - 4px);color:#64748b;color:hsl(var(--muted-foreground));content:attr(data-tooltip);display:none;font-family:ui-sans-serif,system-ui,-apple-system,Segoe UI,Roboto,Ubuntu,Cantarell,Noto Sans,sans-serif,BlinkMacSystemFont,Helvetica Neue,Arial,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji;font-size:.75rem;font-weight:400;letter-spacing:normal;line-height:1rem;opacity:0;padding:.25rem;pointer-events:none;position:absolute;text-align:center;text-decoration-line:none;text-shadow:none;text-transform:none;white-space:pre;z-index:1000000}.headerlink:focus:after,.headerlink:focus:before,.headerlink:hover:after,.headerlink:hover:before{animation-delay:.2s;animation-duration:.4s;animation-fill-mode:forwards;animation-name:tooltip-appear;animation-timing-function:ease-in;display:inline-block;-webkit-text-decoration:none;text-decoration:none}.headerlink:after{margin-top:6px;right:50%;top:100%}.headerlink:before{border-bottom-color:#1a202c;bottom:-7px;margin-right:-6px;right:50%;top:auto}.headerlink:after{margin-right:-16px}.headerlink>*{fill:currentColor;color:#64748b;color:hsl(var(--muted-foreground));visibility:hidden}.admonition-title:hover .headerlink,.admonition-title:hover .headerlink>*,.code-block-caption:hover .headerlink,.code-block-caption:hover .headerlink>*,.headerlink:focus>*,dt:not(.does-not-exist):hover .headerlink,dt:not(.does-not-exist):hover .headerlink>*,figure:not(.does-not-exist):hover .headerlink,figure:not(.does-not-exist):hover .headerlink>*,h1:not(.does-not-exist):hover .headerlink,h1:not(.does-not-exist):hover .headerlink>*,h2:not(.does-not-exist):hover .headerlink,h2:not(.does-not-exist):hover .headerlink>*,h3:not(.does-not-exist):hover .headerlink,h3:not(.does-not-exist):hover .headerlink>*,h4:not(.does-not-exist):hover .headerlink,h4:not(.does-not-exist):hover .headerlink>*,table:not(.does-not-exist):hover .headerlink,table:not(.does-not-exist):hover .headerlink>*{visibility:visible}#left-sidebar .caption{border-radius:calc(.5rem - 2px);border-radius:calc(var(--radius) - 2px);font-size:.875rem;font-weight:600;line-height:1.25rem;margin-bottom:.25rem;padding:1.5rem .5rem .25rem}#left-sidebar .caption:first-child{padding-top:0}#left-sidebar ul{display:grid;font-size:.875rem;grid-auto-flow:row;grid-auto-rows:max-content;line-height:1.25rem;overflow:hidden;transform:translate3d(var(--tw-translate-x),var(--tw-translate-y),0) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transition-duration:.3s;transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1)}@media (prefers-reduced-motion:reduce){#left-sidebar ul{transition-property:none}}#left-sidebar ul ul{margin-left:.75rem;opacity:1;padding:.5rem 0 .5rem .75rem;position:relative;transition-duration:.5s;transition-property:opacity;transition-timing-function:cubic-bezier(.4,0,.2,1)}#left-sidebar ul ul:before{--tw-bg-opacity:1;--tw-content:"";background-color:#e5e7eb;background-color:rgb(229 231 235/var(--tw-bg-opacity));bottom:.25rem;content:"";content:var(--tw-content);left:0;position:absolute;top:.25rem;width:1px}.dark #left-sidebar ul ul:before{--tw-bg-opacity:1;background-color:#262626;background-color:rgb(38 38 38/var(--tw-bg-opacity));content:var(--tw-content)}#left-sidebar a{align-items:center;border-color:transparent;border-radius:calc(.5rem - 2px);border-radius:calc(var(--radius) - 2px);border-width:1px;display:flex;padding:.375rem .5rem;width:100%}#left-sidebar a:hover{text-decoration-line:underline}#left-sidebar a:focus-visible{outline-offset:-1px}#left-sidebar a>button{border-radius:.25rem;color:#64748b;color:hsl(var(--muted-foreground))}#left-sidebar a>button:hover{background-color:rgba(15,23,42,.1);background-color:hsl(var(--primary)/.1)}#left-sidebar a>button>svg{transform:translate3d(var(--tw-translate-x),var(--tw-translate-y),0) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform-origin:center;transition-duration:.15s;transition-property:transform;transition-timing-function:cubic-bezier(.4,0,.2,1)}#left-sidebar a.current{background-color:#f1f5f9;background-color:hsl(var(--accent));border-color:#e2e8f0;border-color:hsl(var(--border));border-width:1px;color:#0f172a;color:hsl(var(--accent-foreground));font-weight:500}#left-sidebar a.expandable{justify-content:space-between}#left-sidebar a.expandable.expanded>button>svg{--tw-rotate:90deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(90deg) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}#right-sidebar ul{margin:0}#right-sidebar ul li{margin-top:0;padding-top:.5rem}#right-sidebar ul li a{color:#64748b;color:hsl(var(--muted-foreground));display:inline-block;text-decoration-line:none;transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1)}#right-sidebar ul li a:hover{color:#0f172a;color:hsl(var(--foreground))}#right-sidebar ul li a:focus-visible{outline-offset:-1px}#right-sidebar ul li a[data-current=true]{color:#0f172a;color:hsl(var(--foreground));font-weight:500}#right-sidebar ul li ul{padding-left:1rem}#right-sidebar ul:not(:last-child){padding-bottom:.5rem}.contents>:not([hidden])~:not([hidden]),.toctree-wrapper>:not([hidden])~:not([hidden]){--tw-space-y-reverse:0;margin-bottom:0;margin-bottom:calc(.5rem*var(--tw-space-y-reverse));margin-top:.5rem;margin-top:calc(.5rem*(1 - var(--tw-space-y-reverse)))}.contents,.toctree-wrapper{font-size:.875rem;line-height:1.25rem}.contents .caption,.contents .topic-title,.toctree-wrapper .caption,.toctree-wrapper .topic-title{font-weight:500;padding-top:1.5rem}.contents ul,.toctree-wrapper ul{list-style-type:none!important;margin:0!important}.contents ul li a.reference,.toctree-wrapper ul li a.reference{color:#64748b!important;color:hsl(var(--muted-foreground))!important;display:inline-block;font-weight:400!important;text-decoration-line:none!important;transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1)}.contents ul li a.reference:hover,.toctree-wrapper ul li a.reference:hover{color:#0f172a;color:hsl(var(--foreground))}.contents ul li ul,.toctree-wrapper ul li ul{padding-left:1rem}.contents ul:not(:last-child),.toctree-wrapper ul:not(:last-child){padding-bottom:.5rem}#search-results .search-summary{color:#64748b;color:hsl(var(--muted-foreground));font-size:1.25rem;line-height:1.75rem;margin-top:1.5rem}#search-results ul.search,#search-results ul.search li{margin-top:1.5rem}#search-results ul.search .context{color:#64748b;color:hsl(var(--muted-foreground));font-size:.875rem;line-height:1.25rem;margin-top:.5rem}.highlighted{background-color:#f1f5f9;background-color:hsl(var(--accent));text-decoration-line:underline;text-decoration-thickness:2px}.highlight-link{border-color:#e2e8f0;border-color:hsl(var(--border));border-radius:.5rem;border-radius:var(--radius);border-width:1px;font-size:.875rem;line-height:1.25rem;padding:.5rem 1rem;position:fixed;right:.5rem;top:4rem}.highlight-link:hover{background-color:#f1f5f9;background-color:hsl(var(--accent))}@media (min-width:1024px){.highlight-link{right:4rem}}.tooltipped{position:relative}.tooltipped:after{-webkit-font-smoothing:subpixel-antialiased;word-wrap:break-word;--tw-bg-opacity:0.75;background-color:#f1f5f9;background-color:hsl(var(--muted));border-radius:calc(.5rem - 4px);border-radius:calc(var(--radius) - 4px);color:#64748b;color:hsl(var(--muted-foreground));content:attr(data-tooltip);display:none;font-family:ui-sans-serif,system-ui,-apple-system,Segoe UI,Roboto,Ubuntu,Cantarell,Noto Sans,sans-serif,BlinkMacSystemFont,Helvetica Neue,Arial,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji;font-size:.75rem;font-weight:400;letter-spacing:normal;line-height:1rem;opacity:0;padding:.25rem;pointer-events:none;position:absolute;text-align:center;text-decoration-line:none;text-shadow:none;text-transform:none;white-space:pre;z-index:1000000}@keyframes tooltip-appear{0%{opacity:0}to{opacity:1}}.tooltipped:focus:after,.tooltipped:focus:before,.tooltipped:hover:after,.tooltipped:hover:before{animation-delay:.2s;animation-duration:.4s;animation-fill-mode:forwards;animation-name:tooltip-appear;animation-timing-function:ease-in;display:inline-block;-webkit-text-decoration:none;text-decoration:none}.tooltipped-no-delay:focus:after,.tooltipped-no-delay:focus:before,.tooltipped-no-delay:hover:after,.tooltipped-no-delay:hover:before{animation-delay:0s}.tooltipped-multiline:focus:after,.tooltipped-multiline:hover:after{display:table-cell}.tooltipped-s:after,.tooltipped-se:after,.tooltipped-sw:after{margin-top:6px;right:50%;top:100%}.tooltipped-s:before,.tooltipped-se:before,.tooltipped-sw:before{border-bottom-color:#1a202c;bottom:-7px;margin-right:-6px;right:50%;top:auto}.tooltipped-se:after{left:50%;margin-left:-16px;right:auto}.tooltipped-sw:after{margin-right:-16px}.tooltipped-n:after,.tooltipped-ne:after,.tooltipped-nw:after{bottom:100%;margin-bottom:6px;right:50%}.tooltipped-n:before,.tooltipped-ne:before,.tooltipped-nw:before{border-top-color:#1a202c;bottom:auto;margin-right:-6px;right:50%;top:-7px}.tooltipped-ne:after{left:50%;margin-left:-16px;right:auto}.tooltipped-nw:after{margin-right:-16px}.tooltipped-n:after,.tooltipped-s:after{transform:translateX(50%)}.tooltipped-w:after{bottom:50%;margin-right:6px;right:100%;transform:translateY(50%)}.tooltipped-w:before{border-left-color:#1a202c;bottom:50%;left:-7px;margin-top:-6px;top:50%}.tooltipped-e:after{bottom:50%;left:100%;margin-left:6px;transform:translateY(50%)}.tooltipped-e:before{border-right-color:#1a202c;bottom:50%;margin-top:-6px;right:-7px;top:50%}.sr-only{clip:rect(0,0,0,0);border-width:0;height:1px;margin:-1px;overflow:hidden;padding:0;position:absolute;white-space:nowrap;width:1px}.pointer-events-none{pointer-events:none}.invisible{visibility:hidden}.collapse{visibility:collapse}.fixed{position:fixed}.absolute{position:absolute}.relative{position:relative}.sticky{position:sticky}.inset-0{left:0;right:0}.inset-0,.inset-y-0{bottom:0;top:0}.bottom-8{bottom:2rem}.left-0{left:0}.right-1{right:.25rem}.right-1\.5{right:.375rem}.right-4{right:1rem}.right-8{right:2rem}.top-0{top:0}.top-16{top:4rem}.top-2{top:.5rem}.top-4{top:1rem}.z-10{z-index:10}.z-20{z-index:20}.z-40{z-index:40}.z-50{z-index:50}.z-\[100\]{z-index:100}.mx-auto{margin-left:auto;margin-right:auto}.my-4{margin-bottom:1rem;margin-top:1rem}.my-6{margin-bottom:1.5rem;margin-top:1.5rem}.my-8{margin-bottom:2rem;margin-top:2rem}.-mt-10{margin-top:-2.5rem}.mb-4{margin-bottom:1rem}.mb-\[2px\]{margin-bottom:2px}.ml-0{margin-left:0}.ml-2{margin-left:.5rem}.ml-auto{margin-left:auto}.mr-1{margin-right:.25rem}.mr-2{margin-right:.5rem}.mr-4{margin-right:1rem}.mr-6{margin-right:1.5rem}.mr-auto{margin-right:auto}.mt-12{margin-top:3rem}.mt-4{margin-top:1rem}.block{display:block}.inline{display:inline}.flex{display:flex}.inline-flex{display:inline-flex}.table{display:table}.hidden{display:none}.h-10{height:2.5rem}.h-14{height:3.5rem}.h-4{height:1rem}.h-5{height:1.25rem}.h-6{height:1.5rem}.h-9{height:2.25rem}.h-\[14px\]{height:14px}.h-\[calc\(100vh-8rem\)\]{height:calc(100vh - 8rem)}.h-full{height:100%}.max-h-\[calc\(var\(--vh\)-4rem\)\]{max-height:calc(var(--vh) - 4rem)}.min-h-screen{min-height:100vh}.w-4{width:1rem}.w-5\/6{width:83.333333%}.w-6{width:1.5rem}.w-9{width:2.25rem}.w-\[14px\]{width:14px}.w-full{width:100%}.min-w-0{min-width:0}.min-w-full{min-width:100%}.max-w-prose{max-width:65ch}.flex-1{flex:1 1 0%}.shrink-0{flex-shrink:0}.-translate-x-full{--tw-translate-x:-100%;transform:translate(-100%,var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.translate-x-0{--tw-translate-x:0px;transform:translateY(var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.rotate-0{--tw-rotate:0deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(0deg) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.rotate-90{--tw-rotate:90deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(90deg) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.scale-0{--tw-scale-x:0;--tw-scale-y:0;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(0) scaleY(0);transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.scale-100{--tw-scale-x:1;--tw-scale-y:1;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(1) scaleY(1)}.scale-100,.transform{transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.select-none{-webkit-user-select:none;-moz-user-select:none;user-select:none}.flex-col{flex-direction:column}.items-start{align-items:flex-start}.items-center{align-items:center}.\!justify-start{justify-content:flex-start!important}.justify-start{justify-content:flex-start}.justify-center{justify-content:center}.justify-between{justify-content:space-between}.gap-1{gap:.25rem}.gap-4{gap:1rem}.space-x-1>:not([hidden])~:not([hidden]){--tw-space-x-reverse:0;margin-left:.25rem;margin-left:calc(.25rem*(1 - var(--tw-space-x-reverse)));margin-right:0;margin-right:calc(.25rem*var(--tw-space-x-reverse))}.space-x-2>:not([hidden])~:not([hidden]){--tw-space-x-reverse:0;margin-left:.5rem;margin-left:calc(.5rem*(1 - var(--tw-space-x-reverse)));margin-right:0;margin-right:calc(.5rem*var(--tw-space-x-reverse))}.space-x-6>:not([hidden])~:not([hidden]){--tw-space-x-reverse:0;margin-left:1.5rem;margin-left:calc(1.5rem*(1 - var(--tw-space-x-reverse)));margin-right:0;margin-right:calc(1.5rem*var(--tw-space-x-reverse))}.space-y-2>:not([hidden])~:not([hidden]){--tw-space-y-reverse:0;margin-bottom:0;margin-bottom:calc(.5rem*var(--tw-space-y-reverse));margin-top:.5rem;margin-top:calc(.5rem*(1 - var(--tw-space-y-reverse)))}.overflow-hidden{overflow:hidden}.overflow-y-auto{overflow-y:auto}.scroll-smooth{scroll-behavior:smooth}.text-ellipsis{text-overflow:ellipsis}.text-clip{text-overflow:clip}.whitespace-nowrap{white-space:nowrap}.rounded{border-radius:.25rem}.rounded-\[0\.5rem\]{border-radius:.5rem}.rounded-md{border-radius:calc(.5rem - 2px);border-radius:calc(var(--radius) - 2px)}.rounded-sm{border-radius:calc(.5rem - 4px);border-radius:calc(var(--radius) - 4px)}.border{border-width:1px}.border-b{border-bottom-width:1px}.border-r{border-right-width:1px}.border-t{border-top-width:1px}.border-border{border-color:#e2e8f0;border-color:hsl(var(--border))}.border-input{border-color:#e2e8f0;border-color:hsl(var(--input))}.bg-background{background-color:#fff;background-color:hsl(var(--background))}.bg-background\/80{background-color:hsla(0,0%,100%,.8);background-color:hsl(var(--background)/.8)}.bg-background\/95{background-color:hsla(0,0%,100%,.95);background-color:hsl(var(--background)/.95)}.bg-gray-700{--tw-bg-opacity:1;background-color:#374151;background-color:rgb(55 65 81/var(--tw-bg-opacity))}.bg-muted{background-color:#f1f5f9;background-color:hsl(var(--muted))}.bg-transparent{background-color:transparent}.fill-current{fill:currentColor}.p-2{padding:.5rem}.p-4{padding:1rem}.p-6{padding:1.5rem}.px-0{padding-left:0;padding-right:0}.px-1{padding-left:.25rem;padding-right:.25rem}.px-1\.5{padding-left:.375rem;padding-right:.375rem}.px-4{padding-left:1rem;padding-right:1rem}.px-8{padding-left:2rem;padding-right:2rem}.py-2{padding-bottom:.5rem;padding-top:.5rem}.py-6{padding-bottom:1.5rem;padding-top:1.5rem}.pr-6{padding-right:1.5rem}.pt-6{padding-top:1.5rem}.text-center{text-align:center}.font-mono{font-family:JetBrains\ Mono,ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace}.font-sans{font-family:ui-sans-serif,system-ui,-apple-system,Segoe UI,Roboto,Ubuntu,Cantarell,Noto Sans,sans-serif,BlinkMacSystemFont,Helvetica Neue,Arial,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji}.text-\[10px\]{font-size:10px}.text-base{font-size:1rem;line-height:1.5rem}.text-sm{font-size:.875rem;line-height:1.25rem}.text-xl{font-size:1.25rem;line-height:1.75rem}.text-xs{font-size:.75rem;line-height:1rem}.font-bold{font-weight:700}.font-medium{font-weight:500}.leading-loose{line-height:2}.text-foreground{color:#0f172a;color:hsl(var(--foreground))}.text-foreground\/60{color:rgba(15,23,42,.6);color:hsl(var(--foreground)/.6)}.text-muted-foreground{color:#64748b;color:hsl(var(--muted-foreground))}.text-red-700{--tw-text-opacity:1;color:#b91c1c;color:rgb(185 28 28/var(--tw-text-opacity))}.text-white{--tw-text-opacity:1;color:#fff;color:rgb(255 255 255/var(--tw-text-opacity))}.underline{text-decoration-line:underline}.underline-offset-4{text-underline-offset:4px}.antialiased{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}.opacity-0{opacity:0}.opacity-100{opacity:1}.opacity-70{opacity:.7}.shadow-sm{--tw-shadow:0 1px 2px 0 rgba(0,0,0,.05);--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);box-shadow:0 0 transparent,0 0 transparent,0 1px 2px 0 rgba(0,0,0,.05);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow)}.ring-offset-background{--tw-ring-offset-color:hsl(var(--background))}.backdrop-blur{--tw-backdrop-blur:blur(8px);-webkit-backdrop-filter:blur(8px) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:blur(8px) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);-webkit-backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia)}.backdrop-blur-sm{--tw-backdrop-blur:blur(4px);-webkit-backdrop-filter:blur(4px) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:blur(4px) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);-webkit-backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia)}.transition{transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,-webkit-backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter,-webkit-backdrop-filter;transition-timing-function:cubic-bezier(.4,0,.2,1)}.transition-all{transition-duration:.15s;transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1)}.transition-colors{transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1)}.transition-opacity{transition-duration:.15s;transition-property:opacity;transition-timing-function:cubic-bezier(.4,0,.2,1)}.duration-100{transition-duration:.1s}.duration-1000{transition-duration:1s}[x-cloak]{display:none!important}@media (max-width:640px){.container{padding-left:1rem;padding-right:1rem}}.hover\:bg-accent:hover{background-color:#f1f5f9;background-color:hsl(var(--accent))}.hover\:bg-gray-950:hover{--tw-bg-opacity:1;background-color:#030712;background-color:rgb(3 7 18/var(--tw-bg-opacity))}.hover\:bg-muted:hover{background-color:#f1f5f9;background-color:hsl(var(--muted))}.hover\:bg-transparent:hover{background-color:transparent}.hover\:text-accent-foreground:hover{color:#0f172a;color:hsl(var(--accent-foreground))}.hover\:text-foreground:hover{color:#0f172a;color:hsl(var(--foreground))}.hover\:text-foreground\/80:hover{color:rgba(15,23,42,.8);color:hsl(var(--foreground)/.8)}.hover\:placeholder-accent-foreground:hover::-moz-placeholder{color:#0f172a;color:hsl(var(--accent-foreground))}.hover\:placeholder-accent-foreground:hover::placeholder{color:#0f172a;color:hsl(var(--accent-foreground))}.hover\:opacity-100:hover{opacity:1}.focus\:translate-x-0:focus{--tw-translate-x:0px;transform:translateY(var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.focus\:bg-accent:focus{background-color:#f1f5f9;background-color:hsl(var(--accent))}.focus\:bg-gray-950:focus{--tw-bg-opacity:1;background-color:#030712;background-color:rgb(3 7 18/var(--tw-bg-opacity))}.focus\:text-accent-foreground:focus{color:#0f172a;color:hsl(var(--accent-foreground))}.focus\:opacity-100:focus{opacity:1}.focus-visible\:outline-none:focus-visible{outline:2px solid transparent;outline-offset:2px}.focus-visible\:ring-2:focus-visible{--tw-ring-offset-shadow:var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow:var(--tw-ring-inset) 0 0 0 calc(2px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color),var(--tw-ring-inset) 0 0 0 calc(2px + var(--tw-ring-offset-width)) var(--tw-ring-color),0 0 transparent;box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow,0 0 #0000)}.focus-visible\:ring-ring:focus-visible{--tw-ring-color:hsl(var(--ring))}.focus-visible\:ring-offset-2:focus-visible{--tw-ring-offset-width:2px}.disabled\:pointer-events-none:disabled{pointer-events:none}.disabled\:opacity-50:disabled{opacity:.5}.group:hover .group-hover\:bg-accent{background-color:#f1f5f9;background-color:hsl(var(--accent))}.group:hover .group-hover\:text-accent-foreground{color:#0f172a;color:hsl(var(--accent-foreground))}.dark .dark\:block{display:block}.dark .dark\:hidden{display:none}.dark .dark\:-rotate-90{--tw-rotate:-90deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(-90deg) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.dark .dark\:rotate-0{--tw-rotate:0deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(0deg) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.dark .dark\:scale-0{--tw-scale-x:0;--tw-scale-y:0;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(0) scaleY(0);transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.dark .dark\:scale-100{--tw-scale-x:1;--tw-scale-y:1;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(1) scaleY(1);transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.dark .dark\:invert{--tw-invert:invert(100%);filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) invert(100%) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow);filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow)}@media (min-width:640px){.sm\:inline-block{display:inline-block}.sm\:flex{display:flex}.sm\:space-x-4>:not([hidden])~:not([hidden]){--tw-space-x-reverse:0;margin-left:1rem;margin-left:calc(1rem*(1 - var(--tw-space-x-reverse)));margin-right:0;margin-right:calc(1rem*var(--tw-space-x-reverse))}.sm\:pr-12{padding-right:3rem}}@media (min-width:768px){.md\:sticky{position:sticky}.md\:top-14{top:3.5rem}.md\:z-30{z-index:30}.md\:my-0{margin-bottom:0;margin-top:0}.md\:-ml-2{margin-left:-.5rem}.md\:inline{display:inline}.md\:flex{display:flex}.md\:grid{display:grid}.md\:\!hidden{display:none!important}.md\:hidden{display:none}.md\:h-24{height:6rem}.md\:h-\[calc\(100vh-3\.5rem\)\]{height:calc(100vh - 3.5rem)}.md\:h-auto{height:auto}.md\:w-40{width:10rem}.md\:w-auto{width:auto}.md\:w-full{width:100%}.md\:flex-none{flex:none}.md\:translate-x-0{--tw-translate-x:0px;transform:translateY(var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.md\:grid-cols-\[220px_minmax\(0\2c 1fr\)\]{grid-template-columns:220px minmax(0,1fr)}.md\:flex-row{flex-direction:row}.md\:justify-end{justify-content:flex-end}.md\:gap-2{gap:.5rem}.md\:gap-6{gap:1.5rem}.md\:overflow-auto{overflow:auto}.md\:bg-transparent{background-color:transparent}.md\:p-0{padding:0}.md\:px-0{padding-left:0;padding-right:0}.md\:py-0{padding-bottom:0;padding-top:0}.md\:text-left{text-align:left}}@media (min-width:1024px){.lg\:my-8{margin-bottom:2rem;margin-top:2rem}.lg\:w-64{width:16rem}.lg\:grid-cols-\[240px_minmax\(0\2c 1fr\)\]{grid-template-columns:240px minmax(0,1fr)}.lg\:gap-10{gap:2.5rem}.lg\:py-8{padding-bottom:2rem;padding-top:2rem}}@media (min-width:1280px){.xl\:block{display:block}.xl\:grid{display:grid}.xl\:grid-cols-\[1fr_300px\]{grid-template-columns:1fr 300px}}
-@font-face{font-display:swap;font-family:JetBrains Mono;font-style:normal;font-weight:400;src:url(d0b41bd1d599bc0a52b7.woff2) format("woff2"),url(6f04107ce68d524ebe69.woff) format("woff")}
-@font-face{font-display:swap;font-family:JetBrains Mono;font-style:italic;font-weight:400;src:url(ff058b7e238adc5cba09.woff2) format("woff2"),url(ad463ea60cc8b68792f4.woff) format("woff")}
-@font-face{font-display:swap;font-family:JetBrains Mono;font-style:normal;font-weight:500;src:url(ec416b97881f4a422686.woff2) format("woff2"),url(46830c334f8112fa510a.woff) format("woff")}
-@font-face{font-display:swap;font-family:JetBrains Mono;font-style:italic;font-weight:500;src:url(31f64b9c465158bd6066.woff2) format("woff2"),url(09be83022f2ac2ce16b0.woff) format("woff")}
-@font-face{font-display:swap;font-family:JetBrains Mono;font-style:normal;font-weight:700;src:url(cfdd43ce3499ca7f900a.woff2) format("woff2"),url(44fd0da18fe361a5cc7f.woff) format("woff")}
-@font-face{font-display:swap;font-family:JetBrains Mono;font-style:italic;font-weight:700;src:url(c3b5f43fe4c8f3f1fa21.woff2) format("woff2"),url(0ffeb7a552b36437b54c.woff) format("woff")}
+@font-face{font-display:swap;font-display:var(--fontsource-display,swap);font-family:JetBrains Mono;font-style:normal;font-weight:400;src:url(4163112e566ed7697acf.woff2) format("woff2"),url(6c1a3008005254946aef.woff) format("woff")}
+@font-face{font-display:swap;font-display:var(--fontsource-display,swap);font-family:JetBrains Mono;font-style:italic;font-weight:400;src:url(2a472f0334546ace60b3.woff2) format("woff2"),url(f509ddf49c74ded8c0ee.woff) format("woff")}
+@font-face{font-display:swap;font-display:var(--fontsource-display,swap);font-family:JetBrains Mono;font-style:normal;font-weight:500;src:url(0ff19efc74e94c856af0.woff2) format("woff2"),url(26400cae88e50682937d.woff) format("woff")}
+@font-face{font-display:swap;font-display:var(--fontsource-display,swap);font-family:JetBrains Mono;font-style:italic;font-weight:500;src:url(c10c163dd1c289f11c49.woff2) format("woff2"),url(5b12b1b913a1d0348fc6.woff) format("woff")}
+@font-face{font-display:swap;font-display:var(--fontsource-display,swap);font-family:JetBrains Mono;font-style:normal;font-weight:700;src:url(f4604891b5f1fc1bdbe5.woff2) format("woff2"),url(3925889378745d0382d0.woff) format("woff")}
+@font-face{font-display:swap;font-display:var(--fontsource-display,swap);font-family:JetBrains Mono;font-style:italic;font-weight:700;src:url(aef37e2fab43d03531cd.woff2) format("woff2"),url(b8546ea1646db8ea9c7f.woff) format("woff")}
```

### Comparing `sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/theme.ad172c0f1249198ea036.js` & `sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/static/theme.929b2cdd5fa757959a38.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
-/*! For license information please see theme.ad172c0f1249198ea036.js.LICENSE.txt */ ! function() {
+/*! For license information please see theme.929b2cdd5fa757959a38.js.LICENSE.txt */ ! function() {
     var e = {
-            152: function(e) {
+            13: function(e) {
                 var t;
                 t = function() {
                     return function() {
                         var e = {
                                 686: function(e, t, n) {
                                     "use strict";
                                     n.d(t, {
@@ -69,60 +69,60 @@
                                     function h(e, t) {
                                         for (var n = 0; n < t.length; n++) {
                                             var r = t[n];
                                             r.enumerable = r.enumerable || !1, r.configurable = !0, "value" in r && (r.writable = !0), Object.defineProperty(e, r.key, r)
                                         }
                                     }
 
-                                    function y(e, t) {
-                                        return y = Object.setPrototypeOf || function(e, t) {
+                                    function m(e, t) {
+                                        return m = Object.setPrototypeOf || function(e, t) {
                                             return e.__proto__ = t, e
-                                        }, y(e, t)
+                                        }, m(e, t)
                                     }
 
-                                    function v(e) {
-                                        return v = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
+                                    function y(e) {
+                                        return y = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
                                             return e.__proto__ || Object.getPrototypeOf(e)
-                                        }, v(e)
+                                        }, y(e)
                                     }
 
-                                    function m(e, t) {
+                                    function v(e, t) {
                                         var n = "data-clipboard-".concat(e);
                                         if (t.hasAttribute(n)) return t.getAttribute(n)
                                     }
                                     var g = function(e) {
                                             ! function(e, t) {
                                                 if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function");
                                                 e.prototype = Object.create(t && t.prototype, {
                                                     constructor: {
                                                         value: e,
                                                         writable: !0,
                                                         configurable: !0
                                                     }
-                                                }), t && y(e, t)
+                                                }), t && m(e, t)
                                             }(l, e);
                                             var t, n, r, i, o, s = (i = l, o = function() {
                                                 if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
                                                 if (Reflect.construct.sham) return !1;
                                                 if ("function" == typeof Proxy) return !0;
                                                 try {
                                                     return Date.prototype.toString.call(Reflect.construct(Date, [], (function() {}))), !0
                                                 } catch (e) {
                                                     return !1
                                                 }
                                             }(), function() {
-                                                var e, t, n = v(i);
+                                                var e, t, n, r = y(i);
                                                 if (o) {
-                                                    var r = v(this).constructor;
-                                                    e = Reflect.construct(n, arguments, r)
-                                                } else e = n.apply(this, arguments);
-                                                return !(t = e) || "object" !== _(t) && "function" != typeof t ? function(e) {
+                                                    var a = y(this).constructor;
+                                                    e = Reflect.construct(r, arguments, a)
+                                                } else e = r.apply(this, arguments);
+                                                return t = this, !(n = e) || "object" !== _(n) && "function" != typeof n ? function(e) {
                                                     if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
                                                     return e
-                                                }(this) : t
+                                                }(t) : n
                                             });
 
                                             function l(e, t) {
                                                 var n;
                                                 return function(e, t) {
                                                     if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
                                                 }(this, l), (n = s.call(this)).resolveOptions(t), n.listenClick(e), n
@@ -178,26 +178,26 @@
                                                             t && t.focus(), window.getSelection().removeAllRanges()
                                                         }
                                                     })
                                                 }
                                             }, {
                                                 key: "defaultAction",
                                                 value: function(e) {
-                                                    return m("action", e)
+                                                    return v("action", e)
                                                 }
                                             }, {
                                                 key: "defaultTarget",
                                                 value: function(e) {
-                                                    var t = m("target", e);
+                                                    var t = v("target", e);
                                                     if (t) return document.querySelector(t)
                                                 }
                                             }, {
                                                 key: "defaultText",
                                                 value: function(e) {
-                                                    return m("text", e)
+                                                    return v("text", e)
                                                 }
                                             }, {
                                                 key: "destroy",
                                                 value: function() {
                                                     this.listener.destroy()
                                                 }
                                             }], r = [{
@@ -404,82 +404,476 @@
                 a: t
             }), t
         }, n.d = function(e, t) {
             for (var r in t) n.o(t, r) && !n.o(e, r) && Object.defineProperty(e, r, {
                 enumerable: !0,
                 get: t[r]
             })
-        }, n.o = function(e, t) {
+        }, n.g = function() {
+            if ("object" == typeof globalThis) return globalThis;
+            try {
+                return this || new Function("return this")()
+            } catch (e) {
+                if ("object" == typeof window) return window
+            }
+        }(), n.o = function(e, t) {
             return Object.prototype.hasOwnProperty.call(e, t)
         },
         function() {
             "use strict";
-            var e, t, r, i, o = !1,
-                a = !1,
-                s = [],
-                l = -1;
 
-            function c(e) {
-                let t = s.indexOf(e); - 1 !== t && t > l && s.splice(t, 1)
+            function e(e, t) {
+                const n = Object.create(null),
+                    r = e.split(",");
+                for (let e = 0; e < r.length; e++) n[r[e]] = !0;
+                return t ? e => !!n[e.toLowerCase()] : e => !!n[e]
             }
+            const t = {},
+                r = (Object.assign, Object.prototype.hasOwnProperty),
+                i = (e, t) => r.call(e, t),
+                o = Array.isArray,
+                a = e => "[object Map]" === u(e),
+                s = e => "symbol" == typeof e,
+                l = e => null !== e && "object" == typeof e,
+                c = Object.prototype.toString,
+                u = e => c.call(e),
+                f = e => u(e).slice(8, -1),
+                d = e => "string" == typeof e && "NaN" !== e && "-" !== e[0] && "" + parseInt(e, 10) === e,
+                p = e => {
+                    const t = Object.create(null);
+                    return n => t[n] || (t[n] = e(n))
+                },
+                _ = /-(\w)/g,
+                h = (p((e => e.replace(_, ((e, t) => t ? t.toUpperCase() : "")))), /\B([A-Z])/g),
+                m = (p((e => e.replace(h, "-$1").toLowerCase())), p((e => e.charAt(0).toUpperCase() + e.slice(1)))),
+                y = (p((e => e ? `on${m(e)}` : "")), (e, t) => e !== t && (e == e || t == t)),
+                v = new WeakMap,
+                g = [];
+            let x;
+            const b = Symbol(""),
+                w = Symbol("");
+            let E = 0;
 
-            function u() {
-                o = !1, a = !0;
-                for (let e = 0; e < s.length; e++) s[e](), l = e;
-                s.length = 0, l = -1, a = !1
+            function S(e) {
+                const {
+                    deps: t
+                } = e;
+                if (t.length) {
+                    for (let n = 0; n < t.length; n++) t[n].delete(e);
+                    t.length = 0
+                }
             }
-            var f = !0;
+            let A = !0;
+            const O = [];
 
-            function d(e) {
-                t = e
+            function k() {
+                const e = O.pop();
+                A = void 0 === e || e
             }
-            var p = [],
-                _ = [],
-                h = [];
 
-            function y(e, t) {
-                "function" == typeof t ? (e._x_cleanups || (e._x_cleanups = []), e._x_cleanups.push(t)) : (t = e, _.push(t))
+            function C(e, t, n) {
+                if (!A || void 0 === x) return;
+                let r = v.get(e);
+                r || v.set(e, r = new Map);
+                let i = r.get(n);
+                i || r.set(n, i = new Set), i.has(x) || (i.add(x), x.deps.push(i))
             }
 
-            function v(e, t) {
+            function j(e, t, n, r, i, s) {
+                const l = v.get(e);
+                if (!l) return;
+                const c = new Set,
+                    u = e => {
+                        e && e.forEach((e => {
+                            (e !== x || e.allowRecurse) && c.add(e)
+                        }))
+                    };
+                if ("clear" === t) l.forEach(u);
+                else if ("length" === n && o(e)) l.forEach(((e, t) => {
+                    ("length" === t || t >= r) && u(e)
+                }));
+                else switch (void 0 !== n && u(l.get(n)), t) {
+                    case "add":
+                        o(e) ? d(n) && u(l.get("length")) : (u(l.get(b)), a(e) && u(l.get(w)));
+                        break;
+                    case "delete":
+                        o(e) || (u(l.get(b)), a(e) && u(l.get(w)));
+                        break;
+                    case "set":
+                        a(e) && u(l.get(b))
+                }
+                c.forEach((e => {
+                    e.options.scheduler ? e.options.scheduler(e) : e()
+                }))
+            }
+            const T = e("__proto__,__v_isRef,__isVue"),
+                L = new Set(Object.getOwnPropertyNames(Symbol).map((e => Symbol[e])).filter(s)),
+                M = R(),
+                $ = R(!0),
+                N = P();
+
+            function P() {
+                const e = {};
+                return ["includes", "indexOf", "lastIndexOf"].forEach((t => {
+                    e[t] = function(...e) {
+                        const n = he(this);
+                        for (let e = 0, t = this.length; e < t; e++) C(n, 0, e + "");
+                        const r = n[t](...e);
+                        return -1 === r || !1 === r ? n[t](...e.map(he)) : r
+                    }
+                })), ["push", "pop", "shift", "unshift", "splice"].forEach((t => {
+                    e[t] = function(...e) {
+                        O.push(A), A = !1;
+                        const n = he(this)[t].apply(this, e);
+                        return k(), n
+                    }
+                })), e
+            }
+
+            function R(e = !1, t = !1) {
+                return function(n, r, a) {
+                    if ("__v_isReactive" === r) return !e;
+                    if ("__v_isReadonly" === r) return e;
+                    if ("__v_raw" === r && a === (e ? t ? fe : ue : t ? ce : le).get(n)) return n;
+                    const c = o(n);
+                    if (!e && c && i(N, r)) return Reflect.get(N, r, a);
+                    const u = Reflect.get(n, r, a);
+                    return (s(r) ? L.has(r) : T(r)) ? u : (e || C(n, 0, r), t ? u : me(u) ? c && d(r) ? u : u.value : l(u) ? e ? pe(u) : de(u) : u)
+                }
+            }
+
+            function q(e = !1) {
+                return function(t, n, r, a) {
+                    let s = t[n];
+                    if (!e && (r = he(r), s = he(s), !o(t) && me(s) && !me(r))) return s.value = r, !0;
+                    const l = o(t) && d(n) ? Number(n) < t.length : i(t, n),
+                        c = Reflect.set(t, n, r, a);
+                    return t === he(a) && (l ? y(r, s) && j(t, "set", n, r) : j(t, "add", n, r)), c
+                }
+            }
+            const I = {
+                    get: M,
+                    set: q(),
+                    deleteProperty: function(e, t) {
+                        const n = i(e, t),
+                            r = (e[t], Reflect.deleteProperty(e, t));
+                        return r && n && j(e, "delete", t, void 0), r
+                    },
+                    has: function(e, t) {
+                        const n = Reflect.has(e, t);
+                        return s(t) && L.has(t) || C(e, 0, t), n
+                    },
+                    ownKeys: function(e) {
+                        return C(e, 0, o(e) ? "length" : b), Reflect.ownKeys(e)
+                    }
+                },
+                z = {
+                    get: $,
+                    set(e, t) {
+                        return !0
+                    },
+                    deleteProperty(e, t) {
+                        return !0
+                    }
+                },
+                D = e => l(e) ? de(e) : e,
+                F = e => l(e) ? pe(e) : e,
+                B = e => e,
+                H = e => Reflect.getPrototypeOf(e);
+
+            function W(e, t, n = !1, r = !1) {
+                const i = he(e = e.__v_raw),
+                    o = he(t);
+                t !== o && !n && C(i, 0, t), !n && C(i, 0, o);
+                const {
+                    has: a
+                } = H(i), s = r ? B : n ? F : D;
+                return a.call(i, t) ? s(e.get(t)) : a.call(i, o) ? s(e.get(o)) : void(e !== i && e.get(t))
+            }
+
+            function V(e, t = !1) {
+                const n = this.__v_raw,
+                    r = he(n),
+                    i = he(e);
+                return e !== i && !t && C(r, 0, e), !t && C(r, 0, i), e === i ? n.has(e) : n.has(e) || n.has(i)
+            }
+
+            function U(e, t = !1) {
+                return e = e.__v_raw, !t && C(he(e), 0, b), Reflect.get(e, "size", e)
+            }
+
+            function Z(e) {
+                e = he(e);
+                const t = he(this);
+                return H(t).has.call(t, e) || (t.add(e), j(t, "add", e, e)), this
+            }
+
+            function K(e, t) {
+                t = he(t);
+                const n = he(this),
+                    {
+                        has: r,
+                        get: i
+                    } = H(n);
+                let o = r.call(n, e);
+                o || (e = he(e), o = r.call(n, e));
+                const a = i.call(n, e);
+                return n.set(e, t), o ? y(t, a) && j(n, "set", e, t) : j(n, "add", e, t), this
+            }
+
+            function J(e) {
+                const t = he(this),
+                    {
+                        has: n,
+                        get: r
+                    } = H(t);
+                let i = n.call(t, e);
+                i || (e = he(e), i = n.call(t, e)), r && r.call(t, e);
+                const o = t.delete(e);
+                return i && j(t, "delete", e, void 0), o
+            }
+
+            function X() {
+                const e = he(this),
+                    t = 0 !== e.size,
+                    n = e.clear();
+                return t && j(e, "clear", void 0, void 0), n
+            }
+
+            function Y(e, t) {
+                return function(n, r) {
+                    const i = this,
+                        o = i.__v_raw,
+                        a = he(o),
+                        s = t ? B : e ? F : D;
+                    return !e && C(a, 0, b), o.forEach(((e, t) => n.call(r, s(e), s(t), i)))
+                }
+            }
+
+            function G(e, t, n) {
+                return function(...r) {
+                    const i = this.__v_raw,
+                        o = he(i),
+                        s = a(o),
+                        l = "entries" === e || e === Symbol.iterator && s,
+                        c = "keys" === e && s,
+                        u = i[e](...r),
+                        f = n ? B : t ? F : D;
+                    return !t && C(o, 0, c ? w : b), {
+                        next() {
+                            const {
+                                value: e,
+                                done: t
+                            } = u.next();
+                            return t ? {
+                                value: e,
+                                done: t
+                            } : {
+                                value: l ? [f(e[0]), f(e[1])] : f(e),
+                                done: t
+                            }
+                        },
+                        [Symbol.iterator]() {
+                            return this
+                        }
+                    }
+                }
+            }
+
+            function Q(e) {
+                return function(...t) {
+                    return "delete" !== e && this
+                }
+            }
+
+            function ee() {
+                const e = {
+                        get(e) {
+                            return W(this, e)
+                        },
+                        get size() {
+                            return U(this)
+                        },
+                        has: V,
+                        add: Z,
+                        set: K,
+                        delete: J,
+                        clear: X,
+                        forEach: Y(!1, !1)
+                    },
+                    t = {
+                        get(e) {
+                            return W(this, e, !1, !0)
+                        },
+                        get size() {
+                            return U(this)
+                        },
+                        has: V,
+                        add: Z,
+                        set: K,
+                        delete: J,
+                        clear: X,
+                        forEach: Y(!1, !0)
+                    },
+                    n = {
+                        get(e) {
+                            return W(this, e, !0)
+                        },
+                        get size() {
+                            return U(this, !0)
+                        },
+                        has(e) {
+                            return V.call(this, e, !0)
+                        },
+                        add: Q("add"),
+                        set: Q("set"),
+                        delete: Q("delete"),
+                        clear: Q("clear"),
+                        forEach: Y(!0, !1)
+                    },
+                    r = {
+                        get(e) {
+                            return W(this, e, !0, !0)
+                        },
+                        get size() {
+                            return U(this, !0)
+                        },
+                        has(e) {
+                            return V.call(this, e, !0)
+                        },
+                        add: Q("add"),
+                        set: Q("set"),
+                        delete: Q("delete"),
+                        clear: Q("clear"),
+                        forEach: Y(!0, !0)
+                    };
+                return ["keys", "values", "entries", Symbol.iterator].forEach((i => {
+                    e[i] = G(i, !1, !1), n[i] = G(i, !0, !1), t[i] = G(i, !1, !0), r[i] = G(i, !0, !0)
+                })), [e, n, t, r]
+            }
+            const [te, ne, re, ie] = ee();
+
+            function oe(e, t) {
+                const n = t ? e ? ie : re : e ? ne : te;
+                return (t, r, o) => "__v_isReactive" === r ? !e : "__v_isReadonly" === r ? e : "__v_raw" === r ? t : Reflect.get(i(n, r) && r in t ? n : t, r, o)
+            }
+            const ae = {
+                    get: oe(!1, !1)
+                },
+                se = {
+                    get: oe(!0, !1)
+                },
+                le = new WeakMap,
+                ce = new WeakMap,
+                ue = new WeakMap,
+                fe = new WeakMap;
+
+            function de(e) {
+                return e && e.__v_isReadonly ? e : _e(e, !1, I, ae, le)
+            }
+
+            function pe(e) {
+                return _e(e, !0, z, se, ue)
+            }
+
+            function _e(e, t, n, r, i) {
+                if (!l(e)) return e;
+                if (e.__v_raw && (!t || !e.__v_isReactive)) return e;
+                const o = i.get(e);
+                if (o) return o;
+                const a = (s = e).__v_skip || !Object.isExtensible(s) ? 0 : function(e) {
+                    switch (e) {
+                        case "Object":
+                        case "Array":
+                            return 1;
+                        case "Map":
+                        case "Set":
+                        case "WeakMap":
+                        case "WeakSet":
+                            return 2;
+                        default:
+                            return 0
+                    }
+                }(f(s));
+                var s;
+                if (0 === a) return e;
+                const c = new Proxy(e, 2 === a ? r : n);
+                return i.set(e, c), c
+            }
+
+            function he(e) {
+                return e && he(e.__v_raw) || e
+            }
+
+            function me(e) {
+                return Boolean(e && !0 === e.__v_isRef)
+            }
+            var ye, ve, ge, xe, be = !1,
+                we = !1,
+                Ee = [],
+                Se = -1;
+
+            function Ae(e) {
+                let t = Ee.indexOf(e); - 1 !== t && t > Se && Ee.splice(t, 1)
+            }
+
+            function Oe() {
+                be = !1, we = !0;
+                for (let e = 0; e < Ee.length; e++) Ee[e](), Se = e;
+                Ee.length = 0, Se = -1, we = !1
+            }
+            var ke = !0;
+
+            function Ce(e) {
+                ve = e
+            }
+            var je = [],
+                Te = [],
+                Le = [];
+
+            function Me(e, t) {
+                "function" == typeof t ? (e._x_cleanups || (e._x_cleanups = []), e._x_cleanups.push(t)) : (t = e, Te.push(t))
+            }
+
+            function $e(e, t) {
                 e._x_attributeCleanups && Object.entries(e._x_attributeCleanups).forEach((([n, r]) => {
                     (void 0 === t || t.includes(n)) && (r.forEach((e => e())), delete e._x_attributeCleanups[n])
                 }))
             }
-            var m = new MutationObserver(k),
-                g = !1;
+            var Ne = new MutationObserver(He),
+                Pe = !1;
 
-            function x() {
-                m.observe(document, {
+            function Re() {
+                Ne.observe(document, {
                     subtree: !0,
                     childList: !0,
                     attributes: !0,
                     attributeOldValue: !0
-                }), g = !0
+                }), Pe = !0
             }
 
-            function b() {
-                (w = w.concat(m.takeRecords())).length && !E && (E = !0, queueMicrotask((() => {
-                    k(w), w.length = 0, E = !1
-                }))), m.disconnect(), g = !1
+            function qe() {
+                (Ie = Ie.concat(Ne.takeRecords())).length && !ze && (ze = !0, queueMicrotask((() => {
+                    He(Ie), Ie.length = 0, ze = !1
+                }))), Ne.disconnect(), Pe = !1
             }
-            var w = [],
-                E = !1;
+            var Ie = [],
+                ze = !1;
 
-            function S(e) {
-                if (!g) return e();
-                b();
+            function De(e) {
+                if (!Pe) return e();
+                qe();
                 let t = e();
-                return x(), t
+                return Re(), t
             }
-            var O = !1,
-                A = [];
+            var Fe = !1,
+                Be = [];
 
-            function k(e) {
-                if (O) return void(A = A.concat(e));
+            function He(e) {
+                if (Fe) return void(Be = Be.concat(e));
                 let t = [],
                     n = [],
                     r = new Map,
                     i = new Map;
                 for (let o = 0; o < e.length; o++)
                     if (!e[o].target._x_ignoreMutationObserver && ("childList" === e[o].type && (e[o].addedNodes.forEach((e => 1 === e.nodeType && t.push(e))), e[o].removedNodes.forEach((e => 1 === e.nodeType && n.push(e)))), "attributes" === e[o].type)) {
                         let t = e[o].target,
@@ -492,52 +886,45 @@
                                 })
                             },
                             l = () => {
                                 i.has(t) || i.set(t, []), i.get(t).push(n)
                             };
                         t.hasAttribute(n) && null === a ? s() : t.hasAttribute(n) ? (l(), s()) : l()
                     } i.forEach(((e, t) => {
-                    v(t, e)
+                    $e(t, e)
                 })), r.forEach(((e, t) => {
-                    p.forEach((n => n(t, e)))
+                    je.forEach((n => n(t, e)))
                 }));
                 for (let e of n)
-                    if (!t.includes(e) && (_.forEach((t => t(e))), e._x_cleanups))
+                    if (!t.includes(e) && (Te.forEach((t => t(e))), e._x_cleanups))
                         for (; e._x_cleanups.length;) e._x_cleanups.pop()();
                 t.forEach((e => {
                     e._x_ignoreSelf = !0, e._x_ignore = !0
                 }));
-                for (let e of t) n.includes(e) || e.isConnected && (delete e._x_ignoreSelf, delete e._x_ignore, h.forEach((t => t(e))), e._x_ignore = !0, e._x_ignoreSelf = !0);
+                for (let e of t) n.includes(e) || e.isConnected && (delete e._x_ignoreSelf, delete e._x_ignore, Le.forEach((t => t(e))), e._x_ignore = !0, e._x_ignoreSelf = !0);
                 t.forEach((e => {
                     delete e._x_ignoreSelf, delete e._x_ignore
                 })), t = null, n = null, r = null, i = null
             }
 
-            function C(e) {
-                return $(L(e))
+            function We(e) {
+                return Ze(Ue(e))
             }
 
-            function j(e, t, n) {
-                return e._x_dataStack = [t, ...L(n || e)], () => {
+            function Ve(e, t, n) {
+                return e._x_dataStack = [t, ...Ue(n || e)], () => {
                     e._x_dataStack = e._x_dataStack.filter((e => e !== t))
                 }
             }
 
-            function T(e, t) {
-                let n = e._x_dataStack[0];
-                Object.entries(t).forEach((([e, t]) => {
-                    n[e] = t
-                }))
-            }
-
-            function L(e) {
-                return e._x_dataStack ? e._x_dataStack : "function" == typeof ShadowRoot && e instanceof ShadowRoot ? L(e.host) : e.parentNode ? L(e.parentNode) : []
+            function Ue(e) {
+                return e._x_dataStack ? e._x_dataStack : "function" == typeof ShadowRoot && e instanceof ShadowRoot ? Ue(e.host) : e.parentNode ? Ue(e.parentNode) : []
             }
 
-            function $(e) {
+            function Ze(e) {
                 let t = new Proxy({}, {
                     ownKeys: () => Array.from(new Set(e.flatMap((e => Object.keys(e))))),
                     has: (t, n) => e.some((e => e.hasOwnProperty(n))),
                     get: (n, r) => (e.find((e => {
                         if (e.hasOwnProperty(r)) {
                             let n = Object.getOwnPropertyDescriptor(e, r);
                             if (n.get && n.get._x_alreadyBound || n.set && n.set._x_alreadyBound) return !0;
@@ -559,502 +946,508 @@
                         let i = e.find((e => e.hasOwnProperty(n)));
                         return i ? i[n] = r : e[e.length - 1][n] = r, !0
                     }
                 });
                 return t
             }
 
-            function M(e) {
+            function Ke(e) {
                 let t = (n, r = "") => {
                     Object.entries(Object.getOwnPropertyDescriptors(n)).forEach((([i, {
                         value: o,
                         enumerable: a
                     }]) => {
                         if (!1 === a || void 0 === o) return;
                         let s = "" === r ? i : `${r}.${i}`;
                         var l;
                         "object" == typeof o && null !== o && o._x_interceptor ? n[i] = o.initialize(e, s, i) : "object" != typeof(l = o) || Array.isArray(l) || null === l || o === n || o instanceof Element || t(o, s)
                     }))
                 };
                 return t(e)
             }
 
-            function N(e, t = (() => {})) {
+            function Je(e, t = (() => {})) {
                 let n = {
                     initialValue: void 0,
                     _x_interceptor: !0,
                     initialize(t, n, r) {
                         return e(this.initialValue, (() => function(e, t) {
                             return t.split(".").reduce(((e, t) => e[t]), e)
-                        }(t, n)), (e => P(t, n, e)), n, r)
+                        }(t, n)), (e => Xe(t, n, e)), n, r)
                     }
                 };
                 return t(n), e => {
                     if ("object" == typeof e && null !== e && e._x_interceptor) {
                         let t = n.initialize.bind(n);
                         n.initialize = (r, i, o) => {
                             let a = e.initialize(r, i, o);
                             return n.initialValue = a, t(r, i, o)
                         }
                     } else n.initialValue = e;
                     return n
                 }
             }
 
-            function P(e, t, n) {
+            function Xe(e, t, n) {
                 if ("string" == typeof t && (t = t.split(".")), 1 !== t.length) {
                     if (0 === t.length) throw error;
-                    return e[t[0]] || (e[t[0]] = {}), P(e[t[0]], t.slice(1), n)
+                    return e[t[0]] || (e[t[0]] = {}), Xe(e[t[0]], t.slice(1), n)
                 }
                 e[t[0]] = n
             }
-            var R = {};
+            var Ye = {};
 
-            function q(e, t) {
-                R[e] = t
+            function Ge(e, t) {
+                Ye[e] = t
             }
 
-            function I(e, t) {
-                return Object.entries(R).forEach((([n, r]) => {
+            function Qe(e, t) {
+                return Object.entries(Ye).forEach((([n, r]) => {
+                    let i = null;
                     Object.defineProperty(e, `$${n}`, {
                         get() {
-                            let [e, n] = re(t);
-                            return e = {
-                                interceptor: N,
-                                ...e
-                            }, y(t, n), r(t, e)
+                            return r(t, function() {
+                                if (i) return i; {
+                                    let [e, n] = vt(t);
+                                    return i = {
+                                        interceptor: Je,
+                                        ...e
+                                    }, Me(t, n), i
+                                }
+                            }())
                         },
                         enumerable: !1
                     })
                 })), e
             }
 
-            function z(e, t, n, ...r) {
+            function et(e, t, n, ...r) {
                 try {
                     return n(...r)
                 } catch (n) {
-                    D(n, e, t)
+                    tt(n, e, t)
                 }
             }
 
-            function D(e, t, n = void 0) {
+            function tt(e, t, n = void 0) {
                 Object.assign(e, {
                     el: t,
                     expression: n
                 }), console.warn(`Alpine Expression Error: ${e.message}\n\n${n?'Expression: "'+n+'"\n\n':""}`, t), setTimeout((() => {
                     throw e
                 }), 0)
             }
-            var B = !0;
+            var nt = !0;
 
-            function F(e, t, n = {}) {
+            function rt(e, t, n = {}) {
                 let r;
-                return H(e, t)((e => r = e), n), r
+                return it(e, t)((e => r = e), n), r
             }
 
-            function H(...e) {
-                return W(...e)
+            function it(...e) {
+                return ot(...e)
             }
-            var W = V;
+            var ot = at;
 
-            function V(e, t) {
+            function at(e, t) {
                 let n = {};
-                I(n, e);
-                let r = [n, ...L(e)],
+                Qe(n, e);
+                let r = [n, ...Ue(e)],
                     i = "function" == typeof t ? function(e, t) {
                         return (n = (() => {}), {
                             scope: r = {},
                             params: i = []
                         } = {}) => {
-                            Z(n, t.apply($([r, ...e]), i))
+                            lt(n, t.apply(Ze([r, ...e]), i))
                         }
                     }(r, t) : function(e, t, n) {
                         let r = function(e, t) {
-                            if (U[e]) return U[e];
+                            if (st[e]) return st[e];
                             let n = Object.getPrototypeOf((async function() {})).constructor,
                                 r = /^[\n\s]*if.*\(.*\)/.test(e) || /^(let|const)\s/.test(e) ? `(async()=>{ ${e} })()` : e;
                             let i = (() => {
                                 try {
                                     return new n(["__self", "scope"], `with (scope) { __self.result = ${r} }; __self.finished = true; return __self.result;`)
                                 } catch (n) {
-                                    return D(n, t, e), Promise.resolve()
+                                    return tt(n, t, e), Promise.resolve()
                                 }
                             })();
-                            return U[e] = i, i
+                            return st[e] = i, i
                         }(t, n);
                         return (i = (() => {}), {
                             scope: o = {},
                             params: a = []
                         } = {}) => {
                             r.result = void 0, r.finished = !1;
-                            let s = $([o, ...e]);
+                            let s = Ze([o, ...e]);
                             if ("function" == typeof r) {
-                                let e = r(r, s).catch((e => D(e, n, t)));
-                                r.finished ? (Z(i, r.result, s, a, n), r.result = void 0) : e.then((e => {
-                                    Z(i, e, s, a, n)
-                                })).catch((e => D(e, n, t))).finally((() => r.result = void 0))
+                                let e = r(r, s).catch((e => tt(e, n, t)));
+                                r.finished ? (lt(i, r.result, s, a, n), r.result = void 0) : e.then((e => {
+                                    lt(i, e, s, a, n)
+                                })).catch((e => tt(e, n, t))).finally((() => r.result = void 0))
                             }
                         }
                     }(r, t, e);
-                return z.bind(null, e, t, i)
+                return et.bind(null, e, t, i)
             }
-            var U = {};
+            var st = {};
 
-            function Z(e, t, n, r, i) {
-                if (B && "function" == typeof t) {
+            function lt(e, t, n, r, i) {
+                if (nt && "function" == typeof t) {
                     let o = t.apply(n, r);
-                    o instanceof Promise ? o.then((t => Z(e, t, n, r))).catch((e => D(e, i, t))) : e(o)
+                    o instanceof Promise ? o.then((t => lt(e, t, n, r))).catch((e => tt(e, i, t))) : e(o)
                 } else "object" == typeof t && t instanceof Promise ? t.then((t => e(t))) : e(t)
             }
-            var K = "x-";
+            var ct = "x-";
 
-            function J(e = "") {
-                return K + e
+            function ut(e = "") {
+                return ct + e
             }
-            var Y = {};
+            var ft = {};
 
-            function X(e, t) {
-                return Y[e] = t, {
+            function dt(e, t) {
+                return ft[e] = t, {
                     before(t) {
-                        if (!Y[t]) return void console.warn("Cannot find directive `${directive}`. `${name}` will use the default order of execution");
-                        const n = fe.indexOf(t);
-                        fe.splice(n >= 0 ? n : fe.indexOf("DEFAULT"), 0, e)
+                        if (!ft[t]) return void console.warn("Cannot find directive `${directive}`. `${name}` will use the default order of execution");
+                        const n = Ot.indexOf(t);
+                        Ot.splice(n >= 0 ? n : Ot.indexOf("DEFAULT"), 0, e)
                     }
                 }
             }
 
-            function G(e, t, n) {
+            function pt(e, t, n) {
                 if (t = Array.from(t), e._x_virtualDirectives) {
                     let n = Object.entries(e._x_virtualDirectives).map((([e, t]) => ({
                             name: e,
                             value: t
                         }))),
-                        r = Q(n);
+                        r = _t(n);
                     n = n.map((e => r.find((t => t.name === e.name)) ? {
                         name: `x-bind:${e.name}`,
                         value: `"${e.value}"`
                     } : e)), t = t.concat(n)
                 }
                 let r = {},
-                    i = t.map(oe(((e, t) => r[e] = t))).filter(le).map(function(e, t) {
+                    i = t.map(xt(((e, t) => r[e] = t))).filter(Et).map(function(e, t) {
                         return ({
                             name: n,
                             value: r
                         }) => {
-                            let i = n.match(ce()),
+                            let i = n.match(St()),
                                 o = n.match(/:([a-zA-Z0-9\-:]+)/),
                                 a = n.match(/\.[^.\]]+(?=[^\]]*$)/g) || [],
                                 s = t || e[n] || n;
                             return {
                                 type: i ? i[1] : null,
                                 value: o ? o[1] : null,
                                 modifiers: a.map((e => e.replace(".", ""))),
                                 expression: r,
                                 original: s
                             }
                         }
-                    }(r, n)).sort(de);
+                    }(r, n)).sort(kt);
                 return i.map((t => function(e, t) {
-                    let n = Y[t.type] || (() => {}),
-                        [r, i] = re(e);
+                    let n = ft[t.type] || (() => {}),
+                        [r, i] = vt(e);
                     ! function(e, t, n) {
                         e._x_attributeCleanups || (e._x_attributeCleanups = {}), e._x_attributeCleanups[t] || (e._x_attributeCleanups[t] = []), e._x_attributeCleanups[t].push(n)
                     }(e, t.original, i);
                     let o = () => {
-                        e._x_ignore || e._x_ignoreSelf || (n.inline && n.inline(e, t, r), n = n.bind(n, e, t, r), ee ? te.get(ne).push(n) : n())
+                        e._x_ignore || e._x_ignoreSelf || (n.inline && n.inline(e, t, r), n = n.bind(n, e, t, r), ht ? mt.get(yt).push(n) : n())
                     };
                     return o.runCleanups = i, o
                 }(e, t)))
             }
 
-            function Q(e) {
-                return Array.from(e).map(oe()).filter((e => !le(e)))
+            function _t(e) {
+                return Array.from(e).map(xt()).filter((e => !Et(e)))
             }
-            var ee = !1,
-                te = new Map,
-                ne = Symbol();
-
-            function re(e) {
-                let n = [],
-                    [i, o] = function(e) {
-                        let n = () => {};
-                        return [i => {
-                            let o = t(i);
+            var ht = !1,
+                mt = new Map,
+                yt = Symbol();
+
+            function vt(e) {
+                let t = [],
+                    [n, r] = function(e) {
+                        let t = () => {};
+                        return [n => {
+                            let r = ve(n);
                             return e._x_effects || (e._x_effects = new Set, e._x_runEffects = () => {
                                 e._x_effects.forEach((e => e()))
-                            }), e._x_effects.add(o), n = () => {
-                                void 0 !== o && (e._x_effects.delete(o), r(o))
-                            }, o
+                            }), e._x_effects.add(r), t = () => {
+                                void 0 !== r && (e._x_effects.delete(r), ge(r))
+                            }, r
                         }, () => {
-                            n()
+                            t()
                         }]
                     }(e);
-                return n.push(o), [{
-                    Alpine: Xe,
-                    effect: i,
-                    cleanup: e => n.push(e),
-                    evaluateLater: H.bind(H, e),
-                    evaluate: F.bind(F, e)
-                }, () => n.forEach((e => e()))]
+                return t.push(r), [{
+                    Alpine: hn,
+                    effect: n,
+                    cleanup: e => t.push(e),
+                    evaluateLater: it.bind(it, e),
+                    evaluate: rt.bind(rt, e)
+                }, () => t.forEach((e => e()))]
             }
-            var ie = (e, t) => ({
+            var gt = (e, t) => ({
                 name: n,
                 value: r
             }) => (n.startsWith(e) && (n = n.replace(e, t)), {
                 name: n,
                 value: r
             });
 
-            function oe(e = (() => {})) {
+            function xt(e = (() => {})) {
                 return ({
                     name: t,
                     value: n
                 }) => {
                     let {
                         name: r,
                         value: i
-                    } = ae.reduce(((e, t) => t(e)), {
+                    } = bt.reduce(((e, t) => t(e)), {
                         name: t,
                         value: n
                     });
                     return r !== t && e(r, t), {
                         name: r,
                         value: i
                     }
                 }
             }
-            var ae = [];
+            var bt = [];
 
-            function se(e) {
-                ae.push(e)
+            function wt(e) {
+                bt.push(e)
             }
 
-            function le({
+            function Et({
                 name: e
             }) {
-                return ce().test(e)
+                return St().test(e)
             }
-            var ce = () => new RegExp(`^${K}([^:^.]+)\\b`),
-                ue = "DEFAULT",
-                fe = ["ignore", "ref", "data", "id", "bind", "init", "for", "model", "modelable", "transition", "show", "if", ue, "teleport"];
+            var St = () => new RegExp(`^${ct}([^:^.]+)\\b`),
+                At = "DEFAULT",
+                Ot = ["ignore", "ref", "data", "id", "bind", "init", "for", "model", "modelable", "transition", "show", "if", At, "teleport"];
 
-            function de(e, t) {
-                let n = -1 === fe.indexOf(e.type) ? ue : e.type,
-                    r = -1 === fe.indexOf(t.type) ? ue : t.type;
-                return fe.indexOf(n) - fe.indexOf(r)
+            function kt(e, t) {
+                let n = -1 === Ot.indexOf(e.type) ? At : e.type,
+                    r = -1 === Ot.indexOf(t.type) ? At : t.type;
+                return Ot.indexOf(n) - Ot.indexOf(r)
             }
 
-            function pe(e, t, n = {}) {
+            function Ct(e, t, n = {}) {
                 e.dispatchEvent(new CustomEvent(t, {
                     detail: n,
                     bubbles: !0,
                     composed: !0,
                     cancelable: !0
                 }))
             }
 
-            function _e(e, t) {
-                if ("function" == typeof ShadowRoot && e instanceof ShadowRoot) return void Array.from(e.children).forEach((e => _e(e, t)));
+            function jt(e, t) {
+                if ("function" == typeof ShadowRoot && e instanceof ShadowRoot) return void Array.from(e.children).forEach((e => jt(e, t)));
                 let n = !1;
                 if (t(e, (() => n = !0)), n) return;
                 let r = e.firstElementChild;
-                for (; r;) _e(r, t), r = r.nextElementSibling
+                for (; r;) jt(r, t), r = r.nextElementSibling
             }
 
-            function he(e, ...t) {
+            function Tt(e, ...t) {
                 console.warn(`Alpine Warning: ${e}`, ...t)
             }
-            var ye = [],
-                ve = [];
+            var Lt = !1,
+                Mt = [],
+                $t = [];
 
-            function me() {
-                return ye.map((e => e()))
+            function Nt() {
+                return Mt.map((e => e()))
             }
 
-            function ge() {
-                return ye.concat(ve).map((e => e()))
+            function Pt() {
+                return Mt.concat($t).map((e => e()))
             }
 
-            function xe(e) {
-                ye.push(e)
+            function Rt(e) {
+                Mt.push(e)
             }
 
-            function be(e) {
-                ve.push(e)
+            function qt(e) {
+                $t.push(e)
             }
 
-            function we(e, t = !1) {
-                return Ee(e, (e => {
-                    if ((t ? ge() : me()).some((t => e.matches(t)))) return !0
+            function It(e, t = !1) {
+                return zt(e, (e => {
+                    if ((t ? Pt() : Nt()).some((t => e.matches(t)))) return !0
                 }))
             }
 
-            function Ee(e, t) {
+            function zt(e, t) {
                 if (e) {
                     if (t(e)) return e;
-                    if (e._x_teleportBack && (e = e._x_teleportBack), e.parentElement) return Ee(e.parentElement, t)
+                    if (e._x_teleportBack && (e = e._x_teleportBack), e.parentElement) return zt(e.parentElement, t)
                 }
             }
-            var Se = [];
+            var Dt = [];
 
-            function Oe(e, t = _e, n = (() => {})) {
+            function Ft(e, t = jt, n = (() => {})) {
                 ! function(r) {
-                    ee = !0;
+                    ht = !0;
                     let i = Symbol();
-                    ne = i, te.set(i, []);
+                    yt = i, mt.set(i, []);
                     let o = () => {
-                        for (; te.get(i).length;) te.get(i).shift()();
-                        te.delete(i)
+                        for (; mt.get(i).length;) mt.get(i).shift()();
+                        mt.delete(i)
                     };
                     t(e, ((e, t) => {
-                        n(e, t), Se.forEach((n => n(e, t))), G(e, e.attributes).forEach((e => e())), e._x_ignore && t()
-                    })), ee = !1, o()
+                        n(e, t), Dt.forEach((n => n(e, t))), pt(e, e.attributes).forEach((e => e())), e._x_ignore && t()
+                    })), ht = !1, o()
                 }()
             }
 
-            function Ae(e) {
-                _e(e, (e => v(e)))
+            function Bt(e) {
+                jt(e, (e => $e(e)))
             }
-            var ke = [],
-                Ce = !1;
+            var Ht = [],
+                Wt = !1;
 
-            function je(e = (() => {})) {
+            function Vt(e = (() => {})) {
                 return queueMicrotask((() => {
-                    Ce || setTimeout((() => {
-                        Te()
+                    Wt || setTimeout((() => {
+                        Ut()
                     }))
                 })), new Promise((t => {
-                    ke.push((() => {
+                    Ht.push((() => {
                         e(), t()
                     }))
                 }))
             }
 
-            function Te() {
-                for (Ce = !1; ke.length;) ke.shift()()
+            function Ut() {
+                for (Wt = !1; Ht.length;) Ht.shift()()
             }
 
-            function Le(e, t) {
-                return Array.isArray(t) ? $e(e, t.join(" ")) : "object" == typeof t && null !== t ? function(e, t) {
+            function Zt(e, t) {
+                return Array.isArray(t) ? Kt(e, t.join(" ")) : "object" == typeof t && null !== t ? function(e, t) {
                     let n = e => e.split(" ").filter(Boolean),
                         r = Object.entries(t).flatMap((([e, t]) => !!t && n(e))).filter(Boolean),
                         i = Object.entries(t).flatMap((([e, t]) => !t && n(e))).filter(Boolean),
                         o = [],
                         a = [];
                     return i.forEach((t => {
                         e.classList.contains(t) && (e.classList.remove(t), a.push(t))
                     })), r.forEach((t => {
                         e.classList.contains(t) || (e.classList.add(t), o.push(t))
                     })), () => {
                         a.forEach((t => e.classList.add(t))), o.forEach((t => e.classList.remove(t)))
                     }
-                }(e, t) : "function" == typeof t ? Le(e, t()) : $e(e, t)
+                }(e, t) : "function" == typeof t ? Zt(e, t()) : Kt(e, t)
             }
 
-            function $e(e, t) {
+            function Kt(e, t) {
                 return t = !0 === t ? t = "" : t || "", n = t.split(" ").filter((t => !e.classList.contains(t))).filter(Boolean), e.classList.add(...n), () => {
                     e.classList.remove(...n)
                 };
                 var n
             }
 
-            function Me(e, t) {
+            function Jt(e, t) {
                 return "object" == typeof t && null !== t ? function(e, t) {
                     let n = {};
                     return Object.entries(t).forEach((([t, r]) => {
                         n[t] = e.style[t], t.startsWith("--") || (t = t.replace(/([a-z])([A-Z])/g, "$1-$2").toLowerCase()), e.style.setProperty(t, r)
                     })), setTimeout((() => {
                         0 === e.style.length && e.removeAttribute("style")
                     })), () => {
-                        Me(e, n)
+                        Jt(e, n)
                     }
                 }(e, t) : function(e, t) {
                     let n = e.getAttribute("style", t);
                     return e.setAttribute("style", t), () => {
                         e.setAttribute("style", n || "")
                     }
                 }(e, t)
             }
 
-            function Ne(e, t = (() => {})) {
+            function Xt(e, t = (() => {})) {
                 let n = !1;
                 return function() {
                     n ? t.apply(this, arguments) : (n = !0, e.apply(this, arguments))
                 }
             }
 
-            function Pe(e, t, n = {}) {
+            function Yt(e, t, n = {}) {
                 e._x_transition || (e._x_transition = {
                     enter: {
                         during: n,
                         start: n,
                         end: n
                     },
                     leave: {
                         during: n,
                         start: n,
                         end: n
                     },
                     in(n = (() => {}), r = (() => {})) {
-                        qe(e, t, {
+                        Qt(e, t, {
                             during: this.enter.during,
                             start: this.enter.start,
                             end: this.enter.end
                         }, n, r)
                     },
                     out(n = (() => {}), r = (() => {})) {
-                        qe(e, t, {
+                        Qt(e, t, {
                             during: this.leave.during,
                             start: this.leave.start,
                             end: this.leave.end
                         }, n, r)
                     }
                 })
             }
 
-            function Re(e) {
+            function Gt(e) {
                 let t = e.parentNode;
-                if (t) return t._x_hidePromise ? t : Re(t)
+                if (t) return t._x_hidePromise ? t : Gt(t)
             }
 
-            function qe(e, t, {
+            function Qt(e, t, {
                 during: n,
                 start: r,
                 end: i
             } = {}, o = (() => {}), a = (() => {})) {
                 if (e._x_transitioning && e._x_transitioning.cancel(), 0 === Object.keys(n).length && 0 === Object.keys(r).length && 0 === Object.keys(i).length) return o(), void a();
                 let s, l, c;
                 ! function(e, t) {
-                    let n, r, i, o = Ne((() => {
-                        S((() => {
-                            n = !0, r || t.before(), i || (t.end(), Te()), t.after(), e.isConnected && t.cleanup(), delete e._x_transitioning
+                    let n, r, i, o = Xt((() => {
+                        De((() => {
+                            n = !0, r || t.before(), i || (t.end(), Ut()), t.after(), e.isConnected && t.cleanup(), delete e._x_transitioning
                         }))
                     }));
                     e._x_transitioning = {
                         beforeCancels: [],
                         beforeCancel(e) {
                             this.beforeCancels.push(e)
                         },
-                        cancel: Ne((function() {
+                        cancel: Xt((function() {
                             for (; this.beforeCancels.length;) this.beforeCancels.shift()();
                             o()
                         })),
                         finish: o
-                    }, S((() => {
+                    }, De((() => {
                         t.start(), t.during()
-                    })), Ce = !0, requestAnimationFrame((() => {
+                    })), Wt = !0, requestAnimationFrame((() => {
                         if (n) return;
                         let o = 1e3 * Number(getComputedStyle(e).transitionDuration.replace(/,.*/, "").replace("s", "")),
                             a = 1e3 * Number(getComputedStyle(e).transitionDelay.replace(/,.*/, "").replace("s", ""));
-                        0 === o && (o = 1e3 * Number(getComputedStyle(e).animationDuration.replace("s", ""))), S((() => {
+                        0 === o && (o = 1e3 * Number(getComputedStyle(e).animationDuration.replace("s", ""))), De((() => {
                             t.before()
                         })), r = !0, requestAnimationFrame((() => {
-                            n || (S((() => {
+                            n || (De((() => {
                                 t.end()
-                            })), Te(), setTimeout(e._x_transitioning.finish, o + a), i = !0)
+                            })), Ut(), setTimeout(e._x_transitioning.finish, o + a), i = !0)
                         }))
                     }))
                 }(e, {
                     start() {
                         s = t(e, r)
                     },
                     during() {
@@ -1067,34 +1460,34 @@
                     after: a,
                     cleanup() {
                         l(), c()
                     }
                 })
             }
 
-            function Ie(e, t, n) {
+            function en(e, t, n) {
                 if (-1 === e.indexOf(t)) return n;
                 const r = e[e.indexOf(t) + 1];
                 if (!r) return n;
                 if ("scale" === t && isNaN(r)) return n;
-                if ("duration" === t) {
+                if ("duration" === t || "delay" === t) {
                     let e = r.match(/([0-9]+)ms/);
                     if (e) return e[1]
                 }
                 return "origin" === t && ["top", "right", "left", "center", "bottom"].includes(e[e.indexOf(t) + 2]) ? [r, e[e.indexOf(t) + 2]].join(" ") : r
             }
-            X("transition", ((e, {
+            dt("transition", ((e, {
                 value: t,
                 modifiers: n,
                 expression: r
             }, {
                 evaluate: i
             }) => {
-                "function" == typeof r && (r = i(r)), r ? function(e, t, n) {
-                    Pe(e, Le, ""), {
+                "function" == typeof r && (r = i(r)), !1 !== r && (r && "boolean" != typeof r ? function(e, t, n) {
+                    Yt(e, Zt, ""), {
                         enter: t => {
                             e._x_transition.enter.during = t
                         },
                         "enter-start": t => {
                             e._x_transition.enter.start = t
                         },
                         "enter-end": t => {
@@ -1107,873 +1500,469 @@
                             e._x_transition.leave.start = t
                         },
                         "leave-end": t => {
                             e._x_transition.leave.end = t
                         }
                     } [n](t)
                 }(e, r, t) : function(e, t, n) {
-                    Pe(e, Me);
+                    Yt(e, Jt);
                     let r = !t.includes("in") && !t.includes("out") && !n,
                         i = r || t.includes("in") || ["enter"].includes(n),
                         o = r || t.includes("out") || ["leave"].includes(n);
                     t.includes("in") && !r && (t = t.filter(((e, n) => n < t.indexOf("out")))), t.includes("out") && !r && (t = t.filter(((e, n) => n > t.indexOf("out"))));
                     let a = !t.includes("opacity") && !t.includes("scale"),
                         s = a || t.includes("opacity") ? 0 : 1,
-                        l = a || t.includes("scale") ? Ie(t, "scale", 95) / 100 : 1,
-                        c = Ie(t, "delay", 0),
-                        u = Ie(t, "origin", "center"),
+                        l = a || t.includes("scale") ? en(t, "scale", 95) / 100 : 1,
+                        c = en(t, "delay", 0) / 1e3,
+                        u = en(t, "origin", "center"),
                         f = "opacity, transform",
-                        d = Ie(t, "duration", 150) / 1e3,
-                        p = Ie(t, "duration", 75) / 1e3,
+                        d = en(t, "duration", 150) / 1e3,
+                        p = en(t, "duration", 75) / 1e3,
                         _ = "cubic-bezier(0.4, 0.0, 0.2, 1)";
                     i && (e._x_transition.enter.during = {
                         transformOrigin: u,
-                        transitionDelay: c,
+                        transitionDelay: `${c}s`,
                         transitionProperty: f,
                         transitionDuration: `${d}s`,
                         transitionTimingFunction: _
                     }, e._x_transition.enter.start = {
                         opacity: s,
                         transform: `scale(${l})`
                     }, e._x_transition.enter.end = {
                         opacity: 1,
                         transform: "scale(1)"
                     }), o && (e._x_transition.leave.during = {
                         transformOrigin: u,
-                        transitionDelay: c,
+                        transitionDelay: `${c}s`,
                         transitionProperty: f,
                         transitionDuration: `${p}s`,
                         transitionTimingFunction: _
                     }, e._x_transition.leave.start = {
                         opacity: 1,
                         transform: "scale(1)"
                     }, e._x_transition.leave.end = {
                         opacity: s,
                         transform: `scale(${l})`
                     })
-                }(e, n, t)
+                }(e, n, t))
             })), window.Element.prototype._x_toggleAndCascadeWithTransitions = function(e, t, n, r) {
                 const i = "visible" === document.visibilityState ? requestAnimationFrame : setTimeout;
                 let o = () => i(n);
                 t ? e._x_transition && (e._x_transition.enter || e._x_transition.leave) ? e._x_transition.enter && (Object.entries(e._x_transition.enter.during).length || Object.entries(e._x_transition.enter.start).length || Object.entries(e._x_transition.enter.end).length) ? e._x_transition.in(n) : o() : e._x_transition ? e._x_transition.in(n) : o() : (e._x_hidePromise = e._x_transition ? new Promise(((t, n) => {
                     e._x_transition.out((() => {}), (() => t(r))), e._x_transitioning.beforeCancel((() => n({
                         isFromCancelledTransition: !0
                     })))
                 })) : Promise.resolve(r), queueMicrotask((() => {
-                    let t = Re(e);
+                    let t = Gt(e);
                     t ? (t._x_hideChildren || (t._x_hideChildren = []), t._x_hideChildren.push(e)) : i((() => {
                         let t = e => {
                             let n = Promise.all([e._x_hidePromise, ...(e._x_hideChildren || []).map(t)]).then((([e]) => e()));
                             return delete e._x_hidePromise, delete e._x_hideChildren, n
                         };
                         t(e).catch((e => {
                             if (!e.isFromCancelledTransition) throw e
                         }))
                     }))
                 })))
             };
-            var ze = !1;
+            var tn = !1;
 
-            function De(e, t = (() => {})) {
-                return (...n) => ze ? t(...n) : e(...n)
+            function nn(e, t = (() => {})) {
+                return (...n) => tn ? t(...n) : e(...n)
             }
 
-            function Be(t, n, r, i = []) {
-                switch (t._x_bindings || (t._x_bindings = e({})), t._x_bindings[n] = r, n = i.includes("camel") ? n.toLowerCase().replace(/-(\w)/g, ((e, t) => t.toUpperCase())) : n) {
+            function rn(e, t, n, r = []) {
+                switch (e._x_bindings || (e._x_bindings = ye({})), e._x_bindings[t] = n, t = r.includes("camel") ? t.toLowerCase().replace(/-(\w)/g, ((e, t) => t.toUpperCase())) : t) {
                     case "value":
                         ! function(e, t) {
-                            if ("radio" === e.type) void 0 === e.attributes.value && (e.value = t), window.fromModel && (e.checked = Fe(e.value, t));
-                            else if ("checkbox" === e.type) Number.isInteger(t) ? e.value = t : Number.isInteger(t) || Array.isArray(t) || "boolean" == typeof t || [null, void 0].includes(t) ? Array.isArray(t) ? e.checked = t.some((t => Fe(t, e.value))) : e.checked = !!t : e.value = String(t);
+                            if ("radio" === e.type) void 0 === e.attributes.value && (e.value = t), window.fromModel && (e.checked = an(e.value, t));
+                            else if ("checkbox" === e.type) Number.isInteger(t) ? e.value = t : Number.isInteger(t) || Array.isArray(t) || "boolean" == typeof t || [null, void 0].includes(t) ? Array.isArray(t) ? e.checked = t.some((t => an(t, e.value))) : e.checked = !!t : e.value = String(t);
                             else if ("SELECT" === e.tagName) ! function(e, t) {
                                 const n = [].concat(t).map((e => e + ""));
                                 Array.from(e.options).forEach((e => {
                                     e.selected = n.includes(e.value)
                                 }))
                             }(e, t);
                             else {
                                 if (e.value === t) return;
                                 e.value = t
                             }
-                        }(t, r);
+                        }(e, n);
                         break;
                     case "style":
                         ! function(e, t) {
-                            e._x_undoAddedStyles && e._x_undoAddedStyles(), e._x_undoAddedStyles = Me(e, t)
-                        }(t, r);
+                            e._x_undoAddedStyles && e._x_undoAddedStyles(), e._x_undoAddedStyles = Jt(e, t)
+                        }(e, n);
                         break;
                     case "class":
                         ! function(e, t) {
-                            e._x_undoAddedClasses && e._x_undoAddedClasses(), e._x_undoAddedClasses = Le(e, t)
-                        }(t, r);
+                            e._x_undoAddedClasses && e._x_undoAddedClasses(), e._x_undoAddedClasses = Zt(e, t)
+                        }(e, n);
                         break;
-                    default:
+                    case "selected":
+                    case "checked":
                         ! function(e, t, n) {
-                            [null, void 0, !1].includes(n) && function(e) {
-                                return !["aria-pressed", "aria-checked", "aria-expanded", "aria-selected"].includes(e)
-                            }(t) ? e.removeAttribute(t) : (He(t) && (n = t), function(e, t, n) {
-                                e.getAttribute(t) != n && e.setAttribute(t, n)
-                            }(e, t, n))
-                        }(t, n, r)
+                            on(e, t, n),
+                                function(e, t, n) {
+                                    e[t] !== n && (e[t] = n)
+                                }(e, t, n)
+                        }(e, t, n);
+                        break;
+                    default:
+                        on(e, t, n)
                 }
             }
 
-            function Fe(e, t) {
+            function on(e, t, n) {
+                [null, void 0, !1].includes(n) && function(e) {
+                    return !["aria-pressed", "aria-checked", "aria-expanded", "aria-selected"].includes(e)
+                }(t) ? e.removeAttribute(t) : (sn(t) && (n = t), function(e, t, n) {
+                    e.getAttribute(t) != n && e.setAttribute(t, n)
+                }(e, t, n))
+            }
+
+            function an(e, t) {
                 return e == t
             }
 
-            function He(e) {
+            function sn(e) {
                 return ["disabled", "checked", "required", "readonly", "hidden", "open", "selected", "autofocus", "itemscope", "multiple", "novalidate", "allowfullscreen", "allowpaymentrequest", "formnovalidate", "autoplay", "controls", "loop", "muted", "playsinline", "default", "ismap", "reversed", "async", "defer", "nomodule"].includes(e)
             }
 
-            function We(e, t) {
+            function ln(e, t) {
                 var n;
                 return function() {
                     var r = this,
                         i = arguments;
                     clearTimeout(n), n = setTimeout((function() {
                         n = null, e.apply(r, i)
                     }), t)
                 }
             }
 
-            function Ve(e, t) {
+            function cn(e, t) {
                 let n;
                 return function() {
                     let r = arguments;
                     n || (e.apply(this, r), n = !0, setTimeout((() => n = !1), t))
                 }
             }
-            var Ue = {},
-                Ze = !1,
-                Ke = {};
+            var un = {},
+                fn = !1,
+                dn = {};
 
-            function Je(e, t, n) {
+            function pn(e, t, n) {
                 let r = [];
                 for (; r.length;) r.pop()();
                 let i = Object.entries(t).map((([e, t]) => ({
                         name: e,
                         value: t
                     }))),
-                    o = Q(i);
+                    o = _t(i);
                 i = i.map((e => o.find((t => t.name === e.name)) ? {
                     name: `x-bind:${e.name}`,
                     value: `"${e.value}"`
-                } : e)), G(e, i, n).map((e => {
+                } : e)), pt(e, i, n).map((e => {
                     r.push(e.runCleanups), e()
                 }))
             }
-            var Ye = {},
-                Xe = {
+            var _n = {},
+                hn = {
                     get reactive() {
-                        return e
+                        return ye
                     },
                     get release() {
-                        return r
+                        return ge
                     },
                     get effect() {
-                        return t
+                        return ve
                     },
                     get raw() {
-                        return i
+                        return xe
                     },
-                    version: "3.12.0",
+                    version: "3.12.1",
                     flushAndStopDeferringMutations: function() {
-                        O = !1, k(A), A = []
+                        Fe = !1, He(Be), Be = []
                     },
                     dontAutoEvaluateFunctions: function(e) {
-                        let t = B;
-                        B = !1, e(), B = t
+                        let t = nt;
+                        nt = !1, e(), nt = t
                     },
                     disableEffectScheduling: function(e) {
-                        f = !1, e(), f = !0
+                        ke = !1, e(), ke = !0
                     },
-                    startObservingMutations: x,
-                    stopObservingMutations: b,
-                    setReactivityEngine: function(n) {
-                        e = n.reactive, r = n.release, t = e => n.effect(e, {
+                    startObservingMutations: Re,
+                    stopObservingMutations: qe,
+                    setReactivityEngine: function(e) {
+                        ye = e.reactive, ge = e.release, ve = t => e.effect(t, {
                             scheduler: e => {
-                                f ? function(e) {
+                                ke ? function(e) {
                                     var t;
-                                    t = e, s.includes(t) || s.push(t), a || o || (o = !0, queueMicrotask(u))
+                                    t = e, Ee.includes(t) || Ee.push(t), we || be || (be = !0, queueMicrotask(Oe))
                                 }(e) : e()
                             }
-                        }), i = n.raw
+                        }), xe = e.raw
                     },
-                    closestDataStack: L,
-                    skipDuringClone: De,
+                    closestDataStack: Ue,
+                    skipDuringClone: nn,
                     onlyDuringClone: function(e) {
-                        return (...t) => ze && e(...t)
+                        return (...t) => tn && e(...t)
                     },
-                    addRootSelector: xe,
-                    addInitSelector: be,
-                    addScopeToNode: j,
+                    addRootSelector: Rt,
+                    addInitSelector: qt,
+                    addScopeToNode: Ve,
                     deferMutations: function() {
-                        O = !0
+                        Fe = !0
                     },
-                    mapAttributes: se,
-                    evaluateLater: H,
+                    mapAttributes: wt,
+                    evaluateLater: it,
                     interceptInit: function(e) {
-                        Se.push(e)
+                        Dt.push(e)
                     },
                     setEvaluator: function(e) {
-                        W = e
+                        ot = e
                     },
-                    mergeProxies: $,
-                    findClosest: Ee,
-                    closestRoot: we,
-                    destroyTree: Ae,
-                    interceptor: N,
-                    transition: qe,
-                    setStyles: Me,
-                    mutateDom: S,
-                    directive: X,
-                    throttle: Ve,
-                    debounce: We,
-                    evaluate: F,
-                    initTree: Oe,
-                    nextTick: je,
-                    prefixed: J,
+                    mergeProxies: Ze,
+                    findClosest: zt,
+                    closestRoot: It,
+                    destroyTree: Bt,
+                    interceptor: Je,
+                    transition: Qt,
+                    setStyles: Jt,
+                    mutateDom: De,
+                    directive: dt,
+                    throttle: cn,
+                    debounce: ln,
+                    evaluate: rt,
+                    initTree: Ft,
+                    nextTick: Vt,
+                    prefixed: ut,
                     prefix: function(e) {
-                        K = e
+                        ct = e
                     },
                     plugin: function(e) {
-                        e(Xe)
+                        (Array.isArray(e) ? e : [e]).forEach((e => e(hn)))
                     },
-                    magic: q,
-                    store: function(t, n) {
-                        if (Ze || (Ue = e(Ue), Ze = !0), void 0 === n) return Ue[t];
-                        Ue[t] = n, "object" == typeof n && null !== n && n.hasOwnProperty("init") && "function" == typeof n.init && Ue[t].init(), M(Ue[t])
+                    magic: Ge,
+                    store: function(e, t) {
+                        if (fn || (un = ye(un), fn = !0), void 0 === t) return un[e];
+                        un[e] = t, "object" == typeof t && null !== t && t.hasOwnProperty("init") && "function" == typeof t.init && un[e].init(), Ke(un[e])
                     },
                     start: function() {
                         var e;
-                        document.body || he("Unable to initialize. Trying to load Alpine before `<body>` is available. Did you forget to add `defer` in Alpine's `<script>` tag?"), pe(document, "alpine:init"), pe(document, "alpine:initializing"), x(), e = e => Oe(e, _e), h.push(e), y((e => Ae(e))), p.push(((e, t) => {
-                            G(e, t).forEach((e => e()))
-                        })), Array.from(document.querySelectorAll(ge())).filter((e => !we(e.parentElement, !0))).forEach((e => {
-                            Oe(e)
-                        })), pe(document, "alpine:initialized")
+                        Lt && Tt("Alpine has already been initialized on this page. Calling Alpine.start() more than once can cause problems."), Lt = !0, document.body || Tt("Unable to initialize. Trying to load Alpine before `<body>` is available. Did you forget to add `defer` in Alpine's `<script>` tag?"), Ct(document, "alpine:init"), Ct(document, "alpine:initializing"), Re(), e = e => Ft(e, jt), Le.push(e), Me((e => Bt(e))), je.push(((e, t) => {
+                            pt(e, t).forEach((e => e()))
+                        })), Array.from(document.querySelectorAll(Pt())).filter((e => !It(e.parentElement, !0))).forEach((e => {
+                            Ft(e)
+                        })), Ct(document, "alpine:initialized")
                     },
-                    clone: function(e, n) {
-                        n._x_dataStack || (n._x_dataStack = e._x_dataStack), ze = !0,
+                    clone: function(e, t) {
+                        t._x_dataStack || (t._x_dataStack = e._x_dataStack), tn = !0,
                             function(e) {
-                                let i = t;
-                                d(((e, t) => {
-                                        let n = i(e);
-                                        return r(n), () => {}
+                                let n = ve;
+                                Ce(((e, t) => {
+                                        let r = n(e);
+                                        return ge(r), () => {}
                                     })),
                                     function(e) {
                                         let t = !1;
-                                        Oe(e, ((e, n) => {
-                                            _e(e, ((e, r) => {
+                                        Ft(e, ((e, n) => {
+                                            jt(e, ((e, r) => {
                                                 if (t && function(e) {
-                                                        return me().some((t => e.matches(t)))
+                                                        return Nt().some((t => e.matches(t)))
                                                     }(e)) return r();
                                                 t = !0, n(e, r)
                                             }))
                                         }))
-                                    }(n), d(i)
-                            }(), ze = !1
+                                    }(t), Ce(n)
+                            }(), tn = !1
                     },
                     bound: function(e, t, n) {
                         if (e._x_bindings && void 0 !== e._x_bindings[t]) return e._x_bindings[t];
                         let r = e.getAttribute(t);
-                        return null === r ? "function" == typeof n ? n() : n : "" === r || (He(t) ? !![t, "true"].includes(r) : r)
+                        return null === r ? "function" == typeof n ? n() : n : "" === r || (sn(t) ? !![t, "true"].includes(r) : r)
                     },
-                    $data: C,
-                    walk: _e,
+                    $data: We,
+                    walk: jt,
                     data: function(e, t) {
-                        Ye[e] = t
+                        _n[e] = t
                     },
                     bind: function(e, t) {
                         let n = "function" != typeof t ? () => t : t;
-                        e instanceof Element ? Je(e, n()) : Ke[e] = n
+                        e instanceof Element ? pn(e, n()) : dn[e] = n
                     }
                 };
-
-            function Ge(e, t) {
-                const n = Object.create(null),
-                    r = e.split(",");
-                for (let e = 0; e < r.length; e++) n[r[e]] = !0;
-                return t ? e => !!n[e.toLowerCase()] : e => !!n[e]
-            }
-            var Qe, et = Object.freeze({}),
-                tt = (Object.freeze([]), Object.assign),
-                nt = Object.prototype.hasOwnProperty,
-                rt = (e, t) => nt.call(e, t),
-                it = Array.isArray,
-                ot = e => "[object Map]" === ct(e),
-                at = e => "symbol" == typeof e,
-                st = e => null !== e && "object" == typeof e,
-                lt = Object.prototype.toString,
-                ct = e => lt.call(e),
-                ut = e => ct(e).slice(8, -1),
-                ft = e => "string" == typeof e && "NaN" !== e && "-" !== e[0] && "" + parseInt(e, 10) === e,
-                dt = e => {
-                    const t = Object.create(null);
-                    return n => t[n] || (t[n] = e(n))
-                },
-                pt = /-(\w)/g,
-                _t = (dt((e => e.replace(pt, ((e, t) => t ? t.toUpperCase() : "")))), /\B([A-Z])/g),
-                ht = (dt((e => e.replace(_t, "-$1").toLowerCase())), dt((e => e.charAt(0).toUpperCase() + e.slice(1)))),
-                yt = (dt((e => e ? `on${ht(e)}` : "")), (e, t) => e !== t && (e == e || t == t)),
-                vt = new WeakMap,
-                mt = [],
-                gt = Symbol("iterate"),
-                xt = Symbol("Map key iterate"),
-                bt = 0;
-
-            function wt(e) {
-                const {
-                    deps: t
-                } = e;
-                if (t.length) {
-                    for (let n = 0; n < t.length; n++) t[n].delete(e);
-                    t.length = 0
-                }
-            }
-            var Et = !0,
-                St = [];
-
-            function Ot() {
-                const e = St.pop();
-                Et = void 0 === e || e
-            }
-
-            function At(e, t, n) {
-                if (!Et || void 0 === Qe) return;
-                let r = vt.get(e);
-                r || vt.set(e, r = new Map);
-                let i = r.get(n);
-                i || r.set(n, i = new Set), i.has(Qe) || (i.add(Qe), Qe.deps.push(i), Qe.options.onTrack && Qe.options.onTrack({
-                    effect: Qe,
-                    target: e,
-                    type: t,
-                    key: n
-                }))
-            }
-
-            function kt(e, t, n, r, i, o) {
-                const a = vt.get(e);
-                if (!a) return;
-                const s = new Set,
-                    l = e => {
-                        e && e.forEach((e => {
-                            (e !== Qe || e.allowRecurse) && s.add(e)
-                        }))
-                    };
-                if ("clear" === t) a.forEach(l);
-                else if ("length" === n && it(e)) a.forEach(((e, t) => {
-                    ("length" === t || t >= r) && l(e)
-                }));
-                else switch (void 0 !== n && l(a.get(n)), t) {
-                    case "add":
-                        it(e) ? ft(n) && l(a.get("length")) : (l(a.get(gt)), ot(e) && l(a.get(xt)));
-                        break;
-                    case "delete":
-                        it(e) || (l(a.get(gt)), ot(e) && l(a.get(xt)));
-                        break;
-                    case "set":
-                        ot(e) && l(a.get(gt))
-                }
-                s.forEach((a => {
-                    a.options.onTrigger && a.options.onTrigger({
-                        effect: a,
-                        target: e,
-                        key: n,
-                        type: t,
-                        newValue: r,
-                        oldValue: i,
-                        oldTarget: o
-                    }), a.options.scheduler ? a.options.scheduler(a) : a()
-                }))
-            }
-            var Ct = Ge("__proto__,__v_isRef,__isVue"),
-                jt = new Set(Object.getOwnPropertyNames(Symbol).map((e => Symbol[e])).filter(at)),
-                Tt = Pt(),
-                Lt = Pt(!1, !0),
-                $t = Pt(!0),
-                Mt = Pt(!0, !0),
-                Nt = {};
-
-            function Pt(e = !1, t = !1) {
-                return function(n, r, i) {
-                    if ("__v_isReactive" === r) return !e;
-                    if ("__v_isReadonly" === r) return e;
-                    if ("__v_raw" === r && i === (e ? t ? fn : un : t ? cn : ln).get(n)) return n;
-                    const o = it(n);
-                    if (!e && o && rt(Nt, r)) return Reflect.get(Nt, r, i);
-                    const a = Reflect.get(n, r, i);
-                    return (at(r) ? jt.has(r) : Ct(r)) ? a : (e || At(n, "get", r), t ? a : yn(a) ? o && ft(r) ? a : a.value : st(a) ? e ? pn(a) : dn(a) : a)
-                }
-            }
-
-            function Rt(e = !1) {
-                return function(t, n, r, i) {
-                    let o = t[n];
-                    if (!e && (r = hn(r), o = hn(o), !it(t) && yn(o) && !yn(r))) return o.value = r, !0;
-                    const a = it(t) && ft(n) ? Number(n) < t.length : rt(t, n),
-                        s = Reflect.set(t, n, r, i);
-                    return t === hn(i) && (a ? yt(r, o) && kt(t, "set", n, r, o) : kt(t, "add", n, r)), s
-                }
-            } ["includes", "indexOf", "lastIndexOf"].forEach((e => {
-                const t = Array.prototype[e];
-                Nt[e] = function(...e) {
-                    const n = hn(this);
-                    for (let e = 0, t = this.length; e < t; e++) At(n, "get", e + "");
-                    const r = t.apply(n, e);
-                    return -1 === r || !1 === r ? t.apply(n, e.map(hn)) : r
-                }
-            })), ["push", "pop", "shift", "unshift", "splice"].forEach((e => {
-                const t = Array.prototype[e];
-                Nt[e] = function(...e) {
-                    St.push(Et), Et = !1;
-                    const n = t.apply(this, e);
-                    return Ot(), n
-                }
-            }));
-            var qt = {
-                    get: Tt,
-                    set: Rt(),
-                    deleteProperty: function(e, t) {
-                        const n = rt(e, t),
-                            r = e[t],
-                            i = Reflect.deleteProperty(e, t);
-                        return i && n && kt(e, "delete", t, void 0, r), i
-                    },
-                    has: function(e, t) {
-                        const n = Reflect.has(e, t);
-                        return at(t) && jt.has(t) || At(e, "has", t), n
-                    },
-                    ownKeys: function(e) {
-                        return At(e, "iterate", it(e) ? "length" : gt), Reflect.ownKeys(e)
-                    }
-                },
-                It = {
-                    get: $t,
-                    set(e, t) {
-                        return console.warn(`Set operation on key "${String(t)}" failed: target is readonly.`, e), !0
-                    },
-                    deleteProperty(e, t) {
-                        return console.warn(`Delete operation on key "${String(t)}" failed: target is readonly.`, e), !0
-                    }
-                },
-                zt = (tt({}, qt, {
-                    get: Lt,
-                    set: Rt(!0)
-                }), tt({}, It, {
-                    get: Mt
-                }), e => st(e) ? dn(e) : e),
-                Dt = e => st(e) ? pn(e) : e,
-                Bt = e => e,
-                Ft = e => Reflect.getPrototypeOf(e);
-
-            function Ht(e, t, n = !1, r = !1) {
-                const i = hn(e = e.__v_raw),
-                    o = hn(t);
-                t !== o && !n && At(i, "get", t), !n && At(i, "get", o);
-                const {
-                    has: a
-                } = Ft(i), s = r ? Bt : n ? Dt : zt;
-                return a.call(i, t) ? s(e.get(t)) : a.call(i, o) ? s(e.get(o)) : void(e !== i && e.get(t))
-            }
-
-            function Wt(e, t = !1) {
-                const n = this.__v_raw,
-                    r = hn(n),
-                    i = hn(e);
-                return e !== i && !t && At(r, "has", e), !t && At(r, "has", i), e === i ? n.has(e) : n.has(e) || n.has(i)
-            }
-
-            function Vt(e, t = !1) {
-                return e = e.__v_raw, !t && At(hn(e), "iterate", gt), Reflect.get(e, "size", e)
-            }
-
-            function Ut(e) {
-                e = hn(e);
-                const t = hn(this);
-                return Ft(t).has.call(t, e) || (t.add(e), kt(t, "add", e, e)), this
-            }
-
-            function Zt(e, t) {
-                t = hn(t);
-                const n = hn(this),
-                    {
-                        has: r,
-                        get: i
-                    } = Ft(n);
-                let o = r.call(n, e);
-                o ? sn(n, r, e) : (e = hn(e), o = r.call(n, e));
-                const a = i.call(n, e);
-                return n.set(e, t), o ? yt(t, a) && kt(n, "set", e, t, a) : kt(n, "add", e, t), this
-            }
-
-            function Kt(e) {
-                const t = hn(this),
-                    {
-                        has: n,
-                        get: r
-                    } = Ft(t);
-                let i = n.call(t, e);
-                i ? sn(t, n, e) : (e = hn(e), i = n.call(t, e));
-                const o = r ? r.call(t, e) : void 0,
-                    a = t.delete(e);
-                return i && kt(t, "delete", e, void 0, o), a
-            }
-
-            function Jt() {
-                const e = hn(this),
-                    t = 0 !== e.size,
-                    n = ot(e) ? new Map(e) : new Set(e),
-                    r = e.clear();
-                return t && kt(e, "clear", void 0, void 0, n), r
-            }
-
-            function Yt(e, t) {
-                return function(n, r) {
-                    const i = this,
-                        o = i.__v_raw,
-                        a = hn(o),
-                        s = t ? Bt : e ? Dt : zt;
-                    return !e && At(a, "iterate", gt), o.forEach(((e, t) => n.call(r, s(e), s(t), i)))
-                }
-            }
-
-            function Xt(e, t, n) {
-                return function(...r) {
-                    const i = this.__v_raw,
-                        o = hn(i),
-                        a = ot(o),
-                        s = "entries" === e || e === Symbol.iterator && a,
-                        l = "keys" === e && a,
-                        c = i[e](...r),
-                        u = n ? Bt : t ? Dt : zt;
-                    return !t && At(o, "iterate", l ? xt : gt), {
-                        next() {
-                            const {
-                                value: e,
-                                done: t
-                            } = c.next();
-                            return t ? {
-                                value: e,
-                                done: t
-                            } : {
-                                value: s ? [u(e[0]), u(e[1])] : u(e),
-                                done: t
-                            }
-                        },
-                        [Symbol.iterator]() {
-                            return this
-                        }
-                    }
-                }
-            }
-
-            function Gt(e) {
-                return function(...t) {
-                    {
-                        const n = t[0] ? `on key "${t[0]}" ` : "";
-                        console.warn(`${ht(e)} operation ${n}failed: target is readonly.`, hn(this))
-                    }
-                    return "delete" !== e && this
-                }
-            }
-            var Qt = {
-                    get(e) {
-                        return Ht(this, e)
-                    },
-                    get size() {
-                        return Vt(this)
-                    },
-                    has: Wt,
-                    add: Ut,
-                    set: Zt,
-                    delete: Kt,
-                    clear: Jt,
-                    forEach: Yt(!1, !1)
-                },
-                en = {
-                    get(e) {
-                        return Ht(this, e, !1, !0)
-                    },
-                    get size() {
-                        return Vt(this)
-                    },
-                    has: Wt,
-                    add: Ut,
-                    set: Zt,
-                    delete: Kt,
-                    clear: Jt,
-                    forEach: Yt(!1, !0)
-                },
-                tn = {
-                    get(e) {
-                        return Ht(this, e, !0)
-                    },
-                    get size() {
-                        return Vt(this, !0)
-                    },
-                    has(e) {
-                        return Wt.call(this, e, !0)
-                    },
-                    add: Gt("add"),
-                    set: Gt("set"),
-                    delete: Gt("delete"),
-                    clear: Gt("clear"),
-                    forEach: Yt(!0, !1)
-                },
-                nn = {
-                    get(e) {
-                        return Ht(this, e, !0, !0)
-                    },
-                    get size() {
-                        return Vt(this, !0)
-                    },
-                    has(e) {
-                        return Wt.call(this, e, !0)
-                    },
-                    add: Gt("add"),
-                    set: Gt("set"),
-                    delete: Gt("delete"),
-                    clear: Gt("clear"),
-                    forEach: Yt(!0, !0)
-                };
-
-            function rn(e, t) {
-                const n = t ? e ? nn : en : e ? tn : Qt;
-                return (t, r, i) => "__v_isReactive" === r ? !e : "__v_isReadonly" === r ? e : "__v_raw" === r ? t : Reflect.get(rt(n, r) && r in t ? n : t, r, i)
-            } ["keys", "values", "entries", Symbol.iterator].forEach((e => {
-                Qt[e] = Xt(e, !1, !1), tn[e] = Xt(e, !0, !1), en[e] = Xt(e, !1, !0), nn[e] = Xt(e, !0, !0)
-            }));
-            var on = {
-                    get: rn(!1, !1)
-                },
-                an = (rn(!1, !0), {
-                    get: rn(!0, !1)
-                });
-
-            function sn(e, t, n) {
-                const r = hn(n);
-                if (r !== n && t.call(e, r)) {
-                    const t = ut(e);
-                    console.warn(`Reactive ${t} contains both the raw and reactive versions of the same object${"Map"===t?" as keys":""}, which can lead to inconsistencies. Avoid differentiating between the raw and reactive versions of an object and only use the reactive version if possible.`)
-                }
-            }
-            rn(!0, !0);
-            var ln = new WeakMap,
-                cn = new WeakMap,
-                un = new WeakMap,
-                fn = new WeakMap;
-
-            function dn(e) {
-                return e && e.__v_isReadonly ? e : _n(e, !1, qt, on, ln)
-            }
-
-            function pn(e) {
-                return _n(e, !0, It, an, un)
-            }
-
-            function _n(e, t, n, r, i) {
-                if (!st(e)) return console.warn(`value cannot be made reactive: ${String(e)}`), e;
-                if (e.__v_raw && (!t || !e.__v_isReactive)) return e;
-                const o = i.get(e);
-                if (o) return o;
-                const a = (s = e).__v_skip || !Object.isExtensible(s) ? 0 : function(e) {
-                    switch (e) {
-                        case "Object":
-                        case "Array":
-                            return 1;
-                        case "Map":
-                        case "Set":
-                        case "WeakMap":
-                        case "WeakSet":
-                            return 2;
-                        default:
-                            return 0
-                    }
-                }(ut(s));
-                var s;
-                if (0 === a) return e;
-                const l = new Proxy(e, 2 === a ? r : n);
-                return i.set(e, l), l
-            }
-
-            function hn(e) {
-                return e && hn(e.__v_raw) || e
-            }
-
-            function yn(e) {
-                return Boolean(e && !0 === e.__v_isRef)
-            }
-            q("nextTick", (() => je)), q("dispatch", (e => pe.bind(pe, e))), q("watch", ((e, {
+            Ge("nextTick", (() => Vt)), Ge("dispatch", (e => Ct.bind(Ct, e))), Ge("watch", ((e, {
                 evaluateLater: t,
                 effect: n
             }) => (r, i) => {
                 let o, a = t(r),
                     s = !0,
                     l = n((() => a((e => {
                         JSON.stringify(e), s ? o = e : queueMicrotask((() => {
                             i(e, o), o = e
                         })), s = !1
                     }))));
                 e._x_effects.delete(l)
-            })), q("store", (function() {
-                return Ue
-            })), q("data", (e => C(e))), q("root", (e => we(e))), q("refs", (e => (e._x_refs_proxy || (e._x_refs_proxy = $(function(e) {
+            })), Ge("store", (function() {
+                return un
+            })), Ge("data", (e => We(e))), Ge("root", (e => It(e))), Ge("refs", (e => (e._x_refs_proxy || (e._x_refs_proxy = Ze(function(e) {
                 let t = [],
                     n = e;
                 for (; n;) n._x_refs && t.push(n._x_refs), n = n.parentNode;
                 return t
             }(e))), e._x_refs_proxy)));
-            var vn = {};
+            var mn = {};
 
-            function mn(e) {
-                return vn[e] || (vn[e] = 0), ++vn[e]
+            function yn(e) {
+                return mn[e] || (mn[e] = 0), ++mn[e]
             }
 
-            function gn(e, t, n) {
-                q(t, (t => he(`You can't use [$${directiveName}] without first installing the "${e}" plugin here: https://alpinejs.dev/plugins/${n}`, t)))
+            function vn(e, t, n) {
+                Ge(t, (t => Tt(`You can't use [$${directiveName}] without first installing the "${e}" plugin here: https://alpinejs.dev/plugins/${n}`, t)))
             }
-            q("id", (e => (t, n = null) => {
+            Ge("id", (e => (t, n = null) => {
                 let r = function(e, t) {
-                        return Ee(e, (e => {
+                        return zt(e, (e => {
                             if (e._x_ids && e._x_ids[t]) return !0
                         }))
                     }(e, t),
-                    i = r ? r._x_ids[t] : mn(t);
+                    i = r ? r._x_ids[t] : yn(t);
                 return n ? `${t}-${i}-${n}` : `${t}-${i}`
-            })), q("el", (e => e)), gn("Focus", "focus", "focus"), gn("Persist", "persist", "persist"), X("modelable", ((e, {
-                expression: n
+            })), Ge("el", (e => e)), vn("Focus", "focus", "focus"), vn("Persist", "persist", "persist"), dt("modelable", ((e, {
+                expression: t
             }, {
-                effect: i,
-                evaluateLater: o,
-                cleanup: a
+                effect: n,
+                evaluateLater: r,
+                cleanup: i
             }) => {
-                let s = o(n),
-                    l = () => {
+                let o = r(t),
+                    a = () => {
                         let e;
-                        return s((t => e = t)), e
+                        return o((t => e = t)), e
                     },
-                    c = o(`${n} = __placeholder`),
-                    u = e => c((() => {}), {
+                    s = r(`${t} = __placeholder`),
+                    l = e => s((() => {}), {
                         scope: {
                             __placeholder: e
                         }
                     }),
-                    f = l();
-                u(f), queueMicrotask((() => {
+                    c = a();
+                l(c), queueMicrotask((() => {
                     if (!e._x_model) return;
                     e._x_removeModelListeners.default();
-                    let n = e._x_model.get,
-                        i = e._x_model.set,
-                        o = function({
+                    let t = e._x_model.get,
+                        n = e._x_model.set,
+                        r = function({
                             get: e,
-                            set: n
+                            set: t
                         }, {
-                            get: i,
-                            set: o
+                            get: n,
+                            set: r
                         }) {
-                            let a, s, l, c, u = !0,
-                                f = t((() => {
-                                    let t, r;
-                                    u ? (t = e(), o(t), r = i(), u = !1) : (t = e(), r = i(), l = JSON.stringify(t), c = JSON.stringify(r), l !== a ? (r = i(), o(t), r = t) : (n(r), t = r)), a = JSON.stringify(t), s = JSON.stringify(r)
+                            let i, o, a, s, l = !0,
+                                c = ve((() => {
+                                    let c, u;
+                                    l ? (c = e(), r(c), u = n(), l = !1) : (c = e(), u = n(), a = JSON.stringify(c), s = JSON.stringify(u), a !== i ? (u = n(), r(c), u = c) : (t(u), c = u)), i = JSON.stringify(c), o = JSON.stringify(u)
                                 }));
                             return () => {
-                                r(f)
+                                ge(c)
                             }
                         }({
                             get() {
-                                return n()
+                                return t()
                             },
                             set(e) {
-                                i(e)
+                                n(e)
                             }
                         }, {
                             get() {
-                                return l()
+                                return a()
                             },
                             set(e) {
-                                u(e)
+                                l(e)
                             }
                         });
-                    a(o)
+                    i(r)
                 }))
             }));
-            var xn = document.createElement("div");
-            X("teleport", ((e, {
+            var gn = document.createElement("div");
+            dt("teleport", ((e, {
                 modifiers: t,
                 expression: n
             }, {
                 cleanup: r
             }) => {
-                "template" !== e.tagName.toLowerCase() && he("x-teleport can only be used on a <template> tag", e);
-                let i = De((() => document.querySelector(n)), (() => xn))();
-                i || he(`Cannot find x-teleport element for selector: "${n}"`);
+                "template" !== e.tagName.toLowerCase() && Tt("x-teleport can only be used on a <template> tag", e);
+                let i = nn((() => document.querySelector(n)), (() => gn))();
+                i || Tt(`Cannot find x-teleport element for selector: "${n}"`);
                 let o = e.content.cloneNode(!0).firstElementChild;
                 e._x_teleport = o, o._x_teleportBack = e, e._x_forwardEvents && e._x_forwardEvents.forEach((t => {
                     o.addEventListener(t, (t => {
                         t.stopPropagation(), e.dispatchEvent(new t.constructor(t.type, t))
                     }))
-                })), j(o, {}, e), S((() => {
-                    t.includes("prepend") ? i.parentNode.insertBefore(o, i) : t.includes("append") ? i.parentNode.insertBefore(o, i.nextSibling) : i.appendChild(o), Oe(o), o._x_ignore = !0
+                })), Ve(o, {}, e), De((() => {
+                    t.includes("prepend") ? i.parentNode.insertBefore(o, i) : t.includes("append") ? i.parentNode.insertBefore(o, i.nextSibling) : i.appendChild(o), Ft(o), o._x_ignore = !0
                 })), r((() => o.remove()))
             }));
-            var bn = () => {};
+            var xn = () => {};
 
-            function wn(e, t, n, r) {
+            function bn(e, t, n, r) {
                 let i = e,
                     o = e => r(e),
                     a = {},
                     s = (e, t) => n => t(e, n);
-                if (n.includes("dot") && (t = t.replace(/-/g, ".")), n.includes("camel") && (t = t.toLowerCase().replace(/-(\w)/g, ((e, t) => t.toUpperCase()))), n.includes("passive") && (a.passive = !0), n.includes("capture") && (a.capture = !0), n.includes("window") && (i = window), n.includes("document") && (i = document), n.includes("prevent") && (o = s(o, ((e, t) => {
-                        t.preventDefault(), e(t)
-                    }))), n.includes("stop") && (o = s(o, ((e, t) => {
-                        t.stopPropagation(), e(t)
-                    }))), n.includes("self") && (o = s(o, ((t, n) => {
-                        n.target === e && t(n)
-                    }))), (n.includes("away") || n.includes("outside")) && (i = document, o = s(o, ((t, n) => {
-                        e.contains(n.target) || !1 !== n.target.isConnected && (e.offsetWidth < 1 && e.offsetHeight < 1 || !1 !== e._x_isShown && t(n))
-                    }))), n.includes("once") && (o = s(o, ((e, n) => {
-                        e(n), i.removeEventListener(t, o, a)
-                    }))), o = s(o, ((e, r) => {
-                        (function(e) {
-                            return ["keydown", "keyup"].includes(e)
-                        })(t) && function(e, t) {
-                            let n = t.filter((e => !["window", "document", "prevent", "stop", "once", "capture"].includes(e)));
-                            if (n.includes("debounce")) {
-                                let e = n.indexOf("debounce");
-                                n.splice(e, En((n[e + 1] || "invalid-wait").split("ms")[0]) ? 2 : 1)
-                            }
-                            if (n.includes("throttle")) {
-                                let e = n.indexOf("throttle");
-                                n.splice(e, En((n[e + 1] || "invalid-wait").split("ms")[0]) ? 2 : 1)
-                            }
-                            if (0 === n.length) return !1;
-                            if (1 === n.length && Sn(e.key).includes(n[0])) return !1;
-                            const r = ["ctrl", "shift", "alt", "meta", "cmd", "super"].filter((e => n.includes(e)));
-                            return n = n.filter((e => !r.includes(e))), !(r.length > 0 && r.filter((t => ("cmd" !== t && "super" !== t || (t = "meta"), e[`${t}Key`]))).length === r.length && Sn(e.key).includes(n[0]))
-                        }(r, n) || e(r)
-                    })), n.includes("debounce")) {
+                if (n.includes("dot") && (t = t.replace(/-/g, ".")), n.includes("camel") && (t = t.toLowerCase().replace(/-(\w)/g, ((e, t) => t.toUpperCase()))), n.includes("passive") && (a.passive = !0), n.includes("capture") && (a.capture = !0), n.includes("window") && (i = window), n.includes("document") && (i = document), n.includes("debounce")) {
                     let e = n[n.indexOf("debounce") + 1] || "invalid-wait",
-                        t = En(e.split("ms")[0]) ? Number(e.split("ms")[0]) : 250;
-                    o = We(o, t)
+                        t = wn(e.split("ms")[0]) ? Number(e.split("ms")[0]) : 250;
+                    o = ln(o, t)
                 }
                 if (n.includes("throttle")) {
                     let e = n[n.indexOf("throttle") + 1] || "invalid-wait",
-                        t = En(e.split("ms")[0]) ? Number(e.split("ms")[0]) : 250;
-                    o = Ve(o, t)
+                        t = wn(e.split("ms")[0]) ? Number(e.split("ms")[0]) : 250;
+                    o = cn(o, t)
                 }
-                return i.addEventListener(t, o, a), () => {
+                return n.includes("prevent") && (o = s(o, ((e, t) => {
+                    t.preventDefault(), e(t)
+                }))), n.includes("stop") && (o = s(o, ((e, t) => {
+                    t.stopPropagation(), e(t)
+                }))), n.includes("self") && (o = s(o, ((t, n) => {
+                    n.target === e && t(n)
+                }))), (n.includes("away") || n.includes("outside")) && (i = document, o = s(o, ((t, n) => {
+                    e.contains(n.target) || !1 !== n.target.isConnected && (e.offsetWidth < 1 && e.offsetHeight < 1 || !1 !== e._x_isShown && t(n))
+                }))), n.includes("once") && (o = s(o, ((e, n) => {
+                    e(n), i.removeEventListener(t, o, a)
+                }))), o = s(o, ((e, r) => {
+                    (function(e) {
+                        return ["keydown", "keyup"].includes(e)
+                    })(t) && function(e, t) {
+                        let n = t.filter((e => !["window", "document", "prevent", "stop", "once", "capture"].includes(e)));
+                        if (n.includes("debounce")) {
+                            let e = n.indexOf("debounce");
+                            n.splice(e, wn((n[e + 1] || "invalid-wait").split("ms")[0]) ? 2 : 1)
+                        }
+                        if (n.includes("throttle")) {
+                            let e = n.indexOf("throttle");
+                            n.splice(e, wn((n[e + 1] || "invalid-wait").split("ms")[0]) ? 2 : 1)
+                        }
+                        if (0 === n.length) return !1;
+                        if (1 === n.length && En(e.key).includes(n[0])) return !1;
+                        const r = ["ctrl", "shift", "alt", "meta", "cmd", "super"].filter((e => n.includes(e)));
+                        return n = n.filter((e => !r.includes(e))), !(r.length > 0 && r.filter((t => ("cmd" !== t && "super" !== t || (t = "meta"), e[`${t}Key`]))).length === r.length && En(e.key).includes(n[0]))
+                    }(r, n) || e(r)
+                })), i.addEventListener(t, o, a), () => {
                     i.removeEventListener(t, o, a)
                 }
             }
 
-            function En(e) {
+            function wn(e) {
                 return !Array.isArray(e) && !isNaN(e)
             }
 
-            function Sn(e) {
+            function En(e) {
                 if (!e) return [];
                 var t;
                 e = [" ", "_"].includes(t = e) ? t : t.replace(/([a-z])([A-Z])/g, "$1-$2").replace(/[_\s]/, "-").toLowerCase();
                 let n = {
                     ctrl: "control",
                     slash: "/",
                     space: " ",
@@ -1990,480 +1979,485 @@
                     underscore: "_"
                 };
                 return n[e] = e, Object.keys(n).map((t => {
                     if (n[t] === e) return t
                 })).filter((e => e))
             }
 
-            function On(e) {
+            function Sn(e) {
                 let t = e ? parseFloat(e) : null;
                 return n = t, Array.isArray(n) || isNaN(n) ? e : t;
                 var n
             }
 
             function An(e) {
                 return null !== e && "object" == typeof e && "function" == typeof e.get && "function" == typeof e.set
             }
 
-            function kn(e, t, n, r) {
+            function On(e, t, n, r) {
                 let i = {};
                 return /^\[.*\]$/.test(e.item) && Array.isArray(t) ? e.item.replace("[", "").replace("]", "").split(",").map((e => e.trim())).forEach(((e, n) => {
                     i[e] = t[n]
                 })) : /^\{.*\}$/.test(e.item) && !Array.isArray(t) && "object" == typeof t ? e.item.replace("{", "").replace("}", "").split(",").map((e => e.trim())).forEach((e => {
                     i[e] = t[e]
                 })) : i[e.item] = t, e.index && (i[e.index] = n), e.collection && (i[e.collection] = r), i
             }
 
-            function Cn() {}
+            function kn() {}
 
-            function jn(e, t, n) {
-                X(t, (r => he(`You can't use [x-${t}] without first installing the "${e}" plugin here: https://alpinejs.dev/plugins/${n}`, r)))
+            function Cn(e, t, n) {
+                dt(t, (r => Tt(`You can't use [x-${t}] without first installing the "${e}" plugin here: https://alpinejs.dev/plugins/${n}`, r)))
             }
-            bn.inline = (e, {
+            xn.inline = (e, {
                 modifiers: t
             }, {
                 cleanup: n
             }) => {
                 t.includes("self") ? e._x_ignoreSelf = !0 : e._x_ignore = !0, n((() => {
                     t.includes("self") ? delete e._x_ignoreSelf : delete e._x_ignore
                 }))
-            }, X("ignore", bn), X("effect", ((e, {
+            }, dt("ignore", xn), dt("effect", ((e, {
                 expression: t
             }, {
                 effect: n
-            }) => n(H(e, t)))), X("model", ((e, {
+            }) => n(it(e, t)))), dt("model", ((e, {
                 modifiers: t,
                 expression: n
             }, {
                 effect: r,
                 cleanup: i
             }) => {
                 let o = e;
                 t.includes("parent") && (o = e.parentNode);
-                let a, s = H(o, n);
-                a = "string" == typeof n ? H(o, `${n} = __placeholder`) : "function" == typeof n && "string" == typeof n() ? H(o, `${n()} = __placeholder`) : () => {};
+                let a, s = it(o, n);
+                a = "string" == typeof n ? it(o, `${n} = __placeholder`) : "function" == typeof n && "string" == typeof n() ? it(o, `${n()} = __placeholder`) : () => {};
                 let l = () => {
                         let e;
                         return s((t => e = t)), An(e) ? e.get() : e
                     },
                     c = e => {
                         let t;
                         s((e => t = e)), An(t) ? t.set(e) : a((() => {}), {
                             scope: {
                                 __placeholder: e
                             }
                         })
                     };
-                t.includes("fill") && e.hasAttribute("value") && (null === l() || "" === l()) && c(e.value), "string" == typeof n && "radio" === e.type && S((() => {
+                "string" == typeof n && "radio" === e.type && De((() => {
                     e.hasAttribute("name") || e.setAttribute("name", n)
                 }));
                 var u = "select" === e.tagName.toLowerCase() || ["checkbox", "radio"].includes(e.type) || t.includes("lazy") ? "change" : "input";
-                let f = ze ? () => {} : wn(e, u, t, (n => {
+                let f = tn ? () => {} : bn(e, u, t, (n => {
                     c(function(e, t, n, r) {
-                        return S((() => {
-                            if (n instanceof CustomEvent && void 0 !== n.detail) return void 0 !== n.detail ? n.detail : n.target.value;
+                        return De((() => {
+                            if (n instanceof CustomEvent && void 0 !== n.detail) return n.detail ?? n.target.value;
                             if ("checkbox" === e.type) {
                                 if (Array.isArray(r)) {
-                                    let e = t.includes("number") ? On(n.target.value) : n.target.value;
+                                    let e = t.includes("number") ? Sn(n.target.value) : n.target.value;
                                     return n.target.checked ? r.concat([e]) : r.filter((t => !(t == e)))
                                 }
                                 return n.target.checked
                             }
-                            if ("select" === e.tagName.toLowerCase() && e.multiple) return t.includes("number") ? Array.from(n.target.selectedOptions).map((e => On(e.value || e.text))) : Array.from(n.target.selectedOptions).map((e => e.value || e.text)); {
+                            if ("select" === e.tagName.toLowerCase() && e.multiple) return t.includes("number") ? Array.from(n.target.selectedOptions).map((e => Sn(e.value || e.text))) : Array.from(n.target.selectedOptions).map((e => e.value || e.text)); {
                                 let e = n.target.value;
-                                return t.includes("number") ? On(e) : t.includes("trim") ? e.trim() : e
+                                return t.includes("number") ? Sn(e) : t.includes("trim") ? e.trim() : e
                             }
                         }))
                     }(e, t, n, l()))
                 }));
-                if (e._x_removeModelListeners || (e._x_removeModelListeners = {}), e._x_removeModelListeners.default = f, i((() => e._x_removeModelListeners.default())), e.form) {
-                    let t = wn(e.form, "reset", [], (t => {
-                        je((() => e._x_model && e._x_model.set(e.value)))
+                if (t.includes("fill") && [null, ""].includes(l()) && e.dispatchEvent(new Event(u, {})), e._x_removeModelListeners || (e._x_removeModelListeners = {}), e._x_removeModelListeners.default = f, i((() => e._x_removeModelListeners.default())), e.form) {
+                    let t = bn(e.form, "reset", [], (t => {
+                        Vt((() => e._x_model && e._x_model.set(e.value)))
                     }));
                     i((() => t()))
                 }
                 e._x_model = {
                     get() {
                         return l()
                     },
                     set(e) {
                         c(e)
                     }
                 }, e._x_forceModelUpdate = t => {
-                    void 0 === (t = void 0 === t ? l() : t) && "string" == typeof n && n.match(/\./) && (t = ""), window.fromModel = !0, S((() => Be(e, "value", t))), delete window.fromModel
+                    void 0 === (t = void 0 === t ? l() : t) && "string" == typeof n && n.match(/\./) && (t = ""), window.fromModel = !0, De((() => rn(e, "value", t))), delete window.fromModel
                 }, r((() => {
                     let n = l();
                     t.includes("unintrusive") && document.activeElement.isSameNode(e) || e._x_forceModelUpdate(n)
                 }))
-            })), X("cloak", (e => queueMicrotask((() => S((() => e.removeAttribute(J("cloak")))))))), be((() => `[${J("init")}]`)), X("init", De(((e, {
+            })), dt("cloak", (e => queueMicrotask((() => De((() => e.removeAttribute(ut("cloak")))))))), qt((() => `[${ut("init")}]`)), dt("init", nn(((e, {
                 expression: t
             }, {
                 evaluate: n
-            }) => "string" == typeof t ? !!t.trim() && n(t, {}, !1) : n(t, {}, !1)))), X("text", ((e, {
+            }) => "string" == typeof t ? !!t.trim() && n(t, {}, !1) : n(t, {}, !1)))), dt("text", ((e, {
                 expression: t
             }, {
                 effect: n,
                 evaluateLater: r
             }) => {
                 let i = r(t);
                 n((() => {
                     i((t => {
-                        S((() => {
+                        De((() => {
                             e.textContent = t
                         }))
                     }))
                 }))
-            })), X("html", ((e, {
+            })), dt("html", ((e, {
                 expression: t
             }, {
                 effect: n,
                 evaluateLater: r
             }) => {
                 let i = r(t);
                 n((() => {
                     i((t => {
-                        S((() => {
-                            e.innerHTML = t, e._x_ignoreSelf = !0, Oe(e), delete e._x_ignoreSelf
+                        De((() => {
+                            e.innerHTML = t, e._x_ignoreSelf = !0, Ft(e), delete e._x_ignoreSelf
                         }))
                     }))
                 }))
-            })), se(ie(":", J("bind:"))), X("bind", ((e, {
+            })), wt(gt(":", ut("bind:"))), dt("bind", ((e, {
                 value: t,
                 modifiers: n,
                 expression: r,
                 original: i
             }, {
                 effect: o
             }) => {
                 if (!t) {
                     let t = {};
-                    return a = t, Object.entries(Ke).forEach((([e, t]) => {
+                    return a = t, Object.entries(dn).forEach((([e, t]) => {
                         Object.defineProperty(a, e, {
                             get() {
                                 return (...e) => t(...e)
                             }
                         })
-                    })), void H(e, r)((t => {
-                        Je(e, t, i)
+                    })), void it(e, r)((t => {
+                        pn(e, t, i)
                     }), {
                         scope: t
                     })
                 }
                 var a;
                 if ("key" === t) return function(e, t) {
                     e._x_keyExpression = t
                 }(e, r);
-                let s = H(e, r);
+                let s = it(e, r);
                 o((() => s((i => {
-                    void 0 === i && "string" == typeof r && r.match(/\./) && (i = ""), S((() => Be(e, t, i, n)))
+                    void 0 === i && "string" == typeof r && r.match(/\./) && (i = ""), De((() => rn(e, t, i, n)))
                 }))))
-            })), xe((() => `[${J("data")}]`)), X("data", De(((t, {
-                expression: n
+            })), Rt((() => `[${ut("data")}]`)), dt("data", nn(((e, {
+                expression: t
             }, {
-                cleanup: r
+                cleanup: n
             }) => {
-                n = "" === n ? "{}" : n;
+                t = "" === t ? "{}" : t;
+                let r = {};
+                Qe(r, e);
                 let i = {};
-                I(i, t);
-                let o = {};
-                var a, s;
-                a = o, s = i, Object.entries(Ye).forEach((([e, t]) => {
-                    Object.defineProperty(a, e, {
+                var o, a;
+                o = i, a = r, Object.entries(_n).forEach((([e, t]) => {
+                    Object.defineProperty(o, e, {
                         get() {
-                            return (...e) => t.bind(s)(...e)
+                            return (...e) => t.bind(a)(...e)
                         },
                         enumerable: !1
                     })
                 }));
-                let l = F(t, n, {
-                    scope: o
+                let s = rt(e, t, {
+                    scope: i
                 });
-                void 0 !== l && !0 !== l || (l = {}), I(l, t);
-                let c = e(l);
-                M(c);
-                let u = j(t, c);
-                c.init && F(t, c.init), r((() => {
-                    c.destroy && F(t, c.destroy), u()
+                void 0 !== s && !0 !== s || (s = {}), Qe(s, e);
+                let l = ye(s);
+                Ke(l);
+                let c = Ve(e, l);
+                l.init && rt(e, l.init), n((() => {
+                    l.destroy && rt(e, l.destroy), c()
                 }))
-            }))), X("show", ((e, {
+            }))), dt("show", ((e, {
                 modifiers: t,
                 expression: n
             }, {
                 effect: r
             }) => {
-                let i = H(e, n);
+                let i = it(e, n);
                 e._x_doHide || (e._x_doHide = () => {
-                    S((() => {
+                    De((() => {
                         e.style.setProperty("display", "none", t.includes("important") ? "important" : void 0)
                     }))
                 }), e._x_doShow || (e._x_doShow = () => {
-                    S((() => {
+                    De((() => {
                         1 === e.style.length && "none" === e.style.display ? e.removeAttribute("style") : e.style.removeProperty("display")
                     }))
                 });
                 let o, a = () => {
                         e._x_doHide(), e._x_isShown = !1
                     },
                     s = () => {
                         e._x_doShow(), e._x_isShown = !0
                     },
                     l = () => setTimeout(s),
-                    c = Ne((e => e ? s() : a()), (t => {
+                    c = Xt((e => e ? s() : a()), (t => {
                         "function" == typeof e._x_toggleAndCascadeWithTransitions ? e._x_toggleAndCascadeWithTransitions(e, t, s, a) : t ? l() : a()
                     })),
                     u = !0;
                 r((() => i((e => {
                     (u || e !== o) && (t.includes("immediate") && (e ? l() : a()), c(e), o = e, u = !1)
                 }))))
-            })), X("for", ((t, {
-                expression: n
+            })), dt("for", ((e, {
+                expression: t
             }, {
-                effect: r,
-                cleanup: i
+                effect: n,
+                cleanup: r
             }) => {
-                let o = function(e) {
+                let i = function(e) {
                         let t = /,([^,\}\]]*)(?:,([^,\}\]]*))?$/,
                             n = e.match(/([\s\S]*?)\s+(?:in|of)\s+([\s\S]*)/);
                         if (!n) return;
                         let r = {};
                         r.items = n[2].trim();
                         let i = n[1].replace(/^\s*\(|\)\s*$/g, "").trim(),
                             o = i.match(t);
                         return o ? (r.item = i.replace(t, "").trim(), r.index = o[1].trim(), o[2] && (r.collection = o[2].trim())) : r.item = i, r
-                    }(n),
-                    a = H(t, o.items),
-                    s = H(t, t._x_keyExpression || "index");
-                t._x_prevKeys = [], t._x_lookup = {}, r((() => function(t, n, r, i) {
-                    let o = t;
-                    r((r => {
-                        var a;
-                        a = r, !Array.isArray(a) && !isNaN(a) && r >= 0 && (r = Array.from(Array(r).keys(), (e => e + 1))), void 0 === r && (r = []);
-                        let s = t._x_lookup,
-                            l = t._x_prevKeys,
-                            u = [],
-                            f = [];
-                        if ("object" != typeof(d = r) || Array.isArray(d))
-                            for (let e = 0; e < r.length; e++) {
-                                let t = kn(n, r[e], e, r);
-                                i((e => f.push(e)), {
+                    }(t),
+                    o = it(e, i.items),
+                    a = it(e, e._x_keyExpression || "index");
+                e._x_prevKeys = [], e._x_lookup = {}, n((() => function(e, t, n, r) {
+                    let i = e;
+                    n((n => {
+                        var o;
+                        o = n, !Array.isArray(o) && !isNaN(o) && n >= 0 && (n = Array.from(Array(n).keys(), (e => e + 1))), void 0 === n && (n = []);
+                        let a = e._x_lookup,
+                            s = e._x_prevKeys,
+                            l = [],
+                            c = [];
+                        if ("object" != typeof(u = n) || Array.isArray(u))
+                            for (let e = 0; e < n.length; e++) {
+                                let i = On(t, n[e], e, n);
+                                r((e => c.push(e)), {
                                     scope: {
                                         index: e,
-                                        ...t
+                                        ...i
                                     }
-                                }), u.push(t)
-                            } else r = Object.entries(r).map((([e, t]) => {
-                                let o = kn(n, t, e, r);
-                                i((e => f.push(e)), {
+                                }), l.push(i)
+                            } else n = Object.entries(n).map((([e, i]) => {
+                                let o = On(t, i, e, n);
+                                r((e => c.push(e)), {
                                     scope: {
                                         index: e,
                                         ...o
                                     }
-                                }), u.push(o)
+                                }), l.push(o)
                             }));
-                        var d;
-                        let p = [],
-                            _ = [],
-                            h = [],
-                            y = [];
-                        for (let e = 0; e < l.length; e++) {
-                            let t = l[e]; - 1 === f.indexOf(t) && h.push(t)
+                        var u;
+                        let f = [],
+                            d = [],
+                            p = [],
+                            _ = [];
+                        for (let e = 0; e < s.length; e++) {
+                            let t = s[e]; - 1 === c.indexOf(t) && p.push(t)
                         }
-                        l = l.filter((e => !h.includes(e)));
-                        let v = "template";
-                        for (let e = 0; e < f.length; e++) {
-                            let t = f[e],
-                                n = l.indexOf(t);
-                            if (-1 === n) l.splice(e, 0, t), p.push([v, e]);
+                        s = s.filter((e => !p.includes(e)));
+                        let h = "template";
+                        for (let e = 0; e < c.length; e++) {
+                            let t = c[e],
+                                n = s.indexOf(t);
+                            if (-1 === n) s.splice(e, 0, t), f.push([h, e]);
                             else if (n !== e) {
-                                let t = l.splice(e, 1)[0],
-                                    r = l.splice(n - 1, 1)[0];
-                                l.splice(e, 0, r), l.splice(n, 0, t), _.push([t, r])
-                            } else y.push(t);
-                            v = t
+                                let t = s.splice(e, 1)[0],
+                                    r = s.splice(n - 1, 1)[0];
+                                s.splice(e, 0, r), s.splice(n, 0, t), d.push([t, r])
+                            } else _.push(t);
+                            h = t
                         }
-                        for (let e = 0; e < h.length; e++) {
-                            let t = h[e];
-                            s[t]._x_effects && s[t]._x_effects.forEach(c), s[t].remove(), s[t] = null, delete s[t]
+                        for (let e = 0; e < p.length; e++) {
+                            let t = p[e];
+                            a[t]._x_effects && a[t]._x_effects.forEach(Ae), a[t].remove(), a[t] = null, delete a[t]
                         }
-                        for (let e = 0; e < _.length; e++) {
-                            let [t, n] = _[e], r = s[t], i = s[n], o = document.createElement("div");
-                            S((() => {
-                                i.after(o), r.after(i), i._x_currentIfEl && i.after(i._x_currentIfEl), o.before(r), r._x_currentIfEl && r.after(r._x_currentIfEl), o.remove()
-                            })), T(i, u[f.indexOf(n)])
+                        for (let e = 0; e < d.length; e++) {
+                            let [t, n] = d[e], r = a[t], o = a[n], s = document.createElement("div");
+                            De((() => {
+                                o || Tt('x-for ":key" is undefined or invalid', i), o.after(s), r.after(o), o._x_currentIfEl && o.after(o._x_currentIfEl), s.before(r), r._x_currentIfEl && r.after(r._x_currentIfEl), s.remove()
+                            })), o._x_refreshXForScope(l[c.indexOf(n)])
                         }
-                        for (let t = 0; t < p.length; t++) {
-                            let [n, r] = p[t], i = "template" === n ? o : s[n];
-                            i._x_currentIfEl && (i = i._x_currentIfEl);
-                            let a = u[r],
-                                l = f[r],
-                                c = document.importNode(o.content, !0).firstElementChild;
-                            j(c, e(a), o), S((() => {
-                                i.after(c), Oe(c)
-                            })), "object" == typeof l && he("x-for key cannot be an object, it must be a string or an integer", o), s[l] = c
+                        for (let e = 0; e < f.length; e++) {
+                            let [t, n] = f[e], r = "template" === t ? i : a[t];
+                            r._x_currentIfEl && (r = r._x_currentIfEl);
+                            let o = l[n],
+                                s = c[n],
+                                u = document.importNode(i.content, !0).firstElementChild,
+                                d = ye(o);
+                            Ve(u, d, i), u._x_refreshXForScope = e => {
+                                Object.entries(e).forEach((([e, t]) => {
+                                    d[e] = t
+                                }))
+                            }, De((() => {
+                                r.after(u), Ft(u)
+                            })), "object" == typeof s && Tt("x-for key cannot be an object, it must be a string or an integer", i), a[s] = u
                         }
-                        for (let e = 0; e < y.length; e++) T(s[y[e]], u[f.indexOf(y[e])]);
-                        o._x_prevKeys = f
+                        for (let e = 0; e < _.length; e++) a[_[e]]._x_refreshXForScope(l[c.indexOf(_[e])]);
+                        i._x_prevKeys = c
                     }))
-                }(t, o, a, s))), i((() => {
-                    Object.values(t._x_lookup).forEach((e => e.remove())), delete t._x_prevKeys, delete t._x_lookup
+                }(e, i, o, a))), r((() => {
+                    Object.values(e._x_lookup).forEach((e => e.remove())), delete e._x_prevKeys, delete e._x_lookup
                 }))
-            })), Cn.inline = (e, {
+            })), kn.inline = (e, {
                 expression: t
             }, {
                 cleanup: n
             }) => {
-                let r = we(e);
+                let r = It(e);
                 r._x_refs || (r._x_refs = {}), r._x_refs[t] = e, n((() => delete r._x_refs[t]))
-            }, X("ref", Cn), X("if", ((e, {
+            }, dt("ref", kn), dt("if", ((e, {
                 expression: t
             }, {
                 effect: n,
                 cleanup: r
             }) => {
-                let i = H(e, t);
+                let i = it(e, t);
                 n((() => i((t => {
                     t ? (() => {
                         if (e._x_currentIfEl) return e._x_currentIfEl;
                         let t = e.content.cloneNode(!0).firstElementChild;
-                        j(t, {}, e), S((() => {
-                            e.after(t), Oe(t)
+                        Ve(t, {}, e), De((() => {
+                            e.after(t), Ft(t)
                         })), e._x_currentIfEl = t, e._x_undoIf = () => {
-                            _e(t, (e => {
-                                e._x_effects && e._x_effects.forEach(c)
+                            jt(t, (e => {
+                                e._x_effects && e._x_effects.forEach(Ae)
                             })), t.remove(), delete e._x_currentIfEl
                         }
                     })() : e._x_undoIf && (e._x_undoIf(), delete e._x_undoIf)
                 })))), r((() => e._x_undoIf && e._x_undoIf()))
-            })), X("id", ((e, {
+            })), dt("id", ((e, {
                 expression: t
             }, {
                 evaluate: n
             }) => {
                 n(t).forEach((t => function(e, t) {
-                    e._x_ids || (e._x_ids = {}), e._x_ids[t] || (e._x_ids[t] = mn(t))
+                    e._x_ids || (e._x_ids = {}), e._x_ids[t] || (e._x_ids[t] = yn(t))
                 }(e, t)))
-            })), se(ie("@", J("on:"))), X("on", De(((e, {
+            })), wt(gt("@", ut("on:"))), dt("on", nn(((e, {
                 value: t,
                 modifiers: n,
                 expression: r
             }, {
                 cleanup: i
             }) => {
-                let o = r ? H(e, r) : () => {};
+                let o = r ? it(e, r) : () => {};
                 "template" === e.tagName.toLowerCase() && (e._x_forwardEvents || (e._x_forwardEvents = []), e._x_forwardEvents.includes(t) || e._x_forwardEvents.push(t));
-                let a = wn(e, t, n, (e => {
+                let a = bn(e, t, n, (e => {
                     o((() => {}), {
                         scope: {
                             $event: e
                         },
                         params: [e]
                     })
                 }));
                 i((() => a()))
-            }))), jn("Collapse", "collapse", "collapse"), jn("Intersect", "intersect", "intersect"), jn("Focus", "trap", "focus"), jn("Mask", "mask", "mask"), Xe.setEvaluator(V), Xe.setReactivityEngine({
-                reactive: dn,
-                effect: function(e, t = et) {
+            }))), Cn("Collapse", "collapse", "collapse"), Cn("Intersect", "intersect", "intersect"), Cn("Focus", "trap", "focus"), Cn("Mask", "mask", "mask"), hn.setEvaluator(at), hn.setReactivityEngine({
+                reactive: de,
+                effect: function(e, n = t) {
                     (function(e) {
                         return e && !0 === e._isEffect
                     })(e) && (e = e.raw);
-                    const n = function(e, t) {
+                    const r = function(e, t) {
                         const n = function() {
                             if (!n.active) return e();
-                            if (!mt.includes(n)) {
-                                wt(n);
+                            if (!g.includes(n)) {
+                                S(n);
                                 try {
-                                    return St.push(Et), Et = !0, mt.push(n), Qe = n, e()
+                                    return O.push(A), A = !0, g.push(n), x = n, e()
                                 } finally {
-                                    mt.pop(), Ot(), Qe = mt[mt.length - 1]
+                                    g.pop(), k(), x = g[g.length - 1]
                                 }
                             }
                         };
-                        return n.id = bt++, n.allowRecurse = !!t.allowRecurse, n._isEffect = !0, n.active = !0, n.raw = e, n.deps = [], n.options = t, n
-                    }(e, t);
-                    return t.lazy || n(), n
+                        return n.id = E++, n.allowRecurse = !!t.allowRecurse, n._isEffect = !0, n.active = !0, n.raw = e, n.deps = [], n.options = t, n
+                    }(e, n);
+                    return n.lazy || r(), r
                 },
                 release: function(e) {
-                    e.active && (wt(e), e.options.onStop && e.options.onStop(), e.active = !1)
+                    e.active && (S(e), e.options.onStop && e.options.onStop(), e.active = !1)
                 },
-                raw: hn
+                raw: he
             });
-            var Tn = Xe;
+            var jn = hn;
 
-            function Ln(e) {
+            function Tn(e) {
                 if (e.includes("full")) return .99;
                 if (e.includes("half")) return .5;
                 if (!e.includes("threshold")) return 0;
                 let t = e[e.indexOf("threshold") + 1];
                 return "100" === t ? 1 : "0" === t ? 0 : Number(`.${t}`)
             }
 
-            function $n(e) {
+            function Ln(e) {
                 let t = e.match(/^(-?[0-9]+)(px|%)?$/);
                 return t ? t[1] + (t[2] || "px") : void 0
             }
 
             function Mn(e) {
                 const t = "0px 0px 0px 0px",
                     n = e.indexOf("margin");
                 if (-1 === n) return t;
                 let r = [];
-                for (let t = 1; t < 5; t++) r.push($n(e[n + t] || ""));
+                for (let t = 1; t < 5; t++) r.push(Ln(e[n + t] || ""));
                 return r = r.filter((e => void 0 !== e)), r.length ? r.join(" ").trim() : t
             }
-            var Nn = n(152),
-                Pn = n.n(Nn);
+            var $n = n(13),
+                Nn = n.n($n);
 
-            function Rn(e, t) {
+            function Pn(e, t) {
                 e.classList.remove("scale-100"), t.classList.add("scale-100"), e.classList.add("scale-0"), t.classList.remove("scale-0")
             }
-            window.Alpine = Tn, Tn.plugin((function(e) {
+            window.Alpine = jn, jn.plugin((function(e) {
                 e.directive("intersect", ((e, {
                     value: t,
                     expression: n,
                     modifiers: r
                 }, {
                     evaluateLater: i,
                     cleanup: o
                 }) => {
                     let a = i(n),
                         s = {
                             rootMargin: Mn(r),
-                            threshold: Ln(r)
+                            threshold: Tn(r)
                         },
                         l = new IntersectionObserver((e => {
                             e.forEach((e => {
                                 e.isIntersecting !== ("leave" === t) && (a(), r.includes("once") && l.disconnect())
                             }))
                         }), s);
                     l.observe(e), o((() => {
                         l.disconnect()
                     }))
                 }))
-            })), Tn.start(), window.addEventListener("DOMContentLoaded", (() => {
+            })), jn.start(), window.addEventListener("DOMContentLoaded", (() => {
                 ! function() {
                     const e = document.querySelectorAll(".highlight");
                     if (!e) return;
                     e.forEach((e => {
                         const t = e.querySelector("pre");
                         if (t) {
                             const e = '<button class="copy z-20 inline-flex h-6 w-6 items-center justify-center rounded-md border border-border bg-background opacity-0 focus:opacity-100 text-sm font-medium transition-all hover:bg-muted absolute right-4 top-4 tooltipped tooltipped-n" data-tooltip="Copy code" type="button"><span class="sr-only">Copy code</span><svg xmlns="http://www.w3.org/2000/svg" height="24" width="24" viewBox="0 96 960 960" fill="currentColor" stroke="none" class="copy-icon h-[14px] w-[14px] transition-all transform scale-100 absolute"><path d="M200 976q-33 0-56.5-23.5T120 896V376q0-17 11.5-28.5T160 336q17 0 28.5 11.5T200 376v520h400q17 0 28.5 11.5T640 936q0 17-11.5 28.5T600 976H200Zm160-160q-33 0-56.5-23.5T280 736V256q0-33 23.5-56.5T360 176h360q33 0 56.5 23.5T800 256v480q0 33-23.5 56.5T720 816H360Zm0-80h360V256H360v480Zm0 0V256v480Z"/></svg><svg xmlns="http://www.w3.org/2000/svg" height="24" width="24" viewBox="0 96 960 960" fill="currentColor" stroke="none" class="copy-success-icon h-[14px] w-[14px] transition-all transform scale-0 absolute"><path d="M382 799q-8 0-15-2.5t-13-8.5L182 616q-11-11-10.5-28.5T183 559q11-11 28-11t28 11l143 143 339-339q11-11 28.5-11t28.5 11q11 11 11 28.5T778 420L410 788q-6 6-13 8.5t-15 2.5Z"/></svg></button>';
                             t.insertAdjacentHTML("beforeend", e)
                         }
                     }));
-                    const t = new(Pn())("button.copy", {
+                    const t = new(Nn())("button.copy", {
                         target: e => e.parentNode
                     });
                     t.on("success", (e => {
                         let {
                             trigger: t
                         } = e;
                         const n = t.getAttribute("data-tooltip"),
                             r = t.querySelector(".copy-icon"),
                             i = t.querySelector(".copy-success-icon");
-                        Rn(r, i), t.setAttribute("data-tooltip", "Copied!"), setTimeout((() => {
-                            Rn(i, r), t.setAttribute("data-tooltip", n)
+                        Pn(r, i), t.setAttribute("data-tooltip", "Copied!"), setTimeout((() => {
+                            Pn(i, r), t.setAttribute("data-tooltip", n)
                         }), 2e3)
                     }))
                 }()
             }))
         }()
 }();
```

### Comparing `sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/toc.py` & `sphinxawesome_theme-5.0.0b2/src/sphinxawesome_theme/toc.py`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.0.0b1/PKG-INFO` & `sphinxawesome_theme-5.0.0b2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxawesome-theme
-Version: 5.0.0b1
+Version: 5.0.0b2
 Summary: An awesome theme for the Sphinx documentation generator
 Home-page: https://sphinxawesome.xyz
 License: MIT
 Author: Kai Welke
 Author-email: kai687@pm.me
 Requires-Python: >=3.8,<4.0
 Classifier: Framework :: Sphinx
@@ -53,30 +53,19 @@
 
    ```python
    html_theme = "sphinxawesome_theme"
    ```
 
    For more information, see [Add your theme](https://sphinxawesome.xyz/how-to/add/).
 
-1. Optional:
-
-   - If you want to use Algolia DocSearch with this theme,
-     load the bundled extension:
-
-     ```python
-     # conf.py
-     extensions += ["sphinxawesome_theme.docsearch"]
-     ```
-
-   - If you want to use awesome features for highlighting code,
-     load the bundled extension:
+1. Optional: add bundled extensions for more awesome features:
 
      ```python
      # conf.py
-     extensions += ["sphinxawesome_theme.highlighting"]
+     extensions += ["sphinxawesome_theme.docsearch", "sphinxawesome.highlighting"]
      ```
 
 ## Features
 
 With the Awesome Theme, you can build readable, functional, and beautiful documentation websites.
 
 ### Awesome code blocks
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sphinxawesome-theme Version: 5.0.0b1 Summary: An
+Metadata-Version: 2.1 Name: sphinxawesome-theme Version: 5.0.0b2 Summary: An
 awesome theme for the Sphinx documentation generator Home-page: https://
 sphinxawesome.xyz License: MIT Author: Kai Welke Author-email: kai687@pm.me
 Requires-Python: >=3.8,<4.0 Classifier: Framework :: Sphinx Classifier:
 Framework :: Sphinx :: Theme Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
@@ -17,20 +17,18 @@
  Create beautiful and awesome documentation websites with Sphinx. See how the
                     theme looks like on sphinxawesome.xyz.
 ## Get started 1. Install the theme as a Python package: ```console pip install
 sphinxawesome-theme ``` For more information, see [Install the theme](https://
 sphinxawesome.xyz/how-to/install/). 1. Add `sphinxawesome_theme` as an HTML
 theme in your Sphinx configuration file `conf.py`: ```python html_theme =
 "sphinxawesome_theme" ``` For more information, see [Add your theme](https://
-sphinxawesome.xyz/how-to/add/). 1. Optional: - If you want to use Algolia
-DocSearch with this theme, load the bundled extension: ```python # conf.py
-extensions += ["sphinxawesome_theme.docsearch"] ``` - If you want to use
-awesome features for highlighting code, load the bundled extension: ```python #
-conf.py extensions += ["sphinxawesome_theme.highlighting"] ``` ## Features With
-the Awesome Theme, you can build readable, functional, and beautiful
+sphinxawesome.xyz/how-to/add/). 1. Optional: add bundled extensions for more
+awesome features: ```python # conf.py extensions +=
+["sphinxawesome_theme.docsearch", "sphinxawesome.highlighting"] ``` ## Features
+With the Awesome Theme, you can build readable, functional, and beautiful
 documentation websites. ### Awesome code blocks - Code block have a **Copy**
 button for copying the code. - If you load the bundled
 `sphinxawesome_theme.highlighting`, you can use these additional options in
 your ``code-block`` directives: - `emphasize-added`. Highlight lines that
 should be added to code - `emphasize-removed`. Highlight lines that should be
 removed from the code - `emphasize-text: TEXT`. Highlight _`TEXT`_ in the code
 block to emphasize placeholder text. ### Better headerlinks Clicking the link
```

