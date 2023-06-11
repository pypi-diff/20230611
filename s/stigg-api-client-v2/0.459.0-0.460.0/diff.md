# Comparing `tmp/stigg_api_client_v2-0.459.0.tar.gz` & `tmp/stigg_api_client_v2-0.460.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_api_client_v2-0.459.0.tar", max compression
+gzip compressed data, was "stigg_api_client_v2-0.460.0.tar", max compression
```

## Comparing `stigg_api_client_v2-0.459.0.tar` & `stigg_api_client_v2-0.460.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     1644 2023-06-07 11:06:32.188135 stigg_api_client_v2-0.459.0/README.md
--rw-r--r--   0        0        0      653 2023-06-07 11:07:10.536314 stigg_api_client_v2-0.459.0/pyproject.toml
--rw-r--r--   0        0        0       44 2023-06-07 11:06:32.188135 stigg_api_client_v2-0.459.0/stigg/__init__.py
--rw-r--r--   0        0        0      363 2023-06-07 11:06:32.188135 stigg_api_client_v2-0.459.0/stigg/client.py
--rw-r--r--   0        0        0    39450 2023-06-07 11:07:08.900310 stigg_api_client_v2-0.459.0/stigg/generated/__init__.py
--rw-r--r--   0        0        0     7303 2023-06-07 11:07:08.544309 stigg_api_client_v2-0.459.0/stigg/generated/async_base_client.py
--rw-r--r--   0        0        0     1951 2023-06-07 11:07:08.544309 stigg_api_client_v2-0.459.0/stigg/generated/base_model.py
--rw-r--r--   0        0        0      527 2023-06-07 11:07:07.684306 stigg_api_client_v2-0.459.0/stigg/generated/cancel_subscription.py
--rw-r--r--   0        0        0      296 2023-06-07 11:07:07.708306 stigg_api_client_v2-0.459.0/stigg/generated/cancel_subscription_updates.py
--rw-r--r--   0        0        0    69448 2023-06-07 11:07:08.752309 stigg_api_client_v2-0.459.0/stigg/generated/client.py
--rw-r--r--   0        0        0      527 2023-06-07 11:07:07.728307 stigg_api_client_v2-0.459.0/stigg/generated/create_subscription.py
--rw-r--r--   0        0        0      541 2023-06-07 11:07:07.808307 stigg_api_client_v2-0.459.0/stigg/generated/entitlements_updated.py
--rw-r--r--   0        0        0    23614 2023-06-07 11:07:05.588301 stigg_api_client_v2-0.459.0/stigg/generated/enums.py
--rw-r--r--   0        0        0      553 2023-06-07 11:07:07.696307 stigg_api_client_v2-0.459.0/stigg/generated/estimate_subscription.py
--rw-r--r--   0        0        0      614 2023-06-07 11:07:07.704306 stigg_api_client_v2-0.459.0/stigg/generated/estimate_subscription_update.py
--rw-r--r--   0        0        0     2366 2023-06-07 11:07:08.544309 stigg_api_client_v2-0.459.0/stigg/generated/exceptions.py
--rw-r--r--   0        0        0    53088 2023-06-07 11:07:08.540309 stigg_api_client_v2-0.459.0/stigg/generated/fragments.py
--rw-r--r--   0        0        0      591 2023-06-07 11:07:07.748307 stigg_api_client_v2-0.459.0/stigg/generated/get_active_subscriptions.py
--rw-r--r--   0        0        0      634 2023-06-07 11:07:07.756307 stigg_api_client_v2-0.459.0/stigg/generated/get_coupons.py
--rw-r--r--   0        0        0      572 2023-06-07 11:07:07.740307 stigg_api_client_v2-0.459.0/stigg/generated/get_customer_by_id.py
--rw-r--r--   0        0        0      533 2023-06-07 11:07:07.792307 stigg_api_client_v2-0.459.0/stigg/generated/get_customer_portal_by_ref_id.py
--rw-r--r--   0        0        0      390 2023-06-07 11:07:07.768307 stigg_api_client_v2-0.459.0/stigg/generated/get_entitlement.py
--rw-r--r--   0        0        0      430 2023-06-07 11:07:07.764307 stigg_api_client_v2-0.459.0/stigg/generated/get_entitlements.py
--rw-r--r--   0        0        0      893 2023-06-07 11:07:07.800307 stigg_api_client_v2-0.459.0/stigg/generated/get_mock_paywall.py
--rw-r--r--   0        0        0      346 2023-06-07 11:07:07.760307 stigg_api_client_v2-0.459.0/stigg/generated/get_paywall.py
--rw-r--r--   0        0        0      657 2023-06-07 11:07:07.776307 stigg_api_client_v2-0.459.0/stigg/generated/get_products.py
--rw-r--r--   0        0        0      650 2023-06-07 11:07:07.788307 stigg_api_client_v2-0.459.0/stigg/generated/get_sdk_configuration.py
--rw-r--r--   0        0        0      465 2023-06-07 11:07:07.652306 stigg_api_client_v2-0.459.0/stigg/generated/import_customer.py
--rw-r--r--   0        0        0      332 2023-06-07 11:07:07.644306 stigg_api_client_v2-0.459.0/stigg/generated/import_customer_bulk.py
--rw-r--r--   0        0        0      350 2023-06-07 11:07:07.672306 stigg_api_client_v2-0.459.0/stigg/generated/import_subscriptions_bulk.py
--rw-r--r--   0        0        0      550 2023-06-07 11:07:07.692306 stigg_api_client_v2-0.459.0/stigg/generated/initiate_checkout.py
--rw-r--r--   0        0        0   125804 2023-06-07 11:07:07.628306 stigg_api_client_v2-0.459.0/stigg/generated/input_types.py
--rw-r--r--   0        0        0      604 2023-06-07 11:07:07.732307 stigg_api_client_v2-0.459.0/stigg/generated/migrate_subscription_to_latest.py
--rw-r--r--   0        0        0     1161 2023-06-07 11:07:07.640306 stigg_api_client_v2-0.459.0/stigg/generated/provision_customer.py
--rw-r--r--   0        0        0      971 2023-06-07 11:07:07.668306 stigg_api_client_v2-0.459.0/stigg/generated/provision_subscription.py
--rw-r--r--   0        0        0      359 2023-06-07 11:07:07.720306 stigg_api_client_v2-0.459.0/stigg/generated/report_entitlement_check_requested.py
--rw-r--r--   0        0        0      637 2023-06-07 11:07:07.716307 stigg_api_client_v2-0.459.0/stigg/generated/report_usage.py
--rw-r--r--   0        0        0      220 2023-06-07 11:07:08.548309 stigg_api_client_v2-0.459.0/stigg/generated/scalars.py
--rw-r--r--   0        0        0      465 2023-06-07 11:07:07.660306 stigg_api_client_v2-0.459.0/stigg/generated/update_customer.py
--rw-r--r--   0        0        0      527 2023-06-07 11:07:07.676306 stigg_api_client_v2-0.459.0/stigg/generated/update_subscription.py
--rw-r--r--   0        0        0      451 2023-06-07 11:07:07.812307 stigg_api_client_v2-0.459.0/stigg/generated/usage_updated.py
--rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.459.0/PKG-INFO
+-rw-r--r--   0        0        0     1644 2023-06-11 06:22:38.788101 stigg_api_client_v2-0.460.0/README.md
+-rw-r--r--   0        0        0      653 2023-06-11 06:23:28.380972 stigg_api_client_v2-0.460.0/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-06-11 06:22:38.788101 stigg_api_client_v2-0.460.0/stigg/__init__.py
+-rw-r--r--   0        0        0      363 2023-06-11 06:22:38.788101 stigg_api_client_v2-0.460.0/stigg/client.py
+-rw-r--r--   0        0        0    39496 2023-06-11 06:23:26.384939 stigg_api_client_v2-0.460.0/stigg/generated/__init__.py
+-rw-r--r--   0        0        0     7303 2023-06-11 06:23:26.008932 stigg_api_client_v2-0.460.0/stigg/generated/async_base_client.py
+-rw-r--r--   0        0        0     1951 2023-06-11 06:23:26.008932 stigg_api_client_v2-0.460.0/stigg/generated/base_model.py
+-rw-r--r--   0        0        0      527 2023-06-11 06:23:24.980915 stigg_api_client_v2-0.460.0/stigg/generated/cancel_subscription.py
+-rw-r--r--   0        0        0      296 2023-06-11 06:23:25.008916 stigg_api_client_v2-0.460.0/stigg/generated/cancel_subscription_updates.py
+-rw-r--r--   0        0        0    69448 2023-06-11 06:23:26.228936 stigg_api_client_v2-0.460.0/stigg/generated/client.py
+-rw-r--r--   0        0        0      527 2023-06-11 06:23:25.028916 stigg_api_client_v2-0.460.0/stigg/generated/create_subscription.py
+-rw-r--r--   0        0        0      541 2023-06-11 06:23:25.112917 stigg_api_client_v2-0.460.0/stigg/generated/entitlements_updated.py
+-rw-r--r--   0        0        0    23730 2023-06-11 06:23:22.468873 stigg_api_client_v2-0.460.0/stigg/generated/enums.py
+-rw-r--r--   0        0        0      553 2023-06-11 06:23:24.996915 stigg_api_client_v2-0.460.0/stigg/generated/estimate_subscription.py
+-rw-r--r--   0        0        0      614 2023-06-11 06:23:25.004915 stigg_api_client_v2-0.460.0/stigg/generated/estimate_subscription_update.py
+-rw-r--r--   0        0        0     2366 2023-06-11 06:23:26.008932 stigg_api_client_v2-0.460.0/stigg/generated/exceptions.py
+-rw-r--r--   0        0        0    53088 2023-06-11 06:23:26.008932 stigg_api_client_v2-0.460.0/stigg/generated/fragments.py
+-rw-r--r--   0        0        0      591 2023-06-11 06:23:25.048916 stigg_api_client_v2-0.460.0/stigg/generated/get_active_subscriptions.py
+-rw-r--r--   0        0        0      634 2023-06-11 06:23:25.056916 stigg_api_client_v2-0.460.0/stigg/generated/get_coupons.py
+-rw-r--r--   0        0        0      572 2023-06-11 06:23:25.044916 stigg_api_client_v2-0.460.0/stigg/generated/get_customer_by_id.py
+-rw-r--r--   0        0        0      533 2023-06-11 06:23:25.096917 stigg_api_client_v2-0.460.0/stigg/generated/get_customer_portal_by_ref_id.py
+-rw-r--r--   0        0        0      390 2023-06-11 06:23:25.072917 stigg_api_client_v2-0.460.0/stigg/generated/get_entitlement.py
+-rw-r--r--   0        0        0      430 2023-06-11 06:23:25.068916 stigg_api_client_v2-0.460.0/stigg/generated/get_entitlements.py
+-rw-r--r--   0        0        0      893 2023-06-11 06:23:25.104917 stigg_api_client_v2-0.460.0/stigg/generated/get_mock_paywall.py
+-rw-r--r--   0        0        0      346 2023-06-11 06:23:25.064916 stigg_api_client_v2-0.460.0/stigg/generated/get_paywall.py
+-rw-r--r--   0        0        0      657 2023-06-11 06:23:25.084917 stigg_api_client_v2-0.460.0/stigg/generated/get_products.py
+-rw-r--r--   0        0        0      650 2023-06-11 06:23:25.092917 stigg_api_client_v2-0.460.0/stigg/generated/get_sdk_configuration.py
+-rw-r--r--   0        0        0      465 2023-06-11 06:23:24.948914 stigg_api_client_v2-0.460.0/stigg/generated/import_customer.py
+-rw-r--r--   0        0        0      332 2023-06-11 06:23:24.940914 stigg_api_client_v2-0.460.0/stigg/generated/import_customer_bulk.py
+-rw-r--r--   0        0        0      350 2023-06-11 06:23:24.968915 stigg_api_client_v2-0.460.0/stigg/generated/import_subscriptions_bulk.py
+-rw-r--r--   0        0        0      550 2023-06-11 06:23:24.988915 stigg_api_client_v2-0.460.0/stigg/generated/initiate_checkout.py
+-rw-r--r--   0        0        0   126306 2023-06-11 06:23:24.924914 stigg_api_client_v2-0.460.0/stigg/generated/input_types.py
+-rw-r--r--   0        0        0      604 2023-06-11 06:23:25.036916 stigg_api_client_v2-0.460.0/stigg/generated/migrate_subscription_to_latest.py
+-rw-r--r--   0        0        0     1161 2023-06-11 06:23:24.936914 stigg_api_client_v2-0.460.0/stigg/generated/provision_customer.py
+-rw-r--r--   0        0        0      971 2023-06-11 06:23:24.964915 stigg_api_client_v2-0.460.0/stigg/generated/provision_subscription.py
+-rw-r--r--   0        0        0      359 2023-06-11 06:23:25.024916 stigg_api_client_v2-0.460.0/stigg/generated/report_entitlement_check_requested.py
+-rw-r--r--   0        0        0      637 2023-06-11 06:23:25.016916 stigg_api_client_v2-0.460.0/stigg/generated/report_usage.py
+-rw-r--r--   0        0        0      220 2023-06-11 06:23:26.012932 stigg_api_client_v2-0.460.0/stigg/generated/scalars.py
+-rw-r--r--   0        0        0      465 2023-06-11 06:23:24.952915 stigg_api_client_v2-0.460.0/stigg/generated/update_customer.py
+-rw-r--r--   0        0        0      527 2023-06-11 06:23:24.976915 stigg_api_client_v2-0.460.0/stigg/generated/update_subscription.py
+-rw-r--r--   0        0        0      451 2023-06-11 06:23:25.120917 stigg_api_client_v2-0.460.0/stigg/generated/usage_updated.py
+-rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.460.0/PKG-INFO
```

### Comparing `stigg_api_client_v2-0.459.0/README.md` & `stigg_api_client_v2-0.460.0/README.md`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.459.0/pyproject.toml` & `stigg_api_client_v2-0.460.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stigg-api-client-v2"
-version = "0.459.0"
+version = "0.460.0"
 description = ""
 authors = ["Stigg <support@stigg.io>"]
 readme = "README.md"
 packages = [{ include = "stigg" }]
 include = ["stigg/generated/*"]
 
 [tool.poetry.dependencies]
```

