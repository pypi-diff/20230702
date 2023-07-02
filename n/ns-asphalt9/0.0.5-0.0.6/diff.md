# Comparing `tmp/ns_asphalt9-0.0.5.tar.gz` & `tmp/ns_asphalt9-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ns_asphalt9-0.0.5.tar", last modified: Sun Jul  2 12:38:46 2023, max compression
+gzip compressed data, was "dist/ns_asphalt9-0.0.6.tar", last modified: Sun Jul  2 12:58:57 2023, max compression
```

## Comparing `ns_asphalt9-0.0.5.tar` & `ns_asphalt9-0.0.6.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-02 12:38:46.000000 ns_asphalt9-0.0.5/
--rw-r--r--   0 sunhao     (501) staff       (20)    35149 2023-04-09 01:28:45.000000 ns_asphalt9-0.0.5/LICENSE
--rw-r--r--   0 sunhao     (501) staff       (20)      180 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.5/MANIFEST.in
--rw-r--r--   0 sunhao     (501) staff       (20)     2276 2023-07-02 12:38:46.000000 ns_asphalt9-0.0.5/PKG-INFO
--rw-r--r--   0 sunhao     (501) staff       (20)     1041 2023-05-15 13:28:06.000000 ns_asphalt9-0.0.5/README.md
-drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-02 12:38:46.000000 ns_asphalt9-0.0.5/ns_asphalt9/
-drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-02 12:38:46.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/
--rw-r--r--   0 sunhao     (501) staff       (20)       20 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/__init__.py
-drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-02 12:38:46.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/actions/
--rw-r--r--   0 sunhao     (501) staff       (20)      208 2023-07-02 11:42:33.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/actions/__init__.py
--rw-r--r--   0 sunhao     (501) staff       (20)      336 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/actions/common.py
--rw-r--r--   0 sunhao     (501) staff       (20)     4033 2023-07-02 12:16:45.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/actions/enter_page.py
--rw-r--r--   0 sunhao     (501) staff       (20)     3881 2023-07-02 05:05:14.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/actions/process_race.py
--rw-r--r--   0 sunhao     (501) staff       (20)     3777 2023-07-02 02:37:32.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/actions/select_car.py
--rw-r--r--   0 sunhao     (501) staff       (20)      706 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/cache.py
--rw-r--r--   0 sunhao     (501) staff       (20)     2996 2023-07-02 12:30:27.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/consts.py
--rw-r--r--   0 sunhao     (501) staff       (20)     2146 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/controller.py
--rw-r--r--   0 sunhao     (501) staff       (20)      634 2023-07-02 02:35:24.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/globals.py
-drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-02 12:38:46.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/gui/
--rw-r--r--   0 sunhao     (501) staff       (20)        0 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/gui/__init__.py
--rw-r--r--   0 sunhao     (501) staff       (20)    18706 2023-07-02 12:06:23.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/gui/app.py
-drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-02 12:38:46.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/gui/images/
--rw-r--r--   0 sunhao     (501) staff       (20)     3097 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/gui/images/help.png
--rw-r--r--   0 sunhao     (501) staff       (20)     2900 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/gui/images/home.png
--rw-r--r--   0 sunhao     (501) staff       (20)   202347 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/gui/images/logo.png
--rw-r--r--   0 sunhao     (501) staff       (20)     3159 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/gui/images/settings.png
--rw-r--r--   0 sunhao     (501) staff       (20)     1530 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/ocr.py
--rw-r--r--   0 sunhao     (501) staff       (20)     1841 2023-07-01 12:06:18.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/page_factory.py
--rw-r--r--   0 sunhao     (501) staff       (20)    12155 2023-07-02 12:33:09.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/pages.py
--rw-r--r--   0 sunhao     (501) staff       (20)      265 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/screenshot.py
--rw-r--r--   0 sunhao     (501) staff       (20)     2572 2023-07-02 12:33:50.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/tasks.py
-drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-02 12:38:46.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/utils/
--rw-r--r--   0 sunhao     (501) staff       (20)        0 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/utils/__init__.py
--rw-r--r--   0 sunhao     (501) staff       (20)     1016 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/utils/decorator.py
--rw-r--r--   0 sunhao     (501) staff       (20)      459 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/utils/fetch_cars.py
--rw-r--r--   0 sunhao     (501) staff       (20)     1993 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/utils/log.py
--rw-r--r--   0 sunhao     (501) staff       (20)      862 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/utils/timer.py
--rw-r--r--   0 sunhao     (501) staff       (20)     5558 2023-07-02 12:12:57.000000 ns_asphalt9-0.0.5/ns_asphalt9/main.py
-drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-02 12:38:46.000000 ns_asphalt9-0.0.5/ns_asphalt9.egg-info/
--rw-r--r--   0 sunhao     (501) staff       (20)     2276 2023-07-02 12:38:46.000000 ns_asphalt9-0.0.5/ns_asphalt9.egg-info/PKG-INFO
--rw-r--r--   0 sunhao     (501) staff       (20)     1169 2023-07-02 12:38:46.000000 ns_asphalt9-0.0.5/ns_asphalt9.egg-info/SOURCES.txt
--rw-r--r--   0 sunhao     (501) staff       (20)        1 2023-07-02 12:38:46.000000 ns_asphalt9-0.0.5/ns_asphalt9.egg-info/dependency_links.txt
--rw-r--r--   0 sunhao     (501) staff       (20)       55 2023-07-02 12:38:46.000000 ns_asphalt9-0.0.5/ns_asphalt9.egg-info/entry_points.txt
--rw-r--r--   0 sunhao     (501) staff       (20)        1 2023-07-02 12:38:46.000000 ns_asphalt9-0.0.5/ns_asphalt9.egg-info/not-zip-safe
--rw-r--r--   0 sunhao     (501) staff       (20)      107 2023-07-02 12:38:46.000000 ns_asphalt9-0.0.5/ns_asphalt9.egg-info/requires.txt
--rw-r--r--   0 sunhao     (501) staff       (20)       12 2023-07-02 12:38:46.000000 ns_asphalt9-0.0.5/ns_asphalt9.egg-info/top_level.txt
--rw-r--r--   0 sunhao     (501) staff       (20)     1299 2023-07-02 12:38:46.000000 ns_asphalt9-0.0.5/setup.cfg
--rw-r--r--   0 sunhao     (501) staff       (20)      387 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.5/setup.py
+drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-02 12:58:57.000000 ns_asphalt9-0.0.6/
+-rw-r--r--   0 sunhao     (501) staff       (20)    35149 2023-04-09 01:28:45.000000 ns_asphalt9-0.0.6/LICENSE
+-rw-r--r--   0 sunhao     (501) staff       (20)      180 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.6/MANIFEST.in
+-rw-r--r--   0 sunhao     (501) staff       (20)     2276 2023-07-02 12:58:57.000000 ns_asphalt9-0.0.6/PKG-INFO
+-rw-r--r--   0 sunhao     (501) staff       (20)     1041 2023-05-15 13:28:06.000000 ns_asphalt9-0.0.6/README.md
+drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-02 12:58:56.000000 ns_asphalt9-0.0.6/ns_asphalt9/
+drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-02 12:58:56.000000 ns_asphalt9-0.0.6/ns_asphalt9/core/
+-rw-r--r--   0 sunhao     (501) staff       (20)       20 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.6/ns_asphalt9/core/__init__.py
+drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-02 12:58:57.000000 ns_asphalt9-0.0.6/ns_asphalt9/core/actions/
+-rw-r--r--   0 sunhao     (501) staff       (20)      208 2023-07-02 11:42:33.000000 ns_asphalt9-0.0.6/ns_asphalt9/core/actions/__init__.py
+-rw-r--r--   0 sunhao     (501) staff       (20)      336 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.6/ns_asphalt9/core/actions/common.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     4033 2023-07-02 12:16:45.000000 ns_asphalt9-0.0.6/ns_asphalt9/core/actions/enter_page.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     3917 2023-07-02 12:56:49.000000 ns_asphalt9-0.0.6/ns_asphalt9/core/actions/process_race.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     3777 2023-07-02 02:37:32.000000 ns_asphalt9-0.0.6/ns_asphalt9/core/actions/select_car.py
+-rw-r--r--   0 sunhao     (501) staff       (20)      706 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.6/ns_asphalt9/core/cache.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     2996 2023-07-02 12:30:27.000000 ns_asphalt9-0.0.6/ns_asphalt9/core/consts.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     2146 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.6/ns_asphalt9/core/controller.py
+-rw-r--r--   0 sunhao     (501) staff       (20)      634 2023-07-02 02:35:24.000000 ns_asphalt9-0.0.6/ns_asphalt9/core/globals.py
+drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-02 12:58:57.000000 ns_asphalt9-0.0.6/ns_asphalt9/core/gui/
+-rw-r--r--   0 sunhao     (501) staff       (20)        0 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.6/ns_asphalt9/core/gui/__init__.py
+-rw-r--r--   0 sunhao     (501) staff       (20)    18706 2023-07-02 12:06:23.000000 ns_asphalt9-0.0.6/ns_asphalt9/core/gui/app.py
+drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-02 12:58:57.000000 ns_asphalt9-0.0.6/ns_asphalt9/core/gui/images/
+-rw-r--r--   0 sunhao     (501) staff       (20)     3097 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.6/ns_asphalt9/core/gui/images/help.png
+-rw-r--r--   0 sunhao     (501) staff       (20)     2900 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.6/ns_asphalt9/core/gui/images/home.png
+-rw-r--r--   0 sunhao     (501) staff       (20)   202347 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.6/ns_asphalt9/core/gui/images/logo.png
+-rw-r--r--   0 sunhao     (501) staff       (20)     3159 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.6/ns_asphalt9/core/gui/images/settings.png
+-rw-r--r--   0 sunhao     (501) staff       (20)     1530 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.6/ns_asphalt9/core/ocr.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     1841 2023-07-01 12:06:18.000000 ns_asphalt9-0.0.6/ns_asphalt9/core/page_factory.py
+-rw-r--r--   0 sunhao     (501) staff       (20)    12155 2023-07-02 12:33:09.000000 ns_asphalt9-0.0.6/ns_asphalt9/core/pages.py
+-rw-r--r--   0 sunhao     (501) staff       (20)      265 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.6/ns_asphalt9/core/screenshot.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     2572 2023-07-02 12:33:50.000000 ns_asphalt9-0.0.6/ns_asphalt9/core/tasks.py
+drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-02 12:58:57.000000 ns_asphalt9-0.0.6/ns_asphalt9/core/utils/
+-rw-r--r--   0 sunhao     (501) staff       (20)        0 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.6/ns_asphalt9/core/utils/__init__.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     1016 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.6/ns_asphalt9/core/utils/decorator.py
+-rw-r--r--   0 sunhao     (501) staff       (20)      459 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.6/ns_asphalt9/core/utils/fetch_cars.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     1993 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.6/ns_asphalt9/core/utils/log.py
+-rw-r--r--   0 sunhao     (501) staff       (20)      862 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.6/ns_asphalt9/core/utils/timer.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     5558 2023-07-02 12:12:57.000000 ns_asphalt9-0.0.6/ns_asphalt9/main.py
+drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-02 12:58:56.000000 ns_asphalt9-0.0.6/ns_asphalt9.egg-info/
+-rw-r--r--   0 sunhao     (501) staff       (20)     2276 2023-07-02 12:58:56.000000 ns_asphalt9-0.0.6/ns_asphalt9.egg-info/PKG-INFO
+-rw-r--r--   0 sunhao     (501) staff       (20)     1169 2023-07-02 12:58:56.000000 ns_asphalt9-0.0.6/ns_asphalt9.egg-info/SOURCES.txt
+-rw-r--r--   0 sunhao     (501) staff       (20)        1 2023-07-02 12:58:56.000000 ns_asphalt9-0.0.6/ns_asphalt9.egg-info/dependency_links.txt
+-rw-r--r--   0 sunhao     (501) staff       (20)       55 2023-07-02 12:58:56.000000 ns_asphalt9-0.0.6/ns_asphalt9.egg-info/entry_points.txt
+-rw-r--r--   0 sunhao     (501) staff       (20)        1 2023-07-02 12:38:46.000000 ns_asphalt9-0.0.6/ns_asphalt9.egg-info/not-zip-safe
+-rw-r--r--   0 sunhao     (501) staff       (20)      107 2023-07-02 12:58:56.000000 ns_asphalt9-0.0.6/ns_asphalt9.egg-info/requires.txt
+-rw-r--r--   0 sunhao     (501) staff       (20)       12 2023-07-02 12:58:56.000000 ns_asphalt9-0.0.6/ns_asphalt9.egg-info/top_level.txt
+-rw-r--r--   0 sunhao     (501) staff       (20)     1299 2023-07-02 12:58:57.000000 ns_asphalt9-0.0.6/setup.cfg
+-rw-r--r--   0 sunhao     (501) staff       (20)      387 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.6/setup.py
```

### Comparing `ns_asphalt9-0.0.5/LICENSE` & `ns_asphalt9-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.5/PKG-INFO` & `ns_asphalt9-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ns_asphalt9
-Version: 0.0.5
+Version: 0.0.6
 Summary: Asphalt 9 daily task handling tool based on NXBT and V4L2.
 Home-page: https://pypi.python.org/pypi/ns_asphalt9
 Author: codehai
 Author-email: wmpksb@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Code, https://github.com/codehai/ns_asphalt9
 Project-URL: Issue tracker, https://github.com/codehai/ns_asphalt9/issues
