# Comparing `tmp/igz_mgmt-0.0.8.tar.gz` & `tmp/igz_mgmt-0.0.9.tar.gz`

## Comparing `igz_mgmt-0.0.8.tar` & `igz_mgmt-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 igz_mgmt-0.0.8/igz_mgmt/__init__.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 igz_mgmt-0.0.8/igz_mgmt/__version__.py
--rw-r--r--   0        0        0    16269 2020-02-02 00:00:00.000000 igz_mgmt-0.0.8/igz_mgmt/client.py
--rw-r--r--   0        0        0     6478 2020-02-02 00:00:00.000000 igz_mgmt-0.0.8/igz_mgmt/constants.py
--rw-r--r--   0        0        0     5545 2020-02-02 00:00:00.000000 igz_mgmt-0.0.8/igz_mgmt/cruds.py
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 igz_mgmt-0.0.8/igz_mgmt/exceptions.py
--rw-r--r--   0        0        0    10302 2020-02-02 00:00:00.000000 igz_mgmt-0.0.8/igz_mgmt/operations.py
--rw-r--r--   0        0        0    47741 2020-02-02 00:00:00.000000 igz_mgmt-0.0.8/igz_mgmt/resources.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 igz_mgmt-0.0.8/igz_mgmt/common/__init__.py
--rw-r--r--   0        0        0     6686 2020-02-02 00:00:00.000000 igz_mgmt-0.0.8/igz_mgmt/common/helpers.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 igz_mgmt-0.0.8/igz_mgmt/logger/__init__.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 igz_mgmt-0.0.8/igz_mgmt/logger/logger.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 igz_mgmt-0.0.8/igz_mgmt/schemas/__init__.py
--rw-r--r--   0        0        0    11993 2020-02-02 00:00:00.000000 igz_mgmt-0.0.8/igz_mgmt/schemas/app_services.py
--rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 igz_mgmt-0.0.8/igz_mgmt/schemas/manual_events.py
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 igz_mgmt-0.0.8/LICENSE
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 igz_mgmt-0.0.8/README.md
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 igz_mgmt-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 igz_mgmt-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 igz_mgmt-0.0.9/igz_mgmt/__init__.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 igz_mgmt-0.0.9/igz_mgmt/__version__.py
+-rw-r--r--   0        0        0    16269 2020-02-02 00:00:00.000000 igz_mgmt-0.0.9/igz_mgmt/client.py
+-rw-r--r--   0        0        0     6478 2020-02-02 00:00:00.000000 igz_mgmt-0.0.9/igz_mgmt/constants.py
+-rw-r--r--   0        0        0     6075 2020-02-02 00:00:00.000000 igz_mgmt-0.0.9/igz_mgmt/cruds.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 igz_mgmt-0.0.9/igz_mgmt/exceptions.py
+-rw-r--r--   0        0        0    10884 2020-02-02 00:00:00.000000 igz_mgmt-0.0.9/igz_mgmt/operations.py
+-rw-r--r--   0        0        0    54629 2020-02-02 00:00:00.000000 igz_mgmt-0.0.9/igz_mgmt/resources.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 igz_mgmt-0.0.9/igz_mgmt/common/__init__.py
+-rw-r--r--   0        0        0     6686 2020-02-02 00:00:00.000000 igz_mgmt-0.0.9/igz_mgmt/common/helpers.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 igz_mgmt-0.0.9/igz_mgmt/logger/__init__.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 igz_mgmt-0.0.9/igz_mgmt/logger/logger.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 igz_mgmt-0.0.9/igz_mgmt/schemas/__init__.py
+-rw-r--r--   0        0        0    12342 2020-02-02 00:00:00.000000 igz_mgmt-0.0.9/igz_mgmt/schemas/app_services.py
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 igz_mgmt-0.0.9/igz_mgmt/schemas/events.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 igz_mgmt-0.0.9/igz_mgmt/schemas/manual_events.py
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 igz_mgmt-0.0.9/LICENSE
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 igz_mgmt-0.0.9/README.md
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 igz_mgmt-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 igz_mgmt-0.0.9/PKG-INFO
```

### Comparing `igz_mgmt-0.0.8/igz_mgmt/__init__.py` & `igz_mgmt-0.0.9/igz_mgmt/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,15 +20,14 @@
     JupyterSpec,
     ScaleResource,
     ScaleToZeroSpec,
 )
 from igz_mgmt.schemas.app_services import (
     ScaleToZeroSpecPresets as AppServiceScaleToZeroSpecPresets,
 )
