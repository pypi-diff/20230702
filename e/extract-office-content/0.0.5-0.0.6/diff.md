# Comparing `tmp/extract_office_content-0.0.5-py3-none-any.whl.zip` & `tmp/extract_office_content-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 10700 bytes, number of entries: 11
--rw-r--r--  2.0 unx      227 b- defN 23-Jul-02 09:11 extract_office_content/__init__.py
--rw-r--r--  2.0 unx     4444 b- defN 23-Jul-02 09:11 extract_office_content/extract_excel.py
--rw-r--r--  2.0 unx     4174 b- defN 23-Jul-02 09:11 extract_office_content/extract_ppt.py
--rw-r--r--  2.0 unx     6505 b- defN 23-Jul-02 09:11 extract_office_content/extract_word.py
--rw-r--r--  2.0 unx     2275 b- defN 23-Jul-02 09:11 extract_office_content/main.py
--rw-r--r--  2.0 unx      969 b- defN 23-Jul-02 09:11 extract_office_content/utils.py
--rw-r--r--  2.0 unx     5315 b- defN 23-Jul-02 09:12 extract_office_content-0.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-02 09:12 extract_office_content-0.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx      245 b- defN 23-Jul-02 09:12 extract_office_content-0.0.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       23 b- defN 23-Jul-02 09:12 extract_office_content-0.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1018 b- defN 23-Jul-02 09:12 extract_office_content-0.0.5.dist-info/RECORD
-11 files, 25287 bytes uncompressed, 8938 bytes compressed:  64.7%
+Zip file size: 10734 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      227 b- defN 23-Jul-02 10:31 extract_office_content/__init__.py
+-rw-r--r--  2.0 unx     4444 b- defN 23-Jul-02 10:31 extract_office_content/extract_excel.py
+-rw-r--r--  2.0 unx     4174 b- defN 23-Jul-02 10:31 extract_office_content/extract_ppt.py
+-rw-r--r--  2.0 unx     6717 b- defN 23-Jul-02 10:31 extract_office_content/extract_word.py
+-rw-r--r--  2.0 unx     2275 b- defN 23-Jul-02 10:31 extract_office_content/main.py
+-rw-r--r--  2.0 unx      969 b- defN 23-Jul-02 10:31 extract_office_content/utils.py
+-rw-r--r--  2.0 unx     5315 b- defN 23-Jul-02 10:31 extract_office_content-0.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-02 10:31 extract_office_content-0.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx      245 b- defN 23-Jul-02 10:31 extract_office_content-0.0.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       23 b- defN 23-Jul-02 10:31 extract_office_content-0.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1018 b- defN 23-Jul-02 10:31 extract_office_content-0.0.6.dist-info/RECORD
+11 files, 25499 bytes uncompressed, 8972 bytes compressed:  64.8%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: extract_office_content/main.py
 Comment: 
 
 Filename: extract_office_content/utils.py
 Comment: 
 
-Filename: extract_office_content-0.0.5.dist-info/METADATA
+Filename: extract_office_content-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: extract_office_content-0.0.5.dist-info/WHEEL
+Filename: extract_office_content-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: extract_office_content-0.0.5.dist-info/entry_points.txt
+Filename: extract_office_content-0.0.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: extract_office_content-0.0.5.dist-info/top_level.txt
+Filename: extract_office_content-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: extract_office_content-0.0.5.dist-info/RECORD
+Filename: extract_office_content-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## extract_office_content/extract_word.py

```diff
@@ -1,16 +1,16 @@
 #! /usr/bin/env python
 # Modified from https://github.com/ankushshah89/python-docx2txt
-from io import BytesIO
 import argparse
 import re
 import xml.etree.ElementTree as ET
 import zipfile
+from io import BytesIO
 from pathlib import Path
-from typing import Union
+from typing import List, Union
 
 import docx
 import lxml.etree as etree
 import pandas as pd
 from docx.document import Document
 from docx.oxml.table import CT_Tbl
 from docx.table import Table, _Cell
@@ -25,22 +25,23 @@
         self.img_suffix = [".jpg", ".jpeg", ".png", ".bmp"]
         self.nsmap = {
             "w": "http://schemas.openxmlformats.org/wordprocessingml/2006/main"
         }
         self.extract_table = ExtractWordTable()
         self.parser = etree.XMLParser()
 
-    def __call__(self, docx_content: Union[str, bytes], save_img_dir=None):
+    def __call__(self, docx_content: Union[str, bytes], save_img_dir=None) -> List:
         if isinstance(docx_content, str) and not Path(docx_content).exists():
             raise FileNotFoundError(f"{docx_content} does not exist.")
         elif isinstance(docx_content, bytes):
             docx_content = BytesIO(docx_content)
 
         self.table_content = self.extract_table(docx_content)
-        text = ""
+
+        text = []
 
         # unzip the docx_content in memory
         zipf = zipfile.ZipFile(docx_content)
         filelist = zipf.namelist()
 
         header_files, footer_files, img_files = [], [], []
         header_xmls = "word/header[0-9]*.xml"
@@ -55,34 +56,41 @@
                 img_files.append(fname)
             else:
                 continue
 
         # get header text
         # there can be 3 header files in the zip
         header_text = [self.xml2text(zipf.read(path)) for path in header_files]
-        text += "".join(header_text)
+        if header_text:
+            header_text = "".join(header_text).strip()
+            text.append(header_text)
 
         # get main text
         doc_xml = "word/document.xml"
         main_txt = self.xml2text(zipf.read(doc_xml))
-        text += main_txt
+        if main_txt:
+            text.append(main_txt.strip())
 
         # get footer text
         # there can be 3 footer files in the zip
         footer_text = [self.xml2text(zipf.read(path)) for path in footer_files]
-        text += "".join(footer_text)
+        if footer_text:
+            footer_text = "".join(footer_text).strip()
+            text.append(footer_text)
 
         if save_img_dir:
             mkdir(save_img_dir)
             for img_path in img_files:
                 dst_fname = Path(save_img_dir) / Path(img_path).name
                 with open(dst_fname, "wb") as dst_f:
                     dst_f.write(zipf.read(img_path))
         zipf.close()
-        return text.strip() + "\n".join(self.table_content)
+
+        text.extend(self.table_content)
+        return text
 
     def qn(self, tag):
         """
         Stands for 'qualified name', a utility function to turn a namespace
         prefixed tag name into a Clark-notation qualified tag name for lxml. For
         example, ``qn('p:cSld')`` returns ``'{http://schemas.../main}cSld'``.
         Source: https://github.com/python-openxml/python-docx/
```

