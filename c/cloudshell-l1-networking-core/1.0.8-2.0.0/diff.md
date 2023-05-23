# Comparing `tmp/cloudshell-l1-networking-core-1.0.8.zip` & `tmp/cloudshell-l1-networking-core-2.0.0.zip`

## zipinfo {}

```diff
@@ -1,55 +1,98 @@
-Zip file size: 29946 bytes, number of entries: 53
--rw-r--r--  2.0 unx       28 b- defN 18-Jun-24 16:01 cloudshell-l1-networking-core-1.0.8/test_requirements.txt
--rw-r--r--  2.0 unx      605 b- defN 18-Dec-05 15:52 cloudshell-l1-networking-core-1.0.8/PKG-INFO
--rw-r--r--  2.0 unx        8 b- defN 18-Jun-24 16:01 cloudshell-l1-networking-core-1.0.8/requirements.txt
--rw-r--r--  2.0 unx       77 b- defN 18-Jun-24 16:01 cloudshell-l1-networking-core-1.0.8/MANIFEST.in
--rw-r--r--  2.0 unx      958 b- defN 18-Jun-24 16:01 cloudshell-l1-networking-core-1.0.8/README.md
--rw-r--r--  2.0 unx     1376 b- defN 18-Jul-04 15:26 cloudshell-l1-networking-core-1.0.8/setup.py
--rw-r--r--  2.0 unx       38 b- defN 18-Dec-05 15:52 cloudshell-l1-networking-core-1.0.8/setup.cfg
--rw-r--r--  2.0 unx        6 b- defN 18-Nov-14 18:17 cloudshell-l1-networking-core-1.0.8/version.txt
--rw-r--r--  2.0 unx      118 b- defN 18-Jun-24 16:01 cloudshell-l1-networking-core-1.0.8/tests/__init__.py
--rw-r--r--  2.0 unx      605 b- defN 18-Dec-05 15:52 cloudshell-l1-networking-core-1.0.8/cloudshell_l1_networking_core.egg-info/PKG-INFO
--rw-r--r--  2.0 unx        1 b- defN 18-Jul-03 17:45 cloudshell-l1-networking-core-1.0.8/cloudshell_l1_networking_core.egg-info/not-zip-safe
--rw-r--r--  2.0 unx     2621 b- defN 18-Dec-05 15:52 cloudshell-l1-networking-core-1.0.8/cloudshell_l1_networking_core.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx       80 b- defN 18-Dec-05 15:52 cloudshell-l1-networking-core-1.0.8/cloudshell_l1_networking_core.egg-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 18-Dec-05 15:52 cloudshell-l1-networking-core-1.0.8/cloudshell_l1_networking_core.egg-info/requires.txt
--rw-r--r--  2.0 unx       11 b- defN 18-Dec-05 15:52 cloudshell-l1-networking-core-1.0.8/cloudshell_l1_networking_core.egg-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 18-Dec-05 15:52 cloudshell-l1-networking-core-1.0.8/cloudshell_l1_networking_core.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx      118 b- defN 18-Jun-24 16:01 cloudshell-l1-networking-core-1.0.8/cloudshell/__init__.py
--rw-r--r--  2.0 unx      118 b- defN 18-Jun-24 16:01 cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/__init__.py
--rw-r--r--  2.0 unx     3725 b- defN 18-Nov-15 16:31 cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/tools/build_driver.py
--rw-r--r--  2.0 unx      118 b- defN 18-Jul-04 15:34 cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/tools/__init__.py
--rw-r--r--  2.0 unx     2700 b- defN 18-Jun-24 16:01 cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/driver_commands_interface.py
--rw-r--r--  2.0 unx    12602 b- defN 18-Jun-24 16:01 cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/command_executor.py
--rw-r--r--  2.0 unx     3362 b- defN 18-Jun-24 16:01 cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/connection_handler.py
--rw-r--r--  2.0 unx      118 b- defN 18-Jun-24 16:01 cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/__init__.py
--rw-r--r--  2.0 unx     3142 b- defN 18-Jun-24 16:01 cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/driver_listener.py
--rw-r--r--  2.0 unx      134 b- defN 18-Jun-24 16:01 cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/layer_one_driver_exception.py
--rw-r--r--  2.0 unx      117 b- defN 18-Jun-24 16:01 cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/response/__init__.py
--rw-r--r--  2.0 unx      863 b- defN 18-Jun-24 16:01 cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/response/command_response.py
--rw-r--r--  2.0 unx     3533 b- defN 18-Jun-24 16:01 cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/response/command_responses_builder.py
--rw-r--r--  2.0 unx     3103 b- defN 18-Jun-24 16:01 cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/response/response_info.py
--rw-r--r--  2.0 unx      183 b- defN 18-Jun-24 16:01 cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/response/templates/command_response_template.xml
--rw-r--r--  2.0 unx       21 b- defN 18-Jun-24 16:01 cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/response/templates/state_id_template.xml
--rw-r--r--  2.0 unx      171 b- defN 18-Jun-24 16:01 cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/response/templates/responses_template.xml
--rw-r--r--  2.0 unx      231 b- defN 18-Jun-24 16:01 cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/response/templates/error_response.xml
--rw-r--r--  2.0 unx      118 b- defN 18-Jun-24 16:01 cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/response/resource_info/__init__.py
--rw-r--r--  2.0 unx     4014 b- defN 18-Jun-24 16:01 cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/response/resource_info/resource_info_builder.py
--rw-r--r--  2.0 unx      156 b- defN 18-Jun-24 16:01 cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/response/resource_info/templates/resource_template.xml
--rw-r--r--  2.0 unx       59 b- defN 18-Jun-24 16:01 cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/response/resource_info/templates/resource_incoming_map_template.xml
--rw-r--r--  2.0 unx       37 b- defN 18-Jun-24 16:01 cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/response/resource_info/templates/resource_attribute_template.xml
--rw-r--r--  2.0 unx     2411 b- defN 18-Jun-24 16:01 cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/response/resource_info/entities/port.py
--rw-r--r--  2.0 unx      856 b- defN 18-Jun-24 16:01 cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/response/resource_info/entities/attributes.py
--rw-r--r--  2.0 unx      285 b- defN 18-Jun-24 16:01 cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/response/resource_info/entities/validators.py
--rw-r--r--  2.0 unx      118 b- defN 18-Jun-24 16:01 cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/response/resource_info/entities/__init__.py
--rw-r--r--  2.0 unx     1080 b- defN 18-Jun-24 16:01 cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/response/resource_info/entities/blade.py
--rw-r--r--  2.0 unx     1949 b- defN 18-Jun-24 16:01 cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/response/resource_info/entities/base.py
--rw-r--r--  2.0 unx     1316 b- defN 18-Jun-24 16:01 cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/response/resource_info/entities/chassis.py
--rw-r--r--  2.0 unx     1704 b- defN 18-Jun-24 16:01 cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/request/requests_parser.py
--rw-r--r--  2.0 unx      117 b- defN 18-Jun-24 16:01 cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/request/__init__.py
--rw-r--r--  2.0 unx      625 b- defN 18-Jun-24 16:01 cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/request/command_request.py
--rw-r--r--  2.0 unx     1038 b- defN 18-Jun-24 16:01 cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/helper/xml_helper.py
--rw-r--r--  2.0 unx      117 b- defN 18-Jun-24 16:01 cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/helper/__init__.py
--rw-r--r--  2.0 unx      654 b- defN 18-Jun-24 16:01 cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/helper/xml_logger.py
--rw-r--r--  2.0 unx     1647 b- defN 18-Nov-15 16:26 cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/helper/runtime_configuration.py
-53 files, 59200 bytes uncompressed, 16904 bytes compressed:  71.4%
+Zip file size: 48481 bytes, number of entries: 96
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/.tox/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell_l1_networking_core.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/tests/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/
+-rw-r--r--  2.0 unx      866 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/README.md
+-rw-r--r--  2.0 unx       22 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/test_requirements.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/version.txt
+-rw-r--r--  2.0 unx       77 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/MANIFEST.in
+-rw-r--r--  2.0 unx        7 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/requirements.txt
+-rw-r--r--  2.0 unx      440 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/PKG-INFO
+-rw-r--r--  2.0 unx     1263 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/setup.py
+-rw-r--r--  2.0 unx       70 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/dev_requirements.txt
+-rw-r--r--  2.0 unx     1113 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/tox.ini
+-rw-r--r--  2.0 unx       38 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/setup.cfg
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/.tox/build/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/.tox/build/lib/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/.tox/build/lib/python3.9/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/.tox/build/lib/python3.9/site-packages/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/.tox/build/lib/python3.9/site-packages/setuptools/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/.tox/build/lib/python3.9/site-packages/wheel/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/.tox/build/lib/python3.9/site-packages/setuptools-67.7.2.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/.tox/build/lib/python3.9/site-packages/pip/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/.tox/build/lib/python3.9/site-packages/wheel-0.40.0.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/.tox/build/lib/python3.9/site-packages/pip-23.1.2.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/.tox/build/lib/python3.9/site-packages/setuptools/command/
+-rw-r--r--  2.0 unx      628 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/.tox/build/lib/python3.9/site-packages/setuptools/command/launcher manifest.xml
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/.tox/build/lib/python3.9/site-packages/wheel/vendored/
+-rw-r--r--  2.0 unx       16 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/.tox/build/lib/python3.9/site-packages/wheel/vendored/vendor.txt
+-rw-r--r--  2.0 unx       41 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/.tox/build/lib/python3.9/site-packages/setuptools-67.7.2.dist-info/top_level.txt
+-rw-r--r--  2.0 unx     2740 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/.tox/build/lib/python3.9/site-packages/setuptools-67.7.2.dist-info/entry_points.txt
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/.tox/build/lib/python3.9/site-packages/pip/_vendor/
+-rw-r--r--  2.0 unx      476 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/.tox/build/lib/python3.9/site-packages/pip/_vendor/vendor.txt
+-rw-r--r--  2.0 unx     1107 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/.tox/build/lib/python3.9/site-packages/wheel-0.40.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      104 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/.tox/build/lib/python3.9/site-packages/wheel-0.40.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx     9953 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/.tox/build/lib/python3.9/site-packages/pip-23.1.2.dist-info/AUTHORS.txt
+-rw-r--r--  2.0 unx     1093 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/.tox/build/lib/python3.9/site-packages/pip-23.1.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx        4 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/.tox/build/lib/python3.9/site-packages/pip-23.1.2.dist-info/top_level.txt
+-rw-r--r--  2.0 unx      125 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/.tox/build/lib/python3.9/site-packages/pip-23.1.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell_l1_networking_core.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell_l1_networking_core.egg-info/not-zip-safe
+-rw-r--r--  2.0 unx        7 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell_l1_networking_core.egg-info/requires.txt
+-rw-r--r--  2.0 unx       17 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell_l1_networking_core.egg-info/top_level.txt
+-rw-r--r--  2.0 unx      440 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell_l1_networking_core.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx       79 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell_l1_networking_core.egg-info/entry_points.txt
+-rw-r--r--  2.0 unx     3532 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell_l1_networking_core.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx       76 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/tests/__init__.py
+-rw-r--r--  2.0 unx      147 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/tests/test_smth.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/
+-rw-r--r--  2.0 unx       76 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/tools/
+-rw-r--r--  2.0 unx       76 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/helper/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/request/
+-rw-r--r--  2.0 unx     9193 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/command_executor.py
+-rw-r--r--  2.0 unx     3411 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/driver_listener.py
+-rw-r--r--  2.0 unx       82 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/layer_one_driver_exception.py
+-rw-r--r--  2.0 unx     3559 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/connection_handler.py
+-rw-r--r--  2.0 unx       76 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/__init__.py
+-rw-r--r--  2.0 unx     2508 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/driver_commands_interface.py
+-rw-r--r--  2.0 unx      685 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/helper/xml_logger.py
+-rw-r--r--  2.0 unx      155 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/helper/logger.py
+-rw-r--r--  2.0 unx      689 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/helper/xml_helper.py
+-rw-r--r--  2.0 unx       76 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/helper/__init__.py
+-rw-r--r--  2.0 unx     1636 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/helper/runtime_configuration.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/resource_info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/templates/
+-rw-r--r--  2.0 unx     3457 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/command_responses_builder.py
+-rw-r--r--  2.0 unx     3149 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/response_info.py
+-rw-r--r--  2.0 unx       76 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/__init__.py
+-rw-r--r--  2.0 unx      755 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/command_response.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/resource_info/entities/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/resource_info/templates/
+-rw-r--r--  2.0 unx       76 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/resource_info/__init__.py
+-rw-r--r--  2.0 unx     3487 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/resource_info/resource_info_builder.py
+-rw-r--r--  2.0 unx     1247 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/resource_info/entities/chassis.py
+-rw-r--r--  2.0 unx     1748 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/resource_info/entities/base.py
+-rw-r--r--  2.0 unx     1069 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/resource_info/entities/blade.py
+-rw-r--r--  2.0 unx      310 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/resource_info/entities/validators.py
+-rw-r--r--  2.0 unx       76 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/resource_info/entities/__init__.py
+-rw-r--r--  2.0 unx     2415 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/resource_info/entities/port.py
+-rw-r--r--  2.0 unx      766 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/resource_info/entities/attributes.py
+-rw-r--r--  2.0 unx      156 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/resource_info/templates/resource_template.xml
+-rw-r--r--  2.0 unx       37 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/resource_info/templates/resource_attribute_template.xml
+-rw-r--r--  2.0 unx       59 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/resource_info/templates/resource_incoming_map_template.xml
+-rw-r--r--  2.0 unx      231 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/templates/error_response.xml
+-rw-r--r--  2.0 unx      183 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/templates/command_response_template.xml
+-rw-r--r--  2.0 unx       21 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/templates/state_id_template.xml
+-rw-r--r--  2.0 unx      171 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/templates/responses_template.xml
+-rw-r--r--  2.0 unx      465 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/request/command_request.py
+-rw-r--r--  2.0 unx     1428 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/request/requests_parser.py
+-rw-r--r--  2.0 unx       76 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/request/__init__.py
+-rw-r--r--  2.0 unx     3841 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/tools/build_driver.py
+-rw-r--r--  2.0 unx       76 b- defN 23-May-23 10:16 cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/tools/__init__.py
+96 files, 72086 bytes uncompressed, 25227 bytes compressed:  65.0%
```

