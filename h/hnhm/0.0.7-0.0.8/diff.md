# Comparing `tmp/hnhm-0.0.7.tar.gz` & `tmp/hnhm-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hnhm-0.0.7.tar", max compression
+gzip compressed data, was "hnhm-0.0.8.tar", max compression
```

## Comparing `hnhm-0.0.7.tar` & `hnhm-0.0.8.tar`

### file list

```diff
@@ -1,36 +1,37 @@
--rw-r--r--   0        0        0      707 2023-05-18 14:47:59.411816 hnhm-0.0.7/hnhm/__init__.py
--rw-r--r--   0        0        0     1481 2023-05-18 14:47:59.411816 hnhm-0.0.7/hnhm/cli.py
--rw-r--r--   0        0        0      648 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/core/__init__.py
--rw-r--r--   0        0        0     1139 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/core/attribute.py
--rw-r--r--   0        0        0      627 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/core/entity.py
--rw-r--r--   0        0        0       80 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/core/error.py
--rw-r--r--   0        0        0      553 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/core/group.py
--rw-r--r--   0        0        0      543 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/core/layout.py
--rw-r--r--   0        0        0      654 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/core/link.py
--rw-r--r--   0        0        0     3147 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/core/migrations.py
--rw-r--r--   0        0        0       94 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/core/priority.py
--rw-r--r--   0        0        0      517 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/core/sql.py
--rw-r--r--   0        0        0     2776 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/core/storage.py
--rw-r--r--   0        0        0     2253 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/core/tasks.py
--rw-r--r--   0        0        0      567 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/file_storage.py
--rw-r--r--   0        0        0     8724 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/flow.py
--rw-r--r--   0        0        0    12112 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/hnhm.py
--rw-r--r--   0        0        0      894 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/hnhm_attribute.py
--rw-r--r--   0        0        0     3915 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/hnhm_entity.py
--rw-r--r--   0        0        0     2564 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/hnhm_link.py
--rw-r--r--   0        0        0     1297 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/hnhm_registry.py
--rw-r--r--   0        0        0     7419 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/plan_printer.py
--rw-r--r--   0        0        0        0 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/postgres/__init__.py
--rw-r--r--   0        0        0    14036 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/postgres/sql.py
--rw-r--r--   0        0        0      488 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/postgres/sql_templates/create_attribute.sql
--rw-r--r--   0        0        0      513 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/postgres/sql_templates/create_group.sql
--rw-r--r--   0        0        0      310 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/postgres/sql_templates/create_hub.sql
--rw-r--r--   0        0        0      540 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/postgres/sql_templates/create_link.sql
--rw-r--r--   0        0        0      192 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/postgres/sql_templates/create_stage.sql
--rw-r--r--   0        0        0      474 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/postgres/sql_templates/load_hub.sql
--rw-r--r--   0        0        0      946 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/postgres/sql_templates/load_ignore.sql
--rw-r--r--   0        0        0     4530 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/postgres/sql_templates/load_new.sql
--rw-r--r--   0        0        0     2103 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/postgres/sql_templates/load_update.sql
--rw-r--r--   0        0        0      781 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/postgres/sql_templates/update_entity_view.sql
--rw-r--r--   0        0        0      806 2023-05-18 14:47:59.419816 hnhm-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      511 1970-01-01 00:00:00.000000 hnhm-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     5111 2023-07-02 15:15:47.065577 hnhm-0.0.8/README.md
+-rw-r--r--   0        0        0      657 2023-07-02 15:15:47.065577 hnhm-0.0.8/hnhm/__init__.py
+-rw-r--r--   0        0        0     1853 2023-07-02 15:15:47.065577 hnhm-0.0.8/hnhm/cli.py
+-rw-r--r--   0        0        0      523 2023-07-02 15:15:47.065577 hnhm-0.0.8/hnhm/core/__init__.py
+-rw-r--r--   0        0        0     1159 2023-07-02 15:15:47.065577 hnhm-0.0.8/hnhm/core/attribute.py
+-rw-r--r--   0        0        0      614 2023-07-02 15:15:47.065577 hnhm-0.0.8/hnhm/core/entity.py
+-rw-r--r--   0        0        0       80 2023-07-02 15:15:47.065577 hnhm-0.0.8/hnhm/core/error.py
+-rw-r--r--   0        0        0      553 2023-07-02 15:15:47.065577 hnhm-0.0.8/hnhm/core/group.py
+-rw-r--r--   0        0        0      543 2023-07-02 15:15:47.065577 hnhm-0.0.8/hnhm/core/layout.py
+-rw-r--r--   0        0        0      666 2023-07-02 15:15:47.065577 hnhm-0.0.8/hnhm/core/link.py
+-rw-r--r--   0        0        0     3147 2023-07-02 15:15:47.065577 hnhm-0.0.8/hnhm/core/migration.py
+-rw-r--r--   0        0        0       94 2023-07-02 15:15:47.065577 hnhm-0.0.8/hnhm/core/priority.py
+-rw-r--r--   0        0        0      692 2023-07-02 15:15:47.065577 hnhm-0.0.8/hnhm/core/sql.py
+-rw-r--r--   0        0        0     2880 2023-07-02 15:15:47.065577 hnhm-0.0.8/hnhm/core/state.py
+-rw-r--r--   0        0        0     2253 2023-07-02 15:15:47.065577 hnhm-0.0.8/hnhm/core/task.py
+-rw-r--r--   0        0        0      547 2023-07-02 15:15:47.065577 hnhm-0.0.8/hnhm/file_state.py
+-rw-r--r--   0        0        0     8662 2023-07-02 15:15:47.065577 hnhm-0.0.8/hnhm/flow.py
+-rw-r--r--   0        0        0    12469 2023-07-02 15:15:47.065577 hnhm-0.0.8/hnhm/hnhm.py
+-rw-r--r--   0        0        0      969 2023-07-02 15:15:47.069577 hnhm-0.0.8/hnhm/hnhm_attribute.py
+-rw-r--r--   0        0        0     3865 2023-07-02 15:15:47.069577 hnhm-0.0.8/hnhm/hnhm_entity.py
+-rw-r--r--   0        0        0     2587 2023-07-02 15:15:47.069577 hnhm-0.0.8/hnhm/hnhm_link.py
+-rw-r--r--   0        0        0     1360 2023-07-02 15:15:47.069577 hnhm-0.0.8/hnhm/hnhm_registry.py
+-rw-r--r--   0        0        0     7388 2023-07-02 15:15:47.069577 hnhm-0.0.8/hnhm/plan_printer.py
+-rw-r--r--   0        0        0        0 2023-07-02 15:15:47.069577 hnhm-0.0.8/hnhm/postgres/__init__.py
+-rw-r--r--   0        0        0    13860 2023-07-02 15:15:47.069577 hnhm-0.0.8/hnhm/postgres/sql.py
+-rw-r--r--   0        0        0      488 2023-07-02 15:15:47.069577 hnhm-0.0.8/hnhm/postgres/sql_templates/create_attribute.sql
+-rw-r--r--   0        0        0      513 2023-07-02 15:15:47.069577 hnhm-0.0.8/hnhm/postgres/sql_templates/create_group.sql
+-rw-r--r--   0        0        0      310 2023-07-02 15:15:47.069577 hnhm-0.0.8/hnhm/postgres/sql_templates/create_hub.sql
+-rw-r--r--   0        0        0      540 2023-07-02 15:15:47.069577 hnhm-0.0.8/hnhm/postgres/sql_templates/create_link.sql
+-rw-r--r--   0        0        0      192 2023-07-02 15:15:47.069577 hnhm-0.0.8/hnhm/postgres/sql_templates/create_stage.sql
+-rw-r--r--   0        0        0      474 2023-07-02 15:15:47.069577 hnhm-0.0.8/hnhm/postgres/sql_templates/load_hub.sql
+-rw-r--r--   0        0        0      946 2023-07-02 15:15:47.069577 hnhm-0.0.8/hnhm/postgres/sql_templates/load_ignore.sql
+-rw-r--r--   0        0        0     4530 2023-07-02 15:15:47.069577 hnhm-0.0.8/hnhm/postgres/sql_templates/load_new.sql
+-rw-r--r--   0        0        0     2103 2023-07-02 15:15:47.069577 hnhm-0.0.8/hnhm/postgres/sql_templates/load_update.sql
+-rw-r--r--   0        0        0      781 2023-07-02 15:15:47.069577 hnhm-0.0.8/hnhm/postgres/sql_templates/update_entity_view.sql
+-rw-r--r--   0        0        0     1014 2023-07-02 15:15:47.069577 hnhm-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     5674 1970-01-01 00:00:00.000000 hnhm-0.0.8/PKG-INFO
```

### Comparing `hnhm-0.0.7/hnhm/cli.py` & `hnhm-0.0.8/hnhm/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,38 @@
-import sys
 import importlib
 
 import click
 
 from .core import HnhmError
