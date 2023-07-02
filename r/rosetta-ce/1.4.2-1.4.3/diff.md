# Comparing `tmp/rosetta-ce-1.4.2.tar.gz` & `tmp/rosetta-ce-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rosetta-ce-1.4.2.tar", last modified: Sun Jul  2 15:59:53 2023, max compression
+gzip compressed data, was "rosetta-ce-1.4.3.tar", last modified: Sun Jul  2 18:04:26 2023, max compression
```

## Comparing `rosetta-ce-1.4.2.tar` & `rosetta-ce-1.4.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-02 15:59:53.402395 rosetta-ce-1.4.2/
--rw-r--r--   0 amahmoud   (502) staff       (20)     1070 2023-04-08 17:22:13.000000 rosetta-ce-1.4.2/LICENSE
--rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-07-02 15:59:53.402075 rosetta-ce-1.4.2/PKG-INFO
--rw-r--r--   0 amahmoud   (502) staff       (20)    10721 2023-06-29 06:50:02.000000 rosetta-ce-1.4.2/README.md
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-02 15:59:53.396174 rosetta-ce-1.4.2/rosetta/
--rw-r--r--   0 amahmoud   (502) staff       (20)       92 2023-04-09 08:11:12.000000 rosetta-ce-1.4.2/rosetta/__init__.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-02 15:59:53.397945 rosetta-ce-1.4.2/rosetta/constants/
--rw-r--r--   0 amahmoud   (502) staff       (20)        0 2023-04-12 16:36:37.000000 rosetta-ce-1.4.2/rosetta/constants/__init__.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1936 2023-04-09 13:32:25.000000 rosetta-ce-1.4.2/rosetta/constants/sensors.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1658 2023-04-25 15:36:11.000000 rosetta-ce-1.4.2/rosetta/constants/sources.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     6697 2023-04-25 15:36:11.000000 rosetta-ce-1.4.2/rosetta/constants/systems.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     3008 2023-04-26 09:01:43.000000 rosetta-ce-1.4.2/rosetta/rconverter.py
--rw-r--r--   0 amahmoud   (502) staff       (20)    43246 2023-07-02 15:59:06.000000 rosetta-ce-1.4.2/rosetta/rfaker.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     8572 2023-06-29 15:55:20.000000 rosetta-ce-1.4.2/rosetta/rsender.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-02 15:59:53.399825 rosetta-ce-1.4.2/rosetta_ce.egg-info/
--rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-07-02 15:59:53.000000 rosetta-ce-1.4.2/rosetta_ce.egg-info/PKG-INFO
--rw-r--r--   0 amahmoud   (502) staff       (20)      459 2023-07-02 15:59:53.000000 rosetta-ce-1.4.2/rosetta_ce.egg-info/SOURCES.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)        1 2023-07-02 15:59:53.000000 rosetta-ce-1.4.2/rosetta_ce.egg-info/dependency_links.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)       23 2023-07-02 15:59:53.000000 rosetta-ce-1.4.2/rosetta_ce.egg-info/requires.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)        8 2023-07-02 15:59:53.000000 rosetta-ce-1.4.2/rosetta_ce.egg-info/top_level.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)       38 2023-07-02 15:59:53.402449 rosetta-ce-1.4.2/setup.cfg
--rw-r--r--   0 amahmoud   (502) staff       (20)      851 2023-07-02 15:59:14.000000 rosetta-ce-1.4.2/setup.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-02 15:59:53.401502 rosetta-ce-1.4.2/tests/
--rw-r--r--   0 amahmoud   (502) staff       (20)     1040 2023-04-26 09:01:43.000000 rosetta-ce-1.4.2/tests/test_rconverter.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     5226 2023-04-25 15:36:11.000000 rosetta-ce-1.4.2/tests/test_rfaker.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1763 2023-04-26 09:02:44.000000 rosetta-ce-1.4.2/tests/test_rsender.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-02 18:04:26.976531 rosetta-ce-1.4.3/
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1070 2023-04-08 17:22:13.000000 rosetta-ce-1.4.3/LICENSE
+-rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-07-02 18:04:26.976226 rosetta-ce-1.4.3/PKG-INFO
+-rw-r--r--   0 amahmoud   (502) staff       (20)    10721 2023-06-29 06:50:02.000000 rosetta-ce-1.4.3/README.md
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-02 18:04:26.970011 rosetta-ce-1.4.3/rosetta/
+-rw-r--r--   0 amahmoud   (502) staff       (20)       92 2023-04-09 08:11:12.000000 rosetta-ce-1.4.3/rosetta/__init__.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-02 18:04:26.971899 rosetta-ce-1.4.3/rosetta/constants/
+-rw-r--r--   0 amahmoud   (502) staff       (20)        0 2023-04-12 16:36:37.000000 rosetta-ce-1.4.3/rosetta/constants/__init__.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1936 2023-04-09 13:32:25.000000 rosetta-ce-1.4.3/rosetta/constants/sensors.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1658 2023-04-25 15:36:11.000000 rosetta-ce-1.4.3/rosetta/constants/sources.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     6697 2023-04-25 15:36:11.000000 rosetta-ce-1.4.3/rosetta/constants/systems.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     3008 2023-04-26 09:01:43.000000 rosetta-ce-1.4.3/rosetta/rconverter.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)    43848 2023-07-02 18:03:11.000000 rosetta-ce-1.4.3/rosetta/rfaker.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     8572 2023-06-29 15:55:20.000000 rosetta-ce-1.4.3/rosetta/rsender.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-02 18:04:26.974039 rosetta-ce-1.4.3/rosetta_ce.egg-info/
+-rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-07-02 18:04:26.000000 rosetta-ce-1.4.3/rosetta_ce.egg-info/PKG-INFO
+-rw-r--r--   0 amahmoud   (502) staff       (20)      459 2023-07-02 18:04:26.000000 rosetta-ce-1.4.3/rosetta_ce.egg-info/SOURCES.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)        1 2023-07-02 18:04:26.000000 rosetta-ce-1.4.3/rosetta_ce.egg-info/dependency_links.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)       23 2023-07-02 18:04:26.000000 rosetta-ce-1.4.3/rosetta_ce.egg-info/requires.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)        8 2023-07-02 18:04:26.000000 rosetta-ce-1.4.3/rosetta_ce.egg-info/top_level.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)       38 2023-07-02 18:04:26.976569 rosetta-ce-1.4.3/setup.cfg
+-rw-r--r--   0 amahmoud   (502) staff       (20)      851 2023-07-02 18:03:11.000000 rosetta-ce-1.4.3/setup.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-02 18:04:26.975745 rosetta-ce-1.4.3/tests/
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1040 2023-04-26 09:01:43.000000 rosetta-ce-1.4.3/tests/test_rconverter.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     5226 2023-04-25 15:36:11.000000 rosetta-ce-1.4.3/tests/test_rfaker.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1763 2023-04-26 09:02:44.000000 rosetta-ce-1.4.3/tests/test_rsender.py
```

### Comparing `rosetta-ce-1.4.2/LICENSE` & `rosetta-ce-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.2/PKG-INFO` & `rosetta-ce-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosetta-ce
-Version: 1.4.2
+Version: 1.4.3
 Summary: Rosetta is a Python package that can be used to fake security logs and alerts for testing different detection and response use cases.
 Home-page: https://github.com/ayman-m/rosetta
 Author: Ayman Mahmoud
 Author-email: content@ayman.online
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rosetta-ce-1.4.2/README.md` & `rosetta-ce-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.2/rosetta/constants/sensors.py` & `rosetta-ce-1.4.3/rosetta/constants/sensors.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.2/rosetta/constants/sources.py` & `rosetta-ce-1.4.3/rosetta/constants/sources.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.2/rosetta/constants/systems.py` & `rosetta-ce-1.4.3/rosetta/constants/systems.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.2/rosetta/rconverter.py` & `rosetta-ce-1.4.3/rosetta/rconverter.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.2/rosetta/rfaker.py` & `rosetta-ce-1.4.3/rosetta/rfaker.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,49 +31,53 @@
 
 class Observables:
     def __init__(self, local_ip: list = None, remote_ip: Optional[list] = None, local_ip_v6: list = None,
                  remote_ip_v6: Optional[list] = None, src_host: Optional[list] = None,
                  dst_host: Optional[list] = None, src_domain: Optional[list] = None, dst_domain: Optional[list] = None,
                  sender_email: Optional[list] = None, recipient_email: Optional[list] = None,
                  email_subject: Optional[list] = None, email_body: Optional[list] = None,
-                 url: Optional[list] = None, port: Optional[list] = None, protocol: Optional[list] = None,
-                 inbound_bytes: Optional[list] = None, outbound_bytes: Optional[list] = None,
-                 app: Optional[list] = None, os: Optional[list] = None, user: Optional[list] = None,
-                 cve: Optional[list] = None, file_name: Optional[list] = None, file_hash: Optional[list] = None,
-                 cmd: Optional[list] = None, process: Optional[list] = None, technique: Optional[list] = None,
-                 entry_type: Optional[list] = None, severity: Optional[list] = None, sensor: Optional[list] = None,
-                 action: Optional[list] = None, event_id: Optional[list] = None, error_code: Optional[list] = None,
-                 terms: Optional[list] = None, alert_types: Optional[list] = None, alert_name: Optional[list] = None,
-                 incident_types: Optional[list] = None, analysts: Optional[list] = None,
-                 action_status: Optional[list] = None):
+                 url: Optional[list] = None, source_port: Optional[list] = None, remote_port: Optional[list] = None,
+                 protocol: Optional[list] = None, inbound_bytes: Optional[list] = None,
+                 outbound_bytes: Optional[list] = None, app: Optional[list] = None, os: Optional[list] = None,
+                 user: Optional[list] = None, cve: Optional[list] = None, file_name: Optional[list] = None,
+                 file_hash: Optional[list] = None, win_cmd: Optional[list] = None, unix_cmd: Optional[list] = None,
+                 win_process: Optional[list] = None, unix_process: Optional[list] = None,
+                 technique: Optional[list] = None, entry_type: Optional[list] = None, severity: Optional[list] = None,
+                 sensor: Optional[list] = None, action: Optional[list] = None, event_id: Optional[list] = None,
+                 error_code: Optional[list] = None, terms: Optional[list] = None, alert_types: Optional[list] = None,
+                 alert_name: Optional[list] = None, incident_types: Optional[list] = None,
+                 analysts: Optional[list] = None, action_status: Optional[list] = None):
         self.local_ip = local_ip
         self.remote_ip = remote_ip
         self.local_ip_v6 = local_ip_v6
         self.remote_ip_v6 = remote_ip_v6
         self.src_host = src_host
         self.dst_host = dst_host
         self.src_domain = src_domain
         self.dst_domain = dst_domain
         self.sender_email = sender_email
         self.recipient_email = recipient_email
         self.email_subject = email_subject
         self.email_body = email_body
         self.url = url
