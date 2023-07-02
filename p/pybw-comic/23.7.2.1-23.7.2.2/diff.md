# Comparing `tmp/pybw_comic-23.7.2.1.tar.gz` & `tmp/pybw_comic-23.7.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybw_comic-23.7.2.1.tar", last modified: Sun Jul  2 03:22:37 2023, max compression
+gzip compressed data, was "pybw_comic-23.7.2.2.tar", last modified: Sun Jul  2 14:21:17 2023, max compression
```

## Comparing `pybw_comic-23.7.2.1.tar` & `pybw_comic-23.7.2.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 03:22:37.457502 pybw_comic-23.7.2.1/
--rw-rw-rw-   0        0        0      577 2023-03-14 13:35:46.000000 pybw_comic-23.7.2.1/- command.txt
--rw-rw-rw-   0        0        0     1167 2023-03-13 12:06:00.000000 pybw_comic-23.7.2.1/LICENSE
--rw-rw-rw-   0        0        0       17 2023-03-13 14:36:52.000000 pybw_comic-23.7.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0      764 2023-07-02 03:22:37.456502 pybw_comic-23.7.2.1/PKG-INFO
--rw-rw-rw-   0        0        0       26 2023-06-21 09:53:53.000000 pybw_comic-23.7.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-02 03:22:37.327492 pybw_comic-23.7.2.1/pybw_comic/
--rw-rw-rw-   0        0        0        0 2022-07-27 05:24:03.000000 pybw_comic-23.7.2.1/pybw_comic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-02 03:22:37.440500 pybw_comic-23.7.2.1/pybw_comic/engines/
--rw-rw-rw-   0        0        0        0 2022-07-27 05:24:03.000000 pybw_comic-23.7.2.1/pybw_comic/engines/__init__.py
--rw-rw-rw-   0        0        0    18753 2023-06-20 12:37:25.000000 pybw_comic-23.7.2.1/pybw_comic/engines/_todo_dmzj_cn.py
--rw-rw-rw-   0        0        0    18538 2023-06-21 10:30:25.000000 pybw_comic-23.7.2.1/pybw_comic/engines/_todo_dmzj_requests.py
--rw-rw-rw-   0        0        0    17144 2022-09-21 08:09:06.000000 pybw_comic-23.7.2.1/pybw_comic/engines/cnanjie.py
--rw-rw-rw-   0        0        0    24188 2023-07-02 03:16:17.000000 pybw_comic-23.7.2.1/pybw_comic/engines/copymanga.py
--rw-rw-rw-   0        0        0    22139 2023-06-21 12:15:34.000000 pybw_comic-23.7.2.1/pybw_comic/engines/dmzj_selenium.py
--rw-rw-rw-   0        0        0    23738 2022-09-21 08:08:24.000000 pybw_comic-23.7.2.1/pybw_comic/engines/manhuaDB.py
--rw-rw-rw-   0        0        0    24178 2022-09-21 08:09:13.000000 pybw_comic-23.7.2.1/pybw_comic/engines/maofly.py
--rw-rw-rw-   0        0        0    20791 2022-09-21 08:08:55.000000 pybw_comic-23.7.2.1/pybw_comic/engines/mhkan.py
--rw-rw-rw-   0        0        0    20845 2022-09-21 08:08:09.000000 pybw_comic-23.7.2.1/pybw_comic/engines/www_1kkk.py
--rw-rw-rw-   0        0        0    20667 2023-06-21 12:06:21.000000 pybw_comic-23.7.2.1/pybw_comic/engines/xmanhua.py
-drwxrwxrwx   0        0        0        0 2023-07-02 03:22:37.446500 pybw_comic-23.7.2.1/pybw_comic/scripts/
--rw-rw-rw-   0        0        0        0 2022-07-27 05:24:03.000000 pybw_comic-23.7.2.1/pybw_comic/scripts/__init__.py
--rw-rw-rw-   0        0        0     3433 2023-06-28 01:12:21.000000 pybw_comic-23.7.2.1/pybw_comic/scripts/comic.py
-drwxrwxrwx   0        0        0        0 2023-07-02 03:22:37.357493 pybw_comic-23.7.2.1/pybw_comic.egg-info/
--rw-rw-rw-   0        0        0      764 2023-07-02 03:22:36.000000 pybw_comic-23.7.2.1/pybw_comic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      687 2023-07-02 03:22:37.000000 pybw_comic-23.7.2.1/pybw_comic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 03:22:37.000000 pybw_comic-23.7.2.1/pybw_comic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-07-02 03:22:37.000000 pybw_comic-23.7.2.1/pybw_comic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       23 2023-06-21 09:53:36.000000 pybw_comic-23.7.2.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-02 03:22:37.458502 pybw_comic-23.7.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1507 2023-07-02 03:22:25.000000 pybw_comic-23.7.2.1/setup.py
--rwxrwxrwx   0        0        0      462 2023-06-28 04:27:58.000000 pybw_comic-23.7.2.1/upload_pypi.bat
+drwxrwxrwx   0        0        0        0 2023-07-02 14:21:17.634547 pybw_comic-23.7.2.2/
+-rw-rw-rw-   0        0        0      577 2023-03-14 13:35:46.000000 pybw_comic-23.7.2.2/- command.txt
+-rw-rw-rw-   0        0        0     1167 2023-03-13 12:06:00.000000 pybw_comic-23.7.2.2/LICENSE
+-rw-rw-rw-   0        0        0       17 2023-03-13 14:36:52.000000 pybw_comic-23.7.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      764 2023-07-02 14:21:17.632547 pybw_comic-23.7.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0       26 2023-06-21 09:53:53.000000 pybw_comic-23.7.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-02 14:21:17.489536 pybw_comic-23.7.2.2/pybw_comic/
+-rw-rw-rw-   0        0        0        0 2022-07-27 05:24:03.000000 pybw_comic-23.7.2.2/pybw_comic/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-02 14:21:17.613546 pybw_comic-23.7.2.2/pybw_comic/engines/
+-rw-rw-rw-   0        0        0        0 2022-07-27 05:24:03.000000 pybw_comic-23.7.2.2/pybw_comic/engines/__init__.py
+-rw-rw-rw-   0        0        0    18753 2023-06-20 12:37:25.000000 pybw_comic-23.7.2.2/pybw_comic/engines/_todo_dmzj_cn.py
+-rw-rw-rw-   0        0        0    18538 2023-06-21 10:30:25.000000 pybw_comic-23.7.2.2/pybw_comic/engines/_todo_dmzj_requests.py
+-rw-rw-rw-   0        0        0    17144 2022-09-21 08:09:06.000000 pybw_comic-23.7.2.2/pybw_comic/engines/cnanjie.py
+-rw-rw-rw-   0        0        0    24223 2023-07-02 14:20:37.000000 pybw_comic-23.7.2.2/pybw_comic/engines/copymanga.py
+-rw-rw-rw-   0        0        0    22139 2023-06-21 12:15:34.000000 pybw_comic-23.7.2.2/pybw_comic/engines/dmzj_selenium.py
+-rw-rw-rw-   0        0        0    23738 2022-09-21 08:08:24.000000 pybw_comic-23.7.2.2/pybw_comic/engines/manhuaDB.py
+-rw-rw-rw-   0        0        0    24178 2022-09-21 08:09:13.000000 pybw_comic-23.7.2.2/pybw_comic/engines/maofly.py
+-rw-rw-rw-   0        0        0    20791 2022-09-21 08:08:55.000000 pybw_comic-23.7.2.2/pybw_comic/engines/mhkan.py
+-rw-rw-rw-   0        0        0    20845 2022-09-21 08:08:09.000000 pybw_comic-23.7.2.2/pybw_comic/engines/www_1kkk.py
+-rw-rw-rw-   0        0        0    20667 2023-06-21 12:06:21.000000 pybw_comic-23.7.2.2/pybw_comic/engines/xmanhua.py
+drwxrwxrwx   0        0        0        0 2023-07-02 14:21:17.621546 pybw_comic-23.7.2.2/pybw_comic/scripts/
+-rw-rw-rw-   0        0        0        0 2022-07-27 05:24:03.000000 pybw_comic-23.7.2.2/pybw_comic/scripts/__init__.py
+-rw-rw-rw-   0        0        0     3433 2023-06-28 01:12:21.000000 pybw_comic-23.7.2.2/pybw_comic/scripts/comic.py
+drwxrwxrwx   0        0        0        0 2023-07-02 14:21:17.520538 pybw_comic-23.7.2.2/pybw_comic.egg-info/
+-rw-rw-rw-   0        0        0      764 2023-07-02 14:21:17.000000 pybw_comic-23.7.2.2/pybw_comic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      687 2023-07-02 14:21:17.000000 pybw_comic-23.7.2.2/pybw_comic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 14:21:17.000000 pybw_comic-23.7.2.2/pybw_comic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-02 14:21:17.000000 pybw_comic-23.7.2.2/pybw_comic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       23 2023-06-21 09:53:36.000000 pybw_comic-23.7.2.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-02 14:21:17.635546 pybw_comic-23.7.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1507 2023-07-02 14:20:55.000000 pybw_comic-23.7.2.2/setup.py
+-rwxrwxrwx   0        0        0      462 2023-06-28 04:27:58.000000 pybw_comic-23.7.2.2/upload_pypi.bat
```

### Comparing `pybw_comic-23.7.2.1/- command.txt` & `pybw_comic-23.7.2.2/- command.txt`

 * *Files identical despite different names*

### Comparing `pybw_comic-23.7.2.1/LICENSE` & `pybw_comic-23.7.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pybw_comic-23.7.2.1/PKG-INFO` & `pybw_comic-23.7.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybw_comic
-Version: 23.7.2.1
+Version: 23.7.2.2
 Summary: comic spider
 Home-page: https://gitee.com/pubowei/comic
 Author: Bowei Pu
 Author-email: pubowei@foxmail.com
 License: MIT
 Project-URL: Docs, https://gitee.com/pubowei/comic
 Project-URL: Package, https://pypi.org/project/pybw
