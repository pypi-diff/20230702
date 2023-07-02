# Comparing `tmp/moosez-2.1.7.tar.gz` & `tmp/moosez-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moosez-2.1.7.tar", last modified: Fri Jun 30 20:20:06 2023, max compression
+gzip compressed data, was "moosez-2.1.8.tar", last modified: Sun Jul  2 12:54:44 2023, max compression
```

## Comparing `moosez-2.1.7.tar` & `moosez-2.1.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:20:06.167757 moosez-2.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-30 20:19:50.000000 moosez-2.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-30 20:20:06.163757 moosez-2.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-06-30 20:19:50.000000 moosez-2.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:20:06.163757 moosez-2.1.7/moosez/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-30 20:19:50.000000 moosez-2.1.7/moosez/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-06-30 20:19:50.000000 moosez-2.1.7/moosez/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-06-30 20:19:50.000000 moosez-2.1.7/moosez/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-06-30 20:19:50.000000 moosez-2.1.7/moosez/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-06-30 20:19:50.000000 moosez-2.1.7/moosez/file_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-06-30 20:19:50.000000 moosez-2.1.7/moosez/image_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    21997 2023-06-30 20:19:50.000000 moosez-2.1.7/moosez/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-06-30 20:19:50.000000 moosez-2.1.7/moosez/input_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-06-30 20:19:50.000000 moosez-2.1.7/moosez/moosez.py
--rw-r--r--   0 runner    (1001) docker     (123)    11697 2023-06-30 20:19:50.000000 moosez-2.1.7/moosez/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-06-30 20:19:50.000000 moosez-2.1.7/moosez/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:20:06.163757 moosez-2.1.7/moosez.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-30 20:20:06.000000 moosez-2.1.7/moosez.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-30 20:20:06.000000 moosez-2.1.7/moosez.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 20:20:06.000000 moosez-2.1.7/moosez.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-30 20:20:06.000000 moosez-2.1.7/moosez.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-30 20:20:06.000000 moosez-2.1.7/moosez.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 20:20:06.000000 moosez-2.1.7/moosez.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 20:20:06.167757 moosez-2.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-30 20:19:50.000000 moosez-2.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:54:44.413198 moosez-2.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-02 12:54:35.000000 moosez-2.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-02 12:54:44.413198 moosez-2.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-07-02 12:54:35.000000 moosez-2.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:54:44.413198 moosez-2.1.8/moosez/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-02 12:54:35.000000 moosez-2.1.8/moosez/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-07-02 12:54:35.000000 moosez-2.1.8/moosez/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-07-02 12:54:35.000000 moosez-2.1.8/moosez/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-07-02 12:54:35.000000 moosez-2.1.8/moosez/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-07-02 12:54:35.000000 moosez-2.1.8/moosez/file_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-07-02 12:54:35.000000 moosez-2.1.8/moosez/image_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21966 2023-07-02 12:54:35.000000 moosez-2.1.8/moosez/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-07-02 12:54:35.000000 moosez-2.1.8/moosez/input_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-07-02 12:54:35.000000 moosez-2.1.8/moosez/moosez.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11863 2023-07-02 12:54:35.000000 moosez-2.1.8/moosez/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-02 12:54:35.000000 moosez-2.1.8/moosez/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:54:44.413198 moosez-2.1.8/moosez.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-02 12:54:44.000000 moosez-2.1.8/moosez.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-02 12:54:44.000000 moosez-2.1.8/moosez.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 12:54:44.000000 moosez-2.1.8/moosez.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-02 12:54:44.000000 moosez-2.1.8/moosez.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-02 12:54:44.000000 moosez-2.1.8/moosez.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-02 12:54:44.000000 moosez-2.1.8/moosez.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 12:54:44.413198 moosez-2.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-02 12:54:35.000000 moosez-2.1.8/setup.py
```

### Comparing `moosez-2.1.7/LICENSE` & `moosez-2.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `moosez-2.1.7/PKG-INFO` & `moosez-2.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moosez
-Version: 2.1.7
+Version: 2.1.8
 Summary: An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks
 Home-page: https://github.com/QIMP-Team/mooseZ
 Author: Lalith Kumar Shiyam Sundar
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
 License: Apache 2.0
 Keywords: moosez model-zoo nnUNet medical-imaging tumor-segmentation organ-segmentation bone-segmentation lung-segmentation muscle-segmentation fat-segmentation vessel-segmentation vertebral-segmentation rib-segmentation preclinical-segmentation clinical-segmentation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `moosez-2.1.7/README.md` & `moosez-2.1.8/README.md`

 * *Files identical despite different names*

### Comparing `moosez-2.1.7/moosez/constants.py` & `moosez-2.1.8/moosez/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,23 +50,24 @@
 Z_AXIS_THRESHOLD = 200
 MARGIN_PADDING = 20
 INTERPOLATION = 'bspline'
 CHUNK_THRESHOLD = 200
 
 # FILE NAMES PREFIX
 