```

### Comparing `ns_asphalt9-0.0.5/README.md` & `ns_asphalt9-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.5/ns_asphalt9/core/actions/enter_page.py` & `ns_asphalt9-0.0.6/ns_asphalt9/core/actions/enter_page.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.5/ns_asphalt9/core/actions/process_race.py` & `ns_asphalt9-0.0.6/ns_asphalt9/core/actions/process_race.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
                         break
                     elif elapsed > 24 and elapsed < 43 or elapsed < 10:
                         pro.press_button(Buttons.Y, 0.7)
                         pro.press_button(Buttons.Y, 0)
                         time.sleep(3)
                     else:
                         time.sleep(0.5)
-        elif page.hunt_car == "APEX AP-0":
+        elif page.hunt_car == "APEX AP-0" and page.mode == consts.car_hunt_zh:
             if progress > 0:
                 start = time.perf_counter()
                 delta = progress * 0.55 + 4.5
                 while globals.G_RUN.is_set():
                     end = time.perf_counter()
                     elapsed = end - start + delta
                     logger.info(f"elapsed = {elapsed}")
```

### Comparing `ns_asphalt9-0.0.5/ns_asphalt9/core/actions/select_car.py` & `ns_asphalt9-0.0.6/ns_asphalt9/core/actions/select_car.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.5/ns_asphalt9/core/cache.py` & `ns_asphalt9-0.0.6/ns_asphalt9/core/cache.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.5/ns_asphalt9/core/consts.py` & `ns_asphalt9-0.0.6/ns_asphalt9/core/consts.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.5/ns_asphalt9/core/controller.py` & `ns_asphalt9-0.0.6/ns_asphalt9/core/controller.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.5/ns_asphalt9/core/globals.py` & `ns_asphalt9-0.0.6/ns_asphalt9/core/globals.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.5/ns_asphalt9/core/gui/app.py` & `ns_asphalt9-0.0.6/ns_asphalt9/core/gui/app.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.5/ns_asphalt9/core/gui/images/help.png` & `ns_asphalt9-0.0.6/ns_asphalt9/core/gui/images/help.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.5/ns_asphalt9/core/gui/images/home.png` & `ns_asphalt9-0.0.6/ns_asphalt9/core/gui/images/home.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.5/ns_asphalt9/core/gui/images/logo.png` & `ns_asphalt9-0.0.6/ns_asphalt9/core/gui/images/logo.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.5/ns_asphalt9/core/gui/images/settings.png` & `ns_asphalt9-0.0.6/ns_asphalt9/core/gui/images/settings.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.5/ns_asphalt9/core/ocr.py` & `ns_asphalt9-0.0.6/ns_asphalt9/core/ocr.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.5/ns_asphalt9/core/page_factory.py` & `ns_asphalt9-0.0.6/ns_asphalt9/core/page_factory.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.5/ns_asphalt9/core/pages.py` & `ns_asphalt9-0.0.6/ns_asphalt9/core/pages.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.5/ns_asphalt9/core/tasks.py` & `ns_asphalt9-0.0.6/ns_asphalt9/core/tasks.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.5/ns_asphalt9/core/utils/decorator.py` & `ns_asphalt9-0.0.6/ns_asphalt9/core/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.5/ns_asphalt9/core/utils/log.py` & `ns_asphalt9-0.0.6/ns_asphalt9/core/utils/log.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.5/ns_asphalt9/core/utils/timer.py` & `ns_asphalt9-0.0.6/ns_asphalt9/core/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.5/ns_asphalt9/main.py` & `ns_asphalt9-0.0.6/ns_asphalt9/main.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.5/ns_asphalt9.egg-info/PKG-INFO` & `ns_asphalt9-0.0.6/ns_asphalt9.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ns-asphalt9
-Version: 0.0.5
+Version: 0.0.6
 Summary: Asphalt 9 daily task handling tool based on NXBT and V4L2.
 Home-page: https://pypi.python.org/pypi/ns_asphalt9
 Author: codehai
 Author-email: wmpksb@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Code, https://github.com/codehai/ns_asphalt9
 Project-URL: Issue tracker, https://github.com/codehai/ns_asphalt9/issues
```

### Comparing `ns_asphalt9-0.0.5/ns_asphalt9.egg-info/SOURCES.txt` & `ns_asphalt9-0.0.6/ns_asphalt9.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.5/setup.cfg` & `ns_asphalt9-0.0.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nxbt
-version = 0.0.5
+version = 0.0.6
 author = codehai
 author-email = wmpksb@gmail.com
 project_urls = 
 	Code = https://github.com/codehai/ns_asphalt9
 	Issue tracker = https://github.com/codehai/ns_asphalt9/issues
 license = GNU General Public License v3 (GPLv3)
 license-file = LICENSE
```

