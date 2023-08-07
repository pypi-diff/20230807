# Comparing `tmp/odoo12_addons_oca_pos-12.0.20230418.0-py3-none-any.whl.zip` & `tmp/odoo12_addons_oca_pos-12.0.20230806.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1981 bytes, number of entries: 4
--rw-r--r--  2.0 unx     4145 b- defN 23-Apr-19 05:54 odoo12_addons_oca_pos-12.0.20230418.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-19 05:54 odoo12_addons_oca_pos-12.0.20230418.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-19 05:54 odoo12_addons_oca_pos-12.0.20230418.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      393 b- defN 23-Apr-19 05:54 odoo12_addons_oca_pos-12.0.20230418.0.dist-info/RECORD
-4 files, 4631 bytes uncompressed, 1207 bytes compressed:  73.9%
+Zip file size: 1989 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     4200 b- defN 23-Aug-07 04:37 odoo12_addons_oca_pos-12.0.20230806.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-07 04:37 odoo12_addons_oca_pos-12.0.20230806.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Aug-07 04:37 odoo12_addons_oca_pos-12.0.20230806.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      393 b- defN 23-Aug-07 04:37 odoo12_addons_oca_pos-12.0.20230806.0.dist-info/RECORD
+4 files, 4686 bytes uncompressed, 1215 bytes compressed:  74.1%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo12_addons_oca_pos-12.0.20230418.0.dist-info/METADATA
+Filename: odoo12_addons_oca_pos-12.0.20230806.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo12_addons_oca_pos-12.0.20230418.0.dist-info/WHEEL
+Filename: odoo12_addons_oca_pos-12.0.20230806.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo12_addons_oca_pos-12.0.20230418.0.dist-info/top_level.txt
+Filename: odoo12_addons_oca_pos-12.0.20230806.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo12_addons_oca_pos-12.0.20230418.0.dist-info/RECORD
+Filename: odoo12_addons_oca_pos-12.0.20230806.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo12_addons_oca_pos-12.0.20230418.0.dist-info/METADATA` & `odoo12_addons_oca_pos-12.0.20230806.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo12-addons-oca-pos
-Version: 12.0.20230418.0
+Version: 12.0.20230806.0
 Summary: Meta package for oca-pos Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 12.0
@@ -55,14 +55,15 @@
 Requires-Dist: odoo12-addon-pos-picking-load
 Requires-Dist: odoo12-addon-pos-picking-load-partner-name
 Requires-Dist: odoo12-addon-pos-place
 Requires-Dist: odoo12-addon-pos-prevent-double-closing
 Requires-Dist: odoo12-addon-pos-price-to-weight
 Requires-Dist: odoo12-addon-pos-pricelist-technical
 Requires-Dist: odoo12-addon-pos-product-default-code
+Requires-Dist: odoo12-addon-pos-product-mergeable-line
 Requires-Dist: odoo12-addon-pos-product-sort
 Requires-Dist: odoo12-addon-pos-product-template
 Requires-Dist: odoo12-addon-pos-quick-logout
 Requires-Dist: odoo12-addon-pos-receipt-xml-header-footer
 Requires-Dist: odoo12-addon-pos-remove-pos-category
 Requires-Dist: odoo12-addon-pos-report-order-payment
 Requires-Dist: odoo12-addon-pos-report-session-summary
```

