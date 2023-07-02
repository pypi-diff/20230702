# Comparing `tmp/simplenetlink-0.6.1-py3-none-any.whl.zip` & `tmp/simplenetlink-0.6.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 10344 bytes, number of entries: 6
--rw-r--r--  2.0 unx    19437 b- defN 23-Jun-22 15:31 simplenetlink/__init__.py
--rwxr-xr-x  2.0 unx    11357 b- defN 23-Jun-22 15:33 simplenetlink-0.6.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     6444 b- defN 23-Jun-22 15:33 simplenetlink-0.6.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-22 15:33 simplenetlink-0.6.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Jun-22 15:33 simplenetlink-0.6.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      500 b- defN 23-Jun-22 15:33 simplenetlink-0.6.1.dist-info/RECORD
-6 files, 37844 bytes uncompressed, 9438 bytes compressed:  75.1%
+Zip file size: 10351 bytes, number of entries: 6
+-rw-r--r--  2.0 unx    19530 b- defN 23-Jul-02 20:49 simplenetlink/__init__.py
+-rwxr-xr-x  2.0 unx    11357 b- defN 23-Jul-02 20:50 simplenetlink-0.6.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6444 b- defN 23-Jul-02 20:50 simplenetlink-0.6.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-02 20:50 simplenetlink-0.6.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Jul-02 20:50 simplenetlink-0.6.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      500 b- defN 23-Jul-02 20:50 simplenetlink-0.6.2.dist-info/RECORD
+6 files, 37937 bytes uncompressed, 9445 bytes compressed:  75.1%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: simplenetlink/__init__.py
 Comment: 
 
-Filename: simplenetlink-0.6.1.dist-info/LICENSE
+Filename: simplenetlink-0.6.2.dist-info/LICENSE
 Comment: 
 
-Filename: simplenetlink-0.6.1.dist-info/METADATA
+Filename: simplenetlink-0.6.2.dist-info/METADATA
 Comment: 
 
-Filename: simplenetlink-0.6.1.dist-info/WHEEL
+Filename: simplenetlink-0.6.2.dist-info/WHEEL
 Comment: 
 
-Filename: simplenetlink-0.6.1.dist-info/top_level.txt
+Filename: simplenetlink-0.6.2.dist-info/top_level.txt
 Comment: 
 
-Filename: simplenetlink-0.6.1.dist-info/RECORD
+Filename: simplenetlink-0.6.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## simplenetlink/__init__.py

```diff
@@ -249,14 +249,15 @@
     def get_interface_mtu(self):
         for attr in self.ipr.link("get", index=idx)[0]['attrs']:
             if attr[0] == "IFLA_MTU":
                 return attr[1]
 
     def get_interface_ip(self, interface, **kwargs):
         namespace, idx = self.find_interface_in_all_namespaces(interface)
+        self.set_current_namespace(namespace)
         retval={
             'ipv4':[],
             'ipv6':[]
         }
 
         for entry in self.ipr.get_addr(index=idx):
 
@@ -275,14 +276,16 @@
 
     def get_interface_ipv6(self,interface):
         return self.get_interface_ip(interface)['ipv6']
 
     def ensure_interface_exists(self, interface, **kwargs):
         self.reset()
         namespace, idx = self.find_interface_in_all_namespaces(interface)
+        self.set_current_namespace(namespace)
+
         if idx:
             if kwargs.get("namespace") != namespace:
                 self._log.debug(
                     f'interface is in namespace {namespace} -> moving to {kwargs.get("namespace")}'
                 )
 
                 if kwargs.get("namespace"):
```

## Comparing `simplenetlink-0.6.1.dist-info/LICENSE` & `simplenetlink-0.6.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `simplenetlink-0.6.1.dist-info/METADATA` & `simplenetlink-0.6.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplenetlink
-Version: 0.6.1
+Version: 0.6.2
 Summary: Abstraction layer for for simplified usage of pyroute2
 Home-page: https://github.com/jinjamator/simplenetlink
 Author: Wilhelm Putz
 Author-email: wp@aci.guru
 License: ASL V2
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

