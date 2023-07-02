# Comparing `tmp/alienpy-1.5.1.tar.gz` & `tmp/alienpy-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alienpy-1.5.1.tar", last modified: Wed Jun  7 06:54:00 2023, max compression
+gzip compressed data, was "alienpy-1.5.2.tar", last modified: Sun Jul  2 21:09:58 2023, max compression
```

## Comparing `alienpy-1.5.1.tar` & `alienpy-1.5.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2023-06-07 06:54:00.756305 alienpy-1.5.1/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1538 2020-05-18 21:36:32.000000 alienpy-1.5.1/LICENSE
--rw-r--r--   0 adrian    (1000) adrian    (1000)    10431 2023-06-07 06:54:00.756305 alienpy-1.5.1/PKG-INFO
--rw-r--r--   0 adrian    (1000) adrian    (1000)     9570 2022-12-20 08:02:48.000000 alienpy-1.5.1/README.md
-drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2023-06-07 06:54:00.755305 alienpy-1.5.1/alienpy/
--rw-r--r--   0 adrian    (1000) adrian    (1000)       17 2023-05-15 09:29:38.000000 alienpy-1.5.1/alienpy/__init__.py
--rwxr-xr-x   0 adrian    (1000) adrian    (1000)    83476 2023-06-07 06:39:48.000000 alienpy-1.5.1/alienpy/alien.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     2821 2023-06-06 09:00:33.000000 alienpy-1.5.1/alienpy/async_tools.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)    14486 2023-06-06 15:39:51.000000 alienpy-1.5.1/alienpy/connect_ssl.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     5936 2023-06-06 17:01:56.000000 alienpy-1.5.1/alienpy/data_structs.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     3684 2023-06-06 17:18:24.000000 alienpy-1.5.1/alienpy/global_vars.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1671 2023-06-06 10:10:16.000000 alienpy-1.5.1/alienpy/setup_cwd.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     2031 2023-06-06 10:37:54.000000 alienpy-1.5.1/alienpy/setup_logging.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1688 2023-06-06 17:02:39.000000 alienpy-1.5.1/alienpy/tools_history.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)    44208 2023-06-06 20:30:18.000000 alienpy-1.5.1/alienpy/tools_nowb.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1875 2023-06-06 17:09:11.000000 alienpy-1.5.1/alienpy/tools_shell.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)      881 2023-06-06 10:31:28.000000 alienpy-1.5.1/alienpy/tools_stackcmd.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)      289 2023-06-07 06:53:28.000000 alienpy-1.5.1/alienpy/version.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)    25028 2023-06-07 05:34:32.000000 alienpy-1.5.1/alienpy/wb_api.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)    10260 2023-06-06 17:09:39.000000 alienpy-1.5.1/alienpy/wb_async.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)    58020 2023-06-06 19:23:52.000000 alienpy-1.5.1/alienpy/xrd_core.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)    24075 2023-06-07 06:49:20.000000 alienpy-1.5.1/alienpy/xrd_tools.py
-drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2023-06-07 06:54:00.756305 alienpy-1.5.1/alienpy.egg-info/
--rw-r--r--   0 adrian    (1000) adrian    (1000)    10431 2023-06-07 06:54:00.000000 alienpy-1.5.1/alienpy.egg-info/PKG-INFO
--rw-r--r--   0 adrian    (1000) adrian    (1000)      606 2023-06-07 06:54:00.000000 alienpy-1.5.1/alienpy.egg-info/SOURCES.txt
--rw-r--r--   0 adrian    (1000) adrian    (1000)        1 2023-06-07 06:54:00.000000 alienpy-1.5.1/alienpy.egg-info/dependency_links.txt
--rw-r--r--   0 adrian    (1000) adrian    (1000)      828 2023-06-07 06:54:00.000000 alienpy-1.5.1/alienpy.egg-info/entry_points.txt
--rw-r--r--   0 adrian    (1000) adrian    (1000)       56 2023-06-07 06:54:00.000000 alienpy-1.5.1/alienpy.egg-info/requires.txt
--rw-r--r--   0 adrian    (1000) adrian    (1000)        8 2023-06-07 06:54:00.000000 alienpy-1.5.1/alienpy.egg-info/top_level.txt
-drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2023-06-07 06:54:00.756305 alienpy-1.5.1/examples/
--rwxr-xr-x   0 adrian    (1000) adrian    (1000)     2169 2022-12-20 08:02:48.000000 alienpy-1.5.1/examples/alien_wbtime
--rw-r--r--   0 adrian    (1000) adrian    (1000)       38 2023-06-07 06:54:00.756305 alienpy-1.5.1/setup.cfg
--rw-r--r--   0 adrian    (1000) adrian    (1000)     4160 2023-06-06 11:45:37.000000 alienpy-1.5.1/setup.py
+drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-02 21:09:58.624886 alienpy-1.5.2/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1538 2020-05-18 21:36:32.000000 alienpy-1.5.2/LICENSE
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    10431 2023-07-02 21:09:58.623886 alienpy-1.5.2/PKG-INFO
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     9570 2022-12-20 08:02:48.000000 alienpy-1.5.2/README.md
+drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-02 21:09:58.623886 alienpy-1.5.2/alienpy/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)       17 2023-05-15 09:29:38.000000 alienpy-1.5.2/alienpy/__init__.py
+-rwxr-xr-x   0 adrian    (1000) adrian    (1000)    84108 2023-07-02 18:51:04.000000 alienpy-1.5.2/alienpy/alien.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     2821 2023-06-06 09:00:33.000000 alienpy-1.5.2/alienpy/async_tools.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    14486 2023-06-06 15:39:51.000000 alienpy-1.5.2/alienpy/connect_ssl.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     5936 2023-06-06 17:01:56.000000 alienpy-1.5.2/alienpy/data_structs.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     3684 2023-06-06 17:18:24.000000 alienpy-1.5.2/alienpy/global_vars.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1671 2023-06-06 10:10:16.000000 alienpy-1.5.2/alienpy/setup_cwd.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     2031 2023-06-06 10:37:54.000000 alienpy-1.5.2/alienpy/setup_logging.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1688 2023-06-06 17:02:39.000000 alienpy-1.5.2/alienpy/tools_history.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    44634 2023-07-02 18:51:04.000000 alienpy-1.5.2/alienpy/tools_nowb.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1875 2023-06-06 17:09:11.000000 alienpy-1.5.2/alienpy/tools_shell.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      881 2023-06-06 10:31:28.000000 alienpy-1.5.2/alienpy/tools_stackcmd.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      289 2023-07-02 21:07:24.000000 alienpy-1.5.2/alienpy/version.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    25028 2023-06-07 05:34:32.000000 alienpy-1.5.2/alienpy/wb_api.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    10260 2023-06-06 17:09:39.000000 alienpy-1.5.2/alienpy/wb_async.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    58095 2023-07-02 18:52:38.000000 alienpy-1.5.2/alienpy/xrd_core.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    24075 2023-06-07 06:49:20.000000 alienpy-1.5.2/alienpy/xrd_tools.py
+drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-02 21:09:58.623886 alienpy-1.5.2/alienpy.egg-info/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    10431 2023-07-02 21:09:58.000000 alienpy-1.5.2/alienpy.egg-info/PKG-INFO
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      606 2023-07-02 21:09:58.000000 alienpy-1.5.2/alienpy.egg-info/SOURCES.txt
+-rw-r--r--   0 adrian    (1000) adrian    (1000)        1 2023-07-02 21:09:58.000000 alienpy-1.5.2/alienpy.egg-info/dependency_links.txt
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      828 2023-07-02 21:09:58.000000 alienpy-1.5.2/alienpy.egg-info/entry_points.txt
+-rw-r--r--   0 adrian    (1000) adrian    (1000)       56 2023-07-02 21:09:58.000000 alienpy-1.5.2/alienpy.egg-info/requires.txt
+-rw-r--r--   0 adrian    (1000) adrian    (1000)        8 2023-07-02 21:09:58.000000 alienpy-1.5.2/alienpy.egg-info/top_level.txt
+drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-02 21:09:58.623886 alienpy-1.5.2/examples/
+-rwxr-xr-x   0 adrian    (1000) adrian    (1000)     2169 2022-12-20 08:02:48.000000 alienpy-1.5.2/examples/alien_wbtime
+-rw-r--r--   0 adrian    (1000) adrian    (1000)       38 2023-07-02 21:09:58.624886 alienpy-1.5.2/setup.cfg
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     4160 2023-06-06 11:45:37.000000 alienpy-1.5.2/setup.py
```

### Comparing `alienpy-1.5.1/LICENSE` & `alienpy-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alienpy-1.5.1/PKG-INFO` & `alienpy-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alienpy
-Version: 1.5.1
+Version: 1.5.2
 Summary: Websocket based cli interface for ALICE experiment GRID infrastructure
 Home-page: https://gitlab.cern.ch/jalien/xjalienfs
 Author: Adrian Sevcenco
 Author-email: adrian.sevcenco@cern.ch
 Project-URL: Dev git, https://github.com/adriansev/jalien_py
 Project-URL: Issues, https://github.com/adriansev/jalien_py/issues
 Project-URL: Changelog, https://github.com/adriansev/jalien_py/commits/master
