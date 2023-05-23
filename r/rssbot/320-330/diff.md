# Comparing `tmp/rssbot-320.tar.gz` & `tmp/rssbot-330.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rssbot-320.tar", last modified: Tue May  9 04:32:40 2023, max compression
+gzip compressed data, was "rssbot-330.tar", last modified: Tue May 23 04:36:47 2023, max compression
```

## Comparing `rssbot-320.tar` & `rssbot-330.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-05-09 04:32:40.166341 rssbot-320/
--rw-r--r--   0 bart      (1000) bart      (1001)     3267 2023-05-09 04:32:40.166341 rssbot-320/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1001)     1798 2023-05-08 05:08:41.000000 rssbot-320/README.rst
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-05-09 04:32:40.166341 rssbot-320/bin/
--rwxr-xr-x   0 bart      (1000) bart      (1001)     3174 2023-05-08 18:19:43.000000 rssbot-320/bin/rssbot
--rwxr-xr-x   0 bart      (1000) bart      (1001)     1648 2023-05-08 20:27:09.000000 rssbot-320/bin/rssbotcmd
--rwxr-xr-x   0 bart      (1000) bart      (1001)      244 2023-05-08 18:26:12.000000 rssbot-320/bin/rssbotctl
--rwxr-xr-x   0 bart      (1000) bart      (1001)     1599 2023-05-09 04:26:44.000000 rssbot-320/bin/rssbotd
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-05-09 04:32:40.166341 rssbot-320/files/
--rw-r--r--   0 bart      (1000) bart      (1001)      317 2023-05-08 05:08:41.000000 rssbot-320/files/rssbot.service
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-05-09 04:32:40.166341 rssbot-320/rssbot/
--rw-r--r--   0 bart      (1000) bart      (1001)      799 2023-05-08 18:20:05.000000 rssbot-320/rssbot/classes.py
--rw-r--r--   0 bart      (1000) bart      (1001)      625 2023-05-09 04:16:38.000000 rssbot-320/rssbot/clients.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1166 2023-05-08 18:20:23.000000 rssbot-320/rssbot/clocked.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1076 2023-05-09 04:19:59.000000 rssbot-320/rssbot/command.py
--rw-r--r--   0 bart      (1000) bart      (1001)      761 2023-05-08 18:20:43.000000 rssbot-320/rssbot/decoder.py
--rw-r--r--   0 bart      (1000) bart      (1001)      527 2023-05-08 18:20:51.000000 rssbot-320/rssbot/default.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1151 2023-05-08 18:20:59.000000 rssbot-320/rssbot/encoder.py
--rw-r--r--   0 bart      (1000) bart      (1001)      579 2023-05-08 18:21:08.000000 rssbot-320/rssbot/errored.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1853 2023-05-09 04:15:17.000000 rssbot-320/rssbot/handler.py
--rw-r--r--   0 bart      (1000) bart      (1001)      981 2023-05-08 18:21:28.000000 rssbot-320/rssbot/listens.py
--rw-r--r--   0 bart      (1000) bart      (1001)     2008 2023-05-08 18:21:36.000000 rssbot-320/rssbot/loggers.py
--rw-r--r--   0 bart      (1000) bart      (1001)     2308 2023-05-09 04:16:01.000000 rssbot-320/rssbot/message.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-05-09 04:32:40.166341 rssbot-320/rssbot/modules/
--rw-r--r--   0 bart      (1000) bart      (1001)      306 2023-05-08 18:21:52.000000 rssbot-320/rssbot/modules/cmd.py
--rw-r--r--   0 bart      (1000) bart      (1001)    20605 2023-05-08 18:24:06.000000 rssbot-320/rssbot/modules/irc.py
--rw-r--r--   0 bart      (1000) bart      (1001)     7959 2023-05-08 18:22:05.000000 rssbot-320/rssbot/modules/rss.py
--rw-r--r--   0 bart      (1000) bart      (1001)     3569 2023-05-08 18:32:28.000000 rssbot-320/rssbot/objects.py
--rw-r--r--   0 bart      (1000) bart      (1001)     4362 2023-05-08 18:22:22.000000 rssbot-320/rssbot/persist.py
--rw-r--r--   0 bart      (1000) bart      (1001)      384 2023-05-08 18:22:31.000000 rssbot-320/rssbot/repeats.py
--rw-r--r--   0 bart      (1000) bart      (1001)      436 2023-05-08 18:22:38.000000 rssbot-320/rssbot/runtime.py
--rw-r--r--   0 bart      (1000) bart      (1001)     2195 2023-05-09 04:15:38.000000 rssbot-320/rssbot/scanner.py
--rw-r--r--   0 bart      (1000) bart      (1001)      300 2023-05-08 18:35:03.000000 rssbot-320/rssbot/skipper.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1965 2023-05-08 18:30:37.000000 rssbot-320/rssbot/threads.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1249 2023-05-08 18:23:18.000000 rssbot-320/rssbot/utility.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-05-09 04:32:40.166341 rssbot-320/rssbot.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1001)     3267 2023-05-09 04:32:40.000000 rssbot-320/rssbot.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1001)      662 2023-05-09 04:32:40.000000 rssbot-320/rssbot.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1001)        1 2023-05-09 04:32:40.000000 rssbot-320/rssbot.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1001)        7 2023-05-09 04:32:40.000000 rssbot-320/rssbot.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1001)        1 2023-05-09 04:32:40.000000 rssbot-320/rssbot.egg-info/zip-safe
--rw-r--r--   0 bart      (1000) bart      (1001)       38 2023-05-09 04:32:40.166341 rssbot-320/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1001)     1081 2023-05-09 04:31:41.000000 rssbot-320/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-23 04:36:47.911666 rssbot-330/
+-rw-r--r--   0 bart      (1000) bart      (1000)     3268 2023-05-23 04:36:47.911666 rssbot-330/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)     1799 2023-05-23 03:36:09.000000 rssbot-330/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-23 04:36:47.907666 rssbot-330/bin/
+-rwxr-xr-x   0 bart      (1000) bart      (1000)     2503 2023-05-23 04:33:42.000000 rssbot-330/bin/rssbot
+-rwxr-xr-x   0 bart      (1000) bart      (1000)     1564 2023-05-23 04:17:10.000000 rssbot-330/bin/rssbotcmd
+-rwxr-xr-x   0 bart      (1000) bart      (1000)      244 2023-05-23 03:11:07.000000 rssbot-330/bin/rssbotctl
+-rwxr-xr-x   0 bart      (1000) bart      (1000)     1543 2023-05-23 04:13:56.000000 rssbot-330/bin/rssbotd
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-23 04:36:47.907666 rssbot-330/files/
+-rw-r--r--   0 bart      (1000) bart      (1000)      317 2023-05-23 03:11:07.000000 rssbot-330/files/rssbot.service
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-23 04:36:47.911666 rssbot-330/rssbot/
+-rw-r--r--   0 bart      (1000) bart      (1000)     2116 2023-05-23 03:55:38.000000 rssbot-330/rssbot/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      801 2023-05-23 03:52:41.000000 rssbot-330/rssbot/classes.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      621 2023-05-23 03:52:41.000000 rssbot-330/rssbot/clients.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1168 2023-05-23 03:52:41.000000 rssbot-330/rssbot/clocked.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1072 2023-05-23 03:52:41.000000 rssbot-330/rssbot/command.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      763 2023-05-23 03:52:41.000000 rssbot-330/rssbot/decoder.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      529 2023-05-23 03:52:41.000000 rssbot-330/rssbot/default.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1153 2023-05-23 03:52:41.000000 rssbot-330/rssbot/encoder.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      581 2023-05-23 03:52:41.000000 rssbot-330/rssbot/errored.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1843 2023-05-23 03:52:41.000000 rssbot-330/rssbot/handler.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      983 2023-05-23 03:52:41.000000 rssbot-330/rssbot/listens.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      525 2023-05-23 03:52:41.000000 rssbot-330/rssbot/loggers.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2304 2023-05-23 03:52:41.000000 rssbot-330/rssbot/message.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-23 04:36:47.911666 rssbot-330/rssbot/modules/
+-rw-r--r--   0 bart      (1000) bart      (1000)      141 2023-05-23 04:01:30.000000 rssbot-330/rssbot/modules/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      301 2023-05-23 03:42:32.000000 rssbot-330/rssbot/modules/cmd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    20524 2023-05-23 04:29:24.000000 rssbot-330/rssbot/modules/irc.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     7903 2023-05-23 04:33:59.000000 rssbot-330/rssbot/modules/rss.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     3565 2023-05-23 03:52:41.000000 rssbot-330/rssbot/objects.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     4335 2023-05-23 03:52:41.000000 rssbot-330/rssbot/persist.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      386 2023-05-23 03:52:41.000000 rssbot-330/rssbot/repeats.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      296 2023-05-23 03:52:41.000000 rssbot-330/rssbot/skipper.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1961 2023-05-23 03:52:41.000000 rssbot-330/rssbot/threads.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1251 2023-05-23 03:52:41.000000 rssbot-330/rssbot/utility.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-05-23 04:36:47.911666 rssbot-330/rssbot.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1000)     3268 2023-05-23 04:36:47.000000 rssbot-330/rssbot.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)      672 2023-05-23 04:36:47.000000 rssbot-330/rssbot.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2023-05-23 04:36:47.000000 rssbot-330/rssbot.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        7 2023-05-23 04:36:47.000000 rssbot-330/rssbot.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2023-05-23 04:36:47.000000 rssbot-330/rssbot.egg-info/zip-safe
+-rw-r--r--   0 bart      (1000) bart      (1000)       38 2023-05-23 04:36:47.911666 rssbot-330/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1000)     1094 2023-05-23 03:39:32.000000 rssbot-330/setup.py
```

### Comparing `rssbot-320/PKG-INFO` & `rssbot-330/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rssbot
-Version: 320
+Version: 330
 Summary: feeding rss into your channel
 Home-page: http://github.com/thatebhj/rssbot
 Author: Bart Thate
 Author-email: thatebhj@gmail.com
 License: Public Domain
 Description: README
         ######
