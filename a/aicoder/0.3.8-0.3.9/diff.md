# Comparing `tmp/aicoder-0.3.8-py3-none-any.whl.zip` & `tmp/aicoder-0.3.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 21652 bytes, number of entries: 12
+Zip file size: 21651 bytes, number of entries: 12
 -rw-r--r--  2.0 unx    12662 b- defN 23-Jul-02 16:18 aicoder/AICoder.py
 -rw-r--r--  2.0 unx     8087 b- defN 23-Jul-02 16:18 aicoder/AICoderFull.py
 -rw-r--r--  2.0 unx     7160 b- defN 23-Jul-02 16:18 aicoder/AICoderPartial.py
 -rw-r--r--  2.0 unx     3571 b- defN 23-Jun-30 12:29 aicoder/AICoderPrompts.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-29 11:14 aicoder/__init__.py
--rw-r--r--  2.0 unx    14753 b- defN 23-Jul-02 16:45 aicoder/main.py
--rw-r--r--  2.0 unx    18809 b- defN 23-Jul-02 16:46 aicoder-0.3.8.dist-info/LICENSE
--rw-r--r--  2.0 unx      473 b- defN 23-Jul-02 16:46 aicoder-0.3.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-02 16:46 aicoder-0.3.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       46 b- defN 23-Jul-02 16:46 aicoder-0.3.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-02 16:46 aicoder-0.3.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      945 b- defN 23-Jul-02 16:46 aicoder-0.3.8.dist-info/RECORD
-12 files, 66606 bytes uncompressed, 20072 bytes compressed:  69.9%
+-rw-r--r--  2.0 unx    14810 b- defN 23-Jul-02 16:54 aicoder/main.py
+-rw-r--r--  2.0 unx    18809 b- defN 23-Jul-02 16:54 aicoder-0.3.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx      473 b- defN 23-Jul-02 16:54 aicoder-0.3.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-02 16:54 aicoder-0.3.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       46 b- defN 23-Jul-02 16:54 aicoder-0.3.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-02 16:54 aicoder-0.3.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      945 b- defN 23-Jul-02 16:54 aicoder-0.3.9.dist-info/RECORD
+12 files, 66663 bytes uncompressed, 20071 bytes compressed:  69.9%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: aicoder/__init__.py
 Comment: 
 
 Filename: aicoder/main.py
 Comment: 
 
-Filename: aicoder-0.3.8.dist-info/LICENSE
+Filename: aicoder-0.3.9.dist-info/LICENSE
 Comment: 
 
-Filename: aicoder-0.3.8.dist-info/METADATA
+Filename: aicoder-0.3.9.dist-info/METADATA
 Comment: 
 
-Filename: aicoder-0.3.8.dist-info/WHEEL
+Filename: aicoder-0.3.9.dist-info/WHEEL
 Comment: 
 
-Filename: aicoder-0.3.8.dist-info/entry_points.txt
+Filename: aicoder-0.3.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: aicoder-0.3.8.dist-info/top_level.txt
+Filename: aicoder-0.3.9.dist-info/top_level.txt
 Comment: 
 
-Filename: aicoder-0.3.8.dist-info/RECORD
+Filename: aicoder-0.3.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aicoder/main.py

