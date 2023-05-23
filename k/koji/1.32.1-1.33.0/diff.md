# Comparing `tmp/koji-1.32.1.tar.gz` & `tmp/koji-1.33.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "koji-1.32.1.tar", last modified: Tue Apr  4 12:08:20 2023, max compression
+gzip compressed data, was "koji-1.33.0.tar", last modified: Tue May 23 15:24:58 2023, max compression
```

## Comparing `koji-1.32.1.tar` & `koji-1.33.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2023-04-04 12:08:20.181328 koji-1.32.1/
--rw-rw-r--   0 tkopecek  (1000) tkopecek  (1000)      796 2021-05-31 13:08:21.000000 koji-1.32.1/COPYING
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     3063 2023-04-04 12:08:20.181328 koji-1.32.1/PKG-INFO
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     2216 2023-03-13 16:13:03.000000 koji-1.32.1/README.md
-drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2023-04-04 12:08:20.172328 koji-1.32.1/cli/
--rwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)    13338 2023-03-13 16:13:03.000000 koji-1.32.1/cli/koji
-drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2023-04-04 12:08:20.173328 koji-1.32.1/cli/koji_cli/
--rw-rw-r--   0 tkopecek  (1000) tkopecek  (1000)        0 2021-05-31 13:15:50.000000 koji-1.32.1/cli/koji_cli/__init__.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)   342459 2023-04-04 12:07:35.000000 koji-1.32.1/cli/koji_cli/commands.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    32560 2023-04-04 12:07:35.000000 koji-1.32.1/cli/koji_cli/lib.py
-drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2023-04-04 12:08:20.177328 koji-1.32.1/koji/
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)   136713 2023-04-04 12:07:35.000000 koji-1.32.1/koji/__init__.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)       89 2023-04-04 11:29:27.000000 koji-1.32.1/koji/_version.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    14256 2023-03-13 16:13:03.000000 koji-1.32.1/koji/arch.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     2634 2023-03-13 16:13:03.000000 koji-1.32.1/koji/context.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    63517 2023-03-14 12:56:33.000000 koji-1.32.1/koji/daemon.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     7535 2023-03-13 16:13:03.000000 koji-1.32.1/koji/plugin.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    12060 2023-03-13 16:13:03.000000 koji-1.32.1/koji/policy.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     9441 2023-03-14 12:56:33.000000 koji-1.32.1/koji/rpmdiff.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     1154 2023-03-14 12:56:33.000000 koji-1.32.1/koji/server.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    33947 2023-03-14 12:56:33.000000 koji-1.32.1/koji/tasks.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    29936 2023-03-14 12:56:33.000000 koji-1.32.1/koji/util.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     3575 2023-03-14 12:56:33.000000 koji-1.32.1/koji/xmlrpcplus.py
-drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2023-04-04 12:08:20.178328 koji-1.32.1/koji.egg-info/
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     3063 2023-04-04 12:08:19.000000 koji-1.32.1/koji.egg-info/PKG-INFO
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)      656 2023-04-04 12:08:20.000000 koji-1.32.1/koji.egg-info/SOURCES.txt
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)        1 2023-04-04 12:08:19.000000 koji-1.32.1/koji.egg-info/dependency_links.txt
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)       45 2023-04-04 12:08:19.000000 koji-1.32.1/koji.egg-info/requires.txt
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)       31 2023-04-04 12:08:19.000000 koji-1.32.1/koji.egg-info/top_level.txt
-drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2023-04-04 12:08:20.172328 koji-1.32.1/plugins/
-drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2023-04-04 12:08:20.178328 koji-1.32.1/plugins/cli/
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     3165 2023-03-14 12:56:33.000000 koji-1.32.1/plugins/cli/dud.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     3607 2023-03-14 12:56:33.000000 koji-1.32.1/plugins/cli/kiwi.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     4759 2023-03-13 16:13:03.000000 koji-1.32.1/plugins/cli/runroot.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     2631 2023-03-13 16:13:03.000000 koji-1.32.1/plugins/cli/save_failed_tree.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     4972 2023-04-03 13:44:13.000000 koji-1.32.1/plugins/cli/sidetag_cli.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)       38 2023-04-04 12:08:20.181328 koji-1.32.1/setup.cfg
--rwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)     2467 2023-03-21 11:20:32.000000 koji-1.32.1/setup.py
-drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2023-04-04 12:08:20.179328 koji-1.32.1/tests/
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     1467 2023-03-13 16:13:03.000000 koji-1.32.1/tests/test_docs_version.py
--rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    26795 2023-03-14 12:56:33.000000 koji-1.32.1/tests/test_scm.py
-drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2023-04-04 12:08:20.180328 koji-1.32.1/util/
--rwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)    41460 2023-04-04 12:07:35.000000 koji-1.32.1/util/koji-gc
--rwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)    53664 2023-03-14 12:56:33.000000 koji-1.32.1/util/koji-shadow
--rwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)    10290 2023-04-04 12:07:35.000000 koji-1.32.1/util/koji-sweep-db
--rwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)    54773 2023-04-04 12:07:35.000000 koji-1.32.1/util/kojira
+drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2023-05-23 15:24:58.643170 koji-1.33.0/
+-rw-rw-r--   0 tkopecek  (1000) tkopecek  (1000)      796 2021-05-31 13:08:21.000000 koji-1.33.0/COPYING
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     3063 2023-05-23 15:24:58.643170 koji-1.33.0/PKG-INFO
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     2216 2023-03-13 16:13:03.000000 koji-1.33.0/README.md
+drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2023-05-23 15:24:58.634170 koji-1.33.0/cli/
+-rwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)    13338 2023-03-13 16:13:03.000000 koji-1.33.0/cli/koji
+drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2023-05-23 15:24:58.636170 koji-1.33.0/cli/koji_cli/
+-rw-rw-r--   0 tkopecek  (1000) tkopecek  (1000)        0 2021-05-31 13:15:50.000000 koji-1.33.0/cli/koji_cli/__init__.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)   343204 2023-05-23 15:21:00.000000 koji-1.33.0/cli/koji_cli/commands.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    32560 2023-05-23 15:20:44.000000 koji-1.33.0/cli/koji_cli/lib.py
+drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2023-05-23 15:24:58.639170 koji-1.33.0/koji/
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)   137022 2023-05-22 08:03:48.000000 koji-1.33.0/koji/__init__.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)       89 2023-05-23 15:21:07.000000 koji-1.33.0/koji/_version.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    14256 2023-03-13 16:13:03.000000 koji-1.33.0/koji/arch.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     2634 2023-03-13 16:13:03.000000 koji-1.33.0/koji/context.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    63517 2023-05-23 15:20:44.000000 koji-1.33.0/koji/daemon.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     7535 2023-03-13 16:13:03.000000 koji-1.33.0/koji/plugin.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    12060 2023-04-17 07:29:52.000000 koji-1.33.0/koji/policy.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     9441 2023-03-14 12:56:33.000000 koji-1.33.0/koji/rpmdiff.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     1154 2023-03-14 12:56:33.000000 koji-1.33.0/koji/server.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    33947 2023-03-14 12:56:33.000000 koji-1.33.0/koji/tasks.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    30372 2023-05-22 08:03:48.000000 koji-1.33.0/koji/util.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     3575 2023-03-14 12:56:33.000000 koji-1.33.0/koji/xmlrpcplus.py
+drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2023-05-23 15:24:58.640170 koji-1.33.0/koji.egg-info/
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     3063 2023-05-23 15:24:58.000000 koji-1.33.0/koji.egg-info/PKG-INFO
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)      656 2023-05-23 15:24:58.000000 koji-1.33.0/koji.egg-info/SOURCES.txt
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)        1 2023-05-23 15:24:58.000000 koji-1.33.0/koji.egg-info/dependency_links.txt
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)       45 2023-05-23 15:24:58.000000 koji-1.33.0/koji.egg-info/requires.txt
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)       31 2023-05-23 15:24:58.000000 koji-1.33.0/koji.egg-info/top_level.txt
+drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2023-05-23 15:24:58.633170 koji-1.33.0/plugins/
+drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2023-05-23 15:24:58.641170 koji-1.33.0/plugins/cli/
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     3165 2023-03-14 12:56:33.000000 koji-1.33.0/plugins/cli/dud.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     3607 2023-03-14 12:56:33.000000 koji-1.33.0/plugins/cli/kiwi.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     4759 2023-03-13 16:13:03.000000 koji-1.33.0/plugins/cli/runroot.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     2631 2023-03-13 16:13:03.000000 koji-1.33.0/plugins/cli/save_failed_tree.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     4972 2023-05-22 08:03:48.000000 koji-1.33.0/plugins/cli/sidetag_cli.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)       38 2023-05-23 15:24:58.643170 koji-1.33.0/setup.cfg
+-rwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)     2467 2023-03-21 11:20:32.000000 koji-1.33.0/setup.py
+drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2023-05-23 15:24:58.641170 koji-1.33.0/tests/
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)     1467 2023-03-13 16:13:03.000000 koji-1.33.0/tests/test_docs_version.py
+-rw-r--r--   0 tkopecek  (1000) tkopecek  (1000)    26795 2023-03-14 12:56:33.000000 koji-1.33.0/tests/test_scm.py
+drwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)        0 2023-05-23 15:24:58.642170 koji-1.33.0/util/
+-rwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)    41460 2023-05-22 08:03:48.000000 koji-1.33.0/util/koji-gc
+-rwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)    53664 2023-03-14 12:56:33.000000 koji-1.33.0/util/koji-shadow
+-rwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)    10290 2023-05-23 15:20:44.000000 koji-1.33.0/util/koji-sweep-db
+-rwxr-xr-x   0 tkopecek  (1000) tkopecek  (1000)    56166 2023-05-22 08:03:48.000000 koji-1.33.0/util/kojira
```

### Comparing `koji-1.32.1/COPYING` & `koji-1.33.0/COPYING`

 * *Files identical despite different names*

### Comparing `koji-1.32.1/PKG-INFO` & `koji-1.33.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: koji
-Version: 1.32.1
+Version: 1.33.0
 Summary: Koji is a system for building and tracking RPMS. The base package contains shared libraries and the command-line interface.
 Home-page: http://pagure.io/koji/
 Author: Koji developers
 Author-email: koji-devel@lists.fedorahosted.org
 License: LGPLv2 and GPLv2+
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `koji-1.32.1/README.md` & `koji-1.33.0/README.md`

 * *Files identical despite different names*