@@ -110,23 +110,23 @@
         
         |
         
         **AUTHOR**
         
         |
         
-        Bart Thate - thatebhj@gmail.com
+        B.H.J. Thate - thatebhj@gmail.com
         
         |
         
         **COPYRIGHT**
         
         |
         
-        ``rssbot`` is placed in the Public Domain.
+        ``rssbot`` is placed in the Public Domain
         
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: Public Domain
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `rssbot-320/README.rst` & `rssbot-330/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -102,16 +102,16 @@
 
 |
 
 **AUTHOR**
 
 |
 
-Bart Thate - thatebhj@gmail.com
+B.H.J. Thate - thatebhj@gmail.com
 
 |
 
 **COPYRIGHT**
 
 |
 
-``rssbot`` is placed in the Public Domain.
+``rssbot`` is placed in the Public Domain
```

### Comparing `rssbot-320/bin/rssbotcmd` & `rssbot-330/bin/rssbotcmd`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 # This file is placed in the Public Domain.
-# pylint: disable=C,I,R,E0611,E0402
+# pylint: disable=C,I,R,E0611,E0401,E0402
 
 
 __author__ = "B.H.J. Thate <thatebhj@gmail.com>"
 __version__ = 1
 
 
 import os
@@ -18,56 +18,53 @@
 
 from rssbot.clients import Client
 from rssbot.command import command, scan
 from rssbot.errored import Errors
 from rssbot.loggers import Logging
 from rssbot.message import parse
 from rssbot.modules import cmd, irc, rss
