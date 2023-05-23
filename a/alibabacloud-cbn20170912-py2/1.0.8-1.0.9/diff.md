# Comparing `tmp/alibabacloud_cbn20170912_py2-1.0.8.tar.gz` & `tmp/alibabacloud_cbn20170912_py2-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cbn20170912_py2-1.0.8.tar", last modified: Mon Mar 13 02:43:55 2023, max compression
+gzip compressed data, was "dist/alibabacloud_cbn20170912_py2-1.0.9.tar", last modified: Fri Mar 17 03:27:37 2023, max compression
```

## Comparing `alibabacloud_cbn20170912_py2-1.0.8.tar` & `alibabacloud_cbn20170912_py2-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 02:43:55.000000 alibabacloud_cbn20170912_py2-1.0.8/
--rw-r--r--   0 root         (0) root         (0)     4475 2023-03-13 02:43:55.000000 alibabacloud_cbn20170912_py2-1.0.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-03-13 02:43:55.000000 alibabacloud_cbn20170912_py2-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-03-13 02:43:55.000000 alibabacloud_cbn20170912_py2-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2493 2023-03-13 02:43:55.000000 alibabacloud_cbn20170912_py2-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1033 2023-03-13 02:43:55.000000 alibabacloud_cbn20170912_py2-1.0.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1116 2023-03-13 02:43:55.000000 alibabacloud_cbn20170912_py2-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 02:43:55.000000 alibabacloud_cbn20170912_py2-1.0.8/alibabacloud_cbn20170912/
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-13 02:43:55.000000 alibabacloud_cbn20170912_py2-1.0.8/alibabacloud_cbn20170912/__init__.py
--rw-r--r--   0 root         (0) root         (0)   534829 2023-03-13 02:43:55.000000 alibabacloud_cbn20170912_py2-1.0.8/alibabacloud_cbn20170912/client.py
--rw-r--r--   0 root         (0) root         (0)  1441451 2023-03-13 02:43:55.000000 alibabacloud_cbn20170912_py2-1.0.8/alibabacloud_cbn20170912/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 02:43:55.000000 alibabacloud_cbn20170912_py2-1.0.8/alibabacloud_cbn20170912_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2493 2023-03-13 02:43:55.000000 alibabacloud_cbn20170912_py2-1.0.8/alibabacloud_cbn20170912_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      440 2023-03-13 02:43:55.000000 alibabacloud_cbn20170912_py2-1.0.8/alibabacloud_cbn20170912_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-13 02:43:55.000000 alibabacloud_cbn20170912_py2-1.0.8/alibabacloud_cbn20170912_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-03-13 02:43:55.000000 alibabacloud_cbn20170912_py2-1.0.8/alibabacloud_cbn20170912_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-03-13 02:43:55.000000 alibabacloud_cbn20170912_py2-1.0.8/alibabacloud_cbn20170912_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-13 02:43:55.000000 alibabacloud_cbn20170912_py2-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2924 2023-03-13 02:43:55.000000 alibabacloud_cbn20170912_py2-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 03:27:37.000000 alibabacloud_cbn20170912_py2-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)     4664 2023-03-17 03:27:37.000000 alibabacloud_cbn20170912_py2-1.0.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-03-17 03:27:37.000000 alibabacloud_cbn20170912_py2-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-03-17 03:27:37.000000 alibabacloud_cbn20170912_py2-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2493 2023-03-17 03:27:37.000000 alibabacloud_cbn20170912_py2-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-03-17 03:27:37.000000 alibabacloud_cbn20170912_py2-1.0.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1116 2023-03-17 03:27:37.000000 alibabacloud_cbn20170912_py2-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 03:27:37.000000 alibabacloud_cbn20170912_py2-1.0.9/alibabacloud_cbn20170912/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-03-17 03:27:37.000000 alibabacloud_cbn20170912_py2-1.0.9/alibabacloud_cbn20170912/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   534888 2023-03-17 03:27:37.000000 alibabacloud_cbn20170912_py2-1.0.9/alibabacloud_cbn20170912/client.py
+-rw-r--r--   0 root         (0) root         (0)  1441739 2023-03-17 03:27:37.000000 alibabacloud_cbn20170912_py2-1.0.9/alibabacloud_cbn20170912/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 03:27:37.000000 alibabacloud_cbn20170912_py2-1.0.9/alibabacloud_cbn20170912_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2493 2023-03-17 03:27:37.000000 alibabacloud_cbn20170912_py2-1.0.9/alibabacloud_cbn20170912_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      440 2023-03-17 03:27:37.000000 alibabacloud_cbn20170912_py2-1.0.9/alibabacloud_cbn20170912_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-17 03:27:37.000000 alibabacloud_cbn20170912_py2-1.0.9/alibabacloud_cbn20170912_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-03-17 03:27:37.000000 alibabacloud_cbn20170912_py2-1.0.9/alibabacloud_cbn20170912_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-03-17 03:27:37.000000 alibabacloud_cbn20170912_py2-1.0.9/alibabacloud_cbn20170912_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-03-17 03:27:37.000000 alibabacloud_cbn20170912_py2-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2924 2023-03-17 03:27:37.000000 alibabacloud_cbn20170912_py2-1.0.9/setup.py
```

### Comparing `alibabacloud_cbn20170912_py2-1.0.8/ChangeLog.md` & `alibabacloud_cbn20170912_py2-1.0.9/ChangeLog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+2023-03-13 Version: 1.0.8
+- Update API DescribeCens support parameter resourceGroupId.
+- Update API DescribeCens support parameter resourceGroupId, tag and response resourceGroupId, tags.
+
 2023-01-13 Version: 1.0.7
 - New API CreateTransitRouteTableAggregation.
 - New API DeleteTransitRouteTableAggregation.
 - New API DescribeTransitRouteTableAggregation.
 - New API DescribeTransitRouteTableAggregationDetail.
 - New API RefreshTransitRouteTableAggregation.
 - Update API CreateTransitRouterRouteTable support parameter RouteTableOptions.
```

### Comparing `alibabacloud_cbn20170912_py2-1.0.8/LICENSE` & `alibabacloud_cbn20170912_py2-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cbn20170912_py2-1.0.8/PKG-INFO` & `alibabacloud_cbn20170912_py2-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_cbn20170912_py2
-Version: 1.0.8
+Version: 1.0.9
 Summary: Alibaba Cloud Cloud Enterprise Network (20170912) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cbn20170912_py2-1.0.8/README-CN.md` & `alibabacloud_cbn20170912_py2-1.0.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cbn20170912_py2-1.0.8/README.md` & `alibabacloud_cbn20170912_py2-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cbn20170912_py2-1.0.8/alibabacloud_cbn20170912/client.py` & `alibabacloud_cbn20170912_py2-1.0.9/alibabacloud_cbn20170912/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1256,15 +1256,15 @@
 
     def create_transit_route_table_aggregation_with_options(self, request, runtime):
         """
         # Prerequisites
         After you add an aggregate route to a route table of an Enterprise Edition transit router, the Enterprise Edition transit router advertises its routes only to route tables of virtual private clouds (VPCs) that are associated with a route table of the Enterprise Edition transit router and have route synchronization enabled.
         Perform the following operations before you create an aggregate route. Otherwise, the Enterprise Edition transit router does not advertise routes to VPC route tables:
         *   Associated forwarding is enabled between the VPCs and the Enterprise Edition transit router. For more information, see [AssociateTransitRouterAttachmentWithRouteTable](~~261242~~).
-        *   The VPCs have route synchronization enabled. For more information, see [CreateTransitRouterVpcAttachment](~~261358~~).
+        *   Route synchronization is enabled for the VPCs. For more information, see [CreateTransitRouterVpcAttachment](~~261358~~).
         
 
         @param request: CreateTransitRouteTableAggregationRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: CreateTransitRouteTableAggregationResponse
@@ -1285,16 +1285,16 @@
             query['ResourceOwnerId'] = request.resource_owner_id
         if not UtilClient.is_unset(request.transit_route_table_aggregation_cidr):
             query['TransitRouteTableAggregationCidr'] = request.transit_route_table_aggregation_cidr
         if not UtilClient.is_unset(request.transit_route_table_aggregation_description):
             query['TransitRouteTableAggregationDescription'] = request.transit_route_table_aggregation_description
         if not UtilClient.is_unset(request.transit_route_table_aggregation_name):
             query['TransitRouteTableAggregationName'] = request.transit_route_table_aggregation_name
-        if not UtilClient.is_unset(request.transit_route_table_aggregation_scop):
-            query['TransitRouteTableAggregationScop'] = request.transit_route_table_aggregation_scop
+        if not UtilClient.is_unset(request.transit_route_table_aggregation_scope):
+            query['TransitRouteTableAggregationScope'] = request.transit_route_table_aggregation_scope
         if not UtilClient.is_unset(request.transit_route_table_id):
             query['TransitRouteTableId'] = request.transit_route_table_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='CreateTransitRouteTableAggregation',
@@ -1314,15 +1314,15 @@
 
     def create_transit_route_table_aggregation(self, request):
         """
         # Prerequisites
         After you add an aggregate route to a route table of an Enterprise Edition transit router, the Enterprise Edition transit router advertises its routes only to route tables of virtual private clouds (VPCs) that are associated with a route table of the Enterprise Edition transit router and have route synchronization enabled.
         Perform the following operations before you create an aggregate route. Otherwise, the Enterprise Edition transit router does not advertise routes to VPC route tables:
         *   Associated forwarding is enabled between the VPCs and the Enterprise Edition transit router. For more information, see [AssociateTransitRouterAttachmentWithRouteTable](~~261242~~).
