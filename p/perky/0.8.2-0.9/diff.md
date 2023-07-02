# Comparing `tmp/perky-0.8.2.tar.gz` & `tmp/perky-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perky-0.8.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "perky-0.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `perky-0.8.2.tar` & `perky-0.9.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0       39 2023-07-01 02:47:29.152522 perky-0.8.2/.gitignore
--rw-r--r--   0        0        0     1089 2023-07-01 02:47:29.152522 perky-0.8.2/LICENSE
--rw-r--r--   0        0        0    15157 2023-07-01 02:49:14.953392 perky-0.8.2/README.md
--rwxr-xr-x   0        0        0    13692 2023-07-01 02:49:14.953392 perky-0.8.2/perky/__init__.py
--rw-r--r--   0        0        0    13071 2023-07-01 02:47:29.152522 perky-0.8.2/perky/tokenize.py
--rw-r--r--   0        0        0     7146 2023-07-01 02:47:29.152522 perky-0.8.2/perky/transform.py
--rw-r--r--   0        0        0     4422 2023-07-01 02:47:29.152522 perky-0.8.2/perky/utility.py
--rw-r--r--   0        0        0      437 2023-07-01 02:47:29.152522 perky-0.8.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-01 02:47:29.156522 perky-0.8.2/tests/__init__.py
--rw-r--r--   0        0        0        3 2023-07-01 02:47:29.156522 perky-0.8.2/tests/include_dict/included.pky
--rw-r--r--   0        0        0       33 2023-07-01 02:47:29.156522 perky-0.8.2/tests/include_dict/main.pky
--rw-r--r--   0        0        0        1 2023-07-01 02:47:29.156522 perky-0.8.2/tests/include_list/included.pky
--rw-r--r--   0        0        0       27 2023-07-01 02:47:29.156522 perky-0.8.2/tests/include_list/main.pky
--rw-r--r--   0        0        0      106 2023-07-01 02:47:29.156522 perky-0.8.2/tests/include_nested/included.pky
--rw-r--r--   0        0        0      190 2023-07-01 02:47:29.156522 perky-0.8.2/tests/include_nested/main.pky
--rw-r--r--   0        0        0       30 2023-07-01 02:47:29.156522 perky-0.8.2/tests/include_path/dir1/main.pky
--rw-r--r--   0        0        0        3 2023-07-01 02:47:29.156522 perky-0.8.2/tests/include_path/dir2/included.pky
--rw-r--r--   0        0        0      766 2023-07-01 02:47:29.156522 perky-0.8.2/tests/perkytestlib.py
--rw-r--r--   0        0        0      669 2023-07-01 02:49:14.953392 perky-0.8.2/tests/test_all.py
--rw-r--r--   0        0        0      214 2023-07-01 02:47:29.156522 perky-0.8.2/tests/test_input.txt
--rw-r--r--   0        0        0    13636 2023-07-01 02:47:29.156522 perky-0.8.2/tests/test_perky.py
--rw-r--r--   0        0        0     8086 2023-07-01 02:47:29.156522 perky-0.8.2/tests/test_tokenize.py
--rw-r--r--   0        0        0     1263 2023-07-01 02:47:29.156522 perky-0.8.2/tests/test_transform.py
--rw-r--r--   0        0        0     1773 2023-07-01 02:47:29.156522 perky-0.8.2/tests/test_utility.py
--rw-r--r--   0        0        0    15593 1970-01-01 00:00:00.000000 perky-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0       39 2023-07-01 02:47:29.152522 perky-0.9/.gitignore
+-rw-r--r--   0        0        0     1089 2023-07-01 02:47:29.152522 perky-0.9/LICENSE
+-rw-r--r--   0        0        0    16340 2023-07-02 09:40:43.158215 perky-0.9/README.md
+-rwxr-xr-x   0        0        0    12120 2023-07-02 09:25:07.558776 perky-0.9/perky/__init__.py
+-rw-r--r--   0        0        0    13688 2023-07-02 09:07:48.078512 perky-0.9/perky/tokenize.py
+-rw-r--r--   0        0        0     7224 2023-07-02 06:53:52.878781 perky-0.9/perky/transform.py
+-rw-r--r--   0        0        0     4807 2023-07-02 07:03:33.843370 perky-0.9/perky/utility.py
+-rw-r--r--   0        0        0      437 2023-07-01 02:47:29.152522 perky-0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-01 02:47:29.156522 perky-0.9/tests/__init__.py
+-rw-r--r--   0        0        0      860 2023-07-02 01:31:55.665423 perky-0.9/tests/benchmark_perky.py
+-rw-r--r--   0        0        0        3 2023-07-01 02:47:29.156522 perky-0.9/tests/include_dict/included.pky
+-rw-r--r--   0        0        0       33 2023-07-01 02:47:29.156522 perky-0.9/tests/include_dict/main.pky
+-rw-r--r--   0        0        0        1 2023-07-01 02:47:29.156522 perky-0.9/tests/include_list/included.pky
+-rw-r--r--   0        0        0       27 2023-07-01 02:47:29.156522 perky-0.9/tests/include_list/main.pky
+-rw-r--r--   0        0        0      106 2023-07-01 02:47:29.156522 perky-0.9/tests/include_nested/included.pky
+-rw-r--r--   0        0        0      190 2023-07-01 02:47:29.156522 perky-0.9/tests/include_nested/main.pky
+-rw-r--r--   0        0        0       30 2023-07-01 02:47:29.156522 perky-0.9/tests/include_path/dir1/main.pky
+-rw-r--r--   0        0        0        3 2023-07-01 02:47:29.156522 perky-0.9/tests/include_path/dir2/included.pky
+-rw-r--r--   0        0        0      766 2023-07-01 02:47:29.156522 perky-0.9/tests/perkytestlib.py
+-rw-r--r--   0        0        0      669 2023-07-01 02:49:14.953392 perky-0.9/tests/test_all.py
+-rw-r--r--   0        0        0      214 2023-07-01 02:47:29.156522 perky-0.9/tests/test_input.txt
+-rw-r--r--   0        0        0    13013 2023-07-02 09:38:44.201269 perky-0.9/tests/test_perky.py
+-rw-r--r--   0        0        0     8237 2023-07-02 09:07:38.622437 perky-0.9/tests/test_tokenize.py
+-rw-r--r--   0        0        0     2545 2023-07-02 09:36:43.836312 perky-0.9/tests/test_transform.py
+-rw-r--r--   0        0        0     2200 2023-07-02 06:57:38.156560 perky-0.9/tests/test_utility.py
+-rw-r--r--   0        0        0    16774 1970-01-01 00:00:00.000000 perky-0.9/PKG-INFO
```

### Comparing `perky-0.8.2/LICENSE` & `perky-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `perky-0.8.2/README.md` & `perky-0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -154,34 +154,34 @@
 
 The first word after the equals sign is the name of the pragma, in this case `"command"`.
 Everything after the name of the pragma is an argument, with all leading
 and trailing whitespace removed, in this case `"argument here"`.
 
 By default, Perky doesn't have any pragma handlers.  And invoking a pragma
 when Perky doesn't have a handler for it is a runtime error.
-But you can define your own pragma handlers when you call `perky.load()`
-or `perky.loads()`, using a named parameter called `pragmas`.
+But you can define your own pragma handlers when you call `load()`
+or `loads()`, using a named parameter called `pragmas`.
 If you pass in a value for `pragmas`, it must be a mapping
 of strings to functions.
 The string name should be the name of the pragma and must be lowercase.
 The function it maps to will "handle" that pragma, and should match this
 prototype:
 
 `def pragma_fn(parser, argument)`
 
 `parser` is the internal Perky `Parser` object.  `argument` is the
 rest of the relevant line, with leading & trailing whitespace stripped.
 (If the rest of the line was empty, `argument` will be `None`).
 The return value of the pragma function is ignored.
 
 There's currently only one predefined pragma handler, a function called
-`perky.pragma_include()`.  This adds "include statement" functionality
+`pragma_include()`.  This adds "include statement" functionality
 to Perky.  If you call this:
 
-`perky.load(filename, pragmas={'include': perky.pragma_include()})`
+`load(filename, pragmas={'include': pragma_include()})`
 
 then Perky will interpret lines inside `filename` starting with `=include`
 as include statements, using the rest of the line as the name of a file.
 For more information, see `pragma_include()` below.
 
 The rules of pragmas:
 * To invoke a pragma, use `=` as the first non-whitespace character
@@ -199,130 +199,153 @@
 ### Parsing Errors
 
 There are only a few errors possible when parsing a Perky text:
 
 * Obviously, syntax errors, for example:
     * A line in a dict that doesn't have an unquoted equals sign
     * A line in a list that looks like a dict line (`name = value`).
-      (If you want a value like that inside a list, simply put it in quotes.)
+      (If you want a value containing an equals sign inside a list,
+      simply put it in quotes.)
     * A triple-quoted string where any line is outdented past
       the ending triple quotes line.
 * Defining the same value twice in the same dict.  This is flagged
-  as an error, because it could easily be a mistake, and in Python
+  as an error, because it could easily be a mistake, and like Python
   we don't want to let errors pass silently.
 * Using an undefined pragma.
 * Using one of Perky's special tokens as a pragma argument, like
   `{`, `[`, `'''`, `"""`, `[]`, or `{}`.
 
 ### API
 
-#### `def loads(s, *, pragmas=None, root=None) -> o`
+#### `loads(s, *, pragmas=None, root=None)`
 
 Parses a Perky-format string, and returns a container filled
 with the values parsed from that string.
 
+If `pragmas` is not `None`, it must be a mapping of
+strings to pragma handler functions.  Please see the
+**Pragmas** section of the documentation.
+
 If `root` is `None`, `loads` behaves as if you passed in an
 empty `dict`.
 
 If `root` is not `None`, it should be a container, either
 a mutable mapping (`dict`) or a mutable sequence (`list`).
 This affects how the data is parsed; if `root` is a
 mutable mapping, the top level of the Perky file must be
 a "mapping context" (a series of `name=value` lines);
 if `root` is a mutable sequence, the top level of the Perky
 file is assumed to be a "sequence context"
 (a series of `value` lines).
 
-#### `def load(s, *, pragmas=None, encoding='utf-8', root=None) -> o`
+#### `load(filename, *, pragmas=None, root=None)`
 
-Parses a file containing Perky-file-format settings.
+Loads a file containing Perky-file-format settings.
 Returns a dict.
 
-`encoding` specifies the encoding used to decode the
-data read from the file.
+The text in the file must be encoded using
+[UTF-8](https://en.wikipedia.org/wiki/UTF-8).
 
-#### `perky.dumps(d) -> s`
+If `root` is `None`, `loads` behaves as if you passed in an
+empty `dict`.
+
+If `root` is not `None`, it should be a container, either
+a mutable mapping (`dict`) or a mutable sequence (`list`).
+This affects how the data is parsed; if `root` is a
+mutable mapping, the top level of the Perky file must be
+a "mapping context" (a series of `name=value` lines);
+if `root` is a mutable sequence, the top level of the Perky
+file is assumed to be a "sequence context"
+(a series of `value` lines).
+
+If `pragmas` is not `None`, it must be a mapping of
+strings to pragma handler functions.  Please see the
+**Pragmas** section of the documentation.
+
+#### `dumps(d)`
 
 Converts a dictionary to a Perky-file-format string.
 Keys in the dictionary must all be strings.  Values
 that are not dicts, lists, or strings will be converted
 to strings using str.
 Returns a string.
 
-#### `perky.dump(filename, d, *, pragmas=None, encoding="utf-8")`
+#### `dump(filename, d)`
 
 Converts a dictionary to a Perky-file-format string
-using `perky.dump`, then writes it to *filename*.
+using `dump`, then writes it to *filename*.
 
-`encoding` specifies the encoding used to encode the
-data written to the file.
+The text in the file will be encoded using
+[UTF-8](https://en.wikipedia.org/wiki/UTF-8).
 
-#### `perky.pragma_include(include_path=(".",), *, encoding='utf-8')`
+#### `pragma_include(include_path=(".",))`
 
 This function generates a pragma handler that adds "include"
 functionality.  "Including" means lexically inserting one Perky
 file inside another, contextually at the spot where the pragma
 exists.
 
-For example:
+For example, if you ran this:
 
-    d = perky.loads("a=3\n" "=include data.pky\n" "c=5\n",
-        pragmas={"include": perky.pragma_include()},
+    d = loads("a=3\n" "=include data.pky\n" "c=5\n",
+        pragmas={"include": pragma_include()},
         )
 
-If *data.pky* contained the following:
+And *data.pky* in the current directory was readable and
+contained the following text:
 
     b=4
 
 then `d` would be set to the dictionary:
 
     {'a': '3', 'b': '4', 'c': '5'}
 
-`perky.pragma_include()` is not the pragma handler itself;
+`pragma_include()` is not the pragma handler itself;
 it returns a function (a closure) which remembers the `include_path`
 you pass in.  This allows you to use it for multiple pragmas that
 include from different paths, e.g.:
 
     include_dirs = [appdirs.user_data_dir(myapp_name)]
     config_dirs = [appdirs.user_config_dir(myapp_name)]
     pragmas = {
-        'include': perky.pragma_include(include_dirs),
-        'config': perky.pragma_include(config_dirs),
+        'include': pragma_include(include_dirs),
+        'config': pragma_include(config_dirs),
     }
 
-`encoding` specifies the encoding used to decode the
-data read in from the included files.
-
 Notes:
 
 * The pragma handler is context-sensitive; the included
 file will be included as if it was copied-and-pasted replacing
 the pragma line.  Among other things, this means that if the pragma
 is invoked inside a sequence context, the included file must *start*
 in a sequence context.
 
 * When loading the file, the pragma handler will pass in the
-current pragma handlers into `perky.load()`.  Among other things,
+current pragma handlers into `load()`.  Among other things,
 this allows for recursive includes.
 
 * When including inside a dict context, you're explicitly permitted
 to re-define existing keys if they were previously defined in
 another file.
 
 * The default value for `include_path` only searches the
 current directory (`"."`).  If you override the default
 and pass in your own include path, the pragma handler
-won't search the current directory unless you add `"."`
-to the include path yourself.
+won't search the current directory unless you explicitly
+add `"."` to the include path yourself.
+
+* If `pragma_include` can't find the requested file on
+its search path, it raises `FileNotFoundError`.
+
 
 #### Deprecated API
 
 Perky has a "transformation" submodule.
 The idea is, you load a Perky file,
-then run `perky.transform` on that dictionary to
+then run `transform` on that dictionary to
 convert the strings into native values.
 
 These functions are no longer maintained or supported,
 and will be removed before 1.0.
 Why?  This part of Perky was always
 an experiment... and the experiment never really paid
 off.  There are better implementations of this idea,
@@ -331,73 +354,87 @@
 this code in Perky, I encourage you to fork
 off a copy and maintain it yourself.  But I doubt
 anybody is.)
 
 For posterity's sakes, here's documentation of the
 now-deprecated API.
 
-`perky.map(d, fn) -> o`
+`map(d, fn) -> o`
 
 Iterates over a dictionary.  Returns a new dictionary where,
 for every *value*:
   * if it's a dict, replace with a new dict.
   * if it's a list, replace with a new list.
   * if it's neither a dict nor a list, replace with
     `fn(value)`.
 
 The function passed in is called a *conversion function*.
 
-`perky.transform(d, schema, default=None) -> o`
+`transform(d, schema, default=None) -> o`
 
 Recursively transforms a Perky dict into some other
 object (usually a dict) using the provided schema.
 Returns a new dict.
 
 A *schema* is a data structure matching the general expected
 shape of *d*, where the values are dicts, lists, and
-callables.  The transformation is similar to `perky.map()`
+callables.  The transformation is similar to `map()`
 except that individual values will have individual conversion
 functions.  Also, a schema conversion function can be specified
 for any value in *d*, even dicts or lists.
 
 *default* is a default conversion function.  If there is a
 value *v* in *d* that doesn't have an equivalent entry in *schema*,
 and *v* is neither a list nor a dict, and if *default* is
 a callable, *v* will be replaced with `default(v)` in the
 output.
 
-`perky.Required`
+`Required`
 
 Experimental.
 
-`perky.nullable(fn) -> fn`
+`nullable(fn) -> fn`
 
 Experimental.
 
-`perky.const(fn) -> o`
+`const(fn) -> o`
 
 Experimental.
 
 
 ### TODO
 
 * Backslash quoting currently does "whatever your version of Python does".  Perhaps this should be explicit, and parsed by Perky itself?
 
 ### Changelog
 
+**0.9** *2023/07/02*
+
+Breaking API change: removed the `encoding` argument entirely.
+
+* From this point forward, Perky only supports reading and
+  writing files in
+  [UTF-8](https://en.wikipedia.org/wiki/UTF-8).
+  If you need to work with a different encoding, you'll have
+  to handle loading it form and saving it to disk yourself.
+  You'll have to use `loads` and `dumps` to handle converting
+  between Perky string format and native Python objects.
+
+* Optimized Perky some more.  It's roughly 11% faster than 0.8.1.
+
 **0.8.2** *2023/06/30*
 
 * Minor API changes:
 
   - You can now pass an `encoding` keyword argument
     into `pragma_include`.  This is now the only way
     to specify the encoding used to decode files
     loaded from disk by `pragma_include`.
   - Removed the (undocumented) `encoding` attribute
-    of the `perky.Parser` object.
+    of Perky's `Parser` object.
   - Removed the `encoding` parameter for `loads`.
   - The `encoding` parameter for `load` is now only
     used by `load` itself when loading the top-level
     Perky file.
 
 **0.8.1** *2023/06/26*
 
@@ -413,16 +450,16 @@
   your own mapping and sequence objects that *don't* inherit from
   `dict` and `list`.
 * Renamed `PerkyFormatError` to `FormatError`.  The old name is
   supported for now, but please transition to the new name.
   The old name will be removed before 1.0.
 * The "transformation" submodule is now deprecated and unsupported.
   Please either stop using it or fork and maintain it yourself.
-  This includes `perky.map`, `perky.transform`, `perky.Required`,
-  `perky.nullable`, and `perky.const`.
+  This includes `map`, `transform`, `Required`,
+  `nullable`, and `const`.
 * Perky now has a proper unit test suite, which it passes with 100%
   coverage--except for the unsupported `transform` submodule.
 * While working towards 100% coverage, also cleaned up the code
   a little in spots.
 
   - Retooled `LineTokenizer`:
```

### Comparing `perky-0.8.2/perky/__init__.py` & `perky-0.9/perky/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,92 +9,14 @@
 #
 #     Apple ][ = {
 #         bits = 8
 #     }
 #
 # because right now it doesn't.
 
-# YOU NEED more TESTS THAT TEST dump()
-#
-# inside dicts (and similarly without "value =" inside lists)
-#
-# what if ''' or """ appears inside the triple-quoted string?
-#
-# turn if 0 module-level tests into real tests, dude
-#
-# explicit fns for xform schema vs function
-#  * need betterer names
-#
-# More library utility functions to manage
-# perky dict/lists:
-# * recursive "chain map"
-# * recursive merge
-#
-# Ensure you can use multiple Required objects
-# with the same function (e.g. "int")
-#
-# transform exceptions should print a breadcrumb
-# trail so we know where the erroneous value lives
-
-# TESTS NEEDED:
-#
-# make sure a quoted # works as a key
-#
-# ensure that unquoted string names can contain
-#   [ { ''' """ #
-# and unquoted string values can contain all those AND
-#   =
-
-# DONE
-#
-# this should fail:
-#    a = '''
-#       outdenting is fun
-#          '''
-#
-# allow
-#     value = []
-#     value = [ ]
-#     value = {}
-#     value = { }
-#
-# pragma parser:
-#  * handle quoted argument, e.g. =include " file starting with space.h"
-#  * reserve all other perky syntax features, complain if they are used
-#      * """ and '''
-#      * {
-#      * [
-#
-# add pragmas parameter to load / loads
-#     {"prefix": fn(d, suffix)}
-# prefix can be None in which case it's called for every comment line, first
-#   fn is called with current dict and the rest of the line after whitespace
-#     e.g.
-#     load(filename, {"include": includify })
-#   if filename contains the line
-#     #include foo.txt
-#   we'll call
-#     includify(d, "foo.txt")
-#
-#   * idea for pragma: allow it to be a dict entry?
-#     #include = filename
-#     #include = [
-#          ...
-#          ]
-#     I think this is maybe kinda icky.
-#
-# ALLOW EMPTY KEYS
-#       foo =
-# is currently an error, it should be an empty string
-#
-# Per-line callback function (for #include)
-#   * and, naturally, an example callback function
-#     for you to use (aka "#include")
-#
-
 """
 A simple, Pythonic file format.  Same interface as the
 "pickle" module (load, loads, dump, dumps).
 """
 
 # leaving this in is sufficient to meet the binary distribution
 # doc requirement
@@ -118,16 +40,15 @@
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
 IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
 TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE
 OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
 
-
-__version__ = "0.8.2"
+__version__ = "0.9"
 
 import ast
 from collections.abc import MutableMapping, MutableSequence, Sequence
 import os.path
 from os.path import isfile, join, normpath
 import re
 import shlex
@@ -155,25 +76,24 @@
         self.lt = LineTokenizer(s)
         self.pragmas = pragmas or {}
         self.root = root if root is not None else {}
         self.breadcrumbs = []
 
     def _parse_pragma(self, line):
         original_line = line
-        line = line.strip()
-        assert line[0] == '='
-        line = line[1:].strip()
+        # skip the leading '='
+        line = line.lstrip()[1:]
 
         fields = line.split(None, 1)
         pragma = fields[0].lower()
         if len(fields) == 1:
             argument = None
         else:
             argument = fields[1]
-            tokens = list(tokenize(argument))
+            tokens = list(tokenize(pushback_str_iterator(argument)))
             if len(tokens) != 1 or tokens[0][0] != STRING:
                 raise PerkyFormatError(f"Line {self.lt.line_number}: Invalid pragma argument {argument}", tokens, original_line)
             argument = tokens[0][1]
 
         fn = self.pragmas.get(pragma)
         if not fn:
             raise PerkyFormatError(f"Line {self.lt.line_number}: Unknown pragma {pragma}", None, original_line)
@@ -195,102 +115,115 @@
 
     def _read_mapping(self, starting_dict=None):
         d = starting_dict if starting_dict is not None else {}
         self.breadcrumbs.append(d)
 
         keys_seen = set()
 
+        d_setitem = d.__setitem__
+        keys_seen_add = keys_seen.add
+        self_parse_value = self._parse_value
+
         for line_number, line, tokens in self.lt:
             if not tokens:
                 # whitespace line
                 continue
             token, argument = tokens[0]
             if token is EQUALS:
                 self._parse_pragma(line)
                 continue
             if len(tokens) == 1:
-                token, argument = tokens[0]
                 if token is RIGHT_CURLY_BRACE:
                     break
                 if token is COMMENT:
                     continue
-            tokens = [t for t in tokens if t[0] is not WHITESPACE]
 
-            raise_if_false(
-                (2 <= len(tokens) <= 3) and tokens[0][0] is STRING and tokens[1][0] is EQUALS,
-                "Invalid token sequence: in mapping, expected STRING = or STRING == VALUE or }",
-                tokens, line)
-            key = tokens[0][1].strip()
-            raise_if_false(
-                key not in keys_seen,
-                f"Invalid Perky mapping: repeated key {key!r}",
-                tokens, line)
-            keys_seen.add(key)
+            if not (
+                (2 <= len(tokens) <= 3)
+                and (tokens[0][0] is STRING)
+                and (tokens[1][0] is EQUALS)
+                ):
+                raise FormatError(
+                    "Invalid token sequence: in mapping, expected STRING = or STRING == VALUE or }",
+                    tokens, line)
+
+            key = tokens[0][1]
+            if key in keys_seen:
+                raise FormatError(
+                    f"Invalid Perky mapping: repeated key {key!r}",
+                    tokens, line)
+            keys_seen_add(key)
             if len(tokens) == 3:
-                value = self._parse_value(tokens[2])
+                value = self_parse_value(tokens[2])
             else:
                 value = ""
-            d[key] = value
+            # d[key] = value
+            d_setitem(key, value)
 
         self.breadcrumbs.pop()
         return d
 
     def _read_sequence(self, starting_list=None):
         l = starting_list if starting_list is not None else []
+        l_append = l.append
+        self_parse_value = self._parse_value
         self.breadcrumbs.append(l)
         for line_number, line, tokens in self.lt:
             if not tokens:
                 # blank line
                 continue
             token, argument = tokens[0]
             if token is EQUALS:
                 self._parse_pragma(line)
                 continue
-            raise_if_false(
-                len(tokens) == 1,
-                "Invalid token sequence: in sequence, expected one token",
-                tokens, line)
-            token, argument = tokens[0]
+            if len(tokens) != 1:
+                raise FormatError(
+                    "Invalid token sequence: in sequence, expected one token",
+                    tokens, line)
             if token is RIGHT_SQUARE_BRACKET:
                 break
             if token is COMMENT:
                 continue
-            value = self._parse_value(tokens[0])
-            l.append(value)
+            value = self_parse_value(tokens[0])
+            l_append(value)
         self.breadcrumbs.pop()
         return l
 
     def _read_textblock(self, marker):
         l = []
-        while self.lt:
-            line_number, line = self.lt.next_line()
+        l_append = l.append
+        lt = self.lt
+        next_line = self.lt.next_line
+        while lt:
+            line_number, line = next_line()
             line = line.rstrip()
             stripped = line.lstrip()
             if stripped == marker:
                 break
-            l.append(line)
+            l_append(line)
 
         prefix = line.partition(stripped)[0]
+        l2 = []
+        l2_append = l2.append
+        len_prefix = len(prefix)
         if prefix:
             # detect this error:
             #    a = '''
             #       outdenting sure is fun!
             #          '''
             for line in l:
-                raise_if_false(
-                    # line must either be empty or start with our prefix
-                    (not line) or line.startswith(prefix),
-                    "Format error: malformed line triple-quoted block",
-                    None, line)
-
-        s = "\n".join(line for line in l)
-        # this one line does all the
-        # heavy lifting in textwrap.dedent()
-        s = re.sub(r'(?m)^' + prefix, '', s)
-        return s
+                # line must either be empty or start with our prefix
+                if line and (not line.startswith(prefix)):
+                    raise FormatError(
+                        "Format error: malformed line triple-quoted block",
+                        None, line)
+                line2 = line[len_prefix:]
+                l2_append(line2)
+
+        return "\n".join(l2)
 
     def parse(self):
         if isinstance(self.root, MutableMapping):
             return self._read_mapping(self.root)
         if isinstance(self.root, MutableSequence):
             return self._read_sequence(self.root)
         raise TypeError(f"root {self.root} is neither MutableMapping nor MutableSequence, don't know how to fill it")
@@ -349,15 +282,15 @@
             ):
             s = s.replace(bad, good)
         return quote + s + quote
 
     def serialize(self, d):
         for name, value in d.items():
             if not isinstance(name, str):
-                raise TypeError("keys in Perky dicts must always be strings")
+                raise TypeError(f"keys in Perky dicts must always be strings, not {name!r}")
             self.line = self.quoted_string(name) + " = "
             self.serialize_value(value)
 
     def serialize_dict(self, value):
         self.newline("{")
         self.indent += 1
         self.serialize(value)
@@ -386,69 +319,73 @@
     def serialize_value(self, value):
         if isinstance(value, MutableMapping):
             return self.serialize_dict(value)
         if isinstance(value, MutableSequence):
             return self.serialize_list(value)
 
         if isinstance(value, bytes):
-            raise TypeError("Perky can't serialize bytes values, please decode to str")
+            raise TypeError(f"Perky can't serialize bytes value {value!r}, please decode to str")
 
         if not isinstance(value, str):
             value = str(value)
         if '\n' in value:
             return self.serialize_textblock(value)
-        if value == value.strip() and "".join(value.split()).isalnum():
+        if (value == value.strip()) and "".join(value.split()).isalnum():
             self.newline(value)
             return
         return self.serialize_quoted_string(value)
 
 
 @export
 def loads(s, *, pragmas=None, root=None):
     p = Parser(s, pragmas=pragmas, root=root)
     d = p.parse()
     return d
 
 @export
+def load(filename, *, pragmas=None, root=None):
+    with open(filename, "rt", encoding="utf-8") as f:
+        return loads(f.read(), pragmas=pragmas, root=root)
+
+@export
 def dumps(d):
     s = Serializer()
     s.serialize(d)
     return s.dumps()
 
 
 @export
-def load(filename, *, pragmas=None, encoding="utf-8", root=None):
-    with open(filename, "rt", encoding=encoding) as f:
-        return loads(f.read(), pragmas=pragmas, root=root)
-
-@export
-def dump(filename, d, *, encoding="utf-8"):
+def dump(filename, d):
     s = Serializer()
     s.serialize(d)
-    with open(filename, "wt", encoding=encoding) as f:
+    with open(filename, "wt", encoding="utf-8") as f:
         f.write(s.dumps())
 
 
 @export
-def pragma_include(include_path=(".",), *, encoding='utf-8'):
-    assert isinstance(include_path, Sequence)
-    assert not isinstance(include_path, str)
-    assert all(isinstance(s, str) for s in include_path)
+def pragma_include(include_path=(".",)):
+    include_path_ok = (
+        isinstance(include_path, Sequence)
+        and (not isinstance(include_path, str))
+        and all(isinstance(s, str) for s in include_path)
+        )
+    if not include_path_ok:
+        raise TypeError(f"include_path must be a sequence of strings, not {include_path!r}")
     include_path = tuple(include_path)
     def pragma_include(parser, filename):
         leaf = parser.breadcrumbs[-1]
         leaf_is_list = isinstance(parser.breadcrumbs[-1], list)
         subroot = [] if leaf_is_list else {}
         for directory in include_path:
             path = normpath(join(directory, filename))
             if isfile(path):
                 break
         else:
             raise FileNotFoundError(filename)
-        load(path, pragmas=parser.pragmas, encoding=encoding, root=subroot)
+        load(path, pragmas=parser.pragmas, root=subroot)
         merged = merge_dicts_and_lists(leaf, subroot)
         # print(f"\n\nXXX merge_dicts_and_lists({leaf=}, {subroot=}) -> {merged=}\n\n")
         leaf.clear()
         if isinstance(leaf, list):
             leaf.extend(merged)
         else:
             leaf.update(merged)
```

### Comparing `perky-0.8.2/perky/tokenize.py` & `perky-0.9/perky/tokenize.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,33 +6,30 @@
 #
 
 import ast
 import collections
 import sys
 
 
-token_first_characters = set()
 c_to_tokens = collections.defaultdict(list)
-s_to_token = {}
 tokens = {}
-token_to_name = {}
+# token_to_name = {}
 
 
 def token(s, description):
-    base = description.strip().lower().replace(" ", "_")
+    base = description.replace(" ", "_")
     token = "<" + base + "_token>"
     name = base.upper()
 
     tokens[token] = (name, s)
-    token_to_name[token] = name
+    # token_to_name[token] = name
 
     if s:
         value = (token, s)
         c_to_tokens[s[0]].append(value)
-        s_to_token[s] = value
 
     return token
 
 # abstract tokens
 WHITESPACE            = token(None, 'whitespace')
 STRING                = token(None, 'string')
 COMMENT               = token(None, 'comment')
@@ -46,60 +43,73 @@
 SINGLE_QUOTE          = token("'", 'single quote')
 DOUBLE_QUOTE          = token('"', 'double quote')
 TRIPLE_SINGLE_QUOTE   = token("'''", 'triple single quote')
 TRIPLE_DOUBLE_QUOTE   = token('"""', 'triple double quote')
 EMPTY_CURLY_BRACES    = token('{}', 'empty curly braces')
 EMPTY_SQUARE_BRACKETS = token('[]', 'empty square brackets')
 
-single_quote_tokens = set((SINGLE_QUOTE, DOUBLE_QUOTE))
-triple_quote_tokens = set((TRIPLE_SINGLE_QUOTE, TRIPLE_DOUBLE_QUOTE))
-left_bracket_tokens = set((LEFT_SQUARE_BRACKET, LEFT_CURLY_BRACE))
-left_bracket_to_right_bracket = {
-    '[': ']',
-    '{': '}',
-}
-left_bracket_to_empty_bracket_token = {
-    '[': (EMPTY_SQUARE_BRACKETS, '[]'),
-    '{': (EMPTY_CURLY_BRACES, '{}'),
-}
-
 non_quoting_operators = set(c for c in c_to_tokens if c not in ('"', "'"))
+# non_quoting_operators = "".join(c for c in c_to_tokens if c not in ('"', "'"))
 
-# sort tokens in c_to_tokens by length, longest first
+# c_to_tokens maps characters to lists of tokens that start with that charcter.
+# It's always true that there are either exactly zero, one, or two tokens that
+# start with any particular character.  If there are two, it's always true that
+# the two tokens are different lengths, and the shorter token is exactly one
+# character long.
+#
+# Sort the list of tokens by length, longest first, and also verify these
+# invariants.
 for value in c_to_tokens.values():
-    value.sort(key=lambda o:len(o[0]), reverse=True)
-    # the parsing code is special-cased to assume:
-    #   * there are either one or two possible tokens for each initial character
-    #   * if there are two, the first token is always multiple characters
-    #     and the second token is always a single character
-    assert 1 <= len(value) <= 2
+    length = len(value)
+    assert 1 <= length <= 2
     if len(value) == 2:
-        assert len(value[0][1]) > 1, f"unexpected value {value}"
-        assert len(value[1][1]) == 1, f"unexpected value {value}"
+        value.sort(key=lambda o:len(o[0]), reverse=True)
+        assert len(value[0][1]) > 1, f"unexpected value {value}, should be a token of 2 or more characters"
+        assert len(value[1][1]) == 1, f"unexpected value {value}, should be a token that is a single character"
+
+_sentinel = object()
 
 class pushback_str_iterator:
     """
     A specialized iterator for strings that permits a
     form of rewinding: while iterating over a string,
     you can "push" strings back onto the iterator,
     which will be yielded first.  (The pushed-back
     strings go on a stack, and are LIFO.)  Technically
     you can "push" any string, though in practice Perky
     only pushes back values yielded by the iterator.
     """
 
     # look! a go-faster stripe!
-    __slots__ = ('i', 'stack')
+    __slots__ = ('i', 'stack', 'push_c')
 
     def __init__(self, s):
         # iterate over s
         self.i = iter(s)
+
         # but maintain a stack for pushbacks
         self.stack = []
 
+        # Optimized version of push that only handles strings of length 1.
+        # Most of the time, Perky pushes individual characters, and push_c
+        # is much faster than push.  This optimization brings a measurable
+        # performance gain.  (Between this and switching to slots, I saw a
+        # 22% *overall* improvement in Perky!)
+        #
+        # This method would be unsafe for public use; it doesn't validate
+        # its input.  Calling push_c with something besides a length-1 string
+        # will result in it yielding garbage.  But pushback_str_iterator
+        # is an internal data structure, unsupported for public use, and
+        # Perky is careful.  So it's fine.
+        self.push_c = self.stack.append
+
+    def reset(self, s):
+        self.i = iter(s)
+        self.stack.clear()
+
     def __repr__(self):
         return f'<pushback i={self.i} stack={list(self.stack)}>'
 
     def push(self, s):
         """
         Pushes a string (or list) back onto the iterator.
 
@@ -109,66 +119,47 @@
             i.push('abcde')
             for c in i:
                 print(c)
 
         prints 'X', 'a', 'b', 'c', 'd', 'e', and 'Y'
         in that order.
         """
-        # assert isinstance(s, (str, list)), f"expected str or list, got s={s} (type(s)={type(s)})"
         if len(s) == 1:
-            self.stack.append(s[0])
+            self.push_c(s[0])
             return
         self.stack.extend(reversed(s))
 
-    def push_c(self, c):
-        """
-        Optimized version of push that only handles strings of length 1.
-        Most of the time, Perky pushes individual characters, and push_c
-        is much faster than push.  This optimization brings a measurable
-        performance gain.  (Between this and switching to slots, I saw a
-        22% *overall* improvement in Perky!)
-
-        This method would be unsafe for public use; it doesn't validate
-        its input.  Calling push_c with something besides a length-1 string
-        will result in it yielding garbage.  But pushback_str_iterator
-        is an internal data structure, unsupported for public use, and
-        Perky is careful.  So it's fine.
-        """
-        # assert isinstance(c, str) and (len(c) == 1), f"expected str of len 1, got c={c} (type(c)={type(c)})"
-        self.stack.append(c)
-
     def __next__(self):
         if self.stack:
-            x = self.stack.pop()
-            return x
+            s = self.stack.pop()
+            return s
         if not self.i:
             raise StopIteration
         try:
-            x = next(self.i)
-            return x
+            s = next(self.i)
+            return s
         except StopIteration as e:
             self.i = None
             raise e
 
     def __iter__(self):
         return self
 
     def __bool__(self):
         if self.stack:
             return True
         if not self.i:
             return False
 
-        try:
-            c = next(self.i)
-            self.push_c(c)
-            return True
-        except StopIteration:
+        c = next(self.i, _sentinel)
+        if c is _sentinel:
             self.i = None
             return False
+        self.push_c(c)
+        return True
 
     def drain(self):
         """
         Return all remaining characters as a string.
         """
         if self.stack:
             s = "".join(reversed(self.stack))
@@ -183,197 +174,213 @@
             else:
                 s = t
             self.i = None
 
         return s
 
 
-def tokenize(s, suppress_whitespace=True):
+def tokenize(i, suppress_whitespace=True):
     """
     Tokenizer for individual lines of a Perky file.
     Hand-written, designed specifically for Perky syntax.
 
+    i should be a pushback_str_iterator iterating over the
+    string you want tokenized.
+
     This function is a generator; it yields tokens from
     the line until the line is exhausted.
 
-    If suppres_whitespace is true (the default),
+    If suppress_whitespace is true (the default),
     this generator will not yield WHITESPACE tokens.
     (Trailing whitespace is generally discarded anyway.)
     """
 
-    # assert "\n" not in s
-
-    i = pushback_str_iterator(s)
-
-    def parse_unquoted_string():
-        """
-        Parse an unquoted string.
-        Note that it *is* permitted to have spaces.
-
-        Returns the unquoted string.
-        If there were no characters to be read, returns an
-        empty string.
-        Note that trailing whitespace is stripped.
-        (If you want trailing whitespace preserved,
-        use a quoted string.)
-
-        Stops the unquoted string at EOL, or the first
-        character used in Perky syntax (=, {, [, etc).
-        (If you need to use one of those inside your string,
-        use a quoted string.)
-
-        """
-        buffer = []
-        for c in i:
-            if c in non_quoting_operators:
-                i.push_c(c)
-                break
-            buffer.append(c)
-        return "".join(buffer).rstrip()
-
-    def parse_quoted_string(quote):
-        """
-        Parse a quoted string.  The ending quote
-        must match the starting quote character
-        passed in.  Handles all the Python escape
-        sequences: all the single-character ones,
-        octal, and the extra-special x u U N ones.
-        """
-        buffer = [quote]
-        backslash = False
-        for c in i:
-            if c == '\\':
-                backslash = not backslash
-                continue
-            if (c == quote) and (not backslash):
-                buffer.append(quote)
-                break
-            if backslash:
-                buffer.append('\\')
-            buffer.append(c)
-            backslash = False
+    # cache looked-up methods in fast locals
+    i_push = i.push
+    i_push_c = i.push_c
+
+    buffer = []
+    buffer_append = buffer.append
+    buffer_clear = buffer.clear
 
-        return ast.literal_eval("".join(buffer))
+    empty_string_join = "".join
 
     for c in i:
         if c.isspace():
-            whitespace = [c]
+            if buffer:
+                buffer_clear()
+            buffer_append(c)
             for c in i:
                 if not c.isspace():
-                    i.push_c(c)
+                    i_push_c(c)
                     break
-                whitespace.append(c)
+                buffer_append(c)
             if not suppress_whitespace:
-                yield WHITESPACE, "".join(whitespace)
+                yield (WHITESPACE, empty_string_join(buffer))
             continue
 
-        t = c_to_tokens.get(c, None)
-        if t:
-            if len(t) > 1:
-                multi, single = t
+        candidates = c_to_tokens.get(c, None)
+        if candidates:
+            if len(candidates) == 1:
+                t = candidates[0]
+            else:
+                multi, single = candidates
                 multi_string = multi[1]
-                token = [c]
+                if buffer:
+                    buffer_clear()
+                buffer_append(c)
                 for c in i:
-                    token.append(c)
-                    if len(token) == len(multi_string):
+                    buffer_append(c)
+                    if len(buffer) == len(multi_string):
                         break
-                token = "".join(token)
+                token = empty_string_join(buffer)
                 if token == multi_string:
                     t = multi
                 else:
                     t = single
-                    i.push(token)
+                    i_push(token)
                     # now throw away c, we just pushed it again
                     c = next(i)
-            else:
-                t = t[0]
 
             token, s = t
 
-            if token == NUMBER_SIGN:
-                yield COMMENT, i.drain()
+            if token is NUMBER_SIGN:
+                yield (COMMENT, i.drain())
                 return
 
-            if token in single_quote_tokens:
-                yield STRING, parse_quoted_string(c)
+            if (token is SINGLE_QUOTE) or (token is DOUBLE_QUOTE):
+                # Parse a quoted string.  The ending quote
+                # must match the starting quote character
+                # passed in.  Handles all the Python escape
+                # sequences: all the single-character ones,
+                # octal, and the extra-special x u U N ones.
+                if buffer:
+                    buffer_clear()
+                quote = c
+                buffer_append(quote)
+                backslash = False
+                for c in i:
+                    if c == '\\':
+                        backslash = not backslash
+                        continue
+                    if backslash:
+                        buffer_append('\\')
+                    elif c == quote:
+                        buffer_append(quote)
+                        break
+                    buffer_append(c)
+                    backslash = False
+
+                s = ast.literal_eval(empty_string_join(buffer))
+                yield (STRING, s)
                 continue
 
-            if token in triple_quote_tokens:
+            if (token is TRIPLE_SINGLE_QUOTE) or (token is TRIPLE_DOUBLE_QUOTE):
                 # triple quote MUST be last thing on line (except possibly-ignored trailing whitespace)
                 trailing = i.drain()
                 if trailing and not trailing.isspace():
                     raise ValueError("tokenizer found triple-quote followed by non-whitespace string " + repr(trailing))
                 yield t
-                # don't yield trailing whitespace here--we never do anywhere else!
-                # if trailing and not suppress_whitespace:
-                #     yield WHITESPACE, trailing
                 return
 
-            if token in left_bracket_tokens:
+            token_is_left_curly_brace = token is LEFT_CURLY_BRACE
+            if token_is_left_curly_brace or (token is LEFT_SQUARE_BRACKET):
                 # handle flattening [] and [   ] into a EMPTY_SQUARE_BRACKETS token
                 # (and similarly for {} and { } and EMPTY_CURLY_BRACES)
-                right_bracket = left_bracket_to_right_bracket[s]
-                characters = []
+                if token_is_left_curly_brace:
+                    right_bracket = '}'
+                    empty_brackets = (EMPTY_CURLY_BRACES, '{}')
+                else:
+                    right_bracket = ']'
+                    empty_brackets = (EMPTY_SQUARE_BRACKETS, '[]')
+                if buffer:
+                    buffer_clear()
                 for c in i:
                     if c.isspace():
-                        characters.append(c)
+                        buffer_append(c)
                         continue
                     if c == right_bracket:
-                        t = left_bracket_to_empty_bracket_token[s]
+                        t = empty_brackets
                         break
-                    i.push_c(c)
-                    i.push(characters)
+                    i_push_c(c)
+                    i_push(buffer)
                     break
 
             yield t
             continue
 
-        i.push_c(c)
-        s = parse_unquoted_string()
-        yield STRING, s
+        # Parse an unquoted string.
+        # Note that it *is* permitted to have spaces.
+        #
+        # Returns the unquoted string.
+        # If there were no characters to be read, returns an
+        # empty string.
+        # Note that trailing whitespace is stripped.
+        # (If you want trailing whitespace preserved,
+        # use a quoted string.)
+        #
+        # Stops the unquoted string at EOL, or the first
+        # character used in Perky syntax (=, {, [, etc).
+        # (If you need to use one of those inside your string,
+        # use a quoted string.)
+        if buffer:
+            buffer_clear()
+        i_push_c(c)
+        for c in i:
+            if c in non_quoting_operators:
+                i_push_c(c)
+                break
+            buffer_append(c)
+        s = empty_string_join(buffer).rstrip()
+        yield (STRING, s)
 
 
 class LineTokenizer:
     """
     A simple tokenizing iterator for Perky.
     It's line-oriented; you can get the next
     line either as a string, or as a sequence
     of tokens.
     """
 
+    # go-faster stripe!
+    __slots__ = ('_lines', 'suppress_whitespace', 'waiting', 'line_number', '_repr', 'i')
+
     def __init__(self, s, suppress_whitespace=True):
         lines = s.split("\n")
         self._lines = enumerate(lines, 1)
         self.suppress_whitespace = suppress_whitespace
         self.waiting = None
         self.line_number = 0
 
         repr_lines = str(lines[:5])
         if len(repr_lines) > 50:
             repr_lines = repr_lines[:47] + "..."
         self._repr = f"<LineTokenizer {{self.line_number}}/{len(lines)} lines {repr_lines}>"
 
+        self.i = pushback_str_iterator('')
+
     def __repr__(self):
         return self._repr.format(self=self)
 
     def __iter__(self):
         return self
 
     def __bool__(self):
         if self.waiting is not None:
             return True
         if self._lines is None:
             return False
 
-        try:
-            self.waiting = next(self._lines)
-            return True
-        except StopIteration:
+        result = next(self._lines, _sentinel)
+        if result is _sentinel:
             self._lines = self.waiting = None
             return False
+        self.waiting = result
+        return True
 
     def next_line(self):
         """
         Returns the 2-tuple
             line_number, line
 
         If the iterator is exhausted,
@@ -384,17 +391,16 @@
 
         if self.waiting is not None:
             t = self.waiting
             self.waiting = None
         else:
             if self._lines is None:
                 return failure
-            try:
-                t = next(self._lines)
-            except StopIteration as e:
+            t = next(self._lines, _sentinel)
+            if t is _sentinel:
                 self._lines = None
                 return failure
 
         self.line_number = t[0]
         return t
 
     def tokens(self):
@@ -410,23 +416,24 @@
 
         if self.waiting is not None:
             t = self.waiting
             self.waiting = None
         else:
             if self._lines is None:
                 return failure
-            try:
-                t = next(self._lines)
-            except StopIteration as e:
+            t = next(self._lines, _sentinel)
+            if t is _sentinel:
                 self._lines = None
                 return failure
 
         line_number, line = t
         self.line_number = line_number
-        tokens = list(tokenize(line, suppress_whitespace=self.suppress_whitespace))
+        i = self.i
+        i.reset(line)
+        tokens = list(tokenize(i, suppress_whitespace=self.suppress_whitespace))
         return (line_number, line, tokens)
 
     def __next__(self):
         t = self.tokens()
         if t == (None, None, None):
             raise StopIteration()
         return t
```

### Comparing `perky-0.8.2/perky/transform.py` & `perky-0.9/perky/transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,47 +132,47 @@
     if isinstance(o, list):
         return [map(value, fn) for value in o]
     return fn(o)
 
 
 def _transform(o, schema, default):
     if isinstance(schema, dict):
-        raise_if_false(
+        raise_format_error_if_false(
             isinstance(o, dict),
             f"schema mismatch: schema is a dict, o should be a dict but is {o!r}",
             None, None)
         result = {}
         for name, value in o.items():
             handler = schema.get(name)
             if handler:
                 value = _transform(value, handler, default)
             elif default:
                 value = default(value)
             result[name] = value
         return result
     if isinstance(schema, list):
-        raise_if_false(
+        raise_format_error_if_false(
             isinstance(o, list) and (len(schema) == 1),
             f"schema mismatch: schema is a list, o should be a list but is {o!r}",
             None, None)
         handler = schema[0]
         return [_transform(value, handler, default) for value in o]
-    raise_if_false(
+    raise_format_error_if_false(
         callable(schema),
         f"schema mismatch: schema values must be dict, list, or callable, got {schema!r}",
         None, None)
     return schema(o)
 
 @export
 def transform(o, schema, default=None):
-    raise_if_false(
+    raise_format_error_if_false(
         isinstance(o, dict),
         "schema must be a dict",
         None, None)
-    raise_if_false(
+    raise_format_error_if_false(
         (not default) or callable(default),
         "default must be either None or a callable",
         None, None)
     return _transform(o, schema, default)
 
 
 constmap = {
@@ -217,15 +217,15 @@
             self.head.append(name + "[")
             self.tail.append(']')
             self.crawl(value[0])
             self.head.pop()
             self.tail.pop()
             return
 
-        raise_if_false(
+        raise_format_error_if_false(
             callable(value),
             "Malformed schema error: " + repr(name) + " = " + repr(value) + ", value is not dict, list, or callable!",
             None, None)
         required = getattr(value, "_perky_required", None)
         if required:
             s = "".join(self.head) + name + "".join(reversed(self.tail))
             required[0] = s
```

### Comparing `perky-0.8.2/perky/utility.py` & `perky-0.9/perky/utility.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from collections.abc import Mapping, Sequence
 
 
 class FormatError(Exception):
     def __init__(self, message, tokens=None, line=None):
         self.message = message
         if tokens:
-            self.tokens = ''.join(t[1] for t in tokens)
+            self.tokens = ' '.join(f'"{t[1]}"' for t in tokens)
         else:
             self.tokens = tokens
         self.line = line
 
     def __strings_for_repr__(self):
         strings = [f"{self.__class__.__name__} {self.message!r}"]
         if self.tokens is not None:
@@ -31,23 +31,24 @@
     def __str__(self):
         return "\n".join(self.__strings_for_repr__())
 
 # old name
 PerkyFormatError = FormatError
 
 
-def raise_if_false(expr, message, tokens, line):
+def raise_format_error_if_false(expr, message, tokens, line):
     if not expr:
         raise FormatError(message, tokens, line)
 
 
 def _merge_dicts_and_lists_recurse_dict(roots):
     sentinel = object()
     for root in roots:
-        assert isinstance(root, Mapping)
+        if not isinstance(root, Mapping):
+            raise TypeError(f"roots must be an iterable of Mapping objects, this root is not a Mapping {root!r}")
 
     d = {}
 
     # why not just iterate over roots?
     # consider merging this list of root dicts:
     #   [
     #   {'a': 1},
@@ -73,27 +74,29 @@
                 # only merge once!
                 continue
             subroots = [value]
             for root in roots:
                 value = root.get(key, sentinel)
                 if value is sentinel:
                     continue
-                assert isinstance(value, value_type)
+                if not isinstance(value, value_type):
+                    raise TypeError(f"value must be {value_type.__name__}, not {value!r}")
                 subroots.append(value)
             if is_mapping:
                 value = _merge_dicts_and_lists_recurse_dict(subroots)
             else:
                 value = _merge_dicts_and_lists_recurse_list(subroots)
             d[key] = value
     return d
 
 def _merge_dicts_and_lists_recurse_list(roots):
     l = []
     for root in roots:
-        assert isinstance(root, Sequence) and not isinstance(root, str)
+        if (not isinstance(root, Sequence)) or isinstance(root, str):
+            raise TypeError(f"roots must be an iterable of Sequence objects that aren't strings, found root {root!r}")
         l.extend(root)
     return l
 
 def merge_dicts_and_lists(*roots):
     """
     Takes a sequence of homogenous roots
     (either Mapping or Sequence objects, with the same
@@ -123,15 +126,16 @@
     """
     if not roots:
         return None
 
     root0 = roots[0]
     is_sequence = isinstance(root0, Sequence) and not isinstance(root0, str)
     is_mapping = isinstance(root0, Mapping)
-    assert is_sequence or is_mapping, f"expected t to be Mapping or Sequence, type of t is {type(t)}, t is {t!r}"
+    if not (is_sequence or is_mapping):
+        raise TypeError(f"expected roots to be Mapping or Sequence, first root is {root0!r}, type {type(root0)}")
 
     if len(roots) == 1:
         if is_mapping:
             return dict(root0)
         return list(root0)
 
     if is_mapping:
```

### Comparing `perky-0.8.2/tests/perkytestlib.py` & `perky-0.9/tests/perkytestlib.py`

 * *Files identical despite different names*

### Comparing `perky-0.8.2/tests/test_all.py` & `perky-0.9/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `perky-0.8.2/tests/test_perky.py` & `perky-0.9/tests/test_perky.py`

 * *Files 3% similar despite different names*

```diff
@@ -201,14 +201,22 @@
             s = str(e)
             r = repr(e)
             self.assertIn('Format error: malformed line triple-quoted block', s)
             self.assertIn('Format error: malformed line triple-quoted block', r)
             self.assertIn('hello', s)
             self.assertIn('hello', r)
 
+    def test_bad_mapping(self):
+        with self.assertRaises(perky.FormatError):
+            perky.loads("a = = 5")
+
+    def test_bad_sequence(self):
+        with self.assertRaises(perky.FormatError):
+            perky.loads("a = [\n  1\n  2\n  x = y\n]")
+
     def test_undefined_pragma(self):
         line = '=balloon'
         try:
             perky.loads(line)
         except perky.FormatError as e:
             self.assertEqual(None, e.tokens)
             self.assertIn('unknown pragma', str(e).lower())
@@ -219,15 +227,16 @@
 
     def test_pragma_format_error(self):
         bad_pragma = '[{=}]'
         line = f'=pragma {bad_pragma}'
         try:
             perky.loads(line)
         except perky.FormatError as e:
-            self.assertEqual(bad_pragma, e.tokens)
+            tokens = ' '.join(f'"{c}"' for c in bad_pragma)
+            self.assertEqual(tokens, e.tokens)
             self.assertIn('invalid pragma argument', str(e).lower())
             self.assertEqual(line, e.line)
             return
         if 1: # pragma: no cover
             self.assertEqual(True, False, "exception not raised!")
 
     def test_parse_trip_repeated_key_error(self):
@@ -237,41 +246,22 @@
         # redefine a key in a different (as in, =include'd) file.
         # test_perky_include_nested tests redefining in different files.
         with self.assertRaises(perky.PerkyFormatError):
             perky.loads("a=3\na=5")
 
 # TODO: check if there are any other formats that would cause a failure
     def test_read_file(self):
-        test_input = perky.load("test_input.txt", encoding="utf-8")
+        test_input = perky.load("test_input.txt")
         self.assertIsNotNone(self, test_input)
 
-    def test_transform_dict(self):
-        o = {'a': '3', 'b': '5.0', 'c': ['1', '2', 'None', '3'], 'd': {'e': 'f', 'g': 'True'}}
-        schema = {'a': int, 'b': float, 'c': [perky.nullable(int)], 'd': {'e': str, 'g': perky.const}}
-        test_func = perky.transform(o, schema)
-        expected_dict = {'a': 3, 'b': 5.0, 'c': [1, 2, None, 3], 'd': {'e': 'f', 'g': True}}
-        self.assertEqual(expected_dict, test_func)
-
-    def test_transform_type_mismatch(self):
-        o = {'a': '3', 'b': '5.0', 'c': ['1', '2', 'None', '3'], 'd': {'e': 'f', 'g': 'True'}}
-        schema = [{'a': int, 'b': float, 'c': [perky.nullable(int)], 'd': {'e': str, 'g': perky.const}}]
-        with self.assertRaises(perky.PerkyFormatError):
-            perky.transform(o, schema)
-
-    def test_transform_bad_obj(self):
-        o2 = {'a': '44'}
-        schema = [{'a': int, 'b': float, 'c': [perky.nullable(int)], 'd': {'e': str, 'g': perky.const}}]
-        with self.assertRaises(perky.PerkyFormatError):
-            perky.transform(o2, schema)
-
-    def test_transform_none(self):
-        o = None
-        schema = {'a': int, 'b': float, 'c': [perky.nullable(int)], 'd': {'e': str, 'g': perky.const}}
-        with self.assertRaises(perky.PerkyFormatError):
-            perky.transform(o, schema)
+    def test_perky_include_bad_include_path(self):
+        with self.assertRaises(TypeError):
+            perky.load("include_list/main.pky", root=[], pragmas={'include':perky.pragma_include( 3.14159 )})
+        with self.assertRaises(TypeError):
+            perky.load("include_list/main.pky", root=[], pragmas={'include':perky.pragma_include( (3.14159,) )})
 
     def test_perky_include_list(self):
         with pushd("include_list"):
             root = perky.load("main.pky", root=[], pragmas={'include':perky.pragma_include()})
         self.assertEqual(root, list("abcd"))
 
     def test_perky_include_dict(self):
```

### Comparing `perky-0.8.2/tests/test_tokenize.py` & `perky-0.9/tests/test_tokenize.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,62 +22,67 @@
 from perky.tokenize import SINGLE_QUOTE
 from perky.tokenize import DOUBLE_QUOTE
 from perky.tokenize import TRIPLE_SINGLE_QUOTE
 from perky.tokenize import TRIPLE_DOUBLE_QUOTE
 from perky.tokenize import EMPTY_CURLY_BRACES
 from perky.tokenize import EMPTY_SQUARE_BRACKETS
 
-from perky.tokenize import token_to_name, tokenize, LineTokenizer
+from perky.tokenize import LineTokenizer, pushback_str_iterator, tokenize
 
+def token_to_name(token):
+    result = perky.tokens.get(token, None)
+    if result is None:
+        return None
+    return result[0]
 
 want_print = False
 
 
 class TestTokenizer(PerkyTestCase):
 
     def test_tokenizer(self):
 
         def _test(s, tokens_and_values, suppress_whitespace):
             tokens = []
             values = []
             tokens_with_values = set((STRING, COMMENT))
             expect_token = True
             for t in tokens_and_values:
-                is_token = token_to_name.get(t)
+                is_token = token_to_name(t)
                 if expect_token:
                     self.assertTrue(is_token, "expected token, got " + str(t))
                     tokens.append(t)
                     if t in tokens_with_values:
                         expect_token = False
                 else:
                     values.append(t)
                     expect_token = True
             if want_print: # pragma: nocover
                 if suppress_whitespace is None:
                     suffix = ""
                 else:
                     modifier = "suppressing" if suppress_whitespace else "keeping"
                     suffix = f", {modifier} whitespace tokens"
-                print(f"test #{test_number}{suffix}:\n  input:\n\t", repr(s), "\n  should match:\n\t", " ".join(x if x in token_to_name else repr(x) for x in tokens_and_values), end="\n\n")
+                print(f"test #{test_number}{suffix}:\n  input:\n\t", repr(s), "\n  should match:\n\t", " ".join(x if token_to_name(x) else repr(x) for x in tokens_and_values), end="\n\n")
                 test_number += 1
-            for tok, s in tokenize(s, suppress_whitespace=suppress_whitespace):
+            for tok, s in tokenize(pushback_str_iterator(s), suppress_whitespace=suppress_whitespace):
                 t = tokens.pop(0)
                 if want_print: # pragma: nocover
                     print("  [want]", t, end="")
                 if tok in tokens_with_values:
                     v = values.pop(0)
                     if want_print: # pragma: nocover
                         print(f" {s!r}")
                 else:
                     if want_print: # pragma: nocover
                         print()
                     v = None
                 if want_print: # pragma: nocover
                     print("  [ got]", tok, repr(s))
-                self.assertEqual(tok, t, "token doesn't match, expected " + str(token_to_name[t]) + " got " + str(token_to_name.get(tok)))
+                self.assertEqual(tok, t, "token doesn't match, expected " + token_to_name(t) + " got " + token_to_name(tok))
                 if v is not None:
                     self.assertEqual(v, s, "token value doesn't match, expected " + repr(v) + " got " + repr(s))
 
         def test(s, *tokens_and_values):
             without_whitespace = tuple(x for x in tokens_and_values if x != WHITESPACE)
             tests_differ = without_whitespace != tokens_and_values
             if tests_differ:
@@ -99,18 +104,18 @@
         test(r""" "quoted string"=[""", WHITESPACE, STRING, "quoted string", EQUALS, LEFT_SQUARE_BRACKET)
         test(r""" "quoted string" = [""", WHITESPACE, STRING, "quoted string", WHITESPACE, EQUALS, WHITESPACE, LEFT_SQUARE_BRACKET)
         test(r"x=y", STRING, "x", EQUALS, STRING, "y")
         test(r"x={", STRING, "x", EQUALS, LEFT_CURLY_BRACE)
         test(r"x=[", STRING, "x", EQUALS, LEFT_SQUARE_BRACKET)
         test(r'''x="quoted string"''', STRING, "x", EQUALS, STRING, "quoted string")
 
-        test(r'''[]''', EMPTY_SQUARE_BRACKETS)
-        test(r'''[ ]''', EMPTY_SQUARE_BRACKETS)
-        test(r'''{}''', EMPTY_CURLY_BRACES)
-        test(r'''{ }''', EMPTY_CURLY_BRACES)
+        test(r'[]', EMPTY_SQUARE_BRACKETS)
+        test(r'[ ]', EMPTY_SQUARE_BRACKETS)
+        test(r'{}', EMPTY_CURLY_BRACES)
+        test(r'{ }', EMPTY_CURLY_BRACES)
 
         # and now, the big finish
         test(r""" 'quoted string' "quoted string 2" [ { = "quoted value" [ { ] } = "yes!" [{}] ''' """,
             WHITESPACE,
             STRING, "quoted string",
             WHITESPACE,
             STRING, "quoted string 2",
@@ -147,15 +152,15 @@
         s = '''
         x = """
           abc
           """ what's this?
         '''
         tokens = []
         with self.assertRaises(ValueError):
-            for t in tokenize(s):
+            for t in tokenize(pushback_str_iterator(s)):
                 tokens.append(t)
         self.assertEqual(tokens, [(STRING, 'x'), (EQUALS, '=')])
 
 
 class TestLineTokenizer(PerkyTestCase):
     def test_empty_line_tokenizer(self):
         lt = LineTokenizer('')
```

### Comparing `perky-0.8.2/tests/test_transform.py` & `perky-0.9/tests/test_utility.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,75 @@
 #!/usr/bin/env python3
 
 import perkytestlib
 perkytestlib.preload_local_perky()
 
-
-import perky.transform
+import perky
 import unittest
 
-class TestTransform(unittest.TestCase):
 
-    def test_RecursiveChainMap(self):
-        dict1 = {'a': 1, 'sub': {1: 2, 3:4, 5:6}}
-        dict2 = {'b': 2, 'sub': {2: 3, 4:5, 6:7}}
-        merged_sub = {a: a+1 for a in range(1, 7)}
-
-        rcm = perky.RecursiveChainMap(dict1, dict2)
-        self.assertEqual(rcm['a'], 1)
-        self.assertEqual(rcm['b'], 2)
+class TestUtility(unittest.TestCase):
 
-        sub = {n: v for n, v in rcm['sub'].items()}
-        self.assertEqual(sub, merged_sub)
+    def test_merge_nothin(self):
+        o = perky.merge_dicts_and_lists()
+        self.assertIsNone(o)
 
     def test_merge_one_dict(self):
         dict1 = {'a': 1, 'b': 2}
-        d = perky.merge_dicts(dict1)
+        d = perky.merge_dicts_and_lists(dict1)
 
         self.assertEqual(d, dict1)
 
+    def test_merge_one_list(self):
+        l = [1, 2, 'c', 4]
+        l2 = perky.merge_dicts_and_lists(l)
+
+        self.assertEqual(l, l2)
+
     def test_merge_two_simple_dicts(self):
         dict1 = {'a': 1, 'b': 2}
         dict2 = {'c': 3}
-        d = perky.merge_dicts()
+        d = perky.merge_dicts_and_lists(dict1, dict2)
+        manually_merged = dict(dict1)
+        manually_merged.update(dict2)
+        self.assertEqual(d, manually_merged)
+
+    def test_merge_two_nested_dicts(self):
+        dict1 = {'a': 1, 'sub': {1:2, 3:4, 5:6}}
+        dict2 = {'b': 2, 'sub': {2:3, 4:5, 6:7}}
+        d = perky.merge_dicts_and_lists(dict1, dict2)
 
-    def test_merge_two_dicts(self):
-        dict1 = {'a': 1, 'sub': {1: 2, 3:4, 5:6}}
-        dict2 = {'b': 2, 'sub': {2: 3, 4:5, 6:7}}
-        merged_sub = {a: a+1 for a in range(1, 7)}
+        d2 = dict(dict1)
+        d2.update(dict2)
+        d2['sub'] = {a: a+1 for a in range(1, 7)}
+        self.assertEqual(d, d2)
+
+    def test_complex_merge_two_nested_dicts(self):
+        dict1 = {'a': 1, 'sub': {1:2, 3:4, 5:6}}
+        dict2 = {'b': 2, 'sub': {2:3, 4:5, 6:7}, 'l': [1, 2, 3]}
+        dict3 = {'c': 3}
+        dict4 = {'a': 5, 'd': 4, 'sub': {7:8, 8:9, 9:10}, 'l': [4, 5, 6]}
+        d = perky.merge_dicts_and_lists(dict1, dict2, dict3, dict4)
 
-        d = perky.merge_dicts(dict1, dict2)
         d2 = dict(dict1)
         d2.update(dict2)
-        d2['sub'] = merged_sub
+        d2.update(dict3)
+        d2.update(dict4)
+        d2['sub'] = {a: a+1 for a in range(1, 10)}
+        d2['l'] = list(range(1, 7))
         self.assertEqual(d, d2)
 
+    def test_invalid_inputs(self):
+        with self.assertRaises(TypeError):
+            perky.merge_dicts_and_lists({}, [])
+        with self.assertRaises(TypeError):
+            perky.merge_dicts_and_lists([], {})
+        with self.assertRaises(TypeError):
+            perky.merge_dicts_and_lists(3.14159, 66)
+        with self.assertRaises(TypeError):
+            perky.merge_dicts_and_lists({'a': [3]}, {'a': {'b': 3}})
+
+
+
 if __name__ == '__main__': # pragma: nocover
     unittest.main()
+
```

### Comparing `perky-0.8.2/PKG-INFO` & `perky-0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perky
-Version: 0.8.2
+Version: 0.9
 Summary: A simple, Pythonic file format.  Same interface as the
 Home-page: https://github.com/larryhastings/perky/
 Author: Larry Hastings
 Author-email: larry@hastings.org
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
@@ -167,34 +167,34 @@
 
 The first word after the equals sign is the name of the pragma, in this case `"command"`.
 Everything after the name of the pragma is an argument, with all leading
 and trailing whitespace removed, in this case `"argument here"`.
 
 By default, Perky doesn't have any pragma handlers.  And invoking a pragma
 when Perky doesn't have a handler for it is a runtime error.
-But you can define your own pragma handlers when you call `perky.load()`
-or `perky.loads()`, using a named parameter called `pragmas`.
+But you can define your own pragma handlers when you call `load()`
+or `loads()`, using a named parameter called `pragmas`.
 If you pass in a value for `pragmas`, it must be a mapping
 of strings to functions.
 The string name should be the name of the pragma and must be lowercase.
 The function it maps to will "handle" that pragma, and should match this
 prototype:
 
 `def pragma_fn(parser, argument)`
 
 `parser` is the internal Perky `Parser` object.  `argument` is the
 rest of the relevant line, with leading & trailing whitespace stripped.
 (If the rest of the line was empty, `argument` will be `None`).
 The return value of the pragma function is ignored.
 
 There's currently only one predefined pragma handler, a function called
-`perky.pragma_include()`.  This adds "include statement" functionality
+`pragma_include()`.  This adds "include statement" functionality
 to Perky.  If you call this:
 
-`perky.load(filename, pragmas={'include': perky.pragma_include()})`
+`load(filename, pragmas={'include': pragma_include()})`
 
 then Perky will interpret lines inside `filename` starting with `=include`
 as include statements, using the rest of the line as the name of a file.
 For more information, see `pragma_include()` below.
 
 The rules of pragmas:
 * To invoke a pragma, use `=` as the first non-whitespace character
@@ -212,130 +212,153 @@
 ### Parsing Errors
 
 There are only a few errors possible when parsing a Perky text:
 
 * Obviously, syntax errors, for example:
     * A line in a dict that doesn't have an unquoted equals sign
     * A line in a list that looks like a dict line (`name = value`).
-      (If you want a value like that inside a list, simply put it in quotes.)
+      (If you want a value containing an equals sign inside a list,
+      simply put it in quotes.)
     * A triple-quoted string where any line is outdented past
       the ending triple quotes line.
 * Defining the same value twice in the same dict.  This is flagged
-  as an error, because it could easily be a mistake, and in Python
+  as an error, because it could easily be a mistake, and like Python
   we don't want to let errors pass silently.
 * Using an undefined pragma.
 * Using one of Perky's special tokens as a pragma argument, like
   `{`, `[`, `'''`, `"""`, `[]`, or `{}`.
 
 ### API
 
-#### `def loads(s, *, pragmas=None, root=None) -> o`
+#### `loads(s, *, pragmas=None, root=None)`
 
 Parses a Perky-format string, and returns a container filled
 with the values parsed from that string.
 
+If `pragmas` is not `None`, it must be a mapping of
+strings to pragma handler functions.  Please see the
+**Pragmas** section of the documentation.
+
 If `root` is `None`, `loads` behaves as if you passed in an
 empty `dict`.
 
 If `root` is not `None`, it should be a container, either
 a mutable mapping (`dict`) or a mutable sequence (`list`).
 This affects how the data is parsed; if `root` is a
 mutable mapping, the top level of the Perky file must be
 a "mapping context" (a series of `name=value` lines);
 if `root` is a mutable sequence, the top level of the Perky
 file is assumed to be a "sequence context"
 (a series of `value` lines).
 
-#### `def load(s, *, pragmas=None, encoding='utf-8', root=None) -> o`
+#### `load(filename, *, pragmas=None, root=None)`
 
-Parses a file containing Perky-file-format settings.
+Loads a file containing Perky-file-format settings.
 Returns a dict.
 
-`encoding` specifies the encoding used to decode the
-data read from the file.
+The text in the file must be encoded using
+[UTF-8](https://en.wikipedia.org/wiki/UTF-8).
 
-#### `perky.dumps(d) -> s`
+If `root` is `None`, `loads` behaves as if you passed in an
+empty `dict`.
+
+If `root` is not `None`, it should be a container, either
+a mutable mapping (`dict`) or a mutable sequence (`list`).
+This affects how the data is parsed; if `root` is a
+mutable mapping, the top level of the Perky file must be
+a "mapping context" (a series of `name=value` lines);
+if `root` is a mutable sequence, the top level of the Perky
+file is assumed to be a "sequence context"
+(a series of `value` lines).
+
+If `pragmas` is not `None`, it must be a mapping of
+strings to pragma handler functions.  Please see the
+**Pragmas** section of the documentation.
+
+#### `dumps(d)`
 
 Converts a dictionary to a Perky-file-format string.
 Keys in the dictionary must all be strings.  Values
 that are not dicts, lists, or strings will be converted
 to strings using str.
 Returns a string.
 
-#### `perky.dump(filename, d, *, pragmas=None, encoding="utf-8")`
+#### `dump(filename, d)`
 
 Converts a dictionary to a Perky-file-format string
-using `perky.dump`, then writes it to *filename*.
+using `dump`, then writes it to *filename*.
 
-`encoding` specifies the encoding used to encode the
-data written to the file.
+The text in the file will be encoded using
+[UTF-8](https://en.wikipedia.org/wiki/UTF-8).
 
-#### `perky.pragma_include(include_path=(".",), *, encoding='utf-8')`
+#### `pragma_include(include_path=(".",))`
 
 This function generates a pragma handler that adds "include"
 functionality.  "Including" means lexically inserting one Perky
 file inside another, contextually at the spot where the pragma
 exists.
 
-For example:
+For example, if you ran this:
 
-    d = perky.loads("a=3\n" "=include data.pky\n" "c=5\n",
-        pragmas={"include": perky.pragma_include()},
+    d = loads("a=3\n" "=include data.pky\n" "c=5\n",
+        pragmas={"include": pragma_include()},
         )
 
-If *data.pky* contained the following:
+And *data.pky* in the current directory was readable and
+contained the following text:
 
     b=4
 
 then `d` would be set to the dictionary:
 
     {'a': '3', 'b': '4', 'c': '5'}
 
-`perky.pragma_include()` is not the pragma handler itself;
+`pragma_include()` is not the pragma handler itself;
 it returns a function (a closure) which remembers the `include_path`
 you pass in.  This allows you to use it for multiple pragmas that
 include from different paths, e.g.:
 
     include_dirs = [appdirs.user_data_dir(myapp_name)]
     config_dirs = [appdirs.user_config_dir(myapp_name)]
     pragmas = {
-        'include': perky.pragma_include(include_dirs),
-        'config': perky.pragma_include(config_dirs),
+        'include': pragma_include(include_dirs),
+        'config': pragma_include(config_dirs),
     }
 
-`encoding` specifies the encoding used to decode the
-data read in from the included files.
-
 Notes:
 
 * The pragma handler is context-sensitive; the included
 file will be included as if it was copied-and-pasted replacing
 the pragma line.  Among other things, this means that if the pragma
 is invoked inside a sequence context, the included file must *start*
 in a sequence context.
 
 * When loading the file, the pragma handler will pass in the
-current pragma handlers into `perky.load()`.  Among other things,
+current pragma handlers into `load()`.  Among other things,
 this allows for recursive includes.
 
 * When including inside a dict context, you're explicitly permitted
 to re-define existing keys if they were previously defined in
 another file.
 
 * The default value for `include_path` only searches the
 current directory (`"."`).  If you override the default
 and pass in your own include path, the pragma handler
-won't search the current directory unless you add `"."`
-to the include path yourself.
+won't search the current directory unless you explicitly
+add `"."` to the include path yourself.
+
+* If `pragma_include` can't find the requested file on
+its search path, it raises `FileNotFoundError`.
+
 
 #### Deprecated API
 
 Perky has a "transformation" submodule.
 The idea is, you load a Perky file,
-then run `perky.transform` on that dictionary to
+then run `transform` on that dictionary to
 convert the strings into native values.
 
 These functions are no longer maintained or supported,
 and will be removed before 1.0.
 Why?  This part of Perky was always
 an experiment... and the experiment never really paid
 off.  There are better implementations of this idea,
@@ -344,73 +367,87 @@
 this code in Perky, I encourage you to fork
 off a copy and maintain it yourself.  But I doubt
 anybody is.)
 
 For posterity's sakes, here's documentation of the
 now-deprecated API.
 
-`perky.map(d, fn) -> o`
+`map(d, fn) -> o`
 
 Iterates over a dictionary.  Returns a new dictionary where,
 for every *value*:
   * if it's a dict, replace with a new dict.
   * if it's a list, replace with a new list.
   * if it's neither a dict nor a list, replace with
     `fn(value)`.
 
 The function passed in is called a *conversion function*.
 
-`perky.transform(d, schema, default=None) -> o`
+`transform(d, schema, default=None) -> o`
 
 Recursively transforms a Perky dict into some other
 object (usually a dict) using the provided schema.
 Returns a new dict.
 
 A *schema* is a data structure matching the general expected
 shape of *d*, where the values are dicts, lists, and
-callables.  The transformation is similar to `perky.map()`
+callables.  The transformation is similar to `map()`
 except that individual values will have individual conversion
 functions.  Also, a schema conversion function can be specified
 for any value in *d*, even dicts or lists.
 
 *default* is a default conversion function.  If there is a
 value *v* in *d* that doesn't have an equivalent entry in *schema*,
 and *v* is neither a list nor a dict, and if *default* is
 a callable, *v* will be replaced with `default(v)` in the
 output.
 
-`perky.Required`
+`Required`
 
 Experimental.
 
-`perky.nullable(fn) -> fn`
+`nullable(fn) -> fn`
 
 Experimental.
 
-`perky.const(fn) -> o`
+`const(fn) -> o`
 
 Experimental.
 
 
 ### TODO
 
 * Backslash quoting currently does "whatever your version of Python does".  Perhaps this should be explicit, and parsed by Perky itself?
 
 ### Changelog
 
+**0.9** *2023/07/02*
+
+Breaking API change: removed the `encoding` argument entirely.
+
+* From this point forward, Perky only supports reading and
+  writing files in
+  [UTF-8](https://en.wikipedia.org/wiki/UTF-8).
+  If you need to work with a different encoding, you'll have
+  to handle loading it form and saving it to disk yourself.
+  You'll have to use `loads` and `dumps` to handle converting
+  between Perky string format and native Python objects.
+
+* Optimized Perky some more.  It's roughly 11% faster than 0.8.1.
+
 **0.8.2** *2023/06/30*
 
 * Minor API changes:
 
   - You can now pass an `encoding` keyword argument
     into `pragma_include`.  This is now the only way
     to specify the encoding used to decode files
     loaded from disk by `pragma_include`.
   - Removed the (undocumented) `encoding` attribute
-    of the `perky.Parser` object.
+    of Perky's `Parser` object.
   - Removed the `encoding` parameter for `loads`.
   - The `encoding` parameter for `load` is now only
     used by `load` itself when loading the top-level
     Perky file.
 
 **0.8.1** *2023/06/26*
 
@@ -426,16 +463,16 @@
   your own mapping and sequence objects that *don't* inherit from
   `dict` and `list`.
 * Renamed `PerkyFormatError` to `FormatError`.  The old name is
   supported for now, but please transition to the new name.
   The old name will be removed before 1.0.
 * The "transformation" submodule is now deprecated and unsupported.
   Please either stop using it or fork and maintain it yourself.
-  This includes `perky.map`, `perky.transform`, `perky.Required`,
-  `perky.nullable`, and `perky.const`.
+  This includes `map`, `transform`, `Required`,
+  `nullable`, and `const`.
 * Perky now has a proper unit test suite, which it passes with 100%
   coverage--except for the unsupported `transform` submodule.
 * While working towards 100% coverage, also cleaned up the code
   a little in spots.
 
   - Retooled `LineTokenizer`:
```

