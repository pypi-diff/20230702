# Comparing `tmp/python_redex-0.0.1.tar.gz` & `tmp/python_redex-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_redex-0.0.1.tar", last modified: Sun Jul  2 15:54:22 2023, max compression
+gzip compressed data, was "python_redex-0.0.2.tar", last modified: Sun Jul  2 15:58:59 2023, max compression
```

## Comparing `python_redex-0.0.1.tar` & `python_redex-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 15:54:22.933618 python_redex-0.0.1/
--rw-rw-rw-   0        0        0     1064 2023-07-02 15:30:02.000000 python_redex-0.0.1/LICENCE.txt
--rw-rw-rw-   0        0        0       11 2023-07-02 15:28:52.000000 python_redex-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      568 2023-07-02 15:54:22.933618 python_redex-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      116 2023-07-02 15:27:01.000000 python_redex-0.0.1/README.txt
-drwxrwxrwx   0        0        0        0 2023-07-02 15:54:22.930552 python_redex-0.0.1/python_redex.egg-info/
--rw-rw-rw-   0        0        0      568 2023-07-02 15:54:22.000000 python_redex-0.0.1/python_redex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2023-07-02 15:54:22.000000 python_redex-0.0.1/python_redex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 15:54:22.000000 python_redex-0.0.1/python_redex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-02 15:54:22.000000 python_redex-0.0.1/python_redex.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-02 15:54:22.931609 python_redex-0.0.1/redex/
--rw-rw-rw-   0        0        0     1440 2023-07-02 15:22:35.000000 python_redex-0.0.1/redex/__init__.py
--rw-rw-rw-   0        0        0       42 2023-07-02 15:54:22.934620 python_redex-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      704 2023-07-02 15:54:14.000000 python_redex-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 15:58:59.230078 python_redex-0.0.2/
+-rw-rw-rw-   0        0        0     1064 2023-07-02 15:30:02.000000 python_redex-0.0.2/LICENCE.txt
+-rw-rw-rw-   0        0        0       11 2023-07-02 15:28:52.000000 python_redex-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      635 2023-07-02 15:58:59.229060 python_redex-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      116 2023-07-02 15:27:01.000000 python_redex-0.0.2/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-02 15:58:59.226179 python_redex-0.0.2/python_redex.egg-info/
+-rw-rw-rw-   0        0        0      635 2023-07-02 15:58:59.000000 python_redex-0.0.2/python_redex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2023-07-02 15:58:59.000000 python_redex-0.0.2/python_redex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 15:58:59.000000 python_redex-0.0.2/python_redex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-02 15:58:59.000000 python_redex-0.0.2/python_redex.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-02 15:58:59.227144 python_redex-0.0.2/redex/
+-rw-rw-rw-   0        0        0     1440 2023-07-02 15:58:19.000000 python_redex-0.0.2/redex/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-07-02 15:58:59.230078 python_redex-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      793 2023-07-02 15:58:53.000000 python_redex-0.0.2/setup.py
```

### Comparing `python_redex-0.0.1/LICENCE.txt` & `python_redex-0.0.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `python_redex-0.0.1/PKG-INFO` & `python_redex-0.0.2/python_redex.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
-Name: python_redex
-Version: 0.0.1
+Name: python-redex
+Version: 0.0.2
 Summary: User friendly version of regex. More information available at https://github.com/TimoKats/redex
 Home-page: 
 Author: Timo Kats
 Author-email: tpakats@gmail.com
 License: MIT
 Keywords: regex
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 License-File: LICENCE.txt
+
+More information available at https://github.com/TimoKats/redex
```

### Comparing `python_redex-0.0.1/python_redex.egg-info/PKG-INFO` & `python_redex-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
-Name: python-redex
-Version: 0.0.1
+Name: python_redex
+Version: 0.0.2
 Summary: User friendly version of regex. More information available at https://github.com/TimoKats/redex
 Home-page: 
 Author: Timo Kats
 Author-email: tpakats@gmail.com
 License: MIT
 Keywords: regex
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 License-File: LICENCE.txt
+
+More information available at https://github.com/TimoKats/redex
```

### Comparing `python_redex-0.0.1/redex/__init__.py` & `python_redex-0.0.2/redex/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,10 +29,10 @@
         elif search.get_result()[index] and format == 'tuple':
             locations.append((index, location))
     return locations
 
 def info():
     print('\n---')
     print('    ^ ^          Description:        Python library for readable regex.')
-    print('("\(-_-)/")      Version:            0.0.1') 
+    print('("\(-_-)/")      Version:            0.0.2') 
     print(' )(  O  )(       Author:             Timo Kats')
     print('((...)(...))     Last updated:       02/07/2023', end='\n---\n\n')
```

### Comparing `python_redex-0.0.1/setup.py` & `python_redex-0.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,16 +7,17 @@
     'License :: OSI Approved :: MIT License',
     'Operating System :: Microsoft :: Windows',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='python_redex',
-    version='0.0.1',
+    version='0.0.2',
     description='User friendly version of regex. More information available at https://github.com/TimoKats/redex',
+    long_description='More information available at https://github.com/TimoKats/redex',
     url='',  
     author='Timo Kats',
     author_email='tpakats@gmail.com',
     license='MIT', 
     classifiers=classifiers,
     keywords='regex', 
     packages=find_packages(),
```

