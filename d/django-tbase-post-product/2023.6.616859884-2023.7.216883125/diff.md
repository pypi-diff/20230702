# Comparing `tmp/django_tbase_post_product-2023.6.616859884.tar.gz` & `tmp/django_tbase_post_product-2023.7.216883125.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tbase_post_product-2023.6.616859884.tar", last modified: Mon Jun  5 18:07:07 2023, max compression
+gzip compressed data, was "django_tbase_post_product-2023.7.216883125.tar", last modified: Sun Jul  2 15:42:14 2023, max compression
```

## Comparing `django_tbase_post_product-2023.6.616859884.tar` & `django_tbase_post_product-2023.7.216883125.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-05 18:07:07.556922 django_tbase_post_product-2023.6.616859884/
--rw-r--r--   0 terry     (1000) terry     (1000)      143 2023-05-20 17:05:28.000000 django_tbase_post_product-2023.6.616859884/MANIFEST.in
--rw-r--r--   0 terry     (1000) terry     (1000)     1544 2023-06-05 18:07:07.556922 django_tbase_post_product-2023.6.616859884/PKG-INFO
--rw-r--r--   0 terry     (1000) terry     (1000)     1222 2023-06-05 15:40:41.000000 django_tbase_post_product-2023.6.616859884/README.md
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-05 18:07:07.546922 django_tbase_post_product-2023.6.616859884/django_tbase_post_product.egg-info/
--rw-r--r--   0 terry     (1000) terry     (1000)     1544 2023-06-05 18:07:07.000000 django_tbase_post_product-2023.6.616859884/django_tbase_post_product.egg-info/PKG-INFO
--rw-r--r--   0 terry     (1000) terry     (1000)     1689 2023-06-05 18:07:07.000000 django_tbase_post_product-2023.6.616859884/django_tbase_post_product.egg-info/SOURCES.txt
--rw-r--r--   0 terry     (1000) terry     (1000)        1 2023-06-05 18:07:07.000000 django_tbase_post_product-2023.6.616859884/django_tbase_post_product.egg-info/dependency_links.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       83 2023-06-05 18:07:07.000000 django_tbase_post_product-2023.6.616859884/django_tbase_post_product.egg-info/requires.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       11 2023-06-05 18:07:07.000000 django_tbase_post_product-2023.6.616859884/django_tbase_post_product.egg-info/top_level.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       38 2023-06-05 18:07:07.556922 django_tbase_post_product-2023.6.616859884/setup.cfg
--rw-r--r--   0 terry     (1000) terry     (1000)     2305 2023-05-26 20:53:14.000000 django_tbase_post_product-2023.6.616859884/setup.py
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-05 18:07:07.556922 django_tbase_post_product-2023.6.616859884/tbase_post/
--rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.6.616859884/tbase_post/__init__.py
--rw-r--r--   0 terry     (1000) terry     (1000)     1727 2023-05-15 18:15:03.000000 django_tbase_post_product-2023.6.616859884/tbase_post/admin.py
--rw-r--r--   0 terry     (1000) terry     (1000)      146 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.6.616859884/tbase_post/apps.py
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-05 18:07:07.556922 django_tbase_post_product-2023.6.616859884/tbase_post/migrations/
--rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.6.616859884/tbase_post/migrations/__init__.py
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-05 18:07:07.556922 django_tbase_post_product-2023.6.616859884/tbase_post/migrations/__pycache__/
--rw-r--r--   0 terry     (1000) terry     (1000)     1062 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.6.616859884/tbase_post/migrations/__pycache__/0001_initial.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     1092 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.6.616859884/tbase_post/migrations/__pycache__/0002_auto_20230421_1307.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     1081 2023-05-05 14:25:13.000000 django_tbase_post_product-2023.6.616859884/tbase_post/migrations/__pycache__/0003_auto_20230505_1424.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     1498 2023-05-05 15:03:52.000000 django_tbase_post_product-2023.6.616859884/tbase_post/migrations/__pycache__/0004_auto_20230505_1503.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)      591 2023-05-05 15:05:58.000000 django_tbase_post_product-2023.6.616859884/tbase_post/migrations/__pycache__/0005_rename_banner_img_post_article_img.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     1059 2023-05-05 15:46:35.000000 django_tbase_post_product-2023.6.616859884/tbase_post/migrations/__pycache__/0006_auto_20230505_1546.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)      168 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.6.616859884/tbase_post/migrations/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     3388 2023-05-05 15:46:17.000000 django_tbase_post_product-2023.6.616859884/tbase_post/models.py
--rw-r--r--   0 terry     (1000) terry     (1000)      479 2023-05-12 18:21:31.000000 django_tbase_post_product-2023.6.616859884/tbase_post/sitemaps.py
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-05 18:07:07.546922 django_tbase_post_product-2023.6.616859884/tbase_post/static/
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-05 18:07:07.556922 django_tbase_post_product-2023.6.616859884/tbase_post/static/images/
--rw-r--r--   0 terry     (1000) terry     (1000)    59619 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.6.616859884/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg
--rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.6.616859884/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg:Zone.Identifier
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-05 18:07:07.556922 django_tbase_post_product-2023.6.616859884/tbase_post/templates/
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-05 18:07:07.556922 django_tbase_post_product-2023.6.616859884/tbase_post/templates/post/
--rw-r--r--   0 terry     (1000) terry     (1000)     3626 2023-06-05 17:51:37.000000 django_tbase_post_product-2023.6.616859884/tbase_post/templates/post/article_list_by_tag.html
--rw-r--r--   0 terry     (1000) terry     (1000)     2116 2023-06-05 15:38:41.000000 django_tbase_post_product-2023.6.616859884/tbase_post/templates/post/blog_index.html
--rw-r--r--   0 terry     (1000) terry     (1000)     5001 2023-06-05 16:20:34.000000 django_tbase_post_product-2023.6.616859884/tbase_post/templates/post/detail.html
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-05 18:07:07.556922 django_tbase_post_product-2023.6.616859884/tbase_post/templates/post/extras/
--rw-r--r--   0 terry     (1000) terry     (1000)      511 2023-06-05 16:10:39.000000 django_tbase_post_product-2023.6.616859884/tbase_post/templates/post/extras/amazon_link.html
--rw-r--r--   0 terry     (1000) terry     (1000)      374 2023-06-05 14:30:33.000000 django_tbase_post_product-2023.6.616859884/tbase_post/templates/post/extras/last_update.html
--rw-r--r--   0 terry     (1000) terry     (1000)      288 2023-06-05 14:30:33.000000 django_tbase_post_product-2023.6.616859884/tbase_post/templates/post/extras/related_post_by_tags.html
--rw-r--r--   0 terry     (1000) terry     (1000)      505 2023-06-05 15:36:14.000000 django_tbase_post_product-2023.6.616859884/tbase_post/templates/post/extras/tags.html
--rw-r--r--   0 terry     (1000) terry     (1000)      391 2023-05-05 16:55:19.000000 django_tbase_post_product-2023.6.616859884/tbase_post/templates/sitemap.xml
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-05 18:07:07.556922 django_tbase_post_product-2023.6.616859884/tbase_post/templatetags/
--rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.6.616859884/tbase_post/templatetags/__init__.py
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-05 18:07:07.556922 django_tbase_post_product-2023.6.616859884/tbase_post/templatetags/__pycache__/
--rw-r--r--   0 terry     (1000) terry     (1000)      170 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.6.616859884/tbase_post/templatetags/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     3002 2023-05-11 17:20:31.000000 django_tbase_post_product-2023.6.616859884/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     5447 2023-06-05 18:06:08.000000 django_tbase_post_product-2023.6.616859884/tbase_post/templatetags/post_extras.py
--rw-r--r--   0 terry     (1000) terry     (1000)       60 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.6.616859884/tbase_post/tests.py
--rw-r--r--   0 terry     (1000) terry     (1000)      725 2023-05-05 16:36:02.000000 django_tbase_post_product-2023.6.616859884/tbase_post/urls.py
--rw-r--r--   0 terry     (1000) terry     (1000)     3823 2023-06-02 08:57:44.000000 django_tbase_post_product-2023.6.616859884/tbase_post/views.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-02 15:42:14.950796 django_tbase_post_product-2023.7.216883125/
+-rw-r--r--   0 terry     (1000) terry     (1000)      143 2023-05-20 17:05:28.000000 django_tbase_post_product-2023.7.216883125/MANIFEST.in
+-rw-r--r--   0 terry     (1000) terry     (1000)     1544 2023-07-02 15:42:14.950796 django_tbase_post_product-2023.7.216883125/PKG-INFO
+-rw-r--r--   0 terry     (1000) terry     (1000)     1222 2023-06-05 15:40:41.000000 django_tbase_post_product-2023.7.216883125/README.md
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-02 15:42:14.950796 django_tbase_post_product-2023.7.216883125/django_tbase_post_product.egg-info/
+-rw-r--r--   0 terry     (1000) terry     (1000)     1544 2023-07-02 15:42:14.000000 django_tbase_post_product-2023.7.216883125/django_tbase_post_product.egg-info/PKG-INFO
+-rw-r--r--   0 terry     (1000) terry     (1000)     1689 2023-07-02 15:42:14.000000 django_tbase_post_product-2023.7.216883125/django_tbase_post_product.egg-info/SOURCES.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)        1 2023-07-02 15:42:14.000000 django_tbase_post_product-2023.7.216883125/django_tbase_post_product.egg-info/dependency_links.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       83 2023-07-02 15:42:14.000000 django_tbase_post_product-2023.7.216883125/django_tbase_post_product.egg-info/requires.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       11 2023-07-02 15:42:14.000000 django_tbase_post_product-2023.7.216883125/django_tbase_post_product.egg-info/top_level.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       38 2023-07-02 15:42:14.950796 django_tbase_post_product-2023.7.216883125/setup.cfg
+-rw-r--r--   0 terry     (1000) terry     (1000)     2305 2023-05-26 20:53:14.000000 django_tbase_post_product-2023.7.216883125/setup.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-02 15:42:14.950796 django_tbase_post_product-2023.7.216883125/tbase_post/
+-rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.7.216883125/tbase_post/__init__.py
+-rw-r--r--   0 terry     (1000) terry     (1000)     1727 2023-05-15 18:15:03.000000 django_tbase_post_product-2023.7.216883125/tbase_post/admin.py
+-rw-r--r--   0 terry     (1000) terry     (1000)      146 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.7.216883125/tbase_post/apps.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-02 15:42:14.950796 django_tbase_post_product-2023.7.216883125/tbase_post/migrations/
+-rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.7.216883125/tbase_post/migrations/__init__.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-02 15:42:14.950796 django_tbase_post_product-2023.7.216883125/tbase_post/migrations/__pycache__/
+-rw-r--r--   0 terry     (1000) terry     (1000)     1062 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.7.216883125/tbase_post/migrations/__pycache__/0001_initial.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     1092 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.7.216883125/tbase_post/migrations/__pycache__/0002_auto_20230421_1307.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     1081 2023-05-05 14:25:13.000000 django_tbase_post_product-2023.7.216883125/tbase_post/migrations/__pycache__/0003_auto_20230505_1424.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     1498 2023-05-05 15:03:52.000000 django_tbase_post_product-2023.7.216883125/tbase_post/migrations/__pycache__/0004_auto_20230505_1503.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)      591 2023-05-05 15:05:58.000000 django_tbase_post_product-2023.7.216883125/tbase_post/migrations/__pycache__/0005_rename_banner_img_post_article_img.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     1059 2023-05-05 15:46:35.000000 django_tbase_post_product-2023.7.216883125/tbase_post/migrations/__pycache__/0006_auto_20230505_1546.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)      168 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.7.216883125/tbase_post/migrations/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     4035 2023-06-30 11:20:55.000000 django_tbase_post_product-2023.7.216883125/tbase_post/models.py
+-rw-r--r--   0 terry     (1000) terry     (1000)      479 2023-05-12 18:21:31.000000 django_tbase_post_product-2023.7.216883125/tbase_post/sitemaps.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-02 15:42:14.940796 django_tbase_post_product-2023.7.216883125/tbase_post/static/
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-02 15:42:14.950796 django_tbase_post_product-2023.7.216883125/tbase_post/static/images/
+-rw-r--r--   0 terry     (1000) terry     (1000)    59619 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.7.216883125/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg
+-rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.7.216883125/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg:Zone.Identifier
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-02 15:42:14.950796 django_tbase_post_product-2023.7.216883125/tbase_post/templates/
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-02 15:42:14.950796 django_tbase_post_product-2023.7.216883125/tbase_post/templates/post/
+-rw-r--r--   0 terry     (1000) terry     (1000)     3672 2023-07-02 15:35:07.000000 django_tbase_post_product-2023.7.216883125/tbase_post/templates/post/article_list_by_tag.html
+-rw-r--r--   0 terry     (1000) terry     (1000)     2127 2023-07-02 15:36:36.000000 django_tbase_post_product-2023.7.216883125/tbase_post/templates/post/blog_index.html
+-rw-r--r--   0 terry     (1000) terry     (1000)     5170 2023-07-02 15:39:11.000000 django_tbase_post_product-2023.7.216883125/tbase_post/templates/post/detail.html
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-02 15:42:14.950796 django_tbase_post_product-2023.7.216883125/tbase_post/templates/post/extras/
+-rw-r--r--   0 terry     (1000) terry     (1000)      583 2023-07-02 15:28:54.000000 django_tbase_post_product-2023.7.216883125/tbase_post/templates/post/extras/amazon_link.html
+-rw-r--r--   0 terry     (1000) terry     (1000)      443 2023-07-02 14:56:34.000000 django_tbase_post_product-2023.7.216883125/tbase_post/templates/post/extras/last_update.html
+-rw-r--r--   0 terry     (1000) terry     (1000)      366 2023-07-02 15:28:37.000000 django_tbase_post_product-2023.7.216883125/tbase_post/templates/post/extras/related_post_by_tags.html
+-rw-r--r--   0 terry     (1000) terry     (1000)      569 2023-07-02 15:24:36.000000 django_tbase_post_product-2023.7.216883125/tbase_post/templates/post/extras/tags.html
+-rw-r--r--   0 terry     (1000) terry     (1000)      391 2023-05-05 16:55:19.000000 django_tbase_post_product-2023.7.216883125/tbase_post/templates/sitemap.xml
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-02 15:42:14.950796 django_tbase_post_product-2023.7.216883125/tbase_post/templatetags/
+-rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.7.216883125/tbase_post/templatetags/__init__.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-02 15:42:14.950796 django_tbase_post_product-2023.7.216883125/tbase_post/templatetags/__pycache__/
+-rw-r--r--   0 terry     (1000) terry     (1000)      170 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.7.216883125/tbase_post/templatetags/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     3002 2023-05-11 17:20:31.000000 django_tbase_post_product-2023.7.216883125/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     5503 2023-07-02 14:31:57.000000 django_tbase_post_product-2023.7.216883125/tbase_post/templatetags/post_extras.py
+-rw-r--r--   0 terry     (1000) terry     (1000)       60 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.7.216883125/tbase_post/tests.py
+-rw-r--r--   0 terry     (1000) terry     (1000)      841 2023-07-02 14:42:11.000000 django_tbase_post_product-2023.7.216883125/tbase_post/urls.py
+-rw-r--r--   0 terry     (1000) terry     (1000)     4014 2023-07-02 14:40:15.000000 django_tbase_post_product-2023.7.216883125/tbase_post/views.py
```

### Comparing `django_tbase_post_product-2023.6.616859884/PKG-INFO` & `django_tbase_post_product-2023.7.216883125/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_tbase_post_product
-Version: 2023.6.616859884
+Version: 2023.7.216883125
 Summary: Terry django base post ,
 Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_post_product/files/README.md
 Author: Terry Chan
 Author-email: napoler2008@gmail.com
 Description-Content-Type: text/markdown
 
 # django-expand/tbase_post_product
