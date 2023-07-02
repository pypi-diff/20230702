# Comparing `tmp/hp_procurvearuba-1.1.0.tar.gz` & `tmp/hp_procurvearuba-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hp_procurvearuba-1.1.0.tar", last modified: Sun May  8 21:18:28 2022, max compression
+gzip compressed data, was "hp_procurvearuba-2.0.0.tar", last modified: Sun Jul  2 19:43:15 2023, max compression
```

## Comparing `hp_procurvearuba-1.1.0.tar` & `hp_procurvearuba-2.0.0.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxrwxr-x   0 brb       (1000) brb       (1000)        0 2022-05-08 21:18:28.576683 hp_procurvearuba-1.1.0/
--rw-rw-r--   0 brb       (1000) brb       (1000)     1067 2021-10-20 14:53:01.000000 hp_procurvearuba-1.1.0/LICENSE
--rw-rw-r--   0 brb       (1000) brb       (1000)     6689 2022-05-08 21:18:28.576683 hp_procurvearuba-1.1.0/PKG-INFO
--rw-rw-r--   0 brb       (1000) brb       (1000)     5997 2021-11-03 10:23:48.000000 hp_procurvearuba-1.1.0/README.md
--rw-rw-r--   0 brb       (1000) brb       (1000)      105 2021-10-20 14:53:01.000000 hp_procurvearuba-1.1.0/pyproject.toml
--rw-rw-r--   0 brb       (1000) brb       (1000)     1596 2022-05-08 21:18:28.580683 hp_procurvearuba-1.1.0/setup.cfg
--rw-rw-r--   0 brb       (1000) brb       (1000)       37 2021-10-20 14:53:01.000000 hp_procurvearuba-1.1.0/setup.py
-drwxrwxr-x   0 brb       (1000) brb       (1000)        0 2022-05-08 21:18:28.572682 hp_procurvearuba-1.1.0/src/
-drwxrwxr-x   0 brb       (1000) brb       (1000)        0 2022-05-08 21:18:28.576683 hp_procurvearuba-1.1.0/src/hp_procurvearuba/
--rw-rw-r--   0 brb       (1000) brb       (1000)       30 2021-10-28 20:41:19.000000 hp_procurvearuba-1.1.0/src/hp_procurvearuba/__init__.py
--rw-rw-r--   0 brb       (1000) brb       (1000)    35692 2022-05-08 20:40:56.000000 hp_procurvearuba-1.1.0/src/hp_procurvearuba/procurvearuba.py
-drwxrwxr-x   0 brb       (1000) brb       (1000)        0 2022-05-08 21:18:28.576683 hp_procurvearuba-1.1.0/src/hp_procurvearuba.egg-info/
--rw-rw-r--   0 brb       (1000) brb       (1000)     6689 2022-05-08 21:18:26.000000 hp_procurvearuba-1.1.0/src/hp_procurvearuba.egg-info/PKG-INFO
--rw-rw-r--   0 brb       (1000) brb       (1000)      341 2022-05-08 21:18:28.000000 hp_procurvearuba-1.1.0/src/hp_procurvearuba.egg-info/SOURCES.txt
--rw-rw-r--   0 brb       (1000) brb       (1000)        1 2022-05-08 21:18:26.000000 hp_procurvearuba-1.1.0/src/hp_procurvearuba.egg-info/dependency_links.txt
--rw-rw-r--   0 brb       (1000) brb       (1000)      706 2022-05-08 21:18:28.000000 hp_procurvearuba-1.1.0/src/hp_procurvearuba.egg-info/requires.txt
--rw-rw-r--   0 brb       (1000) brb       (1000)       17 2022-05-08 21:18:28.000000 hp_procurvearuba-1.1.0/src/hp_procurvearuba.egg-info/top_level.txt
+drwxrwxr-x   0 brb       (1000) brb       (1000)        0 2023-07-02 19:43:15.239742 hp_procurvearuba-2.0.0/
+-rw-rw-r--   0 brb       (1000) brb       (1000)     1067 2021-10-20 14:53:01.000000 hp_procurvearuba-2.0.0/LICENSE
+-rw-rw-r--   0 brb       (1000) brb       (1000)     6504 2023-07-02 19:43:15.239742 hp_procurvearuba-2.0.0/PKG-INFO
+-rw-rw-r--   0 brb       (1000) brb       (1000)     5997 2021-11-03 10:23:48.000000 hp_procurvearuba-2.0.0/README.md
+-rw-rw-r--   0 brb       (1000) brb       (1000)      105 2021-10-20 14:53:01.000000 hp_procurvearuba-2.0.0/pyproject.toml
+-rw-rw-r--   0 brb       (1000) brb       (1000)     1873 2023-07-02 19:43:15.247742 hp_procurvearuba-2.0.0/setup.cfg
+-rw-rw-r--   0 brb       (1000) brb       (1000)       37 2021-10-20 14:53:01.000000 hp_procurvearuba-2.0.0/setup.py
+drwxrwxr-x   0 brb       (1000) brb       (1000)        0 2023-07-02 19:43:15.183741 hp_procurvearuba-2.0.0/src/
+drwxrwxr-x   0 brb       (1000) brb       (1000)        0 2023-07-02 19:43:15.187741 hp_procurvearuba-2.0.0/src/hp_procurvearuba/
+-rw-rw-r--   0 brb       (1000) brb       (1000)       30 2021-10-28 20:41:19.000000 hp_procurvearuba-2.0.0/src/hp_procurvearuba/__init__.py
+-rw-rw-r--   0 brb       (1000) brb       (1000)    35342 2023-07-01 18:29:33.000000 hp_procurvearuba-2.0.0/src/hp_procurvearuba/procurvearuba.py
+drwxrwxr-x   0 brb       (1000) brb       (1000)        0 2023-07-02 19:43:15.191741 hp_procurvearuba-2.0.0/src/hp_procurvearuba.egg-info/
+-rw-rw-r--   0 brb       (1000) brb       (1000)     6504 2023-07-02 19:43:15.000000 hp_procurvearuba-2.0.0/src/hp_procurvearuba.egg-info/PKG-INFO
+-rw-rw-r--   0 brb       (1000) brb       (1000)      381 2023-07-02 19:43:15.000000 hp_procurvearuba-2.0.0/src/hp_procurvearuba.egg-info/SOURCES.txt
+-rw-rw-r--   0 brb       (1000) brb       (1000)        1 2023-07-02 19:43:15.000000 hp_procurvearuba-2.0.0/src/hp_procurvearuba.egg-info/dependency_links.txt
+-rw-rw-r--   0 brb       (1000) brb       (1000)     1076 2023-07-02 19:43:15.000000 hp_procurvearuba-2.0.0/src/hp_procurvearuba.egg-info/requires.txt
+-rw-rw-r--   0 brb       (1000) brb       (1000)       17 2023-07-02 19:43:15.000000 hp_procurvearuba-2.0.0/src/hp_procurvearuba.egg-info/top_level.txt
+drwxrwxr-x   0 brb       (1000) brb       (1000)        0 2023-07-02 19:43:15.231742 hp_procurvearuba-2.0.0/tests/
+-rw-rw-r--   0 brb       (1000) brb       (1000)     9663 2022-05-08 20:40:56.000000 hp_procurvearuba-2.0.0/tests/test_funcs.py
+-rw-r--r--   0 brb       (1000) brb       (1000)     1051 2021-10-20 14:53:01.000000 hp_procurvearuba-2.0.0/tests/test_mocks.py
```

### Comparing `hp_procurvearuba-1.1.0/LICENSE` & `hp_procurvearuba-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hp_procurvearuba-1.1.0/PKG-INFO` & `hp_procurvearuba-2.0.0/src/hp_procurvearuba.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 Metadata-Version: 2.1
-Name: hp_procurvearuba
-Version: 1.1.0
+Name: hp-procurvearuba
+Version: 2.0.0
 Summary: Provides a class with custom functions for easy management of hp procurve and aruba switches
 Home-page: https://github.com/adraf82/hp_procurvearuba
 Author: Adeel Rauf
 Author-email: adraf2000@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div id="top"></div>
