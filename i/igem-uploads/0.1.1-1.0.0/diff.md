# Comparing `tmp/igem-uploads-0.1.1.tar.gz` & `tmp/igem-uploads-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "igem-uploads-0.1.1.tar", last modified: Sat Jul  1 18:46:23 2023, max compression
+gzip compressed data, was "igem-uploads-1.0.0.tar", last modified: Sun Jul  2 08:54:24 2023, max compression
```

## Comparing `igem-uploads-0.1.1.tar` & `igem-uploads-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 liang      (501) staff       (20)        0 2023-07-01 18:46:23.315511 igem-uploads-0.1.1/
--rw-r--r--   0 liang      (501) staff       (20)    18715 2023-07-01 18:14:41.000000 igem-uploads-0.1.1/LICENSE
--rw-r--r--   0 liang      (501) staff       (20)     1248 2023-07-01 18:46:23.315381 igem-uploads-0.1.1/PKG-INFO
--rw-r--r--   0 liang      (501) staff       (20)      856 2023-07-01 18:37:34.000000 igem-uploads-0.1.1/README.md
-drwxr-xr-x   0 liang      (501) staff       (20)        0 2023-07-01 18:46:23.314970 igem-uploads-0.1.1/igem_uploads.egg-info/
--rw-r--r--   0 liang      (501) staff       (20)     1248 2023-07-01 18:46:23.000000 igem-uploads-0.1.1/igem_uploads.egg-info/PKG-INFO
--rw-r--r--   0 liang      (501) staff       (20)      244 2023-07-01 18:46:23.000000 igem-uploads-0.1.1/igem_uploads.egg-info/SOURCES.txt
--rw-r--r--   0 liang      (501) staff       (20)        1 2023-07-01 18:46:23.000000 igem-uploads-0.1.1/igem_uploads.egg-info/dependency_links.txt
--rw-r--r--   0 liang      (501) staff       (20)        6 2023-07-01 18:46:23.000000 igem-uploads-0.1.1/igem_uploads.egg-info/requires.txt
--rw-r--r--   0 liang      (501) staff       (20)        8 2023-07-01 18:46:23.000000 igem-uploads-0.1.1/igem_uploads.egg-info/top_level.txt
--rw-r--r--   0 liang      (501) staff       (20)       38 2023-07-01 18:46:23.315551 igem-uploads-0.1.1/setup.cfg
--rw-r--r--   0 liang      (501) staff       (20)      666 2023-07-01 18:46:13.000000 igem-uploads-0.1.1/setup.py
-drwxr-xr-x   0 liang      (501) staff       (20)        0 2023-07-01 18:46:23.315212 igem-uploads-0.1.1/uploads/
--rw-r--r--   0 liang      (501) staff       (20)       29 2023-06-30 17:37:36.000000 igem-uploads-0.1.1/uploads/__init__.py
--rw-r--r--   0 liang      (501) staff       (20)     7357 2023-07-01 18:33:27.000000 igem-uploads-0.1.1/uploads/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:54:24.550101 igem-uploads-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    18715 2023-07-02 08:54:13.000000 igem-uploads-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-02 08:54:24.550101 igem-uploads-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-02 08:54:13.000000 igem-uploads-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:54:24.550101 igem-uploads-1.0.0/igem_uploads.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-02 08:54:24.000000 igem-uploads-1.0.0/igem_uploads.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-02 08:54:24.000000 igem-uploads-1.0.0/igem_uploads.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 08:54:24.000000 igem-uploads-1.0.0/igem_uploads.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-02 08:54:24.000000 igem-uploads-1.0.0/igem_uploads.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-02 08:54:24.000000 igem-uploads-1.0.0/igem_uploads.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 08:54:24.550101 igem-uploads-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-02 08:54:13.000000 igem-uploads-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:54:24.550101 igem-uploads-1.0.0/uploads/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-02 08:54:13.000000 igem-uploads-1.0.0/uploads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7345 2023-07-02 08:54:13.000000 igem-uploads-1.0.0/uploads/session.py
```

### Comparing `igem-uploads-0.1.1/LICENSE` & `igem-uploads-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `igem-uploads-0.1.1/PKG-INFO` & `igem-uploads-1.0.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: igem-uploads
-Version: 0.1.1
+Version: 1.0.0
 Summary: Helps iGEMers upload their files to the iGEM server.
 Home-page: https://github.com/iGEM-HBUT-China/igem-uploads
 Author: iGEM-HBUT-China
 Author-email: liangtianyi2002@outlook.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved
 Description-Content-Type: text/markdown
@@ -21,31 +21,36 @@
 ```
 
 ## Usage
 
 ```python
 import uploads
 
-# create a session instance, login to igem.org
+# create a session instance
 client = uploads.Session()
+# login to igem.org
 client.login('username', 'password')
 
 # upload a file to specific directory
+client.upload('path/to/file')
 client.upload('path/to/file', 'target_directory')
 
 # query files/dirs in specific directory
-client.query('target_directory')
+client.query('')
+client.query('directory')
 
 # upload a directory and its subdirectories to specific directory
+client.upload_dir('path/to/directory')
 client.upload_dir('path/to/directory', 'target_directory')
 
 # delete file in specific directory
 client.delete('filename', 'file_parent_directory')
 
 # truncate a directory
-client.truncate_dir('directory')
+client.truncate_dir('target_directory')
 ```
 
 ## Links
 
 - [PyPI](https://pypi.org/project/igem-uploads/)
+- [GitHub](https://github.com/iGEM-HBUT-China/igem-uploads)
 - [GitLab](https://gitlab.igem.org/2023/software-tools/hbut-china)
```

### Comparing `igem-uploads-0.1.1/README.md` & `igem-uploads-1.0.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -9,31 +9,36 @@
 ```
 
 ## Usage
 
 ```python
 import uploads
 
-# create a session instance, login to igem.org
+# create a session instance
 client = uploads.Session()
+# login to igem.org
 client.login('username', 'password')
 
 # upload a file to specific directory
+client.upload('path/to/file')
 client.upload('path/to/file', 'target_directory')
 
 # query files/dirs in specific directory
-client.query('target_directory')
+client.query('')
+client.query('directory')
 
 # upload a directory and its subdirectories to specific directory
+client.upload_dir('path/to/directory')
 client.upload_dir('path/to/directory', 'target_directory')
 
 # delete file in specific directory
 client.delete('filename', 'file_parent_directory')
 
 # truncate a directory
-client.truncate_dir('directory')
+client.truncate_dir('target_directory')
 ```
 
 ## Links
 
 - [PyPI](https://pypi.org/project/igem-uploads/)
+- [GitHub](https://github.com/iGEM-HBUT-China/igem-uploads)
 - [GitLab](https://gitlab.igem.org/2023/software-tools/hbut-china)
```

### Comparing `igem-uploads-0.1.1/igem_uploads.egg-info/PKG-INFO` & `igem-uploads-1.0.0/igem_uploads.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: igem-uploads
-Version: 0.1.1
+Version: 1.0.0
 Summary: Helps iGEMers upload their files to the iGEM server.
 Home-page: https://github.com/iGEM-HBUT-China/igem-uploads
 Author: iGEM-HBUT-China
 Author-email: liangtianyi2002@outlook.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved
 Description-Content-Type: text/markdown
@@ -21,31 +21,36 @@
 ```
 
 ## Usage
 
 ```python
 import uploads
 
-# create a session instance, login to igem.org
+# create a session instance
 client = uploads.Session()
+# login to igem.org
 client.login('username', 'password')
 
 # upload a file to specific directory
+client.upload('path/to/file')
 client.upload('path/to/file', 'target_directory')
 
 # query files/dirs in specific directory
-client.query('target_directory')
+client.query('')
+client.query('directory')
 
 # upload a directory and its subdirectories to specific directory
+client.upload_dir('path/to/directory')
 client.upload_dir('path/to/directory', 'target_directory')
 
 # delete file in specific directory
 client.delete('filename', 'file_parent_directory')
 
 # truncate a directory
-client.truncate_dir('directory')
+client.truncate_dir('target_directory')
 ```
 
 ## Links
 
 - [PyPI](https://pypi.org/project/igem-uploads/)
+- [GitHub](https://github.com/iGEM-HBUT-China/igem-uploads)
 - [GitLab](https://gitlab.igem.org/2023/software-tools/hbut-china)
```

### Comparing `igem-uploads-0.1.1/setup.py` & `igem-uploads-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 requirements = ["wheel"]
 
 setup(
     name="igem-uploads",
-    version="0.1.1",
+    version="1.0.0",
     author="iGEM-HBUT-China",
     author_email="liangtianyi2002@outlook.com",
     description="Helps iGEMers upload their files to the iGEM server.",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/iGEM-HBUT-China/igem-uploads",
     packages=find_packages(),
```

### Comparing `igem-uploads-0.1.1/uploads/session.py` & `igem-uploads-1.0.0/uploads/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
             err_info = str(tree.xpath('/html/body/form/div[1]')[0].text).split('.')[0] + '.'
             warnings.warn(err_info)
             exit(1)
 
     def query(self, directory=''):
         """
         query a files/dirs in specific directory
-        :param directory: (optional) directory to query, default to root directory(/)
+        :param directory: (optional) directory to query, default to root directory
         :return: list of files, each file/dir as a dict
         """
         response = self.request('GET', f'https://shim-s3.igem.org/v1/teams/{self.team_id}/wiki?directory={directory}')
         res = response.json()
         if res['KeyCount'] > 0:
             print(directory if directory != '' else '/', 'found:', res['KeyCount'])
             contents = []
@@ -98,15 +98,15 @@
             warnings.warn('Query failed')
             exit(1)
 
     def upload(self, abs_file_path, directory='', list_files=True):
         """
         upload file to specific directory
         :param abs_file_path: absolute path of file
-        :param directory: (optional) target directory, default to root directory(/)
+        :param directory: (optional) target directory, default to root directory
         :param list_files: (optional) need to list files after upload, default to True
         :type list_files: bool
         :return: file url
         """
         path_to_file = Path(abs_file_path)
         if not path_to_file.is_file():
             warnings.warn('Invalid file path: ' + abs_file_path)
@@ -129,15 +129,15 @@
         else:
             warnings.warn('Upload failed' + res.text)
 
     def upload_dir(self, abs_path, directory=''):
         """
         upload a directory and its subdirectories to specific directory
         :param abs_path: absolute path of directory
-        :param directory: (optional) target directory, default to root directory(/)
+        :param directory: (optional) target directory, default to root directory
         :return: list of files, each file/dir as a dict
         """
         path_to_dir = Path(abs_path)
         if not path_to_dir.is_dir():
             warnings.warn('Invalid directory path: ' + abs_path)
             exit(1)
         file_list = os.listdir(abs_path)
@@ -154,15 +154,15 @@
                 self.upload_dir(path_to_dir / filename, dir_path)
         return self.query(dir_path)
 
     def delete(self, filename, directory='', list_files=True):
         """
         delete file in specific directory
         :param filename: filename
-        :param directory: file parent directory, default to root directory(/)
+        :param directory: file parent directory, default to root directory
         :param list_files: need to list files after delete, default to True
         """
         res = self.request('DELETE',
                            f'https://shim-s3.igem.org/v1/teams/{self.team_id}/wiki/{filename}?directory={directory}')
         if res.status_code == 200:
             print(directory + '/' + filename, 'deleted')
             print()
```

