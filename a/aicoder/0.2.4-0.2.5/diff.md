# Comparing `tmp/aicoder-0.2.4-py3-none-any.whl.zip` & `tmp/aicoder-0.2.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 21498 bytes, number of entries: 12
+Zip file size: 21492 bytes, number of entries: 12
 -rw-r--r--  2.0 unx    12669 b- defN 23-Jun-30 12:05 aicoder/AICoder.py
 -rw-r--r--  2.0 unx     8088 b- defN 23-Jun-30 12:27 aicoder/AICoderFull.py
--rw-r--r--  2.0 unx     5658 b- defN 23-Jul-02 14:27 aicoder/AICoderPartial.py
+-rw-r--r--  2.0 unx     5648 b- defN 23-Jul-02 14:31 aicoder/AICoderPartial.py
 -rw-r--r--  2.0 unx     3571 b- defN 23-Jun-30 12:29 aicoder/AICoderPrompts.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-29 11:14 aicoder/__init__.py
 -rw-r--r--  2.0 unx    14606 b- defN 23-Jul-02 14:09 aicoder/main.py
--rw-r--r--  2.0 unx    18809 b- defN 23-Jul-02 14:28 aicoder-0.2.4.dist-info/LICENSE
--rw-r--r--  2.0 unx      473 b- defN 23-Jul-02 14:28 aicoder-0.2.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-02 14:28 aicoder-0.2.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       46 b- defN 23-Jul-02 14:28 aicoder-0.2.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-02 14:28 aicoder-0.2.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      945 b- defN 23-Jul-02 14:28 aicoder-0.2.4.dist-info/RECORD
-12 files, 64965 bytes uncompressed, 19918 bytes compressed:  69.3%
+-rw-r--r--  2.0 unx    18809 b- defN 23-Jul-02 14:31 aicoder-0.2.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx      473 b- defN 23-Jul-02 14:31 aicoder-0.2.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-02 14:31 aicoder-0.2.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       46 b- defN 23-Jul-02 14:31 aicoder-0.2.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-02 14:31 aicoder-0.2.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      945 b- defN 23-Jul-02 14:31 aicoder-0.2.5.dist-info/RECORD
+12 files, 64955 bytes uncompressed, 19912 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: aicoder/__init__.py
 Comment: 
 
 Filename: aicoder/main.py
 Comment: 
 
-Filename: aicoder-0.2.4.dist-info/LICENSE
+Filename: aicoder-0.2.5.dist-info/LICENSE
 Comment: 
 
-Filename: aicoder-0.2.4.dist-info/METADATA
+Filename: aicoder-0.2.5.dist-info/METADATA
 Comment: 
 
-Filename: aicoder-0.2.4.dist-info/WHEEL
+Filename: aicoder-0.2.5.dist-info/WHEEL
 Comment: 
 
-Filename: aicoder-0.2.4.dist-info/entry_points.txt
+Filename: aicoder-0.2.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: aicoder-0.2.4.dist-info/top_level.txt
+Filename: aicoder-0.2.5.dist-info/top_level.txt
 Comment: 
 
-Filename: aicoder-0.2.4.dist-info/RECORD
+Filename: aicoder-0.2.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aicoder/AICoderPartial.py

```diff
@@ -100,16 +100,16 @@
     def create_pull_request(self, commit_message: str, commit_body: str, orig_branch: str, to_branch: str, repo_name: str):
         """Function that creates a pull request"""
 
         github = Github(self.github_token)
         repo = github.get_repo(repo_name)
 
         # Set git user.name and user.email if they are not set
-        subprocess.run(["git", "config", "user.name"]).decode().strip()
-        subprocess.run(["git", "config", "user.email"]).decode().strip()
+        subprocess.run(["git", "config", "user.name"], check=True)
+        subprocess.run(["git", "config", "user.email"], check=True)
 
         # Commit changes to the new branch
         subprocess.run(["git", "add", "."], check=True)
         subprocess.run(["git", "commit", "-m", commit_message[:70]], check=True)
 
         # Get the HTTPS URL of the origin remote, and replace "https://" with "https://token@"
         origin_url = subprocess.check_output(["git", "config", "--get", "remote.origin.url"]).strip().decode()
```

## Comparing `aicoder-0.2.4.dist-info/LICENSE` & `aicoder-0.2.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `aicoder-0.2.4.dist-info/RECORD` & `aicoder-0.2.5.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 aicoder/AICoder.py,sha256=JD6NVUiqbQH9yKxSCeoynQwcIWDrWJCuipwwoqFJ8sA,12669
 aicoder/AICoderFull.py,sha256=ZmQtR3QrZs4hSXPaSdeMgfBSHYITpadujk3HL6Wat_Y,8088
-aicoder/AICoderPartial.py,sha256=Fg-UKcM5uc90QWeoO8yGcg2UHm-mPQfsK9Xk_rGyEfo,5658
+aicoder/AICoderPartial.py,sha256=c3degYT5OVAbvx6rSTcTaQpRvCWfLLtHeNwn4hY5owA,5648
 aicoder/AICoderPrompts.py,sha256=EyVLCIKkUDACV0swEHWVfRPNU_cQwYbLIIQ8nFI2VJY,3571
 aicoder/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 aicoder/main.py,sha256=WYdFffXI3V3r6sI8wcF_FBC_Dsm1VmQ_l9x6mFDZvZ4,14606
-aicoder-0.2.4.dist-info/LICENSE,sha256=nGKG3YDYTyar3KKwoaLPInTfnNQtuvh4aMwTADTd0L8,18809
-aicoder-0.2.4.dist-info/METADATA,sha256=Nvi2wjas2jLzTzk1UE05OlCQOfPpuWLCAqs5TXAxCAE,473
-aicoder-0.2.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-aicoder-0.2.4.dist-info/entry_points.txt,sha256=m__okhQaM4kZ8CCfSA5VGUyQ0gf7TIGax6DhXdTnAeA,46
-aicoder-0.2.4.dist-info/top_level.txt,sha256=B8Pf-hhM5icZE_7vMCXD5mXWG0MAqt5ImotI1aNXdWQ,8
-aicoder-0.2.4.dist-info/RECORD,,
+aicoder-0.2.5.dist-info/LICENSE,sha256=nGKG3YDYTyar3KKwoaLPInTfnNQtuvh4aMwTADTd0L8,18809
+aicoder-0.2.5.dist-info/METADATA,sha256=4uYYmGiXMICzjzsCoF0zBsT5PRY7DKr-ArZvHhaIYxY,473
+aicoder-0.2.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+aicoder-0.2.5.dist-info/entry_points.txt,sha256=m__okhQaM4kZ8CCfSA5VGUyQ0gf7TIGax6DhXdTnAeA,46
+aicoder-0.2.5.dist-info/top_level.txt,sha256=B8Pf-hhM5icZE_7vMCXD5mXWG0MAqt5ImotI1aNXdWQ,8
+aicoder-0.2.5.dist-info/RECORD,,
```