```

### Comparing `alienpy-1.5.1/README.md` & `alienpy-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `alienpy-1.5.1/alienpy/alien.py` & `alienpy-1.5.2/alienpy/alien.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import subprocess  # nosec
 import logging
 import shlex
 import statistics
 from typing import Union
 import time
 from urllib.parse import urlparse
+import uuid
 
 # External imports
 try:
     import requests
 except Exception:
     print("requests module could not be imported! Make sure you can do:\npython3 -c 'import requests'", file = sys.stderr, flush = True)
     sys.exit(1)
@@ -72,14 +73,16 @@
 from .xrd_tools import lfn2meta, lfn2uri, expand_path_grid, extract_glob_pattern, list_files_grid
 from .xrd_core import (xrd_config_init, HAS_XROOTD, xrd_client, DO_XrootdCp,
                        xrdfs_ping, xrdfs_q_config, xrdfs_q_stats, xrdstat2dict, xrdfs_stat, xrdstat_flags2dict,
                        download_tmp, upload_tmp)
 # Global XRootD preferences
 xrd_config_init()
 
+session_id = None  # variable used to keep a session ID
+
 ##################################
 #   START FUNCTIONS DEFINITIONS
 ##################################
 
 
 def DO_dirs(wb, args: Union[str, list, None] = None) -> RET:
     """dirs"""
@@ -639,14 +642,15 @@
             job_list_messages.append(f'{job_info}{machine_info}{state_info}{trace_info if show_trace else ""}{proc_info if show_proc else ""}')
 
     return RET(0, f'{os.linesep}'.join(job_list_messages), '', job_processed_list)
 
 
 def DO_ccdb_query(args: list = None) -> RET:
     """Query CCDB for object data"""
+    global session_id
     if not args: return RET(2, '', 'empty query! Use at least a "/" as argument')
 
     if is_help(args):
         return RET(0, '''ccdb [-host FQDN] [-history] [-nicetime] QUERY
 where query has the form of:
 task name / detector name / start time [ / UUID]
 or
@@ -655,35 +659,46 @@
 -host: specify other ccdb server than alice-ccdb.cern.ch
 -history: use browse to list the whole history of the object
 -unixtime: print the unixtime
 -get: download the specified object/objects - full path will be kept
 -dst: set a specific destination for download
 ''' )
 
-    headers = { 'user-agent': f'alien.py/{ALIENPY_VERSION_STR}', 'Accept': 'application/json', 'Accept-encoding': 'gzip, deflate', }
-
     listing_type = 'browse/' if get_arg(args, '-history') else 'latest/'
     ccdb_default_host = 'http://alice-ccdb.cern.ch/'
     host_arg = get_arg_value(args, '-host')
     do_unixtime = get_arg(args, '-unixtime')
     do_download = get_arg(args, '-get')
+    run_nr = get_arg_value(args, '-run')
+    limit_results = get_arg_value(args, '-limit')
+    if not limit_results: limit_results = 10
 
     dest_arg = get_arg_value(args, '-dst')
     if not dest_arg: dest_arg = '.'
     if not dest_arg.endswith('/'): dest_arg = f'{dest_arg}/'
 
     ccdb = host_arg if host_arg else ccdb_default_host
     if not ccdb.endswith('/'): ccdb = f'{ccdb}/'
     if not ccdb.startswith('http://') and not ccdb.startswith('https://'): ccdb = f'http://{ccdb}'
 
     if not args: return RET(2, '', 'empty query!')
     query_str = args[0]  # after removal of args assume the rest is the query
+    query_str = query_str.replace('.*', '').replace('*', '')
+
+    if run_nr: query_str = f'{query_str}/runNumber={run_nr}'
+    if not session_id: session_id = str(uuid.uuid1())
+
+    headers = { 'User-Agent': f'alien.py/{ALIENPY_VERSION_STR} id/{os.getlogin()}@{os.uname()[1]} session/{session_id}', 'Accept': 'application/json', 'Accept-encoding': 'gzip, deflate', 'Browse-Limit': str(limit_results), }
 
     q = requests.get(f'{ccdb}{listing_type}{query_str}', headers = headers, timeout = 5)
-    q_dict = q.json()
+    try:
+        q_dict = q.json()
+    except Exception:
+        return RET(1, '', f'Invalid answer (no json) from query:\n{ccdb}{listing_type}{query_str}')
+
     # q_path = q_dict.pop('path')
     # q_latest = q_dict.pop('latest')
     # q_patternMatching = q_dict.pop('patternMatching')
     list(map(ccdb_json_cleanup, q_dict['objects']))
 
     if not do_unixtime:
         if 'validAt' in q_dict: q_dict['validAt'] = unixtime2local(q_dict['validAt'])
```