-from rssbot.objects import update
 from rssbot.persist import Persist
-from rssbot.runtime import Cfg
 
 
 scan(cmd)
 scan(irc)
 scan(rss)
 
 
 Persist.workdir = "/var/lib/rssbot/"
 
 
 def cprint(txt):
-    if "v" in Cfg.opts:
-        print(txt)
-        sys.stdout.flush()
+    print(txt)
+    sys.stdout.flush()
 
 
 class CLI(Client):
 
     def announce(self, txt):
         pass
 
     def raw(self, txt):
         print(txt)
         sys.stdout.flush()
 
 
 def main():
     cfg = parse(' '.join(sys.argv[1:]))
-    update(Cfg, cfg)
-    Logging.raw = cprint
+    if "v" in cfg.opts:
+        Logging.verbose = True
+        Logging.raw = cprint
     cli = CLI()
-    command(cli, Cfg.otxt)
+    command(cli, cfg.otxt)
 
 
 def waiter():
     got = []
     for ex in Errors.errors:
-        if not Cfg.silent:
-            traceback.print_exception(type(ex), ex, ex.__traceback__)
+        traceback.print_exception(type(ex), ex, ex.__traceback__)
         got.append(ex)
     for exc in got:
         Errors.errors.remove(exc)
 
 
 def wrap(func):
     fds = sys.stdin.fileno()
