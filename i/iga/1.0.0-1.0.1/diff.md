# Comparing `tmp/iga-1.0.0.tar.gz` & `tmp/iga-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iga-1.0.0.tar", last modified: Fri May 19 00:22:15 2023, max compression
+gzip compressed data, was "iga-1.0.1.tar", last modified: Mon May 22 20:39:47 2023, max compression
```

## Comparing `iga-1.0.0.tar` & `iga-1.0.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-05-19 00:22:15.678299 iga-1.0.0/
--rw-r--r--   0 mhucka     (503) staff       (20)     1527 2023-03-16 00:12:10.000000 iga-1.0.0/LICENSE
--rw-r--r--   0 mhucka     (503) staff       (20)    37613 2023-05-19 00:22:15.678414 iga-1.0.0/PKG-INFO
--rw-r--r--   0 mhucka     (503) staff       (20)    36707 2023-05-18 20:14:21.000000 iga-1.0.0/README.md
-drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-05-19 00:22:15.667889 iga-1.0.0/iga/
--rw-r--r--   0 mhucka     (503) staff       (20)     1458 2023-05-18 19:32:51.000000 iga-1.0.0/iga/__init__.py
--rw-r--r--   0 mhucka     (503) staff       (20)      905 2023-03-16 00:12:36.000000 iga-1.0.0/iga/__main__.py
--rw-r--r--   0 mhucka     (503) staff       (20)    34712 2023-05-18 01:10:50.000000 iga-1.0.0/iga/cli.py
--rw-r--r--   0 mhucka     (503) staff       (20)     3317 2023-03-27 20:05:34.000000 iga-1.0.0/iga/data_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)     2859 2023-04-10 21:11:51.000000 iga-1.0.0/iga/doi.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1252 2023-05-17 19:19:30.000000 iga-1.0.0/iga/exceptions.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1514 2023-05-17 19:19:30.000000 iga-1.0.0/iga/exit_codes.py
--rw-r--r--   0 mhucka     (503) staff       (20)    15499 2023-05-09 20:43:53.000000 iga-1.0.0/iga/github.py
--rw-r--r--   0 mhucka     (503) staff       (20)     4901 2023-04-26 04:08:12.000000 iga-1.0.0/iga/id_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)    18504 2023-05-18 01:10:50.000000 iga-1.0.0/iga/invenio.py
--rw-r--r--   0 mhucka     (503) staff       (20)     2058 2023-04-20 00:58:38.000000 iga-1.0.0/iga/json_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)   242887 2023-03-08 23:12:16.000000 iga-1.0.0/iga/licenses.py
--rw-r--r--   0 mhucka     (503) staff       (20)    69900 2023-05-16 20:21:25.000000 iga-1.0.0/iga/metadata.py
--rw-r--r--   0 mhucka     (503) staff       (20)    14563 2023-04-26 04:08:12.000000 iga-1.0.0/iga/name_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)     5273 2023-04-08 02:44:39.000000 iga-1.0.0/iga/orcid.py
--rw-r--r--   0 mhucka     (503) staff       (20)     5147 2023-04-08 02:44:39.000000 iga-1.0.0/iga/reference.py
--rw-r--r--   0 mhucka     (503) staff       (20)     3969 2023-04-08 02:44:39.000000 iga-1.0.0/iga/ror.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1624 2023-04-08 02:44:39.000000 iga-1.0.0/iga/text_utils.py
-drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-05-19 00:22:15.675952 iga-1.0.0/iga.egg-info/
--rw-r--r--   0 mhucka     (503) staff       (20)    37613 2023-05-19 00:22:15.000000 iga-1.0.0/iga.egg-info/PKG-INFO
--rw-r--r--   0 mhucka     (503) staff       (20)      930 2023-05-19 00:22:15.000000 iga-1.0.0/iga.egg-info/SOURCES.txt
--rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-05-19 00:22:15.000000 iga-1.0.0/iga.egg-info/dependency_links.txt
--rw-r--r--   0 mhucka     (503) staff       (20)       58 2023-05-19 00:22:15.000000 iga-1.0.0/iga.egg-info/entry_points.txt
--rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-05-19 00:22:15.000000 iga-1.0.0/iga.egg-info/not-zip-safe
--rw-r--r--   0 mhucka     (503) staff       (20)      657 2023-05-19 00:22:15.000000 iga-1.0.0/iga.egg-info/requires.txt
--rw-r--r--   0 mhucka     (503) staff       (20)        4 2023-05-19 00:22:15.000000 iga-1.0.0/iga.egg-info/top_level.txt
--rw-r--r--   0 mhucka     (503) staff       (20)     1095 2023-05-19 00:22:15.678737 iga-1.0.0/setup.cfg
--rwxr-xr-x   0 mhucka     (503) staff       (20)     1708 2023-04-08 01:05:22.000000 iga-1.0.0/setup.py
-drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-05-19 00:22:15.678201 iga-1.0.0/tests/
--rw-r--r--   0 mhucka     (503) staff       (20)     6117 2023-05-18 01:03:27.000000 iga-1.0.0/tests/test_cli.py
--rw-r--r--   0 mhucka     (503) staff       (20)     4481 2023-03-27 19:38:15.000000 iga-1.0.0/tests/test_data_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1417 2023-03-17 23:21:28.000000 iga-1.0.0/tests/test_doi.py
--rw-r--r--   0 mhucka     (503) staff       (20)      686 2023-03-02 15:36:12.000000 iga-1.0.0/tests/test_exceptions.py
--rw-r--r--   0 mhucka     (503) staff       (20)      177 2023-01-13 03:19:50.000000 iga-1.0.0/tests/test_exit_codes.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1446 2023-04-07 01:26:59.000000 iga-1.0.0/tests/test_github.py
--rw-r--r--   0 mhucka     (503) staff       (20)     3015 2023-04-07 01:20:36.000000 iga-1.0.0/tests/test_github_mocks.py
--rw-r--r--   0 mhucka     (503) staff       (20)     3666 2023-04-26 04:08:12.000000 iga-1.0.0/tests/test_id_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)      641 2022-12-08 00:11:08.000000 iga-1.0.0/tests/test_init.py
--rw-r--r--   0 mhucka     (503) staff       (20)    49214 2023-04-20 00:58:38.000000 iga-1.0.0/tests/test_is_person.py
--rw-r--r--   0 mhucka     (503) staff       (20)      912 2023-03-02 15:16:32.000000 iga-1.0.0/tests/test_licenses.py
--rw-r--r--   0 mhucka     (503) staff       (20)     4408 2023-04-20 00:58:38.000000 iga-1.0.0/tests/test_name_splitting.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1829 2023-04-20 00:58:38.000000 iga-1.0.0/tests/test_name_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1054 2023-03-18 00:09:09.000000 iga-1.0.0/tests/test_orcid.py
--rw-r--r--   0 mhucka     (503) staff       (20)     5997 2023-05-17 19:19:30.000000 iga-1.0.0/tests/test_record_from_codemeta.py
--rw-r--r--   0 mhucka     (503) staff       (20)     6026 2023-03-02 23:04:18.000000 iga-1.0.0/tests/test_reference.py
--rw-r--r--   0 mhucka     (503) staff       (20)      947 2023-03-18 00:05:51.000000 iga-1.0.0/tests/test_ror.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1375 2023-04-06 22:54:59.000000 iga-1.0.0/tests/test_text_utils.py
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-05-22 20:39:47.395655 iga-1.0.1/
+-rw-r--r--   0 mhucka     (503) staff       (20)     1527 2023-05-22 18:03:26.000000 iga-1.0.1/LICENSE
+-rw-r--r--   0 mhucka     (503) staff       (20)    37612 2023-05-22 20:39:47.395761 iga-1.0.1/PKG-INFO
+-rw-r--r--   0 mhucka     (503) staff       (20)    36706 2023-05-22 18:03:26.000000 iga-1.0.1/README.md
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-05-22 20:39:47.391840 iga-1.0.1/iga/
+-rw-r--r--   0 mhucka     (503) staff       (20)     1458 2023-05-22 20:36:28.000000 iga-1.0.1/iga/__init__.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      905 2023-05-22 18:03:26.000000 iga-1.0.1/iga/__main__.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    34712 2023-05-22 18:03:26.000000 iga-1.0.1/iga/cli.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     3317 2023-05-22 18:03:26.000000 iga-1.0.1/iga/data_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     2859 2023-05-22 18:03:26.000000 iga-1.0.1/iga/doi.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1252 2023-05-22 18:03:26.000000 iga-1.0.1/iga/exceptions.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1514 2023-05-22 18:03:26.000000 iga-1.0.1/iga/exit_codes.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    15499 2023-05-22 18:03:26.000000 iga-1.0.1/iga/github.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     4901 2023-05-22 18:03:26.000000 iga-1.0.1/iga/id_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    18504 2023-05-22 18:03:26.000000 iga-1.0.1/iga/invenio.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     2058 2023-05-22 18:03:26.000000 iga-1.0.1/iga/json_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)   242887 2023-05-22 18:03:26.000000 iga-1.0.1/iga/licenses.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    70400 2023-05-22 20:36:28.000000 iga-1.0.1/iga/metadata.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    14563 2023-05-22 18:03:26.000000 iga-1.0.1/iga/name_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     5273 2023-05-22 18:03:26.000000 iga-1.0.1/iga/orcid.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     5147 2023-05-22 18:03:26.000000 iga-1.0.1/iga/reference.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     3969 2023-05-22 18:03:26.000000 iga-1.0.1/iga/ror.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1624 2023-05-22 18:03:26.000000 iga-1.0.1/iga/text_utils.py
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-05-22 20:39:47.392709 iga-1.0.1/iga.egg-info/
+-rw-r--r--   0 mhucka     (503) staff       (20)    37612 2023-05-22 20:39:47.000000 iga-1.0.1/iga.egg-info/PKG-INFO
+-rw-r--r--   0 mhucka     (503) staff       (20)      930 2023-05-22 20:39:47.000000 iga-1.0.1/iga.egg-info/SOURCES.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-05-22 20:39:47.000000 iga-1.0.1/iga.egg-info/dependency_links.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)       58 2023-05-22 20:39:47.000000 iga-1.0.1/iga.egg-info/entry_points.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-05-22 20:39:47.000000 iga-1.0.1/iga.egg-info/not-zip-safe
+-rw-r--r--   0 mhucka     (503) staff       (20)      657 2023-05-22 20:39:47.000000 iga-1.0.1/iga.egg-info/requires.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)        4 2023-05-22 20:39:47.000000 iga-1.0.1/iga.egg-info/top_level.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)     1095 2023-05-22 20:39:47.396076 iga-1.0.1/setup.cfg
+-rwxr-xr-x   0 mhucka     (503) staff       (20)     1708 2023-05-22 18:03:26.000000 iga-1.0.1/setup.py
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-05-22 20:39:47.395541 iga-1.0.1/tests/
+-rw-r--r--   0 mhucka     (503) staff       (20)     6117 2023-05-22 18:03:26.000000 iga-1.0.1/tests/test_cli.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     4481 2023-05-22 18:03:26.000000 iga-1.0.1/tests/test_data_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1417 2023-05-22 18:03:26.000000 iga-1.0.1/tests/test_doi.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      686 2023-05-22 18:03:26.000000 iga-1.0.1/tests/test_exceptions.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      177 2023-05-22 18:03:26.000000 iga-1.0.1/tests/test_exit_codes.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1446 2023-05-22 18:03:26.000000 iga-1.0.1/tests/test_github.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     3015 2023-05-22 18:03:26.000000 iga-1.0.1/tests/test_github_mocks.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     3666 2023-05-22 18:03:26.000000 iga-1.0.1/tests/test_id_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      641 2023-05-22 18:03:26.000000 iga-1.0.1/tests/test_init.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    49214 2023-05-22 18:03:26.000000 iga-1.0.1/tests/test_is_person.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      912 2023-05-22 18:03:26.000000 iga-1.0.1/tests/test_licenses.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     4408 2023-05-22 18:03:26.000000 iga-1.0.1/tests/test_name_splitting.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1829 2023-05-22 18:03:26.000000 iga-1.0.1/tests/test_name_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1054 2023-05-22 18:03:26.000000 iga-1.0.1/tests/test_orcid.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     5997 2023-05-22 18:03:26.000000 iga-1.0.1/tests/test_record_from_codemeta.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     6026 2023-05-22 18:03:26.000000 iga-1.0.1/tests/test_reference.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      947 2023-05-22 18:03:26.000000 iga-1.0.1/tests/test_ror.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1375 2023-05-22 18:03:26.000000 iga-1.0.1/tests/test_text_utils.py
```

### Comparing `iga-1.0.0/LICENSE` & `iga-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iga-1.0.0/PKG-INFO` & `iga-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iga
-Version: 1.0.0
+Version: 1.0.1
 Summary: InvenioRDM GitHub Archiver
 Home-page: https://github.com/caltechlibrary/iga
 Author: Michael Hucka
 Author-email: helpdesk@library.caltech.edu
 License: https://github.com/caltechlibrary/iga/blob/main/LICENSE
 Project-URL: Source Code, https://github.com/caltechlibrary/iga
 Project-URL: Bug Tracker, https://github.com/caltechlibrary/iga/issues