-from igz_mgmt.schemas.manual_events import ManualEventSchema
 
 from .client import APIClient as Client
 from .constants import (
     ApplyServicesMode,
     AppServiceDesiredStates,
     AppServicePriorityClass,
     ForceApplyAllMode,
@@ -38,22 +37,38 @@
     TenantManagementRoles,
     UserAdminStatuses,
     UserOperationalStatuses,
 )
 from .cruds import ResourceListPagingQueryParams
 from .logger import get_or_create_logger
 from .operations import AppServices, ClusterConfigurations, ManualEvents
-from .resources import AccessKey, AppServicesManifest, Group, Job, Project, User
+from .resources import (
+    AccessKey,
+    AppServicesManifest,
+    AuditEvent,
+    CommunicationEvent,
+    Event,
+    Group,
+    Job,
+    Project,
+    User,
+)
+
+# FOR BC
+ManualEventSchema = Event
 
 __all__ = [
     "Client",
     "User",
     "Group",
     "AccessKey",
     "Job",
+    "Event",
+    "AuditEvent",
+    "CommunicationEvent",
     "ClusterConfigurations",
     "AppServicesManifest",
     "AppServiceBase",
     "AppServiceSpec",
     "AppServiceStatus",
     "CustomAppServiceSpec",
     "JupyterSpec",
```

### Comparing `igz_mgmt-0.0.8/igz_mgmt/__version__.py` & `igz_mgmt-0.0.9/igz_mgmt/__version__.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # limitations under the License.
 #
 
 # version can be either one of the following:
 # x.y.z
 # x.y.z.rcN
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
```

### Comparing `igz_mgmt-0.0.8/igz_mgmt/client.py` & `igz_mgmt-0.0.9/igz_mgmt/client.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.0.8/igz_mgmt/constants.py` & `igz_mgmt-0.0.9/igz_mgmt/constants.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.0.8/igz_mgmt/cruds.py` & `igz_mgmt-0.0.9/igz_mgmt/cruds.py`

 * *Files 10% similar despite different names*

```diff
@@ -48,14 +48,20 @@
             return _AccessKeyCrud
         elif crud_type == "job":
             return _JobCrud
         elif crud_type == "app_services_manifest":
             return _AppServicesManifestCrud
         elif crud_type == "project":
             return _ProjectCrud
+        elif crud_type == "event":
+            return _EventCrud
+        elif crud_type == "audit_event":
+            return _AuditEventCrud
+        elif crud_type == "communication_event":
+            return _CommunicationEventCrud
         else:
             raise Exception("Unknown type")
 
 
 class _BaseCrud(abc.ABC):
     __ALLOW_GET_DETAIL__ = True
 
@@ -152,14 +158,18 @@
                     return jobs_data[0].get("id", None)
 
     @classmethod
     def get_custom(cls, http_client: igz_mgmt.client.APIClient, path, **kwargs):
         return http_client.request("GET", path, **kwargs)
 
     @classmethod
+    def post_custom(cls, http_client: igz_mgmt.client.APIClient, path, **kwargs):
+        return http_client.request("POST", path, **kwargs)
+
+    @classmethod
     def type(cls):
         return inflection.underscore(cls.__name__.strip("_")).replace("_crud", "")
 
 
 class _UserCrud(_BaseCrud):
     pass
 
@@ -178,7 +188,19 @@
 
 class _AppServicesManifestCrud(_BaseCrud):
     __ALLOW_GET_DETAIL__ = False
 
 
 class _ProjectCrud(_BaseCrud):
     pass
+
+
+class _EventCrud(_BaseCrud):
+    pass
+
+
+class _AuditEventCrud(_BaseCrud):
+    pass
+
+
+class _CommunicationEventCrud(_BaseCrud):
+    pass
```

### Comparing `igz_mgmt-0.0.8/igz_mgmt/exceptions.py` & `igz_mgmt-0.0.9/igz_mgmt/exceptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,14 +34,21 @@
 class ResourceListException(Exception):
     """The resource is not list-able."""
 
     def __str__(self):
         return "This resource is not list-able"
 
 
+class ResourceGetException(Exception):
+    """The resource is not get-able."""
+
+    def __str__(self):
+        return "This resource is not get-able"
+
+
 class AppServiceNotExistsException(Exception):
     """The app service not exists in app services list.
 
     Args:
         name (str): App service name.
     """
```

### Comparing `igz_mgmt-0.0.8/igz_mgmt/operations.py` & `igz_mgmt-0.0.9/igz_mgmt/operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 import typing
 
 import igz_mgmt.client
 import igz_mgmt.constants
 import igz_mgmt.exceptions
 import igz_mgmt.resources
 import igz_mgmt.schemas.app_services
-import igz_mgmt.schemas.manual_events
 
 
 class ClusterConfigurations(object):
     """Cluster configuration operations."""
 
     @classmethod
     def reload(
@@ -54,44 +53,59 @@
 class ManualEvents(object):
     """Manual event operations."""
 
     @classmethod
     def emit(
         cls,
         http_client: igz_mgmt.client.APIClient,
-        event: igz_mgmt.schemas.manual_events.ManualEventSchema,
+        event: igz_mgmt.resources.Event,
         audit_tenant_id: typing.Optional[str] = None,
+        **kwargs,
     ):
         """Emits a manual event.
 
         This operation requires system-admin role permissions.
 
         Args:
             http_client (APIClient): The client to use.
             event (ManualEventSchema): The event to emit.
             audit_tenant_id: The assigned tenant id for auditing events (required for audit events).
+            kwargs: Additional arguments to pass to the request.
         """
-        relationships = None
+        # we do not want to send the type in the request body as it is part of the manual event request
+        event.type = None
+
+        # set the audit tenant id on relationships
         if audit_tenant_id:
-            relationships = {
-                "audit_tenant": {
-                    "data": {"type": "tenant", "id": audit_tenant_id},
-                },
+            event.relationships = (
+                {} if event.relationships is None else event.relationships
+            )
+            event.relationships.setdefault("audit_tenant", {}).setdefault("data", {})
+            event.relationships["audit_tenant"]["data"] = {
+                "type": "tenant",
+                "id": audit_tenant_id,
             }
 
-        manual_event_request = {
-            "data": {
-                **igz_mgmt.schemas.manual_events.ManualEventRequest(
-                    attributes=event,
-                    relationships=relationships,
-                ).dict(exclude_none=True)
-            }
-        }
+        # empty out relationships as it is not part of the attributes
+        relationships = event.relationships.copy() if event.relationships else {}
+        event.relationships = None
+
         try:
-            http_client.request("POST", "manual_events", json=manual_event_request)
+            http_client.request(
+                "POST",
+                "manual_events",
+                json={
+                    "data": {
+                        "type": "event",
+                        "relationships": relationships,
+                        "attributes": event.dict(exclude_none=True),
+                    },
+                },
+                **kwargs,
+            )
         except json.JSONDecodeError:
             # endpoint is not json on old igz versions
             pass
 
 
 class AppServices(object):
     """Syntactic sugar to AppServicesManifest class."""
```

### Comparing `igz_mgmt-0.0.8/igz_mgmt/resources.py` & `igz_mgmt-0.0.9/igz_mgmt/resources.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,19 +28,21 @@
 import semver
 
 import igz_mgmt.client
 import igz_mgmt.common.helpers
 import igz_mgmt.constants
 import igz_mgmt.cruds
 import igz_mgmt.exceptions
+import igz_mgmt.schemas
 import igz_mgmt.schemas.app_services
+import igz_mgmt.schemas.events
 
 
-class BaseResource(pydantic.BaseModel):
-    """Base resource contains common attributes and methods for resources in the system."""
+class ResourceBaseModel(pydantic.BaseModel):
+    """Base model for all resources."""
 
     type: str
     id: typing.Optional[typing.Union[int, str]]
     relationships: typing.Optional[dict]
 
     class Config:
         class _BaseGetter(pydantic.utils.GetterDict):
@@ -57,14 +59,18 @@
         use_enum_values = True
         underscore_attrs_are_private = True
         getter_dict = _BaseGetter
 
         # be forward compatible
         extra = "allow"
 
+
+class BaseResource(ResourceBaseModel):
+    """Base resource contains common attributes and methods for resources in the system."""
+
     @classmethod
     def get(
         cls,
         http_client: igz_mgmt.client.APIClient,
         resource_id: typing.Union[int, str],
         include: typing.Optional[typing.List[str]] = None,
     ) -> "BaseResource":
@@ -702,15 +708,15 @@
     def create(
         cls,
         http_client: igz_mgmt.client.APIClient,
         planes: typing.List[
             igz_mgmt.constants.SessionPlanes
         ] = igz_mgmt.constants.SessionPlanes.all(),
         label: str = None,
-    ):
+    ) -> "AccessKey":
         """Creates a new access key.
 
         Args:
             http_client (APIClient): The client to use.
             planes (typing.List[SessionPlanes], optional): The planes of the access key.
             label (str, optional): The label of the access key.
         """
@@ -719,14 +725,53 @@
             attributes={
                 "planes": planes,
                 "label": label,
             },
         )
         return cls.from_orm(created_resource)
 
+    @classmethod
+    def get_or_create(
+        cls,
+        http_client: igz_mgmt.client.APIClient,
+        planes: typing.Optional[typing.List[igz_mgmt.constants.SessionPlanes]] = None,
+        label: typing.Optional[str] = None,
+    ) -> "AccessKey":
+        """Get or create access key.
+
+        If access key with the given planes exists, it will be returned.
+        Otherwise, a new access key will be created.
+        If no planes are given, all planes will be used.
+
+        Args:
+            http_client (APIClient): The client to use.
+            planes (typing.List[SessionPlanes], optional): The planes of the access key.
+            label (str, optional): The label of the access key.
+
+        Returns:
+            AccessKey: An existing or newly created access key.
+        """
+        if not planes:
+            planes = igz_mgmt.constants.SessionPlanes.all()
+
+        request_body = {
+            "data": {
+                "type": "access_key",
+                "attributes": {},
+            }
+        }
+        if label:
+            request_body["data"]["attributes"]["label"] = label
+        if planes:
+            request_body["data"]["attributes"]["planes"] = list(map(str, planes))
+        response = cls._get_crud().post_custom(
+            http_client, "/self/get_or_create_access_key", json=request_body
+        )
+        return cls.from_orm(response)
+
 
 class Job(BaseResource):
     """Job is an abstraction for long-running operations in the API.
 
     Some operations, cannot be finished within a reasonable amount of time for a normal HTTP request.
     Job has a state, id and can be awaited on asynchronously.
     """
@@ -1310,7 +1355,162 @@
             relationships["owner"] = {
                 "data": {
                     "type": "user",
                     "id": user_id,
                 },
             }
         return relationships
+
+
+class Event(BaseResource):
+    """Event resource represents events in the system.
+
+    Events are used to notify about changes in the system.
+    """
+
+    type: str = "event"
+
+    source: str = pydantic.Field(
+        description="The originator of the event, in the form of a service ID (e.g. igz0.vn.3)",
+        default="",
+    )
+    kind: str = pydantic.Field(
+        description="A string in dot notation representing which event occurred",
+        default="",
+    )
+    timestamp_uint64: typing.Optional[int] = pydantic.Field(
+        description="64bit timestamp indicating when the event occurred. if 0 and timestampIso8601 is empty,"
+        " the timestamp will added upon reception of the first platform step.",
+        default=None,
+    )
+    timestamp_iso8601: typing.Optional[str] = pydantic.Field(
+        description="string representation of the timestamp, in ISO8601 format",
+        default=None,
+    )
+    timestamp_uint64_str: typing.Optional[str] = pydantic.Field(
+        description="Same as 'timestampUint64' but in string form",
+        default=None,
+    )
+    parameters_uint64: typing.Optional[
+        typing.List[igz_mgmt.schemas.events.ParametersUint64]
+    ] = pydantic.Field(
+        description="A list of parameters, each containing a name and an int value",
+        default=None,
+    )
+    parameters_text: typing.Optional[
+        typing.List[igz_mgmt.schemas.events.ParametersText]
+    ] = pydantic.Field(
+        description="A list of parameters, each containing a name and a string value",
+        default=None,
+    )
+    description: typing.Optional[str] = pydantic.Field(
+        description="A description of the event", default=None
+    )
+    severity: typing.Optional[igz_mgmt.constants.EventSeverity] = pydantic.Field(
+        description="The severity of the event, Required if event kind doesn't exists in the system",
+        default=None,
+    )
+    tags: typing.Optional[typing.List[str]] = pydantic.Field(
+        description="A list of tags to associate with the event, used for later filtering of events/alerts",
+        default=None,
+    )
+    affected_resources: typing.Optional[
+        typing.List[igz_mgmt.schemas.events.AffectedResource]
+    ] = pydantic.Field(
+        description="Resources affected by this event",
+        default=None,
+    )
+    classification: typing.Optional[
+        igz_mgmt.constants.EventClassification
+    ] = pydantic.Field(
+        description="The classification of the event, Required if event kind doesn't exists in the system",
+        default=None,
+    )
+    system_event: typing.Optional[bool] = pydantic.Field(
+        description="Whether this event is a system event or not",
+        default=False,
+    )
+    visibility: typing.Optional[igz_mgmt.constants.EventVisibility] = pydantic.Field(
+        description="Whom the event will be visible to",
+        default=None,
+    )
+
+    @classmethod
+    def delete_all(cls, http_client: igz_mgmt.client.APIClient):
+        """Delete all events.
+
+        Requires Iguazio privileged user.
+
+        Args:
+            http_client (APIClient): The client to use.
+        """
+        cls._get_crud().delete(http_client, "", False)
+
+    def delete(
+        self,
+        http_client: igz_mgmt.client.APIClient,
+        ignore_missing: bool = False,
+        wait_for_job_deletion: bool = True,
+    ) -> typing.Optional["Job"]:
+        """Deleting a single event is not supported."""
+        raise igz_mgmt.exceptions.ResourceDeleteException
+
+    @classmethod
+    def get(
+        cls,
+        http_client: igz_mgmt.client.APIClient,
+        resource_id: typing.Union[int, str],
+        include: typing.Optional[typing.List[str]] = None,
+    ) -> "BaseResource":
+        """Getting an event is not supported."""
+        raise igz_mgmt.exceptions.ResourceGetException
+
+    def update(
+        self, http_client: igz_mgmt.client.APIClient, relationships=None, **kwargs
+    ) -> "BaseResource":
+        """Updating an event is not supported."""
+        raise igz_mgmt.exceptions.ResourceUpdateException
+
+    def emit(self, http_client, **kwargs):
+        """Emit the event.
+
+        Requires system-admin role.
+
+        :param http_client: HTTP client to use
+        """
+        return igz_mgmt.operations.ManualEvents.emit(http_client, event=self, **kwargs)
+
+
+class CommunicationEvent(Event):
+    """CommunicationEvent resource represents internal communication events in the system.
+
+    Communication events are used to communicate between internal components within the system.
+    Their visibility is internal and the classification is usually "sw".
+    """
+
+    type = "communication_event"
+
+
+class AuditEvent(Event):
+    """AuditEvent resource represents audit events in the system.
+
+    Audit events are used to represent user and system actions within the system
+
+    """
+
+    type = "audit_event"
+
+    @classmethod
+    def delete_all(cls, http_client: igz_mgmt.client.APIClient):
+        """Deleting audit events are not supported."""
+        raise igz_mgmt.exceptions.ResourceDeleteException
+
+    def emit(self, http_client, **kwargs):
+        """Emit the event.
+
+        Requires system-admin role.
+
+        :param http_client: HTTP client to use
+        """
+        return igz_mgmt.operations.ManualEvents.emit(
+            http_client, audit_tenant_id=http_client.tenant_id, event=self, **kwargs
+        )
```

### Comparing `igz_mgmt-0.0.8/igz_mgmt/common/__init__.py` & `igz_mgmt-0.0.9/igz_mgmt/common/__init__.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.0.8/igz_mgmt/common/helpers.py` & `igz_mgmt-0.0.9/igz_mgmt/common/helpers.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.0.8/igz_mgmt/logger/__init__.py` & `igz_mgmt-0.0.9/igz_mgmt/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.0.8/igz_mgmt/logger/logger.py` & `igz_mgmt-0.0.9/igz_mgmt/logger/logger.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.0.8/igz_mgmt/schemas/__init__.py` & `igz_mgmt-0.0.9/igz_mgmt/schemas/events.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,16 +8,32 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+
 import pydantic
 
 
-class _Base(pydantic.BaseModel):
-    class Config:
-        # be forward compatible
-        extra = "allow"
-        orm_mode = True
-        use_enum_values = True
+class AffectedResource(pydantic.BaseModel):
+    """Affected resource."""
+
+    type: str
+    id_str: str
+    id: int
+    name: str
+
+
+class ParametersText(pydantic.BaseModel):
+    """Parameters text."""
+
+    name: str
+    value: str
+
+
+class ParametersUint64(pydantic.BaseModel):
+    """Parameters uint64."""
+
+    name: str
+    value: int
```

### Comparing `igz_mgmt-0.0.8/igz_mgmt/schemas/app_services.py` & `igz_mgmt-0.0.9/igz_mgmt/schemas/app_services.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,59 +38,69 @@
         ScaleResource(
             metric_name=igz_mgmt.constants.AppServicesScaleToZeroMetrics.jupyter_kernel_busyness,
             window_size=window_size,
         ),
     ]
 
 