-        *   The VPCs have route synchronization enabled. For more information, see [CreateTransitRouterVpcAttachment](~~261358~~).
+        *   Route synchronization is enabled for the VPCs. For more information, see [CreateTransitRouterVpcAttachment](~~261358~~).
         
 
         @param request: CreateTransitRouteTableAggregationRequest
 
         @return: CreateTransitRouteTableAggregationResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -1495,15 +1495,15 @@
         """
         runtime = util_models.RuntimeOptions()
         return self.create_transit_router_cidr_with_options(request, runtime)
 
     def create_transit_router_multicast_domain_with_options(self, request, runtime):
         """
         Before you call this operation, read the following rules:
-        *   Only Enterprise Edition transit routers in the Australia (Sydney) and UK (London) regions support the multicast feature. Multicast is unavailable by default. If you want to enable multicast, contact your sales manager or [submit a ticket](https://selfservice.console.aliyun.com/ticket/category/cbn/today) to apply for multicast resources.
+        *   Only Enterprise Edition transit routers in the Australia (Sydney) and UK (London) regions support the multicast feature. Multicast is unavailable by default. If you want to enable multicast, contact your sales manager or [submit a ticket](https://workorder-intl.console.aliyun.com/#/ticket/createIndex) to apply for multicast resources.
         *   Make sure that an Enterprise Edition transit router is deployed in the region where you want to create the multicast domain, and the multicast feature is enabled for the Enterprise Edition transit router. For more information, see [CreateTransitRouter](~~261169~~).
         If an Enterprise Edition transit router was created before you apply for multicast resources, the transit router does not support multicast. You can delete the transit router and create a new one. For more information about how to delete an Enterprise Edition transit router, see [DeleteTransitRouter](~~261218~~).
         *   When you call **CreateTransitRouterMulticastDomain**, if you set **CenId** and **RegionId**, you do not need to set **TransitRouterId**. If you set **TransitRouterId**, you do not need to set **CenId** or **RegionId**.
         
 
         @param request: CreateTransitRouterMulticastDomainRequest
 
@@ -1555,15 +1555,15 @@
             cbn_20170912_models.CreateTransitRouterMulticastDomainResponse(),
             self.call_api(params, req, runtime)
         )
 
     def create_transit_router_multicast_domain(self, request):
         """
         Before you call this operation, read the following rules:
-        *   Only Enterprise Edition transit routers in the Australia (Sydney) and UK (London) regions support the multicast feature. Multicast is unavailable by default. If you want to enable multicast, contact your sales manager or [submit a ticket](https://selfservice.console.aliyun.com/ticket/category/cbn/today) to apply for multicast resources.
+        *   Only Enterprise Edition transit routers in the Australia (Sydney) and UK (London) regions support the multicast feature. Multicast is unavailable by default. If you want to enable multicast, contact your sales manager or [submit a ticket](https://workorder-intl.console.aliyun.com/#/ticket/createIndex) to apply for multicast resources.
         *   Make sure that an Enterprise Edition transit router is deployed in the region where you want to create the multicast domain, and the multicast feature is enabled for the Enterprise Edition transit router. For more information, see [CreateTransitRouter](~~261169~~).
         If an Enterprise Edition transit router was created before you apply for multicast resources, the transit router does not support multicast. You can delete the transit router and create a new one. For more information about how to delete an Enterprise Edition transit router, see [DeleteTransitRouter](~~261218~~).
         *   When you call **CreateTransitRouterMulticastDomain**, if you set **CenId** and **RegionId**, you do not need to set **TransitRouterId**. If you set **TransitRouterId**, you do not need to set **CenId** or **RegionId**.
         
 
         @param request: CreateTransitRouterMulticastDomainRequest
 
@@ -1897,15 +1897,15 @@
     def create_transit_router_vbr_attachment_with_options(self, request, runtime):
         """
         For more information about the regions and zones that support Enterprise Edition transit routers, see [What is CEN?](~~181681~~)
         *   You can use the following methods to connect a VBR to an Enterprise Edition transit router:
         *   If an Enterprise Edition transit router is already created in the region where you want to create a VBR connection, set the **VbrId** and **TransitRouterId** parameters.
         *   If no Enterprise Edition transit router is created in the region where you want to create a VBR connection, set the **VbrId**, **CenId**, and **RegionId** parameters. Then, the system automatically creates an Enterprise Edition transit router in the specified region.
         *   **CreateTransitRouterVbrAttachment** is an asynchronous operation. After you send a request, the system returns a VBR connection ID and runs the task in the background. You can call the **ListTransitRouterVbrAttachments** operation to query the status of a VBR connection.
-        *   If a VBR is in the **Attaching** state, the VBR connection is being created. You can query the VBR connection but cannot perform other operations.
+        *   If a VBR connection is in the **Attaching** state, the VBR connection is being created. You can query the VBR connection but cannot perform other operations.
         *   If a VBR connection is in the **Attached** state, the VBR connection is created.
         
 
         @param request: CreateTransitRouterVbrAttachmentRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
@@ -1965,15 +1965,15 @@
     def create_transit_router_vbr_attachment(self, request):
         """
         For more information about the regions and zones that support Enterprise Edition transit routers, see [What is CEN?](~~181681~~)
         *   You can use the following methods to connect a VBR to an Enterprise Edition transit router:
         *   If an Enterprise Edition transit router is already created in the region where you want to create a VBR connection, set the **VbrId** and **TransitRouterId** parameters.
         *   If no Enterprise Edition transit router is created in the region where you want to create a VBR connection, set the **VbrId**, **CenId**, and **RegionId** parameters. Then, the system automatically creates an Enterprise Edition transit router in the specified region.
         *   **CreateTransitRouterVbrAttachment** is an asynchronous operation. After you send a request, the system returns a VBR connection ID and runs the task in the background. You can call the **ListTransitRouterVbrAttachments** operation to query the status of a VBR connection.
-        *   If a VBR is in the **Attaching** state, the VBR connection is being created. You can query the VBR connection but cannot perform other operations.
+        *   If a VBR connection is in the **Attaching** state, the VBR connection is being created. You can query the VBR connection but cannot perform other operations.
         *   If a VBR connection is in the **Attached** state, the VBR connection is created.
         
 
         @param request: CreateTransitRouterVbrAttachmentRequest
 
         @return: CreateTransitRouterVbrAttachmentResponse
         """
@@ -1982,15 +1982,15 @@
 
     def create_transit_router_vpc_attachment_with_options(self, request, runtime):
         """
         You can use the following methods to connect a VPC to an Enterprise Edition transit router:
         *   If an Enterprise Edition transit router is already created in the region where you want to create a VPC connection, set **VpcId**, **ZoneMappings.N.VSwitchId**, **ZoneMappings.N.ZoneId**, and **TransitRouterId**.
         *   If no Enterprise Edition transit router is created in the region where you want to create a VPC connection, set **VpcId**, **ZoneMappings.N.VSwitchId**, **ZoneMappings.N.ZoneId**, **CenId**, and **RegionId**. When you create a VPC connection, the system automatically creates an Enterprise Edition transit router in the specified region.
         *   **CreateTransitRouterVpcAttachment** is an asynchronous operation. After you send a request, the system returns a VPC connection ID and runs the task in the background. You can call the [ListTransitRouterVpcAttachments](~~261222~~) operation to query the status of a VPC connection.
-        *   If a VPC is in the **Attaching** state, the VPC connection is being created. You can query the VPC connection but cannot perform other operations.
+        *   If a VPC connection is in the **Attaching** state, the VPC connection is being created. You can query the VPC connection but cannot perform other operations.
         *   If a VPC connection is in the **Attached** state, the VPC connection is created.
         *   By default, route learning and associated forwarding are disabled between transit router route tables and VPC connections.
         ## Prerequisites
         Before you call this operation, make sure that the following requirements are met:
         *   At least one vSwitch is deployed for the VPC in the zones supported by Enterprise Edition transit routers. Each vSwitch must have at least one idle IP address. For more information, see [Regions and zones supported by Enterprise Edition transit routers](~~181681~~).
         *   To connect to a network instance that belongs to another Alibaba Cloud account, you must first acquire the required permissions from the account. For more information, see [Acquire permissions to connect to a network instance that belongs to another account](~~181553~~).
         *   VPC connections incur fees. Take note of the billing rules of VPC connections before you create a VPC connection. For more information, see [Billing](~~189836~~).
@@ -2057,15 +2057,15 @@
 
     def create_transit_router_vpc_attachment(self, request):
         """
         You can use the following methods to connect a VPC to an Enterprise Edition transit router:
         *   If an Enterprise Edition transit router is already created in the region where you want to create a VPC connection, set **VpcId**, **ZoneMappings.N.VSwitchId**, **ZoneMappings.N.ZoneId**, and **TransitRouterId**.
         *   If no Enterprise Edition transit router is created in the region where you want to create a VPC connection, set **VpcId**, **ZoneMappings.N.VSwitchId**, **ZoneMappings.N.ZoneId**, **CenId**, and **RegionId**. When you create a VPC connection, the system automatically creates an Enterprise Edition transit router in the specified region.
         *   **CreateTransitRouterVpcAttachment** is an asynchronous operation. After you send a request, the system returns a VPC connection ID and runs the task in the background. You can call the [ListTransitRouterVpcAttachments](~~261222~~) operation to query the status of a VPC connection.
-        *   If a VPC is in the **Attaching** state, the VPC connection is being created. You can query the VPC connection but cannot perform other operations.
+        *   If a VPC connection is in the **Attaching** state, the VPC connection is being created. You can query the VPC connection but cannot perform other operations.
         *   If a VPC connection is in the **Attached** state, the VPC connection is created.
         *   By default, route learning and associated forwarding are disabled between transit router route tables and VPC connections.
         ## Prerequisites
         Before you call this operation, make sure that the following requirements are met:
         *   At least one vSwitch is deployed for the VPC in the zones supported by Enterprise Edition transit routers. Each vSwitch must have at least one idle IP address. For more information, see [Regions and zones supported by Enterprise Edition transit routers](~~181681~~).
         *   To connect to a network instance that belongs to another Alibaba Cloud account, you must first acquire the required permissions from the account. For more information, see [Acquire permissions to connect to a network instance that belongs to another account](~~181553~~).
         *   VPC connections incur fees. Take note of the billing rules of VPC connections before you create a VPC connection. For more information, see [Billing](~~189836~~).
@@ -2076,15 +2076,15 @@
         @return: CreateTransitRouterVpcAttachmentResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_transit_router_vpc_attachment_with_options(request, runtime)
 
     def create_transit_router_vpn_attachment_with_options(self, request, runtime):
         """
-        By default, route learning and associated forwarding are disabled between transit router route tables and VPN attachments.
+        By default, route learning and associated forwarding are disabled between transit router route tables and IPsec-VPN attachments.
         *   When you call `CreateTransitRouterVpnAttachment`, if you set **CenId** and **RegionId**, you do not need to set **TransitRouterId**. If you set **TransitRouterId** and **RegionId**, you do not need to set **CenId**.
         ## Prerequisites
         *   Before you attach an IPsec-VPN connection to a transit router, make sure that at least one IPsec-VPN connection is created in the region where the transit router is deployed. Make sure the IPsec-VPN connection is not associated with a resource. For more information, see [CreateVpnAttachment](~~442455~~).
         *   If the IPsec-VPN connection to be attached to the transit router belongs to a different Alibaba Cloud account, make sure that the transit router has obtained the required permissions from the IPsec-VPN connection. For more information, see [GrantInstanceToTransitRouter](~~417520~~).
         
 
         @param request: CreateTransitRouterVpnAttachmentRequest
@@ -2146,15 +2146,15 @@
         return TeaCore.from_map(
             cbn_20170912_models.CreateTransitRouterVpnAttachmentResponse(),
             self.call_api(params, req, runtime)
         )
 
     def create_transit_router_vpn_attachment(self, request):
         """
-        By default, route learning and associated forwarding are disabled between transit router route tables and VPN attachments.
+        By default, route learning and associated forwarding are disabled between transit router route tables and IPsec-VPN attachments.
         *   When you call `CreateTransitRouterVpnAttachment`, if you set **CenId** and **RegionId**, you do not need to set **TransitRouterId**. If you set **TransitRouterId** and **RegionId**, you do not need to set **CenId**.
         ## Prerequisites
         *   Before you attach an IPsec-VPN connection to a transit router, make sure that at least one IPsec-VPN connection is created in the region where the transit router is deployed. Make sure the IPsec-VPN connection is not associated with a resource. For more information, see [CreateVpnAttachment](~~442455~~).
         *   If the IPsec-VPN connection to be attached to the transit router belongs to a different Alibaba Cloud account, make sure that the transit router has obtained the required permissions from the IPsec-VPN connection. For more information, see [GrantInstanceToTransitRouter](~~417520~~).
         
 
         @param request: CreateTransitRouterVpnAttachmentRequest
```

### Comparing `alibabacloud_cbn20170912_py2-1.0.8/alibabacloud_cbn20170912/models.py` & `alibabacloud_cbn20170912_py2-1.0.9/alibabacloud_cbn20170912/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -768,15 +768,15 @@
     def __init__(self, client_token=None, dry_run=None, owner_account=None, owner_id=None,
                  resource_owner_account=None, resource_owner_id=None, transit_router_attachment_id=None,
                  transit_router_route_table_id=None):
         # The client token that is used to ensure the idempotence of the request.
         # 
         # You can use the client to generate the value, but you must make sure that it is unique among all requests. The client token can contain only ASCII characters.
         # 
-        # > If you do not specify this parameter, the system automatically uses the value of **RequestId**as the value of **ClientToken**. The value of **RequestId** for each API request may be different.
+        # > If you do not specify this parameter, the system automatically uses the value of **RequestId** as the value of **ClientToken**. The value of **RequestId** for each API request may be different.
         self.client_token = client_token  # type: str
         # Specifies whether to perform a dry run. Valid values:
         # 
         # *   **false** (default): performs a dry run. If the request passes the dry run, the associated forwarding correlation is created.
         # *   **true**: performs a dry run and sends the request. If you use this value, the system checks whether the required parameters are set, and whether the request syntax is valid. If the request fails the dry run, an error message is returned. If the request passes the dry run, the system returns the ID of the request.
         self.dry_run = dry_run  # type: bool
         self.owner_account = owner_account  # type: str
@@ -3459,26 +3459,26 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateTransitRouteTableAggregationRequest(TeaModel):
     def __init__(self, client_token=None, dry_run=None, owner_account=None, owner_id=None,
                  resource_owner_account=None, resource_owner_id=None, transit_route_table_aggregation_cidr=None,
-                 transit_route_table_aggregation_description=None, transit_route_table_aggregation_name=None, transit_route_table_aggregation_scop=None,
+                 transit_route_table_aggregation_description=None, transit_route_table_aggregation_name=None, transit_route_table_aggregation_scope=None,
                  transit_route_table_id=None):
         # The client token that is used to ensure the idempotence of the request.
         # 
-        # You can use the client to generate the value, but you must make sure that the value is unique among different requests. The client token can contain only ASCII characters.
+        # You can use the client to generate the token, but you must make sure that the token is unique among different requests. The client token can contain only ASCII characters.
         # 
-        # >  If you do not set this parameter, ClientToken is set to the value of RequestId. The value of RequestId may different for each request.
+        # >  If you do not set this parameter, ClientToken is set to the value of RequestId. The value of RequestId for each API request may be different.
         self.client_token = client_token  # type: str
-        # Specifies whether to precheck the request. Check items include permissions and the status of the specified cloud resources. Valid values:
+        # Specifies whether to perform a dry run. Valid values:
         # 
-        # *   **false** (default): sends the request. If the request passes the precheck, the aggregate route is added.
-        # *   **true**: prechecks the request but does not create the aggregate route. If you use this value, the system checks the required parameters and the request syntax. If the request fails to pass the precheck, an error message is returned. If the request passes the check, the `DryRunOperation` error code is returned.
+        # *   **false** (default): performs a dry run and sends the request.
+        # *   **true**: performs a dry run. The system checks the required parameters and request syntax. If the request fails the dry run, an error message is returned. If the request passes the dry run, the `DryRunOperation` error code is returned.
         self.dry_run = dry_run  # type: bool
         self.owner_account = owner_account  # type: str
         self.owner_id = owner_id  # type: long
         self.resource_owner_account = resource_owner_account  # type: str
         self.resource_owner_id = resource_owner_id  # type: long
         # The destination CIDR block of the aggregate route.
         # 
@@ -3489,20 +3489,17 @@
         self.transit_route_table_aggregation_cidr = transit_route_table_aggregation_cidr  # type: str
         # The description of the aggregate route.
         # 
         # The description must be 2 to 256 characters in length, and can contain letters, digits, and the following special characters: , . ; / @ \_ -. You can also leave the description empty.
         self.transit_route_table_aggregation_description = transit_route_table_aggregation_description  # type: str
         # The name of the aggregate route.
         # 
-        # The name must be 0 to 128 characters in length, and can contain letters, digits, and the following special characters: , . ; / @ \_ -.
+        # The name must be 1 to 128 characters in length, and can contain letters, digits, and the following special characters: , . ; / @ \_ -. You can also leave the name empty.
         self.transit_route_table_aggregation_name = transit_route_table_aggregation_name  # type: str
-        # The scope of networks that you want to advertise the aggregate route.
-        # 
-        # Set the value to **VPC**, which specified that the aggregate route is advertised to VPCs that are in associated forwarding relationship with a route table of the Enterprise Edition transit router and have route synchronization enabled.
-        self.transit_route_table_aggregation_scop = transit_route_table_aggregation_scop  # type: str
+        self.transit_route_table_aggregation_scope = transit_route_table_aggregation_scope  # type: str
         # The ID of the route table of the Enterprise Edition transit router.
         self.transit_route_table_id = transit_route_table_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -3525,16 +3522,16 @@
             result['ResourceOwnerId'] = self.resource_owner_id
         if self.transit_route_table_aggregation_cidr is not None:
             result['TransitRouteTableAggregationCidr'] = self.transit_route_table_aggregation_cidr
         if self.transit_route_table_aggregation_description is not None:
             result['TransitRouteTableAggregationDescription'] = self.transit_route_table_aggregation_description
         if self.transit_route_table_aggregation_name is not None:
             result['TransitRouteTableAggregationName'] = self.transit_route_table_aggregation_name
-        if self.transit_route_table_aggregation_scop is not None:
-            result['TransitRouteTableAggregationScop'] = self.transit_route_table_aggregation_scop
+        if self.transit_route_table_aggregation_scope is not None:
+            result['TransitRouteTableAggregationScope'] = self.transit_route_table_aggregation_scope
         if self.transit_route_table_id is not None:
             result['TransitRouteTableId'] = self.transit_route_table_id
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('ClientToken') is not None:
@@ -3551,16 +3548,16 @@
             self.resource_owner_id = m.get('ResourceOwnerId')
         if m.get('TransitRouteTableAggregationCidr') is not None:
             self.transit_route_table_aggregation_cidr = m.get('TransitRouteTableAggregationCidr')
         if m.get('TransitRouteTableAggregationDescription') is not None:
             self.transit_route_table_aggregation_description = m.get('TransitRouteTableAggregationDescription')
         if m.get('TransitRouteTableAggregationName') is not None:
             self.transit_route_table_aggregation_name = m.get('TransitRouteTableAggregationName')
-        if m.get('TransitRouteTableAggregationScop') is not None:
-            self.transit_route_table_aggregation_scop = m.get('TransitRouteTableAggregationScop')
+        if m.get('TransitRouteTableAggregationScope') is not None:
+            self.transit_route_table_aggregation_scope = m.get('TransitRouteTableAggregationScope')
         if m.get('TransitRouteTableId') is not None:
             self.transit_route_table_id = m.get('TransitRouteTableId')
         return self
 
 
 class CreateTransitRouteTableAggregationResponseBody(TeaModel):
     def __init__(self, request_id=None):
@@ -5399,28 +5396,28 @@
         # *   **false** (default): no
         # *   **true**: yes
         self.auto_publish_route_enabled = auto_publish_route_enabled  # type: bool
         # The ID of the Cloud Enterprise Network (CEN) instance.
         self.cen_id = cen_id  # type: str
         # The client token that is used to ensure the idempotence of the request.
         # 
-        # You can use the client to generate the value, but you must make sure that it is unique among different requests. The client token can contain only ASCII characters.
+        # You can use the client to generate the token, but you must make sure that the token is unique among different requests. The token can contain only ASCII characters.
         # 
         # >  If you do not set this parameter, **ClientToken** is set to the value of **RequestId**. The value of **RequestId** for each API request may be different.
         self.client_token = client_token  # type: str
-        # Specifies whether to perform a dry run. Default values:
+        # Specifies whether to perform a dry run to check information such as the permissions and the instance status. Valid values:
         # 
         # *   **false** (default): performs a dry run and sends the request.
         # *   **true**: performs a dry run. The system checks the required parameters and request syntax. If the request fails the dry run, an error message is returned. If the request passes the dry run, the system returns the ID of the request.
         self.dry_run = dry_run  # type: bool
         self.owner_account = owner_account  # type: str
         self.owner_id = owner_id  # type: long
-        # The region ID of the VBR.
+        # The ID of the region where the VBR is deployed.
         # 
-        # You can call the [DescribeRegions](~~36063~~) operation to obtain the region ID.
+        # You can call the [DescribeRegions](~~36063~~) operation to query the most recent region list.
         self.region_id = region_id  # type: str
         self.resource_owner_account = resource_owner_account  # type: str
         self.resource_owner_id = resource_owner_id  # type: long
         # The information about the tags.
         # 
         # You can specify at most 20 tags in each call.
         self.tag = tag  # type: list[CreateTransitRouterVbrAttachmentRequestTag]
@@ -5434,15 +5431,15 @@
         self.transit_router_attachment_name = transit_router_attachment_name  # type: str
         # The ID of the Enterprise Edition transit router.
         self.transit_router_id = transit_router_id  # type: str
         # The ID of the VBR.
         self.vbr_id = vbr_id  # type: str
         # The ID of the Alibaba Cloud account to which the VBR belongs. The default value is the ID of the current Alibaba Cloud account.
         # 
-        # > If the network instance and the CEN instance belong to different Alibaba Cloud accounts, this parameter is required.
+        # > If the network instance and CEN instance belong to different Alibaba Cloud accounts, this parameter is required.
         self.vbr_owner_id = vbr_owner_id  # type: long
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
                     k.validate()
@@ -5632,19 +5629,19 @@
         if m.get('Value') is not None:
             self.value = m.get('Value')
         return self
 
 
 class CreateTransitRouterVpcAttachmentRequestZoneMappings(TeaModel):
     def __init__(self, v_switch_id=None, zone_id=None):
-        # A vSwitch that is deployed in the zone that supports Enterprise Edition transit routers.
+        # A vSwitch in a zone of the Enterprise Edition transit router.
         # 
         # You can specify vSwitches for at most 10 zones in each call.
         self.v_switch_id = v_switch_id  # type: str
-        # The ID of the zone that supports Enterprise Edition transit routers.
+        # The ID of the zone supported by Enterprise Edition transit routers.
         # 
         # You can call the [DescribeZones](~~36064~~) operation to query the most recent zone list.
         # 
         # You can specify at most 10 zones in each call.
         self.zone_id = zone_id  # type: str
 
     def validate(self):
@@ -5674,23 +5671,23 @@
 class CreateTransitRouterVpcAttachmentRequest(TeaModel):
     def __init__(self, cen_id=None, charge_type=None, client_token=None, dry_run=None, owner_account=None,
                  owner_id=None, region_id=None, resource_owner_account=None, resource_owner_id=None, tag=None,
                  transit_router_attachment_description=None, transit_router_attachment_name=None, transit_router_id=None, vpc_id=None, vpc_owner_id=None,
                  zone_mappings=None):
         # The ID of the Cloud Enterprise Network (CEN) instance.
         self.cen_id = cen_id  # type: str
-        # The billing method. The default value is **POSTPAY**, which specifies the pay-as-you-go billing method.
+        # The billing method. Valid values: The default value is **POSTPAY**, which specifies the pay-as-you-go billing method.
         self.charge_type = charge_type  # type: str
         # The client token that is used to ensure the idempotence of the request.
         # 
-        # You can use the client to generate the value, but you must make sure that it is unique among different requests. The token can contain only ASCII characters.
+        # You can use the client to generate the token, but you must make sure that the token is unique among different requests. The token can contain only ASCII characters.
         # 
         # >  If you do not set this parameter, ClientToken is set to the value of RequestId. The value of RequestId for each API request may be different.
         self.client_token = client_token  # type: str
-        # Specifies whether to perform a dry run. Default values:
+        # Specifies whether to perform a dry run to check information such as the permissions and the instance status. Valid values:
         # 
         # *   **false** (default): performs a dry run and sends the request.
         # *   **true**: performs a dry run. The system checks the required parameters and request syntax. If the request fails the dry run, an error message is returned. If the request passes the dry run, the `DryRunOperation` error code is returned.
         self.dry_run = dry_run  # type: bool
         self.owner_account = owner_account  # type: str
         self.owner_id = owner_id  # type: long
         # The ID of the region where the VPC is deployed.
@@ -5705,27 +5702,27 @@
         self.tag = tag  # type: list[CreateTransitRouterVpcAttachmentRequestTag]
         # The description of the VPC connection.
         # 
         # The description must be 2 to 256 characters in length. The description must start with a letter but cannot start with `http://` or `https://`.
         self.transit_router_attachment_description = transit_router_attachment_description  # type: str
         # The name of the VPC connection.
         # 
-        # The name must be 2 to 128 characters in length, and can contain letters, digits, underscores (\_), and hyphens (-). It must start with a letter.
+        # The name must be 2 to 128 characters in length, and can contain digits, underscores (\_), and hyphens (-). It must start with a letter.
         self.transit_router_attachment_name = transit_router_attachment_name  # type: str
         # The ID of the Enterprise Edition transit router.
         self.transit_router_id = transit_router_id  # type: str
         # The ID of the VPC.
         self.vpc_id = vpc_id  # type: str
         # The ID of the Alibaba Cloud account to which the VPC belongs. The default value is the ID of the current Alibaba Cloud account.
         # 
         # > If the network instance and CEN instance belong to different Alibaba Cloud accounts, this parameter is required.
         self.vpc_owner_id = vpc_owner_id  # type: long
-        # A zone that supports Enterprise Edition transit routers.
+        # A vSwitch in a zone of the Enterprise Edition transit router.
         # 
-        # You can specify at most 10 zones.
+        # You can specify at most 10 vSwitches in each call.
         self.zone_mappings = zone_mappings  # type: list[CreateTransitRouterVpcAttachmentRequestZoneMappings]
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
                     k.validate()
@@ -5891,15 +5888,15 @@
         return self
 
 
 class CreateTransitRouterVpnAttachmentRequestTag(TeaModel):
     def __init__(self, key=None, value=None):
         # The tag key.
         # 
-        # The tag key cannot be an empty string. The tag key can be up to 64 characters in length, and cannot start with `acs:` or `aliyun`. It cannot contain `http://` or `https://`.
+        # The tag key cannot be an empty string. The tag key can be up to 64 characters in length and cannot start with `acs:` or `aliyun`. It cannot contain `http://` or `https://`.
         # 
         # You can specify at most 20 tag keys.
         self.key = key  # type: str
         # The tag value.
         # 
         # The tag value can be 0 to 128 characters in length, and cannot start with `aliyun` or `acs:`. It cannot contain `http://` or `https://`.
         # 
@@ -5928,15 +5925,15 @@
         if m.get('Value') is not None:
             self.value = m.get('Value')
         return self
 
 
 class CreateTransitRouterVpnAttachmentRequestZone(TeaModel):
     def __init__(self, zone_id=None):
-        # The ID of the zone.
+        # The ID of the zone in which you want to create the instance.
         # 
         # You can call the [ListTransitRouterAvailableResource](~~261356~~) operation to query the most recent zone list.
         self.zone_id = zone_id  # type: str
 
     def validate(self):
         pass
 
@@ -5960,26 +5957,26 @@
 class CreateTransitRouterVpnAttachmentRequest(TeaModel):
     def __init__(self, auto_publish_route_enabled=None, cen_id=None, charge_type=None, client_token=None,
                  dry_run=None, owner_account=None, owner_id=None, region_id=None, resource_owner_account=None,
                  resource_owner_id=None, tag=None, transit_router_attachment_description=None, transit_router_attachment_name=None,
                  transit_router_id=None, vpn_id=None, vpn_owner_id=None, zone=None):
         # Specifies whether to allow the transit router to automatically advertise routes to the IPsec-VPN connection. Valid values:
         # 
-        # *   **true** (default): yes
-        # *   **false**: no
+        # *   **true** (default): yes.
+        # *   **false**: no.
         self.auto_publish_route_enabled = auto_publish_route_enabled  # type: bool
-        # The ID of the CEN instance.
+        # The ID of the Cloud Enterprise Network (CEN) instance.
         self.cen_id = cen_id  # type: str
         # The billing method.
         # 
         # Set the value to **POSTPAY**, which is the default value and specifies the pay-as-you-go billing method.
         self.charge_type = charge_type  # type: str
         # The client token that is used to ensure the idempotence of the request.
         # 
-        # You can use the client to generate the value, but you must make sure that it is unique among all requests. The ClientToken value contain only ASCII characters.
+        # You can use the client to generate the token, but you must make sure that the token is unique among different requests. The client token can contain only ASCII characters.
         # 
         # >  If you do not set this parameter, **ClientToken** is set to the value of **RequestId**. The value of **RequestId** for each API request may be different.
         self.client_token = client_token  # type: str
         # Specifies whether to perform a dry run. Valid values:
         # 
         # *   **true**: performs a dry run. The system checks the required parameters, request syntax, and limits. If the request fails the dry run, an error message is returned. If the request passes the dry run, the `DryRunOperation` error code is returned.
         # *   **false** (default): performs a dry run and sends the request.
@@ -5988,15 +5985,15 @@
         self.owner_id = owner_id  # type: long
         # The ID of the region where the transit router is deployed.
         # 
         # You can call the [DescribeChildInstanceRegions](~~132080~~) operation to query the most recent region list.
         self.region_id = region_id  # type: str
         self.resource_owner_account = resource_owner_account  # type: str
         self.resource_owner_id = resource_owner_id  # type: long
-        # The information about the tags.
+        # A list of tags.
         # 
         # You can specify at most 20 tags in each call.
         self.tag = tag  # type: list[CreateTransitRouterVpnAttachmentRequestTag]
         # The description of the VPN attachment.
         # 
         # The description must be 2 to 256 characters in length. The description must start with a letter but cannot start with `http://` or `https://`.
         self.transit_router_attachment_description = transit_router_attachment_description  # type: str
@@ -6009,15 +6006,15 @@
         # The ID of the IPsec-VPN connection.
         self.vpn_id = vpn_id  # type: str
         # The ID of the Alibaba Cloud account to which the IPsec-VPN connection belongs.
         # 
         # *   If you do not set this parameter, the ID of the current Alibaba Cloud account is used.
         # *   You must set VpnOwnerId if you want to connect the transit router to an IPsec-VPN connection that belongs to another Alibaba Cloud account.
         self.vpn_owner_id = vpn_owner_id  # type: long
-        # The ID of the zone in the current region.
+        # The ID of a zone in the current region.
         # 
         # Resources are deployed in the specified zone.
         self.zone = zone  # type: list[CreateTransitRouterVpnAttachmentRequestZone]
 
     def validate(self):
         if self.tag:
             for k in self.tag:
@@ -10601,36 +10598,37 @@
         self.cen_id = cen_id  # type: str
         # The ID of the network instance.
         self.child_instance_id = child_instance_id  # type: str
         # The ID of the region where the network instance is deployed.
         # 
         # You can call the [DescribeChildInstanceRegions](~~132080~~) operation to query the most recent region list.
         self.child_instance_region_id = child_instance_region_id  # type: str
+        # The ID of the route table of the network instance.
         self.child_instance_route_table_id = child_instance_route_table_id  # type: str
         # The type of the network instance. Valid values:
         # 
-        # *   **VPC**\
-        # *   **VBR**\
-        # *   **CCN**\
+        # *   **VPC**: virtual private cloud (VPC)
+        # *   **VBR**: virtual border router (VBR)
+        # *   **CCN**: Cloud Connect Network (CCN) instance
         self.child_instance_type = child_instance_type  # type: str
         self.owner_account = owner_account  # type: str
         self.owner_id = owner_id  # type: long
         # The number of the page to return. Default value: **1**.
         self.page_number = page_number  # type: int
         # The number of entries to return on each page. Default value: **10**. Valid values: **1** to **50**.
         self.page_size = page_size  # type: int
         self.resource_owner_account = resource_owner_account  # type: str
         self.resource_owner_id = resource_owner_id  # type: long
-        # The status of the routes that you want to query. Valid values:
+        # The status of the route. Valid values:
         # 
-        # *   **Active**: active routes
-        # *   **Candidate**: standby routes
-        # *   **Rejected**: rejected routes
-        # *   **Prohibited**: prohibited routes
-        # *   **All** (default value): all routes
+        # *   **Active**: available
+        # *   **Candidate**: standby
+        # *   **Rejected**: rejected
+        # *   **Prohibited**: prohibited
+        # *   **All** (default): all routes
         self.status = status  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeCenChildInstanceRouteEntriesRequest, self).to_map()