```

### Comparing `rssbot-320/bin/rssbotd` & `rssbot-330/bin/rssbotd`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 # This file is placed in the Public Domain.
-# pylint: disable=C,I,R,E0611,E0402,W0212
+# pylint: disable=C,I,R,E0611,E0401,E0402,W0212
 
 
 __author__ = "B.H.J. Thate <thatebhj@gmail.com>"
 __version__ = 1
 
 
 import getpass
@@ -17,15 +17,14 @@
 
 sys.path.insert(0, os.getcwd())
 
 
 from rssbot.errored import Errors
 from rssbot.modules import irc, rss
 from rssbot.persist import Persist
-from rssbot.runtime import Cfg
 
 
 Persist.workdir = "/var/lib/rssbot/"
 
 
 def daemon():
     pid = os.fork()
@@ -66,16 +65,15 @@
     os.setuid(pwnam.pw_uid)
     return username
 
 
 def waiter():
     got = []
     for ex in Errors.errors:
-        if not Cfg.silent:
-            traceback.print_exception(type(ex), ex, ex.__traceback__)
+        traceback.print_exception(type(ex), ex, ex.__traceback__)
         got.append(ex)
     for exc in got:
         Errors.errors.remove(exc)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `rssbot-320/rssbot/classes.py` & `rssbot-330/rssbot/classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This file is placed in the Public Domain.
-# pylint: disable=C,I,R,E0402
+# pylint: disable=C,I,R,W,E0402
 
 
 __author__ = "B.H.J. Thate <thatebhj@gmail.com>"
 __version__ = 1
 
 
 from .default import Default
```

### Comparing `rssbot-320/rssbot/clients.py` & `rssbot-330/rssbot/clients.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This file is placed in the Public Domain.
-# pylint: disable=C,I,R,E0402,W0613
+# pylint: disable=C,I,R,W,E0402
 
 
 __author__ = "B.H.J. Thate <thatebhj@gmail.com>"
 __version__ = 1
 
 
 from .command import Command
```

### Comparing `rssbot-320/rssbot/clocked.py` & `rssbot-330/rssbot/clocked.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This file is placed in the Public Domain.
-# pylint: disable=C,I,R,E0402
+# pylint: disable=C,I,R,W,E0402
 
 
 __author__ = "B.H.J. Thate <thatebhj@gmail.com>"
 __version__ = 1
 
 
 import threading
