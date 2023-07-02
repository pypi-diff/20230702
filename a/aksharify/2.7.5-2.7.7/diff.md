# Comparing `tmp/aksharify-2.7.5.tar.gz` & `tmp/aksharify-2.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aksharify-2.7.5.tar", max compression
+gzip compressed data, was "aksharify-2.7.7.tar", max compression
```

## Comparing `aksharify-2.7.5.tar` & `aksharify-2.7.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       24 2023-05-29 15:23:03.528860 aksharify-2.7.5/aksharify/__init__.py
--rw-r--r--   0        0        0     7763 2023-06-01 02:42:15.057908 aksharify-2.7.5/aksharify/aksharify.py
--rw-r--r--   0        0        0      923 2023-06-01 11:44:58.412316 aksharify-2.7.5/pyproject.toml
--rw-r--r--   0        0        0     5864 2023-05-30 14:27:02.119233 aksharify-2.7.5/README.md
--rw-r--r--   0        0        0     6660 1970-01-01 00:00:00.000000 aksharify-2.7.5/PKG-INFO
+-rw-r--r--   0        0        0       24 2023-05-29 15:23:03.528860 aksharify-2.7.7/aksharify/__init__.py
+-rw-r--r--   0        0        0     8331 2023-06-02 07:36:07.914735 aksharify-2.7.7/aksharify/aksharify.py
+-rw-r--r--   0        0        0      923 2023-06-02 08:04:11.436522 aksharify-2.7.7/pyproject.toml
+-rw-r--r--   0        0        0     5864 2023-05-30 14:27:02.119233 aksharify-2.7.7/README.md
+-rw-r--r--   0        0        0     6660 1970-01-01 00:00:00.000000 aksharify-2.7.7/PKG-INFO
```

### Comparing `aksharify-2.7.5/aksharify/aksharify.py` & `aksharify-2.7.7/aksharify/aksharify.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from io import BytesIO
 
 
 SVG_HEADER = '<?xml version="1.0" standalone="no"?><svg width="{}" height="{}" version="1.1" xmlns="http://www.w3.org/2000/svg" style="font-family: {}; font-size:{};"><desc>Aksharify Art</desc><rect width="100%" height="100%" fill="{}"/>'
 HTML_HEADER = '<!DOCTYPE html><html lang="en"><head><meta charset="UTF-8"><meta name="viewport" content="width=device-width, initial-scale=1.0"><title>Aksharify Art</title></head><body><a href="https://primepatel.github.io/aksharify-docs/">{}</a></body></html>'
 SORTEDCHARS = """ `.-_',~:*;!"^/\+><r=?()|7LxtcYivTljsz[]1Jnufy{}oI#FC4VX2ehk3aZw5ASbdpqUP6%9G8mKO&0EDHg$MWRNQB@"""
 
-def URLtoImg(url):
+def URLtoImg(url: str) -> Image:
     response = requests.get(url)
     image_data = response.content
     try:
         Image.open(BytesIO(image_data))
         return BytesIO(image_data)
     except:
         print("The provided URL does not correspond to an image.")
@@ -25,78 +25,81 @@
         self.image = Image.open(image)
         self.w, self.h = self.image.size
         self.chars = list(set(chars))
         self.CH_CONSTANT = 2.143
         self.H_dis, self.V_dis = 5.55, 10
         self.font_size = 10
     
-    def set_font_size(self, size):
+    def set_font_size(self, size: int) -> None:
         self.H_dis = (size*555)/1000
         self.V_dis = size
         self.font_size = size
 
-    def set_dim(self, width=None, height=None):
+    def set_dim(self, width:int=None, height:int=None) -> None:
         if width != None and height == None:
             self.w, self.h = width, int(
                 (self.h/self.w * width)/self.CH_CONSTANT)
         elif width == None and height != None:
             self.w, self.h = int((self.w/self.h * height)
                                  * self.CH_CONSTANT), height
         else:
             self.w, self.h = width, height
         self.image = self.image.resize((self.w, self.h))
 
-    def asciify(self):
+    def asciify(self) -> None:
         self.matrix = []
         div = 255/(len(self.chars))
         bwdata = self.image.convert('L').getdata()
         for line_no in range(self.h):
             line = []
             for pixel in range(line_no*self.w, line_no*self.w + self.w):
                 line.append(self.chars[int(bwdata[pixel]/div) - 1])
             self.matrix.append(line)
     
