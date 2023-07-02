# Comparing `tmp/epos_print_xml-0.1.tar.gz` & `tmp/epos_print_xml-0.2.tar.gz`

## Comparing `epos_print_xml-0.1.tar` & `epos_print_xml-0.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 epos_print_xml-0.1/src/test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 epos_print_xml-0.1/src/epos/__init__.py
--rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 epos_print_xml-0.1/src/epos/attributes.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 epos_print_xml-0.1/src/epos/constants.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 epos_print_xml-0.1/src/epos/document.py
--rw-r--r--   0        0        0    17159 2020-02-02 00:00:00.000000 epos_print_xml-0.1/src/epos/elements.py
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 epos_print_xml-0.1/src/epos/printer.py
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 epos_print_xml-0.1/src/epos/status.py
--rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 epos_print_xml-0.1/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 epos_print_xml-0.1/LICENSE
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 epos_print_xml-0.1/README.md
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 epos_print_xml-0.1/pyproject.toml
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 epos_print_xml-0.1/PKG-INFO
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 epos_print_xml-0.2/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 epos_print_xml-0.2/src/test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 epos_print_xml-0.2/src/epos/__init__.py
+-rw-r--r--   0        0        0     4084 2020-02-02 00:00:00.000000 epos_print_xml-0.2/src/epos/attributes.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 epos_print_xml-0.2/src/epos/constants.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 epos_print_xml-0.2/src/epos/document.py
+-rw-r--r--   0        0        0    17239 2020-02-02 00:00:00.000000 epos_print_xml-0.2/src/epos/elements.py
+-rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 epos_print_xml-0.2/src/epos/printer.py
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 epos_print_xml-0.2/src/epos/status.py
+-rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 epos_print_xml-0.2/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 epos_print_xml-0.2/LICENSE
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 epos_print_xml-0.2/README.md
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 epos_print_xml-0.2/pyproject.toml
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 epos_print_xml-0.2/PKG-INFO
```

### Comparing `epos_print_xml-0.1/src/test.py` & `epos_print_xml-0.2/src/test.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 from epos.elements import Text, Feed, Barcode
 from epos.constants import Align, BarcodeType, HRI
 
 # Create a new printer object with 10.0.0.10 as ip
 printer = Printer('10.0.0.10')
 # Check if we can connect to the printer with no errors, otherwise exit
 if not printer.try_connection():
-    exit()
-print('Connection with printer established.')
+    print("Printer error!")
+else:
+    print('Connection with printer established.')
 
 # Create a new EposDocument object
 # This will contain all the individual elements
 doc = EposDocument()
 
 # Add an element directly to the body of the document
 doc.add_body(Text('This is example text!\n'))
@@ -28,15 +29,15 @@
 
 # Rotated text
 t = Text('This text is rotated\n')
 t.rotate = True
 doc.add_body(t)
 
 # Find max length in double mode
-t = Text("|"*25)
+t = Text("-"*24)
 t.double_width = True
 t.double_height = True
 t.rotate = False
 t.reverse = True
 t.align = Align.LEFT
 t.bold = False
 doc.add_body(t)
@@ -46,8 +47,9 @@
 
 # Add a barcode
 doc.add_body(Barcode(BarcodeType.CODE39, '01234567890', align=Align.LEFT, width=2, height=64, hri=HRI.BELOW))
 
 # Send the whole document to the printer
 # This will automatially send a Cut at the end of the document body
 r = printer.print(doc)
-print(r)
+print(r)
+print('\n'.join(r.status_msg()))
```

### Comparing `epos_print_xml-0.1/src/epos/attributes.py` & `epos_print_xml-0.2/src/epos/attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,16 +83,15 @@
     def font(self, font: Font):
         try:
             font = Font(font)
         except ValueError:
             pass
 
         if font is not None and font not in Font:
-            raise ValueError(
-                f'"font" must be valid.')
+            raise ValueError('"font" must be valid.')
         self._font = font
 
 
 class LineSpcAtt:
     def __init__(self, linespc, min_linespc=0, max_linespc=255, **kwargs):
         super().__init__(**kwargs)
         self._min_linespc = min_linespc
