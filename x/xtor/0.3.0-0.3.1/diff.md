# Comparing `tmp/xtor-0.3.0.tar.gz` & `tmp/xtor-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xtor-0.3.0.tar", max compression
+gzip compressed data, was "xtor-0.3.1.tar", max compression
```

## Comparing `xtor-0.3.0.tar` & `xtor-0.3.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1079 2023-06-30 12:29:01.033240 xtor-0.3.0/README.md
--rw-r--r--   0        0        0      685 2023-06-30 12:50:22.533886 xtor-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       67 2023-06-30 12:50:16.105940 xtor-0.3.0/xtor/__init__.py
--rw-r--r--   0        0        0      807 2023-06-30 12:47:55.419073 xtor-0.3.0/xtor/cli.py
--rw-r--r--   0        0        0     5090 2023-06-30 12:25:53.430569 xtor-0.3.0/xtor/tor.py
--rw-r--r--   0        0        0     1844 2023-06-28 16:26:22.537395 xtor-0.3.0/xtor/utils.py
--rw-r--r--   0        0        0     1997 1970-01-01 00:00:00.000000 xtor-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1216 2023-07-01 22:45:48.270665 xtor-0.3.1/README.md
+-rw-r--r--   0        0        0      685 2023-07-01 22:45:10.749672 xtor-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0       67 2023-07-01 22:45:07.066969 xtor-0.3.1/xtor/__init__.py
+-rw-r--r--   0        0        0      807 2023-06-30 12:47:55.419073 xtor-0.3.1/xtor/cli.py
+-rw-r--r--   0        0        0     5380 2023-07-01 22:44:59.450642 xtor-0.3.1/xtor/tor.py
+-rw-r--r--   0        0        0     1844 2023-06-28 16:26:22.537395 xtor-0.3.1/xtor/utils.py
+-rw-r--r--   0        0        0     2134 1970-01-01 00:00:00.000000 xtor-0.3.1/PKG-INFO
```

### Comparing `xtor-0.3.0/README.md` & `xtor-0.3.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -45,8 +45,16 @@
     host="127.0.0.1",
     password="passw0rd",
 )
 
 with tor:
   print(tor.ip)
   print(tor.client.get("https://api.ipify.org").text)
+  tor.new_identity(wait=True) # get a new identity and wait for it to be ready (new ip)
+  print(tor.ip)
+```
+
+## CLI
+
+```bash
+xtor --help
 ```
```

### Comparing `xtor-0.3.0/pyproject.toml` & `xtor-0.3.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xtor"
-version = "0.3.0"
+version = "0.3.1"
 description = "Manage Tor instances"
 authors = ["khalidelborai <elboraikhalid@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/khalidelborai/xtor"
 license = "GNU Version 3"
 keywords = [
     "tor",
```

### Comparing `xtor-0.3.0/xtor/cli.py` & `xtor-0.3.1/xtor/cli.py`

 * *Files identical despite different names*

### Comparing `xtor-0.3.0/xtor/tor.py` & `xtor-0.3.1/xtor/tor.py`

 * *Files 3% similar despite different names*

```diff
@@ -170,14 +170,26 @@
         Returns:
             str: instance IP
 
         """
         if not hasattr(self, "_ip"):
             self._ip = self.__getIP()
         return self._ip
+    
+    def new_identity(self, wait = False) -> None:
+        """
+        Get new identity
+        """
+        self.controller.signal("NEWNYM")
+        ip = self.__getIP()
+        if wait:
+            while ip == self.ip:
+                ip = self.__getIP()
+        self._ip = ip
+        
 
     def kill(self) -> None:
         """
         Kill Tor process
         """
         self.tor.kill()
```

### Comparing `xtor-0.3.0/xtor/utils.py` & `xtor-0.3.1/xtor/utils.py`

 * *Files identical despite different names*

### Comparing `xtor-0.3.0/PKG-INFO` & `xtor-0.3.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xtor
-Version: 0.3.0
+Version: 0.3.1
 Summary: Manage Tor instances
 Home-page: https://github.com/khalidelborai/xtor
 License: GNU Version 3
 Keywords: tor,torrc,torrc manager,tor manager,tor instance,proxy
 Author: khalidelborai
 Author-email: elboraikhalid@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -69,9 +69,17 @@
     host="127.0.0.1",
     password="passw0rd",
 )
 
 with tor:
   print(tor.ip)
   print(tor.client.get("https://api.ipify.org").text)
+  tor.new_identity(wait=True) # get a new identity and wait for it to be ready (new ip)
+  print(tor.ip)
+```
+
+## CLI
+
+```bash
+xtor --help
 ```
```

