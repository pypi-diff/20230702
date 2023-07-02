# Comparing `tmp/approvaltests-8.2.5.tar.gz` & `tmp/approvaltests-8.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "approvaltests-8.2.5.tar", last modified: Sun Mar 26 17:58:52 2023, max compression
+gzip compressed data, was "approvaltests-8.3.0.tar", last modified: Sun Jul  2 05:59:59 2023, max compression
```

## Comparing `approvaltests-8.2.5.tar` & `approvaltests-8.3.0.tar`

### file list

```diff
@@ -1,95 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:58:52.050905 approvaltests-8.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-03-26 17:58:35.000000 approvaltests-8.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-26 17:58:35.000000 approvaltests-8.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13549 2023-03-26 17:58:52.050905 approvaltests-8.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12482 2023-03-26 17:58:35.000000 approvaltests-8.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:58:52.046905 approvaltests-8.2.5/approvaltests/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/approval_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    14390 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/approvals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/asserts.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/binary_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/combination_approvals.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/commandline_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:58:52.046905 approvaltests-8.2.5/approvaltests/core/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/core/comparator.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/core/format_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/core/namer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/core/options.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/core/reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/core/scenario_namer.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/core/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/existing_file_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/file_approver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:58:52.046905 approvaltests-8.2.5/approvaltests/mrjob/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/mrjob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/mrjob/mrjob_approvals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:58:52.050905 approvaltests-8.2.5/approvaltests/namer/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/namer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/namer/cli_namer.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/namer/default_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/namer/default_namer_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/namer/namer_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/namer/stack_frame_namer.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/pairwise_combinations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:58:52.050905 approvaltests-8.2.5/approvaltests/pytest/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/pytest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/pytest/py_test_namer.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/reporter_missing_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:58:52.050905 approvaltests-8.2.5/approvaltests/reporters/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/reporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/reporters/clipboard_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/reporters/default_reporter_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/reporters/diff_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/reporters/file_capture_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/reporters/first_working_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/reporters/generic_diff_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/reporters/generic_diff_reporter_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/reporters/generic_diff_reporter_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/reporters/multi_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/reporters/python_native_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/reporters/quiet_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/reporters/received_file_launcher_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/reporters/report_all_to_clipboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/reporters/report_by_creating_diff_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/reporters/report_on_cyber_dojo.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/reporters/report_to_diff_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/reporters/report_with_beyond_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/reporters/report_with_diff_command_line.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/reporters/report_with_vscode.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/reporters/reporter_that_automatically_approves.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/reporters/reporters.json
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/reporters/testing_reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:58:52.050905 approvaltests-8.2.5/approvaltests/scrubbers/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/scrubbers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/scrubbers/date_scrubber.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/scrubbers/scrubbers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/storyboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/string_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:58:52.050905 approvaltests-8.2.5/approvaltests/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/utilities/command_line_approvals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:58:52.050905 approvaltests-8.2.5/approvaltests/utilities/logger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/utilities/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/utilities/logger/simple_logger_approvals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:58:52.050905 approvaltests-8.2.5/approvaltests/verifiable_objects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/verifiable_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-26 17:58:35.000000 approvaltests-8.2.5/approvaltests/verifiable_objects/formatter_of_argparse_namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-26 17:58:46.000000 approvaltests-8.2.5/approvaltests/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:58:52.046905 approvaltests-8.2.5/approvaltests.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13549 2023-03-26 17:58:52.000000 approvaltests-8.2.5/approvaltests.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-03-26 17:58:52.000000 approvaltests-8.2.5/approvaltests.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 17:58:52.000000 approvaltests-8.2.5/approvaltests.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-03-26 17:58:52.000000 approvaltests-8.2.5/approvaltests.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-26 17:58:52.000000 approvaltests-8.2.5/approvaltests.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-03-26 17:58:35.000000 approvaltests-8.2.5/requirements.prod.extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-26 17:58:35.000000 approvaltests-8.2.5/requirements.prod.required.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-26 17:58:35.000000 approvaltests-8.2.5/requirements.prod.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-26 17:58:52.050905 approvaltests-8.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-03-26 17:58:35.000000 approvaltests-8.2.5/setup.publish.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-03-26 17:58:35.000000 approvaltests-8.2.5/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-03-26 17:58:35.000000 approvaltests-8.2.5/setup_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-26 17:58:46.000000 approvaltests-8.2.5/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:59:59.269121 approvaltests-8.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-07-02 05:59:43.000000 approvaltests-8.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-02 05:59:43.000000 approvaltests-8.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13549 2023-07-02 05:59:59.269121 approvaltests-8.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12482 2023-07-02 05:59:43.000000 approvaltests-8.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:59:59.265121 approvaltests-8.3.0/approvaltests/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/approval_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15013 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/approvals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/asserts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/binary_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/combination_approvals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/commandline_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:59:59.265121 approvaltests-8.3.0/approvaltests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/core/comparator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/core/format_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/core/namer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/core/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/core/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/core/scenario_namer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/core/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/existing_file_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/file_approver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:59:59.265121 approvaltests-8.3.0/approvaltests/mrjob/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/mrjob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/mrjob/mrjob_approvals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:59:59.265121 approvaltests-8.3.0/approvaltests/namer/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/namer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/namer/cli_namer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/namer/default_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/namer/default_namer_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/namer/namer_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/namer/stack_frame_namer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/pairwise_combinations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:59:59.265121 approvaltests-8.3.0/approvaltests/pytest/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/pytest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/pytest/py_test_namer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/reporter_missing_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:59:59.269121 approvaltests-8.3.0/approvaltests/reporters/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/reporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/reporters/clipboard_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/reporters/default_reporter_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/reporters/diff_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/reporters/executable_command_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/reporters/file_capture_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/reporters/first_working_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/reporters/generic_diff_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/reporters/generic_diff_reporter_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/reporters/generic_diff_reporter_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/reporters/multi_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/reporters/python_native_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/reporters/quiet_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/reporters/received_file_launcher_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/reporters/report_all_to_clipboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/reporters/report_by_creating_diff_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/reporters/report_on_cyber_dojo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/reporters/report_to_diff_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/reporters/report_with_beyond_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/reporters/report_with_diff_command_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/reporters/report_with_vscode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/reporters/reporter_that_automatically_approves.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/reporters/reporters.json
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/reporters/testing_reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:59:59.269121 approvaltests-8.3.0/approvaltests/scrubbers/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/scrubbers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/scrubbers/date_scrubber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/scrubbers/scrubbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/storyboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/string_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:59:59.269121 approvaltests-8.3.0/approvaltests/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/utilities/command_line_approvals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:59:59.269121 approvaltests-8.3.0/approvaltests/utilities/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/utilities/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/utilities/logger/simple_logger_approvals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:59:59.269121 approvaltests-8.3.0/approvaltests/verifiable_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/verifiable_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-02 05:59:43.000000 approvaltests-8.3.0/approvaltests/verifiable_objects/formatter_of_argparse_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-02 05:59:53.000000 approvaltests-8.3.0/approvaltests/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:59:59.265121 approvaltests-8.3.0/approvaltests.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13549 2023-07-02 05:59:59.000000 approvaltests-8.3.0/approvaltests.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-02 05:59:59.000000 approvaltests-8.3.0/approvaltests.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 05:59:59.000000 approvaltests-8.3.0/approvaltests.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-02 05:59:59.000000 approvaltests-8.3.0/approvaltests.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-02 05:59:59.000000 approvaltests-8.3.0/approvaltests.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-02 05:59:43.000000 approvaltests-8.3.0/requirements.prod.extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-02 05:59:43.000000 approvaltests-8.3.0/requirements.prod.required.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-02 05:59:43.000000 approvaltests-8.3.0/requirements.prod.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-02 05:59:59.269121 approvaltests-8.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-02 05:59:43.000000 approvaltests-8.3.0/setup.publish.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-02 05:59:43.000000 approvaltests-8.3.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-02 05:59:43.000000 approvaltests-8.3.0/setup_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-02 05:59:53.000000 approvaltests-8.3.0/version.py
```

### Comparing `approvaltests-8.2.5/LICENSE` & `approvaltests-8.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `approvaltests-8.2.5/PKG-INFO` & `approvaltests-8.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: approvaltests
-Version: 8.2.5
+Version: 8.3.0
 Summary: Assertion/verification library to aid testing
 Home-page: https://github.com/approvals/ApprovalTests.Python
 Author: ApprovalTests Contributors
 Author-email: llewellyn.falco@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `approvaltests-8.2.5/README.md` & `approvaltests-8.3.0/README.md`

 * *Files identical despite different names*

### Comparing `approvaltests-8.2.5/approvaltests/approvals.py` & `approvaltests-8.3.0/approvaltests/approvals.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 import xml.dom.minidom
 from contextlib import contextmanager
 from pathlib import Path
 from typing import Callable, List, Optional, Any, ByteString, Iterator
 
 import approvaltests.reporters.default_reporter_factory
 from approval_utilities import utils
