# Comparing `tmp/Lin-CMS-0.4.8.tar.gz` & `tmp/Lin-CMS-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Lin-CMS-0.4.8.tar", last modified: Wed Mar 16 02:07:21 2022, max compression
+gzip compressed data, was "Lin-CMS-0.4.9.tar", last modified: Tue Jul 19 06:46:54 2022, max compression
```

## Comparing `Lin-CMS-0.4.8.tar` & `Lin-CMS-0.4.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 02:07:21.596647 Lin-CMS-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1061 2022-03-16 02:07:11.000000 Lin-CMS-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     6520 2022-03-16 02:07:21.596647 Lin-CMS-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5843 2022-03-16 02:07:11.000000 Lin-CMS-0.4.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-16 02:07:21.596647 Lin-CMS-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1252 2022-03-16 02:07:11.000000 Lin-CMS-0.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 02:07:21.592647 Lin-CMS-0.4.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 02:07:21.596647 Lin-CMS-0.4.8/src/Lin_CMS.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6520 2022-03-16 02:07:21.000000 Lin-CMS-0.4.8/src/Lin_CMS.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      592 2022-03-16 02:07:21.000000 Lin-CMS-0.4.8/src/Lin_CMS.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-16 02:07:21.000000 Lin-CMS-0.4.8/src/Lin_CMS.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-16 02:07:20.000000 Lin-CMS-0.4.8/src/Lin_CMS.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-03-16 02:07:21.000000 Lin-CMS-0.4.8/src/Lin_CMS.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-03-16 02:07:21.000000 Lin-CMS-0.4.8/src/Lin_CMS.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 02:07:21.596647 Lin-CMS-0.4.8/src/lin/
--rw-r--r--   0 runner    (1001) docker     (121)     1010 2022-03-16 02:07:11.000000 Lin-CMS-0.4.8/src/lin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11729 2022-03-16 02:07:11.000000 Lin-CMS-0.4.8/src/lin/apidoc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1465 2022-03-16 02:07:11.000000 Lin-CMS-0.4.8/src/lin/config.py
--rw-r--r--   0 runner    (1001) docker     (121)    16521 2022-03-16 02:07:11.000000 Lin-CMS-0.4.8/src/lin/db.py
--rw-r--r--   0 runner    (1001) docker     (121)     2066 2022-03-16 02:07:11.000000 Lin-CMS-0.4.8/src/lin/encoder.py
--rw-r--r--   0 runner    (1001) docker     (121)      284 2022-03-16 02:07:11.000000 Lin-CMS-0.4.8/src/lin/enums.py
--rw-r--r--   0 runner    (1001) docker     (121)     4747 2022-03-16 02:07:11.000000 Lin-CMS-0.4.8/src/lin/exception.py
--rw-r--r--   0 runner    (1001) docker     (121)     6520 2022-03-16 02:07:11.000000 Lin-CMS-0.4.8/src/lin/file.py
--rw-r--r--   0 runner    (1001) docker     (121)     1615 2022-03-16 02:07:11.000000 Lin-CMS-0.4.8/src/lin/form.py
--rw-r--r--   0 runner    (1001) docker     (121)     8245 2022-03-16 02:07:11.000000 Lin-CMS-0.4.8/src/lin/interface.py
--rw-r--r--   0 runner    (1001) docker     (121)     4404 2022-03-16 02:07:11.000000 Lin-CMS-0.4.8/src/lin/jwt.py
--rw-r--r--   0 runner    (1001) docker     (121)     6168 2022-03-16 02:07:11.000000 Lin-CMS-0.4.8/src/lin/lin.py
--rw-r--r--   0 runner    (1001) docker     (121)     2585 2022-03-16 02:07:11.000000 Lin-CMS-0.4.8/src/lin/loader.py
--rw-r--r--   0 runner    (1001) docker     (121)     5510 2022-03-16 02:07:11.000000 Lin-CMS-0.4.8/src/lin/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     8124 2022-03-16 02:07:11.000000 Lin-CMS-0.4.8/src/lin/manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     3675 2022-03-16 02:07:11.000000 Lin-CMS-0.4.8/src/lin/model.py
--rw-r--r--   0 runner    (1001) docker     (121)      982 2022-03-16 02:07:11.000000 Lin-CMS-0.4.8/src/lin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1040 2022-03-16 02:07:11.000000 Lin-CMS-0.4.8/src/lin/redprint.py
--rw-r--r--   0 runner    (1001) docker     (121)     5664 2022-03-16 02:07:11.000000 Lin-CMS-0.4.8/src/lin/syslogger.py
--rw-r--r--   0 runner    (1001) docker     (121)     3753 2022-03-16 02:07:11.000000 Lin-CMS-0.4.8/src/lin/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 06:46:54.305575 Lin-CMS-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1061 2022-07-19 06:46:40.000000 Lin-CMS-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     6518 2022-07-19 06:46:54.305575 Lin-CMS-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5843 2022-07-19 06:46:40.000000 Lin-CMS-0.4.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-19 06:46:54.305575 Lin-CMS-0.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1252 2022-07-19 06:46:40.000000 Lin-CMS-0.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 06:46:54.301575 Lin-CMS-0.4.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 06:46:54.301575 Lin-CMS-0.4.9/src/Lin_CMS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     6518 2022-07-19 06:46:54.000000 Lin-CMS-0.4.9/src/Lin_CMS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      592 2022-07-19 06:46:54.000000 Lin-CMS-0.4.9/src/Lin_CMS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-19 06:46:54.000000 Lin-CMS-0.4.9/src/Lin_CMS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-19 06:46:54.000000 Lin-CMS-0.4.9/src/Lin_CMS.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-07-19 06:46:54.000000 Lin-CMS-0.4.9/src/Lin_CMS.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        4 2022-07-19 06:46:54.000000 Lin-CMS-0.4.9/src/Lin_CMS.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 06:46:54.305575 Lin-CMS-0.4.9/src/lin/
+-rw-r--r--   0 runner    (1001) docker     (121)     1010 2022-07-19 06:46:40.000000 Lin-CMS-0.4.9/src/lin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11729 2022-07-19 06:46:40.000000 Lin-CMS-0.4.9/src/lin/apidoc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1465 2022-07-19 06:46:40.000000 Lin-CMS-0.4.9/src/lin/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16521 2022-07-19 06:46:40.000000 Lin-CMS-0.4.9/src/lin/db.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2066 2022-07-19 06:46:40.000000 Lin-CMS-0.4.9/src/lin/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2022-07-19 06:46:40.000000 Lin-CMS-0.4.9/src/lin/enums.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4747 2022-07-19 06:46:40.000000 Lin-CMS-0.4.9/src/lin/exception.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6520 2022-07-19 06:46:40.000000 Lin-CMS-0.4.9/src/lin/file.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1615 2022-07-19 06:46:40.000000 Lin-CMS-0.4.9/src/lin/form.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8372 2022-07-19 06:46:40.000000 Lin-CMS-0.4.9/src/lin/interface.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4404 2022-07-19 06:46:40.000000 Lin-CMS-0.4.9/src/lin/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6168 2022-07-19 06:46:40.000000 Lin-CMS-0.4.9/src/lin/lin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2585 2022-07-19 06:46:40.000000 Lin-CMS-0.4.9/src/lin/loader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5510 2022-07-19 06:46:40.000000 Lin-CMS-0.4.9/src/lin/logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8124 2022-07-19 06:46:40.000000 Lin-CMS-0.4.9/src/lin/manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4035 2022-07-19 06:46:40.000000 Lin-CMS-0.4.9/src/lin/model.py
+-rw-r--r--   0 runner    (1001) docker     (121)      982 2022-07-19 06:46:40.000000 Lin-CMS-0.4.9/src/lin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1040 2022-07-19 06:46:40.000000 Lin-CMS-0.4.9/src/lin/redprint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5664 2022-07-19 06:46:40.000000 Lin-CMS-0.4.9/src/lin/syslogger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3753 2022-07-19 06:46:40.000000 Lin-CMS-0.4.9/src/lin/utils.py
```

### Comparing `Lin-CMS-0.4.8/LICENSE` & `Lin-CMS-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Lin-CMS-0.4.8/PKG-INFO` & `Lin-CMS-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Lin-CMS
-Version: 0.4.8
+Version: 0.4.9
 Summary: A simple and practical CMS implememted by flask
 Home-page: https://pypi.org/project/Lin-CMS/
 Author: pedroGao
 Author-email: 1312342604@qq.com
 Maintainer: sunlin92
 Maintainer-email: sun.melodies@gmail.com
 License: MIT
