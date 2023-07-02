# Comparing `tmp/aicoder-0.3.6-py3-none-any.whl.zip` & `tmp/aicoder-0.3.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 21548 bytes, number of entries: 12
+Zip file size: 21618 bytes, number of entries: 12
 -rw-r--r--  2.0 unx    12662 b- defN 23-Jul-02 16:18 aicoder/AICoder.py
 -rw-r--r--  2.0 unx     8087 b- defN 23-Jul-02 16:18 aicoder/AICoderFull.py
 -rw-r--r--  2.0 unx     7160 b- defN 23-Jul-02 16:18 aicoder/AICoderPartial.py
 -rw-r--r--  2.0 unx     3571 b- defN 23-Jun-30 12:29 aicoder/AICoderPrompts.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-29 11:14 aicoder/__init__.py
--rw-r--r--  2.0 unx    14035 b- defN 23-Jul-02 16:25 aicoder/main.py
--rw-r--r--  2.0 unx    18809 b- defN 23-Jul-02 16:27 aicoder-0.3.6.dist-info/LICENSE
--rw-r--r--  2.0 unx      473 b- defN 23-Jul-02 16:27 aicoder-0.3.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-02 16:27 aicoder-0.3.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       46 b- defN 23-Jul-02 16:27 aicoder-0.3.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-02 16:27 aicoder-0.3.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      945 b- defN 23-Jul-02 16:27 aicoder-0.3.6.dist-info/RECORD
-12 files, 65888 bytes uncompressed, 19968 bytes compressed:  69.7%
+-rw-r--r--  2.0 unx    14393 b- defN 23-Jul-02 16:42 aicoder/main.py
+-rw-r--r--  2.0 unx    18809 b- defN 23-Jul-02 16:43 aicoder-0.3.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx      473 b- defN 23-Jul-02 16:43 aicoder-0.3.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-02 16:43 aicoder-0.3.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       46 b- defN 23-Jul-02 16:43 aicoder-0.3.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-02 16:43 aicoder-0.3.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      945 b- defN 23-Jul-02 16:43 aicoder-0.3.7.dist-info/RECORD
+12 files, 66246 bytes uncompressed, 20038 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: aicoder/__init__.py
 Comment: 
 
 Filename: aicoder/main.py
 Comment: 
 
-Filename: aicoder-0.3.6.dist-info/LICENSE
+Filename: aicoder-0.3.7.dist-info/LICENSE
 Comment: 
 
-Filename: aicoder-0.3.6.dist-info/METADATA
+Filename: aicoder-0.3.7.dist-info/METADATA
 Comment: 
 
-Filename: aicoder-0.3.6.dist-info/WHEEL
+Filename: aicoder-0.3.7.dist-info/WHEEL
 Comment: 
 
-Filename: aicoder-0.3.6.dist-info/entry_points.txt
+Filename: aicoder-0.3.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: aicoder-0.3.6.dist-info/top_level.txt
+Filename: aicoder-0.3.7.dist-info/top_level.txt
 Comment: 
 
-Filename: aicoder-0.3.6.dist-info/RECORD
+Filename: aicoder-0.3.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aicoder/main.py

