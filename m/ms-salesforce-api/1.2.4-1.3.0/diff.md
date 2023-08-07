# Comparing `tmp/ms_salesforce_api-1.2.4.tar.gz` & `tmp/ms_salesforce_api-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_salesforce_api-1.2.4.tar", max compression
+gzip compressed data, was "ms_salesforce_api-1.3.0.tar", max compression
```

## Comparing `ms_salesforce_api-1.2.4.tar` & `ms_salesforce_api-1.3.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    35149 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/LICENSE
--rw-r--r--   0        0        0     8325 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/README.md
--rw-r--r--   0        0        0        0 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/ms_salesforce_api/__init__.py
--rw-r--r--   0        0        0     1491 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/Auth.py
--rw-r--r--   0        0        0     1244 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/JWTGenerator.py
--rw-r--r--   0        0        0     2926 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py
--rw-r--r--   0        0        0        0 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/__tests__/__init__.py
--rw-r--r--   0        0        0     2749 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/__tests__/test_Auth.py
--rw-r--r--   0        0        0     2205 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py
--rw-r--r--   0        0        0     5168 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py
--rw-r--r--   0        0        0     3541 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/__tests__/__init__.py
--rw-r--r--   0        0        0    15342 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/__tests__/test_Project.py
--rw-r--r--   0        0        0     9629 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/constants.py
--rw-r--r--   0        0        0     3804 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/dto/BillingLineDTO.py
--rw-r--r--   0        0        0    25154 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/dto/OpportunityDTO.py
--rw-r--r--   0        0        0     2166 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/dto/ProjectLineItemDTO.py
--rw-r--r--   0        0        0        0 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/dto/__init__.py
--rw-r--r--   0        0        0    28712 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/export_data/Bigquery.py
--rw-r--r--   0        0        0    12590 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/export_data/CloudSQL.py
--rw-r--r--   0        0        0        0 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/export_data/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/export_data/__tests__/__init__.py
--rw-r--r--   0        0        0    20263 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/export_data/__tests__/test_Bigquery.py
--rw-r--r--   0        0        0    13717 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/export_data/__tests__/test_CloudSQL.py
--rw-r--r--   0        0        0      303 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/helpers.py
--rw-r--r--   0        0        0     1055 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/pyproject.toml
--rw-r--r--   0        0        0     9101 1970-01-01 00:00:00.000000 ms_salesforce_api-1.2.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-07 10:23:50.992955 ms_salesforce_api-1.3.0/LICENSE
+-rw-r--r--   0        0        0     8325 2023-08-07 10:23:50.992955 ms_salesforce_api-1.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-08-07 10:23:50.992955 ms_salesforce_api-1.3.0/ms_salesforce_api/__init__.py
+-rw-r--r--   0        0        0     1491 2023-08-07 10:23:50.992955 ms_salesforce_api-1.3.0/ms_salesforce_api/salesforce/Auth.py
+-rw-r--r--   0        0        0     1244 2023-08-07 10:23:50.992955 ms_salesforce_api-1.3.0/ms_salesforce_api/salesforce/JWTGenerator.py
+-rw-r--r--   0        0        0     2926 2023-08-07 10:23:50.992955 ms_salesforce_api-1.3.0/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py
+-rw-r--r--   0        0        0        0 2023-08-07 10:23:50.992955 ms_salesforce_api-1.3.0/ms_salesforce_api/salesforce/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 10:23:50.992955 ms_salesforce_api-1.3.0/ms_salesforce_api/salesforce/__tests__/__init__.py
+-rw-r--r--   0        0        0     2749 2023-08-07 10:23:50.992955 ms_salesforce_api-1.3.0/ms_salesforce_api/salesforce/__tests__/test_Auth.py
+-rw-r--r--   0        0        0     2205 2023-08-07 10:23:50.992955 ms_salesforce_api-1.3.0/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py
+-rw-r--r--   0        0        0     5168 2023-08-07 10:23:50.992955 ms_salesforce_api-1.3.0/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py
+-rw-r--r--   0        0        0     3718 2023-08-07 10:23:50.992955 ms_salesforce_api-1.3.0/ms_salesforce_api/salesforce/project/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 10:23:50.992955 ms_salesforce_api-1.3.0/ms_salesforce_api/salesforce/project/__tests__/__init__.py
+-rw-r--r--   0        0        0    15342 2023-08-07 10:23:50.992955 ms_salesforce_api-1.3.0/ms_salesforce_api/salesforce/project/__tests__/test_Project.py
+-rw-r--r--   0        0        0     9629 2023-08-07 10:23:50.992955 ms_salesforce_api-1.3.0/ms_salesforce_api/salesforce/project/constants.py
+-rw-r--r--   0        0        0     3967 2023-08-07 10:23:50.996956 ms_salesforce_api-1.3.0/ms_salesforce_api/salesforce/project/dto/BillingLineDTO.py
+-rw-r--r--   0        0        0    25154 2023-08-07 10:23:50.996956 ms_salesforce_api-1.3.0/ms_salesforce_api/salesforce/project/dto/OpportunityDTO.py
+-rw-r--r--   0        0        0     2166 2023-08-07 10:23:50.996956 ms_salesforce_api-1.3.0/ms_salesforce_api/salesforce/project/dto/ProjectLineItemDTO.py
+-rw-r--r--   0        0        0        0 2023-08-07 10:23:50.996956 ms_salesforce_api-1.3.0/ms_salesforce_api/salesforce/project/dto/__init__.py
+-rw-r--r--   0        0        0    29327 2023-08-07 10:23:50.996956 ms_salesforce_api-1.3.0/ms_salesforce_api/salesforce/project/export_data/Bigquery.py
+-rw-r--r--   0        0        0    12590 2023-08-07 10:23:50.996956 ms_salesforce_api-1.3.0/ms_salesforce_api/salesforce/project/export_data/CloudSQL.py
+-rw-r--r--   0        0        0        0 2023-08-07 10:23:50.996956 ms_salesforce_api-1.3.0/ms_salesforce_api/salesforce/project/export_data/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 10:23:50.996956 ms_salesforce_api-1.3.0/ms_salesforce_api/salesforce/project/export_data/__tests__/__init__.py
+-rw-r--r--   0        0        0    20688 2023-08-07 10:23:50.996956 ms_salesforce_api-1.3.0/ms_salesforce_api/salesforce/project/export_data/__tests__/test_Bigquery.py
+-rw-r--r--   0        0        0    13717 2023-08-07 10:23:50.996956 ms_salesforce_api-1.3.0/ms_salesforce_api/salesforce/project/export_data/__tests__/test_CloudSQL.py
+-rw-r--r--   0        0        0      303 2023-08-07 10:23:50.996956 ms_salesforce_api-1.3.0/ms_salesforce_api/salesforce/project/helpers.py
+-rw-r--r--   0        0        0     1055 2023-08-07 10:23:50.996956 ms_salesforce_api-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     9101 1970-01-01 00:00:00.000000 ms_salesforce_api-1.3.0/PKG-INFO
```

### Comparing `ms_salesforce_api-1.2.4/LICENSE` & `ms_salesforce_api-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.2.4/README.md` & `ms_salesforce_api-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/Auth.py` & `ms_salesforce_api-1.3.0/ms_salesforce_api/salesforce/Auth.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/JWTGenerator.py` & `ms_salesforce_api-1.3.0/ms_salesforce_api/salesforce/JWTGenerator.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py` & `ms_salesforce_api-1.3.0/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/__tests__/test_Auth.py` & `ms_salesforce_api-1.3.0/ms_salesforce_api/salesforce/__tests__/test_Auth.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py` & `ms_salesforce_api-1.3.0/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py` & `ms_salesforce_api-1.3.0/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/__init__.py` & `ms_salesforce_api-1.3.0/ms_salesforce_api/salesforce/project/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -72,19 +72,25 @@
                         executor.map(
                             self.fetch_billing_lines,
                             [project_id_batch],
                         )
                     )
                     for billing_line_data in batch_results:
                         for record in billing_line_data:
+                            project_id = record["Project_Line_Item__r"][
+                                "Project__c"
+                            ]
+                            opportunity = opportunities.get(project_id)
+
                             billing_line_dto = (
-                                BillingLineDTO.from_salesforce_record(record)
+                                BillingLineDTO.from_salesforce_record(
+                                    record, opportunity.project_code
+                                )
                             )
-                            project_id = billing_line_dto.project_id
-                            opportunity = opportunities.get(project_id)
+
                             if opportunity is not None:
                                 if not opportunity.billing_lines:
                                     opportunity.billing_lines = []
                                 opportunity.billing_lines.append(
                                     billing_line_dto
                                 )
             opportunities_list = list(opportunities.values())
```

### Comparing `ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/__tests__/test_Project.py` & `ms_salesforce_api-1.3.0/ms_salesforce_api/salesforce/project/__tests__/test_Project.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/constants.py` & `ms_salesforce_api-1.3.0/ms_salesforce_api/salesforce/project/constants.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/dto/BillingLineDTO.py` & `ms_salesforce_api-1.3.0/ms_salesforce_api/salesforce/project/dto/BillingLineDTO.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 class BillingLineDTO:
     def __init__(
         self,
         id,
         name,
         project_id,
+        project_code,
         currency,
         created_date,
         last_modified_date,
         billing_amount,
         billing_date,
         billing_period_ending_date,
         billing_period_starting_date,
@@ -18,14 +19,15 @@
         billing_plan_item,
         billing_plan_service_end_date,
         billing_plan_service_start_date,
     ):
         self.id = id
         self.name = name
         self.project_id = project_id