### Comparing `alienpy-1.5.1/alienpy/async_tools.py` & `alienpy-1.5.2/alienpy/async_tools.py`

 * *Files identical despite different names*

### Comparing `alienpy-1.5.1/alienpy/connect_ssl.py` & `alienpy-1.5.2/alienpy/connect_ssl.py`

 * *Files identical despite different names*

### Comparing `alienpy-1.5.1/alienpy/data_structs.py` & `alienpy-1.5.2/alienpy/data_structs.py`

 * *Files identical despite different names*

### Comparing `alienpy-1.5.1/alienpy/global_vars.py` & `alienpy-1.5.2/alienpy/global_vars.py`

 * *Files identical despite different names*

### Comparing `alienpy-1.5.1/alienpy/setup_cwd.py` & `alienpy-1.5.2/alienpy/setup_cwd.py`

 * *Files identical despite different names*

### Comparing `alienpy-1.5.1/alienpy/setup_logging.py` & `alienpy-1.5.2/alienpy/setup_logging.py`

 * *Files identical despite different names*

### Comparing `alienpy-1.5.1/alienpy/tools_history.py` & `alienpy-1.5.2/alienpy/tools_history.py`

 * *Files identical despite different names*

### Comparing `alienpy-1.5.1/alienpy/tools_nowb.py` & `alienpy-1.5.2/alienpy/tools_nowb.py`

 * *Files 0% similar despite different names*

