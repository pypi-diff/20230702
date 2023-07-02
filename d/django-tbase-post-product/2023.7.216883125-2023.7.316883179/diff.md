# Comparing `tmp/django_tbase_post_product-2023.7.216883125.tar.gz` & `tmp/django_tbase_post_product-2023.7.316883179.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tbase_post_product-2023.7.216883125.tar", last modified: Sun Jul  2 15:42:14 2023, max compression
+gzip compressed data, was "django_tbase_post_product-2023.7.316883179.tar", last modified: Sun Jul  2 17:12:15 2023, max compression
```

## Comparing `django_tbase_post_product-2023.7.216883125.tar` & `django_tbase_post_product-2023.7.316883179.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-02 15:42:14.950796 django_tbase_post_product-2023.7.216883125/
--rw-r--r--   0 terry     (1000) terry     (1000)      143 2023-05-20 17:05:28.000000 django_tbase_post_product-2023.7.216883125/MANIFEST.in
--rw-r--r--   0 terry     (1000) terry     (1000)     1544 2023-07-02 15:42:14.950796 django_tbase_post_product-2023.7.216883125/PKG-INFO
--rw-r--r--   0 terry     (1000) terry     (1000)     1222 2023-06-05 15:40:41.000000 django_tbase_post_product-2023.7.216883125/README.md
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-02 15:42:14.950796 django_tbase_post_product-2023.7.216883125/django_tbase_post_product.egg-info/
--rw-r--r--   0 terry     (1000) terry     (1000)     1544 2023-07-02 15:42:14.000000 django_tbase_post_product-2023.7.216883125/django_tbase_post_product.egg-info/PKG-INFO
--rw-r--r--   0 terry     (1000) terry     (1000)     1689 2023-07-02 15:42:14.000000 django_tbase_post_product-2023.7.216883125/django_tbase_post_product.egg-info/SOURCES.txt
--rw-r--r--   0 terry     (1000) terry     (1000)        1 2023-07-02 15:42:14.000000 django_tbase_post_product-2023.7.216883125/django_tbase_post_product.egg-info/dependency_links.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       83 2023-07-02 15:42:14.000000 django_tbase_post_product-2023.7.216883125/django_tbase_post_product.egg-info/requires.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       11 2023-07-02 15:42:14.000000 django_tbase_post_product-2023.7.216883125/django_tbase_post_product.egg-info/top_level.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       38 2023-07-02 15:42:14.950796 django_tbase_post_product-2023.7.216883125/setup.cfg
--rw-r--r--   0 terry     (1000) terry     (1000)     2305 2023-05-26 20:53:14.000000 django_tbase_post_product-2023.7.216883125/setup.py
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-02 15:42:14.950796 django_tbase_post_product-2023.7.216883125/tbase_post/
--rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.7.216883125/tbase_post/__init__.py
--rw-r--r--   0 terry     (1000) terry     (1000)     1727 2023-05-15 18:15:03.000000 django_tbase_post_product-2023.7.216883125/tbase_post/admin.py
--rw-r--r--   0 terry     (1000) terry     (1000)      146 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.7.216883125/tbase_post/apps.py
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-02 15:42:14.950796 django_tbase_post_product-2023.7.216883125/tbase_post/migrations/
--rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.7.216883125/tbase_post/migrations/__init__.py
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-02 15:42:14.950796 django_tbase_post_product-2023.7.216883125/tbase_post/migrations/__pycache__/
--rw-r--r--   0 terry     (1000) terry     (1000)     1062 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.7.216883125/tbase_post/migrations/__pycache__/0001_initial.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     1092 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.7.216883125/tbase_post/migrations/__pycache__/0002_auto_20230421_1307.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     1081 2023-05-05 14:25:13.000000 django_tbase_post_product-2023.7.216883125/tbase_post/migrations/__pycache__/0003_auto_20230505_1424.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     1498 2023-05-05 15:03:52.000000 django_tbase_post_product-2023.7.216883125/tbase_post/migrations/__pycache__/0004_auto_20230505_1503.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)      591 2023-05-05 15:05:58.000000 django_tbase_post_product-2023.7.216883125/tbase_post/migrations/__pycache__/0005_rename_banner_img_post_article_img.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     1059 2023-05-05 15:46:35.000000 django_tbase_post_product-2023.7.216883125/tbase_post/migrations/__pycache__/0006_auto_20230505_1546.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)      168 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.7.216883125/tbase_post/migrations/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     4035 2023-06-30 11:20:55.000000 django_tbase_post_product-2023.7.216883125/tbase_post/models.py
--rw-r--r--   0 terry     (1000) terry     (1000)      479 2023-05-12 18:21:31.000000 django_tbase_post_product-2023.7.216883125/tbase_post/sitemaps.py
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-02 15:42:14.940796 django_tbase_post_product-2023.7.216883125/tbase_post/static/
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-02 15:42:14.950796 django_tbase_post_product-2023.7.216883125/tbase_post/static/images/
--rw-r--r--   0 terry     (1000) terry     (1000)    59619 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.7.216883125/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg
--rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.7.216883125/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg:Zone.Identifier
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-02 15:42:14.950796 django_tbase_post_product-2023.7.216883125/tbase_post/templates/
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-02 15:42:14.950796 django_tbase_post_product-2023.7.216883125/tbase_post/templates/post/
--rw-r--r--   0 terry     (1000) terry     (1000)     3672 2023-07-02 15:35:07.000000 django_tbase_post_product-2023.7.216883125/tbase_post/templates/post/article_list_by_tag.html
--rw-r--r--   0 terry     (1000) terry     (1000)     2127 2023-07-02 15:36:36.000000 django_tbase_post_product-2023.7.216883125/tbase_post/templates/post/blog_index.html
--rw-r--r--   0 terry     (1000) terry     (1000)     5170 2023-07-02 15:39:11.000000 django_tbase_post_product-2023.7.216883125/tbase_post/templates/post/detail.html
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-02 15:42:14.950796 django_tbase_post_product-2023.7.216883125/tbase_post/templates/post/extras/
--rw-r--r--   0 terry     (1000) terry     (1000)      583 2023-07-02 15:28:54.000000 django_tbase_post_product-2023.7.216883125/tbase_post/templates/post/extras/amazon_link.html
--rw-r--r--   0 terry     (1000) terry     (1000)      443 2023-07-02 14:56:34.000000 django_tbase_post_product-2023.7.216883125/tbase_post/templates/post/extras/last_update.html
--rw-r--r--   0 terry     (1000) terry     (1000)      366 2023-07-02 15:28:37.000000 django_tbase_post_product-2023.7.216883125/tbase_post/templates/post/extras/related_post_by_tags.html
--rw-r--r--   0 terry     (1000) terry     (1000)      569 2023-07-02 15:24:36.000000 django_tbase_post_product-2023.7.216883125/tbase_post/templates/post/extras/tags.html
--rw-r--r--   0 terry     (1000) terry     (1000)      391 2023-05-05 16:55:19.000000 django_tbase_post_product-2023.7.216883125/tbase_post/templates/sitemap.xml
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-02 15:42:14.950796 django_tbase_post_product-2023.7.216883125/tbase_post/templatetags/
--rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.7.216883125/tbase_post/templatetags/__init__.py
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-02 15:42:14.950796 django_tbase_post_product-2023.7.216883125/tbase_post/templatetags/__pycache__/
--rw-r--r--   0 terry     (1000) terry     (1000)      170 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.7.216883125/tbase_post/templatetags/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     3002 2023-05-11 17:20:31.000000 django_tbase_post_product-2023.7.216883125/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     5503 2023-07-02 14:31:57.000000 django_tbase_post_product-2023.7.216883125/tbase_post/templatetags/post_extras.py
--rw-r--r--   0 terry     (1000) terry     (1000)       60 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.7.216883125/tbase_post/tests.py
--rw-r--r--   0 terry     (1000) terry     (1000)      841 2023-07-02 14:42:11.000000 django_tbase_post_product-2023.7.216883125/tbase_post/urls.py
--rw-r--r--   0 terry     (1000) terry     (1000)     4014 2023-07-02 14:40:15.000000 django_tbase_post_product-2023.7.216883125/tbase_post/views.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-02 17:12:14.991070 django_tbase_post_product-2023.7.316883179/
+-rw-r--r--   0 terry     (1000) terry     (1000)      143 2023-05-20 17:05:28.000000 django_tbase_post_product-2023.7.316883179/MANIFEST.in
+-rw-r--r--   0 terry     (1000) terry     (1000)     1544 2023-07-02 17:12:14.991070 django_tbase_post_product-2023.7.316883179/PKG-INFO
+-rw-r--r--   0 terry     (1000) terry     (1000)     1222 2023-06-05 15:40:41.000000 django_tbase_post_product-2023.7.316883179/README.md
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-02 17:12:14.991070 django_tbase_post_product-2023.7.316883179/django_tbase_post_product.egg-info/
+-rw-r--r--   0 terry     (1000) terry     (1000)     1544 2023-07-02 17:12:14.000000 django_tbase_post_product-2023.7.316883179/django_tbase_post_product.egg-info/PKG-INFO
+-rw-r--r--   0 terry     (1000) terry     (1000)     1689 2023-07-02 17:12:14.000000 django_tbase_post_product-2023.7.316883179/django_tbase_post_product.egg-info/SOURCES.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)        1 2023-07-02 17:12:14.000000 django_tbase_post_product-2023.7.316883179/django_tbase_post_product.egg-info/dependency_links.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       83 2023-07-02 17:12:14.000000 django_tbase_post_product-2023.7.316883179/django_tbase_post_product.egg-info/requires.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       11 2023-07-02 17:12:14.000000 django_tbase_post_product-2023.7.316883179/django_tbase_post_product.egg-info/top_level.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       38 2023-07-02 17:12:14.991070 django_tbase_post_product-2023.7.316883179/setup.cfg
+-rw-r--r--   0 terry     (1000) terry     (1000)     2305 2023-05-26 20:53:14.000000 django_tbase_post_product-2023.7.316883179/setup.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-02 17:12:14.991070 django_tbase_post_product-2023.7.316883179/tbase_post/
+-rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.7.316883179/tbase_post/__init__.py
+-rw-r--r--   0 terry     (1000) terry     (1000)     1727 2023-05-15 18:15:03.000000 django_tbase_post_product-2023.7.316883179/tbase_post/admin.py
+-rw-r--r--   0 terry     (1000) terry     (1000)      146 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.7.316883179/tbase_post/apps.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-02 17:12:14.991070 django_tbase_post_product-2023.7.316883179/tbase_post/migrations/
+-rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.7.316883179/tbase_post/migrations/__init__.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-02 17:12:14.991070 django_tbase_post_product-2023.7.316883179/tbase_post/migrations/__pycache__/
+-rw-r--r--   0 terry     (1000) terry     (1000)     1062 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.7.316883179/tbase_post/migrations/__pycache__/0001_initial.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     1092 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.7.316883179/tbase_post/migrations/__pycache__/0002_auto_20230421_1307.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     1081 2023-05-05 14:25:13.000000 django_tbase_post_product-2023.7.316883179/tbase_post/migrations/__pycache__/0003_auto_20230505_1424.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     1498 2023-05-05 15:03:52.000000 django_tbase_post_product-2023.7.316883179/tbase_post/migrations/__pycache__/0004_auto_20230505_1503.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)      591 2023-05-05 15:05:58.000000 django_tbase_post_product-2023.7.316883179/tbase_post/migrations/__pycache__/0005_rename_banner_img_post_article_img.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     1059 2023-05-05 15:46:35.000000 django_tbase_post_product-2023.7.316883179/tbase_post/migrations/__pycache__/0006_auto_20230505_1546.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)      168 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.7.316883179/tbase_post/migrations/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     4035 2023-06-30 11:20:55.000000 django_tbase_post_product-2023.7.316883179/tbase_post/models.py
+-rw-r--r--   0 terry     (1000) terry     (1000)      479 2023-05-12 18:21:31.000000 django_tbase_post_product-2023.7.316883179/tbase_post/sitemaps.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-02 17:12:14.981070 django_tbase_post_product-2023.7.316883179/tbase_post/static/
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-02 17:12:14.991070 django_tbase_post_product-2023.7.316883179/tbase_post/static/images/
+-rw-r--r--   0 terry     (1000) terry     (1000)    59619 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.7.316883179/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg
+-rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.7.316883179/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg:Zone.Identifier
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-02 17:12:14.991070 django_tbase_post_product-2023.7.316883179/tbase_post/templates/
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-02 17:12:14.991070 django_tbase_post_product-2023.7.316883179/tbase_post/templates/post/
+-rw-r--r--   0 terry     (1000) terry     (1000)     3667 2023-07-02 16:58:12.000000 django_tbase_post_product-2023.7.316883179/tbase_post/templates/post/article_list_by_tag.html
+-rw-r--r--   0 terry     (1000) terry     (1000)     2127 2023-07-02 15:36:36.000000 django_tbase_post_product-2023.7.316883179/tbase_post/templates/post/blog_index.html
+-rw-r--r--   0 terry     (1000) terry     (1000)     5170 2023-07-02 16:55:04.000000 django_tbase_post_product-2023.7.316883179/tbase_post/templates/post/detail.html
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-02 17:12:14.991070 django_tbase_post_product-2023.7.316883179/tbase_post/templates/post/extras/
+-rw-r--r--   0 terry     (1000) terry     (1000)      583 2023-07-02 15:28:54.000000 django_tbase_post_product-2023.7.316883179/tbase_post/templates/post/extras/amazon_link.html
+-rw-r--r--   0 terry     (1000) terry     (1000)      443 2023-07-02 14:56:34.000000 django_tbase_post_product-2023.7.316883179/tbase_post/templates/post/extras/last_update.html
+-rw-r--r--   0 terry     (1000) terry     (1000)      366 2023-07-02 15:28:37.000000 django_tbase_post_product-2023.7.316883179/tbase_post/templates/post/extras/related_post_by_tags.html
+-rw-r--r--   0 terry     (1000) terry     (1000)      569 2023-07-02 16:41:58.000000 django_tbase_post_product-2023.7.316883179/tbase_post/templates/post/extras/tags.html
+-rw-r--r--   0 terry     (1000) terry     (1000)      391 2023-06-30 11:21:12.000000 django_tbase_post_product-2023.7.316883179/tbase_post/templates/sitemap.xml
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-02 17:12:14.991070 django_tbase_post_product-2023.7.316883179/tbase_post/templatetags/
+-rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-06-30 11:21:12.000000 django_tbase_post_product-2023.7.316883179/tbase_post/templatetags/__init__.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-02 17:12:14.991070 django_tbase_post_product-2023.7.316883179/tbase_post/templatetags/__pycache__/
+-rw-r--r--   0 terry     (1000) terry     (1000)      176 2023-06-30 11:21:12.000000 django_tbase_post_product-2023.7.316883179/tbase_post/templatetags/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     3444 2023-07-02 16:53:59.000000 django_tbase_post_product-2023.7.316883179/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     6225 2023-07-02 16:53:58.000000 django_tbase_post_product-2023.7.316883179/tbase_post/templatetags/post_extras.py
+-rw-r--r--   0 terry     (1000) terry     (1000)       60 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.7.316883179/tbase_post/tests.py
+-rw-r--r--   0 terry     (1000) terry     (1000)      841 2023-07-02 14:42:11.000000 django_tbase_post_product-2023.7.316883179/tbase_post/urls.py
+-rw-r--r--   0 terry     (1000) terry     (1000)     4262 2023-07-02 17:03:03.000000 django_tbase_post_product-2023.7.316883179/tbase_post/views.py
```

### Comparing `django_tbase_post_product-2023.7.216883125/PKG-INFO` & `django_tbase_post_product-2023.7.316883179/django_tbase_post_product.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: django_tbase_post_product
-Version: 2023.7.216883125
+Name: django-tbase-post-product
+Version: 2023.7.316883179
 Summary: Terry django base post ,
 Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_post_product/files/README.md
 Author: Terry Chan
 Author-email: napoler2008@gmail.com
 Description-Content-Type: text/markdown
 
 # django-expand/tbase_post_product
