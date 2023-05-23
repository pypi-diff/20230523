# Comparing `tmp/DLRN-0.9.0.tar.gz` & `tmp/DLRN-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/DLRN-0.9.0.tar", last modified: Thu Aug 16 13:04:41 2018, max compression
+gzip compressed data, was "dist/DLRN-0.9.1.tar", last modified: Mon Nov  5 14:58:33 2018, max compression
```

## Comparing `DLRN-0.9.0.tar` & `DLRN-0.9.1.tar`

### file list

```diff
@@ -1,163 +1,163 @@
-drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2018-08-16 13:04:41.000000 DLRN-0.9.0/
-drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2018-08-16 13:04:41.000000 DLRN-0.9.0/DLRN.egg-info/
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     4374 2018-08-16 13:04:41.000000 DLRN-0.9.0/DLRN.egg-info/PKG-INFO
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     3745 2018-08-16 13:04:41.000000 DLRN-0.9.0/DLRN.egg-info/SOURCES.txt
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)        1 2018-08-16 13:04:41.000000 DLRN-0.9.0/DLRN.egg-info/dependency_links.txt
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      174 2018-08-16 13:04:41.000000 DLRN-0.9.0/DLRN.egg-info/entry_points.txt
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)        1 2018-08-16 13:04:41.000000 DLRN-0.9.0/DLRN.egg-info/not-zip-safe
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)       46 2018-08-16 13:04:41.000000 DLRN-0.9.0/DLRN.egg-info/pbr.json
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      196 2018-08-16 13:04:41.000000 DLRN-0.9.0/DLRN.egg-info/requires.txt
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)        5 2018-08-16 13:04:41.000000 DLRN-0.9.0/DLRN.egg-info/top_level.txt
-drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2018-08-16 13:04:41.000000 DLRN-0.9.0/dlrn/
-drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2018-08-16 13:04:41.000000 DLRN-0.9.0/dlrn/api/
-drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2018-08-16 13:04:41.000000 DLRN-0.9.0/dlrn/api/static/
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1097 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/api/static/styles.css
-drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2018-08-16 13:04:41.000000 DLRN-0.9.0/dlrn/api/templates/
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     5486 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/api/templates/report.j2
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     5844 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/api/templates/votes.j2
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     3489 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/api/templates/votes_general.j2
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      785 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/api/__init__.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)       91 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/api/config.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)    25244 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/api/dlrn_api.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1664 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/api/utils.py
-drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2018-08-16 13:04:41.000000 DLRN-0.9.0/dlrn/drivers/
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)        0 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/drivers/__init__.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      829 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/drivers/buildrpm.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     5199 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/drivers/coprdriver.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     9076 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/drivers/downstream.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)    10699 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/drivers/gitrepo.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     8866 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/drivers/kojidriver.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     4238 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/drivers/mockdriver.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1634 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/drivers/pkginfo.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     8461 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/drivers/rdoinfo.py
-drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2018-08-16 13:04:41.000000 DLRN-0.9.0/dlrn/migrations/
-drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2018-08-16 13:04:41.000000 DLRN-0.9.0/dlrn/migrations/versions/
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1405 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/migrations/versions/1268c799620f_add_commit_branch_to_db.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     3209 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/migrations/versions/2a0313a8a7d6_change_user_usernames_column_length.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     2338 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/migrations/versions/3c62b0d3ec34_initial_creation.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1409 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/migrations/versions/47ebe0522809_scheme_change_due_to_scm_support_moving_.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1419 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/migrations/versions/4a5651777e5e_add_promotions_table.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1937 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/migrations/versions/638f980c9169_add_tables_required_by_dlrn_api.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1575 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/migrations/versions/ade85b2396bc_add_extended_hash_and_dt_extended_columns_to_.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1996 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/migrations/versions/cab7697f6564_add_user_column_to_civote_and_promotion.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     3778 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/migrations/versions/f38ba3389b85_set_string_length.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)       38 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/migrations/README
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     2608 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/migrations/env.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1042 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/migrations/script.py.mako
-drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2018-08-16 13:04:41.000000 DLRN-0.9.0/dlrn/stylesheets/
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      973 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/stylesheets/styles.css
-drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2018-08-16 13:04:41.000000 DLRN-0.9.0/dlrn/templates/
-drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2018-08-16 13:04:41.000000 DLRN-0.9.0/dlrn/templates/stylesheets/
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      973 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/templates/stylesheets/styles.css
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      357 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/templates/notification_email.j2
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      981 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/templates/queue.j2
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1704 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/templates/report.j2
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     2233 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/templates/status_report.j2
-drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2018-08-16 13:04:41.000000 DLRN-0.9.0/dlrn/tests/
-drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2018-08-16 13:04:41.000000 DLRN-0.9.0/dlrn/tests/samples/
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)    12463 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/tests/samples/commits_1.yaml
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     2384 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/tests/samples/commits_2.yaml
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1099 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/tests/samples/commits_remote.yaml
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     3262 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/tests/samples/versions.csv
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)        0 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/tests/__init__.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1919 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/tests/base.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)    30898 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/tests/test_api.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     4884 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/tests/test_build.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1838 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/tests/test_config.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     6515 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/tests/test_db.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     3705 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/tests/test_driver_copr.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     4030 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/tests/test_driver_downstream.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1942 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/tests/test_driver_git.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)    10473 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/tests/test_driver_koji.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     4898 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/tests/test_driver_mock.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     4176 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/tests/test_notifications.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     2728 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/tests/test_purge.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     2018 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/tests/test_remote.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     3993 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/tests/test_repositories.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     4641 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/tests/test_rpmspecfile.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     3603 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/tests/test_rsync.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     9119 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/tests/test_shell.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     6374 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/tests/test_user.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     3236 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/tests/test_utils.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      660 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/__init__.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)    11547 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/build.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     8014 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/config.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     7057 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/db.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     3797 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/notifications.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     6709 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/purge.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     7454 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/remote.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     6591 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/reporting.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     5124 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/repositories.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     6732 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/rpmspecfile.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     3262 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/rsync.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)    31859 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/shell.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     5243 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/user.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     8027 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/utils.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      659 2018-08-16 13:04:23.000000 DLRN-0.9.0/dlrn/version.py
-drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2018-08-16 13:04:41.000000 DLRN-0.9.0/doc/
-drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2018-08-16 13:04:41.000000 DLRN-0.9.0/doc/source/
-drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2018-08-16 13:04:41.000000 DLRN-0.9.0/doc/source/_images/
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)    43951 2018-08-16 13:04:23.000000 DLRN-0.9.0/doc/source/_images/DLRN.png
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)   462492 2018-08-16 13:04:23.000000 DLRN-0.9.0/doc/source/_images/DLRN.svg
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     5370 2018-08-16 13:04:23.000000 DLRN-0.9.0/doc/source/Makefile
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)    22016 2018-08-16 13:04:23.000000 DLRN-0.9.0/doc/source/api.rst
--rwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)     9111 2018-08-16 13:04:23.000000 DLRN-0.9.0/doc/source/conf.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)       35 2018-08-16 13:04:23.000000 DLRN-0.9.0/doc/source/contributing.rst
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      414 2018-08-16 13:04:23.000000 DLRN-0.9.0/doc/source/index.rst
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)    18770 2018-08-16 13:04:23.000000 DLRN-0.9.0/doc/source/installation.rst
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)    11604 2018-08-16 13:04:23.000000 DLRN-0.9.0/doc/source/internals.rst
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      115 2018-08-16 13:04:23.000000 DLRN-0.9.0/doc/source/intro.rst
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     5243 2018-08-16 13:04:23.000000 DLRN-0.9.0/doc/source/repositories.rst
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      696 2018-08-16 13:04:23.000000 DLRN-0.9.0/doc/source/troubleshooting.rst
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     8581 2018-08-16 13:04:23.000000 DLRN-0.9.0/doc/source/usage.rst
-drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2018-08-16 13:04:41.000000 DLRN-0.9.0/doc/specs/
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     9043 2018-08-16 13:04:23.000000 DLRN-0.9.0/doc/specs/zuul-based-architecture.rst
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)    20588 2018-08-16 13:04:23.000000 DLRN-0.9.0/doc/api_definition.yaml
-drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2018-08-16 13:04:41.000000 DLRN-0.9.0/playbooks/
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)       63 2018-08-16 13:04:23.000000 DLRN-0.9.0/playbooks/README.md
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      469 2018-08-16 13:04:23.000000 DLRN-0.9.0/playbooks/dlrn-api-functional-getlogs.yaml
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     6348 2018-08-16 13:04:23.000000 DLRN-0.9.0/playbooks/dlrn-api-functional.yaml
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1086 2018-08-16 13:04:23.000000 DLRN-0.9.0/playbooks/prepare.yaml
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      362 2018-08-16 13:04:23.000000 DLRN-0.9.0/playbooks/retrieve-logs.yaml
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      245 2018-08-16 13:04:23.000000 DLRN-0.9.0/playbooks/rpmbuild.yaml
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      334 2018-08-16 13:04:23.000000 DLRN-0.9.0/playbooks/tripleo-ci-getlogs.yaml
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      334 2018-08-16 13:04:23.000000 DLRN-0.9.0/playbooks/tripleo-ci-oooq-getlogs.yaml
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     2954 2018-08-16 13:04:23.000000 DLRN-0.9.0/playbooks/tripleo-ci-oooq.yaml
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1196 2018-08-16 13:04:23.000000 DLRN-0.9.0/playbooks/tripleo-ci.yaml
-drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2018-08-16 13:04:41.000000 DLRN-0.9.0/scripts/
--rwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)       67 2018-08-16 13:04:23.000000 DLRN-0.9.0/scripts/api.py
--rwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)     1898 2018-08-16 13:04:23.000000 DLRN-0.9.0/scripts/bisect.sh
--rwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)     6238 2018-08-16 13:04:23.000000 DLRN-0.9.0/scripts/build_srpm.sh
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1611 2018-08-16 13:04:23.000000 DLRN-0.9.0/scripts/centos.cfg
--rwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)     2569 2018-08-16 13:04:23.000000 DLRN-0.9.0/scripts/common-functions
--rwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)     1604 2018-08-16 13:04:23.000000 DLRN-0.9.0/scripts/db_migrate.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1043 2018-08-16 13:04:23.000000 DLRN-0.9.0/scripts/fedora.cfg
--rwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)     1505 2018-08-16 13:04:23.000000 DLRN-0.9.0/scripts/get_rdo_review.py
--rwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)     1489 2018-08-16 13:04:23.000000 DLRN-0.9.0/scripts/map-distgit-name
--rwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)     1173 2018-08-16 13:04:23.000000 DLRN-0.9.0/scripts/map-project-name
--rwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)     2709 2018-08-16 13:04:23.000000 DLRN-0.9.0/scripts/recreate-promotion-symlinks.py
--rwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)     3329 2018-08-16 13:04:23.000000 DLRN-0.9.0/scripts/run_project_tests.sh
--rwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)     4934 2018-08-16 13:04:23.000000 DLRN-0.9.0/scripts/run_sh_tests.sh
--rwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)     6982 2018-08-16 13:04:23.000000 DLRN-0.9.0/scripts/run_tests.sh
--rwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)     2186 2018-08-16 13:04:23.000000 DLRN-0.9.0/scripts/submit_review.sh
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      109 2018-08-16 13:04:23.000000 DLRN-0.9.0/.coveragerc
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)       88 2018-08-16 13:04:23.000000 DLRN-0.9.0/.mailmap
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      318 2018-08-16 13:04:23.000000 DLRN-0.9.0/.testr.conf
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1827 2018-08-16 13:04:23.000000 DLRN-0.9.0/.zuul.yaml
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1567 2018-08-16 13:04:41.000000 DLRN-0.9.0/AUTHORS
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     2451 2018-08-16 13:04:23.000000 DLRN-0.9.0/CONTRIBUTING.rst
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)    24584 2018-08-16 13:04:41.000000 DLRN-0.9.0/ChangeLog
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      168 2018-08-16 13:04:23.000000 DLRN-0.9.0/HACKING.rst
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)    10142 2018-08-16 13:04:23.000000 DLRN-0.9.0/LICENSE
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)       93 2018-08-16 13:04:23.000000 DLRN-0.9.0/MANIFEST.in
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     2754 2018-08-16 13:04:23.000000 DLRN-0.9.0/README.rst
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1465 2018-08-16 13:04:23.000000 DLRN-0.9.0/alembic.ini
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)       16 2018-08-16 13:04:23.000000 DLRN-0.9.0/babel.cfg
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      201 2018-08-16 13:04:23.000000 DLRN-0.9.0/bindep.txt
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1848 2018-08-16 13:04:23.000000 DLRN-0.9.0/projects.ini
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      196 2018-08-16 13:04:23.000000 DLRN-0.9.0/requirements.txt
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1054 2018-08-16 13:04:41.000000 DLRN-0.9.0/setup.cfg
--rwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)      781 2018-08-16 13:04:23.000000 DLRN-0.9.0/setup.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      211 2018-08-16 13:04:23.000000 DLRN-0.9.0/test-requirements.txt
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1483 2018-08-16 13:04:23.000000 DLRN-0.9.0/tox.ini
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     4374 2018-08-16 13:04:41.000000 DLRN-0.9.0/PKG-INFO
+drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2018-11-05 14:58:33.000000 DLRN-0.9.1/
+drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2018-11-05 14:58:33.000000 DLRN-0.9.1/DLRN.egg-info/
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     4374 2018-11-05 14:58:33.000000 DLRN-0.9.1/DLRN.egg-info/PKG-INFO
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     3745 2018-11-05 14:58:33.000000 DLRN-0.9.1/DLRN.egg-info/SOURCES.txt
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)        1 2018-11-05 14:58:33.000000 DLRN-0.9.1/DLRN.egg-info/dependency_links.txt
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      174 2018-11-05 14:58:33.000000 DLRN-0.9.1/DLRN.egg-info/entry_points.txt
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)        1 2018-11-05 14:58:33.000000 DLRN-0.9.1/DLRN.egg-info/not-zip-safe
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)       46 2018-11-05 14:58:33.000000 DLRN-0.9.1/DLRN.egg-info/pbr.json
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      196 2018-11-05 14:58:33.000000 DLRN-0.9.1/DLRN.egg-info/requires.txt
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)        5 2018-11-05 14:58:33.000000 DLRN-0.9.1/DLRN.egg-info/top_level.txt
+drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2018-11-05 14:58:33.000000 DLRN-0.9.1/dlrn/
+drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2018-11-05 14:58:33.000000 DLRN-0.9.1/dlrn/api/
+drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2018-11-05 14:58:33.000000 DLRN-0.9.1/dlrn/api/static/
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1097 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/api/static/styles.css
+drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2018-11-05 14:58:33.000000 DLRN-0.9.1/dlrn/api/templates/
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     5486 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/api/templates/report.j2
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     5844 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/api/templates/votes.j2
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     3489 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/api/templates/votes_general.j2
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      785 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/api/__init__.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)       91 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/api/config.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)    25190 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/api/dlrn_api.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1664 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/api/utils.py
+drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2018-11-05 14:58:33.000000 DLRN-0.9.1/dlrn/drivers/
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)        0 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/drivers/__init__.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      829 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/drivers/buildrpm.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     5294 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/drivers/coprdriver.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)    12348 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/drivers/downstream.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)    11028 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/drivers/gitrepo.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)    11662 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/drivers/kojidriver.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     4381 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/drivers/mockdriver.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1634 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/drivers/pkginfo.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     8573 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/drivers/rdoinfo.py
+drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2018-11-05 14:58:33.000000 DLRN-0.9.1/dlrn/migrations/
+drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2018-11-05 14:58:33.000000 DLRN-0.9.1/dlrn/migrations/versions/
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1405 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/migrations/versions/1268c799620f_add_commit_branch_to_db.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     3209 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/migrations/versions/2a0313a8a7d6_change_user_usernames_column_length.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     2338 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/migrations/versions/3c62b0d3ec34_initial_creation.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1409 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/migrations/versions/47ebe0522809_scheme_change_due_to_scm_support_moving_.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1419 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/migrations/versions/4a5651777e5e_add_promotions_table.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1937 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/migrations/versions/638f980c9169_add_tables_required_by_dlrn_api.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1575 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/migrations/versions/ade85b2396bc_add_extended_hash_and_dt_extended_columns_to_.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1996 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/migrations/versions/cab7697f6564_add_user_column_to_civote_and_promotion.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     3778 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/migrations/versions/f38ba3389b85_set_string_length.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)       38 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/migrations/README
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     2608 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/migrations/env.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1042 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/migrations/script.py.mako
+drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2018-11-05 14:58:33.000000 DLRN-0.9.1/dlrn/stylesheets/
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      973 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/stylesheets/styles.css
+drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2018-11-05 14:58:33.000000 DLRN-0.9.1/dlrn/templates/
+drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2018-11-05 14:58:33.000000 DLRN-0.9.1/dlrn/templates/stylesheets/
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      973 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/templates/stylesheets/styles.css
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      357 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/templates/notification_email.j2
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      981 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/templates/queue.j2
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1704 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/templates/report.j2
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     2233 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/templates/status_report.j2
+drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2018-11-05 14:58:33.000000 DLRN-0.9.1/dlrn/tests/
+drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2018-11-05 14:58:33.000000 DLRN-0.9.1/dlrn/tests/samples/
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)    12463 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/tests/samples/commits_1.yaml
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     2384 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/tests/samples/commits_2.yaml
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1099 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/tests/samples/commits_remote.yaml
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     3262 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/tests/samples/versions.csv
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)        0 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/tests/__init__.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1919 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/tests/base.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)    30898 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/tests/test_api.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     5713 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/tests/test_build.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     2270 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/tests/test_config.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     6515 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/tests/test_db.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     3887 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/tests/test_driver_copr.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     6882 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/tests/test_driver_downstream.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1993 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/tests/test_driver_git.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)    11694 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/tests/test_driver_koji.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     5390 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/tests/test_driver_mock.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     4122 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/tests/test_notifications.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     2728 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/tests/test_purge.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     2018 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/tests/test_remote.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     3939 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/tests/test_repositories.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     4641 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/tests/test_rpmspecfile.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     3549 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/tests/test_rsync.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     9050 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/tests/test_shell.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     6374 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/tests/test_user.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     3236 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/tests/test_utils.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      660 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/__init__.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)    12369 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/build.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     4412 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/config.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     7057 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/db.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     3797 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/notifications.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     6709 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/purge.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     7400 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/remote.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     6591 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/reporting.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     5124 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/repositories.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     6732 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/rpmspecfile.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     3262 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/rsync.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)    31344 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/shell.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     5189 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/user.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     8141 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/utils.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      659 2018-11-05 14:58:11.000000 DLRN-0.9.1/dlrn/version.py
+drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2018-11-05 14:58:33.000000 DLRN-0.9.1/doc/
+drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2018-11-05 14:58:33.000000 DLRN-0.9.1/doc/source/
+drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2018-11-05 14:58:33.000000 DLRN-0.9.1/doc/source/_images/
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)    43951 2018-11-05 14:58:11.000000 DLRN-0.9.1/doc/source/_images/DLRN.png
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)   462492 2018-11-05 14:58:11.000000 DLRN-0.9.1/doc/source/_images/DLRN.svg
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     5370 2018-11-05 14:58:11.000000 DLRN-0.9.1/doc/source/Makefile
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)    22016 2018-11-05 14:58:11.000000 DLRN-0.9.1/doc/source/api.rst
+-rwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)     9111 2018-11-05 14:58:11.000000 DLRN-0.9.1/doc/source/conf.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)       35 2018-11-05 14:58:11.000000 DLRN-0.9.1/doc/source/contributing.rst
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      414 2018-11-05 14:58:11.000000 DLRN-0.9.1/doc/source/index.rst
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)    19707 2018-11-05 14:58:11.000000 DLRN-0.9.1/doc/source/installation.rst
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)    11604 2018-11-05 14:58:11.000000 DLRN-0.9.1/doc/source/internals.rst
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      115 2018-11-05 14:58:11.000000 DLRN-0.9.1/doc/source/intro.rst
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     5243 2018-11-05 14:58:11.000000 DLRN-0.9.1/doc/source/repositories.rst
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      696 2018-11-05 14:58:11.000000 DLRN-0.9.1/doc/source/troubleshooting.rst
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     8581 2018-11-05 14:58:11.000000 DLRN-0.9.1/doc/source/usage.rst
+drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2018-11-05 14:58:33.000000 DLRN-0.9.1/doc/specs/
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     9043 2018-11-05 14:58:11.000000 DLRN-0.9.1/doc/specs/zuul-based-architecture.rst
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)    20588 2018-11-05 14:58:11.000000 DLRN-0.9.1/doc/api_definition.yaml
+drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2018-11-05 14:58:33.000000 DLRN-0.9.1/playbooks/
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)       63 2018-11-05 14:58:11.000000 DLRN-0.9.1/playbooks/README.md
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      469 2018-11-05 14:58:11.000000 DLRN-0.9.1/playbooks/dlrn-api-functional-getlogs.yaml
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     6343 2018-11-05 14:58:11.000000 DLRN-0.9.1/playbooks/dlrn-api-functional.yaml
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1086 2018-11-05 14:58:11.000000 DLRN-0.9.1/playbooks/prepare.yaml
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      362 2018-11-05 14:58:11.000000 DLRN-0.9.1/playbooks/retrieve-logs.yaml
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      245 2018-11-05 14:58:11.000000 DLRN-0.9.1/playbooks/rpmbuild.yaml
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      334 2018-11-05 14:58:11.000000 DLRN-0.9.1/playbooks/tripleo-ci-getlogs.yaml
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      334 2018-11-05 14:58:11.000000 DLRN-0.9.1/playbooks/tripleo-ci-oooq-getlogs.yaml
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     2954 2018-11-05 14:58:11.000000 DLRN-0.9.1/playbooks/tripleo-ci-oooq.yaml
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1196 2018-11-05 14:58:11.000000 DLRN-0.9.1/playbooks/tripleo-ci.yaml
+drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2018-11-05 14:58:33.000000 DLRN-0.9.1/scripts/
+-rwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)       67 2018-11-05 14:58:11.000000 DLRN-0.9.1/scripts/api.py
+-rwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)     1898 2018-11-05 14:58:11.000000 DLRN-0.9.1/scripts/bisect.sh
+-rwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)     6240 2018-11-05 14:58:11.000000 DLRN-0.9.1/scripts/build_srpm.sh
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1611 2018-11-05 14:58:11.000000 DLRN-0.9.1/scripts/centos.cfg
+-rwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)     2569 2018-11-05 14:58:11.000000 DLRN-0.9.1/scripts/common-functions
+-rwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)     1604 2018-11-05 14:58:11.000000 DLRN-0.9.1/scripts/db_migrate.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1043 2018-11-05 14:58:11.000000 DLRN-0.9.1/scripts/fedora.cfg
+-rwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)     1505 2018-11-05 14:58:11.000000 DLRN-0.9.1/scripts/get_rdo_review.py
+-rwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)     1610 2018-11-05 14:58:11.000000 DLRN-0.9.1/scripts/map-distgit-name
+-rwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)     1294 2018-11-05 14:58:11.000000 DLRN-0.9.1/scripts/map-project-name
+-rwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)     2709 2018-11-05 14:58:11.000000 DLRN-0.9.1/scripts/recreate-promotion-symlinks.py
+-rwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)     3329 2018-11-05 14:58:11.000000 DLRN-0.9.1/scripts/run_project_tests.sh
+-rwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)     4934 2018-11-05 14:58:11.000000 DLRN-0.9.1/scripts/run_sh_tests.sh
+-rwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)     7016 2018-11-05 14:58:11.000000 DLRN-0.9.1/scripts/run_tests.sh
+-rwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)     2186 2018-11-05 14:58:11.000000 DLRN-0.9.1/scripts/submit_review.sh
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      109 2018-11-05 14:58:11.000000 DLRN-0.9.1/.coveragerc
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)       88 2018-11-05 14:58:11.000000 DLRN-0.9.1/.mailmap
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      318 2018-11-05 14:58:11.000000 DLRN-0.9.1/.testr.conf
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1827 2018-11-05 14:58:11.000000 DLRN-0.9.1/.zuul.yaml
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1650 2018-11-05 14:58:33.000000 DLRN-0.9.1/AUTHORS
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     2451 2018-11-05 14:58:11.000000 DLRN-0.9.1/CONTRIBUTING.rst
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)    25031 2018-11-05 14:58:33.000000 DLRN-0.9.1/ChangeLog
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      168 2018-11-05 14:58:11.000000 DLRN-0.9.1/HACKING.rst
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)    10142 2018-11-05 14:58:11.000000 DLRN-0.9.1/LICENSE
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)       93 2018-11-05 14:58:11.000000 DLRN-0.9.1/MANIFEST.in
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     2754 2018-11-05 14:58:11.000000 DLRN-0.9.1/README.rst
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1465 2018-11-05 14:58:11.000000 DLRN-0.9.1/alembic.ini
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)       16 2018-11-05 14:58:11.000000 DLRN-0.9.1/babel.cfg
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      201 2018-11-05 14:58:11.000000 DLRN-0.9.1/bindep.txt
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1928 2018-11-05 14:58:11.000000 DLRN-0.9.1/projects.ini
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      196 2018-11-05 14:58:11.000000 DLRN-0.9.1/requirements.txt
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1054 2018-11-05 14:58:33.000000 DLRN-0.9.1/setup.cfg
+-rwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)      781 2018-11-05 14:58:11.000000 DLRN-0.9.1/setup.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      211 2018-11-05 14:58:11.000000 DLRN-0.9.1/test-requirements.txt
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1483 2018-11-05 14:58:11.000000 DLRN-0.9.1/tox.ini
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     4374 2018-11-05 14:58:33.000000 DLRN-0.9.1/PKG-INFO
```

### Comparing `DLRN-0.9.0/DLRN.egg-info/PKG-INFO` & `DLRN-0.9.1/DLRN.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: DLRN
-Version: 0.9.0
+Version: 0.9.1
 Summary: Build packages
 Home-page: http://www.openstack.org/
 Author: OpenStack
 Author-email: openstack-dev@lists.openstack.org
 License: UNKNOWN
 Description: ====
         DLRN
