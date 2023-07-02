# Comparing `tmp/rosetta-ce-1.4.0.tar.gz` & `tmp/rosetta-ce-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rosetta-ce-1.4.0.tar", last modified: Sun Jul  2 08:56:40 2023, max compression
+gzip compressed data, was "rosetta-ce-1.4.1.tar", last modified: Sun Jul  2 15:50:05 2023, max compression
```

## Comparing `rosetta-ce-1.4.0.tar` & `rosetta-ce-1.4.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-02 08:56:40.185110 rosetta-ce-1.4.0/
--rw-r--r--   0 amahmoud   (502) staff       (20)     1070 2023-04-08 17:22:13.000000 rosetta-ce-1.4.0/LICENSE
--rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-07-02 08:56:40.184771 rosetta-ce-1.4.0/PKG-INFO
--rw-r--r--   0 amahmoud   (502) staff       (20)    10721 2023-06-29 06:50:02.000000 rosetta-ce-1.4.0/README.md
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-02 08:56:40.178525 rosetta-ce-1.4.0/rosetta/
--rw-r--r--   0 amahmoud   (502) staff       (20)       92 2023-04-09 08:11:12.000000 rosetta-ce-1.4.0/rosetta/__init__.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-02 08:56:40.180637 rosetta-ce-1.4.0/rosetta/constants/
--rw-r--r--   0 amahmoud   (502) staff       (20)        0 2023-04-12 16:36:37.000000 rosetta-ce-1.4.0/rosetta/constants/__init__.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1936 2023-04-09 13:32:25.000000 rosetta-ce-1.4.0/rosetta/constants/sensors.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1658 2023-04-25 15:36:11.000000 rosetta-ce-1.4.0/rosetta/constants/sources.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     6697 2023-04-25 15:36:11.000000 rosetta-ce-1.4.0/rosetta/constants/systems.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     3008 2023-04-26 09:01:43.000000 rosetta-ce-1.4.0/rosetta/rconverter.py
--rw-r--r--   0 amahmoud   (502) staff       (20)    44021 2023-07-02 08:53:18.000000 rosetta-ce-1.4.0/rosetta/rfaker.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     8572 2023-06-29 15:55:20.000000 rosetta-ce-1.4.0/rosetta/rsender.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-02 08:56:40.182829 rosetta-ce-1.4.0/rosetta_ce.egg-info/
--rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-07-02 08:56:40.000000 rosetta-ce-1.4.0/rosetta_ce.egg-info/PKG-INFO
--rw-r--r--   0 amahmoud   (502) staff       (20)      459 2023-07-02 08:56:40.000000 rosetta-ce-1.4.0/rosetta_ce.egg-info/SOURCES.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)        1 2023-07-02 08:56:40.000000 rosetta-ce-1.4.0/rosetta_ce.egg-info/dependency_links.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)       23 2023-07-02 08:56:40.000000 rosetta-ce-1.4.0/rosetta_ce.egg-info/requires.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)        8 2023-07-02 08:56:40.000000 rosetta-ce-1.4.0/rosetta_ce.egg-info/top_level.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)       38 2023-07-02 08:56:40.185148 rosetta-ce-1.4.0/setup.cfg
--rw-r--r--   0 amahmoud   (502) staff       (20)      851 2023-07-02 08:56:13.000000 rosetta-ce-1.4.0/setup.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-02 08:56:40.184269 rosetta-ce-1.4.0/tests/
--rw-r--r--   0 amahmoud   (502) staff       (20)     1040 2023-04-26 09:01:43.000000 rosetta-ce-1.4.0/tests/test_rconverter.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     5226 2023-04-25 15:36:11.000000 rosetta-ce-1.4.0/tests/test_rfaker.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1763 2023-04-26 09:02:44.000000 rosetta-ce-1.4.0/tests/test_rsender.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-02 15:50:05.766526 rosetta-ce-1.4.1/
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1070 2023-04-08 17:22:13.000000 rosetta-ce-1.4.1/LICENSE
+-rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-07-02 15:50:05.766231 rosetta-ce-1.4.1/PKG-INFO
+-rw-r--r--   0 amahmoud   (502) staff       (20)    10721 2023-06-29 06:50:02.000000 rosetta-ce-1.4.1/README.md
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-02 15:50:05.760109 rosetta-ce-1.4.1/rosetta/
+-rw-r--r--   0 amahmoud   (502) staff       (20)       92 2023-04-09 08:11:12.000000 rosetta-ce-1.4.1/rosetta/__init__.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-02 15:50:05.762004 rosetta-ce-1.4.1/rosetta/constants/
+-rw-r--r--   0 amahmoud   (502) staff       (20)        0 2023-04-12 16:36:37.000000 rosetta-ce-1.4.1/rosetta/constants/__init__.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1936 2023-04-09 13:32:25.000000 rosetta-ce-1.4.1/rosetta/constants/sensors.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1658 2023-04-25 15:36:11.000000 rosetta-ce-1.4.1/rosetta/constants/sources.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     6697 2023-04-25 15:36:11.000000 rosetta-ce-1.4.1/rosetta/constants/systems.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     3008 2023-04-26 09:01:43.000000 rosetta-ce-1.4.1/rosetta/rconverter.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)    42827 2023-07-02 15:44:30.000000 rosetta-ce-1.4.1/rosetta/rfaker.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     8572 2023-06-29 15:55:20.000000 rosetta-ce-1.4.1/rosetta/rsender.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-02 15:50:05.764091 rosetta-ce-1.4.1/rosetta_ce.egg-info/
+-rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-07-02 15:50:05.000000 rosetta-ce-1.4.1/rosetta_ce.egg-info/PKG-INFO
+-rw-r--r--   0 amahmoud   (502) staff       (20)      459 2023-07-02 15:50:05.000000 rosetta-ce-1.4.1/rosetta_ce.egg-info/SOURCES.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)        1 2023-07-02 15:50:05.000000 rosetta-ce-1.4.1/rosetta_ce.egg-info/dependency_links.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)       23 2023-07-02 15:50:05.000000 rosetta-ce-1.4.1/rosetta_ce.egg-info/requires.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)        8 2023-07-02 15:50:05.000000 rosetta-ce-1.4.1/rosetta_ce.egg-info/top_level.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)       38 2023-07-02 15:50:05.766568 rosetta-ce-1.4.1/setup.cfg
+-rw-r--r--   0 amahmoud   (502) staff       (20)      851 2023-07-02 15:47:13.000000 rosetta-ce-1.4.1/setup.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-02 15:50:05.765704 rosetta-ce-1.4.1/tests/
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1040 2023-04-26 09:01:43.000000 rosetta-ce-1.4.1/tests/test_rconverter.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     5226 2023-04-25 15:36:11.000000 rosetta-ce-1.4.1/tests/test_rfaker.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1763 2023-04-26 09:02:44.000000 rosetta-ce-1.4.1/tests/test_rsender.py
```

### Comparing `rosetta-ce-1.4.0/LICENSE` & `rosetta-ce-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.0/PKG-INFO` & `rosetta-ce-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosetta-ce
-Version: 1.4.0
+Version: 1.4.1
 Summary: Rosetta is a Python package that can be used to fake security logs and alerts for testing different detection and response use cases.
 Home-page: https://github.com/ayman-m/rosetta
 Author: Ayman Mahmoud
 Author-email: content@ayman.online
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rosetta-ce-1.4.0/README.md` & `rosetta-ce-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.0/rosetta/constants/sensors.py` & `rosetta-ce-1.4.1/rosetta/constants/sensors.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.0/rosetta/constants/sources.py` & `rosetta-ce-1.4.1/rosetta/constants/sources.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.0/rosetta/constants/systems.py` & `rosetta-ce-1.4.1/rosetta/constants/systems.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.0/rosetta/rconverter.py` & `rosetta-ce-1.4.1/rosetta/rconverter.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.0/rosetta/rfaker.py` & `rosetta-ce-1.4.1/rosetta/rfaker.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,31 +26,33 @@
 
 class ObservableKnown(Enum):
     BAD = 'bad'
     GOOD = 'good'
 
 
 class Observables:
