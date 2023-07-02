# Comparing `tmp/qtgql-0.122.0.tar.gz` & `tmp/qtgql-0.123.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtgql-0.122.0.tar", max compression
+gzip compressed data, was "qtgql-0.123.0.tar", max compression
```

## Comparing `qtgql-0.122.0.tar` & `qtgql-0.123.0.tar`

### file list

```diff
@@ -1,32 +1,35 @@
--rw-r--r--   0        0        0     1064 2023-06-27 12:33:59.107303 qtgql-0.122.0/LICENSE
--rw-r--r--   0        0        0     1805 2023-06-27 12:33:59.107303 qtgql-0.122.0/README.md
--rw-r--r--   0        0        0     4428 2023-06-27 12:34:16.175650 qtgql-0.122.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/__init__.py
--rw-r--r--   0        0        0     1866 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/cli.py
--rw-r--r--   0        0        0     1919 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/config.py
--rw-r--r--   0        0        0        0 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/core/__init__.py
--rw-r--r--   0        0        0     1548 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/core/cppref.py
--rw-r--r--   0        0        0       41 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/core/exceptions.py
--rw-r--r--   0        0        0     3105 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/core/graphql_ref.py
--rw-r--r--   0        0        0     1179 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/core/template.py
--rw-r--r--   0        0        0     3226 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/generator.py
--rw-r--r--   0        0        0        0 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/operation/__init__.py
--rw-r--r--   0        0        0     4175 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/operation/definitions.py
--rw-r--r--   0        0        0    13573 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/operation/evaluation.py
--rw-r--r--   0        0        0      749 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/operation/template.py
--rw-r--r--   0        0        0        0 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/py.typed
--rw-r--r--   0        0        0        0 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/schema/__init__.py
--rw-r--r--   0        0        0     4164 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/schema/definitions.py
--rw-r--r--   0        0        0     8512 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/schema/evaluation.py
--rw-r--r--   0        0        0     1625 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/schema/template.py
--rw-r--r--   0        0        0      445 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/templates/CMakeLists.jinja.cmake
--rw-r--r--   0        0        0     1395 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp
--rw-r--r--   0        0        0     3059 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp
--rw-r--r--   0        0        0     1187 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp
--rw-r--r--   0        0        0     3367 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp
--rw-r--r--   0        0        0     5371 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/templates/operation.jinja.cpp
--rw-r--r--   0        0        0     5200 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/templates/operation.jinja.hpp
--rw-r--r--   0        0        0     3480 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/templates/schema.jinja.hpp
--rw-r--r--   0        0        0    16819 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/types.py
--rw-r--r--   0        0        0     1151 2023-06-27 12:33:59.119304 qtgql-0.122.0/qtgqlcodegen/utils.py
--rw-r--r--   0        0        0     2746 1970-01-01 00:00:00.000000 qtgql-0.122.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-02 14:25:50.094429 qtgql-0.123.0/LICENSE
+-rw-r--r--   0        0        0     1055 2023-07-02 14:25:50.094429 qtgql-0.123.0/README.md
+-rw-r--r--   0        0        0     4428 2023-07-02 14:26:10.810644 qtgql-0.123.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/__init__.py
+-rw-r--r--   0        0        0     1866 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/cli.py
+-rw-r--r--   0        0        0     1919 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/config.py
+-rw-r--r--   0        0        0        0 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/core/__init__.py
+-rw-r--r--   0        0        0     1548 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/core/cppref.py
+-rw-r--r--   0        0        0       41 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/core/exceptions.py
+-rw-r--r--   0        0        0     3105 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/core/graphql_ref.py
+-rw-r--r--   0        0        0     1179 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/core/template.py
+-rw-r--r--   0        0        0     3226 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/generator.py
+-rw-r--r--   0        0        0        0 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/operation/__init__.py
+-rw-r--r--   0        0        0     4202 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/operation/definitions.py
+-rw-r--r--   0        0        0    13608 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/operation/evaluation.py
+-rw-r--r--   0        0        0      749 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/operation/template.py
+-rw-r--r--   0        0        0        0 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/py.typed
+-rw-r--r--   0        0        0        0 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/schema/__init__.py
+-rw-r--r--   0        0        0     4164 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/schema/definitions.py
+-rw-r--r--   0        0        0     8512 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/schema/evaluation.py
+-rw-r--r--   0        0        0     1625 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/schema/template.py
+-rw-r--r--   0        0        0      445 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/templates/CMakeLists.jinja.cmake
+-rw-r--r--   0        0        0     1395 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp
+-rw-r--r--   0        0        0     3573 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp
+-rw-r--r--   0        0        0     1849 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp
+-rw-r--r--   0        0        0      448 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/templates/macros/iterate_type_condition.jinja.hpp
+-rw-r--r--   0        0        0      994 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/templates/macros/proxy_type_fields.jinja.hpp
+-rw-r--r--   0        0        0     4174 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp
+-rw-r--r--   0        0        0     2644 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/templates/macros/update_proxy_field.jinja.cpp
+-rw-r--r--   0        0        0     3536 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/templates/operation.jinja.cpp
+-rw-r--r--   0        0        0     4664 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/templates/operation.jinja.hpp
+-rw-r--r--   0        0        0     3532 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/templates/schema.jinja.hpp
+-rw-r--r--   0        0        0    16979 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/types.py
+-rw-r--r--   0        0        0     1151 2023-07-02 14:25:50.110429 qtgql-0.123.0/qtgqlcodegen/utils.py
+-rw-r--r--   0        0        0     1996 1970-01-01 00:00:00.000000 qtgql-0.123.0/PKG-INFO
```

### Comparing `qtgql-0.122.0/LICENSE` & `qtgql-0.123.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qtgql-0.122.0/pyproject.toml` & `qtgql-0.123.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qtgql"
-version = "0.122.0"
+version = "0.123.0"
 packages = [{ include = "qtgqlcodegen" }]
 description = "Qt framework for building graphql driven QML applications"
 authors = ["Nir <88795475+nrbnlulu@users.noreply.github.com>"]
 maintainers = ["Nir.J Benlulu <nrbnlulu@gmail.com>"]
 license = "MIT"
 readme = "README.md"
