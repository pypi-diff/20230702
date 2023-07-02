# Comparing `tmp/fastq2folder-1.0.5.tar.gz` & `tmp/fastq2folder-1.0.6.tar.gz`

## Comparing `fastq2folder-1.0.5.tar` & `fastq2folder-1.0.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastq2folder-1.0.5/src/fastq2folder/__init__.py
--rw-r--r--   0        0        0     9241 2020-02-02 00:00:00.000000 fastq2folder-1.0.5/src/fastq2folder/fastq2folder.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 fastq2folder-1.0.5/LICENSE
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 fastq2folder-1.0.5/README.md
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 fastq2folder-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 fastq2folder-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastq2folder-1.0.6/src/fastq2folder/__init__.py
+-rw-r--r--   0        0        0     9241 2020-02-02 00:00:00.000000 fastq2folder-1.0.6/src/fastq2folder/fastq2folder.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 fastq2folder-1.0.6/LICENSE
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 fastq2folder-1.0.6/README.md
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 fastq2folder-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 fastq2folder-1.0.6/PKG-INFO
```

### Comparing `fastq2folder-1.0.5/src/fastq2folder/fastq2folder.py` & `fastq2folder-1.0.6/src/fastq2folder/fastq2folder.py`

 * *Files identical despite different names*

### Comparing `fastq2folder-1.0.5/LICENSE` & `fastq2folder-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fastq2folder-1.0.5/README.md` & `fastq2folder-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `fastq2folder-1.0.5/pyproject.toml` & `fastq2folder-1.0.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,49 @@
 00000000: 5b62 7569 6c64 2d73 7973 7465 6d5d 0d0a  [build-system]..
 00000010: 7265 7175 6972 6573 203d 205b 2268 6174  requires = ["hat
-00000020: 6368 6c69 6e67 222c 2022 7061 6e64 6173  chling", "pandas
-00000030: 222c 2022 4269 6f22 2c20 2273 6369 7079  ", "Bio", "scipy
-00000040: 222c 2022 6e75 6d70 7922 2c20 226d 6174  ", "numpy", "mat
-00000050: 706c 6f74 6c69 6222 2c20 2273 6561 626f  plotlib", "seabo
-00000060: 726e 225d 0d0a 6275 696c 642d 6261 636b  rn"]..build-back
-00000070: 656e 6420 3d20 2268 6174 6368 6c69 6e67  end = "hatchling
-00000080: 2e62 7569 6c64 220d 0a0d 0a5b 7072 6f6a  .build"....[proj
-00000090: 6563 745d 0d0a 6e61 6d65 203d 2022 6661  ect]..name = "fa
-000000a0: 7374 7132 666f 6c64 6572 220d 0a76 6572  stq2folder"..ver
-000000b0: 7369 6f6e 203d 2022 312e 302e 3522 0d0a  sion = "1.0.5"..
-000000c0: 6175 7468 6f72 7320 3d20 5b0d 0a20 207b  authors = [..  {
-000000d0: 206e 616d 653d 2245 6c69 7a61 6265 7468   name="Elizabeth
-000000e0: 2047 6172 646e 6572 222c 2065 6d61 696c   Gardner", email
-000000f0: 3d22 6567 6172 3138 3131 3140 676d 6169  ="egar18111@gmai
-00000100: 6c2e 636f 6d22 207d 2c0d 0a5d 0d0a 6465  l.com" },..]..de
-00000110: 7363 7269 7074 696f 6e20 3d20 2253 6372  scription = "Scr
-00000120: 6970 7420 746f 2070 726f 6365 7373 2066  ipt to process f
-00000130: 6173 7471 2066 696c 6573 2062 6566 6f72  astq files befor
-00000140: 6520 6570 6932 6d65 2061 6e61 6c79 7369  e epi2me analysi
-00000150: 7322 0d0a 7265 6164 6d65 203d 2022 5245  s"..readme = "RE
-00000160: 4144 4d45 2e6d 6422 0d0a 7265 7175 6972  ADME.md"..requir
-00000170: 6573 2d70 7974 686f 6e20 3d20 223e 3d33  es-python = ">=3
-00000180: 2e37 220d 0a0d 0a63 6c61 7373 6966 6965  .7"....classifie
-00000190: 7273 203d 205b 0d0a 2020 2020 2250 726f  rs = [..    "Pro
-000001a0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-000001b0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-000001c0: 222c 0d0a 2020 2020 224c 6963 656e 7365  ",..    "License
-000001d0: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
-000001e0: 203a 3a20 4d49 5420 4c69 6365 6e73 6522   :: MIT License"
-000001f0: 2c0d 0a20 2020 2022 4f70 6572 6174 696e  ,..    "Operatin
-00000200: 6720 5379 7374 656d 203a 3a20 4f53 2049  g System :: OS I
-00000210: 6e64 6570 656e 6465 6e74 222c 0d0a 5d0d  ndependent",..].
-00000220: 0a0d 0a5b 7072 6f6a 6563 742e 7572 6c73  ...[project.urls
-00000230: 5d0d 0a22 486f 6d65 7061 6765 2220 3d20  ].."Homepage" = 
-00000240: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
-00000250: 636f 6d2f 7079 7061 2f73 616d 706c 6570  com/pypa/samplep
-00000260: 726f 6a65 6374 220d 0a22 4275 6720 5472  roject".."Bug Tr
-00000270: 6163 6b65 7222 203d 2022 6874 7470 733a  acker" = "https:
-00000280: 2f2f 6769 7468 7562 2e63 6f6d 2f70 7970  //github.com/pyp
-00000290: 612f 7361 6d70 6c65 7072 6f6a 6563 742f  a/sampleproject/
-000002a0: 6973 7375 6573 22                        issues"
+00000020: 6368 6c69 6e67 225d 0d0a 6275 696c 642d  chling"]..build-
+00000030: 6261 636b 656e 6420 3d20 2268 6174 6368  backend = "hatch
+00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
+00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
+00000060: 2022 6661 7374 7132 666f 6c64 6572 220d   "fastq2folder".
+00000070: 0a76 6572 7369 6f6e 203d 2022 312e 302e  .version = "1.0.
+00000080: 3622 0d0a 6175 7468 6f72 7320 3d20 5b0d  6"..authors = [.
+00000090: 0a20 207b 206e 616d 653d 2245 6c69 7a61  .  { name="Eliza
+000000a0: 6265 7468 2047 6172 646e 6572 222c 2065  beth Gardner", e
+000000b0: 6d61 696c 3d22 6567 6172 3138 3131 3140  mail="egar18111@
+000000c0: 676d 6169 6c2e 636f 6d22 207d 2c0d 0a5d  gmail.com" },..]
+000000d0: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
+000000e0: 2253 6372 6970 7420 746f 2070 726f 6365  "Script to proce
+000000f0: 7373 2066 6173 7471 2066 696c 6573 2062  ss fastq files b
+00000100: 6566 6f72 6520 6570 6932 6d65 2061 6e61  efore epi2me ana
+00000110: 6c79 7369 7322 0d0a 7265 6164 6d65 203d  lysis"..readme =
+00000120: 2022 5245 4144 4d45 2e6d 6422 0d0a 7265   "README.md"..re
+00000130: 7175 6972 6573 2d70 7974 686f 6e20 3d20  quires-python = 
+00000140: 223e 3d33 2e37 220d 0a0d 0a64 6570 656e  ">=3.7"....depen
+00000150: 6465 6e63 6965 7320 3d20 5b0d 0a20 2022  dencies = [..  "
+00000160: 7061 6e64 6173 203e 3d20 312e 342e 3222  pandas >= 1.4.2"
+00000170: 2c0d 0a20 2022 4269 6f20 3e3d 2031 2e35  ,..  "Bio >= 1.5
+00000180: 2e39 222c 0d0a 2020 2273 6369 7079 203e  .9",..  "scipy >
+00000190: 3d20 312e 3130 2e31 222c 0d0a 2020 226e  = 1.10.1",..  "n
+000001a0: 756d 7079 203e 3d20 312e 3232 2e34 222c  umpy >= 1.22.4",
+000001b0: 0d0a 2020 226d 6174 706c 6f74 6c69 6220  ..  "matplotlib 
+000001c0: 3e3d 2033 2e36 2e32 222c 0d0a 2020 2273  >= 3.6.2",..  "s
+000001d0: 6561 626f 726e 203e 3d20 302e 3132 2e32  eaborn >= 0.12.2
+000001e0: 220d 0a20 205d 0d0a 0d0a 636c 6173 7369  "..  ]....classi
+000001f0: 6669 6572 7320 3d20 5b0d 0a20 2020 2022  fiers = [..    "
+00000200: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000210: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000220: 3a20 3322 2c0d 0a20 2020 2022 4c69 6365  : 3",..    "Lice
+00000230: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
+00000240: 7665 6420 3a3a 204d 4954 204c 6963 656e  ved :: MIT Licen
+00000250: 7365 222c 0d0a 2020 2020 224f 7065 7261  se",..    "Opera
+00000260: 7469 6e67 2053 7973 7465 6d20 3a3a 204f  ting System :: O
+00000270: 5320 496e 6465 7065 6e64 656e 7422 2c0d  S Independent",.
+00000280: 0a5d 0d0a 0d0a 5b70 726f 6a65 6374 2e75  .]....[project.u
+00000290: 726c 735d 0d0a 2248 6f6d 6570 6167 6522  rls].."Homepage"
+000002a0: 203d 2022 6874 7470 733a 2f2f 6769 7468   = "https://gith
+000002b0: 7562 2e63 6f6d 2f70 7970 612f 7361 6d70  ub.com/pypa/samp
+000002c0: 6c65 7072 6f6a 6563 7422 0d0a 2242 7567  leproject".."Bug
+000002d0: 2054 7261 636b 6572 2220 3d20 2268 7474   Tracker" = "htt
+000002e0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000002f0: 7079 7061 2f73 616d 706c 6570 726f 6a65  pypa/sampleproje
+00000300: 6374 2f69 7373 7565 7322                 ct/issues"
```

### Comparing `fastq2folder-1.0.5/PKG-INFO` & `fastq2folder-1.0.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 Metadata-Version: 2.1
 Name: fastq2folder
-Version: 1.0.5
+Version: 1.0.6
 Summary: Script to process fastq files before epi2me analysis
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Elizabeth Gardner <egar18111@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
+Requires-Dist: bio>=1.5.9
+Requires-Dist: matplotlib>=3.6.2
+Requires-Dist: numpy>=1.22.4
+Requires-Dist: pandas>=1.4.2
+Requires-Dist: scipy>=1.10.1
+Requires-Dist: seaborn>=0.12.2
 Description-Content-Type: text/markdown
 
 
 This code takes the fastq_pass folder generated by the MinION and creates a new folder where the fastq files are sorted into bins based on the estimated size.  
 
 Start with the fastq_pass folder with the barcode folders containing the zipped fastq files.  In the same parent directory, a new folder called 'fastq_bins' will be created.  The fastqs will be unzipped, read lengths are estimated, and then sorted into a folder called bin2000, bin5000, etc., where the bin number is the estimated plasmid size to enter in epi2me.  A summary file pdf is also added to the 'fastq_bins' directory.
```