-    def replace_char(self, char, x, y):
+    def replace_char(self, char:str, x:int, y:int)-> None:
         if x<self.w and y<self.h:
             self.matrix[y][x] = char
         else:
             raise IndexError
 
-    def replace_chars(self, chars, x, y):
+    def replace_chars(self, chars:str, x:int, y:int) -> None:
         if x>self.w or y>self.h:
             raise TypeError
         if self.w - x >= len(chars):
             for i in range(x, x + len(chars)):
                 self.replace_char(
                     chars[i-x], i, y
                     )
         else:
             self.replace_chars(chars[:self.w-x], x, y)
             self.replace_chars(chars[self.w-x:], 0, y+1)
 
-    def txt_output(self, fname):
+    def txt_output(self, fname:str) -> None:
         text = ""
         for line_no in range(self.h):
             text += "".join(self.matrix[line_no]) + "\n"
         with open(fname + ".txt", "w") as file:
             file.write(text)
             
-    def span(self, integer, integer_colour):
-        return f"<span style='color: rgb{integer_colour};'><b>{integer}</b></span>"
+    def bspan(self, char:str, char_colour:tuple) -> str:
+        return f"<span style='color: rgb{char_colour};'><b>{char}</b></span>"
+    
+    def span(self, char:str, char_colour:tuple) -> str:
+        return f"<span style='color: rgb{char_colour};'>{char}</span>"
 
-    def tspan(self, char, char_color, x):
+    def tspan(self, char:str, char_color:str, x:float) -> str:
         return f'<tspan x="{x}" fill="{char_color}">{char}</tspan>'
     
-    def btspan(self, char, char_color, x):
+    def btspan(self, char:str, char_color:str, x:float) -> str:
         return f'<tspan x="{x}" fill="{char_color}" font-weight="bold">{char}</tspan>'
     
-    def rgb2hex(self, rgba):
+    def rgb2hex(self, rgba:tuple) -> str:
         return '#{:02x}{:02x}{:02x}'.format(rgba[0], rgba[1], rgba[2])
 
-    def svgify(self, bg_color="None", bold=False):
+    def svgify(self, bg_color:str="None", bold:bool=False) -> None:
         file = SVG_HEADER.format(
             int(self.w*self.H_dis)+41, 
             int(self.h*self.V_dis)+41,
             "monospace", self.font_size, bg_color
             )
         file += f'<a href="https://primepatel.github.io/aksharify-docs/">'
         x, y = 20, 30
@@ -115,35 +118,39 @@
             file += '</text>'
             x = 20
             y += self.V_dis
         file += "</a>"
         file += "</svg>"
         self.ascii_svg = file
 
-    def htmlify(self):
+    def htmlify(self, bold:bool=False) -> None:
         html_content = '<p style="font-size: 10px; font-family: monospace;">'
+        if bold == True:
+            span = self.bspan
+        else:
+            span = self.span
         for line_no in range(self.h):
             for char_no in range(self.w):