```

### Comparing `DLRN-0.9.0/DLRN.egg-info/SOURCES.txt` & `DLRN-0.9.1/DLRN.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/dlrn/api/static/styles.css` & `DLRN-0.9.1/dlrn/api/static/styles.css`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/dlrn/api/templates/report.j2` & `DLRN-0.9.1/dlrn/api/templates/report.j2`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/dlrn/api/templates/votes.j2` & `DLRN-0.9.1/dlrn/api/templates/votes.j2`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/dlrn/api/templates/votes_general.j2` & `DLRN-0.9.1/dlrn/api/templates/votes_general.j2`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/dlrn/api/__init__.py` & `DLRN-0.9.1/dlrn/api/__init__.py`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/dlrn/api/dlrn_api.py` & `DLRN-0.9.1/dlrn/api/dlrn_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 from dlrn.db import getCommits
 from dlrn.db import getSession
 from dlrn.db import Promotion
 
 from dlrn.config import ConfigOptions
 
 from dlrn.remote import import_commit
-from dlrn.shell import default_options
 
 from flask import jsonify
 from flask import render_template
 from flask import request
 
 import calendar
 import os
@@ -44,15 +43,15 @@
 
 
 pagination_limit = 100
 max_limit = 100
 
 
 def _get_config_options(config_file):
-    cp = configparser.RawConfigParser(default_options)
+    cp = configparser.RawConfigParser()
     cp.read(config_file)
     return ConfigOptions(cp)
 
 
 def _repo_hash(commit):
     return "%s_%s" % (commit.commit_hash, commit.distro_hash[:8])
```

