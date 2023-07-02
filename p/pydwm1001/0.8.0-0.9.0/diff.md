# Comparing `tmp/pydwm1001-0.8.0.tar.gz` & `tmp/pydwm1001-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydwm1001-0.8.0.tar", last modified: Sat Jul  1 01:26:25 2023, max compression
+gzip compressed data, was "pydwm1001-0.9.0.tar", last modified: Sat Jul  1 19:03:38 2023, max compression
```

## Comparing `pydwm1001-0.8.0.tar` & `pydwm1001-0.9.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-01 01:26:25.701798 pydwm1001-0.8.0/
--rw-r--r--   0 adam       (501) staff       (20)     1111 2023-06-21 00:05:54.000000 pydwm1001-0.8.0/LICENSE
--rw-r--r--   0 adam       (501) staff       (20)      637 2023-07-01 01:26:25.701659 pydwm1001-0.8.0/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)      103 2023-06-21 00:05:43.000000 pydwm1001-0.8.0/README.md
--rw-r--r--   0 adam       (501) staff       (20)     4672 2023-07-01 01:24:35.000000 pydwm1001-0.8.0/dwm1001.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-01 01:26:25.701221 pydwm1001-0.8.0/pydwm1001.egg-info/
--rw-r--r--   0 adam       (501) staff       (20)      637 2023-07-01 01:26:25.000000 pydwm1001-0.8.0/pydwm1001.egg-info/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)      229 2023-07-01 01:26:25.000000 pydwm1001-0.8.0/pydwm1001.egg-info/SOURCES.txt
--rw-r--r--   0 adam       (501) staff       (20)        1 2023-07-01 01:26:25.000000 pydwm1001-0.8.0/pydwm1001.egg-info/dependency_links.txt
--rw-r--r--   0 adam       (501) staff       (20)        9 2023-07-01 01:26:25.000000 pydwm1001-0.8.0/pydwm1001.egg-info/requires.txt
--rw-r--r--   0 adam       (501) staff       (20)        8 2023-07-01 01:26:25.000000 pydwm1001-0.8.0/pydwm1001.egg-info/top_level.txt
--rw-r--r--   0 adam       (501) staff       (20)      640 2023-07-01 01:24:35.000000 pydwm1001-0.8.0/pyproject.toml
--rw-r--r--   0 adam       (501) staff       (20)       38 2023-07-01 01:26:25.701840 pydwm1001-0.8.0/setup.cfg
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-01 01:26:25.701316 pydwm1001-0.8.0/tests/
--rw-r--r--   0 adam       (501) staff       (20)     2788 2023-06-30 00:12:46.000000 pydwm1001-0.8.0/tests/test_dwm1001.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-01 19:03:38.033095 pydwm1001-0.9.0/
+-rw-r--r--   0 adam       (501) staff       (20)     1111 2023-06-21 00:05:54.000000 pydwm1001-0.9.0/LICENSE
+-rw-r--r--   0 adam       (501) staff       (20)      637 2023-07-01 19:03:38.032965 pydwm1001-0.9.0/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)      103 2023-06-21 00:05:43.000000 pydwm1001-0.9.0/README.md
+-rw-r--r--   0 adam       (501) staff       (20)     5058 2023-07-01 19:03:20.000000 pydwm1001-0.9.0/dwm1001.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-01 19:03:38.032542 pydwm1001-0.9.0/pydwm1001.egg-info/
+-rw-r--r--   0 adam       (501) staff       (20)      637 2023-07-01 19:03:38.000000 pydwm1001-0.9.0/pydwm1001.egg-info/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)      229 2023-07-01 19:03:38.000000 pydwm1001-0.9.0/pydwm1001.egg-info/SOURCES.txt
+-rw-r--r--   0 adam       (501) staff       (20)        1 2023-07-01 19:03:38.000000 pydwm1001-0.9.0/pydwm1001.egg-info/dependency_links.txt
+-rw-r--r--   0 adam       (501) staff       (20)        9 2023-07-01 19:03:38.000000 pydwm1001-0.9.0/pydwm1001.egg-info/requires.txt
+-rw-r--r--   0 adam       (501) staff       (20)        8 2023-07-01 19:03:38.000000 pydwm1001-0.9.0/pydwm1001.egg-info/top_level.txt
+-rw-r--r--   0 adam       (501) staff       (20)      640 2023-07-01 19:03:20.000000 pydwm1001-0.9.0/pyproject.toml
+-rw-r--r--   0 adam       (501) staff       (20)       38 2023-07-01 19:03:38.033129 pydwm1001-0.9.0/setup.cfg
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-01 19:03:38.032638 pydwm1001-0.9.0/tests/
+-rw-r--r--   0 adam       (501) staff       (20)     2788 2023-06-30 00:12:46.000000 pydwm1001-0.9.0/tests/test_dwm1001.py
```

### Comparing `pydwm1001-0.8.0/LICENSE` & `pydwm1001-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydwm1001-0.8.0/PKG-INFO` & `pydwm1001-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydwm1001
-Version: 0.8.0
+Version: 0.9.0
 Summary: A Python library for interfacing with DWM1001
 Author-email: Adam Morrissett <morrissettal2@vcu.edu>
 Project-URL: Homepage, https://github.com/the-hive-lab/pydwm1001
 Project-URL: Bug Tracker, https://github.com/the-hive-lab/pydwm1001/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pydwm1001-0.8.0/dwm1001.py` & `pydwm1001-0.9.0/dwm1001.py`

 * *Files 9% similar despite different names*