```

### Comparing `django_tbase_post_product-2023.6.616859884/README.md` & `django_tbase_post_product-2023.7.216883125/README.md`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.6.616859884/django_tbase_post_product.egg-info/PKG-INFO` & `django_tbase_post_product-2023.7.216883125/django_tbase_post_product.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-tbase-post-product
-Version: 2023.6.616859884
+Version: 2023.7.216883125
 Summary: Terry django base post ,
 Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_post_product/files/README.md
 Author: Terry Chan
 Author-email: napoler2008@gmail.com
 Description-Content-Type: text/markdown
 
 # django-expand/tbase_post_product
```

### Comparing `django_tbase_post_product-2023.6.616859884/django_tbase_post_product.egg-info/SOURCES.txt` & `django_tbase_post_product-2023.7.216883125/django_tbase_post_product.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.6.616859884/setup.py` & `django_tbase_post_product-2023.7.216883125/setup.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.6.616859884/tbase_post/admin.py` & `django_tbase_post_product-2023.7.216883125/tbase_post/admin.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.6.616859884/tbase_post/migrations/__pycache__/0001_initial.cpython-310.pyc` & `django_tbase_post_product-2023.7.216883125/tbase_post/migrations/__pycache__/0001_initial.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.6.616859884/tbase_post/migrations/__pycache__/0002_auto_20230421_1307.cpython-310.pyc` & `django_tbase_post_product-2023.7.216883125/tbase_post/migrations/__pycache__/0002_auto_20230421_1307.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.6.616859884/tbase_post/migrations/__pycache__/0003_auto_20230505_1424.cpython-310.pyc` & `django_tbase_post_product-2023.7.216883125/tbase_post/migrations/__pycache__/0003_auto_20230505_1424.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.6.616859884/tbase_post/migrations/__pycache__/0004_auto_20230505_1503.cpython-310.pyc` & `django_tbase_post_product-2023.7.216883125/tbase_post/migrations/__pycache__/0004_auto_20230505_1503.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.6.616859884/tbase_post/migrations/__pycache__/0005_rename_banner_img_post_article_img.cpython-310.pyc` & `django_tbase_post_product-2023.7.216883125/tbase_post/migrations/__pycache__/0005_rename_banner_img_post_article_img.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.6.616859884/tbase_post/migrations/__pycache__/0006_auto_20230505_1546.cpython-310.pyc` & `django_tbase_post_product-2023.7.216883125/tbase_post/migrations/__pycache__/0006_auto_20230505_1546.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.6.616859884/tbase_post/models.py` & `django_tbase_post_product-2023.7.216883125/tbase_post/models.py`

 * *Files 15% similar despite different names*

