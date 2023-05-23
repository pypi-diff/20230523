# Comparing `tmp/django_pgclone-2.4.0.tar.gz` & `tmp/django_pgclone-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_pgclone-2.4.0.tar", max compression
+gzip compressed data, was "django_pgclone-2.5.0.tar", max compression
```

## Comparing `django_pgclone-2.4.0.tar` & `django_pgclone-2.5.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0     1456 2023-04-28 15:23:33.432068 django_pgclone-2.4.0/LICENSE
--rw-r--r--   0        0        0     2372 2023-04-28 15:23:33.432068 django_pgclone-2.4.0/README.rst
--rw-r--r--   0        0        0      196 2023-04-28 15:23:33.432068 django_pgclone-2.4.0/pgclone/__init__.py
--rw-r--r--   0        0        0     4004 2023-04-28 15:23:33.432068 django_pgclone-2.4.0/pgclone/db.py
--rw-r--r--   0        0        0     3351 2023-04-28 15:23:33.432068 django_pgclone-2.4.0/pgclone/dump_cmd.py
--rw-r--r--   0        0        0      438 2023-04-28 15:23:33.432068 django_pgclone-2.4.0/pgclone/exceptions.py
--rw-r--r--   0        0        0     2169 2023-04-28 15:23:33.432068 django_pgclone-2.4.0/pgclone/logging.py
--rw-r--r--   0        0        0     3521 2023-04-28 15:23:33.432068 django_pgclone-2.4.0/pgclone/ls_cmd.py
--rw-r--r--   0        0        0        0 2023-04-28 15:23:33.432068 django_pgclone-2.4.0/pgclone/management/__init__.py
--rw-r--r--   0        0        0        0 2023-04-28 15:23:33.432068 django_pgclone-2.4.0/pgclone/management/commands/__init__.py
--rw-r--r--   0        0        0     6457 2023-04-28 15:23:33.432068 django_pgclone-2.4.0/pgclone/management/commands/pgclone.py
--rw-r--r--   0        0        0     2483 2023-04-28 15:23:33.432068 django_pgclone-2.4.0/pgclone/options.py
--rw-r--r--   0        0        0     8964 2023-04-28 15:23:33.432068 django_pgclone-2.4.0/pgclone/restore_cmd.py
--rw-r--r--   0        0        0     1911 2023-04-28 15:23:33.432068 django_pgclone-2.4.0/pgclone/run.py
--rw-r--r--   0        0        0     1807 2023-04-28 15:23:33.432068 django_pgclone-2.4.0/pgclone/settings.py
--rw-r--r--   0        0        0     3202 2023-04-28 15:23:33.432068 django_pgclone-2.4.0/pgclone/storage.py
--rw-r--r--   0        0        0      152 2023-04-28 15:23:33.436068 django_pgclone-2.4.0/pgclone/version.py
--rw-r--r--   0        0        0     2333 2023-04-28 15:24:11.855854 django_pgclone-2.4.0/pyproject.toml
--rw-r--r--   0        0        0     3832 1970-01-01 00:00:00.000000 django_pgclone-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1456 2023-05-23 18:06:16.359548 django_pgclone-2.5.0/LICENSE
+-rw-r--r--   0        0        0     2372 2023-05-23 18:06:16.359548 django_pgclone-2.5.0/README.rst
+-rw-r--r--   0        0        0      196 2023-05-23 18:06:16.359548 django_pgclone-2.5.0/pgclone/__init__.py
+-rw-r--r--   0        0        0     2342 2023-05-23 18:06:16.359548 django_pgclone-2.5.0/pgclone/copy_cmd.py
+-rw-r--r--   0        0        0     4894 2023-05-23 18:06:16.359548 django_pgclone-2.5.0/pgclone/db.py
+-rw-r--r--   0        0        0     3487 2023-05-23 18:06:16.359548 django_pgclone-2.5.0/pgclone/dump_cmd.py
+-rw-r--r--   0        0        0      438 2023-05-23 18:06:16.359548 django_pgclone-2.5.0/pgclone/exceptions.py
+-rw-r--r--   0        0        0     2169 2023-05-23 18:06:16.359548 django_pgclone-2.5.0/pgclone/logging.py
+-rw-r--r--   0        0        0     3521 2023-05-23 18:06:16.359548 django_pgclone-2.5.0/pgclone/ls_cmd.py
+-rw-r--r--   0        0        0        0 2023-05-23 18:06:16.359548 django_pgclone-2.5.0/pgclone/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 18:06:16.359548 django_pgclone-2.5.0/pgclone/management/commands/__init__.py
+-rw-r--r--   0        0        0     7145 2023-05-23 18:06:16.359548 django_pgclone-2.5.0/pgclone/management/commands/pgclone.py
+-rw-r--r--   0        0        0     2483 2023-05-23 18:06:16.359548 django_pgclone-2.5.0/pgclone/options.py
+-rw-r--r--   0        0        0     8429 2023-05-23 18:06:16.359548 django_pgclone-2.5.0/pgclone/restore_cmd.py
+-rw-r--r--   0        0        0     1559 2023-05-23 18:06:16.359548 django_pgclone-2.5.0/pgclone/run.py
+-rw-r--r--   0        0        0     2048 2023-05-23 18:06:16.359548 django_pgclone-2.5.0/pgclone/settings.py
+-rw-r--r--   0        0        0     3505 2023-05-23 18:06:16.359548 django_pgclone-2.5.0/pgclone/storage.py
+-rw-r--r--   0        0        0      152 2023-05-23 18:06:16.359548 django_pgclone-2.5.0/pgclone/version.py
+-rw-r--r--   0        0        0     2333 2023-05-23 18:06:54.895585 django_pgclone-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3832 1970-01-01 00:00:00.000000 django_pgclone-2.5.0/PKG-INFO
```

### Comparing `django_pgclone-2.4.0/LICENSE` & `django_pgclone-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_pgclone-2.4.0/README.rst` & `django_pgclone-2.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `django_pgclone-2.4.0/pgclone/db.py` & `django_pgclone-2.5.0/pgclone/db.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import functools
 import shlex
 
 from django.conf import settings as django_settings
 from django.db import connections, DEFAULT_DB_ALIAS
 from django.db.utils import load_backend
 
-from pgclone import exceptions, settings
+from pgclone import exceptions, run, settings
 
 
 def _no_queries_during_routing(execute, sql, params, many, context):  # pragma: no cover
     alias = context["connection"].alias
     raise RuntimeError(f'Cannot query non-default database "{alias}" during pgclone hooks')
 
 
@@ -67,31 +67,32 @@
     database.setdefault("TIME_ZONE", None)
     for setting in ["NAME", "USER", "PASSWORD", "HOST", "PORT"]:
         database.setdefault(setting, "")
 
     return database
 
 
-def make(db_name, *, using):
+def make(db_name, *, using, check=True):
     """Returns a DB config dict for the database named "db_name"
 
     Also ensures that no other database are configured with the provided
     database name. This is a sanity check to make sure that no dynamic
     databases used by pgclone collide with any that already exist.
 
     Note: In a multi-DB setup, this check might produce errors that don't
     need to happen, such as restricting one from using a name on an
     entirely different DB. We can handle this edge case later
     """
-    for db in django_settings.DATABASES.values():
-        if db.get("NAME") == db_name:  # pragma: no cover
-            raise exceptions.RuntimeError(
-                f'pgclone cannot use temporary database named "{db_name}"'
-                " since it is already configured in settings.DATABASES."
-            )
+    if check:
+        for db in django_settings.DATABASES.values():
+            if db.get("NAME") == db_name:  # pragma: no cover
+                raise exceptions.RuntimeError(
+                    f'pgclone cannot use temporary database named "{db_name}"'
+                    " since it is already configured in settings.DATABASES."
+                )
 
     db_config = conf(using=using)
     db_config["NAME"] = db_name
     return db_config
 
 
 @functools.lru_cache()
@@ -102,7 +103,32 @@
 
 def url(db_config):
     """Convert a database dictionary config to a url"""
     return shlex.quote(
         f'postgresql://{db_config["USER"]}:{db_config["PASSWORD"]}'
         f'@{db_config["HOST"]}:{db_config["PORT"]}/{db_config["NAME"]}'
     )
+
+
+def psql(sql, *, using, ignore_errors=False):
+    """Runs psql -c with properly formatted SQL"""
+    db_url = url(conn(using=using))
+
+    # Format special SQL characters
+    sql = sql.replace("$", "\\$").replace("\n", " ").replace('"', '\\"').strip()
+    return run.shell(f'psql {db_url} -P pager=off -c "{sql};"', ignore_errors=ignore_errors)
+
+
+def kill_connections(database, *, using):
+    kill_connections_sql = f"""
+        SELECT pg_terminate_backend(pg_stat_activity.pid)
+        FROM pg_stat_activity
+        WHERE pg_stat_activity.datname = '{database["NAME"]}'
+            AND pid <> pg_backend_pid()
+    """
+    psql(kill_connections_sql, using=using)
+
+
+def drop(database, *, using):
+    kill_connections(database, using=using)
+    drop_sql = f'DROP DATABASE IF EXISTS "{database["NAME"]}"'
+    psql(drop_sql, using=using)
```

