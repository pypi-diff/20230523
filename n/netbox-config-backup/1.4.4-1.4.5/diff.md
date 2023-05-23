# Comparing `tmp/netbox_config_backup-1.4.4.tar.gz` & `tmp/netbox_config_backup-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_config_backup-1.4.4.tar", last modified: Fri May 19 19:39:07 2023, max compression
+gzip compressed data, was "netbox_config_backup-1.4.5.tar", last modified: Tue May 23 16:30:07 2023, max compression
```

## Comparing `netbox_config_backup-1.4.4.tar` & `netbox_config_backup-1.4.5.tar`

### file list

```diff
@@ -1,75 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:39:07.885653 netbox_config_backup-1.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-19 19:39:07.885653 netbox_config_backup-1.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:39:07.873653 netbox_config_backup-1.4.4/netbox_config_backup/
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:39:07.873653 netbox_config_backup-1.4.4/netbox_config_backup/api/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/api/nested_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/choices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/filtersets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:39:07.873653 netbox_config_backup-1.4.4/netbox_config_backup/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:39:07.873653 netbox_config_backup-1.4.4/netbox_config_backup/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/management/commands/enqueue_if_needed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/management/commands/fix_missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/management/commands/rebuild.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/management/commands/runbackup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:39:07.877653 netbox_config_backup-1.4.4/netbox_config_backup/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/migrations/0002_git_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/migrations/0003_primary_model_to_bigid.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/migrations/0004_custom_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/migrations/0005_commit_add_time_field.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/migrations/0006_backup_add_commit_last_time.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/migrations/0007_backup_job_add_scheduled.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/migrations/0008_backupjob_scheduled_nullable.py
--rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/migrations/0009_bctc_file_model_backup_fk_restructure.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/migrations/0010_backup_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/migrations/0011_alter_backup_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/migrations/0012_backup_status.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:39:07.877653 netbox_config_backup-1.4.4/netbox_config_backup/models/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/models/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     8279 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/models/backups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/models/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/template_content.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:39:07.869653 netbox_config_backup-1.4.4/netbox_config_backup/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:39:07.877653 netbox_config_backup-1.4.4/netbox_config_backup/templates/netbox_config_backup/
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/templates/netbox_config_backup/backup.html
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/templates/netbox_config_backup/backups.html
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/templates/netbox_config_backup/config.html
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/templates/netbox_config_backup/diff.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:39:07.885653 netbox_config_backup-1.4.4/netbox_config_backup/templates/netbox_config_backup/inc/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/templates/netbox_config_backup/inc/backup_tables.html
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/templates/netbox_config_backup/repository.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:39:07.885653 netbox_config_backup-1.4.4/netbox_config_backup/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/templatetags/ncb_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:39:07.885653 netbox_config_backup-1.4.4/netbox_config_backup/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/utils/backups.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/utils/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/utils/rq.py
--rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/netbox_config_backup/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:39:07.873653 netbox_config_backup-1.4.4/netbox_config_backup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-19 19:39:07.000000 netbox_config_backup-1.4.4/netbox_config_backup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-05-19 19:39:07.000000 netbox_config_backup-1.4.4/netbox_config_backup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 19:39:07.000000 netbox_config_backup-1.4.4/netbox_config_backup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 19:39:07.000000 netbox_config_backup-1.4.4/netbox_config_backup.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-19 19:39:07.000000 netbox_config_backup-1.4.4/netbox_config_backup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-19 19:39:07.000000 netbox_config_backup-1.4.4/netbox_config_backup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 19:39:07.885653 netbox_config_backup-1.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-19 19:39:00.000000 netbox_config_backup-1.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:30:07.036311 netbox_config_backup-1.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-23 16:30:07.036311 netbox_config_backup-1.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:30:07.028311 netbox_config_backup-1.4.5/netbox_config_backup/
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:30:07.032311 netbox_config_backup-1.4.5/netbox_config_backup/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/api/nested_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/choices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/filtersets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:30:07.032311 netbox_config_backup-1.4.5/netbox_config_backup/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:30:07.032311 netbox_config_backup-1.4.5/netbox_config_backup/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/management/commands/enqueue_if_needed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/management/commands/fix_missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/management/commands/rebuild.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/management/commands/runbackup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:30:07.032311 netbox_config_backup-1.4.5/netbox_config_backup/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/migrations/0002_git_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/migrations/0003_primary_model_to_bigid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/migrations/0004_custom_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/migrations/0005_commit_add_time_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/migrations/0006_backup_add_commit_last_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/migrations/0007_backup_job_add_scheduled.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/migrations/0008_backupjob_scheduled_nullable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/migrations/0009_bctc_file_model_backup_fk_restructure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/migrations/0010_backup_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/migrations/0011_alter_backup_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/migrations/0012_backup_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/migrations/0013_backup__to_netboxmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:30:07.036311 netbox_config_backup-1.4.5/netbox_config_backup/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/models/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8279 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/models/backups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/models/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/template_content.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:30:07.024311 netbox_config_backup-1.4.5/netbox_config_backup/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:30:07.036311 netbox_config_backup-1.4.5/netbox_config_backup/templates/netbox_config_backup/
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/templates/netbox_config_backup/backup.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/templates/netbox_config_backup/backups.html
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/templates/netbox_config_backup/config.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/templates/netbox_config_backup/diff.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:30:07.036311 netbox_config_backup-1.4.5/netbox_config_backup/templates/netbox_config_backup/inc/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/templates/netbox_config_backup/inc/backup_tables.html
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/templates/netbox_config_backup/repository.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:30:07.036311 netbox_config_backup-1.4.5/netbox_config_backup/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/templatetags/ncb_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:30:07.036311 netbox_config_backup-1.4.5/netbox_config_backup/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/utils/backups.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/utils/rq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/netbox_config_backup/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:30:07.032311 netbox_config_backup-1.4.5/netbox_config_backup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-23 16:30:07.000000 netbox_config_backup-1.4.5/netbox_config_backup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-05-23 16:30:07.000000 netbox_config_backup-1.4.5/netbox_config_backup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 16:30:07.000000 netbox_config_backup-1.4.5/netbox_config_backup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 16:30:07.000000 netbox_config_backup-1.4.5/netbox_config_backup.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-23 16:30:07.000000 netbox_config_backup-1.4.5/netbox_config_backup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-23 16:30:07.000000 netbox_config_backup-1.4.5/netbox_config_backup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 16:30:07.036311 netbox_config_backup-1.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-23 16:30:02.000000 netbox_config_backup-1.4.5/setup.py
```

### Comparing `netbox_config_backup-1.4.4/LICENSE` & `netbox_config_backup-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.4/PKG-INFO` & `netbox_config_backup-1.4.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox_config_backup
-Version: 1.4.4
+Version: 1.4.5
 Summary: NetBox Configuration Backup
 Home-page: https://github.com/dansheps/netbox-config-backup/
 Download-URL: https://github.com/dansheps/netbox-config-backup/
 Author: Daniel Sheppard
 Author-email: dans@dansheps.com
 Maintainer: Daniel Sheppard
 Maintainer-email: dans@dansheps.com