```

### Comparing `pybw_comic-23.7.2.1/pybw_comic/engines/_todo_dmzj_cn.py` & `pybw_comic-23.7.2.2/pybw_comic/engines/_todo_dmzj_cn.py`

 * *Files identical despite different names*

### Comparing `pybw_comic-23.7.2.1/pybw_comic/engines/_todo_dmzj_requests.py` & `pybw_comic-23.7.2.2/pybw_comic/engines/_todo_dmzj_requests.py`

 * *Files identical despite different names*

### Comparing `pybw_comic-23.7.2.1/pybw_comic/engines/cnanjie.py` & `pybw_comic-23.7.2.2/pybw_comic/engines/cnanjie.py`

 * *Files identical despite different names*

### Comparing `pybw_comic-23.7.2.1/pybw_comic/engines/copymanga.py` & `pybw_comic-23.7.2.2/pybw_comic/engines/copymanga.py`

 * *Files 1% similar despite different names*

```diff
@@ -577,15 +577,16 @@
                     if start_label not in chap_title:
                         continue
                     else:
                         start_ok = True
                 
                 ## --- Judge if path_chap exist, and skip it
                 if os.path.exists(path_chap):
-                    if glob('{}/*'.format(path_chap)):
+                    _chap_imgs = os.listdir(path_chap)
+                    if _chap_imgs:
                         continue
                 else:
                     os.makedirs(path_chap)
                 
                 chap_url = chap['url']
                 onechap = Chapter(chap_url, headless=self.headless,
                                   driver_img=self.driver_img)
