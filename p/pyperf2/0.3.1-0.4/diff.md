# Comparing `tmp/pyperf2-0.3.1-py3-none-any.whl.zip` & `tmp/pyperf2-0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 11357 bytes, number of entries: 6
--rw-r--r--  2.0 unx    25016 b- defN 23-Jun-25 23:32 pyperf2/__init__.py
--rwxr-xr-x  2.0 unx    11357 b- defN 23-Jun-25 23:38 pyperf2-0.3.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     3340 b- defN 23-Jun-25 23:38 pyperf2-0.3.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-25 23:38 pyperf2-0.3.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jun-25 23:38 pyperf2-0.3.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      463 b- defN 23-Jun-25 23:38 pyperf2-0.3.1.dist-info/RECORD
-6 files, 40276 bytes uncompressed, 10523 bytes compressed:  73.9%
+Zip file size: 11468 bytes, number of entries: 6
+-rw-r--r--  2.0 unx    26391 b- defN 23-Jun-26 06:20 pyperf2/__init__.py
+-rwxr-xr-x  2.0 unx    11357 b- defN 23-Jul-02 09:16 pyperf2-0.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3338 b- defN 23-Jul-02 09:16 pyperf2-0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-02 09:16 pyperf2-0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-02 09:16 pyperf2-0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      453 b- defN 23-Jul-02 09:16 pyperf2-0.4.dist-info/RECORD
+6 files, 41639 bytes uncompressed, 10654 bytes compressed:  74.4%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: pyperf2/__init__.py
 Comment: 
 
-Filename: pyperf2-0.3.1.dist-info/LICENSE
+Filename: pyperf2-0.4.dist-info/LICENSE
 Comment: 
 
-Filename: pyperf2-0.3.1.dist-info/METADATA
+Filename: pyperf2-0.4.dist-info/METADATA
 Comment: 
 
-Filename: pyperf2-0.3.1.dist-info/WHEEL
+Filename: pyperf2-0.4.dist-info/WHEEL
 Comment: 
 
-Filename: pyperf2-0.3.1.dist-info/top_level.txt
+Filename: pyperf2-0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: pyperf2-0.3.1.dist-info/RECORD
+Filename: pyperf2-0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyperf2/__init__.py

