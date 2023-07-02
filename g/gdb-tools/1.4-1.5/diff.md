# Comparing `tmp/gdb-tools-1.4.tar.gz` & `tmp/gdb-tools-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdb-tools-1.4.tar", last modified: Sat Feb  5 22:52:39 2022, max compression
+gzip compressed data, was "gdb-tools-1.5.tar", last modified: Sun Jul  2 20:16:19 2023, max compression
```

## Comparing `gdb-tools-1.4.tar` & `gdb-tools-1.5.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwx------   0 serg      (1000) serg      (1000)        0 2022-02-05 22:52:39.954886 gdb-tools-1.4/
--rw-------   0 serg      (1000) serg      (1000)     1503 2017-06-09 16:15:52.000000 gdb-tools-1.4/LICENSE
--rw-------   0 serg      (1000) serg      (1000)     3637 2022-02-05 22:52:39.954886 gdb-tools-1.4/PKG-INFO
--rw-------   0 serg      (1000) serg      (1000)     2963 2018-03-02 22:03:47.000000 gdb-tools-1.4/README.md
-drwx------   0 serg      (1000) serg      (1000)        0 2022-02-05 22:52:39.953886 gdb-tools-1.4/duel/
--rw-------   0 serg      (1000) serg      (1000)     1658 2018-02-16 17:41:49.000000 gdb-tools-1.4/duel/__init__.py
--rw-------   0 serg      (1000) serg      (1000)     9482 2022-02-05 15:56:00.000000 gdb-tools-1.4/duel/expr.py
--rw-------   0 serg      (1000) serg      (1000)    12040 2019-02-11 15:22:55.000000 gdb-tools-1.4/duel/help.md
--rw-------   0 serg      (1000) serg      (1000)     1693 2019-08-04 12:47:44.000000 gdb-tools-1.4/duel/help.py
--rw-------   0 serg      (1000) serg      (1000)    14254 2022-02-04 19:33:48.000000 gdb-tools-1.4/duel/parser.py
-drwx------   0 serg      (1000) serg      (1000)        0 2022-02-05 22:52:39.954886 gdb-tools-1.4/gdb_tools.egg-info/
--rw-------   0 serg      (1000) serg      (1000)     3637 2022-02-05 22:52:39.000000 gdb-tools-1.4/gdb_tools.egg-info/PKG-INFO
--rw-------   0 serg      (1000) serg      (1000)      304 2022-02-05 22:52:39.000000 gdb-tools-1.4/gdb_tools.egg-info/SOURCES.txt
--rw-------   0 serg      (1000) serg      (1000)        1 2022-02-05 22:52:39.000000 gdb-tools-1.4/gdb_tools.egg-info/dependency_links.txt
--rw-------   0 serg      (1000) serg      (1000)        9 2022-02-05 22:52:39.000000 gdb-tools-1.4/gdb_tools.egg-info/requires.txt
--rw-------   0 serg      (1000) serg      (1000)       20 2022-02-05 22:52:39.000000 gdb-tools-1.4/gdb_tools.egg-info/top_level.txt
-drwx------   0 serg      (1000) serg      (1000)        0 2022-02-05 22:52:39.954886 gdb-tools-1.4/pretty_printer/
--rw-------   0 serg      (1000) serg      (1000)     2298 2020-10-25 16:59:41.000000 gdb-tools-1.4/pretty_printer/__init__.py
--rw-------   0 serg      (1000) serg      (1000)       83 2022-02-05 21:47:31.000000 gdb-tools-1.4/pyproject.toml
--rw-------   0 serg      (1000) serg      (1000)      726 2022-02-05 22:52:39.954886 gdb-tools-1.4/setup.cfg
+drwx------   0 serg      (1000) serg      (1000)        0 2023-07-02 20:16:19.480998 gdb-tools-1.5/
+-rw-------   0 serg      (1000) serg      (1000)     1503 2017-06-09 16:15:52.000000 gdb-tools-1.5/LICENSE
+-rw-------   0 serg      (1000) serg      (1000)     3600 2023-07-02 20:16:19.480998 gdb-tools-1.5/PKG-INFO
+-rw-------   0 serg      (1000) serg      (1000)     2950 2022-02-05 23:04:08.000000 gdb-tools-1.5/README.md
+drwx------   0 serg      (1000) serg      (1000)        0 2023-07-02 20:16:19.479998 gdb-tools-1.5/duel/
+-rw-------   0 serg      (1000) serg      (1000)     1727 2022-02-20 17:50:49.000000 gdb-tools-1.5/duel/__init__.py
+-rw-------   0 serg      (1000) serg      (1000)    10172 2023-07-02 19:57:23.000000 gdb-tools-1.5/duel/expr.py
+-rw-------   0 serg      (1000) serg      (1000)    12494 2022-02-20 12:27:08.000000 gdb-tools-1.5/duel/help.md
+-rw-------   0 serg      (1000) serg      (1000)     1627 2023-05-04 15:26:48.000000 gdb-tools-1.5/duel/help.py
+-rw-------   0 serg      (1000) serg      (1000)    14256 2023-07-02 20:09:01.000000 gdb-tools-1.5/duel/parser.py
+drwx------   0 serg      (1000) serg      (1000)        0 2023-07-02 20:16:19.479998 gdb-tools-1.5/gdb_tools.egg-info/
+-rw-------   0 serg      (1000) serg      (1000)     3600 2023-07-02 20:16:19.000000 gdb-tools-1.5/gdb_tools.egg-info/PKG-INFO
+-rw-------   0 serg      (1000) serg      (1000)      318 2023-07-02 20:16:19.000000 gdb-tools-1.5/gdb_tools.egg-info/SOURCES.txt
+-rw-------   0 serg      (1000) serg      (1000)        1 2023-07-02 20:16:19.000000 gdb-tools-1.5/gdb_tools.egg-info/dependency_links.txt
+-rw-------   0 serg      (1000) serg      (1000)        9 2023-07-02 20:16:19.000000 gdb-tools-1.5/gdb_tools.egg-info/requires.txt
+-rw-------   0 serg      (1000) serg      (1000)       20 2023-07-02 20:16:19.000000 gdb-tools-1.5/gdb_tools.egg-info/top_level.txt
+drwx------   0 serg      (1000) serg      (1000)        0 2023-07-02 20:16:19.479998 gdb-tools-1.5/pretty_printer/
+-rw-------   0 serg      (1000) serg      (1000)     2298 2020-10-25 16:59:41.000000 gdb-tools-1.5/pretty_printer/__init__.py
+-rw-------   0 serg      (1000) serg      (1000)       83 2022-02-05 21:47:31.000000 gdb-tools-1.5/pyproject.toml
+-rw-------   0 serg      (1000) serg      (1000)      753 2023-07-02 20:16:19.480998 gdb-tools-1.5/setup.cfg
+drwx------   0 serg      (1000) serg      (1000)        0 2023-07-02 20:16:19.480998 gdb-tools-1.5/tests/
+-rwx------   0 serg      (1000) serg      (1000)      763 2023-07-02 20:04:13.000000 gdb-tools-1.5/tests/test.py
```

### Comparing `gdb-tools-1.4/LICENSE` & `gdb-tools-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gdb-tools-1.4/PKG-INFO` & `gdb-tools-1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: gdb-tools
-Version: 1.4
+Version: 1.5
 Summary: Various tools to improve the gdb experience
 Home-page: https://github.com/vuvova/gdb-tools
 Author: Sergei Golubchik
 Author-email: vuvova@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Debuggers
