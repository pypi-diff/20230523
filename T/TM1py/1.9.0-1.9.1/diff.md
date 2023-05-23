# Comparing `tmp/tm1py-1.9.0.tar.gz` & `tmp/tm1py-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TM1py-1.9.0.tar", last modified: Mon Feb  7 21:49:05 2022, max compression
+gzip compressed data, was "TM1py-1.9.1.tar", last modified: Mon Mar 14 13:50:47 2022, max compression
```

## Comparing `tm1py-1.9.0.tar` & `tm1py-1.9.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxrwx   0        0        0        0 2022-02-07 21:49:05.554701 TM1py-1.9.0/
--rw-rw-rw-   0        0        0     1103 2021-04-22 15:27:27.000000 TM1py-1.9.0/LICENSE
--rw-rw-rw-   0        0        0     4493 2022-02-07 21:49:05.554701 TM1py-1.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     2776 2021-04-22 15:27:27.000000 TM1py-1.9.0/README.md
-drwxrwxrwx   0        0        0        0 2022-02-07 21:49:04.853129 TM1py-1.9.0/TM1py/
-drwxrwxrwx   0        0        0        0 2022-02-07 21:49:04.937756 TM1py-1.9.0/TM1py/Exceptions/
--rw-rw-rw-   0        0        0     2929 2021-04-22 15:27:27.000000 TM1py-1.9.0/TM1py/Exceptions/Exceptions.py
--rw-rw-rw-   0        0        0      207 2021-08-10 11:12:50.000000 TM1py-1.9.0/TM1py/Exceptions/__init__.py
-drwxrwxrwx   0        0        0        0 2022-02-07 21:49:05.286776 TM1py-1.9.0/TM1py/Objects/
--rw-rw-rw-   0        0        0     4897 2021-04-22 15:27:27.000000 TM1py-1.9.0/TM1py/Objects/Annotation.py
--rw-rw-rw-   0        0        0     6868 2021-04-22 15:27:27.000000 TM1py-1.9.0/TM1py/Objects/Application.py
--rw-rw-rw-   0        0        0     3781 2021-04-22 15:27:27.000000 TM1py-1.9.0/TM1py/Objects/Axis.py
--rw-rw-rw-   0        0        0     4577 2021-04-22 15:27:27.000000 TM1py-1.9.0/TM1py/Objects/Chore.py
--rw-rw-rw-   0        0        0     2049 2021-04-22 15:27:27.000000 TM1py-1.9.0/TM1py/Objects/ChoreFrequency.py
--rw-rw-rw-   0        0        0     3343 2021-04-22 15:27:27.000000 TM1py-1.9.0/TM1py/Objects/ChoreStartTime.py
--rw-rw-rw-   0        0        0     2513 2021-04-22 15:27:27.000000 TM1py-1.9.0/TM1py/Objects/ChoreTask.py
--rw-rw-rw-   0        0        0     3188 2021-04-22 15:27:27.000000 TM1py-1.9.0/TM1py/Objects/Cube.py
--rw-rw-rw-   0        0        0     4403 2021-04-22 15:27:27.000000 TM1py-1.9.0/TM1py/Objects/Dimension.py
--rw-rw-rw-   0        0        0     2945 2021-04-22 15:27:27.000000 TM1py-1.9.0/TM1py/Objects/Element.py
--rw-rw-rw-   0        0        0     2403 2021-04-22 15:27:27.000000 TM1py-1.9.0/TM1py/Objects/ElementAttribute.py
--rw-rw-rw-   0        0        0     2313 2021-04-22 15:27:27.000000 TM1py-1.9.0/TM1py/Objects/Git.py
--rw-rw-rw-   0        0        0      685 2021-04-22 15:27:27.000000 TM1py-1.9.0/TM1py/Objects/GitCommit.py
--rw-rw-rw-   0        0        0     2905 2021-04-22 15:27:27.000000 TM1py-1.9.0/TM1py/Objects/GitPlan.py
--rw-rw-rw-   0        0        0      743 2021-04-22 15:27:27.000000 TM1py-1.9.0/TM1py/Objects/GitRemote.py
--rw-rw-rw-   0        0        0     9644 2021-04-22 15:27:27.000000 TM1py-1.9.0/TM1py/Objects/Hierarchy.py
--rw-rw-rw-   0        0        0     1666 2021-04-22 15:27:27.000000 TM1py-1.9.0/TM1py/Objects/MDXView.py
--rw-rw-rw-   0        0        0    10548 2021-04-22 15:27:27.000000 TM1py-1.9.0/TM1py/Objects/NativeView.py
--rw-rw-rw-   0        0        0    19482 2021-04-22 15:27:27.000000 TM1py-1.9.0/TM1py/Objects/Process.py
--rw-rw-rw-   0        0        0     2800 2021-04-22 15:27:27.000000 TM1py-1.9.0/TM1py/Objects/Rules.py
--rw-rw-rw-   0        0        0     2194 2021-04-22 15:27:27.000000 TM1py-1.9.0/TM1py/Objects/Sandbox.py
--rw-rw-rw-   0        0        0     1441 2021-07-27 09:30:20.000000 TM1py-1.9.0/TM1py/Objects/Server.py
--rw-rw-rw-   0        0        0     8595 2021-04-22 15:27:27.000000 TM1py-1.9.0/TM1py/Objects/Subset.py
--rw-rw-rw-   0        0        0      601 2021-04-22 15:27:27.000000 TM1py-1.9.0/TM1py/Objects/TM1Object.py
--rw-rw-rw-   0        0        0     5262 2021-04-22 15:27:27.000000 TM1py-1.9.0/TM1py/Objects/User.py
--rw-rw-rw-   0        0        0      812 2021-04-22 15:27:27.000000 TM1py-1.9.0/TM1py/Objects/View.py
--rw-rw-rw-   0        0        0      995 2021-04-22 15:27:27.000000 TM1py-1.9.0/TM1py/Objects/__init__.py
-drwxrwxrwx   0        0        0        0 2022-02-07 21:49:05.523461 TM1py-1.9.0/TM1py/Services/
--rw-rw-rw-   0        0        0     3513 2021-04-22 15:27:27.000000 TM1py-1.9.0/TM1py/Services/AnnotationService.py
--rw-rw-rw-   0        0        0    12102 2022-02-06 21:03:10.000000 TM1py-1.9.0/TM1py/Services/ApplicationService.py
--rw-rw-rw-   0        0        0   141065 2022-02-06 21:06:25.000000 TM1py-1.9.0/TM1py/Services/CellService.py
--rw-rw-rw-   0        0        0    11531 2022-01-13 16:03:57.000000 TM1py-1.9.0/TM1py/Services/ChoreService.py
--rw-rw-rw-   0        0        0    12717 2022-01-12 08:24:58.000000 TM1py-1.9.0/TM1py/Services/CubeService.py
--rw-rw-rw-   0        0        0     7119 2021-11-22 20:25:23.000000 TM1py-1.9.0/TM1py/Services/DimensionService.py
--rw-rw-rw-   0        0        0    27787 2022-02-04 15:31:08.000000 TM1py-1.9.0/TM1py/Services/ElementService.py
--rw-rw-rw-   0        0        0     9351 2021-04-22 15:27:27.000000 TM1py-1.9.0/TM1py/Services/GitService.py
--rw-rw-rw-   0        0        0    14509 2022-01-24 10:44:29.000000 TM1py-1.9.0/TM1py/Services/HierarchyService.py
--rw-rw-rw-   0        0        0     5700 2021-07-12 14:45:20.000000 TM1py-1.9.0/TM1py/Services/MonitoringService.py
--rw-rw-rw-   0        0        0     1729 2021-04-22 15:27:27.000000 TM1py-1.9.0/TM1py/Services/ObjectService.py
--rw-rw-rw-   0        0        0     6459 2021-07-12 14:45:20.000000 TM1py-1.9.0/TM1py/Services/PowerBiService.py
--rw-rw-rw-   0        0        0    18063 2022-01-12 08:24:58.000000 TM1py-1.9.0/TM1py/Services/ProcessService.py
--rw-rw-rw-   0        0        0    25402 2022-01-02 21:12:17.000000 TM1py-1.9.0/TM1py/Services/RestService.py
--rw-rw-rw-   0        0        0     4273 2021-04-22 15:27:27.000000 TM1py-1.9.0/TM1py/Services/SandboxService.py
--rw-rw-rw-   0        0        0     9519 2021-04-22 15:27:27.000000 TM1py-1.9.0/TM1py/Services/SecurityService.py
--rw-rw-rw-   0        0        0    15954 2022-01-27 19:06:00.000000 TM1py-1.9.0/TM1py/Services/ServerService.py
--rw-rw-rw-   0        0        0     8606 2021-04-22 15:27:27.000000 TM1py-1.9.0/TM1py/Services/SubsetService.py
--rw-rw-rw-   0        0        0     3512 2021-11-12 12:59:40.000000 TM1py-1.9.0/TM1py/Services/TM1Service.py
--rw-rw-rw-   0        0        0     9128 2021-04-22 15:27:27.000000 TM1py-1.9.0/TM1py/Services/ViewService.py
--rw-rw-rw-   0        0        0     1134 2021-04-22 15:27:27.000000 TM1py-1.9.0/TM1py/Services/__init__.py
-drwxrwxrwx   0        0        0        0 2022-02-07 21:49:05.554701 TM1py-1.9.0/TM1py/Utils/
--rw-rw-rw-   0        0        0    10265 2021-04-22 15:27:27.000000 TM1py-1.9.0/TM1py/Utils/MDXUtils.py
--rw-rw-rw-   0        0        0    43313 2022-02-04 15:31:08.000000 TM1py-1.9.0/TM1py/Utils/Utils.py
--rw-rw-rw-   0        0        0       69 2021-04-22 15:27:27.000000 TM1py-1.9.0/TM1py/Utils/__init__.py
--rw-rw-rw-   0        0        0     2818 2021-04-23 09:32:05.000000 TM1py-1.9.0/TM1py/__init__.py
-drwxrwxrwx   0        0        0        0 2022-02-07 21:49:04.906507 TM1py-1.9.0/TM1py.egg-info/
--rw-rw-rw-   0        0        0     4493 2022-02-07 21:49:04.000000 TM1py-1.9.0/TM1py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1693 2022-02-07 21:49:04.000000 TM1py-1.9.0/TM1py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-02-07 21:49:04.000000 TM1py-1.9.0/TM1py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      100 2022-02-07 21:49:04.000000 TM1py-1.9.0/TM1py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       64 2022-02-07 21:49:04.000000 TM1py-1.9.0/TM1py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-02-07 21:49:05.554701 TM1py-1.9.0/setup.cfg
--rw-rw-rw-   0        0        0     1466 2022-01-20 12:20:17.000000 TM1py-1.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2022-03-14 13:50:47.958501 TM1py-1.9.1/
+-rw-rw-rw-   0        0        0     1103 2022-02-14 13:07:33.000000 TM1py-1.9.1/LICENSE
+-rw-rw-rw-   0        0        0     3687 2022-03-14 13:50:47.958501 TM1py-1.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2776 2022-02-14 13:07:33.000000 TM1py-1.9.1/README.md
+drwxrwxrwx   0        0        0        0 2022-03-14 13:50:47.579536 TM1py-1.9.1/TM1py/
+drwxrwxrwx   0        0        0        0 2022-03-14 13:50:47.626405 TM1py-1.9.1/TM1py/Exceptions/
+-rw-rw-rw-   0        0        0     2929 2022-02-14 13:07:33.000000 TM1py-1.9.1/TM1py/Exceptions/Exceptions.py
+-rw-rw-rw-   0        0        0      207 2022-02-14 13:07:33.000000 TM1py-1.9.1/TM1py/Exceptions/__init__.py
+drwxrwxrwx   0        0        0        0 2022-03-14 13:50:47.811364 TM1py-1.9.1/TM1py/Objects/
+-rw-rw-rw-   0        0        0     4897 2022-02-14 13:07:33.000000 TM1py-1.9.1/TM1py/Objects/Annotation.py
+-rw-rw-rw-   0        0        0     6868 2022-02-14 13:07:33.000000 TM1py-1.9.1/TM1py/Objects/Application.py
+-rw-rw-rw-   0        0        0     3781 2022-02-14 13:07:33.000000 TM1py-1.9.1/TM1py/Objects/Axis.py
+-rw-rw-rw-   0        0        0     4577 2022-02-14 13:07:33.000000 TM1py-1.9.1/TM1py/Objects/Chore.py
+-rw-rw-rw-   0        0        0     2049 2022-02-14 13:07:33.000000 TM1py-1.9.1/TM1py/Objects/ChoreFrequency.py
+-rw-rw-rw-   0        0        0     3385 2022-02-14 13:07:33.000000 TM1py-1.9.1/TM1py/Objects/ChoreStartTime.py
+-rw-rw-rw-   0        0        0     2513 2022-02-14 13:07:33.000000 TM1py-1.9.1/TM1py/Objects/ChoreTask.py
+-rw-rw-rw-   0        0        0     3188 2022-02-14 13:07:33.000000 TM1py-1.9.1/TM1py/Objects/Cube.py
+-rw-rw-rw-   0        0        0     4403 2022-02-14 13:07:33.000000 TM1py-1.9.1/TM1py/Objects/Dimension.py
+-rw-rw-rw-   0        0        0     2945 2022-02-14 13:07:33.000000 TM1py-1.9.1/TM1py/Objects/Element.py
+-rw-rw-rw-   0        0        0     2403 2022-02-14 13:07:33.000000 TM1py-1.9.1/TM1py/Objects/ElementAttribute.py
+-rw-rw-rw-   0        0        0     2313 2022-02-14 13:07:33.000000 TM1py-1.9.1/TM1py/Objects/Git.py
+-rw-rw-rw-   0        0        0      685 2022-02-14 13:07:33.000000 TM1py-1.9.1/TM1py/Objects/GitCommit.py
+-rw-rw-rw-   0        0        0     2905 2022-02-14 13:07:33.000000 TM1py-1.9.1/TM1py/Objects/GitPlan.py
+-rw-rw-rw-   0        0        0      743 2022-02-14 13:07:33.000000 TM1py-1.9.1/TM1py/Objects/GitRemote.py
+-rw-rw-rw-   0        0        0     9644 2022-02-14 13:07:33.000000 TM1py-1.9.1/TM1py/Objects/Hierarchy.py
+-rw-rw-rw-   0        0        0     2926 2022-02-23 16:24:21.000000 TM1py-1.9.1/TM1py/Objects/MDXView.py
+-rw-rw-rw-   0        0        0    10967 2022-02-23 16:24:21.000000 TM1py-1.9.1/TM1py/Objects/NativeView.py
+-rw-rw-rw-   0        0        0    19482 2022-02-14 13:07:33.000000 TM1py-1.9.1/TM1py/Objects/Process.py
+-rw-rw-rw-   0        0        0     2800 2022-02-14 13:07:33.000000 TM1py-1.9.1/TM1py/Objects/Rules.py
+-rw-rw-rw-   0        0        0     2194 2022-02-14 13:07:33.000000 TM1py-1.9.1/TM1py/Objects/Sandbox.py
+-rw-rw-rw-   0        0        0     1441 2022-02-14 13:07:33.000000 TM1py-1.9.1/TM1py/Objects/Server.py
+-rw-rw-rw-   0        0        0     8595 2022-02-14 13:07:33.000000 TM1py-1.9.1/TM1py/Objects/Subset.py
+-rw-rw-rw-   0        0        0      601 2022-02-14 13:07:33.000000 TM1py-1.9.1/TM1py/Objects/TM1Object.py
+-rw-rw-rw-   0        0        0     5262 2022-02-14 13:07:33.000000 TM1py-1.9.1/TM1py/Objects/User.py
+-rw-rw-rw-   0        0        0      812 2022-02-14 15:19:31.000000 TM1py-1.9.1/TM1py/Objects/View.py
+-rw-rw-rw-   0        0        0      995 2022-02-14 13:07:33.000000 TM1py-1.9.1/TM1py/Objects/__init__.py
+drwxrwxrwx   0        0        0        0 2022-03-14 13:50:47.942879 TM1py-1.9.1/TM1py/Services/
+-rw-rw-rw-   0        0        0     3513 2022-02-14 13:07:33.000000 TM1py-1.9.1/TM1py/Services/AnnotationService.py
+-rw-rw-rw-   0        0        0    12102 2022-02-14 13:07:33.000000 TM1py-1.9.1/TM1py/Services/ApplicationService.py
+-rw-rw-rw-   0        0        0   141382 2022-02-23 16:24:21.000000 TM1py-1.9.1/TM1py/Services/CellService.py
+-rw-rw-rw-   0        0        0    11531 2022-02-14 13:07:33.000000 TM1py-1.9.1/TM1py/Services/ChoreService.py
+-rw-rw-rw-   0        0        0    12717 2022-02-14 13:07:33.000000 TM1py-1.9.1/TM1py/Services/CubeService.py
+-rw-rw-rw-   0        0        0     7119 2022-02-14 13:07:33.000000 TM1py-1.9.1/TM1py/Services/DimensionService.py
+-rw-rw-rw-   0        0        0    28475 2022-03-14 13:48:04.000000 TM1py-1.9.1/TM1py/Services/ElementService.py
+-rw-rw-rw-   0        0        0     9351 2022-02-14 13:07:33.000000 TM1py-1.9.1/TM1py/Services/GitService.py
+-rw-rw-rw-   0        0        0    14509 2022-02-14 13:07:33.000000 TM1py-1.9.1/TM1py/Services/HierarchyService.py
+-rw-rw-rw-   0        0        0     5700 2022-02-14 13:07:33.000000 TM1py-1.9.1/TM1py/Services/MonitoringService.py
+-rw-rw-rw-   0        0        0     1729 2022-02-14 13:07:33.000000 TM1py-1.9.1/TM1py/Services/ObjectService.py
+-rw-rw-rw-   0        0        0     6459 2022-02-14 13:07:33.000000 TM1py-1.9.1/TM1py/Services/PowerBiService.py
+-rw-rw-rw-   0        0        0    18707 2022-03-10 08:02:31.000000 TM1py-1.9.1/TM1py/Services/ProcessService.py
+-rw-rw-rw-   0        0        0    25402 2022-03-14 13:47:56.000000 TM1py-1.9.1/TM1py/Services/RestService.py
+-rw-rw-rw-   0        0        0     4273 2022-02-14 13:07:33.000000 TM1py-1.9.1/TM1py/Services/SandboxService.py
+-rw-rw-rw-   0        0        0     9519 2022-02-14 13:07:33.000000 TM1py-1.9.1/TM1py/Services/SecurityService.py
+-rw-rw-rw-   0        0        0    15954 2022-02-14 13:07:33.000000 TM1py-1.9.1/TM1py/Services/ServerService.py
+-rw-rw-rw-   0        0        0     8606 2022-02-14 13:07:33.000000 TM1py-1.9.1/TM1py/Services/SubsetService.py
+-rw-rw-rw-   0        0        0     3512 2022-02-14 13:07:33.000000 TM1py-1.9.1/TM1py/Services/TM1Service.py
+-rw-rw-rw-   0        0        0     9128 2022-02-14 13:07:33.000000 TM1py-1.9.1/TM1py/Services/ViewService.py
+-rw-rw-rw-   0        0        0     1134 2022-02-14 13:07:33.000000 TM1py-1.9.1/TM1py/Services/__init__.py
+drwxrwxrwx   0        0        0        0 2022-03-14 13:50:47.958501 TM1py-1.9.1/TM1py/Utils/
+-rw-rw-rw-   0        0        0    10265 2022-02-14 13:07:33.000000 TM1py-1.9.1/TM1py/Utils/MDXUtils.py
+-rw-rw-rw-   0        0        0    43419 2022-03-14 13:47:56.000000 TM1py-1.9.1/TM1py/Utils/Utils.py
+-rw-rw-rw-   0        0        0       69 2022-02-14 13:07:33.000000 TM1py-1.9.1/TM1py/Utils/__init__.py
+-rw-rw-rw-   0        0        0     2818 2022-02-14 13:07:33.000000 TM1py-1.9.1/TM1py/__init__.py
+drwxrwxrwx   0        0        0        0 2022-03-14 13:50:47.610811 TM1py-1.9.1/TM1py.egg-info/
+-rw-rw-rw-   0        0        0     3687 2022-03-14 13:50:47.000000 TM1py-1.9.1/TM1py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1693 2022-03-14 13:50:47.000000 TM1py-1.9.1/TM1py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-03-14 13:50:47.000000 TM1py-1.9.1/TM1py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      100 2022-03-14 13:50:47.000000 TM1py-1.9.1/TM1py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       64 2022-03-14 13:50:47.000000 TM1py-1.9.1/TM1py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-03-14 13:50:47.958501 TM1py-1.9.1/setup.cfg
+-rw-rw-rw-   0        0        0     1517 2022-03-14 13:49:28.000000 TM1py-1.9.1/setup.py
```

### Comparing `TM1py-1.9.0/LICENSE` & `TM1py-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `TM1py-1.9.0/README.md` & `TM1py-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `TM1py-1.9.0/TM1py/Exceptions/Exceptions.py` & `TM1py-1.9.1/TM1py/Exceptions/Exceptions.py`

 * *Files identical despite different names*

### Comparing `TM1py-1.9.0/TM1py/Objects/Annotation.py` & `TM1py-1.9.1/TM1py/Objects/Annotation.py`

 * *Files identical despite different names*

### Comparing `TM1py-1.9.0/TM1py/Objects/Application.py` & `TM1py-1.9.1/TM1py/Objects/Application.py`

 * *Files identical despite different names*

### Comparing `TM1py-1.9.0/TM1py/Objects/Axis.py` & `TM1py-1.9.1/TM1py/Objects/Axis.py`

 * *Files identical despite different names*

### Comparing `TM1py-1.9.0/TM1py/Objects/Chore.py` & `TM1py-1.9.1/TM1py/Objects/Chore.py`

 * *Files identical despite different names*

### Comparing `TM1py-1.9.0/TM1py/Objects/ChoreFrequency.py` & `TM1py-1.9.1/TM1py/Objects/ChoreFrequency.py`

 * *Files identical despite different names*

### Comparing `TM1py-1.9.0/TM1py/Objects/ChoreTask.py` & `TM1py-1.9.1/TM1py/Objects/ChoreTask.py`

 * *Files identical despite different names*

### Comparing `TM1py-1.9.0/TM1py/Objects/Cube.py` & `TM1py-1.9.1/TM1py/Objects/Cube.py`

 * *Files identical despite different names*

### Comparing `TM1py-1.9.0/TM1py/Objects/Dimension.py` & `TM1py-1.9.1/TM1py/Objects/Dimension.py`

 * *Files identical despite different names*

### Comparing `TM1py-1.9.0/TM1py/Objects/Element.py` & `TM1py-1.9.1/TM1py/Objects/Element.py`

 * *Files identical despite different names*

### Comparing `TM1py-1.9.0/TM1py/Objects/ElementAttribute.py` & `TM1py-1.9.1/TM1py/Objects/ElementAttribute.py`

 * *Files identical despite different names*

### Comparing `TM1py-1.9.0/TM1py/Objects/Git.py` & `TM1py-1.9.1/TM1py/Objects/Git.py`

 * *Files identical despite different names*

### Comparing `TM1py-1.9.0/TM1py/Objects/GitCommit.py` & `TM1py-1.9.1/TM1py/Objects/GitCommit.py`

 * *Files identical despite different names*

### Comparing `TM1py-1.9.0/TM1py/Objects/GitPlan.py` & `TM1py-1.9.1/TM1py/Objects/GitPlan.py`

 * *Files identical despite different names*

### Comparing `TM1py-1.9.0/TM1py/Objects/GitRemote.py` & `TM1py-1.9.1/TM1py/Objects/GitRemote.py`

 * *Files identical despite different names*

### Comparing `TM1py-1.9.0/TM1py/Objects/Hierarchy.py` & `TM1py-1.9.1/TM1py/Objects/Hierarchy.py`

 * *Files identical despite different names*

### Comparing `TM1py-1.9.0/TM1py/Objects/MDXView.py` & `TM1py-1.9.1/TM1py/Objects/MDXView.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # -*- coding: utf-8 -*-
 
 import collections
 import json
