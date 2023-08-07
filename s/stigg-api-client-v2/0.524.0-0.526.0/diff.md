# Comparing `tmp/stigg_api_client_v2-0.524.0.tar.gz` & `tmp/stigg_api_client_v2-0.526.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_api_client_v2-0.524.0.tar", max compression
+gzip compressed data, was "stigg_api_client_v2-0.526.0.tar", max compression
```

## Comparing `stigg_api_client_v2-0.524.0.tar` & `stigg_api_client_v2-0.526.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     1644 2023-08-06 07:35:24.310589 stigg_api_client_v2-0.524.0/README.md
--rw-r--r--   0        0        0      452 2023-08-06 07:36:11.491213 stigg_api_client_v2-0.524.0/pyproject.toml
--rw-r--r--   0        0        0       62 2023-08-06 07:35:24.310589 stigg_api_client_v2-0.524.0/stigg/__init__.py
--rw-r--r--   0        0        0     4711 2023-08-06 07:35:24.310589 stigg_api_client_v2-0.524.0/stigg/client.py
--rw-r--r--   0        0        0      932 2023-08-06 07:35:24.314589 stigg_api_client_v2-0.524.0/stigg/edge_utils.py
--rw-r--r--   0        0        0    41178 2023-08-06 07:36:09.811191 stigg_api_client_v2-0.524.0/stigg/generated/__init__.py
--rw-r--r--   0        0        0      460 2023-08-06 07:36:08.423174 stigg_api_client_v2-0.524.0/stigg/generated/archive_customer.py
--rw-r--r--   0        0        0     7303 2023-08-06 07:36:09.311185 stigg_api_client_v2-0.524.0/stigg/generated/async_base_client.py
--rw-r--r--   0        0        0    70891 2023-08-06 07:36:09.647189 stigg_api_client_v2-0.524.0/stigg/generated/async_client.py
--rw-r--r--   0        0        0     2731 2023-08-06 07:36:04.055123 stigg_api_client_v2-0.524.0/stigg/generated/base_client.py
--rw-r--r--   0        0        0     1951 2023-08-06 07:36:09.311185 stigg_api_client_v2-0.524.0/stigg/generated/base_model.py
--rw-r--r--   0        0        0      527 2023-08-06 07:36:08.367173 stigg_api_client_v2-0.524.0/stigg/generated/cancel_subscription.py
--rw-r--r--   0        0        0      296 2023-08-06 07:36:08.383173 stigg_api_client_v2-0.524.0/stigg/generated/cancel_subscription_updates.py
--rw-r--r--   0        0        0    70464 2023-08-06 07:36:04.275123 stigg_api_client_v2-0.524.0/stigg/generated/client.py
--rw-r--r--   0        0        0      527 2023-08-06 07:36:08.407173 stigg_api_client_v2-0.524.0/stigg/generated/create_subscription.py
--rw-r--r--   0        0        0    24514 2023-08-06 07:36:05.895142 stigg_api_client_v2-0.524.0/stigg/generated/enums.py
--rw-r--r--   0        0        0      553 2023-08-06 07:36:08.371173 stigg_api_client_v2-0.524.0/stigg/generated/estimate_subscription.py
--rw-r--r--   0        0        0      614 2023-08-06 07:36:08.379173 stigg_api_client_v2-0.524.0/stigg/generated/estimate_subscription_update.py
--rw-r--r--   0        0        0     2366 2023-08-06 07:36:09.311185 stigg_api_client_v2-0.524.0/stigg/generated/exceptions.py
--rw-r--r--   0        0        0    58974 2023-08-06 07:36:09.307185 stigg_api_client_v2-0.524.0/stigg/generated/fragments.py
--rw-r--r--   0        0        0      591 2023-08-06 07:36:08.435174 stigg_api_client_v2-0.524.0/stigg/generated/get_active_subscriptions.py
--rw-r--r--   0        0        0      634 2023-08-06 07:36:08.443174 stigg_api_client_v2-0.524.0/stigg/generated/get_coupons.py
--rw-r--r--   0        0        0      572 2023-08-06 07:36:08.427174 stigg_api_client_v2-0.524.0/stigg/generated/get_customer_by_id.py
--rw-r--r--   0        0        0      533 2023-08-06 07:36:08.483175 stigg_api_client_v2-0.524.0/stigg/generated/get_customer_portal_by_ref_id.py
--rw-r--r--   0        0        0      390 2023-08-06 07:36:08.459174 stigg_api_client_v2-0.524.0/stigg/generated/get_entitlement.py
--rw-r--r--   0        0        0      430 2023-08-06 07:36:08.455174 stigg_api_client_v2-0.524.0/stigg/generated/get_entitlements.py
--rw-r--r--   0        0        0      893 2023-08-06 07:36:08.491175 stigg_api_client_v2-0.524.0/stigg/generated/get_mock_paywall.py
--rw-r--r--   0        0        0      346 2023-08-06 07:36:08.451174 stigg_api_client_v2-0.524.0/stigg/generated/get_paywall.py
--rw-r--r--   0        0        0      657 2023-08-06 07:36:08.467174 stigg_api_client_v2-0.524.0/stigg/generated/get_products.py
--rw-r--r--   0        0        0      650 2023-08-06 07:36:08.475175 stigg_api_client_v2-0.524.0/stigg/generated/get_sdk_configuration.py
--rw-r--r--   0        0        0      465 2023-08-06 07:36:08.335173 stigg_api_client_v2-0.524.0/stigg/generated/import_customer.py
--rw-r--r--   0        0        0      332 2023-08-06 07:36:08.327173 stigg_api_client_v2-0.524.0/stigg/generated/import_customer_bulk.py
--rw-r--r--   0        0        0      350 2023-08-06 07:36:08.355173 stigg_api_client_v2-0.524.0/stigg/generated/import_subscriptions_bulk.py
--rw-r--r--   0        0        0   128817 2023-08-06 07:36:08.191171 stigg_api_client_v2-0.524.0/stigg/generated/input_types.py
--rw-r--r--   0        0        0      604 2023-08-06 07:36:08.415174 stigg_api_client_v2-0.524.0/stigg/generated/migrate_subscription_to_latest.py
--rw-r--r--   0        0        0     1161 2023-08-06 07:36:08.223171 stigg_api_client_v2-0.524.0/stigg/generated/provision_customer.py
--rw-r--r--   0        0        0      971 2023-08-06 07:36:08.347173 stigg_api_client_v2-0.524.0/stigg/generated/provision_subscription.py
--rw-r--r--   0        0        0      359 2023-08-06 07:36:08.403174 stigg_api_client_v2-0.524.0/stigg/generated/report_entitlement_check_requested.py
--rw-r--r--   0        0        0      301 2023-08-06 07:36:08.395173 stigg_api_client_v2-0.524.0/stigg/generated/report_event.py
--rw-r--r--   0        0        0      637 2023-08-06 07:36:08.391173 stigg_api_client_v2-0.524.0/stigg/generated/report_usage.py
--rw-r--r--   0        0        0      220 2023-08-06 07:36:09.315185 stigg_api_client_v2-0.524.0/stigg/generated/scalars.py
--rw-r--r--   0        0        0      465 2023-08-06 07:36:08.339173 stigg_api_client_v2-0.524.0/stigg/generated/update_customer.py
--rw-r--r--   0        0        0      527 2023-08-06 07:36:08.359173 stigg_api_client_v2-0.524.0/stigg/generated/update_subscription.py
--rw-r--r--   0        0        0      445 2023-08-06 07:36:08.499175 stigg_api_client_v2-0.524.0/stigg/generated/usage_history.py
--rw-r--r--   0        0        0     2075 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.524.0/PKG-INFO
+-rw-r--r--   0        0        0     1644 2023-08-07 15:01:25.393482 stigg_api_client_v2-0.526.0/README.md
+-rw-r--r--   0        0        0      452 2023-08-07 15:02:09.638442 stigg_api_client_v2-0.526.0/pyproject.toml
+-rw-r--r--   0        0        0       62 2023-08-07 15:01:25.393482 stigg_api_client_v2-0.526.0/stigg/__init__.py
+-rw-r--r--   0        0        0     4711 2023-08-07 15:01:25.393482 stigg_api_client_v2-0.526.0/stigg/client.py
+-rw-r--r--   0        0        0      932 2023-08-07 15:01:25.393482 stigg_api_client_v2-0.526.0/stigg/edge_utils.py
+-rw-r--r--   0        0        0    41316 2023-08-07 15:02:08.002449 stigg_api_client_v2-0.526.0/stigg/generated/__init__.py
+-rw-r--r--   0        0        0      460 2023-08-07 15:02:06.622420 stigg_api_client_v2-0.526.0/stigg/generated/archive_customer.py
+-rw-r--r--   0        0        0     7303 2023-08-07 15:02:07.522440 stigg_api_client_v2-0.526.0/stigg/generated/async_base_client.py
+-rw-r--r--   0        0        0    70891 2023-08-07 15:02:07.742445 stigg_api_client_v2-0.526.0/stigg/generated/async_client.py
+-rw-r--r--   0        0        0     2731 2023-08-07 15:02:02.454331 stigg_api_client_v2-0.526.0/stigg/generated/base_client.py
+-rw-r--r--   0        0        0     1951 2023-08-07 15:02:07.522440 stigg_api_client_v2-0.526.0/stigg/generated/base_model.py
+-rw-r--r--   0        0        0      527 2023-08-07 15:02:06.566419 stigg_api_client_v2-0.526.0/stigg/generated/cancel_subscription.py
+-rw-r--r--   0        0        0      296 2023-08-07 15:02:06.586420 stigg_api_client_v2-0.526.0/stigg/generated/cancel_subscription_updates.py
+-rw-r--r--   0        0        0    70464 2023-08-07 15:02:02.670335 stigg_api_client_v2-0.526.0/stigg/generated/client.py
+-rw-r--r--   0        0        0      527 2023-08-07 15:02:06.610420 stigg_api_client_v2-0.526.0/stigg/generated/create_subscription.py
+-rw-r--r--   0        0        0    24622 2023-08-07 15:02:04.254370 stigg_api_client_v2-0.526.0/stigg/generated/enums.py
+-rw-r--r--   0        0        0      553 2023-08-07 15:02:06.574419 stigg_api_client_v2-0.526.0/stigg/generated/estimate_subscription.py
+-rw-r--r--   0        0        0      614 2023-08-07 15:02:06.582419 stigg_api_client_v2-0.526.0/stigg/generated/estimate_subscription_update.py
+-rw-r--r--   0        0        0     2366 2023-08-07 15:02:07.522440 stigg_api_client_v2-0.526.0/stigg/generated/exceptions.py
+-rw-r--r--   0        0        0    58974 2023-08-07 15:02:07.518440 stigg_api_client_v2-0.526.0/stigg/generated/fragments.py
+-rw-r--r--   0        0        0      591 2023-08-07 15:02:06.634421 stigg_api_client_v2-0.526.0/stigg/generated/get_active_subscriptions.py
+-rw-r--r--   0        0        0      634 2023-08-07 15:02:06.646421 stigg_api_client_v2-0.526.0/stigg/generated/get_coupons.py
+-rw-r--r--   0        0        0      572 2023-08-07 15:02:06.630421 stigg_api_client_v2-0.526.0/stigg/generated/get_customer_by_id.py
+-rw-r--r--   0        0        0      533 2023-08-07 15:02:06.682422 stigg_api_client_v2-0.526.0/stigg/generated/get_customer_portal_by_ref_id.py
+-rw-r--r--   0        0        0      390 2023-08-07 15:02:06.658421 stigg_api_client_v2-0.526.0/stigg/generated/get_entitlement.py
+-rw-r--r--   0        0        0      430 2023-08-07 15:02:06.654421 stigg_api_client_v2-0.526.0/stigg/generated/get_entitlements.py
+-rw-r--r--   0        0        0      893 2023-08-07 15:02:06.690422 stigg_api_client_v2-0.526.0/stigg/generated/get_mock_paywall.py
+-rw-r--r--   0        0        0      346 2023-08-07 15:02:06.650421 stigg_api_client_v2-0.526.0/stigg/generated/get_paywall.py
+-rw-r--r--   0        0        0      657 2023-08-07 15:02:06.666422 stigg_api_client_v2-0.526.0/stigg/generated/get_products.py
+-rw-r--r--   0        0        0      650 2023-08-07 15:02:06.678422 stigg_api_client_v2-0.526.0/stigg/generated/get_sdk_configuration.py
+-rw-r--r--   0        0        0      465 2023-08-07 15:02:06.534419 stigg_api_client_v2-0.526.0/stigg/generated/import_customer.py
+-rw-r--r--   0        0        0      332 2023-08-07 15:02:06.530418 stigg_api_client_v2-0.526.0/stigg/generated/import_customer_bulk.py
+-rw-r--r--   0        0        0      350 2023-08-07 15:02:06.554419 stigg_api_client_v2-0.526.0/stigg/generated/import_subscriptions_bulk.py
+-rw-r--r--   0        0        0   130043 2023-08-07 15:02:06.514418 stigg_api_client_v2-0.526.0/stigg/generated/input_types.py
+-rw-r--r--   0        0        0      604 2023-08-07 15:02:06.618420 stigg_api_client_v2-0.526.0/stigg/generated/migrate_subscription_to_latest.py
+-rw-r--r--   0        0        0     1161 2023-08-07 15:02:06.526418 stigg_api_client_v2-0.526.0/stigg/generated/provision_customer.py
+-rw-r--r--   0        0        0      971 2023-08-07 15:02:06.550419 stigg_api_client_v2-0.526.0/stigg/generated/provision_subscription.py
+-rw-r--r--   0        0        0      359 2023-08-07 15:02:06.602420 stigg_api_client_v2-0.526.0/stigg/generated/report_entitlement_check_requested.py
+-rw-r--r--   0        0        0      301 2023-08-07 15:02:06.598420 stigg_api_client_v2-0.526.0/stigg/generated/report_event.py
+-rw-r--r--   0        0        0      637 2023-08-07 15:02:06.594420 stigg_api_client_v2-0.526.0/stigg/generated/report_usage.py
+-rw-r--r--   0        0        0      220 2023-08-07 15:02:07.526440 stigg_api_client_v2-0.526.0/stigg/generated/scalars.py
+-rw-r--r--   0        0        0      465 2023-08-07 15:02:06.542419 stigg_api_client_v2-0.526.0/stigg/generated/update_customer.py
+-rw-r--r--   0        0        0      527 2023-08-07 15:02:06.562419 stigg_api_client_v2-0.526.0/stigg/generated/update_subscription.py
+-rw-r--r--   0        0        0      445 2023-08-07 15:02:06.698422 stigg_api_client_v2-0.526.0/stigg/generated/usage_history.py
+-rw-r--r--   0        0        0     2075 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.526.0/PKG-INFO
```

### Comparing `stigg_api_client_v2-0.524.0/README.md` & `stigg_api_client_v2-0.526.0/README.md`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.524.0/stigg/client.py` & `stigg_api_client_v2-0.526.0/stigg/client.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.524.0/stigg/edge_utils.py` & `stigg_api_client_v2-0.526.0/stigg/edge_utils.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.524.0/stigg/generated/__init__.py` & `stigg_api_client_v2-0.526.0/stigg/generated/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-06 07:36
+# Generated by ariadne-codegen on 2023-08-07 15:02
 
 from .archive_customer import ArchiveCustomer, ArchiveCustomerArchiveCustomer
 from .async_base_client import AsyncBaseClient
 from .async_client import AsyncClient
 from .base_model import BaseModel
 from .cancel_subscription import (
     CancelSubscription,
@@ -87,14 +87,15 @@
     SubscriptionScheduleStatus,
     SubscriptionScheduleType,
     SubscriptionStartSetup,
     SubscriptionStatus,
     SyncStatus,
     TaskStatus,
     TaskType,
+    TiersMode,
     TrialPeriodUnits,
     UsageMeasurementSortFields,
     UsageUpdateBehavior,
     VendorIdentifier,
     WeeklyAccordingTo,
     WidgetType,
     experimentGroupType,
@@ -488,14 +489,15 @@
     PlanFilterProductFilter,
     PlanSort,
     PlanUpdateInput,
     PriceFilter,
     PriceFilterPackageDTOFilter,
     PricePeriodInput,
     PriceSort,
+    PriceTierInput,
     PricingModelCreateInput,
     PricingTypeFilterComparison,
     ProductCreateInput,
     ProductFilter,
     ProductSettingsInput,
     ProductSort,
     ProductUpdateInput,
@@ -556,14 +558,15 @@
     SubscriptionStatusFilterComparison,
     SubscriptionUpdateScheduleCancellationInput,
     SyncTaxRatesInput,
     TaskStatusFilterComparison,
     TaskTypeFilterComparison,
     TaxExempt,
     TestHookInput,
+    TiersModeFilterComparison,
     TypographyConfigurationInput,
     UpdateAccountInput,
     UpdateCouponInput,
     UpdateCustomerInput,
     UpdateExperimentInput,
     UpdateFeature,
     UpdateFeatureInput,
@@ -990,14 +993,15 @@
     "PriceFilterPackageDTOFilter",
     "PriceFragment",
     "PriceFragmentFeature",
     "PriceFragmentPrice",
     "PricePeriodInput",
     "PriceSort",
     "PriceSortFields",
+    "PriceTierInput",
     "PricingModelCreateInput",
     "PricingType",
     "PricingTypeFilterComparison",
     "ProductCreateInput",
     "ProductFilter",
     "ProductFragment",
     "ProductFragmentProductSettings",
@@ -1151,14 +1155,16 @@
     "SyncTaxRatesInput",
     "TaskStatus",
     "TaskStatusFilterComparison",
     "TaskType",
     "TaskTypeFilterComparison",
     "TaxExempt",
     "TestHookInput",
+    "TiersMode",
+    "TiersModeFilterComparison",
     "TotalPriceFragment",
     "TotalPriceFragmentSubTotal",
     "TotalPriceFragmentTotal",
     "TrialPeriodUnits",
     "TypographyConfigurationFragment",
     "TypographyConfigurationFragmentBody",
     "TypographyConfigurationFragmentH1",
```

