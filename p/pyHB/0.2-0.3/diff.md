# Comparing `tmp/pyHB-0.2.tar.gz` & `tmp/pyHB-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyHB-0.2.tar", last modified: Sun Jul  2 04:46:04 2023, max compression
+gzip compressed data, was "pyHB-0.3.tar", last modified: Sun Jul  2 05:33:25 2023, max compression
```

## Comparing `pyHB-0.2.tar` & `pyHB-0.3.tar`

### file list

```diff
@@ -1,12 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:46:04.898384 pyHB-0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-02 04:45:53.000000 pyHB-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-02 04:46:04.898384 pyHB-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-02 04:45:53.000000 pyHB-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:46:04.898384 pyHB-0.2/pyHB.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-02 04:46:04.000000 pyHB-0.2/pyHB.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-02 04:46:04.000000 pyHB-0.2/pyHB.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 04:46:04.000000 pyHB-0.2/pyHB.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-02 04:46:04.000000 pyHB-0.2/pyHB.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 04:46:04.000000 pyHB-0.2/pyHB.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 04:46:04.898384 pyHB-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-02 04:45:53.000000 pyHB-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 05:33:25.471655 pyHB-0.3/
+drwxrwxrwx   0        0        0        0 2023-07-02 05:33:25.442114 pyHB-0.3/HB/
+-rw-rw-rw-   0        0        0       45 2023-07-02 05:23:02.000000 pyHB-0.3/HB/__init__.py
+-rw-rw-rw-   0        0        0     2215 2023-07-02 05:23:02.000000 pyHB-0.3/HB/data.py
+-rw-rw-rw-   0        0        0    18587 2023-07-02 05:23:02.000000 pyHB-0.3/HB/functions.py
+-rw-rw-rw-   0        0        0       20 2023-07-02 05:23:02.000000 pyHB-0.3/HB/version.py
+-rw-rw-rw-   0        0        0    35149 2023-07-02 05:23:01.000000 pyHB-0.3/LICENSE
+-rw-rw-rw-   0        0        0      981 2023-07-02 05:33:25.469656 pyHB-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       31 2023-07-02 05:23:01.000000 pyHB-0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-02 05:33:25.466649 pyHB-0.3/pyHB.egg-info/
+-rw-rw-rw-   0        0        0      981 2023-07-02 05:33:25.000000 pyHB-0.3/pyHB.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2023-07-02 05:33:25.000000 pyHB-0.3/pyHB.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 05:33:25.000000 pyHB-0.3/pyHB.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-07-02 05:33:25.000000 pyHB-0.3/pyHB.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        3 2023-07-02 05:33:25.000000 pyHB-0.3/pyHB.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-02 05:33:25.471655 pyHB-0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1555 2023-07-02 05:23:01.000000 pyHB-0.3/setup.py
```

### Comparing `pyHB-0.2/LICENSE` & `pyHB-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyHB-0.2/setup.py` & `pyHB-0.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,20 +5,22 @@
 try:
     with codecs.open( "README.md", 'r', errors='ignore' ) as file:
         readme_contents = file.read()
 except Exception as error:
     readme_contents = ""
     sys.stderr.write( "Warning: Could not open README.md due %s\n" % error )
     
+with open("HB/version.py", "rt", encoding="utf8") as x:
+    version = re.search(r'__version__ = "(.*?)"', x.read()).group(1)
 
 setup(
     name="pyHB",
     author="LegendBoy",
     author_email="krishna045jaiswal@gmail.com",
-    version="0.2",
+    version=version,
     description="This is a simple package which is used in HackBot Support Pyrogram + Telethon",
     long_description = readme_contents,
     long_description_content_type="text/markdown",
     url="https://github.com/LEGEND-AI/pyHB",
     packages=find_packages(),
     license="GNU General Public License v3.0",
     include_package_data=True,
```