@@ -56,15 +56,15 @@
 <span style="font-size: 150%">➜</span>
 <img align="middle" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/example-record-landing-page.jpg" width="40%">
 </p>
 
 IGA offers many notable features:
 * Automatic metadata extraction from GitHub plus [`codemeta.json`](https://codemeta.github.io) and [`CITATION.cff`](https://citation-file-format.github.io) files
 * Thorough coverage of [InvenioRDM record metadata](https://inveniordm.docs.cern.ch/reference/metadata) using painstaking procedures
-* Recognition of identifiers in CodeMeta & CFF files: [ORCID](https://orcid.org),, [DOI](https://www.doi.org),  [PMCID](https://www.ncbi.nlm.nih.gov/pmc/about/public-access-info/), and more
+* Recognition of identifiers in CodeMeta & CFF files: [ORCID](https://orcid.org), [DOI](https://www.doi.org),  [PMCID](https://www.ncbi.nlm.nih.gov/pmc/about/public-access-info/), and more
 * Automatic lookup of publication data in [DOI.org](https://www.doi.org), [PubMed]((https://www.ncbi.nlm.nih.gov/pmc/about/public-access-info/)), Google, and other sources
 * Automatic lookup of organization names in [ROR](https://ror.org) (assuming ROR id's are provided)
 * Automatic lookup of human names in [ORCID.org](https://orcid.org) (assuming ORCID id's are provided)
 * Automatic splitting of human names into family & given names using [ML](https://en.wikipedia.org/wiki/Machine_learning) methods
 * Support for InvenioRDM [communities](https://invenio-communities.readthedocs.io/en/latest/)
 * Support for overriding the record that IGA creates, for complete control if you need it
 * Support for using the GitHub API without a [GitHub access token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) in simple cases
```

### Comparing `iga-1.0.0/README.md` & `iga-1.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 <span style="font-size: 150%">➜</span>
 <img align="middle" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/example-record-landing-page.jpg" width="40%">
 </p>
 
 IGA offers many notable features:
 * Automatic metadata extraction from GitHub plus [`codemeta.json`](https://codemeta.github.io) and [`CITATION.cff`](https://citation-file-format.github.io) files
 * Thorough coverage of [InvenioRDM record metadata](https://inveniordm.docs.cern.ch/reference/metadata) using painstaking procedures
-* Recognition of identifiers in CodeMeta & CFF files: [ORCID](https://orcid.org),, [DOI](https://www.doi.org),  [PMCID](https://www.ncbi.nlm.nih.gov/pmc/about/public-access-info/), and more
+* Recognition of identifiers in CodeMeta & CFF files: [ORCID](https://orcid.org), [DOI](https://www.doi.org),  [PMCID](https://www.ncbi.nlm.nih.gov/pmc/about/public-access-info/), and more
 * Automatic lookup of publication data in [DOI.org](https://www.doi.org), [PubMed]((https://www.ncbi.nlm.nih.gov/pmc/about/public-access-info/)), Google, and other sources
 * Automatic lookup of organization names in [ROR](https://ror.org) (assuming ROR id's are provided)
 * Automatic lookup of human names in [ORCID.org](https://orcid.org) (assuming ORCID id's are provided)
 * Automatic splitting of human names into family & given names using [ML](https://en.wikipedia.org/wiki/Machine_learning) methods
 * Support for InvenioRDM [communities](https://invenio-communities.readthedocs.io/en/latest/)
 * Support for overriding the record that IGA creates, for complete control if you need it
 * Support for using the GitHub API without a [GitHub access token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) in simple cases
```

### Comparing `iga-1.0.0/iga/__init__.py` & `iga-1.0.1/iga/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # .............................................................................
 #
 #  ╭────────────────────── Notice ── Notice ── Notice ─────────────────────╮
 #  |    The following values are automatically updated at every release    |
 #  |    by the Makefile. Manual changes to these values will be lost.      |
 #  ╰────────────────────── Notice ── Notice ── Notice ─────────────────────╯
 
-__version__     = '1.0.0'
+__version__     = '1.0.1'
 __description__ = 'InvenioRDM GitHub Archiver'
 __url__         = 'https://github.com/caltechlibrary/iga'
 __author__      = 'Michael Hucka'
 __email__       = 'helpdesk@library.caltech.edu'
 __license__     = 'https://github.com/caltechlibrary/iga/blob/main/LICENSE'
```

### Comparing `iga-1.0.0/iga/__main__.py` & `iga-1.0.1/iga/__main__.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.0/iga/cli.py` & `iga-1.0.1/iga/cli.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.0/iga/data_utils.py` & `iga-1.0.1/iga/data_utils.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.0/iga/doi.py` & `iga-1.0.1/iga/doi.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.0/iga/exceptions.py` & `iga-1.0.1/iga/exceptions.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.0/iga/exit_codes.py` & `iga-1.0.1/iga/exit_codes.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.0/iga/github.py` & `iga-1.0.1/iga/github.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.0/iga/id_utils.py` & `iga-1.0.1/iga/id_utils.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.0/iga/invenio.py` & `iga-1.0.1/iga/invenio.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.0/iga/json_utils.py` & `iga-1.0.1/iga/json_utils.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.0/iga/licenses.py` & `iga-1.0.1/iga/licenses.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.0/iga/metadata.py` & `iga-1.0.1/iga/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1326,15 +1326,15 @@
                       'given_name': '',
                       'type': 'personal'}
 
         if id_type in ['orcid', 'isni', 'gnd']:
             person.update({'identifiers': [{'identifier': id,
                                             'scheme': id_type}]})
     else:
-        org = _org_from_dict(data)
+        org = _org_from_dict(data, id_field_name='identifier')
         org['type'] = 'organizational'
 
     result = {}
     if person or org:
         result = {'person_or_org': person or org}
     if person:
         affiliations = []
@@ -1346,24 +1346,33 @@
         if affiliations:
             result['affiliations'] = affiliations
     if role:
         result['role'] = {'id': role}
     return result
 
 
-def _org_from_dict(data):
+def _org_from_dict(data, id_field_name='id'):
     # Hopefully it has a name field or id. If it doesn't, we can't do anything
     # more anyway, and will end up with an empty structure.
     org = {}
-    id = detected_id(data.get('@id', ''))  # noqa A001
-    if recognized_scheme(id) == 'ror':
-        org = {'id': detected_id(data)}
-    elif name := (data.get('legalName', '') or data.get('name', '')):
+    # If it has a name, we take it and we're done.
+    if name := (data.get('legalName', '') or data.get('name', '')):
         # In CFF the field name is 'legalName'. In CodeMeta it's 'name'.
         org = {'name': flattened_name(name)}
+    else:
+        # No name field. See if it has an id field of a type that we recognize.
+        id = detected_id(data.get('@id', ''))  # noqa A001
+        if recognized_scheme(id) == 'ror':
+            from iga.ror import name_from_ror
+            if name := name_from_ror(id):
+                org = {'name': name}
+            else:
+                # Got a ROR id but a lookup in ROR.org failed to get a name. We
+                # return just the identifier instead. Not ideal but acceptable.
+                org = {id_field_name: id}
     return org
 
 
 def _entity_match(first, second):
     # Match based on names only.
     p1 = first['person_or_org']
     p2 = second['person_or_org']
```

### Comparing `iga-1.0.0/iga/name_utils.py` & `iga-1.0.1/iga/name_utils.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.0/iga/orcid.py` & `iga-1.0.1/iga/orcid.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.0/iga/reference.py` & `iga-1.0.1/iga/reference.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.0/iga/ror.py` & `iga-1.0.1/iga/ror.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.0/iga/text_utils.py` & `iga-1.0.1/iga/text_utils.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.0/iga.egg-info/PKG-INFO` & `iga-1.0.1/iga.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iga
-Version: 1.0.0
+Version: 1.0.1
 Summary: InvenioRDM GitHub Archiver
 Home-page: https://github.com/caltechlibrary/iga
 Author: Michael Hucka
 Author-email: helpdesk@library.caltech.edu
 License: https://github.com/caltechlibrary/iga/blob/main/LICENSE
 Project-URL: Source Code, https://github.com/caltechlibrary/iga
 Project-URL: Bug Tracker, https://github.com/caltechlibrary/iga/issues
@@ -56,15 +56,15 @@
 <span style="font-size: 150%">➜</span>
 <img align="middle" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/example-record-landing-page.jpg" width="40%">
 </p>
 
 IGA offers many notable features:
 * Automatic metadata extraction from GitHub plus [`codemeta.json`](https://codemeta.github.io) and [`CITATION.cff`](https://citation-file-format.github.io) files
 * Thorough coverage of [InvenioRDM record metadata](https://inveniordm.docs.cern.ch/reference/metadata) using painstaking procedures
-* Recognition of identifiers in CodeMeta & CFF files: [ORCID](https://orcid.org),, [DOI](https://www.doi.org),  [PMCID](https://www.ncbi.nlm.nih.gov/pmc/about/public-access-info/), and more
+* Recognition of identifiers in CodeMeta & CFF files: [ORCID](https://orcid.org), [DOI](https://www.doi.org),  [PMCID](https://www.ncbi.nlm.nih.gov/pmc/about/public-access-info/), and more
 * Automatic lookup of publication data in [DOI.org](https://www.doi.org), [PubMed]((https://www.ncbi.nlm.nih.gov/pmc/about/public-access-info/)), Google, and other sources
 * Automatic lookup of organization names in [ROR](https://ror.org) (assuming ROR id's are provided)
 * Automatic lookup of human names in [ORCID.org](https://orcid.org) (assuming ORCID id's are provided)
 * Automatic splitting of human names into family & given names using [ML](https://en.wikipedia.org/wiki/Machine_learning) methods
 * Support for InvenioRDM [communities](https://invenio-communities.readthedocs.io/en/latest/)
 * Support for overriding the record that IGA creates, for complete control if you need it
 * Support for using the GitHub API without a [GitHub access token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) in simple cases
```

### Comparing `iga-1.0.0/iga.egg-info/SOURCES.txt` & `iga-1.0.1/iga.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iga-1.0.0/iga.egg-info/requires.txt` & `iga-1.0.1/iga.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `iga-1.0.0/setup.cfg` & `iga-1.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = iga
-version = 1.0.0
+version = 1.0.1
 description = InvenioRDM GitHub Archiver
 author = Michael Hucka
 author_email = helpdesk@library.caltech.edu
 license = https://github.com/caltechlibrary/iga/blob/main/LICENSE
 license_files = LICENSE
 url = https://github.com/caltechlibrary/iga
 project_urls =
```

### Comparing `iga-1.0.0/setup.py` & `iga-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.0/tests/test_cli.py` & `iga-1.0.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.0/tests/test_data_utils.py` & `iga-1.0.1/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.0/tests/test_doi.py` & `iga-1.0.1/tests/test_doi.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.0/tests/test_exceptions.py` & `iga-1.0.1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.0/tests/test_github.py` & `iga-1.0.1/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.0/tests/test_github_mocks.py` & `iga-1.0.1/tests/test_github_mocks.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.0/tests/test_id_utils.py` & `iga-1.0.1/tests/test_id_utils.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.0/tests/test_init.py` & `iga-1.0.1/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.0/tests/test_is_person.py` & `iga-1.0.1/tests/test_is_person.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.0/tests/test_licenses.py` & `iga-1.0.1/tests/test_licenses.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.0/tests/test_name_splitting.py` & `iga-1.0.1/tests/test_name_splitting.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.0/tests/test_name_utils.py` & `iga-1.0.1/tests/test_name_utils.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.0/tests/test_orcid.py` & `iga-1.0.1/tests/test_orcid.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.0/tests/test_record_from_codemeta.py` & `iga-1.0.1/tests/test_record_from_codemeta.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.0/tests/test_reference.py` & `iga-1.0.1/tests/test_reference.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.0/tests/test_ror.py` & `iga-1.0.1/tests/test_ror.py`

 * *Files identical despite different names*

### Comparing `iga-1.0.0/tests/test_text_utils.py` & `iga-1.0.1/tests/test_text_utils.py`

 * *Files identical despite different names*

