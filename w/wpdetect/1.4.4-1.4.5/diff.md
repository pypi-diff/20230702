# Comparing `tmp/wpdetect-1.4.4.tar.gz` & `tmp/wpdetect-1.4.5.tar.gz`

## Comparing `wpdetect-1.4.4.tar` & `wpdetect-1.4.5.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 wpdetect-1.4.4/requirements.txt
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 wpdetect-1.4.4/sample_urls.txt
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 wpdetect-1.4.4/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 wpdetect-1.4.4/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 wpdetect-1.4.4/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wpdetect-1.4.4/wpdetect/__init__.py
--rw-r--r--   0        0        0     6981 2020-02-02 00:00:00.000000 wpdetect-1.4.4/wpdetect/__main__.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 wpdetect-1.4.4/.gitignore
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 wpdetect-1.4.4/LICENSE.txt
--rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 wpdetect-1.4.4/README.md
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 wpdetect-1.4.4/pyproject.toml
--rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 wpdetect-1.4.4/PKG-INFO
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 wpdetect-1.4.5/release-tag.sh
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 wpdetect-1.4.5/requirements.txt
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 wpdetect-1.4.5/sample_urls.txt
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 wpdetect-1.4.5/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 wpdetect-1.4.5/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 wpdetect-1.4.5/.vscode/settings.json
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 wpdetect-1.4.5/utils/bump_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wpdetect-1.4.5/wpdetect/__init__.py
+-rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 wpdetect-1.4.5/wpdetect/__main__.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 wpdetect-1.4.5/.gitignore
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 wpdetect-1.4.5/LICENSE.txt
+-rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 wpdetect-1.4.5/README.md
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 wpdetect-1.4.5/pyproject.toml
+-rw-r--r--   0        0        0     3826 2020-02-02 00:00:00.000000 wpdetect-1.4.5/PKG-INFO
```

### Comparing `wpdetect-1.4.4/.github/workflows/pylint.yml` & `wpdetect-1.4.5/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.4/.github/workflows/pypi-publish.yml` & `wpdetect-1.4.5/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.4/wpdetect/__main__.py` & `wpdetect-1.4.5/wpdetect/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,50 @@
 '''
 name: wpdetect
 description: A simple script to detect if a website is running WordPress.
 '''
 
 import sys
+import os
 import urllib.request
 from urllib.parse import urlparse
+import toml
 import click
 from pyfiglet import figlet_format
 
 HEADER = "'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_9_3) AppleWebKit/537.75.14" + \
     " (KHTML, like Gecko) Version/7.0.3 Safari/7046A194A'"
-VERSION = "1.4.4"
 
 # Error messages
 ERROR_UNABLE_TO_OPEN_URL = "Couldn't open url," + \
     " please make sure to type a valid and publicly accessible url.\n"
 
 # List to store the found WordPress installations
 wp_domains = []
 
 
 # cli options store
 cli_options = {
     'verbose': True,  # default value
     'show_signature': False,  # default value
+    'scan_full': False,  # default value
 }
 
 
+def get_package_version():
+    """Returns the version of the package."""
+
+    file_path = os.path.join(os.path.dirname(__file__), '..', 'pyproject.toml')
+
+    with open(file_path, 'r', encoding="utf-8") as pyproject_toml_file:
+        config = toml.load(pyproject_toml_file)
+
+    return config['project']['version']
+
+
 def print_verbose(message):
     """Prints the message if verbose is true."""
 
     if cli_options['verbose']:
         print(message)
 
 
@@ -185,15 +198,19 @@
             print_verbose("Targets,\n")
 
             for domain in domains:
                 print_verbose(domain.strip())
 
             for domain in domains:
                 url = domain.strip()
-                url_check(url)
+
+                if cli_options['scan_full']:
+                    full_scan(url)
+                else:
+                    url_check(url)
 
     except FileNotFoundError:
         print("Please enter the file name correctly, file not found!\n")
 
 
 def print_domains():
     """Prints the found WordPress installations."""
@@ -202,15 +219,15 @@
         for wp_domain in wp_domains:
             print(wp_domain)
 
 
 def full_scan(url):
     """Scans the HTTP & HTTPS of the website for WordPress."""
 
-    print_verbose("Full scan initiated.\n")
+    print_verbose(f"\nFull scan initiated for {url}\n")
 
     print_verbose("[1] Scanning HTTP...")
     url = add_scheme_to_url(url, "http")
     url_check(url)
 
     print_verbose("\n[2] Scanning HTTPS...")
     url = add_scheme_to_url(url, "https")
@@ -231,28 +248,31 @@
 
     if quiet:
         cli_options['verbose'] = False
 
     if show_signature:
         cli_options['show_signature'] = True
 
+    if scan_full:
+        cli_options['scan_full'] = True
+
     if version is False:
-        print_logo(VERSION)
+        print_logo(get_package_version())
 
     if url:
         if scan_full:
             full_scan(url)
         else:
             url_check(url)
 
     if file:
         handle_file(file)
 
     if version:
-        print(f"Version: {VERSION}")
+        print(f"Version: {get_package_version()}")
 
     if len(sys.argv) == 1:
         click.echo(click.get_current_context().get_help())
 
     # print wp_domains if verbose is true
     print_domains()
```

### Comparing `wpdetect-1.4.4/.gitignore` & `wpdetect-1.4.5/.gitignore`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.4/LICENSE.txt` & `wpdetect-1.4.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.4/README.md` & `wpdetect-1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.4/pyproject.toml` & `wpdetect-1.4.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "wpdetect"
-version = "1.4.4"
+version = "1.4.5"
 dependencies = [
-    "pyfiglet", "requests", "click"
+    "pyfiglet", "requests", "click", "toml"
 ]
 authors = [
   { name="S M Mahmudul Hasan", email="he@smmahmudulhasan.com" },
 ]
 description = "A WordPress detection tool, detects if a website is running WordPress"
 readme = "README.md"
 requires-python = ">=3.4"
```

### Comparing `wpdetect-1.4.4/PKG-INFO` & `wpdetect-1.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wpdetect
-Version: 1.4.4
+Version: 1.4.5
 Summary: A WordPress detection tool, detects if a website is running WordPress
 Project-URL: Homepage, https://github.com/IamLizu/wpdetect
 Project-URL: Bug Tracker, https://github.com/IamLizu/wpdetect/issues
 Author-email: S M Mahmudul Hasan <he@smmahmudulhasan.com>
 License-File: LICENSE.txt
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -12,14 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Build Tools
 Requires-Python: >=3.4
 Requires-Dist: click
 Requires-Dist: pyfiglet
 Requires-Dist: requests
+Requires-Dist: toml
 Description-Content-Type: text/markdown
 
 # WP DETECT
 
 A WordPress detection tool, detects if a website is running WordPress. wpdetect is a great tool when you just want to check WordPress' presence but do not want to scan the site for vulnerabilities or issues.
 
 ## Installation
```

