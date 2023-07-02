# Comparing `tmp/mysqlx-1.3.1.tar.gz` & `tmp/mysqlx-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mysqlx-1.3.1.tar", last modified: Tue Jun 20 09:06:19 2023, max compression
+gzip compressed data, was "dist\mysqlx-1.3.2.tar", last modified: Sun Jul  2 08:03:57 2023, max compression
```

## Comparing `mysqlx-1.3.1.tar` & `mysqlx-1.3.2.tar`

### file list

```diff
@@ -1,32 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 09:06:19.000000 mysqlx-1.3.1/
--rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-1.3.1/LICENSE
-drwxrwxrwx   0        0        0        0 2023-06-20 09:06:19.000000 mysqlx-1.3.1/mysqlx/
--rw-rw-rw-   0        0        0     5827 2023-06-19 12:47:48.000000 mysqlx-1.3.1/mysqlx/coder.py
--rw-rw-rw-   0        0        0     1589 2023-06-09 01:09:35.000000 mysqlx-1.3.1/mysqlx/coder.tpl
--rw-rw-rw-   0        0        0    17467 2023-06-18 07:05:30.000000 mysqlx-1.3.1/mysqlx/db.py
--rw-rw-rw-   0        0        0    10001 2023-06-20 01:39:01.000000 mysqlx-1.3.1/mysqlx/dbx.py
--rw-rw-rw-   0        0        0    30506 2023-06-19 05:19:22.000000 mysqlx-1.3.1/mysqlx/orm.py
--rw-rw-rw-   0        0        0     6107 2023-06-18 03:07:16.000000 mysqlx-1.3.1/mysqlx/support.py
--rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.3.1/mysqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 09:06:19.000000 mysqlx-1.3.1/mysqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2023-06-20 09:06:19.000000 mysqlx-1.3.1/mysqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-19 14:08:07.000000 mysqlx-1.3.1/mysqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     4737 2023-06-20 09:06:19.000000 mysqlx-1.3.1/mysqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-06-20 09:06:19.000000 mysqlx-1.3.1/mysqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      487 2023-06-20 09:06:19.000000 mysqlx-1.3.1/mysqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       12 2023-06-20 09:06:19.000000 mysqlx-1.3.1/mysqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4737 2023-06-20 09:06:19.000000 mysqlx-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     4022 2023-06-20 08:57:34.000000 mysqlx-1.3.1/README.md
--rw-rw-rw-   0        0        0     4185 2023-06-20 09:05:43.000000 mysqlx-1.3.1/README.rst
--rw-rw-rw-   0        0        0       42 2023-06-20 09:06:19.000000 mysqlx-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1217 2023-06-20 09:01:58.000000 mysqlx-1.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 09:06:19.000000 mysqlx-1.3.1/test/
--rw-rw-rw-   0        0        0      216 2023-06-10 13:13:30.000000 mysqlx-1.3.1/test/all_unit_test.py
--rw-rw-rw-   0        0        0      312 2023-06-19 03:27:12.000000 mysqlx-1.3.1/test/coder_test.py
--rw-rw-rw-   0        0        0     2966 2023-06-13 02:46:47.000000 mysqlx-1.3.1/test/dbx_test.py
--rw-rw-rw-   0        0        0     5025 2023-06-13 09:20:17.000000 mysqlx-1.3.1/test/db_test.py
--rw-rw-rw-   0        0        0     5090 2023-06-19 12:47:52.000000 mysqlx-1.3.1/test/models.py
--rw-rw-rw-   0        0        0     6869 2023-06-19 05:16:27.000000 mysqlx-1.3.1/test/orm_test.py
--rw-rw-rw-   0        0        0      710 2023-06-11 02:56:34.000000 mysqlx-1.3.1/test/unit_test.py
--rw-rw-rw-   0        0        0      320 2023-06-13 02:39:09.000000 mysqlx-1.3.1/test/user_mapper.py
--rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.3.1/test/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-02 08:03:56.000000 mysqlx-1.3.2/
+-rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-1.3.2/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-02 08:03:56.000000 mysqlx-1.3.2/mysqlx/
+-rw-rw-rw-   0        0        0     5827 2023-06-19 12:47:48.000000 mysqlx-1.3.2/mysqlx/coder.py
+-rw-rw-rw-   0        0        0     1644 2023-06-26 14:04:23.000000 mysqlx-1.3.2/mysqlx/coder.tpl
+-rw-rw-rw-   0        0        0    19388 2023-07-01 16:17:50.000000 mysqlx-1.3.2/mysqlx/db.py
+-rw-rw-rw-   0        0        0    13200 2023-07-02 03:56:40.000000 mysqlx-1.3.2/mysqlx/dbx.py
+-rw-rw-rw-   0        0        0    36870 2023-07-01 16:20:03.000000 mysqlx-1.3.2/mysqlx/orm.py
+-rw-rw-rw-   0        0        0     2392 2023-06-26 14:23:12.000000 mysqlx-1.3.2/mysqlx/snowflake.py
+-rw-rw-rw-   0        0        0     3596 2023-07-02 06:28:56.000000 mysqlx-1.3.2/mysqlx/sql_mapper.py
+-rw-rw-rw-   0        0        0     7811 2023-06-30 06:21:34.000000 mysqlx-1.3.2/mysqlx/support.py
+-rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.3.2/mysqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-02 08:03:56.000000 mysqlx-1.3.2/mysqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-02 08:03:56.000000 mysqlx-1.3.2/mysqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-19 14:08:07.000000 mysqlx-1.3.2/mysqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     4247 2023-07-02 08:03:56.000000 mysqlx-1.3.2/mysqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2023-07-02 08:03:56.000000 mysqlx-1.3.2/mysqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      589 2023-07-02 08:03:56.000000 mysqlx-1.3.2/mysqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       12 2023-07-02 08:03:56.000000 mysqlx-1.3.2/mysqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4247 2023-07-02 08:03:56.000000 mysqlx-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3712 2023-07-02 07:35:05.000000 mysqlx-1.3.2/README.md
+-rw-rw-rw-   0        0        0     4185 2023-06-20 09:05:43.000000 mysqlx-1.3.2/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-02 08:03:56.000000 mysqlx-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1233 2023-07-02 08:03:49.000000 mysqlx-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 08:03:56.000000 mysqlx-1.3.2/test/
+-rw-rw-rw-   0        0        0      216 2023-06-25 13:41:37.000000 mysqlx-1.3.2/test/all_unit_test.py
+-rw-rw-rw-   0        0        0      312 2023-06-19 03:27:12.000000 mysqlx-1.3.2/test/coder_test.py
+-rw-rw-rw-   0        0        0     2988 2023-07-02 06:29:16.000000 mysqlx-1.3.2/test/dbx_test.py
+-rw-rw-rw-   0        0        0     5067 2023-06-27 15:48:31.000000 mysqlx-1.3.2/test/db_test.py
+-rw-rw-rw-   0        0        0      770 2023-07-02 04:45:13.000000 mysqlx-1.3.2/test/mapper_test.py
+-rw-rw-rw-   0        0        0     5202 2023-07-01 16:10:46.000000 mysqlx-1.3.2/test/models.py
+-rw-rw-rw-   0        0        0     5648 2023-07-01 16:10:25.000000 mysqlx-1.3.2/test/orm_test.py
+-rw-rw-rw-   0        0        0      301 2023-06-26 13:41:30.000000 mysqlx-1.3.2/test/snowflake_test.py
+-rw-rw-rw-   0        0        0      381 2023-06-21 05:03:37.000000 mysqlx-1.3.2/test/time_test.py
+-rw-rw-rw-   0        0        0      710 2023-06-11 02:56:34.000000 mysqlx-1.3.2/test/unit_test.py
+-rw-rw-rw-   0        0        0      320 2023-06-13 02:39:09.000000 mysqlx-1.3.2/test/user_mapper.py
+-rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.3.2/test/__init__.py
```

### Comparing `mysqlx-1.3.1/LICENSE` & `mysqlx-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mysqlx-1.3.1/mysqlx/coder.py` & `mysqlx-1.3.2/mysqlx/coder.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.3.1/mysqlx/coder.tpl` & `mysqlx-1.3.2/mysqlx/coder.tpl`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from decimal import Decimal
-from mysqlx.orm import Model
 from datetime import date, datetime
+from mysqlx.orm import Model, PkStrategy
 
 
 class BaseModel(Model):
     __pk__ = '{{__pk__}}'
     __update_by__ = '{{__update_by__}}'
     __update_time__ = '{{__update_time__}}'
     __del_flag__ = '{{__del_flag__}}'
+    __pk_strategy__ = PkStrategy.DB.value
 
     def __init__(self,{% for item in base_columns %}{% if loop.last %}{% if item.DATA_TYPE=='None' %} {{item.COLUMN_NAME}}=None{% else %} {{item.COLUMN_NAME}}: {{item.DATA_TYPE}} = None{% endif %}{% else %}{% if item.DATA_TYPE=='None' %} {{item.COLUMN_NAME}}=None{% else %} {{item.COLUMN_NAME}}: {{item.DATA_TYPE}} = None{% endif %},{% endif %}{% endfor %}): {% for item in base_columns %}
         self.{{item.COLUMN_NAME}} = {{item.COLUMN_NAME}} {% endfor %}
 
 {% for meta in metas %}
 class {{meta.class_name}}(BaseModel):{% if meta.pk != __pk__ %}
     __pk__ = '{{meta.pk}}'{% endif %}
```

### Comparing `mysqlx-1.3.1/mysqlx/db.py` & `mysqlx-1.3.2/mysqlx/db.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,50 @@
 import logging
 import functools
-from typing import Any, Union, Mapping, Sequence
-from .support import DBCtx, ConnectionCtx, Dict, MultiColumnsError, TransactionCtx, try_commit, dynamic_sql, log, get_named_sql, get_named_args, page_log, LIMIT_1, DBError
+from typing import Sequence
+from .support import DBCtx, ConnectionCtx, Dict, MultiColumnsError, TransactionCtx, try_commit, dynamic_sql, log, get_named_sql, get_named_args, \
+    page_log, LIMIT_1, DBError, DB_LOCK, get_batch_args
 
 _DB_CTX = None
 _SHOW_SQL = False
+_MAPPER_PATH = "mapper_path"
 _PK_SQL = 'SELECT LAST_INSERT_ID()'
 
 
-def init_db(user='root', password='', database='test', host='127.0.0.1', port=3306, pool_size=8, use_unicode=True, show_sql=False, **kwargs):
-    from mysql.connector import connect
-    from mysql.connector.pooling import CONNECTION_POOL_LOCK
+def init_db(user='root', password='', database='test', host='127.0.0.1', port=3306, pool_size=5, use_unicode=True, show_sql=False, **kwargs):
+    use_mysql_connector = False
+    try:
+        from mysql.connector import connect
+        use_mysql_connector = True
+    except ImportError:
+        from pymysql import connect
+
     global _DB_CTX
     global _SHOW_SQL
-
-    with CONNECTION_POOL_LOCK:
+    is_pool = use_mysql_connector and pool_size >= 1
+    with DB_LOCK:
         if _DB_CTX is not None:
             raise DBError('DB is already initialized.')
-
         _SHOW_SQL = show_sql
-        if 'mapper_dir' in kwargs:
-            del kwargs['mapper_dir']
-
-        if pool_size >= 1:
+        if _MAPPER_PATH in kwargs:
+            from .dbx import load_mapper
+            load_mapper(kwargs[_MAPPER_PATH])
+            del kwargs[_MAPPER_PATH]
+        if is_pool:
             kwargs['pool_size'] = pool_size
             if 'pool_name' not in kwargs:
-                kwargs['pool_name'] = "%s_pool" % database
-
+                kwargs['pool_name'] = "{}_pool".format(database)
         kwargs['user'] = user
         kwargs['password'] = password
         kwargs['database'] = database
         kwargs['host'] = host
         kwargs['port'] = port
         kwargs['use_unicode'] = use_unicode
-        _DB_CTX = DBCtx(lambda: connect(**kwargs))
-
-    if pool_size >= 1:
+        _DB_CTX = DBCtx(connect=lambda: connect(**kwargs), use_mysql_connector=use_mysql_connector)
+    if is_pool:
         logging.info('Init db engine <%s> ok with connection pool size: %d.' % (hex(id(_DB_CTX)), pool_size))
     else:
         logging.info('Init db engine <%s> ok without connection pool.' % hex(id(_DB_CTX)))
 
 
 def connection():
     """
@@ -94,14 +99,15 @@
     """
     global _DB_CTX
 
     @functools.wraps(func)
     def _wrapper(*args, **kw):
         with TransactionCtx(_DB_CTX):
             return func(*args, **kw)
+
     return _wrapper
 
 
 # ----------------------------------------------------------Update function------------------------------------------------------------------
 def insert(table: str, **kwargs):
     """
     Execute insert SQL, return effect rowcount.
@@ -121,15 +127,15 @@
     :param table: table name
     :param kwargs: name='张三', age=20}
     :return: Primary key
     """
     logging.debug("Exec func 'mysqlx.db.%s' \n\t\t Table: '%s', kwargs: %s" % ('save', table, kwargs))
     global _DB_CTX
     cursor = None
-    sql, args = _insert_sql_args(table.strip(), ** kwargs)
+    sql, args = _insert_sql_args(table.strip(), **kwargs)
     sql = _before_execute('save', sql, *args)
     try:
         cursor = _DB_CTX.connection.cursor()
         cursor.execute(sql, args)
         cursor.execute(_PK_SQL)
         result = cursor.fetchone()
         try_commit(_DB_CTX)
@@ -146,41 +152,41 @@
          INSERT INTO user(name, age) VALUES(:name,:age)  -->  kwargs: {'name': '张三', 'age': 20}
     """
     log('db.execute', sql, *args, **kwargs)
     sql, args = dynamic_sql(sql, *args, **kwargs)
     return do_execute(sql, *args)
 
 
-def batch_insert(table: str, args: Sequence[Mapping[str, Any]]):
+def batch_insert(table: str, *args):
     """
     Batch insert
     :param table: table name
     :param args: All number must have same key. [{'name': '张三', 'age': 20}, {'name': '李四', 'age': 28}]
     :return: Effect row count
     """
     logging.debug("Exec func 'mysqlx.db.%s' \n\t\t Table: '%s', args: %s" % ('batch_insert', table, args))
     assert len(args) > 0, 'args must not be empty.'
-    sql, args = _batch_insert_sql_args(table, args)
-    return batch_execute(sql, args)
+    sql, args = _batch_insert_sql_args(table, *args)
+    return batch_execute(sql, *args)
 
 
-def batch_execute(sql: str, args: Union[Sequence[Sequence[Any]], Sequence[Mapping[str, Any]]]):
+def batch_execute(sql: str, *args):
     """
     Batch execute
     :param sql: INSERT INTO user(name, age) VALUES(?, ?)  -->  args: [('张三', 20), ('李四', 28)]
                 INSERT INTO user(name, age) VALUES(:name,:age)  -->  args: [{'name': '张三', 'age': 20}, {'name': '李四', 'age': 28}]
     :param args: All number must have same size.
     :return: Effect row count
     """
     logging.debug("Exec func 'mysqlx.db.%s' \n\t\t sql: '%s' \n\t\t args: %s" % ('batch_execute', sql, args))
     assert len(args) > 0, 'args must not be empty.'
     if isinstance(args[0], dict):
-        sql, args = _batch_named_sql_args(sql, args)
+        sql, args = _batch_named_sql_args(sql, *args)
 
-    return do_batch_execute(sql, args)
+    return do_batch_execute(sql, *args)
 
 
 # ----------------------------------------------------------Query function------------------------------------------------------------------
 def get(sql: str, *args, **kwargs):
     """
     Execute select SQL and expected one int and only one int result. Automatically add 'limit ?' after sql statement if not.
     MultiColumnsError: Expect only one column.
