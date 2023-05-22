# Comparing `tmp/hcli_core-0.8.0.tar.gz` & `tmp/hcli_core-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcli_core-0.8.0.tar", last modified: Mon Mar 28 02:53:31 2022, max compression
+gzip compressed data, was "hcli_core-0.9.0.tar", last modified: Tue Apr 12 23:15:46 2022, max compression
```

## Comparing `hcli_core-0.8.0.tar` & `hcli_core-0.9.0.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2022-03-28 02:53:31.251089 hcli_core-0.8.0/
--rwxr-x---   0 jeff       (501) staff       (20)     1056 2022-03-20 22:23:05.000000 hcli_core-0.8.0/LICENSE.txt
--rwxr-x---   0 jeff       (501) staff       (20)      280 2022-03-20 22:23:05.000000 hcli_core-0.8.0/MANIFEST.in
--rw-r--r--   0 jeff       (501) staff       (20)     4982 2022-03-28 02:53:31.251183 hcli_core-0.8.0/PKG-INFO
--rwxr-x---   0 jeff       (501) staff       (20)     3459 2022-03-20 22:23:05.000000 hcli_core-0.8.0/README.rst
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2022-03-28 02:53:31.241076 hcli_core-0.8.0/hcli_core/
--rwxr-x---   0 jeff       (501) staff       (20)        0 2022-03-20 22:23:05.000000 hcli_core-0.8.0/hcli_core/__init__.py
--rwxr-x---   0 jeff       (501) staff       (20)     1632 2022-03-20 22:23:05.000000 hcli_core-0.8.0/hcli_core/__main__.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2022-03-28 02:53:31.242331 hcli_core-0.8.0/hcli_core/cli/
--rwxr-x---   0 jeff       (501) staff       (20)        0 2022-03-20 22:23:03.000000 hcli_core-0.8.0/hcli_core/cli/__init__.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2022-03-28 02:53:31.242618 hcli_core-0.8.0/hcli_core/cli/__pycache__/
--rwxr-x---   0 jeff       (501) staff       (20)     1032 2022-03-20 22:23:03.000000 hcli_core-0.8.0/hcli_core/cli/__pycache__/cli.cpython-36.pyc
--rwxr-x---   0 jeff       (501) staff       (20)      794 2022-03-20 22:23:03.000000 hcli_core-0.8.0/hcli_core/cli/cli.py
--rwxr-x---   0 jeff       (501) staff       (20)     1686 2022-03-20 22:23:03.000000 hcli_core-0.8.0/hcli_core/cli/template.json
--rwxr-x---   0 jeff       (501) staff       (20)      786 2022-03-20 22:23:03.000000 hcli_core-0.8.0/hcli_core/config.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2022-03-28 02:53:31.242794 hcli_core-0.8.0/hcli_core/data/
--rwxr-x---   0 jeff       (501) staff       (20)     1535 2022-03-20 22:23:03.000000 hcli_core-0.8.0/hcli_core/data/hcli_core.1
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2022-03-28 02:53:31.243022 hcli_core-0.8.0/hcli_core/haliot/
--rwxr-x---   0 jeff       (501) staff       (20)        0 2022-03-20 22:23:03.000000 hcli_core-0.8.0/hcli_core/haliot/__init__.py
--rwxr-x---   0 jeff       (501) staff       (20)     1842 2022-03-20 22:23:03.000000 hcli_core-0.8.0/hcli_core/haliot/hal.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2022-03-28 02:53:31.245001 hcli_core-0.8.0/hcli_core/hcli/
--rwxr-x---   0 jeff       (501) staff       (20)        0 2022-03-20 22:23:04.000000 hcli_core-0.8.0/hcli_core/hcli/__init__.py
--rwxr-x---   0 jeff       (501) staff       (20)     2278 2022-03-20 22:23:04.000000 hcli_core-0.8.0/hcli_core/hcli/api.py
--rwxr-x---   0 jeff       (501) staff       (20)     1958 2022-03-20 22:23:04.000000 hcli_core-0.8.0/hcli_core/hcli/command.py
--rwxr-x---   0 jeff       (501) staff       (20)     4103 2022-03-20 22:23:04.000000 hcli_core-0.8.0/hcli_core/hcli/document.py
--rwxr-x---   0 jeff       (501) staff       (20)     2085 2022-03-20 22:23:04.000000 hcli_core-0.8.0/hcli_core/hcli/execution.py
--rwxr-x---   0 jeff       (501) staff       (20)     1617 2022-03-20 22:23:04.000000 hcli_core-0.8.0/hcli_core/hcli/finalexecution.py
--rwxr-x---   0 jeff       (501) staff       (20)      894 2022-03-20 22:23:04.000000 hcli_core-0.8.0/hcli_core/hcli/home.py
--rwxr-x---   0 jeff       (501) staff       (20)     1863 2022-03-20 22:23:04.000000 hcli_core-0.8.0/hcli_core/hcli/option.py
--rwxr-x---   0 jeff       (501) staff       (20)     1928 2022-03-20 22:23:04.000000 hcli_core-0.8.0/hcli_core/hcli/parameter.py
--rwxr-x---   0 jeff       (501) staff       (20)      100 2022-03-20 22:23:04.000000 hcli_core-0.8.0/hcli_core/hcli/profile.py
--rwxr-x---   0 jeff       (501) staff       (20)      955 2022-03-20 22:23:04.000000 hcli_core-0.8.0/hcli_core/hcli/secondaryhome.py
--rwxr-x---   0 jeff       (501) staff       (20)      168 2022-03-20 22:23:04.000000 hcli_core-0.8.0/hcli_core/hcli/semantic.py
--rwxr-x---   0 jeff       (501) staff       (20)     1397 2022-03-20 22:23:04.000000 hcli_core-0.8.0/hcli_core/hcli_core.py
--rwxr-x---   0 jeff       (501) staff       (20)      200 2022-03-20 22:23:04.000000 hcli_core-0.8.0/hcli_core/hutils.py
--rwxr-x---   0 jeff       (501) staff       (20)      121 2022-03-28 02:35:48.000000 hcli_core-0.8.0/hcli_core/package.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2022-03-28 02:53:31.238783 hcli_core-0.8.0/hcli_core/sample/
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2022-03-28 02:53:31.238154 hcli_core-0.8.0/hcli_core/sample/hfm/
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2022-03-28 02:53:31.245522 hcli_core-0.8.0/hcli_core/sample/hfm/cli/
--rwxr-x---   0 jeff       (501) staff       (20)        0 2022-03-20 22:23:04.000000 hcli_core-0.8.0/hcli_core/sample/hfm/cli/__init__.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2022-03-28 02:53:31.245809 hcli_core-0.8.0/hcli_core/sample/hfm/cli/__pycache__/
--rwxr-x---   0 jeff       (501) staff       (20)     1024 2022-03-20 22:23:04.000000 hcli_core-0.8.0/hcli_core/sample/hfm/cli/__pycache__/chroot.cpython-36.pyc
--rwxr-x---   0 jeff       (501) staff       (20)     1715 2022-03-20 22:23:04.000000 hcli_core-0.8.0/hcli_core/sample/hfm/cli/__pycache__/cli.cpython-36.pyc
--rwxr-x---   0 jeff       (501) staff       (20)      726 2022-03-20 22:23:04.000000 hcli_core-0.8.0/hcli_core/sample/hfm/cli/chroot.py
--rwxr-x---   0 jeff       (501) staff       (20)     1499 2022-03-20 22:23:04.000000 hcli_core-0.8.0/hcli_core/sample/hfm/cli/cli.py
--rwxr-x---   0 jeff       (501) staff       (20)     2505 2022-03-20 22:23:04.000000 hcli_core-0.8.0/hcli_core/sample/hfm/cli/template.json
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2022-03-28 02:53:31.238345 hcli_core-0.8.0/hcli_core/sample/hptt/
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2022-03-28 02:53:31.246845 hcli_core-0.8.0/hcli_core/sample/hptt/cli/
--rwxr-x---   0 jeff       (501) staff       (20)        0 2022-03-20 22:23:04.000000 hcli_core-0.8.0/hcli_core/sample/hptt/cli/__init__.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2022-03-28 02:53:31.247708 hcli_core-0.8.0/hcli_core/sample/hptt/cli/__pycache__/
--rwxr-x---   0 jeff       (501) staff       (20)      824 2022-03-20 22:23:04.000000 hcli_core-0.8.0/hcli_core/sample/hptt/cli/__pycache__/channel.cpython-36.pyc
--rwxr-x---   0 jeff       (501) staff       (20)     2802 2022-03-20 22:23:04.000000 hcli_core-0.8.0/hcli_core/sample/hptt/cli/__pycache__/channels.cpython-36.pyc
--rwxr-x---   0 jeff       (501) staff       (20)     1025 2022-03-20 22:23:04.000000 hcli_core-0.8.0/hcli_core/sample/hptt/cli/__pycache__/chroot.cpython-36.pyc
--rwxr-x---   0 jeff       (501) staff       (20)     2517 2022-03-20 22:23:04.000000 hcli_core-0.8.0/hcli_core/sample/hptt/cli/__pycache__/cli.cpython-36.pyc
--rwxr-x---   0 jeff       (501) staff       (20)     1612 2022-03-20 22:23:04.000000 hcli_core-0.8.0/hcli_core/sample/hptt/cli/__pycache__/data.cpython-36.pyc
--rwxr-x---   0 jeff       (501) staff       (20)      551 2022-03-20 22:23:04.000000 hcli_core-0.8.0/hcli_core/sample/hptt/cli/channel.py
--rwxr-x---   0 jeff       (501) staff       (20)      385 2022-03-20 22:23:04.000000 hcli_core-0.8.0/hcli_core/sample/hptt/cli/channels.json
--rwxr-x---   0 jeff       (501) staff       (20)     2936 2022-03-20 22:23:04.000000 hcli_core-0.8.0/hcli_core/sample/hptt/cli/channels.py
--rwxr-x---   0 jeff       (501) staff       (20)      726 2022-03-20 22:23:04.000000 hcli_core-0.8.0/hcli_core/sample/hptt/cli/chroot.py
--rwxr-x---   0 jeff       (501) staff       (20)     3562 2022-03-20 22:23:04.000000 hcli_core-0.8.0/hcli_core/sample/hptt/cli/cli.py
--rwxr-x---   0 jeff       (501) staff       (20)     1168 2022-03-20 22:23:04.000000 hcli_core-0.8.0/hcli_core/sample/hptt/cli/data.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2022-03-28 02:53:31.247999 hcli_core-0.8.0/hcli_core/sample/hptt/cli/scripts/
--rwxr-x---   0 jeff       (501) staff       (20)     1684 2022-03-20 22:23:04.000000 hcli_core-0.8.0/hcli_core/sample/hptt/cli/scripts/listen.sh
--rwxr-x---   0 jeff       (501) staff       (20)      390 2022-03-20 22:23:04.000000 hcli_core-0.8.0/hcli_core/sample/hptt/cli/scripts/watch.sh
--rwxr-x---   0 jeff       (501) staff       (20)     6543 2022-03-20 22:23:04.000000 hcli_core-0.8.0/hcli_core/sample/hptt/cli/template.json
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2022-03-28 02:53:31.238628 hcli_core-0.8.0/hcli_core/sample/hub/
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2022-03-28 02:53:31.248977 hcli_core-0.8.0/hcli_core/sample/hub/cli/
--rwxr-x---   0 jeff       (501) staff       (20)        0 2022-03-20 22:23:04.000000 hcli_core-0.8.0/hcli_core/sample/hub/cli/__init__.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2022-03-28 02:53:31.249561 hcli_core-0.8.0/hcli_core/sample/hub/cli/__pycache__/
--rwxr-x---   0 jeff       (501) staff       (20)     1033 2022-03-20 22:23:04.000000 hcli_core-0.8.0/hcli_core/sample/hub/cli/__pycache__/cli.cpython-36.pyc
--rwxr-x---   0 jeff       (501) staff       (20)     1596 2022-03-20 22:23:04.000000 hcli_core-0.8.0/hcli_core/sample/hub/cli/__pycache__/data.cpython-36.pyc
--rwxr-x---   0 jeff       (501) staff       (20)     1708 2022-03-20 22:23:05.000000 hcli_core-0.8.0/hcli_core/sample/hub/cli/__pycache__/hub.cpython-36.pyc
--rwxr-x---   0 jeff       (501) staff       (20)      641 2022-03-20 22:23:05.000000 hcli_core-0.8.0/hcli_core/sample/hub/cli/__pycache__/namespace.cpython-36.pyc
--rwxr-x---   0 jeff       (501) staff       (20)      925 2022-03-20 22:23:04.000000 hcli_core-0.8.0/hcli_core/sample/hub/cli/cli.py
--rwxr-x---   0 jeff       (501) staff       (20)     1153 2022-03-20 22:23:04.000000 hcli_core-0.8.0/hcli_core/sample/hub/cli/data.py
--rwxr-x---   0 jeff       (501) staff       (20)      522 2022-03-20 22:23:04.000000 hcli_core-0.8.0/hcli_core/sample/hub/cli/hub.json
--rwxr-x---   0 jeff       (501) staff       (20)     1431 2022-03-20 22:23:04.000000 hcli_core-0.8.0/hcli_core/sample/hub/cli/hub.py
--rwxr-x---   0 jeff       (501) staff       (20)      216 2022-03-20 22:23:04.000000 hcli_core-0.8.0/hcli_core/sample/hub/cli/namespace.py
--rwxr-x---   0 jeff       (501) staff       (20)     2983 2022-03-20 22:23:04.000000 hcli_core-0.8.0/hcli_core/sample/hub/cli/template.json
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2022-03-28 02:53:31.238829 hcli_core-0.8.0/hcli_core/sample/nw/
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2022-03-28 02:53:31.250386 hcli_core-0.8.0/hcli_core/sample/nw/cli/
--rwxr-x---   0 jeff       (501) staff       (20)        0 2022-03-20 22:23:05.000000 hcli_core-0.8.0/hcli_core/sample/nw/cli/__init__.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2022-03-28 02:53:31.250956 hcli_core-0.8.0/hcli_core/sample/nw/cli/__pycache__/
--rwxr-x---   0 jeff       (501) staff       (20)     2211 2022-03-20 22:23:05.000000 hcli_core-0.8.0/hcli_core/sample/nw/cli/__pycache__/cli.cpython-36.pyc
--rwxr-x---   0 jeff       (501) staff       (20)     1610 2022-03-20 22:23:05.000000 hcli_core-0.8.0/hcli_core/sample/nw/cli/__pycache__/data.cpython-36.pyc
--rwxr-x---   0 jeff       (501) staff       (20)     8358 2022-03-20 22:23:05.000000 hcli_core-0.8.0/hcli_core/sample/nw/cli/__pycache__/networks.cpython-36.pyc
--rwxr-x---   0 jeff       (501) staff       (20)      752 2022-03-20 22:23:05.000000 hcli_core-0.8.0/hcli_core/sample/nw/cli/__pycache__/pool.cpython-36.pyc
--rwxr-x---   0 jeff       (501) staff       (20)     3509 2022-03-20 22:23:05.000000 hcli_core-0.8.0/hcli_core/sample/nw/cli/cli.py
--rwxr-x---   0 jeff       (501) staff       (20)     1168 2022-03-20 22:23:05.000000 hcli_core-0.8.0/hcli_core/sample/nw/cli/data.py
--rwxr-x---   0 jeff       (501) staff       (20)    11712 2022-03-20 22:23:05.000000 hcli_core-0.8.0/hcli_core/sample/nw/cli/networks.py
--rwxr-x---   0 jeff       (501) staff       (20)      418 2022-03-20 22:23:05.000000 hcli_core-0.8.0/hcli_core/sample/nw/cli/pool.py
--rwxr-x---   0 jeff       (501) staff       (20)     8440 2022-03-20 22:23:05.000000 hcli_core-0.8.0/hcli_core/sample/nw/cli/template.json
--rwxr-x---   0 jeff       (501) staff       (20)     3670 2022-03-20 22:23:05.000000 hcli_core-0.8.0/hcli_core/template.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2022-03-28 02:53:31.241868 hcli_core-0.8.0/hcli_core.egg-info/
--rwxr-x---   0 jeff       (501) staff       (20)     4982 2022-03-28 02:53:31.000000 hcli_core-0.8.0/hcli_core.egg-info/PKG-INFO
--rwxr-x---   0 jeff       (501) staff       (20)     2774 2022-03-28 02:53:31.000000 hcli_core-0.8.0/hcli_core.egg-info/SOURCES.txt
--rwxr-x---   0 jeff       (501) staff       (20)        1 2022-03-28 02:53:31.000000 hcli_core-0.8.0/hcli_core.egg-info/dependency_links.txt
--rwxr-x---   0 jeff       (501) staff       (20)       55 2022-03-28 02:53:31.000000 hcli_core-0.8.0/hcli_core.egg-info/entry_points.txt
--rwxr-x---   0 jeff       (501) staff       (20)       14 2022-03-28 02:53:31.000000 hcli_core-0.8.0/hcli_core.egg-info/requires.txt
--rwxr-x---   0 jeff       (501) staff       (20)       10 2022-03-28 02:53:31.000000 hcli_core-0.8.0/hcli_core.egg-info/top_level.txt
--rwxr-x---   0 jeff       (501) staff       (20)       67 2022-03-28 02:53:31.251424 hcli_core-0.8.0/setup.cfg
--rwxr-x---   0 jeff       (501) staff       (20)     2512 2022-03-20 22:23:05.000000 hcli_core-0.8.0/setup.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2022-04-12 23:15:46.758046 hcli_core-0.9.0/
+-rwxr-x---   0 jeff       (501) staff       (20)     1056 2022-03-20 22:23:05.000000 hcli_core-0.9.0/LICENSE.txt
+-rwxr-x---   0 jeff       (501) staff       (20)      280 2022-03-20 22:23:05.000000 hcli_core-0.9.0/MANIFEST.in
+-rw-r--r--   0 jeff       (501) staff       (20)     5361 2022-04-12 23:15:46.758126 hcli_core-0.9.0/PKG-INFO
+-rw-r--r--   0 jeff       (501) staff       (20)     3814 2022-04-12 23:11:26.000000 hcli_core-0.9.0/README.rst
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2022-04-12 23:15:46.748771 hcli_core-0.9.0/hcli_core/
+-rwxr-x---   0 jeff       (501) staff       (20)        0 2022-03-20 22:23:05.000000 hcli_core-0.9.0/hcli_core/__init__.py
+-rwxr-x---   0 jeff       (501) staff       (20)     1632 2022-03-20 22:23:05.000000 hcli_core-0.9.0/hcli_core/__main__.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2022-04-12 23:15:46.749915 hcli_core-0.9.0/hcli_core/cli/
+-rwxr-x---   0 jeff       (501) staff       (20)        0 2022-03-20 22:23:03.000000 hcli_core-0.9.0/hcli_core/cli/__init__.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2022-04-12 23:15:46.750035 hcli_core-0.9.0/hcli_core/cli/__pycache__/
+-rwxr-x---   0 jeff       (501) staff       (20)     1032 2022-03-20 22:23:03.000000 hcli_core-0.9.0/hcli_core/cli/__pycache__/cli.cpython-36.pyc
+-rwxr-x---   0 jeff       (501) staff       (20)      794 2022-03-20 22:23:03.000000 hcli_core-0.9.0/hcli_core/cli/cli.py
+-rwxr-x---   0 jeff       (501) staff       (20)     1686 2022-03-20 22:23:03.000000 hcli_core-0.9.0/hcli_core/cli/template.json
+-rwxr-x---   0 jeff       (501) staff       (20)      786 2022-04-12 23:01:22.000000 hcli_core-0.9.0/hcli_core/config.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2022-04-12 23:15:46.750297 hcli_core-0.9.0/hcli_core/data/
+-rw-r--r--   0 jeff       (501) staff       (20)     1535 2022-04-12 23:02:38.000000 hcli_core-0.9.0/hcli_core/data/hcli_core.1
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2022-04-12 23:15:46.750509 hcli_core-0.9.0/hcli_core/haliot/
+-rwxr-x---   0 jeff       (501) staff       (20)        0 2022-03-20 22:23:03.000000 hcli_core-0.9.0/hcli_core/haliot/__init__.py
+-rwxr-x---   0 jeff       (501) staff       (20)     1842 2022-03-20 22:23:03.000000 hcli_core-0.9.0/hcli_core/haliot/hal.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2022-04-12 23:15:46.752242 hcli_core-0.9.0/hcli_core/hcli/
+-rwxr-x---   0 jeff       (501) staff       (20)        0 2022-03-20 22:23:04.000000 hcli_core-0.9.0/hcli_core/hcli/__init__.py
+-rwxr-x---   0 jeff       (501) staff       (20)     2278 2022-03-20 22:23:04.000000 hcli_core-0.9.0/hcli_core/hcli/api.py
+-rwxr-x---   0 jeff       (501) staff       (20)     1958 2022-03-20 22:23:04.000000 hcli_core-0.9.0/hcli_core/hcli/command.py
+-rwxr-x---   0 jeff       (501) staff       (20)     4103 2022-03-20 22:23:04.000000 hcli_core-0.9.0/hcli_core/hcli/document.py
+-rwxr-x---   0 jeff       (501) staff       (20)     2085 2022-03-20 22:23:04.000000 hcli_core-0.9.0/hcli_core/hcli/execution.py
+-rwxr-x---   0 jeff       (501) staff       (20)     1617 2022-03-20 22:23:04.000000 hcli_core-0.9.0/hcli_core/hcli/finalexecution.py
+-rwxr-x---   0 jeff       (501) staff       (20)      894 2022-03-20 22:23:04.000000 hcli_core-0.9.0/hcli_core/hcli/home.py
+-rwxr-x---   0 jeff       (501) staff       (20)     1863 2022-03-20 22:23:04.000000 hcli_core-0.9.0/hcli_core/hcli/option.py
+-rwxr-x---   0 jeff       (501) staff       (20)     1928 2022-03-20 22:23:04.000000 hcli_core-0.9.0/hcli_core/hcli/parameter.py
+-rwxr-x---   0 jeff       (501) staff       (20)      100 2022-03-20 22:23:04.000000 hcli_core-0.9.0/hcli_core/hcli/profile.py
+-rwxr-x---   0 jeff       (501) staff       (20)      955 2022-03-20 22:23:04.000000 hcli_core-0.9.0/hcli_core/hcli/secondaryhome.py
+-rwxr-x---   0 jeff       (501) staff       (20)      168 2022-03-20 22:23:04.000000 hcli_core-0.9.0/hcli_core/hcli/semantic.py
+-rwxr-x---   0 jeff       (501) staff       (20)     1397 2022-04-12 22:49:17.000000 hcli_core-0.9.0/hcli_core/hcli_core.py
+-rwxr-x---   0 jeff       (501) staff       (20)      200 2022-03-20 22:23:04.000000 hcli_core-0.9.0/hcli_core/hutils.py
+-rwxr-x---   0 jeff       (501) staff       (20)      121 2022-04-12 23:12:02.000000 hcli_core-0.9.0/hcli_core/package.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2022-04-12 23:15:46.747031 hcli_core-0.9.0/hcli_core/sample/
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2022-04-12 23:15:46.746518 hcli_core-0.9.0/hcli_core/sample/hfm/
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2022-04-12 23:15:46.752732 hcli_core-0.9.0/hcli_core/sample/hfm/cli/
+-rwxr-x---   0 jeff       (501) staff       (20)        0 2022-03-20 22:23:04.000000 hcli_core-0.9.0/hcli_core/sample/hfm/cli/__init__.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2022-04-12 23:15:46.752975 hcli_core-0.9.0/hcli_core/sample/hfm/cli/__pycache__/
+-rwxr-x---   0 jeff       (501) staff       (20)     1024 2022-03-20 22:23:04.000000 hcli_core-0.9.0/hcli_core/sample/hfm/cli/__pycache__/chroot.cpython-36.pyc
+-rwxr-x---   0 jeff       (501) staff       (20)     1715 2022-03-20 22:23:04.000000 hcli_core-0.9.0/hcli_core/sample/hfm/cli/__pycache__/cli.cpython-36.pyc
+-rwxr-x---   0 jeff       (501) staff       (20)      726 2022-03-20 22:23:04.000000 hcli_core-0.9.0/hcli_core/sample/hfm/cli/chroot.py
+-rwxr-x---   0 jeff       (501) staff       (20)     1499 2022-03-20 22:23:04.000000 hcli_core-0.9.0/hcli_core/sample/hfm/cli/cli.py
+-rwxr-x---   0 jeff       (501) staff       (20)     2505 2022-03-20 22:23:04.000000 hcli_core-0.9.0/hcli_core/sample/hfm/cli/template.json
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2022-04-12 23:15:46.746681 hcli_core-0.9.0/hcli_core/sample/hptt/
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2022-04-12 23:15:46.753965 hcli_core-0.9.0/hcli_core/sample/hptt/cli/
+-rwxr-x---   0 jeff       (501) staff       (20)        0 2022-03-20 22:23:04.000000 hcli_core-0.9.0/hcli_core/sample/hptt/cli/__init__.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2022-04-12 23:15:46.754837 hcli_core-0.9.0/hcli_core/sample/hptt/cli/__pycache__/
+-rwxr-x---   0 jeff       (501) staff       (20)      824 2022-03-20 22:23:04.000000 hcli_core-0.9.0/hcli_core/sample/hptt/cli/__pycache__/channel.cpython-36.pyc
+-rwxr-x---   0 jeff       (501) staff       (20)     2802 2022-03-20 22:23:04.000000 hcli_core-0.9.0/hcli_core/sample/hptt/cli/__pycache__/channels.cpython-36.pyc
+-rwxr-x---   0 jeff       (501) staff       (20)     1025 2022-03-20 22:23:04.000000 hcli_core-0.9.0/hcli_core/sample/hptt/cli/__pycache__/chroot.cpython-36.pyc
+-rwxr-x---   0 jeff       (501) staff       (20)     2517 2022-03-20 22:23:04.000000 hcli_core-0.9.0/hcli_core/sample/hptt/cli/__pycache__/cli.cpython-36.pyc
+-rwxr-x---   0 jeff       (501) staff       (20)     1612 2022-03-20 22:23:04.000000 hcli_core-0.9.0/hcli_core/sample/hptt/cli/__pycache__/data.cpython-36.pyc
+-rwxr-x---   0 jeff       (501) staff       (20)      551 2022-03-20 22:23:04.000000 hcli_core-0.9.0/hcli_core/sample/hptt/cli/channel.py
+-rwxr-x---   0 jeff       (501) staff       (20)      385 2022-03-20 22:23:04.000000 hcli_core-0.9.0/hcli_core/sample/hptt/cli/channels.json
+-rwxr-x---   0 jeff       (501) staff       (20)     2936 2022-03-20 22:23:04.000000 hcli_core-0.9.0/hcli_core/sample/hptt/cli/channels.py
+-rwxr-x---   0 jeff       (501) staff       (20)      726 2022-03-20 22:23:04.000000 hcli_core-0.9.0/hcli_core/sample/hptt/cli/chroot.py
+-rwxr-x---   0 jeff       (501) staff       (20)     3562 2022-03-20 22:23:04.000000 hcli_core-0.9.0/hcli_core/sample/hptt/cli/cli.py
+-rwxr-x---   0 jeff       (501) staff       (20)     1168 2022-03-20 22:23:04.000000 hcli_core-0.9.0/hcli_core/sample/hptt/cli/data.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2022-04-12 23:15:46.755111 hcli_core-0.9.0/hcli_core/sample/hptt/cli/scripts/
+-rwxr-x---   0 jeff       (501) staff       (20)     1684 2022-03-20 22:23:04.000000 hcli_core-0.9.0/hcli_core/sample/hptt/cli/scripts/listen.sh
+-rwxr-x---   0 jeff       (501) staff       (20)      390 2022-03-20 22:23:04.000000 hcli_core-0.9.0/hcli_core/sample/hptt/cli/scripts/watch.sh
+-rwxr-x---   0 jeff       (501) staff       (20)     6543 2022-03-20 22:23:04.000000 hcli_core-0.9.0/hcli_core/sample/hptt/cli/template.json
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2022-04-12 23:15:46.746906 hcli_core-0.9.0/hcli_core/sample/hub/
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2022-04-12 23:15:46.756030 hcli_core-0.9.0/hcli_core/sample/hub/cli/
+-rwxr-x---   0 jeff       (501) staff       (20)        0 2022-03-20 22:23:04.000000 hcli_core-0.9.0/hcli_core/sample/hub/cli/__init__.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2022-04-12 23:15:46.756576 hcli_core-0.9.0/hcli_core/sample/hub/cli/__pycache__/
+-rwxr-x---   0 jeff       (501) staff       (20)     1033 2022-03-20 22:23:04.000000 hcli_core-0.9.0/hcli_core/sample/hub/cli/__pycache__/cli.cpython-36.pyc
+-rwxr-x---   0 jeff       (501) staff       (20)     1596 2022-03-20 22:23:04.000000 hcli_core-0.9.0/hcli_core/sample/hub/cli/__pycache__/data.cpython-36.pyc
+-rwxr-x---   0 jeff       (501) staff       (20)     1708 2022-03-20 22:23:05.000000 hcli_core-0.9.0/hcli_core/sample/hub/cli/__pycache__/hub.cpython-36.pyc
+-rwxr-x---   0 jeff       (501) staff       (20)      641 2022-03-20 22:23:05.000000 hcli_core-0.9.0/hcli_core/sample/hub/cli/__pycache__/namespace.cpython-36.pyc
+-rwxr-x---   0 jeff       (501) staff       (20)      925 2022-03-20 22:23:04.000000 hcli_core-0.9.0/hcli_core/sample/hub/cli/cli.py
+-rwxr-x---   0 jeff       (501) staff       (20)     1153 2022-03-20 22:23:04.000000 hcli_core-0.9.0/hcli_core/sample/hub/cli/data.py
+-rwxr-x---   0 jeff       (501) staff       (20)      522 2022-03-20 22:23:04.000000 hcli_core-0.9.0/hcli_core/sample/hub/cli/hub.json
+-rwxr-x---   0 jeff       (501) staff       (20)     1431 2022-03-20 22:23:04.000000 hcli_core-0.9.0/hcli_core/sample/hub/cli/hub.py
+-rwxr-x---   0 jeff       (501) staff       (20)      216 2022-03-20 22:23:04.000000 hcli_core-0.9.0/hcli_core/sample/hub/cli/namespace.py
+-rwxr-x---   0 jeff       (501) staff       (20)     2983 2022-03-20 22:23:04.000000 hcli_core-0.9.0/hcli_core/sample/hub/cli/template.json
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2022-04-12 23:15:46.747072 hcli_core-0.9.0/hcli_core/sample/nw/
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2022-04-12 23:15:46.757357 hcli_core-0.9.0/hcli_core/sample/nw/cli/
+-rwxr-x---   0 jeff       (501) staff       (20)        0 2022-03-20 22:23:05.000000 hcli_core-0.9.0/hcli_core/sample/nw/cli/__init__.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2022-04-12 23:15:46.757918 hcli_core-0.9.0/hcli_core/sample/nw/cli/__pycache__/
+-rwxr-x---   0 jeff       (501) staff       (20)     2211 2022-03-20 22:23:05.000000 hcli_core-0.9.0/hcli_core/sample/nw/cli/__pycache__/cli.cpython-36.pyc
+-rwxr-x---   0 jeff       (501) staff       (20)     1610 2022-03-20 22:23:05.000000 hcli_core-0.9.0/hcli_core/sample/nw/cli/__pycache__/data.cpython-36.pyc
+-rwxr-x---   0 jeff       (501) staff       (20)     8358 2022-03-20 22:23:05.000000 hcli_core-0.9.0/hcli_core/sample/nw/cli/__pycache__/networks.cpython-36.pyc
+-rwxr-x---   0 jeff       (501) staff       (20)      752 2022-03-20 22:23:05.000000 hcli_core-0.9.0/hcli_core/sample/nw/cli/__pycache__/pool.cpython-36.pyc
+-rwxr-x---   0 jeff       (501) staff       (20)     3509 2022-03-20 22:23:05.000000 hcli_core-0.9.0/hcli_core/sample/nw/cli/cli.py
+-rwxr-x---   0 jeff       (501) staff       (20)     1168 2022-03-20 22:23:05.000000 hcli_core-0.9.0/hcli_core/sample/nw/cli/data.py
+-rwxr-x---   0 jeff       (501) staff       (20)    11712 2022-03-20 22:23:05.000000 hcli_core-0.9.0/hcli_core/sample/nw/cli/networks.py
+-rwxr-x---   0 jeff       (501) staff       (20)      418 2022-03-20 22:23:05.000000 hcli_core-0.9.0/hcli_core/sample/nw/cli/pool.py
+-rwxr-x---   0 jeff       (501) staff       (20)     8440 2022-03-20 22:23:05.000000 hcli_core-0.9.0/hcli_core/sample/nw/cli/template.json
+-rwxr-x---   0 jeff       (501) staff       (20)     3670 2022-03-20 22:23:05.000000 hcli_core-0.9.0/hcli_core/template.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2022-04-12 23:15:46.749463 hcli_core-0.9.0/hcli_core.egg-info/
+-rwxr-x---   0 jeff       (501) staff       (20)     5361 2022-04-12 23:15:46.000000 hcli_core-0.9.0/hcli_core.egg-info/PKG-INFO
+-rwxr-x---   0 jeff       (501) staff       (20)     2774 2022-04-12 23:15:46.000000 hcli_core-0.9.0/hcli_core.egg-info/SOURCES.txt
+-rwxr-x---   0 jeff       (501) staff       (20)        1 2022-04-12 23:15:46.000000 hcli_core-0.9.0/hcli_core.egg-info/dependency_links.txt
+-rwxr-x---   0 jeff       (501) staff       (20)       55 2022-04-12 23:15:46.000000 hcli_core-0.9.0/hcli_core.egg-info/entry_points.txt
+-rwxr-x---   0 jeff       (501) staff       (20)       14 2022-04-12 23:15:46.000000 hcli_core-0.9.0/hcli_core.egg-info/requires.txt
+-rwxr-x---   0 jeff       (501) staff       (20)       10 2022-04-12 23:15:46.000000 hcli_core-0.9.0/hcli_core.egg-info/top_level.txt
+-rwxr-x---   0 jeff       (501) staff       (20)       67 2022-04-12 23:15:46.758330 hcli_core-0.9.0/setup.cfg
+-rwxr-x---   0 jeff       (501) staff       (20)     2512 2022-03-20 22:23:05.000000 hcli_core-0.9.0/setup.py
```

### Comparing `hcli_core-0.8.0/LICENSE.txt` & `hcli_core-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/PKG-INFO` & `hcli_core-0.9.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: hcli_core
-Version: 0.8.0
+Version: 0.9.0
 Summary: An HCLI connector that can be used to expose any CLI expressed through hypertext command line interface (HCLI) semantics.
 Home-page: https://github.com/cometaj2/hcli_core
 Author: Jeff Michaud
 Author-email: cometaj2@comcast.net
 License: MIT
 Description: HCLI Core |build status|_ |pypi|_
         =================================
