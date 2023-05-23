# Comparing `tmp/enjoy_slurm-0.0.4.tar.gz` & `tmp/enjoy_slurm-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enjoy_slurm-0.0.4.tar", last modified: Sat Apr  8 20:23:01 2023, max compression
+gzip compressed data, was "enjoy_slurm-0.1.0.tar", last modified: Tue May 23 17:37:23 2023, max compression
```

## Comparing `enjoy_slurm-0.0.4.tar` & `enjoy_slurm-0.1.0.tar`

### file list

```diff
@@ -1,59 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:23:01.223911 enjoy_slurm-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:23:01.219911 enjoy_slurm-0.0.4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:23:01.219911 enjoy_slurm-0.0.4/.github/workflows/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:23:01.219911 enjoy_slurm-0.0.4/.github/workflows/optional/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/.github/workflows/optional/linting.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/.github/workflows/slurm.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-04-08 20:23:01.223911 enjoy_slurm-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:23:01.219911 enjoy_slurm-0.0.4/ci/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/ci/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:23:01.219911 enjoy_slurm-0.0.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/docs/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/docs/new_section.rst
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/docs/tutorial.nblink
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/docs/whats_new.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:23:01.219911 enjoy_slurm-0.0.4/enjoy_slurm/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/enjoy_slurm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-08 20:23:01.000000 enjoy_slurm-0.0.4/enjoy_slurm/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/enjoy_slurm/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/enjoy_slurm/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/enjoy_slurm/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/enjoy_slurm/tutorial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/enjoy_slurm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:23:01.223911 enjoy_slurm-0.0.4/enjoy_slurm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-04-08 20:23:01.000000 enjoy_slurm-0.0.4/enjoy_slurm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-08 20:23:01.000000 enjoy_slurm-0.0.4/enjoy_slurm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 20:23:01.000000 enjoy_slurm-0.0.4/enjoy_slurm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 20:23:01.000000 enjoy_slurm-0.0.4/enjoy_slurm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-08 20:23:01.000000 enjoy_slurm-0.0.4/enjoy_slurm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-08 20:23:01.000000 enjoy_slurm-0.0.4/enjoy_slurm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:23:01.223911 enjoy_slurm-0.0.4/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/notebooks/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/notebooks/test.sh
--rw-r--r--   0 runner    (1001) docker     (123)    17016 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/notebooks/tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:23:01.223911 enjoy_slurm-0.0.4/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2710 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/scripts/configure.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-08 20:23:01.223911 enjoy_slurm-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:23:01.223911 enjoy_slurm-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/tests/test_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/tests/test_tutorial.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-08 20:22:52.000000 enjoy_slurm-0.0.4/tests/test_with_slurm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:37:23.407305 enjoy_slurm-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:37:23.399305 enjoy_slurm-0.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:37:23.403305 enjoy_slurm-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/.github/workflows/ci.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:37:23.403305 enjoy_slurm-0.1.0/.github/workflows/optional/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/.github/workflows/optional/linting.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/.github/workflows/slurm.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-05-23 17:37:23.407305 enjoy_slurm-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:37:23.403305 enjoy_slurm-0.1.0/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/ci/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/ci/none.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:37:23.403305 enjoy_slurm-0.1.0/ci/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/ci/slurm/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/ci/slurm/docker-compose.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      152 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/ci/slurm/register_cluster.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/ci/slurm/slurm.conf
+-rwxr-xr-x   0 runner    (1001) docker     (123)      662 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/ci/slurm/start-slurm.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/ci/slurm.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:37:23.403305 enjoy_slurm-0.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/docs/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/docs/new_section.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/docs/tutorial.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/docs/whats_new.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:37:23.403305 enjoy_slurm-0.1.0/enjoy_slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/enjoy_slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-23 17:37:23.000000 enjoy_slurm-0.1.0/enjoy_slurm/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/enjoy_slurm/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/enjoy_slurm/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/enjoy_slurm/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/enjoy_slurm/tutorial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/enjoy_slurm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:37:23.403305 enjoy_slurm-0.1.0/enjoy_slurm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-05-23 17:37:23.000000 enjoy_slurm-0.1.0/enjoy_slurm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-23 17:37:23.000000 enjoy_slurm-0.1.0/enjoy_slurm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 17:37:23.000000 enjoy_slurm-0.1.0/enjoy_slurm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 17:37:23.000000 enjoy_slurm-0.1.0/enjoy_slurm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 17:37:23.000000 enjoy_slurm-0.1.0/enjoy_slurm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-23 17:37:23.000000 enjoy_slurm-0.1.0/enjoy_slurm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:37:23.403305 enjoy_slurm-0.1.0/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/notebooks/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/notebooks/test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    17016 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/notebooks/tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:37:23.403305 enjoy_slurm-0.1.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2710 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/scripts/configure.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-23 17:37:23.407305 enjoy_slurm-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:37:23.407305 enjoy_slurm-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/tests/test_slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/tests/test_tutorial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-23 17:37:16.000000 enjoy_slurm-0.1.0/tests/test_with_slurm.py
```

### Comparing `enjoy_slurm-0.0.4/.github/workflows/release.yaml` & `enjoy_slurm-0.1.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `enjoy_slurm-0.0.4/.github/workflows/slurm.yml` & `enjoy_slurm-0.1.0/.github/workflows/slurm.yml`

 * *Files identical despite different names*

