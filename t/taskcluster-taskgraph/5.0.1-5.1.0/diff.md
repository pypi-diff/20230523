# Comparing `tmp/taskcluster-taskgraph-5.0.1.tar.gz` & `tmp/taskcluster-taskgraph-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskcluster-taskgraph-5.0.1.tar", last modified: Fri Mar 31 09:40:07 2023, max compression
+gzip compressed data, was "taskcluster-taskgraph-5.1.0.tar", last modified: Tue Apr 18 18:59:00 2023, max compression
```

## Comparing `taskcluster-taskgraph-5.0.1.tar` & `taskcluster-taskgraph-5.1.0.tar`

### file list

```diff
@@ -1,140 +1,142 @@
-drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-03-31 09:40:07.128079 taskcluster-taskgraph-5.0.1/
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    16725 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/LICENSE
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      175 2023-03-23 10:10:23.000000 taskcluster-taskgraph-5.0.1/MANIFEST.in
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      699 2023-03-31 09:40:07.128079 taskcluster-taskgraph-5.0.1/PKG-INFO
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     3659 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/README.rst
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      602 2023-03-23 10:10:23.000000 taskcluster-taskgraph-5.0.1/pyproject.toml
-drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-03-31 09:40:07.120079 taskcluster-taskgraph-5.0.1/requirements/
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      191 2023-03-23 10:10:23.000000 taskcluster-taskgraph-5.0.1/requirements/base.in
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    20973 2023-03-23 10:10:23.000000 taskcluster-taskgraph-5.0.1/requirements/base.txt
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)       22 2023-01-13 16:17:04.000000 taskcluster-taskgraph-5.0.1/requirements/dev.in
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1182 2023-02-10 13:42:33.000000 taskcluster-taskgraph-5.0.1/requirements/dev.txt
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)       58 2023-02-10 13:42:33.000000 taskcluster-taskgraph-5.0.1/requirements/test.in
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     9437 2023-03-23 10:10:23.000000 taskcluster-taskgraph-5.0.1/requirements/test.txt
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)       38 2023-03-31 09:40:07.128079 taskcluster-taskgraph-5.0.1/setup.cfg
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1555 2023-03-23 10:10:23.000000 taskcluster-taskgraph-5.0.1/setup.py
-drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-03-31 09:40:07.120079 taskcluster-taskgraph-5.0.1/src/
-drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-03-31 09:40:07.120079 taskcluster-taskgraph-5.0.1/src/taskcluster_taskgraph.egg-info/
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      699 2023-03-31 09:40:07.000000 taskcluster-taskgraph-5.0.1/src/taskcluster_taskgraph.egg-info/PKG-INFO
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     3771 2023-03-31 09:40:07.000000 taskcluster-taskgraph-5.0.1/src/taskcluster_taskgraph.egg-info/SOURCES.txt
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)        1 2023-03-31 09:40:07.000000 taskcluster-taskgraph-5.0.1/src/taskcluster_taskgraph.egg-info/dependency_links.txt
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)       51 2023-03-31 09:40:07.000000 taskcluster-taskgraph-5.0.1/src/taskcluster_taskgraph.egg-info/entry_points.txt
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      215 2023-03-31 09:40:07.000000 taskcluster-taskgraph-5.0.1/src/taskcluster_taskgraph.egg-info/requires.txt
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)       10 2023-03-31 09:40:07.000000 taskcluster-taskgraph-5.0.1/src/taskcluster_taskgraph.egg-info/top_level.txt
-drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-03-31 09:40:07.120079 taskcluster-taskgraph-5.0.1/src/taskgraph/
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      729 2023-03-31 09:39:05.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/__init__.py
-drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-03-31 09:40:07.120079 taskcluster-taskgraph-5.0.1/src/taskgraph/actions/
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      416 2022-04-14 07:55:53.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/actions/__init__.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1831 2022-04-14 07:55:53.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/actions/add_new_jobs.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1309 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/actions/cancel.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1941 2023-03-23 10:10:23.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/actions/cancel_all.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1086 2023-01-13 16:17:04.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/actions/rebuild_cached_tasks.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    13113 2023-03-23 10:10:23.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/actions/registry.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     9382 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/actions/retrigger.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    10667 2023-03-23 10:10:23.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/actions/util.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     4411 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/config.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     5184 2023-03-23 10:10:23.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/create.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    12882 2023-02-24 15:02:25.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/decision.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     7834 2023-02-10 13:42:33.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/docker.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     2793 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/files_changed.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      866 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/filter_tasks.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    15589 2023-02-10 13:42:33.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/generator.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     4667 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/graph.py
-drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-03-31 09:40:07.120079 taskcluster-taskgraph-5.0.1/src/taskgraph/loader/
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)        0 2022-04-14 07:55:53.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/loader/__init__.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     2147 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/loader/transform.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    25712 2023-03-23 10:10:23.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/main.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     9625 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/morph.py
-drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-03-31 09:40:07.124079 taskcluster-taskgraph-5.0.1/src/taskgraph/optimize/
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      123 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/optimize/__init__.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    18341 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/optimize/base.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     2380 2023-02-10 13:42:33.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/optimize/strategies.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    11906 2023-01-13 16:17:04.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/parameters.py
-drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-03-31 09:40:07.124079 taskcluster-taskgraph-5.0.1/src/taskgraph/run-task/
--rwxr-xr-x   0 jcristau  (1000) jcristau  (1000)    29990 2023-03-31 07:42:28.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/run-task/fetch-content
--rwxr-xr-x   0 jcristau  (1000) jcristau  (1000)      896 2022-04-14 07:55:53.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/run-task/hgrc
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    30243 2023-03-31 07:42:28.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/run-task/robustcheckout.py
--rwxr-xr-x   0 jcristau  (1000) jcristau  (1000)    43884 2023-03-31 07:42:28.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/run-task/run-task
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     3324 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/target_tasks.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     3132 2022-04-14 07:55:53.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/task.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     2397 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/taskgraph.py
-drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-03-31 09:40:07.124079 taskcluster-taskgraph-5.0.1/src/taskgraph/transforms/
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      110 2023-01-13 16:17:04.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/transforms/__init__.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     5285 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/transforms/base.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     2607 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/transforms/cached_tasks.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      707 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/transforms/code_review.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     7571 2023-01-13 16:17:04.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/transforms/docker_image.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    10443 2022-10-28 09:29:46.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/transforms/fetch.py
-drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-03-31 09:40:07.124079 taskcluster-taskgraph-5.0.1/src/taskgraph/transforms/job/
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    17271 2023-01-13 16:17:04.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/transforms/job/__init__.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     6826 2022-10-28 09:29:46.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/transforms/job/common.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1220 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/transforms/job/index_search.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     9474 2023-03-23 10:10:23.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/transforms/job/run_task.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     6015 2023-02-10 13:42:33.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/transforms/job/toolchain.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     6019 2023-01-13 16:17:04.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/transforms/notify.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    48693 2023-03-23 10:10:23.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/transforms/task.py
-drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-03-31 09:40:07.124079 taskcluster-taskgraph-5.0.1/src/taskgraph/util/
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)        0 2022-04-14 07:55:53.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/util/__init__.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     2855 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/util/archive.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     2617 2022-04-14 07:55:53.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/util/attributes.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     3406 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/util/cached_tasks.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     2433 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/util/decision.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    11690 2023-03-23 10:10:23.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/util/docker.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1661 2023-01-13 16:17:04.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/util/hash.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     3419 2022-04-14 07:55:53.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/util/keyed_by.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1331 2022-04-14 07:55:53.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/util/memoize.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     3184 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/util/parameterization.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     4468 2023-03-23 10:10:23.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/util/path.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1576 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/util/python_path.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      787 2022-04-14 07:55:53.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/util/readonlydict.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     8323 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/util/schema.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1317 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/util/shell.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    12445 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/util/taskcluster.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1969 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/util/taskgraph.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1417 2022-04-14 07:55:53.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/util/templates.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     3390 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/util/time.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     2138 2022-04-14 07:55:53.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/util/treeherder.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    18534 2023-02-10 13:42:36.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/util/vcs.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     8827 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/util/verify.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     2494 2023-03-23 10:10:23.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/util/workertypes.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1029 2023-03-23 10:10:23.000000 taskcluster-taskgraph-5.0.1/src/taskgraph/util/yaml.py
-drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-03-31 09:40:07.128079 taskcluster-taskgraph-5.0.1/test/
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1584 2023-01-13 16:17:04.000000 taskcluster-taskgraph-5.0.1/test/test_actions_rebuild_cached_tasks.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1670 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/test/test_actions_registry.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     3654 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/test/test_create.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     7688 2023-03-23 10:10:23.000000 taskcluster-taskgraph-5.0.1/test/test_decision.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     3505 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/test/test_files_changed.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     4828 2023-01-13 16:17:04.000000 taskcluster-taskgraph-5.0.1/test/test_generator.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     7063 2023-02-10 13:42:33.000000 taskcluster-taskgraph-5.0.1/test/test_graph.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     7403 2023-03-23 10:10:23.000000 taskcluster-taskgraph-5.0.1/test/test_main.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     2701 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/test/test_morph.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    15145 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/test/test_optimize.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1727 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/test/test_optimize_strategies.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    13921 2023-03-23 10:10:23.000000 taskcluster-taskgraph-5.0.1/test/test_parameters.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     2491 2023-03-31 07:42:28.000000 taskcluster-taskgraph-5.0.1/test/test_scripts_fetch_content.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    11792 2023-02-10 13:42:33.000000 taskcluster-taskgraph-5.0.1/test/test_scripts_run_task.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    12046 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/test/test_target_tasks.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     3759 2023-02-10 13:42:33.000000 taskcluster-taskgraph-5.0.1/test/test_taskgraph.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      874 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/test/test_transforms_base.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1527 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/test/test_transforms_fetch.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     5181 2023-01-13 16:17:04.000000 taskcluster-taskgraph-5.0.1/test/test_transforms_job.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     5183 2023-03-23 10:10:23.000000 taskcluster-taskgraph-5.0.1/test/test_transforms_job_run_task.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     7131 2023-02-10 13:42:33.000000 taskcluster-taskgraph-5.0.1/test/test_transforms_job_toolchain.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     6948 2023-01-13 16:17:04.000000 taskcluster-taskgraph-5.0.1/test/test_transforms_notify.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     4362 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/test/test_transforms_task.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     3596 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/test/test_util_attributes.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    10212 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/test/test_util_docker.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     2340 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/test/test_util_memoize.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     7556 2023-01-13 16:17:04.000000 taskcluster-taskgraph-5.0.1/test/test_util_parameterization.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     5906 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/test/test_util_path.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1045 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/test/test_util_python_path.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1234 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/test/test_util_readonlydict.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     6961 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/test/test_util_schema.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    10115 2023-02-10 13:42:33.000000 taskcluster-taskgraph-5.0.1/test/test_util_taskcluster.py
--rwxr-xr-x   0 jcristau  (1000) jcristau  (1000)     1677 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/test/test_util_templates.py
--rwxr-xr-x   0 jcristau  (1000) jcristau  (1000)     2239 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/test/test_util_time.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      913 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/test/test_util_treeherder.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    14739 2023-03-23 10:10:23.000000 taskcluster-taskgraph-5.0.1/test/test_util_vcs.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     4981 2022-10-10 16:39:57.000000 taskcluster-taskgraph-5.0.1/test/test_util_verify.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      942 2023-03-23 10:10:23.000000 taskcluster-taskgraph-5.0.1/test/test_util_workertypes.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1591 2023-03-23 10:10:23.000000 taskcluster-taskgraph-5.0.1/test/test_util_yaml.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-04-18 18:59:00.900562 taskcluster-taskgraph-5.1.0/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    16725 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.1.0/LICENSE
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      175 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.1.0/MANIFEST.in
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      665 2023-04-18 18:59:00.900562 taskcluster-taskgraph-5.1.0/PKG-INFO
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3659 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.1.0/README.rst
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      602 2023-04-03 20:26:22.000000 taskcluster-taskgraph-5.1.0/pyproject.toml
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-04-18 18:59:00.880562 taskcluster-taskgraph-5.1.0/requirements/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      191 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.1.0/requirements/base.in
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    20973 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.1.0/requirements/base.txt
+-rw-r--r--   0 ahal      (1000) ahal      (1000)       22 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.1.0/requirements/dev.in
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1182 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.1.0/requirements/dev.txt
+-rw-r--r--   0 ahal      (1000) ahal      (1000)       58 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.1.0/requirements/test.in
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     9437 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.1.0/requirements/test.txt
+-rw-r--r--   0 ahal      (1000) ahal      (1000)       38 2023-04-18 18:59:00.900562 taskcluster-taskgraph-5.1.0/setup.cfg
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1555 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.1.0/setup.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-04-18 18:59:00.870562 taskcluster-taskgraph-5.1.0/src/
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-04-18 18:59:00.880562 taskcluster-taskgraph-5.1.0/src/taskcluster_taskgraph.egg-info/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      665 2023-04-18 18:59:00.000000 taskcluster-taskgraph-5.1.0/src/taskcluster_taskgraph.egg-info/PKG-INFO
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3839 2023-04-18 18:59:00.000000 taskcluster-taskgraph-5.1.0/src/taskcluster_taskgraph.egg-info/SOURCES.txt
+-rw-r--r--   0 ahal      (1000) ahal      (1000)        1 2023-04-18 18:59:00.000000 taskcluster-taskgraph-5.1.0/src/taskcluster_taskgraph.egg-info/dependency_links.txt
+-rw-r--r--   0 ahal      (1000) ahal      (1000)       50 2023-04-18 18:59:00.000000 taskcluster-taskgraph-5.1.0/src/taskcluster_taskgraph.egg-info/entry_points.txt
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      215 2023-04-18 18:59:00.000000 taskcluster-taskgraph-5.1.0/src/taskcluster_taskgraph.egg-info/requires.txt
+-rw-r--r--   0 ahal      (1000) ahal      (1000)       10 2023-04-18 18:59:00.000000 taskcluster-taskgraph-5.1.0/src/taskcluster_taskgraph.egg-info/top_level.txt
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-04-18 18:59:00.880562 taskcluster-taskgraph-5.1.0/src/taskgraph/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      729 2023-04-18 18:58:20.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/__init__.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-04-18 18:59:00.880562 taskcluster-taskgraph-5.1.0/src/taskgraph/actions/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      416 2022-06-10 19:06:39.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/actions/__init__.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1831 2022-06-10 19:06:39.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/actions/add_new_jobs.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1309 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/actions/cancel.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1941 2023-03-14 20:54:32.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/actions/cancel_all.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1086 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/actions/rebuild_cached_tasks.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    13113 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/actions/registry.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     9382 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/actions/retrigger.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    10661 2023-04-13 20:26:06.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/actions/util.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     4583 2023-04-13 20:26:06.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/config.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     5184 2023-03-14 20:54:32.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/create.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    12882 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/decision.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     7834 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/docker.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2793 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/files_changed.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      866 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/filter_tasks.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    15386 2023-04-14 15:23:07.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/generator.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     4667 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/graph.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-04-18 18:59:00.880562 taskcluster-taskgraph-5.1.0/src/taskgraph/loader/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)        0 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/loader/__init__.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1185 2023-04-13 20:26:06.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/loader/default.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2147 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/loader/transform.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    25712 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/main.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     9192 2023-04-13 20:26:06.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/morph.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-04-18 18:59:00.880562 taskcluster-taskgraph-5.1.0/src/taskgraph/optimize/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      123 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/optimize/__init__.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    18341 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/optimize/base.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2380 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/optimize/strategies.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    11906 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/parameters.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-04-18 18:59:00.880562 taskcluster-taskgraph-5.1.0/src/taskgraph/run-task/
+-rwxr-xr-x   0 ahal      (1000) ahal      (1000)    29990 2023-04-04 13:08:54.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/run-task/fetch-content
+-rwxr-xr-x   0 ahal      (1000) ahal      (1000)      896 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/run-task/hgrc
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    30243 2023-04-04 13:08:54.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/run-task/robustcheckout.py
+-rwxr-xr-x   0 ahal      (1000) ahal      (1000)    43884 2023-04-04 13:08:30.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/run-task/run-task
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3324 2023-04-03 20:22:29.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/target_tasks.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3132 2023-02-08 18:55:54.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/task.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2397 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/taskgraph.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-04-18 18:59:00.890562 taskcluster-taskgraph-5.1.0/src/taskgraph/transforms/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      110 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/transforms/__init__.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     5285 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/transforms/base.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2607 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/transforms/cached_tasks.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      707 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/transforms/code_review.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     7606 2023-04-13 20:26:06.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/transforms/docker_image.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    10443 2023-03-09 21:54:49.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/transforms/fetch.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-04-18 18:59:00.890562 taskcluster-taskgraph-5.1.0/src/taskgraph/transforms/job/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    17271 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/transforms/job/__init__.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     6826 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/transforms/job/common.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1220 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/transforms/job/index_search.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     9800 2023-04-18 18:34:00.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/transforms/job/run_task.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     6015 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/transforms/job/toolchain.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     6019 2023-03-09 21:54:49.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/transforms/notify.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    49761 2023-04-13 20:26:06.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/transforms/task.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-04-18 18:59:00.890562 taskcluster-taskgraph-5.1.0/src/taskgraph/util/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)        0 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/util/__init__.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2855 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/util/archive.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2617 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/util/attributes.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3406 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/util/cached_tasks.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2433 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/util/decision.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    11690 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/util/docker.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1661 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/util/hash.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3419 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/util/keyed_by.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1331 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/util/memoize.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3184 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/util/parameterization.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     4466 2023-04-13 20:26:06.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/util/path.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1576 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/util/python_path.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      787 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/util/readonlydict.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     8323 2023-04-18 14:17:54.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/util/schema.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1317 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/util/shell.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    12445 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/util/taskcluster.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1969 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/util/taskgraph.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1417 2022-05-30 14:06:28.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/util/templates.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3390 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/util/time.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2687 2023-04-13 20:26:06.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/util/treeherder.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    18534 2023-04-13 20:26:06.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/util/vcs.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     8827 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/util/verify.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2494 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/util/workertypes.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1029 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.1.0/src/taskgraph/util/yaml.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-04-18 18:59:00.900562 taskcluster-taskgraph-5.1.0/test/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1584 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.1.0/test/test_actions_rebuild_cached_tasks.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1670 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.1.0/test/test_actions_registry.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3654 2023-03-09 21:40:30.000000 taskcluster-taskgraph-5.1.0/test/test_create.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     7688 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.1.0/test/test_decision.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3505 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.1.0/test/test_files_changed.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     7588 2023-04-14 15:23:07.000000 taskcluster-taskgraph-5.1.0/test/test_generator.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     7063 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.1.0/test/test_graph.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     7403 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.1.0/test/test_main.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2701 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.1.0/test/test_morph.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    15145 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.1.0/test/test_optimize.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1727 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.1.0/test/test_optimize_strategies.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    13921 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.1.0/test/test_parameters.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2491 2023-04-04 13:08:54.000000 taskcluster-taskgraph-5.1.0/test/test_scripts_fetch_content.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    11792 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.1.0/test/test_scripts_run_task.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    12046 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.1.0/test/test_target_tasks.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3759 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.1.0/test/test_taskgraph.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1812 2023-04-13 20:26:06.000000 taskcluster-taskgraph-5.1.0/test/test_transform_docker_image.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      874 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.1.0/test/test_transforms_base.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1527 2023-03-09 21:27:25.000000 taskcluster-taskgraph-5.1.0/test/test_transforms_fetch.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     5181 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.1.0/test/test_transforms_job.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     6291 2023-04-18 18:34:00.000000 taskcluster-taskgraph-5.1.0/test/test_transforms_job_run_task.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     7131 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.1.0/test/test_transforms_job_toolchain.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     6948 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.1.0/test/test_transforms_notify.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    21918 2023-04-13 20:26:06.000000 taskcluster-taskgraph-5.1.0/test/test_transforms_task.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3596 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.1.0/test/test_util_attributes.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    10212 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.1.0/test/test_util_docker.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2340 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.1.0/test/test_util_memoize.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     7556 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.1.0/test/test_util_parameterization.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     5906 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.1.0/test/test_util_path.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1045 2023-03-09 21:27:25.000000 taskcluster-taskgraph-5.1.0/test/test_util_python_path.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1234 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.1.0/test/test_util_readonlydict.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     6961 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.1.0/test/test_util_schema.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    10115 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.1.0/test/test_util_taskcluster.py
+-rwxr-xr-x   0 ahal      (1000) ahal      (1000)     1677 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.1.0/test/test_util_templates.py
+-rwxr-xr-x   0 ahal      (1000) ahal      (1000)     2239 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.1.0/test/test_util_time.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      913 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.1.0/test/test_util_treeherder.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    14739 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.1.0/test/test_util_vcs.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     4981 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.1.0/test/test_util_verify.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      942 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.1.0/test/test_util_workertypes.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1591 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.1.0/test/test_util_yaml.py
```

### Comparing `taskcluster-taskgraph-5.0.1/LICENSE` & `taskcluster-taskgraph-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/PKG-INFO` & `taskcluster-taskgraph-5.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: taskcluster-taskgraph
-Version: 5.0.1
+Version: 5.1.0
 Summary: Build taskcluster taskgraphs
 Home-page: https://github.com/taskcluster/taskgraph