-from .plan_printer import print_plan
 from .hnhm_registry import HnhmRegistry
+from .plan_printer import Color, print_plan
 
 
 def import_registry(module: str) -> HnhmRegistry:
-    sys.path.append(".")
+    if module == ".":
+        raise HnhmError(
+            "Importing from the current directory '.' is not supported. "
+            "Please, use the hnhm from the parent directory."
+        )
+
+    module = module.rstrip("/").lstrip("/")
+    module = f"{module}.__hnhm__"
+
+    click.secho(
+        f"Importing 'registry' object from the module: '{module}'.",
+        fg=Color.cyan,
+    )
+    click.secho()
     imported_module = importlib.import_module(module)
-    registry: HnhmRegistry = getattr(imported_module, "__registry__", None)
+
+    registry: HnhmRegistry = getattr(imported_module, "registry", None)
     if not registry:
         raise HnhmError(
             f"Failed to import registry from module: '{module}'."
-            " Please, specify your registry via __registry__ object in your DWH module."
+            " Please, specify your registry via 'registry' object in your DWH module."
         )
     return registry
 
 
 @click.group()
 def cli():
     pass
```

### Comparing `hnhm-0.0.7/hnhm/core/attribute.py` & `hnhm-0.0.8/hnhm/core/attribute.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 
 class Type(str, Enum):
     """Attribute type."""
 
     STRING = "STRING"
     INTEGER = "INTEGER"
+    FLOAT = "FLOAT"
     TIMESTAMP = "TIMESTAMP"
 
     def __str__(self):
         return self.name
 
 
 class ChangeType(str, Enum):
```

### Comparing `hnhm-0.0.7/hnhm/core/entity.py` & `hnhm-0.0.8/hnhm/core/entity.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 from .layout import Layout
 from .attribute import Attribute
 
 
 class Entity(pydantic.BaseModel):
     """Entity core representation."""
 
+    fqn: str
     name: str
     layout: Layout
     doc: str
     keys: list[Attribute]
     attributes: dict[str, Attribute]
     groups: dict[str, Group]
 
     @property
     def sk(self) -> str:
         return f"{self.name}_sk"
 
     def __str__(self):
-        return f"<Entity '{self.name}' layout='{self.layout}'>"
+        return f"<Entity '{self.fqn}' layout='{self.layout}'>"
 
     def __hash__(self):
-        return hash(f"{self.name}_{self.layout.type}")
+        return hash(self.fqn)
 
     def __eq__(self, other):
         return hash(self) == hash(other)
```

### Comparing `hnhm-0.0.7/hnhm/core/group.py` & `hnhm-0.0.8/hnhm/core/group.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.7/hnhm/core/layout.py` & `hnhm-0.0.8/hnhm/core/layout.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.7/hnhm/core/link.py` & `hnhm-0.0.8/hnhm/core/link.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,15 +19,16 @@
     def __eq__(self, other):
         return hash(self) == hash(other)
 
 
 class Link(pydantic.BaseModel):
     """Link core representation."""
 
+    fqn: str
     name: str
     doc: str
     layout: Layout
     elements: list[LinkElement]
     keys: list[LinkElement]
 
     def __str__(self):
-        return f"<Link '{self.name}' layout='{self.layout}'>"
+        return f"<Link '{self.fqn}' layout='{self.layout}'>"
```

### Comparing `hnhm-0.0.7/hnhm/core/migrations.py` & `hnhm-0.0.8/hnhm/core/migration.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.7/hnhm/core/sql.py` & `hnhm-0.0.8/hnhm/core/sql.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 import abc
 
-from .tasks import Task
-from .migrations import Migration
+from .task import Task
+from .migration import Migration
 
 
 class Sql(abc.ABC):
     """Generates and executes sql code."""
 
     @abc.abstractmethod
     def generate_sql(self, migration_or_task: Migration | Task) -> str:
         raise NotImplementedError
 
     @abc.abstractmethod
     def execute(self, sql: str):
         raise NotImplementedError
 
+    @abc.abstractmethod
+    def execute_many(self, sql: str, values: list):
+        raise NotImplementedError
+
 
 class FakeSql(Sql):
     def generate_sql(self, migration_or_task: Migration | Task) -> str:
         return ""
 
     def execute(self, sql: str):
         pass
+
+    def execute_many(self, sql: str, values: list):
+        pass
```

### Comparing `hnhm-0.0.7/hnhm/core/tasks.py` & `hnhm-0.0.8/hnhm/core/task.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.7/hnhm/file_storage.py` & `hnhm-0.0.8/hnhm/file_state.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from pathlib import Path
 
-from hnhm.core import Storage, HnhmStorageData
+from .core import State, HnhmStateData
 
 
-class FileStorage(Storage):
+class FileState(State):
     def __init__(self, file_name: str):
         self.file_name = file_name
 
-    def load(self) -> HnhmStorageData:
+    def load(self) -> HnhmStateData:
         if Path(self.file_name).is_file():
-            return HnhmStorageData.parse_file(self.file_name)
+            return HnhmStateData.parse_file(self.file_name)
         else:
-            return HnhmStorageData(entities={}, entities_views=set(), links={})
+            return HnhmStateData(entities={}, entities_views=set(), links={})
 
-    def save(self, data: HnhmStorageData):
+    def save(self, data: HnhmStateData):
         with open(self.file_name, "w") as f:
             f.write(data.json(ensure_ascii=False, indent=2))
