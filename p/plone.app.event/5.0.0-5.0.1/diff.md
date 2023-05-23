# Comparing `tmp/plone.app.event-5.0.0.tar.gz` & `tmp/plone.app.event-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.event-5.0.0.tar", last modified: Thu Apr  6 10:25:04 2023, max compression
+gzip compressed data, was "plone.app.event-5.0.1.tar", last modified: Sat Apr 15 10:18:36 2023, max compression
```

## Comparing `plone.app.event-5.0.0.tar` & `plone.app.event-5.0.1.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:25:04.860607 plone.app.event-5.0.0/
--rw-r--r--   0 maurits    (501) staff       (20)    57393 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)    18099 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      756 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/LICENSE.rst
--rw-r--r--   0 maurits    (501) staff       (20)      202 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    61766 2023-04-06 10:25:04.860881 plone.app.event-5.0.0/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      675 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:25:04.828627 plone.app.event-5.0.0/docs/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:25:04.829798 plone.app.event-5.0.0/docs/api/
--rw-r--r--   0 maurits    (501) staff       (20)       94 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/docs/api/base.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:25:04.831254 plone.app.event-5.0.0/docs/api/browser/
--rw-r--r--   0 maurits    (501) staff       (20)      145 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/docs/api/browser/event_listing.rst
--rw-r--r--   0 maurits    (501) staff       (20)      146 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/docs/api/browser/event_summary.rst
--rw-r--r--   0 maurits    (501) staff       (20)      136 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/docs/api/browser/event_view.rst
--rw-r--r--   0 maurits    (501) staff       (20)      148 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/docs/api/browser/formatted_date.rst
--rw-r--r--   0 maurits    (501) staff       (20)      158 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/docs/api/browser/leadimage_viewlet.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:25:04.832107 plone.app.event-5.0.0/docs/api/dx/
--rw-r--r--   0 maurits    (501) staff       (20)      118 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/docs/api/dx/behaviors.rst
--rw-r--r--   0 maurits    (501) staff       (20)      121 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/docs/api/dx/interfaces.rst
--rw-r--r--   0 maurits    (501) staff       (20)      119 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/docs/api/dx/traverser.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:25:04.832680 plone.app.event-5.0.0/docs/api/ical/
--rw-r--r--   0 maurits    (501) staff       (20)      122 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/docs/api/ical/exporter.rst
--rw-r--r--   0 maurits    (501) staff       (20)      121 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/docs/api/ical/importer.rst
--rw-r--r--   0 maurits    (501) staff       (20)      403 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/docs/api/index.rst
--rw-r--r--   0 maurits    (501) staff       (20)      112 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/docs/api/interfaces.rst
--rw-r--r--   0 maurits    (501) staff       (20)      113 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/docs/api/recurrence.rst
--rw-r--r--   0 maurits    (501) staff       (20)     5633 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/docs/architectural-overview.rst
--rw-r--r--   0 maurits    (501) staff       (20)      395 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/docs/conf.py
--rw-r--r--   0 maurits    (501) staff       (20)     3464 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/docs/designchoices.rst
--rw-r--r--   0 maurits    (501) staff       (20)    10346 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/docs/development.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1590 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/docs/index.rst
--rw-r--r--   0 maurits    (501) staff       (20)     2839 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/docs/installation.rst
--rw-r--r--   0 maurits    (501) staff       (20)      884 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/docs/tests.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:25:04.832969 plone.app.event-5.0.0/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:25:04.835400 plone.app.event-5.0.0/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:25:04.838394 plone.app.event-5.0.0/plone/app/event/
--rw-r--r--   0 maurits    (501) staff       (20)      369 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)    33277 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/base.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:25:04.841789 plone.app.event-5.0.0/plone/app/event/browser/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3398 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     5435 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/browser/event_listing.pt
--rw-r--r--   0 maurits    (501) staff       (20)    15434 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/browser/event_listing.py
--rw-r--r--   0 maurits    (501) staff       (20)     9639 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/browser/event_summary.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2965 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/browser/event_summary.py
--rw-r--r--   0 maurits    (501) staff       (20)     1931 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/browser/event_view.pt
--rw-r--r--   0 maurits    (501) staff       (20)      605 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/browser/event_view.py
--rw-r--r--   0 maurits    (501) staff       (20)     3228 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/browser/formatted_date.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1001 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/browser/formatted_date.py
--rw-r--r--   0 maurits    (501) staff       (20)      726 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/browser/formatted_start_date.pt
--rw-r--r--   0 maurits    (501) staff       (20)      550 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/browser/leadimage_viewlet.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:25:04.842345 plone.app.event-5.0.0/plone/app/event/browser/resources/
--rw-r--r--   0 maurits    (501) staff       (20)      349 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/browser/resources/calendar.svg
--rw-r--r--   0 maurits    (501) staff       (20)     3726 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/browser/resources/event.js
--rw-r--r--   0 maurits    (501) staff       (20)     2121 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/configure.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:25:04.843998 plone.app.event-5.0.0/plone/app/event/dx/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/dx/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)    14257 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/dx/behaviors.py
--rw-r--r--   0 maurits    (501) staff       (20)     1981 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/dx/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      585 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/dx/ical.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      274 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/dx/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      759 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/dx/traverser.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:25:04.845142 plone.app.event-5.0.0/plone/app/event/ical/
--rw-r--r--   0 maurits    (501) staff       (20)      430 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/ical/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3135 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/ical/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    14653 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/ical/exporter.py
--rw-r--r--   0 maurits    (501) staff       (20)    14459 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/ical/importer.py
--rw-r--r--   0 maurits    (501) staff       (20)      350 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      171 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/permissions.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:25:04.846879 plone.app.event-5.0.0/plone/app/event/portlets/
--rw-r--r--   0 maurits    (501) staff       (20)      767 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/portlets/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      836 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/portlets/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     4035 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/portlets/portlet_calendar.pt
--rw-r--r--   0 maurits    (501) staff       (20)    11194 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/portlets/portlet_calendar.py
--rw-r--r--   0 maurits    (501) staff       (20)     3357 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/portlets/portlet_events.pt
--rw-r--r--   0 maurits    (501) staff       (20)     8198 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/portlets/portlet_events.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:25:04.822520 plone.app.event-5.0.0/plone/app/event/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:25:04.849512 plone.app.event-5.0.0/plone/app/event/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)     2651 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/profiles/default/actions.xml
--rw-r--r--   0 maurits    (501) staff       (20)      157 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/profiles/default/browserlayer.xml
--rw-r--r--   0 maurits    (501) staff       (20)      357 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/profiles/default/controlpanel.xml
--rw-r--r--   0 maurits    (501) staff       (20)      321 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)        2 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/profiles/default/plone.app.event-default.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1194 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/profiles/default/portlets.xml
--rw-r--r--   0 maurits    (501) staff       (20)      486 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/profiles/default/registry.xml
--rw-r--r--   0 maurits    (501) staff       (20)      328 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/profiles/default/rolemap.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:25:04.850349 plone.app.event-5.0.0/plone/app/event/profiles/default/types/
--rw-r--r--   0 maurits    (501) staff       (20)      190 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/profiles/default/types/Collection.xml
--rw-r--r--   0 maurits    (501) staff       (20)      186 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/profiles/default/types/Folder.xml
--rw-r--r--   0 maurits    (501) staff       (20)      190 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/profiles/default/types/Plone_Site.xml
--rw-r--r--   0 maurits    (501) staff       (20)      355 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/profiles/default/types.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:25:04.850875 plone.app.event-5.0.0/plone/app/event/profiles/testing/
--rw-r--r--   0 maurits    (501) staff       (20)      181 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/profiles/testing/metadata.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:25:04.851157 plone.app.event-5.0.0/plone/app/event/profiles/testing/types/
--rw-r--r--   0 maurits    (501) staff       (20)     2850 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/profiles/testing/types/plone.app.event.dx.event.xml
--rw-r--r--   0 maurits    (501) staff       (20)      199 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/profiles/testing/types.xml
--rw-r--r--   0 maurits    (501) staff       (20)     6714 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/recurrence.py
--rw-r--r--   0 maurits    (501) staff       (20)      567 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/recurrence.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2462 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/setuphandlers.py
--rw-r--r--   0 maurits    (501) staff       (20)     3694 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:25:04.855788 plone.app.event-5.0.0/plone/app/event/tests/
--rw-r--r--   0 maurits    (501) staff       (20)      898 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/tests/INACTIVE_test_robot.py
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     5753 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/tests/base_setup.py
--rw-r--r--   0 maurits    (501) staff       (20)     2201 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/tests/icaltest.ics
--rw-r--r--   0 maurits    (501) staff       (20)     2202 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/tests/icaltest2.ics
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:25:04.856571 plone.app.event-5.0.0/plone/app/event/tests/javascripts/
--rw-r--r--   0 maurits    (501) staff       (20)    23860 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/tests/javascripts/test_event.html
--rw-r--r--   0 maurits    (501) staff       (20)      715 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/tests/javascripts/test_event.js
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:25:04.857396 plone.app.event-5.0.0/plone/app/event/tests/qunit/
--rw-r--r--   0 maurits    (501) staff       (20)     3952 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/tests/qunit/qunit.css
--rw-r--r--   0 maurits    (501) staff       (20)    37060 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/tests/qunit/qunit.js
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:25:04.858485 plone.app.event-5.0.0/plone/app/event/tests/robot/
--rw-r--r--   0 maurits    (501) staff       (20)     6114 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/tests/robot/test_event_roundtrip.robot
--rw-r--r--   0 maurits    (501) staff       (20)      633 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/tests/robot/variables.py
--rw-r--r--   0 maurits    (501) staff       (20)    35328 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/tests/test_base_module.py
--rw-r--r--   0 maurits    (501) staff       (20)      773 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/tests/test_catalog.py
--rw-r--r--   0 maurits    (501) staff       (20)    22380 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/tests/test_dx_behaviors.py
--rw-r--r--   0 maurits    (501) staff       (20)     6395 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/tests/test_event_listing.py
--rw-r--r--   0 maurits    (501) staff       (20)     4982 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/tests/test_event_summary.py
--rw-r--r--   0 maurits    (501) staff       (20)     2075 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/tests/test_event_view.py
--rw-r--r--   0 maurits    (501) staff       (20)     3583 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/tests/test_ical_import.py
--rw-r--r--   0 maurits    (501) staff       (20)    19302 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/tests/test_icalendar.py
--rw-r--r--   0 maurits    (501) staff       (20)     9253 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/tests/test_portlet_calendar.py
--rw-r--r--   0 maurits    (501) staff       (20)     8861 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/tests/test_portlet_events.py
--rw-r--r--   0 maurits    (501) staff       (20)    13916 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/tests/test_recurrence.py
--rw-r--r--   0 maurits    (501) staff       (20)      544 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/tests/test_search.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:25:04.859728 plone.app.event-5.0.0/plone/app/event/upgrades/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/upgrades/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      969 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/upgrades/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     3415 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/upgrades/upgrades.py
--rw-r--r--   0 maurits    (501) staff       (20)     1261 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone/app/event/vocabularies.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:25:04.835115 plone.app.event-5.0.0/plone.app.event.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    61766 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone.app.event.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     4246 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone.app.event.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone.app.event.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone.app.event.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone.app.event.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      828 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone.app.event.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/plone.app.event.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1732 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      276 2023-04-06 10:25:04.861704 plone.app.event-5.0.0/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2721 2023-04-06 10:25:04.000000 plone.app.event-5.0.0/setup.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.486230 plone.app.event-5.0.1/
+-rw-r--r--   0 gil       (1000) gil       (1000)    57519 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/CHANGES.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)       70 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/CONTRIBUTING.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)    18099 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/LICENSE.GPL
+-rw-r--r--   0 gil       (1000) gil       (1000)      756 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/LICENSE.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      202 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/MANIFEST.in
+-rw-r--r--   0 gil       (1000) gil       (1000)    61804 2023-04-15 10:18:36.486230 plone.app.event-5.0.1/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)      587 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/README.rst
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.475229 plone.app.event-5.0.1/docs/
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.476229 plone.app.event-5.0.1/docs/api/
+-rw-r--r--   0 gil       (1000) gil       (1000)       94 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/docs/api/base.rst
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.476229 plone.app.event-5.0.1/docs/api/browser/
+-rw-r--r--   0 gil       (1000) gil       (1000)      145 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/docs/api/browser/event_listing.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      146 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/docs/api/browser/event_summary.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      136 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/docs/api/browser/event_view.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      148 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/docs/api/browser/formatted_date.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      158 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/docs/api/browser/leadimage_viewlet.rst
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.477229 plone.app.event-5.0.1/docs/api/dx/
+-rw-r--r--   0 gil       (1000) gil       (1000)      118 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/docs/api/dx/behaviors.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      121 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/docs/api/dx/interfaces.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      119 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/docs/api/dx/traverser.rst
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.477229 plone.app.event-5.0.1/docs/api/ical/
+-rw-r--r--   0 gil       (1000) gil       (1000)      122 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/docs/api/ical/exporter.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      121 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/docs/api/ical/importer.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      403 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/docs/api/index.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      112 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/docs/api/interfaces.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      113 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/docs/api/recurrence.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)     5633 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/docs/architectural-overview.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      395 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/docs/conf.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3464 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/docs/designchoices.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)    10346 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/docs/development.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)     1590 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/docs/index.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)     2839 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/docs/installation.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      884 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/docs/tests.rst
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.477229 plone.app.event-5.0.1/plone/
+-rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.478229 plone.app.event-5.0.1/plone/app/
+-rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.479229 plone.app.event-5.0.1/plone/app/event/
+-rw-r--r--   0 gil       (1000) gil       (1000)      369 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    33259 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/base.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.480229 plone.app.event-5.0.1/plone/app/event/browser/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/browser/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3398 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/browser/configure.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)     5435 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/browser/event_listing.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)    15434 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/browser/event_listing.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     9639 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/browser/event_summary.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)     2965 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/browser/event_summary.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1931 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/browser/event_view.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)      605 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/browser/event_view.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3228 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/browser/formatted_date.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)     1001 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/browser/formatted_date.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      726 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/browser/formatted_start_date.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)      550 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/browser/leadimage_viewlet.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.480229 plone.app.event-5.0.1/plone/app/event/browser/resources/
+-rw-r--r--   0 gil       (1000) gil       (1000)      349 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/browser/resources/calendar.svg
+-rw-r--r--   0 gil       (1000) gil       (1000)     3726 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/browser/resources/event.js
+-rw-r--r--   0 gil       (1000) gil       (1000)     2121 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/configure.zcml
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.481229 plone.app.event-5.0.1/plone/app/event/dx/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/dx/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    14257 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/dx/behaviors.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1981 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/dx/configure.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)      585 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/dx/ical.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)      274 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/dx/interfaces.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      759 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/dx/traverser.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.481229 plone.app.event-5.0.1/plone/app/event/ical/
+-rw-r--r--   0 gil       (1000) gil       (1000)      430 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/ical/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3135 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/ical/configure.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)    14653 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/ical/exporter.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    14459 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/ical/importer.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      350 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/interfaces.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      171 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/permissions.zcml
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.482229 plone.app.event-5.0.1/plone/app/event/portlets/
+-rw-r--r--   0 gil       (1000) gil       (1000)      767 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/portlets/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      836 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/portlets/configure.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)     4035 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/portlets/portlet_calendar.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)    11194 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/portlets/portlet_calendar.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3357 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/portlets/portlet_events.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)     8198 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/portlets/portlet_events.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.473229 plone.app.event-5.0.1/plone/app/event/profiles/
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.483229 plone.app.event-5.0.1/plone/app/event/profiles/default/
+-rw-r--r--   0 gil       (1000) gil       (1000)     2651 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/profiles/default/actions.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)      157 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/profiles/default/browserlayer.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)      357 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/profiles/default/controlpanel.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)      321 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/profiles/default/metadata.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)        2 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/profiles/default/plone.app.event-default.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)     1194 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/profiles/default/portlets.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)      479 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/profiles/default/registry.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)      328 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/profiles/default/rolemap.xml
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.483229 plone.app.event-5.0.1/plone/app/event/profiles/default/types/
+-rw-r--r--   0 gil       (1000) gil       (1000)      190 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/profiles/default/types/Collection.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)      186 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/profiles/default/types/Folder.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)      190 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/profiles/default/types/Plone_Site.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)      355 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/profiles/default/types.xml
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.483229 plone.app.event-5.0.1/plone/app/event/profiles/testing/
+-rw-r--r--   0 gil       (1000) gil       (1000)      181 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/profiles/testing/metadata.xml
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.483229 plone.app.event-5.0.1/plone/app/event/profiles/testing/types/
+-rw-r--r--   0 gil       (1000) gil       (1000)     2850 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/profiles/testing/types/plone.app.event.dx.event.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)      199 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/profiles/testing/types.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)     6714 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/recurrence.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      567 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/recurrence.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)     2462 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/setuphandlers.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3694 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/testing.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.485229 plone.app.event-5.0.1/plone/app/event/tests/
+-rw-r--r--   0 gil       (1000) gil       (1000)      898 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/tests/INACTIVE_test_robot.py
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/tests/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     5753 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/tests/base_setup.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2201 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/tests/icaltest.ics
+-rw-r--r--   0 gil       (1000) gil       (1000)     2202 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/tests/icaltest2.ics
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.485229 plone.app.event-5.0.1/plone/app/event/tests/javascripts/
+-rw-r--r--   0 gil       (1000) gil       (1000)    23860 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/tests/javascripts/test_event.html
+-rw-r--r--   0 gil       (1000) gil       (1000)      715 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/tests/javascripts/test_event.js
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.485229 plone.app.event-5.0.1/plone/app/event/tests/qunit/
+-rw-r--r--   0 gil       (1000) gil       (1000)     3952 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/tests/qunit/qunit.css
+-rw-r--r--   0 gil       (1000) gil       (1000)    37060 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/tests/qunit/qunit.js
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.486230 plone.app.event-5.0.1/plone/app/event/tests/robot/
+-rw-r--r--   0 gil       (1000) gil       (1000)     6114 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/tests/robot/test_event_roundtrip.robot
+-rw-r--r--   0 gil       (1000) gil       (1000)      633 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/tests/robot/variables.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    35328 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/tests/test_base_module.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      773 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/tests/test_catalog.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    22380 2023-04-15 10:18:36.000000 plone.app.event-5.0.1/plone/app/event/tests/test_dx_behaviors.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     6395 2023-04-15 10:18:36.000000 plone.app.event-5.0.1/plone/app/event/tests/test_event_listing.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     4982 2023-04-15 10:18:36.000000 plone.app.event-5.0.1/plone/app/event/tests/test_event_summary.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2075 2023-04-15 10:18:36.000000 plone.app.event-5.0.1/plone/app/event/tests/test_event_view.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3583 2023-04-15 10:18:36.000000 plone.app.event-5.0.1/plone/app/event/tests/test_ical_import.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    19302 2023-04-15 10:18:36.000000 plone.app.event-5.0.1/plone/app/event/tests/test_icalendar.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     9253 2023-04-15 10:18:36.000000 plone.app.event-5.0.1/plone/app/event/tests/test_portlet_calendar.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     8861 2023-04-15 10:18:36.000000 plone.app.event-5.0.1/plone/app/event/tests/test_portlet_events.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    13916 2023-04-15 10:18:36.000000 plone.app.event-5.0.1/plone/app/event/tests/test_recurrence.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      544 2023-04-15 10:18:36.000000 plone.app.event-5.0.1/plone/app/event/tests/test_search.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.486230 plone.app.event-5.0.1/plone/app/event/upgrades/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.000000 plone.app.event-5.0.1/plone/app/event/upgrades/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      969 2023-04-15 10:18:36.000000 plone.app.event-5.0.1/plone/app/event/upgrades/configure.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)     3415 2023-04-15 10:18:36.000000 plone.app.event-5.0.1/plone/app/event/upgrades/upgrades.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1261 2023-04-15 10:18:36.000000 plone.app.event-5.0.1/plone/app/event/vocabularies.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.478229 plone.app.event-5.0.1/plone.app.event.egg-info/
+-rw-r--r--   0 gil       (1000) gil       (1000)    61804 2023-04-15 10:18:36.000000 plone.app.event-5.0.1/plone.app.event.egg-info/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)     4246 2023-04-15 10:18:36.000000 plone.app.event-5.0.1/plone.app.event.egg-info/SOURCES.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 10:18:36.000000 plone.app.event-5.0.1/plone.app.event.egg-info/dependency_links.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)       16 2023-04-15 10:18:36.000000 plone.app.event-5.0.1/plone.app.event.egg-info/namespace_packages.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 10:18:36.000000 plone.app.event-5.0.1/plone.app.event.egg-info/not-zip-safe
+-rw-r--r--   0 gil       (1000) gil       (1000)      711 2023-04-15 10:18:36.000000 plone.app.event-5.0.1/plone.app.event.egg-info/requires.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-15 10:18:36.000000 plone.app.event-5.0.1/plone.app.event.egg-info/top_level.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)     2934 2023-04-15 10:18:36.000000 plone.app.event-5.0.1/pyproject.toml
+-rw-r--r--   0 gil       (1000) gil       (1000)      276 2023-04-15 10:18:36.486230 plone.app.event-5.0.1/setup.cfg
+-rw-r--r--   0 gil       (1000) gil       (1000)     2527 2023-04-15 10:18:36.000000 plone.app.event-5.0.1/setup.py
```

### Comparing `plone.app.event-5.0.0/CHANGES.rst` & `plone.app.event-5.0.1/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+5.0.1 (2023-04-15)
+------------------
+
+Internal:
+
+
+- Update configuration files and dependencies.
+  [plone devs] (0b0246aa)
+
+
 5.0.0 (2023-04-06)
 ------------------
 
 Breaking changes:
 
 
 - Breaking dependency cleanup: Move declaration of language independence of on IEventBasic fields to plone.app.multilingual.