### Comparing `stigg_api_client_v2-0.524.0/stigg/generated/async_base_client.py` & `stigg_api_client_v2-0.526.0/stigg/generated/async_base_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-06 07:36
+# Generated by ariadne-codegen on 2023-08-07 15:02
 
 import enum
 import json
 from typing import Any, AsyncIterator, Dict, Optional, TypeVar, cast
 from uuid import uuid4
 
 import httpx
```

### Comparing `stigg_api_client_v2-0.524.0/stigg/generated/async_client.py` & `stigg_api_client_v2-0.526.0/stigg/generated/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-06 07:36
+# Generated by ariadne-codegen on 2023-08-07 15:02
 # Source: operations.graphql
 
 from .archive_customer import ArchiveCustomer
 from .async_base_client import AsyncBaseClient
 from .cancel_subscription import CancelSubscription
 from .cancel_subscription_updates import CancelSubscriptionUpdates
 from .create_subscription import CreateSubscription
```

### Comparing `stigg_api_client_v2-0.524.0/stigg/generated/base_client.py` & `stigg_api_client_v2-0.526.0/stigg/generated/base_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-06 07:36
+# Generated by ariadne-codegen on 2023-08-07 15:02
 
 import json
 from typing import Any, Dict, Optional, TypeVar, cast
 
 import httpx
 from pydantic import BaseModel
 from pydantic.json import pydantic_encoder
