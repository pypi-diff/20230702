# Comparing `tmp/py_madvr-1.4.5.tar.gz` & `tmp/py_madvr-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_madvr-1.4.5.tar", last modified: Fri Jun 30 16:46:15 2023, max compression
+gzip compressed data, was "py_madvr-1.4.6.tar", last modified: Sun Jul  2 15:36:28 2023, max compression
```

## Comparing `py_madvr-1.4.5.tar` & `py_madvr-1.4.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:46:15.149544 py_madvr-1.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-30 16:46:01.000000 py_madvr-1.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-30 16:46:15.149544 py_madvr-1.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-30 16:46:01.000000 py_madvr-1.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:46:15.149544 py_madvr-1.4.5/madvr/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-30 16:46:01.000000 py_madvr-1.4.5/madvr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-06-30 16:46:01.000000 py_madvr-1.4.5/madvr/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-30 16:46:01.000000 py_madvr-1.4.5/madvr/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    16746 2023-06-30 16:46:01.000000 py_madvr-1.4.5/madvr/madvr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:46:15.149544 py_madvr-1.4.5/py_madvr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-30 16:46:15.000000 py_madvr-1.4.5/py_madvr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-30 16:46:15.000000 py_madvr-1.4.5/py_madvr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 16:46:15.000000 py_madvr-1.4.5/py_madvr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-30 16:46:15.000000 py_madvr-1.4.5/py_madvr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 16:46:15.149544 py_madvr-1.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-30 16:46:01.000000 py_madvr-1.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:46:15.149544 py_madvr-1.4.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:46:01.000000 py_madvr-1.4.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-30 16:46:01.000000 py_madvr-1.4.5/tests/testMadVR.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:36:28.052605 py_madvr-1.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-02 15:36:09.000000 py_madvr-1.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-02 15:36:28.052605 py_madvr-1.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-02 15:36:09.000000 py_madvr-1.4.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:36:28.052605 py_madvr-1.4.6/madvr/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-02 15:36:09.000000 py_madvr-1.4.6/madvr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-02 15:36:09.000000 py_madvr-1.4.6/madvr/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-02 15:36:09.000000 py_madvr-1.4.6/madvr/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17415 2023-07-02 15:36:09.000000 py_madvr-1.4.6/madvr/madvr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:36:28.052605 py_madvr-1.4.6/py_madvr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-02 15:36:28.000000 py_madvr-1.4.6/py_madvr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-02 15:36:28.000000 py_madvr-1.4.6/py_madvr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 15:36:28.000000 py_madvr-1.4.6/py_madvr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-02 15:36:28.000000 py_madvr-1.4.6/py_madvr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 15:36:28.052605 py_madvr-1.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-02 15:36:09.000000 py_madvr-1.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:36:28.052605 py_madvr-1.4.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 15:36:09.000000 py_madvr-1.4.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-02 15:36:09.000000 py_madvr-1.4.6/tests/testMadVR.py
```

### Comparing `py_madvr-1.4.5/LICENSE` & `py_madvr-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `py_madvr-1.4.5/PKG-INFO` & `py_madvr-1.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_madvr
-Version: 1.4.5
+Version: 1.4.6
 Summary: A package to control MadVR Envy over IP
 Home-page: https://github.com/iloveicedgreentea/py-madvr
 Author: iloveicedgreentea
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `py_madvr-1.4.5/madvr/commands.py` & `py_madvr-1.4.6/madvr/commands.py`

 * *Files 25% similar despite different names*

```diff
@@ -65,68 +65,62 @@
 
 class DisplayAlert(Enum):
     pass
 
 class Information(Enum):
     pass
 
-class Profiles(Enum):
-    pass
-
 class SettingsPages(Enum):
     pass
 
 class Toggle(Enum):
     pass
 
 class SingleCmd(Enum):
     """for things that are single words"""
 
 class IsInformational(Enum):
     true = True
     false = False
 