### Comparing `koji-1.32.1/cli/koji` & `koji-1.33.0/cli/koji`

 * *Files identical despite different names*

### Comparing `koji-1.32.1/cli/koji_cli/commands.py` & `koji-1.33.0/cli/koji_cli/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import absolute_import, division
 
 import ast
+import dateutil.parser
 import fnmatch
 import itertools
 import json
 import logging
 import os
 import pprint
 import random
@@ -2781,36 +2782,55 @@
         print(line)
 
 
 def anon_handle_list_buildroot(goptions, session, args):
     "[info] List the rpms used in or built in a buildroot"
     usage = "usage: %prog list-buildroot [options] <buildroot-id>"
     parser = OptionParser(usage=get_usage_str(usage))
-    parser.add_option("--built", action="store_true", help="Show the built rpms")
+    parser.add_option("--built", action="store_true", help="Show the built rpms and archives")
     parser.add_option("--verbose", "-v", action="store_true", help="Show more information")
     (options, args) = parser.parse_args(args)
     if len(args) != 1:
         parser.error("Incorrect number of arguments")
     ensure_connection(session, goptions)
     buildrootID = int(args[0])
     opts = {}
     if options.built:
         opts['buildrootID'] = buildrootID
     else:
         opts['componentBuildrootID'] = buildrootID