-        self.port = port
+        self.source_port = source_port
+        self.remote_port = remote_port
         self.protocol = protocol
         self.inbound_bytes = inbound_bytes
         self.outbound_bytes = outbound_bytes
         self.app = app
         self.os = os
         self.user = user
         self.cve = cve
         self.file_name = file_name
         self.file_hash = file_hash
-        self.cmd = cmd
-        self.process = process
+        self.win_cmd = win_cmd
+        self.unix_cmd = unix_cmd
+        self.win_process = win_process
+        self.unix_process = unix_process
         self.technique = technique
         self.entry_type = entry_type
         self.severity = severity
         self.sensor = sensor
         self.action = action
         self.event_id = event_id
         self.error_code = error_code
@@ -289,32 +293,32 @@
         if field == "host":
             field_value = random.choice(observables.src_host) if observables and observables.src_host \
                 else faker.hostname()
         if field == "user":
             field_value = random.choice(observables.user) if observables and observables.user \
                 else faker.user_name()
         if field == "unix_process":
-            field_value = random.choice(observables.process) if observables and observables.process \
+            field_value = random.choice(observables.unix_process) if observables and observables.unix_process \
                 else "sudo"
         if field == "unix_cmd":
-            field_value = random.choice(observables.cmd) if observables and observables.cmd \
+            field_value = random.choice(observables.unix_cmd) if observables and observables.unix_cmd \
                 else random.choice(UNIX_CMD)
         if field == "severity":
             field_value = random.choice(observables.severity) if observables and observables.severity \
                 else faker.random_int(min=1, max=5)
         if field == "local_ip":
             field_value = random.choice(observables.local_ip) if observables and observables.local_ip \
                     else faker.ipv4()
         if field == "local_port":
             field_value = faker.random_int(min=1024, max=65535)
         if field == "remote_ip":
             field_value = random.choice(observables.remote_ip) if observables and observables.remote_ip \
                     else Observables.generator(observable_type=ObservableType.IP, known=ObservableKnown.BAD, count=1)
         if field == "remote_port":