```

### Comparing `hnhm-0.0.7/hnhm/flow.py` & `hnhm-0.0.8/hnhm/flow.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,11 @@
-from hnhm.core import (
-    Task,
-    Entity,
-    LoadHub,
-    LoadLink,
-    Attribute,
-    HnhmError,
-    LoadGroup,
-    LoadAttribute,
-)
-
 from .hnhm_link import HnhmLink
 from .hnhm_attribute import HnhmAttribute
 from .hnhm_entity import HnhmEntity, LayoutType
+from .core import Entity, Attribute, HnhmError, task
 
 
 class Flow:
     def __init__(self, *, source: HnhmEntity, business_time_field: HnhmAttribute):
         source = source.to_core()
         if source.layout.type != LayoutType.STAGE:
             raise HnhmError(
@@ -38,34 +28,34 @@
         # {entity_name -> {group_name -> {attribute_target -> attribute_source}}}
         self._groups: dict[str, dict[str, dict[Attribute, Attribute]]] = {}
 
         # {link_name -> {entity_name -> {attribute_target -> attribute_source}}}
         self._links = {}
 
     @property
-    def tasks(self) -> list[Task]:
+    def tasks(self) -> list[task.Task]:
         tasks = []
         hub_tasks = {}
         for target_name, target in self._hubs.items():
             keys_mapping = self._entities_keys_mappings[target_name]
-            hub_tasks[target_name] = LoadHub(
+            hub_tasks[target_name] = task.LoadHub(
                 source=self.source,
                 target=target,
                 keys_mapping=keys_mapping,
                 business_time_field=self.business_time_field,
             )
 
         for target_name, attributes_mapping in self._attributes.items():
             target = self._hubs[target_name]
             depends_on = [hub_tasks[target_name].id]
             keys_mapping = self._entities_keys_mappings[target_name]
 
             for target_attribute, source_attribute in attributes_mapping.items():
                 tasks.append(
-                    LoadAttribute(
+                    task.LoadAttribute(
                         source=self.source,
                         target=target,
                         keys_mapping=keys_mapping,
                         source_attribute=source_attribute,
                         target_attribute=target_attribute,
                         business_time_field=self.business_time_field,
                         depends_on=depends_on,
@@ -75,15 +65,15 @@
         for target_name, groups_mapping in self._groups.items():
             target = self._hubs[target_name]
             depends_on = [hub_tasks[target_name].id]
             keys_mapping = self._entities_keys_mappings[target_name]
             for group_name, attributes_mapping in groups_mapping.items():
                 group = target.groups[group_name]
                 tasks.append(
-                    LoadGroup(
+                    task.LoadGroup(
                         source=self.source,
                         target=target,
                         group=group,
                         keys_mapping=keys_mapping,
                         attributes_mapping=attributes_mapping,
                         business_time_field=self.business_time_field,
                         depends_on=depends_on,
@@ -94,15 +84,15 @@
             keys_mapping = {}
             depends_on = []
             for link_element in link.elements:
                 entity_name = link_element.entity.name
                 depends_on.append(hub_tasks[entity_name].id)
                 keys_mapping[entity_name] = self._entities_keys_mappings[entity_name]
             tasks.append(
-                LoadLink(
+                task.LoadLink(
                     source=self.source,
                     link=link,
                     keys_mapping=keys_mapping,
                     business_time_field=self.business_time_field,
                     depends_on=depends_on,
                 )
             )
```

### Comparing `hnhm-0.0.7/hnhm/hnhm.py` & `hnhm-0.0.8/hnhm/hnhm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,316 +1,312 @@
 from enum import Enum
 
 import pydantic
 
-from hnhm.core import (
-    Sql,
-    Entity,
-    Storage,
-    HnhmError,
-    Migration,
-    CreateLink,
-    LayoutType,
-    RemoveLink,
-    CreateGroup,
-    RemoveGroup,
-    CreateEntity,
-    RemoveEntity,
-    CreateAttribute,
-    RemoveAttribute,
-    RemoveEntityView,
-    AddGroupAttribute,
-    RecreateEntityView,
-    RemoveGroupAttribute,
-)
-
 from .hnhm_link import HnhmLink
 from .hnhm_entity import HnhmEntity
+from .core import Sql, State, Entity, HnhmError, LayoutType, migration
 
 
 class PlanType(str, Enum):
     CREATE = "CREATE"
     REMOVE = "REMOVE"
     UPDATE = "UPDATE"
 
 
 class PlanCollection(pydantic.BaseModel):
     type: PlanType
-    migrations: list[Migration]
+    migrations: list[migration.Migration]
 
 
 class Plan(pydantic.BaseModel):
     entities_migrations: dict[str, PlanCollection]
     links_migrations: dict[str, PlanCollection]
 
     def is_empty(self):
         return not self.entities_migrations and not self.links_migrations
 
     @property
     def migrations_all(self):
-        migrations: list[Migration] = []
+        migrations: list[migration.Migration] = []
+
         for collection in self.entities_migrations.values():
             migrations.extend(collection.migrations)
+
         for collection in self.links_migrations.values():
             migrations.extend(collection.migrations)
+
         migrations = sorted(migrations, key=lambda m: m.priority)
         return migrations
 
 
 class HnHm:
-    def __init__(self, *, sql: Sql, storage: Storage):
+    def __init__(self, *, sql: Sql, state: State):
         self.sql = sql
-        self.storage = storage
-        self.data = self.storage.load()
+        self.state = state
+        self.data = self.state.load()
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
-        self.storage.save(self.data)
+        self.state.save(self.data)
 
     def plan(
         self,
         *,
         entities: list[HnhmEntity] | None = None,
         links: list[HnhmLink] | None = None,
     ) -> Plan:
         core_entities = {}
         for entity in entities or []:
             entity_core = entity.to_core()
-            core_entities[entity_core.name] = entity_core
+            core_entities[entity_core.fqn] = entity_core
 
         core_links = {}
         for link in links or []:
             link_core = link.to_core()
-            core_links[link_core.name] = link_core
+            core_links[link_core.fqn] = link_core
 
         plan = Plan(entities_migrations={}, links_migrations={})
 
         # Entity: create if not exists
         for entity in core_entities.values():
             migrations = []
 
             # Entity's View: create/update if not exists
             if (
-                entity.name not in self.data.entities_views
+                entity.fqn not in self.data.entities_views
                 and entity.layout.type == LayoutType.HNHM
             ):
-                migrations.append(RecreateEntityView(entity=entity))
+                migrations.append(migration.RecreateEntityView(entity=entity))
 
             # Create Entity
-            if entity.name not in self.data.entities:
-                migrations.append(CreateEntity(entity=entity))
+            if entity.fqn not in self.data.entities:
+                migrations.append(migration.CreateEntity(entity=entity))
 
                 if entity.layout.type == LayoutType.HNHM:
                     # Create Attribute
                     for attribute in entity.attributes.values():
                         migrations.append(
-                            CreateAttribute(entity=entity, attribute=attribute)
+                            migration.CreateAttribute(entity=entity, attribute=attribute)
                         )
                     # Create Group
                     for group in entity.groups.values():
-                        migrations.append(CreateGroup(entity=entity, group=group))
+                        migrations.append(
+                            migration.CreateGroup(entity=entity, group=group)
+                        )
 
             if migrations:
-                plan.entities_migrations[entity.name] = PlanCollection(
+                plan.entities_migrations[entity.fqn] = PlanCollection(
                     type=PlanType.CREATE,
                     migrations=migrations,
                 )
 
         # Entity: create/remove/update Attribute/Group
         for entity in core_entities.values():
-            if entity.name not in self.data.entities:
+            if entity.fqn not in self.data.entities:
                 continue
 
-            attributes_state = self.data.entities[entity.name].attributes
-            groups_state = self.data.entities[entity.name].groups
+            attributes_state = self.data.entities[entity.fqn].attributes
+            groups_state = self.data.entities[entity.fqn].groups
 
             migrations = []
             # Create Attribute
             for attribute_name, attribute in entity.attributes.items():
                 if attribute_name not in attributes_state:
-                    migrations.append(CreateAttribute(entity=entity, attribute=attribute))
+                    migrations.append(
+                        migration.CreateAttribute(entity=entity, attribute=attribute)
+                    )
 
             # Remove Attribute
             for attribute_name, attribute in attributes_state.items():
                 if attribute_name not in entity.attributes:
-                    migrations.append(RemoveAttribute(entity=entity, attribute=attribute))
+                    migrations.append(
+                        migration.RemoveAttribute(entity=entity, attribute=attribute)
+                    )
 
             # Create/Update Group
             for group_name, group in entity.groups.items():
                 # Update
                 if group_name in groups_state:
                     group_state = groups_state[group_name]
                     # Add an Attribute to a Group
                     for attribute_name, attribute in group.attributes.items():
                         if attribute_name not in group_state.attributes:
                             migrations.append(
-                                AddGroupAttribute(
+                                migration.AddGroupAttribute(
                                     entity=entity, group=group, attribute=attribute
                                 )
                             )
                     # Remove an Attribute from a Group
                     for attribute_name, attribute in group_state.attributes.items():
                         if attribute_name not in group.attributes:
                             migrations.append(
-                                RemoveGroupAttribute(
+                                migration.RemoveGroupAttribute(
                                     entity=entity, group=group, attribute=attribute
                                 )
                             )
                 # Create
                 else:
-                    migrations.append(CreateGroup(entity=entity, group=group))
+                    migrations.append(migration.CreateGroup(entity=entity, group=group))
 
             # Remove Group
             for group_name, group in groups_state.items():
                 if group_name not in entity.groups:
-                    migrations.append(RemoveGroup(entity=entity, group=group))
+                    migrations.append(migration.RemoveGroup(entity=entity, group=group))
 
             if migrations:
                 if entity.layout.type == LayoutType.HNHM:
                     migrations.extend(
                         [
-                            RemoveEntityView(entity=entity),
-                            RecreateEntityView(entity=entity),
+                            migration.RemoveEntityView(entity=entity),
+                            migration.RecreateEntityView(entity=entity),
                         ]
                     )
-                plan.entities_migrations[entity.name] = PlanCollection(
+                plan.entities_migrations[entity.fqn] = PlanCollection(
                     type=PlanType.UPDATE,
                     migrations=migrations,
                 )
 
         # Link: remove
         for link_name, link in self.data.links.items():
             if link_name not in core_links:
                 plan.links_migrations[link_name] = PlanCollection(
                     type=PlanType.REMOVE,
-                    migrations=[RemoveLink(link=link)],
+                    migrations=[migration.RemoveLink(link=link)],
                 )
 
         # Entity: remove
         for entity_name, entity in self.data.entities.items():
             if entity_name not in core_entities:
                 migrations = []
 
                 if entity.layout.type == LayoutType.HNHM:
-                    migrations.append(RemoveEntityView(entity=entity))
+                    migrations.append(migration.RemoveEntityView(entity=entity))
 
                     attributes_state = self.data.entities[entity_name].attributes
                     groups_state = self.data.entities[entity_name].groups
                     # Remove Attribute
                     for _, attribute_state in attributes_state.items():
                         migrations.append(
-                            RemoveAttribute(entity=entity, attribute=attribute_state)
+                            migration.RemoveAttribute(
+                                entity=entity, attribute=attribute_state
+                            )
                         )
                     # Remove Group
                     for group_name, group in groups_state.items():
-                        migrations.append(RemoveGroup(entity=entity, group=group))
+                        migrations.append(
+                            migration.RemoveGroup(entity=entity, group=group)
+                        )
 
-                migrations.append(RemoveEntity(entity=entity))
+                migrations.append(migration.RemoveEntity(entity=entity))
                 plan.entities_migrations[entity_name] = PlanCollection(
                     type=PlanType.REMOVE,
                     migrations=migrations,
                 )
 
         # Link: create
         for link_name, link in core_links.items():
             if link_name not in self.data.links:
-                plan.links_migrations[link.name] = PlanCollection(
+                plan.links_migrations[link.fqn] = PlanCollection(
                     type=PlanType.CREATE,
-                    migrations=[CreateLink(link=link)],
+                    migrations=[migration.CreateLink(link=link)],
                 )
 
         return plan
 
     def apply(self, plan: Plan):
-        for migration in plan.migrations_all:
-            sql = self.sql.generate_sql(migration)
+        for plan_migration in plan.migrations_all:
+            sql = self.sql.generate_sql(plan_migration)
 
-            match migration:
-                case CreateEntity(entity=entity):
-                    self.data.check_entity_not_exists(entity.name)
+            match plan_migration:
+                case migration.CreateEntity(entity=entity):
+                    self.data.check_entity_not_exists(entity.fqn)
                     self.sql.execute(sql)
                     if entity.layout.type == LayoutType.HNHM:
                         attributes = {}
                         groups = {}
                     else:
                         attributes = entity.attributes
                         groups = entity.groups
-                    self.data.entities[entity.name] = Entity(
+                    self.data.entities[entity.fqn] = Entity(
+                        fqn=entity.fqn,
                         name=entity.name,
                         layout=entity.layout,
                         doc=entity.doc,
                         keys=entity.keys,
                         attributes=attributes,
                         groups=groups,
                     )
 
-                case RemoveEntity(entity=entity):
-                    self.data.check_entity_exists(entity.name)
+                case migration.RemoveEntity(entity=entity):
+                    self.data.check_entity_exists(entity.fqn)
                     self.sql.execute(sql)
-                    del self.data.entities[entity.name]
+                    del self.data.entities[entity.fqn]
 
-                case RecreateEntityView(entity=entity):
+                case migration.RecreateEntityView(entity=entity):
                     self.sql.execute(sql)
-                    self.data.entities_views.add(entity.name)
+                    self.data.entities_views.add(entity.fqn)
 
-                case RemoveEntityView(entity=entity):
-                    if entity.name not in self.data.entities_views:
-                        raise HnhmError(f"Entity's View '{entity.name}' doesn't exist.")
+                case migration.RemoveEntityView(entity=entity):
+                    if entity.fqn not in self.data.entities_views:
+                        raise HnhmError(f"Entity's View '{entity.fqn}' doesn't exist.")
                     self.sql.execute(sql)
-                    self.data.entities_views.remove(entity.name)
+                    self.data.entities_views.remove(entity.fqn)
 
-                case CreateAttribute(entity=entity, attribute=attribute):
-                    self.data.check_attribute_not_exists(entity.name, attribute.name)
+                case migration.CreateAttribute(entity=entity, attribute=attribute):
+                    self.data.check_attribute_not_exists(entity.fqn, attribute.name)
                     self.sql.execute(sql)
-                    self.data.entities[entity.name].attributes[attribute.name] = attribute
+                    self.data.entities[entity.fqn].attributes[attribute.name] = attribute
 
-                case RemoveAttribute(entity=entity, attribute=attribute):
-                    self.data.check_attribute_exists(entity.name, attribute.name)
+                case migration.RemoveAttribute(entity=entity, attribute=attribute):
+                    self.data.check_attribute_exists(entity.fqn, attribute.name)
                     self.sql.execute(sql)
-                    del self.data.entities[entity.name].attributes[attribute.name]
+                    del self.data.entities[entity.fqn].attributes[attribute.name]
 
-                case CreateGroup(entity=entity, group=group):
-                    self.data.check_group_not_exists(entity.name, group.name)
+                case migration.CreateGroup(entity=entity, group=group):
+                    self.data.check_group_not_exists(entity.fqn, group.name)
                     self.sql.execute(sql)
-                    self.data.entities[entity.name].groups[group.name] = group
+                    self.data.entities[entity.fqn].groups[group.name] = group
 
-                case RemoveGroup(entity=entity, group=group):
-                    self.data.check_group_exists(entity.name, group.name)
+                case migration.RemoveGroup(entity=entity, group=group):
+                    self.data.check_group_exists(entity.fqn, group.name)
                     self.sql.execute(sql)
-                    del self.data.entities[entity.name].groups[group.name]
+                    del self.data.entities[entity.fqn].groups[group.name]
 
-                case AddGroupAttribute(entity=entity, group=group, attribute=attribute):
+                case migration.AddGroupAttribute(
+                    entity=entity, group=group, attribute=attribute
+                ):
                     self.data.check_group_attribute_not_exists(
-                        entity.name, group.name, attribute.name
+                        entity.fqn, group.name, attribute.name
                     )
                     self.sql.execute(sql)
-                    self.data.entities[entity.name].groups[group.name].attributes[
+                    self.data.entities[entity.fqn].groups[group.name].attributes[
                         attribute.name
                     ] = attribute
 
-                case RemoveGroupAttribute(
+                case migration.RemoveGroupAttribute(
                     entity=entity, group=group, attribute=attribute
                 ):
                     self.data.check_group_attribute_exists(
-                        entity.name, group.name, attribute.name
+                        entity.fqn, group.name, attribute.name
                     )
                     self.sql.execute(sql)
                     del (
-                        self.data.entities[entity.name]
+                        self.data.entities[entity.fqn]
                         .groups[group.name]
                         .attributes[attribute.name]
                     )
 
-                case CreateLink(link=link):
-                    self.data.check_link_not_exists(link.name)
+                case migration.CreateLink(link=link):
+                    self.data.check_link_not_exists(link.fqn)
                     self.sql.execute(sql)
-                    self.data.links[link.name] = link
+                    self.data.links[link.fqn] = link
 
-                case RemoveLink(link=link):
-                    self.data.check_link_exists(link.name)
+                case migration.RemoveLink(link=link):
+                    self.data.check_link_exists(link.fqn)
                     self.sql.execute(sql)
-                    del self.data.links[link.name]
+                    del self.data.links[link.fqn]
 
                 case _:
                     raise HnhmError(f"Unknown migration: '{migration}'")
```

### Comparing `hnhm-0.0.7/hnhm/hnhm_attribute.py` & `hnhm-0.0.8/hnhm/hnhm_attribute.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import abc
 
-from hnhm.core import Type, Attribute, ChangeType
+from .core.attribute import Type
+from .core import Attribute, ChangeType
 
 
 class HnhmAttribute(abc.ABC):
     type: Type
 
     def __init__(
         self,
@@ -36,9 +37,13 @@
     type = Type.STRING
 
 
 class Integer(HnhmAttribute):
     type = Type.INTEGER
 
 
+class Float(HnhmAttribute):
+    type = Type.FLOAT
+
+
 class Timestamp(HnhmAttribute):
     type = Type.TIMESTAMP
```

### Comparing `hnhm-0.0.7/hnhm/hnhm_entity.py` & `hnhm-0.0.8/hnhm/hnhm_entity.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import abc
 import inspect
 
-from hnhm.core import Group, Entity, Layout, HnhmError, ChangeType, LayoutType
-
 from .hnhm_attribute import HnhmAttribute
+from .core import Group, Entity, Layout, HnhmError, ChangeType, LayoutType
 
 
 class HnhmEntity(abc.ABC):
     __layout__: Layout = None
     __keys__: list[HnhmAttribute] | None = None
 
     def to_core(self) -> Entity:
@@ -23,38 +22,40 @@
             raise HnhmError(
                 f"Type for Layout '{layout}' is required for entity."
                 " Please, specify LayoutType via 'type' attribute."
             )
 
         name = layout.name
 
+        fqn = f"{layout.type}.{name}"
+
         if not inspected.get("__doc__"):
             raise HnhmError(
-                f"Doc not found or empty for entity: '{layout.type}.{name}'."
+                f"Doc not found or empty for entity: '{fqn}'."
                 " Please, write a documentation for your entity."
             )
         doc: str = inspected["__doc__"]
 
         match layout.type:
             case LayoutType.STAGE:
                 keys = []
 
             case LayoutType.HNHM:
                 if not inspected.get("__keys__"):
                     raise HnhmError(
-                        f"At least one Key is required for entity '{layout.type}.{name}'."
+                        f"At least one Key is required for entity '{fqn}'."
                         " Please, specify entity's keys via the '__keys__' attribute."
                     )
 
                 keys_hnhm: list[HnhmAttribute] = inspected["__keys__"]
                 for key in keys_hnhm:
                     if key.change_type != ChangeType.IGNORE:
                         raise HnhmError(
                             f"Change type='{key.change_type}' is not supported for Key attributes."
-                            f" Use 'ChangeType.IGNORE' for the key attributes in the '{layout.type}.{name}' entity."
+                            f" Use 'ChangeType.IGNORE' for the key attributes in the '{fqn}' entity."
                         )
 
                 keys = [key.to_core(name) for key in keys_hnhm]
                 if len(keys) != len(set(keys)):
                     raise HnhmError(
                         f"Found duplicated keys for entity: '{layout.type}.{name}'."
                     )
@@ -79,28 +80,27 @@
                         entity_name=name,
                         attributes={attribute_name: attribute},
                         change_type=attribute.change_type,
                     )
 
                 if groups[group_name].change_type != attribute.change_type:
                     raise HnhmError(
-                        f"Found conflicting ChangeType for the entity='{layout.type}.{name}' group='{group_name}'."
+                        f"Found conflicting ChangeType for the entity='{fqn}' group='{group_name}'."
                         " Please, use single ChangeType for all attributes within the same group."
                     )
                 groups[group_name].attributes[attribute_name] = attribute
 
             elif attribute not in keys:
                 attributes[attribute_name] = attribute
 
         if layout.type == LayoutType.STAGE and len(attributes) < 1:
-            raise HnhmError(
-                f"Entity='{layout.type}.{name}' should have at least 1 attribute."
-            )
+            raise HnhmError(f"Entity='{fqn}' should have at least 1 attribute.")
 
         return Entity(
+            fqn=fqn,
             name=name,
             layout=layout,
             doc=doc,
             keys=keys,
             attributes=attributes,
             groups=groups,
         )
```

### Comparing `hnhm-0.0.7/hnhm/hnhm_link.py` & `hnhm-0.0.8/hnhm/hnhm_link.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import abc
 import inspect
 
-from hnhm.core import Link, Layout, HnhmError, LayoutType, LinkElement
-
 from .hnhm_entity import HnhmEntity
+from .core import Link, Layout, HnhmError, LayoutType, LinkElement
 
 
 class HnhmLinkElement:
     def __init__(self, *, entity: HnhmEntity, comment: str):
         self.entity = entity
         self.comment = comment
 
@@ -40,42 +39,45 @@
                 f"Layout not found for link: '{self}'."
                 " Please, specify Layout via '__layout__' attribute."
             )
         layout: Layout = inspected["__layout__"]
 
         name = layout.name
 
+        fqn = name
+
         if not inspected.get("__doc__"):
             raise HnhmError(
-                f"Doc not found or empty for link: '{name}'."
+                f"Doc not found or empty for link: '{fqn}'."
                 " Please, write a documentation for your link."
             )
         doc: str = inspected["__doc__"]
 
         if not inspected.get("__keys__"):
             raise HnhmError(
-                f"At least one Key is required for link='{name}'."
+                f"At least one Key is required for '{fqn}'."
                 " Please, specify link's keys via the '__keys__' attribute."
             )
         keys_hnhm: list[HnhmEntity] = inspected["__keys__"]
         keys = [key.to_core() for key in keys_hnhm]
 
         elements = []
         for class_attribute in inspected.values():
             if not isinstance(class_attribute, HnhmLinkElement):
                 continue
             link_element = class_attribute.to_core()
             elements.append(link_element)
 
         if len(elements) < 2:
             raise HnhmError(
-                f"At least two LinkElements are required for link='{name}'."
+                f"At least two LinkElements are required for '{fqn}'."
                 " Please, specify more than one elements."
             )
 
         return Link(
+            fqn=fqn,
             name=name,
             layout=layout,
             doc=doc,
             elements=elements,
             keys=keys,
         )
```

### Comparing `hnhm-0.0.7/hnhm/hnhm_registry.py` & `hnhm-0.0.8/hnhm/hnhm_registry.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,17 @@
     def __init__(
         self,
         *,
         hnhm: HnHm,
         entities: list[HnhmEntity] | None = None,
         links: list[HnhmLink] | None = None,
     ):
+        entities = entities or []
+        links = links or []
+
         entities_names = set()
         for entity in entities:
             entity_core = entity.to_core()
             full_entity_name = f"{entity_core.layout.type}.{entity_core.name}"
             if full_entity_name in entities_names:
                 raise HnhmError(
                     f"Found duplicated entity: '{full_entity_name}'."
```

### Comparing `hnhm-0.0.7/hnhm/plan_printer.py` & `hnhm-0.0.8/hnhm/plan_printer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,21 @@
 from enum import Enum
 
 import click
 import pydantic
 
 from .hnhm import Plan, PlanType
-from .core import (
-    HnhmError,
-    CreateLink,
-    LayoutType,
-    RemoveLink,
-    CreateGroup,
-    RemoveGroup,
-    CreateEntity,
-    RemoveEntity,
-    CreateAttribute,
-    RemoveAttribute,
-    RemoveEntityView,
-    AddGroupAttribute,
-    RecreateEntityView,
-    RemoveGroupAttribute,
-)
+from .core import HnhmError, LayoutType, migration
 
 
 class Color(str, Enum):
     green = "green"
     red = "red"
     yellow = "yellow"
+    cyan = "cyan"
 
 
 class PlanLine(pydantic.BaseModel):
     text: str
     color: str | None = None
 
 
@@ -39,29 +25,29 @@
         lines.append(PlanLine(text="Your DWH is up to date.", color=Color.green))
         return lines
 
     entities_migrations = sorted(plan.entities_migrations.items(), key=lambda kv: kv[0])
     links_migrations = sorted(plan.links_migrations.items(), key=lambda kv: kv[0])
 
     lines.append(PlanLine(text="Plan:"))
-    for entity_name, plan_collection in entities_migrations:
+    for entity_fqn, plan_collection in entities_migrations:
         if plan_collection.type == PlanType.CREATE:
             symbol, color = "+", Color.green
         elif plan_collection.type == PlanType.REMOVE:
             symbol, color = "-", Color.red
         elif plan_collection.type == PlanType.UPDATE:
             symbol, color = "[u]", Color.yellow
         else:
             raise HnhmError()
 
         lines.append(PlanLine(text=""))
-        lines.append(PlanLine(text=f"{symbol} entity '{entity_name}'", color=color))
+        lines.append(PlanLine(text=f"{symbol} entity '{entity_fqn}'", color=color))
         for entity_migration in plan_collection.migrations:
             match entity_migration:
-                case CreateEntity(entity=entity):
+                case migration.CreateEntity(entity=entity):
                     if entity.layout.type == LayoutType.HNHM:
                         lines.append(
                             PlanLine(text=f"  + hub '{entity.name}'", color=Color.green)
                         )
                     else:
                         lines.append(
                             PlanLine(text=f"  + stage '{entity.name}'", color=Color.green)
@@ -70,49 +56,51 @@
                             lines.append(
                                 PlanLine(
                                     text=f"    |attribute '{attribute.name}'",
                                     color=Color.green,
                                 )
                             )
 
-                case RecreateEntityView(entity=entity):
+                case migration.RecreateEntityView(entity=entity):
                     lines.append(
                         PlanLine(text=f"  {symbol} view '{entity.name}'", color=color)
                     )
 
-                case CreateAttribute(entity=_, attribute=attribute):
+                case migration.CreateAttribute(entity=_, attribute=attribute):
                     lines.append(
                         PlanLine(
                             text=f"  + attribute '{attribute.name}'", color=Color.green
                         )
                     )
 
-                case CreateGroup(entity=_, group=group):
+                case migration.CreateGroup(entity=_, group=group):
                     lines.append(
                         PlanLine(text=f"  + group '{group.name}'", color=Color.green)
                     )
                     for attribute in group.attributes.values():
                         lines.append(
                             PlanLine(
                                 text=f"    |attribute '{attribute.name}'",
                                 color=Color.green,
                             )
                         )
 
-                case AddGroupAttribute(entity=_, group=group, attribute=attribute):
+                case migration.AddGroupAttribute(
+                    entity=_, group=group, attribute=attribute
+                ):
                     lines.append(
                         PlanLine(text=f"  [u] group '{group.name}'", color=Color.yellow)
                     )
                     lines.append(
                         PlanLine(
                             text=f"    +attribute '{attribute.name}'", color=Color.green
                         )
                     )
 
-                case RemoveEntity(entity=entity):
+                case migration.RemoveEntity(entity=entity):
                     if entity.layout.type == LayoutType.HNHM:
                         lines.append(
                             PlanLine(text=f"  - hub '{entity.name}'", color=Color.red)
                         )
                     else:
                         lines.append(
                             PlanLine(text=f"  - stage '{entity.name}'", color=Color.red)
@@ -121,69 +109,71 @@
                             lines.append(
                                 PlanLine(
                                     text=f"    |attribute '{attribute.name}'",
                                     color=Color.red,
                                 )
                             )
 
-                case RemoveEntityView(entity=entity):
+                case migration.RemoveEntityView(entity=entity):
                     if plan_collection.type == PlanType.REMOVE:
                         lines.append(
                             PlanLine(text=f"  - view '{entity.name}'", color=Color.red)
                         )
 
-                case RemoveAttribute(entity=_, attribute=attribute):
+                case migration.RemoveAttribute(entity=_, attribute=attribute):
                     lines.append(
                         PlanLine(
                             text=f"  - attribute '{attribute.name}'", color=Color.red
                         )
                     )
 
-                case RemoveGroup(entity=_, group=group):
+                case migration.RemoveGroup(entity=_, group=group):
                     lines.append(
                         PlanLine(text=f"  - group '{group.name}'", color=Color.red)
                     )
                     for attribute in group.attributes.values():
                         lines.append(
                             PlanLine(
                                 text=f"    | attribute '{attribute.name}'",
                                 color=Color.red,
                             )
                         )
 
-                case RemoveGroupAttribute(entity=_, group=group, attribute=attribute):
+                case migration.RemoveGroupAttribute(
+                    entity=_, group=group, attribute=attribute
+                ):
                     lines.append(
                         PlanLine(text=f"  [u] group '{group.name}'", color=Color.yellow)
                     )
                     lines.append(
                         PlanLine(
                             text=f"    -attribute '{attribute.name}'", color=Color.red
                         )
                     )
 
-    for link_name, plan_collection in links_migrations:
+    for link_fqn, plan_collection in links_migrations:
         if plan_collection.type == PlanType.CREATE:
             symbol, color = "+", Color.green
         elif plan_collection.type == PlanType.REMOVE:
             symbol, color = "-", Color.red
         else:
             raise HnhmError()
 
         lines.append(PlanLine(text=""))
-        lines.append(PlanLine(text=f"{symbol} link '{link_name}'", color=color))
+        lines.append(PlanLine(text=f"{symbol} link '{link_fqn}'", color=color))
         for link_migration in plan_collection.migrations:
             match link_migration:
-                case RemoveLink(link=link):
+                case migration.RemoveLink(link=link):
                     for element in link.elements:
                         lines.append(
                             PlanLine(
                                 text=f"  |element '{element.entity.name}'", color=color
                             )
                         )
-                case CreateLink(link=link):
+                case migration.CreateLink(link=link):
                     for element in link.elements:
                         lines.append(
                             PlanLine(
                                 text=f"  |element '{element.entity.name}'", color=color
                             )
                         )
```

### Comparing `hnhm-0.0.7/hnhm/postgres/sql.py` & `hnhm-0.0.8/hnhm/postgres/sql.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,49 +1,28 @@
-from textwrap import dedent
-
 import jinja2
-from sqlalchemy import create_engine
-from sqlalchemy.engine import URL, Engine
+import psycopg2
 
-from hnhm.core import (
-    Sql,
-    Task,
-    Type,
-    LoadHub,
-    LoadLink,
-    HnhmError,
-    LoadGroup,
-    Migration,
-    ChangeType,
-    CreateLink,
-    LayoutType,
-    RemoveLink,
-    CreateGroup,
-    RemoveGroup,
-    CreateEntity,
-    RemoveEntity,
-    LoadAttribute,
-    CreateAttribute,
-    RemoveAttribute,
-    RemoveEntityView,
-    AddGroupAttribute,
-    RecreateEntityView,
-    RemoveGroupAttribute,
-)
+from ..core.attribute import Type
+from ..core import Sql, HnhmError, ChangeType, LayoutType, task, migration
 
 PG_TYPES = {
     Type.STRING: "TEXT",
     Type.INTEGER: "INTEGER",
+    Type.FLOAT: "DOUBLE PRECISION",
     Type.TIMESTAMP: "TIMESTAMPTZ",
 }
 
 
-def generate_sql(migration_or_task: Migration | Task, jinja: jinja2.Environment) -> str:
+def generate_sql(
+    migration_or_task: migration.Migration | task.Task, jinja: jinja2.Environment
+) -> str:
+    """Generates SQL for a given migration or task."""
+
     match migration_or_task:
-        case CreateEntity(entity=entity):
+        case migration.CreateEntity(entity=entity):
             if entity.layout.type == LayoutType.HNHM:
                 template = jinja.get_template("create_hub.sql")
                 columns = []
                 columns_types = []
                 for key in entity.keys:
                     columns.append(key.name)
                     column_type = PG_TYPES[key.type]
@@ -62,15 +41,15 @@
 
             return template.render(
                 name=entity.name,
                 columns=columns,
                 columns_types=columns_types,
             )
 
-        case RecreateEntityView(entity=entity):
+        case migration.RecreateEntityView(entity=entity):
             template = jinja.get_template("update_entity_view.sql")
 
             view_name = f"entity__{entity.name}"
             sk = entity.sk
             hub = f"hub__{entity.name}"
 
             selects = []
@@ -88,15 +67,15 @@
                 sk=sk,
                 hub=hub,
                 selects=selects,
                 attributes=entity.attributes.values(),
                 groups=entity.groups.values(),
             )
 
-        case CreateAttribute(entity=entity, attribute=attribute):
+        case migration.CreateAttribute(entity=entity, attribute=attribute):
             attribute_type = PG_TYPES[attribute.type]
 
             if entity.layout.type == LayoutType.STAGE:
                 return f"ALTER TABLE stg__{entity.name} ADD COLUMN {attribute.name} {attribute_type}"
 
             time_columns = ["valid_from TIMESTAMPTZ NOT NULL"]
             if attribute.change_type == ChangeType.NEW:
@@ -106,15 +85,15 @@
             return template.render(
                 entity_name=entity.name,
                 attribute_name=attribute.name,
                 attribute_type=attribute_type,
                 time_columns=time_columns,
             )
 
-        case CreateGroup(entity=entity, group=group):
+        case migration.CreateGroup(entity=entity, group=group):
             columns = []
             for attribute in group.attributes.values():
                 column_type = PG_TYPES[attribute.type]
                 columns.append(f"{attribute.name} {column_type}")
 
             time_columns = ["valid_from TIMESTAMPTZ NOT NULL"]
             if group.change_type == ChangeType.NEW:
@@ -124,19 +103,19 @@
             return template.render(
                 entity_name=entity.name,
                 group_name=group.name,
                 columns=columns,
                 time_columns=time_columns,
             )
 
-        case AddGroupAttribute(entity=entity, group=group, attribute=attribute):
+        case migration.AddGroupAttribute(entity=entity, group=group, attribute=attribute):
             attribute_type = PG_TYPES[attribute.type]
             return f"ALTER TABLE group__{entity.name}__{group.name} ADD COLUMN {attribute.name} {attribute_type}"
 
-        case CreateLink(link=link):
+        case migration.CreateLink(link=link):
             entities = []
             for link_element in link.elements:
                 entities.append(link_element.entity.name)
 
             primary_keys = ["valid_from"]
             for key in link.keys:
                 primary_keys.append(f"{key.entity.name}_sk")
@@ -144,41 +123,43 @@
             template = jinja.get_template("create_link.sql")
             return template.render(
                 name=link.name,
                 entities=entities,
                 primary_keys=primary_keys,
             )
 
-        case RemoveEntity(entity=entity):
+        case migration.RemoveEntity(entity=entity):
             if entity.layout.type == LayoutType.HNHM:
                 table_name = f"hub__{entity.name}"
             else:
                 table_name = f"stg__{entity.name}"
             return f"DROP TABLE {table_name}"
 
-        case RemoveAttribute(entity=entity, attribute=attribute):
+        case migration.RemoveAttribute(entity=entity, attribute=attribute):
             if entity.layout.type == LayoutType.STAGE:
                 return f"ALTER TABLE stg__{entity.name} DROP COLUMN {attribute.name}"
 
             return f"DROP TABLE attr__{entity.name}__{attribute.name}"
 
-        case RemoveGroup(entity=entity, group=group):
+        case migration.RemoveGroup(entity=entity, group=group):
             return f"DROP TABLE group__{entity.name}__{group.name}"
 
-        case RemoveGroupAttribute(entity=entity, group=group, attribute=attribute):
+        case migration.RemoveGroupAttribute(
+            entity=entity, group=group, attribute=attribute
+        ):
             return f"ALTER TABLE group__{entity.name}__{group.name} DROP COLUMN {attribute.name}"
 
-        case RemoveLink(link=link):
+        case migration.RemoveLink(link=link):
             return f"DROP TABLE link__{link.name}"
 
-        case RemoveEntityView(entity=entity):
+        case migration.RemoveEntityView(entity=entity):
             view_name = f"entity__{entity.name}"
             return f"DROP VIEW {view_name}"
 
-        case LoadHub(
+        case task.LoadHub(
             source=source,
             target=target,
             business_time_field=business_time_field,
             keys_mapping=keys_mapping,
         ):
             source_keys = [key_source.name for key_source in keys_mapping.values()]
             source_sk_components = (f"{key}::TEXT" for key in source_keys)
@@ -193,15 +174,15 @@
                 source_sk=source_sk,
                 source_keys=source_keys,
                 target_name=target.name,
                 target_keys=target_keys,
                 business_time_field=business_time_field.name,
             )
 
-        case LoadAttribute(
+        case task.LoadAttribute(
             source=source,
             target=target,
             business_time_field=business_time_field,
             keys_mapping=keys_mapping,
             source_attribute=source_attribute,
             target_attribute=target_attribute,
         ):
@@ -238,15 +219,15 @@
                 target_sk=target_sk,
                 target_sks=target_sks,
                 target_attributes=target_attributes,
                 business_time_field=business_time_field.name,
                 extra_sks=[],
             )
 
-        case LoadGroup(
+        case task.LoadGroup(
             source=source,
             target=target,
             group=group,
             business_time_field=business_time_field,
             keys_mapping=keys_mapping,
             attributes_mapping=attributes_mapping,
         ):
@@ -287,15 +268,15 @@
                 target_sk=target_sk,
                 target_sks=target_sks,
                 target_attributes=target_attributes,
                 business_time_field=business_time_field.name,
                 extra_sks=[],
             )
 
-        case LoadLink(
+        case task.LoadLink(
             source=source,
             link=link,
             business_time_field=business_time_field,
             keys_mapping=keys_mapping,
         ):
             source_table = f"stg__{source.name}"
 
@@ -329,62 +310,65 @@
         case _:
             migration_or_task_type = type(migration_or_task)
             raise HnhmError(
                 f"Unknown migration or task: '{migration_or_task}' with type='{migration_or_task_type}'."
             )
 
 
-class PostgresSqlalchemySql(Sql):
+class PostgresPsycopgSql(Sql):
     def __init__(
         self,
         *,
         host: str = "localhost",
         port: int = 5432,
         database: str = "postgres",
         user: str = "postgres",
         password: str | None = None,
-        engine: Engine | None = None,
     ):
-        if engine:
-            self.engine = engine
-        else:
-            connection_url = URL.create(
-                "postgresql+psycopg2",
-                username=user,
-                password=password,
-                host=host,
-                database=database,
-                port=port,
-            )
-            self.engine = create_engine(connection_url)
-
+        self.host = host
+        self.port = port
+        self.database = database
+        self.user = user
+        self.password = password
         self.jinja = jinja2.Environment(
             loader=jinja2.PackageLoader("hnhm.postgres", "sql_templates")
         )
         self.jinja.globals.update(zip=zip)
 
-    @classmethod
-    def with_engine(cls, engine: Engine):
-        if engine.url.drivername != "postgresql+psycopg2":
-            raise HnhmError(
-                f"Wrong driver name '{engine.url.drivername}'. Required: 'postgresql+psycopg2'."
-            )
-        return cls(engine=engine)
-
-    def generate_sql(self, migration_or_task: Migration | Task) -> str:
+    def generate_sql(self, migration_or_task: migration.Migration | task.Task) -> str:
         return generate_sql(migration_or_task, self.jinja)
 
-    def execute(self, sql: str, debug: bool = False):
-        if debug:
-            print(dedent(sql).strip())
+    def execute(self, sql: str):
+        connection = psycopg2.connect(
+            database=self.database,
+            user=self.user,
+            password=self.password,
+            port=self.port,
+            host=self.host,
+        )
+        cursor = connection.cursor()
 
-        conn = None
         try:
-            conn = self.engine.connect()
-            conn = conn.execution_options(isolation_level="AUTOCOMMIT")
-            conn.execute(sql)
+            cursor.execute(sql)
+            connection.commit()
         except Exception as e:
             raise e
         finally:
-            if conn:
-                conn.close()
-            self.engine.dispose()
+            cursor.close()
+            connection.close()
+
+    def execute_many(self, sql: str, values: list):
+        connection = psycopg2.connect(
+            database=self.database,
+            user=self.user,
+            password=self.password,
+            port=self.port,
+            host=self.host,
+        )
+        cursor = connection.cursor()
+
+        try:
+            cursor.executemany(sql, values)
+            connection.commit()
+        finally:
+            cursor.close()
+            connection.close()
```

### Comparing `hnhm-0.0.7/hnhm/postgres/sql_templates/create_group.sql` & `hnhm-0.0.8/hnhm/postgres/sql_templates/create_group.sql`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.7/hnhm/postgres/sql_templates/create_link.sql` & `hnhm-0.0.8/hnhm/postgres/sql_templates/create_link.sql`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.7/hnhm/postgres/sql_templates/load_ignore.sql` & `hnhm-0.0.8/hnhm/postgres/sql_templates/load_ignore.sql`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.7/hnhm/postgres/sql_templates/load_new.sql` & `hnhm-0.0.8/hnhm/postgres/sql_templates/load_new.sql`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.7/hnhm/postgres/sql_templates/load_update.sql` & `hnhm-0.0.8/hnhm/postgres/sql_templates/load_update.sql`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.7/hnhm/postgres/sql_templates/update_entity_view.sql` & `hnhm-0.0.8/hnhm/postgres/sql_templates/update_entity_view.sql`

 * *Files identical despite different names*

