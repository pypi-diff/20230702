# Comparing `tmp/photoshop_python_api-0.8.0.tar.gz` & `tmp/photoshop_python_api-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/photoshop_python_api-0.8.0.tar", last modified: Tue Apr  7 17:11:02 2020, max compression
+gzip compressed data, was "dist/photoshop_python_api-0.9.0.tar", last modified: Wed Apr  8 17:30:04 2020, max compression
```

## Comparing `photoshop_python_api-0.8.0.tar` & `photoshop_python_api-0.9.0.tar`

### file list

```diff
@@ -1,120 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-07 17:11:02.659590 photoshop_python_api-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (116)      209 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-07 17:11:02.631590 photoshop_python_api-0.8.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-07 17:11:02.635590 photoshop_python_api-0.8.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (116)      708 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/.github/ISSUE_TEMPLATE/bug_report.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-07 17:11:02.635590 photoshop_python_api-0.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)      865 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (116)      264 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)     1166 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      195 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (116)      568 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (116)      228 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (116)       43 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1061 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     5842 2020-04-07 17:11:02.659590 photoshop_python_api-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     4018 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (116)       26 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-07 17:11:02.635590 photoshop_python_api-0.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (116)     6770 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (116)       30 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (116)     5767 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)     1107 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/docs/generate_usage.py
--rw-r--r--   0 runner    (1001) docker     (116)      233 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)      624 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (116)     6463 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-07 17:11:02.635590 photoshop_python_api-0.8.0/docs/src/
--rw-r--r--   0 runner    (1001) docker     (116)       64 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/docs/src/modules.rst
--rw-r--r--   0 runner    (1001) docker     (116)      794 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/docs/src/photoshop.colors.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1795 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/docs/src/photoshop.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1567 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/docs/src/photoshop.save_options.rst
--rw-r--r--   0 runner    (1001) docker     (116)     2571 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-07 17:11:02.647590 photoshop_python_api-0.8.0/examples/
--rw-r--r--   0 runner    (1001) docker     (116)      540 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/examples/active_layer.py
--rw-r--r--   0 runner    (1001) docker     (116)      650 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/examples/add_slate.py
--rw-r--r--   0 runner    (1001) docker     (116)     1290 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/examples/apply_crystallize_filter_action.py
--rw-r--r--   0 runner    (1001) docker     (116)     1712 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/examples/apply_filters.py
--rw-r--r--   0 runner    (1001) docker     (116)      738 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/examples/color.py
--rw-r--r--   0 runner    (1001) docker     (116)      363 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/examples/compare_colors.py
--rw-r--r--   0 runner    (1001) docker     (116)     1401 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/examples/copy_and_paste.py
--rw-r--r--   0 runner    (1001) docker     (116)      622 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/examples/create_thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (116)      214 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/examples/current_tool.py
--rw-r--r--   0 runner    (1001) docker     (116)     2340 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/examples/emboss_action.py
--rw-r--r--   0 runner    (1001) docker     (116)      252 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/examples/eval_javascript.py
--rw-r--r--   0 runner    (1001) docker     (116)  3148164 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/examples/export_layers_as_png.psd
--rw-r--r--   0 runner    (1001) docker     (116)      943 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/examples/export_layers_as_png.py
--rw-r--r--   0 runner    (1001) docker     (116)      969 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/examples/fill_selection.py
--rw-r--r--   0 runner    (1001) docker     (116)      662 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/examples/hello_world.py
--rw-r--r--   0 runner    (1001) docker     (116)  2689431 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/examples/layer_comps.psd
--rw-r--r--   0 runner    (1001) docker     (116)      578 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/examples/link_layer.py
--rw-r--r--   0 runner    (1001) docker     (116)     1236 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/examples/load_selection.py
--rw-r--r--   0 runner    (1001) docker     (116)      541 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/examples/move_to_end.py
--rw-r--r--   0 runner    (1001) docker     (116)      448 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/examples/new_document.py
--rw-r--r--   0 runner    (1001) docker     (116)      245 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/examples/open_psd.py
--rw-r--r--   0 runner    (1001) docker     (116)      717 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/examples/photoshop_session.py
--rw-r--r--   0 runner    (1001) docker     (116)      625 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/examples/rotate_layer.py
--rw-r--r--   0 runner    (1001) docker     (116)      346 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/examples/save_to_psd.py
--rw-r--r--   0 runner    (1001) docker     (116)     1642 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/examples/selection_stroke.py
--rw-r--r--   0 runner    (1001) docker     (116)      253 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/examples/session_callback.py
--rw-r--r--   0 runner    (1001) docker     (116)      169 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/examples/session_document_duplicate.py
--rw-r--r--   0 runner    (1001) docker     (116)      674 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/examples/session_hello_world.py
--rw-r--r--   0 runner    (1001) docker     (116)      177 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/examples/session_new_document.py
--rw-r--r--   0 runner    (1001) docker     (116)     1817 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/examples/session_smart_sharpen.py
--rw-r--r--   0 runner    (1001) docker     (116)      552 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/examples/set_active_layer.py
--rw-r--r--   0 runner    (1001) docker     (116)   430697 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/examples/slate_template.psd
--rw-r--r--   0 runner    (1001) docker     (116)     1616 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/examples/smart_sharpen.py
--rw-r--r--   0 runner    (1001) docker     (116)      750 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (116)       16 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       67 2020-04-07 17:11:02.659590 photoshop_python_api-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1422 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-07 17:11:02.631590 photoshop_python_api-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-07 17:11:02.655590 photoshop_python_api-0.8.0/src/photoshop/
--rw-r--r--   0 runner    (1001) docker     (116)     7120 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/src/photoshop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      170 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/src/photoshop/_active_document.py
--rw-r--r--   0 runner    (1001) docker     (116)      288 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/src/photoshop/_active_layer.py
--rw-r--r--   0 runner    (1001) docker     (116)     9593 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/src/photoshop/_artlayer.py
--rw-r--r--   0 runner    (1001) docker     (116)      970 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/src/photoshop/_artlayers.py
--rw-r--r--   0 runner    (1001) docker     (116)     4765 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/src/photoshop/_core.py
--rw-r--r--   0 runner    (1001) docker     (116)     9808 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/src/photoshop/_document.py
--rw-r--r--   0 runner    (1001) docker     (116)     1908 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/src/photoshop/_documents.py
--rw-r--r--   0 runner    (1001) docker     (116)     2767 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/src/photoshop/_layer.py
--rw-r--r--   0 runner    (1001) docker     (116)     1096 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/src/photoshop/_layerSet.py
--rw-r--r--   0 runner    (1001) docker     (116)      904 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/src/photoshop/_layerSets.py
--rw-r--r--   0 runner    (1001) docker     (116)     1130 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/src/photoshop/_layers.py
--rw-r--r--   0 runner    (1001) docker     (116)      311 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/src/photoshop/_preferences.py
--rw-r--r--   0 runner    (1001) docker     (116)     4962 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/src/photoshop/_selection.py
--rw-r--r--   0 runner    (1001) docker     (116)     2413 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/src/photoshop/action_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (116)      516 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/src/photoshop/action_list.py
--rw-r--r--   0 runner    (1001) docker     (116)      612 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/src/photoshop/action_refrence.py
--rw-r--r--   0 runner    (1001) docker     (116)     8004 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/src/photoshop/application.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-07 17:11:02.655590 photoshop_python_api-0.8.0/src/photoshop/colors/
--rw-r--r--   0 runner    (1001) docker     (116)      250 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/src/photoshop/colors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1099 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/src/photoshop/colors/cmyk.py
--rw-r--r--   0 runner    (1001) docker     (116)      740 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/src/photoshop/colors/hsb.py
--rw-r--r--   0 runner    (1001) docker     (116)      590 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/src/photoshop/colors/lab.py
--rw-r--r--   0 runner    (1001) docker     (116)      797 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/src/photoshop/colors/rgb.py
--rw-r--r--   0 runner    (1001) docker     (116)     2238 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/src/photoshop/constants.py
--rw-r--r--   0 runner    (1001) docker     (116)     3539 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/src/photoshop/enumerations.py
--rw-r--r--   0 runner    (1001) docker     (116)      234 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/src/photoshop/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-07 17:11:02.655590 photoshop_python_api-0.8.0/src/photoshop/save_options/
--rw-r--r--   0 runner    (1001) docker     (116)      657 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/src/photoshop/save_options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      160 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/src/photoshop/save_options/bmp.py
--rw-r--r--   0 runner    (1001) docker     (116)      183 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/src/photoshop/save_options/eps.py
--rw-r--r--   0 runner    (1001) docker     (116)      183 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/src/photoshop/save_options/gif.py
--rw-r--r--   0 runner    (1001) docker     (116)     1475 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/src/photoshop/save_options/jpg.py
--rw-r--r--   0 runner    (1001) docker     (116)      183 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/src/photoshop/save_options/pdf.py
--rw-r--r--   0 runner    (1001) docker     (116)     1506 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/src/photoshop/save_options/png.py
--rw-r--r--   0 runner    (1001) docker     (116)     1348 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/src/photoshop/save_options/psd.py
--rw-r--r--   0 runner    (1001) docker     (116)     3476 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/src/photoshop/save_options/tif.py
--rw-r--r--   0 runner    (1001) docker     (116)     1503 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/src/photoshop/solid_color.py
--rw-r--r--   0 runner    (1001) docker     (116)      149 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/src/photoshop/text_fonts.py
--rw-r--r--   0 runner    (1001) docker     (116)     1396 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/src/photoshop/text_item.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-07 17:11:02.659590 photoshop_python_api-0.8.0/src/photoshop_python_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     5842 2020-04-07 17:11:01.000000 photoshop_python_api-0.8.0/src/photoshop_python_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2860 2020-04-07 17:11:02.000000 photoshop_python_api-0.8.0/src/photoshop_python_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-04-07 17:11:01.000000 photoshop_python_api-0.8.0/src/photoshop_python_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       16 2020-04-07 17:11:01.000000 photoshop_python_api-0.8.0/src/photoshop_python_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       10 2020-04-07 17:11:01.000000 photoshop_python_api-0.8.0/src/photoshop_python_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-07 17:11:02.659590 photoshop_python_api-0.8.0/test/
--rw-r--r--   0 runner    (1001) docker     (116)      261 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/test/manual_test_all_examples.py
--rw-r--r--   0 runner    (1001) docker     (116)     1503 2020-04-07 17:10:49.000000 photoshop_python_api-0.8.0/test/manual_test_application.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-08 17:30:04.413087 photoshop_python_api-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (116)      209 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-08 17:30:04.393087 photoshop_python_api-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-08 17:30:04.393087 photoshop_python_api-0.9.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (116)      708 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/.github/ISSUE_TEMPLATE/bug_report.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-08 17:30:04.393087 photoshop_python_api-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (116)      865 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      264 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (116)     1166 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      195 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (116)      568 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      228 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (116)       43 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     1061 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)     5842 2020-04-08 17:30:04.413087 photoshop_python_api-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     4018 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (116)       26 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-08 17:30:04.393087 photoshop_python_api-0.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (116)     6770 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (116)       30 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     5767 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1107 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/docs/generate_usage.py
+-rw-r--r--   0 runner    (1001) docker     (116)      233 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      624 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     6463 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-08 17:30:04.393087 photoshop_python_api-0.9.0/docs/src/
+-rw-r--r--   0 runner    (1001) docker     (116)       64 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/docs/src/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      794 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/docs/src/photoshop.colors.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     1795 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/docs/src/photoshop.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     1567 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/docs/src/photoshop.save_options.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     2648 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-08 17:30:04.405087 photoshop_python_api-0.9.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (116)      540 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/examples/active_layer.py
+-rw-r--r--   0 runner    (1001) docker     (116)      401 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/examples/add_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (116)      650 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/examples/add_slate.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1290 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/examples/apply_crystallize_filter_action.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1712 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/examples/apply_filters.py
+-rw-r--r--   0 runner    (1001) docker     (116)      738 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/examples/color.py
+-rw-r--r--   0 runner    (1001) docker     (116)      363 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/examples/compare_colors.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1401 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/examples/copy_and_paste.py
+-rw-r--r--   0 runner    (1001) docker     (116)      622 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/examples/create_thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (116)      214 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/examples/current_tool.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2340 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/examples/emboss_action.py
+-rw-r--r--   0 runner    (1001) docker     (116)      252 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/examples/eval_javascript.py
+-rw-r--r--   0 runner    (1001) docker     (116)  3148164 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/examples/export_layers_as_png.psd
+-rw-r--r--   0 runner    (1001) docker     (116)      943 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/examples/export_layers_as_png.py
+-rw-r--r--   0 runner    (1001) docker     (116)      969 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/examples/fill_selection.py
+-rw-r--r--   0 runner    (1001) docker     (116)      662 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/examples/hello_world.py
+-rw-r--r--   0 runner    (1001) docker     (116)  2689431 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/examples/layer_comps.psd
+-rw-r--r--   0 runner    (1001) docker     (116)      578 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/examples/link_layer.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1236 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/examples/load_selection.py
+-rw-r--r--   0 runner    (1001) docker     (116)      541 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/examples/move_to_end.py
+-rw-r--r--   0 runner    (1001) docker     (116)      448 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/examples/new_document.py
+-rw-r--r--   0 runner    (1001) docker     (116)      245 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/examples/open_psd.py
+-rw-r--r--   0 runner    (1001) docker     (116)      717 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/examples/photoshop_session.py
+-rw-r--r--   0 runner    (1001) docker     (116)      625 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/examples/rotate_layer.py
+-rw-r--r--   0 runner    (1001) docker     (116)      346 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/examples/save_to_psd.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1642 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/examples/selection_stroke.py
+-rw-r--r--   0 runner    (1001) docker     (116)      253 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/examples/session_callback.py
+-rw-r--r--   0 runner    (1001) docker     (116)      169 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/examples/session_document_duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (116)      674 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/examples/session_hello_world.py
+-rw-r--r--   0 runner    (1001) docker     (116)      177 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/examples/session_new_document.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1817 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/examples/session_smart_sharpen.py
+-rw-r--r--   0 runner    (1001) docker     (116)      552 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/examples/set_active_layer.py
+-rw-r--r--   0 runner    (1001) docker     (116)   430697 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/examples/slate_template.psd
+-rw-r--r--   0 runner    (1001) docker     (116)     1616 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/examples/smart_sharpen.py
+-rw-r--r--   0 runner    (1001) docker     (116)      750 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       16 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       67 2020-04-08 17:30:04.413087 photoshop_python_api-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1422 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-08 17:30:04.393087 photoshop_python_api-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-08 17:30:04.409088 photoshop_python_api-0.9.0/src/photoshop/
+-rw-r--r--   0 runner    (1001) docker     (116)     7188 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/src/photoshop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      170 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/src/photoshop/_active_document.py
+-rw-r--r--   0 runner    (1001) docker     (116)      288 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/src/photoshop/_active_layer.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9593 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/src/photoshop/_artlayer.py
+-rw-r--r--   0 runner    (1001) docker     (116)      970 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/src/photoshop/_artlayers.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4765 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/src/photoshop/_core.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9869 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/src/photoshop/_document.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5731 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/src/photoshop/_documentinfo.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1908 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/src/photoshop/_documents.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2767 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/src/photoshop/_layer.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1096 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/src/photoshop/_layerSet.py
+-rw-r--r--   0 runner    (1001) docker     (116)      904 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/src/photoshop/_layerSets.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1130 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/src/photoshop/_layers.py
+-rw-r--r--   0 runner    (1001) docker     (116)      311 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/src/photoshop/_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4962 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/src/photoshop/_selection.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2413 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/src/photoshop/action_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (116)      516 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/src/photoshop/action_list.py
+-rw-r--r--   0 runner    (1001) docker     (116)      612 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/src/photoshop/action_refrence.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8004 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/src/photoshop/application.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-08 17:30:04.409088 photoshop_python_api-0.9.0/src/photoshop/colors/
+-rw-r--r--   0 runner    (1001) docker     (116)      250 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/src/photoshop/colors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1099 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/src/photoshop/colors/cmyk.py
+-rw-r--r--   0 runner    (1001) docker     (116)      740 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/src/photoshop/colors/hsb.py
+-rw-r--r--   0 runner    (1001) docker     (116)      590 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/src/photoshop/colors/lab.py
+-rw-r--r--   0 runner    (1001) docker     (116)      797 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/src/photoshop/colors/rgb.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2238 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/src/photoshop/constants.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3539 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/src/photoshop/enumerations.py
+-rw-r--r--   0 runner    (1001) docker     (116)      234 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/src/photoshop/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-08 17:30:04.413087 photoshop_python_api-0.9.0/src/photoshop/save_options/
+-rw-r--r--   0 runner    (1001) docker     (116)      657 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/src/photoshop/save_options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      160 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/src/photoshop/save_options/bmp.py
+-rw-r--r--   0 runner    (1001) docker     (116)      183 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/src/photoshop/save_options/eps.py
+-rw-r--r--   0 runner    (1001) docker     (116)      183 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/src/photoshop/save_options/gif.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1475 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/src/photoshop/save_options/jpg.py
+-rw-r--r--   0 runner    (1001) docker     (116)      183 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/src/photoshop/save_options/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1506 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/src/photoshop/save_options/png.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1348 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/src/photoshop/save_options/psd.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3476 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/src/photoshop/save_options/tif.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1503 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/src/photoshop/solid_color.py
+-rw-r--r--   0 runner    (1001) docker     (116)      149 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/src/photoshop/text_fonts.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1396 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/src/photoshop/text_item.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-08 17:30:04.413087 photoshop_python_api-0.9.0/src/photoshop_python_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     5842 2020-04-08 17:30:04.000000 photoshop_python_api-0.9.0/src/photoshop_python_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     2916 2020-04-08 17:30:04.000000 photoshop_python_api-0.9.0/src/photoshop_python_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-04-08 17:30:04.000000 photoshop_python_api-0.9.0/src/photoshop_python_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       16 2020-04-08 17:30:04.000000 photoshop_python_api-0.9.0/src/photoshop_python_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       10 2020-04-08 17:30:04.000000 photoshop_python_api-0.9.0/src/photoshop_python_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-08 17:30:04.413087 photoshop_python_api-0.9.0/test/
+-rw-r--r--   0 runner    (1001) docker     (116)      261 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/test/manual_test_all_examples.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1503 2020-04-08 17:29:57.000000 photoshop_python_api-0.9.0/test/manual_test_application.py
```

### Comparing `photoshop_python_api-0.8.0/.github/ISSUE_TEMPLATE/bug_report.md` & `photoshop_python_api-0.9.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/.github/workflows/pythonpublish.yml` & `photoshop_python_api-0.9.0/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/.pre-commit-config.yaml` & `photoshop_python_api-0.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/.readthedocs.yml` & `photoshop_python_api-0.9.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/LICENSE` & `photoshop_python_api-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/PKG-INFO` & `photoshop_python_api-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: photoshop_python_api
-Version: 0.8.0
+Version: 0.9.0
 Summary: The API for using COM (Component Object Model) objects interfaces of Photoshop.
 Home-page: https://github.com/loonghao/photoshop_python_api
 Author: Long Hao
 Author-email: hal.long@outllok.com
 License: UNKNOWN
 Description: photoshop_python_api
         ====================