```

### Comparing `plone.app.event-5.0.0/LICENSE.GPL` & `plone.app.event-5.0.1/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/LICENSE.rst` & `plone.app.event-5.0.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/PKG-INFO` & `plone.app.event-5.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.event
-Version: 5.0.0
+Version: 5.0.1
 Summary: The Plone calendar framework
 Home-page: https://github.com/plone/plone.app.event
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: plone event
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,31 +21,33 @@
 Provides-Extra: test
 License-File: LICENSE.GPL
 License-File: LICENSE.rst
 
 plone.app.event
 ===============
 
-Plone.app.event is the calendaring framework for Plone. It provides Dexterity behaviors and an Archetypes type, Timezone support, RFC5545 icalendar export, Recurrence support, event views and a lot more.
+``plone.app.event`` is the calendaring framework for Plone. 
 
-For a Dexterity event type using plone.app.event, use plone.app.contenttypes 1.1 or newer.
+It provides 
 
-The complete documentation can be found on: https://ploneappevent.readthedocs.org
+- Dexterity behaviors, 
+- timezone support, 
+- RFC5545 icalendar export, 
+- recurrence support, 
+- event views 
+- and a lot more.
 
+It is part of the `CMS Plone <https://plone.org>`_ and does not need additional installation steps.
 
