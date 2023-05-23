# Comparing `tmp/netznoe-smartmeter-portal-api-1.0.1.tar.gz` & `tmp/netznoe-smartmeter-portal-api-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netznoe-smartmeter-portal-api-1.0.1.tar", last modified: Sun Apr 16 20:35:56 2023, max compression
+gzip compressed data, was "netznoe-smartmeter-portal-api-1.0.2.tar", last modified: Tue May 23 07:35:11 2023, max compression
```

## Comparing `netznoe-smartmeter-portal-api-1.0.1.tar` & `netznoe-smartmeter-portal-api-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 schue     (1000) schue     (1000)        0 2023-04-16 20:35:56.896750 netznoe-smartmeter-portal-api-1.0.1/
--rw-r--r--   0 schue     (1000) schue     (1000)     1073 2023-04-16 11:53:11.000000 netznoe-smartmeter-portal-api-1.0.1/LICENSE
--rw-r--r--   0 schue     (1000) schue     (1000)     4569 2023-04-16 20:35:56.896750 netznoe-smartmeter-portal-api-1.0.1/PKG-INFO
--rw-r--r--   0 schue     (1000) schue     (1000)     3681 2023-04-16 20:29:54.000000 netznoe-smartmeter-portal-api-1.0.1/README.md
--rw-r--r--   0 schue     (1000) schue     (1000)       98 2023-04-16 15:15:10.000000 netznoe-smartmeter-portal-api-1.0.1/pyproject.toml
--rw-r--r--   0 schue     (1000) schue     (1000)     1148 2023-04-16 20:35:56.897750 netznoe-smartmeter-portal-api-1.0.1/setup.cfg
--rw-r--r--   0 schue     (1000) schue     (1000)       37 2023-04-16 15:09:50.000000 netznoe-smartmeter-portal-api-1.0.1/setup.py
-drwxr-xr-x   0 schue     (1000) schue     (1000)        0 2023-04-16 20:35:56.893750 netznoe-smartmeter-portal-api-1.0.1/src/
-drwxr-xr-x   0 schue     (1000) schue     (1000)        0 2023-04-16 20:35:56.895750 netznoe-smartmeter-portal-api-1.0.1/src/netznoe_smartmeter_portal_api/
--rw-r--r--   0 schue     (1000) schue     (1000)      193 2023-04-16 10:39:28.000000 netznoe-smartmeter-portal-api-1.0.1/src/netznoe_smartmeter_portal_api/__init__.py
--rw-r--r--   0 schue     (1000) schue     (1000)     6395 2023-04-16 12:12:24.000000 netznoe-smartmeter-portal-api-1.0.1/src/netznoe_smartmeter_portal_api/api.py
--rw-r--r--   0 schue     (1000) schue     (1000)     1247 2023-04-16 11:12:02.000000 netznoe-smartmeter-portal-api-1.0.1/src/netznoe_smartmeter_portal_api/models.py
-drwxr-xr-x   0 schue     (1000) schue     (1000)        0 2023-04-16 20:35:56.896750 netznoe-smartmeter-portal-api-1.0.1/src/netznoe_smartmeter_portal_api.egg-info/
--rw-r--r--   0 schue     (1000) schue     (1000)     4569 2023-04-16 20:35:56.000000 netznoe-smartmeter-portal-api-1.0.1/src/netznoe_smartmeter_portal_api.egg-info/PKG-INFO
--rw-r--r--   0 schue     (1000) schue     (1000)      466 2023-04-16 20:35:56.000000 netznoe-smartmeter-portal-api-1.0.1/src/netznoe_smartmeter_portal_api.egg-info/SOURCES.txt
--rw-r--r--   0 schue     (1000) schue     (1000)        1 2023-04-16 20:35:56.000000 netznoe-smartmeter-portal-api-1.0.1/src/netznoe_smartmeter_portal_api.egg-info/dependency_links.txt
--rw-r--r--   0 schue     (1000) schue     (1000)       33 2023-04-16 20:35:56.000000 netznoe-smartmeter-portal-api-1.0.1/src/netznoe_smartmeter_portal_api.egg-info/requires.txt
--rw-r--r--   0 schue     (1000) schue     (1000)       30 2023-04-16 20:35:56.000000 netznoe-smartmeter-portal-api-1.0.1/src/netznoe_smartmeter_portal_api.egg-info/top_level.txt
+drwxr-xr-x   0 schue     (1000) schue     (1000)        0 2023-05-23 07:35:11.359799 netznoe-smartmeter-portal-api-1.0.2/
+-rw-r--r--   0 schue     (1000) schue     (1000)     1073 2023-04-16 11:53:11.000000 netznoe-smartmeter-portal-api-1.0.2/LICENSE
+-rw-r--r--   0 schue     (1000) schue     (1000)     4732 2023-05-23 07:35:11.360799 netznoe-smartmeter-portal-api-1.0.2/PKG-INFO
+-rw-r--r--   0 schue     (1000) schue     (1000)     3843 2023-04-16 20:40:16.000000 netznoe-smartmeter-portal-api-1.0.2/README.md
+-rw-r--r--   0 schue     (1000) schue     (1000)       98 2023-04-16 15:15:10.000000 netznoe-smartmeter-portal-api-1.0.2/pyproject.toml
+-rw-r--r--   0 schue     (1000) schue     (1000)     1148 2023-05-23 07:35:11.360799 netznoe-smartmeter-portal-api-1.0.2/setup.cfg
+-rw-r--r--   0 schue     (1000) schue     (1000)       37 2023-04-16 15:09:50.000000 netznoe-smartmeter-portal-api-1.0.2/setup.py
+drwxr-xr-x   0 schue     (1000) schue     (1000)        0 2023-05-23 07:35:11.356799 netznoe-smartmeter-portal-api-1.0.2/src/
+drwxr-xr-x   0 schue     (1000) schue     (1000)        0 2023-05-23 07:35:11.358799 netznoe-smartmeter-portal-api-1.0.2/src/netznoe_smartmeter_portal_api/
+-rw-r--r--   0 schue     (1000) schue     (1000)      193 2023-04-16 10:39:28.000000 netznoe-smartmeter-portal-api-1.0.2/src/netznoe_smartmeter_portal_api/__init__.py
+-rw-r--r--   0 schue     (1000) schue     (1000)     6395 2023-04-25 19:25:10.000000 netznoe-smartmeter-portal-api-1.0.2/src/netznoe_smartmeter_portal_api/api.py
+-rw-r--r--   0 schue     (1000) schue     (1000)     1033 2023-04-16 20:45:06.000000 netznoe-smartmeter-portal-api-1.0.2/src/netznoe_smartmeter_portal_api/models.py
+drwxr-xr-x   0 schue     (1000) schue     (1000)        0 2023-05-23 07:35:11.359799 netznoe-smartmeter-portal-api-1.0.2/src/netznoe_smartmeter_portal_api.egg-info/
+-rw-r--r--   0 schue     (1000) schue     (1000)     4732 2023-05-23 07:35:11.000000 netznoe-smartmeter-portal-api-1.0.2/src/netznoe_smartmeter_portal_api.egg-info/PKG-INFO
+-rw-r--r--   0 schue     (1000) schue     (1000)      466 2023-05-23 07:35:11.000000 netznoe-smartmeter-portal-api-1.0.2/src/netznoe_smartmeter_portal_api.egg-info/SOURCES.txt
+-rw-r--r--   0 schue     (1000) schue     (1000)        1 2023-05-23 07:35:11.000000 netznoe-smartmeter-portal-api-1.0.2/src/netznoe_smartmeter_portal_api.egg-info/dependency_links.txt
+-rw-r--r--   0 schue     (1000) schue     (1000)       33 2023-05-23 07:35:11.000000 netznoe-smartmeter-portal-api-1.0.2/src/netznoe_smartmeter_portal_api.egg-info/requires.txt
+-rw-r--r--   0 schue     (1000) schue     (1000)       30 2023-05-23 07:35:11.000000 netznoe-smartmeter-portal-api-1.0.2/src/netznoe_smartmeter_portal_api.egg-info/top_level.txt
```

### Comparing `netznoe-smartmeter-portal-api-1.0.1/LICENSE` & `netznoe-smartmeter-portal-api-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `netznoe-smartmeter-portal-api-1.0.1/PKG-INFO` & `netznoe-smartmeter-portal-api-1.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netznoe-smartmeter-portal-api
-Version: 1.0.1
+Version: 1.0.2
 Summary: An unofficial python implementation of the NetzNÖ Smartmeter Portal API
 Home-page: https://github.com/schue30/NetzNoe-SmartmeterPortal-Api
 Author: Mathias Schuepany
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -117,7 +117,12 @@
 | values                           | consumption                    | kWh  |
 | gridUsageLeftoverValues          | grid_usage_leftover            | kWh  |
 | selfCoverageValues               | self_coverage                  | kWh  |
 | selfCoverageRenewableEnergyValue | self_coverage_renewable_energy | kWh  |
 | jointTenancyProportionValues     | joint_tenancy_proportion       | kWh  |
 | peakDemands                      | peak_demands                   | kW   |
 | is_mixed                         | *< ignored >*                  |      |
+
+## Legal
+
+Disclaimer: This is not affiliated, endorsed or certified by Netz NÖ. This is an independent and unofficial API.
+Provided as is. Use at your own risk.
```

