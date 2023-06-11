# Comparing `tmp/stigg_api_client_v2-0.460.0.tar.gz` & `tmp/stigg_api_client_v2-0.461.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_api_client_v2-0.460.0.tar", max compression
+gzip compressed data, was "stigg_api_client_v2-0.461.2.tar", max compression
```

## Comparing `stigg_api_client_v2-0.460.0.tar` & `stigg_api_client_v2-0.461.2.tar`

### file list

```diff
@@ -1,42 +1,41 @@
--rw-r--r--   0        0        0     1644 2023-06-11 06:22:38.788101 stigg_api_client_v2-0.460.0/README.md
--rw-r--r--   0        0        0      653 2023-06-11 06:23:28.380972 stigg_api_client_v2-0.460.0/pyproject.toml
--rw-r--r--   0        0        0       44 2023-06-11 06:22:38.788101 stigg_api_client_v2-0.460.0/stigg/__init__.py
--rw-r--r--   0        0        0      363 2023-06-11 06:22:38.788101 stigg_api_client_v2-0.460.0/stigg/client.py
--rw-r--r--   0        0        0    39496 2023-06-11 06:23:26.384939 stigg_api_client_v2-0.460.0/stigg/generated/__init__.py
--rw-r--r--   0        0        0     7303 2023-06-11 06:23:26.008932 stigg_api_client_v2-0.460.0/stigg/generated/async_base_client.py
--rw-r--r--   0        0        0     1951 2023-06-11 06:23:26.008932 stigg_api_client_v2-0.460.0/stigg/generated/base_model.py
--rw-r--r--   0        0        0      527 2023-06-11 06:23:24.980915 stigg_api_client_v2-0.460.0/stigg/generated/cancel_subscription.py
--rw-r--r--   0        0        0      296 2023-06-11 06:23:25.008916 stigg_api_client_v2-0.460.0/stigg/generated/cancel_subscription_updates.py
--rw-r--r--   0        0        0    69448 2023-06-11 06:23:26.228936 stigg_api_client_v2-0.460.0/stigg/generated/client.py
--rw-r--r--   0        0        0      527 2023-06-11 06:23:25.028916 stigg_api_client_v2-0.460.0/stigg/generated/create_subscription.py
--rw-r--r--   0        0        0      541 2023-06-11 06:23:25.112917 stigg_api_client_v2-0.460.0/stigg/generated/entitlements_updated.py
--rw-r--r--   0        0        0    23730 2023-06-11 06:23:22.468873 stigg_api_client_v2-0.460.0/stigg/generated/enums.py
--rw-r--r--   0        0        0      553 2023-06-11 06:23:24.996915 stigg_api_client_v2-0.460.0/stigg/generated/estimate_subscription.py
--rw-r--r--   0        0        0      614 2023-06-11 06:23:25.004915 stigg_api_client_v2-0.460.0/stigg/generated/estimate_subscription_update.py
--rw-r--r--   0        0        0     2366 2023-06-11 06:23:26.008932 stigg_api_client_v2-0.460.0/stigg/generated/exceptions.py
--rw-r--r--   0        0        0    53088 2023-06-11 06:23:26.008932 stigg_api_client_v2-0.460.0/stigg/generated/fragments.py
--rw-r--r--   0        0        0      591 2023-06-11 06:23:25.048916 stigg_api_client_v2-0.460.0/stigg/generated/get_active_subscriptions.py
--rw-r--r--   0        0        0      634 2023-06-11 06:23:25.056916 stigg_api_client_v2-0.460.0/stigg/generated/get_coupons.py
--rw-r--r--   0        0        0      572 2023-06-11 06:23:25.044916 stigg_api_client_v2-0.460.0/stigg/generated/get_customer_by_id.py
--rw-r--r--   0        0        0      533 2023-06-11 06:23:25.096917 stigg_api_client_v2-0.460.0/stigg/generated/get_customer_portal_by_ref_id.py
--rw-r--r--   0        0        0      390 2023-06-11 06:23:25.072917 stigg_api_client_v2-0.460.0/stigg/generated/get_entitlement.py
--rw-r--r--   0        0        0      430 2023-06-11 06:23:25.068916 stigg_api_client_v2-0.460.0/stigg/generated/get_entitlements.py
--rw-r--r--   0        0        0      893 2023-06-11 06:23:25.104917 stigg_api_client_v2-0.460.0/stigg/generated/get_mock_paywall.py
--rw-r--r--   0        0        0      346 2023-06-11 06:23:25.064916 stigg_api_client_v2-0.460.0/stigg/generated/get_paywall.py
--rw-r--r--   0        0        0      657 2023-06-11 06:23:25.084917 stigg_api_client_v2-0.460.0/stigg/generated/get_products.py
--rw-r--r--   0        0        0      650 2023-06-11 06:23:25.092917 stigg_api_client_v2-0.460.0/stigg/generated/get_sdk_configuration.py
--rw-r--r--   0        0        0      465 2023-06-11 06:23:24.948914 stigg_api_client_v2-0.460.0/stigg/generated/import_customer.py
--rw-r--r--   0        0        0      332 2023-06-11 06:23:24.940914 stigg_api_client_v2-0.460.0/stigg/generated/import_customer_bulk.py
--rw-r--r--   0        0        0      350 2023-06-11 06:23:24.968915 stigg_api_client_v2-0.460.0/stigg/generated/import_subscriptions_bulk.py
--rw-r--r--   0        0        0      550 2023-06-11 06:23:24.988915 stigg_api_client_v2-0.460.0/stigg/generated/initiate_checkout.py
--rw-r--r--   0        0        0   126306 2023-06-11 06:23:24.924914 stigg_api_client_v2-0.460.0/stigg/generated/input_types.py
--rw-r--r--   0        0        0      604 2023-06-11 06:23:25.036916 stigg_api_client_v2-0.460.0/stigg/generated/migrate_subscription_to_latest.py
--rw-r--r--   0        0        0     1161 2023-06-11 06:23:24.936914 stigg_api_client_v2-0.460.0/stigg/generated/provision_customer.py
--rw-r--r--   0        0        0      971 2023-06-11 06:23:24.964915 stigg_api_client_v2-0.460.0/stigg/generated/provision_subscription.py
--rw-r--r--   0        0        0      359 2023-06-11 06:23:25.024916 stigg_api_client_v2-0.460.0/stigg/generated/report_entitlement_check_requested.py
--rw-r--r--   0        0        0      637 2023-06-11 06:23:25.016916 stigg_api_client_v2-0.460.0/stigg/generated/report_usage.py
--rw-r--r--   0        0        0      220 2023-06-11 06:23:26.012932 stigg_api_client_v2-0.460.0/stigg/generated/scalars.py
--rw-r--r--   0        0        0      465 2023-06-11 06:23:24.952915 stigg_api_client_v2-0.460.0/stigg/generated/update_customer.py
--rw-r--r--   0        0        0      527 2023-06-11 06:23:24.976915 stigg_api_client_v2-0.460.0/stigg/generated/update_subscription.py
--rw-r--r--   0        0        0      451 2023-06-11 06:23:25.120917 stigg_api_client_v2-0.460.0/stigg/generated/usage_updated.py
--rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.460.0/PKG-INFO
+-rw-r--r--   0        0        0     1644 2023-06-11 15:33:37.053950 stigg_api_client_v2-0.461.2/README.md
+-rw-r--r--   0        0        0      653 2023-06-11 15:34:17.538161 stigg_api_client_v2-0.461.2/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-06-11 15:33:37.053950 stigg_api_client_v2-0.461.2/stigg/__init__.py
+-rw-r--r--   0        0        0      363 2023-06-11 15:33:37.053950 stigg_api_client_v2-0.461.2/stigg/client.py
+-rw-r--r--   0        0        0    39294 2023-06-11 15:34:15.654152 stigg_api_client_v2-0.461.2/stigg/generated/__init__.py
+-rw-r--r--   0        0        0     7303 2023-06-11 15:34:15.282150 stigg_api_client_v2-0.461.2/stigg/generated/async_base_client.py
+-rw-r--r--   0        0        0     1951 2023-06-11 15:34:15.282150 stigg_api_client_v2-0.461.2/stigg/generated/base_model.py
+-rw-r--r--   0        0        0      527 2023-06-11 15:34:14.286145 stigg_api_client_v2-0.461.2/stigg/generated/cancel_subscription.py
+-rw-r--r--   0        0        0      296 2023-06-11 15:34:14.306146 stigg_api_client_v2-0.461.2/stigg/generated/cancel_subscription_updates.py
+-rw-r--r--   0        0        0    68793 2023-06-11 15:34:15.502151 stigg_api_client_v2-0.461.2/stigg/generated/client.py
+-rw-r--r--   0        0        0      527 2023-06-11 15:34:14.322146 stigg_api_client_v2-0.461.2/stigg/generated/create_subscription.py
+-rw-r--r--   0        0        0      541 2023-06-11 15:34:14.418146 stigg_api_client_v2-0.461.2/stigg/generated/entitlements_updated.py
+-rw-r--r--   0        0        0    23730 2023-06-11 15:34:11.802134 stigg_api_client_v2-0.461.2/stigg/generated/enums.py
+-rw-r--r--   0        0        0      553 2023-06-11 15:34:14.294145 stigg_api_client_v2-0.461.2/stigg/generated/estimate_subscription.py
+-rw-r--r--   0        0        0      614 2023-06-11 15:34:14.302145 stigg_api_client_v2-0.461.2/stigg/generated/estimate_subscription_update.py
+-rw-r--r--   0        0        0     2366 2023-06-11 15:34:15.282150 stigg_api_client_v2-0.461.2/stigg/generated/exceptions.py
+-rw-r--r--   0        0        0    53088 2023-06-11 15:34:15.282150 stigg_api_client_v2-0.461.2/stigg/generated/fragments.py
+-rw-r--r--   0        0        0      591 2023-06-11 15:34:14.354146 stigg_api_client_v2-0.461.2/stigg/generated/get_active_subscriptions.py
+-rw-r--r--   0        0        0      634 2023-06-11 15:34:14.362146 stigg_api_client_v2-0.461.2/stigg/generated/get_coupons.py
+-rw-r--r--   0        0        0      572 2023-06-11 15:34:14.346146 stigg_api_client_v2-0.461.2/stigg/generated/get_customer_by_id.py
+-rw-r--r--   0        0        0      533 2023-06-11 15:34:14.402146 stigg_api_client_v2-0.461.2/stigg/generated/get_customer_portal_by_ref_id.py
+-rw-r--r--   0        0        0      390 2023-06-11 15:34:14.378146 stigg_api_client_v2-0.461.2/stigg/generated/get_entitlement.py
+-rw-r--r--   0        0        0      430 2023-06-11 15:34:14.374146 stigg_api_client_v2-0.461.2/stigg/generated/get_entitlements.py
+-rw-r--r--   0        0        0      893 2023-06-11 15:34:14.410146 stigg_api_client_v2-0.461.2/stigg/generated/get_mock_paywall.py
+-rw-r--r--   0        0        0      346 2023-06-11 15:34:14.366146 stigg_api_client_v2-0.461.2/stigg/generated/get_paywall.py
+-rw-r--r--   0        0        0      657 2023-06-11 15:34:14.386146 stigg_api_client_v2-0.461.2/stigg/generated/get_products.py
+-rw-r--r--   0        0        0      650 2023-06-11 15:34:14.394146 stigg_api_client_v2-0.461.2/stigg/generated/get_sdk_configuration.py
+-rw-r--r--   0        0        0      465 2023-06-11 15:34:14.254145 stigg_api_client_v2-0.461.2/stigg/generated/import_customer.py
+-rw-r--r--   0        0        0      332 2023-06-11 15:34:14.250145 stigg_api_client_v2-0.461.2/stigg/generated/import_customer_bulk.py
+-rw-r--r--   0        0        0      350 2023-06-11 15:34:14.274145 stigg_api_client_v2-0.461.2/stigg/generated/import_subscriptions_bulk.py
+-rw-r--r--   0        0        0   125303 2023-06-11 15:34:14.230145 stigg_api_client_v2-0.461.2/stigg/generated/input_types.py
+-rw-r--r--   0        0        0      604 2023-06-11 15:34:14.338146 stigg_api_client_v2-0.461.2/stigg/generated/migrate_subscription_to_latest.py
+-rw-r--r--   0        0        0     1161 2023-06-11 15:34:14.242145 stigg_api_client_v2-0.461.2/stigg/generated/provision_customer.py
+-rw-r--r--   0        0        0      971 2023-06-11 15:34:14.270145 stigg_api_client_v2-0.461.2/stigg/generated/provision_subscription.py
+-rw-r--r--   0        0        0      359 2023-06-11 15:34:14.318146 stigg_api_client_v2-0.461.2/stigg/generated/report_entitlement_check_requested.py
+-rw-r--r--   0        0        0      637 2023-06-11 15:34:14.314145 stigg_api_client_v2-0.461.2/stigg/generated/report_usage.py
+-rw-r--r--   0        0        0      220 2023-06-11 15:34:15.286150 stigg_api_client_v2-0.461.2/stigg/generated/scalars.py
+-rw-r--r--   0        0        0      465 2023-06-11 15:34:14.258145 stigg_api_client_v2-0.461.2/stigg/generated/update_customer.py
+-rw-r--r--   0        0        0      527 2023-06-11 15:34:14.282145 stigg_api_client_v2-0.461.2/stigg/generated/update_subscription.py
+-rw-r--r--   0        0        0      451 2023-06-11 15:34:14.422146 stigg_api_client_v2-0.461.2/stigg/generated/usage_updated.py
+-rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.461.2/PKG-INFO
```

### Comparing `stigg_api_client_v2-0.460.0/README.md` & `stigg_api_client_v2-0.461.2/README.md`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.460.0/pyproject.toml` & `stigg_api_client_v2-0.461.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stigg-api-client-v2"
-version = "0.460.0"
+version = "0.461.2"
 description = ""
 authors = ["Stigg <support@stigg.io>"]
 readme = "README.md"
 packages = [{ include = "stigg" }]
 include = ["stigg/generated/*"]
 
 [tool.poetry.dependencies]
```

