# Comparing `tmp/mypy-boto3-fms-1.26.22.tar.gz` & `tmp/mypy-boto3-fms-1.26.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-fms-1.26.22.tar", last modified: Fri Dec  2 20:32:44 2022, max compression
+gzip compressed data, was "mypy-boto3-fms-1.26.5.tar", last modified: Tue Nov  8 20:33:28 2022, max compression
```

## Comparing `mypy-boto3-fms-1.26.22.tar` & `mypy-boto3-fms-1.26.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 20:32:44.387240 mypy-boto3-fms-1.26.22/
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2022-12-02 20:32:12.000000 mypy-boto3-fms-1.26.22/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    19590 2022-12-02 20:32:44.387240 mypy-boto3-fms-1.26.22/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    18169 2022-12-02 20:32:12.000000 mypy-boto3-fms-1.26.22/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 20:32:44.387240 mypy-boto3-fms-1.26.22/mypy_boto3_fms/
--rw-r--r--   0 runner    (1001) docker     (122)     1746 2022-12-02 20:32:12.000000 mypy-boto3-fms-1.26.22/mypy_boto3_fms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1745 2022-12-02 20:32:12.000000 mypy-boto3-fms-1.26.22/mypy_boto3_fms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      892 2022-12-02 20:32:12.000000 mypy-boto3-fms-1.26.22/mypy_boto3_fms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)    27472 2022-12-02 20:32:12.000000 mypy-boto3-fms-1.26.22/mypy_boto3_fms/client.py
--rw-r--r--   0 runner    (1001) docker     (122)    27421 2022-12-02 20:32:12.000000 mypy-boto3-fms-1.26.22/mypy_boto3_fms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (122)    11779 2022-12-02 20:32:12.000000 mypy-boto3-fms-1.26.22/mypy_boto3_fms/literals.py
--rw-r--r--   0 runner    (1001) docker     (122)    11777 2022-12-02 20:32:12.000000 mypy-boto3-fms-1.26.22/mypy_boto3_fms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     7342 2022-12-02 20:32:12.000000 mypy-boto3-fms-1.26.22/mypy_boto3_fms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (122)     7334 2022-12-02 20:32:12.000000 mypy-boto3-fms-1.26.22/mypy_boto3_fms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 20:32:12.000000 mypy-boto3-fms-1.26.22/mypy_boto3_fms/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)    54486 2022-12-02 20:32:13.000000 mypy-boto3-fms-1.26.22/mypy_boto3_fms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (122)    54421 2022-12-02 20:32:12.000000 mypy-boto3-fms-1.26.22/mypy_boto3_fms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (122)       61 2022-12-02 20:32:12.000000 mypy-boto3-fms-1.26.22/mypy_boto3_fms/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 20:32:44.387240 mypy-boto3-fms-1.26.22/mypy_boto3_fms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    19590 2022-12-02 20:32:44.000000 mypy-boto3-fms-1.26.22/mypy_boto3_fms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      604 2022-12-02 20:32:44.000000 mypy-boto3-fms-1.26.22/mypy_boto3_fms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-02 20:32:44.000000 mypy-boto3-fms-1.26.22/mypy_boto3_fms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-02 20:32:44.000000 mypy-boto3-fms-1.26.22/mypy_boto3_fms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       25 2022-12-02 20:32:44.000000 mypy-boto3-fms-1.26.22/mypy_boto3_fms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2022-12-02 20:32:44.000000 mypy-boto3-fms-1.26.22/mypy_boto3_fms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-02 20:32:44.387240 mypy-boto3-fms-1.26.22/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1925 2022-12-02 20:32:11.000000 mypy-boto3-fms-1.26.22/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 20:33:28.885201 mypy-boto3-fms-1.26.5/
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-08 20:33:02.000000 mypy-boto3-fms-1.26.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    19587 2022-11-08 20:33:28.877201 mypy-boto3-fms-1.26.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    18168 2022-11-08 20:33:02.000000 mypy-boto3-fms-1.26.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 20:33:28.873201 mypy-boto3-fms-1.26.5/mypy_boto3_fms/
+-rw-r--r--   0 runner    (1001) docker     (121)     1746 2022-11-08 20:33:02.000000 mypy-boto3-fms-1.26.5/mypy_boto3_fms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1745 2022-11-08 20:33:02.000000 mypy-boto3-fms-1.26.5/mypy_boto3_fms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      889 2022-11-08 20:33:02.000000 mypy-boto3-fms-1.26.5/mypy_boto3_fms/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27532 2022-11-08 20:33:02.000000 mypy-boto3-fms-1.26.5/mypy_boto3_fms/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27481 2022-11-08 20:33:02.000000 mypy-boto3-fms-1.26.5/mypy_boto3_fms/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)    11468 2022-11-08 20:33:03.000000 mypy-boto3-fms-1.26.5/mypy_boto3_fms/literals.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11466 2022-11-08 20:33:02.000000 mypy-boto3-fms-1.26.5/mypy_boto3_fms/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     7438 2022-11-08 20:33:02.000000 mypy-boto3-fms-1.26.5/mypy_boto3_fms/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7429 2022-11-08 20:33:02.000000 mypy-boto3-fms-1.26.5/mypy_boto3_fms/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-08 20:33:02.000000 mypy-boto3-fms-1.26.5/mypy_boto3_fms/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)    54548 2022-11-08 20:33:03.000000 mypy-boto3-fms-1.26.5/mypy_boto3_fms/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    54483 2022-11-08 20:33:03.000000 mypy-boto3-fms-1.26.5/mypy_boto3_fms/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-08 20:33:02.000000 mypy-boto3-fms-1.26.5/mypy_boto3_fms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 20:33:28.877201 mypy-boto3-fms-1.26.5/mypy_boto3_fms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    19587 2022-11-08 20:33:28.000000 mypy-boto3-fms-1.26.5/mypy_boto3_fms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      604 2022-11-08 20:33:28.000000 mypy-boto3-fms-1.26.5/mypy_boto3_fms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-08 20:33:28.000000 mypy-boto3-fms-1.26.5/mypy_boto3_fms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-08 20:33:28.000000 mypy-boto3-fms-1.26.5/mypy_boto3_fms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-08 20:33:28.000000 mypy-boto3-fms-1.26.5/mypy_boto3_fms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-11-08 20:33:28.000000 mypy-boto3-fms-1.26.5/mypy_boto3_fms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-08 20:33:28.885201 mypy-boto3-fms-1.26.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1923 2022-11-08 20:33:02.000000 mypy-boto3-fms-1.26.5/setup.py
```

### Comparing `mypy-boto3-fms-1.26.22/LICENSE` & `mypy-boto3-fms-1.26.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fms-1.26.22/PKG-INFO` & `mypy-boto3-fms-1.26.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-fms
-Version: 1.26.22
-Summary: Type annotations for boto3.FMS 1.26.22 service generated with mypy-boto3-builder 7.11.11
+Version: 1.26.5
+Summary: Type annotations for boto3.FMS 1.26.5 service generated with mypy-boto3-builder 7.11.10
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -37,24 +37,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-fms.svg?color=blue)](https://pypi.org/project/mypy-boto3-fms)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-fms?color=blue)](https://pypistats.org/packages/mypy-boto3-fms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FMS 1.26.22](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
+[boto3.FMS 1.26.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-fms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-fms-1.26.22/README.md` & `mypy-boto3-fms-1.26.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-fms.svg?color=blue)](https://pypi.org/project/mypy-boto3-fms)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-fms?color=blue)](https://pypistats.org/packages/mypy-boto3-fms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FMS 1.26.22](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
+[boto3.FMS 1.26.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-fms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-fms-1.26.22/mypy_boto3_fms/__init__.py` & `mypy-boto3-fms-1.26.5/mypy_boto3_fms/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fms-1.26.22/mypy_boto3_fms/__init__.pyi` & `mypy-boto3-fms-1.26.5/mypy_boto3_fms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fms-1.26.22/mypy_boto3_fms/__main__.py` & `mypy-boto3-fms-1.26.5/mypy_boto3_fms/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.FMS 1.26.22\nVersion:         1.26.22\nBuilder version:"
-        " 7.11.11\nDocs:           "
+        "Type annotations for boto3.FMS 1.26.5\nVersion:         1.26.5\nBuilder version:"
+        " 7.11.10\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.22")
+    print("1.26.5")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-fms-1.26.22/mypy_boto3_fms/client.py` & `mypy-boto3-fms-1.26.5/mypy_boto3_fms/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
-from .literals import ThirdPartyFirewallType
 from .paginator import (
     ListAppsListsPaginator,
     ListComplianceStatusPaginator,
     ListMemberAccountsPaginator,
     ListPoliciesPaginator,
     ListProtocolsListsPaginator,
     ListThirdPartyFirewallFirewallPoliciesPaginator,
@@ -114,15 +113,15 @@
         Sets the Firewall Manager administrator account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.associate_admin_account)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#associate_admin_account)
         """
 
     def associate_third_party_firewall(
-        self, *, ThirdPartyFirewall: ThirdPartyFirewallType
+        self, *, ThirdPartyFirewall: Literal["PALO_ALTO_NETWORKS_CLOUD_NGFW"]
     ) -> AssociateThirdPartyFirewallResponseTypeDef:
         """
         Sets the Firewall Manager policy administrator as a tenant administrator of a
         third-party firewall service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.associate_third_party_firewall)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#associate_third_party_firewall)
