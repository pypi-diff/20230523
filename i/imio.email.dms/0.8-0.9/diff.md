# Comparing `tmp/imio.email.dms-0.8.tar.gz` & `tmp/imio.email.dms-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imio.email.dms-0.8.tar", last modified: Mon Jan 24 14:01:20 2022, max compression
+gzip compressed data, was "imio.email.dms-0.9.tar", last modified: Thu Feb 17 13:15:49 2022, max compression
```

## Comparing `imio.email.dms-0.8.tar` & `imio.email.dms-0.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-01-24 14:01:20.703875 imio.email.dms-0.8/
--rw-rw-r--   0 sge       (1000) sge       (1000)     1199 2022-01-24 14:01:20.000000 imio.email.dms-0.8/CHANGES.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)      148 2022-01-24 14:01:20.000000 imio.email.dms-0.8/CONTRIBUTORS.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)      244 2022-01-24 14:01:20.000000 imio.email.dms-0.8/DEVELOP.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)      653 2022-01-24 14:01:20.000000 imio.email.dms-0.8/Dockerfile
--rw-rw-r--   0 sge       (1000) sge       (1000)     2988 2022-01-24 14:01:20.000000 imio.email.dms-0.8/Jenkinsfile
--rw-rw-r--   0 sge       (1000) sge       (1000)    18092 2022-01-24 14:01:20.000000 imio.email.dms-0.8/LICENSE.GPL
--rw-rw-r--   0 sge       (1000) sge       (1000)      660 2022-01-24 14:01:20.000000 imio.email.dms-0.8/LICENSE.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)      240 2022-01-24 14:01:20.000000 imio.email.dms-0.8/MANIFEST.in
--rw-rw-r--   0 sge       (1000) sge       (1000)      429 2022-01-24 14:01:20.000000 imio.email.dms-0.8/Makefile
--rw-rw-r--   0 sge       (1000) sge       (1000)     4331 2022-01-24 14:01:20.703875 imio.email.dms-0.8/PKG-INFO
--rw-rw-r--   0 sge       (1000) sge       (1000)     1326 2022-01-24 14:01:20.000000 imio.email.dms-0.8/README.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)      986 2022-01-24 14:01:20.000000 imio.email.dms-0.8/buildout.cfg
--rw-rw-r--   0 sge       (1000) sge       (1000)      407 2022-01-24 14:01:20.000000 imio.email.dms-0.8/config.ini
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-01-24 14:01:20.703875 imio.email.dms-0.8/docs/
--rw-rw-r--   0 sge       (1000) sge       (1000)       65 2022-01-24 14:01:20.000000 imio.email.dms-0.8/docs/index.rst
--rwxrwxr-x   0 sge       (1000) sge       (1000)      146 2022-01-24 14:01:20.000000 imio.email.dms-0.8/entrypoint.sh
--rw-rw-r--   0 sge       (1000) sge       (1000)       39 2022-01-24 14:01:20.000000 imio.email.dms-0.8/requirements.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)       38 2022-01-24 14:01:20.703875 imio.email.dms-0.8/setup.cfg
--rw-rw-r--   0 sge       (1000) sge       (1000)     1593 2022-01-24 14:01:20.000000 imio.email.dms-0.8/setup.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      367 2022-01-24 14:01:20.000000 imio.email.dms-0.8/sources.cfg
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-01-24 14:01:20.703875 imio.email.dms-0.8/src/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-01-24 14:01:20.703875 imio.email.dms-0.8/src/imio/
--rw-rw-r--   0 sge       (1000) sge       (1000)       80 2022-01-24 14:01:20.000000 imio.email.dms-0.8/src/imio/__init__.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-01-24 14:01:20.703875 imio.email.dms-0.8/src/imio/email/
--rw-rw-r--   0 sge       (1000) sge       (1000)       80 2022-01-24 14:01:20.000000 imio.email.dms-0.8/src/imio/email/__init__.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-01-24 14:01:20.703875 imio.email.dms-0.8/src/imio/email/dms/
--rw-rw-r--   0 sge       (1000) sge       (1000)       24 2022-01-24 14:01:20.000000 imio.email.dms-0.8/src/imio/email/dms/__init__.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     6457 2022-01-24 14:01:20.000000 imio.email.dms-0.8/src/imio/email/dms/imap.py
--rw-rw-r--   0 sge       (1000) sge       (1000)    20280 2022-01-24 14:01:20.000000 imio.email.dms-0.8/src/imio/email/dms/main.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      561 2022-01-24 14:01:20.000000 imio.email.dms-0.8/src/imio/email/dms/utils.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-01-24 14:01:20.703875 imio.email.dms-0.8/src/imio.email.dms.egg-info/
--rw-rw-r--   0 sge       (1000) sge       (1000)     4331 2022-01-24 14:01:20.000000 imio.email.dms-0.8/src/imio.email.dms.egg-info/PKG-INFO
--rw-rw-r--   0 sge       (1000) sge       (1000)      730 2022-01-24 14:01:20.000000 imio.email.dms-0.8/src/imio.email.dms.egg-info/SOURCES.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)        1 2022-01-24 14:01:20.000000 imio.email.dms-0.8/src/imio.email.dms.egg-info/dependency_links.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)      131 2022-01-24 14:01:20.000000 imio.email.dms-0.8/src/imio.email.dms.egg-info/entry_points.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)       16 2022-01-24 14:01:20.000000 imio.email.dms-0.8/src/imio.email.dms.egg-info/namespace_packages.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)        1 2022-01-24 14:01:20.000000 imio.email.dms-0.8/src/imio.email.dms.egg-info/not-zip-safe
--rw-rw-r--   0 sge       (1000) sge       (1000)      110 2022-01-24 14:01:20.000000 imio.email.dms-0.8/src/imio.email.dms.egg-info/requires.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)        5 2022-01-24 14:01:20.000000 imio.email.dms-0.8/src/imio.email.dms.egg-info/top_level.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)     1006 2022-01-24 14:01:20.000000 imio.email.dms-0.8/versions.cfg
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-02-17 13:15:49.692164 imio.email.dms-0.9/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1434 2022-02-17 13:15:49.000000 imio.email.dms-0.9/CHANGES.rst
+-rw-rw-r--   0 sge       (1000) sge       (1000)      148 2022-02-17 13:15:49.000000 imio.email.dms-0.9/CONTRIBUTORS.rst
+-rw-rw-r--   0 sge       (1000) sge       (1000)      244 2022-02-17 13:15:49.000000 imio.email.dms-0.9/DEVELOP.rst
+-rw-rw-r--   0 sge       (1000) sge       (1000)      653 2022-02-17 13:15:49.000000 imio.email.dms-0.9/Dockerfile
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2988 2022-02-17 13:15:49.000000 imio.email.dms-0.9/Jenkinsfile
+-rw-rw-r--   0 sge       (1000) sge       (1000)    18092 2022-02-17 13:15:49.000000 imio.email.dms-0.9/LICENSE.GPL
+-rw-rw-r--   0 sge       (1000) sge       (1000)      660 2022-02-17 13:15:49.000000 imio.email.dms-0.9/LICENSE.rst
+-rw-rw-r--   0 sge       (1000) sge       (1000)      240 2022-02-17 13:15:49.000000 imio.email.dms-0.9/MANIFEST.in
+-rw-rw-r--   0 sge       (1000) sge       (1000)      429 2022-02-17 13:15:49.000000 imio.email.dms-0.9/Makefile
+-rw-rw-r--   0 sge       (1000) sge       (1000)     4646 2022-02-17 13:15:49.692164 imio.email.dms-0.9/PKG-INFO
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1326 2022-02-17 13:15:49.000000 imio.email.dms-0.9/README.rst
+-rw-rw-r--   0 sge       (1000) sge       (1000)      986 2022-02-17 13:15:49.000000 imio.email.dms-0.9/buildout.cfg
+-rw-rw-r--   0 sge       (1000) sge       (1000)      407 2022-02-17 13:15:49.000000 imio.email.dms-0.9/config.ini
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-02-17 13:15:49.692164 imio.email.dms-0.9/docs/
+-rw-rw-r--   0 sge       (1000) sge       (1000)       65 2022-02-17 13:15:49.000000 imio.email.dms-0.9/docs/index.rst
+-rwxrwxr-x   0 sge       (1000) sge       (1000)      146 2022-02-17 13:15:49.000000 imio.email.dms-0.9/entrypoint.sh
+-rw-rw-r--   0 sge       (1000) sge       (1000)       39 2022-02-17 13:15:49.000000 imio.email.dms-0.9/requirements.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)       38 2022-02-17 13:15:49.692164 imio.email.dms-0.9/setup.cfg
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1593 2022-02-17 13:15:49.000000 imio.email.dms-0.9/setup.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      367 2022-02-17 13:15:49.000000 imio.email.dms-0.9/sources.cfg
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-02-17 13:15:49.692164 imio.email.dms-0.9/src/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-02-17 13:15:49.692164 imio.email.dms-0.9/src/imio/
+-rw-rw-r--   0 sge       (1000) sge       (1000)       80 2022-02-17 13:15:49.000000 imio.email.dms-0.9/src/imio/__init__.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-02-17 13:15:49.692164 imio.email.dms-0.9/src/imio/email/
+-rw-rw-r--   0 sge       (1000) sge       (1000)       80 2022-02-17 13:15:49.000000 imio.email.dms-0.9/src/imio/email/__init__.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-02-17 13:15:49.692164 imio.email.dms-0.9/src/imio/email/dms/
+-rw-rw-r--   0 sge       (1000) sge       (1000)       24 2022-02-17 13:15:49.000000 imio.email.dms-0.9/src/imio/email/dms/__init__.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     6457 2022-02-17 13:15:49.000000 imio.email.dms-0.9/src/imio/email/dms/imap.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)    20407 2022-02-17 13:15:49.000000 imio.email.dms-0.9/src/imio/email/dms/main.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      561 2022-02-17 13:15:49.000000 imio.email.dms-0.9/src/imio/email/dms/utils.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-02-17 13:15:49.692164 imio.email.dms-0.9/src/imio.email.dms.egg-info/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     4646 2022-02-17 13:15:49.000000 imio.email.dms-0.9/src/imio.email.dms.egg-info/PKG-INFO
+-rw-rw-r--   0 sge       (1000) sge       (1000)      730 2022-02-17 13:15:49.000000 imio.email.dms-0.9/src/imio.email.dms.egg-info/SOURCES.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)        1 2022-02-17 13:15:49.000000 imio.email.dms-0.9/src/imio.email.dms.egg-info/dependency_links.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)      131 2022-02-17 13:15:49.000000 imio.email.dms-0.9/src/imio.email.dms.egg-info/entry_points.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)       16 2022-02-17 13:15:49.000000 imio.email.dms-0.9/src/imio.email.dms.egg-info/namespace_packages.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)        1 2022-02-17 13:15:49.000000 imio.email.dms-0.9/src/imio.email.dms.egg-info/not-zip-safe
+-rw-rw-r--   0 sge       (1000) sge       (1000)      110 2022-02-17 13:15:49.000000 imio.email.dms-0.9/src/imio.email.dms.egg-info/requires.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)        5 2022-02-17 13:15:49.000000 imio.email.dms-0.9/src/imio.email.dms.egg-info/top_level.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1006 2022-02-17 13:15:49.000000 imio.email.dms-0.9/versions.cfg
```

### Comparing `imio.email.dms-0.8/CHANGES.rst` & `imio.email.dms-0.9/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,25 @@
 Changelog
 =========
 
 
