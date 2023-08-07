# Comparing `tmp/stigg_api_client-0.524.0.tar.gz` & `tmp/stigg_api_client-0.526.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_api_client-0.524.0.tar", max compression
+gzip compressed data, was "stigg_api_client-0.526.0.tar", max compression
```

## Comparing `stigg_api_client-0.524.0.tar` & `stigg_api_client-0.526.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2479 2023-08-06 07:35:27.692868 stigg_api_client-0.524.0/README.md
--rw-r--r--   0        0        0      480 2023-08-06 07:36:11.481242 stigg_api_client-0.524.0/pyproject.toml
--rw-r--r--   0        0        0       44 2023-08-06 07:35:27.692868 stigg_api_client-0.524.0/stigg/__init__.py
--rw-r--r--   0        0        0     3699 2023-08-06 07:35:27.692868 stigg_api_client-0.524.0/stigg/client.py
--rw-r--r--   0        0        0        0 2023-08-06 07:36:08.997218 stigg_api_client-0.524.0/stigg/generated/__init__.py
--rw-r--r--   0        0        0    51059 2023-08-06 07:36:09.537223 stigg_api_client-0.524.0/stigg/generated/operations.py
--rw-r--r--   0        0        0   471395 2023-08-06 07:36:09.329221 stigg_api_client-0.524.0/stigg/generated/schema.py
--rw-r--r--   0        0        0     3122 1970-01-01 00:00:00.000000 stigg_api_client-0.524.0/PKG-INFO
+-rw-r--r--   0        0        0     2479 2023-08-07 15:01:28.359433 stigg_api_client-0.526.0/README.md
+-rw-r--r--   0        0        0      480 2023-08-07 15:02:15.379748 stigg_api_client-0.526.0/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-08-07 15:01:28.359433 stigg_api_client-0.526.0/stigg/__init__.py
+-rw-r--r--   0        0        0     3699 2023-08-07 15:01:28.359433 stigg_api_client-0.526.0/stigg/client.py
+-rw-r--r--   0        0        0        0 2023-08-07 15:02:12.839749 stigg_api_client-0.526.0/stigg/generated/__init__.py
+-rw-r--r--   0        0        0    51059 2023-08-07 15:02:13.395753 stigg_api_client-0.526.0/stigg/generated/operations.py
+-rw-r--r--   0        0        0   474475 2023-08-07 15:02:13.171751 stigg_api_client-0.526.0/stigg/generated/schema.py
+-rw-r--r--   0        0        0     3122 1970-01-01 00:00:00.000000 stigg_api_client-0.526.0/PKG-INFO
```

### Comparing `stigg_api_client-0.524.0/README.md` & `stigg_api_client-0.526.0/README.md`

 * *Files identical despite different names*

### Comparing `stigg_api_client-0.524.0/stigg/client.py` & `stigg_api_client-0.526.0/stigg/client.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client-0.524.0/stigg/generated/operations.py` & `stigg_api_client-0.526.0/stigg/generated/operations.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client-0.524.0/stigg/generated/schema.py` & `stigg_api_client-0.526.0/stigg/generated/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -271,15 +271,15 @@
 class PlanSortFields(sgqlc.types.Enum):
     __schema__ = schema
     __choices__ = ('billingId', 'createdAt', 'description', 'displayName', 'environmentId', 'id', 'isLatest', 'pricingType', 'productId', 'refId', 'status', 'updatedAt', 'versionNumber')
 
 
 class PriceSortFields(sgqlc.types.Enum):
     __schema__ = schema
-    __choices__ = ('billingId', 'billingModel', 'billingPeriod', 'createdAt', 'id')
+    __choices__ = ('billingId', 'billingModel', 'billingPeriod', 'createdAt', 'id', 'tiersMode')
 
 
 class PricingType(sgqlc.types.Enum):
     __schema__ = schema
     __choices__ = ('CUSTOM', 'FREE', 'PAID')
 
 
@@ -416,14 +416,19 @@
 
 
 class TaskType(sgqlc.types.Enum):
     __schema__ = schema
     __choices__ = ('IMPORT_INTEGRATION_CATALOG', 'IMPORT_INTEGRATION_CUSTOMERS', 'IMPORT_SUBSCRIPTIONS_BULK', 'RECALCULATE_ENTITLEMENTS', 'RESYNC_INTEGRATION', 'SUBSCRIPTION_MIGRATION')
 
 
