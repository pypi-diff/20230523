# Comparing `tmp/rubyvenv-1.1.1.tar.gz` & `tmp/rubyvenv-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubyvenv-1.1.1.tar", last modified: Wed Jul  7 18:13:25 2021, max compression
+gzip compressed data, was "rubyvenv-1.2.0.tar", last modified: Mon May 22 23:09:50 2023, max compression
```

## Comparing `rubyvenv-1.1.1.tar` & `rubyvenv-1.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2021-07-07 18:13:25.402547 rubyvenv-1.1.1/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2021-07-07 18:07:14.000000 rubyvenv-1.1.1/LICENSE
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1515 2021-07-07 18:13:25.402547 rubyvenv-1.1.1/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)      659 2021-07-07 18:07:14.000000 rubyvenv-1.1.1/README.md
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2021-07-07 18:13:25.402547 rubyvenv-1.1.1/rubyvenv.egg-info/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1515 2021-07-07 18:13:25.000000 rubyvenv-1.1.1/rubyvenv.egg-info/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)      242 2021-07-07 18:13:25.000000 rubyvenv-1.1.1/rubyvenv.egg-info/SOURCES.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2021-07-07 18:13:25.000000 rubyvenv-1.1.1/rubyvenv.egg-info/dependency_links.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       44 2021-07-07 18:13:25.000000 rubyvenv-1.1.1/rubyvenv.egg-info/entry_points.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        7 2021-07-07 18:13:25.000000 rubyvenv-1.1.1/rubyvenv.egg-info/requires.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        9 2021-07-07 18:13:25.000000 rubyvenv-1.1.1/rubyvenv.egg-info/top_level.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)     8417 2021-07-07 18:13:04.000000 rubyvenv-1.1.1/rubyvenv.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1328 2021-07-07 18:13:25.402547 rubyvenv-1.1.1/setup.cfg
--rw-r--r--   0 asottile  (1000) asottile  (1000)       37 2021-07-07 18:07:14.000000 rubyvenv-1.1.1/setup.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-22 23:09:50.200587 rubyvenv-1.2.0/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2023-05-22 22:56:01.000000 rubyvenv-1.2.0/LICENSE
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1050 2023-05-22 23:09:50.200587 rubyvenv-1.2.0/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      416 2023-05-22 22:56:01.000000 rubyvenv-1.2.0/README.md
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-22 23:09:50.200587 rubyvenv-1.2.0/rubyvenv.egg-info/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1050 2023-05-22 23:09:50.000000 rubyvenv-1.2.0/rubyvenv.egg-info/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      242 2023-05-22 23:09:50.000000 rubyvenv-1.2.0/rubyvenv.egg-info/SOURCES.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-05-22 23:09:50.000000 rubyvenv-1.2.0/rubyvenv.egg-info/dependency_links.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       43 2023-05-22 23:09:50.000000 rubyvenv-1.2.0/rubyvenv.egg-info/entry_points.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        7 2023-05-22 23:09:50.000000 rubyvenv-1.2.0/rubyvenv.egg-info/requires.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        9 2023-05-22 23:09:50.000000 rubyvenv-1.2.0/rubyvenv.egg-info/top_level.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     8611 2023-05-22 23:09:49.000000 rubyvenv-1.2.0/rubyvenv.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1142 2023-05-22 23:09:50.200587 rubyvenv-1.2.0/setup.cfg
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2023-05-22 22:56:01.000000 rubyvenv-1.2.0/setup.py
```

### Comparing `rubyvenv-1.1.1/LICENSE` & `rubyvenv-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rubyvenv-1.1.1/rubyvenv.py` & `rubyvenv-1.2.0/rubyvenv.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import argparse
 import functools
 import gzip
 import html.parser
 import io
 import os.path
 import pipes
@@ -10,19 +12,16 @@
 import tarfile
 import tempfile
 import urllib.parse
 import urllib.request
 from typing import Callable
 from typing import ContextManager
 from typing import IO
-from typing import List
 from typing import NamedTuple
-from typing import Optional
 from typing import Sequence
