# Comparing `tmp/aicoder-0.2.0-py3-none-any.whl.zip` & `tmp/aicoder-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 21432 bytes, number of entries: 12
+Zip file size: 21442 bytes, number of entries: 12
 -rw-r--r--  2.0 unx    12669 b- defN 23-Jun-30 12:05 aicoder/AICoder.py
--rw-r--r--  2.0 unx     8138 b- defN 23-Jun-30 12:04 aicoder/AICoderFull.py
+-rw-r--r--  2.0 unx     8088 b- defN 23-Jun-30 12:27 aicoder/AICoderFull.py
 -rw-r--r--  2.0 unx     5449 b- defN 23-Jun-30 12:04 aicoder/AICoderPartial.py
--rw-r--r--  2.0 unx     3481 b- defN 23-Jun-28 23:49 aicoder/AICoderPrompts.py
+-rw-r--r--  2.0 unx     3571 b- defN 23-Jun-30 12:29 aicoder/AICoderPrompts.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-29 11:14 aicoder/__init__.py
--rw-r--r--  2.0 unx    14586 b- defN 23-Jun-30 12:04 aicoder/main.py
--rw-r--r--  2.0 unx    18809 b- defN 23-Jun-30 12:05 aicoder-0.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      473 b- defN 23-Jun-30 12:05 aicoder-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-30 12:05 aicoder-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       46 b- defN 23-Jun-30 12:05 aicoder-0.2.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Jun-30 12:05 aicoder-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      945 b- defN 23-Jun-30 12:05 aicoder-0.2.0.dist-info/RECORD
-12 files, 64696 bytes uncompressed, 19852 bytes compressed:  69.3%
+-rw-r--r--  2.0 unx    14599 b- defN 23-Jun-30 12:18 aicoder/main.py
+-rw-r--r--  2.0 unx    18809 b- defN 23-Jul-02 13:22 aicoder-0.2.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      473 b- defN 23-Jul-02 13:22 aicoder-0.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-02 13:22 aicoder-0.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       46 b- defN 23-Jul-02 13:22 aicoder-0.2.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-02 13:22 aicoder-0.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      945 b- defN 23-Jul-02 13:22 aicoder-0.2.1.dist-info/RECORD
+12 files, 64749 bytes uncompressed, 19862 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: aicoder/__init__.py
 Comment: 
 
 Filename: aicoder/main.py
 Comment: 
 
-Filename: aicoder-0.2.0.dist-info/LICENSE
+Filename: aicoder-0.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: aicoder-0.2.0.dist-info/METADATA
+Filename: aicoder-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: aicoder-0.2.0.dist-info/WHEEL
+Filename: aicoder-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: aicoder-0.2.0.dist-info/entry_points.txt
+Filename: aicoder-0.2.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: aicoder-0.2.0.dist-info/top_level.txt
+Filename: aicoder-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: aicoder-0.2.0.dist-info/RECORD
+Filename: aicoder-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aicoder/AICoderFull.py

```diff
@@ -29,16 +29,16 @@
         """Function that asks the model to return the file names to generate the program"""
 
         logger.info("Generating list of files...")
         msg = GET_ALL_FILES + extra_content
         files_to_generate = self.contact(msg)
         try:
             try:
-                all_files = json.loads(files_to_generate)
-            except json.decoder.JSONDecodeError as e:
+                all_files = json.loads(self.remove_fences(files_to_generate))
+            except Exception as e:
                 all_files = self.fix_json(msg, files_to_generate, str(e))
             
             # If more than 50% of files have .h extension, retry
             if len([file for file in all_files if file["path"].endswith(".h")]) > len(all_files) * 0.75 and len(all_files) > 3:
                 logger.warning("Found more than 75% of .h files, retrying asking for the implementations...")
                 extra_content = "\nLast time I asked your response was:\n" + files_to_generate
                 extra_content += "\n\nDon't forget to include the implementation files."
@@ -80,16 +80,16 @@
             user_input = input()
             if user_input.lower() in ["no", "n"]:
                 print("I'll try to generate the files again... Tell me the problem:")
                 extra_content = "\n" + input()
                 return self.get_files_to_generate(extra_content=extra_content)
             
             return all_files
-        except:
-            raise Exception("The response is not a valid JSON: " + files_to_generate)
+        except Exception as e:
+            raise e
 
 
     def wait_on_dependencies(self, file: dict) -> str:
         """Function that waits until all the dependencies are generated"""
 
         dependencies_content = ""
         cont = 0
```

## aicoder/AICoderPrompts.py

```diff
@@ -14,15 +14,16 @@
     {
         "path": "./generated/main.py",
         "description": "<This is a description of the content ./generated/main.py>",
         "dependencies": ["./generated/file2.h", "./generated/file3.py"]
     },
 ]
 
-If needed don't forget headers '.h' and  implementations '.c, .cpp, .m'..."""
+If needed don't forget headers '.h' and  implementations '.c, .cpp, .m'...
+The response must be only a valid JSON with the structure above, don't add anything else."""
 
 
 GET_FILE_CONTENTS = """These are the files we are generating for the program:\n
 __FILES_JSON__
 
 Return only the content that the file __FILE_PATH__ must have. Don't leave TODOs or incomplete code, write all the code of the file, and don't forget imports."""
```

## aicoder/main.py