+class TiersMode(sgqlc.types.Enum):
+    __schema__ = schema
+    __choices__ = ('GRADUATED', 'VOLUME')
+
+
 class TrialPeriodUnits(sgqlc.types.Enum):
     __schema__ = schema
     __choices__ = ('DAY', 'MONTH')
 
 
 class UsageMeasurementSortFields(sgqlc.types.Enum):
     __schema__ = schema
@@ -2168,23 +2173,24 @@
     id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='id')
     parent_plan_id = sgqlc.types.Field(String, graphql_name='parentPlanId')
     status = sgqlc.types.Field(PackageStatus, graphql_name='status')
 
 
 class PriceFilter(sgqlc.types.Input):
     __schema__ = schema
-    __field_names__ = ('and_', 'billing_id', 'billing_model', 'billing_period', 'created_at', 'id', 'or_', 'package')
+    __field_names__ = ('and_', 'billing_id', 'billing_model', 'billing_period', 'created_at', 'id', 'or_', 'package', 'tiers_mode')
     and_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('PriceFilter')), graphql_name='and')
     billing_id = sgqlc.types.Field('StringFieldComparison', graphql_name='billingId')
     billing_model = sgqlc.types.Field(BillingModelFilterComparison, graphql_name='billingModel')
     billing_period = sgqlc.types.Field(BillingPeriodFilterComparison, graphql_name='billingPeriod')
     created_at = sgqlc.types.Field(DateFieldComparison, graphql_name='createdAt')
     id = sgqlc.types.Field('StringFieldComparison', graphql_name='id')
     or_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('PriceFilter')), graphql_name='or')
     package = sgqlc.types.Field('PriceFilterPackageDTOFilter', graphql_name='package')
+    tiers_mode = sgqlc.types.Field('TiersModeFilterComparison', graphql_name='tiersMode')
 
 
 class PriceFilterPackageDTOFilter(sgqlc.types.Input):
     __schema__ = schema
     __field_names__ = ('and_', 'billing_id', 'created_at', 'description', 'display_name', 'environment_id', 'id', 'is_latest', 'or_', 'pricing_type', 'product_id', 'ref_id', 'status', 'updated_at', 'version_number')
     and_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('PriceFilterPackageDTOFilter')), graphql_name='and')
     billing_id = sgqlc.types.Field('StringFieldComparison', graphql_name='billingId')
@@ -2201,36 +2207,45 @@
     status = sgqlc.types.Field(PackageStatusFilterComparison, graphql_name='status')
     updated_at = sgqlc.types.Field(DateFieldComparison, graphql_name='updatedAt')
     version_number = sgqlc.types.Field(IntFieldComparison, graphql_name='versionNumber')
 
 
 class PricePeriodInput(sgqlc.types.Input):
     __schema__ = schema
-    __field_names__ = ('billing_country_code', 'billing_period', 'price')
+    __field_names__ = ('billing_country_code', 'billing_period', 'price', 'tiers')
     billing_country_code = sgqlc.types.Field(String, graphql_name='billingCountryCode')
     billing_period = sgqlc.types.Field(sgqlc.types.non_null(BillingPeriod), graphql_name='billingPeriod')
-    price = sgqlc.types.Field(sgqlc.types.non_null(MoneyInputDTO), graphql_name='price')
+    price = sgqlc.types.Field(MoneyInputDTO, graphql_name='price')
+    tiers = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('PriceTierInput')), graphql_name='tiers')
 
 
 class PriceSort(sgqlc.types.Input):
     __schema__ = schema
     __field_names__ = ('direction', 'field', 'nulls')
     direction = sgqlc.types.Field(sgqlc.types.non_null(SortDirection), graphql_name='direction')
     field = sgqlc.types.Field(sgqlc.types.non_null(PriceSortFields), graphql_name='field')
     nulls = sgqlc.types.Field(SortNulls, graphql_name='nulls')
 
 
+class PriceTierInput(sgqlc.types.Input):
+    __schema__ = schema
+    __field_names__ = ('unit_price', 'up_to')
+    unit_price = sgqlc.types.Field(sgqlc.types.non_null(MoneyInputDTO), graphql_name='unitPrice')
+    up_to = sgqlc.types.Field(sgqlc.types.non_null(Float), graphql_name='upTo')
+
+
 class PricingModelCreateInput(sgqlc.types.Input):
     __schema__ = schema
