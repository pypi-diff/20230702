# Comparing `tmp/langful-0.29-py2.py3-none-any.whl.zip` & `tmp/langful-0.30-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5118 bytes, number of entries: 7
+Zip file size: 5422 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat      224 b- defN 23-Jun-20 12:20 langful/__init__.py
--rw-rw-rw-  2.0 fat     9134 b- defN 23-Jun-28 10:37 langful/lang.py
--rw-rw-rw-  2.0 fat     1066 b- defN 23-Jun-28 10:41 langful-0.29.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2859 b- defN 23-Jun-28 10:41 langful-0.29.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Jun-28 10:41 langful-0.29.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-28 10:41 langful-0.29.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      528 b- defN 23-Jun-28 10:41 langful-0.29.dist-info/RECORD
-7 files, 13929 bytes uncompressed, 4188 bytes compressed:  69.9%
+-rw-rw-rw-  2.0 fat     9667 b- defN 23-Jul-02 03:20 langful/lang.py
+-rw-rw-rw-  2.0 fat     1066 b- defN 23-Jul-02 03:32 langful-0.30.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3101 b- defN 23-Jul-02 03:32 langful-0.30.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Jul-02 03:32 langful-0.30.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-02 03:32 langful-0.30.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      528 b- defN 23-Jul-02 03:32 langful-0.30.dist-info/RECORD
+7 files, 14704 bytes uncompressed, 4492 bytes compressed:  69.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: langful/__init__.py
 Comment: 
 
 Filename: langful/lang.py
 Comment: 
 
-Filename: langful-0.29.dist-info/LICENSE
+Filename: langful-0.30.dist-info/LICENSE
 Comment: 
 
-Filename: langful-0.29.dist-info/METADATA
+Filename: langful-0.30.dist-info/METADATA
 Comment: 
 
-Filename: langful-0.29.dist-info/WHEEL
+Filename: langful-0.30.dist-info/WHEEL
 Comment: 
 
-Filename: langful-0.29.dist-info/top_level.txt
+Filename: langful-0.30.dist-info/top_level.txt
 Comment: 
 
-Filename: langful-0.29.dist-info/RECORD
+Filename: langful-0.30.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## langful/lang.py

