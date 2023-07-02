# Comparing `tmp/katalytic_images-0.7.0.tar.gz` & `tmp/katalytic_images-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic_images-0.7.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "katalytic_images-0.9.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `katalytic_images-0.7.0.tar` & `katalytic_images-0.9.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      109 2023-04-09 19:59:19.451546 katalytic_images-0.7.0/.coveragerc
--rw-r--r--   0        0        0      651 2023-05-01 06:38:08.285250 katalytic_images-0.7.0/.gitignore
--rw-r--r--   0        0        0     3308 2023-05-05 03:58:55.053635 katalytic_images-0.7.0/.gitlab-ci.yml
--rw-r--r--   0        0        0     3831 2023-06-29 18:12:27.326416 katalytic_images-0.7.0/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2023-04-06 18:07:34.500276 katalytic_images-0.7.0/LICENSE.txt
--rw-r--r--   0        0        0     2218 2023-05-31 06:28:52.615620 katalytic_images-0.7.0/README.md
--rw-r--r--   0        0        0     1549 2023-06-29 18:12:27.326416 katalytic_images-0.7.0/pyproject.toml
--rw-r--r--   0        0        0    23618 2023-06-29 18:06:33.150349 katalytic_images-0.7.0/src/katalytic/images.py
--rw-r--r--   0        0        0    18056 2023-06-29 18:05:45.304863 katalytic_images-0.7.0/tests/test_images.py
--rw-r--r--   0        0        0     3694 1970-01-01 00:00:00.000000 katalytic_images-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      109 2023-04-09 19:59:19.451546 katalytic_images-0.9.0/.coveragerc
+-rw-r--r--   0        0        0      651 2023-05-01 06:38:08.285250 katalytic_images-0.9.0/.gitignore
+-rw-r--r--   0        0        0     3308 2023-05-05 03:58:55.053635 katalytic_images-0.9.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0     4677 2023-07-02 19:13:45.536276 katalytic_images-0.9.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2023-04-06 18:07:34.500276 katalytic_images-0.9.0/LICENSE.txt
+-rw-r--r--   0        0        0     2218 2023-05-31 06:28:52.615620 katalytic_images-0.9.0/README.md
+-rw-r--r--   0        0        0     1549 2023-07-02 19:13:45.536276 katalytic_images-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    25454 2023-07-02 16:16:38.305751 katalytic_images-0.9.0/src/katalytic/images.py
+-rw-r--r--   0        0        0    20897 2023-07-02 16:07:05.753628 katalytic_images-0.9.0/tests/test_images.py
+-rw-r--r--   0        0        0     3694 1970-01-01 00:00:00.000000 katalytic_images-0.9.0/PKG-INFO
```

### Comparing `katalytic_images-0.7.0/.gitignore` & `katalytic_images-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `katalytic_images-0.7.0/.gitlab-ci.yml` & `katalytic_images-0.9.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `katalytic_images-0.7.0/CHANGELOG.md` & `katalytic_images-0.9.0/CHANGELOG.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+## 0.9.0 (2023-07-02)
+### feat
+- [[`b0f8c86`](https://gitlab.com/katalytic/katalytic-images/commit/b0f8c868e3035ea13ab8c65af18876cd933dabd3)] make save_image() atomic
+
+
+## 0.8.0 (2023-07-02)
+### feat
+- [[`b0f8c86`](https://gitlab.com/katalytic/katalytic-images/commit/b0f8c868e3035ea13ab8c65af18876cd933dabd3)] make save_image() atomic
+
+
+## 0.10.0 (2023-07-02)
+### feat
+- [[`b0f8c86`](https://gitlab.com/katalytic/katalytic-images/commit/b0f8c868e3035ea13ab8c65af18876cd933dabd3)] make save_image() atomic
+
+
+## 0.9.0 (2023-07-02)
+### feat
+- [[`b0f8c86`](https://gitlab.com/katalytic/katalytic-images/commit/b0f8c868e3035ea13ab8c65af18876cd933dabd3)] make save_image() atomic
+
+
+## 0.8.0 (2023-07-02)
+### feat
+- [[`b0f8c86`](https://gitlab.com/katalytic/katalytic-images/commit/b0f8c868e3035ea13ab8c65af18876cd933dabd3)] make save_image() atomic
+
+
 ## 0.7.0 (2023-06-29)
 ### feat
 - [[`1783c35`](https://gitlab.com/katalytic/katalytic-images/commit/1783c354f5a1da45b5784d065481ef568b80a8a7)] warn when using the wrong saver/loader
 ### fix
 - [[`1f2e027`](https://gitlab.com/katalytic/katalytic-images/commit/1f2e02761af8ee18199841432f2e41af4e9248a6)] some edge case import issues
```

### Comparing `katalytic_images-0.7.0/LICENSE.txt` & `katalytic_images-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic_images-0.7.0/README.md` & `katalytic_images-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `katalytic_images-0.7.0/pyproject.toml` & `katalytic_images-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "katalytic-images"
-version = "0.7.0"
+version = "0.9.0"
 description = "This plugin adds utilities for working with images and videos to the katalytic namespace"
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
```

### Comparing `katalytic_images-0.7.0/src/katalytic/images.py` & `katalytic_images-0.9.0/src/katalytic/images.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import PIL.Image
 __PIL_Image_open = PIL.Image.open
 __PIL_Image_Image = PIL.Image.Image
 
 # noinspection PyProtectedMember
 from katalytic.data import _UNDEFINED
 from katalytic.data.checks import is_iterable, is_number, is_sequence
-from katalytic.pkg import get_version, mark
+from katalytic.pkg import get_version, mark, KatalyticInterrupt
 
 __version__, __version_info__ = get_version(__name__)
 
 
 def bhwc(arr):
     """
     Returns a tuple representing the shape of the input array in the BHWC format: batch, height, width, and channels. The missing dimensions are filled with 1s.
@@ -600,29 +600,67 @@
         if exists == 'error':
             raise FileExistsError(f'[Errno {errno.EEXIST}] File exists: {str(path)!r}')
         elif exists == 'replace':
             pass  # continue executing
         elif exists == 'skip':
             return
 
-    dest_dir = Path(path).parent
-    if make_dirs:
-        from katalytic.files import make_dir
-        make_dir(dest_dir, create_parents=True, exists_ok=True)
-    elif not dest_dir.exists():
-        raise FileNotFoundError(f'[Errno {errno.ENOENT}] Directory does not exist: {str(dest_dir)!r}')
-    elif dest_dir.is_file():
-        raise NotADirectoryError(f'[Errno {errno.ENOTDIR}] Not a directory: {str(dest_dir)!r}')
+    try:
+        dest_dir = Path(path).parent
+        if make_dirs:
+            from katalytic.files import make_dir
+            make_dir(dest_dir, create_parents=True, exists_ok=True)
+        elif not dest_dir.exists():
+            raise FileNotFoundError(f'[Errno {errno.ENOENT}] Directory does not exist: {str(dest_dir)!r}')
+        elif dest_dir.is_file():
+            raise NotADirectoryError(f'[Errno {errno.ENOTDIR}] Not a directory: {str(dest_dir)!r}')
+
+        if isinstance(image, __PIL_Image_Image):
+            image = __np_array(image)
+
+        if isinstance(image, __np_ndarray):
+            if mode != 'BGR':
+                image = convert_image(image, mode, 'BGR')
+
+            ext = str(path).rpartition('.')[2]
+            tmp_path = f'{path}.part.{ext}'
+            __cv2_imwrite(tmp_path, image)
+
+            if save_image.__katalytic_test_atomicity_race_condition__:
+                save_image.__katalytic_test_atomicity_race_condition__ = False
+
+                # I can't use save_image('race condition', path) directly
+                # It would replace the tmp_path = f'{path}.part' created above
+                # and then move it to the target `path`. This function wouldn't
+                # be able to find the tmp_path anymore and will throw an error
+                # at the end of the function: `Path(tmp_path).rename(path)`
+                tmp_path_2 = f'{path}.part2.{ext}'
+                save_image(np.array([[[0,255,0]]], dtype=np.uint8), tmp_path_2)
+                Path(tmp_path_2).rename(path)
+
+            # Checking these conditions again to make the function
+            # as robust as possible against race conditions
+            if Path(path).exists():
+                if exists == 'error':
+                    raise FileExistsError(f'[Errno {errno.EEXIST}] File exists: {str(path)!r}')
+                elif exists == 'replace':
+                    pass  # continue executing
+                elif exists == 'skip':
+                    return
+
+            if save_image.__katalytic_test_atomicity_interrupt__:
+                save_image.__katalytic_test_atomicity_interrupt__ = False
+                raise KatalyticInterrupt(f'Testing atomicity ...')
+
+            Path(tmp_path).rename(path)
+        elif isinstance(image, (str, Path)):
+            from katalytic.files import copy_file
+            copy_file(image, path, exists=exists)
+        else:
+            raise TypeError(f'type(image) = {type(image)!r}')
+    except BaseException as e:
+        if not isinstance(e, KatalyticInterrupt):
+            raise
 
-    if isinstance(image, __PIL_Image_Image):
-        image = __np_array(image)
 
-    if isinstance(image, __np_ndarray):
-        if mode != 'BGR':
-            image = convert_image(image, mode, 'BGR')
-
-        __cv2_imwrite(str(path), image)
-    elif isinstance(image, (str, Path)):
-        from katalytic.files import copy_file
-        copy_file(image, path, exists=exists)
-    else:
-        raise TypeError(f'type(image) = {type(image)!r}')
+save_image.__katalytic_test_atomicity_interrupt__ = False
+save_image.__katalytic_test_atomicity_race_condition__ = False
```

### Comparing `katalytic_images-0.7.0/tests/test_images.py` & `katalytic_images-0.9.0/tests/test_images.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import cv2
 import numpy as np
 import PIL.Image
 import pytest
 from PIL import Image
 
 from katalytic.data import all_types_besides
-from katalytic.files import get_unique_path, load, load_csv, load_json, load_text, move_file, save, save_csv, save_json, save_text
+from katalytic.files import delete_file, get_unique_path, load, load_csv, load_json, load_text, move_file, save, save_csv, save_json, save_text
 from katalytic.images import bhwc, convert_image, create_circle, create_line, create_mask, create_polylines, create_rectangle, create_text, draw, hw, hwc, are_arrays_equal, load_image, save_image
 
 
 def _create_RGB(dtype=np.uint8):
     return np.array([
         [[255, 0, 0], [0, 255, 0], [0, 0, 255]],        # RGB
         [[0, 255, 255], [255, 0, 255], [255, 255, 0]],  # CMY
@@ -319,14 +319,91 @@
             _create_RGB(np.float32),
             _create_RGB(np.uint8),
             check_type=True
         )
 
 
 class Test_load_and_save:
+    def test_atomicity_interrupt(self):
+        path = get_unique_path('{}.png')
+        data = _create_RGB()
+
+        try:
+            save_image.__katalytic_test_atomicity_interrupt__ = True
+            save_image(data, path)
+            assert not Path(path).exists()
+
+            # make sure it's still working after the test
+            # the atomicity flag is set back to False inside the function
+            save_image(data, path)
+            assert are_arrays_equal(load(path), data)
+        except:
+            raise
+
+    def test_atomicity_race_condition_error(self):
+        path = get_unique_path('{}.png')
+        data = _create_RGB()
+
+        try:
+            save_image.__katalytic_test_atomicity_race_condition__ = True
+            assert not Path(path).exists()
+            with pytest.raises(FileExistsError):
+                save_image(data, path, exists='error')
+
+            expected = np.array([[[0,255,0]]], dtype=np.uint8)
+            assert are_arrays_equal(load(path), expected)
+
+            # make sure it's still working after the test
+            # the atomicity flag is set back to False inside the function
+            delete_file(path)
+            assert not Path(path).exists()
+            save_image(data, path, exists='error')
+            assert are_arrays_equal(load(path), data)
+        except:
+            raise
+
+    def test_atomicity_race_condition_replace(self):
+        path = get_unique_path('{}.png')
+        data = _create_RGB()
+
+        try:
+            save_image.__katalytic_test_atomicity_race_condition__ = True
+            assert not Path(path).exists()
+            save_image(data, path, exists='replace')
+            assert are_arrays_equal(load(path), data)
+
+            # make sure it's still working after the test
+            # the atomicity flag is set back to False inside the function
+            delete_file(path)
+            assert not Path(path).exists()
+            save_image(data, path, exists='replace')
+            assert are_arrays_equal(load(path), data)
+        except:
+            raise
+
+    def test_atomicity_race_condition_skip(self):
+        path = get_unique_path('{}.png')
+        data = _create_RGB()
+
+        try:
+            save_image.__katalytic_test_atomicity_race_condition__ = True
+            assert not Path(path).exists()
+            save_image(data, path, exists='skip')
+            expected = np.array([[[0,255,0]]], dtype=np.uint8)
+            assert are_arrays_equal(load(path), expected)
+
+            # make sure it's still working after the test
+            # the atomicity flag is set back to False inside the function
+            delete_file(path)
+            assert not Path(path).exists()
+            save_image(data, path, exists='skip')
+            assert are_arrays_equal(load(path), data)
+        except:
+            raise
+
     # noinspection PyBroadException
     @pytest.mark.parametrize('ext, wrong_load, correct_load', [
         ('jpeg', load_csv, 'load_image'),
         ('jpg', load_json, 'load_image'),
         ('png', load_text, 'load_image'),
     ])
     def test_using_the_wrong_loader_should_always_warn(self, ext, wrong_load, correct_load):
```

### Comparing `katalytic_images-0.7.0/PKG-INFO` & `katalytic_images-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katalytic-images
-Version: 0.7.0
+Version: 0.9.0
 Summary: This plugin adds utilities for working with images and videos to the katalytic namespace
 Author-email: Valentin Neagu <vali19th@protonmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

