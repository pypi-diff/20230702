# Comparing `tmp/wpdetect-1.4.5.tar.gz` & `tmp/wpdetect-1.4.6.tar.gz`

## Comparing `wpdetect-1.4.5.tar` & `wpdetect-1.4.6.tar`

### file list

```diff
@@ -1,14 +1,22 @@
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 wpdetect-1.4.5/release-tag.sh
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 wpdetect-1.4.5/requirements.txt
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 wpdetect-1.4.5/sample_urls.txt
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 wpdetect-1.4.5/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 wpdetect-1.4.5/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 wpdetect-1.4.5/.vscode/settings.json
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 wpdetect-1.4.5/utils/bump_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wpdetect-1.4.5/wpdetect/__init__.py
--rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 wpdetect-1.4.5/wpdetect/__main__.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 wpdetect-1.4.5/.gitignore
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 wpdetect-1.4.5/LICENSE.txt
--rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 wpdetect-1.4.5/README.md
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 wpdetect-1.4.5/pyproject.toml
--rw-r--r--   0        0        0     3826 2020-02-02 00:00:00.000000 wpdetect-1.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 wpdetect-1.4.6/CHANGELOG.md
+-rw-r--r--   0        0        0     5224 2020-02-02 00:00:00.000000 wpdetect-1.4.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     4243 2020-02-02 00:00:00.000000 wpdetect-1.4.6/CONTRIBUTING.md
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 wpdetect-1.4.6/SECURITY.md
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 wpdetect-1.4.6/release-tag.sh
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 wpdetect-1.4.6/requirements.txt
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 wpdetect-1.4.6/sample_urls.txt
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 wpdetect-1.4.6/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 wpdetect-1.4.6/.github/ISSUE_TEMPLATE/custom.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 wpdetect-1.4.6/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 wpdetect-1.4.6/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 wpdetect-1.4.6/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 wpdetect-1.4.6/.vscode/settings.json
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 wpdetect-1.4.6/utils/bump_version.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 wpdetect-1.4.6/utils/generate_changelog.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wpdetect-1.4.6/wpdetect/__init__.py
+-rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 wpdetect-1.4.6/wpdetect/__main__.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 wpdetect-1.4.6/.gitignore
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 wpdetect-1.4.6/LICENSE.txt
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 wpdetect-1.4.6/README.md
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 wpdetect-1.4.6/pyproject.toml
+-rw-r--r--   0        0        0     3313 2020-02-02 00:00:00.000000 wpdetect-1.4.6/PKG-INFO
```

### Comparing `wpdetect-1.4.5/.github/workflows/pylint.yml` & `wpdetect-1.4.6/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.5/.github/workflows/pypi-publish.yml` & `wpdetect-1.4.6/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.5/utils/bump_version.py` & `wpdetect-1.4.6/utils/bump_version.py`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.5/wpdetect/__main__.py` & `wpdetect-1.4.6/wpdetect/__main__.py`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.5/.gitignore` & `wpdetect-1.4.6/.gitignore`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.5/LICENSE.txt` & `wpdetect-1.4.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.5/README.md` & `wpdetect-1.4.6/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # WP DETECT
 
+[![Pylint](https://github.com/IamLizu/wpdetect/actions/workflows/pylint.yml/badge.svg?event=push)](https://github.com/IamLizu/wpdetect/actions/workflows/pylint.yml)
+[![Upload Python Package](https://github.com/IamLizu/wpdetect/actions/workflows/pypi-publish.yml/badge.svg?event=release)](https://github.com/IamLizu/wpdetect/actions/workflows/pypi-publish.yml)
+
 A WordPress detection tool, detects if a website is running WordPress. wpdetect is a great tool when you just want to check WordPress' presence but do not want to scan the site for vulnerabilities or issues.
 
 ## Installation
 
 You can install wpdetect using pip,
 
 ```sh
@@ -47,52 +50,22 @@
 https://wordpress.org
 https://www.newyorker.com/
 http://www.techcrunch.com/
 ```
 
 Please note that, it is not always possible to detect the presence of WordPress, website admins can take extra measures to remove sign of WordPress.
 
-## Changelog
-
-#### What's new in version 1.4.4
-
--   Fixed [#22](https://github.com/IamLizu/wpdetect/issues/22)
--   Cleaned http protocol adding methods.
--   Added options in README
-
-#### What's new in version 1.4.3
-
--   Fixed [#20](https://github.com/IamLizu/wpdetect/issues/20)
-
-#### What's new in version 1.4.2
+## Code of Conduct
 
--   Fixed [#18](https://github.com/IamLizu/wpdetect/issues/18)
+Please see the [code of conduct](CODE_OF_CONDUCT.md).
 
-#### What's new in version 1.4.1
+## Security
 
--   Fixed [#10](https://github.com/IamLizu/wpdetect/issues/10)
--   Added `-h` in `click` help options
+Please see the [security policy](SECURITY.md).
 
-#### What's new in version 1.4.0
+## Contributing
 
--   Removed manual argument parsing.
--   Introduced [click](https://click.palletsprojects.com/en/8.1.x/) and parsing arguments with it.
--   Added a sample URL in the repo for ease of testing.
+Please see the [contributing guide](CONTRIBUTING.md).
 
-#### What's new in version 1.3.9
-
--   Minor bug fixes
--   Added workflow for linting on code push
--   Added workflow for publishing to PyPi on release
-
-#### What's new in version 1.3.8
-
--   Fixed [#8](https://github.com/IamLizu/wpdetect/issues/8)
-
-#### What's new in version 1.3.7
-
--   Migrated to Hatchling build system
--   Updated README
-
-#### What's new in version 1.3.6
+## Changelog
 
--   Fixed minor bugs
+Please see the [changelog](CHANGELOG.md).
```

### Comparing `wpdetect-1.4.5/pyproject.toml` & `wpdetect-1.4.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "wpdetect"
-version = "1.4.5"
+version = "1.4.6"
 dependencies = [
     "pyfiglet", "requests", "click", "toml"
 ]
 authors = [
   { name="S M Mahmudul Hasan", email="he@smmahmudulhasan.com" },
 ]
 description = "A WordPress detection tool, detects if a website is running WordPress"
```

