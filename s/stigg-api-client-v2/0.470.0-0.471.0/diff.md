# Comparing `tmp/stigg_api_client_v2-0.470.0.tar.gz` & `tmp/stigg_api_client_v2-0.471.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_api_client_v2-0.470.0.tar", max compression
+gzip compressed data, was "stigg_api_client_v2-0.471.0.tar", max compression
```

## Comparing `stigg_api_client_v2-0.470.0.tar` & `stigg_api_client_v2-0.471.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1644 2023-06-12 16:19:38.768385 stigg_api_client_v2-0.470.0/README.md
--rw-r--r--   0        0        0      432 2023-06-30 16:55:06.815193 stigg_api_client_v2-0.470.0/pyproject.toml
--rw-r--r--   0        0        0       62 2023-06-30 16:39:54.462400 stigg_api_client_v2-0.470.0/stigg/__init__.py
--rw-r--r--   0        0        0     1520 2023-06-30 16:39:54.462736 stigg_api_client_v2-0.470.0/stigg/client.py
--rw-r--r--   0        0        0    39399 2023-06-30 16:23:24.123748 stigg_api_client_v2-0.470.0/stigg/generated/__init__.py
--rw-r--r--   0        0        0     7303 2023-06-30 16:23:23.230934 stigg_api_client_v2-0.470.0/stigg/generated/async_base_client.py
--rw-r--r--   0        0        0    66201 2023-06-30 16:23:23.754796 stigg_api_client_v2-0.470.0/stigg/generated/async_client.py
--rw-r--r--   0        0        0     2731 2023-06-30 16:23:14.372387 stigg_api_client_v2-0.470.0/stigg/generated/base_client.py
--rw-r--r--   0        0        0     1951 2023-06-30 16:23:23.232149 stigg_api_client_v2-0.470.0/stigg/generated/base_model.py
--rw-r--r--   0        0        0      527 2023-06-30 16:23:21.569815 stigg_api_client_v2-0.470.0/stigg/generated/cancel_subscription.py
--rw-r--r--   0        0        0      296 2023-06-30 16:23:21.598608 stigg_api_client_v2-0.470.0/stigg/generated/cancel_subscription_updates.py
--rw-r--r--   0        0        0    65786 2023-06-30 16:23:14.852597 stigg_api_client_v2-0.470.0/stigg/generated/client.py
--rw-r--r--   0        0        0      527 2023-06-30 16:23:21.639459 stigg_api_client_v2-0.470.0/stigg/generated/create_subscription.py
--rw-r--r--   0        0        0    23994 2023-06-30 16:23:16.926481 stigg_api_client_v2-0.470.0/stigg/generated/enums.py
--rw-r--r--   0        0        0      553 2023-06-30 16:23:21.580409 stigg_api_client_v2-0.470.0/stigg/generated/estimate_subscription.py
--rw-r--r--   0        0        0      614 2023-06-30 16:23:21.592114 stigg_api_client_v2-0.470.0/stigg/generated/estimate_subscription_update.py
--rw-r--r--   0        0        0     2366 2023-06-30 16:23:23.232391 stigg_api_client_v2-0.470.0/stigg/generated/exceptions.py
--rw-r--r--   0        0        0    53605 2023-06-30 16:23:23.229439 stigg_api_client_v2-0.470.0/stigg/generated/fragments.py
--rw-r--r--   0        0        0      591 2023-06-30 16:23:21.676317 stigg_api_client_v2-0.470.0/stigg/generated/get_active_subscriptions.py
--rw-r--r--   0        0        0      634 2023-06-30 16:23:21.693093 stigg_api_client_v2-0.470.0/stigg/generated/get_coupons.py
--rw-r--r--   0        0        0      572 2023-06-30 16:23:21.663635 stigg_api_client_v2-0.470.0/stigg/generated/get_customer_by_id.py
--rw-r--r--   0        0        0      533 2023-06-30 16:23:21.763239 stigg_api_client_v2-0.470.0/stigg/generated/get_customer_portal_by_ref_id.py
--rw-r--r--   0        0        0      390 2023-06-30 16:23:21.721879 stigg_api_client_v2-0.470.0/stigg/generated/get_entitlement.py
--rw-r--r--   0        0        0      430 2023-06-30 16:23:21.711869 stigg_api_client_v2-0.470.0/stigg/generated/get_entitlements.py
--rw-r--r--   0        0        0      893 2023-06-30 16:23:21.781593 stigg_api_client_v2-0.470.0/stigg/generated/get_mock_paywall.py
--rw-r--r--   0        0        0      346 2023-06-30 16:23:21.701849 stigg_api_client_v2-0.470.0/stigg/generated/get_paywall.py
--rw-r--r--   0        0        0      657 2023-06-30 16:23:21.737470 stigg_api_client_v2-0.470.0/stigg/generated/get_products.py
--rw-r--r--   0        0        0      650 2023-06-30 16:23:21.752892 stigg_api_client_v2-0.470.0/stigg/generated/get_sdk_configuration.py
--rw-r--r--   0        0        0      465 2023-06-30 16:23:21.510587 stigg_api_client_v2-0.470.0/stigg/generated/import_customer.py
--rw-r--r--   0        0        0      332 2023-06-30 16:23:21.501488 stigg_api_client_v2-0.470.0/stigg/generated/import_customer_bulk.py
--rw-r--r--   0        0        0      350 2023-06-30 16:23:21.547531 stigg_api_client_v2-0.470.0/stigg/generated/import_subscriptions_bulk.py
--rw-r--r--   0        0        0   126193 2023-06-30 16:23:21.473438 stigg_api_client_v2-0.470.0/stigg/generated/input_types.py
--rw-r--r--   0        0        0      604 2023-06-30 16:23:21.651368 stigg_api_client_v2-0.470.0/stigg/generated/migrate_subscription_to_latest.py
--rw-r--r--   0        0        0     1161 2023-06-30 16:23:21.492844 stigg_api_client_v2-0.470.0/stigg/generated/provision_customer.py
--rw-r--r--   0        0        0      971 2023-06-30 16:23:21.539696 stigg_api_client_v2-0.470.0/stigg/generated/provision_subscription.py
--rw-r--r--   0        0        0      359 2023-06-30 16:23:21.629696 stigg_api_client_v2-0.470.0/stigg/generated/report_entitlement_check_requested.py
--rw-r--r--   0        0        0      301 2023-06-30 16:23:21.622568 stigg_api_client_v2-0.470.0/stigg/generated/report_event.py
--rw-r--r--   0        0        0      637 2023-06-30 16:23:21.614976 stigg_api_client_v2-0.470.0/stigg/generated/report_usage.py
--rw-r--r--   0        0        0      220 2023-06-30 16:23:23.241030 stigg_api_client_v2-0.470.0/stigg/generated/scalars.py
--rw-r--r--   0        0        0      465 2023-06-30 16:23:21.520747 stigg_api_client_v2-0.470.0/stigg/generated/update_customer.py
--rw-r--r--   0        0        0      527 2023-06-30 16:23:21.558933 stigg_api_client_v2-0.470.0/stigg/generated/update_subscription.py
--rw-r--r--   0        0        0      445 2023-06-30 16:23:21.791442 stigg_api_client_v2-0.470.0/stigg/generated/usage_history.py
--rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.470.0/PKG-INFO
+-rw-r--r--   0        0        0     1644 2023-07-02 07:42:22.738785 stigg_api_client_v2-0.471.0/README.md
+-rw-r--r--   0        0        0      432 2023-07-02 07:43:15.147136 stigg_api_client_v2-0.471.0/pyproject.toml
+-rw-r--r--   0        0        0       62 2023-07-02 07:42:22.738785 stigg_api_client_v2-0.471.0/stigg/__init__.py
+-rw-r--r--   0        0        0     1520 2023-07-02 07:42:22.742785 stigg_api_client_v2-0.471.0/stigg/client.py
+-rw-r--r--   0        0        0    39399 2023-07-02 07:43:13.307132 stigg_api_client_v2-0.471.0/stigg/generated/__init__.py
+-rw-r--r--   0        0        0     7303 2023-07-02 07:43:12.903130 stigg_api_client_v2-0.471.0/stigg/generated/async_base_client.py
+-rw-r--r--   0        0        0    66201 2023-07-02 07:43:13.131131 stigg_api_client_v2-0.471.0/stigg/generated/async_client.py
+-rw-r--r--   0        0        0     2731 2023-07-02 07:43:07.559094 stigg_api_client_v2-0.471.0/stigg/generated/base_client.py
+-rw-r--r--   0        0        0     1951 2023-07-02 07:43:12.903130 stigg_api_client_v2-0.471.0/stigg/generated/base_model.py
+-rw-r--r--   0        0        0      527 2023-07-02 07:43:11.903123 stigg_api_client_v2-0.471.0/stigg/generated/cancel_subscription.py
+-rw-r--r--   0        0        0      296 2023-07-02 07:43:11.923123 stigg_api_client_v2-0.471.0/stigg/generated/cancel_subscription_updates.py
+-rw-r--r--   0        0        0    65786 2023-07-02 07:43:07.791096 stigg_api_client_v2-0.471.0/stigg/generated/client.py
+-rw-r--r--   0        0        0      527 2023-07-02 07:43:11.947123 stigg_api_client_v2-0.471.0/stigg/generated/create_subscription.py
+-rw-r--r--   0        0        0    23994 2023-07-02 07:43:09.355106 stigg_api_client_v2-0.471.0/stigg/generated/enums.py
+-rw-r--r--   0        0        0      553 2023-07-02 07:43:11.911123 stigg_api_client_v2-0.471.0/stigg/generated/estimate_subscription.py
+-rw-r--r--   0        0        0      614 2023-07-02 07:43:11.915123 stigg_api_client_v2-0.471.0/stigg/generated/estimate_subscription_update.py
+-rw-r--r--   0        0        0     2366 2023-07-02 07:43:12.903130 stigg_api_client_v2-0.471.0/stigg/generated/exceptions.py
+-rw-r--r--   0        0        0    53605 2023-07-02 07:43:12.899130 stigg_api_client_v2-0.471.0/stigg/generated/fragments.py
+-rw-r--r--   0        0        0      591 2023-07-02 07:43:11.971124 stigg_api_client_v2-0.471.0/stigg/generated/get_active_subscriptions.py
+-rw-r--r--   0        0        0      634 2023-07-02 07:43:11.979124 stigg_api_client_v2-0.471.0/stigg/generated/get_coupons.py
+-rw-r--r--   0        0        0      572 2023-07-02 07:43:11.963123 stigg_api_client_v2-0.471.0/stigg/generated/get_customer_by_id.py
+-rw-r--r--   0        0        0      533 2023-07-02 07:43:12.023124 stigg_api_client_v2-0.471.0/stigg/generated/get_customer_portal_by_ref_id.py
+-rw-r--r--   0        0        0      390 2023-07-02 07:43:11.995124 stigg_api_client_v2-0.471.0/stigg/generated/get_entitlement.py
+-rw-r--r--   0        0        0      430 2023-07-02 07:43:11.991124 stigg_api_client_v2-0.471.0/stigg/generated/get_entitlements.py
+-rw-r--r--   0        0        0      893 2023-07-02 07:43:12.031124 stigg_api_client_v2-0.471.0/stigg/generated/get_mock_paywall.py
+-rw-r--r--   0        0        0      346 2023-07-02 07:43:11.983124 stigg_api_client_v2-0.471.0/stigg/generated/get_paywall.py
+-rw-r--r--   0        0        0      657 2023-07-02 07:43:12.007124 stigg_api_client_v2-0.471.0/stigg/generated/get_products.py
+-rw-r--r--   0        0        0      650 2023-07-02 07:43:12.015124 stigg_api_client_v2-0.471.0/stigg/generated/get_sdk_configuration.py
+-rw-r--r--   0        0        0      465 2023-07-02 07:43:11.867123 stigg_api_client_v2-0.471.0/stigg/generated/import_customer.py
+-rw-r--r--   0        0        0      332 2023-07-02 07:43:11.859123 stigg_api_client_v2-0.471.0/stigg/generated/import_customer_bulk.py
+-rw-r--r--   0        0        0      350 2023-07-02 07:43:11.891123 stigg_api_client_v2-0.471.0/stigg/generated/import_subscriptions_bulk.py
+-rw-r--r--   0        0        0   126193 2023-07-02 07:43:11.839123 stigg_api_client_v2-0.471.0/stigg/generated/input_types.py
+-rw-r--r--   0        0        0      604 2023-07-02 07:43:11.955124 stigg_api_client_v2-0.471.0/stigg/generated/migrate_subscription_to_latest.py
+-rw-r--r--   0        0        0     1161 2023-07-02 07:43:11.855123 stigg_api_client_v2-0.471.0/stigg/generated/provision_customer.py
+-rw-r--r--   0        0        0      971 2023-07-02 07:43:11.883123 stigg_api_client_v2-0.471.0/stigg/generated/provision_subscription.py
+-rw-r--r--   0        0        0      359 2023-07-02 07:43:11.943123 stigg_api_client_v2-0.471.0/stigg/generated/report_entitlement_check_requested.py
+-rw-r--r--   0        0        0      301 2023-07-02 07:43:11.939123 stigg_api_client_v2-0.471.0/stigg/generated/report_event.py
+-rw-r--r--   0        0        0      637 2023-07-02 07:43:11.931123 stigg_api_client_v2-0.471.0/stigg/generated/report_usage.py
+-rw-r--r--   0        0        0      220 2023-07-02 07:43:12.907130 stigg_api_client_v2-0.471.0/stigg/generated/scalars.py
+-rw-r--r--   0        0        0      465 2023-07-02 07:43:11.871123 stigg_api_client_v2-0.471.0/stigg/generated/update_customer.py
+-rw-r--r--   0        0        0      527 2023-07-02 07:43:11.895123 stigg_api_client_v2-0.471.0/stigg/generated/update_subscription.py
+-rw-r--r--   0        0        0      445 2023-07-02 07:43:12.039124 stigg_api_client_v2-0.471.0/stigg/generated/usage_history.py
+-rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.471.0/PKG-INFO
```

### Comparing `stigg_api_client_v2-0.470.0/README.md` & `stigg_api_client_v2-0.471.0/README.md`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.470.0/stigg/client.py` & `stigg_api_client_v2-0.471.0/stigg/client.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.470.0/stigg/generated/__init__.py` & `stigg_api_client_v2-0.471.0/stigg/generated/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-30 19:23
+# Generated by ariadne-codegen on 2023-07-02 07:43
 
 from .async_base_client import AsyncBaseClient
 from .async_client import AsyncClient
 from .base_model import BaseModel
 from .cancel_subscription import (
     CancelSubscription,
     CancelSubscriptionCancelSubscription,
```