### Comparing `DLRN-0.9.0/dlrn/api/utils.py` & `DLRN-0.9.1/dlrn/api/utils.py`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/dlrn/drivers/buildrpm.py` & `DLRN-0.9.1/dlrn/drivers/buildrpm.py`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/dlrn/drivers/coprdriver.py` & `DLRN-0.9.1/dlrn/drivers/coprdriver.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,20 @@
 logging.basicConfig(level=logging.ERROR,
                     format='%(asctime)s %(levelname)s:%(name)s:%(message)s')
 logger = logging.getLogger("dlrn-build-copr")
 logger.setLevel(logging.INFO)
 
 
 class CoprBuildDriver(BuildRPMDriver):
+    DRIVER_CONFIG = {
+        'coprbuild_driver': {
+            'coprid': {},
+        }
+    }
+
     def __init__(self, *args, **kwargs):
         super(CoprBuildDriver, self).__init__(*args, **kwargs)
         self.exe_name = 'copr'
 
     # We are using this method to "tee" copr output to a log file and stdout
     def _process_copr_output(self, line):
         if dlrn.shell.verbose_build:
```

### Comparing `DLRN-0.9.0/dlrn/drivers/downstream.py` & `DLRN-0.9.1/dlrn/drivers/rdoinfo.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,158 +6,122 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
+# The RdoInfoDriver provides the following:
+#
+# 1- A getpackages function based on output provided by rdoinfo
+#    (https://github.com/redhat-openstack/rdoinfo)
+#
+# 2- A getinfo function based on a multi-distgit repo paradigm
+#
+# 3- A preprocess function that is only used if the distgit directory
+#    containts a .spec.j2 file
 
 from dlrn.db import Commit
 from dlrn.drivers.pkginfo import PkgInfoDriver
+from dlrn.repositories import getdistrobranch
 from dlrn.repositories import getsourcebranch
 from dlrn.repositories import refreshrepo
 
-import csv
 import logging
 import os
 import sh
 
-from distroinfo import info
 from distroinfo import query
-from six.moves.urllib.request import urlopen
+from distroinfo import info
 
 
 logging.basicConfig(level=logging.ERROR)
-logger = logging.getLogger("dlrn-downstream-driver")
+logger = logging.getLogger("dlrn-rdoinfo-driver")
 logger.setLevel(logging.INFO)
+rdoinfo_repo = ('https://raw.githubusercontent.com/'
+                'redhat-openstack/rdoinfo/master/')
 
-
-def fail_req_attr_missing(attr_name, package):
-    raise Exception(
-        "Missing required attribute '%s' "
-        "for package: %s (project: %s)" % (
-            attr_name, package['project'], package['name']))
+def buildtagsonly(package):
+    return ('tags' in package and package['tags'] is not None and
+            'build-tags-only' in package['tags'] or
+            'build-tags-only' in package)
 
 
-def fail_req_config_missing(opt_name):
-    raise Exception(
-        "Missing required config option '%s' "
-        "for dlrn.drivers.downstream driver." % opt_name)
-
-
-class DownstreamInfoDriver(PkgInfoDriver):
+class RdoInfoDriver(PkgInfoDriver):
+    DRIVER_CONFIG = {
+        'rdoinfo_driver': {
+            'rdoinfo_repo': {'name': 'repo'},
+        }
+    }
 
     def __init__(self, *args, **kwargs):
-        super(DownstreamInfoDriver, self).__init__(*args, **kwargs)
+        super(RdoInfoDriver, self).__init__(*args, **kwargs)
 
     def getpackages(self, **kwargs):
-        """Valid parameters:
-
+        """ Valid parameters:
         :param local_info_repo: local rdoinfo repo to use instead of fetching
-                                the default one using distroinfo.
-        :param tags: release tags to use (mitaka, newton, etc).
+                                the default one using rdopkg.
+        :param tags: OpenStack release tags to use (mitaka, newton, etc).
         """
         local_info_repo = kwargs.get('local_info_repo')
         tags = kwargs.get('tags')
-
-        info_files = self.config_options.info_files
-        if not info_files:
-            fail_req_config_missing('info_file')
-
         inforepo = None
+
         if local_info_repo:
             inforepo = info.DistroInfo(
-                info_files=info_files,
+                info_files='rdo.yml',
                 local_info=local_info_repo)
         elif self.config_options.rdoinfo_repo:
             inforepo = info.DistroInfo(
-                info_files=info_files,
+                info_files='rdo.yml',
                 remote_git_info=self.config_options.rdoinfo_repo)
         else:
-            fail_req_config_missing('repo')
+            # distroinfo will fetch info files from the rdoinfo repo as needed
+            # and store them under ~/.distroinfo/cache
+            inforepo = info.DistroInfo(
+                info_files='rdo.yml',
+                remote_info=rdoinfo_repo)
+
         pkginfo = inforepo.get_info(apply_tag=tags)
 
         self.packages = pkginfo["packages"]
         if tags:
             # FIXME allow list of tags?
             self.packages = query.filter_pkgs(self.packages, {'tags': tags})
-        if self.config_options.downstream_prefix_filter:
-            # filter out packages missing parameters with
-            # downstream_prefix prefix
-            downstream_prefix = self.config_options.downstream_prefix or ''
-            self.packages = query.filter_pkgs(
-                self.packages,
-                {downstream_prefix + 'distgit': '.+'})
         return self.packages
 
-    def _getversions(self):
-        """Fetch 'versions.csv'
-
-        from versions_url config option and return the contained data as
-        a dict with package name as a key.
-        """
-        versions_url = self.config_options.versions_url
-        if not versions_url:
-            fail_req_config_missing('versions_url')
-
-        # return versions.csv as a dict with package name as a key
-        vers = {}
-        r = urlopen(versions_url)
-        content = [x.decode('utf-8') for x in r.readlines()]
-        # first line is headers
-        for row in csv.reader(content[1:]):
-            vers[row[0]] = row[1:]
-        return vers
-
     def getinfo(self, **kwargs):
         project = kwargs.get('project')
         package = kwargs.get('package')
+        since = kwargs.get('since')
         local = kwargs.get('local')
         dev_mode = kwargs.get('dev_mode')
-
-        ds_prefix = self.config_options.downstream_prefix or ''
         datadir = self.config_options.datadir
         repo = package['upstream']
-        distgit_attr = ds_prefix + 'distgit'
-        distro = package.get(distgit_attr)
-        if not distro:
-            fail_req_attr_missing(distgit_attr, package)
+        distro = package['master-distgit']
+        tags_only = buildtagsonly(package)
+
         distro_dir = self._distgit_clone_dir(package['name'])
         distro_dir_full = self.distgit_dir(package['name'])
-        distro_branch = self.config_options.downstream_distro_branch
-        if not distro_branch:
-            fail_req_config_missing('downstream_distro_branch')
+        distro_branch = getdistrobranch(package)
         source_branch = getsourcebranch(package)
-        versions = self._getversions()
-
-        # only process packages present in versions.csv
-        if package['name'] not in versions:
-            logger.warning('Package %s not present in %s - skipping.' % (
-                package['name'], self.config_options.versions_url))
-            return []
-        version = versions[package['name']]
-
-        dt_distro = 0  # In this driver we do not care about dt_distro
 
         if dev_mode is False:
             try:
-                distro_branch, extended_hash, dt_extended = refreshrepo(
+                distro_branch, distro_hash, dt_distro = refreshrepo(
                     distro, distro_dir, distro_branch, local=local,
                     full_path=distro_dir_full)
-                # extract distro_hash from versions.csv
-                distro_hash = version[3]
             except Exception:
                 # The error was already logged by refreshrepo, and we want
                 # to avoid halting the whole run because this distgit repo
                 # failed, so return an empty list
                 return []
         else:
             distro_hash = "dev"
-            extended_hash = "dev"
-            dt_extended = 0
+            dt_distro = 0  # Doesn't get used in dev mode
             if not os.path.isdir(distro_dir):
                 # We should fail in this case, since we are running
                 # in dev mode, so no try/except
                 refreshrepo(distro, distro_dir, distro_branch, local=local,
                             full_path=distro_dir_full)
 
         # repo is usually a string, but if it contains more then one entry we
@@ -167,33 +131,51 @@
             repos = repo
         project_toprocess = []
         for repo in repos:
             repo_dir = os.path.join(datadir, project)
             if len(repos) > 1:
                 repo_dir = os.path.join(repo_dir, os.path.split(repo)[1])
             try:
-                source_branch, _, _ = refreshrepo(repo, repo_dir,
-                                                  source_branch,
+                source_branch, _, _ = refreshrepo(repo, repo_dir, source_branch,
                                                   local=local)
             except Exception:
                 # The error was already logged by refreshrepo, and the only
                 # side-effect is that we are not adding this commit to the
                 # list of commits to be processed, so we can ignore it and
                 # move on to the next repo
                 continue
-            dt = version[5]
-            commit_hash = version[1]
-            commit = Commit(dt_commit=float(dt), project_name=project,
-                            commit_hash=commit_hash, repo_dir=repo_dir,
-                            distro_hash=distro_hash, dt_distro=dt_distro,
-                            extended_hash=extended_hash,
-                            dt_extended=dt_extended,
-                            distgit_dir=self.distgit_dir(package['name']),
-                            commit_branch=source_branch)
-            project_toprocess.append(commit)
+
+            git = sh.git.bake(_cwd=repo_dir, _tty_out=False)
+            # Git gives us commits already sorted in the right order
+            if tags_only is True:
+                logger.info('Building tags only for %s' % project)
+                if since == '-1':
+                    # we need 2 entries as HEAD will be listed too
+                    since = '-2'
+                lines = filter(
+                    lambda x: x.find('tag: ') >= 0,
+                    git.log('--simplify-by-decoration',
+                            "--pretty=format:'%ct %H %d'",
+                            since, "--first-parent",
+                            "--reverse", "%s" % source_branch))
+            else:
+                lines = git.log("--pretty=format:'%ct %H'",
+                                since, "--first-parent",
+                                "--reverse")
+
+            for line in lines:
+                dt, commit_hash = str(line).strip().strip("'").split(" ")[:2]
+                commit = Commit(dt_commit=float(dt), project_name=project,
+                                commit_hash=commit_hash, repo_dir=repo_dir,
+                                distro_hash=distro_hash, dt_distro=dt_distro,
+                                distgit_dir=self.distgit_dir(package['name']),
+                                commit_branch=source_branch,
+                                dt_extended=0, extended_hash=None)
+                project_toprocess.append(commit)
+
         return project_toprocess
 
     def preprocess(self, **kwargs):
         # Pre-processing is only required if we have a jinja2 spec template
         package_name = kwargs.get('package_name')
         distgit_dir = self.distgit_dir(package_name)
         # Now, try to check if we need to run a pre-processing job
```

### Comparing `DLRN-0.9.0/dlrn/drivers/gitrepo.py` & `DLRN-0.9.1/dlrn/drivers/gitrepo.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,14 +54,24 @@
         return True
     except (urllib.error.HTTPError, urllib.error.URLError):
         # Trouble finding URL
         return False
 
 
 class GitRepoDriver(PkgInfoDriver):
+    DRIVER_CONFIG = {
+        'gitrepo_driver': {
+            'gitrepo_repo': {'name': 'repo'},
+            'gitrepo_dir': {'name': 'directory'},
+            'skip_dirs': {'name': 'skip', 'type': 'list'},
+            'use_version_from_spec': {'type': 'boolean'},
+            'keep_tarball': {'type': 'boolean'},
+        }
+    }
+
     def __init__(self, *args, **kwargs):
         super(GitRepoDriver, self).__init__(*args, **kwargs)
 
     def _get_version_from_pkg(self, packagepath, package):
         self.preprocess(package_name=package)
         pkgdir = os.path.join(packagepath, package)
         for pkgfile in os.listdir(pkgdir):
```

### Comparing `DLRN-0.9.0/dlrn/drivers/kojidriver.py` & `DLRN-0.9.1/dlrn/drivers/kojidriver.py`

 * *Files 20% similar despite different names*

```diff
@@ -33,19 +33,33 @@
 logger = logging.getLogger("dlrn-build-koji")
 logger.setLevel(logging.INFO)
 
 # FIXME(jpena): needs to be configurable, and driver-independent
 mock_base_packages = "basesystem rpm-build python2-devel gcc make "\
                      "python-sqlalchemy python-webob ghostscript graphviz "\
                      "python-sphinx python-eventlet python-six python-pbr "\
-                     "openstack-macros git yum-plugin-priorities rubygems"\
+                     "openstack-macros git yum-plugin-priorities rubygems "\
                      "python-setuptools_scm"
 
 
 class KojiBuildDriver(BuildRPMDriver):
+    DRIVER_CONFIG = {
+        'kojibuild_driver': {
+            'koji_krb_principal': {'name': 'krb_principal'},
+            'koji_krb_keytab': {'name': 'krb_keytab'},
+            'koji_scratch_build': {'name': 'scratch_build', 'type': 'boolean',
+                                   'default': True},
+            'koji_build_target': {'name': 'build_target'},
+            'koji_arch': {'name': 'arch', 'default': 'x86_64'},
+            'koji_use_rhpkg': {'name': 'use_rhpkg', 'type': 'boolean'},
+            'koji_exe': {'default': 'koji'},
+            'fetch_mock_config': {'type': 'boolean'},
+        }
+    }
+
     def __init__(self, *args, **kwargs):
         super(KojiBuildDriver, self).__init__(*args, **kwargs)
         self.exe_name = self.config_options.koji_exe
 
     # We are using this method to "tee" koji output to a log file and stdout
     def _process_koji_output(self, line):
         if dlrn.shell.verbose_build:
@@ -72,15 +86,16 @@
                     lines.append("config_opts['chroot_setup_cmd'] = "
                                  "'install %s'\n" % mock_base_packages)
                 else:
                     lines.append(line)
         with open(filename, 'w') as fp:
             fp.write(''.join(lines))
 
-    def _build_with_rhpkg(self, package_name, output_dir, src_rpm, scratch):
+    def _build_with_rhpkg(self, package_name, output_dir, src_rpm, scratch,
+                          commit):
         """Use rhpkg as build backend
 
         :param package_name: package name to build
         :param output_dir: output directory
         :param src_rpm: source RPM to build
         :param scratch: define if build is scratch or not
         """
@@ -99,30 +114,65 @@
 
         rhpkg = sh.rhpkg.bake(_cwd=distgit_dir, _tty_out=False,
                               _timeout=3600,
                               _err=self._process_koji_output,
                               _out=self._process_koji_output,
                               _env={'PATH': '/usr/bin/'})
 
+        if (self.config_options.pkginfo_driver ==
+            'dlrn.drivers.downstream.DownstreamInfoDriver' and
+                self.config_options.use_upstream_spec):
+            # This is a special situation. We are copying the upstream
+            # spec over, but then building the srpm and importing. In this
+            # situation, rhpkg import will complain because there are
+            # uncommited changes to the repo... and we will commit them
+            # the srpm. So let's reset the git repo right before that.
+            git = sh.git.bake(_cwd=distgit_dir, _tty_out=False,
+                              _timeout=3600,
+                              _err=self._process_koji_output,
+                              _out=self._process_koji_output,
+                              _env={'PATH': '/usr/bin/'})
+            git.checkout('--', '*')
+
         with io.open("%s/rhpkgimport.log" % output_dir, 'a',
                      encoding='utf-8', errors='replace') as self.koji_fp:
             rhpkg('import', '--skip-diff', src_rpm)
             pkg_date = strftime("%Y-%m-%d-%H%M%S", localtime(time()))
             rhpkg('commit', '-p', '-m', 'DLRN build at %s' % pkg_date)
 
+        # After running rhpkg commit, we have a different commit hash, so
+        # let's update it
+        git = sh.git.bake(_cwd=distgit_dir, _tty_out=False, _timeout=3600)
+        repoinfo = str(git.log("--pretty=format:%H %ct", "-1", ".")).\
+            strip().split(" ")
+
+        logger.info("Updated git: %s" % repoinfo)
+        commit.extended_hash = repoinfo[0]
+        commit.dt_extended = repoinfo[1]
+
+        # Since we are changing the extended_hash, we need to rename the
+        # output directory to match the updated value
+        datadir = os.path.realpath(self.config_options.datadir)
+        new_output_dir = os.path.join(datadir, "repos",
+                                      commit.getshardedcommitdir())
+        logger.info("Renaming %s to %s" % (output_dir, new_output_dir))
+        os.rename(output_dir, new_output_dir)
+        output_dir = new_output_dir
+
         with io.open("%s/rhpkgbuild.log" % output_dir, 'a',
                      encoding='utf-8', errors='replace') as self.koji_fp:
             try:
                 rhpkg('build', scratch=scratch)
             except Exception as e:
                 build_exception = e
 
         return build_exception, "%s/rhpkgbuild.log" % output_dir
 
-    def _build_with_exe(self, package_name, output_dir, src_rpm, scratch):
+    def _build_with_exe(self, package_name, output_dir, src_rpm, scratch,
+                        commit):
         """Build using koji/brew executables (cbs being an aliases)
 
         :param package_name: package name to build
         :param output_dir: output directory
         :param src_rpm: source RPM to build
         :param scratch: define if build is scratch or not
         """
@@ -158,28 +208,35 @@
 
         :param output_directory: directory where the SRPM is located,
                                  and the built packages will be.
         :param package_name: name of a package to build
         """
         output_dir = kwargs.get('output_directory')
         package_name = kwargs.get('package_name')