```diff
@@ -488,22 +488,27 @@
     if not path: return ''
     p = Path(path)
     if p.is_dir(): return str('d')
     if p.is_file(): return str('f')
     return ''
 
 
-def fileIsValid(filename: str, size: Union[str, int], reported_md5: str, shallow_check: bool = False) -> RET:
+def fileIsValid(filename: str, size: Union[str, int], mtime: Union[str, int], reported_md5: str, shallow_check: bool = False) -> RET:
     """Check if the file path is consistent with the size and md5 argument. N.B.! the local file will be deleted with size,md5 not match"""
     if os.path.isfile(filename):  # first check
-        if int(os.stat(filename).st_size) != int(size):
+        stat_info = os.stat(filename)
+        local_file_mtime = int(stat_info.st_mtime*1000)
+        if int(stat_info.st_size) != int(size):
             os.remove(filename)
             return RET(9, '', f'{filename} : Removed (invalid size)')
+        if local_file_mtime < int(mtime):  # if the age of local file is > age of lfn then lfn is modified and newer
+            os.remove(filename)
+            return RET(9, '', f'{filename} : Removed (lfn is newer than local file)')
         if shallow_check:
-            return RET(0, f'{filename} --> TARGET VALID (size match)')
+            return RET(0, f'{filename} --> TARGET VALID (size match, local age is lower than remote)')
         if md5(filename) != reported_md5:
             os.remove(filename)
             return RET(9, '', f'{filename} : Removed (invalid md5)')
         return RET(0, f'{filename} --> TARGET VALID (md5 match)')
     return RET(2, '', f'{filename} : No such file')  # ENOENT
 
 
@@ -621,16 +626,16 @@
     norm_path = expand_path_local(path)
     if not os.path.exists(norm_path): return STAT_FILEPATH(norm_path)
     filetype = 'd' if os.path.isdir(norm_path) else 'f'
     statinfo = os.stat(norm_path)
     perm = oct(statinfo.st_mode)[-3:]
     uid = uid2name(statinfo.st_uid)
     gid = gid2name(statinfo.st_gid)
-    ctime = str(statinfo.st_ctime)
-    mtime = str(statinfo.st_mtime)
+    ctime = str(statinfo.st_ctime)  # metadata modification
+    mtime = str(statinfo.st_mtime)  # content modification
     guid = ''
     size = str(statinfo.st_size)
     md5hash = ''
     if do_md5 and filetype == 'f': md5hash = md5(norm_path)
     return STAT_FILEPATH(norm_path, filetype, perm, uid, gid, ctime, mtime, guid, size, md5hash)
```