-    __field_names__ = ('billing_model', 'feature_id', 'max_unit_quantity', 'min_unit_quantity', 'price_periods')
+    __field_names__ = ('billing_model', 'feature_id', 'max_unit_quantity', 'min_unit_quantity', 'price_periods', 'tiers_mode')
     billing_model = sgqlc.types.Field(sgqlc.types.non_null(BillingModel), graphql_name='billingModel')
     feature_id = sgqlc.types.Field(String, graphql_name='featureId')
     max_unit_quantity = sgqlc.types.Field(Float, graphql_name='maxUnitQuantity')
     min_unit_quantity = sgqlc.types.Field(Float, graphql_name='minUnitQuantity')
     price_periods = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(PricePeriodInput))), graphql_name='pricePeriods')
+    tiers_mode = sgqlc.types.Field(TiersMode, graphql_name='tiersMode')
 
 
 class PricingTypeFilterComparison(sgqlc.types.Input):
     __schema__ = schema
     __field_names__ = ('eq', 'gt', 'gte', 'i_like', 'in_', 'is_', 'is_not', 'like', 'lt', 'lte', 'neq', 'not_ilike', 'not_in', 'not_like')
     eq = sgqlc.types.Field(PricingType, graphql_name='eq')
     gt = sgqlc.types.Field(PricingType, graphql_name='gt')
@@ -2703,22 +2718,23 @@
     status = sgqlc.types.Field('SubscriptionStatusFilterComparison', graphql_name='status')
     subscription_id = sgqlc.types.Field(StringFieldComparison, graphql_name='subscriptionId')
     trial_end_date = sgqlc.types.Field(DateFieldComparison, graphql_name='trialEndDate')
 
 
 class SubscriptionAddonFilterPriceFilter(sgqlc.types.Input):
     __schema__ = schema
-    __field_names__ = ('and_', 'billing_id', 'billing_model', 'billing_period', 'created_at', 'id', 'or_')
+    __field_names__ = ('and_', 'billing_id', 'billing_model', 'billing_period', 'created_at', 'id', 'or_', 'tiers_mode')
     and_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('SubscriptionAddonFilterPriceFilter')), graphql_name='and')
     billing_id = sgqlc.types.Field(StringFieldComparison, graphql_name='billingId')
     billing_model = sgqlc.types.Field(BillingModelFilterComparison, graphql_name='billingModel')
     billing_period = sgqlc.types.Field(BillingPeriodFilterComparison, graphql_name='billingPeriod')
     created_at = sgqlc.types.Field(DateFieldComparison, graphql_name='createdAt')
     id = sgqlc.types.Field(StringFieldComparison, graphql_name='id')
     or_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('SubscriptionAddonFilterPriceFilter')), graphql_name='or')
+    tiers_mode = sgqlc.types.Field('TiersModeFilterComparison', graphql_name='tiersMode')
 
 
 class SubscriptionAddonInput(sgqlc.types.Input):
     __schema__ = schema
     __field_names__ = ('addon_id', 'quantity')
     addon_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='addonId')
     quantity = sgqlc.types.Field(Int, graphql_name='quantity')
@@ -2940,22 +2956,23 @@
     status = sgqlc.types.Field('SubscriptionStatusFilterComparison', graphql_name='status')
     subscription_id = sgqlc.types.Field(StringFieldComparison, graphql_name='subscriptionId')
     trial_end_date = sgqlc.types.Field(DateFieldComparison, graphql_name='trialEndDate')
 
 
 class SubscriptionPriceFilterPriceFilter(sgqlc.types.Input):
     __schema__ = schema
-    __field_names__ = ('and_', 'billing_id', 'billing_model', 'billing_period', 'created_at', 'id', 'or_')
+    __field_names__ = ('and_', 'billing_id', 'billing_model', 'billing_period', 'created_at', 'id', 'or_', 'tiers_mode')
     and_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('SubscriptionPriceFilterPriceFilter')), graphql_name='and')
     billing_id = sgqlc.types.Field(StringFieldComparison, graphql_name='billingId')
     billing_model = sgqlc.types.Field(BillingModelFilterComparison, graphql_name='billingModel')
     billing_period = sgqlc.types.Field(BillingPeriodFilterComparison, graphql_name='billingPeriod')
     created_at = sgqlc.types.Field(DateFieldComparison, graphql_name='createdAt')
     id = sgqlc.types.Field(StringFieldComparison, graphql_name='id')
     or_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('SubscriptionPriceFilterPriceFilter')), graphql_name='or')
