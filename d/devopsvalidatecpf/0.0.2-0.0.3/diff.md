# Comparing `tmp/devopsvalidatecpf-0.0.2.tar.gz` & `tmp/devopsvalidatecpf-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devopsvalidatecpf-0.0.2.tar", last modified: Sun Jul  2 20:06:09 2023, max compression
+gzip compressed data, was "devopsvalidatecpf-0.0.3.tar", last modified: Sun Jul  2 21:16:17 2023, max compression
```

## Comparing `devopsvalidatecpf-0.0.2.tar` & `devopsvalidatecpf-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 20:06:09.150923 devopsvalidatecpf-0.0.2/
--rw-rw-rw-   0        0        0      648 2023-07-02 20:06:09.134930 devopsvalidatecpf-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       85 2023-06-28 23:23:56.000000 devopsvalidatecpf-0.0.2/README.md
--rw-rw-rw-   0        0        0      769 2023-07-02 20:05:01.000000 devopsvalidatecpf-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       60 2023-07-02 20:00:37.000000 devopsvalidatecpf-0.0.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-02 20:06:09.151922 devopsvalidatecpf-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-02 20:06:08.958922 devopsvalidatecpf-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-02 20:06:09.051922 devopsvalidatecpf-0.0.2/src/devopsvalidatecpf.egg-info/
--rw-rw-rw-   0        0        0      648 2023-07-02 20:06:08.000000 devopsvalidatecpf-0.0.2/src/devopsvalidatecpf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      345 2023-07-02 20:06:08.000000 devopsvalidatecpf-0.0.2/src/devopsvalidatecpf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 20:06:08.000000 devopsvalidatecpf-0.0.2/src/devopsvalidatecpf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-07-02 20:06:08.000000 devopsvalidatecpf-0.0.2/src/devopsvalidatecpf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-02 20:06:08.000000 devopsvalidatecpf-0.0.2/src/devopsvalidatecpf.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-02 20:06:09.080931 devopsvalidatecpf-0.0.2/src/validate/
--rw-rw-rw-   0        0        0        0 2023-06-29 01:40:15.000000 devopsvalidatecpf-0.0.2/src/validate/__init__.py
--rw-rw-rw-   0        0        0      773 2023-06-29 02:15:02.000000 devopsvalidatecpf-0.0.2/src/validate/validate_cpf.py
-drwxrwxrwx   0        0        0        0 2023-07-02 20:06:09.131923 devopsvalidatecpf-0.0.2/test/
--rw-rw-rw-   0        0        0      190 2023-07-02 19:51:45.000000 devopsvalidatecpf-0.0.2/test/test_validate_cpf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 21:16:17.119365 devopsvalidatecpf-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-02 21:16:17.119365 devopsvalidatecpf-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-02 21:16:07.000000 devopsvalidatecpf-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-02 21:16:07.000000 devopsvalidatecpf-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-02 21:16:07.000000 devopsvalidatecpf-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 21:16:17.119365 devopsvalidatecpf-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 21:16:17.119365 devopsvalidatecpf-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 21:16:17.119365 devopsvalidatecpf-0.0.3/src/devopsvalidatecpf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-02 21:16:17.000000 devopsvalidatecpf-0.0.3/src/devopsvalidatecpf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-02 21:16:17.000000 devopsvalidatecpf-0.0.3/src/devopsvalidatecpf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 21:16:17.000000 devopsvalidatecpf-0.0.3/src/devopsvalidatecpf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-02 21:16:17.000000 devopsvalidatecpf-0.0.3/src/devopsvalidatecpf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-02 21:16:17.000000 devopsvalidatecpf-0.0.3/src/devopsvalidatecpf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 21:16:17.119365 devopsvalidatecpf-0.0.3/src/validate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 21:16:07.000000 devopsvalidatecpf-0.0.3/src/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-02 21:16:07.000000 devopsvalidatecpf-0.0.3/src/validate/validate_cpf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 21:16:17.119365 devopsvalidatecpf-0.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-02 21:16:07.000000 devopsvalidatecpf-0.0.3/test/test_validate_cpf.py
```

### Comparing `devopsvalidatecpf-0.0.2/pyproject.toml` & `devopsvalidatecpf-0.0.3/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "devopsvalidatecpf"
-version = "0.0.2"
-authors = [
-  { name="Ezequiel Lima", email="ezequiel_lima@hotmail.com" },
-]
-description = "DevOps course CPF validation package"
-readme = "README.md"
-requires-python = ">=3.10"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-dynamic = ["dependencies"]
-
-[tool.setuptools.dynamic]
-dependencies = {file = ["requirements.txt"]}
-
-[project.urls]
-"Homepage" = "https://github.com/ezequielcdelima/projeto-final-puc-devops"
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "devopsvalidatecpf"
+version = "0.0.3"
+authors = [
+  { name="Ezequiel Lima", email="ezequiel_lima@hotmail.com" },
+]
+description = "DevOps course CPF validation package"
+readme = "README.md"
+requires-python = ">=3.10"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+dynamic = ["dependencies"]
+
+[tool.setuptools.dynamic]
+dependencies = {file = ["requirements.txt"]}
+
+[project.urls]
+"Homepage" = "https://github.com/ezequielcdelima/projeto-final-puc-devops"
 "Bug Tracker" = "https://github.com/ezequielcdelima/projeto-final-puc-devops/issues"
```