```

### Comparing `epos_print_xml-0.1/src/epos/constants.py` & `epos_print_xml-0.2/src/epos/constants.py`

 * *Files identical despite different names*

### Comparing `epos_print_xml-0.1/src/epos/document.py` & `epos_print_xml-0.2/src/epos/document.py`

 * *Files identical despite different names*

### Comparing `epos_print_xml-0.1/src/epos/elements.py` & `epos_print_xml-0.2/src/epos/elements.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import List
 from dataclasses import dataclass
 
 from . import status
 from .attributes import AlignAtt, ColorAtt, WidthAtt, HeightAtt, FontAtt, RotateAtt, LineSpcAtt
 from .constants import Color, Align, Mode, BarcodeType, HRI, Font, CutType, Lang
 
+
 @dataclass
 class BaseElement:
     """
     Base class for all ePOS-Print XML elements
     """
     tag: str
     text: str
@@ -40,20 +41,14 @@
         element.text = self.text
         element.tail = self.tail
         return element
 
     def to_str(self):
         return ET.tostring(self.to_xml(), encoding='utf-8', )
 
-    def from_xml(self, xml: str):
-        """
-        Loads xml data
-        """
-        dom = ET.fromstring(xml)
-
     def _add_ns(self, tag: str) -> str:
         r = f'{{{self.namespaces["a"]}}}{tag}'
         # print(r)
         return r
 
     def _load_attrs(self):
         """To be overwritten by element class"""
@@ -62,31 +57,39 @@
 
 class Response(BaseElement):
     """
     This is an XML document that is sent back from a printer to an application.
     Reference:
     https://reference.epson-biz.com/modules/ref_epos_print_xml_en/index.php?vid=ref_epos_print_xml_en_xmlforcontrollingprinter_response
     """
-    def __init__(self, success=True):
+    def __init__(
+            self,
+            success: bool = True,
+            code: str = '',
+            status: int = 0,
+            battery: int = 0,
+    ):
         super().__init__('response')
 
         self.success = success
-        self.code = ''
-        self.status = 0
-        self.battery = 0
+        self.code = code
+        self.status = status
+        self.battery = battery
+
+    def __repr__(self):
+        return f'Success: {self.success}, Code: {repr(self.code)}, Status: {self.status}, Battery: {self.battery}'
 
     def _load_attrs(self):
         self.attr['xmlns'] = self.namespaces['epos-print']
         self.attr['success'] = str(self.success).lower()
-        if self.code:
-            self.attr['code'] = self.code
-        self.attr['status'] = str(self.status)
-        self.attr['battery'] = str(self.battery)
+        self.attr['code'] = self.code
+        self.attr['status'] = self.status
+        self.attr['battery'] = self.battery
 