@@ -192,9 +187,7 @@
 
 <!-- MARKDOWN LINKS & IMAGES -->
 <!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
 [black-shield]:https://img.shields.io/badge/code%20style-black-000000.svg
 [black-url]:https://github.com/ambv/black
 [python-shield]:https://img.shields.io/pypi/v/hp_procurvearuba
 [python-url]:https://pypi.org/project/hp-procurvearuba
-
-
```

#### html2text {}

```diff
@@ -1,17 +1,14 @@
-Metadata-Version: 2.1 Name: hp_procurvearuba Version: 1.1.0 Summary: Provides a
+Metadata-Version: 2.1 Name: hp-procurvearuba Version: 2.0.0 Summary: Provides a
 class with custom functions for easy management of hp procurve and aruba
 switches Home-page: https://github.com/adraf82/hp_procurvearuba Author: Adeel
-Rauf Author-email: adraf2000@gmail.com License: UNKNOWN Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
-LICENSE
+Rauf Author-email: adraf2000@gmail.com Classifier: License :: OSI Approved ::
+MIT License Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Requires-Python: >=3.6 Description-
+Content-Type: text/markdown License-File: LICENSE
 [![Code style][black-shield]][black-url] [![PyPI][python-shield]][python-url]
                                     [Logo]
                           **** hp_procurvearuba ****
             For easy management of hp procurve and aruba switches
                              Explore_the_docs_Â»
 
                          Report_Bug Â· Request_Feature
