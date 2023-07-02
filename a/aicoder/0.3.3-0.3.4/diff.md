# Comparing `tmp/aicoder-0.3.3-py3-none-any.whl.zip` & `tmp/aicoder-0.3.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 21596 bytes, number of entries: 12
+Zip file size: 21769 bytes, number of entries: 12
 -rw-r--r--  2.0 unx    12669 b- defN 23-Jun-30 12:05 aicoder/AICoder.py
 -rw-r--r--  2.0 unx     8088 b- defN 23-Jun-30 12:27 aicoder/AICoderFull.py
--rw-r--r--  2.0 unx     6107 b- defN 23-Jul-02 15:40 aicoder/AICoderPartial.py
+-rw-r--r--  2.0 unx     6927 b- defN 23-Jul-02 16:08 aicoder/AICoderPartial.py
 -rw-r--r--  2.0 unx     3571 b- defN 23-Jun-30 12:29 aicoder/AICoderPrompts.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-29 11:14 aicoder/__init__.py
 -rw-r--r--  2.0 unx    14606 b- defN 23-Jul-02 14:09 aicoder/main.py
--rw-r--r--  2.0 unx    18809 b- defN 23-Jul-02 15:41 aicoder-0.3.3.dist-info/LICENSE
--rw-r--r--  2.0 unx      473 b- defN 23-Jul-02 15:41 aicoder-0.3.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-02 15:41 aicoder-0.3.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       46 b- defN 23-Jul-02 15:41 aicoder-0.3.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-02 15:41 aicoder-0.3.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      945 b- defN 23-Jul-02 15:41 aicoder-0.3.3.dist-info/RECORD
-12 files, 65414 bytes uncompressed, 20016 bytes compressed:  69.4%
+-rw-r--r--  2.0 unx    18809 b- defN 23-Jul-02 16:08 aicoder-0.3.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx      473 b- defN 23-Jul-02 16:08 aicoder-0.3.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-02 16:08 aicoder-0.3.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       46 b- defN 23-Jul-02 16:08 aicoder-0.3.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-02 16:08 aicoder-0.3.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      945 b- defN 23-Jul-02 16:08 aicoder-0.3.4.dist-info/RECORD
+12 files, 66234 bytes uncompressed, 20189 bytes compressed:  69.5%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: aicoder/__init__.py
 Comment: 
 
 Filename: aicoder/main.py
 Comment: 
 
-Filename: aicoder-0.3.3.dist-info/LICENSE
+Filename: aicoder-0.3.4.dist-info/LICENSE
 Comment: 
 
-Filename: aicoder-0.3.3.dist-info/METADATA
+Filename: aicoder-0.3.4.dist-info/METADATA
 Comment: 
 
-Filename: aicoder-0.3.3.dist-info/WHEEL
+Filename: aicoder-0.3.4.dist-info/WHEEL
 Comment: 
 
-Filename: aicoder-0.3.3.dist-info/entry_points.txt
+Filename: aicoder-0.3.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: aicoder-0.3.3.dist-info/top_level.txt
+Filename: aicoder-0.3.4.dist-info/top_level.txt
 Comment: 
 
-Filename: aicoder-0.3.3.dist-info/RECORD
+Filename: aicoder-0.3.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aicoder/AICoderPartial.py