-Installation
-------------
-
-For Standalone installation follow the standard buildout procedure::
+Source Code
+===========
 
-    $ virtualenv .
-    $ ./bin/pip install -U zc.buildout setuptools pip
-    $ ./bin/buildout
+Contributors please read the document `Contributing to Plone <https://6.docs.plone.org/contributing/index.html>`_
 
-Note, both commands will install a test and development environment.
+Sources are at the `Plone code repository hosted at Github <https://github.com/plone/plone.dapp.event>`_.
 
 
 Installation
 ============
 
 
 ``plone.app.event`` only provides Dexterity behaviors to build own types based on them.  If you want to install a Dexterity based Event type, you can simply use ``plone.app.contenttypes`` 1.2a3 or up.
@@ -113,14 +115,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+5.0.1 (2023-04-15)
+------------------
+
+Internal:
+
+
+- Update configuration files and dependencies.
+  [plone devs] (0b0246aa)
+
+
 5.0.0 (2023-04-06)
 ------------------
 
 Breaking changes:
 
 
 - Breaking dependency cleanup: Move declaration of language independence of on IEventBasic fields to plone.app.multilingual.
```

### Comparing `plone.app.event-5.0.0/docs/architectural-overview.rst` & `plone.app.event-5.0.1/docs/architectural-overview.rst`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/docs/designchoices.rst` & `plone.app.event-5.0.1/docs/designchoices.rst`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/docs/development.rst` & `plone.app.event-5.0.1/docs/development.rst`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/docs/index.rst` & `plone.app.event-5.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/docs/installation.rst` & `plone.app.event-5.0.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/docs/tests.rst` & `plone.app.event-5.0.1/docs/tests.rst`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/base.py` & `plone.app.event-5.0.1/plone/app/event/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from calendar import monthrange
 from datetime import date
 from datetime import datetime
 from datetime import timedelta
 from DateTime import DateTime
 from persistent.dict import PersistentDict
 from plone.app.event.interfaces import ISO_DATE_FORMAT