```

### Comparing `photoshop_python_api-0.8.0/README.md` & `photoshop_python_api-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/docs/Makefile` & `photoshop_python_api-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/docs/conf.py` & `photoshop_python_api-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/docs/generate_usage.py` & `photoshop_python_api-0.9.0/docs/generate_usage.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/docs/installation.rst` & `photoshop_python_api-0.9.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/docs/make.bat` & `photoshop_python_api-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/docs/src/photoshop.colors.rst` & `photoshop_python_api-0.9.0/docs/src/photoshop.colors.rst`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/docs/src/photoshop.rst` & `photoshop_python_api-0.9.0/docs/src/photoshop.rst`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/docs/src/photoshop.save_options.rst` & `photoshop_python_api-0.9.0/docs/src/photoshop.save_options.rst`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/docs/usage.rst` & `photoshop_python_api-0.9.0/docs/usage.rst`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 Usage
 =====
 
 Active Layer
 ------------
   .. literalinclude:: ../examples/active_layer.py
 
+Add Metadata
+------------
+  .. literalinclude:: ../examples/add_metadata.py
+
 Add Slate
 ---------
   .. literalinclude:: ../examples/add_slate.py
 
 Apply Crystallize Filter Action
 -------------------------------
   .. literalinclude:: ../examples/apply_crystallize_filter_action.py
