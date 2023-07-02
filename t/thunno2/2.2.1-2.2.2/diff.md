# Comparing `tmp/thunno2-2.2.1.tar.gz` & `tmp/thunno2-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thunno2-2.2.1.tar", last modified: Tue May 30 13:17:01 2023, max compression
+gzip compressed data, was "thunno2-2.2.2.tar", last modified: Sun Jul  2 13:19:57 2023, max compression
```

## Comparing `thunno2-2.2.1.tar` & `thunno2-2.2.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-05-30 13:17:01.699792 thunno2-2.2.1/
--rw-r--r--   0 nayak      (501) staff       (20)      959 2023-05-30 13:17:01.699669 thunno2-2.2.1/PKG-INFO
--rw-r--r--   0 nayak      (501) staff       (20)       38 2023-05-30 13:17:01.699831 thunno2-2.2.1/setup.cfg
--rw-r--r--   0 nayak      (501) staff       (20)     1314 2023-05-30 13:16:32.000000 thunno2-2.2.1/setup.py
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-05-30 13:17:01.698978 thunno2-2.2.1/thunno2/
--rw-r--r--   0 nayak      (501) staff       (20)       22 2023-05-01 12:43:53.000000 thunno2-2.2.1/thunno2/__init__.py
--rw-r--r--   0 nayak      (501) staff       (20)     3268 2023-05-14 14:05:01.000000 thunno2-2.2.1/thunno2/autoexplanation.py
--rw-r--r--   0 nayak      (501) staff       (20)     1491 2023-05-11 17:22:25.000000 thunno2-2.2.1/thunno2/canvas.py
--rw-r--r--   0 nayak      (501) staff       (20)     1393 2023-04-16 17:25:02.000000 thunno2-2.2.1/thunno2/codepage.py
--rw-r--r--   0 nayak      (501) staff       (20)    56522 2023-05-30 13:11:50.000000 thunno2-2.2.1/thunno2/commands.py
--rw-r--r--   0 nayak      (501) staff       (20)     3046 2023-05-14 17:13:03.000000 thunno2-2.2.1/thunno2/constants.py
--rw-r--r--   0 nayak      (501) staff       (20)   245360 2023-04-16 17:25:02.000000 thunno2-2.2.1/thunno2/dictionary.py
--rw-r--r--   0 nayak      (501) staff       (20)     7253 2023-05-15 16:46:52.000000 thunno2-2.2.1/thunno2/flags.py
--rw-r--r--   0 nayak      (501) staff       (20)    56820 2023-05-30 13:11:50.000000 thunno2-2.2.1/thunno2/helpers.py
--rw-r--r--   0 nayak      (501) staff       (20)    33860 2023-05-27 16:56:14.000000 thunno2-2.2.1/thunno2/interpreter.py
--rw-r--r--   0 nayak      (501) staff       (20)    26658 2023-05-27 16:18:35.000000 thunno2-2.2.1/thunno2/lexer.py
--rw-r--r--   0 nayak      (501) staff       (20)     3440 2023-05-27 07:11:18.000000 thunno2-2.2.1/thunno2/run.py
--rw-r--r--   0 nayak      (501) staff       (20)    84691 2023-05-30 13:11:50.000000 thunno2-2.2.1/thunno2/tests.py
--rw-r--r--   0 nayak      (501) staff       (20)     4526 2023-05-14 14:36:33.000000 thunno2-2.2.1/thunno2/tokens.py
--rw-r--r--   0 nayak      (501) staff       (20)       97 2023-05-30 13:12:03.000000 thunno2-2.2.1/thunno2/version.py
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-05-30 13:17:01.699509 thunno2-2.2.1/thunno2.egg-info/
--rw-r--r--   0 nayak      (501) staff       (20)      959 2023-05-30 13:17:01.000000 thunno2-2.2.1/thunno2.egg-info/PKG-INFO
--rw-r--r--   0 nayak      (501) staff       (20)      459 2023-05-30 13:17:01.000000 thunno2-2.2.1/thunno2.egg-info/SOURCES.txt
--rw-r--r--   0 nayak      (501) staff       (20)        1 2023-05-30 13:17:01.000000 thunno2-2.2.1/thunno2.egg-info/dependency_links.txt
--rw-r--r--   0 nayak      (501) staff       (20)       54 2023-05-30 13:17:01.000000 thunno2-2.2.1/thunno2.egg-info/entry_points.txt
--rw-r--r--   0 nayak      (501) staff       (20)        8 2023-05-30 13:17:01.000000 thunno2-2.2.1/thunno2.egg-info/top_level.txt
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-07-02 13:19:57.759678 thunno2-2.2.2/
+-rw-r--r--   0 nayak      (501) staff       (20)      959 2023-07-02 13:19:57.759568 thunno2-2.2.2/PKG-INFO
+-rw-r--r--   0 nayak      (501) staff       (20)       38 2023-07-02 13:19:57.759756 thunno2-2.2.2/setup.cfg
+-rw-r--r--   0 nayak      (501) staff       (20)     1314 2023-05-30 13:16:32.000000 thunno2-2.2.2/setup.py
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-07-02 13:19:57.758922 thunno2-2.2.2/thunno2/
+-rw-r--r--   0 nayak      (501) staff       (20)       22 2023-05-01 12:43:53.000000 thunno2-2.2.2/thunno2/__init__.py
+-rw-r--r--   0 nayak      (501) staff       (20)     3268 2023-05-14 14:05:01.000000 thunno2-2.2.2/thunno2/autoexplanation.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1491 2023-05-11 17:22:25.000000 thunno2-2.2.2/thunno2/canvas.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1393 2023-04-16 17:25:02.000000 thunno2-2.2.2/thunno2/codepage.py
+-rw-r--r--   0 nayak      (501) staff       (20)    57155 2023-07-02 13:06:12.000000 thunno2-2.2.2/thunno2/commands.py
+-rw-r--r--   0 nayak      (501) staff       (20)     3046 2023-05-14 17:13:03.000000 thunno2-2.2.2/thunno2/constants.py
+-rw-r--r--   0 nayak      (501) staff       (20)   245360 2023-04-16 17:25:02.000000 thunno2-2.2.2/thunno2/dictionary.py
+-rw-r--r--   0 nayak      (501) staff       (20)     7303 2023-06-03 14:35:27.000000 thunno2-2.2.2/thunno2/flags.py
+-rw-r--r--   0 nayak      (501) staff       (20)    58798 2023-07-02 13:06:12.000000 thunno2-2.2.2/thunno2/helpers.py
+-rw-r--r--   0 nayak      (501) staff       (20)    33291 2023-06-24 09:12:25.000000 thunno2-2.2.2/thunno2/interpreter.py
+-rw-r--r--   0 nayak      (501) staff       (20)    25968 2023-06-24 14:02:54.000000 thunno2-2.2.2/thunno2/lexer.py
+-rw-r--r--   0 nayak      (501) staff       (20)     3440 2023-07-02 13:16:10.000000 thunno2-2.2.2/thunno2/run.py
+-rw-r--r--   0 nayak      (501) staff       (20)    86444 2023-07-02 13:06:12.000000 thunno2-2.2.2/thunno2/tests.py
+-rw-r--r--   0 nayak      (501) staff       (20)     4505 2023-06-24 09:12:25.000000 thunno2-2.2.2/thunno2/tokens.py
+-rw-r--r--   0 nayak      (501) staff       (20)       97 2023-07-02 13:18:12.000000 thunno2-2.2.2/thunno2/version.py
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-07-02 13:19:57.759423 thunno2-2.2.2/thunno2.egg-info/
+-rw-r--r--   0 nayak      (501) staff       (20)      959 2023-07-02 13:19:57.000000 thunno2-2.2.2/thunno2.egg-info/PKG-INFO
+-rw-r--r--   0 nayak      (501) staff       (20)      459 2023-07-02 13:19:57.000000 thunno2-2.2.2/thunno2.egg-info/SOURCES.txt
+-rw-r--r--   0 nayak      (501) staff       (20)        1 2023-07-02 13:19:57.000000 thunno2-2.2.2/thunno2.egg-info/dependency_links.txt
+-rw-r--r--   0 nayak      (501) staff       (20)       54 2023-07-02 13:19:57.000000 thunno2-2.2.2/thunno2.egg-info/entry_points.txt
+-rw-r--r--   0 nayak      (501) staff       (20)        8 2023-07-02 13:19:57.000000 thunno2-2.2.2/thunno2.egg-info/top_level.txt
```

### Comparing `thunno2-2.2.1/PKG-INFO` & `thunno2-2.2.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: thunno2
-Version: 2.2.1
+Version: 2.2.2
 Summary: A golfing language
 Home-page: https://github.com/Thunno/Thunno2
 Author: Rujul Nayak
 Author-email: rujulnayak@outlook.com
 License: MIT
-Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.2.1.tar.gz
+Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.2.2.tar.gz
 Keywords: golfing,code-golf,language
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `thunno2-2.2.1/setup.py` & `thunno2-2.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.1/thunno2/autoexplanation.py` & `thunno2-2.2.2/thunno2/autoexplanation.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.1/thunno2/canvas.py` & `thunno2-2.2.2/thunno2/canvas.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.1/thunno2/codepage.py` & `thunno2-2.2.2/thunno2/codepage.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.1/thunno2/commands.py` & `thunno2-2.2.2/thunno2/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -939,15 +939,20 @@
             (str, str): greater_than_or_equal_to,
         },
         2,
         ("greater_than_or_equal_to",),
     ),
     "&": Overload(2, {(Any[0], Any[0]): logical_and}, 2, ("and", "logical_and")),
     "|": Overload(2, {(Any[0], Any[0]): logical_or}, 2, ("or", "logical_or")),
-    "^": Overload(2, {(Any[0], Any[0]): logical_xor}, 2, ("xor", "logical_xor")),
+    "^": Overload(
+        1,
+        {Number: num_uninterleave_dump, Iterable: uninterleave_dump},
+        0,
+        ("uninterleave_dump",),
+    ),
     "~": Overload(1, {Any: logical_not}, 1, ("not", "logical_not")),
     "ð": Overload(0, {Any: (lambda: " ")}, 0, ("space",)),
     "Ð": Overload(1, {Any: triplicate}, 0, ("triplicate",)),
     "ȧ": Overload(
         3,
         {
             (Any[0], Number[0], Iterable[0]): assign,
@@ -1216,14 +1221,15 @@
     "Ä": Overload(
         1,
         {Number: num_to_alphabet, str: alphabet_to_num},
         1,
         ("num_to_alphabet", "alphabet_to_num"),
     ),
     "¶": Overload(0, {Any: (lambda: "\n")}, 0, ("newline",)),
+    "Ç": Overload(0, {Any: (lambda: "|")}, 0, ("pipe",)),
     "¬": Overload(
         1, {Any: logical_not}, 0, ("non_vectorised_not", "non_vectorised_logical_not")
     ),
     "§": Overload(
         2,
         {
             (Number[0], Number[0]): dyadic_maximum,
@@ -1583,14 +1589,18 @@
     "s": Overload(1, {Any: arc_sine}, 1, ("arc_sine", "arcsin")),
     "t": Overload(1, {Any: arc_tangent}, 1, ("arc_tangent", "arctan")),
     "ḷ": Overload(1, {Any: log2}, 1, ("log2", "log_base_2")),
     "&": Overload(2, {(Any[0], Any[0]): bitwise_and}, 2, ("bitwise_and",)),
     "|": Overload(2, {(Any[0], Any[0]): bitwise_or}, 2, ("bitwise_or",)),
     "^": Overload(2, {(Any[0], Any[0]): bitwise_xor}, 2, ("bitwise_xor",)),
     "~": Overload(1, {Any: bitwise_not}, 1, ("bitwise_not",)),
+    "²": Overload(1, {Any: perfect_square}, 1, ("perfect_square",)),
+    "³": Overload(1, {Any: perfect_cube}, 1, ("perfect_cube",)),
+    "⁴": Overload(1, {Any: perfect_fourth}, 1, ("perfect_fourth",)),
+    "⁵": Overload(1, {Any: perfect_fifth}, 1, ("perfect_fifth",)),
 }
 
 random_digraphs_2 = {
     "R": Overload(
         1, {Number: to_roman_numerals, str: from_roman_numerals}, 1, ("roman_numerals",)
     ),
     "T": Overload(1, {Any: type_of}, 0, ("type",)),
@@ -1657,14 +1667,24 @@
     ),
     "^": Overload(
         2,
         {(Any[0], Any[0]): logical_xor},
         0,
         ("non_vectorised_xor", "non_vectorised_logical_xor"),
     ),
+    "/": Overload(
+        2,
+        {
+            (list, Any[0]): swapped_split_on,
+            (Any[0], Iterable[0]): split_on,
+            (Any[0], Number[0]): num_split_on,
+        },
+        0,
+        ("split_on",),
+    ),
 }
 
 
 def get_a_function(command):
     if not command:
         return Void
     if len(command) == 1:
```