-License: UNKNOWN
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Provides-Extra: load-image
+License-File: LICENSE
```

### Comparing `taskcluster-taskgraph-5.0.1/README.rst` & `taskcluster-taskgraph-5.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/pyproject.toml` & `taskcluster-taskgraph-5.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/requirements/base.txt` & `taskcluster-taskgraph-5.1.0/requirements/base.txt`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/requirements/dev.txt` & `taskcluster-taskgraph-5.1.0/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/requirements/test.txt` & `taskcluster-taskgraph-5.1.0/requirements/test.txt`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/setup.py` & `taskcluster-taskgraph-5.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskcluster_taskgraph.egg-info/PKG-INFO` & `taskcluster-taskgraph-5.1.0/src/taskcluster_taskgraph.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: taskcluster-taskgraph
-Version: 5.0.1
+Version: 5.1.0
 Summary: Build taskcluster taskgraphs
 Home-page: https://github.com/taskcluster/taskgraph
-License: UNKNOWN
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Provides-Extra: load-image
+License-File: LICENSE
```

### Comparing `taskcluster-taskgraph-5.0.1/src/taskcluster_taskgraph.egg-info/SOURCES.txt` & `taskcluster-taskgraph-5.1.0/src/taskcluster_taskgraph.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 src/taskgraph/actions/cancel.py
 src/taskgraph/actions/cancel_all.py
 src/taskgraph/actions/rebuild_cached_tasks.py
 src/taskgraph/actions/registry.py
 src/taskgraph/actions/retrigger.py
 src/taskgraph/actions/util.py
 src/taskgraph/loader/__init__.py
