# Comparing `tmp/pyhubio-1.2.tar.gz` & `tmp/pyhubio-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhubio-1.2.tar", last modified: Thu Mar 16 06:45:56 2023, max compression
+gzip compressed data, was "pyhubio-1.3.tar", last modified: Sun Jul  2 20:00:27 2023, max compression
```

## Comparing `pyhubio-1.2.tar` & `pyhubio-1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 demin     (1000) demin     (1000)        0 2023-03-16 06:45:56.500269 pyhubio-1.2/
--rw-r--r--   0 demin     (1000) demin     (1000)     1078 2023-02-27 17:18:34.000000 pyhubio-1.2/LICENSE
--rw-r--r--   0 demin     (1000) demin     (1000)      720 2023-03-16 06:45:56.500269 pyhubio-1.2/PKG-INFO
--rw-r--r--   0 demin     (1000) demin     (1000)      404 2023-03-16 06:38:13.000000 pyhubio-1.2/README.md
-drwxr-xr-x   0 demin     (1000) demin     (1000)        0 2023-03-16 06:45:56.500269 pyhubio-1.2/pyhubio/
--rw-r--r--   0 demin     (1000) demin     (1000)     8094 2023-03-14 14:17:42.000000 pyhubio-1.2/pyhubio/__init__.py
-drwxr-xr-x   0 demin     (1000) demin     (1000)        0 2023-03-16 06:45:56.500269 pyhubio-1.2/pyhubio.egg-info/
--rw-r--r--   0 demin     (1000) demin     (1000)      720 2023-03-16 06:45:56.000000 pyhubio-1.2/pyhubio.egg-info/PKG-INFO
--rw-r--r--   0 demin     (1000) demin     (1000)      206 2023-03-16 06:45:56.000000 pyhubio-1.2/pyhubio.egg-info/SOURCES.txt
--rw-r--r--   0 demin     (1000) demin     (1000)        1 2023-03-16 06:45:56.000000 pyhubio-1.2/pyhubio.egg-info/dependency_links.txt
--rw-r--r--   0 demin     (1000) demin     (1000)       14 2023-03-16 06:45:56.000000 pyhubio-1.2/pyhubio.egg-info/requires.txt
--rw-r--r--   0 demin     (1000) demin     (1000)        8 2023-03-16 06:45:56.000000 pyhubio-1.2/pyhubio.egg-info/top_level.txt
--rw-r--r--   0 demin     (1000) demin     (1000)      436 2023-03-16 06:44:38.000000 pyhubio-1.2/pyproject.toml
--rw-r--r--   0 demin     (1000) demin     (1000)       38 2023-03-16 06:45:56.500269 pyhubio-1.2/setup.cfg
+drwxr-xr-x   0 demin     (1000) demin     (1000)        0 2023-07-02 20:00:27.520506 pyhubio-1.3/
+-rw-r--r--   0 demin     (1000) demin     (1000)     1078 2023-02-27 17:18:34.000000 pyhubio-1.3/LICENSE
+-rw-r--r--   0 demin     (1000) demin     (1000)     1086 2023-07-02 20:00:27.520506 pyhubio-1.3/PKG-INFO
+-rw-r--r--   0 demin     (1000) demin     (1000)      785 2023-07-02 10:44:33.000000 pyhubio-1.3/README.md
+drwxr-xr-x   0 demin     (1000) demin     (1000)        0 2023-07-02 20:00:27.520506 pyhubio-1.3/pyhubio/
+-rw-r--r--   0 demin     (1000) demin     (1000)    10760 2023-07-02 10:21:52.000000 pyhubio-1.3/pyhubio/__init__.py
+drwxr-xr-x   0 demin     (1000) demin     (1000)        0 2023-07-02 20:00:27.520506 pyhubio-1.3/pyhubio.egg-info/
+-rw-r--r--   0 demin     (1000) demin     (1000)     1086 2023-07-02 20:00:27.000000 pyhubio-1.3/pyhubio.egg-info/PKG-INFO
+-rw-r--r--   0 demin     (1000) demin     (1000)      206 2023-07-02 20:00:27.000000 pyhubio-1.3/pyhubio.egg-info/SOURCES.txt
+-rw-r--r--   0 demin     (1000) demin     (1000)        1 2023-07-02 20:00:27.000000 pyhubio-1.3/pyhubio.egg-info/dependency_links.txt
+-rw-r--r--   0 demin     (1000) demin     (1000)       14 2023-07-02 20:00:27.000000 pyhubio-1.3/pyhubio.egg-info/requires.txt
+-rw-r--r--   0 demin     (1000) demin     (1000)        8 2023-07-02 20:00:27.000000 pyhubio-1.3/pyhubio.egg-info/top_level.txt
+-rw-r--r--   0 demin     (1000) demin     (1000)      421 2023-07-02 18:54:47.000000 pyhubio-1.3/pyproject.toml
+-rw-r--r--   0 demin     (1000) demin     (1000)       38 2023-07-02 20:00:27.520506 pyhubio-1.3/setup.cfg
```

### Comparing `pyhubio-1.2/LICENSE` & `pyhubio-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhubio-1.2/PKG-INFO` & `pyhubio-1.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 Metadata-Version: 2.1
 Name: pyhubio
