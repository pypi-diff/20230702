# Comparing `tmp/jvc_projector_remote_improved2-3.7.0.tar.gz` & `tmp/jvc_projector_remote_improved2-3.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jvc_projector_remote_improved2-3.7.0.tar", last modified: Mon Jun 19 19:09:30 2023, max compression
+gzip compressed data, was "jvc_projector_remote_improved2-3.7.2.tar", last modified: Sun Jul  2 17:16:07 2023, max compression
```

## Comparing `jvc_projector_remote_improved2-3.7.0.tar` & `jvc_projector_remote_improved2-3.7.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:09:30.008897 jvc_projector_remote_improved2-3.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-19 19:09:16.000000 jvc_projector_remote_improved2-3.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7296 2023-06-19 19:09:30.008897 jvc_projector_remote_improved2-3.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-06-19 19:09:16.000000 jvc_projector_remote_improved2-3.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:09:30.008897 jvc_projector_remote_improved2-3.7.0/jvc_projector/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-19 19:09:16.000000 jvc_projector_remote_improved2-3.7.0/jvc_projector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-06-19 19:09:16.000000 jvc_projector_remote_improved2-3.7.0/jvc_projector/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    23311 2023-06-19 19:09:16.000000 jvc_projector_remote_improved2-3.7.0/jvc_projector/jvc_projector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:09:30.008897 jvc_projector_remote_improved2-3.7.0/jvc_projector_remote_improved2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7296 2023-06-19 19:09:29.000000 jvc_projector_remote_improved2-3.7.0/jvc_projector_remote_improved2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-19 19:09:30.000000 jvc_projector_remote_improved2-3.7.0/jvc_projector_remote_improved2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 19:09:29.000000 jvc_projector_remote_improved2-3.7.0/jvc_projector_remote_improved2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-19 19:09:29.000000 jvc_projector_remote_improved2-3.7.0/jvc_projector_remote_improved2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 19:09:30.008897 jvc_projector_remote_improved2-3.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-19 19:09:16.000000 jvc_projector_remote_improved2-3.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:09:30.008897 jvc_projector_remote_improved2-3.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 19:09:16.000000 jvc_projector_remote_improved2-3.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-19 19:09:16.000000 jvc_projector_remote_improved2-3.7.0/tests/testLowLatency.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:16:07.930833 jvc_projector_remote_improved2-3.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-02 17:15:56.000000 jvc_projector_remote_improved2-3.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7296 2023-07-02 17:16:07.930833 jvc_projector_remote_improved2-3.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-07-02 17:15:56.000000 jvc_projector_remote_improved2-3.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:16:07.926833 jvc_projector_remote_improved2-3.7.2/jvc_projector/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-02 17:15:56.000000 jvc_projector_remote_improved2-3.7.2/jvc_projector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-07-02 17:15:56.000000 jvc_projector_remote_improved2-3.7.2/jvc_projector/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23311 2023-07-02 17:15:56.000000 jvc_projector_remote_improved2-3.7.2/jvc_projector/jvc_projector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:16:07.930833 jvc_projector_remote_improved2-3.7.2/jvc_projector_remote_improved2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7296 2023-07-02 17:16:07.000000 jvc_projector_remote_improved2-3.7.2/jvc_projector_remote_improved2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-02 17:16:07.000000 jvc_projector_remote_improved2-3.7.2/jvc_projector_remote_improved2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 17:16:07.000000 jvc_projector_remote_improved2-3.7.2/jvc_projector_remote_improved2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-02 17:16:07.000000 jvc_projector_remote_improved2-3.7.2/jvc_projector_remote_improved2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 17:16:07.930833 jvc_projector_remote_improved2-3.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-02 17:15:56.000000 jvc_projector_remote_improved2-3.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:16:07.930833 jvc_projector_remote_improved2-3.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 17:15:56.000000 jvc_projector_remote_improved2-3.7.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-02 17:15:56.000000 jvc_projector_remote_improved2-3.7.2/tests/testLowLatency.py
```

### Comparing `jvc_projector_remote_improved2-3.7.0/LICENSE` & `jvc_projector_remote_improved2-3.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jvc_projector_remote_improved2-3.7.0/PKG-INFO` & `jvc_projector_remote_improved2-3.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jvc_projector_remote_improved2
-Version: 3.7.0
+Version: 3.7.2
 Summary: A package to control JVC projectors over IP
 Home-page: https://github.com/iloveicedgreentea/jvc_projector_improved
 Author: iloveicedgreentea
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `jvc_projector_remote_improved2-3.7.0/README.md` & `jvc_projector_remote_improved2-3.7.2/README.md`

 * *Files identical despite different names*