+        commit = kwargs.get('commit')
         scratch = self.config_options.koji_scratch_build
         build_exception = None
 
         # Find src.rpm
         for rpm in os.listdir(output_dir):
             if rpm.endswith(".src.rpm"):
                 src_rpm = os.path.realpath('%s/%s' % (output_dir, rpm))
         try:
             if self.config_options.koji_use_rhpkg:
                 build_method = self._build_with_rhpkg
             else:
                 build_method = self._build_with_exe
             build_exception, logfile = build_method(
-                package_name, output_dir, src_rpm, scratch)
+                package_name, output_dir, src_rpm, scratch, commit)
+
+            if self.config_options.koji_use_rhpkg:
+                # In this case, we need to re-calculate the output directory
+                datadir = os.path.realpath(self.config_options.datadir)
+                output_dir = os.path.join(datadir, "repos",
+                                          commit.getshardedcommitdir())
 
             # Find task id to download logs
             with open(logfile, 'r') as fp:
                 log_content = fp.readlines()
             task_id = None
             for line in log_content:
                 m = re.search("^Created task: (\d+)$", line)
```

### Comparing `DLRN-0.9.0/dlrn/drivers/mockdriver.py` & `DLRN-0.9.1/dlrn/drivers/mockdriver.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,20 @@
 logging.basicConfig(level=logging.ERROR,
                     format='%(asctime)s %(levelname)s:%(name)s:%(message)s')
 logger = logging.getLogger("dlrn-build-mock")
 logger.setLevel(logging.INFO)
 
 
 class MockBuildDriver(BuildRPMDriver):
+    DRIVER_CONFIG = {
+        'mockbuild_driver': {
+            'install_after_build': {'type': 'boolean', 'default': True},
+        },
+    }
+
     # We are using this method to "tee" mock output to mock.log and stdout
     def _process_mock_output(self, line):
         if dlrn.shell.verbose_build:
             logger.info(line[:-1])
         self.mock_fp.write(line)
 
     def __init__(self, *args, **kwargs):
```

### Comparing `DLRN-0.9.0/dlrn/drivers/pkginfo.py` & `DLRN-0.9.1/dlrn/drivers/pkginfo.py`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/dlrn/migrations/versions/1268c799620f_add_commit_branch_to_db.py` & `DLRN-0.9.1/dlrn/migrations/versions/1268c799620f_add_commit_branch_to_db.py`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/dlrn/migrations/versions/2a0313a8a7d6_change_user_usernames_column_length.py` & `DLRN-0.9.1/dlrn/migrations/versions/2a0313a8a7d6_change_user_usernames_column_length.py`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/dlrn/migrations/versions/3c62b0d3ec34_initial_creation.py` & `DLRN-0.9.1/dlrn/migrations/versions/3c62b0d3ec34_initial_creation.py`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/dlrn/migrations/versions/47ebe0522809_scheme_change_due_to_scm_support_moving_.py` & `DLRN-0.9.1/dlrn/migrations/versions/47ebe0522809_scheme_change_due_to_scm_support_moving_.py`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/dlrn/migrations/versions/4a5651777e5e_add_promotions_table.py` & `DLRN-0.9.1/dlrn/migrations/versions/4a5651777e5e_add_promotions_table.py`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/dlrn/migrations/versions/638f980c9169_add_tables_required_by_dlrn_api.py` & `DLRN-0.9.1/dlrn/migrations/versions/638f980c9169_add_tables_required_by_dlrn_api.py`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/dlrn/migrations/versions/ade85b2396bc_add_extended_hash_and_dt_extended_columns_to_.py` & `DLRN-0.9.1/dlrn/migrations/versions/ade85b2396bc_add_extended_hash_and_dt_extended_columns_to_.py`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/dlrn/migrations/versions/cab7697f6564_add_user_column_to_civote_and_promotion.py` & `DLRN-0.9.1/dlrn/migrations/versions/cab7697f6564_add_user_column_to_civote_and_promotion.py`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/dlrn/migrations/versions/f38ba3389b85_set_string_length.py` & `DLRN-0.9.1/dlrn/migrations/versions/f38ba3389b85_set_string_length.py`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/dlrn/migrations/env.py` & `DLRN-0.9.1/dlrn/migrations/env.py`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/dlrn/migrations/script.py.mako` & `DLRN-0.9.1/dlrn/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/dlrn/stylesheets/styles.css` & `DLRN-0.9.1/dlrn/stylesheets/styles.css`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/dlrn/templates/stylesheets/styles.css` & `DLRN-0.9.1/dlrn/templates/stylesheets/styles.css`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/dlrn/templates/queue.j2` & `DLRN-0.9.1/dlrn/templates/queue.j2`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/dlrn/templates/report.j2` & `DLRN-0.9.1/dlrn/templates/report.j2`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/dlrn/templates/status_report.j2` & `DLRN-0.9.1/dlrn/templates/status_report.j2`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/dlrn/tests/samples/commits_1.yaml` & `DLRN-0.9.1/dlrn/tests/samples/commits_1.yaml`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/dlrn/tests/samples/commits_2.yaml` & `DLRN-0.9.1/dlrn/tests/samples/commits_2.yaml`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/dlrn/tests/samples/commits_remote.yaml` & `DLRN-0.9.1/dlrn/tests/samples/commits_remote.yaml`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/dlrn/tests/samples/versions.csv` & `DLRN-0.9.1/dlrn/tests/samples/versions.csv`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/dlrn/tests/base.py` & `DLRN-0.9.1/dlrn/tests/base.py`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/dlrn/tests/test_api.py` & `DLRN-0.9.1/dlrn/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/dlrn/tests/test_build.py` & `DLRN-0.9.1/dlrn/tests/test_build.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 
 import dlrn.shell
 
 from dlrn.build import build
 from dlrn.build import build_rpm_wrapper
 from dlrn.config import ConfigOptions
 from dlrn import db
-from dlrn.shell import default_options
 from dlrn.tests import base
 from dlrn import utils
 
 
 class FakePkgInfo(object):
     def preprocess(self, **argv):
         return
@@ -45,21 +44,21 @@
 
 @mock.patch('sh.restorecon', create=True)
 @mock.patch('sh.env', create=True)
 @mock.patch.object(sh.Command, '__call__', autospec=True)
 class TestBuild(base.TestCase):
     def setUp(self):
         super(TestBuild, self).setUp()
-        config = configparser.RawConfigParser(default_options)
-        config.read("projects.ini")
-        config.set('DEFAULT', 'datadir', tempfile.mkdtemp())
-        config.set('DEFAULT', 'scriptsdir', tempfile.mkdtemp())
-        config.set('DEFAULT', 'baseurl', "file://%s" % config.get('DEFAULT',
-                                                                  'datadir'))
-        self.config = ConfigOptions(config)
+        self.configfile = configparser.RawConfigParser()
+        self.configfile.read("projects.ini")
+        self.configfile.set('DEFAULT', 'datadir', tempfile.mkdtemp())
+        self.configfile.set('DEFAULT', 'scriptsdir', tempfile.mkdtemp())
+        self.configfile.set('DEFAULT', 'baseurl', "file://%s" %
+                            self.configfile.get('DEFAULT', 'datadir'))
+        self.config = ConfigOptions(self.configfile)
         shutil.copyfile(os.path.join("scripts", "centos.cfg"),
                         os.path.join(self.config.scriptsdir, "centos.cfg"))
         with open(os.path.join(self.config.datadir,
                   "delorean-deps.repo"), "w") as fp:
             fp.write("[test]\nname=test\nenabled=0\n")
         self.db_fd, filepath = tempfile.mkstemp()
         self.session = db.getSession("sqlite:///%s" % filepath)
@@ -69,14 +68,17 @@
         super(TestBuild, self).tearDown()
         shutil.rmtree(self.config.datadir)
         shutil.rmtree(self.config.scriptsdir)
         os.close(self.db_fd)
 
     @mock.patch('os.listdir', side_effect=mocked_listdir)
     def test_build_rpm_wrapper(self, ld_mock, sh_mock, env_mock, rc_mock):
+        self.configfile.set('DEFAULT', 'build_driver',
+                            'dlrn.drivers.mockdriver.MockBuildDriver')
+        self.config = ConfigOptions(self.configfile)
         commit = db.getCommits(self.session)[-1]
         build_rpm_wrapper(commit, False, False, False, None, True)
         # 4 sh calls:
         # 1- git reset --hard
         # 2- build_srpm.sh
         # 3- mock (handled by env_mock)
         # 4- restorecon (handled by rc_mock)
@@ -84,38 +86,50 @@
         self.assertEqual(rc_mock.call_count, 1)
         self.assertEqual(sh_mock.call_count, 1)
         self.assertTrue(os.path.exists(os.path.join(self.config.datadir,
                                                     "dlrn-1.cfg")))
 
     @mock.patch('os.listdir', side_effect=mocked_listdir)
     def test_build(self, ld_mock, sh_mock, env_mock, rc_mock):
+        self.configfile.set('DEFAULT', 'build_driver',
+                            'dlrn.drivers.mockdriver.MockBuildDriver')
+        self.config = ConfigOptions(self.configfile)
         commit = db.getCommits(self.session)[-1]
         try:
             build([], commit, None, False, False, False, True)
         except Exception as e:
             self.assertIn("No rpms built for", str(e))
 
     @mock.patch('os.listdir', side_effect=mocked_listdir)
     def test_build_configdir(self, ld_mock, sh_mock, env_mock, rc_mock):
-        self.config.configdir = tempfile.mkdtemp()
+        configdir = tempfile.mkdtemp()
+        self.configfile.set('DEFAULT', 'configdir', configdir)
+        self.configfile.set('DEFAULT', 'build_driver',
+                            'dlrn.drivers.mockdriver.MockBuildDriver')
+        self.config = ConfigOptions(self.configfile)
+
         shutil.copyfile(os.path.join("scripts", "centos.cfg"),
-                        os.path.join(self.config.configdir, "centos.cfg"))
+                        os.path.join(configdir, "centos.cfg"))
         commit = db.getCommits(self.session)[-1]
-        expected = [mock.call('%s/centos.cfg' % self.config.configdir,
+        expected = [mock.call('%s/centos.cfg' % configdir,
                               '%s/dlrn-1.cfg.new' % self.config.datadir),
                     mock.call('%s/dlrn-1.cfg.new' % self.config.datadir,
                               '%s/dlrn-1.cfg' % self.config.datadir)]
 
         with mock.patch('shutil.copyfile',
                         side_effect=shutil.copyfile) as cp_mock:
             build_rpm_wrapper(commit, False, False, False, None, True)
             self.assertEqual(expected, cp_mock.call_args_list)
 
+    @mock.patch('dlrn.drivers.kojidriver.KojiBuildDriver.build_package')
     @mock.patch('os.listdir', side_effect=mocked_listdir)
-    @mock.patch('dlrn.drivers.mockdriver.MockBuildDriver.write_mock_config',
+    @mock.patch('dlrn.drivers.kojidriver.KojiBuildDriver.write_mock_config',
                 create=True)
-    def test_build_rpm_wrapper_mock_config(self, wm_mock, ld_mock, sh_mock,
-                                           env_mock, rc_mock):
-        self.config.fetch_mock_config = True
+    def test_build_rpm_wrapper_mock_config(self, wm_mock, ld_mock, bp_mock,
+                                           sh_mock, env_mock, rc_mock):
+        self.configfile.set('kojibuild_driver', 'fetch_mock_config', 'True')
+        self.configfile.set('DEFAULT', 'build_driver',
+                            'dlrn.drivers.kojidriver.KojiBuildDriver')
+        self.config = ConfigOptions(self.configfile)
         commit = db.getCommits(self.session)[-1]
         build_rpm_wrapper(commit, False, False, False, None, True)
         self.assertEqual(wm_mock.call_count, 1)
```