```

### Comparing `hp_procurvearuba-1.1.0/README.md` & `hp_procurvearuba-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `hp_procurvearuba-1.1.0/setup.cfg` & `hp_procurvearuba-2.0.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,72 +1,91 @@
 [metadata]
 name = hp_procurvearuba
-version = 1.1.0
+version = 2.0.0
 author = Adeel Rauf
 author_email = adraf2000@gmail.com
 description = Provides a class with custom functions for easy management of hp procurve and aruba switches
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/adraf82/hp_procurvearuba
 classifiers = 
 	License :: OSI Approved :: MIT License
-	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.6
 install_requires = 
 	appdirs==1.4.4
 	attrs==20.3.0
 	bcrypt==3.2.0
-	black==20.8b1
+	black==21.10b0
+	bleach==5.0.0
+	build==0.7.0
+	certifi==2021.10.8
 	cffi==1.14.4
+	charset-normalizer==2.0.12
 	click==7.1.2
+	commonmark==0.9.1
 	cryptography==3.3.1
+	docutils==0.18.1
 	forwardable==0.4.1
 	future==0.18.2
-	importlib-metadata==3.3.0
+	idna==3.3
+	importlib-metadata==3.6.0
 	importlib-resources==3.3.0
 	iniconfig==1.1.1
+	jeepney==0.8.0
+	keyring==23.5.0
 	mccabe==0.6.1
 	mock==4.0.3
 	mypy-extensions==0.4.3
-	netmiko==3.4.0
-	ntc-templates==1.6.0
+	netmiko==4.1.2
+	ntc-templates==3.0.0
 	packaging==20.8
 	paramiko==2.7.2
-	pathspec==0.8.1
+	pathspec==0.9.0
+	pep517==0.12.0
+	pkginfo==1.8.2
 	pluggy==0.13.1
 	py==1.10.0
 	pycodestyle==2.6.0
 	pycparser==2.20
 	pydocstyle==6.1.1
 	pyflakes==2.3.1
+	Pygments==2.12.0
 	pylama==7.7.1
 	PyNaCl==1.4.0
 	pyparsing==2.4.7
 	pyserial==3.5
 	pytest==6.2.0
 	pytest-mock==3.5.1
 	PyYAML==5.3.1
+	readme-renderer==35.0
 	regex==2020.11.13
+	requests==2.27.1
+	requests-toolbelt==0.9.1
+	rfc3986==2.0.0
+	rich==12.4.1
 	scp==0.13.3
+	SecretStorage==3.3.2
 	six==1.15.0
 	snowballstemmer==2.1.0
 	tenacity==6.2.0
-	textfsm==1.1.0
+	textfsm==1.1.2
 	toml==0.10.2
+	tomli==1.2.3
+	twine==4.0.0
 	typed-ast==1.4.2
-	typing-extensions==3.7.4.3
+	typing-extensions==4.0.0
+	urllib3==1.26.9
+	webencodings==0.5.1
 	zipp==3.4.0
 
 [options.packages.find]
 where = src
 
 [pylama]
 linters = pycodestyle,pyflakes
```

