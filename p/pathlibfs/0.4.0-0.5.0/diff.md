# Comparing `tmp/pathlibfs-0.4.0.tar.gz` & `tmp/pathlibfs-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pathlibfs-0.4.0.tar", max compression
+gzip compressed data, was "pathlibfs-0.5.0.tar", max compression
```

## Comparing `pathlibfs-0.4.0.tar` & `pathlibfs-0.5.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1072 2022-12-23 16:37:29.787681 pathlibfs-0.4.0/LICENSE
--rw-r--r--   0        0        0     7473 2022-12-23 16:37:29.787681 pathlibfs-0.4.0/README.md
--rw-r--r--   0        0        0      836 2022-12-23 16:37:29.787681 pathlibfs-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      395 2022-12-23 16:37:29.787681 pathlibfs-0.4.0/src/pathlibfs/__init__.py
--rw-r--r--   0        0        0       76 2022-12-23 16:37:29.787681 pathlibfs-0.4.0/src/pathlibfs/exception.py
--rw-r--r--   0        0        0    26107 2022-12-23 16:37:29.787681 pathlibfs-0.4.0/src/pathlibfs/path.py
--rw-r--r--   0        0        0     1893 2022-12-23 16:37:29.787681 pathlibfs-0.4.0/src/pathlibfs/s3_support.py
--rw-r--r--   0        0        0     8407 1970-01-01 00:00:00.000000 pathlibfs-0.4.0/setup.py
--rw-r--r--   0        0        0     8083 1970-01-01 00:00:00.000000 pathlibfs-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-23 00:59:47.087581 pathlibfs-0.5.0/LICENSE
+-rw-r--r--   0        0        0     7473 2023-05-23 00:59:47.087581 pathlibfs-0.5.0/README.md
+-rw-r--r--   0        0        0      836 2023-05-23 00:59:47.087581 pathlibfs-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      409 2023-05-23 00:59:47.087581 pathlibfs-0.5.0/src/pathlibfs/__init__.py
+-rw-r--r--   0        0        0       76 2023-05-23 00:59:47.087581 pathlibfs-0.5.0/src/pathlibfs/exception.py
+-rw-r--r--   0        0        0    26107 2023-05-23 00:59:47.087581 pathlibfs-0.5.0/src/pathlibfs/path.py
+-rw-r--r--   0        0        0     1893 2023-05-23 00:59:47.087581 pathlibfs-0.5.0/src/pathlibfs/s3_support.py
+-rw-r--r--   0        0        0     8072 1970-01-01 00:00:00.000000 pathlibfs-0.5.0/PKG-INFO
```

### Comparing `pathlibfs-0.4.0/LICENSE` & `pathlibfs-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pathlibfs-0.4.0/README.md` & `pathlibfs-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pathlibfs-0.4.0/pyproject.toml` & `pathlibfs-0.5.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "pathlibfs"
-version = "0.4.0"
+version = "0.5.0"
 description = "pathlib 🤝 fsspec, manipulate remote filesystem paths."
 readme = "README.md"
 authors = ["Hiroyuki \"Roy\" Tanaka <aflc0x@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-fsspec = "^2022.11.0"
+fsspec = ">=2023.5.0"
 
 [tool.poetry.group.test.dependencies]
-s3fs = "^2022.11.0"
-gcsfs = "^2022.11.0"
-adlfs = "^2022.11.2"
+s3fs = ">=2023.5.0"
+gcsfs = ">=2023.5.0"
+adlfs = ">=2023.4.0"
 pytest = "^7.1.2"
 pytest-cov = "^3.0.0"
 pytest-timeout = "^2.1.0"
 
 [tool.poetry.group.dev]
 optional = true
```

### Comparing `pathlibfs-0.4.0/src/pathlibfs/path.py` & `pathlibfs-0.5.0/src/pathlibfs/path.py`

 * *Files identical despite different names*

### Comparing `pathlibfs-0.4.0/src/pathlibfs/s3_support.py` & `pathlibfs-0.5.0/src/pathlibfs/s3_support.py`

 * *Files identical despite different names*

### Comparing `pathlibfs-0.4.0/setup.py` & `pathlibfs-0.5.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,193 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-package_dir = \
-{'': 'src'}
-
-packages = \
-['pathlibfs']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['fsspec>=2022.11.0,<2023.0.0']
-
-setup_kwargs = {
-    'name': 'pathlibfs',
-    'version': '0.4.0',
-    'description': 'pathlib 🤝 fsspec, manipulate remote filesystem paths.',
-    'long_description': '# pathlibfs\n\n[![codecov](https://codecov.io/gh/roy-ht/pathlibfs/branch/main/graph/badge.svg?token=MX1DTY2CNG)](https://codecov.io/gh/roy-ht/pathlibfs)\n\npathlib 🤝 fsspec\n\nLike pathlib, Python standard library module, manipulate remote filesystem paths.\n\n# Installation\n\n```\npip install pathlibfs\n```\n\n# Getting Started\n\nIt only provide `Path` class:\n\n```python\nfrom pathlibfs import Path\n\np = Path(\'your/path.txt\')\np_s3 = Path(\'s3://bucket/key.txt\')\np_gcs = Path(\'gs://bucket/key.txt\')\n```\n\npathlibfs uses [fsspec](https://github.com/fsspec/filesystem_spec) as a backend filesystem.\nSo if you want to use some specific remote filesystem, you need to install extra dependencies such as `s3fs` or `gcsfs`.\n\nSee [known implementations](https://github.com/fsspec/filesystem_spec/blob/a8cfd9c52a20c930c67ff296b60dbcda89d64db9/fsspec/registry.py#L87)\nto check out supported protocols.\n\n# Special Environment Variables\n| name | description |\n|-|-|\n| PATHLIBFS_S3_SESSION_CACHE | If defined, store S3 session cache locally like [boto3-session-cache](https://github.com/mixja/boto3-session-cache) |\n\n# APIs\n\n`Path` class has many methods, and it\'s almost same as [pathlib](https://docs.python.org/3.10/library/pathlib.html) and [fsspec.AbstractFileSystem](https://filesystem-spec.readthedocs.io/en/latest/api.html#fsspec.spec.AbstractFileSystem)\n.\n\nFor example, like pathlib, you can join path with `/`:\n\n```\np = Path(\'some/dir\') / \'subdir\'  # -> Path(\'some/dir/subdir\')\n```\n\n## properties\n\nGotcha.\n\n| name | description |\n|-|-|\n| fs | backend filesystem of fsspec |\n| path | path without protocol. e.g. Path(\'s3://bucket/key\') == \'bucket/key\' |\n| fullpath | path with protocol. e.g. Path(\'a.txt\') == \'file://a.txt\' |\n| urlpath | path with full chain. e.g. Path(\'simplecache::s3://bucket/key\') == \'simplecache::s3://bucket/key\' |\n| drive | same as pathlib |\n| root | same as pathlib |\n| parts | same as pathlib |\n| anchor | same as pathlib |\n| parents | same as pathlib, return List[Path] |\n| parent | same as pathlib, return Path |\n| has_parent | same as `path.parent != path` |\n| name | same as pathlib |\n| suffix | same as pathlib |\n| suffixes | same as pathlib |\n| stem | same as pathlib |\n| sep | separator of backend filesystem, such as \'/\' |\n| protocol | backend protocol. e.g. \'s3\', \'gcs\' |\n\n\n## pathlib based operations\n\n| name | description |\n|-|-|\n| `as_posix()` | only for local filesystem, otherwise raise an `PathlibfsException` |\n| `chmod(mode: int)` | only for local filesystem, otherwise raise an `PathlibfsException` |\n| `group()` | only for local filesystem, otherwise raise an `PathlibfsException` |\n| `is_mount()` | only for local filesystem, otherwise raise an `PathlibfsException` |\n| `is_symlink()` | only for local filesystem, otherwise raise an `PathlibfsException` |\n| `is_socket()` | only for local filesystem, otherwise raise an `PathlibfsException` |\n| `is_fifo()` | only for local filesystem, otherwise raise an `PathlibfsException` |\n| `is_block_device()` | only for local filesystem, otherwise raise an `PathlibfsException` |\n| `is_char_device()` | only for local filesystem, otherwise raise an `PathlibfsException` |\n| `owner()` | only for local filesystem, otherwise raise an `PathlibfsException` |\n| `symlink_to(target: PathLike)` | only for local filesystem, otherwise raise an `PathlibfsException` |\n| `resolve()` | only for local filesystem, otherwise return `self` |\n| `is_absolute()` | only for local filesystem, otherwise return True |\n| `is_reserved()` | only for local filesystem, otherwise return False |\n| `joinpath(*p)` | same as pathlib |\n| `match(pattern: str)` | same as pathlib |\n| `with_name(name: str)` | same as pathlib |\n| `with_suffix(suffix: str)` | same as pathlib |\n| `read_bytes()` | same as pathlib |\n| `read_text()` | same as pathlib |\n| `write_text(data)` | same as pathlib |\n| `write_bytes(data)` | same as pathlib |\n| `is_dir()` | same as pathlib |\n| `is_file()` | same as pathlib |\n| `unlink()` | same as pathlib |\n| `relative_to(path: PathLike)` | same as pathlib, but **return str**. `path == other / path.relative_to(other)` |\n| `iterdir(**kwargs)` | same as pathlib. It\'s just an wrapper of ls(), **it\'s not efficient.** Use `ls()`. |\n| `stat()` | alias of info. **It\'s not same as pathlib**, but fsspec\'s `info()` |\n| `rglob(pattern, **kwargs)` | same meaning as pathlib, and accept fsspec\'s `glob()` |\n\n## fsspec based mathods\n\n| name | description |\n|-|-|\n| `ls(**kwargs)` | same as fsspec |\n| `listdir()` | alias of ls |\n| `find(maxdepth: Optional[int] = None, withdirs: bool = False, **kwargs)` | same as fsspec |\n| `glob(pattern, **kwargs)` | same as fsspec |\n| `expand_path(recursive: bool = False, maxdepth: Optional[int] = None, **kwargs)` | same as fsspec |\n| `walk(maxdepth: Optional[int] = None, **kwargs)` | same as `os.walk` and fsspec\'s `walk`, yield `(dirpath, dirnames, filenames)`. And `dirpath` is `Path` instance. |\n| `exists(**kwargs)` | same as fsspec |\n| `isdir()` | same as fsspec |\n| `isfile()` | same as fsspec |\n| `lexists()` | same as fsspec |\n| `ukey()` | same as fsspec |\n| `checksum()` | same as fsspec |\n| `sign(expiration: int = 100, **kwargs)` | same as fsspec |\n| `size()` | same as fsspec |\n| `created()` | same as fsspec |\n| `modified()` | same as fsspec |\n| `du(total: bool = True, maxdepth: Optional[int] = None, **kwargs)` | same as fsspec |\n| `disk_usage()` | alias of du |\n| `info(**kwargs)` | same as fsspec |\n| `open()` | same as fsspec |\n| `cat(recursive: bool = False, on_error: str = "raise", **kwargs)` | same as fsspec |\n| `read_block(offset: int, length: int, delimiter: Optional[bytes] = None)` | same as fsspec |\n| `head(size: int = 1024)` | same as fsspec |\n| `tail(size: int = 1024)` | same as fsspec |\n| `mkdir(parents: bool = False, exist_ok: bool = False, **kwargs)` | same as fsspec |\n| `makedir()` | alias of mkdir |\n| `makedirs(exist_ok: bool = False, **kwargs)` | same as `mkdir(parents=True)` |\n| `mkdirs()` | alias of makedirs |\n| `touch(mode: int = 0o666, exist_ok: bool = True, truncate: bool = False, **kwargs) | same as fsspec |\n| `pipe_file(data)` | same as fsspec |\n| `rm_file()` | same as fsspec |\n| `rm(recursive: bool = False, maxdepth: Optional[int] = None)` | same as fsspec |\n| `delete()` | alias of rm |\n| `invalidate_cache()` | same as fsspec |\n| `clear_instance_cache()` | same as fsspec |\n| `copy(dst: PathLike, recursive: bool = False, on_error: Optional[str] = None, **kwargs)` | copy the path to dst. `copy()` can handle any protocol combinations so you don\'t need to call `put()` or `get()` for almost all cases. |\n| `cp()` | alias of copy |\n| `move(dst: PathLike, recursive=False, maxdepth=None, **kwargs)` | similar to copy, but delete source path after copy. |\n| `mv()`, `rename()`, `replace() | alias of move |\n| `put(target: PathLike, recursive: bool = False, callback=fsspec.callbacks._DEFAULT_CALLBACK, **kwargs)` | Upload **local** target to the path. |\n| `upload()` | alias of put |\n| `get(arget: PathLike, recursive: bool = False, callback=fsspec.callbacks._DEFAULT_CALLBACK, **kwargs)` | Downalod the path into **local** target. |\n| `download()` | alias of get |\n\n## others\n\n| name | description |\n|-|-|\n| `islocal()` | True if protocol is local filesystem. |\n| `clone(path: Optional[str] = None)` | copy self instance with different path (optional). |\n| `samefile(target: PathLike)` | same as `self == target` |\n\n\n# How to test\n\nStart mock server for testing.\n\n```\ndocker-compose up -d\n```\n\nRun test:\n```\npytest\n```',
-    'author': 'Hiroyuki "Roy" Tanaka',
-    'author_email': 'aflc0x@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
+Metadata-Version: 2.1
+Name: pathlibfs
+Version: 0.5.0
+Summary: pathlib 🤝 fsspec, manipulate remote filesystem paths.
+License: MIT
+Author: Hiroyuki "Roy" Tanaka
+Author-email: aflc0x@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: fsspec (>=2023.5.0)
+Description-Content-Type: text/markdown
+
+# pathlibfs
+
+[![codecov](https://codecov.io/gh/roy-ht/pathlibfs/branch/main/graph/badge.svg?token=MX1DTY2CNG)](https://codecov.io/gh/roy-ht/pathlibfs)
+
+pathlib 🤝 fsspec
+
+Like pathlib, Python standard library module, manipulate remote filesystem paths.
+
+# Installation
+
+```
+pip install pathlibfs
+```
+
+# Getting Started
+
+It only provide `Path` class:
+
+```python
+from pathlibfs import Path
+
+p = Path('your/path.txt')
+p_s3 = Path('s3://bucket/key.txt')
+p_gcs = Path('gs://bucket/key.txt')
+```
+
+pathlibfs uses [fsspec](https://github.com/fsspec/filesystem_spec) as a backend filesystem.
+So if you want to use some specific remote filesystem, you need to install extra dependencies such as `s3fs` or `gcsfs`.
+
+See [known implementations](https://github.com/fsspec/filesystem_spec/blob/a8cfd9c52a20c930c67ff296b60dbcda89d64db9/fsspec/registry.py#L87)
+to check out supported protocols.
+
+# Special Environment Variables
+| name | description |
+|-|-|
+| PATHLIBFS_S3_SESSION_CACHE | If defined, store S3 session cache locally like [boto3-session-cache](https://github.com/mixja/boto3-session-cache) |
+
+# APIs
+
+`Path` class has many methods, and it's almost same as [pathlib](https://docs.python.org/3.10/library/pathlib.html) and [fsspec.AbstractFileSystem](https://filesystem-spec.readthedocs.io/en/latest/api.html#fsspec.spec.AbstractFileSystem)
+.
+
+For example, like pathlib, you can join path with `/`:
+
+```
+p = Path('some/dir') / 'subdir'  # -> Path('some/dir/subdir')
+```
+
+## properties
+
+Gotcha.
+
+| name | description |
+|-|-|
+| fs | backend filesystem of fsspec |
+| path | path without protocol. e.g. Path('s3://bucket/key') == 'bucket/key' |
+| fullpath | path with protocol. e.g. Path('a.txt') == 'file://a.txt' |
+| urlpath | path with full chain. e.g. Path('simplecache::s3://bucket/key') == 'simplecache::s3://bucket/key' |
+| drive | same as pathlib |
+| root | same as pathlib |
+| parts | same as pathlib |
+| anchor | same as pathlib |
+| parents | same as pathlib, return List[Path] |
+| parent | same as pathlib, return Path |
+| has_parent | same as `path.parent != path` |
+| name | same as pathlib |
+| suffix | same as pathlib |
+| suffixes | same as pathlib |
+| stem | same as pathlib |
+| sep | separator of backend filesystem, such as '/' |
+| protocol | backend protocol. e.g. 's3', 'gcs' |
+
+
+## pathlib based operations
+
+| name | description |
+|-|-|
+| `as_posix()` | only for local filesystem, otherwise raise an `PathlibfsException` |
+| `chmod(mode: int)` | only for local filesystem, otherwise raise an `PathlibfsException` |
+| `group()` | only for local filesystem, otherwise raise an `PathlibfsException` |
+| `is_mount()` | only for local filesystem, otherwise raise an `PathlibfsException` |
+| `is_symlink()` | only for local filesystem, otherwise raise an `PathlibfsException` |
+| `is_socket()` | only for local filesystem, otherwise raise an `PathlibfsException` |
+| `is_fifo()` | only for local filesystem, otherwise raise an `PathlibfsException` |
+| `is_block_device()` | only for local filesystem, otherwise raise an `PathlibfsException` |
+| `is_char_device()` | only for local filesystem, otherwise raise an `PathlibfsException` |
+| `owner()` | only for local filesystem, otherwise raise an `PathlibfsException` |
+| `symlink_to(target: PathLike)` | only for local filesystem, otherwise raise an `PathlibfsException` |
+| `resolve()` | only for local filesystem, otherwise return `self` |
+| `is_absolute()` | only for local filesystem, otherwise return True |
+| `is_reserved()` | only for local filesystem, otherwise return False |
+| `joinpath(*p)` | same as pathlib |
+| `match(pattern: str)` | same as pathlib |
+| `with_name(name: str)` | same as pathlib |
+| `with_suffix(suffix: str)` | same as pathlib |
+| `read_bytes()` | same as pathlib |
+| `read_text()` | same as pathlib |
+| `write_text(data)` | same as pathlib |
+| `write_bytes(data)` | same as pathlib |
+| `is_dir()` | same as pathlib |
+| `is_file()` | same as pathlib |
+| `unlink()` | same as pathlib |
+| `relative_to(path: PathLike)` | same as pathlib, but **return str**. `path == other / path.relative_to(other)` |
+| `iterdir(**kwargs)` | same as pathlib. It's just an wrapper of ls(), **it's not efficient.** Use `ls()`. |
+| `stat()` | alias of info. **It's not same as pathlib**, but fsspec's `info()` |
+| `rglob(pattern, **kwargs)` | same meaning as pathlib, and accept fsspec's `glob()` |
+
+## fsspec based mathods
+
+| name | description |
+|-|-|
+| `ls(**kwargs)` | same as fsspec |
+| `listdir()` | alias of ls |
+| `find(maxdepth: Optional[int] = None, withdirs: bool = False, **kwargs)` | same as fsspec |
+| `glob(pattern, **kwargs)` | same as fsspec |
+| `expand_path(recursive: bool = False, maxdepth: Optional[int] = None, **kwargs)` | same as fsspec |
+| `walk(maxdepth: Optional[int] = None, **kwargs)` | same as `os.walk` and fsspec's `walk`, yield `(dirpath, dirnames, filenames)`. And `dirpath` is `Path` instance. |
+| `exists(**kwargs)` | same as fsspec |
+| `isdir()` | same as fsspec |
+| `isfile()` | same as fsspec |
+| `lexists()` | same as fsspec |
+| `ukey()` | same as fsspec |
+| `checksum()` | same as fsspec |
+| `sign(expiration: int = 100, **kwargs)` | same as fsspec |
+| `size()` | same as fsspec |
+| `created()` | same as fsspec |
+| `modified()` | same as fsspec |
+| `du(total: bool = True, maxdepth: Optional[int] = None, **kwargs)` | same as fsspec |
+| `disk_usage()` | alias of du |
+| `info(**kwargs)` | same as fsspec |
+| `open()` | same as fsspec |
+| `cat(recursive: bool = False, on_error: str = "raise", **kwargs)` | same as fsspec |
+| `read_block(offset: int, length: int, delimiter: Optional[bytes] = None)` | same as fsspec |
+| `head(size: int = 1024)` | same as fsspec |
+| `tail(size: int = 1024)` | same as fsspec |
+| `mkdir(parents: bool = False, exist_ok: bool = False, **kwargs)` | same as fsspec |
+| `makedir()` | alias of mkdir |
+| `makedirs(exist_ok: bool = False, **kwargs)` | same as `mkdir(parents=True)` |
+| `mkdirs()` | alias of makedirs |
+| `touch(mode: int = 0o666, exist_ok: bool = True, truncate: bool = False, **kwargs) | same as fsspec |
+| `pipe_file(data)` | same as fsspec |
+| `rm_file()` | same as fsspec |
+| `rm(recursive: bool = False, maxdepth: Optional[int] = None)` | same as fsspec |
+| `delete()` | alias of rm |
+| `invalidate_cache()` | same as fsspec |
+| `clear_instance_cache()` | same as fsspec |
+| `copy(dst: PathLike, recursive: bool = False, on_error: Optional[str] = None, **kwargs)` | copy the path to dst. `copy()` can handle any protocol combinations so you don't need to call `put()` or `get()` for almost all cases. |
+| `cp()` | alias of copy |
+| `move(dst: PathLike, recursive=False, maxdepth=None, **kwargs)` | similar to copy, but delete source path after copy. |
+| `mv()`, `rename()`, `replace() | alias of move |
+| `put(target: PathLike, recursive: bool = False, callback=fsspec.callbacks._DEFAULT_CALLBACK, **kwargs)` | Upload **local** target to the path. |
+| `upload()` | alias of put |
+| `get(arget: PathLike, recursive: bool = False, callback=fsspec.callbacks._DEFAULT_CALLBACK, **kwargs)` | Downalod the path into **local** target. |
+| `download()` | alias of get |
+
+## others
+
+| name | description |
+|-|-|
+| `islocal()` | True if protocol is local filesystem. |
+| `clone(path: Optional[str] = None)` | copy self instance with different path (optional). |
+| `samefile(target: PathLike)` | same as `self == target` |
+
+
+# How to test
+
+Start mock server for testing.
+
+```
+docker-compose up -d
+```
+
+Run test:
+```
+pytest
+```
```