### Comparing `stigg_api_client_v2-0.459.0/stigg/generated/__init__.py` & `stigg_api_client_v2-0.460.0/stigg/generated/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-07 11:07
+# Generated by ariadne-codegen on 2023-06-11 06:23
 
 from .async_base_client import AsyncBaseClient
 from .base_model import BaseModel
 from .cancel_subscription import (
     CancelSubscription,
     CancelSubscriptionCancelSubscription,
 )
@@ -500,14 +500,15 @@
     ProvisionSubscriptionInput,
     RemoveBasePlanFromPlanInput,
     RemoveCompatibleAddonsFromPlanInput,
     RemoveCouponFromCustomerInput,
     RemoveCouponFromCustomerSubscriptionInput,
     RemoveExperimentFromCustomerInput,
     RemoveExperimentFromCustomerSubscriptionInput,
+    ReportUsageInput,
     ResyncIntegrationInput,
     SetBasePlanOnPlanInput,
     SetCompatibleAddonsOnPlanInput,
     SetCouponOnCustomerInput,
     SetCouponOnCustomerSubscriptionInput,
     SetExperimentOnCustomerInput,
     SetExperimentOnCustomerSubscriptionInput,
@@ -1016,14 +1017,15 @@
     "RemoveCouponFromCustomerInput",
     "RemoveCouponFromCustomerSubscriptionInput",
     "RemoveExperimentFromCustomerInput",
     "RemoveExperimentFromCustomerSubscriptionInput",
     "ReportEntitlementCheckRequested",
     "ReportUsage",
     "ReportUsageCreateUsageMeasurement",
