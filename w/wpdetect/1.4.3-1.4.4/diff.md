# Comparing `tmp/wpdetect-1.4.3.tar.gz` & `tmp/wpdetect-1.4.4.tar.gz`

## Comparing `wpdetect-1.4.3.tar` & `wpdetect-1.4.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 wpdetect-1.4.3/requirements.txt
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 wpdetect-1.4.3/sample_urls.txt
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 wpdetect-1.4.3/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 wpdetect-1.4.3/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 wpdetect-1.4.3/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wpdetect-1.4.3/wpdetect/__init__.py
--rw-r--r--   0        0        0     5982 2020-02-02 00:00:00.000000 wpdetect-1.4.3/wpdetect/__main__.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 wpdetect-1.4.3/.gitignore
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 wpdetect-1.4.3/LICENSE.txt
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 wpdetect-1.4.3/README.md
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 wpdetect-1.4.3/pyproject.toml
--rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 wpdetect-1.4.3/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 wpdetect-1.4.4/requirements.txt
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 wpdetect-1.4.4/sample_urls.txt
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 wpdetect-1.4.4/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 wpdetect-1.4.4/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 wpdetect-1.4.4/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wpdetect-1.4.4/wpdetect/__init__.py
+-rw-r--r--   0        0        0     6981 2020-02-02 00:00:00.000000 wpdetect-1.4.4/wpdetect/__main__.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 wpdetect-1.4.4/.gitignore
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 wpdetect-1.4.4/LICENSE.txt
+-rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 wpdetect-1.4.4/README.md
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 wpdetect-1.4.4/pyproject.toml
+-rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 wpdetect-1.4.4/PKG-INFO
```

### Comparing `wpdetect-1.4.3/.github/workflows/pylint.yml` & `wpdetect-1.4.4/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.3/.github/workflows/pypi-publish.yml` & `wpdetect-1.4.4/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.3/wpdetect/__main__.py` & `wpdetect-1.4.4/wpdetect/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 '''
 name: wpdetect
 description: A simple script to detect if a website is running WordPress.
 '''
 
 import sys
 import urllib.request
-import requests
+from urllib.parse import urlparse
 import click
 from pyfiglet import figlet_format
 
 HEADER = "'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_9_3) AppleWebKit/537.75.14" + \
     " (KHTML, like Gecko) Version/7.0.3 Safari/7046A194A'"
-VERSION = "1.4.3"
+VERSION = "1.4.4"
 
 # Error messages
 ERROR_UNABLE_TO_OPEN_URL = "Couldn't open url," + \
     " please make sure to type a valid and publicly accessible url.\n"
 
 # List to store the found WordPress installations
 wp_domains = []