```

### Comparing `stigg_api_client_v2-0.524.0/stigg/generated/base_model.py` & `stigg_api_client_v2-0.526.0/stigg/generated/base_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-06 07:36
+# Generated by ariadne-codegen on 2023-08-07 15:02
 
 from typing import Any, Dict, Type, Union, get_args, get_origin
 
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic.class_validators import validator
 from pydantic.fields import ModelField
```

### Comparing `stigg_api_client_v2-0.524.0/stigg/generated/cancel_subscription.py` & `stigg_api_client_v2-0.526.0/stigg/generated/cancel_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-06 07:36
+# Generated by ariadne-codegen on 2023-08-07 15:02
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.524.0/stigg/generated/client.py` & `stigg_api_client_v2-0.526.0/stigg/generated/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-06 07:36
+# Generated by ariadne-codegen on 2023-08-07 15:02
 # Source: operations.graphql
 
 from .archive_customer import ArchiveCustomer
 from .base_client import BaseClient
 from .cancel_subscription import CancelSubscription
 from .cancel_subscription_updates import CancelSubscriptionUpdates
 from .create_subscription import CreateSubscription
```

### Comparing `stigg_api_client_v2-0.524.0/stigg/generated/create_subscription.py` & `stigg_api_client_v2-0.526.0/stigg/generated/update_subscription.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# Generated by ariadne-codegen on 2023-08-06 07:36
+# Generated by ariadne-codegen on 2023-08-07 15:02
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
 
 
-class CreateSubscription(BaseModel):
-    create_subscription: "CreateSubscriptionCreateSubscription" = Field(
-        alias="createSubscription"
+class UpdateSubscription(BaseModel):
+    update_subscription: "UpdateSubscriptionUpdateSubscription" = Field(
+        alias="updateSubscription"
     )
 
 
-class CreateSubscriptionCreateSubscription(SlimSubscriptionFragment):
+class UpdateSubscriptionUpdateSubscription(SlimSubscriptionFragment):
     pass
 
 
-CreateSubscription.update_forward_refs()
-CreateSubscriptionCreateSubscription.update_forward_refs()
+UpdateSubscription.update_forward_refs()
+UpdateSubscriptionUpdateSubscription.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.524.0/stigg/generated/enums.py` & `stigg_api_client_v2-0.526.0/stigg/generated/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-06 07:36
+# Generated by ariadne-codegen on 2023-08-07 15:02
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from enum import Enum
 
 
 class AccessDeniedReason(str, Enum):
     CustomerIsArchived = "CustomerIsArchived"
@@ -644,14 +644,15 @@
 
 class PriceSortFields(str, Enum):
     billingId = "billingId"
     billingModel = "billingModel"
     billingPeriod = "billingPeriod"
     createdAt = "createdAt"
     id = "id"
+    tiersMode = "tiersMode"
 
 
 class PricingType(str, Enum):
     CUSTOM = "CUSTOM"
     FREE = "FREE"
     PAID = "PAID"
 
@@ -844,14 +845,19 @@
     IMPORT_INTEGRATION_CUSTOMERS = "IMPORT_INTEGRATION_CUSTOMERS"
     IMPORT_SUBSCRIPTIONS_BULK = "IMPORT_SUBSCRIPTIONS_BULK"
     RECALCULATE_ENTITLEMENTS = "RECALCULATE_ENTITLEMENTS"
     RESYNC_INTEGRATION = "RESYNC_INTEGRATION"
     SUBSCRIPTION_MIGRATION = "SUBSCRIPTION_MIGRATION"
 
 
+class TiersMode(str, Enum):
+    GRADUATED = "GRADUATED"
+    VOLUME = "VOLUME"
+
+
 class TrialPeriodUnits(str, Enum):
     DAY = "DAY"
     MONTH = "MONTH"
 
 
 class UsageMeasurementSortFields(str, Enum):
     createdAt = "createdAt"
```

### Comparing `stigg_api_client_v2-0.524.0/stigg/generated/estimate_subscription.py` & `stigg_api_client_v2-0.526.0/stigg/generated/estimate_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-06 07:36
+# Generated by ariadne-codegen on 2023-08-07 15:02
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.524.0/stigg/generated/estimate_subscription_update.py` & `stigg_api_client_v2-0.526.0/stigg/generated/estimate_subscription_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-06 07:36
+# Generated by ariadne-codegen on 2023-08-07 15:02
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.524.0/stigg/generated/exceptions.py` & `stigg_api_client_v2-0.526.0/stigg/generated/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-06 07:36
+# Generated by ariadne-codegen on 2023-08-07 15:02
 
 from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
 
 class GraphQLClientError(Exception):
```

### Comparing `stigg_api_client_v2-0.524.0/stigg/generated/fragments.py` & `stigg_api_client_v2-0.526.0/stigg/generated/fragments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-06 07:36
+# Generated by ariadne-codegen on 2023-08-07 15:02
 # Source: operations.graphql
 
 from typing import Annotated, Any, List, Literal, Optional, Union
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -342,21 +342,14 @@
     end_date: Optional[Any] = Field(alias="endDate")
 
 
 class CustomerResourceFragment(BaseModel):
     resource_id: str = Field(alias="resourceId")
 
 
-class CustomerPortalSubscriptionAddon(BaseModel):
-    addon_id: str = Field(alias="addonId")
-    description: Optional[str]
-    display_name: str = Field(alias="displayName")
-    quantity: int
-
-
 class CustomerPortalSubscriptionPriceFragment(BaseModel):
     billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
     billing_model: Optional[BillingModel] = Field(alias="billingModel")
     price: Optional["CustomerPortalSubscriptionPriceFragmentPrice"]
     feature: Optional["CustomerPortalSubscriptionPriceFragmentFeature"]
 
 
@@ -421,14 +414,21 @@
     BaseModel
 ):
     typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
     new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
     feature_id: Optional[str] = Field(alias="featureId")
 
 