```

### Comparing `photoshop_python_api-0.8.0/examples/active_layer.py` & `photoshop_python_api-0.9.0/examples/active_layer.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/examples/add_slate.py` & `photoshop_python_api-0.9.0/examples/add_slate.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/examples/apply_crystallize_filter_action.py` & `photoshop_python_api-0.9.0/examples/apply_crystallize_filter_action.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/examples/apply_filters.py` & `photoshop_python_api-0.9.0/examples/apply_filters.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/examples/color.py` & `photoshop_python_api-0.9.0/examples/color.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/examples/copy_and_paste.py` & `photoshop_python_api-0.9.0/examples/copy_and_paste.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/examples/create_thumbnail.py` & `photoshop_python_api-0.9.0/examples/create_thumbnail.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/examples/emboss_action.py` & `photoshop_python_api-0.9.0/examples/emboss_action.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/examples/export_layers_as_png.psd` & `photoshop_python_api-0.9.0/examples/export_layers_as_png.psd`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/examples/export_layers_as_png.py` & `photoshop_python_api-0.9.0/examples/export_layers_as_png.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/examples/fill_selection.py` & `photoshop_python_api-0.9.0/examples/fill_selection.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/examples/hello_world.py` & `photoshop_python_api-0.9.0/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/examples/layer_comps.psd` & `photoshop_python_api-0.9.0/examples/layer_comps.psd`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/examples/link_layer.py` & `photoshop_python_api-0.9.0/examples/link_layer.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/examples/load_selection.py` & `photoshop_python_api-0.9.0/examples/load_selection.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/examples/move_to_end.py` & `photoshop_python_api-0.9.0/examples/move_to_end.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/examples/photoshop_session.py` & `photoshop_python_api-0.9.0/examples/photoshop_session.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/examples/rotate_layer.py` & `photoshop_python_api-0.9.0/examples/rotate_layer.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/examples/selection_stroke.py` & `photoshop_python_api-0.9.0/examples/selection_stroke.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/examples/session_hello_world.py` & `photoshop_python_api-0.9.0/examples/session_hello_world.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/examples/session_smart_sharpen.py` & `photoshop_python_api-0.9.0/examples/session_smart_sharpen.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/examples/set_active_layer.py` & `photoshop_python_api-0.9.0/examples/set_active_layer.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/examples/slate_template.psd` & `photoshop_python_api-0.9.0/examples/slate_template.psd`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/examples/smart_sharpen.py` & `photoshop_python_api-0.9.0/examples/smart_sharpen.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/requirements-dev.txt` & `photoshop_python_api-0.9.0/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/setup.py` & `photoshop_python_api-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/src/photoshop/__init__.py` & `photoshop_python_api-0.9.0/src/photoshop/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,32 @@
     from photoshop.enumerations import *
     from photoshop.errors import *
     from photoshop.colors import *
     from photoshop.solid_color import SolidColor
     from photoshop.save_options import *
     from photoshop.text_fonts import TextFonts
     from photoshop.text_item import TextItem
+
+    # All public APIs.
+    __all__ = (
+        [
+            'ActionDescriptor',
+            'ActionList',
+            'ActionReference',
+            'Application',
+            'SolidColor',
+            'TextFonts',
+            'TextItem',
+            'Session'
+        ]
+        + colors.__all__
+        + save_options.__all__
+        + enumerations.__all__
+        + errors.__all__
+    )
 except ModuleNotFoundError:
     # Fix Build docs failed on readthedocs.
     pass
 
 
 class Session:
     """Session of photoshop.
@@ -195,30 +213,12 @@
         except Exception as err:
             raise PhotoshopPythonAPIError(err)
         finally:
             if self._auto_close:
                 self.active_document.close()
 
 
-# All public APIs.
-__all__ = (
-    [
-        'ActionDescriptor',
-        'ActionList',
-        'ActionReference',
-        'Application',
-        'SolidColor',
-        'TextFonts',
-        'TextItem',
-        'Session'
-    ]
-    + colors.__all__
-    + save_options.__all__
-    + enumerations.__all__
-    + errors.__all__
-)
-
 __title__ = 'photoshop_python_api'
-__version__ = '0.8.0'
+__version__ = '0.9.0'
 __author__ = 'Long Hao'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2018 Long Hao'
```