@@ -198,15 +197,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.delete_protocols_list)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#delete_protocols_list)
         """
 
     def delete_resource_set(self, *, Identifier: str) -> EmptyResponseMetadataTypeDef:
         """
-        Deletes the specified  ResourceSet.
+        Deletes the specified  ResourceSet .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.delete_resource_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#delete_resource_set)
         """
 
     def disassociate_admin_account(self) -> EmptyResponseMetadataTypeDef:
         """
@@ -214,15 +213,15 @@
         administrator account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.disassociate_admin_account)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#disassociate_admin_account)
         """
 
     def disassociate_third_party_firewall(
-        self, *, ThirdPartyFirewall: ThirdPartyFirewallType
+        self, *, ThirdPartyFirewall: Literal["PALO_ALTO_NETWORKS_CLOUD_NGFW"]
     ) -> DisassociateThirdPartyFirewallResponseTypeDef:
         """
         Disassociates a Firewall Manager policy administrator from a third-party
         firewall tenant.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.disassociate_third_party_firewall)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#disassociate_third_party_firewall)
@@ -319,15 +318,15 @@
         Gets information about a specific resource set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.get_resource_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#get_resource_set)
         """
 
     def get_third_party_firewall_association_status(
-        self, *, ThirdPartyFirewall: ThirdPartyFirewallType
+        self, *, ThirdPartyFirewall: Literal["PALO_ALTO_NETWORKS_CLOUD_NGFW"]
     ) -> GetThirdPartyFirewallAssociationStatusResponseTypeDef:
         """
         The onboarding status of a Firewall Manager admin account to third-party
         firewall vendor tenant.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.get_third_party_firewall_association_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#get_third_party_firewall_association_status)
@@ -436,15 +435,19 @@
         Retrieves the list of tags for the specified Amazon Web Services resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#list_tags_for_resource)
         """
 
     def list_third_party_firewall_firewall_policies(
-        self, *, ThirdPartyFirewall: ThirdPartyFirewallType, MaxResults: int, NextToken: str = ...
+        self,
+        *,
+        ThirdPartyFirewall: Literal["PALO_ALTO_NETWORKS_CLOUD_NGFW"],
+        MaxResults: int,
+        NextToken: str = ...
     ) -> ListThirdPartyFirewallFirewallPoliciesResponseTypeDef:
         """
         Retrieves a list of all of the third-party firewall policies that are associated
         with the third-party firewall administrator's account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.list_third_party_firewall_firewall_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#list_third_party_firewall_firewall_policies)