### Comparing `jvc_projector_remote_improved2-3.7.0/jvc_projector/commands.py` & `jvc_projector_remote_improved2-3.7.2/jvc_projector/commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,14 +83,22 @@
     hdr_plus = b"15"
     hdr10_plus = b"15"
     pana_pq = b"16"
     filmmaker = b"17"  # requires firmware 2.0
     frame_adapt_hdr2 = b"18"  # requires firmware 2.0
     frame_adapt_hdr3 = b"19"  # requires firmware 2.0
 
+class PictureModes3D(Enum):
+    natural = b"1"
+    user1 = b"2"
+    user2 = b"3"
+    user3 = b"4"
+    cinema = b"8"
+    film = b"9"
+    last = b"F"
 
 class InstallationModes(Enum):
     mode1 = b"0"
     mode2 = b"1"
     mode3 = b"2"
     mode4 = b"3"
     mode5 = b"4"
@@ -161,15 +169,15 @@
 class LaserDimModes(Enum):
     off = b"0"
     auto1 = b"1"
     auto2 = b"2"
     auto3 = b"3"  # requires firmware 2.0
 
 
-class EnhanceModes(Enum):
+class Numeric(Enum):
     """
     JVC numeric values are the byte values of two complemented hex
     """
 
     zero = b"0000"
     one = b"0001"
     two = b"0002"
@@ -273,14 +281,19 @@
 
 
 class SourceStatuses(Enum):
     logo = b"\x00"
     no_signal = b"0"
     signal = b"1"
 
+class ThreeD(Enum):
+    twoD = b"0"
+    auto = b"1"
+    sbs = b"3"
+    tb = b"4"
 
 class Commands(Enum):
 
     # these use ! unless otherwise indicated
     # power commands
     power = b"PW", PowerModes, ACKs.power_ack
 
@@ -329,15 +342,15 @@
 
     # input_level like 0-255
     input_level = b"ISIL", InputLevel, ACKs.hdmi_ack
 
     # low latency enable/disable
     low_latency = b"PMLL", LowLatencyModes, ACKs.picture_ack
     # enhance
-    enhance = b"PMEN", EnhanceModes, ACKs.picture_ack
+    enhance = b"PMEN", Numeric, ACKs.picture_ack
     # motion enhance
     motion_enhance = b"PMME", MotionEnhanceModes, ACKs.picture_ack
     # graphic mode
     graphic_mode = b"PMGM", GraphicModeModes, ACKs.picture_ack
 
     # mask commands
     mask = b"ISMA", MaskModes, ACKs.hdmi_ack
@@ -364,8 +377,21 @@
     # I don't use this, untested
     anamorphic = b"INVS", AnamorphicModes, ACKs.lens_ack
 
     # e-shift
     eshift_mode = b"PMUS", EshiftModes, ACKs.picture_ack
 
     # source status
-    source_status = b"SC", SourceStatuses, ACKs.source_ack
+    source_status = b"SC", SourceStatuses, ACKs.source_ack
+
+    # 3d
+    signal_3d = b"IS3D", ThreeD, ACKs.hdmi_ack
+    # hdmi phase alignment
+    signal_3d_phase = b"IS3P", Numeric, ACKs.hdmi_ack
+    # 3d parallax (-8 to 8)
+    signal_3d_parallax = b"ISLV", Numeric, ACKs.hdmi_ack
+    # 3d crosstalk cancel (-8 to 8)
+    signal_3d_crosstalk = b"ISCA", Numeric, ACKs.hdmi_ack
+    # 3d pm
+    signal_3d_pm = b"ISS3", PictureModes3D, ACKs.hdmi_ack
+    # 2d signal
+    signal_2d_pm = b"ISS2", PictureModes3D, ACKs.hdmi_ack
```

### Comparing `jvc_projector_remote_improved2-3.7.0/jvc_projector/jvc_projector.py` & `jvc_projector_remote_improved2-3.7.2/jvc_projector/jvc_projector.py`

 * *Files identical despite different names*

### Comparing `jvc_projector_remote_improved2-3.7.0/jvc_projector_remote_improved2.egg-info/PKG-INFO` & `jvc_projector_remote_improved2-3.7.2/jvc_projector_remote_improved2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jvc-projector-remote-improved2
-Version: 3.7.0
+Version: 3.7.2
 Summary: A package to control JVC projectors over IP
 Home-page: https://github.com/iloveicedgreentea/jvc_projector_improved
 Author: iloveicedgreentea
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `jvc_projector_remote_improved2-3.7.0/setup.py` & `jvc_projector_remote_improved2-3.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="jvc_projector_remote_improved2",
-    version="3.7.0",
+    version="3.7.2",
     author="iloveicedgreentea",
     description="A package to control JVC projectors over IP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iloveicedgreentea/jvc_projector_improved",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `jvc_projector_remote_improved2-3.7.0/tests/testLowLatency.py` & `jvc_projector_remote_improved2-3.7.2/tests/testLowLatency.py`

 * *Files identical despite different names*