### Comparing `thunno2-2.2.1/thunno2/constants.py` & `thunno2-2.2.2/thunno2/constants.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.1/thunno2/dictionary.py` & `thunno2-2.2.2/thunno2/dictionary.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.1/thunno2/flags.py` & `thunno2-2.2.2/thunno2/flags.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,14 +204,15 @@
                 except:
                     expected = output.strip()
             except Exception as e:
                 print(f"FAIL ❌ (Got error {e})")
                 continue
             commands.ctx.og_input_list = new_inputs.copy()
             commands.ctx.other_il = new_inputs.copy()
+            commands.ctx.stack = commands.Stack()
             print(line, "--> ", end="")
             interpreter.run(code, context=0, iteration_index=0)
             process_output_flags(new_flags, False)
             actual_output = next(commands.ctx.stack.rmv(1))
             print(actual_output, end="\t")
             if actual_output == expected:
                 print("PASS ✅")
```

### Comparing `thunno2-2.2.1/thunno2/helpers.py` & `thunno2-2.2.2/thunno2/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,14 +159,37 @@
             return fn(*map(float, args))
         except:
             return [*args]
 
     return wrapper
 
 
+def try_number_conversion(func):
+    def wrapper(*args, fn=func):
+        new_args = []
+        try:
+            for a in args:
+                if isinstance(a, int):
+                    new_args.append(a)
+                elif isinstance(a, str):
+                    try:
+                        new_args.append(int(a))
+                    except:
+                        new_args.append(float(a))
+                elif isinstance(a, float):
+                    new_args.append(a)
+                else:
+                    raise
+        except:
+            return args
+        return fn(*new_args)
+
+    return wrapper
+
+
 def safe_max_len(*lsts):
     m = 0
     for lst in lsts:
         if isinstance(lst, list):
             if len(lst) > m:
                 m = len(lst)
     return m
