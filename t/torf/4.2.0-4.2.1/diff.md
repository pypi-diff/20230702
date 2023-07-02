# Comparing `tmp/torf-4.2.0.tar.gz` & `tmp/torf-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torf-4.2.0.tar", last modified: Sun Apr 16 12:04:20 2023, max compression
+gzip compressed data, was "torf-4.2.1.tar", last modified: Sun Jul  2 10:22:17 2023, max compression
```

## Comparing `torf-4.2.0.tar` & `torf-4.2.1.tar`

### file list

```diff
@@ -1,39 +1,41 @@
-drwx------   0 ich       (1000) ich       (1000)        0 2023-04-16 12:04:20.671871 torf-4.2.0/
--rw-------   0 ich       (1000) ich       (1000)    35149 2020-04-02 09:42:44.000000 torf-4.2.0/LICENSE
--rw-------   0 ich       (1000) ich       (1000)     3002 2023-04-16 12:04:20.671871 torf-4.2.0/PKG-INFO
--rw-------   0 ich       (1000) ich       (1000)     2135 2022-04-26 14:13:06.000000 torf-4.2.0/README.rst
--rw-------   0 ich       (1000) ich       (1000)       38 2023-04-16 12:04:20.671871 torf-4.2.0/setup.cfg
--rw-------   0 ich       (1000) ich       (1000)     1575 2022-11-09 17:40:17.000000 torf-4.2.0/setup.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-04-16 12:04:20.663871 torf-4.2.0/tests/
--rw-------   0 ich       (1000) ich       (1000)    19972 2022-04-21 17:08:25.000000 torf-4.2.0/tests/__init__.py
--rw-------   0 ich       (1000) ich       (1000)    23891 2022-11-24 15:38:20.000000 torf-4.2.0/tests/conftest.py
--rw-------   0 ich       (1000) ich       (1000)    61584 2023-04-13 10:06:18.000000 torf-4.2.0/tests/test_attributes.py
--rw-------   0 ich       (1000) ich       (1000)     1925 2020-06-20 13:29:35.000000 torf-4.2.0/tests/test_convert.py
--rw-------   0 ich       (1000) ich       (1000)    11832 2020-08-10 16:19:53.000000 torf-4.2.0/tests/test_exclude.py
--rw-------   0 ich       (1000) ich       (1000)     1638 2020-06-20 13:29:35.000000 torf-4.2.0/tests/test_fuzzy.py
--rw-------   0 ich       (1000) ich       (1000)     9854 2022-11-24 15:38:58.000000 torf-4.2.0/tests/test_generate.py
--rw-------   0 ich       (1000) ich       (1000)    24994 2020-06-20 13:29:35.000000 torf-4.2.0/tests/test_magnet.py
--rw-------   0 ich       (1000) ich       (1000)     3918 2020-06-20 13:29:35.000000 torf-4.2.0/tests/test_partial_size.py
--rw-------   0 ich       (1000) ich       (1000)     9712 2023-04-13 10:06:18.000000 torf-4.2.0/tests/test_read.py
--rw-------   0 ich       (1000) ich       (1000)    29898 2023-01-09 14:33:59.000000 torf-4.2.0/tests/test_reuse.py
--rw-------   0 ich       (1000) ich       (1000)    90416 2023-01-25 18:04:55.000000 torf-4.2.0/tests/test_stream.py
--rw-------   0 ich       (1000) ich       (1000)    30054 2023-04-13 10:16:39.000000 torf-4.2.0/tests/test_utils.py
--rw-------   0 ich       (1000) ich       (1000)    16381 2023-04-13 10:06:18.000000 torf-4.2.0/tests/test_validate.py
--rw-------   0 ich       (1000) ich       (1000)    29451 2023-04-16 11:50:39.000000 torf-4.2.0/tests/test_verify_content.py
--rw-------   0 ich       (1000) ich       (1000)    20528 2022-04-20 10:54:04.000000 torf-4.2.0/tests/test_verify_filesize.py
--rw-------   0 ich       (1000) ich       (1000)     2844 2020-06-20 13:29:35.000000 torf-4.2.0/tests/test_write.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-04-16 12:04:20.671871 torf-4.2.0/torf/
--rw-------   0 ich       (1000) ich       (1000)      891 2023-04-16 11:50:39.000000 torf-4.2.0/torf/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     9952 2023-04-13 10:06:18.000000 torf-4.2.0/torf/_errors.py
--rw-------   0 ich       (1000) ich       (1000)    20636 2023-01-09 11:27:27.000000 torf-4.2.0/torf/_generate.py
--rw-------   0 ich       (1000) ich       (1000)    13957 2022-07-05 14:26:08.000000 torf-4.2.0/torf/_magnet.py
--rw-------   0 ich       (1000) ich       (1000)     7132 2023-03-12 14:07:48.000000 torf-4.2.0/torf/_reuse.py
--rw-------   0 ich       (1000) ich       (1000)    30268 2023-01-25 17:51:42.000000 torf-4.2.0/torf/_stream.py
--rw-------   0 ich       (1000) ich       (1000)    68659 2023-04-13 10:06:18.000000 torf-4.2.0/torf/_torrent.py
--rw-------   0 ich       (1000) ich       (1000)    25915 2023-04-16 11:21:14.000000 torf-4.2.0/torf/_utils.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-04-16 12:04:20.671871 torf-4.2.0/torf.egg-info/
--rw-------   0 ich       (1000) ich       (1000)     3002 2023-04-16 12:04:20.000000 torf-4.2.0/torf.egg-info/PKG-INFO
--rw-------   0 ich       (1000) ich       (1000)      674 2023-04-16 12:04:20.000000 torf-4.2.0/torf.egg-info/SOURCES.txt
--rw-------   0 ich       (1000) ich       (1000)        1 2023-04-16 12:04:20.000000 torf-4.2.0/torf.egg-info/dependency_links.txt
--rw-------   0 ich       (1000) ich       (1000)       19 2023-04-16 12:04:20.000000 torf-4.2.0/torf.egg-info/requires.txt
--rw-------   0 ich       (1000) ich       (1000)        5 2023-04-16 12:04:20.000000 torf-4.2.0/torf.egg-info/top_level.txt
+drwx------   0 ich       (1000) ich       (1000)        0 2023-07-02 10:22:17.687585 torf-4.2.1/
+-rw-------   0 ich       (1000) ich       (1000)    35149 2020-04-02 09:42:44.000000 torf-4.2.1/LICENSE
+-rw-------   0 ich       (1000) ich       (1000)     3278 2023-07-02 10:22:17.687585 torf-4.2.1/PKG-INFO
+-rw-------   0 ich       (1000) ich       (1000)     2135 2022-04-26 14:13:06.000000 torf-4.2.1/README.rst
+drwx------   0 ich       (1000) ich       (1000)        0 2023-07-02 10:22:17.679585 torf-4.2.1/docs/
+-rw-------   0 ich       (1000) ich       (1000)      143 2018-01-20 16:09:50.000000 torf-4.2.1/docs/conf.py
+-rw-------   0 ich       (1000) ich       (1000)     1745 2023-07-02 09:55:50.000000 torf-4.2.1/pyproject.toml
+-rw-------   0 ich       (1000) ich       (1000)       38 2023-07-02 10:22:17.687585 torf-4.2.1/setup.cfg
+drwx------   0 ich       (1000) ich       (1000)        0 2023-07-02 10:22:17.683585 torf-4.2.1/tests/
+-rw-------   0 ich       (1000) ich       (1000)    19972 2022-04-21 17:08:25.000000 torf-4.2.1/tests/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)    23891 2022-11-24 15:38:20.000000 torf-4.2.1/tests/conftest.py
+-rw-------   0 ich       (1000) ich       (1000)    66320 2023-07-02 10:05:57.000000 torf-4.2.1/tests/test_attributes.py
+-rw-------   0 ich       (1000) ich       (1000)     1925 2020-06-20 13:29:35.000000 torf-4.2.1/tests/test_convert.py
+-rw-------   0 ich       (1000) ich       (1000)    11832 2020-08-10 16:19:53.000000 torf-4.2.1/tests/test_exclude.py
+-rw-------   0 ich       (1000) ich       (1000)     1638 2020-06-20 13:29:35.000000 torf-4.2.1/tests/test_fuzzy.py
+-rw-------   0 ich       (1000) ich       (1000)     9854 2022-11-24 15:38:58.000000 torf-4.2.1/tests/test_generate.py
+-rw-------   0 ich       (1000) ich       (1000)    24994 2020-06-20 13:29:35.000000 torf-4.2.1/tests/test_magnet.py
+-rw-------   0 ich       (1000) ich       (1000)     3918 2020-06-20 13:29:35.000000 torf-4.2.1/tests/test_partial_size.py
+-rw-------   0 ich       (1000) ich       (1000)     9712 2023-04-13 10:06:18.000000 torf-4.2.1/tests/test_read.py
+-rw-------   0 ich       (1000) ich       (1000)    29898 2023-01-09 14:33:59.000000 torf-4.2.1/tests/test_reuse.py
+-rw-------   0 ich       (1000) ich       (1000)    90416 2023-01-25 18:04:55.000000 torf-4.2.1/tests/test_stream.py
+-rw-------   0 ich       (1000) ich       (1000)    30096 2023-07-02 10:05:57.000000 torf-4.2.1/tests/test_utils.py
+-rw-------   0 ich       (1000) ich       (1000)    16381 2023-04-13 10:06:18.000000 torf-4.2.1/tests/test_validate.py
+-rw-------   0 ich       (1000) ich       (1000)    29465 2023-07-02 10:05:57.000000 torf-4.2.1/tests/test_verify_content.py
+-rw-------   0 ich       (1000) ich       (1000)    20528 2022-04-20 10:54:04.000000 torf-4.2.1/tests/test_verify_filesize.py
+-rw-------   0 ich       (1000) ich       (1000)     2844 2020-06-20 13:29:35.000000 torf-4.2.1/tests/test_write.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-07-02 10:22:17.683585 torf-4.2.1/torf/
+-rw-------   0 ich       (1000) ich       (1000)      891 2023-07-02 10:18:45.000000 torf-4.2.1/torf/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     9952 2023-04-13 10:06:18.000000 torf-4.2.1/torf/_errors.py
+-rw-------   0 ich       (1000) ich       (1000)    20661 2023-07-02 10:05:57.000000 torf-4.2.1/torf/_generate.py
+-rw-------   0 ich       (1000) ich       (1000)    13985 2023-07-02 10:05:57.000000 torf-4.2.1/torf/_magnet.py
+-rw-------   0 ich       (1000) ich       (1000)     7132 2023-03-12 14:07:48.000000 torf-4.2.1/torf/_reuse.py
+-rw-------   0 ich       (1000) ich       (1000)    30246 2023-07-02 10:05:57.000000 torf-4.2.1/torf/_stream.py
+-rw-------   0 ich       (1000) ich       (1000)    69033 2023-07-02 10:02:58.000000 torf-4.2.1/torf/_torrent.py
+-rw-------   0 ich       (1000) ich       (1000)    25903 2023-07-02 10:05:57.000000 torf-4.2.1/torf/_utils.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-07-02 10:22:17.687585 torf-4.2.1/torf.egg-info/
+-rw-------   0 ich       (1000) ich       (1000)     3278 2023-07-02 10:22:17.000000 torf-4.2.1/torf.egg-info/PKG-INFO
+-rw-------   0 ich       (1000) ich       (1000)      693 2023-07-02 10:22:17.000000 torf-4.2.1/torf.egg-info/SOURCES.txt
+-rw-------   0 ich       (1000) ich       (1000)        1 2023-07-02 10:22:17.000000 torf-4.2.1/torf.egg-info/dependency_links.txt
+-rw-------   0 ich       (1000) ich       (1000)      118 2023-07-02 10:22:17.000000 torf-4.2.1/torf.egg-info/requires.txt
+-rw-------   0 ich       (1000) ich       (1000)       26 2023-07-02 10:22:17.000000 torf-4.2.1/torf.egg-info/top_level.txt
```

### Comparing `torf-4.2.0/LICENSE` & `torf-4.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `torf-4.2.0/PKG-INFO` & `torf-4.2.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 Metadata-Version: 2.1
 Name: torf
-Version: 4.2.0
+Version: 4.2.1
 Summary: Python 3 module for creating and parsing torrent files and magnet URIs
-Home-page: https://github.com/rndusr/torf
-Author: Random User
-Author-email: rndusr@posteo.de
-License: GPLv3+
-Keywords: bittorrent torrent magnet
+Author-email: Random User <rndusr@posteo.de>
+License: GPL-3.0-or-later
+Project-URL: Repository, https://github.com/rndusr/torf
+Project-URL: Documentation, https://torf.readthedocs.io/
+Project-URL: Bug Tracker, https://github.com/rndusr/torf/issues
+Project-URL: Changelog, https://raw.githubusercontent.com/rndusr/torf/master/CHANGELOG
+Keywords: bittorrent,torrent,magnet
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.7, ==3.*
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+Provides-Extra: dev
 License-File: LICENSE
 
 torf
 ====
 
 torf provides a ``Torrent`` and a ``Magnet`` class.
```