+src/taskgraph/loader/default.py
 src/taskgraph/loader/transform.py
 src/taskgraph/optimize/__init__.py
 src/taskgraph/optimize/base.py
 src/taskgraph/optimize/strategies.py
 src/taskgraph/run-task/fetch-content
 src/taskgraph/run-task/hgrc
 src/taskgraph/run-task/robustcheckout.py
@@ -96,14 +97,15 @@
 test/test_optimize.py
 test/test_optimize_strategies.py
 test/test_parameters.py
 test/test_scripts_fetch_content.py
 test/test_scripts_run_task.py
 test/test_target_tasks.py
 test/test_taskgraph.py
+test/test_transform_docker_image.py
 test/test_transforms_base.py
 test/test_transforms_fetch.py
 test/test_transforms_job.py
 test/test_transforms_job_run_task.py
 test/test_transforms_job_toolchain.py
 test/test_transforms_notify.py
 test/test_transforms_task.py
```

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/__init__.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-__version__ = "5.0.1"
+__version__ = "5.1.0"
 
 # Maximum number of dependencies a single task can have
 # https://docs.taskcluster.net/reference/platform/taskcluster-queue/references/api#createTask
 # specifies 100, but we also optionally add the decision task id as a dep in
 # taskgraph.create, so let's set this to 99.
 MAX_DEPENDENCIES = 99
```

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/actions/add_new_jobs.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/actions/add_new_jobs.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/actions/cancel.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/actions/cancel.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/actions/cancel_all.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/actions/cancel_all.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/actions/rebuild_cached_tasks.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/actions/rebuild_cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/actions/registry.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/actions/registry.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/actions/retrigger.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/actions/retrigger.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/actions/util.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/actions/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
     If `suffix` is given, then it is used to give unique names to the resulting
     artifacts.  If you call this function multiple times in the same action,
     pass a different suffix each time to avoid overwriting artifacts.
 
     If you wish to create the tasks in a new group, leave out decision_task_id.
 
     Returns an updated label_to_taskid containing the new tasks"""
-    if suffix != "":
+    if suffix:
         suffix = f"-{suffix}"
     to_run = set(to_run)
 
     #  Copy to avoid side-effects later
     full_task_graph = copy.deepcopy(full_task_graph)
     label_to_taskid = label_to_taskid.copy()
```

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/config.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,14 +51,18 @@
             ): str,
             Optional("decision-parameters"): str,
             Optional(
                 "cached-task-prefix",
                 description="The taskcluster index prefix to use for caching tasks. "
                 "Defaults to `trust-domain`.",
             ): str,
+            Optional(
+                "index-path-regexes",
+                description="Regular expressions matching index paths to be summarized.",
+            ): [str],
             Required("repositories"): All(
                 {
                     str: {
                         Required("name"): str,
                         Optional("project-regex"): str,
                         Optional("ssh-secret-name"): str,
                         # FIXME
```

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/create.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/create.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/decision.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/decision.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/docker.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/docker.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/files_changed.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/files_changed.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/filter_tasks.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/filter_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/generator.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     config = attr.ib(type=dict)
     graph_config = attr.ib(type=GraphConfig)
 
     def _get_loader(self):
         try:
             loader = self.config["loader"]
         except KeyError:
-            raise KeyError(f"{self.path!r} does not define `loader`")
+            loader = "taskgraph.loader.default:loader"
         return find_object(loader)
 
     def load_tasks(self, parameters, loaded_tasks, write_artifacts):
         loader = self._get_loader()
         config = copy.deepcopy(self.config)
 
         kind_dependencies = config.get("kind-dependencies", [])
@@ -54,14 +54,17 @@
             task.label: task for task in loaded_tasks if task.kind in kind_dependencies
         }
 
         inputs = loader(self.name, self.path, config, parameters, loaded_tasks)
 
         transforms = TransformSequence()
         for xform_path in config["transforms"]:
+            if ":" not in xform_path:
+                xform_path = f"{xform_path}:transforms"
+
             transform = find_object(xform_path)
             transforms.add(transform)
 
         # perform the transformations on the loaded inputs
         trans_config = TransformConfig(
             self.name,
             self.path,
@@ -348,34 +351,28 @@
                 "Filter %s pruned %d tasks (%d remain)"
                 % (fltr.__name__, old_len - len(target_tasks), len(target_tasks))
             )
 
         yield self.verify("target_task_set", target_task_set, graph_config, parameters)
 
         logger.info("Generating target task graph")
-        # include all docker-image build tasks here, in case they are needed for a graph morph
-        docker_image_tasks = {
-            t.label
-            for t in full_task_graph.tasks.values()
-            if t.attributes["kind"] == "docker-image"
-        }
         # include all tasks with `always_target` set
         if parameters["enable_always_target"]:
             always_target_tasks = {
                 t.label
                 for t in full_task_graph.tasks.values()
                 if t.attributes.get("always_target")
             }
         else:
             always_target_tasks = set()
         logger.info(
             "Adding %d tasks with `always_target` attribute"
             % (len(always_target_tasks) - len(always_target_tasks & target_tasks))
         )
-        requested_tasks = target_tasks | docker_image_tasks | always_target_tasks
+        requested_tasks = target_tasks | always_target_tasks
         target_graph = full_task_graph.graph.transitive_closure(requested_tasks)
         target_task_graph = TaskGraph(
             {l: all_tasks[l] for l in target_graph.nodes}, target_graph
         )
         yield self.verify(
             "target_task_graph", target_task_graph, graph_config, parameters
         )
```

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/graph.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/graph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/loader/transform.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/loader/transform.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/main.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/main.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/morph.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/morph.py`

 * *Files 5% similar despite different names*

```diff
@@ -106,26 +106,14 @@
         task=task_def,
         dependencies=dependencies,
     )
     task.task_id = slugid()
     return task, taskgraph, label_to_taskid
 
 
-# these regular expressions capture route prefixes for which we have a star
-# scope, allowing them to be summarized.  Each should correspond to a star scope
-# in each Gecko `assume:repo:hg.mozilla.org/...` role.
-_SCOPE_SUMMARY_REGEXPS = [
-    # TODO Bug 1631839 - Remove these scopes once the migration is done
-    re.compile(r"(index:insert-task:project\.mobile\.fenix\.v2\.[^.]*\.).*"),
-    re.compile(
-        r"(index:insert-task:project\.mobile\.reference-browser\.v3\.[^.]*\.).*"
-    ),
-]
-
-
 def make_index_task(parent_task, taskgraph, label_to_taskid, parameters, graph_config):
     index_paths = [
         r.split(".", 1)[1] for r in parent_task.task["routes"] if r.startswith("index.")
     ]
     parent_task.task["routes"] = [
         r for r in parent_task.task["routes"] if not r.startswith("index.")
     ]
@@ -134,27 +122,29 @@
         parent_task, taskgraph, label_to_taskid, parameters, graph_config
     )
 
     # we need to "summarize" the scopes, otherwise a particularly
     # namespace-heavy index task might have more scopes than can fit in a
     # temporary credential.
     scopes = set()
-    domain_scope_regex = re.compile(
-        r"(index:insert-task:{trust_domain}\.v2\.[^.]*\.).*".format(
+    domain_index_regex = re.compile(
+        r"({trust_domain}\.v2\.[^.]*\.).*".format(
             trust_domain=re.escape(graph_config["trust-domain"])
         )
     )
-    all_scopes_summary_regexps = _SCOPE_SUMMARY_REGEXPS + [domain_scope_regex]
+    index_path_res = [domain_index_regex]
+    for path in graph_config["taskgraph"].get("index-path-regexes", ()):
+        index_path_res.append(re.compile(path))
     for path in index_paths:
-        scope = f"index:insert-task:{path}"
-        for summ_re in all_scopes_summary_regexps:
-            match = summ_re.match(scope)
+        for index_path_re in index_path_res:
+            match = index_path_re.match(path)
             if match:
-                scope = match.group(1) + "*"
+                path = match.group(1) + "*"
                 break
+        scope = f"index:insert-task:{path}"
         scopes.add(scope)
     task.task["scopes"] = sorted(scopes)
 
     task.task["payload"]["command"] = ["insert-indexes.js"] + index_paths
     task.task["payload"]["env"] = {
         "TARGET_TASKID": parent_task.task_id,
         "INDEX_RANK": parent_task.task.get("extra", {}).get("index", {}).get("rank", 0),
```

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/optimize/base.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/optimize/base.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/optimize/strategies.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/optimize/strategies.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/parameters.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/parameters.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/run-task/fetch-content` & `taskcluster-taskgraph-5.1.0/src/taskgraph/run-task/fetch-content`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/run-task/hgrc` & `taskcluster-taskgraph-5.1.0/src/taskgraph/run-task/hgrc`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/run-task/robustcheckout.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/run-task/robustcheckout.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/run-task/run-task` & `taskcluster-taskgraph-5.1.0/src/taskgraph/run-task/run-task`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/target_tasks.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/target_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/task.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/taskgraph.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/taskgraph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/transforms/base.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/transforms/base.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/transforms/cached_tasks.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/transforms/cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/transforms/code_review.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/transforms/code_review.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/transforms/docker_image.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/transforms/docker_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,14 +137,15 @@
         taskdesc = {
             "label": "build-docker-image-" + image_name,
             "description": description,
             "attributes": {
                 "image_name": image_name,
                 "artifact_prefix": "public",
             },
+            "always-target": True,
             "expires-after": "28 days" if config.params.is_try() else "1 year",
             "scopes": [],
             "run-on-projects": [],
             "worker-type": "images",
             "worker": {
                 "implementation": "docker-worker",
                 "os": "linux",
```

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/transforms/fetch.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/transforms/fetch.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/transforms/job/__init__.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/transforms/job/__init__.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/transforms/job/common.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/transforms/job/common.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/transforms/job/index_search.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/transforms/job/index_search.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/transforms/job/run_task.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/transforms/job/run_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,17 @@
             # file. If a value is present in both the provided file and directly
             # in command-context, the latter will take priority.
             Optional("from-file"): str,
             Extra: object,
         },
         # What to execute the command with in the event command is a string.
         Optional("exec-with"): Any(*list(EXEC_COMMANDS)),
+        # Command used to invoke the `run-task` script. Can be used if the script
+        # or Python installation is in a non-standard location on the workers.
+        Optional("run-task-command"): list,
         # Base work directory used to set up the task.
         Required("workdir"): str,
         # Whether to run as root. (defaults to False)
         Optional("run-as-root"): bool,
     }
 )
 
@@ -156,15 +159,15 @@
 
 @run_job_using(
     "docker-worker", "run-task", schema=run_task_schema, defaults=worker_defaults
 )
 def docker_worker_run_task(config, job, taskdesc):
     run = job["run"]
     worker = taskdesc["worker"] = job["worker"]
-    command = ["/usr/local/bin/run-task"]
+    command = run.pop("run-task-command", ["/usr/local/bin/run-task"])
     common_setup(config, job, taskdesc, command)
 
     if run.get("cache-dotcache"):
         worker["caches"].append(
             {
                 "type": "persistent",
                 "name": "{project}-dotcache".format(**config.params),
@@ -199,20 +202,22 @@
 def generic_worker_run_task(config, job, taskdesc):
     run = job["run"]
     worker = taskdesc["worker"] = job["worker"]
     is_win = worker["os"] == "windows"
     is_mac = worker["os"] == "macosx"
     is_bitbar = worker["os"] == "linux-bitbar"
 
-    if is_win:
-        command = ["C:/mozilla-build/python3/python3.exe", "run-task"]
-    elif is_mac:
-        command = ["/tools/python36/bin/python3", "run-task"]
-    else:
-        command = ["./run-task"]
+    command = run.pop("run-task-command", None)
+    if not command:
+        if is_win:
+            command = ["C:/mozilla-build/python3/python3.exe", "run-task"]
+        elif is_mac:
+            command = ["/tools/python36/bin/python3", "run-task"]
+        else:
+            command = ["./run-task"]
 
     common_setup(config, job, taskdesc, command)
 
     worker.setdefault("mounts", [])
     if run.get("cache-dotcache"):
         worker["mounts"].append(
             {
```

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/transforms/job/toolchain.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/transforms/job/toolchain.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/transforms/notify.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/transforms/notify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/transforms/task.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/transforms/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     OptimizationSchema,
     Schema,
     optionally_keyed_by,
     resolve_keyed_by,
     taskref_or_string,
     validate_schema,
 )
-from taskgraph.util.treeherder import split_symbol
+from taskgraph.util.treeherder import split_symbol, treeherder_defaults
 from taskgraph.util.workertypes import worker_type_implementation
 
 from ..util import docker as dockerutil
 from ..util.workertypes import get_worker_type
 
 RUN_TASK = os.path.join(
     os.path.dirname(os.path.dirname(__file__)), "run-task", "run-task"
@@ -91,28 +91,42 @@
         Optional("scopes"): [str],
         # Tags
         Optional("tags"): {str: str},
         # custom "task.extra" content
         Optional("extra"): {str: object},
         # treeherder-related information; see
         # https://schemas.taskcluster.net/taskcluster-treeherder/v1/task-treeherder-config.json
+        # This may be provided in one of two ways:
+        # 1) A simple `true` will cause taskgraph to generate the required information
+        # 2) A dictionary with one or more of the required keys. Any key not present
+        #    will use a default as described below.
         # If not specified, no treeherder extra information or routes will be
         # added to the task
-        Optional("treeherder"): {
-            # either a bare symbol, or "grp(sym)".
-            "symbol": str,
-            # the job kind
-            "kind": Any("build", "test", "other"),
-            # tier for this task
-            "tier": int,
-            # task platform, in the form platform/collection, used to set
-            # treeherder.machine.platform and treeherder.collection or
-            # treeherder.labels
-            "platform": str,
-        },
+        Optional("treeherder"): Any(
+            True,
+            {
+                # either a bare symbol, or "grp(sym)".
+                # The default symbol is the uppercased first letter of each
+                # section of the kind (delimited by "-") all smooshed together.
+                # Eg: "test" becomes "T", "docker-image" becomes "DI", etc.
+                "symbol": Optional(str),
+                # the job kind
+                # If "build" or "test" is found in the kind name, this defaults
+                # to the appropriate value. Otherwise, defaults to "other"
+                "kind": Optional(Any("build", "test", "other")),
+                # tier for this task
+                # Defaults to 1
+                "tier": Optional(int),
+                # task platform, in the form platform/collection, used to set
+                # treeherder.machine.platform and treeherder.collection or
+                # treeherder.labels
+                # Defaults to "default/opt"
+                "platform": Optional(str),
+            },
+        ),
         # information for indexing this build so its artifacts can be discovered;
         # if omitted, the build will not be indexed.
         Optional("index"): {
             # the name of the product this build produces
             "product": str,
             # the names to use for this job in the TaskCluster index
             "job-name": str,
@@ -914,46 +928,14 @@
     for tpl in V2_ROUTE_TEMPLATES:
         routes.append(tpl.format(**subs))
 
     return task
 
 
 @transforms.add
-def add_index_routes(config, tasks):
-    for task in tasks:
-        index = task.get("index", {})
-
-        # The default behavior is to rank tasks according to their tier
-        extra_index = task.setdefault("extra", {}).setdefault("index", {})
-        rank = index.get("rank", "by-tier")
-
-        if rank == "by-tier":
-            # rank is zero for non-tier-1 tasks and based on pushid for others;
-            # this sorts tier-{2,3} builds below tier-1 in the index
-            tier = task.get("treeherder", {}).get("tier", 3)
-            extra_index["rank"] = 0 if tier > 1 else int(config.params["build_date"])
-        elif rank == "build_date":
-            extra_index["rank"] = int(config.params["build_date"])
-        else:
-            extra_index["rank"] = rank
-
-        if not index:
-            yield task
-            continue
-
-        index_type = index.get("type", "generic")
-        if index_type not in index_builders:
-            raise ValueError(f"Unknown index-type {index_type}")
-        task = index_builders[index_type](config, task)
-
-        del task["index"]
-        yield task
-
-
-@transforms.add
 def build_task(config, tasks):
     for task in tasks:
         level = str(config.params["level"])
 
         provisioner_id, worker_type = get_worker_type(
             config.graph_config,
             task["worker-type"],
@@ -968,40 +950,45 @@
         ]
 
         # set up extra
         extra = task.get("extra", {})
         extra["parent"] = os.environ.get("TASK_ID", "")
         task_th = task.get("treeherder")
         if task_th:
-            extra.setdefault("treeherder-platform", task_th["platform"])
-            treeherder = extra.setdefault("treeherder", {})
+            treeherder = extra.setdefault(
+                "treeherder", treeherder_defaults(config.kind, task["label"])
+            )
+            if isinstance(task_th, dict):
+                treeherder.update(task_th)
+
+            extra.setdefault("treeherder-platform", treeherder["platform"])
 
-            machine_platform, collection = task_th["platform"].split("/", 1)
+            machine_platform, collection = treeherder["platform"].split("/", 1)
             treeherder["machine"] = {"platform": machine_platform}
             treeherder["collection"] = {collection: True}
 
             group_names = config.graph_config["treeherder"]["group-names"]
-            groupSymbol, symbol = split_symbol(task_th["symbol"])
+            groupSymbol, symbol = split_symbol(treeherder["symbol"])
             if groupSymbol != "?":
                 treeherder["groupSymbol"] = groupSymbol
                 if groupSymbol not in group_names:
                     path = os.path.join(config.path, task.get("task-from", ""))
                     raise Exception(UNKNOWN_GROUP_NAME.format(groupSymbol, path))
                 treeherder["groupName"] = group_names[groupSymbol]
             treeherder["symbol"] = symbol
             if len(symbol) > 25 or len(groupSymbol) > 25:
                 raise RuntimeError(
                     "Treeherder group and symbol names must not be longer than "
                     "25 characters: {} (see {})".format(
-                        task_th["symbol"],
+                        treeherder["symbol"],
                         TC_TREEHERDER_SCHEMA_URL,
                     )
                 )
-            treeherder["jobKind"] = task_th["kind"]
-            treeherder["tier"] = task_th["tier"]
+            treeherder["jobKind"] = treeherder["kind"]
+            treeherder["tier"] = treeherder["tier"]
 
             branch_rev = get_branch_rev(config)
 
             if config.params["tasks_for"].startswith("github-pull-request"):
                 # In the past we used `project` for this, but that ends up being
                 # set to the repository name of the _head_ repo, which is not correct
                 # (and causes scope issues) if it doesn't match the name of the
@@ -1141,14 +1128,46 @@
             "soft-dependencies": task.get("soft-dependencies", []),
             "attributes": attributes,
             "optimization": task.get("optimization", None),
         }
 
 
 @transforms.add
+def add_index_routes(config, tasks):
+    for task in tasks:
+        index = task.get("index", {})
+
+        # The default behavior is to rank tasks according to their tier
+        extra_index = task.setdefault("extra", {}).setdefault("index", {})
+        rank = index.get("rank", "by-tier")
+
+        if rank == "by-tier":
+            # rank is zero for non-tier-1 tasks and based on pushid for others;
+            # this sorts tier-{2,3} builds below tier-1 in the index
+            tier = task.get("treeherder", {}).get("tier", 3)
+            extra_index["rank"] = 0 if tier > 1 else int(config.params["build_date"])
+        elif rank == "build_date":
+            extra_index["rank"] = int(config.params["build_date"])
+        else:
+            extra_index["rank"] = rank
+
+        if not index:
+            yield task
+            continue
+
+        index_type = index.get("type", "generic")
+        if index_type not in index_builders:
+            raise ValueError(f"Unknown index-type {index_type}")
+        task = index_builders[index_type](config, task)
+
+        del task["index"]
+        yield task
+
+
+@transforms.add
 def add_github_checks(config, tasks):
     """
     For git repositories, add checks route to all tasks.
 
     This will be replaced by a configurable option in the future.
     """
     if config.params["repository_type"] != "git":
```

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/util/archive.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/util/archive.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/util/attributes.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/util/attributes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/util/cached_tasks.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/util/cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/util/decision.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/util/decision.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/util/docker.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/util/docker.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/util/hash.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/util/hash.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/util/keyed_by.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/util/keyed_by.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/util/memoize.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/util/memoize.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/util/parameterization.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/util/parameterization.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/util/path.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/util/path.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         (`'foo'` and `'foo/bar'` both match, but `'foo/bar'` is the deepest match)
     """
     path = normsep(path)
     bases = [normsep(b) for b in bases]
     if path in bases:
         return path
     for b in sorted(bases, reverse=True):
