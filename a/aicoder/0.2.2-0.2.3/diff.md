# Comparing `tmp/aicoder-0.2.2-py3-none-any.whl.zip` & `tmp/aicoder-0.2.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 21450 bytes, number of entries: 12
+Zip file size: 21552 bytes, number of entries: 12
 -rw-r--r--  2.0 unx    12669 b- defN 23-Jun-30 12:05 aicoder/AICoder.py
 -rw-r--r--  2.0 unx     8088 b- defN 23-Jun-30 12:27 aicoder/AICoderFull.py
--rw-r--r--  2.0 unx     5449 b- defN 23-Jun-30 12:04 aicoder/AICoderPartial.py
+-rw-r--r--  2.0 unx     6030 b- defN 23-Jul-02 14:23 aicoder/AICoderPartial.py
 -rw-r--r--  2.0 unx     3571 b- defN 23-Jun-30 12:29 aicoder/AICoderPrompts.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-29 11:14 aicoder/__init__.py
 -rw-r--r--  2.0 unx    14606 b- defN 23-Jul-02 14:09 aicoder/main.py
--rw-r--r--  2.0 unx    18809 b- defN 23-Jul-02 14:11 aicoder-0.2.2.dist-info/LICENSE
--rw-r--r--  2.0 unx      473 b- defN 23-Jul-02 14:11 aicoder-0.2.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-02 14:11 aicoder-0.2.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       46 b- defN 23-Jul-02 14:11 aicoder-0.2.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-02 14:11 aicoder-0.2.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      945 b- defN 23-Jul-02 14:11 aicoder-0.2.2.dist-info/RECORD
-12 files, 64756 bytes uncompressed, 19870 bytes compressed:  69.3%
+-rw-r--r--  2.0 unx    18809 b- defN 23-Jul-02 14:23 aicoder-0.2.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx      473 b- defN 23-Jul-02 14:23 aicoder-0.2.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-02 14:23 aicoder-0.2.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       46 b- defN 23-Jul-02 14:23 aicoder-0.2.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-02 14:23 aicoder-0.2.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      945 b- defN 23-Jul-02 14:23 aicoder-0.2.3.dist-info/RECORD
+12 files, 65337 bytes uncompressed, 19972 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: aicoder/__init__.py
 Comment: 
 
 Filename: aicoder/main.py
 Comment: 
 
-Filename: aicoder-0.2.2.dist-info/LICENSE
+Filename: aicoder-0.2.3.dist-info/LICENSE
 Comment: 
 
-Filename: aicoder-0.2.2.dist-info/METADATA
+Filename: aicoder-0.2.3.dist-info/METADATA
 Comment: 
 
-Filename: aicoder-0.2.2.dist-info/WHEEL
+Filename: aicoder-0.2.3.dist-info/WHEEL
 Comment: 
 
-Filename: aicoder-0.2.2.dist-info/entry_points.txt
+Filename: aicoder-0.2.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: aicoder-0.2.2.dist-info/top_level.txt
+Filename: aicoder-0.2.3.dist-info/top_level.txt
 Comment: 
 
-Filename: aicoder-0.2.2.dist-info/RECORD
+Filename: aicoder-0.2.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aicoder/AICoderPartial.py

```diff
@@ -99,14 +99,25 @@
 
     def create_pull_request(self, commit_message: str, commit_body: str, orig_branch: str, to_branch: str, repo_name: str):
         """Function that creates a pull request"""
 
         github = Github(self.github_token)
         repo = github.get_repo(repo_name)
 
+        # Set git user.name and user.email if they are not set
+        git_config_username = subprocess.check_output(["git", "config", "user.name"]).decode().strip()
+        git_config_email = subprocess.check_output(["git", "config", "user.email"]).decode().strip()
+
+        # Set git user.name and user.email if they are not set
+        if not git_config_username:
+            subprocess.run(["git", "config", "user.name", "aicoder"], check=True)
+
+        if not git_config_email:
+            subprocess.run(["git", "config", "user.email", "aicoder@aicoderhub.ai"], check=True)
+
         # Commit changes to the new branch
         subprocess.run(["git", "add", "."], check=True)
         subprocess.run(["git", "commit", "-m", commit_message[:70]], check=True)
 
         # Get the HTTPS URL of the origin remote, and replace "https://" with "https://token@"
         origin_url = subprocess.check_output(["git", "config", "--get", "remote.origin.url"]).strip().decode()
         new_origin_url = origin_url.replace("https://", f"https://{urllib.parse.quote(self.github_token)}@")
```

## Comparing `aicoder-0.2.2.dist-info/LICENSE` & `aicoder-0.2.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `aicoder-0.2.2.dist-info/RECORD` & `aicoder-0.2.3.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 aicoder/AICoder.py,sha256=JD6NVUiqbQH9yKxSCeoynQwcIWDrWJCuipwwoqFJ8sA,12669
 aicoder/AICoderFull.py,sha256=ZmQtR3QrZs4hSXPaSdeMgfBSHYITpadujk3HL6Wat_Y,8088
-aicoder/AICoderPartial.py,sha256=_NadBlkGml2FSfK0gJPyN4zVUkQpe6e6nwAeywmJlEI,5449
+aicoder/AICoderPartial.py,sha256=fiNx747bJvpSsIYXvxi62VsEMERdi83lq1_x-quAKl8,6030
 aicoder/AICoderPrompts.py,sha256=EyVLCIKkUDACV0swEHWVfRPNU_cQwYbLIIQ8nFI2VJY,3571
 aicoder/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 aicoder/main.py,sha256=WYdFffXI3V3r6sI8wcF_FBC_Dsm1VmQ_l9x6mFDZvZ4,14606
-aicoder-0.2.2.dist-info/LICENSE,sha256=nGKG3YDYTyar3KKwoaLPInTfnNQtuvh4aMwTADTd0L8,18809
-aicoder-0.2.2.dist-info/METADATA,sha256=tKSj-bBDFHVF7JsM620-9AhIW3GaBIk6d42oO7NI24Q,473
-aicoder-0.2.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-aicoder-0.2.2.dist-info/entry_points.txt,sha256=m__okhQaM4kZ8CCfSA5VGUyQ0gf7TIGax6DhXdTnAeA,46
-aicoder-0.2.2.dist-info/top_level.txt,sha256=B8Pf-hhM5icZE_7vMCXD5mXWG0MAqt5ImotI1aNXdWQ,8
-aicoder-0.2.2.dist-info/RECORD,,
+aicoder-0.2.3.dist-info/LICENSE,sha256=nGKG3YDYTyar3KKwoaLPInTfnNQtuvh4aMwTADTd0L8,18809
+aicoder-0.2.3.dist-info/METADATA,sha256=hEVl6nyLuYlX4CXuUpYohnp97rBoz49UG70Es_HQC1s,473
+aicoder-0.2.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+aicoder-0.2.3.dist-info/entry_points.txt,sha256=m__okhQaM4kZ8CCfSA5VGUyQ0gf7TIGax6DhXdTnAeA,46
+aicoder-0.2.3.dist-info/top_level.txt,sha256=B8Pf-hhM5icZE_7vMCXD5mXWG0MAqt5ImotI1aNXdWQ,8
+aicoder-0.2.3.dist-info/RECORD,,
```

