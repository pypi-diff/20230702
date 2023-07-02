# Comparing `tmp/pytest-pyreport-1.0.1.tar.gz` & `tmp/pytest-pyreport-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-pyreport-1.0.1.tar", last modified: Mon May  8 15:21:00 2023, max compression
+gzip compressed data, was "pytest-pyreport-1.1.0.tar", last modified: Sun Jul  2 00:34:34 2023, max compression
```

## Comparing `pytest-pyreport-1.0.1.tar` & `pytest-pyreport-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:21:00.685508 pytest-pyreport-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-08 15:20:49.000000 pytest-pyreport-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-08 15:21:00.685508 pytest-pyreport-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-08 15:20:49.000000 pytest-pyreport-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 15:21:00.685508 pytest-pyreport-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-08 15:20:49.000000 pytest-pyreport-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:21:00.685508 pytest-pyreport-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:21:00.685508 pytest-pyreport-1.0.1/src/pytest_pyreport/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:20:49.000000 pytest-pyreport-1.0.1/src/pytest_pyreport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-08 15:20:49.000000 pytest-pyreport-1.0.1/src/pytest_pyreport/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:21:00.685508 pytest-pyreport-1.0.1/src/pytest_pyreport/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-08 15:20:49.000000 pytest-pyreport-1.0.1/src/pytest_pyreport/templates/template.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:21:00.685508 pytest-pyreport-1.0.1/src/pytest_pyreport.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-08 15:21:00.000000 pytest-pyreport-1.0.1/src/pytest_pyreport.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-08 15:21:00.000000 pytest-pyreport-1.0.1/src/pytest_pyreport.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 15:21:00.000000 pytest-pyreport-1.0.1/src/pytest_pyreport.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-08 15:21:00.000000 pytest-pyreport-1.0.1/src/pytest_pyreport.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-08 15:21:00.000000 pytest-pyreport-1.0.1/src/pytest_pyreport.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 15:21:00.000000 pytest-pyreport-1.0.1/src/pytest_pyreport.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 00:34:34.293845 pytest-pyreport-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-02 00:34:21.000000 pytest-pyreport-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-02 00:34:34.293845 pytest-pyreport-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-02 00:34:21.000000 pytest-pyreport-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 00:34:34.293845 pytest-pyreport-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-02 00:34:21.000000 pytest-pyreport-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 00:34:34.293845 pytest-pyreport-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 00:34:34.293845 pytest-pyreport-1.1.0/src/pytest_pyreport/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 00:34:21.000000 pytest-pyreport-1.1.0/src/pytest_pyreport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-07-02 00:34:21.000000 pytest-pyreport-1.1.0/src/pytest_pyreport/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 00:34:34.293845 pytest-pyreport-1.1.0/src/pytest_pyreport/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     9214 2023-07-02 00:34:21.000000 pytest-pyreport-1.1.0/src/pytest_pyreport/templates/template.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 00:34:34.293845 pytest-pyreport-1.1.0/src/pytest_pyreport.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-02 00:34:34.000000 pytest-pyreport-1.1.0/src/pytest_pyreport.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-02 00:34:34.000000 pytest-pyreport-1.1.0/src/pytest_pyreport.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 00:34:34.000000 pytest-pyreport-1.1.0/src/pytest_pyreport.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-02 00:34:34.000000 pytest-pyreport-1.1.0/src/pytest_pyreport.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-02 00:34:34.000000 pytest-pyreport-1.1.0/src/pytest_pyreport.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-02 00:34:34.000000 pytest-pyreport-1.1.0/src/pytest_pyreport.egg-info/top_level.txt
```

### Comparing `pytest-pyreport-1.0.1/LICENSE` & `pytest-pyreport-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-pyreport-1.0.1/PKG-INFO` & `pytest-pyreport-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-pyreport
-Version: 1.0.1
+Version: 1.1.0
 Summary: PyReport is a lightweight reporting plugin for Pytest that provides concise HTML report
 Home-page: https://github.com/ToghrulMirzayev/pytest-pyreport
 Author: Toghrul Mirzayev
 Author-email: togrul.mirzoev@gmail.com
 License: MIT
 Keywords: pytest_pyreport,python,pytest,report
 Classifier: Framework :: Pytest
@@ -17,22 +17,32 @@
 License-File: LICENSE
 
 # PyReport
 
 # Quick overview
 PyReport is a lightweight reporting plugin for Pytest that provides concise HTML reports by parsing JunitXML test results
 
+# Pre-requisites
+To be able to use this plugin you will need below dependencies:
+* Python >=3.8
+* Jinja2
+* Pytest
+
 # Getting started
 
 To start using PyReport please follow below instructions:
 
 * Install `pytest-pyreport` plugin:
 ```
 pip install pytest-pyreport==<version>
 ```
 
 * Run tests using below command:
 ```
 pytest --junitxml=result.xml -o junit_family="xunit1" --pyreport
 ```
 