@@ -281,43 +287,55 @@
         return effect_rowcount
     finally:
         if cursor:
             cursor.close()
 
 
 @with_connection
-def do_batch_execute(sql: str, args: Sequence[Sequence[Any]]):
+def do_batch_execute(sql: str, *args):
     """
     Batch execute sql return effect rowcount
     :param sql: insert into user(name, age) values(?, ?)  -->  args: [('张三', 20), ('李四', 28)]
     :param args: All number must have same size.
     :return: Effect rowcount
     """
     global _DB_CTX
     cursor = None
     sql = _before_execute('do_batch_execute', sql.strip(), *args)
+    args = get_batch_args(*args)
     try:
         cursor = _DB_CTX.cursor()
         cursor.executemany(sql, args)
         effect_rowcount = cursor.rowcount
         try_commit(_DB_CTX)
         return effect_rowcount
     finally:
         if cursor:
             cursor.close()
 
 
 def do_get(sql: str, *args):
     """
-    Execute select SQL and expected one int and only one int result. Automatically add 'limit ?' after sql statement if not.
+    Execute select SQL and expected one int and only one int result. Automatically add 'limit ?' behind the sql statement if not.
     MultiColumnsError: Expect only one column.
     sql: SELECT count(1) FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
-    logging.debug("Exec func 'mysqlx.db.%s' \n\t\t sql: %s \n\t\t  args: %s" % ('do_get', sql, args))
-    result = do_select_one(sql, *args)
+    logging.debug("Exec func 'mysqlx.db.%s' \n\t\t sql: %s \n\t\t args: %s" % ('do_get', sql, args))
+    sql, args = _limit_one_sql_args(sql, *args)
+    return do_get_limit(sql, *args)
+
+
+def do_get_limit(sql: str, *args):
+    """
+    Execute select SQL and expected one int and only one int result, SQL contain 'limit'.
+    MultiColumnsError: Expect only one column.
+    sql: SELECT count(1) FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
+    """
+    logging.debug("Exec func 'mysqlx.db.%s' \n\t\t sql: %s \n\t\t args: %s" % ('do_get_limit', sql, args))
+    result = do_select_one_limit(sql, *args)
     if result:
         if len(result) == 1:
             return result[0]
         msg = "Exec func 'mysqlx.db.%s' expect only one column but %d." % ('do_get', len(result))
         logging.error('%s  \n\t\t sql: %s \n\t\t args: %s' % (msg, sql, args))
         raise MultiColumnsError(msg)
     return None
@@ -327,15 +345,15 @@
 def do_query(sql: str, *args):
     """
     Execute select SQL and return list results(dict).
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
     """
     global _DB_CTX
     cursor = None
-    sql = _before_execute('do_select', sql.strip(), *args)
+    sql = _before_execute('do_query', sql.strip(), *args)
     try:
         cursor = _DB_CTX.cursor()
         cursor.execute(sql, args)
         if cursor.description:
             names = [x[0] for x in cursor.description]
             return [Dict(names, x) for x in cursor.fetchall()]
         else:
@@ -344,21 +362,32 @@
         if cursor:
             cursor.close()
 
 
 @with_connection
 def do_query_one(sql: str, *args):
     """
-    execute select SQL and return unique result(dict). Automatically add 'limit ?' after sql statement if not.
+    execute select SQL and return unique result(dict). Automatically add 'limit ?' behind the sql statement if not.
+    sql: SELECT * FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
+    """
+    logging.debug("Exec func 'mysqlx.db.%s' \n\t\t sql: %s \n\t\t args: %s" % ('do_query_one', sql, args))
+    sql, args = _limit_one_sql_args(sql, *args)
+    return do_query_one_limit(sql, *args)
+
+
+@with_connection
+def do_query_one_limit(sql: str, *args):
+    """
+    execute select SQL and return unique result(dict), SQL contain 'limit'.
     sql: SELECT * FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
     global _DB_CTX
     cursor = None
     sql, args = _limit_one_sql_args(sql, *args)
-    sql = _before_execute('do_query_one', sql.strip(), *args)
+    sql = _before_execute('do_query_one_limit', sql.strip(), *args)
     try:
         cursor = _DB_CTX.cursor()
         cursor.execute(sql, args)
         if cursor.description:
             names = [x[0] for x in cursor.description]
             result = cursor.fetchone()
             return Dict(names, result) if result else result
@@ -383,50 +412,59 @@
         cursor.execute(sql, args)
         return cursor.fetchall()
     finally:
         if cursor:
             cursor.close()
 
 
-@with_connection
 def do_select_one(sql: str, *args):
     """
-    Execute select SQL and return unique result(tuple). Automatically add 'limit ?' after sql statement if not.
+    Execute select SQL and return unique result(tuple). Automatically add 'limit ?' behind the sql statement if not.
+    sql: SELECT * FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
+    """
+    logging.debug("Exec func 'mysqlx.db.%s' \n\t\t sql: %s \n\t\t args: %s" % ('do_select_one', sql, args))
+    sql, args = _limit_one_sql_args(sql, *args)
+    return do_select_one_limit(sql, *args)
+
+
+@with_connection
+def do_select_one_limit(sql: str, *args):
+    """
+    Execute select SQL and return unique result(tuple), SQL contain 'limit'.
     sql: SELECT * FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
     global _DB_CTX
     cursor = None
-    sql, args = _limit_one_sql_args(sql, *args)
-    sql = _before_execute('do_select_one', sql.strip(), *args)
+    sql = _before_execute('do_select_one_limit', sql.strip(), *args)
     try:
         cursor = _DB_CTX.cursor()
         cursor.execute(sql, args)
         return cursor.fetchone()
     finally:
         if cursor:
             cursor.close()
 
 
 def do_query_page(sql: str, page_num=1, page_size=10, *args):
     """
     Execute select SQL and return list results(dict).
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
     """
+    _do_page_log('do_query_page', sql, page_num, page_size, args)
     sql, args = _page_sql_args(sql, page_num, page_size, *args)
-    sql = _before_execute('do_query_page', sql.strip(), *args)
     return do_query(sql, *args)
 
 
 def do_select_page(sql: str, page_num=1, page_size=10, *args):
     """
     Execute select SQL and return list results(dict).
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
     """
+    _do_page_log('do_select_page', sql, page_num, page_size, args)
     sql, args = _page_sql_args(sql, page_num, page_size, *args)
-    sql = _before_execute('do_select_page', sql.strip(), *args)
     return do_select(sql, *args)
 
 
 def get_connection():
     global _DB_CTX
     if _DB_CTX.is_not_init():
         _DB_CTX.init()
@@ -447,49 +485,58 @@
 
 def _insert_sql_args(table: str, **kwargs):
     cols, args = zip(*kwargs.items())
     sql = _create_insert_sql(table, cols)
     return sql, args
 
 
-def _batch_insert_sql_args(table: str, args: Sequence[Mapping[str, Any]]):
+def _batch_insert_sql_args(table: str, *args):
+    args = get_batch_args(*args)
     args = [zip(*arg.items()) for arg in args]  # [(cols, args)]
-    cols, args = zip(*args)
+    cols, args = zip(*args)  # (cols), (args)
     sql = _create_insert_sql(table, cols[0])
     return sql, args
 
 
-def _batch_named_sql_args(sql: str, args: Sequence[Mapping[str, Any]]):
+def _batch_named_sql_args(sql: str, *args):
+    args = get_batch_args(*args)
     args = [get_named_args(sql, **arg) for arg in args]
     sql = get_named_sql(sql)
     return sql, args
 
 
+@functools.lru_cache(maxsize=128)
 def _create_insert_sql(table: str, cols: Sequence[str]):
-    return 'INSERT INTO `%s` (%s) VALUES (%s)' % (table, ','.join(['`%s`' % col for col in cols]), ','.join(['?' for _ in range(len(cols))]))
+    columns, placeholders = zip(*[('`{}`'.format(col), '?') for col in cols])
+    return 'INSERT INTO `{}` ({}) VALUES ({})'.format(table, ','.join(columns), ','.join(placeholders))
 
 
 def _page_sql_args(sql: str, page_num=1, page_size=10, *args):
+    start = (page_num - 1) * page_size
+    args = [*args, start, page_size]
     if _require_limit(sql):
-        sql = '%s limit ?,?' % sql
-        start = (page_num - 1) * page_size
-        args = [*args, start, page_size]
+        sql = '{} limit ?,?'.format(sql)
     return sql, args
 
 
 def _limit_one_sql_args(sql: str, *args):
     if _require_limit(sql):
-        return '%s limit ?' % sql, [*args, LIMIT_1]
+        return '{} limit ?'.format(sql), [*args, LIMIT_1]
 
     return sql, args
 
 
 def _require_limit(sql: str):
     lower_sql = sql.lower()
     if 'limit' not in lower_sql:
         return True
 
     idx = lower_sql.rindex('limit')
     if idx > 0 and ')' in lower_sql[idx:]:
         return True
 
     return False
+
+
+def _do_page_log(function: str, sql: str, page_num, page_size, *args):
+    logging.debug(
+        "Exec func 'mysqlx.db.%s', page_num: %d, page_size: %d \n\t\t sql: %s \n\t\t args: %s" % (function, page_num, page_size, sql.strip(), args))
```

### Comparing `mysqlx-1.3.1/mysqlx/dbx.py` & `mysqlx-1.3.2/mysqlx/dbx.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,245 +1,308 @@
 import os
-from . import db
+import re
+import logging
 from jinja2 import Template
-from typing import Any, Union, Sequence, Mapping
-from .support import simple_sql, SqlModel, log, page_log, MapperError, is_dynamic_sql
+from typing import Mapping
+from .support import get_named_sql_args, SqlModel, MapperError, is_dynamic_sql, get_batch_args, SqlAction
+from .db import do_get, do_query, do_query_one, do_execute, do_select_page, do_select, do_select_one, do_query_page, init_db as _init_db, \
+    get_connection as _get_connection, insert as _insert, save as _save, batch_insert as _batch_insert, batch_execute as _batch_execute
+
 try:
     import xml.etree.cElementTree as ET
 except ImportError:
     import xml.etree.ElementTree as ET
 
 _SQL_CONTAINER = dict()
+_valid_sql_actions = (SqlAction.INSERT.value, SqlAction.UPDATE.value, SqlAction.DELETE.value, SqlAction.SELECT.value)
 
 
-def init_db(user='root', password='', database='test', host='127.0.0.1', port=3306, pool_size=8, use_unicode=True, show_sql=False,
-            mapper_dir='mapper', **kwargs):
-    _load_mapper(mapper_dir)
-    db.init_db(user, password, database, host, port, pool_size, use_unicode, show_sql, **kwargs)
+def init_db(user='root', password='', database='test', host='127.0.0.1', port=3306, pool_size=5, use_unicode=True, show_sql=False,
+        mapper_path='mapper', **kwargs):
+    load_mapper(mapper_path)
+    _init_db(user, password, database, host, port, pool_size, use_unicode, show_sql, **kwargs)
 
 
 def insert(table: str, **kwargs):
     """
     Execute insert SQL, return effect rowcount.
     :param table: table name
     :param kwargs: {'name': '张三', 'age': 20}
     return: Effect rowcount
     """
-    return db.insert(table, **kwargs)
+    return _insert(table, **kwargs)
 
 
 def save(table: str, **kwargs):
     """
     Execute insert SQL, return primary key.
     :param table: table name
     :param kwargs: {'name': '张三', 'age': 20}
     :return: Primary key
     """
-    return db.save(table, **kwargs)
+    return _save(table, **kwargs)
 
 
 def execute(sql_id: str, *args, **kwargs):
     """
     Execute SQL.
     sql: INSERT INTO user(name, age) VALUES(?, ?)  -->  args: ('张三', 20)
          INSERT INTO user(name, age) VALUES(:name,:age)  -->  kwargs: {'name': '张三', 'age': 20}
     """
-    sql = get_sql(sql_id, **kwargs)
-    log('dbx.execute', sql, *args, **kwargs)
-    sql, args = simple_sql(sql, *args, **kwargs)
-    return db.do_execute(sql, *args)
+    _sql_id_log('dbx.execute', sql_id, *args, **kwargs)
+    sql, args = get_sql(sql_id, *args, **kwargs)
+    return do_execute(sql, *args)
 
 
-def batch_insert(table: str, args: Sequence[Mapping[str, Any]]):
+def batch_insert(table: str, *args):
     """
     Batch insert
     :param table: table name
     :param args: All number must have same key. [{'name': '张三', 'age': 20}, {'name': '李四', 'age': 28}]
     :return: Effect row count
     """
-    return db.batch_insert(table, args)
+    return _batch_insert(table, *args)
 
 
-def batch_execute(sql_id: str, args: Union[Sequence[Sequence[Any]], Sequence[Mapping[str, Any]]]):
+def batch_execute(sql_id: str, *args):
     """
     Batch execute
     sql: INSERT INTO user(name, age) VALUES(?, ?)  -->  args: [('张三', 20), ('李四', 28)]
          INSERT INTO user(name, age) VALUES(:name,:age)  -->  args: [{'name': '张三', 'age': 20}, {'name': '李四', 'age': 28}]
     :return: Effect row count
     """
-    sql = get_sql(sql_id)
-    return db.batch_execute(sql, args)
+    args = get_batch_args(*args)
+    sql, _ = do_get_sql(get_sql_model(sql_id), True, None, *args)
+    return _batch_execute(sql, *args)
 
 
 # ----------------------------------------------------------Query function------------------------------------------------------------------
 def get(sql_id: str, *args, **kwargs):
     """
