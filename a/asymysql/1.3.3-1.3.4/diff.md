# Comparing `tmp/asymysql-1.3.3.tar.gz` & `tmp/asymysql-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asymysql-1.3.3.tar", last modified: Tue Jun 13 15:45:50 2023, max compression
+gzip compressed data, was "asymysql-1.3.4.tar", last modified: Sun Jul  2 06:45:49 2023, max compression
```

## Comparing `asymysql-1.3.3.tar` & `asymysql-1.3.4.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.569575 asymysql-1.3.3/LICENSE
--rw-r--r--   0        0        0     4993 2023-06-13 15:29:36.475109 asymysql-1.3.3/README.md
--rw-r--r--   0        0        0       28 2023-04-10 03:48:57.281686 asymysql-1.3.3/asymysql.py
--rw-r--r--   0        0        0      589 2023-06-13 15:45:44.120150 asymysql-1.3.3/pyproject.toml
--rw-r--r--   0        0        0     5246 1970-01-01 00:00:00.000000 asymysql-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.569575 asymysql-1.3.4/LICENSE
+-rw-r--r--   0        0        0     4693 2023-07-02 06:05:28.485396 asymysql-1.3.4/README.md
+-rw-r--r--   0        0        0       28 2023-04-10 03:48:57.281686 asymysql-1.3.4/asymysql/__init__.py
+-rw-r--r--   0        0        0    18318 2023-06-14 09:12:35.228575 asymysql-1.3.4/asymysql/docs/index.md
+-rw-r--r--   0        0        0      591 2023-07-02 06:04:20.413474 asymysql-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0     4950 1970-01-01 00:00:00.000000 asymysql-1.3.4/PKG-INFO
```

### Comparing `asymysql-1.3.3/LICENSE` & `asymysql-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `asymysql-1.3.3/README.md` & `asymysql-1.3.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,168 +1,179 @@
-# 项目描述
-
-异步的 mysql ORM 。
-
-# 安装与教程
-
-安装：`pip install asymysql`
-
-[教程](https://github.com/lcctoor/lccpy/blob/main/packages/asymysql/docs/doc.md)
-
-# Bug提交、功能提议
-
-您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR-max.jpg)、[技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/lccpy/WechatReadersGroupQR-original.jpg) 与我联系。
-
-# 关于作者
-
-作者：许灿标
-
-邮箱：lcctoor@outlook.com
-
-[主页](https://github.com/lcctoor/me#readme) | [微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR-max.jpg) | [微信公众号](https://raw.githubusercontent.com/lcctoor/me/main/author/WechatSubscribeQRAndSearch-max.png) | [Python技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/lccpy/WechatReadersGroupQR-original.jpg)
-
-开源项目：[让Python更简单一点](https://github.com/lcctoor/lccpy#readme)
-
-# 教程预览
-
-#### 导入
-
-```python
-from aiomysql import connect
-from asymysql import ORM, mc, mf
-```
-
-#### 创建ORM
-
-```python
-async def mkconn():
-    return await connect(
-        host = 'localhost',
-        port = 3306,
-        user = 'root',
-        password = '123456789'
-    )
-
-orm = await ORM(mkconn)  # 账户ORM
-db = orm['泉州市']  # 库ORM
-sheet = db['希望小学']  # 表ORM
-```
-
-#### 新增数据
-
-```python
-line1 = {'姓名': '小一', '年龄':11, '签到日期':'2023-01-11'}
-line2 = {'姓名': '小二', '年龄':12, '签到日期':'2023-01-12'}
-line3 = {'姓名': '小三', '年龄':13, '签到日期':'2023-01-13'}
-line4 = {'姓名': '小四', '年龄':14, '签到日期':'2023-01-14'}
-line5 = {'姓名': '小五', '年龄':15, '签到日期':'2023-01-15'}
-line6 = {'姓名': '小六', '年龄':16, '签到日期':'2023-01-16'}
-
-await sheet.insert(line1)  # 添加1条数据
-await sheet.insert([ line2, line3, line4, line5, line6 ])  # 批量添加
-```
-
-#### 查询
-
-```python
-await sheet[:]  # 查询所有数据
-
-await sheet[3]  # 查询第3条数据
-
-await sheet[mc.年龄>13][mc.姓名=='小五'][1]  # 查询年龄大于13、且姓名叫'小五'的第1条数据
-```
-
-#### 修改
-
-```python
-data = {
-    '视力': 5.0,
-    '性别': '男',
-    '爱好': '足球,篮球,画画,跳绳'
-}
-
-await sheet.update(data)[2:5]
-```
-
-#### 删除
-
-```python
-# 删除年龄>=15的所有数据
-await sheet[mc.年龄>=15].delete()[:]
-
-# 删除年龄大于10、且喜欢足球的第2条数据
-await sheet[mc.年龄>10][mc.爱好.re('足球')].delete()[2]
-
-# 删除所有数据
-await sheet.delete()[:]
-```
-
-#### 比较运算
-
-| **代码** |
-| -------------- |
-| mc.年龄 > 10   |
-| mc.年龄 >= 10  |
-| mc.年龄 < 10   |
-| ...            |
-
-#### 成员运算
-
-| **代码**               | **解释**                   |
-| ---------------------------- | -------------------------------- |
-| mc.年级.isin('初三', '高二') | 若字段值是传入值的成员，则符合   |
-| mc.年级.notin(10, 30, 45)    | 若字段值不是传入值的成员，则符合 |
-
-#### 过滤器的集合运算
-
-| **代码**                                                       | **解释** |
-| -------------------------------------------------------------------- | -------------- |
-| [ mc.年龄>3 ][ mc.年龄<100 ]                                         | 交集           |
-| [ (mc.年龄<30)\| (mc.年龄>30) \| (mc.年龄==30) \| (mc.年龄==None) ] | 并集           |
-| [ (mc.年龄>3) - (mc.年龄>100) ]                                      | 差集           |
-| [ ~(mc.年龄>100) ]                                                   | 补集           |
-
-#### 限定字段
-
-只返回姓名、年龄这2个字段：
-
-```python
-await sheet[mc.年级=='高一']['姓名','年龄'][:]
-```
-
-#### 排序
-
-优先按年龄降序，其次按姓名升序，排序后返回第2\~4条数据：
-
-```python
-await sheet[mc.年级=='高一'].order(年龄=False, 姓名=True)[2:4]
-```
-
-#### 执行原生SQL语句
-
-```python
-data, cursor = await sheet.execute('select 姓名 from 希望小学 limit 1')
-data
-# >>> [{'姓名': '小一'}]
-
-data, cursor = await sheet.execute('update 希望小学 set 爱好="编程" limit 3')
-cursor.rowcount
-# >>> 3
-
-data, cursor = await sheet.execute("delete from 希望小学 limit 2")
-cursor.rowcount
-# >>> 2
-
-sql = 'insert into 希望小学(姓名, 年龄) values (%s, %s)'
-students = [('小七', 17), ('小八', 18)]
-data, cursor = await sheet.executemany(sql, students)
-cursor.lastrowid
-# >>> 8
-```
-
-# 支持作者1元
-
-asymysql 是一个免费的开源项目，由个人维护。
-
-每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
-
-<img src="https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR-1rmb-max.jpg" width="200px">
+Metadata-Version: 2.1
+Name: asymysql
+Version: 1.3.4
+Summary: 异步的 mysql ORM
+Keywords: asymysql,aiomysql,mysql,pymysql,orm
+Author-email: 许灿标 <lcctoor@outlook.com>
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Classifier: License :: OSI Approved :: Apache Software License
+Requires-Dist: lccpy >=1.4.7.1
+Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/packages/asymysql#readme
+
+# 项目描述
+
+异步的 mysql ORM 。
+
+# 安装与教程
+
+安装：`pip install asymysql`
+
+[教程](https://github.com/lcctoor/lccpy/blob/main/packages/asymysql/asymysql/docs/index.md)
+
+# Bug提交、功能提议
+
+您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg)、[技术交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg) 与我联系。
+
+# 关于作者
+
+作者：许灿标
+
+邮箱：lcctoor@outlook.com
+
+[主页](https://lcctoor.github.io/me/) | [微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) | [Python技术交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg)
+
+# 教程预览
+
+#### 导入
+
+```python
+from aiomysql import connect
+from asymysql import ORM, mc, mf
+```
+
+#### 创建ORM
+
+```python
+async def mkconn():
+    return await connect(
+        host = 'localhost',
+        port = 3306,
+        user = 'root',
+        password = '123456789'
+    )
+
+orm = await ORM(mkconn)  # 账户ORM
+db = orm['泉州市']  # 库ORM
+sheet = db['希望小学']  # 表ORM
+```
+
+#### 新增数据
+
+```python
+line1 = {'姓名': '小一', '年龄':11, '签到日期':'2023-01-11'}
+line2 = {'姓名': '小二', '年龄':12, '签到日期':'2023-01-12'}
+line3 = {'姓名': '小三', '年龄':13, '签到日期':'2023-01-13'}
+line4 = {'姓名': '小四', '年龄':14, '签到日期':'2023-01-14'}
+line5 = {'姓名': '小五', '年龄':15, '签到日期':'2023-01-15'}
+line6 = {'姓名': '小六', '年龄':16, '签到日期':'2023-01-16'}
+
+await sheet.insert(line1)  # 添加1条数据
+await sheet.insert([ line2, line3, line4, line5, line6 ])  # 批量添加
+```
+
+#### 查询
+
+```python
+await sheet[:]  # 查询所有数据
+
+await sheet[3]  # 查询第3条数据
+
+await sheet[mc.年龄>13][mc.姓名=='小五'][1]  # 查询年龄大于13、且姓名叫'小五'的第1条数据
+```
+
+#### 修改
+
+```python
+data = {
+    '视力': 5.0,
+    '性别': '男',
+    '爱好': '足球,篮球,画画,跳绳'
+}
+
+await sheet.update(data)[2:5]
+```
+
+#### 删除
+
+```python
+# 删除年龄>=15的所有数据
+await sheet[mc.年龄>=15].delete()[:]
+
+# 删除年龄大于10、且喜欢足球的第2条数据
+await sheet[mc.年龄>10][mc.爱好.re('足球')].delete()[2]
+
+# 删除所有数据
+await sheet.delete()[:]
+```
+
+#### 比较运算
+
+| **代码** |
+| -------------- |
+| mc.年龄 > 10   |
+| mc.年龄 >= 10  |
+| mc.年龄 < 10   |
+| ...            |
+
+#### 成员运算
+
+| **代码**               | **解释**                   |
+| ---------------------------- | -------------------------------- |
+| mc.年级.isin('初三', '高二') | 若字段值是传入值的成员，则符合   |
+| mc.年级.notin(10, 30, 45)    | 若字段值不是传入值的成员，则符合 |
+
+#### 过滤器的集合运算
+
+| **代码**                                                       | **解释** |
+| -------------------------------------------------------------------- | -------------- |
+| [ mc.年龄>3 ][ mc.年龄<100 ]                                         | 交集           |
+| [ (mc.年龄<30)\| (mc.年龄>30) \| (mc.年龄==30) \| (mc.年龄==None) ] | 并集           |
+| [ (mc.年龄>3) - (mc.年龄>100) ]                                      | 差集           |
+| [ ~(mc.年龄>100) ]                                                   | 补集           |
+
+#### 限定字段
+
+只返回姓名、年龄这2个字段：
+
+```python
+await sheet[mc.年级=='高一']['姓名','年龄'][:]
+```
+
+#### 排序
+
+优先按年龄降序，其次按姓名升序，排序后返回第2\~4条数据：
+
+```python
+await sheet[mc.年级=='高一'].order(年龄=False, 姓名=True)[2:4]
+```
+
+#### 执行原生SQL语句
+
+```python
+data, cursor = await sheet.execute('select 姓名 from 希望小学 limit 1')
+data
+# >>> [{'姓名': '小一'}]
+
+data, cursor = await sheet.execute('update 希望小学 set 爱好="编程" limit 3')
+cursor.rowcount
+# >>> 3
+
+data, cursor = await sheet.execute("delete from 希望小学 limit 2")
+cursor.rowcount
+# >>> 2
+
+sql = 'insert into 希望小学(姓名, 年龄) values (%s, %s)'
+students = [('小七', 17), ('小八', 18)]
+data, cursor = await sheet.executemany(sql, students)
+cursor.lastrowid
+# >>> 8
+```
+
+# 支持作者1元
+
+asymysql 是一个免费的开源项目，由个人维护。
+
+每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
+
+<img src="https://lcctoor.github.io/me/donation/donationQR-1rmb-max.jpg" width="200px">
+
```

### Comparing `asymysql-1.3.3/pyproject.toml` & `asymysql-1.3.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "asymysql"
-version = "1.3.3"
+version = "1.3.4"
 description = "异步的 mysql ORM"
-dependencies = ["lccpy >=1.4.7"]
+dependencies = ["lccpy >=1.4.7.1"]
 keywords = ["asymysql", "aiomysql", "mysql", "pymysql", "orm"]
 
 readme = "README.md"
 authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 requires-python = ">=3.7"
```