## Comparing `extract_office_content-0.0.5.dist-info/METADATA` & `extract_office_content-0.0.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extract-office-content
-Version: 0.0.5
+Version: 0.0.6
 Summary: Tool for extracting content from office files.
 Home-page: https://github.com/SWHL/ExtractOfficeText.git
 Author: SWHL
 Author-email: liekkaskono@163.com
 License: Apache-2.0
 Keywords: extract,office,text,content
 Platform: Any
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: extract-office-content Version: 0.0.5 Summary: Tool
+Metadata-Version: 2.1 Name: extract-office-content Version: 0.0.6 Summary: Tool
 for extracting content from office files. Home-page: https://github.com/SWHL/
 ExtractOfficeText.git Author: SWHL Author-email: liekkaskono@163.com License:
 Apache-2.0 Keywords: extract,office,text,content Platform: Any Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Python: >=3.6,<=3.11 Description-Content-Type: text/
```

## Comparing `extract_office_content-0.0.5.dist-info/RECORD` & `extract_office_content-0.0.6.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 extract_office_content/__init__.py,sha256=Ge-pxaPmMXWiBzju-OCsdUwYXM8GLvY56qktBKTO3Xw,227
 extract_office_content/extract_excel.py,sha256=OpaS3EewiWwSJTrpwZVk9sVRgA8nMU51LnJjt3EI3kk,4444
 extract_office_content/extract_ppt.py,sha256=wmQzIgvCFK4N1fOhEv3LKzfZ86zqdp_KNMYUfYjxb2U,4174
-extract_office_content/extract_word.py,sha256=hmqO5ALqFwG2v4QdFrPEF_75cw3B_iShxqGdNmUZlyA,6505
+extract_office_content/extract_word.py,sha256=q_mNYLnfQNIT9LGvKhFU-iwn1HYjEhW2xe5Pl5hpdBE,6717
 extract_office_content/main.py,sha256=gcmeuhNQsZvNYfWOB-9nxxenQzkMyl_Wnr2UoyD8s3U,2275
 extract_office_content/utils.py,sha256=qPiuHyITVAScykQOrXEQz7U8W8OvwRdZhN-m5gyf7VU,969
-extract_office_content-0.0.5.dist-info/METADATA,sha256=q8nmOdmiWFSDx4qvuwAqQ4lFrbxntJ6DBURtWH1FxRk,5315
-extract_office_content-0.0.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-extract_office_content-0.0.5.dist-info/entry_points.txt,sha256=JXiZmmPdeFuKjf78O0nnnTigzul8d99FV6YuamdcI6Y,245
-extract_office_content-0.0.5.dist-info/top_level.txt,sha256=quDoGD7DEfkl_J2tdoeRUbk5H4oKd5-dWIOLRaLB_mc,23
-extract_office_content-0.0.5.dist-info/RECORD,,
+extract_office_content-0.0.6.dist-info/METADATA,sha256=qmYJjJ99ygwyjwpNUWsoiZZcjHQZ0OgcpDQC3y6J5F0,5315
+extract_office_content-0.0.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+extract_office_content-0.0.6.dist-info/entry_points.txt,sha256=JXiZmmPdeFuKjf78O0nnnTigzul8d99FV6YuamdcI6Y,245
+extract_office_content-0.0.6.dist-info/top_level.txt,sha256=quDoGD7DEfkl_J2tdoeRUbk5H4oKd5-dWIOLRaLB_mc,23
+extract_office_content-0.0.6.dist-info/RECORD,,
```