@@ -772,15 +795,18 @@
 def list_replace(x, y, z):
     return [x if i == y else i for i in z]
 
 
 def digit_reverse(num):
     r = str(num)[::-1]
     try:
-        return eval(r)
+        try:
+            return int(r)
+        except:
+            return eval(r)
     except:
         return r
 
 
 def reverse(x):
     return x[::-1]
 
@@ -813,14 +839,22 @@
     return [l[0::2], l[1::2]]
 
 
 def num_uninterleave(n):
     return uninterleave(_digits(n))
 
 
+def uninterleave_dump(l):
+    return l[0::2], l[1::2]
+
+
+def num_uninterleave_dump(n):
+    return uninterleave_dump(_digits(n))
+
+
 def bool2(x):
     return int(bool(x))
 
 
 def isalphanum(s):
     return int(s.isalnum())
 
@@ -1755,59 +1789,75 @@
 
 
 def mirror(x):
     return x + x[::-1]
 
 
 def str_transliterate(a, b, c):
-    for i, j in zip(a, b):
-        c = str(c).replace(str(j), str(i))
-    return str(c)
+    r = ""
+    d = dict(zip(map(str, b), map(str, a)))
+    for x in str(c):
+        r += str(d.get(x, x))
+    return r
 
 
 def list_transliterate(a, b, c):