-Version: 1.2
-Summary: A small library to communicate with the applications for the USB104 A7 board
+Version: 1.3
+Summary: A small library to communicate with AXI4 and AXI4-Stream hubs
 Author: Pavel Demin
 License: MIT
 Project-URL: Homepage, https://github.com/pavel-demin/pyhubio
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-This library uses [python-libusb1](https://github.com/vpelletier/python-libusb1) to communicate with configuration registers, status registers, AXI4-Stream and BRAM ports via AXI4-Stream USB and AXI4-Stream hub modules:
+This library is used to communicate with configuration registers, status registers, AXI4-Stream and BRAM interfaces on Digilent USB104 A7 and Red Pitaya STEMlab boards:
+
+https://pavel-demin.github.io/usb104-a7-notes
+
+https://pavel-demin.github.io/red-pitaya-notes
+
+This library uses the [python-libusb1](https://github.com/vpelletier/python-libusb1) library to communicate via the USB interface with the AXI4-Stream USB and AXI4-Stream hub modules on the Digilent USB104 A7 board:
 
 https://pavel-demin.github.io/usb104-a7-notes/usb-interface
 
-This library is mainly used with the applications for the USB104 A7 board:
+This library uses the [socket](https://docs.python.org/3/library/socket.html) library to communicate via the Ethernet interface with the AXI4 hub module on the Red Pitaya STEMlab board:
 
-https://pavel-demin.github.io/usb104-a7-notes
+https://pavel-demin.github.io/red-pitaya-notes/axi-hub
```

### Comparing `pyhubio-1.2/pyhubio/__init__.py` & `pyhubio-1.3/pyhubio/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import usb1
+import socket
 import numpy as np
 import time
 
 
 class PyhubIO:
     def __init__(self, vid=0x0403, pid=0x6014):
         self.id = (vid, pid)
@@ -240,7 +241,84 @@
     def program(self, path):
         self.start()
         self.flush()
         self.setup()
         self.idle()
         self.configure(path)
         self.stop()
+
+
+class PyhubTCP:
+    def __init__(self, host="192.168.1.100", port=1001):
+        self.address = (host, port)
+        self.socket = None
+
+    def start(self):
+        if self.socket:
+            return
+        self.socket = socket.create_connection(self.address, 1)
+
+    def stop(self):
+        if self.socket is None:
+            return
+        self.socket.close()
+        self.socket = None
+
+    def read(self, data, port=1, addr=0):
+        if self.socket is None:
+            return
+        view = data.view(np.uint8)
+        for part in np.split(view, np.arange(16777216, view.size, 16777216)):
+            view = part.view(np.uint8)
+            size = part.size
+            incr = np.arange(0, size, 65536, np.uint64)
+            rlen = np.full_like(incr, 65536)
+            mod = size % 65536
+            if mod > 0:
+                rlen[-1] = mod
+            command = rlen << 28 | (port & 0x7) << 24 | (addr + incr) & 0xFFFFFF
+            self.socket.sendall(command.tobytes())
+            offset = 0
+            limit = view.size
+            while offset < limit:
+                buffer = self.socket.recv(limit - offset)
+                buffer = np.frombuffer(buffer, np.uint8)
+                size = buffer.size
+                view[offset : offset + size] = buffer
+                offset += size
+            addr += part.size
+
+    def write(self, data, port=0, addr=0):
+        if self.socket is None:
+            return
+        view = data.view(np.uint8)
+        for part in np.split(view, np.arange(65536, view.size, 65536)):
+            size = part.size
+            command = np.uint64([1 << 52 | size << 28 | (port & 0x7) << 24 | addr & 0xFFFFFF])
+            addr += part.size
+            self.socket.sendall(command.tobytes())
+            self.socket.sendall(part.tobytes())
+
+    def edge(self, data, mask, positive=True, addr=0):
+        if self.socket is None:
+            return data
+        command = np.uint64([1 << 52 | 1 << 28 | addr & 0xFFFFFF])
+        view = command.view(np.uint8)
+        lo = np.uint8([data & ~mask])
+        hi = np.uint8([data | mask])
+        if positive:
+            sequence = np.concatenate((view, lo, view, hi))
+            result = hi
+        else:
+            sequence = np.concatenate((view, hi, view, lo))
+            result = lo
+        self.socket.sendall(sequence.tobytes())
+        return result
+
+    def program(self, path):
+        if self.socket is None:
+            return
+        data = np.fromfile(path, np.uint8)
+        size = data.size
+        command = np.uint64([2 << 52 | size << 28])
+        self.socket.sendall(command.tobytes())
+        self.socket.sendall(data.tobytes())
```

### Comparing `pyhubio-1.2/pyhubio.egg-info/PKG-INFO` & `pyhubio-1.3/pyhubio.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 Metadata-Version: 2.1
 Name: pyhubio
-Version: 1.2
-Summary: A small library to communicate with the applications for the USB104 A7 board
+Version: 1.3
+Summary: A small library to communicate with AXI4 and AXI4-Stream hubs
 Author: Pavel Demin
 License: MIT
 Project-URL: Homepage, https://github.com/pavel-demin/pyhubio
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-This library uses [python-libusb1](https://github.com/vpelletier/python-libusb1) to communicate with configuration registers, status registers, AXI4-Stream and BRAM ports via AXI4-Stream USB and AXI4-Stream hub modules:
+This library is used to communicate with configuration registers, status registers, AXI4-Stream and BRAM interfaces on Digilent USB104 A7 and Red Pitaya STEMlab boards:
+
+https://pavel-demin.github.io/usb104-a7-notes
+
+https://pavel-demin.github.io/red-pitaya-notes
+
+This library uses the [python-libusb1](https://github.com/vpelletier/python-libusb1) library to communicate via the USB interface with the AXI4-Stream USB and AXI4-Stream hub modules on the Digilent USB104 A7 board:
 
 https://pavel-demin.github.io/usb104-a7-notes/usb-interface
 
-This library is mainly used with the applications for the USB104 A7 board:
+This library uses the [socket](https://docs.python.org/3/library/socket.html) library to communicate via the Ethernet interface with the AXI4 hub module on the Red Pitaya STEMlab board:
 
-https://pavel-demin.github.io/usb104-a7-notes
+https://pavel-demin.github.io/red-pitaya-notes/axi-hub
```

