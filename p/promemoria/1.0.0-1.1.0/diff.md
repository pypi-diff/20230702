# Comparing `tmp/promemoria-1.0.0.tar.gz` & `tmp/promemoria-1.1.0.tar.gz`

## Comparing `promemoria-1.0.0.tar` & `promemoria-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 promemoria-1.0.0/.gitattributes
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 promemoria-1.0.0/Makefile
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 promemoria-1.0.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 promemoria-1.0.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 promemoria-1.0.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 promemoria-1.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     3448 2020-02-02 00:00:00.000000 promemoria-1.0.0/src/promemoria/__init__.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 promemoria-1.0.0/src/promemoria/__main__.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 promemoria-1.0.0/src/promemoria/exceptions.py
--rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 promemoria-1.0.0/src/promemoria/promemoria.py
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 promemoria-1.0.0/src/promemoria/utilities.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 promemoria-1.0.0/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 promemoria-1.0.0/LICENSE
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 promemoria-1.0.0/README.md
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 promemoria-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 promemoria-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 promemoria-1.1.0/.gitattributes
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 promemoria-1.1.0/Makefile
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 promemoria-1.1.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 promemoria-1.1.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 promemoria-1.1.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 promemoria-1.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 promemoria-1.1.0/src/promemoria/__init__.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 promemoria-1.1.0/src/promemoria/__main__.py
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 promemoria-1.1.0/src/promemoria/files.py
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 promemoria-1.1.0/src/promemoria/help.py
+-rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 promemoria-1.1.0/src/promemoria/reminders.py
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 promemoria-1.1.0/src/promemoria/utilities.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 promemoria-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 promemoria-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 promemoria-1.1.0/README.md
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 promemoria-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3432 2020-02-02 00:00:00.000000 promemoria-1.1.0/PKG-INFO
```

### Comparing `promemoria-1.0.0/.github/ISSUE_TEMPLATE/feature_request.md` & `promemoria-1.1.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `promemoria-1.0.0/.github/workflows/python-publish.yml` & `promemoria-1.1.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `promemoria-1.0.0/LICENSE` & `promemoria-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `promemoria-1.0.0/README.md` & `promemoria-1.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -24,100 +24,100 @@
 
 ```
 python3 -m pip install --upgrade promemoria
 ```
 
 ## Usage
 
-### Show the list of reminders
+**promemoria** features a small and simple-to-use set of commands.  
+These commands can be easily retrieved at any moment by issuing `promemoria help`[^1][^2][^3]
 
-By simply calling `promemoria`[^1] you'll have:
+[^1]: Shouldn't `promemoria` work, try `python3 -m promemoria`.
 
-[^1]: Shouldn't this work, you can call **promemoria** by `python3 -m promemoria`.
+[^2]: A color coded output will serve you better than this example.
+
+[^3]: Referring to version 1.1.0
 
 ```
 [promemoria]
 
-You have 1 reminder(s).
------------------------
+Available commands.
+-------------------
 
-◯ [1] New reminder !!
-      Empty reminder for test purposes.
-      Due: 2023-07-10
+promemoria Shows the list of active reminders
+    --all Shows every reminder.
 
-------------
-0 completed.
-```
+promemoria new Creates a new reminder
+    -t title, string.
+    -de description, string. 
+    -da date, string, ISO 8601 compliant.
+    -ti time, string.
+    -p priority, integer, [1-3].
 
-### Create a new reminder
+promemoria delete Deletes the specified reminder
+    -i index, integer.
 
-The command for creating a new reminder is the following:
+promemoria toggle Toggles the specified reminder
+    -i index, integer.
 
+promemoria clear Deletes every reminder
 ```
-promemoria new -t "TITLE" -de "DESCRIPTION" -da "DATE" -p PRIORITY
-```
 
-and an example would be:
+## Examples
+
+### Quickly check your reminders
 
 ```
-promemoria new -t "Christmas" -de "It's Christmas!" -da "2023-12-25" -p 3
+promemoria
 ```
 
-which would result in
+which results in:
 
 ```
 [promemoria]
 
-Reminder created succesfully!
+You have 1 reminder(s).
+-----------------------
 
-◯ Christmas !!!
-  It's Christmas!
-  Due: 2023-12-25
+◯ [1] Go get some groceries. !
+      2023-07-12 08:30
 ```
 
-### Delete every reminder
-
-By
+### Creating a reminder
 
 ```
-promemoria clear
+promemoria new -t "Christmas" -de "It's Christmas\!" -da "2023-12-25" -p 3
 ```
 
-you'll delete every reminder.
+which results in:
 
 ```
 [promemoria]
 
-Your reminders have been deleted.
-```
-
-### Delete a specific reminder
-
-By 
+Reminder created succesfully!
+-----------------------------
 
+◯ Christmas !!!
+  It's Christmas!
+  2023-12-25
 ```