### Comparing `stigg_api_client_v2-0.470.0/stigg/generated/async_base_client.py` & `stigg_api_client_v2-0.471.0/stigg/generated/async_base_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-30 19:23
+# Generated by ariadne-codegen on 2023-07-02 07:43
 
 import enum
 import json
 from typing import Any, AsyncIterator, Dict, Optional, TypeVar, cast
 from uuid import uuid4
 
 import httpx
```

### Comparing `stigg_api_client_v2-0.470.0/stigg/generated/async_client.py` & `stigg_api_client_v2-0.471.0/stigg/generated/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-30 19:23
+# Generated by ariadne-codegen on 2023-07-02 07:43
 # Source: operations.graphql
 
 from .async_base_client import AsyncBaseClient
 from .cancel_subscription import CancelSubscription
 from .cancel_subscription_updates import CancelSubscriptionUpdates
 from .create_subscription import CreateSubscription
 from .estimate_subscription import EstimateSubscription
```

### Comparing `stigg_api_client_v2-0.470.0/stigg/generated/base_client.py` & `stigg_api_client_v2-0.471.0/stigg/generated/base_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-30 19:23
+# Generated by ariadne-codegen on 2023-07-02 07:43
 
 import json
 from typing import Any, Dict, Optional, TypeVar, cast
 
 import httpx
 from pydantic import BaseModel
 from pydantic.json import pydantic_encoder