-* You should see `pyreport.html` file that auto generated by using above command. Open it and check the test results
+* You should see `pyreport.html` file that auto generated by using above command. \
+Open it and check the test results as shown in below presentation
+
+# Presentation
+![pyreport](presentation.gif)
```

### Comparing `pytest-pyreport-1.0.1/setup.py` & `pytest-pyreport-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pytest-pyreport',
-    version='1.0.1',
+    version='1.1.0',
     description='PyReport is a lightweight reporting plugin for Pytest that provides concise HTML report',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     author='Toghrul Mirzayev',
     author_email='togrul.mirzoev@gmail.com',
     url='https://github.com/ToghrulMirzayev/pytest-pyreport',
     packages=find_packages("src"),
```

### Comparing `pytest-pyreport-1.0.1/src/pytest_pyreport/plugin.py` & `pytest-pyreport-1.1.0/src/pytest_pyreport/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-pyreport-1.0.1/src/pytest_pyreport/templates/template.html` & `pytest-pyreport-1.1.0/src/pytest_pyreport/templates/template.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,129 +1,199 @@
 <!DOCTYPE html>
 <html>
 <head>
 	<title>PyReport</title>
 	<style>
 		body {
-font-family: Arial, Helvetica, sans-serif;
-margin: 0;
-padding: 0;
-}
-
-.frame {
-width: 80%;
-margin: 0 auto;
-border: 1px solid #ccc;
-padding: 20px;
-box-sizing: border-box;
-background-color: #f2f2f2;
-}
-
-h1 {
-text-align: center;
-}
-
-table {
-width: 100%;
-border-collapse: collapse;
-margin-top: 20px;
-}
-
-th, td {
-padding: 10px;
-text-align: left;
-border-bottom: 1px solid #ddd;
-}
-
-th {
-background-color: #4CAF50;
-color: white;
-}
-
-.pass {
-    color: #4CAF50 !important;
-    font-weight: bold;
-}
-
-
-.fail {
-color: red;
-font-weight: bold;
-cursor: zoom-in;
-}
-
-.skip {
-color: rgb(255, 165, 0);
-font-weight: bold;
-}
-
-.hide {
-display: none;
-}
-
-.fail.expanded {
-    cursor: zoom-out;
-}
-
-.collapse {
-    display: none;
-}
-
-#pie-chart {
-    width: 200px;
-    height: 200px;
-}
-
-#test_results {
-  max-width: 600px;
-  margin: 5px auto;
-}
-
-.frame {
-    max-width: 600px;
-    margin: 40px auto;
-}
-
-#test_results {
-    max-width: 600px;
-    margin: 20px auto;
-}
-
-#summary_table {
-    max-width: 600px;
-    margin: 20px auto;
-}
-
-body {
-  background: linear-gradient(to bottom right, #d1f7c4, #ffffff);
-}
+			font-family: Arial, Helvetica, sans-serif;
+			margin: 0;
+			padding: 0;
+			transition: background-color 0.3s ease;
+		}
+
+		.frame {
+			width: 80%;
+			margin: 0 auto;
+			border: 1px solid #ccc;
+			padding: 20px;
+			box-sizing: border-box;
+			background-color: #f2f2f2;
+		}
 