-    def __init__(self, src_ip: list = None, dst_ip: Optional[list] = None, src_ipv6: list = None,
-                 dst_ipv6: Optional[list] = None, src_host: Optional[list] = None,
+    def __init__(self, local_ip: list = None, remote_ip: Optional[list] = None, local_ip_v6: list = None,
+                 remote_ip_v6: Optional[list] = None, src_host: Optional[list] = None,
                  dst_host: Optional[list] = None, src_domain: Optional[list] = None, dst_domain: Optional[list] = None,
                  sender_email: Optional[list] = None, recipient_email: Optional[list] = None,
                  email_subject: Optional[list] = None, email_body: Optional[list] = None,
                  url: Optional[list] = None, port: Optional[list] = None, protocol: Optional[list] = None,
                  inbound_bytes: Optional[list] = None, outbound_bytes: Optional[list] = None,
                  app: Optional[list] = None, os: Optional[list] = None, user: Optional[list] = None,
                  cve: Optional[list] = None, file_name: Optional[list] = None, file_hash: Optional[list] = None,
                  cmd: Optional[list] = None, process: Optional[list] = None, technique: Optional[list] = None,
                  entry_type: Optional[list] = None, severity: Optional[list] = None, sensor: Optional[list] = None,
                  action: Optional[list] = None, event_id: Optional[list] = None, error_code: Optional[list] = None,
-                 terms: Optional[list] = None, incident_types: Optional[list] = None, analysts: Optional[list] = None):
-        self.src_ip = src_ip
-        self.dst_ip = dst_ip
-        self.src_ipv6 = src_ipv6
-        self.dst_ipv6 = dst_ipv6
+                 terms: Optional[list] = None, alert_types: Optional[list] = None, alert_name: Optional[list] = None,
+                 incident_types: Optional[list] = None, analysts: Optional[list] = None,
+                 action_status: Optional[list] = None):
+        self.local_ip = local_ip
+        self.remote_ip = remote_ip
+        self.local_ip_v6 = local_ip_v6
+        self.remote_ip_v6 = remote_ip_v6
         self.src_host = src_host
         self.dst_host = dst_host
         self.src_domain = src_domain
         self.dst_domain = dst_domain
         self.sender_email = sender_email
         self.recipient_email = recipient_email
         self.email_subject = email_subject
@@ -74,14 +76,17 @@
         self.sensor = sensor
         self.action = action
         self.event_id = event_id
         self.error_code = error_code
         self.terms = terms
         self.incident_types = incident_types
         self.analysts = analysts
