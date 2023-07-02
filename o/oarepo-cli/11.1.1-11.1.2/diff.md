# Comparing `tmp/oarepo-cli-11.1.1.tar.gz` & `tmp/oarepo-cli-11.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-cli-11.1.1.tar", last modified: Sun Jul  2 12:39:00 2023, max compression
+gzip compressed data, was "oarepo-cli-11.1.2.tar", last modified: Sun Jul  2 13:13:29 2023, max compression
```

## Comparing `oarepo-cli-11.1.1.tar` & `oarepo-cli-11.1.2.tar`

### file list

```diff
@@ -1,402 +1,402 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.275783 oarepo-cli-11.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-07-02 12:39:00.275783 oarepo-cli-11.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.211781 oarepo-cli-11.1.1/oarepo_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.211781 oarepo-cli-11.1.1/oarepo_cli/build_command/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/build_command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/build_command/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.211781 oarepo-cli-11.1.1/oarepo_cli/build_command/steps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/build_command/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/build_command/wizard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.211781 oarepo-cli-11.1.1/oarepo_cli/develop/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/develop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/develop/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/develop/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/develop/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.211781 oarepo-cli-11.1.1/oarepo_cli/develop/runners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/develop/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/develop/runners/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/develop/runners/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.211781 oarepo-cli-11.1.1/oarepo_cli/develop/steps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/develop/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/develop/steps/check_db.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/develop/steps/check_s3_location.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/develop/steps/check_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/develop/steps/check_site.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/develop/steps/check_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/develop/steps/check_venv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/develop/steps/develop_step.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/develop/wizard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.211781 oarepo-cli-11.1.1/oarepo_cli/format/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/format/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/format/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.215782 oarepo-cli-11.1.1/oarepo_cli/format/steps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/format/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/format/steps/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/format/steps/format_javascript.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/format/steps/format_jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/format/steps/format_python.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/format/wizard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.215782 oarepo-cli-11.1.1/oarepo_cli/initialize/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/initialize/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.215782 oarepo-cli-11.1.1/oarepo_cli/initialize/steps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/initialize/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/initialize/steps/create_monorepo.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/initialize/steps/initialize_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/initialize/steps/install_nrp_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/initialize/wizard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.215782 oarepo-cli-11.1.1/oarepo_cli/kill/
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/kill/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.215782 oarepo-cli-11.1.1/oarepo_cli/local/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/local/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.215782 oarepo-cli-11.1.1/oarepo_cli/local/add/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/local/add/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/local/add/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.215782 oarepo-cli-11.1.1/oarepo_cli/local/add/steps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/local/add/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/local/add/steps/add_local.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/local/add/steps/install.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/local/add/wizard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.215782 oarepo-cli-11.1.1/oarepo_cli/local/remove/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/local/remove/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/local/remove/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.215782 oarepo-cli-11.1.1/oarepo_cli/local/remove/steps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/local/remove/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/local/remove/steps/uninstall.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/local/remove/wizard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.215782 oarepo-cli-11.1.1/oarepo_cli/model/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.215782 oarepo-cli-11.1.1/oarepo_cli/model/add/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/model/add/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/model/add/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.219782 oarepo-cli-11.1.1/oarepo_cli/model/add/steps/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/model/add/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/model/add/steps/add_custom_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/model/add/steps/add_docs_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/model/add/steps/add_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/model/add/steps/add_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/model/add/steps/add_nr_vocabularies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/model/add/steps/add_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/model/add/steps/add_pid_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/model/add/steps/add_relations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/model/add/steps/add_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/model/add/steps/add_vocabularies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/model/add/steps/create_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/model/add/wizard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.219782 oarepo-cli-11.1.1/oarepo_cli/model/compile/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/model/compile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/model/compile/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.219782 oarepo-cli-11.1.1/oarepo_cli/model/compile/steps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/model/compile/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/model/compile/steps/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/model/compile/steps/remove_previous.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/model/compile/wizard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.219782 oarepo-cli-11.1.1/oarepo_cli/model/gen/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/model/gen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/model/gen/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/model/gen/formats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.219782 oarepo-cli-11.1.1/oarepo_cli/model/install/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/model/install/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/model/install/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.219782 oarepo-cli-11.1.1/oarepo_cli/model/install/steps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/model/install/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/model/install/steps/alembic.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/model/install/steps/install.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/model/install/steps/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/model/install/steps/update_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/model/install/wizard.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/model/list.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/model/model_support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.219782 oarepo-cli-11.1.1/oarepo_cli/model/uninstall/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/model/uninstall/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/model/uninstall/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.219782 oarepo-cli-11.1.1/oarepo_cli/model/uninstall/steps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/model/uninstall/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/model/uninstall/steps/uninstall.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/model/uninstall/wizard.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/model/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/package_versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.223782 oarepo-cli-11.1.1/oarepo_cli/run/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/run/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.223782 oarepo-cli-11.1.1/oarepo_cli/run/steps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/run/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/run/steps/run_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/run/wizard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.223782 oarepo-cli-11.1.1/oarepo_cli/site/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/site/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.223782 oarepo-cli-11.1.1/oarepo_cli/site/add/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/site/add/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/site/add/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.223782 oarepo-cli-11.1.1/oarepo_cli/site/add/steps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/site/add/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/site/add/steps/check_requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/site/add/steps/compile_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/site/add/steps/init_database.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/site/add/steps/init_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/site/add/steps/install_invenio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/site/add/steps/install_site.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/site/add/steps/link_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/site/add/steps/next_steps.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/site/add/steps/resolve_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/site/add/steps/start_containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/site/add/wizard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/site/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/site/list.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/site/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)    18674 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/site/site_support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.223782 oarepo-cli-11.1.1/oarepo_cli/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.223782 oarepo-cli-11.1.1/oarepo_cli/templates/repo/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/repo/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.223782 oarepo-cli-11.1.1/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/.envrc
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.223782 oarepo-cli-11.1.1/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/local/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/local/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/local/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.227782 oarepo-cli-11.1.1/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/models/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      337 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/nrp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.227782 oarepo-cli-11.1.1/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/sites/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/sites/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.227782 oarepo-cli-11.1.1/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/ui/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/ui/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.227782 oarepo-cli-11.1.1/oarepo_cli/templates/site/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.227782 oarepo-cli-11.1.1/oarepo_cli/templates/site/diffs/
--rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/diffs/oarepo-to-rdm-v11.0.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.227782 oarepo-cli-11.1.1/oarepo_cli/templates/site/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/hooks/post_gen_project.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.227782 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/.envrc
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/.eslintrc.json
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.227782 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/app_data/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/app_data/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.227782 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/app_data/pages/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/app_data/pages/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.247782 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/app_data/vocabularies/
--rw-r--r--   0 runner    (1001) docker     (123) 19635835 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/app_data/vocabularies/affiliations_ror.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/app_data/vocabularies/subjects_oecd_fos.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/app_data/vocabularies.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.203781 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.247782 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/assets/less/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.247782 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/assets/less/site/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/assets/less/site/css.overrides
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.247782 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/assets/less/site/globals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/assets/less/site/globals/site.overrides
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/assets/less/site/globals/site.variables
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/assets/less/theme.config
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/assets/less/theme.less
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.247782 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/assets/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/assets/templates/.readme
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.247782 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/assets/templates/custom_fields/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/assets/templates/custom_fields/.readme
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/build.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.247782 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker/
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker/Dockerfile.production
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.251783 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker/nginx/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker/nginx/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.251783 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker/nginx/conf.d/
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker/nginx/conf.d/default.conf
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker/nginx/nginx.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.251783 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker/pgadmin/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker/pgadmin/servers.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.251783 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker/uwsgi/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker/uwsgi/uwsgi.ini
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker-compose.full.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker-services.yml
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/invenio.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/prettierrc.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.251783 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.251783 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/tests/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.251783 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.203781 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.203781 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/assets/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.203781 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/assets/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.251783 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/assets/semantic-ui/js/{{cookiecutter.package_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/assets/semantic-ui/js/{{cookiecutter.package_name}}/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.203781 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/assets/semantic-ui/less/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.251783 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/assets/semantic-ui/less/{{cookiecutter.package_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/assets/semantic-ui/less/{{cookiecutter.package_name}}/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.203781 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.203781 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.255783 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/templates/semantic-ui/oarepo_ui/
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/templates/semantic-ui/oarepo_ui/detail.html
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/templates/semantic-ui/oarepo_ui/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/templates/semantic-ui/oarepo_ui/header.html
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/templates/semantic-ui/oarepo_ui/javascript.html
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/templates/semantic-ui/oarepo_ui/trackingcode.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.255783 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/templates/semantic-ui/{{cookiecutter.package_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/templates/semantic-ui/{{cookiecutter.package_name}}/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/templates/semantic-ui/{{cookiecutter.package_name}}/frontpage.html
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/templates/semantic-ui/{{cookiecutter.package_name}}/searchbar.html
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.255783 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.255783 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/static/images/invenio-rdm.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/static/images/logo-invenio-white.svg
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/static/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.203781 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.255783 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/templates/semantic-ui/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/templates/semantic-ui/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.255783 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/translations/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/translations/babel.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/variables
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.255783 oarepo-cli-11.1.1/oarepo_cli/templates/ui/
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/cookiecutter.json
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/local_extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.255783 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.259783 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.259783 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/resources/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/resources/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.207781 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.207781 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.259783 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/templates/semantic-ui/{{cookiecutter.app_package}}/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/templates/semantic-ui/{{cookiecutter.app_package}}/detail.html
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/templates/semantic-ui/{{cookiecutter.app_package}}/main.html
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/templates/semantic-ui/{{cookiecutter.app_package}}/search.html
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/templates/semantic-ui/{{cookiecutter.app_package}}/sidebar.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.259783 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.207781 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.259783 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.207781 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.259783 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/js/{{cookiecutter.app_package}}/
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/js/{{cookiecutter.app_package}}/custom-components.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.259783 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/js/{{cookiecutter.app_package}}/search/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.263783 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/js/{{cookiecutter.app_package}}/search/components/
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/js/{{cookiecutter.app_package}}/search/components/EmptyResultsElement.jsx
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/js/{{cookiecutter.app_package}}/search/components/MultipleSearchBarElement.jsx
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/js/{{cookiecutter.app_package}}/search/components/ResultsGridItem.jsx
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/js/{{cookiecutter.app_package}}/search/components/ResultsListItem.jsx
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/js/{{cookiecutter.app_package}}/search/components/index.js
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/js/{{cookiecutter.app_package}}/search/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.207781 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/less/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.263783 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/less/{{cookiecutter.app_package}}/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/less/{{cookiecutter.app_package}}/custom-components.less
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.263783 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/less/{{cookiecutter.app_package}}/definitions/
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/less/{{cookiecutter.app_package}}/definitions/sample.less
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.207781 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/less/{{cookiecutter.app_package}}/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.263783 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/less/{{cookiecutter.app_package}}/theme/elements/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/less/{{cookiecutter.app_package}}/theme/elements/sample.overrides
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/less/{{cookiecutter.app_package}}/theme/elements/sample.variables
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.207781 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.263783 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/i18next-scanner.config.js
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/i18next.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.263783 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.263783 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/cs/
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/cs/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/cs/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.263783 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/de/
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/de/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/de/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.263783 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/el/
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/el/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/el/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.263783 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/en/
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/en/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/en/translations.json
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.267783 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/scripts/compileCatalog.js
--rwxr-xr-x   0 runner    (1001) docker     (123)      351 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/scripts/compileLanguages.sh
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/scripts/initCatalog.js
--rw-r--r--   0 runner    (1001) docker     (123)    41082 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/yarn.lock
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/webpack.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.267783 oarepo-cli-11.1.1/oarepo_cli/ui/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.267783 oarepo-cli-11.1.1/oarepo_cli/ui/add/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/ui/add/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/ui/add/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/ui/add/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.267783 oarepo-cli-11.1.1/oarepo_cli/ui/add/steps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/ui/add/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/ui/add/steps/add_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/ui/add/steps/jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/ui/add/wizard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.267783 oarepo-cli-11.1.1/oarepo_cli/ui/install/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/ui/install/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/ui/install/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.267783 oarepo-cli-11.1.1/oarepo_cli/ui/install/steps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/ui/install/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/ui/install/steps/build_assets_step.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/ui/install/steps/install_step.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/ui/install/wizard.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/ui/list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.271783 oarepo-cli-11.1.1/oarepo_cli/ui/uninstall/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/ui/uninstall/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/ui/uninstall/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.271783 oarepo-cli-11.1.1/oarepo_cli/ui/uninstall/steps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/ui/uninstall/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/ui/uninstall/steps/uninstall.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/ui/uninstall/wizard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.271783 oarepo-cli-11.1.1/oarepo_cli/upgrade/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/upgrade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/upgrade/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.271783 oarepo-cli-11.1.1/oarepo_cli/upgrade/steps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/upgrade/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/upgrade/steps/upgrade_docker_nrp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/upgrade/steps/upgrade_nrp.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/upgrade/steps/upgrade_site.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/upgrade/wizard.py
--rw-r--r--   0 runner    (1001) docker     (123)    19458 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.271783 oarepo-cli-11.1.1/oarepo_cli/watch/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/watch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/watch/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.271783 oarepo-cli-11.1.1/oarepo_cli/watch/steps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/watch/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/watch/steps/watcher_step.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/watch/wizard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.275783 oarepo-cli-11.1.1/oarepo_cli/wizard/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/wizard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/wizard/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/wizard/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/wizard/steps.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/oarepo_cli/wizard/wizard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:39:00.211781 oarepo-cli-11.1.1/oarepo_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-07-02 12:39:00.000000 oarepo-cli-11.1.1/oarepo_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18498 2023-07-02 12:39:00.000000 oarepo-cli-11.1.1/oarepo_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 12:39:00.000000 oarepo-cli-11.1.1/oarepo_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-02 12:39:00.000000 oarepo-cli-11.1.1/oarepo_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-02 12:39:00.000000 oarepo-cli-11.1.1/oarepo_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-02 12:39:00.000000 oarepo-cli-11.1.1/oarepo_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-02 12:39:00.275783 oarepo-cli-11.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-02 12:38:54.000000 oarepo-cli-11.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.495100 oarepo-cli-11.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-07-02 13:13:29.495100 oarepo-cli-11.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.399099 oarepo-cli-11.1.2/oarepo_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.403100 oarepo-cli-11.1.2/oarepo_cli/build_command/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/build_command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/build_command/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.403100 oarepo-cli-11.1.2/oarepo_cli/build_command/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/build_command/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/build_command/wizard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.403100 oarepo-cli-11.1.2/oarepo_cli/develop/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/develop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/develop/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/develop/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/develop/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.407100 oarepo-cli-11.1.2/oarepo_cli/develop/runners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/develop/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/develop/runners/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/develop/runners/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.407100 oarepo-cli-11.1.2/oarepo_cli/develop/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/develop/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/develop/steps/check_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/develop/steps/check_s3_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/develop/steps/check_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/develop/steps/check_site.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/develop/steps/check_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/develop/steps/check_venv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/develop/steps/develop_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/develop/wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.407100 oarepo-cli-11.1.2/oarepo_cli/format/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/format/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/format/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.411100 oarepo-cli-11.1.2/oarepo_cli/format/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/format/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/format/steps/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/format/steps/format_javascript.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/format/steps/format_jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/format/steps/format_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/format/wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.411100 oarepo-cli-11.1.2/oarepo_cli/initialize/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/initialize/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.411100 oarepo-cli-11.1.2/oarepo_cli/initialize/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/initialize/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/initialize/steps/create_monorepo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/initialize/steps/initialize_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/initialize/steps/install_nrp_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/initialize/wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.411100 oarepo-cli-11.1.2/oarepo_cli/kill/
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/kill/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.411100 oarepo-cli-11.1.2/oarepo_cli/local/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/local/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.415099 oarepo-cli-11.1.2/oarepo_cli/local/add/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/local/add/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/local/add/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.415099 oarepo-cli-11.1.2/oarepo_cli/local/add/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/local/add/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/local/add/steps/add_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/local/add/steps/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/local/add/wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.415099 oarepo-cli-11.1.2/oarepo_cli/local/remove/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/local/remove/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/local/remove/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.415099 oarepo-cli-11.1.2/oarepo_cli/local/remove/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/local/remove/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/local/remove/steps/uninstall.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/local/remove/wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.415099 oarepo-cli-11.1.2/oarepo_cli/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.415099 oarepo-cli-11.1.2/oarepo_cli/model/add/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/model/add/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/model/add/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.419100 oarepo-cli-11.1.2/oarepo_cli/model/add/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/model/add/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/model/add/steps/add_custom_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/model/add/steps/add_docs_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/model/add/steps/add_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/model/add/steps/add_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/model/add/steps/add_nr_vocabularies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/model/add/steps/add_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/model/add/steps/add_pid_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/model/add/steps/add_relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/model/add/steps/add_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/model/add/steps/add_vocabularies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/model/add/steps/create_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/model/add/wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.419100 oarepo-cli-11.1.2/oarepo_cli/model/compile/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/model/compile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/model/compile/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.423100 oarepo-cli-11.1.2/oarepo_cli/model/compile/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/model/compile/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/model/compile/steps/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/model/compile/steps/remove_previous.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/model/compile/wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.423100 oarepo-cli-11.1.2/oarepo_cli/model/gen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/model/gen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/model/gen/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/model/gen/formats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.423100 oarepo-cli-11.1.2/oarepo_cli/model/install/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/model/install/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/model/install/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.423100 oarepo-cli-11.1.2/oarepo_cli/model/install/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/model/install/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/model/install/steps/alembic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/model/install/steps/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/model/install/steps/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/model/install/steps/update_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/model/install/wizard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/model/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/model/model_support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.427100 oarepo-cli-11.1.2/oarepo_cli/model/uninstall/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/model/uninstall/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/model/uninstall/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.427100 oarepo-cli-11.1.2/oarepo_cli/model/uninstall/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/model/uninstall/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/model/uninstall/steps/uninstall.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/model/uninstall/wizard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/package_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.427100 oarepo-cli-11.1.2/oarepo_cli/run/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/run/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.427100 oarepo-cli-11.1.2/oarepo_cli/run/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/run/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/run/steps/run_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/run/wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.427100 oarepo-cli-11.1.2/oarepo_cli/site/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/site/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.431100 oarepo-cli-11.1.2/oarepo_cli/site/add/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/site/add/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/site/add/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.431100 oarepo-cli-11.1.2/oarepo_cli/site/add/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/site/add/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/site/add/steps/check_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/site/add/steps/compile_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/site/add/steps/init_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/site/add/steps/init_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/site/add/steps/install_invenio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/site/add/steps/install_site.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/site/add/steps/link_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/site/add/steps/next_steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/site/add/steps/resolve_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/site/add/steps/start_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/site/add/wizard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/site/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/site/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/site/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18674 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/site/site_support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.431100 oarepo-cli-11.1.2/oarepo_cli/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.431100 oarepo-cli-11.1.2/oarepo_cli/templates/repo/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/repo/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.435100 oarepo-cli-11.1.2/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/.envrc
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.435100 oarepo-cli-11.1.2/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/local/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/local/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/local/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.435100 oarepo-cli-11.1.2/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/models/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      337 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/nrp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.435100 oarepo-cli-11.1.2/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/sites/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/sites/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.435100 oarepo-cli-11.1.2/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/ui/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.435100 oarepo-cli-11.1.2/oarepo_cli/templates/site/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.435100 oarepo-cli-11.1.2/oarepo_cli/templates/site/diffs/
+-rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/diffs/oarepo-to-rdm-v11.0.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.435100 oarepo-cli-11.1.2/oarepo_cli/templates/site/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/hooks/post_gen_project.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.439100 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/.envrc
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/.eslintrc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.439100 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/app_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/app_data/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.439100 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/app_data/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/app_data/pages/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.467100 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/app_data/vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (123) 19635835 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/app_data/vocabularies/affiliations_ror.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/app_data/vocabularies/subjects_oecd_fos.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/app_data/vocabularies.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.387100 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.467100 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/assets/less/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.467100 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/assets/less/site/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/assets/less/site/css.overrides
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.467100 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/assets/less/site/globals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/assets/less/site/globals/site.overrides
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/assets/less/site/globals/site.variables
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/assets/less/theme.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/assets/less/theme.less
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.467100 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/assets/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/assets/templates/.readme
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.467100 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/assets/templates/custom_fields/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/assets/templates/custom_fields/.readme
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/build.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.471100 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker/Dockerfile.production
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.471100 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker/nginx/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker/nginx/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.471100 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker/nginx/conf.d/
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker/nginx/conf.d/default.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker/nginx/nginx.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.471100 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker/pgadmin/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker/pgadmin/servers.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.471100 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker/uwsgi/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker/uwsgi/uwsgi.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker-compose.full.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker-services.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/invenio.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/prettierrc.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.471100 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.471100 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/tests/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.471100 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.391100 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.391100 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/assets/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.391100 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/assets/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.475100 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/assets/semantic-ui/js/{{cookiecutter.package_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/assets/semantic-ui/js/{{cookiecutter.package_name}}/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.391100 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/assets/semantic-ui/less/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.475100 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/assets/semantic-ui/less/{{cookiecutter.package_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/assets/semantic-ui/less/{{cookiecutter.package_name}}/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.391100 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.391100 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.475100 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/templates/semantic-ui/oarepo_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/templates/semantic-ui/oarepo_ui/detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/templates/semantic-ui/oarepo_ui/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/templates/semantic-ui/oarepo_ui/header.html
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/templates/semantic-ui/oarepo_ui/javascript.html
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/templates/semantic-ui/oarepo_ui/trackingcode.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.475100 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/templates/semantic-ui/{{cookiecutter.package_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/templates/semantic-ui/{{cookiecutter.package_name}}/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/templates/semantic-ui/{{cookiecutter.package_name}}/frontpage.html
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/templates/semantic-ui/{{cookiecutter.package_name}}/searchbar.html
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.475100 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.475100 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/static/images/invenio-rdm.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/static/images/logo-invenio-white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/static/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.391100 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.475100 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/templates/semantic-ui/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/templates/semantic-ui/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.475100 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/translations/babel.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/variables
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.479100 oarepo-cli-11.1.2/oarepo_cli/templates/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/cookiecutter.json
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/local_extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.479100 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.479100 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.479100 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/resources/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/resources/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.391100 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.391100 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.479100 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/templates/semantic-ui/{{cookiecutter.app_package}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/templates/semantic-ui/{{cookiecutter.app_package}}/detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/templates/semantic-ui/{{cookiecutter.app_package}}/main.html
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/templates/semantic-ui/{{cookiecutter.app_package}}/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/templates/semantic-ui/{{cookiecutter.app_package}}/sidebar.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.479100 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.391100 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.483100 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.391100 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.483100 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/js/{{cookiecutter.app_package}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/js/{{cookiecutter.app_package}}/custom-components.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.483100 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/js/{{cookiecutter.app_package}}/search/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.483100 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/js/{{cookiecutter.app_package}}/search/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/js/{{cookiecutter.app_package}}/search/components/EmptyResultsElement.jsx
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/js/{{cookiecutter.app_package}}/search/components/MultipleSearchBarElement.jsx
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/js/{{cookiecutter.app_package}}/search/components/ResultsGridItem.jsx
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/js/{{cookiecutter.app_package}}/search/components/ResultsListItem.jsx
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/js/{{cookiecutter.app_package}}/search/components/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/js/{{cookiecutter.app_package}}/search/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.395099 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/less/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.483100 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/less/{{cookiecutter.app_package}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/less/{{cookiecutter.app_package}}/custom-components.less
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.483100 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/less/{{cookiecutter.app_package}}/definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/less/{{cookiecutter.app_package}}/definitions/sample.less
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.395099 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/less/{{cookiecutter.app_package}}/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.483100 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/less/{{cookiecutter.app_package}}/theme/elements/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/less/{{cookiecutter.app_package}}/theme/elements/sample.overrides
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/less/{{cookiecutter.app_package}}/theme/elements/sample.variables
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.395099 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.483100 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/i18next-scanner.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/i18next.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.483100 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.483100 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/cs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/cs/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/cs/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.487100 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/de/
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/de/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/de/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.487100 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/el/
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/el/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/el/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.487100 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/en/
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/en/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/en/translations.json
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.487100 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/scripts/compileCatalog.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)      351 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/scripts/compileLanguages.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/scripts/initCatalog.js
+-rw-r--r--   0 runner    (1001) docker     (123)    41082 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/yarn.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/webpack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.487100 oarepo-cli-11.1.2/oarepo_cli/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.487100 oarepo-cli-11.1.2/oarepo_cli/ui/add/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/ui/add/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/ui/add/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/ui/add/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.487100 oarepo-cli-11.1.2/oarepo_cli/ui/add/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/ui/add/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/ui/add/steps/add_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/ui/add/steps/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/ui/add/wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.491100 oarepo-cli-11.1.2/oarepo_cli/ui/install/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/ui/install/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/ui/install/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.491100 oarepo-cli-11.1.2/oarepo_cli/ui/install/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/ui/install/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/ui/install/steps/build_assets_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/ui/install/steps/install_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/ui/install/wizard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/ui/list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.491100 oarepo-cli-11.1.2/oarepo_cli/ui/uninstall/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/ui/uninstall/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/ui/uninstall/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.491100 oarepo-cli-11.1.2/oarepo_cli/ui/uninstall/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/ui/uninstall/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/ui/uninstall/steps/uninstall.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/ui/uninstall/wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.491100 oarepo-cli-11.1.2/oarepo_cli/upgrade/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/upgrade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/upgrade/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.491100 oarepo-cli-11.1.2/oarepo_cli/upgrade/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/upgrade/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/upgrade/steps/upgrade_docker_nrp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/upgrade/steps/upgrade_nrp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/upgrade/steps/upgrade_site.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/upgrade/wizard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19593 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.491100 oarepo-cli-11.1.2/oarepo_cli/watch/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/watch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/watch/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.495100 oarepo-cli-11.1.2/oarepo_cli/watch/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/watch/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/watch/steps/watcher_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/watch/wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.495100 oarepo-cli-11.1.2/oarepo_cli/wizard/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/wizard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/wizard/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/wizard/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/wizard/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/oarepo_cli/wizard/wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:13:29.403100 oarepo-cli-11.1.2/oarepo_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-07-02 13:13:29.000000 oarepo-cli-11.1.2/oarepo_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18498 2023-07-02 13:13:29.000000 oarepo-cli-11.1.2/oarepo_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 13:13:29.000000 oarepo-cli-11.1.2/oarepo_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-02 13:13:29.000000 oarepo-cli-11.1.2/oarepo_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-02 13:13:29.000000 oarepo-cli-11.1.2/oarepo_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-02 13:13:29.000000 oarepo-cli-11.1.2/oarepo_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-02 13:13:29.495100 oarepo-cli-11.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-02 13:13:22.000000 oarepo-cli-11.1.2/setup.py
```

### Comparing `oarepo-cli-11.1.1/PKG-INFO` & `oarepo-cli-11.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-cli
-Version: 11.1.1
+Version: 11.1.2
 Summary: Utilities for managing invenio monorepo
 Description-Content-Type: text/markdown
 
 # oarepo-cli
 
 Work in progress.
```

### Comparing `oarepo-cli-11.1.1/README.md` & `oarepo-cli-11.1.2/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/build_command/cli.py` & `oarepo-cli-11.1.2/oarepo_cli/build_command/cli.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/build_command/wizard.py` & `oarepo-cli-11.1.2/oarepo_cli/build_command/wizard.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/cli.py` & `oarepo-cli-11.1.2/oarepo_cli/cli.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/config.py` & `oarepo-cli-11.1.2/oarepo_cli/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/develop/cli.py` & `oarepo-cli-11.1.2/oarepo_cli/develop/cli.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/develop/controller.py` & `oarepo-cli-11.1.2/oarepo_cli/develop/controller.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/develop/runners/docker.py` & `oarepo-cli-11.1.2/oarepo_cli/develop/runners/docker.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/develop/runners/local.py` & `oarepo-cli-11.1.2/oarepo_cli/develop/runners/local.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/develop/steps/check_db.py` & `oarepo-cli-11.1.2/oarepo_cli/develop/steps/check_db.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/develop/steps/check_s3_location.py` & `oarepo-cli-11.1.2/oarepo_cli/develop/steps/check_s3_location.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/develop/steps/check_search.py` & `oarepo-cli-11.1.2/oarepo_cli/develop/steps/check_search.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/develop/steps/check_site.py` & `oarepo-cli-11.1.2/oarepo_cli/develop/steps/check_site.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/develop/steps/check_venv.py` & `oarepo-cli-11.1.2/oarepo_cli/develop/steps/check_venv.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/develop/steps/develop_step.py` & `oarepo-cli-11.1.2/oarepo_cli/develop/steps/develop_step.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/develop/wizard.py` & `oarepo-cli-11.1.2/oarepo_cli/develop/wizard.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/format/cli.py` & `oarepo-cli-11.1.2/oarepo_cli/format/cli.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/format/steps/base.py` & `oarepo-cli-11.1.2/oarepo_cli/format/steps/base.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/format/steps/format_javascript.py` & `oarepo-cli-11.1.2/oarepo_cli/format/steps/format_javascript.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/format/steps/format_jinja.py` & `oarepo-cli-11.1.2/oarepo_cli/format/steps/format_jinja.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/format/steps/format_python.py` & `oarepo-cli-11.1.2/oarepo_cli/format/steps/format_python.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/format/wizard.py` & `oarepo-cli-11.1.2/oarepo_cli/format/wizard.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/initialize/cli.py` & `oarepo-cli-11.1.2/oarepo_cli/initialize/cli.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/initialize/steps/create_monorepo.py` & `oarepo-cli-11.1.2/oarepo_cli/initialize/steps/create_monorepo.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/initialize/steps/initialize_directory.py` & `oarepo-cli-11.1.2/oarepo_cli/initialize/steps/initialize_directory.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/initialize/steps/install_nrp_cli.py` & `oarepo-cli-11.1.2/oarepo_cli/initialize/steps/install_nrp_cli.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/initialize/wizard.py` & `oarepo-cli-11.1.2/oarepo_cli/initialize/wizard.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/kill/__init__.py` & `oarepo-cli-11.1.2/oarepo_cli/kill/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/local/add/cli.py` & `oarepo-cli-11.1.2/oarepo_cli/local/add/cli.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/local/add/steps/add_local.py` & `oarepo-cli-11.1.2/oarepo_cli/local/add/steps/add_local.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/local/remove/cli.py` & `oarepo-cli-11.1.2/oarepo_cli/local/remove/cli.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/model/__init__.py` & `oarepo-cli-11.1.2/oarepo_cli/model/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/model/add/cli.py` & `oarepo-cli-11.1.2/oarepo_cli/model/add/cli.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/model/add/steps/add_custom_fields.py` & `oarepo-cli-11.1.2/oarepo_cli/model/add/steps/add_custom_fields.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/model/add/steps/add_docs_base.py` & `oarepo-cli-11.1.2/oarepo_cli/model/add/steps/add_docs_base.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/model/add/steps/add_files.py` & `oarepo-cli-11.1.2/oarepo_cli/model/add/steps/add_files.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/model/add/steps/add_metadata.py` & `oarepo-cli-11.1.2/oarepo_cli/model/add/steps/add_metadata.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/model/add/steps/add_nr_vocabularies.py` & `oarepo-cli-11.1.2/oarepo_cli/model/add/steps/add_nr_vocabularies.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/model/add/steps/add_permissions.py` & `oarepo-cli-11.1.2/oarepo_cli/model/add/steps/add_permissions.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/model/add/steps/add_pid_type.py` & `oarepo-cli-11.1.2/oarepo_cli/model/add/steps/add_pid_type.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/model/add/steps/add_relations.py` & `oarepo-cli-11.1.2/oarepo_cli/model/add/steps/add_relations.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/model/add/steps/add_tests.py` & `oarepo-cli-11.1.2/oarepo_cli/model/add/steps/add_tests.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/model/add/steps/add_vocabularies.py` & `oarepo-cli-11.1.2/oarepo_cli/model/add/steps/add_vocabularies.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/model/add/steps/create_model.py` & `oarepo-cli-11.1.2/oarepo_cli/model/add/steps/create_model.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/model/add/wizard.py` & `oarepo-cli-11.1.2/oarepo_cli/model/add/wizard.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/model/compile/cli.py` & `oarepo-cli-11.1.2/oarepo_cli/model/compile/cli.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/model/compile/steps/compile.py` & `oarepo-cli-11.1.2/oarepo_cli/model/compile/steps/compile.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/model/compile/steps/remove_previous.py` & `oarepo-cli-11.1.2/oarepo_cli/model/compile/steps/remove_previous.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/model/gen/base.py` & `oarepo-cli-11.1.2/oarepo_cli/model/gen/base.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/model/gen/formats.py` & `oarepo-cli-11.1.2/oarepo_cli/model/gen/formats.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/model/install/cli.py` & `oarepo-cli-11.1.2/oarepo_cli/model/install/cli.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/model/install/steps/alembic.py` & `oarepo-cli-11.1.2/oarepo_cli/model/install/steps/alembic.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/model/install/steps/test_model.py` & `oarepo-cli-11.1.2/oarepo_cli/model/install/steps/test_model.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/model/install/steps/update_index.py` & `oarepo-cli-11.1.2/oarepo_cli/model/install/steps/update_index.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/model/install/wizard.py` & `oarepo-cli-11.1.2/oarepo_cli/model/install/wizard.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/model/model_support.py` & `oarepo-cli-11.1.2/oarepo_cli/model/model_support.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/model/uninstall/cli.py` & `oarepo-cli-11.1.2/oarepo_cli/model/uninstall/cli.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/model/utils.py` & `oarepo-cli-11.1.2/oarepo_cli/model/utils.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/package_versions.py` & `oarepo-cli-11.1.2/oarepo_cli/package_versions.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/run/cli.py` & `oarepo-cli-11.1.2/oarepo_cli/run/cli.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/run/steps/run_server.py` & `oarepo-cli-11.1.2/oarepo_cli/run/steps/run_server.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/site/add/cli.py` & `oarepo-cli-11.1.2/oarepo_cli/site/add/cli.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/site/add/steps/check_requirements.py` & `oarepo-cli-11.1.2/oarepo_cli/site/add/steps/check_requirements.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/site/add/steps/compile_gui.py` & `oarepo-cli-11.1.2/oarepo_cli/site/add/steps/compile_gui.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/site/add/steps/init_database.py` & `oarepo-cli-11.1.2/oarepo_cli/site/add/steps/init_database.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/site/add/steps/init_files.py` & `oarepo-cli-11.1.2/oarepo_cli/site/add/steps/init_files.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/site/add/steps/install_invenio.py` & `oarepo-cli-11.1.2/oarepo_cli/site/add/steps/install_invenio.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/site/add/steps/install_site.py` & `oarepo-cli-11.1.2/oarepo_cli/site/add/steps/install_site.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/site/add/steps/link_env.py` & `oarepo-cli-11.1.2/oarepo_cli/site/add/steps/link_env.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/site/add/steps/next_steps.py` & `oarepo-cli-11.1.2/oarepo_cli/site/add/steps/next_steps.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/site/add/steps/start_containers.py` & `oarepo-cli-11.1.2/oarepo_cli/site/add/steps/start_containers.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/site/add/wizard.py` & `oarepo-cli-11.1.2/oarepo_cli/site/add/wizard.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/site/assets.py` & `oarepo-cli-11.1.2/oarepo_cli/site/assets.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/site/site_support.py` & `oarepo-cli-11.1.2/oarepo_cli/site/site_support.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/.gitignore` & `oarepo-cli-11.1.2/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/.gitignore`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/local/README.md` & `oarepo-cli-11.1.2/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/local/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/models/README.md` & `oarepo-cli-11.1.2/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/models/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/sites/README.md` & `oarepo-cli-11.1.2/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/sites/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/ui/README.md` & `oarepo-cli-11.1.2/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/ui/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/site/LICENSE` & `oarepo-cli-11.1.2/oarepo_cli/templates/site/LICENSE`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/site/cookiecutter.json` & `oarepo-cli-11.1.2/oarepo_cli/templates/site/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/site/diffs/oarepo-to-rdm-v11.0.patch` & `oarepo-cli-11.1.2/oarepo_cli/templates/site/diffs/oarepo-to-rdm-v11.0.patch`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/site/hooks/post_gen_project.sh` & `oarepo-cli-11.1.2/oarepo_cli/templates/site/hooks/post_gen_project.sh`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/.eslintrc.json` & `oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/.eslintrc.json`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/.gitignore` & `oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/.gitignore`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/README.md` & `oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/app_data/vocabularies/affiliations_ror.yaml` & `oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/app_data/vocabularies/affiliations_ror.yaml`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/app_data/vocabularies/subjects_oecd_fos.yaml` & `oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/app_data/vocabularies/subjects_oecd_fos.yaml`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/assets/less/site/css.overrides` & `oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/assets/less/site/css.overrides`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/assets/less/theme.config` & `oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/assets/less/theme.config`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/assets/less/theme.less` & `oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/assets/less/theme.less`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/build.sh` & `oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/build.sh`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker/Dockerfile.production` & `oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker/Dockerfile.production`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker/nginx/conf.d/default.conf` & `oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker/nginx/conf.d/default.conf`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker/nginx/nginx.conf` & `oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker/nginx/nginx.conf`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker-compose.full.yml` & `oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker-compose.full.yml`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker-compose.yml` & `oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker-services.yml` & `oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker-services.yml`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/invenio.cfg` & `oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/invenio.cfg`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/setup.cfg` & `oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/setup.cfg`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/templates/semantic-ui/oarepo_ui/detail.html` & `oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/templates/semantic-ui/oarepo_ui/detail.html`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/templates/semantic-ui/oarepo_ui/footer.html` & `oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/templates/semantic-ui/oarepo_ui/footer.html`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/templates/semantic-ui/oarepo_ui/header.html` & `oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/templates/semantic-ui/oarepo_ui/header.html`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/templates/semantic-ui/{{cookiecutter.package_name}}/searchbar.html` & `oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/templates/semantic-ui/{{cookiecutter.package_name}}/searchbar.html`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/webpack.py` & `oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/webpack.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/static/images/invenio-rdm.svg` & `oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/static/images/invenio-rdm.svg`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/static/images/logo-invenio-white.svg` & `oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/static/images/logo-invenio-white.svg`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/variables` & `oarepo-cli-11.1.2/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/variables`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/ui/cookiecutter.json` & `oarepo-cli-11.1.2/oarepo_cli/templates/ui/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/.gitignore` & `oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/.gitignore`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/LICENSE` & `oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/LICENSE`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/MANIFEST.in` & `oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/setup.cfg` & `oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/setup.cfg`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/ext.py` & `oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/ext.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/resources/config.py` & `oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/resources/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/templates/semantic-ui/{{cookiecutter.app_package}}/search.html` & `oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/templates/semantic-ui/{{cookiecutter.app_package}}/search.html`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/js/{{cookiecutter.app_package}}/custom-components.js` & `oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/js/{{cookiecutter.app_package}}/custom-components.js`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/js/{{cookiecutter.app_package}}/search/components/EmptyResultsElement.jsx` & `oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/js/{{cookiecutter.app_package}}/search/components/EmptyResultsElement.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/js/{{cookiecutter.app_package}}/search/components/MultipleSearchBarElement.jsx` & `oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/js/{{cookiecutter.app_package}}/search/components/MultipleSearchBarElement.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/js/{{cookiecutter.app_package}}/search/components/ResultsGridItem.jsx` & `oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/js/{{cookiecutter.app_package}}/search/components/ResultsGridItem.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/js/{{cookiecutter.app_package}}/search/components/ResultsListItem.jsx` & `oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/js/{{cookiecutter.app_package}}/search/components/ResultsListItem.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/js/{{cookiecutter.app_package}}/search/index.js` & `oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/js/{{cookiecutter.app_package}}/search/index.js`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/less/{{cookiecutter.app_package}}/definitions/sample.less` & `oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/less/{{cookiecutter.app_package}}/definitions/sample.less`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/i18next-scanner.config.js` & `oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/i18next-scanner.config.js`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/i18next.js` & `oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/i18next.js`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/cs/messages.po` & `oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/cs/messages.po`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/cs/translations.json` & `oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/cs/translations.json`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/de/messages.po` & `oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/de/messages.po`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/de/translations.json` & `oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/de/translations.json`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/el/messages.po` & `oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/el/messages.po`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/el/translations.json` & `oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/el/translations.json`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/en/messages.po` & `oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/en/messages.po`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/en/translations.json` & `oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/en/translations.json`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/package.json` & `oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/package.json`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/scripts/compileCatalog.js` & `oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/scripts/compileCatalog.js`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/scripts/initCatalog.js` & `oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/scripts/initCatalog.js`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/yarn.lock` & `oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/yarn.lock`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/webpack.py` & `oarepo-cli-11.1.2/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/webpack.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/ui/add/cli.py` & `oarepo-cli-11.1.2/oarepo_cli/ui/add/cli.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/ui/add/mixins.py` & `oarepo-cli-11.1.2/oarepo_cli/ui/add/mixins.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/ui/add/steps/add_ui.py` & `oarepo-cli-11.1.2/oarepo_cli/ui/add/steps/add_ui.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/ui/add/steps/jinja.py` & `oarepo-cli-11.1.2/oarepo_cli/ui/add/steps/jinja.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/ui/add/wizard.py` & `oarepo-cli-11.1.2/oarepo_cli/ui/add/wizard.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/ui/install/cli.py` & `oarepo-cli-11.1.2/oarepo_cli/ui/install/cli.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/ui/install/wizard.py` & `oarepo-cli-11.1.2/oarepo_cli/ui/install/wizard.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/ui/uninstall/cli.py` & `oarepo-cli-11.1.2/oarepo_cli/ui/uninstall/cli.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/upgrade/cli.py` & `oarepo-cli-11.1.2/oarepo_cli/upgrade/cli.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/upgrade/steps/upgrade_nrp.py` & `oarepo-cli-11.1.2/oarepo_cli/upgrade/steps/upgrade_nrp.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/upgrade/steps/upgrade_site.py` & `oarepo-cli-11.1.2/oarepo_cli/upgrade/steps/upgrade_site.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/upgrade/wizard.py` & `oarepo-cli-11.1.2/oarepo_cli/upgrade/wizard.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/utils.py` & `oarepo-cli-11.1.2/oarepo_cli/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,25 +199,32 @@
     return cookiecutter_path, cookiecutter_branch
 
 
 def commit_git(repo_dir, tag_name, message):
     if "DOCKER_AROUND" in os.environ:
         return
     tag_index = 1
+
+    if not (repo_dir / '.git').exists():
+        git.Repo.init(repo_dir)
+
     try:
         for commit in pydriller.Repository(str(repo_dir)).traverse_commits():
             for m in commit.msg.split("\n"):
                 if m.startswith("omb-"):
                     tag_index += 1
     except git.exc.GitCommandError:
         pass
+    except git.exc.InvalidGitRepositoryError:
+        pass
+
     repo = git.Repo(repo_dir)
     tag_name = f"omb-{tag_index:05d}-{tag_name}"
-    index = repo.index
     repo.git.add(repo_dir)
+    index = repo.index
     if index.entries:
         index.commit(message + "\n\n" + tag_name)
 
 
 def must_be_committed(repo_dir):
     if "DOCKER_AROUND" in os.environ:
         return
```

### Comparing `oarepo-cli-11.1.1/oarepo_cli/watch/cli.py` & `oarepo-cli-11.1.2/oarepo_cli/watch/cli.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/watch/steps/watcher_step.py` & `oarepo-cli-11.1.2/oarepo_cli/watch/steps/watcher_step.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/wizard/base.py` & `oarepo-cli-11.1.2/oarepo_cli/wizard/base.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/wizard/docker.py` & `oarepo-cli-11.1.2/oarepo_cli/wizard/docker.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/wizard/steps.py` & `oarepo-cli-11.1.2/oarepo_cli/wizard/steps.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli/wizard/wizard.py` & `oarepo-cli-11.1.2/oarepo_cli/wizard/wizard.py`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/oarepo_cli.egg-info/PKG-INFO` & `oarepo-cli-11.1.2/oarepo_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-cli
-Version: 11.1.1
+Version: 11.1.2
 Summary: Utilities for managing invenio monorepo
 Description-Content-Type: text/markdown
 
 # oarepo-cli
 
 Work in progress.
```

### Comparing `oarepo-cli-11.1.1/oarepo_cli.egg-info/SOURCES.txt` & `oarepo-cli-11.1.2/oarepo_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oarepo-cli-11.1.1/setup.cfg` & `oarepo-cli-11.1.2/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-cli
-version = 11.1.1
+version = 11.1.2
 description = Utilities for managing invenio monorepo
 authors = Miroslav Simek <simeki@vscht.cz>
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
```