```

### Comparing `rssbot-320/rssbot/command.py` & `rssbot-330/rssbot/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This file is placed in the Public Domain.
-# pylint: disable=C,I,R,E0402,W0703
+# pylint: disable=C,I,R,W,E0402
 
 
 __author__ = "B.H.J. Thate <thatebhj@gmail.com>"
 __version__ = 1
 
 
 import inspect
```

### Comparing `rssbot-320/rssbot/decoder.py` & `rssbot-330/rssbot/decoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This file is placed in the Public Domain.
-# pylint: disable=C,I,R,E0402
+# pylint: disable=C,I,R,W,E0402
 
 
 __author__ = "B.H.J. Thate <thatebhj@gmail.com>"
 __version__ = 1
 
 
 import json
```

### Comparing `rssbot-320/rssbot/default.py` & `rssbot-330/rssbot/default.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This file is placed in the Public Domain.
-# pylint: disable=C,I,R,E0402
+# pylint: disable=C,I,R,W,E0402
 
 
 __author__ = "B.H.J. Thate <thatebhj@gmail.com>"
 __version__ = 1
 
 
 from .objects import Object
```

### Comparing `rssbot-320/rssbot/encoder.py` & `rssbot-330/rssbot/encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This file is placed in the Public Domain.
-# pylint: disable=C,I,R,E0402
+# pylint: disable=C,I,R,W,E0402
 
 
 __author__ = "B.H.J. Thate <thatebhj@gmail.com>"
 __version__ = 1
 
 
 import json
```

### Comparing `rssbot-320/rssbot/errored.py` & `rssbot-330/rssbot/errored.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This file is placed in the Public Domain.
-# pylint: disable=C,I,R,E0402
+# pylint: disable=C,I,R,W,E0402
 
 
 __author__ = "B.H.J. Thate <thatebhj@gmail.com>"
 __version__ = 1
 
 
 from .objects import  Object
```

### Comparing `rssbot-320/rssbot/handler.py` & `rssbot-330/rssbot/handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This file is placed in the Public Domain.
-# pylint: disable=C,I,R,E0402,W0212,W0703
+# pylint: disable=C,I,R,W,E0402
 
 
 __author__ = "B.H.J. Thate <thatebhj@gmail.com>"
 __version__ = 1
 
 
 import queue
```

### Comparing `rssbot-320/rssbot/listens.py` & `rssbot-330/rssbot/listens.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This file is placed in the Public Domain.
-# pylint: disable=C,I,R,E0402
+# pylint: disable=C,I,R,W,E0402
 
 
 __author__ = "B.H.J. Thate <thatebhj@gmail.com>"
 __version__ = 1
 
 
 from .objects import Object
```

### Comparing `rssbot-320/rssbot/message.py` & `rssbot-330/rssbot/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This file is placed in the Public Domain.
-# pylint: disable=C,I,R,E0402,W0201
+# pylint: disable=C,I,R,W,E0402
 
 
 __author__ = "B.H.J. Thate <thatebhj@gmail.com>"
 __version__ = 1
 
 
 import threading
```

### Comparing `rssbot-320/rssbot/modules/irc.py` & `rssbot-330/rssbot/modules/irc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,78 +1,78 @@
 # This file is placed in the Public Domain.
-# pylint: disable=C,I,R,E0402,E1101,W0613
+# pylint: disable=C,I,R,W,E0401,E0402,E1101
 
 
 """internet relay chat
 
 IRC
 
 ::
 
- $ rssbot cfg server=<server> channel=<channel> nick=<nick>
+ $ operbot cfg server=<server> channel=<channel> nick=<nick>
 
  (*) default channel/server is #opb on localhost
 
 
 SASL
 
 ::
 
- $ rssbot pwd <nickservnick> <nickservpass>
- $ rssbot cfg password=<outputfrompwd>
+ $ operbot pwd <nickservnick> <nickservpass>
+ $ operbot cfg password=<outputfrompwd>
 
 
 USERS
 
 as default the user's userhost is not checked when a user types a command in a
 channel. To enable userhost checking enable users with the ``cfg`` command::
 
- $ rssbot cfg users=True
+ $ operbot cfg users=True
 
 
 To add a user to the bot use the met command::
 
- $ rssbot  met <userhost>
+ $ operbot  met <userhost>
 
 to delete a user use the del command with a substring of the userhost::
 
- $ rssbot del <substring>
+ $ operbot del <substring>
 
 """
 
 __author__ = "B.H.J. Thate <thatebhj@gmail.com>"
 __version__ = 1
 
 
 
 import base64
 import os
 import queue
 import random
 import socket
 import ssl
