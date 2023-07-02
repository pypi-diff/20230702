# Comparing `tmp/pyvhs-0.1.2.tar.gz` & `tmp/pyvhs-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvhs-0.1.2.tar", max compression
+gzip compressed data, was "pyvhs-0.1.3.tar", max compression
```

## Comparing `pyvhs-0.1.2.tar` & `pyvhs-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1068 2023-06-19 13:27:10.974931 pyvhs-0.1.2/LICENSE
--rw-r--r--   0        0        0     9080 2023-06-24 13:34:33.656701 pyvhs-0.1.2/README.md
--rw-r--r--   0        0        0   176080 2023-06-19 12:45:19.455984 pyvhs-0.1.2/doc/imgs/playback.png
--rw-r--r--   0        0        0   242536 2023-06-19 12:48:00.793752 pyvhs-0.1.2/doc/imgs/pyvhs.png
--rw-r--r--   0        0        0      570 2023-07-01 16:40:20.739303 pyvhs-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-19 19:27:59.639929 pyvhs-0.1.2/pyvhs/__init__.py
--rw-r--r--   0        0        0    59151 2023-06-17 12:32:19.507485 pyvhs-0.1.2/pyvhs/template_imgs/template001.png
--rw-r--r--   0        0        0     2321 2023-06-17 12:48:13.782701 pyvhs-0.1.2/pyvhs/template_imgs/template002.png
--rw-r--r--   0        0        0        0 2023-06-18 18:24:43.368411 pyvhs-0.1.2/pyvhs/utils/__init__.py
--rw-r--r--   0        0        0    11843 2023-07-01 16:39:33.865046 pyvhs-0.1.2/pyvhs/utils/edits.py
--rw-r--r--   0        0        0     1217 2023-07-01 16:36:30.187897 pyvhs-0.1.2/pyvhs/utils/files.py
--rw-r--r--   0        0        0     4565 2023-07-01 16:36:30.187897 pyvhs-0.1.2/pyvhs/vhs.py
--rw-r--r--   0        0        0     9926 1970-01-01 00:00:00.000000 pyvhs-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-19 13:27:10.974931 pyvhs-0.1.3/LICENSE
+-rw-r--r--   0        0        0    10489 2023-07-02 19:01:00.760100 pyvhs-0.1.3/README.md
+-rw-r--r--   0        0        0   176080 2023-06-19 12:45:19.455984 pyvhs-0.1.3/doc/imgs/playback.png
+-rw-r--r--   0        0        0   242536 2023-06-19 12:48:00.793752 pyvhs-0.1.3/doc/imgs/pyvhs.png
+-rw-r--r--   0        0        0      570 2023-07-02 19:01:44.098427 pyvhs-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-19 19:27:59.639929 pyvhs-0.1.3/pyvhs/__init__.py
+-rw-r--r--   0        0        0    59151 2023-06-17 12:32:19.507485 pyvhs-0.1.3/pyvhs/template_imgs/template001.png
+-rw-r--r--   0        0        0     2321 2023-06-17 12:48:13.782701 pyvhs-0.1.3/pyvhs/template_imgs/template002.png
+-rw-r--r--   0        0        0        0 2023-06-18 18:24:43.368411 pyvhs-0.1.3/pyvhs/utils/__init__.py
+-rw-r--r--   0        0        0    11843 2023-07-01 16:47:43.874844 pyvhs-0.1.3/pyvhs/utils/edits.py
+-rw-r--r--   0        0        0     1217 2023-07-01 16:36:30.187897 pyvhs-0.1.3/pyvhs/utils/files.py
+-rw-r--r--   0        0        0     4565 2023-07-01 16:36:30.187897 pyvhs-0.1.3/pyvhs/vhs.py
+-rw-r--r--   0        0        0    11335 1970-01-01 00:00:00.000000 pyvhs-0.1.3/PKG-INFO
```

### Comparing `pyvhs-0.1.2/LICENSE` & `pyvhs-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvhs-0.1.2/README.md` & `pyvhs-0.1.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -47,14 +47,40 @@
 
 **NOTE**: The original digitized video files are not altered with <b>PyVHS</b>.
 
 A primary benefit of this package is that there is no need to manually remove blank segments from the digitized videos. This saves lots of time especially if there are multiple video files.
 
 
 # Installation