+        self.alert_types = alert_types
+        self.alert_name = alert_name
+        self.action_status = action_status
 
     @staticmethod
     def _get_observables_from_source(source: dict) -> list:
         """
         Fetches observables from a given source and returns them as a list.
 
         Args:
@@ -268,25 +273,174 @@
         """
         Returns:
             Faker instance.
         """
         return Observables()
 
     @classmethod
-    def syslog(cls, count: int, timestamp: Optional[datetime] = None, observables: Optional[Observables] = None) -> \
-            List[str]:
+    def set_field(cls, field, observables: Optional[Observables] = None):
+        """
+        Returns:
+            Field value.
+        """
+        field_value = None
+        faker = cls._create_faker()
+        if field == "pid":
+            field_value = faker.random_int(min=1000, max=65535)
+        if field == "host":
+            field_value = random.choice(observables.src_host) if observables and observables.src_host \
+                else faker.hostname()
+        if field == "user":
+            field_value = random.choice(observables.user) if observables and observables.user \
+                else faker.user_name()
+        if field == "unix_process":
+            field_value = random.choice(observables.process) if observables and observables.process \
+                else "sudo"
+        if field == "unix_cmd":
+            field_value = random.choice(observables.cmd) if observables and observables.cmd \
+                else random.choice(UNIX_CMD)
+        if field == "severity":
+            field_value = random.choice(observables.severity) if observables and observables.severity \
+                else faker.random_int(min=1, max=5)
+        if field == "local_ip":
+            field_value = random.choice(observables.local_ip) if observables and observables.local_ip \
+                    else faker.ipv4()
+        if field == "local_port":
+            field_value = faker.random_int(min=1024, max=65535)
+        if field == "remote_ip":
+            field_value = random.choice(observables.remote_ip) if observables and observables.remote_ip \
+                    else Observables.generator(observable_type=ObservableType.IP, known=ObservableKnown.BAD, count=1)
+        if field == "remote_port":
+            field_value = random.choice(observables.port) if observables and observables.port \
+                    else faker.random_int(min=1024, max=65535)
+        if field == "dst_url":
+            field_value = random.choice(observables.url) if observables and observables.url \
+                    else Observables.generator(observable_type=ObservableType.URL, known=ObservableKnown.BAD, count=1)
+        if field == "inbound_bytes":
+            field_value = random.choice(observables.inbound_bytes) if observables and observables.inbound_bytes \
+                    else faker.random_int(min=10, max=1073741824)
+        if field == "outbound_bytes":
+            field_value = random.choice(observables.outbound_bytes) if observables and observables.outbound_bytes \
+                    else faker.random_int(min=10, max=1073741824)
+        if field == "protocol":
+            field_value = random.choice(observables.protocol) if observables and observables.protocol \
+                    else random.choice(PROTOCOLS)
+        if field == "rule_id":
+            field_value = random.choice(observables.event_id) if observables and observables.event_id \
+                    else faker.random_int(min=1, max=200)
+        if field == "action":
+            field_value = random.choice(observables.action) if observables and observables.action \
+                    else random.choice(ACTIONS)
+        if field == "src_domain":
+            field_value = random.choice(observables.src_domain) if observables and observables.src_domain \
+                    else faker.domain_name()
+        if field == "sender_email":
+            field_value = random.choice(observables.sender_email) if observables and observables.sender_email \
+                    else faker.email()
+        if field == "email_subject":
+            field_value = random.choice(observables.email_subject) if observables and observables.email_subject \
+                    else faker.sentence(nb_words=6)
+        if field == "email_body":
+            field_value = random.choice(observables.email_body) if observables and observables.email_body else \
+                    faker.sentence(nb_words=50)
+        if field == "attachment_hash":
+            field_value = random.choice(observables.file_hash) if observables and observables.file_hash \
+                    else Observables.generator(observable_type=ObservableType.SHA256, known=ObservableKnown.BAD,
+                                               count=1)
+        if field == "spam_score":
+            field_value = faker.random_int(min=1, max=5)
+        if field == "method":
+            field_value = random.choice(observables.technique).get('mechanism') if observables and \
+                    observables.technique else random.choice(TECHNIQUES).get('mechanism')
+        if field == "url":
+            field_value = random.choice(observables.technique).get('indicator') if observables and \
+                    observables.technique else random.choice(TECHNIQUES).get('indicator')
+        if field == "user_agent":
+            field_value = faker.user_agent()
+        if field == "referer":
+            field_value = random.choice(observables.url) if observables and observables.url \
+                    else Observables.generator(observable_type=ObservableType.URL, known=ObservableKnown.BAD, count=1)
+        if field == "response_code":
+            field_value = random.choice(observables.error_code) if observables and observables.error_code \
+                    else random.choice(ERROR_CODE)
+        if field == "response_size":
+            field_value = faker.random_int(min=100, max=10000)
+        if field == "attack_type":
+            field_value = random.choice(observables.technique).get('technique') if observables and \
+                    observables.technique else random.choice(TECHNIQUES).get('technique')
+        if field == "cookies":
+            field_value = f"{faker.word()}={faker.uuid4()}"
+        if field == "guid":
+            field_value = faker.uuid4()
+        if field == "transmitted_services":
+            field_value = faker.sentence(nb_words=5)
+        if field == "process_id":
+            field_value = faker.random_int()
+        if field == "new_process_id":
+            field_value = faker.random_int()
+        if field == "thread_id":
+            field_value = faker.random_int()
+        if field == "target_pid":
+            field_value = faker.random_int()
+        if field == "subject_login_id":
+            field_value = faker.random_int()
+        if field == "win_user_id":
+            field_value = "S-1-" + str(faker.random_int())
+        if field == "destination_login_id":
+            field_value = faker.random_int()
+        if field == "privilege_list":
+            field_value = faker.sentence(nb_words=5)
+        if field == "event_record_id":
+            field_value = random.choice(observables.event_id) if observables and observables.event_id \
+                else faker.random.randint(1, 999)
+        if field == "win_process_name":
+            field_value = random.choice(observables.process) if observables and observables.process \
+                else random.choice(WIN_PROCESSES)
+        if field == "win_cmd":
+            field_value = random.choice(observables.cmd) if observables and observables.cmd \
+                else random.choice(WINDOWS_CMD)
+        if field == "source_network_address":
+            field_value = random.choice(observables.local_ip) if observables and observables.local_ip \
+                else faker.ipv4_private()
+        if field == "file_name":
+            field_value = random.choice(observables.file_name) if observables and observables.file_name \
+                else faker.file_name()
+        if field == "cve_id":
+            field_value = random.choice(observables.cve) if observables and observables.cve \
+                    else Observables.generator(observable_type=ObservableType.CVE, count=1)
+        if field == "file_hash":
+            field_value = random.choice(observables.file_hash) if observables and observables.file_hash \
+                    else Observables.generator(observable_type=ObservableType.SHA256, known=ObservableKnown.BAD,
+                                               count=1)
+        if field == "incident_types":
+            field_value = observables.incident_types if observables and observables.incident_types \
+                else INCIDENTS_TYPES
+        if field == "analysts":
+            field_value = observables.analysts if observables and observables.analysts \
+                else [faker.unique.first_name() for _ in range(10)]
+        if field == "duration":
+            field_value = random.randint(1, 5)
+        if field == "log_id":
+            field_value = faker.uuid4()
+        return field_value
+
+    @classmethod
+    def syslog(cls, count: int, timestamp: Optional[datetime] = None, observables: Optional[Observables] = None,
+               required_fields: Optional[str] = "pid,host,user,unix_process,unix_cmd") -> List[str]:
         """
         Generate fake syslog messages.
 
         Args:
             count: The number of syslog messages to generate.
             timestamp: Optional. The starting timestamp for the syslog messages. If not provided, a random time during
             the past hour from now will be used.
             observables: Optional. An observables object. If not provided, random objservable will be generated
             and used.