@@ -23,16 +21,14 @@
 This repository contains various tools used to make the time spent in gdb more
 comfortable.
 
 To install these tools, first install the modules with
 
     pip install gdb-tools
 
-or with `easy_install` or `python setup.py install [--user]`.
-
 Then you need to import corresponding modules into your gdb. Add, for example,
 
     py import duel
 
 into your `~/.gdbinit`. If you plan to use `pretty_printer` module, I'd
 recommend to put all your python gdb enhancements in `~/.gdb.py` and source it
 from `~/.gdbinit`.
@@ -90,10 +86,8 @@
 `dl head-->next->val` | `val` of each element in a linked list
 `dl head-->(left,right)->val` | `val` of each element in a binary tree
 `dl head-->next[[20]]` | element 20 of list
 `dl #/head-->next` | count elements on a linked list
 `dl #/(head-->next-val>?5)` | count those over 5
 `dl head-->(next!=?head)` | expand cyclic linked list
 
-Or read the [manual](duel/help.md).
-
-
+Or read the [manual](https://github.com/vuvova/gdb-tools/blob/arpeggio/duel/help.md).
```

### Comparing `gdb-tools-1.4/README.md` & `gdb-tools-1.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 This repository contains various tools used to make the time spent in gdb more
 comfortable.
 
 To install these tools, first install the modules with
 
     pip install gdb-tools
 
-or with `easy_install` or `python setup.py install [--user]`.
-
 Then you need to import corresponding modules into your gdb. Add, for example,
 
     py import duel
 
 into your `~/.gdbinit`. If you plan to use `pretty_printer` module, I'd
 recommend to put all your python gdb enhancements in `~/.gdb.py` and source it
 from `~/.gdbinit`.
@@ -70,8 +68,8 @@
 `dl head-->next->val` | `val` of each element in a linked list
 `dl head-->(left,right)->val` | `val` of each element in a binary tree
 `dl head-->next[[20]]` | element 20 of list
 `dl #/head-->next` | count elements on a linked list
 `dl #/(head-->next-val>?5)` | count those over 5
 `dl head-->(next!=?head)` | expand cyclic linked list
 
-Or read the [manual](duel/help.md).
+Or read the [manual](https://github.com/vuvova/gdb-tools/blob/arpeggio/duel/help.md).
```

### Comparing `gdb-tools-1.4/duel/__init__.py` & `gdb-tools-1.5/duel/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import gdb
 import sys
 import traceback
 
 from duel.help import *
 from duel import parser, expr
 
+VERSION='1.5'
+
 class duel (gdb.Command):
     """Evaluate Duel expressions.
 
 Duel is a high level data exploration language.
 Type "dl" for help"""
 
     debug = False
 
     def __init__ (self):
         super (duel, self).__init__ ("duel", gdb.COMMAND_DATA, gdb.COMPLETE_EXPRESSION, False)
         gdb.execute('alias -a dl = duel')
-        gdb.write("Loaded " + HEADER)
+        gdb.write("Loaded DUEL.py " + VERSION + ", high level data exploration language\n")
 
     def invoke (self, arg, from_tty):
         if arg == "":
             gdb.write(INTRO)
         elif arg in [ '?', 'help' ]:
             gdb.write(HELP)
         elif arg in [ '??', 'longhelp' ]:
```

### Comparing `gdb-tools-1.4/duel/expr.py` & `gdb-tools-1.5/duel/expr.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,23 @@
 scopes = list()
 
 def val2str(v):
     try: v = v.referenced_value() if v.type.code==gdb.TYPE_CODE_REF else v
     except: pass
     return str(v)
 
+# this uses gdb convenience variables to avoid convering all arguments to strings
+def parse_and_call(func, *args):
+    s = func + '('
+    for i, a in enumerate(args):
+        n = 'duel_eval_func_call_'+str(i)
+        gdb.set_convenience_variable(n, a)
+        s += '$' + n + ','
+    return gdb.parse_and_eval(s[0:-1]+')')
+
 class Expr(object):
     def name(self): return self.name_
     def value(self): return self.value_
     def eval(self): yield self.name(), self.value()
     def no_parens(self): return False
     def scoped_eval(self, v):
         g = self.eval()
@@ -134,15 +143,21 @@
                 l = len(queue)
                 for n2,v2 in self.arg2_.scoped_eval(v1.dereference()):
                     queue.insert(l, (n1+[n2], v2))
 
 class TakeNth(BinaryBase):
     name_ = '{0}[[{1}]]'
     def eval(self):
+        l = None
         for n2,v2 in self.arg2_.eval():
+            if v2 < 0:
+                if l is None: l = sum(1 for i in self.arg1_.eval())
+                v2 += l
+                if isinstance(self.arg2_, Curlies): n2 = str(v2)
+                if v2 < 0: raise StopIteration
             val = self.arg1_.eval()
             for i in xrange(0,v2): next(val)
             n1, v1 = next(val)
             yield self.name_.format(self.arg1_.name(), n2), v1
 
 class Until(BinaryBase):
     name_ = '{0}@{1}'
@@ -262,14 +277,16 @@
     def eval(self):
         for n1,v1 in self.arg1_.eval():
             args = self.arg2_.args_
             gens = [] + args
             nams = [] + args
             vals = [] + args
             cur = -1
+            if v1.type.code == gdb.TYPE_CODE_INTERNAL_FUNCTION:
+                v1=lambda *args: parse_and_call(n1, *args)
             while True:
                 while cur < len(args)-1:
                     cur += 1
                     gens[cur] = args[cur].eval()
                     nams[cur], vals[cur] = next(gens[cur])
                 yield self.name_.format(n1, ','.join(nams)), v1(*vals)
                 repeat = True
```

### Comparing `gdb-tools-1.4/duel/help.md` & `gdb-tools-1.5/duel/help.md`

 * *Files 3% similar despite different names*

```diff
@@ -95,16 +95,26 @@
     (gdb) head-->next[[3]]->data
     head-->next[[3]]->data = 26
 
 For example,
 
     (gdb) dl head-->next[[50..60]]->data
 
-return the 50th through the 60th elements in the list. The `#/x`
-operator counts the number of values, so
+return the 50th through the 60th elements in the list. By specifying a
+negative number one can count from the end:
+
+    (gdb) head-->next[[-1]]->data
+    head-->next[[-1]]->data = 123
+
+And curly braces evaluate the offset, as usual:
+
+    (gdb) head-->next[[{-1}]]->data
+    head-->next[[73]]->data = 123
+
+The `#/x` operator counts the number of values, so
 
     (gdb) dl #/( head-->next->data >? 50 )
 
 counts the number of data elements over 50 on the list.
 
 Operator `x@y` stops `x` generating values, as soon as `y` becomes
 true.  It is mainly used with the unbounded `x..` range:
@@ -186,19 +196,20 @@
 * `x#y` - for every value of `x`, set `y` to the index of this `x`
   value (0, 1, ...).
 * `x.y`, `x->y`, `x-->y`, `x[y]`, `x[[y]]`, `x@y` - the first two
   operators are *scope* operators, they evaluate `y` in the scope of
   `x`. The third one walks the linked list, evaluating `x`, `x->y`,
   `x->y->y`, etc until NULL. The fourth is a familiar C array element
   access, the fifth takes the `y`-th value in the sequence of values
-  of `x`. The last one stops `x` from generating values as soon as `y`
-  (evaluated in the scope of `x`) becomes true. If `y` is a literal,
-  stops as soon as `x` value becomes equal to `y`. If `y` is a
-  sequence of values, stops when at least one value in the sequence is
-  true, and prints `x` if at least one value in the sequence is false.
+  of `x` (counting from the end, if `y` is negative). The last one
+  stops `x` from generating values as soon as `y` (evaluated in the
+  scope of `x`) becomes true. If `y` is a literal, stops as soon as
+  `x` value becomes equal to `y`. If `y` is a sequence of values,
+  stops when at least one value in the sequence is true, and prints
+  `x` if at least one value in the sequence is false.
 * `(cast)x`, `-x`, `*x`, `&x`, `!x`, `~x`, `#/x`, `+/x`, `&&/x`, `||/x` -
   first six are conventional unary C operators, the last four are
   *grouping* operators.  The first one counts the numbers of values of
   `x`, the second sums them, the third returns a boolean AND of all
   values of `x`, the fourth - boolean OR. Just like in C, AND and OR
   operators are lazy and stop as soon as the result value is known.
 * `x/y`, `x*y`, `x%y` - conventional C operators.
@@ -328,25 +339,29 @@
 
     dl #/head-->next
 
 Find the last element in a linked list:
 
     dl x-->y[[#/x-->y - 1]]
 
+Or just
+
+    dl x-->y[[-1]]
+
 Walk the cyclic linked list (start from `head`, walk until seeing `head` again):
 
     dl head-->(next!=?head)
 
 Walk the binary tree:
 
     dl root-->(left,right)->key
 
 Select matching strings from the array:
 
-    dl strncmp(items[i:=0..20], "foo", 3) ==? 0 => items[i]
+    dl $_regex(items[i:=0..20], "foo") ==? 1 => items[i]
 
 Find first 10 primes greater than 1000:
 
     dl (1000..=>if(&&/(2,3.._-1=>__%_ )) _)[[..10]]
 
 To Do
 -----
@@ -357,14 +372,17 @@
 * Builtins: `frame()`, `sizeof()`, `frames_no`, `func.x`
 * Variables: `int i; i=5; i++`
 * Assignments: `x[..10]=0`
 * `while` and `for` operators
 
 Features that were not in the original Duel:
 * gdb scope specification: `file.c::var`
+* gdb convenience variables (`$a`), references to results (`$1`) and
+  functions (`$_streq`)
+* negative indexes in `[[ ]]` operator
 
 
 Author
 ------
 
 Duel was designed by Michael Golan as part of a PhD thesis in the
 Computer Science Department of Princeton University. He also
```

### Comparing `gdb-tools-1.4/duel/help.py` & `gdb-tools-1.5/duel/help.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import re
 
-HEADER = 'DUEL.py 0.9.7, high level data exploration language\n'
-
 INTRO = """\
 Supported DUEL commands:
 duel help      - give basic help (shortcut: dl ?)
 duel longhelp  - give a longer help (dl ??)
 duel examples  - show useful usage examples
 duel operators - operators summary
 duel aliases   - show current aliases
@@ -31,10 +29,10 @@
 
 Duel was created by Michael Golan at Princeton University.
 Duel.py is a pure-python Duel implementation by Sergei Golubchik.
 
 Try "dl operators" or "dl longhelp"
 """
 
-OPERATORS = re.sub(r'^(?s).*\nOperators\n---------\n\n*(.*?\n)[^\n]+\n-----+\n.*$', r'\1', LONGHELP)
-EXAMPLES = re.sub(r'^(?s).*\nExamples\n--------\n\n*(.*?\n)[^\n]+\n-----+\n.*$', r'\1', LONGHELP)
+OPERATORS = re.sub(r'(?s)^.*\nOperators\n---------\n\n*(.*?\n)[^\n]+\n-----+\n.*$', r'\1', LONGHELP)
+EXAMPLES = re.sub(r'(?s)^.*\nExamples\n--------\n\n*(.*?\n)[^\n]+\n-----+\n.*$', r'\1', LONGHELP)
 EXAMPLES = re.sub(r'\n\n', r'\n', EXAMPLES)
```

### Comparing `gdb-tools-1.4/duel/parser.py` & `gdb-tools-1.5/duel/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 def hexadecimal(): return RegExMatch(r'0[xX][0-9A-Fa-f]*\b')
 def decimal(): return RegExMatch(r'[1-9][0-9]*\b')
 def octal(): return RegExMatch(r'0[0-7]*\b')
 def char(): return RegExMatch(r"'([^'\\]|"+escapes+")'")
 def string(): return RegExMatch(r'"([^\\"]|'+escapes+')*"')
 def ident(): return RegExMatch(r'[A-Za-z_]\w*')
 def gdbvar(): return RegExMatch(r'\$\w+')
-def underscores(): return RegExMatch(r'_+')
+def underscores(): return RegExMatch(r'_+\b')
 def parens(): return [('(', expression, ')'), ('{', expression, '}')]
 def term21(): return [real, hexadecimal, decimal, octal, char, string,
                       underscores, ident, gdbvar]
 def term20(): return [ term21, parens ]
 def term19a(): return term20, Optional('#', ident)
 def term19(): return term19a, ZeroOrMore([
             (['.', '->', '-->', '@'], term19a),
```

### Comparing `gdb-tools-1.4/gdb_tools.egg-info/PKG-INFO` & `gdb-tools-1.5/gdb_tools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: gdb-tools
-Version: 1.4
+Version: 1.5
 Summary: Various tools to improve the gdb experience
 Home-page: https://github.com/vuvova/gdb-tools
 Author: Sergei Golubchik
 Author-email: vuvova@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Debuggers
@@ -23,16 +21,14 @@
 This repository contains various tools used to make the time spent in gdb more
 comfortable.
 
 To install these tools, first install the modules with
 
     pip install gdb-tools
 
-or with `easy_install` or `python setup.py install [--user]`.
-
 Then you need to import corresponding modules into your gdb. Add, for example,
 
     py import duel
 
 into your `~/.gdbinit`. If you plan to use `pretty_printer` module, I'd
 recommend to put all your python gdb enhancements in `~/.gdb.py` and source it
 from `~/.gdbinit`.
@@ -90,10 +86,8 @@
 `dl head-->next->val` | `val` of each element in a linked list
 `dl head-->(left,right)->val` | `val` of each element in a binary tree
 `dl head-->next[[20]]` | element 20 of list
 `dl #/head-->next` | count elements on a linked list
 `dl #/(head-->next-val>?5)` | count those over 5
 `dl head-->(next!=?head)` | expand cyclic linked list
 
-Or read the [manual](duel/help.md).
-
-
+Or read the [manual](https://github.com/vuvova/gdb-tools/blob/arpeggio/duel/help.md).
```

### Comparing `gdb-tools-1.4/pretty_printer/__init__.py` & `gdb-tools-1.5/pretty_printer/__init__.py`

 * *Files identical despite different names*

