# Comparing `tmp/timer-module-1.1.2.tar.gz` & `tmp/timer-module-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timer-module-1.1.2.tar", last modified: Sat Jul  1 15:23:35 2023, max compression
+gzip compressed data, was "timer-module-1.1.3.tar", last modified: Sun Jul  2 20:42:22 2023, max compression
```

## Comparing `timer-module-1.1.2.tar` & `timer-module-1.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 15:23:35.509932 timer-module-1.1.2/
--rw-rw-rw-   0        0        0     1091 2023-02-11 02:09:32.000000 timer-module-1.1.2/LICENSE
--rw-rw-rw-   0        0        0     2428 2023-07-01 15:23:35.508931 timer-module-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1859 2023-05-20 04:26:53.000000 timer-module-1.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-01 15:23:35.509932 timer-module-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      902 2023-07-01 15:20:34.000000 timer-module-1.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-01 15:23:35.501899 timer-module-1.1.2/timer_module/
--rw-rw-rw-   0        0        0      127 2023-05-20 04:38:26.000000 timer-module-1.1.2/timer_module/__init__.py
--rw-rw-rw-   0        0        0     6004 2023-07-01 15:20:18.000000 timer-module-1.1.2/timer_module/metrics.py
--rw-rw-rw-   0        0        0     7178 2023-07-01 10:42:41.000000 timer-module-1.1.2/timer_module/profiler.py
--rw-rw-rw-   0        0        0     1358 2023-06-29 22:39:56.000000 timer-module-1.1.2/timer_module/terminal.py
--rw-rw-rw-   0        0        0     1459 2023-05-20 04:38:26.000000 timer-module-1.1.2/timer_module/timer.py
-drwxrwxrwx   0        0        0        0 2023-07-01 15:23:35.507925 timer-module-1.1.2/timer_module.egg-info/
--rw-rw-rw-   0        0        0     2428 2023-07-01 15:23:35.000000 timer-module-1.1.2/timer_module.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2023-07-01 15:23:35.000000 timer-module-1.1.2/timer_module.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 15:23:35.000000 timer-module-1.1.2/timer_module.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-01 15:23:35.000000 timer-module-1.1.2/timer_module.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-01 15:23:35.000000 timer-module-1.1.2/timer_module.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-02 20:42:22.233569 timer-module-1.1.3/
+-rw-rw-rw-   0        0        0     1091 2023-02-11 02:09:32.000000 timer-module-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0     2428 2023-07-02 20:42:22.233569 timer-module-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1859 2023-05-20 04:26:53.000000 timer-module-1.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-02 20:42:22.234570 timer-module-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      902 2023-07-02 20:41:15.000000 timer-module-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 20:42:22.211543 timer-module-1.1.3/timer_module/
+-rw-rw-rw-   0        0        0      127 2023-05-20 04:38:26.000000 timer-module-1.1.3/timer_module/__init__.py
+-rw-rw-rw-   0        0        0     6019 2023-07-02 20:34:07.000000 timer-module-1.1.3/timer_module/metrics.py
+-rw-rw-rw-   0        0        0     7032 2023-07-02 20:35:17.000000 timer-module-1.1.3/timer_module/profiler.py
+-rw-rw-rw-   0        0        0     1358 2023-06-29 22:39:56.000000 timer-module-1.1.3/timer_module/terminal.py
+-rw-rw-rw-   0        0        0     1459 2023-05-20 04:38:26.000000 timer-module-1.1.3/timer_module/timer.py
+drwxrwxrwx   0        0        0        0 2023-07-02 20:42:22.232569 timer-module-1.1.3/timer_module.egg-info/
+-rw-rw-rw-   0        0        0     2428 2023-07-02 20:42:22.000000 timer-module-1.1.3/timer_module.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2023-07-02 20:42:22.000000 timer-module-1.1.3/timer_module.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 20:42:22.000000 timer-module-1.1.3/timer_module.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-02 20:42:22.000000 timer-module-1.1.3/timer_module.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-02 20:42:22.000000 timer-module-1.1.3/timer_module.egg-info/top_level.txt
```

### Comparing `timer-module-1.1.2/LICENSE` & `timer-module-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `timer-module-1.1.2/PKG-INFO` & `timer-module-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timer-module
-Version: 1.1.2
+Version: 1.1.3
 Summary: Timer Module with performance profiling features
 Home-page: https://github.com/syn-chromatic/timer-module
 Author: syn-chromatic
 Author-email: synchromatic.github@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `timer-module-1.1.2/README.md` & `timer-module-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `timer-module-1.1.2/setup.py` & `timer-module-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path
 from setuptools import setup, find_packages
 
-VERSION = "1.1.2"
+VERSION = "1.1.3"
 DESCRIPTION = "Timer Module with performance profiling features"
 
 root = Path(__file__).parent
 long_description = (root / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="timer-module",
```