-    for i, j in zip(a, b):
-        c = list_replace(i, j, c)
-    return c
+    r = []
+    d = dict(zip(b, a))
+    for x in c:
+        r.append(d.get(x, x))
+    return r
 
 
 def str_transliterate_overload_1(a, b, c):
-    for i, j in zip(a, str(b)):
-        c = str(c).replace(str(j), str(i))
-    return str(c)
+    r = ""
+    d = dict(zip(str(b), map(str, a)))
+    for x in str(c):
+        r += str(d.get(x, x))
+    return r
 
 
 def list_transliterate_overload_1(a, b, c):
-    for i, j in zip(a, str(b)):
-        c = list_replace(i, j, c)
-    return c
+    r = []
+    d = dict(zip(str(b), a))
+    for x in c:
+        r.append(d.get(x, x))
+    return r
 
 
 def str_transliterate_overload_2(a, b, c):
-    for i, j in zip(str(a), b):
-        c = str(c).replace(str(j), str(i))
-    return str(c)
+    r = ""
+    d = dict(zip(map(str, b), str(a)))
+    for x in str(c):
+        r += str(d.get(x, x))
+    return r
 
 
 def list_transliterate_overload_2(a, b, c):
-    for i, j in zip(str(a), b):
-        c = list_replace(i, j, c)
-    return c
+    r = []
+    d = dict(zip(b, str(a)))
+    for x in c:
+        r.append(d.get(x, x))
+    return r
 
 
 def str_transliterate_overload_3(a, b, c):
-    for i, j in zip(str(a), str(b)):
-        c = str(c).replace(str(j), str(i))
-    return str(c)
+    r = ""
+    d = dict(zip(str(b), str(a)))
+    for x in str(c):
+        r += str(d.get(x, x))
+    return r
 
 
 def list_transliterate_overload_3(a, b, c):
-    for i, j in zip(str(a), str(b)):
-        c = list_replace(i, j, c)
-    return c
+    r = []
+    d = dict(zip(str(b), str(a)))
+    for x in c:
+        r.append(d.get(x, x))
+    return r
 
 
 def combinations_with_replacement1(n, x):
     if n > len(x):
         n = len(x)
     if n < 1:
         n = 1
@@ -2233,18 +2283,22 @@
     if not l:
         return l
     return random.choice(l)
 
 
 def square_root(i):
     n = abs(i)
-    x, y = math.sqrt(n), math.isqrt(n)
-    if x == y:
-        return y
-    return x
+    x = math.sqrt(n)
+    try:
+        y = math.isqrt(n)
+        if x == y:
+            return y
+        return x
+    except:
+        return x
 
 
 def every_second_item(s):
     return s[::2]
 
 
 def sign(n):
@@ -2280,15 +2334,15 @@
             r.append(it_sum(i))
         else:
             r.append(digit_sum(i))
     return r
 
 
 def all_equal(l):
-    return int(len({*l}) <= 1)
+    return int(len(uniquify_lst(l)) <= 1)
 
 
 def num_all_equal(n):
     return all_equal(str(n))
 
 
 def symmetric_set_difference(x, y):
@@ -3064,7 +3118,61 @@
 def ln(a):
     return math.log(a)
 
 
 @try_float_conversion
 def log2(a):
     return math.log2(a)
+
+
+def split_on(x, l):
+    if isinstance(l, str):
+        x = str(x)
+    r = [l * 0]
+    for i in l:
+        if i == x:
+            r.append(l * 0)
+        else:
+            r[-1] += [i] if isinstance(l, list) else i
+    return r
+
+
+def num_split_on(x, y):
+    return split_on(x, _digits(y))
+
+
+def swapped_split_on(l, x):
+    return split_on(x, l)
+
+
+def perfect_nth(n, a):
+    if isinstance(a, float):
+        if not str(a).endswith(".0"):
+            return 0
+        a = int(a)
+    n = int(n)
+    if n <= 0:
+        return 0
+    if n == 1:
+        return 1
+    l = [i**n for i in inclusive_zero_range(abs(a))]
+    return int(a in l)
+
+
+@try_number_conversion
+def perfect_square(a):
+    return perfect_nth(2, a)
+
+
+@try_number_conversion
+def perfect_cube(a):
+    return perfect_nth(3, a)
+
+
+@try_number_conversion
+def perfect_fourth(a):
+    return perfect_nth(4, a)
+
+
+@try_number_conversion
+def perfect_fifth(a):
+    return perfect_nth(5, a)
```

### Comparing `thunno2-2.2.1/thunno2/interpreter.py` & `thunno2-2.2.2/thunno2/interpreter.py`

 * *Files 1% similar despite different names*

```diff
@@ -688,29 +688,14 @@
                 r.append(k[-1])
             ctx.stack = Stack(copy.deepcopy(old_stack))
             ctx.stack.push(a)
             k = f2()
             if k:
                 r.append(k[-1])
             ctx.stack.push(r)
