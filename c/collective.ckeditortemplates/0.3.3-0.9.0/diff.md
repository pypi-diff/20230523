# Comparing `tmp/collective.ckeditortemplates-0.3.3.tar.gz` & `tmp/collective.ckeditortemplates-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/collective.ckeditortemplates-0.3.3.tar", last modified: Tue Apr 20 10:35:05 2021, max compression
+gzip compressed data, was "collective.ckeditortemplates-0.9.0.tar", last modified: Tue May 23 08:50:10 2023, max compression
```

## Comparing `collective.ckeditortemplates-0.3.3.tar` & `collective.ckeditortemplates-0.9.0.tar`

### file list

```diff
@@ -1,77 +1,84 @@
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/
--rw-rw-r--   0 sge       (1000) sge       (1000)       38 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/setup.cfg
--rw-rw-r--   0 sge       (1000) sge       (1000)     5840 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/PKG-INFO
--rw-rw-r--   0 sge       (1000) sge       (1000)     1633 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/setup.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     2079 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/README.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)      161 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/MANIFEST.in
--rw-rw-r--   0 sge       (1000) sge       (1000)      157 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/CONTRIBUTORS.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)     1623 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/CHANGES.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)      176 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/.gitignore
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective.ckeditortemplates.egg-info/
--rw-rw-r--   0 sge       (1000) sge       (1000)       11 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective.ckeditortemplates.egg-info/top_level.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)      151 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective.ckeditortemplates.egg-info/requires.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)        1 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective.ckeditortemplates.egg-info/not-zip-safe
--rw-rw-r--   0 sge       (1000) sge       (1000)       11 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective.ckeditortemplates.egg-info/namespace_packages.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)       37 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective.ckeditortemplates.egg-info/entry_points.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)        1 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective.ckeditortemplates.egg-info/dependency_links.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)     2812 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective.ckeditortemplates.egg-info/SOURCES.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)     5840 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective.ckeditortemplates.egg-info/PKG-INFO
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/
--rw-rw-r--   0 sge       (1000) sge       (1000)       56 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/__init__.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/
--rw-rw-r--   0 sge       (1000) sge       (1000)     1650 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/upgrades.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     1837 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/testing.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     1229 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/setuphandlers.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     1675 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/profiles.zcml
--rw-rw-r--   0 sge       (1000) sge       (1000)     1303 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/configure.zcml
--rw-rw-r--   0 sge       (1000) sge       (1000)      940 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/cktemplatefolder_icon.gif
--rw-rw-r--   0 sge       (1000) sge       (1000)      915 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/cktemplate_icon.gif
--rw-rw-r--   0 sge       (1000) sge       (1000)     2653 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/cktemplate.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      203 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/__init__.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/tests/
--rw-rw-r--   0 sge       (1000) sge       (1000)      483 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/tests/test_robot.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      873 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/tests/test_cktemplate.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     1612 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/tests/test.robot
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/tests/__init__.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/profiles/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/profiles/default/
--rw-rw-r--   0 sge       (1000) sge       (1000)      232 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/profiles/default/workflows.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      206 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/profiles/default/types.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      293 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/profiles/default/propertiestool.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      236 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/profiles/default/metadata.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      503 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/profiles/default/controlpanel.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/profiles/default/collective.ckeditortemplates_various.txt
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/profiles/default/workflows/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/profiles/default/workflows/cktemplate_workflow/
--rw-rw-r--   0 sge       (1000) sge       (1000)     5539 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/profiles/default/workflows/cktemplate_workflow/definition.xml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/profiles/default/types/
--rw-rw-r--   0 sge       (1000) sge       (1000)     2300 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/profiles/default/types/cktemplatefolder.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)     2045 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/profiles/default/types/cktemplate.xml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/locales/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/locales/nl/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/locales/nl/LC_MESSAGES/
--rw-rw-r--   0 sge       (1000) sge       (1000)     2308 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/locales/nl/LC_MESSAGES/plone.po
--rw-rw-r--   0 sge       (1000) sge       (1000)      941 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/locales/nl/LC_MESSAGES/collective.ckeditortemplates.po
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/locales/fr/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 sge       (1000) sge       (1000)     2393 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/locales/fr/LC_MESSAGES/plone.po
--rw-rw-r--   0 sge       (1000) sge       (1000)     1170 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/locales/fr/LC_MESSAGES/collective.ckeditortemplates.po
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/locales/es/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/locales/es/LC_MESSAGES/
--rw-rw-r--   0 sge       (1000) sge       (1000)     2986 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/locales/es/LC_MESSAGES/plone.po
--rw-rw-r--   0 sge       (1000) sge       (1000)     1550 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/locales/es/LC_MESSAGES/collective.ckeditortemplates.po
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/locales/en/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/locales/en/LC_MESSAGES/
--rw-rw-r--   0 sge       (1000) sge       (1000)     2308 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/locales/en/LC_MESSAGES/plone.po
--rw-rw-r--   0 sge       (1000) sge       (1000)      941 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/locales/en/LC_MESSAGES/collective.ckeditortemplates.po
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/browser/
--rw-rw-r--   0 sge       (1000) sge       (1000)      444 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/browser/configure.zcml
--rw-rw-r--   0 sge       (1000) sge       (1000)     1784 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/browser/cktemplatelisting.py
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/browser/__init__.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/browser/tests/
--rw-rw-r--   0 sge       (1000) sge       (1000)     1496 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/browser/tests/test_cktemplatelisting.py
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/browser/tests/__init__.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/docs/
--rw-rw-r--   0 sge       (1000) sge       (1000)      725 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/docs/LICENSE.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)    18092 2021-04-20 10:35:05.000000 collective.ckeditortemplates-0.3.3/docs/LICENSE.GPL
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-05-23 08:50:10.231679 collective.ckeditortemplates-0.9.0/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      226 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/.gitignore
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1719 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/CHANGES.rst
+-rw-rw-r--   0 sge       (1000) sge       (1000)      157 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/CONTRIBUTORS.rst
+-rw-rw-r--   0 sge       (1000) sge       (1000)      161 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/MANIFEST.in
+-rw-rw-r--   0 sge       (1000) sge       (1000)     4740 2023-05-23 08:50:10.231679 collective.ckeditortemplates-0.9.0/PKG-INFO
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2079 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/README.rst
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-05-23 08:50:10.231679 collective.ckeditortemplates-0.9.0/docs/
+-rw-rw-r--   0 sge       (1000) sge       (1000)    18092 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/docs/LICENSE.GPL
+-rw-rw-r--   0 sge       (1000) sge       (1000)      725 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/docs/LICENSE.rst
+-rw-rw-r--   0 sge       (1000) sge       (1000)       38 2023-05-23 08:50:10.231679 collective.ckeditortemplates-0.9.0/setup.cfg
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1852 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/setup.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-05-23 08:50:10.227679 collective.ckeditortemplates-0.9.0/src/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-05-23 08:50:10.231679 collective.ckeditortemplates-0.9.0/src/collective/
+-rw-rw-r--   0 sge       (1000) sge       (1000)       56 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective/__init__.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-05-23 08:50:10.231679 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      270 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/__init__.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-05-23 08:50:10.231679 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/browser/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/browser/__init__.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1788 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/browser/cktemplatelisting.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      444 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/browser/configure.zcml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-05-23 08:50:10.231679 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/browser/tests/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/browser/tests/__init__.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2314 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/browser/tests/test_cktemplatelisting.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2675 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/cktemplate.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      915 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/cktemplate_icon.gif
+-rw-rw-r--   0 sge       (1000) sge       (1000)      940 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/cktemplatefolder_icon.gif
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1032 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/configure.zcml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-05-23 08:50:10.227679 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/locales/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-05-23 08:50:10.227679 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/locales/en/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-05-23 08:50:10.231679 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/locales/en/LC_MESSAGES/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      941 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/locales/en/LC_MESSAGES/collective.ckeditortemplates.po
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2308 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/locales/en/LC_MESSAGES/plone.po
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-05-23 08:50:10.227679 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/locales/es/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-05-23 08:50:10.231679 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/locales/es/LC_MESSAGES/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1550 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/locales/es/LC_MESSAGES/collective.ckeditortemplates.po
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2986 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/locales/es/LC_MESSAGES/plone.po
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-05-23 08:50:10.227679 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/locales/fr/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-05-23 08:50:10.231679 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1170 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/locales/fr/LC_MESSAGES/collective.ckeditortemplates.po
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2393 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/locales/fr/LC_MESSAGES/plone.po
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-05-23 08:50:10.227679 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/locales/nl/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-05-23 08:50:10.231679 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/locales/nl/LC_MESSAGES/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      941 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/locales/nl/LC_MESSAGES/collective.ckeditortemplates.po
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2308 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/locales/nl/LC_MESSAGES/plone.po
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-05-23 08:50:10.227679 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/profiles/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-05-23 08:50:10.231679 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/profiles/default/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/profiles/default/collective.ckeditortemplates_various.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)      503 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/profiles/default/controlpanel.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      236 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/profiles/default/metadata.xml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-05-23 08:50:10.231679 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/profiles/default/types/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2045 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/profiles/default/types/cktemplate.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2300 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/profiles/default/types/cktemplatefolder.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      206 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/profiles/default/types.xml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-05-23 08:50:10.227679 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/profiles/default/workflows/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-05-23 08:50:10.231679 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/profiles/default/workflows/cktemplate_workflow/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     5539 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/profiles/default/workflows/cktemplate_workflow/definition.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      232 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/profiles/default/workflows.xml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-05-23 08:50:10.231679 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/profiles/plone4/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/profiles/plone4/collective.ckeditortemplates_various.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)      187 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/profiles/plone4/metadata.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      293 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/profiles/plone4/propertiestool.xml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-05-23 08:50:10.231679 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/profiles/plone6/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/profiles/plone6/collective.ckeditortemplates_various.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)      187 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/profiles/plone6/metadata.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      269 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/profiles/plone6/registry.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2713 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/profiles.zcml
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1230 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/setuphandlers.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1834 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/testing.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-05-23 08:50:10.231679 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/tests/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/tests/__init__.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1612 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/tests/test.robot
+-rw-rw-r--   0 sge       (1000) sge       (1000)      930 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/tests/test_cktemplate.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      483 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/tests/test_robot.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2019 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/upgrades.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-05-23 08:50:10.231679 collective.ckeditortemplates-0.9.0/src/collective.ckeditortemplates.egg-info/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     4740 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective.ckeditortemplates.egg-info/PKG-INFO
+-rw-rw-r--   0 sge       (1000) sge       (1000)     3177 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective.ckeditortemplates.egg-info/SOURCES.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)        1 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective.ckeditortemplates.egg-info/dependency_links.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)       37 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective.ckeditortemplates.egg-info/entry_points.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)       11 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective.ckeditortemplates.egg-info/namespace_packages.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)        1 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective.ckeditortemplates.egg-info/not-zip-safe
+-rw-rw-r--   0 sge       (1000) sge       (1000)      151 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective.ckeditortemplates.egg-info/requires.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)       11 2023-05-23 08:50:10.000000 collective.ckeditortemplates-0.9.0/src/collective.ckeditortemplates.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `collective.ckeditortemplates-0.3.3/setup.py` & `collective.ckeditortemplates-0.9.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup, find_packages
 
-version = '0.3.3'
+version = '0.9.0'
 
 long_description = (
     open('README.rst').read()
     + '\n' +
     'Contributors\n'
     '============\n'
     + '\n' +
@@ -19,19 +19,23 @@
       description="Plone templates for ckeditor",
       long_description=long_description,
       # Get more strings from
       # http://pypi.python.org/pypi?%3Aaction=list_classifiers
       classifiers=[
           "Environment :: Web Environment",
           "Framework :: Plone",
-          "Framework :: Plone :: 4.2",
+          "Framework :: Plone :: Addon",
           "Framework :: Plone :: 4.3",
+          "Framework :: Plone :: 6.0",
           "Operating System :: OS Independent",
           "Programming Language :: Python",
           "Programming Language :: Python :: 2.7",
+          "Programming Language :: Python :: 3.10",
+          "Operating System :: OS Independent",
+          "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
       ],
       keywords='',
       author='IMIO',
       author_email='support@imio.be',
       url='https://github.com/collective/',
       license='gpl',
       packages=find_packages('src'),
```