```diff
@@ -29,18 +29,18 @@
 
 # Function to generate a random string
 def get_random_string(length):
     letters = string.ascii_letters
     return ''.join(random.choice(letters) for _ in range(length))
 
 # Function to generate a full program
-def full_generator(prompt: str, api_key: str, github_token: str, model: str="gpt-4"):
+def full_generator(prompt: str, api_key: str, model: str="gpt-4"):
     if os.path.isdir("generated"):
         os.system("rm -rf generated")
-    aicoderfull = AICoderFull(prompt, api_key, github_token, model)
+    aicoderfull = AICoderFull(prompt, api_key, "", model)
     aicoderfull.generate_program()
 
 # Function to generate a file from templates
 def file_generator(prompt: str, api_key: str, github_token: str, model: str, template_files: list, orig_branch: str, new_branch: str, repo_name: str):
     aicoderpartial = AICoderPartial(prompt, api_key, github_token, model)
     aicoderpartial.gen_file_from_templates(template_files, prompt, orig_branch, new_branch, repo_name)
 
@@ -165,18 +165,20 @@
             template_files = list(os.environ.get("TEMPALTE_FILES").split(",")) or args.template_files
                 
         elif args.mode in ["file-enhancer", "file-comments", "file-security", "file-optimizer", "file-bugfixer"]:
             check_path = os.environ.get("CHECK_PATH") or args.path
     
     if not prompt and not args.mode in ["file-comments", "file-security", "file-optimizer"]:
         logger.error("Error: Missing prompt.")
+        parser.print_help()
         sys.exit(1)
     
     if not api_key:
         logger.error("Error: Missing API key.")
+        parser.print_help()
         sys.exit(1)
     
     # If prompt is file path, read it
     if prompt and os.path.isfile(prompt):
         logger.debug(f"Prompt read from {prompt}")
         with open(prompt, "r") as f:
             prompt = f.read()
@@ -184,15 +186,15 @@
     # If prompt is url, download it
     elif prompt and prompt.startswith("http"):
         logger.debug(f"Prompt downloaded from {prompt}")
         prompt = requests.get(prompt).text
     
     # If full generator mode
     if args.mode == 'full-generator':
-        full_generator(prompt, api_key, github_token, model)
+        full_generator(prompt, api_key, model)
         exit(0)
     
     ### Checks for single file modifiers
     
     if not github_token:
         logger.warning("No Github token. PRs cannot be created automatically.")
```

## Comparing `aicoder-0.2.0.dist-info/LICENSE` & `aicoder-0.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `aicoder-0.2.0.dist-info/RECORD` & `aicoder-0.2.1.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 aicoder/AICoder.py,sha256=JD6NVUiqbQH9yKxSCeoynQwcIWDrWJCuipwwoqFJ8sA,12669
-aicoder/AICoderFull.py,sha256=twZM0v57Zpa0S8nE9pmv-DWsncZcxDPVcXiOZgTWfzU,8138
+aicoder/AICoderFull.py,sha256=ZmQtR3QrZs4hSXPaSdeMgfBSHYITpadujk3HL6Wat_Y,8088
 aicoder/AICoderPartial.py,sha256=_NadBlkGml2FSfK0gJPyN4zVUkQpe6e6nwAeywmJlEI,5449
-aicoder/AICoderPrompts.py,sha256=ZQGA2rNfSHzYdmc914960_HOJagGO_AuRXn_08sMeW4,3481
+aicoder/AICoderPrompts.py,sha256=EyVLCIKkUDACV0swEHWVfRPNU_cQwYbLIIQ8nFI2VJY,3571
 aicoder/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-aicoder/main.py,sha256=wXJXURSK7-H1_K33LHVhf_zh2OFmzvz389fgla7lDPc,14586
-aicoder-0.2.0.dist-info/LICENSE,sha256=nGKG3YDYTyar3KKwoaLPInTfnNQtuvh4aMwTADTd0L8,18809
-aicoder-0.2.0.dist-info/METADATA,sha256=DiiPdmkTBgNHPCQ1A7uA5_BREvECxdrAiXQoKC6xY1s,473
-aicoder-0.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-aicoder-0.2.0.dist-info/entry_points.txt,sha256=m__okhQaM4kZ8CCfSA5VGUyQ0gf7TIGax6DhXdTnAeA,46
-aicoder-0.2.0.dist-info/top_level.txt,sha256=B8Pf-hhM5icZE_7vMCXD5mXWG0MAqt5ImotI1aNXdWQ,8
-aicoder-0.2.0.dist-info/RECORD,,
+aicoder/main.py,sha256=A1N1pSQoReeKAbF8of0kJgGxvC8YW_32cA7aLnZ5cDk,14599
+aicoder-0.2.1.dist-info/LICENSE,sha256=nGKG3YDYTyar3KKwoaLPInTfnNQtuvh4aMwTADTd0L8,18809
+aicoder-0.2.1.dist-info/METADATA,sha256=OWyY3d3qbrfm6rhz9do3t7uv2SvJFLWAYYj41viemx0,473
+aicoder-0.2.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+aicoder-0.2.1.dist-info/entry_points.txt,sha256=m__okhQaM4kZ8CCfSA5VGUyQ0gf7TIGax6DhXdTnAeA,46
+aicoder-0.2.1.dist-info/top_level.txt,sha256=B8Pf-hhM5icZE_7vMCXD5mXWG0MAqt5ImotI1aNXdWQ,8
+aicoder-0.2.1.dist-info/RECORD,,
```

