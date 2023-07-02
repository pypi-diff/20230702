# Comparing `tmp/cloudflarepycli-1.7.0.tar.gz` & `tmp/cloudflarepycli-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudflarepycli-1.7.0.tar", last modified: Fri Oct 14 17:08:50 2022, max compression
+gzip compressed data, was "cloudflarepycli-1.8.tar", last modified: Sun Jul  2 17:24:24 2023, max compression
```

## Comparing `cloudflarepycli-1.7.0.tar` & `cloudflarepycli-1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-10-14 17:08:50.769501 cloudflarepycli-1.7.0/
--rw-rw-rw-   0        0        0     4416 2022-10-14 17:08:50.769798 cloudflarepycli-1.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     3788 2022-10-11 21:36:20.000000 cloudflarepycli-1.7.0/README.md
--rw-rw-rw-   0        0        0      118 2022-10-14 16:48:01.000000 cloudflarepycli-1.7.0/pyproject.toml
--rw-rw-rw-   0        0        0      962 2022-10-14 17:08:50.770192 cloudflarepycli-1.7.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-10-14 17:08:50.759113 cloudflarepycli-1.7.0/src/
-drwxrwxrwx   0        0        0        0 2022-10-14 17:08:50.763503 cloudflarepycli-1.7.0/src/cloudflarepycli/
--rw-rw-rw-   0        0        0        0 2022-09-03 18:15:25.000000 cloudflarepycli-1.7.0/src/cloudflarepycli/__init__.py
--rw-rw-rw-   0        0        0     1370 2022-10-11 20:10:41.000000 cloudflarepycli-1.7.0/src/cloudflarepycli/__main__.py
--rw-rw-rw-   0        0        0     8074 2022-10-11 21:26:35.000000 cloudflarepycli-1.7.0/src/cloudflarepycli/cloudflareclass.py
-drwxrwxrwx   0        0        0        0 2022-10-14 17:08:50.768501 cloudflarepycli-1.7.0/src/cloudflarepycli.egg-info/
--rw-rw-rw-   0        0        0     4416 2022-10-14 17:08:50.000000 cloudflarepycli-1.7.0/src/cloudflarepycli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      397 2022-10-14 17:08:50.000000 cloudflarepycli-1.7.0/src/cloudflarepycli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-14 17:08:50.000000 cloudflarepycli-1.7.0/src/cloudflarepycli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2022-10-14 17:08:50.000000 cloudflarepycli-1.7.0/src/cloudflarepycli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2022-10-14 17:08:50.000000 cloudflarepycli-1.7.0/src/cloudflarepycli.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2022-10-14 17:08:50.000000 cloudflarepycli-1.7.0/src/cloudflarepycli.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-02 17:24:24.447970 cloudflarepycli-1.8/
+-rw-rw-rw-   0        0        0     4139 2023-07-02 17:24:24.447970 cloudflarepycli-1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3509 2023-07-01 22:20:08.000000 cloudflarepycli-1.8/README.md
+-rw-rw-rw-   0        0        0      135 2022-09-03 18:15:25.000000 cloudflarepycli-1.8/pyproject.toml
+-rw-rw-rw-   0        0        0      964 2023-07-02 17:24:24.450012 cloudflarepycli-1.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-02 17:24:24.405109 cloudflarepycli-1.8/src/
+drwxrwxrwx   0        0        0        0 2023-07-02 17:24:24.426012 cloudflarepycli-1.8/src/cloudflarepycli/
+-rw-rw-rw-   0        0        0        0 2022-09-03 18:15:25.000000 cloudflarepycli-1.8/src/cloudflarepycli/__init__.py
+-rw-rw-rw-   0        0        0     1521 2023-07-01 22:04:09.000000 cloudflarepycli-1.8/src/cloudflarepycli/__main__.py
+-rw-rw-rw-   0        0        0     8107 2023-07-01 22:06:17.000000 cloudflarepycli-1.8/src/cloudflarepycli/cloudflareclass.py
+drwxrwxrwx   0        0        0        0 2023-07-02 17:24:24.446970 cloudflarepycli-1.8/src/cloudflarepycli.egg-info/
+-rw-rw-rw-   0        0        0     4139 2023-07-02 17:24:24.000000 cloudflarepycli-1.8/src/cloudflarepycli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      397 2023-07-02 17:24:24.000000 cloudflarepycli-1.8/src/cloudflarepycli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 17:24:24.000000 cloudflarepycli-1.8/src/cloudflarepycli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-07-02 17:24:24.000000 cloudflarepycli-1.8/src/cloudflarepycli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2023-07-02 17:24:24.000000 cloudflarepycli-1.8/src/cloudflarepycli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-02 17:24:24.000000 cloudflarepycli-1.8/src/cloudflarepycli.egg-info/top_level.txt
```

### Comparing `cloudflarepycli-1.7.0/PKG-INFO` & `cloudflarepycli-1.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: cloudflarepycli
-Version: 1.7.0
-Summary: Python CLI and python class for retrieving user's realtime performance statistics
+Version: 1.8
+Summary: "Python CLI and python class for retrieving user's realtime performance statistics"
 Home-page: https://github.com/tevslin/cloudflarepycli