+class CustomerPortalSubscriptionAddon(BaseModel):
+    addon_id: str = Field(alias="addonId")
+    description: Optional[str]
+    display_name: str = Field(alias="displayName")
+    quantity: int
+
+
 class CustomerPortalSubscriptionFragment(BaseModel):
     subscription_id: str = Field(alias="subscriptionId")
     plan_name: str = Field(alias="planName")
     pricing_type: PricingType = Field(alias="pricingType")
     prices: List["CustomerPortalSubscriptionFragmentPrices"]
     pricing: "CustomerPortalSubscriptionFragmentPricing"
     status: SubscriptionStatus
@@ -548,14 +548,61 @@
     pass
 
 
 class CustomerPortalFragmentResource(CustomerResourceFragment):
     pass
 
 
+class SubscriptionFutureUpdateData(BaseModel):
+    subscription_schedule_type: SubscriptionScheduleType = Field(
+        alias="subscriptionScheduleType"
+    )
+    schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
+    scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
+    target_package: Optional["SubscriptionFutureUpdateDataTargetPackage"] = Field(
+        alias="targetPackage"
+    )
+    schedule_variables: Optional[
+        Annotated[
+            Union[
+                "SubscriptionFutureUpdateDataScheduleVariablesBillingPeriodChangeVariables",
+                "SubscriptionFutureUpdateDataScheduleVariablesDowngradeChangeVariables",
+                "SubscriptionFutureUpdateDataScheduleVariablesUnitAmountChangeVariables",
+            ],
+            Field(discriminator="typename__"),
+        ]
+    ] = Field(alias="scheduleVariables")
+
+
+class SubscriptionFutureUpdateDataTargetPackage(BaseModel):
+    id: str
+    ref_id: str = Field(alias="refId")
+    display_name: str = Field(alias="displayName")
+
+
+class SubscriptionFutureUpdateDataScheduleVariablesBillingPeriodChangeVariables(
+    BaseModel
+):
+    typename__: Literal["BillingPeriodChangeVariables"] = Field(alias="__typename")
+    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
+
+
+class SubscriptionFutureUpdateDataScheduleVariablesDowngradeChangeVariables(BaseModel):
+    typename__: Literal["DowngradeChangeVariables"] = Field(alias="__typename")
+    addon_ref_ids: Optional[str] = Field(alias="addonRefIds")
+    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
+    downgrade_plan_ref_id: str = Field(alias="downgradePlanRefId")
+
+
+class SubscriptionFutureUpdateDataScheduleVariablesUnitAmountChangeVariables(BaseModel):
+    typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
+    new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
+    feature_id: Optional[str] = Field(alias="featureId")
+
+
 class TotalPriceFragment(BaseModel):
     sub_total: "TotalPriceFragmentSubTotal" = Field(alias="subTotal")
     total: "TotalPriceFragmentTotal"
 
 
 class TotalPriceFragmentSubTotal(BaseModel):
     amount: float