+import sys
 import time
 import textwrap
 import threading
 import _thread
 
 
-from rssbot.classes import Classes
-from rssbot.clients import Client
-from rssbot.command import Command
-from rssbot.default import Default
-from rssbot.errored import Errors
-from rssbot.message import Message
-from rssbot.listens import Listens
-from rssbot.loggers import Logging
-from rssbot.objects import Object, copy, edit, keys, prt, update
-from rssbot.persist import find, fntime, last, write
-from rssbot.runtime import Cfg
-from rssbot.threads import launch
-from rssbot.utility import elapsed
+from ..classes import Classes
+from ..clients import Client
+from ..command import Command
+from ..default import Default
+from ..errored import Errors
+from ..message import Message
+from ..listens import Listens
+from ..loggers import Logging
+from ..objects import Object, copy, edit, keys, prt, update
+from ..persist import find, fntime, last, write
+from ..threads import launch
+from ..utility import elapsed
 
 
 def __dir__():
     return (
             'Config',
             'IRC',
             'NoUser',
@@ -83,43 +83,44 @@
             'met'
             'mre',
             'pwd',
             'start'
            )
 
 
+NAME = "rssbot"
 saylock = _thread.allocate_lock()
 
 
 def start():
     irc = IRC()
     irc.start()
-    if "v" in Cfg.opts:
+    if "v" in irc.cfg.opts:
         Logging.debug(prt(
                           irc.cfg,
                           ",".join(keys(irc.cfg)),
                           skip='control,password,realname,sleep,username')
                          )
         irc.joined.wait()
     return irc
 
 
 class Config(Default):
 
-    channel = '#%s' % Cfg.name
+    channel = '#%s' % NAME
     control = '!'
-    nick = Cfg.name
+    nick = NAME
     password = ''
     port = 6667
-    realname = Cfg.name
+    realname = NAME
     sasl = False
     server = 'localhost'
     servermodes = ''
     sleep = 60
-    username = Cfg.name
+    username = NAME
     users = False
 
     def __init__(self):
         Default.__init__(self)
         self.control = Config.control
         self.channel = Config.channel
         self.nick = Config.nick
@@ -416,18 +417,18 @@
                 break
 
     def logon(self, server, nck):
         self.connected.wait()
         self.authed.wait()
         self.direct('NICK %s' % nck)
         self.direct(
-                 'USER %s %s %s :%s' % (self.cfg.username or Cfg.name,
+                 'USER %s %s %s :%s' % (self.cfg.username or NAME,
                  server,
                  server,
-                 self.cfg.realname or Cfg.name)
+                 self.cfg.realname or NAME)
                 )
 
     def kill(self, event):
         pass
 
     def log(self, event):
         pass
@@ -553,15 +554,15 @@
             except (
                     ssl.SSLError,
                     ssl.SSLZeroReturnError,
                     ConnectionResetError,
                     BrokenPipeError
                    ) as ex:
                 Errors.errors.append(ex)
-                #self.stop()
+                self.stop()
                 return
         self.state.last = time.time()
         self.state.nrsend += 1
 
     def reconnect(self):
         try:
             self.disconnect()