-class CredentialsSpec(igz_mgmt.schemas._Base):
+class AppServicesOperationBaseModel(pydantic.BaseModel):
+    """Base model for all operations."""
+
+    class Config:
+        # be forward compatible
+        extra = "allow"
+        orm_mode = True
+        use_enum_values = True
+
+
+class CredentialsSpec(AppServicesOperationBaseModel):
     """Credentials spec.
 
     Spec for describing credentials with which the app service will preform its operations with in the Iguazio cluster.
     """
 
     username: str = pydantic.Field(description="Iguazio username")
 
 
-class SystemResources(igz_mgmt.schemas._Base):
+class SystemResources(AppServicesOperationBaseModel):
     """System resource description for use with limits and requests."""
 
     cpu: typing.Optional[str]
     memory: typing.Optional[str]
     nvidia_gpu: typing.Optional[str]
 
 
-class ResourcesSpec(igz_mgmt.schemas._Base):
+class ResourcesSpec(AppServicesOperationBaseModel):
     """Resource spec describing the limits and requests for each app service."""
 
     limits: typing.Optional[SystemResources]
     requests: typing.Optional[SystemResources]
 
 
-class ScaleResource(igz_mgmt.schemas._Base):
+class ScaleResource(AppServicesOperationBaseModel):
     """Threshold descriptor for scaling app services to zero."""
 
     metric_name: str = pydantic.Field(description="The threshold metric to watch")
     threshold: int = pydantic.Field(
         0,
         description="The value of the metric where if exceeded, the resource will be scaled",
     )
     window_size: str = pydantic.Field(
         description="The amount of time for which the threshold has to be exceeded for the resource to be scaled"
     )
 
 
