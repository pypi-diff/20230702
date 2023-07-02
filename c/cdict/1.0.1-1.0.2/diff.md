# Comparing `tmp/cdict-1.0.1.tar.gz` & `tmp/cdict-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdict-1.0.1.tar", last modified: Sat Jul  1 06:35:02 2023, max compression
+gzip compressed data, was "cdict-1.0.2.tar", last modified: Sun Jul  2 03:43:31 2023, max compression
```

## Comparing `cdict-1.0.1.tar` & `cdict-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jeffwu     (503) staff       (20)        0 2023-07-01 06:35:02.570132 cdict-1.0.1/
--rw-r--r--   0 jeffwu     (503) staff       (20)       42 2022-05-24 14:35:55.000000 cdict-1.0.1/.gitignore
--rw-r--r--   0 jeffwu     (503) staff       (20)     1080 2022-05-24 14:35:55.000000 cdict-1.0.1/LICENSE
--rw-r--r--   0 jeffwu     (503) staff       (20)      199 2023-07-01 06:35:02.569545 cdict-1.0.1/PKG-INFO
--rw-r--r--   0 jeffwu     (503) staff       (20)     2599 2023-06-09 16:03:29.000000 cdict-1.0.1/README.md
-drwxr-xr-x   0 jeffwu     (503) staff       (20)        0 2023-07-01 06:35:02.546092 cdict-1.0.1/cdict/
--rw-r--r--   0 jeffwu     (503) staff       (20)       29 2023-02-07 17:31:36.000000 cdict-1.0.1/cdict/__init__.py
--rw-r--r--   0 jeffwu     (503) staff       (20)     4176 2023-07-01 06:26:23.000000 cdict-1.0.1/cdict/main.py
-drwxr-xr-x   0 jeffwu     (503) staff       (20)        0 2023-07-01 06:35:02.560096 cdict-1.0.1/cdict.egg-info/
--rw-r--r--   0 jeffwu     (503) staff       (20)      199 2023-07-01 06:35:01.000000 cdict-1.0.1/cdict.egg-info/PKG-INFO
--rw-r--r--   0 jeffwu     (503) staff       (20)      204 2023-07-01 06:35:01.000000 cdict-1.0.1/cdict.egg-info/SOURCES.txt
--rw-r--r--   0 jeffwu     (503) staff       (20)        1 2023-07-01 06:35:01.000000 cdict-1.0.1/cdict.egg-info/dependency_links.txt
--rw-r--r--   0 jeffwu     (503) staff       (20)        6 2023-07-01 06:35:01.000000 cdict-1.0.1/cdict.egg-info/top_level.txt
--rw-r--r--   0 jeffwu     (503) staff       (20)       38 2023-07-01 06:35:02.570216 cdict-1.0.1/setup.cfg
--rw-r--r--   0 jeffwu     (503) staff       (20)      282 2023-07-01 06:34:54.000000 cdict-1.0.1/setup.py
-drwxr-xr-x   0 jeffwu     (503) staff       (20)        0 2023-07-01 06:35:02.568448 cdict-1.0.1/tests/
--rw-r--r--   0 jeffwu     (503) staff       (20)     5070 2023-06-09 16:03:25.000000 cdict-1.0.1/tests/test_main.py
+drwxr-xr-x   0 jeffwu     (503) staff       (20)        0 2023-07-02 03:43:31.283189 cdict-1.0.2/
+-rw-r--r--   0 jeffwu     (503) staff       (20)       42 2022-05-24 14:35:55.000000 cdict-1.0.2/.gitignore
+-rw-r--r--   0 jeffwu     (503) staff       (20)     1080 2022-05-24 14:35:55.000000 cdict-1.0.2/LICENSE
+-rw-r--r--   0 jeffwu     (503) staff       (20)      199 2023-07-02 03:43:31.282728 cdict-1.0.2/PKG-INFO
+-rw-r--r--   0 jeffwu     (503) staff       (20)     3053 2023-07-02 03:39:44.000000 cdict-1.0.2/README.md
+drwxr-xr-x   0 jeffwu     (503) staff       (20)        0 2023-07-02 03:43:31.274032 cdict-1.0.2/cdict/
+-rw-r--r--   0 jeffwu     (503) staff       (20)       29 2023-02-07 17:31:36.000000 cdict-1.0.2/cdict/__init__.py
+-rw-r--r--   0 jeffwu     (503) staff       (20)     5108 2023-07-02 03:41:48.000000 cdict-1.0.2/cdict/main.py
+drwxr-xr-x   0 jeffwu     (503) staff       (20)        0 2023-07-02 03:43:31.281280 cdict-1.0.2/cdict.egg-info/
+-rw-r--r--   0 jeffwu     (503) staff       (20)      199 2023-07-02 03:43:30.000000 cdict-1.0.2/cdict.egg-info/PKG-INFO
+-rw-r--r--   0 jeffwu     (503) staff       (20)      204 2023-07-02 03:43:30.000000 cdict-1.0.2/cdict.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffwu     (503) staff       (20)        1 2023-07-02 03:43:30.000000 cdict-1.0.2/cdict.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffwu     (503) staff       (20)        6 2023-07-02 03:43:30.000000 cdict-1.0.2/cdict.egg-info/top_level.txt
+-rw-r--r--   0 jeffwu     (503) staff       (20)       38 2023-07-02 03:43:31.283261 cdict-1.0.2/setup.cfg
+-rw-r--r--   0 jeffwu     (503) staff       (20)      282 2023-07-02 03:43:25.000000 cdict-1.0.2/setup.py
+drwxr-xr-x   0 jeffwu     (503) staff       (20)        0 2023-07-02 03:43:31.281977 cdict-1.0.2/tests/
+-rw-r--r--   0 jeffwu     (503) staff       (20)     7469 2023-07-02 03:43:14.000000 cdict-1.0.2/tests/test_main.py
```

### Comparing `cdict-1.0.1/LICENSE` & `cdict-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cdict-1.0.1/tests/test_main.py` & `cdict-1.0.2/tests/test_main.py`

 * *Files 22% similar despite different names*

```diff
@@ -29,14 +29,23 @@
         found = 0
         for d2 in dicts2:
             if d1 == d2:
                 found += 1
         assert found == 1
 
 