-    Execute select SQL and expected one int and only one int result. Automatically add 'limit ?' after sql statement if not.
+    Execute select SQL and expected one int and only one int result. Automatically add 'limit ?' behind the sql statement if not.
     MultiColumnsError: Expect only one column.
     sql: SELECT count(1) FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
          SELECT count(1) FROM user WHERE name=:name and age=:age limit 1  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
-    sql = get_sql(sql_id, **kwargs)
-    log('dbx.get', sql, *args, **kwargs)
-    sql, args = simple_sql(sql, *args, **kwargs)
-    return db.do_get(sql, *args)
+    _sql_id_log('dbx.get', sql_id, *args, **kwargs)
+    sql, args = get_sql(sql_id, *args, **kwargs)
+    return do_get(sql, *args)
 
 
 def query(sql_id: str, *args, **kwargs):
     """
     Execute select SQL and return list or empty list if no result.
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
          SELECT * FROM user WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
-    sql = get_sql(sql_id, **kwargs)
-    log('dbx.query', sql, *args, **kwargs)
-    sql, args = simple_sql(sql, *args, **kwargs)
-    return db.do_query(sql, *args)
+    _sql_id_log('dbx.query', sql_id, *args, **kwargs)
+    sql, args = get_sql(sql_id, *args, **kwargs)
+    return do_query(sql, *args)
 
 
 def query_one(sql_id: str, *args, **kwargs):
     """
-    Execute select SQL and expected one row result(dict). Automatically add 'limit ?' after sql statement if not.
+    Execute select SQL and expected one row result(dict). Automatically add 'limit ?' behind the sql statement if not.
     If no result found, return None.
     If multiple results found, the first one returned.
     sql: SELECT * FROM user WHERE name=? and age=? limit 1 -->  args: ('张三', 20)
          SELECT * FROM user WHERE name=:name and age=:age limit 1  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
-    sql = get_sql(sql_id, **kwargs)
-    log('dbx.query_one', sql, *args, **kwargs)
-    sql, args = simple_sql(sql, *args, **kwargs)
-    return db.do_query_one(sql, *args)
+    _sql_id_log('dbx.query_one', sql_id, *args, **kwargs)
+    sql, args = get_sql(sql_id, *args, **kwargs)
+    return do_query_one(sql, *args)
 
 
 def select(sql_id: str, *args, **kwargs):
     """
     Execute select SQL and return list(tuple) or empty list if no result.
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
          SELECT * FROM user WHERE name=:name and age=:age   -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
-    sql = get_sql(sql_id, **kwargs)
-    log('dbx.select', sql, *args, **kwargs)
-    sql, args = simple_sql(sql, *args, **kwargs)
-    return db.do_select(sql, *args)
+    _sql_id_log('dbx.select', sql_id, *args, **kwargs)
+    sql, args = get_sql(sql_id, *args, **kwargs)
+    return do_select(sql, *args)
 
 
 def select_one(sql_id: str, *args, **kwargs):
     """
-    Execute select SQL and expected one row result(tuple). Automatically add 'limit ?' after sql statement if not.
+    Execute select SQL and expected one row result(tuple). Automatically add 'limit ?' behind the sql statement if not.
     If no result found, return None.
     If multiple results found, the first one returned.
     sql: SELECT * FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
          SELECT * FROM user WHERE name=:name and age=:age limit 1  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
-    sql = get_sql(sql_id, **kwargs)
-    log('dbx.select_one', sql, *args, **kwargs)
-    sql, args = simple_sql(sql, *args, **kwargs)
-    return db.do_select_one(sql, *args)
+    _sql_id_log('dbx.select_one', sql_id, *args, **kwargs)
+    sql, args = get_sql(sql_id, *args, **kwargs)
+    return do_select_one(sql, *args)
 
 
 def query_page(sql_id: str, page_num=1, page_size=10, *args, **kwargs):
     """
     Execute select SQL and return list or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
          SELECT * FROM user WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
-    sql = get_sql(sql_id, **kwargs)
-    page_log('dbx.query_page', sql, page_num, page_size, *args, **kwargs)
-    sql, args = simple_sql(sql, *args, **kwargs)
-    return db.do_query_page(sql, page_num, page_size, *args)
+    _page_log('dbx.query_page', sql_id, page_num, page_size, *args, **kwargs)
+    sql, args = get_sql(sql_id, *args, **kwargs)
+    return do_query_page(sql, page_num, page_size, *args)
 
 
 def select_page(sql_id: str, page_num=1, page_size=10, *args, **kwargs):
     """
     Execute select SQL and return list or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
          SELECT * FROM user WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
-    sql = get_sql(sql_id, **kwargs)
-    page_log('dbx.select_page', sql, page_num, page_size, *args, **kwargs)
-    sql, args = simple_sql(sql, *args, **kwargs)
-    return db.do_select_page(sql, page_num, page_size, *args)
+    _page_log('dbx.select_page', sql_id, page_num, page_size, *args, **kwargs)
+    sql, args = get_sql(sql_id, *args, **kwargs)
+    return do_select_page(sql, page_num, page_size, *args)
 
 
 def get_connection():
-    return db.get_connection()
+    return _get_connection()
+
+
+def get_sql(sql_id: str, *args, **kwargs):
+    sql_model = get_sql_model(sql_id)
+    return do_get_sql(sql_model, False, None, *args, **kwargs)
+
+
+def do_get_sql(sql_model, batch, param_names, *args, **kwargs):
+    """
+    Get sql from SqlModel.
+    :param sql_model: SqlModel
+    :param batch: bool, is batch or not
+    :param param_names: original function parameter names
+    :param args:
+    :param kwargs:
+    :return:
+    """
+    if sql_model.dynamic:
+        sql = sql_model.sql.render(**kwargs)
+        logging.debug("Original sql: {}".format(sql))
+        return get_named_sql_args(sql, **kwargs)
+    else:
+        logging.debug("Original sql: {}".format(sql_model.sql))
+        if sql_model.mapping and kwargs:
+            return get_named_sql_args(sql_model.sql, **kwargs)
+        elif sql_model.placeholder and kwargs:
+            logging.warning("Better use 'func(arg1, arg2...)' then 'func(arg1=arg1, arg2=arg2...)' if sql contain '?' placeholder.")
+            args = [kwargs[name] for name in param_names if name in kwargs] if param_names else list(kwargs.values())
+        elif sql_model.mapping and not kwargs and (not batch or
+                                                   (batch and (not args or not isinstance(args[0], Mapping)))):  # batch_execute时args可能为List[Mapping]
+            raise MapperError("Parameter 'kwargs' must not be empty when named mapping sql.")
+        return sql_model.sql, args
+
+
+def build_sql_id(namespace, _id):
+    return namespace + "." + _id
+
+
+def get_sql_model(sql_id: str):
+    global _SQL_CONTAINER
+    return _SQL_CONTAINER[sql_id]
 
 
 # ----------------------------------------------------------Load mapper--------------------------------------------------------------------
-# def _get_abs_path(path: str):
-#     parent_flg = '../'
-#     current_flg = './'
-#     if path.startswith(parent_flg):
-#         idx = path.rindex(parent_flg) + 3
-#         parent_path = path[:idx]
-#         os.chdir(parent_path)
-#         path = path[idx:]
-#     elif path.startswith(current_flg):
-#         path = path[2:]
-#     return os.path.join(os.getcwd(), path)
-
-
-def _load_mapper(path: str):
-    # if not os.path.isabs(path):
-    #     path = _get_abs_path(path)
+def load_mapper(path: str):
     if os.path.isfile(path) and path.endswith(".xml"):
         _parse_mapper_file(path)
     elif os.path.isdir(path):
         for f in os.listdir(path):
             file = os.path.join(path, f)
             if os.path.isfile(file) and f.endswith(".xml"):
                 _parse_mapper_file(file)
             elif os.path.isdir(file):
-                _load_mapper(file)
+                load_mapper(file)
 
 
 def _parse_mapper_file(file: str):
+    global _SQL_CONTAINER
     tree = ET.parse(file)
     root = tree.getroot()
     namespace = root.attrib.get('namespace', '')
     results = list(map(lambda child: _load_sql(namespace, child, file), root))
-    sql_ids, file_includes = zip(*results)
-    invalid_includes = [include for includes in file_includes if includes for include in includes if include not in sql_ids]
-    if invalid_includes:
-        raise MapperError("Includes %s are not exist in mapper file: %s" % (set(invalid_includes), file))
-
-
-def get_sql(sql_id: str, **kwargs):
-    sql_model = _get_sql_model(sql_id)
-    if sql_model.includes:
-        for include in sql_model.includes:
-            assert include not in kwargs, "include: '%s' in kwargs: %s" % (include, kwargs)
-            kwargs[include] = get_sql(_build_sql_id(sql_model.namespace, include), **kwargs)
-    return sql_model.sql.render(**kwargs) if sql_model.dynamic else sql_model.sql
-
-
-def _get_sql_model(sql_id: str):
-    global _SQL_CONTAINER
-    return _SQL_CONTAINER[sql_id]
-
-
-def _build_sql_id(namespace, _id):
-    return namespace + "." + _id
+    sql_ids, file_all_includes = zip(*results)
+    for i, includes in enumerate(file_all_includes):
+        if includes:
+            for include in includes:
+                if include not in sql_ids:
+                    raise MapperError("Include '%s' are not exist in mapper file: %s" % (include, file))
+
+                include_sql_id = build_sql_id(namespace, include)
+                include_sql_model = _SQL_CONTAINER[include_sql_id]
+                if include_sql_model.includes:
+                    raise MapperError("Nested include: '%s' include '%s' and it include %s in mapper file: %s" % (
+                        sql_ids[i], include, include_sql_model.includes, file))
+
+    # include sql
+    include_results = filter(lambda x: x[1] is not None, results)
+    for sql_id, includes in include_results:
+        _handle_includes(build_sql_id(namespace, sql_id), includes)
+
+    # dynamic sql change to Template
+    for sql_id in sql_ids:
+        sql_model = _SQL_CONTAINER[build_sql_id(namespace, sql_id)]
+        if sql_model.dynamic:
+            sql_model.sql = Template(sql_model.sql)
+
+
+def _handle_includes(sql_id, includes):
+    is_dynamic = False
+    sql_model = _SQL_CONTAINER[sql_id]
+    for include in includes:
+        include_sql_id = build_sql_id(sql_model.namespace, include)
+        include_sql_model = _SQL_CONTAINER[include_sql_id]
+        if include_sql_model.dynamic:
+            is_dynamic = True
+        if include_sql_model.includes:
+            _handle_includes(include_sql_id, include_sql_model.includes)
+        sql = re.sub(r'{{\s*%s\s*}}' % include, include_sql_model.sql, sql_model.sql)
+
+    _valid_sql(sql_id, sql, sql_model.action)
+    if is_dynamic or is_dynamic_sql(sql):
+        sql_model.dynamic = True
+        sql_model.mapping = True
+        sql_model.placeholder = False
+    else:
+        sql_model.mapping = ':' in sql
+        sql_model.placeholder = False if sql_model.mapping else '?' in sql
+    sql_model.sql = sql
+    sql_model.includes = None
 
 
 def _load_sql(namespace, child, file):
     global _SQL_CONTAINER
-    # child.tag = select
     includes = None
     _id = child.attrib.get('id')
     assert _id, "Mapper 'id' must be set in mapper file: %s." % file
-    sql_id = _build_sql_id(namespace, _id)
+    sql_id = build_sql_id(namespace, _id)
     assert sql_id not in _SQL_CONTAINER, "Sql id '%s' repeat." % sql_id
     include = child.attrib.get('include')
     sql = child.text.strip()
     if include:
         includes = include.split(",")
         for include in set(includes):
             assert include != _id, "Include must not be it self, id: '%s' = include: '%s' " % (_id, include)
-        _SQL_CONTAINER[sql_id] = SqlModel(sql=Template(sql), namespace=namespace, dynamic=True, includes=includes)
+        _SQL_CONTAINER[sql_id] = SqlModel(sql=sql, action=child.tag, namespace=namespace, includes=includes)
     elif is_dynamic_sql(sql):
-        _SQL_CONTAINER[sql_id] = SqlModel(sql=Template(sql), namespace=namespace, dynamic=True)
+        _valid_sql(sql_id, sql, child.tag)
+        _SQL_CONTAINER[sql_id] = SqlModel(sql=sql, action=child.tag, namespace=namespace, dynamic=True)
     else:
-        _SQL_CONTAINER[sql_id] = SqlModel(sql=sql, namespace=namespace)
+        _valid_sql(sql_id, sql, child.tag)
+        _SQL_CONTAINER[sql_id] = SqlModel(sql=sql, action=child.tag, namespace=namespace)
 
     return _id, includes
 
+
+def _sql_id_log(function: str, sql_id: str, *args, **kwargs):
+    logging.debug("Exec func 'mysqlx.%s', sql_id: %s, args: %s, kwargs: %s" % (function, sql_id.strip(), args, kwargs))
+
+
+def _page_log(function: str, sql_id: str, page_num, page_size, *args, **kwargs):
+    logging.debug("Exec func 'mysqlx.%s', page_num: %d, page_size: %d, sql_id: %s, args: %s, kwargs: %s" % (
+        function, page_num, page_size, sql_id.strip(), args, kwargs))
+
+
+def _valid_sql(sql_id, sql, tag):
+    assert tag in _valid_sql_actions and tag in sql.lower(), "Sql id: '{}' has not '{}' key word in {} sql.".format(sql_id, tag, tag)
```

### Comparing `mysqlx-1.3.1/mysqlx/orm.py` & `mysqlx-1.3.2/mysqlx/orm.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 import sys
 import logging
-from . import db
 from enum import IntEnum
-from typing import Any, Mapping, Sequence
+from typing import Sequence, Union, List, Tuple
+from .snowflake import get_id
 from datetime import datetime
-from .support import LIMIT_1, DBError
+from functools import lru_cache
+from .support import LIMIT_1, DBError, PkStrategy, simple_sql
+from .db import do_get_limit, do_query, do_query_one_limit, do_execute, insert, save, do_select, do_select_one_limit, transaction, batch_insert, \
+    do_query_page, do_select_page, do_get
 
 NO_LIMIT = 0
 DEFAULT_PK_FIELD = 'id'
 SYMBOLS = ['=', '>', '<']
 BETWEEN, LIKE, IN = 'between', 'like', 'in'