### Comparing `torf-4.2.0/README.rst` & `torf-4.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `torf-4.2.0/tests/__init__.py` & `torf-4.2.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `torf-4.2.0/tests/conftest.py` & `torf-4.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `torf-4.2.0/tests/test_attributes.py` & `torf-4.2.1/tests/test_attributes.py`

 * *Files 3% similar despite different names*

```diff
@@ -236,15 +236,15 @@
     assert torrent.metainfo['info']['name'] == 'foo'
     assert torrent.metainfo['info']['length'] == 4
     assert 'pieces' in torrent.metainfo['info']
     assert torrent.files == (torf.File(Path('foo'), size=4),)
 
 def test_files_needs_common_path(create_torrent, tmp_path):
     content = tmp_path / 'asdf' ; content.mkdir()  # noqa: E702
-    for i in range(1, 3): (content / f'file{i}').write_text('<data>')
+    for i in range(1, 3): (content / f'file{i}').write_text('<data>')  # noqa: E701
     torrent = create_torrent(path=content)
     torrent.generate()
     with pytest.raises(torf.CommonPathError) as excinfo:
         torrent.files = (torf.File(Path('foo/bar/baz'), size=123),
                          torf.File(Path('quux/bar/bam'), size=456),)
     assert str(excinfo.value) == 'No common parent path: foo/bar/baz, quux/bar/bam'
 
@@ -253,15 +253,15 @@
                                                  {'path': ['file2'], 'length': 6}]
     assert torrent.metainfo['info']['name'] == 'asdf'
     assert 'pieces' in torrent.metainfo['info']
     assert 'length' not in torrent.metainfo['info']
 
 def test_files_updates_metainfo_when_manipulated(create_torrent, tmp_path):
     content = tmp_path / 'bar' ; content.mkdir()  # noqa: E702
-    for i in range(1, 3): (content / f'file{i}').write_text('<data>')
+    for i in range(1, 3): (content / f'file{i}').write_text('<data>')  # noqa: E701
     torrent = create_torrent(path=content)
     torrent.generate()
     assert torrent.metainfo['info']['name'] == 'bar'
     assert 'pieces' in torrent.metainfo['info']
     assert 'length' not in torrent.metainfo['info']
     assert torrent.files == (torf.File(Path('bar', 'file1'), size=6),
                              torf.File(Path('bar', 'file2'), size=6),)
@@ -822,17 +822,17 @@
             None, None,
             errors.PieceSizeError(456),
             id='Invalid custom piece_size_max',
         ),
     ),
     ids=lambda v: repr(v),
 )
-def test_piece_size_min_max(piece_size_, piece_size_min, piece_size_max,
-                            exp_piece_size_max, exp_piece_size_min, exp_exception,
-                            with_path, singlefile_content, mocker):
+def test_piece_size_min_max_arguments(piece_size_, piece_size_min, piece_size_max,
+                                      exp_piece_size_max, exp_piece_size_min, exp_exception,
+                                      with_path, singlefile_content, mocker):
     mocker.patch.object(torf.Torrent, 'piece_size_min_default', PIECE_SIZE_MIN_DEFAULT)
     mocker.patch.object(torf.Torrent, 'piece_size_max_default', PIECE_SIZE_MAX_DEFAULT)
 
     if exp_exception:
         with pytest.raises(type(exp_exception), match=rf'^{re.escape(str(exp_exception))}$'):
             torf.Torrent(
                 path=singlefile_content.path if with_path else None,
@@ -855,14 +855,131 @@
         assert torrent.piece_size_min == exp_piece_size_min
         assert torrent.piece_size_max == exp_piece_size_max
         assert torrent.piece_size_min_default == PIECE_SIZE_MIN_DEFAULT
         assert torrent.piece_size_max_default == PIECE_SIZE_MAX_DEFAULT
 
 
 @pytest.mark.parametrize(
+    argnames=(
+        'old_piece_size, new_piece_size, piece_size_min, piece_size_max, order,'
+        'exp_piece_size, exp_piece_size_min, exp_piece_size_max, exp_exception'
+    ),
+    argvalues=(
+        pytest.param(
+            0, 524288, 131072, 1048576, 'piece_size_is_set_first',
+            524288, 131072, 1048576,
+            None,
+            id='old_piece_size=0; new_piece_size between min/max; piece_size_is_set_first',
+        ),
+        pytest.param(
+            0, 524288, 131072, 1048576, 'min_max_is_set_first',
+            524288, 131072, 1048576,
+            None,
+            id='old_piece_size=0; new_piece_size between min/max; min_max_is_set_first',
+        ),
+
+        pytest.param(
+            0, 65536, 131072, 1048576, 'piece_size_is_set_first',
+            131072, 131072, 1048576,
+            None,
+            id='old_piece_size=0; new_piece_size < min; piece_size_is_set_first',
+        ),
+        pytest.param(
+            0, 65536, 131072, 1048576, 'min_max_is_set_first',
+            0, 131072, 1048576,
+            errors.PieceSizeError(65536, min=131072, max=1048576),
+            id='old_piece_size=0; new_piece_size < min; min_max_is_set_first',
+        ),
+
+        pytest.param(
+            0, 1048576 * 2, 131072, 1048576, 'piece_size_is_set_first',
+            1048576, 131072, 1048576,
+            None,
+            id='old_piece_size=0; new_piece_size > max; piece_size_is_set_first',
+        ),
+        pytest.param(
+            0, 1048576 * 2, 131072, 1048576, 'min_max_is_set_first',
+            0, 131072, 1048576,
+            errors.PieceSizeError(1048576 * 2, min=131072, max=1048576),
+            id='old_piece_size=0; new_piece_size > max; min_max_is_set_first',
+        ),
+
+        pytest.param(
+            262144, 524288, 131072, 1048576, 'piece_size_is_set_first',
+            524288, 131072, 1048576,
+            None,
+            id='old_piece_size=262144; new_piece_size between min/max; piece_size_is_set_first',
+        ),
+        pytest.param(
+            262144, 524288, 131072, 1048576, 'min_max_is_set_first',
+            524288, 131072, 1048576,
+            None,
+            id='old_piece_size=262144; new_piece_size between min/max; min_max_is_set_first',
+        ),
+
+        pytest.param(
+            262144, 65536, 131072, 1048576, 'piece_size_is_set_first',
+            131072, 131072, 1048576,
+            None,
+            id='old_piece_size=262144; new_piece_size < min; piece_size_is_set_first',
+        ),
+        pytest.param(
+            262144, 65536, 131072, 1048576, 'min_max_is_set_first',
+            262144, 131072, 1048576,
+            errors.PieceSizeError(65536, min=131072, max=1048576),
+            id='old_piece_size=262144; new_piece_size < min; min_max_is_set_first',
+        ),
+
+        pytest.param(
+            262144, 1048576 * 2, 131072, 1048576, 'piece_size_is_set_first',
+            1048576, 131072, 1048576,
+            None,
+            id='old_piece_size=262144; new_piece_size > max; piece_size_is_set_first',
+        ),
+        pytest.param(
+            262144, 1048576 * 2, 131072, 1048576, 'min_max_is_set_first',
+            262144, 131072, 1048576,
+            errors.PieceSizeError(1048576 * 2, min=131072, max=1048576),
+            id='old_piece_size=262144; new_piece_size > max; min_max_is_set_first',
+        ),
+    ),
+    ids=lambda v: repr(v),
+)
+def test_piece_size_min_max_attributes(old_piece_size, new_piece_size, piece_size_min, piece_size_max, order,
+                                       exp_piece_size, exp_piece_size_min, exp_piece_size_max, exp_exception,
+                                       singlefile_content, mocker):
+    mocker.patch.object(torf.Torrent, 'piece_size_min_default', 0)
+    mocker.patch.object(torf.Torrent, 'piece_size_max_default', float('inf'))
+
+    torrent = torf.Torrent()
+    torrent.metainfo['info']['piece length'] = old_piece_size
+    assert torrent.piece_size == old_piece_size
+
+    def do_test():
+        if order == 'piece_size_is_set_first':
+            torrent.piece_size = new_piece_size
+            torrent.piece_size_min = piece_size_min
+            torrent.piece_size_max = piece_size_max
+        else:
+            torrent.piece_size_min = piece_size_min
+            torrent.piece_size_max = piece_size_max
+            torrent.piece_size = new_piece_size
+
+    if exp_exception:
+        with pytest.raises(type(exp_exception), match=rf'^{re.escape(str(exp_exception))}$'):
+            do_test()
+    else:
+        do_test()
+
+    assert torrent.piece_size == exp_piece_size
+    assert torrent.piece_size_min == exp_piece_size_min
+    assert torrent.piece_size_max == exp_piece_size_max
+
+
+@pytest.mark.parametrize(
     argnames='kwargs, cls_attrs',
     argvalues=(
         ({'min_size': 1024, 'max_size': 256 * 2**20}, {}),
         ({}, {'piece_size_min_default': 1024, 'piece_size_max_default': 256 * 2**20}),
         ({'min_size': 1024, 'max_size': 256 * 2**20}, {'piece_size_min_default': 1048576, 'piece_size_max_default': 1048576 * 2}),
     ),
 )
```