-        elif desc == "two function map":
-            a = next(ctx.stack.rmv(1))
-            old_stack = Stack(copy.deepcopy(list(ctx.stack).copy()))
-            r = []
-            f1, f2 = info
-            x = listify(a)
-            for i in x:
-                ctx.stack = Stack(copy.deepcopy(list(old_stack).copy()))
-                ctx.stack.push(i)
-                for j in f1():
-                    ctx.stack.push(j)
-                for k in f2():
-                    ctx.stack.push(k)
-                r.append(next(ctx.stack.rmv(1)))
-            ctx.stack.push(r)
         elif desc == "recursive environment":
             a = next(ctx.stack.rmv(1))
             if isinstance(a, list):
                 x = copy.deepcopy(a)
             else:
                 x = [a]
             for i in x:
```

### Comparing `thunno2-2.2.1/thunno2/lexer.py` & `thunno2-2.2.2/thunno2/lexer.py`

 * *Files 1% similar despite different names*

```diff
@@ -638,34 +638,14 @@
                 if cmd2 in DIGRAPHS:
                     index += 1
                     cmd2 += code[index]
                 func2 = get_a_function(cmd2)
             except:
                 func2, cmd2 = Void, ""
             ret.append((char + cmd1 + cmd2, "pair apply", (func1, func2)))
-        elif char == "Ç":
-            try:
-                index += 1
-                cmd1 = code[index]
-                if cmd1 in DIGRAPHS:
-                    index += 1
-                    cmd1 += code[index]
-                func1 = get_a_function(cmd1)
-            except:
-                func1, cmd1 = Void, ""
-            try:
-                index += 1
-                cmd2 = code[index]
-                if cmd2 in DIGRAPHS:
-                    index += 1
-                    cmd2 += code[index]
-                func2 = get_a_function(cmd2)
-            except:
-                func2, cmd2 = Void, ""
-            ret.append((char + cmd1 + cmd2, "two function map", (func1, func2)))
         elif char in expected_end:
             return index, ret
         elif char == ":":
             ret.append((":", "command", commands["="]))
             return index + 1, ret
         elif char == "}":
             ret.append(("}", "command", commands["¬"]))
```

### Comparing `thunno2-2.2.1/thunno2/run.py` & `thunno2-2.2.2/thunno2/run.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.1/thunno2/tests.py` & `thunno2-2.2.2/thunno2/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -627,14 +627,15 @@
 
 assert_eq(call("p", [1, 2, "abc", 3]), 6)
 
 # r
 
 assert_eq(call("r", 1.23), 32.1)
 assert_eq(call("r", -456), "654-")
+assert_eq(call("r", 3210), 123)
 
 assert_eq(call("r", "abcd"), "dcba")
 assert_eq(call("r", ""), "")
 
 assert_eq(call("r", [1, 2, 3, 4]), [4, 3, 2, 1])
 assert_eq(call("r", [123, "abc", 456, "def"]), ["def", 456, "abc", 123])
 
@@ -1214,21 +1215,22 @@
 assert_eq(call("|", -123, "abc"), "abc")
 assert_eq(call("|", "xyz", 0), "xyz")
 
 assert_eq(call("|", [-1, 0, 1], ["abc", "def", ""]), ["abc", "def", 1])
 
 # ^
 
