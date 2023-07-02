# Comparing `tmp/python-dict-display-filter-0.9.7.tar.gz` & `tmp/python-dict-display-filter-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-dict-display-filter-0.9.7.tar", last modified: Sun Feb 27 13:44:10 2022, max compression
+gzip compressed data, was "python-dict-display-filter-0.9.8.tar", last modified: Sun Jul  2 14:31:04 2023, max compression
```

## Comparing `python-dict-display-filter-0.9.7.tar` & `python-dict-display-filter-0.9.8.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2022-02-27 13:44:10.067005 python-dict-display-filter-0.9.7/
--rw-rw-r--   0 tengel    (1000) tengel    (1000)    35149 2022-02-01 18:33:10.000000 python-dict-display-filter-0.9.7/LICENSE
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     4177 2022-02-27 13:44:10.067005 python-dict-display-filter-0.9.7/PKG-INFO
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     3723 2022-02-25 14:32:10.000000 python-dict-display-filter-0.9.7/README.md
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2022-02-27 13:44:10.067005 python-dict-display-filter-0.9.7/pydictdisplayfilter/
--rw-rw-r--   0 tengel    (1000) tengel    (1000)      807 2022-02-14 23:33:52.000000 python-dict-display-filter-0.9.7/pydictdisplayfilter/__init__.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     5822 2022-02-27 13:41:38.000000 python-dict-display-filter-0.9.7/pydictdisplayfilter/display_filters.py
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2022-02-27 13:44:10.067005 python-dict-display-filter-0.9.7/pydictdisplayfilter/evaluators/
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     8100 2022-02-27 13:41:38.000000 python-dict-display-filter-0.9.7/pydictdisplayfilter/evaluators/__init__.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)    17999 2022-02-27 13:41:38.000000 python-dict-display-filter-0.9.7/pydictdisplayfilter/evaluators/common.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1414 2022-02-14 23:33:52.000000 python-dict-display-filter-0.9.7/pydictdisplayfilter/exceptions.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1341 2022-02-14 23:33:52.000000 python-dict-display-filter-0.9.7/pydictdisplayfilter/factories.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     6911 2022-02-14 23:43:51.000000 python-dict-display-filter-0.9.7/pydictdisplayfilter/helpers.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1524 2022-02-14 23:33:52.000000 python-dict-display-filter-0.9.7/pydictdisplayfilter/models.py
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2022-02-27 13:44:10.067005 python-dict-display-filter-0.9.7/pydictdisplayfilter/parsers/
--rw-rw-r--   0 tengel    (1000) tengel    (1000)      797 2022-02-14 23:33:52.000000 python-dict-display-filter-0.9.7/pydictdisplayfilter/parsers/__init__.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     4311 2022-02-14 23:33:52.000000 python-dict-display-filter-0.9.7/pydictdisplayfilter/parsers/common.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     7361 2022-02-14 23:33:52.000000 python-dict-display-filter-0.9.7/pydictdisplayfilter/parsers/display_filter.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     6142 2022-02-14 23:33:52.000000 python-dict-display-filter-0.9.7/pydictdisplayfilter/slicers.py
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2022-02-27 13:44:10.067005 python-dict-display-filter-0.9.7/python_dict_display_filter.egg-info/
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     4177 2022-02-27 13:44:09.000000 python-dict-display-filter-0.9.7/python_dict_display_filter.egg-info/PKG-INFO
--rw-rw-r--   0 tengel    (1000) tengel    (1000)      823 2022-02-27 13:44:09.000000 python-dict-display-filter-0.9.7/python_dict_display_filter.egg-info/SOURCES.txt
--rw-rw-r--   0 tengel    (1000) tengel    (1000)        1 2022-02-27 13:44:09.000000 python-dict-display-filter-0.9.7/python_dict_display_filter.egg-info/dependency_links.txt
--rw-rw-r--   0 tengel    (1000) tengel    (1000)       77 2022-02-27 13:44:09.000000 python-dict-display-filter-0.9.7/python_dict_display_filter.egg-info/requires.txt
--rw-rw-r--   0 tengel    (1000) tengel    (1000)       26 2022-02-27 13:44:09.000000 python-dict-display-filter-0.9.7/python_dict_display_filter.egg-info/top_level.txt
--rw-rw-r--   0 tengel    (1000) tengel    (1000)       38 2022-02-27 13:44:10.067005 python-dict-display-filter-0.9.7/setup.cfg
--rw-rw-r--   0 tengel    (1000) tengel    (1000)      974 2022-02-27 13:42:06.000000 python-dict-display-filter-0.9.7/setup.py
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2022-02-27 13:44:10.067005 python-dict-display-filter-0.9.7/tests/
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1014 2022-02-14 23:33:52.000000 python-dict-display-filter-0.9.7/tests/__init__.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)    10562 2022-02-14 23:33:52.000000 python-dict-display-filter-0.9.7/tests/test_dict_display_filter.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     6105 2022-02-14 23:33:52.000000 python-dict-display-filter-0.9.7/tests/test_display_filter_parser.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     4050 2022-02-14 23:33:52.000000 python-dict-display-filter-0.9.7/tests/test_slicers.py
+drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-02 14:31:04.424356 python-dict-display-filter-0.9.8/
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)    35149 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.8/LICENSE
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     4177 2023-07-02 14:31:04.424356 python-dict-display-filter-0.9.8/PKG-INFO
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     3723 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.8/README.md
+drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-02 14:31:04.424356 python-dict-display-filter-0.9.8/pydictdisplayfilter/
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)      807 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.8/pydictdisplayfilter/__init__.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)    10804 2023-07-02 14:04:11.000000 python-dict-display-filter-0.9.8/pydictdisplayfilter/display_filters.py
+drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-02 14:31:04.424356 python-dict-display-filter-0.9.8/pydictdisplayfilter/evaluators/
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     8100 2023-06-27 14:26:40.000000 python-dict-display-filter-0.9.8/pydictdisplayfilter/evaluators/__init__.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)    18018 2023-06-30 21:51:51.000000 python-dict-display-filter-0.9.8/pydictdisplayfilter/evaluators/common.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     1414 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.8/pydictdisplayfilter/exceptions.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     1341 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.8/pydictdisplayfilter/factories.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     8057 2023-07-02 13:18:01.000000 python-dict-display-filter-0.9.8/pydictdisplayfilter/helpers.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     1524 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.8/pydictdisplayfilter/models.py
+drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-02 14:31:04.424356 python-dict-display-filter-0.9.8/pydictdisplayfilter/parsers/
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)      797 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.8/pydictdisplayfilter/parsers/__init__.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     4311 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.8/pydictdisplayfilter/parsers/common.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     7361 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.8/pydictdisplayfilter/parsers/display_filter.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     6142 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.8/pydictdisplayfilter/slicers.py
+drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-02 14:31:04.424356 python-dict-display-filter-0.9.8/python_dict_display_filter.egg-info/
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     4177 2023-07-02 14:31:04.000000 python-dict-display-filter-0.9.8/python_dict_display_filter.egg-info/PKG-INFO
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)      856 2023-07-02 14:31:04.000000 python-dict-display-filter-0.9.8/python_dict_display_filter.egg-info/SOURCES.txt
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)        1 2023-07-02 14:31:04.000000 python-dict-display-filter-0.9.8/python_dict_display_filter.egg-info/dependency_links.txt
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)       93 2023-07-02 14:31:04.000000 python-dict-display-filter-0.9.8/python_dict_display_filter.egg-info/requires.txt
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)       26 2023-07-02 14:31:04.000000 python-dict-display-filter-0.9.8/python_dict_display_filter.egg-info/top_level.txt
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)       38 2023-07-02 14:31:04.424356 python-dict-display-filter-0.9.8/setup.cfg
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     1001 2023-06-30 10:16:10.000000 python-dict-display-filter-0.9.8/setup.py
+drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2023-07-02 14:31:04.424356 python-dict-display-filter-0.9.8/tests/
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     1014 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.8/tests/__init__.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)    10562 2023-06-30 09:43:27.000000 python-dict-display-filter-0.9.8/tests/test_dict_display_filter.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     6105 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.8/tests/test_display_filter_parser.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     4050 2023-06-27 11:06:36.000000 python-dict-display-filter-0.9.8/tests/test_slicers.py
+-rw-rw-r--   0 tengel    (1000) tengel    (1000)     7550 2023-07-02 14:04:11.000000 python-dict-display-filter-0.9.8/tests/test_sql_display_filter.py
```

### Comparing `python-dict-display-filter-0.9.7/LICENSE` & `python-dict-display-filter-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-0.9.7/PKG-INFO` & `python-dict-display-filter-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-dict-display-filter
-Version: 0.9.7
+Version: 0.9.8
 Summary: A Wireshark-like display filter for dictionaries.
 Home-page: https://github.com/bytebutcher/python-dict-display-filter
 Author: bytebutcher
 Author-email: thomas.engel.web@gmail.com
 License: GPL-3.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-dict-display-filter Version: 0.9.7 Summary:
+Metadata-Version: 2.1 Name: python-dict-display-filter Version: 0.9.8 Summary:
 A Wireshark-like display filter for dictionaries. Home-page: https://
 github.com/bytebutcher/python-dict-display-filter Author: bytebutcher Author-
 email: thomas.engel.web@gmail.com License: GPL-3.0 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
 OS Independent Description-Content-Type: text/markdown License-File: LICENSE
                        [python_dict_display_filter Logo]
                 ****** Python Dictionary Display Filter ******
```

### Comparing `python-dict-display-filter-0.9.7/README.md` & `python-dict-display-filter-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-0.9.7/pydictdisplayfilter/__init__.py` & `python-dict-display-filter-0.9.8/pydictdisplayfilter/__init__.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-0.9.7/pydictdisplayfilter/evaluators/__init__.py` & `python-dict-display-filter-0.9.8/pydictdisplayfilter/evaluators/__init__.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-0.9.7/pydictdisplayfilter/evaluators/common.py` & `python-dict-display-filter-0.9.8/pydictdisplayfilter/evaluators/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 class AbstractEvaluator(ABC):
     """
     A basic evaluator which is ment to be used as base class for other evaluators and is quite useless on its own.
     """
 
     def __init__(self):
         """ Initializes the BasicEvaluator. """