+class Menus(Enum):
+    Info = b"Info"
+    Settings = b"Settings"
+    Configuration = b"Configuration"
+    Profiles = b"Profiles"
+    TestPatterns = b"TestPatterns" 
+
+class Profiles(Enum):
+    SOURCE = b"SOURCE"
+    DISPLAY = b"DISPLAY"
+
 class Commands(Enum):
     # Power stuff
     PowerOff = b"PowerOff", SingleCmd, IsInformational.false
     Standby = b"Standby", SingleCmd, IsInformational.false
     Restart = b"Restart", SingleCmd, IsInformational.false
     ReloadSoftware = b"ReloadSoftware", SingleCmd, IsInformational.false
     Bye = b"Bye", SingleCmd, IsInformational.false
+    ResetTemporary = b"ResetTemporary", SingleCmd, IsInformational.false
 
-    #  vb'KeyPress MENU\r\n'
-# b'CloseMenu\r\n'
-# b'OK\r\nIncomingSignalInfo 3840x2160 59.940p 2D 420 10bit SDR 709 TV 16:9\r\nReloadSoftware\r\nOutgoingSignalInfo 4096x2160 59.940p 2D RGB 8bit SDR 709 TV\r\nIncomingSignalInfo 3840x2160 59.940p 2D 420 10bit SDR 709 TV 16:9\r\nAspectRatio 3840:2160 1.778 178 "16:9"\r\nMaskingRatio 3044:1712 1.778 178\r\nKeyPress MENU\r\nOpenMenu Configuration\r\n'
-    # playing fast n furous 
-    # b'OK\r\nAspectRatio 3816:2146 1.778 178 "16:9"\r\nResetTemporary\r\nNoSignal\r\nOutgoingSignalInfo 4096x2160 59.940p 2D RGB 8bit SDR 709 TV\r\nIncomingSignalInfo 1280x720 59.940p 2D 422 12bit SDR 709 TV 16:9\r\nAspectRatio 1280:0720 1.778 178 "16:9"\r\nAspectRatio 1272:0525 2.423 240 "Panavision"\r\nMaskingRatio 4092:1689 2.423 240\r\n'
+    ActivateProfile = b"ActivateProfile", Profiles, IsInformational.false
 
     # Menu
-    OpenMenu = b"OpenMenu", SingleCmd, IsInformational.false
+    OpenMenu = b"OpenMenu", Menus, IsInformational.false
     CloseMenu = b"CloseMenu", SingleCmd, IsInformational.false
     KeyPress = b"KeyPress", KeyPress, IsInformational.false
     KeyHold = b"KeyHold", KeyPress, IsInformational.false
-    
-    # display_alert = b"DisplayAlertWindow", ACKs.reply
-    # close_alert = b"CloseAlertWindow", ACKs.reply
-    # display_message = b"DisplayMessage", ACKs.reply
 
     GetIncomingSignalInfo = b"GetIncomingSignalInfo", SignalInfo, IsInformational.true
     GetOutgoingSignalInfo = b"GetOutgoingSignalInfo", OutgoingSignalInfo, IsInformational.true
     GetAspectRatio = b"GetAspectRatio", AspectRatio, IsInformational.true
     GetMaskingRatio = b"GetMaskingRatio", SingleCmd, IsInformational.true
     GetTemperatures = b"GetTemperatures", Temperatures, IsInformational.true
     GetMacAddress = b"GetMacAddress", SingleCmd, IsInformational.true
 
-    # enum_settings = b"EnumSettingsPages"
-    # enum_configs = b"EnumConfigPages"
-    # enum_options = b"EnumOptions"
-    # query_option = b"QueryOption"
-    # change_option = b"ChangeOption"
-    # reset_temp = b"ResetTemporary"
-
     # toggle = b"Toggle"
     ToneMapOn = b"ToneMapOn", SingleCmd, IsInformational.false
     ToneMapOff = b"ToneMapOff", SingleCmd, IsInformational.false
 
     Hotplug = b"Hotplug", SingleCmd, IsInformational.false
     RefreshLicenseInfo = b"RefreshLicenseInfo", SingleCmd, IsInformational.false
     Force1080p60Output = b"Force1080p60Output", SingleCmd, IsInformational.false