@@ -563,56 +610,60 @@
 
 
 class TotalPriceFragmentTotal(BaseModel):
     amount: float
     currency: Currency
 
 
-class SubscriptionFutureUpdateData(BaseModel):
+class SubscriptionScheduledUpdateData(BaseModel):
     subscription_schedule_type: SubscriptionScheduleType = Field(
         alias="subscriptionScheduleType"
     )
     schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
     scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
-    target_package: Optional["SubscriptionFutureUpdateDataTargetPackage"] = Field(
+    target_package: Optional["SubscriptionScheduledUpdateDataTargetPackage"] = Field(
         alias="targetPackage"
     )
     schedule_variables: Optional[
         Annotated[
             Union[
-                "SubscriptionFutureUpdateDataScheduleVariablesBillingPeriodChangeVariables",
-                "SubscriptionFutureUpdateDataScheduleVariablesDowngradeChangeVariables",
-                "SubscriptionFutureUpdateDataScheduleVariablesUnitAmountChangeVariables",
+                "SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables",
+                "SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables",
+                "SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables",
             ],
             Field(discriminator="typename__"),
         ]
     ] = Field(alias="scheduleVariables")
 
 
-class SubscriptionFutureUpdateDataTargetPackage(BaseModel):
+class SubscriptionScheduledUpdateDataTargetPackage(BaseModel):
     id: str
     ref_id: str = Field(alias="refId")
     display_name: str = Field(alias="displayName")
 
 
-class SubscriptionFutureUpdateDataScheduleVariablesBillingPeriodChangeVariables(
+class SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables(
     BaseModel
 ):
     typename__: Literal["BillingPeriodChangeVariables"] = Field(alias="__typename")
     billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
 
 
-class SubscriptionFutureUpdateDataScheduleVariablesDowngradeChangeVariables(BaseModel):
+class SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables(
+    BaseModel
+):
     typename__: Literal["DowngradeChangeVariables"] = Field(alias="__typename")
     addon_ref_ids: Optional[str] = Field(alias="addonRefIds")
     billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
     downgrade_plan_ref_id: str = Field(alias="downgradePlanRefId")
 
 
-class SubscriptionFutureUpdateDataScheduleVariablesUnitAmountChangeVariables(BaseModel):
+class SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables(
+    BaseModel
+):
     typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
     new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
     feature_id: Optional[str] = Field(alias="featureId")
 
 
 class ProductFragment(BaseModel):
     ref_id: str = Field(alias="refId")
@@ -683,65 +734,14 @@
 
 
 class PlanFragmentDefaultTrialConfig(BaseModel):
     duration: float
     units: TrialPeriodUnits
 
 
-class SubscriptionScheduledUpdateData(BaseModel):
-    subscription_schedule_type: SubscriptionScheduleType = Field(
-        alias="subscriptionScheduleType"
-    )
-    schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
-    scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
-    target_package: Optional["SubscriptionScheduledUpdateDataTargetPackage"] = Field(
-        alias="targetPackage"
-    )
-    schedule_variables: Optional[
-        Annotated[
-            Union[
-                "SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables",
-                "SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables",
-                "SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables",
-            ],
-            Field(discriminator="typename__"),
-        ]
-    ] = Field(alias="scheduleVariables")
-
-
-class SubscriptionScheduledUpdateDataTargetPackage(BaseModel):
-    id: str
-    ref_id: str = Field(alias="refId")
-    display_name: str = Field(alias="displayName")
-
-
-class SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables(
-    BaseModel
-):
-    typename__: Literal["BillingPeriodChangeVariables"] = Field(alias="__typename")
-    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
-
-
-class SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables(
-    BaseModel
-):
-    typename__: Literal["DowngradeChangeVariables"] = Field(alias="__typename")
-    addon_ref_ids: Optional[str] = Field(alias="addonRefIds")
-    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
-    downgrade_plan_ref_id: str = Field(alias="downgradePlanRefId")
-
-
-class SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables(
-    BaseModel
-):
-    typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
-    new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
-    feature_id: Optional[str] = Field(alias="featureId")
-
-
 class SubscriptionFragment(BaseModel):
     id: str
     start_date: Any = Field(alias="startDate")
     end_date: Optional[Any] = Field(alias="endDate")
     trial_end_date: Optional[Any] = Field(alias="trialEndDate")
     cancellation_date: Optional[Any] = Field(alias="cancellationDate")
     effective_end_date: Optional[Any] = Field(alias="effectiveEndDate")
@@ -1433,23 +1433,23 @@
 FeatureFragment.update_forward_refs()
 CustomerPortalEntitlement.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationMonthlyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationWeeklyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementFeature.update_forward_refs()
 CustomerPortalPromotionalEntitlement.update_forward_refs()
 CustomerResourceFragment.update_forward_refs()
-CustomerPortalSubscriptionAddon.update_forward_refs()
 CustomerPortalSubscriptionPriceFragment.update_forward_refs()
 CustomerPortalSubscriptionPriceFragmentPrice.update_forward_refs()
 CustomerPortalSubscriptionPriceFragmentFeature.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateData.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
+CustomerPortalSubscriptionAddon.update_forward_refs()
 CustomerPortalSubscriptionFragment.update_forward_refs()
 CustomerPortalSubscriptionFragmentPrices.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricing.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricingPrice.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricingFeature.update_forward_refs()
 CustomerPortalSubscriptionFragmentBillingPeriodRange.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPrice.update_forward_refs()
@@ -1461,38 +1461,38 @@
 CustomerPortalFragment.update_forward_refs()
 CustomerPortalFragmentSubscriptions.update_forward_refs()
 CustomerPortalFragmentEntitlements.update_forward_refs()
 CustomerPortalFragmentPromotionalEntitlements.update_forward_refs()
 CustomerPortalFragmentBillingInformation.update_forward_refs()
 CustomerPortalFragmentConfiguration.update_forward_refs()
 CustomerPortalFragmentResource.update_forward_refs()
-TotalPriceFragment.update_forward_refs()
-TotalPriceFragmentSubTotal.update_forward_refs()
-TotalPriceFragmentTotal.update_forward_refs()
 SubscriptionFutureUpdateData.update_forward_refs()
 SubscriptionFutureUpdateDataTargetPackage.update_forward_refs()
 SubscriptionFutureUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
 SubscriptionFutureUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
 SubscriptionFutureUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
+TotalPriceFragment.update_forward_refs()
+TotalPriceFragmentSubTotal.update_forward_refs()
+TotalPriceFragmentTotal.update_forward_refs()
+SubscriptionScheduledUpdateData.update_forward_refs()
+SubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
+SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
+SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
+SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
 ProductFragment.update_forward_refs()
 ProductFragmentProductSettings.update_forward_refs()
 ProductFragmentProductSettingsDowngradePlan.update_forward_refs()
 PlanFragment.update_forward_refs()
 PlanFragmentProduct.update_forward_refs()
 PlanFragmentBasePlan.update_forward_refs()
 PlanFragmentEntitlements.update_forward_refs()
 PlanFragmentInheritedEntitlements.update_forward_refs()
 PlanFragmentCompatibleAddons.update_forward_refs()
 PlanFragmentPrices.update_forward_refs()
 PlanFragmentDefaultTrialConfig.update_forward_refs()
-SubscriptionScheduledUpdateData.update_forward_refs()
-SubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
-SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
-SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
-SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
 SubscriptionFragment.update_forward_refs()
 SubscriptionFragmentResource.update_forward_refs()
 SubscriptionFragmentExperimentInfo.update_forward_refs()
 SubscriptionFragmentPrices.update_forward_refs()
 SubscriptionFragmentPricesPrice.update_forward_refs()
 SubscriptionFragmentTotalPrice.update_forward_refs()
 SubscriptionFragmentPlan.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.524.0/stigg/generated/get_active_subscriptions.py` & `stigg_api_client_v2-0.526.0/stigg/generated/get_active_subscriptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-06 07:36
+# Generated by ariadne-codegen on 2023-08-07 15:02
 # Source: operations.graphql
 
 from typing import List
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.524.0/stigg/generated/get_coupons.py` & `stigg_api_client_v2-0.526.0/stigg/generated/get_coupons.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-06 07:36
+# Generated by ariadne-codegen on 2023-08-07 15:02
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import CouponFragment
```

### Comparing `stigg_api_client_v2-0.524.0/stigg/generated/get_customer_portal_by_ref_id.py` & `stigg_api_client_v2-0.526.0/stigg/generated/get_customer_portal_by_ref_id.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-06 07:36
+# Generated by ariadne-codegen on 2023-08-07 15:02
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import CustomerPortalFragment
```

### Comparing `stigg_api_client_v2-0.524.0/stigg/generated/get_mock_paywall.py` & `stigg_api_client_v2-0.526.0/stigg/generated/get_mock_paywall.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-06 07:36
+# Generated by ariadne-codegen on 2023-08-07 15:02
 # Source: operations.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.524.0/stigg/generated/get_products.py` & `stigg_api_client_v2-0.526.0/stigg/generated/get_products.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-06 07:36
+# Generated by ariadne-codegen on 2023-08-07 15:02
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import ProductFragment
```

### Comparing `stigg_api_client_v2-0.524.0/stigg/generated/get_sdk_configuration.py` & `stigg_api_client_v2-0.526.0/stigg/generated/get_sdk_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-06 07:36
+# Generated by ariadne-codegen on 2023-08-07 15:02
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.524.0/stigg/generated/input_types.py` & `stigg_api_client_v2-0.526.0/stigg/generated/input_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-06 07:36
+# Generated by ariadne-codegen on 2023-08-07 15:02
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from typing import Any, List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -66,14 +66,15 @@
     SubscriptionMigrationTime,
     SubscriptionPriceSortFields,
     SubscriptionScheduleStatus,
     SubscriptionStartSetup,
     SubscriptionStatus,
     TaskStatus,
     TaskType,
+    TiersMode,
     TrialPeriodUnits,
     UsageMeasurementSortFields,
     UsageUpdateBehavior,
     VendorIdentifier,
     WeeklyAccordingTo,
     WidgetType,
 )
@@ -1651,14 +1652,15 @@
     billing_period: Optional["BillingPeriodFilterComparison"] = Field(
         alias="billingPeriod"
     )
     created_at: Optional["DateFieldComparison"] = Field(alias="createdAt")
     id: Optional["StringFieldComparison"]
     or_: Optional[List["PriceFilter"]] = Field(alias="or")
     package: Optional["PriceFilterPackageDTOFilter"]
+    tiers_mode: Optional["TiersModeFilterComparison"] = Field(alias="tiersMode")
 
 
 class PriceFilterPackageDTOFilter(BaseModel):
     and_: Optional[List["PriceFilterPackageDTOFilter"]] = Field(alias="and")
     billing_id: Optional["StringFieldComparison"] = Field(alias="billingId")
     created_at: Optional["DateFieldComparison"] = Field(alias="createdAt")
     description: Optional["StringFieldComparison"]
@@ -1674,29 +1676,36 @@
     updated_at: Optional["DateFieldComparison"] = Field(alias="updatedAt")
     version_number: Optional["IntFieldComparison"] = Field(alias="versionNumber")
 
 
 class PricePeriodInput(BaseModel):
     billing_country_code: Optional[str] = Field(alias="billingCountryCode")
     billing_period: BillingPeriod = Field(alias="billingPeriod")
-    price: "MoneyInputDTO"
+    price: Optional["MoneyInputDTO"]
+    tiers: Optional[List["PriceTierInput"]]
 
 
 class PriceSort(BaseModel):
     direction: SortDirection
     field: PriceSortFields
     nulls: Optional[SortNulls]
 
 
+class PriceTierInput(BaseModel):
+    unit_price: "MoneyInputDTO" = Field(alias="unitPrice")
+    up_to: float = Field(alias="upTo")
+
+
 class PricingModelCreateInput(BaseModel):
     billing_model: BillingModel = Field(alias="billingModel")
     feature_id: Optional[str] = Field(alias="featureId")
     max_unit_quantity: Optional[float] = Field(alias="maxUnitQuantity")
     min_unit_quantity: Optional[float] = Field(alias="minUnitQuantity")
     price_periods: List["PricePeriodInput"] = Field(alias="pricePeriods")
+    tiers_mode: Optional[TiersMode] = Field(alias="tiersMode")
 
 
 class PricingTypeFilterComparison(BaseModel):
     eq: Optional[PricingType]
     gt: Optional[PricingType]
     gte: Optional[PricingType]
     i_like: Optional[PricingType] = Field(alias="iLike")
@@ -2151,14 +2160,15 @@
     )
     billing_period: Optional["BillingPeriodFilterComparison"] = Field(
         alias="billingPeriod"
     )
     created_at: Optional["DateFieldComparison"] = Field(alias="createdAt")
     id: Optional["StringFieldComparison"]
     or_: Optional[List["SubscriptionAddonFilterPriceFilter"]] = Field(alias="or")