-class ScaleToZeroSpec(igz_mgmt.schemas._Base):
+class ScaleToZeroSpec(AppServicesOperationBaseModel):
     """Spec describing the scale to zero resources/rules."""
 
     mode: igz_mgmt.constants.ScaleToZeroMode
     scale_resources: typing.Optional[typing.List[ScaleResource]]
 
 
-class PvcSpec(igz_mgmt.schemas._Base):
+class PvcSpec(AppServicesOperationBaseModel):
     """Pvc - kubernetes persistent volume claim spec for app service pod."""
 
     # TODO: convert mounts entries to dictionary
     mounts: typing.Optional[
         typing.Dict[str, typing.List[typing.Dict[str, str]]]
     ] = pydantic.Field(
         description="Dictionary describing the pvc mounts where the key is a volume and the values \
@@ -124,62 +134,62 @@
     )
     four_hours = ScaleToZeroSpec(
         mode=igz_mgmt.constants.ScaleToZeroMode.enabled,
         scale_resources=generate_scale_to_zero_spec("4h"),
     )
 
 
-class SecurityContextSpec(igz_mgmt.schemas._Base):
+class SecurityContextSpec(AppServicesOperationBaseModel):
     """Kubernetes Security context spec for app service pods."""
 
     run_as_user: str
     run_as_group: str
     fs_group: str
     supplemental_groups: typing.List[str]
     run_as_non_root: bool
 
 
