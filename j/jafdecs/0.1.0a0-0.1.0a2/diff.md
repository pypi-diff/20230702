# Comparing `tmp/jafdecs-0.1.0a0.tar.gz` & `tmp/jafdecs-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jafdecs-0.1.0a0.tar", last modified: Fri Jun 30 14:42:28 2023, max compression
+gzip compressed data, was "jafdecs-0.1.0a2.tar", last modified: Sun Jul  2 15:53:36 2023, max compression
```

## Comparing `jafdecs-0.1.0a0.tar` & `jafdecs-0.1.0a2.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxr-x   0 doug      (1000) doug      (1000)        0 2023-06-30 14:42:28.672471 jafdecs-0.1.0a0/
--rw-rw-r--   0 doug      (1000) doug      (1000)     1721 2023-06-30 14:42:28.676471 jafdecs-0.1.0a0/PKG-INFO
--rw-rw-r--   0 doug      (1000) doug      (1000)     1262 2023-06-30 14:40:46.000000 jafdecs-0.1.0a0/README.rst
--rw-rw-r--   0 doug      (1000) doug      (1000)       87 2023-06-29 14:49:37.000000 jafdecs-0.1.0a0/pyproject.toml
--rw-rw-r--   0 doug      (1000) doug      (1000)      618 2023-06-30 14:42:28.676471 jafdecs-0.1.0a0/setup.cfg
-drwxrwxr-x   0 doug      (1000) doug      (1000)        0 2023-06-30 14:42:28.672471 jafdecs-0.1.0a0/src/
-drwxrwxr-x   0 doug      (1000) doug      (1000)        0 2023-06-30 14:42:28.672471 jafdecs-0.1.0a0/src/jafdecs/
--rw-rw-r--   0 doug      (1000) doug      (1000)       24 2023-06-30 14:42:14.000000 jafdecs-0.1.0a0/src/jafdecs/__init__.py
--rw-rw-r--   0 doug      (1000) doug      (1000)     2390 2023-06-30 14:23:23.000000 jafdecs-0.1.0a0/src/jafdecs/worm.py
-drwxrwxr-x   0 doug      (1000) doug      (1000)        0 2023-06-30 14:42:28.672471 jafdecs-0.1.0a0/src/jafdecs.egg-info/
--rw-rw-r--   0 doug      (1000) doug      (1000)     1721 2023-06-30 14:42:28.000000 jafdecs-0.1.0a0/src/jafdecs.egg-info/PKG-INFO
--rw-rw-r--   0 doug      (1000) doug      (1000)      219 2023-06-30 14:42:28.000000 jafdecs-0.1.0a0/src/jafdecs.egg-info/SOURCES.txt
--rw-rw-r--   0 doug      (1000) doug      (1000)        1 2023-06-30 14:42:28.000000 jafdecs-0.1.0a0/src/jafdecs.egg-info/dependency_links.txt
--rw-rw-r--   0 doug      (1000) doug      (1000)        8 2023-06-30 14:42:28.000000 jafdecs-0.1.0a0/src/jafdecs.egg-info/top_level.txt
+drwxrwxr-x   0 doug      (1000) doug      (1000)        0 2023-07-02 15:53:36.775400 jafdecs-0.1.0a2/
+-rw-rw-r--   0 doug      (1000) doug      (1000)     5117 2023-07-02 15:53:36.775400 jafdecs-0.1.0a2/PKG-INFO
+-rw-rw-r--   0 doug      (1000) doug      (1000)     4658 2023-07-02 15:53:25.000000 jafdecs-0.1.0a2/README.rst
+-rw-rw-r--   0 doug      (1000) doug      (1000)       87 2023-06-29 14:49:37.000000 jafdecs-0.1.0a2/pyproject.toml
+-rw-rw-r--   0 doug      (1000) doug      (1000)      618 2023-07-02 15:53:36.775400 jafdecs-0.1.0a2/setup.cfg
+drwxrwxr-x   0 doug      (1000) doug      (1000)        0 2023-07-02 15:53:36.771401 jafdecs-0.1.0a2/src/
+drwxrwxr-x   0 doug      (1000) doug      (1000)        0 2023-07-02 15:53:36.771401 jafdecs-0.1.0a2/src/jafdecs/
+-rw-rw-r--   0 doug      (1000) doug      (1000)       25 2023-07-02 15:53:25.000000 jafdecs-0.1.0a2/src/jafdecs/__init__.py
+-rw-rw-r--   0 doug      (1000) doug      (1000)      398 2023-07-02 15:53:25.000000 jafdecs-0.1.0a2/src/jafdecs/initialize.py
+-rw-rw-r--   0 doug      (1000) doug      (1000)      144 2023-07-02 15:53:25.000000 jafdecs-0.1.0a2/src/jafdecs/utilities.py
+-rw-rw-r--   0 doug      (1000) doug      (1000)     2385 2023-07-02 15:53:25.000000 jafdecs-0.1.0a2/src/jafdecs/worm.py
+drwxrwxr-x   0 doug      (1000) doug      (1000)        0 2023-07-02 15:53:36.775400 jafdecs-0.1.0a2/src/jafdecs.egg-info/
+-rw-rw-r--   0 doug      (1000) doug      (1000)     5117 2023-07-02 15:53:36.000000 jafdecs-0.1.0a2/src/jafdecs.egg-info/PKG-INFO
+-rw-rw-r--   0 doug      (1000) doug      (1000)      270 2023-07-02 15:53:36.000000 jafdecs-0.1.0a2/src/jafdecs.egg-info/SOURCES.txt
+-rw-rw-r--   0 doug      (1000) doug      (1000)        1 2023-07-02 15:53:36.000000 jafdecs-0.1.0a2/src/jafdecs.egg-info/dependency_links.txt
+-rw-rw-r--   0 doug      (1000) doug      (1000)        8 2023-07-02 15:53:36.000000 jafdecs-0.1.0a2/src/jafdecs.egg-info/top_level.txt
```

### Comparing `jafdecs-0.1.0a0/setup.cfg` & `jafdecs-0.1.0a2/setup.cfg`

 * *Files identical despite different names*

### Comparing `jafdecs-0.1.0a0/src/jafdecs/worm.py` & `jafdecs-0.1.0a2/src/jafdecs/worm.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Decorators facilitating a 'Write Once Read Many' paradigm of evaluation of
 decorated items.
 """
 
 import functools
-from typing import Any, Type
+from typing import Any, Type, Optional
 
 
-def onproperties(cls: Type[Any] | None = None, *, prefix: str = '_'):
+def onproperties(cls: Optional[Type[Any]] = None, *, prefix: str = '_'):
     """Decorator for classes to compute a property once when it is first read
     and cache the value as private member to not be recomputed again.
     
     The example below will save a member variable named `_member` to an
     instance of `SampleClass` when it is first accessed. Follow-up accesses to
     `.member` will pull from `._member` (or `{prefix}member` if the prefix is 
     explicitly defined) and will avoid re-computing the property's method.