```

### Comparing `django_tbase_post_product-2023.7.216883125/README.md` & `django_tbase_post_product-2023.7.316883179/README.md`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.7.216883125/django_tbase_post_product.egg-info/PKG-INFO` & `django_tbase_post_product-2023.7.316883179/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: django-tbase-post-product
-Version: 2023.7.216883125
+Name: django_tbase_post_product
+Version: 2023.7.316883179
 Summary: Terry django base post ,
 Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_post_product/files/README.md
 Author: Terry Chan
 Author-email: napoler2008@gmail.com
 Description-Content-Type: text/markdown
 
 # django-expand/tbase_post_product
```

### Comparing `django_tbase_post_product-2023.7.216883125/django_tbase_post_product.egg-info/SOURCES.txt` & `django_tbase_post_product-2023.7.316883179/django_tbase_post_product.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.7.216883125/setup.py` & `django_tbase_post_product-2023.7.316883179/setup.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.7.216883125/tbase_post/admin.py` & `django_tbase_post_product-2023.7.316883179/tbase_post/admin.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.7.216883125/tbase_post/migrations/__pycache__/0001_initial.cpython-310.pyc` & `django_tbase_post_product-2023.7.316883179/tbase_post/migrations/__pycache__/0001_initial.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.7.216883125/tbase_post/migrations/__pycache__/0002_auto_20230421_1307.cpython-310.pyc` & `django_tbase_post_product-2023.7.316883179/tbase_post/migrations/__pycache__/0002_auto_20230421_1307.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.7.216883125/tbase_post/migrations/__pycache__/0003_auto_20230505_1424.cpython-310.pyc` & `django_tbase_post_product-2023.7.316883179/tbase_post/migrations/__pycache__/0003_auto_20230505_1424.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.7.216883125/tbase_post/migrations/__pycache__/0004_auto_20230505_1503.cpython-310.pyc` & `django_tbase_post_product-2023.7.316883179/tbase_post/migrations/__pycache__/0004_auto_20230505_1503.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.7.216883125/tbase_post/migrations/__pycache__/0005_rename_banner_img_post_article_img.cpython-310.pyc` & `django_tbase_post_product-2023.7.316883179/tbase_post/migrations/__pycache__/0005_rename_banner_img_post_article_img.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.7.216883125/tbase_post/migrations/__pycache__/0006_auto_20230505_1546.cpython-310.pyc` & `django_tbase_post_product-2023.7.316883179/tbase_post/migrations/__pycache__/0006_auto_20230505_1546.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.7.216883125/tbase_post/models.py` & `django_tbase_post_product-2023.7.316883179/tbase_post/models.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.7.216883125/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg` & `django_tbase_post_product-2023.7.316883179/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.7.216883125/tbase_post/templates/post/article_list_by_tag.html` & `django_tbase_post_product-2023.7.316883179/tbase_post/templates/post/article_list_by_tag.html`

 * *Files 5% similar despite different names*