```diff
@@ -33,44 +33,68 @@
         ret += f"{ key } = { value }\n"
     return ret
 
 class lang :
     """
     # lang
     """
-    def __init__( self , lang_dir : str  |  bool = "lang" , default_locale : str = "en_us" ) -> None :
+
+    def __getitem__( self , key ) -> str :
+        return self.get( key )
+
+    def __setitem__( self , key , value ) -> None :
+        self.set( key , value )
+
+    def __delitem__( self , key ) -> None :
+        self.remove( key )
+
+    def __call__( self ) -> None :
+        self.init()
+
+    def __len__( self ) -> int :
+        return len( self.languages )
+
+    def __init__( self , lang_dir : str  |  bool = "lang" , default_locale : str = "en_us" , json_first : bool = True ) -> None :
         """
         lang_dir: lang files dir, if use dict to set that False
         default_locale: default locale
+        json_first: is load json file first
         """
-        self.lang_dir = lang_dir
         system_locale = self.get_system_locale
         self.default_locale = default_locale
         self.system_locale = system_locale
+        self.json_first = json_first
         self.replace_letter = "%"
+        self.lang_dir = lang_dir
         self.is_file = False
         self.languages = {}
         self.locales = []
         self.types = {}
         self.init()
 
     def init( self ) -> None :
         """
-        # init
+        init by a directory
         """
         path = self.lang_dir
         if isinstance( path , str ) :
             self.is_file = True
+        if not isinstance( self.json_first , bool ) :
+            self.json_first = True
+        if self.json_first :
+            loads = [ ".json" , ".lang" ]
+        else :
+            loads = [ ".lang" , ".json" ]
         if self.is_file :
             if not os.path.exists( path ) :
                 raise FileNotFoundError( f"can't find '{ os.path.abspath( path ) }'" )
             files = []
             for i in os.listdir( path ) :
                 name , suffix = os.path.splitext( i )
-                if ( suffix == ".json" ) or ( name + ".json" not in files ) :
+                if ( suffix in loads ) and ( ( suffix == loads[0] ) or ( name + loads[0] not in files ) ) :
                     files.append( i )
                     with open( os.path.join( path , i ) , encoding = "utf-8" ) as file :
                         if suffix == ".json" :
                             try :
                                 data = json.load( file )
                             except json.decoder.JSONDecodeError :
                                 raise SyntaxError( "can't to load .json file" )
@@ -80,15 +104,15 @@
                             continue
                     self.locales.append( name )
                     self.languages[ name ] = data
                     self.types[ name ] = suffix
 
     def init_dict( self , language : dict ) -> None :
         """
-        init by a dictionary, but cant't to save
+        init by a dictionary, so cant't to save it to the file
         """
         if self.is_file :
             raise TypeError( "can't init by a dictionary, because it's init by a dir" )
         for value in language.values() :
             if not isinstance( value , dict ) :
                 raise TypeError( f"can't use type '{ type( value ) }'" )
         for key in language.keys() :
@@ -126,79 +150,92 @@
     def lang( self ) -> dict :
         """
         same to language function
         """
         return self.language
 
     @property
+    def langs( self ) -> dict :
+        """
+        same to languages variable
+        """
+        return self.languages
+
+    @property
     def type( self ) -> str :
         """
-        get type, '.json' or '.lang'
+        get type, ".json" or ".lang"
         """
         return self.types[ self.locale ]
 
     def get_locale( self , locale : str = None ) -> str :
+        """
+        get locale, usually use in function
+        """
         if locale :
             return locale
         else :
             return self.locale
 
     def get_replace_letter( self , replace_letter : str = None ) -> str :
+        """
+        get replace letter, usually use in function
+        """
         if replace_letter :
             return replace_letter
         else :
             return self.replace_letter
 
     def set_locale( self , locale : str = None  ) -> None :
         """
-        set/reset locale
+        if give a locale then set that, else reset it
         """
         if locale != None :
             self.system_locale = locale
         else :
             self.system_locale = self.get_system_locale
 
     def lang_set( self , locale : str , suffix : str , value : dict = {} ) -> None :
         """
-        set lang
+        set a new lang
         """
         self.languages[ locale ] = value
         self.types[ locale ] = suffix
 
     def lang_del( self , locale : str ) -> None :
         """
-        del lang
+        del a lang
         """
         del self.languages[ locale ]
         del self.types[ locale ]
 
     def get( self , key : str | int , locale : str = None ) -> str :
         """
-        get
+        get the key by a locale dictionary
         """
         locale = self.get_locale( locale )
         return self.languages[ locale ][ key ]
 
     def set( self , key : str | int , value : str , locale : str = None ) -> None :
         """
-        set
+        set a value by a locale dictionary
         """
         locale = self.get_locale( locale )
         self.languages[ locale ][ key ] = value
 
     def remove( self , key : str | int , locale : str = None ) -> None :
         """
-        remove
+        remove a value by a locale dictionary
         """
         locale = self.get_locale( locale )
         del self.languages[ locale ][ key ]
 
     def save( self ) -> None :
         """
-        save file, when is_file is true
+        save file when is_file variable is true, else raise the error
         """
         if self.is_file :
             for key , value in self.languages.items() :
                 suffix = self.types[ key ]
                 print(suffix,value)
                 with open( os.path.join( self.lang_dir , key + suffix ) , "w+" , encoding = "utf-8" ) as file :
                     if suffix == ".json" :
@@ -206,59 +243,40 @@
                     elif suffix == ".lang" :
                         file.write( json_to_lang( value ) )
         else :
             raise TypeError( "can't to save, because it's not a file" )
 
     def save_dict( self ) -> dict :
         """
-        save dict. in fact, it just return the 'languages' variable
+        save dict. in fact, it just return the "languages" variable
         """
         if not self.is_file :
             return self.languages
         else :
             raise TypeError( "can't to save, because it's not a dict" )
 
     def replace( self , key : str = None , args : list | str = None , locale : str = None , replace_letter : str = None ) -> str :
         """
         replace
         """
-        # locale = self.get_locale( locale )
-        # replace_letter = self.get_replace_letter( replace_letter )
-        # text = []
-        # ret = ""
-        # p = 0
-        # for i in self.get( key ).split( replace_letter * 2 ) :
-        #     if i :
-        #         print(i.split( replace_letter ))
-        #         text += i.split( replace_letter )
-        #     else :
-        #         text += replace_letter
-        # print(text)
-        # if not isinstance( args , list ) :
-        #     args = [ str( args ) ]
-        # for i in range ( len( text ) ) :
-        #     print(text[i])
-        #     p += 1
-        # return ret
-        if not replace_letter :
-            replace_letter = self.replace_letter
-        if not locale :
-            locale = self.locale
+        replace_letter = self.get_replace_letter( replace_letter )
+        locale = self.get_locale( locale )
         text = self.get( key , locale ).split( replace_letter )
-        if len( text ) == 1 :
-            text = text[0]
+        if isinstance( args , str ) :
+            args = [ args ]
         ret = ""
-        for i in range( len( text ) ) :
-            if ( len( text ) - 1 ) > i :
-                if len( args ) > i :
-                    ret += text[i] + args[i]
+        p = 0
+        for i in text :
+            ret += i
+            if ( p + 1 ) < len( text ) :
+                if p < len( args ) :
+                    ret += str( args[ p ] )
                 else :
-                    ret += text[i] + args[-1]
-            else :
-                ret += text[i]
+                    ret += str( args[ -1 ] )
+                p += 1
         return ret
 
     def replace_str( self , text : str , locale : str = None , replace_letter : str = None ) -> str :
         """
         replace by str
         """
         locale = self.get_locale( locale )
```

