# Comparing `tmp/aicoder-0.2.1-py3-none-any.whl.zip` & `tmp/aicoder-0.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 21442 bytes, number of entries: 12
+Zip file size: 21450 bytes, number of entries: 12
 -rw-r--r--  2.0 unx    12669 b- defN 23-Jun-30 12:05 aicoder/AICoder.py
 -rw-r--r--  2.0 unx     8088 b- defN 23-Jun-30 12:27 aicoder/AICoderFull.py
 -rw-r--r--  2.0 unx     5449 b- defN 23-Jun-30 12:04 aicoder/AICoderPartial.py
 -rw-r--r--  2.0 unx     3571 b- defN 23-Jun-30 12:29 aicoder/AICoderPrompts.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-29 11:14 aicoder/__init__.py
--rw-r--r--  2.0 unx    14599 b- defN 23-Jun-30 12:18 aicoder/main.py
--rw-r--r--  2.0 unx    18809 b- defN 23-Jul-02 13:22 aicoder-0.2.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      473 b- defN 23-Jul-02 13:22 aicoder-0.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-02 13:22 aicoder-0.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       46 b- defN 23-Jul-02 13:22 aicoder-0.2.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-02 13:22 aicoder-0.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      945 b- defN 23-Jul-02 13:22 aicoder-0.2.1.dist-info/RECORD
-12 files, 64749 bytes uncompressed, 19862 bytes compressed:  69.3%
+-rw-r--r--  2.0 unx    14606 b- defN 23-Jul-02 14:09 aicoder/main.py
+-rw-r--r--  2.0 unx    18809 b- defN 23-Jul-02 14:11 aicoder-0.2.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      473 b- defN 23-Jul-02 14:11 aicoder-0.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-02 14:11 aicoder-0.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       46 b- defN 23-Jul-02 14:11 aicoder-0.2.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-02 14:11 aicoder-0.2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      945 b- defN 23-Jul-02 14:11 aicoder-0.2.2.dist-info/RECORD
+12 files, 64756 bytes uncompressed, 19870 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: aicoder/__init__.py
 Comment: 
 
 Filename: aicoder/main.py
 Comment: 
 
-Filename: aicoder-0.2.1.dist-info/LICENSE
+Filename: aicoder-0.2.2.dist-info/LICENSE
 Comment: 
 
-Filename: aicoder-0.2.1.dist-info/METADATA
+Filename: aicoder-0.2.2.dist-info/METADATA
 Comment: 
 
-Filename: aicoder-0.2.1.dist-info/WHEEL
+Filename: aicoder-0.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: aicoder-0.2.1.dist-info/entry_points.txt
+Filename: aicoder-0.2.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: aicoder-0.2.1.dist-info/top_level.txt
+Filename: aicoder-0.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: aicoder-0.2.1.dist-info/RECORD
+Filename: aicoder-0.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aicoder/main.py

```diff
@@ -148,25 +148,25 @@
     file_bug_fixer_parser.add_argument('--orig-branch', default=None, type=str, help='Branch to upload the changes.')
     file_bug_fixer_parser.add_argument('--to-branch', default=None, type=str, help='Branch to send the PR to.')
     file_bug_fixer_parser.add_argument('--repo-name', default=None, type=str, help='Indicate the name of the repo: org_name/repo_name')
     
     # Parse arguments
     args = parser.parse_args()
     prompt = os.environ.get("INPUT_PROMPT") or (args.prompt if hasattr(args,"prompt") else None)
-    api_key = os.environ.get("INPUT_API_KEY") or (args.api_key if hasattr(args,"api_key") else None)
+    api_key = os.environ.get("INPUT_OPENAI_API_KEY") or (args.api_key if hasattr(args,"api_key") else None)
     model = os.environ.get("INPUT_MODEL") or (args.model if hasattr(args,"model") else None)
 
     if args.mode in ["file-generator", "file-enhancer", "file-comments", "file-security", "file-optimizer", "file-bugfixer"]:
         github_token = os.environ.get("GITHUB_TOKEN") or args.github_token
         orig_branch = os.environ.get("ORIGIN_BRANCH") or args.orig_branch
         to_branch = os.environ.get("TO_BRANCH") or args.to_branch
         repo_name = os.environ.get("GITHUB_REPOSITORY") or args.repo_name or get_git_org_repo_name()
 
         if args.mode == "file-generator":
-            template_files = list(os.environ.get("TEMPALTE_FILES").split(",")) or args.template_files
+            template_files = list(os.environ.get("TEMPLATE_FILES").split(",")) or args.template_files
                 
         elif args.mode in ["file-enhancer", "file-comments", "file-security", "file-optimizer", "file-bugfixer"]:
             check_path = os.environ.get("CHECK_PATH") or args.path
     
     if not prompt and not args.mode in ["file-comments", "file-security", "file-optimizer"]:
         logger.error("Error: Missing prompt.")
         parser.print_help()
```

## Comparing `aicoder-0.2.1.dist-info/LICENSE` & `aicoder-0.2.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `aicoder-0.2.1.dist-info/RECORD` & `aicoder-0.2.2.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 aicoder/AICoder.py,sha256=JD6NVUiqbQH9yKxSCeoynQwcIWDrWJCuipwwoqFJ8sA,12669
 aicoder/AICoderFull.py,sha256=ZmQtR3QrZs4hSXPaSdeMgfBSHYITpadujk3HL6Wat_Y,8088
 aicoder/AICoderPartial.py,sha256=_NadBlkGml2FSfK0gJPyN4zVUkQpe6e6nwAeywmJlEI,5449
 aicoder/AICoderPrompts.py,sha256=EyVLCIKkUDACV0swEHWVfRPNU_cQwYbLIIQ8nFI2VJY,3571
 aicoder/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-aicoder/main.py,sha256=A1N1pSQoReeKAbF8of0kJgGxvC8YW_32cA7aLnZ5cDk,14599
-aicoder-0.2.1.dist-info/LICENSE,sha256=nGKG3YDYTyar3KKwoaLPInTfnNQtuvh4aMwTADTd0L8,18809
-aicoder-0.2.1.dist-info/METADATA,sha256=OWyY3d3qbrfm6rhz9do3t7uv2SvJFLWAYYj41viemx0,473
-aicoder-0.2.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-aicoder-0.2.1.dist-info/entry_points.txt,sha256=m__okhQaM4kZ8CCfSA5VGUyQ0gf7TIGax6DhXdTnAeA,46
-aicoder-0.2.1.dist-info/top_level.txt,sha256=B8Pf-hhM5icZE_7vMCXD5mXWG0MAqt5ImotI1aNXdWQ,8
-aicoder-0.2.1.dist-info/RECORD,,
+aicoder/main.py,sha256=WYdFffXI3V3r6sI8wcF_FBC_Dsm1VmQ_l9x6mFDZvZ4,14606
+aicoder-0.2.2.dist-info/LICENSE,sha256=nGKG3YDYTyar3KKwoaLPInTfnNQtuvh4aMwTADTd0L8,18809
+aicoder-0.2.2.dist-info/METADATA,sha256=tKSj-bBDFHVF7JsM620-9AhIW3GaBIk6d42oO7NI24Q,473
+aicoder-0.2.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+aicoder-0.2.2.dist-info/entry_points.txt,sha256=m__okhQaM4kZ8CCfSA5VGUyQ0gf7TIGax6DhXdTnAeA,46
+aicoder-0.2.2.dist-info/top_level.txt,sha256=B8Pf-hhM5icZE_7vMCXD5mXWG0MAqt5ImotI1aNXdWQ,8
+aicoder-0.2.2.dist-info/RECORD,,
```