-ORGANS_MULTILABEL_SUFFIX = 'Organs-Multilabel-'
-LUNGS_MULTILABEL_SUFFIX = 'Lungs-Multilabel-'
-MULTILABEL_SUFFIX = 'MULTILABEL-'
+ORGANS_MULTILABEL_PREFIX = 'Organs-Multilabel-'
+LUNGS_MULTILABEL_PREFIX = 'Lungs-Multilabel-'
+MULTILABEL_PREFIX = 'MULTILABEL-'
 
 # FILE NAMES
 
 RESAMPLED_IMAGE_FILE_NAME = 'resampled_image_0000.nii.gz'
 RESAMPLED_MASK_FILE_NAME = 'resampled_mask.nii.gz'
-
+CHUNK_FILENAMES = ["chunk01_0000.nii.gz", "chunk02_0000.nii.gz", "chunk03_0000.nii.gz"]
+CHUNK_PREFIX = 'chunk'
 
 # ORGAN INDICES
 
 ORGAN_INDICES = {
     "clin_ct_organs": {
         1: "spleen",
         2: "kidney_right",
```

### Comparing `moosez-2.1.7/moosez/display.py` & `moosez-2.1.8/moosez/display.py`

 * *Files 8% similar despite different names*

```diff
@@ -93,28 +93,27 @@
     modality = model_info['Modality']
 
     # check for special case where 'FDG-PET-CT' should be split into 'FDG-PET' and 'CT'
     if modality == 'FDG-PET-CT':
         modalities = ['FDG-PET', 'CT']
     else:
         modalities = [modality]
-    expected_suffix = [m.replace('-', '_') + "_" for m in modalities]
+    expected_prefix = [m.replace('-', '_') + "_" for m in modalities]
 
     print(
-        f" Imaging: {constants.ANSI_ORANGE}{model_info['Imaging']}{constants.ANSI_RESET} |"
-        f" Modality: {constants.ANSI_ORANGE}{modality}{constants.ANSI_RESET} | "
-        f"Tissue of interest: {constants.ANSI_ORANGE}{model_info['Tissue of interest']}{constants.ANSI_RESET}")
+        f" Imaging: {model_info['Imaging']} |"
+        f" Modality: {modality} | "
+        f"Tissue of interest: {model_info['Tissue of interest']}")
     print(
-        f" Required modalities: {constants.ANSI_ORANGE}{modalities}{constants.ANSI_RESET} | "
-        f" No. of modalities: {constants.ANSI_ORANGE}{len(modalities)}{constants.ANSI_RESET}"
-        f" | Required Suffix for non-DICOM files: {constants.ANSI_ORANGE}{expected_suffix}"
-        f"{constants.ANSI_RESET}")
+        f" Required modalities: {modalities} | "
+        f" No. of modalities: {len(modalities)}"
+        f" | Required prefix for non-DICOM files: {expected_prefix}")
     logging.info(f" Required modalities: {modalities} |  No. of modalities: {len(modalities)} "
-                 f"| Required Suffix for non-DICOM files: {expected_suffix} ")
+                 f"| Required prefix for non-DICOM files: {expected_prefix} ")
     print(
-        f"{constants.ANSI_ORANGE} Warning: Subjects which don't have the required modalities [check file suffix] "
+        f"{constants.ANSI_ORANGE} Warning: Subjects which don't have the required modalities [check file prefix] "
         f"will be skipped. {constants.ANSI_RESET}")
-    warning_message = " Skipping subjects without the required modalities (check file suffix).\n" \
+    warning_message = " Skipping subjects without the required modalities (check file prefix).\n" \
                       " These subjects will be excluded from analysis and their data will not be used."
     logging.warning(warning_message)
 
     return modalities
