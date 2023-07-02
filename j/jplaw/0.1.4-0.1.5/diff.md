# Comparing `tmp/jplaw-0.1.4.tar.gz` & `tmp/jplaw-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jplaw-0.1.4.tar", last modified: Sat Jul  1 05:01:21 2023, max compression
+gzip compressed data, was "jplaw-0.1.5.tar", last modified: Sun Jul  2 05:30:02 2023, max compression
```

## Comparing `jplaw-0.1.4.tar` & `jplaw-0.1.5.tar`

### file list

```diff
@@ -1,36 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:01:21.388112 jplaw-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-01 05:01:08.000000 jplaw-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-01 05:01:21.388112 jplaw-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-01 05:01:08.000000 jplaw-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:01:21.384112 jplaw-0.1.4/jplaw/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-01 05:01:08.000000 jplaw-0.1.4/jplaw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10966 2023-07-01 05:01:08.000000 jplaw-0.1.4/jplaw/api_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)    13992 2023-07-01 05:01:08.000000 jplaw-0.1.4/jplaw/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)    13277 2023-07-01 05:01:08.000000 jplaw-0.1.4/jplaw/community.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-01 05:01:08.000000 jplaw-0.1.4/jplaw/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-07-01 05:01:08.000000 jplaw-0.1.4/jplaw/lemmy.py
--rw-r--r--   0 runner    (1001) docker     (123)    15339 2023-07-01 05:01:08.000000 jplaw-0.1.4/jplaw/post.py
--rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-07-01 05:01:08.000000 jplaw-0.1.4/jplaw/private_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-07-01 05:01:08.000000 jplaw-0.1.4/jplaw/requestor.py
--rw-r--r--   0 runner    (1001) docker     (123)    29866 2023-07-01 05:01:08.000000 jplaw-0.1.4/jplaw/site.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:01:21.388112 jplaw-0.1.4/jplaw/types/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-01 05:01:08.000000 jplaw-0.1.4/jplaw/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-01 05:01:08.000000 jplaw-0.1.4/jplaw/types/comment_sort_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-01 05:01:08.000000 jplaw-0.1.4/jplaw/types/http_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-01 05:01:08.000000 jplaw-0.1.4/jplaw/types/listing_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-01 05:01:08.000000 jplaw-0.1.4/jplaw/types/modlog_action_type.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-01 05:01:08.000000 jplaw-0.1.4/jplaw/types/post_feature_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-01 05:01:08.000000 jplaw-0.1.4/jplaw/types/registration_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-01 05:01:08.000000 jplaw-0.1.4/jplaw/types/search_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-01 05:01:08.000000 jplaw-0.1.4/jplaw/types/sort_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-01 05:01:08.000000 jplaw-0.1.4/jplaw/types/subscribed_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    21163 2023-07-01 05:01:08.000000 jplaw-0.1.4/jplaw/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:01:21.384112 jplaw-0.1.4/jplaw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-01 05:01:21.000000 jplaw-0.1.4/jplaw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-01 05:01:21.000000 jplaw-0.1.4/jplaw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 05:01:21.000000 jplaw-0.1.4/jplaw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-01 05:01:21.000000 jplaw-0.1.4/jplaw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-01 05:01:21.000000 jplaw-0.1.4/jplaw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-01 05:01:08.000000 jplaw-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 05:01:21.388112 jplaw-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-01 05:01:08.000000 jplaw-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:30:02.050643 jplaw-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-02 05:29:48.000000 jplaw-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-07-02 05:30:02.050643 jplaw-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-07-02 05:29:48.000000 jplaw-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:30:02.046643 jplaw-0.1.5/jplaw/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-02 05:29:48.000000 jplaw-0.1.5/jplaw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10966 2023-07-02 05:29:48.000000 jplaw-0.1.5/jplaw/api_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13992 2023-07-02 05:29:48.000000 jplaw-0.1.5/jplaw/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13296 2023-07-02 05:29:48.000000 jplaw-0.1.5/jplaw/community.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-02 05:29:48.000000 jplaw-0.1.5/jplaw/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-07-02 05:29:48.000000 jplaw-0.1.5/jplaw/lemmy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15339 2023-07-02 05:29:48.000000 jplaw-0.1.5/jplaw/post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-07-02 05:29:48.000000 jplaw-0.1.5/jplaw/private_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-07-02 05:29:48.000000 jplaw-0.1.5/jplaw/requestor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29866 2023-07-02 05:29:48.000000 jplaw-0.1.5/jplaw/site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:30:02.050643 jplaw-0.1.5/jplaw/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-02 05:29:48.000000 jplaw-0.1.5/jplaw/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-02 05:29:48.000000 jplaw-0.1.5/jplaw/types/comment_sort_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-02 05:29:48.000000 jplaw-0.1.5/jplaw/types/http_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-02 05:29:48.000000 jplaw-0.1.5/jplaw/types/listing_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-02 05:29:48.000000 jplaw-0.1.5/jplaw/types/modlog_action_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-02 05:29:48.000000 jplaw-0.1.5/jplaw/types/post_feature_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-02 05:29:48.000000 jplaw-0.1.5/jplaw/types/registration_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-02 05:29:48.000000 jplaw-0.1.5/jplaw/types/search_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-02 05:29:48.000000 jplaw-0.1.5/jplaw/types/sort_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-02 05:29:48.000000 jplaw-0.1.5/jplaw/types/subscribed_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21163 2023-07-02 05:29:48.000000 jplaw-0.1.5/jplaw/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:30:02.046643 jplaw-0.1.5/jplaw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-07-02 05:30:02.000000 jplaw-0.1.5/jplaw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-02 05:30:02.000000 jplaw-0.1.5/jplaw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 05:30:02.000000 jplaw-0.1.5/jplaw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-02 05:30:02.000000 jplaw-0.1.5/jplaw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-02 05:29:48.000000 jplaw-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 05:30:02.050643 jplaw-0.1.5/setup.cfg
```

### Comparing `jplaw-0.1.4/LICENSE` & `jplaw-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jplaw-0.1.4/PKG-INFO` & `jplaw-0.1.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: jplaw
-Version: 0.1.4
+Version: 0.1.5
 Summary: A python wrapper for the lemmy HTTP API. Forked from plaw by Benjamin Jablonski (benja810)