-assert_eq(call("^", 123, 456), 0)
-assert_eq(call("^", 123, 0), 1)
+assert_eq(call("^", 12345), [1, 3, 5], [2, 4])
+assert_eq(call("^", -6.789), [6, 8], [7, 9])
 
-assert_eq(call("^", -123, "abc"), 0)
-assert_eq(call("^", "xyz", 0), 1)
+assert_eq(call("^", "abcdef"), "ace", "bdf")
+assert_eq(call("^", "xyz"), "xz", "y")
 
-assert_eq(call("^", [-1, 0, 1], ["abc", "def", ""]), [0, 1, 1])
+assert_eq(call("^", [1, 2, 3, 4]), [1, 3], [2, 4])
+assert_eq(call("^", []), [], [])
 
 # ~
 
 assert_eq(call("~", 123), 0)
 assert_eq(call("~", 0), 1)
 
 assert_eq(call("~", "abc"), 0)
@@ -1549,14 +1551,20 @@
 assert_eq(
     call("Ṃ", [123, "abc", 456, "def"]),
     [123, "abc", 456, "def", "def", 456, "abc", 123],
 )
 
 # Ṇ
 
+assert_eq(
+    call(
+        "Ṇ", "ZYXWVUTSRQPONMLKJIHGFEDCBA", "ABCDEFGHIJKLMNOPQRSTUVWXYZ", "HELLO, WORLD!"
+    ),
+    "SVOOL, DLIOW!",
+)
 assert_eq(call("Ṇ", "wxyz", 4321, "abcd1234"), "abcdzyxw")
 assert_eq(
     call("Ṇ", "abc", 123, ["1", "9", "4", "7", "8", "5", "6", "2", "3"]),
     ["a", "9", "4", "7", "8", "5", "6", "b", "c"],
 )
 assert_eq(call("Ṇ", 456, [1, "y", 3], "123xyz"), "426x5z")
 
@@ -2155,23 +2163,28 @@
 # ƭ
 
 assert_eq(call("ƭ", 100), 10)
 assert_eq(call("ƭ", 10), 3.1622776601683795)
 assert_eq(
     call("ƭ", [-2, -1, 0, 1, 2]), [1.4142135623730951, 1, 0, 1, 1.4142135623730951]
 )
+assert_eq(call("ƭ", 6.25), 2.5)
 
 assert_eq(call("ƭ", "abcdef"), "ace")
 assert_eq(call("ƭ", "xyz"), "xz")
 assert_eq(call("ƭ", ""), "")
 
 # ¶
 
 assert_eq(call("¶"), "\n")
 
+# Ç
+
+assert_eq(call("Ç"), "|")
+
 # ¬
 
 assert_eq(call("¬", 123), 0)
 assert_eq(call("¬", 0), 1)
 
 assert_eq(call("¬", "abc"), 0)
 assert_eq(call("¬", ""), 1)
@@ -3112,14 +3125,58 @@
 assert_eq(
     call("Æ~", [11, 12, 13, 14, 15, 16, 17, 18, 19, 20]),
     [-12, -13, -14, -15, -16, -17, -18, -19, -20, -21],
 )
 
 assert_eq(call("Æ~", "abc"), ["abc"])
 