-from plone.app.layout.navigation.interfaces import INavigationRoot
-from plone.app.layout.navigation.root import getNavigationRootObject
 from plone.base.i18nl10n import ulocalized_time as orig_ulocalized_time
+from plone.base.interfaces import INavigationRoot
 from plone.base.interfaces.siteroot import IPloneSiteRoot
+from plone.base.navigationroot import get_navigation_root_object
 from plone.base.utils import safe_callable
 from plone.event.interfaces import IEvent
 from plone.event.interfaces import IEventAccessor
 from plone.event.interfaces import IEventRecurrence
 from plone.event.interfaces import IRecurrenceSupport
 from plone.event.utils import default_timezone as fallback_default_timezone
 from plone.event.utils import dt2int
@@ -125,15 +125,15 @@
     query["object_provides"] = IEvent.__identifier__
 
     query.update(start_end_query(start, end))
 
     if "path" not in kw:
         # limit to the current navigation root, usually (not always) site
         portal = getSite()
-        navroot = getNavigationRootObject(context, portal)
+        navroot = get_navigation_root_object(context, portal)
         query["path"] = "/".join(navroot.getPhysicalPath())
     else:
         query["path"] = kw["path"]
 
     # Sorting
     # In expand mode we sort after calculation of recurrences again. But we
     # need to leave this sorting here in place, since no sort definition could