+from approval_utilities.approvaltests.core.executable_command import ExecutableCommand
 from approval_utilities.approvaltests.core.verifiable import Verifiable
 from approval_utilities.list_utils import format_list
 from approval_utilities.utilities.exceptions.exception_utils import to_string
 from approval_utilities.utilities.map_reduce import first
+from approvaltests import Options
 from approvaltests.approval_exception import ApprovalException
 from approvaltests.binary_writer import BinaryWriter
 from approvaltests.core import Reporter, Writer
 from approvaltests.core.format_wrapper import FormatWrapper, AlwaysMatch
 from approvaltests.core.namer import Namer
 from approvaltests.core.options import Options
 from approvaltests.core.scenario_namer import ScenarioNamer
 from approvaltests.existing_file_writer import ExistingFileWriter
 from approvaltests.file_approver import FileApprover
 from approvaltests.namer.stack_frame_namer import StackFrameNamer
 from approvaltests.reporters.diff_reporter import DiffReporter
+from approvaltests.reporters.executable_command_reporter import (
+    ExecutableCommandReporter,
+)
 from approvaltests.string_writer import StringWriter
 from approvaltests.verifiable_objects.formatter_of_argparse_namespace import (
     FormatterWrapperOfArgparseNamespace,
 )
 
 __unittest = True
 __tracebackhide__ = True