+0.9 (2022-02-17)
+----------------
+
+- Removed pattern in sent email for ignored error.
+  [sgeulette]
+- Corrected badly addresses from email.utils.getAddresses (in imio.email.parser)
+  [sgeulette]
+- Upgraded mail-parser
+  [sgeulette]
+
 0.8 (2022-01-24)
 ----------------
 
-- Ignored ignored flaged mails when getting waiting emails.
+- Ignored 'ignored' flaged mails when getting waiting emails.
   [sgeulette]
 
 0.7 (2022-01-21)
 ----------------
 
 - Added transferer check following pattern to avoid anyone can push an email in the app.
   [sgeulette]
```

### Comparing `imio.email.dms-0.8/Dockerfile` & `imio.email.dms-0.9/Dockerfile`

 * *Files identical despite different names*

### Comparing `imio.email.dms-0.8/Jenkinsfile` & `imio.email.dms-0.9/Jenkinsfile`

 * *Files identical despite different names*

### Comparing `imio.email.dms-0.8/LICENSE.GPL` & `imio.email.dms-0.9/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `imio.email.dms-0.8/LICENSE.rst` & `imio.email.dms-0.9/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `imio.email.dms-0.8/PKG-INFO` & `imio.email.dms-0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: imio.email.dms
-Version: 0.8
+Version: 0.9
 Summary: Package to read emails and send them to DMS
 Home-page: https://pypi.python.org/pypi/imio.email.dms
 Author: Laurent Lasudry
 Author-email: info@affinitic.be
 License: GPL version 2
 Description: ==============
         imio.email.dms
