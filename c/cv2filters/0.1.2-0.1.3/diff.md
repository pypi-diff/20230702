# Comparing `tmp/cv2filters-0.1.2.tar.gz` & `tmp/cv2filters-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cv2filters-0.1.2.tar", last modified: Sat Jul  1 15:26:53 2023, max compression
+gzip compressed data, was "cv2filters-0.1.3.tar", last modified: Sun Jul  2 07:12:15 2023, max compression
```

## Comparing `cv2filters-0.1.2.tar` & `cv2filters-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 15:26:53.965485 cv2filters-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-01 15:26:34.000000 cv2filters-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-07-01 15:26:53.965485 cv2filters-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8102 2023-07-01 15:26:34.000000 cv2filters-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 15:26:53.965485 cv2filters-0.1.2/cv2filters/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-01 15:26:34.000000 cv2filters-0.1.2/cv2filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16204 2023-07-01 15:26:34.000000 cv2filters-0.1.2/cv2filters/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 15:26:53.965485 cv2filters-0.1.2/cv2filters.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-07-01 15:26:53.000000 cv2filters-0.1.2/cv2filters.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-01 15:26:53.000000 cv2filters-0.1.2/cv2filters.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 15:26:53.000000 cv2filters-0.1.2/cv2filters.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-01 15:26:53.000000 cv2filters-0.1.2/cv2filters.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-01 15:26:53.000000 cv2filters-0.1.2/cv2filters.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 15:26:53.965485 cv2filters-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-01 15:26:34.000000 cv2filters-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:12:15.034077 cv2filters-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-02 07:11:53.000000 cv2filters-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8303 2023-07-02 07:12:15.034077 cv2filters-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7466 2023-07-02 07:11:53.000000 cv2filters-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:12:15.034077 cv2filters-0.1.3/cv2filters/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-02 07:11:53.000000 cv2filters-0.1.3/cv2filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16204 2023-07-02 07:11:53.000000 cv2filters-0.1.3/cv2filters/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:12:15.034077 cv2filters-0.1.3/cv2filters.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8303 2023-07-02 07:12:14.000000 cv2filters-0.1.3/cv2filters.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-02 07:12:14.000000 cv2filters-0.1.3/cv2filters.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 07:12:14.000000 cv2filters-0.1.3/cv2filters.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-02 07:12:14.000000 cv2filters-0.1.3/cv2filters.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-02 07:12:14.000000 cv2filters-0.1.3/cv2filters.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 07:12:15.034077 cv2filters-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-02 07:11:53.000000 cv2filters-0.1.3/setup.py
```

### Comparing `cv2filters-0.1.2/LICENSE` & `cv2filters-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cv2filters-0.1.2/PKG-INFO` & `cv2filters-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: cv2filters
-Version: 0.1.2
-Summary:  Unleash the power of OpenCV with CV2Filters, the ultimate image processing wrapper for all skill levels, revolutionizing computer vision with seamless exploration, manipulation, and groundbreaking research
-Home-page: https://github.com/nuhmanpk/cv2filters
-Author: Nuhman Pk
-Author-email: nuhmanpk7@gmail.com
-License: MIT
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # CV2Filters
 
 CV2Filters a powerful Python package designed as a wrapper around OpenCV, the popular open-source computer vision library. cv2Filters simplifies image processing tasks by providing a higher-level abstraction of the underlying OpenCV functionality. This package aims to make image processing more accessible to both beginner and advanced users, enabling them to efficiently perform a wide range of image manipulation and analysis tasks
 
 CV2Filters empowers users to harness the power of OpenCV in a simplified and intuitive manner. By abstracting away the complexities, the package enables a broader audience to explore image processing, drive innovation, and unlock new possibilities in the field of computer vision.
 
 [![Downloads](https://static.pepy.tech/personalized-badge/cv2filters?period=total&units=international_system&left_color=grey&right_color=yellow&left_text=Total-Downloads)](https://pepy.tech/project/cv2filters)
@@ -45,44 +29,16 @@
 
 ```python
 from cv2filters import Filters
 # Create an instance of the Filters class
 filters = Filters()
 ```
 
-or
-
-```python
-from cv2filters.filters import <function-to-be-used>
-```
-
-
 Now you can use the various filtering functions available in the library. For example, let's show how to use the increase_brightness and apply_blur functions:
 
-```python
-from cv2filters.filters import increase_brightness, apply_blur
-import cv2
-
-image = cv2.imread('image.jpg')
-
-# Increase brightness of the image
-brightened_image = increase_brightness(image, value=50)
-
-# Apply blur to the image
-blurred_image = apply_blur(image, kernel_size=5)
-
-# Display the results
-cv2.imshow('Original Image', image)
-cv2.imshow('Brightened Image', brightened_image)
-cv2.imshow('Blurred Image', blurred_image)
-cv2.waitKey(0)
-cv2.destroyAllWindows()
-```
-
-* Note: Make sure to replace 'image.jpg' with the path to your actual image file.
 
 Create an instance of the Filters class and then call the desired methods on the instance. For example:
 
 ```python
 from cv2filters import Filters
 # Create an instance of the Filters class
 filters = Filters()
@@ -187,20 +143,18 @@
 
 15. **morphological_opening**(image: np.ndarray, kernel: np.ndarray = None, iterations: int = 2) -> np.ndarray:
 This method applies morphological opening to an image to remove noise and small objects.
 
 16. **closing**(image: np.ndarray, kernel: np.ndarray = None, iterations: int = 2) -> np.ndarray:
 This method applies morphological closing to an image to close small holes.
 
-17. **hi1ghlight_box**(image: np.ndarray, box: Tuple[int, int, int, int]) -> np.ndarray:
+17. **highlight_box**(image: np.ndarray, box: Tuple[int, int, int, int]) -> np.ndarray:
 This method highlights a box region in an image by turning the rest of the image to black.
 
 ## Contributing
 
 If you'd like to contribute to this library, please follow these steps:
 
 * Fork the repository.
 * Create a new branch.
 * Make your changes and test them.
 * Submit a pull request.
-
-
```

### Comparing `cv2filters-0.1.2/README.md` & `cv2filters-0.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+Metadata-Version: 2.1
+Name: cv2filters
+Version: 0.1.3
+Summary:  Unleash the power of OpenCV with CV2Filters, the ultimate image processing wrapper for all skill levels, revolutionizing computer vision with seamless exploration, manipulation, and groundbreaking research
+Home-page: https://github.com/nuhmanpk/cv2filters
+Author: Nuhman Pk
+Author-email: nuhmanpk7@gmail.com
+License: MIT
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # CV2Filters
 
 CV2Filters a powerful Python package designed as a wrapper around OpenCV, the popular open-source computer vision library. cv2Filters simplifies image processing tasks by providing a higher-level abstraction of the underlying OpenCV functionality. This package aims to make image processing more accessible to both beginner and advanced users, enabling them to efficiently perform a wide range of image manipulation and analysis tasks
 
 CV2Filters empowers users to harness the power of OpenCV in a simplified and intuitive manner. By abstracting away the complexities, the package enables a broader audience to explore image processing, drive innovation, and unlock new possibilities in the field of computer vision.
 
 [![Downloads](https://static.pepy.tech/personalized-badge/cv2filters?period=total&units=international_system&left_color=grey&right_color=yellow&left_text=Total-Downloads)](https://pepy.tech/project/cv2filters)
@@ -29,44 +49,16 @@
 
 ```python
 from cv2filters import Filters
 # Create an instance of the Filters class
 filters = Filters()
 ```
 
-or
-
-```python
-from cv2filters.filters import <function-to-be-used>
-```
-
-
 Now you can use the various filtering functions available in the library. For example, let's show how to use the increase_brightness and apply_blur functions:
 
-```python
-from cv2filters.filters import increase_brightness, apply_blur
-import cv2
-
-image = cv2.imread('image.jpg')
-
-# Increase brightness of the image
-brightened_image = increase_brightness(image, value=50)
-
-# Apply blur to the image
-blurred_image = apply_blur(image, kernel_size=5)
-
-# Display the results
-cv2.imshow('Original Image', image)
-cv2.imshow('Brightened Image', brightened_image)
-cv2.imshow('Blurred Image', blurred_image)
-cv2.waitKey(0)
-cv2.destroyAllWindows()
-```
-
-* Note: Make sure to replace 'image.jpg' with the path to your actual image file.
 
 Create an instance of the Filters class and then call the desired methods on the instance. For example:
 
 ```python
 from cv2filters import Filters
 # Create an instance of the Filters class
 filters = Filters()
@@ -171,18 +163,20 @@
 
 15. **morphological_opening**(image: np.ndarray, kernel: np.ndarray = None, iterations: int = 2) -> np.ndarray:
 This method applies morphological opening to an image to remove noise and small objects.
 
 16. **closing**(image: np.ndarray, kernel: np.ndarray = None, iterations: int = 2) -> np.ndarray:
 This method applies morphological closing to an image to close small holes.
 
-17. **hi1ghlight_box**(image: np.ndarray, box: Tuple[int, int, int, int]) -> np.ndarray:
+17. **highlight_box**(image: np.ndarray, box: Tuple[int, int, int, int]) -> np.ndarray:
 This method highlights a box region in an image by turning the rest of the image to black.
 
 ## Contributing
 
 If you'd like to contribute to this library, please follow these steps:
 
 * Fork the repository.
 * Create a new branch.
 * Make your changes and test them.
 * Submit a pull request.
+
+
```

### Comparing `cv2filters-0.1.2/cv2filters/filters.py` & `cv2filters-0.1.3/cv2filters/filters.py`

 * *Files identical despite different names*

### Comparing `cv2filters-0.1.2/cv2filters.egg-info/PKG-INFO` & `cv2filters-0.1.3/cv2filters.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 Metadata-Version: 2.1
 Name: cv2filters
-Version: 0.1.2
+Version: 0.1.3
 Summary:  Unleash the power of OpenCV with CV2Filters, the ultimate image processing wrapper for all skill levels, revolutionizing computer vision with seamless exploration, manipulation, and groundbreaking research
 Home-page: https://github.com/nuhmanpk/cv2filters
 Author: Nuhman Pk
 Author-email: nuhmanpk7@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CV2Filters
@@ -45,44 +49,16 @@
 
 ```python
 from cv2filters import Filters
 # Create an instance of the Filters class
 filters = Filters()
 ```
 
-or
-
-```python
-from cv2filters.filters import <function-to-be-used>
-```
-
-
 Now you can use the various filtering functions available in the library. For example, let's show how to use the increase_brightness and apply_blur functions:
 
-```python
-from cv2filters.filters import increase_brightness, apply_blur
-import cv2
-
-image = cv2.imread('image.jpg')
-
-# Increase brightness of the image
-brightened_image = increase_brightness(image, value=50)
-
-# Apply blur to the image
-blurred_image = apply_blur(image, kernel_size=5)
-
-# Display the results
-cv2.imshow('Original Image', image)
-cv2.imshow('Brightened Image', brightened_image)
-cv2.imshow('Blurred Image', blurred_image)
-cv2.waitKey(0)
-cv2.destroyAllWindows()
-```
-
-* Note: Make sure to replace 'image.jpg' with the path to your actual image file.
 
 Create an instance of the Filters class and then call the desired methods on the instance. For example:
 
 ```python
 from cv2filters import Filters
 # Create an instance of the Filters class
 filters = Filters()
@@ -187,15 +163,15 @@
 
 15. **morphological_opening**(image: np.ndarray, kernel: np.ndarray = None, iterations: int = 2) -> np.ndarray:
 This method applies morphological opening to an image to remove noise and small objects.
 
 16. **closing**(image: np.ndarray, kernel: np.ndarray = None, iterations: int = 2) -> np.ndarray:
 This method applies morphological closing to an image to close small holes.
 
-17. **hi1ghlight_box**(image: np.ndarray, box: Tuple[int, int, int, int]) -> np.ndarray:
+17. **highlight_box**(image: np.ndarray, box: Tuple[int, int, int, int]) -> np.ndarray:
 This method highlights a box region in an image by turning the rest of the image to black.
 
 ## Contributing
 
 If you'd like to contribute to this library, please follow these steps:
 
 * Fork the repository.
```