```

### Comparing `stigg_api_client_v2-0.470.0/stigg/generated/base_model.py` & `stigg_api_client_v2-0.471.0/stigg/generated/base_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-30 19:23
+# Generated by ariadne-codegen on 2023-07-02 07:43
 
 from typing import Any, Dict, Type, Union, get_args, get_origin
 
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic.class_validators import validator
 from pydantic.fields import ModelField
```

### Comparing `stigg_api_client_v2-0.470.0/stigg/generated/cancel_subscription.py` & `stigg_api_client_v2-0.471.0/stigg/generated/cancel_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-30 19:23
+# Generated by ariadne-codegen on 2023-07-02 07:43
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.470.0/stigg/generated/client.py` & `stigg_api_client_v2-0.471.0/stigg/generated/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-30 19:23
+# Generated by ariadne-codegen on 2023-07-02 07:43
 # Source: operations.graphql
 
 from .base_client import BaseClient
 from .cancel_subscription import CancelSubscription
 from .cancel_subscription_updates import CancelSubscriptionUpdates
 from .create_subscription import CreateSubscription
 from .estimate_subscription import EstimateSubscription
```

### Comparing `stigg_api_client_v2-0.470.0/stigg/generated/create_subscription.py` & `stigg_api_client_v2-0.471.0/stigg/generated/create_subscription.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-30 19:23
+# Generated by ariadne-codegen on 2023-07-02 07:43
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.470.0/stigg/generated/enums.py` & `stigg_api_client_v2-0.471.0/stigg/generated/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-30 19:23
+# Generated by ariadne-codegen on 2023-07-02 07:43
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from enum import Enum
 
 
 class AccessDeniedReason(str, Enum):
     CustomerNotFound = "CustomerNotFound"