### Comparing `enjoy_slurm-0.0.4/.github/workflows/test.yaml` & `enjoy_slurm-0.1.0/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `enjoy_slurm-0.0.4/.gitignore` & `enjoy_slurm-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `enjoy_slurm-0.0.4/.pre-commit-config.yaml` & `enjoy_slurm-0.1.0/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -3,27 +3,27 @@
     rev: v4.4.0
     hooks:
     - id: check-yaml
     - id: check-json
     - id: end-of-file-fixer
     - id: trailing-whitespace
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
     - id: black
   - repo: https://github.com/pycqa/isort
     rev: 5.12.0
     hooks:
       - id: isort
         name: isort (python)
         args: ["--profile", "black", "--filter-files"]
   - repo: https://github.com/pycqa/flake8
     rev: 6.0.0
     hooks:
       - id: flake8
   - repo: https://github.com/nbQA-dev/nbQA
-    rev: 1.6.3
+    rev: 1.7.0
     hooks:
       - id: nbqa-black
       - id: nbqa-pyupgrade
         args: [ --py38-plus ]
       - id: nbqa-isort
```

### Comparing `enjoy_slurm-0.0.4/LICENSE.txt` & `enjoy_slurm-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `enjoy_slurm-0.0.4/PKG-INFO` & `enjoy_slurm-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enjoy_slurm
-Version: 0.0.4
+Version: 0.1.0
 Summary: naive python slurm control
 Home-page: https://github.com/larsbuntemeyer/enjoy-slurm
 Author: Lars Buntemeyer
 Author-email: lars.buntemeyer@hereon.de
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `enjoy_slurm-0.0.4/README.md` & `enjoy_slurm-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `enjoy_slurm-0.0.4/docs/Makefile` & `enjoy_slurm-0.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `enjoy_slurm-0.0.4/docs/conf.py` & `enjoy_slurm-0.1.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,14 @@
 autosummary_generate = True
 
 autodoc_typehints = "description"
 autodoc_typehints_description_target = "documented"
 autodoc_default_options = {
     "members": True,
     "undoc-members": True,
-    "private-members": True,
+    "private-members": False,
 }
 napoleon_use_param = True
 napoleon_use_rtype = True
 
 numpydoc_show_class_members = False
 # numpydoc_validation_checks = {"all"}
```

### Comparing `enjoy_slurm-0.0.4/docs/index.rst` & `enjoy_slurm-0.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `enjoy_slurm-0.0.4/enjoy_slurm/config.py` & `enjoy_slurm-0.1.0/enjoy_slurm/config.py`

 * *Files identical despite different names*

### Comparing `enjoy_slurm-0.0.4/enjoy_slurm/parser.py` & `enjoy_slurm-0.1.0/enjoy_slurm/parser.py`

 * *Files identical despite different names*

### Comparing `enjoy_slurm-0.0.4/enjoy_slurm/slurm.py` & `enjoy_slurm-0.1.0/enjoy_slurm/slurm.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,16 +7,15 @@
     args_to_list,
     handle_sacct_format,
     kwargs_to_list,
     parse_header,
     parse_sacct,
     split_script,
 )