### Comparing `collective.ckeditortemplates-0.3.3/README.rst` & `collective.ckeditortemplates-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `collective.ckeditortemplates-0.3.3/CHANGES.rst` & `collective.ckeditortemplates-0.9.0/CHANGES.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+0.9.0 (2023-05-23)
+------------------
+
+- Made compatible Plone 4.3 and Plone 6.0
+  [sgeulette]
+
 0.3.3 (2021-04-20)
 ------------------
 
 - Add Transifex.net service integration to manage the translation process.
   [macagua]
 - Add Spanish translation
   [macagua]
```

### Comparing `collective.ckeditortemplates-0.3.3/src/collective.ckeditortemplates.egg-info/SOURCES.txt` & `collective.ckeditortemplates-0.9.0/src/collective.ckeditortemplates.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -36,17 +36,22 @@
 src/collective/ckeditortemplates/locales/fr/LC_MESSAGES/collective.ckeditortemplates.po
 src/collective/ckeditortemplates/locales/fr/LC_MESSAGES/plone.po
 src/collective/ckeditortemplates/locales/nl/LC_MESSAGES/collective.ckeditortemplates.po
 src/collective/ckeditortemplates/locales/nl/LC_MESSAGES/plone.po
 src/collective/ckeditortemplates/profiles/default/collective.ckeditortemplates_various.txt
 src/collective/ckeditortemplates/profiles/default/controlpanel.xml
 src/collective/ckeditortemplates/profiles/default/metadata.xml
