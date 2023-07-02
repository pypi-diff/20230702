# Comparing `tmp/aicoder-0.3.5-py3-none-any.whl.zip` & `tmp/aicoder-0.3.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 21779 bytes, number of entries: 12
--rw-r--r--  2.0 unx    12669 b- defN 23-Jun-30 12:05 aicoder/AICoder.py
--rw-r--r--  2.0 unx     8088 b- defN 23-Jun-30 12:27 aicoder/AICoderFull.py
--rw-r--r--  2.0 unx     7162 b- defN 23-Jul-02 16:10 aicoder/AICoderPartial.py
+Zip file size: 21548 bytes, number of entries: 12
+-rw-r--r--  2.0 unx    12662 b- defN 23-Jul-02 16:18 aicoder/AICoder.py
+-rw-r--r--  2.0 unx     8087 b- defN 23-Jul-02 16:18 aicoder/AICoderFull.py
+-rw-r--r--  2.0 unx     7160 b- defN 23-Jul-02 16:18 aicoder/AICoderPartial.py
 -rw-r--r--  2.0 unx     3571 b- defN 23-Jun-30 12:29 aicoder/AICoderPrompts.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-29 11:14 aicoder/__init__.py
--rw-r--r--  2.0 unx    14606 b- defN 23-Jul-02 14:09 aicoder/main.py
--rw-r--r--  2.0 unx    18809 b- defN 23-Jul-02 16:10 aicoder-0.3.5.dist-info/LICENSE
--rw-r--r--  2.0 unx      473 b- defN 23-Jul-02 16:10 aicoder-0.3.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-02 16:10 aicoder-0.3.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       46 b- defN 23-Jul-02 16:10 aicoder-0.3.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-02 16:10 aicoder-0.3.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      945 b- defN 23-Jul-02 16:10 aicoder-0.3.5.dist-info/RECORD
-12 files, 66469 bytes uncompressed, 20199 bytes compressed:  69.6%
+-rw-r--r--  2.0 unx    14035 b- defN 23-Jul-02 16:25 aicoder/main.py
+-rw-r--r--  2.0 unx    18809 b- defN 23-Jul-02 16:27 aicoder-0.3.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx      473 b- defN 23-Jul-02 16:27 aicoder-0.3.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-02 16:27 aicoder-0.3.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       46 b- defN 23-Jul-02 16:27 aicoder-0.3.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-02 16:27 aicoder-0.3.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      945 b- defN 23-Jul-02 16:27 aicoder-0.3.6.dist-info/RECORD
+12 files, 65888 bytes uncompressed, 19968 bytes compressed:  69.7%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: aicoder/__init__.py
 Comment: 
 
 Filename: aicoder/main.py
 Comment: 
 
-Filename: aicoder-0.3.5.dist-info/LICENSE
+Filename: aicoder-0.3.6.dist-info/LICENSE
 Comment: 
 
-Filename: aicoder-0.3.5.dist-info/METADATA
+Filename: aicoder-0.3.6.dist-info/METADATA
 Comment: 
 
-Filename: aicoder-0.3.5.dist-info/WHEEL
+Filename: aicoder-0.3.6.dist-info/WHEEL
 Comment: 
 
-Filename: aicoder-0.3.5.dist-info/entry_points.txt
+Filename: aicoder-0.3.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: aicoder-0.3.5.dist-info/top_level.txt
+Filename: aicoder-0.3.6.dist-info/top_level.txt
 Comment: 
 
-Filename: aicoder-0.3.5.dist-info/RECORD
+Filename: aicoder-0.3.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aicoder/AICoder.py

```diff
@@ -58,15 +58,15 @@
     def remove_fences(self, text: str) -> str:
         """Function that removes code fences from the response"""
 
         if len(text.split("```")) == 3:
             text = "\n".join(text.split("```")[1].split("\n")[1:])
         
         elif len(text.split("```")) > 3:
-            logger.debug(f"The response has more than 3 code fences: " + text)
+            logger.info(f"The response has more than 3 code fences: " + text)
         
         return text
 
     def fix_json(self, orig_text: str, orig_response: str, json_error: str) -> str:
         """Function that asks to fix a given json"""
 
         all_msg = f"{orig_text}\n\n You already gave this reponse:\n{orig_response}\n\nWhich resulted in this error:\n{json_error}\n\nPlease fix it and respond with a valid json."