-class AdvancedSpec(igz_mgmt.schemas._Base):
+class AdvancedSpec(AppServicesOperationBaseModel):
     """Advanced app service spec."""
 
     # TODO: convert node_selector entries to dictionary
     # "entries" kind of list. e.g.: {"entries:[{"key":"", "value":""}, ...]}
     node_selector: typing.Optional[typing.Dict[str, typing.List[typing.Dict[str, str]]]]
     priority_class_name: typing.Optional[str] = pydantic.Field(
         description="Use `igz_mgmt.AppServicePriorityClass` enum for the value. \
         However, it is possible to pass any priority class name you want"
     )
 
 
-class Url(igz_mgmt.schemas._Base):
+class Url(AppServicesOperationBaseModel):
     """URL for accessing app services."""
 
     kind: str
     url: str
 
 
-class Meta(igz_mgmt.schemas._Base):
+class Meta(AppServicesOperationBaseModel):
     """App services metadata class."""
 
     labels: typing.Optional[typing.Dict[str, str]] = pydantic.Field(
         description="Labels for the app service. these will be propagated to all the app service resources"
     )
 
     # TODO: convert annotations entries to dictionary
     # annotations: typing.Optional[typing.Dict[str, str]]
 
 
-class StatusErrorInfo(igz_mgmt.schemas._Base):
+class StatusErrorInfo(AppServicesOperationBaseModel):
     """App service Status error info."""
 
     description: str
     timestamp: str
 
 