@@ -131,9 +131,7 @@
 CMS 系统。当然，Lin 本身不限制开发者选用任何的组件库，你完全可以根据自己的喜好/
 习惯/熟悉度，去选择任意的一个基于 Vue 的组件库，比如前面提到的 Vue Element 和
 iView 等。你甚至可以混搭使用。当然，前提是这些组件库是基于 Vue 的。
 
 #### 完善的文档
 
 我们将提供详尽的文档来帮助开发者使用 Lin
-
-
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Lin-CMS Version: 0.4.8 Summary: A simple and
+Metadata-Version: 2.1 Name: Lin-CMS Version: 0.4.9 Summary: A simple and
 practical CMS implememted by flask Home-page: https://pypi.org/project/Lin-CMS/
 Author: pedroGao Author-email: 1312342604@qq.com Maintainer: sunlin92
 Maintainer-email: sun.melodies@gmail.com License: MIT Keywords:
 flask,CMS,authority,jwt,openapi Platform: any Classifier: Development Status ::
 3 - Alpha Classifier: Environment :: Web Environment Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
```

### Comparing `Lin-CMS-0.4.8/README.md` & `Lin-CMS-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `Lin-CMS-0.4.8/setup.py` & `Lin-CMS-0.4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import setuptools
 
 with io.open("README.md", "rt", encoding="utf8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="Lin-CMS",
-    version="0.4.8",
+    version="0.4.9",
     url="https://pypi.org/project/Lin-CMS/",
     license="MIT",
     author="pedroGao",
     author_email="1312342604@qq.com",
     maintainer="sunlin92",
     maintainer_email="sun.melodies@gmail.com",
     description="A simple and practical CMS implememted by flask",
```