@@ -51,15 +56,15 @@
     data: Any,
     reporter: Optional[Reporter] = None,
     namer: Optional[Namer] = None,
     encoding: Optional[str] = None,
     errors: Optional[str] = None,
     newline: Optional[str] = None,
     *,  # enforce keyword arguments - https://www.python.org/dev/peps/pep-3102/
-    options: Optional[Options] = None
+    options: Optional[Options] = None,
 ) -> None:
     """Verify string data against a previously approved version of the string.
 
     Args:
         data: A string containing the data to be compared with approved data from a previous run.
             On Python 2 this can be a bytes, str, or unicode object. On Python 3 this should be
             a str object.
@@ -123,15 +128,15 @@
     return wrapper.wrap(data)
 
 
 def verify_binary(
     data: ByteString,
     file_extension_with_dot: str,
     *,  # enforce keyword arguments - https://www.python.org/dev/peps/pep-3102/
-    options: Optional[Options] = None
+    options: Optional[Options] = None,
 ) -> None:
     options = initialize_options(options, None).for_file.with_extension(
         file_extension_with_dot
     )
     verify_with_namer_and_writer(
         options.namer,
         BinaryWriter(data, file_extension_with_dot),
@@ -154,15 +159,15 @@
     data: Any,
     namer: Namer,
     reporter: Optional[Reporter] = None,
     encoding: Optional[str] = None,
     errors: Optional[str] = None,
     newline: Optional[str] = None,
     *,  # enforce keyword arguments - https://www.python.org/dev/peps/pep-3102/
-    options: Optional[Options] = None
+    options: Optional[Options] = None,
 ) -> None:
     """Verify string data against a previously approved version of the string.
 
     Args:
         data: A string containing the data to be compared with approved data from a previous run.
             On Python 2 this can be a bytes, str, or unicode object. On Python 3 this should be
             a str object.