@@ -10715,17 +10713,17 @@
         if m.get('AsPath') is not None:
             self.as_path = m.get('AsPath')
         return self
 
 
 class DescribeCenChildInstanceRouteEntriesResponseBodyCenRouteEntriesCenRouteEntryCenRouteMapRecordsCenRouteMapRecord(TeaModel):
     def __init__(self, region_id=None, route_map_id=None):
-        # The ID of the region where the route map is applied.
+        # The ID of the region in which the routing policy is applied.
         self.region_id = region_id  # type: str
-        # The ID of the route map.
+        # The ID of the routing policy.
         self.route_map_id = route_map_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeCenChildInstanceRouteEntriesResponseBodyCenRouteEntriesCenRouteEntryCenRouteMapRecordsCenRouteMapRecord, self).to_map()
@@ -10803,30 +10801,30 @@
             self.community = m.get('Community')
         return self
 
 
 class DescribeCenChildInstanceRouteEntriesResponseBodyCenRouteEntriesCenRouteEntryConflictsConflict(TeaModel):
     def __init__(self, destination_cidr_block=None, instance_id=None, instance_type=None, region_id=None,
                  status=None):
-        # The destination CIDR block of the conflicting route.
+        # The destination CIDR block of the overlapping route.
         self.destination_cidr_block = destination_cidr_block  # type: str
