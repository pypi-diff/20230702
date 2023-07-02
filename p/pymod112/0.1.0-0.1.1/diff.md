# Comparing `tmp/pymod112-0.1.0.tar.gz` & `tmp/pymod112-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymod112-0.1.0.tar", last modified: Sat Jun 24 04:44:23 2023, max compression
+gzip compressed data, was "pymod112-0.1.1.tar", last modified: Sun Jul  2 03:29:15 2023, max compression
```

## Comparing `pymod112-0.1.0.tar` & `pymod112-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 04:44:23.537482 pymod112-0.1.0/
--rw-rw-rw-   0        0        0     1535 2023-06-24 01:55:06.000000 pymod112-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     1341 2023-06-24 04:44:23.536482 pymod112-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      801 2023-06-24 03:06:42.000000 pymod112-0.1.0/README.md
--rw-rw-rw-   0        0        0      622 2023-06-24 04:44:03.000000 pymod112-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-24 04:44:23.537482 pymod112-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-24 04:44:23.511450 pymod112-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-24 04:44:23.529482 pymod112-0.1.0/src/pymod112/
--rw-rw-rw-   0        0        0      193 2023-06-24 02:40:54.000000 pymod112-0.1.0/src/pymod112/__init__.py
--rw-rw-rw-   0        0        0     7067 2023-06-24 04:11:34.000000 pymod112-0.1.0/src/pymod112/mod112.py
-drwxrwxrwx   0        0        0        0 2023-06-24 04:44:23.535482 pymod112-0.1.0/src/pymod112.egg-info/
--rw-rw-rw-   0        0        0     1341 2023-06-24 04:44:23.000000 pymod112-0.1.0/src/pymod112.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-06-24 04:44:23.000000 pymod112-0.1.0/src/pymod112.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 04:44:23.000000 pymod112-0.1.0/src/pymod112.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-24 04:44:23.000000 pymod112-0.1.0/src/pymod112.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-02 03:29:15.284884 pymod112-0.1.1/
+-rw-rw-rw-   0        0        0     1535 2023-06-24 01:55:06.000000 pymod112-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1996 2023-07-02 03:29:15.284884 pymod112-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1456 2023-07-02 03:24:34.000000 pymod112-0.1.1/README.md
+-rw-rw-rw-   0        0        0      622 2023-07-02 03:28:24.000000 pymod112-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-02 03:29:15.285884 pymod112-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-02 03:29:15.267883 pymod112-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-02 03:29:15.275883 pymod112-0.1.1/src/pymod112/
+-rw-rw-rw-   0        0        0      214 2023-07-02 03:26:32.000000 pymod112-0.1.1/src/pymod112/__init__.py
+-rw-rw-rw-   0        0        0     7198 2023-07-02 03:27:48.000000 pymod112-0.1.1/src/pymod112/mod112.py
+drwxrwxrwx   0        0        0        0 2023-07-02 03:29:15.281883 pymod112-0.1.1/src/pymod112.egg-info/
+-rw-rw-rw-   0        0        0     1996 2023-07-02 03:29:15.000000 pymod112-0.1.1/src/pymod112.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-07-02 03:29:15.000000 pymod112-0.1.1/src/pymod112.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 03:29:15.000000 pymod112-0.1.1/src/pymod112.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-02 03:29:15.000000 pymod112-0.1.1/src/pymod112.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-02 03:29:15.283883 pymod112-0.1.1/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-27 15:26:13.000000 pymod112-0.1.1/tests/test_basic.py
```

### Comparing `pymod112-0.1.0/LICENSE` & `pymod112-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymod112-0.1.0/PKG-INFO` & `pymod112-0.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymod112
-Version: 0.1.0
+Version: 0.1.1
 Summary: 一个可以离线检验公民身份号码是否合法的程序
 Author-email: HoshsL <HoshsL@outlook.com>
 Project-URL: Homepage, https://gitee.com/HoshsL/PyMOD11-2
 Project-URL: Bug Tracker, https://gitee.com/HoshsL/PyMOD11-2/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -14,23 +14,23 @@
 
 # pymod112
 
 一个基于Python开发的公民身份号码检验与地区代码查找程序
 
 ## 安装 Installation
 
