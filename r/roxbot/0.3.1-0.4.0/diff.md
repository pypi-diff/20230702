# Comparing `tmp/roxbot-0.3.1.tar.gz` & `tmp/roxbot-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roxbot-0.3.1.tar", last modified: Wed Jun 28 16:13:34 2023, max compression
+gzip compressed data, was "roxbot-0.4.0.tar", last modified: Sun Jul  2 18:55:29 2023, max compression
```

## Comparing `roxbot-0.3.1.tar` & `roxbot-0.4.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 16:13:34.818577 roxbot-0.3.1/
--rw-rw-rw-   0 root         (0) root         (0)     1081 2023-06-28 16:13:23.000000 roxbot-0.3.1/LICENCE
--rw-r--r--   0 root         (0) root         (0)      382 2023-06-28 16:13:34.818577 roxbot-0.3.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1734 2023-06-28 16:13:23.000000 roxbot-0.3.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      360 2023-06-28 16:13:34.819578 roxbot-0.3.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1570 2023-06-28 16:13:23.000000 roxbot-0.3.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 16:13:34.811578 roxbot-0.3.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 16:13:34.814577 roxbot-0.3.1/src/roxbot/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-28 16:13:23.000000 roxbot-0.3.1/src/roxbot/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1095 2023-06-28 16:13:23.000000 roxbot-0.3.1/src/roxbot/base_classes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 16:13:34.816578 roxbot-0.3.1/src/roxbot/bridges/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-28 16:13:23.000000 roxbot-0.3.1/src/roxbot/bridges/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4917 2023-06-28 16:13:23.000000 roxbot-0.3.1/src/roxbot/bridges/web_bridge.py
--rw-rw-rw-   0 root         (0) root         (0)      302 2023-06-28 16:13:23.000000 roxbot-0.3.1/src/roxbot/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     5874 2023-06-28 16:13:23.000000 roxbot-0.3.1/src/roxbot/gps.py
--rw-rw-rw-   0 root         (0) root         (0)      337 2023-06-28 16:13:23.000000 roxbot-0.3.1/src/roxbot/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     5514 2023-06-28 16:13:23.000000 roxbot-0.3.1/src/roxbot/models.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-28 16:13:23.000000 roxbot-0.3.1/src/roxbot/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 16:13:34.816578 roxbot-0.3.1/src/roxbot/simulators/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-28 16:13:23.000000 roxbot-0.3.1/src/roxbot/simulators/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1809 2023-06-28 16:13:23.000000 roxbot-0.3.1/src/roxbot/simulators/trike.py
--rw-rw-rw-   0 root         (0) root         (0)      209 2023-06-28 16:13:23.000000 roxbot-0.3.1/src/roxbot/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     5020 2023-06-28 16:13:23.000000 roxbot-0.3.1/src/roxbot/vectors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 16:13:34.816578 roxbot-0.3.1/src/roxbot.egg-info/
--rw-r--r--   0 root         (0) root         (0)      382 2023-06-28 16:13:34.000000 roxbot-0.3.1/src/roxbot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      770 2023-06-28 16:13:34.000000 roxbot-0.3.1/src/roxbot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 16:13:34.000000 roxbot-0.3.1/src/roxbot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-06-28 16:13:34.000000 roxbot-0.3.1/src/roxbot.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 16:13:26.000000 roxbot-0.3.1/src/roxbot.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       55 2023-06-28 16:13:34.000000 roxbot-0.3.1/src/roxbot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-28 16:13:34.000000 roxbot-0.3.1/src/roxbot.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 16:13:34.818577 roxbot-0.3.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)      462 2023-06-28 16:13:23.000000 roxbot-0.3.1/tests/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2780 2023-06-28 16:13:23.000000 roxbot-0.3.1/tests/test_gps.py
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-06-28 16:13:23.000000 roxbot-0.3.1/tests/test_interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2070 2023-06-28 16:13:23.000000 roxbot-0.3.1/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)     1591 2023-06-28 16:13:23.000000 roxbot-0.3.1/tests/test_trike.py
--rw-rw-rw-   0 root         (0) root         (0)      748 2023-06-28 16:13:23.000000 roxbot-0.3.1/tests/test_trike_sim.py
--rw-rw-rw-   0 root         (0) root         (0)     2781 2023-06-28 16:13:23.000000 roxbot-0.3.1/tests/test_vectors.py
--rw-rw-rw-   0 root         (0) root         (0)     1982 2023-06-28 16:13:23.000000 roxbot-0.3.1/tests/test_ws_bridge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:55:29.285815 roxbot-0.4.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1081 2023-07-02 18:55:17.000000 roxbot-0.4.0/LICENCE
+-rw-r--r--   0 root         (0) root         (0)      382 2023-07-02 18:55:29.285815 roxbot-0.4.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1734 2023-07-02 18:55:17.000000 roxbot-0.4.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      360 2023-07-02 18:55:29.286815 roxbot-0.4.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1570 2023-07-02 18:55:17.000000 roxbot-0.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:55:29.279815 roxbot-0.4.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:55:29.282815 roxbot-0.4.0/src/roxbot/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-02 18:55:17.000000 roxbot-0.4.0/src/roxbot/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1095 2023-07-02 18:55:17.000000 roxbot-0.4.0/src/roxbot/base_classes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:55:29.283815 roxbot-0.4.0/src/roxbot/bridges/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-02 18:55:17.000000 roxbot-0.4.0/src/roxbot/bridges/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4917 2023-07-02 18:55:17.000000 roxbot-0.4.0/src/roxbot/bridges/web_bridge.py
+-rw-rw-rw-   0 root         (0) root         (0)      302 2023-07-02 18:55:17.000000 roxbot-0.4.0/src/roxbot/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     5874 2023-07-02 18:55:17.000000 roxbot-0.4.0/src/roxbot/gps.py
+-rw-rw-rw-   0 root         (0) root         (0)      337 2023-07-02 18:55:17.000000 roxbot-0.4.0/src/roxbot/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     5666 2023-07-02 18:55:17.000000 roxbot-0.4.0/src/roxbot/models.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-02 18:55:17.000000 roxbot-0.4.0/src/roxbot/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:55:29.284815 roxbot-0.4.0/src/roxbot/simulators/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-02 18:55:17.000000 roxbot-0.4.0/src/roxbot/simulators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1809 2023-07-02 18:55:17.000000 roxbot-0.4.0/src/roxbot/simulators/trike.py
+-rw-rw-rw-   0 root         (0) root         (0)      209 2023-07-02 18:55:17.000000 roxbot-0.4.0/src/roxbot/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     5020 2023-07-02 18:55:17.000000 roxbot-0.4.0/src/roxbot/vectors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:55:29.283815 roxbot-0.4.0/src/roxbot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      382 2023-07-02 18:55:29.000000 roxbot-0.4.0/src/roxbot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      770 2023-07-02 18:55:29.000000 roxbot-0.4.0/src/roxbot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 18:55:29.000000 roxbot-0.4.0/src/roxbot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-07-02 18:55:29.000000 roxbot-0.4.0/src/roxbot.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 18:55:21.000000 roxbot-0.4.0/src/roxbot.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-02 18:55:29.000000 roxbot-0.4.0/src/roxbot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-02 18:55:29.000000 roxbot-0.4.0/src/roxbot.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:55:29.285815 roxbot-0.4.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      462 2023-07-02 18:55:17.000000 roxbot-0.4.0/tests/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2780 2023-07-02 18:55:17.000000 roxbot-0.4.0/tests/test_gps.py
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-07-02 18:55:17.000000 roxbot-0.4.0/tests/test_interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2152 2023-07-02 18:55:17.000000 roxbot-0.4.0/tests/test_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1591 2023-07-02 18:55:17.000000 roxbot-0.4.0/tests/test_trike.py
+-rw-rw-rw-   0 root         (0) root         (0)      748 2023-07-02 18:55:17.000000 roxbot-0.4.0/tests/test_trike_sim.py
+-rw-rw-rw-   0 root         (0) root         (0)     2781 2023-07-02 18:55:17.000000 roxbot-0.4.0/tests/test_vectors.py
+-rw-rw-rw-   0 root         (0) root         (0)     1982 2023-07-02 18:55:17.000000 roxbot-0.4.0/tests/test_ws_bridge.py
```

### Comparing `roxbot-0.3.1/LICENCE` & `roxbot-0.4.0/LICENCE`

 * *Files identical despite different names*

### Comparing `roxbot-0.3.1/README.md` & `roxbot-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `roxbot-0.3.1/setup.py` & `roxbot-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.3.1/src/roxbot/base_classes.py` & `roxbot-0.4.0/src/roxbot/base_classes.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.3.1/src/roxbot/bridges/web_bridge.py` & `roxbot-0.4.0/src/roxbot/bridges/web_bridge.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.3.1/src/roxbot/gps.py` & `roxbot-0.4.0/src/roxbot/gps.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.3.1/src/roxbot/models.py` & `roxbot-0.4.0/src/roxbot/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,21 +74,26 @@
             self.val = max(self.val, self.min_val)
 
 
 class Wheel:
     """simple wheel model with a linear speed profile"""
 
     def __init__(self, diameter: float, accel: float):
-        """create a wheel wit LinearModel driver and a diameter"""
+        """create a wheel wit LinearModel driver and a diameter
+        Parameters
+        ----------
+        diameter : float [m] wheel diameter
+        accel : float [m/s^2] acceleration"""
+
         self._diameter = diameter
         self._circumference = math.pi * self._diameter
         self.time = 0.0
 
         # angular velocity model
-        self._model = LinearModel(roc=accel)
+        self._model = LinearModel(roc=1 / self._circumference * accel)
 
         self.revolutions = 0.0
 
     @property
     def rps(self) -> float:
         """revolutions per second"""
         return self._model.val
```