### Comparing `hp_procurvearuba-1.1.0/src/hp_procurvearuba/procurvearuba.py` & `hp_procurvearuba-2.0.0/src/hp_procurvearuba/procurvearuba.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 @forwardable()
 class HP:
     """Class HP provides custom methods to manage HP Procurve and Aruba
     switches"""
 
     def_delegators(
         "HPProcurveSSH",
-        "send_command_timing, send_command, find_prompt, disconnect",
+        "send_multiline_timing, send_command, find_prompt, disconnect",
     )
 
     def __init__(self, hostname, *args, **kwargs):
         """
         Parameters
         ----------
         hostname : str
@@ -41,15 +41,15 @@
 
     def __repr__(self):
         """Displays the device hostname of the HP class object instance"""
         return f"{self.hostname}"
 
     def find_stp_mode(self):
         """Finds the spanning tree mode of the switch"""
-        output = self.send_command_timing("show spanning-tree")
+        output = self.send_command("show spanning-tree")
         print("-" * 20)
         print(f"{'HOSTNAME':^10}{'STP_MODE':^10}")
         print("-" * 20)
         try:
             rpvst = re.search(r"^\s+Mode\s+:\s+(?P<mode>RPVST)", output, flags=re.M)
             print(f"{self.hostname:^10}{rpvst.group('mode'):^10}")
             print("-" * 20)
@@ -78,15 +78,15 @@
                         print("-" * 20)
                     except AttributeError:
                         print(f"{self.hostname:^10}{'CHECK SPANNING TREE IS ENABLED'}")
 
     def find_stp_disabled_switch(self):
         """Finds the switch which has spanning tree disabled."""
         print("-" * 20)
-        output = self.send_command_timing("show spanning-tree")
+        output = self.send_command("show spanning-tree")
         print(f"{'STP_DISABLED_SWITCH':^20}")
         print("-" * 20)
         try:
             if (
                 re.search(
                     r"^\s+STP\s+Enabled\s+(\[No\]\s+:\s+No|:\s+No)", output, flags=re.M
                 ).group(0)
@@ -95,15 +95,15 @@
                 print(f"{self.hostname:^20}")
                 print("-" * 20)
         except AttributeError:
             print("-" * 20)
 
     def find_stp_enabled_switch(self):
         """Finds and displays the switch which has spanning tree enabled."""
-        output = self.send_command_timing("show spanning-tree")
+        output = self.send_command("show spanning-tree")
         print("-" * 20)
         print(f"{'STP_ENABLED_SWITCH':^20}")
         print("-" * 20)
         try:
             if (
                 re.search(
                     r"^\s+STP\s+Enabled\s+(\[No\]\s+:\s+Yes|:\s+Yes)",
@@ -303,22 +303,22 @@
                           Set the multiple_mac_port parameter to True when
                           searching for a mac address which is likely to be
                           found on a port containing multiple mac addresses.
         """
         print("-" * 40)
         print(f"{'HOSTNAME':^10}{'PORT':^10}{'MAC_ADDRESS':^10}{'VLAN':^10}")
         print("-" * 40)
-        output = self.send_command_timing("show mac-address", use_textfsm=True)
+        output = self.send_command("show mac-address", use_textfsm=True)
         for mac in output:
             for m in mac_addresses:
                 if mac["mac"] == m:
                     mac_addr = mac["mac"]
                     ports = mac["port"]
                     vlan = mac["vlan"]
-                    output_2 = self.send_command_timing("show mac-address " + ports)
+                    output_2 = self.send_command("show mac-address " + ports)
                     line_output = output_2.splitlines()
                     if multiple_mac_port:
                         for line in line_output:
                             if mac_addr in line:
                                 print(
                                     f"{self.hostname:^10}{ports:^10}{mac_addr:^10}{vlan:^10}"
                                 )
@@ -339,39 +339,39 @@
         ----------
         vlan : list
              The vlan parameter accepts one or more vlan integer as input to the
              find_vlan function.
         """
         print("-" * 20)
         print(f"{'HOSTNAME':^10}{'VLAN':^10}")
-        output = self.send_command_timing("show vlans", use_textfsm=True)
+        output = self.send_command("show vlans", use_textfsm=True)
         print("-" * 20)
         for v in output:
             for vlan_num in vlan:
                 if v["vlan_id"] == str(vlan_num):
                     print(f"{self.hostname:^10}{v['vlan_id']:^10}")
                     print("-" * 20)
 
     def find_interface_errors(self):
         """Finds and displays transmit or/and receive errors on the interface."""
         print("-" * 40)
         print(f"{'HOSTNAME':^10}{'PORT':^10}{'ERRORS_RX':^10}{'DROPS_TX':^10}")
         print("-" * 40)
-        output = self.send_command_timing("show interfaces", use_textfsm=True)
+        output = self.send_command("show interfaces", use_textfsm=True)
         for errors in output:
             if errors["errors_rx"] > "0" or errors["drops_tx"] > "0":
                 print(
                     f"{self.hostname:^10}{errors['port']:^10}{errors['errors_rx']:^10}"
                     f"{errors['drops_tx']:^10}"
                 )
                 print("-" * 40)
 
     def find_intrusion_alerts(self):
         """Finds and displays port security intrusion alarms on an interface."""
-        output = self.send_command_timing("show interfaces brief", use_textfsm=True)
+        output = self.send_command("show int brief", use_textfsm=True)
         print("-" * 40)
         print(f"{'HOSTNAME':^10}{'PORT':^10}{'INTRUSION':^10}{'STATUS':^10}")
         print("-" * 40)
         for alerts in output:
             if alerts["intrusion_alert"] == "Yes":
                 print(
                     f"{self.hostname:^10}{alerts['port']:^10}{alerts['intrusion_alert']:^10}"
@@ -388,40 +388,42 @@
                        Specify the sftp server IP address
         username : str
                  Specify the username of the sftp server
         password : str
                  Specify the password of the sftp server
         """
         if username and password:
-            output = self.send_command_timing(
+            cmd_list = [
                 "copy startup-config sftp "
                 + username
                 + "@"
                 + sftp_server_ip
                 + " "
                 + str(self.hostname)
                 + "_"
-                + str(date.today())
-            )
-            output += self.send_command_timing(password)
+                + str(date.today()),
+                password,
+            ]
+            output = self.send_multiline_timing(cmd_list)
             if "SFTP download" in output:
                 # if self.find_prompt():
                 print(
                     f"Startup configuration successfully backed up for {self.hostname}"
                 )
         else:
-            output = self.send_command_timing(
+            cmd_list = [
                 "copy startup-config sftp "
                 + sftp_server_ip
                 + " "
                 + str(self.hostname)
                 + "_"
-                + str(date.today())
-            )
-            output += self.send_command_timing("\n")
+                + str(date.today()),
+                "\n",
+            ]
+            output = self.send_multiline_timing(cmd_list)
             if "SFTP download" in output:
                 # if self.find_prompt():
                 print(
                     f"Startup configuration successfully backed up for {self.hostname}"
                 )
 
     def sftp_load_config(self, sftp_server_ip, filename, username=None, password=None):
@@ -435,31 +437,33 @@
                 Specify the filename of the configuration to be loaded
         username : str
                     Specify the username of the sftp server
         password : str
                     Specify the password of the sftp server
         """
         if username and password:
-            output = self.send_command_timing(
+            cmd_list = [
                 "copy sftp startup-config "
                 + username
                 + "@"
                 + sftp_server_ip
                 + " "
-                + filename
-            )
-            output += self.send_command_timing("y")
-            output += self.send_command_timing(password)
+                + filename,
+                "y",
+                password,
+            ]
+            self.send_multiline_timing(cmd_list)
             print("Rebooting ", self.hostname)
         else:
-            output = self.send_command_timing(
-                "copy sftp startup-config " + sftp_server_ip + " " + filename
-            )
-            output += self.send_command_timing("y")
-            output += self.send_command_timing("\n")
+            cmd_list = [
+                "copy sftp startup-config " + sftp_server_ip + " " + filename,
+                "y",
+                "\n",
+            ]
+            self.send_multiline_timing(cmd_list)
             print("Rebooting ", self.hostname)
 
     def sftp_load_firmware(
         self,
         sftp_server_ip,
         filename,
         boot_image,
@@ -481,79 +485,83 @@
                   Specify the username of the sftp server
         password : str
                   Specify the password of the sftp server
         reboot : bool
                Set to True if switch is to be rebooted after firmware has been loaded
         """
         if username and password:
-            output = self.send_command_timing(
+            cmd_list = [
                 "copy sftp flash "
                 + username
                 + "@"
                 + sftp_server_ip
                 + " "
                 + filename
                 + " "
-                + boot_image
-            )
-            output += self.send_command_timing("y")
-            output += self.send_command_timing(password, delay_factor=10)
+                + boot_image,
+                "y",
+                password,
+            ]
+            self.send_multiline_timing(cmd_list)
             print("Firmware loaded for ", self.hostname)
-            if reboot:
-                self.send_command_timing("boot system flash " + boot_image)
-                self.send_command_timing("y")
+            if reboot is True:
+                cmd_list = ["boot system flash " + boot_image, "y"]
+                self.send_multiline_timing(cmd_list)
                 print("Rebooting ", self.hostname)
                 self.disconnect()
         else:
-            output = self.send_command_timing(
-                "copy sftp flash " + sftp_server_ip + " " + filename + " " + boot_image
-            )
-            output += self.send_command_timing("y")
-            output += self.send_command_timing("\n", delay_factor=10)
+            cmd_list = [
+                "copy sftp flash " + sftp_server_ip + " " + filename + " " + boot_image,
+                "y",
+                "\n",
+            ]
+            self.send_multiline_timing(cmd_list)
             print("Firmware loaded for ", self.hostname)