-使用pip安装
+[PyPi](https://pypi.org/project/pymod112/) 使用pip安装
 
 ```sh
 pip install pymod112
 ```
 
 ## 使用 Usage
 
-基础使用
+身份证号码校验
 
 ```python
 import pymod112
 
 pymod112.mod112('11010519491231002X', details=True)
 '''返回值为(dict)
 {'id': '11010519491231002X', 
@@ -41,20 +41,49 @@
  'gender': 0, 
  'result': True, 
  'problem': '000'}
 '''
 
 ```
 
-拓展功能(查询地区代码对应的地区名)
+查询地区代码对应的地区名
 
 ```python
 import pymod112
 
 pymod112.code_to_location(['51', '01', '06'])
 '''返回值为(list)
 ['四川省', '成都市', '金牛区']
 '''
 ```
 
+返回全部错误代码及其对应内容
+
+```python
+import pymod112
+
+pymod112.code_to_error
+'''dict
+{'000':'不存在问题',
+'001':'<未定义>',
+'002':'<未定义>',
+'003':'<未定义>',
+'004':'参数id长度错误',
+'005':'参数id内容包含非法字符',
+'006':'参数id不合法',
+'007':'参数id中包含不存在的地区',
+'008':'参数id中包含不存在的时间'
+}
+'''
+```
+
 ## 许可证 License
 BSD 3-Clause License
+
+## 更新日志 Changelog
+### **0.1.1**
+ - 加入参数类型检查
+ - 优化错误代码（停用001 002 003）
+ - 删除函数problem()
+
+### **0.1.0(2023-6-24)**
+- 这是第一个正式发行版
```

### Comparing `pymod112-0.1.0/pyproject.toml` & `pymod112-0.1.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pymod112"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="HoshsL", email="HoshsL@outlook.com" },
 ]
 description = "一个可以离线检验公民身份号码是否合法的程序"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pymod112-0.1.0/src/pymod112/mod112.py` & `pymod112-0.1.1/src/pymod112/mod112.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import pickle
 import time
 import os
 
-problem_and_code = {'000':'不存在问题',
-                    '001':'参数id类型错误',
-                    '002':'参数time_check类型错误',
-                    '003':'参数details类型错误',
-                    '004':'参数id长度错误',
-                    '005':'参数id内容包含非法字符错误',
-                    '006':'参数id不合法',
-                    '007':'参数id中包含不存在的地区',
-                    '008':'参数id中包含不存在的时间'
-                    }
+code_to_error = {'000':'不存在问题',
+                   '001':'<未定义>',
+                   '002':'<未定义>',
+                   '003':'<未定义>',
+                   '004':'参数id长度错误',
+                   '005':'参数id内容包含非法字符',
+                   '006':'参数id不合法',
+                   '007':'参数id中包含不存在的地区',
+                   '008':'参数id中包含不存在的时间'
+                   }
 
 def code_to_location(code: list|tuple) -> list:
     '''
     通过中华人民共和国县以上行政区划代码获取对应单位名称(地方名称)\n
     数据来自《2020年12月中华人民共和国县以上行政区划代码》\n
     注：暂无三沙市西沙区和三沙市南沙区代码)\n
     \n
@@ -24,27 +24,28 @@
     例：'410102'则传入['41', '01', '02']\n
     输出\n
     list -> [<省>, <市>, <县>]\n
     注：不存在地区的返回值为空字符串\n
     '''
 
     # 参数检查
-    ...
+    if not isinstance(code, (list, tuple)):
+        raise TypeError('"code" should be a list or tuple')
 
     # 查询
     workplace = os.getcwd()
     os.chdir(os.path.dirname(__file__))
     with open('./RegionCode', 'rb') as f:
         region_code: dict = pickle.load(f)  # 例{code:name}
     result = [region_code.get(f'{code[0]}0000', ''), 
               region_code.get(f'{code[0]}{code[1]}00', ''), 
               region_code.get(f'{code[0]}{code[1]}{code[2]}', '')]
     os.chdir(workplace)
     return result
-            
+     
 def mod112(id: str, time_check: bool=True, details: bool=False) -> bool|dict:
     """
     检验传入的ID是否是符合规范的中华人民共和国公民身份号码。\n
     该检验无法接入公安系统故无法检验传入的ID是否真实存在。\n
     \n
     参数\n
     id: str -> 传入内容即为需要检验的ID，最后一位自动忽略大小写\n
@@ -58,60 +59,59 @@
              'county':[<编号:int>, <名称:str>],\n
              'birth_date':[<年:int>, <月:int>, <日:int>],\n
              'gender':<性别:int>,\n
              'result':<检验结果:bool>,\n
              'problem':<问题代码:str>}\n
     注0：不存在的会用空字符串代替\n
     注1：'gender'中1指代男性 0指代女性\n
-    注2：获取问题详情请使用problem(code=<问题代码:str>)\n
-    注3：问题代码为'000'时表示不存在问题\n
+    注2：问题代码为'000'时表示不存在问题\n
     """
 
     # 结束函数
     def analyse(code:str='000') -> bool|dict:
         # 参数检查
-        ...
+        if not isinstance(code, str):
+            raise TypeError('"code" should be a str')
 
         # 输出处理
         if details:
-            result = {'id':'',  
+            result = {'id':id,  
                       'province':['', ''], 
                       'city':['', ''], 
                       'county':['', ''],
                       'birth_date':['', '', ''],
                       'gender':'',
                       'result':False,
                       'problem':code}
             if code == '000':
                 result['result'] = True
-            if code == '001':
-                pass
-            else:
                 result['id'] = id
-            if code == '004':
-                pass
-            else:
+            if not (code in ('004', '005')):
                 result['birth_date'] = birth_date
                 result['gender'] = gender
-            if len(location) == 0:
-                pass
-            else:
-                result.update(location)
+            result.update(location)
             return result
         else:
             if code == '000':
                 return True
             else:
                 return False
 
-    # 参数类型检查
-    ...
-
     # 变量设置
-    location = {}
+    location = {'province':['', ''], 'city':['', ''], 'county':['', '']}
+
+    # 参数类型检查
+    if not isinstance(id, str):
+        raise TypeError('"id" should be a str')
+    if not isinstance(time_check, bool):
+        raise TypeError('"time_check" should be a bool')
+    if not isinstance(details, bool):
+        raise TypeError('"details" should be a bool')
+    if not id[:17].isnumeric():
+        return analyse('005')
 
     # 参数预处理
     if len(id) == 18:
         address = [id[:2], id[2:4], id[4:6]]
         birth_date = [id[6:10], id[10:12], id[12:14]]
         gender = int(id[16:17])%2
         check_code = id[17:18]
@@ -128,15 +128,17 @@
         pass
     elif str(calculation_result) == check_code:
         pass
     else:
         return analyse('006')
 
     # 校验2
-    location = {'province':[address[0], ''], 'city':[address[1], ''], 'county':[address[2], '']}
+    location['province'][0] = address[0]
+    location['city'][0] = address[1]
+    location['county'][0] = address[2]
     location['province'][1], location['city'][1], location['county'][1] = code_to_location([address[0], address[1], address[2]])
     if location['province'][1] == '':
         return analyse('007')
     
     # 校验3
     if time_check:  # 对出生日期合法性的检查
         if int(birth_date[0]) <= int(time.strftime("%Y", time.localtime())):  # 年
@@ -168,21 +170,14 @@
             return analyse('008')
     else:
         pass
 
     # 返回值
     return analyse('000')
 
-def problem(code: str) -> str:
-    '''
-    用问题代码查找对应的问题详情
-    '''
-
-    return problem_and_code[code]
-
 
 if __name__ == '__main__':
     # 效果演示(实例来自于GB11643-1999)
     # 北京市朝阳区1949年12月31日出生的一女性公民
     print(mod112('11010519491231002X', details=True))
     # 广东省汕头市朝阳县1880年1月1日出生的一男性公民
     print(mod112('440524188001010014', details=True))
```

### Comparing `pymod112-0.1.0/src/pymod112.egg-info/PKG-INFO` & `pymod112-0.1.1/src/pymod112.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymod112
-Version: 0.1.0
+Version: 0.1.1
 Summary: 一个可以离线检验公民身份号码是否合法的程序
 Author-email: HoshsL <HoshsL@outlook.com>
 Project-URL: Homepage, https://gitee.com/HoshsL/PyMOD11-2
 Project-URL: Bug Tracker, https://gitee.com/HoshsL/PyMOD11-2/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -14,23 +14,23 @@
 
 # pymod112
 
 一个基于Python开发的公民身份号码检验与地区代码查找程序
 
 ## 安装 Installation
 
-使用pip安装
+[PyPi](https://pypi.org/project/pymod112/) 使用pip安装
 
 ```sh
 pip install pymod112
 ```
 
 ## 使用 Usage
 
-基础使用
+身份证号码校验
 
 ```python
 import pymod112
 
 pymod112.mod112('11010519491231002X', details=True)
 '''返回值为(dict)
 {'id': '11010519491231002X', 
@@ -41,20 +41,49 @@
  'gender': 0, 
  'result': True, 
  'problem': '000'}
 '''
 
 ```
 
-拓展功能(查询地区代码对应的地区名)
+查询地区代码对应的地区名
 
 ```python
 import pymod112
 
 pymod112.code_to_location(['51', '01', '06'])
 '''返回值为(list)
 ['四川省', '成都市', '金牛区']
 '''
 ```
 
+返回全部错误代码及其对应内容
+
+```python
+import pymod112
+
+pymod112.code_to_error
+'''dict
+{'000':'不存在问题',
+'001':'<未定义>',
+'002':'<未定义>',
+'003':'<未定义>',
+'004':'参数id长度错误',
+'005':'参数id内容包含非法字符',
+'006':'参数id不合法',
+'007':'参数id中包含不存在的地区',
+'008':'参数id中包含不存在的时间'
+}
+'''
+```
+
 ## 许可证 License
 BSD 3-Clause License
+
+## 更新日志 Changelog
+### **0.1.1**
+ - 加入参数类型检查
+ - 优化错误代码（停用001 002 003）
+ - 删除函数problem()
+
+### **0.1.0(2023-6-24)**
+- 这是第一个正式发行版
```

