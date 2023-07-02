# Comparing `tmp/tracker-exporter-0.1.17.tar.gz` & `tmp/tracker-exporter-0.1.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tracker-exporter-0.1.17.tar", last modified: Thu Sep 22 07:13:37 2022, max compression
+gzip compressed data, was "tracker-exporter-0.1.18.tar", last modified: Sun Jul  2 07:28:26 2023, max compression
```

## Comparing `tracker-exporter-0.1.17.tar` & `tracker-exporter-0.1.18.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 akimrx     (503) staff       (20)        0 2022-09-22 07:13:37.000000 tracker-exporter-0.1.17/
--rw-r--r--   0 akimrx     (503) staff       (20)    12457 2022-09-22 07:13:37.000000 tracker-exporter-0.1.17/PKG-INFO
--rw-r--r--   0 akimrx     (503) staff       (20)     9811 2022-09-22 07:06:05.000000 tracker-exporter-0.1.17/README.md
--rw-r--r--   0 akimrx     (503) staff       (20)      480 2022-09-22 07:13:37.000000 tracker-exporter-0.1.17/setup.cfg
--rw-r--r--   0 akimrx     (503) staff       (20)     1773 2022-09-22 06:49:30.000000 tracker-exporter-0.1.17/setup.py
-drwxr-xr-x   0 akimrx     (503) staff       (20)        0 2022-09-22 07:13:37.000000 tracker-exporter-0.1.17/tracker_exporter/
--rw-r--r--   0 akimrx     (503) staff       (20)        0 2022-09-22 06:49:30.000000 tracker-exporter-0.1.17/tracker_exporter/__init__.py
--rw-r--r--   0 akimrx     (503) staff       (20)      348 2022-09-22 06:54:20.000000 tracker-exporter-0.1.17/tracker_exporter/__version__.py
--rw-r--r--   0 akimrx     (503) staff       (20)     2694 2022-09-22 06:49:30.000000 tracker-exporter-0.1.17/tracker_exporter/defaults.py
--rw-r--r--   0 akimrx     (503) staff       (20)      364 2022-09-22 06:49:30.000000 tracker-exporter-0.1.17/tracker_exporter/errors.py
--rw-r--r--   0 akimrx     (503) staff       (20)     4749 2022-09-22 06:57:31.000000 tracker-exporter-0.1.17/tracker_exporter/exporter.py
--rw-r--r--   0 akimrx     (503) staff       (20)     3048 2022-09-22 06:49:30.000000 tracker-exporter-0.1.17/tracker_exporter/main.py
-drwxr-xr-x   0 akimrx     (503) staff       (20)        0 2022-09-22 07:13:37.000000 tracker-exporter-0.1.17/tracker_exporter/models/
--rw-r--r--   0 akimrx     (503) staff       (20)        0 2022-09-22 06:49:30.000000 tracker-exporter-0.1.17/tracker_exporter/models/__init__.py
--rw-r--r--   0 akimrx     (503) staff       (20)     1118 2022-09-22 06:51:49.000000 tracker-exporter-0.1.17/tracker_exporter/models/base.py
--rw-r--r--   0 akimrx     (503) staff       (20)      348 2022-09-22 06:51:33.000000 tracker-exporter-0.1.17/tracker_exporter/models/enums.py
--rw-r--r--   0 akimrx     (503) staff       (20)     6730 2022-09-22 06:49:30.000000 tracker-exporter-0.1.17/tracker_exporter/models/issue.py
-drwxr-xr-x   0 akimrx     (503) staff       (20)        0 2022-09-22 07:13:37.000000 tracker-exporter-0.1.17/tracker_exporter/services/
--rw-r--r--   0 akimrx     (503) staff       (20)        0 2022-09-22 06:49:30.000000 tracker-exporter-0.1.17/tracker_exporter/services/__init__.py
--rw-r--r--   0 akimrx     (503) staff       (20)     4378 2022-09-22 06:53:33.000000 tracker-exporter-0.1.17/tracker_exporter/services/clickhouse.py
--rw-r--r--   0 akimrx     (503) staff       (20)     3365 2022-09-22 06:49:30.000000 tracker-exporter-0.1.17/tracker_exporter/services/monitoring.py
--rw-r--r--   0 akimrx     (503) staff       (20)     2086 2022-09-22 06:49:30.000000 tracker-exporter-0.1.17/tracker_exporter/services/tracker.py
-drwxr-xr-x   0 akimrx     (503) staff       (20)        0 2022-09-22 07:13:37.000000 tracker-exporter-0.1.17/tracker_exporter/utils/
--rw-r--r--   0 akimrx     (503) staff       (20)        0 2022-09-22 06:49:30.000000 tracker-exporter-0.1.17/tracker_exporter/utils/__init__.py
--rw-r--r--   0 akimrx     (503) staff       (20)     6079 2022-09-22 06:49:30.000000 tracker-exporter-0.1.17/tracker_exporter/utils/helpers.py
-drwxr-xr-x   0 akimrx     (503) staff       (20)        0 2022-09-22 07:13:37.000000 tracker-exporter-0.1.17/tracker_exporter.egg-info/
--rw-r--r--   0 akimrx     (503) staff       (20)    12457 2022-09-22 07:13:37.000000 tracker-exporter-0.1.17/tracker_exporter.egg-info/PKG-INFO
--rw-r--r--   0 akimrx     (503) staff       (20)      838 2022-09-22 07:13:37.000000 tracker-exporter-0.1.17/tracker_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 akimrx     (503) staff       (20)        1 2022-09-22 07:13:37.000000 tracker-exporter-0.1.17/tracker_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 akimrx     (503) staff       (20)       65 2022-09-22 07:13:37.000000 tracker-exporter-0.1.17/tracker_exporter.egg-info/entry_points.txt
--rw-r--r--   0 akimrx     (503) staff       (20)        1 2022-09-22 07:13:37.000000 tracker-exporter-0.1.17/tracker_exporter.egg-info/not-zip-safe
--rw-r--r--   0 akimrx     (503) staff       (20)      209 2022-09-22 07:13:37.000000 tracker-exporter-0.1.17/tracker_exporter.egg-info/requires.txt
--rw-r--r--   0 akimrx     (503) staff       (20)       17 2022-09-22 07:13:37.000000 tracker-exporter-0.1.17/tracker_exporter.egg-info/top_level.txt
+drwxr-xr-x   0 akimrx     (503) staff       (20)        0 2023-07-02 07:28:26.384276 tracker-exporter-0.1.18/
+-rw-r--r--   0 akimrx     (503) staff       (20)     1074 2023-07-02 06:51:32.000000 tracker-exporter-0.1.18/LICENSE
+-rw-r--r--   0 akimrx     (503) staff       (20)    13203 2023-07-02 07:28:26.384440 tracker-exporter-0.1.18/PKG-INFO
+-rw-r--r--   0 akimrx     (503) staff       (20)    10493 2023-07-02 07:26:23.000000 tracker-exporter-0.1.18/README.md
+-rw-r--r--   0 akimrx     (503) staff       (20)      480 2023-07-02 07:28:26.384816 tracker-exporter-0.1.18/setup.cfg
+-rw-r--r--   0 akimrx     (503) staff       (20)     1773 2023-07-02 06:51:32.000000 tracker-exporter-0.1.18/setup.py
+drwxr-xr-x   0 akimrx     (503) staff       (20)        0 2023-07-02 07:28:26.382107 tracker-exporter-0.1.18/tracker_exporter/
+-rw-r--r--   0 akimrx     (503) staff       (20)        0 2023-07-02 06:51:32.000000 tracker-exporter-0.1.18/tracker_exporter/__init__.py
+-rw-r--r--   0 akimrx     (503) staff       (20)      340 2023-07-02 07:26:23.000000 tracker-exporter-0.1.18/tracker_exporter/__version__.py
+-rw-r--r--   0 akimrx     (503) staff       (20)     2919 2023-07-02 07:26:23.000000 tracker-exporter-0.1.18/tracker_exporter/defaults.py
+-rw-r--r--   0 akimrx     (503) staff       (20)      364 2023-07-02 06:51:32.000000 tracker-exporter-0.1.18/tracker_exporter/errors.py
+-rw-r--r--   0 akimrx     (503) staff       (20)     4814 2023-07-02 07:26:23.000000 tracker-exporter-0.1.18/tracker_exporter/exporter.py
+-rw-r--r--   0 akimrx     (503) staff       (20)     3072 2023-07-02 07:26:23.000000 tracker-exporter-0.1.18/tracker_exporter/main.py
+drwxr-xr-x   0 akimrx     (503) staff       (20)        0 2023-07-02 07:28:26.383419 tracker-exporter-0.1.18/tracker_exporter/models/
+-rw-r--r--   0 akimrx     (503) staff       (20)        0 2023-07-02 06:51:32.000000 tracker-exporter-0.1.18/tracker_exporter/models/__init__.py
+-rw-r--r--   0 akimrx     (503) staff       (20)     1118 2023-07-02 06:51:32.000000 tracker-exporter-0.1.18/tracker_exporter/models/base.py
+-rw-r--r--   0 akimrx     (503) staff       (20)      348 2023-07-02 06:51:32.000000 tracker-exporter-0.1.18/tracker_exporter/models/enums.py
+-rw-r--r--   0 akimrx     (503) staff       (20)     6730 2023-07-02 06:51:32.000000 tracker-exporter-0.1.18/tracker_exporter/models/issue.py
+drwxr-xr-x   0 akimrx     (503) staff       (20)        0 2023-07-02 07:28:26.383875 tracker-exporter-0.1.18/tracker_exporter/services/
+-rw-r--r--   0 akimrx     (503) staff       (20)        0 2023-07-02 06:51:32.000000 tracker-exporter-0.1.18/tracker_exporter/services/__init__.py
+-rw-r--r--   0 akimrx     (503) staff       (20)     4378 2023-07-02 06:51:32.000000 tracker-exporter-0.1.18/tracker_exporter/services/clickhouse.py
+-rw-r--r--   0 akimrx     (503) staff       (20)     3365 2023-07-02 06:51:32.000000 tracker-exporter-0.1.18/tracker_exporter/services/monitoring.py
+-rw-r--r--   0 akimrx     (503) staff       (20)     2086 2023-07-02 06:51:32.000000 tracker-exporter-0.1.18/tracker_exporter/services/tracker.py
+drwxr-xr-x   0 akimrx     (503) staff       (20)        0 2023-07-02 07:28:26.384092 tracker-exporter-0.1.18/tracker_exporter/utils/
+-rw-r--r--   0 akimrx     (503) staff       (20)        0 2023-07-02 06:51:32.000000 tracker-exporter-0.1.18/tracker_exporter/utils/__init__.py
+-rw-r--r--   0 akimrx     (503) staff       (20)     6410 2023-07-02 07:26:23.000000 tracker-exporter-0.1.18/tracker_exporter/utils/helpers.py
+drwxr-xr-x   0 akimrx     (503) staff       (20)        0 2023-07-02 07:28:26.382934 tracker-exporter-0.1.18/tracker_exporter.egg-info/
+-rw-r--r--   0 akimrx     (503) staff       (20)    13203 2023-07-02 07:28:26.000000 tracker-exporter-0.1.18/tracker_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 akimrx     (503) staff       (20)      846 2023-07-02 07:28:26.000000 tracker-exporter-0.1.18/tracker_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 akimrx     (503) staff       (20)        1 2023-07-02 07:28:26.000000 tracker-exporter-0.1.18/tracker_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 akimrx     (503) staff       (20)       65 2023-07-02 07:28:26.000000 tracker-exporter-0.1.18/tracker_exporter.egg-info/entry_points.txt
+-rw-r--r--   0 akimrx     (503) staff       (20)        1 2023-07-02 07:28:26.000000 tracker-exporter-0.1.18/tracker_exporter.egg-info/not-zip-safe
+-rw-r--r--   0 akimrx     (503) staff       (20)      189 2023-07-02 07:28:26.000000 tracker-exporter-0.1.18/tracker_exporter.egg-info/requires.txt
+-rw-r--r--   0 akimrx     (503) staff       (20)       17 2023-07-02 07:28:26.000000 tracker-exporter-0.1.18/tracker_exporter.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tracker-exporter-0.1.17/PKG-INFO` & `tracker-exporter-0.1.18/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: tracker-exporter
-Version: 0.1.17
+Version: 0.1.18
 Summary: Yandex.Tracker issue metrics exporter
 Home-page: https://github.com/akimrx/yandex-tracker-exporter
 Author: Akim Faskhutdinov