```

### Comparing `netbox_config_backup-1.4.4/README.md` & `netbox_config_backup-1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.4/netbox_config_backup/__init__.py` & `netbox_config_backup-1.4.5/netbox_config_backup/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.4/netbox_config_backup/api/serializers.py` & `netbox_config_backup-1.4.5/netbox_config_backup/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.4/netbox_config_backup/choices.py` & `netbox_config_backup-1.4.5/netbox_config_backup/choices.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.4/netbox_config_backup/filtersets.py` & `netbox_config_backup-1.4.5/netbox_config_backup/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.4/netbox_config_backup/forms.py` & `netbox_config_backup-1.4.5/netbox_config_backup/forms.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.4/netbox_config_backup/git.py` & `netbox_config_backup-1.4.5/netbox_config_backup/git.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.4/netbox_config_backup/management/commands/fix_missing.py` & `netbox_config_backup-1.4.5/netbox_config_backup/management/commands/fix_missing.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.4/netbox_config_backup/management/commands/rebuild.py` & `netbox_config_backup-1.4.5/netbox_config_backup/management/commands/rebuild.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.4/netbox_config_backup/management/commands/runbackup.py` & `netbox_config_backup-1.4.5/netbox_config_backup/management/commands/runbackup.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.4/netbox_config_backup/migrations/0001_initial.py` & `netbox_config_backup-1.4.5/netbox_config_backup/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.4/netbox_config_backup/migrations/0002_git_models.py` & `netbox_config_backup-1.4.5/netbox_config_backup/migrations/0002_git_models.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.4/netbox_config_backup/migrations/0003_primary_model_to_bigid.py` & `netbox_config_backup-1.4.5/netbox_config_backup/migrations/0003_primary_model_to_bigid.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.4/netbox_config_backup/migrations/0006_backup_add_commit_last_time.py` & `netbox_config_backup-1.4.5/netbox_config_backup/migrations/0006_backup_add_commit_last_time.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.4/netbox_config_backup/migrations/0007_backup_job_add_scheduled.py` & `netbox_config_backup-1.4.5/netbox_config_backup/migrations/0007_backup_job_add_scheduled.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.4/netbox_config_backup/migrations/0009_bctc_file_model_backup_fk_restructure.py` & `netbox_config_backup-1.4.5/netbox_config_backup/migrations/0009_bctc_file_model_backup_fk_restructure.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.4/netbox_config_backup/migrations/0010_backup_ip.py` & `netbox_config_backup-1.4.5/netbox_config_backup/migrations/0010_backup_ip.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.4/netbox_config_backup/models/backups.py` & `netbox_config_backup-1.4.5/netbox_config_backup/models/backups.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.4/netbox_config_backup/models/jobs.py` & `netbox_config_backup-1.4.5/netbox_config_backup/models/jobs.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.4/netbox_config_backup/navigation.py` & `netbox_config_backup-1.4.5/netbox_config_backup/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.4/netbox_config_backup/tables.py` & `netbox_config_backup-1.4.5/netbox_config_backup/tables.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.4/netbox_config_backup/tasks.py` & `netbox_config_backup-1.4.5/netbox_config_backup/tasks.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.4/netbox_config_backup/template_content.py` & `netbox_config_backup-1.4.5/netbox_config_backup/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.4/netbox_config_backup/templates/netbox_config_backup/backup.html` & `netbox_config_backup-1.4.5/netbox_config_backup/templates/netbox_config_backup/backup.html`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.4/netbox_config_backup/templates/netbox_config_backup/backups.html` & `netbox_config_backup-1.4.5/netbox_config_backup/templates/netbox_config_backup/backups.html`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.4/netbox_config_backup/templates/netbox_config_backup/diff.html` & `netbox_config_backup-1.4.5/netbox_config_backup/templates/netbox_config_backup/diff.html`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.4/netbox_config_backup/urls.py` & `netbox_config_backup-1.4.5/netbox_config_backup/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.4/netbox_config_backup/utils/backups.py` & `netbox_config_backup-1.4.5/netbox_config_backup/utils/backups.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.4/netbox_config_backup/utils/git.py` & `netbox_config_backup-1.4.5/netbox_config_backup/utils/git.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.4/netbox_config_backup/utils/rq.py` & `netbox_config_backup-1.4.5/netbox_config_backup/utils/rq.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.4/netbox_config_backup/views.py` & `netbox_config_backup-1.4.5/netbox_config_backup/views.py`

 * *Files identical despite different names*