+    tiers_mode: Optional["TiersModeFilterComparison"] = Field(alias="tiersMode")
 
 
 class SubscriptionAddonInput(BaseModel):
     addon_id: str = Field(alias="addonId")
     quantity: Optional[int] = 1
 
 
@@ -2406,14 +2416,15 @@
     )
     billing_period: Optional["BillingPeriodFilterComparison"] = Field(
         alias="billingPeriod"
     )
     created_at: Optional["DateFieldComparison"] = Field(alias="createdAt")
     id: Optional["StringFieldComparison"]
     or_: Optional[List["SubscriptionPriceFilterPriceFilter"]] = Field(alias="or")
+    tiers_mode: Optional["TiersModeFilterComparison"] = Field(alias="tiersMode")
 
 
 class SubscriptionPriceSort(BaseModel):
     direction: SortDirection
     field: SubscriptionPriceSortFields
     nulls: Optional[SortNulls]
 
@@ -2486,14 +2497,31 @@
 
 class TestHookInput(BaseModel):
     endpoint_url: str = Field(alias="endpointUrl")
     environment_id: str = Field(alias="environmentId")
     hook_event_type: EventLogType = Field(alias="hookEventType")
 
 
+class TiersModeFilterComparison(BaseModel):
+    eq: Optional[TiersMode]
+    gt: Optional[TiersMode]
+    gte: Optional[TiersMode]
+    i_like: Optional[TiersMode] = Field(alias="iLike")
+    in_: Optional[List[TiersMode]] = Field(alias="in")
+    is_: Optional[bool] = Field(alias="is")
+    is_not: Optional[bool] = Field(alias="isNot")
+    like: Optional[TiersMode]
+    lt: Optional[TiersMode]
+    lte: Optional[TiersMode]
+    neq: Optional[TiersMode]
+    not_i_like: Optional[TiersMode] = Field(alias="notILike")
+    not_in: Optional[List[TiersMode]] = Field(alias="notIn")
+    not_like: Optional[TiersMode] = Field(alias="notLike")
+
+
 class TypographyConfigurationInput(BaseModel):
     body: Optional["FontVariantInput"]
     font_family: Optional[str] = Field(alias="fontFamily")
     h1: Optional["FontVariantInput"]
     h2: Optional["FontVariantInput"]
     h3: Optional["FontVariantInput"]
 