+def test_multilist():
+    c = C.dict(a=C.list(1, 2), b=C.list(1, 2))
+    assert_dicts(c, [
+        dict(a=1, b=1),
+        dict(a=1, b=2),
+        dict(a=2, b=1),
+        dict(a=2, b=2),
+    ])
+
 def test_simple():
     c0 = C.dict(a=5, b=3)
     assert_dicts(c0, [dict(a=5, b=3)])
 
     c1 = C.dict(a=5, b=C.list(3, 30))
     assert_dicts(c1, [dict(a=5, b=3), dict(a=5, b=30)])
 
@@ -82,14 +91,72 @@
     assert_dicts(c8, [
         dict(a=0, b=0),
         dict(a=0, b=1),
         dict(a=1, b=0),
         dict(a=1, b=1),
     ])
 
+def test_nested_times():
+    c0 = C.dict(a=C.dict(a=C.list(1, 2)))
+    assert_dicts(c0, [dict(a=dict(a=1)), dict(a=dict(a=2))])
+    c1 = C.dict(a=C.dict(b=C.list(1, 2)))
+    assert_dicts(c1, [dict(a=dict(b=1)), dict(a=dict(b=2))])
+
+    assert_dicts(c0 * c1, [
+        dict(a=dict(a=1, b=1)),
+        dict(a=dict(a=1, b=2)),
+        dict(a=dict(a=2, b=1)),
+        dict(a=dict(a=2, b=2)),
+    ])
+
+    # normal dict can't get overridden
+    c0 = C.dict(a=dict(a=1)) + C.dict(a=dict(a=2))
+    assert_dicts(c0, [dict(a=dict(a=1)), dict(a=dict(a=2))])
+    c1 = C.dict(a=C.dict(b=C.list(1, 2)))
+    assert_dicts(c1, [dict(a=dict(b=1)), dict(a=dict(b=2))])
+    with pytest.raises(ValueError):
+        list(c0 * c1)
+
+    # finaldict can't get overridden
+    c0 = C.dict(a=C.finaldict(a=C.list(1, 2)))
+    assert_dicts(c0, [dict(a=dict(a=1)), dict(a=dict(a=2))])
+    c1 = C.dict(a=C.dict(b=C.list(1, 2)))
+    assert_dicts(c1, [dict(a=dict(b=1)), dict(a=dict(b=2))])
+    with pytest.raises(ValueError):
+        list(c0 * c1)
+
+    c0 = C.dict(a=C.dict(a=C.list(1, 2)))
+    c1 = C.dict(a=C.dict(a=C.list(3, 4)))
+
+    with pytest.raises(ValueError):
+        list(c0 * c1)
+
+    c0 = C.dict(a=C.dict(a=C.finaldict(a=1)))
+    assert_dicts(c0, [dict(a=dict(a=dict(a=1)))])
+    c1 = C.dict(a=C.dict(b=C.finaldict(a=1)))
+    assert_dicts(c1, [dict(a=dict(b=dict(a=1)))])
+
+    assert_dicts(c0 * c1, [
+        dict(a=dict(a=dict(a=1), b=dict(a=1))),
+    ])
+
+    # finaldict can't get overridden
+    c0 = C.dict(a=C.finaldict(a=C.list(1, 2)))
+    assert_dicts(c0, [dict(a=dict(a=1)), dict(a=dict(a=2))])
+    c1 = C.dict(b=C.finaldict(b=C.list(1, 2)))
+    assert_dicts(c1, [dict(b=dict(b=1)), dict(b=dict(b=2))])
+    assert_dicts(c0 * c1, [
+        dict(a=dict(a=1), b=dict(b=1)),
+        dict(a=dict(a=1), b=dict(b=2)),
+        dict(a=dict(a=2), b=dict(b=1)),
+        dict(a=dict(a=2), b=dict(b=2)),
+    ])
+
+
+
 def test_overwriting():
     c0 = C.dict(a=5, b=3)
     c1 = C.dict(a=6, c=4)
     with pytest.raises(ValueError):
         assert_dicts(c0 * c1, [
             dict(a=6, b=3, c=4),
         ])
