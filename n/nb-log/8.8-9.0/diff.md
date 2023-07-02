# Comparing `tmp/nb_log-8.8.tar.gz` & `tmp/nb_log-9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nb_log-8.8.tar", last modified: Sat Jun 24 15:59:50 2023, max compression
+gzip compressed data, was "nb_log-9.0.tar", last modified: Sun Jul  2 08:25:01 2023, max compression
```

## Comparing `nb_log-8.8.tar` & `nb_log-9.0.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 15:59:50.323320 nb_log-8.8/
--rw-rw-rw-   0        0        0    27859 2023-06-24 15:59:50.320319 nb_log-8.8/PKG-INFO
--rw-rw-rw-   0        0        0    26926 2023-05-13 11:59:47.000000 nb_log-8.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 15:59:50.299320 nb_log-8.8/nb_log/
--rw-rw-rw-   0        0        0     2369 2023-06-24 02:46:57.000000 nb_log-8.8/nb_log/__init__.py
--rw-rw-rw-   0        0        0    50691 2023-06-24 02:46:57.000000 nb_log-8.8/nb_log/handlers.py
--rw-rw-rw-   0        0        0    49868 2022-09-12 12:13:59.000000 nb_log-8.8/nb_log/handlers0000.py
--rw-rw-rw-   0        0        0      247 2023-06-24 02:46:57.000000 nb_log-8.8/nb_log/helper.py
--rw-rw-rw-   0        0        0    30621 2023-06-24 02:46:57.000000 nb_log-8.8/nb_log/log_manager.py
--rw-rw-rw-   0        0        0     7782 2023-06-24 02:46:57.000000 nb_log-8.8/nb_log/monkey_print.py
--rw-rw-rw-   0        0        0     9470 2023-06-24 02:46:57.000000 nb_log-8.8/nb_log/nb_log_config_default.py
--rw-rw-rw-   0        0        0     7710 2023-06-24 02:46:57.000000 nb_log-8.8/nb_log/set_nb_log_config.py
-drwxrwxrwx   0        0        0        0 2023-06-24 15:59:50.316305 nb_log-8.8/nb_log.egg-info/
--rw-rw-rw-   0        0        0    27859 2023-06-24 15:59:50.000000 nb_log-8.8/nb_log.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      350 2023-06-24 15:59:50.000000 nb_log-8.8/nb_log.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 15:59:50.000000 nb_log-8.8/nb_log.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      187 2023-06-24 15:59:50.000000 nb_log-8.8/nb_log.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-24 15:59:50.000000 nb_log-8.8/nb_log.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 15:59:50.323320 nb_log-8.8/setup.cfg
--rw-rw-rw-   0        0        0     2345 2023-06-24 15:59:45.000000 nb_log-8.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 08:25:01.384092 nb_log-9.0/
+-rw-rw-rw-   0        0        0    27859 2023-07-02 08:25:01.382082 nb_log-9.0/PKG-INFO
+-rw-rw-rw-   0        0        0    26926 2023-05-13 11:59:47.000000 nb_log-9.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-02 08:25:01.360077 nb_log-9.0/nb_log/
+-rw-rw-rw-   0        0        0     3192 2023-07-02 07:24:38.000000 nb_log-9.0/nb_log/__init__.py
+-rw-rw-rw-   0        0        0     2068 2023-07-01 05:31:11.000000 nb_log-9.0/nb_log/file_write.py
+-rw-rw-rw-   0        0        0    50691 2023-06-24 02:46:57.000000 nb_log-9.0/nb_log/handlers.py
+-rw-rw-rw-   0        0        0    49868 2022-09-12 12:13:59.000000 nb_log-9.0/nb_log/handlers0000.py
+-rw-rw-rw-   0        0        0    30839 2023-06-30 14:23:45.000000 nb_log-9.0/nb_log/log_manager.py
+-rw-rw-rw-   0        0        0     6409 2023-07-02 07:15:56.000000 nb_log-9.0/nb_log/monkey_print.py
+-rw-rw-rw-   0        0        0      853 2023-07-01 05:26:36.000000 nb_log-9.0/nb_log/monkey_std_filter_words.py
+-rw-rw-rw-   0        0        0      819 2023-07-02 07:15:56.000000 nb_log-9.0/nb_log/monkey_sys_std.py
+-rw-rw-rw-   0        0        0    10520 2023-07-02 08:12:50.000000 nb_log-9.0/nb_log/nb_log_config_default.py
+-rw-rw-rw-   0        0        0     4328 2023-06-30 14:23:45.000000 nb_log-9.0/nb_log/nb_logger.py
+-rw-rw-rw-   0        0        0     7710 2023-06-24 02:46:57.000000 nb_log-9.0/nb_log/set_nb_log_config.py
+drwxrwxrwx   0        0        0        0 2023-07-02 08:25:01.378081 nb_log-9.0/nb_log.egg-info/
+-rw-rw-rw-   0        0        0    27859 2023-07-02 08:25:01.000000 nb_log-9.0/nb_log.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      433 2023-07-02 08:25:01.000000 nb_log-9.0/nb_log.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 08:25:01.000000 nb_log-9.0/nb_log.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      187 2023-07-02 08:25:01.000000 nb_log-9.0/nb_log.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-02 08:25:01.000000 nb_log-9.0/nb_log.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-02 08:25:01.384092 nb_log-9.0/setup.cfg
+-rw-rw-rw-   0        0        0     2345 2023-07-02 08:17:40.000000 nb_log-9.0/setup.py
```

### Comparing `nb_log-8.8/PKG-INFO` & `nb_log-9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb_log
-Version: 8.8
+Version: 9.0
 Summary: very sharp color display,monkey patch bulitin print  and high-performance multiprocess safe roating file handler,other handlers includeing dintalk ,email,kafka,elastic and so on 
 Home-page: https://github.com/ydf0509/nb_log
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
```

### Comparing `nb_log-8.8/README.md` & `nb_log-9.0/README.md`

 * *Files identical despite different names*

### Comparing `nb_log-8.8/nb_log/handlers.py` & `nb_log-9.0/nb_log/handlers.py`

 * *Files identical despite different names*

### Comparing `nb_log-8.8/nb_log/handlers0000.py` & `nb_log-9.0/nb_log/handlers0000.py`

 * *Files identical despite different names*

### Comparing `nb_log-8.8/nb_log/log_manager.py` & `nb_log-9.0/nb_log/log_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 """
 import logging
 import multiprocessing
 import typing
 from functools import lru_cache
 from logging import FileHandler, _checkLevel  # noqa
-from nb_log import nb_log_config_default  # noqa
+from nb_log import nb_log_config_default, nb_logger  # noqa
 from nb_log.handlers import *
 import deprecated
 
 
 # noinspection DuplicatedCode
 def revision_call_handlers(self, record):  # 对logging标准模块打猴子补丁。主要是使父命名空间的handler不重复记录当前命名空间日志已有种类的handler。
     """
