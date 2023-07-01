# Comparing `tmp/photos_where-1.2.tar.gz` & `tmp/photos_where-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "photos_where-1.2.tar", last modified: Fri Jun 30 22:42:25 2023, max compression
+gzip compressed data, was "photos_where-1.3.tar", last modified: Sat Jul  1 22:30:59 2023, max compression
```

## Comparing `photos_where-1.2.tar` & `photos_where-1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 visgean    (501) staff       (20)        0 2023-06-30 22:42:25.819659 photos_where-1.2/
--rw-r--r--   0 visgean    (501) staff       (20)     1063 2022-09-28 18:42:28.000000 photos_where-1.2/LICENSE
--rw-r--r--   0 visgean    (501) staff       (20)       52 2023-06-30 18:32:54.000000 photos_where-1.2/MANIFEST.in
--rw-r--r--   0 visgean    (501) staff       (20)     1941 2023-06-30 22:42:25.819526 photos_where-1.2/PKG-INFO
--rw-r--r--   0 visgean    (501) staff       (20)     1251 2023-06-30 22:41:25.000000 photos_where-1.2/README.md
-drwxr-xr-x   0 visgean    (501) staff       (20)        0 2023-06-30 22:42:25.818537 photos_where-1.2/photos_where/
--rw-r--r--   0 visgean    (501) staff       (20)       25 2023-06-30 22:30:00.000000 photos_where-1.2/photos_where/__init__.py
--rwxr-xr-x   0 visgean    (501) staff       (20)     2037 2023-06-30 18:47:13.000000 photos_where-1.2/photos_where/main.py
--rw-r--r--   0 visgean    (501) staff       (20)     5100 2023-06-30 22:25:30.000000 photos_where-1.2/photos_where/where.py
-drwxr-xr-x   0 visgean    (501) staff       (20)        0 2023-06-30 22:42:25.819339 photos_where-1.2/photos_where.egg-info/
--rw-r--r--   0 visgean    (501) staff       (20)     1941 2023-06-30 22:42:25.000000 photos_where-1.2/photos_where.egg-info/PKG-INFO
--rw-r--r--   0 visgean    (501) staff       (20)      324 2023-06-30 22:42:25.000000 photos_where-1.2/photos_where.egg-info/SOURCES.txt
--rw-r--r--   0 visgean    (501) staff       (20)        1 2023-06-30 22:42:25.000000 photos_where-1.2/photos_where.egg-info/dependency_links.txt
--rw-r--r--   0 visgean    (501) staff       (20)       57 2023-06-30 22:42:25.000000 photos_where-1.2/photos_where.egg-info/entry_points.txt
--rw-r--r--   0 visgean    (501) staff       (20)       54 2023-06-30 22:42:25.000000 photos_where-1.2/photos_where.egg-info/requires.txt
--rw-r--r--   0 visgean    (501) staff       (20)       13 2023-06-30 22:42:25.000000 photos_where-1.2/photos_where.egg-info/top_level.txt
--rw-r--r--   0 visgean    (501) staff       (20)       38 2023-06-30 22:42:25.819699 photos_where-1.2/setup.cfg
--rw-r--r--   0 visgean    (501) staff       (20)     1017 2023-06-30 22:41:25.000000 photos_where-1.2/setup.py
+drwxr-xr-x   0 visgean    (501) staff       (20)        0 2023-07-01 22:30:59.739050 photos_where-1.3/
+-rw-r--r--   0 visgean    (501) staff       (20)     1063 2022-09-28 18:42:28.000000 photos_where-1.3/LICENSE
+-rw-r--r--   0 visgean    (501) staff       (20)       52 2023-06-30 18:32:54.000000 photos_where-1.3/MANIFEST.in
+-rw-r--r--   0 visgean    (501) staff       (20)     1943 2023-07-01 22:30:59.738836 photos_where-1.3/PKG-INFO
+-rw-r--r--   0 visgean    (501) staff       (20)     1253 2023-07-01 21:31:17.000000 photos_where-1.3/README.md
+drwxr-xr-x   0 visgean    (501) staff       (20)        0 2023-07-01 22:30:59.737936 photos_where-1.3/photos_where/
+-rw-r--r--   0 visgean    (501) staff       (20)       25 2023-06-30 22:30:00.000000 photos_where-1.3/photos_where/__init__.py
+-rwxr-xr-x   0 visgean    (501) staff       (20)     2037 2023-06-30 18:47:13.000000 photos_where-1.3/photos_where/main.py
+-rw-r--r--   0 visgean    (501) staff       (20)     5152 2023-07-01 22:17:33.000000 photos_where-1.3/photos_where/where.py
+drwxr-xr-x   0 visgean    (501) staff       (20)        0 2023-07-01 22:30:59.738582 photos_where-1.3/photos_where.egg-info/
+-rw-r--r--   0 visgean    (501) staff       (20)     1943 2023-07-01 22:30:59.000000 photos_where-1.3/photos_where.egg-info/PKG-INFO
+-rw-r--r--   0 visgean    (501) staff       (20)      324 2023-07-01 22:30:59.000000 photos_where-1.3/photos_where.egg-info/SOURCES.txt
+-rw-r--r--   0 visgean    (501) staff       (20)        1 2023-07-01 22:30:59.000000 photos_where-1.3/photos_where.egg-info/dependency_links.txt
+-rw-r--r--   0 visgean    (501) staff       (20)       57 2023-07-01 22:30:59.000000 photos_where-1.3/photos_where.egg-info/entry_points.txt
+-rw-r--r--   0 visgean    (501) staff       (20)       62 2023-07-01 22:30:59.000000 photos_where-1.3/photos_where.egg-info/requires.txt
+-rw-r--r--   0 visgean    (501) staff       (20)       13 2023-07-01 22:30:59.000000 photos_where-1.3/photos_where.egg-info/top_level.txt
+-rw-r--r--   0 visgean    (501) staff       (20)       38 2023-07-01 22:30:59.739101 photos_where-1.3/setup.cfg
+-rw-r--r--   0 visgean    (501) staff       (20)     1036 2023-07-01 22:30:15.000000 photos_where-1.3/setup.py
```

### Comparing `photos_where-1.2/LICENSE` & `photos_where-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `photos_where-1.2/PKG-INFO` & `photos_where-1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: photos_where
-Version: 1.2
+Version: 1.3
 Summary: Analyze exif data
 Home-page: https://github.com/visgean/where
 Author: Visgean
 Author-email: visgean@gmail.com
 License: MIT
 Description: # Where - day by day location from your photos 
         
@@ -19,17 +19,17 @@
         
         See ``example.ipynb`` for example graphs and data frames exported.
         
         ## Install:
         
         See PYPI [Python package](https://pypi.org/project/photos-where/). 
         
-        ``
+        ```
         $ pip install photos-where