```

### Comparing `plone.app.event-5.0.0/plone/app/event/browser/configure.zcml` & `plone.app.event-5.0.1/plone/app/event/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/browser/event_listing.pt` & `plone.app.event-5.0.1/plone/app/event/browser/event_listing.pt`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/browser/event_listing.py` & `plone.app.event-5.0.1/plone/app/event/browser/event_listing.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/browser/event_summary.pt` & `plone.app.event-5.0.1/plone/app/event/browser/event_summary.pt`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/browser/event_summary.py` & `plone.app.event-5.0.1/plone/app/event/browser/event_summary.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/browser/event_view.pt` & `plone.app.event-5.0.1/plone/app/event/browser/event_view.pt`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/browser/event_view.py` & `plone.app.event-5.0.1/plone/app/event/browser/event_view.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/browser/formatted_date.pt` & `plone.app.event-5.0.1/plone/app/event/browser/formatted_date.pt`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/browser/formatted_date.py` & `plone.app.event-5.0.1/plone/app/event/browser/formatted_date.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/browser/formatted_start_date.pt` & `plone.app.event-5.0.1/plone/app/event/browser/formatted_start_date.pt`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/browser/leadimage_viewlet.py` & `plone.app.event-5.0.1/plone/app/event/browser/leadimage_viewlet.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/browser/resources/event.js` & `plone.app.event-5.0.1/plone/app/event/browser/resources/event.js`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/configure.zcml` & `plone.app.event-5.0.1/plone/app/event/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/dx/behaviors.py` & `plone.app.event-5.0.1/plone/app/event/dx/behaviors.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/dx/configure.zcml` & `plone.app.event-5.0.1/plone/app/event/dx/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/dx/ical.zcml` & `plone.app.event-5.0.1/plone/app/event/dx/ical.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/dx/traverser.py` & `plone.app.event-5.0.1/plone/app/event/dx/traverser.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/ical/configure.zcml` & `plone.app.event-5.0.1/plone/app/event/ical/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/ical/exporter.py` & `plone.app.event-5.0.1/plone/app/event/ical/exporter.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/ical/importer.py` & `plone.app.event-5.0.1/plone/app/event/ical/importer.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/portlets/__init__.py` & `plone.app.event-5.0.1/plone/app/event/portlets/__init__.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/portlets/configure.zcml` & `plone.app.event-5.0.1/plone/app/event/portlets/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/portlets/portlet_calendar.pt` & `plone.app.event-5.0.1/plone/app/event/portlets/portlet_calendar.pt`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/portlets/portlet_calendar.py` & `plone.app.event-5.0.1/plone/app/event/portlets/portlet_calendar.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/portlets/portlet_events.pt` & `plone.app.event-5.0.1/plone/app/event/portlets/portlet_events.pt`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/portlets/portlet_events.py` & `plone.app.event-5.0.1/plone/app/event/portlets/portlet_events.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/profiles/default/actions.xml` & `plone.app.event-5.0.1/plone/app/event/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/profiles/default/portlets.xml` & `plone.app.event-5.0.1/plone/app/event/profiles/default/portlets.xml`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/profiles/testing/types/plone.app.event.dx.event.xml` & `plone.app.event-5.0.1/plone/app/event/profiles/testing/types/plone.app.event.dx.event.xml`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/recurrence.py` & `plone.app.event-5.0.1/plone/app/event/recurrence.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/recurrence.zcml` & `plone.app.event-5.0.1/plone/app/event/recurrence.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/setuphandlers.py` & `plone.app.event-5.0.1/plone/app/event/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/testing.py` & `plone.app.event-5.0.1/plone/app/event/testing.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/tests/INACTIVE_test_robot.py` & `plone.app.event-5.0.1/plone/app/event/tests/INACTIVE_test_robot.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/tests/base_setup.py` & `plone.app.event-5.0.1/plone/app/event/tests/base_setup.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/tests/icaltest.ics` & `plone.app.event-5.0.1/plone/app/event/tests/icaltest.ics`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/tests/icaltest2.ics` & `plone.app.event-5.0.1/plone/app/event/tests/icaltest2.ics`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/tests/javascripts/test_event.html` & `plone.app.event-5.0.1/plone/app/event/tests/javascripts/test_event.html`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/tests/javascripts/test_event.js` & `plone.app.event-5.0.1/plone/app/event/tests/javascripts/test_event.js`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/tests/qunit/qunit.css` & `plone.app.event-5.0.1/plone/app/event/tests/qunit/qunit.css`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/tests/qunit/qunit.js` & `plone.app.event-5.0.1/plone/app/event/tests/qunit/qunit.js`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/tests/robot/test_event_roundtrip.robot` & `plone.app.event-5.0.1/plone/app/event/tests/robot/test_event_roundtrip.robot`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/tests/robot/variables.py` & `plone.app.event-5.0.1/plone/app/event/tests/robot/variables.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/tests/test_base_module.py` & `plone.app.event-5.0.1/plone/app/event/tests/test_base_module.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/tests/test_catalog.py` & `plone.app.event-5.0.1/plone/app/event/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/tests/test_dx_behaviors.py` & `plone.app.event-5.0.1/plone/app/event/tests/test_dx_behaviors.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/tests/test_event_listing.py` & `plone.app.event-5.0.1/plone/app/event/tests/test_event_listing.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/tests/test_event_summary.py` & `plone.app.event-5.0.1/plone/app/event/tests/test_event_summary.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/tests/test_event_view.py` & `plone.app.event-5.0.1/plone/app/event/tests/test_event_view.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/tests/test_ical_import.py` & `plone.app.event-5.0.1/plone/app/event/tests/test_ical_import.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/tests/test_icalendar.py` & `plone.app.event-5.0.1/plone/app/event/tests/test_icalendar.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/tests/test_portlet_calendar.py` & `plone.app.event-5.0.1/plone/app/event/tests/test_portlet_calendar.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/tests/test_portlet_events.py` & `plone.app.event-5.0.1/plone/app/event/tests/test_portlet_events.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/tests/test_recurrence.py` & `plone.app.event-5.0.1/plone/app/event/tests/test_recurrence.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/tests/test_search.py` & `plone.app.event-5.0.1/plone/app/event/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/upgrades/configure.zcml` & `plone.app.event-5.0.1/plone/app/event/upgrades/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/upgrades/upgrades.py` & `plone.app.event-5.0.1/plone/app/event/upgrades/upgrades.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone/app/event/vocabularies.py` & `plone.app.event-5.0.1/plone/app/event/vocabularies.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone.app.event.egg-info/PKG-INFO` & `plone.app.event-5.0.1/plone.app.event.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.event
-Version: 5.0.0
+Version: 5.0.1
 Summary: The Plone calendar framework
 Home-page: https://github.com/plone/plone.app.event
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: plone event
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,31 +21,33 @@
 Provides-Extra: test
 License-File: LICENSE.GPL
 License-File: LICENSE.rst
 
 plone.app.event
 ===============
 
-Plone.app.event is the calendaring framework for Plone. It provides Dexterity behaviors and an Archetypes type, Timezone support, RFC5545 icalendar export, Recurrence support, event views and a lot more.
+``plone.app.event`` is the calendaring framework for Plone. 
 
-For a Dexterity event type using plone.app.event, use plone.app.contenttypes 1.1 or newer.
+It provides 
 
-The complete documentation can be found on: https://ploneappevent.readthedocs.org
+- Dexterity behaviors, 
+- timezone support, 
+- RFC5545 icalendar export, 
+- recurrence support, 
+- event views 
+- and a lot more.
 
+It is part of the `CMS Plone <https://plone.org>`_ and does not need additional installation steps.
 
