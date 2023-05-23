# Comparing `tmp/odoo_addons_oca_stock_logistics_workflow-16.0.20230514.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_stock_logistics_workflow-16.0.20230522.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1765 bytes, number of entries: 4
--rw-r--r--  2.0 unx     2244 b- defN 23-May-15 07:36 odoo_addons_oca_stock_logistics_workflow-16.0.20230514.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-15 07:36 odoo_addons_oca_stock_logistics_workflow-16.0.20230514.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-May-15 07:36 odoo_addons_oca_stock_logistics_workflow-16.0.20230514.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      469 b- defN 23-May-15 07:36 odoo_addons_oca_stock_logistics_workflow-16.0.20230514.0.dist-info/RECORD
-4 files, 2806 bytes uncompressed, 839 bytes compressed:  70.1%
+Zip file size: 1776 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     2318 b- defN 23-May-23 05:24 odoo_addons_oca_stock_logistics_workflow-16.0.20230522.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-23 05:24 odoo_addons_oca_stock_logistics_workflow-16.0.20230522.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-May-23 05:24 odoo_addons_oca_stock_logistics_workflow-16.0.20230522.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      469 b- defN 23-May-23 05:24 odoo_addons_oca_stock_logistics_workflow-16.0.20230522.0.dist-info/RECORD
+4 files, 2880 bytes uncompressed, 850 bytes compressed:  70.5%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_stock_logistics_workflow-16.0.20230514.0.dist-info/METADATA
+Filename: odoo_addons_oca_stock_logistics_workflow-16.0.20230522.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_stock_logistics_workflow-16.0.20230514.0.dist-info/WHEEL
+Filename: odoo_addons_oca_stock_logistics_workflow-16.0.20230522.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_stock_logistics_workflow-16.0.20230514.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_stock_logistics_workflow-16.0.20230522.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_stock_logistics_workflow-16.0.20230514.0.dist-info/RECORD
+Filename: odoo_addons_oca_stock_logistics_workflow-16.0.20230522.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_stock_logistics_workflow-16.0.20230514.0.dist-info/METADATA` & `odoo_addons_oca_stock_logistics_workflow-16.0.20230522.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-stock-logistics-workflow
-Version: 16.0.20230514.0
+Version: 16.0.20230522.0
 Summary: Meta package for oca-stock-logistics-workflow Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
@@ -24,14 +24,15 @@
 Requires-Dist: odoo-addon-stock-picking-group-by-base (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-stock-picking-group-by-max-weight (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-stock-picking-invoice-link (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-stock-picking-purchase-order-link (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-stock-picking-sale-order-link (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-stock-picking-show-return (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-stock-picking-start (<16.1dev,>=16.0dev)
+Requires-Dist: odoo-addon-stock-procurement-customer (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-stock-putaway-hook (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-stock-quant-package-dimension (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-stock-quant-package-product-packaging (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-stock-receipt-lot-info (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-stock-restrict-lot (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-stock-split-picking (<16.1dev,>=16.0dev)
```