+import re
 from typing import Optional, Dict
 
 from TM1py.Objects.View import View
+from TM1py.Utils import case_and_space_insensitive_equals
 
 
 class MDXView(View):
     """ Abstraction on TM1 MDX view
 
         IMPORTANT. MDXViews can't be seen through the old TM1 clients (Archict, Perspectives). They do exist though!
     """
@@ -33,14 +35,44 @@
     def MDX(self, value: str):
         self._mdx = value
 
     @property
     def body(self) -> str:
         return self.construct_body()
 
+    def substitute_title(self, dimension: str, hierarchy: str, element: str):
+        """ dimension and hierarchy name are space sensitive!
+
+        :param dimension:
+        :param hierarchy:
+        :param element:
+        :return:
+        """
+        pattern = re.compile(r"\[" + dimension + r"\].\[" + hierarchy + r"\].\[(.*?)\]", re.IGNORECASE)
+        findings = re.findall(pattern, self._mdx)
+
+        if findings:
+            self._mdx = re.sub(
+                pattern=pattern,
+                repl=f"[{dimension}].[{hierarchy}].[{element}]",
+                string=self._mdx)
+            return
+
+        if hierarchy is None or case_and_space_insensitive_equals(dimension, hierarchy):
+            pattern = re.compile(r"\[" + dimension + r"\].\[(.*?)\]", re.IGNORECASE)
+            findings = re.findall(pattern, self._mdx)
+            if findings:
+                self._mdx = re.sub(
+                    pattern=pattern,
+                    repl=f"[{dimension}].[{element}]",
+                    string=self._mdx)
+                return
+
+        raise ValueError(f"No selection in title with dimension: '{dimension}' and hierarchy: '{hierarchy}'")
+
     @classmethod
     def from_json(cls, view_as_json: str, cube_name: Optional[str] = None) -> 'MDXView':
         view_as_dict = json.loads(view_as_json)
         return cls.from_dict(view_as_dict, cube_name)
 
     @classmethod
     def from_dict(cls, view_as_dict: Dict, cube_name: str = None) -> 'MDXView':