+            required_fields: Optional. A list of fields that are required to present in the generated data, whether from
+            observables or randomely.
         Returns:
             A list of syslog messages.
 
         Examples:
             >>> Events.syslog(5)
             ['Jan 01 05:32:48 myhostname sudo[1023]: username : COMMAND ; cat /etc/shadow',
              'Jan 01 05:17:59 myhostname sudo[2019]: username : COMMAND ; find / -name \'*.log\' -exec rm -f {} \\;',
@@ -298,45 +452,43 @@
         syslog_messages = []
         faker = cls._create_faker()
         if timestamp is None:
             timestamp = datetime.now() - timedelta(hours=1)
             timestamp += timedelta(seconds=faker.random_int(min=0, max=3599))
         for i in range(count):
             timestamp += timedelta(seconds=1)
-            pid = faker.random_int(min=1000, max=65535)
-            action = "COMMAND"
-            host = random.choice(observables.src_host) if observables and observables.src_host \
-                else faker.hostname()
-            user = random.choice(observables.user) if observables and observables.user \
-                else faker.user_name()
-            process = random.choice(observables.process) if observables and observables.process \
-                else "sudo"
-            command = random.choice(observables.cmd) if observables and observables.cmd \
-                else random.choice(UNIX_CMD)
-            syslog_messages.append(f"{timestamp.strftime('%Y-%m-%d %H:%M:%S')} {host} {process}[{pid}]: {user}"
-                                   f" : {action} ; {command}")
+            syslog_message = f"{timestamp.strftime('%Y-%m-%d %H:%M:%S')}"
+            for field in required_fields.split(","):
+                syslog_message += f" {cls.set_field(field, observables)}"
+            if observables:
+                for observable, observable_value in vars(observables).items():
+                    if observable_value and observable not in required_fields.split(","):
+                        syslog_message += f" {random.choice(observable_value)}"
+            syslog_messages.append(syslog_message)
         return syslog_messages
 
     @classmethod
     def cef(cls, count: int, vendor: Optional[str] = None, product: Optional[str] = None,
             version: Optional[str] = None, timestamp: Optional[datetime] = None,
-            observables: Optional[Observables] = None) -> List[str]:
+            observables: Optional[Observables] = None, required_fields: Optional[str] = None) -> List[str]:
         """
         Generates fake CEF (Common Event Format) messages.
 
         Args:
             count: The number of CEF messages to generate.
             timestamp: Optional. The starting timestamp for the syslog messages. If not provided, a random time during.
             vendor: Optional. The vendor.
             product: Optional. The product value options include:
             - Firewall
             - EmailGW
             version: Optional. The version.
             observables: Optional. An observables object. If not provided, random objservable will be generated
             and used.
+            required_fields: Optional. A list of fields that are required to present in the generated data, whether from
+            observables or randomely.
         Returns:
             A list of fake CEF messages in string format.
 
         Raises:
             None.
 
         Example Usage:
@@ -354,116 +506,52 @@
         cef_messages = []
         faker = cls._create_faker()
         vendor = vendor or faker.company()
         version = version or faker.numerify("1.0.#")
         if timestamp is None:
             timestamp = datetime.now() - timedelta(hours=1)
             timestamp += timedelta(seconds=faker.random_int(min=0, max=3599))
-        if product == "Firewall":
-            for i in range(count):
-                log_id = faker.uuid4()
-                timestamp += timedelta(seconds=1)
-                severity = random.choice(observables.severity) if observables and observables.severity \
-                    else faker.random_int(min=1, max=5)
-                src_ip = random.choice(observables.src_ip) if observables and observables.src_ip \
-                    else faker.ipv4()
-                src_port = faker.random_int(min=1024, max=65535)
-                dst_ip = random.choice(observables.dst_ip) if observables and observables.dst_ip \
-                    else Observables.generator(observable_type=ObservableType.IP, known=ObservableKnown.BAD, count=1)
-                dst_port = random.choice(observables.port) if observables and observables.port \
-                    else faker.random_int(min=1024, max=65535)
-                dst_url = random.choice(observables.url) if observables and observables.url \
-                    else Observables.generator(observable_type=ObservableType.URL, known=ObservableKnown.BAD, count=1)
-                inbound_bytes = random.choice(observables.inbound_bytes) if observables and observables.inbound_bytes \
-                    else faker.random_int(min=10, max=1073741824)
-                outbound_bytes = random.choice(observables.outbound_bytes) if observables and \
-                    observables.outbound_bytes \
-                    else faker.random_int(min=10, max=1073741824)
-                protocol = random.choice(observables.protocol) if observables and observables.protocol \
-                    else random.choice(PROTOCOLS)
-                rule_id = random.choice(observables.event_id) if observables and observables.event_id \
-                    else faker.random_int(min=1, max=200)
-                action = random.choice(observables.action) if observables and observables.action \
-                    else random.choice(ACTIONS)
-                event_description = f"Firewall {action} {protocol} traffic from {src_ip}:{src_port} to " \
-                                    f"{dst_ip}:{dst_port}"
-                cef_messages.append(f"CEF:0|{vendor}|{product}|{version}|{log_id}|{timestamp}|{severity}|"
-                                    f"{event_description}|src_ip={src_ip} src_port={src_port} dst_ip={dst_ip} "
-                                    f"url={dst_url} dst_port={dst_port} in_bytes={inbound_bytes} "
-                                    f"out_bytes={outbound_bytes} proto={protocol} rule={rule_id} act={action}")
-        elif product == "EmailGW":
-            for i in range(count):
-                mail_id = faker.uuid4()
-                timestamp += timedelta(seconds=1)
-                src_ip = random.choice(observables.src_ip) if observables and observables.src_ip \
-                    else faker.ipv4()
-                src_domain = random.choice(observables.src_domain) if observables and observables.src_domain \
-                    else faker.domain_name()
-                sender_email = random.choice(observables.sender_email) if observables and observables.sender_email \
-                    else faker.email()
-                recipient_email = random.choice(observables.recipient_email) if observables and \
-                    observables.recipient_email else faker.email()
-                email_subject = random.choice(observables.email_subject) if observables and observables.email_subject \
-                    else faker.sentence(nb_words=6)
-                email_body = random.choice(observables.email_body) if observables and observables.email_body else \
-                    faker.sentence(nb_words=50)
-                attachment_hash = random.choice(observables.file_hash) if observables and observables.file_hash \
-                    else Observables.generator(observable_type=ObservableType.SHA256, known=ObservableKnown.BAD,
-                                               count=1)
-                spam_score = faker.random_int(min=1, max=5)
-                action = random.choice(observables.action) if observables and observables.action \
-                    else random.choice(ACTIONS)
-                cef_messages.append(f"CEF:0|{vendor}|{product}|{version}|{mail_id}|{timestamp}|"
-                                    f"src_ip={src_ip} src_domain={src_domain} sender_email={sender_email} "
-                                    f"recipient_email={recipient_email} email_subject={email_subject} "
-                                    f"email_body={email_body} attachment_hash={attachment_hash} spam_score={spam_score}"
-                                    f" action={action}")
-        else:
-            for i in range(count):
-                log_id = faker.uuid4()
-                timestamp += timedelta(seconds=1)
-                severity = random.choice(observables.severity) if observables and observables.severity \
-                    else faker.random_int(min=1, max=5)
-                src_ip = random.choice(observables.src_ip) if observables and observables.src_ip \
-                    else faker.ipv4()
-                src_port = faker.random_int(min=1024, max=65535)
-                dst_ip = random.choice(observables.dst_ip) if observables and observables.dst_ip \
-                    else Observables.generator(observable_type=ObservableType.IP, known=ObservableKnown.BAD, count=1)
-                dst_port = random.choice(observables.port) if observables and observables.port \
-                    else faker.random_int(min=1024, max=65535)
-                protocol = random.choice(observables.protocol) if observables and observables.protocol \
-                    else random.choice(PROTOCOLS)
-                rule_id = random.choice(observables.event_id) if observables and observables.event_id \
-                    else faker.random_int(min=1, max=200)
-                action = random.choice(observables.action) if observables and observables.action \
-                    else random.choice(ACTIONS)
-                generic_cef = f"CEF:0|{vendor}|{product}|{version}|{log_id}|{timestamp}|{severity}|src_ip={src_ip} " \
-                              f"src_port={src_port} dst_ip={dst_ip} dst_port={dst_port} proto={protocol} " \
-                              f"rule={rule_id} act={action}"
-                if observables:
-                    for observable, observable_value in vars(observables).items():
-                        if observable_value:
-                            generic_cef += f" {observable}={random.choice(observable_value)}"
-                cef_messages.append(generic_cef)
+        if not required_fields:
+            if product == "Firewall":
+                required_fields = "local_ip,local_port,remote_ip,remote_port,dst_url,inbound_bytes," \
+                          "outbound_bytes,protocol,rule_id,action"
+            elif product == "EmailGW":
+                required_fields = "local_ip,src_domain,sender_email,recipient_email,email_subject,email_body," \
+                                  "attachment_hash,spam_score,action"
+            else:
+                required_fields = "local_ip,local_port,remote_ip,remote_port,protocol,rule_id,action"
+        for i in range(count):
+            timestamp += timedelta(seconds=1)
+            cef_message = f"CEF:0|{vendor}|{product}|{version}|{cls.set_field('log_id', observables)}|{timestamp}" \
+                          f"|{cls.set_field('severity', observables)}|"
+            for field in required_fields.split(","):
+                cef_message += f" {field}={cls.set_field(field, observables)}"
+            if observables:
+                for observable, observable_value in vars(observables).items():
+                    if observable_value and observable not in required_fields.split(","):
+                        cef_message += f" {observable}={random.choice(observable_value)}"
+            cef_messages.append(cef_message)
         return cef_messages
 
     @classmethod
     def leef(cls, count, timestamp: Optional[datetime] = None, vendor: Optional[str] = None,
              product: Optional[str] = None, version: Optional[str] = None,
-             observables: Optional[Observables] = None) -> List[str]:
+             observables: Optional[Observables] = None, required_fields: Optional[str] = None) -> List[str]:
         """
         Generates fake LEEF (Log Event Extended Format) messages.
 
         Parameters:
             count (int): The number of LEEF messages to generate.
             timestamp: Optional. The starting timestamp for the syslog messages. If not provided, a random time during.
             vendor: Optional. The vendor.
             product: Optional. The product.
             version: Optional. The version.
             observables: An observables object. If not provided, random objservable will be generated and used.