@@ -82,14 +82,17 @@
         
             $ huckle help
         
         Bugs
         ----
         
         - No good handling of control over request and response in cli code which can lead to exceptions and empty response client side.
+        - The hfm sample HCLI fails disgracefully when copying a remote file name that doesn't exist (server error).
+        - Unresolved, but otherwise apparently unimpactful gunicorn deprecated warning (gunicorn/workers/gthread.py:323: DeprecatedWarning: Call to deprecated property body. Please use text instead.
+          respiter = self.wsgi(environ, resp.start_response)).
         
         .. |build status| image:: https://circleci.com/gh/cometaj2/hcli_core.svg?style=shield
         .. _build status: https://circleci.com/gh/cometaj2/huckle
         .. |pypi| image:: https://badge.fury.io/py/hcli-core.svg
         .. _pypi: https://badge.fury.io/py/hcli-core
         
 Keywords: cli client server connector hypermedia rest generic development
```

### Comparing `hcli_core-0.8.0/README.rst` & `hcli_core-0.9.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -74,12 +74,15 @@
 
     $ huckle help
 
 Bugs
 ----
 
 - No good handling of control over request and response in cli code which can lead to exceptions and empty response client side.
+- The hfm sample HCLI fails disgracefully when copying a remote file name that doesn't exist (server error).
+- Unresolved, but otherwise apparently unimpactful gunicorn deprecated warning (gunicorn/workers/gthread.py:323: DeprecatedWarning: Call to deprecated property body. Please use text instead.
+  respiter = self.wsgi(environ, resp.start_response)).
 
 .. |build status| image:: https://circleci.com/gh/cometaj2/hcli_core.svg?style=shield
 .. _build status: https://circleci.com/gh/cometaj2/huckle
 .. |pypi| image:: https://badge.fury.io/py/hcli-core.svg
 .. _pypi: https://badge.fury.io/py/hcli-core