```diff
@@ -50,14 +50,29 @@
                            """
                            )
     
     # author = models.TextField()
     # text = MarkdownField(rendered_field='text_rendered', use_editor=False, use_admin_editor=True,validator=VALIDATOR_STANDARD)
     # text_rendered = RenderedMarkdownField(default='')
     tags = TaggableManager("标签")
+    meta_keywords = models.CharField("meta keywords",
+                           max_length=128,
+                           blank=True,
+                           help_text="""
+                            关键词,用于搜索引擎优化使用,关键词使用英文逗号分割
+                           """
+                           )
+    meta_description = models.CharField("meta description",
+                           max_length=255,
+                           blank=True,
+                           help_text="""
+                            用于搜索引擎优化使用
+                           """
+                           )
+    
     def get_absolute_url(self):
         return reverse('detail_view', args=[self.pk])
 
     def __str__(self):
         return self.title
 
     def save(self, *args, **kwargs):
```

### Comparing `django_tbase_post_product-2023.6.616859884/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg` & `django_tbase_post_product-2023.7.216883125/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.6.616859884/tbase_post/templates/post/article_list_by_tag.html` & `django_tbase_post_product-2023.7.216883125/tbase_post/templates/post/article_list_by_tag.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 {% extends 'blog/blog.html' %}
 {% load static %}
 {% comment %} {% extends 'base.html' %} {% endcomment %}