-from typing import Tuple
 
 import distro
 
 # Roughly stolen from python virtualenv 15.0.1
 ACTIVATE = '''\
 # This file must be used with "source bin/activate" *from bash*
 # you cannot run it directly
@@ -142,20 +141,20 @@
 def get_platform_info() -> Platform:
     return Platform(distro.id(), distro.version(), platform.machine())
 
 
 class GetsAHrefs(html.parser.HTMLParser):
     def __init__(self) -> None:
         super().__init__()
-        self.hrefs: List[Optional[str]] = []
+        self.hrefs: list[str | None] = []
 
     def handle_starttag(
             self,
             tag: str,
-            attrs: List[Tuple[str, Optional[str]]],
+            attrs: list[tuple[str, str | None]],
     ) -> None:
         if tag == 'a':
             self.hrefs.append(dict(attrs)['href'])
 
 
 def _decode_response(resp_bytes: bytes) -> str:
     """Even though we request identity, rvm.io sends us gzip."""
@@ -180,15 +179,15 @@
 
 def _download_url(platform_info: Platform, version: str) -> str:
     return urllib.parse.urljoin(
         platform_info.rvm_url, _version_to_filename(version),
     )
 
 
-def get_prebuilt_versions(platform_info: Platform) -> Tuple[Version, ...]:
+def get_prebuilt_versions(platform_info: Platform) -> tuple[Version, ...]:
     url = platform_info.rvm_url
     resp = _decode_response(urllib.request.urlopen(url).read())
     parser = GetsAHrefs()
     parser.feed(resp)
     return tuple(
         Version(
             _filename_to_version(href),
@@ -223,14 +222,19 @@
 
 def _write_activate(dest: str, more: str = '') -> None:
     with open(os.path.join(dest, 'bin', 'activate'), 'w') as activate:
         activate.write(ACTIVATE.replace('DIRECTORY', pipes.quote(dest)))
         activate.write(more)
 
 
+def _write_gitignore(dest: str) -> None:
+    with open(os.path.join(dest, '.gitignore'), 'w') as gitignore:
+        gitignore.write('# created by rubyvenv automatically\n*\n')
+
+
 def make_environment(dest: str, version: Version) -> int:
     platform_info = get_platform_info()
     filename = _version_to_filename(version.version)
     cache_file = '{name}/{version}/{arch}/{filename}'.format(
         filename=filename, **platform_info._asdict(),
     )
     get_fileobj = functools.partial(urllib.request.urlopen, version.url)
@@ -251,27 +255,29 @@
         for member in members:
             if os.sep in member.name:
                 _, member.name = member.name.split(os.sep, 1)
             else:
                 member.name = ''
         tar_file.extractall(dest, members)
     _write_activate(dest)
+    _write_gitignore(dest)
     return 0
 
 
 def make_system_environment(dest: str) -> int:
     os.makedirs(os.path.join(dest, 'bin'), exist_ok=True)
     ruby = shutil.which('ruby')
     gem = shutil.which('gem')
     assert ruby and gem, (ruby, gem)
     _write_activate(dest, more=SET_GEM_HOME)
+    _write_gitignore(dest)
     return 0
 
 
-def main(argv: Optional[Sequence[str]] = None) -> int:
+def main(argv: Sequence[str] | None = None) -> int:
     parser = argparse.ArgumentParser()
     parser.add_argument('dest', nargs='?', metavar='DEST_DIR')
     parser.add_argument('--ruby', default='latest')
     parser.add_argument(
         '--list-versions', action='store_true',
         help='List versions available for your system',
     )
@@ -287,8 +293,8 @@
             return make_system_environment(args.dest)
         else:
             version = pick_version(args.ruby)
             return make_environment(args.dest, version)
 
 
 if __name__ == '__main__':
-    exit(main())
+    raise SystemExit(main())
```

### Comparing `rubyvenv-1.1.1/setup.cfg` & `rubyvenv-1.2.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 [metadata]
 name = rubyvenv
-version = 1.1.1
+version = 1.2.0
 description = Create no-hassle ruby "virtualenvs".  No .bashrc, no shims, no cd-magic.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/asottile/rubyvenv
 author = Anthony Sottile
 author_email = asottile@umich.edu
 license = MIT
 license_file = LICENSE
 classifiers = 
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
-	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 
 [options]
 py_modules = rubyvenv
 install_requires = 
 	distro
-python_requires = >=3.6.1
+python_requires = >=3.7
 
 [options.entry_points]
 console_scripts = 
 	rubyvenv = rubyvenv:main
 
 [bdist_wheel]
 universal = True
@@ -37,15 +33,14 @@
 plugins = covdefaults
 
 [mypy]
 check_untyped_defs = true
 disallow_any_generics = true
 disallow_incomplete_defs = true
 disallow_untyped_defs = true
-no_implicit_optional = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 
 [mypy-testing.*]
 disallow_untyped_defs = false
 
 [mypy-tests.*]
```