-Author: Amar Persaud
 Author-email: Amar Persaud <tehspartaa@gmail.com>
 Project-URL: Homepage, https://github.com/amarpersaud/python-jplaw
 Project-URL: Bug Tracker, https://github.com/amarpersaud/python-jplaw/issues
-Keywords: lemmy plaw api jplaw
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Python Lemmy API Wrapper
-[![Build](https://github.com/amarpersaud/python-jplaw/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/amarpersaud/python-jplaw/actions/workflows/python-package.yml)   [![PYPI Package](https://github.com/amarpersaud/python-jplaw/actions/workflows/python-publish.yml/badge.svg?branch=main)](https://github.com/amarpersaud/python-jplaw/actions/workflows/python-publish.yml)
+[![Build](https://github.com/amarpersaud/python-jplaw/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/amarpersaud/python-jplaw/actions/workflows/python-package.yml) 
 [![Generate Python Documentation](https://github.com/amarpersaud/python-jplaw/actions/workflows/python-documentation.yml/badge.svg)](https://github.com/amarpersaud/python-jplaw/actions/workflows/python-documentation.yml)
 
 Like PRAW but for Lemmy
 
 Written using the [Lemmy TS library](https://github.com/LemmyNet/lemmy-js-client) for reference.
 
 Forked from benja810's plaw
@@ -53,7 +51,43 @@
 
 #Print the JSON response from getting a specific community
 print(lem.Community.get("test@lemmy.ml"))
 ```
 
 # Documentation
 See [the documentation](https://amarpersaud.github.io/python-jplaw/) for more information on how to use jplaw.
+
+# Roadmap 
+### v0.1.7
+- Work on return types and usability.
+
+### v0.1.6
+- Work on testing functions and finding / squashing bugs
+
+# Changelog
+### v0.1.5
+- Fix namespace issues
+- Fix build issues
+- Fix missing instance argument in list communities
+
+### v0.1.4
+- Created documentation
+    - Versioned documentation for browsing info on previous versions (things will prob change pretty quickly in early releases)
+    - Available [here](https://amarpersaud.github.io/python-jplaw/)
+- Fixed some issues with argument types not using enums properly or missing references
+- Created Emoji class for creating, editing and deleting custom emoji
+
+### v0.1.3
+- Moved enums like SortType to submodule jplaw.types
+- Fix missing enum types
+- Rename a large portion of the functions to remove repetition.
+    - Decouples naming scheme from Lemmy API
+    - Shortens names and removes repetitive naming like "Lemmy.Comment.likeComment()" -> "Lemmy.Comment.like()."
+
+### v0.1.2
+- Added majority of the API functions except for image uploading
+
+### v0.1.1
+- Getting PyPi package working and added some functions
+
+### v0.1
+- Alpha release. After forking from plaw, fork was broken and migrated to this repository from the [jplaw](https://github.com/amarpersaud/jplaw/) repository, as I wanted to do something a little different from having a purely API equivalent library.
```

### Comparing `jplaw-0.1.4/jplaw/api_paths.py` & `jplaw-0.1.5/jplaw/api_paths.py`

 * *Files identical despite different names*

### Comparing `jplaw-0.1.4/jplaw/comment.py` & `jplaw-0.1.5/jplaw/comment.py`

 * *Files identical despite different names*

### Comparing `jplaw-0.1.4/jplaw/community.py` & `jplaw-0.1.5/jplaw/community.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         """
         form = {
             "name": name
         }
         res = self._req.lemmyRequest("getCommunity", instance=instance, form=form, auth=auth, auth_token=auth_token)
         return res["community_view"]
         
-    def list(self, type: ListingType=None, sort:SortType=None, page:int=None, limit:int=None, auth:bool=True, auth_token:str=None): 
+    def list(self, type: ListingType=None, sort:SortType=None, page:int=None, limit:int=None, instance:str=None, auth:bool=True, auth_token:str=None): 
         """
         Get a list of communities (federated or local)
         
         Args:
             type (ListingType): Type of community (all or local). Optional
             sort (SortType): Sorting Mode. Optional
             page (int): Page number. Optional
```

### Comparing `jplaw-0.1.4/jplaw/emoji.py` & `jplaw-0.1.5/jplaw/emoji.py`

 * *Files identical despite different names*

### Comparing `jplaw-0.1.4/jplaw/lemmy.py` & `jplaw-0.1.5/jplaw/lemmy.py`

 * *Files identical despite different names*

### Comparing `jplaw-0.1.4/jplaw/post.py` & `jplaw-0.1.5/jplaw/post.py`

 * *Files identical despite different names*

### Comparing `jplaw-0.1.4/jplaw/private_message.py` & `jplaw-0.1.5/jplaw/private_message.py`

 * *Files identical despite different names*

### Comparing `jplaw-0.1.4/jplaw/requestor.py` & `jplaw-0.1.5/jplaw/requestor.py`

 * *Files identical despite different names*

### Comparing `jplaw-0.1.4/jplaw/site.py` & `jplaw-0.1.5/jplaw/site.py`

 * *Files identical despite different names*

### Comparing `jplaw-0.1.4/jplaw/types/modlog_action_type.py` & `jplaw-0.1.5/jplaw/types/modlog_action_type.py`

 * *Files identical despite different names*

### Comparing `jplaw-0.1.4/jplaw/user.py` & `jplaw-0.1.5/jplaw/user.py`

 * *Files identical despite different names*

### Comparing `jplaw-0.1.4/jplaw.egg-info/PKG-INFO` & `jplaw-0.1.5/jplaw.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: jplaw
-Version: 0.1.4
+Version: 0.1.5
 Summary: A python wrapper for the lemmy HTTP API. Forked from plaw by Benjamin Jablonski (benja810)
-Author: Amar Persaud
 Author-email: Amar Persaud <tehspartaa@gmail.com>
 Project-URL: Homepage, https://github.com/amarpersaud/python-jplaw
 Project-URL: Bug Tracker, https://github.com/amarpersaud/python-jplaw/issues
-Keywords: lemmy plaw api jplaw
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Python Lemmy API Wrapper
-[![Build](https://github.com/amarpersaud/python-jplaw/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/amarpersaud/python-jplaw/actions/workflows/python-package.yml)   [![PYPI Package](https://github.com/amarpersaud/python-jplaw/actions/workflows/python-publish.yml/badge.svg?branch=main)](https://github.com/amarpersaud/python-jplaw/actions/workflows/python-publish.yml)
+[![Build](https://github.com/amarpersaud/python-jplaw/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/amarpersaud/python-jplaw/actions/workflows/python-package.yml) 
 [![Generate Python Documentation](https://github.com/amarpersaud/python-jplaw/actions/workflows/python-documentation.yml/badge.svg)](https://github.com/amarpersaud/python-jplaw/actions/workflows/python-documentation.yml)
 
 Like PRAW but for Lemmy
 
 Written using the [Lemmy TS library](https://github.com/LemmyNet/lemmy-js-client) for reference.
 
 Forked from benja810's plaw
@@ -53,7 +51,43 @@
 
 #Print the JSON response from getting a specific community
 print(lem.Community.get("test@lemmy.ml"))
 ```
 
 # Documentation
 See [the documentation](https://amarpersaud.github.io/python-jplaw/) for more information on how to use jplaw.
+
+# Roadmap 
+### v0.1.7
+- Work on return types and usability.
+
+### v0.1.6
+- Work on testing functions and finding / squashing bugs
+
+# Changelog
+### v0.1.5
+- Fix namespace issues
+- Fix build issues
+- Fix missing instance argument in list communities
+
+### v0.1.4
+- Created documentation
+    - Versioned documentation for browsing info on previous versions (things will prob change pretty quickly in early releases)
+    - Available [here](https://amarpersaud.github.io/python-jplaw/)
+- Fixed some issues with argument types not using enums properly or missing references
+- Created Emoji class for creating, editing and deleting custom emoji
+
+### v0.1.3
+- Moved enums like SortType to submodule jplaw.types
+- Fix missing enum types
+- Rename a large portion of the functions to remove repetition.
+    - Decouples naming scheme from Lemmy API
+    - Shortens names and removes repetitive naming like "Lemmy.Comment.likeComment()" -> "Lemmy.Comment.like()."
+
+### v0.1.2
+- Added majority of the API functions except for image uploading
+
+### v0.1.1
+- Getting PyPi package working and added some functions
+
+### v0.1
+- Alpha release. After forking from plaw, fork was broken and migrated to this repository from the [jplaw](https://github.com/amarpersaud/jplaw/) repository, as I wanted to do something a little different from having a purely API equivalent library.
```

### Comparing `jplaw-0.1.4/jplaw.egg-info/SOURCES.txt` & `jplaw-0.1.5/jplaw.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 LICENSE
 README.md
 pyproject.toml
-setup.py
 jplaw/__init__.py
 jplaw/api_paths.py
 jplaw/comment.py
 jplaw/community.py
 jplaw/emoji.py
 jplaw/lemmy.py
 jplaw/post.py
 jplaw/private_message.py
 jplaw/requestor.py
 jplaw/site.py
 jplaw/user.py
 jplaw.egg-info/PKG-INFO
 jplaw.egg-info/SOURCES.txt
 jplaw.egg-info/dependency_links.txt
-jplaw.egg-info/requires.txt
 jplaw.egg-info/top_level.txt
 jplaw/types/__init__.py
 jplaw/types/comment_sort_type.py
 jplaw/types/http_type.py
 jplaw/types/listing_type.py
 jplaw/types/modlog_action_type.py
 jplaw/types/post_feature_type.py
```

### Comparing `jplaw-0.1.4/pyproject.toml` & `jplaw-0.1.5/pyproject.toml`

 * *Files identical despite different names*