```diff
@@ -147,23 +147,25 @@
     if args.mode in ["file-generator", "file-enhancer", "file-comments", "file-security", "file-optimizer", "file-bugfixer"]:
         github_token = os.environ.get("GITHUB_TOKEN") or args.github_token
         orig_branch = os.environ.get("ORIGIN_BRANCH") or args.orig_branch
         to_branch = os.environ.get("TO_BRANCH") or args.to_branch
         repo_name = os.environ.get("GITHUB_REPOSITORY") or args.repo_name or get_git_org_repo_name()
 
         if args.mode == "file-generator":
-            template_files = list(os.environ.get("TEMPLATE_FILES").split(",")) or args.template_files.split(',')
-            final_file_path = list(os.environ.get("FINAL_FILE_PATH").split(",")) or args.file_path
+            template_files = os.environ.get("TEMPLATE_FILES") or args.template_files
+            template_files = list(template_files.strip().split(","))
+            final_file_path = os.environ.get("FINAL_FILE_PATH") or args.file_path
             if not template_files or not final_file_path:
                 logger.error("Error: Missing template_files or final_file_path.")
                 parser.print_help()
                 sys.exit(1)
                 
         elif args.mode in ["file-enhancer", "file-comments", "file-security", "file-optimizer", "file-bugfixer"]:
-            check_paths = os.environ.get("CHECK_PATHS").split(',') or args.paths.split(',')
+            check_paths = os.environ.get("CHECK_PATHS") or args.paths
+            check_paths = list(check_paths.split(","))
             if not check_paths:
                 logger.error("Error: Missing check_paths.")
                 parser.print_help()
                 sys.exit(1)
     
     if not prompt and not args.mode in ["file-comments", "file-security", "file-optimizer"]:
         logger.error("Error: Missing prompt.")
```

## Comparing `aicoder-0.3.8.dist-info/LICENSE` & `aicoder-0.3.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `aicoder-0.3.8.dist-info/RECORD` & `aicoder-0.3.9.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 aicoder/AICoder.py,sha256=83hZ7Sdvyd0wtiJE5kPLSaAt7wIC6BlN8MVYaaehwiw,12662
 aicoder/AICoderFull.py,sha256=VjCIDZZMCVoCsnn1XVVyizhplfxDLlS-V30iW3r0TCk,8087
 aicoder/AICoderPartial.py,sha256=nClKfFoVbRZpoM2rLIeQoOtllSD8dMAHNuiFyLj-kcA,7160
 aicoder/AICoderPrompts.py,sha256=EyVLCIKkUDACV0swEHWVfRPNU_cQwYbLIIQ8nFI2VJY,3571
 aicoder/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-aicoder/main.py,sha256=iNm9RVeWfLgEqO-OKTJuw4KWLh3BdI2vwHmR4WBxE54,14753
-aicoder-0.3.8.dist-info/LICENSE,sha256=nGKG3YDYTyar3KKwoaLPInTfnNQtuvh4aMwTADTd0L8,18809
-aicoder-0.3.8.dist-info/METADATA,sha256=VeVctvtJVl53llSu2G8NOQnaoZX_AR8uAvCAI3Rz4Nk,473
-aicoder-0.3.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-aicoder-0.3.8.dist-info/entry_points.txt,sha256=m__okhQaM4kZ8CCfSA5VGUyQ0gf7TIGax6DhXdTnAeA,46
-aicoder-0.3.8.dist-info/top_level.txt,sha256=B8Pf-hhM5icZE_7vMCXD5mXWG0MAqt5ImotI1aNXdWQ,8
-aicoder-0.3.8.dist-info/RECORD,,
+aicoder/main.py,sha256=EX5ONXJ75jaCpoRo0oUQfMESx9JAdzowDyqpaeDAw0Y,14810
+aicoder-0.3.9.dist-info/LICENSE,sha256=nGKG3YDYTyar3KKwoaLPInTfnNQtuvh4aMwTADTd0L8,18809
+aicoder-0.3.9.dist-info/METADATA,sha256=F43E6NuIG8n0fm8FWRDA5Ssji0CymY8QOGgLCxj93eE,473
+aicoder-0.3.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+aicoder-0.3.9.dist-info/entry_points.txt,sha256=m__okhQaM4kZ8CCfSA5VGUyQ0gf7TIGax6DhXdTnAeA,46
+aicoder-0.3.9.dist-info/top_level.txt,sha256=B8Pf-hhM5icZE_7vMCXD5mXWG0MAqt5ImotI1aNXdWQ,8
+aicoder-0.3.9.dist-info/RECORD,,
```