-        # The ID of the peer network instance on which conflicting routes are found.
+        # The ID of the peer network instance on which the overlapping routes are found.
         self.instance_id = instance_id  # type: str
-        # The type of the peer network instance on which conflicting routes are found. 
+        # The type of the peer network instance on which the overlapping routes are found. Valid values: Valid values:
         # 
-        # - **VPC**\
-        # - **VBR**\
-        # - **CCN**\
+        # *   **VPC**: VPC
+        # *   **VBR**: VBR
+        # *   **CCN**: CCN instance
         self.instance_type = instance_type  # type: str
-        # The ID of the region where the peer network instance on which conflicting routes are found is deployed.
+        # The ID of the region where the peer network instance on which the overlapping routes are found is deployed.
         self.region_id = region_id  # type: str
-        # The cause of the route error. Valid values: 
+        # The cause of the route error. Valid values:
         # 
-        # - **conflict**: Two routes have the same destination CIDR block.
-        # - **overflow**: The number of routes in the route table configured on another network instance reached the upper limit.
+        # *   **conflict**: The routes have the same destination CIDR block.
+        # *   **overflow**: The number of routes in the route table configured on another network instance has reached the upper limit.
         self.status = status  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeCenChildInstanceRouteEntriesResponseBodyCenRouteEntriesCenRouteEntryConflictsConflict, self).to_map()