### Comparing `stigg_api_client_v2-0.460.0/stigg/generated/__init__.py` & `stigg_api_client_v2-0.461.2/stigg/generated/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-11 06:23
+# Generated by ariadne-codegen on 2023-06-11 15:34
 
 from .async_base_client import AsyncBaseClient
 from .base_model import BaseModel
 from .cancel_subscription import (
     CancelSubscription,
     CancelSubscriptionCancelSubscription,
 )
@@ -322,15 +322,14 @@
 from .get_sdk_configuration import (
     GetSdkConfiguration,
     GetSdkConfigurationSdkConfiguration,
 )
 from .import_customer import ImportCustomer, ImportCustomerImportCustomer
 from .import_customer_bulk import ImportCustomerBulk
 from .import_subscriptions_bulk import ImportSubscriptionsBulk
-from .initiate_checkout import InitiateCheckout, InitiateCheckoutInitiateCheckout
 from .input_types import (
     AddCompatibleAddonsToPlanInput,
     AddonCreateInput,
     AddonFilter,
     AddonSort,
     AddonUpdateInput,
     Address,
@@ -436,15 +435,14 @@
     ImportIntegrationCatalogInput,
     ImportIntegrationCustomersInput,
     ImportIntegrationTaskFilter,
     ImportIntegrationTaskSort,
     ImportSubscriptionInput,
     ImportSubscriptionsBulk,
     InitAddStripeCustomerPaymentMethodInput,
-    InitiateCheckoutInput,
     IntegrationFilter,
     IntegrationSort,
     IntFieldComparison,
     IntFieldComparisonBetween,
     MemberFilter,
     MemberSort,
     MeterAggregation,
@@ -859,17 +857,14 @@
     "ImportIntegrationTaskFilter",
     "ImportIntegrationTaskSort",
     "ImportIntegrationTaskSortFields",
     "ImportSubscriptionInput",
     "ImportSubscriptionsBulk",
     "ImportSubscriptionsBulk",
     "InitAddStripeCustomerPaymentMethodInput",
-    "InitiateCheckout",
-    "InitiateCheckoutInitiateCheckout",
-    "InitiateCheckoutInput",
     "IntFieldComparison",
     "IntFieldComparisonBetween",
     "IntegrationFilter",
     "IntegrationSort",
     "IntegrationSortFields",
     "LayoutConfigurationFragment",
     "MemberFilter",
```

### Comparing `stigg_api_client_v2-0.460.0/stigg/generated/async_base_client.py` & `stigg_api_client_v2-0.461.2/stigg/generated/async_base_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-11 06:23
+# Generated by ariadne-codegen on 2023-06-11 15:34
 
 import enum
 import json
 from typing import Any, AsyncIterator, Dict, Optional, TypeVar, cast
 from uuid import uuid4
 
 import httpx
```

### Comparing `stigg_api_client_v2-0.460.0/stigg/generated/base_model.py` & `stigg_api_client_v2-0.461.2/stigg/generated/base_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-11 06:23
+# Generated by ariadne-codegen on 2023-06-11 15:34
 
 from typing import Any, Dict, Type, Union, get_args, get_origin
 
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic.class_validators import validator
 from pydantic.fields import ModelField
```

### Comparing `stigg_api_client_v2-0.460.0/stigg/generated/cancel_subscription.py` & `stigg_api_client_v2-0.461.2/stigg/generated/cancel_subscription.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-11 06:23
+# Generated by ariadne-codegen on 2023-06-11 15:34
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.460.0/stigg/generated/client.py` & `stigg_api_client_v2-0.461.2/stigg/generated/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-11 06:23
+# Generated by ariadne-codegen on 2023-06-11 15:34
 # Source: operations.graphql
 
 from typing import AsyncIterator
 
 from .async_base_client import AsyncBaseClient
 from .cancel_subscription import CancelSubscription
 from .cancel_subscription_updates import CancelSubscriptionUpdates
@@ -19,29 +19,27 @@
 from .get_mock_paywall import GetMockPaywall
 from .get_paywall import GetPaywall
 from .get_products import GetProducts
 from .get_sdk_configuration import GetSdkConfiguration
 from .import_customer import ImportCustomer
 from .import_customer_bulk import ImportCustomerBulk
 from .import_subscriptions_bulk import ImportSubscriptionsBulk
-from .initiate_checkout import InitiateCheckout
 from .input_types import (
     CustomerPortalInput,
     EntitlementCheckRequested,
     EstimateSubscriptionInput,
     EstimateSubscriptionUpdateInput,
     FetchEntitlementQuery,
     FetchEntitlementsQuery,
     GetActiveSubscriptionsInput,
     GetCustomerByRefIdInput,
     GetPaywallInput,
     ImportCustomerBulk,
     ImportCustomerInput,
     ImportSubscriptionsBulk,
-    InitiateCheckoutInput,
     ProvisionCustomerInput,
     ProvisionSubscriptionInput,
     SubscriptionCancellationInput,
     SubscriptionInput,
     SubscriptionMigrationInput,
     SubscriptionUpdateScheduleCancellationInput,
     UpdateCustomerInput,
@@ -546,30 +544,14 @@
             """
         )
         variables: dict[str, object] = {"input": input}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return CancelSubscription.parse_obj(data)
 
-    async def initiate_checkout(self, input: InitiateCheckoutInput) -> InitiateCheckout:
-        query = gql(
-            """
-            mutation InitiateCheckout($input: InitiateCheckoutInput!) {
-              initiateCheckout(input: $input) {
-                checkoutUrl
-                checkoutBillingId
-              }
-            }
-            """
-        )
-        variables: dict[str, object] = {"input": input}
-        response = await self.execute(query=query, variables=variables)
-        data = self.get_data(response)
-        return InitiateCheckout.parse_obj(data)
-
     async def estimate_subscription(
         self, input: EstimateSubscriptionInput
     ) -> EstimateSubscription:
         query = gql(
             """
             mutation EstimateSubscription($input: EstimateSubscriptionInput!) {
               estimateSubscription(input: $input) {
```

### Comparing `stigg_api_client_v2-0.460.0/stigg/generated/create_subscription.py` & `stigg_api_client_v2-0.461.2/stigg/generated/create_subscription.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-11 06:23
+# Generated by ariadne-codegen on 2023-06-11 15:34
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.460.0/stigg/generated/entitlements_updated.py` & `stigg_api_client_v2-0.461.2/stigg/generated/entitlements_updated.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-11 06:23
+# Generated by ariadne-codegen on 2023-06-11 15:34
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import EntitlementsUpdatedPayload
```

### Comparing `stigg_api_client_v2-0.460.0/stigg/generated/enums.py` & `stigg_api_client_v2-0.461.2/stigg/generated/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-11 06:23
+# Generated by ariadne-codegen on 2023-06-11 15:34
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from enum import Enum
 
 
 class AccessDeniedReason(str, Enum):
     CustomerNotFound = "CustomerNotFound"
```

### Comparing `stigg_api_client_v2-0.460.0/stigg/generated/estimate_subscription.py` & `stigg_api_client_v2-0.461.2/stigg/generated/estimate_subscription.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-11 06:23
+# Generated by ariadne-codegen on 2023-06-11 15:34
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.460.0/stigg/generated/estimate_subscription_update.py` & `stigg_api_client_v2-0.461.2/stigg/generated/estimate_subscription_update.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-11 06:23
+# Generated by ariadne-codegen on 2023-06-11 15:34
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.460.0/stigg/generated/exceptions.py` & `stigg_api_client_v2-0.461.2/stigg/generated/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-11 06:23
+# Generated by ariadne-codegen on 2023-06-11 15:34
 
 from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
 
 class GraphQLClientError(Exception):
```

### Comparing `stigg_api_client_v2-0.460.0/stigg/generated/fragments.py` & `stigg_api_client_v2-0.461.2/stigg/generated/fragments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-11 06:23
+# Generated by ariadne-codegen on 2023-06-11 15:34
 # Source: operations.graphql
 
 from typing import Annotated, Any, List, Literal, Optional, Union
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -124,14 +124,25 @@
     status: SyncStatus
 
 
 class CouponFragmentCustomers(BaseModel):
     id: str
 
 
+class SlimCustomerFragment(BaseModel):
+    id: str
+    name: Optional[str]
+    email: Optional[str]
+    created_at: Optional[Any] = Field(alias="createdAt")
+    updated_at: Any = Field(alias="updatedAt")
+    ref_id: str = Field(alias="refId")
+    billing_id: Optional[str] = Field(alias="billingId")
+    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
+
+
 class PromotionalEntitlementFragment(BaseModel):
     status: PromotionalEntitlementStatus
     usage_limit: Optional[float] = Field(alias="usageLimit")
     feature_id: str = Field(alias="featureId")
     has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
     reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
     end_date: Optional[Any] = Field(alias="endDate")
@@ -146,25 +157,14 @@
     feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
     ref_id: str = Field(alias="refId")
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
 
 
-class SlimCustomerFragment(BaseModel):
-    id: str
-    name: Optional[str]
-    email: Optional[str]
-    created_at: Optional[Any] = Field(alias="createdAt")
-    updated_at: Any = Field(alias="updatedAt")
-    ref_id: str = Field(alias="refId")
-    billing_id: Optional[str] = Field(alias="billingId")
-    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
-
-
 class CustomerFragment(SlimCustomerFragment):
     has_payment_method: bool = Field(alias="hasPaymentMethod")
     has_active_subscription: bool = Field(alias="hasActiveSubscription")
     default_payment_expiration_month: Optional[int] = Field(
         alias="defaultPaymentExpirationMonth"
     )
     default_payment_expiration_year: Optional[int] = Field(
@@ -328,19 +328,21 @@
     weekly_according_to: Optional[WeeklyAccordingTo] = Field(alias="weeklyAccordingTo")
 
 
 class CustomerPortalEntitlementFeature(FeatureFragment):
     pass
 
 
-class CustomerPortalSubscriptionAddon(BaseModel):
-    addon_id: str = Field(alias="addonId")
-    description: Optional[str]
+class CustomerPortalPromotionalEntitlement(BaseModel):
     display_name: str = Field(alias="displayName")
-    quantity: int
+    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
+    usage_limit: Optional[float] = Field(alias="usageLimit")
+    period: PromotionalEntitlementPeriod
+    start_date: Any = Field(alias="startDate")
+    end_date: Optional[Any] = Field(alias="endDate")
 
 
 class CustomerPortalSubscriptionScheduledUpdateData(BaseModel):
     subscription_schedule_type: SubscriptionScheduleType = Field(
         alias="subscriptionScheduleType"
     )
     schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
@@ -386,14 +388,21 @@
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
     pricing: "CustomerPortalSubscriptionFragmentPricing"
     status: SubscriptionStatus
     trial_remaining_days: Optional[int] = Field(alias="trialRemainingDays")
     billing_period_range: Optional[
@@ -462,23 +471,14 @@
 
 class CustomerPortalSubscriptionFragmentScheduledUpdates(
     CustomerPortalSubscriptionScheduledUpdateData
 ):
     pass
 
 
-class CustomerPortalPromotionalEntitlement(BaseModel):
-    display_name: str = Field(alias="displayName")
-    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
-    usage_limit: Optional[float] = Field(alias="usageLimit")
-    period: PromotionalEntitlementPeriod
-    start_date: Any = Field(alias="startDate")
-    end_date: Optional[Any] = Field(alias="endDate")
-
-
 class CustomerResourceFragment(BaseModel):
     resource_id: str = Field(alias="resourceId")
 
 
 class CustomerPortalFragment(BaseModel):
     subscriptions: List["CustomerPortalFragmentSubscriptions"]
     entitlements: List["CustomerPortalFragmentEntitlements"]
@@ -517,14 +517,80 @@
     pass
 
 
 class CustomerPortalFragmentResource(CustomerResourceFragment):
     pass
 
 
+class SubscriptionScheduledUpdateData(BaseModel):
+    subscription_schedule_type: SubscriptionScheduleType = Field(
+        alias="subscriptionScheduleType"
+    )
+    schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
+    scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
+    target_package: Optional["SubscriptionScheduledUpdateDataTargetPackage"] = Field(
+        alias="targetPackage"
+    )
+    schedule_variables: Optional[
+        Annotated[
+            Union[
+                "SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables",
+                "SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables",
+                "SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables",
+            ],
+            Field(discriminator="typename__"),
+        ]
+    ] = Field(alias="scheduleVariables")
+
+
+class SubscriptionScheduledUpdateDataTargetPackage(BaseModel):
+    id: str
+    ref_id: str = Field(alias="refId")
+    display_name: str = Field(alias="displayName")
+
+
+class SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables(
+    BaseModel
+):
+    typename__: Literal["BillingPeriodChangeVariables"] = Field(alias="__typename")
+    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
+
+
+class SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables(
+    BaseModel
+):
+    typename__: Literal["DowngradeChangeVariables"] = Field(alias="__typename")
+    addon_ref_ids: Optional[str] = Field(alias="addonRefIds")
+    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
+    downgrade_plan_ref_id: str = Field(alias="downgradePlanRefId")
+
+
+class SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables(
+    BaseModel
+):
+    typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
+    new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
+    feature_id: Optional[str] = Field(alias="featureId")
+
+
+class TotalPriceFragment(BaseModel):
+    sub_total: "TotalPriceFragmentSubTotal" = Field(alias="subTotal")
+    total: "TotalPriceFragmentTotal"
+
+
+class TotalPriceFragmentSubTotal(BaseModel):
+    amount: float
+    currency: Currency
+
+
+class TotalPriceFragmentTotal(BaseModel):
+    amount: float
+    currency: Currency
+
+
 class ProductFragment(BaseModel):
     ref_id: str = Field(alias="refId")
     display_name: Optional[str] = Field(alias="displayName")
     description: Optional[str]
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
     product_settings: "ProductFragmentProductSettings" = Field(alias="productSettings")
 
@@ -589,80 +655,14 @@
 
 
 class PlanFragmentDefaultTrialConfig(BaseModel):
     duration: float
     units: TrialPeriodUnits
 
 
-class TotalPriceFragment(BaseModel):
-    sub_total: "TotalPriceFragmentSubTotal" = Field(alias="subTotal")
-    total: "TotalPriceFragmentTotal"
-
-
-class TotalPriceFragmentSubTotal(BaseModel):
-    amount: float
-    currency: Currency
-
-
-class TotalPriceFragmentTotal(BaseModel):
-    amount: float
-    currency: Currency
-
-
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
@@ -813,34 +813,14 @@
 class LayoutConfigurationFragment(BaseModel):
     alignment: Optional[Alignment]
     plan_width: Optional[float] = Field(alias="planWidth")
     plan_margin: Optional[float] = Field(alias="planMargin")
     plan_padding: Optional[float] = Field(alias="planPadding")
 
 
-class MockPaywallPackageEntitlementFragment(BaseModel):
-    usage_limit: Optional[float] = Field(alias="usageLimit")
-    has_unlimited_usage: bool = Field(alias="hasUnlimitedUsage")
-    reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
-    hidden_from_widgets: Optional[List[WidgetType]] = Field(alias="hiddenFromWidgets")
-    display_name_override: Optional[str] = Field(alias="displayNameOverride")
-    feature: Optional["MockPaywallPackageEntitlementFragmentFeature"]
-
-
-class MockPaywallPackageEntitlementFragmentFeature(BaseModel):
-    feature_type: FeatureType = Field(alias="featureType")
-    meter_type: Optional[MeterType] = Field(alias="meterType")
-    feature_units: Optional[str] = Field(alias="featureUnits")
-    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
-    display_name: str = Field(alias="displayName")
-    description: Optional[str]
-    ref_id: str = Field(alias="refId")
-    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
-
-
 class MockPaywallPriceFragment(BaseModel):
     billing_model: BillingModel = Field(alias="billingModel")
     billing_period: BillingPeriod = Field(alias="billingPeriod")
     billing_id: Optional[str] = Field(alias="billingId")
     min_unit_quantity: Optional[float] = Field(alias="minUnitQuantity")
     max_unit_quantity: Optional[float] = Field(alias="maxUnitQuantity")
     billing_country_code: Optional[str] = Field(alias="billingCountryCode")
@@ -855,14 +835,34 @@
 
 class MockPaywallPriceFragmentFeature(BaseModel):
     feature_units: Optional[str] = Field(alias="featureUnits")
     feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
     display_name: str = Field(alias="displayName")
 
 
+class MockPaywallPackageEntitlementFragment(BaseModel):
+    usage_limit: Optional[float] = Field(alias="usageLimit")
+    has_unlimited_usage: bool = Field(alias="hasUnlimitedUsage")
+    reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
+    hidden_from_widgets: Optional[List[WidgetType]] = Field(alias="hiddenFromWidgets")
+    display_name_override: Optional[str] = Field(alias="displayNameOverride")
+    feature: Optional["MockPaywallPackageEntitlementFragmentFeature"]
+
+
+class MockPaywallPackageEntitlementFragmentFeature(BaseModel):
+    feature_type: FeatureType = Field(alias="featureType")
+    meter_type: Optional[MeterType] = Field(alias="meterType")
+    feature_units: Optional[str] = Field(alias="featureUnits")
+    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
+    display_name: str = Field(alias="displayName")
+    description: Optional[str]
+    ref_id: str = Field(alias="refId")
+    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
+
+
 class MockPaywallAddonFragment(BaseModel):
     ref_id: str = Field(alias="refId")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
     billing_id: Optional[str] = Field(alias="billingId")
     entitlements: List["MockPaywallAddonFragmentEntitlements"]
@@ -1279,17 +1279,17 @@
 PackageEntitlementFragmentFeature.update_forward_refs()
 AddonFragment.update_forward_refs()
 AddonFragmentEntitlements.update_forward_refs()
 AddonFragmentPrices.update_forward_refs()
 CouponFragment.update_forward_refs()
 CouponFragmentSyncStates.update_forward_refs()
 CouponFragmentCustomers.update_forward_refs()
+SlimCustomerFragment.update_forward_refs()
 PromotionalEntitlementFragment.update_forward_refs()
 PromotionalEntitlementFragmentFeature.update_forward_refs()
-SlimCustomerFragment.update_forward_refs()
 CustomerFragment.update_forward_refs()
 CustomerFragmentTrialedPlans.update_forward_refs()
 CustomerFragmentExperimentInfo.update_forward_refs()
 CustomerFragmentCoupon.update_forward_refs()
 CustomerFragmentEligibleForTrial.update_forward_refs()
 CustomerFragmentPromotionalEntitlements.update_forward_refs()
 CustomerPortalBillingInformation.update_forward_refs()
@@ -1303,59 +1303,59 @@
 CustomerPortalConfigurationFragmentPalette.update_forward_refs()
 CustomerPortalConfigurationFragmentTypography.update_forward_refs()
 FeatureFragment.update_forward_refs()
 CustomerPortalEntitlement.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationMonthlyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationWeeklyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementFeature.update_forward_refs()
-CustomerPortalSubscriptionAddon.update_forward_refs()
+CustomerPortalPromotionalEntitlement.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateData.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
+CustomerPortalSubscriptionAddon.update_forward_refs()
 CustomerPortalSubscriptionFragment.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricing.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricingPrice.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricingFeature.update_forward_refs()
 CustomerPortalSubscriptionFragmentBillingPeriodRange.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPrice.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceSubTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceAddonsTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentAddons.update_forward_refs()
 CustomerPortalSubscriptionFragmentScheduledUpdates.update_forward_refs()
-CustomerPortalPromotionalEntitlement.update_forward_refs()
 CustomerResourceFragment.update_forward_refs()
 CustomerPortalFragment.update_forward_refs()
 CustomerPortalFragmentSubscriptions.update_forward_refs()
 CustomerPortalFragmentEntitlements.update_forward_refs()
 CustomerPortalFragmentPromotionalEntitlements.update_forward_refs()
 CustomerPortalFragmentBillingInformation.update_forward_refs()
 CustomerPortalFragmentConfiguration.update_forward_refs()
 CustomerPortalFragmentResource.update_forward_refs()
+SubscriptionScheduledUpdateData.update_forward_refs()
+SubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
+SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
+SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
+SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
+TotalPriceFragment.update_forward_refs()
+TotalPriceFragmentSubTotal.update_forward_refs()
+TotalPriceFragmentTotal.update_forward_refs()
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
-TotalPriceFragment.update_forward_refs()
-TotalPriceFragmentSubTotal.update_forward_refs()
-TotalPriceFragmentTotal.update_forward_refs()
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
@@ -1371,19 +1371,19 @@
 UsageUpdatedFragment.update_forward_refs()
 EntitlementUsageUpdated.update_forward_refs()
 EntitlementUsageUpdatedUsage.update_forward_refs()
 EntitlementUsageUpdatedEntitlement.update_forward_refs()
 EntitlementsUpdatedPayload.update_forward_refs()
 EntitlementsUpdatedPayloadEntitlements.update_forward_refs()
 LayoutConfigurationFragment.update_forward_refs()
-MockPaywallPackageEntitlementFragment.update_forward_refs()
-MockPaywallPackageEntitlementFragmentFeature.update_forward_refs()
 MockPaywallPriceFragment.update_forward_refs()
 MockPaywallPriceFragmentPrice.update_forward_refs()
 MockPaywallPriceFragmentFeature.update_forward_refs()
+MockPaywallPackageEntitlementFragment.update_forward_refs()
+MockPaywallPackageEntitlementFragmentFeature.update_forward_refs()
 MockPaywallAddonFragment.update_forward_refs()
 MockPaywallAddonFragmentEntitlements.update_forward_refs()
 MockPaywallAddonFragmentPrices.update_forward_refs()
 MockPaywallPlanFragment.update_forward_refs()
 MockPaywallPlanFragmentProduct.update_forward_refs()
 MockPaywallPlanFragmentBasePlan.update_forward_refs()
 MockPaywallPlanFragmentEntitlements.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.460.0/stigg/generated/get_active_subscriptions.py` & `stigg_api_client_v2-0.461.2/stigg/generated/get_active_subscriptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-11 06:23
+# Generated by ariadne-codegen on 2023-06-11 15:34
 # Source: operations.graphql
 
 from typing import List
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.460.0/stigg/generated/get_coupons.py` & `stigg_api_client_v2-0.461.2/stigg/generated/get_coupons.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-11 06:23
+# Generated by ariadne-codegen on 2023-06-11 15:34
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import CouponFragment
```

### Comparing `stigg_api_client_v2-0.460.0/stigg/generated/get_customer_by_id.py` & `stigg_api_client_v2-0.461.2/stigg/generated/get_customer_by_id.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-11 06:23
+# Generated by ariadne-codegen on 2023-06-11 15:34
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.460.0/stigg/generated/get_customer_portal_by_ref_id.py` & `stigg_api_client_v2-0.461.2/stigg/generated/get_customer_portal_by_ref_id.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-11 06:23
+# Generated by ariadne-codegen on 2023-06-11 15:34
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import CustomerPortalFragment
```

### Comparing `stigg_api_client_v2-0.460.0/stigg/generated/get_mock_paywall.py` & `stigg_api_client_v2-0.461.2/stigg/generated/get_mock_paywall.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-11 06:23
+# Generated by ariadne-codegen on 2023-06-11 15:34
 # Source: operations.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.460.0/stigg/generated/get_products.py` & `stigg_api_client_v2-0.461.2/stigg/generated/get_products.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-11 06:23
+# Generated by ariadne-codegen on 2023-06-11 15:34
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import ProductFragment
```

### Comparing `stigg_api_client_v2-0.460.0/stigg/generated/get_sdk_configuration.py` & `stigg_api_client_v2-0.461.2/stigg/generated/get_sdk_configuration.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-11 06:23
+# Generated by ariadne-codegen on 2023-06-11 15:34
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.460.0/stigg/generated/input_types.py` & `stigg_api_client_v2-0.461.2/stigg/generated/input_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-11 06:23
+# Generated by ariadne-codegen on 2023-06-11 15:34
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from typing import Any, List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -1217,36 +1217,14 @@
 
 
 class InitAddStripeCustomerPaymentMethodInput(BaseModel):
     customer_ref_id: str = Field(alias="customerRefId")
     environment_id: Optional[str] = Field(alias="environmentId")
 
 
-class InitiateCheckoutInput(BaseModel):
-    addons: Optional[List["SubscriptionAddonInput"]]
-    allow_promo_codes: Optional[bool] = Field(alias="allowPromoCodes", default=False)
-    allow_tax_id_collection: Optional[bool] = Field(
-        alias="allowTaxIdCollection", default=False
-    )
-    billing_country_code: Optional[str] = Field(alias="billingCountryCode")
-    billing_period: BillingPeriod = Field(alias="billingPeriod")
-    cancel_url: str = Field(alias="cancelUrl")
-    collect_billing_address: Optional[bool] = Field(
-        alias="collectBillingAddress", default=False
-    )
-    collect_phone_number: Optional[bool] = Field(
-        alias="collectPhoneNumber", default=False
-    )
-    customer_id: str = Field(alias="customerId")
-    plan_id: str = Field(alias="planId")
-    resource_id: Optional[str] = Field(alias="resourceId")
-    success_url: str = Field(alias="successUrl")
-    unit_quantity: Optional[int] = Field(alias="unitQuantity")
-
-
 class IntFieldComparison(BaseModel):
     between: Optional["IntFieldComparisonBetween"]
     eq: Optional[int]
     gt: Optional[int]
     gte: Optional[int]
     in_: Optional[List[int]] = Field(alias="in")
     is_: Optional[bool] = Field(alias="is")
@@ -2874,15 +2852,14 @@
 ImportIntegrationCatalogInput.update_forward_refs()
 ImportIntegrationCustomersInput.update_forward_refs()
 ImportIntegrationTaskFilter.update_forward_refs()
 ImportIntegrationTaskSort.update_forward_refs()
 ImportSubscriptionInput.update_forward_refs()
 ImportSubscriptionsBulk.update_forward_refs()
 InitAddStripeCustomerPaymentMethodInput.update_forward_refs()
-InitiateCheckoutInput.update_forward_refs()
 IntFieldComparison.update_forward_refs()
 IntFieldComparisonBetween.update_forward_refs()
 IntegrationFilter.update_forward_refs()
 IntegrationSort.update_forward_refs()
 MemberFilter.update_forward_refs()
 MemberSort.update_forward_refs()
 MeterAggregation.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.460.0/stigg/generated/migrate_subscription_to_latest.py` & `stigg_api_client_v2-0.461.2/stigg/generated/migrate_subscription_to_latest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-11 06:23
+# Generated by ariadne-codegen on 2023-06-11 15:34
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.460.0/stigg/generated/provision_customer.py` & `stigg_api_client_v2-0.461.2/stigg/generated/provision_customer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-11 06:23
+# Generated by ariadne-codegen on 2023-06-11 15:34
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.460.0/stigg/generated/provision_subscription.py` & `stigg_api_client_v2-0.461.2/stigg/generated/provision_subscription.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-11 06:23
+# Generated by ariadne-codegen on 2023-06-11 15:34
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.460.0/stigg/generated/update_subscription.py` & `stigg_api_client_v2-0.461.2/stigg/generated/update_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-11 06:23
+# Generated by ariadne-codegen on 2023-06-11 15:34
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.460.0/PKG-INFO` & `stigg_api_client_v2-0.461.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stigg-api-client-v2
-Version: 0.460.0
+Version: 0.461.2
 Summary: 
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