-src/collective/ckeditortemplates/profiles/default/propertiestool.xml
 src/collective/ckeditortemplates/profiles/default/types.xml
 src/collective/ckeditortemplates/profiles/default/workflows.xml
 src/collective/ckeditortemplates/profiles/default/types/cktemplate.xml
 src/collective/ckeditortemplates/profiles/default/types/cktemplatefolder.xml
 src/collective/ckeditortemplates/profiles/default/workflows/cktemplate_workflow/definition.xml
+src/collective/ckeditortemplates/profiles/plone4/collective.ckeditortemplates_various.txt
+src/collective/ckeditortemplates/profiles/plone4/metadata.xml
+src/collective/ckeditortemplates/profiles/plone4/propertiestool.xml
+src/collective/ckeditortemplates/profiles/plone6/collective.ckeditortemplates_various.txt
+src/collective/ckeditortemplates/profiles/plone6/metadata.xml
+src/collective/ckeditortemplates/profiles/plone6/registry.xml
 src/collective/ckeditortemplates/tests/__init__.py
 src/collective/ckeditortemplates/tests/test.robot
 src/collective/ckeditortemplates/tests/test_cktemplate.py
 src/collective/ckeditortemplates/tests/test_robot.py
```

### Comparing `collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/upgrades.py` & `collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/upgrades.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # -*- coding: utf-8 -*-
-from Products.CMFCore.utils import getToolByName
+from collective.ckeditortemplates import PLONE_VERSION
 from plone import api
 from plone.app.dexterity.behaviors.exclfromnav import IExcludeFromNavigation
