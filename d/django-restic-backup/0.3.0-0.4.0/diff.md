# Comparing `tmp/django_restic_backup-0.3.0.tar.gz` & `tmp/django_restic_backup-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_restic_backup-0.3.0.tar", max compression
+gzip compressed data, was "django_restic_backup-0.4.0.tar", max compression
```

## Comparing `django_restic_backup-0.3.0.tar` & `django_restic_backup-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0        0 2022-12-06 09:35:26.515979 django_restic_backup-0.3.0/LICENSE
--rw-r--r--   0        0        0      523 2023-03-09 11:20:14.910169 django_restic_backup-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-12-06 09:35:26.515979 django_restic_backup-0.3.0/restore/__init__.py
--rw-r--r--   0        0        0       63 2022-12-06 09:35:26.515979 django_restic_backup-0.3.0/restore/admin.py
--rw-r--r--   0        0        0      146 2023-02-17 11:09:31.266210 django_restic_backup-0.3.0/restore/apps.py
--rw-r--r--   0        0        0     1495 2023-03-09 11:20:14.910169 django_restic_backup-0.3.0/restore/common_commands.py
--rw-r--r--   0        0        0        0 2022-12-06 09:35:26.515979 django_restic_backup-0.3.0/restore/management/__init__.py
--rw-r--r--   0        0        0      150 2022-12-06 09:35:26.515979 django_restic_backup-0.3.0/restore/management/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0        0 2022-12-06 09:35:26.515979 django_restic_backup-0.3.0/restore/management/commands/__init__.py
--rw-r--r--   0        0        0      159 2022-12-06 09:35:26.515979 django_restic_backup-0.3.0/restore/management/commands/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     8846 2022-12-06 09:35:26.519979 django_restic_backup-0.3.0/restore/management/commands/__pycache__/restore2.cpython-38.pyc
--rw-r--r--   0        0        0    14267 2023-03-09 11:20:14.910169 django_restic_backup-0.3.0/restore/management/commands/restore.py
--rw-r--r--   0        0        0        0 2022-12-06 09:35:26.519979 django_restic_backup-0.3.0/restore/migrations/__init__.py
--rw-r--r--   0        0        0       57 2022-12-06 09:35:26.519979 django_restic_backup-0.3.0/restore/models.py
--rw-r--r--   0        0        0       60 2022-12-06 09:35:26.519979 django_restic_backup-0.3.0/restore/tests.py
--rw-r--r--   0        0        0       63 2022-12-06 09:35:26.519979 django_restic_backup-0.3.0/restore/views.py
--rw-r--r--   0        0        0      852 1970-01-01 00:00:00.000000 django_restic_backup-0.3.0/setup.py
--rw-r--r--   0        0        0      612 1970-01-01 00:00:00.000000 django_restic_backup-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-12-06 09:35:26.515979 django_restic_backup-0.4.0/LICENSE
+-rw-r--r--   0        0        0      523 2023-05-23 13:46:38.892609 django_restic_backup-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-12-06 09:35:26.515979 django_restic_backup-0.4.0/restore/__init__.py
+-rw-r--r--   0        0        0       63 2022-12-06 09:35:26.515979 django_restic_backup-0.4.0/restore/admin.py
+-rw-r--r--   0        0        0      146 2023-02-17 11:09:31.266210 django_restic_backup-0.4.0/restore/apps.py
+-rw-r--r--   0        0        0     1495 2023-03-09 11:20:14.910169 django_restic_backup-0.4.0/restore/common_commands.py
+-rw-r--r--   0        0        0        0 2022-12-06 09:35:26.515979 django_restic_backup-0.4.0/restore/management/__init__.py
+-rw-r--r--   0        0        0      150 2022-12-06 09:35:26.515979 django_restic_backup-0.4.0/restore/management/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0        0 2022-12-06 09:35:26.515979 django_restic_backup-0.4.0/restore/management/commands/__init__.py
+-rw-r--r--   0        0        0      159 2022-12-06 09:35:26.515979 django_restic_backup-0.4.0/restore/management/commands/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     8846 2022-12-06 09:35:26.519979 django_restic_backup-0.4.0/restore/management/commands/__pycache__/restore2.cpython-38.pyc
+-rw-r--r--   0        0        0    19760 2023-05-23 13:46:38.892609 django_restic_backup-0.4.0/restore/management/commands/restore.py
+-rw-r--r--   0        0        0        0 2022-12-06 09:35:26.519979 django_restic_backup-0.4.0/restore/migrations/__init__.py
+-rw-r--r--   0        0        0       57 2022-12-06 09:35:26.519979 django_restic_backup-0.4.0/restore/models.py
+-rw-r--r--   0        0        0       60 2022-12-06 09:35:26.519979 django_restic_backup-0.4.0/restore/tests.py
+-rw-r--r--   0        0        0       63 2022-12-06 09:35:26.519979 django_restic_backup-0.4.0/restore/views.py
+-rw-r--r--   0        0        0      612 1970-01-01 00:00:00.000000 django_restic_backup-0.4.0/PKG-INFO
```

### Comparing `django_restic_backup-0.3.0/pyproject.toml` & `django_restic_backup-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-restic-backup"
-version = "0.3.0"
+version = "0.4.0"
 description = "Restore files or/and database backup from an environment (backup server) with encrypted secret file after decrypting it (secret file is defined in settings.BACKUP_CONF_FILE"
 authors = ["Dedomainia"]
 packages = [
     { include = "restore/" }
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `django_restic_backup-0.3.0/restore/common_commands.py` & `django_restic_backup-0.4.0/restore/common_commands.py`

 * *Files identical despite different names*

### Comparing `django_restic_backup-0.3.0/restore/management/commands/__pycache__/restore2.cpython-38.pyc` & `django_restic_backup-0.4.0/restore/management/commands/__pycache__/restore2.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django_restic_backup-0.3.0/restore/management/commands/restore.py` & `django_restic_backup-0.4.0/restore/management/commands/restore.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import base64
 import getpass
 import multiprocessing
 import os
 import re
 import subprocess  # nosec
+from datetime import datetime, timezone
 from distutils.dir_util import copy_tree
 from pathlib import Path
 
 import yaml
 from cryptography.fernet import Fernet, InvalidToken
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.kdf.pbkdf2 import PBKDF2HMAC
@@ -20,14 +21,35 @@
     help = (
         "Restore files or/and database backup from an environment (backup server) "
         "with encrypted secret file after decrypting it (secret file is defined in "
         "settings.BACKUP_CONF_FILE)"
     )
 
     def handle(self, *args, **options):
+        # postgres_db, dump_name and files_path can be used as a django parameter
+        # or as a command line parameter.
+        # The command line has priority.
+        if options["postgres_db"] is None:
+            try:
+                options["postgres_db"] = settings.USE_POSTGRES_DB
+            except AttributeError:
+                options["postgres_db"] = False
+
+        if options["dump_name"] is None:
+            try:
+                options["dump_name"] = settings.DB_BACKUP_DUMP_NAME
+            except AttributeError:
+                options["dump_name"] = False
+
+        if options["files_path"] is None:
+            try:
+                options["files_path"] = settings.FILES_BACKUP_PATH
+            except AttributeError:
+                options["files_path"] = False
+
         if options["encrypt"] is True and options["decrypt"] is True:
             return self.error(
                 "You can not use both encrypt and decrypt options at the same time"
             )
 
         if options["db_only"] is True and options["files_only"] is True:
             return self.error(
@@ -42,15 +64,14 @@
 
         try:
             self.management(options, should_manage_app_and_db)
         except InvalidToken:
             return self.error("Invalid password")
 
     def management(self, options, should_manage_app_and_db):
-
         conf = self.get_backup_conf()
         key = self.create_key(confirm_password=options["encrypt"])
 
         if options["encrypt"] is True:
             # Just encrypt the conf file
             if should_manage_app_and_db is True or options["db_only"] is True:
                 # Encrypt restic database backup configuration
@@ -81,37 +102,43 @@
                 # Show secrets of database backup configuration
                 self.display_secret(conf, options["name_env"], "DB", key)
             if should_manage_app_and_db is True or options["files_only"] is True:
                 # Show secrets of documents backup configuration
                 self.display_secret(conf, options["name_env"], "APP", key)
         else:
             # decrypt conf file and restore backup
-            lisa_conf = self.get_db_conf()
+            db_conf = self.get_db_conf()
             if should_manage_app_and_db is True or options["db_only"] is True:
                 # Restore or unlock database
                 db_access = self.decrypt(conf, options["name_env"], "DB", key)
                 self.set_restic_access(db_access)
                 if options["unlock"] is True:
                     self.unlock_backups("db")
                 elif options["list_snapshots"] is True:
                     self.list_snapshots()
                 else:
-                    self.get_backup_db(lisa_conf, options["db_id"])
+                    self.get_backup_db(
+                        db_conf=db_conf,
+                        backup_id=options["db_id"],
+                        dump_name=options["dump_name"],
+                        postgres_db=options["postgres_db"],
+                    )
 
             if should_manage_app_and_db is True or options["files_only"] is True:
                 # Restore or unlock app documents
                 app_access = self.decrypt(conf, options["name_env"], "APP", key)
                 self.set_restic_access(app_access)
                 if options["unlock"] is True:
                     self.unlock_backups("app")
                 elif options["list_snapshots"] is True:
                     self.list_snapshots()
                 else:
-                    self.get_backup_documents(options["app_id"], options["deal"])
-                    self.success("Restoration of documents completed.")
+                    self.get_backup_documents(
+                        options["app_id"], options["deal"], options["files_path"]
+                    )
 
     def add_arguments(self, parser):
         parser.add_argument(
             "name_env",
             type=str,
             help="Name of env to back up "
             '(like primary for "digital ocean" and secondary for "aws")',
@@ -183,32 +210,54 @@
             help="show the secret decrypted configured for the environment selected",
         )
         parser.add_argument(
             "--deal",
             type=str,
             help="Deal folder that should be retrive",
         )
+        parser.add_argument(
+            "--postgres_db",
+            default=None,
+            required=False,
+            action="store_true",
+            help="Use postgres database, default: mysql",
+        )
+        parser.add_argument(
+            "--dump_name",
+            type=str,
+            default=None,
+            required=False,
+            help="Name of dump",
+        )
+        parser.add_argument(
+            "--files_path",
+            type=str,
+            default=None,
+            required=False,
+            help="Name of path of documents",
+        )
 
     def get_db_conf(self):
-        f = open(settings.CONF_FILE, mode="r")
-        conf_content = f.read()
-        lisa_conf = {}
-        data = re.search(r'USER\"\s*:\s*"(.+)"', conf_content)
-        lisa_conf["USER"] = data.group(1)
-        data = re.search(r'PASSWORD\"\s*:\s*"(.+)"', conf_content)
-        lisa_conf["PASSWORD"] = data.group(1)
-        data = re.search(r'NAME\"\s*:\s*"(.+)"', conf_content)
-        lisa_conf["NAME"] = data.group(1)
-        data = re.search(r'HOST\"\s*:\s*"(.+)"', conf_content)
-        if data is not None:
-            lisa_conf["HOST"] = data.group(1)
-        data = re.search(r'PORT\"\s*:\s*"(.+)"', conf_content)
-        if data is not None:
-            lisa_conf["PORT"] = data.group(1)
-        return lisa_conf
+        db_configuration = {}
+
+        with open(settings.CONF_FILE, mode="r") as f:
+            conf_content = f.read()
+            data = re.search(r'USER\"\s*:\s*"(.+)"', conf_content)
+            db_configuration["USER"] = data.group(1)
+            data = re.search(r'PASSWORD\"\s*:\s*"(.+)"', conf_content)
+            db_configuration["PASSWORD"] = data.group(1)
+            data = re.search(r'NAME\"\s*:\s*"(.+)"', conf_content)
+            db_configuration["NAME"] = data.group(1)
+            data = re.search(r'HOST\"\s*:\s*"(.+)"', conf_content)
+            if data is not None:
+                db_configuration["HOST"] = data.group(1)
+            data = re.search(r'PORT\"\s*:\s*"(.+)"', conf_content)
+            if data is not None:
+                db_configuration["PORT"] = data.group(1)
+        return db_configuration
 
     def get_backup_conf(self):
         with open(settings.BACKUP_CONF_FILE) as file:
             conf = yaml.load(file, Loader=yaml.SafeLoader)
             return conf
 
     def encrypt(self, conf, env, type, key):
@@ -280,71 +329,158 @@
         os.environ["RESTIC_REPOSITORY"] = re.search(
             'RESTIC_REPOSITORY="(.+)"', access_str
         ).group(1)
         os.environ["RESTIC_PASSWORD"] = re.search(
             'RESTIC_PASSWORD="(.+)"', access_str
         ).group(1)
 
-    def get_backup_db(self, lisa_conf, backup_id):
-        p1 = subprocess.Popen(  # nosec
-            ["restic", "dump", backup_id, "icarus_test.sql.gz"],
-            stdout=subprocess.PIPE,
-            stderr=subprocess.PIPE,
-        )
-        p2 = subprocess.Popen(  # nosec
-            ["pigz", "-d"],
-            stdin=p1.stdout,
-            stdout=subprocess.PIPE,
-            stderr=subprocess.PIPE,
-        )
-        p3 = subprocess.Popen(  # nosec
-            [
-                "mysql",
-                "-u",
-                lisa_conf["USER"],
-                lisa_conf["NAME"],
-                f"-p{lisa_conf['PASSWORD']}",
-            ]
-            + (["-h", lisa_conf["HOST"]] if "HOST" in lisa_conf else []),
-            stdin=p2.stdout,
-            stdout=subprocess.PIPE,
-            stderr=subprocess.PIPE,
+        # self.success(os.environ)
+
+    def get_backup_db(self, db_conf, backup_id, dump_name: str, postgres_db: bool):
+        self.info(f"Requested: {os.environ['RESTIC_REPOSITORY']}")
+
+        self.warning(
+            "The database must be empty before continuing with the restore command. "
+            "Drop and recreate a database manually before proceeding if this is not the case."
         )
-        (output3, err3) = p3.communicate()
-        (output2, err2) = p2.communicate()
-        (output1, err1) = p1.communicate()
-        if (
-            len(err3.decode("utf-8")) != 0
-            or len(err2.decode("utf-8")) != 0
-            or len(err1.decode("utf-8")) != 0
-        ):
+
+        pw = input("Do you want to continue ? (type y for yes)\n")
+        if pw != "y":
+            self.error("Restoration canceled")
+            return
+
+        if postgres_db:
+            dump_file_path = f"dump_{backup_id}.sql"
+
+            self.warning(
+                f"WARNING. You should remove database dump file ("
+                + dump_file_path
+                + ") on this system after the restoration."
+            )
+
+            remove_dump_file_after_restore = False
+            if backup_id == "latest":
+                # to avoid different latest dump
+                remove_dump_file_after_restore = True
+            else:
+                pw = input(
+                    "Do you want to remove it after database restoration ? (tape n for no)\n"
+                )
+                if pw != "n":
+                    remove_dump_file_after_restore = True
+
+            self.info(
+                "Database restoration in progress... Started at "
+                + self.get_datetime_now()
+            )
+
+            errors = ""
+
+            if os.path.isfile(dump_file_path):
+                self.info(
+                    "Download skipped. The dump file already exists locally. "
+                    "It is it that will be used for the restoration."
+                )
+            else:
+                self.info("Downloading dump...")
+                dump_file = open(dump_file_path, "wb")
+
+                p1 = subprocess.Popen(  # nosec
+                    ["restic", "dump", backup_id, dump_name],
+                    stdout=dump_file,
+                    stderr=subprocess.PIPE,
+                )
+                (output1, err1) = p1.communicate()
+                errors += err1.decode("utf-8")
+
+                dump_file.flush()
+                dump_file.close()
+
+            if len(errors) == 0:
+                os.environ["PGPASSWORD"] = db_conf["PASSWORD"]
+                p2 = subprocess.Popen(  # nosec
+                    [
+                        "pg_restore",
+                        "-Fc",
+                        "-d",
+                        db_conf["NAME"],
+                        "-U",
+                        db_conf["USER"],
+                        "-h",
+                        db_conf["HOST"],
+                    ]
+                    + (["-p", db_conf["PORT"]] if "PORT" in db_conf else [])
+                    + (["-1", dump_file_path]),
+                    stdout=subprocess.PIPE,
+                    stderr=subprocess.PIPE,
+                )
+
+                self.info("Dump loading...")
+                (output2, err2) = p2.communicate()
+                errors = err2.decode("utf-8") + errors
+
+                if remove_dump_file_after_restore:
+                    os.remove(dump_file_path)
+                    self.info("Dump file (" + dump_file_path + ") removed.")
+        else:
+            self.info(
+                "Database restoration in progress... Started at "
+                + self.get_datetime_now()
+            )
+            p1 = subprocess.Popen(  # nosec
+                ["restic", "dump", backup_id, dump_name],
+                stdout=subprocess.PIPE,
+                stderr=subprocess.PIPE,
+            )
+            p2 = subprocess.Popen(  # nosec
+                ["pigz", "-d"],
+                stdin=p1.stdout,
+                stdout=subprocess.PIPE,
+                stderr=subprocess.PIPE,
+            )
+            p3 = subprocess.Popen(  # nosec
+                [
+                    "mysql",
+                    "-u",
+                    db_conf["USER"],
+                    db_conf["NAME"],
+                    f"-p{db_conf['PASSWORD']}",
+                ]
+                + (["-h", db_conf["HOST"]] if "HOST" in db_conf else []),
+                stdin=p2.stdout,
+                stdout=subprocess.PIPE,
+                stderr=subprocess.PIPE,
+            )
+            (output3, err3) = p3.communicate()
+            (output2, err2) = p2.communicate()
+            (output1, err1) = p1.communicate()
+            errors = err3.decode("utf-8") + err2.decode("utf-8") + err1.decode("utf-8")
+        if len(errors) != 0:
             self.error(
                 "Restoration of database not completed:\n"
-                "-----------------\n"
-                + err3.decode("utf-8")
-                + err2.decode("utf-8")
-                + err1.decode("utf-8")
-                + "-----------------\n"
+                f"-----------------\n {errors} -----------------\n"
             )
             self.unlock_backups("DB")
         else:
-            self.success("Restoration of database completed.")
+            self.success(
+                "Restoration of database completed. " + self.get_datetime_now()
+            )
 
     def unlock_backups(self, repo_name):
         p1 = subprocess.Popen(  # nosec
             [
                 "restic",
                 "unlock",
             ],
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
         )
         (output, err) = p1.communicate()
         if len(err.decode("utf-8")) == 0:
-            self.success(f"Backups are successfully unlocked for {repo_name}.")
+            self.success(f"Backups are unlocked for {repo_name}.")
         else:
             self.error(
                 f"Backups have not been unlocked for {repo_name}:\n"
                 + err.decode("utf-8")
             )
 
     def list_snapshots(self):
@@ -354,29 +490,44 @@
                 "snapshots",
             ],
         )
         p1.communicate()
 
         self.info("Time is UTC.")
 
-    def get_backup_documents(self, backup_id, deal):
+    def get_backup_documents(self, backup_id, deal, files_path: str):
+        self.info(f"Requested: {os.environ['RESTIC_REPOSITORY']}")
+        self.info("Files restoration in progress... " + self.get_datetime_now())
+
         if deal is None:
-            arguments = ["restic", "restore", backup_id, "--target", "/tmp/restic"]
+            arguments = [
+                "restic",
+                "restore",
+                backup_id,
+                "--target",
+                "/tmp/restic",
+            ]
         else:
             arguments = [
                 "restic",
                 "restore",
                 backup_id,
                 "--target",
                 "/tmp/restic",
                 "--include",
                 deal,
             ]
         p = subprocess.Popen(arguments)  # nosec
         (output, err) = p.communicate()
         p.wait()
         location = Path("/tmp/restic")
-        documents_path = next(iter(location.rglob("**/documents/")))
+        documents_path = next(iter(location.rglob(f"**/{files_path}/")))
         copy_tree(
             documents_path,
-            "documents/",
+            files_path + "/",
         )
+
+        self.success("Restoration of documents completed. " + self.get_datetime_now())
+
+    @staticmethod
+    def get_datetime_now() -> str:
+        return datetime.now(timezone.utc).strftime("%Y-%d-%m %H:%M:%S") + " (UTC)"
```

### Comparing `django_restic_backup-0.3.0/PKG-INFO` & `django_restic_backup-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-restic-backup
-Version: 0.3.0
+Version: 0.4.0
 Summary: Restore files or/and database backup from an environment (backup server) with encrypted secret file after decrypting it (secret file is defined in settings.BACKUP_CONF_FILE
 Author: Dedomainia
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