```

### Comparing `hcli_core-0.8.0/hcli_core/__main__.py` & `hcli_core-0.9.0/hcli_core/__main__.py`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/cli/__pycache__/cli.cpython-36.pyc` & `hcli_core-0.9.0/hcli_core/cli/__pycache__/cli.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/cli/cli.py` & `hcli_core-0.9.0/hcli_core/cli/cli.py`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/cli/template.json` & `hcli_core-0.9.0/hcli_core/cli/template.json`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/config.py` & `hcli_core-0.9.0/hcli_core/config.py`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/data/hcli_core.1` & `hcli_core-0.9.0/hcli_core/data/hcli_core.1`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/haliot/hal.py` & `hcli_core-0.9.0/hcli_core/haliot/hal.py`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/hcli/api.py` & `hcli_core-0.9.0/hcli_core/hcli/api.py`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/hcli/command.py` & `hcli_core-0.9.0/hcli_core/hcli/command.py`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/hcli/document.py` & `hcli_core-0.9.0/hcli_core/hcli/document.py`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/hcli/execution.py` & `hcli_core-0.9.0/hcli_core/hcli/execution.py`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/hcli/finalexecution.py` & `hcli_core-0.9.0/hcli_core/hcli/finalexecution.py`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/hcli/home.py` & `hcli_core-0.9.0/hcli_core/hcli/home.py`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/hcli/option.py` & `hcli_core-0.9.0/hcli_core/hcli/option.py`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/hcli/parameter.py` & `hcli_core-0.9.0/hcli_core/hcli/parameter.py`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/hcli/secondaryhome.py` & `hcli_core-0.9.0/hcli_core/hcli/secondaryhome.py`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/hcli_core.py` & `hcli_core-0.9.0/hcli_core/hcli_core.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 def connector(plugin_path=None):
 
         # We load the HCLI template in memory to reduce disk io
         config.set_plugin_path(plugin_path)
         config.parse_template(template.Template())
 
         # We setup the HCLI Connector
-        server = falcon.API()
+        server = falcon.App()
         server.add_route(home.HomeController.route, api.HomeApi())
         server.add_route(secondaryhome.SecondaryHomeController.route, api.SecondaryHomeApi())
         server.add_route(document.DocumentController.route, api.DocumentApi())
         server.add_route(command.CommandController.route, api.CommandApi())
         server.add_route(option.OptionController.route, api.OptionApi())
         server.add_route(execution.ExecutionController.route, api.ExecutionApi())
         server.add_route(finalexecution.FinalGetExecutionController.route, api.FinalExecutionApi())
```