-Installation
-------------
-
-For Standalone installation follow the standard buildout procedure::
+Source Code
+===========
 
-    $ virtualenv .
-    $ ./bin/pip install -U zc.buildout setuptools pip
-    $ ./bin/buildout
+Contributors please read the document `Contributing to Plone <https://6.docs.plone.org/contributing/index.html>`_
 
-Note, both commands will install a test and development environment.
+Sources are at the `Plone code repository hosted at Github <https://github.com/plone/plone.dapp.event>`_.
 
 
 Installation
 ============
 
 
 ``plone.app.event`` only provides Dexterity behaviors to build own types based on them.  If you want to install a Dexterity based Event type, you can simply use ``plone.app.contenttypes`` 1.2a3 or up.
@@ -113,14 +115,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+5.0.1 (2023-04-15)
+------------------
+
+Internal:
+
+
+- Update configuration files and dependencies.
+  [plone devs] (0b0246aa)
+
+
 5.0.0 (2023-04-06)
 ------------------
 
 Breaking changes:
 
 
 - Breaking dependency cleanup: Move declaration of language independence of on IEventBasic fields to plone.app.multilingual.
```

### Comparing `plone.app.event-5.0.0/plone.app.event.egg-info/SOURCES.txt` & `plone.app.event-5.0.1/plone.app.event.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.0/plone.app.event.egg-info/requires.txt` & `plone.app.event-5.0.1/plone.app.event.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,18 @@
 setuptools
 plone.base