```diff
@@ -18,16 +18,14 @@
 
 {% endblock %}
 
 {% block body_class_expand %}tag{% endblock %}
  {% block article_list %}
 
  {% for detail in object_list %}
-
-
             <article class="w-full flex flex-col shadow my-4">
                 <!-- Article Image -->
                 {%if detail.article_img%}
                 <div class="flex items-center justify-center bg-gray-100">
                  <p class="hover:opacity-75">
                      <img alt="{{detail.product_name}}" title="{{detail.title}}" src="{{detail.article_img}}">
                  </p>
@@ -36,20 +34,21 @@
                 <div class="bg-white flex flex-col justify-start p-6">
                     <a href="{% url 'detail_view' detail.pk %}" class="text-3xl font-bold hover:text-gray-700 pb-4">{{detail.title}}</a>
                     <p  class="text-sm pb-3">
                        Published on {{detail.created_on}}
                     </p>
 
                     <p class="pb-6">
-                        {% cache 36000 content_truncatechars 128 object.pk %}  
+                        {% cache 36000 content_truncatechars_128 detail.pk %}  
                         {{detail.content|truncatechars:128}}
                         {% endcache %}
                     </p>
 
-    {% cache 36000 tags object.pk %}
+
+{% cache 36000 tags detail.pk %}
 {% tags detail.tags 5 detail.pk %}
 {% endcache %}
                     <a href="{% url 'detail_view' detail.pk %}" class="uppercase text-gray-800 hover:text-black">Continue Reading {{detail.product_name}}<i class="fas fa-arrow-right"></i></a>
                 </div>
             </article>
 
  {% endfor %}
```