-from .utils import (
-    create_scontrol_func,
+from .utils import (  # create_scontrol_func,
     execute,
     interp_from_shebang,
     shebang_from_interp,
 )
 
 
 def sbatch(
@@ -145,35 +144,35 @@
     if format is not None and "JobID" not in format:
         format.append("JobID")
     acct = sacct(jobid, format, steps, **kwargs)
 
     return acct.set_index("JobID").to_dict(orient="index")
 
 
-class SControl(type):
-    def __getattr__(cls, key):
-        return create_scontrol_func(key)
+# class SControl(type):
+#     def __getattr__(cls, key):
+#         return create_scontrol_func(key)
+
+
+# class scontrol(metaclass=SControl):
+#     """
+#     View or modify Slurm configuration and state
+#     """
+
+#     def show(*args, **kwargs):
+#         """
+#         Display state of identified entity, default is all records.
+
+#         Entity may be "aliases", "assoc_mgr", "bbstat", "burstBuffer",
+#         "config", "daemons", "dwstat", "federation", "frontend",
+#         "hostlist", "hostlistsorted", "hostnames", "job", "node",
+#         "partition", "reservation", "slurmd", "step", or "topology".
 
-
-class scontrol(metaclass=SControl):
-    """
-    View or modify Slurm configuration and state
-    """
-
-    def show(*args, **kwargs):
-        """
-        Display state of identified entity, default is all records.
-
-        Entity may be "aliases", "assoc_mgr", "bbstat", "burstBuffer",
-        "config", "daemons", "dwstat", "federation", "frontend",
-        "hostlist", "hostlistsorted", "hostnames", "job", "node",
-        "partition", "reservation", "slurmd", "step", or "topology".
-
-        """
-        return create_scontrol_func("show")(*args, **kwargs)
+#         """
+#         return create_scontrol_func("show")(*args, **kwargs)
 
 
 class Job:
     """
     Slurm Job class.
 
     The Job class can manage meta data and submission of a Slurm job.
@@ -202,14 +201,15 @@
     ):
         self.job = job
         self.jobid = jobid
         self.interpreter = interpreter
         self.shebang = shebang
         self.verbose = verbose
         self.kwargs = kwargs
+        self.config = {}
         self.filename = None
 
         if job is None:
             self.job = ""
         self.wrap = None
 
         if op.isfile(self.job):
@@ -254,32 +254,32 @@
 
     def __getattr__(self, key):
         return self.jobinfo(format=key)
 
     def __repr__(self):
         indent = 2 * " "
         # txt = f"job         : {self.job}\n"
-        txt = f"filename     : {self.filename}\n"
+        txt = f"filename    : {self.filename}\n"
         txt += f"jobid       : {self.jobid}\n\n"
         txt += "Slurm\n"
-        for k, v in self.kwargs.items():
+        for k, v in self.config.items():
             txt += indent + f"{k} : {v}\n"
         return txt
 
     @property
     def fields(self):
         """Available job attributes"""
         return list(self.sacct(format="all").columns)
 
     def sbatch(self, **kwargs):
         """Submit job to Slurm"""
-        config = self.kwargs.copy()
+        config = self.config.copy()
         config.update(kwargs)
-        jobid = sbatch(self.jobscript, wrap=self.wrap, **config)
-        self.scontrol = scontrol.show(jobid=jobid)
+        jobid = sbatch(self.filename, wrap=self.wrap, **config)
+        # self.scontrol = scontrol.show(jobid=jobid)
         if self.jobid is None:
             self.jobid = jobid
             return self
         job = copy.copy(self)
         job.jobid = jobid
         return job
```

### Comparing `enjoy_slurm-0.0.4/enjoy_slurm/tutorial.py` & `enjoy_slurm-0.1.0/enjoy_slurm/tutorial.py`

 * *Files identical despite different names*

### Comparing `enjoy_slurm-0.0.4/enjoy_slurm/utils.py` & `enjoy_slurm-0.1.0/enjoy_slurm/utils.py`

 * *Files identical despite different names*

### Comparing `enjoy_slurm-0.0.4/enjoy_slurm.egg-info/PKG-INFO` & `enjoy_slurm-0.1.0/enjoy_slurm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enjoy-slurm
-Version: 0.0.4
+Version: 0.1.0
 Summary: naive python slurm control
 Home-page: https://github.com/larsbuntemeyer/enjoy-slurm
 Author: Lars Buntemeyer
 Author-email: lars.buntemeyer@hereon.de
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `enjoy_slurm-0.0.4/enjoy_slurm.egg-info/SOURCES.txt` & `enjoy_slurm-0.1.0/enjoy_slurm.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 .gitignore
 .pre-commit-config.yaml
 LICENSE.txt
 README.md
+conftest.py
 docker-compose.yml
 environment.yml
 pyproject.toml
 readthedocs.yml
 setup.cfg
 setup.py
 .github/dependabot.yml
+.github/workflows/ci.yaml
 .github/workflows/release.yaml
 .github/workflows/slurm.yml
 .github/workflows/test.yaml
 .github/workflows/optional/linting.yaml
 ci/environment.yml
+ci/none.sh
+ci/slurm.sh
+ci/slurm/Dockerfile
+ci/slurm/docker-compose.yml
+ci/slurm/register_cluster.sh
+ci/slurm/slurm.conf
+ci/slurm/start-slurm.sh
 docs/Makefile
 docs/api.rst
 docs/conf.py
 docs/environment.yml
 docs/index.rst
 docs/new_section.rst
 docs/tutorial.nblink
@@ -38,10 +47,11 @@
 notebooks/.gitkeep
 notebooks/test.sh
 notebooks/tutorial.ipynb
 scripts/configure.sh
 tests/__init__.py
 tests/test_job.py
 tests/test_parser.py
+tests/test_slurm.py
 tests/test_tutorial.py
 tests/test_utils.py
 tests/test_with_slurm.py
```

### Comparing `enjoy_slurm-0.0.4/notebooks/tutorial.ipynb` & `enjoy_slurm-0.1.0/notebooks/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `enjoy_slurm-0.0.4/pyproject.toml` & `enjoy_slurm-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `enjoy_slurm-0.0.4/scripts/configure.sh` & `enjoy_slurm-0.1.0/scripts/configure.sh`

 * *Files identical despite different names*

### Comparing `enjoy_slurm-0.0.4/setup.cfg` & `enjoy_slurm-0.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `enjoy_slurm-0.0.4/tests/__init__.py` & `enjoy_slurm-0.1.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `enjoy_slurm-0.0.4/tests/test_job.py` & `enjoy_slurm-0.1.0/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `enjoy_slurm-0.0.4/tests/test_parser.py` & `enjoy_slurm-0.1.0/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `enjoy_slurm-0.0.4/tests/test_tutorial.py` & `enjoy_slurm-0.1.0/tests/test_tutorial.py`

 * *Files identical despite different names*

### Comparing `enjoy_slurm-0.0.4/tests/test_with_slurm.py` & `enjoy_slurm-0.1.0/tests/test_with_slurm.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from enjoy_slurm import Job, sacct, sbatch, scontrol
+from enjoy_slurm import Job, sacct, sbatch
 
 from . import hostname, on_levante, requires_slurm
 
 test_kwargs = {
     "levante": {"partitions": ["compute", "shared"]},
     "docker": {"partitions": ["debug", "normal"]},
 }
@@ -21,31 +21,31 @@
         kwargs = {"partition": "shared", "account": "ch0636"}
     else:
         kwargs = {}
     jobid = sbatch(wrap="echo Hello World", **kwargs)
     print(jobid)
 
 
-@requires_slurm
-def test_partitions():
-    if on_levante:
-        partitions = test_kwargs["levante"]["partitions"]
-    else:
-        partitions = test_kwargs["docker"]["partitions"]
-    for p in partitions:
-        pdict = scontrol.show(partition=p)
-        assert p in pdict
+# @requires_slurm
+# def test_partitions():
+#    if on_levante:
+#        partitions = test_kwargs["levante"]["partitions"]
+#    else:
+#        partitions = test_kwargs["docker"]["partitions"]
+#    for p in partitions:
+#        pdict = scontrol.show(partition=p)
+#        assert p in pdict
 
 
 @requires_slurm
 def test_sacct():
     jobid = sbatch(wrap="echo Hello World", **kwargs)
     sacct(jobid=jobid)
-    scon = scontrol.show(jobid=jobid)
-    assert str(jobid) in scon
+    # scon = scontrol.show(jobid=jobid)
+    # assert str(jobid) in scon
 
 
 @requires_slurm
 def test_job():
     import time
 
     jobid = sbatch(wrap="echo Hello World", **kwargs)
```