```

### Comparing `TM1py-1.9.0/TM1py/Objects/NativeView.py` & `TM1py-1.9.1/TM1py/Objects/NativeView.py`

 * *Files 3% similar despite different names*

```diff
@@ -199,14 +199,23 @@
         :param dimension_name: name of the dimension.
         :return:
         """
         for title in self._titles[:]:
             if case_and_space_insensitive_equals(title.dimension_name, dimension_name):
                 self._titles.remove(title)
 
+    def substitute_title(self, dimension: str, element: str):
+        for title in self._titles:
+            if case_and_space_insensitive_equals(title.dimension_name, dimension):
+                title._subset = AnonymousSubset(dimension, dimension, elements=[element])
+                title._selected = element
+                return
+
+        raise ValueError(f"Dimension '{dimension}' not found in titles")
+
     @classmethod
     def from_json(cls, view_as_json: str, cube_name: Optional[str] = None) -> 'NativeView':
         """ Alternative constructor
                 :Parameters:
                     `view_as_json` : string, JSON
 
                 :Returns:
```

### Comparing `TM1py-1.9.0/TM1py/Objects/Process.py` & `TM1py-1.9.1/TM1py/Objects/Process.py`

 * *Files identical despite different names*

### Comparing `TM1py-1.9.0/TM1py/Objects/Rules.py` & `TM1py-1.9.1/TM1py/Objects/Rules.py`

 * *Files identical despite different names*

### Comparing `TM1py-1.9.0/TM1py/Objects/Sandbox.py` & `TM1py-1.9.1/TM1py/Objects/Sandbox.py`

 * *Files identical despite different names*

### Comparing `TM1py-1.9.0/TM1py/Objects/Server.py` & `TM1py-1.9.1/TM1py/Objects/Server.py`

 * *Files identical despite different names*

### Comparing `TM1py-1.9.0/TM1py/Objects/Subset.py` & `TM1py-1.9.1/TM1py/Objects/Subset.py`

 * *Files identical despite different names*

### Comparing `TM1py-1.9.0/TM1py/Objects/TM1Object.py` & `TM1py-1.9.1/TM1py/Objects/TM1Object.py`

 * *Files identical despite different names*

### Comparing `TM1py-1.9.0/TM1py/Objects/User.py` & `TM1py-1.9.1/TM1py/Objects/User.py`

 * *Files identical despite different names*

### Comparing `TM1py-1.9.0/TM1py/Objects/View.py` & `TM1py-1.9.1/TM1py/Objects/View.py`

 * *Files identical despite different names*

### Comparing `TM1py-1.9.0/TM1py/Objects/__init__.py` & `TM1py-1.9.1/TM1py/Objects/__init__.py`

 * *Files identical despite different names*

### Comparing `TM1py-1.9.0/TM1py/Services/AnnotationService.py` & `TM1py-1.9.1/TM1py/Services/AnnotationService.py`

 * *Files identical despite different names*

### Comparing `TM1py-1.9.0/TM1py/Services/ApplicationService.py` & `TM1py-1.9.1/TM1py/Services/ApplicationService.py`

 * *Files identical despite different names*

### Comparing `TM1py-1.9.0/TM1py/Services/CellService.py` & `TM1py-1.9.1/TM1py/Services/CellService.py`

 * *Files 1% similar despite different names*

```diff
@@ -2294,14 +2294,15 @@
             skip_rule_derived_cells: bool = False,
             csv_dialect: 'csv.Dialect' = None,
             line_separator: str = "\r\n",
             value_separator: str = ",",
             sandbox_name: str = None,
             include_attributes: bool = False,
             use_compact_json: bool = False,