### Comparing `torf-4.2.0/tests/test_convert.py` & `torf-4.2.1/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `torf-4.2.0/tests/test_exclude.py` & `torf-4.2.1/tests/test_exclude.py`

 * *Files identical despite different names*

### Comparing `torf-4.2.0/tests/test_fuzzy.py` & `torf-4.2.1/tests/test_fuzzy.py`

 * *Files identical despite different names*

### Comparing `torf-4.2.0/tests/test_generate.py` & `torf-4.2.1/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `torf-4.2.0/tests/test_magnet.py` & `torf-4.2.1/tests/test_magnet.py`

 * *Files identical despite different names*

### Comparing `torf-4.2.0/tests/test_partial_size.py` & `torf-4.2.1/tests/test_partial_size.py`

 * *Files identical despite different names*

### Comparing `torf-4.2.0/tests/test_read.py` & `torf-4.2.1/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `torf-4.2.0/tests/test_reuse.py` & `torf-4.2.1/tests/test_reuse.py`

 * *Files identical despite different names*

### Comparing `torf-4.2.0/tests/test_stream.py` & `torf-4.2.1/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `torf-4.2.0/tests/test_utils.py` & `torf-4.2.1/tests/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -388,23 +388,23 @@
         assert fps == ('foo', tmp_path / 'cwd' / 'bar')
     finally:
         os.chdir(cwd)
 
 def test_Filepaths_handles_directories(tmp_path):
     # Create directory with 2 files
     content = tmp_path / 'content' ; content.mkdir()  # noqa: E702
