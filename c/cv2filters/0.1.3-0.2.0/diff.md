# Comparing `tmp/cv2filters-0.1.3.tar.gz` & `tmp/cv2filters-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cv2filters-0.1.3.tar", last modified: Sun Jul  2 07:12:15 2023, max compression
+gzip compressed data, was "cv2filters-0.2.0.tar", last modified: Sun Jul  2 12:07:54 2023, max compression
```

## Comparing `cv2filters-0.1.3.tar` & `cv2filters-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:12:15.034077 cv2filters-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-02 07:11:53.000000 cv2filters-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8303 2023-07-02 07:12:15.034077 cv2filters-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7466 2023-07-02 07:11:53.000000 cv2filters-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:12:15.034077 cv2filters-0.1.3/cv2filters/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-02 07:11:53.000000 cv2filters-0.1.3/cv2filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16204 2023-07-02 07:11:53.000000 cv2filters-0.1.3/cv2filters/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:12:15.034077 cv2filters-0.1.3/cv2filters.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8303 2023-07-02 07:12:14.000000 cv2filters-0.1.3/cv2filters.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-02 07:12:14.000000 cv2filters-0.1.3/cv2filters.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 07:12:14.000000 cv2filters-0.1.3/cv2filters.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-02 07:12:14.000000 cv2filters-0.1.3/cv2filters.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-02 07:12:14.000000 cv2filters-0.1.3/cv2filters.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 07:12:15.034077 cv2filters-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-02 07:11:53.000000 cv2filters-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:07:54.099502 cv2filters-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-02 12:07:28.000000 cv2filters-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8303 2023-07-02 12:07:54.099502 cv2filters-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7466 2023-07-02 12:07:28.000000 cv2filters-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:07:54.099502 cv2filters-0.2.0/cv2filters/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-02 12:07:28.000000 cv2filters-0.2.0/cv2filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18668 2023-07-02 12:07:28.000000 cv2filters-0.2.0/cv2filters/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:07:54.099502 cv2filters-0.2.0/cv2filters.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8303 2023-07-02 12:07:54.000000 cv2filters-0.2.0/cv2filters.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-02 12:07:54.000000 cv2filters-0.2.0/cv2filters.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 12:07:54.000000 cv2filters-0.2.0/cv2filters.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-02 12:07:54.000000 cv2filters-0.2.0/cv2filters.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-02 12:07:54.000000 cv2filters-0.2.0/cv2filters.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 12:07:54.099502 cv2filters-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-02 12:07:28.000000 cv2filters-0.2.0/setup.py
```

### Comparing `cv2filters-0.1.3/LICENSE` & `cv2filters-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cv2filters-0.1.3/PKG-INFO` & `cv2filters-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cv2filters
-Version: 0.1.3
+Version: 0.2.0
 Summary:  Unleash the power of OpenCV with CV2Filters, the ultimate image processing wrapper for all skill levels, revolutionizing computer vision with seamless exploration, manipulation, and groundbreaking research
 Home-page: https://github.com/nuhmanpk/cv2filters
 Author: Nuhman Pk
 Author-email: nuhmanpk7@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cv2filters-0.1.3/README.md` & `cv2filters-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `cv2filters-0.1.3/cv2filters/filters.py` & `cv2filters-0.2.0/cv2filters/filters.py`

 * *Files 3% similar despite different names*