```

### Comparing `mypy-boto3-fms-1.26.22/mypy_boto3_fms/client.pyi` & `mypy-boto3-fms-1.26.5/mypy_boto3_fms/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
-from .literals import ThirdPartyFirewallType
 from .paginator import (
     ListAppsListsPaginator,
     ListComplianceStatusPaginator,
     ListMemberAccountsPaginator,
     ListPoliciesPaginator,
     ListProtocolsListsPaginator,
     ListThirdPartyFirewallFirewallPoliciesPaginator,
@@ -108,15 +107,15 @@
         """
         Sets the Firewall Manager administrator account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.associate_admin_account)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#associate_admin_account)
         """
     def associate_third_party_firewall(
-        self, *, ThirdPartyFirewall: ThirdPartyFirewallType
+        self, *, ThirdPartyFirewall: Literal["PALO_ALTO_NETWORKS_CLOUD_NGFW"]
     ) -> AssociateThirdPartyFirewallResponseTypeDef:
         """
         Sets the Firewall Manager policy administrator as a tenant administrator of a
         third-party firewall service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.associate_third_party_firewall)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#associate_third_party_firewall)
@@ -183,29 +182,29 @@
         Permanently deletes an Firewall Manager protocols list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.delete_protocols_list)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#delete_protocols_list)
         """
     def delete_resource_set(self, *, Identifier: str) -> EmptyResponseMetadataTypeDef:
         """
-        Deletes the specified  ResourceSet.
+        Deletes the specified  ResourceSet .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.delete_resource_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#delete_resource_set)
         """
     def disassociate_admin_account(self) -> EmptyResponseMetadataTypeDef:
         """
         Disassociates the account that has been set as the Firewall Manager
         administrator account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.disassociate_admin_account)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#disassociate_admin_account)
         """
     def disassociate_third_party_firewall(
-        self, *, ThirdPartyFirewall: ThirdPartyFirewallType
+        self, *, ThirdPartyFirewall: Literal["PALO_ALTO_NETWORKS_CLOUD_NGFW"]
     ) -> DisassociateThirdPartyFirewallResponseTypeDef:
         """
         Disassociates a Firewall Manager policy administrator from a third-party
         firewall tenant.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.disassociate_third_party_firewall)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#disassociate_third_party_firewall)
@@ -292,15 +291,15 @@
         """
         Gets information about a specific resource set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.get_resource_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#get_resource_set)
         """
     def get_third_party_firewall_association_status(
-        self, *, ThirdPartyFirewall: ThirdPartyFirewallType
+        self, *, ThirdPartyFirewall: Literal["PALO_ALTO_NETWORKS_CLOUD_NGFW"]
     ) -> GetThirdPartyFirewallAssociationStatusResponseTypeDef:
         """
         The onboarding status of a Firewall Manager admin account to third-party
         firewall vendor tenant.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.get_third_party_firewall_association_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#get_third_party_firewall_association_status)
@@ -398,15 +397,19 @@
         """
         Retrieves the list of tags for the specified Amazon Web Services resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#list_tags_for_resource)
         """
     def list_third_party_firewall_firewall_policies(
-        self, *, ThirdPartyFirewall: ThirdPartyFirewallType, MaxResults: int, NextToken: str = ...
+        self,
+        *,
+        ThirdPartyFirewall: Literal["PALO_ALTO_NETWORKS_CLOUD_NGFW"],
+        MaxResults: int,
+        NextToken: str = ...
     ) -> ListThirdPartyFirewallFirewallPoliciesResponseTypeDef:
         """
         Retrieves a list of all of the third-party firewall policies that are associated
         with the third-party firewall administrator's account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.list_third_party_firewall_firewall_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/client/#list_third_party_firewall_firewall_policies)
```

### Comparing `mypy-boto3-fms-1.26.22/mypy_boto3_fms/literals.py` & `mypy-boto3-fms-1.26.5/mypy_boto3_fms/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     "TRANSIT_GATEWAY",
     "VPC_ENDPOINT",
     "VPC_PEERING_CONNECTION",
 ]
 ThirdPartyFirewallAssociationStatusType = Literal[
     "NOT_EXIST", "OFFBOARDING", "OFFBOARD_COMPLETE", "ONBOARDING", "ONBOARD_COMPLETE"
 ]
-ThirdPartyFirewallType = Literal["FORTIGATE_CLOUD_NATIVE_FIREWALL", "PALO_ALTO_NETWORKS_CLOUD_NGFW"]
+ThirdPartyFirewallType = Literal["PALO_ALTO_NETWORKS_CLOUD_NGFW"]
 ViolationReasonType = Literal[
     "BLACK_HOLE_ROUTE_DETECTED",
     "BLACK_HOLE_ROUTE_DETECTED_IN_FIREWALL_SUBNET",
     "FIREWALL_SUBNET_IS_OUT_OF_SCOPE",
     "FIREWALL_SUBNET_MISSING_EXPECTED_ROUTE",
     "FIREWALL_SUBNET_MISSING_VPCE_ENDPOINT",
     "FMS_CREATED_SECURITY_GROUP_EDITED",
@@ -155,15 +155,14 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
-    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -173,29 +172,27 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
-    "chime-sdk-voice",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
     "cloudwatch",
     "codeartifact",
     "codebuild",
-    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -224,15 +221,14 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
-    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -280,15 +276,14 @@
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -354,32 +349,28 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
-    "oam",
-    "omics",
     "opensearch",
-    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
-    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -407,43 +398,38 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
-    "sagemaker-geospatial",
     "sagemaker-runtime",
     "savingsplans",
-    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
-    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
-    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
-    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
```

### Comparing `mypy-boto3-fms-1.26.22/mypy_boto3_fms/literals.pyi` & `mypy-boto3-fms-1.26.5/mypy_boto3_fms/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     "TRANSIT_GATEWAY",
     "VPC_ENDPOINT",
     "VPC_PEERING_CONNECTION",
 ]
 ThirdPartyFirewallAssociationStatusType = Literal[
     "NOT_EXIST", "OFFBOARDING", "OFFBOARD_COMPLETE", "ONBOARDING", "ONBOARD_COMPLETE"
 ]
-ThirdPartyFirewallType = Literal["FORTIGATE_CLOUD_NATIVE_FIREWALL", "PALO_ALTO_NETWORKS_CLOUD_NGFW"]
+ThirdPartyFirewallType = Literal["PALO_ALTO_NETWORKS_CLOUD_NGFW"]
 ViolationReasonType = Literal[
     "BLACK_HOLE_ROUTE_DETECTED",
     "BLACK_HOLE_ROUTE_DETECTED_IN_FIREWALL_SUBNET",
     "FIREWALL_SUBNET_IS_OUT_OF_SCOPE",
     "FIREWALL_SUBNET_MISSING_EXPECTED_ROUTE",
     "FIREWALL_SUBNET_MISSING_VPCE_ENDPOINT",
     "FMS_CREATED_SECURITY_GROUP_EDITED",
@@ -153,15 +153,14 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
-    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -171,29 +170,27 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
-    "chime-sdk-voice",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
     "cloudwatch",
     "codeartifact",
     "codebuild",
-    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -222,15 +219,14 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
-    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -278,15 +274,14 @@
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -352,32 +347,28 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
-    "oam",
-    "omics",
     "opensearch",
-    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
-    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -405,43 +396,38 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
-    "sagemaker-geospatial",
     "sagemaker-runtime",
     "savingsplans",
-    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
-    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
-    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
-    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
```

### Comparing `mypy-boto3-fms-1.26.22/mypy_boto3_fms/paginator.py` & `mypy-boto3-fms-1.26.5/mypy_boto3_fms/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,29 +25,35 @@
     list_compliance_status_paginator: ListComplianceStatusPaginator = client.get_paginator("list_compliance_status")
     list_member_accounts_paginator: ListMemberAccountsPaginator = client.get_paginator("list_member_accounts")
     list_policies_paginator: ListPoliciesPaginator = client.get_paginator("list_policies")
     list_protocols_lists_paginator: ListProtocolsListsPaginator = client.get_paginator("list_protocols_lists")
     list_third_party_firewall_firewall_policies_paginator: ListThirdPartyFirewallFirewallPoliciesPaginator = client.get_paginator("list_third_party_firewall_firewall_policies")
     ```
 """
+import sys
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
-from .literals import ThirdPartyFirewallType
 from .type_defs import (
     ListAppsListsResponseTypeDef,
     ListComplianceStatusResponseTypeDef,
     ListMemberAccountsResponseTypeDef,
     ListPoliciesResponseTypeDef,
     ListProtocolsListsResponseTypeDef,
     ListThirdPartyFirewallFirewallPoliciesResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
+if sys.version_info >= (3, 9):
+    from typing import Literal
+else:
+    from typing_extensions import Literal
+
+
 __all__ = (
     "ListAppsListsPaginator",
     "ListComplianceStatusPaginator",
     "ListMemberAccountsPaginator",
     "ListPoliciesPaginator",
     "ListProtocolsListsPaginator",
     "ListThirdPartyFirewallFirewallPoliciesPaginator",
@@ -144,14 +150,14 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListThirdPartyFirewallFirewallPolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listthirdpartyfirewallfirewallpoliciespaginator)
     """
 
     def paginate(
         self,
         *,
-        ThirdPartyFirewall: ThirdPartyFirewallType,
+        ThirdPartyFirewall: Literal["PALO_ALTO_NETWORKS_CLOUD_NGFW"],
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListThirdPartyFirewallFirewallPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListThirdPartyFirewallFirewallPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listthirdpartyfirewallfirewallpoliciespaginator)
         """
```

### Comparing `mypy-boto3-fms-1.26.22/mypy_boto3_fms/paginator.pyi` & `mypy-boto3-fms-1.26.5/mypy_boto3_fms/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -25,29 +25,34 @@
     list_compliance_status_paginator: ListComplianceStatusPaginator = client.get_paginator("list_compliance_status")
     list_member_accounts_paginator: ListMemberAccountsPaginator = client.get_paginator("list_member_accounts")
     list_policies_paginator: ListPoliciesPaginator = client.get_paginator("list_policies")
     list_protocols_lists_paginator: ListProtocolsListsPaginator = client.get_paginator("list_protocols_lists")
     list_third_party_firewall_firewall_policies_paginator: ListThirdPartyFirewallFirewallPoliciesPaginator = client.get_paginator("list_third_party_firewall_firewall_policies")
     ```
 """
+import sys
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
-from .literals import ThirdPartyFirewallType
 from .type_defs import (
     ListAppsListsResponseTypeDef,
     ListComplianceStatusResponseTypeDef,
     ListMemberAccountsResponseTypeDef,
     ListPoliciesResponseTypeDef,
     ListProtocolsListsResponseTypeDef,
     ListThirdPartyFirewallFirewallPoliciesResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
+if sys.version_info >= (3, 9):
+    from typing import Literal
+else:
+    from typing_extensions import Literal
+
 __all__ = (
     "ListAppsListsPaginator",
     "ListComplianceStatusPaginator",
     "ListMemberAccountsPaginator",
     "ListPoliciesPaginator",
     "ListProtocolsListsPaginator",
     "ListThirdPartyFirewallFirewallPoliciesPaginator",
@@ -136,14 +141,14 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListThirdPartyFirewallFirewallPolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listthirdpartyfirewallfirewallpoliciespaginator)
     """
 
     def paginate(
         self,
         *,
-        ThirdPartyFirewall: ThirdPartyFirewallType,
+        ThirdPartyFirewall: Literal["PALO_ALTO_NETWORKS_CLOUD_NGFW"],
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListThirdPartyFirewallFirewallPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListThirdPartyFirewallFirewallPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listthirdpartyfirewallfirewallpoliciespaginator)
         """
```

### Comparing `mypy-boto3-fms-1.26.22/mypy_boto3_fms/type_defs.py` & `mypy-boto3-fms-1.26.5/mypy_boto3_fms/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -25,28 +25,26 @@
     MarketplaceSubscriptionOnboardingStatusType,
     PolicyComplianceStatusTypeType,
     RemediationActionTypeType,
     RuleOrderType,
     SecurityServiceTypeType,
     TargetTypeType,
     ThirdPartyFirewallAssociationStatusType,
-    ThirdPartyFirewallType,
     ViolationReasonType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ActionTargetTypeDef",
     "AppTypeDef",
     "AssociateAdminAccountRequestRequestTypeDef",
     "AssociateThirdPartyFirewallRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AwsEc2NetworkInterfaceViolationTypeDef",
@@ -211,15 +209,15 @@
         "AdminAccount": str,
     },
 )
 
 AssociateThirdPartyFirewallRequestRequestTypeDef = TypedDict(
     "AssociateThirdPartyFirewallRequestRequestTypeDef",
     {
-        "ThirdPartyFirewall": ThirdPartyFirewallType,
+        "ThirdPartyFirewall": Literal["PALO_ALTO_NETWORKS_CLOUD_NGFW"],
     },
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
@@ -301,21 +299,19 @@
     "_OptionalDeletePolicyRequestRequestTypeDef",
     {
         "DeleteAllPolicyResources": bool,
     },
     total=False,
 )
 