-    for f in ('a', 'b'): (content / f).write_text('<data>')
+    for f in ('a', 'b'): (content / f).write_text('<data>')  # noqa: E701
     fps = utils.Filepaths((content,))
     assert fps == (content / 'a', content / 'b')
 
     # Replace one file with multilevel subdirectory
     subdir = content / 'b' ; subdir.unlink() ; subdir.mkdir()  # noqa: E702
-    for f in ('c', 'd'): (subdir / f).write_text('<subdata>')
+    for f in ('c', 'd'): (subdir / f).write_text('<subdata>')  # noqa: E701
     subsubdir = subdir / 'subsubdir' ; subsubdir.mkdir()  # noqa: E702
-    for f in ('e', 'f'): (subsubdir / f).write_text('<subdata>')
+    for f in ('e', 'f'): (subsubdir / f).write_text('<subdata>')  # noqa: E701
     fps[1] = content / 'b'
     assert fps == (content / 'a', subdir / 'c', subdir / 'd', subsubdir / 'e', subsubdir / 'f')
 
     # Replace subdirectory with file again
     for f in (subdir / 'c', subdir / 'd', subsubdir / 'e', subsubdir / 'f'):
         f.unlink()
     subsubdir.rmdir()
```

### Comparing `torf-4.2.0/tests/test_validate.py` & `torf-4.2.1/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `torf-4.2.0/tests/test_verify_content.py` & `torf-4.2.1/tests/test_verify_content.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,18 +5,30 @@
 import random
 from unittest import mock
 
 import pytest
 
 import torf
 
-from . import (ComparableException, calc_corruptions, calc_good_pieces,
-               calc_piece_indexes, calc_pieces_done, change_file_size,
-               display_filespecs, file_piece_indexes, file_range, fuzzylist,
-               pos2file, pos2files, random_positions, round_down_to_multiple)
+from . import (
+    ComparableException,
+    calc_corruptions,
+    calc_good_pieces,
+    calc_piece_indexes,
+    calc_pieces_done,
+    change_file_size,
+    display_filespecs,
+    file_piece_indexes,
+    file_range,
+    fuzzylist,
+    pos2file,
+    pos2files,
+    random_positions,
+    round_down_to_multiple,
+)
 
 import logging  # isort:skip
 debug = logging.getLogger('test').debug
 
 
 # Allow arbitrary small piece sizes to make debugging easier.
 @pytest.fixture(autouse=True)
```

