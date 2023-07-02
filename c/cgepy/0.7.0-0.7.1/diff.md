# Comparing `tmp/cgepy-0.7.0.tar.gz` & `tmp/cgepy-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgepy-0.7.0.tar", max compression
+gzip compressed data, was "cgepy-0.7.1.tar", max compression
```

## Comparing `cgepy-0.7.0.tar` & `cgepy-0.7.1.tar`

### file list

```diff
@@ -1,12 +1,10 @@
--rw-r--r--   0        0        0     1066 2023-02-26 04:58:20.892527 cgepy-0.7.0/LICENSE.md
--rw-r--r--   0        0        0      324 2023-02-28 03:06:43.826763 cgepy-0.7.0/README.md
--rw-r--r--   0        0        0     6148 2023-03-01 02:28:34.930621 cgepy-0.7.0/cgepy/.DS_Store
--rw-r--r--   0        0        0     3878 2023-03-01 01:55:58.390955 cgepy-0.7.0/cgepy/__init__.py
--rw-r--r--   0        0        0      464 2023-02-28 03:06:43.828963 cgepy-0.7.0/cgepy/colors.py
--rw-r--r--   0        0        0     6148 2023-02-28 04:38:35.421132 cgepy-0.7.0/cgepy/ext/.DS_Store
--rw-r--r--   0        0        0       22 2023-02-28 03:06:43.830102 cgepy-0.7.0/cgepy/ext/beta/__init__.py
--rw-r--r--   0        0        0       74 2023-03-01 02:06:54.374203 cgepy-0.7.0/cgepy/ext/clear.py
--rw-r--r--   0        0        0     1218 2023-03-01 02:23:56.765792 cgepy-0.7.0/cgepy/ext/text.py
--rw-r--r--   0        0        0      337 2023-02-28 03:06:43.833135 cgepy-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      911 1970-01-01 00:00:00.000000 cgepy-0.7.0/setup.py
--rw-r--r--   0        0        0      978 1970-01-01 00:00:00.000000 cgepy-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-29 01:41:56.304652 cgepy-0.7.1/LICENSE.md
+-rw-r--r--   0        0        0      508 2023-07-02 20:29:03.422470 cgepy-0.7.1/README.md
+-rw-r--r--   0        0        0     4976 2023-07-02 20:34:38.268411 cgepy-0.7.1/cgepy/__init__.py
+-rw-r--r--   0        0        0      464 2023-06-24 18:46:51.694033 cgepy-0.7.1/cgepy/colors.py
+-rw-r--r--   0        0        0       99 2023-07-02 16:23:21.890637 cgepy-0.7.1/cgepy/ext/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-29 01:45:06.356080 cgepy-0.7.1/cgepy/ext/beta/__init__.py
+-rw-r--r--   0        0        0     1318 2023-07-02 20:33:33.211943 cgepy-0.7.1/cgepy/ext/text.py
+-rw-r--r--   0        0        0      315 2023-06-24 18:46:56.773316 cgepy-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     1085 1970-01-01 00:00:00.000000 cgepy-0.7.1/setup.py
+-rw-r--r--   0        0        0     1128 1970-01-01 00:00:00.000000 cgepy-0.7.1/PKG-INFO
```

### Comparing `cgepy-0.7.0/LICENSE.md` & `cgepy-0.7.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cgepy-0.7.0/cgepy/__init__.py` & `cgepy-0.7.1/cgepy/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,73 +1,86 @@
-__version__ = '0.7.0'
+__version__ = '0.7.1'
+
 try:
-	from cgePy.cgepy.colors import *
+	from cgepy.cgepy.colors import *
 except ModuleNotFoundError:
 	try:
-		from cgepy.cgepy.colors import *
+		from cgePy.cgepy.colors import *
 	except ModuleNotFoundError:
 		from cgepy.colors import *
 
-def cs(): #clear-screen
-	print("\033[2J") #Clears screen
-	print('\033[0;0H') #Resets cursor
-
 spritecolor = RED
 background = BLUE
 gridsize = 100
-
 global pr
 
-class from_getkey:
-	'''These escape sequences were taken from the getkey module. I didn't find these!'''
-	def __init__(self):
-		up = "\x1b[A"
-		down = "\x1b[B"
-		right = "\x1b[C"
-		left = "\x1b[D"
-
-keys = from_getkey()
-del from_getkey
-
+# Internal Functions
+def cs():
+	'''Internal utility for clearing the screen.'''
+	print("\033[2J") #Clears screen
+	print('\033[0;0H') #Resets cursor
 def update():
 	global pr
 	pr = int(gridsize**0.5)