-        self._logger = logging.getLogger()
+        self._logger = logging.getLogger(__name__)
 
     @abstractmethod
     def _convert_expression_value(self, value: Optional[Union[int, str]]) -> Optional[Any]:
         """
         Converts a given value as defined in the expression to a more useful representation.
         :param value: a given value from the actual expression. Since we are kind of in control of the parsing process
                       we may expect an integer, string or None value here.
@@ -300,15 +300,15 @@
         Transform the expression value to an integer. Handles octal, decimal and hexadecimal values as well.
         :param value: A given value from the expression. Since we are kind of in control of the parsing process
                       we may expect an integer, string or None value here.
         :returns the transformed value.
         :raises Exception when value can not be converted. Since we expect either an integer, string or None here
                 it is rather unlikely that an exception is raised here.
         """
-        return not isinstance(value, bool) and int(super()._convert_expression_value(value))
+        return int(value) if isinstance(value, bool) else int(super()._convert_expression_value(value))
 
 
 class IPv4AddressEvaluator(CallbackEvaluator):
     """ Evaluates IPv4 addresses. """
 
     def _convert_item_value(self, value: Any) -> ipaddress.IPv4Address:
         return self._convert_expression_value(value)
```

### Comparing `python-dict-display-filter-0.9.7/pydictdisplayfilter/exceptions.py` & `python-dict-display-filter-0.9.8/pydictdisplayfilter/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-0.9.7/pydictdisplayfilter/factories.py` & `python-dict-display-filter-0.9.8/pydictdisplayfilter/factories.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-0.9.7/pydictdisplayfilter/helpers.py` & `python-dict-display-filter-0.9.8/pydictdisplayfilter/helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,24 +19,27 @@
 import logging
 import os
 import time
 import traceback
 from typing import List, Set
 
 from pydictdisplayfilter import DictDisplayFilter