-    data = session.listRPMs(**opts)
+
+    list_rpms = session.listRPMs(**opts)
+    if list_rpms:
+        if options.built:
+            print('Built RPMs:')
+        else:
+            print('Component RPMs:')
 
     fmt = "%(nvr)s.%(arch)s"
-    order = sorted([(fmt % x, x) for x in data])
+    order = sorted([(fmt % x, x) for x in list_rpms])
     for nvra, rinfo in order:
         if options.verbose and rinfo.get('is_update'):
             print("%s [update]" % nvra)
         else:
             print(nvra)
 
+    list_archives = session.listArchives(**opts)
+    if list_archives:
+        if list_rpms:
+            # print empty line between list of RPMs and archives
+            print('')
+        if options.built:
+            print('Built Archives:')
+        else:
+            print('Component Archives:')
+    order = sorted([x['filename'] for x in list_archives])
+    for filename in order:
+        print(filename)
+
 
 def anon_handle_list_untagged(goptions, session, args):
     "[info] List untagged builds"
     usage = "usage: %prog list-untagged [options] [<package>]"
     parser = OptionParser(usage=get_usage_str(usage))
     parser.add_option("--paths", action="store_true", help="Show the file paths")
     parser.add_option("--show-references", action="store_true", help="Show build references")
@@ -3132,32 +3152,22 @@
 
     def yesno(x):
         if x:
             return 'Y'
         else:
             return 'N'
 
