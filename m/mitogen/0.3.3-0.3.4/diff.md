# Comparing `tmp/mitogen-0.3.3.tar.gz` & `tmp/mitogen-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mitogen-0.3.3.tar", last modified: Sun Jun 12 10:59:02 2022, max compression
+gzip compressed data, was "mitogen-0.3.4.tar", last modified: Sun Jul  2 18:44:33 2023, max compression
```

## Comparing `mitogen-0.3.3.tar` & `mitogen-0.3.4.tar`

### file list

```diff
@@ -1,97 +1,93 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-06-12 10:59:02.000000 mitogen-0.3.3/
--rw-r--r--   0 alex       (501) staff       (20)     1755 2022-06-12 10:59:02.000000 mitogen-0.3.3/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)     1465 2021-12-15 12:14:30.000000 mitogen-0.3.3/LICENSE
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-06-12 10:59:02.000000 mitogen-0.3.3/ansible_mitogen/
--rw-r--r--   0 alex       (501) staff       (20)     4924 2022-06-12 10:57:37.000000 mitogen-0.3.3/ansible_mitogen/logging.py
--rw-r--r--   0 alex       (501) staff       (20)    22000 2022-06-12 10:57:37.000000 mitogen-0.3.3/ansible_mitogen/planner.py
--rw-r--r--   0 alex       (501) staff       (20)    21499 2022-06-12 10:57:37.000000 mitogen-0.3.3/ansible_mitogen/mixins.py
--rw-r--r--   0 alex       (501) staff       (20)    34775 2022-06-12 10:57:37.000000 mitogen-0.3.3/ansible_mitogen/runner.py
--rw-r--r--   0 alex       (501) staff       (20)    20647 2022-06-12 10:57:37.000000 mitogen-0.3.3/ansible_mitogen/services.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-06-12 10:59:02.000000 mitogen-0.3.3/ansible_mitogen/compat/
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-06-12 10:59:02.000000 mitogen-0.3.3/ansible_mitogen/compat/simplejson/
--rw-r--r--   0 alex       (501) staff       (20)    12404 2022-06-12 10:56:48.000000 mitogen-0.3.3/ansible_mitogen/compat/simplejson/decoder.py
--rw-r--r--   0 alex       (501) staff       (20)     2227 2022-06-12 10:56:48.000000 mitogen-0.3.3/ansible_mitogen/compat/simplejson/scanner.py
--rw-r--r--   0 alex       (501) staff       (20)    12463 2022-06-12 10:56:48.000000 mitogen-0.3.3/ansible_mitogen/compat/simplejson/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)    16033 2022-06-12 10:56:48.000000 mitogen-0.3.3/ansible_mitogen/compat/simplejson/encoder.py
--rw-r-----   0 alex       (501) staff       (20)        0 2021-10-31 14:17:43.000000 mitogen-0.3.3/ansible_mitogen/compat/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     3122 2022-06-12 10:57:37.000000 mitogen-0.3.3/ansible_mitogen/parsing.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-06-12 10:59:02.000000 mitogen-0.3.3/ansible_mitogen/plugins/
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-06-12 10:59:02.000000 mitogen-0.3.3/ansible_mitogen/plugins/connection/
--rw-r--r--   0 alex       (501) staff       (20)     3119 2022-06-12 10:57:37.000000 mitogen-0.3.3/ansible_mitogen/plugins/connection/mitogen_kubectl.py
--rw-r--r--   0 alex       (501) staff       (20)     3134 2022-06-12 10:57:37.000000 mitogen-0.3.3/ansible_mitogen/plugins/connection/mitogen_local.py
--rw-r--r--   0 alex       (501) staff       (20)     1944 2022-06-12 10:57:37.000000 mitogen-0.3.3/ansible_mitogen/plugins/connection/mitogen_doas.py
--rw-r--r--   0 alex       (501) staff       (20)     1925 2022-06-12 10:57:37.000000 mitogen-0.3.3/ansible_mitogen/plugins/connection/mitogen_jail.py
--rw-r-----   0 alex       (501) staff       (20)        0 2021-10-31 14:17:43.000000 mitogen-0.3.3/ansible_mitogen/plugins/connection/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     2719 2022-06-12 10:57:37.000000 mitogen-0.3.3/ansible_mitogen/plugins/connection/mitogen_ssh.py
--rw-r--r--   0 alex       (501) staff       (20)     1942 2022-06-12 10:57:37.000000 mitogen-0.3.3/ansible_mitogen/plugins/connection/mitogen_su.py
--rw-r--r--   0 alex       (501) staff       (20)     1944 2022-06-12 10:57:37.000000 mitogen-0.3.3/ansible_mitogen/plugins/connection/mitogen_sudo.py
--rw-r--r--   0 alex       (501) staff       (20)     1924 2022-06-12 10:57:37.000000 mitogen-0.3.3/ansible_mitogen/plugins/connection/mitogen_lxd.py
--rw-r--r--   0 alex       (501) staff       (20)     1937 2022-06-12 10:57:37.000000 mitogen-0.3.3/ansible_mitogen/plugins/connection/mitogen_setns.py
--rw-r--r--   0 alex       (501) staff       (20)     1924 2022-06-12 10:57:37.000000 mitogen-0.3.3/ansible_mitogen/plugins/connection/mitogen_lxc.py
--rw-r--r--   0 alex       (501) staff       (20)     1928 2022-06-12 10:57:37.000000 mitogen-0.3.3/ansible_mitogen/plugins/connection/mitogen_buildah.py
--rw-r--r--   0 alex       (501) staff       (20)     1935 2022-06-12 10:57:37.000000 mitogen-0.3.3/ansible_mitogen/plugins/connection/mitogen_podman.py
--rw-r--r--   0 alex       (501) staff       (20)     1942 2022-06-12 10:57:37.000000 mitogen-0.3.3/ansible_mitogen/plugins/connection/mitogen_machinectl.py
--rw-r--r--   0 alex       (501) staff       (20)     2088 2022-06-12 10:57:37.000000 mitogen-0.3.3/ansible_mitogen/plugins/connection/mitogen_docker.py
--rw-r-----   0 alex       (501) staff       (20)        0 2021-10-31 14:17:43.000000 mitogen-0.3.3/ansible_mitogen/plugins/__init__.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-06-12 10:59:02.000000 mitogen-0.3.3/ansible_mitogen/plugins/action/
--rw-r--r--   0 alex       (501) staff       (20)     9840 2022-06-12 10:57:37.000000 mitogen-0.3.3/ansible_mitogen/plugins/action/mitogen_fetch.py
--rw-r-----   0 alex       (501) staff       (20)        0 2022-04-23 07:08:36.000000 mitogen-0.3.3/ansible_mitogen/plugins/action/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     2448 2022-06-12 10:57:37.000000 mitogen-0.3.3/ansible_mitogen/plugins/action/mitogen_get_stack.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-06-12 10:59:02.000000 mitogen-0.3.3/ansible_mitogen/plugins/strategy/
--rw-r--r--   0 alex       (501) staff       (20)     2943 2022-06-12 10:57:37.000000 mitogen-0.3.3/ansible_mitogen/plugins/strategy/mitogen_host_pinned.py
--rw-r--r--   0 alex       (501) staff       (20)     2805 2022-06-12 10:57:37.000000 mitogen-0.3.3/ansible_mitogen/plugins/strategy/mitogen.py
--rw-r-----   0 alex       (501) staff       (20)        0 2021-10-31 14:17:43.000000 mitogen-0.3.3/ansible_mitogen/plugins/strategy/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     2811 2022-06-12 10:57:37.000000 mitogen-0.3.3/ansible_mitogen/plugins/strategy/mitogen_free.py
--rw-r--r--   0 alex       (501) staff       (20)     2813 2022-06-12 10:57:37.000000 mitogen-0.3.3/ansible_mitogen/plugins/strategy/mitogen_linear.py
--rw-r--r--   0 alex       (501) staff       (20)     3781 2022-06-12 10:57:37.000000 mitogen-0.3.3/ansible_mitogen/loaders.py
--rw-r--r--   0 alex       (501) staff       (20)    10196 2022-06-12 10:57:37.000000 mitogen-0.3.3/ansible_mitogen/affinity.py
--rw-r-----   0 alex       (501) staff       (20)        0 2021-10-31 14:17:43.000000 mitogen-0.3.3/ansible_mitogen/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)    12611 2022-06-12 10:57:37.000000 mitogen-0.3.3/ansible_mitogen/strategy.py
--rw-r--r--   0 alex       (501) staff       (20)     5140 2022-06-12 10:57:37.000000 mitogen-0.3.3/ansible_mitogen/module_finder.py
--rw-r--r--   0 alex       (501) staff       (20)    26889 2022-06-12 10:57:37.000000 mitogen-0.3.3/ansible_mitogen/transport_config.py
--rw-r--r--   0 alex       (501) staff       (20)    39355 2022-06-12 10:57:37.000000 mitogen-0.3.3/ansible_mitogen/connection.py
--rw-r--r--   0 alex       (501) staff       (20)      278 2022-06-12 10:57:37.000000 mitogen-0.3.3/ansible_mitogen/utils.py
--rw-r--r--   0 alex       (501) staff       (20)    25388 2022-06-12 10:57:37.000000 mitogen-0.3.3/ansible_mitogen/target.py
--rw-r--r--   0 alex       (501) staff       (20)    26191 2022-06-12 10:57:37.000000 mitogen-0.3.3/ansible_mitogen/process.py
--rw-r-----   0 alex       (501) staff       (20)       16 2021-10-31 14:17:43.000000 mitogen-0.3.3/MANIFEST.in
--rw-r--r--   0 alex       (501) staff       (20)      495 2021-12-15 12:14:30.000000 mitogen-0.3.3/README.md
--rw-r--r--   0 alex       (501) staff       (20)     3491 2022-06-12 10:57:37.000000 mitogen-0.3.3/setup.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-06-12 10:59:02.000000 mitogen-0.3.3/mitogen/
--rw-r--r--   0 alex       (501) staff       (20)    41691 2022-06-12 10:57:37.000000 mitogen-0.3.3/mitogen/service.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-06-12 10:59:02.000000 mitogen-0.3.3/mitogen/compat/
--rw-r--r--   0 alex       (501) staff       (20)     3037 2022-06-02 12:15:58.000000 mitogen-0.3.3/mitogen/compat/shutil.py
--rw-r--r--   0 alex       (501) staff       (20)    20406 2022-06-02 12:33:49.000000 mitogen-0.3.3/mitogen/compat/pkgutil.py
--rw-r-----   0 alex       (501) staff       (20)        0 2022-04-23 07:08:36.000000 mitogen-0.3.3/mitogen/compat/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)    17572 2022-06-02 12:33:49.000000 mitogen-0.3.3/mitogen/compat/tokenize.py
--rw-r--r--   0 alex       (501) staff       (20)     7133 2022-06-02 12:35:19.000000 mitogen-0.3.3/mitogen/unix.py
--rw-r--r--   0 alex       (501) staff       (20)     2853 2022-06-12 10:57:37.000000 mitogen-0.3.3/mitogen/lxc.py
--rw-r--r--   0 alex       (501) staff       (20)     5093 2022-06-02 12:35:19.000000 mitogen-0.3.3/mitogen/minify.py
--rw-r--r--   0 alex       (501) staff       (20)    12089 2022-06-02 12:35:19.000000 mitogen-0.3.3/mitogen/sudo.py
--rw-r--r--   0 alex       (501) staff       (20)     2730 2022-06-12 10:57:37.000000 mitogen-0.3.3/mitogen/podman.py
--rw-r--r--   0 alex       (501) staff       (20)     8436 2022-06-02 12:35:19.000000 mitogen-0.3.3/mitogen/fork.py
--rw-r--r--   0 alex       (501) staff       (20)     2681 2022-06-12 10:57:37.000000 mitogen-0.3.3/mitogen/buildah.py
--rw-r--r--   0 alex       (501) staff       (20)    97884 2022-06-12 10:57:37.000000 mitogen-0.3.3/mitogen/parent.py
--rw-r--r--   0 alex       (501) staff       (20)     4145 2022-06-12 10:57:37.000000 mitogen-0.3.3/mitogen/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)   145257 2022-06-12 10:57:37.000000 mitogen-0.3.3/mitogen/core.py
--rw-r--r--   0 alex       (501) staff       (20)     2537 2022-06-02 12:35:19.000000 mitogen-0.3.3/mitogen/jail.py
--rw-r--r--   0 alex       (501) staff       (20)     4958 2022-06-02 12:35:19.000000 mitogen-0.3.3/mitogen/doas.py
--rw-r--r--   0 alex       (501) staff       (20)     5656 2022-06-02 12:35:19.000000 mitogen-0.3.3/mitogen/su.py
--rw-r--r--   0 alex       (501) staff       (20)     3085 2022-06-02 12:35:19.000000 mitogen-0.3.3/mitogen/docker.py
--rw-r--r--   0 alex       (501) staff       (20)     6624 2022-06-12 10:57:37.000000 mitogen-0.3.3/mitogen/os_fork.py
--rw-r--r--   0 alex       (501) staff       (20)     8450 2022-06-02 12:35:19.000000 mitogen-0.3.3/mitogen/setns.py
--rw-r--r--   0 alex       (501) staff       (20)    50896 2022-06-12 10:57:37.000000 mitogen-0.3.3/mitogen/master.py
--rw-r--r--   0 alex       (501) staff       (20)     7167 2022-06-12 10:57:37.000000 mitogen-0.3.3/mitogen/utils.py
--rw-r--r--   0 alex       (501) staff       (20)     6699 2022-06-02 12:35:19.000000 mitogen-0.3.3/mitogen/debug.py
--rw-r--r--   0 alex       (501) staff       (20)    10892 2022-06-02 12:35:19.000000 mitogen-0.3.3/mitogen/ssh.py
--rw-r--r--   0 alex       (501) staff       (20)    12325 2022-06-02 12:35:19.000000 mitogen-0.3.3/mitogen/select.py
--rw-r--r--   0 alex       (501) staff       (20)    15577 2022-06-12 10:57:37.000000 mitogen-0.3.3/mitogen/fakessh.py
--rw-r--r--   0 alex       (501) staff       (20)     5392 2022-06-02 12:35:19.000000 mitogen-0.3.3/mitogen/profiler.py
--rw-r--r--   0 alex       (501) staff       (20)     2844 2022-06-12 10:57:37.000000 mitogen-0.3.3/mitogen/lxd.py
--rw-r--r--   0 alex       (501) staff       (20)     2561 2022-06-12 10:57:37.000000 mitogen-0.3.3/mitogen/kubectl.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-06-12 10:59:02.000000 mitogen-0.3.3/mitogen.egg-info/
--rwxrwx---   0 alex       (501) staff       (20)     1755 2022-06-12 10:59:02.000000 mitogen-0.3.3/mitogen.egg-info/PKG-INFO
--rwxrwx---   0 alex       (501) staff       (20)        1 2018-03-10 21:10:22.000000 mitogen-0.3.3/mitogen.egg-info/not-zip-safe
--rwxrwx---   0 alex       (501) staff       (20)     2619 2022-06-12 10:59:02.000000 mitogen-0.3.3/mitogen.egg-info/SOURCES.txt
--rwxrwx---   0 alex       (501) staff       (20)       24 2022-06-12 10:59:02.000000 mitogen-0.3.3/mitogen.egg-info/top_level.txt
--rwxrwx---   0 alex       (501) staff       (20)        1 2022-06-12 10:59:02.000000 mitogen-0.3.3/mitogen.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)      206 2022-06-12 10:59:02.000000 mitogen-0.3.3/setup.cfg
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-02 18:44:33.594516 mitogen-0.3.4/
+-rw-r--r--   0 alex       (501) staff       (20)     1465 2022-06-24 21:10:35.000000 mitogen-0.3.4/LICENSE
+-rw-r--r--   0 alex       (501) staff       (20)       16 2022-06-24 21:04:22.000000 mitogen-0.3.4/MANIFEST.in
+-rw-r--r--   0 alex       (501) staff       (20)     1674 2023-07-02 18:44:33.594606 mitogen-0.3.4/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)      495 2022-06-24 21:10:35.000000 mitogen-0.3.4/README.md
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-02 18:44:33.582419 mitogen-0.3.4/ansible_mitogen/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2022-06-24 21:04:22.000000 mitogen-0.3.4/ansible_mitogen/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)    10196 2022-06-24 21:10:35.000000 mitogen-0.3.4/ansible_mitogen/affinity.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-02 18:44:33.582620 mitogen-0.3.4/ansible_mitogen/compat/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2022-06-24 21:04:22.000000 mitogen-0.3.4/ansible_mitogen/compat/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)    39600 2023-07-02 18:42:28.000000 mitogen-0.3.4/ansible_mitogen/connection.py
+-rw-r--r--   0 alex       (501) staff       (20)     3851 2023-07-02 18:42:28.000000 mitogen-0.3.4/ansible_mitogen/loaders.py
+-rw-r--r--   0 alex       (501) staff       (20)     4924 2022-06-24 21:10:35.000000 mitogen-0.3.4/ansible_mitogen/logging.py
+-rw-r--r--   0 alex       (501) staff       (20)    21499 2022-06-24 21:10:35.000000 mitogen-0.3.4/ansible_mitogen/mixins.py
+-rw-r--r--   0 alex       (501) staff       (20)     5140 2022-06-24 21:10:35.000000 mitogen-0.3.4/ansible_mitogen/module_finder.py
+-rw-r--r--   0 alex       (501) staff       (20)     3122 2022-06-24 21:10:35.000000 mitogen-0.3.4/ansible_mitogen/parsing.py
+-rw-r--r--   0 alex       (501) staff       (20)    22044 2023-07-02 18:42:28.000000 mitogen-0.3.4/ansible_mitogen/planner.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-02 18:44:33.582709 mitogen-0.3.4/ansible_mitogen/plugins/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2022-06-24 21:04:22.000000 mitogen-0.3.4/ansible_mitogen/plugins/__init__.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-02 18:44:33.583124 mitogen-0.3.4/ansible_mitogen/plugins/action/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2022-06-24 21:04:22.000000 mitogen-0.3.4/ansible_mitogen/plugins/action/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     9840 2022-06-24 21:10:35.000000 mitogen-0.3.4/ansible_mitogen/plugins/action/mitogen_fetch.py
+-rw-r--r--   0 alex       (501) staff       (20)     2448 2022-06-24 21:10:35.000000 mitogen-0.3.4/ansible_mitogen/plugins/action/mitogen_get_stack.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-02 18:44:33.586014 mitogen-0.3.4/ansible_mitogen/plugins/connection/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2022-06-24 21:04:22.000000 mitogen-0.3.4/ansible_mitogen/plugins/connection/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     1928 2022-06-24 21:10:35.000000 mitogen-0.3.4/ansible_mitogen/plugins/connection/mitogen_buildah.py
+-rw-r--r--   0 alex       (501) staff       (20)     1944 2022-06-24 21:10:35.000000 mitogen-0.3.4/ansible_mitogen/plugins/connection/mitogen_doas.py
+-rw-r--r--   0 alex       (501) staff       (20)     2088 2022-06-24 21:10:35.000000 mitogen-0.3.4/ansible_mitogen/plugins/connection/mitogen_docker.py
+-rw-r--r--   0 alex       (501) staff       (20)     1925 2022-06-24 21:10:35.000000 mitogen-0.3.4/ansible_mitogen/plugins/connection/mitogen_jail.py
+-rw-r--r--   0 alex       (501) staff       (20)     3119 2022-06-24 21:10:35.000000 mitogen-0.3.4/ansible_mitogen/plugins/connection/mitogen_kubectl.py
+-rw-r--r--   0 alex       (501) staff       (20)     3134 2022-06-24 21:10:35.000000 mitogen-0.3.4/ansible_mitogen/plugins/connection/mitogen_local.py
+-rw-r--r--   0 alex       (501) staff       (20)     1924 2022-06-24 21:10:35.000000 mitogen-0.3.4/ansible_mitogen/plugins/connection/mitogen_lxc.py
+-rw-r--r--   0 alex       (501) staff       (20)     1924 2022-06-24 21:10:35.000000 mitogen-0.3.4/ansible_mitogen/plugins/connection/mitogen_lxd.py
+-rw-r--r--   0 alex       (501) staff       (20)     1942 2022-06-24 21:10:35.000000 mitogen-0.3.4/ansible_mitogen/plugins/connection/mitogen_machinectl.py
+-rw-r--r--   0 alex       (501) staff       (20)     1935 2022-06-24 21:10:35.000000 mitogen-0.3.4/ansible_mitogen/plugins/connection/mitogen_podman.py
+-rw-r--r--   0 alex       (501) staff       (20)     1937 2022-06-24 21:10:35.000000 mitogen-0.3.4/ansible_mitogen/plugins/connection/mitogen_setns.py
+-rw-r--r--   0 alex       (501) staff       (20)     3301 2023-07-02 18:42:28.000000 mitogen-0.3.4/ansible_mitogen/plugins/connection/mitogen_ssh.py
+-rw-r--r--   0 alex       (501) staff       (20)     1942 2022-06-24 21:10:35.000000 mitogen-0.3.4/ansible_mitogen/plugins/connection/mitogen_su.py
+-rw-r--r--   0 alex       (501) staff       (20)     1944 2022-06-24 21:10:35.000000 mitogen-0.3.4/ansible_mitogen/plugins/connection/mitogen_sudo.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-02 18:44:33.587112 mitogen-0.3.4/ansible_mitogen/plugins/strategy/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2022-06-24 21:04:22.000000 mitogen-0.3.4/ansible_mitogen/plugins/strategy/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     2805 2022-06-24 21:10:35.000000 mitogen-0.3.4/ansible_mitogen/plugins/strategy/mitogen.py
+-rw-r--r--   0 alex       (501) staff       (20)     2811 2022-06-24 21:10:35.000000 mitogen-0.3.4/ansible_mitogen/plugins/strategy/mitogen_free.py
+-rw-r--r--   0 alex       (501) staff       (20)     2943 2022-06-24 21:10:35.000000 mitogen-0.3.4/ansible_mitogen/plugins/strategy/mitogen_host_pinned.py
+-rw-r--r--   0 alex       (501) staff       (20)     2813 2022-06-24 21:10:35.000000 mitogen-0.3.4/ansible_mitogen/plugins/strategy/mitogen_linear.py
+-rw-r--r--   0 alex       (501) staff       (20)    24921 2023-07-02 18:42:28.000000 mitogen-0.3.4/ansible_mitogen/process.py
+-rw-r--r--   0 alex       (501) staff       (20)    34698 2023-07-02 18:42:28.000000 mitogen-0.3.4/ansible_mitogen/runner.py
+-rw-r--r--   0 alex       (501) staff       (20)    20647 2022-08-25 18:47:42.000000 mitogen-0.3.4/ansible_mitogen/services.py
+-rw-r--r--   0 alex       (501) staff       (20)    12611 2022-06-24 21:10:35.000000 mitogen-0.3.4/ansible_mitogen/strategy.py
+-rw-r--r--   0 alex       (501) staff       (20)    25091 2023-07-02 18:42:28.000000 mitogen-0.3.4/ansible_mitogen/target.py
+-rw-r--r--   0 alex       (501) staff       (20)    27116 2023-07-02 18:42:28.000000 mitogen-0.3.4/ansible_mitogen/transport_config.py
+-rw-r--r--   0 alex       (501) staff       (20)      278 2022-06-24 21:10:35.000000 mitogen-0.3.4/ansible_mitogen/utils.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-02 18:44:33.592330 mitogen-0.3.4/mitogen/
+-rw-r--r--   0 alex       (501) staff       (20)     4145 2023-07-02 18:42:28.000000 mitogen-0.3.4/mitogen/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     2681 2022-08-25 18:47:42.000000 mitogen-0.3.4/mitogen/buildah.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-02 18:44:33.594098 mitogen-0.3.4/mitogen/compat/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2022-06-24 21:04:22.000000 mitogen-0.3.4/mitogen/compat/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)    20406 2022-08-25 18:47:42.000000 mitogen-0.3.4/mitogen/compat/pkgutil.py
+-rw-r--r--   0 alex       (501) staff       (20)    17572 2022-08-25 18:47:42.000000 mitogen-0.3.4/mitogen/compat/tokenize.py
+-rw-r--r--   0 alex       (501) staff       (20)   145257 2022-08-25 18:47:42.000000 mitogen-0.3.4/mitogen/core.py
+-rw-r--r--   0 alex       (501) staff       (20)     6699 2022-08-25 18:47:42.000000 mitogen-0.3.4/mitogen/debug.py
+-rw-r--r--   0 alex       (501) staff       (20)     4958 2022-08-25 18:47:42.000000 mitogen-0.3.4/mitogen/doas.py
+-rw-r--r--   0 alex       (501) staff       (20)     3085 2022-08-25 18:47:42.000000 mitogen-0.3.4/mitogen/docker.py
+-rw-r--r--   0 alex       (501) staff       (20)    15577 2022-08-25 18:47:42.000000 mitogen-0.3.4/mitogen/fakessh.py
+-rw-r--r--   0 alex       (501) staff       (20)     8436 2022-08-25 18:47:42.000000 mitogen-0.3.4/mitogen/fork.py
+-rw-r--r--   0 alex       (501) staff       (20)     2537 2022-08-25 18:47:42.000000 mitogen-0.3.4/mitogen/jail.py
+-rw-r--r--   0 alex       (501) staff       (20)     2561 2022-08-25 18:47:42.000000 mitogen-0.3.4/mitogen/kubectl.py
+-rw-r--r--   0 alex       (501) staff       (20)     2853 2022-08-25 18:47:42.000000 mitogen-0.3.4/mitogen/lxc.py
+-rw-r--r--   0 alex       (501) staff       (20)     2844 2022-08-25 18:47:42.000000 mitogen-0.3.4/mitogen/lxd.py
+-rw-r--r--   0 alex       (501) staff       (20)    50908 2023-07-02 18:42:28.000000 mitogen-0.3.4/mitogen/master.py
+-rw-r--r--   0 alex       (501) staff       (20)     5093 2022-08-25 18:47:42.000000 mitogen-0.3.4/mitogen/minify.py
+-rw-r--r--   0 alex       (501) staff       (20)     6624 2022-08-25 18:47:42.000000 mitogen-0.3.4/mitogen/os_fork.py
+-rw-r--r--   0 alex       (501) staff       (20)    97884 2022-08-25 18:47:42.000000 mitogen-0.3.4/mitogen/parent.py
+-rw-r--r--   0 alex       (501) staff       (20)     2730 2022-08-25 18:47:42.000000 mitogen-0.3.4/mitogen/podman.py
+-rw-r--r--   0 alex       (501) staff       (20)     5392 2022-08-25 18:47:42.000000 mitogen-0.3.4/mitogen/profiler.py
+-rw-r--r--   0 alex       (501) staff       (20)    12325 2022-08-25 18:47:42.000000 mitogen-0.3.4/mitogen/select.py
+-rw-r--r--   0 alex       (501) staff       (20)    41691 2022-08-25 18:47:42.000000 mitogen-0.3.4/mitogen/service.py
+-rw-r--r--   0 alex       (501) staff       (20)     8450 2022-08-25 18:47:42.000000 mitogen-0.3.4/mitogen/setns.py
+-rw-r--r--   0 alex       (501) staff       (20)    10892 2023-07-02 14:09:52.000000 mitogen-0.3.4/mitogen/ssh.py
+-rw-r--r--   0 alex       (501) staff       (20)     5656 2022-08-25 18:47:42.000000 mitogen-0.3.4/mitogen/su.py
+-rw-r--r--   0 alex       (501) staff       (20)    12089 2022-08-25 18:47:42.000000 mitogen-0.3.4/mitogen/sudo.py
+-rw-r--r--   0 alex       (501) staff       (20)     7133 2022-08-25 18:47:42.000000 mitogen-0.3.4/mitogen/unix.py
+-rw-r--r--   0 alex       (501) staff       (20)     7167 2022-08-25 18:47:42.000000 mitogen-0.3.4/mitogen/utils.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-02 18:44:33.593568 mitogen-0.3.4/mitogen.egg-info/
+-rwxrwx---   0 alex       (501) staff       (20)     1674 2023-07-02 18:44:33.000000 mitogen-0.3.4/mitogen.egg-info/PKG-INFO
+-rwxrwx---   0 alex       (501) staff       (20)     2430 2023-07-02 18:44:33.000000 mitogen-0.3.4/mitogen.egg-info/SOURCES.txt
+-rwxrwx---   0 alex       (501) staff       (20)        1 2023-07-02 18:44:33.000000 mitogen-0.3.4/mitogen.egg-info/dependency_links.txt
+-rwxrwx---   0 alex       (501) staff       (20)        1 2018-03-10 21:10:22.000000 mitogen-0.3.4/mitogen.egg-info/not-zip-safe
+-rwxrwx---   0 alex       (501) staff       (20)       24 2023-07-02 18:44:33.000000 mitogen-0.3.4/mitogen.egg-info/top_level.txt
+-rw-r--r--   0 alex       (501) staff       (20)      206 2023-07-02 18:44:33.594879 mitogen-0.3.4/setup.cfg
+-rw-r--r--   0 alex       (501) staff       (20)     3491 2022-06-24 21:10:35.000000 mitogen-0.3.4/setup.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-02 18:44:33.594379 mitogen-0.3.4/tests/
+-rw-r--r--   0 alex       (501) staff       (20)    19717 2023-07-02 18:42:28.000000 mitogen-0.3.4/tests/testlib.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mitogen-0.3.3/PKG-INFO` & `mitogen-0.3.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,14 @@
 Metadata-Version: 2.1
 Name: mitogen