```diff
@@ -31,56 +31,56 @@
 
 def full_generator(prompt: str, api_key: str, model: str="gpt-4"):
     if os.path.isdir("generated"):
         os.system("rm -rf generated")
     aicoderfull = AICoderFull(prompt, api_key, "", model)
     aicoderfull.generate_program()
 
-def file_generator(prompt: str, api_key: str, github_token: str, model: str, template_files: list, orig_branch: str, new_branch: str, repo_name: str):
+def file_generator(prompt: str, api_key: str, github_token: str, model: str, template_files: list, final_file_path: str, orig_branch: str, to_branch: str, repo_name: str):
     aicoderpartial = AICoderPartial(prompt, api_key, github_token, model)
-    aicoderpartial.gen_file_from_templates(template_files, prompt, orig_branch, new_branch, repo_name)
+    aicoderpartial.gen_file_from_templates(template_files, final_file_path, prompt, orig_branch, to_branch, repo_name)
 
-def enhancer(prompt: str, api_key: str, github_token: str, model: str, file_paths: list, orig_branch: str, new_branch: str, repo_name: str):
+def enhancer(prompt: str, api_key: str, github_token: str, model: str, file_paths: list, orig_branch: str, to_branch: str, repo_name: str):
     aicoderpartial = AICoderPartial(prompt, api_key, github_token, model)
     for file_path in file_paths:
-        aicoderpartial.modify_file(file_path, prompt, orig_branch, new_branch, repo_name)
+        aicoderpartial.modify_file(file_path, prompt, orig_branch, to_branch, repo_name)
 
-def add_comments(prompt: str, api_key: str, github_token: str, model: str, file_paths: list, orig_branch: str, new_branch: str, repo_name: str):
+def add_comments(prompt: str, api_key: str, github_token: str, model: str, file_paths: list, orig_branch: str, to_branch: str, repo_name: str):
     final_prompt = "Given some code, add useful comments to it inside the code to easily understand what it does."
     if prompt:
         final_prompt = "\n" + prompt
     aicoderpartial = AICoderPartial(final_prompt, api_key, github_token, model)
     for file_path in file_paths:
-        aicoderpartial.modify_file(file_path, final_prompt, orig_branch, new_branch, repo_name)
+        aicoderpartial.modify_file(file_path, final_prompt, orig_branch, to_branch, repo_name)
 
-def check_security(prompt: str, api_key: str, github_token: str, model: str, file_paths: list, orig_branch: str, new_branch: str, repo_name: str):
+def check_security(prompt: str, api_key: str, github_token: str, model: str, file_paths: list, orig_branch: str, to_branch: str, repo_name: str):
     final_prompt = "Given some code, search for security vulnerabilities and potential backdoors on it and if any, create a new code fixing it (if possible). Return only the fixed code with the comments. If you changed anything, add at the end of the code comments explaining the changes."
     if prompt:
         final_prompt = "\n" + prompt
     aicoderpartial = AICoderPartial(final_prompt, api_key, github_token, model)
     for file_path in file_paths:
-        aicoderpartial.modify_file(file_path, final_prompt, orig_branch, new_branch, repo_name)
+        aicoderpartial.modify_file(file_path, final_prompt, orig_branch, to_branch, repo_name)
 
-def optimize_file(prompt: str, api_key: str, github_token: str, model: str, file_paths: list, orig_branch: str, new_branch: str, repo_name: str):
+def optimize_file(prompt: str, api_key: str, github_token: str, model: str, file_paths: list, orig_branch: str, to_branch: str, repo_name: str):
     final_prompt = "Given some code, optimize it without loosing functionality. Return a code that keeping the same functionality and respecting the class and function names, it's more clean and beautiful, simple, don't have duplice code, don't have code smells and is more efficient if possible. "
     final_prompt += "Don't remove comments, just improve them if possible. If you cannot improve the code just return the same code. If you changed anything, add at the end of the code comments explaining the changes. "
     final_prompt += "Be careful with chunks of code that looks similar but aren't exactly the same, even if part of the code can be improved the different functionalities must be keeped."
     if prompt:
         final_prompt = "\n" + prompt
     aicoderpartial = AICoderPartial(final_prompt, api_key, github_token, model)
     for file_path in file_paths:
-        aicoderpartial.modify_file(file_path, final_prompt, orig_branch, new_branch, repo_name)
+        aicoderpartial.modify_file(file_path, final_prompt, orig_branch, to_branch, repo_name)
 
-def fix_bugs(prompt: str, api_key: str, github_token: str, model: str, file_paths: list, orig_branch: str, new_branch: str, repo_name: str):
+def fix_bugs(prompt: str, api_key: str, github_token: str, model: str, file_paths: list, orig_branch: str, to_branch: str, repo_name: str):
     final_prompt = "Given some code and keeping the same functionality fix all the bugs in it. Also, don't remove comments, just improve them if possible."
     if prompt:
         final_prompt = "\n" + prompt
     aicoderpartial = AICoderPartial(final_prompt, api_key, github_token, model)
     for file_path in file_paths:
-        aicoderpartial.modify_file(file_path, final_prompt, orig_branch, new_branch, repo_name)
+        aicoderpartial.modify_file(file_path, final_prompt, orig_branch, to_branch, repo_name)
 
 def add_common_arguments(parser):
     parser.add_argument('--api-key', default=None, type=str, help='Input API key')
     parser.add_argument('--model', default="gpt-4", type=str, help='Model to use')
     parser.add_argument('--prompt', default=None, type=str, help='Input prompt. It can be string, a file path or a url.')
 
 def get_git_org_repo_name():
@@ -103,14 +103,15 @@
         add_common_arguments(subparser)
 
     file_generator_parser.add_argument('--template-files', type=str, help='Comma separated list of template files')
     file_generator_parser.add_argument('--github-token', default=None, type=str, help='Github token')
     file_generator_parser.add_argument('--orig-branch', default=None, type=str, help='Branch to upload the changes.')
     file_generator_parser.add_argument('--to-branch', default=None, type=str, help='Branch to send the PR to.')
     file_generator_parser.add_argument('--repo-name', default=None, type=str, help='Indicate the name of the repo: org_name/repo_name')
+    file_generator_parser.add_argument('--file-path', default=None, type=str, help='File path to generate')
     
     file_enhancer_parser.add_argument('--paths', type=str, help='Comma separated list of file paths to enhance')
     file_enhancer_parser.add_argument('--github-token', default=None, type=str, help='Github token')
     file_enhancer_parser.add_argument('--orig-branch', default=None, type=str, help='Branch to upload the changes.')
     file_enhancer_parser.add_argument('--to-branch', default=None, type=str, help='Branch to send the PR to.')
     file_enhancer_parser.add_argument('--repo-name', default=None, type=str, help='Indicate the name of the repo: org_name/repo_name')
     
@@ -147,14 +148,15 @@
         github_token = os.environ.get("GITHUB_TOKEN") or args.github_token
         orig_branch = os.environ.get("ORIGIN_BRANCH") or args.orig_branch
         to_branch = os.environ.get("TO_BRANCH") or args.to_branch
         repo_name = os.environ.get("GITHUB_REPOSITORY") or args.repo_name or get_git_org_repo_name()
 
         if args.mode == "file-generator":
             template_files = list(os.environ.get("TEMPLATE_FILES").split(",")) or args.template_files.split(',')
+            final_file_path = list(os.environ.get("FINAL_FILE_PATH").split(",")) or args.file_path
                 
         elif args.mode in ["file-enhancer", "file-comments", "file-security", "file-optimizer", "file-bugfixer"]:
             check_paths = os.environ.get("CHECK_PATHS").split(',') or args.paths.split(',')
     
     if not prompt and not args.mode in ["file-comments", "file-security", "file-optimizer"]:
         logger.error("Error: Missing prompt.")
         parser.print_help()
@@ -194,15 +196,15 @@
         exit(1)
     
     if github_token and not repo_name:
         logger.error("Error: No repo name. PRs cannot be created automatically. Stopping.")
         exit(1)
     
     elif args.mode == 'file-generator':
-        file_generator(prompt, api_key, github_token, model, template_files, orig_branch, to_branch, repo_name)
+        file_generator(prompt, api_key, github_token, model, template_files, final_file_path, orig_branch, to_branch, repo_name)
         exit(0)
     
     elif args.mode in ['file-enhancer', 'file-comments', 'file-security', 'file-optimizer', 'file-bugfixer']:
         if args.mode == 'file-enhancer':
             f = enhancer
         elif args.mode == 'file-comments':
             f = add_comments
@@ -221,11 +223,14 @@
             elif os.path.isdir(file_path):
                 logger.info(f"Given path {file_path} is a folder.")
                 with ThreadPoolExecutor(max_workers=3) as executor:
                     for root, dirs, files in os.walk(file_path):
                         for file in files:
                             logger.info(f"Checking file: {file_path}")
                             executor.submit(f, prompt, api_key, github_token, model, os.path.join(root, file), orig_branch, to_branch, repo_name)
+            else:
+                logger.error(f"Given path {file_path} is neither a file nor a folder.")
+
         exit(0)
 
 if __name__ == "__main__":
     main()
```