-                html_content += self.span(
+                html_content += span(
                     self.matrix[line_no][char_no], 
                     self.image.getpixel((char_no, line_no))
                     )
             html_content += '<br>'
         html_content += "</p>"
         self.ascii_html = HTML_HEADER.format(html_content)
     
-    def html_output(self, fname):
+    def html_output(self, fname:str) -> None:
         with open(fname + ".html", "w") as file:
             file.write(self.ascii_html)
 
-    def svg_output(self, fname):
+    def svg_output(self, fname:str) -> None:
         with open(fname + ".svg", "w", encoding="utf-8-sig") as file:
             file.write(self.ascii_svg)
     
-    def png_output(self, fname, svg2png, bg_color="None", height=None, width=None):
+    def png_output(self, fname:str, svg2png, bg_color:str="None", height:int=None, width:int=None) -> None:
         self.svgify(bg_color)
         if height == None and width != None:
             svg2png(bytestring=self.ascii_svg,write_to=fname+'.png',output_width=width)
         elif width == None and height != None:
             svg2png(bytestring=self.ascii_svg,write_to=fname+'.png',output_height=height)
         elif height == None and width == None:
             svg2png(bytestring=self.ascii_svg, write_to=fname+'.png')
@@ -152,60 +159,60 @@
 
 
 class EmojiArt(AksharArt):
     def __init__(self, image, chars="🙂😅") -> None:
         super().__init__(image, chars)
         self.H_dis = 20
     
-    def set_font_size(self, size):
+    def set_font_size(self, size:float) -> None:
         self.H_dis = size
         self.V_dis = size
         self.font_size = size
 
 class TextArt(AksharArt):
     
-    def __init__(self, image, chars=SORTEDCHARS, ordered=False) -> None:
+    def __init__(self, image:Image, chars:str=SORTEDCHARS, ordered:bool=False) -> None:
         super().__init__(image)
         self.chars = list(set(chars))
         if not ordered:
             chars = []
             for char in SORTEDCHARS:
                 if char in self.chars:
                     chars.append(f"&#{ord(char)};")
             self.chars = chars
 
 
 class NumberArt(AksharArt):
 
-    def __init__(self, image, numbers= "0123456789") -> None:
+    def __init__(self, image:Image, numbers:str="0123456789") -> None:
         super().__init__(image, numbers)
         for i in self.chars:
             if not i.isnumeric():
                 raise TypeError
         self.numbers = self.chars
 
-    def numberify(self, first_num=0):
+    def numberify(self, first_num:int=0) -> None:
         self.asciify()
         if first_num != 0:
             self.matrix[0][0] = first_num
-        return self.ascii_text
 
 class PrimeArt(NumberArt):
     
-    def __init__(self, image) -> None:
+    def __init__(self, image:Image) -> None:
         super().__init__(image, "01")
     
-    def binary_to_decimal(self, binary):
+    def binary_to_decimal(self, binary:str) -> int:
         decimal = 0
         l = len(binary)
         for x in binary:
             l -= 1
             decimal += pow(2, l) * int(x)
         return int(decimal)
     
-    def primify(self, prime, asis=True, func=bin):
-        if not asis and len(bin(int(prime))) == len(func(self.ascii_text)):
-            self.ascii_text = func(int(prime))
-        elif len(str(int(prime))) == len(self.ascii_text):
-            self.ascii_text = str(prime)
-        else:
-            print("not primified")
+    # Avoid using self.asciitext
+    # def primify(self, prime, asis=True, func=bin):
+    #     if not asis and len(bin(int(prime))) == len(func(self.ascii_text)):
+    #         self.ascii_text = func(int(prime))
+    #     elif len(str(int(prime))) == len(self.ascii_text):
+    #         self.ascii_text = str(prime)
+    #     else:
+    #         print("not primified")
```

### Comparing `aksharify-2.7.5/pyproject.toml` & `aksharify-2.7.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b74 6f6f 6c2e 706f 6574 7279 5d0d 0a6e  [tool.poetry]..n
 00000010: 616d 6520 3d20 2261 6b73 6861 7269 6679  ame = "aksharify
 00000020: 220d 0a76 6572 7369 6f6e 203d 2022 322e  "..version = "2.
-00000030: 372e 3522 0d0a 6465 7363 7269 7074 696f  7.5"..descriptio
+00000030: 372e 3722 0d0a 6465 7363 7269 7074 696f  7.7"..descriptio
 00000040: 6e20 3d20 2250 7974 686f 6e20 4173 6369  n = "Python Asci
 00000050: 6920 2b20 456d 6f6a 6920 4172 7420 4d6f  i + Emoji Art Mo
 00000060: 6475 6c65 220d 0a61 7574 686f 7273 203d  dule"..authors =
 00000070: 205b 2250 7269 6d65 2050 6174 656c 203c   ["Prime Patel <
 00000080: 7072 696d 6573 7061 7465 6c40 676d 6169  primespatel@gmai
 00000090: 6c2e 636f 6d3e 225d 0d0a 6c69 6365 6e73  l.com>"]..licens
 000000a0: 6520 3d20 224d 4954 220d 0a72 6561 646d  e = "MIT"..readm
```

### Comparing `aksharify-2.7.5/README.md` & `aksharify-2.7.7/README.md`

 * *Files identical despite different names*

### Comparing `aksharify-2.7.5/PKG-INFO` & `aksharify-2.7.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aksharify
-Version: 2.7.5
+Version: 2.7.7
 Summary: Python Ascii + Emoji Art Module
 Home-page: https://primepatel.github.io/aksharify-docs/
 License: MIT
 Keywords: Ascii Art,Emoji Art,Prime Patel,primepatel
 Author: Prime Patel
 Author-email: primespatel@gmail.com
 Requires-Python: >=3.10,<4.0
```

