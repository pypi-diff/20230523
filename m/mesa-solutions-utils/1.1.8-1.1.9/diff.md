# Comparing `tmp/mesa-solutions-utils-1.1.8.tar.gz` & `tmp/mesa-solutions-utils-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mesa-solutions-utils-1.1.8.tar", last modified: Thu Apr  7 21:55:34 2022, max compression
+gzip compressed data, was "dist/mesa-solutions-utils-1.1.9.tar", last modified: Wed May 11 19:14:17 2022, max compression
```

## Comparing `mesa-solutions-utils-1.1.8.tar` & `mesa-solutions-utils-1.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-07 21:55:34.000000 mesa-solutions-utils-1.1.8/
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-07 21:55:34.000000 mesa-solutions-utils-1.1.8/MesaSoapManager/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       57 2021-10-12 20:01:41.000000 mesa-solutions-utils-1.1.8/MesaSoapManager/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13494 2022-04-07 21:55:26.000000 mesa-solutions-utils-1.1.8/MesaSoapManager/nav_soap_client.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-07 21:55:34.000000 mesa-solutions-utils-1.1.8/ODCHelperFunctions/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2021-10-12 20:01:41.000000 mesa-solutions-utils-1.1.8/ODCHelperFunctions/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2350 2021-10-12 20:01:41.000000 mesa-solutions-utils-1.1.8/ODCHelperFunctions/helpers.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      422 2022-04-07 21:55:34.000000 mesa-solutions-utils-1.1.8/PKG-INFO
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-07 21:55:34.000000 mesa-solutions-utils-1.1.8/PaligoClient/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       51 2021-10-12 20:01:41.000000 mesa-solutions-utils-1.1.8/PaligoClient/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2639 2021-10-22 19:25:06.000000 mesa-solutions-utils-1.1.8/PaligoClient/paligoclient.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-04-07 21:55:34.000000 mesa-solutions-utils-1.1.8/mesa_solutions_utils.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      422 2022-04-07 21:55:33.000000 mesa-solutions-utils-1.1.8/mesa_solutions_utils.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      405 2022-04-07 21:55:33.000000 mesa-solutions-utils-1.1.8/mesa_solutions_utils.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2022-04-07 21:55:33.000000 mesa-solutions-utils-1.1.8/mesa_solutions_utils.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       26 2022-04-07 21:55:33.000000 mesa-solutions-utils-1.1.8/mesa_solutions_utils.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       48 2022-04-07 21:55:33.000000 mesa-solutions-utils-1.1.8/mesa_solutions_utils.egg-info/top_level.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2022-04-07 21:55:34.000000 mesa-solutions-utils-1.1.8/setup.cfg
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      631 2022-04-07 21:55:26.000000 mesa-solutions-utils-1.1.8/setup.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-05-11 19:14:17.000000 mesa-solutions-utils-1.1.9/
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-05-11 19:14:17.000000 mesa-solutions-utils-1.1.9/MesaSoapManager/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       57 2021-10-12 20:01:41.000000 mesa-solutions-utils-1.1.9/MesaSoapManager/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14787 2022-05-11 19:14:08.000000 mesa-solutions-utils-1.1.9/MesaSoapManager/nav_soap_client.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-05-11 19:14:17.000000 mesa-solutions-utils-1.1.9/ODCHelperFunctions/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2021-10-12 20:01:41.000000 mesa-solutions-utils-1.1.9/ODCHelperFunctions/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2350 2021-10-12 20:01:41.000000 mesa-solutions-utils-1.1.9/ODCHelperFunctions/helpers.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      422 2022-05-11 19:14:17.000000 mesa-solutions-utils-1.1.9/PKG-INFO
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-05-11 19:14:17.000000 mesa-solutions-utils-1.1.9/PaligoClient/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       51 2021-10-12 20:01:41.000000 mesa-solutions-utils-1.1.9/PaligoClient/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2639 2021-10-22 19:25:06.000000 mesa-solutions-utils-1.1.9/PaligoClient/paligoclient.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-05-11 19:14:17.000000 mesa-solutions-utils-1.1.9/mesa_solutions_utils.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      422 2022-05-11 19:14:16.000000 mesa-solutions-utils-1.1.9/mesa_solutions_utils.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      405 2022-05-11 19:14:16.000000 mesa-solutions-utils-1.1.9/mesa_solutions_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2022-05-11 19:14:16.000000 mesa-solutions-utils-1.1.9/mesa_solutions_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       26 2022-05-11 19:14:16.000000 mesa-solutions-utils-1.1.9/mesa_solutions_utils.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       48 2022-05-11 19:14:16.000000 mesa-solutions-utils-1.1.9/mesa_solutions_utils.egg-info/top_level.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2022-05-11 19:14:17.000000 mesa-solutions-utils-1.1.9/setup.cfg
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      631 2022-05-11 19:14:08.000000 mesa-solutions-utils-1.1.9/setup.py
```

### Comparing `mesa-solutions-utils-1.1.8/MesaSoapManager/nav_soap_client.py` & `mesa-solutions-utils-1.1.9/MesaSoapManager/nav_soap_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -279,56 +279,85 @@
                 custRespGroup=cust_resp_grp_id,
                 siteType=site_type
         )
 
         serialized_response = serialize_object(soap_response)
         return serialized_response
 