### Comparing `Lin-CMS-0.4.8/src/Lin_CMS.egg-info/PKG-INFO` & `Lin-CMS-0.4.9/src/Lin_CMS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Lin-CMS
-Version: 0.4.8
+Version: 0.4.9
 Summary: A simple and practical CMS implememted by flask
 Home-page: https://pypi.org/project/Lin-CMS/
 Author: pedroGao
 Author-email: 1312342604@qq.com
 Maintainer: sunlin92
 Maintainer-email: sun.melodies@gmail.com
 License: MIT
@@ -131,9 +131,7 @@
 CMS 系统。当然，Lin 本身不限制开发者选用任何的组件库，你完全可以根据自己的喜好/
 习惯/熟悉度，去选择任意的一个基于 Vue 的组件库，比如前面提到的 Vue Element 和
 iView 等。你甚至可以混搭使用。当然，前提是这些组件库是基于 Vue 的。
 
 #### 完善的文档
 
 我们将提供详尽的文档来帮助开发者使用 Lin
-
-
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Lin-CMS Version: 0.4.8 Summary: A simple and
+Metadata-Version: 2.1 Name: Lin-CMS Version: 0.4.9 Summary: A simple and
 practical CMS implememted by flask Home-page: https://pypi.org/project/Lin-CMS/
 Author: pedroGao Author-email: 1312342604@qq.com Maintainer: sunlin92
 Maintainer-email: sun.melodies@gmail.com License: MIT Keywords:
 flask,CMS,authority,jwt,openapi Platform: any Classifier: Development Status ::
 3 - Alpha Classifier: Environment :: Web Environment Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
```

### Comparing `Lin-CMS-0.4.8/src/Lin_CMS.egg-info/SOURCES.txt` & `Lin-CMS-0.4.9/src/Lin_CMS.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Lin-CMS-0.4.8/src/lin/__init__.py` & `Lin-CMS-0.4.9/src/lin/__init__.py`

 * *Files identical despite different names*

### Comparing `Lin-CMS-0.4.8/src/lin/apidoc.py` & `Lin-CMS-0.4.9/src/lin/apidoc.py`

 * *Files identical despite different names*

### Comparing `Lin-CMS-0.4.8/src/lin/config.py` & `Lin-CMS-0.4.9/src/lin/config.py`

 * *Files identical despite different names*

### Comparing `Lin-CMS-0.4.8/src/lin/db.py` & `Lin-CMS-0.4.9/src/lin/db.py`

 * *Files identical despite different names*

### Comparing `Lin-CMS-0.4.8/src/lin/encoder.py` & `Lin-CMS-0.4.9/src/lin/encoder.py`

 * *Files identical despite different names*

### Comparing `Lin-CMS-0.4.8/src/lin/exception.py` & `Lin-CMS-0.4.9/src/lin/exception.py`

 * *Files identical despite different names*

### Comparing `Lin-CMS-0.4.8/src/lin/file.py` & `Lin-CMS-0.4.9/src/lin/file.py`

 * *Files identical despite different names*

### Comparing `Lin-CMS-0.4.8/src/lin/form.py` & `Lin-CMS-0.4.9/src/lin/form.py`

 * *Files identical despite different names*

### Comparing `Lin-CMS-0.4.8/src/lin/interface.py` & `Lin-CMS-0.4.9/src/lin/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,14 +190,20 @@
     __table_args__ = (Index("name_module", "name", "module", unique=True),)
 
     id = Column(Integer(), primary_key=True)
     name = Column(String(60), nullable=False, comment="权限名称，例如：访问首页")
     module = Column(String(50), nullable=False, comment="权限所属模块，例如：人员管理")
     mount = Column(Boolean, nullable=False, comment="是否为挂载权限")
 