### Comparing `alienpy-1.5.1/alienpy/tools_shell.py` & `alienpy-1.5.2/alienpy/tools_shell.py`

 * *Files identical despite different names*

### Comparing `alienpy-1.5.1/alienpy/tools_stackcmd.py` & `alienpy-1.5.2/alienpy/tools_stackcmd.py`

 * *Files identical despite different names*

### Comparing `alienpy-1.5.1/alienpy/wb_api.py` & `alienpy-1.5.2/alienpy/wb_api.py`

 * *Files identical despite different names*

### Comparing `alienpy-1.5.1/alienpy/wb_async.py` & `alienpy-1.5.2/alienpy/wb_async.py`

 * *Files identical despite different names*

### Comparing `alienpy-1.5.1/alienpy/xrd_core.py` & `alienpy-1.5.2/alienpy/xrd_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
     # Default value for the time after which an error is declared if it was impossible to get a response to a request.
     # N.B.!!. This is the total time for the initialization dialogue!! see https://xrootd.slac.stanford.edu/doc/xrdcl-docs/www/xrdcldocs.html#x1-580004.3.6
     if not os.getenv('XRD_REQUESTTIMEOUT'): XRD_EnvPut('RequestTimeout', int(1200))  # default 1800
 
     # Default value for the time after which a connection error is declared (and a recovery attempted) if there are unfulfilled requests and there is no socket activity or a registered wait timeout.
     # N.B.!!. we actually want this timeout for failure on onverloaded/unresponsive server. see https://github.com/xrootd/xrootd/issues/1597#issuecomment-1064081574
-    if not os.getenv('XRD_STREAMTIMEOUT'): XRD_EnvPut('StreamTimeout', int(20))  # default 60
+    if not os.getenv('XRD_STREAMTIMEOUT'): XRD_EnvPut('StreamTimeout', int(60))  # default 60
 
     # Maximum time allowed for the copy process to initialize, ie. open the source and destination files.
     if not os.getenv('XRD_CPINITTIMEOUT'): XRD_EnvPut('CPInitTimeout', int(300))  # default 600
 
     # Time period after which an idle connection to a data server should be closed.
     if not os.getenv('XRD_DATASERVERTTL'): XRD_EnvPut('DataServerTTL', int(20))  # we have no reasons to keep idle connections
 
@@ -208,31 +208,31 @@
     error_msg = ''  # container which accumulates the error messages
     isWrite = not isDownload
     if isDownload:  # pylint: disable=too-many-nested-blocks  # src is GRID, we are DOWNLOADING from GRID location
         # to reduce the remote calls we treat files and directory on separate code-paths
         if src_stat.type == 'f':  # single file
             dst_filename = format_dst_fn(src, src, dst, parent)
             # if overwrite the file validity checking will do md5
-            skip_file = (retf_print(fileIsValid(dst_filename, src_stat.size, src_stat.md5, shallow_check = not overwrite), opts = 'noerr') == 0)
 