-Author: Tom Evslin
+Author: "Tom Evslin"
 Author-email: tevslin@gmail.com
 Project-URL: Bug Tracker, https://github.com/tevslin/cloudflarepycli/issues
 Keywords: speedtest,cloudflare,latency,jitter
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -19,15 +19,15 @@
 
 ## Purpose
 
 Retrieve near-term performance data about the service provided to a user by an ISP. The data includes up and download speeds, latency, and jitter. The CLI makes it possible to pipe the data to other processes for possible uploading, analysis etc. and/or to build a GUI for displaying current and past data. The cloudflareclass.py module is useful for varying the types of test that are done. I will use both in future projects to expand the functionality.
 
 ## Install
 
-Type 'pip install cloudflarepycli' in the Python environment you want to use. Note: code here is one version later than what's on PyPI. the pip installable version is still Windows only.
+For now, install from here. pypi version is not uptodate.
 
 ## CLI usage
 
 Type 'cfspeedtest' in the environment where you installed the package. Note that this is a shell command, not a Python command.
 
 ### Options
 
@@ -47,15 +47,15 @@
 
 https://github.com/tevslin/cloudflarepycli
 
 ## How it works
 
 Tests for latency are done by requesting one byte packets from Cloudflare, measuring the elapsed time to get a response, and subtracting the server processing time taken from the header in the returned message. Jitter is computed as the mean of the absolute difference between the arrival of consecutive requests.
 