### Comparing `torf-4.2.0/tests/test_verify_filesize.py` & `torf-4.2.1/tests/test_verify_filesize.py`

 * *Files identical despite different names*

### Comparing `torf-4.2.0/tests/test_write.py` & `torf-4.2.1/tests/test_write.py`

 * *Files identical despite different names*

### Comparing `torf-4.2.0/torf/__init__.py` & `torf-4.2.1/torf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,14 @@
 
 # flake8: noqa
 
 """
 Create and parse torrent files and magnet URIs
 """
 
-__version__ = '4.2.0'
+__version__ = '4.2.1'
 
 from ._errors import *
 from ._magnet import Magnet
 from ._stream import TorrentFileStream
 from ._torrent import Torrent
 from ._utils import File, Filepath
```

### Comparing `torf-4.2.0/torf/_errors.py` & `torf-4.2.1/torf/_errors.py`

 * *Files identical despite different names*

### Comparing `torf-4.2.0/torf/_generate.py` & `torf-4.2.1/torf/_generate.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,15 +244,16 @@
     def _handle_piece(self, piece_index, filepath, piece, exceptions):
         if exceptions:
             # _debug(f'{_thread_name()}: Forwarding exceptions for #{piece_index}: {exceptions!r}')
             self._hash_queue.put((piece_index, filepath, None, exceptions))
 
         elif piece:
             piece_hash = sha1(piece).digest()