### Comparing `netznoe-smartmeter-portal-api-1.0.1/README.md` & `netznoe-smartmeter-portal-api-1.0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -95,7 +95,12 @@
 | values                           | consumption                    | kWh  |
 | gridUsageLeftoverValues          | grid_usage_leftover            | kWh  |
 | selfCoverageValues               | self_coverage                  | kWh  |
 | selfCoverageRenewableEnergyValue | self_coverage_renewable_energy | kWh  |
 | jointTenancyProportionValues     | joint_tenancy_proportion       | kWh  |
 | peakDemands                      | peak_demands                   | kW   |
 | is_mixed                         | *< ignored >*                  |      |
+
+## Legal
+
+Disclaimer: This is not affiliated, endorsed or certified by Netz NÖ. This is an independent and unofficial API.
+Provided as is. Use at your own risk.
```

### Comparing `netznoe-smartmeter-portal-api-1.0.1/setup.cfg` & `netznoe-smartmeter-portal-api-1.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = netznoe-smartmeter-portal-api
-version = 1.0.1
+version = 1.0.2
 description = An unofficial python implementation of the NetzNÖ Smartmeter Portal API
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 author = Mathias Schuepany
 url = https://github.com/schue30/NetzNoe-SmartmeterPortal-Api
 classifiers = 
