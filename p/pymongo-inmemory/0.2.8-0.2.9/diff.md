# Comparing `tmp/pymongo_inmemory-0.2.8.tar.gz` & `tmp/pymongo_inmemory-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymongo_inmemory-0.2.8.tar", last modified: Fri May 13 07:26:40 2022, max compression
+gzip compressed data, was "pymongo_inmemory-0.2.9.tar", last modified: Sun Oct  2 20:47:13 2022, max compression
```

## Comparing `pymongo_inmemory-0.2.8.tar` & `pymongo_inmemory-0.2.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1031 2022-05-13 07:26:08.025413 pymongo_inmemory-0.2.8/LICENSE
--rw-r--r--   0        0        0     8383 2022-05-13 07:26:08.025413 pymongo_inmemory-0.2.8/README.md
--rw-r--r--   0        0        0      155 2022-05-13 07:26:08.025413 pymongo_inmemory-0.2.8/pymongo_inmemory/__init__.py
--rw-r--r--   0        0        0      612 2022-05-13 07:26:08.025413 pymongo_inmemory-0.2.8/pymongo_inmemory/_pim.py
--rw-r--r--   0        0        0     2631 2022-05-13 07:26:08.025413 pymongo_inmemory-0.2.8/pymongo_inmemory/_utils.py
--rw-r--r--   0        0        0     1104 2022-05-13 07:26:08.025413 pymongo_inmemory-0.2.8/pymongo_inmemory/downloader/README.md
--rw-r--r--   0        0        0     6289 2022-05-13 07:26:08.025413 pymongo_inmemory-0.2.8/pymongo_inmemory/downloader/__init__.py
--rw-r--r--   0        0        0      149 2022-05-13 07:26:08.025413 pymongo_inmemory-0.2.8/pymongo_inmemory/downloader/__main__.py
--rw-r--r--   0        0        0    23107 2022-05-13 07:26:08.025413 pymongo_inmemory-0.2.8/pymongo_inmemory/downloader/_patterns.py
--rw-r--r--   0        0        0     2562 2022-05-13 07:26:08.025413 pymongo_inmemory-0.2.8/pymongo_inmemory/downloader/_urls.py
--rw-r--r--   0        0        0     2643 2022-05-13 07:26:08.025413 pymongo_inmemory-0.2.8/pymongo_inmemory/downloader/check_urls.py
--rw-r--r--   0        0        0     6048 2022-05-13 07:26:08.025413 pymongo_inmemory-0.2.8/pymongo_inmemory/mongod.py
--rw-r--r--   0        0        0     1386 2022-05-13 07:26:08.025413 pymongo_inmemory-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     9313 2022-05-13 07:26:40.359034 pymongo_inmemory-0.2.8/setup.py
--rw-r--r--   0        0        0     9679 2022-05-13 07:26:40.359897 pymongo_inmemory-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1031 2022-10-02 20:46:39.174609 pymongo_inmemory-0.2.9/LICENSE
+-rw-r--r--   0        0        0     8383 2022-10-02 20:46:39.174609 pymongo_inmemory-0.2.9/README.md
+-rw-r--r--   0        0        0      155 2022-10-02 20:46:39.178609 pymongo_inmemory-0.2.9/pymongo_inmemory/__init__.py
+-rw-r--r--   0        0        0      612 2022-10-02 20:46:39.178609 pymongo_inmemory-0.2.9/pymongo_inmemory/_pim.py
+-rw-r--r--   0        0        0     2631 2022-10-02 20:46:39.178609 pymongo_inmemory-0.2.9/pymongo_inmemory/_utils.py
+-rw-r--r--   0        0        0     1104 2022-10-02 20:46:39.178609 pymongo_inmemory-0.2.9/pymongo_inmemory/downloader/README.md
+-rw-r--r--   0        0        0     6310 2022-10-02 20:46:39.178609 pymongo_inmemory-0.2.9/pymongo_inmemory/downloader/__init__.py
+-rw-r--r--   0        0        0      149 2022-10-02 20:46:39.178609 pymongo_inmemory-0.2.9/pymongo_inmemory/downloader/__main__.py
+-rw-r--r--   0        0        0    23107 2022-10-02 20:46:39.178609 pymongo_inmemory-0.2.9/pymongo_inmemory/downloader/_patterns.py
+-rw-r--r--   0        0        0     2571 2022-10-02 20:46:39.178609 pymongo_inmemory-0.2.9/pymongo_inmemory/downloader/_urls.py
+-rw-r--r--   0        0        0     2643 2022-10-02 20:46:39.178609 pymongo_inmemory-0.2.9/pymongo_inmemory/downloader/check_urls.py
+-rw-r--r--   0        0        0     6048 2022-10-02 20:46:39.178609 pymongo_inmemory-0.2.9/pymongo_inmemory/mongod.py
+-rw-r--r--   0        0        0     1386 2022-10-02 20:46:39.178609 pymongo_inmemory-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     9313 2022-10-02 20:47:13.660418 pymongo_inmemory-0.2.9/setup.py
+-rw-r--r--   0        0        0     9679 2022-10-02 20:47:13.661315 pymongo_inmemory-0.2.9/PKG-INFO
```

### Comparing `pymongo_inmemory-0.2.8/LICENSE` & `pymongo_inmemory-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pymongo_inmemory-0.2.8/README.md` & `pymongo_inmemory-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `pymongo_inmemory-0.2.8/pymongo_inmemory/_pim.py` & `pymongo_inmemory-0.2.9/pymongo_inmemory/_pim.py`

 * *Files identical despite different names*