+            skip_file = (retf_print(fileIsValid(dst_filename, src_stat.size, src_stat.mtime, src_stat.md5, shallow_check = not overwrite), opts = 'noerr') == 0)
             if not skip_file:
                 tokens = lfn2fileTokens(wb, lfn2file(src, dst_filename), specs_list, isWrite, strictspec, httpurl)
                 if tokens and 'answer' in tokens:
                     copy_list.append(CopyFile(src, dst_filename, isWrite, tokens['answer'], src))
         else:  # directory to be listed
             results_list = list_files_grid(wb, src, pattern, is_regex, " ".join(find_args))
             if "results" not in results_list.ansdict or len(results_list.ansdict["results"]) < 1:
                 msg = f"No files found with: find {' '.join(find_args) if find_args else ''}{' -r ' if is_regex else ''} -a -s {src} {pattern}"
                 return RET(42, '', msg)  # ENOMSG /* No message of desired type */
 
             for lfn_obj in results_list.ansdict["results"]:  # make CopyFile objs for each lfn
                 lfn = get_lfn_key(lfn_obj)
                 dst_filename = format_dst_fn(src, lfn, dst, parent)
                 # if overwrite the file validity checking will do md5
-                skip_file = (retf_print(fileIsValid(dst_filename, lfn_obj['size'], lfn_obj['md5'], shallow_check = not overwrite), opts = 'noerr') == 0)
+                skip_file = (retf_print(fileIsValid(dst_filename, lfn_obj['size'], lfn_obj['ctime'], lfn_obj['md5'], shallow_check = not overwrite), opts = 'noerr') == 0)
                 if skip_file: continue  # destination exists and is valid, no point to re-download
 
                 tokens = lfn2fileTokens(wb, lfn2file(lfn, dst_filename), specs_list, isWrite, strictspec, httpurl)
                 if not tokens or 'answer' not in tokens: continue
                 copy_list.append(CopyFile(lfn, dst_filename, isWrite, tokens['answer'], lfn))
 
     else:  # src is LOCAL, we are UPLOADING
@@ -386,15 +386,15 @@
         XRD_EnvPut('CpRetry', retry)
 
     _use_system_xrdcp = get_arg(xrd_copy_command, '-xrdcp')
     f_arg = get_arg(xrd_copy_command, '-f')
     if f_arg:
         print_out('No longer used flag! md5 verification of present destination is default; disable with -fastcheck')
 
-    fastcheck = get_arg(xrd_copy_command, '-fastcheck')
+    fastcheck = get_arg(xrd_copy_command, '-fastcheck') or get_arg(xrd_copy_command, '-skipmd5')
     overwrite = not fastcheck
 
     get_arg(xrd_copy_command, '-cksum')
     cksum = True
 
     dryrun = get_arg(xrd_copy_command, '-dryrun')
```

### Comparing `alienpy-1.5.1/alienpy/xrd_tools.py` & `alienpy-1.5.2/alienpy/xrd_tools.py`

 * *Files identical despite different names*

### Comparing `alienpy-1.5.1/alienpy.egg-info/PKG-INFO` & `alienpy-1.5.2/alienpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alienpy
-Version: 1.5.1
+Version: 1.5.2
 Summary: Websocket based cli interface for ALICE experiment GRID infrastructure
 Home-page: https://gitlab.cern.ch/jalien/xjalienfs
 Author: Adrian Sevcenco
 Author-email: adrian.sevcenco@cern.ch
 Project-URL: Dev git, https://github.com/adriansev/jalien_py
 Project-URL: Issues, https://github.com/adriansev/jalien_py/issues
 Project-URL: Changelog, https://github.com/adriansev/jalien_py/commits/master
```

### Comparing `alienpy-1.5.1/alienpy.egg-info/SOURCES.txt` & `alienpy-1.5.2/alienpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alienpy-1.5.1/alienpy.egg-info/entry_points.txt` & `alienpy-1.5.2/alienpy.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `alienpy-1.5.1/examples/alien_wbtime` & `alienpy-1.5.2/examples/alien_wbtime`

 * *Files identical despite different names*

### Comparing `alienpy-1.5.1/setup.py` & `alienpy-1.5.2/setup.py`

 * *Files identical despite different names*