```

### Comparing `moosez-2.1.7/moosez/download.py` & `moosez-2.1.8/moosez/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,25 +56,25 @@
         logging.info(f" Downloading {directory}")
         # show progress using rich
         response = requests.get(url, stream=True)
         total_size = int(response.headers.get("Content-Length", 0))
         chunk_size = 1024 * 10
 
         with Progress() as progress:
-            task = progress.add_task(f"[cyan] Downloading {model_name}...", total=total_size)
+            task = progress.add_task(f"[white] Downloading {model_name}...", total=total_size)
             for chunk in response.iter_content(chunk_size=chunk_size):
                 open(filename, "ab").write(chunk)
                 progress.update(task, advance=chunk_size)
 
         # Unzip the model
         import zipfile
         with Progress() as progress:
             with zipfile.ZipFile(filename, 'r') as zip_ref:
                 total_size = sum((file.file_size for file in zip_ref.infolist()))
-                task = progress.add_task(f"[cyan] Extracting {model_name}...", total=total_size)
+                task = progress.add_task(f"[white] Extracting {model_name}...", total=total_size)
                 # Get the parent directory of 'directory'
                 parent_directory = os.path.dirname(directory)
                 for file in zip_ref.infolist():
                     zip_ref.extract(file, parent_directory)
                     extracted_size = file.file_size
                     progress.update(task, advance=extracted_size)
```

### Comparing `moosez-2.1.7/moosez/file_utilities.py` & `moosez-2.1.8/moosez/file_utilities.py`

 * *Files identical despite different names*

### Comparing `moosez-2.1.7/moosez/image_conversion.py` & `moosez-2.1.8/moosez/image_conversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,29 +79,29 @@
     """
     # go through the subdirectories
     subjects = os.listdir(parent_dir)
     # get only the directories
     subjects = [subject for subject in subjects if os.path.isdir(os.path.join(parent_dir, subject))]
 
     with Progress() as progress:
-        task = progress.add_task("[cyan] Processing subjects...", total=len(subjects))
+        task = progress.add_task("[white] Processing subjects...", total=len(subjects))
         for subject in subjects:
             subject_path = os.path.join(parent_dir, subject)
             if os.path.isdir(subject_path):
                 images = os.listdir(subject_path)
                 for image in images:
                     if os.path.isdir(os.path.join(subject_path, image)):
                         image_path = os.path.join(subject_path, image)
                         non_nifti_to_nifti(image_path)
                     elif os.path.isfile(os.path.join(subject_path, image)):
                         image_path = os.path.join(subject_path, image)
                         non_nifti_to_nifti(image_path)
             else:
                 continue
-            progress.update(task, advance=1, description=f"[cyan] Processing {subject}...")
+            progress.update(task, advance=1, description=f"[white] Processing {subject}...")
 
 
 def dcm2niix(input_path: str, output_image_basename: str) -> None:
     """
     Converts DICOM images into Nifti images using dcm2niix
     :param input_path: Path to the folder with the dicom files to convert
     """
```

### Comparing `moosez-2.1.7/moosez/image_processing.py` & `moosez-2.1.8/moosez/image_processing.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 #
 # ----------------------------------------------------------------------------------------------------------------------
 
 import os
 import numpy as np
 import nibabel
 import SimpleITK as sitk
-from moosez.constants import MATRIX_THRESHOLD, Z_AXIS_THRESHOLD, CHUNK_THRESHOLD, MARGIN_PADDING, ORGAN_INDICES
+from moosez.constants import MATRIX_THRESHOLD, Z_AXIS_THRESHOLD, CHUNK_THRESHOLD, MARGIN_PADDING, ORGAN_INDICES, \
+    CHUNK_FILENAMES
 import dask.array as da
 from mpire import WorkerPool
 import pandas as pd
 
 
 def get_intensity_statistics(image: sitk.Image, mask_image: sitk.Image, model_name: str, out_csv: str) -> None:
     """
@@ -85,15 +86,15 @@
     if large_image:
         # Calculate indices for image chunks
         num_chunks = 3
         chunk_size = image_shape[2] // num_chunks
         chunk_indices = [(0, chunk_size + MARGIN_PADDING),
                          (chunk_size + 1 - MARGIN_PADDING, chunk_size * 2 + MARGIN_PADDING),
                          (chunk_size * 2 + 1 - MARGIN_PADDING, None)]