+            required_fields: Optional. A list of fields that are required to present in the generated data, whether from
+            observables or randomely.
 
         Returns:
             A list of generated LEEF messages.
 
         Example:
             To generate 10 fake LEEF messages:
             ```
@@ -482,77 +570,31 @@
         leef_messages = []
         faker = cls._create_faker()
         vendor = vendor or faker.company()
         version = version or faker.numerify("1.0.#")
         if timestamp is None:
             timestamp = datetime.now() - timedelta(hours=1)
             timestamp += timedelta(seconds=faker.random_int(min=0, max=3599))
-        if product == "WAF":
-            for i in range(count):
-                timestamp += timedelta(seconds=1)
-                severity = random.choice(observables.severity) if observables and observables.severity \
-                    else faker.random_int(min=1, max=5)
-                src_ip = random.choice(observables.src_ip) if observables and observables.src_ip \
-                    else faker.ipv4()
-                src_port = faker.random_int(min=1024, max=65535)
-                host = random.choice(observables.src_host) if observables and observables.src_host \
-                    else faker.hostname()
-                method = random.choice(observables.technique).get('mechanism') if observables and observables.technique \
-                    else random.choice(TECHNIQUES).get('mechanism')
-                url = random.choice(observables.technique).get('indicator') if observables and observables.technique \
-                    else random.choice(TECHNIQUES).get('indicator')
-                protocol = random.choice(observables.protocol) if observables and observables.protocol \
-                    else random.choice(PROTOCOLS)
-                user_agent = faker.user_agent()
-                referer = random.choice(observables.url) if observables and observables.url \
-                    else Observables.generator(observable_type=ObservableType.URL, known=ObservableKnown.BAD, count=1)
-                response_code = random.choice(observables.error_code) if observables and observables.error_code \
-                    else random.choice(ERROR_CODE)
-                response_size = faker.random_int(min=100, max=10000)
-                rule_id = random.choice(observables.event_id) if observables and observables.event_id \
-                    else faker.random_int(min=1, max=200)
-                action = random.choice(observables.action) if observables and observables.action \
-                    else random.choice(ACTIONS)
-                attack_type = random.choice(observables.technique).get('technique') if observables and \
-                    observables.technique else random.choice(TECHNIQUES).get('technique')
-                cookie_name = faker.word()
-                cookie_value = faker.uuid4()
-                cookies = f"{cookie_name}={cookie_value}"
-                leef_log = f"LEEF:1.0|{vendor}|{product}|{version}|deviceEventDate={timestamp}|{faker.ipv4()}|{host}|"
-                leef_log += f"src_ip={src_ip} src_port={src_port} request_url={url} method={method} referer={referer} "
-                leef_log += f"protocol={protocol} status={str(response_code)} action={action} attack_type={attack_type}"
-                leef_log += f" response_size={response_size} rule_id={rule_id} user_agent={user_agent} "
-                leef_log += f"severity={severity} cookie={cookies}"
-                leef_messages.append(leef_log)
-        else:
-            for i in range(count):
-                timestamp += timedelta(seconds=1)
-                severity = random.choice(observables.severity) if observables and observables.severity \
-                    else faker.random_int(min=1, max=5)
-                src_ip = random.choice(observables.src_ip) if observables and observables.src_ip \
-                    else faker.ipv4()
-                src_port = faker.random_int(min=1024, max=65535)
-                host = random.choice(observables.src_host) if observables and observables.src_host \
-                    else faker.hostname()
-                url = random.choice(observables.technique).get('indicator') if observables and observables.technique \
-                    else random.choice(TECHNIQUES).get('indicator')
-                protocol = random.choice(observables.protocol) if observables and observables.protocol \
-                    else random.choice(PROTOCOLS)
-                response_code = random.choice(observables.error_code) if observables and observables.error_code \
-                    else random.choice(ERROR_CODE)
-                action = random.choice(observables.action) if observables and observables.action \
-                    else random.choice(ACTIONS)
-                leef_log = f"LEEF:1.0|{vendor}|{product}|{version}|deviceEventDate={timestamp}|{faker.ipv4()}|{host}|"
-                leef_log += f"src_ip={src_ip} src_port={src_port} request_url={url} protocol={protocol} "
-                leef_log += f"status={str(response_code)} action={action} severity={severity}"
-                if observables:
-                    for observable, observable_value in vars(observables).items():
-                        if observable_value:
-                            leef_log += f" {observable}={random.choice(observable_value)}"
-                leef_messages.append(leef_log)
+        if not required_fields:
+            if product == "WAF":
+                required_fields = "local_ip,local_port,host,method,url,protocol," \
+                                  "user_agent,referer,response_code,response_size,rule_id,action,attack_type,cookies"
+            else:
+                required_fields = "local_ip,local_port,host,url,protocol,response_code,action"
+        for i in range(count):
+            timestamp += timedelta(seconds=1)
+            leef_message = f"LEEF:1.0|{vendor}|{product}|{version}|deviceEventDate={timestamp}|" \
+                           f"severity={cls.set_field('severity', observables)}|"
+            for field in required_fields.split(","):
+                leef_message += f" {field}={cls.set_field(field, observables)}"
+            if observables:
+                for observable, observable_value in vars(observables).items():
+                    if observable_value and observable not in required_fields.split(","):
+                        leef_message += f" {observable}={random.choice(observable_value)}"
+            leef_messages.append(required_fields)
         return leef_messages
 
     @classmethod
     def winevent(cls, count, timestamp: Optional[datetime] = None, observables: Optional[Observables] = None) -> \
             List[str]:
         """
         Generates fake Windows Event Log messages.
@@ -573,15 +615,15 @@
         faker = cls._create_faker()
         if timestamp is None:
             timestamp = datetime.now() - timedelta(hours=1)
             timestamp += timedelta(seconds=faker.random_int(min=0, max=3599))
         for i in range(count):
             timestamp += timedelta(seconds=1)
             guid = faker.uuid4()
-            src_port = faker.random_int(min=1024, max=65535)
+            local_port = faker.random_int(min=1024, max=65535)
             transmitted_services = faker.sentence(nb_words=5)
             system_time = timestamp
             process_id = faker.random_int()
             new_process_id = faker.random_int()
             thread_id = faker.random_int()
             target_pid = faker.random_int()
             domain_name = faker.domain_name()
@@ -595,45 +637,48 @@
                 else random.choice(WIN_PROCESSES)
             host = random.choice(observables.src_host) if observables and observables.src_host \
                 else faker.hostname()
             user_name = random.choice(observables.user) if observables and observables.user \
                 else faker.user_name()
             cmd = random.choice(observables.cmd) if observables and observables.cmd \
                 else random.choice(WINDOWS_CMD)
-            source_network_address = random.choice(observables.src_ip) if observables and observables.src_ip \
+            source_network_address = random.choice(observables.local_ip) if observables and observables.local_ip \
                 else faker.ipv4_private()
             file_name = random.choice(observables.file_name) if observables and observables.file_name \
                 else faker.file_name()
             unformatted_event = random.choice(WIN_EVENTS)
             win_event = unformatted_event.format(guid=guid, system_time=system_time, event_record_id=event_record_id,
                                                  process_id=process_id, process_name=process_name,
                                                  new_process_id=new_process_id, thread_id=thread_id,
                                                  target_pid=target_pid, host=host, user_id=user_id, user_name=user_name,
                                                  domain_name=domain_name, subject_login_id=subject_login_id,
                                                  privilege_list=privilege_list, cmd=cmd,
                                                  destination_login_id=destination_login_id,
-                                                 source_network_address=source_network_address, source_port=src_port,
+                                                 source_network_address=source_network_address, source_port=local_port,
                                                  transmitted_services=transmitted_services, file_name=file_name)
             winevent_messages.append(win_event)
         return winevent_messages
 
     @classmethod
     def json(cls, count, timestamp: Optional[datetime] = None, vendor: Optional[str] = None,
-             product: Optional[str] = None, version: Optional[str] = None, observables: Optional[Observables] = None) -> List[dict]:
+             product: Optional[str] = None, version: Optional[str] = None, observables: Optional[Observables] = None,
+             required_fields: Optional[str] = None) -> List[dict]:
         """
         Generate fake JSON messages representing discovered vulnerabilities.
 
         Args:
             count (int): The number of JSON messages to generate.
             timestamp: Optional. The starting timestamp for the syslog messages. If not provided, a random time during.
             vendor: Optional. The vendor.
             product: Optional. The product value options include:
             - VulnScanner
             version: Optional. The version.
             observables: An observables object. If not provided, random objservable will be generated and used.
+            required_fields: Optional. A list of fields that are required to present in the generated data, whether from
+            observables or randomely.
         Returns:
             List[Dict[str, Union[str, int]]]: A list of dictionaries representing the generated JSON messages.
 
         Example:
             >>> fake_messages = json(5)
             >>> len(fake_messages)
             5
@@ -644,62 +689,34 @@
         json_messages = []
         faker = cls._create_faker()
         vendor = vendor or faker.company()
         version = version or faker.numerify("1.0.#")
         if timestamp is None:
             timestamp = datetime.now() - timedelta(hours=1)
             timestamp += timedelta(seconds=faker.random_int(min=0, max=3599))
-        if product == "VulnScanner":
-            for i in range(count):
-                timestamp += timedelta(seconds=1)
-                system_time = timestamp.strftime('%Y-%m-%d %H:%M:%S')
-                cve_id = random.choice(observables.cve) if observables and observables.cve \
-                    else Observables.generator(observable_type=ObservableType.CVE, count=1)
-                host = random.choice(observables.src_host) if observables and observables.src_host \
-                    else faker.hostname()
-                severity = random.choice(observables.severity) if observables and observables.severity \
-                    else faker.random_int(min=1, max=5)
-                file_hash = random.choice(observables.file_hash) if observables and observables.file_hash \
-                    else Observables.generator(observable_type=ObservableType.SHA256, known=ObservableKnown.BAD, count=1)
-                event = {
-                    'vendor': vendor,
-                    'product': product,
-                    'version': version,
-                    'event_type': 'vulnerability_discovered',
-                    'timestamp': system_time,
-                    'severity': severity,
-                    'host': host,
-                    'file_hash': file_hash,
-                    'cve': cve_id
-                }
-                json_messages.append(event)
-        else:
-            for i in range(count):
-                timestamp += timedelta(seconds=1)
-                system_time = timestamp.strftime('%Y-%m-%d %H:%M:%S')
-                user = random.choice(observables.user) if observables and observables.user \
-                    else faker.user_name()
-                host = random.choice(observables.src_host) if observables and observables.src_host \
-                    else faker.hostname()
-                severity = random.choice(observables.severity) if observables and observables.severity \
-                    else faker.random_int(min=1, max=5)
-                event = {
-                    'vendor': vendor,
-                    'product': product,
-                    'version': version,
-                    'timestamp': system_time,
-                    'severity': severity,
-                    'host': host,
-                    'user': user
-                }
-                if observables:
-                    for observable, observable_value in vars(observables).items():
-                        if observable_value:
-                            event[observable] = random.choice(observable_value)
-                json_messages.append(event)
+        if not required_fields:
+            if product == "VulnScanner":
+                required_fields = "cve_id,host,file_hash"
+            else:
+                required_fields = "user,host"
+        for i in range(count):
+            timestamp += timedelta(seconds=1)
+            event = {
+                'vendor': vendor,
+                'product': product,
+                'version': version,
+                'severity': cls.set_field("severity", observables)
+            }
+            for field in required_fields.split(","):
+                event[field] = cls.set_field(field, observables)
+            if observables:
+                for observable, observable_value in vars(observables).items():
+                    if observable_value and observable not in required_fields.split(","):
+                        event[observable] = random.choice(observable_value)
+            json_messages.append(event)
         return json_messages
 
     @classmethod
     def incidents(cls, count, fields: Optional[str] = None, timestamp: Optional[datetime] = None,
                   vendor: Optional[str] = None, product: Optional[str] = None, version: Optional[str] = None,
                   observables: Optional[Observables] = None) -> List[dict]:
         """
@@ -746,15 +763,14 @@
         analysts = observables.analysts if observables and observables.analysts \
             else [faker.unique.first_name() for _ in range(10)]
         analyst_incident_map = {}
         for analyst in analysts:
             mapped_incident_type = incident_types.pop(0)
             analyst_incident_map[analyst] = mapped_incident_type
             incident_types.append(mapped_incident_type)
-
         for i in range(count):
             incident = {}
             duration = random.randint(1, 5)
             while True:
                 incident_id = random.randint(1, count)
                 if incident_id not in incident_ids:
                     incident_ids.add(incident_id)
```