@@ -100,14 +167,18 @@
 
     c0 = C.dict(a=summing_number(5), b=summing_number(3))
     c1 = C.dict(a=summing_number(6), c=summing_number(4))
     assert_dicts(c0 * c1, [
         dict(a=11, b=3, c=4),
     ])
 
+    assert_dicts(c0 | c1, [
+        dict(a=11, b=3, c=4),
+    ])
+
     class overriding_number(int):
         def cdict_combine(self, other):
             return overriding_number(other)
 
     c0 = C.dict(a=overriding_number(5), b=overriding_number(3))
     c1 = C.dict(a=overriding_number(6), c=overriding_number(4))
     c2 = C.dict(a=overriding_number(7), d=overriding_number(5))
@@ -115,26 +186,31 @@
         dict(a=7, b=3, c=4, d=5),
     ])
 
 
 def test_or():
     c0 = C.dict(a=5, b=3)
     c1 = C.dict(a=6, c=4)
-    assert_dicts(c0 | c1, [
-        dict(a=6, b=3, c=4),
-    ])
+    with pytest.raises(ValueError):
+        assert_dicts(c0 | c1, [
+            dict(a=6, b=3, c=4),
+        ])
 
     c0 = C.dict(a=C.list(5, 6), b=3)
     c1 = C.dict(c=C.list(4, 3))
     assert_dicts(c0 | c1, [
         dict(a=5, b=3, c=4),
         dict(a=6, b=3, c=3),
     ])
 
-    c0 = C.dict(a=C.list(5, 6), b=3)
+    class overriding_number(int):
+        def cdict_combine(self, other):
+            return overriding_number(other)
+
+    c0 = C.dict(a=C.list(overriding_number(5), overriding_number(6)), b=3)
     c1 = C.dict(a=6, c=C.list(4, 3))
     assert_dicts(c0 | c1, [
         dict(a=6, b=3, c=4),
         dict(a=6, b=3, c=3),
     ])
 
     with pytest.raises(ValueError):
@@ -166,13 +242,15 @@
     code = m.group(1)
     assert code.startswith('python')
     code = code[6:].strip()
     exec(code, globals(), globals())
 
 
 if __name__ == "__main__":
+    test_multilist()
     test_simple()
     test_overwriting()
+    test_nested_times()
     test_or()
     test_distributive()
     test_commutative_mult()
     test_readme_code()
```