#### html2text {}

```diff
@@ -6,17 +6,17 @@
  {% endif %} {% endblock %} {% block body_class_expand %}tag{% endblock %} {%
 block article_list %} {% for detail in object_list %}   {%if
 detail.article_img%}
 [{{detail.product_name}}]
 {%endif%}
 {{detail.title}}
 Published on {{detail.created_on}}
-{% cache 36000 content_truncatechars 128 object.pk %} {
+{% cache 36000 content_truncatechars_128 detail.pk %} {
 {detail.content|truncatechars:128}} {% endcache %}
-{% cache 36000 tags object.pk %} {% tags detail.tags 5 detail.pk %} {% endcache
+{% cache 36000 tags detail.pk %} {% tags detail.tags 5 detail.pk %} {% endcache
 %}
 Continue_Reading_{{detail.product_name}}
  {% endfor %} {% comment %}
  {% if page_obj.has_previous %} «_first previous {% endif %}  Page {
 { page_obj.number }} of {{ page_obj.paginator.num_pages }}.  {% if
 page_obj.has_next %} next last_» {% endif %}
 {% endcomment %} {% endblock %} {% block sidebar_section %}  {% block about_us
```

### Comparing `django_tbase_post_product-2023.7.216883125/tbase_post/templates/post/blog_index.html` & `django_tbase_post_product-2023.7.316883179/tbase_post/templates/post/blog_index.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.7.216883125/tbase_post/templates/post/detail.html` & `django_tbase_post_product-2023.7.316883179/tbase_post/templates/post/detail.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.7.216883125/tbase_post/templates/post/extras/amazon_link.html` & `django_tbase_post_product-2023.7.316883179/tbase_post/templates/post/extras/amazon_link.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.7.216883125/tbase_post/templates/post/extras/tags.html` & `django_tbase_post_product-2023.7.316883179/tbase_post/templates/post/extras/tags.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.7.216883125/tbase_post/templatetags/post_extras.py` & `django_tbase_post_product-2023.7.316883179/tbase_post/templatetags/post_extras.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from django import template
 from tbase_post.models import Post
 from pprint import pprint as pp
 from django.db.models import F
 from django.db.models import Count
 from django.views.decorators.cache import cache_control