+    def __hash__(self):
+        raise NotImplementedError()
+
+    def __eq__(self, other):
+        raise NotImplementedError()
+
 
 class UserInterface(InfoCrud):
     __tablename__ = "lin_user"
     __table_args__ = (
         Index("username_del", "username", "is_deleted", unique=True),
         Index("email_del", "email", "is_deleted", unique=True),
     )
```

### Comparing `Lin-CMS-0.4.8/src/lin/jwt.py` & `Lin-CMS-0.4.9/src/lin/jwt.py`

 * *Files identical despite different names*

### Comparing `Lin-CMS-0.4.8/src/lin/lin.py` & `Lin-CMS-0.4.9/src/lin/lin.py`

 * *Files identical despite different names*

### Comparing `Lin-CMS-0.4.8/src/lin/loader.py` & `Lin-CMS-0.4.9/src/lin/loader.py`

 * *Files identical despite different names*

### Comparing `Lin-CMS-0.4.8/src/lin/logger.py` & `Lin-CMS-0.4.9/src/lin/logger.py`

 * *Files identical despite different names*

### Comparing `Lin-CMS-0.4.8/src/lin/manager.py` & `Lin-CMS-0.4.9/src/lin/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,22 +138,22 @@
             return plugin.services.get(name)
 
     def sync_permissions(self):
         with db.auto_commit():
             db.create_all()
             permissions = self.permission_model.get(one=False)
             # 新增的权限记录
-            new_added_permissions = list()
+            new_added_permissions: set = set()
             deleted_ids = [permission.id for permission in permissions]
             # mount-> unmount
             unmounted_ids = list()
             # unmount-> mount 的记录
             mounted_ids = list()
             # 用代码中记录的权限比对数据库中的权限
-            for ep, meta in self.ep_meta.items():
+            for _, meta in self.ep_meta.items():
                 name, module, mount = meta
                 # db_existed 判定 代码中的权限是否存在于权限表记录中
                 db_existed = False
                 for permission in permissions:
                     if permission.name == name and permission.module == module:
                         # 此条记录存在,从待删除列表中移除,不会被删除
                         if permission.id in deleted_ids:
@@ -169,15 +169,15 @@
                         break
                 # 遍历结束，代码中的记录不存在于已有的权限表中，则将其添加到新增权限记录列表
                 if not db_existed:
                     permission = self.permission_model()
                     permission.name = name
                     permission.module = module
                     permission.mount = mount
-                    new_added_permissions.append(permission)
+                    new_added_permissions.add(permission)
             _sync_permissions(
                 self, new_added_permissions, unmounted_ids, mounted_ids, deleted_ids
             )
 
 
 def _sync_permissions(
     manager, new_added_permissions, unmounted_ids, mounted_ids, deleted_ids
```

### Comparing `Lin-CMS-0.4.8/src/lin/model.py` & `Lin-CMS-0.4.9/src/lin/model.py`

 * *Files 24% similar despite different names*

```diff
@@ -29,15 +29,24 @@
 
 
 class GroupPermission(GroupPermissionInterface):
     pass
 
 
 class Permission(PermissionInterface):
-    pass
+    def __hash__(self):
+        return hash(self.name + self.module)
+
+    def __eq__(self, other):
+        if self.name == other.name and self.module == other.module:
+            # 如果出现了复用同名权限，则要保证mount=True的权限生效
+            self.mount = self.mount or other.mount
+            return True
+        else:
+            return False
 
 
 class User(UserInterface):
     @property
     def avatar(self):
         site_domain = current_app.config.get(
             "SITE_DOMAIN",
```

### Comparing `Lin-CMS-0.4.8/src/lin/plugin.py` & `Lin-CMS-0.4.9/src/lin/plugin.py`

 * *Files identical despite different names*

### Comparing `Lin-CMS-0.4.8/src/lin/redprint.py` & `Lin-CMS-0.4.9/src/lin/redprint.py`

 * *Files identical despite different names*

### Comparing `Lin-CMS-0.4.8/src/lin/syslogger.py` & `Lin-CMS-0.4.9/src/lin/syslogger.py`

 * *Files identical despite different names*

### Comparing `Lin-CMS-0.4.8/src/lin/utils.py` & `Lin-CMS-0.4.9/src/lin/utils.py`

 * *Files identical despite different names*