```diff
@@ -173,15 +173,19 @@
         Returns:
             np.ndarray: The grayscale image as a NumPy array.
         """
         if not isinstance(image, np.ndarray):
             raise ValueError("Input 'image' must be a NumPy array.")
 
         try:
-            grayscale_image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
+            #grayscale_image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
+            if len(image.shape) == 3:
+                grayscale_image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
+            else:
+                grayscale_image = image
             return grayscale_image
         except cv2.error as e:
             raise ValueError(f"OpenCV error: {str(e)}")
 
     @staticmethod
     def detect_edges(image: np.ndarray, threshold1: float = 100, threshold2: float = 200) -> np.ndarray:
         """
@@ -432,8 +436,80 @@
         elif method == 'adaptive_thresholding':
             segmented_image = cv2.adaptiveThreshold(
                 image, 255, cv2.ADAPTIVE_THRESH_MEAN_C, cv2.THRESH_BINARY, 11, 2)
         else:
             raise ValueError(
                 "Invalid segmentation method. Supported methods are 'simple_thresholding' and 'adaptive_thresholding'.")
 
-        return segmented_image
+        return segmented_image
+
+    @staticmethod
+    def image_negative(image: np.ndarray) -> np.ndarray:
+        """
+        Compute the negative of an image.
+
+        Args:
+            image (np.ndarray): The input image as a NumPy array.
+
+        Returns:
+            np.ndarray: The negative image as a NumPy array.
+        """
+        try:
+            negative_image = 255 - image
+            return negative_image
+        except cv2.error as e:
+            raise ValueError(f"OpenCV error: {str(e)}")
+
+    @staticmethod
+    def histogram_correction(image: np.ndarray) -> np.ndarray:
+        """
+        Apply histogram correction to the image.
+
+        Args:
+            image (np.ndarray): The input image as a NumPy array.
+
+        Returns:
+            np.ndarray: The histogram-corrected image as a NumPy array.
+        """
+        try:
+            # gray_image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
+            if len(image.shape) == 3:
+                gray_image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
+            else:
+                gray_image = image
+            equalized_image = cv2.equalizeHist(gray_image)
+            return equalized_image
+        except cv2.error as e:
+            raise ValueError(f"OpenCV error: {str(e)}")
+
+    @staticmethod
+    def pencil(image: np.ndarray) -> np.ndarray:
+        """
+        Apply a pencil sketch effect to the image.
+
+        Args:
+            image (np.ndarray): The input image as a NumPy array.
+
+        Returns:
+            np.ndarray: The image with a pencil sketch effect applied, as a NumPy array.
+        """
+        try:
+            if len(image.shape) == 3:
+                gray_image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
+            else:
+                gray_image = image
+
+            kernel_size = 5  
+            kernel = np.ones((kernel_size, kernel_size),
+                                np.float32) / (kernel_size * kernel_size)
+            blurred_image = cv2.filter2D(gray_image, -1, kernel)  
+
+
+            pencil_image = cv2.divide(gray_image, blurred_image, scale=255)
+
+
+            if len(image.shape) == 3:
+                        pencil_image = cv2.cvtColor(pencil_image, cv2.COLOR_GRAY2BGR)
+            
+            return pencil_image
+        except cv2.error as e:
+            raise ValueError(f"OpenCV error: {str(e)}")
```

### Comparing `cv2filters-0.1.3/cv2filters.egg-info/PKG-INFO` & `cv2filters-0.2.0/cv2filters.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cv2filters
-Version: 0.1.3
+Version: 0.2.0
 Summary:  Unleash the power of OpenCV with CV2Filters, the ultimate image processing wrapper for all skill levels, revolutionizing computer vision with seamless exploration, manipulation, and groundbreaking research
 Home-page: https://github.com/nuhmanpk/cv2filters
 Author: Nuhman Pk
 Author-email: nuhmanpk7@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cv2filters-0.1.3/setup.py` & `cv2filters-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 file = pathlib.Path(__file__).parent
 
 README = (file / "README.md").read_text()
 
 setuptools.setup(
     name="cv2filters",
-    version="0.1.3",
+    version="0.2.0",
     author="Nuhman Pk",
     author_email="nuhmanpk7@gmail.com",
     long_description = README,
     long_description_content_type = "text/markdown",
     description=" Unleash the power of OpenCV with CV2Filters, the ultimate image processing wrapper for all skill levels, revolutionizing computer vision with seamless exploration, manipulation, and groundbreaking research",
     license="MIT",
     url="https://github.com/nuhmanpk/cv2filters",
```