+from Products.CMFCore.utils import getToolByName
+
 
 PROFILE = 'profile-collective.ckeditortemplates:default'
 FOLDER = 'ckeditortemplates'
 
 
 def install_folder(site):
     folder = site.get(FOLDER)
@@ -33,16 +35,22 @@
 
 def add_dx_language_behavior(context):
     setup = getToolByName(context, 'portal_setup')
     setup.runAllImportStepsFromProfile(PROFILE)
 
 
 def remove_dx_language_behavior(context):
-    installer = api.portal.get_tool('portal_quickinstaller')
-    if installer.isProductInstalled('plone.multilingualbehavior'):
-        installer.uninstallProducts(['plone.multilingualbehavior'])
+    if PLONE_VERSION >= '5.1':
+        from Products.CMFPlone.utils import get_installer  # noqa
+        installer = get_installer(context)
+        if installer.is_product_installed('plone.multilingualbehavior'):
+            installer.uninstall_product('plone.multilingualbehavior')
+    else:
+        installer = api.portal.get_tool('portal_quickinstaller')  # noqa
+        if installer.isProductInstalled('plone.multilingualbehavior'):
+            installer.uninstallProducts(['plone.multilingualbehavior'])
 
 
 def update_workflow(context):
     context.runImportStepFromProfile(PROFILE, 'workflow')
     portal_workflow = api.portal.get_tool(name='portal_workflow')
     portal_workflow.updateRoleMappings()