-    try:
-        first = session.getLastHostUpdate(hosts[0]['id'], ts=True)
-        opts = {'ts': True}
-    except koji.ParameterError:
-        # Hubs prior to v1.25.0 do not have a "ts" parameter for getLastHostUpdate
-        first = session.getLastHostUpdate(hosts[0]['id'])
-        opts = {}
-
-    # pull in the last update using multicall to speed it up a bit
-    with session.multicall() as m:
-        result = [m.getLastHostUpdate(host['id'], **opts) for host in hosts[1:]]
-    updateList = [first] + [x.result for x in result]
+    if 'update_ts' not in hosts[0]:
+        _get_host_update_oldhub(session, hosts)
 
-    for host, update in zip(hosts, updateList):
-        if update is None:
+    for host in hosts:
+        if host['update_ts'] is None:
             host['update'] = '-'
         else:
-            host['update'] = koji.formatTimeLong(update)
+            host['update'] = koji.formatTimeLong(host['update_ts'])
         host['enabled'] = yesno(host['enabled'])
         host['ready'] = yesno(host['ready'])
         host['arches'] = ','.join(host['arches'].split())
         host['description'] = truncate_string(host['description'])
         host['comment'] = truncate_string(host['comment'])
 
     # pull hosts' channels
@@ -3199,14 +3209,41 @@
         mask += " %(comment)-50s"
     if options.show_channels:
         mask += " %(channels)s"
     for host in hosts:
         print(mask % host)
 
 
+def _get_host_update_oldhub(session, hosts):
+    """Fetch host update times from older hubs"""
+
+    # figure out if hub supports ts parameter
+    try:
+        first = session.getLastHostUpdate(hosts[0]['id'], ts=True)
+        opts = {'ts': True}
+    except koji.ParameterError:
+        # Hubs prior to v1.25.0 do not have a "ts" parameter for getLastHostUpdate
+        first = session.getLastHostUpdate(hosts[0]['id'])
+        opts = {}
+
+    with session.multicall() as m:
+        result = [m.getLastHostUpdate(host['id'], **opts) for host in hosts[1:]]
+
+    updateList = [first] + [x.result for x in result]
+
+    for host, update in zip(hosts, updateList):
+        if 'ts' in opts:
+            host['update_ts'] = update
+        elif update is None:
+            host['update_ts'] = None
+        else:
+            dt = dateutil.parser.parse(update)
+            host['update_ts'] = time.mktime(dt.timetuple())
+
+
 def anon_handle_list_pkgs(goptions, session, args):
     "[info] Print the package listing for tag or for owner"
     usage = "usage: %prog list-pkgs [options]"
     parser = OptionParser(usage=get_usage_str(usage))
     parser.add_option("--owner", help="Specify owner")
     parser.add_option("--tag", help="Specify tag")
     parser.add_option("--package", help="Specify package")
@@ -3639,19 +3676,18 @@
             print("Comment: %s" % comment[0])
             for line in comment[1:]:
                 print("%s%s" % (" " * 9, line))
         else:
             print("Comment:")
         print("Enabled: %s" % (info['enabled'] and 'yes' or 'no'))
         print("Ready: %s" % (info['ready'] and 'yes' or 'no'))
-        try:
-            update = session.getLastHostUpdate(info['id'], ts=True)
-        except koji.ParameterError:
-            # Hubs prior to v1.25.0 do not have a "ts" parameter for getLastHostUpdate
-            update = session.getLastHostUpdate(info['id'])
+
+        if 'update_ts' not in info:
+            _get_host_update_oldhub(session, [info])
+        update = info['update_ts']
         if update is None:
             update = "never"
         else:
             update = koji.formatTimeLong(update)
         print("Last Update: %s" % update)
         print("Channels: %s" % ' '.join([c['name']
                                          for c in session.listChannels(hostID=info['id'])]))