@@ -37,40 +37,38 @@
 
     if cls is None:
         # Called when decorator is called or arguments are passed to the decorator.
         # e.g. @worm.onproperties(prefix='__')
         #      @worm.onproperties()
         return functools.partial(onproperties, prefix=prefix)
     
-    @functools.wraps(cls)
-    def wrapper(*args, **kwargs):
-        return cls(*args, **kwargs)
+    @functools.wraps(cls, updated=[])
+    class DecoratedClass(cls):
+        pass
 
     def wrapped_getter(instance: cls, member: property, private_name: str):
         if not hasattr(instance, private_name):
             value = member.fget(self=instance)
             setattr(instance, private_name, value)
         
         else:
             value = getattr(instance, private_name)
 
         return value
 
     for name, member in vars(cls).items():
         # Skip over anything that is not annotated with @property
-        if not isinstance(member, property):
-            continue
+        if isinstance(member, property):
+            decorated_member = property(
+                fget=functools.partial(wrapped_getter, member=member, private_name=f'{prefix}{name}'),
+                fset=member.fset,
+                fdel=member.fdel,
+                doc=member.__doc__
+            )
 
-        if name.startswith('__') and name.endswith('__'):
-            continue
-
-        decorated_member = property(
-            fget=functools.partial(wrapped_getter, member=member, private_name=f'{prefix}{name}'),
-            fset=member.fset,
-            fdel=member.fdel,
-            doc=member.__doc__
-        )
-
-        # Overwrite the property to use the new method.
-        setattr(cls, name, decorated_member)
+            # Overwrite the property to use the new method.
+            setattr(DecoratedClass, name, decorated_member)
+        
+        else:
+            continue        
     
-    return wrapper
+    return DecoratedClass
```