### Comparing `netbox_config_backup-1.4.4/netbox_config_backup.egg-info/PKG-INFO` & `netbox_config_backup-1.4.5/netbox_config_backup.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-config-backup
-Version: 1.4.4
+Version: 1.4.5
 Summary: NetBox Configuration Backup
 Home-page: https://github.com/dansheps/netbox-config-backup/
 Download-URL: https://github.com/dansheps/netbox-config-backup/
 Author: Daniel Sheppard
 Author-email: dans@dansheps.com
 Maintainer: Daniel Sheppard
 Maintainer-email: dans@dansheps.com
```

### Comparing `netbox_config_backup-1.4.4/netbox_config_backup.egg-info/SOURCES.txt` & `netbox_config_backup-1.4.5/netbox_config_backup.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 netbox_config_backup/migrations/0006_backup_add_commit_last_time.py
 netbox_config_backup/migrations/0007_backup_job_add_scheduled.py
 netbox_config_backup/migrations/0008_backupjob_scheduled_nullable.py
 netbox_config_backup/migrations/0009_bctc_file_model_backup_fk_restructure.py
 netbox_config_backup/migrations/0010_backup_ip.py
 netbox_config_backup/migrations/0011_alter_backup_name.py
 netbox_config_backup/migrations/0012_backup_status.py
+netbox_config_backup/migrations/0013_backup__to_netboxmodel.py
 netbox_config_backup/migrations/__init__.py
 netbox_config_backup/models/__init__.py
 netbox_config_backup/models/abstract.py
 netbox_config_backup/models/backups.py
 netbox_config_backup/models/jobs.py
 netbox_config_backup/templates/netbox_config_backup/backup.html
 netbox_config_backup/templates/netbox_config_backup/backups.html
```

### Comparing `netbox_config_backup-1.4.4/setup.py` & `netbox_config_backup-1.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='netbox_config_backup',
-    version='1.4.4',
+    version='1.4.5',
     description='NetBox Configuration Backup',
     long_description='Plugin to backup device configuration',
     url='https://github.com/dansheps/netbox-config-backup/',
     download_url='https://github.com/dansheps/netbox-config-backup/',
     author='Daniel Sheppard',
     author_email='dans@dansheps.com',
     maintainer='Daniel Sheppard',
```

