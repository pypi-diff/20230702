# Comparing `tmp/igem-uploads-1.0.0.tar.gz` & `tmp/igem-uploads-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "igem-uploads-1.0.0.tar", last modified: Sun Jul  2 08:54:24 2023, max compression
+gzip compressed data, was "igem-uploads-1.1.0.tar", last modified: Sun Jul  2 09:27:00 2023, max compression
```

## Comparing `igem-uploads-1.0.0.tar` & `igem-uploads-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:54:24.550101 igem-uploads-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    18715 2023-07-02 08:54:13.000000 igem-uploads-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-02 08:54:24.550101 igem-uploads-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-02 08:54:13.000000 igem-uploads-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:54:24.550101 igem-uploads-1.0.0/igem_uploads.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-02 08:54:24.000000 igem-uploads-1.0.0/igem_uploads.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-02 08:54:24.000000 igem-uploads-1.0.0/igem_uploads.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 08:54:24.000000 igem-uploads-1.0.0/igem_uploads.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-02 08:54:24.000000 igem-uploads-1.0.0/igem_uploads.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-02 08:54:24.000000 igem-uploads-1.0.0/igem_uploads.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 08:54:24.550101 igem-uploads-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-02 08:54:13.000000 igem-uploads-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:54:24.550101 igem-uploads-1.0.0/uploads/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-02 08:54:13.000000 igem-uploads-1.0.0/uploads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7345 2023-07-02 08:54:13.000000 igem-uploads-1.0.0/uploads/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:27:00.293294 igem-uploads-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    18715 2023-07-02 09:26:49.000000 igem-uploads-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-02 09:27:00.293294 igem-uploads-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-02 09:26:49.000000 igem-uploads-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:27:00.289294 igem-uploads-1.1.0/igem_uploads.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-02 09:27:00.000000 igem-uploads-1.1.0/igem_uploads.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-02 09:27:00.000000 igem-uploads-1.1.0/igem_uploads.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 09:27:00.000000 igem-uploads-1.1.0/igem_uploads.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-02 09:27:00.000000 igem-uploads-1.1.0/igem_uploads.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-02 09:27:00.000000 igem-uploads-1.1.0/igem_uploads.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 09:27:00.293294 igem-uploads-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-02 09:26:49.000000 igem-uploads-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:27:00.293294 igem-uploads-1.1.0/uploads/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-02 09:26:49.000000 igem-uploads-1.1.0/uploads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-07-02 09:26:49.000000 igem-uploads-1.1.0/uploads/session.py
```

### Comparing `igem-uploads-1.0.0/LICENSE` & `igem-uploads-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `igem-uploads-1.0.0/PKG-INFO` & `igem-uploads-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: igem-uploads
-Version: 1.0.0
+Version: 1.1.0
 Summary: Helps iGEMers upload their files to the iGEM server.
 Home-page: https://github.com/iGEM-HBUT-China/igem-uploads
 Author: iGEM-HBUT-China
 Author-email: liangtianyi2002@outlook.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved
 Description-Content-Type: text/markdown
```

### Comparing `igem-uploads-1.0.0/README.md` & `igem-uploads-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `igem-uploads-1.0.0/igem_uploads.egg-info/PKG-INFO` & `igem-uploads-1.1.0/igem_uploads.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: igem-uploads
-Version: 1.0.0
+Version: 1.1.0
 Summary: Helps iGEMers upload their files to the iGEM server.
 Home-page: https://github.com/iGEM-HBUT-China/igem-uploads
 Author: iGEM-HBUT-China
 Author-email: liangtianyi2002@outlook.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved
 Description-Content-Type: text/markdown
