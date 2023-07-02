# Comparing `tmp/eradiate-0.23.2rc3.tar.gz` & `tmp/eradiate-0.23.2rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eradiate-0.23.2rc3.tar", last modified: Fri Jun 30 15:13:58 2023, max compression
+gzip compressed data, was "eradiate-0.23.2rc4.tar", last modified: Sun Jul  2 13:40:50 2023, max compression
```

## Comparing `eradiate-0.23.2rc3.tar` & `eradiate-0.23.2rc4.tar`

### file list

```diff
@@ -1,631 +1,631 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.098151 eradiate-0.23.2rc3/
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/.clang-format
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.030152 eradiate-0.23.2rc3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.034152 eradiate-0.23.2rc3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.034152 eradiate-0.23.2rc3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/.github/workflows/cd.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    18807 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7263 2023-06-30 15:13:58.098151 eradiate-0.23.2rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.034152 eradiate-0.23.2rc3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.034152 eradiate-0.23.2rc3/docs/_ext/
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/_ext/exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/_ext/pluginparameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.034152 eradiate-0.23.2rc3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/_static/.keep
--rw-r--r--   0 runner    (1001) docker     (123)    17013 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/_static/eradiate-logo-typo-black.png
--rw-r--r--   0 runner    (1001) docker     (123)    32795 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/_static/eradiate-logo-typo-black.svg
--rw-r--r--   0 runner    (1001) docker     (123)    25531 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/_static/eradiate-logo-typo-darkgrey.png
--rw-r--r--   0 runner    (1001) docker     (123)    34059 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/_static/eradiate-logo-typo-darkgrey.svg
--rw-r--r--   0 runner    (1001) docker     (123)    18587 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/_static/eradiate-logo-typo-white.png
--rw-r--r--   0 runner    (1001) docker     (123)    34061 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/_static/eradiate-logo-typo-white.svg
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/_static/theme_overrides.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.022152 eradiate-0.23.2rc3/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.034152 eradiate-0.23.2rc3/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/_templates/autosummary/module.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.034152 eradiate-0.23.2rc3/docs/_templates/sections/
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/_templates/sections/footer-content.html
--rw-r--r--   0 runner    (1001) docker     (123)    10467 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/convert_figures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.042152 eradiate-0.23.2rc3/docs/fig/
--rw-r--r--   0 runner    (1001) docker     (123)    20540 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/atmosphere_attributes.png
--rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/atmosphere_attributes.svg
--rw-r--r--   0 runner    (1001) docker     (123)    28149 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/azimuth-east_left.png
--rw-r--r--   0 runner    (1001) docker     (123)    32937 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/azimuth-east_left.svg
--rw-r--r--   0 runner    (1001) docker     (123)    28852 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/azimuth-east_right.png
--rw-r--r--   0 runner    (1001) docker     (123)    35278 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/azimuth-east_right.svg
--rw-r--r--   0 runner    (1001) docker     (123)    30666 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/azimuth-north_left.png
--rw-r--r--   0 runner    (1001) docker     (123)    32862 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/azimuth-north_left.svg
--rw-r--r--   0 runner    (1001) docker     (123)    28115 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/azimuth-north_right.png
--rw-r--r--   0 runner    (1001) docker     (123)    32455 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/azimuth-north_right.svg
--rw-r--r--   0 runner    (1001) docker     (123)    28153 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/azimuth-south_left.png
--rw-r--r--   0 runner    (1001) docker     (123)    32939 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/azimuth-south_left.svg
--rw-r--r--   0 runner    (1001) docker     (123)    28118 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/azimuth-south_right.png
--rw-r--r--   0 runner    (1001) docker     (123)    32455 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/azimuth-south_right.svg
--rw-r--r--   0 runner    (1001) docker     (123)    28178 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/azimuth-west_left.png
--rw-r--r--   0 runner    (1001) docker     (123)    32935 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/azimuth-west_left.svg
--rw-r--r--   0 runner    (1001) docker     (123)    28067 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/azimuth-west_right.png
--rw-r--r--   0 runner    (1001) docker     (123)    32437 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/azimuth-west_right.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/cartesian-coordinate-system.png
--rw-r--r--   0 runner    (1001) docker     (123)    15939 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/cartesian-coordinate-system.svg
--rw-r--r--   0 runner    (1001) docker     (123)    25301 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/cuboid_leaf_cloud_params.png
--rw-r--r--   0 runner    (1001) docker     (123)    11009 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/cuboid_leaf_cloud_params.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.042152 eradiate-0.23.2rc3/docs/fig/diagrams/
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/diagrams/class_diagram_biosphere.drawio
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/diagrams/cuboid_leaf_cloud_params.drawio
--rw-r--r--   0 runner    (1001) docker     (123)    20990 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/diagrams/package.drawio
--rw-r--r--   0 runner    (1001) docker     (123)    40438 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/eradiate-logo-typo-black.png
--rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/eradiate-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/icon_eradiate.png
--rw-r--r--   0 runner    (1001) docker     (123)    38873 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/package.png
--rw-r--r--   0 runner    (1001) docker     (123)    57417 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/package.svg
--rw-r--r--   0 runner    (1001) docker     (123)    32384 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/radiancemeter_hsphere.png
--rw-r--r--   0 runner    (1001) docker     (123)    43351 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/radiancemeter_hsphere.svg
--rw-r--r--   0 runner    (1001) docker     (123)    36773 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/radiancemeter_plane.png
--rw-r--r--   0 runner    (1001) docker     (123)    31853 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/radiancemeter_plane.svg
--rw-r--r--   0 runner    (1001) docker     (123)    31276 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/requirement_layers.png
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/requirement_layers.svg
--rw-r--r--   0 runner    (1001) docker     (123)    21451 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/solid_2017.png
--rw-r--r--   0 runner    (1001) docker     (123)    24994 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/spectral_discretization_ckd_atm_interval.png
--rw-r--r--   0 runner    (1001) docker     (123)    16459 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/spectral_discretization_ckd_atm_isolated.png
--rw-r--r--   0 runner    (1001) docker     (123)    28519 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/spectral_discretization_ckd_noatm_interval.png
--rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/spectral_discretization_ckd_noatm_isolated.png
--rw-r--r--   0 runner    (1001) docker     (123)    27127 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/spectral_discretization_mono_atm_interval.png
--rw-r--r--   0 runner    (1001) docker     (123)    12577 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/spectral_discretization_mono_atm_isolated.png
--rw-r--r--   0 runner    (1001) docker     (123)    46208 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/spectral_discretization_mono_noatm_interval1.png
--rw-r--r--   0 runner    (1001) docker     (123)    14036 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/spectral_discretization_mono_noatm_interval2.png
--rw-r--r--   0 runner    (1001) docker     (123)    21975 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/spectral_discretization_mono_noatm_isolated.png
--rw-r--r--   0 runner    (1001) docker     (123)    10036 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/spherical-coordinate-system.png
--rw-r--r--   0 runner    (1001) docker     (123)    19861 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/spherical-coordinate-system.svg
--rw-r--r--   0 runner    (1001) docker     (123)    20660 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/fig/thuillier_2003.png
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/generate_md_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/generate_rst_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/generate_rst_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/index_latex.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)    16528 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/references.bib
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.042152 eradiate-0.23.2rc3/docs/rst/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/bibliography.rst
--rw-r--r--   0 runner    (1001) docker     (123)    22779 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/dependencies.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.042152 eradiate-0.23.2rc3/docs/rst/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/developer_guide/design_atmosphere.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11633 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/developer_guide/dev_install.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/developer_guide/factory_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/developer_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/developer_guide/lazy_loading.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/developer_guide/radiometric_kernel_interface.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/developer_guide/scene_generator.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/developer_guide/update.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14549 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/maintainer_guide.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.050151 eradiate-0.23.2rc3/docs/rst/reference_api/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/attrs.rst
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/config.rst
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/constants.rst
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/contexts.rst
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/converters.rst
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/data.rst
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/eradiate_core.rst
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/experiments.rst
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/factory.rst
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/frame.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/kernel.rst
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/mode.rst
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/notebook.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/pipelines.rst
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/plot.rst
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/quad.rst
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/radprops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/rng.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/scenes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/spectral.rst
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/srf_tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/test_tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/thermoprops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/units.rst
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/util.rst
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/validators.rst
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/warp.rst
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_api/xarray.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.050151 eradiate-0.23.2rc3/docs/rst/reference_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/reference_plugins/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.050151 eradiate-0.23.2rc3/docs/rst/user_guide/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.050151 eradiate-0.23.2rc3/docs/rst/user_guide/atmosphere/
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/atmosphere/absorption.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.050151 eradiate-0.23.2rc3/docs/rst/user_guide/atmosphere/fig/
--rw-r--r--   0 runner    (1001) docker     (123)    25171 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/atmosphere/fig/bad_resolution.png
--rw-r--r--   0 runner    (1001) docker     (123)    26889 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/atmosphere/fig/good_resolution.png
--rw-r--r--   0 runner    (1001) docker     (123)    24938 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/atmosphere/fig/line.png
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/atmosphere/heterogeneous.rst
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/atmosphere/homogeneous.rst
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/atmosphere/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/atmosphere/intro.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/atmosphere/molecular.rst
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/atmosphere/particle_layer.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/atmosphere/rayleigh_scattering.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/basic_concepts.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/conventions.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.050151 eradiate-0.23.2rc3/docs/rst/user_guide/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/data/absorption.rst
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/data/atmosphere_radprops.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/data/atmosphere_thermoprops.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/data/ckd.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.050151 eradiate-0.23.2rc3/docs/rst/user_guide/data/fig/
--rw-r--r--   0 runner    (1001) docker     (123)    30117 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/data/fig/p_interp_rerr_histo_65349.png
--rw-r--r--   0 runner    (1001) docker     (123)    59107 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/data/fig/pt_points.png
--rw-r--r--   0 runner    (1001) docker     (123)    28580 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/data/fig/w_interp_rerr_histo_101325.png
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/data/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/data/intro.rst
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/data/particle_radprops.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11896 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/data/solar_irradiance.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/data/spectra-us76_u86_4.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/data/srf.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/onedim_experiment.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/package_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13015 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/spectral_discretization.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5386 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/rst/user_guide/unit_guide_user.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.054151 eradiate-0.23.2rc3/docs/src/
--rw-r--r--   0 runner    (1001) docker     (123)    18807 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/src/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/docs/src/reference_cli.md
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.054151 eradiate-0.23.2rc3/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/check_conda_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.058152 eradiate-0.23.2rc3/requirements/conda/
--rw-r--r--   0 runner    (1001) docker     (123)    22312 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-dependencies-linux-64.lock
--rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-dependencies-osx-64.lock
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-dependencies.dot
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-dependencies.yml
--rw-r--r--   0 runner    (1001) docker     (123)    41340 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-dev-linux-64.lock
--rw-r--r--   0 runner    (1001) docker     (123)    32328 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-dev-osx-64.lock
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-dev.dot
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-dev.yml
--rw-r--r--   0 runner    (1001) docker     (123)    29544 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-docs-linux-64.lock
--rw-r--r--   0 runner    (1001) docker     (123)    20325 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-docs-osx-64.lock
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-docs.dot
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    22312 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-main-linux-64.lock
--rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-main-osx-64.lock
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-main.dot
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-main.yml
--rw-r--r--   0 runner    (1001) docker     (123)    41340 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-optional-linux-64.lock
--rw-r--r--   0 runner    (1001) docker     (123)    32328 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-optional-osx-64.lock
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-optional.dot
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-optional.yml
--rw-r--r--   0 runner    (1001) docker     (123)    20158 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-recommended-linux-64.lock
--rw-r--r--   0 runner    (1001) docker     (123)    19689 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-recommended-osx-64.lock
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-recommended.dot
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-recommended.yml
--rw-r--r--   0 runner    (1001) docker     (123)    23014 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-tests-linux-64.lock
--rw-r--r--   0 runner    (1001) docker     (123)    14040 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-tests-osx-64.lock
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-tests.dot
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/environment-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/conda/layer_graph.dot
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/copy_envvars.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/environment.in
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/layered.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/make_conda_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/make_pip_in_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.058152 eradiate-0.23.2rc3/requirements/pip/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/pip/dependencies.in
--rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/pip/dependencies.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/pip/dev.in
--rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/pip/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/pip/docs.in
--rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/pip/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/pip/main.in
--rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/pip/main.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/pip/optional.in
--rw-r--r--   0 runner    (1001) docker     (123)    20980 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/pip/optional.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/pip/recommended.in
--rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/pip/recommended.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/pip/tests.in
--rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/requirements/pip/tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/setpath.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 15:13:58.098151 eradiate-0.23.2rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.022152 eradiate-0.23.2rc3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.062152 eradiate-0.23.2rc3/src/eradiate/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9328 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    10601 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10473 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/attrs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.062152 eradiate-0.23.2rc3/src/eradiate/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/cli/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/cli/show.py
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/cli/srf.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/converters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.062152 eradiate-0.23.2rc3/src/eradiate/data/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/data/_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/data/_blind_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/data/_blind_online.py
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/data/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/data/_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/data/_safe_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/data/_safe_online.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/data/_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    16343 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/data/downloads.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/data/downloads_development.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.066151 eradiate-0.23.2rc3/src/eradiate/experiments/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/experiments/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7387 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/experiments/_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/experiments/_canopy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/experiments/_canopy_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (123)    20760 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/experiments/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7795 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/experiments/_dem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/experiments/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12531 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/frame.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.066151 eradiate-0.23.2rc3/src/eradiate/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/kernel/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/kernel/_bitmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/kernel/_bsdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/kernel/_kernel_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    11961 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/kernel/_render.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/kernel/gridvolume.py
--rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/kernel/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/kernel/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.066151 eradiate-0.23.2rc3/src/eradiate/notebook/
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/notebook/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/notebook/tutorials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.066151 eradiate-0.23.2rc3/src/eradiate/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/pipelines/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7620 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/pipelines/_aggregate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11488 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/pipelines/_assemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     8299 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/pipelines/_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/pipelines/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/pipelines/_gather.py
--rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/quad.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.066151 eradiate-0.23.2rc3/src/eradiate/radprops/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/radprops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/radprops/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/radprops/_afgl1986.py
--rw-r--r--   0 runner    (1001) docker     (123)    14982 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/radprops/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/radprops/_us76_approx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/radprops/_util_mono.py
--rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/radprops/absorption.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/radprops/rayleigh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/rng.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.066151 eradiate-0.23.2rc3/src/eradiate/scenes/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.070151 eradiate-0.23.2rc3/src/eradiate/scenes/atmosphere/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/atmosphere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/atmosphere/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    23375 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/atmosphere/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    11741 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/atmosphere/_heterogeneous.py
--rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/atmosphere/_homogeneous.py
--rw-r--r--   0 runner    (1001) docker     (123)    17072 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/atmosphere/_molecular_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (123)    10737 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/atmosphere/_particle_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)    17259 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/atmosphere/_particle_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.070151 eradiate-0.23.2rc3/src/eradiate/scenes/biosphere/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/biosphere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/biosphere/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10144 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/biosphere/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    12392 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/biosphere/_discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)    38992 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/biosphere/_leaf_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    17136 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/biosphere/_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.070151 eradiate-0.23.2rc3/src/eradiate/scenes/bsdfs/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/bsdfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/bsdfs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/bsdfs/_black.py
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/bsdfs/_checkerboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/bsdfs/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/bsdfs/_lambertian.py
--rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/bsdfs/_mqdiffuse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/bsdfs/_opacity_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/bsdfs/_rpv.py
--rw-r--r--   0 runner    (1001) docker     (123)    17684 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.070151 eradiate-0.23.2rc3/src/eradiate/scenes/illumination/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/illumination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/illumination/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/illumination/_astro_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/illumination/_constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/illumination/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/illumination/_directional.py
--rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/illumination/_spot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.070151 eradiate-0.23.2rc3/src/eradiate/scenes/integrators/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/integrators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/integrators/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/integrators/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/integrators/_path_tracers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.074151 eradiate-0.23.2rc3/src/eradiate/scenes/measure/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/measure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/measure/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9940 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/measure/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     9534 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/measure/_distant.py
--rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/measure/_distant_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/measure/_hemispherical_distant.py
--rw-r--r--   0 runner    (1001) docker     (123)    22410 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/measure/_multi_distant.py
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/measure/_multi_radiancemeter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/measure/_perspective.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/measure/_radiancemeter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.074151 eradiate-0.23.2rc3/src/eradiate/scenes/phase/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/phase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/phase/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/phase/_blend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/phase/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/phase/_hg.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/phase/_isotropic.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/phase/_rayleigh.py
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/phase/_tabulated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.074151 eradiate-0.23.2rc3/src/eradiate/scenes/shapes/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/shapes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/shapes/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/shapes/_buffermesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/shapes/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/shapes/_cuboid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/shapes/_filemesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/shapes/_rectangle.py
--rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/shapes/_sphere.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.074151 eradiate-0.23.2rc3/src/eradiate/scenes/spectra/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/spectra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/spectra/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/spectra/_air_scattering_coefficient.py
--rw-r--r--   0 runner    (1001) docker     (123)     9743 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/spectra/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    12948 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/spectra/_interpolated.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/spectra/_multi_delta.py
--rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/spectra/_solar_irradiance.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/spectra/_uniform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.074151 eradiate-0.23.2rc3/src/eradiate/scenes/surface/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/surface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/surface/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/surface/_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/surface/_central_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/surface/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    18023 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/scenes/surface/_dem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.078151 eradiate-0.23.2rc3/src/eradiate/spectral/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/spectral/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/spectral/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9009 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/spectral/ckd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/spectral/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/spectral/mono.py
--rw-r--r--   0 runner    (1001) docker     (123)    26484 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/srf_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.078151 eradiate-0.23.2rc3/src/eradiate/test_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/test_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/test_tools/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    12204 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/test_tools/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/test_tools/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/test_tools/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.078151 eradiate-0.23.2rc3/src/eradiate/thermoprops/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/thermoprops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/thermoprops/afgl_1986.py
--rw-r--r--   0 runner    (1001) docker     (123)    42061 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/thermoprops/us76.py
--rw-r--r--   0 runner    (1001) docker     (123)    22124 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/thermoprops/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.078151 eradiate-0.23.2rc3/src/eradiate/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11933 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/util/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)    15100 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/util/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/util/numpydoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/util/sys_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/warp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.078151 eradiate-0.23.2rc3/src/eradiate/xarray/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/xarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/xarray/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/xarray/_accessors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/xarray/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/src/eradiate/xarray/interp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.062152 eradiate-0.23.2rc3/src/eradiate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7263 2023-06-30 15:13:57.000000 eradiate-0.23.2rc3/src/eradiate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22344 2023-06-30 15:13:58.000000 eradiate-0.23.2rc3/src/eradiate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 15:13:57.000000 eradiate-0.23.2rc3/src/eradiate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-30 15:13:57.000000 eradiate-0.23.2rc3/src/eradiate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-30 15:13:57.000000 eradiate-0.23.2rc3/src/eradiate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-30 15:13:57.000000 eradiate-0.23.2rc3/src/eradiate.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.078151 eradiate-0.23.2rc3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.078151 eradiate-0.23.2rc3/tests/01_eradiate/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.082152 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.082152 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/data/test_blind_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/data/test_blind_online.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/data/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/data/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/data/test_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/data/test_open.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/data/test_safe_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/data/test_safe_online.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.082152 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/experiments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8819 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/experiments/test_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/experiments/test_canopy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10387 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/experiments/test_canopy_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/experiments/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/experiments/test_dem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/experiments/test_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.082152 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/kernel/test_gridvolume.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/kernel/test_kernel_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/kernel/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/kernel/test_render.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/kernel/test_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.082152 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/pipelines/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/pipelines/test_aggregate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/pipelines/test_assemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/pipelines/test_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/pipelines/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/pipelines/test_gather.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.086151 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/radprops/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/radprops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/radprops/test_absorption.py
--rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/radprops/test_afgl_1986.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/radprops/test_rayleigh_scattering.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/radprops/test_us76_approx.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/radprops/test_zgrid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.086151 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.086151 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/atmosphere/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/atmosphere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/atmosphere/test_heterogeneous.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/atmosphere/test_homogeneous.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/atmosphere/test_molecular_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/atmosphere/test_particle_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)    13966 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/atmosphere/test_particle_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.086151 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/biosphere/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/biosphere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/biosphere/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/biosphere/test_discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)    10746 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/biosphere/test_leaf_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/biosphere/test_tree_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/biosphere/test_tree_mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.086151 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/bsdfs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/bsdfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/bsdfs/test_black.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/bsdfs/test_checkerboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/bsdfs/test_lambertian.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/bsdfs/test_mqdiffuse.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/bsdfs/test_rpv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.086151 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/illumination/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/illumination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/illumination/test_astro_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/illumination/test_constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/illumination/test_directional.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/illumination/test_spot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.090151 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/integrators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/integrators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/integrators/test_path_tracers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.090151 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/measure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/measure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/measure/test_distant_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/measure/test_hemispherical_distant.py
--rw-r--r--   0 runner    (1001) docker     (123)     9311 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/measure/test_multi_distant.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/measure/test_multi_radiancemeter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/measure/test_perspective.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/measure/test_radiancemeter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/measure/test_target.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.090151 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/phase/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/phase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/phase/test_blend.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/phase/test_hg.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/phase/test_isotropic.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/phase/test_rayleigh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/phase/test_tabulated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.090151 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/shapes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/shapes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/shapes/test_buffermesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/shapes/test_cuboid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/shapes/test_filemesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/shapes/test_rectangle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/shapes/test_sphere.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.094151 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/spectra/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/spectra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/spectra/test_air_scattering_coefficient.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/spectra/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/spectra/test_interpolated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/spectra/test_solar_irradiance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/spectra/test_uniform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.094151 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/surface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/surface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/surface/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/surface/test_central_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/surface/test_dem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/test_core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.094151 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/spectral/
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/spectral/test_ckd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/spectral/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/spectral/test_mono.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/test_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/test_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/test_quad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/test_rng.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/test_srf_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.094151 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/test_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/test_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/test_tools/test_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/test_units.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/test_warp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.094151 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/thermoprops/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/thermoprops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/thermoprops/test_afgl1986.py
--rw-r--r--   0 runner    (1001) docker     (123)    11910 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/thermoprops/test_us76.py
--rw-r--r--   0 runner    (1001) docker     (123)    10534 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/thermoprops/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.094151 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/util/test_deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/util/test_misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.094151 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/xarray/
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/xarray/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/01_unit/xarray/test_interp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.098151 eradiate-0.23.2rc3/tests/01_eradiate/02_system/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/02_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/02_system/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_albedo.py
--rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_atmosphere_ckd_vs_mono.py
--rw-r--r--   0 runner    (1001) docker     (123)    25312 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_atmosphere_rpv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_ckd_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_compare_canopy_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_expansion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_parameter_id_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_irradiance_scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_kernel_render_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_maximum_scene_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_mdistant_insitu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_onedim_lambertian_brf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_onedim_phase.py
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_onedim_symmetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_spectral_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.098151 eradiate-0.23.2rc3/tests/01_eradiate/03_regression/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/03_regression/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.098151 eradiate-0.23.2rc3/tests/01_eradiate/03_regression/atmospheres/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/03_regression/atmospheres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/03_regression/atmospheres/test_rpv_afgl1986.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/03_regression/atmospheres/test_rpv_afgl1986_continental.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.098151 eradiate-0.23.2rc3/tests/01_eradiate/03_regression/rami4atm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/03_regression/rami4atm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/03_regression/rami4atm/test_rami4atm_hom00_bla_sd2s_m03_z30a000_brfpp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:58.098151 eradiate-0.23.2rc3/tests/01_eradiate/03_regression/romc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/03_regression/romc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/03_regression/romc/test_het01.py
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/03_regression/romc/test_het04.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/03_regression/romc/test_het06.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/01_eradiate/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-06-30 15:13:46.000000 eradiate-0.23.2rc3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.283059 eradiate-0.23.2rc4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.175057 eradiate-0.23.2rc4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.175057 eradiate-0.23.2rc4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.175057 eradiate-0.23.2rc4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/.github/workflows/cd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    18807 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7263 2023-07-02 13:40:50.283059 eradiate-0.23.2rc4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.175057 eradiate-0.23.2rc4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.175057 eradiate-0.23.2rc4/docs/_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/_ext/exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/_ext/pluginparameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.179057 eradiate-0.23.2rc4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/_static/.keep
+-rw-r--r--   0 runner    (1001) docker     (123)    17013 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/_static/eradiate-logo-typo-black.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32795 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/_static/eradiate-logo-typo-black.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    25531 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/_static/eradiate-logo-typo-darkgrey.png
+-rw-r--r--   0 runner    (1001) docker     (123)    34059 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/_static/eradiate-logo-typo-darkgrey.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    18587 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/_static/eradiate-logo-typo-white.png
+-rw-r--r--   0 runner    (1001) docker     (123)    34061 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/_static/eradiate-logo-typo-white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/_static/theme_overrides.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.163056 eradiate-0.23.2rc4/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.179057 eradiate-0.23.2rc4/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/_templates/autosummary/module.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.179057 eradiate-0.23.2rc4/docs/_templates/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/_templates/sections/footer-content.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10467 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/convert_figures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.191057 eradiate-0.23.2rc4/docs/fig/
+-rw-r--r--   0 runner    (1001) docker     (123)    20540 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/atmosphere_attributes.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/atmosphere_attributes.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28149 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/azimuth-east_left.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32937 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/azimuth-east_left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28852 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/azimuth-east_right.png
+-rw-r--r--   0 runner    (1001) docker     (123)    35278 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/azimuth-east_right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    30666 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/azimuth-north_left.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32862 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/azimuth-north_left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28115 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/azimuth-north_right.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32455 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/azimuth-north_right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28153 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/azimuth-south_left.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32939 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/azimuth-south_left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28118 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/azimuth-south_right.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32455 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/azimuth-south_right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28178 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/azimuth-west_left.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32935 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/azimuth-west_left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28067 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/azimuth-west_right.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32437 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/azimuth-west_right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/cartesian-coordinate-system.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15939 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/cartesian-coordinate-system.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    25301 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/cuboid_leaf_cloud_params.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11009 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/cuboid_leaf_cloud_params.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.191057 eradiate-0.23.2rc4/docs/fig/diagrams/
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/diagrams/class_diagram_biosphere.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/diagrams/cuboid_leaf_cloud_params.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    20990 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/diagrams/package.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    40438 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/eradiate-logo-typo-black.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/eradiate-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/icon_eradiate.png
+-rw-r--r--   0 runner    (1001) docker     (123)    38873 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/package.png
+-rw-r--r--   0 runner    (1001) docker     (123)    57417 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/package.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    32384 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/radiancemeter_hsphere.png
+-rw-r--r--   0 runner    (1001) docker     (123)    43351 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/radiancemeter_hsphere.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    36773 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/radiancemeter_plane.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31853 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/radiancemeter_plane.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    31276 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/requirement_layers.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/requirement_layers.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    21451 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/solid_2017.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24994 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/spectral_discretization_ckd_atm_interval.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16459 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/spectral_discretization_ckd_atm_isolated.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28519 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/spectral_discretization_ckd_noatm_interval.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/spectral_discretization_ckd_noatm_isolated.png
+-rw-r--r--   0 runner    (1001) docker     (123)    27127 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/spectral_discretization_mono_atm_interval.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12577 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/spectral_discretization_mono_atm_isolated.png
+-rw-r--r--   0 runner    (1001) docker     (123)    46208 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/spectral_discretization_mono_noatm_interval1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14036 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/spectral_discretization_mono_noatm_interval2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21975 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/spectral_discretization_mono_noatm_isolated.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10036 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/spherical-coordinate-system.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19861 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/spherical-coordinate-system.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    20660 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/fig/thuillier_2003.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/generate_md_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/generate_rst_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/generate_rst_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/index_latex.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)    16528 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/references.bib
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.191057 eradiate-0.23.2rc4/docs/rst/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/bibliography.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    22779 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/dependencies.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.191057 eradiate-0.23.2rc4/docs/rst/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/developer_guide/design_atmosphere.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11633 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/developer_guide/dev_install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/developer_guide/factory_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/developer_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/developer_guide/lazy_loading.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/developer_guide/radiometric_kernel_interface.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/developer_guide/scene_generator.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/developer_guide/update.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14549 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/maintainer_guide.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.199057 eradiate-0.23.2rc4/docs/rst/reference_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/reference_api/attrs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/reference_api/config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/reference_api/constants.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/reference_api/contexts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/reference_api/converters.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/reference_api/data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/reference_api/eradiate_core.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/reference_api/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/reference_api/experiments.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/reference_api/factory.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/reference_api/frame.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/reference_api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/reference_api/kernel.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/reference_api/mode.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/reference_api/notebook.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/reference_api/pipelines.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/reference_api/plot.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/reference_api/quad.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/reference_api/radprops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/reference_api/rng.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/reference_api/scenes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/reference_api/spectral.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/reference_api/srf_tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/reference_api/test_tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/reference_api/thermoprops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/reference_api/units.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/reference_api/util.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/reference_api/validators.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/reference_api/warp.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/reference_api/xarray.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.199057 eradiate-0.23.2rc4/docs/rst/reference_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/reference_plugins/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.199057 eradiate-0.23.2rc4/docs/rst/user_guide/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.203057 eradiate-0.23.2rc4/docs/rst/user_guide/atmosphere/
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/user_guide/atmosphere/absorption.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.203057 eradiate-0.23.2rc4/docs/rst/user_guide/atmosphere/fig/
+-rw-r--r--   0 runner    (1001) docker     (123)    25171 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/user_guide/atmosphere/fig/bad_resolution.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26889 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/user_guide/atmosphere/fig/good_resolution.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24938 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/user_guide/atmosphere/fig/line.png
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/user_guide/atmosphere/heterogeneous.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/user_guide/atmosphere/homogeneous.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/user_guide/atmosphere/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/user_guide/atmosphere/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/user_guide/atmosphere/molecular.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/user_guide/atmosphere/particle_layer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/user_guide/atmosphere/rayleigh_scattering.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/user_guide/basic_concepts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/user_guide/conventions.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.203057 eradiate-0.23.2rc4/docs/rst/user_guide/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/user_guide/data/absorption.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/user_guide/data/atmosphere_radprops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/user_guide/data/atmosphere_thermoprops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/user_guide/data/ckd.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.203057 eradiate-0.23.2rc4/docs/rst/user_guide/data/fig/
+-rw-r--r--   0 runner    (1001) docker     (123)    30117 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/user_guide/data/fig/p_interp_rerr_histo_65349.png
+-rw-r--r--   0 runner    (1001) docker     (123)    59107 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/user_guide/data/fig/pt_points.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28580 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/user_guide/data/fig/w_interp_rerr_histo_101325.png
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/user_guide/data/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/user_guide/data/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/user_guide/data/particle_radprops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11896 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/user_guide/data/solar_irradiance.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/user_guide/data/spectra-us76_u86_4.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/user_guide/data/srf.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/user_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/user_guide/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/user_guide/onedim_experiment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/user_guide/package_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13015 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/user_guide/spectral_discretization.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5386 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/rst/user_guide/unit_guide_user.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.203057 eradiate-0.23.2rc4/docs/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    18807 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/src/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/docs/src/reference_cli.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.207057 eradiate-0.23.2rc4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/check_conda_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.211057 eradiate-0.23.2rc4/requirements/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)    22407 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/conda/environment-dependencies-linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    13337 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/conda/environment-dependencies-osx-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/conda/environment-dependencies.dot
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/conda/environment-dependencies.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    41546 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/conda/environment-dev-linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    32550 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/conda/environment-dev-osx-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/conda/environment-dev.dot
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/conda/environment-dev.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    29639 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/conda/environment-docs-linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    20436 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/conda/environment-docs-osx-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/conda/environment-docs.dot
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/conda/environment-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    22407 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/conda/environment-main-linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    13337 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/conda/environment-main-osx-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/conda/environment-main.dot
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/conda/environment-main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    41546 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/conda/environment-optional-linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    32550 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/conda/environment-optional-osx-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/conda/environment-optional.dot
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/conda/environment-optional.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    20269 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/conda/environment-recommended-linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    19798 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/conda/environment-recommended-osx-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/conda/environment-recommended.dot
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/conda/environment-recommended.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    23107 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/conda/environment-tests-linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    14149 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/conda/environment-tests-osx-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/conda/environment-tests.dot
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/conda/environment-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/conda/layer_graph.dot
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/copy_envvars.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/environment.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/layered.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/make_conda_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/make_pip_in_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.215057 eradiate-0.23.2rc4/requirements/pip/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/pip/dependencies.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/pip/dependencies.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/pip/dev.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/pip/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/pip/docs.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10184 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/pip/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/pip/main.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/pip/main.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/pip/optional.in
+-rw-r--r--   0 runner    (1001) docker     (123)    21236 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/pip/optional.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/pip/recommended.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/pip/recommended.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/pip/tests.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/requirements/pip/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/setpath.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 13:40:50.283059 eradiate-0.23.2rc4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.163056 eradiate-0.23.2rc4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.219058 eradiate-0.23.2rc4/src/eradiate/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9328 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10601 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10473 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/attrs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.219058 eradiate-0.23.2rc4/src/eradiate/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/cli/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/cli/show.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/cli/srf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/converters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.223058 eradiate-0.23.2rc4/src/eradiate/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/data/_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/data/_blind_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/data/_blind_online.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/data/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/data/_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/data/_safe_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/data/_safe_online.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/data/_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16343 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/data/downloads.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/data/downloads_development.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.223058 eradiate-0.23.2rc4/src/eradiate/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/experiments/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7387 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/experiments/_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/experiments/_canopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/experiments/_canopy_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20760 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/experiments/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7795 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/experiments/_dem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/experiments/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12531 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/frame.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.227058 eradiate-0.23.2rc4/src/eradiate/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/kernel/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/kernel/_bitmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/kernel/_bsdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/kernel/_kernel_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11961 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/kernel/_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/kernel/gridvolume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/kernel/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/kernel/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.227058 eradiate-0.23.2rc4/src/eradiate/notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/notebook/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/notebook/tutorials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.231058 eradiate-0.23.2rc4/src/eradiate/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/pipelines/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7620 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/pipelines/_aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11488 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/pipelines/_assemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8299 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/pipelines/_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/pipelines/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/pipelines/_gather.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/quad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.235058 eradiate-0.23.2rc4/src/eradiate/radprops/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/radprops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/radprops/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/radprops/_afgl1986.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14982 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/radprops/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/radprops/_us76_approx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/radprops/_util_mono.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/radprops/absorption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/radprops/rayleigh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/rng.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.239058 eradiate-0.23.2rc4/src/eradiate/scenes/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.239058 eradiate-0.23.2rc4/src/eradiate/scenes/atmosphere/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/atmosphere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/atmosphere/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    23375 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/atmosphere/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11741 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/atmosphere/_heterogeneous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/atmosphere/_homogeneous.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17072 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/atmosphere/_molecular_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10737 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/atmosphere/_particle_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17259 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/atmosphere/_particle_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.239058 eradiate-0.23.2rc4/src/eradiate/scenes/biosphere/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/biosphere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/biosphere/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10144 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/biosphere/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12392 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/biosphere/_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38992 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/biosphere/_leaf_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17136 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/biosphere/_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.243058 eradiate-0.23.2rc4/src/eradiate/scenes/bsdfs/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/bsdfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/bsdfs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/bsdfs/_black.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/bsdfs/_checkerboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/bsdfs/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/bsdfs/_lambertian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/bsdfs/_mqdiffuse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/bsdfs/_opacity_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/bsdfs/_rpv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17684 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.243058 eradiate-0.23.2rc4/src/eradiate/scenes/illumination/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/illumination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/illumination/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/illumination/_astro_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/illumination/_constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/illumination/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/illumination/_directional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/illumination/_spot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.243058 eradiate-0.23.2rc4/src/eradiate/scenes/integrators/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/integrators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/integrators/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/integrators/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/integrators/_path_tracers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.247058 eradiate-0.23.2rc4/src/eradiate/scenes/measure/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/measure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/measure/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9940 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/measure/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9534 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/measure/_distant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/measure/_distant_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/measure/_hemispherical_distant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22410 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/measure/_multi_distant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/measure/_multi_radiancemeter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/measure/_perspective.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/measure/_radiancemeter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.247058 eradiate-0.23.2rc4/src/eradiate/scenes/phase/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/phase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/phase/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/phase/_blend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/phase/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/phase/_hg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/phase/_isotropic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/phase/_rayleigh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/phase/_tabulated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.247058 eradiate-0.23.2rc4/src/eradiate/scenes/shapes/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/shapes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/shapes/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/shapes/_buffermesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/shapes/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/shapes/_cuboid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/shapes/_filemesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/shapes/_rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/shapes/_sphere.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.251058 eradiate-0.23.2rc4/src/eradiate/scenes/spectra/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/spectra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/spectra/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/spectra/_air_scattering_coefficient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9743 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/spectra/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12948 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/spectra/_interpolated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/spectra/_multi_delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/spectra/_solar_irradiance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/spectra/_uniform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.251058 eradiate-0.23.2rc4/src/eradiate/scenes/surface/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/surface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/surface/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/surface/_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/surface/_central_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/surface/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18023 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/scenes/surface/_dem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.251058 eradiate-0.23.2rc4/src/eradiate/spectral/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/spectral/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/spectral/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9009 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/spectral/ckd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/spectral/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/spectral/mono.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26484 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/srf_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.251058 eradiate-0.23.2rc4/src/eradiate/test_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/test_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/test_tools/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12204 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/test_tools/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/test_tools/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/test_tools/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.255058 eradiate-0.23.2rc4/src/eradiate/thermoprops/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/thermoprops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/thermoprops/afgl_1986.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42061 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/thermoprops/us76.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22124 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/thermoprops/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.255058 eradiate-0.23.2rc4/src/eradiate/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11933 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/util/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15100 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/util/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/util/numpydoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/util/sys_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/warp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.255058 eradiate-0.23.2rc4/src/eradiate/xarray/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/xarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/xarray/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/xarray/_accessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/xarray/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/src/eradiate/xarray/interp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.219058 eradiate-0.23.2rc4/src/eradiate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7263 2023-07-02 13:40:50.000000 eradiate-0.23.2rc4/src/eradiate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22344 2023-07-02 13:40:50.000000 eradiate-0.23.2rc4/src/eradiate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 13:40:50.000000 eradiate-0.23.2rc4/src/eradiate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-02 13:40:50.000000 eradiate-0.23.2rc4/src/eradiate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-07-02 13:40:50.000000 eradiate-0.23.2rc4/src/eradiate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-02 13:40:50.000000 eradiate-0.23.2rc4/src/eradiate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.255058 eradiate-0.23.2rc4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.255058 eradiate-0.23.2rc4/tests/01_eradiate/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.259059 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.259059 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/data/test_blind_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/data/test_blind_online.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/data/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/data/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/data/test_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/data/test_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/data/test_safe_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/data/test_safe_online.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.263059 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8819 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/experiments/test_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/experiments/test_canopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10387 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/experiments/test_canopy_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/experiments/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/experiments/test_dem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/experiments/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.263059 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/kernel/test_gridvolume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/kernel/test_kernel_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/kernel/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/kernel/test_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/kernel/test_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.263059 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/pipelines/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/pipelines/test_aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/pipelines/test_assemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/pipelines/test_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/pipelines/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/pipelines/test_gather.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.263059 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/radprops/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/radprops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/radprops/test_absorption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/radprops/test_afgl_1986.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/radprops/test_rayleigh_scattering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/radprops/test_us76_approx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/radprops/test_zgrid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.263059 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.267059 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/atmosphere/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/atmosphere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/atmosphere/test_heterogeneous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/atmosphere/test_homogeneous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/atmosphere/test_molecular_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/atmosphere/test_particle_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13966 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/atmosphere/test_particle_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.267059 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/biosphere/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/biosphere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/biosphere/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/biosphere/test_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10746 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/biosphere/test_leaf_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/biosphere/test_tree_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/biosphere/test_tree_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.267059 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/bsdfs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/bsdfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/bsdfs/test_black.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/bsdfs/test_checkerboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/bsdfs/test_lambertian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/bsdfs/test_mqdiffuse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/bsdfs/test_rpv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.267059 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/illumination/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/illumination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/illumination/test_astro_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/illumination/test_constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/illumination/test_directional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/illumination/test_spot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.267059 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/integrators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/integrators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/integrators/test_path_tracers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.271059 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/measure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/measure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/measure/test_distant_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/measure/test_hemispherical_distant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9311 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/measure/test_multi_distant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/measure/test_multi_radiancemeter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/measure/test_perspective.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/measure/test_radiancemeter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/measure/test_target.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.271059 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/phase/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/phase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/phase/test_blend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/phase/test_hg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/phase/test_isotropic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/phase/test_rayleigh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/phase/test_tabulated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.271059 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/shapes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/shapes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/shapes/test_buffermesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/shapes/test_cuboid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/shapes/test_filemesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/shapes/test_rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/shapes/test_sphere.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.275059 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/spectra/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/spectra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/spectra/test_air_scattering_coefficient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/spectra/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/spectra/test_interpolated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/spectra/test_solar_irradiance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/spectra/test_uniform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.275059 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/surface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/surface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/surface/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/surface/test_central_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/surface/test_dem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.275059 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/spectral/
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/spectral/test_ckd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/spectral/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/spectral/test_mono.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/test_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/test_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/test_quad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/test_rng.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/test_srf_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.275059 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/test_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/test_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/test_tools/test_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/test_warp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.275059 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/thermoprops/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/thermoprops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/thermoprops/test_afgl1986.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11910 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/thermoprops/test_us76.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10534 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/thermoprops/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.275059 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/util/test_deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/util/test_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.275059 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/xarray/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/xarray/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/01_unit/xarray/test_interp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.279059 eradiate-0.23.2rc4/tests/01_eradiate/02_system/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/02_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/02_system/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/02_system/test_albedo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/02_system/test_atmosphere_ckd_vs_mono.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25312 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/02_system/test_atmosphere_rpv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/02_system/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/02_system/test_ckd_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/02_system/test_compare_canopy_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_parameter_id_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/02_system/test_irradiance_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/02_system/test_kernel_render_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/02_system/test_maximum_scene_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/02_system/test_mdistant_insitu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/02_system/test_onedim_lambertian_brf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/02_system/test_onedim_phase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/02_system/test_onedim_symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/02_system/test_spectral_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.279059 eradiate-0.23.2rc4/tests/01_eradiate/03_regression/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/03_regression/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.279059 eradiate-0.23.2rc4/tests/01_eradiate/03_regression/atmospheres/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/03_regression/atmospheres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/03_regression/atmospheres/test_rpv_afgl1986.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/03_regression/atmospheres/test_rpv_afgl1986_continental.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.283059 eradiate-0.23.2rc4/tests/01_eradiate/03_regression/rami4atm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/03_regression/rami4atm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/03_regression/rami4atm/test_rami4atm_hom00_bla_sd2s_m03_z30a000_brfpp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:50.283059 eradiate-0.23.2rc4/tests/01_eradiate/03_regression/romc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/03_regression/romc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/03_regression/romc/test_het01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/03_regression/romc/test_het04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/03_regression/romc/test_het06.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/01_eradiate/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-07-02 13:40:34.000000 eradiate-0.23.2rc4/tests/conftest.py
```

### Comparing `eradiate-0.23.2rc3/.clang-format` & `eradiate-0.23.2rc4/.clang-format`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/.github/ISSUE_TEMPLATE/bug_report.md` & `eradiate-0.23.2rc4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/.github/ISSUE_TEMPLATE/feature_request.md` & `eradiate-0.23.2rc4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/.github/pull_request_template.md` & `eradiate-0.23.2rc4/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/.github/workflows/cd.yml` & `eradiate-0.23.2rc4/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/.github/workflows/ci.yml` & `eradiate-0.23.2rc4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/.pre-commit-config.yaml` & `eradiate-0.23.2rc4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/.readthedocs.yml` & `eradiate-0.23.2rc4/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/CHANGELOG.md` & `eradiate-0.23.2rc4/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/CONTRIBUTING.md` & `eradiate-0.23.2rc4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/LICENSE` & `eradiate-0.23.2rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/Makefile` & `eradiate-0.23.2rc4/Makefile`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/PKG-INFO` & `eradiate-0.23.2rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eradiate
-Version: 0.23.2rc3
+Version: 0.23.2rc4
 Summary: A radiative transfer model for the Earth observation community
 Author: The Eradiate Team
 Maintainer: The Eradiate Team
 License: LGPLv3
 Project-URL: changelog, https://github.com/eradiate/eradiate/CHANGELOG.md
 Project-URL: documentation, https://eradiate.readthedocs.io
 Project-URL: repository, https://github.com/eradiate/eradiate
```

### Comparing `eradiate-0.23.2rc3/README.md` & `eradiate-0.23.2rc4/README.md`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/Makefile` & `eradiate-0.23.2rc4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/_ext/exec.py` & `eradiate-0.23.2rc4/docs/_ext/exec.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/_ext/pluginparameters.py` & `eradiate-0.23.2rc4/docs/_ext/pluginparameters.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/_static/eradiate-logo-typo-black.png` & `eradiate-0.23.2rc4/docs/_static/eradiate-logo-typo-black.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/_static/eradiate-logo-typo-black.svg` & `eradiate-0.23.2rc4/docs/_static/eradiate-logo-typo-black.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/_static/eradiate-logo-typo-darkgrey.png` & `eradiate-0.23.2rc4/docs/_static/eradiate-logo-typo-darkgrey.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/_static/eradiate-logo-typo-darkgrey.svg` & `eradiate-0.23.2rc4/docs/_static/eradiate-logo-typo-darkgrey.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/_static/eradiate-logo-typo-white.png` & `eradiate-0.23.2rc4/docs/_static/eradiate-logo-typo-white.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/_static/eradiate-logo-typo-white.svg` & `eradiate-0.23.2rc4/docs/_static/eradiate-logo-typo-white.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/_templates/autosummary/module.rst` & `eradiate-0.23.2rc4/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/_templates/sections/footer-content.html` & `eradiate-0.23.2rc4/docs/_templates/sections/footer-content.html`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/conf.py` & `eradiate-0.23.2rc4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/atmosphere_attributes.png` & `eradiate-0.23.2rc4/docs/fig/atmosphere_attributes.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/atmosphere_attributes.svg` & `eradiate-0.23.2rc4/docs/fig/atmosphere_attributes.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/azimuth-east_left.png` & `eradiate-0.23.2rc4/docs/fig/azimuth-east_left.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/azimuth-east_left.svg` & `eradiate-0.23.2rc4/docs/fig/azimuth-east_left.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/azimuth-east_right.png` & `eradiate-0.23.2rc4/docs/fig/azimuth-east_right.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/azimuth-east_right.svg` & `eradiate-0.23.2rc4/docs/fig/azimuth-east_right.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/azimuth-north_left.png` & `eradiate-0.23.2rc4/docs/fig/azimuth-north_left.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/azimuth-north_left.svg` & `eradiate-0.23.2rc4/docs/fig/azimuth-north_left.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/azimuth-north_right.png` & `eradiate-0.23.2rc4/docs/fig/azimuth-north_right.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/azimuth-north_right.svg` & `eradiate-0.23.2rc4/docs/fig/azimuth-north_right.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/azimuth-south_left.png` & `eradiate-0.23.2rc4/docs/fig/azimuth-south_left.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/azimuth-south_left.svg` & `eradiate-0.23.2rc4/docs/fig/azimuth-south_left.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/azimuth-south_right.png` & `eradiate-0.23.2rc4/docs/fig/azimuth-south_right.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/azimuth-south_right.svg` & `eradiate-0.23.2rc4/docs/fig/azimuth-south_right.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/azimuth-west_left.png` & `eradiate-0.23.2rc4/docs/fig/azimuth-west_left.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/azimuth-west_left.svg` & `eradiate-0.23.2rc4/docs/fig/azimuth-west_left.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/azimuth-west_right.png` & `eradiate-0.23.2rc4/docs/fig/azimuth-west_right.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/azimuth-west_right.svg` & `eradiate-0.23.2rc4/docs/fig/azimuth-west_right.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/cartesian-coordinate-system.png` & `eradiate-0.23.2rc4/docs/fig/cartesian-coordinate-system.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/cartesian-coordinate-system.svg` & `eradiate-0.23.2rc4/docs/fig/cartesian-coordinate-system.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/cuboid_leaf_cloud_params.png` & `eradiate-0.23.2rc4/docs/fig/cuboid_leaf_cloud_params.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/cuboid_leaf_cloud_params.svg` & `eradiate-0.23.2rc4/docs/fig/cuboid_leaf_cloud_params.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/diagrams/class_diagram_biosphere.drawio` & `eradiate-0.23.2rc4/docs/fig/diagrams/class_diagram_biosphere.drawio`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/diagrams/cuboid_leaf_cloud_params.drawio` & `eradiate-0.23.2rc4/docs/fig/diagrams/cuboid_leaf_cloud_params.drawio`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/diagrams/package.drawio` & `eradiate-0.23.2rc4/docs/fig/diagrams/package.drawio`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/eradiate-logo-typo-black.png` & `eradiate-0.23.2rc4/docs/fig/eradiate-logo-typo-black.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/eradiate-logo.svg` & `eradiate-0.23.2rc4/docs/fig/eradiate-logo.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/icon_eradiate.png` & `eradiate-0.23.2rc4/docs/fig/icon_eradiate.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/package.png` & `eradiate-0.23.2rc4/docs/fig/package.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/package.svg` & `eradiate-0.23.2rc4/docs/fig/package.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/radiancemeter_hsphere.png` & `eradiate-0.23.2rc4/docs/fig/radiancemeter_hsphere.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/radiancemeter_hsphere.svg` & `eradiate-0.23.2rc4/docs/fig/radiancemeter_hsphere.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/radiancemeter_plane.png` & `eradiate-0.23.2rc4/docs/fig/radiancemeter_plane.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/radiancemeter_plane.svg` & `eradiate-0.23.2rc4/docs/fig/radiancemeter_plane.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/requirement_layers.png` & `eradiate-0.23.2rc4/docs/fig/requirement_layers.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/requirement_layers.svg` & `eradiate-0.23.2rc4/docs/fig/requirement_layers.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/solid_2017.png` & `eradiate-0.23.2rc4/docs/fig/solid_2017.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/spectral_discretization_ckd_atm_interval.png` & `eradiate-0.23.2rc4/docs/fig/spectral_discretization_ckd_atm_interval.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/spectral_discretization_ckd_atm_isolated.png` & `eradiate-0.23.2rc4/docs/fig/spectral_discretization_ckd_atm_isolated.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/spectral_discretization_ckd_noatm_interval.png` & `eradiate-0.23.2rc4/docs/fig/spectral_discretization_ckd_noatm_interval.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/spectral_discretization_ckd_noatm_isolated.png` & `eradiate-0.23.2rc4/docs/fig/spectral_discretization_ckd_noatm_isolated.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/spectral_discretization_mono_atm_interval.png` & `eradiate-0.23.2rc4/docs/fig/spectral_discretization_mono_atm_interval.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/spectral_discretization_mono_atm_isolated.png` & `eradiate-0.23.2rc4/docs/fig/spectral_discretization_mono_atm_isolated.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/spectral_discretization_mono_noatm_interval1.png` & `eradiate-0.23.2rc4/docs/fig/spectral_discretization_mono_noatm_interval1.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/spectral_discretization_mono_noatm_interval2.png` & `eradiate-0.23.2rc4/docs/fig/spectral_discretization_mono_noatm_interval2.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/spectral_discretization_mono_noatm_isolated.png` & `eradiate-0.23.2rc4/docs/fig/spectral_discretization_mono_noatm_isolated.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/spherical-coordinate-system.png` & `eradiate-0.23.2rc4/docs/fig/spherical-coordinate-system.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/spherical-coordinate-system.svg` & `eradiate-0.23.2rc4/docs/fig/spherical-coordinate-system.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/fig/thuillier_2003.png` & `eradiate-0.23.2rc4/docs/fig/thuillier_2003.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/generate_md_cli.py` & `eradiate-0.23.2rc4/docs/generate_md_cli.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/generate_rst_api.py` & `eradiate-0.23.2rc4/docs/generate_rst_api.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/generate_rst_plugins.py` & `eradiate-0.23.2rc4/docs/generate_rst_plugins.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/index.rst` & `eradiate-0.23.2rc4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/make.bat` & `eradiate-0.23.2rc4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/references.bib` & `eradiate-0.23.2rc4/docs/references.bib`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/contributing.rst` & `eradiate-0.23.2rc4/docs/rst/contributing.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/dependencies.rst` & `eradiate-0.23.2rc4/docs/rst/dependencies.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/developer_guide/design_atmosphere.rst` & `eradiate-0.23.2rc4/docs/rst/developer_guide/design_atmosphere.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/developer_guide/dev_install.rst` & `eradiate-0.23.2rc4/docs/rst/developer_guide/dev_install.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/developer_guide/factory_guide.rst` & `eradiate-0.23.2rc4/docs/rst/developer_guide/factory_guide.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/developer_guide/lazy_loading.rst` & `eradiate-0.23.2rc4/docs/rst/developer_guide/lazy_loading.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/developer_guide/radiometric_kernel_interface.rst` & `eradiate-0.23.2rc4/docs/rst/developer_guide/radiometric_kernel_interface.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/developer_guide/scene_generator.rst` & `eradiate-0.23.2rc4/docs/rst/developer_guide/scene_generator.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/developer_guide/update.rst` & `eradiate-0.23.2rc4/docs/rst/developer_guide/update.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/maintainer_guide.rst` & `eradiate-0.23.2rc4/docs/rst/maintainer_guide.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/reference_api/data.rst` & `eradiate-0.23.2rc4/docs/rst/reference_api/data.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/reference_api/eradiate_core.rst` & `eradiate-0.23.2rc4/docs/rst/reference_api/eradiate_core.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/reference_api/experiments.rst` & `eradiate-0.23.2rc4/docs/rst/reference_api/experiments.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/reference_api/factory.rst` & `eradiate-0.23.2rc4/docs/rst/reference_api/factory.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/reference_api/index.rst` & `eradiate-0.23.2rc4/docs/rst/reference_api/index.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/reference_api/kernel.rst` & `eradiate-0.23.2rc4/docs/rst/reference_api/kernel.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/reference_api/pipelines.rst` & `eradiate-0.23.2rc4/docs/rst/reference_api/pipelines.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/reference_api/scenes.rst` & `eradiate-0.23.2rc4/docs/rst/reference_api/scenes.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/reference_api/srf_tools.rst` & `eradiate-0.23.2rc4/docs/rst/reference_api/srf_tools.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/reference_api/test_tools.rst` & `eradiate-0.23.2rc4/docs/rst/reference_api/test_tools.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/reference_api/xarray.rst` & `eradiate-0.23.2rc4/docs/rst/reference_api/xarray.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/user_guide/atmosphere/absorption.rst` & `eradiate-0.23.2rc4/docs/rst/user_guide/atmosphere/absorption.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/user_guide/atmosphere/fig/bad_resolution.png` & `eradiate-0.23.2rc4/docs/rst/user_guide/atmosphere/fig/bad_resolution.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/user_guide/atmosphere/fig/good_resolution.png` & `eradiate-0.23.2rc4/docs/rst/user_guide/atmosphere/fig/good_resolution.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/user_guide/atmosphere/fig/line.png` & `eradiate-0.23.2rc4/docs/rst/user_guide/atmosphere/fig/line.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/user_guide/atmosphere/heterogeneous.rst` & `eradiate-0.23.2rc4/docs/rst/user_guide/atmosphere/heterogeneous.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/user_guide/atmosphere/intro.rst` & `eradiate-0.23.2rc4/docs/rst/user_guide/atmosphere/intro.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/user_guide/atmosphere/molecular.rst` & `eradiate-0.23.2rc4/docs/rst/user_guide/atmosphere/molecular.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/user_guide/atmosphere/rayleigh_scattering.rst` & `eradiate-0.23.2rc4/docs/rst/user_guide/atmosphere/rayleigh_scattering.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/user_guide/basic_concepts.rst` & `eradiate-0.23.2rc4/docs/rst/user_guide/basic_concepts.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/user_guide/conventions.rst` & `eradiate-0.23.2rc4/docs/rst/user_guide/conventions.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/user_guide/data/absorption.rst` & `eradiate-0.23.2rc4/docs/rst/user_guide/data/absorption.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/user_guide/data/atmosphere_radprops.rst` & `eradiate-0.23.2rc4/docs/rst/user_guide/data/atmosphere_radprops.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/user_guide/data/atmosphere_thermoprops.rst` & `eradiate-0.23.2rc4/docs/rst/user_guide/data/atmosphere_thermoprops.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/user_guide/data/ckd.rst` & `eradiate-0.23.2rc4/docs/rst/user_guide/data/ckd.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/user_guide/data/fig/p_interp_rerr_histo_65349.png` & `eradiate-0.23.2rc4/docs/rst/user_guide/data/fig/p_interp_rerr_histo_65349.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/user_guide/data/fig/pt_points.png` & `eradiate-0.23.2rc4/docs/rst/user_guide/data/fig/pt_points.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/user_guide/data/fig/w_interp_rerr_histo_101325.png` & `eradiate-0.23.2rc4/docs/rst/user_guide/data/fig/w_interp_rerr_histo_101325.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/user_guide/data/intro.rst` & `eradiate-0.23.2rc4/docs/rst/user_guide/data/intro.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/user_guide/data/particle_radprops.rst` & `eradiate-0.23.2rc4/docs/rst/user_guide/data/particle_radprops.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/user_guide/data/solar_irradiance.rst` & `eradiate-0.23.2rc4/docs/rst/user_guide/data/solar_irradiance.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/user_guide/data/spectra-us76_u86_4.rst` & `eradiate-0.23.2rc4/docs/rst/user_guide/data/spectra-us76_u86_4.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/user_guide/data/srf.rst` & `eradiate-0.23.2rc4/docs/rst/user_guide/data/srf.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/user_guide/index.rst` & `eradiate-0.23.2rc4/docs/rst/user_guide/index.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/user_guide/install.rst` & `eradiate-0.23.2rc4/docs/rst/user_guide/install.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/user_guide/onedim_experiment.rst` & `eradiate-0.23.2rc4/docs/rst/user_guide/onedim_experiment.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/user_guide/package_structure.rst` & `eradiate-0.23.2rc4/docs/rst/user_guide/package_structure.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/user_guide/spectral_discretization.rst` & `eradiate-0.23.2rc4/docs/rst/user_guide/spectral_discretization.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/rst/user_guide/unit_guide_user.rst` & `eradiate-0.23.2rc4/docs/rst/user_guide/unit_guide_user.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/src/CHANGELOG.md` & `eradiate-0.23.2rc4/docs/src/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/docs/src/reference_cli.md` & `eradiate-0.23.2rc4/docs/src/reference_cli.md`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/pyproject.toml` & `eradiate-0.23.2rc4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/requirements/conda/environment-dependencies-linux-64.lock` & `eradiate-0.23.2rc4/requirements/conda/environment-dependencies-linux-64.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Generated by conda-lock.
 # platform: linux-64
-# input_hash: 7978c39d039c87858107e33a8ec1a02d28c787cf6cb89fe0234d346f144c81b5
+# input_hash: 6dda966feaa106a4b9c32ba6874b70e59748f77d06acaa3ddb4b6ebf7a7dda44
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2#d7c89558ba9fa0495403155b64376d81
 https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2023.5.7-hbcca054_0.conda#f5c65075fc34438d5b456c7f3f5ab695
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-dejavu-sans-mono-2.37-hab24e00_0.tar.bz2#0c96522c6bdaed4b1566d11387caaf45
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-inconsolata-3.000-h77eed37_0.tar.bz2#34893075a5c9e55cdafac56607368fc6
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-source-code-pro-2.038-h77eed37_0.tar.bz2#4d59c254e01d9cde7957100457e2d5fb
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-ubuntu-0.83-hab24e00_0.tar.bz2#19410c3df09dfb12d1206132a1d357c5
@@ -25,27 +25,27 @@
 https://conda.anaconda.org/conda-forge/linux-64/gettext-0.21.1-h27087fc_0.tar.bz2#14947d8770185e5153fdd04d4673ed37
 https://conda.anaconda.org/conda-forge/linux-64/graphite2-1.3.13-h58526e2_1001.tar.bz2#8c54672728e8ec6aa6db90cf2806d220
 https://conda.anaconda.org/conda-forge/linux-64/icu-72.1-hcb278e6_0.conda#7c8d20d847bb45f56bd941578fcfa146
 https://conda.anaconda.org/conda-forge/linux-64/keyutils-1.6.1-h166bdaf_0.tar.bz2#30186d27e2c9fa62b45fb1476b7200e3
 https://conda.anaconda.org/conda-forge/linux-64/lame-3.100-h166bdaf_1003.tar.bz2#a8832b479f93521a9e7b5b743803be51
 https://conda.anaconda.org/conda-forge/linux-64/lerc-4.0.0-h27087fc_0.tar.bz2#76bbff344f0134279f225174e9064c8f
 https://conda.anaconda.org/conda-forge/linux-64/libaec-1.0.6-hcb278e6_1.conda#0f683578378cddb223e7fd24f785ab2a
-https://conda.anaconda.org/conda-forge/linux-64/libbrotlicommon-1.0.9-h166bdaf_8.tar.bz2#9194c9bf9428035a05352d031462eae4
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlicommon-1.0.9-h166bdaf_9.conda#61641e239f96eae2b8492dc7e755828c
 https://conda.anaconda.org/conda-forge/linux-64/libdeflate-1.18-h0b41bf4_0.conda#6aa9c9de5542ecb07fdda9ca626252d8
 https://conda.anaconda.org/conda-forge/linux-64/libev-4.33-h516909a_1.tar.bz2#6f8720dff19e17ce5d48cfe7f3d2f0a3
 https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.5.0-hcb278e6_1.conda#6305a3dd2752c76335295da4e581f2fd
 https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2#d645c6d2ac96843a2bfaccd2d62b3ac3
 https://conda.anaconda.org/conda-forge/linux-64/libiconv-1.17-h166bdaf_0.tar.bz2#b62b52da46c39ee2bc3c162ac7f1804d
 https://conda.anaconda.org/conda-forge/linux-64/libjpeg-turbo-2.1.5.1-h0b41bf4_0.conda#1edd9e67bdb90d78cea97733ff6b54e6
 https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.0-h7f98852_0.tar.bz2#39b1328babf85c7c3a61636d9cd50206
-https://conda.anaconda.org/conda-forge/linux-64/libogg-1.3.4-h7f98852_1.tar.bz2#6e8cc2173440d77708196c5b93771680
+https://repo.anaconda.com/pkgs/main/linux-64/libogg-1.3.5-h27cfd23_1.conda#710ee7fdb0ddf7591a5af7ca7eb4d73d
 https://conda.anaconda.org/conda-forge/linux-64/libopenblas-0.3.23-pthreads_h80387f5_0.conda#9c5ea51ccb8ffae7d06c645869d24ce6
 https://conda.anaconda.org/conda-forge/linux-64/libopus-1.3.1-h7f98852_1.tar.bz2#15345e56d527b330e1cacbdf58676e8f
 https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda#40b61aab5c7ba9ff276c41cfffe6b80b
-https://conda.anaconda.org/conda-forge/linux-64/libwebp-base-1.3.0-h0b41bf4_0.conda#0d4a7508d8c6c65314f2b9c1f56ad408
+https://conda.anaconda.org/conda-forge/linux-64/libwebp-base-1.3.1-hd590300_0.conda#82bf6f63eb15ef719b556b63feec3a77
 https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-hd590300_5.conda#f36c115f1ee199da648e0597ec2047ad
 https://conda.anaconda.org/conda-forge/linux-64/lz4-c-1.9.4-hcb278e6_0.conda#318b08df404f9c9be5712aaa5a6f0bb0
 https://conda.anaconda.org/conda-forge/linux-64/mpg123-1.31.3-hcb278e6_0.conda#141a126675b6d1a4eabb111a4a353898
 https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.4-hcb278e6_0.conda#681105bccc2a3f7f1a837d47d39c9179
 https://conda.anaconda.org/conda-forge/linux-64/nspr-4.35-h27087fc_0.conda#da0ec11a6454ae19bff5b02ed881a2b1
 https://conda.anaconda.org/conda-forge/linux-64/openssl-3.1.1-hd590300_1.conda#2e1d7b458ac8f1e3ca4e18b77add6277
 https://conda.anaconda.org/conda-forge/linux-64/pixman-0.40.0-h36c2ea0_0.tar.bz2#660e72c82f2e75a6b3fe6a6e75c79f19
@@ -59,58 +59,59 @@
 https://conda.anaconda.org/conda-forge/linux-64/xorg-xextproto-7.3.0-h0b41bf4_1003.conda#bce9f945da8ad2ae9b1d7165a64d0f87
 https://conda.anaconda.org/conda-forge/linux-64/xorg-xf86vidmodeproto-2.3.1-h7f98852_1002.tar.bz2#3ceea9668625c18f19530de98b15d5b0
 https://conda.anaconda.org/conda-forge/linux-64/xorg-xproto-7.0.31-h7f98852_1007.tar.bz2#b4a4381d54784606820704f7b5f05a15
 https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2#2161070d867d1b1204ea749c8eec4ef0
 https://conda.anaconda.org/conda-forge/linux-64/expat-2.5.0-hcb278e6_1.conda#8b9b5aca60558d02ddaa09d599e55920
 https://conda.anaconda.org/conda-forge/linux-64/hdf4-4.2.15-h501b40f_6.conda#c3e9338e15d90106f467377017352b97
 https://conda.anaconda.org/conda-forge/linux-64/libblas-3.9.0-17_linux64_openblas.conda#57fb44770b1bc832fb2dbefa1bd502de
-https://conda.anaconda.org/conda-forge/linux-64/libbrotlidec-1.0.9-h166bdaf_8.tar.bz2#4ae4d7795d33e02bd20f6b23d91caf82
-https://conda.anaconda.org/conda-forge/linux-64/libbrotlienc-1.0.9-h166bdaf_8.tar.bz2#04bac51ba35ea023dc48af73c1c88c25
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlidec-1.0.9-h166bdaf_9.conda#081aa22f4581c08e4372b0b6c2f8478e
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlienc-1.0.9-h166bdaf_9.conda#1f0a03af852a9659ed2bf08f2f1704fd
 https://conda.anaconda.org/conda-forge/linux-64/libcap-2.67-he9d0100_0.conda#d05556c80caffff164d17bdea0105a1a
 https://conda.anaconda.org/conda-forge/linux-64/libedit-3.1.20191231-he28a2e2_2.tar.bz2#4d331e44109e3f0e19b4cb8f9b82f3e1
 https://conda.anaconda.org/conda-forge/linux-64/libevent-2.1.12-hf998b51_1.conda#a1cfcc585f0c42bf8d5546bb1dfb668d
-https://conda.anaconda.org/conda-forge/linux-64/libflac-1.4.2-h27087fc_0.tar.bz2#7daf72d8e2a8e848e11d63ed6d1026e0
+https://conda.anaconda.org/conda-forge/linux-64/libflac-1.4.3-h59595ed_0.conda#ee48bf17cc83a00f59ca1494d5646869
 https://conda.anaconda.org/conda-forge/linux-64/libgpg-error-1.47-h71f35ed_0.conda#c2097d0b46367996f09b4e8e4920384a
 https://conda.anaconda.org/conda-forge/linux-64/libnghttp2-1.52.0-h61bc06f_0.conda#613955a50485812985c059e7b269f42e
 https://conda.anaconda.org/conda-forge/linux-64/libpng-1.6.39-h753d276_0.conda#e1c890aebdebbfbf87e2c917187b4416
 https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.42.0-h2797004_0.conda#fdaae20a1cf7cd62130a0973190a31b7
 https://conda.anaconda.org/conda-forge/linux-64/libssh2-1.11.0-h0841786_0.conda#1f5a58e686b13bcfde88b93f547d23fe
 https://conda.anaconda.org/conda-forge/linux-64/libvorbis-1.3.7-h9c3ff4c_0.tar.bz2#309dec04b70a3cc0f1e84a4013683bc0
 https://conda.anaconda.org/conda-forge/linux-64/libxcb-1.15-h0b41bf4_0.conda#33277193f5b92bad9fdd230eb700929c
 https://conda.anaconda.org/conda-forge/linux-64/libxml2-2.11.4-h0d562d8_0.conda#e46fad17d5fb57316b956f88dca765e4
 https://conda.anaconda.org/conda-forge/linux-64/libzip-1.9.2-hc929e4a_1.tar.bz2#5b122b50e738c4be5c3f2899f010d7cf
-https://conda.anaconda.org/conda-forge/linux-64/mysql-common-8.0.33-hf1915f5_0.conda#aa8b86066614c4573f6db62c91978fa9
+https://conda.anaconda.org/conda-forge/linux-64/mysql-common-8.0.33-hf1915f5_1.conda#b241363e3b72bae6dfbd31e9fecf7d26
 https://conda.anaconda.org/conda-forge/linux-64/pcre2-10.40-hc3806b6_0.tar.bz2#69e2c796349cd9b273890bee0febfe1b
 https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda#47d31b792659ce70f470b5c82fdfb7a4
 https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.12-h27826a3_0.tar.bz2#5b8c42eb62e9fc961af70bdd6a26e168
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libsm-1.2.4-h7391055_0.conda#93ee23f12bc2e684548181256edd2cf6
 https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.13-hd590300_5.conda#68c34ec6149623be41a1933ab996a209
 https://conda.anaconda.org/conda-forge/linux-64/zstd-1.5.2-h3eb15da_6.conda#6b63daed8feeca47be78f323e793d555
 https://conda.anaconda.org/conda-forge/linux-64/blosc-1.21.4-h0f2a231_0.conda#876286b5941933a0f558777e57d883cc
-https://conda.anaconda.org/conda-forge/linux-64/brotli-bin-1.0.9-h166bdaf_8.tar.bz2#e5613f2bc717e9945840ff474419b8e4
+https://conda.anaconda.org/conda-forge/linux-64/brotli-bin-1.0.9-h166bdaf_9.conda#d47dee1856d9cb955b8076eeff304a5b
 https://conda.anaconda.org/conda-forge/linux-64/freetype-2.12.1-hca18f0e_1.conda#e1232042de76d24539a436d37597eb06
 https://conda.anaconda.org/conda-forge/linux-64/krb5-1.20.1-h81ceb04_0.conda#89a41adce7106749573d883b2f657d78
 https://conda.anaconda.org/conda-forge/linux-64/libcblas-3.9.0-17_linux64_openblas.conda#7ef0969b00fe3d6eef56a8151d3afb29
 https://conda.anaconda.org/conda-forge/linux-64/libgcrypt-1.10.1-h166bdaf_0.tar.bz2#f967fc95089cd247ceed56eda31de3a9
 https://conda.anaconda.org/conda-forge/linux-64/libglib-2.76.3-hebfc3b9_0.conda#a64f11b244b2c112cd3fa1cbe9493999
 https://conda.anaconda.org/conda-forge/linux-64/liblapack-3.9.0-17_linux64_openblas.conda#a2103882c46492e26500fcb56c03de8b
 https://conda.anaconda.org/conda-forge/linux-64/libllvm16-16.0.6-h5cf9203_0.conda#753e078cccad40fe4b396bdcf27a3c15
 https://conda.anaconda.org/conda-forge/linux-64/libsndfile-1.2.0-hb75c966_0.conda#c648d19cd9c8625898d5d370414de7c7
 https://conda.anaconda.org/conda-forge/linux-64/libtiff-4.5.1-h8b53f26_0.conda#8ad377fb60abab446a9f02c62b3c2190
-https://conda.anaconda.org/conda-forge/linux-64/mysql-libs-8.0.33-hca2cd23_0.conda#276339b0115d92c6e0793dcdc7afe308
+https://conda.anaconda.org/conda-forge/linux-64/mysql-libs-8.0.33-hca2cd23_1.conda#a04ac37f0659929f3ba0f33c7f3d750f
 https://conda.anaconda.org/conda-forge/linux-64/nss-3.89-he45b914_0.conda#2745719a58eeaab6657256a3f142f099
 https://conda.anaconda.org/conda-forge/linux-64/python-3.8.17-he550d4f_0_cpython.conda#72d038de0a228e4f0ef4011940641293
 https://conda.anaconda.org/conda-forge/linux-64/xcb-util-0.4.0-hd590300_1.conda#9bfac7ccd94d54fd21a0501296d60424
 https://conda.anaconda.org/conda-forge/linux-64/xcb-util-keysyms-0.4.0-h8ee46fc_1.conda#632413adcd8bc16b515cab87a2932913
 https://conda.anaconda.org/conda-forge/linux-64/xcb-util-renderutil-0.3.9-hd590300_1.conda#e995b155d938b6779da6ace6c6b13816
 https://conda.anaconda.org/conda-forge/linux-64/xcb-util-wm-0.4.1-h8ee46fc_1.conda#90108a432fb5c6150ccfee3f03388656
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libx11-1.8.6-h8ee46fc_0.conda#7590b76c3d11d21caa44f3fc38ac584a
-https://conda.anaconda.org/conda-forge/noarch/aenum-3.1.12-pyhd8ed1ab_0.conda#602716538da00b2ca3cc85c4d35c0245
+https://conda.anaconda.org/conda-forge/noarch/aenum-3.1.15-pyhd8ed1ab_0.conda#24cff7ab050ebb8a16bdeb02e8ed6f63
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
-https://conda.anaconda.org/conda-forge/linux-64/brotli-1.0.9-h166bdaf_8.tar.bz2#2ff08978892a3e8b954397c461f18418
+https://conda.anaconda.org/conda-forge/linux-64/brotli-1.0.9-h166bdaf_9.conda#4601544b4982ba1861fa9b9c607b2c06
+https://conda.anaconda.org/conda-forge/linux-64/brotli-python-1.0.9-py38hfa26641_9.conda#d056745008e5ed73210a31dcfd4d183a
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
 https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-unix_pyhd8ed1ab_2.tar.bz2#20e4087407c7cb04a40817114b333dbf
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/noarch/cycler-0.11.0-pyhd8ed1ab_0.tar.bz2#a50559fad0affdbb33729a68669ca1cb
 https://conda.anaconda.org/conda-forge/linux-64/dbus-1.13.6-h5008d03_3.tar.bz2#ecfff944ba3960ecb334b9a2663d708d
 https://conda.anaconda.org/conda-forge/linux-64/fontconfig-2.14.2-h14ed4e7_0.conda#0f69b688f52ff6da70bccb7ff7001d1d
@@ -122,75 +123,75 @@
 https://conda.anaconda.org/conda-forge/linux-64/libclang13-16.0.6-default_h4d60ac6_0.conda#b10174a063ec195f8fe1b278282c3149
 https://conda.anaconda.org/conda-forge/linux-64/libcups-2.3.3-h36d4200_3.conda#c9f4416a34bc91e0eb029f912c68f81f
 https://conda.anaconda.org/conda-forge/linux-64/libcurl-8.1.2-h409715c_0.conda#50c873c9660ed116707ae15b663928d8
 https://conda.anaconda.org/conda-forge/linux-64/libpq-15.3-hbcd7760_1.conda#8afb2a97d256ffde95b91a6283bc598c
 https://conda.anaconda.org/conda-forge/linux-64/libsystemd0-253-h8c4010b_1.conda#9176b1e2cb8beca37a7510b0e801e38f
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.0-pyhd8ed1ab_0.tar.bz2#f8dab71fdc13b1bf29a01248b156d268
 https://conda.anaconda.org/conda-forge/noarch/munkres-1.1.4-pyh9f0ad1d_0.tar.bz2#2ba8498c1018c1e9c61eb99b973dfe19
-https://conda.anaconda.org/conda-forge/linux-64/numpy-1.24.3-py38h59b608b_0.conda#5836e4ab0399136ede58446a4776b2ff
+https://conda.anaconda.org/conda-forge/linux-64/numpy-1.24.4-py38h59b608b_0.conda#8c3e050afeeb2b32575bdb8955cc67b2
 https://conda.anaconda.org/conda-forge/linux-64/openjpeg-2.5.0-hfec8fc6_2.conda#5ce6a42505c6e9e6151c54c3ec8d68ea
 https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
 https://conda.anaconda.org/conda-forge/noarch/pint-0.21-pyhd8ed1ab_0.conda#8d7b829e37d78447569c180f9d827005
 https://conda.anaconda.org/conda-forge/noarch/ply-3.11-py_1.tar.bz2#7205635cd71531943440fbfe3b6b5727
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
 https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.1.0-pyhd8ed1ab_0.conda#d3ed087d1f7f8f5590e8e87b57a8ce64
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
 https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
 https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml.clib-0.2.7-py38h1de0b5d_1.conda#9afa2fc3c51cc4e7d1589c38e4e00d5c
-https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda#3b68bc43ec6baa48f7354a446267eefe
+https://conda.anaconda.org/conda-forge/noarch/setuptools-68.0.0-pyhd8ed1ab_0.conda#5a7739d0f57ee64133c9d32e6507c46d
 https://conda.anaconda.org/conda-forge/noarch/shellingham-1.4.0-pyh44b312d_0.tar.bz2#437655338696f9d0dfdb0a024e66b255
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/linux-64/tornado-6.3.2-py38h01eb140_0.conda#3db869202b0e523d606d13e81ca79ab6
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.3-pyha770c72_0.conda#4a3014a4d107d15475d106b751c4e352
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.0-pyha770c72_0.conda#c76ebd4731d3668ba16975a30ef19d0d
 https://conda.anaconda.org/conda-forge/linux-64/unicodedata2-15.0.0-py38h0a891b7_0.tar.bz2#44421904760e9f5ae2035193e04360f0
 https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
 https://conda.anaconda.org/conda-forge/linux-64/xcb-util-image-0.4.0-h8ee46fc_1.conda#9d7bcddf49cbf727730af10e71022c73
 https://conda.anaconda.org/conda-forge/linux-64/xkeyboard-config-2.39-hd590300_0.conda#d88c7fc8a11858fb14761832e4da1954
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxext-1.3.4-h0b41bf4_2.conda#82b6df12252e6f32402b96dacc656fec
-https://conda.anaconda.org/conda-forge/linux-64/xorg-libxrender-0.9.10-h7f98852_1003.tar.bz2#f59c1242cc1dd93e72c2ee2b360979eb
+https://conda.anaconda.org/conda-forge/linux-64/xorg-libxrender-0.9.11-hd590300_0.conda#ed67c36f215b310412b2af935bf3e530
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
 https://conda.anaconda.org/conda-forge/linux-64/cairo-1.16.0-hbbf8b49_1016.conda#c1dd96500b9b1a75e9e511931f415cbc
 https://conda.anaconda.org/conda-forge/linux-64/cftime-1.6.2-py38h26c90d9_1.tar.bz2#dcc025a7bb54374979c500c2e161fac9
 https://conda.anaconda.org/conda-forge/linux-64/contourpy-1.1.0-py38h7f3f72f_0.conda#0fdf3cc879156e0234e05962d55b6502
 https://conda.anaconda.org/conda-forge/linux-64/curl-8.1.2-h409715c_0.conda#9f88cfb15b7d08b25880b138f91e0eb4
 https://conda.anaconda.org/eradiate/noarch/dessinemoi-23.1.0-py_0.tar.bz2#490780e63e113a7dc444bd068e049bfe
 https://conda.anaconda.org/conda-forge/noarch/environ-config-22.1.0-pyhd8ed1ab_0.tar.bz2#a1103faffa0a877313c1fba776aa0fc0
 https://conda.anaconda.org/conda-forge/linux-64/fonttools-4.40.0-py38h01eb140_0.conda#f893b6bac56c477dd71498569b4a9022
 https://conda.anaconda.org/conda-forge/linux-64/glib-2.76.3-hfc55251_0.conda#950e02f5665f5f4ff0437a6acba58798
-https://conda.anaconda.org/conda-forge/linux-64/hdf5-1.14.0-nompi_hb72d44e_103.conda#975973a4350ab45ff1981fe535a12af5
+https://conda.anaconda.org/conda-forge/linux-64/hdf5-1.14.1-nompi_h4f84152_100.conda#ff9ae10aa224826c07da7ef26cb0b717
 https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
 https://conda.anaconda.org/conda-forge/linux-64/libclang-16.0.6-default_h1cdf331_0.conda#e976871e132fe506da52c1240229246a
 https://conda.anaconda.org/conda-forge/linux-64/libxkbcommon-1.5.0-h5d7e998_3.conda#c91ea308d7bf70b62ddda568478aa03b
 https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-3.0.0-pyhd8ed1ab_0.conda#93a8e71256479c62074356ef6ebf501b
-https://conda.anaconda.org/conda-forge/linux-64/pillow-9.5.0-py38h885162f_1.conda#0eec8a20a17f17ec9e0b6839be466866
+https://conda.anaconda.org/conda-forge/linux-64/pillow-10.0.0-py38h885162f_0.conda#777c54134d5422a867aed7084cf5db5e
 https://conda.anaconda.org/eradiate/noarch/pinttrs-23.2.0-py_0.tar.bz2#1aebe9fa813278f719fa8e31d8000452
 https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
 https://conda.anaconda.org/conda-forge/noarch/portion-2.4.0-pyhd8ed1ab_0.conda#9d34bac22e169b41f4e34525a140c13b
 https://conda.anaconda.org/conda-forge/linux-64/pulseaudio-client-16.1-hb77b528_4.conda#8f349ca16d30950aa00870484d9d30c4
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
 https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml-0.17.32-py38h01eb140_0.conda#c92cc8efb1341f90ea5f51f576480580
 https://conda.anaconda.org/conda-forge/linux-64/sip-6.7.9-py38h17151c0_0.conda#6a54fd42b71a8b1c5f9c4a691270cdf1
 https://conda.anaconda.org/conda-forge/noarch/tqdm-4.65.0-pyhd8ed1ab_1.conda#ed792aff3acb977d09c7013358097f83
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.3-hd8ed1ab_0.conda#3876f650ed7d0f95d70fa4b647621909
-https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.3-pyhd8ed1ab_0.conda#ae465d0fbf9f1979cb2d8d4043d885e2
-https://conda.anaconda.org/conda-forge/linux-64/gstreamer-1.22.3-h977cf35_1.conda#410ed3b168e5a139d12ebaf4143072cd
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.0-hd8ed1ab_0.conda#37761dccc7ca8eaa08c60c4f62eb2dcc
+https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.3-pyhd8ed1ab_1.conda#89efeecbb24c62e2f1ed0b8ca959ec69
+https://repo.anaconda.com/pkgs/main/linux-64/gstreamer-1.22.3-h5eee18b_0.conda#c2ffbb79cb2f51b042de223d482b7b29
 https://conda.anaconda.org/conda-forge/linux-64/harfbuzz-7.3.0-hdb3a94d_0.conda#765bc76c0dfaf24ff9d8a2935b2510df
 https://conda.anaconda.org/conda-forge/noarch/importlib-resources-5.12.0-pyhd8ed1ab_0.conda#3544c818f0720c89eb16ae6940ab440b
-https://conda.anaconda.org/conda-forge/linux-64/libnetcdf-4.9.2-nompi_h0f3d0bb_105.conda#b5d412441b84305460e9df8a016a3392
+https://conda.anaconda.org/conda-forge/linux-64/libnetcdf-4.9.2-nompi_h78c856c_106.conda#47665bf3dec451455474556ecd940ed2
 https://conda.anaconda.org/conda-forge/linux-64/pandas-1.5.3-py38hdc8b05c_1.conda#c944b033a2126e7f714a7ecaecb22011
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.6.0-pyhd8ed1ab_0.conda#741384b21c1b512617f4ee4ea8457c5d
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.8.0-pyhd8ed1ab_0.conda#3e4aca765371893ad848397794600632
 https://conda.anaconda.org/conda-forge/linux-64/pyqt5-sip-12.11.0-py38h8dc9893_3.conda#7bb0328b4a0f857aeb432426b9a5f908
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/noarch/rich-13.4.2-pyhd8ed1ab_0.conda#f993baacc175e83fafd6b846e9c4c8a2
-https://conda.anaconda.org/conda-forge/linux-64/gst-plugins-base-1.22.3-h938bd60_1.conda#1f317eb7f00db75f4112a07476345376
+https://repo.anaconda.com/pkgs/main/linux-64/gst-plugins-base-1.22.3-he621ea3_0.conda#27be67671dce7d6d8c53bf6260090c15
 https://conda.anaconda.org/conda-forge/linux-64/matplotlib-base-3.7.1-py38hd6c3c57_0.conda#3b8ba76acae09fbd4b2247c4ee4c0324
-https://conda.anaconda.org/conda-forge/linux-64/netcdf4-1.6.4-nompi_py38hdfa7aa7_100.conda#ce30178fb90d4509c3fda5b572124200
+https://conda.anaconda.org/conda-forge/linux-64/netcdf4-1.6.4-nompi_py38h383a0a3_101.conda#693cbd2ee4f62c8a2521cfaf7560b647
 https://conda.anaconda.org/conda-forge/noarch/pooch-1.7.0-pyha770c72_3.conda#5936894aade8240c867d292aa0d980c6
 https://conda.anaconda.org/conda-forge/noarch/typer-0.9.0-pyhd8ed1ab_0.conda#5030a13b2fe5e143d5956d4943d3018f
 https://conda.anaconda.org/conda-forge/noarch/xarray-2023.1.0-pyhd8ed1ab_0.conda#c11eb03b6f77a0d22ae88c454c940f55
 https://conda.anaconda.org/conda-forge/linux-64/qt-main-5.15.8-h01ceb2d_12.conda#60fd4bdf187f88bac57cdc1a052f2811
 https://conda.anaconda.org/conda-forge/linux-64/scipy-1.10.1-py38h59b608b_3.conda#2f2a57462fcfbc67dfdbb0de6f7484c2
 https://conda.anaconda.org/conda-forge/linux-64/pyqt-5.15.7-py38ha0d8c90_3.conda#e965dc172d67920d058ac2b3a0e27565
 https://conda.anaconda.org/conda-forge/linux-64/matplotlib-3.7.1-py38h578d9bd_0.conda#50ff9e0a3dd459a0ca365741072bf9a2
```

### Comparing `eradiate-0.23.2rc3/requirements/conda/environment-dependencies-osx-64.lock` & `eradiate-0.23.2rc4/requirements/conda/environment-dependencies-osx-64.lock`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,62 @@
 # Generated by conda-lock.
 # platform: osx-64
-# input_hash: 43b100c35a9f50d9602c3c883dfa4017d94b56250d5acd29f7e2e8f351eb49c8
+# input_hash: 64bbf5cbb57a84037576a4bb20f3fcdd7659bb44787ea5ed3dd2b4bdf1110c04
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h0d85af4_4.tar.bz2#37edc4e6304ca87316e160f5ca0bd1b5
 https://conda.anaconda.org/conda-forge/osx-64/c-ares-1.19.1-h0dc2134_0.conda#b3e62631b4e1b9801477523ce1d6f355
 https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2023.5.7-h8857fd0_0.conda#b704e4b79ba0d887c4870b7b09d6a4df
 https://conda.anaconda.org/conda-forge/osx-64/icu-72.1-h7336db1_0.conda#c9689510a50a4bb2ae978421671a125e
-https://conda.anaconda.org/conda-forge/osx-64/libbrotlicommon-1.0.9-hb7f2c08_8.tar.bz2#37157d273eaf3bc7d6862104161d9ec9
+https://conda.anaconda.org/conda-forge/osx-64/libbrotlicommon-1.0.9-hb7f2c08_9.conda#ee1ee8c79c3426229ad03290573be552
 https://conda.anaconda.org/conda-forge/osx-64/libcxx-16.0.6-hd57cbcb_0.conda#7d6972792161077908b62971802f289a
 https://conda.anaconda.org/conda-forge/osx-64/libdeflate-1.18-hac1461d_0.conda#3d131584456b277ce0871e6481fde49b
 https://conda.anaconda.org/conda-forge/osx-64/libev-4.33-haf1e3a3_1.tar.bz2#79dc2be110b2a3d1e97ec21f691c50ad
 https://conda.anaconda.org/conda-forge/osx-64/libffi-3.4.2-h0d85af4_5.tar.bz2#ccb34fb14960ad8b125962d3d79b31a9
 https://conda.anaconda.org/conda-forge/osx-64/libiconv-1.17-hac89ed1_0.tar.bz2#691d103d11180486154af49c037b7ed9
 https://conda.anaconda.org/conda-forge/osx-64/libjpeg-turbo-2.1.5.1-hb7f2c08_0.conda#d7309a152b9b79799063b8bb47e34a3a
-https://conda.anaconda.org/conda-forge/osx-64/libwebp-base-1.3.0-hb7f2c08_0.conda#18981e4c840126d6118d8952485fea51
+https://conda.anaconda.org/conda-forge/osx-64/libwebp-base-1.3.1-h0dc2134_0.conda#a25a41b5be3fed4b671a58b998dcf89b
 https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-h8a1eda9_5.conda#4a3ad23f6e16f99c04e166767193d700
 https://conda.anaconda.org/conda-forge/osx-64/llvm-openmp-16.0.6-hff08bdf_0.conda#39a5227d906f75102bf8586741690128
 https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.4-hf0c8a7f_0.conda#c3dbae2411164d9b02c69090a9a91857
 https://conda.anaconda.org/conda-forge/osx-64/pthread-stubs-0.4-hc929b4f_1001.tar.bz2#addd19059de62181cd11ae8f4ef26084
 https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.8-3_cp38.conda#ff192f59f7fe23555612030493a079f8
 https://conda.anaconda.org/conda-forge/osx-64/xorg-libxau-1.0.11-h0dc2134_0.conda#9566b4c29274125b0266d0177b5eb97b
 https://conda.anaconda.org/conda-forge/osx-64/xorg-libxdmcp-1.1.3-h35c211d_0.tar.bz2#86ac76d6bf1cbb9621943eb3bd9ae36e
 https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2#a72f9d4ea13d55d745ff1ed594747f10
 https://conda.anaconda.org/conda-forge/osx-64/hdf4-4.2.15-h9804679_6.conda#c13d8841112ba7f5931d1d60631394f3
 https://conda.anaconda.org/conda-forge/osx-64/lerc-4.0.0-hb486fe8_0.tar.bz2#f9d6a4c82889d5ecedec1d90eb673c55
 https://conda.anaconda.org/conda-forge/osx-64/libaec-1.0.6-hf0c8a7f_1.conda#7c0f82f435ab4c48d65dc9b28db2ad9e
-https://conda.anaconda.org/conda-forge/osx-64/libbrotlidec-1.0.9-hb7f2c08_8.tar.bz2#7f952a036d9014b4dab96c6ea0f8c2a7
-https://conda.anaconda.org/conda-forge/osx-64/libbrotlienc-1.0.9-hb7f2c08_8.tar.bz2#b36a3bfe866d9127f25f286506982166
+https://conda.anaconda.org/conda-forge/osx-64/libbrotlidec-1.0.9-hb7f2c08_9.conda#4043ef9fe42e178785e0e1853b79bdf9
+https://conda.anaconda.org/conda-forge/osx-64/libbrotlienc-1.0.9-hb7f2c08_9.conda#b64d4dcc70aa141db7fccbf13bad81e1
 https://conda.anaconda.org/conda-forge/osx-64/libedit-3.1.20191231-h0678c8f_2.tar.bz2#6016a8a1d0e63cac3de2c352cd40208b
 https://conda.anaconda.org/conda-forge/osx-64/libgfortran5-12.2.0-he409387_31.conda#5a544130e584b1f204ac896ff071d5b3
 https://conda.anaconda.org/conda-forge/osx-64/libpng-1.6.39-ha978bb4_0.conda#35e4928794c5391aec14ffdf1deaaee5
 https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.42.0-h58db7d2_0.conda#a7d3b44b7b0c9901ac7813b7a0462893
 https://conda.anaconda.org/conda-forge/osx-64/libxcb-1.15-hb7f2c08_0.conda#5513f57e0238c87c12dffedbcc9c1a4a
 https://conda.anaconda.org/conda-forge/osx-64/libxml2-2.11.4-hd95e348_0.conda#681f8dda25e73a830d774a37b9839c85
 https://conda.anaconda.org/conda-forge/osx-64/lz4-c-1.9.4-hf0c8a7f_0.conda#aa04f7143228308662696ac24023f991
 https://conda.anaconda.org/conda-forge/osx-64/openssl-3.1.1-h8a1eda9_1.conda#c7822d6ee74e34af1fd74365cfd18983
 https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda#f17f77f2acf4d344734bda76829ce14e
 https://conda.anaconda.org/conda-forge/osx-64/snappy-1.1.10-h225ccf5_0.conda#4320a8781f14cd959689b86e349f3b73
 https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.12-h5dbffcc_0.tar.bz2#8e9480d9c47061db2ed1b4ecce519a7f
 https://conda.anaconda.org/conda-forge/osx-64/zstd-1.5.2-hbc0c0cd_6.conda#40a188783d3c425bdccc9ae9104acbb8
 https://conda.anaconda.org/conda-forge/osx-64/blosc-1.21.4-heccf04b_0.conda#02e92eb72b9ae4c1745b95d03a9c949e
-https://conda.anaconda.org/conda-forge/osx-64/brotli-bin-1.0.9-hb7f2c08_8.tar.bz2#aac5ad0d8f747ef7f871508146df75d9
+https://conda.anaconda.org/conda-forge/osx-64/brotli-bin-1.0.9-hb7f2c08_9.conda#72c526f7ffa265473e6c75fd90605e52
 https://conda.anaconda.org/conda-forge/osx-64/freetype-2.12.1-h3f81eb7_1.conda#852224ea3e8991a8342228eab274840e
 https://conda.anaconda.org/conda-forge/osx-64/krb5-1.20.1-h049b76e_0.conda#db11fa2968ef0837288fe2d7f5b77a50
 https://conda.anaconda.org/conda-forge/osx-64/libgfortran-5.0.0-11_3_0_h97931a8_31.conda#97451338600bd9c5b535eb224ef6c471
 https://conda.anaconda.org/conda-forge/osx-64/libnghttp2-1.52.0-he2ab024_0.conda#12ac7d100bf260263e30a019517f42a2
 https://conda.anaconda.org/conda-forge/osx-64/libssh2-1.11.0-hd019ec5_0.conda#ca3a72efba692c59a90d4b9fc0dfe774
 https://conda.anaconda.org/conda-forge/osx-64/libtiff-4.5.1-hf955e92_0.conda#56523ed556e3a44c0fd55bcf17045892
 https://conda.anaconda.org/conda-forge/osx-64/libzip-1.9.2-h6db710c_1.tar.bz2#ce732d37e479919f3d22b1ccdeb858ac
 https://conda.anaconda.org/conda-forge/osx-64/python-3.8.17-hf9b03c3_0_cpython.conda#f613b663d3829f325b4ffb626bf612b6
-https://conda.anaconda.org/conda-forge/noarch/aenum-3.1.12-pyhd8ed1ab_0.conda#602716538da00b2ca3cc85c4d35c0245
+https://conda.anaconda.org/conda-forge/noarch/aenum-3.1.15-pyhd8ed1ab_0.conda#24cff7ab050ebb8a16bdeb02e8ed6f63
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
-https://conda.anaconda.org/conda-forge/osx-64/brotli-1.0.9-hb7f2c08_8.tar.bz2#55f612fe4a9b5f6ac76348b6de94aaeb
+https://conda.anaconda.org/conda-forge/osx-64/brotli-1.0.9-hb7f2c08_9.conda#53cff90f0cea22e13e5b791f0e5a8e7d
+https://conda.anaconda.org/conda-forge/osx-64/brotli-python-1.0.9-py38h4cd09af_9.conda#f958e25488ff7e044031bca8a6c5267b
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
 https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-unix_pyhd8ed1ab_2.tar.bz2#20e4087407c7cb04a40817114b333dbf
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/noarch/cycler-0.11.0-pyhd8ed1ab_0.tar.bz2#a50559fad0affdbb33729a68669ca1cb
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/osx-64/kiwisolver-1.4.4-py38h98b9b1b_1.tar.bz2#c11eff21a36bc5809b8e23a05ee71df8
@@ -69,51 +70,51 @@
 https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
 https://conda.anaconda.org/conda-forge/noarch/pint-0.21-pyhd8ed1ab_0.conda#8d7b829e37d78447569c180f9d827005
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
 https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.1.0-pyhd8ed1ab_0.conda#d3ed087d1f7f8f5590e8e87b57a8ce64
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
 https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
 https://conda.anaconda.org/conda-forge/osx-64/ruamel.yaml.clib-0.2.7-py38hef030d1_1.conda#9a8e866b0680b61b2e988b18a1eaecae
-https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda#3b68bc43ec6baa48f7354a446267eefe
+https://conda.anaconda.org/conda-forge/noarch/setuptools-68.0.0-pyhd8ed1ab_0.conda#5a7739d0f57ee64133c9d32e6507c46d
 https://conda.anaconda.org/conda-forge/noarch/shellingham-1.4.0-pyh44b312d_0.tar.bz2#437655338696f9d0dfdb0a024e66b255
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
 https://conda.anaconda.org/conda-forge/osx-64/tornado-6.3.2-py38hcafd530_0.conda#afefcf665a5049b030efb084a51e3935
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.3-pyha770c72_0.conda#4a3014a4d107d15475d106b751c4e352
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.0-pyha770c72_0.conda#c76ebd4731d3668ba16975a30ef19d0d
 https://conda.anaconda.org/conda-forge/osx-64/unicodedata2-15.0.0-py38hef030d1_0.tar.bz2#51020c740c53f14657f6307b9eb23f85
 https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
 https://conda.anaconda.org/conda-forge/osx-64/curl-8.1.2-hbee3ae8_0.conda#6cc301a6c2ba26e29949818efdc133ca
 https://conda.anaconda.org/eradiate/noarch/dessinemoi-23.1.0-py_0.tar.bz2#490780e63e113a7dc444bd068e049bfe
 https://conda.anaconda.org/conda-forge/noarch/environ-config-22.1.0-pyhd8ed1ab_0.tar.bz2#a1103faffa0a877313c1fba776aa0fc0
 https://conda.anaconda.org/conda-forge/osx-64/fonttools-4.40.0-py38hcafd530_0.conda#b26b38c5f75e03e86cecf860ca9fb1cd
-https://conda.anaconda.org/conda-forge/osx-64/hdf5-1.14.0-nompi_hbf0aa07_103.conda#90f50d124606a4e62628823b614a2f4c
+https://conda.anaconda.org/conda-forge/osx-64/hdf5-1.14.1-nompi_hedada53_100.conda#033c310c83abbd9c2f9a5c13b9f54225
 https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
 https://conda.anaconda.org/conda-forge/osx-64/libblas-3.9.0-17_osx64_openblas.conda#65299527582e2449b05d27fcf8352125
 https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-3.0.0-pyhd8ed1ab_0.conda#93a8e71256479c62074356ef6ebf501b
-https://conda.anaconda.org/conda-forge/osx-64/pillow-9.5.0-py38h16710f9_1.conda#c5bf174a033ef668679cc80918422515
+https://conda.anaconda.org/conda-forge/osx-64/pillow-10.0.0-py38h16710f9_0.conda#8f73f0573ab381d56588e001754c53d3
 https://conda.anaconda.org/eradiate/noarch/pinttrs-23.2.0-py_0.tar.bz2#1aebe9fa813278f719fa8e31d8000452
 https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
 https://conda.anaconda.org/conda-forge/noarch/portion-2.4.0-pyhd8ed1ab_0.conda#9d34bac22e169b41f4e34525a140c13b
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
 https://conda.anaconda.org/conda-forge/osx-64/ruamel.yaml-0.17.32-py38hcafd530_0.conda#cb301e0b2b162330bc3b03fe51ea0d15
 https://conda.anaconda.org/conda-forge/noarch/tqdm-4.65.0-pyhd8ed1ab_1.conda#ed792aff3acb977d09c7013358097f83
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.3-hd8ed1ab_0.conda#3876f650ed7d0f95d70fa4b647621909
-https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.3-pyhd8ed1ab_0.conda#ae465d0fbf9f1979cb2d8d4043d885e2
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.0-hd8ed1ab_0.conda#37761dccc7ca8eaa08c60c4f62eb2dcc
+https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.3-pyhd8ed1ab_1.conda#89efeecbb24c62e2f1ed0b8ca959ec69
 https://conda.anaconda.org/conda-forge/noarch/importlib-resources-5.12.0-pyhd8ed1ab_0.conda#3544c818f0720c89eb16ae6940ab440b
 https://conda.anaconda.org/conda-forge/osx-64/libcblas-3.9.0-17_osx64_openblas.conda#380151ca00704172b242a63701b7bf8a
 https://conda.anaconda.org/conda-forge/osx-64/liblapack-3.9.0-17_osx64_openblas.conda#6ab83532872bf3659613638589dd10af
-https://conda.anaconda.org/conda-forge/osx-64/libnetcdf-4.9.2-nompi_hf077d52_105.conda#64d626e024a284777458e2b315e9eb56
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.6.0-pyhd8ed1ab_0.conda#741384b21c1b512617f4ee4ea8457c5d
+https://conda.anaconda.org/conda-forge/osx-64/libnetcdf-4.9.2-nompi_hfeda9e8_106.conda#66108519efbf30b02632ad35f519773f
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.8.0-pyhd8ed1ab_0.conda#3e4aca765371893ad848397794600632
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/noarch/rich-13.4.2-pyhd8ed1ab_0.conda#f993baacc175e83fafd6b846e9c4c8a2
-https://conda.anaconda.org/conda-forge/osx-64/numpy-1.24.3-py38h9a4a08f_0.conda#5ff64b8133dea66865fe1bd35fb1d6d6
+https://conda.anaconda.org/conda-forge/osx-64/numpy-1.24.4-py38h9a4a08f_0.conda#85debc55a30068d6bb76a6deaf599afa
 https://conda.anaconda.org/conda-forge/noarch/pooch-1.7.0-pyha770c72_3.conda#5936894aade8240c867d292aa0d980c6
 https://conda.anaconda.org/conda-forge/noarch/typer-0.9.0-pyhd8ed1ab_0.conda#5030a13b2fe5e143d5956d4943d3018f
 https://conda.anaconda.org/conda-forge/osx-64/cftime-1.6.2-py38hbd87e4b_1.tar.bz2#6b61efa56393b9655334192cc5423659
 https://conda.anaconda.org/conda-forge/osx-64/contourpy-1.1.0-py38h15a1a5b_0.conda#30d645ffb3572a3875e6fc8687857182
 https://conda.anaconda.org/conda-forge/osx-64/pandas-1.5.3-py38hec72209_1.conda#a8f001ab0a7c6312cea020bd20689765
 https://conda.anaconda.org/conda-forge/osx-64/scipy-1.10.1-py38h9cf86d3_3.conda#5e20c77455e815704b008ab8f42f6169
 https://conda.anaconda.org/conda-forge/osx-64/matplotlib-base-3.7.1-py38hcb346ec_0.conda#1f1eea98c232c8ef720175e12b00d0c4
-https://conda.anaconda.org/conda-forge/osx-64/netcdf4-1.6.4-nompi_py38h47ac6a0_100.conda#f86d4df9f8f46ae6d0c29bb87fe093b0
+https://conda.anaconda.org/conda-forge/osx-64/netcdf4-1.6.4-nompi_py38ha129777_101.conda#0e0f917d6168b9744a407d5ef3c2cb09
 https://conda.anaconda.org/conda-forge/noarch/xarray-2023.1.0-pyhd8ed1ab_0.conda#c11eb03b6f77a0d22ae88c454c940f55
 https://conda.anaconda.org/conda-forge/osx-64/matplotlib-3.7.1-py38h50d1736_0.conda#14bce132d8a4546246b131c4289b480f
```

### Comparing `eradiate-0.23.2rc3/requirements/conda/environment-dev-linux-64.lock` & `eradiate-0.23.2rc4/requirements/conda/environment-dev-linux-64.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Generated by conda-lock.
 # platform: linux-64
-# input_hash: 9dcecc3b104941efb0fda739f479016fbf6654d5f0596f31fc7e8f13170c7d08
+# input_hash: 663e5d9eaad318a79c7cbf185aa33c7e6c2fba5cd7511d678b1e7304b2233d11
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2#d7c89558ba9fa0495403155b64376d81
 https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2023.5.7-hbcca054_0.conda#f5c65075fc34438d5b456c7f3f5ab695
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-dejavu-sans-mono-2.37-hab24e00_0.tar.bz2#0c96522c6bdaed4b1566d11387caaf45
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-inconsolata-3.000-h77eed37_0.tar.bz2#34893075a5c9e55cdafac56607368fc6
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-source-code-pro-2.038-h77eed37_0.tar.bz2#4d59c254e01d9cde7957100457e2d5fb
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-ubuntu-0.83-hab24e00_0.tar.bz2#19410c3df09dfb12d1206132a1d357c5
@@ -26,28 +26,28 @@
 https://conda.anaconda.org/conda-forge/linux-64/gmp-6.2.1-h58526e2_0.tar.bz2#b94cf2db16066b242ebd26db2facbd56
 https://conda.anaconda.org/conda-forge/linux-64/graphite2-1.3.13-h58526e2_1001.tar.bz2#8c54672728e8ec6aa6db90cf2806d220
 https://conda.anaconda.org/conda-forge/linux-64/icu-72.1-hcb278e6_0.conda#7c8d20d847bb45f56bd941578fcfa146
 https://conda.anaconda.org/conda-forge/linux-64/keyutils-1.6.1-h166bdaf_0.tar.bz2#30186d27e2c9fa62b45fb1476b7200e3
 https://conda.anaconda.org/conda-forge/linux-64/lame-3.100-h166bdaf_1003.tar.bz2#a8832b479f93521a9e7b5b743803be51
 https://conda.anaconda.org/conda-forge/linux-64/lerc-4.0.0-h27087fc_0.tar.bz2#76bbff344f0134279f225174e9064c8f
 https://conda.anaconda.org/conda-forge/linux-64/libaec-1.0.6-hcb278e6_1.conda#0f683578378cddb223e7fd24f785ab2a
-https://conda.anaconda.org/conda-forge/linux-64/libbrotlicommon-1.0.9-h166bdaf_8.tar.bz2#9194c9bf9428035a05352d031462eae4
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlicommon-1.0.9-h166bdaf_9.conda#61641e239f96eae2b8492dc7e755828c
 https://conda.anaconda.org/conda-forge/linux-64/libdeflate-1.18-h0b41bf4_0.conda#6aa9c9de5542ecb07fdda9ca626252d8
 https://conda.anaconda.org/conda-forge/linux-64/libev-4.33-h516909a_1.tar.bz2#6f8720dff19e17ce5d48cfe7f3d2f0a3
 https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.5.0-hcb278e6_1.conda#6305a3dd2752c76335295da4e581f2fd
 https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2#d645c6d2ac96843a2bfaccd2d62b3ac3
 https://conda.anaconda.org/conda-forge/linux-64/libiconv-1.17-h166bdaf_0.tar.bz2#b62b52da46c39ee2bc3c162ac7f1804d
 https://conda.anaconda.org/conda-forge/linux-64/libjpeg-turbo-2.1.5.1-h0b41bf4_0.conda#1edd9e67bdb90d78cea97733ff6b54e6
 https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.0-h7f98852_0.tar.bz2#39b1328babf85c7c3a61636d9cd50206
-https://conda.anaconda.org/conda-forge/linux-64/libogg-1.3.4-h7f98852_1.tar.bz2#6e8cc2173440d77708196c5b93771680
+https://repo.anaconda.com/pkgs/main/linux-64/libogg-1.3.5-h27cfd23_1.conda#710ee7fdb0ddf7591a5af7ca7eb4d73d
 https://conda.anaconda.org/conda-forge/linux-64/libopenblas-0.3.23-pthreads_h80387f5_0.conda#9c5ea51ccb8ffae7d06c645869d24ce6
 https://conda.anaconda.org/conda-forge/linux-64/libopus-1.3.1-h7f98852_1.tar.bz2#15345e56d527b330e1cacbdf58676e8f
 https://conda.anaconda.org/conda-forge/linux-64/libsodium-1.0.18-h36c2ea0_1.tar.bz2#c3788462a6fbddafdb413a9f9053e58d
 https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda#40b61aab5c7ba9ff276c41cfffe6b80b
-https://conda.anaconda.org/conda-forge/linux-64/libwebp-base-1.3.0-h0b41bf4_0.conda#0d4a7508d8c6c65314f2b9c1f56ad408
+https://conda.anaconda.org/conda-forge/linux-64/libwebp-base-1.3.1-hd590300_0.conda#82bf6f63eb15ef719b556b63feec3a77
 https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-hd590300_5.conda#f36c115f1ee199da648e0597ec2047ad
 https://conda.anaconda.org/conda-forge/linux-64/lz4-c-1.9.4-hcb278e6_0.conda#318b08df404f9c9be5712aaa5a6f0bb0
 https://conda.anaconda.org/conda-forge/linux-64/mpg123-1.31.3-hcb278e6_0.conda#141a126675b6d1a4eabb111a4a353898
 https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.4-hcb278e6_0.conda#681105bccc2a3f7f1a837d47d39c9179
 https://conda.anaconda.org/conda-forge/linux-64/nspr-4.35-h27087fc_0.conda#da0ec11a6454ae19bff5b02ed881a2b1
 https://conda.anaconda.org/conda-forge/linux-64/openssl-3.1.1-hd590300_1.conda#2e1d7b458ac8f1e3ca4e18b77add6277
 https://conda.anaconda.org/conda-forge/linux-64/pixman-0.40.0-h36c2ea0_0.tar.bz2#660e72c82f2e75a6b3fe6a6e75c79f19
@@ -62,65 +62,65 @@
 https://conda.anaconda.org/conda-forge/linux-64/xorg-xf86vidmodeproto-2.3.1-h7f98852_1002.tar.bz2#3ceea9668625c18f19530de98b15d5b0
 https://conda.anaconda.org/conda-forge/linux-64/xorg-xproto-7.0.31-h7f98852_1007.tar.bz2#b4a4381d54784606820704f7b5f05a15
 https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2#2161070d867d1b1204ea749c8eec4ef0
 https://conda.anaconda.org/conda-forge/linux-64/yaml-0.2.5-h7f98852_2.tar.bz2#4cb3ad778ec2d5a7acbdf254eb1c42ae
 https://conda.anaconda.org/conda-forge/linux-64/expat-2.5.0-hcb278e6_1.conda#8b9b5aca60558d02ddaa09d599e55920
 https://conda.anaconda.org/conda-forge/linux-64/hdf4-4.2.15-h501b40f_6.conda#c3e9338e15d90106f467377017352b97
 https://conda.anaconda.org/conda-forge/linux-64/libblas-3.9.0-17_linux64_openblas.conda#57fb44770b1bc832fb2dbefa1bd502de
-https://conda.anaconda.org/conda-forge/linux-64/libbrotlidec-1.0.9-h166bdaf_8.tar.bz2#4ae4d7795d33e02bd20f6b23d91caf82
-https://conda.anaconda.org/conda-forge/linux-64/libbrotlienc-1.0.9-h166bdaf_8.tar.bz2#04bac51ba35ea023dc48af73c1c88c25
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlidec-1.0.9-h166bdaf_9.conda#081aa22f4581c08e4372b0b6c2f8478e
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlienc-1.0.9-h166bdaf_9.conda#1f0a03af852a9659ed2bf08f2f1704fd
 https://conda.anaconda.org/conda-forge/linux-64/libcap-2.67-he9d0100_0.conda#d05556c80caffff164d17bdea0105a1a
 https://conda.anaconda.org/conda-forge/linux-64/libedit-3.1.20191231-he28a2e2_2.tar.bz2#4d331e44109e3f0e19b4cb8f9b82f3e1
 https://conda.anaconda.org/conda-forge/linux-64/libevent-2.1.12-hf998b51_1.conda#a1cfcc585f0c42bf8d5546bb1dfb668d
-https://conda.anaconda.org/conda-forge/linux-64/libflac-1.4.2-h27087fc_0.tar.bz2#7daf72d8e2a8e848e11d63ed6d1026e0
+https://conda.anaconda.org/conda-forge/linux-64/libflac-1.4.3-h59595ed_0.conda#ee48bf17cc83a00f59ca1494d5646869
 https://conda.anaconda.org/conda-forge/linux-64/libgpg-error-1.47-h71f35ed_0.conda#c2097d0b46367996f09b4e8e4920384a
 https://conda.anaconda.org/conda-forge/linux-64/libnghttp2-1.52.0-h61bc06f_0.conda#613955a50485812985c059e7b269f42e
 https://conda.anaconda.org/conda-forge/linux-64/libpng-1.6.39-h753d276_0.conda#e1c890aebdebbfbf87e2c917187b4416
 https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.42.0-h2797004_0.conda#fdaae20a1cf7cd62130a0973190a31b7
 https://conda.anaconda.org/conda-forge/linux-64/libssh2-1.11.0-h0841786_0.conda#1f5a58e686b13bcfde88b93f547d23fe
 https://conda.anaconda.org/conda-forge/linux-64/libvorbis-1.3.7-h9c3ff4c_0.tar.bz2#309dec04b70a3cc0f1e84a4013683bc0
 https://conda.anaconda.org/conda-forge/linux-64/libxcb-1.15-h0b41bf4_0.conda#33277193f5b92bad9fdd230eb700929c
 https://conda.anaconda.org/conda-forge/linux-64/libxml2-2.11.4-h0d562d8_0.conda#e46fad17d5fb57316b956f88dca765e4
 https://conda.anaconda.org/conda-forge/linux-64/libzip-1.9.2-hc929e4a_1.tar.bz2#5b122b50e738c4be5c3f2899f010d7cf
-https://conda.anaconda.org/conda-forge/linux-64/mysql-common-8.0.33-hf1915f5_0.conda#aa8b86066614c4573f6db62c91978fa9
+https://conda.anaconda.org/conda-forge/linux-64/mysql-common-8.0.33-hf1915f5_1.conda#b241363e3b72bae6dfbd31e9fecf7d26
 https://conda.anaconda.org/conda-forge/linux-64/pcre2-10.40-hc3806b6_0.tar.bz2#69e2c796349cd9b273890bee0febfe1b
 https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda#47d31b792659ce70f470b5c82fdfb7a4
 https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.12-h27826a3_0.tar.bz2#5b8c42eb62e9fc961af70bdd6a26e168
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libsm-1.2.4-h7391055_0.conda#93ee23f12bc2e684548181256edd2cf6
 https://conda.anaconda.org/conda-forge/linux-64/zeromq-4.3.4-h9c3ff4c_1.tar.bz2#21743a8d2ea0c8cfbbf8fe489b0347df
 https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.13-hd590300_5.conda#68c34ec6149623be41a1933ab996a209
 https://conda.anaconda.org/conda-forge/linux-64/zstd-1.5.2-h3eb15da_6.conda#6b63daed8feeca47be78f323e793d555
 https://conda.anaconda.org/conda-forge/linux-64/blosc-1.21.4-h0f2a231_0.conda#876286b5941933a0f558777e57d883cc
-https://conda.anaconda.org/conda-forge/linux-64/brotli-bin-1.0.9-h166bdaf_8.tar.bz2#e5613f2bc717e9945840ff474419b8e4
+https://conda.anaconda.org/conda-forge/linux-64/brotli-bin-1.0.9-h166bdaf_9.conda#d47dee1856d9cb955b8076eeff304a5b
 https://conda.anaconda.org/conda-forge/linux-64/freetype-2.12.1-hca18f0e_1.conda#e1232042de76d24539a436d37597eb06
 https://conda.anaconda.org/conda-forge/linux-64/krb5-1.20.1-h81ceb04_0.conda#89a41adce7106749573d883b2f657d78
 https://conda.anaconda.org/conda-forge/linux-64/libcblas-3.9.0-17_linux64_openblas.conda#7ef0969b00fe3d6eef56a8151d3afb29
 https://conda.anaconda.org/conda-forge/linux-64/libgcrypt-1.10.1-h166bdaf_0.tar.bz2#f967fc95089cd247ceed56eda31de3a9
 https://conda.anaconda.org/conda-forge/linux-64/libglib-2.76.3-hebfc3b9_0.conda#a64f11b244b2c112cd3fa1cbe9493999
 https://conda.anaconda.org/conda-forge/linux-64/liblapack-3.9.0-17_linux64_openblas.conda#a2103882c46492e26500fcb56c03de8b
 https://conda.anaconda.org/conda-forge/linux-64/libllvm16-16.0.6-h5cf9203_0.conda#753e078cccad40fe4b396bdcf27a3c15
 https://conda.anaconda.org/conda-forge/linux-64/libsndfile-1.2.0-hb75c966_0.conda#c648d19cd9c8625898d5d370414de7c7
 https://conda.anaconda.org/conda-forge/linux-64/libtiff-4.5.1-h8b53f26_0.conda#8ad377fb60abab446a9f02c62b3c2190
-https://conda.anaconda.org/conda-forge/linux-64/mysql-libs-8.0.33-hca2cd23_0.conda#276339b0115d92c6e0793dcdc7afe308
+https://conda.anaconda.org/conda-forge/linux-64/mysql-libs-8.0.33-hca2cd23_1.conda#a04ac37f0659929f3ba0f33c7f3d750f
 https://conda.anaconda.org/conda-forge/linux-64/nss-3.89-he45b914_0.conda#2745719a58eeaab6657256a3f142f099
 https://conda.anaconda.org/conda-forge/linux-64/pandoc-3.1.3-h32600fe_0.conda#8287aeb8462e2d4b235eff788e75919d
 https://conda.anaconda.org/conda-forge/linux-64/python-3.8.17-he550d4f_0_cpython.conda#72d038de0a228e4f0ef4011940641293
 https://conda.anaconda.org/conda-forge/linux-64/xcb-util-0.4.0-hd590300_1.conda#9bfac7ccd94d54fd21a0501296d60424
 https://conda.anaconda.org/conda-forge/linux-64/xcb-util-keysyms-0.4.0-h8ee46fc_1.conda#632413adcd8bc16b515cab87a2932913
 https://conda.anaconda.org/conda-forge/linux-64/xcb-util-renderutil-0.3.9-hd590300_1.conda#e995b155d938b6779da6ace6c6b13816
 https://conda.anaconda.org/conda-forge/linux-64/xcb-util-wm-0.4.1-h8ee46fc_1.conda#90108a432fb5c6150ccfee3f03388656
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libx11-1.8.6-h8ee46fc_0.conda#7590b76c3d11d21caa44f3fc38ac584a
 https://conda.anaconda.org/eradiate/noarch/aabbtree-2.8.0-py_0.tar.bz2#647bcce5f0af4974e507591d5420486b
-https://conda.anaconda.org/conda-forge/noarch/aenum-3.1.12-pyhd8ed1ab_0.conda#602716538da00b2ca3cc85c4d35c0245
+https://conda.anaconda.org/conda-forge/noarch/aenum-3.1.15-pyhd8ed1ab_0.conda#24cff7ab050ebb8a16bdeb02e8ed6f63
 https://conda.anaconda.org/conda-forge/noarch/alabaster-0.7.13-pyhd8ed1ab_0.conda#06006184e203b61d3525f90de394471e
 https://conda.anaconda.org/conda-forge/noarch/appdirs-1.4.4-pyh9f0ad1d_0.tar.bz2#5f095bc6454094e96f146491fd03633b
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
-https://conda.anaconda.org/conda-forge/linux-64/brotli-1.0.9-h166bdaf_8.tar.bz2#2ff08978892a3e8b954397c461f18418
+https://conda.anaconda.org/conda-forge/linux-64/brotli-1.0.9-h166bdaf_9.conda#4601544b4982ba1861fa9b9c607b2c06
 https://conda.anaconda.org/conda-forge/noarch/cachy-0.3.0-pyhd8ed1ab_1.tar.bz2#5dfee17f24e2dfd18d7392b48c9351e2
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
 https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-unix_pyhd8ed1ab_2.tar.bz2#20e4087407c7cb04a40817114b333dbf
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/noarch/crashtest-0.4.1-pyhd8ed1ab_0.tar.bz2#709a2295dd907bb34afb57d54320642f
 https://conda.anaconda.org/conda-forge/noarch/cycler-0.11.0-pyhd8ed1ab_0.tar.bz2#a50559fad0affdbb33729a68669ca1cb
@@ -138,15 +138,15 @@
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
 https://conda.anaconda.org/conda-forge/linux-64/fontconfig-2.14.2-h14ed4e7_0.conda#0f69b688f52ff6da70bccb7ff7001d1d
 https://conda.anaconda.org/conda-forge/linux-64/glib-tools-2.76.3-hfc55251_0.conda#8951eedf3cdf94dd733c1b5eee1f4880
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/imagesize-1.4.1-pyhd8ed1ab_0.tar.bz2#7de5386c8fea29e76b303f37dde4c352
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda#f800d2da156d08e289b14e87e43c1ae5
 https://conda.anaconda.org/conda-forge/noarch/jeepney-0.8.0-pyhd8ed1ab_0.tar.bz2#9800ad1699b42612478755a2d26c722d
-https://conda.anaconda.org/conda-forge/noarch/json5-0.9.5-pyh9f0ad1d_0.tar.bz2#10759827a94e6b14996e81fb002c0bda
+https://conda.anaconda.org/conda-forge/noarch/json5-0.9.14-pyhd8ed1ab_0.conda#dac1dabba2b5a9d1aee175c5fcc7b436
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.7-pyhd8ed1ab_1.conda#0c0a54e16b764bafcae35913cc9d60ff
 https://conda.anaconda.org/conda-forge/linux-64/kiwisolver-1.4.4-py38h43d8883_1.tar.bz2#41ca56d5cac7bfc7eb4fcdbee878eb84
 https://conda.anaconda.org/conda-forge/noarch/lazy_loader-0.2-pyhd8ed1ab_0.conda#d060d017720c9882c4eca0544a4a0592
 https://conda.anaconda.org/conda-forge/linux-64/lcms2-2.15-haa2dc70_1.conda#980d8aca0bc23ca73fa8caa3e7c84c28
 https://conda.anaconda.org/conda-forge/linux-64/libclang13-16.0.6-default_h4d60ac6_0.conda#b10174a063ec195f8fe1b278282c3149
 https://conda.anaconda.org/conda-forge/linux-64/libcups-2.3.3-h36d4200_3.conda#c9f4416a34bc91e0eb029f912c68f81f
 https://conda.anaconda.org/conda-forge/linux-64/libcurl-8.1.2-h409715c_0.conda#50c873c9660ed116707ae15b663928d8
@@ -157,25 +157,25 @@
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.0-pyhd8ed1ab_0.tar.bz2#f8dab71fdc13b1bf29a01248b156d268
 https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.0-pyhd8ed1ab_0.conda#c7d0ea64c37752ecbe6da458aee662d2
 https://conda.anaconda.org/conda-forge/noarch/more-itertools-9.1.0-pyhd8ed1ab_0.conda#1698a717f83cfecf644a877c174c84bd
 https://conda.anaconda.org/conda-forge/linux-64/msgpack-python-1.0.5-py38hfbd4bf9_0.conda#5401b83c1007f408d0c74e23fa9b5eff
 https://conda.anaconda.org/conda-forge/noarch/munkres-1.1.4-pyh9f0ad1d_0.tar.bz2#2ba8498c1018c1e9c61eb99b973dfe19
 https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.5.6-pyhd8ed1ab_0.tar.bz2#7b868f21adde0d9b8b38f9c16836589b
 https://conda.anaconda.org/conda-forge/noarch/networkx-3.1-pyhd8ed1ab_0.conda#254f787d5068bc89f578bf63893ce8b4
-https://conda.anaconda.org/conda-forge/linux-64/numpy-1.24.3-py38h59b608b_0.conda#5836e4ab0399136ede58446a4776b2ff
+https://conda.anaconda.org/conda-forge/linux-64/numpy-1.24.4-py38h59b608b_0.conda#8c3e050afeeb2b32575bdb8955cc67b2
 https://conda.anaconda.org/conda-forge/linux-64/openjpeg-2.5.0-hfec8fc6_2.conda#5ce6a42505c6e9e6151c54c3ec8d68ea
 https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/parso-0.8.3-pyhd8ed1ab_0.tar.bz2#17a565a0c3899244e938cdf417e7b094
 https://conda.anaconda.org/conda-forge/noarch/pastel-0.2.1-pyhd8ed1ab_0.tar.bz2#a4eea5bff523f26442405bc5d1f52adb
 https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
 https://conda.anaconda.org/conda-forge/noarch/pint-0.21-pyhd8ed1ab_0.conda#8d7b829e37d78447569c180f9d827005
 https://conda.anaconda.org/conda-forge/noarch/pkginfo-1.9.6-pyhd8ed1ab_0.conda#be1e9f1c65a1ed0f2ae9352fec99db64
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2#89e3c7cdde7d3aaa2aee933b604dd07f
-https://conda.anaconda.org/conda-forge/noarch/pluggy-1.0.0-pyhd8ed1ab_5.tar.bz2#7d301a0d25f424d96175f810935f0da9
+https://conda.anaconda.org/conda-forge/noarch/pluggy-1.2.0-pyhd8ed1ab_0.conda#7263924c642d22e311d9e59b839f1b33
 https://conda.anaconda.org/conda-forge/noarch/ply-3.11-py_1.tar.bz2#7205635cd71531943440fbfe3b6b5727
 https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.0-pyhd8ed1ab_0.conda#95c5be3c7cbd872509d16c216617fdab
 https://conda.anaconda.org/conda-forge/linux-64/psutil-5.9.5-py38h1de0b5d_0.conda#92e899e7b0ed27c793014d1fa54f9b7b
 https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2#359eeb6536da0e687af562ed265ec263
 https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2#6784285c7e55cb7212efabc79e4c2883
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
@@ -187,15 +187,15 @@
 https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.7-pyhd8ed1ab_0.conda#a61bf9ec79426938ff785eb69dbb1960
 https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
 https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0-py38h0a891b7_5.tar.bz2#0856c59f9ddb710c640dc0428d66b1b7
 https://conda.anaconda.org/conda-forge/linux-64/pyzmq-25.1.0-py38h509eb50_0.conda#33872b6650886eba869408b76c96994c
 https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2#912a71cc01012ee38e6b90ddd561e36f
 https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml.clib-0.2.7-py38h1de0b5d_1.conda#9afa2fc3c51cc4e7d1589c38e4e00d5c
 https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyh41d4057_0.conda#ada5a17adcd10be4fc7e37e4166ba0e2
-https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda#3b68bc43ec6baa48f7354a446267eefe
+https://conda.anaconda.org/conda-forge/noarch/setuptools-68.0.0-pyhd8ed1ab_0.conda#5a7739d0f57ee64133c9d32e6507c46d
 https://conda.anaconda.org/conda-forge/noarch/shellingham-1.4.0-pyh44b312d_0.tar.bz2#437655338696f9d0dfdb0a024e66b255
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/smmap-3.0.5-pyh44b312d_0.tar.bz2#3a8dc70789709aa315325d5df06fb7e4
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
 https://conda.anaconda.org/conda-forge/noarch/snowballstemmer-2.2.0-pyhd8ed1ab_0.tar.bz2#4d22a9315e78c6827f806065957d566e
 https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
@@ -207,32 +207,32 @@
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-serializinghtml-1.1.5-pyhd8ed1ab_2.tar.bz2#9ff55a0901cf952f05c654394de76bf7
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.11.8-pyha770c72_0.conda#75838e8556166263a82038b51d01d5f1
 https://conda.anaconda.org/conda-forge/noarch/toolz-0.12.0-pyhd8ed1ab_0.tar.bz2#92facfec94bc02d6ccf42e7173831a36
 https://conda.anaconda.org/conda-forge/linux-64/tornado-6.3.2-py38h01eb140_0.conda#3db869202b0e523d606d13e81ca79ab6
 https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.3-pyha770c72_0.conda#4a3014a4d107d15475d106b751c4e352
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.0-pyha770c72_0.conda#c76ebd4731d3668ba16975a30ef19d0d
 https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/linux-64/unicodedata2-15.0.0-py38h0a891b7_0.tar.bz2#44421904760e9f5ae2035193e04360f0
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
-https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.0-pyhd8ed1ab_0.conda#1dd6387a73d84e16b6f73de676bb4c36
+https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda#c34d9325a609381a0b0e8a5b4f325147
 https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
 https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.7-pyhd8ed1ab_0.conda#bcc54b91a8ce88f60f538b87b409909e
 https://conda.anaconda.org/conda-forge/linux-64/xcb-util-image-0.4.0-h8ee46fc_1.conda#9d7bcddf49cbf727730af10e71022c73
 https://conda.anaconda.org/conda-forge/linux-64/xkeyboard-config-2.39-hd590300_0.conda#d88c7fc8a11858fb14761832e4da1954
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxext-1.3.4-h0b41bf4_2.conda#82b6df12252e6f32402b96dacc656fec
-https://conda.anaconda.org/conda-forge/linux-64/xorg-libxrender-0.9.10-h7f98852_1003.tar.bz2#f59c1242cc1dd93e72c2ee2b360979eb
+https://conda.anaconda.org/conda-forge/linux-64/xorg-libxrender-0.9.11-hd590300_0.conda#ed67c36f215b310412b2af935bf3e530
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
 https://conda.anaconda.org/conda-forge/noarch/accessible-pygments-0.0.4-pyhd8ed1ab_0.conda#46a2e6e3dfa718ce3492018d5a110dd6
 https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.0-pyhd8ed1ab_1.conda#2b35a85d654a47aac8f34c1bb6de7142
 https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
 https://conda.anaconda.org/conda-forge/noarch/async-lru-2.0.2-pyhd8ed1ab_0.conda#41221f97a0c82e5a60b21716a3d7469c
 https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
-https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.4-pyhd8ed1ab_0.tar.bz2#c5b3edc62d6309088f4970b3eaaa65a6
+https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda#6b1b907661838a75d067a22f87996b2e
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
 https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda#d48b143d01385872a88ef8417e96c30e
 https://conda.anaconda.org/conda-forge/linux-64/cairo-1.16.0-hbbf8b49_1016.conda#c1dd96500b9b1a75e9e511931f415cbc
 https://conda.anaconda.org/conda-forge/linux-64/cffi-1.15.1-py38h4a40e3a_3.conda#3ac112151c6b6cfe457e976de41af0c5
 https://conda.anaconda.org/conda-forge/linux-64/cftime-1.6.2-py38h26c90d9_1.tar.bz2#dcc025a7bb54374979c500c2e161fac9
 https://conda.anaconda.org/conda-forge/noarch/click-default-group-1.2.2-pyhd8ed1ab_1.tar.bz2#72a46ffc25701c173932fd55cf0965d3
 https://conda.anaconda.org/conda-forge/noarch/clikit-0.6.2-pyhd8ed1ab_2.conda#02abb7b66b02e8b9f5a9b05454400087
@@ -240,15 +240,15 @@
 https://conda.anaconda.org/conda-forge/linux-64/contourpy-1.1.0-py38h7f3f72f_0.conda#0fdf3cc879156e0234e05962d55b6502
 https://conda.anaconda.org/conda-forge/linux-64/curl-8.1.2-h409715c_0.conda#9f88cfb15b7d08b25880b138f91e0eb4
 https://conda.anaconda.org/eradiate/noarch/dessinemoi-23.1.0-py_0.tar.bz2#490780e63e113a7dc444bd068e049bfe
 https://conda.anaconda.org/conda-forge/noarch/environ-config-22.1.0-pyhd8ed1ab_0.tar.bz2#a1103faffa0a877313c1fba776aa0fc0
 https://conda.anaconda.org/conda-forge/linux-64/fonttools-4.40.0-py38h01eb140_0.conda#f893b6bac56c477dd71498569b4a9022
 https://conda.anaconda.org/conda-forge/noarch/gitdb-4.0.10-pyhd8ed1ab_0.conda#3706d2f3d7cb5dae600c833345a76132
 https://conda.anaconda.org/conda-forge/linux-64/glib-2.76.3-hfc55251_0.conda#950e02f5665f5f4ff0437a6acba58798
-https://conda.anaconda.org/conda-forge/linux-64/hdf5-1.14.0-nompi_hb72d44e_103.conda#975973a4350ab45ff1981fe535a12af5
+https://conda.anaconda.org/conda-forge/linux-64/hdf5-1.14.1-nompi_h4f84152_100.conda#ff9ae10aa224826c07da7ef26cb0b717
 https://conda.anaconda.org/conda-forge/noarch/html5lib-1.1-pyh9f0ad1d_0.tar.bz2#b2355343d6315c892543200231d7154a
 https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.7.0-pyha770c72_0.conda#ba3786c6846e46038fe60c785d46dc81
 https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
 https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.2.3-pyhd8ed1ab_0.tar.bz2#31e4a1506968d017229bdb64695013a1
 https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
 https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-4.12.0-py38h578d9bd_0.conda#e7f204764ab3683174c1707240368b84
@@ -257,82 +257,84 @@
 https://conda.anaconda.org/conda-forge/linux-64/libclang-16.0.6-default_h1cdf331_0.conda#e976871e132fe506da52c1240229246a
 https://conda.anaconda.org/conda-forge/linux-64/libxkbcommon-1.5.0-h5d7e998_3.conda#c91ea308d7bf70b62ddda568478aa03b
 https://conda.anaconda.org/conda-forge/noarch/livereload-2.6.3-pyh9f0ad1d_0.tar.bz2#b7190e3ec3eff52839434bf4698e2d62
 https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-2.2.0-pyhd8ed1ab_0.conda#b2928a6c6d52d7e3562b4a59c3214e3a
 https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
 https://conda.anaconda.org/conda-forge/noarch/overrides-7.3.1-pyhd8ed1ab_0.tar.bz2#a5745ced46e69aa9754053ba061974ab
 https://conda.anaconda.org/conda-forge/noarch/pexpect-4.8.0-pyh1a96a4e_2.tar.bz2#330448ce4403cc74990ac07c555942a1
-https://conda.anaconda.org/conda-forge/linux-64/pillow-9.5.0-py38h885162f_1.conda#0eec8a20a17f17ec9e0b6839be466866
+https://conda.anaconda.org/conda-forge/linux-64/pillow-10.0.0-py38h885162f_0.conda#777c54134d5422a867aed7084cf5db5e
 https://conda.anaconda.org/eradiate/noarch/pinttrs-23.2.0-py_0.tar.bz2#1aebe9fa813278f719fa8e31d8000452
 https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
 https://conda.anaconda.org/conda-forge/noarch/portion-2.4.0-pyhd8ed1ab_0.conda#9d34bac22e169b41f4e34525a140c13b
 https://conda.anaconda.org/conda-forge/linux-64/pulseaudio-client-16.1-hb77b528_4.conda#8f349ca16d30950aa00870484d9d30c4
 https://conda.anaconda.org/conda-forge/linux-64/pyerfa-2.0.0.3-py38h7e4f40d_0.conda#631de6b5c8aec9c8ae2dcc596f8d2f72
 https://conda.anaconda.org/conda-forge/noarch/pyproject_hooks-1.0.0-pyhd8ed1ab_0.conda#21de50391d584eb7f4441b9de1ad773f
-https://conda.anaconda.org/conda-forge/noarch/pytest-7.3.2-pyhd8ed1ab_1.conda#f2465696f4396245eca4613f6e924796
+https://conda.anaconda.org/conda-forge/noarch/pytest-7.4.0-pyhd8ed1ab_0.conda#3cfe9b9e958e7238a386933c75d190db
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
 https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
 https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml-0.17.32-py38h01eb140_0.conda#c92cc8efb1341f90ea5f51f576480580
 https://conda.anaconda.org/conda-forge/linux-64/sip-6.7.9-py38h17151c0_0.conda#6a54fd42b71a8b1c5f9c4a691270cdf1
 https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.1-pyh41d4057_0.conda#3788984d535770cad699efaeb6cb3037
 https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
 https://conda.anaconda.org/conda-forge/noarch/tqdm-4.65.0-pyhd8ed1ab_1.conda#ed792aff3acb977d09c7013358097f83
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.3-hd8ed1ab_0.conda#3876f650ed7d0f95d70fa4b647621909
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.0-hd8ed1ab_0.conda#37761dccc7ca8eaa08c60c4f62eb2dcc
+https://conda.anaconda.org/conda-forge/noarch/annotated-types-0.5.0-pyhd8ed1ab_0.conda#578ae086f225bc2380c79f3b551ff2f7
 https://conda.anaconda.org/conda-forge/linux-64/argon2-cffi-bindings-21.2.0-py38h0a891b7_3.tar.bz2#efcaa056d265a3138d2038a4b6b68791
 https://conda.anaconda.org/conda-forge/linux-64/astropy-5.0.6-py38h07e1bb6_0.conda#0fcc655ae90038f1f66db3e3046d6c51
 https://conda.anaconda.org/conda-forge/linux-64/brotlipy-0.7.0-py38h0a891b7_1005.tar.bz2#e99e08812dfff30fdd17b3f8838e2759
 https://conda.anaconda.org/conda-forge/linux-64/cryptography-41.0.1-py38hcdda232_0.conda#8dc6f3a9342a870c3c927927e86aa4ad
 https://conda.anaconda.org/conda-forge/noarch/gitpython-3.1.31-pyhd8ed1ab_0.conda#f6e6b482110246a81c3f03e81c68752d
-https://conda.anaconda.org/conda-forge/linux-64/gstreamer-1.22.3-h977cf35_1.conda#410ed3b168e5a139d12ebaf4143072cd
+https://repo.anaconda.com/pkgs/main/linux-64/gstreamer-1.22.3-h5eee18b_0.conda#c2ffbb79cb2f51b042de223d482b7b29
 https://conda.anaconda.org/conda-forge/linux-64/harfbuzz-7.3.0-hdb3a94d_0.conda#765bc76c0dfaf24ff9d8a2935b2510df
 https://conda.anaconda.org/conda-forge/noarch/importlib-resources-5.12.0-pyhd8ed1ab_0.conda#3544c818f0720c89eb16ae6940ab440b
 https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.7.0-hd8ed1ab_0.conda#27a4cec373ec84d1c1aa02a1e37f8eaf
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.4.4-pyhd8ed1ab_1.conda#7c0965e1d4a0ee1529e8eaa03a78a5b3
-https://conda.anaconda.org/conda-forge/linux-64/libnetcdf-4.9.2-nompi_h0f3d0bb_105.conda#b5d412441b84305460e9df8a016a3392
+https://conda.anaconda.org/conda-forge/linux-64/libnetcdf-4.9.2-nompi_h78c856c_106.conda#47665bf3dec451455474556ecd940ed2
 https://conda.anaconda.org/conda-forge/noarch/mdit-py-plugins-0.4.0-pyhd8ed1ab_0.conda#6c5358a10873a15398b6f15f60cb5e1f
 https://conda.anaconda.org/conda-forge/linux-64/pandas-1.5.3-py38hdc8b05c_1.conda#c944b033a2126e7f714a7ecaecb22011
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.6.0-pyhd8ed1ab_0.conda#741384b21c1b512617f4ee4ea8457c5d
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.8.0-pyhd8ed1ab_0.conda#3e4aca765371893ad848397794600632
 https://conda.anaconda.org/conda-forge/noarch/pybtex-0.24.0-pyhd8ed1ab_2.tar.bz2#2099b86a7399c44c0c61cdb6de6915ba
-https://conda.anaconda.org/conda-forge/linux-64/pydantic-1.10.9-py38h01eb140_0.conda#2d8a27b52507d0ba49c938005465b5e3
+https://conda.anaconda.org/conda-forge/linux-64/pydantic-core-2.0.1-py38h0cc4f7c_0.conda#c4f9a324d600fb26bf8cf25757e382f8
 https://conda.anaconda.org/conda-forge/linux-64/pyqt5-sip-12.11.0-py38h8dc9893_3.conda#7bb0328b4a0f857aeb432426b9a5f908
 https://conda.anaconda.org/conda-forge/noarch/pytest-metadata-3.0.0-pyhd8ed1ab_1.conda#8bdcc0f401561213821bf67513abeeff
 https://conda.anaconda.org/conda-forge/noarch/python-build-0.10.0-pyhd8ed1ab_1.conda#0ab47ce574f6a8bcb9f2076436e7fedb
 https://conda.anaconda.org/conda-forge/noarch/rich-13.4.2-pyhd8ed1ab_0.conda#f993baacc175e83fafd6b846e9c4c8a2
 https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
-https://conda.anaconda.org/conda-forge/linux-64/gst-plugins-base-1.22.3-h938bd60_1.conda#1f317eb7f00db75f4112a07476345376
-https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.2.0-pyhd8ed1ab_0.conda#58ca2d50c3b27b86fd7df62eaadbf9a9
+https://repo.anaconda.com/pkgs/main/linux-64/gst-plugins-base-1.22.3-he621ea3_0.conda#27be67671dce7d6d8c53bf6260090c15
+https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda#1d018ee4ab13217e2544f795eb0a6798
 https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
 https://conda.anaconda.org/conda-forge/linux-64/matplotlib-base-3.7.1-py38hd6c3c57_0.conda#3b8ba76acae09fbd4b2247c4ee4c0324
 https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.0-pyhd8ed1ab_0.conda#f525a01528c3eba1d381a232a6971c6a
-https://conda.anaconda.org/conda-forge/linux-64/netcdf4-1.6.4-nompi_py38hdfa7aa7_100.conda#ce30178fb90d4509c3fda5b572124200
-https://conda.anaconda.org/conda-forge/noarch/pip-tools-6.13.0-pyhd8ed1ab_1.conda#566e41c99730f1124d6948ab8fe1c18d
+https://conda.anaconda.org/conda-forge/linux-64/netcdf4-1.6.4-nompi_py38h383a0a3_101.conda#693cbd2ee4f62c8a2521cfaf7560b647
+https://conda.anaconda.org/conda-forge/noarch/pip-tools-6.14.0-pyhd8ed1ab_0.conda#4c3828f6213d5ddba2f5033d4b422d17
 https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
 https://conda.anaconda.org/conda-forge/linux-64/pybtex-docutils-1.0.2-py38h578d9bd_2.tar.bz2#178c840a19be1a4c809798a73b285d27
+https://conda.anaconda.org/conda-forge/linux-64/pydantic-2.0-py38h01eb140_0.conda#453742dca59531095a6a6aae78665c81
 https://conda.anaconda.org/conda-forge/noarch/pyopenssl-23.2.0-pyhd8ed1ab_1.conda#34f7d568bf59d18e3fef8c405cbece21
 https://conda.anaconda.org/conda-forge/noarch/pytest-json-report-1.5.0-pyhd8ed1ab_0.tar.bz2#837e335fa428cf7c784ee2e80594506c
 https://conda.anaconda.org/conda-forge/linux-64/secretstorage-3.3.3-py38h578d9bd_1.tar.bz2#7ff0f00ee67fcbccbae548be59bfae77
 https://conda.anaconda.org/conda-forge/noarch/typer-0.9.0-pyhd8ed1ab_0.conda#5030a13b2fe5e143d5956d4943d3018f
 https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.23.1-pyhd8ed1ab_0.conda#838b85f656b078bdd882ef97978e7f40
 https://conda.anaconda.org/conda-forge/noarch/xarray-2023.1.0-pyhd8ed1ab_0.conda#c11eb03b6f77a0d22ae88c454c940f55
-https://conda.anaconda.org/conda-forge/linux-64/keyring-23.13.1-py38h578d9bd_0.conda#713b14390d450db02fea6b0c0535d67a
+https://conda.anaconda.org/conda-forge/linux-64/keyring-24.2.0-py38h578d9bd_0.conda#886a052bb649eff357b194d6005052cf
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.8.0-pyhd8ed1ab_0.conda#e78da91cf428faaf05701ce8cc8f2f9b
 https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.38-hd8ed1ab_0.conda#45b74f64d8808eda7e6f6e6b1d641fd2
 https://conda.anaconda.org/conda-forge/linux-64/qt-main-5.15.8-h01ceb2d_12.conda#60fd4bdf187f88bac57cdc1a052f2811
 https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.15-pyhd8ed1ab_0.conda#27db656619a55d727eaf5a6ece3d2fd6
 https://conda.anaconda.org/conda-forge/noarch/ipython-8.12.0-pyh41d4057_0.conda#e89d0c5836e45f9e6a66c5c24fc9ef35
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.6.0-pyhd8ed1ab_0.conda#879782bde4bbdb4c7b5d4054504a20d5
 https://conda.anaconda.org/conda-forge/linux-64/pyqt-5.15.7-py38ha0d8c90_3.conda#e965dc172d67920d058ac2b3a0e27565
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/noarch/cachecontrol-0.13.0-pyhd8ed1ab_0.conda#9f0b2eb5f5dd2cec36d5342a80adfec0
 https://conda.anaconda.org/conda-forge/noarch/ensureconda-1.4.3-pyhd8ed1ab_0.tar.bz2#c99ae3abf501990769047b4b40a98f17
-https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.1-pyh210e3f2_0.conda#4b57b688e22d094d1479a35543c18e93
-https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.6.0-pyhd8ed1ab_0.conda#39fd52b0fcb2fb52bac47a1419bf09bd
+https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.3-pyh71e2992_0.conda#482f0176a89f14e10a7d15f9f1980e36
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.7.0-pyhd8ed1ab_0.conda#7488cd1f4d35a2af96faa765b7e5b2f0
 https://conda.anaconda.org/conda-forge/linux-64/matplotlib-3.7.1-py38h578d9bd_0.conda#50ff9e0a3dd459a0ca365741072bf9a2
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.6.0-pyhd8ed1ab_0.conda#e8172ca42f2869bb90185c9356899e81
 https://conda.anaconda.org/conda-forge/noarch/pooch-1.7.0-pyha770c72_3.conda#5936894aade8240c867d292aa0d980c6
 https://conda.anaconda.org/conda-forge/noarch/sphinx-5.0.0-pyh6c4a22f_1.tar.bz2#a7cc4b9c94548ff9a19b368f975e5404
 https://conda.anaconda.org/conda-forge/noarch/autodocsumm-0.2.11-pyhd8ed1ab_0.conda#547c48372c97c463c93af86d7f2c868c
 https://conda.anaconda.org/conda-forge/noarch/cachecontrol-with-filecache-0.13.0-pyhd8ed1ab_0.conda#3fd3d55ea862cc0736ac1cce6f44c2d1
 https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.6-pyhd8ed1ab_0.conda#68627a08556e4a273e4c7bfc84251457
```

### Comparing `eradiate-0.23.2rc3/requirements/conda/environment-dev-osx-64.lock` & `eradiate-0.23.2rc4/requirements/conda/environment-dev-osx-64.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 # Generated by conda-lock.
 # platform: osx-64
-# input_hash: bf11f624e722c74ec0e342583ae0fcb21524c22ae8ca653349f3b25602fab72a
+# input_hash: 7698d8dd9c55c8170544c99f0bbcc0e151b7ed643f053944f557aef5d422032c
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h0d85af4_4.tar.bz2#37edc4e6304ca87316e160f5ca0bd1b5
 https://conda.anaconda.org/conda-forge/osx-64/c-ares-1.19.1-h0dc2134_0.conda#b3e62631b4e1b9801477523ce1d6f355
 https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2023.5.7-h8857fd0_0.conda#b704e4b79ba0d887c4870b7b09d6a4df
 https://conda.anaconda.org/conda-forge/osx-64/icu-72.1-h7336db1_0.conda#c9689510a50a4bb2ae978421671a125e
-https://conda.anaconda.org/conda-forge/osx-64/libbrotlicommon-1.0.9-hb7f2c08_8.tar.bz2#37157d273eaf3bc7d6862104161d9ec9
+https://conda.anaconda.org/conda-forge/osx-64/libbrotlicommon-1.0.9-hb7f2c08_9.conda#ee1ee8c79c3426229ad03290573be552
 https://conda.anaconda.org/conda-forge/osx-64/libcxx-16.0.6-hd57cbcb_0.conda#7d6972792161077908b62971802f289a
 https://conda.anaconda.org/conda-forge/osx-64/libdeflate-1.18-hac1461d_0.conda#3d131584456b277ce0871e6481fde49b
 https://conda.anaconda.org/conda-forge/osx-64/libev-4.33-haf1e3a3_1.tar.bz2#79dc2be110b2a3d1e97ec21f691c50ad
 https://conda.anaconda.org/conda-forge/osx-64/libffi-3.4.2-h0d85af4_5.tar.bz2#ccb34fb14960ad8b125962d3d79b31a9
 https://conda.anaconda.org/conda-forge/osx-64/libiconv-1.17-hac89ed1_0.tar.bz2#691d103d11180486154af49c037b7ed9
 https://conda.anaconda.org/conda-forge/osx-64/libjpeg-turbo-2.1.5.1-hb7f2c08_0.conda#d7309a152b9b79799063b8bb47e34a3a
 https://conda.anaconda.org/conda-forge/osx-64/libsodium-1.0.18-hbcb3906_1.tar.bz2#24632c09ed931af617fe6d5292919cab
-https://conda.anaconda.org/conda-forge/osx-64/libwebp-base-1.3.0-hb7f2c08_0.conda#18981e4c840126d6118d8952485fea51
+https://conda.anaconda.org/conda-forge/osx-64/libwebp-base-1.3.1-h0dc2134_0.conda#a25a41b5be3fed4b671a58b998dcf89b
 https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-h8a1eda9_5.conda#4a3ad23f6e16f99c04e166767193d700
 https://conda.anaconda.org/conda-forge/osx-64/llvm-openmp-16.0.6-hff08bdf_0.conda#39a5227d906f75102bf8586741690128
 https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.4-hf0c8a7f_0.conda#c3dbae2411164d9b02c69090a9a91857
 https://conda.anaconda.org/conda-forge/osx-64/pthread-stubs-0.4-hc929b4f_1001.tar.bz2#addd19059de62181cd11ae8f4ef26084
 https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.8-3_cp38.conda#ff192f59f7fe23555612030493a079f8
 https://conda.anaconda.org/conda-forge/osx-64/xorg-libxau-1.0.11-h0dc2134_0.conda#9566b4c29274125b0266d0177b5eb97b
 https://conda.anaconda.org/conda-forge/osx-64/xorg-libxdmcp-1.1.3-h35c211d_0.tar.bz2#86ac76d6bf1cbb9621943eb3bd9ae36e
 https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2#a72f9d4ea13d55d745ff1ed594747f10
 https://conda.anaconda.org/conda-forge/osx-64/yaml-0.2.5-h0d85af4_2.tar.bz2#d7e08fcf8259d742156188e8762b4d20
 https://conda.anaconda.org/conda-forge/osx-64/hdf4-4.2.15-h9804679_6.conda#c13d8841112ba7f5931d1d60631394f3
 https://conda.anaconda.org/conda-forge/osx-64/lerc-4.0.0-hb486fe8_0.tar.bz2#f9d6a4c82889d5ecedec1d90eb673c55
 https://conda.anaconda.org/conda-forge/osx-64/libaec-1.0.6-hf0c8a7f_1.conda#7c0f82f435ab4c48d65dc9b28db2ad9e
-https://conda.anaconda.org/conda-forge/osx-64/libbrotlidec-1.0.9-hb7f2c08_8.tar.bz2#7f952a036d9014b4dab96c6ea0f8c2a7
-https://conda.anaconda.org/conda-forge/osx-64/libbrotlienc-1.0.9-hb7f2c08_8.tar.bz2#b36a3bfe866d9127f25f286506982166
+https://conda.anaconda.org/conda-forge/osx-64/libbrotlidec-1.0.9-hb7f2c08_9.conda#4043ef9fe42e178785e0e1853b79bdf9
+https://conda.anaconda.org/conda-forge/osx-64/libbrotlienc-1.0.9-hb7f2c08_9.conda#b64d4dcc70aa141db7fccbf13bad81e1
 https://conda.anaconda.org/conda-forge/osx-64/libedit-3.1.20191231-h0678c8f_2.tar.bz2#6016a8a1d0e63cac3de2c352cd40208b
 https://conda.anaconda.org/conda-forge/osx-64/libgfortran5-12.2.0-he409387_31.conda#5a544130e584b1f204ac896ff071d5b3
 https://conda.anaconda.org/conda-forge/osx-64/libpng-1.6.39-ha978bb4_0.conda#35e4928794c5391aec14ffdf1deaaee5
 https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.42.0-h58db7d2_0.conda#a7d3b44b7b0c9901ac7813b7a0462893
 https://conda.anaconda.org/conda-forge/osx-64/libxcb-1.15-hb7f2c08_0.conda#5513f57e0238c87c12dffedbcc9c1a4a
 https://conda.anaconda.org/conda-forge/osx-64/libxml2-2.11.4-hd95e348_0.conda#681f8dda25e73a830d774a37b9839c85
 https://conda.anaconda.org/conda-forge/osx-64/lz4-c-1.9.4-hf0c8a7f_0.conda#aa04f7143228308662696ac24023f991
@@ -40,32 +40,32 @@
 https://conda.anaconda.org/conda-forge/osx-64/pandoc-3.1.3-h9d075a6_0.conda#e86a3d5c966a09b6129354114483f7a7
 https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda#f17f77f2acf4d344734bda76829ce14e
 https://conda.anaconda.org/conda-forge/osx-64/snappy-1.1.10-h225ccf5_0.conda#4320a8781f14cd959689b86e349f3b73
 https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.12-h5dbffcc_0.tar.bz2#8e9480d9c47061db2ed1b4ecce519a7f
 https://conda.anaconda.org/conda-forge/osx-64/zeromq-4.3.4-he49afe7_1.tar.bz2#1972d732b123ed04b60fd21e94f0b178
 https://conda.anaconda.org/conda-forge/osx-64/zstd-1.5.2-hbc0c0cd_6.conda#40a188783d3c425bdccc9ae9104acbb8
 https://conda.anaconda.org/conda-forge/osx-64/blosc-1.21.4-heccf04b_0.conda#02e92eb72b9ae4c1745b95d03a9c949e
-https://conda.anaconda.org/conda-forge/osx-64/brotli-bin-1.0.9-hb7f2c08_8.tar.bz2#aac5ad0d8f747ef7f871508146df75d9
+https://conda.anaconda.org/conda-forge/osx-64/brotli-bin-1.0.9-hb7f2c08_9.conda#72c526f7ffa265473e6c75fd90605e52
 https://conda.anaconda.org/conda-forge/osx-64/freetype-2.12.1-h3f81eb7_1.conda#852224ea3e8991a8342228eab274840e
 https://conda.anaconda.org/conda-forge/osx-64/krb5-1.20.1-h049b76e_0.conda#db11fa2968ef0837288fe2d7f5b77a50
 https://conda.anaconda.org/conda-forge/osx-64/libgfortran-5.0.0-11_3_0_h97931a8_31.conda#97451338600bd9c5b535eb224ef6c471
 https://conda.anaconda.org/conda-forge/osx-64/libnghttp2-1.52.0-he2ab024_0.conda#12ac7d100bf260263e30a019517f42a2
 https://conda.anaconda.org/conda-forge/osx-64/libssh2-1.11.0-hd019ec5_0.conda#ca3a72efba692c59a90d4b9fc0dfe774
 https://conda.anaconda.org/conda-forge/osx-64/libtiff-4.5.1-hf955e92_0.conda#56523ed556e3a44c0fd55bcf17045892
 https://conda.anaconda.org/conda-forge/osx-64/libzip-1.9.2-h6db710c_1.tar.bz2#ce732d37e479919f3d22b1ccdeb858ac
 https://conda.anaconda.org/conda-forge/osx-64/python-3.8.17-hf9b03c3_0_cpython.conda#f613b663d3829f325b4ffb626bf612b6
 https://conda.anaconda.org/eradiate/noarch/aabbtree-2.8.0-py_0.tar.bz2#647bcce5f0af4974e507591d5420486b
-https://conda.anaconda.org/conda-forge/noarch/aenum-3.1.12-pyhd8ed1ab_0.conda#602716538da00b2ca3cc85c4d35c0245
+https://conda.anaconda.org/conda-forge/noarch/aenum-3.1.15-pyhd8ed1ab_0.conda#24cff7ab050ebb8a16bdeb02e8ed6f63
 https://conda.anaconda.org/conda-forge/noarch/alabaster-0.7.13-pyhd8ed1ab_0.conda#06006184e203b61d3525f90de394471e
 https://conda.anaconda.org/conda-forge/noarch/appdirs-1.4.4-pyh9f0ad1d_0.tar.bz2#5f095bc6454094e96f146491fd03633b
 https://conda.anaconda.org/conda-forge/noarch/appnope-0.1.3-pyhd8ed1ab_0.tar.bz2#54ac328d703bff191256ffa1183126d1
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
-https://conda.anaconda.org/conda-forge/osx-64/brotli-1.0.9-hb7f2c08_8.tar.bz2#55f612fe4a9b5f6ac76348b6de94aaeb
+https://conda.anaconda.org/conda-forge/osx-64/brotli-1.0.9-hb7f2c08_9.conda#53cff90f0cea22e13e5b791f0e5a8e7d
 https://conda.anaconda.org/conda-forge/noarch/cachy-0.3.0-pyhd8ed1ab_1.tar.bz2#5dfee17f24e2dfd18d7392b48c9351e2
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
 https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-unix_pyhd8ed1ab_2.tar.bz2#20e4087407c7cb04a40817114b333dbf
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/noarch/crashtest-0.4.1-pyhd8ed1ab_0.tar.bz2#709a2295dd907bb34afb57d54320642f
 https://conda.anaconda.org/conda-forge/noarch/cycler-0.11.0-pyhd8ed1ab_0.tar.bz2#a50559fad0affdbb33729a68669ca1cb
@@ -79,15 +79,15 @@
 https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
 https://conda.anaconda.org/conda-forge/noarch/executing-1.2.0-pyhd8ed1ab_0.tar.bz2#4c1bc140e2be5c8ba6e3acab99e25c50
 https://conda.anaconda.org/conda-forge/noarch/filelock-3.12.2-pyhd8ed1ab_0.conda#53522ec72e6adae42bd373ef58357230
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/imagesize-1.4.1-pyhd8ed1ab_0.tar.bz2#7de5386c8fea29e76b303f37dde4c352
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda#f800d2da156d08e289b14e87e43c1ae5
-https://conda.anaconda.org/conda-forge/noarch/json5-0.9.5-pyh9f0ad1d_0.tar.bz2#10759827a94e6b14996e81fb002c0bda
+https://conda.anaconda.org/conda-forge/noarch/json5-0.9.14-pyhd8ed1ab_0.conda#dac1dabba2b5a9d1aee175c5fcc7b436
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.7-pyhd8ed1ab_1.conda#0c0a54e16b764bafcae35913cc9d60ff
 https://conda.anaconda.org/conda-forge/osx-64/kiwisolver-1.4.4-py38h98b9b1b_1.tar.bz2#c11eff21a36bc5809b8e23a05ee71df8
 https://conda.anaconda.org/conda-forge/noarch/lazy_loader-0.2-pyhd8ed1ab_0.conda#d060d017720c9882c4eca0544a4a0592
 https://conda.anaconda.org/conda-forge/osx-64/lcms2-2.15-h2dcdeff_1.conda#f1df9b0c2d9fbe985e62f4b24773a9e4
 https://conda.anaconda.org/conda-forge/osx-64/libcurl-8.1.2-hbee3ae8_0.conda#d51e337da844262f9033c9a26452520f
 https://conda.anaconda.org/conda-forge/osx-64/libopenblas-0.3.23-openmp_h429af6e_0.conda#7000a828e29608e4f57e662b5502d2c9
 https://conda.anaconda.org/conda-forge/noarch/lockfile-0.12.2-py_1.tar.bz2#c104d98e09c47519950cffb8dd5b4f10
@@ -104,15 +104,15 @@
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/parso-0.8.3-pyhd8ed1ab_0.tar.bz2#17a565a0c3899244e938cdf417e7b094
 https://conda.anaconda.org/conda-forge/noarch/pastel-0.2.1-pyhd8ed1ab_0.tar.bz2#a4eea5bff523f26442405bc5d1f52adb
 https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
 https://conda.anaconda.org/conda-forge/noarch/pint-0.21-pyhd8ed1ab_0.conda#8d7b829e37d78447569c180f9d827005
 https://conda.anaconda.org/conda-forge/noarch/pkginfo-1.9.6-pyhd8ed1ab_0.conda#be1e9f1c65a1ed0f2ae9352fec99db64
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2#89e3c7cdde7d3aaa2aee933b604dd07f
-https://conda.anaconda.org/conda-forge/noarch/pluggy-1.0.0-pyhd8ed1ab_5.tar.bz2#7d301a0d25f424d96175f810935f0da9
+https://conda.anaconda.org/conda-forge/noarch/pluggy-1.2.0-pyhd8ed1ab_0.conda#7263924c642d22e311d9e59b839f1b33
 https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.0-pyhd8ed1ab_0.conda#95c5be3c7cbd872509d16c216617fdab
 https://conda.anaconda.org/conda-forge/osx-64/psutil-5.9.5-py38hef030d1_0.conda#20b4cc7adae881327b943c883be6335e
 https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2#359eeb6536da0e687af562ed265ec263
 https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2#6784285c7e55cb7212efabc79e4c2883
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
 https://conda.anaconda.org/conda-forge/noarch/pylev-1.4.0-pyhd8ed1ab_0.tar.bz2#edf8651c4379d9d1495ad6229622d150
@@ -122,15 +122,15 @@
 https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.17.1-pyhd8ed1ab_0.conda#dd4f393d857e9283eef2442234bd05e3
 https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.7-pyhd8ed1ab_0.conda#a61bf9ec79426938ff785eb69dbb1960
 https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
 https://conda.anaconda.org/conda-forge/osx-64/pyyaml-6.0-py38hef030d1_5.tar.bz2#e27d698dc29c6d5b49f1385bcd1d50f9
 https://conda.anaconda.org/conda-forge/osx-64/pyzmq-25.1.0-py38h3b70857_0.conda#a48761bc98b3bc22d209e9bb2f3dc5c1
 https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2#912a71cc01012ee38e6b90ddd561e36f
 https://conda.anaconda.org/conda-forge/osx-64/ruamel.yaml.clib-0.2.7-py38hef030d1_1.conda#9a8e866b0680b61b2e988b18a1eaecae
-https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda#3b68bc43ec6baa48f7354a446267eefe
+https://conda.anaconda.org/conda-forge/noarch/setuptools-68.0.0-pyhd8ed1ab_0.conda#5a7739d0f57ee64133c9d32e6507c46d
 https://conda.anaconda.org/conda-forge/noarch/shellingham-1.4.0-pyh44b312d_0.tar.bz2#437655338696f9d0dfdb0a024e66b255
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/smmap-3.0.5-pyh44b312d_0.tar.bz2#3a8dc70789709aa315325d5df06fb7e4
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
 https://conda.anaconda.org/conda-forge/noarch/snowballstemmer-2.2.0-pyhd8ed1ab_0.tar.bz2#4d22a9315e78c6827f806065957d566e
 https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
@@ -141,128 +141,130 @@
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-qthelp-1.0.3-py_0.tar.bz2#d01180388e6d1838c3e1ad029590aa7a
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-serializinghtml-1.1.5-pyhd8ed1ab_2.tar.bz2#9ff55a0901cf952f05c654394de76bf7
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.11.8-pyha770c72_0.conda#75838e8556166263a82038b51d01d5f1
 https://conda.anaconda.org/conda-forge/noarch/toolz-0.12.0-pyhd8ed1ab_0.tar.bz2#92facfec94bc02d6ccf42e7173831a36
 https://conda.anaconda.org/conda-forge/osx-64/tornado-6.3.2-py38hcafd530_0.conda#afefcf665a5049b030efb084a51e3935
 https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.3-pyha770c72_0.conda#4a3014a4d107d15475d106b751c4e352
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.0-pyha770c72_0.conda#c76ebd4731d3668ba16975a30ef19d0d
 https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/osx-64/unicodedata2-15.0.0-py38hef030d1_0.tar.bz2#51020c740c53f14657f6307b9eb23f85
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
-https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.0-pyhd8ed1ab_0.conda#1dd6387a73d84e16b6f73de676bb4c36
+https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda#c34d9325a609381a0b0e8a5b4f325147
 https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
 https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.7-pyhd8ed1ab_0.conda#bcc54b91a8ce88f60f538b87b409909e
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
 https://conda.anaconda.org/conda-forge/noarch/accessible-pygments-0.0.4-pyhd8ed1ab_0.conda#46a2e6e3dfa718ce3492018d5a110dd6
 https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.0-pyhd8ed1ab_1.conda#2b35a85d654a47aac8f34c1bb6de7142
 https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
 https://conda.anaconda.org/conda-forge/noarch/async-lru-2.0.2-pyhd8ed1ab_0.conda#41221f97a0c82e5a60b21716a3d7469c
 https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
-https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.4-pyhd8ed1ab_0.tar.bz2#c5b3edc62d6309088f4970b3eaaa65a6
+https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda#6b1b907661838a75d067a22f87996b2e
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
 https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda#d48b143d01385872a88ef8417e96c30e
 https://conda.anaconda.org/conda-forge/osx-64/cffi-1.15.1-py38hb368cf1_3.conda#a2b3ae2a1fd2aea0b4433d9e7fff8cf3
 https://conda.anaconda.org/conda-forge/noarch/click-default-group-1.2.2-pyhd8ed1ab_1.tar.bz2#72a46ffc25701c173932fd55cf0965d3
 https://conda.anaconda.org/conda-forge/noarch/clikit-0.6.2-pyhd8ed1ab_2.conda#02abb7b66b02e8b9f5a9b05454400087
 https://conda.anaconda.org/conda-forge/noarch/comm-0.1.3-pyhd8ed1ab_0.conda#168ae0f82cdf7505048e81054c7354e4
 https://conda.anaconda.org/conda-forge/osx-64/curl-8.1.2-hbee3ae8_0.conda#6cc301a6c2ba26e29949818efdc133ca
 https://conda.anaconda.org/eradiate/noarch/dessinemoi-23.1.0-py_0.tar.bz2#490780e63e113a7dc444bd068e049bfe
 https://conda.anaconda.org/conda-forge/noarch/environ-config-22.1.0-pyhd8ed1ab_0.tar.bz2#a1103faffa0a877313c1fba776aa0fc0
 https://conda.anaconda.org/conda-forge/osx-64/fonttools-4.40.0-py38hcafd530_0.conda#b26b38c5f75e03e86cecf860ca9fb1cd
 https://conda.anaconda.org/conda-forge/noarch/gitdb-4.0.10-pyhd8ed1ab_0.conda#3706d2f3d7cb5dae600c833345a76132
-https://conda.anaconda.org/conda-forge/osx-64/hdf5-1.14.0-nompi_hbf0aa07_103.conda#90f50d124606a4e62628823b614a2f4c
+https://conda.anaconda.org/conda-forge/osx-64/hdf5-1.14.1-nompi_hedada53_100.conda#033c310c83abbd9c2f9a5c13b9f54225
 https://conda.anaconda.org/conda-forge/noarch/html5lib-1.1-pyh9f0ad1d_0.tar.bz2#b2355343d6315c892543200231d7154a
 https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.7.0-pyha770c72_0.conda#ba3786c6846e46038fe60c785d46dc81
 https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
 https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.2.3-pyhd8ed1ab_0.tar.bz2#31e4a1506968d017229bdb64695013a1
 https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.2.2-pyhd8ed1ab_0.tar.bz2#243f63592c8e449f40cd42eb5cf32f40
 https://conda.anaconda.org/conda-forge/noarch/latexcodec-2.0.1-pyh9f0ad1d_0.tar.bz2#8d67904973263afd2985ba56aa2d6bb4
 https://conda.anaconda.org/conda-forge/osx-64/libblas-3.9.0-17_osx64_openblas.conda#65299527582e2449b05d27fcf8352125
 https://conda.anaconda.org/conda-forge/noarch/livereload-2.6.3-pyh9f0ad1d_0.tar.bz2#b7190e3ec3eff52839434bf4698e2d62
 https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-2.2.0-pyhd8ed1ab_0.conda#b2928a6c6d52d7e3562b4a59c3214e3a
 https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
 https://conda.anaconda.org/conda-forge/noarch/overrides-7.3.1-pyhd8ed1ab_0.tar.bz2#a5745ced46e69aa9754053ba061974ab
 https://conda.anaconda.org/conda-forge/noarch/pexpect-4.8.0-pyh1a96a4e_2.tar.bz2#330448ce4403cc74990ac07c555942a1
-https://conda.anaconda.org/conda-forge/osx-64/pillow-9.5.0-py38h16710f9_1.conda#c5bf174a033ef668679cc80918422515
+https://conda.anaconda.org/conda-forge/osx-64/pillow-10.0.0-py38h16710f9_0.conda#8f73f0573ab381d56588e001754c53d3
 https://conda.anaconda.org/eradiate/noarch/pinttrs-23.2.0-py_0.tar.bz2#1aebe9fa813278f719fa8e31d8000452
 https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
 https://conda.anaconda.org/conda-forge/noarch/portion-2.4.0-pyhd8ed1ab_0.conda#9d34bac22e169b41f4e34525a140c13b
 https://conda.anaconda.org/conda-forge/osx-64/pyobjc-core-9.2-py38h095c2e5_0.conda#8dbb4798b2066b678d8da47734d1c763
 https://conda.anaconda.org/conda-forge/noarch/pyproject_hooks-1.0.0-pyhd8ed1ab_0.conda#21de50391d584eb7f4441b9de1ad773f
-https://conda.anaconda.org/conda-forge/noarch/pytest-7.3.2-pyhd8ed1ab_1.conda#f2465696f4396245eca4613f6e924796
+https://conda.anaconda.org/conda-forge/noarch/pytest-7.4.0-pyhd8ed1ab_0.conda#3cfe9b9e958e7238a386933c75d190db
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
 https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
 https://conda.anaconda.org/conda-forge/osx-64/ruamel.yaml-0.17.32-py38hcafd530_0.conda#cb301e0b2b162330bc3b03fe51ea0d15
 https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.1-pyhd1c38e8_0.conda#046120b71d8896cb7faef78bfdbfee1e
 https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
 https://conda.anaconda.org/conda-forge/noarch/tqdm-4.65.0-pyhd8ed1ab_1.conda#ed792aff3acb977d09c7013358097f83
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.3-hd8ed1ab_0.conda#3876f650ed7d0f95d70fa4b647621909
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.0-hd8ed1ab_0.conda#37761dccc7ca8eaa08c60c4f62eb2dcc
+https://conda.anaconda.org/conda-forge/noarch/annotated-types-0.5.0-pyhd8ed1ab_0.conda#578ae086f225bc2380c79f3b551ff2f7
 https://conda.anaconda.org/conda-forge/osx-64/argon2-cffi-bindings-21.2.0-py38hef030d1_3.tar.bz2#fc1bc20add8eff07c367973bba25e8eb
 https://conda.anaconda.org/conda-forge/osx-64/brotlipy-0.7.0-py38hef030d1_1005.tar.bz2#2fa6826f6f94c847bf26709f2162a09c
 https://conda.anaconda.org/conda-forge/osx-64/cryptography-41.0.1-py38he13da33_0.conda#845f16b2278f26769e23796d04636e06
 https://conda.anaconda.org/conda-forge/noarch/gitpython-3.1.31-pyhd8ed1ab_0.conda#f6e6b482110246a81c3f03e81c68752d
 https://conda.anaconda.org/conda-forge/noarch/importlib-resources-5.12.0-pyhd8ed1ab_0.conda#3544c818f0720c89eb16ae6940ab440b
 https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.7.0-hd8ed1ab_0.conda#27a4cec373ec84d1c1aa02a1e37f8eaf
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.4.4-pyhd8ed1ab_1.conda#7c0965e1d4a0ee1529e8eaa03a78a5b3
 https://conda.anaconda.org/conda-forge/osx-64/libcblas-3.9.0-17_osx64_openblas.conda#380151ca00704172b242a63701b7bf8a
 https://conda.anaconda.org/conda-forge/osx-64/liblapack-3.9.0-17_osx64_openblas.conda#6ab83532872bf3659613638589dd10af
-https://conda.anaconda.org/conda-forge/osx-64/libnetcdf-4.9.2-nompi_hf077d52_105.conda#64d626e024a284777458e2b315e9eb56
+https://conda.anaconda.org/conda-forge/osx-64/libnetcdf-4.9.2-nompi_hfeda9e8_106.conda#66108519efbf30b02632ad35f519773f
 https://conda.anaconda.org/conda-forge/noarch/mdit-py-plugins-0.4.0-pyhd8ed1ab_0.conda#6c5358a10873a15398b6f15f60cb5e1f
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.6.0-pyhd8ed1ab_0.conda#741384b21c1b512617f4ee4ea8457c5d
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.8.0-pyhd8ed1ab_0.conda#3e4aca765371893ad848397794600632
 https://conda.anaconda.org/conda-forge/noarch/pybtex-0.24.0-pyhd8ed1ab_2.tar.bz2#2099b86a7399c44c0c61cdb6de6915ba
-https://conda.anaconda.org/conda-forge/osx-64/pydantic-1.10.9-py38hcafd530_0.conda#253819655b95aedbeddf0ff7fa26cf16
+https://conda.anaconda.org/conda-forge/osx-64/pydantic-core-2.0.1-py38h7510fb3_0.conda#85a94a4914e522e379c1c36cb38923a1
 https://conda.anaconda.org/conda-forge/osx-64/pyobjc-framework-cocoa-9.2-py38h095c2e5_0.conda#fa3e3307ff143e7a9e823ce7bbc916ad
 https://conda.anaconda.org/conda-forge/noarch/pytest-metadata-3.0.0-pyhd8ed1ab_1.conda#8bdcc0f401561213821bf67513abeeff
 https://conda.anaconda.org/conda-forge/noarch/python-build-0.10.0-pyhd8ed1ab_1.conda#0ab47ce574f6a8bcb9f2076436e7fedb
 https://conda.anaconda.org/conda-forge/noarch/rich-13.4.2-pyhd8ed1ab_0.conda#f993baacc175e83fafd6b846e9c4c8a2
 https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
 https://conda.anaconda.org/conda-forge/osx-64/jupyter_core-5.3.1-py38h50d1736_0.conda#03a3619e222793567b29b5966c2a821d
 https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
-https://conda.anaconda.org/conda-forge/osx-64/keyring-23.13.1-py38h50d1736_0.conda#7ba9ac4c5edbaddcffe213189e679b13
-https://conda.anaconda.org/conda-forge/osx-64/numpy-1.24.3-py38h9a4a08f_0.conda#5ff64b8133dea66865fe1bd35fb1d6d6
-https://conda.anaconda.org/conda-forge/noarch/pip-tools-6.13.0-pyhd8ed1ab_1.conda#566e41c99730f1124d6948ab8fe1c18d
+https://conda.anaconda.org/conda-forge/osx-64/keyring-24.2.0-py38h50d1736_0.conda#150c457dbd44f1b53e77ebf98a1680ec
+https://conda.anaconda.org/conda-forge/osx-64/numpy-1.24.4-py38h9a4a08f_0.conda#85debc55a30068d6bb76a6deaf599afa
+https://conda.anaconda.org/conda-forge/noarch/pip-tools-6.14.0-pyhd8ed1ab_0.conda#4c3828f6213d5ddba2f5033d4b422d17
 https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
 https://conda.anaconda.org/conda-forge/osx-64/pybtex-docutils-1.0.2-py38h50d1736_2.tar.bz2#5650c819d7ae44ff91c456370f175706
+https://conda.anaconda.org/conda-forge/osx-64/pydantic-2.0-py38hcafd530_0.conda#475d41478cd6aa73a1d0930fdee989ab
 https://conda.anaconda.org/conda-forge/noarch/pyopenssl-23.2.0-pyhd8ed1ab_1.conda#34f7d568bf59d18e3fef8c405cbece21
 https://conda.anaconda.org/conda-forge/noarch/pytest-json-report-1.5.0-pyhd8ed1ab_0.tar.bz2#837e335fa428cf7c784ee2e80594506c
 https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyhd1c38e8_0.conda#2657c3de5371c571aef6678afb4aaadd
 https://conda.anaconda.org/conda-forge/noarch/typer-0.9.0-pyhd8ed1ab_0.conda#5030a13b2fe5e143d5956d4943d3018f
 https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.23.1-pyhd8ed1ab_0.conda#838b85f656b078bdd882ef97978e7f40
 https://conda.anaconda.org/conda-forge/osx-64/cftime-1.6.2-py38hbd87e4b_1.tar.bz2#6b61efa56393b9655334192cc5423659
 https://conda.anaconda.org/conda-forge/osx-64/contourpy-1.1.0-py38h15a1a5b_0.conda#30d645ffb3572a3875e6fc8687857182
-https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.2.0-pyhd8ed1ab_0.conda#58ca2d50c3b27b86fd7df62eaadbf9a9
+https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda#1d018ee4ab13217e2544f795eb0a6798
 https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.0-pyhd8ed1ab_0.conda#f525a01528c3eba1d381a232a6971c6a
 https://conda.anaconda.org/conda-forge/osx-64/pandas-1.5.3-py38hec72209_1.conda#a8f001ab0a7c6312cea020bd20689765
 https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.38-hd8ed1ab_0.conda#45b74f64d8808eda7e6f6e6b1d641fd2
 https://conda.anaconda.org/conda-forge/osx-64/pyerfa-2.0.0.3-py38hbd87e4b_0.conda#48a43c20176ae9fba912e9142bc066ad
 https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.15-pyhd8ed1ab_0.conda#27db656619a55d727eaf5a6ece3d2fd6
 https://conda.anaconda.org/conda-forge/osx-64/astropy-5.0.6-py38h073b4c8_0.conda#d2955fea4da9c60ab73746c1d7e588bb
 https://conda.anaconda.org/conda-forge/noarch/ipython-8.12.0-pyhd1c38e8_0.conda#4b25de6cd2891e6bce87de8c5d85e27c
 https://conda.anaconda.org/conda-forge/osx-64/matplotlib-base-3.7.1-py38hcb346ec_0.conda#1f1eea98c232c8ef720175e12b00d0c4
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.8.0-pyhd8ed1ab_0.conda#e78da91cf428faaf05701ce8cc8f2f9b
-https://conda.anaconda.org/conda-forge/osx-64/netcdf4-1.6.4-nompi_py38h47ac6a0_100.conda#f86d4df9f8f46ae6d0c29bb87fe093b0
+https://conda.anaconda.org/conda-forge/osx-64/netcdf4-1.6.4-nompi_py38ha129777_101.conda#0e0f917d6168b9744a407d5ef3c2cb09
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/noarch/xarray-2023.1.0-pyhd8ed1ab_0.conda#c11eb03b6f77a0d22ae88c454c940f55
 https://conda.anaconda.org/conda-forge/noarch/cachecontrol-0.13.0-pyhd8ed1ab_0.conda#9f0b2eb5f5dd2cec36d5342a80adfec0
 https://conda.anaconda.org/conda-forge/noarch/ensureconda-1.4.3-pyhd8ed1ab_0.tar.bz2#c99ae3abf501990769047b4b40a98f17
-https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.1-pyh736e0ef_0.conda#d5aa7d2cc9fe03f62cf6e7bcc8e1a8df
+https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.3-pyh5fb750a_0.conda#00cfe411a8e07b8322185e573ae7c5a3
 https://conda.anaconda.org/conda-forge/osx-64/matplotlib-3.7.1-py38h50d1736_0.conda#14bce132d8a4546246b131c4289b480f
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.6.0-pyhd8ed1ab_0.conda#879782bde4bbdb4c7b5d4054504a20d5
 https://conda.anaconda.org/conda-forge/noarch/pooch-1.7.0-pyha770c72_3.conda#5936894aade8240c867d292aa0d980c6
 https://conda.anaconda.org/conda-forge/noarch/sphinx-5.0.0-pyh6c4a22f_1.tar.bz2#a7cc4b9c94548ff9a19b368f975e5404
 https://conda.anaconda.org/conda-forge/noarch/autodocsumm-0.2.11-pyhd8ed1ab_0.conda#547c48372c97c463c93af86d7f2c868c
 https://conda.anaconda.org/conda-forge/noarch/cachecontrol-with-filecache-0.13.0-pyhd8ed1ab_0.conda#3fd3d55ea862cc0736ac1cce6f44c2d1
 https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.6-pyhd8ed1ab_0.conda#68627a08556e4a273e4c7bfc84251457
-https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.6.0-pyhd8ed1ab_0.conda#39fd52b0fcb2fb52bac47a1419bf09bd
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.7.0-pyhd8ed1ab_0.conda#7488cd1f4d35a2af96faa765b7e5b2f0
 https://conda.anaconda.org/conda-forge/noarch/myst-parser-0.18.1-pyhd8ed1ab_0.tar.bz2#bcfdf5c7d8bf5c6f6be7b4c66fff2eca
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.6.0-pyhd8ed1ab_0.conda#e8172ca42f2869bb90185c9356899e81
 https://conda.anaconda.org/conda-forge/noarch/pydata-sphinx-theme-0.13.3-pyhd8ed1ab_0.conda#07aca5f2dea315dcc16680d6891e9056
 https://conda.anaconda.org/conda-forge/osx-64/scipy-1.10.1-py38h9cf86d3_3.conda#5e20c77455e815704b008ab8f42f6169
 https://conda.anaconda.org/conda-forge/noarch/sphinx-autobuild-2021.3.14-pyhd8ed1ab_0.tar.bz2#1909f784dc37b4ab97afe2c95aeeabaa
 https://conda.anaconda.org/conda-forge/noarch/sphinx-copybutton-0.5.2-pyhd8ed1ab_0.conda#ac832cc43adc79118cf6e23f1f9b8995
 https://conda.anaconda.org/conda-forge/noarch/sphinx-design-0.4.1-pyhd8ed1ab_1.conda#c6b2e7903121c3210462a0866a561993
```

### Comparing `eradiate-0.23.2rc3/requirements/conda/environment-dev.dot` & `eradiate-0.23.2rc4/requirements/conda/environment-dev.dot`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/requirements/conda/environment-dev.yml` & `eradiate-0.23.2rc4/requirements/conda/environment-dev.yml`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/requirements/conda/environment-docs-linux-64.lock` & `eradiate-0.23.2rc4/requirements/conda/environment-docs-linux-64.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Generated by conda-lock.
 # platform: linux-64
-# input_hash: b7bbfe20c225205e6a608fff7b6e10034a7098a907606a9ce8f56207b6fb77e8
+# input_hash: f387df537a374bb0bb7066e2ab37db09fde2ece77dde681a595c2588a08347d9
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2#d7c89558ba9fa0495403155b64376d81
 https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2023.5.7-hbcca054_0.conda#f5c65075fc34438d5b456c7f3f5ab695
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-dejavu-sans-mono-2.37-hab24e00_0.tar.bz2#0c96522c6bdaed4b1566d11387caaf45
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-inconsolata-3.000-h77eed37_0.tar.bz2#34893075a5c9e55cdafac56607368fc6
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-source-code-pro-2.038-h77eed37_0.tar.bz2#4d59c254e01d9cde7957100457e2d5fb
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-ubuntu-0.83-hab24e00_0.tar.bz2#19410c3df09dfb12d1206132a1d357c5
@@ -26,28 +26,28 @@
 https://conda.anaconda.org/conda-forge/linux-64/gmp-6.2.1-h58526e2_0.tar.bz2#b94cf2db16066b242ebd26db2facbd56
 https://conda.anaconda.org/conda-forge/linux-64/graphite2-1.3.13-h58526e2_1001.tar.bz2#8c54672728e8ec6aa6db90cf2806d220
 https://conda.anaconda.org/conda-forge/linux-64/icu-72.1-hcb278e6_0.conda#7c8d20d847bb45f56bd941578fcfa146
 https://conda.anaconda.org/conda-forge/linux-64/keyutils-1.6.1-h166bdaf_0.tar.bz2#30186d27e2c9fa62b45fb1476b7200e3
 https://conda.anaconda.org/conda-forge/linux-64/lame-3.100-h166bdaf_1003.tar.bz2#a8832b479f93521a9e7b5b743803be51
 https://conda.anaconda.org/conda-forge/linux-64/lerc-4.0.0-h27087fc_0.tar.bz2#76bbff344f0134279f225174e9064c8f
 https://conda.anaconda.org/conda-forge/linux-64/libaec-1.0.6-hcb278e6_1.conda#0f683578378cddb223e7fd24f785ab2a
-https://conda.anaconda.org/conda-forge/linux-64/libbrotlicommon-1.0.9-h166bdaf_8.tar.bz2#9194c9bf9428035a05352d031462eae4
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlicommon-1.0.9-h166bdaf_9.conda#61641e239f96eae2b8492dc7e755828c
 https://conda.anaconda.org/conda-forge/linux-64/libdeflate-1.18-h0b41bf4_0.conda#6aa9c9de5542ecb07fdda9ca626252d8
 https://conda.anaconda.org/conda-forge/linux-64/libev-4.33-h516909a_1.tar.bz2#6f8720dff19e17ce5d48cfe7f3d2f0a3
 https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.5.0-hcb278e6_1.conda#6305a3dd2752c76335295da4e581f2fd
 https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2#d645c6d2ac96843a2bfaccd2d62b3ac3
 https://conda.anaconda.org/conda-forge/linux-64/libiconv-1.17-h166bdaf_0.tar.bz2#b62b52da46c39ee2bc3c162ac7f1804d
 https://conda.anaconda.org/conda-forge/linux-64/libjpeg-turbo-2.1.5.1-h0b41bf4_0.conda#1edd9e67bdb90d78cea97733ff6b54e6
 https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.0-h7f98852_0.tar.bz2#39b1328babf85c7c3a61636d9cd50206
-https://conda.anaconda.org/conda-forge/linux-64/libogg-1.3.4-h7f98852_1.tar.bz2#6e8cc2173440d77708196c5b93771680
+https://repo.anaconda.com/pkgs/main/linux-64/libogg-1.3.5-h27cfd23_1.conda#710ee7fdb0ddf7591a5af7ca7eb4d73d
 https://conda.anaconda.org/conda-forge/linux-64/libopenblas-0.3.23-pthreads_h80387f5_0.conda#9c5ea51ccb8ffae7d06c645869d24ce6
 https://conda.anaconda.org/conda-forge/linux-64/libopus-1.3.1-h7f98852_1.tar.bz2#15345e56d527b330e1cacbdf58676e8f
 https://conda.anaconda.org/conda-forge/linux-64/libsodium-1.0.18-h36c2ea0_1.tar.bz2#c3788462a6fbddafdb413a9f9053e58d
 https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda#40b61aab5c7ba9ff276c41cfffe6b80b
-https://conda.anaconda.org/conda-forge/linux-64/libwebp-base-1.3.0-h0b41bf4_0.conda#0d4a7508d8c6c65314f2b9c1f56ad408
+https://conda.anaconda.org/conda-forge/linux-64/libwebp-base-1.3.1-hd590300_0.conda#82bf6f63eb15ef719b556b63feec3a77
 https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-hd590300_5.conda#f36c115f1ee199da648e0597ec2047ad
 https://conda.anaconda.org/conda-forge/linux-64/lz4-c-1.9.4-hcb278e6_0.conda#318b08df404f9c9be5712aaa5a6f0bb0
 https://conda.anaconda.org/conda-forge/linux-64/mpg123-1.31.3-hcb278e6_0.conda#141a126675b6d1a4eabb111a4a353898
 https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.4-hcb278e6_0.conda#681105bccc2a3f7f1a837d47d39c9179
 https://conda.anaconda.org/conda-forge/linux-64/nspr-4.35-h27087fc_0.conda#da0ec11a6454ae19bff5b02ed881a2b1
 https://conda.anaconda.org/conda-forge/linux-64/openssl-3.1.1-hd590300_1.conda#2e1d7b458ac8f1e3ca4e18b77add6277
 https://conda.anaconda.org/conda-forge/linux-64/pixman-0.40.0-h36c2ea0_0.tar.bz2#660e72c82f2e75a6b3fe6a6e75c79f19
@@ -62,61 +62,62 @@
 https://conda.anaconda.org/conda-forge/linux-64/xorg-xf86vidmodeproto-2.3.1-h7f98852_1002.tar.bz2#3ceea9668625c18f19530de98b15d5b0
 https://conda.anaconda.org/conda-forge/linux-64/xorg-xproto-7.0.31-h7f98852_1007.tar.bz2#b4a4381d54784606820704f7b5f05a15
 https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2#2161070d867d1b1204ea749c8eec4ef0
 https://conda.anaconda.org/conda-forge/linux-64/yaml-0.2.5-h7f98852_2.tar.bz2#4cb3ad778ec2d5a7acbdf254eb1c42ae
 https://conda.anaconda.org/conda-forge/linux-64/expat-2.5.0-hcb278e6_1.conda#8b9b5aca60558d02ddaa09d599e55920
 https://conda.anaconda.org/conda-forge/linux-64/hdf4-4.2.15-h501b40f_6.conda#c3e9338e15d90106f467377017352b97
 https://conda.anaconda.org/conda-forge/linux-64/libblas-3.9.0-17_linux64_openblas.conda#57fb44770b1bc832fb2dbefa1bd502de
-https://conda.anaconda.org/conda-forge/linux-64/libbrotlidec-1.0.9-h166bdaf_8.tar.bz2#4ae4d7795d33e02bd20f6b23d91caf82
-https://conda.anaconda.org/conda-forge/linux-64/libbrotlienc-1.0.9-h166bdaf_8.tar.bz2#04bac51ba35ea023dc48af73c1c88c25
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlidec-1.0.9-h166bdaf_9.conda#081aa22f4581c08e4372b0b6c2f8478e
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlienc-1.0.9-h166bdaf_9.conda#1f0a03af852a9659ed2bf08f2f1704fd
 https://conda.anaconda.org/conda-forge/linux-64/libcap-2.67-he9d0100_0.conda#d05556c80caffff164d17bdea0105a1a
 https://conda.anaconda.org/conda-forge/linux-64/libedit-3.1.20191231-he28a2e2_2.tar.bz2#4d331e44109e3f0e19b4cb8f9b82f3e1
 https://conda.anaconda.org/conda-forge/linux-64/libevent-2.1.12-hf998b51_1.conda#a1cfcc585f0c42bf8d5546bb1dfb668d
-https://conda.anaconda.org/conda-forge/linux-64/libflac-1.4.2-h27087fc_0.tar.bz2#7daf72d8e2a8e848e11d63ed6d1026e0
+https://conda.anaconda.org/conda-forge/linux-64/libflac-1.4.3-h59595ed_0.conda#ee48bf17cc83a00f59ca1494d5646869
 https://conda.anaconda.org/conda-forge/linux-64/libgpg-error-1.47-h71f35ed_0.conda#c2097d0b46367996f09b4e8e4920384a
 https://conda.anaconda.org/conda-forge/linux-64/libnghttp2-1.52.0-h61bc06f_0.conda#613955a50485812985c059e7b269f42e
 https://conda.anaconda.org/conda-forge/linux-64/libpng-1.6.39-h753d276_0.conda#e1c890aebdebbfbf87e2c917187b4416
 https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.42.0-h2797004_0.conda#fdaae20a1cf7cd62130a0973190a31b7
 https://conda.anaconda.org/conda-forge/linux-64/libssh2-1.11.0-h0841786_0.conda#1f5a58e686b13bcfde88b93f547d23fe
 https://conda.anaconda.org/conda-forge/linux-64/libvorbis-1.3.7-h9c3ff4c_0.tar.bz2#309dec04b70a3cc0f1e84a4013683bc0
 https://conda.anaconda.org/conda-forge/linux-64/libxcb-1.15-h0b41bf4_0.conda#33277193f5b92bad9fdd230eb700929c
 https://conda.anaconda.org/conda-forge/linux-64/libxml2-2.11.4-h0d562d8_0.conda#e46fad17d5fb57316b956f88dca765e4
 https://conda.anaconda.org/conda-forge/linux-64/libzip-1.9.2-hc929e4a_1.tar.bz2#5b122b50e738c4be5c3f2899f010d7cf
-https://conda.anaconda.org/conda-forge/linux-64/mysql-common-8.0.33-hf1915f5_0.conda#aa8b86066614c4573f6db62c91978fa9
+https://conda.anaconda.org/conda-forge/linux-64/mysql-common-8.0.33-hf1915f5_1.conda#b241363e3b72bae6dfbd31e9fecf7d26
 https://conda.anaconda.org/conda-forge/linux-64/pcre2-10.40-hc3806b6_0.tar.bz2#69e2c796349cd9b273890bee0febfe1b
 https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda#47d31b792659ce70f470b5c82fdfb7a4
 https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.12-h27826a3_0.tar.bz2#5b8c42eb62e9fc961af70bdd6a26e168
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libsm-1.2.4-h7391055_0.conda#93ee23f12bc2e684548181256edd2cf6
 https://conda.anaconda.org/conda-forge/linux-64/zeromq-4.3.4-h9c3ff4c_1.tar.bz2#21743a8d2ea0c8cfbbf8fe489b0347df
 https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.13-hd590300_5.conda#68c34ec6149623be41a1933ab996a209
 https://conda.anaconda.org/conda-forge/linux-64/zstd-1.5.2-h3eb15da_6.conda#6b63daed8feeca47be78f323e793d555
 https://conda.anaconda.org/conda-forge/linux-64/blosc-1.21.4-h0f2a231_0.conda#876286b5941933a0f558777e57d883cc
-https://conda.anaconda.org/conda-forge/linux-64/brotli-bin-1.0.9-h166bdaf_8.tar.bz2#e5613f2bc717e9945840ff474419b8e4
+https://conda.anaconda.org/conda-forge/linux-64/brotli-bin-1.0.9-h166bdaf_9.conda#d47dee1856d9cb955b8076eeff304a5b
 https://conda.anaconda.org/conda-forge/linux-64/freetype-2.12.1-hca18f0e_1.conda#e1232042de76d24539a436d37597eb06
 https://conda.anaconda.org/conda-forge/linux-64/krb5-1.20.1-h81ceb04_0.conda#89a41adce7106749573d883b2f657d78
 https://conda.anaconda.org/conda-forge/linux-64/libcblas-3.9.0-17_linux64_openblas.conda#7ef0969b00fe3d6eef56a8151d3afb29
 https://conda.anaconda.org/conda-forge/linux-64/libgcrypt-1.10.1-h166bdaf_0.tar.bz2#f967fc95089cd247ceed56eda31de3a9
 https://conda.anaconda.org/conda-forge/linux-64/libglib-2.76.3-hebfc3b9_0.conda#a64f11b244b2c112cd3fa1cbe9493999
 https://conda.anaconda.org/conda-forge/linux-64/liblapack-3.9.0-17_linux64_openblas.conda#a2103882c46492e26500fcb56c03de8b
 https://conda.anaconda.org/conda-forge/linux-64/libllvm16-16.0.6-h5cf9203_0.conda#753e078cccad40fe4b396bdcf27a3c15
 https://conda.anaconda.org/conda-forge/linux-64/libsndfile-1.2.0-hb75c966_0.conda#c648d19cd9c8625898d5d370414de7c7
 https://conda.anaconda.org/conda-forge/linux-64/libtiff-4.5.1-h8b53f26_0.conda#8ad377fb60abab446a9f02c62b3c2190
-https://conda.anaconda.org/conda-forge/linux-64/mysql-libs-8.0.33-hca2cd23_0.conda#276339b0115d92c6e0793dcdc7afe308
+https://conda.anaconda.org/conda-forge/linux-64/mysql-libs-8.0.33-hca2cd23_1.conda#a04ac37f0659929f3ba0f33c7f3d750f
 https://conda.anaconda.org/conda-forge/linux-64/nss-3.89-he45b914_0.conda#2745719a58eeaab6657256a3f142f099
 https://conda.anaconda.org/conda-forge/linux-64/pandoc-3.1.3-h32600fe_0.conda#8287aeb8462e2d4b235eff788e75919d
 https://conda.anaconda.org/conda-forge/linux-64/python-3.8.17-he550d4f_0_cpython.conda#72d038de0a228e4f0ef4011940641293
 https://conda.anaconda.org/conda-forge/linux-64/xcb-util-0.4.0-hd590300_1.conda#9bfac7ccd94d54fd21a0501296d60424
 https://conda.anaconda.org/conda-forge/linux-64/xcb-util-keysyms-0.4.0-h8ee46fc_1.conda#632413adcd8bc16b515cab87a2932913
 https://conda.anaconda.org/conda-forge/linux-64/xcb-util-renderutil-0.3.9-hd590300_1.conda#e995b155d938b6779da6ace6c6b13816
 https://conda.anaconda.org/conda-forge/linux-64/xcb-util-wm-0.4.1-h8ee46fc_1.conda#90108a432fb5c6150ccfee3f03388656
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libx11-1.8.6-h8ee46fc_0.conda#7590b76c3d11d21caa44f3fc38ac584a
-https://conda.anaconda.org/conda-forge/noarch/aenum-3.1.12-pyhd8ed1ab_0.conda#602716538da00b2ca3cc85c4d35c0245
+https://conda.anaconda.org/conda-forge/noarch/aenum-3.1.15-pyhd8ed1ab_0.conda#24cff7ab050ebb8a16bdeb02e8ed6f63
 https://conda.anaconda.org/conda-forge/noarch/alabaster-0.7.13-pyhd8ed1ab_0.conda#06006184e203b61d3525f90de394471e
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
-https://conda.anaconda.org/conda-forge/linux-64/brotli-1.0.9-h166bdaf_8.tar.bz2#2ff08978892a3e8b954397c461f18418
+https://conda.anaconda.org/conda-forge/linux-64/brotli-1.0.9-h166bdaf_9.conda#4601544b4982ba1861fa9b9c607b2c06
+https://conda.anaconda.org/conda-forge/linux-64/brotli-python-1.0.9-py38hfa26641_9.conda#d056745008e5ed73210a31dcfd4d183a
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
 https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-unix_pyhd8ed1ab_2.tar.bz2#20e4087407c7cb04a40817114b333dbf
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/noarch/cycler-0.11.0-pyhd8ed1ab_0.tar.bz2#a50559fad0affdbb33729a68669ca1cb
 https://conda.anaconda.org/conda-forge/noarch/dataclasses-0.8-pyhc8e2a94_3.tar.bz2#a362b2124b06aad102e2ee4581acee7d
 https://conda.anaconda.org/conda-forge/linux-64/dbus-1.13.6-h5008d03_3.tar.bz2#ecfff944ba3960ecb334b9a2663d708d
@@ -135,15 +136,15 @@
 https://conda.anaconda.org/conda-forge/linux-64/libcurl-8.1.2-h409715c_0.conda#50c873c9660ed116707ae15b663928d8
 https://conda.anaconda.org/conda-forge/linux-64/libpq-15.3-hbcd7760_1.conda#8afb2a97d256ffde95b91a6283bc598c
 https://conda.anaconda.org/conda-forge/linux-64/libsystemd0-253-h8c4010b_1.conda#9176b1e2cb8beca37a7510b0e801e38f
 https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.3-py38h01eb140_0.conda#17d2a5314adf0f25220eeebb312d00a4
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.0-pyhd8ed1ab_0.tar.bz2#f8dab71fdc13b1bf29a01248b156d268
 https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.0-pyhd8ed1ab_0.conda#c7d0ea64c37752ecbe6da458aee662d2
 https://conda.anaconda.org/conda-forge/noarch/munkres-1.1.4-pyh9f0ad1d_0.tar.bz2#2ba8498c1018c1e9c61eb99b973dfe19
-https://conda.anaconda.org/conda-forge/linux-64/numpy-1.24.3-py38h59b608b_0.conda#5836e4ab0399136ede58446a4776b2ff
+https://conda.anaconda.org/conda-forge/linux-64/numpy-1.24.4-py38h59b608b_0.conda#8c3e050afeeb2b32575bdb8955cc67b2
 https://conda.anaconda.org/conda-forge/linux-64/openjpeg-2.5.0-hfec8fc6_2.conda#5ce6a42505c6e9e6151c54c3ec8d68ea
 https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/pint-0.21-pyhd8ed1ab_0.conda#8d7b829e37d78447569c180f9d827005
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2#89e3c7cdde7d3aaa2aee933b604dd07f
 https://conda.anaconda.org/conda-forge/noarch/ply-3.11-py_1.tar.bz2#7205635cd71531943440fbfe3b6b5727
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
@@ -151,15 +152,15 @@
 https://conda.anaconda.org/conda-forge/linux-64/pyrsistent-0.19.3-py38h1de0b5d_0.conda#a33157288d499397a2a56da4d724948d
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
 https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.17.1-pyhd8ed1ab_0.conda#dd4f393d857e9283eef2442234bd05e3
 https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
 https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0-py38h0a891b7_5.tar.bz2#0856c59f9ddb710c640dc0428d66b1b7
 https://conda.anaconda.org/conda-forge/linux-64/pyzmq-25.1.0-py38h509eb50_0.conda#33872b6650886eba869408b76c96994c
 https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml.clib-0.2.7-py38h1de0b5d_1.conda#9afa2fc3c51cc4e7d1589c38e4e00d5c
-https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda#3b68bc43ec6baa48f7354a446267eefe
+https://conda.anaconda.org/conda-forge/noarch/setuptools-68.0.0-pyhd8ed1ab_0.conda#5a7739d0f57ee64133c9d32e6507c46d
 https://conda.anaconda.org/conda-forge/noarch/shellingham-1.4.0-pyh44b312d_0.tar.bz2#437655338696f9d0dfdb0a024e66b255
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/snowballstemmer-2.2.0-pyhd8ed1ab_0.tar.bz2#4d22a9315e78c6827f806065957d566e
 https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-applehelp-1.0.4-pyhd8ed1ab_0.conda#5a31a7d564f551d0e6dff52fd8cb5b16
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-devhelp-1.0.2-py_0.tar.bz2#68e01cac9d38d0e717cd5c87bc3d2cc9
@@ -167,76 +168,76 @@
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-jsmath-1.0.1-py_0.tar.bz2#67cd9d9c0382d37479b4d306c369a2d4
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-qthelp-1.0.3-py_0.tar.bz2#d01180388e6d1838c3e1ad029590aa7a
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-serializinghtml-1.1.5-pyhd8ed1ab_2.tar.bz2#9ff55a0901cf952f05c654394de76bf7
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/linux-64/tornado-6.3.2-py38h01eb140_0.conda#3db869202b0e523d606d13e81ca79ab6
 https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.3-pyha770c72_0.conda#4a3014a4d107d15475d106b751c4e352
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.0-pyha770c72_0.conda#c76ebd4731d3668ba16975a30ef19d0d
 https://conda.anaconda.org/conda-forge/linux-64/unicodedata2-15.0.0-py38h0a891b7_0.tar.bz2#44421904760e9f5ae2035193e04360f0
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
 https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
 https://conda.anaconda.org/conda-forge/linux-64/xcb-util-image-0.4.0-h8ee46fc_1.conda#9d7bcddf49cbf727730af10e71022c73
 https://conda.anaconda.org/conda-forge/linux-64/xkeyboard-config-2.39-hd590300_0.conda#d88c7fc8a11858fb14761832e4da1954
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxext-1.3.4-h0b41bf4_2.conda#82b6df12252e6f32402b96dacc656fec
-https://conda.anaconda.org/conda-forge/linux-64/xorg-libxrender-0.9.10-h7f98852_1003.tar.bz2#f59c1242cc1dd93e72c2ee2b360979eb
+https://conda.anaconda.org/conda-forge/linux-64/xorg-libxrender-0.9.11-hd590300_0.conda#ed67c36f215b310412b2af935bf3e530
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
 https://conda.anaconda.org/conda-forge/noarch/accessible-pygments-0.0.4-pyhd8ed1ab_0.conda#46a2e6e3dfa718ce3492018d5a110dd6
 https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
 https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda#d48b143d01385872a88ef8417e96c30e
 https://conda.anaconda.org/conda-forge/linux-64/cairo-1.16.0-hbbf8b49_1016.conda#c1dd96500b9b1a75e9e511931f415cbc
 https://conda.anaconda.org/conda-forge/linux-64/cftime-1.6.2-py38h26c90d9_1.tar.bz2#dcc025a7bb54374979c500c2e161fac9
 https://conda.anaconda.org/conda-forge/linux-64/contourpy-1.1.0-py38h7f3f72f_0.conda#0fdf3cc879156e0234e05962d55b6502
 https://conda.anaconda.org/conda-forge/linux-64/curl-8.1.2-h409715c_0.conda#9f88cfb15b7d08b25880b138f91e0eb4
 https://conda.anaconda.org/eradiate/noarch/dessinemoi-23.1.0-py_0.tar.bz2#490780e63e113a7dc444bd068e049bfe
 https://conda.anaconda.org/conda-forge/noarch/environ-config-22.1.0-pyhd8ed1ab_0.tar.bz2#a1103faffa0a877313c1fba776aa0fc0
 https://conda.anaconda.org/conda-forge/linux-64/fonttools-4.40.0-py38h01eb140_0.conda#f893b6bac56c477dd71498569b4a9022
 https://conda.anaconda.org/conda-forge/linux-64/glib-2.76.3-hfc55251_0.conda#950e02f5665f5f4ff0437a6acba58798
-https://conda.anaconda.org/conda-forge/linux-64/hdf5-1.14.0-nompi_hb72d44e_103.conda#975973a4350ab45ff1981fe535a12af5
+https://conda.anaconda.org/conda-forge/linux-64/hdf5-1.14.1-nompi_h4f84152_100.conda#ff9ae10aa224826c07da7ef26cb0b717
 https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.7.0-pyha770c72_0.conda#ba3786c6846e46038fe60c785d46dc81
 https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
 https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-4.12.0-py38h578d9bd_0.conda#e7f204764ab3683174c1707240368b84
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.2.2-pyhd8ed1ab_0.tar.bz2#243f63592c8e449f40cd42eb5cf32f40
 https://conda.anaconda.org/conda-forge/noarch/latexcodec-2.0.1-pyh9f0ad1d_0.tar.bz2#8d67904973263afd2985ba56aa2d6bb4
 https://conda.anaconda.org/conda-forge/linux-64/libclang-16.0.6-default_h1cdf331_0.conda#e976871e132fe506da52c1240229246a
 https://conda.anaconda.org/conda-forge/linux-64/libxkbcommon-1.5.0-h5d7e998_3.conda#c91ea308d7bf70b62ddda568478aa03b
 https://conda.anaconda.org/conda-forge/noarch/livereload-2.6.3-pyh9f0ad1d_0.tar.bz2#b7190e3ec3eff52839434bf4698e2d62
 https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-2.2.0-pyhd8ed1ab_0.conda#b2928a6c6d52d7e3562b4a59c3214e3a
-https://conda.anaconda.org/conda-forge/linux-64/pillow-9.5.0-py38h885162f_1.conda#0eec8a20a17f17ec9e0b6839be466866
+https://conda.anaconda.org/conda-forge/linux-64/pillow-10.0.0-py38h885162f_0.conda#777c54134d5422a867aed7084cf5db5e
 https://conda.anaconda.org/eradiate/noarch/pinttrs-23.2.0-py_0.tar.bz2#1aebe9fa813278f719fa8e31d8000452
 https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
 https://conda.anaconda.org/conda-forge/noarch/portion-2.4.0-pyhd8ed1ab_0.conda#9d34bac22e169b41f4e34525a140c13b
 https://conda.anaconda.org/conda-forge/linux-64/pulseaudio-client-16.1-hb77b528_4.conda#8f349ca16d30950aa00870484d9d30c4
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
 https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml-0.17.32-py38h01eb140_0.conda#c92cc8efb1341f90ea5f51f576480580
 https://conda.anaconda.org/conda-forge/linux-64/sip-6.7.9-py38h17151c0_0.conda#6a54fd42b71a8b1c5f9c4a691270cdf1
 https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
 https://conda.anaconda.org/conda-forge/noarch/tqdm-4.65.0-pyhd8ed1ab_1.conda#ed792aff3acb977d09c7013358097f83
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.3-hd8ed1ab_0.conda#3876f650ed7d0f95d70fa4b647621909
-https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.3-pyhd8ed1ab_0.conda#ae465d0fbf9f1979cb2d8d4043d885e2
-https://conda.anaconda.org/conda-forge/linux-64/gstreamer-1.22.3-h977cf35_1.conda#410ed3b168e5a139d12ebaf4143072cd
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.0-hd8ed1ab_0.conda#37761dccc7ca8eaa08c60c4f62eb2dcc
+https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.3-pyhd8ed1ab_1.conda#89efeecbb24c62e2f1ed0b8ca959ec69
+https://repo.anaconda.com/pkgs/main/linux-64/gstreamer-1.22.3-h5eee18b_0.conda#c2ffbb79cb2f51b042de223d482b7b29
 https://conda.anaconda.org/conda-forge/linux-64/harfbuzz-7.3.0-hdb3a94d_0.conda#765bc76c0dfaf24ff9d8a2935b2510df
 https://conda.anaconda.org/conda-forge/noarch/importlib-resources-5.12.0-pyhd8ed1ab_0.conda#3544c818f0720c89eb16ae6940ab440b
 https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.7.0-hd8ed1ab_0.conda#27a4cec373ec84d1c1aa02a1e37f8eaf
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
-https://conda.anaconda.org/conda-forge/linux-64/libnetcdf-4.9.2-nompi_h0f3d0bb_105.conda#b5d412441b84305460e9df8a016a3392
+https://conda.anaconda.org/conda-forge/linux-64/libnetcdf-4.9.2-nompi_h78c856c_106.conda#47665bf3dec451455474556ecd940ed2
 https://conda.anaconda.org/conda-forge/noarch/mdit-py-plugins-0.4.0-pyhd8ed1ab_0.conda#6c5358a10873a15398b6f15f60cb5e1f
 https://conda.anaconda.org/conda-forge/linux-64/pandas-1.5.3-py38hdc8b05c_1.conda#c944b033a2126e7f714a7ecaecb22011
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.6.0-pyhd8ed1ab_0.conda#741384b21c1b512617f4ee4ea8457c5d
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.8.0-pyhd8ed1ab_0.conda#3e4aca765371893ad848397794600632
 https://conda.anaconda.org/conda-forge/noarch/pybtex-0.24.0-pyhd8ed1ab_2.tar.bz2#2099b86a7399c44c0c61cdb6de6915ba
 https://conda.anaconda.org/conda-forge/linux-64/pyqt5-sip-12.11.0-py38h8dc9893_3.conda#7bb0328b4a0f857aeb432426b9a5f908
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/noarch/rich-13.4.2-pyhd8ed1ab_0.conda#f993baacc175e83fafd6b846e9c4c8a2
-https://conda.anaconda.org/conda-forge/linux-64/gst-plugins-base-1.22.3-h938bd60_1.conda#1f317eb7f00db75f4112a07476345376
-https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.2.0-pyhd8ed1ab_0.conda#58ca2d50c3b27b86fd7df62eaadbf9a9
+https://repo.anaconda.com/pkgs/main/linux-64/gst-plugins-base-1.22.3-he621ea3_0.conda#27be67671dce7d6d8c53bf6260090c15
+https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda#1d018ee4ab13217e2544f795eb0a6798
 https://conda.anaconda.org/conda-forge/linux-64/matplotlib-base-3.7.1-py38hd6c3c57_0.conda#3b8ba76acae09fbd4b2247c4ee4c0324
 https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.0-pyhd8ed1ab_0.conda#f525a01528c3eba1d381a232a6971c6a
-https://conda.anaconda.org/conda-forge/linux-64/netcdf4-1.6.4-nompi_py38hdfa7aa7_100.conda#ce30178fb90d4509c3fda5b572124200
+https://conda.anaconda.org/conda-forge/linux-64/netcdf4-1.6.4-nompi_py38h383a0a3_101.conda#693cbd2ee4f62c8a2521cfaf7560b647
 https://conda.anaconda.org/conda-forge/noarch/pooch-1.7.0-pyha770c72_3.conda#5936894aade8240c867d292aa0d980c6
 https://conda.anaconda.org/conda-forge/linux-64/pybtex-docutils-1.0.2-py38h578d9bd_2.tar.bz2#178c840a19be1a4c809798a73b285d27
 https://conda.anaconda.org/conda-forge/noarch/sphinx-5.0.0-pyh6c4a22f_1.tar.bz2#a7cc4b9c94548ff9a19b368f975e5404
 https://conda.anaconda.org/conda-forge/noarch/typer-0.9.0-pyhd8ed1ab_0.conda#5030a13b2fe5e143d5956d4943d3018f
 https://conda.anaconda.org/conda-forge/noarch/xarray-2023.1.0-pyhd8ed1ab_0.conda#c11eb03b6f77a0d22ae88c454c940f55
 https://conda.anaconda.org/conda-forge/noarch/autodocsumm-0.2.11-pyhd8ed1ab_0.conda#547c48372c97c463c93af86d7f2c868c
 https://conda.anaconda.org/conda-forge/noarch/myst-parser-0.18.1-pyhd8ed1ab_0.tar.bz2#bcfdf5c7d8bf5c6f6be7b4c66fff2eca
```

### Comparing `eradiate-0.23.2rc3/requirements/conda/environment-docs-osx-64.lock` & `eradiate-0.23.2rc4/requirements/conda/environment-recommended-linux-64.lock`

 * *Files 7% similar despite different names*

```diff
@@ -1,179 +1,177 @@
 # Generated by conda-lock.
-# platform: osx-64
-# input_hash: c2b53750c00ef3f7883c4e6ca8543b71d05b09d221763358420b323fa23bf813
+# platform: linux-64
+# input_hash: 154be24de6d10a5d1c1f6776afadc7341a16933e3aa9188c627bd36c248b0a33
 @EXPLICIT
-https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h0d85af4_4.tar.bz2#37edc4e6304ca87316e160f5ca0bd1b5
-https://conda.anaconda.org/conda-forge/osx-64/c-ares-1.19.1-h0dc2134_0.conda#b3e62631b4e1b9801477523ce1d6f355
-https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2023.5.7-h8857fd0_0.conda#b704e4b79ba0d887c4870b7b09d6a4df
-https://conda.anaconda.org/conda-forge/osx-64/icu-72.1-h7336db1_0.conda#c9689510a50a4bb2ae978421671a125e
-https://conda.anaconda.org/conda-forge/osx-64/libbrotlicommon-1.0.9-hb7f2c08_8.tar.bz2#37157d273eaf3bc7d6862104161d9ec9
-https://conda.anaconda.org/conda-forge/osx-64/libcxx-16.0.6-hd57cbcb_0.conda#7d6972792161077908b62971802f289a
-https://conda.anaconda.org/conda-forge/osx-64/libdeflate-1.18-hac1461d_0.conda#3d131584456b277ce0871e6481fde49b
-https://conda.anaconda.org/conda-forge/osx-64/libev-4.33-haf1e3a3_1.tar.bz2#79dc2be110b2a3d1e97ec21f691c50ad
-https://conda.anaconda.org/conda-forge/osx-64/libffi-3.4.2-h0d85af4_5.tar.bz2#ccb34fb14960ad8b125962d3d79b31a9
-https://conda.anaconda.org/conda-forge/osx-64/libiconv-1.17-hac89ed1_0.tar.bz2#691d103d11180486154af49c037b7ed9
-https://conda.anaconda.org/conda-forge/osx-64/libjpeg-turbo-2.1.5.1-hb7f2c08_0.conda#d7309a152b9b79799063b8bb47e34a3a
-https://conda.anaconda.org/conda-forge/osx-64/libsodium-1.0.18-hbcb3906_1.tar.bz2#24632c09ed931af617fe6d5292919cab
-https://conda.anaconda.org/conda-forge/osx-64/libwebp-base-1.3.0-hb7f2c08_0.conda#18981e4c840126d6118d8952485fea51
-https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-h8a1eda9_5.conda#4a3ad23f6e16f99c04e166767193d700
-https://conda.anaconda.org/conda-forge/osx-64/llvm-openmp-16.0.6-hff08bdf_0.conda#39a5227d906f75102bf8586741690128
-https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.4-hf0c8a7f_0.conda#c3dbae2411164d9b02c69090a9a91857
-https://conda.anaconda.org/conda-forge/osx-64/pthread-stubs-0.4-hc929b4f_1001.tar.bz2#addd19059de62181cd11ae8f4ef26084
-https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.8-3_cp38.conda#ff192f59f7fe23555612030493a079f8
-https://conda.anaconda.org/conda-forge/osx-64/xorg-libxau-1.0.11-h0dc2134_0.conda#9566b4c29274125b0266d0177b5eb97b
-https://conda.anaconda.org/conda-forge/osx-64/xorg-libxdmcp-1.1.3-h35c211d_0.tar.bz2#86ac76d6bf1cbb9621943eb3bd9ae36e
-https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2#a72f9d4ea13d55d745ff1ed594747f10
-https://conda.anaconda.org/conda-forge/osx-64/yaml-0.2.5-h0d85af4_2.tar.bz2#d7e08fcf8259d742156188e8762b4d20
-https://conda.anaconda.org/conda-forge/osx-64/hdf4-4.2.15-h9804679_6.conda#c13d8841112ba7f5931d1d60631394f3
-https://conda.anaconda.org/conda-forge/osx-64/lerc-4.0.0-hb486fe8_0.tar.bz2#f9d6a4c82889d5ecedec1d90eb673c55
-https://conda.anaconda.org/conda-forge/osx-64/libaec-1.0.6-hf0c8a7f_1.conda#7c0f82f435ab4c48d65dc9b28db2ad9e
-https://conda.anaconda.org/conda-forge/osx-64/libbrotlidec-1.0.9-hb7f2c08_8.tar.bz2#7f952a036d9014b4dab96c6ea0f8c2a7
-https://conda.anaconda.org/conda-forge/osx-64/libbrotlienc-1.0.9-hb7f2c08_8.tar.bz2#b36a3bfe866d9127f25f286506982166
-https://conda.anaconda.org/conda-forge/osx-64/libedit-3.1.20191231-h0678c8f_2.tar.bz2#6016a8a1d0e63cac3de2c352cd40208b
-https://conda.anaconda.org/conda-forge/osx-64/libgfortran5-12.2.0-he409387_31.conda#5a544130e584b1f204ac896ff071d5b3
-https://conda.anaconda.org/conda-forge/osx-64/libpng-1.6.39-ha978bb4_0.conda#35e4928794c5391aec14ffdf1deaaee5
-https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.42.0-h58db7d2_0.conda#a7d3b44b7b0c9901ac7813b7a0462893
-https://conda.anaconda.org/conda-forge/osx-64/libxcb-1.15-hb7f2c08_0.conda#5513f57e0238c87c12dffedbcc9c1a4a
-https://conda.anaconda.org/conda-forge/osx-64/libxml2-2.11.4-hd95e348_0.conda#681f8dda25e73a830d774a37b9839c85
-https://conda.anaconda.org/conda-forge/osx-64/lz4-c-1.9.4-hf0c8a7f_0.conda#aa04f7143228308662696ac24023f991
-https://conda.anaconda.org/conda-forge/osx-64/openssl-3.1.1-h8a1eda9_1.conda#c7822d6ee74e34af1fd74365cfd18983
-https://conda.anaconda.org/conda-forge/osx-64/pandoc-3.1.3-h9d075a6_0.conda#e86a3d5c966a09b6129354114483f7a7
-https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda#f17f77f2acf4d344734bda76829ce14e
-https://conda.anaconda.org/conda-forge/osx-64/snappy-1.1.10-h225ccf5_0.conda#4320a8781f14cd959689b86e349f3b73
-https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.12-h5dbffcc_0.tar.bz2#8e9480d9c47061db2ed1b4ecce519a7f
-https://conda.anaconda.org/conda-forge/osx-64/zeromq-4.3.4-he49afe7_1.tar.bz2#1972d732b123ed04b60fd21e94f0b178
-https://conda.anaconda.org/conda-forge/osx-64/zstd-1.5.2-hbc0c0cd_6.conda#40a188783d3c425bdccc9ae9104acbb8
-https://conda.anaconda.org/conda-forge/osx-64/blosc-1.21.4-heccf04b_0.conda#02e92eb72b9ae4c1745b95d03a9c949e
-https://conda.anaconda.org/conda-forge/osx-64/brotli-bin-1.0.9-hb7f2c08_8.tar.bz2#aac5ad0d8f747ef7f871508146df75d9
-https://conda.anaconda.org/conda-forge/osx-64/freetype-2.12.1-h3f81eb7_1.conda#852224ea3e8991a8342228eab274840e
-https://conda.anaconda.org/conda-forge/osx-64/krb5-1.20.1-h049b76e_0.conda#db11fa2968ef0837288fe2d7f5b77a50
-https://conda.anaconda.org/conda-forge/osx-64/libgfortran-5.0.0-11_3_0_h97931a8_31.conda#97451338600bd9c5b535eb224ef6c471
-https://conda.anaconda.org/conda-forge/osx-64/libnghttp2-1.52.0-he2ab024_0.conda#12ac7d100bf260263e30a019517f42a2
-https://conda.anaconda.org/conda-forge/osx-64/libssh2-1.11.0-hd019ec5_0.conda#ca3a72efba692c59a90d4b9fc0dfe774
-https://conda.anaconda.org/conda-forge/osx-64/libtiff-4.5.1-hf955e92_0.conda#56523ed556e3a44c0fd55bcf17045892
-https://conda.anaconda.org/conda-forge/osx-64/libzip-1.9.2-h6db710c_1.tar.bz2#ce732d37e479919f3d22b1ccdeb858ac
-https://conda.anaconda.org/conda-forge/osx-64/python-3.8.17-hf9b03c3_0_cpython.conda#f613b663d3829f325b4ffb626bf612b6
-https://conda.anaconda.org/conda-forge/noarch/aenum-3.1.12-pyhd8ed1ab_0.conda#602716538da00b2ca3cc85c4d35c0245
-https://conda.anaconda.org/conda-forge/noarch/alabaster-0.7.13-pyhd8ed1ab_0.conda#06006184e203b61d3525f90de394471e
+https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2#d7c89558ba9fa0495403155b64376d81
+https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2023.5.7-hbcca054_0.conda#f5c65075fc34438d5b456c7f3f5ab695
+https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h41732ed_0.conda#7aca3059a1729aa76c597603f10b0dd3
+https://conda.anaconda.org/conda-forge/linux-64/libgfortran5-13.1.0-h15d22d2_0.conda#afb656a334c409dd9805508af1c89c7a
+https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.1.0-hfd8a6a1_0.conda#067bcc23164642f4c226da631f2a2e1d
+https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.11-3_cp311.conda#c2e2630ddb68cf52eec74dc7dfab20b5
+https://conda.anaconda.org/conda-forge/noarch/tzdata-2023c-h71feb2d_0.conda#939e3e74d8be4dac89ce83b20de2492a
+https://conda.anaconda.org/conda-forge/linux-64/libgfortran-ng-13.1.0-h69a702a_0.conda#506dc07710dd5b0ba63cbf134897fc10
+https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.1.0-he5830b7_0.conda#56ca14d57ac29a75d23a39eb3ee0ddeb
+https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2#73aaf86a425cc6e73fcf236a5a46396d
+https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.1.0-he5830b7_0.conda#cd93f779ff018dd85c7544c015c9db3c
+https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-h7f98852_4.tar.bz2#a1fd65c7ccbf10880423d82bca54eb54
+https://conda.anaconda.org/conda-forge/linux-64/lerc-4.0.0-h27087fc_0.tar.bz2#76bbff344f0134279f225174e9064c8f
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlicommon-1.0.9-h166bdaf_9.conda#61641e239f96eae2b8492dc7e755828c
+https://conda.anaconda.org/conda-forge/linux-64/libdeflate-1.18-h0b41bf4_0.conda#6aa9c9de5542ecb07fdda9ca626252d8
+https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.5.0-hcb278e6_1.conda#6305a3dd2752c76335295da4e581f2fd
+https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2#d645c6d2ac96843a2bfaccd2d62b3ac3
+https://conda.anaconda.org/conda-forge/linux-64/libjpeg-turbo-2.1.5.1-h0b41bf4_0.conda#1edd9e67bdb90d78cea97733ff6b54e6
+https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.0-h7f98852_0.tar.bz2#39b1328babf85c7c3a61636d9cd50206
+https://conda.anaconda.org/conda-forge/linux-64/libopenblas-0.3.23-pthreads_h80387f5_0.conda#9c5ea51ccb8ffae7d06c645869d24ce6
+https://conda.anaconda.org/conda-forge/linux-64/libsodium-1.0.18-h36c2ea0_1.tar.bz2#c3788462a6fbddafdb413a9f9053e58d
+https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda#40b61aab5c7ba9ff276c41cfffe6b80b
+https://conda.anaconda.org/conda-forge/linux-64/libwebp-base-1.3.1-hd590300_0.conda#82bf6f63eb15ef719b556b63feec3a77
+https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-hd590300_5.conda#f36c115f1ee199da648e0597ec2047ad
+https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.4-hcb278e6_0.conda#681105bccc2a3f7f1a837d47d39c9179
+https://conda.anaconda.org/conda-forge/linux-64/openssl-3.1.1-hd590300_1.conda#2e1d7b458ac8f1e3ca4e18b77add6277
+https://conda.anaconda.org/conda-forge/linux-64/pthread-stubs-0.4-h36c2ea0_1001.tar.bz2#22dad4df6e8630e8dff2428f6f6a7036
+https://conda.anaconda.org/conda-forge/linux-64/xorg-libxau-1.0.11-hd590300_0.conda#2c80dc38fface310c9bd81b17037fee5
+https://conda.anaconda.org/conda-forge/linux-64/xorg-libxdmcp-1.1.3-h7f98852_0.tar.bz2#be93aabceefa2fac576e971aef407908
+https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2#2161070d867d1b1204ea749c8eec4ef0
+https://conda.anaconda.org/conda-forge/linux-64/yaml-0.2.5-h7f98852_2.tar.bz2#4cb3ad778ec2d5a7acbdf254eb1c42ae
+https://conda.anaconda.org/conda-forge/linux-64/libblas-3.9.0-17_linux64_openblas.conda#57fb44770b1bc832fb2dbefa1bd502de
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlidec-1.0.9-h166bdaf_9.conda#081aa22f4581c08e4372b0b6c2f8478e
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlienc-1.0.9-h166bdaf_9.conda#1f0a03af852a9659ed2bf08f2f1704fd
+https://conda.anaconda.org/conda-forge/linux-64/libpng-1.6.39-h753d276_0.conda#e1c890aebdebbfbf87e2c917187b4416
+https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.42.0-h2797004_0.conda#fdaae20a1cf7cd62130a0973190a31b7
+https://conda.anaconda.org/conda-forge/linux-64/libxcb-1.15-h0b41bf4_0.conda#33277193f5b92bad9fdd230eb700929c
+https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda#47d31b792659ce70f470b5c82fdfb7a4
+https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.12-h27826a3_0.tar.bz2#5b8c42eb62e9fc961af70bdd6a26e168
+https://conda.anaconda.org/conda-forge/linux-64/zeromq-4.3.4-h9c3ff4c_1.tar.bz2#21743a8d2ea0c8cfbbf8fe489b0347df
+https://conda.anaconda.org/conda-forge/linux-64/zstd-1.5.2-h3eb15da_6.conda#6b63daed8feeca47be78f323e793d555
+https://conda.anaconda.org/conda-forge/linux-64/brotli-bin-1.0.9-h166bdaf_9.conda#d47dee1856d9cb955b8076eeff304a5b
+https://conda.anaconda.org/conda-forge/linux-64/freetype-2.12.1-hca18f0e_1.conda#e1232042de76d24539a436d37597eb06
+https://conda.anaconda.org/conda-forge/linux-64/libcblas-3.9.0-17_linux64_openblas.conda#7ef0969b00fe3d6eef56a8151d3afb29
+https://conda.anaconda.org/conda-forge/linux-64/liblapack-3.9.0-17_linux64_openblas.conda#a2103882c46492e26500fcb56c03de8b
+https://conda.anaconda.org/conda-forge/linux-64/libtiff-4.5.1-h8b53f26_0.conda#8ad377fb60abab446a9f02c62b3c2190
+https://conda.anaconda.org/conda-forge/linux-64/python-3.11.4-hab00c5b_0_cpython.conda#1c628861a2a126b9fc9363ca1b7d014e
+https://conda.anaconda.org/eradiate/noarch/aabbtree-2.8.0-py_0.tar.bz2#647bcce5f0af4974e507591d5420486b
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
-https://conda.anaconda.org/conda-forge/osx-64/brotli-1.0.9-hb7f2c08_8.tar.bz2#55f612fe4a9b5f6ac76348b6de94aaeb
+https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
+https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
+https://conda.anaconda.org/conda-forge/linux-64/brotli-1.0.9-h166bdaf_9.conda#4601544b4982ba1861fa9b9c607b2c06
+https://conda.anaconda.org/conda-forge/linux-64/brotli-python-1.0.9-py311ha362b79_9.conda#ced5340f5dc6cff43a80deac8d0e398f
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
-https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-unix_pyhd8ed1ab_2.tar.bz2#20e4087407c7cb04a40817114b333dbf
-https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/noarch/cycler-0.11.0-pyhd8ed1ab_0.tar.bz2#a50559fad0affdbb33729a68669ca1cb
-https://conda.anaconda.org/conda-forge/noarch/dataclasses-0.8-pyhc8e2a94_3.tar.bz2#a362b2124b06aad102e2ee4581acee7d
+https://conda.anaconda.org/conda-forge/linux-64/debugpy-1.6.7-py311hcafe171_0.conda#f4c810ad9d791c8df5ad900ed74b085b
+https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
-https://conda.anaconda.org/conda-forge/osx-64/docutils-0.16-py38h50d1736_3.tar.bz2#935f17c6604af240ea1c31c1d3292293
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
+https://conda.anaconda.org/conda-forge/noarch/executing-1.2.0-pyhd8ed1ab_0.tar.bz2#4c1bc140e2be5c8ba6e3acab99e25c50
+https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
-https://conda.anaconda.org/conda-forge/noarch/imagesize-1.4.1-pyhd8ed1ab_0.tar.bz2#7de5386c8fea29e76b303f37dde4c352
-https://conda.anaconda.org/conda-forge/osx-64/kiwisolver-1.4.4-py38h98b9b1b_1.tar.bz2#c11eff21a36bc5809b8e23a05ee71df8
-https://conda.anaconda.org/conda-forge/noarch/lazy_loader-0.2-pyhd8ed1ab_0.conda#d060d017720c9882c4eca0544a4a0592
-https://conda.anaconda.org/conda-forge/osx-64/lcms2-2.15-h2dcdeff_1.conda#f1df9b0c2d9fbe985e62f4b24773a9e4
-https://conda.anaconda.org/conda-forge/osx-64/libcurl-8.1.2-hbee3ae8_0.conda#d51e337da844262f9033c9a26452520f
-https://conda.anaconda.org/conda-forge/osx-64/libopenblas-0.3.23-openmp_h429af6e_0.conda#7000a828e29608e4f57e662b5502d2c9
-https://conda.anaconda.org/conda-forge/osx-64/markupsafe-2.1.3-py38hcafd530_0.conda#e8ee9933dc3749c889baccb1c4b4f014
-https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.0-pyhd8ed1ab_0.tar.bz2#f8dab71fdc13b1bf29a01248b156d268
+https://conda.anaconda.org/conda-forge/noarch/json5-0.9.14-pyhd8ed1ab_0.conda#dac1dabba2b5a9d1aee175c5fcc7b436
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.7-pyhd8ed1ab_1.conda#0c0a54e16b764bafcae35913cc9d60ff
+https://conda.anaconda.org/conda-forge/linux-64/kiwisolver-1.4.4-py311h4dd048b_1.tar.bz2#46d451f575392c01dc193069bd89766d
+https://conda.anaconda.org/conda-forge/linux-64/lcms2-2.15-haa2dc70_1.conda#980d8aca0bc23ca73fa8caa3e7c84c28
+https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.3-py311h459d7ec_0.conda#9904dc4adb5d547cb21e136f98cb24b0
 https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.0-pyhd8ed1ab_0.conda#c7d0ea64c37752ecbe6da458aee662d2
 https://conda.anaconda.org/conda-forge/noarch/munkres-1.1.4-pyh9f0ad1d_0.tar.bz2#2ba8498c1018c1e9c61eb99b973dfe19
-https://conda.anaconda.org/conda-forge/osx-64/openjpeg-2.5.0-h13ac156_2.conda#299a29af9ac9f550ad459d655739280b
+https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.5.6-pyhd8ed1ab_0.tar.bz2#7b868f21adde0d9b8b38f9c16836589b
+https://conda.anaconda.org/conda-forge/linux-64/numpy-1.25.0-py311h64a7726_0.conda#4df60430eca64502eb01e02df92246bf
+https://conda.anaconda.org/conda-forge/linux-64/openjpeg-2.5.0-hfec8fc6_2.conda#5ce6a42505c6e9e6151c54c3ec8d68ea
 https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
-https://conda.anaconda.org/conda-forge/noarch/pint-0.21-pyhd8ed1ab_0.conda#8d7b829e37d78447569c180f9d827005
+https://conda.anaconda.org/conda-forge/noarch/parso-0.8.3-pyhd8ed1ab_0.tar.bz2#17a565a0c3899244e938cdf417e7b094
+https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2#89e3c7cdde7d3aaa2aee933b604dd07f
+https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.0-pyhd8ed1ab_0.conda#95c5be3c7cbd872509d16c216617fdab
+https://conda.anaconda.org/conda-forge/linux-64/psutil-5.9.5-py311h2582759_0.conda#a90f8e278c1cd7064b2713e6b7db87e6
+https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2#359eeb6536da0e687af562ed265ec263
+https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2#6784285c7e55cb7212efabc79e4c2883
+https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
 https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.1.0-pyhd8ed1ab_0.conda#d3ed087d1f7f8f5590e8e87b57a8ce64
-https://conda.anaconda.org/conda-forge/osx-64/pyrsistent-0.19.3-py38hef030d1_0.conda#01ca11f08679d88fc881a19902a0a008
+https://conda.anaconda.org/conda-forge/linux-64/pyrsistent-0.19.3-py311h2582759_0.conda#e53876b66dcc4ba8a0afa63cd8502ac3
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
 https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.17.1-pyhd8ed1ab_0.conda#dd4f393d857e9283eef2442234bd05e3
+https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.7-pyhd8ed1ab_0.conda#a61bf9ec79426938ff785eb69dbb1960
+https://conda.anaconda.org/conda-forge/noarch/python-tzdata-2023.3-pyhd8ed1ab_0.conda#2590495f608a63625e165915fb4e2e34
 https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
-https://conda.anaconda.org/conda-forge/osx-64/pyyaml-6.0-py38hef030d1_5.tar.bz2#e27d698dc29c6d5b49f1385bcd1d50f9
-https://conda.anaconda.org/conda-forge/osx-64/pyzmq-25.1.0-py38h3b70857_0.conda#a48761bc98b3bc22d209e9bb2f3dc5c1
-https://conda.anaconda.org/conda-forge/osx-64/ruamel.yaml.clib-0.2.7-py38hef030d1_1.conda#9a8e866b0680b61b2e988b18a1eaecae
-https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda#3b68bc43ec6baa48f7354a446267eefe
-https://conda.anaconda.org/conda-forge/noarch/shellingham-1.4.0-pyh44b312d_0.tar.bz2#437655338696f9d0dfdb0a024e66b255
+https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0-py311hd4cff14_5.tar.bz2#da8769492e423103c59f469f4f17f8d9
+https://conda.anaconda.org/conda-forge/linux-64/pyzmq-25.1.0-py311h75c88c4_0.conda#db94a7a9e865fbfde8c023b6e8958bb2
+https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2#912a71cc01012ee38e6b90ddd561e36f
+https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyh41d4057_0.conda#ada5a17adcd10be4fc7e37e4166ba0e2
+https://conda.anaconda.org/conda-forge/noarch/setuptools-68.0.0-pyhd8ed1ab_0.conda#5a7739d0f57ee64133c9d32e6507c46d
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
-https://conda.anaconda.org/conda-forge/noarch/snowballstemmer-2.2.0-pyhd8ed1ab_0.tar.bz2#4d22a9315e78c6827f806065957d566e
-https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
+https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
-https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-applehelp-1.0.4-pyhd8ed1ab_0.conda#5a31a7d564f551d0e6dff52fd8cb5b16
-https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-devhelp-1.0.2-py_0.tar.bz2#68e01cac9d38d0e717cd5c87bc3d2cc9
-https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-htmlhelp-2.0.1-pyhd8ed1ab_0.conda#6c8c4d6eb2325e59290ac6dbbeacd5f0
-https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-jsmath-1.0.1-py_0.tar.bz2#67cd9d9c0382d37479b4d306c369a2d4
-https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-qthelp-1.0.3-py_0.tar.bz2#d01180388e6d1838c3e1ad029590aa7a
-https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-serializinghtml-1.1.5-pyhd8ed1ab_2.tar.bz2#9ff55a0901cf952f05c654394de76bf7
-https://conda.anaconda.org/conda-forge/osx-64/tornado-6.3.2-py38hcafd530_0.conda#afefcf665a5049b030efb084a51e3935
+https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
+https://conda.anaconda.org/conda-forge/linux-64/tornado-6.3.2-py311h459d7ec_0.conda#12b1c374ee90a1aa11ea921858394dc8
 https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.3-pyha770c72_0.conda#4a3014a4d107d15475d106b751c4e352
-https://conda.anaconda.org/conda-forge/osx-64/unicodedata2-15.0.0-py38hef030d1_0.tar.bz2#51020c740c53f14657f6307b9eb23f85
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.0-pyha770c72_0.conda#c76ebd4731d3668ba16975a30ef19d0d
+https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
+https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda#c34d9325a609381a0b0e8a5b4f325147
 https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
+https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.7-pyhd8ed1ab_0.conda#bcc54b91a8ce88f60f538b87b409909e
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
-https://conda.anaconda.org/conda-forge/noarch/accessible-pygments-0.0.4-pyhd8ed1ab_0.conda#46a2e6e3dfa718ce3492018d5a110dd6
+https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.0-pyhd8ed1ab_1.conda#2b35a85d654a47aac8f34c1bb6de7142
+https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
+https://conda.anaconda.org/conda-forge/noarch/async-lru-2.0.2-pyhd8ed1ab_0.conda#41221f97a0c82e5a60b21716a3d7469c
 https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
+https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda#6b1b907661838a75d067a22f87996b2e
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
 https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda#d48b143d01385872a88ef8417e96c30e
-https://conda.anaconda.org/conda-forge/osx-64/curl-8.1.2-hbee3ae8_0.conda#6cc301a6c2ba26e29949818efdc133ca
-https://conda.anaconda.org/eradiate/noarch/dessinemoi-23.1.0-py_0.tar.bz2#490780e63e113a7dc444bd068e049bfe
-https://conda.anaconda.org/conda-forge/noarch/environ-config-22.1.0-pyhd8ed1ab_0.tar.bz2#a1103faffa0a877313c1fba776aa0fc0
-https://conda.anaconda.org/conda-forge/osx-64/fonttools-4.40.0-py38hcafd530_0.conda#b26b38c5f75e03e86cecf860ca9fb1cd
-https://conda.anaconda.org/conda-forge/osx-64/hdf5-1.14.0-nompi_hbf0aa07_103.conda#90f50d124606a4e62628823b614a2f4c
+https://conda.anaconda.org/conda-forge/linux-64/cffi-1.15.1-py311h409f033_3.conda#9025d0786dbbe4bc91fd8e85502decce
+https://conda.anaconda.org/conda-forge/noarch/comm-0.1.3-pyhd8ed1ab_0.conda#168ae0f82cdf7505048e81054c7354e4
+https://conda.anaconda.org/conda-forge/linux-64/contourpy-1.1.0-py311h9547e67_0.conda#daf3f23397ab2265d0cdfa339f3627ba
+https://conda.anaconda.org/conda-forge/linux-64/fonttools-4.40.0-py311h459d7ec_0.conda#b19f671a6b221f922cf871d71a71c0fa
 https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.7.0-pyha770c72_0.conda#ba3786c6846e46038fe60c785d46dc81
 https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
+https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.2.2-pyhd8ed1ab_0.tar.bz2#243f63592c8e449f40cd42eb5cf32f40
-https://conda.anaconda.org/conda-forge/noarch/latexcodec-2.0.1-pyh9f0ad1d_0.tar.bz2#8d67904973263afd2985ba56aa2d6bb4
-https://conda.anaconda.org/conda-forge/osx-64/libblas-3.9.0-17_osx64_openblas.conda#65299527582e2449b05d27fcf8352125
-https://conda.anaconda.org/conda-forge/noarch/livereload-2.6.3-pyh9f0ad1d_0.tar.bz2#b7190e3ec3eff52839434bf4698e2d62
-https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-2.2.0-pyhd8ed1ab_0.conda#b2928a6c6d52d7e3562b4a59c3214e3a
-https://conda.anaconda.org/conda-forge/osx-64/pillow-9.5.0-py38h16710f9_1.conda#c5bf174a033ef668679cc80918422515
-https://conda.anaconda.org/eradiate/noarch/pinttrs-23.2.0-py_0.tar.bz2#1aebe9fa813278f719fa8e31d8000452
+https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
+https://conda.anaconda.org/conda-forge/noarch/overrides-7.3.1-pyhd8ed1ab_0.tar.bz2#a5745ced46e69aa9754053ba061974ab
+https://conda.anaconda.org/conda-forge/noarch/pexpect-4.8.0-pyh1a96a4e_2.tar.bz2#330448ce4403cc74990ac07c555942a1
+https://conda.anaconda.org/conda-forge/linux-64/pillow-10.0.0-py311h0b84326_0.conda#4b24acdc1fbbae9da03147e7d2cf8c8a
 https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
-https://conda.anaconda.org/conda-forge/noarch/portion-2.4.0-pyhd8ed1ab_0.conda#9d34bac22e169b41f4e34525a140c13b
+https://conda.anaconda.org/conda-forge/linux-64/pyerfa-2.0.0.3-py311hcb2cf0a_0.conda#0a3b00610d438d129341e810f0ce053d
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
-https://conda.anaconda.org/conda-forge/osx-64/ruamel.yaml-0.17.32-py38hcafd530_0.conda#cb301e0b2b162330bc3b03fe51ea0d15
+https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
+https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.1-pyh41d4057_0.conda#3788984d535770cad699efaeb6cb3037
 https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
-https://conda.anaconda.org/conda-forge/noarch/tqdm-4.65.0-pyhd8ed1ab_1.conda#ed792aff3acb977d09c7013358097f83
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.3-hd8ed1ab_0.conda#3876f650ed7d0f95d70fa4b647621909
-https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.3-pyhd8ed1ab_0.conda#ae465d0fbf9f1979cb2d8d4043d885e2
-https://conda.anaconda.org/conda-forge/noarch/importlib-resources-5.12.0-pyhd8ed1ab_0.conda#3544c818f0720c89eb16ae6940ab440b
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.0-hd8ed1ab_0.conda#37761dccc7ca8eaa08c60c4f62eb2dcc
+https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.3-pyhd8ed1ab_1.conda#89efeecbb24c62e2f1ed0b8ca959ec69
+https://conda.anaconda.org/conda-forge/linux-64/argon2-cffi-bindings-21.2.0-py311hd4cff14_3.tar.bz2#5159e874f65ac382773d2b534a1d7b80
+https://conda.anaconda.org/conda-forge/linux-64/astropy-5.3-py311h1f0f07a_0.conda#9e745ec84b02bbe087debe6074413da0
 https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.7.0-hd8ed1ab_0.conda#27a4cec373ec84d1c1aa02a1e37f8eaf
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
-https://conda.anaconda.org/conda-forge/osx-64/libcblas-3.9.0-17_osx64_openblas.conda#380151ca00704172b242a63701b7bf8a
-https://conda.anaconda.org/conda-forge/osx-64/liblapack-3.9.0-17_osx64_openblas.conda#6ab83532872bf3659613638589dd10af
-https://conda.anaconda.org/conda-forge/osx-64/libnetcdf-4.9.2-nompi_hf077d52_105.conda#64d626e024a284777458e2b315e9eb56
-https://conda.anaconda.org/conda-forge/noarch/mdit-py-plugins-0.4.0-pyhd8ed1ab_0.conda#6c5358a10873a15398b6f15f60cb5e1f
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.6.0-pyhd8ed1ab_0.conda#741384b21c1b512617f4ee4ea8457c5d
-https://conda.anaconda.org/conda-forge/noarch/pybtex-0.24.0-pyhd8ed1ab_2.tar.bz2#2099b86a7399c44c0c61cdb6de6915ba
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.4.4-pyhd8ed1ab_1.conda#7c0965e1d4a0ee1529e8eaa03a78a5b3
+https://conda.anaconda.org/conda-forge/linux-64/matplotlib-base-3.7.1-py311h8597a09_0.conda#70c3b734ffe82c16b6d121aaa11929a8
+https://conda.anaconda.org/conda-forge/linux-64/pandas-2.0.3-py311h320fe9a_0.conda#c9308b00067b8aa10893cb020bc39627
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.8.0-pyhd8ed1ab_0.conda#3e4aca765371893ad848397794600632
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
-https://conda.anaconda.org/conda-forge/noarch/rich-13.4.2-pyhd8ed1ab_0.conda#f993baacc175e83fafd6b846e9c4c8a2
-https://conda.anaconda.org/conda-forge/osx-64/jupyter_core-5.3.1-py38h50d1736_0.conda#03a3619e222793567b29b5966c2a821d
-https://conda.anaconda.org/conda-forge/osx-64/numpy-1.24.3-py38h9a4a08f_0.conda#5ff64b8133dea66865fe1bd35fb1d6d6
+https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
+https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
+https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
+https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-5.3.1-py311h38be061_0.conda#0cf8259b01ede82c76007996f73f89ed
+https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
 https://conda.anaconda.org/conda-forge/noarch/pooch-1.7.0-pyha770c72_3.conda#5936894aade8240c867d292aa0d980c6
-https://conda.anaconda.org/conda-forge/osx-64/pybtex-docutils-1.0.2-py38h50d1736_2.tar.bz2#5650c819d7ae44ff91c456370f175706
-https://conda.anaconda.org/conda-forge/noarch/sphinx-5.0.0-pyh6c4a22f_1.tar.bz2#a7cc4b9c94548ff9a19b368f975e5404
-https://conda.anaconda.org/conda-forge/noarch/typer-0.9.0-pyhd8ed1ab_0.conda#5030a13b2fe5e143d5956d4943d3018f
-https://conda.anaconda.org/conda-forge/noarch/autodocsumm-0.2.11-pyhd8ed1ab_0.conda#547c48372c97c463c93af86d7f2c868c
-https://conda.anaconda.org/conda-forge/osx-64/cftime-1.6.2-py38hbd87e4b_1.tar.bz2#6b61efa56393b9655334192cc5423659
-https://conda.anaconda.org/conda-forge/osx-64/contourpy-1.1.0-py38h15a1a5b_0.conda#30d645ffb3572a3875e6fc8687857182
-https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.2.0-pyhd8ed1ab_0.conda#58ca2d50c3b27b86fd7df62eaadbf9a9
-https://conda.anaconda.org/conda-forge/noarch/myst-parser-0.18.1-pyhd8ed1ab_0.tar.bz2#bcfdf5c7d8bf5c6f6be7b4c66fff2eca
+https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
+https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda#1d018ee4ab13217e2544f795eb0a6798
 https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.0-pyhd8ed1ab_0.conda#f525a01528c3eba1d381a232a6971c6a
-https://conda.anaconda.org/conda-forge/osx-64/pandas-1.5.3-py38hec72209_1.conda#a8f001ab0a7c6312cea020bd20689765
-https://conda.anaconda.org/conda-forge/noarch/pydata-sphinx-theme-0.13.3-pyhd8ed1ab_0.conda#07aca5f2dea315dcc16680d6891e9056
-https://conda.anaconda.org/conda-forge/osx-64/scipy-1.10.1-py38h9cf86d3_3.conda#5e20c77455e815704b008ab8f42f6169
-https://conda.anaconda.org/conda-forge/noarch/sphinx-autobuild-2021.3.14-pyhd8ed1ab_0.tar.bz2#1909f784dc37b4ab97afe2c95aeeabaa
-https://conda.anaconda.org/conda-forge/noarch/sphinx-copybutton-0.5.2-pyhd8ed1ab_0.conda#ac832cc43adc79118cf6e23f1f9b8995
-https://conda.anaconda.org/conda-forge/noarch/sphinx-design-0.4.1-pyhd8ed1ab_1.conda#c6b2e7903121c3210462a0866a561993
-https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-bibtex-2.5.0-pyhd8ed1ab_0.tar.bz2#b2e5c9aece936ebf9f26abdf71ddd74b
-https://conda.anaconda.org/conda-forge/osx-64/matplotlib-base-3.7.1-py38hcb346ec_0.conda#1f1eea98c232c8ef720175e12b00d0c4
+https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.38-hd8ed1ab_0.conda#45b74f64d8808eda7e6f6e6b1d641fd2
+https://conda.anaconda.org/conda-forge/linux-64/scipy-1.11.1-py311h64a7726_0.conda#356da36102fc1eeb8a81e6d79e53bc7e
+https://conda.anaconda.org/conda-forge/noarch/iapws-1.5.3-pyhd8ed1ab_0.tar.bz2#c5cad28f7c667df1910c3e9f8213c5eb
+https://conda.anaconda.org/conda-forge/noarch/ipython-8.14.0-pyh41d4057_0.conda#0a0b0d8177c4a209017b356439292db8
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.8.0-pyhd8ed1ab_0.conda#e78da91cf428faaf05701ce8cc8f2f9b
-https://conda.anaconda.org/conda-forge/osx-64/netcdf4-1.6.4-nompi_py38h47ac6a0_100.conda#f86d4df9f8f46ae6d0c29bb87fe093b0
-https://conda.anaconda.org/conda-forge/noarch/sphinx-book-theme-1.0.1-pyhd8ed1ab_0.conda#1ef419576de2c51b6e3a5a393eb35cda
-https://conda.anaconda.org/conda-forge/noarch/xarray-2023.1.0-pyhd8ed1ab_0.conda#c11eb03b6f77a0d22ae88c454c940f55
-https://conda.anaconda.org/conda-forge/osx-64/matplotlib-3.7.1-py38h50d1736_0.conda#14bce132d8a4546246b131c4289b480f
+https://conda.anaconda.org/conda-forge/noarch/patsy-0.5.3-pyhd8ed1ab_0.tar.bz2#50ef6b29b1fb0768ca82c5aeb4fb2d96
+https://conda.anaconda.org/conda-forge/noarch/seaborn-base-0.12.2-pyhd8ed1ab_0.conda#cf88f3a1c11536bc3c10c14ad00ccc42
+https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.3-pyh71e2992_0.conda#482f0176a89f14e10a7d15f9f1980e36
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.6.0-pyhd8ed1ab_0.conda#879782bde4bbdb4c7b5d4054504a20d5
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.6.0-pyhd8ed1ab_0.conda#e8172ca42f2869bb90185c9356899e81
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.6.0-pyhd8ed1ab_0.conda#59976ee8df1c6f82c4aa94b5fd6b745e
-https://conda.anaconda.org/conda-forge/noarch/nbsphinx-0.9.2-pyhd8ed1ab_0.conda#d1212b423fdd10d2da59601385561ff7
+https://conda.anaconda.org/conda-forge/linux-64/statsmodels-0.14.0-py311h1f0f07a_1.conda#a1daa39fa0bfed4d91a3640c2274034a
+https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.6-pyhd8ed1ab_0.conda#68627a08556e4a273e4c7bfc84251457
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.7.0-pyhd8ed1ab_0.conda#7488cd1f4d35a2af96faa765b7e5b2f0
+https://conda.anaconda.org/conda-forge/noarch/seaborn-0.12.2-hd8ed1ab_0.conda#50847a47c07812f88581081c620f5160
+https://conda.anaconda.org/conda-forge/noarch/jupyter-lsp-2.2.0-pyhd8ed1ab_0.conda#38589f4104d11f2a59ff01a9f4e3bfb3
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.23.0-pyhd8ed1ab_0.conda#942aa06b962c7e507884c6fbeb4d1f7d
+https://conda.anaconda.org/conda-forge/noarch/notebook-shim-0.2.3-pyhd8ed1ab_0.conda#67e0fe74c156267d9159e9133df7fd37
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab-4.0.2-pyhd8ed1ab_0.conda#8e102bf37f10dd49c248910450242a19
```

### Comparing `eradiate-0.23.2rc3/requirements/conda/environment-docs.dot` & `eradiate-0.23.2rc4/requirements/conda/environment-docs.dot`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/requirements/conda/environment-docs.yml` & `eradiate-0.23.2rc4/requirements/conda/environment-docs.yml`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/requirements/conda/environment-main-linux-64.lock` & `eradiate-0.23.2rc4/requirements/conda/environment-main-linux-64.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Generated by conda-lock.
 # platform: linux-64
-# input_hash: 7978c39d039c87858107e33a8ec1a02d28c787cf6cb89fe0234d346f144c81b5
+# input_hash: 6dda966feaa106a4b9c32ba6874b70e59748f77d06acaa3ddb4b6ebf7a7dda44
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2#d7c89558ba9fa0495403155b64376d81
 https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2023.5.7-hbcca054_0.conda#f5c65075fc34438d5b456c7f3f5ab695
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-dejavu-sans-mono-2.37-hab24e00_0.tar.bz2#0c96522c6bdaed4b1566d11387caaf45
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-inconsolata-3.000-h77eed37_0.tar.bz2#34893075a5c9e55cdafac56607368fc6
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-source-code-pro-2.038-h77eed37_0.tar.bz2#4d59c254e01d9cde7957100457e2d5fb
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-ubuntu-0.83-hab24e00_0.tar.bz2#19410c3df09dfb12d1206132a1d357c5
@@ -25,27 +25,27 @@
 https://conda.anaconda.org/conda-forge/linux-64/gettext-0.21.1-h27087fc_0.tar.bz2#14947d8770185e5153fdd04d4673ed37
 https://conda.anaconda.org/conda-forge/linux-64/graphite2-1.3.13-h58526e2_1001.tar.bz2#8c54672728e8ec6aa6db90cf2806d220
 https://conda.anaconda.org/conda-forge/linux-64/icu-72.1-hcb278e6_0.conda#7c8d20d847bb45f56bd941578fcfa146
 https://conda.anaconda.org/conda-forge/linux-64/keyutils-1.6.1-h166bdaf_0.tar.bz2#30186d27e2c9fa62b45fb1476b7200e3
 https://conda.anaconda.org/conda-forge/linux-64/lame-3.100-h166bdaf_1003.tar.bz2#a8832b479f93521a9e7b5b743803be51
 https://conda.anaconda.org/conda-forge/linux-64/lerc-4.0.0-h27087fc_0.tar.bz2#76bbff344f0134279f225174e9064c8f
 https://conda.anaconda.org/conda-forge/linux-64/libaec-1.0.6-hcb278e6_1.conda#0f683578378cddb223e7fd24f785ab2a
-https://conda.anaconda.org/conda-forge/linux-64/libbrotlicommon-1.0.9-h166bdaf_8.tar.bz2#9194c9bf9428035a05352d031462eae4
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlicommon-1.0.9-h166bdaf_9.conda#61641e239f96eae2b8492dc7e755828c
 https://conda.anaconda.org/conda-forge/linux-64/libdeflate-1.18-h0b41bf4_0.conda#6aa9c9de5542ecb07fdda9ca626252d8
 https://conda.anaconda.org/conda-forge/linux-64/libev-4.33-h516909a_1.tar.bz2#6f8720dff19e17ce5d48cfe7f3d2f0a3
 https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.5.0-hcb278e6_1.conda#6305a3dd2752c76335295da4e581f2fd
 https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2#d645c6d2ac96843a2bfaccd2d62b3ac3
 https://conda.anaconda.org/conda-forge/linux-64/libiconv-1.17-h166bdaf_0.tar.bz2#b62b52da46c39ee2bc3c162ac7f1804d
 https://conda.anaconda.org/conda-forge/linux-64/libjpeg-turbo-2.1.5.1-h0b41bf4_0.conda#1edd9e67bdb90d78cea97733ff6b54e6
 https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.0-h7f98852_0.tar.bz2#39b1328babf85c7c3a61636d9cd50206
-https://conda.anaconda.org/conda-forge/linux-64/libogg-1.3.4-h7f98852_1.tar.bz2#6e8cc2173440d77708196c5b93771680
+https://repo.anaconda.com/pkgs/main/linux-64/libogg-1.3.5-h27cfd23_1.conda#710ee7fdb0ddf7591a5af7ca7eb4d73d
 https://conda.anaconda.org/conda-forge/linux-64/libopenblas-0.3.23-pthreads_h80387f5_0.conda#9c5ea51ccb8ffae7d06c645869d24ce6
 https://conda.anaconda.org/conda-forge/linux-64/libopus-1.3.1-h7f98852_1.tar.bz2#15345e56d527b330e1cacbdf58676e8f
 https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda#40b61aab5c7ba9ff276c41cfffe6b80b
-https://conda.anaconda.org/conda-forge/linux-64/libwebp-base-1.3.0-h0b41bf4_0.conda#0d4a7508d8c6c65314f2b9c1f56ad408
+https://conda.anaconda.org/conda-forge/linux-64/libwebp-base-1.3.1-hd590300_0.conda#82bf6f63eb15ef719b556b63feec3a77
 https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-hd590300_5.conda#f36c115f1ee199da648e0597ec2047ad
 https://conda.anaconda.org/conda-forge/linux-64/lz4-c-1.9.4-hcb278e6_0.conda#318b08df404f9c9be5712aaa5a6f0bb0
 https://conda.anaconda.org/conda-forge/linux-64/mpg123-1.31.3-hcb278e6_0.conda#141a126675b6d1a4eabb111a4a353898
 https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.4-hcb278e6_0.conda#681105bccc2a3f7f1a837d47d39c9179
 https://conda.anaconda.org/conda-forge/linux-64/nspr-4.35-h27087fc_0.conda#da0ec11a6454ae19bff5b02ed881a2b1
 https://conda.anaconda.org/conda-forge/linux-64/openssl-3.1.1-hd590300_1.conda#2e1d7b458ac8f1e3ca4e18b77add6277
 https://conda.anaconda.org/conda-forge/linux-64/pixman-0.40.0-h36c2ea0_0.tar.bz2#660e72c82f2e75a6b3fe6a6e75c79f19
@@ -59,58 +59,59 @@
 https://conda.anaconda.org/conda-forge/linux-64/xorg-xextproto-7.3.0-h0b41bf4_1003.conda#bce9f945da8ad2ae9b1d7165a64d0f87
 https://conda.anaconda.org/conda-forge/linux-64/xorg-xf86vidmodeproto-2.3.1-h7f98852_1002.tar.bz2#3ceea9668625c18f19530de98b15d5b0
 https://conda.anaconda.org/conda-forge/linux-64/xorg-xproto-7.0.31-h7f98852_1007.tar.bz2#b4a4381d54784606820704f7b5f05a15
 https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2#2161070d867d1b1204ea749c8eec4ef0
 https://conda.anaconda.org/conda-forge/linux-64/expat-2.5.0-hcb278e6_1.conda#8b9b5aca60558d02ddaa09d599e55920
 https://conda.anaconda.org/conda-forge/linux-64/hdf4-4.2.15-h501b40f_6.conda#c3e9338e15d90106f467377017352b97
 https://conda.anaconda.org/conda-forge/linux-64/libblas-3.9.0-17_linux64_openblas.conda#57fb44770b1bc832fb2dbefa1bd502de
-https://conda.anaconda.org/conda-forge/linux-64/libbrotlidec-1.0.9-h166bdaf_8.tar.bz2#4ae4d7795d33e02bd20f6b23d91caf82
-https://conda.anaconda.org/conda-forge/linux-64/libbrotlienc-1.0.9-h166bdaf_8.tar.bz2#04bac51ba35ea023dc48af73c1c88c25
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlidec-1.0.9-h166bdaf_9.conda#081aa22f4581c08e4372b0b6c2f8478e
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlienc-1.0.9-h166bdaf_9.conda#1f0a03af852a9659ed2bf08f2f1704fd
 https://conda.anaconda.org/conda-forge/linux-64/libcap-2.67-he9d0100_0.conda#d05556c80caffff164d17bdea0105a1a
 https://conda.anaconda.org/conda-forge/linux-64/libedit-3.1.20191231-he28a2e2_2.tar.bz2#4d331e44109e3f0e19b4cb8f9b82f3e1
 https://conda.anaconda.org/conda-forge/linux-64/libevent-2.1.12-hf998b51_1.conda#a1cfcc585f0c42bf8d5546bb1dfb668d
-https://conda.anaconda.org/conda-forge/linux-64/libflac-1.4.2-h27087fc_0.tar.bz2#7daf72d8e2a8e848e11d63ed6d1026e0
+https://conda.anaconda.org/conda-forge/linux-64/libflac-1.4.3-h59595ed_0.conda#ee48bf17cc83a00f59ca1494d5646869
 https://conda.anaconda.org/conda-forge/linux-64/libgpg-error-1.47-h71f35ed_0.conda#c2097d0b46367996f09b4e8e4920384a
 https://conda.anaconda.org/conda-forge/linux-64/libnghttp2-1.52.0-h61bc06f_0.conda#613955a50485812985c059e7b269f42e
 https://conda.anaconda.org/conda-forge/linux-64/libpng-1.6.39-h753d276_0.conda#e1c890aebdebbfbf87e2c917187b4416
 https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.42.0-h2797004_0.conda#fdaae20a1cf7cd62130a0973190a31b7
 https://conda.anaconda.org/conda-forge/linux-64/libssh2-1.11.0-h0841786_0.conda#1f5a58e686b13bcfde88b93f547d23fe
 https://conda.anaconda.org/conda-forge/linux-64/libvorbis-1.3.7-h9c3ff4c_0.tar.bz2#309dec04b70a3cc0f1e84a4013683bc0
 https://conda.anaconda.org/conda-forge/linux-64/libxcb-1.15-h0b41bf4_0.conda#33277193f5b92bad9fdd230eb700929c
 https://conda.anaconda.org/conda-forge/linux-64/libxml2-2.11.4-h0d562d8_0.conda#e46fad17d5fb57316b956f88dca765e4
 https://conda.anaconda.org/conda-forge/linux-64/libzip-1.9.2-hc929e4a_1.tar.bz2#5b122b50e738c4be5c3f2899f010d7cf
-https://conda.anaconda.org/conda-forge/linux-64/mysql-common-8.0.33-hf1915f5_0.conda#aa8b86066614c4573f6db62c91978fa9
+https://conda.anaconda.org/conda-forge/linux-64/mysql-common-8.0.33-hf1915f5_1.conda#b241363e3b72bae6dfbd31e9fecf7d26
 https://conda.anaconda.org/conda-forge/linux-64/pcre2-10.40-hc3806b6_0.tar.bz2#69e2c796349cd9b273890bee0febfe1b
 https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda#47d31b792659ce70f470b5c82fdfb7a4
 https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.12-h27826a3_0.tar.bz2#5b8c42eb62e9fc961af70bdd6a26e168
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libsm-1.2.4-h7391055_0.conda#93ee23f12bc2e684548181256edd2cf6
 https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.13-hd590300_5.conda#68c34ec6149623be41a1933ab996a209
 https://conda.anaconda.org/conda-forge/linux-64/zstd-1.5.2-h3eb15da_6.conda#6b63daed8feeca47be78f323e793d555
 https://conda.anaconda.org/conda-forge/linux-64/blosc-1.21.4-h0f2a231_0.conda#876286b5941933a0f558777e57d883cc
-https://conda.anaconda.org/conda-forge/linux-64/brotli-bin-1.0.9-h166bdaf_8.tar.bz2#e5613f2bc717e9945840ff474419b8e4
+https://conda.anaconda.org/conda-forge/linux-64/brotli-bin-1.0.9-h166bdaf_9.conda#d47dee1856d9cb955b8076eeff304a5b
 https://conda.anaconda.org/conda-forge/linux-64/freetype-2.12.1-hca18f0e_1.conda#e1232042de76d24539a436d37597eb06
 https://conda.anaconda.org/conda-forge/linux-64/krb5-1.20.1-h81ceb04_0.conda#89a41adce7106749573d883b2f657d78
 https://conda.anaconda.org/conda-forge/linux-64/libcblas-3.9.0-17_linux64_openblas.conda#7ef0969b00fe3d6eef56a8151d3afb29
 https://conda.anaconda.org/conda-forge/linux-64/libgcrypt-1.10.1-h166bdaf_0.tar.bz2#f967fc95089cd247ceed56eda31de3a9
 https://conda.anaconda.org/conda-forge/linux-64/libglib-2.76.3-hebfc3b9_0.conda#a64f11b244b2c112cd3fa1cbe9493999
 https://conda.anaconda.org/conda-forge/linux-64/liblapack-3.9.0-17_linux64_openblas.conda#a2103882c46492e26500fcb56c03de8b
 https://conda.anaconda.org/conda-forge/linux-64/libllvm16-16.0.6-h5cf9203_0.conda#753e078cccad40fe4b396bdcf27a3c15
 https://conda.anaconda.org/conda-forge/linux-64/libsndfile-1.2.0-hb75c966_0.conda#c648d19cd9c8625898d5d370414de7c7
 https://conda.anaconda.org/conda-forge/linux-64/libtiff-4.5.1-h8b53f26_0.conda#8ad377fb60abab446a9f02c62b3c2190
-https://conda.anaconda.org/conda-forge/linux-64/mysql-libs-8.0.33-hca2cd23_0.conda#276339b0115d92c6e0793dcdc7afe308
+https://conda.anaconda.org/conda-forge/linux-64/mysql-libs-8.0.33-hca2cd23_1.conda#a04ac37f0659929f3ba0f33c7f3d750f
 https://conda.anaconda.org/conda-forge/linux-64/nss-3.89-he45b914_0.conda#2745719a58eeaab6657256a3f142f099
 https://conda.anaconda.org/conda-forge/linux-64/python-3.8.17-he550d4f_0_cpython.conda#72d038de0a228e4f0ef4011940641293
 https://conda.anaconda.org/conda-forge/linux-64/xcb-util-0.4.0-hd590300_1.conda#9bfac7ccd94d54fd21a0501296d60424
 https://conda.anaconda.org/conda-forge/linux-64/xcb-util-keysyms-0.4.0-h8ee46fc_1.conda#632413adcd8bc16b515cab87a2932913
 https://conda.anaconda.org/conda-forge/linux-64/xcb-util-renderutil-0.3.9-hd590300_1.conda#e995b155d938b6779da6ace6c6b13816
 https://conda.anaconda.org/conda-forge/linux-64/xcb-util-wm-0.4.1-h8ee46fc_1.conda#90108a432fb5c6150ccfee3f03388656
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libx11-1.8.6-h8ee46fc_0.conda#7590b76c3d11d21caa44f3fc38ac584a
-https://conda.anaconda.org/conda-forge/noarch/aenum-3.1.12-pyhd8ed1ab_0.conda#602716538da00b2ca3cc85c4d35c0245
+https://conda.anaconda.org/conda-forge/noarch/aenum-3.1.15-pyhd8ed1ab_0.conda#24cff7ab050ebb8a16bdeb02e8ed6f63
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
-https://conda.anaconda.org/conda-forge/linux-64/brotli-1.0.9-h166bdaf_8.tar.bz2#2ff08978892a3e8b954397c461f18418
+https://conda.anaconda.org/conda-forge/linux-64/brotli-1.0.9-h166bdaf_9.conda#4601544b4982ba1861fa9b9c607b2c06
+https://conda.anaconda.org/conda-forge/linux-64/brotli-python-1.0.9-py38hfa26641_9.conda#d056745008e5ed73210a31dcfd4d183a
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
 https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-unix_pyhd8ed1ab_2.tar.bz2#20e4087407c7cb04a40817114b333dbf
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/noarch/cycler-0.11.0-pyhd8ed1ab_0.tar.bz2#a50559fad0affdbb33729a68669ca1cb
 https://conda.anaconda.org/conda-forge/linux-64/dbus-1.13.6-h5008d03_3.tar.bz2#ecfff944ba3960ecb334b9a2663d708d
 https://conda.anaconda.org/conda-forge/linux-64/fontconfig-2.14.2-h14ed4e7_0.conda#0f69b688f52ff6da70bccb7ff7001d1d
@@ -122,75 +123,75 @@
 https://conda.anaconda.org/conda-forge/linux-64/libclang13-16.0.6-default_h4d60ac6_0.conda#b10174a063ec195f8fe1b278282c3149
 https://conda.anaconda.org/conda-forge/linux-64/libcups-2.3.3-h36d4200_3.conda#c9f4416a34bc91e0eb029f912c68f81f
 https://conda.anaconda.org/conda-forge/linux-64/libcurl-8.1.2-h409715c_0.conda#50c873c9660ed116707ae15b663928d8
 https://conda.anaconda.org/conda-forge/linux-64/libpq-15.3-hbcd7760_1.conda#8afb2a97d256ffde95b91a6283bc598c
 https://conda.anaconda.org/conda-forge/linux-64/libsystemd0-253-h8c4010b_1.conda#9176b1e2cb8beca37a7510b0e801e38f
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.0-pyhd8ed1ab_0.tar.bz2#f8dab71fdc13b1bf29a01248b156d268
 https://conda.anaconda.org/conda-forge/noarch/munkres-1.1.4-pyh9f0ad1d_0.tar.bz2#2ba8498c1018c1e9c61eb99b973dfe19
-https://conda.anaconda.org/conda-forge/linux-64/numpy-1.24.3-py38h59b608b_0.conda#5836e4ab0399136ede58446a4776b2ff
+https://conda.anaconda.org/conda-forge/linux-64/numpy-1.24.4-py38h59b608b_0.conda#8c3e050afeeb2b32575bdb8955cc67b2
 https://conda.anaconda.org/conda-forge/linux-64/openjpeg-2.5.0-hfec8fc6_2.conda#5ce6a42505c6e9e6151c54c3ec8d68ea
 https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
 https://conda.anaconda.org/conda-forge/noarch/pint-0.21-pyhd8ed1ab_0.conda#8d7b829e37d78447569c180f9d827005
 https://conda.anaconda.org/conda-forge/noarch/ply-3.11-py_1.tar.bz2#7205635cd71531943440fbfe3b6b5727
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
 https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.1.0-pyhd8ed1ab_0.conda#d3ed087d1f7f8f5590e8e87b57a8ce64
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
 https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
 https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml.clib-0.2.7-py38h1de0b5d_1.conda#9afa2fc3c51cc4e7d1589c38e4e00d5c
-https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda#3b68bc43ec6baa48f7354a446267eefe
+https://conda.anaconda.org/conda-forge/noarch/setuptools-68.0.0-pyhd8ed1ab_0.conda#5a7739d0f57ee64133c9d32e6507c46d
 https://conda.anaconda.org/conda-forge/noarch/shellingham-1.4.0-pyh44b312d_0.tar.bz2#437655338696f9d0dfdb0a024e66b255
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/linux-64/tornado-6.3.2-py38h01eb140_0.conda#3db869202b0e523d606d13e81ca79ab6
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.3-pyha770c72_0.conda#4a3014a4d107d15475d106b751c4e352
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.0-pyha770c72_0.conda#c76ebd4731d3668ba16975a30ef19d0d
 https://conda.anaconda.org/conda-forge/linux-64/unicodedata2-15.0.0-py38h0a891b7_0.tar.bz2#44421904760e9f5ae2035193e04360f0
 https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
 https://conda.anaconda.org/conda-forge/linux-64/xcb-util-image-0.4.0-h8ee46fc_1.conda#9d7bcddf49cbf727730af10e71022c73
 https://conda.anaconda.org/conda-forge/linux-64/xkeyboard-config-2.39-hd590300_0.conda#d88c7fc8a11858fb14761832e4da1954
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxext-1.3.4-h0b41bf4_2.conda#82b6df12252e6f32402b96dacc656fec
-https://conda.anaconda.org/conda-forge/linux-64/xorg-libxrender-0.9.10-h7f98852_1003.tar.bz2#f59c1242cc1dd93e72c2ee2b360979eb
+https://conda.anaconda.org/conda-forge/linux-64/xorg-libxrender-0.9.11-hd590300_0.conda#ed67c36f215b310412b2af935bf3e530
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
 https://conda.anaconda.org/conda-forge/linux-64/cairo-1.16.0-hbbf8b49_1016.conda#c1dd96500b9b1a75e9e511931f415cbc
 https://conda.anaconda.org/conda-forge/linux-64/cftime-1.6.2-py38h26c90d9_1.tar.bz2#dcc025a7bb54374979c500c2e161fac9
 https://conda.anaconda.org/conda-forge/linux-64/contourpy-1.1.0-py38h7f3f72f_0.conda#0fdf3cc879156e0234e05962d55b6502
 https://conda.anaconda.org/conda-forge/linux-64/curl-8.1.2-h409715c_0.conda#9f88cfb15b7d08b25880b138f91e0eb4
 https://conda.anaconda.org/eradiate/noarch/dessinemoi-23.1.0-py_0.tar.bz2#490780e63e113a7dc444bd068e049bfe
 https://conda.anaconda.org/conda-forge/noarch/environ-config-22.1.0-pyhd8ed1ab_0.tar.bz2#a1103faffa0a877313c1fba776aa0fc0
 https://conda.anaconda.org/conda-forge/linux-64/fonttools-4.40.0-py38h01eb140_0.conda#f893b6bac56c477dd71498569b4a9022
 https://conda.anaconda.org/conda-forge/linux-64/glib-2.76.3-hfc55251_0.conda#950e02f5665f5f4ff0437a6acba58798
-https://conda.anaconda.org/conda-forge/linux-64/hdf5-1.14.0-nompi_hb72d44e_103.conda#975973a4350ab45ff1981fe535a12af5
+https://conda.anaconda.org/conda-forge/linux-64/hdf5-1.14.1-nompi_h4f84152_100.conda#ff9ae10aa224826c07da7ef26cb0b717
 https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
 https://conda.anaconda.org/conda-forge/linux-64/libclang-16.0.6-default_h1cdf331_0.conda#e976871e132fe506da52c1240229246a
 https://conda.anaconda.org/conda-forge/linux-64/libxkbcommon-1.5.0-h5d7e998_3.conda#c91ea308d7bf70b62ddda568478aa03b
 https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-3.0.0-pyhd8ed1ab_0.conda#93a8e71256479c62074356ef6ebf501b
-https://conda.anaconda.org/conda-forge/linux-64/pillow-9.5.0-py38h885162f_1.conda#0eec8a20a17f17ec9e0b6839be466866
+https://conda.anaconda.org/conda-forge/linux-64/pillow-10.0.0-py38h885162f_0.conda#777c54134d5422a867aed7084cf5db5e
 https://conda.anaconda.org/eradiate/noarch/pinttrs-23.2.0-py_0.tar.bz2#1aebe9fa813278f719fa8e31d8000452
 https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
 https://conda.anaconda.org/conda-forge/noarch/portion-2.4.0-pyhd8ed1ab_0.conda#9d34bac22e169b41f4e34525a140c13b
 https://conda.anaconda.org/conda-forge/linux-64/pulseaudio-client-16.1-hb77b528_4.conda#8f349ca16d30950aa00870484d9d30c4
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
 https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml-0.17.32-py38h01eb140_0.conda#c92cc8efb1341f90ea5f51f576480580
 https://conda.anaconda.org/conda-forge/linux-64/sip-6.7.9-py38h17151c0_0.conda#6a54fd42b71a8b1c5f9c4a691270cdf1
 https://conda.anaconda.org/conda-forge/noarch/tqdm-4.65.0-pyhd8ed1ab_1.conda#ed792aff3acb977d09c7013358097f83
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.3-hd8ed1ab_0.conda#3876f650ed7d0f95d70fa4b647621909
-https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.3-pyhd8ed1ab_0.conda#ae465d0fbf9f1979cb2d8d4043d885e2
-https://conda.anaconda.org/conda-forge/linux-64/gstreamer-1.22.3-h977cf35_1.conda#410ed3b168e5a139d12ebaf4143072cd
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.0-hd8ed1ab_0.conda#37761dccc7ca8eaa08c60c4f62eb2dcc
+https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.3-pyhd8ed1ab_1.conda#89efeecbb24c62e2f1ed0b8ca959ec69
+https://repo.anaconda.com/pkgs/main/linux-64/gstreamer-1.22.3-h5eee18b_0.conda#c2ffbb79cb2f51b042de223d482b7b29
 https://conda.anaconda.org/conda-forge/linux-64/harfbuzz-7.3.0-hdb3a94d_0.conda#765bc76c0dfaf24ff9d8a2935b2510df
 https://conda.anaconda.org/conda-forge/noarch/importlib-resources-5.12.0-pyhd8ed1ab_0.conda#3544c818f0720c89eb16ae6940ab440b
-https://conda.anaconda.org/conda-forge/linux-64/libnetcdf-4.9.2-nompi_h0f3d0bb_105.conda#b5d412441b84305460e9df8a016a3392
+https://conda.anaconda.org/conda-forge/linux-64/libnetcdf-4.9.2-nompi_h78c856c_106.conda#47665bf3dec451455474556ecd940ed2
 https://conda.anaconda.org/conda-forge/linux-64/pandas-1.5.3-py38hdc8b05c_1.conda#c944b033a2126e7f714a7ecaecb22011
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.6.0-pyhd8ed1ab_0.conda#741384b21c1b512617f4ee4ea8457c5d
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.8.0-pyhd8ed1ab_0.conda#3e4aca765371893ad848397794600632
 https://conda.anaconda.org/conda-forge/linux-64/pyqt5-sip-12.11.0-py38h8dc9893_3.conda#7bb0328b4a0f857aeb432426b9a5f908
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/noarch/rich-13.4.2-pyhd8ed1ab_0.conda#f993baacc175e83fafd6b846e9c4c8a2
-https://conda.anaconda.org/conda-forge/linux-64/gst-plugins-base-1.22.3-h938bd60_1.conda#1f317eb7f00db75f4112a07476345376
+https://repo.anaconda.com/pkgs/main/linux-64/gst-plugins-base-1.22.3-he621ea3_0.conda#27be67671dce7d6d8c53bf6260090c15
 https://conda.anaconda.org/conda-forge/linux-64/matplotlib-base-3.7.1-py38hd6c3c57_0.conda#3b8ba76acae09fbd4b2247c4ee4c0324
-https://conda.anaconda.org/conda-forge/linux-64/netcdf4-1.6.4-nompi_py38hdfa7aa7_100.conda#ce30178fb90d4509c3fda5b572124200
+https://conda.anaconda.org/conda-forge/linux-64/netcdf4-1.6.4-nompi_py38h383a0a3_101.conda#693cbd2ee4f62c8a2521cfaf7560b647
 https://conda.anaconda.org/conda-forge/noarch/pooch-1.7.0-pyha770c72_3.conda#5936894aade8240c867d292aa0d980c6
 https://conda.anaconda.org/conda-forge/noarch/typer-0.9.0-pyhd8ed1ab_0.conda#5030a13b2fe5e143d5956d4943d3018f
 https://conda.anaconda.org/conda-forge/noarch/xarray-2023.1.0-pyhd8ed1ab_0.conda#c11eb03b6f77a0d22ae88c454c940f55
 https://conda.anaconda.org/conda-forge/linux-64/qt-main-5.15.8-h01ceb2d_12.conda#60fd4bdf187f88bac57cdc1a052f2811
 https://conda.anaconda.org/conda-forge/linux-64/scipy-1.10.1-py38h59b608b_3.conda#2f2a57462fcfbc67dfdbb0de6f7484c2
 https://conda.anaconda.org/conda-forge/linux-64/pyqt-5.15.7-py38ha0d8c90_3.conda#e965dc172d67920d058ac2b3a0e27565
 https://conda.anaconda.org/conda-forge/linux-64/matplotlib-3.7.1-py38h578d9bd_0.conda#50ff9e0a3dd459a0ca365741072bf9a2
```

### Comparing `eradiate-0.23.2rc3/requirements/conda/environment-main-osx-64.lock` & `eradiate-0.23.2rc4/requirements/conda/environment-main-osx-64.lock`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,62 @@
 # Generated by conda-lock.
 # platform: osx-64
-# input_hash: 43b100c35a9f50d9602c3c883dfa4017d94b56250d5acd29f7e2e8f351eb49c8
+# input_hash: 64bbf5cbb57a84037576a4bb20f3fcdd7659bb44787ea5ed3dd2b4bdf1110c04
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h0d85af4_4.tar.bz2#37edc4e6304ca87316e160f5ca0bd1b5
 https://conda.anaconda.org/conda-forge/osx-64/c-ares-1.19.1-h0dc2134_0.conda#b3e62631b4e1b9801477523ce1d6f355
 https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2023.5.7-h8857fd0_0.conda#b704e4b79ba0d887c4870b7b09d6a4df
 https://conda.anaconda.org/conda-forge/osx-64/icu-72.1-h7336db1_0.conda#c9689510a50a4bb2ae978421671a125e
-https://conda.anaconda.org/conda-forge/osx-64/libbrotlicommon-1.0.9-hb7f2c08_8.tar.bz2#37157d273eaf3bc7d6862104161d9ec9
+https://conda.anaconda.org/conda-forge/osx-64/libbrotlicommon-1.0.9-hb7f2c08_9.conda#ee1ee8c79c3426229ad03290573be552
 https://conda.anaconda.org/conda-forge/osx-64/libcxx-16.0.6-hd57cbcb_0.conda#7d6972792161077908b62971802f289a
 https://conda.anaconda.org/conda-forge/osx-64/libdeflate-1.18-hac1461d_0.conda#3d131584456b277ce0871e6481fde49b
 https://conda.anaconda.org/conda-forge/osx-64/libev-4.33-haf1e3a3_1.tar.bz2#79dc2be110b2a3d1e97ec21f691c50ad
 https://conda.anaconda.org/conda-forge/osx-64/libffi-3.4.2-h0d85af4_5.tar.bz2#ccb34fb14960ad8b125962d3d79b31a9
 https://conda.anaconda.org/conda-forge/osx-64/libiconv-1.17-hac89ed1_0.tar.bz2#691d103d11180486154af49c037b7ed9
 https://conda.anaconda.org/conda-forge/osx-64/libjpeg-turbo-2.1.5.1-hb7f2c08_0.conda#d7309a152b9b79799063b8bb47e34a3a
-https://conda.anaconda.org/conda-forge/osx-64/libwebp-base-1.3.0-hb7f2c08_0.conda#18981e4c840126d6118d8952485fea51
+https://conda.anaconda.org/conda-forge/osx-64/libwebp-base-1.3.1-h0dc2134_0.conda#a25a41b5be3fed4b671a58b998dcf89b
 https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-h8a1eda9_5.conda#4a3ad23f6e16f99c04e166767193d700
 https://conda.anaconda.org/conda-forge/osx-64/llvm-openmp-16.0.6-hff08bdf_0.conda#39a5227d906f75102bf8586741690128
 https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.4-hf0c8a7f_0.conda#c3dbae2411164d9b02c69090a9a91857
 https://conda.anaconda.org/conda-forge/osx-64/pthread-stubs-0.4-hc929b4f_1001.tar.bz2#addd19059de62181cd11ae8f4ef26084
 https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.8-3_cp38.conda#ff192f59f7fe23555612030493a079f8
 https://conda.anaconda.org/conda-forge/osx-64/xorg-libxau-1.0.11-h0dc2134_0.conda#9566b4c29274125b0266d0177b5eb97b
 https://conda.anaconda.org/conda-forge/osx-64/xorg-libxdmcp-1.1.3-h35c211d_0.tar.bz2#86ac76d6bf1cbb9621943eb3bd9ae36e
 https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2#a72f9d4ea13d55d745ff1ed594747f10
 https://conda.anaconda.org/conda-forge/osx-64/hdf4-4.2.15-h9804679_6.conda#c13d8841112ba7f5931d1d60631394f3
 https://conda.anaconda.org/conda-forge/osx-64/lerc-4.0.0-hb486fe8_0.tar.bz2#f9d6a4c82889d5ecedec1d90eb673c55
 https://conda.anaconda.org/conda-forge/osx-64/libaec-1.0.6-hf0c8a7f_1.conda#7c0f82f435ab4c48d65dc9b28db2ad9e
-https://conda.anaconda.org/conda-forge/osx-64/libbrotlidec-1.0.9-hb7f2c08_8.tar.bz2#7f952a036d9014b4dab96c6ea0f8c2a7
-https://conda.anaconda.org/conda-forge/osx-64/libbrotlienc-1.0.9-hb7f2c08_8.tar.bz2#b36a3bfe866d9127f25f286506982166
+https://conda.anaconda.org/conda-forge/osx-64/libbrotlidec-1.0.9-hb7f2c08_9.conda#4043ef9fe42e178785e0e1853b79bdf9
+https://conda.anaconda.org/conda-forge/osx-64/libbrotlienc-1.0.9-hb7f2c08_9.conda#b64d4dcc70aa141db7fccbf13bad81e1
 https://conda.anaconda.org/conda-forge/osx-64/libedit-3.1.20191231-h0678c8f_2.tar.bz2#6016a8a1d0e63cac3de2c352cd40208b
 https://conda.anaconda.org/conda-forge/osx-64/libgfortran5-12.2.0-he409387_31.conda#5a544130e584b1f204ac896ff071d5b3
 https://conda.anaconda.org/conda-forge/osx-64/libpng-1.6.39-ha978bb4_0.conda#35e4928794c5391aec14ffdf1deaaee5
 https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.42.0-h58db7d2_0.conda#a7d3b44b7b0c9901ac7813b7a0462893
 https://conda.anaconda.org/conda-forge/osx-64/libxcb-1.15-hb7f2c08_0.conda#5513f57e0238c87c12dffedbcc9c1a4a
 https://conda.anaconda.org/conda-forge/osx-64/libxml2-2.11.4-hd95e348_0.conda#681f8dda25e73a830d774a37b9839c85
 https://conda.anaconda.org/conda-forge/osx-64/lz4-c-1.9.4-hf0c8a7f_0.conda#aa04f7143228308662696ac24023f991
 https://conda.anaconda.org/conda-forge/osx-64/openssl-3.1.1-h8a1eda9_1.conda#c7822d6ee74e34af1fd74365cfd18983
 https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda#f17f77f2acf4d344734bda76829ce14e
 https://conda.anaconda.org/conda-forge/osx-64/snappy-1.1.10-h225ccf5_0.conda#4320a8781f14cd959689b86e349f3b73
 https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.12-h5dbffcc_0.tar.bz2#8e9480d9c47061db2ed1b4ecce519a7f
 https://conda.anaconda.org/conda-forge/osx-64/zstd-1.5.2-hbc0c0cd_6.conda#40a188783d3c425bdccc9ae9104acbb8
 https://conda.anaconda.org/conda-forge/osx-64/blosc-1.21.4-heccf04b_0.conda#02e92eb72b9ae4c1745b95d03a9c949e
-https://conda.anaconda.org/conda-forge/osx-64/brotli-bin-1.0.9-hb7f2c08_8.tar.bz2#aac5ad0d8f747ef7f871508146df75d9
+https://conda.anaconda.org/conda-forge/osx-64/brotli-bin-1.0.9-hb7f2c08_9.conda#72c526f7ffa265473e6c75fd90605e52
 https://conda.anaconda.org/conda-forge/osx-64/freetype-2.12.1-h3f81eb7_1.conda#852224ea3e8991a8342228eab274840e
 https://conda.anaconda.org/conda-forge/osx-64/krb5-1.20.1-h049b76e_0.conda#db11fa2968ef0837288fe2d7f5b77a50
 https://conda.anaconda.org/conda-forge/osx-64/libgfortran-5.0.0-11_3_0_h97931a8_31.conda#97451338600bd9c5b535eb224ef6c471
 https://conda.anaconda.org/conda-forge/osx-64/libnghttp2-1.52.0-he2ab024_0.conda#12ac7d100bf260263e30a019517f42a2
 https://conda.anaconda.org/conda-forge/osx-64/libssh2-1.11.0-hd019ec5_0.conda#ca3a72efba692c59a90d4b9fc0dfe774
 https://conda.anaconda.org/conda-forge/osx-64/libtiff-4.5.1-hf955e92_0.conda#56523ed556e3a44c0fd55bcf17045892
 https://conda.anaconda.org/conda-forge/osx-64/libzip-1.9.2-h6db710c_1.tar.bz2#ce732d37e479919f3d22b1ccdeb858ac
 https://conda.anaconda.org/conda-forge/osx-64/python-3.8.17-hf9b03c3_0_cpython.conda#f613b663d3829f325b4ffb626bf612b6
-https://conda.anaconda.org/conda-forge/noarch/aenum-3.1.12-pyhd8ed1ab_0.conda#602716538da00b2ca3cc85c4d35c0245
+https://conda.anaconda.org/conda-forge/noarch/aenum-3.1.15-pyhd8ed1ab_0.conda#24cff7ab050ebb8a16bdeb02e8ed6f63
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
-https://conda.anaconda.org/conda-forge/osx-64/brotli-1.0.9-hb7f2c08_8.tar.bz2#55f612fe4a9b5f6ac76348b6de94aaeb
+https://conda.anaconda.org/conda-forge/osx-64/brotli-1.0.9-hb7f2c08_9.conda#53cff90f0cea22e13e5b791f0e5a8e7d
+https://conda.anaconda.org/conda-forge/osx-64/brotli-python-1.0.9-py38h4cd09af_9.conda#f958e25488ff7e044031bca8a6c5267b
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
 https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-unix_pyhd8ed1ab_2.tar.bz2#20e4087407c7cb04a40817114b333dbf
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/noarch/cycler-0.11.0-pyhd8ed1ab_0.tar.bz2#a50559fad0affdbb33729a68669ca1cb
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/osx-64/kiwisolver-1.4.4-py38h98b9b1b_1.tar.bz2#c11eff21a36bc5809b8e23a05ee71df8
@@ -69,51 +70,51 @@
 https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
 https://conda.anaconda.org/conda-forge/noarch/pint-0.21-pyhd8ed1ab_0.conda#8d7b829e37d78447569c180f9d827005
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
 https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.1.0-pyhd8ed1ab_0.conda#d3ed087d1f7f8f5590e8e87b57a8ce64
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
 https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
 https://conda.anaconda.org/conda-forge/osx-64/ruamel.yaml.clib-0.2.7-py38hef030d1_1.conda#9a8e866b0680b61b2e988b18a1eaecae
-https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda#3b68bc43ec6baa48f7354a446267eefe
+https://conda.anaconda.org/conda-forge/noarch/setuptools-68.0.0-pyhd8ed1ab_0.conda#5a7739d0f57ee64133c9d32e6507c46d
 https://conda.anaconda.org/conda-forge/noarch/shellingham-1.4.0-pyh44b312d_0.tar.bz2#437655338696f9d0dfdb0a024e66b255
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
 https://conda.anaconda.org/conda-forge/osx-64/tornado-6.3.2-py38hcafd530_0.conda#afefcf665a5049b030efb084a51e3935
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.3-pyha770c72_0.conda#4a3014a4d107d15475d106b751c4e352
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.0-pyha770c72_0.conda#c76ebd4731d3668ba16975a30ef19d0d
 https://conda.anaconda.org/conda-forge/osx-64/unicodedata2-15.0.0-py38hef030d1_0.tar.bz2#51020c740c53f14657f6307b9eb23f85
 https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
 https://conda.anaconda.org/conda-forge/osx-64/curl-8.1.2-hbee3ae8_0.conda#6cc301a6c2ba26e29949818efdc133ca
 https://conda.anaconda.org/eradiate/noarch/dessinemoi-23.1.0-py_0.tar.bz2#490780e63e113a7dc444bd068e049bfe
 https://conda.anaconda.org/conda-forge/noarch/environ-config-22.1.0-pyhd8ed1ab_0.tar.bz2#a1103faffa0a877313c1fba776aa0fc0
 https://conda.anaconda.org/conda-forge/osx-64/fonttools-4.40.0-py38hcafd530_0.conda#b26b38c5f75e03e86cecf860ca9fb1cd
-https://conda.anaconda.org/conda-forge/osx-64/hdf5-1.14.0-nompi_hbf0aa07_103.conda#90f50d124606a4e62628823b614a2f4c
+https://conda.anaconda.org/conda-forge/osx-64/hdf5-1.14.1-nompi_hedada53_100.conda#033c310c83abbd9c2f9a5c13b9f54225
 https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
 https://conda.anaconda.org/conda-forge/osx-64/libblas-3.9.0-17_osx64_openblas.conda#65299527582e2449b05d27fcf8352125
 https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-3.0.0-pyhd8ed1ab_0.conda#93a8e71256479c62074356ef6ebf501b
-https://conda.anaconda.org/conda-forge/osx-64/pillow-9.5.0-py38h16710f9_1.conda#c5bf174a033ef668679cc80918422515
+https://conda.anaconda.org/conda-forge/osx-64/pillow-10.0.0-py38h16710f9_0.conda#8f73f0573ab381d56588e001754c53d3
 https://conda.anaconda.org/eradiate/noarch/pinttrs-23.2.0-py_0.tar.bz2#1aebe9fa813278f719fa8e31d8000452
 https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
 https://conda.anaconda.org/conda-forge/noarch/portion-2.4.0-pyhd8ed1ab_0.conda#9d34bac22e169b41f4e34525a140c13b
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
 https://conda.anaconda.org/conda-forge/osx-64/ruamel.yaml-0.17.32-py38hcafd530_0.conda#cb301e0b2b162330bc3b03fe51ea0d15
 https://conda.anaconda.org/conda-forge/noarch/tqdm-4.65.0-pyhd8ed1ab_1.conda#ed792aff3acb977d09c7013358097f83
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.3-hd8ed1ab_0.conda#3876f650ed7d0f95d70fa4b647621909
-https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.3-pyhd8ed1ab_0.conda#ae465d0fbf9f1979cb2d8d4043d885e2
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.0-hd8ed1ab_0.conda#37761dccc7ca8eaa08c60c4f62eb2dcc
+https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.3-pyhd8ed1ab_1.conda#89efeecbb24c62e2f1ed0b8ca959ec69
 https://conda.anaconda.org/conda-forge/noarch/importlib-resources-5.12.0-pyhd8ed1ab_0.conda#3544c818f0720c89eb16ae6940ab440b
 https://conda.anaconda.org/conda-forge/osx-64/libcblas-3.9.0-17_osx64_openblas.conda#380151ca00704172b242a63701b7bf8a
 https://conda.anaconda.org/conda-forge/osx-64/liblapack-3.9.0-17_osx64_openblas.conda#6ab83532872bf3659613638589dd10af
-https://conda.anaconda.org/conda-forge/osx-64/libnetcdf-4.9.2-nompi_hf077d52_105.conda#64d626e024a284777458e2b315e9eb56
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.6.0-pyhd8ed1ab_0.conda#741384b21c1b512617f4ee4ea8457c5d
+https://conda.anaconda.org/conda-forge/osx-64/libnetcdf-4.9.2-nompi_hfeda9e8_106.conda#66108519efbf30b02632ad35f519773f
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.8.0-pyhd8ed1ab_0.conda#3e4aca765371893ad848397794600632
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/noarch/rich-13.4.2-pyhd8ed1ab_0.conda#f993baacc175e83fafd6b846e9c4c8a2
-https://conda.anaconda.org/conda-forge/osx-64/numpy-1.24.3-py38h9a4a08f_0.conda#5ff64b8133dea66865fe1bd35fb1d6d6
+https://conda.anaconda.org/conda-forge/osx-64/numpy-1.24.4-py38h9a4a08f_0.conda#85debc55a30068d6bb76a6deaf599afa
 https://conda.anaconda.org/conda-forge/noarch/pooch-1.7.0-pyha770c72_3.conda#5936894aade8240c867d292aa0d980c6
 https://conda.anaconda.org/conda-forge/noarch/typer-0.9.0-pyhd8ed1ab_0.conda#5030a13b2fe5e143d5956d4943d3018f
 https://conda.anaconda.org/conda-forge/osx-64/cftime-1.6.2-py38hbd87e4b_1.tar.bz2#6b61efa56393b9655334192cc5423659
 https://conda.anaconda.org/conda-forge/osx-64/contourpy-1.1.0-py38h15a1a5b_0.conda#30d645ffb3572a3875e6fc8687857182
 https://conda.anaconda.org/conda-forge/osx-64/pandas-1.5.3-py38hec72209_1.conda#a8f001ab0a7c6312cea020bd20689765
 https://conda.anaconda.org/conda-forge/osx-64/scipy-1.10.1-py38h9cf86d3_3.conda#5e20c77455e815704b008ab8f42f6169
 https://conda.anaconda.org/conda-forge/osx-64/matplotlib-base-3.7.1-py38hcb346ec_0.conda#1f1eea98c232c8ef720175e12b00d0c4
-https://conda.anaconda.org/conda-forge/osx-64/netcdf4-1.6.4-nompi_py38h47ac6a0_100.conda#f86d4df9f8f46ae6d0c29bb87fe093b0
+https://conda.anaconda.org/conda-forge/osx-64/netcdf4-1.6.4-nompi_py38ha129777_101.conda#0e0f917d6168b9744a407d5ef3c2cb09
 https://conda.anaconda.org/conda-forge/noarch/xarray-2023.1.0-pyhd8ed1ab_0.conda#c11eb03b6f77a0d22ae88c454c940f55
 https://conda.anaconda.org/conda-forge/osx-64/matplotlib-3.7.1-py38h50d1736_0.conda#14bce132d8a4546246b131c4289b480f
```

### Comparing `eradiate-0.23.2rc3/requirements/conda/environment-optional-linux-64.lock` & `eradiate-0.23.2rc4/requirements/conda/environment-optional-linux-64.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Generated by conda-lock.
 # platform: linux-64
-# input_hash: 9dcecc3b104941efb0fda739f479016fbf6654d5f0596f31fc7e8f13170c7d08
+# input_hash: 663e5d9eaad318a79c7cbf185aa33c7e6c2fba5cd7511d678b1e7304b2233d11
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2#d7c89558ba9fa0495403155b64376d81
 https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2023.5.7-hbcca054_0.conda#f5c65075fc34438d5b456c7f3f5ab695
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-dejavu-sans-mono-2.37-hab24e00_0.tar.bz2#0c96522c6bdaed4b1566d11387caaf45
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-inconsolata-3.000-h77eed37_0.tar.bz2#34893075a5c9e55cdafac56607368fc6
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-source-code-pro-2.038-h77eed37_0.tar.bz2#4d59c254e01d9cde7957100457e2d5fb
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-ubuntu-0.83-hab24e00_0.tar.bz2#19410c3df09dfb12d1206132a1d357c5
@@ -26,28 +26,28 @@
 https://conda.anaconda.org/conda-forge/linux-64/gmp-6.2.1-h58526e2_0.tar.bz2#b94cf2db16066b242ebd26db2facbd56
 https://conda.anaconda.org/conda-forge/linux-64/graphite2-1.3.13-h58526e2_1001.tar.bz2#8c54672728e8ec6aa6db90cf2806d220
 https://conda.anaconda.org/conda-forge/linux-64/icu-72.1-hcb278e6_0.conda#7c8d20d847bb45f56bd941578fcfa146
 https://conda.anaconda.org/conda-forge/linux-64/keyutils-1.6.1-h166bdaf_0.tar.bz2#30186d27e2c9fa62b45fb1476b7200e3
 https://conda.anaconda.org/conda-forge/linux-64/lame-3.100-h166bdaf_1003.tar.bz2#a8832b479f93521a9e7b5b743803be51
 https://conda.anaconda.org/conda-forge/linux-64/lerc-4.0.0-h27087fc_0.tar.bz2#76bbff344f0134279f225174e9064c8f
 https://conda.anaconda.org/conda-forge/linux-64/libaec-1.0.6-hcb278e6_1.conda#0f683578378cddb223e7fd24f785ab2a
-https://conda.anaconda.org/conda-forge/linux-64/libbrotlicommon-1.0.9-h166bdaf_8.tar.bz2#9194c9bf9428035a05352d031462eae4
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlicommon-1.0.9-h166bdaf_9.conda#61641e239f96eae2b8492dc7e755828c
 https://conda.anaconda.org/conda-forge/linux-64/libdeflate-1.18-h0b41bf4_0.conda#6aa9c9de5542ecb07fdda9ca626252d8
 https://conda.anaconda.org/conda-forge/linux-64/libev-4.33-h516909a_1.tar.bz2#6f8720dff19e17ce5d48cfe7f3d2f0a3
 https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.5.0-hcb278e6_1.conda#6305a3dd2752c76335295da4e581f2fd
 https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2#d645c6d2ac96843a2bfaccd2d62b3ac3
 https://conda.anaconda.org/conda-forge/linux-64/libiconv-1.17-h166bdaf_0.tar.bz2#b62b52da46c39ee2bc3c162ac7f1804d
 https://conda.anaconda.org/conda-forge/linux-64/libjpeg-turbo-2.1.5.1-h0b41bf4_0.conda#1edd9e67bdb90d78cea97733ff6b54e6
 https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.0-h7f98852_0.tar.bz2#39b1328babf85c7c3a61636d9cd50206
-https://conda.anaconda.org/conda-forge/linux-64/libogg-1.3.4-h7f98852_1.tar.bz2#6e8cc2173440d77708196c5b93771680
+https://repo.anaconda.com/pkgs/main/linux-64/libogg-1.3.5-h27cfd23_1.conda#710ee7fdb0ddf7591a5af7ca7eb4d73d
 https://conda.anaconda.org/conda-forge/linux-64/libopenblas-0.3.23-pthreads_h80387f5_0.conda#9c5ea51ccb8ffae7d06c645869d24ce6
 https://conda.anaconda.org/conda-forge/linux-64/libopus-1.3.1-h7f98852_1.tar.bz2#15345e56d527b330e1cacbdf58676e8f
 https://conda.anaconda.org/conda-forge/linux-64/libsodium-1.0.18-h36c2ea0_1.tar.bz2#c3788462a6fbddafdb413a9f9053e58d
 https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda#40b61aab5c7ba9ff276c41cfffe6b80b
-https://conda.anaconda.org/conda-forge/linux-64/libwebp-base-1.3.0-h0b41bf4_0.conda#0d4a7508d8c6c65314f2b9c1f56ad408
+https://conda.anaconda.org/conda-forge/linux-64/libwebp-base-1.3.1-hd590300_0.conda#82bf6f63eb15ef719b556b63feec3a77
 https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-hd590300_5.conda#f36c115f1ee199da648e0597ec2047ad
 https://conda.anaconda.org/conda-forge/linux-64/lz4-c-1.9.4-hcb278e6_0.conda#318b08df404f9c9be5712aaa5a6f0bb0
 https://conda.anaconda.org/conda-forge/linux-64/mpg123-1.31.3-hcb278e6_0.conda#141a126675b6d1a4eabb111a4a353898
 https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.4-hcb278e6_0.conda#681105bccc2a3f7f1a837d47d39c9179
 https://conda.anaconda.org/conda-forge/linux-64/nspr-4.35-h27087fc_0.conda#da0ec11a6454ae19bff5b02ed881a2b1
 https://conda.anaconda.org/conda-forge/linux-64/openssl-3.1.1-hd590300_1.conda#2e1d7b458ac8f1e3ca4e18b77add6277
 https://conda.anaconda.org/conda-forge/linux-64/pixman-0.40.0-h36c2ea0_0.tar.bz2#660e72c82f2e75a6b3fe6a6e75c79f19
@@ -62,65 +62,65 @@
 https://conda.anaconda.org/conda-forge/linux-64/xorg-xf86vidmodeproto-2.3.1-h7f98852_1002.tar.bz2#3ceea9668625c18f19530de98b15d5b0
 https://conda.anaconda.org/conda-forge/linux-64/xorg-xproto-7.0.31-h7f98852_1007.tar.bz2#b4a4381d54784606820704f7b5f05a15
 https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2#2161070d867d1b1204ea749c8eec4ef0
 https://conda.anaconda.org/conda-forge/linux-64/yaml-0.2.5-h7f98852_2.tar.bz2#4cb3ad778ec2d5a7acbdf254eb1c42ae
 https://conda.anaconda.org/conda-forge/linux-64/expat-2.5.0-hcb278e6_1.conda#8b9b5aca60558d02ddaa09d599e55920
 https://conda.anaconda.org/conda-forge/linux-64/hdf4-4.2.15-h501b40f_6.conda#c3e9338e15d90106f467377017352b97
 https://conda.anaconda.org/conda-forge/linux-64/libblas-3.9.0-17_linux64_openblas.conda#57fb44770b1bc832fb2dbefa1bd502de
-https://conda.anaconda.org/conda-forge/linux-64/libbrotlidec-1.0.9-h166bdaf_8.tar.bz2#4ae4d7795d33e02bd20f6b23d91caf82
-https://conda.anaconda.org/conda-forge/linux-64/libbrotlienc-1.0.9-h166bdaf_8.tar.bz2#04bac51ba35ea023dc48af73c1c88c25
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlidec-1.0.9-h166bdaf_9.conda#081aa22f4581c08e4372b0b6c2f8478e
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlienc-1.0.9-h166bdaf_9.conda#1f0a03af852a9659ed2bf08f2f1704fd
 https://conda.anaconda.org/conda-forge/linux-64/libcap-2.67-he9d0100_0.conda#d05556c80caffff164d17bdea0105a1a
 https://conda.anaconda.org/conda-forge/linux-64/libedit-3.1.20191231-he28a2e2_2.tar.bz2#4d331e44109e3f0e19b4cb8f9b82f3e1
 https://conda.anaconda.org/conda-forge/linux-64/libevent-2.1.12-hf998b51_1.conda#a1cfcc585f0c42bf8d5546bb1dfb668d
-https://conda.anaconda.org/conda-forge/linux-64/libflac-1.4.2-h27087fc_0.tar.bz2#7daf72d8e2a8e848e11d63ed6d1026e0
+https://conda.anaconda.org/conda-forge/linux-64/libflac-1.4.3-h59595ed_0.conda#ee48bf17cc83a00f59ca1494d5646869
 https://conda.anaconda.org/conda-forge/linux-64/libgpg-error-1.47-h71f35ed_0.conda#c2097d0b46367996f09b4e8e4920384a
 https://conda.anaconda.org/conda-forge/linux-64/libnghttp2-1.52.0-h61bc06f_0.conda#613955a50485812985c059e7b269f42e
 https://conda.anaconda.org/conda-forge/linux-64/libpng-1.6.39-h753d276_0.conda#e1c890aebdebbfbf87e2c917187b4416
 https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.42.0-h2797004_0.conda#fdaae20a1cf7cd62130a0973190a31b7
 https://conda.anaconda.org/conda-forge/linux-64/libssh2-1.11.0-h0841786_0.conda#1f5a58e686b13bcfde88b93f547d23fe
 https://conda.anaconda.org/conda-forge/linux-64/libvorbis-1.3.7-h9c3ff4c_0.tar.bz2#309dec04b70a3cc0f1e84a4013683bc0
 https://conda.anaconda.org/conda-forge/linux-64/libxcb-1.15-h0b41bf4_0.conda#33277193f5b92bad9fdd230eb700929c
 https://conda.anaconda.org/conda-forge/linux-64/libxml2-2.11.4-h0d562d8_0.conda#e46fad17d5fb57316b956f88dca765e4
 https://conda.anaconda.org/conda-forge/linux-64/libzip-1.9.2-hc929e4a_1.tar.bz2#5b122b50e738c4be5c3f2899f010d7cf
-https://conda.anaconda.org/conda-forge/linux-64/mysql-common-8.0.33-hf1915f5_0.conda#aa8b86066614c4573f6db62c91978fa9
+https://conda.anaconda.org/conda-forge/linux-64/mysql-common-8.0.33-hf1915f5_1.conda#b241363e3b72bae6dfbd31e9fecf7d26
 https://conda.anaconda.org/conda-forge/linux-64/pcre2-10.40-hc3806b6_0.tar.bz2#69e2c796349cd9b273890bee0febfe1b
 https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda#47d31b792659ce70f470b5c82fdfb7a4
 https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.12-h27826a3_0.tar.bz2#5b8c42eb62e9fc961af70bdd6a26e168
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libsm-1.2.4-h7391055_0.conda#93ee23f12bc2e684548181256edd2cf6
 https://conda.anaconda.org/conda-forge/linux-64/zeromq-4.3.4-h9c3ff4c_1.tar.bz2#21743a8d2ea0c8cfbbf8fe489b0347df
 https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.13-hd590300_5.conda#68c34ec6149623be41a1933ab996a209
 https://conda.anaconda.org/conda-forge/linux-64/zstd-1.5.2-h3eb15da_6.conda#6b63daed8feeca47be78f323e793d555
 https://conda.anaconda.org/conda-forge/linux-64/blosc-1.21.4-h0f2a231_0.conda#876286b5941933a0f558777e57d883cc
-https://conda.anaconda.org/conda-forge/linux-64/brotli-bin-1.0.9-h166bdaf_8.tar.bz2#e5613f2bc717e9945840ff474419b8e4
+https://conda.anaconda.org/conda-forge/linux-64/brotli-bin-1.0.9-h166bdaf_9.conda#d47dee1856d9cb955b8076eeff304a5b
 https://conda.anaconda.org/conda-forge/linux-64/freetype-2.12.1-hca18f0e_1.conda#e1232042de76d24539a436d37597eb06
 https://conda.anaconda.org/conda-forge/linux-64/krb5-1.20.1-h81ceb04_0.conda#89a41adce7106749573d883b2f657d78
 https://conda.anaconda.org/conda-forge/linux-64/libcblas-3.9.0-17_linux64_openblas.conda#7ef0969b00fe3d6eef56a8151d3afb29
 https://conda.anaconda.org/conda-forge/linux-64/libgcrypt-1.10.1-h166bdaf_0.tar.bz2#f967fc95089cd247ceed56eda31de3a9
 https://conda.anaconda.org/conda-forge/linux-64/libglib-2.76.3-hebfc3b9_0.conda#a64f11b244b2c112cd3fa1cbe9493999
 https://conda.anaconda.org/conda-forge/linux-64/liblapack-3.9.0-17_linux64_openblas.conda#a2103882c46492e26500fcb56c03de8b
 https://conda.anaconda.org/conda-forge/linux-64/libllvm16-16.0.6-h5cf9203_0.conda#753e078cccad40fe4b396bdcf27a3c15
 https://conda.anaconda.org/conda-forge/linux-64/libsndfile-1.2.0-hb75c966_0.conda#c648d19cd9c8625898d5d370414de7c7
 https://conda.anaconda.org/conda-forge/linux-64/libtiff-4.5.1-h8b53f26_0.conda#8ad377fb60abab446a9f02c62b3c2190
-https://conda.anaconda.org/conda-forge/linux-64/mysql-libs-8.0.33-hca2cd23_0.conda#276339b0115d92c6e0793dcdc7afe308
+https://conda.anaconda.org/conda-forge/linux-64/mysql-libs-8.0.33-hca2cd23_1.conda#a04ac37f0659929f3ba0f33c7f3d750f
 https://conda.anaconda.org/conda-forge/linux-64/nss-3.89-he45b914_0.conda#2745719a58eeaab6657256a3f142f099
 https://conda.anaconda.org/conda-forge/linux-64/pandoc-3.1.3-h32600fe_0.conda#8287aeb8462e2d4b235eff788e75919d
 https://conda.anaconda.org/conda-forge/linux-64/python-3.8.17-he550d4f_0_cpython.conda#72d038de0a228e4f0ef4011940641293
 https://conda.anaconda.org/conda-forge/linux-64/xcb-util-0.4.0-hd590300_1.conda#9bfac7ccd94d54fd21a0501296d60424
 https://conda.anaconda.org/conda-forge/linux-64/xcb-util-keysyms-0.4.0-h8ee46fc_1.conda#632413adcd8bc16b515cab87a2932913
 https://conda.anaconda.org/conda-forge/linux-64/xcb-util-renderutil-0.3.9-hd590300_1.conda#e995b155d938b6779da6ace6c6b13816
 https://conda.anaconda.org/conda-forge/linux-64/xcb-util-wm-0.4.1-h8ee46fc_1.conda#90108a432fb5c6150ccfee3f03388656
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libx11-1.8.6-h8ee46fc_0.conda#7590b76c3d11d21caa44f3fc38ac584a
 https://conda.anaconda.org/eradiate/noarch/aabbtree-2.8.0-py_0.tar.bz2#647bcce5f0af4974e507591d5420486b
-https://conda.anaconda.org/conda-forge/noarch/aenum-3.1.12-pyhd8ed1ab_0.conda#602716538da00b2ca3cc85c4d35c0245
+https://conda.anaconda.org/conda-forge/noarch/aenum-3.1.15-pyhd8ed1ab_0.conda#24cff7ab050ebb8a16bdeb02e8ed6f63
 https://conda.anaconda.org/conda-forge/noarch/alabaster-0.7.13-pyhd8ed1ab_0.conda#06006184e203b61d3525f90de394471e
 https://conda.anaconda.org/conda-forge/noarch/appdirs-1.4.4-pyh9f0ad1d_0.tar.bz2#5f095bc6454094e96f146491fd03633b
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
-https://conda.anaconda.org/conda-forge/linux-64/brotli-1.0.9-h166bdaf_8.tar.bz2#2ff08978892a3e8b954397c461f18418
+https://conda.anaconda.org/conda-forge/linux-64/brotli-1.0.9-h166bdaf_9.conda#4601544b4982ba1861fa9b9c607b2c06
 https://conda.anaconda.org/conda-forge/noarch/cachy-0.3.0-pyhd8ed1ab_1.tar.bz2#5dfee17f24e2dfd18d7392b48c9351e2
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
 https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-unix_pyhd8ed1ab_2.tar.bz2#20e4087407c7cb04a40817114b333dbf
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/noarch/crashtest-0.4.1-pyhd8ed1ab_0.tar.bz2#709a2295dd907bb34afb57d54320642f
 https://conda.anaconda.org/conda-forge/noarch/cycler-0.11.0-pyhd8ed1ab_0.tar.bz2#a50559fad0affdbb33729a68669ca1cb
@@ -138,15 +138,15 @@
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
 https://conda.anaconda.org/conda-forge/linux-64/fontconfig-2.14.2-h14ed4e7_0.conda#0f69b688f52ff6da70bccb7ff7001d1d
 https://conda.anaconda.org/conda-forge/linux-64/glib-tools-2.76.3-hfc55251_0.conda#8951eedf3cdf94dd733c1b5eee1f4880
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/imagesize-1.4.1-pyhd8ed1ab_0.tar.bz2#7de5386c8fea29e76b303f37dde4c352
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda#f800d2da156d08e289b14e87e43c1ae5
 https://conda.anaconda.org/conda-forge/noarch/jeepney-0.8.0-pyhd8ed1ab_0.tar.bz2#9800ad1699b42612478755a2d26c722d
-https://conda.anaconda.org/conda-forge/noarch/json5-0.9.5-pyh9f0ad1d_0.tar.bz2#10759827a94e6b14996e81fb002c0bda
+https://conda.anaconda.org/conda-forge/noarch/json5-0.9.14-pyhd8ed1ab_0.conda#dac1dabba2b5a9d1aee175c5fcc7b436
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.7-pyhd8ed1ab_1.conda#0c0a54e16b764bafcae35913cc9d60ff
 https://conda.anaconda.org/conda-forge/linux-64/kiwisolver-1.4.4-py38h43d8883_1.tar.bz2#41ca56d5cac7bfc7eb4fcdbee878eb84
 https://conda.anaconda.org/conda-forge/noarch/lazy_loader-0.2-pyhd8ed1ab_0.conda#d060d017720c9882c4eca0544a4a0592
 https://conda.anaconda.org/conda-forge/linux-64/lcms2-2.15-haa2dc70_1.conda#980d8aca0bc23ca73fa8caa3e7c84c28
 https://conda.anaconda.org/conda-forge/linux-64/libclang13-16.0.6-default_h4d60ac6_0.conda#b10174a063ec195f8fe1b278282c3149
 https://conda.anaconda.org/conda-forge/linux-64/libcups-2.3.3-h36d4200_3.conda#c9f4416a34bc91e0eb029f912c68f81f
 https://conda.anaconda.org/conda-forge/linux-64/libcurl-8.1.2-h409715c_0.conda#50c873c9660ed116707ae15b663928d8
@@ -157,25 +157,25 @@
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.0-pyhd8ed1ab_0.tar.bz2#f8dab71fdc13b1bf29a01248b156d268
 https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.0-pyhd8ed1ab_0.conda#c7d0ea64c37752ecbe6da458aee662d2
 https://conda.anaconda.org/conda-forge/noarch/more-itertools-9.1.0-pyhd8ed1ab_0.conda#1698a717f83cfecf644a877c174c84bd
 https://conda.anaconda.org/conda-forge/linux-64/msgpack-python-1.0.5-py38hfbd4bf9_0.conda#5401b83c1007f408d0c74e23fa9b5eff
 https://conda.anaconda.org/conda-forge/noarch/munkres-1.1.4-pyh9f0ad1d_0.tar.bz2#2ba8498c1018c1e9c61eb99b973dfe19
 https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.5.6-pyhd8ed1ab_0.tar.bz2#7b868f21adde0d9b8b38f9c16836589b
 https://conda.anaconda.org/conda-forge/noarch/networkx-3.1-pyhd8ed1ab_0.conda#254f787d5068bc89f578bf63893ce8b4
-https://conda.anaconda.org/conda-forge/linux-64/numpy-1.24.3-py38h59b608b_0.conda#5836e4ab0399136ede58446a4776b2ff
+https://conda.anaconda.org/conda-forge/linux-64/numpy-1.24.4-py38h59b608b_0.conda#8c3e050afeeb2b32575bdb8955cc67b2
 https://conda.anaconda.org/conda-forge/linux-64/openjpeg-2.5.0-hfec8fc6_2.conda#5ce6a42505c6e9e6151c54c3ec8d68ea
 https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/parso-0.8.3-pyhd8ed1ab_0.tar.bz2#17a565a0c3899244e938cdf417e7b094
 https://conda.anaconda.org/conda-forge/noarch/pastel-0.2.1-pyhd8ed1ab_0.tar.bz2#a4eea5bff523f26442405bc5d1f52adb
 https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
 https://conda.anaconda.org/conda-forge/noarch/pint-0.21-pyhd8ed1ab_0.conda#8d7b829e37d78447569c180f9d827005
 https://conda.anaconda.org/conda-forge/noarch/pkginfo-1.9.6-pyhd8ed1ab_0.conda#be1e9f1c65a1ed0f2ae9352fec99db64
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2#89e3c7cdde7d3aaa2aee933b604dd07f
-https://conda.anaconda.org/conda-forge/noarch/pluggy-1.0.0-pyhd8ed1ab_5.tar.bz2#7d301a0d25f424d96175f810935f0da9
+https://conda.anaconda.org/conda-forge/noarch/pluggy-1.2.0-pyhd8ed1ab_0.conda#7263924c642d22e311d9e59b839f1b33
 https://conda.anaconda.org/conda-forge/noarch/ply-3.11-py_1.tar.bz2#7205635cd71531943440fbfe3b6b5727
 https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.0-pyhd8ed1ab_0.conda#95c5be3c7cbd872509d16c216617fdab
 https://conda.anaconda.org/conda-forge/linux-64/psutil-5.9.5-py38h1de0b5d_0.conda#92e899e7b0ed27c793014d1fa54f9b7b
 https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2#359eeb6536da0e687af562ed265ec263
 https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2#6784285c7e55cb7212efabc79e4c2883
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
@@ -187,15 +187,15 @@
 https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.7-pyhd8ed1ab_0.conda#a61bf9ec79426938ff785eb69dbb1960
 https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
 https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0-py38h0a891b7_5.tar.bz2#0856c59f9ddb710c640dc0428d66b1b7
 https://conda.anaconda.org/conda-forge/linux-64/pyzmq-25.1.0-py38h509eb50_0.conda#33872b6650886eba869408b76c96994c
 https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2#912a71cc01012ee38e6b90ddd561e36f
 https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml.clib-0.2.7-py38h1de0b5d_1.conda#9afa2fc3c51cc4e7d1589c38e4e00d5c
 https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyh41d4057_0.conda#ada5a17adcd10be4fc7e37e4166ba0e2
-https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda#3b68bc43ec6baa48f7354a446267eefe
+https://conda.anaconda.org/conda-forge/noarch/setuptools-68.0.0-pyhd8ed1ab_0.conda#5a7739d0f57ee64133c9d32e6507c46d
 https://conda.anaconda.org/conda-forge/noarch/shellingham-1.4.0-pyh44b312d_0.tar.bz2#437655338696f9d0dfdb0a024e66b255
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/smmap-3.0.5-pyh44b312d_0.tar.bz2#3a8dc70789709aa315325d5df06fb7e4
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
 https://conda.anaconda.org/conda-forge/noarch/snowballstemmer-2.2.0-pyhd8ed1ab_0.tar.bz2#4d22a9315e78c6827f806065957d566e
 https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
@@ -207,32 +207,32 @@
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-serializinghtml-1.1.5-pyhd8ed1ab_2.tar.bz2#9ff55a0901cf952f05c654394de76bf7
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.11.8-pyha770c72_0.conda#75838e8556166263a82038b51d01d5f1
 https://conda.anaconda.org/conda-forge/noarch/toolz-0.12.0-pyhd8ed1ab_0.tar.bz2#92facfec94bc02d6ccf42e7173831a36
 https://conda.anaconda.org/conda-forge/linux-64/tornado-6.3.2-py38h01eb140_0.conda#3db869202b0e523d606d13e81ca79ab6
 https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.3-pyha770c72_0.conda#4a3014a4d107d15475d106b751c4e352
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.0-pyha770c72_0.conda#c76ebd4731d3668ba16975a30ef19d0d
 https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/linux-64/unicodedata2-15.0.0-py38h0a891b7_0.tar.bz2#44421904760e9f5ae2035193e04360f0
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
-https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.0-pyhd8ed1ab_0.conda#1dd6387a73d84e16b6f73de676bb4c36
+https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda#c34d9325a609381a0b0e8a5b4f325147
 https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
 https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.7-pyhd8ed1ab_0.conda#bcc54b91a8ce88f60f538b87b409909e
 https://conda.anaconda.org/conda-forge/linux-64/xcb-util-image-0.4.0-h8ee46fc_1.conda#9d7bcddf49cbf727730af10e71022c73
 https://conda.anaconda.org/conda-forge/linux-64/xkeyboard-config-2.39-hd590300_0.conda#d88c7fc8a11858fb14761832e4da1954
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxext-1.3.4-h0b41bf4_2.conda#82b6df12252e6f32402b96dacc656fec
-https://conda.anaconda.org/conda-forge/linux-64/xorg-libxrender-0.9.10-h7f98852_1003.tar.bz2#f59c1242cc1dd93e72c2ee2b360979eb
+https://conda.anaconda.org/conda-forge/linux-64/xorg-libxrender-0.9.11-hd590300_0.conda#ed67c36f215b310412b2af935bf3e530
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
 https://conda.anaconda.org/conda-forge/noarch/accessible-pygments-0.0.4-pyhd8ed1ab_0.conda#46a2e6e3dfa718ce3492018d5a110dd6
 https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.0-pyhd8ed1ab_1.conda#2b35a85d654a47aac8f34c1bb6de7142
 https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
 https://conda.anaconda.org/conda-forge/noarch/async-lru-2.0.2-pyhd8ed1ab_0.conda#41221f97a0c82e5a60b21716a3d7469c
 https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
-https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.4-pyhd8ed1ab_0.tar.bz2#c5b3edc62d6309088f4970b3eaaa65a6
+https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda#6b1b907661838a75d067a22f87996b2e
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
 https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda#d48b143d01385872a88ef8417e96c30e
 https://conda.anaconda.org/conda-forge/linux-64/cairo-1.16.0-hbbf8b49_1016.conda#c1dd96500b9b1a75e9e511931f415cbc
 https://conda.anaconda.org/conda-forge/linux-64/cffi-1.15.1-py38h4a40e3a_3.conda#3ac112151c6b6cfe457e976de41af0c5
 https://conda.anaconda.org/conda-forge/linux-64/cftime-1.6.2-py38h26c90d9_1.tar.bz2#dcc025a7bb54374979c500c2e161fac9
 https://conda.anaconda.org/conda-forge/noarch/click-default-group-1.2.2-pyhd8ed1ab_1.tar.bz2#72a46ffc25701c173932fd55cf0965d3
 https://conda.anaconda.org/conda-forge/noarch/clikit-0.6.2-pyhd8ed1ab_2.conda#02abb7b66b02e8b9f5a9b05454400087
@@ -240,15 +240,15 @@
 https://conda.anaconda.org/conda-forge/linux-64/contourpy-1.1.0-py38h7f3f72f_0.conda#0fdf3cc879156e0234e05962d55b6502
 https://conda.anaconda.org/conda-forge/linux-64/curl-8.1.2-h409715c_0.conda#9f88cfb15b7d08b25880b138f91e0eb4
 https://conda.anaconda.org/eradiate/noarch/dessinemoi-23.1.0-py_0.tar.bz2#490780e63e113a7dc444bd068e049bfe
 https://conda.anaconda.org/conda-forge/noarch/environ-config-22.1.0-pyhd8ed1ab_0.tar.bz2#a1103faffa0a877313c1fba776aa0fc0
 https://conda.anaconda.org/conda-forge/linux-64/fonttools-4.40.0-py38h01eb140_0.conda#f893b6bac56c477dd71498569b4a9022
 https://conda.anaconda.org/conda-forge/noarch/gitdb-4.0.10-pyhd8ed1ab_0.conda#3706d2f3d7cb5dae600c833345a76132
 https://conda.anaconda.org/conda-forge/linux-64/glib-2.76.3-hfc55251_0.conda#950e02f5665f5f4ff0437a6acba58798
-https://conda.anaconda.org/conda-forge/linux-64/hdf5-1.14.0-nompi_hb72d44e_103.conda#975973a4350ab45ff1981fe535a12af5
+https://conda.anaconda.org/conda-forge/linux-64/hdf5-1.14.1-nompi_h4f84152_100.conda#ff9ae10aa224826c07da7ef26cb0b717
 https://conda.anaconda.org/conda-forge/noarch/html5lib-1.1-pyh9f0ad1d_0.tar.bz2#b2355343d6315c892543200231d7154a
 https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.7.0-pyha770c72_0.conda#ba3786c6846e46038fe60c785d46dc81
 https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
 https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.2.3-pyhd8ed1ab_0.tar.bz2#31e4a1506968d017229bdb64695013a1
 https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
 https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-4.12.0-py38h578d9bd_0.conda#e7f204764ab3683174c1707240368b84
@@ -257,82 +257,84 @@
 https://conda.anaconda.org/conda-forge/linux-64/libclang-16.0.6-default_h1cdf331_0.conda#e976871e132fe506da52c1240229246a
 https://conda.anaconda.org/conda-forge/linux-64/libxkbcommon-1.5.0-h5d7e998_3.conda#c91ea308d7bf70b62ddda568478aa03b
 https://conda.anaconda.org/conda-forge/noarch/livereload-2.6.3-pyh9f0ad1d_0.tar.bz2#b7190e3ec3eff52839434bf4698e2d62
 https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-2.2.0-pyhd8ed1ab_0.conda#b2928a6c6d52d7e3562b4a59c3214e3a
 https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
 https://conda.anaconda.org/conda-forge/noarch/overrides-7.3.1-pyhd8ed1ab_0.tar.bz2#a5745ced46e69aa9754053ba061974ab
 https://conda.anaconda.org/conda-forge/noarch/pexpect-4.8.0-pyh1a96a4e_2.tar.bz2#330448ce4403cc74990ac07c555942a1
-https://conda.anaconda.org/conda-forge/linux-64/pillow-9.5.0-py38h885162f_1.conda#0eec8a20a17f17ec9e0b6839be466866
+https://conda.anaconda.org/conda-forge/linux-64/pillow-10.0.0-py38h885162f_0.conda#777c54134d5422a867aed7084cf5db5e
 https://conda.anaconda.org/eradiate/noarch/pinttrs-23.2.0-py_0.tar.bz2#1aebe9fa813278f719fa8e31d8000452
 https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
 https://conda.anaconda.org/conda-forge/noarch/portion-2.4.0-pyhd8ed1ab_0.conda#9d34bac22e169b41f4e34525a140c13b
 https://conda.anaconda.org/conda-forge/linux-64/pulseaudio-client-16.1-hb77b528_4.conda#8f349ca16d30950aa00870484d9d30c4
 https://conda.anaconda.org/conda-forge/linux-64/pyerfa-2.0.0.3-py38h7e4f40d_0.conda#631de6b5c8aec9c8ae2dcc596f8d2f72
 https://conda.anaconda.org/conda-forge/noarch/pyproject_hooks-1.0.0-pyhd8ed1ab_0.conda#21de50391d584eb7f4441b9de1ad773f
-https://conda.anaconda.org/conda-forge/noarch/pytest-7.3.2-pyhd8ed1ab_1.conda#f2465696f4396245eca4613f6e924796
+https://conda.anaconda.org/conda-forge/noarch/pytest-7.4.0-pyhd8ed1ab_0.conda#3cfe9b9e958e7238a386933c75d190db
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
 https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
 https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml-0.17.32-py38h01eb140_0.conda#c92cc8efb1341f90ea5f51f576480580
 https://conda.anaconda.org/conda-forge/linux-64/sip-6.7.9-py38h17151c0_0.conda#6a54fd42b71a8b1c5f9c4a691270cdf1
 https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.1-pyh41d4057_0.conda#3788984d535770cad699efaeb6cb3037
 https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
 https://conda.anaconda.org/conda-forge/noarch/tqdm-4.65.0-pyhd8ed1ab_1.conda#ed792aff3acb977d09c7013358097f83
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.3-hd8ed1ab_0.conda#3876f650ed7d0f95d70fa4b647621909
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.0-hd8ed1ab_0.conda#37761dccc7ca8eaa08c60c4f62eb2dcc
+https://conda.anaconda.org/conda-forge/noarch/annotated-types-0.5.0-pyhd8ed1ab_0.conda#578ae086f225bc2380c79f3b551ff2f7
 https://conda.anaconda.org/conda-forge/linux-64/argon2-cffi-bindings-21.2.0-py38h0a891b7_3.tar.bz2#efcaa056d265a3138d2038a4b6b68791
 https://conda.anaconda.org/conda-forge/linux-64/astropy-5.0.6-py38h07e1bb6_0.conda#0fcc655ae90038f1f66db3e3046d6c51
 https://conda.anaconda.org/conda-forge/linux-64/brotlipy-0.7.0-py38h0a891b7_1005.tar.bz2#e99e08812dfff30fdd17b3f8838e2759
 https://conda.anaconda.org/conda-forge/linux-64/cryptography-41.0.1-py38hcdda232_0.conda#8dc6f3a9342a870c3c927927e86aa4ad
 https://conda.anaconda.org/conda-forge/noarch/gitpython-3.1.31-pyhd8ed1ab_0.conda#f6e6b482110246a81c3f03e81c68752d
-https://conda.anaconda.org/conda-forge/linux-64/gstreamer-1.22.3-h977cf35_1.conda#410ed3b168e5a139d12ebaf4143072cd
+https://repo.anaconda.com/pkgs/main/linux-64/gstreamer-1.22.3-h5eee18b_0.conda#c2ffbb79cb2f51b042de223d482b7b29
 https://conda.anaconda.org/conda-forge/linux-64/harfbuzz-7.3.0-hdb3a94d_0.conda#765bc76c0dfaf24ff9d8a2935b2510df
 https://conda.anaconda.org/conda-forge/noarch/importlib-resources-5.12.0-pyhd8ed1ab_0.conda#3544c818f0720c89eb16ae6940ab440b
 https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.7.0-hd8ed1ab_0.conda#27a4cec373ec84d1c1aa02a1e37f8eaf
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.4.4-pyhd8ed1ab_1.conda#7c0965e1d4a0ee1529e8eaa03a78a5b3
-https://conda.anaconda.org/conda-forge/linux-64/libnetcdf-4.9.2-nompi_h0f3d0bb_105.conda#b5d412441b84305460e9df8a016a3392
+https://conda.anaconda.org/conda-forge/linux-64/libnetcdf-4.9.2-nompi_h78c856c_106.conda#47665bf3dec451455474556ecd940ed2
 https://conda.anaconda.org/conda-forge/noarch/mdit-py-plugins-0.4.0-pyhd8ed1ab_0.conda#6c5358a10873a15398b6f15f60cb5e1f
 https://conda.anaconda.org/conda-forge/linux-64/pandas-1.5.3-py38hdc8b05c_1.conda#c944b033a2126e7f714a7ecaecb22011
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.6.0-pyhd8ed1ab_0.conda#741384b21c1b512617f4ee4ea8457c5d
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.8.0-pyhd8ed1ab_0.conda#3e4aca765371893ad848397794600632
 https://conda.anaconda.org/conda-forge/noarch/pybtex-0.24.0-pyhd8ed1ab_2.tar.bz2#2099b86a7399c44c0c61cdb6de6915ba
-https://conda.anaconda.org/conda-forge/linux-64/pydantic-1.10.9-py38h01eb140_0.conda#2d8a27b52507d0ba49c938005465b5e3
+https://conda.anaconda.org/conda-forge/linux-64/pydantic-core-2.0.1-py38h0cc4f7c_0.conda#c4f9a324d600fb26bf8cf25757e382f8
 https://conda.anaconda.org/conda-forge/linux-64/pyqt5-sip-12.11.0-py38h8dc9893_3.conda#7bb0328b4a0f857aeb432426b9a5f908
 https://conda.anaconda.org/conda-forge/noarch/pytest-metadata-3.0.0-pyhd8ed1ab_1.conda#8bdcc0f401561213821bf67513abeeff
 https://conda.anaconda.org/conda-forge/noarch/python-build-0.10.0-pyhd8ed1ab_1.conda#0ab47ce574f6a8bcb9f2076436e7fedb
 https://conda.anaconda.org/conda-forge/noarch/rich-13.4.2-pyhd8ed1ab_0.conda#f993baacc175e83fafd6b846e9c4c8a2
 https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
-https://conda.anaconda.org/conda-forge/linux-64/gst-plugins-base-1.22.3-h938bd60_1.conda#1f317eb7f00db75f4112a07476345376
-https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.2.0-pyhd8ed1ab_0.conda#58ca2d50c3b27b86fd7df62eaadbf9a9
+https://repo.anaconda.com/pkgs/main/linux-64/gst-plugins-base-1.22.3-he621ea3_0.conda#27be67671dce7d6d8c53bf6260090c15
+https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda#1d018ee4ab13217e2544f795eb0a6798
 https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
 https://conda.anaconda.org/conda-forge/linux-64/matplotlib-base-3.7.1-py38hd6c3c57_0.conda#3b8ba76acae09fbd4b2247c4ee4c0324
 https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.0-pyhd8ed1ab_0.conda#f525a01528c3eba1d381a232a6971c6a
-https://conda.anaconda.org/conda-forge/linux-64/netcdf4-1.6.4-nompi_py38hdfa7aa7_100.conda#ce30178fb90d4509c3fda5b572124200
-https://conda.anaconda.org/conda-forge/noarch/pip-tools-6.13.0-pyhd8ed1ab_1.conda#566e41c99730f1124d6948ab8fe1c18d
+https://conda.anaconda.org/conda-forge/linux-64/netcdf4-1.6.4-nompi_py38h383a0a3_101.conda#693cbd2ee4f62c8a2521cfaf7560b647
+https://conda.anaconda.org/conda-forge/noarch/pip-tools-6.14.0-pyhd8ed1ab_0.conda#4c3828f6213d5ddba2f5033d4b422d17
 https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
 https://conda.anaconda.org/conda-forge/linux-64/pybtex-docutils-1.0.2-py38h578d9bd_2.tar.bz2#178c840a19be1a4c809798a73b285d27
+https://conda.anaconda.org/conda-forge/linux-64/pydantic-2.0-py38h01eb140_0.conda#453742dca59531095a6a6aae78665c81
 https://conda.anaconda.org/conda-forge/noarch/pyopenssl-23.2.0-pyhd8ed1ab_1.conda#34f7d568bf59d18e3fef8c405cbece21
 https://conda.anaconda.org/conda-forge/noarch/pytest-json-report-1.5.0-pyhd8ed1ab_0.tar.bz2#837e335fa428cf7c784ee2e80594506c
 https://conda.anaconda.org/conda-forge/linux-64/secretstorage-3.3.3-py38h578d9bd_1.tar.bz2#7ff0f00ee67fcbccbae548be59bfae77
 https://conda.anaconda.org/conda-forge/noarch/typer-0.9.0-pyhd8ed1ab_0.conda#5030a13b2fe5e143d5956d4943d3018f
 https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.23.1-pyhd8ed1ab_0.conda#838b85f656b078bdd882ef97978e7f40
 https://conda.anaconda.org/conda-forge/noarch/xarray-2023.1.0-pyhd8ed1ab_0.conda#c11eb03b6f77a0d22ae88c454c940f55
-https://conda.anaconda.org/conda-forge/linux-64/keyring-23.13.1-py38h578d9bd_0.conda#713b14390d450db02fea6b0c0535d67a
+https://conda.anaconda.org/conda-forge/linux-64/keyring-24.2.0-py38h578d9bd_0.conda#886a052bb649eff357b194d6005052cf
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.8.0-pyhd8ed1ab_0.conda#e78da91cf428faaf05701ce8cc8f2f9b
 https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.38-hd8ed1ab_0.conda#45b74f64d8808eda7e6f6e6b1d641fd2
 https://conda.anaconda.org/conda-forge/linux-64/qt-main-5.15.8-h01ceb2d_12.conda#60fd4bdf187f88bac57cdc1a052f2811
 https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.15-pyhd8ed1ab_0.conda#27db656619a55d727eaf5a6ece3d2fd6
 https://conda.anaconda.org/conda-forge/noarch/ipython-8.12.0-pyh41d4057_0.conda#e89d0c5836e45f9e6a66c5c24fc9ef35
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.6.0-pyhd8ed1ab_0.conda#879782bde4bbdb4c7b5d4054504a20d5
 https://conda.anaconda.org/conda-forge/linux-64/pyqt-5.15.7-py38ha0d8c90_3.conda#e965dc172d67920d058ac2b3a0e27565
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/noarch/cachecontrol-0.13.0-pyhd8ed1ab_0.conda#9f0b2eb5f5dd2cec36d5342a80adfec0
 https://conda.anaconda.org/conda-forge/noarch/ensureconda-1.4.3-pyhd8ed1ab_0.tar.bz2#c99ae3abf501990769047b4b40a98f17
-https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.1-pyh210e3f2_0.conda#4b57b688e22d094d1479a35543c18e93
-https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.6.0-pyhd8ed1ab_0.conda#39fd52b0fcb2fb52bac47a1419bf09bd
+https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.3-pyh71e2992_0.conda#482f0176a89f14e10a7d15f9f1980e36
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.7.0-pyhd8ed1ab_0.conda#7488cd1f4d35a2af96faa765b7e5b2f0
 https://conda.anaconda.org/conda-forge/linux-64/matplotlib-3.7.1-py38h578d9bd_0.conda#50ff9e0a3dd459a0ca365741072bf9a2
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.6.0-pyhd8ed1ab_0.conda#e8172ca42f2869bb90185c9356899e81
 https://conda.anaconda.org/conda-forge/noarch/pooch-1.7.0-pyha770c72_3.conda#5936894aade8240c867d292aa0d980c6
 https://conda.anaconda.org/conda-forge/noarch/sphinx-5.0.0-pyh6c4a22f_1.tar.bz2#a7cc4b9c94548ff9a19b368f975e5404
 https://conda.anaconda.org/conda-forge/noarch/autodocsumm-0.2.11-pyhd8ed1ab_0.conda#547c48372c97c463c93af86d7f2c868c
 https://conda.anaconda.org/conda-forge/noarch/cachecontrol-with-filecache-0.13.0-pyhd8ed1ab_0.conda#3fd3d55ea862cc0736ac1cce6f44c2d1
 https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.6-pyhd8ed1ab_0.conda#68627a08556e4a273e4c7bfc84251457
```

### Comparing `eradiate-0.23.2rc3/requirements/conda/environment-optional-osx-64.lock` & `eradiate-0.23.2rc4/requirements/conda/environment-optional-osx-64.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 # Generated by conda-lock.
 # platform: osx-64
-# input_hash: bf11f624e722c74ec0e342583ae0fcb21524c22ae8ca653349f3b25602fab72a
+# input_hash: 7698d8dd9c55c8170544c99f0bbcc0e151b7ed643f053944f557aef5d422032c
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h0d85af4_4.tar.bz2#37edc4e6304ca87316e160f5ca0bd1b5
 https://conda.anaconda.org/conda-forge/osx-64/c-ares-1.19.1-h0dc2134_0.conda#b3e62631b4e1b9801477523ce1d6f355
 https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2023.5.7-h8857fd0_0.conda#b704e4b79ba0d887c4870b7b09d6a4df
 https://conda.anaconda.org/conda-forge/osx-64/icu-72.1-h7336db1_0.conda#c9689510a50a4bb2ae978421671a125e
-https://conda.anaconda.org/conda-forge/osx-64/libbrotlicommon-1.0.9-hb7f2c08_8.tar.bz2#37157d273eaf3bc7d6862104161d9ec9
+https://conda.anaconda.org/conda-forge/osx-64/libbrotlicommon-1.0.9-hb7f2c08_9.conda#ee1ee8c79c3426229ad03290573be552
 https://conda.anaconda.org/conda-forge/osx-64/libcxx-16.0.6-hd57cbcb_0.conda#7d6972792161077908b62971802f289a
 https://conda.anaconda.org/conda-forge/osx-64/libdeflate-1.18-hac1461d_0.conda#3d131584456b277ce0871e6481fde49b
 https://conda.anaconda.org/conda-forge/osx-64/libev-4.33-haf1e3a3_1.tar.bz2#79dc2be110b2a3d1e97ec21f691c50ad
 https://conda.anaconda.org/conda-forge/osx-64/libffi-3.4.2-h0d85af4_5.tar.bz2#ccb34fb14960ad8b125962d3d79b31a9
 https://conda.anaconda.org/conda-forge/osx-64/libiconv-1.17-hac89ed1_0.tar.bz2#691d103d11180486154af49c037b7ed9
 https://conda.anaconda.org/conda-forge/osx-64/libjpeg-turbo-2.1.5.1-hb7f2c08_0.conda#d7309a152b9b79799063b8bb47e34a3a
 https://conda.anaconda.org/conda-forge/osx-64/libsodium-1.0.18-hbcb3906_1.tar.bz2#24632c09ed931af617fe6d5292919cab
-https://conda.anaconda.org/conda-forge/osx-64/libwebp-base-1.3.0-hb7f2c08_0.conda#18981e4c840126d6118d8952485fea51
+https://conda.anaconda.org/conda-forge/osx-64/libwebp-base-1.3.1-h0dc2134_0.conda#a25a41b5be3fed4b671a58b998dcf89b
 https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-h8a1eda9_5.conda#4a3ad23f6e16f99c04e166767193d700
 https://conda.anaconda.org/conda-forge/osx-64/llvm-openmp-16.0.6-hff08bdf_0.conda#39a5227d906f75102bf8586741690128
 https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.4-hf0c8a7f_0.conda#c3dbae2411164d9b02c69090a9a91857
 https://conda.anaconda.org/conda-forge/osx-64/pthread-stubs-0.4-hc929b4f_1001.tar.bz2#addd19059de62181cd11ae8f4ef26084
 https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.8-3_cp38.conda#ff192f59f7fe23555612030493a079f8
 https://conda.anaconda.org/conda-forge/osx-64/xorg-libxau-1.0.11-h0dc2134_0.conda#9566b4c29274125b0266d0177b5eb97b
 https://conda.anaconda.org/conda-forge/osx-64/xorg-libxdmcp-1.1.3-h35c211d_0.tar.bz2#86ac76d6bf1cbb9621943eb3bd9ae36e
 https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2#a72f9d4ea13d55d745ff1ed594747f10
 https://conda.anaconda.org/conda-forge/osx-64/yaml-0.2.5-h0d85af4_2.tar.bz2#d7e08fcf8259d742156188e8762b4d20
 https://conda.anaconda.org/conda-forge/osx-64/hdf4-4.2.15-h9804679_6.conda#c13d8841112ba7f5931d1d60631394f3
 https://conda.anaconda.org/conda-forge/osx-64/lerc-4.0.0-hb486fe8_0.tar.bz2#f9d6a4c82889d5ecedec1d90eb673c55
 https://conda.anaconda.org/conda-forge/osx-64/libaec-1.0.6-hf0c8a7f_1.conda#7c0f82f435ab4c48d65dc9b28db2ad9e
-https://conda.anaconda.org/conda-forge/osx-64/libbrotlidec-1.0.9-hb7f2c08_8.tar.bz2#7f952a036d9014b4dab96c6ea0f8c2a7
-https://conda.anaconda.org/conda-forge/osx-64/libbrotlienc-1.0.9-hb7f2c08_8.tar.bz2#b36a3bfe866d9127f25f286506982166
+https://conda.anaconda.org/conda-forge/osx-64/libbrotlidec-1.0.9-hb7f2c08_9.conda#4043ef9fe42e178785e0e1853b79bdf9
+https://conda.anaconda.org/conda-forge/osx-64/libbrotlienc-1.0.9-hb7f2c08_9.conda#b64d4dcc70aa141db7fccbf13bad81e1
 https://conda.anaconda.org/conda-forge/osx-64/libedit-3.1.20191231-h0678c8f_2.tar.bz2#6016a8a1d0e63cac3de2c352cd40208b
 https://conda.anaconda.org/conda-forge/osx-64/libgfortran5-12.2.0-he409387_31.conda#5a544130e584b1f204ac896ff071d5b3
 https://conda.anaconda.org/conda-forge/osx-64/libpng-1.6.39-ha978bb4_0.conda#35e4928794c5391aec14ffdf1deaaee5
 https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.42.0-h58db7d2_0.conda#a7d3b44b7b0c9901ac7813b7a0462893
 https://conda.anaconda.org/conda-forge/osx-64/libxcb-1.15-hb7f2c08_0.conda#5513f57e0238c87c12dffedbcc9c1a4a
 https://conda.anaconda.org/conda-forge/osx-64/libxml2-2.11.4-hd95e348_0.conda#681f8dda25e73a830d774a37b9839c85
 https://conda.anaconda.org/conda-forge/osx-64/lz4-c-1.9.4-hf0c8a7f_0.conda#aa04f7143228308662696ac24023f991
@@ -40,32 +40,32 @@
 https://conda.anaconda.org/conda-forge/osx-64/pandoc-3.1.3-h9d075a6_0.conda#e86a3d5c966a09b6129354114483f7a7
 https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda#f17f77f2acf4d344734bda76829ce14e
 https://conda.anaconda.org/conda-forge/osx-64/snappy-1.1.10-h225ccf5_0.conda#4320a8781f14cd959689b86e349f3b73
 https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.12-h5dbffcc_0.tar.bz2#8e9480d9c47061db2ed1b4ecce519a7f
 https://conda.anaconda.org/conda-forge/osx-64/zeromq-4.3.4-he49afe7_1.tar.bz2#1972d732b123ed04b60fd21e94f0b178
 https://conda.anaconda.org/conda-forge/osx-64/zstd-1.5.2-hbc0c0cd_6.conda#40a188783d3c425bdccc9ae9104acbb8
 https://conda.anaconda.org/conda-forge/osx-64/blosc-1.21.4-heccf04b_0.conda#02e92eb72b9ae4c1745b95d03a9c949e
-https://conda.anaconda.org/conda-forge/osx-64/brotli-bin-1.0.9-hb7f2c08_8.tar.bz2#aac5ad0d8f747ef7f871508146df75d9
+https://conda.anaconda.org/conda-forge/osx-64/brotli-bin-1.0.9-hb7f2c08_9.conda#72c526f7ffa265473e6c75fd90605e52
 https://conda.anaconda.org/conda-forge/osx-64/freetype-2.12.1-h3f81eb7_1.conda#852224ea3e8991a8342228eab274840e
 https://conda.anaconda.org/conda-forge/osx-64/krb5-1.20.1-h049b76e_0.conda#db11fa2968ef0837288fe2d7f5b77a50
 https://conda.anaconda.org/conda-forge/osx-64/libgfortran-5.0.0-11_3_0_h97931a8_31.conda#97451338600bd9c5b535eb224ef6c471
 https://conda.anaconda.org/conda-forge/osx-64/libnghttp2-1.52.0-he2ab024_0.conda#12ac7d100bf260263e30a019517f42a2
 https://conda.anaconda.org/conda-forge/osx-64/libssh2-1.11.0-hd019ec5_0.conda#ca3a72efba692c59a90d4b9fc0dfe774
 https://conda.anaconda.org/conda-forge/osx-64/libtiff-4.5.1-hf955e92_0.conda#56523ed556e3a44c0fd55bcf17045892
 https://conda.anaconda.org/conda-forge/osx-64/libzip-1.9.2-h6db710c_1.tar.bz2#ce732d37e479919f3d22b1ccdeb858ac
 https://conda.anaconda.org/conda-forge/osx-64/python-3.8.17-hf9b03c3_0_cpython.conda#f613b663d3829f325b4ffb626bf612b6
 https://conda.anaconda.org/eradiate/noarch/aabbtree-2.8.0-py_0.tar.bz2#647bcce5f0af4974e507591d5420486b
-https://conda.anaconda.org/conda-forge/noarch/aenum-3.1.12-pyhd8ed1ab_0.conda#602716538da00b2ca3cc85c4d35c0245
+https://conda.anaconda.org/conda-forge/noarch/aenum-3.1.15-pyhd8ed1ab_0.conda#24cff7ab050ebb8a16bdeb02e8ed6f63
 https://conda.anaconda.org/conda-forge/noarch/alabaster-0.7.13-pyhd8ed1ab_0.conda#06006184e203b61d3525f90de394471e
 https://conda.anaconda.org/conda-forge/noarch/appdirs-1.4.4-pyh9f0ad1d_0.tar.bz2#5f095bc6454094e96f146491fd03633b
 https://conda.anaconda.org/conda-forge/noarch/appnope-0.1.3-pyhd8ed1ab_0.tar.bz2#54ac328d703bff191256ffa1183126d1
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
-https://conda.anaconda.org/conda-forge/osx-64/brotli-1.0.9-hb7f2c08_8.tar.bz2#55f612fe4a9b5f6ac76348b6de94aaeb
+https://conda.anaconda.org/conda-forge/osx-64/brotli-1.0.9-hb7f2c08_9.conda#53cff90f0cea22e13e5b791f0e5a8e7d
 https://conda.anaconda.org/conda-forge/noarch/cachy-0.3.0-pyhd8ed1ab_1.tar.bz2#5dfee17f24e2dfd18d7392b48c9351e2
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
 https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-unix_pyhd8ed1ab_2.tar.bz2#20e4087407c7cb04a40817114b333dbf
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/noarch/crashtest-0.4.1-pyhd8ed1ab_0.tar.bz2#709a2295dd907bb34afb57d54320642f
 https://conda.anaconda.org/conda-forge/noarch/cycler-0.11.0-pyhd8ed1ab_0.tar.bz2#a50559fad0affdbb33729a68669ca1cb
@@ -79,15 +79,15 @@
 https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
 https://conda.anaconda.org/conda-forge/noarch/executing-1.2.0-pyhd8ed1ab_0.tar.bz2#4c1bc140e2be5c8ba6e3acab99e25c50
 https://conda.anaconda.org/conda-forge/noarch/filelock-3.12.2-pyhd8ed1ab_0.conda#53522ec72e6adae42bd373ef58357230
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/imagesize-1.4.1-pyhd8ed1ab_0.tar.bz2#7de5386c8fea29e76b303f37dde4c352
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda#f800d2da156d08e289b14e87e43c1ae5
-https://conda.anaconda.org/conda-forge/noarch/json5-0.9.5-pyh9f0ad1d_0.tar.bz2#10759827a94e6b14996e81fb002c0bda
+https://conda.anaconda.org/conda-forge/noarch/json5-0.9.14-pyhd8ed1ab_0.conda#dac1dabba2b5a9d1aee175c5fcc7b436
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.7-pyhd8ed1ab_1.conda#0c0a54e16b764bafcae35913cc9d60ff
 https://conda.anaconda.org/conda-forge/osx-64/kiwisolver-1.4.4-py38h98b9b1b_1.tar.bz2#c11eff21a36bc5809b8e23a05ee71df8
 https://conda.anaconda.org/conda-forge/noarch/lazy_loader-0.2-pyhd8ed1ab_0.conda#d060d017720c9882c4eca0544a4a0592
 https://conda.anaconda.org/conda-forge/osx-64/lcms2-2.15-h2dcdeff_1.conda#f1df9b0c2d9fbe985e62f4b24773a9e4
 https://conda.anaconda.org/conda-forge/osx-64/libcurl-8.1.2-hbee3ae8_0.conda#d51e337da844262f9033c9a26452520f
 https://conda.anaconda.org/conda-forge/osx-64/libopenblas-0.3.23-openmp_h429af6e_0.conda#7000a828e29608e4f57e662b5502d2c9
 https://conda.anaconda.org/conda-forge/noarch/lockfile-0.12.2-py_1.tar.bz2#c104d98e09c47519950cffb8dd5b4f10
@@ -104,15 +104,15 @@
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/parso-0.8.3-pyhd8ed1ab_0.tar.bz2#17a565a0c3899244e938cdf417e7b094
 https://conda.anaconda.org/conda-forge/noarch/pastel-0.2.1-pyhd8ed1ab_0.tar.bz2#a4eea5bff523f26442405bc5d1f52adb
 https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
 https://conda.anaconda.org/conda-forge/noarch/pint-0.21-pyhd8ed1ab_0.conda#8d7b829e37d78447569c180f9d827005
 https://conda.anaconda.org/conda-forge/noarch/pkginfo-1.9.6-pyhd8ed1ab_0.conda#be1e9f1c65a1ed0f2ae9352fec99db64
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2#89e3c7cdde7d3aaa2aee933b604dd07f
-https://conda.anaconda.org/conda-forge/noarch/pluggy-1.0.0-pyhd8ed1ab_5.tar.bz2#7d301a0d25f424d96175f810935f0da9
+https://conda.anaconda.org/conda-forge/noarch/pluggy-1.2.0-pyhd8ed1ab_0.conda#7263924c642d22e311d9e59b839f1b33
 https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.0-pyhd8ed1ab_0.conda#95c5be3c7cbd872509d16c216617fdab
 https://conda.anaconda.org/conda-forge/osx-64/psutil-5.9.5-py38hef030d1_0.conda#20b4cc7adae881327b943c883be6335e
 https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2#359eeb6536da0e687af562ed265ec263
 https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2#6784285c7e55cb7212efabc79e4c2883
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
 https://conda.anaconda.org/conda-forge/noarch/pylev-1.4.0-pyhd8ed1ab_0.tar.bz2#edf8651c4379d9d1495ad6229622d150
@@ -122,15 +122,15 @@
 https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.17.1-pyhd8ed1ab_0.conda#dd4f393d857e9283eef2442234bd05e3
 https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.7-pyhd8ed1ab_0.conda#a61bf9ec79426938ff785eb69dbb1960
 https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
 https://conda.anaconda.org/conda-forge/osx-64/pyyaml-6.0-py38hef030d1_5.tar.bz2#e27d698dc29c6d5b49f1385bcd1d50f9
 https://conda.anaconda.org/conda-forge/osx-64/pyzmq-25.1.0-py38h3b70857_0.conda#a48761bc98b3bc22d209e9bb2f3dc5c1
 https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2#912a71cc01012ee38e6b90ddd561e36f
 https://conda.anaconda.org/conda-forge/osx-64/ruamel.yaml.clib-0.2.7-py38hef030d1_1.conda#9a8e866b0680b61b2e988b18a1eaecae
-https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda#3b68bc43ec6baa48f7354a446267eefe
+https://conda.anaconda.org/conda-forge/noarch/setuptools-68.0.0-pyhd8ed1ab_0.conda#5a7739d0f57ee64133c9d32e6507c46d
 https://conda.anaconda.org/conda-forge/noarch/shellingham-1.4.0-pyh44b312d_0.tar.bz2#437655338696f9d0dfdb0a024e66b255
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/smmap-3.0.5-pyh44b312d_0.tar.bz2#3a8dc70789709aa315325d5df06fb7e4
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
 https://conda.anaconda.org/conda-forge/noarch/snowballstemmer-2.2.0-pyhd8ed1ab_0.tar.bz2#4d22a9315e78c6827f806065957d566e
 https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
@@ -141,128 +141,130 @@
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-qthelp-1.0.3-py_0.tar.bz2#d01180388e6d1838c3e1ad029590aa7a
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-serializinghtml-1.1.5-pyhd8ed1ab_2.tar.bz2#9ff55a0901cf952f05c654394de76bf7
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.11.8-pyha770c72_0.conda#75838e8556166263a82038b51d01d5f1
 https://conda.anaconda.org/conda-forge/noarch/toolz-0.12.0-pyhd8ed1ab_0.tar.bz2#92facfec94bc02d6ccf42e7173831a36
 https://conda.anaconda.org/conda-forge/osx-64/tornado-6.3.2-py38hcafd530_0.conda#afefcf665a5049b030efb084a51e3935
 https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.3-pyha770c72_0.conda#4a3014a4d107d15475d106b751c4e352
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.0-pyha770c72_0.conda#c76ebd4731d3668ba16975a30ef19d0d
 https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/osx-64/unicodedata2-15.0.0-py38hef030d1_0.tar.bz2#51020c740c53f14657f6307b9eb23f85
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
-https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.0-pyhd8ed1ab_0.conda#1dd6387a73d84e16b6f73de676bb4c36
+https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda#c34d9325a609381a0b0e8a5b4f325147
 https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
 https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.7-pyhd8ed1ab_0.conda#bcc54b91a8ce88f60f538b87b409909e
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
 https://conda.anaconda.org/conda-forge/noarch/accessible-pygments-0.0.4-pyhd8ed1ab_0.conda#46a2e6e3dfa718ce3492018d5a110dd6
 https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.0-pyhd8ed1ab_1.conda#2b35a85d654a47aac8f34c1bb6de7142
 https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
 https://conda.anaconda.org/conda-forge/noarch/async-lru-2.0.2-pyhd8ed1ab_0.conda#41221f97a0c82e5a60b21716a3d7469c
 https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
-https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.4-pyhd8ed1ab_0.tar.bz2#c5b3edc62d6309088f4970b3eaaa65a6
+https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda#6b1b907661838a75d067a22f87996b2e
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
 https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda#d48b143d01385872a88ef8417e96c30e
 https://conda.anaconda.org/conda-forge/osx-64/cffi-1.15.1-py38hb368cf1_3.conda#a2b3ae2a1fd2aea0b4433d9e7fff8cf3
 https://conda.anaconda.org/conda-forge/noarch/click-default-group-1.2.2-pyhd8ed1ab_1.tar.bz2#72a46ffc25701c173932fd55cf0965d3
 https://conda.anaconda.org/conda-forge/noarch/clikit-0.6.2-pyhd8ed1ab_2.conda#02abb7b66b02e8b9f5a9b05454400087
 https://conda.anaconda.org/conda-forge/noarch/comm-0.1.3-pyhd8ed1ab_0.conda#168ae0f82cdf7505048e81054c7354e4
 https://conda.anaconda.org/conda-forge/osx-64/curl-8.1.2-hbee3ae8_0.conda#6cc301a6c2ba26e29949818efdc133ca
 https://conda.anaconda.org/eradiate/noarch/dessinemoi-23.1.0-py_0.tar.bz2#490780e63e113a7dc444bd068e049bfe
 https://conda.anaconda.org/conda-forge/noarch/environ-config-22.1.0-pyhd8ed1ab_0.tar.bz2#a1103faffa0a877313c1fba776aa0fc0
 https://conda.anaconda.org/conda-forge/osx-64/fonttools-4.40.0-py38hcafd530_0.conda#b26b38c5f75e03e86cecf860ca9fb1cd
 https://conda.anaconda.org/conda-forge/noarch/gitdb-4.0.10-pyhd8ed1ab_0.conda#3706d2f3d7cb5dae600c833345a76132
-https://conda.anaconda.org/conda-forge/osx-64/hdf5-1.14.0-nompi_hbf0aa07_103.conda#90f50d124606a4e62628823b614a2f4c
+https://conda.anaconda.org/conda-forge/osx-64/hdf5-1.14.1-nompi_hedada53_100.conda#033c310c83abbd9c2f9a5c13b9f54225
 https://conda.anaconda.org/conda-forge/noarch/html5lib-1.1-pyh9f0ad1d_0.tar.bz2#b2355343d6315c892543200231d7154a
 https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.7.0-pyha770c72_0.conda#ba3786c6846e46038fe60c785d46dc81
 https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
 https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.2.3-pyhd8ed1ab_0.tar.bz2#31e4a1506968d017229bdb64695013a1
 https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.2.2-pyhd8ed1ab_0.tar.bz2#243f63592c8e449f40cd42eb5cf32f40
 https://conda.anaconda.org/conda-forge/noarch/latexcodec-2.0.1-pyh9f0ad1d_0.tar.bz2#8d67904973263afd2985ba56aa2d6bb4
 https://conda.anaconda.org/conda-forge/osx-64/libblas-3.9.0-17_osx64_openblas.conda#65299527582e2449b05d27fcf8352125
 https://conda.anaconda.org/conda-forge/noarch/livereload-2.6.3-pyh9f0ad1d_0.tar.bz2#b7190e3ec3eff52839434bf4698e2d62
 https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-2.2.0-pyhd8ed1ab_0.conda#b2928a6c6d52d7e3562b4a59c3214e3a
 https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
 https://conda.anaconda.org/conda-forge/noarch/overrides-7.3.1-pyhd8ed1ab_0.tar.bz2#a5745ced46e69aa9754053ba061974ab
 https://conda.anaconda.org/conda-forge/noarch/pexpect-4.8.0-pyh1a96a4e_2.tar.bz2#330448ce4403cc74990ac07c555942a1
-https://conda.anaconda.org/conda-forge/osx-64/pillow-9.5.0-py38h16710f9_1.conda#c5bf174a033ef668679cc80918422515
+https://conda.anaconda.org/conda-forge/osx-64/pillow-10.0.0-py38h16710f9_0.conda#8f73f0573ab381d56588e001754c53d3
 https://conda.anaconda.org/eradiate/noarch/pinttrs-23.2.0-py_0.tar.bz2#1aebe9fa813278f719fa8e31d8000452
 https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
 https://conda.anaconda.org/conda-forge/noarch/portion-2.4.0-pyhd8ed1ab_0.conda#9d34bac22e169b41f4e34525a140c13b
 https://conda.anaconda.org/conda-forge/osx-64/pyobjc-core-9.2-py38h095c2e5_0.conda#8dbb4798b2066b678d8da47734d1c763
 https://conda.anaconda.org/conda-forge/noarch/pyproject_hooks-1.0.0-pyhd8ed1ab_0.conda#21de50391d584eb7f4441b9de1ad773f
-https://conda.anaconda.org/conda-forge/noarch/pytest-7.3.2-pyhd8ed1ab_1.conda#f2465696f4396245eca4613f6e924796
+https://conda.anaconda.org/conda-forge/noarch/pytest-7.4.0-pyhd8ed1ab_0.conda#3cfe9b9e958e7238a386933c75d190db
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
 https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
 https://conda.anaconda.org/conda-forge/osx-64/ruamel.yaml-0.17.32-py38hcafd530_0.conda#cb301e0b2b162330bc3b03fe51ea0d15
 https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.1-pyhd1c38e8_0.conda#046120b71d8896cb7faef78bfdbfee1e
 https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
 https://conda.anaconda.org/conda-forge/noarch/tqdm-4.65.0-pyhd8ed1ab_1.conda#ed792aff3acb977d09c7013358097f83
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.3-hd8ed1ab_0.conda#3876f650ed7d0f95d70fa4b647621909
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.0-hd8ed1ab_0.conda#37761dccc7ca8eaa08c60c4f62eb2dcc
+https://conda.anaconda.org/conda-forge/noarch/annotated-types-0.5.0-pyhd8ed1ab_0.conda#578ae086f225bc2380c79f3b551ff2f7
 https://conda.anaconda.org/conda-forge/osx-64/argon2-cffi-bindings-21.2.0-py38hef030d1_3.tar.bz2#fc1bc20add8eff07c367973bba25e8eb
 https://conda.anaconda.org/conda-forge/osx-64/brotlipy-0.7.0-py38hef030d1_1005.tar.bz2#2fa6826f6f94c847bf26709f2162a09c
 https://conda.anaconda.org/conda-forge/osx-64/cryptography-41.0.1-py38he13da33_0.conda#845f16b2278f26769e23796d04636e06
 https://conda.anaconda.org/conda-forge/noarch/gitpython-3.1.31-pyhd8ed1ab_0.conda#f6e6b482110246a81c3f03e81c68752d
 https://conda.anaconda.org/conda-forge/noarch/importlib-resources-5.12.0-pyhd8ed1ab_0.conda#3544c818f0720c89eb16ae6940ab440b
 https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.7.0-hd8ed1ab_0.conda#27a4cec373ec84d1c1aa02a1e37f8eaf
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.4.4-pyhd8ed1ab_1.conda#7c0965e1d4a0ee1529e8eaa03a78a5b3
 https://conda.anaconda.org/conda-forge/osx-64/libcblas-3.9.0-17_osx64_openblas.conda#380151ca00704172b242a63701b7bf8a
 https://conda.anaconda.org/conda-forge/osx-64/liblapack-3.9.0-17_osx64_openblas.conda#6ab83532872bf3659613638589dd10af
-https://conda.anaconda.org/conda-forge/osx-64/libnetcdf-4.9.2-nompi_hf077d52_105.conda#64d626e024a284777458e2b315e9eb56
+https://conda.anaconda.org/conda-forge/osx-64/libnetcdf-4.9.2-nompi_hfeda9e8_106.conda#66108519efbf30b02632ad35f519773f
 https://conda.anaconda.org/conda-forge/noarch/mdit-py-plugins-0.4.0-pyhd8ed1ab_0.conda#6c5358a10873a15398b6f15f60cb5e1f
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.6.0-pyhd8ed1ab_0.conda#741384b21c1b512617f4ee4ea8457c5d
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.8.0-pyhd8ed1ab_0.conda#3e4aca765371893ad848397794600632
 https://conda.anaconda.org/conda-forge/noarch/pybtex-0.24.0-pyhd8ed1ab_2.tar.bz2#2099b86a7399c44c0c61cdb6de6915ba
-https://conda.anaconda.org/conda-forge/osx-64/pydantic-1.10.9-py38hcafd530_0.conda#253819655b95aedbeddf0ff7fa26cf16
+https://conda.anaconda.org/conda-forge/osx-64/pydantic-core-2.0.1-py38h7510fb3_0.conda#85a94a4914e522e379c1c36cb38923a1
 https://conda.anaconda.org/conda-forge/osx-64/pyobjc-framework-cocoa-9.2-py38h095c2e5_0.conda#fa3e3307ff143e7a9e823ce7bbc916ad
 https://conda.anaconda.org/conda-forge/noarch/pytest-metadata-3.0.0-pyhd8ed1ab_1.conda#8bdcc0f401561213821bf67513abeeff
 https://conda.anaconda.org/conda-forge/noarch/python-build-0.10.0-pyhd8ed1ab_1.conda#0ab47ce574f6a8bcb9f2076436e7fedb
 https://conda.anaconda.org/conda-forge/noarch/rich-13.4.2-pyhd8ed1ab_0.conda#f993baacc175e83fafd6b846e9c4c8a2
 https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
 https://conda.anaconda.org/conda-forge/osx-64/jupyter_core-5.3.1-py38h50d1736_0.conda#03a3619e222793567b29b5966c2a821d
 https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
-https://conda.anaconda.org/conda-forge/osx-64/keyring-23.13.1-py38h50d1736_0.conda#7ba9ac4c5edbaddcffe213189e679b13
-https://conda.anaconda.org/conda-forge/osx-64/numpy-1.24.3-py38h9a4a08f_0.conda#5ff64b8133dea66865fe1bd35fb1d6d6
-https://conda.anaconda.org/conda-forge/noarch/pip-tools-6.13.0-pyhd8ed1ab_1.conda#566e41c99730f1124d6948ab8fe1c18d
+https://conda.anaconda.org/conda-forge/osx-64/keyring-24.2.0-py38h50d1736_0.conda#150c457dbd44f1b53e77ebf98a1680ec
+https://conda.anaconda.org/conda-forge/osx-64/numpy-1.24.4-py38h9a4a08f_0.conda#85debc55a30068d6bb76a6deaf599afa
+https://conda.anaconda.org/conda-forge/noarch/pip-tools-6.14.0-pyhd8ed1ab_0.conda#4c3828f6213d5ddba2f5033d4b422d17
 https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
 https://conda.anaconda.org/conda-forge/osx-64/pybtex-docutils-1.0.2-py38h50d1736_2.tar.bz2#5650c819d7ae44ff91c456370f175706
+https://conda.anaconda.org/conda-forge/osx-64/pydantic-2.0-py38hcafd530_0.conda#475d41478cd6aa73a1d0930fdee989ab
 https://conda.anaconda.org/conda-forge/noarch/pyopenssl-23.2.0-pyhd8ed1ab_1.conda#34f7d568bf59d18e3fef8c405cbece21
 https://conda.anaconda.org/conda-forge/noarch/pytest-json-report-1.5.0-pyhd8ed1ab_0.tar.bz2#837e335fa428cf7c784ee2e80594506c
 https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyhd1c38e8_0.conda#2657c3de5371c571aef6678afb4aaadd
 https://conda.anaconda.org/conda-forge/noarch/typer-0.9.0-pyhd8ed1ab_0.conda#5030a13b2fe5e143d5956d4943d3018f
 https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.23.1-pyhd8ed1ab_0.conda#838b85f656b078bdd882ef97978e7f40
 https://conda.anaconda.org/conda-forge/osx-64/cftime-1.6.2-py38hbd87e4b_1.tar.bz2#6b61efa56393b9655334192cc5423659
 https://conda.anaconda.org/conda-forge/osx-64/contourpy-1.1.0-py38h15a1a5b_0.conda#30d645ffb3572a3875e6fc8687857182
-https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.2.0-pyhd8ed1ab_0.conda#58ca2d50c3b27b86fd7df62eaadbf9a9
+https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda#1d018ee4ab13217e2544f795eb0a6798
 https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.0-pyhd8ed1ab_0.conda#f525a01528c3eba1d381a232a6971c6a
 https://conda.anaconda.org/conda-forge/osx-64/pandas-1.5.3-py38hec72209_1.conda#a8f001ab0a7c6312cea020bd20689765
 https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.38-hd8ed1ab_0.conda#45b74f64d8808eda7e6f6e6b1d641fd2
 https://conda.anaconda.org/conda-forge/osx-64/pyerfa-2.0.0.3-py38hbd87e4b_0.conda#48a43c20176ae9fba912e9142bc066ad
 https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.15-pyhd8ed1ab_0.conda#27db656619a55d727eaf5a6ece3d2fd6
 https://conda.anaconda.org/conda-forge/osx-64/astropy-5.0.6-py38h073b4c8_0.conda#d2955fea4da9c60ab73746c1d7e588bb
 https://conda.anaconda.org/conda-forge/noarch/ipython-8.12.0-pyhd1c38e8_0.conda#4b25de6cd2891e6bce87de8c5d85e27c
 https://conda.anaconda.org/conda-forge/osx-64/matplotlib-base-3.7.1-py38hcb346ec_0.conda#1f1eea98c232c8ef720175e12b00d0c4
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.8.0-pyhd8ed1ab_0.conda#e78da91cf428faaf05701ce8cc8f2f9b
-https://conda.anaconda.org/conda-forge/osx-64/netcdf4-1.6.4-nompi_py38h47ac6a0_100.conda#f86d4df9f8f46ae6d0c29bb87fe093b0
+https://conda.anaconda.org/conda-forge/osx-64/netcdf4-1.6.4-nompi_py38ha129777_101.conda#0e0f917d6168b9744a407d5ef3c2cb09
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/noarch/xarray-2023.1.0-pyhd8ed1ab_0.conda#c11eb03b6f77a0d22ae88c454c940f55
 https://conda.anaconda.org/conda-forge/noarch/cachecontrol-0.13.0-pyhd8ed1ab_0.conda#9f0b2eb5f5dd2cec36d5342a80adfec0
 https://conda.anaconda.org/conda-forge/noarch/ensureconda-1.4.3-pyhd8ed1ab_0.tar.bz2#c99ae3abf501990769047b4b40a98f17
-https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.1-pyh736e0ef_0.conda#d5aa7d2cc9fe03f62cf6e7bcc8e1a8df
+https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.3-pyh5fb750a_0.conda#00cfe411a8e07b8322185e573ae7c5a3
 https://conda.anaconda.org/conda-forge/osx-64/matplotlib-3.7.1-py38h50d1736_0.conda#14bce132d8a4546246b131c4289b480f
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.6.0-pyhd8ed1ab_0.conda#879782bde4bbdb4c7b5d4054504a20d5
 https://conda.anaconda.org/conda-forge/noarch/pooch-1.7.0-pyha770c72_3.conda#5936894aade8240c867d292aa0d980c6
 https://conda.anaconda.org/conda-forge/noarch/sphinx-5.0.0-pyh6c4a22f_1.tar.bz2#a7cc4b9c94548ff9a19b368f975e5404
 https://conda.anaconda.org/conda-forge/noarch/autodocsumm-0.2.11-pyhd8ed1ab_0.conda#547c48372c97c463c93af86d7f2c868c
 https://conda.anaconda.org/conda-forge/noarch/cachecontrol-with-filecache-0.13.0-pyhd8ed1ab_0.conda#3fd3d55ea862cc0736ac1cce6f44c2d1
 https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.6-pyhd8ed1ab_0.conda#68627a08556e4a273e4c7bfc84251457
-https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.6.0-pyhd8ed1ab_0.conda#39fd52b0fcb2fb52bac47a1419bf09bd
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.7.0-pyhd8ed1ab_0.conda#7488cd1f4d35a2af96faa765b7e5b2f0
 https://conda.anaconda.org/conda-forge/noarch/myst-parser-0.18.1-pyhd8ed1ab_0.tar.bz2#bcfdf5c7d8bf5c6f6be7b4c66fff2eca
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.6.0-pyhd8ed1ab_0.conda#e8172ca42f2869bb90185c9356899e81
 https://conda.anaconda.org/conda-forge/noarch/pydata-sphinx-theme-0.13.3-pyhd8ed1ab_0.conda#07aca5f2dea315dcc16680d6891e9056
 https://conda.anaconda.org/conda-forge/osx-64/scipy-1.10.1-py38h9cf86d3_3.conda#5e20c77455e815704b008ab8f42f6169
 https://conda.anaconda.org/conda-forge/noarch/sphinx-autobuild-2021.3.14-pyhd8ed1ab_0.tar.bz2#1909f784dc37b4ab97afe2c95aeeabaa
 https://conda.anaconda.org/conda-forge/noarch/sphinx-copybutton-0.5.2-pyhd8ed1ab_0.conda#ac832cc43adc79118cf6e23f1f9b8995
 https://conda.anaconda.org/conda-forge/noarch/sphinx-design-0.4.1-pyhd8ed1ab_1.conda#c6b2e7903121c3210462a0866a561993
```

### Comparing `eradiate-0.23.2rc3/requirements/conda/environment-optional.dot` & `eradiate-0.23.2rc4/requirements/conda/environment-optional.dot`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/requirements/conda/environment-optional.yml` & `eradiate-0.23.2rc4/requirements/conda/environment-optional.yml`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/requirements/conda/environment-recommended-linux-64.lock` & `eradiate-0.23.2rc4/requirements/conda/environment-tests-linux-64.lock`

 * *Files 8% similar despite different names*

```diff
@@ -1,176 +1,203 @@
 # Generated by conda-lock.
 # platform: linux-64
-# input_hash: 84e13a5b4b26b1b0383814c85dad1bbe52d5781f164b39f7f592b07d2bf79ca7
+# input_hash: 3cf157dfd557bfe6a4245d59c308b232e715ddba0b7b300c71ddb9306ac670bf
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2#d7c89558ba9fa0495403155b64376d81
 https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2023.5.7-hbcca054_0.conda#f5c65075fc34438d5b456c7f3f5ab695
+https://conda.anaconda.org/conda-forge/noarch/font-ttf-dejavu-sans-mono-2.37-hab24e00_0.tar.bz2#0c96522c6bdaed4b1566d11387caaf45
+https://conda.anaconda.org/conda-forge/noarch/font-ttf-inconsolata-3.000-h77eed37_0.tar.bz2#34893075a5c9e55cdafac56607368fc6
+https://conda.anaconda.org/conda-forge/noarch/font-ttf-source-code-pro-2.038-h77eed37_0.tar.bz2#4d59c254e01d9cde7957100457e2d5fb
+https://conda.anaconda.org/conda-forge/noarch/font-ttf-ubuntu-0.83-hab24e00_0.tar.bz2#19410c3df09dfb12d1206132a1d357c5
 https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h41732ed_0.conda#7aca3059a1729aa76c597603f10b0dd3
 https://conda.anaconda.org/conda-forge/linux-64/libgfortran5-13.1.0-h15d22d2_0.conda#afb656a334c409dd9805508af1c89c7a
 https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.1.0-hfd8a6a1_0.conda#067bcc23164642f4c226da631f2a2e1d
-https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.11-3_cp311.conda#c2e2630ddb68cf52eec74dc7dfab20b5
-https://conda.anaconda.org/conda-forge/noarch/tzdata-2023c-h71feb2d_0.conda#939e3e74d8be4dac89ce83b20de2492a
+https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.8-3_cp38.conda#2f3f7af062b42d664117662612022204
+https://conda.anaconda.org/conda-forge/noarch/fonts-conda-forge-1-0.tar.bz2#f766549260d6815b0c52253f1fb1bb29
 https://conda.anaconda.org/conda-forge/linux-64/libgfortran-ng-13.1.0-h69a702a_0.conda#506dc07710dd5b0ba63cbf134897fc10
 https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.1.0-he5830b7_0.conda#56ca14d57ac29a75d23a39eb3ee0ddeb
 https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2#73aaf86a425cc6e73fcf236a5a46396d
+https://conda.anaconda.org/conda-forge/noarch/fonts-conda-ecosystem-1-0.tar.bz2#fee5683a3f04bd15cbd8318b096a27ab
 https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.1.0-he5830b7_0.conda#cd93f779ff018dd85c7544c015c9db3c
+https://conda.anaconda.org/conda-forge/linux-64/alsa-lib-1.2.8-h166bdaf_0.tar.bz2#be733e69048951df1e4b4b7bb8c7666f
+https://conda.anaconda.org/conda-forge/linux-64/attr-2.5.1-h166bdaf_1.tar.bz2#d9c69a24ad678ffce24c6543a0176b00
 https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-h7f98852_4.tar.bz2#a1fd65c7ccbf10880423d82bca54eb54
+https://conda.anaconda.org/conda-forge/linux-64/c-ares-1.19.1-hd590300_0.conda#e8c18d865be43e2fb3f7a145b6adf1f5
+https://conda.anaconda.org/conda-forge/linux-64/gettext-0.21.1-h27087fc_0.tar.bz2#14947d8770185e5153fdd04d4673ed37
+https://conda.anaconda.org/conda-forge/linux-64/graphite2-1.3.13-h58526e2_1001.tar.bz2#8c54672728e8ec6aa6db90cf2806d220
+https://conda.anaconda.org/conda-forge/linux-64/icu-72.1-hcb278e6_0.conda#7c8d20d847bb45f56bd941578fcfa146
+https://conda.anaconda.org/conda-forge/linux-64/keyutils-1.6.1-h166bdaf_0.tar.bz2#30186d27e2c9fa62b45fb1476b7200e3
+https://conda.anaconda.org/conda-forge/linux-64/lame-3.100-h166bdaf_1003.tar.bz2#a8832b479f93521a9e7b5b743803be51
 https://conda.anaconda.org/conda-forge/linux-64/lerc-4.0.0-h27087fc_0.tar.bz2#76bbff344f0134279f225174e9064c8f
-https://conda.anaconda.org/conda-forge/linux-64/libbrotlicommon-1.0.9-h166bdaf_8.tar.bz2#9194c9bf9428035a05352d031462eae4
+https://conda.anaconda.org/conda-forge/linux-64/libaec-1.0.6-hcb278e6_1.conda#0f683578378cddb223e7fd24f785ab2a
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlicommon-1.0.9-h166bdaf_9.conda#61641e239f96eae2b8492dc7e755828c
 https://conda.anaconda.org/conda-forge/linux-64/libdeflate-1.18-h0b41bf4_0.conda#6aa9c9de5542ecb07fdda9ca626252d8
+https://conda.anaconda.org/conda-forge/linux-64/libev-4.33-h516909a_1.tar.bz2#6f8720dff19e17ce5d48cfe7f3d2f0a3
 https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.5.0-hcb278e6_1.conda#6305a3dd2752c76335295da4e581f2fd
 https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2#d645c6d2ac96843a2bfaccd2d62b3ac3
+https://conda.anaconda.org/conda-forge/linux-64/libiconv-1.17-h166bdaf_0.tar.bz2#b62b52da46c39ee2bc3c162ac7f1804d
 https://conda.anaconda.org/conda-forge/linux-64/libjpeg-turbo-2.1.5.1-h0b41bf4_0.conda#1edd9e67bdb90d78cea97733ff6b54e6
 https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.0-h7f98852_0.tar.bz2#39b1328babf85c7c3a61636d9cd50206
+https://repo.anaconda.com/pkgs/main/linux-64/libogg-1.3.5-h27cfd23_1.conda#710ee7fdb0ddf7591a5af7ca7eb4d73d
 https://conda.anaconda.org/conda-forge/linux-64/libopenblas-0.3.23-pthreads_h80387f5_0.conda#9c5ea51ccb8ffae7d06c645869d24ce6
-https://conda.anaconda.org/conda-forge/linux-64/libsodium-1.0.18-h36c2ea0_1.tar.bz2#c3788462a6fbddafdb413a9f9053e58d
+https://conda.anaconda.org/conda-forge/linux-64/libopus-1.3.1-h7f98852_1.tar.bz2#15345e56d527b330e1cacbdf58676e8f
 https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda#40b61aab5c7ba9ff276c41cfffe6b80b
-https://conda.anaconda.org/conda-forge/linux-64/libwebp-base-1.3.0-h0b41bf4_0.conda#0d4a7508d8c6c65314f2b9c1f56ad408
+https://conda.anaconda.org/conda-forge/linux-64/libwebp-base-1.3.1-hd590300_0.conda#82bf6f63eb15ef719b556b63feec3a77
 https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-hd590300_5.conda#f36c115f1ee199da648e0597ec2047ad
+https://conda.anaconda.org/conda-forge/linux-64/lz4-c-1.9.4-hcb278e6_0.conda#318b08df404f9c9be5712aaa5a6f0bb0
+https://conda.anaconda.org/conda-forge/linux-64/mpg123-1.31.3-hcb278e6_0.conda#141a126675b6d1a4eabb111a4a353898
 https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.4-hcb278e6_0.conda#681105bccc2a3f7f1a837d47d39c9179
+https://conda.anaconda.org/conda-forge/linux-64/nspr-4.35-h27087fc_0.conda#da0ec11a6454ae19bff5b02ed881a2b1
 https://conda.anaconda.org/conda-forge/linux-64/openssl-3.1.1-hd590300_1.conda#2e1d7b458ac8f1e3ca4e18b77add6277
+https://conda.anaconda.org/conda-forge/linux-64/pixman-0.40.0-h36c2ea0_0.tar.bz2#660e72c82f2e75a6b3fe6a6e75c79f19
 https://conda.anaconda.org/conda-forge/linux-64/pthread-stubs-0.4-h36c2ea0_1001.tar.bz2#22dad4df6e8630e8dff2428f6f6a7036
+https://conda.anaconda.org/conda-forge/linux-64/snappy-1.1.10-h9fff704_0.conda#e6d228cd0bb74a51dd18f5bfce0b4115
+https://conda.anaconda.org/conda-forge/linux-64/xorg-kbproto-1.0.7-h7f98852_1002.tar.bz2#4b230e8381279d76131116660f5a241a
+https://conda.anaconda.org/conda-forge/linux-64/xorg-libice-1.1.1-hd590300_0.conda#b462a33c0be1421532f28bfe8f4a7514
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxau-1.0.11-hd590300_0.conda#2c80dc38fface310c9bd81b17037fee5
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxdmcp-1.1.3-h7f98852_0.tar.bz2#be93aabceefa2fac576e971aef407908
+https://conda.anaconda.org/conda-forge/linux-64/xorg-renderproto-0.11.1-h7f98852_1002.tar.bz2#06feff3d2634e3097ce2fe681474b534
+https://conda.anaconda.org/conda-forge/linux-64/xorg-xextproto-7.3.0-h0b41bf4_1003.conda#bce9f945da8ad2ae9b1d7165a64d0f87
+https://conda.anaconda.org/conda-forge/linux-64/xorg-xf86vidmodeproto-2.3.1-h7f98852_1002.tar.bz2#3ceea9668625c18f19530de98b15d5b0
+https://conda.anaconda.org/conda-forge/linux-64/xorg-xproto-7.0.31-h7f98852_1007.tar.bz2#b4a4381d54784606820704f7b5f05a15
 https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2#2161070d867d1b1204ea749c8eec4ef0
-https://conda.anaconda.org/conda-forge/linux-64/yaml-0.2.5-h7f98852_2.tar.bz2#4cb3ad778ec2d5a7acbdf254eb1c42ae
+https://conda.anaconda.org/conda-forge/linux-64/expat-2.5.0-hcb278e6_1.conda#8b9b5aca60558d02ddaa09d599e55920
+https://conda.anaconda.org/conda-forge/linux-64/hdf4-4.2.15-h501b40f_6.conda#c3e9338e15d90106f467377017352b97
 https://conda.anaconda.org/conda-forge/linux-64/libblas-3.9.0-17_linux64_openblas.conda#57fb44770b1bc832fb2dbefa1bd502de
-https://conda.anaconda.org/conda-forge/linux-64/libbrotlidec-1.0.9-h166bdaf_8.tar.bz2#4ae4d7795d33e02bd20f6b23d91caf82
-https://conda.anaconda.org/conda-forge/linux-64/libbrotlienc-1.0.9-h166bdaf_8.tar.bz2#04bac51ba35ea023dc48af73c1c88c25
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlidec-1.0.9-h166bdaf_9.conda#081aa22f4581c08e4372b0b6c2f8478e
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlienc-1.0.9-h166bdaf_9.conda#1f0a03af852a9659ed2bf08f2f1704fd
+https://conda.anaconda.org/conda-forge/linux-64/libcap-2.67-he9d0100_0.conda#d05556c80caffff164d17bdea0105a1a
+https://conda.anaconda.org/conda-forge/linux-64/libedit-3.1.20191231-he28a2e2_2.tar.bz2#4d331e44109e3f0e19b4cb8f9b82f3e1
+https://conda.anaconda.org/conda-forge/linux-64/libevent-2.1.12-hf998b51_1.conda#a1cfcc585f0c42bf8d5546bb1dfb668d
+https://conda.anaconda.org/conda-forge/linux-64/libflac-1.4.3-h59595ed_0.conda#ee48bf17cc83a00f59ca1494d5646869
+https://conda.anaconda.org/conda-forge/linux-64/libgpg-error-1.47-h71f35ed_0.conda#c2097d0b46367996f09b4e8e4920384a
+https://conda.anaconda.org/conda-forge/linux-64/libnghttp2-1.52.0-h61bc06f_0.conda#613955a50485812985c059e7b269f42e
 https://conda.anaconda.org/conda-forge/linux-64/libpng-1.6.39-h753d276_0.conda#e1c890aebdebbfbf87e2c917187b4416
 https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.42.0-h2797004_0.conda#fdaae20a1cf7cd62130a0973190a31b7
+https://conda.anaconda.org/conda-forge/linux-64/libssh2-1.11.0-h0841786_0.conda#1f5a58e686b13bcfde88b93f547d23fe
+https://conda.anaconda.org/conda-forge/linux-64/libvorbis-1.3.7-h9c3ff4c_0.tar.bz2#309dec04b70a3cc0f1e84a4013683bc0
 https://conda.anaconda.org/conda-forge/linux-64/libxcb-1.15-h0b41bf4_0.conda#33277193f5b92bad9fdd230eb700929c
+https://conda.anaconda.org/conda-forge/linux-64/libxml2-2.11.4-h0d562d8_0.conda#e46fad17d5fb57316b956f88dca765e4
+https://conda.anaconda.org/conda-forge/linux-64/libzip-1.9.2-hc929e4a_1.tar.bz2#5b122b50e738c4be5c3f2899f010d7cf
+https://conda.anaconda.org/conda-forge/linux-64/mysql-common-8.0.33-hf1915f5_1.conda#b241363e3b72bae6dfbd31e9fecf7d26
+https://conda.anaconda.org/conda-forge/linux-64/pcre2-10.40-hc3806b6_0.tar.bz2#69e2c796349cd9b273890bee0febfe1b
 https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda#47d31b792659ce70f470b5c82fdfb7a4
 https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.12-h27826a3_0.tar.bz2#5b8c42eb62e9fc961af70bdd6a26e168
-https://conda.anaconda.org/conda-forge/linux-64/zeromq-4.3.4-h9c3ff4c_1.tar.bz2#21743a8d2ea0c8cfbbf8fe489b0347df
+https://conda.anaconda.org/conda-forge/linux-64/xorg-libsm-1.2.4-h7391055_0.conda#93ee23f12bc2e684548181256edd2cf6
+https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.13-hd590300_5.conda#68c34ec6149623be41a1933ab996a209
 https://conda.anaconda.org/conda-forge/linux-64/zstd-1.5.2-h3eb15da_6.conda#6b63daed8feeca47be78f323e793d555
-https://conda.anaconda.org/conda-forge/linux-64/brotli-bin-1.0.9-h166bdaf_8.tar.bz2#e5613f2bc717e9945840ff474419b8e4
+https://conda.anaconda.org/conda-forge/linux-64/blosc-1.21.4-h0f2a231_0.conda#876286b5941933a0f558777e57d883cc
+https://conda.anaconda.org/conda-forge/linux-64/brotli-bin-1.0.9-h166bdaf_9.conda#d47dee1856d9cb955b8076eeff304a5b
 https://conda.anaconda.org/conda-forge/linux-64/freetype-2.12.1-hca18f0e_1.conda#e1232042de76d24539a436d37597eb06
+https://conda.anaconda.org/conda-forge/linux-64/krb5-1.20.1-h81ceb04_0.conda#89a41adce7106749573d883b2f657d78
 https://conda.anaconda.org/conda-forge/linux-64/libcblas-3.9.0-17_linux64_openblas.conda#7ef0969b00fe3d6eef56a8151d3afb29
+https://conda.anaconda.org/conda-forge/linux-64/libgcrypt-1.10.1-h166bdaf_0.tar.bz2#f967fc95089cd247ceed56eda31de3a9
+https://conda.anaconda.org/conda-forge/linux-64/libglib-2.76.3-hebfc3b9_0.conda#a64f11b244b2c112cd3fa1cbe9493999
 https://conda.anaconda.org/conda-forge/linux-64/liblapack-3.9.0-17_linux64_openblas.conda#a2103882c46492e26500fcb56c03de8b
+https://conda.anaconda.org/conda-forge/linux-64/libllvm16-16.0.6-h5cf9203_0.conda#753e078cccad40fe4b396bdcf27a3c15
+https://conda.anaconda.org/conda-forge/linux-64/libsndfile-1.2.0-hb75c966_0.conda#c648d19cd9c8625898d5d370414de7c7
 https://conda.anaconda.org/conda-forge/linux-64/libtiff-4.5.1-h8b53f26_0.conda#8ad377fb60abab446a9f02c62b3c2190
-https://conda.anaconda.org/conda-forge/linux-64/python-3.11.4-hab00c5b_0_cpython.conda#1c628861a2a126b9fc9363ca1b7d014e
-https://conda.anaconda.org/eradiate/noarch/aabbtree-2.8.0-py_0.tar.bz2#647bcce5f0af4974e507591d5420486b
+https://conda.anaconda.org/conda-forge/linux-64/mysql-libs-8.0.33-hca2cd23_1.conda#a04ac37f0659929f3ba0f33c7f3d750f
+https://conda.anaconda.org/conda-forge/linux-64/nss-3.89-he45b914_0.conda#2745719a58eeaab6657256a3f142f099
+https://conda.anaconda.org/conda-forge/linux-64/python-3.8.17-he550d4f_0_cpython.conda#72d038de0a228e4f0ef4011940641293
+https://conda.anaconda.org/conda-forge/linux-64/xcb-util-0.4.0-hd590300_1.conda#9bfac7ccd94d54fd21a0501296d60424
+https://conda.anaconda.org/conda-forge/linux-64/xcb-util-keysyms-0.4.0-h8ee46fc_1.conda#632413adcd8bc16b515cab87a2932913
+https://conda.anaconda.org/conda-forge/linux-64/xcb-util-renderutil-0.3.9-hd590300_1.conda#e995b155d938b6779da6ace6c6b13816
+https://conda.anaconda.org/conda-forge/linux-64/xcb-util-wm-0.4.1-h8ee46fc_1.conda#90108a432fb5c6150ccfee3f03388656
+https://conda.anaconda.org/conda-forge/linux-64/xorg-libx11-1.8.6-h8ee46fc_0.conda#7590b76c3d11d21caa44f3fc38ac584a
+https://conda.anaconda.org/conda-forge/noarch/aenum-3.1.15-pyhd8ed1ab_0.conda#24cff7ab050ebb8a16bdeb02e8ed6f63
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
-https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
-https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
-https://conda.anaconda.org/conda-forge/linux-64/brotli-1.0.9-h166bdaf_8.tar.bz2#2ff08978892a3e8b954397c461f18418
+https://conda.anaconda.org/conda-forge/linux-64/brotli-1.0.9-h166bdaf_9.conda#4601544b4982ba1861fa9b9c607b2c06
+https://conda.anaconda.org/conda-forge/linux-64/brotli-python-1.0.9-py38hfa26641_9.conda#d056745008e5ed73210a31dcfd4d183a
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
+https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-unix_pyhd8ed1ab_2.tar.bz2#20e4087407c7cb04a40817114b333dbf
+https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/noarch/cycler-0.11.0-pyhd8ed1ab_0.tar.bz2#a50559fad0affdbb33729a68669ca1cb
-https://conda.anaconda.org/conda-forge/linux-64/debugpy-1.6.7-py311hcafe171_0.conda#f4c810ad9d791c8df5ad900ed74b085b
-https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
-https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
-https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
+https://conda.anaconda.org/conda-forge/linux-64/dbus-1.13.6-h5008d03_3.tar.bz2#ecfff944ba3960ecb334b9a2663d708d
 https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
-https://conda.anaconda.org/conda-forge/noarch/executing-1.2.0-pyhd8ed1ab_0.tar.bz2#4c1bc140e2be5c8ba6e3acab99e25c50
-https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
+https://conda.anaconda.org/conda-forge/linux-64/fontconfig-2.14.2-h14ed4e7_0.conda#0f69b688f52ff6da70bccb7ff7001d1d
+https://conda.anaconda.org/conda-forge/linux-64/glib-tools-2.76.3-hfc55251_0.conda#8951eedf3cdf94dd733c1b5eee1f4880
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
-https://conda.anaconda.org/conda-forge/noarch/json5-0.9.5-pyh9f0ad1d_0.tar.bz2#10759827a94e6b14996e81fb002c0bda
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.7-pyhd8ed1ab_1.conda#0c0a54e16b764bafcae35913cc9d60ff
-https://conda.anaconda.org/conda-forge/linux-64/kiwisolver-1.4.4-py311h4dd048b_1.tar.bz2#46d451f575392c01dc193069bd89766d
+https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda#f800d2da156d08e289b14e87e43c1ae5
+https://conda.anaconda.org/conda-forge/linux-64/kiwisolver-1.4.4-py38h43d8883_1.tar.bz2#41ca56d5cac7bfc7eb4fcdbee878eb84
+https://conda.anaconda.org/conda-forge/noarch/lazy_loader-0.2-pyhd8ed1ab_0.conda#d060d017720c9882c4eca0544a4a0592
 https://conda.anaconda.org/conda-forge/linux-64/lcms2-2.15-haa2dc70_1.conda#980d8aca0bc23ca73fa8caa3e7c84c28
-https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.3-py311h459d7ec_0.conda#9904dc4adb5d547cb21e136f98cb24b0
-https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.0-pyhd8ed1ab_0.conda#c7d0ea64c37752ecbe6da458aee662d2
+https://conda.anaconda.org/conda-forge/linux-64/libclang13-16.0.6-default_h4d60ac6_0.conda#b10174a063ec195f8fe1b278282c3149
+https://conda.anaconda.org/conda-forge/linux-64/libcups-2.3.3-h36d4200_3.conda#c9f4416a34bc91e0eb029f912c68f81f
+https://conda.anaconda.org/conda-forge/linux-64/libcurl-8.1.2-h409715c_0.conda#50c873c9660ed116707ae15b663928d8
+https://conda.anaconda.org/conda-forge/linux-64/libpq-15.3-hbcd7760_1.conda#8afb2a97d256ffde95b91a6283bc598c
+https://conda.anaconda.org/conda-forge/linux-64/libsystemd0-253-h8c4010b_1.conda#9176b1e2cb8beca37a7510b0e801e38f
+https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.0-pyhd8ed1ab_0.tar.bz2#f8dab71fdc13b1bf29a01248b156d268
 https://conda.anaconda.org/conda-forge/noarch/munkres-1.1.4-pyh9f0ad1d_0.tar.bz2#2ba8498c1018c1e9c61eb99b973dfe19
-https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.5.6-pyhd8ed1ab_0.tar.bz2#7b868f21adde0d9b8b38f9c16836589b
-https://conda.anaconda.org/conda-forge/linux-64/numpy-1.25.0-py311h64a7726_0.conda#4df60430eca64502eb01e02df92246bf
+https://conda.anaconda.org/conda-forge/linux-64/numpy-1.24.4-py38h59b608b_0.conda#8c3e050afeeb2b32575bdb8955cc67b2
 https://conda.anaconda.org/conda-forge/linux-64/openjpeg-2.5.0-hfec8fc6_2.conda#5ce6a42505c6e9e6151c54c3ec8d68ea
 https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
-https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
-https://conda.anaconda.org/conda-forge/noarch/parso-0.8.3-pyhd8ed1ab_0.tar.bz2#17a565a0c3899244e938cdf417e7b094
-https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
-https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2#89e3c7cdde7d3aaa2aee933b604dd07f
-https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.0-pyhd8ed1ab_0.conda#95c5be3c7cbd872509d16c216617fdab
-https://conda.anaconda.org/conda-forge/linux-64/psutil-5.9.5-py311h2582759_0.conda#a90f8e278c1cd7064b2713e6b7db87e6
-https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2#359eeb6536da0e687af562ed265ec263
-https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2#6784285c7e55cb7212efabc79e4c2883
-https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
+https://conda.anaconda.org/conda-forge/noarch/pint-0.21-pyhd8ed1ab_0.conda#8d7b829e37d78447569c180f9d827005
+https://conda.anaconda.org/conda-forge/noarch/pluggy-1.2.0-pyhd8ed1ab_0.conda#7263924c642d22e311d9e59b839f1b33
+https://conda.anaconda.org/conda-forge/noarch/ply-3.11-py_1.tar.bz2#7205635cd71531943440fbfe3b6b5727
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
 https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.1.0-pyhd8ed1ab_0.conda#d3ed087d1f7f8f5590e8e87b57a8ce64
-https://conda.anaconda.org/conda-forge/linux-64/pyrsistent-0.19.3-py311h2582759_0.conda#e53876b66dcc4ba8a0afa63cd8502ac3
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
-https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.17.1-pyhd8ed1ab_0.conda#dd4f393d857e9283eef2442234bd05e3
-https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.7-pyhd8ed1ab_0.conda#a61bf9ec79426938ff785eb69dbb1960
-https://conda.anaconda.org/conda-forge/noarch/python-tzdata-2023.3-pyhd8ed1ab_0.conda#2590495f608a63625e165915fb4e2e34
 https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
-https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0-py311hd4cff14_5.tar.bz2#da8769492e423103c59f469f4f17f8d9
-https://conda.anaconda.org/conda-forge/linux-64/pyzmq-25.1.0-py311h75c88c4_0.conda#db94a7a9e865fbfde8c023b6e8958bb2
-https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2#912a71cc01012ee38e6b90ddd561e36f
-https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyh41d4057_0.conda#ada5a17adcd10be4fc7e37e4166ba0e2
-https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda#3b68bc43ec6baa48f7354a446267eefe
+https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml.clib-0.2.7-py38h1de0b5d_1.conda#9afa2fc3c51cc4e7d1589c38e4e00d5c
+https://conda.anaconda.org/conda-forge/noarch/setuptools-68.0.0-pyhd8ed1ab_0.conda#5a7739d0f57ee64133c9d32e6507c46d
+https://conda.anaconda.org/conda-forge/noarch/shellingham-1.4.0-pyh44b312d_0.tar.bz2#437655338696f9d0dfdb0a024e66b255
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
-https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
-https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
+https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
+https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
-https://conda.anaconda.org/conda-forge/linux-64/tornado-6.3.2-py311h459d7ec_0.conda#12b1c374ee90a1aa11ea921858394dc8
-https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.3-pyha770c72_0.conda#4a3014a4d107d15475d106b751c4e352
-https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
-https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
-https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.0-pyhd8ed1ab_0.conda#1dd6387a73d84e16b6f73de676bb4c36
+https://conda.anaconda.org/conda-forge/linux-64/tornado-6.3.2-py38h01eb140_0.conda#3db869202b0e523d606d13e81ca79ab6
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.0-pyha770c72_0.conda#c76ebd4731d3668ba16975a30ef19d0d
+https://conda.anaconda.org/conda-forge/linux-64/unicodedata2-15.0.0-py38h0a891b7_0.tar.bz2#44421904760e9f5ae2035193e04360f0
 https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
-https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.7-pyhd8ed1ab_0.conda#bcc54b91a8ce88f60f538b87b409909e
+https://conda.anaconda.org/conda-forge/linux-64/xcb-util-image-0.4.0-h8ee46fc_1.conda#9d7bcddf49cbf727730af10e71022c73
+https://conda.anaconda.org/conda-forge/linux-64/xkeyboard-config-2.39-hd590300_0.conda#d88c7fc8a11858fb14761832e4da1954
+https://conda.anaconda.org/conda-forge/linux-64/xorg-libxext-1.3.4-h0b41bf4_2.conda#82b6df12252e6f32402b96dacc656fec
+https://conda.anaconda.org/conda-forge/linux-64/xorg-libxrender-0.9.11-hd590300_0.conda#ed67c36f215b310412b2af935bf3e530
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
-https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.0-pyhd8ed1ab_1.conda#2b35a85d654a47aac8f34c1bb6de7142
-https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
-https://conda.anaconda.org/conda-forge/noarch/async-lru-2.0.2-pyhd8ed1ab_0.conda#41221f97a0c82e5a60b21716a3d7469c
-https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
-https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.4-pyhd8ed1ab_0.tar.bz2#c5b3edc62d6309088f4970b3eaaa65a6
-https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
-https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda#d48b143d01385872a88ef8417e96c30e
-https://conda.anaconda.org/conda-forge/linux-64/cffi-1.15.1-py311h409f033_3.conda#9025d0786dbbe4bc91fd8e85502decce
-https://conda.anaconda.org/conda-forge/noarch/comm-0.1.3-pyhd8ed1ab_0.conda#168ae0f82cdf7505048e81054c7354e4
-https://conda.anaconda.org/conda-forge/linux-64/contourpy-1.1.0-py311h9547e67_0.conda#daf3f23397ab2265d0cdfa339f3627ba
-https://conda.anaconda.org/conda-forge/linux-64/fonttools-4.40.0-py311h459d7ec_0.conda#b19f671a6b221f922cf871d71a71c0fa
-https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.7.0-pyha770c72_0.conda#ba3786c6846e46038fe60c785d46dc81
+https://conda.anaconda.org/conda-forge/linux-64/cairo-1.16.0-hbbf8b49_1016.conda#c1dd96500b9b1a75e9e511931f415cbc
+https://conda.anaconda.org/conda-forge/linux-64/cftime-1.6.2-py38h26c90d9_1.tar.bz2#dcc025a7bb54374979c500c2e161fac9
+https://conda.anaconda.org/conda-forge/linux-64/contourpy-1.1.0-py38h7f3f72f_0.conda#0fdf3cc879156e0234e05962d55b6502
+https://conda.anaconda.org/conda-forge/linux-64/curl-8.1.2-h409715c_0.conda#9f88cfb15b7d08b25880b138f91e0eb4
+https://conda.anaconda.org/eradiate/noarch/dessinemoi-23.1.0-py_0.tar.bz2#490780e63e113a7dc444bd068e049bfe
+https://conda.anaconda.org/conda-forge/noarch/environ-config-22.1.0-pyhd8ed1ab_0.tar.bz2#a1103faffa0a877313c1fba776aa0fc0
+https://conda.anaconda.org/conda-forge/linux-64/fonttools-4.40.0-py38h01eb140_0.conda#f893b6bac56c477dd71498569b4a9022
+https://conda.anaconda.org/conda-forge/linux-64/glib-2.76.3-hfc55251_0.conda#950e02f5665f5f4ff0437a6acba58798
+https://conda.anaconda.org/conda-forge/linux-64/hdf5-1.14.1-nompi_h4f84152_100.conda#ff9ae10aa224826c07da7ef26cb0b717
 https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
-https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
-https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.2.2-pyhd8ed1ab_0.tar.bz2#243f63592c8e449f40cd42eb5cf32f40
-https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
-https://conda.anaconda.org/conda-forge/noarch/overrides-7.3.1-pyhd8ed1ab_0.tar.bz2#a5745ced46e69aa9754053ba061974ab
-https://conda.anaconda.org/conda-forge/noarch/pexpect-4.8.0-pyh1a96a4e_2.tar.bz2#330448ce4403cc74990ac07c555942a1
-https://conda.anaconda.org/conda-forge/linux-64/pillow-9.5.0-py311h0b84326_1.conda#6be2190fdbf26a6c1d3356a54d955237
+https://conda.anaconda.org/conda-forge/linux-64/libclang-16.0.6-default_h1cdf331_0.conda#e976871e132fe506da52c1240229246a
+https://conda.anaconda.org/conda-forge/linux-64/libxkbcommon-1.5.0-h5d7e998_3.conda#c91ea308d7bf70b62ddda568478aa03b
+https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-3.0.0-pyhd8ed1ab_0.conda#93a8e71256479c62074356ef6ebf501b
+https://conda.anaconda.org/conda-forge/linux-64/pillow-10.0.0-py38h885162f_0.conda#777c54134d5422a867aed7084cf5db5e
+https://conda.anaconda.org/eradiate/noarch/pinttrs-23.2.0-py_0.tar.bz2#1aebe9fa813278f719fa8e31d8000452
 https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
-https://conda.anaconda.org/conda-forge/linux-64/pyerfa-2.0.0.3-py311hcb2cf0a_0.conda#0a3b00610d438d129341e810f0ce053d
+https://conda.anaconda.org/conda-forge/noarch/portion-2.4.0-pyhd8ed1ab_0.conda#9d34bac22e169b41f4e34525a140c13b
+https://conda.anaconda.org/conda-forge/linux-64/pulseaudio-client-16.1-hb77b528_4.conda#8f349ca16d30950aa00870484d9d30c4
+https://conda.anaconda.org/conda-forge/noarch/pytest-7.4.0-pyhd8ed1ab_0.conda#3cfe9b9e958e7238a386933c75d190db
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
-https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
-https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.1-pyh41d4057_0.conda#3788984d535770cad699efaeb6cb3037
-https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.3-hd8ed1ab_0.conda#3876f650ed7d0f95d70fa4b647621909
-https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.3-pyhd8ed1ab_0.conda#ae465d0fbf9f1979cb2d8d4043d885e2
-https://conda.anaconda.org/conda-forge/linux-64/argon2-cffi-bindings-21.2.0-py311hd4cff14_3.tar.bz2#5159e874f65ac382773d2b534a1d7b80
-https://conda.anaconda.org/conda-forge/linux-64/astropy-5.3-py311h1f0f07a_0.conda#9e745ec84b02bbe087debe6074413da0
-https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.7.0-hd8ed1ab_0.conda#27a4cec373ec84d1c1aa02a1e37f8eaf
-https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
-https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.4.4-pyhd8ed1ab_1.conda#7c0965e1d4a0ee1529e8eaa03a78a5b3
-https://conda.anaconda.org/conda-forge/linux-64/matplotlib-base-3.7.1-py311h8597a09_0.conda#70c3b734ffe82c16b6d121aaa11929a8
-https://conda.anaconda.org/conda-forge/linux-64/pandas-2.0.2-py311h320fe9a_0.conda#509769b430266dc5c2f6a3eab0f23164
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.6.0-pyhd8ed1ab_0.conda#741384b21c1b512617f4ee4ea8457c5d
+https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml-0.17.32-py38h01eb140_0.conda#c92cc8efb1341f90ea5f51f576480580
+https://conda.anaconda.org/conda-forge/linux-64/sip-6.7.9-py38h17151c0_0.conda#6a54fd42b71a8b1c5f9c4a691270cdf1
+https://conda.anaconda.org/conda-forge/noarch/tqdm-4.65.0-pyhd8ed1ab_1.conda#ed792aff3acb977d09c7013358097f83
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.0-hd8ed1ab_0.conda#37761dccc7ca8eaa08c60c4f62eb2dcc
+https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.3-pyhd8ed1ab_1.conda#89efeecbb24c62e2f1ed0b8ca959ec69
+https://repo.anaconda.com/pkgs/main/linux-64/gstreamer-1.22.3-h5eee18b_0.conda#c2ffbb79cb2f51b042de223d482b7b29
+https://conda.anaconda.org/conda-forge/linux-64/harfbuzz-7.3.0-hdb3a94d_0.conda#765bc76c0dfaf24ff9d8a2935b2510df
+https://conda.anaconda.org/conda-forge/noarch/importlib-resources-5.12.0-pyhd8ed1ab_0.conda#3544c818f0720c89eb16ae6940ab440b
+https://conda.anaconda.org/conda-forge/linux-64/libnetcdf-4.9.2-nompi_h78c856c_106.conda#47665bf3dec451455474556ecd940ed2
+https://conda.anaconda.org/conda-forge/linux-64/pandas-1.5.3-py38hdc8b05c_1.conda#c944b033a2126e7f714a7ecaecb22011
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.8.0-pyhd8ed1ab_0.conda#3e4aca765371893ad848397794600632
+https://conda.anaconda.org/conda-forge/linux-64/pyqt5-sip-12.11.0-py38h8dc9893_3.conda#7bb0328b4a0f857aeb432426b9a5f908
+https://conda.anaconda.org/conda-forge/noarch/pytest-metadata-3.0.0-pyhd8ed1ab_1.conda#8bdcc0f401561213821bf67513abeeff
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
-https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
-https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
-https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
-https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-5.3.1-py311h38be061_0.conda#0cf8259b01ede82c76007996f73f89ed
-https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
+https://conda.anaconda.org/conda-forge/noarch/rich-13.4.2-pyhd8ed1ab_0.conda#f993baacc175e83fafd6b846e9c4c8a2
+https://repo.anaconda.com/pkgs/main/linux-64/gst-plugins-base-1.22.3-he621ea3_0.conda#27be67671dce7d6d8c53bf6260090c15
+https://conda.anaconda.org/conda-forge/linux-64/matplotlib-base-3.7.1-py38hd6c3c57_0.conda#3b8ba76acae09fbd4b2247c4ee4c0324
+https://conda.anaconda.org/conda-forge/linux-64/netcdf4-1.6.4-nompi_py38h383a0a3_101.conda#693cbd2ee4f62c8a2521cfaf7560b647
 https://conda.anaconda.org/conda-forge/noarch/pooch-1.7.0-pyha770c72_3.conda#5936894aade8240c867d292aa0d980c6
-https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
-https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.2.0-pyhd8ed1ab_0.conda#58ca2d50c3b27b86fd7df62eaadbf9a9
-https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.0-pyhd8ed1ab_0.conda#f525a01528c3eba1d381a232a6971c6a
-https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.38-hd8ed1ab_0.conda#45b74f64d8808eda7e6f6e6b1d641fd2
-https://conda.anaconda.org/conda-forge/linux-64/scipy-1.10.1-py311h64a7726_3.conda#a01a3a7428e770db5a0c8c7ab5fce7f7
-https://conda.anaconda.org/conda-forge/noarch/iapws-1.5.3-pyhd8ed1ab_0.tar.bz2#c5cad28f7c667df1910c3e9f8213c5eb
-https://conda.anaconda.org/conda-forge/noarch/ipython-8.14.0-pyh41d4057_0.conda#0a0b0d8177c4a209017b356439292db8
-https://conda.anaconda.org/conda-forge/noarch/nbclient-0.8.0-pyhd8ed1ab_0.conda#e78da91cf428faaf05701ce8cc8f2f9b
-https://conda.anaconda.org/conda-forge/noarch/patsy-0.5.3-pyhd8ed1ab_0.tar.bz2#50ef6b29b1fb0768ca82c5aeb4fb2d96
-https://conda.anaconda.org/conda-forge/noarch/seaborn-base-0.12.2-pyhd8ed1ab_0.conda#cf88f3a1c11536bc3c10c14ad00ccc42
-https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.1-pyh210e3f2_0.conda#4b57b688e22d094d1479a35543c18e93
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.6.0-pyhd8ed1ab_0.conda#879782bde4bbdb4c7b5d4054504a20d5
-https://conda.anaconda.org/conda-forge/linux-64/statsmodels-0.14.0-py311h1f0f07a_1.conda#a1daa39fa0bfed4d91a3640c2274034a
-https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.6-pyhd8ed1ab_0.conda#68627a08556e4a273e4c7bfc84251457
-https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.6.0-pyhd8ed1ab_0.conda#39fd52b0fcb2fb52bac47a1419bf09bd
-https://conda.anaconda.org/conda-forge/noarch/seaborn-0.12.2-hd8ed1ab_0.conda#50847a47c07812f88581081c620f5160
-https://conda.anaconda.org/conda-forge/noarch/jupyter-lsp-2.2.0-pyhd8ed1ab_0.conda#38589f4104d11f2a59ff01a9f4e3bfb3
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.23.0-pyhd8ed1ab_0.conda#942aa06b962c7e507884c6fbeb4d1f7d
-https://conda.anaconda.org/conda-forge/noarch/notebook-shim-0.2.3-pyhd8ed1ab_0.conda#67e0fe74c156267d9159e9133df7fd37
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab-4.0.2-pyhd8ed1ab_0.conda#8e102bf37f10dd49c248910450242a19
+https://conda.anaconda.org/conda-forge/noarch/pytest-json-report-1.5.0-pyhd8ed1ab_0.tar.bz2#837e335fa428cf7c784ee2e80594506c
+https://conda.anaconda.org/conda-forge/noarch/typer-0.9.0-pyhd8ed1ab_0.conda#5030a13b2fe5e143d5956d4943d3018f
+https://conda.anaconda.org/conda-forge/noarch/xarray-2023.1.0-pyhd8ed1ab_0.conda#c11eb03b6f77a0d22ae88c454c940f55
+https://conda.anaconda.org/conda-forge/linux-64/qt-main-5.15.8-h01ceb2d_12.conda#60fd4bdf187f88bac57cdc1a052f2811
+https://conda.anaconda.org/conda-forge/linux-64/scipy-1.10.1-py38h59b608b_3.conda#2f2a57462fcfbc67dfdbb0de6f7484c2
+https://conda.anaconda.org/conda-forge/linux-64/pyqt-5.15.7-py38ha0d8c90_3.conda#e965dc172d67920d058ac2b3a0e27565
+https://conda.anaconda.org/conda-forge/linux-64/matplotlib-3.7.1-py38h578d9bd_0.conda#50ff9e0a3dd459a0ca365741072bf9a2
```

### Comparing `eradiate-0.23.2rc3/requirements/conda/environment-recommended-osx-64.lock` & `eradiate-0.23.2rc4/requirements/conda/environment-recommended-osx-64.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1,66 +1,67 @@
 # Generated by conda-lock.
 # platform: osx-64
-# input_hash: ab6dd7f82045463565400de32534d39bd9c4ded94492c4c9f4ca965e0e6cdfb1
+# input_hash: f87dd54695dc2f303b3687b491dc0f4745052b00efd7ce6f5fad8b8b684519b0
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h0d85af4_4.tar.bz2#37edc4e6304ca87316e160f5ca0bd1b5
 https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2023.5.7-h8857fd0_0.conda#b704e4b79ba0d887c4870b7b09d6a4df
-https://conda.anaconda.org/conda-forge/osx-64/libbrotlicommon-1.0.9-hb7f2c08_8.tar.bz2#37157d273eaf3bc7d6862104161d9ec9
+https://conda.anaconda.org/conda-forge/osx-64/libbrotlicommon-1.0.9-hb7f2c08_9.conda#ee1ee8c79c3426229ad03290573be552
 https://conda.anaconda.org/conda-forge/osx-64/libcxx-16.0.6-hd57cbcb_0.conda#7d6972792161077908b62971802f289a
 https://conda.anaconda.org/conda-forge/osx-64/libdeflate-1.18-hac1461d_0.conda#3d131584456b277ce0871e6481fde49b
 https://conda.anaconda.org/conda-forge/osx-64/libexpat-2.5.0-hf0c8a7f_1.conda#6c81cb022780ee33435cca0127dd43c9
 https://conda.anaconda.org/conda-forge/osx-64/libffi-3.4.2-h0d85af4_5.tar.bz2#ccb34fb14960ad8b125962d3d79b31a9
 https://conda.anaconda.org/conda-forge/osx-64/libjpeg-turbo-2.1.5.1-hb7f2c08_0.conda#d7309a152b9b79799063b8bb47e34a3a
 https://conda.anaconda.org/conda-forge/osx-64/libsodium-1.0.18-hbcb3906_1.tar.bz2#24632c09ed931af617fe6d5292919cab
-https://conda.anaconda.org/conda-forge/osx-64/libwebp-base-1.3.0-hb7f2c08_0.conda#18981e4c840126d6118d8952485fea51
+https://conda.anaconda.org/conda-forge/osx-64/libwebp-base-1.3.1-h0dc2134_0.conda#a25a41b5be3fed4b671a58b998dcf89b
 https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-h8a1eda9_5.conda#4a3ad23f6e16f99c04e166767193d700
 https://conda.anaconda.org/conda-forge/osx-64/llvm-openmp-16.0.6-hff08bdf_0.conda#39a5227d906f75102bf8586741690128
 https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.4-hf0c8a7f_0.conda#c3dbae2411164d9b02c69090a9a91857
 https://conda.anaconda.org/conda-forge/osx-64/pthread-stubs-0.4-hc929b4f_1001.tar.bz2#addd19059de62181cd11ae8f4ef26084
 https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.11-3_cp311.conda#5e0a069a585445333868d2c6651c3b3f
 https://conda.anaconda.org/conda-forge/noarch/tzdata-2023c-h71feb2d_0.conda#939e3e74d8be4dac89ce83b20de2492a
 https://conda.anaconda.org/conda-forge/osx-64/xorg-libxau-1.0.11-h0dc2134_0.conda#9566b4c29274125b0266d0177b5eb97b
 https://conda.anaconda.org/conda-forge/osx-64/xorg-libxdmcp-1.1.3-h35c211d_0.tar.bz2#86ac76d6bf1cbb9621943eb3bd9ae36e
 https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2#a72f9d4ea13d55d745ff1ed594747f10
 https://conda.anaconda.org/conda-forge/osx-64/yaml-0.2.5-h0d85af4_2.tar.bz2#d7e08fcf8259d742156188e8762b4d20
 https://conda.anaconda.org/conda-forge/osx-64/lerc-4.0.0-hb486fe8_0.tar.bz2#f9d6a4c82889d5ecedec1d90eb673c55
-https://conda.anaconda.org/conda-forge/osx-64/libbrotlidec-1.0.9-hb7f2c08_8.tar.bz2#7f952a036d9014b4dab96c6ea0f8c2a7
-https://conda.anaconda.org/conda-forge/osx-64/libbrotlienc-1.0.9-hb7f2c08_8.tar.bz2#b36a3bfe866d9127f25f286506982166
+https://conda.anaconda.org/conda-forge/osx-64/libbrotlidec-1.0.9-hb7f2c08_9.conda#4043ef9fe42e178785e0e1853b79bdf9
+https://conda.anaconda.org/conda-forge/osx-64/libbrotlienc-1.0.9-hb7f2c08_9.conda#b64d4dcc70aa141db7fccbf13bad81e1
 https://conda.anaconda.org/conda-forge/osx-64/libgfortran5-12.2.0-he409387_31.conda#5a544130e584b1f204ac896ff071d5b3
 https://conda.anaconda.org/conda-forge/osx-64/libpng-1.6.39-ha978bb4_0.conda#35e4928794c5391aec14ffdf1deaaee5
 https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.42.0-h58db7d2_0.conda#a7d3b44b7b0c9901ac7813b7a0462893
 https://conda.anaconda.org/conda-forge/osx-64/libxcb-1.15-hb7f2c08_0.conda#5513f57e0238c87c12dffedbcc9c1a4a
 https://conda.anaconda.org/conda-forge/osx-64/openssl-3.1.1-h8a1eda9_1.conda#c7822d6ee74e34af1fd74365cfd18983
 https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda#f17f77f2acf4d344734bda76829ce14e
 https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.12-h5dbffcc_0.tar.bz2#8e9480d9c47061db2ed1b4ecce519a7f
 https://conda.anaconda.org/conda-forge/osx-64/zeromq-4.3.4-he49afe7_1.tar.bz2#1972d732b123ed04b60fd21e94f0b178
 https://conda.anaconda.org/conda-forge/osx-64/zstd-1.5.2-hbc0c0cd_6.conda#40a188783d3c425bdccc9ae9104acbb8
-https://conda.anaconda.org/conda-forge/osx-64/brotli-bin-1.0.9-hb7f2c08_8.tar.bz2#aac5ad0d8f747ef7f871508146df75d9
+https://conda.anaconda.org/conda-forge/osx-64/brotli-bin-1.0.9-hb7f2c08_9.conda#72c526f7ffa265473e6c75fd90605e52
 https://conda.anaconda.org/conda-forge/osx-64/freetype-2.12.1-h3f81eb7_1.conda#852224ea3e8991a8342228eab274840e
 https://conda.anaconda.org/conda-forge/osx-64/libgfortran-5.0.0-11_3_0_h97931a8_31.conda#97451338600bd9c5b535eb224ef6c471
 https://conda.anaconda.org/conda-forge/osx-64/libtiff-4.5.1-hf955e92_0.conda#56523ed556e3a44c0fd55bcf17045892
 https://conda.anaconda.org/conda-forge/osx-64/python-3.11.4-h30d4d87_0_cpython.conda#e40b3075f85db0184d5f61d17c580ef7
 https://conda.anaconda.org/eradiate/noarch/aabbtree-2.8.0-py_0.tar.bz2#647bcce5f0af4974e507591d5420486b
 https://conda.anaconda.org/conda-forge/noarch/appnope-0.1.3-pyhd8ed1ab_0.tar.bz2#54ac328d703bff191256ffa1183126d1
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
-https://conda.anaconda.org/conda-forge/osx-64/brotli-1.0.9-hb7f2c08_8.tar.bz2#55f612fe4a9b5f6ac76348b6de94aaeb
+https://conda.anaconda.org/conda-forge/osx-64/brotli-1.0.9-hb7f2c08_9.conda#53cff90f0cea22e13e5b791f0e5a8e7d
+https://conda.anaconda.org/conda-forge/osx-64/brotli-python-1.0.9-py311h814d153_9.conda#034ddcc806d421524fbc46778447e87c
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
 https://conda.anaconda.org/conda-forge/noarch/cycler-0.11.0-pyhd8ed1ab_0.tar.bz2#a50559fad0affdbb33729a68669ca1cb
 https://conda.anaconda.org/conda-forge/osx-64/debugpy-1.6.7-py311h814d153_0.conda#c27802860b87fe024c9b6276205a56b5
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
 https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
 https://conda.anaconda.org/conda-forge/noarch/executing-1.2.0-pyhd8ed1ab_0.tar.bz2#4c1bc140e2be5c8ba6e3acab99e25c50
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
-https://conda.anaconda.org/conda-forge/noarch/json5-0.9.5-pyh9f0ad1d_0.tar.bz2#10759827a94e6b14996e81fb002c0bda
+https://conda.anaconda.org/conda-forge/noarch/json5-0.9.14-pyhd8ed1ab_0.conda#dac1dabba2b5a9d1aee175c5fcc7b436
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.7-pyhd8ed1ab_1.conda#0c0a54e16b764bafcae35913cc9d60ff
 https://conda.anaconda.org/conda-forge/osx-64/kiwisolver-1.4.4-py311hd2070f0_1.tar.bz2#5219e72a43e53e8f6af4fdf76a0f90ef
 https://conda.anaconda.org/conda-forge/osx-64/lcms2-2.15-h2dcdeff_1.conda#f1df9b0c2d9fbe985e62f4b24773a9e4
 https://conda.anaconda.org/conda-forge/osx-64/libopenblas-0.3.23-openmp_h429af6e_0.conda#7000a828e29608e4f57e662b5502d2c9
 https://conda.anaconda.org/conda-forge/osx-64/markupsafe-2.1.3-py311h2725bcf_0.conda#65b70928fcc2a81891ad1a8a6a7b085a
 https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.0-pyhd8ed1ab_0.conda#c7d0ea64c37752ecbe6da458aee662d2
 https://conda.anaconda.org/conda-forge/noarch/munkres-1.1.4-pyh9f0ad1d_0.tar.bz2#2ba8498c1018c1e9c61eb99b973dfe19
@@ -83,91 +84,91 @@
 https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.17.1-pyhd8ed1ab_0.conda#dd4f393d857e9283eef2442234bd05e3
 https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.7-pyhd8ed1ab_0.conda#a61bf9ec79426938ff785eb69dbb1960
 https://conda.anaconda.org/conda-forge/noarch/python-tzdata-2023.3-pyhd8ed1ab_0.conda#2590495f608a63625e165915fb4e2e34
 https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
 https://conda.anaconda.org/conda-forge/osx-64/pyyaml-6.0-py311h5547dcb_5.tar.bz2#8d1e456914ce961119b07f396187a564
 https://conda.anaconda.org/conda-forge/osx-64/pyzmq-25.1.0-py311h5dacc12_0.conda#1f65b37886e7cb8476d48ea8bb9d19c0
 https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2#912a71cc01012ee38e6b90ddd561e36f
-https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda#3b68bc43ec6baa48f7354a446267eefe
+https://conda.anaconda.org/conda-forge/noarch/setuptools-68.0.0-pyhd8ed1ab_0.conda#5a7739d0f57ee64133c9d32e6507c46d
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/osx-64/tornado-6.3.2-py311h2725bcf_0.conda#276fe4341e39dcd9d9d33ca18140d2e7
 https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.3-pyha770c72_0.conda#4a3014a4d107d15475d106b751c4e352
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.0-pyha770c72_0.conda#c76ebd4731d3668ba16975a30ef19d0d
 https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
-https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.0-pyhd8ed1ab_0.conda#1dd6387a73d84e16b6f73de676bb4c36
+https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda#c34d9325a609381a0b0e8a5b4f325147
 https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
 https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.7-pyhd8ed1ab_0.conda#bcc54b91a8ce88f60f538b87b409909e
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
 https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.0-pyhd8ed1ab_1.conda#2b35a85d654a47aac8f34c1bb6de7142
 https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
 https://conda.anaconda.org/conda-forge/noarch/async-lru-2.0.2-pyhd8ed1ab_0.conda#41221f97a0c82e5a60b21716a3d7469c
 https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
-https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.4-pyhd8ed1ab_0.tar.bz2#c5b3edc62d6309088f4970b3eaaa65a6
+https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda#6b1b907661838a75d067a22f87996b2e
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
 https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda#d48b143d01385872a88ef8417e96c30e
 https://conda.anaconda.org/conda-forge/osx-64/cffi-1.15.1-py311ha86e640_3.conda#5967be4da33261eada7cc79593f71088
 https://conda.anaconda.org/conda-forge/noarch/comm-0.1.3-pyhd8ed1ab_0.conda#168ae0f82cdf7505048e81054c7354e4
 https://conda.anaconda.org/conda-forge/osx-64/fonttools-4.40.0-py311h2725bcf_0.conda#97ba9b04f9e416a1b0782a9a55c63efc
 https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.7.0-pyha770c72_0.conda#ba3786c6846e46038fe60c785d46dc81
 https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
 https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.2.2-pyhd8ed1ab_0.tar.bz2#243f63592c8e449f40cd42eb5cf32f40
 https://conda.anaconda.org/conda-forge/osx-64/libblas-3.9.0-17_osx64_openblas.conda#65299527582e2449b05d27fcf8352125
 https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
 https://conda.anaconda.org/conda-forge/noarch/overrides-7.3.1-pyhd8ed1ab_0.tar.bz2#a5745ced46e69aa9754053ba061974ab
 https://conda.anaconda.org/conda-forge/noarch/pexpect-4.8.0-pyh1a96a4e_2.tar.bz2#330448ce4403cc74990ac07c555942a1
-https://conda.anaconda.org/conda-forge/osx-64/pillow-9.5.0-py311h7cb0e2d_1.conda#bf4feca7fd63e619c39ab32eac625edf
+https://conda.anaconda.org/conda-forge/osx-64/pillow-10.0.0-py311h7cb0e2d_0.conda#042cee47581520be03136d16e8cc0969
 https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
 https://conda.anaconda.org/conda-forge/osx-64/pyobjc-core-9.2-py311hf110eff_0.conda#460e6d2c254ec4aa4299cd9bffa3b7f8
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
 https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
 https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.1-pyhd1c38e8_0.conda#046120b71d8896cb7faef78bfdbfee1e
 https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.3-hd8ed1ab_0.conda#3876f650ed7d0f95d70fa4b647621909
-https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.3-pyhd8ed1ab_0.conda#ae465d0fbf9f1979cb2d8d4043d885e2
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.0-hd8ed1ab_0.conda#37761dccc7ca8eaa08c60c4f62eb2dcc
+https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.3-pyhd8ed1ab_1.conda#89efeecbb24c62e2f1ed0b8ca959ec69
 https://conda.anaconda.org/conda-forge/osx-64/argon2-cffi-bindings-21.2.0-py311h5547dcb_3.tar.bz2#c09459e349fa61afc352f473766de109
 https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.7.0-hd8ed1ab_0.conda#27a4cec373ec84d1c1aa02a1e37f8eaf
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.4.4-pyhd8ed1ab_1.conda#7c0965e1d4a0ee1529e8eaa03a78a5b3
 https://conda.anaconda.org/conda-forge/osx-64/libcblas-3.9.0-17_osx64_openblas.conda#380151ca00704172b242a63701b7bf8a
 https://conda.anaconda.org/conda-forge/osx-64/liblapack-3.9.0-17_osx64_openblas.conda#6ab83532872bf3659613638589dd10af
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.6.0-pyhd8ed1ab_0.conda#741384b21c1b512617f4ee4ea8457c5d
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.8.0-pyhd8ed1ab_0.conda#3e4aca765371893ad848397794600632
 https://conda.anaconda.org/conda-forge/osx-64/pyobjc-framework-cocoa-9.2-py311hf110eff_0.conda#6ba4637fa1ed0a1e829b1f278c12274a
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
 https://conda.anaconda.org/conda-forge/osx-64/jupyter_core-5.3.1-py311h6eed73b_0.conda#2d45628b123595054093ff65996b98ae
 https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
 https://conda.anaconda.org/conda-forge/osx-64/numpy-1.25.0-py311hc44ba51_0.conda#11037145324619832869a29d0b21f66f
 https://conda.anaconda.org/conda-forge/noarch/pooch-1.7.0-pyha770c72_3.conda#5936894aade8240c867d292aa0d980c6
 https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
 https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyhd1c38e8_0.conda#2657c3de5371c571aef6678afb4aaadd
 https://conda.anaconda.org/conda-forge/osx-64/contourpy-1.1.0-py311h5fe6e05_0.conda#1969042c846644a15c25ea78f487459c
-https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.2.0-pyhd8ed1ab_0.conda#58ca2d50c3b27b86fd7df62eaadbf9a9
+https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda#1d018ee4ab13217e2544f795eb0a6798
 https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.0-pyhd8ed1ab_0.conda#f525a01528c3eba1d381a232a6971c6a
-https://conda.anaconda.org/conda-forge/osx-64/pandas-2.0.2-py311hab14417_0.conda#a490b12cf9ba39a6968000e93826c283
+https://conda.anaconda.org/conda-forge/osx-64/pandas-2.0.3-py311hab14417_0.conda#f9dddf66591e316635e4a8541a4ed385
 https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.38-hd8ed1ab_0.conda#45b74f64d8808eda7e6f6e6b1d641fd2
 https://conda.anaconda.org/conda-forge/osx-64/pyerfa-2.0.0.3-py311hd5badaa_0.conda#18093456a2390c1f8b1714280e1a31c4
-https://conda.anaconda.org/conda-forge/osx-64/scipy-1.10.1-py311h16c3c4d_3.conda#a3ba8e96a7511ef8c3b61d28a68da6ed
+https://conda.anaconda.org/conda-forge/osx-64/scipy-1.11.1-py311h16c3c4d_0.conda#3492280f8227a6070eb1ee8c84ab5827
 https://conda.anaconda.org/conda-forge/osx-64/astropy-5.3-py311h4a70a88_0.conda#566257e29859e9c3f5e57a253c0688f4
 https://conda.anaconda.org/conda-forge/noarch/iapws-1.5.3-pyhd8ed1ab_0.tar.bz2#c5cad28f7c667df1910c3e9f8213c5eb
 https://conda.anaconda.org/conda-forge/noarch/ipython-8.14.0-pyhd1c38e8_0.conda#f56fab4cea853c2248105b6cd7d79bf0
 https://conda.anaconda.org/conda-forge/osx-64/matplotlib-base-3.7.1-py311h2bf763f_0.conda#d67ac9c9b834ae77ff7b2c59f702803c
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.8.0-pyhd8ed1ab_0.conda#e78da91cf428faaf05701ce8cc8f2f9b
 https://conda.anaconda.org/conda-forge/noarch/patsy-0.5.3-pyhd8ed1ab_0.tar.bz2#50ef6b29b1fb0768ca82c5aeb4fb2d96
-https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.1-pyh736e0ef_0.conda#d5aa7d2cc9fe03f62cf6e7bcc8e1a8df
+https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.3-pyh5fb750a_0.conda#00cfe411a8e07b8322185e573ae7c5a3
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.6.0-pyhd8ed1ab_0.conda#879782bde4bbdb4c7b5d4054504a20d5
 https://conda.anaconda.org/conda-forge/noarch/seaborn-base-0.12.2-pyhd8ed1ab_0.conda#cf88f3a1c11536bc3c10c14ad00ccc42
 https://conda.anaconda.org/conda-forge/osx-64/statsmodels-0.14.0-py311h4a70a88_1.conda#8dc3f215493f36f9d9fa42bd24aaee7a
 https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.6-pyhd8ed1ab_0.conda#68627a08556e4a273e4c7bfc84251457
-https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.6.0-pyhd8ed1ab_0.conda#39fd52b0fcb2fb52bac47a1419bf09bd
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.7.0-pyhd8ed1ab_0.conda#7488cd1f4d35a2af96faa765b7e5b2f0
 https://conda.anaconda.org/conda-forge/noarch/seaborn-0.12.2-hd8ed1ab_0.conda#50847a47c07812f88581081c620f5160
 https://conda.anaconda.org/conda-forge/noarch/jupyter-lsp-2.2.0-pyhd8ed1ab_0.conda#38589f4104d11f2a59ff01a9f4e3bfb3
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.23.0-pyhd8ed1ab_0.conda#942aa06b962c7e507884c6fbeb4d1f7d
 https://conda.anaconda.org/conda-forge/noarch/notebook-shim-0.2.3-pyhd8ed1ab_0.conda#67e0fe74c156267d9159e9133df7fd37
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab-4.0.2-pyhd8ed1ab_0.conda#8e102bf37f10dd49c248910450242a19
```

### Comparing `eradiate-0.23.2rc3/requirements/conda/environment-tests-osx-64.lock` & `eradiate-0.23.2rc4/requirements/conda/environment-tests-osx-64.lock`

 * *Files 4% similar despite different names*

```diff
@@ -1,61 +1,62 @@
 # Generated by conda-lock.
 # platform: osx-64
-# input_hash: 50e26e276d2e64fb83958f5d0741cc2682dfd1a187ca01e50168781d16482c74
+# input_hash: 1c29b330cc88d36df475dc636bda463fb714b08d5c79427c7fc31a60ac0aa52b
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h0d85af4_4.tar.bz2#37edc4e6304ca87316e160f5ca0bd1b5
 https://conda.anaconda.org/conda-forge/osx-64/c-ares-1.19.1-h0dc2134_0.conda#b3e62631b4e1b9801477523ce1d6f355
 https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2023.5.7-h8857fd0_0.conda#b704e4b79ba0d887c4870b7b09d6a4df
 https://conda.anaconda.org/conda-forge/osx-64/icu-72.1-h7336db1_0.conda#c9689510a50a4bb2ae978421671a125e
-https://conda.anaconda.org/conda-forge/osx-64/libbrotlicommon-1.0.9-hb7f2c08_8.tar.bz2#37157d273eaf3bc7d6862104161d9ec9
+https://conda.anaconda.org/conda-forge/osx-64/libbrotlicommon-1.0.9-hb7f2c08_9.conda#ee1ee8c79c3426229ad03290573be552
 https://conda.anaconda.org/conda-forge/osx-64/libcxx-16.0.6-hd57cbcb_0.conda#7d6972792161077908b62971802f289a
 https://conda.anaconda.org/conda-forge/osx-64/libdeflate-1.18-hac1461d_0.conda#3d131584456b277ce0871e6481fde49b
 https://conda.anaconda.org/conda-forge/osx-64/libev-4.33-haf1e3a3_1.tar.bz2#79dc2be110b2a3d1e97ec21f691c50ad
 https://conda.anaconda.org/conda-forge/osx-64/libffi-3.4.2-h0d85af4_5.tar.bz2#ccb34fb14960ad8b125962d3d79b31a9
 https://conda.anaconda.org/conda-forge/osx-64/libiconv-1.17-hac89ed1_0.tar.bz2#691d103d11180486154af49c037b7ed9
 https://conda.anaconda.org/conda-forge/osx-64/libjpeg-turbo-2.1.5.1-hb7f2c08_0.conda#d7309a152b9b79799063b8bb47e34a3a
-https://conda.anaconda.org/conda-forge/osx-64/libwebp-base-1.3.0-hb7f2c08_0.conda#18981e4c840126d6118d8952485fea51
+https://conda.anaconda.org/conda-forge/osx-64/libwebp-base-1.3.1-h0dc2134_0.conda#a25a41b5be3fed4b671a58b998dcf89b
 https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-h8a1eda9_5.conda#4a3ad23f6e16f99c04e166767193d700
 https://conda.anaconda.org/conda-forge/osx-64/llvm-openmp-16.0.6-hff08bdf_0.conda#39a5227d906f75102bf8586741690128
 https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.4-hf0c8a7f_0.conda#c3dbae2411164d9b02c69090a9a91857
 https://conda.anaconda.org/conda-forge/osx-64/pthread-stubs-0.4-hc929b4f_1001.tar.bz2#addd19059de62181cd11ae8f4ef26084
 https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.8-3_cp38.conda#ff192f59f7fe23555612030493a079f8
 https://conda.anaconda.org/conda-forge/osx-64/xorg-libxau-1.0.11-h0dc2134_0.conda#9566b4c29274125b0266d0177b5eb97b
 https://conda.anaconda.org/conda-forge/osx-64/xorg-libxdmcp-1.1.3-h35c211d_0.tar.bz2#86ac76d6bf1cbb9621943eb3bd9ae36e
 https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2#a72f9d4ea13d55d745ff1ed594747f10
 https://conda.anaconda.org/conda-forge/osx-64/hdf4-4.2.15-h9804679_6.conda#c13d8841112ba7f5931d1d60631394f3
 https://conda.anaconda.org/conda-forge/osx-64/lerc-4.0.0-hb486fe8_0.tar.bz2#f9d6a4c82889d5ecedec1d90eb673c55
 https://conda.anaconda.org/conda-forge/osx-64/libaec-1.0.6-hf0c8a7f_1.conda#7c0f82f435ab4c48d65dc9b28db2ad9e
-https://conda.anaconda.org/conda-forge/osx-64/libbrotlidec-1.0.9-hb7f2c08_8.tar.bz2#7f952a036d9014b4dab96c6ea0f8c2a7
-https://conda.anaconda.org/conda-forge/osx-64/libbrotlienc-1.0.9-hb7f2c08_8.tar.bz2#b36a3bfe866d9127f25f286506982166
+https://conda.anaconda.org/conda-forge/osx-64/libbrotlidec-1.0.9-hb7f2c08_9.conda#4043ef9fe42e178785e0e1853b79bdf9
+https://conda.anaconda.org/conda-forge/osx-64/libbrotlienc-1.0.9-hb7f2c08_9.conda#b64d4dcc70aa141db7fccbf13bad81e1
 https://conda.anaconda.org/conda-forge/osx-64/libedit-3.1.20191231-h0678c8f_2.tar.bz2#6016a8a1d0e63cac3de2c352cd40208b
 https://conda.anaconda.org/conda-forge/osx-64/libgfortran5-12.2.0-he409387_31.conda#5a544130e584b1f204ac896ff071d5b3
 https://conda.anaconda.org/conda-forge/osx-64/libpng-1.6.39-ha978bb4_0.conda#35e4928794c5391aec14ffdf1deaaee5
 https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.42.0-h58db7d2_0.conda#a7d3b44b7b0c9901ac7813b7a0462893
 https://conda.anaconda.org/conda-forge/osx-64/libxcb-1.15-hb7f2c08_0.conda#5513f57e0238c87c12dffedbcc9c1a4a
 https://conda.anaconda.org/conda-forge/osx-64/libxml2-2.11.4-hd95e348_0.conda#681f8dda25e73a830d774a37b9839c85
 https://conda.anaconda.org/conda-forge/osx-64/lz4-c-1.9.4-hf0c8a7f_0.conda#aa04f7143228308662696ac24023f991
 https://conda.anaconda.org/conda-forge/osx-64/openssl-3.1.1-h8a1eda9_1.conda#c7822d6ee74e34af1fd74365cfd18983
 https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda#f17f77f2acf4d344734bda76829ce14e
 https://conda.anaconda.org/conda-forge/osx-64/snappy-1.1.10-h225ccf5_0.conda#4320a8781f14cd959689b86e349f3b73
 https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.12-h5dbffcc_0.tar.bz2#8e9480d9c47061db2ed1b4ecce519a7f
 https://conda.anaconda.org/conda-forge/osx-64/zstd-1.5.2-hbc0c0cd_6.conda#40a188783d3c425bdccc9ae9104acbb8
 https://conda.anaconda.org/conda-forge/osx-64/blosc-1.21.4-heccf04b_0.conda#02e92eb72b9ae4c1745b95d03a9c949e
-https://conda.anaconda.org/conda-forge/osx-64/brotli-bin-1.0.9-hb7f2c08_8.tar.bz2#aac5ad0d8f747ef7f871508146df75d9
+https://conda.anaconda.org/conda-forge/osx-64/brotli-bin-1.0.9-hb7f2c08_9.conda#72c526f7ffa265473e6c75fd90605e52
 https://conda.anaconda.org/conda-forge/osx-64/freetype-2.12.1-h3f81eb7_1.conda#852224ea3e8991a8342228eab274840e
 https://conda.anaconda.org/conda-forge/osx-64/krb5-1.20.1-h049b76e_0.conda#db11fa2968ef0837288fe2d7f5b77a50
 https://conda.anaconda.org/conda-forge/osx-64/libgfortran-5.0.0-11_3_0_h97931a8_31.conda#97451338600bd9c5b535eb224ef6c471
 https://conda.anaconda.org/conda-forge/osx-64/libnghttp2-1.52.0-he2ab024_0.conda#12ac7d100bf260263e30a019517f42a2
 https://conda.anaconda.org/conda-forge/osx-64/libssh2-1.11.0-hd019ec5_0.conda#ca3a72efba692c59a90d4b9fc0dfe774
 https://conda.anaconda.org/conda-forge/osx-64/libtiff-4.5.1-hf955e92_0.conda#56523ed556e3a44c0fd55bcf17045892
 https://conda.anaconda.org/conda-forge/osx-64/libzip-1.9.2-h6db710c_1.tar.bz2#ce732d37e479919f3d22b1ccdeb858ac
 https://conda.anaconda.org/conda-forge/osx-64/python-3.8.17-hf9b03c3_0_cpython.conda#f613b663d3829f325b4ffb626bf612b6
-https://conda.anaconda.org/conda-forge/noarch/aenum-3.1.12-pyhd8ed1ab_0.conda#602716538da00b2ca3cc85c4d35c0245
+https://conda.anaconda.org/conda-forge/noarch/aenum-3.1.15-pyhd8ed1ab_0.conda#24cff7ab050ebb8a16bdeb02e8ed6f63
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
-https://conda.anaconda.org/conda-forge/osx-64/brotli-1.0.9-hb7f2c08_8.tar.bz2#55f612fe4a9b5f6ac76348b6de94aaeb
+https://conda.anaconda.org/conda-forge/osx-64/brotli-1.0.9-hb7f2c08_9.conda#53cff90f0cea22e13e5b791f0e5a8e7d
+https://conda.anaconda.org/conda-forge/osx-64/brotli-python-1.0.9-py38h4cd09af_9.conda#f958e25488ff7e044031bca8a6c5267b
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
 https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-unix_pyhd8ed1ab_2.tar.bz2#20e4087407c7cb04a40817114b333dbf
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/noarch/cycler-0.11.0-pyhd8ed1ab_0.tar.bz2#a50559fad0affdbb33729a68669ca1cb
 https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
@@ -66,61 +67,61 @@
 https://conda.anaconda.org/conda-forge/osx-64/libcurl-8.1.2-hbee3ae8_0.conda#d51e337da844262f9033c9a26452520f
 https://conda.anaconda.org/conda-forge/osx-64/libopenblas-0.3.23-openmp_h429af6e_0.conda#7000a828e29608e4f57e662b5502d2c9
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.0-pyhd8ed1ab_0.tar.bz2#f8dab71fdc13b1bf29a01248b156d268
 https://conda.anaconda.org/conda-forge/noarch/munkres-1.1.4-pyh9f0ad1d_0.tar.bz2#2ba8498c1018c1e9c61eb99b973dfe19
 https://conda.anaconda.org/conda-forge/osx-64/openjpeg-2.5.0-h13ac156_2.conda#299a29af9ac9f550ad459d655739280b
 https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
 https://conda.anaconda.org/conda-forge/noarch/pint-0.21-pyhd8ed1ab_0.conda#8d7b829e37d78447569c180f9d827005
-https://conda.anaconda.org/conda-forge/noarch/pluggy-1.0.0-pyhd8ed1ab_5.tar.bz2#7d301a0d25f424d96175f810935f0da9
+https://conda.anaconda.org/conda-forge/noarch/pluggy-1.2.0-pyhd8ed1ab_0.conda#7263924c642d22e311d9e59b839f1b33
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
 https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.1.0-pyhd8ed1ab_0.conda#d3ed087d1f7f8f5590e8e87b57a8ce64
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
 https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
 https://conda.anaconda.org/conda-forge/osx-64/ruamel.yaml.clib-0.2.7-py38hef030d1_1.conda#9a8e866b0680b61b2e988b18a1eaecae
-https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda#3b68bc43ec6baa48f7354a446267eefe
+https://conda.anaconda.org/conda-forge/noarch/setuptools-68.0.0-pyhd8ed1ab_0.conda#5a7739d0f57ee64133c9d32e6507c46d
 https://conda.anaconda.org/conda-forge/noarch/shellingham-1.4.0-pyh44b312d_0.tar.bz2#437655338696f9d0dfdb0a024e66b255
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/osx-64/tornado-6.3.2-py38hcafd530_0.conda#afefcf665a5049b030efb084a51e3935
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.3-pyha770c72_0.conda#4a3014a4d107d15475d106b751c4e352
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.0-pyha770c72_0.conda#c76ebd4731d3668ba16975a30ef19d0d
 https://conda.anaconda.org/conda-forge/osx-64/unicodedata2-15.0.0-py38hef030d1_0.tar.bz2#51020c740c53f14657f6307b9eb23f85
 https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
 https://conda.anaconda.org/conda-forge/osx-64/curl-8.1.2-hbee3ae8_0.conda#6cc301a6c2ba26e29949818efdc133ca
 https://conda.anaconda.org/eradiate/noarch/dessinemoi-23.1.0-py_0.tar.bz2#490780e63e113a7dc444bd068e049bfe
 https://conda.anaconda.org/conda-forge/noarch/environ-config-22.1.0-pyhd8ed1ab_0.tar.bz2#a1103faffa0a877313c1fba776aa0fc0
 https://conda.anaconda.org/conda-forge/osx-64/fonttools-4.40.0-py38hcafd530_0.conda#b26b38c5f75e03e86cecf860ca9fb1cd
-https://conda.anaconda.org/conda-forge/osx-64/hdf5-1.14.0-nompi_hbf0aa07_103.conda#90f50d124606a4e62628823b614a2f4c
+https://conda.anaconda.org/conda-forge/osx-64/hdf5-1.14.1-nompi_hedada53_100.conda#033c310c83abbd9c2f9a5c13b9f54225
 https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
 https://conda.anaconda.org/conda-forge/osx-64/libblas-3.9.0-17_osx64_openblas.conda#65299527582e2449b05d27fcf8352125
 https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-3.0.0-pyhd8ed1ab_0.conda#93a8e71256479c62074356ef6ebf501b
-https://conda.anaconda.org/conda-forge/osx-64/pillow-9.5.0-py38h16710f9_1.conda#c5bf174a033ef668679cc80918422515
+https://conda.anaconda.org/conda-forge/osx-64/pillow-10.0.0-py38h16710f9_0.conda#8f73f0573ab381d56588e001754c53d3
 https://conda.anaconda.org/eradiate/noarch/pinttrs-23.2.0-py_0.tar.bz2#1aebe9fa813278f719fa8e31d8000452
 https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
 https://conda.anaconda.org/conda-forge/noarch/portion-2.4.0-pyhd8ed1ab_0.conda#9d34bac22e169b41f4e34525a140c13b
-https://conda.anaconda.org/conda-forge/noarch/pytest-7.3.2-pyhd8ed1ab_1.conda#f2465696f4396245eca4613f6e924796
+https://conda.anaconda.org/conda-forge/noarch/pytest-7.4.0-pyhd8ed1ab_0.conda#3cfe9b9e958e7238a386933c75d190db
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
 https://conda.anaconda.org/conda-forge/osx-64/ruamel.yaml-0.17.32-py38hcafd530_0.conda#cb301e0b2b162330bc3b03fe51ea0d15
 https://conda.anaconda.org/conda-forge/noarch/tqdm-4.65.0-pyhd8ed1ab_1.conda#ed792aff3acb977d09c7013358097f83
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.3-hd8ed1ab_0.conda#3876f650ed7d0f95d70fa4b647621909
-https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.3-pyhd8ed1ab_0.conda#ae465d0fbf9f1979cb2d8d4043d885e2
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.0-hd8ed1ab_0.conda#37761dccc7ca8eaa08c60c4f62eb2dcc
+https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.3-pyhd8ed1ab_1.conda#89efeecbb24c62e2f1ed0b8ca959ec69
 https://conda.anaconda.org/conda-forge/noarch/importlib-resources-5.12.0-pyhd8ed1ab_0.conda#3544c818f0720c89eb16ae6940ab440b
 https://conda.anaconda.org/conda-forge/osx-64/libcblas-3.9.0-17_osx64_openblas.conda#380151ca00704172b242a63701b7bf8a
 https://conda.anaconda.org/conda-forge/osx-64/liblapack-3.9.0-17_osx64_openblas.conda#6ab83532872bf3659613638589dd10af
-https://conda.anaconda.org/conda-forge/osx-64/libnetcdf-4.9.2-nompi_hf077d52_105.conda#64d626e024a284777458e2b315e9eb56
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.6.0-pyhd8ed1ab_0.conda#741384b21c1b512617f4ee4ea8457c5d
+https://conda.anaconda.org/conda-forge/osx-64/libnetcdf-4.9.2-nompi_hfeda9e8_106.conda#66108519efbf30b02632ad35f519773f
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.8.0-pyhd8ed1ab_0.conda#3e4aca765371893ad848397794600632
 https://conda.anaconda.org/conda-forge/noarch/pytest-metadata-3.0.0-pyhd8ed1ab_1.conda#8bdcc0f401561213821bf67513abeeff
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/noarch/rich-13.4.2-pyhd8ed1ab_0.conda#f993baacc175e83fafd6b846e9c4c8a2
-https://conda.anaconda.org/conda-forge/osx-64/numpy-1.24.3-py38h9a4a08f_0.conda#5ff64b8133dea66865fe1bd35fb1d6d6
+https://conda.anaconda.org/conda-forge/osx-64/numpy-1.24.4-py38h9a4a08f_0.conda#85debc55a30068d6bb76a6deaf599afa
 https://conda.anaconda.org/conda-forge/noarch/pooch-1.7.0-pyha770c72_3.conda#5936894aade8240c867d292aa0d980c6
 https://conda.anaconda.org/conda-forge/noarch/pytest-json-report-1.5.0-pyhd8ed1ab_0.tar.bz2#837e335fa428cf7c784ee2e80594506c
 https://conda.anaconda.org/conda-forge/noarch/typer-0.9.0-pyhd8ed1ab_0.conda#5030a13b2fe5e143d5956d4943d3018f
 https://conda.anaconda.org/conda-forge/osx-64/cftime-1.6.2-py38hbd87e4b_1.tar.bz2#6b61efa56393b9655334192cc5423659
 https://conda.anaconda.org/conda-forge/osx-64/contourpy-1.1.0-py38h15a1a5b_0.conda#30d645ffb3572a3875e6fc8687857182
 https://conda.anaconda.org/conda-forge/osx-64/pandas-1.5.3-py38hec72209_1.conda#a8f001ab0a7c6312cea020bd20689765
 https://conda.anaconda.org/conda-forge/osx-64/scipy-1.10.1-py38h9cf86d3_3.conda#5e20c77455e815704b008ab8f42f6169
 https://conda.anaconda.org/conda-forge/osx-64/matplotlib-base-3.7.1-py38hcb346ec_0.conda#1f1eea98c232c8ef720175e12b00d0c4
-https://conda.anaconda.org/conda-forge/osx-64/netcdf4-1.6.4-nompi_py38h47ac6a0_100.conda#f86d4df9f8f46ae6d0c29bb87fe093b0
+https://conda.anaconda.org/conda-forge/osx-64/netcdf4-1.6.4-nompi_py38ha129777_101.conda#0e0f917d6168b9744a407d5ef3c2cb09
 https://conda.anaconda.org/conda-forge/noarch/xarray-2023.1.0-pyhd8ed1ab_0.conda#c11eb03b6f77a0d22ae88c454c940f55
 https://conda.anaconda.org/conda-forge/osx-64/matplotlib-3.7.1-py38h50d1736_0.conda#14bce132d8a4546246b131c4289b480f
```

### Comparing `eradiate-0.23.2rc3/requirements/conda/layer_graph.dot` & `eradiate-0.23.2rc4/requirements/conda/layer_graph.dot`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/requirements/copy_envvars.py` & `eradiate-0.23.2rc4/requirements/copy_envvars.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/requirements/layered.yml` & `eradiate-0.23.2rc4/requirements/layered.yml`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/requirements/make_conda_env.py` & `eradiate-0.23.2rc4/requirements/make_conda_env.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/requirements/make_pip_in_files.py` & `eradiate-0.23.2rc4/requirements/make_pip_in_files.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/requirements/pip/dependencies.txt` & `eradiate-0.23.2rc4/requirements/pip/dependencies.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --allow-unsafe --output-file=requirements/pip/dependencies.txt --resolver=backtracking requirements/pip/dependencies.in
+#    pip-compile --allow-unsafe --config=pyproject.toml --output-file=requirements/pip/dependencies.txt --resolver=backtracking requirements/pip/dependencies.in
 #
-aenum==3.1.12
+aenum==3.1.15
     # via -r requirements/pip/main.in
 attrs==23.1.0
     # via
     #   -r requirements/pip/main.in
     #   dessinemoi
     #   environ-config
     #   pinttrs
@@ -39,15 +39,15 @@
     #   matplotlib
 dessinemoi==23.1.0
     # via -r requirements/pip/main.in
 drjit==0.4.1
     # via eradiate-mitsuba
 environ-config==23.2.0
     # via -r requirements/pip/main.in
-eradiate-mitsuba==0.0.1
+eradiate-mitsuba==0.0.2
     # via -r requirements/pip/dependencies.in
 fonttools==4.40.0
     # via
     #   -c requirements/pip/dev.txt
     #   matplotlib
 idna==3.4
     # via
@@ -57,29 +57,29 @@
     # via
     #   -c requirements/pip/dev.txt
     #   matplotlib
 kiwisolver==1.4.4
     # via
     #   -c requirements/pip/dev.txt
     #   matplotlib
-lazy-loader==0.2
+lazy-loader==0.3
     # via -r requirements/pip/main.in
 markdown-it-py==3.0.0
     # via
     #   -c requirements/pip/dev.txt
     #   rich
 matplotlib==3.7.1
     # via -r requirements/pip/main.in
 mdurl==0.1.2
     # via
     #   -c requirements/pip/dev.txt
     #   markdown-it-py
 netcdf4==1.6.4
     # via -r requirements/pip/main.in
-numpy==1.24.3
+numpy==1.24.4
     # via
     #   -r requirements/pip/main.in
     #   cftime
     #   contourpy
     #   matplotlib
     #   netcdf4
     #   pandas
@@ -87,29 +87,29 @@
     #   xarray
 packaging==23.1
     # via
     #   -c requirements/pip/dev.txt
     #   matplotlib
     #   pooch
     #   xarray
-pandas==2.0.2
+pandas==2.0.3
     # via
     #   -c requirements/pip/dev.txt
     #   xarray
-pillow==9.5.0
+pillow==10.0.0
     # via
     #   -c requirements/pip/dev.txt
     #   matplotlib
 pint==0.21.1
     # via
     #   -r requirements/pip/main.in
     #   pinttrs
 pinttrs==23.2.0
     # via -r requirements/pip/main.in
-platformdirs==3.6.0
+platformdirs==3.8.0
     # via
     #   -c requirements/pip/dev.txt
     #   pooch
 pooch==1.7.0
     # via -r requirements/pip/main.in
 portion==2.4.0
     # via -r requirements/pip/main.in
@@ -154,15 +154,15 @@
     # via
     #   -c requirements/pip/dev.txt
     #   portion
 tqdm==4.65.0
     # via -r requirements/pip/main.in
 typer==0.9.0
     # via -r requirements/pip/main.in
-typing-extensions==4.6.3
+typing-extensions==4.7.0
     # via
     #   -c requirements/pip/dev.txt
     #   rich
     #   typer
 tzdata==2023.3
     # via
     #   -c requirements/pip/dev.txt
```

### Comparing `eradiate-0.23.2rc3/requirements/pip/dev.txt` & `eradiate-0.23.2rc4/requirements/pip/dev.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 #
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --allow-unsafe --output-file=requirements/pip/dev.txt --resolver=backtracking requirements/pip/dev.in
+#    pip-compile --allow-unsafe --config=pyproject.toml --output-file=requirements/pip/dev.txt --resolver=backtracking requirements/pip/dev.in
 #
 aabbtree==2.8.1
     # via -r requirements/pip/recommended.in
 accessible-pygments==0.0.4
     # via pydata-sphinx-theme
-aenum==3.1.12
+aenum==3.1.15
     # via -r requirements/pip/main.in
 alabaster==0.7.13
     # via sphinx
+annotated-types==0.5.0
+    # via pydantic
 anyio==3.7.0
     # via jupyter-server
 appdirs==1.4.4
     # via ensureconda
 argon2-cffi==21.3.0
     # via jupyter-server
 argon2-cffi-bindings==21.2.0
@@ -165,15 +167,15 @@
     # via
     #   jsonschema
     #   jupyterlab
     #   keyring
     #   matplotlib
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.23.2
+ipykernel==6.23.3
     # via
     #   ipywidgets
     #   jupyterlab
 ipython==8.12.2
     # via
     #   -r requirements/pip/recommended.in
     #   ipykernel
@@ -205,15 +207,15 @@
 jsonpointer==2.4
     # via jsonschema
 jsonschema[format-nongpl]==4.17.3
     # via
     #   jupyter-events
     #   jupyterlab-server
     #   nbformat
-jupyter-client==8.2.0
+jupyter-client==8.3.0
     # via
     #   ipykernel
     #   jupyter-server
     #   nbclient
 jupyter-core==5.3.1
     # via
     #   ipykernel
@@ -223,15 +225,15 @@
     #   nbclient
     #   nbconvert
     #   nbformat
 jupyter-events==0.6.3
     # via jupyter-server
 jupyter-lsp==2.2.0
     # via jupyterlab
-jupyter-server==2.6.0
+jupyter-server==2.7.0
     # via
     #   jupyter-lsp
     #   jupyterlab
     #   jupyterlab-server
     #   notebook-shim
 jupyter-server-terminals==0.4.4
     # via jupyter-server
@@ -239,21 +241,21 @@
     # via -r requirements/pip/recommended.in
 jupyterlab-pygments==0.2.2
     # via nbconvert
 jupyterlab-server==2.23.0
     # via jupyterlab
 jupyterlab-widgets==3.0.7
     # via ipywidgets
-keyring==24.0.0
+keyring==24.2.0
     # via conda-lock
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-lazy-loader==0.2
+lazy-loader==0.3
     # via -r requirements/pip/main.in
 livereload==2.6.3
     # via sphinx-autobuild
 markdown-it-py==3.0.0
     # via
     #   mdit-py-plugins
     #   myst-parser
@@ -300,15 +302,15 @@
     # via ipykernel
 netcdf4==1.6.4
     # via -r requirements/pip/main.in
 networkx==3.1
     # via -r requirements/pip/dev.in
 notebook-shim==0.2.3
     # via jupyterlab
-numpy==1.24.3
+numpy==1.24.4
     # via
     #   -r requirements/pip/main.in
     #   astropy
     #   cftime
     #   contourpy
     #   matplotlib
     #   netcdf4
@@ -331,48 +333,48 @@
     #   matplotlib
     #   nbconvert
     #   pooch
     #   pydata-sphinx-theme
     #   pytest
     #   sphinx
     #   xarray
-pandas==2.0.2
+pandas==2.0.3
     # via
     #   seaborn
     #   xarray
 pandocfilters==1.5.0
     # via nbconvert
 parso==0.8.3
     # via jedi
 pastel==0.2.1
     # via clikit
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
-pillow==9.5.0
+pillow==10.0.0
     # via matplotlib
 pint==0.21.1
     # via
     #   -r requirements/pip/main.in
     #   pinttrs
 pinttrs==23.2.0
     # via -r requirements/pip/main.in
-pip-tools==6.13.0
+pip-tools==6.14.0
     # via -r requirements/pip/dev.in
 pkginfo==1.9.6
     # via conda-lock
 pkgutil-resolve-name==1.3.10
     # via jsonschema
-platformdirs==3.6.0
+platformdirs==3.8.0
     # via
     #   jupyter-core
     #   pooch
     #   virtualenv
-pluggy==1.0.0
+pluggy==1.2.0
     # via pytest
 pooch==1.7.0
     # via -r requirements/pip/main.in
 portion==2.4.0
     # via -r requirements/pip/main.in
 prometheus-client==0.17.0
     # via jupyter-server
@@ -390,16 +392,18 @@
     # via
     #   pybtex-docutils
     #   sphinxcontrib-bibtex
 pybtex-docutils==1.0.2
     # via sphinxcontrib-bibtex
 pycparser==2.21
     # via cffi
-pydantic==1.10.9
+pydantic==2.0
     # via conda-lock
+pydantic-core==2.0.1
+    # via pydantic
 pydata-sphinx-theme==0.13.3
     # via sphinx-book-theme
 pyerfa==2.0.0.3
     # via astropy
 pygments==2.15.1
     # via
     #   accessible-pygments
@@ -412,15 +416,15 @@
     # via clikit
 pyparsing==3.1.0
     # via matplotlib
 pyproject-hooks==1.0.0
     # via build
 pyrsistent==0.19.3
     # via jsonschema
-pytest==7.3.2
+pytest==7.4.0
     # via
     #   -r requirements/pip/tests.in
     #   pytest-json-report
     #   pytest-metadata
 pytest-json-report==1.5.0
     # via -r requirements/pip/tests.in
 pytest-metadata==3.0.0
@@ -549,14 +553,15 @@
 tinycss2==1.2.1
     # via nbconvert
 tomli==2.0.1
     # via
     #   build
     #   conda-lock
     #   jupyterlab
+    #   pip-tools
     #   pyproject-hooks
     #   pytest
 tomlkit==0.11.8
     # via conda-lock
 toolz==0.12.0
     # via conda-lock
 tornado==6.3.2
@@ -583,26 +588,28 @@
     #   matplotlib-inline
     #   nbclient
     #   nbconvert
     #   nbformat
     #   nbsphinx
 typer==0.9.0
     # via -r requirements/pip/main.in
-typing-extensions==4.6.3
+typing-extensions==4.7.0
     # via
+    #   annotated-types
     #   async-lru
     #   conda-lock
     #   ipython
     #   pydantic
+    #   pydantic-core
     #   pydata-sphinx-theme
     #   rich
     #   typer
 tzdata==2023.3
     # via pandas
-uri-template==1.2.0
+uri-template==1.3.0
     # via jsonschema
 urllib3==1.26.16
     # via
     #   conda-lock
     #   requests
 virtualenv==20.23.1
     # via conda-lock
@@ -611,15 +618,15 @@
 webcolors==1.13
     # via jsonschema
 webencodings==0.5.1
     # via
     #   bleach
     #   html5lib
     #   tinycss2
-websocket-client==1.6.0
+websocket-client==1.6.1
     # via jupyter-server
 wheel==0.40.0
     # via pip-tools
 widgetsnbextension==4.0.7
     # via ipywidgets
 xarray==2023.1.0
     # via -r requirements/pip/main.in
```

### Comparing `eradiate-0.23.2rc3/requirements/pip/docs.txt` & `eradiate-0.23.2rc4/requirements/pip/docs.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --allow-unsafe --output-file=requirements/pip/docs.txt --resolver=backtracking requirements/pip/docs.in
+#    pip-compile --allow-unsafe --config=pyproject.toml --output-file=requirements/pip/docs.txt --resolver=backtracking requirements/pip/docs.in
 #
 accessible-pygments==0.0.4
     # via
     #   -c requirements/pip/dev.txt
     #   pydata-sphinx-theme
-aenum==3.1.12
+aenum==3.1.15
     # via
     #   -c requirements/pip/dev.txt
     #   -r requirements/pip/main.in
 alabaster==0.7.13
     # via
     #   -c requirements/pip/dev.txt
     #   sphinx
@@ -126,15 +126,15 @@
     #   nbconvert
     #   nbsphinx
     #   sphinx
 jsonschema==4.17.3
     # via
     #   -c requirements/pip/dev.txt
     #   nbformat
-jupyter-client==8.2.0
+jupyter-client==8.3.0
     # via
     #   -c requirements/pip/dev.txt
     #   nbclient
 jupyter-core==5.3.1
     # via
     #   -c requirements/pip/dev.txt
     #   jupyter-client
@@ -149,15 +149,15 @@
     # via
     #   -c requirements/pip/dev.txt
     #   matplotlib
 latexcodec==2.0.1
     # via
     #   -c requirements/pip/dev.txt
     #   pybtex
-lazy-loader==0.2
+lazy-loader==0.3
     # via
     #   -c requirements/pip/dev.txt
     #   -r requirements/pip/main.in
 livereload==2.6.3
     # via
     #   -c requirements/pip/dev.txt
     #   sphinx-autobuild
@@ -206,15 +206,15 @@
     #   nbsphinx
 nbsphinx==0.9.2
     # via -r requirements/pip/docs.in
 netcdf4==1.6.4
     # via
     #   -c requirements/pip/dev.txt
     #   -r requirements/pip/main.in
-numpy==1.24.3
+numpy==1.24.4
     # via
     #   -c requirements/pip/dev.txt
     #   -r requirements/pip/main.in
     #   cftime
     #   contourpy
     #   matplotlib
     #   netcdf4
@@ -226,23 +226,23 @@
     #   -c requirements/pip/dev.txt
     #   matplotlib
     #   nbconvert
     #   pooch
     #   pydata-sphinx-theme
     #   sphinx
     #   xarray
-pandas==2.0.2
+pandas==2.0.3
     # via
     #   -c requirements/pip/dev.txt
     #   xarray
 pandocfilters==1.5.0
     # via
     #   -c requirements/pip/dev.txt
     #   nbconvert
-pillow==9.5.0
+pillow==10.0.0
     # via
     #   -c requirements/pip/dev.txt
     #   matplotlib
 pint==0.21.1
     # via
     #   -c requirements/pip/dev.txt
     #   -r requirements/pip/main.in
@@ -251,15 +251,15 @@
     # via
     #   -c requirements/pip/dev.txt
     #   -r requirements/pip/main.in
 pkgutil-resolve-name==1.3.10
     # via
     #   -c requirements/pip/dev.txt
     #   jsonschema
-platformdirs==3.6.0
+platformdirs==3.8.0
     # via
     #   -c requirements/pip/dev.txt
     #   jupyter-core
     #   pooch
 pooch==1.7.0
     # via
     #   -c requirements/pip/dev.txt
@@ -430,15 +430,15 @@
     #   nbconvert
     #   nbformat
     #   nbsphinx
 typer==0.9.0
     # via
     #   -c requirements/pip/dev.txt
     #   -r requirements/pip/main.in
-typing-extensions==4.6.3
+typing-extensions==4.7.0
     # via
     #   -c requirements/pip/dev.txt
     #   pydata-sphinx-theme
     #   rich
     #   typer
 tzdata==2023.3
     # via
```

### Comparing `eradiate-0.23.2rc3/requirements/pip/main.txt` & `eradiate-0.23.2rc4/requirements/pip/main.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --allow-unsafe --output-file=requirements/pip/main.txt --resolver=backtracking requirements/pip/main.in
+#    pip-compile --allow-unsafe --config=pyproject.toml --output-file=requirements/pip/main.txt --resolver=backtracking requirements/pip/main.in
 #
-aenum==3.1.12
+aenum==3.1.15
     # via -r requirements/pip/main.in
 attrs==23.1.0
     # via
     #   -r requirements/pip/main.in
     #   dessinemoi
     #   environ-config
     #   pinttrs
@@ -53,29 +53,29 @@
     # via
     #   -c requirements/pip/dev.txt
     #   matplotlib
 kiwisolver==1.4.4
     # via
     #   -c requirements/pip/dev.txt
     #   matplotlib
-lazy-loader==0.2
+lazy-loader==0.3
     # via -r requirements/pip/main.in
 markdown-it-py==3.0.0
     # via
     #   -c requirements/pip/dev.txt
     #   rich
 matplotlib==3.7.1
     # via -r requirements/pip/main.in
 mdurl==0.1.2
     # via
     #   -c requirements/pip/dev.txt
     #   markdown-it-py
 netcdf4==1.6.4
     # via -r requirements/pip/main.in
-numpy==1.24.3
+numpy==1.24.4
     # via
     #   -r requirements/pip/main.in
     #   cftime
     #   contourpy
     #   matplotlib
     #   netcdf4
     #   pandas
@@ -83,29 +83,29 @@
     #   xarray
 packaging==23.1
     # via
     #   -c requirements/pip/dev.txt
     #   matplotlib
     #   pooch
     #   xarray
-pandas==2.0.2
+pandas==2.0.3
     # via
     #   -c requirements/pip/dev.txt
     #   xarray
-pillow==9.5.0
+pillow==10.0.0
     # via
     #   -c requirements/pip/dev.txt
     #   matplotlib
 pint==0.21.1
     # via
     #   -r requirements/pip/main.in
     #   pinttrs
 pinttrs==23.2.0
     # via -r requirements/pip/main.in
-platformdirs==3.6.0
+platformdirs==3.8.0
     # via
     #   -c requirements/pip/dev.txt
     #   pooch
 pooch==1.7.0
     # via -r requirements/pip/main.in
 portion==2.4.0
     # via -r requirements/pip/main.in
@@ -150,15 +150,15 @@
     # via
     #   -c requirements/pip/dev.txt
     #   portion
 tqdm==4.65.0
     # via -r requirements/pip/main.in
 typer==0.9.0
     # via -r requirements/pip/main.in
-typing-extensions==4.6.3
+typing-extensions==4.7.0
     # via
     #   -c requirements/pip/dev.txt
     #   rich
     #   typer
 tzdata==2023.3
     # via
     #   -c requirements/pip/dev.txt
```

### Comparing `eradiate-0.23.2rc3/requirements/pip/optional.txt` & `eradiate-0.23.2rc4/requirements/pip/optional.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 #
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --allow-unsafe --output-file=requirements/pip/optional.txt --resolver=backtracking requirements/pip/optional.in
+#    pip-compile --allow-unsafe --config=pyproject.toml --output-file=requirements/pip/optional.txt --resolver=backtracking requirements/pip/optional.in
 #
 aabbtree==2.8.1
     # via
     #   -c requirements/pip/dev.txt
     #   -r requirements/pip/recommended.in
 accessible-pygments==0.0.4
     # via
     #   -c requirements/pip/dev.txt
     #   pydata-sphinx-theme
-aenum==3.1.12
+aenum==3.1.15
     # via
     #   -c requirements/pip/dev.txt
     #   -r requirements/pip/main.in
 alabaster==0.7.13
     # via
     #   -c requirements/pip/dev.txt
     #   sphinx
+annotated-types==0.5.0
+    # via
+    #   -c requirements/pip/dev.txt
+    #   pydantic
 anyio==3.7.0
     # via
     #   -c requirements/pip/dev.txt
     #   jupyter-server
 appdirs==1.4.4
     # via
     #   -c requirements/pip/dev.txt
@@ -192,15 +196,15 @@
     # via
     #   -c requirements/pip/dev.txt
     #   conda-lock
 environ-config==23.2.0
     # via
     #   -c requirements/pip/dev.txt
     #   -r requirements/pip/main.in
-eradiate-mitsuba==0.0.1
+eradiate-mitsuba==0.0.2
     # via -r requirements/pip/optional.in
 exceptiongroup==1.1.1
     # via
     #   -c requirements/pip/dev.txt
     #   anyio
     #   pytest
 executing==1.2.0
@@ -270,15 +274,15 @@
     #   jupyterlab
     #   keyring
     #   matplotlib
 iniconfig==2.0.0
     # via
     #   -c requirements/pip/dev.txt
     #   pytest
-ipykernel==6.23.2
+ipykernel==6.23.3
     # via
     #   -c requirements/pip/dev.txt
     #   ipywidgets
     #   jupyterlab
 ipython==8.12.2
     # via
     #   -c requirements/pip/dev.txt
@@ -327,15 +331,15 @@
     #   jsonschema
 jsonschema[format-nongpl]==4.17.3
     # via
     #   -c requirements/pip/dev.txt
     #   jupyter-events
     #   jupyterlab-server
     #   nbformat
-jupyter-client==8.2.0
+jupyter-client==8.3.0
     # via
     #   -c requirements/pip/dev.txt
     #   ipykernel
     #   jupyter-server
     #   nbclient
 jupyter-core==5.3.1
     # via
@@ -351,15 +355,15 @@
     # via
     #   -c requirements/pip/dev.txt
     #   jupyter-server
 jupyter-lsp==2.2.0
     # via
     #   -c requirements/pip/dev.txt
     #   jupyterlab
-jupyter-server==2.6.0
+jupyter-server==2.7.0
     # via
     #   -c requirements/pip/dev.txt
     #   jupyter-lsp
     #   jupyterlab
     #   jupyterlab-server
     #   notebook-shim
 jupyter-server-terminals==0.4.4
@@ -378,27 +382,27 @@
     # via
     #   -c requirements/pip/dev.txt
     #   jupyterlab
 jupyterlab-widgets==3.0.7
     # via
     #   -c requirements/pip/dev.txt
     #   ipywidgets
-keyring==24.0.0
+keyring==24.2.0
     # via
     #   -c requirements/pip/dev.txt
     #   conda-lock
 kiwisolver==1.4.4
     # via
     #   -c requirements/pip/dev.txt
     #   matplotlib
 latexcodec==2.0.1
     # via
     #   -c requirements/pip/dev.txt
     #   pybtex
-lazy-loader==0.2
+lazy-loader==0.3
     # via
     #   -c requirements/pip/dev.txt
     #   -r requirements/pip/main.in
 livereload==2.6.3
     # via
     #   -c requirements/pip/dev.txt
     #   sphinx-autobuild
@@ -477,15 +481,15 @@
     #   -r requirements/pip/main.in
 networkx==3.1
     # via -r requirements/pip/dev.in
 notebook-shim==0.2.3
     # via
     #   -c requirements/pip/dev.txt
     #   jupyterlab
-numpy==1.24.3
+numpy==1.24.4
     # via
     #   -c requirements/pip/dev.txt
     #   -r requirements/pip/main.in
     #   astropy
     #   cftime
     #   contourpy
     #   matplotlib
@@ -512,15 +516,15 @@
     #   matplotlib
     #   nbconvert
     #   pooch
     #   pydata-sphinx-theme
     #   pytest
     #   sphinx
     #   xarray
-pandas==2.0.2
+pandas==2.0.3
     # via
     #   -c requirements/pip/dev.txt
     #   seaborn
     #   xarray
 pandocfilters==1.5.0
     # via
     #   -c requirements/pip/dev.txt
@@ -537,44 +541,44 @@
     # via
     #   -c requirements/pip/dev.txt
     #   ipython
 pickleshare==0.7.5
     # via
     #   -c requirements/pip/dev.txt
     #   ipython
-pillow==9.5.0
+pillow==10.0.0
     # via
     #   -c requirements/pip/dev.txt
     #   matplotlib
 pint==0.21.1
     # via
     #   -c requirements/pip/dev.txt
     #   -r requirements/pip/main.in
     #   pinttrs
 pinttrs==23.2.0
     # via
     #   -c requirements/pip/dev.txt
     #   -r requirements/pip/main.in
-pip-tools==6.13.0
+pip-tools==6.14.0
     # via -r requirements/pip/dev.in
 pkginfo==1.9.6
     # via
     #   -c requirements/pip/dev.txt
     #   conda-lock
 pkgutil-resolve-name==1.3.10
     # via
     #   -c requirements/pip/dev.txt
     #   jsonschema
-platformdirs==3.6.0
+platformdirs==3.8.0
     # via
     #   -c requirements/pip/dev.txt
     #   jupyter-core
     #   pooch
     #   virtualenv
-pluggy==1.0.0
+pluggy==1.2.0
     # via
     #   -c requirements/pip/dev.txt
     #   pytest
 pooch==1.7.0
     # via
     #   -c requirements/pip/dev.txt
     #   -r requirements/pip/main.in
@@ -612,18 +616,22 @@
     # via
     #   -c requirements/pip/dev.txt
     #   sphinxcontrib-bibtex
 pycparser==2.21
     # via
     #   -c requirements/pip/dev.txt
     #   cffi
-pydantic==1.10.9
+pydantic==2.0
     # via
     #   -c requirements/pip/dev.txt
     #   conda-lock
+pydantic-core==2.0.1
+    # via
+    #   -c requirements/pip/dev.txt
+    #   pydantic
 pydata-sphinx-theme==0.13.3
     # via
     #   -c requirements/pip/dev.txt
     #   sphinx-book-theme
 pyerfa==2.0.0.3
     # via
     #   -c requirements/pip/dev.txt
@@ -649,15 +657,15 @@
     # via
     #   -c requirements/pip/dev.txt
     #   build
 pyrsistent==0.19.3
     # via
     #   -c requirements/pip/dev.txt
     #   jsonschema
-pytest==7.3.2
+pytest==7.4.0
     # via
     #   -r requirements/pip/tests.in
     #   pytest-json-report
     #   pytest-metadata
 pytest-json-report==1.5.0
     # via -r requirements/pip/tests.in
 pytest-metadata==3.0.0
@@ -851,14 +859,15 @@
     #   nbconvert
 tomli==2.0.1
     # via
     #   -c requirements/pip/dev.txt
     #   build
     #   conda-lock
     #   jupyterlab
+    #   pip-tools
     #   pyproject-hooks
     #   pytest
 tomlkit==0.11.8
     # via
     #   -c requirements/pip/dev.txt
     #   conda-lock
 toolz==0.12.0
@@ -895,29 +904,31 @@
     #   nbconvert
     #   nbformat
     #   nbsphinx
 typer==0.9.0
     # via
     #   -c requirements/pip/dev.txt
     #   -r requirements/pip/main.in
-typing-extensions==4.6.3
+typing-extensions==4.7.0
     # via
     #   -c requirements/pip/dev.txt
+    #   annotated-types
     #   async-lru
     #   conda-lock
     #   ipython
     #   pydantic
+    #   pydantic-core
     #   pydata-sphinx-theme
     #   rich
     #   typer
 tzdata==2023.3
     # via
     #   -c requirements/pip/dev.txt
     #   pandas
-uri-template==1.2.0
+uri-template==1.3.0
     # via
     #   -c requirements/pip/dev.txt
     #   jsonschema
 urllib3==1.26.16
     # via
     #   -c requirements/pip/dev.txt
     #   conda-lock
@@ -936,15 +947,15 @@
     #   jsonschema
 webencodings==0.5.1
     # via
     #   -c requirements/pip/dev.txt
     #   bleach
     #   html5lib
     #   tinycss2
-websocket-client==1.6.0
+websocket-client==1.6.1
     # via
     #   -c requirements/pip/dev.txt
     #   jupyter-server
 wheel==0.40.0
     # via
     #   -c requirements/pip/dev.txt
     #   pip-tools
```

### Comparing `eradiate-0.23.2rc3/requirements/pip/recommended.txt` & `eradiate-0.23.2rc4/requirements/pip/recommended.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --allow-unsafe --output-file=requirements/pip/recommended.txt --resolver=backtracking requirements/pip/recommended.in
+#    pip-compile --allow-unsafe --config=pyproject.toml --output-file=requirements/pip/recommended.txt --resolver=backtracking requirements/pip/recommended.in
 #
 aabbtree==2.8.1
     # via -r requirements/pip/recommended.in
 anyio==3.7.0
     # via jupyter-server
 argon2-cffi==21.3.0
     # via jupyter-server
@@ -73,15 +73,15 @@
     #   jupyterlab-server
     #   nbconvert
 importlib-resources==5.12.0
     # via
     #   jsonschema
     #   jupyterlab
     #   matplotlib
-ipykernel==6.23.2
+ipykernel==6.23.3
     # via
     #   ipywidgets
     #   jupyterlab
 ipython==8.12.2
     # via
     #   -r requirements/pip/recommended.in
     #   ipykernel
@@ -103,15 +103,15 @@
 jsonpointer==2.4
     # via jsonschema
 jsonschema[format-nongpl]==4.17.3
     # via
     #   jupyter-events
     #   jupyterlab-server
     #   nbformat
-jupyter-client==8.2.0
+jupyter-client==8.3.0
     # via
     #   ipykernel
     #   jupyter-server
     #   nbclient
 jupyter-core==5.3.1
     # via
     #   ipykernel
@@ -121,15 +121,15 @@
     #   nbclient
     #   nbconvert
     #   nbformat
 jupyter-events==0.6.3
     # via jupyter-server
 jupyter-lsp==2.2.0
     # via jupyterlab
-jupyter-server==2.6.0
+jupyter-server==2.7.0
     # via
     #   jupyter-lsp
     #   jupyterlab
     #   jupyterlab-server
     #   notebook-shim
 jupyter-server-terminals==0.4.4
     # via jupyter-server
@@ -164,15 +164,15 @@
     #   jupyter-server
     #   nbclient
     #   nbconvert
 nest-asyncio==1.5.6
     # via ipykernel
 notebook-shim==0.2.3
     # via jupyterlab
-numpy==1.24.3
+numpy==1.24.4
     # via
     #   astropy
     #   contourpy
     #   matplotlib
     #   pandas
     #   pyerfa
     #   scipy
@@ -184,29 +184,29 @@
     #   astropy
     #   ipykernel
     #   jupyter-server
     #   jupyterlab
     #   jupyterlab-server
     #   matplotlib
     #   nbconvert
-pandas==2.0.2
+pandas==2.0.3
     # via seaborn
 pandocfilters==1.5.0
     # via nbconvert
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
-pillow==9.5.0
+pillow==10.0.0
     # via matplotlib
 pkgutil-resolve-name==1.3.10
     # via jsonschema
-platformdirs==3.6.0
+platformdirs==3.8.0
     # via jupyter-core
 prometheus-client==0.17.0
     # via jupyter-server
 prompt-toolkit==3.0.38
     # via ipython
 psutil==5.9.5
     # via ipykernel
@@ -304,33 +304,33 @@
     #   jupyter-events
     #   jupyter-server
     #   jupyterlab
     #   matplotlib-inline
     #   nbclient
     #   nbconvert
     #   nbformat
-typing-extensions==4.6.3
+typing-extensions==4.7.0
     # via
     #   async-lru
     #   ipython
 tzdata==2023.3
     # via pandas
-uri-template==1.2.0
+uri-template==1.3.0
     # via jsonschema
 urllib3==2.0.3
     # via requests
 wcwidth==0.2.6
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
 webencodings==0.5.1
     # via
     #   bleach
     #   tinycss2
-websocket-client==1.6.0
+websocket-client==1.6.1
     # via jupyter-server
 widgetsnbextension==4.0.7
     # via ipywidgets
 zipp==3.15.0
     # via
     #   importlib-metadata
     #   importlib-resources
```

### Comparing `eradiate-0.23.2rc3/requirements/pip/tests.txt` & `eradiate-0.23.2rc4/requirements/pip/tests.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --allow-unsafe --output-file=requirements/pip/tests.txt --resolver=backtracking requirements/pip/tests.in
+#    pip-compile --allow-unsafe --config=pyproject.toml --output-file=requirements/pip/tests.txt --resolver=backtracking requirements/pip/tests.in
 #
-aenum==3.1.12
+aenum==3.1.15
     # via
     #   -c requirements/pip/dev.txt
     #   -r requirements/pip/main.in
 attrs==23.1.0
     # via
     #   -c requirements/pip/dev.txt
     #   -r requirements/pip/main.in
@@ -69,15 +69,15 @@
     # via
     #   -c requirements/pip/dev.txt
     #   pytest
 kiwisolver==1.4.4
     # via
     #   -c requirements/pip/dev.txt
     #   matplotlib
-lazy-loader==0.2
+lazy-loader==0.3
     # via
     #   -c requirements/pip/dev.txt
     #   -r requirements/pip/main.in
 markdown-it-py==3.0.0
     # via
     #   -c requirements/pip/dev.txt
     #   rich
@@ -89,15 +89,15 @@
     # via
     #   -c requirements/pip/dev.txt
     #   markdown-it-py
 netcdf4==1.6.4
     # via
     #   -c requirements/pip/dev.txt
     #   -r requirements/pip/main.in
-numpy==1.24.3
+numpy==1.24.4
     # via
     #   -c requirements/pip/dev.txt
     #   -r requirements/pip/main.in
     #   cftime
     #   contourpy
     #   matplotlib
     #   netcdf4
@@ -107,36 +107,36 @@
 packaging==23.1
     # via
     #   -c requirements/pip/dev.txt
     #   matplotlib
     #   pooch
     #   pytest
     #   xarray
-pandas==2.0.2
+pandas==2.0.3
     # via
     #   -c requirements/pip/dev.txt
     #   xarray
-pillow==9.5.0
+pillow==10.0.0
     # via
     #   -c requirements/pip/dev.txt
     #   matplotlib
 pint==0.21.1
     # via
     #   -c requirements/pip/dev.txt
     #   -r requirements/pip/main.in
     #   pinttrs
 pinttrs==23.2.0
     # via
     #   -c requirements/pip/dev.txt
     #   -r requirements/pip/main.in
-platformdirs==3.6.0
+platformdirs==3.8.0
     # via
     #   -c requirements/pip/dev.txt
     #   pooch
-pluggy==1.0.0
+pluggy==1.2.0
     # via
     #   -c requirements/pip/dev.txt
     #   pytest
 pooch==1.7.0
     # via
     #   -c requirements/pip/dev.txt
     #   -r requirements/pip/main.in
@@ -148,15 +148,15 @@
     # via
     #   -c requirements/pip/dev.txt
     #   rich
 pyparsing==3.1.0
     # via
     #   -c requirements/pip/dev.txt
     #   matplotlib
-pytest==7.3.2
+pytest==7.4.0
     # via
     #   -r requirements/pip/tests.in
     #   pytest-json-report
     #   pytest-metadata
 pytest-json-report==1.5.0
     # via -r requirements/pip/tests.in
 pytest-metadata==3.0.0
@@ -212,15 +212,15 @@
     # via
     #   -c requirements/pip/dev.txt
     #   -r requirements/pip/main.in
 typer==0.9.0
     # via
     #   -c requirements/pip/dev.txt
     #   -r requirements/pip/main.in
-typing-extensions==4.6.3
+typing-extensions==4.7.0
     # via
     #   -c requirements/pip/dev.txt
     #   rich
     #   typer
 tzdata==2023.3
     # via
     #   -c requirements/pip/dev.txt
```

### Comparing `eradiate-0.23.2rc3/setpath.sh` & `eradiate-0.23.2rc4/setpath.sh`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/__init__.pyi` & `eradiate-0.23.2rc4/src/eradiate/__init__.pyi`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/_config.py` & `eradiate-0.23.2rc4/src/eradiate/_config.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/_factory.py` & `eradiate-0.23.2rc4/src/eradiate/_factory.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/_mode.py` & `eradiate-0.23.2rc4/src/eradiate/_mode.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/attrs.py` & `eradiate-0.23.2rc4/src/eradiate/attrs.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/cli/__init__.py` & `eradiate-0.23.2rc4/src/eradiate/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/cli/data.py` & `eradiate-0.23.2rc4/src/eradiate/cli/data.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/cli/show.py` & `eradiate-0.23.2rc4/src/eradiate/cli/show.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/cli/srf.py` & `eradiate-0.23.2rc4/src/eradiate/cli/srf.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/contexts.py` & `eradiate-0.23.2rc4/src/eradiate/contexts.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/converters.py` & `eradiate-0.23.2rc4/src/eradiate/converters.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/data/__init__.pyi` & `eradiate-0.23.2rc4/src/eradiate/data/__init__.pyi`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/data/_access.py` & `eradiate-0.23.2rc4/src/eradiate/data/_access.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/data/_blind_directory.py` & `eradiate-0.23.2rc4/src/eradiate/data/_blind_directory.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/data/_blind_online.py` & `eradiate-0.23.2rc4/src/eradiate/data/_blind_online.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/data/_core.py` & `eradiate-0.23.2rc4/src/eradiate/data/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/data/_multi.py` & `eradiate-0.23.2rc4/src/eradiate/data/_multi.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/data/_safe_directory.py` & `eradiate-0.23.2rc4/src/eradiate/data/_safe_directory.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/data/_safe_online.py` & `eradiate-0.23.2rc4/src/eradiate/data/_safe_online.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/data/_store.py` & `eradiate-0.23.2rc4/src/eradiate/data/_store.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/data/downloads.yml` & `eradiate-0.23.2rc4/src/eradiate/data/downloads.yml`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/data/downloads_development.yml` & `eradiate-0.23.2rc4/src/eradiate/data/downloads_development.yml`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/exceptions.py` & `eradiate-0.23.2rc4/src/eradiate/exceptions.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/experiments/_atmosphere.py` & `eradiate-0.23.2rc4/src/eradiate/experiments/_atmosphere.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/experiments/_canopy.py` & `eradiate-0.23.2rc4/src/eradiate/experiments/_canopy.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/experiments/_canopy_atmosphere.py` & `eradiate-0.23.2rc4/src/eradiate/experiments/_canopy_atmosphere.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/experiments/_core.py` & `eradiate-0.23.2rc4/src/eradiate/experiments/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/experiments/_dem.py` & `eradiate-0.23.2rc4/src/eradiate/experiments/_dem.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/experiments/_helpers.py` & `eradiate-0.23.2rc4/src/eradiate/experiments/_helpers.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/frame.py` & `eradiate-0.23.2rc4/src/eradiate/frame.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/kernel/__init__.py` & `eradiate-0.23.2rc4/src/eradiate/kernel/__init__.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/kernel/__init__.pyi` & `eradiate-0.23.2rc4/src/eradiate/kernel/__init__.pyi`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/kernel/_bitmap.py` & `eradiate-0.23.2rc4/src/eradiate/kernel/_bitmap.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/kernel/_bsdf.py` & `eradiate-0.23.2rc4/src/eradiate/kernel/_bsdf.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/kernel/_kernel_dict.py` & `eradiate-0.23.2rc4/src/eradiate/kernel/_kernel_dict.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/kernel/_render.py` & `eradiate-0.23.2rc4/src/eradiate/kernel/_render.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/kernel/gridvolume.py` & `eradiate-0.23.2rc4/src/eradiate/kernel/gridvolume.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/kernel/logging.py` & `eradiate-0.23.2rc4/src/eradiate/kernel/logging.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/kernel/transform.py` & `eradiate-0.23.2rc4/src/eradiate/kernel/transform.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/notebook/__init__.py` & `eradiate-0.23.2rc4/src/eradiate/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/notebook/tutorials.py` & `eradiate-0.23.2rc4/src/eradiate/notebook/tutorials.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/pipelines/__init__.pyi` & `eradiate-0.23.2rc4/src/eradiate/pipelines/__init__.pyi`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/pipelines/_aggregate.py` & `eradiate-0.23.2rc4/src/eradiate/pipelines/_aggregate.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/pipelines/_assemble.py` & `eradiate-0.23.2rc4/src/eradiate/pipelines/_assemble.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/pipelines/_compute.py` & `eradiate-0.23.2rc4/src/eradiate/pipelines/_compute.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/pipelines/_core.py` & `eradiate-0.23.2rc4/src/eradiate/pipelines/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/pipelines/_gather.py` & `eradiate-0.23.2rc4/src/eradiate/pipelines/_gather.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/plot.py` & `eradiate-0.23.2rc4/src/eradiate/plot.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/quad.py` & `eradiate-0.23.2rc4/src/eradiate/quad.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/radprops/_afgl1986.py` & `eradiate-0.23.2rc4/src/eradiate/radprops/_afgl1986.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/radprops/_core.py` & `eradiate-0.23.2rc4/src/eradiate/radprops/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/radprops/_us76_approx.py` & `eradiate-0.23.2rc4/src/eradiate/radprops/_us76_approx.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/radprops/_util_mono.py` & `eradiate-0.23.2rc4/src/eradiate/radprops/_util_mono.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/radprops/absorption.py` & `eradiate-0.23.2rc4/src/eradiate/radprops/absorption.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/radprops/rayleigh.py` & `eradiate-0.23.2rc4/src/eradiate/radprops/rayleigh.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/rng.py` & `eradiate-0.23.2rc4/src/eradiate/rng.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/atmosphere/__init__.pyi` & `eradiate-0.23.2rc4/src/eradiate/scenes/atmosphere/__init__.pyi`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/atmosphere/_core.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/atmosphere/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/atmosphere/_heterogeneous.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/atmosphere/_heterogeneous.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/atmosphere/_homogeneous.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/atmosphere/_homogeneous.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/atmosphere/_molecular_atmosphere.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/atmosphere/_molecular_atmosphere.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/atmosphere/_particle_dist.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/atmosphere/_particle_dist.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/atmosphere/_particle_layer.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/atmosphere/_particle_layer.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/biosphere/_core.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/biosphere/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/biosphere/_discrete.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/biosphere/_discrete.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/biosphere/_leaf_cloud.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/biosphere/_leaf_cloud.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/biosphere/_tree.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/biosphere/_tree.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/bsdfs/_black.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/bsdfs/_black.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/bsdfs/_checkerboard.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/bsdfs/_checkerboard.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/bsdfs/_core.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/bsdfs/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/bsdfs/_lambertian.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/bsdfs/_lambertian.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/bsdfs/_mqdiffuse.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/bsdfs/_mqdiffuse.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/bsdfs/_opacity_mask.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/bsdfs/_opacity_mask.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/bsdfs/_rpv.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/bsdfs/_rpv.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/core.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/geometry.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/geometry.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/illumination/_astro_object.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/illumination/_astro_object.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/illumination/_constant.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/illumination/_constant.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/illumination/_core.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/illumination/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/illumination/_directional.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/illumination/_directional.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/illumination/_spot.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/illumination/_spot.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/integrators/_core.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/integrators/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/integrators/_path_tracers.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/integrators/_path_tracers.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/measure/__init__.pyi` & `eradiate-0.23.2rc4/src/eradiate/scenes/measure/__init__.pyi`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/measure/_core.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/measure/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/measure/_distant.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/measure/_distant.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/measure/_distant_flux.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/measure/_distant_flux.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/measure/_hemispherical_distant.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/measure/_hemispherical_distant.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/measure/_multi_distant.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/measure/_multi_distant.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/measure/_multi_radiancemeter.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/measure/_multi_radiancemeter.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/measure/_perspective.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/measure/_perspective.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/measure/_radiancemeter.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/measure/_radiancemeter.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/phase/_blend.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/phase/_blend.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/phase/_core.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/phase/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/phase/_hg.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/phase/_hg.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/phase/_rayleigh.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/phase/_rayleigh.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/phase/_tabulated.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/phase/_tabulated.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/shapes/_buffermesh.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/shapes/_buffermesh.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/shapes/_core.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/shapes/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/shapes/_cuboid.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/shapes/_cuboid.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/shapes/_filemesh.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/shapes/_filemesh.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/shapes/_rectangle.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/shapes/_rectangle.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/shapes/_sphere.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/shapes/_sphere.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/spectra/_air_scattering_coefficient.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/spectra/_air_scattering_coefficient.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/spectra/_core.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/spectra/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/spectra/_interpolated.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/spectra/_interpolated.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/spectra/_multi_delta.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/spectra/_multi_delta.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/spectra/_solar_irradiance.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/spectra/_solar_irradiance.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/spectra/_uniform.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/spectra/_uniform.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/surface/_basic.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/surface/_basic.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/surface/_central_patch.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/surface/_central_patch.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/surface/_core.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/surface/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/scenes/surface/_dem.py` & `eradiate-0.23.2rc4/src/eradiate/scenes/surface/_dem.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/spectral/ckd.py` & `eradiate-0.23.2rc4/src/eradiate/spectral/ckd.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/spectral/index.py` & `eradiate-0.23.2rc4/src/eradiate/spectral/index.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/spectral/mono.py` & `eradiate-0.23.2rc4/src/eradiate/spectral/mono.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/srf_tools.py` & `eradiate-0.23.2rc4/src/eradiate/srf_tools.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/test_tools/plugin.py` & `eradiate-0.23.2rc4/src/eradiate/test_tools/plugin.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/test_tools/regression.py` & `eradiate-0.23.2rc4/src/eradiate/test_tools/regression.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/test_tools/types.py` & `eradiate-0.23.2rc4/src/eradiate/test_tools/types.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/test_tools/util.py` & `eradiate-0.23.2rc4/src/eradiate/test_tools/util.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/thermoprops/afgl_1986.py` & `eradiate-0.23.2rc4/src/eradiate/thermoprops/afgl_1986.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/thermoprops/us76.py` & `eradiate-0.23.2rc4/src/eradiate/thermoprops/us76.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/thermoprops/util.py` & `eradiate-0.23.2rc4/src/eradiate/thermoprops/util.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/units.py` & `eradiate-0.23.2rc4/src/eradiate/units.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/util/deprecation.py` & `eradiate-0.23.2rc4/src/eradiate/util/deprecation.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/util/misc.py` & `eradiate-0.23.2rc4/src/eradiate/util/misc.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/util/numpydoc.py` & `eradiate-0.23.2rc4/src/eradiate/util/numpydoc.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/util/sys_info.py` & `eradiate-0.23.2rc4/src/eradiate/util/sys_info.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/validators.py` & `eradiate-0.23.2rc4/src/eradiate/validators.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/warp.py` & `eradiate-0.23.2rc4/src/eradiate/warp.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/xarray/_accessors.py` & `eradiate-0.23.2rc4/src/eradiate/xarray/_accessors.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/xarray/_helpers.py` & `eradiate-0.23.2rc4/src/eradiate/xarray/_helpers.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate/xarray/interp.py` & `eradiate-0.23.2rc4/src/eradiate/xarray/interp.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate.egg-info/PKG-INFO` & `eradiate-0.23.2rc4/src/eradiate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eradiate
-Version: 0.23.2rc3
+Version: 0.23.2rc4
 Summary: A radiative transfer model for the Earth observation community
 Author: The Eradiate Team
 Maintainer: The Eradiate Team
 License: LGPLv3
 Project-URL: changelog, https://github.com/eradiate/eradiate/CHANGELOG.md
 Project-URL: documentation, https://eradiate.readthedocs.io
 Project-URL: repository, https://github.com/eradiate/eradiate
```

### Comparing `eradiate-0.23.2rc3/src/eradiate.egg-info/SOURCES.txt` & `eradiate-0.23.2rc4/src/eradiate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/src/eradiate.egg-info/requires.txt` & `eradiate-0.23.2rc4/src/eradiate.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-aenum==3.1.12
+aenum==3.1.15
 attrs==23.1.0
 certifi==2023.5.7
 cftime==1.6.2
 charset-normalizer==3.1.0
 click==8.1.3
 contourpy==1.1.0
 cycler==0.11.0
 dessinemoi==23.1.0
 drjit==0.4.1
 environ-config==23.2.0
-eradiate-mitsuba==0.0.1
+eradiate-mitsuba==0.0.2
 fonttools==4.40.0
 idna==3.4
 importlib-resources==5.12.0
 kiwisolver==1.4.4
-lazy-loader==0.2
+lazy-loader==0.3
 markdown-it-py==3.0.0
 matplotlib==3.7.1
 mdurl==0.1.2
 netcdf4==1.6.4
-numpy==1.24.3
+numpy==1.24.4
 packaging==23.1
-pandas==2.0.2
-pillow==9.5.0
+pandas==2.0.3
+pillow==10.0.0
 pint==0.21.1
 pinttrs==23.2.0
-platformdirs==3.6.0
+platformdirs==3.8.0
 pooch==1.7.0
 portion==2.4.0
 pygments==2.15.1
 pyparsing==3.1.0
 python-dateutil==2.8.2
 pytz==2023.3
 requests==2.31.0
@@ -38,15 +38,15 @@
 ruamel-yaml-clib==0.2.7
 scipy==1.10.1
 shellingham==1.5.0.post1
 six==1.16.0
 sortedcontainers==2.4.0
 tqdm==4.65.0
 typer==0.9.0
-typing-extensions==4.6.3
+typing-extensions==4.7.0
 tzdata==2023.3
 urllib3==1.26.16
 xarray==2023.1.0
 zipp==3.15.0
 
 [recommended]
 aabbtree==2.8.1
@@ -76,28 +76,28 @@
 fastjsonschema==2.17.1
 fonttools==4.40.0
 fqdn==1.5.1
 iapws==1.5.3
 idna==3.4
 importlib-metadata==6.7.0
 importlib-resources==5.12.0
-ipykernel==6.23.2
+ipykernel==6.23.3
 ipython==8.12.2
 ipywidgets==8.0.6
 isoduration==20.11.0
 jedi==0.18.2
 jinja2==3.1.2
 json5==0.9.14
 jsonpointer==2.4
 jsonschema[format-nongpl]==4.17.3
-jupyter-client==8.2.0
+jupyter-client==8.3.0
 jupyter-core==5.3.1
 jupyter-events==0.6.3
 jupyter-lsp==2.2.0
-jupyter-server==2.6.0
+jupyter-server==2.7.0
 jupyter-server-terminals==0.4.4
 jupyterlab==4.0.2
 jupyterlab-pygments==0.2.2
 jupyterlab-server==2.23.0
 jupyterlab-widgets==3.0.7
 kiwisolver==1.4.4
 markupsafe==2.1.3
@@ -105,25 +105,25 @@
 matplotlib-inline==0.1.6
 mistune==3.0.1
 nbclient==0.8.0
 nbconvert==7.6.0
 nbformat==5.9.0
 nest-asyncio==1.5.6
 notebook-shim==0.2.3
-numpy==1.24.3
+numpy==1.24.4
 overrides==7.3.1
 packaging==23.1
-pandas==2.0.2
+pandas==2.0.3
 pandocfilters==1.5.0
 parso==0.8.3
 pexpect==4.8.0
 pickleshare==0.7.5
-pillow==9.5.0
+pillow==10.0.0
 pkgutil-resolve-name==1.3.10
-platformdirs==3.6.0
+platformdirs==3.8.0
 prometheus-client==0.17.0
 prompt-toolkit==3.0.38
 psutil==5.9.5
 ptyprocess==0.7.0
 pure-eval==0.2.2
 pycparser==2.21
 pyerfa==2.0.0.3
@@ -146,17 +146,17 @@
 soupsieve==2.4.1
 stack-data==0.6.2
 terminado==0.17.1
 tinycss2==1.2.1
 tomli==2.0.1
 tornado==6.3.2
 traitlets==5.9.0
-typing-extensions==4.6.3
+typing-extensions==4.7.0
 tzdata==2023.3
-uri-template==1.2.0
+uri-template==1.3.0
 urllib3==2.0.3
 wcwidth==0.2.6
 webcolors==1.13
 webencodings==0.5.1
-websocket-client==1.6.0
+websocket-client==1.6.1
 widgetsnbextension==4.0.7
 zipp==3.15.0
```

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/data/test_blind_directory.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/data/test_blind_directory.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/data/test_blind_online.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/data/test_blind_online.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/data/test_core.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/data/test_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/data/test_datasets.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/data/test_datasets.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/data/test_multi.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/data/test_multi.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/data/test_safe_directory.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/data/test_safe_directory.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/data/test_safe_online.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/data/test_safe_online.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/experiments/test_atmosphere.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/experiments/test_atmosphere.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/experiments/test_canopy.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/experiments/test_canopy.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/experiments/test_canopy_atmosphere.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/experiments/test_canopy_atmosphere.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/experiments/test_core.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/experiments/test_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/experiments/test_dem.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/experiments/test_dem.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/experiments/test_helpers.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/experiments/test_helpers.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/kernel/test_gridvolume.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/kernel/test_gridvolume.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/kernel/test_kernel_dict.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/kernel/test_kernel_dict.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/kernel/test_logging.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/kernel/test_logging.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/kernel/test_render.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/kernel/test_render.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/kernel/test_transform.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/kernel/test_transform.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/pipelines/conftest.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/pipelines/conftest.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/pipelines/test_aggregate.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/pipelines/test_aggregate.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/pipelines/test_assemble.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/pipelines/test_assemble.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/pipelines/test_compute.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/pipelines/test_compute.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/pipelines/test_core.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/pipelines/test_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/pipelines/test_gather.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/pipelines/test_gather.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/radprops/test_absorption.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/radprops/test_absorption.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/radprops/test_afgl_1986.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/radprops/test_afgl_1986.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/radprops/test_rayleigh_scattering.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/radprops/test_rayleigh_scattering.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/radprops/test_us76_approx.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/radprops/test_us76_approx.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/radprops/test_zgrid.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/radprops/test_zgrid.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/atmosphere/test_heterogeneous.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/atmosphere/test_heterogeneous.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/atmosphere/test_homogeneous.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/atmosphere/test_homogeneous.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/atmosphere/test_molecular_atmosphere.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/atmosphere/test_molecular_atmosphere.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/atmosphere/test_particle_dist.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/atmosphere/test_particle_dist.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/atmosphere/test_particle_layer.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/atmosphere/test_particle_layer.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/biosphere/test_core.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/biosphere/test_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/biosphere/test_discrete.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/biosphere/test_discrete.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/biosphere/test_leaf_cloud.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/biosphere/test_leaf_cloud.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/biosphere/test_tree_abstract.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/biosphere/test_tree_abstract.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/biosphere/test_tree_mesh.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/biosphere/test_tree_mesh.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/bsdfs/test_black.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/bsdfs/test_black.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/bsdfs/test_checkerboard.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/bsdfs/test_checkerboard.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/bsdfs/test_lambertian.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/bsdfs/test_lambertian.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/bsdfs/test_mqdiffuse.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/bsdfs/test_mqdiffuse.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/bsdfs/test_rpv.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/bsdfs/test_rpv.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/illumination/test_astro_object.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/illumination/test_astro_object.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/illumination/test_constant.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/illumination/test_constant.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/illumination/test_directional.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/illumination/test_directional.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/illumination/test_spot.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/illumination/test_spot.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/integrators/test_path_tracers.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/integrators/test_path_tracers.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/measure/test_distant_flux.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/measure/test_distant_flux.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/measure/test_hemispherical_distant.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/measure/test_hemispherical_distant.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/measure/test_multi_distant.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/measure/test_multi_distant.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/measure/test_multi_radiancemeter.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/measure/test_multi_radiancemeter.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/measure/test_perspective.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/measure/test_perspective.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/measure/test_radiancemeter.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/measure/test_radiancemeter.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/measure/test_target.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/measure/test_target.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/phase/test_blend.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/phase/test_blend.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/phase/test_tabulated.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/phase/test_tabulated.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/shapes/test_buffermesh.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/shapes/test_buffermesh.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/shapes/test_cuboid.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/shapes/test_cuboid.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/shapes/test_filemesh.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/shapes/test_filemesh.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/shapes/test_rectangle.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/shapes/test_rectangle.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/shapes/test_sphere.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/shapes/test_sphere.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/spectra/test_air_scattering_coefficient.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/spectra/test_air_scattering_coefficient.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/spectra/test_core.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/spectra/test_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/spectra/test_interpolated.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/spectra/test_interpolated.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/spectra/test_solar_irradiance.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/spectra/test_solar_irradiance.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/spectra/test_uniform.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/spectra/test_uniform.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/surface/test_basic.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/surface/test_basic.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/surface/test_central_patch.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/surface/test_central_patch.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/surface/test_dem.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/surface/test_dem.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/scenes/test_core.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/scenes/test_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/spectral/test_ckd.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/spectral/test_ckd.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/spectral/test_index.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/spectral/test_index.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/spectral/test_mono.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/spectral/test_mono.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/test_config.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/test_config.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/test_factory.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/test_factory.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/test_frame.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/test_frame.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/test_mode.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/test_mode.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/test_quad.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/test_quad.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/test_rng.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/test_rng.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/test_srf_tools.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/test_srf_tools.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/test_tools/test_regression.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/test_tools/test_regression.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/test_units.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/test_units.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/test_validators.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/test_validators.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/test_warp.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/test_warp.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/thermoprops/test_afgl1986.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/thermoprops/test_afgl1986.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/thermoprops/test_us76.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/thermoprops/test_us76.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/thermoprops/test_util.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/thermoprops/test_util.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/util/test_deprecation.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/util/test_deprecation.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/util/test_misc.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/util/test_misc.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/xarray/conftest.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/xarray/conftest.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/01_unit/xarray/test_interp.py` & `eradiate-0.23.2rc4/tests/01_eradiate/01_unit/xarray/test_interp.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/02_system/conftest.py` & `eradiate-0.23.2rc4/tests/01_eradiate/02_system/conftest.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_albedo.py` & `eradiate-0.23.2rc4/tests/01_eradiate/02_system/test_albedo.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_atmosphere_ckd_vs_mono.py` & `eradiate-0.23.2rc4/tests/01_eradiate/02_system/test_atmosphere_ckd_vs_mono.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_atmosphere_rpv.py` & `eradiate-0.23.2rc4/tests/01_eradiate/02_system/test_atmosphere_rpv.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_basic.py` & `eradiate-0.23.2rc4/tests/01_eradiate/02_system/test_basic.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_ckd_basic.py` & `eradiate-0.23.2rc4/tests/01_eradiate/02_system/test_ckd_basic.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_compare_canopy_atmosphere.py` & `eradiate-0.23.2rc4/tests/01_eradiate/02_system/test_compare_canopy_atmosphere.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_expansion.py` & `eradiate-0.23.2rc4/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_expansion.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_flags.py` & `eradiate-0.23.2rc4/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_flags.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_parameter_id_lookup.py` & `eradiate-0.23.2rc4/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_parameter_id_lookup.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_irradiance_scaling.py` & `eradiate-0.23.2rc4/tests/01_eradiate/02_system/test_irradiance_scaling.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_kernel_render_benchmark.py` & `eradiate-0.23.2rc4/tests/01_eradiate/02_system/test_kernel_render_benchmark.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_maximum_scene_size.py` & `eradiate-0.23.2rc4/tests/01_eradiate/02_system/test_maximum_scene_size.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_mdistant_insitu.py` & `eradiate-0.23.2rc4/tests/01_eradiate/02_system/test_mdistant_insitu.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_onedim_lambertian_brf.py` & `eradiate-0.23.2rc4/tests/01_eradiate/02_system/test_onedim_lambertian_brf.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_onedim_phase.py` & `eradiate-0.23.2rc4/tests/01_eradiate/02_system/test_onedim_phase.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_onedim_symmetry.py` & `eradiate-0.23.2rc4/tests/01_eradiate/02_system/test_onedim_symmetry.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/02_system/test_spectral_loop.py` & `eradiate-0.23.2rc4/tests/01_eradiate/02_system/test_spectral_loop.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/03_regression/atmospheres/test_rpv_afgl1986.py` & `eradiate-0.23.2rc4/tests/01_eradiate/03_regression/atmospheres/test_rpv_afgl1986.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/03_regression/atmospheres/test_rpv_afgl1986_continental.py` & `eradiate-0.23.2rc4/tests/01_eradiate/03_regression/atmospheres/test_rpv_afgl1986_continental.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/03_regression/rami4atm/test_rami4atm_hom00_bla_sd2s_m03_z30a000_brfpp.py` & `eradiate-0.23.2rc4/tests/01_eradiate/03_regression/rami4atm/test_rami4atm_hom00_bla_sd2s_m03_z30a000_brfpp.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/03_regression/romc/test_het01.py` & `eradiate-0.23.2rc4/tests/01_eradiate/03_regression/romc/test_het01.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/03_regression/romc/test_het04.py` & `eradiate-0.23.2rc4/tests/01_eradiate/03_regression/romc/test_het04.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/03_regression/romc/test_het06.py` & `eradiate-0.23.2rc4/tests/01_eradiate/03_regression/romc/test_het06.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/01_eradiate/conftest.py` & `eradiate-0.23.2rc4/tests/01_eradiate/conftest.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc3/tests/conftest.py` & `eradiate-0.23.2rc4/tests/conftest.py`

 * *Files identical despite different names*