+# Æ²
+
+assert_eq(call("Æ²", 100), 1)
+assert_eq(call("Æ²", 10), 0)
+assert_eq(call("Æ²", 6.25), 0)
+
+assert_eq(call("Æ²", [-3, -2, -1, 0, 1, 2, 3]), [0, 0, 0, 1, 1, 0, 0])
+assert_eq(call("Æ²", [9998, 9999, 10000, 10001, 10002]), [0, 0, 1, 0, 0])
+
+assert_eq(call("Æ²", "abc"), "abc")
+
+# Æ³
+
+assert_eq(call("Æ³", 1000), 1)
+assert_eq(call("Æ³", 100), 0)
+assert_eq(call("Æ³", 15.625), 0)
+
+assert_eq(call("Æ³", [-3, -2, -1, 0, 1, 2, 3]), [0, 0, 0, 1, 1, 0, 0])
+assert_eq(call("Æ³", [998, 999, 1000, 1001, 1002]), [0, 0, 1, 0, 0])
+
+assert_eq(call("Æ³", "abc"), "abc")
+
+# Æ⁴
+
+assert_eq(call("Æ⁴", 256), 1)
+assert_eq(call("Æ⁴", 1000), 0)
+assert_eq(call("Æ⁴", 39.0625), 0)
+
+assert_eq(call("Æ⁴", [-3, -2, -1, 0, 1, 2, 3]), [0, 0, 0, 1, 1, 0, 0])
+assert_eq(call("Æ⁴", [623, 624, 625, 626, 627]), [0, 0, 1, 0, 0])
+
+assert_eq(call("Æ⁴", "abc"), "abc")
+
+# Æ⁵
+
+assert_eq(call("Æ⁵", 1024), 1)
+assert_eq(call("Æ⁵", 512), 0)
+assert_eq(call("Æ⁵", 97.65625), 0)
+
+assert_eq(call("Æ⁵", [-3, -2, -1, 0, 1, 2, 3]), [0, 0, 0, 1, 1, 0, 0])
+assert_eq(call("Æ⁵", [241, 242, 243, 244, 245]), [0, 0, 1, 0, 0])
+
+assert_eq(call("Æ⁵", "abc"), "abc")
+
 # µR
 
 assert_eq(call("µR", 12), "XII")
 assert_eq(call("µR", -4.56), "-IV")
 assert_eq(
     call("µR", [123, 456, 789, 1234, 5678, 9012]),
     ["CXXIII", "CDLVI", "DCCLXXXIX", "MCCXXXIV", "MMMMMDCLXXVIII", "MMMMMMMMMXII"],
@@ -3323,14 +3380,23 @@
 
 assert_eq(call("µ^", -123, "abc"), 0)
 assert_eq(call("µ^", "xyz", 0), 1)
 
 assert_eq(call("µ^", [-1, 0, 1], ["abc", "def", ""]), 0)
 assert_eq(call("µ^", 5, []), 1)
 
+# µ/
+
+assert_eq(call("µ/", "b", "abcbabcba"), ["a", "c", "a", "c", "a"])
+assert_eq(
+    call("µ/", 3, 12345432123454321), [[1, 2], [4, 5, 4], [2, 1, 2], [4, 5, 4], [2, 1]]
+)
+
+assert_eq(call("µ/", 123, [123, 456, 789, 123, 456, 789]), [[], [456, 789], [456, 789]])
+
 # After all the tests
 
 all_commands = (
     [*commands]
     + ["ø" + cmd1 for cmd1 in string_digraphs]
     + ["Ø" + cmd2 for cmd2 in list_digraphs]
     + ["Æ" + cmd3 for cmd3 in random_digraphs_1]
```

### Comparing `thunno2-2.2.1/thunno2/tokens.py` & `thunno2-2.2.2/thunno2/tokens.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,18 +78,17 @@
     "¥": ("fixed_point",),
     "{": ("open_for_loop",),
     "}": ("close_for_loop",),
     "(": ("open_while_loop",),
     ")": ("close_while_loop",),
     "⁽": ("open_forever_loop",),
     "⁾": ("close_forever_loop",),
-    "?": ("if_statement",),
-    ":": ("else_statement",),
+    "?": ("if_statement", "if"),
+    ":": ("else_statement", "else"),
     ";": ("close_statement",),
-    "Ç": ("two_function_map",),
     "ç": ("pair_apply",),
     "n": ("context_variable",),
     "ṅ": ("iteration_index",),
     "x": ("get_x",),
     "y": ("get_y",),
     "X": ("set_x",),
     "Y": ("set_y",),
```

### Comparing `thunno2-2.2.1/thunno2.egg-info/PKG-INFO` & `thunno2-2.2.2/thunno2.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: thunno2
-Version: 2.2.1
+Version: 2.2.2
 Summary: A golfing language
 Home-page: https://github.com/Thunno/Thunno2
 Author: Rujul Nayak
 Author-email: rujulnayak@outlook.com
 License: MIT
-Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.2.1.tar.gz
+Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.2.2.tar.gz
 Keywords: golfing,code-golf,language
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