-ExtensionClass
-Products.DateRecurringIndex
 Products.statusmessages
 icalendar
-Products.GenericSetup
+Products.DateRecurringIndex
 Products.ZCatalog
-persistent
 plone.app.contenttypes
 plone.app.uuid
 plone.resource
-zope.annotation
-zope.contentprovider
 plone.app.contentlisting
 plone.app.dexterity
-plone.app.layout
 plone.app.portlets>=2.5.1
 plone.app.querystring
 plone.app.registry
 plone.app.textfield
 plone.app.vocabularies>=2.1.15
 plone.app.z3cform>=2.0.1
 plone.autoform>=1.4
@@ -28,15 +22,14 @@
 plone.event>=1.0
 plone.folder
 plone.formwidget.recurrence[z3cform]>=1.2.4
 plone.indexer
 plone.memoize
 plone.namedfile
 plone.portlets
-plone.registry
 plone.supermodel
 plone.uuid
 plone.z3cform
 pytz
 z3c.form>=3.2.1
 zope.globalrequest
```

### Comparing `plone.app.event-5.0.0/pyproject.toml` & `plone.app.event-5.0.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -44,21 +44,41 @@
 
 [tool.dependencychecker]
 Zope = [
   # Zope own provided namespaces
   'App', 'OFS', 'Products.Five', 'Products.OFSP', 'Products.PageTemplates',
   'Products.SiteAccess', 'Shared', 'Testing', 'ZPublisher', 'ZTUtils',
   'Zope2', 'webdav', 'zmi',
+  # ExtensionClass own provided namespaces
+  'ExtensionClass', 'ComputedAttribute', 'MethodObject',
   # Zope dependencies
-  'Acquisition', 'DateTime', 'transaction', 'zExceptions', 'ZODB', 'zope.component',
-  'zope.configuration', 'zope.container', 'zope.deferredimport', 'zope.event',
-  'zope.exceptions', 'zope.globalrequest', 'zope.i18n', 'zope.i18nmessageid',
-  'zope.interface', 'zope.lifecycleevent', 'zope.location', 'zope.publisher',
-  'zope.schema', 'zope.security', 'zope.site', 'zope.traversing', 'AccessControl',
+  'AccessControl', 'Acquisition', 'AuthEncoding', 'beautifulsoup4', 'BTrees',
+  'cffi', 'Chameleon', 'DateTime', 'DocumentTemplate',
+  'MultiMapping', 'multipart', 'PasteDeploy', 'Persistence', 'persistent',
+  'pycparser', 'python-gettext', 'pytz', 'RestrictedPython', 'roman', 'six',
+  'soupsieve', 'transaction', 'waitress', 'WebOb', 'WebTest', 'WSGIProxy2',
+  'z3c.pt', 'zc.lockfile', 'ZConfig', 'zExceptions', 'ZODB', 'zodbpickle',
+  'zope.annotation', 'zope.browser', 'zope.browsermenu', 'zope.browserpage',
+  'zope.browserresource', 'zope.cachedescriptors', 'zope.component',
+  'zope.configuration', 'zope.container', 'zope.contentprovider',
+  'zope.contenttype', 'zope.datetime', 'zope.deferredimport',
+  'zope.deprecation', 'zope.dottedname', 'zope.event', 'zope.exceptions',
+  'zope.filerepresentation', 'zope.globalrequest', 'zope.hookable',
+  'zope.i18n', 'zope.i18nmessageid', 'zope.interface', 'zope.lifecycleevent',
+  'zope.location', 'zope.pagetemplate', 'zope.processlifetime', 'zope.proxy',
+  'zope.ptresource', 'zope.publisher', 'zope.schema', 'zope.security',
+  'zope.sequencesort', 'zope.site', 'zope.size', 'zope.structuredtext',
+  'zope.tal', 'zope.tales', 'zope.testbrowser', 'zope.testing',
+  'zope.traversing', 'zope.viewlet'
+]
+'Products.CMFCore' = [
+  'docutils', 'five.localsitemanager', 'Missing', 'Products.BTreeFolder2',
+  'Products.GenericSetup', 'Products.MailHost', 'Products.PythonScripts',
+  'Products.StandardCacheManagers', 'Products.ZCatalog', 'Record',
+  'zope.sendmail', 'Zope'
 ]
 'plone.base' = [
-  'AccessControl', 'Products.BTreeFolder2', 'Products.CMFCore',
-  'Products.CMFDynamicViewFTI', 'zope.deprecation',
+  'plone.batching', 'plone.registry', 'plone.schema','plone.z3cform',
+  'Products.CMFCore', 'Products.CMFDynamicViewFTI',
 ]
 python-dateutil = ['dateutil']