-            field_value = random.choice(observables.port) if observables and observables.port \
+            field_value = random.choice(observables.remote_port) if observables and observables.remote_port \
                     else faker.random_int(min=1024, max=65535)
         if field == "dst_url":
             field_value = random.choice(observables.url) if observables and observables.url \
                     else Observables.generator(observable_type=ObservableType.URL, known=ObservableKnown.BAD, count=1)
         if field == "inbound_bytes":
             field_value = random.choice(observables.inbound_bytes) if observables and observables.inbound_bytes \
                     else faker.random_int(min=10, max=1073741824)
@@ -332,14 +336,17 @@
                     else random.choice(ACTIONS)
         if field == "src_domain":
             field_value = random.choice(observables.src_domain) if observables and observables.src_domain \
                     else faker.domain_name()
         if field == "sender_email":
             field_value = random.choice(observables.sender_email) if observables and observables.sender_email \
                     else faker.email()
+        if field == "recipient_email":
+            field_value = random.choice(observables.recipient_email) if observables and observables.recipient_email \
+                    else faker.email()
         if field == "email_subject":
             field_value = random.choice(observables.email_subject) if observables and observables.email_subject \
                     else faker.sentence(nb_words=6)
         if field == "email_body":
             field_value = random.choice(observables.email_body) if observables and observables.email_body else \
                     faker.sentence(nb_words=50)
         if field == "attachment_hash":