### Comparing `photoshop_python_api-0.8.0/src/photoshop/_artlayer.py` & `photoshop_python_api-0.9.0/src/photoshop/_artlayer.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/src/photoshop/_artlayers.py` & `photoshop_python_api-0.9.0/src/photoshop/_artlayers.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/src/photoshop/_core.py` & `photoshop_python_api-0.9.0/src/photoshop/_core.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/src/photoshop/_document.py` & `photoshop_python_api-0.9.0/src/photoshop/_document.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from photoshop.errors import COMError
 from photoshop._layers import Layers
 from photoshop._layerSets import LayerSets
 from photoshop._selection import Selection
 from photoshop._layerSet import LayerSet
 from photoshop.enumerations import ExtensionType
 from photoshop.enumerations import SaveOptions
+from photoshop._documentinfo import DocumentInfo
 
 
 # pylint: disable=too-many-public-methods
 class Document(Photoshop):
     object_name = 'Application'
 
     def __init__(self, parent):
@@ -98,15 +99,15 @@
     def fullName(self):
         """The full path name of the Document."""
         try:
             return self.app.fullName
         except COMError:
             self.eval_javascript(
                 'alert ("Please save your Document first!",'
-                '"{}")'.format(self.title),
+                '"{}")'.format(self.name),
             )
 
     @property
     def height(self):
         """The height of the Document."""
         return self.app.Height
 