```

### Comparing `collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/testing.py` & `collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/testing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 # encoding: utf-8
-from plone.app.testing import PloneSandboxLayer
+from plone import api
+from plone.app.robotframework.testing import AUTOLOGIN_LIBRARY_FIXTURE
 from plone.app.testing import applyProfile
-from plone.app.testing import PLONE_FIXTURE
-from plone.app.testing import IntegrationTesting
 from plone.app.testing import FunctionalTesting
-
-from plone.app.robotframework.testing import AUTOLOGIN_LIBRARY_FIXTURE
-
-from plone import api
+from plone.app.testing import IntegrationTesting
+from plone.app.testing import PLONE_FIXTURE
+from plone.app.testing import PloneSandboxLayer
 from plone.testing import z2
-
 from zope.configuration import xmlconfig
 
 
 class CollectiveCKTemplatesLayer(PloneSandboxLayer):
 
     defaultBases = (PLONE_FIXTURE,)
```

### Comparing `collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/setuphandlers.py` & `collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/setuphandlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 from plone import api
-from Products.CMFCore.utils import getToolByName
 from plone.app.dexterity.behaviors.exclfromnav import IExcludeFromNavigation
+from Products.CMFCore.utils import getToolByName
+
 
 FOLDER = "ckeditortemplates"
 
 
 def setupVarious(context):
     site = context.getSite()
     if context.readDataFile('collective.ckeditortemplates_various.txt') is None:
```

### Comparing `collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/profiles.zcml` & `collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/profiles.zcml`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,47 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
     xmlns:genericsetup="http://namespaces.zope.org/genericsetup"
+    xmlns:zcml="http://namespaces.zope.org/zcml"
     i18n_domain="collective.ckeditortemplates">
 
+  <genericsetup:registerProfile
+      name="install-base"
+      title="collective.ckeditortemplates base"
+      directory="profiles/default"
+      description="Base of collective.ckeditortemplates package: do not select, use other installation package"
+      provides="Products.GenericSetup.interfaces.EXTENSION"
+      />
+
+  <genericsetup:registerProfile
+      zcml:condition="not-have plone-5"
+      name="default"
+      title="collective.ckeditortemplates installation"
+      directory="profiles/plone4"
+      description="Installs the collective.ckeditortemplates package for Plone 4"
+      provides="Products.GenericSetup.interfaces.EXTENSION"
+      />
+
+  <genericsetup:registerProfile
+      zcml:condition="have plone-60"
+      name="default"
+      title="collective.ckeditortemplates installation"
+      directory="profiles/plone6"
+      description="Installs the collective.ckeditortemplates package for Plone 6"
+      provides="Products.GenericSetup.interfaces.EXTENSION"
+      />
+
   <genericsetup:importStep
       name="collective.ckeditortemplates"
       title="collective.ckeditortemplates: miscellaneous import steps"
       description="Various import steps that are not handled by GS import/export handlers."
       handler="collective.ckeditortemplates.setuphandlers.setupVarious">
       <depends name="typeinfo"/>
   </genericsetup:importStep>
 
-
   <genericsetup:upgradeStep
       title="Disable global allow for ckeditortemplates folder"
       description="Disable global allow for ckeditortemplates folder"
       source="*"
       destination="0002"
       handler=".upgrades.update_content_folder"
       profile="collective.ckeditortemplates:default" />
```