@@ -10893,76 +10891,76 @@
         return self
 
 
 class DescribeCenChildInstanceRouteEntriesResponseBodyCenRouteEntriesCenRouteEntry(TeaModel):
     def __init__(self, as_paths=None, cen_route_map_records=None, communities=None, conflicts=None,
                  destination_cidr_block=None, next_hop_instance_id=None, next_hop_region_id=None, next_hop_type=None,
                  operational_mode=None, publish_status=None, route_table_id=None, status=None, type=None):
-        # The AS paths of the routes.
+        # The autonomous system (AS) paths of the routes.
         self.as_paths = as_paths  # type: DescribeCenChildInstanceRouteEntriesResponseBodyCenRouteEntriesCenRouteEntryAsPaths
-        # The route maps that the routes match.
+        # The routing policy that the routes match.
         self.cen_route_map_records = cen_route_map_records  # type: DescribeCenChildInstanceRouteEntriesResponseBodyCenRouteEntriesCenRouteEntryCenRouteMapRecords
-        # The community attributes of the routes.
+        # The community attributes of the route entry.
         self.communities = communities  # type: DescribeCenChildInstanceRouteEntriesResponseBodyCenRouteEntriesCenRouteEntryCommunities
-        # The array of conflicting routes.
+        # A list of overlapping routes.
         self.conflicts = conflicts  # type: DescribeCenChildInstanceRouteEntriesResponseBodyCenRouteEntriesCenRouteEntryConflicts
         # The destination CIDR block of the route.
         self.destination_cidr_block = destination_cidr_block  # type: str
         # The ID of the instance specified as the next hop in the route.
         self.next_hop_instance_id = next_hop_instance_id  # type: str
         # The ID of the region where the instance specified as the next hop in the route belongs.
         self.next_hop_region_id = next_hop_region_id  # type: str