-            # _debug(f'{_thread_name()}: Hashed #{piece_index}: {_pretty_bytes(piece)} [{len(piece)} bytes] -> {piece_hash}')
+            # _debug(f'{_thread_name()}: Hashed #{piece_index}: '
+            #        f'{_pretty_bytes(piece)} [{len(piece)} bytes] -> {piece_hash}')
             self._hash_queue.put((piece_index, filepath, piece_hash, ()))
 
         else:
             # _debug(f'{_thread_name()}: Nothing to hash for #{piece_index}: {piece!r}')
             self._hash_queue.put((piece_index, filepath, None, ()))
 
     def _janitor_thread(self):
```

### Comparing `torf-4.2.0/torf/_magnet.py` & `torf-4.2.1/torf/_magnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,16 +286,16 @@
         :return: ``True`` if the "info" section was successfully downloaded,
             ``False`` otherwise
         """
         def success():
             return hasattr(self, '_info')
 
         torrent_urls = []
-        if self.xs: torrent_urls.append(self.xs)
-        if self.as_: torrent_urls.append(self.as_)
+        if self.xs: torrent_urls.append(self.xs)  # noqa: E701
+        if self.as_: torrent_urls.append(self.as_)  # noqa: E701
         torrent_urls.extend((url.rstrip('/') + '.torrent' for url in self.ws))
         # I couldn't find any documentation for the "/file?info_hash=..." GET request, but
         # it seems to work for HTTP trackers.
         # https://stackoverflow.com/a/1019588
         for url in self.tr:
             if url.scheme in ('http', 'https'):
                 infohash_enc = urllib.parse.quote_from_bytes(binascii.unhexlify(self.infohash))
```

### Comparing `torf-4.2.0/torf/_reuse.py` & `torf-4.2.1/torf/_reuse.py`

 * *Files identical despite different names*

### Comparing `torf-4.2.0/torf/_stream.py` & `torf-4.2.1/torf/_stream.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import errno
-import functools
 import hashlib
 import itertools
 import math
 import os
 
 from . import _errors as error
 
@@ -539,15 +538,15 @@
 
         return iter_pieces(fh, prepend), skip_bytes
 
     def _read_from_fh(self, fh, size, oom_callback):
         while True:
             try:
                 return fh.read(size)
-            except MemoryError as e:
+            except MemoryError:
                 e = error.MemoryError(f'Out of memory while reading from {fh.name} at position {fh.tell()}')
                 if oom_callback is None:
                     raise e
                 else:
                     oom_callback(e)
 
     def get_piece_hash(self, piece_index, content_path=None):
```

### Comparing `torf-4.2.0/torf/_torrent.py` & `torf-4.2.1/torf/_torrent.py`

 * *Files 1% similar despite different names*

```diff
@@ -632,46 +632,52 @@
             self.metainfo['info']['piece length'] = piece_length
 
     @property
     def piece_size_min(self):
         """
         Smallest allowed piece size
 