+The following steps are required to use <b>PyVHS</b>:
+
+1) [Install Python](https://www.python.org/downloads/): Python can be installed on Windows, macOS, and Linux operating systems. Go to the official [Python download page](https://www.python.org/downloads/) and install Python 3.9 or higher.
+    * If you are a Windows user and need help installing Python then there are many helpful online articles for this topic. For example, here is helpful [step-by-step set of instructions from Digital Ocean](https://www.digitalocean.com/community/tutorials/install-python-windows-10).
+2) Once Python is installed open a command line shell (e.g. in Windows type `cmd` in the lower-left search field).
+3) A virtual environment is recommended for installing <b>PyVHS</b>. This is easily setup from the command line by typing:
+
+<b>Windows Users</b>: using the cmd shell
+```cmd
+pip install virtualenv
+virtualenv myenv
+myenv\Scripts\activate
+pip install pyvhs
+pyvhs -dir="PATH_TO_DIRECTORY_CONTAINING_VIDEO"
+```
+
+<b>macOS and Linux Users</b>: using the bash shell
+```bash
+pip install virtualenv
+virtualenv myenv
+source ./myenv/venv/bin/activate
+pip install pyvhs
+pyvhs -dir="PATH_TO_DIRECTORY_CONTAINING_VIDEO"
+```
+More information on setting-up and deactivating virtual environments can be found in this [online Geeks for Geeks article](https://www.geeksforgeeks.org/creating-python-virtual-environment-windows-linux/).
+
 ## pip
 Available on [PyPI](https://pypi.org/project/pyvhs/)
 ```bash
 pip install pyvhs
 ```
 ## Git Clone
 Download the GitHub repository, create a [Python Virtual Environment](https://docs.python.org/3/library/venv.html), and pip install PyVHS
```

#### html2text {}

```diff
@@ -28,34 +28,52 @@
 #2) from video files, - automatically remove blank segments from a single or
 multiple video files, - save new video file(s) which will have a smaller file
 size, - save new video files(s) with only footage and no more boring blank
 screens, - execute using either the command-line interface (CLI), Python
 scripts, or Jupyter Notebooks. **NOTE**: The original digitized video files are
 not altered with PyVHS. A primary benefit of this package is that there is no
 need to manually remove blank segments from the digitized videos. This saves
-lots of time especially if there are multiple video files. # Installation ##
-pip Available on [PyPI](https://pypi.org/project/pyvhs/) ```bash pip install
-pyvhs ``` ## Git Clone Download the GitHub repository, create a [Python Virtual
-Environment](https://docs.python.org/3/library/venv.html), and pip install
-PyVHS ``` git clone https://github.com/mddunlap924/PyVHS.git cd PyVHS python3 -
-m venv .venv pip install . ``` For other dependency management tool, please
-visit # Usage ## Use PyVHS as a command line tool from the terminal ### Convert
-a single video ```bash pyvhs -dir='./video_to_edit/video000.mp4' ``` ``` File
-Structure for Editing a Single Video Note: Set Folder and File Names to Your
-Choice Input: video000.mp4 Output: video000_edited.mp4 (with blank segments
-removed) âââ ./video_to_edit â âââ video0.mp4 â âââ
-video0_edited.mp4 ``` ### Convert multiple videos ```bash pyvhs -dir='./
-videos_to_edit' ``` ``` File Structure for Editing Multiple Videos Note: Set
-Folder and Files Names to Your Choice Inputs: video000.mp4; video001.mpy;
-video002.mpy; ... Outputs: video000_edited.mp4; video001_edited.mpy;
-video002_edited.mpy; ... âââ ./videos_to_edit â âââ video0.mp4
-â âââ video0_edited.mp4 â âââ video1.mp4 â âââ
-video1_edited.mp4 â âââ video2.mp4 â âââ video2_edited.mp4 â
-âââ ... ``` ## Use PyVHS as a library Refer to the [Jupyter Notebook]
-(https://github.com/mddunlap924/PyVHS/blob/main/notebooks/
+lots of time especially if there are multiple video files. # Installation The
+following steps are required to use PyVHS: 1) [Install Python](https://
+www.python.org/downloads/): Python can be installed on Windows, macOS, and
+Linux operating systems. Go to the official [Python download page](https://
+www.python.org/downloads/) and install Python 3.9 or higher. * If you are a
+Windows user and need help installing Python then there are many helpful online
+articles for this topic. For example, here is helpful [step-by-step set of
+instructions from Digital Ocean](https://www.digitalocean.com/community/
+tutorials/install-python-windows-10). 2) Once Python is installed open a
+command line shell (e.g. in Windows type `cmd` in the lower-left search field).
+3) A virtual environment is recommended for installing PyVHS. This is easily
+setup from the command line by typing: Windows Users: using the cmd shell
+```cmd pip install virtualenv virtualenv myenv myenv\Scripts\activate pip
+install pyvhs pyvhs -dir="PATH_TO_DIRECTORY_CONTAINING_VIDEO" ``` macOS and
+Linux Users: using the bash shell ```bash pip install virtualenv virtualenv
+myenv source ./myenv/venv/bin/activate pip install pyvhs pyvhs -
+dir="PATH_TO_DIRECTORY_CONTAINING_VIDEO" ``` More information on setting-up and
+deactivating virtual environments can be found in this [online Geeks for Geeks
+article](https://www.geeksforgeeks.org/creating-python-virtual-environment-
+windows-linux/). ## pip Available on [PyPI](https://pypi.org/project/pyvhs/
+) ```bash pip install pyvhs ``` ## Git Clone Download the GitHub repository,
+create a [Python Virtual Environment](https://docs.python.org/3/library/
+venv.html), and pip install PyVHS ``` git clone https://github.com/mddunlap924/
+PyVHS.git cd PyVHS python3 -m venv .venv pip install . ``` For other dependency
+management tool, please visit # Usage ## Use PyVHS as a command line tool from
+the terminal ### Convert a single video ```bash pyvhs -dir='./video_to_edit/
+video000.mp4' ``` ``` File Structure for Editing a Single Video Note: Set
+Folder and File Names to Your Choice Input: video000.mp4 Output:
+video000_edited.mp4 (with blank segments removed) âââ ./video_to_edit â
+âââ video0.mp4 â âââ video0_edited.mp4 ``` ### Convert multiple
+videos ```bash pyvhs -dir='./videos_to_edit' ``` ``` File Structure for Editing
+Multiple Videos Note: Set Folder and Files Names to Your Choice Inputs:
+video000.mp4; video001.mpy; video002.mpy; ... Outputs: video000_edited.mp4;
+video001_edited.mpy; video002_edited.mpy; ... âââ ./videos_to_edit â
+âââ video0.mp4 â âââ video0_edited.mp4 â âââ video1.mp4
+â âââ video1_edited.mp4 â âââ video2.mp4 â âââ
+video2_edited.mp4 â âââ ... ``` ## Use PyVHS as a library Refer to the
+[Jupyter Notebook](https://github.com/mddunlap924/PyVHS/blob/main/notebooks/
 edit_single_video.ipynb) example showing how to edit a single video. ```python
 from pyvhs.utils.files import VideosToEdit from pyvhs.utils.edits import
 EditVideo # List video files videos = VideosToEdit(path=PATH_VIDEO)
 videos.list_videos() # Create a video editing object video_edit = EditVideo
 (path_original=videos.original[0], path_edited=videos.edited[0],
 templates=template_imgs, interval=3, ) print(f'Video Duration:
 {video_edit.duration:,.2f} seconds') print(f'Check Video Frames Every:
```

### Comparing `pyvhs-0.1.2/doc/imgs/playback.png` & `pyvhs-0.1.3/doc/imgs/playback.png`

 * *Files identical despite different names*

### Comparing `pyvhs-0.1.2/doc/imgs/pyvhs.png` & `pyvhs-0.1.3/doc/imgs/pyvhs.png`

 * *Files identical despite different names*

### Comparing `pyvhs-0.1.2/pyproject.toml` & `pyvhs-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyvhs"
-version = "0.1.2"
+version = "0.1.3"
 description = "Digitized VHS Cassette Editing with Python"
 authors = ["Myles Dunlap"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/mddunlap924/PyVHS/tree/main"
 keywords = ["vhs", "vcr", "image processing", "video"]
```

### Comparing `pyvhs-0.1.2/pyvhs/template_imgs/template001.png` & `pyvhs-0.1.3/pyvhs/template_imgs/template001.png`

 * *Files identical despite different names*

### Comparing `pyvhs-0.1.2/pyvhs/template_imgs/template002.png` & `pyvhs-0.1.3/pyvhs/template_imgs/template002.png`

 * *Files identical despite different names*

### Comparing `pyvhs-0.1.2/pyvhs/utils/edits.py` & `pyvhs-0.1.3/pyvhs/utils/edits.py`

 * *Files identical despite different names*

### Comparing `pyvhs-0.1.2/pyvhs/utils/files.py` & `pyvhs-0.1.3/pyvhs/utils/files.py`

 * *Files identical despite different names*

### Comparing `pyvhs-0.1.2/pyvhs/vhs.py` & `pyvhs-0.1.3/pyvhs/vhs.py`

 * *Files identical despite different names*

### Comparing `pyvhs-0.1.2/PKG-INFO` & `pyvhs-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvhs
-Version: 0.1.2
+Version: 0.1.3
 Summary: Digitized VHS Cassette Editing with Python
 Home-page: https://github.com/mddunlap924/PyVHS/tree/main
 License: MIT
 Keywords: vhs,vcr,image processing,video
 Author: Myles Dunlap
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -69,14 +69,40 @@
 
 **NOTE**: The original digitized video files are not altered with <b>PyVHS</b>.
 
 A primary benefit of this package is that there is no need to manually remove blank segments from the digitized videos. This saves lots of time especially if there are multiple video files.
 
 
 # Installation
+The following steps are required to use <b>PyVHS</b>:
+
+1) [Install Python](https://www.python.org/downloads/): Python can be installed on Windows, macOS, and Linux operating systems. Go to the official [Python download page](https://www.python.org/downloads/) and install Python 3.9 or higher.
+    * If you are a Windows user and need help installing Python then there are many helpful online articles for this topic. For example, here is helpful [step-by-step set of instructions from Digital Ocean](https://www.digitalocean.com/community/tutorials/install-python-windows-10).
+2) Once Python is installed open a command line shell (e.g. in Windows type `cmd` in the lower-left search field).
+3) A virtual environment is recommended for installing <b>PyVHS</b>. This is easily setup from the command line by typing:
+
+<b>Windows Users</b>: using the cmd shell
+```cmd
+pip install virtualenv
+virtualenv myenv
+myenv\Scripts\activate
+pip install pyvhs
+pyvhs -dir="PATH_TO_DIRECTORY_CONTAINING_VIDEO"
+```
+
+<b>macOS and Linux Users</b>: using the bash shell
+```bash
+pip install virtualenv
+virtualenv myenv
+source ./myenv/venv/bin/activate
+pip install pyvhs
+pyvhs -dir="PATH_TO_DIRECTORY_CONTAINING_VIDEO"
+```
+More information on setting-up and deactivating virtual environments can be found in this [online Geeks for Geeks article](https://www.geeksforgeeks.org/creating-python-virtual-environment-windows-linux/).
+
 ## pip
 Available on [PyPI](https://pypi.org/project/pyvhs/)
 ```bash
 pip install pyvhs
 ```
 ## Git Clone
 Download the GitHub repository, create a [Python Virtual Environment](https://docs.python.org/3/library/venv.html), and pip install PyVHS
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyvhs Version: 0.1.2 Summary: Digitized VHS
+Metadata-Version: 2.1 Name: pyvhs Version: 0.1.3 Summary: Digitized VHS
 Cassette Editing with Python Home-page: https://github.com/mddunlap924/PyVHS/
 tree/main License: MIT Keywords: vhs,vcr,image processing,video Author: Myles
 Dunlap Requires-Python: >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: matplotlib (>=3.7.1,<4.0.0) Requires-
@@ -39,34 +39,52 @@
 #2) from video files, - automatically remove blank segments from a single or
 multiple video files, - save new video file(s) which will have a smaller file
 size, - save new video files(s) with only footage and no more boring blank
 screens, - execute using either the command-line interface (CLI), Python
 scripts, or Jupyter Notebooks. **NOTE**: The original digitized video files are
 not altered with PyVHS. A primary benefit of this package is that there is no
 need to manually remove blank segments from the digitized videos. This saves
-lots of time especially if there are multiple video files. # Installation ##
-pip Available on [PyPI](https://pypi.org/project/pyvhs/) ```bash pip install
-pyvhs ``` ## Git Clone Download the GitHub repository, create a [Python Virtual
-Environment](https://docs.python.org/3/library/venv.html), and pip install
-PyVHS ``` git clone https://github.com/mddunlap924/PyVHS.git cd PyVHS python3 -
-m venv .venv pip install . ``` For other dependency management tool, please
-visit # Usage ## Use PyVHS as a command line tool from the terminal ### Convert
-a single video ```bash pyvhs -dir='./video_to_edit/video000.mp4' ``` ``` File
-Structure for Editing a Single Video Note: Set Folder and File Names to Your
-Choice Input: video000.mp4 Output: video000_edited.mp4 (with blank segments
-removed) âââ ./video_to_edit â âââ video0.mp4 â âââ
-video0_edited.mp4 ``` ### Convert multiple videos ```bash pyvhs -dir='./
-videos_to_edit' ``` ``` File Structure for Editing Multiple Videos Note: Set
-Folder and Files Names to Your Choice Inputs: video000.mp4; video001.mpy;
-video002.mpy; ... Outputs: video000_edited.mp4; video001_edited.mpy;
-video002_edited.mpy; ... âââ ./videos_to_edit â âââ video0.mp4
-â âââ video0_edited.mp4 â âââ video1.mp4 â âââ
-video1_edited.mp4 â âââ video2.mp4 â âââ video2_edited.mp4 â
-âââ ... ``` ## Use PyVHS as a library Refer to the [Jupyter Notebook]
-(https://github.com/mddunlap924/PyVHS/blob/main/notebooks/
+lots of time especially if there are multiple video files. # Installation The
+following steps are required to use PyVHS: 1) [Install Python](https://
+www.python.org/downloads/): Python can be installed on Windows, macOS, and
+Linux operating systems. Go to the official [Python download page](https://
+www.python.org/downloads/) and install Python 3.9 or higher. * If you are a
+Windows user and need help installing Python then there are many helpful online
+articles for this topic. For example, here is helpful [step-by-step set of
+instructions from Digital Ocean](https://www.digitalocean.com/community/
+tutorials/install-python-windows-10). 2) Once Python is installed open a
+command line shell (e.g. in Windows type `cmd` in the lower-left search field).
+3) A virtual environment is recommended for installing PyVHS. This is easily
+setup from the command line by typing: Windows Users: using the cmd shell
+```cmd pip install virtualenv virtualenv myenv myenv\Scripts\activate pip
+install pyvhs pyvhs -dir="PATH_TO_DIRECTORY_CONTAINING_VIDEO" ``` macOS and
+Linux Users: using the bash shell ```bash pip install virtualenv virtualenv
+myenv source ./myenv/venv/bin/activate pip install pyvhs pyvhs -
+dir="PATH_TO_DIRECTORY_CONTAINING_VIDEO" ``` More information on setting-up and
+deactivating virtual environments can be found in this [online Geeks for Geeks
+article](https://www.geeksforgeeks.org/creating-python-virtual-environment-
+windows-linux/). ## pip Available on [PyPI](https://pypi.org/project/pyvhs/
+) ```bash pip install pyvhs ``` ## Git Clone Download the GitHub repository,
+create a [Python Virtual Environment](https://docs.python.org/3/library/
+venv.html), and pip install PyVHS ``` git clone https://github.com/mddunlap924/
+PyVHS.git cd PyVHS python3 -m venv .venv pip install . ``` For other dependency
+management tool, please visit # Usage ## Use PyVHS as a command line tool from
+the terminal ### Convert a single video ```bash pyvhs -dir='./video_to_edit/
+video000.mp4' ``` ``` File Structure for Editing a Single Video Note: Set
+Folder and File Names to Your Choice Input: video000.mp4 Output:
+video000_edited.mp4 (with blank segments removed) âââ ./video_to_edit â
+âââ video0.mp4 â âââ video0_edited.mp4 ``` ### Convert multiple
+videos ```bash pyvhs -dir='./videos_to_edit' ``` ``` File Structure for Editing
+Multiple Videos Note: Set Folder and Files Names to Your Choice Inputs:
+video000.mp4; video001.mpy; video002.mpy; ... Outputs: video000_edited.mp4;
+video001_edited.mpy; video002_edited.mpy; ... âââ ./videos_to_edit â
+âââ video0.mp4 â âââ video0_edited.mp4 â âââ video1.mp4
+â âââ video1_edited.mp4 â âââ video2.mp4 â âââ
+video2_edited.mp4 â âââ ... ``` ## Use PyVHS as a library Refer to the
+[Jupyter Notebook](https://github.com/mddunlap924/PyVHS/blob/main/notebooks/
 edit_single_video.ipynb) example showing how to edit a single video. ```python
 from pyvhs.utils.files import VideosToEdit from pyvhs.utils.edits import
 EditVideo # List video files videos = VideosToEdit(path=PATH_VIDEO)
 videos.list_videos() # Create a video editing object video_edit = EditVideo
 (path_original=videos.original[0], path_edited=videos.edited[0],
 templates=template_imgs, interval=3, ) print(f'Video Duration:
 {video_edit.duration:,.2f} seconds') print(f'Check Video Frames Every:
```