```

### Comparing `stigg_api_client_v2-0.470.0/stigg/generated/estimate_subscription.py` & `stigg_api_client_v2-0.471.0/stigg/generated/estimate_subscription.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-30 19:23
+# Generated by ariadne-codegen on 2023-07-02 07:43
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.470.0/stigg/generated/estimate_subscription_update.py` & `stigg_api_client_v2-0.471.0/stigg/generated/estimate_subscription_update.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-30 19:23
+# Generated by ariadne-codegen on 2023-07-02 07:43
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.470.0/stigg/generated/exceptions.py` & `stigg_api_client_v2-0.471.0/stigg/generated/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-30 19:23
+# Generated by ariadne-codegen on 2023-07-02 07:43
 
 from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
 
 class GraphQLClientError(Exception):
```

### Comparing `stigg_api_client_v2-0.470.0/stigg/generated/fragments.py` & `stigg_api_client_v2-0.471.0/stigg/generated/fragments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-30 19:23
+# Generated by ariadne-codegen on 2023-07-02 07:43
 # Source: operations.graphql
 
 from typing import Annotated, Any, List, Literal, Optional, Union
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -337,14 +337,18 @@
     has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
     usage_limit: Optional[float] = Field(alias="usageLimit")
     period: PromotionalEntitlementPeriod
     start_date: Any = Field(alias="startDate")
     end_date: Optional[Any] = Field(alias="endDate")
 
 