+    "ReportUsageInput",
     "ResyncIntegrationInput",
     "SetBasePlanOnPlanInput",
     "SetCompatibleAddonsOnPlanInput",
     "SetCouponOnCustomerInput",
     "SetCouponOnCustomerSubscriptionInput",
     "SetExperimentOnCustomerInput",
     "SetExperimentOnCustomerSubscriptionInput",
```

### Comparing `stigg_api_client_v2-0.459.0/stigg/generated/async_base_client.py` & `stigg_api_client_v2-0.460.0/stigg/generated/async_base_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-07 11:07
+# Generated by ariadne-codegen on 2023-06-11 06:23
 
 import enum
 import json
 from typing import Any, AsyncIterator, Dict, Optional, TypeVar, cast
 from uuid import uuid4
 
 import httpx
```

### Comparing `stigg_api_client_v2-0.459.0/stigg/generated/base_model.py` & `stigg_api_client_v2-0.460.0/stigg/generated/base_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-07 11:07
+# Generated by ariadne-codegen on 2023-06-11 06:23
 
 from typing import Any, Dict, Type, Union, get_args, get_origin
 
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic.class_validators import validator
 from pydantic.fields import ModelField
```

### Comparing `stigg_api_client_v2-0.459.0/stigg/generated/cancel_subscription.py` & `stigg_api_client_v2-0.460.0/stigg/generated/cancel_subscription.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-07 11:07
+# Generated by ariadne-codegen on 2023-06-11 06:23
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.459.0/stigg/generated/client.py` & `stigg_api_client_v2-0.460.0/stigg/generated/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-07 11:07
+# Generated by ariadne-codegen on 2023-06-11 06:23
 # Source: operations.graphql
 
 from typing import AsyncIterator
 
 from .async_base_client import AsyncBaseClient
 from .cancel_subscription import CancelSubscription
 from .cancel_subscription_updates import CancelSubscriptionUpdates