@@ -42,14 +42,20 @@
     """
 
     print_verbose(figlet_format('     wpdetect     '))
     print_verbose("=================== VERSION: " +
                   version + " ===================\n")
 
 
+def print_checking_message(url):
+    """Prints the message before checking the url."""
+
+    print_verbose("\nChecking: " + str(url))
+
+
 def wp_check(url):
     """Checks if the given url is a WordPress installation."""
 
     wp_signature = urllib.request.Request(url, headers={'User-Agent': HEADER})
 
     try:
         with urllib.request.urlopen(wp_signature) as _:
@@ -57,62 +63,76 @@
 
     except urllib.error.HTTPError:
         pass
 
     return False
 
 
-def check_protocol(url):
+def get_protocol(url):
+    """Returns the protocol of the url."""
+
+    parsed_url = urlparse(url)
+    return parsed_url.scheme if parsed_url.scheme else None
+
+
+def add_scheme_to_url(url, scheme):
+    """Adds the scheme to the url."""
+
+    parsed_url = urlparse(url)
+    updated_url = parsed_url._replace(scheme=scheme)
+
+    return updated_url.scheme + "://" + updated_url.netloc + updated_url.path
+
+
+def add_http(url):
     """Checks if the url has a protocol specified, if not, it adds HTTP."""
 
-    print_verbose("[!] No protocol specified.")
-    url = "http://" + url
-    print_verbose("[+] Going with HTTP.\n")
-    print_verbose("Checking: " + str(url))
+    print_verbose("[+] Going with HTTP.")
+    url = add_scheme_to_url(url, "http")
 
     return url
 
 
+def get_redirected_url(url):
+    """Returns the redirected url."""
+
+    opener = urllib.request.build_opener(urllib.request.HTTPRedirectHandler)
+    response = opener.open(url)
+    redirected_url = response.url
+
+    return redirected_url
+
+
 def check_redirect(url):
     """Checks if the url redirects to another url, if so, it follows the redirect."""
 
-    headers = {'User-Agent': 'Mozilla/5.0'}
-    response = requests.head(url, allow_redirects=True,
-                             headers=headers, timeout=5)
-    redirected_url = response.url
+    redirected_url = get_redirected_url(url)
 
     if url != redirected_url:
         print_verbose(f"[!] {url} redirected to {redirected_url}")
         # Recursively follow the redirect
+        print_checking_message(redirected_url)
+
         return check_redirect(redirected_url)
 
     return redirected_url
 
 
-def check_http(url):
-    """Instead of HTTPS, it tries to connect over HTTP."""
-
-    print_verbose("[!] Couldn't connect over HTTPS.")
-    print_verbose("[+] Trying with HTTP.\n")
-    url = "http://" + url[8:]
-    print_verbose("Checking: " + str(url))
-
-    return url
-
-
 def url_check(url):
     """
         Checks if the url is valid and publicly accessible.
         If so, it runs wp_check on it.
     """
 
-    print_verbose("\nChecking: " + str(url))
+    print_checking_message(url)
+
     try:
-        if url[:4] != "http":
-            url = check_protocol(url)
+        if get_protocol(url) is None:
+            print_verbose("[!] No protocol specified.")
+            url = add_http(url)
 
         url = check_redirect(url)
 
         wp_signatures = {
             1: url + "/wp-login.php",
             2: url + "/wp-content/",
             3: url + "/wp-admin/",
@@ -137,16 +157,17 @@
             break
 
     except urllib.error.HTTPError as error:
         if error.code == 403:
             print_verbose("Got 403! Website seems to be behind a WAF.")
 
     except urllib.error.URLError:
-        if url[:5] == "https":
-            url = check_http(url)
+        if get_protocol(url) == "https":
+            print_verbose("[!] Couldn't connect over HTTPS.")
+            url = add_http(url)
 
             try:
                 url_check(url)
             except urllib.error.URLError:
                 print_verbose(ERROR_UNABLE_TO_OPEN_URL)
         else:
             print_verbose(ERROR_UNABLE_TO_OPEN_URL)
@@ -178,35 +199,54 @@
     """Prints the found WordPress installations."""
 
     if cli_options['verbose'] is False:
         for wp_domain in wp_domains:
             print(wp_domain)
 
 
+def full_scan(url):
+    """Scans the HTTP & HTTPS of the website for WordPress."""
+
+    print_verbose("Full scan initiated.\n")
+
+    print_verbose("[1] Scanning HTTP...")
+    url = add_scheme_to_url(url, "http")
+    url_check(url)
+
+    print_verbose("\n[2] Scanning HTTPS...")
+    url = add_scheme_to_url(url, "https")
+    url_check(url)
+
+
 @click.command(context_settings={"help_option_names": ['-h', '--help']})
 @click.argument('url', required=False)
 @click.option('-f', '--file', type=click.Path(exists=True), help="File with list of URLs to check.")
 @click.option('-v', '--version', is_flag=True, help="Print version.")
 @click.option('-ss', '--show-signature', is_flag=True,
               help="Show by which signature WordPress is detected in a domain.")
 @click.option('-q', '--quiet', is_flag=True, help="Only print the detected domains.")
-def main(url, file, version, show_signature, quiet):
+@click.option('-sf', '--scan-full', is_flag=True,
+              help="Scan HTTP & HTTPS of the website for WordPress.")
+def main(*, url=None, file=None, version=None, show_signature=None, quiet=None, scan_full=None):
     """Detects if a website is running WordPress."""
 
     if quiet:
         cli_options['verbose'] = False
 
     if show_signature:
         cli_options['show_signature'] = True
 
     if version is False:
         print_logo(VERSION)
 
     if url:
-        url_check(url)
+        if scan_full:
+            full_scan(url)
+        else:
+            url_check(url)
 
     if file:
         handle_file(file)
 
     if version:
         print(f"Version: {VERSION}")
 
@@ -214,8 +254,8 @@
         click.echo(click.get_current_context().get_help())
 
     # print wp_domains if verbose is true
     print_domains()
 
 
 if __name__ == '__main__':
-    main(None, None, None, None, None)
+    main()
```

### Comparing `wpdetect-1.4.3/.gitignore` & `wpdetect-1.4.4/.gitignore`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.3/LICENSE.txt` & `wpdetect-1.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.3/README.md` & `wpdetect-1.4.4/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -10,14 +10,25 @@
 pip install wpdetect
 ```
 
 wpdetect requires Python 3 or above to run. If you have Python 2 installed too, make sure to use the right pip.
 
 ## Usage
 
+| Option                  | Description                                                                           |
+| ----------------------- | ------------------------------------------------------------------------------------- |
+| `url`                   | The URL to check. No need to pass the `url` flag, just pass the actual domain or url. |
+| `-f, --file`            | File with a list of URLs to check.                                                    |
+| `-v, --version`         | Print the version.                                                                    |
+| `-ss, --show-signature` | Show by which signature WordPress is detected in a domain.                            |
+| `-q, --quiet`           | Only print the detected domains.                                                      |
+| `-sf, --scan-full`      | Scan HTTP & HTTPS of the website for WordPress.                                       |
+
+Here's a few basic examples,
+
 ```sh
 wpdetect <website_url>
 ```
 
 Example
 
 ```sh
@@ -38,14 +49,20 @@
 http://www.techcrunch.com/
 ```
 
 Please note that, it is not always possible to detect the presence of WordPress, website admins can take extra measures to remove sign of WordPress.
 
 ## Changelog
 
+#### What's new in version 1.4.4
+
+-   Fixed [#22](https://github.com/IamLizu/wpdetect/issues/22)
+-   Cleaned http protocol adding methods.
+-   Added options in README
+
 #### What's new in version 1.4.3
 
 -   Fixed [#20](https://github.com/IamLizu/wpdetect/issues/20)
 
 #### What's new in version 1.4.2
 
 -   Fixed [#18](https://github.com/IamLizu/wpdetect/issues/18)
```

### Comparing `wpdetect-1.4.3/pyproject.toml` & `wpdetect-1.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "wpdetect"
-version = "1.4.3"
+version = "1.4.4"
 dependencies = [
     "pyfiglet", "requests", "click"
 ]
 authors = [
   { name="S M Mahmudul Hasan", email="he@smmahmudulhasan.com" },
 ]
 description = "A WordPress detection tool, detects if a website is running WordPress"
```

### Comparing `wpdetect-1.4.3/PKG-INFO` & `wpdetect-1.4.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wpdetect
-Version: 1.4.3
+Version: 1.4.4
 Summary: A WordPress detection tool, detects if a website is running WordPress
 Project-URL: Homepage, https://github.com/IamLizu/wpdetect
 Project-URL: Bug Tracker, https://github.com/IamLizu/wpdetect/issues
 Author-email: S M Mahmudul Hasan <he@smmahmudulhasan.com>
 License-File: LICENSE.txt
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -30,14 +30,25 @@
 pip install wpdetect
 ```
 
 wpdetect requires Python 3 or above to run. If you have Python 2 installed too, make sure to use the right pip.
 
 ## Usage
 
+| Option                  | Description                                                                           |
+| ----------------------- | ------------------------------------------------------------------------------------- |
+| `url`                   | The URL to check. No need to pass the `url` flag, just pass the actual domain or url. |
+| `-f, --file`            | File with a list of URLs to check.                                                    |
+| `-v, --version`         | Print the version.                                                                    |
+| `-ss, --show-signature` | Show by which signature WordPress is detected in a domain.                            |
+| `-q, --quiet`           | Only print the detected domains.                                                      |
+| `-sf, --scan-full`      | Scan HTTP & HTTPS of the website for WordPress.                                       |
+
+Here's a few basic examples,
+
 ```sh
 wpdetect <website_url>
 ```
 
 Example
 
 ```sh
@@ -58,14 +69,20 @@
 http://www.techcrunch.com/
 ```
 
 Please note that, it is not always possible to detect the presence of WordPress, website admins can take extra measures to remove sign of WordPress.
 
 ## Changelog
 
+#### What's new in version 1.4.4
+
+-   Fixed [#22](https://github.com/IamLizu/wpdetect/issues/22)
+-   Cleaned http protocol adding methods.
+-   Added options in README
+
 #### What's new in version 1.4.3
 
 -   Fixed [#20](https://github.com/IamLizu/wpdetect/issues/20)
 
 #### What's new in version 1.4.2
 
 -   Fixed [#18](https://github.com/IamLizu/wpdetect/issues/18)
```