### Comparing `timer-module-1.1.2/timer_module/metrics.py` & `timer-module-1.1.3/timer_module/metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,20 @@
         return self.format_nanoseconds()
 
 
 class CallableMetrics:
     __slots__ = ("name", "module", "call_hash", "ncalls", "time_ns")
 
     def __init__(
-        self, name: str, module: str, call_hash: int, ncalls: int, time_ns: float
+        self,
+        name: str,
+        module: str,
+        call_hash: int,
+        ncalls: int,
+        time_ns: float,
     ):
         self.name = name
         self.module = module
         self.call_hash = call_hash
         self.ncalls = ncalls
         self.time_ns = time_ns
 
@@ -143,15 +148,14 @@
             total_time += callable_refs[pcall_hash].time_ns
         return total_time
 
     def write_report(
         self,
         callable_refs: dict[int, CallableMetrics],
         timing_refs: dict[int, dict[int, CallableMetrics]],
-        total_time_ns: float,
     ):
         for pcall_hash, subcalls in timing_refs.items():
             pcall_metrics = callable_refs[pcall_hash]
             self.write_primary_call_header(pcall_metrics)
             pcall_time = pcall_metrics.time_ns
             for _, subcall_metrics in subcalls.items():
                 if subcall_metrics == pcall_metrics:
```

### Comparing `timer-module-1.1.2/timer_module/profiler.py` & `timer-module-1.1.3/timer_module/profiler.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,27 +18,25 @@
         self._realtime: bool = realtime
 
     def __new__(cls, *args, **kwargs):
         if not hasattr(cls, "instance") or not isinstance(cls.instance, cls):
             cls.instance = super(TimeProfilerBase, cls).__new__(cls)
             cls._callable_refs: dict[int, CallableMetrics] = {}
             cls._timing_refs: dict[int, dict[int, CallableMetrics]] = {}
-            cls._timing_total: float = 0.0
             cls._pcall_hash: Optional[int] = None
         return cls.instance
 
     def __del__(self) -> None:
         self._print_report()
 
     def _print_report(self, realtime: bool = False):
         metrics_report = ProfileMetricsReport(realtime)
         callable_refs = self._callable_refs
         timing_refs = self._timing_refs
-        total_time = self._timing_total
-        metrics_report.write_report(callable_refs, timing_refs, total_time)
+        metrics_report.write_report(callable_refs, timing_refs)
 
     @staticmethod
     def _set_attribute(instance: CT, name: str, method: Callable) -> CT:
         try:
             instance.__setattr__(name, method)
         except AttributeError:
             print(f"Class Method ({name}) is read-only and cannot be timed.")
@@ -49,16 +47,14 @@
         pcall_hash = self._pcall_hash
 
         if pcall_hash is not None:
             if call_hash == pcall_hash:
                 call_metrics = callable_refs[call_hash]
                 call_metrics.time_ns += time_ns
                 call_metrics.ncalls += 1
-
-                self._timing_total += time_ns
                 self._pcall_hash = None
 
                 if self._realtime:
                     self._print_report(realtime=True)
             else:
                 call_metrics = self._timing_refs[pcall_hash][call_hash]
                 call_metrics.time_ns += time_ns
```

### Comparing `timer-module-1.1.2/timer_module/terminal.py` & `timer-module-1.1.3/timer_module/terminal.py`

 * *Files identical despite different names*

### Comparing `timer-module-1.1.2/timer_module/timer.py` & `timer-module-1.1.3/timer_module/timer.py`

 * *Files identical despite different names*

### Comparing `timer-module-1.1.2/timer_module.egg-info/PKG-INFO` & `timer-module-1.1.3/timer_module.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timer-module
-Version: 1.1.2
+Version: 1.1.3
 Summary: Timer Module with performance profiling features
 Home-page: https://github.com/syn-chromatic/timer-module
 Author: syn-chromatic
 Author-email: synchromatic.github@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