@@ -202,29 +207,29 @@
 
 
 def verify_with_namer_and_writer(
     namer: Namer,
     writer: Writer,
     reporter: Optional[Reporter] = None,
     *,  # enforce keyword arguments - https://www.python.org/dev/peps/pep-3102/
-    options: Optional[Options] = None
+    options: Optional[Options] = None,
 ) -> None:
     options = initialize_options(options, reporter)
     error = FileApprover.verify(namer, writer, options.reporter, options.comparator)
     if error:
         raise ApprovalException(error)
 
 
 # begin-snippet: verify_as_json
 def verify_as_json(
     object_to_verify,
     reporter=None,
     *,  # enforce keyword arguments - https://www.python.org/dev/peps/pep-3102/
     deserialize_json_fields=False,
-    options: Optional[Options] = None
+    options: Optional[Options] = None,
 ):
     if deserialize_json_fields:
         object_to_verify = utils.deserialize_json_fields(object_to_verify)
     options = initialize_options(options, reporter)
     json_text = utils.to_json(object_to_verify) + "\n"
     verify(json_text, None, encoding="utf-8", newline="\n", options=options)
 
@@ -232,30 +237,30 @@
 # end-snippet
 
 
 def verify_xml(
     xml_string: str,
     reporter: None = None,
     *,  # enforce keyword arguments - https://www.python.org/dev/peps/pep-3102/
-    options: Optional[Options] = None
+    options: Optional[Options] = None,
 ) -> None:
     options = initialize_options(options, reporter)
     try:
         dom = xml.dom.minidom.parseString(xml_string)
         pretty_xml = dom.toprettyxml()
     except Exception:
         pretty_xml = xml_string
 
     verify(pretty_xml, options=options.for_file.with_extension(".xml"))
 
 
 def verify_html(
     html_string: str,
     *,  # enforce keyword arguments - https://www.python.org/dev/peps/pep-3102/
-    options: Optional[Options] = None
+    options: Optional[Options] = None,
 ) -> None:
     options = initialize_options(options)
     try:
         from bs4 import BeautifulSoup
 
         pretty_html = BeautifulSoup(html_string, "html.parser").prettify()
     except Exception:
@@ -264,15 +269,15 @@
     verify(pretty_html, options=options.for_file.with_extension(".html"))
 
 
 def verify_file(
     file_name: str,
     reporter: Reporter = None,
     *,  # enforce keyword arguments - https://www.python.org/dev/peps/pep-3102/
-    options: Optional[Options] = None
+    options: Optional[Options] = None,
 ) -> None:
     """Verify the contents of a text file against previously approved contents.
 
     Args:
         file_name: The path to a file. The file will be opened in text mode.
 
         reporter: An optional Reporter. If None (the default), the default reporter
@@ -298,15 +303,15 @@
     alist: List[str],
     formatter: Optional[Callable] = None,
     reporter: Optional[DiffReporter] = None,
     encoding: None = None,
     errors: None = None,
     newline: None = None,
     *,  # enforce keyword arguments - https://www.python.org/dev/peps/pep-3102/
-    options: Optional[Options] = None
+    options: Optional[Options] = None,
 ) -> None:
     """Verify a collection of items against a previously approved collection.
 
     Args:
         header: A header line string to be included before the list of items.
 
         alist: An iterable series of objects, a string representation of each of which will be