+            include_headers: bool = True,
             **kwargs) -> str:
         """ Execute cellset and return only the 'Content', in csv format
 
         :param cellset_id: String; ID of existing cellset
         :param top: Int, number of cells to return (counting from top)
         :param skip: Int, number of cells to skip (counting from top)
         :param skip_zeros: skip zeros in cellset (irrespective of zero suppression in MDX / view)
@@ -2310,31 +2311,37 @@
         :param csv_dialect: provide all csv output settings through standard library csv.Dialect
             If not provided dialect is created based on line_separator and value_separator arguments.
         :param line_separator:
         :param value_separator
         :param sandbox_name: str
         :param include_attributes: include attribute columns
         :param use_compact_json: bool
+        :param include_headers: bool
         :return: Raw format from TM1.
         """
+        if 'delete_cellset' in kwargs:
+            delete_cellset = kwargs.pop('delete_cellset')
+        else:
+            delete_cellset = True
         _, _, rows, columns = self.extract_cellset_composition(cellset_id, delete_cellset=False,
                                                                sandbox_name=sandbox_name, **kwargs)
         cellset_dict = self.extract_cellset_raw(cellset_id, cell_properties=["Value"], top=top, skip=skip,
                                                 skip_contexts=True, skip_zeros=skip_zeros,
                                                 skip_consolidated_cells=skip_consolidated_cells,
                                                 skip_rule_derived_cells=skip_rule_derived_cells,
-                                                delete_cellset=True, sandbox_name=sandbox_name,
+                                                delete_cellset=delete_cellset, sandbox_name=sandbox_name,
                                                 elem_properties=['Name'],
                                                 member_properties=['Name',
                                                                    'Attributes'] if include_attributes else None,
                                                 use_compact_json=use_compact_json,
                                                 **kwargs)
         return build_csv_from_cellset_dict(rows, columns, cellset_dict, csv_dialect=csv_dialect,
                                            line_separator=line_separator, value_separator=value_separator,
-                                           top=top, include_attributes=include_attributes)
+                                           top=top, include_attributes=include_attributes,
+                                           include_headers=include_headers)
 
     def extract_cellset_csv_iter_json(
             self,
             cellset_id: str,
             top: int = None,
             skip: int = None,
             skip_zeros: bool = True,
```

### Comparing `TM1py-1.9.0/TM1py/Services/ChoreService.py` & `TM1py-1.9.1/TM1py/Services/ChoreService.py`

 * *Files identical despite different names*

### Comparing `TM1py-1.9.0/TM1py/Services/CubeService.py` & `TM1py-1.9.1/TM1py/Services/CubeService.py`

 * *Files identical despite different names*

### Comparing `TM1py-1.9.0/TM1py/Services/DimensionService.py` & `TM1py-1.9.1/TM1py/Services/DimensionService.py`

 * *Files identical despite different names*

### Comparing `TM1py-1.9.0/TM1py/Services/ElementService.py` & `TM1py-1.9.1/TM1py/Services/ElementService.py`

 * *Files 2% similar despite different names*

```diff
@@ -557,14 +557,34 @@
               f'{expand_properties}))'
 
         payload = {"MDX": mdx}
         response = self._rest.POST(url, json.dumps(payload, ensure_ascii=False), **kwargs)
         raw_dict = response.json()
         return [tuples['Members'] for tuples in raw_dict['Tuples']]
 
+    def remove_edge(self, dimension_name: str, hierarchy_name: str, parent: str, component: str, **kwargs) -> Response:
+        """ Remove one edge from hierarchy. Fails if parent or child element doesn't exist.
+
+        :param dimension_name:
+        :param hierarchy_name:
+        :param parent:
+        :param component:
+        :return:
+        """
+
+        url = format_url(
+            "/api/v1/Dimensions('{}')/Hierarchies('{}')/Elements('{}')/Edges(ParentName='{}',ComponentName='{}')",
+            dimension_name,
+            hierarchy_name,
+            parent,
+            parent,
+            component)
+
+        return self._rest.DELETE(url=url, **kwargs)
+
     def add_edges(self, dimension_name: str, hierarchy_name: str = None, edges: Dict[Tuple[str, str], int] = None,
                   **kwargs) -> Response:
         """ Add Edges to hierarchy. Fails if one edge already exists.
 
         :param dimension_name:
         :param hierarchy_name:
         :param edges:
```

### Comparing `TM1py-1.9.0/TM1py/Services/GitService.py` & `TM1py-1.9.1/TM1py/Services/GitService.py`

 * *Files identical despite different names*

### Comparing `TM1py-1.9.0/TM1py/Services/HierarchyService.py` & `TM1py-1.9.1/TM1py/Services/HierarchyService.py`

 * *Files identical despite different names*

### Comparing `TM1py-1.9.0/TM1py/Services/MonitoringService.py` & `TM1py-1.9.1/TM1py/Services/MonitoringService.py`

 * *Files identical despite different names*

### Comparing `TM1py-1.9.0/TM1py/Services/ObjectService.py` & `TM1py-1.9.1/TM1py/Services/ObjectService.py`

 * *Files identical despite different names*

### Comparing `TM1py-1.9.0/TM1py/Services/PowerBiService.py` & `TM1py-1.9.1/TM1py/Services/PowerBiService.py`

 * *Files identical despite different names*

### Comparing `TM1py-1.9.0/TM1py/Services/ProcessService.py` & `TM1py-1.9.1/TM1py/Services/ProcessService.py`

 * *Files 1% similar despite different names*

```diff
@@ -396,7 +396,22 @@
 
         raw_url = "/api/v1/ProcessDebugContexts('{}')?$expand=Breakpoints," \
                   "Thread,CallStack($expand=Variables,Process($select=Name))"
         url = format_url(raw_url, debug_id)
         response = self._rest.GET(url, **kwargs)
 
         return response.json()
+
+    def debug_step_out(self, debug_id: str, **kwargs) -> Dict:
+        url = format_url("/api/v1/ProcessDebugContexts('{}')/tm1.StepOut", debug_id)
+        self._rest.POST(url, **kwargs)
+
+        # digest time  necessary for TM1 <= 11.8
+        # ToDo: remove in later versions of TM1 once issue in TM1 server is resolved
+        time.sleep(0.1)
+
+        raw_url = "/api/v1/ProcessDebugContexts('{}')?$expand=Breakpoints," \
+                  "Thread,CallStack($expand=Variables,Process($select=Name))"
+        url = format_url(raw_url, debug_id)
+        response = self._rest.GET(url, **kwargs)
+
+        return response.json()
```

### Comparing `TM1py-1.9.0/TM1py/Services/RestService.py` & `TM1py-1.9.1/TM1py/Services/RestService.py`

 * *Files identical despite different names*

### Comparing `TM1py-1.9.0/TM1py/Services/SandboxService.py` & `TM1py-1.9.1/TM1py/Services/SandboxService.py`

 * *Files identical despite different names*

### Comparing `TM1py-1.9.0/TM1py/Services/SecurityService.py` & `TM1py-1.9.1/TM1py/Services/SecurityService.py`

 * *Files identical despite different names*

### Comparing `TM1py-1.9.0/TM1py/Services/ServerService.py` & `TM1py-1.9.1/TM1py/Services/ServerService.py`

 * *Files identical despite different names*

### Comparing `TM1py-1.9.0/TM1py/Services/SubsetService.py` & `TM1py-1.9.1/TM1py/Services/SubsetService.py`

 * *Files identical despite different names*

### Comparing `TM1py-1.9.0/TM1py/Services/TM1Service.py` & `TM1py-1.9.1/TM1py/Services/TM1Service.py`

 * *Files identical despite different names*

### Comparing `TM1py-1.9.0/TM1py/Services/ViewService.py` & `TM1py-1.9.1/TM1py/Services/ViewService.py`

 * *Files identical despite different names*

### Comparing `TM1py-1.9.0/TM1py/Services/__init__.py` & `TM1py-1.9.1/TM1py/Services/__init__.py`

 * *Files identical despite different names*

### Comparing `TM1py-1.9.0/TM1py/Utils/MDXUtils.py` & `TM1py-1.9.1/TM1py/Utils/MDXUtils.py`

 * *Files identical despite different names*

### Comparing `TM1py-1.9.0/TM1py/Utils/Utils.py` & `TM1py-1.9.1/TM1py/Utils/Utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -334,25 +334,27 @@
         row_dimensions: List[str],
         column_dimensions: List[str],
         raw_cellset_as_dict: Dict,
         top: Optional[int] = None,
         csv_dialect: 'csv.Dialect' = None,
         line_separator: str = "\r\n",
         value_separator: str = ",",
-        include_attributes: bool = False) -> str:
+        include_attributes: bool = False,
+        include_headers: bool = True) -> str:
     """ transform raw cellset data into concise dictionary
     :param column_dimensions:
     :param row_dimensions:
     :param raw_cellset_as_dict:
     :param top: Maximum Number of cells
     :param csv_dialect: provide all csv output settings through standard library csv.Dialect
         If not provided dialect is created based on line_separator and value_separator arguments.
     :param line_separator:
     :param value_separator:
     :param include_attributes: include attribute columns
+    :param include_headers: bool
     :return:
     """
 
     cells = raw_cellset_as_dict['Cells']
     # empty cellsets produce "" in order to be compliant with previous implementation that used `/Content` API endpoint
     if len(cells) == 0:
         return ""
@@ -362,16 +364,17 @@
         csv_dialect = csv.get_dialect("TM1py")
 
     csv_content = StringIO()
     csv_writer = csv.writer(csv_content, dialect=csv_dialect)
 
     column_axis, row_axis, _ = extract_axes_from_cellset(raw_cellset_as_dict=raw_cellset_as_dict)
 
-    headers = _build_headers_for_csv(row_axis, column_axis, row_dimensions, column_dimensions, include_attributes)
-    csv_writer.writerow(headers)
+    if include_headers:
+        headers = _build_headers_for_csv(row_axis, column_axis, row_dimensions, column_dimensions, include_attributes)
+        csv_writer.writerow(headers)
 
     for ordinal, cell in enumerate(cells[:top or len(cells)]):
         # if skip is used in execution we must use the original ordinal from the cell, if not we can simply enumerate
         ordinal = cell.get("Ordinal", ordinal)
 
         line = []
         if column_axis and row_axis:
```

### Comparing `TM1py-1.9.0/TM1py/__init__.py` & `TM1py-1.9.1/TM1py/__init__.py`

 * *Files identical despite different names*

### Comparing `TM1py-1.9.0/TM1py.egg-info/SOURCES.txt` & `TM1py-1.9.1/TM1py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TM1py-1.9.0/setup.py` & `TM1py-1.9.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-SCHEDULE_VERSION = '1.9.0'
+SCHEDULE_VERSION = '1.9.1'
 SCHEDULE_DOWNLOAD_URL = (
         'https://github.com/Cubewise-code/TM1py/tarball/' + SCHEDULE_VERSION
 )
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
@@ -27,14 +27,15 @@
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
         'Natural Language :: English',
     ],
     install_requires=[
         'ijson',
         'requests',
         'pytz',
         'requests_negotiate_sspi;platform_system=="Windows"',
```