-
+{% load cache %}
 {% load post_extras %}
 {% block title %}<title>{{title}}</title>{% endblock %}
 
 
 {% block top_nav %}
 
 {% endblock %}
@@ -32,30 +32,33 @@
                      <img alt="{{detail.product_name}}" title="{{detail.title}}" src="{{detail.article_img}}">
                  </p>
                 </div>
                 {%endif%}
                 <div class="bg-white flex flex-col justify-start p-6">
                     <a href="{% url 'detail_view' detail.pk %}" class="text-3xl font-bold hover:text-gray-700 pb-4">{{detail.title}}</a>
                     <p  class="text-sm pb-3">
-                        By <a href="#" class="font-semibold hover:text-gray-800">David Grzyb</a>, Published on {{detail.created_on}}
+                       Published on {{detail.created_on}}
                     </p>
 
                     <p class="pb-6">
-                        {% comment %} 限制文本长度 {% endcomment %}
-                          {{detail.content|truncatechars:128}}
+                        {% cache 36000 content_truncatechars 128 object.pk %}  
+                        {{detail.content|truncatechars:128}}
+                        {% endcache %}
                     </p>
-{% tags detail.tags%}
 
+    {% cache 36000 tags object.pk %}
+{% tags detail.tags 5 detail.pk %}
+{% endcache %}
                     <a href="{% url 'detail_view' detail.pk %}" class="uppercase text-gray-800 hover:text-black">Continue Reading {{detail.product_name}}<i class="fas fa-arrow-right"></i></a>
                 </div>
             </article>
 
  {% endfor %}
 