-Author-email: a.faskhutdinov@yclients.tech
+Author-email: akimstrong@yandex.ru
 License: MIT
 Download-URL: https://pypi.org/project/tracker-exporter/
 Description: # Yandex.Tracker Exporter
         
         Export issue metadata & agile metrics to OLAP data storage. Metrics based on issue changelog.
         
+        > This is a working example of collecting metadata and metrics from Yandex.Tracker for analytics, based on the first version of the internal private tool.
+        > You can fork this repository and refine the tool the way you want. Or use it as it is - this will allow you to build basic analytics on the tasks from Yandex.Tracker.
+        
         ## Self-hosted arch example
         
         ![](/docs/images/agile_metrics.png)
         
         So, you can install Clickhouse with Clickhouse Proxy via Ansible role inside project.  
         Edit the inventory file `ansible/inventory/hosts.yml` and just run ansible-playbook.
         
@@ -25,14 +28,71 @@
         ```bash
         
         pip3 install -r requirements-dev.txt
         cd ansible
         ansible-playbook -i inventory/hosts.yml playbooks/clickhouse.yml --limit agile
         ```
         
+        ## Usage
+        
+        ### Native
+        
+        #### Install from source
+        
+        ```bash
+        # prepare virtual environment
+        python3 -m venv venv
+        source venv/bin/activate
+        python3 setup.py install
+        
+        # configure environment variables
+        export EXPORTER_TRACKER_TOKEN="xxxx"
+        export EXPORTER_TRACKER_ORG_ID="123456"
+        
+        export EXPORTER_TRACKER_ISSUES_SEARCH_RANGE="6h"
+        export EXPORTER_TRACKER_FETCH_INTERVAL=30
+        
+        export EXPORTER_CLICKHOUSE_USER="default"
+        export EXPORTER_CLICKHOUSE_PASSWORD="strongpassword"
+        export EXPORTER_CLICKHOUSE_HOST="clickhouse01.example.com"
+        export EXPORTER_CLICKHOUSE_HTTP_PORT="8121"
+        
+        export EXPORTER_LOGLEVEL="info"
+        export EXPORTER_ENABLE_UPLOAD=true
+        
+        # run
+        tracker-exporter
+        ```
+        
+        #### Install from pypi
+        
+        ```bash
+        pip3 install tracker-exporter
+        tracker-exporter
+        ```
+        
+        #### Use .env file
+        
+        Read about the settings [here](#environment-variables-settings)
+        
+        ```bash
+        tracker-exporter --env-file /home/akimrx/tracker/.settings
+        ```
+        
+        
+        ### Docker
+        
+        ```bash
+        
+        cd yandex-tracker-exporter
+        touch .env  # prepare the environment variables file (dotenv), like the example above
+        docker-compose up -d --build
+        docker logs tracker-exporter -f
+        ```
+        
         
         ## Serverless arch example
         
         ![](/docs/images/agile_metrics_cloud.png)
         
         ### Create a Managed Clickhouse cluster
         
@@ -194,69 +254,18 @@
         | `EXPORTER_CLICKHOUSE_USER` | ❌ | `default` | Clickhouse read-write username |
         | `EXPORTER_CLICKHOUSE_PASSWORD` | ✅ | None | Clickhouse user password. **If your clickhouse/user can work without password just ignore this variable.** |
         | `EXPORTER_CLICKHOUSE_CACERT_PATH` | ❌ | `None` | Path to CA certificate. Only for HTTPS |
         | `EXPORTER_CLICKHOUSE_SERVERLESS_PROXY_ID` | ❌ | `None` | Database connection ID. Only for serverless |
         | `EXPORTER_CLICKHOUSE_DATABASE` | ❌ | `agile` | Database for exporter CH tables |
         | `EXPORTER_CLICKHOUSE_ISSUES_TABLE` | ❌ | `issues` | Table when store issues metadata |
         | `EXPORTER_CLICKHOUSE_ISSUE_METRICS_TABLE` | ❌ | `issue_metrics` | Table when store issue metrics |
+        | `EXPORTER_WORKHOURS_START` | ❌ | 9 | The beginning of working hours for calculating business hour metrics |
+        | `EXPORTER_WORKHOURS_END` | ❌ | 22 | The end of working hours for calculating business hour metrics |
         
         
-        # Usage
-        
-        ## Native
-        
-        ### Install from source
-        
-        ```bash
-        
-        python3 -m venv venv
-        source venv/bin/activate
-        python3 setup.py install
-        
-        export EXPORTER_TRACKER_TOKEN="xxxx"
-        export EXPORTER_TRACKER_ORG_ID="123456"
-        
-        export EXPORTER_TRACKER_ISSUES_SEARCH_RANGE="6h"
-        export EXPORTER_TRACKER_FETCH_INTERVAL=30
-        
-        export EXPORTER_CLICKHOUSE_USER="default"
-        export EXPORTER_CLICKHOUSE_PASSWORD="strongpassword"
-        export EXPORTER_CLICKHOUSE_HOST="clickhouse01.example.com"
-        export EXPORTER_CLICKHOUSE_HTTP_PORT="8121"
-        
-        export EXPORTER_LOGLEVEL="info"
-        export EXPORTER_ENABLE_UPLOAD=true
-        
-        tracker-exporter
-        ```
-        
-        ### Install from pypi
-        
-        ```bash
-        pip3 install tracker-exporter
-        tracker-exporter
-        ```
-        
-        ### Use .env file
-        
-        ```bash
-        tracker-exporter --env-file /home/akimrx/tracker/.settings
-        ```
-        
-        
-        ## Docker
-        
-        ```bash
-        
-        cd yandex-tracker-exporter
-        touch .env  # prepare the environment variables file (dotenv), like the example above
-        docker-compose up -d --build
-        docker logs tracker-exporter -f
-        ```
-        
         # Monitoring
         
         | Metric name | Metric type | Labels | Description |
         |-------------|-------------|--------|-------------|
         | `tracker_exporter_clickhouse_insert_time_seconds` | `time` | `project` | Insert query time |
         | `tracker_exporter_clickhouse_optimize_time_seconds` | `time` | `project` | Optimize query time |
         | `tracker_exporter_clickhouse_inserted_rows` | `gauge` | `project`, `database`, `table` | Inserted rows to Clickhouse from last update |
```

### Comparing `tracker-exporter-0.1.17/README.md` & `tracker-exporter-0.1.18/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # Yandex.Tracker Exporter
 
 Export issue metadata & agile metrics to OLAP data storage. Metrics based on issue changelog.
 
+> This is a working example of collecting metadata and metrics from Yandex.Tracker for analytics, based on the first version of the internal private tool.
+> You can fork this repository and refine the tool the way you want. Or use it as it is - this will allow you to build basic analytics on the tasks from Yandex.Tracker.
+
 ## Self-hosted arch example
 
 ![](/docs/images/agile_metrics.png)
 
 So, you can install Clickhouse with Clickhouse Proxy via Ansible role inside project.  
 Edit the inventory file `ansible/inventory/hosts.yml` and just run ansible-playbook.
 
@@ -16,14 +19,71 @@
 ```bash
 
 pip3 install -r requirements-dev.txt
 cd ansible
 ansible-playbook -i inventory/hosts.yml playbooks/clickhouse.yml --limit agile
 ```
 
+## Usage
+
+### Native
+
+#### Install from source
+
+```bash
+# prepare virtual environment
+python3 -m venv venv
+source venv/bin/activate
+python3 setup.py install
+
+# configure environment variables
+export EXPORTER_TRACKER_TOKEN="xxxx"
+export EXPORTER_TRACKER_ORG_ID="123456"
+
+export EXPORTER_TRACKER_ISSUES_SEARCH_RANGE="6h"
+export EXPORTER_TRACKER_FETCH_INTERVAL=30
+
+export EXPORTER_CLICKHOUSE_USER="default"
+export EXPORTER_CLICKHOUSE_PASSWORD="strongpassword"
+export EXPORTER_CLICKHOUSE_HOST="clickhouse01.example.com"
+export EXPORTER_CLICKHOUSE_HTTP_PORT="8121"
+
+export EXPORTER_LOGLEVEL="info"
+export EXPORTER_ENABLE_UPLOAD=true
+
+# run
+tracker-exporter
+```
+
+#### Install from pypi
+
+```bash
+pip3 install tracker-exporter
+tracker-exporter
+```
+
+#### Use .env file
+
+Read about the settings [here](#environment-variables-settings)
+
+```bash
+tracker-exporter --env-file /home/akimrx/tracker/.settings
+```
+
+
+### Docker
+
+```bash
+
+cd yandex-tracker-exporter
+touch .env  # prepare the environment variables file (dotenv), like the example above
+docker-compose up -d --build
+docker logs tracker-exporter -f
+```
+
 
 ## Serverless arch example
 
 ![](/docs/images/agile_metrics_cloud.png)
 
 ### Create a Managed Clickhouse cluster
 
@@ -185,69 +245,18 @@
 | `EXPORTER_CLICKHOUSE_USER` | ❌ | `default` | Clickhouse read-write username |
 | `EXPORTER_CLICKHOUSE_PASSWORD` | ✅ | None | Clickhouse user password. **If your clickhouse/user can work without password just ignore this variable.** |
 | `EXPORTER_CLICKHOUSE_CACERT_PATH` | ❌ | `None` | Path to CA certificate. Only for HTTPS |
 | `EXPORTER_CLICKHOUSE_SERVERLESS_PROXY_ID` | ❌ | `None` | Database connection ID. Only for serverless |
 | `EXPORTER_CLICKHOUSE_DATABASE` | ❌ | `agile` | Database for exporter CH tables |
 | `EXPORTER_CLICKHOUSE_ISSUES_TABLE` | ❌ | `issues` | Table when store issues metadata |
 | `EXPORTER_CLICKHOUSE_ISSUE_METRICS_TABLE` | ❌ | `issue_metrics` | Table when store issue metrics |
+| `EXPORTER_WORKHOURS_START` | ❌ | 9 | The beginning of working hours for calculating business hour metrics |
+| `EXPORTER_WORKHOURS_END` | ❌ | 22 | The end of working hours for calculating business hour metrics |
 
 
-# Usage
-
-## Native
-
-### Install from source
-
-```bash
-
-python3 -m venv venv
-source venv/bin/activate
-python3 setup.py install
-
-export EXPORTER_TRACKER_TOKEN="xxxx"
-export EXPORTER_TRACKER_ORG_ID="123456"
-
-export EXPORTER_TRACKER_ISSUES_SEARCH_RANGE="6h"
-export EXPORTER_TRACKER_FETCH_INTERVAL=30
-
-export EXPORTER_CLICKHOUSE_USER="default"
-export EXPORTER_CLICKHOUSE_PASSWORD="strongpassword"
-export EXPORTER_CLICKHOUSE_HOST="clickhouse01.example.com"
-export EXPORTER_CLICKHOUSE_HTTP_PORT="8121"
-
-export EXPORTER_LOGLEVEL="info"
-export EXPORTER_ENABLE_UPLOAD=true
-
-tracker-exporter
-```
-
-### Install from pypi
-
-```bash
-pip3 install tracker-exporter
-tracker-exporter
-```
-
-### Use .env file
-
-```bash
-tracker-exporter --env-file /home/akimrx/tracker/.settings
-```
-
-
-## Docker
-
-```bash
-
-cd yandex-tracker-exporter
-touch .env  # prepare the environment variables file (dotenv), like the example above
-docker-compose up -d --build
-docker logs tracker-exporter -f
-```
-
 # Monitoring
 
 | Metric name | Metric type | Labels | Description |
 |-------------|-------------|--------|-------------|
 | `tracker_exporter_clickhouse_insert_time_seconds` | `time` | `project` | Insert query time |
 | `tracker_exporter_clickhouse_optimize_time_seconds` | `time` | `project` | Optimize query time |
 | `tracker_exporter_clickhouse_inserted_rows` | `gauge` | `project`, `database`, `table` | Inserted rows to Clickhouse from last update |
```

### Comparing `tracker-exporter-0.1.17/setup.py` & `tracker-exporter-0.1.18/setup.py`

 * *Files identical despite different names*

### Comparing `tracker-exporter-0.1.17/tracker_exporter/defaults.py` & `tracker-exporter-0.1.18/tracker_exporter/defaults.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,21 @@
 import datetime as dt
 
 # Common settings
 LOGLEVEL = os.environ.get("EXPORTER_LOGLEVEL", "info")
 UPLOAD_TO_STORAGE = os.environ.get("EXPORTER_ENABLE_UPLOAD", "false").lower() in ("true", "yes")
 
 # Business days settings
-BUSINESS_HOURS_START = dt.time(9)
-BUSINESS_HOURS_END = dt.time(22)
-WEEKENDS = (5, 6,)  # Monday is 0, Sunday is 6
+WORKDAYS = [0, 1, 2, 3, 4]  # From Monday to Friday
+try:
+    BUSINESS_HOURS_START = dt.time(int(os.environ.get("EXPORTER_WORKHOURS_START", "9")))
+    BUSINESS_HOURS_END = dt.time(int(os.environ.get("EXPORTER_WORKHOURS_END", "22")))
+except (ValueError, TypeError):
+    BUSINESS_HOURS_START = dt.time(9)
+    BUSINESS_HOURS_END = dt.time(22)
 
 # Monitoring settings
 MONITORING_ENABLED = os.environ.get("EXPORTER_MONITORING_ENABLED", "false").lower() in ("true", "yes")
 MONITORING_HOST = os.environ.get("EXPORTER_MONITORING_HOST", "localhost")
 MONITORING_PORT = os.environ.get("EXPORTER_MONITORING_PORT", 8125)
 MONITORING_METRIC_BASE_PREFIX = os.environ.get("MONITORING_METRIC_PREFIX", "tracker_exporter")
 MONITORING_BASE_LABELS = [
```

### Comparing `tracker-exporter-0.1.17/tracker_exporter/exporter.py` & `tracker-exporter-0.1.18/tracker_exporter/exporter.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 monitoring = DogStatsdClient(enabled=MONITORING_ENABLED)
 
 
 class Exporter:
     # TODO: configure class instance
     # TODO: parse migration from sprint to sprint by changelog (field changed),
     # by default exported only last sprint (tracker logic)
-    def __init__(self):
-        self.clickhouse = ClickhouseClient(
+    def __init__(self, clickhouse_client: ClickhouseClient = None):
+        self.clickhouse = clickhouse_client or ClickhouseClient(
             host=CLICKHOUSE_HOST,
             port=CLICKHOUSE_HTTP_PORT,
             user=CLICKHOUSE_USER,
             password=CLICKHOUSE_PASSWORD
         )
 
     @monitoring.send_time_metric("issues_processing_time_seconds")
```

### Comparing `tracker-exporter-0.1.17/tracker_exporter/main.py` & `tracker-exporter-0.1.18/tracker_exporter/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,20 @@
     metavar="file",
     dest="env_file",
     type=str,
     required=False,
     help="Path to .env file"
 )
 args = parser.parse_args()
-load_dotenv(args.env_file)
 warnings.filterwarnings("ignore")
 
+if args.env_file:
+    load_dotenv(args.env_file)
+
+
 # pylint: disable=C0413
 from .errors import ExportError
 from .services.monitoring import DogStatsdClient, sentry_events_filter
 from .exporter import Exporter
 from .__version__ import appname, version
 from .defaults import (
     EXCLUDE_QUEUES,
```

### Comparing `tracker-exporter-0.1.17/tracker_exporter/models/base.py` & `tracker-exporter-0.1.18/tracker_exporter/models/base.py`

 * *Files identical despite different names*

### Comparing `tracker-exporter-0.1.17/tracker_exporter/models/issue.py` & `tracker-exporter-0.1.18/tracker_exporter/models/issue.py`

 * *Files identical despite different names*

### Comparing `tracker-exporter-0.1.17/tracker_exporter/services/clickhouse.py` & `tracker-exporter-0.1.18/tracker_exporter/services/clickhouse.py`

 * *Files identical despite different names*

### Comparing `tracker-exporter-0.1.17/tracker_exporter/services/monitoring.py` & `tracker-exporter-0.1.18/tracker_exporter/services/monitoring.py`

 * *Files identical despite different names*

### Comparing `tracker-exporter-0.1.17/tracker_exporter/services/tracker.py` & `tracker-exporter-0.1.18/tracker_exporter/services/tracker.py`

 * *Files identical despite different names*

### Comparing `tracker-exporter-0.1.17/tracker_exporter/utils/helpers.py` & `tracker-exporter-0.1.18/tracker_exporter/utils/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 
 from functools import wraps
 from typing import Union, Tuple
 from datetime import datetime
 
 import holidays
 import pandas as pd
+import businesstimedelta
 
-from businesstime import BusinessTime
 from tracker_exporter.models.enums import TimeDeltaOut
 from tracker_exporter.defaults import (
     NOT_NULLABLE_FIELDS,
-    WEEKENDS,
+    WORKDAYS,
     BUSINESS_HOURS_START,
     BUSINESS_HOURS_END,
     TRACKER_DEFAULT_DATETIME_FORMAT
 )
 
 logger = logging.getLogger(__name__)
 
@@ -36,34 +36,45 @@
         return delta
     return delta
 
 
 def calculate_time_spent(start_date: datetime,
                          end_date: datetime,
                          busdays_only: bool = False,
-                         weekends: Tuple[int] = WEEKENDS,
+                         workdays: list = WORKDAYS,
                          business_hours: Tuple = (BUSINESS_HOURS_START, BUSINESS_HOURS_END,)) -> int:
     """
     Calculate timedelta between dates with business days support.
     Weekdays: Monday is 0, Sunday is 6, so weekends (5, 6) mean (Sat, Sun).
+    Returns: seconds
     """
     if not isinstance(start_date, datetime):
         start_date = pd.to_datetime(start_date)
     if not isinstance(end_date, datetime):
         end_date = pd.to_datetime(end_date)
 
+    holiday_rules = businesstimedelta.HolidayRule(holidays.RU())
+    workday_rules = businesstimedelta.WorkDayRule(
+        start_time=business_hours[0],
+        end_time=business_hours[1],
+        working_days=workdays)
+
+
     if busdays_only:
-        bt = BusinessTime(business_hours=business_hours, weekends=weekends, holidays=holidays.RU())  # pylint: disable=C0103
-        result = bt.businesstimedelta(start_date, end_date).total_seconds()
+        logger.debug(f"Calculating workhours. Business hours: {business_hours}. {start_date}, {end_date}")
+        bt = businesstimedelta.Rules([workday_rules, holiday_rules])
+        result = bt.difference(start_date, end_date).timedelta.total_seconds()
     else:
+        logger.debug(f"Calculating regular hours")
         result = (end_date - start_date).total_seconds()
 
     return abs(int(result))
 
 
+
 def fix_null_dates(data: dict) -> dict:
     to_remove = []
 
     for key, value in data.items():
         if key in NOT_NULLABLE_FIELDS and (value is None or value == ""):
             to_remove.append(key)
```

### Comparing `tracker-exporter-0.1.17/tracker_exporter.egg-info/PKG-INFO` & `tracker-exporter-0.1.18/tracker_exporter.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: tracker-exporter
-Version: 0.1.17
+Version: 0.1.18
 Summary: Yandex.Tracker issue metrics exporter
 Home-page: https://github.com/akimrx/yandex-tracker-exporter
 Author: Akim Faskhutdinov
-Author-email: a.faskhutdinov@yclients.tech
+Author-email: akimstrong@yandex.ru
 License: MIT
 Download-URL: https://pypi.org/project/tracker-exporter/
 Description: # Yandex.Tracker Exporter
         
         Export issue metadata & agile metrics to OLAP data storage. Metrics based on issue changelog.
         
+        > This is a working example of collecting metadata and metrics from Yandex.Tracker for analytics, based on the first version of the internal private tool.
+        > You can fork this repository and refine the tool the way you want. Or use it as it is - this will allow you to build basic analytics on the tasks from Yandex.Tracker.
+        
         ## Self-hosted arch example
         
         ![](/docs/images/agile_metrics.png)
         
         So, you can install Clickhouse with Clickhouse Proxy via Ansible role inside project.  
         Edit the inventory file `ansible/inventory/hosts.yml` and just run ansible-playbook.
         
@@ -25,14 +28,71 @@
         ```bash
         
         pip3 install -r requirements-dev.txt
         cd ansible
         ansible-playbook -i inventory/hosts.yml playbooks/clickhouse.yml --limit agile
         ```
         
+        ## Usage
+        
+        ### Native
+        
+        #### Install from source
+        
+        ```bash
+        # prepare virtual environment
+        python3 -m venv venv
+        source venv/bin/activate
+        python3 setup.py install
+        
+        # configure environment variables
+        export EXPORTER_TRACKER_TOKEN="xxxx"
+        export EXPORTER_TRACKER_ORG_ID="123456"
+        
+        export EXPORTER_TRACKER_ISSUES_SEARCH_RANGE="6h"
+        export EXPORTER_TRACKER_FETCH_INTERVAL=30
+        
+        export EXPORTER_CLICKHOUSE_USER="default"
+        export EXPORTER_CLICKHOUSE_PASSWORD="strongpassword"
+        export EXPORTER_CLICKHOUSE_HOST="clickhouse01.example.com"
+        export EXPORTER_CLICKHOUSE_HTTP_PORT="8121"
+        
+        export EXPORTER_LOGLEVEL="info"
+        export EXPORTER_ENABLE_UPLOAD=true
+        
+        # run
+        tracker-exporter
+        ```
+        
+        #### Install from pypi
+        
+        ```bash
+        pip3 install tracker-exporter
+        tracker-exporter
+        ```
+        
+        #### Use .env file
+        
+        Read about the settings [here](#environment-variables-settings)
+        
+        ```bash
+        tracker-exporter --env-file /home/akimrx/tracker/.settings
+        ```
+        
+        
+        ### Docker
+        
+        ```bash
+        
+        cd yandex-tracker-exporter
+        touch .env  # prepare the environment variables file (dotenv), like the example above
+        docker-compose up -d --build
+        docker logs tracker-exporter -f
+        ```
+        
         
         ## Serverless arch example
         
         ![](/docs/images/agile_metrics_cloud.png)
         
         ### Create a Managed Clickhouse cluster
         
@@ -194,69 +254,18 @@
         | `EXPORTER_CLICKHOUSE_USER` | ❌ | `default` | Clickhouse read-write username |
         | `EXPORTER_CLICKHOUSE_PASSWORD` | ✅ | None | Clickhouse user password. **If your clickhouse/user can work without password just ignore this variable.** |
         | `EXPORTER_CLICKHOUSE_CACERT_PATH` | ❌ | `None` | Path to CA certificate. Only for HTTPS |
         | `EXPORTER_CLICKHOUSE_SERVERLESS_PROXY_ID` | ❌ | `None` | Database connection ID. Only for serverless |
         | `EXPORTER_CLICKHOUSE_DATABASE` | ❌ | `agile` | Database for exporter CH tables |
         | `EXPORTER_CLICKHOUSE_ISSUES_TABLE` | ❌ | `issues` | Table when store issues metadata |
         | `EXPORTER_CLICKHOUSE_ISSUE_METRICS_TABLE` | ❌ | `issue_metrics` | Table when store issue metrics |
+        | `EXPORTER_WORKHOURS_START` | ❌ | 9 | The beginning of working hours for calculating business hour metrics |
+        | `EXPORTER_WORKHOURS_END` | ❌ | 22 | The end of working hours for calculating business hour metrics |
         
         
-        # Usage
-        
-        ## Native
-        
-        ### Install from source
-        
-        ```bash
-        
-        python3 -m venv venv
-        source venv/bin/activate
-        python3 setup.py install
-        
-        export EXPORTER_TRACKER_TOKEN="xxxx"
-        export EXPORTER_TRACKER_ORG_ID="123456"
-        
-        export EXPORTER_TRACKER_ISSUES_SEARCH_RANGE="6h"
-        export EXPORTER_TRACKER_FETCH_INTERVAL=30
-        
-        export EXPORTER_CLICKHOUSE_USER="default"
-        export EXPORTER_CLICKHOUSE_PASSWORD="strongpassword"
-        export EXPORTER_CLICKHOUSE_HOST="clickhouse01.example.com"
-        export EXPORTER_CLICKHOUSE_HTTP_PORT="8121"
-        
-        export EXPORTER_LOGLEVEL="info"
-        export EXPORTER_ENABLE_UPLOAD=true
-        
-        tracker-exporter
-        ```
-        
-        ### Install from pypi
-        
-        ```bash
-        pip3 install tracker-exporter
-        tracker-exporter
-        ```
-        
-        ### Use .env file
-        
-        ```bash
-        tracker-exporter --env-file /home/akimrx/tracker/.settings
-        ```
-        
-        
-        ## Docker
-        
-        ```bash
-        
-        cd yandex-tracker-exporter
-        touch .env  # prepare the environment variables file (dotenv), like the example above
-        docker-compose up -d --build
-        docker logs tracker-exporter -f
-        ```
-        
         # Monitoring
         
         | Metric name | Metric type | Labels | Description |
         |-------------|-------------|--------|-------------|
         | `tracker_exporter_clickhouse_insert_time_seconds` | `time` | `project` | Insert query time |
         | `tracker_exporter_clickhouse_optimize_time_seconds` | `time` | `project` | Optimize query time |
         | `tracker_exporter_clickhouse_inserted_rows` | `gauge` | `project`, `database`, `table` | Inserted rows to Clickhouse from last update |
```

### Comparing `tracker-exporter-0.1.17/tracker_exporter.egg-info/SOURCES.txt` & `tracker-exporter-0.1.18/tracker_exporter.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.cfg
 setup.py
 tracker_exporter/__init__.py
 tracker_exporter/__version__.py
 tracker_exporter/defaults.py
 tracker_exporter/errors.py
```