-        # The type of the instance specified as the next hop in the route. 
+        # The type of the instance specified as the next hop in the route. Valid values:
         # 
-        # - **Instance**: ECS instance
-        # - **HaVip**: HAVIP
-        # - **RouterInterface**: router interface
-        # - **NetworkInterface**: ENI
-        # - **VpnGateway**: VPN gateway
-        # - **IPv6Gateway**: IPv6 gateway
-        # - **NatGateway**: NAT gateway
-        # - **Attachment**: network instance connection
-        # - **service**: cloud service
-        # - **VBR**: virtual border router
-        # - **CCN**: CCN instance
-        # - **VPC**: virtual private cloud
-        # - **local**: system route. No next hop is specified.
-        # - **TR**: transit router
-        # - **BlackHole**: blackhole route. No next hop is specified.
-        # - **EcRouterInterface**: router interface for Express Connect
-        # - **HealthCheck**: health check
-        # - **AS**: access gateway for CCN
-        # - **classic**: classic network-type instance
-        # - **GatewayEndpoint**: gateway endpoint
-        # - **CPE**: data center connected by VBRs
+        # *   **Instance**: Elastic Compute Service (ECS) instance.
+        # *   **HaVip**: high-availability virtual IP address (HAVIP).
+        # *   **RouterInterface**: router interface.
+        # *   **NetworkInterface**: elastic network interface (ENI).
+        # *   **VpnGateway**: VPN gateway.
+        # *   **IPv6Gateway**: IPv6 gateway.
+        # *   **NatGateway**: NAT gateway.
+        # *   **Attachment**: network instance connection.
+        # *   **service**: cloud service.
+        # *   **VBR**: VBR.
+        # *   **CCN**: CCN instance.
+        # *   **VPC**: VPC.
+        # *   **local**: system route. No next hop is specified.
+        # *   **TR**: transit router.
+        # *   \*\*BlackHole\*\*: blackhole route. No next hop is specified.
+        # *   \*\*EcRouterInterface\*\*: router interface for Express Connect
+        # *   **HealthCheck**: health check.
+        # *   **AS**: access gateway for CCN.
+        # *   **classicLink**: classic network-type instance.
+        # *   **GatewayEndpoint**: gateway endpoint.
+        # *   **CPE**: data center connected to the VBR.
         self.next_hop_type = next_hop_type  # type: str
-        # Indicates whether the route is allowed to be advertised to or withdrawn from the CEN instance. Valid values:  
+        # Indicates whether the route is allowed to be advertised to or withdrawn from the CEN instance. Valid values:
         # 
-        # - **true**: The route is allowed to be advertised to or withdrawn from the CEN instance.
-        # - **false**: The route is not allowed to be advertised to or withdrawn from the CEN instance.
+        # *   **true**: The route is allowed to be advertised to or withdrawn from the CEN instance.
+        # *   **false**: The route is not allowed to be advertised to or withdrawn from the CEN instance.
         self.operational_mode = operational_mode  # type: bool
-        # Indicates whether the route is advertised to the CEN instance. Valid values: 
+        # Indicates whether the route is advertised to the CEN instance. Valid values: Valid values:
         # 
-        # - **Published**: The route is advertised to the CEN instance.
-        # - **NonPublished**: The route is not advertised to the CEN instance.
+        # *   **Published**: The route is advertised to the CEN instance.
+        # *   **NonPublished**: The route is not advertised to the CEN instance.
         self.publish_status = publish_status  # type: str
         # The ID of the route table.
         self.route_table_id = route_table_id  # type: str
-        # The status of the route. Valid values: 
+        # The status of the route. Valid values:
         # 