+    tiers_mode = sgqlc.types.Field('TiersModeFilterComparison', graphql_name='tiersMode')
 
 
 class SubscriptionPriceSort(sgqlc.types.Input):
     __schema__ = schema
     __field_names__ = ('direction', 'field', 'nulls')
     direction = sgqlc.types.Field(sgqlc.types.non_null(SortDirection), graphql_name='direction')
     field = sgqlc.types.Field(sgqlc.types.non_null(SubscriptionPriceSortFields), graphql_name='field')
@@ -3044,14 +3061,33 @@
     __schema__ = schema
     __field_names__ = ('endpoint_url', 'environment_id', 'hook_event_type')
     endpoint_url = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='endpointUrl')
     environment_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='environmentId')
     hook_event_type = sgqlc.types.Field(sgqlc.types.non_null(EventLogType), graphql_name='hookEventType')
 
 
+class TiersModeFilterComparison(sgqlc.types.Input):
+    __schema__ = schema
+    __field_names__ = ('eq', 'gt', 'gte', 'i_like', 'in_', 'is_', 'is_not', 'like', 'lt', 'lte', 'neq', 'not_ilike', 'not_in', 'not_like')
+    eq = sgqlc.types.Field(TiersMode, graphql_name='eq')
+    gt = sgqlc.types.Field(TiersMode, graphql_name='gt')
+    gte = sgqlc.types.Field(TiersMode, graphql_name='gte')
+    i_like = sgqlc.types.Field(TiersMode, graphql_name='iLike')
+    in_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(TiersMode)), graphql_name='in')
+    is_ = sgqlc.types.Field(Boolean, graphql_name='is')
+    is_not = sgqlc.types.Field(Boolean, graphql_name='isNot')
+    like = sgqlc.types.Field(TiersMode, graphql_name='like')
+    lt = sgqlc.types.Field(TiersMode, graphql_name='lt')
+    lte = sgqlc.types.Field(TiersMode, graphql_name='lte')
+    neq = sgqlc.types.Field(TiersMode, graphql_name='neq')
+    not_ilike = sgqlc.types.Field(TiersMode, graphql_name='notILike')
+    not_in = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(TiersMode)), graphql_name='notIn')
+    not_like = sgqlc.types.Field(TiersMode, graphql_name='notLike')
+
+
 class TypographyConfigurationInput(sgqlc.types.Input):
     __schema__ = schema
     __field_names__ = ('body', 'font_family', 'h1', 'h2', 'h3')
     body = sgqlc.types.Field(FontVariantInput, graphql_name='body')
     font_family = sgqlc.types.Field(String, graphql_name='fontFamily')
     h1 = sgqlc.types.Field(FontVariantInput, graphql_name='h1')
     h2 = sgqlc.types.Field(FontVariantInput, graphql_name='h2')
@@ -6118,15 +6154,15 @@
     __schema__ = schema
     __field_names__ = ('version_number',)
     version_number = sgqlc.types.Field(Float, graphql_name='versionNumber')
 
 
 class Price(sgqlc.types.Type):
     __schema__ = schema
-    __field_names__ = ('billing_country_code', 'billing_id', 'billing_model', 'billing_period', 'created_at', 'crm_id', 'crm_link_url', 'feature', 'feature_id', 'id', 'max_unit_quantity', 'min_unit_quantity', 'package', 'package_id', 'price', 'used_in_subscriptions')
+    __field_names__ = ('billing_country_code', 'billing_id', 'billing_model', 'billing_period', 'created_at', 'crm_id', 'crm_link_url', 'feature', 'feature_id', 'id', 'max_unit_quantity', 'min_unit_quantity', 'package', 'package_id', 'price', 'tiers', 'tiers_mode', 'used_in_subscriptions')
     billing_country_code = sgqlc.types.Field(String, graphql_name='billingCountryCode')
     billing_id = sgqlc.types.Field(String, graphql_name='billingId')
     billing_model = sgqlc.types.Field(sgqlc.types.non_null(BillingModel), graphql_name='billingModel')
     billing_period = sgqlc.types.Field(sgqlc.types.non_null(BillingPeriod), graphql_name='billingPeriod')
     created_at = sgqlc.types.Field(DateTime, graphql_name='createdAt')
     crm_id = sgqlc.types.Field(String, graphql_name='crmId')
     crm_link_url = sgqlc.types.Field(String, graphql_name='crmLinkUrl')