```

### Comparing `igem-uploads-1.0.0/setup.py` & `igem-uploads-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 requirements = ["wheel"]
 
 setup(
     name="igem-uploads",
-    version="1.0.0",
+    version="1.1.0",
     author="iGEM-HBUT-China",
     author_email="liangtianyi2002@outlook.com",
     description="Helps iGEMers upload their files to the iGEM server.",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/iGEM-HBUT-China/igem-uploads",
     packages=find_packages(),
```

### Comparing `igem-uploads-1.0.0/uploads/session.py` & `igem-uploads-1.1.0/uploads/session.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,20 +8,29 @@
 from lxml import etree
 
 NOT_LOGGED_IN = 0
 LOGGED_IN = 1
 LOGGED_FAILED = -1
 
 
+def check_parameter(directory: str):
+    if directory.count('/') == len(directory):
+        warnings.warn('You specified \'/\' as a directory name, which may cause unknown errors')
+        exit(1)
+    if directory.startswith('/'):
+        warnings.warn('You specified a directory name starting with \'/\', which may cause unknown errors')
+        exit(1)
+
+
 class Session:
     requests_session_instance = requests.session()
     status = NOT_LOGGED_IN
     team_id = ''
 
-    def request(self, method, url, data=None, files=None):
+    def request(self, method: str, url: str, data=None, files=None):
         if self.status != LOGGED_IN:
             warnings.warn('Not logged in, please login first')
             exit(1)
         return self.requests_session_instance.request(method=method, url=url, data=data, files=files)
 
     def request_team_id(self):
         response = self.requests_session_instance.request('GET', 'https://old.igem.org/aj/session_info?use_my_cookie=1')
@@ -40,15 +49,15 @@
         print('Your role:', team_role)
         if team_status != 'Accepted':
             warnings.warn('Your team is not accepted')
         if team_role_status != 'Accepted':
             warnings.warn('Your team role is not accepted')
         return team_id
 
-    def login(self, username, password):
+    def login(self, username: str, password: str):
         """
         login to igem.org
         :param username: your username
         :param password: your password
         """
         data = {
             "username": username,
@@ -63,20 +72,21 @@
         else:
             self.status = LOGGED_FAILED
             tree = etree.HTML(response.text)
             err_info = str(tree.xpath('/html/body/form/div[1]')[0].text).split('.')[0] + '.'
             warnings.warn(err_info)
             exit(1)
 
-    def query(self, directory=''):
+    def query(self, directory: str = ''):
         """
         query a files/dirs in specific directory
         :param directory: (optional) directory to query, default to root directory
         :return: list of files, each file/dir as a dict
         """
+        check_parameter(directory)
         response = self.request('GET', f'https://shim-s3.igem.org/v1/teams/{self.team_id}/wiki?directory={directory}')
         res = response.json()
         if res['KeyCount'] > 0:
             print(directory if directory != '' else '/', 'found:', res['KeyCount'])
             contents = []
             if res.get('CommonPrefixes', False):
                 contents.extend(sorted(res['CommonPrefixes'], key=lambda x: x['Name']))
@@ -94,23 +104,27 @@
         elif res['KeyCount'] == 0:
             print(directory if directory != '' else '/', 'found:', res['KeyCount'])
             return []
         else:
             warnings.warn('Query failed')
             exit(1)
 
-    def upload(self, abs_file_path, directory='', list_files=True):
+    def upload(self, abs_file_path: str, directory: str = '', list_files: bool = True):
         """
         upload file to specific directory
         :param abs_file_path: absolute path of file
         :param directory: (optional) target directory, default to root directory
         :param list_files: (optional) need to list files after upload, default to True
         :type list_files: bool
         :return: file url
         """
+        check_parameter(directory)
+        if directory == '/':
+            warnings.warn('You specified \'/\' as a directory name, which may cause unknown errors')
+            exit(1)
         path_to_file = Path(abs_file_path)
         if not path_to_file.is_file():
             warnings.warn('Invalid file path: ' + abs_file_path)
             exit(1)
         mime_type = mimetypes.guess_type(abs_file_path, True)[0]
         data = {
             'directory': directory
@@ -125,21 +139,25 @@
             print()
             if list_files:
                 self.query(directory)
             return res.json()['location']
         else:
             warnings.warn('Upload failed' + res.text)
 
-    def upload_dir(self, abs_path, directory=''):
+    def upload_dir(self, abs_path: str, directory: str = ''):
         """
         upload a directory and its subdirectories to specific directory
         :param abs_path: absolute path of directory
         :param directory: (optional) target directory, default to root directory
         :return: list of files, each file/dir as a dict
         """
+        check_parameter(directory)
+        if directory == '/':
+            warnings.warn('You specified \'/\' as a directory name, which may cause unknown errors')
+            exit(1)
         path_to_dir = Path(abs_path)
         if not path_to_dir.is_dir():
             warnings.warn('Invalid directory path: ' + abs_path)
             exit(1)
         file_list = os.listdir(abs_path)
         if directory == '':
             dir_path = path_to_dir.name
@@ -150,32 +168,36 @@
                 continue
             if (path_to_dir / filename).is_file():
                 self.upload(path_to_dir / filename, dir_path, False)
             if (path_to_dir / filename).is_dir():
                 self.upload_dir(path_to_dir / filename, dir_path)
         return self.query(dir_path)
 
-    def delete(self, filename, directory='', list_files=True):
+    def delete(self, filename: str, directory: str = '', list_files: bool = True):
         """
         delete file in specific directory
         :param filename: filename
         :param directory: file parent directory, default to root directory
         :param list_files: need to list files after delete, default to True
         """
+        check_parameter(directory)
+        if directory == '/':
+            warnings.warn('You specified \'/\' as a directory name, which may cause unknown errors')
+            exit(1)
         res = self.request('DELETE',
                            f'https://shim-s3.igem.org/v1/teams/{self.team_id}/wiki/{filename}?directory={directory}')
         if res.status_code == 200:
             print(directory + '/' + filename, 'deleted')
             print()
             if list_files:
                 self.query(directory)
         else:
             warnings.warn(directory + '/' + filename + ' delete failed')
 
-    def truncate_dir(self, directory):
+    def truncate_dir(self, directory: str):
         """
         truncate a directory
         :param directory: directory to truncate
         :return: list files after truncate
         """
         contents = self.query(directory)
         for item in contents:
```