### Comparing `DLRN-0.9.0/dlrn/tests/test_config.py` & `DLRN-0.9.1/dlrn/tests/test_config.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,39 +13,48 @@
 # under the License.
 
 from dlrn.tests import base
 from six.moves import configparser
 
 from dlrn.config import ConfigOptions
 from dlrn.config import getConfigOptions
-from dlrn.shell import default_options
 
 
 class TestConfigOptions(base.TestCase):
     def setUp(self):
         super(TestConfigOptions, self).setUp()
-        self.config = configparser.RawConfigParser(default_options)
+        self.config = configparser.RawConfigParser()
         self.config.read("projects.ini")
 
     def test_without_gitrepo_driver(self):
         self.config.remove_section("gitrepo_driver")
         ConfigOptions(self.config)
 
     def test_with_gitrepo_driver(self):
+        self.config.set("DEFAULT", "pkginfo_driver",
+                        "dlrn.drivers.gitrepo.GitRepoDriver")
         self.config.set("gitrepo_driver", "skip", "pkg1,pkg2")
         config = ConfigOptions(self.config)
         self.assertEqual(config.skip_dirs, ["pkg1", "pkg2"])
 
     def test_without_rdoinfo_driver(self):
         self.config.remove_section("rdoinfo_driver")
         ConfigOptions(self.config)
 
     def test_with_rdoinfo_driver(self):
+        self.config.set("DEFAULT", "pkginfo_driver",
+                        "dlrn.drivers.rdoinfo.RdoInfoDriver")
         self.config.set(
             "rdoinfo_driver", "repo", "https://test/test.git")
         config = ConfigOptions(self.config)
         self.assertEqual(
             config.rdoinfo_repo, 'https://test/test.git')
 
     def test_get_config_option(self):
         config = ConfigOptions(self.config)
         self.assertEqual(config, getConfigOptions())
+
+    def test_dynamic_dirs(self):
+        config = ConfigOptions(self.config)
+        self.assertEqual(config.scriptsdir, './scripts')
+        self.assertEqual(config.configdir, './scripts')
+        self.assertEqual(config.templatedir, './dlrn/templates')
```

### Comparing `DLRN-0.9.0/dlrn/tests/test_db.py` & `DLRN-0.9.1/dlrn/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/dlrn/tests/test_driver_copr.py` & `DLRN-0.9.1/dlrn/tests/test_driver_copr.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,28 +15,29 @@
 import mock
 import os
 import shutil
 import tempfile
 
 from dlrn.config import ConfigOptions
 from dlrn.drivers.coprdriver import CoprBuildDriver
-from dlrn.shell import default_options
 from dlrn.tests import base
 from six.moves import configparser
 
 
 @mock.patch('sh.restorecon', create=True)
 @mock.patch('sh.env', create=True)
 class TestDriverCopr(base.TestCase):
     def setUp(self):
         super(TestDriverCopr, self).setUp()
-        config = configparser.RawConfigParser(default_options)
+        config = configparser.RawConfigParser()
         config.read("projects.ini")
+        config.set("DEFAULT", "build_driver",
+                   "dlrn.drivers.coprdriver.CoprBuildDriver")
+        config.set('coprbuild_driver', 'coprid', 'foo/repo')
         self.config = ConfigOptions(config)
-        self.config.coprid = 'account/repo'
         self.temp_dir = tempfile.mkdtemp()
         # Create fake src.rpm
         with open('%s/pkg.src.rpm' % self.temp_dir, 'a') as fp:
             fp.write('')
         # Create fake build and download logs
         with open("%s/coprbuild.log" % self.temp_dir, 'a') as fp:
             fp.write("Created builds: 1234")
@@ -84,7 +85,10 @@
         # Make sure output_dir is as expected
         content = os.listdir(self.temp_dir)
         self.assertIn('coprdownload.log', content)
         self.assertIn('state.log.gz', content)
         self.assertIn('pkg.rpm', content)
         self.assertIn('pkg.src.rpm', content)
         self.assertNotIn('1234', content)
+
+    def test_driver_config(self, env_mock, rc_mock):
+        self.assertEqual(self.config.coprid, 'foo/repo')
```

### Comparing `DLRN-0.9.0/dlrn/tests/test_driver_git.py` & `DLRN-0.9.1/dlrn/tests/test_driver_git.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,24 +17,25 @@
 import shutil
 import tempfile
 
 from six.moves import configparser
 
 from dlrn.config import ConfigOptions
 from dlrn.drivers.gitrepo import GitRepoDriver
-from dlrn.shell import default_options
 from dlrn.tests import base
 
 
 @mock.patch.object(sh.Command, '__call__', autospec=True)
 class TestDriverGit(base.TestCase):
     def setUp(self):
         super(TestDriverGit, self).setUp()
-        config = configparser.RawConfigParser(default_options)
+        config = configparser.RawConfigParser()
         config.read("projects.ini")
+        config.set("DEFAULT", "pkginfo_driver",
+                   "dlrn.drivers.gitrepo.GitRepoDriver")
         self.config = ConfigOptions(config)
         self.config.gitrepo_dir = tempfile.mkdtemp()
 
     def tearDown(self):
         super(TestDriverGit, self).tearDown()
         shutil.rmtree(self.config.gitrepo_dir)
```

### Comparing `DLRN-0.9.0/dlrn/tests/test_driver_koji.py` & `DLRN-0.9.1/dlrn/tests/test_driver_koji.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,48 +16,62 @@
 import os
 import sh
 import shutil
 import stat
 import tempfile
 
 from dlrn.config import ConfigOptions
+from dlrn import db
 from dlrn.drivers.kojidriver import KojiBuildDriver
-from dlrn.shell import default_options
 from dlrn.tests import base
 from six.moves import configparser
 from time import localtime
 from time import strftime
 
 
 def _mocked_listdir(directory):
     return ['python-pysaml2-3.0-1a.el7.centos.src.rpm']
 
 
 def _mocked_time():
     return float(1533293385.545039)
 
 
+def _mocked_call(*args, **kwargs):
+    if args[0] == '/usr/bin/git log':
+        return '1 2'
+    return True
+
+
 @mock.patch('sh.restorecon', create=True)
 @mock.patch('sh.env', create=True)
 @mock.patch('os.listdir', side_effect=_mocked_listdir)
 class TestDriverKoji(base.TestCase):
     def setUp(self):
         super(TestDriverKoji, self).setUp()
-        config = configparser.RawConfigParser(default_options)
+        config = configparser.RawConfigParser()
         config.read("projects.ini")
+        config.set("DEFAULT", "build_driver",
+                   "dlrn.drivers.kojidriver.KojiBuildDriver")
         self.config = ConfigOptions(config)
         self.config.koji_krb_principal = 'test@example.com'
         self.config.koji_krb_keytab = '/home/test/test.keytab'
         self.config.koji_scratch_build = True
         self.config.koji_build_target = 'build-target'
         self.temp_dir = tempfile.mkdtemp()
+        self.config.datadir = self.temp_dir
         # Create fake build log
         with open("%s/kojibuild.log" % self.temp_dir, 'a') as fp:
             fp.write("Created task: 1234")
-        with open("%s/rhpkgbuild.log" % self.temp_dir, 'a') as fp:
+        # In the rhpkg case, we need to create a full dir structure
+        self.rhpkg_extra_dir = "%s/repos/12/34/1234567890abcdef_12345678_1"\
+                               % self.temp_dir
+        os.makedirs(self.rhpkg_extra_dir)
+        with open("%s/rhpkgbuild.log"
+                  % self.rhpkg_extra_dir, 'a') as fp:
             fp.write("Created task: 5678")
         # Create a fake rhpkg binary
         with open("%s/rhpkg" % self.temp_dir, 'a') as fp:
             fp.write("true")
         os.chmod("%s/rhpkg" % self.temp_dir,
                  stat.S_IREAD | stat.S_IWRITE | stat.S_IEXEC)
         os.environ['PATH'] = self.temp_dir + ':' + os.environ['PATH']
@@ -176,46 +190,61 @@
         # 1- koji build (handled by env_mock)
         # 2- koji download (handled by env_mock)
         # 3- restorecon (handled by rc_mock)
         self.assertEqual(env_mock.call_count, 2)
         self.assertEqual(rc_mock.call_count, 1)
         self.assertEqual(env_mock.call_args_list, expected)
 
-    @mock.patch.object(sh.Command, '__call__', autospec=True)
+    @mock.patch('os.rename')
+    @mock.patch.object(sh.Command, '__call__', autospec=True,
+                       side_effect=_mocked_call)
     @mock.patch('dlrn.drivers.kojidriver.time', side_effect=_mocked_time)
     @mock.patch('sh.kinit', create=True)
-    def test_build_package_rhpkg(self, ki_mock, tm_mock, rh_mock, ld_mock,
-                                 env_mock, rc_mock):
+    def test_build_package_rhpkg(self, ki_mock, tm_mock, rh_mock, rn_mock,
+                                 ld_mock, env_mock, rc_mock):
         self.config.koji_use_rhpkg = True
+        commit = db.Commit(dt_commit=123, project_name='python-pysaml2',
+                           commit_hash='1234567890abcdef',
+                           distro_hash='1234567890abcdef',
+                           extended_hash='1234567890abcdef',
+                           dt_distro=123,
+                           dt_extended=123)
+
         driver = KojiBuildDriver(cfg_options=self.config)
         driver.build_package(output_directory=self.temp_dir,
-                             package_name='python-pysaml2')
+                             package_name='python-pysaml2',
+                             commit=commit)
 
         expected_env = [mock.call(['koji', 'download-task', '--logs', '5678'],
                                   _err=driver._process_koji_output,
                                   _out=driver._process_koji_output,
-                                  _cwd=self.temp_dir,
+                                  _cwd=self.rhpkg_extra_dir,
                                   _env={'PATH': '/usr/bin/'})]
 
         pkg_date = strftime("%Y-%m-%d-%H%M%S", localtime(_mocked_time()))
         expected_rh = [mock.call('%s/rhpkg' % self.temp_dir, 'import',
                                  '--skip-diff',
                                  '%s/python-pysaml2-3.0-1a.el7.centos.src'
                                  '.rpm' % self.temp_dir),
                        mock.call('%s/rhpkg' % self.temp_dir, 'commit', '-p',
                                  '-m',
                                  'DLRN build at %s' % pkg_date),
+                       mock.call('/usr/bin/git log', '--pretty=format:%H %ct',
+                                 '-1', '.'),
                        mock.call('%s/rhpkg' % self.temp_dir, 'build',
                                  scratch=True)]
 
         # 1- kinit (handled by kb_mock)
         # 2- rhpkg import (handled by rh_mock)
         # 3- rhpkg commit (handled by rh_mock)
-        # 4- rhpkg build (handled by rh_mock)
-        # 5- koji download (handled by env_mock)
-        # 6- restorecon (handled by rc_mock)
+        # 4- git log (handled by rh_mock)
+        # 5- rename (handled by rn_mock)
+        # 5- rhpkg build (handled by rh_mock)
+        # 6- koji download (handled by env_mock)
+        # 7- restorecon (handled by rc_mock)
         self.assertEqual(ki_mock.call_count, 1)