## Comparing `aicoder-0.3.6.dist-info/LICENSE` & `aicoder-0.3.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `aicoder-0.3.6.dist-info/RECORD` & `aicoder-0.3.7.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 aicoder/AICoder.py,sha256=83hZ7Sdvyd0wtiJE5kPLSaAt7wIC6BlN8MVYaaehwiw,12662
 aicoder/AICoderFull.py,sha256=VjCIDZZMCVoCsnn1XVVyizhplfxDLlS-V30iW3r0TCk,8087
 aicoder/AICoderPartial.py,sha256=nClKfFoVbRZpoM2rLIeQoOtllSD8dMAHNuiFyLj-kcA,7160
 aicoder/AICoderPrompts.py,sha256=EyVLCIKkUDACV0swEHWVfRPNU_cQwYbLIIQ8nFI2VJY,3571
 aicoder/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-aicoder/main.py,sha256=GmzGkU_bmxRhm-NfqnLGnbRd0ELbn-GHd92yHRKyMzg,14035
-aicoder-0.3.6.dist-info/LICENSE,sha256=nGKG3YDYTyar3KKwoaLPInTfnNQtuvh4aMwTADTd0L8,18809
-aicoder-0.3.6.dist-info/METADATA,sha256=RHn7LZFZ7HaZxtfv7Xt0iU4MmjWSicc73riKO8NkZUo,473
-aicoder-0.3.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-aicoder-0.3.6.dist-info/entry_points.txt,sha256=m__okhQaM4kZ8CCfSA5VGUyQ0gf7TIGax6DhXdTnAeA,46
-aicoder-0.3.6.dist-info/top_level.txt,sha256=B8Pf-hhM5icZE_7vMCXD5mXWG0MAqt5ImotI1aNXdWQ,8
-aicoder-0.3.6.dist-info/RECORD,,
+aicoder/main.py,sha256=RrnB-5DK_7mSlFVpfW64JKTiSHGanaRrlh_i7dJWWIc,14393
+aicoder-0.3.7.dist-info/LICENSE,sha256=nGKG3YDYTyar3KKwoaLPInTfnNQtuvh4aMwTADTd0L8,18809
+aicoder-0.3.7.dist-info/METADATA,sha256=1dlh0yypUK_uiPcfQSsn0NlskUzG4U18Pwvv0k9-Bq0,473
+aicoder-0.3.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+aicoder-0.3.7.dist-info/entry_points.txt,sha256=m__okhQaM4kZ8CCfSA5VGUyQ0gf7TIGax6DhXdTnAeA,46
+aicoder-0.3.7.dist-info/top_level.txt,sha256=B8Pf-hhM5icZE_7vMCXD5mXWG0MAqt5ImotI1aNXdWQ,8
+aicoder-0.3.7.dist-info/RECORD,,
```