### Comparing `pymongo_inmemory-0.2.8/pymongo_inmemory/_utils.py` & `pymongo_inmemory-0.2.9/pymongo_inmemory/_utils.py`

 * *Files identical despite different names*

### Comparing `pymongo_inmemory-0.2.8/pymongo_inmemory/downloader/README.md` & `pymongo_inmemory-0.2.9/pymongo_inmemory/downloader/README.md`

 * *Files identical despite different names*

### Comparing `pymongo_inmemory-0.2.8/pymongo_inmemory/downloader/__init__.py` & `pymongo_inmemory-0.2.9/pymongo_inmemory/downloader/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -122,31 +122,27 @@
         logger.info("Extractiong finished.")
 
 
 def _collect_archive_name(url):
     return url.split("/")[-1]
 
 
-def _get_mongod():
+def _get_mongod(version):
     for binfile_path in glob.iglob(
-        path.join(_extract_folder(), "**/bin/*"), recursive=True
+        path.join(_extract_folder(), f"**{version}**/bin/*"), recursive=True
     ):
         binfile_name = path.basename(binfile_path)
         try:
             binfile_name.index("mongod")
         except ValueError:
             continue
         else:
             return binfile_path
 
 
-def _has_mongod():
-    return _get_mongod() is not None
-
-
 def download(os_name=None, version=None, os_ver=None, ignore_cache=False):
     """Download MongoDB binaries.
     Available versions are collected form this URL:
     https://www.mongodb.com/download-center/community/releases
     and this one:
     https://www.mongodb.com/download-center/community/releases/archive
 
@@ -182,15 +178,15 @@
             "Starting from MongoDB 4.0.23 "
             "there isn't a generic Linux version of MongoDB"
             ))
 
     if os_ver is None:
         os_ver = conf("os_version")
 
-    dl_url = conf("download_url", best_url(
+    dl_url, downloaded_version = conf("download_url", best_url(
         os_name,
         version=version,
         os_ver=os_ver
     ))
 
     logger.debug("Downloading MongoD from {}".format(dl_url))
     dl_folder = _download_folder()
@@ -199,11 +195,11 @@
     should_ignore_cache = bool(conf("ignore_cache", ignore_cache))
 
     if should_ignore_cache or not path.isfile(archive_file):
         logger.info("Archive file is not found, {}".format(archive_file))
         _download_file(dl_url, archive_file)
         _extract(archive_file)
 
-    if not _has_mongod():
+    if _get_mongod(downloaded_version) is None:
         _extract(archive_file)
 
-    return path.dirname(_get_mongod())
+    return path.dirname(_get_mongod(downloaded_version))
```

### Comparing `pymongo_inmemory-0.2.8/pymongo_inmemory/downloader/_patterns.py` & `pymongo_inmemory-0.2.9/pymongo_inmemory/downloader/_patterns.py`

 * *Files identical despite different names*

### Comparing `pymongo_inmemory-0.2.8/pymongo_inmemory/downloader/_urls.py` & `pymongo_inmemory-0.2.9/pymongo_inmemory/downloader/_urls.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     elif patch not in version_branch[major][minor]["patches"]:
         patch = max(version_branch[major][minor]["patches"])
 
     logger.info("Requested MongoDB version {}, found version: {}.{}.{}".format(
         version, major, minor, patch
     ))
     version = "{}.{}.{}".format(major, minor, patch)
-    return version_branch[major][minor]["url"].format(version)
+    return version_branch[major][minor]["url"].format(version), version
 
 
 def expand_url_tree(tree):
     for os_name, os_leaf in tree.items():
         for os_version, version_leaf in os_leaf.items():
             for major, major_leaf in version_leaf.items():
                 for minor, minor_leaf in major_leaf.items():
```

### Comparing `pymongo_inmemory-0.2.8/pymongo_inmemory/downloader/check_urls.py` & `pymongo_inmemory-0.2.9/pymongo_inmemory/downloader/check_urls.py`

 * *Files identical despite different names*

### Comparing `pymongo_inmemory-0.2.8/pymongo_inmemory/mongod.py` & `pymongo_inmemory-0.2.9/pymongo_inmemory/mongod.py`

 * *Files identical despite different names*

### Comparing `pymongo_inmemory-0.2.8/pyproject.toml` & `pymongo_inmemory-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pymongo_inmemory"
-version = "0.2.8"
+version = "0.2.9"
 description = "A mongo mocking library with an ephemeral MongoDB running in memory."
 authors = [
     "Kaizen Dorks <kaizendorks@gmail.com>",
 ]
 maintainers = [
     "Ertugrul Karademir <ekarademir@gmail.com>",
     "Daniel Jimenez Garcia",
```

### Comparing `pymongo_inmemory-0.2.8/setup.py` & `pymongo_inmemory-0.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pymongo']
 
 setup_kwargs = {
     'name': 'pymongo-inmemory',
-    'version': '0.2.8',
+    'version': '0.2.9',
     'description': 'A mongo mocking library with an ephemeral MongoDB running in memory.',
     'long_description': "[![PyPI\nversion](https://badge.fury.io/py/pymongo-inmemory.svg)](https://badge.fury.io/py/pymongo-inmemory)\n\n# pymongo_inmemory\nA mongo mocking library with an ephemeral MongoDB running in memory.\n\n## Installation\n```bash\npip install pymongo-inmemory\n```\n\n## Usage\n### Configure\nThere are several ways you can configure `pymongo_inmemory`.\n\n1. Insert a new section titled `pymongo_inmemory` to your project's `setup.cfg`\nversion you want to spin up:\n    ```ini\n    [pymongo_inmemory]\n    operating_system = ubuntu\n    os_version = 18\n    mongod_port = 27019\n    ```\n2. Define an `ALL_CAPS` environment variables with prefix `PYMONGOIM__` (attention to trailing double\n   underscores.) For instance, to override the port, set up an environment variable\n   `PYMONGOIM__MONGOD_PORT`.\n\n### Import and use\n`pymongo_inmemory` wraps the client class `MongoClient` that comes from `pymongo` and configures with an ephemeral MongoDB server.\nYou can import this `MongoClient` from `pymongo_inmemory` instead of `pymongo` and use it to perform tests:\n\n```python\nfrom pymongo_inmemory import MongoClient\n\nclient = MongoClient()  # No need to provide host\ndb = client['testdb']\ncollection = db['test-collection']\n# etc., etc.\nclient.close()\n\n# Also usable with context manager\nwith MongoClient() as client:\n    # do stuff\n```\n\n## Configuration\n| Config param       | Description                               | Optional? | Default                                          |\n|--------------------|-------------------------------------------|-----------|--------------------------------------------------|\n| `mongo_version`    | Which MongoD version to download and use. | Yes       | Latest for the OS                                            |\n| `mongod_port`      | Override port preference.                 | Yes       | Automatically picked between `27017` and `28000` after testing availability                |\n| `operating_system` | This makes sense for Linux setting, where there are several flavours         | Yes       | Automatically determined (Generic for Linux)*           |\n| `os_version`       | If an operating system has several versions use this parameter to select one | Yes       | Latest versoin of the OS will be selected from the list |\n| `download_url`     | If set, it won't attempt to determine which MongoDB to download. However there won't be a fallback either.| Yes       | Automatically determined from given parameters and using [internal URL bank](pymongo_inmemory/downloader/_patterns.py)**|\n| `ignore_cache`     | Even if there is a downloaded version in the cache, download it again. | Yes       | False               |\n||||\n\n* ****Note 1:*** Generic Linux version offering for MongoDB ends with version **4.0.23**. If the operating system is just `linux` and if selected MongoDB version is higher, it will default to `4.0.23`.\n* *****Note 2:*** URL bank is filled with URLs collected from [release list](https://www.mongodb.com/download-center/community/releases) and [archived released list](https://www.mongodb.com/download-center/community/releases/archive), so if a version is not in the bank you can use the same list to provide an official download link.\n\n\n## Available MongoDB versions\nThere is an internal [URL bank](pymongo_inmemory/downloader/_patterns.py) that is filled with URLs collected from\n* [release list](https://www.mongodb.com/download-center/community/releases) and\n* [archived released list](https://www.mongodb.com/download-center/community/releases/archive)\n\nBelow table is a summary of possible setting for `operating_system`, `os_version` and available MongoDB versions for\nthem to set as `mongo_version` at `major.minor` level.\n\nNote that, not all `major.minor.patch` level is available for all OS versions. For exact patch level range, either see\nrelease pages of MongoDB or have a look at the internal [URL bank](pymongo_inmemory/downloader/_patterns.py).\n\n| `operating_system` | `os_version` | MongoDB versions (`major.minor`)|\n|-|-|-|\n|`osx`|`generic`*| `2.6`, `3.0`, `3.2`, `3.4`, `3.6`, `4.0`, `4.2`, `4.4`, `5.0`|\n|`windows`|`generic`*| `2.6`, `3.0`, `3.2`, `3.4`, `3.6`, `4.0`, `4.2`, `4.4`, `5.0`|\n|`linux`|`generic`*| `2.6`, `3.0`, `3.2`, `3.4`, `3.6`, `4.0`|\n|`amazon`|`1`| `3.0`, `3.2`, `3.4`, `3.6`, `4.0`, `4.2`, `4.4`, `5.0`|\n|`amazon`|`2`| `3.6`, `4.0`, `4.2`, `4.4`, `5.0`|\n|`debian`|`7`| `3.0`, `3.2`, `3.4`, `3.6`|\n|`debian`|`8`| `3.2`, `3.4`, `3.6`, `4.0`|\n|`debian`|`9`| `3.6`, `4.0`, `4.2`, `4.4`, `4.5`, `4.6`, `5.0`|\n|`debian`|`10`| `4.2`, `4.4`, `4.5`, `4.6`, `5.0`|\n|`debian`|`11`| `5.0`|\n|`rhel`|`5`| `3.0`, `3.2`|\n|`rhel`|`6`| `3.0`, `3.2`, `3.4`, `3.6`, `4.0`, `4.2`, `4.4`|\n|`rhel`|`7`| `3.0`, `3.2`, `3.4`, `3.6`, `4.0`, `4.2`, `4.4`, `5.0`|\n|`rhel`|`8`| `3.6`, `4.0`, `4.2`, `4.4`, `5.0`|\n|`suse`|`11`| `3.0`, `3.2`, `3.4`, `3.6`|\n|`suse`|`12`| `3.2`, `3.4`, `3.6`, `4.0`, `4.2`, `4.4`, `5.0`|\n|`suse`|`15`| `4.2`, `4.4`, `5.0`|\n|`ubuntu`|`12`| `3.0`, `3.2`, `3.4`, `3.6`|\n|`ubuntu`|`14`| `3.0`, `3.2`, `3.4`, `3.6`, `4.0`|\n|`ubuntu`|`16`| `3.2`, `3.4`, `3.6`, `4.0`, `4.2`, `4.4`|\n|`ubuntu`|`18`| `3.6`, `4.0`, `4.2`, `4.4`, `5.0`|\n|`ubuntu`|`20`| `4.4`, `5.0`|\n|`sunos`|`5`| `2.6`, `3.0`, `3.2`, `3.4`|\n||||\n\n****Note:*** No need to specify `generic`, as it will be chosen automatically since it's the only version for that OS.\n\n### How do we determine which MongoDB to download?\nThere are two (three if it's a Linux flavour) bits of information we need to determine a MongoDB:\noperating system and MongoDB version.\n\n**Note:** You can always set `download_url` to provide an exact URL to download from.\n\n#### Operating System detection\nPython has limited tools in its standard library to determine the exact version of the operating\nsystem and operating system version. `pymongo_inmemory` basically reads output of [`platform.system()`](platform.system())\nto determine if underlying OS is Linux, MacOS or Windows.\n\nFor Windows and MacOS, it will download only one flavour of OS for a particular MongoDB version (64bit and, for Windows, Windows Server version if there is one.)\nHowever, Linux has many flavours. Up to MongoDB `4.0.23`, a MongoDB for a generic Linux OS can still be downloaded, but for later\nversions of MongoDB, there are no such builds, hence you will need to explicitly set `operating_system`\nparameter if you want to use MongoDB versions higher than that.\n\nOperating system detection behaviour of `pymongo_inmemory` might change in the future, if there is a demand for more **magic**,\nbut for now we are keeping things simple.\n\n#### Deciding MongoDB version\n* If no version is provided, highest version of MongoDB for the operating system is selected.\n* If only a **major** version is given, like `4`, then highest `minor.patch` version is selected, like 4.4.4.\n* If only **major.minor** version is given, like `4.0`, then highest `patch` version is selected, like 4.0.23.\n* If exact **major.minor.patch** version is given, like `4.0.22`, then that version is selected.\n* If patch version is not found. like `4.0.50`, highest `patch` version is selected, like `4.0.23`.\n* If minor version is not found. like `3.90.50`, highest `minor.patch` version is selected, like `3.6.22`.\n* If major version is not found. like `1.0.0`, highest `major.minor.patch` version is selected, like `4.4.4`.\n\n## Supported Python versions\nSince few development tools only support Python version 3.6 and above, all testing and tooling done\nfrom that version up.\n\nThis also limits the minimum Python version of tested features. However there shouldn't\nbe a hard limitation to use Python 3.5. We recommend upgrading older Python versions than that.\n\n## Development\nProject is set up to develop with [poetry](https://python-poetry.org/). We rely on\n[pyenv](https://github.com/pyenv/pyenv#installation) to maintain the minimum supported\nPython version.\n\nAfter installing `pyenv`, `poetry`, and cloning the repo, create the shell and install\nall package requirements:\n\n```bash\npyenv install --skip-existing\npoetry install --no-root\npoetry shell\n```\n\nRun the tests:\n```bash\npytest\n```\n\nIf on NIX systems you can run further tests:\n```bash\nbash tests/integrity/test_integrity.sh\n```\n\n### Adding a new MongoDB version\nFollow the guide [here](pymongo_inmemory/downloader/README.md).\n\n### See how you can wet your feet\nCheck out [good first issues](https://github.com/kaizendorks/pymongo_inmemory/contribute).\n",
     'author': 'Kaizen Dorks',
     'author_email': 'kaizendorks@gmail.com',
     'maintainer': 'Ertugrul Karademir',
     'maintainer_email': 'ekarademir@gmail.com',
     'url': 'https://github.com/kaizendorks/pymongo_inmemory',
```

### Comparing `pymongo_inmemory-0.2.8/PKG-INFO` & `pymongo_inmemory-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymongo-inmemory
-Version: 0.2.8
+Version: 0.2.9
 Summary: A mongo mocking library with an ephemeral MongoDB running in memory.
 Home-page: https://github.com/kaizendorks/pymongo_inmemory
 License: MIT
 Keywords: mongodb,testing,pymongo
 Author: Kaizen Dorks
 Author-email: kaizendorks@gmail.com
 Maintainer: Ertugrul Karademir
```

