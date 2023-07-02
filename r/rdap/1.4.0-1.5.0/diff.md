# Comparing `tmp/rdap-1.4.0.tar.gz` & `tmp/rdap-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdap-1.4.0.tar", max compression
+gzip compressed data, was "rdap-1.5.0.tar", max compression
```

## Comparing `rdap-1.4.0.tar` & `rdap-1.5.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11358 2020-10-30 16:40:23.636777 rdap-1.4.0/LICENSE
--rw-r--r--   0        0        0     3025 2023-06-30 22:46:20.453257 rdap-1.4.0/README.md
--rw-r--r--   0        0        0     1381 2023-06-30 22:51:13.194666 rdap-1.4.0/pyproject.toml
--rw-r--r--   0        0        0      309 2021-01-13 02:09:22.693448 rdap-1.4.0/rdap/__init__.py
--rw-r--r--   0        0        0     3978 2023-06-30 22:24:27.233315 rdap-1.4.0/rdap/assignment.py
--rw-r--r--   0        0        0     1872 2021-01-13 18:02:14.687255 rdap-1.4.0/rdap/bootstrap.py
--rw-r--r--   0        0        0     2250 2022-09-23 17:55:38.098616 rdap-1.4.0/rdap/cli.py
--rw-r--r--   0        0        0    10225 2023-06-30 22:46:20.449257 rdap-1.4.0/rdap/client.py
--rw-r--r--   0        0        0      746 2021-01-13 18:02:14.688254 rdap-1.4.0/rdap/config.py
--rw-r--r--   0        0        0      237 2020-10-30 16:40:23.637777 rdap-1.4.0/rdap/exceptions.py
--rw-r--r--   0        0        0     5323 2023-06-30 22:46:20.449257 rdap-1.4.0/rdap/objects.py
--rw-r--r--   0        0        0     3944 1970-01-01 00:00:00.000000 rdap-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2020-10-30 16:40:23.636777 rdap-1.5.0/LICENSE
+-rw-r--r--   0        0        0     3020 2023-07-02 16:43:38.068929 rdap-1.5.0/README.md
+-rw-r--r--   0        0        0     1381 2023-07-02 16:44:09.566339 rdap-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0      309 2021-01-13 02:09:22.693448 rdap-1.5.0/rdap/__init__.py
+-rw-r--r--   0        0        0     3978 2023-07-02 16:43:38.069929 rdap-1.5.0/rdap/assignment.py
+-rw-r--r--   0        0        0     1872 2021-01-13 18:02:14.687255 rdap-1.5.0/rdap/bootstrap.py
+-rw-r--r--   0        0        0     2417 2023-07-02 16:43:38.069929 rdap-1.5.0/rdap/cli.py
+-rw-r--r--   0        0        0    10221 2023-07-02 16:43:38.069929 rdap-1.5.0/rdap/client.py
+-rw-r--r--   0        0        0      746 2021-01-13 18:02:14.688254 rdap-1.5.0/rdap/config.py
+-rw-r--r--   0        0        0      237 2020-10-30 16:40:23.637777 rdap-1.5.0/rdap/exceptions.py
+-rw-r--r--   0        0        0     6595 2023-07-02 16:43:38.069929 rdap-1.5.0/rdap/objects.py
+-rw-r--r--   0        0        0     3939 1970-01-01 00:00:00.000000 rdap-1.5.0/PKG-INFO
```

### Comparing `rdap-1.4.0/LICENSE` & `rdap-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rdap-1.4.0/README.md` & `rdap-1.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -15,35 +15,33 @@
 pip install rdap
 ```
 
 
 ## Usage
 
 ```