@@ -125,15 +126,15 @@
     def id(self):
         """The unique ID of this Document."""
         return self.app.Id
 
     @property
     def info(self):
         """Metadata about the Document."""
-        return self.app.info
+        return DocumentInfo(self.app.info)
 
     @property
     def layerComps(self):
         """The layer comps collection in this Document."""
         return self.app.LayerComps
 
     @property
@@ -175,15 +176,15 @@
     def path(self):
         """The path to the Document."""
         try:
             return self.app.Path
         except COMError:
             self.eval_javascript(
                 'alert ("Please save your Document first!",'
-                '"{}")'.format(self.title),
+                '"{}")'.format(self.name),
             )
 
     @path.setter
     def path(self, path):
         self.app.fullName = path
 
     @property
```

### Comparing `photoshop_python_api-0.8.0/src/photoshop/_documents.py` & `photoshop_python_api-0.9.0/src/photoshop/_documents.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/src/photoshop/_layer.py` & `photoshop_python_api-0.9.0/src/photoshop/_layer.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/src/photoshop/_layerSet.py` & `photoshop_python_api-0.9.0/src/photoshop/_layerSet.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/src/photoshop/_layerSets.py` & `photoshop_python_api-0.9.0/src/photoshop/_layerSets.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/src/photoshop/_layers.py` & `photoshop_python_api-0.9.0/src/photoshop/_layers.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/src/photoshop/_selection.py` & `photoshop_python_api-0.9.0/src/photoshop/_selection.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/src/photoshop/action_descriptor.py` & `photoshop_python_api-0.9.0/src/photoshop/action_descriptor.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/src/photoshop/action_list.py` & `photoshop_python_api-0.9.0/src/photoshop/action_list.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/src/photoshop/action_refrence.py` & `photoshop_python_api-0.9.0/src/photoshop/action_refrence.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/src/photoshop/application.py` & `photoshop_python_api-0.9.0/src/photoshop/application.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/src/photoshop/colors/cmyk.py` & `photoshop_python_api-0.9.0/src/photoshop/colors/cmyk.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/src/photoshop/colors/hsb.py` & `photoshop_python_api-0.9.0/src/photoshop/colors/hsb.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/src/photoshop/colors/lab.py` & `photoshop_python_api-0.9.0/src/photoshop/colors/lab.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/src/photoshop/colors/rgb.py` & `photoshop_python_api-0.9.0/src/photoshop/colors/rgb.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/src/photoshop/constants.py` & `photoshop_python_api-0.9.0/src/photoshop/constants.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/src/photoshop/enumerations.py` & `photoshop_python_api-0.9.0/src/photoshop/enumerations.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/src/photoshop/save_options/__init__.py` & `photoshop_python_api-0.9.0/src/photoshop/save_options/__init__.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/src/photoshop/save_options/jpg.py` & `photoshop_python_api-0.9.0/src/photoshop/save_options/jpg.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/src/photoshop/save_options/png.py` & `photoshop_python_api-0.9.0/src/photoshop/save_options/png.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/src/photoshop/save_options/psd.py` & `photoshop_python_api-0.9.0/src/photoshop/save_options/psd.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/src/photoshop/save_options/tif.py` & `photoshop_python_api-0.9.0/src/photoshop/save_options/tif.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/src/photoshop/solid_color.py` & `photoshop_python_api-0.9.0/src/photoshop/solid_color.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/src/photoshop/text_item.py` & `photoshop_python_api-0.9.0/src/photoshop/text_item.py`

 * *Files identical despite different names*

### Comparing `photoshop_python_api-0.8.0/src/photoshop_python_api.egg-info/PKG-INFO` & `photoshop_python_api-0.9.0/src/photoshop_python_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: photoshop-python-api
-Version: 0.8.0
+Version: 0.9.0
 Summary: The API for using COM (Component Object Model) objects interfaces of Photoshop.
 Home-page: https://github.com/loonghao/photoshop_python_api
 Author: Long Hao
 Author-email: hal.long@outllok.com
 License: UNKNOWN
 Description: photoshop_python_api
         ====================