### Comparing `rosetta-ce-1.4.0/rosetta/rsender.py` & `rosetta-ce-1.4.1/rosetta/rsender.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.0/rosetta_ce.egg-info/PKG-INFO` & `rosetta-ce-1.4.1/rosetta_ce.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosetta-ce
-Version: 1.4.0
+Version: 1.4.1
 Summary: Rosetta is a Python package that can be used to fake security logs and alerts for testing different detection and response use cases.
 Home-page: https://github.com/ayman-m/rosetta
 Author: Ayman Mahmoud
 Author-email: content@ayman.online
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rosetta-ce-1.4.0/setup.py` & `rosetta-ce-1.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rosetta-ce",
-    version="1.4.0",
+    version="1.4.1",
     author="Ayman Mahmoud",
     author_email="content@ayman.online",
     description="Rosetta is a Python package that can be used to fake security logs and alerts for testing different "
                 "detection and response use cases.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ayman-m/rosetta",
```

### Comparing `rosetta-ce-1.4.0/tests/test_rconverter.py` & `rosetta-ce-1.4.1/tests/test_rconverter.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.0/tests/test_rfaker.py` & `rosetta-ce-1.4.1/tests/test_rfaker.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.0/tests/test_rsender.py` & `rosetta-ce-1.4.1/tests/test_rsender.py`

 * *Files identical despite different names*

