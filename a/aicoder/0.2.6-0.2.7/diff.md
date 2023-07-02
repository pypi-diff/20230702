# Comparing `tmp/aicoder-0.2.6-py3-none-any.whl.zip` & `tmp/aicoder-0.2.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 21504 bytes, number of entries: 12
+Zip file size: 21496 bytes, number of entries: 12
 -rw-r--r--  2.0 unx    12669 b- defN 23-Jun-30 12:05 aicoder/AICoder.py
 -rw-r--r--  2.0 unx     8088 b- defN 23-Jun-30 12:27 aicoder/AICoderFull.py
--rw-r--r--  2.0 unx     5684 b- defN 23-Jul-02 14:35 aicoder/AICoderPartial.py
+-rw-r--r--  2.0 unx     5658 b- defN 23-Jul-02 14:47 aicoder/AICoderPartial.py
 -rw-r--r--  2.0 unx     3571 b- defN 23-Jun-30 12:29 aicoder/AICoderPrompts.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-29 11:14 aicoder/__init__.py
 -rw-r--r--  2.0 unx    14606 b- defN 23-Jul-02 14:09 aicoder/main.py
--rw-r--r--  2.0 unx    18809 b- defN 23-Jul-02 14:35 aicoder-0.2.6.dist-info/LICENSE
--rw-r--r--  2.0 unx      473 b- defN 23-Jul-02 14:35 aicoder-0.2.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-02 14:35 aicoder-0.2.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       46 b- defN 23-Jul-02 14:35 aicoder-0.2.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-02 14:35 aicoder-0.2.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      945 b- defN 23-Jul-02 14:35 aicoder-0.2.6.dist-info/RECORD
-12 files, 64991 bytes uncompressed, 19924 bytes compressed:  69.3%
+-rw-r--r--  2.0 unx    18809 b- defN 23-Jul-02 14:47 aicoder-0.2.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx      473 b- defN 23-Jul-02 14:47 aicoder-0.2.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-02 14:47 aicoder-0.2.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       46 b- defN 23-Jul-02 14:47 aicoder-0.2.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-02 14:47 aicoder-0.2.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      945 b- defN 23-Jul-02 14:47 aicoder-0.2.7.dist-info/RECORD
+12 files, 64965 bytes uncompressed, 19916 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: aicoder/__init__.py
 Comment: 
 
 Filename: aicoder/main.py
 Comment: 
 
-Filename: aicoder-0.2.6.dist-info/LICENSE
+Filename: aicoder-0.2.7.dist-info/LICENSE
 Comment: 
 
-Filename: aicoder-0.2.6.dist-info/METADATA
+Filename: aicoder-0.2.7.dist-info/METADATA
 Comment: 
 
-Filename: aicoder-0.2.6.dist-info/WHEEL
+Filename: aicoder-0.2.7.dist-info/WHEEL
 Comment: 
 
-Filename: aicoder-0.2.6.dist-info/entry_points.txt
+Filename: aicoder-0.2.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: aicoder-0.2.6.dist-info/top_level.txt
+Filename: aicoder-0.2.7.dist-info/top_level.txt
 Comment: 
 
-Filename: aicoder-0.2.6.dist-info/RECORD
+Filename: aicoder-0.2.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aicoder/AICoderPartial.py

```diff
@@ -109,15 +109,15 @@
 
         # Commit changes to the new branch
         subprocess.run(["git", "add", "."], check=True)
         subprocess.run(["git", "commit", "-m", commit_message[:70]], check=True)
 
         # Get the HTTPS URL of the origin remote, and replace "https://" with "https://token@"
         origin_url = subprocess.check_output(["git", "config", "--get", "remote.origin.url"]).strip().decode()
-        new_origin_url = origin_url.replace("https://", f"https://{urllib.parse.quote(self.github_token)}@")
+        new_origin_url = f"https://{self.github_token}@github.com/{repo_name}.git"
         
         # Push the changes
         push_result = subprocess.run(["git", "push", "--set-upstream", new_origin_url, orig_branch], text=True, capture_output=True)
         if push_result.returncode != 0:
             print("Failed to push the changes to the origin.")
             return
```

## Comparing `aicoder-0.2.6.dist-info/LICENSE` & `aicoder-0.2.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `aicoder-0.2.6.dist-info/RECORD` & `aicoder-0.2.7.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 aicoder/AICoder.py,sha256=JD6NVUiqbQH9yKxSCeoynQwcIWDrWJCuipwwoqFJ8sA,12669
 aicoder/AICoderFull.py,sha256=ZmQtR3QrZs4hSXPaSdeMgfBSHYITpadujk3HL6Wat_Y,8088
-aicoder/AICoderPartial.py,sha256=B3Hrzns9P9Tk5Z68zjOMejeN2c4mibgLFaHYRoUfm-k,5684
+aicoder/AICoderPartial.py,sha256=GrdHxNoI4g-V20AWXFKoEQx6P4p2PovJILLL5flU8Ao,5658
 aicoder/AICoderPrompts.py,sha256=EyVLCIKkUDACV0swEHWVfRPNU_cQwYbLIIQ8nFI2VJY,3571
 aicoder/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 aicoder/main.py,sha256=WYdFffXI3V3r6sI8wcF_FBC_Dsm1VmQ_l9x6mFDZvZ4,14606
-aicoder-0.2.6.dist-info/LICENSE,sha256=nGKG3YDYTyar3KKwoaLPInTfnNQtuvh4aMwTADTd0L8,18809
-aicoder-0.2.6.dist-info/METADATA,sha256=mTgqLL4EsgDLAU46SVHkTLrbrMW4tQV1Hd5TPhLtPiQ,473
-aicoder-0.2.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-aicoder-0.2.6.dist-info/entry_points.txt,sha256=m__okhQaM4kZ8CCfSA5VGUyQ0gf7TIGax6DhXdTnAeA,46
-aicoder-0.2.6.dist-info/top_level.txt,sha256=B8Pf-hhM5icZE_7vMCXD5mXWG0MAqt5ImotI1aNXdWQ,8
-aicoder-0.2.6.dist-info/RECORD,,
+aicoder-0.2.7.dist-info/LICENSE,sha256=nGKG3YDYTyar3KKwoaLPInTfnNQtuvh4aMwTADTd0L8,18809
+aicoder-0.2.7.dist-info/METADATA,sha256=VK0DnrqshKgUMMbmxHmZ4LwyFdKqTpN3AhjDcgffnEc,473
+aicoder-0.2.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+aicoder-0.2.7.dist-info/entry_points.txt,sha256=m__okhQaM4kZ8CCfSA5VGUyQ0gf7TIGax6DhXdTnAeA,46
+aicoder-0.2.7.dist-info/top_level.txt,sha256=B8Pf-hhM5icZE_7vMCXD5mXWG0MAqt5ImotI1aNXdWQ,8
+aicoder-0.2.7.dist-info/RECORD,,
```