-        if b == "" or path.startswith(b + "/"):
+        if not b or path.startswith(b + "/"):
             return b
 
 
 re_cache = {}
 MATCH_STAR_STAR_RE = re.compile(r"(^|/)\\\*\\\*/")
 MATCH_STAR_STAR_END_RE = re.compile(r"(^|/)\\\*\\\*$")
```

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/util/python_path.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/util/python_path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/util/readonlydict.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/util/readonlydict.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/util/schema.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/util/schema.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/util/shell.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/util/shell.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/util/taskcluster.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/util/taskcluster.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/util/taskgraph.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/util/taskgraph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/util/templates.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/util/templates.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/util/time.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/util/time.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/util/treeherder.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/util/treeherder.py`

 * *Files 16% similar despite different names*

```diff
@@ -58,7 +58,27 @@
     treeherder.setdefault("platform", f"{dep_th_platform}/{dep_th_collection}")
     treeherder.setdefault(
         "tier", dep_job.task.get("extra", {}).get("treeherder", {}).get("tier", 1)
     )
     # Does not set symbol
     treeherder.setdefault("kind", "build")
     return treeherder
+
+
+def treeherder_defaults(kind, label):
+    defaults = {
+        # Despite its name, this is expected to be a platform+collection
+        "platform": "default/opt",
+        "tier": 1,
+    }
+    if "build" in kind:
+        defaults["kind"] = "build"
+    elif "test" in kind:
+        defaults["kind"] = "test"
+    else:
+        defaults["kind"] = "other"
+
+    # Takes the uppercased first letter of each part of the kind name, eg:
+    # apple-banana -> AB
+    defaults["symbol"] = "".join([c[0] for c in kind.split("-")]).upper()
+
+    return defaults
```

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/util/vcs.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/util/vcs.py`

 * *Files 0% similar despite different names*

```diff
@@ -302,15 +302,15 @@
             f"last(ancestors('{base_ref_or_rev}') and ancestors('{head_rev}'))",
             "--template",
             "{node}",
         ).strip()
 
     def does_revision_exist_locally(self, revision):
         try:
-            return self.run("log", "-r", revision).strip() != ""
+            return bool(self.run("log", "-r", revision).strip())
         except subprocess.CalledProcessError as e:
             # Error code 255 comes with the message:
             # "abort: unknown revision $REVISION"
             if e.returncode == 255:
                 return False
             raise
```

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/util/verify.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/util/verify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/util/workertypes.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/util/workertypes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/src/taskgraph/util/yaml.py` & `taskcluster-taskgraph-5.1.0/src/taskgraph/util/yaml.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/test/test_actions_rebuild_cached_tasks.py` & `taskcluster-taskgraph-5.1.0/test/test_actions_rebuild_cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/test/test_actions_registry.py` & `taskcluster-taskgraph-5.1.0/test/test_actions_registry.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/test/test_create.py` & `taskcluster-taskgraph-5.1.0/test/test_create.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/test/test_decision.py` & `taskcluster-taskgraph-5.1.0/test/test_decision.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/test/test_files_changed.py` & `taskcluster-taskgraph-5.1.0/test/test_files_changed.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/test/test_graph.py` & `taskcluster-taskgraph-5.1.0/test/test_graph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/test/test_main.py` & `taskcluster-taskgraph-5.1.0/test/test_main.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/test/test_morph.py` & `taskcluster-taskgraph-5.1.0/test/test_morph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/test/test_optimize.py` & `taskcluster-taskgraph-5.1.0/test/test_optimize.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/test/test_optimize_strategies.py` & `taskcluster-taskgraph-5.1.0/test/test_optimize_strategies.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/test/test_parameters.py` & `taskcluster-taskgraph-5.1.0/test/test_parameters.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/test/test_scripts_fetch_content.py` & `taskcluster-taskgraph-5.1.0/test/test_scripts_fetch_content.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/test/test_scripts_run_task.py` & `taskcluster-taskgraph-5.1.0/test/test_scripts_run_task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/test/test_target_tasks.py` & `taskcluster-taskgraph-5.1.0/test/test_target_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/test/test_taskgraph.py` & `taskcluster-taskgraph-5.1.0/test/test_taskgraph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/test/test_transforms_base.py` & `taskcluster-taskgraph-5.1.0/test/test_transforms_base.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/test/test_transforms_fetch.py` & `taskcluster-taskgraph-5.1.0/test/test_transforms_fetch.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/test/test_transforms_job.py` & `taskcluster-taskgraph-5.1.0/test/test_transforms_job.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/test/test_transforms_job_run_task.py` & `taskcluster-taskgraph-5.1.0/test/test_transforms_job_run_task.py`

 * *Files 10% similar despite different names*