### Comparing `hcli_core-0.8.0/hcli_core/sample/hfm/cli/__pycache__/chroot.cpython-36.pyc` & `hcli_core-0.9.0/hcli_core/sample/hfm/cli/__pycache__/chroot.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/sample/hfm/cli/__pycache__/cli.cpython-36.pyc` & `hcli_core-0.9.0/hcli_core/sample/hfm/cli/__pycache__/cli.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/sample/hfm/cli/chroot.py` & `hcli_core-0.9.0/hcli_core/sample/hfm/cli/chroot.py`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/sample/hfm/cli/cli.py` & `hcli_core-0.9.0/hcli_core/sample/hfm/cli/cli.py`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/sample/hfm/cli/template.json` & `hcli_core-0.9.0/hcli_core/sample/hfm/cli/template.json`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/sample/hptt/cli/__pycache__/channel.cpython-36.pyc` & `hcli_core-0.9.0/hcli_core/sample/hptt/cli/__pycache__/channel.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/sample/hptt/cli/__pycache__/channels.cpython-36.pyc` & `hcli_core-0.9.0/hcli_core/sample/hptt/cli/__pycache__/channels.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/sample/hptt/cli/__pycache__/chroot.cpython-36.pyc` & `hcli_core-0.9.0/hcli_core/sample/hptt/cli/__pycache__/chroot.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/sample/hptt/cli/__pycache__/cli.cpython-36.pyc` & `hcli_core-0.9.0/hcli_core/sample/hptt/cli/__pycache__/cli.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/sample/hptt/cli/__pycache__/data.cpython-36.pyc` & `hcli_core-0.9.0/hcli_core/sample/hptt/cli/__pycache__/data.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/sample/hptt/cli/channel.py` & `hcli_core-0.9.0/hcli_core/sample/hptt/cli/channel.py`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/sample/hptt/cli/channels.py` & `hcli_core-0.9.0/hcli_core/sample/hptt/cli/channels.py`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/sample/hptt/cli/chroot.py` & `hcli_core-0.9.0/hcli_core/sample/hptt/cli/chroot.py`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/sample/hptt/cli/cli.py` & `hcli_core-0.9.0/hcli_core/sample/hptt/cli/cli.py`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/sample/hptt/cli/data.py` & `hcli_core-0.9.0/hcli_core/sample/hptt/cli/data.py`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/sample/hptt/cli/scripts/listen.sh` & `hcli_core-0.9.0/hcli_core/sample/hptt/cli/scripts/listen.sh`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/sample/hptt/cli/template.json` & `hcli_core-0.9.0/hcli_core/sample/hptt/cli/template.json`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/sample/hub/cli/__pycache__/cli.cpython-36.pyc` & `hcli_core-0.9.0/hcli_core/sample/hub/cli/__pycache__/cli.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/sample/hub/cli/__pycache__/data.cpython-36.pyc` & `hcli_core-0.9.0/hcli_core/sample/hub/cli/__pycache__/data.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/sample/hub/cli/__pycache__/hub.cpython-36.pyc` & `hcli_core-0.9.0/hcli_core/sample/hub/cli/__pycache__/hub.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/sample/hub/cli/__pycache__/namespace.cpython-36.pyc` & `hcli_core-0.9.0/hcli_core/sample/hub/cli/__pycache__/namespace.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/sample/hub/cli/cli.py` & `hcli_core-0.9.0/hcli_core/sample/hub/cli/cli.py`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/sample/hub/cli/data.py` & `hcli_core-0.9.0/hcli_core/sample/hub/cli/data.py`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/sample/hub/cli/hub.json` & `hcli_core-0.9.0/hcli_core/sample/hub/cli/hub.json`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/sample/hub/cli/hub.py` & `hcli_core-0.9.0/hcli_core/sample/hub/cli/hub.py`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/sample/hub/cli/template.json` & `hcli_core-0.9.0/hcli_core/sample/hub/cli/template.json`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/sample/nw/cli/__pycache__/cli.cpython-36.pyc` & `hcli_core-0.9.0/hcli_core/sample/nw/cli/__pycache__/cli.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/sample/nw/cli/__pycache__/data.cpython-36.pyc` & `hcli_core-0.9.0/hcli_core/sample/nw/cli/__pycache__/data.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/sample/nw/cli/__pycache__/networks.cpython-36.pyc` & `hcli_core-0.9.0/hcli_core/sample/nw/cli/__pycache__/networks.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/sample/nw/cli/__pycache__/pool.cpython-36.pyc` & `hcli_core-0.9.0/hcli_core/sample/nw/cli/__pycache__/pool.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/sample/nw/cli/cli.py` & `hcli_core-0.9.0/hcli_core/sample/nw/cli/cli.py`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/sample/nw/cli/data.py` & `hcli_core-0.9.0/hcli_core/sample/nw/cli/data.py`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/sample/nw/cli/networks.py` & `hcli_core-0.9.0/hcli_core/sample/nw/cli/networks.py`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/sample/nw/cli/template.json` & `hcli_core-0.9.0/hcli_core/sample/nw/cli/template.json`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core/template.py` & `hcli_core-0.9.0/hcli_core/template.py`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/hcli_core.egg-info/PKG-INFO` & `hcli_core-0.9.0/hcli_core.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: hcli-core
-Version: 0.8.0
+Version: 0.9.0
 Summary: An HCLI connector that can be used to expose any CLI expressed through hypertext command line interface (HCLI) semantics.
 Home-page: https://github.com/cometaj2/hcli_core
 Author: Jeff Michaud
 Author-email: cometaj2@comcast.net
 License: MIT
 Description: HCLI Core |build status|_ |pypi|_
         =================================
@@ -82,14 +82,17 @@
         
             $ huckle help
         
         Bugs
         ----
         
         - No good handling of control over request and response in cli code which can lead to exceptions and empty response client side.
+        - The hfm sample HCLI fails disgracefully when copying a remote file name that doesn't exist (server error).
+        - Unresolved, but otherwise apparently unimpactful gunicorn deprecated warning (gunicorn/workers/gthread.py:323: DeprecatedWarning: Call to deprecated property body. Please use text instead.
+          respiter = self.wsgi(environ, resp.start_response)).
         
         .. |build status| image:: https://circleci.com/gh/cometaj2/hcli_core.svg?style=shield
         .. _build status: https://circleci.com/gh/cometaj2/huckle
         .. |pypi| image:: https://badge.fury.io/py/hcli-core.svg
         .. _pypi: https://badge.fury.io/py/hcli-core
         
 Keywords: cli client server connector hypermedia rest generic development
```

### Comparing `hcli_core-0.8.0/hcli_core.egg-info/SOURCES.txt` & `hcli_core-0.9.0/hcli_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcli_core-0.8.0/setup.py` & `hcli_core-0.9.0/setup.py`

 * *Files identical despite different names*