-    def get_status(self) -> List[str]:
+    def status_msg(self) -> List[str]:
         return status.parse_code(self.status)
 
 
 class Text(BaseElement, FontAtt, WidthAtt, HeightAtt, AlignAtt, LineSpcAtt, RotateAtt, ColorAtt):
     def __init__(
             self,
             text: str = '',
@@ -170,15 +173,15 @@
     def smooth(self, smooth: bool):
         if smooth == 'true':
             self._smooth = True
         elif smooth == 'false':
             self._smooth = False
         else:
             self._smooth = smooth
-    
+
     @property
     def double_width(self) -> bool:
         return self._double_width
 
     @double_width.setter
     def double_width(self, double_width: bool):
         if double_width == 'true':
@@ -191,15 +194,15 @@
     @property
     def dw(self):
         return self.double_width
 
     @dw.setter
     def dw(self, dw):
         self.double_width = dw
-    
+
     @property
     def double_height(self) -> bool:
         return self._double_height
 
     @double_height.setter
     def double_height(self, double_height: bool):
         if double_height == 'true':
@@ -212,15 +215,15 @@
     @property
     def dh(self):
         return self.double_height
 
     @dh.setter
     def dh(self, dh):
         self.double_height = dh
-    
+
     @property
     def reverse(self) -> bool:
         return self._reverse
 
     @reverse.setter
     def reverse(self, reverse: bool):
         if reverse == 'true':
@@ -238,23 +241,23 @@
     def underline(self, underline: bool):
         if underline == 'true':
             self._underline = True
         elif underline == 'false':
             self._underline = False
         else:
             self._underline = underline
-    
+
     @property
     def ul(self):
         return self.underline
-    
+
     @ul.setter
     def ul(self, ul):
         self.underline = ul
-    
+
     @property
     def bold(self) -> bool:
         return self._bold
 
     @bold.setter
     def bold(self, bold: bool|str):
         if bold == 'true':
@@ -267,26 +270,26 @@
     @property
     def em(self):
         return self.bold
 
     @em.setter
     def em(self, em):
         self.bold = em
-    
+
     @property
     def x(self) -> int:
         return self._x
 
     @x.setter
     def x(self, x: int):
         try:
             x = int(x)
         except TypeError:
             pass
-        
+
         if x is not None and (x < 0 or x > 576):
             raise ValueError('"x" must be between 0 and 576 inclusive') from None
         self._x = x
 
     @property
     def y(self) -> int:
         return self._y
@@ -407,19 +410,19 @@
         self.key1 = key1
         self.key2 = key2
 
     def _load_attrs(self):
         self.attr['key1'] = str(self.key1)
         self.attr['key2'] = str(self.key2)
         self.attr['align'] = self.align
-    
+
     @property
     def key1(self) -> int:
         return self._key1
-    
+
     @key1.setter
     def key1(self, key1: int):
         try:
             key1 = int(key1)
         except TypeError:
             pass
 
@@ -570,15 +573,15 @@
 class Cut(BaseElement):
     def __init__(self, type: CutType = None):
         super().__init__('cut')
         self.type = type
 
     def _load_attrs(self):
         self.attr['type'] = self.type
-        
+
     @property
     def type(self) -> CutType:
         return self._type
 
     @type.setter
     def type(self, type: CutType):
         try:
```

### Comparing `epos_print_xml-0.1/src/epos/printer.py` & `epos_print_xml-0.2/src/epos/printer.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,63 +1,88 @@
+import xml.etree.ElementTree as ET
+
 import requests
 
-from .constants import BarcodeType
 from .document import EposDocument
-from .elements import Text, Feed, Cut, Barcode
+from .elements import Cut, Response
+
 
+namespaces = {
+    's': 'http://schemas.xmlsoap.org/soap/envelope/',
+    'epos-print': 'http://www.epson-pos.com/schemas/2011/03/epos-print',
+}
 
 class Printer:
     def __init__(self, ip):
         self.ip = ip
 
         # Defaults, normally not changed
         self.use_https = False
         self.devid = 'local_printer'
         self.timeout = 5000
         self.url = '/cgi-bin/epos/service.cgi'
 
     def try_connection(self):
-        """Send empty page and check the status"""
+        """Send empty page to check the status"""
         doc = EposDocument()
-        resp = self._send_printjob(doc.body_to_str())
-        return 'success="true' in resp
+        resp = self.print(doc, autocut=False)
+        return resp.success
 
-    def print(self, doc: EposDocument, autocut=True):
+    def print(self, doc: EposDocument, autocut=True) -> Response:
         if autocut:
             doc.add_body(Cut())
-        resp = self._send_printjob(doc.body_to_str())
-        return resp
+        r = self._send_printjob(doc.body_to_str())
+
+        response = Response(success=False)
+
+        xml_dom = ET.fromstring(r)
+        body = xml_dom.find('./s:Body', namespaces)
+        if not body:
+            response.code = 'NO_BODY_FOUND'
+            return response
+
+        for element in body:
+            if 'response' in element.tag:
+                attr = element.attrib
+                break
+        else:
+            response.code = 'NO_RESPONSE_FOUND'
+            return response
+
+        response.success = attr['success'] == 'true'
+        response.code = attr['code']
+        response.status = int(attr['status'])
+        response.battery = int(attr['battery'])
+
+        return response
 
     def _send_printjob(self, data):
         prefix = 'https://' if self.use_https else 'http://'
         url = prefix + self.ip + self.url
         headers = {
             'content-type': 'text/xml; charset=utf-8',
             'If-Modified-Since': 'Thu, 01 Jan 1970 00:00:00 GMT',
             'SOAPAction': '""',
         }
         params = {'devid': self.devid, 'timeout': self.timeout}
 
-        #print(data)
-
         response = requests.post(
             url,
             data=_add_soap_enveloppe(data),
             headers=headers,
             params=params,
         )
 
         return response.text
 
 
 def _add_soap_enveloppe(body: str, header: str = '') -> str:
     """Add the soap enveloppe, header and body"""
-    soap = []
+    soap = [f'<s:Envelope xmlns:s="{namespaces["s"]}">']
 
-    soap.append('<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">')
     if header:
         soap.append('<s:Header>')
         soap.append(header)
         soap.append('/<s:Header>')
     soap.append('<s:Body>')
     soap.append(body)
     soap.append('</s:Body>')
```

### Comparing `epos_print_xml-0.1/src/epos/status.py` & `epos_print_xml-0.2/src/epos/status.py`

 * *Files identical despite different names*

### Comparing `epos_print_xml-0.1/.gitignore` & `epos_print_xml-0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `epos_print_xml-0.1/LICENSE` & `epos_print_xml-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `epos_print_xml-0.1/README.md` & `epos_print_xml-0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 # py-epos-print-xml
 Python library to communicate with Epson thermal printers via ePos-Print XML.
 This makes it easy and intuitive to create print orders for ePos-Print XML compatible printers, like the Epson TM-T20, TM-m30 and TM-m50 series.
 Depending on the printer model, some elements are not supported. Check your manual or the [Epson reference](https://reference.epson-biz.com/modules/ref_epos_print_xml_en/index.php?vid=ref_epos_print_xml_en_devicespecifications_supportedelementslist) to see which elements are supported.
 
 This is still in active development, don't expect everything to work.
 
+## Instaling
+```
+pip install ePos-Print-XML
+```
+
 ## Example
 
 ```python
 from epos.printer import Printer
 from epos.document import EposDocument
 from epos.elements import Text, Feed, Barcode
 from epos.constants import Align
@@ -37,13 +42,20 @@
 doc.add_body(Feed(2))
 
 # Add a barcode
 doc.add_body(Barcode(BarcodeType.CODE39, 'text in barcode'))
 
 # Send the whole document to the printer
 # This will automatially send a Cut at the end of the document body
-printer.print(doc) 
+r = printer.print(doc)
+
+# The print method returns a response element
+# Here we can check if the printing was succesfull
+if r.success:
+    print('The printing was successfull!')
+else:
+    print(f'Printing failed. Error: {r.code}')
 ```
 
 
 ## Documentation
 Tech reference of all the xml elements by Epson: https://reference.epson-biz.com/modules/ref_epos_print_xml_en/index.php?content_id=1
```

### Comparing `epos_print_xml-0.1/pyproject.toml` & `epos_print_xml-0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "ePos-Print-XML"
-version = "0.1"
+version = "0.2"
 dependencies = [
   'requests',
 ]
 authors = [
   { name="Merten Fermont" },
 ]
 description = "Library to communicate with Epson thermal printers via ePOS-Print XML protocol"
```

### Comparing `epos_print_xml-0.1/PKG-INFO` & `epos_print_xml-0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ePos-Print-XML
-Version: 0.1
+Version: 0.2
 Summary: Library to communicate with Epson thermal printers via ePOS-Print XML protocol
 Project-URL: Homepage, https://github.com/MertenF/epos-print-xml
 Project-URL: Bug Tracker, https://github.com/MertenF/epos-print-xml/issues
 Author: Merten Fermont
 License-File: LICENSE
 Keywords: epos,printing,receipt,thermoprinter,voucher printer
 Classifier: License :: OSI Approved :: MIT License
@@ -19,14 +19,19 @@
 # py-epos-print-xml
 Python library to communicate with Epson thermal printers via ePos-Print XML.
 This makes it easy and intuitive to create print orders for ePos-Print XML compatible printers, like the Epson TM-T20, TM-m30 and TM-m50 series.
 Depending on the printer model, some elements are not supported. Check your manual or the [Epson reference](https://reference.epson-biz.com/modules/ref_epos_print_xml_en/index.php?vid=ref_epos_print_xml_en_devicespecifications_supportedelementslist) to see which elements are supported.
 
 This is still in active development, don't expect everything to work.
 
+## Instaling
+```
+pip install ePos-Print-XML
+```
+
 ## Example
 
 ```python
 from epos.printer import Printer
 from epos.document import EposDocument
 from epos.elements import Text, Feed, Barcode
 from epos.constants import Align
@@ -55,13 +60,20 @@
 doc.add_body(Feed(2))
 
 # Add a barcode
 doc.add_body(Barcode(BarcodeType.CODE39, 'text in barcode'))
 
 # Send the whole document to the printer
 # This will automatially send a Cut at the end of the document body
-printer.print(doc) 
+r = printer.print(doc)
+
+# The print method returns a response element
+# Here we can check if the printing was succesfull
+if r.success:
+    print('The printing was successfull!')
+else:
+    print(f'Printing failed. Error: {r.code}')
 ```
 
 
 ## Documentation
 Tech reference of all the xml elements by Epson: https://reference.epson-biz.com/modules/ref_epos_print_xml_en/index.php?content_id=1
```