-        # - **Active**: The route is active.
-        # - **Candidate**: The route is a standby route.
-        # - **Rejected**: The route is rejected.
-        # - **Prohibited**: The route is prohibited.
+        # *   **Active**: available
+        # *   **Candidate**: standby
+        # *   **Rejected**: rejected
+        # *   **Prohibited**: prohibited
         self.status = status  # type: str
-        # The type of the route. Valid values: 
+        # The type of the route. Valid values: Valid values:
         # 
-        # - **CEN**: route that is advertised through CEN
-        # - **System**: system route
-        # - **Custom**: custom route
+        # *   **CEN**: advertised by CEN
+        # *   **System**: system route
+        # *   **Custom**: custom route
         self.type = type  # type: str
 
     def validate(self):
         if self.as_paths:
             self.as_paths.validate()
         if self.cen_route_map_records:
             self.cen_route_map_records.validate()
@@ -11070,15 +11068,15 @@
                 temp_model = DescribeCenChildInstanceRouteEntriesResponseBodyCenRouteEntriesCenRouteEntry()
                 self.cen_route_entry.append(temp_model.from_map(k))
         return self
 
 
 class DescribeCenChildInstanceRouteEntriesResponseBody(TeaModel):
     def __init__(self, cen_route_entries=None, page_number=None, page_size=None, request_id=None, total_count=None):
-        # The array of routes.
+        # The information about the routes.
         self.cen_route_entries = cen_route_entries  # type: DescribeCenChildInstanceRouteEntriesResponseBodyCenRouteEntries
         # The page number of the returned page.
         self.page_number = page_number  # type: int
         # The number of entries returned per page.
         self.page_size = page_size  # type: int
         # The ID of the request.
         self.request_id = request_id  # type: str
@@ -16525,20 +16523,20 @@
             self.transit_route_table_aggregation_cidr = m.get('TransitRouteTableAggregationCidr')
         if m.get('TransitRouteTableId') is not None:
             self.transit_route_table_id = m.get('TransitRouteTableId')
         return self
 
 
 class DescribeTransitRouteTableAggregationResponseBodyData(TeaModel):
-    def __init__(self, description=None, name=None, route_type=None, scop=None, status=None, tr_route_table_id=None,
+    def __init__(self, description=None, name=None, route_type=None, scope=None, status=None, tr_route_table_id=None,
                  transit_route_table_aggregation_cidr=None):
         self.description = description  # type: str
         self.name = name  # type: str
         self.route_type = route_type  # type: str
-        self.scop = scop  # type: str
+        self.scope = scope  # type: str
         self.status = status  # type: str
         self.tr_route_table_id = tr_route_table_id  # type: str
         self.transit_route_table_aggregation_cidr = transit_route_table_aggregation_cidr  # type: str
 
     def validate(self):
         pass
 
@@ -16550,16 +16548,16 @@
         result = dict()
         if self.description is not None:
             result['Description'] = self.description
         if self.name is not None:
             result['Name'] = self.name
         if self.route_type is not None:
             result['RouteType'] = self.route_type
-        if self.scop is not None:
-            result['Scop'] = self.scop
+        if self.scope is not None:
+            result['Scope'] = self.scope
         if self.status is not None:
             result['Status'] = self.status
         if self.tr_route_table_id is not None:
             result['TrRouteTableId'] = self.tr_route_table_id
         if self.transit_route_table_aggregation_cidr is not None:
             result['TransitRouteTableAggregationCidr'] = self.transit_route_table_aggregation_cidr
         return result
@@ -16568,16 +16566,16 @@
         m = m or dict()
         if m.get('Description') is not None:
             self.description = m.get('Description')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('RouteType') is not None:
             self.route_type = m.get('RouteType')
-        if m.get('Scop') is not None:
-            self.scop = m.get('Scop')
+        if m.get('Scope') is not None:
+            self.scope = m.get('Scope')
         if m.get('Status') is not None:
             self.status = m.get('Status')
         if m.get('TrRouteTableId') is not None:
             self.tr_route_table_id = m.get('TrRouteTableId')
         if m.get('TransitRouteTableAggregationCidr') is not None:
             self.transit_route_table_aggregation_cidr = m.get('TransitRouteTableAggregationCidr')
         return self
@@ -22189,15 +22187,15 @@
 
 class ListTransitRouterPrefixListAssociationRequest(TeaModel):
     def __init__(self, next_hop=None, next_hop_instance_id=None, next_hop_type=None, owner_account=None,
                  owner_id=None, owner_uid=None, page_number=None, page_size=None, prefix_list_id=None, region_id=None,
                  resource_owner_account=None, resource_owner_id=None, status=None, transit_router_id=None, transit_router_table_id=None):
         # The ID of the next hop.
         # 
-        # >  Enter **BlackHole** if you want to query the prefix list that generates blackhole routes.
+        # > Set the value to **BlackHole** if you want to query the prefix list that generates blackhole routes.
         self.next_hop = next_hop  # type: str
         self.next_hop_instance_id = next_hop_instance_id  # type: str
         # The type of the next hop. Valid values:
         # 
         # *   **BlackHole**: The prefix list that generates blackhole routes.
         # *   **VPC**: The prefix list whose next hop is a virtual private cloud (VPC) connection.
         # *   **VBR**: The prefix list whose next hop is a virtual border router (VBR) connection.
@@ -22302,19 +22300,19 @@
 
 
 class ListTransitRouterPrefixListAssociationResponseBodyPrefixLists(TeaModel):
     def __init__(self, next_hop=None, next_hop_instance_id=None, next_hop_type=None, owner_uid=None,
                  prefix_list_id=None, status=None, transit_router_id=None, transit_router_table_id=None):
         # The ID of the next hop.
         # 
-        # >  If the value is **BlackHole**, all the CIDR blocks in the prefix list are blackhole routes. Packets destined for the CIDR blocks are dropped.
+        # > A value of **BlackHole** indicates that all the CIDR blocks in the prefix list are blackhole routes. Packets destined for the CIDR blocks are dropped.
         self.next_hop = next_hop  # type: str
         # The ID of the network instance associated with the next hop connection.
         self.next_hop_instance_id = next_hop_instance_id  # type: str
-        # The type of the next hop.
+        # The type of the next hop. Valid values:
         # 
         # *   **BlackHole**: All the CIDR blocks in the prefix list are blackhole routes. Packets destined for the CIDR blocks are dropped.
         # *   **VPC**: The next hop of the CIDR blocks in the prefix list is a VPC connection.
         # *   **VBR**: The next hop of the CIDR blocks in the prefix list is a VBR connection.
         # *   **TR**: The next hop of the CIDR blocks in the prefix list is an inter-region connection.
         self.next_hop_type = next_hop_type  # type: str
         # The ID of the Alibaba Cloud account to which the prefix list belongs.
@@ -22381,19 +22379,19 @@
 
 class ListTransitRouterPrefixListAssociationResponseBody(TeaModel):
     def __init__(self, page_number=None, page_size=None, prefix_lists=None, request_id=None, total_count=None):
         # The page number of the returned page.
         self.page_number = page_number  # type: int
         # The number of entries returned per page.
         self.page_size = page_size  # type: int
-        # The information about the prefix list.
+        # A list of prefix lists.
         self.prefix_lists = prefix_lists  # type: list[ListTransitRouterPrefixListAssociationResponseBodyPrefixLists]
         # The ID of the request.
         self.request_id = request_id  # type: str
-        # The number of entries returned.
+        # The total number of entries returned.
         self.total_count = total_count  # type: int
 
     def validate(self):
         if self.prefix_lists:
             for k in self.prefix_lists:
                 if k:
                     k.validate()
@@ -23407,16 +23405,16 @@
         return self
 
 
 class ListTransitRouterRouteTablesRequestRouteTableOptions(TeaModel):
     def __init__(self, multi_region_ecmp=None):
         # Specifies whether to enable equal-cost multi-path (ECMP) routing. Valid values:
         # 
-        # *   **disable**: no If you disable ECMP routing, routes that are learned from different regions but have the same prefix and attributes select the transit route with the smallest region ID as the next hop. Region IDs are sorted in alphabetic order. The network latency and bandwidth consumption also vary based on the region. Proceed with caution.
-        # *   **enable**: yes If you enable ECMP routing, routes that are learned from different regions but have the same prefix and attributes form an ECMP route. The network latency and bandwidth consumption also vary based on the region. Proceed with caution.
+        # *   **disable**: disables ECMP routing If you disable ECMP routing, routes that are learned from different regions but have the same prefix and attributes select the transit router with the smallest region ID as the next hop. Region IDs are sorted in alphabetic order. The network latency and bandwidth consumption also vary based on the region. Proceed with caution.
+        # *   **enable**: enables ECMP routing. If you enable ECMP routing, routes that are learned from different regions but have the same prefix and attributes form an ECMP route. The network latency and bandwidth consumption also vary based on the region. Proceed with caution.
         self.multi_region_ecmp = multi_region_ecmp  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListTransitRouterRouteTablesRequestRouteTableOptions, self).to_map()