+        self.project_code = project_code
         self.currency = currency
         self.created_date = created_date
         self.last_modified_date = last_modified_date
         self.billing_amount = billing_amount
         self.billing_date = billing_date
         self.billing_period_ending_date = billing_period_ending_date
         self.billing_period_starting_date = billing_period_starting_date
@@ -34,25 +36,26 @@
         self.billing_plan_amount = billing_plan_amount
         self.billing_plan_billing_date = billing_plan_billing_date
         self.billing_plan_item = billing_plan_item
         self.billing_plan_service_end_date = billing_plan_service_end_date
         self.billing_plan_service_start_date = billing_plan_service_start_date
 
     @staticmethod
-    def from_salesforce_record(record):
+    def from_salesforce_record(record, project_code):
         def _get_project_id():
             try:
                 return record["Project_Line_Item__r"]["Project__c"]
             except (TypeError, KeyError):
                 return ""
 
         return BillingLineDTO(
             id=record["Id"],
             name=record["Name"],
             project_id=_get_project_id(),
+            project_code=project_code,
             currency=record["CurrencyIsoCode"],
             created_date=record["CreatedDate"],
             last_modified_date=record["LastModifiedDate"],
             billing_amount=record["Biling_Ammount__c"],
             billing_date=record["Billing_Date__c"],
             billing_period_ending_date=record["Billing_Period_Ending_Date__c"],
             billing_period_starting_date=record[
@@ -71,14 +74,15 @@
             ],
         )
 
     def to_dict(self):
         return {
             "id": self.id,
             "project_id": self.project_id,
+            "project_code": self.project_code,
             "name": self.name,
             "currency": self.currency,
             "created_date": self.created_date,
             "last_modified_date": self.last_modified_date,
             "billing_amount": self.billing_amount,
             "billing_date": self.billing_date,
             "billing_period_ending_date": self.billing_period_ending_date,
```

### Comparing `ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/dto/OpportunityDTO.py` & `ms_salesforce_api-1.3.0/ms_salesforce_api/salesforce/project/dto/OpportunityDTO.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/dto/ProjectLineItemDTO.py` & `ms_salesforce_api-1.3.0/ms_salesforce_api/salesforce/project/dto/ProjectLineItemDTO.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/export_data/Bigquery.py` & `ms_salesforce_api-1.3.0/ms_salesforce_api/salesforce/project/export_data/Bigquery.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,25 +63,27 @@
                 "currency": "STRING",
                 "hourly_price": "FLOAT",
                 "id": "STRING",
                 "last_modified_date": "TIMESTAMP",
                 "name": "STRING",
                 "project_id": "STRING",
                 "revenue_dedication": "FLOAT",
+                "project_code": "STRING",
             },
             "project_line_items": {
                 "country": "STRING",
                 "created_date": "TIMESTAMP",
                 "effort": "STRING",
                 "ending_date": "DATE",
                 "id": "STRING",
                 "last_modified_date": "TIMESTAMP",
                 "ms_pli_name": "STRING",
                 "product_name": "STRING",
                 "project_id": "STRING",
+                "project_code": "STRING",
                 "quantity": "FLOAT",
                 "starting_date": "DATE",
                 "total_price": "STRING",
                 "unit_price": "STRING",
             },
             "accounts": {
                 "assigment_group": "STRING",
@@ -103,23 +105,25 @@
                 "mail_invoicing": "STRING",
                 "name": "STRING",
                 "office": "STRING",
                 "payment_terms": "STRING",
                 "pec_email": "STRING",
                 "phone": "STRING",
                 "project_id": "STRING",
+                "project_code": "STRING",
                 "sap_id": "STRING",
                 "tax_category": "STRING",
                 "tax_classification": "STRING",
                 "tax_id_type": "STRING",
                 "tier": "STRING",
                 "website": "STRING",
             },
             "groups": {
                 "project_id": "STRING",
+                "project_code": "STRING",
                 "groupid": "STRING",
                 "name": "STRING",
                 "start_date": "STRING",
                 "end_date": "STRING",
                 "bqid": "STRING",
                 "pck_type": "STRING",
             },