-
 class DeletePolicyRequestRequestTypeDef(
     _RequiredDeletePolicyRequestRequestTypeDef, _OptionalDeletePolicyRequestRequestTypeDef
 ):
     pass
 
-
 DeleteProtocolsListRequestRequestTypeDef = TypedDict(
     "DeleteProtocolsListRequestRequestTypeDef",
     {
         "ListId": str,
     },
 )
 
@@ -325,15 +321,15 @@
         "Identifier": str,
     },
 )
 
 DisassociateThirdPartyFirewallRequestRequestTypeDef = TypedDict(
     "DisassociateThirdPartyFirewallRequestRequestTypeDef",
     {
-        "ThirdPartyFirewall": ThirdPartyFirewallType,
+        "ThirdPartyFirewall": Literal["PALO_ALTO_NETWORKS_CLOUD_NGFW"],
     },
 )
 
 DiscoveredResourceTypeDef = TypedDict(
     "DiscoveredResourceTypeDef",
     {
         "URI": str,
@@ -440,21 +436,19 @@
     "_OptionalGetAppsListRequestRequestTypeDef",
     {
         "DefaultList": bool,
     },
     total=False,
 )
 
-
 class GetAppsListRequestRequestTypeDef(
     _RequiredGetAppsListRequestRequestTypeDef, _OptionalGetAppsListRequestRequestTypeDef
 ):
     pass
 
-
 GetComplianceDetailRequestRequestTypeDef = TypedDict(
     "GetComplianceDetailRequestRequestTypeDef",
     {
         "PolicyId": str,
         "MemberAccount": str,
     },
 )
@@ -480,43 +474,39 @@
         "EndTime": Union[datetime, str],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class GetProtectionStatusRequestRequestTypeDef(
     _RequiredGetProtectionStatusRequestRequestTypeDef,
     _OptionalGetProtectionStatusRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetProtocolsListRequestRequestTypeDef = TypedDict(
     "_RequiredGetProtocolsListRequestRequestTypeDef",
     {
         "ListId": str,
     },
 )
 _OptionalGetProtocolsListRequestRequestTypeDef = TypedDict(
     "_OptionalGetProtocolsListRequestRequestTypeDef",
     {
         "DefaultList": bool,
     },
     total=False,
 )
 
-
 class GetProtocolsListRequestRequestTypeDef(
     _RequiredGetProtocolsListRequestRequestTypeDef, _OptionalGetProtocolsListRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredProtocolsListDataTypeDef = TypedDict(
     "_RequiredProtocolsListDataTypeDef",
     {
         "ListName": str,
         "ProtocolsList": List[str],
     },
 )
@@ -528,21 +518,19 @@
         "CreateTime": datetime,
         "LastUpdateTime": datetime,
         "PreviousProtocolsList": Dict[str, List[str]],
     },
     total=False,
 )
 
-
 class ProtocolsListDataTypeDef(
     _RequiredProtocolsListDataTypeDef, _OptionalProtocolsListDataTypeDef
 ):
     pass
 
-
 GetResourceSetRequestRequestTypeDef = TypedDict(
     "GetResourceSetRequestRequestTypeDef",
     {
         "Identifier": str,
     },
 )
 
@@ -560,23 +548,21 @@
         "Description": str,
         "UpdateToken": str,
         "LastUpdateTime": datetime,
     },
     total=False,
 )
 
-
 class ResourceSetTypeDef(_RequiredResourceSetTypeDef, _OptionalResourceSetTypeDef):
     pass
 