-class AppServiceStatus(igz_mgmt.schemas._Base):
+class AppServiceStatus(AppServicesOperationBaseModel):
     """App service status."""
 
     state: str
     urls: typing.Optional[typing.List[Url]]
     api_urls: typing.Optional[typing.List[Url]]
     internal_api_urls: typing.Optional[typing.List[Url]]
     version: typing.Optional[str]
@@ -197,29 +207,29 @@
         description="Shell specific app service status"
     )
     jupyter: typing.Optional[typing.Dict[str, typing.Any]] = pydantic.Field(
         description="jupyter specific app service status"
     )
 
 
-class HomeContainer(igz_mgmt.schemas._Base):
+class HomeContainer(AppServicesOperationBaseModel):
     """Home container."""
 
     container: str
     prefix: str
 
 
-class SSHServerSpec(igz_mgmt.schemas._Base):
+class SSHServerSpec(AppServicesOperationBaseModel):
     """SSH configuration for accessing interactive shell app services (e.g. jupyter, shell)."""
 
     force_key_regeneration: bool
     port: int
 
 
-class CustomAppServiceSpec(igz_mgmt.schemas._Base):
+class CustomAppServiceSpec(AppServicesOperationBaseModel):
     """Base class for custom app service spec."""
 
     pass
 
 
 class JupyterSpec(CustomAppServiceSpec):
     """Jupyter app service spec."""