@@ -6134,54 +6170,60 @@
     feature_id = sgqlc.types.Field(String, graphql_name='featureId')
     id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='id')
     max_unit_quantity = sgqlc.types.Field(Float, graphql_name='maxUnitQuantity')
     min_unit_quantity = sgqlc.types.Field(Float, graphql_name='minUnitQuantity')
     package = sgqlc.types.Field(sgqlc.types.non_null(PackageDTO), graphql_name='package')
     package_id = sgqlc.types.Field(String, graphql_name='packageId')
     price = sgqlc.types.Field(sgqlc.types.non_null(Money), graphql_name='price')
+    tiers = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('PriceTier')), graphql_name='tiers')
+    tiers_mode = sgqlc.types.Field(TiersMode, graphql_name='tiersMode')
     used_in_subscriptions = sgqlc.types.Field(Boolean, graphql_name='usedInSubscriptions')
 
 
 class PriceAggregateGroupBy(sgqlc.types.Type):
     __schema__ = schema
-    __field_names__ = ('billing_id', 'billing_model', 'billing_period', 'created_at', 'id')
+    __field_names__ = ('billing_id', 'billing_model', 'billing_period', 'created_at', 'id', 'tiers_mode')
     billing_id = sgqlc.types.Field(String, graphql_name='billingId')
     billing_model = sgqlc.types.Field(BillingModel, graphql_name='billingModel')
     billing_period = sgqlc.types.Field(BillingPeriod, graphql_name='billingPeriod')
     created_at = sgqlc.types.Field(DateTime, graphql_name='createdAt')
     id = sgqlc.types.Field(String, graphql_name='id')
+    tiers_mode = sgqlc.types.Field(TiersMode, graphql_name='tiersMode')
 
 
 class PriceCountAggregate(sgqlc.types.Type):
     __schema__ = schema
-    __field_names__ = ('billing_id', 'billing_model', 'billing_period', 'created_at', 'id')
+    __field_names__ = ('billing_id', 'billing_model', 'billing_period', 'created_at', 'id', 'tiers_mode')
     billing_id = sgqlc.types.Field(Int, graphql_name='billingId')
     billing_model = sgqlc.types.Field(Int, graphql_name='billingModel')
     billing_period = sgqlc.types.Field(Int, graphql_name='billingPeriod')
     created_at = sgqlc.types.Field(Int, graphql_name='createdAt')
     id = sgqlc.types.Field(Int, graphql_name='id')
+    tiers_mode = sgqlc.types.Field(Int, graphql_name='tiersMode')
 
 
 class PriceDeleteResponse(sgqlc.types.Type):
     __schema__ = schema
-    __field_names__ = ('billing_country_code', 'billing_id', 'billing_model', 'billing_period', 'created_at', 'crm_id', 'crm_link_url', 'feature', 'feature_id', 'id', 'max_unit_quantity', 'min_unit_quantity', 'package_id', 'price', 'used_in_subscriptions')
+    __field_names__ = ('billing_country_code', 'billing_id', 'billing_model', 'billing_period', 'created_at', 'crm_id', 'crm_link_url', 'feature', 'feature_id', 'id', 'max_unit_quantity', 'min_unit_quantity', 'package_id', 'price', 'tiers', 'tiers_mode', 'used_in_subscriptions')
     billing_country_code = sgqlc.types.Field(String, graphql_name='billingCountryCode')
     billing_id = sgqlc.types.Field(String, graphql_name='billingId')
     billing_model = sgqlc.types.Field(BillingModel, graphql_name='billingModel')
     billing_period = sgqlc.types.Field(BillingPeriod, graphql_name='billingPeriod')
     created_at = sgqlc.types.Field(DateTime, graphql_name='createdAt')
     crm_id = sgqlc.types.Field(String, graphql_name='crmId')
     crm_link_url = sgqlc.types.Field(String, graphql_name='crmLinkUrl')
     feature = sgqlc.types.Field(Feature, graphql_name='feature')
     feature_id = sgqlc.types.Field(String, graphql_name='featureId')
     id = sgqlc.types.Field(String, graphql_name='id')
     max_unit_quantity = sgqlc.types.Field(Float, graphql_name='maxUnitQuantity')
     min_unit_quantity = sgqlc.types.Field(Float, graphql_name='minUnitQuantity')
     package_id = sgqlc.types.Field(String, graphql_name='packageId')
     price = sgqlc.types.Field(Money, graphql_name='price')