@@ -2965,14 +2993,15 @@
 PlanFilterProductFilter.update_forward_refs()
 PlanSort.update_forward_refs()
 PlanUpdateInput.update_forward_refs()
 PriceFilter.update_forward_refs()
 PriceFilterPackageDTOFilter.update_forward_refs()
 PricePeriodInput.update_forward_refs()
 PriceSort.update_forward_refs()
+PriceTierInput.update_forward_refs()
 PricingModelCreateInput.update_forward_refs()
 PricingTypeFilterComparison.update_forward_refs()
 ProductCreateInput.update_forward_refs()
 ProductFilter.update_forward_refs()
 ProductSettingsInput.update_forward_refs()
 ProductSort.update_forward_refs()
 ProductUpdateInput.update_forward_refs()
@@ -3033,14 +3062,15 @@
 SubscriptionStatusFilterComparison.update_forward_refs()
 SubscriptionUpdateScheduleCancellationInput.update_forward_refs()
 SyncTaxRatesInput.update_forward_refs()
 TaskStatusFilterComparison.update_forward_refs()
 TaskTypeFilterComparison.update_forward_refs()
 TaxExempt.update_forward_refs()
 TestHookInput.update_forward_refs()
+TiersModeFilterComparison.update_forward_refs()
 TypographyConfigurationInput.update_forward_refs()
 UpdateAccountInput.update_forward_refs()
 UpdateCouponInput.update_forward_refs()
 UpdateCustomerInput.update_forward_refs()
 UpdateExperimentInput.update_forward_refs()
 UpdateFeature.update_forward_refs()
 UpdateFeatureInput.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.524.0/stigg/generated/migrate_subscription_to_latest.py` & `stigg_api_client_v2-0.526.0/stigg/generated/migrate_subscription_to_latest.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-06 07:36
+# Generated by ariadne-codegen on 2023-08-07 15:02
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.524.0/stigg/generated/provision_customer.py` & `stigg_api_client_v2-0.526.0/stigg/generated/provision_customer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-06 07:36
+# Generated by ariadne-codegen on 2023-08-07 15:02
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.524.0/stigg/generated/provision_subscription.py` & `stigg_api_client_v2-0.526.0/stigg/generated/provision_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-06 07:36
+# Generated by ariadne-codegen on 2023-08-07 15:02
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.524.0/stigg/generated/report_usage.py` & `stigg_api_client_v2-0.526.0/stigg/generated/report_usage.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-08-06 07:36
+# Generated by ariadne-codegen on 2023-08-07 15:02
 # Source: operations.graphql
 
 from typing import Any, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.524.0/PKG-INFO` & `stigg_api_client_v2-0.526.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stigg-api-client-v2
-Version: 0.524.0
+Version: 0.526.0
 Summary: 
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

