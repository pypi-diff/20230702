# Comparing `tmp/ICICONSOLEGPT-0.0.5.tar.gz` & `tmp/ICICONSOLEGPT-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ICICONSOLEGPT-0.0.5.tar", last modified: Fri Jun 30 00:17:48 2023, max compression
+gzip compressed data, was "ICICONSOLEGPT-0.0.6.tar", last modified: Sun Jul  2 16:02:20 2023, max compression
```

## Comparing `ICICONSOLEGPT-0.0.5.tar` & `ICICONSOLEGPT-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-06-30 00:17:48.401379 ICICONSOLEGPT-0.0.5/
-drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-06-30 00:17:48.400411 ICICONSOLEGPT-0.0.5/ICICONSOLEGPT/
--rw-r--r--   0 sahilsamar   (501) staff       (20)      882 2023-06-23 17:51:06.000000 ICICONSOLEGPT-0.0.5/ICICONSOLEGPT/BasicCypherCommands.py
--rw-r--r--   0 sahilsamar   (501) staff       (20)      527 2023-06-30 00:13:52.000000 ICICONSOLEGPT-0.0.5/ICICONSOLEGPT/Utilities.py
--rw-r--r--   0 sahilsamar   (501) staff       (20)        0 2023-06-29 23:51:42.000000 ICICONSOLEGPT-0.0.5/ICICONSOLEGPT/__init__.py
--rw-r--r--   0 sahilsamar   (501) staff       (20)    10683 2023-06-30 00:17:12.000000 ICICONSOLEGPT-0.0.5/ICICONSOLEGPT/__main__.py
--rw-r--r--   0 sahilsamar   (501) staff       (20)      428 2023-06-29 22:42:43.000000 ICICONSOLEGPT-0.0.5/ICICONSOLEGPT/helpCypher.json
-drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-06-30 00:17:48.401099 ICICONSOLEGPT-0.0.5/ICICONSOLEGPT.egg-info/
--rw-r--r--   0 sahilsamar   (501) staff       (20)     4015 2023-06-30 00:17:48.000000 ICICONSOLEGPT-0.0.5/ICICONSOLEGPT.egg-info/PKG-INFO
--rw-r--r--   0 sahilsamar   (501) staff       (20)      414 2023-06-30 00:17:48.000000 ICICONSOLEGPT-0.0.5/ICICONSOLEGPT.egg-info/SOURCES.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)        1 2023-06-30 00:17:48.000000 ICICONSOLEGPT-0.0.5/ICICONSOLEGPT.egg-info/dependency_links.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)       59 2023-06-30 00:17:48.000000 ICICONSOLEGPT-0.0.5/ICICONSOLEGPT.egg-info/entry_points.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)       48 2023-06-30 00:17:48.000000 ICICONSOLEGPT-0.0.5/ICICONSOLEGPT.egg-info/requires.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)       14 2023-06-30 00:17:48.000000 ICICONSOLEGPT-0.0.5/ICICONSOLEGPT.egg-info/top_level.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)     1068 2023-06-29 23:15:21.000000 ICICONSOLEGPT-0.0.5/LICENSE
--rw-r--r--   0 sahilsamar   (501) staff       (20)       38 2023-06-29 23:58:53.000000 ICICONSOLEGPT-0.0.5/MANIFEST.in
--rw-r--r--   0 sahilsamar   (501) staff       (20)     4015 2023-06-30 00:17:48.401261 ICICONSOLEGPT-0.0.5/PKG-INFO
--rw-r--r--   0 sahilsamar   (501) staff       (20)     2130 2023-06-30 00:00:47.000000 ICICONSOLEGPT-0.0.5/README.md
--rw-r--r--   0 sahilsamar   (501) staff       (20)     1007 2023-06-30 00:17:23.000000 ICICONSOLEGPT-0.0.5/pyproject.toml
--rw-r--r--   0 sahilsamar   (501) staff       (20)       38 2023-06-30 00:17:48.401414 ICICONSOLEGPT-0.0.5/setup.cfg
+drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-07-02 16:02:20.800277 ICICONSOLEGPT-0.0.6/
+drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-07-02 16:02:20.799179 ICICONSOLEGPT-0.0.6/ICICONSOLEGPT/
+-rw-r--r--   0 sahilsamar   (501) staff       (20)      882 2023-06-23 17:51:06.000000 ICICONSOLEGPT-0.0.6/ICICONSOLEGPT/BasicCypherCommands.py
+-rw-r--r--   0 sahilsamar   (501) staff       (20)      527 2023-06-30 00:13:52.000000 ICICONSOLEGPT-0.0.6/ICICONSOLEGPT/Utilities.py
+-rw-r--r--   0 sahilsamar   (501) staff       (20)        0 2023-06-29 23:51:42.000000 ICICONSOLEGPT-0.0.6/ICICONSOLEGPT/__init__.py
+-rw-r--r--   0 sahilsamar   (501) staff       (20)    13294 2023-07-02 15:58:56.000000 ICICONSOLEGPT-0.0.6/ICICONSOLEGPT/__main__.py
+-rw-r--r--   0 sahilsamar   (501) staff       (20)      428 2023-06-29 22:42:43.000000 ICICONSOLEGPT-0.0.6/ICICONSOLEGPT/helpCypher.json
+drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-07-02 16:02:20.800009 ICICONSOLEGPT-0.0.6/ICICONSOLEGPT.egg-info/
+-rw-r--r--   0 sahilsamar   (501) staff       (20)     4018 2023-07-02 16:02:20.000000 ICICONSOLEGPT-0.0.6/ICICONSOLEGPT.egg-info/PKG-INFO
+-rw-r--r--   0 sahilsamar   (501) staff       (20)      414 2023-07-02 16:02:20.000000 ICICONSOLEGPT-0.0.6/ICICONSOLEGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)        1 2023-07-02 16:02:20.000000 ICICONSOLEGPT-0.0.6/ICICONSOLEGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       59 2023-07-02 16:02:20.000000 ICICONSOLEGPT-0.0.6/ICICONSOLEGPT.egg-info/entry_points.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       48 2023-07-02 16:02:20.000000 ICICONSOLEGPT-0.0.6/ICICONSOLEGPT.egg-info/requires.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       14 2023-07-02 16:02:20.000000 ICICONSOLEGPT-0.0.6/ICICONSOLEGPT.egg-info/top_level.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)     1068 2023-06-29 23:15:21.000000 ICICONSOLEGPT-0.0.6/LICENSE
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       38 2023-06-29 23:58:53.000000 ICICONSOLEGPT-0.0.6/MANIFEST.in
+-rw-r--r--   0 sahilsamar   (501) staff       (20)     4018 2023-07-02 16:02:20.800164 ICICONSOLEGPT-0.0.6/PKG-INFO
+-rw-r--r--   0 sahilsamar   (501) staff       (20)     2133 2023-07-01 02:08:09.000000 ICICONSOLEGPT-0.0.6/README.md
+-rw-r--r--   0 sahilsamar   (501) staff       (20)     1007 2023-07-02 16:02:01.000000 ICICONSOLEGPT-0.0.6/pyproject.toml
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       38 2023-07-02 16:02:20.800311 ICICONSOLEGPT-0.0.6/setup.cfg
```

### Comparing `ICICONSOLEGPT-0.0.5/ICICONSOLEGPT/BasicCypherCommands.py` & `ICICONSOLEGPT-0.0.6/ICICONSOLEGPT/BasicCypherCommands.py`

 * *Files identical despite different names*

### Comparing `ICICONSOLEGPT-0.0.5/ICICONSOLEGPT/Utilities.py` & `ICICONSOLEGPT-0.0.6/ICICONSOLEGPT/Utilities.py`

 * *Files identical despite different names*

### Comparing `ICICONSOLEGPT-0.0.5/ICICONSOLEGPT/__main__.py` & `ICICONSOLEGPT-0.0.6/ICICONSOLEGPT/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import openai
 import pandas as pd
 from datascroller import scroll
 from getpass import getpass
 
 import datetime
 import time
