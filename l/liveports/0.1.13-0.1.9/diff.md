# Comparing `tmp/liveports-0.1.13.tar.gz` & `tmp/liveports-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liveports-0.1.13.tar", last modified: Sat Jul  1 22:22:12 2023, max compression
+gzip compressed data, was "liveports-0.1.9.tar", last modified: Tue Jun  6 07:02:51 2023, max compression
```

## Comparing `liveports-0.1.13.tar` & `liveports-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-01 22:22:12.512221 liveports-0.1.13/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       39 2023-06-06 12:57:43.000000 liveports-0.1.13/MANIFEST.in
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      450 2023-07-01 22:22:12.512221 liveports-0.1.13/PKG-INFO
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      204 2023-06-04 16:55:25.000000 liveports-0.1.13/README.md
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-01 22:22:12.512221 liveports-0.1.13/liveports/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-06-02 16:32:43.000000 liveports-0.1.13/liveports/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3351 2023-06-13 08:37:52.000000 liveports-0.1.13/liveports/blaster_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    13169 2023-07-01 22:21:35.000000 liveports-0.1.13/liveports/client.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6235 2023-06-04 15:53:56.000000 liveports-0.1.13/liveports/logviewer.html
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-01 22:22:12.512221 liveports-0.1.13/liveports.egg-info/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      450 2023-07-01 22:22:12.000000 liveports-0.1.13/liveports.egg-info/PKG-INFO
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      331 2023-07-01 22:22:12.000000 liveports-0.1.13/liveports.egg-info/SOURCES.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        1 2023-07-01 22:22:12.000000 liveports-0.1.13/liveports.egg-info/dependency_links.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       53 2023-07-01 22:22:12.000000 liveports-0.1.13/liveports.egg-info/entry_points.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       16 2023-07-01 22:22:12.000000 liveports-0.1.13/liveports.egg-info/requires.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       10 2023-07-01 22:22:12.000000 liveports-0.1.13/liveports.egg-info/top_level.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       91 2023-06-06 12:59:07.000000 liveports-0.1.13/run.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       38 2023-07-01 22:22:12.512221 liveports-0.1.13/setup.cfg
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      623 2023-07-01 22:21:49.000000 liveports-0.1.13/setup.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-06 07:02:51.429820 liveports-0.1.9/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       25 2023-06-05 08:38:22.000000 liveports-0.1.9/MANIFEST.in
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      449 2023-06-06 07:02:51.429820 liveports-0.1.9/PKG-INFO
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      204 2023-06-04 16:55:25.000000 liveports-0.1.9/README.md
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-06 07:02:51.429820 liveports-0.1.9/liveports/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-06-02 16:32:43.000000 liveports-0.1.9/liveports/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3467 2023-06-06 07:01:01.000000 liveports-0.1.9/liveports/blaster_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    12793 2023-06-06 07:01:01.000000 liveports-0.1.9/liveports/client.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6235 2023-06-04 15:53:56.000000 liveports-0.1.9/liveports/logviewer.html
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-06 07:02:51.429820 liveports-0.1.9/liveports.egg-info/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      449 2023-06-06 07:02:51.000000 liveports-0.1.9/liveports.egg-info/PKG-INFO
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      324 2023-06-06 07:02:51.000000 liveports-0.1.9/liveports.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        1 2023-06-06 07:02:51.000000 liveports-0.1.9/liveports.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       53 2023-06-06 07:02:51.000000 liveports-0.1.9/liveports.egg-info/entry_points.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       33 2023-06-06 07:02:51.000000 liveports-0.1.9/liveports.egg-info/requires.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       10 2023-06-06 07:02:51.000000 liveports-0.1.9/liveports.egg-info/top_level.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       38 2023-06-06 07:02:51.429820 liveports-0.1.9/setup.cfg
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      677 2023-06-06 07:00:03.000000 liveports-0.1.9/setup.py
```

### Comparing `liveports-0.1.13/liveports/blaster_utils.py` & `liveports-0.1.9/liveports/blaster_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,38 +9,44 @@
 	pass
 
 
 # UTILITIES COPIED FROM BLASTER SERVER CODE
 def parse_cmd_line_arguments():
 	from sys import argv
 	args = []