-PK, TABLE, UPDATE_BY, UPDATE_TIME, DEL_FLAG = '__pk__', '__table__', '__update_by__', '__update_time__', '__del_flag__'
+PK, TABLE, UPDATE_BY, UPDATE_TIME, DEL_FLAG, PK_STRATEGY = '__pk__', '__table__', '__update_by__', '__update_time__', '__del_flag__', '__pk_strategy__'
+_COLUMN_SQL = '''SELECT GROUP_CONCAT(CONCAT("`",column_name,"`") SEPARATOR ",") 
+                 FROM information_schema.columns WHERE table_schema = (SELECT DATABASE()) AND table_name = ? limit ?'''
 
 
 class DelFlag(IntEnum):
     UN_DELETE = 0
     DELETED = 1
 
 
 class Model:
     """
-    Use db.init_db(...) or dbx.init_db(...) init db first, then create a class extends Model:
+    Create a class extends Model:
 
     class User(Model):
         __pk__ = 'id'
         __table__ = 'user'
         __update_by__ = 'update_by'
         __update_time__ = 'update_time'
         __del_flag__ = 'del_flag'
@@ -32,19 +37,24 @@
         def __init__(self, id: int = None, name: str = None, age: int = None, update_by: int = None, update_time: datetime = None, del_flag: int = None):
             self.id = id
             self.update_by = update_by
             self.update_time = update_time
             self.del_flag = del_flag
             self.name = name
             self.age = age
+
+    then you can use like follow:
+        db.init_db(user='xxx', password='xxx', database='xxx', host='xxx', ...)  # or dbx.init_db(...) init db first,
+        user = User(name='张三', age=55)
+        effect_rowcount = user.persist()
+        id = user.inst_save()
     """
 
     def __str__(self):
-        kv = {k: v for k, v in self.__dict__.items() if not k.startswith("__")}
-        return str(kv)
+        return str({k: v for k, v in self.__dict__.items() if not k.startswith("__")})
 
     def __getattr__(self, name):
         if PK == name:
             return self._get_pk()
         elif TABLE == name:
             return self._get_table()
         elif UPDATE_BY == name:
@@ -53,21 +63,34 @@
             return self._get_update_time_field()
         else:
             return None
 
     def persist(self):
         """
         user = User(name='张三', age=55)
-        id = user.persist()
-        :return: Primary key
+        effect_rowcount = user.persist()
+        :return: effect rowcount
         """
         logging.debug("Exec func 'mysqlx.orm.Model.%s', Class: '%s'" % ('persist', self.__class__.__name__))
         kv = {k: v for k, v in self.__dict__.items() if v is not None}
-        self.id = db.save(self._get_table(), **kv)
-        return self.id
+        return self.insert(**kv)
+
+    def inst_save(self):
+        """
+        user = User(name='张三', age=55)
+        id = user.save()
+        :return: Primary key
+        """
+        logging.debug("Exec func 'mysqlx.orm.Model.%s', Class: '%s'" % ('inst_save', self.__class__.__name__))
+        kv = {k: v for k, v in self.__dict__.items() if v is not None}
+        pk = self._get_pk()
+        _id = self.save(**kv)
+        if pk not in kv:
+            self.__dict__.update({pk: _id})
+        return _id
 
     def update(self):
         """
         user = User(id=1, name='李四', age=66)
         rowcount = user.update()
         :return: Effect rowcount
         """
@@ -132,51 +155,75 @@
         """
         logging.debug("Exec func 'mysqlx.orm.Model.%s', Class: '%s'" % ('un_delete', self.__class__.__name__))
         pk = self._get_pk()
         _id = self.__dict__.get(pk)
         update_by = self.__dict__.get(self._get_update_by_field())
         if _id is None:
             raise KeyError("Not primary key.")
-
         return self.un_delete_by_id(_id, update_by)
 
     def physical_delete(self):
         """
         Physical delete
         user = User(id=1)
         rowcount = user.physical_delete()
         """
         logging.debug("Exec func 'mysqlx.orm.Model.%s', Class: '%s'" % ('physical_delete', self.__class__.__name__))
         pk = self._get_pk()
         _id = self.__dict__.get(pk)
         if _id is None:
             raise KeyError("Not primary key.")
-
         return self.physical_delete_by_id(_id)
 
     # ----------------------------------------------------------Class method------------------------------------------------------------------
     @classmethod
     def insert(cls, **kwargs):
         """
         rowcount = User.insert(name='张三', age=20)
         return: Effect rowcount
         """
         _insert_log('insert', cls.__name__, **kwargs)
-        table = cls._get_table()
-        return db.insert(table, **kwargs)
+        pk, table = cls._get_pk_and_table()
+        pk_strategy = cls._get_pk_strategy()
+        if pk_strategy == PkStrategy.SNOWFLAKE.value and pk not in kwargs:
+            kwargs[pk] = get_id()
+        return insert(table, **kwargs)
 
     @classmethod
     def save(cls, **kwargs):
         """
         id = User.save(name='张三', age=20)
         :return: Primary key
         """
         _insert_log('save', cls.__name__, **kwargs)
-        table = cls._get_table()
-        return db.save(table, **kwargs)
+        pk, table = cls._get_pk_and_table()
+        pk_strategy = cls._get_pk_strategy()
+        if pk_strategy == PkStrategy.SNOWFLAKE.value:
+            if pk in kwargs:
+                _id = kwargs[pk]
+            else:
+                _id = get_id()
+                kwargs[pk] = _id
+            insert(table, **kwargs)
+        else:
+            _id = save(table, **kwargs)
+        return _id
+
+    @classmethod
+    def create(cls, **kwargs):
+        """
+        user = User.create(name='张三', age=20)
+        :return: Instance object
+        """
+        _insert_log('create', cls.__name__, **kwargs)
+        pk = cls._get_pk()
+        _id = cls.save(**kwargs)
+        if pk not in kwargs:
+            kwargs[pk] = _id
+        return cls._dict2obj(kwargs)
 
     @classmethod
     def update_by_id(cls, _id: int, **kwargs):
         """
         rowcount = User.update_by_id(id=1, name='王五')
         return: Effect rowcount
         """
@@ -184,15 +231,15 @@
         assert kwargs, 'Must set update kv'
         pk = cls._get_pk()
         where = '`%s`=?' % pk
         cols, args = zip(*kwargs.items())
         sql, update_time_arg = cls._update_sql(where, *cols)
         if update_time_arg:
             args = [*args, update_time_arg]
-        return db.do_execute(sql, *args, _id, LIMIT_1)
+        return do_execute(sql, *args, _id, LIMIT_1)
 
     @classmethod
     def delete_by_id(cls, _id: int, update_by: int = None):
         """
         Logic delete only update the del flag
         rowcount = User.delete_by_id(id=1, update_by=100)
         return: Effect rowcount
@@ -229,36 +276,38 @@
         return: Effect rowcount
         """
         logging.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', ids: %s, update_by: %s, batch_size: %s" % (
             'un_delete_by_ids', cls.__name__, ids, update_by, batch_size))
         return cls._delete_by_ids_op(ids, update_by=update_by, batch_size=batch_size, del_status=DelFlag.UN_DELETE)
 
     @classmethod
-    def physical_delete_by(cls, where: str, *args):
+    def physical_delete_by(cls, where: str, *args, **kwargs):
         """
         Physical delete
         rowcount = User.physical_delete_by('where name=? and age=?', '张三', 55)
         return: Effect rowcount
         """
-        _by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args)
+        _by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
+        assert where.lower().startswith('where'), "Must start with 'WHERE' in the where parameter."
         table = cls._get_table()
         sql = 'DELETE FROM `%s` %s' % (table, where)
-        return db.do_execute(sql, *args)
+        sql, args = simple_sql(sql, *args, **kwargs)
+        return do_execute(sql, *args)
 
     @classmethod
     def physical_delete_by_id(cls, _id: int):
         """
         Physical delete
         rowcount = User.physical_delete_by_id(id=1)
         return: Effect rowcount
         """
         logging.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', id: %d" % ('physical_delete_by_id', cls.__name__, _id))
         pk, table = cls._get_pk_and_table()
         sql = 'DELETE FROM `%s` WHERE `%s`=? limit ?' % (table, pk)
-        return db.do_execute(sql, _id, LIMIT_1)
+        return do_execute(sql, _id, LIMIT_1)
 
     @classmethod
     def physical_delete_by_ids(cls, ids: Sequence[int], batch_size=128):
         """
         Physical delete
         rowcount = User.physical_delete_by_ids(id=[1,2])
         return: Effect rowcount
@@ -270,71 +319,91 @@
 
         if ids_size == 1:
             return cls.physical_delete_by_id(ids[0])
         elif ids_size <= batch_size:
             return cls._physical_delete_by_ids(ids)
         else:
             split_ids = _split_ids(ids, batch_size)
-            with db.transaction():
+            with transaction():
                 results = list(map(cls._physical_delete_by_ids, split_ids))
             return sum(results)
 
     @classmethod
-    def batch_insert(cls, args: Sequence[Mapping[str, Any]]):
+    def batch_insert(cls, *args):
         """
         Batch insert
         rowcount = User.batch_insert([{'name': '张三', 'age': 55},{'name': '李四', 'age': 66}])
         :param args: All number must have same key.
         :return: Effect rowcount
         """
         logging.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', args: %s" % ('batch_insert', cls.__name__, args))
-        table = cls._get_table()
-        return db.batch_insert(table, args)
+        assert len(args) > 0, 'args must not be empty.'
+        pk, table = cls._get_pk_and_table()
+        pk_strategy = cls._get_pk_strategy()
+        if pk_strategy == PkStrategy.SNOWFLAKE.value:
+            for arg in args:
+                if pk not in arg:
+                    arg[pk] = get_id()
+
+        return batch_insert(table, *args)
 
     # ------------------------------------------------Class query method--------------------------------------------------------
     @classmethod
     def count(cls, **kwargs):
         """
         count = User.count(name='张三', age=55)
         """
         logging.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', kwargs: %s" % ('count', cls.__name__, kwargs))
+        table = cls._get_table()
         where, args, _ = _get_where_arg_limit(**kwargs)
         fields = 'count(1)'
-        sql = cls._select_sql(where, LIMIT_1, fields)
-        return db.do_get(sql, *args, LIMIT_1)
+        sql = _select_sql(table, where, LIMIT_1, fields)
+        return do_get_limit(sql, *args, LIMIT_1)
 
     @classmethod
-    def count_by(cls, where: str, *args):
+    def count_by(cls, where: str, *args, **kwargs):
         """
         Automatically add 'limit ?' where if not.
         count = User.count_by('where name=?', '李四')
         """
-        _by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args)
+        _by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
+        assert where.lower().startswith('where'), "Must start with 'where' in the where parameter."
         table = cls._get_table()
-        sql = "SELECT count(1) FROM `%s` %s" % (table, where)
-        return db.do_get(sql, *args)
+        sql = "SELECT count(1) FROM `{}` {}".format(table, where)
+        sql, args = simple_sql(sql, *args, **kwargs)
+        return do_get(sql, *args)
+
+    @classmethod
+    def exists(cls, **kwargs):
+        logging.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', kwargs: %s" % ('exists', cls.__name__, kwargs))
+        return cls.count(**kwargs) > 0
+
+    @classmethod
+    def exists_by(cls, where: str, *args, **kwargs):
+        _by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
+        return cls.count_by(where, *args, **kwargs) > 0
 
     @classmethod
     def find(cls, *fields, **kwargs):
         """
         Return list(object) or empty list if no result.
         users = User.find('id', 'name', 'age', name='张三', age=55)
         :param fields: Default select all fields with 'select *' if not set
         """
         logging.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', fields: %s, kwargs: %s" % ('find', cls.__name__, fields, kwargs))
         return [cls._dict2obj(d) for d in cls.query(*fields, **kwargs)]
 
     @classmethod
-    def find_by(cls, where: str, *args):
+    def find_by(cls, where: str, *args, **kwargs):
         """
         Return list(dict) or empty list if no result.
         rows = User.find_by('where name=?', '李四')
         """
-        _by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args)
-        return [cls._dict2obj(d) for d in cls.query_by(where, *args)]
+        _by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
+        return [cls._dict2obj(d) for d in cls.query_by(where, *args, **kwargs)]
 
     @classmethod
     def find_page(cls, page_num=1, page_size=10, *fields, **kwargs):
         """
         Return list(object) or empty list if no result.
         users = User.find_page(1, 10, 'name', 'age', name='张三', age=55)
         :param page_num: page number
@@ -342,21 +411,21 @@
         :param fields: Default select all fields with 'select *' if not set
         """
         _page_log('find_page', page_num, page_size, cls.__name__, *fields, **kwargs)
         result = cls.query_page(page_num, page_size, *fields, **kwargs)
         return [cls._dict2obj(d) for d in result]
 
     @classmethod
-    def find_by_page(cls, page_num: int, page_size: int, where: str, *args):
+    def find_page_by(cls, page_num: int, page_size: int, where: str, *args, **kwargs):
         """
         Return list(dict) or empty list if no result. Automatically add 'limit ?,?' after where if not.
         rows = User.find_by_page(1, 10, 'where name=?', '李四')
         """