@@ -199,32 +199,40 @@
 
 
 def check_log_level(log_level: int):
     if log_level not in LOG_LEVEL_LIST:
         raise ValueError(f'你设置的日志级别不正确,你设置的级别是 {log_level} ，日志级别必须是 {LOG_LEVEL_LIST} 其中之一')
 
 
+
+
 # noinspection PyMissingOrEmptyDocstring,PyPep8
 class LogManager(object):
     """
     一个日志管理类，用于创建logger和添加handler，支持将日志打印到控制台打印和写入日志文件和mongodb和邮件。
     """
     logger_name_list = []
     logger_list = []
     preset_name__level_map = dict()
 
+    # logger_cls = logging.Logger
+    logger_cls = nb_logger.NbLogger
+
     def __init__(self, logger_name: typing.Union[str, None] = 'nb_log_default_namespace'):
         """
         :param logger_name: 日志名称，当为None时候创建root命名空间的日志，一般情况下千万不要传None，除非你确定需要这么做和是在做什么.这个命名空间是双刃剑
         """
         if logger_name in (None, '',) and multiprocessing.process.current_process().name == 'MainProcess':
             very_nb_print('logger_name 设置为None和空字符串都是一个意义，在操作根日志命名空间，任何其他日志的行为将会发生变化，'
                           '一定要弄清楚原生logging包的日志name的意思。这个命名空间是双刃剑')
         self._logger_name = logger_name
