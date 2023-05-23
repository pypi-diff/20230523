# Comparing `tmp/democracy-1.0.20.tar.gz` & `tmp/democracy-1.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "democracy-1.0.20.tar", last modified: Tue May 23 06:51:06 2023, max compression
+gzip compressed data, was "democracy-1.0.21.tar", last modified: Tue May 23 06:55:09 2023, max compression
```

## Comparing `democracy-1.0.20.tar` & `democracy-1.0.21.tar`

### file list

```diff
@@ -1,9 +1,10 @@
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-23 06:51:06.535693 democracy-1.0.20/
--rw-rw-r--   0 a         (1000) a         (1000)      762 2023-05-23 06:51:06.535693 democracy-1.0.20/PKG-INFO
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-23 06:51:06.531693 democracy-1.0.20/democracy.egg-info/
--rw-rw-r--   0 a         (1000) a         (1000)      762 2023-05-23 06:51:06.000000 democracy-1.0.20/democracy.egg-info/PKG-INFO
--rw-rw-r--   0 a         (1000) a         (1000)      146 2023-05-23 06:51:06.000000 democracy-1.0.20/democracy.egg-info/SOURCES.txt
--rw-rw-r--   0 a         (1000) a         (1000)        1 2023-05-23 06:51:06.000000 democracy-1.0.20/democracy.egg-info/dependency_links.txt
--rw-rw-r--   0 a         (1000) a         (1000)       10 2023-05-23 06:51:06.000000 democracy-1.0.20/democracy.egg-info/top_level.txt
--rw-r--r--   0 a         (1000) a         (1000)     5585 2023-05-23 06:46:26.000000 democracy-1.0.20/pyproject.toml
--rw-rw-r--   0 a         (1000) a         (1000)       38 2023-05-23 06:51:06.535693 democracy-1.0.20/setup.cfg
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-23 06:55:09.044192 democracy-1.0.21/
+-rw-rw-r--   0 a         (1000) a         (1000)    40852 2023-05-23 06:55:09.044192 democracy-1.0.21/PKG-INFO
+-rw-rw-r--   0 a         (1000) a         (1000)    40089 2023-05-23 06:53:15.000000 democracy-1.0.21/README.md
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-23 06:55:09.040192 democracy-1.0.21/democracy.egg-info/
+-rw-rw-r--   0 a         (1000) a         (1000)    40852 2023-05-23 06:55:08.000000 democracy-1.0.21/democracy.egg-info/PKG-INFO
+-rw-rw-r--   0 a         (1000) a         (1000)      156 2023-05-23 06:55:09.000000 democracy-1.0.21/democracy.egg-info/SOURCES.txt
+-rw-rw-r--   0 a         (1000) a         (1000)        1 2023-05-23 06:55:08.000000 democracy-1.0.21/democracy.egg-info/dependency_links.txt
+-rw-rw-r--   0 a         (1000) a         (1000)       10 2023-05-23 06:55:08.000000 democracy-1.0.21/democracy.egg-info/top_level.txt
+-rw-r--r--   0 a         (1000) a         (1000)     5601 2023-05-23 06:54:47.000000 democracy-1.0.21/pyproject.toml
+-rw-rw-r--   0 a         (1000) a         (1000)       38 2023-05-23 06:55:09.044192 democracy-1.0.21/setup.cfg
```

### Comparing `democracy-1.0.20/pyproject.toml` & `democracy-1.0.21/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "democracy"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.0.20"  # Required
+version = "1.0.21"  # Required
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "Trying to help with democracy, see https://github.com/gregoryc/democracy"  # Optional
 
 # This is an optional longer description of your project that represents
@@ -124,14 +124,14 @@
 # which executes the function `main` from this package when invoked.
 
 # This is configuration specific to the `setuptools` build backend.
 # If you are using a different build backend, you will need to change this.
 [tool.setuptools]
 # If there are data files included in your packages that need to be
 # installed, specify them here.
-package-data = {}
+package-data = {"sample" = ["*"]}
 
 [build-system]
 # These are the assumed default build requirements from pip:
 # https://pip.pypa.io/en/stable/reference/pip/#pep-517-and-518-support
 requires = ["setuptools>=43.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
```