-
+ 
 
 
 
 
 
 {% comment %}
 
@@ -93,17 +96,19 @@
     <!-- about_us -->
     <div class="w-full bg-white shadow flex flex-col my-4 p-6">
         <!-- <p class="text-xl font-semibold pb-5">About Us</p>
         <p class="pb-2">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas mattis est eu odio sagittis tristique. Vestibulum ut finibus leo. In hac habitasse platea dictumst.</p>
         <a href="#" class="w-full bg-blue-800 text-white font-bold text-sm uppercase rounded hover:bg-blue-700 flex items-center justify-center px-2 py-3 mt-4">
             Get to know us
         </a> -->
-        {% last_update 10 %}
+    
 
-        
+ 
+    {% last_update 10 %}
+ 
     </div>
    {% endblock %}
     <div class="w-full bg-white shadow flex flex-col my-4 p-6">
 
     </div>
     <!-- sidebar_section endblock -->
    {% endblock %}
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,21 +1,23 @@
 {% extends 'blog/blog.html' %} {% load static %} {% comment %} {% extends
-'base.html' %} {% endcomment %} {% load post_extras %} {% block title %}
+'base.html' %} {% endcomment %} {% load cache %} {% load post_extras %} {%
+block title %}
 {% endblock %} {% block top_nav %} {% endblock %} {% block head %} {% if
 meta.noindex %}
  {% endif %} {% endblock %} {% block body_class_expand %}tag{% endblock %} {%
 block article_list %} {% for detail in object_list %}   {%if
 detail.article_img%}
 [{{detail.product_name}}]
 {%endif%}
 {{detail.title}}