-        self.assertEqual(rh_mock.call_count, 3)
+        self.assertEqual(rh_mock.call_count, 4)
         self.assertEqual(env_mock.call_count, 1)
         self.assertEqual(rc_mock.call_count, 1)
+        self.assertEqual(rn_mock.call_count, 1)
         self.assertEqual(env_mock.call_args_list, expected_env)
         self.assertEqual(rh_mock.call_args_list, expected_rh)
```

### Comparing `DLRN-0.9.0/dlrn/tests/test_driver_mock.py` & `DLRN-0.9.1/dlrn/tests/test_driver_mock.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,31 +15,32 @@
 import mock
 import os
 import shutil
 import tempfile
 
 from dlrn.config import ConfigOptions
 from dlrn.drivers.mockdriver import MockBuildDriver
-from dlrn.shell import default_options
 from dlrn.tests import base
 from six.moves import configparser
 
 
 def _mocked_listdir(directory):
     return ['python-pysaml2-3.0-1a.el7.centos.src.rpm']
 
 
 @mock.patch('sh.restorecon', create=True)
 @mock.patch('sh.env', create=True)
 @mock.patch('os.listdir', side_effect=_mocked_listdir)
 class TestDriverMock(base.TestCase):
     def setUp(self):
         super(TestDriverMock, self).setUp()
-        config = configparser.RawConfigParser(default_options)
+        config = configparser.RawConfigParser()
         config.read("projects.ini")
+        config.set("DEFAULT", "build_driver",
+                   "dlrn.drivers.mockdriver.MockBuildDriver")
         self.config = ConfigOptions(config)
         self.temp_dir = tempfile.mkdtemp()
 
     def tearDown(self):
         super(TestDriverMock, self).tearDown()
         shutil.rmtree(self.temp_dir)
 
@@ -108,7 +109,17 @@
                               postinstall=True)]
         # 2 sh calls:
         # 1- mock (handled by mock_mock)
         # 2- restorecon (handled by rc_mock)
         self.assertEqual(env_mock.call_count, 1)
         self.assertEqual(rc_mock.call_count, 1)
         self.assertEqual(env_mock.call_args_list, expected)
+
+    def test_driver_config(self, ld_mock, env_mock, rc_mock):
+        cp = configparser.RawConfigParser()
+        cp.read("projects.ini")
+        cp.set("DEFAULT", "build_driver",
+               "dlrn.drivers.mockdriver.MockBuildDriver")
+        # default is True, test override
+        cp.set('mockbuild_driver', 'install_after_build', '0')
+        config = ConfigOptions(cp)
+        self.assertEqual(False, config.install_after_build)
```

### Comparing `DLRN-0.9.0/dlrn/tests/test_notifications.py` & `DLRN-0.9.1/dlrn/tests/test_notifications.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,23 +14,22 @@
 import os
 import shutil
 import tempfile
 
 from dlrn.config import ConfigOptions
 from dlrn import db
 from dlrn import notifications
-from dlrn.shell import default_options
 from dlrn.tests import base
 from six.moves import configparser
 
 
 class TestNotifications(base.TestCase):
     def setUp(self):
         super(TestNotifications, self).setUp()
-        config = configparser.RawConfigParser(default_options)
+        config = configparser.RawConfigParser()
         config.read("projects.ini")
         config.set('DEFAULT', 'datadir', tempfile.mkdtemp())
         config.set('DEFAULT', 'scriptsdir', tempfile.mkdtemp())
         config.set('DEFAULT', 'baseurl', "file://%s" % config.get('DEFAULT',
                                                                   'datadir'))
 
         self.config = ConfigOptions(config)
```

### Comparing `DLRN-0.9.0/dlrn/tests/test_purge.py` & `DLRN-0.9.1/dlrn/tests/test_purge.py`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/dlrn/tests/test_remote.py` & `DLRN-0.9.1/dlrn/tests/test_remote.py`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/dlrn/tests/test_repositories.py` & `DLRN-0.9.1/dlrn/tests/test_repositories.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # License for the specific language governing permissions and limitations
 # under the License.
 import mock
 import sh
 
 from dlrn.config import ConfigOptions
 from dlrn import repositories
-from dlrn.shell import default_options
 from dlrn.tests import base
 
 from six.moves import configparser
 
 
 def _aux_sh(*args):
     call = args[0]
@@ -66,15 +65,15 @@
                     mock.call(sh.git.fetch, 'origin'),
                     mock.call(sh.git.checkout, '-f', 'branch'),
                     mock.call(sh.git.reset, '--hard', 'origin/branch'),
                     mock.call(sh.git.log, '--pretty=format:%H %ct', '-1', '.')]
         self.assertEqual(sh_mock.call_args_list, expected)
 
     def test_clone_no_fallback(self, sh_mock):
-        config = configparser.RawConfigParser(default_options)
+        config = configparser.RawConfigParser()
         config.read("projects.ini")
         config.set('DEFAULT', 'fallback_to_master', '0')
         self.config = ConfigOptions(config)
         # We need to redefine the mock object again, to use a side effect
         # that will fail in the git checkout call. A bit convoluted, but
         # it works
         with mock.patch.object(sh.Command, '__call__') as new_mock:
```

### Comparing `DLRN-0.9.0/dlrn/tests/test_rpmspecfile.py` & `DLRN-0.9.1/dlrn/tests/test_rpmspecfile.py`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/dlrn/tests/test_rsync.py` & `DLRN-0.9.1/dlrn/tests/test_rsync.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,24 +14,23 @@
 import os
 import shutil
 import tempfile
 
 from dlrn.config import ConfigOptions
 from dlrn import db
 from dlrn import rsync
-from dlrn.shell import default_options
 from dlrn.tests import base
 from six.moves import configparser
 
 
 @mock.patch('sh.rsync', create=True)
 class TestSyncRepo(base.TestCase):
     def setUp(self):
         super(TestSyncRepo, self).setUp()
-        config = configparser.RawConfigParser(default_options)
+        config = configparser.RawConfigParser()
         config.read("projects.ini")
         config.set('DEFAULT', 'datadir', tempfile.mkdtemp())
         config.set('DEFAULT', 'scriptsdir', tempfile.mkdtemp())
         config.set('DEFAULT', 'baseurl', "file://%s" % config.get('DEFAULT',
                                                                   'datadir'))
         config.set('DEFAULT', 'rsyncport', '30000')
         config.set('DEFAULT', 'rsyncdest', 'user@host:/directory')
```

### Comparing `DLRN-0.9.0/dlrn/tests/test_shell.py` & `DLRN-0.9.1/dlrn/tests/test_shell.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import os
 import shutil
 import tempfile
 
 from dlrn.config import ConfigOptions
 from dlrn import db
 from dlrn import shell
-from dlrn.shell import default_options
 from dlrn.tests import base
 from dlrn import utils
 
 from six.moves import configparser
 
 
 def mocked_session(url):
@@ -30,15 +29,15 @@
     utils.loadYAML(session, './dlrn/tests/samples/commits_1.yaml')
     return session
 
 
 class TestProcessBuildResult(base.TestCase):
     def setUp(self):
         super(TestProcessBuildResult, self).setUp()
