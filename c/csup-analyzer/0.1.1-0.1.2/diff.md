# Comparing `tmp/csup_analyzer-0.1.1.tar.gz` & `tmp/csup_analyzer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csup_analyzer-0.1.1.tar", last modified: Sun Jun 25 17:04:49 2023, max compression
+gzip compressed data, was "csup_analyzer-0.1.2.tar", last modified: Sun Jul  2 16:28:57 2023, max compression
```

## Comparing `csup_analyzer-0.1.1.tar` & `csup_analyzer-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1072 2023-06-22 17:30:13.797630 csup_analyzer-0.1.1/LICENSE
--rw-r--r--   0        0        0     3238 2023-06-25 14:15:51.741459 csup_analyzer-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-06-25 17:04:13.213877 csup_analyzer-0.1.1/csup_analyzer/__init__.py
--rw-r--r--   0        0        0     1776 2023-06-24 10:42:39.455239 csup_analyzer-0.1.1/csup_analyzer/event/Driver.py
--rw-r--r--   0        0        0     6195 2023-06-25 11:28:00.122788 csup_analyzer-0.1.1/csup_analyzer/event/Event.py
--rw-r--r--   0        0        0      438 2023-06-24 08:34:34.445951 csup_analyzer-0.1.1/csup_analyzer/event/LineUp.py
--rw-r--r--   0        0        0    10866 2023-06-25 16:48:37.404077 csup_analyzer-0.1.1/csup_analyzer/event/Result.py
--rw-r--r--   0        0        0        0 2023-06-25 13:43:11.091718 csup_analyzer-0.1.1/csup_analyzer/event/__init__.py
--rw-r--r--   0        0        0      161 2023-06-25 13:44:36.861708 csup_analyzer-0.1.1/csup_analyzer/plots/Plots.py
--rw-r--r--   0        0        0        0 2023-06-25 13:43:18.531717 csup_analyzer-0.1.1/csup_analyzer/plots/__init__.py
--rw-r--r--   0        0        0     1862 2023-06-23 10:03:47.753255 csup_analyzer-0.1.1/csup_analyzer/replay/FileHandler.py
--rw-r--r--   0        0        0     1950 2023-06-22 18:44:16.696831 csup_analyzer-0.1.1/csup_analyzer/replay/ReplayFile.py
--rw-r--r--   0        0        0        0 2023-06-22 18:33:34.336945 csup_analyzer-0.1.1/csup_analyzer/replay/__init__.py
--rw-r--r--   0        0        0      564 2023-06-25 17:04:49.393877 csup_analyzer-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3645 1970-01-01 00:00:00.000000 csup_analyzer-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-22 17:30:13.797630 csup_analyzer-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3447 2023-06-25 17:09:16.513819 csup_analyzer-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-25 17:04:13.213877 csup_analyzer-0.1.2/csup_analyzer/__init__.py
+-rw-r--r--   0        0        0     1776 2023-06-24 10:42:39.455239 csup_analyzer-0.1.2/csup_analyzer/event/Driver.py
+-rw-r--r--   0        0        0     6195 2023-06-25 11:28:00.122788 csup_analyzer-0.1.2/csup_analyzer/event/Event.py
+-rw-r--r--   0        0        0      438 2023-06-24 08:34:34.445951 csup_analyzer-0.1.2/csup_analyzer/event/LineUp.py
+-rw-r--r--   0        0        0    10866 2023-06-25 16:48:37.404077 csup_analyzer-0.1.2/csup_analyzer/event/Result.py
+-rw-r--r--   0        0        0        0 2023-06-25 13:43:11.091718 csup_analyzer-0.1.2/csup_analyzer/event/__init__.py
+-rw-r--r--   0        0        0      161 2023-06-25 13:44:36.861708 csup_analyzer-0.1.2/csup_analyzer/plots/Plots.py
+-rw-r--r--   0        0        0        0 2023-06-25 13:43:18.531717 csup_analyzer-0.1.2/csup_analyzer/plots/__init__.py
+-rw-r--r--   0        0        0     1862 2023-06-23 10:03:47.753255 csup_analyzer-0.1.2/csup_analyzer/replay/FileHandler.py
+-rw-r--r--   0        0        0     1950 2023-06-22 18:44:16.696831 csup_analyzer-0.1.2/csup_analyzer/replay/ReplayFile.py
+-rw-r--r--   0        0        0        0 2023-06-22 18:33:34.336945 csup_analyzer-0.1.2/csup_analyzer/replay/__init__.py
+-rw-r--r--   0        0        0      563 2023-07-02 16:28:57.597220 csup_analyzer-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3853 1970-01-01 00:00:00.000000 csup_analyzer-0.1.2/PKG-INFO
```

### Comparing `csup_analyzer-0.1.1/LICENSE` & `csup_analyzer-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `csup_analyzer-0.1.1/README.md` & `csup_analyzer-0.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -36,17 +36,19 @@
 Another reason for this project is that the initial author, Dremet, is administrating the community website https://www.csup.app/ which offers league administration, standings calculations, an elo list, driver statistics etc. Until the 1.5.0 patch there was no way to automatically enter race results into the database behind the website. Extracting data from the .header files is the first step to (semi-) automize result entry. The plan is to launch a CSUP.APP discord bot that offers a `/enter_results {race_id} {header_files}` command for organizers to enter results easily. That bot would use this library to extract the data from the replay files.
 
 ## How
 After each race you can find a .header file for each session (e.g. one for qualification and one for the race) in a folder. Assuming your main drive is named **"C:"** as well you only need to replace "WINDOWS_USER" and "SOME_USER_ID" in the follow folder path to find the replay files on your computer:
 
 `C:\Users\WINDOWS_USER\AppData\LocalLow\Square Enix Ltd\circuit-superstars\SOME_USER_ID\race-recordings`
 
-If you use pdm for your python environments you should be able to easily set up the environment with the pyproject.toml file. Otherwise a `requirements.txt` file is provided. 
+If you just want to use the library, simply install it like any other library with `pip install csup_analyzer` or `pdm add csup_analyzer`. 
 
-Then you can adapt the file paths in `run.py` and have fun with the modified pandas DataFrame accessible via `event.result_df`. 
+If you want to develop/contribute and you use pdm for your python environments you should be able to easily set up the environment with the pyproject.toml file (`pdm install`). Otherwise a `requirements.txt` file is provided. 
+
+Afterwards you can adapt the file paths in `run.py` to test it and have fun with the modified pandas DataFrame accessible via `event.result_df`. 
 
 
 ## Contribute
 
 You are very welcome to work on this project and create pull requests! Feel free to contact me (Dremet) on Discord. You'll find me on (almost) all CSUP discord servers.
 
 If you want to add calculations please have a look at `csup_analyzer/event/Result.py`.
```