-h1 {
+		h1 {
 			font-size: 36px;
 			text-align: center;
 			text-transform: uppercase;
 			letter-spacing: 2px;
 			color: #333;
 			border-bottom: 2px solid #333;
 			padding: 20px;
 			margin: 0;
 		}
 
-.header {
-	position: fixed;
-	top: 0;
-	left: 0;
-	width: 100%;
-	padding: 2px;
-	background-color: #4CAF50;
-}
+		table {
+			width: 100%;
+			border-collapse: collapse;
+			margin-top: 20px;
+		}
+
+		th, td {
+			padding: 10px;
+			text-align: left;
+			border-bottom: 1px solid #ddd;
+		}
+
+		th {
+			background-color: #4CAF50;
+			color: white;
+		}
+
+		.pass {
+			color: #4CAF50 !important;
+			font-weight: bold;
+		}
+		.test_row.pass td {
+			color: #4CAF50 !important;
+			font-weight: bold;
+		}
+
+		.fail {
+			color: red !important;
+			font-weight: bold;
+			cursor: zoom-in;
+		}
+
+		.test_row.fail td {
+			color: red !important;
+			font-weight: bold;
+			cursor: zoom-in;
+		}
+
+		.skip {
+			color: rgb(255, 165, 0) !important;
+			font-weight: bold;
+		}
+
+		.test_row.skip td {
+			color: rgb(255, 165, 0) !important;
+			font-weight: bold;
+		}
+
+		.hide {
+			display: none;
+		}
+
+		.fail.expanded {
+			cursor: zoom-out;
+			color: red;
+		}
+
+		.collapse {
+			display: none;
+		}
+
+		#pie-chart {
+			width: 200px;
+			height: 200px;
+		}
+
+		#test_results {
+			max-width: 600px;
+			margin: 5px auto;
+		}
+
+		.frame {
+			max-width: 600px;
+			margin: 40px auto;
+		}
+
+		#test_results {
+			max-width: 600px;
+			margin: 20px auto;
+		}
+
+		#summary_table {
+			max-width: 600px;
+			margin: 20px auto;
+		}
+
+		.header {
+			position: fixed;
+			top: 0;
+			left: 0;
+			width: 100%;
+			padding: 2px;
+			background-color: #4CAF50;
+		}
+
+		.toggle-switch {
+			position: fixed;
+			top: 50px;
+			right: 10px;
+			z-index: 999;
+			display: flex;
+			align-items: center;
+			justify-content: center;
+			width: 60px;
+			height: 30px;
+			background-color: #042D50;
+			border-radius: 15px;
+			cursor: pointer;
+			transition: background-color 0.3s ease;
+		}
+
+		.toggle-switch::before {
+			content: '';
+			position: absolute;
+			width: 26px;
+			height: 26px;
+			border-radius: 50%;
+			background-color: white;
+			box-shadow: 0 2px 4px rgba(0, 0, 0, 0.4);
+			transition: transform 0.3s ease;
+			left: 2px;
+		}
+
+		.night-mode {
+			background-color: #031D33;
+		}
+
+		.night-mode .toggle-switch {
+			background-color: #4CAF50;
+		}
+
+		.night-mode .toggle-switch::before {
+			transform: translateX(30px);
+		}
+		.night-mode body {
+			background-color: #031D33;
+		}
+
+		.night-mode h1 {
+			border-bottom-color: #fff;
+			color: #fff;
+		}
+
+		.night-mode th {
+			background-color: #042D50;
+		}
+
+		.night-mode .header {
+			background-color: #042D50;
+		}
+		.night-mode tr td {
+    	color: white;
+    	}
 	</style>
 	<script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
 	<script src="https://cdn.jsdelivr.net/npm/chart.js@3.7.1/dist/chart.min.js"></script>
 	<script>
+	function toggleNightMode() {
+			document.body.classList.toggle('night-mode');
+		}
 		$(document).ready(function() {
 			$('.test_row.fail').click(function(){
 				$(this).next('.collapse').toggle();
 				$(this).toggleClass('expanded');
 			});
 		});
 	</script>
@@ -132,14 +202,16 @@
 	<header style="text-align: center;">
 		<div class="header">
 		<a href="/">
             <img src="data:image/png;base64,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" alt="PyReport Logo">
         </a>
 	</div>
 	</header>
+	<div class="toggle-switch" onclick="toggleNightMode()">
+	</div>
 	<div class="frame">
 		<div style="width: 100%;">
 			<canvas id="pie-chart"></canvas>
 		</div>
 	</div>
 	<script>
 		var ctx = document.getElementById('pie-chart').getContext('2d');
```

### Comparing `pytest-pyreport-1.0.1/src/pytest_pyreport.egg-info/PKG-INFO` & `pytest-pyreport-1.1.0/src/pytest_pyreport.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-pyreport
-Version: 1.0.1
+Version: 1.1.0
 Summary: PyReport is a lightweight reporting plugin for Pytest that provides concise HTML report
 Home-page: https://github.com/ToghrulMirzayev/pytest-pyreport
 Author: Toghrul Mirzayev
 Author-email: togrul.mirzoev@gmail.com
 License: MIT
 Keywords: pytest_pyreport,python,pytest,report
 Classifier: Framework :: Pytest
@@ -17,22 +17,32 @@
 License-File: LICENSE
 
 # PyReport
 
 # Quick overview
 PyReport is a lightweight reporting plugin for Pytest that provides concise HTML reports by parsing JunitXML test results
 
+# Pre-requisites
+To be able to use this plugin you will need below dependencies:
+* Python >=3.8
+* Jinja2
+* Pytest
+
 # Getting started
 
 To start using PyReport please follow below instructions:
 
 * Install `pytest-pyreport` plugin:
 ```
 pip install pytest-pyreport==<version>
 ```
 
 * Run tests using below command:
 ```
 pytest --junitxml=result.xml -o junit_family="xunit1" --pyreport
 ```
 
-* You should see `pyreport.html` file that auto generated by using above command. Open it and check the test results
+* You should see `pyreport.html` file that auto generated by using above command. \
+Open it and check the test results as shown in below presentation
+
+# Presentation
+![pyreport](presentation.gif)
```