-By David_Grzyb, Published on {{detail.created_on}}
-{% comment %} éå¶ææ¬é¿åº¦ {% endcomment %} {
-{detail.content|truncatechars:128}}
-{% tags detail.tags%}
+Published on {{detail.created_on}}
+{% cache 36000 content_truncatechars 128 object.pk %} {
+{detail.content|truncatechars:128}} {% endcache %}
+{% cache 36000 tags object.pk %} {% tags detail.tags 5 detail.pk %} {% endcache
+%}
 Continue_Reading_{{detail.product_name}}
  {% endfor %} {% comment %}
  {% if page_obj.has_previous %} «_first previous {% endif %}  Page {
 { page_obj.number }} of {{ page_obj.paginator.num_pages }}.  {% if
 page_obj.has_next %} next last_» {% endif %}
 {% endcomment %} {% endblock %} {% block sidebar_section %}  {% block about_us
 %}
```

### Comparing `django_tbase_post_product-2023.6.616859884/tbase_post/templates/post/blog_index.html` & `django_tbase_post_product-2023.7.216883125/tbase_post/templates/post/blog_index.html`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
                         <p class="pb-6">
                             {% comment %} 限制文本长度 {% endcomment %}
                             {{detail.content|truncatechars:128}}
                             <a href="{% url 'detail_view' detail.pk %}" class="uppercase text-gray-800 hover:text-black">Continue Reading {{detail.product_name}}<i class="fas fa-arrow-right"></i></a>
   
                         </p>
-    {% tags detail.tags%}
+  {% tags detail.tags 5 detail.pk %}
     </div>
     </article>
     {% endfor %}
      <!--object_list end-->
 
 {% endblock %}
 {% comment %} article_list end {% endcomment %}
```

#### html2text {}

```diff
@@ -8,9 +8,9 @@
 {%endif%}
 {{detail.title|truncatechars:48}}
 {% comment %} By David_Grzyb, {% endcomment %} Published on {
 {detail.created_on}}
 {% comment %} éå¶ææ¬é¿åº¦ {% endcomment %} {
 {detail.content|truncatechars:128}}
 Continue_Reading_{{detail.product_name}}
-{% tags detail.tags%}
+{% tags detail.tags 5 detail.pk %}
  {% endfor %}  {% endblock %} {% comment %} article_list end {% endcomment %}
```

### Comparing `django_tbase_post_product-2023.6.616859884/tbase_post/templates/post/detail.html` & `django_tbase_post_product-2023.7.216883125/tbase_post/templates/post/detail.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 {% extends 'blog/post.html' %}
 {% comment %} 加载区 {% endcomment %}
 {% load static %}
 {% comment %} {% extends 'base.html' %} {% endcomment %}
 {% load martortags %}
 {% load post_extras %}
 {% load solo_tags %}