@@ -19,15 +19,15 @@
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 
 [options]
 python_requires = >=3.7
 install_requires = 
-	requests>=2.28.2
+	requests>=2.31.0
 	pendulum>=2.1.2
 package_dir = 
 	=src
 packages = find:
 
 [options.packages.find]
 where = src
```

### Comparing `netznoe-smartmeter-portal-api-1.0.1/src/netznoe_smartmeter_portal_api/api.py` & `netznoe-smartmeter-portal-api-1.0.2/src/netznoe_smartmeter_portal_api/api.py`

 * *Files identical despite different names*

### Comparing `netznoe-smartmeter-portal-api-1.0.1/src/netznoe_smartmeter_portal_api/models.py` & `netznoe-smartmeter-portal-api-1.0.2/src/netznoe_smartmeter_portal_api/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,26 +2,25 @@
 from typing import Dict, Union
 
 from pendulum import Date, DateTime
 
 
 @dataclass
 class SmartmeterResult:
-    consumption_metered: Dict[Union[Date, DateTime], float]  # Verbrauch gemessen in kWh
-    consumption_estimated: Dict[Union[Date, DateTime], float]  # Verbrauch geschaetzt in kWh
+    consumption_metered: Dict[Union[Date, DateTime], float]
+    consumption_estimated: Dict[Union[Date, DateTime], float]
     grid_usage_leftover: Dict[Union[Date, DateTime], float]
     self_coverage: Dict[Union[Date, DateTime], float]
     self_coverage_renewable_energy: Dict[Union[Date, DateTime], float]
     joint_tenancy_proportion: Dict[Union[Date, DateTime], float]
-    peak_demands_metered: Dict[Union[Date, DateTime], float]  # Leistung gemessen in kW
-    peak_demands_estimated: Dict[Union[Date, DateTime], float]  # Leistung geschaetzt in kW
+    peak_demands_metered: Dict[Union[Date, DateTime], float]
+    peak_demands_estimated: Dict[Union[Date, DateTime], float]
 
 
 @dataclass
 class SmartmeterResultYearly:
-    consumption: Dict[Union[Date, DateTime], float]  # Verbrauch in kWh
+    consumption: Dict[Union[Date, DateTime], float]
     grid_usage_leftover: Dict[Union[Date, DateTime], float]
     self_coverage: Dict[Union[Date, DateTime], float]
     self_coverage_renewable_energy: Dict[Union[Date, DateTime], float]
     joint_tenancy_proportion: Dict[Union[Date, DateTime], float]
-    peak_demands: Dict[Union[Date, DateTime], float]  # Leistung in kW
-    # is_mixed -> don't know that this does (true or false)
+    peak_demands: Dict[Union[Date, DateTime], float]
```

### Comparing `netznoe-smartmeter-portal-api-1.0.1/src/netznoe_smartmeter_portal_api.egg-info/PKG-INFO` & `netznoe-smartmeter-portal-api-1.0.2/src/netznoe_smartmeter_portal_api.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netznoe-smartmeter-portal-api
-Version: 1.0.1
+Version: 1.0.2
 Summary: An unofficial python implementation of the NetzNÖ Smartmeter Portal API
 Home-page: https://github.com/schue30/NetzNoe-SmartmeterPortal-Api
 Author: Mathias Schuepany
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -117,7 +117,12 @@
 | values                           | consumption                    | kWh  |
 | gridUsageLeftoverValues          | grid_usage_leftover            | kWh  |
 | selfCoverageValues               | self_coverage                  | kWh  |
 | selfCoverageRenewableEnergyValue | self_coverage_renewable_energy | kWh  |
 | jointTenancyProportionValues     | joint_tenancy_proportion       | kWh  |
 | peakDemands                      | peak_demands                   | kW   |
 | is_mixed                         | *< ignored >*                  |      |
+
+## Legal
+
+Disclaimer: This is not affiliated, endorsed or certified by Netz NÖ. This is an independent and unofficial API.
+Provided as is. Use at your own risk.
```