```

### Comparing `pybw_comic-23.7.2.1/pybw_comic/engines/dmzj_selenium.py` & `pybw_comic-23.7.2.2/pybw_comic/engines/dmzj_selenium.py`

 * *Files identical despite different names*

### Comparing `pybw_comic-23.7.2.1/pybw_comic/engines/manhuaDB.py` & `pybw_comic-23.7.2.2/pybw_comic/engines/manhuaDB.py`

 * *Files identical despite different names*

### Comparing `pybw_comic-23.7.2.1/pybw_comic/engines/maofly.py` & `pybw_comic-23.7.2.2/pybw_comic/engines/maofly.py`

 * *Files identical despite different names*

### Comparing `pybw_comic-23.7.2.1/pybw_comic/engines/mhkan.py` & `pybw_comic-23.7.2.2/pybw_comic/engines/mhkan.py`

 * *Files identical despite different names*

### Comparing `pybw_comic-23.7.2.1/pybw_comic/engines/www_1kkk.py` & `pybw_comic-23.7.2.2/pybw_comic/engines/www_1kkk.py`

 * *Files identical despite different names*

### Comparing `pybw_comic-23.7.2.1/pybw_comic/engines/xmanhua.py` & `pybw_comic-23.7.2.2/pybw_comic/engines/xmanhua.py`

 * *Files identical despite different names*

### Comparing `pybw_comic-23.7.2.1/pybw_comic/scripts/comic.py` & `pybw_comic-23.7.2.2/pybw_comic/scripts/comic.py`

 * *Files identical despite different names*

### Comparing `pybw_comic-23.7.2.1/pybw_comic.egg-info/PKG-INFO` & `pybw_comic-23.7.2.2/pybw_comic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybw-comic
-Version: 23.7.2.1
+Version: 23.7.2.2
 Summary: comic spider
 Home-page: https://gitee.com/pubowei/comic
 Author: Bowei Pu
 Author-email: pubowei@foxmail.com
 License: MIT
 Project-URL: Docs, https://gitee.com/pubowei/comic
 Project-URL: Package, https://pypi.org/project/pybw
```

### Comparing `pybw_comic-23.7.2.1/pybw_comic.egg-info/SOURCES.txt` & `pybw_comic-23.7.2.2/pybw_comic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybw_comic-23.7.2.1/setup.py` & `pybw_comic-23.7.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 with open('README.md', encoding='utf-8') as f:
     readme = f.read()
 
 
 setup(
     name='pybw_comic',
-    version='23.7.2.1',
+    version='23.7.2.2',
     python_requires='>=3.6',
     
     author='Bowei Pu',
     author_email='pubowei@foxmail.com',
     
     description='comic spider',
     long_description=readme,
```