+from django.core.cache import cache
 register = template.Library()
 
 
 
 # 创建信息
 # https://docs.djangoproject.com/zh-hans/4.2/howto/custom-template-tags/
 
@@ -39,26 +40,41 @@
     }
 
 
 def tags_with_count(tags):
     """
     将标签数量添加到每个标签对象中
     """
+    key = "-".join(list(tags.slugs()))
+    key=f'tags_with_count_{key}'
+    # print("key",key)
+    tags_with_count_dict= cache.get(key)
+    if tags_with_count_dict is not None:
+        return tags_with_count_dict
+
+
+    # if cache.get(key)
     # 查询每个标签及其数量
     # tags_with_count = tags.through.objects.values('tag__name').annotate(count=Count('tag__name'))
-    tags_with_count = tags.through.objects.values('tag__pk').annotate(count=Count('tag__pk'))
+
+    tags_with_count= cache.get('tags_with_count') 
+    if tags_with_count is None:
+        tags_with_count = tags.through.objects.values('tag__pk').annotate(count=Count('tag__pk'))
+        # print("tags_with_count",tags_with_count)
+        cache.set('tags_with_count',tags_with_count, 60*60*24)
+
     # 将标签数量添加到每个标签对象中
     # tags = [{"tag__name":tag['tag__name'], "count":tag['count']} for tag in tags_with_count]
     # print("tags", context)
     # tags_with_count
     tags_with_count_dict = {}
     for tag in tags_with_count:
         tags_with_count_dict[tag['tag__pk']]=tag['count']
     
