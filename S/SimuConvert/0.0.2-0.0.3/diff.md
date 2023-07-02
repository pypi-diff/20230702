# Comparing `tmp/SimuConvert-0.0.2.tar.gz` & `tmp/SimuConvert-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SimuConvert-0.0.2.tar", last modified: Sun Jul  2 12:45:04 2023, max compression
+gzip compressed data, was "SimuConvert-0.0.3.tar", last modified: Sun Jul  2 13:45:52 2023, max compression
```

## Comparing `SimuConvert-0.0.2.tar` & `SimuConvert-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 yanzhonghuang   (501) staff       (20)        0 2023-07-02 12:45:04.530074 SimuConvert-0.0.2/
--rw-r--r--   0 yanzhonghuang   (501) staff       (20)     1071 2023-07-01 08:02:44.000000 SimuConvert-0.0.2/LICENSE
--rw-r--r--   0 yanzhonghuang   (501) staff       (20)      932 2023-07-02 12:45:04.529940 SimuConvert-0.0.2/PKG-INFO
--rw-r--r--   0 yanzhonghuang   (501) staff       (20)      480 2023-07-01 08:55:36.000000 SimuConvert-0.0.2/README.md
-drwxr-xr-x   0 yanzhonghuang   (501) staff       (20)        0 2023-07-02 12:45:04.528961 SimuConvert-0.0.2/SimuConvert/
--rw-r--r--   0 yanzhonghuang   (501) staff       (20)       32 2023-07-01 09:02:59.000000 SimuConvert-0.0.2/SimuConvert/__init__.py
--rw-r--r--   0 yanzhonghuang   (501) staff       (20)     2359 2023-07-01 09:02:06.000000 SimuConvert-0.0.2/SimuConvert/zuhedashi_convert.py
-drwxr-xr-x   0 yanzhonghuang   (501) staff       (20)        0 2023-07-02 12:45:04.529707 SimuConvert-0.0.2/SimuConvert.egg-info/
--rw-r--r--   0 yanzhonghuang   (501) staff       (20)      932 2023-07-02 12:45:04.000000 SimuConvert-0.0.2/SimuConvert.egg-info/PKG-INFO
--rw-r--r--   0 yanzhonghuang   (501) staff       (20)      257 2023-07-02 12:45:04.000000 SimuConvert-0.0.2/SimuConvert.egg-info/SOURCES.txt
--rw-r--r--   0 yanzhonghuang   (501) staff       (20)        1 2023-07-02 12:45:04.000000 SimuConvert-0.0.2/SimuConvert.egg-info/dependency_links.txt
--rw-r--r--   0 yanzhonghuang   (501) staff       (20)       62 2023-07-02 12:45:04.000000 SimuConvert-0.0.2/SimuConvert.egg-info/requires.txt
--rw-r--r--   0 yanzhonghuang   (501) staff       (20)       12 2023-07-02 12:45:04.000000 SimuConvert-0.0.2/SimuConvert.egg-info/top_level.txt
--rw-r--r--   0 yanzhonghuang   (501) staff       (20)       38 2023-07-02 12:45:04.530123 SimuConvert-0.0.2/setup.cfg
--rw-r--r--   0 yanzhonghuang   (501) staff       (20)      851 2023-07-02 12:44:16.000000 SimuConvert-0.0.2/setup.py
+drwxr-xr-x   0 yanzhonghuang   (501) staff       (20)        0 2023-07-02 13:45:52.202401 SimuConvert-0.0.3/
+-rw-r--r--   0 yanzhonghuang   (501) staff       (20)     1071 2023-07-01 08:02:44.000000 SimuConvert-0.0.3/LICENSE
+-rw-r--r--   0 yanzhonghuang   (501) staff       (20)      932 2023-07-02 13:45:52.202275 SimuConvert-0.0.3/PKG-INFO
+-rw-r--r--   0 yanzhonghuang   (501) staff       (20)      480 2023-07-01 08:55:36.000000 SimuConvert-0.0.3/README.md
+drwxr-xr-x   0 yanzhonghuang   (501) staff       (20)        0 2023-07-02 13:45:52.201480 SimuConvert-0.0.3/SimuConvert/
+-rw-r--r--   0 yanzhonghuang   (501) staff       (20)       32 2023-07-01 09:02:59.000000 SimuConvert-0.0.3/SimuConvert/__init__.py
+-rw-r--r--   0 yanzhonghuang   (501) staff       (20)     2420 2023-07-02 13:45:33.000000 SimuConvert-0.0.3/SimuConvert/zuhedashi_convert.py
+drwxr-xr-x   0 yanzhonghuang   (501) staff       (20)        0 2023-07-02 13:45:52.202103 SimuConvert-0.0.3/SimuConvert.egg-info/
+-rw-r--r--   0 yanzhonghuang   (501) staff       (20)      932 2023-07-02 13:45:52.000000 SimuConvert-0.0.3/SimuConvert.egg-info/PKG-INFO
+-rw-r--r--   0 yanzhonghuang   (501) staff       (20)      257 2023-07-02 13:45:52.000000 SimuConvert-0.0.3/SimuConvert.egg-info/SOURCES.txt
+-rw-r--r--   0 yanzhonghuang   (501) staff       (20)        1 2023-07-02 13:45:52.000000 SimuConvert-0.0.3/SimuConvert.egg-info/dependency_links.txt
+-rw-r--r--   0 yanzhonghuang   (501) staff       (20)       62 2023-07-02 13:45:52.000000 SimuConvert-0.0.3/SimuConvert.egg-info/requires.txt
+-rw-r--r--   0 yanzhonghuang   (501) staff       (20)       12 2023-07-02 13:45:52.000000 SimuConvert-0.0.3/SimuConvert.egg-info/top_level.txt
+-rw-r--r--   0 yanzhonghuang   (501) staff       (20)       38 2023-07-02 13:45:52.202435 SimuConvert-0.0.3/setup.cfg
+-rw-r--r--   0 yanzhonghuang   (501) staff       (20)      851 2023-07-02 13:44:06.000000 SimuConvert-0.0.3/setup.py
```

### Comparing `SimuConvert-0.0.2/LICENSE` & `SimuConvert-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `SimuConvert-0.0.2/PKG-INFO` & `SimuConvert-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimuConvert
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package for converting private fund equity data 
 Home-page: https://github.com/Yanzhong-Hub/SimuConvert
 Author: Yanzhong Huang
 Author-email: yanzhong.huang@outlook.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `SimuConvert-0.0.2/SimuConvert/zuhedashi_convert.py` & `SimuConvert-0.0.3/SimuConvert/zuhedashi_convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     raw_data = _read_simupaipai_csv(path)
     
     # 分为每三列为一组，数据为一个基金
     funds: list[pd.DataFrame] = []
     for i in range(0, len(raw_data.columns), 3):
         df = raw_data.iloc[:, i:i+3].copy()
         fund_name = df.columns[0]
+        df.dropna(inplace=True)  # type: ignore 删除空行
         df.columns = ['nav', 'nav_adj', 'nav_acc']  # 重命名列名        
         df['fund_name'] = fund_name  # 增加基金名称列
         funds.append(df)
     funds_df = pd.concat(funds, axis=0)  # type: ignore
     funds_df.index.name = 'trade_date'
     funds_df.reset_index(inplace=True)
     funds_df.index.name = 'id'
```

### Comparing `SimuConvert-0.0.2/SimuConvert.egg-info/PKG-INFO` & `SimuConvert-0.0.3/SimuConvert.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimuConvert
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package for converting private fund equity data 
 Home-page: https://github.com/Yanzhong-Hub/SimuConvert
 Author: Yanzhong Huang
 Author-email: yanzhong.huang@outlook.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `SimuConvert-0.0.2/setup.py` & `SimuConvert-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="SimuConvert",
-    version="0.0.2",
+    version="0.0.3",
     author="Yanzhong Huang",
     author_email="yanzhong.huang@outlook.com",
     description="A package for converting private fund equity data ",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Yanzhong-Hub/SimuConvert",
     packages=find_packages(),
```