@@ -388,19 +395,19 @@
         if field == "destination_login_id":
             field_value = faker.random_int()
         if field == "privilege_list":
             field_value = faker.sentence(nb_words=5)
         if field == "event_record_id":
             field_value = random.choice(observables.event_id) if observables and observables.event_id \
                 else faker.random.randint(1, 999)
-        if field == "win_process_name":
-            field_value = random.choice(observables.process) if observables and observables.process \
+        if field == "win_process":
+            field_value = random.choice(observables.win_process) if observables and observables.win_process \
                 else random.choice(WIN_PROCESSES)
         if field == "win_cmd":
-            field_value = random.choice(observables.cmd) if observables and observables.cmd \
+            field_value = random.choice(observables.win_cmd) if observables and observables.win_cmd \
                 else random.choice(WINDOWS_CMD)
         if field == "source_network_address":
             field_value = random.choice(observables.local_ip) if observables and observables.local_ip \
                 else faker.ipv4_private()
         if field == "file_name":
             field_value = random.choice(observables.file_name) if observables and observables.file_name \
                 else faker.file_name()
@@ -421,15 +428,15 @@
             field_value = random.randint(1, 5)
         if field == "log_id":
             field_value = faker.uuid4()
         return field_value
 
     @classmethod
     def syslog(cls, count: int, timestamp: Optional[datetime] = None, observables: Optional[Observables] = None,
-               required_fields: Optional[str] = "pid,host,user,unix_process,unix_cmd") -> List[str]:
+               required_fields: Optional[str] = None) -> List[str]:
         """
         Generate fake syslog messages.
 
         Args:
             count: The number of syslog messages to generate.
             timestamp: Optional. The starting timestamp for the syslog messages. If not provided, a random time during
             the past hour from now will be used.
@@ -450,14 +457,16 @@
 
         """
         syslog_messages = []
         faker = cls._create_faker()
         if timestamp is None:
             timestamp = datetime.now() - timedelta(hours=1)
             timestamp += timedelta(seconds=faker.random_int(min=0, max=3599))