+import pytz
 import os
 import signal
 import json
 import pkg_resources
 from collections import deque
 
 try:
@@ -32,21 +33,24 @@
 signal.signal(signal.SIGALRM, timeout_handler)
 
 # Setting up flag for ctrl+c input
 flag = GracefulExiter()
 
 
 # Base URL for ICICLE Tapis
-default_base_url = "https://icicle.tapis.io"
+default_base_url = "icicle.tapis.io"
 base_url = default_base_url
+global https_base_url
 # Global variable to store pod id
 pod_id = ""
 # Global variable to store username, set upon initial input from login to TAPIS
 user = ""
 
+global t
+
 
 # This function formats a message to be like a title
 def heavyFormat(message):
     print("*" * (len(message) // 2))
     print("-" * (len(message) // 2))
     print(message)
     print("-" * (len(message) // 2))
@@ -75,40 +79,42 @@
 # The console function needs to parameters: a Neo4j graph object, and a pod id. 
 # The graph object allows for queries to be interpreted as Cypher and passed into the Neo4j pod.
 # The pod id is only needed here so that the user can see what pod they are connected to.
 
 command_stack = deque()
 
 def console(graph, pod_id):
+    global base_url
     # Instructions message, formatted with the lightFormat function
     lightFormat("Type \"new\" to access a different pod, or type \"exit\" to leave ICICONSOLE. Type \"help\" for help!\nNote that the scrolling menu, which appears on some queries, has a separate help menu.")
 
     # Loop so that the console keeps prompting the user for commands, until the user exits
     while(True):
         # This is reading the actual input from the user; the input message shows the username and the pod id
-        query = str(input("[" + user + "@" + pod_id + "] "))
+        query = str(input("[" + user + "@" + pod_id + "]$ "))
 
-        executeCypher = True
+        execute_cypher = True
 
         match query:
             case "exit":
                 os._exit(0)
             # The command to pick a new pod to connect to. Calls the choosePod function, defined below.
             case "new":
+                login()
                 choosePod()
-                executeCypher = False
+                execute_cypher = False
             # The command to clear the screen. Has a recursive call to itself so that the user is once again prompted, and the instruction message is still shown.
             case "clear":
                 os.system('cls' if os.name == 'nt' else 'clear')
                 console(graph, pod_id)
-                executeCypher = False
+                execute_cypher = False
             case "help":
                 try:
                     helpCypher()
-                    executeCypher = False
+                    execute_cypher = False
                 except:
                     pass
             case "all":
                 query = bcc.getAll()
             case "allNames":
                 query = bcc.getAllNames()
             case "oneByName":
@@ -140,89 +146,140 @@
                 except TimeoutError:
                     print("Timeout occurred.")
                 print(str(reply))
                 validate = input("Run this? (y/n) ")
                 if validate == "y":
                     query = str(reply)
                 else:
-                    executeCypher = False
+                    execute_cypher = False
             case _:
                 pass
 
         command_stack.append(query)
 
-        if (executeCypher):
-            # This tries to read the input as Cypher and apply the command to the Neo4j graph object.
-            # also parses the data to show the scrolling view in the right context
+        if execute_cypher:
             try:
-                result = graph.run(query)
-                for record in result:
-                    type_result = type(record[0])
-                    break
-                if type_result == py2neo.data.Node:
-                    data = []
-                    for record in result:
-                        node = record[0]
-                        properties = dict(node)
-                        data.append(properties)
-                    df = pd.DataFrame(data)
-                    with pd.option_context('display.max_rows', None, 'display.max_columns', None):
-                        scroll(df)
-                else:
-                    df = result.to_data_frame()
-                    with pd.option_context('expand_frame_repr', False, 'display.max_rows', None): 
-                        print(df)
+                try:
+                    if "DELETE" in query or "delete" in query:
+                        validate = input("Are you sure you want to delete node(s)? (y/n) ")
+                        if validate == "y":
+                            graph.run(query)
+                    # This tries to read the input as Cypher and apply the command to the Neo4j graph object.
+                    # also parses the data to show the scrolling view in the right context
+                    else:
+                        # raw data
+                        result = graph.run(query)
+                        # dictionary to store nodes, keys are node labels. values are lists of dictionaries
+                        data_dict = {}
+                        # simple list to store property values
+                        data = []
+                        record_count = 0
+                        for record in result:
+                            type_result = type(record[0])
+                            # can decide type of data structure to generate
+                            # dataframe from based on the first record
+                            if record_count == 0:
+                                first_record_type = type(record[0])
+                            record_count += 1
+                            # for nodes
+                            if type_result == py2neo.data.Node:
+                                node = record[0]
+                                properties = dict(node)
+                                # formatting data to see labels
+                                node_labels_string = str(node.labels)
+                                node_labels_string = node_labels_string.lstrip(":")
+                                node_labels = node_labels_string.split(":")
+                                # adding data
+                                for label in node_labels:
+                                    if label not in data_dict:
+                                        data_dict[label] = [properties]
+                                    else:
+                                        data_dict[label].append(properties)
+                            # for non-node data, can just add the record
+                            else:
+                                data.append(record)
+
+                        # separating node view by label for best viewing
+                        if first_record_type == py2neo.data.Node:
+                            keys = list(data_dict.keys())
+                            keys_string = " | ".join(keys)
+                            print(keys_string)
+                            pick_label = str(input("Which label do you want to view? "))
+                            label_data = data_dict[pick_label]
+                            df = pd.DataFrame(label_data)
+
+                        # need to manually assign the column names via keys
+                        else:
+                            keys = result.keys()
+                            df = pd.DataFrame(data, columns=keys)
+
+                        # datascroller view
+                        with pd.option_context('display.max_rows', None, 'display.max_columns', None):
+                            scroll(df)
+                # multiline input handling
+                except:
+                    queries = query.splitlines()
+                    for cypher_query in queries:
+                        try:
+                            graph.run(cypher_query)
+                        except:
+                            pass
 
             # Error catching, if the Cypher was not executed properly
             except:
                 if flag.exit():
                     break
                 print("Something went wrong")
 
 
-# This is the function that allows the user to pick a pod to connect to. It needs no paramters.
+# This is the function that allows the user to pick a pod to connect to. It needs no parameters.
 def choosePod():
 
     heavyFormat("Here are the IDs for your available TAPIS Pods: ")
 
     # The below loop prints the pod id for all pods that the TACC user is authorized to. If there are no pods, then the user is notified.
     i = 1
-    # t.pods.getpods() returns a list of all of the pods with more information about each pod
+    # t.pods.getpods() returns a list of all the pods with more information about each pod
     for pod in t.pods.get_pods():
         # pod.pod_id takes each element of the list, representing each pod, and extracts only the pod id
         # This is done because connecting to a Neo4j pod only requires the pod id.
         if "neo4j" in pod.pod_template:
             print(str(i) + ". " + pod.pod_id)
             i += 1
-    if (i == 1):
-        print("You don't have access to any TAPIS Neo4j pods. Try again after you have verified access to at least one pod.")
-        os._exit(0)
-    i = 1
+    if i == 1:
+        if base_url != default_base_url:
+            attempt_again = str(input(f"No Tapis pods on {base_url}. Try another base url? (y/n) "))
+            if attempt_again == "y":
+                login()
+            else:
+                print("Please verify access to a Neo4j template Tapis pod, and then try again later.")
+                os._exit(0)
 
-    while(True):
+    while True:
+        global pod_id
         try: 
             # The user gets a list of available pod ids from the above loop, and then enters the id they wish to connect to.
             # This input is stored in the pod_id variable
             pod_id = str(input("Enter the ID of the pod you want to access: ")).lower()
             # If the use has no pods or doesn't see what they are looking for, they can exit
-            if(pod_id == "exit"):
+            if pod_id == "exit":
                 os._exit(0)
             # Securely getting the username and password associated with the pod for later authentication to connect
             pod_username, password = t.pods.get_pod_credentials(pod_id=pod_id).user_username, t.pods.get_pod_credentials(pod_id=pod_id).user_password
             break
         # This is if there is trouble getting the username and password
         except:
             if flag.exit():
                 break
             print("Invalid Pod ID. Make sure you have access to this Pod.")
 
     # This is the standard format for the link that connects to the Neo4j Pod
-    graph_link = f"bolt+ssc://{pod_id}.pods.icicle.tapis.io:443"
+    graph_link = f"bolt+ssc://{pod_id}.pods.{base_url}:443"
 
-    while(True):
+    while True:
         try:
             # A graph object is created that authenticates with the previously gotten username and password. 
             graph = Graph(graph_link, auth=(pod_username, password), secure=True, verify=True)
             # Entering into the cypher console
             os.system('cls' if os.name == 'nt' else 'clear')
             time.sleep(0.25)
             heavyFormat(f"Hey there {user}! Welcome to the Neo4j Cypher Console for: " + str(pod_id))
@@ -231,37 +288,36 @@
         # This catches the error where there is an issue connecting or authenticating to the Pod.
         except:
             if flag.exit():
                 break
             print("There was a connection error.")
             break
 
-            
-# The below loop handles initial login.
-while(True):
-    try:
+
+def login():
+    global t
+    global user
+    global base_url
+    global https_base_url
+    while True:
         try:
-            t
-            if t.base_url == base_url and t.username == user and t.access_token:
-                print("Tapis object already exists.")
-                if t.access_token.expires_at < datetime.datetime.now(pytz.utc):
-                    raise
-            else:
-                raise
+            change_base_url = str(input(f"Change base url from {base_url}? (y/n) "))
+            if change_base_url == "y":
+                base_url = str(input("New base url: "))
+            https_base_url = "https://" + base_url
+            user = str(input("Enter Your TACC Username: "))
+            t = Tapis(base_url=https_base_url, username=user, password=getpass('Enter Your TACC Password: '))
+            t.get_tokens()
+            choosePod()
+            break
         except:
-            try:
-                user = str(input("Enter Your TACC Username: "))
-                t = Tapis(base_url = base_url, username=user,
-                        password = getpass('Enter Your TACC Password: '))
-                t.get_tokens()
-                # After logging in, choosePod is called to begin the workflow for the user.
-                choosePod()
+            if flag.exit():
                 break
-            except Exception as e:
-                raise
-    except:
-        if flag.exit():
-            break
-        print("An error occurred, likely due to mistyped login. Try again. ")
+            print(f"Wrong credentials, or you don't have an account on {base_url}.")
+
+
+login()
+
+
```

### Comparing `ICICONSOLEGPT-0.0.5/ICICONSOLEGPT.egg-info/PKG-INFO` & `ICICONSOLEGPT-0.0.6/ICICONSOLEGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ICICONSOLEGPT
-Version: 0.0.5
+Version: 0.0.6
 Summary: GPT Powered Command-line Interface tailored to working with Neo4j Knowledge Graph Databses hosted via Tapis Pods.
 Author-email: Sahil Samar <sahilsamar031@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Sahil Samar
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -60,15 +60,15 @@
 **OR**
 
 ```shell 
 git clone https://github.com/AD1616/ICICONSOLE.git
 ```
 
 ```shell
-cd ICICONSOLE/ICICONSOLEGPT/ICICONSOLE/
+cd ICICONSOLE/ICICONSOLEGPT/ICICONSOLEGPT/
 ```
 
 ```shell
 pip install pandas
 ```
 
 ```shell
```

### Comparing `ICICONSOLEGPT-0.0.5/LICENSE` & `ICICONSOLEGPT-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ICICONSOLEGPT-0.0.5/PKG-INFO` & `ICICONSOLEGPT-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ICICONSOLEGPT
-Version: 0.0.5
+Version: 0.0.6
 Summary: GPT Powered Command-line Interface tailored to working with Neo4j Knowledge Graph Databses hosted via Tapis Pods.
 Author-email: Sahil Samar <sahilsamar031@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Sahil Samar
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -60,15 +60,15 @@
 **OR**
 
 ```shell 
 git clone https://github.com/AD1616/ICICONSOLE.git
 ```
 
 ```shell
-cd ICICONSOLE/ICICONSOLEGPT/ICICONSOLE/
+cd ICICONSOLE/ICICONSOLEGPT/ICICONSOLEGPT/
 ```
 
 ```shell
 pip install pandas
 ```
 
 ```shell
```

### Comparing `ICICONSOLEGPT-0.0.5/README.md` & `ICICONSOLEGPT-0.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 **OR**
 
 ```shell 
 git clone https://github.com/AD1616/ICICONSOLE.git
 ```
 
 ```shell
-cd ICICONSOLE/ICICONSOLEGPT/ICICONSOLE/
+cd ICICONSOLE/ICICONSOLEGPT/ICICONSOLEGPT/
 ```
 
 ```shell
 pip install pandas
 ```
 
 ```shell
```

### Comparing `ICICONSOLEGPT-0.0.5/pyproject.toml` & `ICICONSOLEGPT-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ICICONSOLEGPT"
-version = "0.0.5"
+version = "0.0.6"
 description = "GPT Powered Command-line Interface tailored to working with Neo4j Knowledge Graph Databses hosted via Tapis Pods."
 readme = "README.md"
 authors = [{ name = "Sahil Samar", email = "sahilsamar031@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Programming Language :: Python",
```

