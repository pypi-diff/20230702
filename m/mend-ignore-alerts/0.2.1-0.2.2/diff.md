# Comparing `tmp/mend_ignore_alerts-0.2.1-py3-none-any.whl.zip` & `tmp/mend_ignore_alerts-0.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 11777 bytes, number of entries: 11
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-02 16:23 mend_ignore_alerts/__init__.py
--rw-r--r--  2.0 unx      107 b- defN 23-Jul-02 16:23 mend_ignore_alerts/_version.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-02 16:23 mend_ignore_alerts/conftest.py
--rw-r--r--  2.0 unx     1554 b- defN 23-Jul-02 16:23 mend_ignore_alerts/const.py
--rw-r--r--  2.0 unx    10597 b- defN 23-Jul-02 16:23 mend_ignore_alerts/ignore_alerts.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jul-02 16:23 mend_ignore_alerts-0.2.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     5250 b- defN 23-Jul-02 16:23 mend_ignore_alerts-0.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-02 16:23 mend_ignore_alerts-0.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       72 b- defN 23-Jul-02 16:23 mend_ignore_alerts-0.2.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       19 b- defN 23-Jul-02 16:23 mend_ignore_alerts-0.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      979 b- defN 23-Jul-02 16:23 mend_ignore_alerts-0.2.1.dist-info/RECORD
-11 files, 30027 bytes uncompressed, 10085 bytes compressed:  66.4%
+Zip file size: 11809 bytes, number of entries: 11
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-02 17:10 mend_ignore_alerts/__init__.py
+-rw-r--r--  2.0 unx      107 b- defN 23-Jul-02 17:10 mend_ignore_alerts/_version.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-02 17:10 mend_ignore_alerts/conftest.py
+-rw-r--r--  2.0 unx     1554 b- defN 23-Jul-02 17:10 mend_ignore_alerts/const.py
+-rw-r--r--  2.0 unx    10673 b- defN 23-Jul-02 17:10 mend_ignore_alerts/ignore_alerts.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-02 17:11 mend_ignore_alerts-0.2.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5250 b- defN 23-Jul-02 17:11 mend_ignore_alerts-0.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-02 17:11 mend_ignore_alerts-0.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       72 b- defN 23-Jul-02 17:11 mend_ignore_alerts-0.2.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       19 b- defN 23-Jul-02 17:11 mend_ignore_alerts-0.2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      979 b- defN 23-Jul-02 17:11 mend_ignore_alerts-0.2.2.dist-info/RECORD
+11 files, 30103 bytes uncompressed, 10117 bytes compressed:  66.4%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: mend_ignore_alerts/const.py
 Comment: 
 
 Filename: mend_ignore_alerts/ignore_alerts.py
 Comment: 
 
-Filename: mend_ignore_alerts-0.2.1.dist-info/LICENSE
+Filename: mend_ignore_alerts-0.2.2.dist-info/LICENSE
 Comment: 
 
-Filename: mend_ignore_alerts-0.2.1.dist-info/METADATA
+Filename: mend_ignore_alerts-0.2.2.dist-info/METADATA
 Comment: 
 
-Filename: mend_ignore_alerts-0.2.1.dist-info/WHEEL
+Filename: mend_ignore_alerts-0.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: mend_ignore_alerts-0.2.1.dist-info/entry_points.txt
+Filename: mend_ignore_alerts-0.2.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: mend_ignore_alerts-0.2.1.dist-info/top_level.txt
+Filename: mend_ignore_alerts-0.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: mend_ignore_alerts-0.2.1.dist-info/RECORD
+Filename: mend_ignore_alerts-0.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mend_ignore_alerts/_version.py

```diff
@@ -1,3 +1,3 @@
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 __tool_name__ = "ignore_alerts"
 __description__ = "Parse yml file and update alerts"
```

## mend_ignore_alerts/ignore_alerts.py

```diff
@@ -66,16 +66,16 @@
     parser = argparse.ArgumentParser(description=__description__)
     parser.add_argument(*aliases.get_aliases_str("userkey"), help="Mend user key", dest='ws_user_key',
                         default=varenvs.get_env("wsuserkey"), required=not varenvs.get_env("wsuserkey"))
     parser.add_argument(*aliases.get_aliases_str("apikey"), help="Mend API key", dest='ws_token',
                         default=varenvs.get_env("wsapikey"), required=not varenvs.get_env("wsapikey"))
     parser.add_argument(*aliases.get_aliases_str("url"), help="Mend server URL", dest='ws_url',
                         default=varenvs.get_env("wsurl"), required=not varenvs.get_env("wsurl"))
-    parser.add_argument(*aliases.get_aliases_str("projectkey"), help="Mend project scope", dest='scope_token',
-                        default=varenvs.get_env("wsproject"))
+    #parser.add_argument(*aliases.get_aliases_str("projectkey"), help="Mend project scope", dest='scope_token',
+    #                    default=varenvs.get_env("wsproject"))
     parser.add_argument(*aliases.get_aliases_str("yaml"), help="YAML file", dest='yaml',
                         default=varenvs.get_env("waiver"), required=not varenvs.get_env("waiver"))
     parser.add_argument(*aliases.get_aliases_str("githubpat"), help="GitHub PAT", dest='pat',
                         default=varenvs.get_env("githubpat"))
     parser.add_argument(*aliases.get_aliases_str("githubrepo"), help="GitHub Repo", dest='repo',
                         default=varenvs.get_env("githubrepo"))
     parser.add_argument(*aliases.get_aliases_str("githubowner"), help="GitHub Owner", dest='owner',
@@ -266,18 +266,18 @@
     hdr_title = f'{APP_TITLE} {__version__}'
     hdr = f'\n{len(hdr_title)*"="}\n{hdr_title}\n{len(hdr_title)*"="}'
     logger.info(hdr)
     input_data = None
 
     try:
         args = parse_args()
-        if args.pat and args.repo and args.owner:
+        if args.pat and args.repo and (args.owner or "/" in args.repo):
             try:
                 g = Github(args.pat)
-                repo = g.get_repo(f'{args.owner}/{args.repo}')
+                repo = g.get_repo(f'{args.repo}') if "/" in args.repo else g.get_repo(f'{args.owner}/{args.repo}')
                 input_data = repo.get_contents(args.yaml).decoded_content.decode("utf-8")
             except Exception as err:
                 logger.error(f"Access to {args.owner}/{args.repo} forbidden")
         #create_waiver()
         logger.info(f'[{fn()}] Getting project list')
         load_prj = json.dumps({
             "requestType" : "getOrganizationProjectVitals",
```

## Comparing `mend_ignore_alerts-0.2.1.dist-info/LICENSE` & `mend_ignore_alerts-0.2.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mend_ignore_alerts-0.2.1.dist-info/METADATA` & `mend_ignore_alerts-0.2.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mend-ignore-alerts
-Version: 0.2.1
+Version: 0.2.2
 Summary: Parse yml file and update alerts
 Home-page: https://github.com/mend-toolkit/ignore-alerts
 Author: Mend Professional Services
 Author-email: ps@mend.io
 License: LICENSE.txt
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