+        if not required_fields:
+            required_fields = "pid,host,user,unix_process,unix_cmd"
         for i in range(count):
             timestamp += timedelta(seconds=1)
             syslog_message = f"{timestamp.strftime('%Y-%m-%d %H:%M:%S')}"
             for field in required_fields.split(","):
                 syslog_message += f" {cls.set_field(field, observables)}"
             if observables:
                 for observable, observable_value in vars(observables).items():
@@ -586,15 +595,15 @@
                            f"severity={cls.set_field('severity', observables)}|"
             for field in required_fields.split(","):
                 leef_message += f" {field}={cls.set_field(field, observables)}"
             if observables:
                 for observable, observable_value in vars(observables).items():
                     if observable_value and observable not in required_fields.split(","):
                         leef_message += f" {observable}={random.choice(observable_value)}"
-            leef_messages.append(required_fields)
+            leef_messages.append(leef_message)
         return leef_messages
 
     @classmethod
     def winevent(cls, count, timestamp: Optional[datetime] = None, observables: Optional[Observables] = None) -> \
             List[str]:
         """
         Generates fake Windows Event Log messages.
@@ -629,21 +638,21 @@
             domain_name = faker.domain_name()
             subject_login_id = faker.random_int()
             user_id = "S-1-" + str(faker.random_int())
             destination_login_id = faker.random_int()
             privilege_list = faker.sentence(nb_words=5)
             event_record_id = random.choice(observables.event_id) if observables and observables.event_id \
                 else faker.random.randint(1, 999)
-            process_name = random.choice(observables.process) if observables and observables.process \
+            process_name = random.choice(observables.win_process) if observables and observables.win_process \
                 else random.choice(WIN_PROCESSES)
             host = random.choice(observables.src_host) if observables and observables.src_host \
                 else faker.hostname()
             user_name = random.choice(observables.user) if observables and observables.user \
                 else faker.user_name()
-            cmd = random.choice(observables.cmd) if observables and observables.cmd \
+            cmd = random.choice(observables.win_cmd) if observables and observables.win_cmd \
                 else random.choice(WINDOWS_CMD)
             source_network_address = random.choice(observables.local_ip) if observables and observables.local_ip \
                 else faker.ipv4_private()
             file_name = random.choice(observables.file_name) if observables and observables.file_name \
                 else faker.file_name()
             unformatted_event = random.choice(WIN_EVENTS)
             win_event = unformatted_event.format(guid=guid, system_time=system_time, event_record_id=event_record_id,
```

### Comparing `rosetta-ce-1.4.2/rosetta/rsender.py` & `rosetta-ce-1.4.3/rosetta/rsender.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.2/rosetta_ce.egg-info/PKG-INFO` & `rosetta-ce-1.4.3/rosetta_ce.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosetta-ce
-Version: 1.4.2
+Version: 1.4.3
 Summary: Rosetta is a Python package that can be used to fake security logs and alerts for testing different detection and response use cases.
 Home-page: https://github.com/ayman-m/rosetta
 Author: Ayman Mahmoud
 Author-email: content@ayman.online
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rosetta-ce-1.4.2/setup.py` & `rosetta-ce-1.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rosetta-ce",
-    version="1.4.2",
+    version="1.4.3",
     author="Ayman Mahmoud",
     author_email="content@ayman.online",
     description="Rosetta is a Python package that can be used to fake security logs and alerts for testing different "
                 "detection and response use cases.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ayman-m/rosetta",
```

### Comparing `rosetta-ce-1.4.2/tests/test_rconverter.py` & `rosetta-ce-1.4.3/tests/test_rconverter.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.2/tests/test_rfaker.py` & `rosetta-ce-1.4.3/tests/test_rfaker.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.2/tests/test_rsender.py` & `rosetta-ce-1.4.3/tests/test_rsender.py`

 * *Files identical despite different names*