@@ -291,14 +295,15 @@
             )
 
             billing_lines_values.append(
                 f"""
                 (
                     "{bl['id']}",
                     "{bl['project_id']}",
+                    "{bl['project_code']}",
                     "{bl['name']}",
                     "{bl['currency']}",
                     TIMESTAMP "{bl['created_date']}",
                     TIMESTAMP "{bl['last_modified_date']}",
                     {bl['billing_amount'] if bl['billing_amount'] else 0.0},
                     {billing_date},
                     {billing_period_ending_date},
@@ -315,14 +320,15 @@
             )
 
         if billing_lines_values:
             insert_billing_lines_query = f"""
                 INSERT INTO `{self.project_id}.{self.dataset_id}.billing_lines` (
                     id,
                     project_id,
+                    project_code,
                     name,
                     currency,
                     created_date,
                     last_modified_date,
                     billing_amount,
                     billing_date,
                     billing_period_ending_date,
@@ -358,25 +364,28 @@
             for opp in opportunities:
                 remaining_plis = islice(
                     opp["project_line_items"], i, i + self.batch_size
                 )
                 batch_opportunities.append(opp)
                 batch_plis.extend(remaining_plis)
                 project_id = opp["project_id"]
+                project_code = opp["project_code"]
 
                 if len(batch_plis) >= self.batch_size:
-                    self._process_plis_batch(batch_plis, project_id)
+                    self._process_plis_batch(
+                        batch_plis, project_id, project_code
+                    )
 
                     batch_opportunities = []
                     batch_plis = []
 
             if batch_plis:
-                self._process_plis_batch(batch_plis, project_id)
+                self._process_plis_batch(batch_plis, project_id, project_code)
 
-    def _process_plis_batch(self, plis, project_id):
+    def _process_plis_batch(self, plis, project_id, project_code):
         plis_values = []
         for pli in plis:
             effort = f"{pli['effort']}" if pli["effort"] else "NULL"
             total_price = (
                 f"{pli['total_price']}" if pli["total_price"] else "NULL"
             )
 
@@ -407,15 +416,16 @@
                     TIMESTAMP "{pli['last_modified_date']}",
                     "{pli['ms_pli_name']}",
                     "{pli['product_name']}",
                     {pli['quantity'] if pli['quantity'] else 0.0},
                     {starting_date},
                     "{total_price}",
                     "{unit_price}",
-                    "{project_id}"
+                    "{project_id}",
+                    "{project_code}"
                 )
                 """
             )
 
         if plis_values:
             insert_plis_query = f"""
                 INSERT INTO `{self.project_id}.{self.dataset_id}.project_line_items` (
@@ -427,15 +437,16 @@
                     last_modified_date,
                     ms_pli_name,
                     product_name,
                     quantity,
                     starting_date,
                     total_price,
                     unit_price,
-                    project_id
+                    project_id,
+                    project_code
                 ) VALUES {', '.join(plis_values)};
             """
 
             insert_plis_query = (
                 insert_plis_query.replace("\n", "")
                 .replace("    ", "")
                 .replace("  ", "")
@@ -574,14 +585,15 @@
                 else "NULL"
             )
 
             account_values.append(
                 f"""
                 (
                     "{opp['project_id']}",
+                    "{opp['project_code']}",
                     {account_name},
                     {assigment_group},
                     {account_tax_category},
                     {account_tax_classification},
                     {account_sap_id},
                     {account_business_function},
                     {account_tax_id_type},
@@ -609,14 +621,15 @@
                 """
             )
 
         if account_values:
             insert_accounts_query = f"""
                 INSERT INTO `{self.project_id}.{self.dataset_id}.accounts` (
                     project_id,
+                    project_code,
                     name,
                     assigment_group,
                     tax_category,
                     tax_classification,
                     sap_id,
                     business_function,
                     tax_id_type,
@@ -684,14 +697,15 @@
                 else "NULL"
             )
 
             group_values.append(
                 f"""
                 (
                     "{opp['project_id']}",
+                    "{opp['project_code']}",
                     {group_id},
                     {group_name},
                     {group_start},
                     {group_end},
                     {group_bqid},
                     {group_pck_type}
 
@@ -699,14 +713,15 @@
                 """
             )
 
         if group_values:
             insert_group_query = f"""
                 INSERT INTO `{self.project_id}.{self.dataset_id}.groups` (
                     project_id,
+                    project_code,
                     groupid,
                     name,
                     start_date,
                     end_date,
                     bqid,
                     pck_type
                 ) VALUES {', '.join(group_values)};
```

### Comparing `ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/export_data/CloudSQL.py` & `ms_salesforce_api-1.3.0/ms_salesforce_api/salesforce/project/export_data/CloudSQL.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/export_data/__tests__/test_Bigquery.py` & `ms_salesforce_api-1.3.0/ms_salesforce_api/salesforce/project/export_data/__tests__/test_Bigquery.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,15 @@
                 "project_tier": "Unknown",
                 "jira_task_url": "ESMSBD0001-11848",
                 "opportunity_percentage": 10.0,
                 "billing_lines": [
                     {
                         "id": "a0sAa0000004Lx7IAE",
                         "project_id": "a003X000015kaPxQAI",
+                        "project_code": "ESMSEX00430",
                         "name": "BL-000320965",
                         "currency": "EUR",
                         "created_date": "2023-05-13T09:04:20.000+0000",
                         "last_modified_date": "2023-05-16T13:18:01.000+0000",
                         "billing_amount": 90.0,
                         "billing_date": "2023-05-13",
                         "billing_period_ending_date": "2023-05-27",
@@ -184,14 +185,15 @@
     def test_export_billing_lines(self):
         self.exporter._export_billing_lines(self.opportunities)
 
         expected_query = """
             INSERT INTO `your-project-id.your-dataset-id.billing_lines` (
                 id,
                 project_id,
+                project_code,
                 name,
                 currency,
                 created_date,
                 last_modified_date,
                 billing_amount,
                 billing_date,
                 billing_period_ending_date,
@@ -202,14 +204,15 @@
                 billing_plan_billing_date,
                 billing_plan_item,
                 billing_plan_service_end_date,
                 billing_plan_service_start_date
             ) VALUES (
                 "a0sAa0000004Lx7IAE",
                 "a003X000015kaPxQAI",
+                "ESMSEX00430",
                 "BL-000320965",
                 "EUR",
                 TIMESTAMP "2023-05-13T09:04:20.000+0000",
                 TIMESTAMP "2023-05-16T13:18:01.000+0000",
                 90.0,
                 DATE "2023-05-13",
                 DATE "2023-05-27",
@@ -245,29 +248,31 @@
                 last_modified_date,
                 ms_pli_name,
                 product_name,
                 quantity,
                 starting_date,
                 total_price,
                 unit_price,
-                project_id
+                project_id,
+                project_code
             ) VALUES (
                 "Spain",
                 TIMESTAMP "2023-05-13T09:03:14.000+0000",
                 "12",
                 DATE "2023-05-27",
                 "a0VAa000000fWbdMAE",
                 TIMESTAMP "2023-05-16T13:18:01.000+0000",
                 "_MSEX00430",
                 "ESM PRODUCT",
                 12.0,
                 DATE "2023-05-13",
                 "1080.0",
                 "90.0",
-                "a003X000015kaPxQAI"
+                "a003X000015kaPxQAI",
+                "ESMSEX00430"
             );
         """
 
         execute_query_calls = self.exporter.client.execute_query.call_args_list
 
         expected_query_stripped = re.sub(r"\s+", "", expected_query)
         execute_query_stripped = re.sub(
@@ -333,14 +338,15 @@
             );
         """
 
         expected_billing_lines_query = """
             INSERT INTO `your-project-id.your-dataset-id.billing_lines` (
                 id,
                 project_id,
+                project_code,
                 name,
                 currency,
                 created_date,
                 last_modified_date,
                 billing_amount,
                 billing_date,
                 billing_period_ending_date,
@@ -351,14 +357,15 @@
                 billing_plan_billing_date,
                 billing_plan_item,
                 billing_plan_service_end_date,
                 billing_plan_service_start_date
             ) VALUES (
                 "a0sAa0000004Lx7IAE",
                 "a003X000015kaPxQAI",
+                "ESMSEX00430",
                 "BL-000320965",
                 "EUR",
                 TIMESTAMP "2023-05-13T09:04:20.000+0000",
                 TIMESTAMP "2023-05-16T13:18:01.000+0000",
                 90.0,
                 DATE "2023-05-13",
                 DATE "2023-05-27",
@@ -383,35 +390,38 @@
                 last_modified_date,
                 ms_pli_name,
                 product_name,
                 quantity,
                 starting_date,
                 total_price,
                 unit_price,
-                project_id
+                project_id,
+                project_code
             ) VALUES (
                 "Spain",
                 TIMESTAMP "2023-05-13T09:03:14.000+0000",
                 "12",
                 DATE "2023-05-27",
                 "a0VAa000000fWbdMAE",
                 TIMESTAMP "2023-05-16T13:18:01.000+0000",
                 "_MSEX00430",
                 "ESM PRODUCT",
                 12.0,
                 DATE "2023-05-13",
                 "1080.0",
                 "90.0",
-                "a003X000015kaPxQAI"
+                "a003X000015kaPxQAI",
+                "ESMSEX00430"
             );
         """
 
         expected_accounts_query = """
             INSERT INTO `your-project-id.your-dataset-id.accounts` (
                 project_id,
+                project_code,
                 name,
                 assigment_group,
                 tax_category,
                 tax_classification,
                 sap_id,
                 business_function,
                 tax_id_type,
@@ -434,14 +444,15 @@
                 payment_terms,
                 billing_state_code,
                 mail_invoicing,
                 invoicing_email
             ) VALUES
                 (
                     "a003X000015kaPxQAI",
+                    "ESMSEX00430",
                     "ESMProjectAccount",
                     NULL,
                     NULL,
                     "0",
                     "10004171",
                     "BP03",
                     "CA2",
@@ -468,22 +479,24 @@
                 )
                 ;
         """
 
         expected_group_query = """
             INSERT INTO `your-project-id.your-dataset-id.groups`(
                 project_id,
+                project_code,
                 groupid,
                 name,
                 start_date,
                 end_date,
                 bqid,
                 pck_type
             ) VALUES(
                 "a003X000015kaPxQAI",
+                "ESMSEX00430",
                 "group_id_test",
                 "group_name_test",
                 "group_start_date_test",
                 "group_end_date_test",
                 "group_bqid_test",
                 "group_pck_type_test"
             );
```

### Comparing `ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/export_data/__tests__/test_CloudSQL.py` & `ms_salesforce_api-1.3.0/ms_salesforce_api/salesforce/project/export_data/__tests__/test_CloudSQL.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.2.4/pyproject.toml` & `ms_salesforce_api-1.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ms-salesforce-api"
-version = "1.2.4"
+version = "1.3.0"
 description = "Python library used to extract data from Salesforce API and migrate it to Bigquery and Postgres."
 authors = ["Making Science"]
 readme = "README.md"
 packages = [{include = "ms_salesforce_api"}]
 include = ["pre-commit-config.yaml"]
 
 [tool.poetry.dependencies]
```

### Comparing `ms_salesforce_api-1.2.4/PKG-INFO` & `ms_salesforce_api-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-salesforce-api
-Version: 1.2.4
+Version: 1.3.0
 Summary: Python library used to extract data from Salesforce API and migrate it to Bigquery and Postgres.
 Author: Making Science
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