-
 update()
 
-"Classes"
-
+# Classes
+class keys:
+	'''These escape sequences were taken from the getkey module. I didn't find them!'''
+	up = "\x1b[A"
+	down = "\x1b[B"
+	right = "\x1b[C"
+	left = "\x1b[D"
+class Color:
+	"""As of version 7.1, this class is currently unfinished and can not be used.\n\n\nTakes a given string and converts it into a color.\nArguments:\n\tcolor:str\nReturns:\n\tA color object."""
+	def __init__(self, color:str):
+		#self.color=color.replace("BG",background)
+		#self.color=color.replace("RE",RED)
+		#self.color=color.replace("YE",YELLOW)
+		#self.color=color.replace("BG",background)
+		#self.color=color.replace("BG",background)
+		#self.color=color.replace("BG",background)
+		#self.color=color.replace("BG",background)
+		#self.color=color.replace("BG",background)
+		#self.color=color.replace("BG",background)
+		#self.color=color.replace("BG",background)
+		#self.color=color.replace("BG",background)
+		#self.color=color.replace("BG",background)
+		#self.color=color.replace("BG",background)
+		pass
 class Output:
 	pass
-""
 class Exceptions:
 	class OutOfRangeError(Exception):
 		pass
 	class MapError(Exception):
 		pass
-""
 class legacy:
-	
+	'''Legacy functions previously used instead of classes.\n\nNote:\nThese functions are still in use. However, they are considered legacy as you do not need to manually call them anymore.'''
+
 	def creategrid() -> list:
-			newmap=[]
-			for i in range(gridsize):
-				newmap.append(background+"  ")
-			return newmap
+		'''Returns an empty grid.'''
+		newmap=[]
+		for i in range(gridsize):
+			newmap.append(background+"  ")
+		return newmap
 		
 	def updategrid(grid):
+		'''Print a grid onto the screen'''
 		buffer = []
 		for n in range(len(grid)):
 			buffer.append(grid[n])
 			if (n+1) % pr == 0:
 				buffer.append("\n")
 		cs()
 		print(''.join(buffer), end='')
 		print("\x1b[0m")
 		
 	def paint(map: str) -> list:
+		'''Paint a grid using text.'''
 		map = map.replace(" ","")
 		map = map.replace(",","")
 		map = map.replace("\n","")
 		map = map.replace("BG",background+"  ,")
 		map = map.replace("RE",RED+"  ,")
 		map = map.replace("YE",YELLOW+"  ,")
 		map = map.replace("GR",GREEN+"  ,")
@@ -75,16 +88,16 @@
 		map = map.replace("CY",CYAN+" ,")
 		map = map.replace("MA",MAGENTA+"  ,")
 		map = map.replace("BB",BLACK+"  ,")
 		map = map.replace("WH",WHITE+"  ,")
 		map = map.replace("RR",RESET+"  ,")
 		map = map.split(",")
 		return map
-""
 class Grid:
+
 	def __init__(self, ctx="", border = False):
 		update()
 		self.ctx = ctx
 		self.sprites = []
 
 		if ctx == "":
 			if border == False:
@@ -118,15 +131,14 @@
 		self.ctx = legacy.creategrid()
 		
 	def write(self, pos, new):
 		try:
 			self.ctx[pos] = new
 
 		except IndexError:
-			pass
 			raise Exceptions.OutOfRangeError
 			
 	def swap(self, new):
 		self.ctx = new
 
 	def Update(self):
 		update()
@@ -145,50 +157,49 @@
 
 		else:
 
 			legacy.updategrid(self.ctx)
 			
 		
 	def Self(self):
-		return self.ctx
-""		     
+		return self.ctx	     
 class Map:
 
 	def __init__(self, map=False):
 		if map==False:
 			self.main = '''undefined'''
 		else:
 			self.main = map
 	def Paint(self):
 		if self.main == '''undefined''':
 			raise Exceptions.MapError("Cannot paint an undefined map.")
 		else:
 			self.ctx = legacy.paint(self.main)
 			del self.main
 			self.__class__ = Grid
-""
 class Sprite:
-	def __init__(self,pos=0,color=RED):
+	def __init__(self, pos=0, color=RED):
 		self.pos = pos
 		self.color = color
 		self.sprite = color+"  "