```

### Comparing `stigg_api_client_v2-0.459.0/stigg/generated/create_subscription.py` & `stigg_api_client_v2-0.460.0/stigg/generated/create_subscription.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-07 11:07
+# Generated by ariadne-codegen on 2023-06-11 06:23
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.459.0/stigg/generated/entitlements_updated.py` & `stigg_api_client_v2-0.460.0/stigg/generated/entitlements_updated.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-07 11:07
+# Generated by ariadne-codegen on 2023-06-11 06:23
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import EntitlementsUpdatedPayload
```

### Comparing `stigg_api_client_v2-0.459.0/stigg/generated/enums.py` & `stigg_api_client_v2-0.460.0/stigg/generated/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-07 11:07
+# Generated by ariadne-codegen on 2023-06-11 06:23
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from enum import Enum
 
 
 class AccessDeniedReason(str, Enum):
     CustomerNotFound = "CustomerNotFound"
@@ -332,14 +332,17 @@
     AuthCustomerMismatch = "AuthCustomerMismatch"
     BadUserInput = "BadUserInput"
     BillingPeriodMissingError = "BillingPeriodMissingError"
     CannotDeleteCustomerError = "CannotDeleteCustomerError"
     CannotDeleteFeatureError = "CannotDeleteFeatureError"
     CannotDeleteProductError = "CannotDeleteProductError"
     CannotEditPackageInNonDraftMode = "CannotEditPackageInNonDraftMode"