@@ -6000,17 +6036,14 @@
     arches = []
     for arch in args[4:]:
         arches.append(koji.canonArch(arch))
 
     # Upload the KS file to the staging area.
     # If it's a URL, it's kojid's job to go get it when it does the checkout.
     if not task_opts.ksurl:
-        if not task_opts.scratch:
-            # only scratch builds can omit ksurl
-            raise koji.GenericError("Non-scratch builds must provide ksurl")
         ksfile = task_opts.kickstart
         serverdir = unique_path('cli-image')
         session.uploadWrapper(ksfile, serverdir, callback=callback)
         task_opts.kickstart = os.path.join('work', serverdir,
                                            os.path.basename(ksfile))
         print('')
```

### Comparing `koji-1.32.1/cli/koji_cli/lib.py` & `koji-1.33.0/cli/koji_cli/lib.py`

 * *Files identical despite different names*

### Comparing `koji-1.32.1/koji/__init__.py` & `koji-1.33.0/koji/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3099,14 +3099,15 @@
             return MultiCallInProgress
         else:
             handler, headers, request = self._prepCall(name, args, kwargs)
             tries = 0
             self.retries = 0
             max_retries = self.opts.get('max_retries', 30)
             interval = self.opts.get('retry_interval', 20)
+            err = None
             while True:
                 tries += 1
                 self.retries += 1
                 try:
                     return self._sendCall(handler, headers, request)
                 # basically, we want to retry on most errors, with a few exceptions
                 #  - faults (this means the call completed and failed)
@@ -3122,15 +3123,17 @@
                             secs = self.opts.get('offline_retry_interval', interval)
                             self.logger.debug("Server offline. Retrying in %i seconds", secs)
                             time.sleep(secs)
                             # reset try count - this isn't a typical error, this is a running
                             # server correctly reporting an outage
                             tries = 0
                             continue
-                    raise err
+                    # we don't want tracebacks to show the lower details
+                    # `raise err from None` only works for py 3.3+
+                    # so instead, we will raise err after the try
                 except (SystemExit, KeyboardInterrupt):
                     # (depending on the python version, these may or may not be subclasses of
                     # Exception)
                     raise
                 except Exception as e:
                     tb_str = ''.join(traceback.format_exception(*sys.exc_info()))
                     self.new_session()
@@ -3152,14 +3155,17 @@
                     if tries > max_retries:
                         raise
                     # otherwise keep retrying
                     if self.logger.isEnabledFor(logging.DEBUG):
                         self.logger.debug(tb_str)
                     self.logger.info("Try #%s for call %s (%s) failed: %s",
                                      tries, self.callnum, name, e)