```diff
@@ -83,26 +83,40 @@
             commit_body = f"AICoder created the file {final_file_path} based on the files {', '.join(template_file_paths)} according to this input:\n{prompt}"
             self.create_pull_request(commit_msg, commit_body, orig_branch, to_branch, repo_name)
 
 
     def change_branch(self, orig_branch: str):
         """Function that changes the branch"""
 
-        # Check if the branch exists
-        result = subprocess.run(["git", "rev-parse", "--verify", "--quiet", orig_branch], text=True, capture_output=True)
+        # Fetch the remote branches
+        subprocess.run(["git", "fetch"], check=True)
+
+        # Check if the branch exists locally
+        result = subprocess.run(["git", "show-ref", "--verify", "--quiet", f"refs/heads/{orig_branch}"])
 
-        # If the branch doesn't exist, create it
         if result.returncode != 0:
+            # The branch does not exist locally, so create it
             subprocess.run(["git", "checkout", "-b", orig_branch], check=True)
             logger.info(f"Branch {orig_branch} created")
-        else:  # If the branch exists, just check it out
+
+            # Check if the branch exists remotely
+            result = subprocess.run(["git", "ls-remote", "--exit-code", "--heads", "origin", orig_branch])
+            if result.returncode == 0:
+                # The branch exists remotely, so set up tracking and pull the latest changes
+                subprocess.run(["git", "branch", "--set-upstream-to", f"origin/{orig_branch}", orig_branch], check=True)
+                subprocess.run(["git", "config", "pull.rebase", "false"], check=True)
+                subprocess.run(["git", "pull", "--no-edit"], check=True)
+                logger.info(f"Downloaded the latest changes from branch {orig_branch}")
+        else:
+            # The branch exists locally, so check it out and pull the latest changes
             subprocess.run(["git", "checkout", orig_branch], check=True)
             subprocess.run(["git", "config", "pull.rebase", "false"], check=True)
-            subprocess.run(["git", "pull"], check=True)
-            logger.info(f"Branch {orig_branch} checked out")
+            subprocess.run(["git", "pull", "--no-edit"], check=True)
+            logger.info(f"Branch {orig_branch} checked out and updated")
+
 
 
     def create_pull_request(self, commit_message: str, commit_body: str, orig_branch: str, to_branch: str, repo_name: str):
         """Function that creates a pull request"""
 
         github = Github(self.github_token)
         repo = github.get_repo(repo_name)
```

## Comparing `aicoder-0.3.3.dist-info/LICENSE` & `aicoder-0.3.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `aicoder-0.3.3.dist-info/RECORD` & `aicoder-0.3.4.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 aicoder/AICoder.py,sha256=JD6NVUiqbQH9yKxSCeoynQwcIWDrWJCuipwwoqFJ8sA,12669
 aicoder/AICoderFull.py,sha256=ZmQtR3QrZs4hSXPaSdeMgfBSHYITpadujk3HL6Wat_Y,8088
-aicoder/AICoderPartial.py,sha256=H5oO0Un02xfZTOP9oeT-46pC-NmKbrrN6r9w8J1aMlo,6107
+aicoder/AICoderPartial.py,sha256=lgQc6HtbMNsyqHjb5Z3HFctOinhNBYvKyB2OekB0KYY,6927
 aicoder/AICoderPrompts.py,sha256=EyVLCIKkUDACV0swEHWVfRPNU_cQwYbLIIQ8nFI2VJY,3571
 aicoder/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 aicoder/main.py,sha256=WYdFffXI3V3r6sI8wcF_FBC_Dsm1VmQ_l9x6mFDZvZ4,14606
-aicoder-0.3.3.dist-info/LICENSE,sha256=nGKG3YDYTyar3KKwoaLPInTfnNQtuvh4aMwTADTd0L8,18809
-aicoder-0.3.3.dist-info/METADATA,sha256=VQT5yuZiDJUuF8NGQaRi3SdXWHa48oXUKsPJvXGEJvo,473
-aicoder-0.3.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-aicoder-0.3.3.dist-info/entry_points.txt,sha256=m__okhQaM4kZ8CCfSA5VGUyQ0gf7TIGax6DhXdTnAeA,46
-aicoder-0.3.3.dist-info/top_level.txt,sha256=B8Pf-hhM5icZE_7vMCXD5mXWG0MAqt5ImotI1aNXdWQ,8
-aicoder-0.3.3.dist-info/RECORD,,
+aicoder-0.3.4.dist-info/LICENSE,sha256=nGKG3YDYTyar3KKwoaLPInTfnNQtuvh4aMwTADTd0L8,18809
+aicoder-0.3.4.dist-info/METADATA,sha256=feCP0HDouEZr35na44zIyNIZfXHKohnoEeKcExU4C40,473
+aicoder-0.3.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+aicoder-0.3.4.dist-info/entry_points.txt,sha256=m__okhQaM4kZ8CCfSA5VGUyQ0gf7TIGax6DhXdTnAeA,46
+aicoder-0.3.4.dist-info/top_level.txt,sha256=B8Pf-hhM5icZE_7vMCXD5mXWG0MAqt5ImotI1aNXdWQ,8
+aicoder-0.3.4.dist-info/RECORD,,
```