-Version: 0.3.3
+Version: 0.3.4
 Summary: Library for writing distributed self-replicating programs.
 Home-page: https://github.com/mitogen-hq/mitogen/
 Author: David Wilson
 License: New BSD
-Description: # Mitogen
-        
-        <a href="https://mitogen.networkgenomics.com/">Please see the documentation</a>.
-        
-        ![](https://i.imgur.com/eBM6LhJ.gif)
-        
-        [![Total alerts](https://img.shields.io/lgtm/alerts/g/mitogen-hq/mitogen.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/mitogen-hq/mitogen/alerts/)
-        
-        [![Build Status](https://dev.azure.com/mitogen-hq/mitogen/_apis/build/status/mitogen-hq.mitogen?branchName=master)](https://dev.azure.com/mitogen-hq/mitogen/_build/latest?definitionId=1&branchName=master)
-        
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Framework :: Ansible
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
@@ -31,7 +20,18 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: System :: Distributed Computing
 Classifier: Topic :: System :: Systems Administration
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Mitogen
+
+<a href="https://mitogen.networkgenomics.com/">Please see the documentation</a>.
+
+![](https://i.imgur.com/eBM6LhJ.gif)
+
+[![Total alerts](https://img.shields.io/lgtm/alerts/g/mitogen-hq/mitogen.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/mitogen-hq/mitogen/alerts/)
+
+[![Build Status](https://dev.azure.com/mitogen-hq/mitogen/_apis/build/status/mitogen-hq.mitogen?branchName=master)](https://dev.azure.com/mitogen-hq/mitogen/_build/latest?definitionId=1&branchName=master)
```

#### html2text {}

```diff
@@ -1,23 +1,22 @@
-Metadata-Version: 2.1 Name: mitogen Version: 0.3.3 Summary: Library for writing
+Metadata-Version: 2.1 Name: mitogen Version: 0.3.4 Summary: Library for writing
 distributed self-replicating programs. Home-page: https://github.com/mitogen-
-hq/mitogen/ Author: David Wilson License: New BSD Description: # Mitogen Please
-see_the_documentation. ![](https://i.imgur.com/eBM6LhJ.gif) [![Total alerts]
-(https://img.shields.io/lgtm/alerts/g/mitogen-hq/
-mitogen.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/mitogen-hq/
-mitogen/alerts/) [![Build Status](https://dev.azure.com/mitogen-hq/mitogen/
-_apis/build/status/mitogen-hq.mitogen?branchName=master)](https://
-dev.azure.com/mitogen-hq/mitogen/_build/
-latest?definitionId=1&branchName=master) Platform: UNKNOWN Classifier:
-Environment :: Console Classifier: Framework :: Ansible Classifier: Intended
-Audience :: System Administrators Classifier: License :: OSI Approved :: BSD
-License Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating
-System :: POSIX Classifier: Programming Language :: Python Classifier:
-Programming Language :: Python :: 2.7 Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.6 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: Implementation :: CPython Classifier: Topic :: System :: Distributed
-Computing Classifier: Topic :: System :: Systems Administration Requires-
-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
-Description-Content-Type: text/markdown
+hq/mitogen/ Author: David Wilson License: New BSD Classifier: Environment ::
+Console Classifier: Framework :: Ansible Classifier: Intended Audience ::
+System Administrators Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
+:: POSIX Classifier: Programming Language :: Python Classifier: Programming
+Language :: Python :: 2.7 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python ::
+Implementation :: CPython Classifier: Topic :: System :: Distributed Computing
+Classifier: Topic :: System :: Systems Administration Requires-Python: >=2.7,
+!=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.* Description-Content-Type:
+text/markdown License-File: LICENSE # Mitogen Please_see_the_documentation. ![]
+(https://i.imgur.com/eBM6LhJ.gif) [![Total alerts](https://img.shields.io/lgtm/
+alerts/g/mitogen-hq/mitogen.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/
+projects/g/mitogen-hq/mitogen/alerts/) [![Build Status](https://dev.azure.com/
+mitogen-hq/mitogen/_apis/build/status/mitogen-hq.mitogen?branchName=master)]
+(https://dev.azure.com/mitogen-hq/mitogen/_build/
+latest?definitionId=1&branchName=master)
```

### Comparing `mitogen-0.3.3/LICENSE` & `mitogen-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.3/ansible_mitogen/logging.py` & `mitogen-0.3.4/ansible_mitogen/logging.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.3/ansible_mitogen/planner.py` & `mitogen-0.3.4/ansible_mitogen/planner.py`

 * *Files 1% similar despite different names*

```diff
@@ -319,14 +319,15 @@
     #: Module names appearing in this set always require forking, usually due
     #: to some terminal leakage that cannot be worked around in any sane
     #: manner.
     ALWAYS_FORK_MODULES = frozenset([
         'dnf',  # issue #280; py-dnf/hawkey need therapy
         'firewalld',  # issue #570: ansible module_utils caches dbus conn
         'ansible.legacy.dnf',  # issue #776
+        'ansible.builtin.dnf', # issue #832
     ])
 
     def should_fork(self):
         """
         In addition to asynchronous tasks, new-style modules should be forked
         if:
```

### Comparing `mitogen-0.3.3/ansible_mitogen/mixins.py` & `mitogen-0.3.4/ansible_mitogen/mixins.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.3/ansible_mitogen/runner.py` & `mitogen-0.3.4/ansible_mitogen/runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 """
 
 from __future__ import absolute_import, division, print_function
 __metaclass__ = type
 
 import atexit
 import imp
+import json
 import os
 import re
 import shlex
 import shutil
 import sys
 import tempfile
 import traceback
@@ -60,20 +61,14 @@
 try:
     import ctypes
 except ImportError:
     # Python 2.4
     ctypes = None
 
 try:
-    import json
-except ImportError:
-    # Python 2.4
-    import simplejson as json
-
-try:
     # Cannot use cStringIO as it does not support Unicode.
     from StringIO import StringIO
 except ImportError:
     from io import StringIO
 
 try:
     from shlex import quote as shlex_quote
```

### Comparing `mitogen-0.3.3/ansible_mitogen/services.py` & `mitogen-0.3.4/ansible_mitogen/services.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.3/ansible_mitogen/parsing.py` & `mitogen-0.3.4/ansible_mitogen/parsing.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.3/ansible_mitogen/plugins/connection/mitogen_kubectl.py` & `mitogen-0.3.4/ansible_mitogen/plugins/connection/mitogen_kubectl.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.3/ansible_mitogen/plugins/connection/mitogen_local.py` & `mitogen-0.3.4/ansible_mitogen/plugins/connection/mitogen_local.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.3/ansible_mitogen/plugins/connection/mitogen_doas.py` & `mitogen-0.3.4/ansible_mitogen/plugins/connection/mitogen_doas.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.3/ansible_mitogen/plugins/connection/mitogen_jail.py` & `mitogen-0.3.4/ansible_mitogen/plugins/connection/mitogen_jail.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.3/ansible_mitogen/plugins/connection/mitogen_ssh.py` & `mitogen-0.3.4/ansible_mitogen/plugins/connection/mitogen_su.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,42 +28,19 @@
 
 from __future__ import absolute_import, division, print_function
 __metaclass__ = type
 
 import os.path
 import sys
 
-DOCUMENTATION = """
-    author: David Wilson <dw@botanicus.net>
-    connection: mitogen_ssh
-    short_description: Connect over SSH via Mitogen
-    description:
-        - This connects using an OpenSSH client controlled by the Mitogen for
-          Ansible extension. It accepts every option the vanilla ssh plugin
-          accepts.
-    version_added: "2.5"
-    options:
-"""
-
 try:
-    import ansible_mitogen
+    import ansible_mitogen.connection
 except ImportError:
     base_dir = os.path.dirname(__file__)
     sys.path.insert(0, os.path.abspath(os.path.join(base_dir, '../../..')))
     del base_dir
 
 import ansible_mitogen.connection
-import ansible_mitogen.loaders
 
 
 class Connection(ansible_mitogen.connection.Connection):
-    transport = 'ssh'
-    vanilla_class = ansible_mitogen.loaders.connection_loader__get(
-        'ssh',
-        class_only=True,
-    )
-
-    @staticmethod
-    def _create_control_path(*args, **kwargs):
-        """Forward _create_control_path() to the implementation in ssh.py."""
-        # https://github.com/dw/mitogen/issues/342
-        return Connection.vanilla_class._create_control_path(*args, **kwargs)
+    transport = 'mitogen_su'
```

### Comparing `mitogen-0.3.3/ansible_mitogen/plugins/connection/mitogen_su.py` & `mitogen-0.3.4/ansible_mitogen/plugins/connection/mitogen_sudo.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,8 +39,8 @@
     sys.path.insert(0, os.path.abspath(os.path.join(base_dir, '../../..')))
     del base_dir
 
 import ansible_mitogen.connection
 
 
 class Connection(ansible_mitogen.connection.Connection):
-    transport = 'mitogen_su'
+    transport = 'mitogen_sudo'
```

### Comparing `mitogen-0.3.3/ansible_mitogen/plugins/connection/mitogen_sudo.py` & `mitogen-0.3.4/ansible_mitogen/plugins/connection/mitogen_lxc.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,18 +29,18 @@
 from __future__ import absolute_import, division, print_function
 __metaclass__ = type
 
 import os.path
 import sys
 
 try:
-    import ansible_mitogen.connection
+    import ansible_mitogen
 except ImportError:
     base_dir = os.path.dirname(__file__)
     sys.path.insert(0, os.path.abspath(os.path.join(base_dir, '../../..')))
     del base_dir
 
 import ansible_mitogen.connection
 
 
 class Connection(ansible_mitogen.connection.Connection):
-    transport = 'mitogen_sudo'
+    transport = 'lxc'
```

### Comparing `mitogen-0.3.3/ansible_mitogen/plugins/connection/mitogen_lxd.py` & `mitogen-0.3.4/ansible_mitogen/plugins/connection/mitogen_lxd.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.3/ansible_mitogen/plugins/connection/mitogen_setns.py` & `mitogen-0.3.4/ansible_mitogen/plugins/connection/mitogen_setns.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.3/ansible_mitogen/plugins/connection/mitogen_lxc.py` & `mitogen-0.3.4/ansible_mitogen/plugins/connection/mitogen_machinectl.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,18 +29,18 @@
 from __future__ import absolute_import, division, print_function
 __metaclass__ = type
 
 import os.path
 import sys
 
 try:
-    import ansible_mitogen
+    import ansible_mitogen.connection
 except ImportError:
     base_dir = os.path.dirname(__file__)
     sys.path.insert(0, os.path.abspath(os.path.join(base_dir, '../../..')))
     del base_dir
 
 import ansible_mitogen.connection
 
 
 class Connection(ansible_mitogen.connection.Connection):
-    transport = 'lxc'
+    transport = 'machinectl'
```

### Comparing `mitogen-0.3.3/ansible_mitogen/plugins/connection/mitogen_buildah.py` & `mitogen-0.3.4/ansible_mitogen/plugins/connection/mitogen_buildah.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.3/ansible_mitogen/plugins/connection/mitogen_podman.py` & `mitogen-0.3.4/ansible_mitogen/plugins/connection/mitogen_podman.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.3/ansible_mitogen/plugins/connection/mitogen_machinectl.py` & `mitogen-0.3.4/ansible_mitogen/plugins/connection/mitogen_docker.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,18 +29,25 @@
 from __future__ import absolute_import, division, print_function
 __metaclass__ = type
 
 import os.path
 import sys
 
 try:
-    import ansible_mitogen.connection
+    import ansible_mitogen
 except ImportError:
     base_dir = os.path.dirname(__file__)
     sys.path.insert(0, os.path.abspath(os.path.join(base_dir, '../../..')))
     del base_dir
 
 import ansible_mitogen.connection
 
 
 class Connection(ansible_mitogen.connection.Connection):
-    transport = 'machinectl'
+    transport = 'docker'
+
+    @property
+    def docker_cmd(self):
+        """
+        Ansible 2.3 synchronize module wants to know how we run Docker.
+        """
+        return 'docker'
```

### Comparing `mitogen-0.3.3/ansible_mitogen/plugins/connection/mitogen_docker.py` & `mitogen-0.3.4/ansible_mitogen/plugins/strategy/mitogen.py`

 * *Files 19% similar despite different names*

```diff
@@ -28,26 +28,36 @@
 
 from __future__ import absolute_import, division, print_function
 __metaclass__ = type
 
 import os.path
 import sys
 
-try:
-    import ansible_mitogen
-except ImportError:
-    base_dir = os.path.dirname(__file__)
-    sys.path.insert(0, os.path.abspath(os.path.join(base_dir, '../../..')))
-    del base_dir
-
-import ansible_mitogen.connection
-
-
-class Connection(ansible_mitogen.connection.Connection):
-    transport = 'docker'
-
-    @property
-    def docker_cmd(self):
-        """
-        Ansible 2.3 synchronize module wants to know how we run Docker.
-        """
-        return 'docker'
+#
+# This is not the real Strategy implementation module, it simply exists as a
+# proxy to the real module, which is loaded using Python's regular import
+# mechanism, to prevent Ansible's PluginLoader from making up a fake name that
+# results in ansible_mitogen plugin modules being loaded twice: once by
+# PluginLoader with a name like "ansible.plugins.strategy.mitogen", which is
+# stuffed into sys.modules even though attempting to import it will trigger an
+# ImportError, and once under its canonical name, "ansible_mitogen.strategy".
+#
+# Therefore we have a proxy module that imports it under the real name, and
+# sets up the duff PluginLoader-imported module to just contain objects from
+# the real module, so duplicate types don't exist in memory, and things like
+# debuggers and isinstance() work predictably.
+#
+
+BASE_DIR = os.path.abspath(
+    os.path.join(os.path.dirname(__file__), '../../..')
+)
+
+if BASE_DIR not in sys.path:
+    sys.path.insert(0, BASE_DIR)
+
+import ansible_mitogen.strategy
+import ansible.plugins.strategy.linear
+
+
+class StrategyModule(ansible_mitogen.strategy.StrategyMixin,
+                     ansible.plugins.strategy.linear.StrategyModule):
+    pass
```

### Comparing `mitogen-0.3.3/ansible_mitogen/plugins/action/mitogen_fetch.py` & `mitogen-0.3.4/ansible_mitogen/plugins/action/mitogen_fetch.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.3/ansible_mitogen/plugins/action/mitogen_get_stack.py` & `mitogen-0.3.4/ansible_mitogen/plugins/action/mitogen_get_stack.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.3/ansible_mitogen/plugins/strategy/mitogen_host_pinned.py` & `mitogen-0.3.4/ansible_mitogen/plugins/strategy/mitogen_host_pinned.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.3/ansible_mitogen/plugins/strategy/mitogen.py` & `mitogen-0.3.4/ansible_mitogen/plugins/strategy/mitogen_linear.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 BASE_DIR = os.path.abspath(
     os.path.join(os.path.dirname(__file__), '../../..')
 )
 
 if BASE_DIR not in sys.path:
     sys.path.insert(0, BASE_DIR)
 
+import ansible_mitogen.loaders
 import ansible_mitogen.strategy
-import ansible.plugins.strategy.linear
 
 
-class StrategyModule(ansible_mitogen.strategy.StrategyMixin,
-                     ansible.plugins.strategy.linear.StrategyModule):
+Base = ansible_mitogen.loaders.strategy_loader.get('linear', class_only=True)
+
+class StrategyModule(ansible_mitogen.strategy.StrategyMixin, Base):
     pass
```

### Comparing `mitogen-0.3.3/ansible_mitogen/plugins/strategy/mitogen_free.py` & `mitogen-0.3.4/ansible_mitogen/plugins/strategy/mitogen_free.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.3/ansible_mitogen/plugins/strategy/mitogen_linear.py` & `mitogen-0.3.4/ansible_mitogen/plugins/connection/mitogen_ssh.py`

 * *Files 25% similar despite different names*

```diff
@@ -28,37 +28,60 @@
 
 from __future__ import absolute_import, division, print_function
 __metaclass__ = type
 
 import os.path
 import sys
 
-#
-# This is not the real Strategy implementation module, it simply exists as a
-# proxy to the real module, which is loaded using Python's regular import
-# mechanism, to prevent Ansible's PluginLoader from making up a fake name that
-# results in ansible_mitogen plugin modules being loaded twice: once by
-# PluginLoader with a name like "ansible.plugins.strategy.mitogen", which is
-# stuffed into sys.modules even though attempting to import it will trigger an
-# ImportError, and once under its canonical name, "ansible_mitogen.strategy".
-#
-# Therefore we have a proxy module that imports it under the real name, and
-# sets up the duff PluginLoader-imported module to just contain objects from
-# the real module, so duplicate types don't exist in memory, and things like
-# debuggers and isinstance() work predictably.
-#
-
-BASE_DIR = os.path.abspath(
-    os.path.join(os.path.dirname(__file__), '../../..')
-)
-
-if BASE_DIR not in sys.path:
-    sys.path.insert(0, BASE_DIR)
+DOCUMENTATION = """
+    author: David Wilson <dw@botanicus.net>
+    connection: mitogen_ssh
+    short_description: Connect over SSH via Mitogen
+    description:
+        - This connects using an OpenSSH client controlled by the Mitogen for
+          Ansible extension. It accepts every option the vanilla ssh plugin
+          accepts.
+    version_added: "2.5"
+    options:
+        ssh_args:
+            type: str
+            vars:
+                - name: ssh_args
+                - name: ansible_ssh_args
+                - name: ansible_mitogen_ssh_args
+        ssh_common_args:
+            type: str
+            vars:
+                - name: ssh_args
+                - name: ansible_ssh_common_args
+                - name: ansible_mitogen_ssh_common_args
+        ssh_extra_args:
+            type: str
+            vars:
+                - name: ssh_args
+                - name: ansible_ssh_extra_args
+                - name: ansible_mitogen_ssh_extra_args
+"""
+
+try:
+    import ansible_mitogen
+except ImportError:
+    base_dir = os.path.dirname(__file__)
+    sys.path.insert(0, os.path.abspath(os.path.join(base_dir, '../../..')))
+    del base_dir
 
+import ansible_mitogen.connection
 import ansible_mitogen.loaders
-import ansible_mitogen.strategy
-
 
-Base = ansible_mitogen.loaders.strategy_loader.get('linear', class_only=True)
 
-class StrategyModule(ansible_mitogen.strategy.StrategyMixin, Base):
-    pass
+class Connection(ansible_mitogen.connection.Connection):
+    transport = 'ssh'
+    vanilla_class = ansible_mitogen.loaders.connection_loader__get(
+        'ssh',
+        class_only=True,
+    )
+
+    @staticmethod
+    def _create_control_path(*args, **kwargs):
+        """Forward _create_control_path() to the implementation in ssh.py."""
+        # https://github.com/dw/mitogen/issues/342
+        return Connection.vanilla_class._create_control_path(*args, **kwargs)
```

### Comparing `mitogen-0.3.3/ansible_mitogen/loaders.py` & `mitogen-0.3.4/ansible_mitogen/loaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,24 +35,25 @@
 
 import ansible.errors
 
 import ansible_mitogen.utils
 
 __all__ = [
     'action_loader',
+    'become_loader',
     'connection_loader',
     'module_loader',
     'module_utils_loader',
     'shell_loader',
     'strategy_loader',
 ]
 
 
 ANSIBLE_VERSION_MIN = (2, 10)
-ANSIBLE_VERSION_MAX = (2, 12)
+ANSIBLE_VERSION_MAX = (2, 13)
 
 NEW_VERSION_MSG = (
     "Your Ansible version (%s) is too recent. The most recent version\n"
     "supported by Mitogen for Ansible is %s.x. Please check the Mitogen\n"
     "release notes to see if a new version is available, otherwise\n"
     "subscribe to the corresponding GitHub issue to be notified when\n"
     "support becomes available.\n"
@@ -86,14 +87,15 @@
 # this is the first file our strategy plugins import, so we need to check this here
 # in prior Ansible versions, connection_loader.get_with_context didn't exist, so if a user
 # is trying to load an old Ansible version, we'll fail and error gracefully
 assert_supported_release()
 
 
 from ansible.plugins.loader import action_loader
+from ansible.plugins.loader import become_loader
 from ansible.plugins.loader import connection_loader
 from ansible.plugins.loader import module_loader
 from ansible.plugins.loader import module_utils_loader
 from ansible.plugins.loader import shell_loader
 from ansible.plugins.loader import strategy_loader
 
 # These are original, unwrapped implementations
```

### Comparing `mitogen-0.3.3/ansible_mitogen/affinity.py` & `mitogen-0.3.4/ansible_mitogen/affinity.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.3/ansible_mitogen/strategy.py` & `mitogen-0.3.4/ansible_mitogen/strategy.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.3/ansible_mitogen/module_finder.py` & `mitogen-0.3.4/ansible_mitogen/module_finder.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.3/ansible_mitogen/transport_config.py` & `mitogen-0.3.4/ansible_mitogen/transport_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,15 @@
     discover_interpreter = lambda action,interpreter_name,discovery_mode,task_vars: '/usr/bin/python'
 
 try:
     from ansible.utils.unsafe_proxy import AnsibleUnsafeText
 except ImportError:
     from ansible.vars.unsafe_proxy import AnsibleUnsafeText
 
+import ansible_mitogen.loaders
 import mitogen.core
 
 
 def run_interpreter_discovery_if_necessary(s, task_vars, action, rediscover_python):
     """
     Triggers ansible python interpreter discovery if requested.
     Caches this value the same way Ansible does it.
@@ -431,15 +432,18 @@
     def become_method(self):
         return self._play_context.become_method
 
     def become_user(self):
         return self._play_context.become_user
 
     def become_pass(self):
-        return optional_secret(self._play_context.become_pass)
+        become_method = self.become_method()
+        become_plugin = ansible_mitogen.loaders.become_loader.get(become_method)
+        become_pass = become_plugin.get_option('become_pass', hostvars=self._task_vars)
+        return optional_secret(become_pass)
 
     def password(self):
         return optional_secret(self._play_context.password)
 
     def port(self):
         return self._play_context.port
 
@@ -648,16 +652,16 @@
         )
 
     def become_user(self):
         return self._become_user
 
     def become_pass(self):
         return optional_secret(
-            self._host_vars.get('ansible_become_password') or
-            self._host_vars.get('ansible_become_pass')
+            self._host_vars.get('ansible_become_pass') or
+            self._host_vars.get('ansible_become_password')
         )
 
     def password(self):
         return optional_secret(
             self._host_vars.get('ansible_ssh_pass') or
             self._host_vars.get('ansible_password')
         )
@@ -745,15 +749,15 @@
     def mitogen_docker_path(self):
         return self._host_vars.get('mitogen_docker_path')
 
     def mitogen_kubectl_path(self):
         return self._host_vars.get('mitogen_kubectl_path')
 
     def mitogen_lxc_path(self):
-        return self.host_vars.get('mitogen_lxc_path')
+        return self._host_vars.get('mitogen_lxc_path')
 
     def mitogen_lxc_attach_path(self):
         return self._host_vars.get('mitogen_lxc_attach_path')
 
     def mitogen_lxc_info_path(self):
         return self._host_vars.get('mitogen_lxc_info_path')
```

### Comparing `mitogen-0.3.3/ansible_mitogen/connection.py` & `mitogen-0.3.4/ansible_mitogen/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -480,14 +480,15 @@
     context = None
 
     #: Context for the login account on the target. This is always the login
     #: account, even when become=True.
     login_context = None
 
     #: Only sudo, su, and doas are supported for now.
+    # Ansible ConnectionBase attribute, removed in Ansible >= 2.8
     become_methods = ['sudo', 'su', 'doas']
 
     #: Dict containing init_child() return value as recorded at startup by
     #: ContextService. Contains:
     #:
     #:  fork_context:   Context connected to the fork parent : process in the
     #:                  target account.
@@ -517,23 +518,14 @@
     #: to change the working directory to that of the current playbook,
     #: matching vanilla Ansible behaviour.
     loader_basedir = None
 
     # set by `_get_task_vars()` for interpreter discovery
     _action = None
 
-    def __del__(self):
-        """
-        Ansible cannot be trusted to always call close() e.g. the synchronize
-        action constructs a local connection like this. So provide a destructor
-        in the hopes of catching these cases.
-        """
-        # https://github.com/dw/mitogen/issues/140
-        self.close()
-
     def on_action_run(self, task_vars, delegate_to_hostname, loader_basedir):
         """
         Invoked by ActionModuleMixin to indicate a new task is about to start
         executing. We use the opportunity to grab relevant bits from the
         task-specific data.
 
         :param dict task_vars:
@@ -680,14 +672,17 @@
         establishment, file transfer, ..) for our desired target.
         """
         assert self.binding is not None
         return self.binding
 
     @property
     def connected(self):
+        """
+        Ansible connection plugin property. Used by ansible-connection command.
+        """
         return self.context is not None
 
     def _spec_from_via(self, proxied_inventory_name, via_spec):
         """
         Produce a dict connection specifiction given a string `via_spec`, of
         the form `[[become_method:]become_user@]inventory_hostname`.
         """
@@ -838,15 +833,19 @@
         constructing a mitogen.master.Router to communicate with the master,
         and a mitogen.parent.Context to represent it.
 
         Depending on the original transport we should emulate, trigger one of
         the _connect_*() service calls defined above to cause the master
         process to establish the real connection on our behalf, or return a
         reference to the existing one.
+
+        Ansible connection plugin method.
         """
+        # In some Ansible connection plugins this method returns self.
+        # However nothing I've found uses it, it's not even assigned.
         if self.connected:
             return
 
         inventory_name, stack = self._build_stack()
         worker_model = ansible_mitogen.process.get_worker_model()
         self.binding = worker_model.get_binding(
             mitogen.utils.cast(inventory_name)
@@ -876,14 +875,16 @@
         self.chain = None
 
     def close(self):
         """
         Arrange for the mitogen.master.Router running in the worker to
         gracefully shut down, and wait for shutdown to complete. Safe to call
         multiple times.
+
+        Ansible connection plugin method.
         """
         self._put_connection()
         if self.binding:
             self.binding.close()
             self.binding = None
 
     reset_compat_msg = (
@@ -892,14 +893,16 @@
 
     def reset(self):
         """
         Explicitly terminate the connection to the remote host. This discards
         any local state we hold for the connection, returns the Connection to
         the 'disconnected' state, and informs ContextService the connection is
         bad somehow, and should be shut down and discarded.
+
+        Ansible connection plugin method.
         """
         if self._play_context.remote_addr is None:
             # <2.5.6 incorrectly populate PlayContext for reset_connection
             # https://github.com/ansible/ansible/issues/27520
             raise ansible.errors.AnsibleConnectionFailure(
                 self.reset_compat_msg
             )
@@ -998,14 +1001,16 @@
 
         :param str cmd:
             Shell command to execute.
         :param bytes in_data:
             Data to supply on ``stdin`` of the process.
         :returns:
             (return code, stdout bytes, stderr bytes)
+
+        Ansible connection plugin method.
         """
         emulate_tty = (not in_data and sudoable)
         rc, stdout, stderr = self.get_chain().call(
             ansible_mitogen.target.exec_command,
             cmd=mitogen.utils.cast(cmd),
             in_data=mitogen.utils.cast(in_data),
             chdir=mitogen_chdir or self.get_default_cwd(),
@@ -1023,14 +1028,16 @@
         Implement fetch_file() by calling the corresponding
         ansible_mitogen.target function in the target.
 
         :param str in_path:
             Remote filesystem path to read.
         :param str out_path:
             Local filesystem path to write.
+
+        Ansible connection plugin method.
         """
         self._connect()
         ansible_mitogen.target.transfer_file(
             context=self.context,
             # in_path may be AnsibleUnicode
             in_path=mitogen.utils.cast(in_path),
             out_path=out_path
@@ -1072,14 +1079,16 @@
         Implement put_file() by streamily transferring the file via
         FileService.
 
         :param str in_path:
             Local filesystem path to read.
         :param str out_path:
             Remote filesystem path to write.
+
+        Ansible connection plugin method.
         """
         try:
             st = os.stat(in_path)
         except OSError as e:
             self._throw_io_error(e, in_path)
             raise
```

### Comparing `mitogen-0.3.3/ansible_mitogen/target.py` & `mitogen-0.3.4/ansible_mitogen/target.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 """
 
 from __future__ import absolute_import, division, print_function
 __metaclass__ = type
 
 import errno
 import grp
+import json
 import operator
 import os
 import pwd
 import re
 import signal
 import stat
 import subprocess
@@ -55,19 +56,14 @@
 
 import mitogen.core
 import mitogen.parent
 import mitogen.service
 from mitogen.core import b
 
 try:
-    import json
-except ImportError:
-    import simplejson as json
-
-try:
     reduce
 except NameError:
     # Python 3.x.
     from functools import reduce
 
 try:
     BaseException
@@ -367,19 +363,14 @@
     """
     # Copying the master's log level causes log messages to be filtered before
     # they reach LogForwarder, thus reducing an influx of tiny messges waking
     # the connection multiplexer process in the master.
     LOG.setLevel(log_level)
     logging.getLogger('ansible_mitogen').setLevel(log_level)
 
-    # issue #536: if the json module is available, remove simplejson from the
-    # importer whitelist to avoid confusing certain Ansible modules.
-    if json.__name__ == 'json':
-        econtext.importer.whitelist.remove('simplejson')
-
     global _fork_parent
     if FORK_SUPPORTED:
         mitogen.parent.upgrade_router(econtext)
         _fork_parent = econtext.router.fork()
 
     global good_temp_dir
     good_temp_dir = find_good_temp_dir(candidate_temp_dirs)
```

### Comparing `mitogen-0.3.3/ansible_mitogen/process.py` & `mitogen-0.3.4/ansible_mitogen/process.py`

 * *Files 4% similar despite different names*

```diff
@@ -176,58 +176,21 @@
     pool.add(mitogen.service.FileService(router=pool.router))
     pool.add(mitogen.service.PushFileService(router=pool.router))
     pool.add(ansible_mitogen.services.ContextService(router=pool.router))
     pool.add(ansible_mitogen.services.ModuleDepService(pool.router))
     LOG.debug('Service pool configured: size=%d', pool.size)
 
 
-def _setup_simplejson(responder):
-    """
-    We support serving simplejson for Python 2.4 targets on Ansible 2.3, at
-    least so the package's own CI Docker scripts can run without external
-    help, however newer versions of simplejson no longer support Python
-    2.4. Therefore override any installed/loaded version with a
-    2.4-compatible version we ship in the compat/ directory.
-    """
-    responder.whitelist_prefix('simplejson')
-
-    # issue #536: must be at end of sys.path, in case existing newer
-    # version is already loaded.
-    compat_path = os.path.join(os.path.dirname(__file__), 'compat')
-    sys.path.append(compat_path)
-
-    for fullname, is_pkg, suffix in (
-        (u'simplejson', True, '__init__.py'),
-        (u'simplejson.decoder', False, 'decoder.py'),
-        (u'simplejson.encoder', False, 'encoder.py'),
-        (u'simplejson.scanner', False, 'scanner.py'),
-    ):
-        path = os.path.join(compat_path, 'simplejson', suffix)
-        fp = open(path, 'rb')
-        try:
-            source = fp.read()
-        finally:
-            fp.close()
-
-        responder.add_source_override(
-            fullname=fullname,
-            path=path,
-            source=source,
-            is_pkg=is_pkg,
-        )
-
-
 def _setup_responder(responder):
     """
     Configure :class:`mitogen.master.ModuleResponder` to only permit
     certain packages, and to generate custom responses for certain modules.
     """
     responder.whitelist_prefix('ansible')
     responder.whitelist_prefix('ansible_mitogen')
-    _setup_simplejson(responder)
 
     # Ansible 2.3 is compatible with Python 2.4 targets, however
     # ansible/__init__.py is not. Instead, executor/module_common.py writes
     # out a 2.4-compatible namespace package for unknown reasons. So we
     # copy it here.
     responder.add_source_override(
         fullname='ansible',
```

### Comparing `mitogen-0.3.3/setup.py` & `mitogen-0.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.3/mitogen/service.py` & `mitogen-0.3.4/mitogen/service.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.3/mitogen/compat/pkgutil.py` & `mitogen-0.3.4/mitogen/compat/pkgutil.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.3/mitogen/compat/tokenize.py` & `mitogen-0.3.4/mitogen/compat/tokenize.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.3/mitogen/unix.py` & `mitogen-0.3.4/mitogen/unix.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.3/mitogen/lxc.py` & `mitogen-0.3.4/mitogen/lxc.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.3/mitogen/minify.py` & `mitogen-0.3.4/mitogen/minify.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.3/mitogen/sudo.py` & `mitogen-0.3.4/mitogen/sudo.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.3/mitogen/podman.py` & `mitogen-0.3.4/mitogen/podman.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.3/mitogen/fork.py` & `mitogen-0.3.4/mitogen/fork.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.3/mitogen/buildah.py` & `mitogen-0.3.4/mitogen/buildah.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.3/mitogen/parent.py` & `mitogen-0.3.4/mitogen/parent.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.3/mitogen/__init__.py` & `mitogen-0.3.4/mitogen/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 """
 On the Mitogen master, this is imported from ``mitogen/__init__.py`` as would
 be expected. On the slave, it is built dynamically during startup.
 """
 
 
 #: Library version as a tuple.
-__version__ = (0, 3, 3)
+__version__ = (0, 3, 4)
 
 
 #: This is :data:`False` in slave contexts. Previously it was used to prevent
 #: re-execution of :mod:`__main__` in single file programs, however that now
 #: happens automatically.
 is_master = True
```

### Comparing `mitogen-0.3.3/mitogen/core.py` & `mitogen-0.3.4/mitogen/core.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.3/mitogen/jail.py` & `mitogen-0.3.4/mitogen/jail.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.3/mitogen/doas.py` & `mitogen-0.3.4/mitogen/doas.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.3/mitogen/su.py` & `mitogen-0.3.4/mitogen/su.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.3/mitogen/docker.py` & `mitogen-0.3.4/mitogen/docker.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.3/mitogen/os_fork.py` & `mitogen-0.3.4/mitogen/os_fork.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.3/mitogen/setns.py` & `mitogen-0.3.4/mitogen/setns.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.3/mitogen/master.py` & `mitogen-0.3.4/mitogen/master.py`

 * *Files 0% similar despite different names*

```diff
@@ -532,15 +532,15 @@
         if not loader:
             LOG.debug('%r: find_loader(%r) returned %r, aborting',
                       self, fullname, loader)
             return
 
         try:
             path = loader.get_filename(fullname)
-        except (AttributeError, ImportError):
+        except (AttributeError, ImportError, ValueError):
             # - get_filename() may throw ImportError if pkgutil.find_loader()
             #   picks a "parent" package's loader for some crap that's been
             #   stuffed in sys.modules, for example in the case of urllib3:
             #       "loader for urllib3.contrib.pyopenssl cannot handle
             #        requests.packages.urllib3.contrib.pyopenssl"
             e = sys.exc_info()[1]
             LOG.debug('%r: %r.get_file_name(%r) failed: %r', self, loader, fullname, e)
```

### Comparing `mitogen-0.3.3/mitogen/utils.py` & `mitogen-0.3.4/mitogen/utils.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.3/mitogen/debug.py` & `mitogen-0.3.4/mitogen/debug.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.3/mitogen/ssh.py` & `mitogen-0.3.4/mitogen/ssh.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.3/mitogen/select.py` & `mitogen-0.3.4/mitogen/select.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.3/mitogen/fakessh.py` & `mitogen-0.3.4/mitogen/fakessh.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.3/mitogen/profiler.py` & `mitogen-0.3.4/mitogen/profiler.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.3/mitogen/lxd.py` & `mitogen-0.3.4/mitogen/lxd.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.3/mitogen/kubectl.py` & `mitogen-0.3.4/mitogen/kubectl.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.3/mitogen.egg-info/PKG-INFO` & `mitogen-0.3.4/mitogen.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,14 @@
 Metadata-Version: 2.1
 Name: mitogen
-Version: 0.3.3
+Version: 0.3.4
 Summary: Library for writing distributed self-replicating programs.
 Home-page: https://github.com/mitogen-hq/mitogen/
 Author: David Wilson
 License: New BSD
-Description: # Mitogen
-        
-        <a href="https://mitogen.networkgenomics.com/">Please see the documentation</a>.
-        
-        ![](https://i.imgur.com/eBM6LhJ.gif)
-        
-        [![Total alerts](https://img.shields.io/lgtm/alerts/g/mitogen-hq/mitogen.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/mitogen-hq/mitogen/alerts/)
-        
-        [![Build Status](https://dev.azure.com/mitogen-hq/mitogen/_apis/build/status/mitogen-hq.mitogen?branchName=master)](https://dev.azure.com/mitogen-hq/mitogen/_build/latest?definitionId=1&branchName=master)
-        
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Framework :: Ansible
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
@@ -31,7 +20,18 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: System :: Distributed Computing
 Classifier: Topic :: System :: Systems Administration
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Mitogen
+
+<a href="https://mitogen.networkgenomics.com/">Please see the documentation</a>.
+
+![](https://i.imgur.com/eBM6LhJ.gif)
+
+[![Total alerts](https://img.shields.io/lgtm/alerts/g/mitogen-hq/mitogen.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/mitogen-hq/mitogen/alerts/)
+
+[![Build Status](https://dev.azure.com/mitogen-hq/mitogen/_apis/build/status/mitogen-hq.mitogen?branchName=master)](https://dev.azure.com/mitogen-hq/mitogen/_build/latest?definitionId=1&branchName=master)
```

#### html2text {}

```diff
@@ -1,23 +1,22 @@
-Metadata-Version: 2.1 Name: mitogen Version: 0.3.3 Summary: Library for writing
+Metadata-Version: 2.1 Name: mitogen Version: 0.3.4 Summary: Library for writing
 distributed self-replicating programs. Home-page: https://github.com/mitogen-
-hq/mitogen/ Author: David Wilson License: New BSD Description: # Mitogen Please
-see_the_documentation. ![](https://i.imgur.com/eBM6LhJ.gif) [![Total alerts]
-(https://img.shields.io/lgtm/alerts/g/mitogen-hq/
-mitogen.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/mitogen-hq/
-mitogen/alerts/) [![Build Status](https://dev.azure.com/mitogen-hq/mitogen/
-_apis/build/status/mitogen-hq.mitogen?branchName=master)](https://
-dev.azure.com/mitogen-hq/mitogen/_build/
-latest?definitionId=1&branchName=master) Platform: UNKNOWN Classifier:
-Environment :: Console Classifier: Framework :: Ansible Classifier: Intended
-Audience :: System Administrators Classifier: License :: OSI Approved :: BSD
-License Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating
-System :: POSIX Classifier: Programming Language :: Python Classifier:
-Programming Language :: Python :: 2.7 Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.6 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: Implementation :: CPython Classifier: Topic :: System :: Distributed
-Computing Classifier: Topic :: System :: Systems Administration Requires-
-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
-Description-Content-Type: text/markdown
+hq/mitogen/ Author: David Wilson License: New BSD Classifier: Environment ::
+Console Classifier: Framework :: Ansible Classifier: Intended Audience ::
+System Administrators Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
+:: POSIX Classifier: Programming Language :: Python Classifier: Programming
+Language :: Python :: 2.7 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python ::
+Implementation :: CPython Classifier: Topic :: System :: Distributed Computing
+Classifier: Topic :: System :: Systems Administration Requires-Python: >=2.7,
+!=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.* Description-Content-Type:
+text/markdown License-File: LICENSE # Mitogen Please_see_the_documentation. ![]
+(https://i.imgur.com/eBM6LhJ.gif) [![Total alerts](https://img.shields.io/lgtm/
+alerts/g/mitogen-hq/mitogen.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/
+projects/g/mitogen-hq/mitogen/alerts/) [![Build Status](https://dev.azure.com/
+mitogen-hq/mitogen/_apis/build/status/mitogen-hq.mitogen?branchName=master)]
+(https://dev.azure.com/mitogen-hq/mitogen/_build/
+latest?definitionId=1&branchName=master)
```

### Comparing `mitogen-0.3.3/mitogen.egg-info/SOURCES.txt` & `mitogen-0.3.4/mitogen.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -16,18 +16,14 @@
 ansible_mitogen/runner.py
 ansible_mitogen/services.py
 ansible_mitogen/strategy.py
 ansible_mitogen/target.py
 ansible_mitogen/transport_config.py
 ansible_mitogen/utils.py
 ansible_mitogen/compat/__init__.py
-ansible_mitogen/compat/simplejson/__init__.py
-ansible_mitogen/compat/simplejson/decoder.py
-ansible_mitogen/compat/simplejson/encoder.py
-ansible_mitogen/compat/simplejson/scanner.py
 ansible_mitogen/plugins/__init__.py
 ansible_mitogen/plugins/action/__init__.py
 ansible_mitogen/plugins/action/mitogen_fetch.py
 ansible_mitogen/plugins/action/mitogen_get_stack.py
 ansible_mitogen/plugins/connection/__init__.py
 ansible_mitogen/plugins/connection/mitogen_buildah.py
 ansible_mitogen/plugins/connection/mitogen_doas.py
@@ -77,9 +73,9 @@
 mitogen.egg-info/PKG-INFO
 mitogen.egg-info/SOURCES.txt
 mitogen.egg-info/dependency_links.txt
 mitogen.egg-info/not-zip-safe
 mitogen.egg-info/top_level.txt
 mitogen/compat/__init__.py
 mitogen/compat/pkgutil.py
-mitogen/compat/shutil.py
-mitogen/compat/tokenize.py
+mitogen/compat/tokenize.py
+tests/testlib.py
```