-        self.logger = logging.getLogger(logger_name)
+        if self.logger_cls == nb_logger.NbLogger:
+            self.logger = nb_logger.NbLogger(logger_name)
+        else:
+            self.logger = logging.getLogger(logger_name)
 
     def preset_log_level(self, log_level_int=20):
         """
         提前设置锁定日志级别，当之后再设置该命名空间日志的级别的时候，按照提前预设的级别，无视之后设定的级别。
         主要是针对动态初始化的日志，在生成日志之后再去设置日志级别不方便。
         :param log_level_int:logging.DEBUG LOGGING.INFO 等
         :return:
```

### Comparing `nb_log-8.8/nb_log/monkey_print.py` & `nb_log-9.0/nb_log/monkey_print.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,92 +2,89 @@
 # @Author  : ydf
 # @Time    : 2022/5/9 19:02
 """
 不直接给print打补丁，自己重新赋值。
 
 """
 import multiprocessing
+import os
 import sys
 import time
 import traceback
 from nb_log import nb_log_config_default
-from nb_log.helper import _need_filter_print
+from nb_log.file_write import PrintFileWritter
 
 print_raw = print
-sys_stdout_write_raw = sys.stdout.write
-sys_stderr_write_raw = sys.stderr.write
-
 WORD_COLOR = 37
 
 
-def _sys_stdout_write_monkey(msg: str):
-    if _need_filter_print(msg):
-        return
-    else:
-        sys_stdout_write_raw(msg)
-
-def _sys_stderr_write_monkey(msg: str):
-    if _need_filter_print(msg):
-        return
-    else:
-        sys_stderr_write_raw(msg)
-
-
-sys.stdout.write = _sys_stdout_write_monkey  # 对 sys.stdout.write 打了猴子补丁。使得可以过滤包含指定字符串的消息。
-sys.stderr.write = _sys_stderr_write_monkey
-
-
 def stdout_write(msg: str):
     sys.stdout.write(msg)
     sys.stdout.flush()
 
 
 def stderr_write(msg: str):
     sys.stderr.write(msg)
     sys.stderr.flush()
 
 
-# noinspection PyProtectedMember,PyUnusedLocal,PyIncorrectDocstring,DuplicatedCode
-def nb_print(*args, sep=' ', end='\n', file=None, flush=True):
-    """
-    超流弊的print补丁
-    :param x:
-    :return:
-    """
+print_wrtie_file_name = os.environ.get('PRINT_WRTIE_FILE_NAME', None) or nb_log_config_default.PRINT_WRTIE_FILE_NAME
 
+print_file_writter = PrintFileWritter(print_wrtie_file_name)
+
+
+def _print_with_file_line(*args, sep=' ', end='\n', file=None, flush=True, sys_getframe_n=2):
     args = (str(arg) for arg in args)  # REMIND 防止是数字不能被join
+    args_str = sep.join(args) + end
+    # stdout_write(f'56:{file}')
     if file == sys.stderr:
-        stderr_write(sep.join(args))  # 如 threading 模块第926行，打印线程错误，希望保持原始的红色错误方式，不希望转成蓝色。
+        stderr_write(args_str)  # 如 threading 模块第926行，打印线程错误，希望保持原始的红色错误方式，不希望转成蓝色。
+        print_file_writter.write_2_file(args_str)
     elif file in [sys.stdout, None]:
         # 获取被调用函数在被调用时所处代码行数
-        line = sys._getframe().f_back.f_lineno
-        # 获取被调用函数所在模块文件名
-        file_name = sys._getframe(1).f_code.co_filename
+        fra = sys._getframe(sys_getframe_n)
+        line = fra.f_lineno
+        file_name = fra.f_code.co_filename
+        fun = fra.f_code.co_name
         # sys.stdout.write(f'"{__file__}:{sys._getframe().f_lineno}"    {x}\n')
         if nb_log_config_default.DEFAULUT_USE_COLOR_HANDLER:
             if nb_log_config_default.DISPLAY_BACKGROUD_COLOR_IN_CONSOLE:
                 stdout_write(
-                    f'\033[0;34m{time.strftime("%H:%M:%S")}  "{file_name}:{line}"   \033[0;{WORD_COLOR};44m{sep.join(args)}\033[0m{end} \033[0m')  # 36  93 96 94
+                    f'\033[0;34m{time.strftime("%H:%M:%S")}  "{file_name}:{line}" {fun}  \033[0;{WORD_COLOR};44m{args_str}\033[0m \033[0m')  # 36  93 96 94
             else:
                 stdout_write(
-                    f'\033[0;{WORD_COLOR};34m{time.strftime("%H:%M:%S")}  "{file_name}:{line}"   {sep.join(args)} {end} \033[0m')  # 36  93 96 94
+                    f'\033[0;{WORD_COLOR};34m{time.strftime("%H:%M:%S")}  "{file_name}:{line}" {fun}  {args_str}  \033[0m')  # 36  93 96 94
             # sys.stdout.write(f'\033[0;30;44m"{file_name}:{line}"  {time.strftime("%H:%M:%S")}  {"".join(args)}\033[0m\n')
         else:
             stdout_write(
-                f'{time.strftime("%H:%M:%S")}  "{file_name}:{line}"   {sep.join(args)} {end}')  # 36  93 96 94
+                f'{time.strftime("%H:%M:%S")}  "{file_name}:{line}"  {fun} {args_str} ')
+        print_file_writter.write_2_file(f'{time.strftime("%H:%M:%S")}  "{file_name}:{line}" {fun} {args_str} ')  # 36  93 96 94
     else:  # 例如traceback模块的print_exception函数 file的入参是   <_io.StringIO object at 0x00000264F2F065E8>，必须把内容重定向到这个对象里面，否则exception日志记录不了错误堆栈。
-        print_raw(*args, sep=sep, end=end, file=file)
+        print_raw(args_str, sep=sep, end=end, file=file)
+        print_file_writter.write_2_file(args_str)
+
+
+# noinspection PyProtectedMember,PyUnusedLocal,PyIncorrectDocstring,DuplicatedCode
+def nb_print(*args, sep=' ', end='\n', file=None, flush=True):
+    """
+    超流弊的print补丁
+    :param x:
+    :return:
+    """
+    _print_with_file_line(*args, sep=sep, end=end, file=file, flush=flush, sys_getframe_n=2)
 
 
 # noinspection PyPep8,PyUnusedLocal
 def print_exception(etype, value, tb, limit=None, file=None, chain=True):
     """
     避免每行有两个可跳转的，导致第二个可跳转的不被ide识别。
     主要是针对print_exception，logging.exception里面会调用这个函数。
 