-        Setting :attr:`piece_size` to a smaller value raises
-        :class:`PieceSizeError`.
+        Setting this property also sets :attr:`piece_size` to the same value if
+        it is smaller.
         """
         return self._piece_size_min
 
     @piece_size_min.setter
     def piece_size_min(self, piece_size_min):
         if piece_size_min is None:
             self._piece_size_min = type(self).piece_size_min_default
         elif not utils.is_divisible_by_16_kib(piece_size_min):
             raise error.PieceSizeError(piece_size_min)
         else:
             self._piece_size_min = int(piece_size_min)
+            # If a piece size is set, silently limit it to new minimum
+            if self.piece_size:
+                self.piece_size = max(self.piece_size_min, self.piece_size)
 
     @property
     def piece_size_max(self):
         """
-        Smallest allowed piece size
+        Largest allowed piece size
 
-        Setting :attr:`piece_size` to a smaller value raises
-        :class:`PieceSizeError`.
+        Setting this property also sets :attr:`piece_size` to the same value if
+        it is bigger.
         """
         return self._piece_size_max
 
     @piece_size_max.setter
     def piece_size_max(self, piece_size_max):
         if piece_size_max is None:
             self._piece_size_max = type(self).piece_size_max_default
         elif not utils.is_divisible_by_16_kib(piece_size_max):
             raise error.PieceSizeError(piece_size_max)
         else:
             self._piece_size_max = int(piece_size_max)
+            # If a piece size is set, silently limit it to new maximum
+            if self.piece_size:
+                self.piece_size = min(self.piece_size_max, self.piece_size)
 
     piece_size_min_default = 16 * 1024  # 16 KiB
     """
     Smallest allowed piece size (default value)
 
     Setting :attr:`piece_size` to a smaller value raises
     :class:`PieceSizeError`.