```

### Comparing `qtgql-0.122.0/qtgqlcodegen/cli.py` & `qtgql-0.123.0/qtgqlcodegen/cli.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.122.0/qtgqlcodegen/config.py` & `qtgql-0.123.0/qtgqlcodegen/config.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.122.0/qtgqlcodegen/core/cppref.py` & `qtgql-0.123.0/qtgqlcodegen/core/cppref.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.122.0/qtgqlcodegen/core/graphql_ref.py` & `qtgql-0.123.0/qtgqlcodegen/core/graphql_ref.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.122.0/qtgqlcodegen/core/template.py` & `qtgql-0.123.0/qtgqlcodegen/core/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.122.0/qtgqlcodegen/generator.py` & `qtgql-0.123.0/qtgqlcodegen/generator.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.122.0/qtgqlcodegen/operation/definitions.py` & `qtgql-0.123.0/qtgqlcodegen/operation/definitions.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     @cached_property
     def property_type(self) -> str:
         """
 
         :return: C++ property type that will be exposed to QML.
         """
         tp = self.type
-        if tp.is_queried_object_type:
+        if tp.is_queried_object_type or tp.is_queried_interface:
             return f"{self.type_name} *"
 
         if cs := tp.is_custom_scalar:
             return cs.to_qt_type
 
         if model := tp.is_model:
             if model.of_type.is_queried_object_type:
```

### Comparing `qtgql-0.122.0/qtgqlcodegen/operation/evaluation.py` & `qtgql-0.123.0/qtgqlcodegen/operation/evaluation.py`

 * *Files 7% similar despite different names*

```diff
@@ -228,63 +228,65 @@
 
 def _evaluate_interface(
     type_info: OperationTypeInfo,
     concrete: QtGqlInterface,
     selection_set: gql_lang.SelectionSetNode,
     path: str,  # current path in the query tree.
 ) -> QtGqlQueriedInterface:
-    # first get all linear selections.
-    linear_fields: dict[str, QtGqlQueriedField] = {}
-    choices: defaultdict[str, dict[str, QtGqlQueriedField]] = defaultdict(dict)
-
-    for selection in selection_set.selections:
-        if not is_inline_fragment(selection):
-            inner_field_node = is_field_node(selection)
-            assert inner_field_node
-            if not is_type_name_selection(inner_field_node):
-                __f = _evaluate_field(
-                    type_info=type_info,
-                    concrete_field=concrete.fields_dict[inner_field_node.name.value],
-                    field_node=inner_field_node,
-                    path=path,
-                    origin=concrete,
-                )
-                linear_fields[__f.name] = __f
+    choices: list[QtGqlQueriedObjectType] = []
 
+    # first get all linear selections, these are selection that can be applied to
+    # any of the interface implementors
+    inline_fragments: list[gql_lang.InlineFragmentNode] = []
+    linear_fields: dict[str, QtGqlQueriedField] = {}
+    for field_or_frag in selection_set.selections:
+        if inline_frag := is_inline_fragment(field_or_frag):
+            inline_fragments.append(inline_frag)
+        else:
+            field_node = is_field_node(field_or_frag)
+            assert field_node
+            __f = _evaluate_field(
+                type_info=type_info,
+                concrete_field=concrete.fields_dict[field_node.name.value],
+                field_node=field_node,
+                path=path,
+                origin=concrete,
+            )
+            linear_fields[__f.name] = __f
     # evaluate type conditions
-    for selection in selection_set.selections:
-        if inline_frag := is_inline_fragment(selection):
-            type_name = inline_frag.type_condition.name.value
-            # no need to validate inner types are implementation, graphql-core does this.
-            resolved_type = type_info.schema_type_info.get_object_type(
-                type_name,
-            ) or type_info.schema_type_info.get_interface(type_name)
-            assert resolved_type
-            for inner_selection in inline_frag.selection_set.selections:
-                inner_field_node = is_field_node(inner_selection)
-                assert inner_field_node
-                if not is_type_name_selection(inner_field_node):
-                    __f = _evaluate_field(
-                        type_info=type_info,
-                        concrete_field=resolved_type.fields_dict[inner_field_node.name.value],
-                        field_node=inner_field_node,
-                        path=path,
-                        origin=resolved_type,
-                    )
-                    choices[type_name][inner_field_node.name.value] = __f
-    for choice in choices.values():
-        choice.update(linear_fields)
+    for inline_frag in inline_fragments:
+        type_name = inline_frag.type_condition.name.value
+        # no need to validate inner types are implementation, graphql-core does this.
+        concrete_choice = type_info.schema_type_info.get_object_type(
+            type_name,
+        ) or type_info.schema_type_info.get_interface(type_name)
+        assert concrete_choice
+        choices.append(
+            _evaluate_object_type(
+                type_info=type_info,
+                concrete=concrete_choice,
+                selection_set=inline_frag.selection_set,
+                path=path,
+            ),
+        )
+
+        # inject __type_name selection, we'll use this to deserialize correctly.
+        if not has_typename_selection(inline_frag.selection_set):
+            inject_typename_selection(inline_frag.selection_set)
 
     name = f"{concrete.name}__{path}"
     ret = QtGqlQueriedInterface(
         name=name,
         concrete=concrete,
         choices=choices,
         fields_dict=linear_fields,
     )