-The cloudflareclass.py module makes Python requests to various subaddresses of [speed.cloudflare.com](https://speed.cloudflare.com). Their API is not documented, as far as I know, and so that is a vulnerability for this code. There is also a request to [ipdatabase.com](http://www.ipdatabase.com/ip) and the return is screen-scraped for the actual ISP name.
+The cloudflareclass.py module makes Python requests to various subaddresses of [speed.cloudflare.com](https://speed.cloudflare.com). Their API is not documented, as far as I know, and so that is a vulnerability for this code.
 
 Mirroring the performance of the Cloudflare webpage, the CLI does multiple uploads and downloads with different block sizes and the 90th percentile of all these tests is used for calculating up and download times. Results are similar to those obtained from the webpage. Tests can be varied using the cloudflareclass module.
 
 Unlike Ookla's speedtest CLI, Cloudflare does not require downloading a licensed exe. Cloudflare uses test sites from its own network of caching and hosting centers. This is useful because much of the content users would be retrieving is actually coming from these centers. On the other hand, coverage may be thin in some parts of the world.
 
 ## Privacy
 
@@ -65,12 +65,12 @@
 
 ## Background
 
 Billions of federal dollars are being disbursed to improve broadband availability and quality, especially in rural areas. Tools are needed to assure that ISPs deliver the quality they promise. This software is a pro bono contribution to getting those tools written. 
 
 ## Disclaimers
 
-No claims of any sort are made for this software. It has been tested on Windows 10 and 11, MacOS, and  Raspberry Pi OS and should work on other Linux versions but not tested. Use and/or redistribute solely at your own risk. No commitment is made to maintain this software. As noted above, changes made by Cloudflare or ipdatabase.com might break the functionality.
+No claims of any sort are made for this software. It has been tested on Windows 10 and 11, MacOS, and  Raspberry Pi OS and should work on other Linux versions but not tested. Use and/or redistribute solely at your own risk. No commitment is made to maintain this software. As noted above, changes made by Cloudflare might break the functionality.
 
 I have no affiliation with Cloudflare, any hosting service, or any ISP (except as a customer).
```

### Comparing `cloudflarepycli-1.7.0/README.md` & `cloudflarepycli-1.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 ## Purpose
 
 Retrieve near-term performance data about the service provided to a user by an ISP. The data includes up and download speeds, latency, and jitter. The CLI makes it possible to pipe the data to other processes for possible uploading, analysis etc. and/or to build a GUI for displaying current and past data. The cloudflareclass.py module is useful for varying the types of test that are done. I will use both in future projects to expand the functionality.
 
 ## Install
 
-Type 'pip install cloudflarepycli' in the Python environment you want to use. Note: code here is one version later than what's on PyPI. the pip installable version is still Windows only.
+For now, install from here. pypi version is not uptodate.
 
 ## CLI usage
 
 Type 'cfspeedtest' in the environment where you installed the package. Note that this is a shell command, not a Python command.
 
 ### Options
 
@@ -32,15 +32,15 @@
 
 https://github.com/tevslin/cloudflarepycli
 
 ## How it works
 
 Tests for latency are done by requesting one byte packets from Cloudflare, measuring the elapsed time to get a response, and subtracting the server processing time taken from the header in the returned message. Jitter is computed as the mean of the absolute difference between the arrival of consecutive requests.
 
-The cloudflareclass.py module makes Python requests to various subaddresses of [speed.cloudflare.com](https://speed.cloudflare.com). Their API is not documented, as far as I know, and so that is a vulnerability for this code. There is also a request to [ipdatabase.com](http://www.ipdatabase.com/ip) and the return is screen-scraped for the actual ISP name.
+The cloudflareclass.py module makes Python requests to various subaddresses of [speed.cloudflare.com](https://speed.cloudflare.com). Their API is not documented, as far as I know, and so that is a vulnerability for this code.
 
 Mirroring the performance of the Cloudflare webpage, the CLI does multiple uploads and downloads with different block sizes and the 90th percentile of all these tests is used for calculating up and download times. Results are similar to those obtained from the webpage. Tests can be varied using the cloudflareclass module.
 
 Unlike Ookla's speedtest CLI, Cloudflare does not require downloading a licensed exe. Cloudflare uses test sites from its own network of caching and hosting centers. This is useful because much of the content users would be retrieving is actually coming from these centers. On the other hand, coverage may be thin in some parts of the world.
 
 ## Privacy
 
@@ -50,12 +50,12 @@
 
 ## Background
 
 Billions of federal dollars are being disbursed to improve broadband availability and quality, especially in rural areas. Tools are needed to assure that ISPs deliver the quality they promise. This software is a pro bono contribution to getting those tools written. 
 
 ## Disclaimers
 
-No claims of any sort are made for this software. It has been tested on Windows 10 and 11, MacOS, and  Raspberry Pi OS and should work on other Linux versions but not tested. Use and/or redistribute solely at your own risk. No commitment is made to maintain this software. As noted above, changes made by Cloudflare or ipdatabase.com might break the functionality.
+No claims of any sort are made for this software. It has been tested on Windows 10 and 11, MacOS, and  Raspberry Pi OS and should work on other Linux versions but not tested. Use and/or redistribute solely at your own risk. No commitment is made to maintain this software. As noted above, changes made by Cloudflare might break the functionality.
 
 I have no affiliation with Cloudflare, any hosting service, or any ISP (except as a customer).
```

### Comparing `cloudflarepycli-1.7.0/setup.cfg` & `cloudflarepycli-1.8/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,61 +1,61 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 6c6f 7564 666c 6172 6570 7963   = cloudflarepyc
 00000020: 6c69 0d0a 7665 7273 696f 6e20 3d20 312e  li..version = 1.
-00000030: 372e 300d 0a61 7574 686f 7220 3d20 546f  7.0..author = To
-00000040: 6d20 4576 736c 696e 0d0a 6175 7468 6f72  m Evslin..author
+00000030: 380d 0a61 7574 686f 7220 3d20 2254 6f6d  8..author = "Tom
+00000040: 2045 7673 6c69 6e22 0d0a 6175 7468 6f72   Evslin"..author
 00000050: 5f65 6d61 696c 203d 2074 6576 736c 696e  _email = tevslin
 00000060: 4067 6d61 696c 2e63 6f6d 0d0a 6465 7363  @gmail.com..desc
-00000070: 7269 7074 696f 6e20 3d20 5079 7468 6f6e  ription = Python
-00000080: 2043 4c49 2061 6e64 2070 7974 686f 6e20   CLI and python 
-00000090: 636c 6173 7320 666f 7220 7265 7472 6965  class for retrie
-000000a0: 7669 6e67 2075 7365 7227 7320 7265 616c  ving user's real
-000000b0: 7469 6d65 2070 6572 666f 726d 616e 6365  time performance
-000000c0: 2073 7461 7469 7374 6963 730d 0a6c 6f6e   statistics..lon
-000000d0: 675f 6465 7363 7269 7074 696f 6e20 3d20  g_description = 
-000000e0: 6669 6c65 3a20 5245 4144 4d45 2e6d 640d  file: README.md.
-000000f0: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
-00000100: 6e5f 636f 6e74 656e 745f 7479 7065 203d  n_content_type =
-00000110: 2074 6578 742f 6d61 726b 646f 776e 0d0a   text/markdown..
-00000120: 7572 6c20 3d20 6874 7470 733a 2f2f 6769  url = https://gi
-00000130: 7468 7562 2e63 6f6d 2f74 6576 736c 696e  thub.com/tevslin
-00000140: 2f63 6c6f 7564 666c 6172 6570 7963 6c69  /cloudflarepycli
-00000150: 0d0a 7072 6f6a 6563 745f 7572 6c73 203d  ..project_urls =
-00000160: 200d 0a09 4275 6720 5472 6163 6b65 7220   ...Bug Tracker 
-00000170: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
-00000180: 2e63 6f6d 2f74 6576 736c 696e 2f63 6c6f  .com/tevslin/clo
-00000190: 7564 666c 6172 6570 7963 6c69 2f69 7373  udflarepycli/iss
-000001a0: 7565 730d 0a6c 6963 656e 7365 5f66 696c  ues..license_fil
-000001b0: 6573 203d 2066 696c 653a 4c69 6365 6e73  es = file:Licens
-000001c0: 650d 0a63 6c61 7373 6966 6965 7273 203d  e..classifiers =
-000001d0: 200d 0a09 5072 6f67 7261 6d6d 696e 6720   ...Programming 
-000001e0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-000001f0: 6f6e 203a 3a20 330d 0a09 4c69 6365 6e73  on :: 3...Licens
-00000200: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
-00000210: 6420 3a3a 2047 4e55 2047 656e 6572 616c  d :: GNU General
-00000220: 2050 7562 6c69 6320 4c69 6365 6e73 6520   Public License 
-00000230: 7633 2028 4750 4c76 3329 0d0a 094f 7065  v3 (GPLv3)...Ope
-00000240: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
-00000250: 204f 5320 496e 6465 7065 6e64 656e 740d   OS Independent.
-00000260: 0a6b 6579 776f 7264 7320 3d20 0d0a 0973  .keywords = ...s
-00000270: 7065 6564 7465 7374 0d0a 0963 6c6f 7564  peedtest...cloud
-00000280: 666c 6172 650d 0a09 6c61 7465 6e63 790d  flare...latency.
-00000290: 0a09 6a69 7474 6572 0d0a 0d0a 5b6f 7074  ..jitter....[opt
-000002a0: 696f 6e73 5d0d 0a70 6163 6b61 6765 5f64  ions]..package_d
-000002b0: 6972 203d 200d 0a09 3d20 7372 630d 0a70  ir = ...= src..p
-000002c0: 6163 6b61 6765 7320 3d20 6669 6e64 3a0d  ackages = find:.
-000002d0: 0a70 7974 686f 6e5f 7265 7175 6972 6573  .python_requires
-000002e0: 203d 203e 3d33 2e37 0d0a 696e 7374 616c   = >=3.7..instal
-000002f0: 6c5f 7265 7175 6972 6573 203d 200d 0a09  l_requires = ...
-00000300: 7265 7175 6573 7473 0d0a 096e 756d 7079  requests...numpy
-00000310: 0d0a 0d0a 5b6f 7074 696f 6e73 2e70 6163  ....[options.pac
-00000320: 6b61 6765 732e 6669 6e64 5d0d 0a77 6865  kages.find]..whe
-00000330: 7265 203d 2073 7263 0d0a 0d0a 5b6f 7074  re = src....[opt
-00000340: 696f 6e73 2e65 6e74 7279 5f70 6f69 6e74  ions.entry_point
-00000350: 735d 0d0a 636f 6e73 6f6c 655f 7363 7269  s]..console_scri
-00000360: 7074 7320 3d20 0d0a 0963 6673 7065 6564  pts = ...cfspeed
-00000370: 7465 7374 203d 2063 6c6f 7564 666c 6172  test = cloudflar
-00000380: 6570 7963 6c69 2e5f 5f6d 6169 6e5f 5f3a  epycli.__main__:
-00000390: 6d61 696e 0d0a 0d0a 5b65 6767 5f69 6e66  main....[egg_inf
-000003a0: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
-000003b0: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
-000003c0: 0d0a                                     ..
+00000070: 7269 7074 696f 6e20 3d20 2250 7974 686f  ription = "Pytho
+00000080: 6e20 434c 4920 616e 6420 7079 7468 6f6e  n CLI and python
+00000090: 2063 6c61 7373 2066 6f72 2072 6574 7269   class for retri
+000000a0: 6576 696e 6720 7573 6572 2773 2072 6561  eving user's rea
+000000b0: 6c74 696d 6520 7065 7266 6f72 6d61 6e63  ltime performanc
+000000c0: 6520 7374 6174 6973 7469 6373 220d 0a6c  e statistics"..l
+000000d0: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
+000000e0: 3d20 6669 6c65 3a20 5245 4144 4d45 2e6d  = file: README.m
+000000f0: 640d 0a6c 6f6e 675f 6465 7363 7269 7074  d..long_descript
+00000100: 696f 6e5f 636f 6e74 656e 745f 7479 7065  ion_content_type
+00000110: 203d 2074 6578 742f 6d61 726b 646f 776e   = text/markdown
+00000120: 0d0a 7572 6c20 3d20 6874 7470 733a 2f2f  ..url = https://
+00000130: 6769 7468 7562 2e63 6f6d 2f74 6576 736c  github.com/tevsl
+00000140: 696e 2f63 6c6f 7564 666c 6172 6570 7963  in/cloudflarepyc
+00000150: 6c69 0d0a 7072 6f6a 6563 745f 7572 6c73  li..project_urls
+00000160: 203d 200d 0a09 4275 6720 5472 6163 6b65   = ...Bug Tracke
+00000170: 7220 3d20 6874 7470 733a 2f2f 6769 7468  r = https://gith
+00000180: 7562 2e63 6f6d 2f74 6576 736c 696e 2f63  ub.com/tevslin/c
+00000190: 6c6f 7564 666c 6172 6570 7963 6c69 2f69  loudflarepycli/i
+000001a0: 7373 7565 730d 0a6c 6963 656e 7365 5f66  ssues..license_f
+000001b0: 696c 6573 203d 2066 696c 653a 4c69 6365  iles = file:Lice
+000001c0: 6e73 650d 0a63 6c61 7373 6966 6965 7273  nse..classifiers
+000001d0: 203d 200d 0a09 5072 6f67 7261 6d6d 696e   = ...Programmin
+000001e0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+000001f0: 7468 6f6e 203a 3a20 330d 0a09 4c69 6365  thon :: 3...Lice
+00000200: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
+00000210: 7665 6420 3a3a 2047 4e55 2047 656e 6572  ved :: GNU Gener
+00000220: 616c 2050 7562 6c69 6320 4c69 6365 6e73  al Public Licens
+00000230: 6520 7633 2028 4750 4c76 3329 0d0a 094f  e v3 (GPLv3)...O
+00000240: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
+00000250: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
+00000260: 740d 0a6b 6579 776f 7264 7320 3d20 0d0a  t..keywords = ..
+00000270: 0973 7065 6564 7465 7374 0d0a 0963 6c6f  .speedtest...clo
+00000280: 7564 666c 6172 650d 0a09 6c61 7465 6e63  udflare...latenc
+00000290: 790d 0a09 6a69 7474 6572 0d0a 0d0a 5b6f  y...jitter....[o
+000002a0: 7074 696f 6e73 5d0d 0a70 6163 6b61 6765  ptions]..package
+000002b0: 5f64 6972 203d 200d 0a09 3d20 7372 630d  _dir = ...= src.
+000002c0: 0a70 6163 6b61 6765 7320 3d20 6669 6e64  .packages = find
+000002d0: 3a0d 0a70 7974 686f 6e5f 7265 7175 6972  :..python_requir
+000002e0: 6573 203d 203e 3d33 2e37 0d0a 696e 7374  es = >=3.7..inst
+000002f0: 616c 6c5f 7265 7175 6972 6573 203d 200d  all_requires = .
+00000300: 0a09 7265 7175 6573 7473 0d0a 096e 756d  ..requests...num
+00000310: 7079 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  py....[options.p
+00000320: 6163 6b61 6765 732e 6669 6e64 5d0d 0a77  ackages.find]..w
+00000330: 6865 7265 203d 2073 7263 0d0a 0d0a 5b6f  here = src....[o
+00000340: 7074 696f 6e73 2e65 6e74 7279 5f70 6f69  ptions.entry_poi
+00000350: 6e74 735d 0d0a 636f 6e73 6f6c 655f 7363  nts]..console_sc
+00000360: 7269 7074 7320 3d20 0d0a 0963 6673 7065  ripts = ...cfspe
+00000370: 6564 7465 7374 203d 2063 6c6f 7564 666c  edtest = cloudfl
+00000380: 6172 6570 7963 6c69 2e5f 5f6d 6169 6e5f  arepycli.__main_
+00000390: 5f3a 6d61 696e 0d0a 0d0a 5b65 6767 5f69  _:main....[egg_i
+000003a0: 6e66 6f5d 0d0a 7461 675f 6275 696c 6420  nfo]..tag_build 
+000003b0: 3d20 0d0a 7461 675f 6461 7465 203d 2030  = ..tag_date = 0
+000003c0: 0d0a 0d0a                                ....
```

### Comparing `cloudflarepycli-1.7.0/src/cloudflarepycli/__main__.py` & `cloudflarepycli-1.8/src/cloudflarepycli/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -31,11 +31,16 @@
     parser.add_argument('--version',action='version',version='%(prog)s version '+str(version))
     args=parser.parse_args()
     
     thetester=cloudflareclass.cloudflare(debug=args.debug,printit=(not args.json)) #reopen with correct params
     thedict=thetester.runalltests()
     if args.json:
         print (json.dumps(thedict))
+        
+    #test deprecated rountines
+    print (thetester.getcolo())
+    print (thetester.getcolodetails(""))
+    print (thetester.getisp(""))
 
 if __name__=='__main__':
     main()
```

### Comparing `cloudflarepycli-1.7.0/src/cloudflarepycli/cloudflareclass.py` & `cloudflarepycli-1.8/src/cloudflarepycli/cloudflareclass.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,22 +21,28 @@
     if None, defaultuptests (see below) is used
     format is ((size, reps, label)......)
         size: size of block to upload
         reps: number of times to repeat test
         label: text label for test - also becomes key in the dict
 latencyreps: number of repetitions for latency test
 
+version 1.8.0
+removed dependency on ipdatabase.com
+added getfulldata to get all data about test locs and isp from cloudflare
+getcolo, getcolodetails, and getisp deprecated but left functional
+
+
 @author: /tevslin
 """
 
 class cloudflare:
     #tests changed 1/1/22 to mirror those done by web-based test
     uploadtests=((101000,8,'100kB'),(1001000, 6,'1MB'),(10001000, 4,'10MB'))
     downloadtests=((101000, 10,'100kB'),(1001000, 8,'1MB'),(10001000, 6,'10MB'),(25001000, 4,'25MB'))
-    version="1.7.0"
+    version="1.8.0" #7/1/23
     def __init__(self,thedict=None,debug=False,printit=True,downtests=None,uptests=None,latencyreps=20,timeout=(3.05,25)):
 
         import requests
         
         if debug:
             import logging
             
@@ -65,39 +71,37 @@
             self.downloadtests=downtests
         if not uptests is None:
             self.uploadtests=uptests
         self.mequests=requests.Session()
         self.timeout=timeout
 
     def getcolo(self):
-    # retrieves cloudflare colo and user ip address
-
-        r=self.mequests.get('http://speed.cloudflare.com/cdn-cgi/trace')       
-        dicty={}
-        for lines in r.text.splitlines():
-            words=lines.split("=")
-            dicty[words[0]]=words[1]
-        return dicty['colo'],dicty['ip']
+    # retrieves cloudflare colo, user ip address 
+    # deprecated but left for compatability
+        colo,ip,org,region,city=self.getfulldata()
+        return colo,ip
     
     def getisp(self,ip):
-        from bs4 import BeautifulSoup
-        import requests
-        
-        r=requests.get("http://www.ipdatabase.com/ip/"+ip)
-        soup = BeautifulSoup(r.content, 'html.parser')
-        first=soup.find(class_='table-head',string='Organization')
-        return(first.find_next_sibling().string)
-
+    # retrieves ISP
+    # deprecated but left for compatability
+        colo,ip,org,region,city=self.getfulldata()
+        return org
+    
     def getcolodetails(self,colo):
-        #retrieves colocation list for cloudflare
-        r=self.mequests.get('http://speed.cloudflare.com/locations')
-        for locs in r.json():
-            if locs['iata']==colo: #if match found
-                return(locs['region'],locs['city'])
-        return ("not found","not found")
+        #retrieves region and city for cf gateway
+        # deprecated but left for compatability
+        colo,ip,org,region,city=self.getfulldata()
+        return region,city
+
+    
+    def getfulldata(self):
+    # retrieves cloudflare colo, user ip address, ISP, city, and region
+        r=self.mequests.get('http://speed.cloudflare.com/meta')       
+        dicty=r.json()
+        return dicty['colo'],dicty['clientIp'],dicty['asOrganization'],dicty['region'],dicty['city']
 
     def download(self,numbytes,iterations):
         #runs download tests
         import os
         from contextlib import nullcontext
         import time
         if os.name == 'nt':
@@ -146,20 +150,18 @@
         self.thedict[label.replace(' ','_')]={"time":time.time(),"value":value} #add to dictionary
         
     def runalltests(self):
         #runs full suite of tests
         import numpy as np
         
         self.sprint('version',self.version)
-        colo,ip=self.getcolo() 
+        colo,ip,isp,region,city=self.getfulldata() 
         self.sprint('your ip',ip)
-        isp=self.getisp(ip)
         self.sprint('your ISP',isp)
         self.sprint('test location code',colo)
-        region,city=self.getcolodetails(colo)
         self.sprint ('test location city',city)
         self.sprint ('test location region',region)        
         fulltimes,servertimes,requesttimes=self.download(1,self.latencyreps) #measure latency and jitter
         latencies=np.subtract(requesttimes,servertimes)*1e3
         jitter=np.median([abs(latencies[i]-latencies[i-1]) for i in range(1,len(latencies))])
         self.sprint ('latency ms',round(np.median(latencies),2))
         self.sprint ('Jitter ms',round(jitter,2))
```

### Comparing `cloudflarepycli-1.7.0/src/cloudflarepycli.egg-info/PKG-INFO` & `cloudflarepycli-1.8/src/cloudflarepycli.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: cloudflarepycli
-Version: 1.7.0
-Summary: Python CLI and python class for retrieving user's realtime performance statistics
+Version: 1.8
+Summary: "Python CLI and python class for retrieving user's realtime performance statistics"
 Home-page: https://github.com/tevslin/cloudflarepycli
-Author: Tom Evslin
+Author: "Tom Evslin"
 Author-email: tevslin@gmail.com
 Project-URL: Bug Tracker, https://github.com/tevslin/cloudflarepycli/issues
 Keywords: speedtest,cloudflare,latency,jitter
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -19,15 +19,15 @@
 
 ## Purpose
 
 Retrieve near-term performance data about the service provided to a user by an ISP. The data includes up and download speeds, latency, and jitter. The CLI makes it possible to pipe the data to other processes for possible uploading, analysis etc. and/or to build a GUI for displaying current and past data. The cloudflareclass.py module is useful for varying the types of test that are done. I will use both in future projects to expand the functionality.
 
 ## Install
 
-Type 'pip install cloudflarepycli' in the Python environment you want to use. Note: code here is one version later than what's on PyPI. the pip installable version is still Windows only.
+For now, install from here. pypi version is not uptodate.
 
 ## CLI usage
 
 Type 'cfspeedtest' in the environment where you installed the package. Note that this is a shell command, not a Python command.
 
 ### Options
 
@@ -47,15 +47,15 @@
 
 https://github.com/tevslin/cloudflarepycli
 
 ## How it works
 
 Tests for latency are done by requesting one byte packets from Cloudflare, measuring the elapsed time to get a response, and subtracting the server processing time taken from the header in the returned message. Jitter is computed as the mean of the absolute difference between the arrival of consecutive requests.
 
-The cloudflareclass.py module makes Python requests to various subaddresses of [speed.cloudflare.com](https://speed.cloudflare.com). Their API is not documented, as far as I know, and so that is a vulnerability for this code. There is also a request to [ipdatabase.com](http://www.ipdatabase.com/ip) and the return is screen-scraped for the actual ISP name.
+The cloudflareclass.py module makes Python requests to various subaddresses of [speed.cloudflare.com](https://speed.cloudflare.com). Their API is not documented, as far as I know, and so that is a vulnerability for this code.
 
 Mirroring the performance of the Cloudflare webpage, the CLI does multiple uploads and downloads with different block sizes and the 90th percentile of all these tests is used for calculating up and download times. Results are similar to those obtained from the webpage. Tests can be varied using the cloudflareclass module.
 
 Unlike Ookla's speedtest CLI, Cloudflare does not require downloading a licensed exe. Cloudflare uses test sites from its own network of caching and hosting centers. This is useful because much of the content users would be retrieving is actually coming from these centers. On the other hand, coverage may be thin in some parts of the world.
 
 ## Privacy
 
@@ -65,12 +65,12 @@
 
 ## Background
 
 Billions of federal dollars are being disbursed to improve broadband availability and quality, especially in rural areas. Tools are needed to assure that ISPs deliver the quality they promise. This software is a pro bono contribution to getting those tools written. 
 
 ## Disclaimers
 
-No claims of any sort are made for this software. It has been tested on Windows 10 and 11, MacOS, and  Raspberry Pi OS and should work on other Linux versions but not tested. Use and/or redistribute solely at your own risk. No commitment is made to maintain this software. As noted above, changes made by Cloudflare or ipdatabase.com might break the functionality.
+No claims of any sort are made for this software. It has been tested on Windows 10 and 11, MacOS, and  Raspberry Pi OS and should work on other Linux versions but not tested. Use and/or redistribute solely at your own risk. No commitment is made to maintain this software. As noted above, changes made by Cloudflare might break the functionality.
 
 I have no affiliation with Cloudflare, any hosting service, or any ISP (except as a customer).
```