```diff
@@ -142,14 +142,41 @@
         "powershell.exe",
         "-ExecutionPolicy",
         "Bypass",
         "echo hello world",
     ]
 
 
+def assert_run_task_command_docker_worker(task):
+    assert task["worker"]["command"] == [
+        "/foo/bar/python3",
+        "run-task",
+        "--ci-checkout=/builds/worker/checkouts/vcs/",
+        "--",
+        "bash",
+        "-cx",
+        "echo hello world",
+    ]
+
+
+def assert_run_task_command_generic_worker(task):
+    assert task["worker"]["command"] == [
+        ["chmod", "+x", "run-task"],
+        [
+            "/foo/bar/python3",
+            "run-task",
+            "--ci-checkout=./checkouts/vcs/",
+            "--",
+            "bash",
+            "-cx",
+            "echo hello world",
+        ],
+    ]
+
+
 @pytest.mark.parametrize(
     "task",
     (
         pytest.param(
             {},
             id="docker_worker",
         ),
@@ -167,14 +194,29 @@
             {
                 "run": {
                     "exec-with": "powershell",
                 },
             },
             id="exec_with",
         ),
+        pytest.param(
+            {
+                "run": {"run-task-command": ["/foo/bar/python3", "run-task"]},
+            },
+            id="run_task_command_docker_worker",
+        ),
+        pytest.param(
+            {
+                "run": {"run-task-command": ["/foo/bar/python3", "run-task"]},
+                "worker": {
+                    "implementation": "generic-worker",
+                },
+            },
+            id="run_task_command_generic_worker",
+        ),
     ),
 )
 def test_run_task(request, run_job_using, task):
     taskdesc = run_job_using(task)
     print("Task Description:")
     pprint(taskdesc)
     param_id = request.node.callspec.id
```