-	args_map = {}
+	args_map = {
+		"args": args
+	}
 	i = 0
 	num_args = len(argv)
 	while(i < num_args):
 		arg = argv[i]
-		if(arg.startswith("-")):
+		if(arg.startswith("--")):
 			if("=" in arg):
 				key, val = arg.split("=", 1)
 				args_map[key.lstrip("-")] = val
 			else:
-				next_arg = True
-				if(i + 1 < num_args and not argv[i + 1].startswith("-")):
-					next_arg = argv[i + 1]
-					i += 1
-				args_map[arg.lstrip("-")] = next_arg
+				args_map[arg.lstrip("-")] = True
+		elif(arg.startswith("-")):  # Flags
+			key = arg.lstrip("-")
+			# if next argument doesn't start with - its considered as value
+			val = True
+			if (i + 1 < num_args and argv[i + 1][0] != "-"):
+				val = argv[i + 1]
+				i += 1
+			args_map[key] = val
 		else:
 			args.append(arg)
 
 		i += 1
-	return args, args_map
+	return args_map
 
 
 # PARSE COMMAND LINE ARGUMENTS BY DEFAULT
-CommandLineArgs, CommandLineNamedArgs = parse_cmd_line_arguments()
+CommandLineArgs = parse_cmd_line_arguments()
 
 
 def run_shell(cmd, output_parser=None, shell=False, max_buf=5000, fail=True, state=None, env=None, **kwargs):
 
 	state = state if state != None else DummyObject()
 	state.total_output = ""
 	state.total_err = ""
```

### Comparing `liveports-0.1.13/liveports/client.py` & `liveports-0.1.9/liveports/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,69 +1,68 @@
 import socket
 import signal
 import time
 import brotli
 import tempfile
 import zlib
 from urllib.parse import urlparse
-import urllib.request as requester
+import requests
 from collections import deque
 import os
 import gzip
 import sys
 import ssl
 import json
 import threading
 import http.server
 import http.client
 import urllib
 import socketserver
 import fcntl
-from .blaster_utils import run_shell, CommandLineNamedArgs, CommandLineArgs,\
-	DummyObject, nsplit
+from .blaster_utils import run_shell, CommandLineArgs, DummyObject, nsplit
 
-__version__ = "0.1.13"
+requests.packages.urllib3.disable_warnings()
 
 ssl_context = ssl.create_default_context()
 ssl_context.check_hostname = False
 ssl_context.verify_mode = ssl.CERT_NONE
 
-socketserver.ThreadingTCPServer.allow_reuse_address = True
+socketserver.TCPServer.allow_reuse_address = True
 
 # Process command line arguments
 try:
-	SOURCE = CommandLineNamedArgs.get("source", "")  # given domain
+	SOURCE = CommandLineArgs.get("source", "")  # given domain
 
 	# If request logging enabled, we will use a proxy server to log request/response
-	LOCAL_PROXY_PORT = int(CommandLineNamedArgs.get("proxyPort", 4060))
-	LOG_VIEWER_PORT = int(CommandLineNamedArgs.get("logViewerPort") or (LOCAL_PROXY_PORT + 1))
-	DEBUG_LOG_LEVEL = int(CommandLineNamedArgs.get("logLevel") or 0)
+	LOCAL_PROXY_PORT = int(CommandLineArgs.get("proxyPort", 4060))
+	LOG_VIEWER_PORT = int(CommandLineArgs.get("logViewerPort") or (LOCAL_PROXY_PORT + 1))
+	DEBUG_LOG_LEVEL = int(CommandLineArgs.get("logLevel") or 0)
 	# target
 	TARGET_HOST = "localhost"
