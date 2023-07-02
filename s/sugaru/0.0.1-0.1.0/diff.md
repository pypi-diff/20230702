# Comparing `tmp/sugaru-0.0.1.tar.gz` & `tmp/sugaru-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sugaru-0.0.1.tar", max compression
+gzip compressed data, was "sugaru-0.1.0.tar", max compression
```

## Comparing `sugaru-0.0.1.tar` & `sugaru-0.1.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0        9 2023-04-29 11:30:37.987300 sugaru-0.0.1/README.md
--rw-r--r--   0        0        0     2932 2023-05-30 19:59:23.909689 sugaru-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      207 2023-05-30 19:01:44.923763 sugaru-0.0.1/sugaru/__init__.py
--rw-r--r--   0        0        0     3945 2023-05-30 19:25:52.032423 sugaru-0.0.1/sugaru/__main__.py
--rw-r--r--   0        0        0      361 2023-05-30 19:25:52.032486 sugaru-0.0.1/sugaru/file_loader/__init__.py
--rw-r--r--   0        0        0       43 2023-05-27 10:32:35.934813 sugaru-0.0.1/sugaru/file_loader/logging.py
--rw-r--r--   0        0        0      213 2023-05-28 12:51:09.154439 sugaru-0.0.1/sugaru/file_loader/simple_json/__init__.py
--rw-r--r--   0        0        0       27 2023-05-27 09:56:20.482663 sugaru-0.0.1/sugaru/file_loader/simple_yaml/__init__.py
--rw-r--r--   0        0        0      900 2023-05-30 19:27:41.258566 sugaru-0.0.1/sugaru/file_loader/simple_yaml/loader.py
--rw-r--r--   0        0        0       57 2023-05-28 12:23:31.427955 sugaru-0.0.1/sugaru/file_loader/types.py
--rw-r--r--   0        0        0      715 2023-05-30 19:25:52.032591 sugaru-0.0.1/sugaru/file_writer/__init__.py
--rw-r--r--   0        0        0       43 2023-05-27 10:45:29.328049 sugaru-0.0.1/sugaru/file_writer/logging.py
--rw-r--r--   0        0        0      305 2023-05-28 12:54:11.428563 sugaru-0.0.1/sugaru/file_writer/simple_json/__init__.py
--rw-r--r--   0        0        0      558 2023-05-28 13:06:33.113696 sugaru-0.0.1/sugaru/file_writer/simple_yaml/__init__.py
--rw-r--r--   0        0        0       57 2023-05-28 16:42:06.420378 sugaru-0.0.1/sugaru/file_writer/types.py
--rw-r--r--   0        0        0     1450 2023-05-30 19:31:14.568144 sugaru-0.0.1/sugaru/interfaces.py
--rw-r--r--   0        0        0      242 2023-04-30 11:20:40.610572 sugaru-0.0.1/sugaru/logging.py
--rw-r--r--   0        0        0      168 2023-05-28 18:18:21.215541 sugaru-0.0.1/sugaru/object_loader/__init__.py
--rw-r--r--   0        0        0      745 2023-05-31 17:38:01.828666 sugaru-0.0.1/sugaru/object_loader/module_loader.py
--rw-r--r--   0        0        0      386 2023-05-27 16:36:46.779457 sugaru-0.0.1/sugaru/object_loader/object_creator.py
--rw-r--r--   0        0        0      972 2023-05-28 17:34:49.316099 sugaru-0.0.1/sugaru/object_loader/objects_loader.py
--rw-r--r--   0        0        0     1921 2023-05-28 19:15:12.928361 sugaru-0.0.1/sugaru/object_loader/simple_loader.py
--rw-r--r--   0        0        0       45 2023-05-30 17:57:12.076838 sugaru-0.0.1/sugaru/plugin_executor/__init__.py
--rw-r--r--   0        0        0     1512 2023-05-30 18:23:39.001664 sugaru-0.0.1/sugaru/plugin_executor/executor.py
--rw-r--r--   0        0        0        0 2023-04-29 11:56:35.917536 sugaru-0.0.1/sugaru/py.typed
--rw-r--r--   0        0        0     2088 2023-05-30 18:23:26.953458 sugaru-0.0.1/sugaru/sugarator.py
--rw-r--r--   0        0        0      216 2023-05-30 19:05:44.288717 sugaru-0.0.1/sugaru/types.py
--rw-r--r--   0        0        0      343 2023-05-30 19:27:20.564411 sugaru-0.0.1/sugaru/utils/__init__.py
--rw-r--r--   0        0        0      697 2023-05-30 18:28:46.359589 sugaru-0.0.1/sugaru/utils/encode_decode.py
--rw-r--r--   0        0        0      365 2023-05-30 19:26:29.360833 sugaru-0.0.1/sugaru/utils/names_and_types.py
--rw-r--r--   0        0        0      508 2023-05-30 18:40:24.190184 sugaru-0.0.1/sugaru/utils/object_loading.py
--rw-r--r--   0        0        0     1499 2023-05-28 16:49:43.294965 sugaru-0.0.1/sugaru/utils/signature.py
--rw-r--r--   0        0        0      934 2023-05-31 18:15:48.334230 sugaru-0.0.1/setup.py
--rw-r--r--   0        0        0      923 2023-05-31 18:15:48.334363 sugaru-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-02 18:21:56.816316 sugaru-0.1.0/LICENSE
+-rw-r--r--   0        0        0     6690 2023-07-02 18:21:56.816316 sugaru-0.1.0/README.md
+-rw-r--r--   0        0        0     2932 2023-07-02 18:21:56.820316 sugaru-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      207 2023-07-02 18:21:56.820316 sugaru-0.1.0/sugaru/__init__.py
+-rw-r--r--   0        0        0     4112 2023-07-02 18:21:56.820316 sugaru-0.1.0/sugaru/__main__.py
+-rw-r--r--   0        0        0      361 2023-07-02 18:21:56.820316 sugaru-0.1.0/sugaru/file_loader/__init__.py
+-rw-r--r--   0        0        0       43 2023-07-02 18:21:56.820316 sugaru-0.1.0/sugaru/file_loader/logging.py
+-rw-r--r--   0        0        0      213 2023-07-02 18:21:56.820316 sugaru-0.1.0/sugaru/file_loader/simple_json/__init__.py
+-rw-r--r--   0        0        0       27 2023-07-02 18:21:56.820316 sugaru-0.1.0/sugaru/file_loader/simple_yaml/__init__.py
+-rw-r--r--   0        0        0      900 2023-07-02 18:21:56.820316 sugaru-0.1.0/sugaru/file_loader/simple_yaml/loader.py
+-rw-r--r--   0        0        0       57 2023-07-02 18:21:56.820316 sugaru-0.1.0/sugaru/file_loader/types.py
+-rw-r--r--   0        0        0      715 2023-07-02 18:21:56.820316 sugaru-0.1.0/sugaru/file_writer/__init__.py
+-rw-r--r--   0        0        0       43 2023-07-02 18:21:56.820316 sugaru-0.1.0/sugaru/file_writer/logging.py
+-rw-r--r--   0        0        0      305 2023-07-02 18:21:56.820316 sugaru-0.1.0/sugaru/file_writer/simple_json/__init__.py
+-rw-r--r--   0        0        0      558 2023-07-02 18:21:56.820316 sugaru-0.1.0/sugaru/file_writer/simple_yaml/__init__.py
+-rw-r--r--   0        0        0       57 2023-07-02 18:21:56.820316 sugaru-0.1.0/sugaru/file_writer/types.py
+-rw-r--r--   0        0        0     1450 2023-07-02 18:21:56.820316 sugaru-0.1.0/sugaru/interfaces.py
+-rw-r--r--   0        0        0      762 2023-07-02 18:21:56.820316 sugaru-0.1.0/sugaru/logging.py
+-rw-r--r--   0        0        0      168 2023-07-02 18:21:56.820316 sugaru-0.1.0/sugaru/object_loader/__init__.py
+-rw-r--r--   0        0        0      760 2023-07-02 18:21:56.820316 sugaru-0.1.0/sugaru/object_loader/module_loader.py
+-rw-r--r--   0        0        0      386 2023-07-02 18:21:56.820316 sugaru-0.1.0/sugaru/object_loader/object_creator.py
+-rw-r--r--   0        0        0      972 2023-07-02 18:21:56.820316 sugaru-0.1.0/sugaru/object_loader/objects_loader.py
+-rw-r--r--   0        0        0     1921 2023-07-02 18:21:56.820316 sugaru-0.1.0/sugaru/object_loader/simple_loader.py
+-rw-r--r--   0        0        0       45 2023-07-02 18:21:56.820316 sugaru-0.1.0/sugaru/plugin_executor/__init__.py
+-rw-r--r--   0        0        0     1729 2023-07-02 18:21:56.820316 sugaru-0.1.0/sugaru/plugin_executor/executor.py
+-rw-r--r--   0        0        0        0 2023-07-02 18:21:56.820316 sugaru-0.1.0/sugaru/py.typed
+-rw-r--r--   0        0        0     2088 2023-07-02 18:21:56.820316 sugaru-0.1.0/sugaru/sugarator.py
+-rw-r--r--   0        0        0      335 2023-07-02 18:21:56.824316 sugaru-0.1.0/sugaru/types.py
+-rw-r--r--   0        0        0      242 2023-07-02 18:21:56.824316 sugaru-0.1.0/sugaru/utils/__init__.py
+-rw-r--r--   0        0        0      746 2023-07-02 18:21:56.824316 sugaru-0.1.0/sugaru/utils/encode_decode.py
+-rw-r--r--   0        0        0      507 2023-07-02 18:21:56.824316 sugaru-0.1.0/sugaru/utils/names_and_types.py
+-rw-r--r--   0        0        0      551 2023-07-02 18:21:56.824316 sugaru-0.1.0/sugaru/utils/object_loading.py
+-rw-r--r--   0        0        0     2695 2023-07-02 18:21:56.824316 sugaru-0.1.0/sugaru/utils/signature.py
+-rw-r--r--   0        0        0     7604 1970-01-01 00:00:00.000000 sugaru-0.1.0/PKG-INFO
```

### Comparing `sugaru-0.0.1/pyproject.toml` & `sugaru-0.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 lines_after_imports = 2
 include_trailing_comma = true
 use_parentheses= true
 
 
 [tool.poetry]
 name = "sugaru"