-        config = configparser.RawConfigParser(default_options)
+        config = configparser.RawConfigParser()
         config.read("projects.ini")
         config.set('DEFAULT', 'datadir', tempfile.mkdtemp())
         config.set('DEFAULT', 'scriptsdir', tempfile.mkdtemp())
         config.set('DEFAULT', 'baseurl', "file://%s" % config.get('DEFAULT',
                                                                   'datadir'))
         self.config = ConfigOptions(config)
         self.commit = db.Commit(dt_commit=123, project_name='foo',
@@ -113,15 +112,15 @@
         self.assertEqual(sr_mock.call_count, 1)
 
 
 @mock.patch('sh.createrepo_c', create=True)
 class TestPostBuild(base.TestCase):
     def setUp(self):
         super(TestPostBuild, self).setUp()
-        config = configparser.RawConfigParser(default_options)
+        config = configparser.RawConfigParser()
         config.read("projects.ini")
         config.set('DEFAULT', 'datadir', tempfile.mkdtemp())
         config.set('DEFAULT', 'scriptsdir', tempfile.mkdtemp())
         config.set('DEFAULT', 'baseurl', "file://%s" % config.get('DEFAULT',
                                                                   'datadir'))
         self.config = ConfigOptions(config)
         self.commit = db.Commit(dt_commit=123, project_name='foo',
```

### Comparing `DLRN-0.9.0/dlrn/tests/test_user.py` & `DLRN-0.9.1/dlrn/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/dlrn/tests/test_utils.py` & `DLRN-0.9.1/dlrn/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/dlrn/__init__.py` & `DLRN-0.9.1/dlrn/__init__.py`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/dlrn/build.py` & `DLRN-0.9.1/dlrn/build.py`

 * *Files 7% similar despite different names*

```diff
@@ -69,27 +69,30 @@
     config_options = getConfigOptions()
     # Set the build timestamp to now
     commit.dt_build = int(time())
 
     project_name = commit.project_name
     datadir = os.path.realpath(config_options.datadir)
     yumrepodir = _get_yumrepodir(commit)
-    yumrepodir_abs = os.path.join(datadir, yumrepodir)
     version_from = get_version_from(packages, project_name)
 
     try:
         build_rpm_wrapper(commit, dev_mode, use_public, bootstrap,
                           env_vars, sequential,
                           version_from=version_from)
     except Exception as e:
         logger.error('Build failed. See logs at: %s/%s/' % (datadir,
                                                             yumrepodir))
         raise Exception("Error in build_rpm_wrapper for %s: %s" %
                         (project_name, e))
 
+    # This *could* have changed during the build, see kojidriver.py
+    yumrepodir = _get_yumrepodir(commit)
+    yumrepodir_abs = os.path.join(datadir, yumrepodir)
+
     built_rpms = []
     for rpm in os.listdir(yumrepodir_abs):
         if rpm.endswith(".rpm"):
             built_rpms.append(os.path.join(yumrepodir, rpm))
     if not built_rpms:
         raise Exception("No rpms built for %s" % project_name)
 
@@ -128,15 +131,17 @@
     datadir = os.path.realpath(config_options.datadir)
     baseurl = config_options.baseurl
     templatecfg = os.path.join(configdir, config_options.target + ".cfg")
     newcfg = os.path.join(datadir, mock_config + ".new")
     oldcfg = os.path.join(datadir, mock_config)
     shutil.copyfile(templatecfg, newcfg)
 
-    if config_options.fetch_mock_config:
+    if (config_options.build_driver ==
+            'dlrn.drivers.kojidriver.KojiBuildDriver' and
+            config_options.fetch_mock_config):
         buildrpm.write_mock_config(oldcfg)
 
     # Add the most current repo, we may have dependencies in it
     if os.path.exists(os.path.join(datadir, "repos", "current", "repodata")):
         # Get the real path for the current repo, this could change during
         # parallel builds
         repolink = os.readlink(os.path.join(datadir, "repos", "current"))
@@ -208,22 +213,28 @@
 
         with open(newcfg, "w") as fp:
             fp.writelines(contents)
 
     # don't change dlrn.cfg if the content hasn't changed to prevent
     # mock from rebuilding its cache.
     try:
-        if not config_options.fetch_mock_config and \
-           not filecmp.cmp(newcfg, oldcfg):
-            shutil.copyfile(newcfg, oldcfg)
+        if not filecmp.cmp(newcfg, oldcfg):
+            if (config_options.build_driver ==
+                    'dlrn.drivers.kojidriver.KojiBuildDriver'):
+                if not config_options.fetch_mock_config:
+                    shutil.copyfile(newcfg, oldcfg)
+            else:
+                shutil.copyfile(newcfg, oldcfg)
     except OSError:
         shutil.copyfile(newcfg, oldcfg)
 
     # Set env variable for Copr configuration
-    if config_options.coprid:
+    if (config_options.build_driver ==
+            'dlrn.drivers.coprdriver.CoprBuildDriver' and
+            config_options.coprid):
         os.environ['COPR_ID'] = config_options.coprid
 
     # Set release numbering option
     if config_options.release_numbering == '0.1.date.hash':
         os.environ['RELEASE_NUMBERING'] = '0.1.date.hash'
     else:
         os.environ['RELEASE_NUMBERING'] = '0.date.hash'
@@ -235,15 +246,17 @@
     if bootstrap is True:
         additional_mock_options = '-D repo_bootstrap 1'
     else:
         additional_mock_options = None
 
     dlrn.shell.pkginfo.preprocess(package_name=commit.project_name)
 
-    if config_options.keep_tarball:
+    if (config_options.pkginfo_driver ==
+            'dlrn.drivers.gitrepo.GitRepoDriver' and
+            config_options.keep_tarball):
         if commit.commit_branch == config_options.source:
             # We are following the master tarball here, use it
             os.environ['DLRN_KEEP_TARBALL'] = '1'
         else:
             if 'DLRN_KEEP_TARBALL' in os.environ:
                 del os.environ['DLRN_KEEP_TARBALL']
 
@@ -257,15 +270,16 @@
     # SRPM is built, now build the RPM using the driver
     datadir = os.path.realpath(config_options.datadir)
     yumrepodir = _get_yumrepodir(commit)
     yumrepodir_abs = os.path.join(datadir, yumrepodir)
 
     buildrpm.build_package(output_directory=yumrepodir_abs,
                            additional_mock_opts=additional_mock_options,
-                           package_name=commit.project_name)
+                           package_name=commit.project_name,
+                           commit=commit)
 
 
 def run(program, commit, env_vars, dev_mode, use_public, bootstrap,
         do_build=True, version_from=None):
     config_options = getConfigOptions()
     datadir = os.path.realpath(config_options.datadir)
     yumrepodir = _get_yumrepodir(commit)
@@ -300,14 +314,17 @@
                     os.path.realpath(commit.distgit_dir)])
     if not do_build:
         logger.info('Running %s' % ' '.join(run_cmd))
 
     try:
         sh.env(run_cmd, _err=process_mock_output, _out=process_mock_output)
     except Exception as e:
+        # This *could* have changed during the build, see kojidriver.py
+        datadir = os.path.realpath(config_options.datadir)
+        yumrepodir = _get_yumrepodir(commit)
         logger.error('cmd failed. See logs at: %s/%s/' % (datadir,
                                                           yumrepodir))
         raise e
 
 
 def process_mock_output(line):
     if dlrn.shell.verbose_build:
```

### Comparing `DLRN-0.9.0/dlrn/db.py` & `DLRN-0.9.1/dlrn/db.py`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/dlrn/notifications.py` & `DLRN-0.9.1/dlrn/notifications.py`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/dlrn/purge.py` & `DLRN-0.9.1/dlrn/purge.py`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/dlrn/remote.py` & `DLRN-0.9.1/dlrn/remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,30 +21,29 @@
 from six.moves.urllib.request import urlopen
 from tempfile import mkstemp
 
 from dlrn.config import ConfigOptions
 from dlrn.db import closeSession
 from dlrn.db import getLastProcessedCommit
 from dlrn.db import getSession
-from dlrn.shell import default_options
 from dlrn.shell import post_build
 from dlrn.shell import process_build_result
 from dlrn.utils import import_object
 from dlrn.utils import loadYAML_list
 from dlrn.utils import lock_file
 
 
 logging.basicConfig(level=logging.ERROR)
 logger = logging.getLogger("dlrn-remote")
 logger.setLevel(logging.INFO)
 
 
 def import_commit(repo_url, config_file, db_connection=None,
                   local_info_repo=None):
-    cp = configparser.RawConfigParser(default_options)
+    cp = configparser.RawConfigParser()
     cp.read(config_file)
     config_options = ConfigOptions(cp)
     pkginfo_driver = config_options.pkginfo_driver
     pkginfo = import_object(pkginfo_driver, cfg_options=config_options)
     packages = pkginfo.getpackages(local_info_repo=local_info_repo,
                                    tags=config_options.tags,
                                    dev_mode=False)
```

### Comparing `DLRN-0.9.0/dlrn/reporting.py` & `DLRN-0.9.1/dlrn/reporting.py`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/dlrn/repositories.py` & `DLRN-0.9.1/dlrn/repositories.py`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/dlrn/rpmspecfile.py` & `DLRN-0.9.1/dlrn/rpmspecfile.py`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/dlrn/rsync.py` & `DLRN-0.9.1/dlrn/rsync.py`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/dlrn/shell.py` & `DLRN-0.9.1/dlrn/shell.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import logging
 import multiprocessing
 import os
 import sys
 import tempfile
 
 from copy import deepcopy
+from functools import cmp_to_key
 from functools import partial
 
 import sh
 from six.moves import configparser
 
 from dlrn.build import build_worker
 
@@ -55,30 +56,14 @@
 from dlrn import version
 
 logging.basicConfig(level=logging.ERROR,
                     format='%(asctime)s %(levelname)s:%(name)s:%(message)s')
 logger = logging.getLogger("dlrn")
 logger.setLevel(logging.INFO)
 
-default_options = {'maxretries': '3', 'tags': None, 'gerrit': None,
-                   'templatedir': os.path.join(
-                       os.path.dirname(os.path.realpath(__file__)),
-                       "templates"),
-                   'project_name': 'RDO',
-                   'rsyncdest': '', 'rsyncport': '22',
-                   'pkginfo_driver': 'dlrn.drivers.rdoinfo.RdoInfoDriver',
-                   'build_driver': 'dlrn.drivers.mockdriver.MockBuildDriver',
-                   'workers': '1',
-                   'gerrit_topic': 'rdo-FTBFS',
-                   'database_connection': 'sqlite:///commits.sqlite',
-                   'fallback_to_master': '1',
-                   'coprid': None,
-                   'release_numbering': '0.date.hash',
-                   }
-
 
 def deprecation():
     # We will still call main, but will indicate that this way of calling
     # the application will be deprecated.
     print("Using the 'delorean' command has been deprecated. Please use 'dlrn'"
           " instead.")
     main()
@@ -151,15 +136,15 @@
     if options.verbose_mock:
         logger.warning('The --verbose-mock command-line option is deprecated.'
                        ' Please use --verbose-build instead.')
         options.verbose_build = options.verbose_mock
     global verbose_build
     verbose_build = options.verbose_build
 
-    cp = configparser.RawConfigParser(default_options)
+    cp = configparser.RawConfigParser()
     cp.read(options.config_file)
 
     if options.log_commands is True:
         logging.getLogger("sh.command").setLevel(logging.INFO)
     if options.order is True:
         options.sequential = True
 
@@ -346,18 +331,25 @@
             orders.insert(orders.index('python-networking_arista'),
                           'python-networking-arista')
 
         # sort the commits according to the score of their project and
         # then use the timestamp of the commits as a secondary key
         def my_cmp(a, b):
             if a.project_name == b.project_name:
-                return cmp(a.dt_commit, b.dt_commit)
-            return cmp(orders.index(a.project_name),
-                       orders.index(b.project_name))
-        toprocess.sort(cmp=my_cmp)
+                _a = a.dt_commit
+                _b = b.dt_commit
+            else:
+                _a = orders.index(a.project_name)
+                _b = orders.index(b.project_name)
+            # cmp is no longer available in python3 so replace it. See Ordering
+            # Comparisons on:
+            # https://docs.python.org/3.0/whatsnew/3.0.html
+            return (_a > _b) - (_a < _b)
+
+        toprocess.sort(key=cmp_to_key(my_cmp))
     else:
         # sort according to the timestamp of the commits
         toprocess.sort()
 
     exit_code = 0
     if options.sequential is True:
         toprocess_copy = deepcopy(toprocess)
```

### Comparing `DLRN-0.9.0/dlrn/user.py` & `DLRN-0.9.1/dlrn/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 from six.moves import input
 import sys
 
 from dlrn.config import ConfigOptions
 from dlrn.db import closeSession
 from dlrn.db import getSession
 from dlrn.db import User
-from dlrn.shell import default_options
 
 
 def create_user(options, db_connection):
     try:
         session = getSession(db_connection)
         olduser = session.query(User).filter(
             User.username == options.username).first()
@@ -137,13 +136,13 @@
     parser_update.add_argument('--username', type=str, required=True,
                                help='User name')
     parser_update.add_argument('--password', type=str, required=True,
                                help='New password')
 
     options = parser.parse_args(sys.argv[1:])
 
-    cp = configparser.RawConfigParser(default_options)
+    cp = configparser.RawConfigParser()
     cp.read(options.config_file)
     config_options = ConfigOptions(cp)
 
     return command_funcs[options.command](options,
                                           config_options.database_connection)
```

### Comparing `DLRN-0.9.0/dlrn/utils.py` & `DLRN-0.9.1/dlrn/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,25 +33,31 @@
                              'Failed to synchronize cache for repo|'
                              'No route to host|'
                              'Device or resource busy|'
                              'Could not resolve host|'
                              'Temporary failure in name resolution')
 
 
-# Import a Python object
-def import_object(import_str, *args, **kwargs):
+# Import a Python class
+def import_class(import_str):
     mod_str, _sep, class_str = import_str.rpartition('.')
     __import__(mod_str)
     try:
         myclass = getattr(sys.modules[mod_str], class_str)
-        return myclass(*args, **kwargs)
+        return myclass
     except AttributeError:
         raise ImportError('Cannot find class %s' % class_str)
 
 
+# Import a Python object
+def import_object(import_str, *args, **kwargs):
+    myclass = import_class(import_str)
+    return myclass(*args, **kwargs)
+
+
 # Load a yaml file into a db session, used to populate a in memory database
 # during tests
 def loadYAML(session, yamlfile):
     with open(yamlfile) as fp:
         data = yaml.load(fp)
 
     for commit in data['commits']:
```

### Comparing `DLRN-0.9.0/dlrn/version.py` & `DLRN-0.9.1/dlrn/version.py`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/doc/source/_images/DLRN.png` & `DLRN-0.9.1/doc/source/_images/DLRN.png`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/doc/source/_images/DLRN.svg` & `DLRN-0.9.1/doc/source/_images/DLRN.svg`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/doc/source/Makefile` & `DLRN-0.9.1/doc/source/Makefile`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/doc/source/api.rst` & `DLRN-0.9.1/doc/source/api.rst`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/doc/source/conf.py` & `DLRN-0.9.1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/doc/source/installation.rst` & `DLRN-0.9.1/doc/source/installation.rst`

 * *Files 3% similar despite different names*

```diff
@@ -247,14 +247,16 @@
     [downstream_driver]
     repo=http://github.com/org/fooinfo
     info_files=foo.yml
     versions_url=https://trunk.rdoproject.org/centos7-master/current/versions.csv
     downstream_distro_branch=foo-rocky
     downstream_prefix=foo-
     downstream_prefix_filter=True
+    use_upstream_spec=False
+    downstream_spec_replace_list=^foo/bar,string1/string2
 
 * ``repo`` selects a distroinfo repository to get package information from.
 * ``info_files`` selects an info file (or a list of info files) to get package
   information from (within the distroinfo repo selected with ``repo``)
 * ``versions_url`` must point to a ``versions.csv`` file generated by
   DLRN instance. ``distro_hash`` and ``commit_hash`` will be reused from
   supplied ``versions.csv`` and only packages present in the file are
@@ -264,14 +266,27 @@
 * ``downstream_prefix`` when accessing package metadata, use this prefix
   for all attributes. For example ``downstream_prefix=foo-`` will cause the
   downstream driver to look at ``foo-distgit`` attribute instead of just
   ``distgit``.
 * ``downstream_distro_filter`` will filter ``packages`` section of packaging
   metadata (from ``repo``/``info_files``) to only contain packages with
   ``downstream_prefix``-ed attributes.
+* ``use_upstream_spec`` defines if the upstream distgit contents (spec file and
+  additional files) should be copied over the downstream distgit after cloning.
+* ``downstream_spec_replace_list``, when ``use_upstream_spec`` is set to True,
+  will perform some sed-like edits in the spec file after copying it from the
+  upstream to the downstream distgit. This is specially useful when the
+  downstream DLRN instance has special requirements, such as building without
+  documentation. in that case, a regular expresion like the following could be
+  used:
+
+.. code-block:: ini
+    downstream_spec_replace_list=^%global with_doc.+/%global with_doc 0
+
+  Multiple regular expressions can be used, separated by commas.
 
 The optional ``[mockbuild_driver]`` section has the following configuration
 options:
 
 .. code-block:: ini
 
     [mockbuild_driver]
@@ -322,14 +337,17 @@
   * Instead of using ``koji_exe`` to trigger the build, DLRN will generate the
     source RPM, and upload it to the distgit path using ``rhpkg import``.
   * DLRN will run ``rhpkg build`` to actually trigger the build.
 
   Note that ``rhpkg`` requires a valid Kerberos ticket, so the ``krb_principal``
   and ``krb_keytab`` options must be set.
 
+  Also note that setting ``rhpkg`` only makes sense when using ``dlrn.drivers.downstream.DownstreamInfoDriver``
+  as the pkginfo driver.
+
 The optional ``[coprbuild_driver]`` section has the following configuration
 options:
 
 .. code-block:: ini
 
     [coprbuild_driver]
     coprid=account/repo
```

### Comparing `DLRN-0.9.0/doc/source/internals.rst` & `DLRN-0.9.1/doc/source/internals.rst`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/doc/source/repositories.rst` & `DLRN-0.9.1/doc/source/repositories.rst`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/doc/source/troubleshooting.rst` & `DLRN-0.9.1/doc/source/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/doc/source/usage.rst` & `DLRN-0.9.1/doc/source/usage.rst`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/doc/specs/zuul-based-architecture.rst` & `DLRN-0.9.1/doc/specs/zuul-based-architecture.rst`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/doc/api_definition.yaml` & `DLRN-0.9.1/doc/api_definition.yaml`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/playbooks/dlrn-api-functional.yaml` & `DLRN-0.9.1/playbooks/dlrn-api-functional.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ---
 - hosts: all
   vars:
     working_dir: '{{ ansible_user_dir }}/{{ zuul.project.src_dir }}/..'
     dlrnapi_auth: "--username foo --password bar"
     dlrnapi_url: "--url http://localhost:5000"
-    imported_repo: "https://trunk.rdoproject.org/centos7-master-head/f0/4a/f04aa34cb4b8781aadcb7724839d2b763f280866_79378a47"
-    imported_commit_hash: "f04aa34cb4b8781aadcb7724839d2b763f280866"
-    imported_distro_hash: "79378a476db38d8ac55b4bdbe7b665845983a56a"
+    imported_repo: "https://trunk.rdoproject.org/centos7-master/fa/e4/fae4326cccc28274d533dd3bea7247f96713fac8_da2d5667"
+    imported_commit_hash: "fae4326cccc28274d533dd3bea7247f96713fac8"
+    imported_distro_hash: "da2d566769a158653fec2aa01a4e83eca8574b86"
   tasks:
 # FIXME(jpena): this should be done using the pip module, however there is
 # an issue with Ansible 2.3.1 that prevents this
 # See https://github.com/ansible/ansible-modules-core/issues/5458
     - name: Prepare virtualenv
       command: virtualenv -p python2 "{{ working_dir }}/.venv"
```

### Comparing `DLRN-0.9.0/playbooks/prepare.yaml` & `DLRN-0.9.1/playbooks/prepare.yaml`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/playbooks/tripleo-ci-oooq.yaml` & `DLRN-0.9.1/playbooks/tripleo-ci-oooq.yaml`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/playbooks/tripleo-ci.yaml` & `DLRN-0.9.1/playbooks/tripleo-ci.yaml`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/scripts/bisect.sh` & `DLRN-0.9.1/scripts/bisect.sh`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/scripts/build_srpm.sh` & `DLRN-0.9.1/scripts/build_srpm.sh`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     /usr/bin/mock $MOCKOPTS --chroot "cd /var/tmp/pkgsrc && gem build $GEMSPEC"
     /usr/bin/mock $MOCKOPTS --copyout /var/tmp/pkgsrc/$PROJECT-$VERSION.gem ./$PROJECT-$VERSION.gem
     setversionandrelease "$VERSION" $(git log --abbrev=7 -n1 --format=format:%h)
 else
     SOURCETYPE='tarball'
     # For Puppet modules, check the version in metadata.json (preferred) or Modulefile
     if [ -r metadata.json ]; then
-        version=$(python -c "import json; print json.loads(open('metadata.json').read(-1))['version']")
+        version=$(python -c "import json; print(json.loads(open('metadata.json').read(-1))['version'])")
     elif [ -r Modulefile ]; then
         version=$(grep version Modulefile | sed "s@version *'\(.*\)'@\1@")
     else
         version=""
     fi
 
     # Not able to discover version, use git tags
@@ -103,15 +103,15 @@
     setversionandrelease "$version" $(git log --abbrev=7 -n1 --format=format:%h)
     if [ -r metadata.json ]; then
         # Detect if this is am OpenStack puppet module
         TARBALLS_OPS=$(egrep -c -e "^Source0.*tarballs.openstack.org" -e "^Source0.*github.com\/openstack" -e "^Source0.*git.openstack.org\/openstack" ${DISTGIT_DIR}/*spec||true)
         echo $TARBALLS_OPS
         # We know OpenStack puppet modules have a common style for metadata.json
         if [ $TARBALLS_OPS -ne 0 ]; then
-            TARNAME=$(python -c "import json; print json.loads(open('metadata.json').read(-1))['name']")
+            TARNAME=$(python -c "import json; print(json.loads(open('metadata.json').read(-1))['name'])")
         else
             TARNAME=$(git remote -v|head -1|awk '{print $2;}'|sed 's@.*/@@;s@\.git$@@')
         fi
     elif [ -r Modulefile ]; then
         TARNAME=$(git remote -v|head -1|awk '{print $2;}'|sed 's@.*/@@;s@\.git$@@')
     elif [ -r Kconfig -a -r Kbuild ]; then
         TARNAME=linux
```

### Comparing `DLRN-0.9.0/scripts/centos.cfg` & `DLRN-0.9.1/scripts/centos.cfg`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/scripts/common-functions` & `DLRN-0.9.1/scripts/common-functions`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/scripts/db_migrate.py` & `DLRN-0.9.1/scripts/db_migrate.py`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/scripts/fedora.cfg` & `DLRN-0.9.1/scripts/fedora.cfg`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/scripts/get_rdo_review.py` & `DLRN-0.9.1/scripts/get_rdo_review.py`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/scripts/map-distgit-name` & `DLRN-0.9.1/scripts/map-distgit-name`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 #!/usr/bin/env python
 # Maps repository names to rdoinfo distgit names
 # package names are all either exact matches or prefixed with either
 # "python-" or "openstack-", so we just check that the ends match
 
+import sh
 import sys
 
-from rdopkg.actionmods import rdoinfo
+from distroinfo import info
 
 if len(sys.argv) == 3:
     rdoinfo_location = sys.argv[2]
 else:
     rdoinfo_location = "https://github.com/redhat-openstack/rdoinfo.git"
 
 if rdoinfo_location.startswith('http'):
-    inforepo = rdoinfo.RdoinfoRepo(".", rdoinfo_location)
-    inforepo.init()
+    sh.git('clone', rdoinfo_location, 'rdoinfo')
+    inforepo = info.DistroInfo(info_files='rdo.yml',
+                               local_info='rdoinfo')
 else:
-    inforepo = rdoinfo.RdoinfoRepo(local_repo_path=rdoinfo_location)
+    inforepo = info.DistroInfo(info_files='rdo.yml',
+                               local_info=rdoinfo_location)
 
 # Attempt a strict mapping with project name
 for package in inforepo.get_info()["packages"]:
     if "project" in package and sys.argv[1] == package["project"]:
         if package["project"].startswith("puppet"):
             print("puppet/%s-distgit" % package["project"])
         else:
```

### Comparing `DLRN-0.9.0/scripts/map-project-name` & `DLRN-0.9.1/scripts/map-project-name`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 #!/usr/bin/env python
 # Maps repository names to rdoinfo package names
 # package names are all either exact matches or prefixed with either
 # "python-" or "openstack-", so we just check that the ends match
 
+import sh
 import sys
 
-from rdopkg.actionmods import rdoinfo
+from distroinfo import info
 
 if len(sys.argv) == 3:
     rdoinfo_location = sys.argv[2]
 else:
     rdoinfo_location = "https://github.com/redhat-openstack/rdoinfo.git"
 
 if rdoinfo_location.startswith('http'):
-    inforepo = rdoinfo.RdoinfoRepo(".", rdoinfo_location)
-    inforepo.init()
+    sh.git('clone', rdoinfo_location, 'rdoinfo')
+    inforepo = info.DistroInfo(info_files='rdo.yml',
+                               local_info='rdoinfo')
 else:
-    inforepo = rdoinfo.RdoinfoRepo(local_repo_path=rdoinfo_location)
+    inforepo = info.DistroInfo(info_files='rdo.yml',
+                               local_info=rdoinfo_location)
 
 # Attempt a strict mapping with project name
 for package in inforepo.get_info()["packages"]:
     if "project" in package and sys.argv[1] == package["project"]:
         print(package["name"])
         exit(0)
```

### Comparing `DLRN-0.9.0/scripts/recreate-promotion-symlinks.py` & `DLRN-0.9.1/scripts/recreate-promotion-symlinks.py`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/scripts/run_project_tests.sh` & `DLRN-0.9.1/scripts/run_project_tests.sh`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/scripts/run_sh_tests.sh` & `DLRN-0.9.1/scripts/run_sh_tests.sh`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/scripts/run_tests.sh` & `DLRN-0.9.1/scripts/run_tests.sh`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/bin/bash
 set -ex
 
 # TODO(hguemar): have proper arguments parsing
 # Usage with all supported arguments
-# ./run_tests.sh <path_to_rdoinfo> <distro (either centos or fedora)> <baseurl to trunk repo>
+# ./run_tests.sh <path_to_rdoinfo> <distro (either centos or fedora)> <baseurl to trunk repo> <tag (optional)>
 
 # Simple script to test that DLRN works either locally or in a zuul environment
 GIT_BASE_URL="https://review.rdoproject.org/r/p"
 OPENSTACK_GIT_URL="git://git.openstack.org"
 ZUUL3_HOME="${ZUUL3_HOME:-/home/zuul}"
 ZUUL_CLONES_DIR="${ZUUL3_HOME}/src/review.rdoproject.org"
 RDOINFO="${1:-$GIT_BASE_URL/rdoinfo}"
@@ -85,18 +85,19 @@
     branch=$(sed "s/-rdo//" <<< "${ZUUL_BRANCH}")
     baseurl="http://trunk.rdoproject.org/${branch}/centos7/"
     src="stable/${branch}"
     PROJECT_DISTRO_BRANCH=$ZUUL_BRANCH
 fi
 
 # Update the configuration
+tag=${4:-$branch}
 sed -i "s%target=.*%target=${target}%" projects.ini
 sed -i "s%source=.*%source=${src}%" projects.ini
 sed -i "s%baseurl=.*%baseurl=${baseurl}%" projects.ini
-sed -i "s%tags=.*%tags=${branch}%" projects.ini
+sed -i "s%tags=.*%tags=${tag}%" projects.ini
 
 # Prepare directories for distro repo
 mkdir -p data/repos
 
 # If the commands below throws an error we still want the logs
 function copy_logs() {
     mkdir -p logs
@@ -165,16 +166,16 @@
             if [ "$branch" != "" ]; then
                 REVIEW_BRANCH="stable%2F$branch"
             else
                 REVIEW_BRANCH="master"
             fi
 
             JSON=$(curl -s -L https://review.openstack.org/changes/openstack%2F${UPSTREAM_PROJECT_NAME}~$REVIEW_BRANCH~$UPSTREAM_ID/revisions/current/review|sed 1d)
-            COMMIT=$(python -c 'import json;import sys; s = json.loads(sys.stdin.read(-1)); print s["revisions"].keys()[0]' <<< $JSON)
-            REF=$(python -c "import json;import sys; s = json.loads(sys.stdin.read(-1)); print s['revisions']['$COMMIT']['ref']" <<< $JSON)
+            COMMIT=$(python -c 'import json;import sys; s = json.loads(sys.stdin.read(-1)); print(s["revisions"].keys()[0])' <<< $JSON)
+            REF=$(python -c "import json;import sys; s = json.loads(sys.stdin.read(-1)); print(s['revisions']['$COMMIT']['ref'])" <<< $JSON)
             pushd data/${PROJECT_TO_BUILD_MAPPED}
             if [ -n "$REF" -a "$REF" != null ]; then
                 git fetch ${UPSTREAM_URL} $REF
                 git checkout FETCH_HEAD
             fi
             git log -1
             popd
```

### Comparing `DLRN-0.9.0/scripts/submit_review.sh` & `DLRN-0.9.1/scripts/submit_review.sh`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/.zuul.yaml` & `DLRN-0.9.1/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/AUTHORS` & `DLRN-0.9.1/AUTHORS`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 Alan Pevec <alan.pevec@redhat.com>
+Alex Schultz <aschultz@next-development.com>
 Alfredo Moralejo <amoralej@redhat.com>
 Arie Bregman <abregman@redhat.com>
 Attila Darazs <adarazs@redhat.com>
 Chandan Kumar <chkumar246@gmail.com>
 Chandan Kumar <chkumar@redhat.com>
 Dan Prince <dprince@redhat.com>
 David Moreau Simard <dms@redhat.com>
@@ -30,14 +31,15 @@
 Lennart Regebro <lregebro@redhat.com>
 Lennart Regebro <regebro@gmail.com>
 Luigi Toscano <ltoscano@redhat.com>
 Martin Mágr <mmagr@redhat.com>
 Mohammed Naser <mnaser@vexxhost.com>
 Monty Taylor <mordred@inaugust.com>
 Paul Belanger <pabelanger@redhat.com>
+Quique Llorente <ellorent@redhat.com>
 Robbie Harwood (frozencemetery) <rharwood@redhat.com>
 Steve Baker <sbaker@redhat.com>
 Tristan Cacqueray <tdecacqu@redhat.com>
 Your Name <you@example.com>
 Zuul CI <zuul@softwarefactory-project.io>
 chandan kumar <chkumar246@gmail.com>
 yatin <ykarel@redhat.com>
```

### Comparing `DLRN-0.9.0/CONTRIBUTING.rst` & `DLRN-0.9.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/ChangeLog` & `DLRN-0.9.1/ChangeLog`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,24 @@
 CHANGES
 =======
 
+0.9.1
+-----
+
+* Adapt python print to python3
+* Update commit used by functional CI job
+* Fix mock\_base\_packages list for the koji driver
+* Allow specifying a tag in run\_tests.sh
+* Fix commit id in database when using rhpkg
+* Additional requirements for the downstream repo
+* Allow driver-side configuration options
+* Introduce universal config interface
+* Fix legacy map-\*-name scripts for new rdopkg
+* Fix --order when running under python3
+
 0.9.0
 -----
 
 * Revert "Pin rdopkg<0.47.0 due to backward incompatibility"
 * Pin rdopkg<0.47.0 due to backward incompatibility
 * Add option to use rhpkg in KojiBuildDriver
 * Update commit to be imported in functional tests
```

### Comparing `DLRN-0.9.0/LICENSE` & `DLRN-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/README.rst` & `DLRN-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/alembic.ini` & `DLRN-0.9.1/alembic.ini`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/projects.ini` & `DLRN-0.9.1/projects.ini`

 * *Files 10% similar despite different names*

```diff
@@ -45,14 +45,16 @@
 #
 #repo=http://github.com/org/fooinfo
 #info_files=foo.yml
 #versions_url=https://trunk.rdoproject.org/centos7-master/current/versions.csv
 #downstream_distro_branch=foo-rocky
 #downstream_prefix=foo-
 #downstream_prefix_filter=True
+#use_upstream_spec=False
+#downstream_spec_replace_list=^foo/bar,string1/string2
 
 [mockbuild_driver]
 # options to be specified if build_driver is set to
 # dlrn.drivers.mockdriver.MockBuildDriver
 #install_after_build=1
 
 [kojibuild_driver]
```

### Comparing `DLRN-0.9.0/setup.cfg` & `DLRN-0.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/setup.py` & `DLRN-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/tox.ini` & `DLRN-0.9.1/tox.ini`

 * *Files identical despite different names*

### Comparing `DLRN-0.9.0/PKG-INFO` & `DLRN-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: DLRN
-Version: 0.9.0
+Version: 0.9.1
 Summary: Build packages
 Home-page: http://www.openstack.org/
 Author: OpenStack
 Author-email: openstack-dev@lists.openstack.org
 License: UNKNOWN
 Description: ====
         DLRN
```