### Comparing `django_pgclone-2.4.0/pgclone/dump_cmd.py` & `django_pgclone-2.5.0/pgclone/dump_cmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import datetime as dt
 import os
 import re
 
 from django.apps import apps
 
-from pgclone import db, logging, options, run, storage
+from pgclone import db, exceptions, logging, options, run, settings, storage
 
 
 DT_FORMAT = "%Y-%m-%d-%H-%M-%S-%f"
 
 
 def _dump_key(*, instance, database, config):
     """Obtain the key for the db dump"""
@@ -17,14 +17,17 @@
     database = re.sub(r"[^a-zA-Z0-9_-]", "_", database)
     config_name = re.sub(r"[^a-zA-Z0-9_-]", "_", config)
     return os.path.join(instance, database, config_name, f"{now}.dump")
 
 
 def _dump(*, exclude, config, pre_dump_hooks, instance, database, storage_location):
     """Dump implementation"""
+    if not settings.allow_dump():  # pragma: no cover
+        raise exceptions.RuntimeError("Dump not allowed.")
+
     storage_client = storage.client(storage_location)
     dump_db = db.conf(using=database)
 
     # pre-dump hooks
     with db.route(dump_db):
         for management_command_name in pre_dump_hooks:  # pragma: no cover
             logging.success_msg(f'Running "manage.py {management_command_name}" pre_dump hook')
