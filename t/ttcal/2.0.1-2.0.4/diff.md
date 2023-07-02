# Comparing `tmp/ttcal-2.0.1.tar.gz` & `tmp/ttcal-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ttcal-2.0.1.tar", last modified: Tue Sep 27 01:20:14 2022, max compression
+gzip compressed data, was "ttcal-2.0.4.tar", last modified: Sun Jul  2 19:53:12 2023, max compression
```

## Comparing `ttcal-2.0.1.tar` & `ttcal-2.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2022-09-27 01:20:14.000000 ttcal-2.0.1/
--rw-rw-rw-   0        0        0     1057 2020-08-20 19:43:04.000000 ttcal-2.0.1/LICENSE
--rw-rw-rw-   0        0        0     1457 2022-09-27 01:20:14.000000 ttcal-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      763 2020-08-20 19:43:04.000000 ttcal-2.0.1/README.rst
--rw-rw-rw-   0        0        0       68 2022-09-27 01:20:14.000000 ttcal-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0      911 2022-09-27 01:19:15.000000 ttcal-2.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-09-27 01:20:14.000000 ttcal-2.0.1/ttcal/
--rw-rw-rw-   0        0        0     1778 2022-09-27 00:56:19.000000 ttcal-2.0.1/ttcal/calfns.py
--rw-rw-rw-   0        0        0    14932 2022-09-27 00:59:27.000000 ttcal-2.0.1/ttcal/day.py
--rw-rw-rw-   0        0        0     8940 2022-09-27 00:59:27.000000 ttcal-2.0.1/ttcal/duration.py
--rw-rw-rw-   0        0        0    10783 2022-09-27 00:56:20.000000 ttcal-2.0.1/ttcal/month.py
-drwxrwxrwx   0        0        0        0 2022-09-27 01:20:14.000000 ttcal-2.0.1/ttcal/templatetags/
--rw-rw-rw-   0        0        0      989 2022-09-27 00:59:27.000000 ttcal-2.0.1/ttcal/templatetags/ttcal_tags.py
--rw-rw-rw-   0        0        0        0 2020-08-20 19:43:04.000000 ttcal-2.0.1/ttcal/templatetags/__init__.py
--rw-rw-rw-   0        0        0     6399 2022-09-27 00:12:48.000000 ttcal-2.0.1/ttcal/week.py
--rw-rw-rw-   0        0        0     8524 2022-09-27 00:56:20.000000 ttcal-2.0.1/ttcal/year.py
--rw-rw-rw-   0        0        0      494 2022-09-27 01:19:15.000000 ttcal-2.0.1/ttcal/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-27 01:20:14.000000 ttcal-2.0.1/ttcal.egg-info/
--rw-rw-rw-   0        0        0        1 2022-09-27 01:20:14.000000 ttcal-2.0.1/ttcal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2020-08-20 20:02:17.000000 ttcal-2.0.1/ttcal.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     1457 2022-09-27 01:20:14.000000 ttcal-2.0.1/ttcal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      353 2022-09-27 01:20:14.000000 ttcal-2.0.1/ttcal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        6 2022-09-27 01:20:14.000000 ttcal-2.0.1/ttcal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:53:12.643231 ttcal-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-02 19:53:00.000000 ttcal-2.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-02 19:53:12.643231 ttcal-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-02 19:53:00.000000 ttcal-2.0.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-02 19:53:12.643231 ttcal-2.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-02 19:53:00.000000 ttcal-2.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:53:12.643231 ttcal-2.0.4/ttcal/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-02 19:53:00.000000 ttcal-2.0.4/ttcal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-02 19:53:00.000000 ttcal-2.0.4/ttcal/calfns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15869 2023-07-02 19:53:00.000000 ttcal-2.0.4/ttcal/day.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9262 2023-07-02 19:53:00.000000 ttcal-2.0.4/ttcal/duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10783 2023-07-02 19:53:00.000000 ttcal-2.0.4/ttcal/month.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:53:12.643231 ttcal-2.0.4/ttcal/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 19:53:00.000000 ttcal-2.0.4/ttcal/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-02 19:53:00.000000 ttcal-2.0.4/ttcal/templatetags/ttcal_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-07-02 19:53:00.000000 ttcal-2.0.4/ttcal/week.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-07-02 19:53:00.000000 ttcal-2.0.4/ttcal/year.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:53:12.643231 ttcal-2.0.4/ttcal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-02 19:53:12.000000 ttcal-2.0.4/ttcal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-02 19:53:12.000000 ttcal-2.0.4/ttcal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 19:53:12.000000 ttcal-2.0.4/ttcal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 19:53:12.000000 ttcal-2.0.4/ttcal.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-02 19:53:12.000000 ttcal-2.0.4/ttcal.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ttcal-2.0.1/LICENSE` & `ttcal-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ttcal-2.0.1/setup.py` & `ttcal-2.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Programming Language :: Python :: 3
 Topic :: Software Development :: Libraries
 """
 
 import sys, os
 import setuptools
 
-version = '2.0.1'
+version = '2.0.4'
 
 DIRNAME = os.path.dirname(__file__)
 description = open(os.path.join(DIRNAME, 'README.rst'), 'r').read()
 
 
 setuptools.setup(
     name='ttcal',
```

### Comparing `ttcal-2.0.1/ttcal/calfns.py` & `ttcal-2.0.4/ttcal/calfns.py`

 * *Files identical despite different names*

### Comparing `ttcal-2.0.1/ttcal/day.py` & `ttcal-2.0.4/ttcal/day.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,45 +2,78 @@
 Date (single day) operations.
 """
 import calendar
 import datetime
 import re
 from .calfns import rangecmp, rangetuple
 from .duration import Duration, Period