### Comparing `taskcluster-taskgraph-5.0.1/test/test_transforms_job_toolchain.py` & `taskcluster-taskgraph-5.1.0/test/test_transforms_job_toolchain.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/test/test_transforms_notify.py` & `taskcluster-taskgraph-5.1.0/test/test_transforms_notify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/test/test_util_attributes.py` & `taskcluster-taskgraph-5.1.0/test/test_util_attributes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/test/test_util_docker.py` & `taskcluster-taskgraph-5.1.0/test/test_util_docker.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/test/test_util_memoize.py` & `taskcluster-taskgraph-5.1.0/test/test_util_memoize.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/test/test_util_parameterization.py` & `taskcluster-taskgraph-5.1.0/test/test_util_parameterization.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/test/test_util_path.py` & `taskcluster-taskgraph-5.1.0/test/test_util_path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/test/test_util_python_path.py` & `taskcluster-taskgraph-5.1.0/test/test_util_python_path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/test/test_util_readonlydict.py` & `taskcluster-taskgraph-5.1.0/test/test_util_readonlydict.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/test/test_util_schema.py` & `taskcluster-taskgraph-5.1.0/test/test_util_schema.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/test/test_util_taskcluster.py` & `taskcluster-taskgraph-5.1.0/test/test_util_taskcluster.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/test/test_util_templates.py` & `taskcluster-taskgraph-5.1.0/test/test_util_templates.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/test/test_util_time.py` & `taskcluster-taskgraph-5.1.0/test/test_util_time.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/test/test_util_treeherder.py` & `taskcluster-taskgraph-5.1.0/test/test_util_treeherder.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/test/test_util_vcs.py` & `taskcluster-taskgraph-5.1.0/test/test_util_vcs.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/test/test_util_verify.py` & `taskcluster-taskgraph-5.1.0/test/test_util_verify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/test/test_util_workertypes.py` & `taskcluster-taskgraph-5.1.0/test/test_util_workertypes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.0.1/test/test_util_yaml.py` & `taskcluster-taskgraph-5.1.0/test/test_util_yaml.py`

 * *Files identical despite different names*