@@ -23435,15 +23433,15 @@
         return self
 
 
 class ListTransitRouterRouteTablesRequestTag(TeaModel):
     def __init__(self, key=None, value=None):
         # The tag key.
         # 
-        # The tag key cannot be an empty string. The tag key can be up to 64 characters in length, and cannot start with `acs:` or `aliyun`. It cannot contain `http://` or `https://`.
+        # The tag key cannot be an empty string. The tag key can be up to 64 characters in length and cannot start with `acs:` or `aliyun`. It cannot contain `http://` or `https://`.
         # 
         # You can specify at most 20 tag keys.
         self.key = key  # type: str
         # The tag value.
         # 
         # The tag value can be 0 to 128 characters in length, and cannot start with `aliyun` or `acs:`. It cannot contain `http://` or `https://`.
         # 
@@ -23477,18 +23475,18 @@
 class ListTransitRouterRouteTablesRequest(TeaModel):
     def __init__(self, max_results=None, next_token=None, owner_account=None, owner_id=None,
                  resource_owner_account=None, resource_owner_id=None, route_table_options=None, tag=None, transit_router_id=None,
                  transit_router_route_table_ids=None, transit_router_route_table_names=None, transit_router_route_table_status=None,
                  transit_router_route_table_type=None):
         # The number of entries to return on each page. Valid values: **1** to **100**. Default value: **20**.
         self.max_results = max_results  # type: int
-        # The token that determines the start point of the next query. Valid values:
+        # The token that determines the start point of the query. Valid values:
         # 
         # *   If this is your first query or no subsequent query is to be sent, ignore this parameter.
-        # *   If a next query is to be sent, set the value to the value of **NextToken** that is returned from the last call.
+        # *   If a subsequent query is to be sent, set the value to the value of **NextToken** that is returned from the last call.
         self.next_token = next_token  # type: str
         self.owner_account = owner_account  # type: str
         self.owner_id = owner_id  # type: long
         self.resource_owner_account = resource_owner_account  # type: str
         self.resource_owner_id = resource_owner_id  # type: long
         # The features of the route table.
         self.route_table_options = route_table_options  # type: ListTransitRouterRouteTablesRequestRouteTableOptions
@@ -23506,22 +23504,22 @@
         # 
         # You can query multiple route tables in each call. Maximum value of **N**: **20**.
         # 
         # > If you set both **TransitRouterRouteTableNames.N** and **TransitRouterRouteTableIds.N**, make sure that the specified name and ID belong to the same route table.
         self.transit_router_route_table_names = transit_router_route_table_names  # type: list[str]
         # The status of the route table. Valid values:
         # 
-        # *   **Creating**: being created
-        # *   **Deleting**: being deleted
-        # *   **Active**: available
+        # *   **Creating**: The route table is being created.
+        # *   **Deleting**: The route table is being deleted.
+        # *   **Active**: The route table is available.
         self.transit_router_route_table_status = transit_router_route_table_status  # type: str
         # The type of the route table. Valid values:
         # 
         # *   **Custom**: a custom route table
-        # *   **System**: the default system route table
+        # *   **System**: the default route table
         self.transit_router_route_table_type = transit_router_route_table_type  # type: str
 
     def validate(self):
         if self.route_table_options:
             self.route_table_options.validate()
         if self.tag:
             for k in self.tag:
@@ -23599,16 +23597,16 @@
         return self
 
 
 class ListTransitRouterRouteTablesResponseBodyTransitRouterRouteTablesRouteTableOptions(TeaModel):
     def __init__(self, multi_region_ecmp=None):
         # Indicates whether ECMP routing is enabled. Valid values:
         # 
-        # *   **disable**: disabled If you disable ECMP routing, routes that are learned from different regions but have the same prefix and attributes select the transit route with the smallest region ID as the next hop. Region IDs are sorted in alphabetic order. The network latency and bandwidth consumption also vary based on the region. Proceed with caution.
-        # *   **enable**: enables ECMP routing. If you enable ECMP routing, routes that are learned from different regions but have the same prefix and attributes form an ECMP route. The network latency and bandwidth consumption also vary based on the region. Proceed with caution.
+        # *   **disable**: ECMP routing is disabled. If ECMP routing is disabled, routes that are learned from different regions but have the same prefix and attributes select the transit router with the smallest region ID as the next hop. Region IDs are sorted in alphabetic order. The network latency and bandwidth consumption also vary based on the region. Proceed with caution.
+        # *   **enable**: ECMP routing is enabled. If ECMP routing is enabled, routes that are learned from different regions but have the same prefix and attributes form an ECMP route. The network latency and bandwidth consumption also vary based on the region. Proceed with caution.
         self.multi_region_ecmp = multi_region_ecmp  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListTransitRouterRouteTablesResponseBodyTransitRouterRouteTablesRouteTableOptions, self).to_map()
@@ -23666,33 +23664,33 @@
         # 
         # The time follows the ISO8601 standard in the YYYY-MM-DDThh:mmZ format. The time is displayed in UTC.
         self.create_time = create_time  # type: str
         # The ID of the region where the Enterprise Edition transit router is deployed.
         self.region_id = region_id  # type: str
         # The features of the route table.
         self.route_table_options = route_table_options  # type: ListTransitRouterRouteTablesResponseBodyTransitRouterRouteTablesRouteTableOptions
-        # The tags.
+        # A list of tags.
         self.tags = tags  # type: list[ListTransitRouterRouteTablesResponseBodyTransitRouterRouteTablesTags]
         self.transit_router_id = transit_router_id  # type: str
         # The description of the route table.
         self.transit_router_route_table_description = transit_router_route_table_description  # type: str
         # The ID of the route table.
         self.transit_router_route_table_id = transit_router_route_table_id  # type: str
         # The name of the route table.
         self.transit_router_route_table_name = transit_router_route_table_name  # type: str
         # The status of the route table. Valid values:
         # 
-        # *   **Creating**: being created
-        # *   **Deleting**: being deleted
-        # *   **Active**: available
+        # *   **Creating**: The route table is being created.
+        # *   **Deleting**: The route table is being deleted.
+        # *   **Active**: The route table is available.
         self.transit_router_route_table_status = transit_router_route_table_status  # type: str
         # The type of the route table. Valid value:
         # 
         # *   **Custom**: a custom route table
-        # *   **System**: the default system route table
+        # *   **System**: the default route table
         self.transit_router_route_table_type = transit_router_route_table_type  # type: str
 
     def validate(self):
         if self.route_table_options:
             self.route_table_options.validate()
         if self.tags:
             for k in self.tags:
@@ -23757,20 +23755,20 @@
             self.transit_router_route_table_type = m.get('TransitRouterRouteTableType')
         return self
 
 
 class ListTransitRouterRouteTablesResponseBody(TeaModel):
     def __init__(self, max_results=None, next_token=None, request_id=None, total_count=None,
                  transit_router_route_tables=None):
-        # The number of entries returned on each page.
+        # The number of entries returned per page.
         self.max_results = max_results  # type: int
         # The token that determines the start point of the next query. Valid values:
         # 
-        # *   If **NextToken** was not returned, it indicates that no additional results exist.
         # *   If **NextToken** was returned in the previous query, specify the value to obtain the next set of results.
+        # *   If a value of **NextToken** is not returned, it indicates that no additional results exist.
         self.next_token = next_token  # type: str
         # The ID of the request.
         self.request_id = request_id  # type: str
         # The total number of entries returned.
         self.total_count = total_count  # type: int
         # A list of route tables.
         self.transit_router_route_tables = transit_router_route_tables  # type: list[ListTransitRouterRouteTablesResponseBodyTransitRouterRouteTables]
```

### Comparing `alibabacloud_cbn20170912_py2-1.0.8/alibabacloud_cbn20170912_py2.egg-info/PKG-INFO` & `alibabacloud_cbn20170912_py2-1.0.9/alibabacloud_cbn20170912_py2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-cbn20170912-py2
-Version: 1.0.8
+Version: 1.0.9
 Summary: Alibaba Cloud Cloud Enterprise Network (20170912) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cbn20170912_py2-1.0.8/setup.py` & `alibabacloud_cbn20170912_py2-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_cbn20170912_py2.
 
-Created on 13/03/2023
+Created on 17/03/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_cbn20170912"
 NAME = "alibabacloud_cbn20170912_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Cloud Enterprise Network (20170912) SDK Library for Python2"
```