-usage: rdap [-h] [--debug] [--home HOME] [--verbose] [--quiet] [--version] [--output-format OUTPUT_FORMAT] [--show-requests] [--parse]
-            [--write-bootstrap-data]
-            query [query ...]
+usage: rdap [-h] [--debug] [--home HOME] [--verbose] [--quiet] [--version] [--output-format OUTPUT_FORMAT] [--show-requests] [--parse] [--rir] [--write-bootstrap-data] query [query ...]
 
 rdap
 
 positional arguments:
   query
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   --debug               enable extra debug output
-  --home HOME           specify the home directory, by default will check in order: $RDAP_HOME, ./.rdap, /home/$USER/.rdap,
-                        /home/$USER/.config/rdap
+  --home HOME           specify the home directory, by default will check in order: $RDAP_HOME, ./.rdap, /home/grizz/.rdap, /home/grizz/.config/rdap
   --verbose             enable more verbose output
   --quiet               no output at all
-  --version             show version number and exit
+  --version             show program's version number and exit
   --output-format OUTPUT_FORMAT
                         output format (yaml, json, text)
   --show-requests       show all requests
   --parse               parse data into object before display
+  --rir                 display rir
   --write-bootstrap-data
                         write bootstrap data for type (as query)
 ```
 
 
 ## Config file
```