+                if err:
+                    # raise the converted fault from above
+                    raise err
                 if tries > 1:
                     # first retry is immediate, after that we honor retry_interval
                     time.sleep(interval)
             # not reached
 
     def multiCall(self, strict=False, batch=None):
         """Execute a prepared multicall
@@ -3367,15 +3373,15 @@
 
         start = time.time()
         # XXX - stick in a config or something
         retries = 3
         fo = open(localfile, "rb")  # specify bufsize?
         totalsize = os.path.getsize(localfile)
         ofs = 0
-        sha256sum = hashlib.sha256sum()
+        sha256sum = hashlib.sha256()
         debug = self.opts.get('debug', False)
         if callback:
             callback(0, totalsize, 0, 0, 0)
         while True:
             lap = time.time()
             contents = fo.read(blocksize)
             sha256sum.update(contents)
```

### Comparing `koji-1.32.1/koji/arch.py` & `koji-1.33.0/koji/arch.py`

 * *Files identical despite different names*

### Comparing `koji-1.32.1/koji/context.py` & `koji-1.33.0/koji/context.py`

 * *Files identical despite different names*

### Comparing `koji-1.32.1/koji/daemon.py` & `koji-1.33.0/koji/daemon.py`

 * *Files identical despite different names*

### Comparing `koji-1.32.1/koji/plugin.py` & `koji-1.33.0/koji/plugin.py`

 * *Files identical despite different names*

### Comparing `koji-1.32.1/koji/policy.py` & `koji-1.33.0/koji/policy.py`

 * *Files identical despite different names*

### Comparing `koji-1.32.1/koji/rpmdiff.py` & `koji-1.33.0/koji/rpmdiff.py`

 * *Files identical despite different names*

### Comparing `koji-1.32.1/koji/server.py` & `koji-1.33.0/koji/server.py`

 * *Files identical despite different names*

### Comparing `koji-1.32.1/koji/tasks.py` & `koji-1.33.0/koji/tasks.py`

 * *Files identical despite different names*

### Comparing `koji-1.32.1/koji/util.py` & `koji-1.33.0/koji/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -453,46 +453,48 @@
         while True:
             try:
                 os.chdir(path)
             except OSError as e:
                 if e.errno in (errno.ENOENT, errno.ESTALE):
                     # likely racing with another rmtree
                     # if the dir doesn't exist, we're done
+                    logger.warning("Directory to remove has disappeared: %s" % path)
                     return
                 raise
             try:
-                _rmtree(dev)
-            except _RetryRmtree:
+                _rmtree(dev, logger)
+            except _RetryRmtree as e:
                 # reset and retry
                 os.chdir(cwd)
+                logger.warning("Retrying rmtree due to %s" % e)
                 continue
             break
     finally:
         os.chdir(cwd)
 
     # a successful _rmtree call should leave us with an empty directory
     try:
         os.rmdir(path)
     except OSError as e:
         if e.errno != errno.ENOENT:
             raise
 
 
-def _rmtree(dev):
+def _rmtree(dev, logger):
     """Remove all contents of CWD"""
     # This implementation avoids forming long paths and recursion. Otherwise
     # we will have errors with very deep directory trees.
     # - to avoid forming long paths we change directory as we go
     # - to avoid recursion we maintain our own stack
     dirstack = []
     # Each entry in dirstack is a list of subdirs for that level
     # As we descend into the tree, we append a new entry to dirstack
     # When we ascend back up after removal, we pop them off
     while True:
-        dirs = _stripcwd(dev)
+        dirs = _stripcwd(dev, logger)
 
         # if cwd has no subdirs, walk back up until we find some
         while not dirs and dirstack:
             try:
                 os.chdir('..')
             except OSError as e:
                 if e.errno in (errno.ENOENT, errno.ESTALE):
@@ -503,19 +505,20 @@
             dirs = dirstack.pop()
 
             # now that we've ascended back up by one, the first dir entry is
             # one we've just cleared, so we should remove it
             empty_dir = dirs.pop()
             try:
                 os.rmdir(empty_dir)
-            except OSError:
+            except OSError as e:
                 # If this happens, either something else is writing to the dir,
                 # or there is a bug in our code.
                 # For now, we ignore this and proceed, but we'll still fail at
                 # the top level rmdir
+                logger.error("Unable to remove directory %s: %s" % (empty_dir, e))
                 pass
 
         if not dirs:
             # we are done
             break
 
         # otherwise we descend into the next subdir
@@ -525,27 +528,29 @@
             os.chdir(subdir)
         except OSError as e:
             if e.errno == errno.ENOENT:
                 # likely in a race with another rmtree
                 # we'll ignore this and continue
                 # since subdir doesn't exist, we'll pop it off and forget about it
                 dirs.pop()
+                logger.warning("Subdir disappeared during rmtree %s: %s" % (subdir, e))
                 continue  # with dirstack unchanged
             raise
         dirstack.append(dirs)
 
 
-def _stripcwd(dev):
+def _stripcwd(dev, logger):
     """Unlink all files in cwd and return list of subdirs"""
     dirs = []
     try:
         fdirs = os.listdir('.')
     except OSError as e:
-        # cwd has been removed by others, just return an empty list
         if e.errno in (errno.ENOENT, errno.ESTALE):
+            # cwd could have been removed by others, just return an empty list
+            logger.warning("Unable to read directory: %s" % e)
             return dirs
         raise
     for fn in fdirs:
         try:
             st = os.lstat(fn)
         except OSError as e:
             if e.errno == errno.ENOENT:
```

### Comparing `koji-1.32.1/koji/xmlrpcplus.py` & `koji-1.33.0/koji/xmlrpcplus.py`

 * *Files identical despite different names*

### Comparing `koji-1.32.1/koji.egg-info/PKG-INFO` & `koji-1.33.0/koji.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: koji
-Version: 1.32.1
+Version: 1.33.0
 Summary: Koji is a system for building and tracking RPMS. The base package contains shared libraries and the command-line interface.
 Home-page: http://pagure.io/koji/
 Author: Koji developers
 Author-email: koji-devel@lists.fedorahosted.org
 License: LGPLv2 and GPLv2+
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `koji-1.32.1/koji.egg-info/SOURCES.txt` & `koji-1.33.0/koji.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `koji-1.32.1/plugins/cli/dud.py` & `koji-1.33.0/plugins/cli/dud.py`

 * *Files identical despite different names*

### Comparing `koji-1.32.1/plugins/cli/kiwi.py` & `koji-1.33.0/plugins/cli/kiwi.py`

 * *Files identical despite different names*

### Comparing `koji-1.32.1/plugins/cli/runroot.py` & `koji-1.33.0/plugins/cli/runroot.py`

 * *Files identical despite different names*

### Comparing `koji-1.32.1/plugins/cli/save_failed_tree.py` & `koji-1.33.0/plugins/cli/save_failed_tree.py`

 * *Files identical despite different names*

### Comparing `koji-1.32.1/plugins/cli/sidetag_cli.py` & `koji-1.33.0/plugins/cli/sidetag_cli.py`

 * *Files identical despite different names*

### Comparing `koji-1.32.1/setup.py` & `koji-1.33.0/setup.py`

 * *Files identical despite different names*

### Comparing `koji-1.32.1/tests/test_docs_version.py` & `koji-1.33.0/tests/test_docs_version.py`

 * *Files identical despite different names*

### Comparing `koji-1.32.1/tests/test_scm.py` & `koji-1.33.0/tests/test_scm.py`

 * *Files identical despite different names*

### Comparing `koji-1.32.1/util/koji-gc` & `koji-1.33.0/util/koji-gc`

 * *Files identical despite different names*

### Comparing `koji-1.32.1/util/koji-shadow` & `koji-1.33.0/util/koji-shadow`

 * *Files identical despite different names*

### Comparing `koji-1.32.1/util/koji-sweep-db` & `koji-1.33.0/util/koji-sweep-db`

 * *Files identical despite different names*

### Comparing `koji-1.32.1/util/kojira` & `koji-1.33.0/util/kojira`

 * *Files 3% similar despite different names*

```diff
@@ -791,22 +791,49 @@
         ts = entry['expire_ts']
         age = time.time() - ts
         # XXX - need to make sure our times aren't far off, otherwise this
         # scoring could have the opposite of the desired effect
         if age < 0:
             self.logger.warning("Needed tag has future expire_ts: %r", entry)
             age = 0
-        entry['score'] = age * adj
+        entry['score'] = age * adj * entry.get('score_adjust', 1)
         self.logger.debug("Needed tag %s got score %.2f",
                           entry['taginfo']['name'], entry['score'])
         # so a day old unused repo gets about the regen same score as a
         # 2.4-hour-old, very popular repo
 
     def updateTagScores(self):
-        for entry in list(self.needed_tags.values()):
+        # call listTasks waitrepo
+        tasks = self.session.listTasks(opts={'method': ['waitrepo'],
+                                             'decode': True,
+                                             'state': [koji.TASK_STATES['FREE'],
+                                                       koji.TASK_STATES['ASSIGNED'],
+                                                       koji.TASK_STATES['OPEN']]})
+        awaited = set()
+        if tasks:
+            logger.debug("Checking %s active waitrepo tasks", len(tasks))
+        for task in tasks:
+            try:
+                tag_param = koji.parse_task_params('waitrepo', task['request'])['tag']
+                taginfo = getTag(self.session, tag_param)
+            except Exception:
+                # ignore malformed tasks
+                self.logger.debug(f"Malformed task: {task}")
+                continue
+            if taginfo:
+                awaited.add(taginfo['id'])
+            else:
+                self.logger.debug("Found waitrepo task %i with bad tag arg: %r",
+                                  task['id'], tag_param)
+
+        for tag_id, entry in self.needed_tags.items():
+            if tag_id in awaited:
+                # score multiplication factor, prioritize tags which are being awaited for
+                # not needed on every setTagScore call (initial point will not account it for)
+                entry['score_adjust'] = 2
             self.setTagScore(entry)
 
     def _delete_needed_tag(self, tag_id):
         try:
             del self.needed_tags[tag_id]
         except KeyError:
             pass
```