```

### Comparing `photoshop_python_api-0.8.0/src/photoshop_python_api.egg-info/SOURCES.txt` & `photoshop_python_api-0.9.0/src/photoshop_python_api.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 docs/make.bat
 docs/usage.rst
 docs/src/modules.rst
 docs/src/photoshop.colors.rst
 docs/src/photoshop.rst
 docs/src/photoshop.save_options.rst
 examples/active_layer.py
+examples/add_metadata.py
 examples/add_slate.py
 examples/apply_crystallize_filter_action.py
 examples/apply_filters.py
 examples/color.py
 examples/compare_colors.py
 examples/copy_and_paste.py
 examples/create_thumbnail.py
@@ -62,14 +63,15 @@
 src/photoshop/__init__.py
 src/photoshop/_active_document.py
 src/photoshop/_active_layer.py
 src/photoshop/_artlayer.py
 src/photoshop/_artlayers.py
 src/photoshop/_core.py
 src/photoshop/_document.py
+src/photoshop/_documentinfo.py
 src/photoshop/_documents.py
 src/photoshop/_layer.py
 src/photoshop/_layerSet.py
 src/photoshop/_layerSets.py
 src/photoshop/_layers.py
 src/photoshop/_preferences.py
 src/photoshop/_selection.py
```

### Comparing `photoshop_python_api-0.8.0/test/manual_test_application.py` & `photoshop_python_api-0.9.0/test/manual_test_application.py`

 * *Files identical despite different names*