+    # traceback.print_exception = print_exception  # file类型为 <_io.StringIO object at 0x00000264F2F065E8> 单独判断sys.stderr sys.stdout 以外的情况了，解决了，不需要用到p rint_exception。
+
     :param etype:
     :param value:
     :param tb:
     :param limit:
     :param file:
     :param chain:
     :return:
@@ -163,36 +160,15 @@
     return multiprocessing.process.current_process().name == 'MainProcess'
 
 
 # noinspection DuplicatedCode
 def only_print_on_main_process(*args, sep=' ', end='\n', file=None, flush=True):
     # 获取被调用函数在被调用时所处代码行数
     if is_main_process():
-        args = (str(arg) for arg in args)  # REMIND 防止是数字不能被join
-        if file == sys.stderr:
-            stderr_write(sep.join(args))  # 如 threading 模块第926行，打印线程错误，希望保持原始的红色错误方式，不希望转成蓝色。
-        elif file in [sys.stdout, None]:
-            # 获取被调用函数在被调用时所处代码行数
-            line = sys._getframe().f_back.f_lineno
-            # 获取被调用函数所在模块文件名
-            file_name = sys._getframe(1).f_code.co_filename
-            # sys.stdout.write(f'"{__file__}:{sys._getframe().f_lineno}"    {x}\n')
-            if nb_log_config_default.DEFAULUT_USE_COLOR_HANDLER:
-                if nb_log_config_default.DISPLAY_BACKGROUD_COLOR_IN_CONSOLE:
-                    stdout_write(
-                        f'\033[0;34m{time.strftime("%H:%M:%S")}  "{file_name}:{line}"   \033[0;{WORD_COLOR};44m{sep.join(args)}\033[0m{end} \033[0m')  # 36  93 96 94
-                else:
-                    stdout_write(
-                        f'\033[0;{WORD_COLOR};34m{time.strftime("%H:%M:%S")}  "{file_name}:{line}"   {sep.join(args)} {end} \033[0m')  # 36  93 96 94
-                # sys.stdout.write(f'\033[0;30;44m"{file_name}:{line}"  {time.strftime("%H:%M:%S")}  {"".join(args)}\033[0m\n')
-            else:
-                stdout_write(
-                    f'{time.strftime("%H:%M:%S")}  "{file_name}:{line}"   {sep.join(args)} {end}')  # 36  93 96 94
-        else:  # 例如traceback模块的print_exception函数 file的入参是   <_io.StringIO object at 0x00000264F2F065E8>，必须把内容重定向到这个对象里面，否则exception日志记录不了错误堆栈。
-            print_raw(*args, sep=sep, end=end, file=file)
+        _print_with_file_line(*args, sep=sep, end=end, file=file, flush=flush, sys_getframe_n=2)
 
 
 if __name__ == '__main__':
     print('before patch')
     patch_print()
     print(0)
     nb_print(123, 'abc')