+    CannotReportUsageForEntitlementWithMeterError = (
+        "CannotReportUsageForEntitlementWithMeterError"
+    )
     CheckoutIsNotSupported = "CheckoutIsNotSupported"
     CheckoutOptionsMissing = "CheckoutOptionsMissing"
     CouponNotFound = "CouponNotFound"
     CustomerAlreadyHaveCustomerCoupon = "CustomerAlreadyHaveCustomerCoupon"
     CustomerAlreadyUsesCoupon = "CustomerAlreadyUsesCoupon"
     CustomerHasNoPaymentMethod = "CustomerHasNoPaymentMethod"
     CustomerNoBillingId = "CustomerNoBillingId"
```

### Comparing `stigg_api_client_v2-0.459.0/stigg/generated/estimate_subscription.py` & `stigg_api_client_v2-0.460.0/stigg/generated/estimate_subscription.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-07 11:07
+# Generated by ariadne-codegen on 2023-06-11 06:23
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.459.0/stigg/generated/estimate_subscription_update.py` & `stigg_api_client_v2-0.460.0/stigg/generated/estimate_subscription_update.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-07 11:07
+# Generated by ariadne-codegen on 2023-06-11 06:23
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.459.0/stigg/generated/exceptions.py` & `stigg_api_client_v2-0.460.0/stigg/generated/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-07 11:07
+# Generated by ariadne-codegen on 2023-06-11 06:23
 
 from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
 
 class GraphQLClientError(Exception):
```

### Comparing `stigg_api_client_v2-0.459.0/stigg/generated/fragments.py` & `stigg_api_client_v2-0.460.0/stigg/generated/fragments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-07 11:07
+# Generated by ariadne-codegen on 2023-06-11 06:23
 # Source: operations.graphql
 
 from typing import Annotated, Any, List, Literal, Optional, Union
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -32,36 +32,14 @@
     VendorIdentifier,
     WeeklyAccordingTo,
     WidgetType,
     experimentGroupType,
 )
 
 
-class PackageEntitlementFragment(BaseModel):
-    usage_limit: Optional[float] = Field(alias="usageLimit")
-    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
-    feature_id: str = Field(alias="featureId")
-    reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
-    hidden_from_widgets: Optional[List[WidgetType]] = Field(alias="hiddenFromWidgets")
-    is_custom: Optional[bool] = Field(alias="isCustom")
-    display_name_override: Optional[str] = Field(alias="displayNameOverride")
-    feature: "PackageEntitlementFragmentFeature"
-
-
-class PackageEntitlementFragmentFeature(BaseModel):
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
 class PriceFragment(BaseModel):
     billing_model: BillingModel = Field(alias="billingModel")
     billing_period: BillingPeriod = Field(alias="billingPeriod")
     billing_id: Optional[str] = Field(alias="billingId")
     min_unit_quantity: Optional[float] = Field(alias="minUnitQuantity")
     max_unit_quantity: Optional[float] = Field(alias="maxUnitQuantity")
     billing_country_code: Optional[str] = Field(alias="billingCountryCode")