-        ``
+        ```
         
         ## Use:
         
         ```
         $ photos_where Dropbox/Photos/2020/
         $ ls where
         cities-pie.jpg
```

### Comparing `photos_where-1.2/README.md` & `photos_where-1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 
 See ``example.ipynb`` for example graphs and data frames exported.
 
 ## Install:
 
 See PYPI [Python package](https://pypi.org/project/photos-where/). 
 
-``
+```
 $ pip install photos-where
-``
+```
 
 ## Use:
 
 ```
 $ photos_where Dropbox/Photos/2020/
 $ ls where
 cities-pie.jpg
```

### Comparing `photos_where-1.2/photos_where/main.py` & `photos_where-1.3/photos_where/main.py`

 * *Files identical despite different names*

### Comparing `photos_where-1.2/photos_where/where.py` & `photos_where-1.3/photos_where/where.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,17 @@
                 ['cleaned_latitude', 'cleaned_longitude']
             ].itertuples(index=False)
         ]
         country_df = pd.DataFrame(geocoder.query(tuple_locs))
         # add date index, geocoder preservers the
         # order of the rows so this is fine
         country_df.index = df_location.index
-        return df_location.join(country_df)
+        df = df_location.join(country_df)
+        df.sort_index(inplace=True)
+        return df
 
 
     def _get_intervals(self):
         first_row = self.countries_df[:1].to_dict(orient='index')
         previous_date = list(first_row.keys())[0]
         previous_country_code = first_row[previous_date]['cc']
         previous_country = first_row[previous_date]['admin1']
```

### Comparing `photos_where-1.2/photos_where.egg-info/PKG-INFO` & `photos_where-1.3/photos_where.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: photos-where
-Version: 1.2
+Version: 1.3
 Summary: Analyze exif data
 Home-page: https://github.com/visgean/where
 Author: Visgean
 Author-email: visgean@gmail.com
 License: MIT
 Description: # Where - day by day location from your photos 
         
@@ -19,17 +19,17 @@
         
         See ``example.ipynb`` for example graphs and data frames exported.
         
         ## Install:
         
         See PYPI [Python package](https://pypi.org/project/photos-where/). 
         
-        ``
+        ```
         $ pip install photos-where
-        ``
+        ```
         
         ## Use:
         
         ```
         $ photos_where Dropbox/Photos/2020/
         $ ls where
         cities-pie.jpg
```

### Comparing `photos_where-1.2/setup.py` & `photos_where-1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     from distutils.core import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="photos_where",
-    version="1.2",
+    version="1.3",
     description="Analyze exif data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Visgean",
     author_email="visgean@gmail.com",
     url="https://github.com/visgean/where",
     packages=[
@@ -31,10 +31,11 @@
         "Programming Language :: Python :: 3.7",
     ],
     install_requires=[
         "exif2pandas",
         "pandas",
         "matplotlib",
         "reverse-geocoder==1.5.1",
+        "pyarrow",
     ],
     entry_points={"console_scripts": ["photos_where = photos_where.main:main"]},
 )
```