-version = "0.0.1"
+version = "0.1.0"
 description = "Create your own syntax stupidly simple!"
 readme = "README.md"
 license = "MIT"
 authors = ["Dmitry Makarov <mit.makaroff@gmail.com>"]
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
```

### Comparing `sugaru-0.0.1/sugaru/__main__.py` & `sugaru-0.1.0/sugaru/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from enum import Enum
 from pathlib import Path
 from typing import List
 
 import typer
 
 from .file_loader import loader_by_extension
 from .file_writer import stdout_writer_by_extension, writer_by_extension
@@ -9,15 +10,15 @@
     FinalFileWriter,
     ObjectLoader,
     PluginExecutor,
     SectionDecoder,
     SectionEncoder,
     SugarFileLoader,
 )
-from .logging import logger
+from .logging import LogLevel, logger, set_log_level
 from .object_loader import SimpleObjectLoader
 from .plugin_executor import simple_plugin_executor
 from .sugarator import sugarate
 from .utils import Final, decode_section, encode_section, load_object_or_raise_error
 
 
 STDOUT: Final[str] = "stdout"
@@ -34,37 +35,38 @@
     output: str = STDOUT,
     obj_loader: str = AUTO,
     file_loader: str = AUTO,
     file_writer: str = AUTO,
     sec_encoder: str = AUTO,
     sec_decoder: str = AUTO,
     plug_executor: str = AUTO,