```diff
@@ -11,26 +11,27 @@
 from decimal import Decimal
 from pprint import pprint, pformat
 import logging
 import datetime
 from pyroute2 import netns
 
 
-
 def output_reader(proc, outq, parent):
     for line in iter(proc.stdout.readline, b""):
         outq.put(line.decode("utf-8"))
 
         # print("{0} {1}".format(parent.name,line.decode('utf-8')))
 
         parent.line_ready_callback()
 
+
 class NameSpaceNotFoundError(Exception):
     pass
 
+
 class IPerfInstance(object):
     def __init__(self):
         self.type = None
         self.report_interval = "1"
         self.protocol = "tcp"
         self.iperf_binary_path = "/usr/bin/iperf"
         self._outq = queue.Queue()
@@ -55,15 +56,15 @@
         self._on_packetloss_callbacks = []
         self.currently_has_loss = {}
         self._output_reader_thread = None
         self._cleanup_timer_thread = None
         self._raw_log_filepath = None
         self._raw_log_filehandler = None
         self._creation_time = datetime.datetime.now().replace(microsecond=0).isoformat()
-        self.ttl=255
+        self.ttl = 255
 
         if "pps" in self.bandwidth:
             self.expected_interval_packets = int(
                 Decimal(self.report_interval) * Decimal(self.bandwidth[:-3])
             )
         else:
             self.expected_interval_packets = None
@@ -97,16 +98,19 @@
         packet_loss_event_message = False
         report_message = False
         timestamp = datetime.datetime.now().isoformat()
         if self._raw_log_filehandler:
             self._raw_log_filehandler.write(line)
             self._raw_log_filehandler.flush()
         if not self._info_regex:
-            raise RuntimeError("missing regex for parsing output",pformat(self.generate_cli_from_options()))
-        
+            raise RuntimeError(
+                "missing regex for parsing output",
+                pformat(self.generate_cli_from_options()),
+            )
+
         result = self._info_regex.match(line)  # check if it's an info header
         if result:
             info_data = result.groupdict()
             stream_id = info_data["stream_id"]
             if (
                 stream_id not in self._results
             ):  # new stream id detected -> create new result structure
@@ -116,14 +120,16 @@
                     "info": result.groupdict(),
                     "events": [],
                     "timestamp": timestamp,
                 }
                 self.currently_has_loss[stream_id] = False
 
         result = self._result_regex.match(line)  # check if it's a report line
+        
+        
         if result:
             report_data = result.groupdict()
             stream_id = report_data["stream_id"]
 
             interval_begin = Decimal(report_data["interval_begin"])
             interval_end = Decimal(report_data["interval_end"])
             if "packets_lost" in report_data:
@@ -143,14 +149,20 @@
             if (
                 last_interval_begin > interval_begin
             ):  # if it's a summary store it and return
                 self._results[stream_id]["summary"] = result.groupdict()
                 self._log.debug("got summary result")
                 return True  # suppress any message for summary
 
+            if is_sender:
+                report_message = copy.copy(report_data)
+                report_message["stream_name"] = self.name
+
+
+
             if is_receiver:
                 report_message = copy.copy(report_data)
                 report_message["stream_name"] = self.name
 
                 if packets_received < self.expected_interval_packets:
                     probably_packets_lost = (
                         self.expected_interval_packets - packets_received
@@ -436,26 +448,34 @@
                 retval[k] = v
         return retval
 
     def generate_cli_from_options(self):
         _cli = []
         if self.use_linux_namespace:
             if self.use_linux_namespace not in list(netns.listnetns()):
-                raise NameSpaceNotFoundError(f"Namespace {self.use_linux_namespace} cannot be found.")
+                raise NameSpaceNotFoundError(
+                    f"Namespace {self.use_linux_namespace} cannot be found."
+                )
             _cli.extend("ip netns exec {0}".format(self.use_linux_namespace).split(" "))
         _cli.append(self.iperf_binary_path)
         _cli.append("-e")
         if self.test_duration:
             _cli.append("-t")
             _cli.append(self.test_duration)
         if self.type == "server":
             _cli.append("-s")
             if self.bind_ip:
                 _cli.append("-B")
                 _cli.append(self.bind_ip)
+            ####Ü
+            if self.protocol == "tcp":
+                self._result_regex = re.compile(
+                    r"^\[\s*(?P<stream_id>\d+)\]\s+(?P<interval_begin>\d+\.\d+)-(?P<interval_end>\d+\.\d+)\s+(?P<interval_unit>\S+)\s+(?P<received>\S+)\s+(?P<received_unit>\S+)\s+(?P<bandwidth>\S+)\s+(?P<bandwidth_unit>\S+)?"
+                )
+
             if self.protocol == "udp":
                 # multicast server result
                 # [  4] 2.6000-2.7000 sec  0.00 Bytes   0.00 bits/sec    0.000 ms    0/    0 (0%)  -/-/-/-                    ms    0 pps
                 # [  3] 8.7000-8.8000 sec   144 KBytes  11.8 Mbits/sec   0.002 ms    0/  100 (0%)  0.015/ 0.008/ 0.037/ 0.006 ms 1000 pps  100753.94
                 self._result_regex = re.compile(
                     r"^\[\s*(?P<stream_id>\d+)\]\s+(?P<interval_begin>\d+\.\d+)-(?P<interval_end>\d+\.\d+)\s+(?P<interval_unit>\S+)\s+(?P<received>\S+)\s+(?P<received_unit>\S+)\s+(?P<bandwidth>\S+)\s+(?P<bandwidth_unit>\S+)\s+(?P<jitter>\S+)\s+(?P<jitter_unit>\S+)\s+(?P<packets_lost>\S+)/\s*(?P<packets_received>\S+)\s+\(.*\)\s+(?P<latency_avg>\S+)\s*/\s*(?P<latency_min>\S+)\s*/\s*(?P<latency_max>\S+)\s*/\s*(?P<latency_stdev>\S+)\s+(?P<latency_unit>\S+)\s+(?P<packet_rate>\d+)\s+(?P<packet_rate_unit>\S+)\s*(?P<net_pwr>\S+)?"
                 )
@@ -465,40 +485,53 @@
             if not self.server_ip:
                 raise ValueError("Client needs server_ip to be set")
             _cli.append(self.server_ip)
             if self.bind_ip and self.client_source_port:
                 _cli.append("-B")
                 _cli.append("{0}:{1}".format(self.bind_ip, self.client_source_port))
             if self.protocol == "udp":
-                _cli.append("-l")
-                _cli.append(self.packet_len)
                 # [  3] local 192.168.51.154 port 54877 connected with 225.0.0.5 port 5001
                 self._result_regex = re.compile(
                     r"^\[\s*(?P<stream_id>\d+)\]\s+(?P<interval_begin>\d+\.\d+)-(?P<interval_end>\d+\.\d+)\s+(?P<interval_unit>\S+)\s+(?P<transferred>\S+)\s+(?P<transferred_unit>\S+)\s+(?P<bandwidth>\S+)\s+(?P<bandwidth_unit>\S+)\s+(?P<packets_written>\S+)/(?P<packets_error>\S+)\s+(?P<packet_rate>\d+)\s+(?P<packet_rate_unit>\S+)"
                 )
+            if self.protocol == "tcp":
+                self._result_regex = re.compile(
+                    r"^\[\s*(?P<stream_id>\d+)\]\s+(?P<interval_begin>\d+\.\d+)-(?P<interval_end>\d+\.\d+)\s+(?P<interval_unit>\S+)\s+(?P<transferred>\S+)\s+(?P<transferred_unit>\S+)\s+(?P<bandwidth>\S+)\s+(?P<bandwidth_unit>\S+)\s+(?P<packets_written>\S+)/(?P<packets_error>\S+)\s+(?P<retry>\d+)\s+(?P<cwnd>\S+)/(?P<rtt>\d+)\S(?P<var>\d+)\W*(?P<var_unit>\S+)\W*(?P<netpower>\d+\S*)"
+                )
+            if self.packet_len:
+                _cli.append("-l")
+                _cli.append(self.packet_len)
             if self.ttl:
                 _cli.append("-T")
                 _cli.append(str(self.ttl))
 
         else:
             raise ValueError("type must be set to either server or client")
         if self.protocol == "udp":
             _cli.append("-u")
+        if self.protocol == "udp" or "tcp":
             self._info_regex = re.compile(
                 r"^\[\s*(?P<stream_id>\d+)\]\s+local\s+(?P<local_ip>\S+)\s+port\s+(?P<local_port>\S+)\s+connected\s+with\s+(?P<remote_ip>\S+)\s+port\s+(?P<remote_port>\S+)"
             )
             #
         if self.realtime:
             _cli.append("-z")
 
         _cli.append("-i")
         _cli.append(self.report_interval)
 
         _cli.append("-b")
-        _cli.append(self.bandwidth)
+        if self.protocol == "tcp":
+            if "pps" not in self.bandwidth:
+                _cli.append(self.bandwidth)
+            else:
+                _cli.append("1M")
+
+        if self.protocol == "udp":
+            _cli.append(self.bandwidth)
 
         _cli.append("-p")
         _cli.append(self.port)
 
         if self.dscp:
             accepted_tos_values = [
                 "af11",
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `pyperf2-0.3.1.dist-info/LICENSE` & `pyperf2-0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyperf2-0.3.1.dist-info/METADATA` & `pyperf2-0.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyperf2
-Version: 0.3.1
+Version: 0.4
 Summary: Abstraction layer for iperf2 linux binary
 Home-page: https://github.com/jinjamator/pyperf2
 Author: Wilhelm Putz
 Author-email: wp@aci.guru
 License: ASL V2
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