## zipnote {}

```diff
@@ -1,160 +1,289 @@
-Filename: cloudshell-l1-networking-core-1.0.8/test_requirements.txt
+Filename: cloudshell-l1-networking-core-2.0.0/
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/PKG-INFO
+Filename: cloudshell-l1-networking-core-2.0.0/.tox/
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/requirements.txt
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell_l1_networking_core.egg-info/
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/MANIFEST.in
+Filename: cloudshell-l1-networking-core-2.0.0/tests/
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/README.md
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/setup.py
+Filename: cloudshell-l1-networking-core-2.0.0/README.md
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/setup.cfg
+Filename: cloudshell-l1-networking-core-2.0.0/test_requirements.txt
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/version.txt
+Filename: cloudshell-l1-networking-core-2.0.0/version.txt
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/tests/__init__.py
+Filename: cloudshell-l1-networking-core-2.0.0/MANIFEST.in
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/cloudshell_l1_networking_core.egg-info/PKG-INFO
+Filename: cloudshell-l1-networking-core-2.0.0/requirements.txt
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/cloudshell_l1_networking_core.egg-info/not-zip-safe
+Filename: cloudshell-l1-networking-core-2.0.0/PKG-INFO
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/cloudshell_l1_networking_core.egg-info/SOURCES.txt
+Filename: cloudshell-l1-networking-core-2.0.0/setup.py
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/cloudshell_l1_networking_core.egg-info/entry_points.txt
+Filename: cloudshell-l1-networking-core-2.0.0/dev_requirements.txt
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/cloudshell_l1_networking_core.egg-info/requires.txt
+Filename: cloudshell-l1-networking-core-2.0.0/tox.ini
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/cloudshell_l1_networking_core.egg-info/top_level.txt
+Filename: cloudshell-l1-networking-core-2.0.0/setup.cfg
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/cloudshell_l1_networking_core.egg-info/dependency_links.txt
+Filename: cloudshell-l1-networking-core-2.0.0/.tox/build/
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/cloudshell/__init__.py
+Filename: cloudshell-l1-networking-core-2.0.0/.tox/build/lib/
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/__init__.py
+Filename: cloudshell-l1-networking-core-2.0.0/.tox/build/lib/python3.9/
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/tools/build_driver.py
+Filename: cloudshell-l1-networking-core-2.0.0/.tox/build/lib/python3.9/site-packages/
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/tools/__init__.py
+Filename: cloudshell-l1-networking-core-2.0.0/.tox/build/lib/python3.9/site-packages/setuptools/
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/driver_commands_interface.py
+Filename: cloudshell-l1-networking-core-2.0.0/.tox/build/lib/python3.9/site-packages/wheel/
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/command_executor.py
+Filename: cloudshell-l1-networking-core-2.0.0/.tox/build/lib/python3.9/site-packages/setuptools-67.7.2.dist-info/
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/connection_handler.py
+Filename: cloudshell-l1-networking-core-2.0.0/.tox/build/lib/python3.9/site-packages/pip/
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/__init__.py
+Filename: cloudshell-l1-networking-core-2.0.0/.tox/build/lib/python3.9/site-packages/wheel-0.40.0.dist-info/
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/driver_listener.py
+Filename: cloudshell-l1-networking-core-2.0.0/.tox/build/lib/python3.9/site-packages/pip-23.1.2.dist-info/
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/layer_one_driver_exception.py
+Filename: cloudshell-l1-networking-core-2.0.0/.tox/build/lib/python3.9/site-packages/setuptools/command/
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/response/__init__.py
+Filename: cloudshell-l1-networking-core-2.0.0/.tox/build/lib/python3.9/site-packages/setuptools/command/launcher manifest.xml
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/response/command_response.py
+Filename: cloudshell-l1-networking-core-2.0.0/.tox/build/lib/python3.9/site-packages/wheel/vendored/
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/response/command_responses_builder.py
+Filename: cloudshell-l1-networking-core-2.0.0/.tox/build/lib/python3.9/site-packages/wheel/vendored/vendor.txt
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/response/response_info.py
+Filename: cloudshell-l1-networking-core-2.0.0/.tox/build/lib/python3.9/site-packages/setuptools-67.7.2.dist-info/top_level.txt
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/response/templates/command_response_template.xml
+Filename: cloudshell-l1-networking-core-2.0.0/.tox/build/lib/python3.9/site-packages/setuptools-67.7.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/response/templates/state_id_template.xml
+Filename: cloudshell-l1-networking-core-2.0.0/.tox/build/lib/python3.9/site-packages/pip/_vendor/
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/response/templates/responses_template.xml
+Filename: cloudshell-l1-networking-core-2.0.0/.tox/build/lib/python3.9/site-packages/pip/_vendor/vendor.txt
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/response/templates/error_response.xml
+Filename: cloudshell-l1-networking-core-2.0.0/.tox/build/lib/python3.9/site-packages/wheel-0.40.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/response/resource_info/__init__.py
+Filename: cloudshell-l1-networking-core-2.0.0/.tox/build/lib/python3.9/site-packages/wheel-0.40.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/response/resource_info/resource_info_builder.py
+Filename: cloudshell-l1-networking-core-2.0.0/.tox/build/lib/python3.9/site-packages/pip-23.1.2.dist-info/AUTHORS.txt
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/response/resource_info/templates/resource_template.xml
+Filename: cloudshell-l1-networking-core-2.0.0/.tox/build/lib/python3.9/site-packages/pip-23.1.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/response/resource_info/templates/resource_incoming_map_template.xml
+Filename: cloudshell-l1-networking-core-2.0.0/.tox/build/lib/python3.9/site-packages/pip-23.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/response/resource_info/templates/resource_attribute_template.xml
+Filename: cloudshell-l1-networking-core-2.0.0/.tox/build/lib/python3.9/site-packages/pip-23.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/response/resource_info/entities/port.py
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell_l1_networking_core.egg-info/dependency_links.txt
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/response/resource_info/entities/attributes.py
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell_l1_networking_core.egg-info/not-zip-safe
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/response/resource_info/entities/validators.py
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell_l1_networking_core.egg-info/requires.txt
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/response/resource_info/entities/__init__.py
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell_l1_networking_core.egg-info/top_level.txt
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/response/resource_info/entities/blade.py
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell_l1_networking_core.egg-info/PKG-INFO
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/response/resource_info/entities/base.py
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell_l1_networking_core.egg-info/entry_points.txt
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/response/resource_info/entities/chassis.py
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell_l1_networking_core.egg-info/SOURCES.txt
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/request/requests_parser.py
+Filename: cloudshell-l1-networking-core-2.0.0/tests/__init__.py
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/request/__init__.py
+Filename: cloudshell-l1-networking-core-2.0.0/tests/test_smth.py
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/request/command_request.py
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/helper/xml_helper.py
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/__init__.py
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/helper/__init__.py
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/helper/xml_logger.py
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/tools/
 Comment: 
 
-Filename: cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/helper/runtime_configuration.py
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/__init__.py
+Comment: 
+
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/helper/
+Comment: 
+
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/
+Comment: 
+
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/request/
+Comment: 
+
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/command_executor.py
+Comment: 
+
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/driver_listener.py
+Comment: 
+
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/layer_one_driver_exception.py
+Comment: 
+
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/connection_handler.py
+Comment: 
+
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/__init__.py
+Comment: 
+
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/driver_commands_interface.py
+Comment: 
+
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/helper/xml_logger.py
+Comment: 
+
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/helper/logger.py
+Comment: 
+
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/helper/xml_helper.py
+Comment: 
+
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/helper/__init__.py
+Comment: 
+
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/helper/runtime_configuration.py
+Comment: 
+
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/resource_info/
+Comment: 
+
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/templates/
+Comment: 
+
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/command_responses_builder.py
+Comment: 
+
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/response_info.py
+Comment: 
+
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/__init__.py
+Comment: 
+
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/command_response.py
+Comment: 
+
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/resource_info/entities/
+Comment: 
+
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/resource_info/templates/
+Comment: 
+
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/resource_info/__init__.py
+Comment: 
+
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/resource_info/resource_info_builder.py
+Comment: 
+
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/resource_info/entities/chassis.py
+Comment: 
+
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/resource_info/entities/base.py
+Comment: 
+
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/resource_info/entities/blade.py
+Comment: 
+
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/resource_info/entities/validators.py
+Comment: 
+
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/resource_info/entities/__init__.py
+Comment: 
+
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/resource_info/entities/port.py
+Comment: 
+
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/resource_info/entities/attributes.py
+Comment: 
+
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/resource_info/templates/resource_template.xml
+Comment: 
+
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/resource_info/templates/resource_attribute_template.xml
+Comment: 
+
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/resource_info/templates/resource_incoming_map_template.xml
+Comment: 
+
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/templates/error_response.xml
+Comment: 
+
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/templates/command_response_template.xml
+Comment: 
+
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/templates/state_id_template.xml
+Comment: 
+
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/templates/responses_template.xml
+Comment: 
+
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/request/command_request.py
+Comment: 
+
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/request/requests_parser.py
+Comment: 
+
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/request/__init__.py
+Comment: 
+
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/tools/build_driver.py
+Comment: 
+
+Filename: cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/tools/__init__.py
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## Comparing `cloudshell-l1-networking-core-1.0.8/README.md` & `cloudshell-l1-networking-core-2.0.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # CloudShell L1 Networking Core
-[![Build status](https://travis-ci.org/QualiSystems/cloudshell-L1-networking-core.svg?branch=dev)](https://travis-ci.org/QualiSystems/cloudshell-L1-networking-core)
-[![Coverage Status](https://coveralls.io/repos/github/QualiSystems/cloudshell-L1-networking-core/badge.svg?branch=dev)](https://coveralls.io/github/QualiSystems/cloudshell-L1-networking-core?branch=dev)
-[![Dependency Status](https://dependencyci.com/github/QualiSystems/cloudshell-L1-networking-core/badge)](https://dependencyci.com/github/QualiSystems/cloudshell-L1-networking-core)
-[![Stories in Ready](https://badge.waffle.io/QualiSystems/cloudshell-L1-networking-core.svg?label=ready&title=Ready)](http://waffle.io/QualiSystems/cloudshell-L1-networking-core)
+[![Build status](https://github.com/QualiSystems/cloudshell-L1-networking-core/workflows/CI/badge.svg?branch=master)](https://github.com/QualiSystems/cloudshell-L1-networking-core/actions?query=branch%3Amaster)
+[![codecov](https://codecov.io/gh/QualiSystems/cloudshell-L1-networking-core/branch/master/graph/badge.svg)](https://codecov.io/gh/QualiSystems/cloudshell-L1-networking-core)
+[![PyPI version](https://badge.fury.io/py/cloudshell-l1-networking-core.svg)](https://badge.fury.io/py/cloudshell-L1-networking-core)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 
 
 This is core package which implements basic services and entities for L1 drivers.
 Follow [L1 Driver Guide](https://github.com/QualiSystems/shell-L1-template/blob/dev/DEVGUIDE.md) how to use them.
```

## Comparing `cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/tools/build_driver.py` & `cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/tools/build_driver.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,111 +2,121 @@
 import re
 import subprocess
 import sys
 import zipfile
 
 from cloudshell.layer_one.core.helper.runtime_configuration import RuntimeConfiguration
 
-CONFIG_FILE = 'package_config.yml'
-PACKAGE_FILES_KEY = 'PACKAGE_FILES'
-COLLECT_DEPENDENCIES_KEY = 'COLLECT_DEPENDENCIES'
+CONFIG_FILE = "package_config.yml"
+PACKAGE_FILES_KEY = "PACKAGE_FILES"
+COLLECT_DEPENDENCIES_KEY = "COLLECT_DEPENDENCIES"
 DEFAULT_FILES = [
-    'datamodel',
-    'main.py',
-    'install_driver.bat',
-    'driver_exe_template',
-    'requirements.txt',
-    'version.txt',
-    'INSTALL.txt']
+    "datamodel",
+    "main.py",
+    "install_driver.bat",
+    "driver_exe_template",
+    "requirements.txt",
+    "version.txt",
+    "INSTALL.txt",
+]
+DEFAULT_PACKAGES = ("pip", "wheel", "setuptools")
 
 
 def zip_driver(driver_path, driver_zip_file, files):
-    with zipfile.ZipFile(driver_zip_file, 'w', zipfile.ZIP_DEFLATED) as zip_file:
+    with zipfile.ZipFile(driver_zip_file, "w", zipfile.ZIP_DEFLATED) as zip_file:
         for name in files:
             _append_files(os.path.join(driver_path, name), zip_file)
 
 
 def _append_files(path, zip_file):
     if os.path.isfile(path):
-        rel_path = os.path.relpath(path, os.path.join(path, os.path.pardir, os.path.pardir))
+        rel_path = os.path.relpath(
+            path, os.path.join(path, os.path.pardir, os.path.pardir)
+        )
         zip_file.write(path, rel_path)
     else:
         for root, dirs, files in os.walk(path):
             for file_or_dir in files + dirs:
-                if not file_or_dir.endswith('.pyc'):
+                if not file_or_dir.endswith(".pyc"):
                     full_path = os.path.join(root, file_or_dir)
-                    rel_path = os.path.relpath(full_path, os.path.join(path, os.path.pardir, os.path.pardir))
+                    rel_path = os.path.relpath(
+                        full_path, os.path.join(path, os.path.pardir, os.path.pardir)
+                    )
                     zip_file.write(full_path, rel_path)
 
 
 def download_packages(packages_path, requirements):
-    subprocess.call(['pip', 'download', '-r', requirements, '-d', packages_path, '-q'])
+    subprocess.call(["pip", "download", "-r", requirements, "-d", packages_path, "-q"])
+    for lib_name in DEFAULT_PACKAGES:
+        subprocess.call(["pip", "download", lib_name, "-d", packages_path, "-q"])
 
 
 def _print_help():
     message = """Usage: build_driver [OPTIONS]
 
 Options:
     -h, --help  Show this message and exit.
     -i, --ignore-packages  Do not collect driver dependencies
     """
-    print(message)
+    print(message)  # noqa: T201
 
 
 def build(args=None):
     if not args:
         args = sys.argv
 
-    if '--help' in args[1:] or '-h' in args[1:]:
+    if "--help" in args[1:] or "-h" in args[1:]:
         _print_help()
         sys.exit(0)
 
-    # driver_path = os.path.abspath(os.path.join(os.path.dirname(__file__), os.pardir))
-    # driver_path = '/Users/yar/Projects/Quali/Github/LayerOne/cloudshell-L1-rome'
     driver_path = os.getcwd()
 
-    with open(os.path.join(driver_path, 'version.txt')) as ver_file:
+    with open(os.path.join(driver_path, "version.txt")) as ver_file:
         version = ver_file.read().strip()
 
     config = RuntimeConfiguration(os.path.join(driver_path, CONFIG_FILE))
 
     file_list = config.read_key(PACKAGE_FILES_KEY, [])
     file_list.extend(DEFAULT_FILES)
 
     driver_folder_name = os.path.basename(driver_path)
-    driver_name = re.sub('cloudshell-L1-', '', driver_folder_name, flags=re.IGNORECASE)
-    driver_name = re.sub('-', '_', driver_name)
+    driver_name = re.sub("cloudshell-L1-", "", driver_folder_name, flags=re.IGNORECASE)
+    driver_name = re.sub("-", "_", driver_name)
     if os.path.exists(os.path.join(driver_path, driver_name)):
         file_list.append(driver_name)
     else:
-        print('Cannot find driver src folder {}'.format(driver_name))
+        print(f"Cannot find driver src folder {driver_name}")  # noqa: T201
         sys.exit(1)
 
-    runtime_config = driver_name + '_runtime_config.yml'
+    runtime_config = f"{driver_name}_runtime_config.yml"
     if os.path.exists(os.path.join(driver_path, runtime_config)):
         file_list.append(runtime_config)
     else:
-        print('Cannot find driver runtime config {}'.format(runtime_config))
+        print("Cannot find driver runtime config {runtime_config}")  # noqa: T201
         sys.exit(1)
 
-    driver_folder_name_ver = '{}-{}'.format(driver_folder_name, version)
-    dist_path = os.path.join(driver_path, 'dist')
-    driver_zip_path = os.path.join(dist_path, driver_folder_name_ver + '.zip')
+    driver_folder_name_ver = f"{driver_folder_name}-{version}"
+    dist_path = os.path.join(driver_path, "dist")
+    driver_zip_path = os.path.join(dist_path, driver_folder_name_ver + ".zip")
 
     if not os.path.exists(dist_path):
         os.mkdir(dist_path)
 
-    if '--ignore-packages' not in args[1:] and '-i' not in args[1:] and config.read_key(COLLECT_DEPENDENCIES_KEY, True):
-        packages_path = os.path.join(driver_path, 'packages')
-        requirements_path = os.path.join(driver_path, 'requirements.txt')
+    if (
+        "--ignore-packages" not in args[1:]
+        and "-i" not in args[1:]
+        and config.read_key(COLLECT_DEPENDENCIES_KEY, True)
+    ):
+        packages_path = os.path.join(driver_path, "packages")
+        requirements_path = os.path.join(driver_path, "requirements.txt")
 
         if not os.path.exists(packages_path):
             os.mkdir(packages_path)
 
         download_packages(packages_path, requirements_path)
-        file_list.append('packages')
+        file_list.append("packages")
 
     zip_driver(driver_path, driver_zip_path, set(file_list))
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     build()
```

## Comparing `cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/connection_handler.py` & `cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/connection_handler.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,96 +1,103 @@
+from __future__ import annotations
+
+import logging
 import re
 import socket
 import traceback
 from threading import Thread
 
+from cloudshell.layer_one.core.command_executor import CommandExecutor
+from cloudshell.layer_one.core.helper.logger import get_l1_logger
 from cloudshell.layer_one.core.request.requests_parser import RequestsParser
-from cloudshell.layer_one.core.response.command_responses_builder import CommandResponsesBuilder
+from cloudshell.layer_one.core.response.command_responses_builder import (
+    CommandResponsesBuilder,
+)
+
+logger = get_l1_logger(name=__name__)
 
 
 class ConnectionClosedException(Exception):
     pass
 
 
 class ConnectionHandler(Thread):
-    """
-    Handle connections
-    """
-    REQUEST_END = r'</Commands>'
-    END_COMMAND = '\r\n'
+    """Handle connections."""
+
+    REQUEST_END = rb"</Commands>"
+    END_COMMAND = "\r\n"
     READ_TIMEOUT = 30
 
-    def __init__(self, connection_socket, command_executor, xml_logger, logger, buffer_size=2048):
-        """
-        :param connection_socket:
-        :type connection_socket: socket.socket
-        :param command_executor:
-        :type command_executor: cloudshell.layer_one.core.command_executor.CommandExecutor
-        :param xml_logger: 
-        :param logger: 
-        :param buffer_size: 
-        """
-        super(ConnectionHandler, self).__init__()
+    def __init__(
+        self,
+        connection_socket: socket.socket,
+        command_executor: CommandExecutor,
+        xml_logger: logging.Logger,
+        buffer_size: int = 2048,
+    ):
+        """Initialize class."""
+        super().__init__()
         self._connection_socket = connection_socket
         self._xml_logger = xml_logger
-        self._logger = logger
         self._command_executor = command_executor
         self._buffer_size = buffer_size
 
     def run(self):
-        """Start handling new connection"""
+        """Start handling new connection."""
         while True:
             try:
                 command_requests = self._read_request_commands()
                 responses = self._command_executor.execute_commands(command_requests)
                 self._send_response(
-                    CommandResponsesBuilder.to_string(CommandResponsesBuilder.build_xml_result(responses)))
+                    CommandResponsesBuilder.to_string(
+                        CommandResponsesBuilder.build_xml_result(responses)
+                    )
+                )
             except ConnectionClosedException:
                 self._connection_socket.close()
-                self._logger.debug('Connection closed by remote host')
+                logger.debug("Connection closed by remote host")
                 break
             except socket.timeout:
                 self._connection_socket.close()
-                self._logger.debug('Connection closed by timeout')
+                logger.debug("Connection closed by timeout")
                 break
             except Exception as ex:
                 self._send_response(
-                    CommandResponsesBuilder.to_string(CommandResponsesBuilder.build_xml_error(0, ex.message)))
+                    CommandResponsesBuilder.to_string(
+                        CommandResponsesBuilder.build_xml_error(0, str(ex))
+                    )
+                )
                 tb = traceback.format_exc()
-                self._logger.critical(tb)
+                logger.error(tb, exc_info=True)
                 self._connection_socket.close()
                 break
 
-    def _read_socket(self):
-        """
-        Read data from socket
-        :return: 
-        """
+    def _read_socket(self) -> str:
+        """Read data from socket."""
         self._connection_socket.settimeout(self.READ_TIMEOUT)
-        data = ''
+        data = b""
         while True:
             input_buffer = self._connection_socket.recv(self._buffer_size)
             if not input_buffer:
                 raise ConnectionClosedException()
             else:
-                data += input_buffer.strip()
+                # removed input_buffer.strip(), fixes
+                # https://github.com/QualiSystems/cloudshell-L1-networking-core/issues/25
+                data += input_buffer
                 if re.search(self.REQUEST_END, data):
                     break
 
-        return data
+        return data.decode()
 
-    def _read_request_commands(self):
-        """Read data and create requests"""
+    def _read_request_commands(self) -> list:
+        """Read data and create requests."""
         request_string = self._read_socket()
-        self._xml_logger.info(request_string.replace('\r', '') + "\n\n")
+        self._xml_logger.info(request_string.replace("\r", "") + "\n\n")
         requests = RequestsParser.parse_request_commands(request_string)
-        self._logger.debug(requests)
+        logger.debug(requests)
         return requests
 
-    def _send_response(self, response_string):
-        """
-        Send response
-        :param response_string: 
-        :return: 
-        """
-        self._connection_socket.send(response_string + self.END_COMMAND + self.END_COMMAND)
+    def _send_response(self, response_string: str):
+        """Send response."""
+        data = response_string + self.END_COMMAND + self.END_COMMAND
+        self._connection_socket.send(data.encode())
         self._xml_logger.info(response_string)
```

## Comparing `cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/driver_listener.py` & `cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/driver_listener.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,85 +1,95 @@
-#!/usr/bin/python
-# -*- coding: utf-8 -*-
-
 import os
 import socket
 import sys
 import threading
 import time
-from abc import ABCMeta
+from abc import ABC
 
 from cloudshell.layer_one.core.connection_handler import ConnectionHandler
+from cloudshell.layer_one.core.helper.logger import get_l1_logger
 from cloudshell.layer_one.core.helper.runtime_configuration import RuntimeConfiguration
 
+logger = get_l1_logger(name=__name__)
+
 
-class DriverListener(object):
-    """
-    Listen for new connection
-    """
-    __metaclass__ = ABCMeta
-    BACKLOG = 100
-    SERVER_HOST = '0.0.0.0'
+class DriverListener(ABC):
+    """Listen for new connection."""
+
+    BACKLOG = 10
+    SERVER_HOST = "0.0.0.0"
     SERVER_PORT = 1024
+    SOCKET_TIMEOUT = 900
 
-    def __init__(self, command_executor, xml_logger, command_logger):
+    def __init__(self, command_executor, xml_logger):
         self._command_executor = command_executor
-        self._command_logger = command_logger
         self._xml_logger = xml_logger
         self._is_running = False
 
-        self._debug_mode = RuntimeConfiguration().read_key('DEBUG_ENABLED', False)
+        self._debug_mode = RuntimeConfiguration().read_key("DEBUG_ENABLED", False)
 
-    def _initialize_socket(self, host, port):
-        """
-        Initialize socket, and start listening
-        :return: 
-        """
+    def _initialize_socket(self, host: str, port: str):
+        """Initialize socket, and start listening."""
         server_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         server_socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
-        self._command_logger.debug('New socket created')
+        logger.debug("New socket created")
         try:
             server_socket.bind((host, int(port)))
+            server_socket.settimeout(self.SOCKET_TIMEOUT)
             server_socket.listen(self.BACKLOG)
         except Exception as ex:
             # log will be  here
-            self._command_logger.error(str(ex))
+            logger.error(str(ex))
             raise
-        self._command_logger.debug("Listen address {0}:{1}".format(host, port))
+        logger.debug(f"Listen address {host}:{port}")
         self._is_running = True
         return server_socket
 
     def set_running(self, is_running):
         self._is_running = is_running
 
     def _wait_for_debugger_attach(self):
         pid = str(os.getpid())
 
         while not sys.gettrace():
-            self._command_logger.info(
-                "Waiting for a debugger to attach to this python driver process. (PID #{})".format(pid))
+            logger.info(
+                f"Waiting for a debugger to attach to this python driver process. "
+                f"(PID #{pid})"
+            )
             time.sleep(2)
 
-        self._command_logger.info("Debugger attached. (PID #{})".format(pid))
+        logger.info(f"Debugger attached. (PID #{pid})")
 
     def start_listening(self, host=None, port=None):
-        """Initialize socket and start listening"""
+        """Initialize socket and start listening."""
         host = host if host else self.SERVER_HOST
         port = port if port else self.SERVER_PORT
-        print "Listen address {0}:{1}".format(host, port)
+        print(f"Listen address {host}:{port}")  # noqa: T201
         server_socket = self._initialize_socket(host, port)
         while self._is_running:
-            connection, connection_data = server_socket.accept()
-            self._command_logger.debug("New connection from {0}:{1}".format(connection_data[0], connection_data[1]))
+            try:
+                connection, connection_data = server_socket.accept()
+            except socket.timeout:
+                map(  # noqa: C417
+                    lambda th: isinstance(th, ConnectionHandler) and th.join(),
+                    threading.enumerate(),
+                )
+                logger.debug("Terminating by idle timeout")
+                break
+            logger.debug(
+                f"New connection from {connection_data[0]}:{connection_data[1]}"
+            )
             if connection is not None:
-                request_handler = ConnectionHandler(connection, self._command_executor, self._xml_logger,
-                                                    self._command_logger)
+                request_handler = ConnectionHandler(
+                    connection,
+                    self._command_executor,
+                    self._xml_logger,
+                )
                 if self._debug_mode:
                     self._wait_for_debugger_attach()
                     try:
                         request_handler.run()
-                    except:
-                        self._command_logger.debug('ConnectionHandler Error')
+                    except Exception as err:
+                        logger.debug(f"ConnectionHandler Error: {str(err)}")
                 else:
                     request_handler.start()
-                    self._command_logger.debug("Threads count: {}".format(threading.activeCount()))
-
+                    logger.debug(f"Threads count: {threading.activeCount()}")
```

## Comparing `cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/response/command_response.py` & `cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/command_response.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-#!/usr/bin/python
-# -*- coding: utf-8 -*-
-
 from datetime import datetime
 
+from cloudshell.layer_one.core.request.command_request import CommandRequest
+
 
-class CommandResponse(object):
-    def __init__(self, command_request):
-        """
-        Command response
-        :param command_request:
-        :type command_request: cloudshell.layer_one.core.request.command_request.CommandRequest
-        """
+class CommandResponse:
+    def __init__(self, command_request: CommandRequest):
+        """Command response."""
         self.command_request = command_request
 
         # Response attributes
         self.success = False
         self.error = None
         self.log = None
         self.timestamp = datetime.now().strftime("%d.%m.%Y %H:%M:%S")
         self.response_info = None
 
     def __str__(self):
-        return 'Command: {0}, {1}, {2}'.format(self.command_request.command_name, self.command_request.command_id,
-                                               self.command_request.command_params)
+        return (
+            f"Command: {self.command_request.command_name}, "
+            f"{self.command_request.command_id}, "
+            f"{self.command_request.command_params}"
+        )
 
     def __repr__(self):
         return self.__str__()
```

## Comparing `cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/response/command_responses_builder.py` & `cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/command_responses_builder.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,88 +1,90 @@
-#!/usr/bin/python
-# -*- coding: utf-8 -*-
+from __future__ import annotations
 
 import os
 from xml.etree import ElementTree
 
 from cloudshell.layer_one.core.helper.xml_helper import XMLHelper
+from cloudshell.layer_one.core.response.command_response import CommandResponse
 
-ElementTree.register_namespace("", "http://schemas.qualisystems.com/ResourceManagement/DriverCommandResult.xsd")
+ElementTree.register_namespace(
+    "", "http://schemas.qualisystems.com/ResourceManagement/DriverCommandResult.xsd"
+)
 
 
-def full_path(relative_path):
+def full_path(relative_path: str) -> str:
     return os.path.join(os.path.dirname(__file__), relative_path)
 
 
-class CommandResponsesBuilder(object):
-    RESPONSES_TEMPLATE = XMLHelper.read_template(full_path('templates/responses_template.xml'))
-    COMMAND_RESPONSE_TEMPLATE = XMLHelper.read_template(full_path('templates/command_response_template.xml'))
-    ERROR_RESPONSE = XMLHelper.read_template(full_path('templates/error_response.xml'))
+class CommandResponsesBuilder:
+    RESPONSES_TEMPLATE = XMLHelper.read_template(
+        full_path("templates/responses_template.xml")
+    )
+    COMMAND_RESPONSE_TEMPLATE = XMLHelper.read_template(
+        full_path("templates/command_response_template.xml")
+    )
+    ERROR_RESPONSE = XMLHelper.read_template(full_path("templates/error_response.xml"))
 
     @staticmethod
-    def _build_command_response_node(command_response):
-        """
-        Build command response node
-        :param command_response: 
-        :type command_response: cloudshell.layer_one.core.response.command_response.CommandResponse
-        :return: 
-        :rtype: ElementTree.Element
-        """
-        command_response_node = XMLHelper.build_node_from_string(CommandResponsesBuilder.COMMAND_RESPONSE_TEMPLATE)
-        command_response_node.set('CommandName', command_response.command_request.command_name)
-        command_response_node.set('CommandId', command_response.command_request.command_id)
-        command_response_node.set('Success', str(command_response.success).lower())
+    def _build_command_response_node(
+        command_response: CommandResponse,
+    ) -> ElementTree.Element:
+        """Build command response node."""
+        command_response_node = XMLHelper.build_node_from_string(
+            CommandResponsesBuilder.COMMAND_RESPONSE_TEMPLATE
+        )
+        command_response_node.set(
+            "CommandName", command_response.command_request.command_name
+        )
+        command_response_node.set(
+            "CommandId", command_response.command_request.command_id
+        )
+        command_response_node.set("Success", str(command_response.success).lower())
 
-        timestamp_node = command_response_node.find('Timestamp')
+        timestamp_node = command_response_node.find("Timestamp")
         timestamp_node.text = command_response.timestamp
 
         if command_response.error is not None:
-            command_response_node.find('Error').text = command_response.error
+            command_response_node.find("Error").text = command_response.error
 
         if command_response.log is not None:
-            command_response_node.find('Log').text = command_response.log
+            command_response_node.find("Log").text = command_response.log
 
         if command_response.response_info is not None:
-            command_response_node.append(command_response.response_info.build_xml_node())
+            command_response_node.append(
+                command_response.response_info.build_xml_node()
+            )
         else:
-            command_response_node.append(ElementTree.Element('ResponseInfo'))
+            command_response_node.append(ElementTree.Element("ResponseInfo"))
         return command_response_node
 
     @staticmethod
-    def build_xml_result(responses):
-        """
-        Builde responses for list of responces objects
-        :param responses: 
-        :type responses: list
-        :return:
-        :rtype: xml.etree.ElementTree.Element
-        """
-        responses_node = XMLHelper.build_node_from_string(CommandResponsesBuilder.RESPONSES_TEMPLATE)
+    def build_xml_result(responses: list[CommandResponse]) -> ElementTree.Element:
+        """Build responses for list of responses objects."""
+        responses_node = XMLHelper.build_node_from_string(
+            CommandResponsesBuilder.RESPONSES_TEMPLATE
+        )
         tree = ElementTree.ElementTree(responses_node)
         for command_response in responses:
-            responses_node.append(CommandResponsesBuilder._build_command_response_node(command_response))
+            responses_node.append(
+                CommandResponsesBuilder._build_command_response_node(command_response)
+            )
         return tree.getroot()
 
     @staticmethod
-    def to_string(root):
-        """
-        Generate string for xml node
-        :param root: 
-        :return: 
-        :type str
-        """
-        return ElementTree.tostring(root, encoding='UTF-8', method='xml').replace('\n', '\r\n')
+    def to_string(root: ElementTree.Element) -> str:
+        """Generate string for xml node."""
+        return ElementTree.tostring(root, encoding="unicode", method="xml").replace(
+            "\n", "\r\n"
+        )
 
     @staticmethod
     def build_xml_error(error_code, log_message):
-        """
-        Build error response
-        :param error_code: 
-        :param log_message: 
-        :return: 
-        """
-        command_response_node = XMLHelper.build_node_from_string(CommandResponsesBuilder.ERROR_RESPONSE)
+        """Build error response."""
+        command_response_node = XMLHelper.build_node_from_string(
+            CommandResponsesBuilder.ERROR_RESPONSE
+        )
         tree = ElementTree.ElementTree(command_response_node)
         namespace = XMLHelper.get_node_namespace(command_response_node)
-        command_response_node.find(namespace + 'ErrorCode').text = str(error_code)
-        command_response_node.find(namespace + 'Log').text = str(log_message)
+        command_response_node.find(f"{namespace}ErrorCode").text = str(error_code)
+        command_response_node.find(f"{namespace}Log").text = str(log_message)
         return tree.getroot()
```

## Comparing `cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/response/response_info.py` & `cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/response_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,93 +1,97 @@
-#!/usr/bin/python
-# -*- coding: utf-8 -*-
+from __future__ import annotations
 
-from abc import ABCMeta, abstractmethod
+from abc import ABC, abstractmethod
+from collections.abc import Collection
 from xml.etree.ElementTree import Element
 
-from cloudshell.layer_one.core.response.resource_info.resource_info_builder import ResourceInfoBuilder
+from cloudshell.layer_one.core.response.resource_info.resource_info_builder import (
+    ResourceInfoBuilder,
+)
 
 
-class ResponseInfo(object):
-    """
-    Basic response builder
-    """
-    __metaclass__ = ABCMeta
+class ResponseInfo(ABC):
+    """Basic response builder."""
 
     @abstractmethod
     def build_xml_node(self):
-        """Build xml node"""
+        """Build xml node."""
         pass
 
     @staticmethod
     def _build_response_info_node():
-        return Element('ResponseInfo')
+        return Element("ResponseInfo")
 
 
 class ResourceDescriptionResponseInfo(ResponseInfo):
-    """Resource description builder"""
+    """Resource description builder."""
 
     def __init__(self, resource_info):
-        if isinstance(resource_info, list):
+        if isinstance(resource_info, Collection):
             self.resource_info_list = resource_info
         else:
             self.resource_info_list = [resource_info]
 
     def build_xml_node(self):
-        """Build xml node for resource description"""
+        """Build xml node for resource description."""
         response_info_node = self._build_response_info_node()
-        response_info_node.attrib['xmlns:xsi'] = "http://www.w3.org/2001/XMLSchema-instance"
-        response_info_node.attrib['xsi:type'] = "ResourceInfoResponse"
+        response_info_node.attrib[
+            "xmlns:xsi"
+        ] = "http://www.w3.org/2001/XMLSchema-instance"
+        response_info_node.attrib["xsi:type"] = "ResourceInfoResponse"
         for resource_info in self.resource_info_list:
-            response_info_node.append(ResourceInfoBuilder.build_resource_info_nodes(resource_info))
+            response_info_node.append(
+                ResourceInfoBuilder.build_resource_info_nodes(resource_info)
+            )
         return response_info_node
 
 
 class KeyValueResponseInfo(ResponseInfo):
-    """Simple key value builde, used for Get/Set attribute"""
+    """Simple key value builder, used for Get/Set attribute."""
 
-    def __init__(self, attributes_dict):
-        """
-        :param attributes_dict:
-        :type attributes_dict: dict
-        """
+    def __init__(self, attributes_dict: dict):
+        """Initialize class."""
         self.attributes_dict = attributes_dict
 
     def build_xml_node(self):
         response_info_node = self._build_response_info_node()
-        for name, value in self.attributes_dict.iteritems():
+        for name, value in self.attributes_dict.items():
             attribute_node = Element(name)
             attribute_node.text = value
             response_info_node.append(attribute_node)
         return response_info_node
 
 
 class GetStateIdResponseInfo(ResponseInfo):
-    ATTRIBUTE_NAME = 'StateId'
+    ATTRIBUTE_NAME = "StateId"
 
     def __init__(self, state_id):
         self._state_id = str(state_id)
 
     def build_xml_node(self):
         response_info_node = self._build_response_info_node()
-        response_info_node.attrib['xmlns:xsi'] = "http://www.w3.org/2001/XMLSchema-instance"
-        response_info_node.attrib['xsi:type'] = "StateInfo"
+        response_info_node.attrib[
+            "xmlns:xsi"
+        ] = "http://www.w3.org/2001/XMLSchema-instance"
+        response_info_node.attrib["xsi:type"] = "StateInfo"
         attribute_node = Element(self.ATTRIBUTE_NAME)
         attribute_node.text = self._state_id
         response_info_node.append(attribute_node)
         return response_info_node
 
 
 class AttributeValueResponseInfo(ResponseInfo):
-    ATTRIBUTE_NAME = 'Value'
+    ATTRIBUTE_NAME = "Value"
 
     def __init__(self, value):
-        self._value = value if value else 'NA'
+        self._value = value if value else "NA"
 
     def build_xml_node(self):
         response_info_node = self._build_response_info_node()
-        response_info_node.attrib['xmlns:xsi'] = "http://www.w3.org/2001/XMLSchema-instance"
-        response_info_node.attrib['xsi:type'] = "AttributeInfoResponse"
+        response_info_node.attrib[
+            "xmlns:xsi"
+        ] = "http://www.w3.org/2001/XMLSchema-instance"
+        response_info_node.attrib["xsi:type"] = "AttributeInfoResponse"
         attribute_node = Element(self.ATTRIBUTE_NAME)
         attribute_node.text = self._value
         response_info_node.append(attribute_node)
         return response_info_node
```

## Comparing `cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/response/resource_info/resource_info_builder.py` & `cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/resource_info/resource_info_builder.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-#!/usr/bin/python
-# -*- coding: utf-8 -*-
-
 import os
+from xml.etree.ElementTree import Element
 
 from cloudshell.layer_one.core.helper.xml_helper import XMLHelper
+from cloudshell.layer_one.core.response.resource_info.entities.base import (
+    Attribute,
+    ResourceInfo,
+)
 
 
-def full_path(relative_path):
+def full_path(relative_path: str) -> str:
     return os.path.join(os.path.dirname(__file__), relative_path)
 
 
-class ResourceInfoBuilder(object):
-    """
-    Build resource info node
-    """
-    RESOURCE_TEMPLATE = XMLHelper.read_template(full_path('templates/resource_template.xml'))
-    ATTRIBUTE_TEMPLATE = XMLHelper.read_template(full_path('templates/resource_attribute_template.xml'))
-    MAPPING_TEMPLATE = XMLHelper.read_template(full_path('templates/resource_incoming_map_template.xml'))
+class ResourceInfoBuilder:
+    """Build resource info node."""
+
+    RESOURCE_TEMPLATE = XMLHelper.read_template(
+        full_path("templates/resource_template.xml")
+    )
+    ATTRIBUTE_TEMPLATE = XMLHelper.read_template(
+        full_path("templates/resource_attribute_template.xml")
+    )
+    MAPPING_TEMPLATE = XMLHelper.read_template(
+        full_path("templates/resource_incoming_map_template.xml")
+    )
 
     @staticmethod
-    def _build_resource_node(resource_info):
-        """
-        Build resource xml node
-        :param resource_info:
-        :type resource_info: cloudshell.layer_one.core.response.entities.base.ResourceInfo
-        :return: Resource node
-        :rtype: xml.etree.ElementTree.Element
-        """
+    def _build_resource_node(resource_info: ResourceInfo) -> Element:
+        """Build resource xml node."""
         node = XMLHelper.build_node_from_string(ResourceInfoBuilder.RESOURCE_TEMPLATE)
         node.set("Name", resource_info.name)
         node.set("ResourceFamilyName", resource_info.family_name)
         node.set("ResourceModelName", resource_info.model_name)
         node.set("SerialNumber", resource_info.serial_number)
         node.set("Address", resource_info.address)
         attributes_node = node.find("ResourceAttributes")
@@ -38,63 +39,46 @@
             attribute_node = ResourceInfoBuilder._build_attribute_node(attribute)
             attributes_node.append(attribute_node)
         if resource_info.mapping:
             node.append(ResourceInfoBuilder._build_mapping_node(resource_info.mapping))
         return node
 
     @staticmethod
-    def _build_attribute_node(attribute):
-        """
-        Build attribute node
-        :param attribute: 
-        :type attribute: cloudshell.layer_one.core.response.entities.base.Attribute
+    def _build_attribute_node(attribute: Attribute) -> Element:
+        """Build attribute node.
+
+        :type attribute: cloudshell.layer_one.core.response.resource_info.entities.base.Attribute  # noqa: E501
         :return: Attribute node
         :rtype: xml.etree.ElementTree.Element
         """
         node = XMLHelper.build_node_from_string(ResourceInfoBuilder.ATTRIBUTE_TEMPLATE)
         node.set("Name", attribute.name)
         node.set("Type", attribute.type)
         node.set("Value", attribute.value)
         return node
 
     @staticmethod
-    def _build_mapping_node(mapping_node):
-        """
-        Build mapping node
-        :param mapping_node: 
-        :type mapping_node: cloudshell.layer_one.core.response.entities.base.ResourceInfo
-        :return: Mapping node
-        :rtype: xml.etree.ElementTree.Element
-        """
+    def _build_mapping_node(mapping_node: ResourceInfo) -> Element:
+        """Build mapping node."""
         node = XMLHelper.build_node_from_string(ResourceInfoBuilder.MAPPING_TEMPLATE)
         child_incoming_node = node.find("IncomingMapping")
         child_incoming_node.text = mapping_node.address
         return node
 
     @staticmethod
-    def _build_resource_child_nodes(node, resource):
-        """
-        Build resource nodes for children recursively
-        :param resource:
-        :type resource: cloudshell.layer_one.core.response.entities.base.ResourceInfo
-        :param node: 
-        :type node: xml.etree.ElementTree.Element
-        """
+    def _build_resource_child_nodes(node: Element, resource: ResourceInfo):
+        """Build resource nodes for children recursively."""
         if len(resource.child_resources) > 0:
-            child_resources_node = node.find('ChildResources')
+            child_resources_node = node.find("ChildResources")
             for child_resource in resource.child_resources.values():
                 child_node = ResourceInfoBuilder._build_resource_node(child_resource)
                 child_resources_node.append(child_node)
-                ResourceInfoBuilder._build_resource_child_nodes(child_node, child_resource)
+                ResourceInfoBuilder._build_resource_child_nodes(
+                    child_node, child_resource
+                )
 
     @staticmethod
-    def build_resource_info_nodes(base_resource):
-        """
-        Build tree of xml nodes for resource tree
-        :param base_resource:
-        :type base_resource: cloudshell.layer_one.core.response.entities.base.ResourceInfo
-        :return:
-        :type: xml.etree.ElementTree.Element
-        """
+    def build_resource_info_nodes(base_resource: ResourceInfo) -> Element:
+        """Build tree of xml nodes for resource tree."""
         resource_node = ResourceInfoBuilder._build_resource_node(base_resource)
         ResourceInfoBuilder._build_resource_child_nodes(resource_node, base_resource)
         return resource_node
```

## Comparing `cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/response/resource_info/entities/port.py` & `cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/resource_info/entities/port.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,69 +1,75 @@
-#!/usr/bin/python
-# -*- coding: utf-8 -*-
 import re
 
-from cloudshell.layer_one.core.response.resource_info.entities.attributes import StringAttribute, NumericAttribute, \
-    BooleanAttribute
+from cloudshell.layer_one.core.response.resource_info.entities.attributes import (
+    BooleanAttribute,
+    NumericAttribute,
+    StringAttribute,
+)
 from cloudshell.layer_one.core.response.resource_info.entities.base import ResourceInfo
-from cloudshell.layer_one.core.response.resource_info.entities.validators import EntityValidator
+from cloudshell.layer_one.core.response.resource_info.entities.validators import (
+    EntityValidator,
+)
 
 
 class Port(ResourceInfo):
-    """
-    Port resource entity
-    """
-    NAME_TEMPLATE = 'Port {}'
-    FAMILY_NAME = 'L1 Switch Port'
-    MODEL_NAME = 'Generic L1 Port'
+    """Port resource entity."""
 
-    def __init__(self, resource_id, model_name=None, serial_number='NA', mapping=None):
+    NAME_TEMPLATE = "Port {}"
+    FAMILY_NAME = "L1 Switch Port"
+    MODEL_NAME = "Generic L1 Port"
+
+    def __init__(self, resource_id, model_name=None, serial_number=None, mapping=None):
         model_name = model_name or self.MODEL_NAME
-        name = self.NAME_TEMPLATE.format(EntityValidator.validate_id_for_name_template(resource_id))
-        super(Port, self).__init__(resource_id, name, self.FAMILY_NAME, model_name, serial_number, mapping)
+        name = self.NAME_TEMPLATE.format(
+            EntityValidator.validate_id_for_name_template(resource_id)
+        )
+        super().__init__(
+            resource_id, name, self.FAMILY_NAME, model_name, serial_number, mapping
+        )
 
     def set_model_name(self, value):
         if value:
-            self.attributes.append(StringAttribute('Model Name', value))
+            self.attributes.append(StringAttribute("Model Name", value))
 
     def set_protocol_value(self, value):
         if value:
-            self.attributes.append(StringAttribute('Protocol Value', value))
+            self.attributes.append(StringAttribute("Protocol Value", value))
 
     def set_protocol_type_value(self, value):
         if value:
-            self.attributes.append(StringAttribute('Protocol Type Value', value))
+            self.attributes.append(StringAttribute("Protocol Type Value", value))
 
     def set_duplex(self, value):
         if value:
-            if re.match(r'full', value, flags=re.IGNORECASE):
-                num_value = '3'
+            if re.match(r"full", value, flags=re.IGNORECASE):
+                num_value = "3"
             else:
-                num_value = '2'
-            self.attributes.append(NumericAttribute('Duplex', num_value))
+                num_value = "2"
+            self.attributes.append(NumericAttribute("Duplex", num_value))
 
     def set_auto_negotiation(self, value):
         if not isinstance(value, bool):
             return
 
         if value:
             bool_value = BooleanAttribute.TRUE
         else:
             bool_value = BooleanAttribute.FALSE
 
-        self.attributes.append(BooleanAttribute('Auto Negotiation', bool_value))
+        self.attributes.append(BooleanAttribute("Auto Negotiation", bool_value))
 
     def set_rx_power(self, value):
         if value:
-            self.attributes.append(StringAttribute('Rx Power (dBm)', value))
+            self.attributes.append(StringAttribute("Rx Power (dBm)", value))
 
     def set_tx_power(self, value):
         if value:
-            self.attributes.append(StringAttribute('Tx Power (dBm)', value))
+            self.attributes.append(StringAttribute("Tx Power (dBm)", value))
 
     def set_port_speed(self, value):
         if value:
-            self.attributes.append(StringAttribute('Port Speed', value))
+            self.attributes.append(StringAttribute("Port Speed", value))
 
     def set_wavelength(self, value):
         if value:
-            self.attributes.append(StringAttribute('Wavelength', value))
+            self.attributes.append(StringAttribute("Wavelength", value))
```

## Comparing `cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/response/resource_info/entities/blade.py` & `cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/resource_info/entities/chassis.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,38 @@
-#!/usr/bin/python
-# -*- coding: utf-8 -*-
-from cloudshell.layer_one.core.response.resource_info.entities.attributes import StringAttribute
+from cloudshell.layer_one.core.response.resource_info.entities.attributes import (
+    StringAttribute,
+)
 from cloudshell.layer_one.core.response.resource_info.entities.base import ResourceInfo
-from cloudshell.layer_one.core.response.resource_info.entities.validators import EntityValidator
+from cloudshell.layer_one.core.response.resource_info.entities.validators import (
+    EntityValidator,
+)
 
 
-class Blade(ResourceInfo):
-    """Blade resource entity"""
-    NAME_TEMPLATE = 'Blade {}'
-    FAMILY_NAME = 'L1 Switch Blade'
-    MODEL_NAME = 'Generic L1 Module'
-
-    def __init__(self, resource_id, model_name=None, serial_number='NA'):
-        model_name = model_name or self.MODEL_NAME
-        name = self.NAME_TEMPLATE.format(EntityValidator.validate_id_for_name_template(resource_id))
-        super(Blade, self).__init__(resource_id, name, self.FAMILY_NAME, model_name, serial_number)
+class Chassis(ResourceInfo):
+    """Chassis resource entity."""
+
+    NAME_TEMPLATE = "Chassis {}"
+    FAMILY_NAME = "L1 Switch"
+
+    def __init__(self, resource_id, address, model_name, serial_number=None):
+        self._address = address
+        name = self.NAME_TEMPLATE.format(
+            EntityValidator.validate_id_for_name_template(resource_id)
+        )
+        family_name = self.FAMILY_NAME
+        super().__init__(resource_id, name, family_name, model_name, serial_number)
+
+    @property
+    def address(self):
+        return self._address
 
     def set_model_name(self, value):
         if value:
-            self.attributes.append(StringAttribute('Model Name', value))
+            self.attributes.append(StringAttribute("Model Name", value))
 
     def set_serial_number(self, value):
         if value:
-            self.attributes.append(StringAttribute('Serial Number', value))
+            self.attributes.append(StringAttribute("Serial Number", value))
+
+    def set_os_version(self, value):
+        if value:
+            self.attributes.append(StringAttribute("OS Version", value))
```

## Comparing `cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/response/resource_info/entities/base.py` & `cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/response/resource_info/entities/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,78 +1,65 @@
-#!/usr/bin/python
-# -*- coding: utf-8 -*-
+class ResourceInfo:
+    """Basic resource info entity."""
 
-
-class ResourceInfo(object):
-    """
-    Basic resource info entity
-    """
-
-    def __init__(self, resource_id, name, family_name, model_name, serial_number, mapping=None):
+    def __init__(
+        self, resource_id, name, family_name, model_name, serial_number, mapping=None
+    ):
         self.resource_id = str(resource_id)
         self.name = name
         self.family_name = family_name
         self.model_name = model_name
-        self.serial_number = serial_number
+        self.serial_number = serial_number or "NA"
 
         self.child_resources = {}
         self.attributes = []
         self._parent_resource = None
         self.mapping = mapping
 
     def set_parent_resource(self, parent_resource):
-        """
-        Set parent
+        """Set parent.
+
         :param parent_resource:
         :type parent_resource: ResourceInfo
-        :return: 
+        :return:
         """
         self._parent_resource = parent_resource
         parent_resource.child_resources[self.resource_id] = self
 
     @property
     def address(self):
-        """
-        Resource address
-        :return: 
-        """
+        """Resource address."""
         if self._parent_resource and self._parent_resource.address:
-            address = '{0}/{1}'.format(self._parent_resource.address, self.resource_id)
+            address = f"{self._parent_resource.address}/{self.resource_id}"
         else:
             address = self.resource_id
         return address
 
     def __str__(self):
-        return '{0}, {1}'.format(self.name, self.address)
+        return f"{self.name}, {self.address}"
 
     def __repr__(self):
         return self.__str__()
 
     def add_mapping(self, resource_info):
-        """
-        Resource mapping, used for port resources
-        :param resource_info: 
-        :return: 
-        """
+        """Resource mapping, used for port resources."""
         self.mapping = resource_info
 
 
-class Attribute(object):
-    """
-    Basic attribute entity
-    """
-    NUMERIC = 'Numeric'
-    STRING = 'String'
-    BOOLEAN = 'Boolean'
+class Attribute:
+    """Basic attribute entity."""
 
-    DEFAULT_VALUE = 'NA'
+    NUMERIC = "Numeric"
+    STRING = "String"
+    BOOLEAN = "Boolean"
+    DEFAULT_VALUE = "NA"
 
     def __init__(self, name, attr_type, value):
         self.name = name
         self.type = attr_type
         self.value = value
 
     def __str__(self):
-        return '{0}: {1}'.format(self.name, self.value)
+        return f"{self.name}: {self.value}"
 
     def __repr__(self):
         return self.__str__()
```

## Comparing `cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/request/requests_parser.py` & `cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/request/requests_parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,36 @@
-#!/usr/bin/python
-# -*- coding: utf-8 -*-
+from __future__ import annotations
+
 from collections import defaultdict
+from xml.etree.ElementTree import Element
 
 from cloudshell.layer_one.core.helper.xml_helper import XMLHelper
 from cloudshell.layer_one.core.request.command_request import CommandRequest
 
 
-class RequestsParser(object):
-    """
-    Parse request data and build command requests
-    """
-
-    def __init__(self, logger):
-        self.logger = logger
+class RequestsParser:
+    """Parse request data and build command requests."""
 
     @staticmethod
-    def _build_command_instance(command_node):
-        """
-        Build command instance for command node
-        :param command_node: 
-        :type command_node: xml.etree.ElementTree.Element
-        :return:
-        :rtype: cloudshell.layer_one.core.entities.command.Command
-        """
-        command_name = command_node.get('CommandName')
-        command_id = command_node.get('CommandId')
+    def _build_command_instance(command_node: Element) -> CommandRequest:
+        """Build command instance for command node."""
+        command_name = command_node.get("CommandName")
+        command_id = command_node.get("CommandId")
         command_params = defaultdict(list)
         namespace = XMLHelper.get_node_namespace(command_node)
-        parameters_node = command_node.find(namespace + 'Parameters')
+        parameters_node = command_node.find(namespace + "Parameters")
 
         if parameters_node is not None:
             for param_node in parameters_node:
-                key = param_node.tag.replace(namespace, '')
+                key = param_node.tag.replace(namespace, "")
                 command_params[key].append(param_node.text)
 
         return CommandRequest(command_name, command_id, command_params)
 
     @staticmethod
-    def parse_request_commands(xml_request):
-        """
-        Parse xml request and create command instances
-        :param xml_request: 
-        :return:
-        :rtype: list
-        """
+    def parse_request_commands(xml_request: str) -> list:
+        """Parse xml request and create command instances."""
         commands = []
         request_node = XMLHelper.build_node_from_string(xml_request)
         for command_node in request_node:
             commands.append(RequestsParser._build_command_instance(command_node))
         return commands
```

## Comparing `cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/helper/xml_logger.py` & `cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/helper/xml_logger.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import os
 import re
 
 
-class XMLLogger(object):
-    """Simple logger used for xml"""
+class XMLLogger:
+    """Simple logger used for xml."""
+
     PASSWORD_DISPLAY = "Password>*******</"
 
-    def __init__(self, path):
+    def __init__(self, path: str):
         try:
             os.makedirs(os.path.dirname(path))
-        except:
+        except Exception:
             pass
-        self._descriptor = open(path, 'w+')
+        self._descriptor = open(path, "w+")
 
     def __del__(self):
         self._descriptor.close()
 
-    def _write_data(self, data):
-        self._descriptor.write(data + '\r\n')
+    def _write_data(self, data: str):
+        self._descriptor.write(data + "\r\n")
         self._descriptor.flush()
 
-    def info(self, data):
+    def info(self, data: str):
         self._write_data(self._prepare_output(data))
 
-    def _prepare_output(self, data):
+    def _prepare_output(self, data: str) -> str:
         return re.sub(r"Password>.*?</", self.PASSWORD_DISPLAY, data)
```

## Comparing `cloudshell-l1-networking-core-1.0.8/cloudshell/layer_one/core/helper/runtime_configuration.py` & `cloudshell-l1-networking-core-2.0.0/cloudshell/layer_one/core/helper/runtime_configuration.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,57 +1,52 @@
+from __future__ import annotations
+
 import os
 import re
+from typing import Any
 
-from yaml import load
+from yaml import Loader, load
 
-_instance = None
 
+class Singleton(type):
+    _instances = {}
 
-class Singleton(object):
-    _instance = None
+    def __call__(cls, *args, **kwargs):
+        if cls not in cls._instances:
+            cls._instances[cls] = super().__call__(*args, **kwargs)
+        return cls._instances[cls]
 
-    def __new__(cls, *args, **kwargs):
-        if not isinstance(cls._instance, cls):
-            cls._instance = object.__new__(cls, *args, **kwargs)
-        return cls._instance
 
+class RuntimeConfiguration(metaclass=Singleton):
+    """Runtime configuration helper."""
 
-class RuntimeConfiguration(Singleton):
-    """
-    Runtime configuration helper
-    """
-    KEY_SEPARATOR_LIST = ['\.', '\:', '\/']
+    KEY_SEPARATOR_LIST = [r"\.", r"\:", r"\/"]
 
-    def __init__(self, config_path=None):
-        self._key_separator_pattern = r'|'.join(self.KEY_SEPARATOR_LIST)
-        if not hasattr(self, '_configuration'):
+    def __init__(self, config_path: str = None):
+        self._key_separator_pattern = r"|".join(self.KEY_SEPARATOR_LIST)
+        if not hasattr(self, "_configuration"):
             self._configuration = self._read_configuration(config_path)
 
     @property
-    def configuration(self):
-        """
-        Configuration property
-        :return: 
-        :rtype: dict
-        """
+    def configuration(self) -> dict:
+        """Configuration property."""
         return self._configuration
 
-    def _read_configuration(self, config_path):
-        """Read configuration from file if exists or use default"""
-        if config_path and os.path.isfile(config_path) and os.access(config_path, os.R_OK):
-            with open(config_path, 'r') as config:
-                return load(config)
-
-    def read_key(self, complex_key, default_value=None):
-        """
-        Value for complex key like CLI.PORTS
-        :param complex_key:
-        :param default_value: Default value
-        :return:
-        """
+    def _read_configuration(self, config_path: str) -> dict:
+        """Read configuration from file if exists or use default."""
+        if (
+            config_path
+            and os.path.isfile(config_path)
+            and os.access(config_path, os.R_OK)
+        ):
+            with open(config_path) as config:
+                return load(config, Loader=Loader)
+
+    def read_key(self, complex_key: str, default_value: Any = None):
+        """Value for complex key like CLI.PORTS."""
         value = self.configuration
         for key in re.split(self._key_separator_pattern, complex_key):
             if isinstance(value, dict):
                 value = value.get(key)
             else:
                 return default_value
```