### Comparing `rdap-1.4.0/pyproject.toml` & `rdap-1.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rdap"
-version = "1.4.0"
+version = "1.5.0"
 description = "Registration Data Access Protocol tools"
 authors = ["20C <code@20c.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 
 repository = "https://github.com/20c/rdap"
```

### Comparing `rdap-1.4.0/rdap/assignment.py` & `rdap-1.5.0/rdap/assignment.py`

 * *Files identical despite different names*

### Comparing `rdap-1.4.0/rdap/bootstrap.py` & `rdap-1.5.0/rdap/bootstrap.py`

 * *Files identical despite different names*

### Comparing `rdap-1.4.0/rdap/cli.py` & `rdap-1.5.0/rdap/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     parser.add_argument("--output-format", help="output format (yaml, json, text)")
     parser.add_argument(
         "--show-requests", action="store_true", help="show all requests"
     )
     parser.add_argument(
         "--parse", action="store_true", help="parse data into object before display"
     )
+    parser.add_argument("--rir", action="store_true", help="display rir", default=False)
     parser.add_argument(
         "--write-bootstrap-data",
         action="store_true",
         help="write bootstrap data for type (as query)",
     )
 
     parser.add_argument("query", nargs="+")
@@ -71,14 +72,16 @@
         for each in argd["query"]:
             client.write_bootstrap_data(each)
         return 0
 
     codec = munge.get_codec(output_format)()
     for each in argd["query"]:
         obj = client.get(each)
+        if argd.get("rir", False):
+            print(f"rir: {obj.get_rir()}")
         if argd.get("parse", False):
             print(codec.dumps(obj.parsed()))
         else:
             print(codec.dumps(obj.data))
 
     if argd.get("show_requests", False):
         print("# Requests")
```

### Comparing `rdap-1.4.0/rdap/client.py` & `rdap-1.5.0/rdap/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         # use setter
         self._recurse_roles = None
         self.recurse_roles = set(
             config.get("recurse_roles", ["administrative", "technical"])
         )
 
         self._last_req = None
-        self._last_req_url = None
+        self.last_req_url = None
         self._history = []
         self._asn_tree = None
         self.timeout = config.get("timeout")
 
         self.http = requests.Session()
         self.http.auth = RdapRequestAuth(
             **dict(
@@ -279,15 +279,15 @@
         if not base_url:
             base_url = self.url
 
         # FIXME - url join
         url = f"{base_url}{query}"
         self._last_req = self._get(url)
         # split query off to get the base url for following entity lookups
-        self._last_req_url = self._last_req.url.rsplit(query, 1)[0]
+        self.last_req_url = self._last_req.url.rsplit(query, 1)[0]
         return self._last_req
 
     def get_asn(self, asn):
         """
         Get an ASN object.
         """
         asn = int(asn)
@@ -326,16 +326,16 @@
         """
         Get entity url for handle.
 
         This function must be able to handle doing recursive lookups to the current URL
         after a bootstrap redirect for registries that don't link 'self'
         """
 
-        if self._last_req_url:
-            url = self._last_req_url
+        if self.last_req_url:
+            url = self.last_req_url
 
         # last ditch effort to use bootstrap
         else:
             url = self.url
 
         url = f"{url}/entity/{handle}"
         return url
```

### Comparing `rdap-1.4.0/rdap/config.py` & `rdap-1.5.0/rdap/config.py`

 * *Files identical despite different names*

### Comparing `rdap-1.4.0/rdap/objects.py` & `rdap-1.5.0/rdap/objects.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,24 @@
 from rdap.exceptions import RdapHTTPError, RdapNotFoundError
 
 
+def rir_from_domain(domain):
+    """Gets the RIR from a URL or domain, if possible"""
+    try:
+        for rir in ["arin", "apnic", "afrinic", "lacnic", "ripe"]:
+            if rir in domain:
+                return rir
+
+        if "nic.br" in domain:
+            return "lacnic"
+
+    except Exception:
+        return None
+
+
 class RdapObject:
     """
     RDAP base object, allows for lazy parsing
     """
 
     def __init__(self, data, rdapc=None):
         self._rdapc = rdapc
@@ -122,26 +136,54 @@
                             raise
 
         # WORKAROUND APNIC keeps org info in remarks
         if "apnic" in self._data.get("port43", ""):
             try:
                 for rem in self._data["remarks"]:
                     if rem["title"] == "description":
-                        org_name = rem["description"][0]
+                        if org_name:
+                            org_name += ", "
+                        org_name += rem["description"][0]
+                        break
+            except KeyError:
+                pass
+
+        # RIPE keeps org info in remarks
+        elif "ripe" in self._data.get("port43", ""):
+            try:
+                for rem in self._data["remarks"]:
+                    if rem["description"]:
+                        if org_name:
+                            org_name += ", "
+                        org_name += rem["description"][0]
                         break
             except KeyError:
                 pass
 
         self._parsed = dict(
             name=name,
             emails=sorted(emails),
             org_name=org_name,
             org_address=org_address,
         )
 
+    def get_rir(self):
+        """Gets the RIR for the object, if possible"""
+        try:
+            if "port43" in self._data:
+                if rir := rir_from_domain(self._data.get("port43")):
+                    return rir
+
+            if self._rdapc and self._rdapc.last_req_url:
+                if rir := rir_from_domain(self._rdapc.last_req_url):
+                    return rir
+
+        except Exception:
+            return None
+
 
 class RdapAsn(RdapObject):
     """
     access interface for lazy parsing of RDAP looked up aut-num objects
     """
 
     def __init__(self, data, rdapc=None):
```

### Comparing `rdap-1.4.0/PKG-INFO` & `rdap-1.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdap
-Version: 1.4.0
+Version: 1.5.0
 Summary: Registration Data Access Protocol tools
 Home-page: https://github.com/20c/rdap
 License: Apache-2.0
 Author: 20C
 Author-email: code@20c.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -40,35 +40,33 @@
 pip install rdap
 ```
 
 
 ## Usage
 
 ```
-usage: rdap [-h] [--debug] [--home HOME] [--verbose] [--quiet] [--version] [--output-format OUTPUT_FORMAT] [--show-requests] [--parse]
-            [--write-bootstrap-data]
-            query [query ...]
+usage: rdap [-h] [--debug] [--home HOME] [--verbose] [--quiet] [--version] [--output-format OUTPUT_FORMAT] [--show-requests] [--parse] [--rir] [--write-bootstrap-data] query [query ...]
 
 rdap
 
 positional arguments:
   query
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   --debug               enable extra debug output
-  --home HOME           specify the home directory, by default will check in order: $RDAP_HOME, ./.rdap, /home/$USER/.rdap,
-                        /home/$USER/.config/rdap
+  --home HOME           specify the home directory, by default will check in order: $RDAP_HOME, ./.rdap, /home/grizz/.rdap, /home/grizz/.config/rdap
   --verbose             enable more verbose output
   --quiet               no output at all
-  --version             show version number and exit
+  --version             show program's version number and exit
   --output-format OUTPUT_FORMAT
                         output format (yaml, json, text)
   --show-requests       show all requests
   --parse               parse data into object before display
+  --rir                 display rir
   --write-bootstrap-data
                         write bootstrap data for type (as query)
 ```
 
 
 ## Config file
```

