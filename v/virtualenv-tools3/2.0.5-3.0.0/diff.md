# Comparing `tmp/virtualenv-tools3-2.0.5.tar.gz` & `tmp/virtualenv_tools3-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/virtualenv-tools3-2.0.5.tar", last modified: Tue Mar  9 23:26:49 2021, max compression
+gzip compressed data, was "virtualenv_tools3-3.0.0.tar", last modified: Tue May 23 00:31:13 2023, max compression
```

## Comparing `virtualenv-tools3-2.0.5.tar` & `virtualenv_tools3-3.0.0.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 bariteau  (3176) users      (100)        0 2021-03-09 23:26:49.000000 virtualenv-tools3-2.0.5/
--rw-r--r--   0 bariteau  (3176) users      (100)       18 2021-03-08 23:57:24.000000 virtualenv-tools3-2.0.5/MANIFEST.in
--rw-r--r--   0 bariteau  (3176) users      (100)     4355 2021-03-09 23:26:49.000000 virtualenv-tools3-2.0.5/PKG-INFO
--rw-r--r--   0 bariteau  (3176) users      (100)     2921 2021-03-08 23:57:24.000000 virtualenv-tools3-2.0.5/README.md
--rw-r--r--   0 bariteau  (3176) users      (100)       70 2021-03-09 23:26:49.000000 virtualenv-tools3-2.0.5/setup.cfg
--rw-r--r--   0 bariteau  (3176) users      (100)     1025 2021-03-09 23:23:11.000000 virtualenv-tools3-2.0.5/setup.py
--rw-r--r--   0 bariteau  (3176) users      (100)    11661 2021-03-09 23:23:04.000000 virtualenv-tools3-2.0.5/virtualenv_tools.py
-drwxr-xr-x   0 bariteau  (3176) users      (100)        0 2021-03-09 23:26:49.000000 virtualenv-tools3-2.0.5/virtualenv_tools3.egg-info/
--rw-r--r--   0 bariteau  (3176) users      (100)     4355 2021-03-09 23:26:49.000000 virtualenv-tools3-2.0.5/virtualenv_tools3.egg-info/PKG-INFO
--rw-r--r--   0 bariteau  (3176) users      (100)      308 2021-03-09 23:26:49.000000 virtualenv-tools3-2.0.5/virtualenv_tools3.egg-info/SOURCES.txt
--rw-r--r--   0 bariteau  (3176) users      (100)        1 2021-03-09 23:26:49.000000 virtualenv-tools3-2.0.5/virtualenv_tools3.egg-info/dependency_links.txt
--rw-r--r--   0 bariteau  (3176) users      (100)       60 2021-03-09 23:26:49.000000 virtualenv-tools3-2.0.5/virtualenv_tools3.egg-info/entry_points.txt
--rw-r--r--   0 bariteau  (3176) users      (100)        1 2021-03-09 00:03:57.000000 virtualenv-tools3-2.0.5/virtualenv_tools3.egg-info/not-zip-safe
--rw-r--r--   0 bariteau  (3176) users      (100)       17 2021-03-09 23:26:49.000000 virtualenv-tools3-2.0.5/virtualenv_tools3.egg-info/top_level.txt
+drwxr-xr-x   0 ckuehl    (3119) users      (100)        0 2023-05-23 00:31:13.194668 virtualenv_tools3-3.0.0/
+-rw-r--r--   0 ckuehl    (3119) users      (100)     1499 2017-07-22 21:16:14.000000 virtualenv_tools3-3.0.0/LICENSE
+-rw-r--r--   0 ckuehl    (3119) users      (100)     3602 2023-05-23 00:31:13.194668 virtualenv_tools3-3.0.0/PKG-INFO
+-rw-r--r--   0 ckuehl    (3119) users      (100)     2921 2017-10-19 21:09:54.000000 virtualenv_tools3-3.0.0/README.md
+-rw-r--r--   0 ckuehl    (3119) users      (100)     1136 2023-05-23 00:31:13.194668 virtualenv_tools3-3.0.0/setup.cfg
+-rw-r--r--   0 ckuehl    (3119) users      (100)       37 2023-05-23 00:30:18.000000 virtualenv_tools3-3.0.0/setup.py
+-rw-r--r--   0 ckuehl    (3119) users      (100)    10527 2023-05-23 00:30:18.000000 virtualenv_tools3-3.0.0/virtualenv_tools.py
+drwxr-xr-x   0 ckuehl    (3119) users      (100)        0 2023-05-23 00:31:13.194668 virtualenv_tools3-3.0.0/virtualenv_tools3.egg-info/
+-rw-r--r--   0 ckuehl    (3119) users      (100)     3602 2023-05-23 00:31:13.000000 virtualenv_tools3-3.0.0/virtualenv_tools3.egg-info/PKG-INFO
+-rw-r--r--   0 ckuehl    (3119) users      (100)      264 2023-05-23 00:31:13.000000 virtualenv_tools3-3.0.0/virtualenv_tools3.egg-info/SOURCES.txt
+-rw-r--r--   0 ckuehl    (3119) users      (100)        1 2023-05-23 00:31:13.000000 virtualenv_tools3-3.0.0/virtualenv_tools3.egg-info/dependency_links.txt
+-rw-r--r--   0 ckuehl    (3119) users      (100)       60 2023-05-23 00:31:13.000000 virtualenv_tools3-3.0.0/virtualenv_tools3.egg-info/entry_points.txt
+-rw-r--r--   0 ckuehl    (3119) users      (100)       17 2023-05-23 00:31:13.000000 virtualenv_tools3-3.0.0/virtualenv_tools3.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `virtualenv-tools3-2.0.5/README.md` & `virtualenv_tools3-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `virtualenv-tools3-2.0.5/virtualenv_tools.py` & `virtualenv_tools3-3.0.0/virtualenv_tools.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,58 +6,57 @@
     A helper script that moves virtualenvs to a new location.
 
     It only supports POSIX based virtualenvs and at the moment.
 
     :copyright: (c) 2012 by Fireteam Ltd.
     :license: BSD, see LICENSE for more details.
 """
-from __future__ import print_function
+from __future__ import annotations
 
 import argparse
-import collections
 import marshal
 import os.path
 import re
 import shutil
 import sys
 from types import CodeType
+from typing import NamedTuple
+from typing import Sequence
 
 
 ACTIVATION_SCRIPTS = [
     'activate',
     'activate.csh',
     'activate.fish',
     'activate.xsh',
 ]
 _pybin_match = re.compile(r'^python\d+\.\d+$')
-_pypy_match = re.compile(r'^\d+(.\d+)?$')
+_pypy_match = re.compile(r'^pypy\d+.\d+$')
 _activation_path_re = re.compile(
     r'^(?:set -gx |setenv |)VIRTUAL_ENV[ =][\'"](.*?)[\'"]\s*$',
 )
 VERBOSE = False
-MAGIC_LENGTH = 4 + 4  # magic length + 4 byte timestamp
-# In python3.3, a 4 byte "size" hint was added to pyc files
-if sys.version_info >= (3, 3):  # pragma: no cover (PY33+)
-    MAGIC_LENGTH += 4
+# magic length
+# + 4 byte timestamp
+# + 4 byte "size" hint was added to pyc files
 # PEP 552 (implemented in python 3.7) extends this by another word
-if sys.version_info >= (3, 7):  # pragma: no cover (PY37+)
-    MAGIC_LENGTH += 4
+MAGIC_LENGTH = 4 + 4 + 4 + 4
 
 
-def debug(msg):
+def debug(msg: str) -> None:
     if VERBOSE:
         print(msg)
 
 
-def update_activation_script(script_filename, new_path):
+def update_activation_script(script_filename: str, new_path: str) -> None:
     """Updates the paths for the activate shell scripts."""
     with open(script_filename) as f:
         lines = list(f)
 
-    def _handle_sub(match):
+    def _handle_sub(match: re.Match[str]) -> str:
         text = match.group()
         start, end = match.span()
         g_start, g_end = match.span(1)
         return text[:(g_start - start)] + new_path + text[(g_end - end):]
 
     changed = False
     for idx, line in enumerate(lines):
@@ -68,24 +67,28 @@
 
     if changed:
         debug('A %s' % script_filename)
         with open(script_filename, 'w') as f:
             f.writelines(lines)
 
 
-def path_is_within(path, within):
+def path_is_within(path: bytes, within: bytes) -> bool:
     relpath = os.path.relpath(path, within)
     return not relpath.startswith(b'.')
 
 
-def update_script(script_filename, old_path, new_path):
+def update_script(
+        script_filename: str,
+        old_path_s: str,
+        new_path_s: str,
+) -> None:
     """Updates shebang lines for actual scripts."""
     filesystem_encoding = sys.getfilesystemencoding()
-    old_path = old_path.encode(filesystem_encoding)
-    new_path = new_path.encode(filesystem_encoding)
+    old_path = old_path_s.encode(filesystem_encoding)
+    new_path = new_path_s.encode(filesystem_encoding)
 
     with open(script_filename, 'rb') as f:
         if f.read(2) != b'#!':
             return
         f.seek(0)
         lines = list(f)
     args = lines[0][2:].strip().split()
@@ -100,75 +103,61 @@
     args[0] = new_bin
     lines[0] = b'#!' + b' '.join(args) + b'\n'
     debug('S %s' % script_filename)
     with open(script_filename, 'wb') as f:
         f.writelines(lines)
 
 
-def update_scripts(bin_dir, orig_path, new_path, activation=False):
+def update_scripts(
+        bin_dir: str,
+        orig_path: str,
+        new_path: str,
+        activation: bool = False,
+) -> None:
     """Updates all scripts in the bin folder."""
     for fname in os.listdir(bin_dir):
         path = os.path.join(bin_dir, fname)
         if fname in ACTIVATION_SCRIPTS and activation:
             update_activation_script(path, new_path)
         elif os.path.isfile(path):
             update_script(path, orig_path, new_path)
 
 
-def update_pyc(filename, new_path):
+def update_pyc(filename: str, new_path: str) -> None:
     """Updates the filenames stored in pyc files."""
-    with open(filename, 'rb') as f:
-        magic = f.read(MAGIC_LENGTH)
+    with open(filename, 'rb') as rf:
+        magic = rf.read(MAGIC_LENGTH)
         try:
-            code = marshal.load(f)
+            code = marshal.load(rf)
         except Exception:
             print('Error in %s' % filename)
             raise
 
-    def _make_code(code, filename, consts):
-        if sys.version_info[0] == 2:  # pragma: no cover (PY2)
-            return CodeType(
-                code.co_argcount, code.co_nlocals, code.co_stacksize,
-                code.co_flags, code.co_code, tuple(consts), code.co_names,
-                code.co_varnames, filename, code.co_name, code.co_firstlineno,
-                code.co_lnotab, code.co_freevars, code.co_cellvars,
-            )
-        elif sys.version_info < (3, 8):  # pragma: no cover (<py38)
-            return CodeType(
-                code.co_argcount, code.co_kwonlyargcount, code.co_nlocals,
-                code.co_stacksize, code.co_flags, code.co_code, tuple(consts),
-                code.co_names, code.co_varnames, filename, code.co_name,
-                code.co_firstlineno, code.co_lnotab, code.co_freevars,
-                code.co_cellvars,
-            )
-        else:  # pragma: no cover (py38+)
-            return code.replace(co_consts=tuple(consts), co_filename=filename)
-
-    def _process(code):
+    def _process(code: CodeType) -> CodeType:
         consts = []
         for const in code.co_consts:
             if type(const) is CodeType:
                 const = _process(const)
             consts.append(const)
         if new_path != code.co_filename or consts != list(code.co_consts):
-            code = _make_code(code, new_path, consts)
+            code = code.replace(co_filename=new_path, co_consts=tuple(consts))
         return code
 
     new_code = _process(code)
 
     if new_code is not code:
         debug('B %s' % filename)
-        with open(filename, 'wb') as f:
-            f.write(magic)
-            marshal.dump(new_code, f)
+        with open(filename, 'wb') as wf:
+            wf.write(magic)
+            marshal.dump(new_code, wf)
 
 
-def update_pycs(lib_dir, new_path):
+def update_pycs(lib_dir: str, new_path: str) -> None:
     """Walks over all pyc files and updates their paths."""
-    def get_new_path(filename):
+    def get_new_path(filename: str) -> str:
         filename = os.path.normpath(filename)
         return os.path.join(new_path, filename[len(lib_dir) + 1:])
 
     for dirname, dirnames, filenames in os.walk(lib_dir):
         for filename in filenames:
             if (
                     filename.endswith(('.pyc', '.pyo')) and
@@ -176,68 +165,67 @@
                     not os.path.islink(os.path.join(dirname, filename))
             ):
                 filename = os.path.join(dirname, filename)
                 local_path = get_new_path(filename)
                 update_pyc(filename, local_path)
 
 
-def _update_pth_file(pth_filename, orig_path, is_pypy):
+def _update_pth_file(pth_filename: str, orig_path: str) -> None:
     with open(pth_filename) as f:
         lines = f.readlines()
     changed = False
     for i, line in enumerate(lines):
         val = line.strip()
         if val.startswith('import ') or not os.path.isabs(val):
             continue
         changed = True
         relto_original = os.path.relpath(val, orig_path)
         # If we are moving a pypy venv the site-packages directory
         # is in a different location than if we are moving a cpython venv
         relto_pth = os.path.join(
-            '..' if is_pypy    # venv/site-packages
-            else '../../..',   # venv/lib/pythonX.X/site-packages
+            '../../..',   # venv/lib/pythonX.X/site-packages
             relto_original
         )
-        lines[i] = '{}\n'.format(relto_pth)
+        lines[i] = f'{relto_pth}\n'
     if changed:
         with open(pth_filename, 'w') as f:
             f.write(''.join(lines))
-        debug('P {}'.format(pth_filename))
+        debug(f'P {pth_filename}')
 
 
-def update_pth_files(site_packages, orig_path, is_pypy):
+def update_pth_files(site_packages: str, orig_path: str) -> None:
     """Converts /full/paths in pth files to relative relocatable paths."""
     for filename in os.listdir(site_packages):
         filename = os.path.join(site_packages, filename)
         if filename.endswith('.pth') and os.path.isfile(filename):
-            _update_pth_file(filename, orig_path, is_pypy)
+            _update_pth_file(filename, orig_path)
 
 
-def remove_local(base):
+def remove_local(base: str) -> None:
     """On some systems virtualenv seems to have something like a local
     directory with symlinks.  This directory is safe to remove in modern
     versions of virtualenv.  Delete it.
     """
     local_dir = os.path.join(base, 'local')
     if os.path.exists(local_dir):  # pragma: no cover (not all systems)
-        debug('D {}'.format(local_dir))
+        debug(f'D {local_dir}')
         shutil.rmtree(local_dir)
 
 
-def update_paths(venv, new_path):
+def update_paths(venv: Virtualenv, new_path: str) -> None:
     """Updates all paths in a virtualenv to a new one."""
     update_scripts(venv.bin_dir, venv.orig_path, new_path)
     for lib_dir in venv.lib_dirs:
         update_pycs(lib_dir, new_path)
-    update_pth_files(venv.site_packages, venv.orig_path, venv.is_pypy)
+    update_pth_files(venv.site_packages, venv.orig_path)
     remove_local(venv.path)
     update_scripts(venv.bin_dir, venv.orig_path, new_path, activation=True)
 
 
-def get_orig_path(venv_path):
+def get_orig_path(venv_path: str) -> str:
     """This helps us know whether someone has tried to relocate the
     virtualenv
     """
     activate_path = os.path.join(venv_path, 'bin/activate')
 
     with open(activate_path) as activate:
         for line in activate:
@@ -248,38 +236,31 @@
         else:
             raise AssertionError(
                 'Could not find VIRTUAL_ENV= in activation script: %s' %
                 activate_path
             )
 
 
-class NotAVirtualenvError(OSError):
-    def __init__(self, *args):
-        self.args = args
-
-    def __str__(self):
+class NotAVirtualenvError(ValueError):
+    def __str__(self) -> str:
         return '{} is not a virtualenv: not a {}: {}'.format(*self.args)
 
 
-Virtualenv = collections.namedtuple(
-    'Virtualenv', (
-        'path',
-        'bin_dir',
-        'lib_dirs',
-        'site_packages',
-        'orig_path',
-        'is_pypy'
-    ),
-)
+class Virtualenv(NamedTuple):
+    path: str
+    bin_dir: str
+    lib_dirs: list[str]
+    site_packages: str
+    orig_path: str
 
 
-def _get_original_state(path):
-    is_pypy = os.path.isdir(os.path.join(path, 'lib_pypy'))
+def _get_original_state(path: str) -> Virtualenv:
+    is_pypy = os.path.isfile(os.path.join(path, 'bin', 'pypy'))
     bin_dir = os.path.join(path, 'bin')
-    base_lib_dir = os.path.join(path, 'lib-python' if is_pypy else 'lib')
+    base_lib_dir = os.path.join(path, 'lib')
     activate_file = os.path.join(bin_dir, 'activate')
 
     for dir_path in (bin_dir, base_lib_dir):
         if not os.path.isdir(dir_path):
             raise NotAVirtualenvError(path, 'directory', dir_path)
     if not os.path.isfile(activate_file):
         raise NotAVirtualenvError(path, 'file', activate_file)
@@ -290,36 +271,32 @@
         for potential_lib_dir in os.listdir(base_lib_dir)
         if matcher.match(potential_lib_dir)
     ]
     if len(lib_dirs) != 1:
         raise NotAVirtualenvError(
             path,
             'directory',
-            os.path.join(base_lib_dir, '#(.#)?' if is_pypy else 'python#.#'),
+            os.path.join(base_lib_dir, 'pypy#.#)' if is_pypy else 'python#.#'),
         )
     lib_dir, = lib_dirs
 
-    site_packages = os.path.join(path if is_pypy else lib_dir, 'site-packages')
+    site_packages = os.path.join(lib_dir, 'site-packages')
     if not os.path.isdir(site_packages):
         raise NotAVirtualenvError(path, 'directory', site_packages)
 
-    lib_dirs = [lib_dir]
-    if is_pypy:  # pragma: no cover (pypy only)
-        lib_dirs.append(os.path.join(path, 'lib_pypy'))
     return Virtualenv(
         path=path,
         bin_dir=bin_dir,
-        lib_dirs=lib_dirs,
+        lib_dirs=[lib_dir],
         site_packages=site_packages,
         orig_path=get_orig_path(path),
-        is_pypy=is_pypy
     )
 
 
-def main(argv=None):
+def main(argv: Sequence[str] | None = None) -> int:
     parser = argparse.ArgumentParser()
     parser.add_argument(
         '--update-path',
         required=True,
         help=(
             'Update the path for all required executables and helper files '
             'that are supported to the new python prefix.  You can also set '
@@ -337,27 +314,27 @@
 
     if args.update_path == 'auto':
         update_path = os.path.abspath(args.path)
     else:
         update_path = args.update_path
 
     if not os.path.isabs(update_path):
-        print('--update-path must be absolute: {}'.format(update_path))
+        print(f'--update-path must be absolute: {update_path}')
         return 1
 
     try:
         venv = _get_original_state(path=args.path)
     except NotAVirtualenvError as e:
         print(e)
         return 1
 
     if venv.orig_path == update_path:
-        print('Already up-to-date: %s (%s)' % (venv.path, update_path))
+        print(f'Already up-to-date: {venv.path} ({update_path})')
         return 0
 
     update_paths(venv, update_path)
-    print('Updated: %s (%s -> %s)' % (venv.path, venv.orig_path, update_path))
+    print(f'Updated: {venv.path} ({venv.orig_path} -> {update_path})')
     return 0
 
 
 if __name__ == '__main__':
-    exit(main())
+    raise SystemExit(main())
```

