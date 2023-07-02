# Comparing `tmp/SiteScraper-2.3.2.tar.gz` & `tmp/SiteScraper-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SiteScraper-2.3.2.tar", last modified: Sun Jul  2 08:25:36 2023, max compression
+gzip compressed data, was "SiteScraper-2.3.3.tar", last modified: Sun Jul  2 08:28:53 2023, max compression
```

## Comparing `SiteScraper-2.3.2.tar` & `SiteScraper-2.3.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 08:25:36.217382 SiteScraper-2.3.2/
--rw-rw-rw-   0        0        0     3989 2023-07-02 08:25:36.217382 SiteScraper-2.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     3760 2023-05-25 09:12:48.000000 SiteScraper-2.3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-02 08:25:36.209963 SiteScraper-2.3.2/SiteScraper/
--rw-rw-rw-   0        0        0    11218 2023-07-02 08:25:07.000000 SiteScraper-2.3.2/SiteScraper/SiteScraper.py
--rw-rw-rw-   0        0        0       46 2023-05-25 10:05:57.000000 SiteScraper-2.3.2/SiteScraper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-02 08:25:36.215864 SiteScraper-2.3.2/SiteScraper.egg-info/
--rw-rw-rw-   0        0        0     3989 2023-07-02 08:25:36.000000 SiteScraper-2.3.2/SiteScraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-07-02 08:25:36.000000 SiteScraper-2.3.2/SiteScraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 08:25:36.000000 SiteScraper-2.3.2/SiteScraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-02 08:25:36.000000 SiteScraper-2.3.2/SiteScraper.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-07-02 08:25:36.000000 SiteScraper-2.3.2/SiteScraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-02 08:25:36.000000 SiteScraper-2.3.2/SiteScraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      626 2023-05-25 07:53:45.000000 SiteScraper-2.3.2/licence.txt
--rw-rw-rw-   0        0        0      158 2023-07-02 08:25:36.219730 SiteScraper-2.3.2/setup.cfg
--rw-rw-rw-   0        0        0      497 2023-07-02 08:24:45.000000 SiteScraper-2.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 08:28:53.951607 SiteScraper-2.3.3/
+-rw-rw-rw-   0        0        0     3989 2023-07-02 08:28:53.952604 SiteScraper-2.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3760 2023-05-25 09:12:48.000000 SiteScraper-2.3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-02 08:28:53.942850 SiteScraper-2.3.3/SiteScraper/
+-rw-rw-rw-   0        0        0    11128 2023-07-02 08:28:31.000000 SiteScraper-2.3.3/SiteScraper/SiteScraper.py
+-rw-rw-rw-   0        0        0       46 2023-05-25 10:05:57.000000 SiteScraper-2.3.3/SiteScraper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-02 08:28:53.951607 SiteScraper-2.3.3/SiteScraper.egg-info/
+-rw-rw-rw-   0        0        0     3989 2023-07-02 08:28:53.000000 SiteScraper-2.3.3/SiteScraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-07-02 08:28:53.000000 SiteScraper-2.3.3/SiteScraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 08:28:53.000000 SiteScraper-2.3.3/SiteScraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-02 08:28:53.000000 SiteScraper-2.3.3/SiteScraper.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-07-02 08:28:53.000000 SiteScraper-2.3.3/SiteScraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-02 08:28:53.000000 SiteScraper-2.3.3/SiteScraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      626 2023-05-25 07:53:45.000000 SiteScraper-2.3.3/licence.txt
+-rw-rw-rw-   0        0        0      158 2023-07-02 08:28:53.953609 SiteScraper-2.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      497 2023-07-02 08:28:42.000000 SiteScraper-2.3.3/setup.py
```

### Comparing `SiteScraper-2.3.2/PKG-INFO` & `SiteScraper-2.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SiteScraper
-Version: 2.3.2
+Version: 2.3.3
 Summary: Scraping high intensity content sites
 Author: Ibrahim
 Author-email: string2025@gmail.com
 Description-Content-Type: text/markdown
 License-File: licence.txt
 
 # SiteScraper
```

### Comparing `SiteScraper-2.3.2/README.md` & `SiteScraper-2.3.3/README.md`

 * *Files identical despite different names*

### Comparing `SiteScraper-2.3.2/SiteScraper/SiteScraper.py` & `SiteScraper-2.3.3/SiteScraper/SiteScraper.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,13 +226,10 @@
                             else:
                                 counter=0
 
             
             links = driver.find_elements(By.XPATH, '//*[@id="video-title-link"]')
             vedio_links = [link.get_attribute('href') for link in links]
             return vedio_links
-        except Exception as e:
-            logging.error('Error: {}'.format(str(e)))
-        
-        finally:
-            if 'driver' in locals():
+        except:
                 driver.quit()
+                logging.error('Invalid url')
```

### Comparing `SiteScraper-2.3.2/SiteScraper.egg-info/PKG-INFO` & `SiteScraper-2.3.3/SiteScraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SiteScraper
-Version: 2.3.2
+Version: 2.3.3
 Summary: Scraping high intensity content sites
 Author: Ibrahim
 Author-email: string2025@gmail.com
 Description-Content-Type: text/markdown
 License-File: licence.txt
 
 # SiteScraper
```

### Comparing `SiteScraper-2.3.2/licence.txt` & `SiteScraper-2.3.3/licence.txt`

 * *Files identical despite different names*