### Comparing `csup_analyzer-0.1.1/csup_analyzer/event/Driver.py` & `csup_analyzer-0.1.2/csup_analyzer/event/Driver.py`

 * *Files identical despite different names*

### Comparing `csup_analyzer-0.1.1/csup_analyzer/event/Event.py` & `csup_analyzer-0.1.2/csup_analyzer/event/Event.py`

 * *Files identical despite different names*

### Comparing `csup_analyzer-0.1.1/csup_analyzer/event/Result.py` & `csup_analyzer-0.1.2/csup_analyzer/event/Result.py`

 * *Files identical despite different names*

### Comparing `csup_analyzer-0.1.1/csup_analyzer/replay/FileHandler.py` & `csup_analyzer-0.1.2/csup_analyzer/replay/FileHandler.py`

 * *Files identical despite different names*

### Comparing `csup_analyzer-0.1.1/csup_analyzer/replay/ReplayFile.py` & `csup_analyzer-0.1.2/csup_analyzer/replay/ReplayFile.py`

 * *Files identical despite different names*

### Comparing `csup_analyzer-0.1.1/pyproject.toml` & `csup_analyzer-0.1.2/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [project]
 name = "csup_analyzer"
-version = "0.1.1"
+version = "0.1.2"
 description = "Reads replay files from the game Circuit Superstars and offers tools to analyze the extracted data"
 authors = [
     { name = "Andre Petersen", email = "info@csup.app" },
 ]
 dependencies = [
     "pandas>=2.0.2",
     "numpy>=1.25.0",
     "matplotlib>=3.7.1",
     "scipy>=1.9.3",
 ]
-requires-python = ">=3.10"
+requires-python = ">=3.9"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
```

### Comparing `csup_analyzer-0.1.1/PKG-INFO` & `csup_analyzer-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
-Name: csup-analyzer
-Version: 0.1.1
+Name: csup_analyzer
+Version: 0.1.2
 Summary: Reads replay files from the game Circuit Superstars and offers tools to analyze the extracted data
 Author-Email: Andre Petersen <info@csup.app>
 License: MIT
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Requires-Dist: pandas>=2.0.2
 Requires-Dist: numpy>=1.25.0
 Requires-Dist: matplotlib>=3.7.1
 Requires-Dist: scipy>=1.9.3
 Description-Content-Type: text/markdown
 
 # CSUP Analyzer
@@ -49,17 +49,19 @@
 Another reason for this project is that the initial author, Dremet, is administrating the community website https://www.csup.app/ which offers league administration, standings calculations, an elo list, driver statistics etc. Until the 1.5.0 patch there was no way to automatically enter race results into the database behind the website. Extracting data from the .header files is the first step to (semi-) automize result entry. The plan is to launch a CSUP.APP discord bot that offers a `/enter_results {race_id} {header_files}` command for organizers to enter results easily. That bot would use this library to extract the data from the replay files.
 
 ## How
 After each race you can find a .header file for each session (e.g. one for qualification and one for the race) in a folder. Assuming your main drive is named **"C:"** as well you only need to replace "WINDOWS_USER" and "SOME_USER_ID" in the follow folder path to find the replay files on your computer:
 
 `C:\Users\WINDOWS_USER\AppData\LocalLow\Square Enix Ltd\circuit-superstars\SOME_USER_ID\race-recordings`
 
-If you use pdm for your python environments you should be able to easily set up the environment with the pyproject.toml file. Otherwise a `requirements.txt` file is provided. 
+If you just want to use the library, simply install it like any other library with `pip install csup_analyzer` or `pdm add csup_analyzer`. 
 
-Then you can adapt the file paths in `run.py` and have fun with the modified pandas DataFrame accessible via `event.result_df`. 
+If you want to develop/contribute and you use pdm for your python environments you should be able to easily set up the environment with the pyproject.toml file (`pdm install`). Otherwise a `requirements.txt` file is provided. 
+
+Afterwards you can adapt the file paths in `run.py` to test it and have fun with the modified pandas DataFrame accessible via `event.result_df`. 
 
 
 ## Contribute
 
 You are very welcome to work on this project and create pull requests! Feel free to contact me (Dremet) on Discord. You'll find me on (almost) all CSUP discord servers.
 
 If you want to add calculations please have a look at `csup_analyzer/event/Result.py`.
```