+from pydictdisplayfilter.display_filters import BaseDisplayFilter
 from pydictdisplayfilter.exceptions import ParserError, EvaluationError
 
 
-class DictTable:
+class TableError(Exception):
+    pass
+
+
+class Table:
     """ Data store with filter capabilities and pretty table printout. """
 
-    def __init__(self, data_store):
-        """ Initializes the DictTable with a data store. """
-        self._data_store = data_store
-        self._dict_display_filter = DictDisplayFilter(data_store)
+    def __init__(self, display_filter: BaseDisplayFilter):
+        self._display_filter = display_filter
 
     def _make_table(self, data_store) -> List[str]:
         """ Creates a table including header from the data store. """
         if not data_store:
             return []
         table = [self.fields()]
         column_size = self._calculate_column_size(data_store)
@@ -48,126 +51,158 @@
         return [""] + [ format_str.format(*item) for item in table ]
 
     def _calculate_column_size(self, data_store) -> List[int]:
         """ Calculates and returns the necessary size of each column in the data store. """
         header = list(data_store[0].keys())
         items = [list(item.values()) for item in data_store]
         return [
-            max(map(len, column)) for column in zip(*items + [header])
+            max(len(str(item)) for item in column) for column in zip(*items + [header])
         ]
 
     def _make_footer(self, items, duration) -> List[str]:
         """ Creates a footer for the table which prints some statistics. """
         item_count = len(items)
         result = [""]
         if item_count == 0:
             result.append("Empty set ({:.2f} secs)".format(duration))
         else:
             type_name = "row" if item_count == 1 else "rows"
             result.append("{} {} in set ({:.2f} secs)".format(item_count, type_name, duration))
         result.append("")
         return result
 
-    def fields(self, thorough: bool = False) -> Set[str]:
-        """
-        Returns the field names used in the data store.
-        :param thorough: if enabled, scans each item in the data store for its field names, otherwise only the first
-                         item is looked upon which is usually enough. Disabled by default.
-        """
-        if not self._data_store:
-            # No items in data store, so there are no fields to query either.
-            return set()
-        if not thorough:
-            return self._data_store[0].keys()
-        else:
-            return set(itertools.chain.from_iterable([item.keys() for item in self._data_store]))
+    def fields(self) -> List[str]:
+        """ Returns the field names used in the data store. """
+        raise NotImplementedError()
 
-    def filter(self, display_filter) -> str:
+    def filter(self, display_filter: str) -> str:
         """
         Filters the items in the data store using the specified display filter and returns the result in a table.
         """
         start = time.time()
-        result = list(self._dict_display_filter.filter(display_filter))
+        result = list(self._display_filter.filter(display_filter))
         end = time.time()
         duration = end - start
         return os.linesep.join(self._make_table(result) + self._make_footer(result, duration))
 
 
-class DictDisplayFilterShell(cmd.Cmd):
+class DisplayFilterShell(cmd.Cmd):
     """ A little shell for the display filter. """
 
     intro = 'Type help or ? to list commands.\n'
     prompt = '> '
 
-    def __init__(self, data_store):
+    def __init__(self, table: Table):
         """ Initializes the DisplayFilterShell with a data store. """
         super().__init__()