@@ -595,15 +596,15 @@
         self.connected.clear()
         self.joined.clear()
         launch(Client.start, self)
         launch(Output.start, self)
         launch(
                self.doconnect,
                self.cfg.server or "localhost",
-               self.cfg.nick or Cfg.name,
+               self.cfg.nick or NAME,
                int(self.cfg.port or '6667')
               )
         if not self.keeprunning:
             launch(self.keep)
 
     def stop(self):
         Logging.debug("stopping")
```

### Comparing `rssbot-320/rssbot/modules/rss.py` & `rssbot-330/rssbot/modules/rss.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,22 +15,21 @@
 
 
 from urllib.error import HTTPError, URLError
 from urllib.parse import quote_plus, urlencode
 from urllib.request import Request, urlopen
 
 
-from rssbot.classes import Classes
-from rssbot.listens import Listens
-from rssbot.objects import Object, prt, update
-from rssbot.persist import find, fntime, last, write
-from rssbot.repeats import Repeater
-from rssbot.runtime import Cfg
-from rssbot.threads import launch, threaded
-from rssbot.utility import elapsed, spl
+from ..classes import Classes
+from ..listens import Listens
+from ..objects import Object, prt, update
+from ..persist import find, fntime, last, write
+from ..repeats import Repeater
+from ..threads import launch, threaded
+from ..utility import elapsed, spl
 
 
 def __dir__():
     return (
         'Feed',
         'Fetcher',
         'Repeater',
@@ -49,14 +48,17 @@
 def start():
     fetcher = Fetcher()
     fetcher.start()
     return fetcher
 
 
 DEBUG = False
+NAME = "rssbot"
+
+
 fetchlock = _thread.allocate_lock()
 
 
 class Feed(Object):
 
     pass
 
@@ -192,15 +194,15 @@
             for itm in spl(item):
                 setattr(obj, itm, Parser.getitem(line, itm))
             res.append(obj)
         return res
 
 
 def getfeed(url, item):
-    if Cfg.debug:
+    if DEBUG:
         return [Object(), Object()]
     try:
         result = geturl(url)
     except (ValueError, HTTPError, URLError):
         return [Object(), Object()]
     if not result:
         return [Object(), Object()]
@@ -224,15 +226,15 @@
                 return i.groups()
     return []
 
 
 def geturl(url):
     url = urllib.parse.urlunparse(urllib.parse.urlparse(url))
     req = urllib.request.Request(url)
-    req.add_header('User-agent', useragent(Cfg.name.upper()))
+    req.add_header('User-agent', useragent(NAME.upper()))
     with urllib.request.urlopen(req) as response:
         response.data = response.read()
         return response
 
 
 def striphtml(text):
     clean = re.compile('<.*?>')
```

### Comparing `rssbot-320/rssbot/objects.py` & `rssbot-330/rssbot/objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This file is placed in the Public Domain.
-# pylint: disable=C,I,R,E0402,W0613
+# pylint: disable=C,I,R,W,E0402
 
 
 __author__ = "B.H.J. Thate <thatebhj@gmail.com>"
 __version__ = 1
 
 
 import datetime
```

### Comparing `rssbot-320/rssbot/persist.py` & `rssbot-330/rssbot/persist.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Tihs file is placed in the Public Domain.
-# pylint: disable=C,I,R,E0402
+# pylint: disable=C,I,R,W,E0402
 
 
 __author__ = "B.H.J. Thate <thatebhj@gmail.com>"
 __version__ = 1
 
 
 import json
@@ -14,15 +14,14 @@
 
 
 from .classes import Classes
 from .decoder import ObjectDecoder
 from .encoder import ObjectEncoder
 from .errored import NoClassError
 from .objects import Object, kind, search, update
-from .runtime import Cfg
 
 
 def __dir__():
     return (
             'Persist',
             'cdir',
             'last',
@@ -37,15 +36,15 @@
 
 
 disklock = _thread.allocate_lock()
 
 
 class Persist(Object):
 
-    workdir = Cfg.wd
+    workdir = ""
 
     @staticmethod
     def logdir():
         return os.path.join(Persist.workdir, "logs")
 
     @staticmethod
     def storedir():
```

### Comparing `rssbot-320/rssbot/threads.py` & `rssbot-330/rssbot/threads.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This file is placed in the Public Domain.
-# pylint: disable=C,I,R,E0402,W0613
+# pylint: disable=C,I,R,W,E0402
 
 
 __author__ = "B.H.J. Thate <thatebhj@gmail.com>"
 __version__ = 1
 
 
 import queue
```

### Comparing `rssbot-320/rssbot/utility.py` & `rssbot-330/rssbot/utility.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This file is placed in the Public Domain.
-# pylint: disable=C,I,R,E0402
+# pylint: disable=C,I,R,W,E0402
 
 
 __author__ = "B.H.J. Thate <thatebhj@gmail.com>"
 __version__ = 1
 
 
 def __dir__():
```

### Comparing `rssbot-320/rssbot.egg-info/PKG-INFO` & `rssbot-330/rssbot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rssbot
-Version: 320
+Version: 330
 Summary: feeding rss into your channel
 Home-page: http://github.com/thatebhj/rssbot
 Author: Bart Thate
 Author-email: thatebhj@gmail.com
 License: Public Domain
 Description: README
         ######
@@ -110,23 +110,23 @@
         
         |
         
         **AUTHOR**
         
         |
         
-        Bart Thate - thatebhj@gmail.com
+        B.H.J. Thate - thatebhj@gmail.com
         
         |
         
         **COPYRIGHT**
         
         |
         
-        ``rssbot`` is placed in the Public Domain.
+        ``rssbot`` is placed in the Public Domain
         
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: Public Domain
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `rssbot-320/rssbot.egg-info/SOURCES.txt` & `rssbot-330/rssbot.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 README.rst
 setup.py
 bin/rssbot
 bin/rssbotcmd
 bin/rssbotctl
 bin/rssbotd
 files/rssbot.service
+rssbot/__init__.py
 rssbot/classes.py
 rssbot/clients.py
 rssbot/clocked.py
 rssbot/command.py
 rssbot/decoder.py
 rssbot/default.py
 rssbot/encoder.py
@@ -16,20 +17,19 @@
 rssbot/handler.py
 rssbot/listens.py
 rssbot/loggers.py
 rssbot/message.py
 rssbot/objects.py
 rssbot/persist.py
 rssbot/repeats.py
-rssbot/runtime.py
-rssbot/scanner.py
 rssbot/skipper.py
 rssbot/threads.py
 rssbot/utility.py
 rssbot.egg-info/PKG-INFO
 rssbot.egg-info/SOURCES.txt
 rssbot.egg-info/dependency_links.txt
 rssbot.egg-info/top_level.txt
 rssbot.egg-info/zip-safe
+rssbot/modules/__init__.py
 rssbot/modules/cmd.py
 rssbot/modules/irc.py
 rssbot/modules/rss.py
```

### Comparing `rssbot-320/setup.py` & `rssbot-330/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 def read():
     return open("README.rst", "r").read()
 
 
 setup(
     name="rssbot",
-    version="320",
+    version="330",
     author="Bart Thate",
     author_email="thatebhj@gmail.com",
     url="http://github.com/thatebhj/rssbot",
     description="feeding rss into your channel",
     long_description=read(),
     long_description_content_type="text/x-rst",
     license="Public Domain",
@@ -30,15 +30,16 @@
     data_files=[
                 ("rssbot", ["files/rssbot.service",]),
                ],
     scripts=[
              "bin/rssbot",
              "bin/rssbotcmd",
              "bin/rssbotctl",
-             "bin/rssbotd"],
+             "bin/rssbotd"
+            ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "License :: Public Domain",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 3 :: Only",
         "Topic :: Software Development :: Libraries :: Python Modules",
      ],
```