### Comparing `roxbot-0.3.1/src/roxbot/simulators/trike.py` & `roxbot-0.4.0/src/roxbot/simulators/trike.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.3.1/src/roxbot/vectors.py` & `roxbot-0.4.0/src/roxbot/vectors.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.3.1/src/roxbot.egg-info/SOURCES.txt` & `roxbot-0.4.0/src/roxbot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `roxbot-0.3.1/tests/test_gps.py` & `roxbot-0.4.0/tests/test_gps.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.3.1/tests/test_models.py` & `roxbot-0.4.0/tests/test_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,18 @@
 def test_wheel():
     # create a wheel with a diameter of 1 meter and an acceleration of 1 radian per second squared # noqa
     wheel = Wheel(diameter=1.0, accel=1.0)
 
     # set the velocity of the wheel to 1 meter per second
     wheel.set_velocity_ms(1.0)
 
+    # check acceleration
+    wheel.step(0.5)
+    assert wheel.velocity_ms == 0.5
+
     # simulate time passing with a time step of 10 second
     wheel.step(dt=10.0)
 
     # get distance
     _ = wheel.distance
 
     # check that the wheel's angular velocity is correct
```

### Comparing `roxbot-0.3.1/tests/test_trike.py` & `roxbot-0.4.0/tests/test_trike.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.3.1/tests/test_trike_sim.py` & `roxbot-0.4.0/tests/test_trike_sim.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.3.1/tests/test_vectors.py` & `roxbot-0.4.0/tests/test_vectors.py`

 * *Files identical despite different names*

### Comparing `roxbot-0.3.1/tests/test_ws_bridge.py` & `roxbot-0.4.0/tests/test_ws_bridge.py`

 * *Files identical despite different names*