-	if(target_host := CommandLineNamedArgs.get("target")):
+	if(target_host := CommandLineArgs.get("target")):
 		TARGET_PROTOCOL = urlparse(target_host).scheme or "http"
 		TARGET_PORT = urlparse(target_host).port or (80 if TARGET_PROTOCOL == "http" else 443)
 		TARGET_HOST = urlparse(target_host).hostname or "localhost"
 	else:
-		TARGET_PORT = int(CommandLineNamedArgs.get("targetPort") or CommandLineArgs[-1])
+		TARGET_PORT = int(CommandLineArgs.get("targetPort") or CommandLineArgs["args"][-1])
 		TARGET_PROTOCOL = (
-			CommandLineNamedArgs.get("targetProtocol")
-			or (CommandLineArgs[1] if len(CommandLineArgs) > 1 else "http")
+			CommandLineArgs.get("targetProtocol")
+			or (CommandLineArgs["args"][1] if len(CommandLineArgs["args"]) > 1 else "http")
 		).lower()
 
-	NO_PROXY = bool(CommandLineNamedArgs.get("noproxy", False)) and TARGET_HOST == "localhost"  # only when target host is localhost
+	NO_PROXY = bool(CommandLineArgs.get("noproxy", False)) and TARGET_HOST == "localhost"  # only when target host is localhost
 except Exception:
 	print('''
 Invalid Arguments. Usage Examples:
 - liveports http 3000
 - liveports https 8000
 - liveports https 8000 --source="https://yourdomain.com"
 - liveports https 8000 --source="https://yourdomain.com" --noproxy  # for no mediating logging
 - liveports --target="https://localhost:3000" --source="https://yourdomain.com"
-- liveports --target="https://example.com" --source="https://yourdomain.com"
+- liveports --target="https://google.com" --source="https://yourdomain.com"
 ''')
 	sys.exit(1)
 
 if(TARGET_PROTOCOL not in ["http", "https"]):
 	print("Invalid protocol: must be one of http/https", TARGET_PROTOCOL)
 	sys.exit(1)
 
@@ -86,24 +85,22 @@
 
 	@classmethod
 	def start_proxy_server(cls):
 		cls.proxy_server = proxy_server = socketserver.ThreadingTCPServer(("", LOCAL_PROXY_PORT), ProxyHandler)
 		proxy_server.timeout = 5
 		while(Client.is_running):
 			proxy_server.handle_request()
-		cls.proxy_server.server_close()
 		cls.proxy_server = None
 
 	@classmethod
 	def start_log_viewer(cls):
 		cls.log_viewer_server = log_viewer_server = socketserver.ThreadingTCPServer(("", LOG_VIEWER_PORT), LogViewer)
 		log_viewer_server.timeout = 5
 		while(Client.is_running):
 			log_viewer_server.handle_request()
-		cls.log_viewer_server.server_close()
 		cls.log_viewer_server = None
 
 	@staticmethod
 	def ssh_reverse_proxy(server_hostname, server_port, password):
 		echo_password_file = os.path.join(tempfile.gettempdir(), "liveports_echo_pass")
 		open(echo_password_file, "w").write(f"#!/bin/bash\necho \"{password}\"\n")
 		run_shell(f"chmod +x {echo_password_file}", shell=True)
@@ -325,41 +322,36 @@
 	prev_source_config = cache.get(SOURCE) or {}
 	prev_source_config.update(config)
 	cache[SOURCE] = prev_source_config
 	open(SERVER_CACHED_RESP_FILE, "w").write(json.dumps(cache))
 
 
 def main():
-	print(f"v{__version__}")
 	while(not Client.is_stopped):
 
 		lock = open(LOCK_FILE, "w")
 		try:
 			fcntl.flock(lock.fileno(), fcntl.LOCK_EX | fcntl.LOCK_NB)
 
 			prev_resp = get_config().get(SOURCE) or {}
 			server_hostname = prev_resp.get("server_hostname")
-			if(not server_hostname or CommandLineNamedArgs.get("force")):
+			if(not server_hostname or CommandLineArgs.get("force")):
 				server_hostname = "ports.live"
 			server_hostnames_tried = set()
 			while(server_hostname not in server_hostnames_tried):
 				try:
-					resp = json.loads(
-						requester.urlopen(
-							requester.Request(
-								url="https://" + server_hostname + "/api/register",
-								data=json.dumps({
-									"protocol": TARGET_PROTOCOL if NO_PROXY else "http",
-									"target": TARGET_HOST + (f":{TARGET_PORT}" if TARGET_PORT not in (80, 443) else ""),
-									"source": SOURCE,
-									"api_key": CommandLineNamedArgs.get("api_key", prev_resp.get("api_key"))
-								}).encode("utf-8"),
-							)
-						).read().decode("utf-8")
-					)
+					resp = requests.post(
+						"https://" + server_hostname + "/api/register",
+						json={
+							"protocol": TARGET_PROTOCOL if NO_PROXY else "http",
+							"target": TARGET_HOST + (f":{TARGET_PORT}" if TARGET_PORT not in (80, 443) else ""),
+							"source": SOURCE,
+							"api_key": CommandLineArgs.get("api_key", prev_resp.get("api_key"))
+						}
+					).json()
 				except Exception as ex:
 					print(
 						"Sorry there was an error connecting to the server. Please try again in a moment or add \"--force\" to force new hostname"
 					)
 					sys.exit(1)
 
 				if(redirect_to := resp.get("redirect")):
@@ -367,32 +359,27 @@
 					server_hostnames_tried.add(server_hostname)
 				else:
 					break
 
 			# update the previously cached data and cache it
 			save_config(resp)
 
-			if(hints := resp.get("hints")):
-				for k, v in hints.items():
+			if(resp.get("hints")):
+				for k, v in resp["hints"].items():
 					print(v)
 
-				if(hints.get("wait_retry")):
-					print("Reconnecting...")
-					time.sleep(5)
-					continue
-
 			if(resp.get("errors")):
 				for k, v in resp["errors"].items():
 					print(v)
 				sys.exit(1)
 
-			Client.is_running = True
 			server_threads = []
+
+			# START LOGVIEWER SERVER
 			if(not NO_PROXY):
-				# START LOGVIEWER SERVER
 				log_viewer_server = threading.Thread(target=Client.start_log_viewer)
 				log_viewer_server.start()
 				server_threads.append(log_viewer_server)
 				print(f'Log viewer: http://localhost:{LOG_VIEWER_PORT}')
 
 				# START PROXYSERVER
 				proxy_server = threading.Thread(target=Client.start_proxy_server)
@@ -400,14 +387,15 @@
 				server_threads.append(proxy_server)
 
 			print(f'Your public hostname is: https://{resp["public_hostname"]}')
 			print("-------")
 			# START SSH REVERSE PROXY
 			Client.ssh_reverse_proxy(resp["server_hostname"], resp["server_port"], resp["password"])
 
+			# WAIT FOR ALL THREADS STOPPED
 			for _thread in server_threads:
 				_thread.join()
 
 		except IOError:
 			print("Sorry! process may be running already")
 			sys.exit(1)
 		except Exception as ex:
```

### Comparing `liveports-0.1.13/liveports/logviewer.html` & `liveports-0.1.9/liveports/logviewer.html`

 * *Files identical despite different names*

### Comparing `liveports-0.1.13/setup.py` & `liveports-0.1.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,26 @@
+from setuptools import setup
 from setuptools import setup, find_packages
 
-
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='liveports',
-    version='0.1.13',
+    version='0.1.9',
     description='Give address to your localmachine',
     author='Abhinav',
     author_email='abhinavabcd@gmail.com',
-    packages=find_packages(),
+    packages=['liveports'],
     include_package_data=True,
     install_requires=[
+        "requests>=2.23.0",
         "brotlipy>=0.7.0",
     ],
     long_description=long_description,
     long_description_content_type='text/markdown',
     entry_points={
         'console_scripts': [
             'liveports = liveports.client:main',
         ],
-    }
+    },
 )
```