-promemoria delete -i INDEX
-```
-
-you'll be able to delete the i-th reminder in your list.
 
-### Toggle a reminder
+### Toggling a reminder
 
-By 
-
-```
-promemoria toggle -i INDEX
 ```
+promemoria toggle -i 1
+````
 
-you'll be able to toggle the i-th reminder in your list.
+which results[^2][^4] in:
 
-By calling `promemoria toggle -i 1` on the *Christmas* reminder created before:
+[^4]: The mark changes and the title gets dimmed.
 
 ```
 [promemoria]
 
-● ̶C̶h̶r̶i̶s̶t̶m̶a̶s !!!
-  It's Christmas!
-  Due: 2023-12-25
-```
+You toggled a reminder.
+-----------------------
 
-the reminder gets toggled and its title gets striked.
+● Christmas !!!
+  It's Christmas!
+  2023-12-25
+```
```

### Comparing `promemoria-1.0.0/pyproject.toml` & `promemoria-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "promemoria"
-version = "1.0.0"
+version = "1.1.0"
 authors = [
   { name="Andrea Di Antonio", email="mail@diantonioandrea.com" },
 ]
 description = ""
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = ["colorama", "setuptools"]
```

### Comparing `promemoria-1.0.0/PKG-INFO` & `promemoria-1.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promemoria
-Version: 1.0.0
+Version: 1.1.0
 Project-URL: Homepage, https://github.com/diantonioandrea/promemoria
 Project-URL: Bug Tracker, https://github.com/diantonioandrea/promemoria/issues
 Author-email: Andrea Di Antonio <mail@diantonioandrea.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -39,100 +39,100 @@
 
 ```
 python3 -m pip install --upgrade promemoria
 ```
 
 ## Usage
 
-### Show the list of reminders
+**promemoria** features a small and simple-to-use set of commands.  
+These commands can be easily retrieved at any moment by issuing `promemoria help`[^1][^2][^3]
 
-By simply calling `promemoria`[^1] you'll have:
+[^1]: Shouldn't `promemoria` work, try `python3 -m promemoria`.
 
-[^1]: Shouldn't this work, you can call **promemoria** by `python3 -m promemoria`.
+[^2]: A color coded output will serve you better than this example.
+
+[^3]: Referring to version 1.1.0
 
 ```
 [promemoria]
 
-You have 1 reminder(s).
------------------------
+Available commands.
+-------------------
 
-◯ [1] New reminder !!
-      Empty reminder for test purposes.
-      Due: 2023-07-10
+promemoria Shows the list of active reminders
+    --all Shows every reminder.
 
-------------
-0 completed.
-```
+promemoria new Creates a new reminder
+    -t title, string.
+    -de description, string. 
+    -da date, string, ISO 8601 compliant.
+    -ti time, string.
+    -p priority, integer, [1-3].
 
-### Create a new reminder
+promemoria delete Deletes the specified reminder
+    -i index, integer.
 
-The command for creating a new reminder is the following:
+promemoria toggle Toggles the specified reminder
+    -i index, integer.
 
+promemoria clear Deletes every reminder
 ```
-promemoria new -t "TITLE" -de "DESCRIPTION" -da "DATE" -p PRIORITY
-```
 
-and an example would be:
+## Examples
+
+### Quickly check your reminders
 
 ```
-promemoria new -t "Christmas" -de "It's Christmas!" -da "2023-12-25" -p 3
+promemoria
 ```
 
-which would result in
+which results in:
 
 ```
 [promemoria]
 
-Reminder created succesfully!
+You have 1 reminder(s).
+-----------------------
 
-◯ Christmas !!!
-  It's Christmas!
-  Due: 2023-12-25
+◯ [1] Go get some groceries. !
+      2023-07-12 08:30
 ```
 
-### Delete every reminder
-
-By
+### Creating a reminder
 
 ```
-promemoria clear
+promemoria new -t "Christmas" -de "It's Christmas\!" -da "2023-12-25" -p 3
 ```
 
-you'll delete every reminder.
+which results in:
 
 ```
 [promemoria]
 
-Your reminders have been deleted.
-```
-
-### Delete a specific reminder
-
-By 
+Reminder created succesfully!
+-----------------------------
 
+◯ Christmas !!!
+  It's Christmas!
+  2023-12-25
 ```
-promemoria delete -i INDEX
-```
-
-you'll be able to delete the i-th reminder in your list.
 
-### Toggle a reminder
+### Toggling a reminder
 
-By 
-
-```
-promemoria toggle -i INDEX
 ```
+promemoria toggle -i 1
+````
 
-you'll be able to toggle the i-th reminder in your list.
+which results[^2][^4] in:
 
-By calling `promemoria toggle -i 1` on the *Christmas* reminder created before:
+[^4]: The mark changes and the title gets dimmed.
 
 ```
 [promemoria]
 
-● ̶C̶h̶r̶i̶s̶t̶m̶a̶s !!!
-  It's Christmas!
-  Due: 2023-12-25
-```
+You toggled a reminder.
+-----------------------
 
-the reminder gets toggled and its title gets striked.
+● Christmas !!!
+  It's Christmas!
+  2023-12-25
+```
```

