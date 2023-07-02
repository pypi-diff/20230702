# Comparing `tmp/oarepo-cli-11.0.8.tar.gz` & `tmp/oarepo-cli-11.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-cli-11.0.8.tar", last modified: Fri Feb 24 09:15:57 2023, max compression
+gzip compressed data, was "oarepo-cli-11.1.0.tar", last modified: Sun Jul  2 09:34:36 2023, max compression
```

## Comparing `oarepo-cli-11.0.8.tar` & `oarepo-cli-11.1.0.tar`

### file list

```diff
@@ -1,81 +1,396 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:15:57.809679 oarepo-cli-11.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-02-24 09:15:57.809679 oarepo-cli-11.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:15:57.797679 oarepo-cli-11.0.8/oarepo_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:15:57.801679 oarepo-cli-11.0.8/oarepo_cli/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:15:57.801679 oarepo-cli-11.0.8/oarepo_cli/cli/initialize/
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/initialize/step_01_initialize_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/initialize/step_02_deployment_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/initialize/step_03_create_monorepo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/initialize/step_04_install_invenio_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/initialize/step_05_install_oarepo_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/initialize/step_06_primary_site_name.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:15:57.801679 oarepo-cli-11.0.8/oarepo_cli/cli/model/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/model/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/model/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/model/install.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/model/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/model/load.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/model/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:15:57.805679 oarepo-cli-11.0.8/oarepo_cli/cli/run/
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/run/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:15:57.805679 oarepo-cli-11.0.8/oarepo_cli/cli/site/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/site/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/site/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/site/step_01_install_site.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/site/step_02_check_requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/site/step_03_fixup_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/site/step_04_start_containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/site/step_05_create_pipenv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/site/step_06_install_invenio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/site/step_07_init_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/site/step_08_next_steps.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/site/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:15:57.805679 oarepo-cli-11.0.8/oarepo_cli/cli/ui/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/ui/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/ui/install.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/ui/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     8979 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:15:57.805679 oarepo-cli-11.0.8/oarepo_cli/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:15:57.805679 oarepo-cli-11.0.8/oarepo_cli/templates/repo/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/templates/repo/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:15:57.809679 oarepo-cli-11.0.8/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:15:57.809679 oarepo-cli-11.0.8/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/.bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      234 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/.bin/cookiecutter
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/.bin/readme.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/.envrc
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      676 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/invenio-cli
--rwxr-xr-x   0 runner    (1001) docker     (123)      261 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/nrp-cli
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:15:57.809679 oarepo-cli-11.0.8/oarepo_cli/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/ui/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/ui/radio.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/ui/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/ui/widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:15:57.809679 oarepo-cli-11.0.8/oarepo_cli/ui/wizard/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/ui/wizard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/ui/wizard/steps.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/ui/wizard/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/ui/wizard/wizard.py
--rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/oarepo_cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:15:57.801679 oarepo-cli-11.0.8/oarepo_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-02-24 09:15:57.000000 oarepo-cli-11.0.8/oarepo_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-02-24 09:15:57.000000 oarepo-cli-11.0.8/oarepo_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 09:15:57.000000 oarepo-cli-11.0.8/oarepo_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-24 09:15:57.000000 oarepo-cli-11.0.8/oarepo_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-02-24 09:15:57.000000 oarepo-cli-11.0.8/oarepo_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-24 09:15:57.000000 oarepo-cli-11.0.8/oarepo_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-02-24 09:15:57.809679 oarepo-cli-11.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-24 09:15:52.000000 oarepo-cli-11.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.696000 oarepo-cli-11.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-07-02 09:34:36.696000 oarepo-cli-11.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.627999 oarepo-cli-11.1.0/oarepo_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.631999 oarepo-cli-11.1.0/oarepo_cli/develop/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/develop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/develop/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/develop/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/develop/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.631999 oarepo-cli-11.1.0/oarepo_cli/develop/runners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/develop/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/develop/runners/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/develop/runners/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.631999 oarepo-cli-11.1.0/oarepo_cli/develop/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/develop/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/develop/steps/check_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/develop/steps/check_s3_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/develop/steps/check_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/develop/steps/check_site.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/develop/steps/check_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/develop/steps/check_venv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/develop/steps/develop_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/develop/wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.631999 oarepo-cli-11.1.0/oarepo_cli/format/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/format/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/format/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.631999 oarepo-cli-11.1.0/oarepo_cli/format/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/format/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/format/steps/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/format/steps/format_javascript.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/format/steps/format_jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/format/steps/format_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/format/wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.635999 oarepo-cli-11.1.0/oarepo_cli/initialize/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/initialize/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.635999 oarepo-cli-11.1.0/oarepo_cli/initialize/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/initialize/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/initialize/steps/create_monorepo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/initialize/steps/initialize_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/initialize/steps/install_nrp_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/initialize/wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.635999 oarepo-cli-11.1.0/oarepo_cli/kill/
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/kill/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.635999 oarepo-cli-11.1.0/oarepo_cli/local/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/local/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.635999 oarepo-cli-11.1.0/oarepo_cli/local/add/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/local/add/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/local/add/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.635999 oarepo-cli-11.1.0/oarepo_cli/local/add/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/local/add/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/local/add/steps/add_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/local/add/steps/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/local/add/wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.635999 oarepo-cli-11.1.0/oarepo_cli/local/remove/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/local/remove/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/local/remove/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.635999 oarepo-cli-11.1.0/oarepo_cli/local/remove/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/local/remove/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/local/remove/steps/uninstall.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/local/remove/wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.635999 oarepo-cli-11.1.0/oarepo_cli/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.635999 oarepo-cli-11.1.0/oarepo_cli/model/add/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/model/add/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/model/add/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.639999 oarepo-cli-11.1.0/oarepo_cli/model/add/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/model/add/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/model/add/steps/add_custom_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/model/add/steps/add_docs_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/model/add/steps/add_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/model/add/steps/add_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/model/add/steps/add_nr_vocabularies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/model/add/steps/add_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/model/add/steps/add_pid_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/model/add/steps/add_relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/model/add/steps/add_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/model/add/steps/add_vocabularies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/model/add/steps/create_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/model/add/wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.639999 oarepo-cli-11.1.0/oarepo_cli/model/compile/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/model/compile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/model/compile/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.639999 oarepo-cli-11.1.0/oarepo_cli/model/compile/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/model/compile/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/model/compile/steps/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/model/compile/steps/remove_previous.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/model/compile/wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.639999 oarepo-cli-11.1.0/oarepo_cli/model/gen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/model/gen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/model/gen/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/model/gen/formats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.639999 oarepo-cli-11.1.0/oarepo_cli/model/install/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/model/install/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/model/install/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.639999 oarepo-cli-11.1.0/oarepo_cli/model/install/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/model/install/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/model/install/steps/alembic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/model/install/steps/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/model/install/steps/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/model/install/steps/update_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/model/install/wizard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/model/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/model/model_support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.643999 oarepo-cli-11.1.0/oarepo_cli/model/uninstall/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/model/uninstall/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/model/uninstall/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.643999 oarepo-cli-11.1.0/oarepo_cli/model/uninstall/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/model/uninstall/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/model/uninstall/steps/uninstall.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/model/uninstall/wizard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/package_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.643999 oarepo-cli-11.1.0/oarepo_cli/run/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/run/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.643999 oarepo-cli-11.1.0/oarepo_cli/run/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/run/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/run/steps/run_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/run/wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.643999 oarepo-cli-11.1.0/oarepo_cli/site/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/site/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.643999 oarepo-cli-11.1.0/oarepo_cli/site/add/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/site/add/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/site/add/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.643999 oarepo-cli-11.1.0/oarepo_cli/site/add/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/site/add/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/site/add/steps/check_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/site/add/steps/compile_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/site/add/steps/init_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/site/add/steps/init_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/site/add/steps/install_invenio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/site/add/steps/install_site.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/site/add/steps/link_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/site/add/steps/next_steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/site/add/steps/resolve_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/site/add/steps/start_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/site/add/wizard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/site/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/site/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/site/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18674 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/site/site_support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.647999 oarepo-cli-11.1.0/oarepo_cli/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.647999 oarepo-cli-11.1.0/oarepo_cli/templates/repo/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/repo/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.647999 oarepo-cli-11.1.0/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/.envrc
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.647999 oarepo-cli-11.1.0/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/local/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/local/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/local/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.647999 oarepo-cli-11.1.0/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/models/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      337 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/nrp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.647999 oarepo-cli-11.1.0/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/sites/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/sites/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.647999 oarepo-cli-11.1.0/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/ui/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.647999 oarepo-cli-11.1.0/oarepo_cli/templates/site/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.647999 oarepo-cli-11.1.0/oarepo_cli/templates/site/diffs/
+-rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/diffs/oarepo-to-rdm-v11.0.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.647999 oarepo-cli-11.1.0/oarepo_cli/templates/site/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/hooks/post_gen_project.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.647999 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/.envrc
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/.eslintrc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.647999 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/app_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/app_data/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.651999 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/app_data/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/app_data/pages/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.675999 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/app_data/vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (123) 19635835 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/app_data/vocabularies/affiliations_ror.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/app_data/vocabularies/subjects_oecd_fos.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/app_data/vocabularies.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.619999 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.675999 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/assets/less/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.675999 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/assets/less/site/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/assets/less/site/css.overrides
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.679999 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/assets/less/site/globals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/assets/less/site/globals/site.overrides
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/assets/less/site/globals/site.variables
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/assets/less/theme.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/assets/less/theme.less
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.679999 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/assets/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/assets/templates/.readme
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.679999 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/assets/templates/custom_fields/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/assets/templates/custom_fields/.readme
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/build.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.679999 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker/Dockerfile.production
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.679999 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker/nginx/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker/nginx/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.679999 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker/nginx/conf.d/
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker/nginx/conf.d/default.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker/nginx/nginx.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.679999 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker/pgadmin/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker/pgadmin/servers.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.679999 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker/uwsgi/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker/uwsgi/uwsgi.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker-compose.full.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/docker-services.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/invenio.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/prettierrc.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.679999 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.679999 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/tests/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.679999 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.623999 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.623999 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/assets/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.623999 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/assets/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.679999 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/assets/semantic-ui/js/{{cookiecutter.package_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/assets/semantic-ui/js/{{cookiecutter.package_name}}/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.623999 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/assets/semantic-ui/less/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.679999 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/assets/semantic-ui/less/{{cookiecutter.package_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/assets/semantic-ui/less/{{cookiecutter.package_name}}/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.623999 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.623999 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.679999 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/templates/semantic-ui/oarepo_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/templates/semantic-ui/oarepo_ui/detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/templates/semantic-ui/oarepo_ui/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/templates/semantic-ui/oarepo_ui/header.html
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/templates/semantic-ui/oarepo_ui/javascript.html
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/templates/semantic-ui/oarepo_ui/trackingcode.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.679999 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/templates/semantic-ui/{{cookiecutter.package_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/templates/semantic-ui/{{cookiecutter.package_name}}/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/templates/semantic-ui/{{cookiecutter.package_name}}/frontpage.html
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/templates/semantic-ui/{{cookiecutter.package_name}}/searchbar.html
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/site/{{cookiecutter.package_name}}/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.679999 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.684000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/static/images/invenio-rdm.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/static/images/logo-invenio-white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/static/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.623999 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.684000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/templates/semantic-ui/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/templates/semantic-ui/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.684000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/translations/babel.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/site/{{cookiecutter.project_shortname}}/variables
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.684000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/cookiecutter.json
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/local_extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.684000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.684000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.684000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/resources/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/resources/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.623999 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.623999 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.684000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/templates/semantic-ui/{{cookiecutter.app_package}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/templates/semantic-ui/{{cookiecutter.app_package}}/detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/templates/semantic-ui/{{cookiecutter.app_package}}/main.html
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/templates/semantic-ui/{{cookiecutter.app_package}}/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/templates/semantic-ui/{{cookiecutter.app_package}}/sidebar.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.684000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.623999 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.684000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.623999 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.684000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/js/{{cookiecutter.app_package}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/js/{{cookiecutter.app_package}}/custom-components.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.684000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/js/{{cookiecutter.app_package}}/search/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.688000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/js/{{cookiecutter.app_package}}/search/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/js/{{cookiecutter.app_package}}/search/components/EmptyResultsElement.jsx
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/js/{{cookiecutter.app_package}}/search/components/MultipleSearchBarElement.jsx
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/js/{{cookiecutter.app_package}}/search/components/ResultsGridItem.jsx
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/js/{{cookiecutter.app_package}}/search/components/ResultsListItem.jsx
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/js/{{cookiecutter.app_package}}/search/components/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/js/{{cookiecutter.app_package}}/search/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.623999 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/less/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.688000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/less/{{cookiecutter.app_package}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/less/{{cookiecutter.app_package}}/custom-components.less
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.688000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/less/{{cookiecutter.app_package}}/definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/less/{{cookiecutter.app_package}}/definitions/sample.less
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.623999 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/less/{{cookiecutter.app_package}}/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.688000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/less/{{cookiecutter.app_package}}/theme/elements/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/less/{{cookiecutter.app_package}}/theme/elements/sample.overrides
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/less/{{cookiecutter.app_package}}/theme/elements/sample.variables
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.627999 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.688000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/i18next-scanner.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/i18next.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.688000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.688000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/cs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/cs/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/cs/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.688000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/de/
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/de/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/de/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.688000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/el/
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/el/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/el/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.688000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/en/
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/en/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/en/translations.json
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/messages/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.688000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/scripts/compileCatalog.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)      351 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/scripts/compileLanguages.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/scripts/initCatalog.js
+-rw-r--r--   0 runner    (1001) docker     (123)    41082 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/assets/semantic-ui/translations/{{cookiecutter.app_package}}/yarn.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/theme/webpack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/templates/ui/{{cookiecutter.app_name}}/{{cookiecutter.app_package}}/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.688000 oarepo-cli-11.1.0/oarepo_cli/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.692000 oarepo-cli-11.1.0/oarepo_cli/ui/add/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/ui/add/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/ui/add/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/ui/add/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.692000 oarepo-cli-11.1.0/oarepo_cli/ui/add/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/ui/add/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/ui/add/steps/add_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/ui/add/steps/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/ui/add/wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.692000 oarepo-cli-11.1.0/oarepo_cli/ui/install/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/ui/install/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/ui/install/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.692000 oarepo-cli-11.1.0/oarepo_cli/ui/install/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/ui/install/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/ui/install/steps/build_assets_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/ui/install/steps/install_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/ui/install/wizard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/ui/list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.692000 oarepo-cli-11.1.0/oarepo_cli/ui/uninstall/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/ui/uninstall/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/ui/uninstall/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.692000 oarepo-cli-11.1.0/oarepo_cli/ui/uninstall/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/ui/uninstall/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/ui/uninstall/steps/uninstall.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/ui/uninstall/wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.692000 oarepo-cli-11.1.0/oarepo_cli/upgrade/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/upgrade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/upgrade/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.692000 oarepo-cli-11.1.0/oarepo_cli/upgrade/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/upgrade/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/upgrade/steps/upgrade_docker_nrp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/upgrade/steps/upgrade_nrp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/upgrade/steps/upgrade_site.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/upgrade/wizard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19458 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.692000 oarepo-cli-11.1.0/oarepo_cli/watch/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/watch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/watch/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.692000 oarepo-cli-11.1.0/oarepo_cli/watch/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/watch/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/watch/steps/watcher_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/watch/wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.696000 oarepo-cli-11.1.0/oarepo_cli/wizard/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/wizard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/wizard/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/wizard/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/wizard/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/oarepo_cli/wizard/wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:34:36.631999 oarepo-cli-11.1.0/oarepo_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-07-02 09:34:36.000000 oarepo-cli-11.1.0/oarepo_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18351 2023-07-02 09:34:36.000000 oarepo-cli-11.1.0/oarepo_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 09:34:36.000000 oarepo-cli-11.1.0/oarepo_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-02 09:34:36.000000 oarepo-cli-11.1.0/oarepo_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-02 09:34:36.000000 oarepo-cli-11.1.0/oarepo_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-02 09:34:36.000000 oarepo-cli-11.1.0/oarepo_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-02 09:34:36.696000 oarepo-cli-11.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-02 09:34:30.000000 oarepo-cli-11.1.0/setup.py
```

### Comparing `oarepo-cli-11.0.8/PKG-INFO` & `oarepo-cli-11.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-Metadata-Version: 2.1
-Name: oarepo-cli
-Version: 11.0.8
-Summary: Utilities for managing invenio monorepo
-Description-Content-Type: text/markdown
-
 # oarepo-cli
 
 Work in progress.
 
 ## Repository project initialization
 
 Download the file from
```

### Comparing `oarepo-cli-11.0.8/README.md` & `oarepo-cli-11.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+Metadata-Version: 2.1
+Name: oarepo-cli
+Version: 11.1.0
+Summary: Utilities for managing invenio monorepo
+Description-Content-Type: text/markdown
+
 # oarepo-cli
 
 Work in progress.
 
 ## Repository project initialization
 
 Download the file from
```

### Comparing `oarepo-cli-11.0.8/oarepo_cli/cli/initialize/step_01_initialize_directory.py` & `oarepo-cli-11.1.0/oarepo_cli/initialize/steps/initialize_directory.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import logging
+import sys
 
-from oarepo_cli.ui.wizard import WizardStep
-from oarepo_cli.utils import to_python_name
+from colorama import Fore, Style
 from git import Repo
 
-log = logging.getLogger("step_01_initialize_directory")
+from oarepo_cli.utils import to_python_name
+from oarepo_cli.wizard import WizardStep
 
+log = logging.getLogger("step_01_initialize_directory")
 
-class DirectoryStep(WizardStep):
-    def __init__(self, *args, **kwargs):
-        super().__init__(heading="Creating the target directory ...")
 
+class MonorepoDirectoryStep(WizardStep):
     def after_run(self):
         self.data["project_package"] = to_python_name(self.data.project_dir.name)
         p = self.data.project_dir
         if not p.exists():
+            print(f"{Fore.BLUE}Creating {Style.RESET_ALL} {p}", file=sys.__stderr__)
             p.mkdir(parents=True)
         if not (p / ".git").exists():
             Repo.init(p)
 
     def should_run(self):
-        return True
+        return not self.data.project_dir.exists()
```

### Comparing `oarepo-cli-11.0.8/oarepo_cli/cli/initialize/step_03_create_monorepo.py` & `oarepo-cli-11.1.0/oarepo_cli/initialize/steps/create_monorepo.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,27 @@
 import os
 import shutil
 from pathlib import Path
 
-from oarepo_cli.cli.utils import ProjectWizardMixin
 from oarepo_cli.templates import get_cookiecutter_template
-from oarepo_cli.ui.wizard import WizardStep
-
-from oarepo_cli.utils import commit_git
+from oarepo_cli.utils import ProjectWizardMixin, commit_git
+from oarepo_cli.wizard import WizardStep
 
 
 def keep_existing_copy(src, dst, *, follow_symlinks=True):
     if os.path.isdir(dst):
         _dst = os.path.join(dst, os.path.basename(src))
     else:
         _dst = dst
     if Path(_dst).exists():
         return _dst
     return shutil.copy2(src, dst, follow_symlinks=follow_symlinks)
 
 
 class CreateMonorepoStep(ProjectWizardMixin, WizardStep):
-    def __init__(self, **kwargs):
-        super().__init__(
-            heading="Now I will create the monorepo inside the selected directory.",
-            **kwargs
-        )
-
     def after_run(self):
         project_dir, repo_name, repo_out = self._repo_params
         self.run_cookiecutter(
             template=get_cookiecutter_template("repo"),
             config_file="monorepo",
             output_dir=str(repo_out),
             extra_context={
@@ -54,8 +46,8 @@
         project_dir = self.data.project_dir
         repo_name = project_dir.name
         repo_out = project_dir.parent / (project_dir.name + "-tmp")
         return project_dir, repo_name, repo_out
 
     def should_run(self):
         project_dir, repo_name, repo_out = self._repo_params
-        return not (project_dir / "invenio-cli").exists()
+        return not (project_dir / "nrp-cli").exists()
```

### Comparing `oarepo-cli-11.0.8/oarepo_cli/cli/site/add.py` & `oarepo-cli-11.1.0/oarepo_cli/model/install/cli.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,49 +1,58 @@
-import click
+import click as click
 
-from oarepo_cli.cli.utils import with_config
+from oarepo_cli.utils import commit_git, with_config
 
-from ...ui.wizard import Wizard
-from ...utils import commit_git, to_python_name
-from .step_01_install_site import InstallSiteStep
-from .step_02_check_requirements import CheckRequirementsStep
-from .step_03_fixup_code import FixupSiteCodeStep
-from .step_04_start_containers import StartContainersStep
-from .step_05_create_pipenv import CreatePipenvStep
-from .step_06_install_invenio import InstallInvenioStep
-from .step_07_init_database import InitDatabaseStep
-from .step_08_next_steps import NextStepsStep
+from ...site.site_support import SiteSupport
+from ...wizard.docker import DockerRunner
+from ..model_support import ModelSupport
+from .wizard import InstallModelWizard
 
 
 @click.command(
-    name="add",
-    help="""Generate a new site.  Required arguments:
-    <name>   ... name of the site. The recommended pattern for it is <something>-site""",
+    name="install",
+    help="""
+Install the model into the current site. Required arguments:
+    <name>   ... name of the already existing model""",
 )
-@click.argument("name")
-@with_config(config_section=lambda name, **kwargs: ["sites", name])
-@click.pass_context
-def add_site(ctx, cfg=None, name=None, **kwargs):
+@click.argument("name", required=True)
+@click.argument("site_name", required=False)
+@with_config(config_section=lambda name, **kwargs: ["models", name])
+def install_model(
+    cfg=None,
+    no_input=False,
+    silent=False,
+    step=None,
+    steps=False,
+    verbose=False,
+    site_name=None,
+    **kwargs,
+):
     commit_git(
         cfg.project_dir,
-        f"before-site-install-{cfg.section}",
-        f"Committed automatically before site {cfg.section} has been added",
+        f"before-model-install-{cfg.section}",
+        f"Committed automatically before model {cfg.section} has been installed",
     )
-    cfg["site_package"] = to_python_name(name)
-    cfg["site_dir"] = f"sites/{name}"
+    site_support = SiteSupport(cfg, site_name)
 
-    initialize_wizard = Wizard(
-        InstallSiteStep(pause=True),
-        CheckRequirementsStep(),
-        FixupSiteCodeStep(),
-        StartContainersStep(pause=True),
-        CreatePipenvStep(),
-        InstallInvenioStep(pause=True),
-        InitDatabaseStep(),
-        NextStepsStep(pause=True),
+    model_sites = cfg.setdefault("sites", [])
+    if site_support.site_name not in model_sites:
+        model_sites.append(site_support.site_name)
+    cfg.save()
+
+    runner = DockerRunner(cfg, no_input)
+    wizard = InstallModelWizard(
+        runner, model_support=ModelSupport(cfg), site_support=site_support
+    )
+
+    if steps:
+        wizard.list_steps()
+        return
+
+    wizard.run_wizard(
+        cfg, no_input=no_input, silent=silent, selected_steps=step, verbose=verbose
     )
-    initialize_wizard.run(cfg)
     commit_git(
         cfg.project_dir,
-        f"after-site-install-{cfg.section}",
-        f"Committed automatically after site {cfg.section} has been added",
+        f"after-model-install-{cfg.section}",
+        f"Committed automatically after model {cfg.section} has been installed",
     )
```

### Comparing `oarepo-cli-11.0.8/oarepo_cli/cli/site/step_01_install_site.py` & `oarepo-cli-11.1.0/oarepo_cli/site/add/steps/install_site.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,140 +1,109 @@
 from __future__ import annotations
 
 import datetime
 import os
 import re
 
-from oarepo_cli.cli.site.utils import SiteWizardStepMixin
-from oarepo_cli.ui.wizard import StaticWizardStep, WizardStep
-from oarepo_cli.ui.wizard.steps import InputWizardStep, RadioWizardStep
+from oarepo_cli.site.mixins import SiteWizardStepMixin
+from oarepo_cli.templates import get_cookiecutter_template
+from oarepo_cli.utils import ProjectWizardMixin, commit_git
+from oarepo_cli.wizard import InputStep, RadioStep, StaticStep, WizardStep
 
-from ...utils import commit_git, get_cookiecutter_source, run_cmdline
 
-
-class InstallSiteStep(SiteWizardStepMixin, WizardStep):
+class InstallSiteStep(SiteWizardStepMixin, ProjectWizardMixin, WizardStep):
     def __init__(self, **kwargs):
         super().__init__(
-            heading="""
-Now I will add site sources, that can be used to change the overall CSS style and
-configure your repository. Please fill in the following values. 
-If not sure, keep the default values.""",
-            **kwargs,
-        )
-
-    def get_steps(self):
-        self.data.setdefault(
-            "transifex_project", self.data.get("config.project_package", "")
-        )
-        # substeps of this step
-        site_dir_name = self.site_dir.name
-        return [
-            InputWizardStep(
+            InputStep(
                 "repository_name",
                 prompt="""Enter the repository name ("title" of the HTML site)""",
-                default=re.sub("[_-]", " ", site_dir_name).title(),
+                default=lambda data: re.sub("[_-]", " ", self.site_dir.name).title(),
             ),
-            InputWizardStep(
+            InputStep(
                 "www",
                 prompt="""Enter the WWW address on which the repository will reside""",
             ),
-            InputWizardStep(
+            InputStep(
                 "author_name",
                 prompt="""Author name""",
                 default=os.environ.get("USERNAME") or os.environ.get("USER"),
             ),
-            InputWizardStep("author_email", prompt="""Author email"""),
-            InputWizardStep(
+            InputStep("author_email", prompt="""Author email"""),
+            InputStep(
                 "year",
                 prompt="""Year (for copyright)""",
                 default=datetime.datetime.today().strftime("%Y"),
             ),
-            InputWizardStep("copyright_holder", prompt="""Copyright holder"""),
-            RadioWizardStep(
+            InputStep("copyright_holder", prompt="""Copyright holder"""),
+            RadioStep(
                 "use_oarepo_vocabularies",
                 options={"yes": "Yes", "no": "No"},
                 default="yes",
                 heading=f"""
-            Are you planning to use extended vocabularies (extra fields on vocabularies, hierarchy in vocabulary items)? If in doubt, select 'yes'.
-                """,
+                    Are you planning to use extended vocabularies (extra fields on vocabularies, hierarchy in vocabulary items)? If in doubt, select 'yes'.
+                        """,
             ),
-            StaticWizardStep(
+            StaticStep(
                 heading="""I have all the information to generate the site.
-To do so, I'll call the invenio client. If anything goes wrong, please fix the problem
-and run the wizard again.
-            """,
+        To do so, I'll call the cookiecutter to install the size template. If anything goes wrong, please fix the problem
+        and run the wizard again.
+                    """,
             ),
-        ]
+            heading="""
+Now I will add site sources, that can be used to change the overall CSS style and
+configure your repository. Please fill in the required values. 
+If not sure, keep the default values.""",
+            **kwargs,
+        )
+
+    def on_before_run(self):
+        self.data.setdefault(
+            "transifex_project", self.data.get("config.project_package", "")
+        )
+        return True
 
     def after_run(self):
-        # create site config for invenio-cli
-        cookiecutter_config_file = self.data.project_dir / ".invenio"
+        site_name = self.site_dir.name
         site_dir = self.site_dir
         if not site_dir.parent.exists():
             site_dir.parent.mkdir(parents=True)
 
-        with open(cookiecutter_config_file, "w") as f:
-            print(
-                f"""
-[cookiecutter]
-project_name = {self.data['repository_name']}
-project_shortname = {self.site_dir.name}
-project_site = {self.data['www']}
-github_repo = 
-description = {self.data['repository_name']} OARepo Instance
-author_name = {self.data['author_name']}
-author_email = {self.data['author_email']}
-year = {self.data['year']}
-python_version = 3.9
-database = postgresql
-search = opensearch2
-file_storage = S3
-development_tools = yes
-site_code = yes
-use_oarepo_vocabularies = {self.data['use_oarepo_vocabularies']}
-                """,
-                file=f,
-            )
-        # and run invenio-cli with our site template
-        # (submodule from https://github.com/oarepo/cookiecutter-oarepo-instance)
-
-        cookiecutter_path, cookiecutter_branch = get_cookiecutter_source(
-            "OAREPO_SITE_COOKIECUTTER_VERSION",
-            "https://github.com/oarepo/cookiecutter-site",
-            "v11.0",
-            master_version="master",
+        self.run_cookiecutter(
+            template=get_cookiecutter_template("site"),
+            config_file=f"site-{site_name}",
+            output_dir=str(site_dir.parent),
+            extra_context=dict(
+                project_name=self.data["repository_name"],
+                project_shortname=self.site_dir.name,
+                project_site=self.data["www"],
+                jsonschemas_host=get_host_name(self.data["www"]),
+                github_repo="",
+                description=f"{self.data['repository_name']} OARepo Instance",
+                author_name=self.data["author_name"],
+                author_email=self.data["author_email"],
+                year=self.data["year"],
+                python_version="3.9",
+                database="postgresql",
+                search="opensearch2",
+                file_storage="S3",
+                development_tools="yes",
+                site_code="yes",
+                use_oarepo_vocabularies=self.data["use_oarepo_vocabularies"],
+            ),
         )
 
-        run_cmdline(
-            self.data.project_dir / self.data.get("config.invenio_cli"),
-            "init",
-            "rdm",
-            "-t",
-            cookiecutter_path,
-            *(
-                [
-                    "-c",
-                    cookiecutter_branch,
-                ]
-                if cookiecutter_branch
-                else []
-            ),
-            "--no-input",
-            "--config",
-            str(cookiecutter_config_file),
-            cwd=self.data.project_dir / "sites",
-            environ={
-                "PIPENV_IGNORE_VIRTUALENVS": "1",
-                # use our own cookiecutter, not the system one
-                "PATH": f"{self.data.get('config.project_dir')}/.bin:{os.environ['PATH']}",
-            },
-        )
-        with open(self.site_dir / ".check.ok", "w") as f:
-            f.write("oarepo check ok")
         commit_git(
             self.data.project_dir,
             f"after-site-cookiecutter-{self.data.section}",
             f"Committed automatically after site {self.data.section} cookiecutter has been called",
         )
 
     def should_run(self):
-        return not (self.site_dir / ".check.ok").exists()
+        return not (self.site_dir / "variables").exists()
+
+
+def get_host_name(url):
+    if url.startswith("http://"):
+        url = url[7:]
+    if url.startswith("https://"):
+        url = url[8:]
+    return url.split("/", maxsplit=1)[0]
```

### Comparing `oarepo-cli-11.0.8/oarepo_cli/cli/site/step_06_install_invenio.py` & `oarepo-cli-11.1.0/oarepo_cli/initialize/steps/install_nrp_cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,62 +1,50 @@
-from oarepo_cli.cli.site.utils import SiteWizardStepMixin
-from oarepo_cli.ui.wizard import WizardStep
+from __future__ import annotations
 
-from ...utils import commit_git, run_cmdline
+import shutil
+import venv
 
+from oarepo_cli.package_versions import NRP_CLI_VERSION
+from oarepo_cli.utils import commit_git, pip_install
+from oarepo_cli.wizard import WizardStep
 
-class InstallInvenioStep(SiteWizardStepMixin, WizardStep):
+
+class InstallINRPCliStep(WizardStep):
     def __init__(self, **kwargs):
         super().__init__(
             heading="""
-Now I'll install invenio site.
-
-Note that this can take a lot of time as UI dependencies
-will be downloaded and installed and UI will be compiled.
+I will install nrp command-line tools that make using the invenio easier.
+To run them, invoke the "nrp-cli" script from within the project directory.            
             """,
             **kwargs,
         )
 
     def after_run(self):
-        run_cmdline(
-            self.data.project_dir / self.data.get("config.invenio_cli"),
-            "install",
-            cwd=self.site_dir,
-            environ={"PIPENV_IGNORE_VIRTUALENVS": "1"},
+        print("Creating nrp-cli virtualenv")
+        self.data["oarepo_cli"] = str(
+            (self.nrp_cli_dir / "bin" / "nrp-cli").relative_to(self.data.project_dir)
+        )
+        if self.nrp_cli_dir.exists():
+            shutil.rmtree(self.nrp_cli_dir)
+        venv.main([str(self.nrp_cli_dir)])
+
+        pip_install(
+            self.nrp_cli_dir / "bin" / "pip",
+            "NRP_CLI_VERSION",
+            NRP_CLI_VERSION,
+            "https://github.com/oarepo/oarepo-cli",
         )
-        if not self._manifest_file.exists():
-            raise FileNotFoundError(
-                "invenio-cli install has not created var/instance/static/dist/manifest.json."
-                "Please check the output, correct errors and run this command again"
-            )
+
+        with open(self.nrp_cli_dir / ".check.ok", "w") as f:
+            f.write("oarepo check ok")
         commit_git(
             self.data.project_dir,
-            f"after-site-invenio-cli-install-{self.data.section}",
-            f"Committed automatically after site {self.data.section} has been installed",
+            "after-install-oarepo-cli",
+            "Committed automatically after oarepo-cli has been installed",
         )
 
     @property
-    def _pipenv_venv_dir(self):
-        success = run_cmdline(
-            "pipenv",
-            "--venv",
-            cwd=self.site_dir,
-            environ={"PIPENV_IGNORE_VIRTUALENVS": "1"},
-            check_only=True,
-            grab_stdout=True,
-        )
-        if not success:
-            return None
-        return success.strip()
+    def nrp_cli_dir(self):
+        return self.data.project_dir / ".venv" / "nrp-cli"
 
     def should_run(self):
-        manifest_file = self._manifest_file
-        return not manifest_file.exists()
-
-    @property
-    def _manifest_file(self):
-        pipenv_dir = self.data.project_dir / self.data["site_pipenv_dir"]
-        manifest_file = (
-            pipenv_dir / "var" / "instance" / "static" / "dist" / "manifest.json"
-        )
-
-        return manifest_file
+        return not (self.nrp_cli_dir / ".check.ok").exists()
```

### Comparing `oarepo-cli-11.0.8/oarepo_cli/cli/site/step_07_init_database.py` & `oarepo-cli-11.1.0/oarepo_cli/site/add/steps/init_database.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 import re
 import subprocess
 
-from oarepo_cli.cli.site.utils import SiteWizardStepMixin
-from oarepo_cli.ui.radio import Radio
-from oarepo_cli.ui.wizard import WizardStep
-
-from ...utils import commit_git, run_cmdline
+from oarepo_cli.site.mixins import SiteWizardStepMixin
+from oarepo_cli.wizard import RadioStep, WizardStep
 
 
 class InitDatabaseStep(SiteWizardStepMixin, WizardStep):
     def __init__(self, **kwargs):
         super().__init__(
-            Radio(
+            RadioStep(
                 "init_database",
                 options={"yes": "Yes", "no": "No"},
                 default="yes",
             ),
             heading="""
 If the database has not been initialized, I can do it now - 
 this will delete all the previous data in the database.
@@ -23,35 +20,22 @@
 Should I do it?
             """,
             **kwargs,
         )
 
     def after_run(self):
         if self.data["init_database"] == "yes":
-            run_cmdline(
-                "pipenv",
-                "run",
-                "invenio",
-                "db",
-                "create",
-                cwd=self.site_dir,
-                environ={"PIPENV_IGNORE_VIRTUALENVS": "1"},
-            )
+            self.site_support.call_invenio("db", "create")
         self.check_db_initialized(raise_error=True)
 
     def check_db_initialized(self, raise_error=False):
         try:
-            output = run_cmdline(
-                "pipenv",
-                "run",
-                "invenio",
+            output = self.site_support.call_invenio(
                 "alembic",
                 "current",
-                cwd=self.site_dir,
-                environ={"PIPENV_IGNORE_VIRTUALENVS": "1"},
                 grab_stdout=True,
                 raise_exception=True,
             )
         except subprocess.CalledProcessError:
             raise Exception(
                 "Alembic initialization failed. This could mean that the database "
                 "does not exist or that there is already an incompatible alembic "
```

### Comparing `oarepo-cli-11.0.8/oarepo_cli/cli/site/step_08_next_steps.py` & `oarepo-cli-11.1.0/oarepo_cli/site/add/steps/next_steps.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from oarepo_cli.cli.site.utils import SiteWizardStepMixin
-from oarepo_cli.ui.wizard import WizardStep
+from oarepo_cli.site.mixins import SiteWizardStepMixin
+from oarepo_cli.wizard import WizardStep
 
 
 class NextStepsStep(SiteWizardStepMixin, WizardStep):
     def __init__(self, **kwargs):
         super().__init__(
             heading=lambda data: f"""
 The repository skeleton has been created and dependencies installed.
```

### Comparing `oarepo-cli-11.0.8/oarepo_cli/config.py` & `oarepo-cli-11.1.0/oarepo_cli/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -36,26 +36,30 @@
 
     def on_changed(self):
         pass
 
 
 class MonorepoConfig(Config):
     type = "monorepo"
+    running_in_docker = False
+    use_docker = False
+    no_input = False
 
     def __init__(self, path: Path, section=["config"]):
         super().__init__()
         self.path = path
         self.existing = False
         if not section:
             section = []
         elif isinstance(section, str):
             section = [section]
         self.section_path = tuple(section)
         self.whole_data = {}
         self._load_section()
+        self.readonly = False
 
     def load(self):
         with open(self.path, "r") as f:
             data = yaml.safe_load(f)
             self.whole_data = data
             self._load_section()
             self.existing = True
@@ -63,23 +67,30 @@
     def _load_section(self):
         data = self.whole_data
         for s in self.section_path:
             data = data.setdefault(s, {})
         self.config = data
 
     def save(self):
+        # import locally to prevent circular dependencies
+        if self.readonly:
+            return
+
         data = {**self.whole_data, "type": self.type}
+
         # just try to dump so that if that is not successful we do not overwrite the config
         sio = StringIO()
         yaml.safe_dump(data, sio)
 
         # and real dump here
         if self.path.parent.exists():
             with open(self.path, "w") as f:
                 f.write(sio.getvalue())
+            # and reload the changes
+            self.load()
 
     def on_changed(self):
         if self.path.parent.exists():
             self.save()
 
     def _section(self, name, default=None):
         name = name.split(".")
@@ -104,7 +115,17 @@
     def merge_config(self, config_data, top=False):
         if top:
             always_merger.merge(self.whole_data, config_data)
             self._load_section()
             self.save()
         else:
             always_merger.merge(self.config, config_data)
+
+    def __str__(self):
+        return f"MonorepoConfig[{self.config}]"
+
+    def clone(self, section_path):
+        ret = MonorepoConfig(self.path, section=section_path)
+        ret.running_in_docker = self.running_in_docker
+        ret.use_docker = self.use_docker
+        ret.load()
+        return ret
```

### Comparing `oarepo-cli-11.0.8/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/.gitignore` & `oarepo-cli-11.1.0/oarepo_cli/templates/repo/{{cookiecutter.repo_name}}/.gitignore`

 * *Files 14% similar despite different names*

```diff
@@ -28,16 +28,15 @@
 lib64/
 parts/
 sdist/
 var/
 *.egg-info/
 .installed.cfg
 *.egg
-Pipfile
-Pipfile.lock
+__pycache__/*
 
 # PyInstaller
 #  Usually these files are written by a python script from a template
 #  before PyInstaller builds the exe, so as to inject date/other infos into it.
 *.manifest
 *.spec
 
@@ -51,24 +50,18 @@
 .coverage
 .coverage.*
 .cache
 nosetests.xml
 coverage.xml
 *,cover
 
-# Translations
-*.mo
-
 # Django stuff:
 *.log
 
 # Sphinx documentation
 docs/_build/
 
 # PyBuilder
 target/
 
 # Vim swapfiles
 .*.sw?
-.DS_Store
-
-.venv-*/
```

### Comparing `oarepo-cli-11.0.8/oarepo_cli.egg-info/PKG-INFO` & `oarepo-cli-11.1.0/oarepo_cli.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-cli
-Version: 11.0.8
+Version: 11.1.0
 Summary: Utilities for managing invenio monorepo
 Description-Content-Type: text/markdown
 
 # oarepo-cli
 
 Work in progress.
```