@@ -167,15 +167,15 @@
 
         msg_imports = f"These are all the imports files are using: {json.dumps(ALL_IMPORTS, indent=4)}\n\n"
         compilation_command = self.contact(COMPILATION_COMMAND + "\n\n" + msg_imports)
         compilation_command = self.remove_fences(compilation_command)
         compilation_command = json.loads(compilation_command)["command"]
 
         if not compilation_command:
-            logger.debug("The program doesn't need to be compiled")
+            logger.info("The program doesn't need to be compiled")
             return
 
         print("This is the compilation command: ", compilation_command)
         print("Is this ok? If not, you will be asked for a command (Y/n)")
         user_input = input()
         if user_input.lower() in ["no", "n"]:
             print("Ok, do you want to indicate a compilation command? (Y/n)")
@@ -198,23 +198,23 @@
             self.fix_errors_per_file_auto(compilation_command)
 
 
     def fix_errors_per_file_auto(self, command_to_run):
         """Function that ask the model to fix the errors per file after running a command"""
 
         # execute getting the stdout and stderr
-        logger.debug(f"Running '{command_to_run}' ...")
+        logger.info(f"Running '{command_to_run}' ...")
         process = subprocess.Popen(command_to_run, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
         stdout, stderr = process.communicate()
         stdout = stdout.decode("utf-8")
         stderr = stderr.decode("utf-8")
 
         # Print the results
-        logger.debug(f"[+] stdout: {stdout}\n")
-        logger.debug("====================================")
+        logger.info(f"[+] stdout: {stdout}\n")
+        logger.info("====================================")
         print()
         logger.warning(f"[+] stderr: {stderr}\n")
 
         if not stderr:
             logger.info("No errors found, the program should work now!")
             return
 
@@ -229,21 +229,21 @@
 
         # Remove empty errors
         for err in errors:
             if not err["errors_text"]:
                 errors.remove(err)
         
         # Errors found
-        logger.debug("These are the errors found:")
+        logger.info("These are the errors found:")
         print(json.dumps(errors, indent=4))
 
         for err in errors:
             # Get the file path
             file_path = err["file_path"]
-            logger.debug(f"Fixing errors in {file_path} ...")
+            logger.info(f"Fixing errors in {file_path} ...")
 
             # Ask user if he wants to fix the errors
             print("Do you want to fix that errors? (Y/n)")
             user_input = input()
             if user_input.lower() in ["no", "n"]:
                 logger.info("Ok, not fixing that file")
                 continue
```

## aicoder/AICoderFull.py

```diff
@@ -94,15 +94,15 @@
         dependencies_content = ""
         cont = 0
         all_exists = True
         while cont < 50:
             for dep in file["dependencies"]:
                 if not os.path.exists(dep):
                     all_exists = False
-                    logger.debug(f"Sleeping from {file['path']} the dependency: {dep}")
+                    logger.info(f"Sleeping from {file['path']} the dependency: {dep}")
                     sleep(10)
                     if cont > 48:
                         logger.warning(f"The dependency {dep} of {file['path']} doesn't exist.")
                     cont += 1
                     continue
             if all_exists:
                 break
```

## aicoder/AICoderPartial.py

```diff
@@ -141,19 +141,19 @@
         push_result = subprocess.run(["git", "push", "--set-upstream", new_origin_url, orig_branch], text=True, capture_output=True)
         if push_result.returncode != 0:
             print(f"Failed to push the changes to the origin {new_origin_url}: ", push_result.stderr)
             return
 
         # Create a pull request
         sleep(1)
-        logger.debug(f"Creating a pull request to repo {repo_name}, from branch {orig_branch} to branch {to_branch}...")
+        logger.info(f"Creating a pull request to repo {repo_name}, from branch {orig_branch} to branch {to_branch}...")
         pr = repo.create_pull(
             title=commit_message,
             body=commit_body,
             head=orig_branch,
             base=to_branch
         )
 
-        logger.debug(f"Pull request created: {pr.html_url}")
+        logger.info(f"Pull request created: {pr.html_url}")
 
         # Set the origin URL back to the original URL
         push_result = subprocess.run(["git", "push", "--set-upstream", origin_url, orig_branch], text=True, capture_output=True)
```

## aicoder/main.py

```diff
@@ -7,198 +7,181 @@
 import logging
 import colorlog
 import subprocess
 from concurrent.futures import ThreadPoolExecutor
 from aicoder.AICoderFull import AICoderFull
 from aicoder.AICoderPartial import AICoderPartial
 
-# Logger setup
 handler = colorlog.StreamHandler()
 handler.setFormatter(colorlog.ColoredFormatter('%(log_color)s%(levelname)s:%(message)s'))
 logger = colorlog.getLogger('file_generator')
 if not logger.hasHandlers():
     logger.addHandler(handler)
     logger.setLevel(logging.INFO)
 
-# Function to check if the current directory is a git repo
 def is_git_repo():
     try:
         subprocess.run(["git", "rev-parse", "--is-inside-work-tree"], check=True, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
         return True
     except subprocess.CalledProcessError:
         return False
 
-# Function to generate a random string
 def get_random_string(length):
     letters = string.ascii_letters
     return ''.join(random.choice(letters) for _ in range(length))
 
-# Function to generate a full program
 def full_generator(prompt: str, api_key: str, model: str="gpt-4"):
     if os.path.isdir("generated"):
         os.system("rm -rf generated")
     aicoderfull = AICoderFull(prompt, api_key, "", model)
     aicoderfull.generate_program()
 
-# Function to generate a file from templates
 def file_generator(prompt: str, api_key: str, github_token: str, model: str, template_files: list, orig_branch: str, new_branch: str, repo_name: str):
     aicoderpartial = AICoderPartial(prompt, api_key, github_token, model)
     aicoderpartial.gen_file_from_templates(template_files, prompt, orig_branch, new_branch, repo_name)
 
-# Function to enhance a file
-def enhancer(prompt: str, api_key: str, github_token: str, model: str, file_path: str, orig_branch: str, new_branch: str, repo_name: str):
+def enhancer(prompt: str, api_key: str, github_token: str, model: str, file_paths: list, orig_branch: str, new_branch: str, repo_name: str):
     aicoderpartial = AICoderPartial(prompt, api_key, github_token, model)
-    aicoderpartial.modify_file(file_path, prompt, orig_branch, new_branch, repo_name)
+    for file_path in file_paths:
+        aicoderpartial.modify_file(file_path, prompt, orig_branch, new_branch, repo_name)
 
-# Function to add comments to a file
-def add_comments(prompt: str, api_key: str, github_token: str, model: str, file_path: str, orig_branch: str, new_branch: str, repo_name: str):
+def add_comments(prompt: str, api_key: str, github_token: str, model: str, file_paths: list, orig_branch: str, new_branch: str, repo_name: str):
     final_prompt = "Given some code, add useful comments to it inside the code to easily understand what it does."
     if prompt:
         final_prompt = "\n" + prompt
     aicoderpartial = AICoderPartial(final_prompt, api_key, github_token, model)
-    aicoderpartial.modify_file(file_path, final_prompt, orig_branch, new_branch, repo_name)
+    for file_path in file_paths:
+        aicoderpartial.modify_file(file_path, final_prompt, orig_branch, new_branch, repo_name)
 
-# Function to check for security vulnerabilities in a file
-def check_security(prompt: str, api_key: str, github_token: str, model: str, file_path: str, orig_branch: str, new_branch: str, repo_name: str):
+def check_security(prompt: str, api_key: str, github_token: str, model: str, file_paths: list, orig_branch: str, new_branch: str, repo_name: str):
     final_prompt = "Given some code, search for security vulnerabilities and potential backdoors on it and if any, create a new code fixing it (if possible). Return only the fixed code with the comments. If you changed anything, add at the end of the code comments explaining the changes."
     if prompt:
         final_prompt = "\n" + prompt
     aicoderpartial = AICoderPartial(final_prompt, api_key, github_token, model)
-    aicoderpartial.modify_file(file_path, final_prompt, orig_branch, new_branch, repo_name)
+    for file_path in file_paths:
+        aicoderpartial.modify_file(file_path, final_prompt, orig_branch, new_branch, repo_name)
 
-# Function to optimize a file
-def optimize_file(prompt: str, api_key: str, github_token: str, model: str, file_path: str, orig_branch: str, new_branch: str, repo_name: str):
+def optimize_file(prompt: str, api_key: str, github_token: str, model: str, file_paths: list, orig_branch: str, new_branch: str, repo_name: str):
     final_prompt = "Given some code, optimize it without loosing functionality. Return a code that keeping the same functionality and respecting the class and function names, it's more clean and beautiful, simple, don't have duplice code, don't have code smells and is more efficient if possible. "
     final_prompt += "Don't remove comments, just improve them if possible. If you cannot improve the code just return the same code. If you changed anything, add at the end of the code comments explaining the changes. "
     final_prompt += "Be careful with chunks of code that looks similar but aren't exactly the same, even if part of the code can be improved the different functionalities must be keeped."
     if prompt:
         final_prompt = "\n" + prompt
     aicoderpartial = AICoderPartial(final_prompt, api_key, github_token, model)
-    aicoderpartial.modify_file(file_path, final_prompt, orig_branch, new_branch, repo_name)
+    for file_path in file_paths:
+        aicoderpartial.modify_file(file_path, final_prompt, orig_branch, new_branch, repo_name)
 
-# Function to fix bugs in a file
-def fix_bugs(prompt: str, api_key: str, github_token: str, model: str, file_path: str, orig_branch: str, new_branch: str, repo_name: str):
+def fix_bugs(prompt: str, api_key: str, github_token: str, model: str, file_paths: list, orig_branch: str, new_branch: str, repo_name: str):
     final_prompt = "Given some code and keeping the same functionality fix all the bugs in it. Also, don't remove comments, just improve them if possible."
     if prompt:
         final_prompt = "\n" + prompt
     aicoderpartial = AICoderPartial(final_prompt, api_key, github_token, model)
-    aicoderpartial.modify_file(file_path, final_prompt, orig_branch, new_branch, repo_name)
+    for file_path in file_paths:
+        aicoderpartial.modify_file(file_path, final_prompt, orig_branch, new_branch, repo_name)
 
-# Function to add common arguments to a parser
 def add_common_arguments(parser):
     parser.add_argument('--api-key', default=None, type=str, help='Input API key')
     parser.add_argument('--model', default="gpt-4", type=str, help='Model to use')
     parser.add_argument('--prompt', default=None, type=str, help='Input prompt. It can be string, a file path or a url.')
 
-# Function to get repo name
 def get_git_org_repo_name():
     command = ['bash', '-c', 'git config --get remote.origin.url | sed -nE \'s/.*github.com[:\/]([^\/]*)\/(.*)\.git/\\1\\/\\2/p\'']
     return subprocess.check_output(command).strip().decode()
 
-# Main function
 def main():
     parser = argparse.ArgumentParser()
-    subparsers = parser.add_subparsers(dest="mode")  # Create subparsers
+    subparsers = parser.add_subparsers(dest="mode")  
 
-    # Create subparsers
     full_generator_parser = subparsers.add_parser('full-generator', help='Generate a full program from the prompt.')
     file_generator_parser = subparsers.add_parser('file-generator', help='Generate a file based on others as templates.')
     file_enhancer_parser = subparsers.add_parser('file-enhancer', help='Enhance a file based on the given prompt.')
     file_commentor_parser = subparsers.add_parser('file-comments', help='Ask to add comments to a file.')
     file_security_parser = subparsers.add_parser('file-security', help='Ask to search security vulnerabilities and backdoors in a file.')
     file_optimizer_parser = subparsers.add_parser('file-optimizer', help='Ask to optimize a file in terms of clean code and efficiency.')
     file_bug_fixer_parser = subparsers.add_parser('file-bugfixer', help='Ask to fix bugs in a file.')
 
-    # Add common arguments to each subparser
     for subparser in [full_generator_parser, file_generator_parser, file_enhancer_parser, file_commentor_parser, file_security_parser, file_optimizer_parser, file_bug_fixer_parser]:
         add_common_arguments(subparser)
 
-    # Add specific arguments to each subparser    
-    file_generator_parser.add_argument('--template-files', nargs='+', help='List of template files')
+    file_generator_parser.add_argument('--template-files', type=str, help='Comma separated list of template files')
     file_generator_parser.add_argument('--github-token', default=None, type=str, help='Github token')
     file_generator_parser.add_argument('--orig-branch', default=None, type=str, help='Branch to upload the changes.')
     file_generator_parser.add_argument('--to-branch', default=None, type=str, help='Branch to send the PR to.')
     file_generator_parser.add_argument('--repo-name', default=None, type=str, help='Indicate the name of the repo: org_name/repo_name')
     
-    file_enhancer_parser.add_argument('--path', type=str, help='Path to file to enhance')
+    file_enhancer_parser.add_argument('--paths', type=str, help='Comma separated list of file paths to enhance')
     file_enhancer_parser.add_argument('--github-token', default=None, type=str, help='Github token')
     file_enhancer_parser.add_argument('--orig-branch', default=None, type=str, help='Branch to upload the changes.')
     file_enhancer_parser.add_argument('--to-branch', default=None, type=str, help='Branch to send the PR to.')
     file_enhancer_parser.add_argument('--repo-name', default=None, type=str, help='Indicate the name of the repo: org_name/repo_name')
     
-    file_commentor_parser.add_argument('--path', type=str, help='Path to file or folder to add comments')
+    file_commentor_parser.add_argument('--paths', type=str, help='Comma separated list of file paths to add comments')
     file_commentor_parser.add_argument('--github-token', default=None, type=str, help='Github token')
     file_commentor_parser.add_argument('--orig-branch', default=None, type=str, help='Branch to upload the changes.')
     file_commentor_parser.add_argument('--to-branch', default=None, type=str, help='Branch to send the PR to.')
     file_commentor_parser.add_argument('--repo-name', default=None, type=str, help='Indicate the name of the repo: org_name/repo_name')
     
-    file_security_parser.add_argument('--path', type=str, help='Path to file or folder to search vulnerabilities')
+    file_security_parser.add_argument('--paths', type=str, help='Comma separated list of file paths to search vulnerabilities')
     file_security_parser.add_argument('--github-token', default=None, type=str, help='Github token')
     file_security_parser.add_argument('--orig-branch', default=None, type=str, help='Branch to upload the changes.')
     file_security_parser.add_argument('--to-branch', default=None, type=str, help='Branch to send the PR to.')
     file_security_parser.add_argument('--repo-name', default=None, type=str, help='Indicate the name of the repo: org_name/repo_name')
     
-    file_optimizer_parser.add_argument('--path', type=str, help='Path to file or folder to optimize')
+    file_optimizer_parser.add_argument('--paths', type=str, help='Comma separated list of file paths to optimize')
     file_optimizer_parser.add_argument('--github-token', default=None, type=str, help='Github token')
     file_optimizer_parser.add_argument('--orig-branch', default=None, type=str, help='Branch to upload the changes.')
     file_optimizer_parser.add_argument('--to-branch', default=None, type=str, help='Branch to send the PR to.')
     file_optimizer_parser.add_argument('--repo-name', default=None, type=str, help='Indicate the name of the repo: org_name/repo_name')
 
-    file_bug_fixer_parser.add_argument('--path', type=str, help='Path to file or folder to fix bugs')
+    file_bug_fixer_parser.add_argument('--paths', type=str, help='Comma separated list of file paths to fix bugs')
     file_bug_fixer_parser.add_argument('--github-token', default=None, type=str, help='Github token')
     file_bug_fixer_parser.add_argument('--orig-branch', default=None, type=str, help='Branch to upload the changes.')
     file_bug_fixer_parser.add_argument('--to-branch', default=None, type=str, help='Branch to send the PR to.')
     file_bug_fixer_parser.add_argument('--repo-name', default=None, type=str, help='Indicate the name of the repo: org_name/repo_name')
     
-    # Parse arguments
     args = parser.parse_args()
     prompt = os.environ.get("INPUT_PROMPT") or (args.prompt if hasattr(args,"prompt") else None)
     api_key = os.environ.get("INPUT_OPENAI_API_KEY") or (args.api_key if hasattr(args,"api_key") else None)
     model = os.environ.get("INPUT_MODEL") or (args.model if hasattr(args,"model") else None)
 
     if args.mode in ["file-generator", "file-enhancer", "file-comments", "file-security", "file-optimizer", "file-bugfixer"]:
         github_token = os.environ.get("GITHUB_TOKEN") or args.github_token
         orig_branch = os.environ.get("ORIGIN_BRANCH") or args.orig_branch
         to_branch = os.environ.get("TO_BRANCH") or args.to_branch
         repo_name = os.environ.get("GITHUB_REPOSITORY") or args.repo_name or get_git_org_repo_name()
 
         if args.mode == "file-generator":
-            template_files = list(os.environ.get("TEMPLATE_FILES").split(",")) or args.template_files
+            template_files = list(os.environ.get("TEMPLATE_FILES").split(",")) or args.template_files.split(',')
                 
         elif args.mode in ["file-enhancer", "file-comments", "file-security", "file-optimizer", "file-bugfixer"]:
-            check_path = os.environ.get("CHECK_PATH") or args.path
+            check_paths = os.environ.get("CHECK_PATHS").split(',') or args.paths.split(',')
     
     if not prompt and not args.mode in ["file-comments", "file-security", "file-optimizer"]:
         logger.error("Error: Missing prompt.")
         parser.print_help()
         sys.exit(1)
     
     if not api_key:
         logger.error("Error: Missing API key.")
         parser.print_help()
         sys.exit(1)
     
-    # If prompt is file path, read it
     if prompt and os.path.isfile(prompt):
-        logger.debug(f"Prompt read from {prompt}")
+        logger.info(f"Prompt read from {prompt}")
         with open(prompt, "r") as f:
             prompt = f.read()
     
-    # If prompt is url, download it
     elif prompt and prompt.startswith("http"):
-        logger.debug(f"Prompt downloaded from {prompt}")
+        logger.info(f"Prompt downloaded from {prompt}")
         prompt = requests.get(prompt).text
     
-    # If full generator mode
     if args.mode == 'full-generator':
         full_generator(prompt, api_key, model)
         exit(0)
     
-    ### Checks for single file modifiers
-    
     if not github_token:
         logger.warning("No Github token. PRs cannot be created automatically.")
     
     if github_token and not is_git_repo():
         logger.error("Error: Current directory isn't a git repository. Stopping.")
         exit(1)
     
@@ -210,43 +193,39 @@
         logger.error("Error: No to branch. PRs cannot be created automatically. Stopping.")
         exit(1)
     
     if github_token and not repo_name:
         logger.error("Error: No repo name. PRs cannot be created automatically. Stopping.")
         exit(1)
     
-    # If file enhancer mode
     elif args.mode == 'file-generator':
         file_generator(prompt, api_key, github_token, model, template_files, orig_branch, to_branch, repo_name)
         exit(0)
     
-    # If file commentor mode
     elif args.mode in ['file-enhancer', 'file-comments', 'file-security', 'file-optimizer', 'file-bugfixer']:
-        # pompt is optional for all these modes except file-enhancer
         if args.mode == 'file-enhancer':
             f = enhancer
         elif args.mode == 'file-comments':
             f = add_comments
         elif args.mode == 'file-security':
             f = check_security
         elif args.mode == 'file-optimizer':
             f = optimize_file
         elif args.mode == 'file-bugfixer':
             f = fix_bugs
         
-        # Check if path is file or folder
-        if os.path.isfile(check_path):
-            logger.debug(f"Given path {check_path} is a file.")
-            f(prompt, api_key, github_token, model, check_path, orig_branch, to_branch, repo_name)
+        for file_path in check_paths:
+            if os.path.isfile(file_path):
+                logger.info(f"Given path {file_path} is a file.")
+                f(prompt, api_key, github_token, model, file_path, orig_branch, to_branch, repo_name)
         
-        elif os.path.isdir(check_path):
-            logger.debug(f"Given path {check_path} is a folder.")
-            with ThreadPoolExecutor(max_workers=3) as executor:
-                for root, dirs, files in os.walk(check_path):
-                    for file in files:
-                        logger.debug(f"Checking file: {check_path}")
-                        executor.submit(f, prompt, api_key, github_token, model, os.path.join(root, file), orig_branch, to_branch, repo_name)
+            elif os.path.isdir(file_path):
+                logger.info(f"Given path {file_path} is a folder.")
+                with ThreadPoolExecutor(max_workers=3) as executor:
+                    for root, dirs, files in os.walk(file_path):
+                        for file in files:
+                            logger.info(f"Checking file: {file_path}")
+                            executor.submit(f, prompt, api_key, github_token, model, os.path.join(root, file), orig_branch, to_branch, repo_name)
         exit(0)
 
-    
 if __name__ == "__main__":
     main()
```

## Comparing `aicoder-0.3.5.dist-info/LICENSE` & `aicoder-0.3.6.dist-info/LICENSE`

 * *Files identical despite different names*