```

### Comparing `django_pgclone-2.4.0/pgclone/logging.py` & `django_pgclone-2.5.0/pgclone/logging.py`

 * *Files identical despite different names*

### Comparing `django_pgclone-2.4.0/pgclone/ls_cmd.py` & `django_pgclone-2.5.0/pgclone/ls_cmd.py`

 * *Files identical despite different names*

### Comparing `django_pgclone-2.4.0/pgclone/management/commands/pgclone.py` & `django_pgclone-2.5.0/pgclone/management/commands/pgclone.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 
 from django.core.management.base import BaseCommand
 
-from pgclone import dump_cmd, exceptions, logging, ls_cmd, restore_cmd
+from pgclone import copy_cmd, dump_cmd, exceptions, logging, ls_cmd, restore_cmd
 
 
 class Subcommands(BaseCommand):
     """
     Subcommand class vendored in from
     https://github.com/andrewp-as-is/django-subcommands.py
     because of installation issues
@@ -179,13 +179,36 @@
             reversible=options["reversible"],
             database=options["database"],
             storage_location=options["storage_location"],
             config=options["config"],
         )
 
 
+class CopyCommand(BaseSubcommand):
+    def add_arguments(self, parser):
+        parser.add_argument("dump_key", nargs="?", help="The local dump key to copy to.")
+        parser.add_argument(
+            "-d",
+            "--database",
+            help="Restore to this database.",
+        )
+        parser.add_argument(
+            "-c",
+            "--config",
+            help="Use this configuration to supply default option values.",
+        )
+
+    def subhandle(self, *args, **options):
+        copy_cmd.copy(
+            dump_key=options["dump_key"],
+            database=options["database"],
+            config=options["config"],
+        )
+
+
 class Command(Subcommands):
     subcommands = {
         "ls": LsCommand,
         "dump": DumpCommand,
         "restore": RestoreCommand,
+        "copy": CopyCommand,
     }
```

### Comparing `django_pgclone-2.4.0/pgclone/options.py` & `django_pgclone-2.5.0/pgclone/options.py`

 * *Files identical despite different names*

### Comparing `django_pgclone-2.4.0/pgclone/restore_cmd.py` & `django_pgclone-2.5.0/pgclone/restore_cmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,45 +11,29 @@
     try:
         run.shell(f'psql {conn_db_url} -lqt | cut -d \\| -f 1 | grep -qw {database["NAME"]}')
         return True
     except RuntimeError:
         return False
 
 
-def _kill_connections_to_db(database, *, using):
-    kill_connections_sql = f"""
-        SELECT pg_terminate_backend(pg_stat_activity.pid)
-        FROM pg_stat_activity
-        WHERE pg_stat_activity.datname = '{database["NAME"]}'
-            AND pid <> pg_backend_pid()
-    """
-    run.psql(kill_connections_sql, using=using)
-
-
-def _drop_db(database, *, using):
-    _kill_connections_to_db(database, using=using)
-    drop_sql = f'DROP DATABASE IF EXISTS "{database["NAME"]}"'
-    run.psql(drop_sql, using=using)
-
-
 def _set_search_path(database, *, using):
     """
     pg_restore does not restore the original search_path variable of the
     database, which can cause issues with extensions. This function obtains
     the original search path and sets it as the search path of the restored
     database
 
     https://www.postgresql.org/message-id/CAKFQuwbWpd1DXA_YY3zXRKGKKLL1ZTi9MHDQ15zJ8ufVBwVJEA%40mail.gmail.com
     """
     with connections[using].cursor() as cursor:
         cursor.execute("SHOW search_path;")
         search_path = cursor.fetchone()[0]
 
     set_search_path_sql = f'ALTER DATABASE "{database["NAME"]}" SET search_path to {search_path}'
-    run.psql(set_search_path_sql, using=using)
+    db.psql(set_search_path_sql, using=using)
 
 
 def _local_restore(dump_key, *, temp_db, curr_db, prev_db, using):
     """
     Performs a restore using a local database
     """
     if dump_key == ":current":
@@ -65,20 +49,20 @@
             ' Use "pgclone ls --local" to see local database keys.'
         )
 
     # Perform the local restore process. It is completely valid to
     # try to restore the temp_db, so do nothing if this database
     # is provided by the user
     if local_restore_db != temp_db:  # pragma: no branch
-        _drop_db(temp_db, using=using)
+        db.drop(temp_db, using=using)
         create_temp_sql = f"""
             CREATE DATABASE "{temp_db["NAME"]}"
             TEMPLATE "{local_restore_db["NAME"]}"
         """
-        run.psql(create_temp_sql, using=using)
+        db.psql(create_temp_sql, using=using)
 
     _set_search_path(temp_db, using=using)
 
     return dump_key
 
 
 def _remote_restore(dump_key, *, temp_db, using, storage_location):
@@ -97,17 +81,17 @@
             )
 
         dump_key = found_dump_key
 
     file_path = os.path.join(storage_location, dump_key)
 
     logging.success_msg("Creating the temporary restore db")
-    _drop_db(temp_db, using=using)
+    db.drop(temp_db, using=using)
     create_temp_sql = f'CREATE DATABASE "{temp_db["NAME"]}"'
-    run.psql(create_temp_sql, using=using)
+    db.psql(create_temp_sql, using=using)
     _set_search_path(temp_db, using=using)
 
     logging.success_msg(f'Running pg_restore on "{dump_key}"')
     pg_restore_cmd = f"pg_restore --verbose --no-acl --no-owner -d {db.url(temp_db)}"
     pg_restore_cmd = storage_client.pg_restore(file_path) + " " + pg_restore_cmd
 
     # When restoring, we need to ignore errors because there are certain
@@ -161,51 +145,51 @@
             dump_key, temp_db=temp_db, using=database, storage_location=storage_location
         )
 
     # When in reversible mode, make a special __curr db snapshot.
     # Avoid this if we are restoring the current db
     if reversible and local_restore_db != curr_db:
         logging.success_msg("Creating snapshot for reversible restore")
-        _drop_db(curr_db, using=database)
+        db.drop(curr_db, using=database)
         create_current_db_sql = f"""
             CREATE DATABASE "{curr_db['NAME']}"
              WITH TEMPLATE
             "{temp_db['NAME']}"
         """
-        run.psql(create_current_db_sql, using=database)
+        db.psql(create_current_db_sql, using=database)
 
     # pre-swap hook step
     with db.route(temp_db):
         for management_command_name in pre_swap_hooks:
             logging.success_msg(f'Running "manage.py {management_command_name}" pre_swap hook')
             run.management(management_command_name)
 
     # swap step
     logging.success_msg("Swapping the restored copy with the primary database")
-    _drop_db(prev_db, using=database)
-    _kill_connections_to_db(restore_db, using=database)
+    db.drop(prev_db, using=database)
+    db.kill_connections(restore_db, using=database)
     alter_db_sql = f"""
         ALTER DATABASE "{restore_db['NAME']}" RENAME TO
         "{prev_db['NAME']}"
     """
     # There's a scenario where the default DB may not exist before running
     # this, so just ignore errors on this command
-    run.psql(alter_db_sql, ignore_errors=True, using=database)
+    db.psql(alter_db_sql, ignore_errors=True, using=database)
 
-    _kill_connections_to_db(temp_db, using=database)
+    db.kill_connections(temp_db, using=database)
     rename_sql = f"""
         ALTER DATABASE "{temp_db["NAME"]}"
         RENAME TO "{restore_db["NAME"]}"
     """
-    run.psql(rename_sql, using=database)
+    db.psql(rename_sql, using=database)
 
     if not reversible:
         logging.success_msg("Cleaning old pgclone resources")
-        _drop_db(curr_db, using=database)
-        _drop_db(prev_db, using=database)
+        db.drop(curr_db, using=database)
+        db.drop(prev_db, using=database)
 
     logging.success_msg(f'Successfully restored dump "{dump_key}" to database "{database}"')
 
     return dump_key
 
 
 def restore(
```

### Comparing `django_pgclone-2.4.0/pgclone/run.py` & `django_pgclone-2.5.0/pgclone/run.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import contextlib
 import io
 import os
 import subprocess
 
 from django.core.management import call_command
 
-from pgclone import db, exceptions, logging
+from pgclone import exceptions, logging
 
 
 def shell(cmd, ignore_errors=False, env=None):
     """
     Utility for running a command. Ensures that an error
     is raised if it fails.
     """
@@ -47,16 +47,7 @@
         # If an exception happened, be sure to print off any stdout/stderr
         # leading up the error and log the exception.
         logger.info(output.getvalue())
         logger.exception(f'An exception occurred during "manage.py {cmd}"')
         raise
     else:
         logger.info(output.getvalue())
-
-
-def psql(sql, *, using, ignore_errors=False):
-    """Runs psql -c with properly formatted SQL"""
-    db_url = db.url(db.conn(using=using))
-
-    # Format special SQL characters
-    sql = sql.replace("$", "\\$").replace("\n", " ").replace('"', '\\"').strip()
-    return shell(f'psql {db_url} -P pager=off -c "{sql};"', ignore_errors=ignore_errors)
```

### Comparing `django_pgclone-2.4.0/pgclone/settings.py` & `django_pgclone-2.5.0/pgclone/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 from pgclone import exceptions
 
 
 def s3_config():
     return getattr(settings, "PGCLONE_S3_CONFIG", {})
 
 
+def s3_endpoint_url():
+    return getattr(settings, "PGCLONE_S3_ENDPOINT_URL", None)
+
+
 def storage_location():
     location = getattr(settings, "PGCLONE_STORAGE_LOCATION", ".pgclone")
     if not location.endswith("/"):  # pragma: no cover
         location += "/"
     return location
 
 
@@ -22,14 +26,22 @@
     return getattr(settings, "PGCLONE_REVERSIBLE", False)
 
 
 def allow_restore():
     return getattr(settings, "PGCLONE_ALLOW_RESTORE", True)
 
 
+def allow_dump():
+    return getattr(settings, "PGCLONE_ALLOW_DUMP", True)
+
+
+def allow_copy():
+    return getattr(settings, "PGCLONE_ALLOW_COPY", True)
+
+
 def configs():
     return getattr(settings, "PGCLONE_CONFIGS", {})
 
 
 def validate_dump_keys():
     return getattr(settings, "PGCLONE_VALIDATE_DUMP_KEYS", True)
```

### Comparing `django_pgclone-2.4.0/pgclone/storage.py` & `django_pgclone-2.5.0/pgclone/storage.py`

 * *Files 14% similar despite different names*

```diff
@@ -42,38 +42,44 @@
         """Given a file path, generates the CLI fragment to prepend to pg_restore"""
         pass
 
 
 class S3(Storage):
     def __init__(self, *args, **kwargs):
         validate_s3_support()
+        self.s3_endpoint_url = (
+            f" --endpoint-url {settings.s3_endpoint_url()}"
+            if settings.s3_endpoint_url() is not None
+            and isinstance(settings.s3_endpoint_url(), str)
+            else ""
+        )
         super().__init__(*args, **kwargs)
 
     def ls(self, prefix=None):  # pragma: no cover
         s3_path = os.path.join(self.storage_location, prefix or "")
         s3_bucket = "s3://" + s3_path[5:].split("/", 1)[0]
-        cmd = f"aws s3 ls {s3_path} --recursive | cut -c32-"
+        cmd = f"aws s3 ls {s3_path}{self.s3_endpoint_url} --recursive | cut -c32-"
         process = subprocess.run(
             cmd, shell=True, stdout=subprocess.PIPE, check=True, env=dict(os.environ, **self.env)
         )
         abs_paths = [
             os.path.join(s3_bucket, path)
             for path in process.stdout.decode("utf-8").split("\n")
             if path
         ]
         return [self.dump_key(path) for path in abs_paths]
 
     def get_env(self):
         return settings.s3_config()
 
     def pg_dump(self, file_path):
-        return f"| aws s3 cp - {file_path}"
+        return f"| aws s3 cp - {file_path}{self.s3_endpoint_url}"
 
     def pg_restore(self, file_path):
-        return f"aws s3 cp {file_path} - |"
+        return f"aws s3 cp {file_path} -{self.s3_endpoint_url} |"
 
 
 class Local(Storage):
     def ls(self, prefix=None):
         abs_paths = [
             os.path.join(dirpath, file_name)
             for dirpath, _, file_names in os.walk(self.storage_location)
```

### Comparing `django_pgclone-2.4.0/pyproject.toml` & `django_pgclone-2.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 name = "django-pgclone"
 packages = [
   { include = "pgclone" }
 ]
 exclude = [
   "*/tests/"
 ]
-version = "2.4.0"
+version = "2.5.0"
 description = "Dump and restore Postgres databases with Django."
 authors = ["Wes Kendall", "Ethan O'Brien"]
 classifiers = [
   "Framework :: Django",
   "Framework :: Django :: 2.2",
   "Framework :: Django :: 3.2",
   "Framework :: Django :: 4.0",
```

### Comparing `django_pgclone-2.4.0/PKG-INFO` & `django_pgclone-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pgclone
-Version: 2.4.0
+Version: 2.5.0
 Summary: Dump and restore Postgres databases with Django.
 Home-page: https://github.com/Opus10/django-pgclone
 License: BSD-3-Clause
 Author: Wes Kendall
 Requires-Python: >=3.7.0,<4
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
```