@@ -77,14 +55,36 @@
 class PriceFragmentFeature(BaseModel):
     feature_units: Optional[str] = Field(alias="featureUnits")
     feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
 
 
+class PackageEntitlementFragment(BaseModel):
+    usage_limit: Optional[float] = Field(alias="usageLimit")
+    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
+    feature_id: str = Field(alias="featureId")
+    reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
+    hidden_from_widgets: Optional[List[WidgetType]] = Field(alias="hiddenFromWidgets")
+    is_custom: Optional[bool] = Field(alias="isCustom")
+    display_name_override: Optional[str] = Field(alias="displayNameOverride")
+    feature: "PackageEntitlementFragmentFeature"
+
+
+class PackageEntitlementFragmentFeature(BaseModel):
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
 class AddonFragment(BaseModel):
     id: str
     ref_id: str = Field(alias="refId")
     billing_id: Optional[str] = Field(alias="billingId")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
@@ -462,27 +462,27 @@
 
 class CustomerPortalSubscriptionFragmentScheduledUpdates(
     CustomerPortalSubscriptionScheduledUpdateData
 ):
     pass
 
 
-class CustomerResourceFragment(BaseModel):
-    resource_id: str = Field(alias="resourceId")
-
-
 class CustomerPortalPromotionalEntitlement(BaseModel):
     display_name: str = Field(alias="displayName")
     has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
     usage_limit: Optional[float] = Field(alias="usageLimit")
     period: PromotionalEntitlementPeriod
     start_date: Any = Field(alias="startDate")
     end_date: Optional[Any] = Field(alias="endDate")
 
 