-        filenames = ["chunk01_0000.nii.gz", "chunk02_0000.nii.gz", "chunk03_0000.nii.gz"]
+        filenames = CHUNK_FILENAMES
         save_dir = os.path.dirname(out_image_path)
         chunk_paths = [os.path.join(save_dir, filename) for filename in filenames]
 
         chunk_data = []
         for chunk_index, chunk_path in zip(chunk_indices, chunk_paths):
             chunk_data.append({"chunk_index": chunk_index, "image_chunk_path": chunk_path})
```

### Comparing `moosez-2.1.7/moosez/input_validation.py` & `moosez-2.1.8/moosez/input_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,26 +36,26 @@
         raise Exception(f"Error: The directory '{directory_path}' does not exist.")
 
 
 def select_moose_compliant_subjects(subject_paths: list, modality_tags: list) -> list:
     """
     Selects the subjects that have the files that have names that are compliant with the moosez.
     :param subject_paths: The path to the list of subjects that are present in the parent directory.
-    :param modality_tags: The list of appropriate modality suffixes that should be attached to the files for them to be moose
+    :param modality_tags: The list of appropriate modality prefixes that should be attached to the files for them to be moose
     compliant.
     :return: The list of subject paths that are moose compliant.
     """
     # go through each subject in the parent directory
     moose_compliant_subjects = []
     for subject_path in subject_paths:
-        # go through each subject and see if the files have the appropriate modality suffixes
+        # go through each subject and see if the files have the appropriate modality prefixes
 
         files = [file for file in os.listdir(subject_path) if file.endswith('.nii') or file.endswith('.nii.gz')]
-        suffixes = [file.startswith(tag) for tag in modality_tags for file in files]
-        if sum(suffixes) == len(modality_tags):
+        prefixes = [file.startswith(tag) for tag in modality_tags for file in files]
+        if sum(prefixes) == len(modality_tags):
             moose_compliant_subjects.append(subject_path)
     print(f"{constants.ANSI_ORANGE} Number of moose compliant subjects: {len(moose_compliant_subjects)} out of "
           f"{len(subject_paths)} {constants.ANSI_RESET}")
     logging.info(f" Number of moose compliant subjects: {len(moose_compliant_subjects)} out of "
                  f"{len(subject_paths)}")
 
     return moose_compliant_subjects
```

### Comparing `moosez-2.1.7/moosez/moosez.py` & `moosez-2.1.8/moosez/moosez.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,15 +179,15 @@
         # ----------------------------------
         # EXTRACT PET ACTIVITY
         # ----------------------------------
         pet_file = file_utilities.find_pet_file(subject)
         if pet_file is not None:
             pet_image = SimpleITK.ReadImage(pet_file)
             spinner.text = f' Extracting PET activity for {os.path.basename(subject)}...'
-            multilabel_file = glob.glob(os.path.join(output_dir, constants.MULTILABEL_SUFFIX + '*nii*'))[0]
+            multilabel_file = glob.glob(os.path.join(output_dir, constants.MULTILABEL_PREFIX + '*nii*'))[0]
             multilabel_image = SimpleITK.ReadImage(multilabel_file)
             resampled_multilabel_image = ImageResampler.reslice_identity(reference_image=pet_image,
                                                                          moving_image=multilabel_image,
                                                                          is_label_image=True)
             out_csv = os.path.join(stats_dir, os.path.basename(subject) + '_pet_activity.csv')
             image_processing.get_intensity_statistics(pet_image, resampled_multilabel_image, model_name, out_csv)
             spinner.text = f'{constants.ANSI_GREEN} PET activity extracted for {os.path.basename(subject)}! ' \