```

### Comparing `torf-4.2.0/torf/_utils.py` & `torf-4.2.1/torf/_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 import collections
 import contextlib
 import errno
 import fnmatch
 import functools
 import http.client
 import itertools
-import math
 import os
 import pathlib
 import re
 import socket
 import typing
 import urllib.error
 import urllib.parse
```

### Comparing `torf-4.2.0/torf.egg-info/PKG-INFO` & `torf-4.2.1/torf.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 Metadata-Version: 2.1
 Name: torf
-Version: 4.2.0
+Version: 4.2.1
 Summary: Python 3 module for creating and parsing torrent files and magnet URIs
-Home-page: https://github.com/rndusr/torf
-Author: Random User
-Author-email: rndusr@posteo.de
-License: GPLv3+
-Keywords: bittorrent torrent magnet
+Author-email: Random User <rndusr@posteo.de>
+License: GPL-3.0-or-later
+Project-URL: Repository, https://github.com/rndusr/torf
+Project-URL: Documentation, https://torf.readthedocs.io/
+Project-URL: Bug Tracker, https://github.com/rndusr/torf/issues
+Project-URL: Changelog, https://raw.githubusercontent.com/rndusr/torf/master/CHANGELOG
+Keywords: bittorrent,torrent,magnet
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.7, ==3.*
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+Provides-Extra: dev
 License-File: LICENSE
 
 torf
 ====
 
 torf provides a ``Torrent`` and a ``Magnet`` class.
```

### Comparing `torf-4.2.0/torf.egg-info/SOURCES.txt` & `torf-4.2.1/torf.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 README.rst
-setup.py
+pyproject.toml
+docs/conf.py
 tests/__init__.py
 tests/conftest.py
 tests/test_attributes.py
 tests/test_convert.py
 tests/test_exclude.py
 tests/test_fuzzy.py
 tests/test_generate.py
```