-
+{% load cache %}
 
 {% comment %} 加载区 结束 {% endcomment %}
 
 
  {% block tailwind_css %}
 <style type="text/tailwindcss">
     @layer utilities {
@@ -50,16 +50,16 @@
 {% endblock %}
 
 {% block title %}<title>{{detail.title}} : {{title}}</title>{% endblock %}
 
 
 {% block head %}
 {% tag_names object.tags 4 as tag%}
-<meta name="description" content="{{detail.content|truncatechars:128}}">
-<meta name="keywords" content="{{detail.product_name}},{{ tag.names_text}}">
+<meta name="description" content="{{detail.description|truncatechars:128}}">
+<meta name="keywords" content="{{detail.product_name}},{{ detail.meta_keywords}}">
 {% if meta.noindex %} 
 <meta name="robots" content="noindex">
 {% endif %} 
 <!-- <meta name="author" content="Terry"> -->
 
 {% endblock %}
 
@@ -130,29 +130,35 @@
                 </div>
       
      
 
 
           </div>
           
-      
-
-        <!--标签-->
-        {% tags object.tags%}
-        <!--标签结束-->
-
+{% cache 36000 tags object.pk %}
+<!--标签-->
+{% tags object.tags 5 object.pk %}
+<!--标签结束-->
+{% endcache %}
     </div>
 
 <!--相关内容-->
 <div class="w-full flex pt-6">
 <div class="w-1/2 bg-white text-left p-6">
+
+ {% cache 36000 related_post_by_tags object.pk %}
 {% related_post_by_tags object.tags 10 object.pk %}
+{% endcache %}
+
 </div>
 <div class="w-1/2 bg-white text-left p-6">
-{% last_update 10 %}
+{% cache 500 last_update %}
+    {% last_update 10 %}
+{% endcache %}
+
     </div>
 </div>
 <!--相关内容结束-->
 
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 {% extends 'blog/post.html' %} {% comment %} å è½½åº {% endcomment %} {% load
 static %} {% comment %} {% extends 'base.html' %} {% endcomment %} {% load
-martortags %} {% load post_extras %} {% load solo_tags %} {% comment %}
-å è½½åº ç»æ {% endcomment %} {% block tailwind_css %}
+martortags %} {% load post_extras %} {% load solo_tags %} {% load cache %} {%
+comment %} å è½½åº ç»æ {% endcomment %} {% block tailwind_css %}
  {% endblock %} {% block title %}
 {% endblock %} {% block head %} {% tag_names object.tags 4 as tag%}
 
  {% if meta.noindex %}
  {% endif %}  {% endblock %} {% block top_header %} {% endblock %} {% block
 top_nav %} {% endblock %} {% block body_class_expand %}detail{% endblock %} {%
 block text_header %} {% endblock %} {% block article_img %} {%if
@@ -18,16 +18,18 @@
 {% comment %} By David_Grzyb, {% endcomment %} Published on {
 {detail.created_on}}
 {% comment %} {{detail.content}} {% endcomment %}  {
 { detail.content|safe_markdown }}
 [{{detail.product_name}}]
  {% get_solo 'tbase_post.AmazonSettings' as amazon %} {% amazon_link
 object.product_id detail.product_name amazon.store_id %}
- {% tags object.tags%}
-{% related_post_by_tags object.tags 10 object.pk %}
-{% last_update 10 %}
+{% cache 36000 tags object.pk %}  {% tags object.tags 5 object.pk %}  {%
+endcache %}
+{% cache 36000 related_post_by_tags object.pk %} {% related_post_by_tags
+object.tags 10 object.pk %} {% endcache %}
+{% cache 500 last_update %} {% last_update 10 %} {% endcache %}
  {% endblock %}  {% block article_previous_next %} {% if
 detail.get_previous_by_created_on %}
  {{detail.get_previous_by_created_on.title}}
  {%endif%} {% if detail.get_next_by_created_on %}
 {{detail.get_next_by_created_on.title}}
  {%endif%} {% endblock %}   {% block article_author %} {% endblock %}
```

### Comparing `django_tbase_post_product-2023.6.616859884/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc` & `django_tbase_post_product-2023.7.216883125/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.6.616859884/tbase_post/templatetags/post_extras.py` & `django_tbase_post_product-2023.7.216883125/tbase_post/templatetags/post_extras.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from django import template
 from tbase_post.models import Post
 from pprint import pprint as pp
 from django.db.models import F
 from django.db.models import Count
+from django.views.decorators.cache import cache_control
 register = template.Library()
 
 
 
 # 创建信息
 # https://docs.djangoproject.com/zh-hans/4.2/howto/custom-template-tags/
```

### Comparing `django_tbase_post_product-2023.6.616859884/tbase_post/urls.py` & `django_tbase_post_product-2023.7.216883125/tbase_post/urls.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from django.urls import path
 from django.contrib.sitemaps.views import sitemap
+from django.views.decorators.cache import cache_page
 from .sitemaps import PostSitemap
 from . import views
 sitemaps = {
     'posts': PostSitemap,
 }
 urlpatterns = [
-    path('', views.IndexView.as_view(), name='detail_index'),
-    path('detail/<int:pk>/', views.DetailView.as_view(), name='detail_view'),
+    path('', cache_page(60 * 15)(views.IndexView.as_view()), name='detail_index'),
+    path('detail/<int:pk>/', cache_page(60 * 15)(views.DetailView.as_view()), name='detail_view'),
     path('tag/<int:pk>/',
-         views.TagListView.as_view(),
+         cache_page(60 * 60)(views.TagListView.as_view()),
          name='article_list_by_tag'),
     path('sitemap.xml', 
          sitemap, 
          {'sitemaps': sitemaps}, 
          name='django.contrib.sitemaps.views.sitemap'),  # 网站地图 
     # path('detail/<int:pk>', views.DetailView.as_view(), name='post_view'),
     # path('<int:pk>/', views.PostView.as_view(), name='post'),
```

### Comparing `django_tbase_post_product-2023.6.616859884/tbase_post/views.py` & `django_tbase_post_product-2023.7.216883125/tbase_post/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,27 +4,29 @@
 # Create your views here.
 from django.http import HttpResponse, Http404
 
 from taggit.models import TaggedItem
 from taggit.models import Tag
 from django.views.generic.base import TemplateView
 from django.views import generic
+from django.views.decorators.cache import cache_page
+# from django.core.cache import caches
 from . import models
 # class DetailView(TemplateView):
 
 #     # def get(self, request, pk, *args, **kwargs):
 #     #     return HttpResponse(f'Hello, World!{pk}')
 #     template_name = "detail.html"
 
 #     def get_context_data(self, **kwargs):
 #         context = super().get_context_data(**kwargs)
 #         context['latest_articles'] = Article.objects.all()[:5]
 #         return context
 
-
+# @cache_page(60*2)
 class DetailView(generic.DetailView):
     template_name = 'post/detail.html'
     # context_object_name = 'post'
     # def get(request, pk):
     #     """Return the last five published questions."""
     #     return Post.objects.get(id=pk)
     model = models.Post
@@ -40,21 +42,20 @@
     #     # context['now'] = timezone.now()
     #     return context
 
     def get_context_data(self, *args, **kwargs):
         # print("kwargs",kwargs)
         # context = Post.objects.get(id=pk)
         context = super().get_context_data(**kwargs)
-
         # context['now'] = timezone.now()
         # context['title'] = "Post Details"
         # print(context)
         return context
 
-
+# @cache_page(60*2)
 class IndexView(generic.ListView):
 
     # def get(self, request, *args, **kwargs):
     #     return HttpResponse('Hello, World! index')
 
     template_name = 'post/blog_index.html'
     model = models.Post
@@ -71,15 +72,15 @@
         # context = Post.objects.get(id=pk)
         context = super().get_context_data(**kwargs)
         # context['now'] = timezone.now()
         # context['title'] = "Post Details"
         # print(context)
         return context
 
-
+# @cache_page(60*60)
 class TagListView(generic.ListView):
     model = models.Post
     template_name = 'post/article_list_by_tag.html'
     context_object_name = 'posts'
     paginate_by = 20
     ordering = ['-created_on']
     def get_queryset(self):
@@ -99,14 +100,15 @@
 
         """
         context = super().get_context_data(**kwargs)
         # 获取tag的标签
         tag_slug = self.kwargs['pk']
         tag = Tag.objects.get(pk=tag_slug)
         context['title'] = tag
+        context['pk'] = self.kwargs['pk']
         # print("context", context)
    
         if len(context['object_list'])<10:
             print("No")
             context['meta'] = {
             'noindex':True
             }
```