-        self._logger = logging.getLogger()
-        self._dict_table = DictTable(data_store)
+        self._logger = self._init_logger()
+        self._table = table
+
+    def _init_logger(self) -> logging.Logger:
+        """ Setups the logger. Makes sure that info messages are actually printed. """
+        logger = logging.getLogger(__name__)
+        logger.setLevel(logging.INFO)
+        return logger
 
     def do_debug(self, *args):
         """ Toggles debug mode on/off. """
         if self._logger.level == logging.DEBUG:
             self._logger.level = logging.INFO
             self._logger.warning("Debug mode disabled")
         else:
             self._logger.level = logging.DEBUG
             self._logger.warning("Debug mode enabled")
 
     def do_fields(self, *args):
         """ Returns the fields the display filter can be applied on. """
         try:
-            for key in self._dict_table.fields():
+            for key in self._table.fields():
                 print(key)
         except Exception as err:
             self._logger.error('There was an error retrieving the fields!')
             self._logger.debug(err)
             if self._logger.level == logging.DEBUG:
                 traceback.print_exc()
 
-    def do_import(self, *args):
-        """ Imports data from a given file. """
-        self._logger.error("This function is currently not implemented!")
-        return False
-
-    def do_export(self, *args):
-        """ Exports the data to a given file. Optional display filter for only exporting specific data. """
-        self._logger.error("This function is currently not implemented!")
-        return False
-
     def do_filter(self, *args):
         """ Applies the given display filter to the data and prints the result. """
         try:
             display_filter = ' '.join(args)
             if not display_filter:
                 self._logger.error("No arguments supplied to filter function.")
                 return
-            print(self._dict_table.filter(display_filter))
+            print(self._table.filter(display_filter))
         except ParserError as err:
             self._logger.error('Invalid display filter!')
             self._logger.debug(err)
             if self._logger.level == logging.DEBUG:
                 traceback.print_exc()
         except EvaluationError as err:
             self._logger.error('There was an unknown error evaluating the results!')
             self._logger.debug(err)
             if self._logger.level == logging.DEBUG:
                 traceback.print_exc()
+        except TableError as err:
+            self._logger.error(err)
+            if self._logger.level == logging.DEBUG:
+                traceback.print_exc()
         except Exception as err:
             self._logger.error('There was an unknown error displaying the results!')
             self._logger.debug(err)
             if self._logger.level == logging.DEBUG:
                 traceback.print_exc()
 
+    def do_import(self, *args):
+        """ Imports data from a given file. """
+        self._logger.error("This function is currently not implemented!")
+        return False
+
+    def do_export(self, *args):
+        """ Exports the data to a given file. Optional display filter for only exporting specific data. """
+        self._logger.error("This function is currently not implemented!")
+        return False
+
     def get_names(self):
         """ Override get_names() method of cmd.Cmd to remove functions from the help we do not want to show. """
         names = super().get_names()
         names.remove('do_EOF')
         return names
 
     def do_EOF(self, line):
         """ Exit application when pressing CTRL+D. """
         return True
 
     def do_exit(self, *args):
         """ Exit application. """
         return True