-
+    cache.set(key,tags_with_count_dict, 60*60*24)
     return tags_with_count_dict
 
 
 # tags格式化
 @register.simple_tag(takes_context=False)
 def tag_names(tags, limit=5,*args, **kwargs):
     """
@@ -88,15 +104,15 @@
             "names_text":",".join(names)}
     pass
 
 
 # tags格式化
 @register.filter
 @register.inclusion_tag("post/extras/tags.html", takes_context=False)
-def tags(tags,limit=5, *args, **kwargs):
+def tags(tags,limit=5, pk=None,*args, **kwargs):
     # print("tags",tags)
     # tags
     # 查询每个标签及其数量
     items_with_count=tags_with_count(tags)
     items=[]
     i=0
     for item in  tags.all():
@@ -110,19 +126,21 @@
             'count':items_with_count[item.pk],
             'object':item
 
         })
         i=i+1
 
     # print("tags", context)
+    key = "-".join(list(tags.slugs()))
     return {
         "title":"Tags:",
         # "item_with_count":item_with_count,
         "items":items,
-        "tags":tags
+        "tags":tags,
+        "pk":key #pk
         }
     pass
 
 # 相关内容推荐
 # 根据tags过滤相关内容
 """
 主题模板中使用
@@ -136,14 +154,15 @@
 """
 
 @register.inclusion_tag('post/extras/related_post_by_tags.html',
                         takes_context=False)
 def related_post_by_tags(tags=[], limit=5,exclude_pk=None):
     try:
         # page_obj=tags.similar_objects()[-limit:]
+        key = "-".join(list(tags.slugs()))
         page_obj=tags.similar_objects()[:limit]
         # slugs = list(tags.slugs())
         # # print("slugs", slugs)
         # # 排除本节点，查询相关的tags
         # if exclude_pk==None:
         #     page_obj = Post.objects.filter(tags__slug__in=slugs).order_by('-pk').distinct()[:limit]
         # else:
@@ -152,14 +171,15 @@
 
         # print("page_obj", page_obj)
         return {
             'state': True,
             'link': "context['home_link']",
             'title': "Related Content",
             "page_obj": page_obj,
+            "pk":key
             # "content": context
         }
     except Exception as e:
         # print(e)
         return {
             'state': False,
             'link': "context['home_link']",
@@ -185,18 +205,20 @@
 
         # print("page_obj", page_obj)
         return {
             'state': True,
             'link': "context['home_link']",
             'title': "Last Update",
             "page_obj": page_obj,
+            "pk":"last_update"
             # "content": context
         }
     except Exception as e:
         # print(e)
         return {
             'state': False,
             'link': "context['home_link']",
             'title': "Last Update",
             "page_obj": [],
+            "pk":"last_update"
             # "content": context
         }
```

### Comparing `django_tbase_post_product-2023.7.216883125/tbase_post/urls.py` & `django_tbase_post_product-2023.7.316883179/tbase_post/urls.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.7.216883125/tbase_post/views.py` & `django_tbase_post_product-2023.7.316883179/tbase_post/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from taggit.models import TaggedItem
 from taggit.models import Tag
 from django.views.generic.base import TemplateView
 from django.views import generic
 from django.views.decorators.cache import cache_page
 # from django.core.cache import caches
+from django.core.cache import cache
 from . import models
 # class DetailView(TemplateView):
 
 #     # def get(self, request, pk, *args, **kwargs):
 #     #     return HttpResponse(f'Hello, World!{pk}')
 #     template_name = "detail.html"
 
@@ -82,32 +83,40 @@
     template_name = 'post/article_list_by_tag.html'
     context_object_name = 'posts'
     paginate_by = 20
     ordering = ['-created_on']
     def get_queryset(self):
         # retrieve the tag from the URL
         tag_slug = self.kwargs['pk']
+
+        key=f'article_tag_{tag_slug}'
+        articles=cache.get(key)
+        if articles is not None: 
+            return articles
+        
         # get the tag object based on the slug
         tag = Tag.objects.get(pk=tag_slug)
         # filter articles based on the tag
+ 
         articles = self.model.objects.filter(tags=tag)
         # if len(articles)<500:
         #     print("No articles")
             # return Http404('project list dose not exist')
+        cache.set(key,articles,60*60*25)
         return articles
 
     def get_context_data(self, *args, **kwargs):
         """
 
         """
         context = super().get_context_data(**kwargs)
         # 获取tag的标签
         tag_slug = self.kwargs['pk']
         tag = Tag.objects.get(pk=tag_slug)
-        context['title'] = tag
+        context['title'] = f"{tag}-{context['page_obj']}"
         context['pk'] = self.kwargs['pk']
         # print("context", context)
    
         if len(context['object_list'])<10:
             print("No")
             context['meta'] = {
             'noindex':True
```