## Comparing `langful-0.29.dist-info/LICENSE` & `langful-0.30.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `langful-0.29.dist-info/METADATA` & `langful-0.30.dist-info/METADATA`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: langful
-Version: 0.29
+Version: 0.30
 Home-page: https://github.com/cueavyqwp/langful
 Author: cueavyqwp
 Author-email: cueavyqwp@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: > 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<div align="center">
+<div align = "center" >
     <h1>langful</h1>
     <a href = "https://pypi.org/project/langful" >
         <img alt = "PyPI version" src = "https://img.shields.io/pypi/v/langful?color=blue" >
     </a>
     <a href = "https://www.python.org" >
         <img alt = "Python version" src = "https://img.shields.io/badge/python-3.6+-blue" >
     </a>
@@ -24,61 +24,80 @@
     </a>
     <a href = "https://github.com/cueavyqwp/langful" >
         <img alt = "Github stars" src = "https://img.shields.io/github/stars/cueavyqwp/langful?color=blue" >
     </a>
     <a href = "https://github.com/cueavyqwp/langful" >
         <img alt = "Github issues" src = "https://img.shields.io/github/issues/cueavyqwp/langful?color=blue" >
     </a>
-</div>
 
-# install
+---
 
-`pip3 install langful` or `pip install langful`
+[
+en_us
+|
+[zh_cn](./README-zh_cn.md)
+]
 
-# vscode-langful
+---
 
-[GitHub](https://github.com/cueavy/vscode-langful)
+</div>
+
+# install
 
-[VSCode](https://marketplace.visualstudio.com/items?itemName=cueavyqwp.langful)
+`pip3 install langful` or `pip install langful`
 
 # get start
 
 ## lang file
 
 > ps: `langful` load json file first
+>
+> or you can set to `langful.lang( json_first = False )`
 
-### .json
+.json
 
 ```json
 {
     "key": "value" ,
     "..." : "..."
 }
 ```
 
-### .lang
+.lang
+
+> if you need highlight, you can install `vscode-langful` : [GitHub](https://github.com/cueavy/vscode-langful) [VSCode](https://marketplace.visualstudio.com/items?itemName=cueavyqwp.langful)
 
 ```
 key = value # hi, this is a example
 # hi, I am a example, too
 ... = ...
 ```
 
 ## init
 
 there have `two` ways to init
 
-> by files
+### by files
 
 ```python
 import langful
 lang = langful.lang()
 ```
 
-> by dictionary
+then you can put file at there :
+
+* lang
+* * en_us.lang
+* * en_us.json
+* * zh_cn.lang
+* * zh_cn.json
+
+or use other directory name and set `langful.lang( "directory name" )`
+
+### by dictionary
 
 ```python
 import langful
 lang = langful.lang( False )
 lang.init_dict( {
     "en_us" : {
         "hi" : "Hi" ,
@@ -87,34 +106,31 @@
     "zh_cn" : {
         "hi" : "你好" ,
         "welcome" : "欢迎"
     }
 } )
 ```
 
-## replace
+## function
 
-have bug
+### replace
 
-<!-- ```python
-import langful
+
+```python
 lang = langful.lang( False )
+lang.replace_letter = "&"
 lang.init_dict( {
     "en_us" : {
-        "hi" : "Hi" ,
-        "welcome" : "Welcome"
-    } ,
-    "zh_cn" : {
-        "hi" : "你好" ,
-        "welcome" : "欢迎"
+        "test" : "&.&%"
     }
 } )
-``` -->
+print( lang.replace( "test" , [ 33 , 3 ] ) )
+```
 
-## replace str
+### replace str
 
 ```python
 import langful
 lang = langful.lang( False )
 lang.init_dict( {
     "en_us" : {
         "hi" : "Hi" ,
@@ -124,14 +140,14 @@
         "hi" : "你好" ,
         "welcome" : "欢迎"
     }
 } )
 print(lang.replace_str( "%hi%, %welcome%!" ))
 ```
 
-# About
-
-github: https://github.com/cueavyqwp/langful
-
-pypi: https://pypi.org/project/langful
+# about
 
-issues: https://github.com/cueavyqwp/langful/issues
+[
+[github](https://github.com/cueavyqwp/langful)
+|
+[pypi](https://pypi.org/project/langful)
+]
```