-    type_check: bool = True,
+    log_level: Enum("", {level.name: level.name for level in LogLevel}) = LogLevel.INFO.name,  # type: ignore
 ) -> None:
+    set_log_level(LogLevel[log_level.value])
     file_path: Path = Path(file)
     if not file_path.is_file():
         logger.warning(f"File '{file}' does not exist or is not a file")
         return
 
     object_loader: ObjectLoader = SimpleObjectLoader()
     if obj_loader != AUTO:
         object_loader = load_object_or_raise_error(
             object_loader,
             obj_name=obj_loader,
             class_=ObjectLoader,
-            type_check=type_check,
+            type_check=False,
         )
 
     sugar_file_loader: SugarFileLoader
     if file_loader != AUTO:
         sugar_file_loader = load_object_or_raise_error(
             object_loader,
             obj_name=file_loader,
             class_=SugarFileLoader,
-            type_check=type_check,
+            type_check=False,
         )
     else:
         ext: str = file_path.suffix
         if ext not in loader_by_extension:
             logger.warning(f"Cannot find plugin loader by extension '{ext}'")
             return
 
@@ -74,65 +76,68 @@
 
     output_path: Path = file_path
     if file_writer != AUTO:
         sugar_file_writer = load_object_or_raise_error(
             object_loader,
             obj_name=file_writer,
             class_=FinalFileWriter,
-            type_check=type_check,
+            type_check=False,
         )
     else:
-        if output == STDOUT:
-            sugar_file_writer = stdout_writer_by_extension[file_path.suffix]
-        else:
+        write_obj_by_ext = stdout_writer_by_extension
+        out_ext: str = file_path.suffix
+
+        if output != STDOUT:
             output_path = Path(output)
-            out_ext: str = output_path.suffix
+            out_ext = output_path.suffix
+            write_obj_by_ext = writer_by_extension
+
+        if out_ext not in write_obj_by_ext:
+            logger.warning(f"cannot find plugin writer by extension '{out_ext}'")
+            return
 
-            if out_ext not in writer_by_extension:
-                logger.warning(f"cannot find plugin writer by extension '{out_ext}'")
-                return
-            sugar_file_writer = writer_by_extension[out_ext]
+        sugar_file_writer = write_obj_by_ext[out_ext]
 
     section_encoder: SectionEncoder = encode_section
     section_decoder: SectionDecoder = decode_section
 
     if sec_encoder != AUTO:
         section_encoder = load_object_or_raise_error(
             object_loader,
             obj_name=sec_encoder,
             class_=SectionEncoder,
-            type_check=type_check,
+            type_check=False,
         )
 
     if sec_decoder != AUTO:
         section_decoder = load_object_or_raise_error(
             object_loader,
             obj_name=sec_decoder,
             class_=SectionDecoder,
-            type_check=type_check,
+            type_check=False,
         )
 
     plugin_executor: PluginExecutor = simple_plugin_executor
     if plug_executor != AUTO:
         plugin_executor = load_object_or_raise_error(
             object_loader,
             obj_name=plug_executor,
             class_=PluginExecutor,
-            type_check=type_check,
+            type_check=False,
         )
 
     sugarate(
         plugin_name_list=plugin,
         object_loader=object_loader,
         sugar_file_path=file_path,
         sugar_file_loader=sugar_file_loader,
         final_file_path=output_path,
         final_file_writer=sugar_file_writer,
         section_encoder=section_encoder,
         section_decoder=section_decoder,
         plugin_executor=plugin_executor,
-        type_check=type_check,
+        type_check=False,
     )
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `sugaru-0.0.1/sugaru/file_loader/simple_yaml/loader.py` & `sugaru-0.1.0/sugaru/file_loader/simple_yaml/loader.py`

 * *Files identical despite different names*

### Comparing `sugaru-0.0.1/sugaru/file_writer/__init__.py` & `sugaru-0.1.0/sugaru/file_writer/__init__.py`

 * *Files identical despite different names*

### Comparing `sugaru-0.0.1/sugaru/file_writer/simple_yaml/__init__.py` & `sugaru-0.1.0/sugaru/file_writer/simple_yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `sugaru-0.0.1/sugaru/interfaces.py` & `sugaru-0.1.0/sugaru/interfaces.py`

 * *Files identical despite different names*

### Comparing `sugaru-0.0.1/sugaru/object_loader/module_loader.py` & `sugaru-0.1.0/sugaru/object_loader/module_loader.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 def load_module(plugin_name: str) -> Optional[ModuleType]:
     module_name: str = plugin_name
     while True:
         logger.trace(f"Try to import module by name '{module_name}'")
         try:
             return import_module(module_name)