+class CustomerResourceFragment(BaseModel):
+    resource_id: str = Field(alias="resourceId")
+
+
 class CustomerPortalFragment(BaseModel):
     subscriptions: List["CustomerPortalFragmentSubscriptions"]
     entitlements: List["CustomerPortalFragmentEntitlements"]
     promotional_entitlements: List[
         "CustomerPortalFragmentPromotionalEntitlements"
     ] = Field(alias="promotionalEntitlements")
     billing_information: "CustomerPortalFragmentBillingInformation" = Field(
@@ -517,80 +517,14 @@
     pass
 
 
 class CustomerPortalFragmentResource(CustomerResourceFragment):
     pass
 
 
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
 class ProductFragment(BaseModel):
     ref_id: str = Field(alias="refId")
     display_name: Optional[str] = Field(alias="displayName")
     description: Optional[str]
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
     product_settings: "ProductFragmentProductSettings" = Field(alias="productSettings")
 
@@ -655,14 +589,80 @@
 
 
 class PlanFragmentDefaultTrialConfig(BaseModel):
     duration: float
     units: TrialPeriodUnits
 
 
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
 class SubscriptionFragment(BaseModel):
     id: str
     start_date: Any = Field(alias="startDate")
     end_date: Optional[Any] = Field(alias="endDate")
     trial_end_date: Optional[Any] = Field(alias="trialEndDate")
     cancellation_date: Optional[Any] = Field(alias="cancellationDate")
     effective_end_date: Optional[Any] = Field(alias="effectiveEndDate")
@@ -813,14 +813,34 @@
 class LayoutConfigurationFragment(BaseModel):
     alignment: Optional[Alignment]
     plan_width: Optional[float] = Field(alias="planWidth")
     plan_margin: Optional[float] = Field(alias="planMargin")
     plan_padding: Optional[float] = Field(alias="planPadding")
 
 
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
 class MockPaywallPriceFragment(BaseModel):
     billing_model: BillingModel = Field(alias="billingModel")
     billing_period: BillingPeriod = Field(alias="billingPeriod")
     billing_id: Optional[str] = Field(alias="billingId")
     min_unit_quantity: Optional[float] = Field(alias="minUnitQuantity")
     max_unit_quantity: Optional[float] = Field(alias="maxUnitQuantity")
     billing_country_code: Optional[str] = Field(alias="billingCountryCode")
@@ -835,34 +855,14 @@
 
 class MockPaywallPriceFragmentFeature(BaseModel):
     feature_units: Optional[str] = Field(alias="featureUnits")
     feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
     display_name: str = Field(alias="displayName")
 
 
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
 class MockPaywallAddonFragment(BaseModel):
     ref_id: str = Field(alias="refId")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
     billing_id: Optional[str] = Field(alias="billingId")
     entitlements: List["MockPaywallAddonFragmentEntitlements"]
@@ -1268,19 +1268,19 @@
 
 
 class SubscriptionPreviewFragmentProrationNetAmount(BaseModel):
     amount: float
     currency: Currency
 
 
-PackageEntitlementFragment.update_forward_refs()
-PackageEntitlementFragmentFeature.update_forward_refs()
 PriceFragment.update_forward_refs()
 PriceFragmentPrice.update_forward_refs()
 PriceFragmentFeature.update_forward_refs()
+PackageEntitlementFragment.update_forward_refs()
+PackageEntitlementFragmentFeature.update_forward_refs()
 AddonFragment.update_forward_refs()
 AddonFragmentEntitlements.update_forward_refs()
 AddonFragmentPrices.update_forward_refs()
 CouponFragment.update_forward_refs()
 CouponFragmentSyncStates.update_forward_refs()
 CouponFragmentCustomers.update_forward_refs()
 PromotionalEntitlementFragment.update_forward_refs()
@@ -1320,42 +1320,42 @@
 CustomerPortalSubscriptionFragmentBillingPeriodRange.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPrice.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceSubTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceAddonsTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentAddons.update_forward_refs()
 CustomerPortalSubscriptionFragmentScheduledUpdates.update_forward_refs()
-CustomerResourceFragment.update_forward_refs()
 CustomerPortalPromotionalEntitlement.update_forward_refs()
+CustomerResourceFragment.update_forward_refs()
 CustomerPortalFragment.update_forward_refs()
 CustomerPortalFragmentSubscriptions.update_forward_refs()
 CustomerPortalFragmentEntitlements.update_forward_refs()
 CustomerPortalFragmentPromotionalEntitlements.update_forward_refs()
 CustomerPortalFragmentBillingInformation.update_forward_refs()
 CustomerPortalFragmentConfiguration.update_forward_refs()
 CustomerPortalFragmentResource.update_forward_refs()
-SubscriptionScheduledUpdateData.update_forward_refs()
-SubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
-SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
-SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
-SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
-TotalPriceFragment.update_forward_refs()
-TotalPriceFragmentSubTotal.update_forward_refs()
-TotalPriceFragmentTotal.update_forward_refs()
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
+TotalPriceFragment.update_forward_refs()
+TotalPriceFragmentSubTotal.update_forward_refs()
+TotalPriceFragmentTotal.update_forward_refs()
+SubscriptionScheduledUpdateData.update_forward_refs()
+SubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
+SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
+SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
+SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
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
+MockPaywallPackageEntitlementFragment.update_forward_refs()
+MockPaywallPackageEntitlementFragmentFeature.update_forward_refs()
 MockPaywallPriceFragment.update_forward_refs()
 MockPaywallPriceFragmentPrice.update_forward_refs()
 MockPaywallPriceFragmentFeature.update_forward_refs()
-MockPaywallPackageEntitlementFragment.update_forward_refs()
-MockPaywallPackageEntitlementFragmentFeature.update_forward_refs()
 MockPaywallAddonFragment.update_forward_refs()
 MockPaywallAddonFragmentEntitlements.update_forward_refs()
 MockPaywallAddonFragmentPrices.update_forward_refs()
 MockPaywallPlanFragment.update_forward_refs()
 MockPaywallPlanFragmentProduct.update_forward_refs()
 MockPaywallPlanFragmentBasePlan.update_forward_refs()
 MockPaywallPlanFragmentEntitlements.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.459.0/stigg/generated/get_active_subscriptions.py` & `stigg_api_client_v2-0.460.0/stigg/generated/get_active_subscriptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-07 11:07
+# Generated by ariadne-codegen on 2023-06-11 06:23
 # Source: operations.graphql
 
 from typing import List
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.459.0/stigg/generated/get_coupons.py` & `stigg_api_client_v2-0.460.0/stigg/generated/get_coupons.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-07 11:07
+# Generated by ariadne-codegen on 2023-06-11 06:23
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import CouponFragment
```

### Comparing `stigg_api_client_v2-0.459.0/stigg/generated/get_customer_by_id.py` & `stigg_api_client_v2-0.460.0/stigg/generated/get_customer_by_id.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-07 11:07
+# Generated by ariadne-codegen on 2023-06-11 06:23
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.459.0/stigg/generated/get_customer_portal_by_ref_id.py` & `stigg_api_client_v2-0.460.0/stigg/generated/get_customer_portal_by_ref_id.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-07 11:07
+# Generated by ariadne-codegen on 2023-06-11 06:23
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import CustomerPortalFragment
```

### Comparing `stigg_api_client_v2-0.459.0/stigg/generated/get_mock_paywall.py` & `stigg_api_client_v2-0.460.0/stigg/generated/get_mock_paywall.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-07 11:07
+# Generated by ariadne-codegen on 2023-06-11 06:23
 # Source: operations.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.459.0/stigg/generated/get_products.py` & `stigg_api_client_v2-0.460.0/stigg/generated/get_products.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-07 11:07
+# Generated by ariadne-codegen on 2023-06-11 06:23
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import ProductFragment
```

### Comparing `stigg_api_client_v2-0.459.0/stigg/generated/get_sdk_configuration.py` & `stigg_api_client_v2-0.460.0/stigg/generated/get_sdk_configuration.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-07 11:07
+# Generated by ariadne-codegen on 2023-06-11 06:23
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.459.0/stigg/generated/input_types.py` & `stigg_api_client_v2-0.460.0/stigg/generated/input_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-07 11:07
+# Generated by ariadne-codegen on 2023-06-11 06:23
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from typing import Any, List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -1956,14 +1956,26 @@
 
 
 class RemoveExperimentFromCustomerSubscriptionInput(BaseModel):
     id: str
     relation_id: str = Field(alias="relationId")
 
 
+class ReportUsageInput(BaseModel):
+    created_at: Optional[Any] = Field(alias="createdAt")
+    customer_id: str = Field(alias="customerId")
+    environment_id: Optional[str] = Field(alias="environmentId")
+    feature_id: str = Field(alias="featureId")
+    resource_id: Optional[str] = Field(alias="resourceId")
+    update_behavior: Optional[UsageUpdateBehavior] = Field(
+        alias="updateBehavior", default=UsageUpdateBehavior.DELTA
+    )
+    value: float
+
+
 class ResyncIntegrationInput(BaseModel):
     environment_id: str = Field(alias="environmentId")
     vendor_identifier: VendorIdentifier = Field(alias="vendorIdentifier")
 
 
 class SetBasePlanOnPlanInput(BaseModel):
     id: str
@@ -2926,14 +2938,15 @@
 ProvisionSubscriptionInput.update_forward_refs()
 RemoveBasePlanFromPlanInput.update_forward_refs()
 RemoveCompatibleAddonsFromPlanInput.update_forward_refs()
 RemoveCouponFromCustomerInput.update_forward_refs()
 RemoveCouponFromCustomerSubscriptionInput.update_forward_refs()
 RemoveExperimentFromCustomerInput.update_forward_refs()
 RemoveExperimentFromCustomerSubscriptionInput.update_forward_refs()
+ReportUsageInput.update_forward_refs()
 ResyncIntegrationInput.update_forward_refs()
 SetBasePlanOnPlanInput.update_forward_refs()
 SetCompatibleAddonsOnPlanInput.update_forward_refs()
 SetCouponOnCustomerInput.update_forward_refs()
 SetCouponOnCustomerSubscriptionInput.update_forward_refs()
 SetExperimentOnCustomerInput.update_forward_refs()
 SetExperimentOnCustomerSubscriptionInput.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.459.0/stigg/generated/migrate_subscription_to_latest.py` & `stigg_api_client_v2-0.460.0/stigg/generated/migrate_subscription_to_latest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-07 11:07
+# Generated by ariadne-codegen on 2023-06-11 06:23
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.459.0/stigg/generated/provision_customer.py` & `stigg_api_client_v2-0.460.0/stigg/generated/provision_customer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-07 11:07
+# Generated by ariadne-codegen on 2023-06-11 06:23
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.459.0/stigg/generated/provision_subscription.py` & `stigg_api_client_v2-0.460.0/stigg/generated/provision_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-07 11:07
+# Generated by ariadne-codegen on 2023-06-11 06:23
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.459.0/stigg/generated/report_usage.py` & `stigg_api_client_v2-0.460.0/stigg/generated/report_usage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-07 11:07
+# Generated by ariadne-codegen on 2023-06-11 06:23
 # Source: operations.graphql
 
 from typing import Any, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.459.0/stigg/generated/update_subscription.py` & `stigg_api_client_v2-0.460.0/stigg/generated/update_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-07 11:07
+# Generated by ariadne-codegen on 2023-06-11 06:23
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.459.0/PKG-INFO` & `stigg_api_client_v2-0.460.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stigg-api-client-v2
-Version: 0.459.0
+Version: 0.460.0
 Summary: 
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