-
 GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef = TypedDict(
     "GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef",
     {
-        "ThirdPartyFirewall": ThirdPartyFirewallType,
+        "ThirdPartyFirewall": Literal["PALO_ALTO_NETWORKS_CLOUD_NGFW"],
     },
 )
 
 GetViolationDetailsRequestRequestTypeDef = TypedDict(
     "GetViolationDetailsRequestRequestTypeDef",
     {
         "PolicyId": str,
@@ -607,21 +593,19 @@
     {
         "DefaultLists": bool,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListAppsListsRequestRequestTypeDef(
     _RequiredListAppsListsRequestRequestTypeDef, _OptionalListAppsListsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListComplianceStatusRequestRequestTypeDef = TypedDict(
     "_RequiredListComplianceStatusRequestRequestTypeDef",
     {
         "PolicyId": str,
     },
 )
 _OptionalListComplianceStatusRequestRequestTypeDef = TypedDict(
@@ -629,22 +613,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListComplianceStatusRequestRequestTypeDef(
     _RequiredListComplianceStatusRequestRequestTypeDef,
     _OptionalListComplianceStatusRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListDiscoveredResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListDiscoveredResourcesRequestRequestTypeDef",
     {
         "MemberAccountIds": Sequence[str],
         "ResourceType": str,
     },
 )
@@ -653,22 +635,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListDiscoveredResourcesRequestRequestTypeDef(
     _RequiredListDiscoveredResourcesRequestRequestTypeDef,
     _OptionalListDiscoveredResourcesRequestRequestTypeDef,
 ):
     pass
 
-
 ListMemberAccountsRequestRequestTypeDef = TypedDict(
     "ListMemberAccountsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -708,22 +688,20 @@
     {
         "DefaultLists": bool,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListProtocolsListsRequestRequestTypeDef(
     _RequiredListProtocolsListsRequestRequestTypeDef,
     _OptionalListProtocolsListsRequestRequestTypeDef,
 ):
     pass
 
-
 ProtocolsListDataSummaryTypeDef = TypedDict(
     "ProtocolsListDataSummaryTypeDef",
     {
         "ListArn": str,
         "ListId": str,
         "ListName": str,
         "ProtocolsList": List[str],
@@ -742,41 +720,37 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListResourceSetResourcesRequestRequestTypeDef(
     _RequiredListResourceSetResourcesRequestRequestTypeDef,
     _OptionalListResourceSetResourcesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredResourceTypeDef = TypedDict(
     "_RequiredResourceTypeDef",
     {
         "URI": str,
     },
 )
 _OptionalResourceTypeDef = TypedDict(
     "_OptionalResourceTypeDef",
     {
         "AccountId": str,
     },
     total=False,
 )
 
-
 class ResourceTypeDef(_RequiredResourceTypeDef, _OptionalResourceTypeDef):
     pass
 
-
 ListResourceSetsRequestRequestTypeDef = TypedDict(
     "ListResourceSetsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -807,34 +781,32 @@
         "Value": str,
     },
 )
 
 _RequiredListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef",
     {
-        "ThirdPartyFirewall": ThirdPartyFirewallType,
+        "ThirdPartyFirewall": Literal["PALO_ALTO_NETWORKS_CLOUD_NGFW"],
         "MaxResults": int,
     },
 )
 _OptionalListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef = TypedDict(
     "_OptionalListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef(
     _RequiredListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef,
     _OptionalListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef,
 ):
     pass
 
-
 ThirdPartyFirewallFirewallPolicyTypeDef = TypedDict(
     "ThirdPartyFirewallFirewallPolicyTypeDef",
     {
         "FirewallPolicyId": str,
         "FirewallPolicyName": str,
     },
     total=False,
@@ -937,19 +909,17 @@
     "_OptionalResourceTagTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-
 class ResourceTagTypeDef(_RequiredResourceTagTypeDef, _OptionalResourceTagTypeDef):
     pass
 
-
 PutNotificationChannelRequestRequestTypeDef = TypedDict(
     "PutNotificationChannelRequestRequestTypeDef",
     {
         "SnsTopicArn": str,
         "SnsRoleName": str,
     },
 )
@@ -1021,21 +991,19 @@
         "Description": str,
         "SubnetId": ActionTargetTypeDef,
         "GatewayId": ActionTargetTypeDef,
     },
     total=False,
 )
 
-
 class EC2AssociateRouteTableActionTypeDef(
     _RequiredEC2AssociateRouteTableActionTypeDef, _OptionalEC2AssociateRouteTableActionTypeDef
 ):
     pass
 
-
 _RequiredEC2CopyRouteTableActionTypeDef = TypedDict(
     "_RequiredEC2CopyRouteTableActionTypeDef",
     {
         "VpcId": ActionTargetTypeDef,
         "RouteTableId": ActionTargetTypeDef,
     },
 )
@@ -1043,21 +1011,19 @@
     "_OptionalEC2CopyRouteTableActionTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class EC2CopyRouteTableActionTypeDef(
     _RequiredEC2CopyRouteTableActionTypeDef, _OptionalEC2CopyRouteTableActionTypeDef
 ):
     pass
 
-
 _RequiredEC2CreateRouteActionTypeDef = TypedDict(
     "_RequiredEC2CreateRouteActionTypeDef",
     {
         "RouteTableId": ActionTargetTypeDef,
     },
 )
 _OptionalEC2CreateRouteActionTypeDef = TypedDict(
@@ -1069,42 +1035,38 @@
         "DestinationIpv6CidrBlock": str,
         "VpcEndpointId": ActionTargetTypeDef,
         "GatewayId": ActionTargetTypeDef,
     },
     total=False,
 )
 
-
 class EC2CreateRouteActionTypeDef(
     _RequiredEC2CreateRouteActionTypeDef, _OptionalEC2CreateRouteActionTypeDef
 ):
     pass
 
-
 _RequiredEC2CreateRouteTableActionTypeDef = TypedDict(
     "_RequiredEC2CreateRouteTableActionTypeDef",
     {
         "VpcId": ActionTargetTypeDef,
     },
 )
 _OptionalEC2CreateRouteTableActionTypeDef = TypedDict(
     "_OptionalEC2CreateRouteTableActionTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class EC2CreateRouteTableActionTypeDef(
     _RequiredEC2CreateRouteTableActionTypeDef, _OptionalEC2CreateRouteTableActionTypeDef
 ):
     pass
 
-
 _RequiredEC2DeleteRouteActionTypeDef = TypedDict(
     "_RequiredEC2DeleteRouteActionTypeDef",
     {
         "RouteTableId": ActionTargetTypeDef,
     },
 )
 _OptionalEC2DeleteRouteActionTypeDef = TypedDict(
@@ -1114,21 +1076,19 @@
         "DestinationCidrBlock": str,
         "DestinationPrefixListId": str,
         "DestinationIpv6CidrBlock": str,
     },
     total=False,
 )
 
-
 class EC2DeleteRouteActionTypeDef(
     _RequiredEC2DeleteRouteActionTypeDef, _OptionalEC2DeleteRouteActionTypeDef
 ):
     pass
 
-
 _RequiredEC2ReplaceRouteActionTypeDef = TypedDict(
     "_RequiredEC2ReplaceRouteActionTypeDef",
     {
         "RouteTableId": ActionTargetTypeDef,
     },
 )
 _OptionalEC2ReplaceRouteActionTypeDef = TypedDict(
@@ -1139,21 +1099,19 @@
         "DestinationPrefixListId": str,
         "DestinationIpv6CidrBlock": str,
         "GatewayId": ActionTargetTypeDef,
     },
     total=False,
 )
 
-
 class EC2ReplaceRouteActionTypeDef(
     _RequiredEC2ReplaceRouteActionTypeDef, _OptionalEC2ReplaceRouteActionTypeDef
 ):
     pass
 
-
 _RequiredEC2ReplaceRouteTableAssociationActionTypeDef = TypedDict(
     "_RequiredEC2ReplaceRouteTableAssociationActionTypeDef",
     {
         "AssociationId": ActionTargetTypeDef,
         "RouteTableId": ActionTargetTypeDef,
     },
 )
@@ -1161,22 +1119,20 @@
     "_OptionalEC2ReplaceRouteTableAssociationActionTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class EC2ReplaceRouteTableAssociationActionTypeDef(
     _RequiredEC2ReplaceRouteTableAssociationActionTypeDef,
     _OptionalEC2ReplaceRouteTableAssociationActionTypeDef,
 ):
     pass
 
-
 AppsListDataSummaryTypeDef = TypedDict(
     "AppsListDataSummaryTypeDef",
     {
         "ListArn": str,
         "ListId": str,
         "ListName": str,
         "AppsList": List[AppTypeDef],
@@ -1199,19 +1155,17 @@
         "CreateTime": datetime,
         "LastUpdateTime": datetime,
         "PreviousAppsList": Dict[str, List[AppTypeDef]],
     },
     total=False,
 )
 
-
 class AppsListDataTypeDef(_RequiredAppsListDataTypeDef, _OptionalAppsListDataTypeDef):
     pass
 
-
 AssociateThirdPartyFirewallResponseTypeDef = TypedDict(
     "AssociateThirdPartyFirewallResponseTypeDef",
     {
         "ThirdPartyFirewallStatus": ThirdPartyFirewallAssociationStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1407,22 +1361,20 @@
     "_OptionalListComplianceStatusRequestListComplianceStatusPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListComplianceStatusRequestListComplianceStatusPaginateTypeDef(
     _RequiredListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
     _OptionalListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
 ):
     pass
 
-
 ListMemberAccountsRequestListMemberAccountsPaginateTypeDef = TypedDict(
     "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -1443,33 +1395,31 @@
     },
     total=False,
 )
 
 _RequiredListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef = TypedDict(
     "_RequiredListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef",
     {
-        "ThirdPartyFirewall": ThirdPartyFirewallType,
+        "ThirdPartyFirewall": Literal["PALO_ALTO_NETWORKS_CLOUD_NGFW"],
     },
 )
 _OptionalListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef = TypedDict(
     "_OptionalListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef(
     _RequiredListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
     _OptionalListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
 ):
     pass
 
-
 ListPoliciesResponseTypeDef = TypedDict(
     "ListPoliciesResponseTypeDef",
     {
         "PolicyList": List[PolicySummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1520,42 +1470,38 @@
     "_OptionalPutProtocolsListRequestRequestTypeDef",
     {
         "TagList": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class PutProtocolsListRequestRequestTypeDef(
     _RequiredPutProtocolsListRequestRequestTypeDef, _OptionalPutProtocolsListRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredPutResourceSetRequestRequestTypeDef = TypedDict(
     "_RequiredPutResourceSetRequestRequestTypeDef",
     {
         "ResourceSet": ResourceSetTypeDef,
     },
 )
 _OptionalPutResourceSetRequestRequestTypeDef = TypedDict(
     "_OptionalPutResourceSetRequestRequestTypeDef",
     {
         "TagList": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class PutResourceSetRequestRequestTypeDef(
     _RequiredPutResourceSetRequestRequestTypeDef, _OptionalPutResourceSetRequestRequestTypeDef
 ):
     pass
 
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagList": Sequence[TagTypeDef],
     },
 )
@@ -1742,21 +1688,19 @@
     "_OptionalPutAppsListRequestRequestTypeDef",
     {
         "TagList": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class PutAppsListRequestRequestTypeDef(
     _RequiredPutAppsListRequestRequestTypeDef, _OptionalPutAppsListRequestRequestTypeDef
 ):
     pass
 
-
 PutAppsListResponseTypeDef = TypedDict(
     "PutAppsListResponseTypeDef",
     {
         "AppsList": AppsListDataTypeDef,
         "AppsListArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1804,21 +1748,19 @@
     {
         "ManagedServiceData": str,
         "PolicyOption": PolicyOptionTypeDef,
     },
     total=False,
 )
 
-
 class SecurityServicePolicyDataTypeDef(
     _RequiredSecurityServicePolicyDataTypeDef, _OptionalSecurityServicePolicyDataTypeDef
 ):
     pass
 
-
 AwsVPCSecurityGroupViolationTypeDef = TypedDict(
     "AwsVPCSecurityGroupViolationTypeDef",
     {
         "ViolationTarget": str,
         "ViolationTargetDescription": str,
         "PartialMatches": List[PartialMatchTypeDef],
         "PossibleSecurityGroupRemediationActions": List[SecurityGroupRemediationActionTypeDef],
@@ -1867,19 +1809,17 @@
         "ExcludeMap": Dict[CustomerPolicyScopeIdTypeType, List[str]],
         "ResourceSetIds": List[str],
         "PolicyDescription": str,
     },
     total=False,
 )
 
-
 class PolicyTypeDef(_RequiredPolicyTypeDef, _OptionalPolicyTypeDef):
     pass
 
-
 _RequiredPossibleRemediationActionTypeDef = TypedDict(
     "_RequiredPossibleRemediationActionTypeDef",
     {
         "OrderedRemediationActions": List[RemediationActionWithOrderTypeDef],
     },
 )
 _OptionalPossibleRemediationActionTypeDef = TypedDict(
@@ -1887,21 +1827,19 @@
     {
         "Description": str,
         "IsDefaultAction": bool,
     },
     total=False,
 )
 
-
 class PossibleRemediationActionTypeDef(
     _RequiredPossibleRemediationActionTypeDef, _OptionalPossibleRemediationActionTypeDef
 ):
     pass
 
-
 GetPolicyResponseTypeDef = TypedDict(
     "GetPolicyResponseTypeDef",
     {
         "Policy": PolicyTypeDef,
         "PolicyArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1917,21 +1855,19 @@
     "_OptionalPutPolicyRequestRequestTypeDef",
     {
         "TagList": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class PutPolicyRequestRequestTypeDef(
     _RequiredPutPolicyRequestRequestTypeDef, _OptionalPutPolicyRequestRequestTypeDef
 ):
     pass
 
-
 PutPolicyResponseTypeDef = TypedDict(
     "PutPolicyResponseTypeDef",
     {
         "Policy": PolicyTypeDef,
         "PolicyArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1991,19 +1927,17 @@
     {
         "ResourceTags": List[TagTypeDef],
         "ResourceDescription": str,
     },
     total=False,
 )
 
-
 class ViolationDetailTypeDef(_RequiredViolationDetailTypeDef, _OptionalViolationDetailTypeDef):
     pass
 
-
 GetViolationDetailsResponseTypeDef = TypedDict(
     "GetViolationDetailsResponseTypeDef",
     {
         "ViolationDetail": ViolationDetailTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-fms-1.26.22/mypy_boto3_fms/type_defs.pyi` & `mypy-boto3-fms-1.26.5/mypy_boto3_fms/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,27 +25,27 @@
     MarketplaceSubscriptionOnboardingStatusType,
     PolicyComplianceStatusTypeType,
     RemediationActionTypeType,
     RuleOrderType,
     SecurityServiceTypeType,
     TargetTypeType,
     ThirdPartyFirewallAssociationStatusType,
-    ThirdPartyFirewallType,
     ViolationReasonType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ActionTargetTypeDef",
     "AppTypeDef",
     "AssociateAdminAccountRequestRequestTypeDef",
     "AssociateThirdPartyFirewallRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AwsEc2NetworkInterfaceViolationTypeDef",
@@ -210,15 +210,15 @@
         "AdminAccount": str,
     },
 )
 
 AssociateThirdPartyFirewallRequestRequestTypeDef = TypedDict(
     "AssociateThirdPartyFirewallRequestRequestTypeDef",
     {
-        "ThirdPartyFirewall": ThirdPartyFirewallType,
+        "ThirdPartyFirewall": Literal["PALO_ALTO_NETWORKS_CLOUD_NGFW"],
     },
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
@@ -300,19 +300,21 @@
     "_OptionalDeletePolicyRequestRequestTypeDef",
     {
         "DeleteAllPolicyResources": bool,
     },
     total=False,
 )
 
+
 class DeletePolicyRequestRequestTypeDef(
     _RequiredDeletePolicyRequestRequestTypeDef, _OptionalDeletePolicyRequestRequestTypeDef
 ):
     pass
 
+
 DeleteProtocolsListRequestRequestTypeDef = TypedDict(
     "DeleteProtocolsListRequestRequestTypeDef",
     {
         "ListId": str,
     },
 )
 
@@ -322,15 +324,15 @@
         "Identifier": str,
     },
 )
 
 DisassociateThirdPartyFirewallRequestRequestTypeDef = TypedDict(
     "DisassociateThirdPartyFirewallRequestRequestTypeDef",
     {
-        "ThirdPartyFirewall": ThirdPartyFirewallType,
+        "ThirdPartyFirewall": Literal["PALO_ALTO_NETWORKS_CLOUD_NGFW"],
     },
 )
 
 DiscoveredResourceTypeDef = TypedDict(
     "DiscoveredResourceTypeDef",
     {
         "URI": str,
@@ -437,19 +439,21 @@
     "_OptionalGetAppsListRequestRequestTypeDef",
     {
         "DefaultList": bool,
     },
     total=False,
 )
 
+
 class GetAppsListRequestRequestTypeDef(
     _RequiredGetAppsListRequestRequestTypeDef, _OptionalGetAppsListRequestRequestTypeDef
 ):
     pass
 
+
 GetComplianceDetailRequestRequestTypeDef = TypedDict(
     "GetComplianceDetailRequestRequestTypeDef",
     {
         "PolicyId": str,
         "MemberAccount": str,
     },
 )
@@ -475,39 +479,43 @@
         "EndTime": Union[datetime, str],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class GetProtectionStatusRequestRequestTypeDef(
     _RequiredGetProtectionStatusRequestRequestTypeDef,
     _OptionalGetProtectionStatusRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetProtocolsListRequestRequestTypeDef = TypedDict(
     "_RequiredGetProtocolsListRequestRequestTypeDef",
     {
         "ListId": str,
     },
 )
 _OptionalGetProtocolsListRequestRequestTypeDef = TypedDict(
     "_OptionalGetProtocolsListRequestRequestTypeDef",
     {
         "DefaultList": bool,
     },
     total=False,
 )
 
+
 class GetProtocolsListRequestRequestTypeDef(
     _RequiredGetProtocolsListRequestRequestTypeDef, _OptionalGetProtocolsListRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredProtocolsListDataTypeDef = TypedDict(
     "_RequiredProtocolsListDataTypeDef",
     {
         "ListName": str,
         "ProtocolsList": List[str],
     },
 )
@@ -519,19 +527,21 @@
         "CreateTime": datetime,
         "LastUpdateTime": datetime,
         "PreviousProtocolsList": Dict[str, List[str]],
     },
     total=False,
 )
 
+
 class ProtocolsListDataTypeDef(
     _RequiredProtocolsListDataTypeDef, _OptionalProtocolsListDataTypeDef
 ):
     pass
 
+
 GetResourceSetRequestRequestTypeDef = TypedDict(
     "GetResourceSetRequestRequestTypeDef",
     {
         "Identifier": str,
     },
 )
 
@@ -549,21 +559,23 @@
         "Description": str,
         "UpdateToken": str,
         "LastUpdateTime": datetime,
     },
     total=False,
 )
 
+
 class ResourceSetTypeDef(_RequiredResourceSetTypeDef, _OptionalResourceSetTypeDef):
     pass
 
+
 GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef = TypedDict(
     "GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef",
     {
-        "ThirdPartyFirewall": ThirdPartyFirewallType,
+        "ThirdPartyFirewall": Literal["PALO_ALTO_NETWORKS_CLOUD_NGFW"],
     },
 )
 
 GetViolationDetailsRequestRequestTypeDef = TypedDict(
     "GetViolationDetailsRequestRequestTypeDef",
     {
         "PolicyId": str,
@@ -594,19 +606,21 @@
     {
         "DefaultLists": bool,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListAppsListsRequestRequestTypeDef(
     _RequiredListAppsListsRequestRequestTypeDef, _OptionalListAppsListsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListComplianceStatusRequestRequestTypeDef = TypedDict(
     "_RequiredListComplianceStatusRequestRequestTypeDef",
     {
         "PolicyId": str,
     },
 )
 _OptionalListComplianceStatusRequestRequestTypeDef = TypedDict(
@@ -614,20 +628,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListComplianceStatusRequestRequestTypeDef(
     _RequiredListComplianceStatusRequestRequestTypeDef,
     _OptionalListComplianceStatusRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListDiscoveredResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListDiscoveredResourcesRequestRequestTypeDef",
     {
         "MemberAccountIds": Sequence[str],
         "ResourceType": str,
     },
 )
@@ -636,20 +652,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListDiscoveredResourcesRequestRequestTypeDef(
     _RequiredListDiscoveredResourcesRequestRequestTypeDef,
     _OptionalListDiscoveredResourcesRequestRequestTypeDef,
 ):
     pass
 
+
 ListMemberAccountsRequestRequestTypeDef = TypedDict(
     "ListMemberAccountsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -689,20 +707,22 @@
     {
         "DefaultLists": bool,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListProtocolsListsRequestRequestTypeDef(
     _RequiredListProtocolsListsRequestRequestTypeDef,
     _OptionalListProtocolsListsRequestRequestTypeDef,
 ):
     pass
 
+
 ProtocolsListDataSummaryTypeDef = TypedDict(
     "ProtocolsListDataSummaryTypeDef",
     {
         "ListArn": str,
         "ListId": str,
         "ListName": str,
         "ProtocolsList": List[str],
@@ -721,37 +741,41 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListResourceSetResourcesRequestRequestTypeDef(
     _RequiredListResourceSetResourcesRequestRequestTypeDef,
     _OptionalListResourceSetResourcesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredResourceTypeDef = TypedDict(
     "_RequiredResourceTypeDef",
     {
         "URI": str,
     },
 )
 _OptionalResourceTypeDef = TypedDict(
     "_OptionalResourceTypeDef",
     {
         "AccountId": str,
     },
     total=False,
 )
 
+
 class ResourceTypeDef(_RequiredResourceTypeDef, _OptionalResourceTypeDef):
     pass
 
+
 ListResourceSetsRequestRequestTypeDef = TypedDict(
     "ListResourceSetsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -782,32 +806,34 @@
         "Value": str,
     },
 )
 
 _RequiredListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef",
     {
-        "ThirdPartyFirewall": ThirdPartyFirewallType,
+        "ThirdPartyFirewall": Literal["PALO_ALTO_NETWORKS_CLOUD_NGFW"],
         "MaxResults": int,
     },
 )
 _OptionalListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef = TypedDict(
     "_OptionalListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef(
     _RequiredListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef,
     _OptionalListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef,
 ):
     pass
 
+
 ThirdPartyFirewallFirewallPolicyTypeDef = TypedDict(
     "ThirdPartyFirewallFirewallPolicyTypeDef",
     {
         "FirewallPolicyId": str,
         "FirewallPolicyName": str,
     },
     total=False,
@@ -910,17 +936,19 @@
     "_OptionalResourceTagTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
+
 class ResourceTagTypeDef(_RequiredResourceTagTypeDef, _OptionalResourceTagTypeDef):
     pass
 
+
 PutNotificationChannelRequestRequestTypeDef = TypedDict(
     "PutNotificationChannelRequestRequestTypeDef",
     {
         "SnsTopicArn": str,
         "SnsRoleName": str,
     },
 )
@@ -992,19 +1020,21 @@
         "Description": str,
         "SubnetId": ActionTargetTypeDef,
         "GatewayId": ActionTargetTypeDef,
     },
     total=False,
 )
 
+
 class EC2AssociateRouteTableActionTypeDef(
     _RequiredEC2AssociateRouteTableActionTypeDef, _OptionalEC2AssociateRouteTableActionTypeDef
 ):
     pass
 
+
 _RequiredEC2CopyRouteTableActionTypeDef = TypedDict(
     "_RequiredEC2CopyRouteTableActionTypeDef",
     {
         "VpcId": ActionTargetTypeDef,
         "RouteTableId": ActionTargetTypeDef,
     },
 )
@@ -1012,19 +1042,21 @@
     "_OptionalEC2CopyRouteTableActionTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class EC2CopyRouteTableActionTypeDef(
     _RequiredEC2CopyRouteTableActionTypeDef, _OptionalEC2CopyRouteTableActionTypeDef
 ):
     pass
 
+
 _RequiredEC2CreateRouteActionTypeDef = TypedDict(
     "_RequiredEC2CreateRouteActionTypeDef",
     {
         "RouteTableId": ActionTargetTypeDef,
     },
 )
 _OptionalEC2CreateRouteActionTypeDef = TypedDict(
@@ -1036,38 +1068,42 @@
         "DestinationIpv6CidrBlock": str,
         "VpcEndpointId": ActionTargetTypeDef,
         "GatewayId": ActionTargetTypeDef,
     },
     total=False,
 )
 
+
 class EC2CreateRouteActionTypeDef(
     _RequiredEC2CreateRouteActionTypeDef, _OptionalEC2CreateRouteActionTypeDef
 ):
     pass
 
+
 _RequiredEC2CreateRouteTableActionTypeDef = TypedDict(
     "_RequiredEC2CreateRouteTableActionTypeDef",
     {
         "VpcId": ActionTargetTypeDef,
     },
 )
 _OptionalEC2CreateRouteTableActionTypeDef = TypedDict(
     "_OptionalEC2CreateRouteTableActionTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class EC2CreateRouteTableActionTypeDef(
     _RequiredEC2CreateRouteTableActionTypeDef, _OptionalEC2CreateRouteTableActionTypeDef
 ):
     pass
 
+
 _RequiredEC2DeleteRouteActionTypeDef = TypedDict(
     "_RequiredEC2DeleteRouteActionTypeDef",
     {
         "RouteTableId": ActionTargetTypeDef,
     },
 )
 _OptionalEC2DeleteRouteActionTypeDef = TypedDict(
@@ -1077,19 +1113,21 @@
         "DestinationCidrBlock": str,
         "DestinationPrefixListId": str,
         "DestinationIpv6CidrBlock": str,
     },
     total=False,
 )
 
+
 class EC2DeleteRouteActionTypeDef(
     _RequiredEC2DeleteRouteActionTypeDef, _OptionalEC2DeleteRouteActionTypeDef
 ):
     pass
 
+
 _RequiredEC2ReplaceRouteActionTypeDef = TypedDict(
     "_RequiredEC2ReplaceRouteActionTypeDef",
     {
         "RouteTableId": ActionTargetTypeDef,
     },
 )
 _OptionalEC2ReplaceRouteActionTypeDef = TypedDict(
@@ -1100,19 +1138,21 @@
         "DestinationPrefixListId": str,
         "DestinationIpv6CidrBlock": str,
         "GatewayId": ActionTargetTypeDef,
     },
     total=False,
 )
 
+
 class EC2ReplaceRouteActionTypeDef(
     _RequiredEC2ReplaceRouteActionTypeDef, _OptionalEC2ReplaceRouteActionTypeDef
 ):
     pass
 
+
 _RequiredEC2ReplaceRouteTableAssociationActionTypeDef = TypedDict(
     "_RequiredEC2ReplaceRouteTableAssociationActionTypeDef",
     {
         "AssociationId": ActionTargetTypeDef,
         "RouteTableId": ActionTargetTypeDef,
     },
 )
@@ -1120,20 +1160,22 @@
     "_OptionalEC2ReplaceRouteTableAssociationActionTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class EC2ReplaceRouteTableAssociationActionTypeDef(
     _RequiredEC2ReplaceRouteTableAssociationActionTypeDef,
     _OptionalEC2ReplaceRouteTableAssociationActionTypeDef,
 ):
     pass
 
+
 AppsListDataSummaryTypeDef = TypedDict(
     "AppsListDataSummaryTypeDef",
     {
         "ListArn": str,
         "ListId": str,
         "ListName": str,
         "AppsList": List[AppTypeDef],
@@ -1156,17 +1198,19 @@
         "CreateTime": datetime,
         "LastUpdateTime": datetime,
         "PreviousAppsList": Dict[str, List[AppTypeDef]],
     },
     total=False,
 )
 
+
 class AppsListDataTypeDef(_RequiredAppsListDataTypeDef, _OptionalAppsListDataTypeDef):
     pass
 
+
 AssociateThirdPartyFirewallResponseTypeDef = TypedDict(
     "AssociateThirdPartyFirewallResponseTypeDef",
     {
         "ThirdPartyFirewallStatus": ThirdPartyFirewallAssociationStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1362,20 +1406,22 @@
     "_OptionalListComplianceStatusRequestListComplianceStatusPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListComplianceStatusRequestListComplianceStatusPaginateTypeDef(
     _RequiredListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
     _OptionalListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
 ):
     pass
 
+
 ListMemberAccountsRequestListMemberAccountsPaginateTypeDef = TypedDict(
     "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -1396,31 +1442,33 @@
     },
     total=False,
 )
 
 _RequiredListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef = TypedDict(
     "_RequiredListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef",
     {
-        "ThirdPartyFirewall": ThirdPartyFirewallType,
+        "ThirdPartyFirewall": Literal["PALO_ALTO_NETWORKS_CLOUD_NGFW"],
     },
 )
 _OptionalListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef = TypedDict(
     "_OptionalListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef(
     _RequiredListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
     _OptionalListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
 ):
     pass
 
+
 ListPoliciesResponseTypeDef = TypedDict(
     "ListPoliciesResponseTypeDef",
     {
         "PolicyList": List[PolicySummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1471,38 +1519,42 @@
     "_OptionalPutProtocolsListRequestRequestTypeDef",
     {
         "TagList": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class PutProtocolsListRequestRequestTypeDef(
     _RequiredPutProtocolsListRequestRequestTypeDef, _OptionalPutProtocolsListRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredPutResourceSetRequestRequestTypeDef = TypedDict(
     "_RequiredPutResourceSetRequestRequestTypeDef",
     {
         "ResourceSet": ResourceSetTypeDef,
     },
 )
 _OptionalPutResourceSetRequestRequestTypeDef = TypedDict(
     "_OptionalPutResourceSetRequestRequestTypeDef",
     {
         "TagList": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class PutResourceSetRequestRequestTypeDef(
     _RequiredPutResourceSetRequestRequestTypeDef, _OptionalPutResourceSetRequestRequestTypeDef
 ):
     pass
 
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagList": Sequence[TagTypeDef],
     },
 )
@@ -1689,19 +1741,21 @@
     "_OptionalPutAppsListRequestRequestTypeDef",
     {
         "TagList": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class PutAppsListRequestRequestTypeDef(
     _RequiredPutAppsListRequestRequestTypeDef, _OptionalPutAppsListRequestRequestTypeDef
 ):
     pass
 
+
 PutAppsListResponseTypeDef = TypedDict(
     "PutAppsListResponseTypeDef",
     {
         "AppsList": AppsListDataTypeDef,
         "AppsListArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1749,19 +1803,21 @@
     {
         "ManagedServiceData": str,
         "PolicyOption": PolicyOptionTypeDef,
     },
     total=False,
 )
 
+
 class SecurityServicePolicyDataTypeDef(
     _RequiredSecurityServicePolicyDataTypeDef, _OptionalSecurityServicePolicyDataTypeDef
 ):
     pass
 
+
 AwsVPCSecurityGroupViolationTypeDef = TypedDict(
     "AwsVPCSecurityGroupViolationTypeDef",
     {
         "ViolationTarget": str,
         "ViolationTargetDescription": str,
         "PartialMatches": List[PartialMatchTypeDef],
         "PossibleSecurityGroupRemediationActions": List[SecurityGroupRemediationActionTypeDef],
@@ -1810,17 +1866,19 @@
         "ExcludeMap": Dict[CustomerPolicyScopeIdTypeType, List[str]],
         "ResourceSetIds": List[str],
         "PolicyDescription": str,
     },
     total=False,
 )
 
+
 class PolicyTypeDef(_RequiredPolicyTypeDef, _OptionalPolicyTypeDef):
     pass
 
+
 _RequiredPossibleRemediationActionTypeDef = TypedDict(
     "_RequiredPossibleRemediationActionTypeDef",
     {
         "OrderedRemediationActions": List[RemediationActionWithOrderTypeDef],
     },
 )
 _OptionalPossibleRemediationActionTypeDef = TypedDict(
@@ -1828,19 +1886,21 @@
     {
         "Description": str,
         "IsDefaultAction": bool,
     },
     total=False,
 )
 
+
 class PossibleRemediationActionTypeDef(
     _RequiredPossibleRemediationActionTypeDef, _OptionalPossibleRemediationActionTypeDef
 ):
     pass
 
+
 GetPolicyResponseTypeDef = TypedDict(
     "GetPolicyResponseTypeDef",
     {
         "Policy": PolicyTypeDef,
         "PolicyArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1856,19 +1916,21 @@
     "_OptionalPutPolicyRequestRequestTypeDef",
     {
         "TagList": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class PutPolicyRequestRequestTypeDef(
     _RequiredPutPolicyRequestRequestTypeDef, _OptionalPutPolicyRequestRequestTypeDef
 ):
     pass
 
+
 PutPolicyResponseTypeDef = TypedDict(
     "PutPolicyResponseTypeDef",
     {
         "Policy": PolicyTypeDef,
         "PolicyArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1928,17 +1990,19 @@
     {
         "ResourceTags": List[TagTypeDef],
         "ResourceDescription": str,
     },
     total=False,
 )
 
+
 class ViolationDetailTypeDef(_RequiredViolationDetailTypeDef, _OptionalViolationDetailTypeDef):
     pass
 
+
 GetViolationDetailsResponseTypeDef = TypedDict(
     "GetViolationDetailsResponseTypeDef",
     {
         "ViolationDetail": ViolationDetailTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-fms-1.26.22/mypy_boto3_fms.egg-info/PKG-INFO` & `mypy-boto3-fms-1.26.5/mypy_boto3_fms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-fms
-Version: 1.26.22
-Summary: Type annotations for boto3.FMS 1.26.22 service generated with mypy-boto3-builder 7.11.11
+Version: 1.26.5
+Summary: Type annotations for boto3.FMS 1.26.5 service generated with mypy-boto3-builder 7.11.10
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -37,24 +37,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-fms.svg?color=blue)](https://pypi.org/project/mypy-boto3-fms)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-fms?color=blue)](https://pypistats.org/packages/mypy-boto3-fms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FMS 1.26.22](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
+[boto3.FMS 1.26.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-fms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-fms-1.26.22/mypy_boto3_fms.egg-info/SOURCES.txt` & `mypy-boto3-fms-1.26.5/mypy_boto3_fms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fms-1.26.22/setup.py` & `mypy-boto3-fms-1.26.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-fms",
-    version="1.26.22",
+    version="1.26.5",
     packages=["mypy_boto3_fms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.FMS 1.26.22 service generated with mypy-boto3-builder 7.11.11"
+        "Type annotations for boto3.FMS 1.26.5 service generated with mypy-boto3-builder 7.11.10"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