### Comparing `collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/configure.zcml` & `collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/configure.zcml`

 * *Files 11% similar despite different names*

```diff
@@ -11,22 +11,14 @@
   <include file="profiles.zcml" />
 
   <include package="plone.app.dexterity" />
   <include package="plone.supermodel" />
 
   <include package=".browser" />
 
-  <genericsetup:registerProfile
-      name="default"
-      title="collective.ckeditortemplates"
-      directory="profiles/default"
-      description="Installs the collective.ckeditortemplates package"
-      provides="Products.GenericSetup.interfaces.EXTENSION"
-      />
-
   <utility factory=".cktemplate.CKTemplateSchemaPolicy"
            name="schema_policy_cktemplate" />
 
   <utility factory=".cktemplate.CKTemplateFolderSchemaPolicy"
            name="schema_policy_cktemplatefolder" />
 
   <browser:resource
```

### Comparing `collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/cktemplatefolder_icon.gif` & `collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/cktemplatefolder_icon.gif`

 * *Files identical despite different names*

### Comparing `collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/cktemplate_icon.gif` & `collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/cktemplate_icon.gif`

 * *Files identical despite different names*

### Comparing `collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/cktemplate.py` & `collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/cktemplate.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,26 +5,28 @@
 from plone.app.contenttypes.content import Folder
 from plone.app.contenttypes.interfaces import IDocument
 from plone.app.contenttypes.interfaces import IFolder
 from plone.app.textfield import RichText
 from plone.dexterity.schema import DexteritySchemaPolicy
 from plone.namedfile.field import NamedImage
 from plone.supermodel import model
+from Products.CMFPlone.utils import safe_unicode
 from zope.i18nmessageid import MessageFactory
-from zope.interface import implements
+from zope.interface import implementer
+
 
 PMF = MessageFactory('plone')
 
 
 class ICKTemplateFolder(model.Schema, IFolder):
     """ Schema for CKEditor template folder """
 
 
+@implementer(ICKTemplateFolder)
 class CKTemplateFolder(Folder):
-    implements(ICKTemplateFolder)
 
     # This method is used by index methods.
     # If None is returned, the linked content type is not catalogued
     def _getCatalogTool(self):
         return None
 
 
@@ -43,37 +45,35 @@
                              required=False)
 
     content = RichText(title=_(u'Template content'),
                        description=_(u"The content that will be pasted when the template is used"),
                        required=True)
 
 
+@implementer(ICKTemplate)
 class CKTemplate(Document):
-    implements(ICKTemplate)
 
-    @property
     def image(self):
         return (u"view/++widget++form.widgets.custom_icon/@@download/%s" %
                 self.custom_icon.filename)
 
-    @property
     def html(self):
         soup = BeautifulSoup(self.content.raw, features='lxml')
         soup.html.hidden = True
         soup.body.hidden = True
 
         # Replace quotes in contents
         for element in soup.findAll(text=True):
-            text = unicode(element)
+            text = safe_unicode(element)
             text = text.replace(u'"', u'U+0022')
             text = text.strip()
             element.replaceWith(text)
         # Remove new lines an carriage returns
         content = ''.join(str(soup).splitlines())
-        content = content.decode('utf-8')
+        content = safe_unicode(content)
         content = content.replace('"', "'")
         content = content.replace(u'U+0022', u'&quot;')
         return content.strip()
 
 
 class CKTemplateSchemaPolicy(DexteritySchemaPolicy):
     """ Schema Policy for CKTemplate """
```

### Comparing `collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/tests/test_cktemplate.py` & `collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/tests/test_cktemplate.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # encoding: utf-8
-import unittest
+from collective.ckeditortemplates import cktemplate
+from collective.ckeditortemplates.testing import CKTEMPLATES_INTEGRATION_TESTING
 