+
+
+class DictTable(Table):
+    """ Data store with filter capabilities and pretty table printout. """
+
+    def __init__(self, data_store: List[dict]):
+        """ Initializes the DictTable with a data store. """
+        self._data_store = data_store
+        super().__init__(DictDisplayFilter(data_store))
+
+    def fields(self, thorough: bool = False) -> List[str]:
+        """
+        Returns the field names used in the data store.
+        :param thorough: if enabled, scans each item in the data store for its field names, otherwise only the first
+                         item is looked upon which is usually enough. Disabled by default.
+        """
+        if not self._data_store:
+            # No items in data store, so there are no fields to query either.
+            return list()
+
+        if not thorough:
+            return list(self._data_store[0].keys())
+        else:
+            return itertools.chain.from_iterable([item.keys() for item in self._data_store])
+
+
+class DictDisplayFilterShell(DisplayFilterShell):
+    """ A little shell for querying a list of dictionaries using the display filter. """
+
+    def __init__(self, data_store: List[dict]):
+        """ Initializes the DictDisplayFilterShell with a data store. """
+        super().__init__(DictTable(data_store))
```

### Comparing `python-dict-display-filter-0.9.7/pydictdisplayfilter/models.py` & `python-dict-display-filter-0.9.8/pydictdisplayfilter/models.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-0.9.7/pydictdisplayfilter/parsers/__init__.py` & `python-dict-display-filter-0.9.8/pydictdisplayfilter/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-0.9.7/pydictdisplayfilter/parsers/common.py` & `python-dict-display-filter-0.9.8/pydictdisplayfilter/parsers/common.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-0.9.7/pydictdisplayfilter/parsers/display_filter.py` & `python-dict-display-filter-0.9.8/pydictdisplayfilter/parsers/display_filter.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-0.9.7/pydictdisplayfilter/slicers.py` & `python-dict-display-filter-0.9.8/pydictdisplayfilter/slicers.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-0.9.7/python_dict_display_filter.egg-info/PKG-INFO` & `python-dict-display-filter-0.9.8/python_dict_display_filter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-dict-display-filter
-Version: 0.9.7
+Version: 0.9.8
 Summary: A Wireshark-like display filter for dictionaries.
 Home-page: https://github.com/bytebutcher/python-dict-display-filter
 Author: bytebutcher
 Author-email: thomas.engel.web@gmail.com
 License: GPL-3.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-dict-display-filter Version: 0.9.7 Summary:
+Metadata-Version: 2.1 Name: python-dict-display-filter Version: 0.9.8 Summary:
 A Wireshark-like display filter for dictionaries. Home-page: https://
 github.com/bytebutcher/python-dict-display-filter Author: bytebutcher Author-
 email: thomas.engel.web@gmail.com License: GPL-3.0 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
 OS Independent Description-Content-Type: text/markdown License-File: LICENSE
                        [python_dict_display_filter Logo]
                 ****** Python Dictionary Display Filter ******
```

### Comparing `python-dict-display-filter-0.9.7/python_dict_display_filter.egg-info/SOURCES.txt` & `python-dict-display-filter-0.9.8/python_dict_display_filter.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,8 +17,9 @@
 python_dict_display_filter.egg-info/SOURCES.txt
 python_dict_display_filter.egg-info/dependency_links.txt
 python_dict_display_filter.egg-info/requires.txt
 python_dict_display_filter.egg-info/top_level.txt
 tests/__init__.py
 tests/test_dict_display_filter.py
 tests/test_display_filter_parser.py
-tests/test_slicers.py
+tests/test_slicers.py
+tests/test_sql_display_filter.py
```

### Comparing `python-dict-display-filter-0.9.7/setup.py` & `python-dict-display-filter-0.9.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,28 +7,29 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="python-dict-display-filter",
-    version="0.9.7",
+    version="0.9.8",
     description="A Wireshark-like display filter for dictionaries.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/bytebutcher/python-dict-display-filter",
     author="bytebutcher",
     author_email="thomas.engel.web@gmail.com",
     license="GPL-3.0",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent"
     ],
     packages=setuptools.find_packages(),
     install_requires=[
+        'packaging==23.1',
         'parameterized==0.8.1',
         'pyparsing==3.0.6',
         'ipranger==1.1.2',
         'python-dateutil==2.8.2'
     ],
     include_package_data=True,
 )
```

### Comparing `python-dict-display-filter-0.9.7/tests/__init__.py` & `python-dict-display-filter-0.9.8/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-0.9.7/tests/test_dict_display_filter.py` & `python-dict-display-filter-0.9.8/tests/test_dict_display_filter.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-0.9.7/tests/test_display_filter_parser.py` & `python-dict-display-filter-0.9.8/tests/test_display_filter_parser.py`

 * *Files identical despite different names*

### Comparing `python-dict-display-filter-0.9.7/tests/test_slicers.py` & `python-dict-display-filter-0.9.8/tests/test_slicers.py`

 * *Files identical despite different names*