@@ -346,15 +351,15 @@
         text, None, encoding=encoding, errors=errors, newline=newline, options=options
     )
 
 
 def verify_exception(
     code_that_throws_exception: Callable,
     *,  # enforce keyword arguments - https://www.python.org/dev/peps/pep-3102/
-    options: Optional[Options] = None
+    options: Optional[Options] = None,
 ):
     result = ""
     try:
         code_that_throws_exception()
         result = "No exception was thrown"
     except BaseException as exception:
         result = to_string(exception)
@@ -365,7 +370,21 @@
     return ScenarioNamer(get_default_namer(), *scenario_name)
 
 
 def delete_approved_file():
     filename = Path(get_default_namer().get_approved_filename())
     if filename.exists():
         filename.unlink()
+
+
+def verify_executable_command(
+    command: ExecutableCommand,
+    *,  # enforce keyword arguments - https://www.python.org/dev/peps/pep-3102/
+    options: Optional[Options] = None,
+):
+    options = initialize_options(options)
+    verify(
+        command.get_command(),
+        options=options.with_reporter(
+            ExecutableCommandReporter(command, options.reporter)
+        ),
+    )
```

### Comparing `approvaltests-8.2.5/approvaltests/asserts.py` & `approvaltests-8.3.0/approvaltests/asserts.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.2.5/approvaltests/binary_writer.py` & `approvaltests-8.3.0/approvaltests/binary_writer.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.2.5/approvaltests/combination_approvals.py` & `approvaltests-8.3.0/approvaltests/combination_approvals.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.2.5/approvaltests/command.py` & `approvaltests-8.3.0/approvaltests/command.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.2.5/approvaltests/commandline_interface.py` & `approvaltests-8.3.0/approvaltests/commandline_interface.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.2.5/approvaltests/core/comparator.py` & `approvaltests-8.3.0/approvaltests/core/comparator.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.2.5/approvaltests/core/options.py` & `approvaltests-8.3.0/approvaltests/core/options.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.2.5/approvaltests/core/reporter.py` & `approvaltests-8.3.0/approvaltests/core/reporter.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.2.5/approvaltests/core/scenario_namer.py` & `approvaltests-8.3.0/approvaltests/core/scenario_namer.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.2.5/approvaltests/existing_file_writer.py` & `approvaltests-8.3.0/approvaltests/existing_file_writer.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.2.5/approvaltests/file_approver.py` & `approvaltests-8.3.0/approvaltests/file_approver.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.2.5/approvaltests/mrjob/mrjob_approvals.py` & `approvaltests-8.3.0/approvaltests/mrjob/mrjob_approvals.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.2.5/approvaltests/namer/default_namer_factory.py` & `approvaltests-8.3.0/approvaltests/namer/default_namer_factory.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.2.5/approvaltests/namer/namer_base.py` & `approvaltests-8.3.0/approvaltests/namer/namer_base.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.2.5/approvaltests/namer/stack_frame_namer.py` & `approvaltests-8.3.0/approvaltests/namer/stack_frame_namer.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.2.5/approvaltests/pytest/py_test_namer.py` & `approvaltests-8.3.0/approvaltests/pytest/py_test_namer.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.2.5/approvaltests/reporters/__init__.py` & `approvaltests-8.3.0/approvaltests/reporters/__init__.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.2.5/approvaltests/reporters/clipboard_reporter.py` & `approvaltests-8.3.0/approvaltests/reporters/clipboard_reporter.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.2.5/approvaltests/reporters/default_reporter_factory.py` & `approvaltests-8.3.0/approvaltests/reporters/default_reporter_factory.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.2.5/approvaltests/reporters/diff_reporter.py` & `approvaltests-8.3.0/approvaltests/reporters/diff_reporter.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.2.5/approvaltests/reporters/file_capture_reporter.py` & `approvaltests-8.3.0/approvaltests/reporters/file_capture_reporter.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.2.5/approvaltests/reporters/first_working_reporter.py` & `approvaltests-8.3.0/approvaltests/reporters/first_working_reporter.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.2.5/approvaltests/reporters/generic_diff_reporter.py` & `approvaltests-8.3.0/approvaltests/reporters/generic_diff_reporter.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.2.5/approvaltests/reporters/generic_diff_reporter_factory.py` & `approvaltests-8.3.0/approvaltests/reporters/generic_diff_reporter_factory.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.2.5/approvaltests/reporters/python_native_reporter.py` & `approvaltests-8.3.0/approvaltests/reporters/python_native_reporter.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.2.5/approvaltests/reporters/received_file_launcher_reporter.py` & `approvaltests-8.3.0/approvaltests/reporters/received_file_launcher_reporter.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.2.5/approvaltests/reporters/report_all_to_clipboard.py` & `approvaltests-8.3.0/approvaltests/reporters/report_all_to_clipboard.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.2.5/approvaltests/reporters/report_by_creating_diff_file.py` & `approvaltests-8.3.0/approvaltests/reporters/report_by_creating_diff_file.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.2.5/approvaltests/reporters/report_to_diff_engine.py` & `approvaltests-8.3.0/approvaltests/reporters/report_to_diff_engine.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.2.5/approvaltests/reporters/report_with_beyond_compare.py` & `approvaltests-8.3.0/approvaltests/reporters/report_with_beyond_compare.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.2.5/approvaltests/reporters/reporters.json` & `approvaltests-8.3.0/approvaltests/reporters/reporters.json`

 * *Files identical despite different names*

### Comparing `approvaltests-8.2.5/approvaltests/scrubbers/date_scrubber.py` & `approvaltests-8.3.0/approvaltests/scrubbers/date_scrubber.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.2.5/approvaltests/scrubbers/scrubbers.py` & `approvaltests-8.3.0/approvaltests/scrubbers/scrubbers.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.2.5/approvaltests/storyboard.py` & `approvaltests-8.3.0/approvaltests/storyboard.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.2.5/approvaltests/string_writer.py` & `approvaltests-8.3.0/approvaltests/string_writer.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.2.5/approvaltests/utilities/command_line_approvals.py` & `approvaltests-8.3.0/approvaltests/utilities/command_line_approvals.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.2.5/approvaltests/utilities/logger/simple_logger_approvals.py` & `approvaltests-8.3.0/approvaltests/utilities/logger/simple_logger_approvals.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.2.5/approvaltests/verifiable_objects/formatter_of_argparse_namespace.py` & `approvaltests-8.3.0/approvaltests/verifiable_objects/formatter_of_argparse_namespace.py`

 * *Files identical despite different names*

### Comparing `approvaltests-8.2.5/approvaltests.egg-info/PKG-INFO` & `approvaltests-8.3.0/approvaltests.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: approvaltests
-Version: 8.2.5
+Version: 8.3.0
 Summary: Assertion/verification library to aid testing
 Home-page: https://github.com/approvals/ApprovalTests.Python
 Author: ApprovalTests Contributors
 Author-email: llewellyn.falco@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `approvaltests-8.2.5/approvaltests.egg-info/SOURCES.txt` & `approvaltests-8.3.0/approvaltests.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 approvaltests/namer/stack_frame_namer.py
 approvaltests/pytest/__init__.py
 approvaltests/pytest/py_test_namer.py
 approvaltests/reporters/__init__.py
 approvaltests/reporters/clipboard_reporter.py
 approvaltests/reporters/default_reporter_factory.py
 approvaltests/reporters/diff_reporter.py
+approvaltests/reporters/executable_command_reporter.py
 approvaltests/reporters/file_capture_reporter.py
 approvaltests/reporters/first_working_reporter.py
 approvaltests/reporters/generic_diff_reporter.py
 approvaltests/reporters/generic_diff_reporter_config.py
 approvaltests/reporters/generic_diff_reporter_factory.py
 approvaltests/reporters/multi_reporter.py
 approvaltests/reporters/python_native_reporter.py
```

### Comparing `approvaltests-8.2.5/setup_utils.py` & `approvaltests-8.3.0/setup_utils.py`

 * *Files identical despite different names*