-        _page_log(sys._getframe().f_code.co_name, page_num, page_size, cls.__name__, where, *args)
-        return [cls._dict2obj(d) for d in cls.query_by_page(page_num, page_size, where, *args)]
+        _page_log(sys._getframe().f_code.co_name, page_num, page_size, cls.__name__, where, *args, **kwargs)
+        return [cls._dict2obj(d) for d in cls.query_page_by(page_num, page_size, where, *args, **kwargs)]
 
     @classmethod
     def find_by_id(cls, _id: int, *fields):
         """
         Return one class object or None if no result.
         user = User.find_by_id(1, 'id', 'name', 'age')
         :param _id: pk
@@ -382,228 +451,236 @@
         """
         Return list(dict) or empty list if no result.
         users = User.query('id', 'name', 'age', name='张三', age=55)
         :param fields: Default select all fields with 'select *' if not set
         """
         logging.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', fields: %s, kwargs: %s" % ('query', cls.__name__, fields, kwargs))
         where, args, limit = _get_where_arg_limit(**kwargs)
-        if not limit:
-            limit = 1000
-
-        sql = cls._select_sql(where, limit, *fields)
-        return db.do_query(sql, *args, limit) if limit else db.do_query(sql, *args)
+        table = cls._get_table()
+        sql = _select_sql(table, where, limit, *fields)
+        if limit:
+            if isinstance(limit, int):
+                args = [*args, limit]
+            else:
+                args = [*args, *limit]
+        return do_query(sql, *args)
 
     @classmethod
-    def query_by(cls, where: str, *args):
+    def query_by(cls, where: str, *args, **kwargs):
         """
         Return list(dict) or empty list if no result.
         rows = User.query_by('where name=?', '李四')
         """
-        _by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args)
-        table = cls._get_table()
-        sql = "SELECT * FROM `%s` %s" % (table, where)
-        return db.do_query(sql, *args)
+        _by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
+        sql = cls._where_sql(where)
+        sql, args = simple_sql(sql, *args, **kwargs)
+        return do_query(sql, *args)
 
     @classmethod
     def query_page(cls, page_num=1, page_size=10, *fields, **kwargs):
         """
         Return list(dict) or empty list if no result.
         users = User.query_page(1, 10, 'id', 'name', 'age', name='张三', age=55)
         :param page_num: page number
         :param page_size: page size
         :param fields: Default select all fields with 'select *' if not set
         """
         _page_log('query_page', page_num, page_size, cls.__name__, *fields, **kwargs)
+        table = cls._get_table()
         where, args, _ = _get_where_arg_limit(**kwargs)
-        sql = cls._select_sql(where, NO_LIMIT, *fields)
-        return db.do_query_page(sql, page_num, page_size, *args)
+        sql = _select_sql(table, where, NO_LIMIT, *fields)
+        return do_query_page(sql, page_num, page_size, *args)
 
     @classmethod
-    def query_by_page(cls, page_num: int, page_size: int, where: str, *args):
+    def query_page_by(cls, page_num: int, page_size: int, where: str, *args, **kwargs):
         """
         Return list(dict) or empty list if no result. Automatically add 'limit ?,?' after where if not.
         rows = User.query_by_page(1, 10, 'where name=?', '李四')
         """
-        _page_log(sys._getframe().f_code.co_name, page_num, page_size, cls.__name__, where, *args)
-        table = cls._get_table()
-        sql = "SELECT * FROM `%s` %s" % (table, where)
-        return db.do_query_page(sql, page_num, page_size, *args)
+        _by_page_log(sys._getframe().f_code.co_name, page_num, page_size, cls.__name__, where, *args, **kwargs)
+        sql = cls._where_sql(where)
+        sql, args = simple_sql(sql, *args, **kwargs)
+        return do_query_page(sql, page_num, page_size, *args)
 
     @classmethod
     def query_by_id(cls, _id: int, *fields):
         """
         Return one row(dict) or None if no result.
         user = User.query_by_id(1, 'id', 'name', 'age')
         :param _id: pk
         :param fields: Default select all fields with 'select *' if not set
         """
         logging.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', id: %d, fields: %s" % ('query_by_id', cls.__name__, _id, fields))
-        pk = cls._get_pk()
-        where = 'WHERE `%s`=?' % pk
-        sql = cls._select_sql(where, LIMIT_1, *fields)
-        return db.do_query_one(sql, _id, LIMIT_1)
+        pk, table = cls._get_pk_and_table()
+        where = 'WHERE `{}`=?'.format(pk)
+        sql = _select_sql(table, where, LIMIT_1, *fields)
+        return do_query_one_limit(sql, _id, LIMIT_1)
 
     @classmethod
     def query_by_ids(cls, ids: Sequence[int], *fields):
         """
         Return list(dict) or empty list if no result.
         users = User.query_by_ids([1,2], 'id', 'name', 'age')
         :param ids: List of pk
         :param fields: Default select all fields with 'select *' if not set
         """
         logging.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', ids: %s, fields: %s" % ('query_by_ids', cls.__name__, ids, fields))
         ids_size = len(ids)
         assert ids_size > 0, 'ids must not be empty.'
 
-        pk = cls._get_pk()
-        where = 'WHERE `%s` in (%s)' % (pk, ','.join(['?' for _ in range(ids_size)]))
-        sql = cls._select_sql(where, ids_size, *fields)
-        return db.do_query(sql, *ids, ids_size)
+        pk, table = cls._get_pk_and_table()
+        where = 'WHERE `{}` in ({})'.format(pk, ','.join(['?' for _ in range(ids_size)]))
+        sql = _select_sql(table, where, ids_size, *fields)
+        return do_query(sql, *ids, ids_size)
 
     @classmethod
     def select(cls, *fields, **kwargs):
         """
         Return list(dict) or empty list if no result.
         rows = User.select('id', 'name', 'age', name='张三', age=55)
         :param fields: Default select all fields with 'select *' if not set
         """
         logging.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', fields: %s, kwargs: %s" % ('select', cls.__name__, fields, kwargs))
         where, args, limit = _get_where_arg_limit(**kwargs)
-        if not limit:
-            limit = 1000
-
-        sql = cls._select_sql(where, limit, *fields)
-        return db.do_select(sql, *args, limit) if limit else db.do_select(sql, *args)
+        table = cls._get_table()
+        sql = _select_sql(table, where, limit, *fields)
+        if limit:
+            if isinstance(limit, int):
+                args = [*args, limit]
+            else:
+                args = [*args, *limit]
+        return do_select(sql, *args)
 
     @classmethod
-    def select_by(cls, where: str, *args):
+    def select_by(cls, where: str, *args, **kwargs):
         """
         Return list(dict) or empty list if no result.
         rows = User.select_by('where name=?', '李四')
         """
-        _by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args)
-        table = cls._get_table()
-        sql = "SELECT * FROM `%s` %s" % (table, where)
-        return db.do_select(sql, *args)
+        _by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
+        sql = cls._where_sql(where)
+        sql, args = simple_sql(sql, *args, **kwargs)
+        return do_select(sql, *args)
 
     @classmethod
     def select_page(cls, page_num=1, page_size=10, *fields, **kwargs):
         """
         Return list(dict) or empty list if no result.
         rows = User.select_page('id', 'name', 'age', name='张三', age=55)
         :param page_num: page number
         :param page_size: page size
         :param fields: Default select all fields with 'select *' if not set
         """
         _page_log('select_page', page_num, page_size, cls.__name__, *fields, **kwargs)
+        table = cls._get_table()
         where, args, _ = _get_where_arg_limit(**kwargs)
-        sql = cls._select_sql(where, NO_LIMIT, *fields)
-        return db.do_select_page(sql, page_num, page_size, *args)
+        sql = _select_sql(table, where, NO_LIMIT, *fields)
+        return do_select_page(sql, page_num, page_size, *args)
 
     @classmethod
-    def select_by_page(cls, page_num: int, page_size: int, where: str, *args):
+    def select_page_by(cls, page_num: int, page_size: int, where: str, *args, **kwargs):
         """
         Return list(dict) or empty list if no result. Automatically add 'limit ?,?' after where if not.
         rows = User.select_by_page(1, 10, 'where name=?', '李四')
         """
-        _page_log(sys._getframe().f_code.co_name, page_num, page_size, cls.__name__, where, *args)
-        table = cls._get_table()
-        sql = "SELECT * FROM `%s` %s" % (table, where)
-        return db.do_select_page(sql, page_num, page_size, *args)
+        _by_page_log(sys._getframe().f_code.co_name, page_num, page_size, cls.__name__, where, *args, **kwargs)
+        sql = cls._where_sql(where)
+        sql, args = simple_sql(sql, *args, **kwargs)
+        return do_select_page(sql, page_num, page_size, *args)
 
     @classmethod
     def select_by_id(cls, _id: int, *fields):
         """
         Return one row(dict) or None if no result.
         row = User.select_by_id(1, 'id', 'name', 'age')
         :param _id: pk
         :param fields: Default select all fields with 'select *' if not set
         """
         logging.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', id: %d, fields: %s" % ('select_by_id', cls.__name__, _id, fields))
-        pk = cls._get_pk()
-        where = 'WHERE `%s`=?' % pk
-        sql = cls._select_sql(where, LIMIT_1, *fields)
-        return db.do_select_one(sql, _id, LIMIT_1)
+        pk, table = cls._get_pk_and_table()
+        where = 'WHERE `{}`=?'.format(pk)
+        sql = _select_sql(table, where, LIMIT_1, *fields)
+        return do_select_one_limit(sql, _id, LIMIT_1)
 
     @classmethod
     def select_by_ids(cls, ids: Sequence[int], *fields):
         """
         Return list(dict) or empty list if no result.
         rows = User.select_by_ids([1,2], 'id', 'name', 'age')
         :param ids: List of pk
         :param fields: Default select all fields with 'select *' if not set
         """
         logging.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', ids: %s, fields: %s" % ('select_by_ids', cls.__name__, ids, fields))
         ids_size = len(ids)
         assert ids_size > 0, 'ids must not be empty.'
 
-        pk = cls._get_pk()
-        where = 'WHERE `%s` in (%s)' % (pk, ','.join(['?' for _ in range(ids_size)]))
-        sql = cls._select_sql(where, ids_size, *fields)
-        return db.do_select(sql, *ids, ids_size)
+        pk, table = cls._get_pk_and_table()
+        where = 'WHERE `{}` in ({})'.format(pk, ','.join(['?' for _ in range(ids_size)]))
+        sql = _select_sql(table, where, ids_size, *fields)
+        return do_select(sql, *ids, ids_size)
 
     # ------------------------------------------------Private class method------------------------------------------------------------------
     @classmethod
     def _delete_by_id_op(cls, _id: int, update_by: int = None, del_status=DelFlag.DELETED):
         pk, table = cls._get_pk_and_table()
         del_flag_field = cls._get_del_flag_field()
         update_by_field = cls._get_update_by_field()
 
         where = '`%s`=?' % pk
         if update_by is not None and update_by_field is not None:
             sql, update_time_arg = cls._update_sql(where, del_flag_field, update_by_field)
             if update_time_arg:
-                return db.do_execute(sql, del_status.value, update_by, update_time_arg, _id, LIMIT_1)
-            return db.do_execute(sql, del_status.value, update_by, _id, LIMIT_1)
+                return do_execute(sql, del_status.value, update_by, update_time_arg, _id, LIMIT_1)
+            return do_execute(sql, del_status.value, update_by, _id, LIMIT_1)
         else:
             sql, update_time_arg = cls._update_sql(where, del_flag_field)
             if update_time_arg:
-                return db.do_execute(sql, del_status.value, update_time_arg, _id, LIMIT_1)
-            return db.do_execute(sql, del_status.value, _id, LIMIT_1)
+                return do_execute(sql, del_status.value, update_time_arg, _id, LIMIT_1)
+            return do_execute(sql, del_status.value, _id, LIMIT_1)
 
     @classmethod
     def _delete_by_ids_op(cls, ids: Sequence[int], update_by: int = None, batch_size=128, del_status=DelFlag.DELETED):
         ids_size = len(ids)
         assert ids_size > 0, 'ids must not be empty.'
 
         if ids_size == 1:
             return cls._delete_by_id_op(ids[0], update_by, del_status)
         elif ids_size <= batch_size:
             return cls._do_delete_by_ids(ids, update_by, del_status)
         else:
             split_ids = _split_ids(ids, batch_size)
-            with db.transaction():
+            with transaction():
                 results = [cls._do_delete_by_ids(ids, update_by, del_status) for ids in split_ids]
             return sum(results)
 
     @classmethod
     def _do_delete_by_ids(cls, ids: Sequence[int], update_by: int = None, del_status=DelFlag.DELETED):
         ids_size = len(ids)
         pk = cls._get_pk()
         del_flag_field = cls._get_del_flag_field()
         update_by_field = cls._get_update_by_field()
 
         where = '`%s` in (%s)' % (pk, ','.join(['?' for _ in range(ids_size)]))
         if update_by is not None and update_by_field is not None:
             sql, update_time_arg = cls._update_sql(where, del_flag_field, update_by_field)
             if update_time_arg:
-                return db.do_execute(sql, del_status.value, update_by, update_time_arg, *ids, ids_size)
-            return db.do_execute(sql, del_status.value, update_by, *ids, ids_size)
+                return do_execute(sql, del_status.value, update_by, update_time_arg, *ids, ids_size)
+            return do_execute(sql, del_status.value, update_by, *ids, ids_size)
         else:
             sql, update_time_arg = cls._update_sql(where, del_flag_field)
             if update_time_arg:
-                return db.do_execute(sql, del_status.value, update_time_arg, *ids, ids_size)
-            return db.do_execute(sql, del_status.value, *ids, ids_size)
+                return do_execute(sql, del_status.value, update_time_arg, *ids, ids_size)
+            return do_execute(sql, del_status.value, *ids, ids_size)
 
     @classmethod
     def _physical_delete_by_ids(cls, ids: Sequence[int]):
         ids_size = len(ids)
         pk, table = cls._get_pk_and_table()
-        sql = 'DELETE FROM `%s` WHERE `%s` in (%s) limit ?' % (table, pk, ','.join(['?' for _ in range(ids_size)]))
-        return db.do_execute(sql, *ids, ids_size)
+        sql = 'DELETE FROM `{}` WHERE `{}` in ({}) limit ?'.format(table, pk, ','.join(['?' for _ in range(ids_size)]))
+        return do_execute(sql, *ids, ids_size)
 
     @classmethod
     def _get_pk(cls):
         if hasattr(cls, PK):
             return cls.__pk__
         logging.warning("%s not set attribute '%s'" % (cls.__name__, PK))
         return DEFAULT_PK_FIELD
@@ -616,17 +693,23 @@
         return _get_table_name(cls.__name__)
 
     @classmethod
     def _get_pk_and_table(cls):
         return cls._get_pk(), cls._get_table()
 
     @classmethod
+    def _get_pk_strategy(cls):
+        if hasattr(cls, PK_STRATEGY):
+            return cls.__pk_strategy__
+        return None
+
+    @classmethod
     def _dict2obj(cls, dictionary):
         m = cls.__new__(cls)
-        m.__init__(**dictionary)
+        m.__dict__.update(dictionary)
         return m
 
     @classmethod
     def _get_update_by_field(cls):
         if hasattr(cls, UPDATE_BY):
             return cls.__update_by__
         return None
@@ -639,97 +722,152 @@
 
     @classmethod
     def _get_del_flag_field(cls):
         assert hasattr(cls, DEL_FLAG), "%s not set attribute '%s'" % (cls.__name__, DEL_FLAG)
         return cls.__del_flag__
 
     @classmethod
-    def _select_sql(cls, where, limit, *fields):
-        table = cls._get_table()
-        if not fields:
-            fields = '*'
-        else:
-            fields = ','.join(['%s' % col if '(' in col else '`%s`' % col for col in fields])
-
-        if limit:
-            return 'SELECT %s FROM `%s` %s limit ?' % (fields, table, where)
-        else:
-            return 'SELECT %s FROM `%s` %s' % (fields, table, where)
-
-    @classmethod
     def _update_sql(cls, where, *update_fields):
         update_time_arg = None
         table = cls._get_table()
         update_time_field = cls._get_update_time_field()
         if update_time_field is not None and update_time_field not in update_fields:
             update_fields = [*update_fields, update_time_field]
             update_time_arg = datetime.now()
 
-        update_fields = ','.join(['`%s`=?' % col for col in update_fields])
-        return 'UPDATE `%s` SET %s WHERE %s limit ?' % (table, update_fields, where), update_time_arg
+        update_fields = ','.join(['`{}`=?'.format(col) for col in update_fields])
+        return 'UPDATE `{}` SET {} WHERE {} limit ?'.format(table, update_fields, where), update_time_arg
+
+    @classmethod
+    def _where_sql(cls, where: str):
+        low_where = where.lower()
+        if low_where.startswith('where'):
+            table = cls._get_table()
+            return _select_sql(table, where, NO_LIMIT)
+        elif low_where.startswith('select'):
+            return where
+        raise DBError("The where parameter must be a complete SQL statement or conditions start with 'where'")
 
 
 # ----------------------------------------------------------Private function------------------------------------------------------------------
-def _get_condition_arg(k, v):
-    if not isinstance(v, str):
-        return "`%s`=?" % k, v
+def _select_sql(table: str, where: str, limit: Union[int, Tuple[int], List[int]], *fields):
+    if fields:
+        fields = ','.join([col if '(' in col else '`{}`'.format(col) for col in fields])
+    else:
+        fields = _get_table_columns(table)
 
-    v_lower = v.lower()
-    if any([symbol in SYMBOLS for symbol in v_lower]):
-        return "`%s`%s" % (k, v), None
-    elif BETWEEN in v_lower or LIKE in v_lower or IN in v_lower:
-        return "`%s` %s" % (k, v), None
+    if limit:
+        if isinstance(limit, int):
+            return 'SELECT {} FROM `{}` {} limit ?'.format(fields, table, where)
+        elif (isinstance(limit, Tuple) or isinstance(limit, List)) and len(limit) == 2:
+            return 'SELECT {} FROM `{}` {} limit ?,?'.format(fields, table, where)
+        else:
+            raise ValueError("The type of the parameter 'limit' must be 'int' or tuple, list, and it length is 2.")
     else:
-        return "`%s`=?" % k, v
+        return 'SELECT {} FROM `{}` {}'.format(fields, table, where)
+
+
+@lru_cache(maxsize=128)
+def _get_table_columns(table: str):
+    return do_get_limit(_COLUMN_SQL, table, LIMIT_1)
+
+
+def _physical_delete_by_id_sql(table, pk):
+    return 'DELETE FROM `{}` WHERE `{}`=? limit ?'.format(table, pk)
+
+
+def _get_condition_arg(k: str, v: object):
+    if k.endswith("__eq"):
+        return "`{}`=?".format(k[:-4]), v
+    if k.endswith("__gt"):
+        return "`{}`>?".format(k[:-4]), v
+    if k.endswith("__lt"):
+        return "`{}`<?".format(k[:-4]), v
+    if k.endswith("__ge"):
+        return "`{}`>=?".format(k[:-4]), v
+    if k.endswith("__gte"):
+        return "`{}`>=?".format(k[:-5]), v
+    if k.endswith("__le"):
+        return "`{}`<=?".format(k[:-4]), v
+    if k.endswith("__lte"):
+        return "`{}`<=?".format(k[:-5]), v
+    if k.endswith("__in") and isinstance(v, Sequence) and not isinstance(v, str):
+        return "`{}` in ({})".format(k[:-4], ','.join(['?' for _ in v])), v
+    if k.endswith("__in"):
+        return "`{}` in ({})".format(k[:-4], '?'), v
+    if k.endswith("__startswith"):
+        return "`{}` like ?".format(k[:-12]), '{}%'.format(v)
+    if k.endswith("__endswith"):
+        return "`{}` like ?".format(k[:-10]), '%{}'.format(v)
+    if k.endswith("__contains"):
+        return "`{}` like ?".format(k[:-10]), '%{}%'.format(v)
+    if k.endswith("__between") and isinstance(v, Sequence) and 2 == len(v) and not isinstance(v, str):
+        return "`{}` between ? and ?".format(k[:-9]), v
+    if k.endswith("__between"):
+        return ValueError("Must is instance of Sequence with length 2 when use between statement")
+
+    if not isinstance(v, str):
+        return "`{}`=?".format(k), v
+    lower_v = v.lower()
+    if any([symbol in SYMBOLS for symbol in lower_v]):
+        return "`{}`{}".format(k, v), None
+    elif BETWEEN in lower_v or LIKE in lower_v or IN in lower_v:
+        return "`{}` {}".format(k, v), None
+    else:
+        return "`{}`=?".format(k), v
 
 
 def _get_where_arg_limit(**kwargs):
     where, args, limit = '', [], 0
     if 'limit' in kwargs:
         limit = kwargs.get('limit')
         del kwargs['limit']
 
     if kwargs:
-        conditions, args = zip(*[_get_condition_arg(k, v) for k, v in kwargs.items()])
-        args = [arg for arg in args if arg is not None]
-        where = 'WHERE %s' % ' and '.join(conditions)
+        conditions, tmp_args = zip(*[_get_condition_arg(k, v) for k, v in kwargs.items()])
+        tmp_args = [arg for arg in tmp_args if arg is not None]
+
+        for arg in tmp_args:
+            if arg:
+                if isinstance(arg, Sequence) and not isinstance(arg, str):
+                    args.extend(arg)
+                else:
+                    args.append(arg)
+        where = 'WHERE {}'.format(' and '.join(conditions))
 
     return where, args, limit
 
 
 def _split_ids(ids: Sequence[int], batch_size):
     ids_size = len(ids)
-    mod = ids_size % batch_size
     n = ids_size // batch_size
-    if mod != 0:
-        n += 1
-
+    n += 0 if ids_size % batch_size == 0 else 1
     return [ids[i:i + batch_size] for i in range(0, ids_size, batch_size)]
 
 
 def _get_table_name(class_name):
     for i in range(1, len(class_name) - 1)[::-1]:
         if class_name[i].isupper():
             class_name = class_name[:i] + '_' + class_name[i:]
     return class_name.lower()
 
 
-def _page_log(function, page_num, page_size, class_name, where, *args):
-    logging.debug("Exec func 'mysqlx.orm.Model.%s', page_num: %d, page_size: %d \n\t\t Class: '%s', where: %s, args: %s" % (
-        function, page_num, page_size, class_name, where, args))
+def _by_page_log(function, page_num, page_size, class_name, where, *args, **kwargs):
+    logging.debug("Exec func 'mysqlx.orm.Model.%s', page_num: %d, page_size: %d \n\t\t Class: '%s', where: %s, args: %s, kwargs: %s" % (
+        function, page_num, page_size, class_name, where, args, kwargs))
 
 
-def _by_page_log(function, page_num, page_size, class_name, *fields, **kwargs):
+def _page_log(function, page_num, page_size, class_name, *fields, **kwargs):
     logging.debug("Exec func 'mysqlx.orm.Model.%s', page_num: %d, page_size: %d \n\t\t Class: '%s', fields: %s, kwargs: %s" % (
         function, page_num, page_size, class_name, fields, kwargs))
 
 
 def _insert_log(function, class_name, **kwargs):
     logging.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', kwargs: %s" % (function, class_name, kwargs))
 
 
 def _delete_by_id_log(function, class_name, _id, update_by):
     logging.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', id: %d, update_by: %s" % (function, class_name, _id, update_by))
 
 
-def _by_log(function, class_name, where, *args):
-    logging.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', where: %s, args: %s" % (function, class_name, where, args))
+def _by_log(function, class_name, where, *args, **kwargs):
+    logging.debug("Exec func 'mysqlx.orm.Model.%s' \n\t\t Class: '%s', where: %s, args: %s, kwargs: %s" % (function, class_name, where, args, kwargs))
```

### Comparing `mysqlx-1.3.1/mysqlx/support.py` & `mysqlx-1.3.2/mysqlx/support.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 import re
 import logging
 import threading
+from enum import Enum
+from typing import Sequence
 from jinja2 import Template
+from functools import lru_cache
 
 LIMIT_1 = 1
 _REGEX = r':[\w|\d]*'
 DYNAMIC_REGEX = '{%|{{|}}|%}'
+DB_LOCK = threading.RLock()
+
+
+def get_batch_args(*args):
+    return args[0] if isinstance(args, tuple) and len(args) == 1 and isinstance(args[0], Sequence) else args
 
 
 def try_commit(db_ctx):
     if db_ctx.transactions == 0:
         logging.debug('Commit transaction...')
         try:
             db_ctx.connection.commit()
@@ -17,86 +25,98 @@
         except Exception:
             logging.warning('Commit failed, try rollback...')
             db_ctx.connection.rollback()
             logging.warning('Rollback ok.')
             raise
 
 
-def simple_sql(sql, *args, **kwargs):
+def simple_sql(sql: str, *args, **kwargs):
     return get_named_sql_args(sql, **kwargs) if kwargs else (sql, args)
 
 
-def is_dynamic_sql(sql: str):
-    return re.search(DYNAMIC_REGEX, sql)
-
-
-def dynamic_sql(sql, *args, **kwargs):
+def dynamic_sql(sql: str, *args, **kwargs):
     if kwargs:
-        if is_dynamic_sql(sql):
+        if _is_dynamic_sql(sql):
             sql = Template(sql).render(**kwargs)
         return get_named_sql_args(sql, **kwargs)
 
     return sql, args
 
 
-def log(function: str, sql: str, *args, **kwargs):
-    logging.debug("Exec func 'mysqlx.%s' \n\t\tsql: %s \n\t\targs: %s \n\t\tkwargs: %s" % (function, sql.strip(), args, kwargs))
+def is_dynamic_sql(sql: str):
+    return re.search(DYNAMIC_REGEX, sql)
 
 
-def page_log(function: str, sql: str, page_num, page_size, *args, **kwargs):
-    logging.debug("Exec func 'mysqlx.%s', page_num: %d, page_size: %d \n\t\tsql: %s \n\t\targs: %s \n\t\tkwargs: %s" % (
-        function, page_num, page_size, sql.strip(), args, kwargs))
+@lru_cache(maxsize=128)
+def _is_dynamic_sql(sql: str):
+    return True if is_dynamic_sql(sql) else False
 
 
 def get_named_sql_args(sql: str, **kwargs):
     args = get_named_args(sql, **kwargs)
     return get_named_sql(sql), args
 
 
+@lru_cache(maxsize=256)
 def get_named_sql(sql: str):
     return re.sub(_REGEX, '?', sql)
 
 
 def get_named_args(sql: str, **kwargs):
     return [kwargs[r[1:]] for r in re.findall(_REGEX, sql)]
 
 
+def log(function: str, sql: str, *args, **kwargs):
+    logging.debug("Exec func 'mysqlx.%s' \n\t\tsql: %s \n\t\targs: %s \n\t\tkwargs: %s" % (function, sql.strip(), args, kwargs))
+
+
+def page_log(function: str, sql: str, page_num, page_size, *args, **kwargs):
+    logging.debug("Exec func 'mysqlx.%s', page_num: %d, page_size: %d \n\t\tsql: %s \n\t\targs: %s \n\t\tkwargs: %s" % (
+        function, page_num, page_size, sql.strip(), args, kwargs))
+
+
 class DBCtx(threading.local):
     """
     Thread local object that holds connection info.
     """
 
-    def __init__(self, connect):
+    def __init__(self, connect, use_mysql_connector):
         self.connect = connect
         self.connection = None
         self.transactions = 0
         self.prepared = True
+        if use_mysql_connector:
+            self.get_cursor = lambda: self.connection.cursor(prepared=self.prepared)
+            self.log = lambda action: logging.debug('%s connection <%s>...' % (action, hex(id(self.connection._cnx))))
+        else:
+            self.get_cursor = lambda: self.connection.cursor()
+            self.log = lambda action: logging.debug('%s connection <%s>...' % (action, hex(id(self.connection))))
 
     def is_not_init(self):
         return self.connection is None
 
     def init(self):
         self.transactions = 0
         self.connection = self.connect()
-        logging.debug('Use connection <%s>...' % hex(id(self.connection._cnx)))
+        self.log('Use')
 
     def release(self):
         if self.connection:
-            logging.debug('Release connection <%s>...' % hex(id(self.connection._cnx)))
+            self.log('Release')
             self.connection.close()
             self.connection = None
 
     def cursor(self):
         """
         Return cursor
         """
         # logging.debug('Cursor prepared: %s' % self.prepared)
-        return self.connection.cursor(prepared=self.prepared)
+        return self.get_cursor()
 
-    def statement(self, sql):
+    def statement(self, sql: str):
         """
         Return statement
         """
         return self.connection.statement(sql)
 
 
 class ConnectionCtx(object):
@@ -220,12 +240,38 @@
 
     def __setattr__(self, key, value):
         self[key] = value
 
 
 class SqlModel:
     from typing import List
-    def __init__(self, sql: str, namespace: str, dynamic=False, includes: List[str] = None):
+    def __init__(self, sql: str, action: str, namespace: str, dynamic=False, includes: List[str] = None):
         self.sql = sql
+        self.action = action
         self.namespace = namespace
         self.dynamic = dynamic
         self.includes = includes
+        self.mapping = True if dynamic else ':' in sql
+        self.placeholder = False if self.mapping else '?' in sql
+
+
+class SqlAction(Enum):
+    CALL = 'call'
+    INSERT = 'insert'
+    UPDATE = 'update'
+    DELETE = 'delete'
+    SELECT = 'select'
+
+
+class PkStrategy(Enum):
+    """
+    DB: 由数据库的AUTO_INCREMENT自动生成主键
+    SNOWFLAKE: 由Snowflake算法生成主键
+
+    在Windows上，使用Snowflake可能会报下列错误，这是因为Snowflake生成的id是15位的数字，而Windows上C语言的long类型是32位的
+    OverflowError: Python int too large to convert to C long
+
+    如果用的是mysql.connector，且在Windows上开发测试，可以就在初始化数据库的时候加上参数'use_pure'为True用纯python的connect; 在linux是部署生成环境时去掉'use_pure'用
+    C语言写的connect, 以提高性能.
+    """
+    DB = 'db'
+    SNOWFLAKE = 'snowflake'
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mysqlx-1.3.1/mysqlx.egg-info/PKG-INFO` & `mysqlx-1.3.2/test/db_test.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,132 +1,132 @@
-Metadata-Version: 2.1
-Name: mysqlx
-Version: 1.3.1
-Summary: MySqlx is a simple python sql executor for MySQL like iBatis.
-Home-page: https://gitee.com/summry/mysqlx
-Author: summry
-Author-email: xiazhongbiao@126.com
-License: UNKNOWN
-Keywords: sql,MySQL,iBatis,MyBatis,python
-Platform: UNKNOWN
-Requires-Python: >=3.6.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-Install
-'''''''
-
-::
-
-   pip install mysqlx
-
-Usage Sample
-''''''''''''
-
-::
-
-   CREATE TABLE `user` (
-     `id` bigint NOT NULL AUTO_INCREMENT,
-     `name` varchar(45) NOT NULL,
-     `age` int NOT NULL,
-     `birth_date` date DEFAULT NULL,
-     `sex` tinyint DEFAULT NULL,
-     `grade` float DEFAULT NULL,
-     `point` double DEFAULT NULL,
-     `money` decimal(8,4) DEFAULT NULL,
-     `create_by` bigint DEFAULT NULL,
-     `create_time` datetime DEFAULT CURRENT_TIMESTAMP,
-     `update_by` bigint DEFAULT NULL,
-     `update_time` datetime DEFAULT NULL,
-     `del_flag` tinyint NOT NULL DEFAULT '0',
-     PRIMARY KEY (`id`)
-   ) ENGINE=InnoDB AUTO_INCREMENT=62 DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_0900_ai_ci
-
-
-   ----------------------------------------------------------------------------------------
-
-   from mysqlx import db
-
-   db_conf = {
-       'host': '127.0.0.1',
-       'port': 3306, 
-       'user': 'root', 
-       'password': 'xxx', 
-       'database': 'test',
-       'pool_size': 5,
-       'show_sql': True
-   }
-
-   if __name__ == '__main__':
-       db.init_db(**db_conf)
-       
-       # Return effect rowcount
-       rowcount = db.insert('user', name='寮犱笁', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
-       assert rowcount == 1, '1 effect rowcount'
-       assert db.get('select count(1) from user') == 1, 'count is 1'
-
-       # Return primary key
-       id2 = db.save('user', name='鏉庡洓', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
-       assert db.get('select count(1) from user') == 2, 'count is 2'
-
-       db.execute('update user set name=? where id=?', '鐜嬩簲', id2)
-       assert db.get('select name from user where id=?', id2) == '鐜嬩簲', 'execute'
-
-       db.execute('update user set name=:name where id=:id', name='璧靛叚', id=id2)
-       assert db.select_one('select id, name from user where id=:id', id=id2)[0] == id2, 'execute'
-
-       db.execute('update user set name=:name where id=:id', name='璧靛叚', id=id2)
-       assert db.query_one('select name from user where id=:id', id=id2)['name'] == '璧靛叚', 'execute'
-
-       args = [
-           ('寮犱笁', 55, '1968=-10-08', 0, 1.0, 20.5, 854.56),
-           ('寮犱笁', 55, '1968=-10-08', 0, 1.0, 20.5, 854.56)
-       ]
-       db.batch_execute('insert into user(name, age, birth_date, sex, grade, point, money) values(?,?,?,?,?,?,?)', args)
-       users = db.select('select id, del_flag from user')
-       assert len(users) == 4, 'batch_execute'
-       users = db.query('select id, del_flag from user')
-       assert len(users) == 4, 'batch_execute'
-
-       users = db.select('select id, del_flag from user where id=?', id2)
-       assert len(users) == 1, 'select'
-       users = db.query('select id, del_flag from user where id=?', id2)
-       assert len(users) == 1, 'select'
-
-       users = db.select('select id, del_flag from user where id=:id', id=id2)
-       assert len(users) == 1, 'select'
-       users = db.query('select id, del_flag from user where id=:id', id=id2)
-       assert len(users) == 1, 'select'
-
-       db.execute('delete from user where id=? limit 1', id2)
-       assert db.get('select count(1) from user') == 3, 'execute delete'
-
-Transaction
-'''''''''''
-
-::
-
-   @db.with_transaction
-   def test_transaction():
-       db.insert('user', name='寮犱笁', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
-       db.insert('user', name='鏉庡洓', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
-
-
-   def test_transaction2():
-       with db.transaction():
-           db.insert('user', name='寮犱笁', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
-           db.insert('user', name='鏉庡洓', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
-
-Note: the functions return type
-'''''''''''''''''''''''''''''''
-
-::
-
-   get: Return only one object, like count
-   query_one: Return one row with dict
-   select_one: Return one row with tuple
-   find_by_id: Return one row with class instance object
-   query: Return list of dict
-   select: Return list of tuple
-   find: Return list of class instance object
+import logging
+from mysqlx import db
+from config import DB_CONF
+
+create_table_sql = '''
+CREATE TABLE `user` (
+  `id` bigint unsigned NOT NULL AUTO_INCREMENT,
+  `name` varchar(45) NOT NULL,
+  `age` int unsigned NOT NULL,
+  `birth_date` date DEFAULT NULL,
+  `sex` tinyint unsigned DEFAULT NULL,
+  `grade` float DEFAULT NULL,
+  `point` double DEFAULT NULL,
+  `money` decimal(8,4) DEFAULT NULL,
+  `create_by` bigint DEFAULT NULL,
+  `create_time` datetime DEFAULT CURRENT_TIMESTAMP,
+  `update_by` bigint DEFAULT NULL,
+  `update_time` datetime DEFAULT NULL,
+  `del_flag` tinyint NOT NULL DEFAULT '0',
+  PRIMARY KEY (`id`)
+) ENGINE=InnoDB AUTO_INCREMENT=62 DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_0900_ai_ci
+'''
+
+
+def create_truncate_table(table):
+    cnt = db.do_get("SELECT count(1) FROM information_schema.TABLES WHERE table_schema=database() AND table_name=?", table)
+    if cnt == 0:
+        db.do_execute(create_table_sql)
+    else:
+        db.do_execute('truncate table %s' % table)
+
+
+def drop_table():
+    db.execute('DROP TABLE IF EXISTS user')
+
+
+@db.with_transaction
+def test_transaction(rollback: bool = False):
+    db.insert('user', name='张三', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
+    assert db.get('select count(1) from user limit 1') == 4, 'transaction'
+    if rollback:
+        1 / 0
+    db.save('user', name='李四', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
+
+
+def test_transaction2(rollback: bool = False):
+    with db.transaction():
+        db.insert('user', name='张三', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
+        assert db.get('select count(1) from user') == 6, 'transaction2'
+        if rollback:
+            1 / 0
+        db.save('user', name='李四', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
+
+
+def full_test():
+    create_truncate_table('user')
+    #######################################################################################################
+
+    rowcount = db.insert('user', name='张三', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
+    assert rowcount == 1, 'insert'
+    assert db.get('select count(1) from user') == 1, 'insert'
+
+    id2 = db.save('user', name='李四', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
+    assert id2 > 0, 'save'
+    assert db.get('select count(1) from user') == 2, 'save'
+
+    db.execute('update user set name=? where id=?', '王五', id2)
+    assert db.get('select name from user where id=?', id2) == '王五', 'execute'
+
+    db.execute('update user set name=:name where id=:id', name='赵六', id=id2)
+    assert db.select_one('select id, name from user where id=:id', id=id2)[0] == id2, 'execute'
+
+    db.execute('update user set name=:name where id=:id', name='赵六', id=id2)
+    assert db.query_one('select name from user where id=:id', id=id2)['name'] == '赵六', 'execute'
+
+    args = [
+        ('张三', 55, '1968=-10-08', 0, 1.0, 20.5, 854.56),
+        ('张三', 55, '1968=-10-08', 0, 1.0, 20.5, 854.56)
+    ]
+    db.batch_execute('insert into user(name, age, birth_date, sex, grade, point, money) values(?,?,?,?,?,?,?)', *args)
+    users = db.select('select id, del_flag from user')
+    assert len(users) == 4, 'batch_execute'
+    users = db.query('select id, del_flag from user')
+    assert len(users) == 4, 'batch_execute'
+
+    users = db.select('select id, del_flag from user where id=?', id2)
+    assert len(users) == 1, 'select'
+    users = db.query('select id, del_flag from user where id=?', id2)
+    assert len(users) == 1, 'select'
+
+    users = db.select('select id, del_flag from user where id=:id', id=id2)
+    assert len(users) == 1, 'select'
+    users = db.query('select id, del_flag from user where id=:id', id=id2)
+    assert len(users) == 1, 'select'
+
+    db.execute('delete from user where id=? limit 1', id2)
+    assert db.get('select count(1) from user') == 3, 'execute delete'
+
+    try:
+        test_transaction(rollback=True)
+    except Exception:
+        print('Rollback.')
+    assert db.get('select count(1) from user') == 3, 'transaction'
+
+    test_transaction(rollback=False)
+    assert db.get('select count(1) from user') == 5, 'transaction'
+
+    try:
+        test_transaction2(rollback=True)
+    except Exception:
+        print('Rollback.')
+    assert db.get('select count(1) from user') == 5, 'transaction2'
+
+    test_transaction2(rollback=False)
+    assert db.get('select count(1) from user') == 7, 'transaction2'
+
+
+if __name__ == '__main__':
+    logging.basicConfig(level=logging.DEBUG, format='[%(levelname)s]: %(asctime)s %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
+    db.init_db(**DB_CONF, pool_size=2)
+    # drop_table()
+    full_test()
+
+
+    # for u in db.select('select * from user'):
+    #     print(u)
+    #
+    # for u in db.select_page('select * from user', 2, 3):
+    #     print(u)
+
```

### Comparing `mysqlx-1.3.1/PKG-INFO` & `mysqlx-1.3.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,132 +1,97 @@
-Metadata-Version: 2.1
-Name: mysqlx
-Version: 1.3.1
-Summary: MySqlx is a simple python sql executor for MySQL like iBatis.
-Home-page: https://gitee.com/summry/mysqlx
-Author: summry
-Author-email: xiazhongbiao@126.com
-License: UNKNOWN
-Keywords: sql,MySQL,iBatis,MyBatis,python
-Platform: UNKNOWN
-Requires-Python: >=3.6.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-Install
-'''''''
-
-::
-
-   pip install mysqlx
-
-Usage Sample
-''''''''''''
-
-::
-
-   CREATE TABLE `user` (
-     `id` bigint NOT NULL AUTO_INCREMENT,
-     `name` varchar(45) NOT NULL,
-     `age` int NOT NULL,
-     `birth_date` date DEFAULT NULL,
-     `sex` tinyint DEFAULT NULL,
-     `grade` float DEFAULT NULL,
-     `point` double DEFAULT NULL,
-     `money` decimal(8,4) DEFAULT NULL,
-     `create_by` bigint DEFAULT NULL,
-     `create_time` datetime DEFAULT CURRENT_TIMESTAMP,
-     `update_by` bigint DEFAULT NULL,
-     `update_time` datetime DEFAULT NULL,
-     `del_flag` tinyint NOT NULL DEFAULT '0',
-     PRIMARY KEY (`id`)
-   ) ENGINE=InnoDB AUTO_INCREMENT=62 DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_0900_ai_ci
-
-
-   ----------------------------------------------------------------------------------------
-
-   from mysqlx import db
-
-   db_conf = {
-       'host': '127.0.0.1',
-       'port': 3306, 
-       'user': 'root', 
-       'password': 'xxx', 
-       'database': 'test',
-       'pool_size': 5,
-       'show_sql': True
-   }
-
-   if __name__ == '__main__':
-       db.init_db(**db_conf)
-       
-       # Return effect rowcount
-       rowcount = db.insert('user', name='寮犱笁', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
-       assert rowcount == 1, '1 effect rowcount'
-       assert db.get('select count(1) from user') == 1, 'count is 1'
-
-       # Return primary key
-       id2 = db.save('user', name='鏉庡洓', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
-       assert db.get('select count(1) from user') == 2, 'count is 2'
-
-       db.execute('update user set name=? where id=?', '鐜嬩簲', id2)
-       assert db.get('select name from user where id=?', id2) == '鐜嬩簲', 'execute'
-
-       db.execute('update user set name=:name where id=:id', name='璧靛叚', id=id2)
-       assert db.select_one('select id, name from user where id=:id', id=id2)[0] == id2, 'execute'
-
-       db.execute('update user set name=:name where id=:id', name='璧靛叚', id=id2)
-       assert db.query_one('select name from user where id=:id', id=id2)['name'] == '璧靛叚', 'execute'
-
-       args = [
-           ('寮犱笁', 55, '1968=-10-08', 0, 1.0, 20.5, 854.56),
-           ('寮犱笁', 55, '1968=-10-08', 0, 1.0, 20.5, 854.56)
-       ]
-       db.batch_execute('insert into user(name, age, birth_date, sex, grade, point, money) values(?,?,?,?,?,?,?)', args)
-       users = db.select('select id, del_flag from user')
-       assert len(users) == 4, 'batch_execute'
-       users = db.query('select id, del_flag from user')
-       assert len(users) == 4, 'batch_execute'
-
-       users = db.select('select id, del_flag from user where id=?', id2)
-       assert len(users) == 1, 'select'
-       users = db.query('select id, del_flag from user where id=?', id2)
-       assert len(users) == 1, 'select'
-
-       users = db.select('select id, del_flag from user where id=:id', id=id2)
-       assert len(users) == 1, 'select'
-       users = db.query('select id, del_flag from user where id=:id', id=id2)
-       assert len(users) == 1, 'select'
-
-       db.execute('delete from user where id=? limit 1', id2)
-       assert db.get('select count(1) from user') == 3, 'execute delete'
-
-Transaction
-'''''''''''
-
-::
-
-   @db.with_transaction
-   def test_transaction():
-       db.insert('user', name='寮犱笁', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
-       db.insert('user', name='鏉庡洓', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
-
-
-   def test_transaction2():
-       with db.transaction():
-           db.insert('user', name='寮犱笁', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
-           db.insert('user', name='鏉庡洓', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
-
-Note: the functions return type
-'''''''''''''''''''''''''''''''
-
-::
-
-   get: Return only one object, like count
-   query_one: Return one row with dict
-   select_one: Return one row with tuple
-   find_by_id: Return one row with class instance object
-   query: Return list of dict
-   select: Return list of tuple
-   find: Return list of class instance object
-
-
+##### Install
+```
+pip install mysqlx
+```
+##### Usage Sample
+```
+CREATE TABLE `user` (
+  `id` bigint NOT NULL AUTO_INCREMENT,
+  `name` varchar(45) NOT NULL,
+  `age` int NOT NULL,
+  `birth_date` date DEFAULT NULL,
+  `sex` tinyint DEFAULT NULL,
+  PRIMARY KEY (`id`)
+) ENGINE=InnoDB AUTO_INCREMENT=62 DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_0900_ai_ci
+
+
+----------------------------------------------------------------------------------------
+
+from mysqlx import db
+
+db_conf = {
+    'host': '127.0.0.1',
+    'port': 3306, 
+    'user': 'root', 
+    'password': 'xxx', 
+    'database': 'test',
+    'pool_size': 5,
+    'show_sql': True
+}
+
+if __name__ == '__main__':
+    db.init_db(**db_conf)
+    
+    # Return effect rowcount
+    rowcount = db.insert('user', name='张三', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
+    assert rowcount == 1, '1 effect rowcount'
+    assert db.get('select count(1) from user') == 1, 'count is 1'
+
+    # Return primary key
+    id2 = db.save('user', name='李四', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
+    assert db.get('select count(1) from user') == 2, 'count is 2'
+
+    db.execute('update user set name=? where id=?', '王五', id2)
+    assert db.get('select name from user where id=?', id2) == '王五', 'execute'
+
+    db.execute('update user set name=:name where id=:id', name='赵六', id=id2)
+    assert db.select_one('select id, name from user where id=:id', id=id2)[0] == id2, 'execute'
+
+    db.execute('update user set name=:name where id=:id', name='赵六', id=id2)
+    assert db.query_one('select name from user where id=:id', id=id2)['name'] == '赵六', 'execute'
+
+    args = [
+        ('张三', 55, '1968=-10-08', 0, 1.0, 20.5, 854.56),
+        ('张三', 55, '1968=-10-08', 0, 1.0, 20.5, 854.56)
+    ]
+    db.batch_execute('insert into user(name, age, birth_date, sex, grade, point, money) values(?,?,?,?,?,?,?)', args)
+    users = db.select('select id, del_flag from user')
+    assert len(users) == 4, 'batch_execute'
+    users = db.query('select id, del_flag from user')
+    assert len(users) == 4, 'batch_execute'
+
+    users = db.select('select id, del_flag from user where id=?', id2)
+    assert len(users) == 1, 'select'
+    users = db.query('select id, del_flag from user where id=?', id2)
+    assert len(users) == 1, 'select'
+
+    users = db.select('select id, del_flag from user where id=:id', id=id2)
+    assert len(users) == 1, 'select'
+    users = db.query('select id, del_flag from user where id=:id', id=id2)
+    assert len(users) == 1, 'select'
+
+    db.execute('delete from user where id=? limit 1', id2)
+    assert db.get('select count(1) from user') == 3, 'execute delete'
+```
+##### Transaction
+```
+@db.with_transaction
+def test_transaction():
+    db.insert('user', name='张三', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
+    db.insert('user', name='李四', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
+
+
+def test_transaction2():
+    with db.transaction():
+        db.insert('user', name='张三', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
+        db.insert('user', name='李四', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
+```
+##### Note: the functions return type
+```
+get: Return only one object, like count
+query_one: Return one row with dict
+select_one: Return one row with tuple
+find_by_id: Return one row with class instance object
+query: Return list of dict
+select: Return list of tuple
+find: Return list of class instance object
+```
```

### Comparing `mysqlx-1.3.1/README.rst` & `mysqlx-1.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `mysqlx-1.3.1/setup.py` & `mysqlx-1.3.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,34 +2,34 @@
 from setuptools import setup, find_packages
 
 # INSTALL_PACKAGES = open(path.join(DIR, 'requirements.txt')).read().splitlines()
 def read(rel_path: str) -> str:
     here = os.path.abspath(os.path.dirname(__file__))
     # intentionally *not* adding an encoding option to open, See:
     #   https://github.com/pypa/virtualenv/issues/201#issuecomment-3145690
-    with open(os.path.join(here, rel_path)) as fp:
+    with open(os.path.join(here, rel_path), 'r', encoding='UTF-8') as fp:
         return fp.read()
 
-long_description = read("README.rst")
+long_description = read("README_en.rst")
 
 setup(
     name='mysqlx',
     packages=find_packages(),
     description="MySqlx is a simple python sql executor for MySQL like iBatis.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'Jinja2>=3.0.3',
         'mysql-connector-python>=8.0.20',
     ],
-    version='1.3.1',
+    version='1.3.2',
     url='https://gitee.com/summry/mysqlx',
     author='summry',
     author_email='xiazhongbiao@126.com',
-    keywords=['sql', 'MySQL', 'iBatis', 'MyBatis', 'python'],
+    keywords=['sql', 'MySQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
     },
     include_package_data=True,
     python_requires='>=3.6.0',
     zip_safe=False
```

### Comparing `mysqlx-1.3.1/test/dbx_test.py` & `mysqlx-1.3.2/test/dbx_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+import sys
+
 from config import DB_CONF
 from mysqlx import dbx
 import logging
 from test.db_test import create_truncate_table
 from test import user_mapper
 
 
 def full_test():
-    create_truncate_table()
+    create_truncate_table('user')
     #######################################################################################################
 
     rowcount = dbx.insert('user', name='张三', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
     assert rowcount == 1, 'insert'
     assert dbx.get(user_mapper.user_count) == 1, 'insert'
 
     id2 = dbx.save('user', name='李四', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
@@ -73,7 +75,8 @@
     for u in dbx.select_page('user.select_all', page_num=2, page_size=3):
         print(u)
 
     for u in dbx.query_page('user.select_all', page_num=2, page_size=3):
         print(u)
 
 
+
```

### Comparing `mysqlx-1.3.1/test/models.py` & `mysqlx-1.3.2/test/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,119 +1,129 @@
 from decimal import Decimal
-from mysqlx.orm import Model
 from datetime import date, datetime
+from mysqlx.orm import Model, PkStrategy
 
 
 class BaseModel(Model):
     __pk__ = 'id'
     __update_by__ = 'update_by'
     __update_time__ = 'update_time'
     __del_flag__ = 'del_flag'
+    __pk_strategy__ = PkStrategy.DB.value
 
-    def __init__(self, id: int = None, create_by: int = None, create_time: datetime = None, update_by: int = None, update_time: datetime = None, del_flag: int = None): 
-        self.id = id 
-        self.create_by = create_by 
-        self.create_time = create_time 
-        self.update_by = update_by 
-        self.update_time = update_time 
-        self.del_flag = del_flag 
+    def __init__(self, id: int = None, create_by: int = None, create_time: datetime = None, update_by: int = None, update_time: datetime = None,
+            del_flag: int = None):
+        self.id = id
+        self.create_by = create_by
+        self.create_time = create_time
+        self.update_by = update_by
+        self.update_time = update_time
+        self.del_flag = del_flag
 
 
-class Fund(BaseModel):
-    __table__ = 'fund'
+class User(BaseModel):
+    __table__ = 'user'
 
-    def __init__(self, id: int = None, code: str = None, name: str = None, alias: str = None, sort: int = None, last_profit: Decimal = None, net_worth_date: date = None, buy_rate: Decimal = None, day1: int = None, sell_rate1: Decimal = None, day2=None, sell_rate2: Decimal = None, day3=None, sell_rate3: Decimal = None, day4=None, sell_rate4: Decimal = None, sell_rate5: Decimal = None, hidden: int = None, statistics_date: date = None, show_trade_date: date = None, del_flag: int = None, ctl_flag: int = None):
-        super().__init__(id=id, del_flag=del_flag) 
-        self.code = code 
-        self.name = name 
-        self.alias = alias 
-        self.sort = sort 
-        self.last_profit = last_profit 
-        self.net_worth_date = net_worth_date 
-        self.buy_rate = buy_rate 
-        self.day1 = day1 
-        self.sell_rate1 = sell_rate1 
-        self.day2 = day2 
-        self.sell_rate2 = sell_rate2 
-        self.day3 = day3 
-        self.sell_rate3 = sell_rate3 
-        self.day4 = day4 
-        self.sell_rate4 = sell_rate4 
-        self.sell_rate5 = sell_rate5 
-        self.hidden = hidden 
-        self.statistics_date = statistics_date 
-        self.show_trade_date = show_trade_date 
-        self.ctl_flag = ctl_flag 
+    def __init__(self, id: int = None, name: str = None, age: int = None, birth_date: date = None, sex: int = None, grade: float = None,
+            point: float = None, money: Decimal = None, create_by: int = None, create_time: datetime = None, update_by: int = None,
+            update_time: datetime = None, del_flag: int = None):
+        super().__init__(id=id, create_by=create_by, create_time=create_time, update_by=update_by, update_time=update_time, del_flag=del_flag)
+        self.name = name
+        self.age = age
+        self.birth_date = birth_date
+        self.sex = sex
+        self.grade = grade
+        self.point = point
+        self.money = money
 
 
 class Person(BaseModel):
     __table__ = 'person'
 
     def __init__(self, id: int = None, name: str = None, age: int = None, sex: int = None):
-        super().__init__(id=id) 
-        self.name = name 
-        self.age = age 
-        self.sex = sex 
+        super().__init__(id=id)
+        self.name = name
+        self.age = age
+        self.sex = sex
 
 
 class Trade(BaseModel):
     __table__ = 'trade'
 
-    def __init__(self, id: int = None, fund_id: int = None, buy_date: date = None, amount: Decimal = None, buy_fee: Decimal = None, buy_worth: Decimal = None, fund_num: Decimal = None, status: int = None, sell_date: date = None, sell_amount: Decimal = None, sell_worth: Decimal = None, sell7: int = None, confirm_date: date = None):
-        super().__init__(id=id) 
-        self.fund_id = fund_id 
-        self.buy_date = buy_date 
-        self.amount = amount 
-        self.buy_fee = buy_fee 
-        self.buy_worth = buy_worth 
-        self.fund_num = fund_num 
-        self.status = status 
-        self.sell_date = sell_date 
-        self.sell_amount = sell_amount 
-        self.sell_worth = sell_worth 
-        self.sell7 = sell7 
-        self.confirm_date = confirm_date 
+    def __init__(self, id: int = None, fund_id: int = None, buy_date: date = None, amount: Decimal = None, buy_fee: Decimal = None,
+            buy_worth: Decimal = None, fund_num: Decimal = None, status: int = None, sell_date: date = None, sell_amount: Decimal = None,
+            sell_worth: Decimal = None, sell7: int = None, confirm_date: date = None):
+        super().__init__(id=id)
+        self.fund_id = fund_id
+        self.buy_date = buy_date
+        self.amount = amount
+        self.buy_fee = buy_fee
+        self.buy_worth = buy_worth
+        self.fund_num = fund_num
+        self.status = status
+        self.sell_date = sell_date
+        self.sell_amount = sell_amount
+        self.sell_worth = sell_worth
+        self.sell7 = sell7
+        self.confirm_date = confirm_date
 
 
 class FundDaliy(BaseModel):
     __table__ = 'fund_daliy'
 
-    def __init__(self, id: int = None, fund_id: int = None, net_worth_date: date = None, net_worth: Decimal = None, day_growth: Decimal = None, day_profit: Decimal = None, total_profit: Decimal = None, last_profit: Decimal = None, curr_profit: Decimal = None, amount: Decimal = None, buy_fee: Decimal = None, sell_fee: Decimal = None, act_amount: Decimal = None, act_day_profit: Decimal = None):
-        super().__init__(id=id) 
-        self.fund_id = fund_id 
-        self.net_worth_date = net_worth_date 
-        self.net_worth = net_worth 
-        self.day_growth = day_growth 
-        self.day_profit = day_profit 
-        self.total_profit = total_profit 
-        self.last_profit = last_profit 
-        self.curr_profit = curr_profit 
-        self.amount = amount 
-        self.buy_fee = buy_fee 
-        self.sell_fee = sell_fee 
-        self.act_amount = act_amount 
-        self.act_day_profit = act_day_profit 
+    def __init__(self, id: int = None, fund_id: int = None, net_worth_date: date = None, net_worth: Decimal = None, day_growth: Decimal = None,
+            day_profit: Decimal = None, total_profit: Decimal = None, last_profit: Decimal = None, curr_profit: Decimal = None,
+            amount: Decimal = None, buy_fee: Decimal = None, sell_fee: Decimal = None, act_amount: Decimal = None, act_day_profit: Decimal = None):
+        super().__init__(id=id)
+        self.fund_id = fund_id
+        self.net_worth_date = net_worth_date
+        self.net_worth = net_worth
+        self.day_growth = day_growth
+        self.day_profit = day_profit
+        self.total_profit = total_profit
+        self.last_profit = last_profit
+        self.curr_profit = curr_profit
+        self.amount = amount
+        self.buy_fee = buy_fee
+        self.sell_fee = sell_fee
+        self.act_amount = act_amount
+        self.act_day_profit = act_day_profit
 
 
-class Bonus(BaseModel):
-    __table__ = 'bonus'
-
-    def __init__(self, id: int = None, fund_id: int = None, dividend_date: date = None, amount: Decimal = None):
-        super().__init__(id=id) 
-        self.fund_id = fund_id 
-        self.dividend_date = dividend_date 
-        self.amount = amount 
+class Fund(BaseModel):
+    __table__ = 'fund'
 
+    def __init__(self, id: int = None, code: str = None, name: str = None, alias: str = None, sort: int = None, last_profit: Decimal = None,
+            net_worth_date: date = None, buy_rate: Decimal = None, day1: int = None, sell_rate1: Decimal = None, day2=None,
+            sell_rate2: Decimal = None, day3=None, sell_rate3: Decimal = None, day4=None, sell_rate4: Decimal = None, sell_rate5: Decimal = None,
+            hidden: int = None, statistics_date: date = None, show_trade_date: date = None, del_flag: int = None, ctl_flag: int = None):
+        super().__init__(id=id, del_flag=del_flag)
+        self.code = code
+        self.name = name
+        self.alias = alias
+        self.sort = sort
+        self.last_profit = last_profit
+        self.net_worth_date = net_worth_date
+        self.buy_rate = buy_rate
+        self.day1 = day1
+        self.sell_rate1 = sell_rate1
+        self.day2 = day2
+        self.sell_rate2 = sell_rate2
+        self.day3 = day3
+        self.sell_rate3 = sell_rate3
+        self.day4 = day4
+        self.sell_rate4 = sell_rate4
+        self.sell_rate5 = sell_rate5
+        self.hidden = hidden
+        self.statistics_date = statistics_date
+        self.show_trade_date = show_trade_date
+        self.ctl_flag = ctl_flag
 
-class User(BaseModel):
-    __table__ = 'user'
 
-    def __init__(self, id: int = None, name: str = None, age: int = None, birth_date: date = None, sex: int = None, grade: float = None, point: float = None, money: Decimal = None, create_by: int = None, create_time: datetime = None, update_by: int = None, update_time: datetime = None, del_flag: int = None):
-        super().__init__(id=id, create_by=create_by, create_time=create_time, update_by=update_by, update_time=update_time, del_flag=del_flag) 
-        self.name = name 
-        self.age = age 
-        self.birth_date = birth_date 
-        self.sex = sex 
-        self.grade = grade 
-        self.point = point 
-        self.money = money 
+class Bonus(BaseModel):
+    __table__ = 'bonus'
 
+    def __init__(self, id: int = None, fund_id: int = None, dividend_date: date = None, amount: Decimal = None):
+        super().__init__(id=id)
+        self.fund_id = fund_id
+        self.dividend_date = dividend_date
+        self.amount = amount
```

### Comparing `mysqlx-1.3.1/test/unit_test.py` & `mysqlx-1.3.2/test/unit_test.py`

 * *Files identical despite different names*