+    tiers = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('PriceTier')), graphql_name='tiers')
+    tiers_mode = sgqlc.types.Field(TiersMode, graphql_name='tiersMode')
     used_in_subscriptions = sgqlc.types.Field(Boolean, graphql_name='usedInSubscriptions')
 
 
 class PriceEdge(sgqlc.types.Type):
     __schema__ = schema
     __field_names__ = ('cursor', 'node')
     cursor = sgqlc.types.Field(sgqlc.types.non_null(ConnectionCursor), graphql_name='cursor')
@@ -6201,39 +6243,48 @@
     reset_period_configuration = sgqlc.types.Field('ResetPeriodConfiguration', graphql_name='resetPeriodConfiguration')
     updated_at = sgqlc.types.Field(DateTime, graphql_name='updatedAt')
     usage_limit = sgqlc.types.Field(Float, graphql_name='usageLimit')
 
 
 class PriceMaxAggregate(sgqlc.types.Type):
     __schema__ = schema
-    __field_names__ = ('billing_id', 'billing_model', 'billing_period', 'created_at', 'id')
+    __field_names__ = ('billing_id', 'billing_model', 'billing_period', 'created_at', 'id', 'tiers_mode')
     billing_id = sgqlc.types.Field(String, graphql_name='billingId')
     billing_model = sgqlc.types.Field(BillingModel, graphql_name='billingModel')
     billing_period = sgqlc.types.Field(BillingPeriod, graphql_name='billingPeriod')
     created_at = sgqlc.types.Field(DateTime, graphql_name='createdAt')
     id = sgqlc.types.Field(String, graphql_name='id')
+    tiers_mode = sgqlc.types.Field(TiersMode, graphql_name='tiersMode')
 
 
 class PriceMinAggregate(sgqlc.types.Type):
     __schema__ = schema
-    __field_names__ = ('billing_id', 'billing_model', 'billing_period', 'created_at', 'id')
+    __field_names__ = ('billing_id', 'billing_model', 'billing_period', 'created_at', 'id', 'tiers_mode')
     billing_id = sgqlc.types.Field(String, graphql_name='billingId')
     billing_model = sgqlc.types.Field(BillingModel, graphql_name='billingModel')
     billing_period = sgqlc.types.Field(BillingPeriod, graphql_name='billingPeriod')
     created_at = sgqlc.types.Field(DateTime, graphql_name='createdAt')
     id = sgqlc.types.Field(String, graphql_name='id')
+    tiers_mode = sgqlc.types.Field(TiersMode, graphql_name='tiersMode')
 
 
 class PriceNotFoundError(sgqlc.types.Type):
     __schema__ = schema
     __field_names__ = ('code', 'is_validation_error')
     code = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='code')
     is_validation_error = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='isValidationError')
 
 
+class PriceTier(sgqlc.types.Type):
+    __schema__ = schema
+    __field_names__ = ('unit_price', 'up_to')
+    unit_price = sgqlc.types.Field(sgqlc.types.non_null(Money), graphql_name='unitPrice')
+    up_to = sgqlc.types.Field(sgqlc.types.non_null(Float), graphql_name='upTo')
+
+
 class PricingTypeChange(sgqlc.types.Type):
     __schema__ = schema
     __field_names__ = ('after', 'before', 'change_type')
     after = sgqlc.types.Field(PricingType, graphql_name='after')
     before = sgqlc.types.Field(PricingType, graphql_name='before')
     change_type = sgqlc.types.Field(ChangeType, graphql_name='changeType')
```

### Comparing `stigg_api_client-0.524.0/PKG-INFO` & `stigg_api_client-0.526.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stigg-api-client
-Version: 0.524.0
+Version: 0.526.0
 Summary: 
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