+    for choice in choices:
+        choice.base_interface = ret
+        choice.fields_dict.update(linear_fields)
     type_info.narrowed_interfaces_map[name] = ret
     return ret
 
 
 def _evaluate_object_type(
     type_info: OperationTypeInfo,
     concrete: QtGqlObjectType,
@@ -294,14 +296,16 @@
     # inject id selection for node implementors, it is required for caching purposes.
     if concrete.implements_node and not has_id_selection(selection_set):
         inject_id_selection(selection_set)
 
     fields: dict[str, QtGqlQueriedField] = {}
     for selection in selection_set.selections:
         if f_node := is_field_node(selection):
+            if is_type_name_selection(f_node):
+                continue  # __type_name selection is handled with special care.
             concrete_field = concrete.fields_dict[f_node.name.value]
             fields[concrete_field.name] = _evaluate_field(
                 type_info=type_info,
                 concrete_field=concrete_field,
                 field_node=f_node,
                 path=path,
                 origin=concrete,
@@ -353,14 +357,15 @@
     root_field = root_proxy_type.fields[0]
     return QtGqlOperationDefinition(
         root_field=root_field,
         root_type=root_proxy_type,
         operation_def=operation,
         variables=type_info.variables,
         narrowed_types=tuple(type_info.narrowed_types_map.values()),
+        interfaces=tuple(type_info.narrowed_interfaces_map.values()),
     )
 
 
 class _OperationsVisitor(visitor.Visitor):
     def __init__(self, type_info: SchemaTypeInfo):
         super().__init__()
         self.schema_type_info = type_info
```

### Comparing `qtgql-0.122.0/qtgqlcodegen/operation/template.py` & `qtgql-0.123.0/qtgqlcodegen/operation/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.122.0/qtgqlcodegen/schema/definitions.py` & `qtgql-0.123.0/qtgqlcodegen/schema/definitions.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.122.0/qtgqlcodegen/schema/evaluation.py` & `qtgql-0.123.0/qtgqlcodegen/schema/evaluation.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.122.0/qtgqlcodegen/schema/template.py` & `qtgql-0.123.0/qtgqlcodegen/schema/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.122.0/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp` & `qtgql-0.123.0/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.122.0/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp` & `qtgql-0.123.0/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,30 @@
-{% macro deserialize_concrete_field(proxy_field, setter_name, operation_pointer = "operation",
+{%- from "macros/iterate_type_condition.jinja.hpp" import  iterate_type_condition -%}
+{% macro deserialize_concrete_field(proxy_field, operation_pointer = "operation",
                            do_after_deserialized = "") -%}
+{% set setter_name %}inst->👉 proxy_field.concrete.setter_name 👈{% endset %}
 {% set setter_end -%}
 {% if proxy_field.cached_by_args %}
 , 👉proxy_field.build_variables_tuple_for_field_arguments👈
 {% endif -%}
 {% endset -%}
 if (!data.value("👉proxy_field.name👈").isNull()){
 {% if proxy_field.type.is_queried_object_type -%}
 👉 setter_name 👈(👉proxy_field.type.deserializer_name👈(data.value("👉proxy_field.name👈").toObject(), 👉operation_pointer👈) 👉 setter_end 👈);
 
 {% elif proxy_field.type.is_queried_interface -%}
-if field_data:
-👉 setter_name 👈(👉proxy_field.type.is_interface.name👈.from_dict(
-        parent,
-        field_data,
-        inner_config,
-👉operation_pointer👈,
-👉 setter_end 👈);
+auto 👉proxy_field.name👈_data = data.value("👉proxy_field.name👈").toObject();
+auto 👉proxy_field.name👈_typename  = 👉proxy_field.name👈_data.value("__typename").toString();
+{%set type_cond -%}👉proxy_field.name👈_typename{% endset -%}
+{% for choice in proxy_field.type.choices -%}
+{% set do_on_meets -%}
+👉 setter_name 👈(👉choice.deserializer_name👈(👉proxy_field.name👈_data, 👉operation_pointer👈) 👉 setter_end 👈);
+{% endset -%}
+👉iterate_type_condition(choice,type_cond, do_on_meets, loop)👈
+{% endfor %}
 {% elif proxy_field.type.is_model -%}
 {% if proxy_field.type.is_model.of_type.is_queried_object_type -%}
 👉proxy_field.concrete.type.member_type👈 obj_list;
 for (const auto& node: data.value("👉proxy_field.name👈").toArray()){
 obj_list.append(👉 proxy_field.type.is_model.of_type.is_queried_object_type.deserializer_name 👈(node.toObject(), 👉operation_pointer👈));
 };
 👉 setter_name 👈(obj_list👉 setter_end 👈);
```

### Comparing `qtgql-0.122.0/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp` & `qtgql-0.123.0/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,30 @@
+{%- from "macros/iterate_type_condition.jinja.hpp" import  iterate_type_condition -%}
 {% macro initialize_proxy_field(field, operation_pointer = "operation") -%}
 {%set instance_of_concrete -%}
 m_inst->👉field.concrete.getter_name 👈(👉field.build_variables_tuple_for_field_arguments 👈)
 {% endset -%}
 
 {% if field.type.is_queried_object_type  and field.type.is_optional %}
 if (👉 instance_of_concrete 👈){
 👉field.private_name👈 = new 👉field.type_name👈(👉operation_pointer👈, 👉 instance_of_concrete 👈);
 }
-else{
-👉field.private_name👈 = nullptr;
-}
 {% elif field.type.is_queried_object_type %}
 👉field.private_name👈 = new 👉field.type_name👈(👉operation_pointer👈, 👉 instance_of_concrete 👈);
 {% elif field.type.is_model and field.type.is_model.of_type.is_queried_object_type %}
 auto init_list_👉 field.name 👈 =  std::make_unique<QList<👉field.type.of_type.name👈*>>();
 for (const auto & node: 👉 instance_of_concrete 👈){
 init_list_👉 field.name 👈->append(new 👉field.type.of_type.name👈(👉operation_pointer👈, node));
 }
 👉field.private_name👈 = new qtgql::bases::ListModelABC<👉 field.type.of_type.name 👈>(this, std::move(init_list_👉 field.name 👈));
+{% elif field.type.is_queried_interface %}
+auto concrete_👉field.name👈 = 👉 instance_of_concrete 👈;
+auto 👉field.name👈_typename = concrete_👉field.name👈->TYPE_NAME();
+{%set type_cond -%}👉field.name👈_typename{% endset -%}
+{% for choice in field.type.choices -%}
+{% set do_on_meets -%}
+👉field.private_name👈 = qobject_cast<👉 field.type.name 👈*>(new 👉choice.type_name()👈(👉operation_pointer👈, std::static_pointer_cast<👉 choice.concrete.name 👈>(concrete_👉field.name👈)));
+{% endset -%}
+👉iterate_type_condition(choice,type_cond, do_on_meets, loop)👈
+{% endfor %}
 {% endif -%}
 {% endmacro -%}
```

### Comparing `qtgql-0.122.0/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp` & `qtgql-0.123.0/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 {%- from "macros/deserialize_concrete_field.jinja.hpp" import  deserialize_concrete_field -%}
+{%- from "macros/iterate_type_condition.jinja.hpp" import  iterate_type_condition -%}
 {% macro update_concrete_field(proxy_field,f_concrete, private_name, operation_pointer="operation") -%}
 {% if proxy_field.variable_uses  -%}
 👉f_concrete.arguments_type👈 👉private_name👈_args = 👉proxy_field.build_variables_tuple_for_field_arguments👈;
 {% endif %}
 {%- set current -%}
 {% if proxy_field.variable_uses  -%}
 inst->👉private_name👈.at(👉private_name👈_args)
@@ -13,23 +14,24 @@
 {% set setter_end -%}
 {% if proxy_field.variable_uses -%}
 , 👉private_name👈_args
 {% endif -%}
 {%- endset -%}
 {%- set setter_name -%}inst->👉 proxy_field.concrete.setter_name 👈{% endset -%}
 
-{%- if proxy_field.is_root and f_concrete.type.is_object_type -%}
+{%- if proxy_field.is_root and f_concrete.type.is_object_type or f_concrete.type.is_interface -%}
 {#- // root fields that has no default value might not have value even if they are not optional -#}
 {% if proxy_field.variable_uses  -%}
 if (!inst->👉private_name👈.contains(👉private_name👈_args))
 {% else -%}
 if (!👉current👈)
 {% endif %}
 {
-    👉deserialize_concrete_field(proxy_field, setter_name)👈
+    {#- // Note: we can't use deserializer name since it might not be an object type. -#}
+    👉deserialize_concrete_field(proxy_field)👈
 }
 else
 {% endif -%}
 if (!data.value("👉f_concrete.name👈").isNull()){
 {% if proxy_field.type.is_builtin_scalar -%}
 {% if proxy_field.type.is_void -%}
 /* deliberately empty */
@@ -54,20 +56,30 @@
     else{
     👉 setter_name 👈(👉proxy_field.type.deserializer_name👈(👉f_concrete.name👈_data, 👉operation_pointer👈) 👉 setter_end 👈);
     }
     {% else %}
     👉proxy_field.type.updater_name👈(👉current👈, 👉f_concrete.name👈_data,  👉operation_pointer👈);
     {% endif %}
 {% elif proxy_field.type.is_model %}
-👉deserialize_concrete_field(proxy_field, setter_name)👈
+👉deserialize_concrete_field(proxy_field)👈
 {% elif proxy_field.type.is_enum %}
 auto new_👉f_concrete.name👈= Enums::👉proxy_field.type.is_enum.map_name👈::by_name(data.value("👉proxy_field.name👈").toString());
 if (👉current👈 != new_👉f_concrete.name👈){
 👉 setter_name 👈(new_👉f_concrete.name👈 👉 setter_end 👈);
 }
+{% elif proxy_field.type.is_queried_interface %}
+auto 👉f_concrete.name👈_data = data.value("👉f_concrete.name👈").toObject();
+auto 👉f_concrete.name👈_typename  = 👉f_concrete.name👈_data.value("__typename").toString();
+{%set type_cond -%}👉f_concrete.name👈_typename{% endset -%}
+{% for choice in proxy_field.type.choices %}
+{% set do_on_meets -%}
+👉choice.updater_name👈(std::static_pointer_cast<👉choice.concrete.name👈>(👉current👈), 👉f_concrete.name👈_data,  👉operation_pointer👈);
+{% endset -%}
+👉iterate_type_condition(choice,type_cond, do_on_meets, loop)👈
+{% endfor %}
 {% else %}
 throw qtgql::exceptions::NotImplementedError({"👉proxy_field.type.__class__.__name__👈 is not supporting updates ATM"});
 {% endif %}
 }
 {% if proxy_field.type.is_optional %}
 else {
 👉 setter_name 👈({} 👉 setter_end 👈);
```

### Comparing `qtgql-0.122.0/qtgqlcodegen/templates/operation.jinja.hpp` & `qtgql-0.123.0/qtgqlcodegen/templates/operation.jinja.hpp`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-{%- from "macros/initialize_proxy_field.jinja.hpp" import initialize_proxy_field -%}
 {%- from "macros/deserialize_concrete_field.jinja.hpp" import  deserialize_concrete_field -%}
+{%- from "macros/proxy_type_fields.jinja.hpp" import  proxy_type_fields -%}
 #pragma once
 #include "./schema.hpp"
 #include <qtgql/gqlwstransport/gqlwstransport.hpp>
 #include <QObject>
 
 namespace 👉 context.config.env_name 👈::👉context.ns👈{
 class 👉 context.operation.name 👈;
@@ -17,69 +17,50 @@
 {% endfor -%}
 };
 
 namespace updaters{
 {% for t in context.operation.narrowed_types -%}
 void update_👉 t.name 👈(👉 t.concrete.member_type_arg 👈 inst, const QJsonObject &data, const 👉 context.operation.name 👈 * operation);
 {% endfor -%}
-
 };
 
-// ------------ Narrowed Object types ------------
-{% for t in context.operation.narrowed_types %}
+// ------------ Narrowed Interfaces ------------
+{% for t in context.operation.interfaces -%}
 class 👉 t.name 👈: public QObject{
-    Q_OBJECT
+👉 proxy_type_fields(t, context) 👈
+public:
+    using QObject::QObject;
 {% for f in t.fields -%}
-Q_PROPERTY(const 👉 f.property_type 👈 👉 f.name 👈 READ 👉 f.concrete.getter_name 👈 NOTIFY 👉 f.concrete.signal_name 👈);
-{% endfor %}
-signals:
-{%for f in t.fields -%}
-void 👉 f.concrete.signal_name 👈();
-{% endfor %}
-
-{# members #}
-{% if context.debug -%}
-public: // WARNING: members are public because you have debug=True in your config file.
-{% else %}
-protected:
-{% endif %}
-{% if t.concrete.is_root %} {# // root types are singletons, no need for shared ptr -#}
-👉context.schema_ns👈::👉 t.concrete.name 👈 * m_inst;
-{% else %}
-const std::shared_ptr<👉context.schema_ns👈::👉 t.concrete.name 👈> m_inst;
-{% endif %}
-{% for ref_field in t.references -%}
-const 👉ref_field.property_type👈 m_👉ref_field.name👈 = {};
+[[nodiscard]] inline virtual const 👉 f.property_type 👈  👉 f.concrete.getter_name 👈() const {
+throw qtgql::exceptions::InterfaceDirectAccessError("👉t.concrete.name👈");
+}
 {% endfor %}
-{%- for model_field in t.models -%}
-👉 model_field.property_type 👈 👉model_field.private_name👈;
+};
 {% endfor %}
-
+// ------------ Narrowed Object types ------------
+{% for t in context.operation.narrowed_types %}
+class 👉 t.name 👈: public 👉 "QObject" if not t.base_interface else t.base_interface.name 👈{
+👉 proxy_type_fields(t, context) 👈
 public:
 {% if t.concrete.is_root -%}
 👉 t.name 👈(👉 context.operation.name 👈 * operation);
 {% else -%}
 👉 t.name 👈(👉 context.operation.name 👈 * operation, const std::shared_ptr<👉 t.concrete.name 👈> &inst);
-{% endif -%}
-
-
+{% endif %}
+public:
 {% for f in t.fields -%}
-{%- if f.type.is_queried_object_type or f.type.is_model %}
 [[nodiscard]] inline const 👉 f.property_type 👈  👉 f.concrete.getter_name 👈() const {
-    return m_👉f.name👈;
+{%- if f.type.is_queried_object_type or f.type.is_model or f.type.is_queried_interface %}
+return m_👉f.name👈;
 {%- else -%}
-[[nodiscard]] inline const 👉 f.property_type 👈 👉 f.concrete.getter_name 👈() const {
-    {% if f.type.is_queried_object_type -%}
-    return *m_👉f.name👈;
-    {% else -%}
-    return m_inst->👉 f.concrete.getter_name 👈();
-    {% endif -%}
+return m_inst->👉 f.concrete.getter_name 👈();
 {%- endif -%}
 };
 {% endfor -%}
+
 };
 {% endfor %}
 
 struct 👉 context.operation.generated_variables_type 👈{
 {% for var in context.operation.variables -%}
 std::optional<👉 var.type.member_type 👈> 👉 var.name 👈 = {};
 {% endfor -%}
@@ -124,22 +105,22 @@
 
 inline const QUuid & operation_id() const override{
 return m_operation_id;
 }
 
 
 void on_next(const QJsonObject &message) override{
+    auto data = message.value("data").toObject();
     if (!m_data){
-        auto data = message.value("data").toObject();
         👉 context.operation.root_type.updater_name👈(👉 context.operation.root_type.concrete.name👈::instance(), data, this);
         m_data = new 👉 context.operation.root_type.name👈(this);
         emit dataChanged();
     }
     else{
-    throw qtgql::exceptions::NotImplementedError({"Updates on root types is not implemented yet."});
+        👉 context.operation.root_type.updater_name👈(👉 context.operation.root_type.concrete.name👈::instance(), data, this);
     }
 }
 
 inline const 👉 context.operation.root_type.name 👈 * data() const{
     if (m_data){
         return m_data.value();
     }
```

### Comparing `qtgql-0.122.0/qtgqlcodegen/templates/schema.jinja.hpp` & `qtgql-0.123.0/qtgqlcodegen/templates/schema.jinja.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,18 @@
 }
 {% else %}
 QTGQL_STATIC_MAKE_SHARED(👉 type.name 👈)
 {% endif %}
 
 👉 type.name 👈()= default;
 
-inline static const QString TYPE_NAME = "👉 type.name 👈";
+inline const QString & TYPE_NAME() final{
+    static const QString ret = "👉 type.name 👈";
+    return ret;
+};
 
 {% if type.implements_node -%}
 static std::optional<std::shared_ptr<👉 type.name 👈>> get_node(const QString & id){
     auto node = ENV_CACHE()->get_node(id);
     if (node.has_value()){
         return std::static_pointer_cast<👉 type.name 👈>(node.value());
     }
```

### Comparing `qtgql-0.122.0/qtgqlcodegen/types.py` & `qtgql-0.123.0/qtgqlcodegen/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,15 +281,15 @@
         not_unique_interfaces: list[QtGqlInterface] = []
 
         if not self.interfaces_raw:
             # TODO(https://github.com/qtgql/qtgql/issues/267): these are not really interfaces though they are inherited if there are no interfaces.
             if interface := self.is_interface:
                 if interface.is_node_interface:
                     return [QtGqlTypes.NodeInterfaceABC]  # type: ignore
-
+                return [QtGqlTypes.ObjectTypeABC]  # type: ignore
             else:
                 return [QtGqlTypes.ObjectTypeABC]  # type: ignore
 
         for interface in self.interfaces_raw:
             for other in self.interfaces_raw:
                 if other is not interface:
                     if interface.implements(other):
@@ -432,14 +432,15 @@
 
 
 @define(slots=False, repr=False)
 class QtGqlQueriedObjectType(QtGqlQueriedTypeABC, QtGqlTypeABC):
     name: str
     concrete: QtGqlObjectType
     fields_dict: dict[str, QtGqlQueriedField] = attrs.Factory(dict)
+    base_interface: QtGqlQueriedInterface | None = None  # I think that there could be only one
 
     @property
     def is_queried_object_type(self) -> QtGqlQueriedObjectType | None:
         return self
 
     @cached_property
     def fields(self) -> tuple[QtGqlQueriedField, ...]:
@@ -454,30 +455,30 @@
         return f"updaters::update_{self.name}"
 
     def type_name(self) -> str:
         return self.name
 
     @cached_property
     def references(self) -> list[QtGqlQueriedField]:
-        return [f for f in self.fields if f.type.is_queried_object_type]
+        return [
+            f for f in self.fields if f.type.is_queried_object_type or f.type.is_queried_interface
+        ]
 
     @cached_property
     def models(self) -> list[QtGqlQueriedField]:
         return [f for f in self.fields if f.type.is_model]
 
     @cached_property
     def private_name(self) -> str:
         return f"m_{self.name}"
 
 
 @define(slots=False, repr=False)
 class QtGqlQueriedInterface(QtGqlQueriedObjectType):
-    choices: defaultdict[str, dict[str, QtGqlQueriedField]] = attrs.Factory(
-        lambda: defaultdict(dict),
-    )
+    choices: list[QtGqlQueriedObjectType] = attrs.Factory(list)
 
     @property
     def is_queried_object_type(self) -> QtGqlQueriedObjectType | None:
         return None
 
     @property
     def is_queried_interface(self) -> QtGqlQueriedInterface | None:
```

### Comparing `qtgql-0.122.0/qtgqlcodegen/utils.py` & `qtgql-0.123.0/qtgqlcodegen/utils.py`

 * *Files identical despite different names*