```diff
@@ -64,32 +64,42 @@
         # We only use the last four characters in the address
         return TagName("DW" + self.tag_id[-4:])
 
     @property
     def tag_id(self) -> TagId:
         self.send_shell_command(ShellCommand.SI)
 
-        response = []
-        for _ in range(9):
-            response.append(self.serial_handle.readline().decode())
+        response = self.get_shell_response().splitlines()
 
         # System info response has several lines, but we only care about the address
-        address_line = response[2]
+        address_line = response[1]
         address_text_start = address_line.find("addr=")
         address_string = address_line[address_text_start:].strip()
 
         return TagId("0" + address_string.removeprefix("addr="))
 
     def send_shell_command(self, command: ShellCommand) -> None:
         self.serial_handle.write(command.value)
         self.serial_handle.write(ShellCommand.ENTER.value)
         self.serial_handle.flush()
 
         time.sleep(self.SHELL_COMMAND_DELAY_PERIOD)
 
+    def get_shell_response(self) -> str:
+        raw_data = self.serial_handle.read_until(b"dwm> ")
+
+        # Raw data includes sent command, followed by a new line. The
+        # response starts after the new line.
+        response_begin = raw_data.find(b"\r\n") + 2
+
+        # Raw data always ends with the shell prompt.
+        response_end = raw_data.rfind(b"dwm> ")
+
+        return raw_data[response_begin:response_end].decode().rstrip()
+
     def reset(self) -> None:
         self.send_shell_command(ShellCommand.RESET)
 
         time.sleep(self.RESET_DELAY_PERIOD)
 
     def enter_shell_mode(self) -> None:
         self.serial_handle.write(ShellCommand.DOUBLE_ENTER.value)
```

### Comparing `pydwm1001-0.8.0/pydwm1001.egg-info/PKG-INFO` & `pydwm1001-0.9.0/pydwm1001.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydwm1001
-Version: 0.8.0
+Version: 0.9.0
 Summary: A Python library for interfacing with DWM1001
 Author-email: Adam Morrissett <morrissettal2@vcu.edu>
 Project-URL: Homepage, https://github.com/the-hive-lab/pydwm1001
 Project-URL: Bug Tracker, https://github.com/the-hive-lab/pydwm1001/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pydwm1001-0.8.0/pyproject.toml` & `pydwm1001-0.9.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pydwm1001"
-version = "0.8.0"
+version = "0.9.0"
 authors = [
   { name="Adam Morrissett", email="morrissettal2@vcu.edu" },
 ]
 description = "A Python library for interfacing with DWM1001"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pydwm1001-0.8.0/tests/test_dwm1001.py` & `pydwm1001-0.9.0/tests/test_dwm1001.py`

 * *Files identical despite different names*