+from typing import List, Tuple
 
 
 class fstr(str):
     """String sub-class with a split() method that splits a given indexes.
 
        Usage::
-          >>> from __future__ import print_function
           >>> r = fstr('D2008022002')
           >>> print(r.split(1, 5, 7, 9))
           ['D', '2008', '02', '20', '02']
           >>> _, year, _ = r.split(1,5)
           >>> year
           '2008'
 
     """
-    def split(self, *ndxs):
-        if len(ndxs) == 0:
+    def _validate_indexes(self, *ndxs: Tuple[int]) -> Tuple[int]:
+        """Return indexes that are valid for this string, in order.
+        """
+        ndxs = sorted(set(ndxs))
+        if not ndxs:
+            return []
+        if ndxs and ndxs[0] == 0:
+            ndxs = ndxs[1:]
+        while ndxs and ndxs[-1] > len(self):
+            ndxs = ndxs[:-1]
+        return ndxs
+
+    def split(self, *ndxs: Tuple[int]) -> List[str]:
+        ndxs = self._validate_indexes(*ndxs)
+        if not ndxs:
             return [self]
-        if len(ndxs) == 1:
-            i = ndxs[0]
-            return [self[:i], self[i:]]
 
         res = []
         b = 0
         while ndxs:
             a, b, ndxs = b, ndxs[0], ndxs[1:]
             res.append(self[a:b])
         res.append(self[b:])
 
         return res
 
+    @classmethod
+    def join(cls, strings: List[str], *ndxs: Tuple[int]) -> str:
+        ndxs = [n for n in ndxs if n > 0]
+        if not ndxs:
+            return strings[0] if strings else ''
+        res = ''
+        for s, n in zip(strings, ndxs):
+            res += s[:n]
+        res += strings[-1]
+        return res
+
+
+def fsplit(strval: str, *ndxs: Tuple[int]) -> List[str]:
+    """Split a string at given indexes.
+    """
+    return fstr(strval).split(*ndxs)
+
+
+def fjoin(strings: List[str], *ndxs: Tuple[int]) -> str:
+    """Join a sequence of strings.
+    """
+    return fstr.join(strings, *ndxs)
+
 
 class Day(datetime.date):  # pylint:disable=too-many-public-methods
     """A calendar date.
     """
 
     day_name = '''mandag tirsdag onsdag torsdag fredag
                   lørdag søndag'''.split()
```

### Comparing `ttcal-2.0.1/ttcal/duration.py` & `ttcal-2.0.4/ttcal/duration.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,15 +56,15 @@
             start = cls(0)
         res = start
         for item in sequence:
             res += item
         return res
 
     @classmethod
-    def parse(cls, txt):
+    def parse(cls, txt, raise_on_error=False):
         """Parse a textual representation into a Duration object.
            Format HHH:MM:SS.
         """
         if not txt:
             return None
 
         time_matcher = re.compile(r"""
@@ -83,14 +83,18 @@
                 (?P<hours>\d+):
                 (?P<minutes>\d+)
                 (?::(?P<seconds>\d+)
                 (?:\.(?P<microseconds>\d+))?)?
             )?
             """, re.VERBOSE)
         time_matches = time_matcher.match(txt)
+        if raise_on_error and not time_matches:
+            raise ValueError(f"Couldn't parse {txt} as a duration.")
+        if raise_on_error and time_matches.span()[1] != len(txt):
+            raise ValueError(f"Remaining text: {txt[time_matches.span()[1]:]} could not be parsed as a duration.")
         time_groups = time_matches.groupdict()
         keys = list(time_groups.keys())
 
         if time_groups.get('negation') == '-':
             scale = -1
             keys.remove('negation')
         else:
@@ -160,15 +164,15 @@
         return int(sgn == "") * hr
 
     @property
     def hours(self):
         """The number of hours in self (not including days).
         """
         sgn, hr, _mn, _sc = self.duration_tuple()
-        return int(sgn == "") * (hr%24)
+        return int(sgn == "") * (hr % 24)
 
     @property
     def mins(self):
         """The number of minutes in self.
         """
         sgn, _hr, mn, _sc = self.duration_tuple()
         return int(sgn == "") * mn
```

### Comparing `ttcal-2.0.1/ttcal/month.py` & `ttcal-2.0.4/ttcal/month.py`

 * *Files identical despite different names*

### Comparing `ttcal-2.0.1/ttcal/templatetags/ttcal_tags.py` & `ttcal-2.0.4/ttcal/templatetags/ttcal_tags.py`

 * *Files identical despite different names*

### Comparing `ttcal-2.0.1/ttcal/week.py` & `ttcal-2.0.4/ttcal/week.py`

 * *Files identical despite different names*

### Comparing `ttcal-2.0.1/ttcal/year.py` & `ttcal-2.0.4/ttcal/year.py`

 * *Files identical despite different names*