-            if reboot:
-                self.send_command_timing("boot system flash " + boot_image)
-                self.send_command_timing("y")
+            if reboot is True:
+                cmd_list = ["boot system flash " + boot_image, "y"]
+                self.send_multiline_timing(cmd_list)
                 print("Rebooting ", self.hostname)
                 self.disconnect()
 
     def tftp_backup_config(self, tftp_server_ip):
         """Backs up the startup configuration to a tftp server.
 
         Parameters
         ----------
         tftp_server_ip : str
                       Specify the tftp server IP address
         """
-        output = self.send_command_timing(
+        cmd_list = [
             "copy startup-config tftp "
             + tftp_server_ip
             + " "
             + self.hostname
             + "_"
             + str(date.today())
-        )
+        ]
+        output = self.send_multiline_timing(cmd_list)
         if "TFTP download" in output:
             print(f"Startup configuration successfully backed up for {self.hostname}")
 
     def tftp_load_config(self, tftp_server_ip, filename):
         """Loads a startup configuration from an sftp server.
 
         Parameters
         ----------
         tftp_server_ip : str
                          Specify the tftp server IP address
         filename : str
                    Specify the filename of the configuration to be loaded
         """
-        output = self.send_command_timing(
-            "copy tftp startup-config " + tftp_server_ip + " " + filename
-        )
-        output += self.send_command_timing("y")
-        output += self.send_command_timing("\n")
+        cmd_list = [
+            "copy tftp startup-config " + tftp_server_ip + " " + filename,
+            "y",
+            "\n",
+        ]
+        self.send_multiline_timing(cmd_list)
         print("Rebooting ", self.hostname)
 
     def tftp_load_firmware(self, tftp_server_ip, filename, boot_image, reboot=False):
         """Loads the switch firmware from a tftp server.
 
         Parameters
         ----------
@@ -562,23 +570,24 @@
         filename : str
                   Specify the filename of the configuration to be loaded
         boot_image : str
                     Specify the boot image. Can be primary or secondary boot image
         reboot : bool
                Set to True if switch is to be rebooted after firmware has been loaded
         """
-        output = self.send_command_timing(
-            "copy tftp flash " + tftp_server_ip + " " + filename + " " + boot_image
-        )
-        output += self.send_command_timing("y")
-        output += self.send_command_timing("\n", delay_factor=10)
+        cmd_list = [
+            "copy tftp flash " + tftp_server_ip + " " + filename + " " + boot_image,
+            "y",
+            "\n",
+        ]
+        self.send_multiline_timing(cmd_list)
         print("Firmware loaded for ", self.hostname)
-        if reboot:
-            self.send_command_timing("boot system flash " + boot_image)
-            self.send_command_timing("y")
+        if reboot is True:
+            cmd_list = ["boot system flash " + boot_image, "y"]
+            self.send_multiline_timing(cmd_list)
             print("Rebooting ", self.hostname)
             self.disconnect()
 
     def find_firmware_version(self):
         """Displays the version of firmware on the switch."""
         print("-" * 25)
         print(f"{'HOSTNAME':^10}{'VERSION':^10}")
@@ -631,15 +640,15 @@
     def find_ports_down(self):
         """Finds and displays the interfaces in a 'DOWN' state."""
         print("-" * 12)
         print(f"{self.hostname:^10}")
         print("-" * 12)
         print(f"{'PORT':5}{'STATUS':5}")
         print("-" * 12)
-        output = self.send_command_timing("show int brief", use_textfsm=True)
+        output = self.send_command("show int brief", use_textfsm=True)
         count = 0
         for ports in output:
             if ports["status"] == "Down":
                 count += 1
                 print(f"{ports['port']:^5}{ports['status']:^5}")
                 print("-" * 12)
         print()
@@ -648,15 +657,15 @@
     def find_ports_up(self):
         """Finds and displays the interfaces in an 'UP' state."""
         print("-" * 12)
         print(f"{self.hostname :^10}")
         print("-" * 12)
         print(f"{'PORT':5}{'STATUS':5}")
         print("-" * 12)
-        output = self.send_command_timing("show int brief", use_textfsm=True)
+        output = self.send_command("show int brief", use_textfsm=True)
         count = 0
         for ports in output:
             if ports["status"] == "Up":
                 count += 1
                 print(f"{ports['port']:^5}{ports['status']:^5}")
                 print("-" * 12)
         print()