@@ -241,15 +251,15 @@
     ]
     demos_datasets_archive_address: typing.Optional[str]
     docker_registry_name: typing.Optional[str]
     ssh_enabled: typing.Optional[bool]
     ssh_server: typing.Optional[SSHServerSpec]
 
 
-class AppServiceSpec(igz_mgmt.schemas._Base):
+class AppServiceSpec(AppServicesOperationBaseModel):
     """App service spec."""
 
     name: str = pydantic.Field(description="The name of the app service")
     kind: str = pydantic.Field(description="The app service kind (jupyter / shell .. )")
 
     # optional fields
     owner: typing.Optional[str] = pydantic.Field(
@@ -334,13 +344,13 @@
                     self.__fields__[field_name].type_, CustomAppServiceSpec
                 ) and kwargs.get(field_name):
                     kwargs["kind"] = field_name
                     break
         super().__init__(**kwargs)
 
 
-class AppServiceBase(igz_mgmt.schemas._Base):
+class AppServiceBase(AppServicesOperationBaseModel):
     """App service base class."""
 
     spec: AppServiceSpec
     meta: typing.Optional[Meta]
     status: typing.Optional[AppServiceStatus]
```

### Comparing `igz_mgmt-0.0.8/LICENSE` & `igz_mgmt-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.0.8/pyproject.toml` & `igz_mgmt-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.0.8/PKG-INFO` & `igz_mgmt-0.0.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: igz-mgmt
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python SDK For Iguazio Management API
 Project-URL: Homepage, https://github.com/iguazio/igz-mgmt-sdk
 Author-email: Iguazio Platform Team <liranb@iguazio.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