-from .. import cktemplate
-from ..testing import CKTEMPLATES_INTEGRATION_TESTING
+import unittest
 
 
 class TestCKTemplate(unittest.TestCase):
     layer = CKTEMPLATES_INTEGRATION_TESTING
 
     def test_html_simple(self):
         template = cktemplate.CKTemplate()
         content = """<h1>My title</h1><p>Lorem ipsum dolor..."""
         template.content = type('content', (object, ), {'raw': content})
         html = """<h1>My title</h1><p>Lorem ipsum dolor...</p>"""
-        self.assertEqual(html, template.html)
+        self.assertEqual(html, template.html())
 
     def test_html_complex(self):
         template = cktemplate.CKTemplate()
         content = """<p class="a">text1'<a href="b">"text2"</a></p>"""
         template.content = type('content', (object, ), {'raw': content})
         html = """<p class='a'>text1'<a href='b'>&quot;text2&quot;</a></p>"""
-        self.assertEqual(html, template.html)
+        self.assertEqual(html, template.html())
```

### Comparing `collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/tests/test.robot` & `collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/tests/test.robot`

 * *Files identical despite different names*

### Comparing `collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/profiles/default/workflows/cktemplate_workflow/definition.xml` & `collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/profiles/default/workflows/cktemplate_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/profiles/default/types/cktemplatefolder.xml` & `collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/profiles/default/types/cktemplatefolder.xml`

 * *Files identical despite different names*

### Comparing `collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/profiles/default/types/cktemplate.xml` & `collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/profiles/default/types/cktemplate.xml`

 * *Files identical despite different names*

### Comparing `collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/locales/nl/LC_MESSAGES/plone.po` & `collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/locales/en/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/locales/nl/LC_MESSAGES/collective.ckeditortemplates.po` & `collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/locales/en/LC_MESSAGES/collective.ckeditortemplates.po`

 * *Files identical despite different names*

### Comparing `collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/locales/fr/LC_MESSAGES/plone.po` & `collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/locales/fr/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/locales/fr/LC_MESSAGES/collective.ckeditortemplates.po` & `collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/locales/fr/LC_MESSAGES/collective.ckeditortemplates.po`

 * *Files identical despite different names*

### Comparing `collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/locales/es/LC_MESSAGES/plone.po` & `collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/locales/es/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/locales/es/LC_MESSAGES/collective.ckeditortemplates.po` & `collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/locales/es/LC_MESSAGES/collective.ckeditortemplates.po`

 * *Files identical despite different names*

### Comparing `collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/locales/en/LC_MESSAGES/plone.po` & `collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/locales/nl/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/locales/en/LC_MESSAGES/collective.ckeditortemplates.po` & `collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/locales/nl/LC_MESSAGES/collective.ckeditortemplates.po`

 * *Files identical despite different names*

### Comparing `collective.ckeditortemplates-0.3.3/src/collective/ckeditortemplates/browser/cktemplatelisting.py` & `collective.ckeditortemplates-0.9.0/src/collective/ckeditortemplates/browser/cktemplatelisting.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,13 +39,13 @@
     def render_template(self, template, path):
         """Render each template as a javascript dic."""
         base = ('{title: "%(title)s", %(image)s'
                 'description: "%(description)s", '
                 'html: "%(html)s"}')
         icon = ''
         if template.custom_icon is not None:
-            icon = 'image: "%s/%s", ' % (path, template.image)
+            icon = 'image: "%s/%s", ' % (path, template.image())
         return base % {
             u'title': template.title.replace('"', '&quot;'),
             u'image': icon,
             u'description': template.description.replace('"', '&quot;'),
-            u'html': template.html}
+            u'html': template.html()}
```

### Comparing `collective.ckeditortemplates-0.3.3/docs/LICENSE.rst` & `collective.ckeditortemplates-0.9.0/docs/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `collective.ckeditortemplates-0.3.3/docs/LICENSE.GPL` & `collective.ckeditortemplates-0.9.0/docs/LICENSE.GPL`

 * *Files identical despite different names*