-        except ModuleNotFoundError:
-            logger.trace(f"Module '{module_name}' import failed.")
+        except ModuleNotFoundError as exc:
+            logger.trace(f"Module '{module_name}' import failed ({exc}).")
             if plugin_name != module_name or "." not in module_name:
                 break
 
             module_name, plugin = module_name.rsplit(".", maxsplit=1)
             logger.trace(f"Consider '{module_name}' as module name and '{plugin}' as plugin name")
 
     return None
```

### Comparing `sugaru-0.0.1/sugaru/object_loader/objects_loader.py` & `sugaru-0.1.0/sugaru/object_loader/objects_loader.py`

 * *Files identical despite different names*

### Comparing `sugaru-0.0.1/sugaru/object_loader/simple_loader.py` & `sugaru-0.1.0/sugaru/object_loader/simple_loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,26 +37,26 @@
             if check_callable_signature(
                 obj,
                 class_=class_,
                 type_check=type_check,
             )
         ]
 
-        logger.debug(
+        logger.trace(
             f"{_self}: classes after signature check: {[p.__name__ for p in object_classes]}"
         )
 
         objects: List[Callable] = []
         for obj_class in object_classes:
             obj: Optional[Callable] = create_object(obj_class)
             if not obj:
                 logger.info(
                     f"{_self}: Object '{callable_name(obj_class)}' can't be created in a simple way. Skip."
                 )
                 continue
             objects.append(obj)
 
-        logger.debug(
+        logger.trace(
             f"{_self}: objects after classes instantiating: {[callable_name(p) for p in objects]}"
         )
 
         return objects
```

### Comparing `sugaru-0.0.1/sugaru/plugin_executor/executor.py` & `sugaru-0.1.0/sugaru/plugin_executor/executor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from copy import deepcopy
-from typing import Dict, Mapping, cast
+from typing import Any, Dict, Mapping
 
 from ..interfaces import Plugin
 from ..logging import logger
 from ..types import SecName, Section
+from ..utils import callable_params
 
 
 def simple_plugin_executor(
     *,
     sections: Mapping[str, Section],
     plugins: Mapping[str, Plugin],
 ) -> Dict[str, Section]:
@@ -18,28 +19,30 @@
     plugin_name: str
     plugin: Plugin
 
     sections_template: Mapping[str, Section] = deepcopy(sections)
 
     for section_name, section in sections.items():
         for plugin_name, plugin in plugins.items():
-            section_to_pass: Section = cast(
-                Section,
-                deepcopy(
-                    sugar_sections.get(section_name, section),
-                ),
-            )
-
-            new_section: Section = plugin(
-                section_name=section_name,
-                section=section_to_pass,
-                sections=sections,
-            )
+            plugin_params: Dict[str, Any] = callable_params(plugin)
 
-            if new_section != section_to_pass:
+            values: Dict[str, Any] = {
+                "section_name": section_name,
+                "sections": sections,
+            }
+            if "section" in plugin_params:
+                values["section"] = deepcopy(sugar_sections.get(section_name, section))
+
+            kwargs: Dict[str, Any] = {
+                param_name: values[param_name] for param_name in plugin_params
+            }
+
+            new_section: Section = plugin(**kwargs)
+
+            if kwargs.get("section") and new_section != kwargs["section"]:
                 logger.trace(f"Section '{section_name}' was modified by plugin '{plugin_name}'")
 
             sugar_sections[section_name] = new_section
 
             if sections != sections_template:
                 raise RuntimeError(
                     f"Plugin '{plugin_name}' modified sections, but it's forbidden."
```

### Comparing `sugaru-0.0.1/sugaru/sugarator.py` & `sugaru-0.1.0/sugaru/sugarator.py`

 * *Files identical despite different names*

### Comparing `sugaru-0.0.1/sugaru/utils/encode_decode.py` & `sugaru-0.1.0/sugaru/utils/encode_decode.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from typing import Dict
 
 from ..types import JSON, SecName, Section
 
 
+__all__ = ["decode_section", "encode_section"]
+
+
 def encode_section(content: JSON) -> Dict[SecName, Section]:
     if isinstance(content, list):
         return {str(i): item for i, item in enumerate(content)}
 
     if isinstance(content, (str, int, float, type(None), bool)):
         return {"": content}
```

### Comparing `sugaru-0.0.1/sugaru/utils/signature.py` & `sugaru-0.1.0/sugaru/utils/signature.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,92 @@
 from inspect import Signature, isclass, isfunction, signature
-from typing import Any, Dict, Type
+from types import FunctionType
+from typing import Any, Callable, Dict, Optional, Tuple, Type, Union
 
+from ..interfaces import Plugin
 from ..logging import logger
+from ..utils import callable_name
 from .names_and_types import is_builtin
 
 
-def check_callable_signature(
-    obj: Type[Any],
-    class_: Type[Any],
-    *,
-    type_check: bool = False,
-) -> bool:
-    if is_builtin(obj):
-        return False
+__all__ = [
+    "callable_params",
+    "callable_signature",
+    "check_callable_signature",
+    "signature_params",
+    "signature_type_check",
+]
 
-    standard: Signature = signature(class_.__call__)
 
-    standard_params: Dict[str, Any] = {
-        p.name: p.annotation
-        for p in standard.parameters.values()
-        if p.name not in ("self", "args", "kwargs")
-    }
-
-    sign: Signature
+def callable_signature(obj: Union[Type[Any], FunctionType]) -> Optional[Signature]:
+    sign: Optional[Signature] = None
 
     if isclass(obj) and hasattr(obj, "__call__"):
-        logger.trace(f"Object '{obj.__name__}' is a class and callable")
+        logger.trace(f"Object '{callable_name(obj)}' is a class and callable")
         sign = signature(obj.__call__)
     elif isfunction(obj):
-        logger.trace(f"Object '{obj.__name__}' is a function")
+        logger.trace(f"Object '{callable_name(obj)}' is a function")
         sign = signature(obj)
     else:
-        logger.trace(f"Object '{obj.__name__}' is neither class with __call__ nor function. skip")
-        return False
+        logger.trace(
+            f"Object '{callable_name(obj)}' is neither class with __call__ nor function. skip"
+        )
+
+    return sign
+
+
+def signature_params(
+    sign: Signature,
+    *,
+    ignore_names: Tuple = ("self", "args", "kwargs"),
+) -> Dict[str, Any]:
+    return {p.name: p.annotation for p in sign.parameters.values() if p.name not in ignore_names}
+
+
+def callable_params(obj: Callable) -> Dict[str, Any]:
+    sign: Optional[Signature]
+    if isfunction(obj):
+        sign = callable_signature(obj)
+    else:
+        sign = callable_signature(type(obj))
 
-    obj_params: Dict[str, Any] = {
-        p.name: p.annotation for p in sign.parameters.values() if p.name not in ("self", "kwargs")
-    }
+    if not sign:
+        raise ValueError(f"Object '{callable_name(obj)}' is not callable")
 
-    if obj_params.keys() != standard_params.keys():
-        logger.info(f"Object '{object.__name__}' has got bad param names")
+    return signature_params(sign)
+
+
+def signature_type_check(*, check: Signature, origin: Signature) -> bool:
+    logger.info("'type_check' option is not implemented yet")
+    return True
+
+
+def check_callable_signature(
+    obj: Type[Any],
+    class_: Type[Any],
+    *,
+    type_check: bool = False,
+) -> bool:
+    obj_sign: Optional[Signature] = callable_signature(obj)
+    if is_builtin(obj) or not obj_sign:
         return False
 
+    cls_sign: Signature = signature(class_.__call__)
+
+    obj_params: Dict[str, Any] = signature_params(obj_sign)
+    cls_params: Dict[str, Any] = signature_params(cls_sign)
+
+    if class_ is not Plugin:
+        if obj_params.keys() != cls_params.keys():
+            logger.trace(f"Object '{callable_name(obj)}' has got bad param names")
+            return False
+    else:
+        if not set(obj_params.keys()).intersection(set(cls_params.keys())):
+            logger.trace(
+                f"Object '{callable_name(obj)}' is not satisfy any of possible 'Plugin' signatures."
+            )
+            return False
+
     if type_check:
-        logger.warning(
-            "'type_check' option is not implemented yet"
-            "The thing is consider 'dict' and 'typing.Dict' types as the same types"
-        )
+        return signature_type_check(check=obj_sign, origin=cls_sign)
 
     return True
```

