# Comparing `tmp/automation-utilities-1.3.3.tar.gz` & `tmp/automation-utilities-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation-utilities-1.3.3.tar", last modified: Tue Jun 27 20:35:23 2023, max compression
+gzip compressed data, was "automation-utilities-1.3.4.tar", last modified: Sun Jul  2 20:14:52 2023, max compression
```

## Comparing `automation-utilities-1.3.3.tar` & `automation-utilities-1.3.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 20:35:23.042883 automation-utilities-1.3.3/
-drwxrwxrwx   0        0        0        0 2023-06-27 20:35:23.040890 automation-utilities-1.3.3/Automation_Utilities.egg-info/
--rw-rw-rw-   0        0        0      134 2023-06-27 20:35:22.000000 automation-utilities-1.3.3/Automation_Utilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      562 2023-06-27 20:35:22.000000 automation-utilities-1.3.3/Automation_Utilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 20:35:22.000000 automation-utilities-1.3.3/Automation_Utilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-27 20:35:22.000000 automation-utilities-1.3.3/Automation_Utilities.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-27 20:35:22.000000 automation-utilities-1.3.3/Automation_Utilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      134 2023-06-27 20:35:23.041883 automation-utilities-1.3.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-27 20:35:23.035724 automation-utilities-1.3.3/automation_utilities/
--rw-rw-rw-   0        0        0     1237 2023-06-27 18:45:24.000000 automation-utilities-1.3.3/automation_utilities/Data.py
--rw-rw-rw-   0        0        0      590 2023-06-27 12:14:03.000000 automation-utilities-1.3.3/automation_utilities/Files.py
--rw-rw-rw-   0        0        0      143 2023-06-26 15:50:11.000000 automation-utilities-1.3.3/automation_utilities/Input.py
--rw-rw-rw-   0        0        0      835 2023-06-27 20:34:27.000000 automation-utilities-1.3.3/automation_utilities/PhoneNumbers.py
--rw-rw-rw-   0        0        0        0 2023-06-26 15:36:31.000000 automation-utilities-1.3.3/automation_utilities/__init__.py
--rw-rw-rw-   0        0        0       42 2023-06-27 20:35:23.042883 automation-utilities-1.3.3/setup.cfg
--rw-rw-rw-   0        0        0      262 2023-06-27 20:35:21.000000 automation-utilities-1.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 20:14:52.467036 automation-utilities-1.3.4/
+drwxrwxrwx   0        0        0        0 2023-07-02 20:14:52.464789 automation-utilities-1.3.4/Automation_Utilities.egg-info/
+-rw-rw-rw-   0        0        0      134 2023-07-02 20:14:52.000000 automation-utilities-1.3.4/Automation_Utilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      562 2023-07-02 20:14:52.000000 automation-utilities-1.3.4/Automation_Utilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 20:14:52.000000 automation-utilities-1.3.4/Automation_Utilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-02 20:14:52.000000 automation-utilities-1.3.4/Automation_Utilities.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-07-02 20:14:52.000000 automation-utilities-1.3.4/Automation_Utilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      134 2023-07-02 20:14:52.465800 automation-utilities-1.3.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-02 20:14:52.463278 automation-utilities-1.3.4/automation_utilities/
+-rw-rw-rw-   0        0        0     1237 2023-06-27 18:45:24.000000 automation-utilities-1.3.4/automation_utilities/Data.py
+-rw-rw-rw-   0        0        0      669 2023-07-02 12:40:51.000000 automation-utilities-1.3.4/automation_utilities/Files.py
+-rw-rw-rw-   0        0        0      147 2023-07-02 15:43:12.000000 automation-utilities-1.3.4/automation_utilities/Input.py
+-rw-rw-rw-   0        0        0      835 2023-06-27 20:34:27.000000 automation-utilities-1.3.4/automation_utilities/PhoneNumbers.py
+-rw-rw-rw-   0        0        0        0 2023-06-26 15:36:31.000000 automation-utilities-1.3.4/automation_utilities/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-07-02 20:14:52.467036 automation-utilities-1.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      262 2023-07-02 20:14:48.000000 automation-utilities-1.3.4/setup.py
```

### Comparing `automation-utilities-1.3.3/Automation_Utilities.egg-info/SOURCES.txt` & `automation-utilities-1.3.4/Automation_Utilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `automation-utilities-1.3.3/automation_utilities/Data.py` & `automation-utilities-1.3.4/automation_utilities/Data.py`

 * *Files identical despite different names*

### Comparing `automation-utilities-1.3.3/automation_utilities/Files.py` & `automation-utilities-1.3.4/automation_utilities/Files.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,17 +8,19 @@
     open(to, 'a').write(text)
     lock.release()
 
 
 def load(*file_names: str):
     lists = []
     for file_name in file_names:
-        lock.acquire()
-        lists.append(open(file_name, 'r').read().split('\n'))
-        lock.release()
+        try:
+            lists.append(open(file_name, 'r').read().split('\n'))
+        except FileNotFoundError:
+            open(file_name, 'w').write('')
+            lists.append([])
     return lists if len(lists) > 1 else lists[0]
 
 
 def delete(text: str, from_file: str):
     lock.acquire()
     new_text = open(from_file, 'r').read().replace(text, '')
     open(from_file, 'w').write(new_text)
```

### Comparing `automation-utilities-1.3.3/automation_utilities/PhoneNumbers.py` & `automation-utilities-1.3.4/automation_utilities/PhoneNumbers.py`

 * *Files identical despite different names*