```

### Comparing `py_madvr-1.4.5/madvr/madvr.py` & `py_madvr-1.4.6/madvr/madvr.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,55 +219,71 @@
             "raw_command: %s -- raw_command length: %s", raw_command, len(raw_command)
         )
 
         skip_val = False
         # HA seems to always send commands as a list even if you set them as a str
 
         # This lets you use single cmds or something with val like KEYPRESS
-        # If len is 1 like ["keypress,val"], then try to split, otherwise its just one word
 
-        if len(raw_command) == 1:
+        # If len is 1 like ["keypress,val"], then try to split, otherwise its just one word
+        # sent directly from HA send_command
+        if len(raw_command) == 1:  # if its a list
             try:
-                # ['key_press, menu']
-                command, raw_value = raw_command[0].split(",")
+                # ['key_press, menu'] -> 'key_press', ['menu']
+                # ['activate_profile, SOURCE, 1'] -> 'activate_profile', ['SOURCE', '1']
+                command, *raw_value = raw_command[0].split(",")
                 # remove space
-                value = raw_value.strip()
-                self.logger.debug("using command %s and value %s", command, value)
+                values = [val.strip() for val in raw_value]
+                self.logger.debug("using command %s and values %s", command, values)
             # if valuerror it means theres just one command like PowerOff, so use that directly
             except ValueError as err:
                 self.logger.debug(err)
                 self.logger.debug("Using raw_command directly")
                 command = raw_command[0]
                 skip_val = True
-        # if there are more than two values, this is incorrect, error
-        elif len(raw_command) > 2:
+        # if there are more than three values, this is incorrect, error
+        elif len(raw_command) > 3:
             self.logger.error(
-                "More than two command values provided. Envy does not have more than 2 command values e.g KeyPress MENU"
+                "More than three command values provided."
             )
             raise NotImplementedError(f"Too many values provided {raw_command}")
         else:
+            self.logger.debug("command is a list")
             # else a command was provided as a proper list ['keypress', 'menu']
-            # raw command will be a list of 2
-            command, value = raw_command
+            # raw command will be a list of 2+
+            command, *values = raw_command
 
         self.logger.debug("checking command %s", command)
 
         # Check if command is implemented
         if not hasattr(Commands, command):
             raise NotImplementedError(f"Command not implemented: {command}")
         self.logger.debug("Found command")
         # construct the command with nested Enums
         command_name, val, _ = Commands[command].value
 
         # if there is a value to process
         if not skip_val:
             try:
-                command_base: bytes = command_name + b" " + val[value.lstrip(" ")].value
+                # add the base command
+                command_base: bytes = command_name
+
+                # append each value with a space
+                for value in values:
+                    # if value is a number, use it directly
+                    # TODO: check this?
+                    if value.isnumeric(): # encode 1 for ActivateProfile
+                        command_base += b" " + value.encode("utf-8")
+                    else:
+                        # else use the enum
+                        command_base += b" " + val[value.lstrip(" ")].value
+
                 # Construct command based on required values
                 cmd: bytes = command_base + Footer.footer.value
+
             except KeyError as exc:
                 raise NotImplementedError(
                     "Incorrect parameter given for command"
                 ) from exc
         else:
             cmd: bytes = command_name + Footer.footer.value
```

### Comparing `py_madvr-1.4.5/py_madvr.egg-info/PKG-INFO` & `py_madvr-1.4.6/py_madvr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-madvr
-Version: 1.4.5
+Version: 1.4.6
 Summary: A package to control MadVR Envy over IP
 Home-page: https://github.com/iloveicedgreentea/py-madvr
 Author: iloveicedgreentea
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `py_madvr-1.4.5/setup.py` & `py_madvr-1.4.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="py_madvr",
-    version="1.4.5",
+    version="1.4.6",
     author="iloveicedgreentea",
     description="A package to control MadVR Envy over IP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iloveicedgreentea/py-madvr",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `py_madvr-1.4.5/tests/testMadVR.py` & `py_madvr-1.4.6/tests/testMadVR.py`

 * *Files identical despite different names*