```

### Comparing `moosez-2.1.7/moosez/predict.py` & `moosez-2.1.8/moosez/predict.py`

 * *Files 6% similar despite different names*

```diff
@@ -137,15 +137,15 @@
     Postprocesses the predicted images.
     :param original_image: The path to the original image.
     :param output_dir: The output directory containing the label image.
     :return: None
     """
     # [1] Resample the predicted image to the original image's voxel spacing
     predicted_image = file_utilities.get_files(output_dir, '.nii.gz')[0]
-    multilabel_image = os.path.join(output_dir, constants.MULTILABEL_SUFFIX + os.path.basename(original_image))
+    multilabel_image = os.path.join(output_dir, constants.MULTILABEL_PREFIX + os.path.basename(original_image))
     original_header = nib.load(original_image).header
     native_spacing = original_header.get_zooms()
     native_size = original_header.get_data_shape()
     resampled_prediction = ImageResampler.resample_segmentations(input_image_path=predicted_image,
                                                                  desired_spacing=native_spacing,
                                                                  desired_size=native_size)
     image_processing.write_image(resampled_prediction, multilabel_image, False)
@@ -258,27 +258,32 @@
     # Create an empty array with the original image's shape
     merged_image_data = np.zeros(original_image_shape, dtype=np.uint8)
 
     # Calculate the split index along the z-axis
     z_split_index = original_image_shape[2] // 3
 
     # Load each part, extract its data, and place it in the correct position in the merged image
-    merged_image_data[:, :, :z_split_index] = nib.load(os.path.join(save_dir, "chunk01.nii.gz")).get_fdata()[:,
+
+    predicted_chunk_filenames = [s.replace("_0000", "") for s in constants.CHUNK_FILENAMES]
+
+    merged_image_data[:, :, :z_split_index] = nib.load(
+        os.path.join(save_dir, predicted_chunk_filenames[0])).get_fdata()[:,
                                               :, :-constants.MARGIN_PADDING]
     merged_image_data[:, :, z_split_index:z_split_index * 2] = nib.load(
-        os.path.join(save_dir, "chunk02.nii.gz")).get_fdata()[:, :,
+        os.path.join(save_dir, predicted_chunk_filenames[1])).get_fdata()[:, :,
                                                                constants.MARGIN_PADDING - 1:-constants.MARGIN_PADDING]
-    merged_image_data[:, :, z_split_index * 2:] = nib.load(os.path.join(save_dir, "chunk03.nii.gz")).get_fdata()[
+    merged_image_data[:, :, z_split_index * 2:] = nib.load(
+        os.path.join(save_dir, predicted_chunk_filenames[2])).get_fdata()[
                                                   :, :, constants.MARGIN_PADDING - 1:]
 
     # Create a new Nifti1Image with the merged data and the original image's affine transformation
     merged_image = nib.Nifti1Image(merged_image_data, original_image_affine)
 
     # remove the split image parts
-    files_to_remove = glob.glob(os.path.join(save_dir, "chunk*"))
+    files_to_remove = glob.glob(os.path.join(save_dir, constants.CHUNK_PREFIX+"*"))
     for file in files_to_remove:
         os.remove(file)
 
     # write the merged image to disk
     merged_image_path = os.path.join(save_dir, constants.RESAMPLED_IMAGE_FILE_NAME)
     nib.save(merged_image, merged_image_path)
```

### Comparing `moosez-2.1.7/moosez/resources.py` & `moosez-2.1.8/moosez/resources.py`

 * *Files identical despite different names*

### Comparing `moosez-2.1.7/moosez.egg-info/PKG-INFO` & `moosez-2.1.8/moosez.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moosez
-Version: 2.1.7
+Version: 2.1.8
 Summary: An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks
 Home-page: https://github.com/QIMP-Team/mooseZ
 Author: Lalith Kumar Shiyam Sundar
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
 License: Apache 2.0
 Keywords: moosez model-zoo nnUNet medical-imaging tumor-segmentation organ-segmentation bone-segmentation lung-segmentation muscle-segmentation fat-segmentation vessel-segmentation vertebral-segmentation rib-segmentation preclinical-segmentation clinical-segmentation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `moosez-2.1.7/setup.py` & `moosez-2.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='moosez',
-    version='2.1.7',
+    version='2.1.8',
     author='Lalith Kumar Shiyam Sundar',
     author_email='Lalith.shiyamsundar@meduniwien.ac.at',
     description='An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks',
     python_requires='>=3.9',
     long_description='mooseZ is an AI-inference engine based on nnUNet, designed for 3D clinical and preclinical'
                      ' whole-body segmentation tasks. It serves models tailored towards different modalities such'
                      ' as PET, CT, and MR. mooseZ provides fast and accurate segmentation results, making it a '
```