-	def Color(self,color):
+	def Color(self, color):
 		self.color = color
 		self.sprite = color+"  "
-	def Move(self,dir):
+	def Move(self, dir:str):
 		if dir.lower() in ["up","w","i","\x1b[A"]:
 			self.pos -= pr
 		if dir.lower() in ["down","s","k","\x1b[B"]:
 			self.pos += pr
 		if dir.lower() in ["left","a","j","\x1b[D"]:
 			self.pos -= 1
 		if dir.lower() in ["right","d","l","\x1b[C"]:
 			self.pos += 1
-
-	def Drop(self,grid,request=False):
+	def Drop(self, grid, request=False):
 		if request == False:
 			grid.sprites.append(self)
 		if request == True:
 			grid.sprites.remove(self)
 			self.Drop(grid)
-	def Remove(self,grid):
+	def Remove(self, grid):
 		grid.sprites.remove(self)
+
+# cgePy.cgepy.__init__.py
```

### Comparing `cgepy-0.7.0/cgepy/ext/text.py` & `cgepy-0.7.1/cgepy/ext/text.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-__version__ = '0.7.0'
+__version__ = '0.7.1'
 
 try:
 	from cgePy.cgepy.colors import *
 	from cgePy.cgepy.__init__ import *
 except ModuleNotFoundError:
 	try:
 		from cgepy.cgepy.colors import *
 		from cgepy.cgepy.__init__ import *
 	except ModuleNotFoundError:
 		from cgepy.colors import *
 		from cgepy.__init__ import *
 
 class empty:
+	'''The name says it all.'''
 	pass
 
-class Engine:
-	def __init__(self, grid: Grid):
+class TextEngine:
+	'''A text engine allowing for text inside grids.'''
+	def __init__(self, grid: Grid) -> TextEngine:
 		self.grid = grid
 		self.temp = empty()
 	def Insert(self, content, index=0):
 		self.temp.content = content
 		self.index = index
 		self.temp.contentlen = len(content)
 		if self.temp.contentlen % 2 != 0:
```

### Comparing `cgepy-0.7.0/setup.py` & `cgepy-0.7.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 ['cgepy', 'cgepy.ext', 'cgepy.ext.beta']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'cgepy',
-    'version': '0.7.0',
+    'version': '0.7.1',
     'description': 'Tools for developing graphical programs inside the console.',
-    'long_description': '### cgepy // 0.7.0\n###### A simple graphics engine with no dependencies.\n***\ncgePy, or cge, is a text-based graphics engine that can operate in the console or terminal.\\\nCurrently with zero dependencies, a simple system that can suit many needs, and easily tweaked settings, cgePy will allow you to turn ideas into reality.\n',
+    'long_description': "### cgepy // 0.7.1\n##### A lightweight 8-bit graphics engine\n***\n###### Documentation: https://cgepy.github.io/docs\nLooking for something simple to use? Want to use a reliable package for once?\\\ncgepy's got you covered.\n\nFeaturing a powerful, but easy-to-use system, you can make fun games with cgepy.\\\nThough cgepy lacks many things like mouse support and native keyboard support, it is ever growing and will soon have so many features in place of those, while maintaining that same speed and reliablility.\n",
     'author': 'catbox305',
-    'author_email': 'lion712yt@gmail.com',
+    'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'python_requires': '>=3.6,<4.0',
 }
```

### Comparing `cgepy-0.7.0/PKG-INFO` & `cgepy-0.7.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: cgepy
-Version: 0.7.0
+Version: 0.7.1
 Summary: Tools for developing graphical programs inside the console.
 License: MIT
 Author: catbox305
-Author-email: lion712yt@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
-### cgepy // 0.7.0
-###### A simple graphics engine with no dependencies.
+### cgepy // 0.7.1
+##### A lightweight 8-bit graphics engine
 ***
-cgePy, or cge, is a text-based graphics engine that can operate in the console or terminal.\
-Currently with zero dependencies, a simple system that can suit many needs, and easily tweaked settings, cgePy will allow you to turn ideas into reality.
+###### Documentation: https://cgepy.github.io/docs
+Looking for something simple to use? Want to use a reliable package for once?\
+cgepy's got you covered.
+
+Featuring a powerful, but easy-to-use system, you can make fun games with cgepy.\
+Though cgepy lacks many things like mouse support and native keyboard support, it is ever growing and will soon have so many features in place of those, while maintaining that same speed and reliablility.
```