@@ -669,15 +678,15 @@
         ----------
         mac_addresses : list
                        Specify the mac address(s)
         """
         print("-" * 70)
         print(f"{'HOSTNAME':^20}{'MAC_ADDRESS':>20}{'IP_ADDRESS':>20}")
         print("-" * 70)
-        output = self.send_command_timing("show arp", use_textfsm=True)
+        output = self.send_command("show arp", use_textfsm=True)
         for ip in output:
             for i in mac_address:
                 if ip["mac"] == i:
                     print(f"{self.hostname :^20}{ip['mac']:^30}{ip['ip']:^10}")
                     print("-" * 70)
 
     def find_mac_from_ip_address(self, ip_address):
@@ -687,15 +696,15 @@
         ----------
         ip_address : list
                        Specify the IP address(s)
         """
         print("-" * 70)
         print(f"{'HOSTNAME':^20}{'MAC_ADDRESS':>20}{'IP_ADDRESS':>20}")
         print("-" * 70)
-        output = self.send_command_timing("show arp", use_textfsm=True)
+        output = self.send_command("show arp", use_textfsm=True)
         for ip_addr in output:
             for i in ip_address:
                 if ip_addr["ip"] == i:
                     print(
                         f"{self.hostname :^20}{ip_addr['mac']:^30}{ip_addr['ip']:^10}"
                     )
                     print("-" * 70)
@@ -705,15 +714,15 @@
         print("-" * 85)
         print(f"{self.hostname:^85}")
         print("-" * 85)
         print(
             f"{'PORT':^20}{'LEARN_MODE':^20}{'ACTION':^20}{'EAVESDROP_PREVENTION':^25}"
         )
         print("-" * 85)
-        output = self.send_command_timing("show port-security", use_textfsm=True)
+        output = self.send_command("show port-security", use_textfsm=True)
         for port in output:
             if port["learn_mode"] != "Continuous":
                 print(
                     f"{port['port'] :^20}{port['learn_mode'] :^20}{port['action'] :^20}"
                     f"{port['eavesdrop_prevention'] :^25}"
                 )
                 print("-" * 85)
@@ -723,15 +732,15 @@
         print("-" * 85)
         print(f"{self.hostname:^85}")
         print("-" * 85)
         print(
             f"{'PORT':^20}{'LEARN_MODE':^20}{'ACTION':^20}{'EAVESDROP_PREVENTION':^25}"
         )
         print("-" * 85)
-        output = self.send_command_timing("show port-security", use_textfsm=True)
+        output = self.send_command("show port-security", use_textfsm=True)
         for port in output:
             if port["learn_mode"] == "Continuous":
                 print(
                     f"{port['port'] :^20}{port['learn_mode'] :^20}{port['action'] :^20}"
                     f"{port['eavesdrop_prevention'] :^25}"
                 )
                 print("-" * 85)
@@ -743,15 +752,15 @@
         ----------
         jumbo_vlan : list
                    Specify the jumbo vlan
         """
         print("-" * 20)
         print(f"{'HOSTNAME':^10}{'JUMBO_VLAN':^10}")
         print("-" * 20)
-        output = self.send_command_timing("show vlans", use_textfsm=True)
+        output = self.send_command("show vlans", use_textfsm=True)
         for j in output:
             for v in jumbo_vlan:
                 if j["jumbo"] == "Yes" and j["vlan_id"] == str(v):
                     print(f"{self.hostname:^10}{j['vlan_id']:^10}")
                     print("-" * 20)
 
     def find_voice_vlan(self, voice_vlan):
@@ -761,26 +770,27 @@
         ----------
         voice_vlan : int
                    Specify the voice vlan
         """
         print("-" * 20)
         print(f"{'HOSTNAME':^10}{'VOICE_VLAN':^10}")
         print("-" * 20)
-        output = self.send_command_timing("show vlans", use_textfsm=True)
+        output = self.send_command("show vlans", use_textfsm=True)
         for v in output:
             if v["voice"] == "Yes" and v["vlan_id"] == str(voice_vlan):
                 print(f"{self.hostname:^10}{v['vlan_id']:^10}")
                 print("-" * 20)
 
     def find_poe_enabled_ports(self):
         """Finds and displays the POE+ enabled ports"""
         print("-" * 25)
         print(f"{self.hostname :^25}")
         print("-" * 25)
         print(f"{'PORT':^10}{'POE_ENABLED':^10}")