```

### Comparing `nb_log-8.8/nb_log/nb_log_config_default.py` & `nb_log-9.0/nb_log/nb_log_config_default.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 如果反对日志有各种彩色，可以设置 DEFAULUT_USE_COLOR_HANDLER = False
 如果反对日志有块状背景彩色，可以设置 DISPLAY_BACKGROUD_COLOR_IN_CONSOLE = False
 如果想屏蔽nb_log包对怎么设置pycahrm的颜色的提示，可以设置 WARNING_PYCHARM_COLOR_SETINGS = False
 如果想改变日志模板，可以设置 FORMATTER_KIND 参数，只带了7种模板，可以自定义添加喜欢的模板
 LOG_PATH 配置文件日志的保存路径的文件夹。
 """
-
+import sys
 # noinspection PyUnresolvedReferences
 import logging
 import os
 # noinspection PyUnresolvedReferences
 from pathlib import Path  # noqa
 import socket
 from pythonjsonlogger.jsonlogger import JsonFormatter
@@ -62,14 +62,22 @@
 ELASTIC_PORT = 9200
 
 KAFKA_BOOTSTRAP_SERVERS = ['192.168.199.202:9092']
 ALWAYS_ADD_KAFKA_HANDLER_IN_TEST_ENVIRONENT = False
 
 MONGO_URL = 'mongodb://myUserAdmin:mimamiama@127.0.0.1:27016/admin'
 
+# 项目中的print是否自动写入到文件中。值为None则不重定向标准输出到文件中。 自动每天一个文件， 2023-06-30.my_proj.out,生成的文件位置在定义的LOG_PATH
+# 如果你设置了环境变量，export PRINT_WRTIE_FILE_NAME="my_proj.print" (linux临时环境变量语法，windows语法自己百度这里不举例),那就优先使用环境变量中设置的文件名字，而不是nb_log_config.py中设置的名字
+PRINT_WRTIE_FILE_NAME = Path(sys.path[1]).name + '.print'
+
+# 项目中的所有标准输出（不仅包括print，还包括了streamHandler日志）都写入到这个文件。自动每天一个文件， 2023-06-30.my_proj.std,生成的文件位置在定义的LOG_PATH
+# 如果你设置了环境变量，export SYS_STD_FILE_NAME="my_proj.std"  (linux临时环境变量语法，windows语法自己百度这里不举例),那就优先使用环境变量中设置的文件名字，，而不是nb_log_config.py中设置的名字
+SYS_STD_FILE_NAME = Path(sys.path[1]).name + '.std'
+
 DEFAULUT_USE_COLOR_HANDLER = True  # 是否默认使用有彩的日志。
 DISPLAY_BACKGROUD_COLOR_IN_CONSOLE = True  # 在控制台是否显示彩色块状的日志。为False则不使用大块的背景颜色。
 AUTO_PATCH_PRINT = True  # 是否自动打print的猴子补丁，如果打了猴子补丁，print自动变色和可点击跳转。
 SHOW_PYCHARM_COLOR_SETINGS = True  # 有的人很反感启动代码时候提示教你怎么优化pycahrm控制台颜色，可以把这里设置为False
 
 DEFAULT_ADD_MULTIPROCESSING_SAFE_ROATING_FILE_HANDLER = False  # 是否默认同时将日志记录到记log文件记事本中，就是用户不指定 log_filename的值，会自动写入日志命名空间.log文件中。
 LOG_FILE_SIZE = 100  # 单位是M,每个文件的切片大小，超过多少后就自动切割
@@ -95,15 +103,15 @@
 
 LOG_LEVEL_FILTER = logging.DEBUG  # 默认日志级别，低于此级别的日志不记录了。例如设置为INFO，那么logger.debug的不会记录，只会记录logger.info以上级别的。
 # 强烈不建议调高这里的级别为INFO，日志是有命名空间的，单独提高打印啰嗦的日志命名空间的日志级别就可以了，不要全局提高日志级别。
 # https://nb-log-doc.readthedocs.io/zh_CN/latest/articles/c9.html#id2  文档9.5里面讲了几百次 python logging的命名空间的作用了，有些人到现在还不知道日志的name作用。
 
 # 屏蔽的字符串显示，用 if in {打印信息} 来判断实现的,如果打印的消息中包括 FILTER_WORDS_PRINT 数组中的任何一个字符串，那么消息就不执行打印。
 # 这个配置对 print 和 logger的控制台输出都生效。这个可以过滤某些啰嗦的print信息，也可以过滤同级别日志中的某些烦人的日志。可以用来过滤三方包中某些控制台打印。数组不要配置过多，否则有一丝丝影响性能会。
-FILTER_WORDS_PRINT = []  # 例如， 你希望消息中包括阿弥陀佛 或者 包括善哉善哉 就不打印，那么可以把  FILTER_WORDS_PRINT = ['阿弥陀佛','善哉善哉']
+FILTER_WORDS_PRINT = []  # 例如， 你希望消息中包括阿弥陀佛 或者 包括善哉善哉 就不打印，那么可以设置  FILTER_WORDS_PRINT = ['阿弥陀佛','善哉善哉']
 
 RUN_ENV = 'test'
 
 FORMATTER_DICT = {
     1: logging.Formatter(
         '日志时间【%(asctime)s】 - 日志名称【%(name)s】 - 文件【%(filename)s】 - 第【%(lineno)d】行 - 日志等级【%(levelname)s】 - 日志信息【%(message)s】',
         "%Y-%m-%d %H:%M:%S"),
```

### Comparing `nb_log-8.8/nb_log/set_nb_log_config.py` & `nb_log-9.0/nb_log/set_nb_log_config.py`

 * *Files identical despite different names*

### Comparing `nb_log-8.8/nb_log.egg-info/PKG-INFO` & `nb_log-9.0/nb_log.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb-log
-Version: 8.8
+Version: 9.0
 Summary: very sharp color display,monkey patch bulitin print  and high-performance multiprocess safe roating file handler,other handlers includeing dintalk ,email,kafka,elastic and so on 
 Home-page: https://github.com/ydf0509/nb_log
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
```

### Comparing `nb_log-8.8/setup.py` & `nb_log-9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 ]
 
 if os.name == 'nt':
     install_requires.append('pywin32')
 
 setup(
     name='nb_log',  #
-    version="8.8",
+    version="9.0",
     description=(
         'very sharp color display,monkey patch bulitin print  and high-performance multiprocess safe roating file handler,other handlers includeing dintalk ,email,kafka,elastic and so on '
     ),
     keywords=["logging", "logger", "multiprocess file handler", "color handler"],
     # long_description=open('README.md', 'r',encoding='utf8').read(),
     long_description_content_type="text/markdown",
     long_description=open(filepath, 'r', encoding='utf8').read(),
@@ -62,14 +62,14 @@
 """
 打包上传
 python setup.py sdist upload -r pypi
 
 
 
 python setup.py sdist & twine upload dist/nb_log-6.0.tar.gz
-python setup.py sdist & python -m  twine upload dist/nb_log-8.8.tar.gz
+python setup.py sdist & python -m  twine upload dist/nb_log-9.0.tar.gz
 
 twine upload dist/*
 
 
 python -m pip install nb_log --upgrade -i https://pypi.org/simple   # 及时的方式，不用等待 阿里云 豆瓣 同步
 """
```