-ExtensionClass = ['ComputedAttribute']
-ignore-packages = ['Products.DateRecurringIndex']
+ignore-packages = ['plone.app.layout', 'Products.DateRecurringIndex']
```

### Comparing `plone.app.event-5.0.0/setup.py` & `plone.app.event-5.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages
 from setuptools import setup
 
 import os
 
 
-version = "5.0.0"
+version = "5.0.1"
 
 
 long_description = "\n\n".join(
     [
         open("README.rst").read(),
         open(os.path.join("docs", "installation.rst")).read(),
         open("CHANGES.rst").read(),
@@ -42,29 +42,23 @@
     namespace_packages=["plone", "plone.app"],
     include_package_data=True,
     python_requires=">=3.7",
     zip_safe=False,
     install_requires=[
         "setuptools",
         "plone.base",
-        "ExtensionClass",
-        "Products.DateRecurringIndex",
         "Products.statusmessages",
         "icalendar",  # >4.0.2
-        "Products.GenericSetup",
+        "Products.DateRecurringIndex",
         "Products.ZCatalog",
-        "persistent",
         "plone.app.contenttypes",
         "plone.app.uuid",
         "plone.resource",
-        "zope.annotation",
-        "zope.contentprovider",
         "plone.app.contentlisting",
         "plone.app.dexterity",
-        "plone.app.layout",
         "plone.app.portlets >= 2.5.1",
         "plone.app.querystring",
         "plone.app.registry",
         "plone.app.textfield",
         "plone.app.vocabularies >= 2.1.15",
         "plone.app.z3cform>=2.0.1",
         "plone.autoform>=1.4",
@@ -74,15 +68,14 @@
         "plone.event>=1.0",
         "plone.folder",
         "plone.formwidget.recurrence [z3cform] >= 1.2.4",
         "plone.indexer",
         "plone.memoize",
         "plone.namedfile",
         "plone.portlets",
-        "plone.registry",
         "plone.supermodel",
         "plone.uuid",
         "plone.z3cform",
         "pytz",
         "z3c.form >= 3.2.1",
         "zope.globalrequest",
     ],
```