+        print("_" * 25)
         output = self.send_command("show power-over-ethernet brief")
         output = output.strip().splitlines()
         for line in output:
             if re.search(r"^\s+\d+\s+Yes\s+", line, flags=re.M):
                 port, poe_status, *extra = line.split()
                 print(f"{port: ^10}{poe_status: ^10}")
                 print("-" * 25)
@@ -885,31 +895,29 @@
         print(f"{'NEIGHBOR':^15}{'TRUNK PORT':^15}{'PORT SPEED':^15}")
         print("-" * 45)
         output = self.send_command("show lldp info remote-device", use_textfsm=True)
         for i in output:
             if i["neighbor_sysname"] is not None:
                 neighbor_sysname = i["neighbor_sysname"]
                 port_number = i["local_port"]
-                int_output = self.send_command_timing(
-                    "show int brief", use_textfsm=True
-                )
+                int_output = self.send_command("show int brief", use_textfsm=True)
                 for i in int_output:
                     if port_number == i["port"]:
                         mode = i["mode"]
                         print(f"{neighbor_sysname:^15}{port_number:^15}{mode:^15}")
                         print("-" * 45)
                         print()
 
     def find_ntp_config(self):
         """finds and displays the ntp server if configured."""
         print()
         print("-" * 30)
         print(f"{'HOSTNAME':^15}{'NTP SERVER':^15}")
         print("-" * 30)
-        ntp_output = self.send_command_timing("show run").strip()
+        ntp_output = self.send_command("show run").strip()
         try:
             ntp_server = re.search(
                 r"^(ntp server (?P<ntp>\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3}))",
                 ntp_output,
                 flags=re.M,
             )
             print(f"{self.hostname:^15}{ntp_server.group('ntp'):^15}")
@@ -918,15 +926,15 @@
 
     def find_ntp_status(self):
         """finds and displays the ntp status with either Enabled or Disabled."""
         print()
         print("-" * 30)
         print(f"{'HOSTNAME':^15}{'NTP STATUS':^15}")
         print("-" * 30)
-        ntp_output = self.send_command_timing("show ntp status").strip()
+        ntp_output = self.send_command("show ntp status").strip()
         try:
             ntp_output = re.search(
                 r"^\s+NTP Status\s+:\s+(?P<ntp_status>Disabled|Enabled)\s+.*",
                 ntp_output,
                 flags=re.M,
             )
             print(f"{self.hostname:^15}{ntp_output.group('ntp_status'):^15}")
```

### Comparing `hp_procurvearuba-1.1.0/src/hp_procurvearuba.egg-info/PKG-INFO` & `hp_procurvearuba-2.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 Metadata-Version: 2.1
-Name: hp-procurvearuba
-Version: 1.1.0
+Name: hp_procurvearuba
+Version: 2.0.0
 Summary: Provides a class with custom functions for easy management of hp procurve and aruba switches
 Home-page: https://github.com/adraf82/hp_procurvearuba
 Author: Adeel Rauf
 Author-email: adraf2000@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div id="top"></div>
@@ -192,9 +187,7 @@
 
 <!-- MARKDOWN LINKS & IMAGES -->
 <!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
 [black-shield]:https://img.shields.io/badge/code%20style-black-000000.svg
 [black-url]:https://github.com/ambv/black
 [python-shield]:https://img.shields.io/pypi/v/hp_procurvearuba
 [python-url]:https://pypi.org/project/hp-procurvearuba
-
-
```

#### html2text {}

```diff
@@ -1,17 +1,14 @@
-Metadata-Version: 2.1 Name: hp-procurvearuba Version: 1.1.0 Summary: Provides a
+Metadata-Version: 2.1 Name: hp_procurvearuba Version: 2.0.0 Summary: Provides a
 class with custom functions for easy management of hp procurve and aruba
 switches Home-page: https://github.com/adraf82/hp_procurvearuba Author: Adeel
-Rauf Author-email: adraf2000@gmail.com License: UNKNOWN Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
-LICENSE
+Rauf Author-email: adraf2000@gmail.com Classifier: License :: OSI Approved ::
+MIT License Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Requires-Python: >=3.6 Description-
+Content-Type: text/markdown License-File: LICENSE
 [![Code style][black-shield]][black-url] [![PyPI][python-shield]][python-url]
                                     [Logo]
                           **** hp_procurvearuba ****
             For easy management of hp procurve and aruba switches
                              Explore_the_docs_Â»
 
                          Report_Bug Â· Request_Feature
```

