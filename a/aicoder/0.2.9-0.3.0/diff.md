# Comparing `tmp/aicoder-0.2.9-py3-none-any.whl.zip` & `tmp/aicoder-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 21540 bytes, number of entries: 12
+Zip file size: 21553 bytes, number of entries: 12
 -rw-r--r--  2.0 unx    12669 b- defN 23-Jun-30 12:05 aicoder/AICoder.py
 -rw-r--r--  2.0 unx     8088 b- defN 23-Jun-30 12:27 aicoder/AICoderFull.py
--rw-r--r--  2.0 unx     5812 b- defN 23-Jul-02 15:17 aicoder/AICoderPartial.py
+-rw-r--r--  2.0 unx     5851 b- defN 23-Jul-02 15:21 aicoder/AICoderPartial.py
 -rw-r--r--  2.0 unx     3571 b- defN 23-Jun-30 12:29 aicoder/AICoderPrompts.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-29 11:14 aicoder/__init__.py
 -rw-r--r--  2.0 unx    14606 b- defN 23-Jul-02 14:09 aicoder/main.py
--rw-r--r--  2.0 unx    18809 b- defN 23-Jul-02 15:18 aicoder-0.2.9.dist-info/LICENSE
--rw-r--r--  2.0 unx      473 b- defN 23-Jul-02 15:18 aicoder-0.2.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-02 15:18 aicoder-0.2.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       46 b- defN 23-Jul-02 15:18 aicoder-0.2.9.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-02 15:18 aicoder-0.2.9.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      945 b- defN 23-Jul-02 15:18 aicoder-0.2.9.dist-info/RECORD
-12 files, 65119 bytes uncompressed, 19960 bytes compressed:  69.3%
+-rw-r--r--  2.0 unx    18809 b- defN 23-Jul-02 15:21 aicoder-0.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      473 b- defN 23-Jul-02 15:21 aicoder-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-02 15:21 aicoder-0.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       46 b- defN 23-Jul-02 15:21 aicoder-0.3.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-02 15:21 aicoder-0.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      945 b- defN 23-Jul-02 15:21 aicoder-0.3.0.dist-info/RECORD
+12 files, 65158 bytes uncompressed, 19973 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: aicoder/__init__.py
 Comment: 
 
 Filename: aicoder/main.py
 Comment: 
 
-Filename: aicoder-0.2.9.dist-info/LICENSE
+Filename: aicoder-0.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: aicoder-0.2.9.dist-info/METADATA
+Filename: aicoder-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: aicoder-0.2.9.dist-info/WHEEL
+Filename: aicoder-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: aicoder-0.2.9.dist-info/entry_points.txt
+Filename: aicoder-0.3.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: aicoder-0.2.9.dist-info/top_level.txt
+Filename: aicoder-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: aicoder-0.2.9.dist-info/RECORD
+Filename: aicoder-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aicoder/AICoderPartial.py

```diff
@@ -114,15 +114,15 @@
         # Get the HTTPS URL of the origin remote, and replace "https://" with "https://token@"
         origin_url = subprocess.check_output(["git", "config", "--get", "remote.origin.url"]).strip().decode()
         new_origin_url = origin_url.replace("https://", f"https://{self.github_token}@")
         
         # Push the changes
         push_result = subprocess.run(["git", "push", "--set-upstream", new_origin_url, orig_branch], text=True, capture_output=True)
         if push_result.returncode != 0:
-            print("Failed to push the changes to the origin.")
+            print(f"Failed to push the changes to the origin {new_origin_url}: ", push_result.stderr)
             return
 
         # Create a pull request
         sleep(1)
         logger.debug(f"Creating a pull request to repo {repo_name}, from branch {orig_branch} to branch {to_branch}...")
         pr = repo.create_pull(
             title=commit_message,
```

## Comparing `aicoder-0.2.9.dist-info/LICENSE` & `aicoder-0.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `aicoder-0.2.9.dist-info/RECORD` & `aicoder-0.3.0.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 aicoder/AICoder.py,sha256=JD6NVUiqbQH9yKxSCeoynQwcIWDrWJCuipwwoqFJ8sA,12669
 aicoder/AICoderFull.py,sha256=ZmQtR3QrZs4hSXPaSdeMgfBSHYITpadujk3HL6Wat_Y,8088
-aicoder/AICoderPartial.py,sha256=6-Z70dDESC7ESR6r1TJXNFiz05-yvnYjVAXXk68XFUk,5812
+aicoder/AICoderPartial.py,sha256=CfddiZ0T718vjgrWvKUuLZmf8Sm097NRjY6Y8ZSzQuM,5851
 aicoder/AICoderPrompts.py,sha256=EyVLCIKkUDACV0swEHWVfRPNU_cQwYbLIIQ8nFI2VJY,3571
 aicoder/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 aicoder/main.py,sha256=WYdFffXI3V3r6sI8wcF_FBC_Dsm1VmQ_l9x6mFDZvZ4,14606
-aicoder-0.2.9.dist-info/LICENSE,sha256=nGKG3YDYTyar3KKwoaLPInTfnNQtuvh4aMwTADTd0L8,18809
-aicoder-0.2.9.dist-info/METADATA,sha256=h1BiOJKIpHdpqn2MJUpp_-lfHw0YghEKseirX6DuEzI,473
-aicoder-0.2.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-aicoder-0.2.9.dist-info/entry_points.txt,sha256=m__okhQaM4kZ8CCfSA5VGUyQ0gf7TIGax6DhXdTnAeA,46
-aicoder-0.2.9.dist-info/top_level.txt,sha256=B8Pf-hhM5icZE_7vMCXD5mXWG0MAqt5ImotI1aNXdWQ,8
-aicoder-0.2.9.dist-info/RECORD,,
+aicoder-0.3.0.dist-info/LICENSE,sha256=nGKG3YDYTyar3KKwoaLPInTfnNQtuvh4aMwTADTd0L8,18809
+aicoder-0.3.0.dist-info/METADATA,sha256=V0JFMffuy2uX4iqFqudGziCV-qFGnakAf5YFPpU-aqE,473
+aicoder-0.3.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+aicoder-0.3.0.dist-info/entry_points.txt,sha256=m__okhQaM4kZ8CCfSA5VGUyQ0gf7TIGax6DhXdTnAeA,46
+aicoder-0.3.0.dist-info/top_level.txt,sha256=B8Pf-hhM5icZE_7vMCXD5mXWG0MAqt5ImotI1aNXdWQ,8
+aicoder-0.3.0.dist-info/RECORD,,
```