@@ -81,18 +81,28 @@
         - Stéphan Geulette, stephan.geulette@imio.be
         
         
         Changelog
         =========
         
         
+        0.9 (2022-02-17)
+        ----------------
+        
+        - Removed pattern in sent email for ignored error.
+          [sgeulette]
+        - Corrected badly addresses from email.utils.getAddresses (in imio.email.parser)
+          [sgeulette]
+        - Upgraded mail-parser
+          [sgeulette]
+        
         0.8 (2022-01-24)
         ----------------
         
-        - Ignored ignored flaged mails when getting waiting emails.
+        - Ignored 'ignored' flaged mails when getting waiting emails.
           [sgeulette]
         
         0.7 (2022-01-21)
         ----------------
         
         - Added transferer check following pattern to avoid anyone can push an email in the app.
           [sgeulette]
```

### Comparing `imio.email.dms-0.8/README.rst` & `imio.email.dms-0.9/README.rst`

 * *Files identical despite different names*

### Comparing `imio.email.dms-0.8/buildout.cfg` & `imio.email.dms-0.9/buildout.cfg`

 * *Files identical despite different names*

### Comparing `imio.email.dms-0.8/setup.py` & `imio.email.dms-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     open('CONTRIBUTORS.rst').read(),
     open('CHANGES.rst').read(),
 ])
 
 
 setup(
     name='imio.email.dms',
-    version='0.8',
+    version='0.9',
     description="Package to read emails and send them to DMS",
     long_description=long_description,
     # Get more from https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Environment :: Web Environment",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
```

### Comparing `imio.email.dms-0.8/src/imio/email/dms/imap.py` & `imio.email.dms-0.9/src/imio/email/dms/imap.py`

 * *Files identical despite different names*

### Comparing `imio.email.dms-0.8/src/imio/email/dms/main.py` & `imio.email.dms-0.9/src/imio/email/dms/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 Bonjour,
 Votre adresse email {3} n'est pas autorisée à transférer un email vers iA.docs.
 Si cette action est justifiée, veuillez prendre contact avec votre référent interne.\n
 Le mail concerné est en pièce jointe.\n
 Client ID : {0}
 IMAP login : {1}
 mail id : {2}
-pattern : "{4}"
+pattern : "caché"
 """
 
 RESULT_MAIL = u"""
 Client ID : {0}
 IMAP login : {1}\n
 {2}\n
 """
@@ -194,16 +194,16 @@
 
     msg = MIMEMultipart()
     msg["Subject"] = "Transfert non autorisé de {} pour le client {}".format(from_, client_id)
     msg["From"] = sender
     msg["To"] = from_
     msg["Bcc"] = recipient
 
-    main_text = MIMEText(IGNORED_MAIL.format(client_id, login, mail_id, from_, config['mailinfos']['sender-pattern']),
-                         "plain")
+#    main_text = MIMEText(IGNORED_MAIL.format(client_id, login, mail_id, from_, config['mailinfos']['sender-pattern']),
+    main_text = MIMEText(IGNORED_MAIL.format(client_id, login, mail_id, from_), "plain")
     msg.attach(main_text)
 
     attachment = MIMEBase("message", "rfc822")
     attachment.set_payload(mail.as_string())
     attachment.add_header("Content-Disposition", "inline")
     msg.attach(attachment)
 
@@ -360,17 +360,19 @@
     elif arguments.get("--list_emails"):
         handler.list_last_emails(nb=int(arguments.get("--list_emails")))
         # import ipdb; ipdb.set_trace()
         # handler.mark_reset_error('58')
         # handler.mark_reset_ignored('77')
         # res, data = handler.connection.search(None, 'SUBJECT "JBC client"')
         # for mail_id in data[0].split():
-        #      mail = handler.get_mail(mail_id)
-        #      mail_infos = MailData(mail_id, mail)
-        #      email = mail_infos.mail
+        #      omail = handler.get_mail(mail_id)
+        #      parser = Parser(omail)
+        #      headers = parser.headers
+        #      amail = parser.message
+        #      parsed = MailParser(omail)
         #     logger.info(email['Subject'])
         handler.disconnect()
         lock.close()
         sys.exit()
     elif arguments.get("--get_eml"):
         mail_id = arguments['--get_eml']
         if not mail_id:
```

### Comparing `imio.email.dms-0.8/src/imio/email/dms/utils.py` & `imio.email.dms-0.9/src/imio/email/dms/utils.py`

 * *Files identical despite different names*

### Comparing `imio.email.dms-0.8/src/imio.email.dms.egg-info/PKG-INFO` & `imio.email.dms-0.9/src/imio.email.dms.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: imio.email.dms
-Version: 0.8
+Version: 0.9
 Summary: Package to read emails and send them to DMS
 Home-page: https://pypi.python.org/pypi/imio.email.dms
 Author: Laurent Lasudry
 Author-email: info@affinitic.be
 License: GPL version 2
 Description: ==============
         imio.email.dms
@@ -81,18 +81,28 @@
         - Stéphan Geulette, stephan.geulette@imio.be
         
         
         Changelog
         =========
         
         
+        0.9 (2022-02-17)
+        ----------------
+        
+        - Removed pattern in sent email for ignored error.
+          [sgeulette]
+        - Corrected badly addresses from email.utils.getAddresses (in imio.email.parser)
+          [sgeulette]
+        - Upgraded mail-parser
+          [sgeulette]
+        
         0.8 (2022-01-24)
         ----------------
         
-        - Ignored ignored flaged mails when getting waiting emails.
+        - Ignored 'ignored' flaged mails when getting waiting emails.
           [sgeulette]
         
         0.7 (2022-01-21)
         ----------------
         
         - Added transferer check following pattern to avoid anyone can push an email in the app.
           [sgeulette]
```

### Comparing `imio.email.dms-0.8/src/imio.email.dms.egg-info/SOURCES.txt` & `imio.email.dms-0.9/src/imio.email.dms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imio.email.dms-0.8/versions.cfg` & `imio.email.dms-0.9/versions.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 zc.lockfile = 2.0
 
 # Required by:
 # imio.email.parser
 beautifulsoup4 = 4.9.3
 html5lib = 1.1
 lxml = 4.6.1
-mail-parser = 3.12.0
+mail-parser = 3.15.0
 pdfminer3k = 1.3.4
 Pillow = 8.0.1
 ply = 3.11
 PyPDF2 = 1.26.0
 python-magic = 0.4.18
 reportlab = 3.5.54
 soupsieve = 2.0.1
```