-    def deploy_unit(self, cust_no, site_code, rental_order, unit_id, move_date, billing_start, engine_hours):
+    def deploy_unit(self, cust_no, site_code, rental_order, unit_id, deploy_date, billing_start, engine_hours, billing_size):
         """
         Use this when a unit is deployed to a site, to set the unit on the rental order.
+        rental_order, unit_id, deploy_date, and billing_start require values, all else should be empty strings.
         """
         session = Session()
         session.auth = HTTPBasicAuth(self.nav_user, self.nav_password)
 
         soap_service_url = self.nav_soap_service + \
             self.nav_company + "/Codeunit/UnitMove"
         client = Client(soap_service_url, transport=Transport(
             session=session, cache=SqliteCache()))
 
         soap_response = client.service.DeployEquip(
             custNo = cust_no,
             siteCode = site_code,
             rentalOrderNo = rental_order,
             equipNo = unit_id,
-            deployDate = move_date,
+            deployDate = deploy_date,
             startDate = billing_start,
             engineHours = engine_hours,
+            billingCode = billing_size
         )
 
         serialized_response = serialize_object(soap_response)
         return serialized_response
 
-    def retrieve_unit(self, cust_no, site_code, rental_order, unit_id, move_date, billing_start, engine_hours):
+    def retrieve_unit(self, cust_no, site_code, rental_order, unit_id, retrieval_date, billing_end, engine_hours):
         """
         Use this when a unit is retrieved from a site, to remove the unit from the rental order.
+        rental_order, unit_id, retrieval_date, and billing_end require values, all else should be empty strings.
         """
         session = Session()
         session.auth = HTTPBasicAuth(self.nav_user, self.nav_password)
 
         soap_service_url = self.nav_soap_service + \
             self.nav_company + "/Codeunit/UnitMove"
         client = Client(soap_service_url, transport=Transport(
             session=session, cache=SqliteCache()))
 
         soap_response = client.service.ReturnEquip(
             custNo = cust_no,
             siteCode = site_code,
             rentalOrderNo = rental_order,
             equipNo = unit_id,
-            returnDate = move_date,
-            endDate = billing_start,
+            returnDate = retrieval_date,
+            endDate = billing_end,
             engineHours = engine_hours,
         )
 
         serialized_response = serialize_object(soap_response)
+        return serialized_response
+
+    def swap(self, cust_no, site_code, rental_order, retrieved_unit_id, deployed_unit_id, swap_date, return_field_office, size_swap, billing_size):
+        """
+        Use this when units are swapped.
+        """
+        session = Session()
+        session.auth = HTTPBasicAuth(self.nav_user, self.nav_password)
+
+        soap_service_url = self.nav_soap_service + \
+            self.nav_company + "/Codeunit/UnitMove"
+        client = Client(soap_service_url, transport=Transport(
+            session=session, cache=SqliteCache()))
+
+        soap_response = client.service.SwapEquip(
+            custNo = cust_no,
+            siteCode = site_code,
+            rentalOrderNo = rental_order,
+            oldEquipNo = retrieved_unit_id,
+            newEquipNo = deployed_unit_id,
+            swapDate = swap_date,
+            returnLocation = return_field_office,
+            isSiteSwap = size_swap,
+        )
+
+        serialized_response = serialize_object(soap_response)
         return serialized_response
```

### Comparing `mesa-solutions-utils-1.1.8/ODCHelperFunctions/helpers.py` & `mesa-solutions-utils-1.1.9/ODCHelperFunctions/helpers.py`

 * *Files identical despite different names*

### Comparing `mesa-solutions-utils-1.1.8/PaligoClient/paligoclient.py` & `mesa-solutions-utils-1.1.9/PaligoClient/paligoclient.py`

 * *Files identical despite different names*

### Comparing `mesa-solutions-utils-1.1.8/setup.py` & `mesa-solutions-utils-1.1.9/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from distutils.core import setup
 import setuptools
 
 setup(
     name='mesa-solutions-utils',
     packages=['MesaSoapManager', 'ODCHelperFunctions', 'PaligoClient'],
-    version='1.1.8',
+    version='1.1.9',
     license='MIT',
     description='Various utilities functions and classes',
     author='Mesa Natural Gas Solutions, LLC',
     author_email='support@mesangs.com',
     url='https://dev.azure.com/mesa-ngs/_git/mesa-solutions-utils',
     download_url='https://dev.azure.com/mesa-ngs/_git/mesa-solutions-utils',
     keywords=['Microsoft Dynamics NAV', 'Paligo' 'SOAP'],
```