+class CustomerResourceFragment(BaseModel):
+    resource_id: str = Field(alias="resourceId")
+
+
 class CustomerPortalSubscriptionScheduledUpdateData(BaseModel):
     subscription_schedule_type: SubscriptionScheduleType = Field(
         alias="subscriptionScheduleType"
     )
     schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
     scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
     target_package: Optional[
@@ -471,18 +475,14 @@
 
 class CustomerPortalSubscriptionFragmentScheduledUpdates(
     CustomerPortalSubscriptionScheduledUpdateData
 ):
     pass
 
 
-class CustomerResourceFragment(BaseModel):
-    resource_id: str = Field(alias="resourceId")
-
-
 class CustomerPortalFragment(BaseModel):
     subscriptions: List["CustomerPortalFragmentSubscriptions"]
     entitlements: List["CustomerPortalFragmentEntitlements"]
     promotional_entitlements: List[
         "CustomerPortalFragmentPromotionalEntitlements"
     ] = Field(alias="promotionalEntitlements")
     billing_information: "CustomerPortalFragmentBillingInformation" = Field(
@@ -517,65 +517,14 @@
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
 class ProductFragment(BaseModel):
     ref_id: str = Field(alias="refId")
     display_name: Optional[str] = Field(alias="displayName")
     description: Optional[str]
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
     product_settings: "ProductFragmentProductSettings" = Field(alias="productSettings")
 
@@ -655,14 +604,65 @@
 
 
 class TotalPriceFragmentTotal(BaseModel):
     amount: float
     currency: Currency
 
 
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
@@ -1318,14 +1318,15 @@
 CustomerPortalConfigurationFragmentTypography.update_forward_refs()
 FeatureFragment.update_forward_refs()
 CustomerPortalEntitlement.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationMonthlyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationWeeklyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementFeature.update_forward_refs()
 CustomerPortalPromotionalEntitlement.update_forward_refs()
+CustomerResourceFragment.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateData.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionAddon.update_forward_refs()
 CustomerPortalSubscriptionFragment.update_forward_refs()
@@ -1335,41 +1336,40 @@
 CustomerPortalSubscriptionFragmentBillingPeriodRange.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPrice.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceSubTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceAddonsTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentAddons.update_forward_refs()
 CustomerPortalSubscriptionFragmentScheduledUpdates.update_forward_refs()
-CustomerResourceFragment.update_forward_refs()
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
 TotalPriceFragment.update_forward_refs()
 TotalPriceFragmentSubTotal.update_forward_refs()
 TotalPriceFragmentTotal.update_forward_refs()
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
@@ -1385,19 +1385,19 @@
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

### Comparing `stigg_api_client_v2-0.470.0/stigg/generated/get_active_subscriptions.py` & `stigg_api_client_v2-0.471.0/stigg/generated/get_active_subscriptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-30 19:23
+# Generated by ariadne-codegen on 2023-07-02 07:43
 # Source: operations.graphql
 
 from typing import List
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.470.0/stigg/generated/get_coupons.py` & `stigg_api_client_v2-0.471.0/stigg/generated/get_coupons.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-30 19:23
+# Generated by ariadne-codegen on 2023-07-02 07:43
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import CouponFragment
```

### Comparing `stigg_api_client_v2-0.470.0/stigg/generated/get_customer_portal_by_ref_id.py` & `stigg_api_client_v2-0.471.0/stigg/generated/get_customer_portal_by_ref_id.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-30 19:23
+# Generated by ariadne-codegen on 2023-07-02 07:43
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import CustomerPortalFragment
```

### Comparing `stigg_api_client_v2-0.470.0/stigg/generated/get_mock_paywall.py` & `stigg_api_client_v2-0.471.0/stigg/generated/get_mock_paywall.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-30 19:23
+# Generated by ariadne-codegen on 2023-07-02 07:43
 # Source: operations.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.470.0/stigg/generated/get_products.py` & `stigg_api_client_v2-0.471.0/stigg/generated/get_products.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-30 19:23
+# Generated by ariadne-codegen on 2023-07-02 07:43
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import ProductFragment
```

### Comparing `stigg_api_client_v2-0.470.0/stigg/generated/get_sdk_configuration.py` & `stigg_api_client_v2-0.471.0/stigg/generated/get_sdk_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-30 19:23
+# Generated by ariadne-codegen on 2023-07-02 07:43
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.470.0/stigg/generated/input_types.py` & `stigg_api_client_v2-0.471.0/stigg/generated/input_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-30 19:23
+# Generated by ariadne-codegen on 2023-07-02 07:43
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from typing import Any, List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.470.0/stigg/generated/migrate_subscription_to_latest.py` & `stigg_api_client_v2-0.471.0/stigg/generated/migrate_subscription_to_latest.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-30 19:23
+# Generated by ariadne-codegen on 2023-07-02 07:43
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.470.0/stigg/generated/provision_customer.py` & `stigg_api_client_v2-0.471.0/stigg/generated/provision_customer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-30 19:23
+# Generated by ariadne-codegen on 2023-07-02 07:43
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.470.0/stigg/generated/provision_subscription.py` & `stigg_api_client_v2-0.471.0/stigg/generated/provision_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-30 19:23
+# Generated by ariadne-codegen on 2023-07-02 07:43
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.470.0/stigg/generated/report_usage.py` & `stigg_api_client_v2-0.471.0/stigg/generated/report_usage.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-30 19:23
+# Generated by ariadne-codegen on 2023-07-02 07:43
 # Source: operations.graphql
 
 from typing import Any, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.470.0/stigg/generated/update_subscription.py` & `stigg_api_client_v2-0.471.0/stigg/generated/update_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-30 19:23
+# Generated by ariadne-codegen on 2023-07-02 07:43
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.470.0/PKG-INFO` & `stigg_api_client_v2-0.471.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stigg-api-client-v2
-Version: 0.470.0
+Version: 0.471.0
 Summary: 
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

