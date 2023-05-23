# Comparing `tmp/dstack-0.9.post1.tar.gz` & `tmp/dstack-0.9rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dstack-0.9.post1.tar", last modified: Mon May 22 08:55:00 2023, max compression
+gzip compressed data, was "dstack-0.9rc2.tar", last modified: Mon May 22 10:07:01 2023, max compression
```

## Comparing `dstack-0.9.post1.tar` & `dstack-0.9rc2.tar`

### file list

```diff
@@ -1,273 +1,273 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.895295 dstack-0.9.post1/
--rw-r--r--   0 runner    (1001) docker     (123)    15976 2023-05-22 08:54:04.000000 dstack-0.9.post1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-05-22 08:55:00.895295 dstack-0.9.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-05-22 08:54:04.000000 dstack-0.9.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.875295 dstack-0.9.post1/cli/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.875295 dstack-0.9.post1/cli/dstack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.875295 dstack-0.9.post1/cli/dstack/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.879295 dstack-0.9.post1/cli/dstack/api/hub/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/api/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19505 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/api/hub/_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11650 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/api/hub/_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/api/hub/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/api/hub/_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/api/hub/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/api/repos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/api/runs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.879295 dstack-0.9.post1/cli/dstack/backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.879295 dstack-0.9.post1/cli/dstack/backend/aws/
--rw-r--r--   0 runner    (1001) docker     (123)     9192 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/aws/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/aws/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/aws/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/aws/repos.py
--rw-r--r--   0 runner    (1001) docker     (123)    22378 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/aws/runners.py
--rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/aws/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/aws/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/aws/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.879295 dstack-0.9.post1/cli/dstack/backend/azure/
--rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14195 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/azure/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/azure/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/azure/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/azure/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/azure/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/azure/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.879295 dstack-0.9.post1/cli/dstack/backend/base/
--rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/base/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/base/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/base/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/base/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9539 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/base/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/base/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/base/repos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/base/runners.py
--rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/base/runs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/base/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/base/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/base/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.879295 dstack-0.9.post1/cli/dstack/backend/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28759 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/gcp/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/gcp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/gcp/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/gcp/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/gcp/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/gcp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.883295 dstack-0.9.post1/cli/dstack/backend/local/
--rw-r--r--   0 runner    (1001) docker     (123)     7654 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/local/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/local/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/local/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/local/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/local/runners.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/local/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/local/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.883295 dstack-0.9.post1/cli/dstack/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.883295 dstack-0.9.post1/cli/dstack/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/cli/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.883295 dstack-0.9.post1/cli/dstack/cli/commands/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/cli/commands/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.883295 dstack-0.9.post1/cli/dstack/cli/commands/cp/
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/cli/commands/cp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.883295 dstack-0.9.post1/cli/dstack/cli/commands/init/
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/cli/commands/init/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.883295 dstack-0.9.post1/cli/dstack/cli/commands/logs/
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/cli/commands/logs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.883295 dstack-0.9.post1/cli/dstack/cli/commands/ls/
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/cli/commands/ls/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.883295 dstack-0.9.post1/cli/dstack/cli/commands/prune/
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/cli/commands/prune/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.883295 dstack-0.9.post1/cli/dstack/cli/commands/ps/
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/cli/commands/ps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.883295 dstack-0.9.post1/cli/dstack/cli/commands/resubmit/
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/cli/commands/resubmit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.883295 dstack-0.9.post1/cli/dstack/cli/commands/rm/
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/cli/commands/rm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.883295 dstack-0.9.post1/cli/dstack/cli/commands/run/
--rw-r--r--   0 runner    (1001) docker     (123)    11390 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/cli/commands/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/cli/commands/run/ssh_tunnel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.883295 dstack-0.9.post1/cli/dstack/cli/commands/secrets/
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/cli/commands/secrets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.883295 dstack-0.9.post1/cli/dstack/cli/commands/start/
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/cli/commands/start/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.883295 dstack-0.9.post1/cli/dstack/cli/commands/stop/
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/cli/commands/stop/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.883295 dstack-0.9.post1/cli/dstack/cli/commands/tags/
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/cli/commands/tags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/cli/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/cli/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/cli/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/cli/updates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.887295 dstack-0.9.post1/cli/dstack/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/core/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/core/artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/core/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/core/dependents.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/core/error.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/core/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    16854 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/core/job.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/core/log_event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.887295 dstack-0.9.post1/cli/dstack/core/repo/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/core/repo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/core/repo/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/core/repo/head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/core/repo/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/core/repo/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/core/repo/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/core/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/core/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/core/runners.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/core/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/core/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/core/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/core/userconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.887295 dstack-0.9.post1/cli/dstack/hub/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.887295 dstack-0.9.post1/cli/dstack/hub/background/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/background/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.887295 dstack-0.9.post1/cli/dstack/hub/background/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/background/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/background/tasks/resubmit_jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.887295 dstack-0.9.post1/cli/dstack/hub/db/
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/db/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/db/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.887295 dstack-0.9.post1/cli/dstack/hub/migration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/migration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/migration/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.887295 dstack-0.9.post1/cli/dstack/hub/migration/versions/
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/migration/versions/3b900659c822_.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/migration/versions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.887295 dstack-0.9.post1/cli/dstack/hub/models/
--rw-r--r--   0 runner    (1001) docker     (123)     7094 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.887295 dstack-0.9.post1/cli/dstack/hub/repository/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/repository/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/repository/users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.887295 dstack-0.9.post1/cli/dstack/hub/routers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/routers/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/routers/backends.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/routers/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/routers/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/routers/link.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/routers/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/routers/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/routers/repos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/routers/runners.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/routers/runs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/routers/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/routers/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/routers/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/routers/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/routers/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/routers/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.887295 dstack-0.9.post1/cli/dstack/hub/security/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/security/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/security/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.887295 dstack-0.9.post1/cli/dstack/hub/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.887295 dstack-0.9.post1/cli/dstack/hub/services/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/services/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.887295 dstack-0.9.post1/cli/dstack/hub/services/backends/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/services/backends/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/services/backends/aws/configurator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.891295 dstack-0.9.post1/cli/dstack/hub/services/backends/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/services/backends/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/services/backends/azure/azure_identity_credential_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    34538 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/services/backends/azure/configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/services/backends/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.891295 dstack-0.9.post1/cli/dstack/hub/services/backends/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/services/backends/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11910 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/services/backends/gcp/configurator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.891295 dstack-0.9.post1/cli/dstack/hub/services/backends/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/services/backends/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/services/backends/local/configurator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.891295 dstack-0.9.post1/cli/dstack/hub/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/utils/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.891295 dstack-0.9.post1/cli/dstack/providers/
--rw-r--r--   0 runner    (1001) docker     (123)    18660 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.891295 dstack-0.9.post1/cli/dstack/providers/_torchrun/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/providers/_torchrun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/providers/_torchrun/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.891295 dstack-0.9.post1/cli/dstack/providers/bash/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/providers/bash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/providers/bash/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.891295 dstack-0.9.post1/cli/dstack/providers/code/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/providers/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/providers/code/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.891295 dstack-0.9.post1/cli/dstack/providers/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/providers/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/providers/docker/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.891295 dstack-0.9.post1/cli/dstack/providers/lab/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/providers/lab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/providers/lab/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.891295 dstack-0.9.post1/cli/dstack/providers/notebook/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/providers/notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/providers/notebook/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.891295 dstack-0.9.post1/cli/dstack/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.891295 dstack-0.9.post1/cli/dstack/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/utils/escape.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/utils/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/utils/interpolator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/utils/random_names.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/utils/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/utils/workflows.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-22 08:54:59.000000 dstack-0.9.post1/cli/dstack/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.875295 dstack-0.9.post1/cli/dstack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-05-22 08:55:00.000000 dstack-0.9.post1/cli/dstack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-22 08:55:00.000000 dstack-0.9.post1/cli/dstack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 08:55:00.000000 dstack-0.9.post1/cli/dstack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-22 08:55:00.000000 dstack-0.9.post1/cli/dstack.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-22 08:55:00.000000 dstack-0.9.post1/cli/dstack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-22 08:55:00.000000 dstack-0.9.post1/cli/dstack.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.891295 dstack-0.9.post1/cli/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.891295 dstack-0.9.post1/cli/tests/backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/tests/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.891295 dstack-0.9.post1/cli/tests/backend/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/tests/backend/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/tests/backend/base/test_logs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.891295 dstack-0.9.post1/cli/tests/hub/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/tests/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/tests/hub/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/tests/hub/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.891295 dstack-0.9.post1/cli/tests/hub/routers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/tests/hub/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/tests/hub/routers/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/tests/hub/routers/test_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/tests/hub/routers/test_users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.891295 dstack-0.9.post1/cli/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/tests/integration/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7213 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/tests/integration/test_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.891295 dstack-0.9.post1/cli/tests/providers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/tests/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.891295 dstack-0.9.post1/cli/tests/providers/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/tests/providers/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/tests/providers/docker/test_entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/tests/providers/test_local_path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.895295 dstack-0.9.post1/cli/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/tests/utils/escape.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/tests/utils/test_interpolator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/tests/utils/test_merge_workflow_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/tests/utils/test_tarignore.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 08:55:00.895295 dstack-0.9.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-05-22 08:54:04.000000 dstack-0.9.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.521556 dstack-0.9rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)    15976 2023-05-22 10:05:51.000000 dstack-0.9rc2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-05-22 10:07:01.517555 dstack-0.9rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-05-22 10:05:51.000000 dstack-0.9rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.485555 dstack-0.9rc2/cli/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.489555 dstack-0.9rc2/cli/dstack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.489555 dstack-0.9rc2/cli/dstack/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.489555 dstack-0.9rc2/cli/dstack/api/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/api/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19505 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/api/hub/_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11650 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/api/hub/_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/api/hub/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/api/hub/_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/api/hub/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/api/repos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/api/runs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.489555 dstack-0.9rc2/cli/dstack/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.493555 dstack-0.9rc2/cli/dstack/backend/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)     9192 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/backend/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/backend/aws/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/backend/aws/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/backend/aws/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/backend/aws/repos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22378 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/backend/aws/runners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/backend/aws/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/backend/aws/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/backend/aws/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.493555 dstack-0.9rc2/cli/dstack/backend/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/backend/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14195 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/backend/azure/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/backend/azure/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/backend/azure/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/backend/azure/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/backend/azure/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/backend/azure/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.493555 dstack-0.9rc2/cli/dstack/backend/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/backend/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/backend/base/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/backend/base/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/backend/base/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/backend/base/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9539 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/backend/base/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/backend/base/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/backend/base/repos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/backend/base/runners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/backend/base/runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/backend/base/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/backend/base/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/backend/base/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.497555 dstack-0.9rc2/cli/dstack/backend/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/backend/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28759 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/backend/gcp/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/backend/gcp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/backend/gcp/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/backend/gcp/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/backend/gcp/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/backend/gcp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.497555 dstack-0.9rc2/cli/dstack/backend/local/
+-rw-r--r--   0 runner    (1001) docker     (123)     7654 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/backend/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/backend/local/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/backend/local/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/backend/local/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/backend/local/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/backend/local/runners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/backend/local/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/backend/local/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.497555 dstack-0.9rc2/cli/dstack/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.497555 dstack-0.9rc2/cli/dstack/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/cli/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.497555 dstack-0.9rc2/cli/dstack/cli/commands/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/cli/commands/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.497555 dstack-0.9rc2/cli/dstack/cli/commands/cp/
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/cli/commands/cp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.497555 dstack-0.9rc2/cli/dstack/cli/commands/init/
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/cli/commands/init/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.497555 dstack-0.9rc2/cli/dstack/cli/commands/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/cli/commands/logs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.497555 dstack-0.9rc2/cli/dstack/cli/commands/ls/
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/cli/commands/ls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.497555 dstack-0.9rc2/cli/dstack/cli/commands/prune/
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/cli/commands/prune/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.497555 dstack-0.9rc2/cli/dstack/cli/commands/ps/
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/cli/commands/ps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.497555 dstack-0.9rc2/cli/dstack/cli/commands/resubmit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/cli/commands/resubmit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.497555 dstack-0.9rc2/cli/dstack/cli/commands/rm/
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/cli/commands/rm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.497555 dstack-0.9rc2/cli/dstack/cli/commands/run/
+-rw-r--r--   0 runner    (1001) docker     (123)    11390 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/cli/commands/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/cli/commands/run/ssh_tunnel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.501555 dstack-0.9rc2/cli/dstack/cli/commands/secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/cli/commands/secrets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.501555 dstack-0.9rc2/cli/dstack/cli/commands/start/
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/cli/commands/start/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.501555 dstack-0.9rc2/cli/dstack/cli/commands/stop/
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/cli/commands/stop/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.501555 dstack-0.9rc2/cli/dstack/cli/commands/tags/
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/cli/commands/tags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/cli/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/cli/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/cli/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/cli/updates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.501555 dstack-0.9rc2/cli/dstack/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/core/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/core/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/core/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/core/dependents.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/core/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/core/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16854 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/core/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/core/log_event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.505555 dstack-0.9rc2/cli/dstack/core/repo/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/core/repo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/core/repo/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/core/repo/head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/core/repo/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/core/repo/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/core/repo/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/core/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/core/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/core/runners.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/core/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/core/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/core/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/core/userconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.505555 dstack-0.9rc2/cli/dstack/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.505555 dstack-0.9rc2/cli/dstack/hub/background/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/background/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.505555 dstack-0.9rc2/cli/dstack/hub/background/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/background/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/background/tasks/resubmit_jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.505555 dstack-0.9rc2/cli/dstack/hub/db/
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/db/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/db/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.505555 dstack-0.9rc2/cli/dstack/hub/migration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/migration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/migration/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.505555 dstack-0.9rc2/cli/dstack/hub/migration/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/migration/versions/3b900659c822_.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/migration/versions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.505555 dstack-0.9rc2/cli/dstack/hub/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     7094 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.505555 dstack-0.9rc2/cli/dstack/hub/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/repository/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/repository/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.509555 dstack-0.9rc2/cli/dstack/hub/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/routers/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/routers/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/routers/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/routers/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/routers/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/routers/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/routers/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/routers/repos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/routers/runners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/routers/runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/routers/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/routers/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/routers/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/routers/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/routers/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/routers/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.509555 dstack-0.9rc2/cli/dstack/hub/security/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/security/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/security/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.509555 dstack-0.9rc2/cli/dstack/hub/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.509555 dstack-0.9rc2/cli/dstack/hub/services/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/services/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.509555 dstack-0.9rc2/cli/dstack/hub/services/backends/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/services/backends/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/services/backends/aws/configurator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.513555 dstack-0.9rc2/cli/dstack/hub/services/backends/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/services/backends/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/services/backends/azure/azure_identity_credential_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34538 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/services/backends/azure/configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/services/backends/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.513555 dstack-0.9rc2/cli/dstack/hub/services/backends/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/services/backends/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11910 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/services/backends/gcp/configurator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.513555 dstack-0.9rc2/cli/dstack/hub/services/backends/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/services/backends/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/services/backends/local/configurator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.513555 dstack-0.9rc2/cli/dstack/hub/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/hub/utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.513555 dstack-0.9rc2/cli/dstack/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)    18660 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.513555 dstack-0.9rc2/cli/dstack/providers/_torchrun/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/providers/_torchrun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/providers/_torchrun/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.513555 dstack-0.9rc2/cli/dstack/providers/bash/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/providers/bash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/providers/bash/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.513555 dstack-0.9rc2/cli/dstack/providers/code/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/providers/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/providers/code/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.513555 dstack-0.9rc2/cli/dstack/providers/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/providers/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/providers/docker/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.513555 dstack-0.9rc2/cli/dstack/providers/lab/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/providers/lab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/providers/lab/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.513555 dstack-0.9rc2/cli/dstack/providers/notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/providers/notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/providers/notebook/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.513555 dstack-0.9rc2/cli/dstack/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.513555 dstack-0.9rc2/cli/dstack/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/utils/escape.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/utils/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/utils/interpolator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/utils/random_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/utils/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/dstack/utils/workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-22 10:07:00.000000 dstack-0.9rc2/cli/dstack/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.489555 dstack-0.9rc2/cli/dstack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-05-22 10:07:01.000000 dstack-0.9rc2/cli/dstack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-22 10:07:01.000000 dstack-0.9rc2/cli/dstack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 10:07:01.000000 dstack-0.9rc2/cli/dstack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-22 10:07:01.000000 dstack-0.9rc2/cli/dstack.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-22 10:07:01.000000 dstack-0.9rc2/cli/dstack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-22 10:07:01.000000 dstack-0.9rc2/cli/dstack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.517555 dstack-0.9rc2/cli/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.517555 dstack-0.9rc2/cli/tests/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/tests/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.517555 dstack-0.9rc2/cli/tests/backend/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/tests/backend/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/tests/backend/base/test_logs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.517555 dstack-0.9rc2/cli/tests/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/tests/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/tests/hub/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/tests/hub/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.517555 dstack-0.9rc2/cli/tests/hub/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/tests/hub/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/tests/hub/routers/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/tests/hub/routers/test_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/tests/hub/routers/test_users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.517555 dstack-0.9rc2/cli/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/tests/integration/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7213 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/tests/integration/test_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.517555 dstack-0.9rc2/cli/tests/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/tests/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.517555 dstack-0.9rc2/cli/tests/providers/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/tests/providers/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/tests/providers/docker/test_entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/tests/providers/test_local_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:07:01.517555 dstack-0.9rc2/cli/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/tests/utils/escape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/tests/utils/test_interpolator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/tests/utils/test_merge_workflow_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-22 10:05:51.000000 dstack-0.9rc2/cli/tests/utils/test_tarignore.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 10:07:01.521556 dstack-0.9rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-05-22 10:05:51.000000 dstack-0.9rc2/setup.py
```

### Comparing `dstack-0.9.post1/LICENSE.md` & `dstack-0.9rc2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/PKG-INFO` & `dstack-0.9rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dstack
-Version: 0.9.post1
+Version: 0.9rc2
 Summary: Develop ML faster. Easily and cost-effectively run dev environments, pipelines, and apps on any cloud.
 Home-page: https://dstack.ai
 Author: Andrey Cheptsov
 Author-email: andrey@dstack.ai
 License: UNKNOWN
 Project-URL: Source, https://github.com/dstackai/dstack
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: dstack Version: 0.9.post1 Summary: Develop ML
-faster. Easily and cost-effectively run dev environments, pipelines, and apps
-on any cloud. Home-page: https://dstack.ai Author: Andrey Cheptsov Author-
-email: andrey@dstack.ai License: UNKNOWN Project-URL: Source, https://
-github.com/dstackai/dstack Platform: UNKNOWN Classifier: Development Status ::
-2 - Pre-Alpha Classifier: Topic :: Scientific/Engineering :: Artificial
-Intelligence Classifier: License :: OSI Approved :: Mozilla Public License 2.0
-(MPL 2.0) Classifier: Programming Language :: Python :: 3 Requires-Python:
->=3.7 Description-Content-Type: text/markdown Provides-Extra: aws Provides-
-Extra: azure Provides-Extra: gcp License-File: LICENSE.md
+Metadata-Version: 2.1 Name: dstack Version: 0.9rc2 Summary: Develop ML faster.
+Easily and cost-effectively run dev environments, pipelines, and apps on any
+cloud. Home-page: https://dstack.ai Author: Andrey Cheptsov Author-email:
+andrey@dstack.ai License: UNKNOWN Project-URL: Source, https://github.com/
+dstackai/dstack Platform: UNKNOWN Classifier: Development Status :: 2 - Pre-
+Alpha Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
+Classifier: Programming Language :: Python :: 3 Requires-Python: >=3.7
+Description-Content-Type: text/markdown Provides-Extra: aws Provides-Extra:
+azure Provides-Extra: gcp License-File: LICENSE.md
                             ****** [dstack] ******
                   **** Develop ML faster. Use any cloud. ****
                      Docs â¢ Examples â¢ Blog â¢ Slack
       [![Last commit](https://img.shields.io/github/last-commit/dstackai/
 dstack?style=flat-square)](https://github.com/dstackai/dstack/commits/) [![PyPI
 - License](https://img.shields.io/pypi/l/dstack?style=flat-square&color=blue)]
           (https://github.com/dstackai/dstack/blob/master/LICENSE.md)
```

### Comparing `dstack-0.9.post1/README.md` & `dstack-0.9rc2/README.md`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/api/hub/_api_client.py` & `dstack-0.9rc2/cli/dstack/api/hub/_api_client.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/api/hub/_client.py` & `dstack-0.9rc2/cli/dstack/api/hub/_client.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/api/hub/_storage.py` & `dstack-0.9rc2/cli/dstack/api/hub/_storage.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/api/repos.py` & `dstack-0.9rc2/cli/dstack/api/repos.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/api/runs.py` & `dstack-0.9rc2/cli/dstack/api/runs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/backend/aws/__init__.py` & `dstack-0.9rc2/cli/dstack/backend/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/backend/aws/compute.py` & `dstack-0.9rc2/cli/dstack/backend/aws/compute.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/backend/aws/config.py` & `dstack-0.9rc2/cli/dstack/backend/aws/config.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/backend/aws/logs.py` & `dstack-0.9rc2/cli/dstack/backend/aws/logs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/backend/aws/runners.py` & `dstack-0.9rc2/cli/dstack/backend/aws/runners.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/backend/aws/secrets.py` & `dstack-0.9rc2/cli/dstack/backend/aws/secrets.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/backend/aws/storage.py` & `dstack-0.9rc2/cli/dstack/backend/aws/storage.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/backend/aws/utils.py` & `dstack-0.9rc2/cli/dstack/backend/aws/utils.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/backend/azure/__init__.py` & `dstack-0.9rc2/cli/dstack/backend/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/backend/azure/compute.py` & `dstack-0.9rc2/cli/dstack/backend/azure/compute.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/backend/azure/config.py` & `dstack-0.9rc2/cli/dstack/backend/azure/config.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/backend/azure/logs.py` & `dstack-0.9rc2/cli/dstack/backend/azure/logs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/backend/azure/secrets.py` & `dstack-0.9rc2/cli/dstack/backend/azure/secrets.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/backend/azure/storage.py` & `dstack-0.9rc2/cli/dstack/backend/azure/storage.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/backend/azure/utils.py` & `dstack-0.9rc2/cli/dstack/backend/azure/utils.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/backend/base/__init__.py` & `dstack-0.9rc2/cli/dstack/backend/base/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/backend/base/artifacts.py` & `dstack-0.9rc2/cli/dstack/backend/base/artifacts.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/backend/base/compute.py` & `dstack-0.9rc2/cli/dstack/backend/base/compute.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/backend/base/config.py` & `dstack-0.9rc2/cli/dstack/backend/base/config.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/backend/base/jobs.py` & `dstack-0.9rc2/cli/dstack/backend/base/jobs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/backend/base/logs.py` & `dstack-0.9rc2/cli/dstack/backend/base/logs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/backend/base/repos.py` & `dstack-0.9rc2/cli/dstack/backend/base/repos.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/backend/base/runners.py` & `dstack-0.9rc2/cli/dstack/backend/base/runners.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/backend/base/runs.py` & `dstack-0.9rc2/cli/dstack/backend/base/runs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/backend/base/secrets.py` & `dstack-0.9rc2/cli/dstack/backend/base/secrets.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/backend/base/storage.py` & `dstack-0.9rc2/cli/dstack/backend/base/storage.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/backend/base/tags.py` & `dstack-0.9rc2/cli/dstack/backend/base/tags.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/backend/gcp/__init__.py` & `dstack-0.9rc2/cli/dstack/backend/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/backend/gcp/compute.py` & `dstack-0.9rc2/cli/dstack/backend/gcp/compute.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/backend/gcp/config.py` & `dstack-0.9rc2/cli/dstack/backend/gcp/config.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/backend/gcp/logs.py` & `dstack-0.9rc2/cli/dstack/backend/gcp/logs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/backend/gcp/secrets.py` & `dstack-0.9rc2/cli/dstack/backend/gcp/secrets.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/backend/gcp/storage.py` & `dstack-0.9rc2/cli/dstack/backend/gcp/storage.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/backend/gcp/utils.py` & `dstack-0.9rc2/cli/dstack/backend/gcp/utils.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/backend/local/__init__.py` & `dstack-0.9rc2/cli/dstack/backend/local/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/backend/local/compute.py` & `dstack-0.9rc2/cli/dstack/backend/local/compute.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/backend/local/config.py` & `dstack-0.9rc2/cli/dstack/backend/local/config.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/backend/local/logs.py` & `dstack-0.9rc2/cli/dstack/backend/local/logs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/backend/local/runners.py` & `dstack-0.9rc2/cli/dstack/backend/local/runners.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/backend/local/secrets.py` & `dstack-0.9rc2/cli/dstack/backend/local/secrets.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/backend/local/storage.py` & `dstack-0.9rc2/cli/dstack/backend/local/storage.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/cli/commands/__init__.py` & `dstack-0.9rc2/cli/dstack/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/cli/commands/config/__init__.py` & `dstack-0.9rc2/cli/dstack/cli/commands/config/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/cli/commands/cp/__init__.py` & `dstack-0.9rc2/cli/dstack/cli/commands/cp/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/cli/commands/init/__init__.py` & `dstack-0.9rc2/cli/dstack/cli/commands/init/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/cli/commands/logs/__init__.py` & `dstack-0.9rc2/cli/dstack/cli/commands/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/cli/commands/ls/__init__.py` & `dstack-0.9rc2/cli/dstack/cli/commands/ls/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/cli/commands/prune/__init__.py` & `dstack-0.9rc2/cli/dstack/cli/commands/prune/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/cli/commands/ps/__init__.py` & `dstack-0.9rc2/cli/dstack/cli/commands/ps/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/cli/commands/resubmit/__init__.py` & `dstack-0.9rc2/cli/dstack/cli/commands/resubmit/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/cli/commands/rm/__init__.py` & `dstack-0.9rc2/cli/dstack/cli/commands/rm/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/cli/commands/run/__init__.py` & `dstack-0.9rc2/cli/dstack/cli/commands/run/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/cli/commands/run/ssh_tunnel.py` & `dstack-0.9rc2/cli/dstack/cli/commands/run/ssh_tunnel.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/cli/commands/secrets/__init__.py` & `dstack-0.9rc2/cli/dstack/cli/commands/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/cli/commands/start/__init__.py` & `dstack-0.9rc2/cli/dstack/cli/commands/start/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/cli/commands/stop/__init__.py` & `dstack-0.9rc2/cli/dstack/cli/commands/stop/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/cli/commands/tags/__init__.py` & `dstack-0.9rc2/cli/dstack/cli/commands/tags/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/cli/common.py` & `dstack-0.9rc2/cli/dstack/cli/common.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/cli/config.py` & `dstack-0.9rc2/cli/dstack/cli/config.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/cli/handlers.py` & `dstack-0.9rc2/cli/dstack/cli/handlers.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/cli/main.py` & `dstack-0.9rc2/cli/dstack/cli/main.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/cli/updates.py` & `dstack-0.9rc2/cli/dstack/cli/updates.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/core/app.py` & `dstack-0.9rc2/cli/dstack/core/app.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/core/error.py` & `dstack-0.9rc2/cli/dstack/core/error.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/core/job.py` & `dstack-0.9rc2/cli/dstack/core/job.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/core/repo/base.py` & `dstack-0.9rc2/cli/dstack/core/repo/base.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/core/repo/head.py` & `dstack-0.9rc2/cli/dstack/core/repo/head.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/core/repo/local.py` & `dstack-0.9rc2/cli/dstack/core/repo/local.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/core/repo/remote.py` & `dstack-0.9rc2/cli/dstack/core/repo/remote.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/core/repo/spec.py` & `dstack-0.9rc2/cli/dstack/core/repo/spec.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/core/request.py` & `dstack-0.9rc2/cli/dstack/core/request.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/core/run.py` & `dstack-0.9rc2/cli/dstack/core/run.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/core/runners.py` & `dstack-0.9rc2/cli/dstack/core/runners.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/core/tag.py` & `dstack-0.9rc2/cli/dstack/core/tag.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/hub/background/tasks/resubmit_jobs.py` & `dstack-0.9rc2/cli/dstack/hub/background/tasks/resubmit_jobs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/hub/db/__init__.py` & `dstack-0.9rc2/cli/dstack/hub/db/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/hub/db/models.py` & `dstack-0.9rc2/cli/dstack/hub/db/models.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/hub/main.py` & `dstack-0.9rc2/cli/dstack/hub/main.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/hub/migration/env.py` & `dstack-0.9rc2/cli/dstack/hub/migration/env.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/hub/migration/versions/3b900659c822_.py` & `dstack-0.9rc2/cli/dstack/hub/migration/versions/3b900659c822_.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/hub/models/__init__.py` & `dstack-0.9rc2/cli/dstack/hub/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/hub/repository/projects.py` & `dstack-0.9rc2/cli/dstack/hub/repository/projects.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/hub/repository/users.py` & `dstack-0.9rc2/cli/dstack/hub/repository/users.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/hub/routers/artifacts.py` & `dstack-0.9rc2/cli/dstack/hub/routers/artifacts.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/hub/routers/cache.py` & `dstack-0.9rc2/cli/dstack/hub/routers/cache.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/hub/routers/jobs.py` & `dstack-0.9rc2/cli/dstack/hub/routers/jobs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/hub/routers/link.py` & `dstack-0.9rc2/cli/dstack/hub/routers/link.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/hub/routers/logs.py` & `dstack-0.9rc2/cli/dstack/hub/routers/logs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/hub/routers/projects.py` & `dstack-0.9rc2/cli/dstack/hub/routers/projects.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/hub/routers/repos.py` & `dstack-0.9rc2/cli/dstack/hub/routers/repos.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/hub/routers/runners.py` & `dstack-0.9rc2/cli/dstack/hub/routers/runners.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/hub/routers/runs.py` & `dstack-0.9rc2/cli/dstack/hub/routers/runs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/hub/routers/secrets.py` & `dstack-0.9rc2/cli/dstack/hub/routers/secrets.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/hub/routers/storage.py` & `dstack-0.9rc2/cli/dstack/hub/routers/storage.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/hub/routers/tags.py` & `dstack-0.9rc2/cli/dstack/hub/routers/tags.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/hub/routers/users.py` & `dstack-0.9rc2/cli/dstack/hub/routers/users.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/hub/routers/util.py` & `dstack-0.9rc2/cli/dstack/hub/routers/util.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/hub/routers/workflows.py` & `dstack-0.9rc2/cli/dstack/hub/routers/workflows.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/hub/security/permissions.py` & `dstack-0.9rc2/cli/dstack/hub/security/permissions.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/hub/services/backends/__init__.py` & `dstack-0.9rc2/cli/dstack/hub/services/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/hub/services/backends/aws/configurator.py` & `dstack-0.9rc2/cli/dstack/hub/services/backends/aws/configurator.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/hub/services/backends/azure/azure_identity_credential_adapter.py` & `dstack-0.9rc2/cli/dstack/hub/services/backends/azure/azure_identity_credential_adapter.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/hub/services/backends/azure/configurator.py` & `dstack-0.9rc2/cli/dstack/hub/services/backends/azure/configurator.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/hub/services/backends/base.py` & `dstack-0.9rc2/cli/dstack/hub/services/backends/base.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/hub/services/backends/gcp/configurator.py` & `dstack-0.9rc2/cli/dstack/hub/services/backends/gcp/configurator.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/hub/services/backends/local/configurator.py` & `dstack-0.9rc2/cli/dstack/hub/services/backends/local/configurator.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/hub/utils/logging.py` & `dstack-0.9rc2/cli/dstack/hub/utils/logging.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/providers/__init__.py` & `dstack-0.9rc2/cli/dstack/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/providers/_torchrun/main.py` & `dstack-0.9rc2/cli/dstack/providers/_torchrun/main.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/providers/bash/main.py` & `dstack-0.9rc2/cli/dstack/providers/bash/main.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/providers/code/main.py` & `dstack-0.9rc2/cli/dstack/providers/code/main.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/providers/docker/main.py` & `dstack-0.9rc2/cli/dstack/providers/docker/main.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/providers/lab/main.py` & `dstack-0.9rc2/cli/dstack/providers/lab/main.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/providers/notebook/main.py` & `dstack-0.9rc2/cli/dstack/providers/notebook/main.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/utils/common.py` & `dstack-0.9rc2/cli/dstack/utils/common.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/utils/escape.py` & `dstack-0.9rc2/cli/dstack/utils/escape.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/utils/hash.py` & `dstack-0.9rc2/cli/dstack/utils/hash.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/utils/interpolator.py` & `dstack-0.9rc2/cli/dstack/utils/interpolator.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/utils/random_names.py` & `dstack-0.9rc2/cli/dstack/utils/random_names.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/utils/ssh.py` & `dstack-0.9rc2/cli/dstack/utils/ssh.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack/utils/workflows.py` & `dstack-0.9rc2/cli/dstack/utils/workflows.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack.egg-info/PKG-INFO` & `dstack-0.9rc2/cli/dstack.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dstack
-Version: 0.9.post1
+Version: 0.9rc2
 Summary: Develop ML faster. Easily and cost-effectively run dev environments, pipelines, and apps on any cloud.
 Home-page: https://dstack.ai
 Author: Andrey Cheptsov
 Author-email: andrey@dstack.ai
 License: UNKNOWN
 Project-URL: Source, https://github.com/dstackai/dstack
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: dstack Version: 0.9.post1 Summary: Develop ML
-faster. Easily and cost-effectively run dev environments, pipelines, and apps
-on any cloud. Home-page: https://dstack.ai Author: Andrey Cheptsov Author-
-email: andrey@dstack.ai License: UNKNOWN Project-URL: Source, https://
-github.com/dstackai/dstack Platform: UNKNOWN Classifier: Development Status ::
-2 - Pre-Alpha Classifier: Topic :: Scientific/Engineering :: Artificial
-Intelligence Classifier: License :: OSI Approved :: Mozilla Public License 2.0
-(MPL 2.0) Classifier: Programming Language :: Python :: 3 Requires-Python:
->=3.7 Description-Content-Type: text/markdown Provides-Extra: aws Provides-
-Extra: azure Provides-Extra: gcp License-File: LICENSE.md
+Metadata-Version: 2.1 Name: dstack Version: 0.9rc2 Summary: Develop ML faster.
+Easily and cost-effectively run dev environments, pipelines, and apps on any
+cloud. Home-page: https://dstack.ai Author: Andrey Cheptsov Author-email:
+andrey@dstack.ai License: UNKNOWN Project-URL: Source, https://github.com/
+dstackai/dstack Platform: UNKNOWN Classifier: Development Status :: 2 - Pre-
+Alpha Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
+Classifier: Programming Language :: Python :: 3 Requires-Python: >=3.7
+Description-Content-Type: text/markdown Provides-Extra: aws Provides-Extra:
+azure Provides-Extra: gcp License-File: LICENSE.md
                             ****** [dstack] ******
                   **** Develop ML faster. Use any cloud. ****
                      Docs â¢ Examples â¢ Blog â¢ Slack
       [![Last commit](https://img.shields.io/github/last-commit/dstackai/
 dstack?style=flat-square)](https://github.com/dstackai/dstack/commits/) [![PyPI
 - License](https://img.shields.io/pypi/l/dstack?style=flat-square&color=blue)]
           (https://github.com/dstackai/dstack/blob/master/LICENSE.md)
```

### Comparing `dstack-0.9.post1/cli/dstack.egg-info/SOURCES.txt` & `dstack-0.9rc2/cli/dstack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/dstack.egg-info/requires.txt` & `dstack-0.9rc2/cli/dstack.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/tests/backend/base/test_logs.py` & `dstack-0.9rc2/cli/tests/backend/base/test_logs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/tests/hub/common.py` & `dstack-0.9rc2/cli/tests/hub/common.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/tests/hub/routers/test_jobs.py` & `dstack-0.9rc2/cli/tests/hub/routers/test_jobs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/tests/hub/routers/test_projects.py` & `dstack-0.9rc2/cli/tests/hub/routers/test_projects.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/tests/hub/routers/test_users.py` & `dstack-0.9rc2/cli/tests/hub/routers/test_users.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/tests/integration/common.py` & `dstack-0.9rc2/cli/tests/integration/common.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/tests/integration/conftest.py` & `dstack-0.9rc2/cli/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/tests/integration/test_commands.py` & `dstack-0.9rc2/cli/tests/integration/test_commands.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/tests/providers/docker/test_entrypoint.py` & `dstack-0.9rc2/cli/tests/providers/docker/test_entrypoint.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/tests/providers/test_local_path.py` & `dstack-0.9rc2/cli/tests/providers/test_local_path.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/tests/utils/escape.py` & `dstack-0.9rc2/cli/tests/utils/escape.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/tests/utils/test_interpolator.py` & `dstack-0.9rc2/cli/tests/utils/test_interpolator.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/tests/utils/test_merge_workflow_data.py` & `dstack-0.9rc2/cli/tests/utils/test_merge_workflow_data.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/cli/tests/utils/test_tarignore.py` & `dstack-0.9rc2/cli/tests/utils/test_tarignore.py`

 * *Files identical despite different names*

### Comparing `dstack-0.9.post1/setup.py` & `dstack-0.9rc2/setup.py`

 * *Files identical despite different names*

