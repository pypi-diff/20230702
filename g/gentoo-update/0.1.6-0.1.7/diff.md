# Comparing `tmp/gentoo-update-0.1.6.tar.gz` & `tmp/gentoo-update-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gentoo-update-0.1.6.tar", last modified: Wed Jun 21 18:59:06 2023, max compression
+gzip compressed data, was "gentoo-update-0.1.7.tar", last modified: Sun Jul  2 21:04:33 2023, max compression
```

## Comparing `gentoo-update-0.1.6.tar` & `gentoo-update-0.1.7.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:59:06.958921 gentoo-update-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-21 18:58:57.000000 gentoo-update-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-21 18:58:57.000000 gentoo-update-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-06-21 18:59:06.958921 gentoo-update-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-21 18:58:57.000000 gentoo-update-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:59:06.958921 gentoo-update-0.1.6/gentoo_update/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-21 18:58:57.000000 gentoo-update-0.1.6/gentoo_update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-06-21 18:58:57.000000 gentoo-update-0.1.6/gentoo_update/gentoo_update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:59:06.958921 gentoo-update-0.1.6/gentoo_update/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5610 2023-06-21 18:58:57.000000 gentoo-update-0.1.6/gentoo_update/scripts/updater.sh
--rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-06-21 18:58:57.000000 gentoo-update-0.1.6/gentoo_update/shell_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:59:06.958921 gentoo-update-0.1.6/gentoo_update.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-06-21 18:59:06.000000 gentoo-update-0.1.6/gentoo_update.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-21 18:59:06.000000 gentoo-update-0.1.6/gentoo_update.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 18:59:06.000000 gentoo-update-0.1.6/gentoo_update.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-21 18:59:06.000000 gentoo-update-0.1.6/gentoo_update.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-21 18:59:06.000000 gentoo-update-0.1.6/gentoo_update.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-21 18:59:06.958921 gentoo-update-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-21 18:58:57.000000 gentoo-update-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:59:06.958921 gentoo-update-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-21 18:58:57.000000 gentoo-update-0.1.6/tests/test_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 21:04:33.186520 gentoo-update-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-02 21:04:24.000000 gentoo-update-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-02 21:04:24.000000 gentoo-update-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-07-02 21:04:33.186520 gentoo-update-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-02 21:04:24.000000 gentoo-update-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 21:04:33.186520 gentoo-update-0.1.7/gentoo_update/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-02 21:04:24.000000 gentoo-update-0.1.7/gentoo_update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-02 21:04:24.000000 gentoo-update-0.1.7/gentoo_update/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-07-02 21:04:24.000000 gentoo-update-0.1.7/gentoo_update/gentoo_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-07-02 21:04:24.000000 gentoo-update-0.1.7/gentoo_update/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 21:04:33.186520 gentoo-update-0.1.7/gentoo_update/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6057 2023-07-02 21:04:24.000000 gentoo-update-0.1.7/gentoo_update/scripts/updater.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-07-02 21:04:24.000000 gentoo-update-0.1.7/gentoo_update/shell_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 21:04:33.186520 gentoo-update-0.1.7/gentoo_update.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-07-02 21:04:33.000000 gentoo-update-0.1.7/gentoo_update.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-02 21:04:33.000000 gentoo-update-0.1.7/gentoo_update.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 21:04:33.000000 gentoo-update-0.1.7/gentoo_update.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-02 21:04:33.000000 gentoo-update-0.1.7/gentoo_update.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-02 21:04:33.000000 gentoo-update-0.1.7/gentoo_update.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-02 21:04:33.186520 gentoo-update-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-02 21:04:24.000000 gentoo-update-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 21:04:33.186520 gentoo-update-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-02 21:04:24.000000 gentoo-update-0.1.7/tests/test_updater.py
```

### Comparing `gentoo-update-0.1.6/LICENSE` & `gentoo-update-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gentoo-update-0.1.6/PKG-INFO` & `gentoo-update-0.1.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gentoo-update
-Version: 0.1.6
+Version: 0.1.7
 Summary: Gentoo Linux updater
 Home-page: https://github.com/Lab-Brat/gentoo_update
 Author: Lab-Brat
 Author-email: labbrat_social@pm.me
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
@@ -17,27 +17,31 @@
 
 `gentoo-update` is a tool that automates updates on Gentoo Linux. 
 By default it only installs security updates from [GLSA](https://security.gentoo.org/glsa/), 
 but it can also be used to update all packages on the system. i.e. `@world`.  
 
 This project 
 [originates](https://wiki.gentoo.org/wiki/Google_Summer_of_Code/2023/Ideas/Automated_Gentoo_system_updater) 
-from 2023 Google Summer of Code.
+from 2023 Google Summer of Code, more about it can be found in the 
+[blog post](https://labbrat.net/blog/gsoc2023/gentoo_update_intro/) and 
+[Gentoo Forums](https://forums.gentoo.org/viewtopic-p-8793827.html#8793827).  
 
 
 #### Usage
 `gentoo-update` is in [GURU](https://wiki.gentoo.org/wiki/Project:GURU) 
 overlay, and can be installed using `emerge`:
 ```bash
 emerge --ask app-admin/gentoo_update
 ```
 
-Alternatively, updater can be installed with pip:
-```
-pip install gentoo_update --break-system-packages
+Alternatively, it can be installed with pip in a virtual environment:
+```bash
+python -m venv gentoo_update
+source gentoo_update/bin/activate
+python -m pip install gentoo_update
 ```
 
 The updater creates a subdirectory in Portage's default `PORTAGE_LOGDIR` located at `/var/log/portage/gentoo-update`. 
 However, if this variable is set to a different value in `make.conf`, it will use the new location instead of the default.  
 
 Here are some usage examples:
 * Basic security update
```

### Comparing `gentoo-update-0.1.6/README.md` & `gentoo-update-0.1.7/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -2,27 +2,31 @@
 
 `gentoo-update` is a tool that automates updates on Gentoo Linux. 
 By default it only installs security updates from [GLSA](https://security.gentoo.org/glsa/), 
 but it can also be used to update all packages on the system. i.e. `@world`.  
 
 This project 
 [originates](https://wiki.gentoo.org/wiki/Google_Summer_of_Code/2023/Ideas/Automated_Gentoo_system_updater) 
-from 2023 Google Summer of Code.
+from 2023 Google Summer of Code, more about it can be found in the 
+[blog post](https://labbrat.net/blog/gsoc2023/gentoo_update_intro/) and 
+[Gentoo Forums](https://forums.gentoo.org/viewtopic-p-8793827.html#8793827).  
 
 
 #### Usage
 `gentoo-update` is in [GURU](https://wiki.gentoo.org/wiki/Project:GURU) 
 overlay, and can be installed using `emerge`:
 ```bash
 emerge --ask app-admin/gentoo_update
 ```
 
-Alternatively, updater can be installed with pip:
-```
-pip install gentoo_update --break-system-packages
+Alternatively, it can be installed with pip in a virtual environment:
+```bash
+python -m venv gentoo_update
+source gentoo_update/bin/activate
+python -m pip install gentoo_update
 ```
 
 The updater creates a subdirectory in Portage's default `PORTAGE_LOGDIR` located at `/var/log/portage/gentoo-update`. 
 However, if this variable is set to a different value in `make.conf`, it will use the new location instead of the default.  
 
 Here are some usage examples:
 * Basic security update
```

### Comparing `gentoo-update-0.1.6/gentoo_update/gentoo_update.py` & `gentoo-update-0.1.7/gentoo_update/gentoo_update.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import argparse
 from .shell_runner import ShellRunner
+from ._version import __version__
 
-__version__ = "0.1.6"
 current_path = os.path.dirname(os.path.realpath(__file__))
 
 
 def create_cli() -> argparse.Namespace:
     """
     Define CLI command flags using argparse.
 
@@ -38,21 +38,19 @@
         "Example:\n"
         "--args 'quiet-build=n color=y keep-going'",
     )
     parser.add_argument(
         "-c",
         "--config-update-mode",
         default="ignore",
-        choices=["ignore", "merge", "interactive", "dispatch"],
+        choices=["ignore", "merge"],
         help="Set the way new configurations are handled after an update.\n"
         "Options:\n"
         "* ignore: do not update configuration files at all.\n"
         "* merge: automatically merge changes in configuration files.\n"
-        "* interactive: launch interactive etc-upgrade.\n"
-        "* dispatch: launch interactive dispatch-conf.\n"
         "Default: ignore\n",
     )
     parser.add_argument(
         "-d",
         "--daemon-restart",
         default="n",
         choices=["y", "n"],
@@ -85,14 +83,21 @@
         "-q",
         "--quiet",
         default="n",
         choices=["y", "n"],
         help="Do not show logs on the terminal screen.\n" "Default: n\n",
     )
     parser.add_argument(
+        "-r",
+        "--report",
+        default="n",
+        choices=["y", "n"],
+        help="Show report or the last update log.\n",
+    )
+    parser.add_argument(
         "--version",
         action="version",
         version=__version__,
         help="Print updater version.\n",
     )
 
     args = parser.parse_args()
@@ -101,37 +106,36 @@
 
 def add_prefixes(args: str) -> str:
     """
     Function to add prefixes to a list of arguments passed to
     --update-mode full.
 
     Parameters:
-    args_list (str): A string of space separated arguments without prefixes 
+    args_list (str): A string of space separated arguments without prefixes
         example: "quiet-build=n color=y keep-going"
 
     Returns:
     str: A new string of space separated arguments with added prefixes,
         example: "--quiet-build=n --color=y --keep-going"
     """
     args = args.split(" ")
-    print(args)
     prefixed_args = []
 
     for arg in args:
         if len(arg) == 1:
             prefixed_args.append("-" + arg)
         else:
             prefixed_args.append("--" + arg)
-    print(prefixed_args)
     return " ".join(prefixed_args)
 
 
 def main() -> None:
     args = create_cli()
-    runner = ShellRunner(args.quiet)
+
+    runner = ShellRunner(args.quiet, args.report)
 
     runner.run_shell_script(
         args.update_mode,
         add_prefixes(args.args) if args.args else "NOARGS",
         args.config_update_mode,
         args.daemon_restart,
         args.clean,
```

### Comparing `gentoo-update-0.1.6/gentoo_update/scripts/updater.sh` & `gentoo-update-0.1.7/gentoo_update/scripts/updater.sh`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 #!/bin/bash
 
 set -euo pipefail
 
 # ---------------------- VARIABLES ----------------------- #
-UPDATE_MODE="${1}"
-UPDATE_FLAGS="${2}"
+FUNCTION="${1}"
+UPDATE_MODE="${2}"
+UPDATE_FLAGS="${3}"
 if [[ "${UPDATE_FLAGS}" == "NOARGS" ]]; then
     UPDATE_FLAGS=""
 fi
-CONFIG_UPDATE_MODE="${3}"
-DAEMON_RESTART="${4}"
-CLEAN="${5}"
-READ_ELOGS="${6}"
-READ_NEWS="${7}"
+CONFIG_UPDATE_MODE="${4}"
+DAEMON_RESTART="${5}"
+CLEAN="${6}"
+READ_ELOGS="${7}"
+READ_NEWS="${8}"
 
 # ------------------ SYNC_PORTAGE_TREE ------------------- #
 function sync_tree() {
+    echo -e "{{ SYNC PORTAGE TREE }}\n"
+
     # Update main Portage tree
     echo "Syncing Portage Tree"
     emerge --sync
 }
 
 # -------------------- UPDATE_SYSTEM --------------------- #
 function update_security() {
+    echo -e "{{ UPDATE SYSTEM }}\n"
+
     # Check for GLSAs and install updates if necessary
     glsa=$(glsa-check --list affected)
 
     if [ -z "${glsa}" ]; then
         echo "No affected GLSAs found."
     else
         echo "Affected GLSAs found. Applying updates..."
@@ -39,69 +44,84 @@
     # run emerge with custom flags
     local update_flags="${1}"
     echo "Update command:"
     echo "emerge --verbose --quiet-build=y --update --newuse --deep ${update_flags} @world"
     eval "emerge --verbose --quiet-build=y --update --newuse --deep ${update_flags} @world"
 }
 
-function update_full() {
-    update_flags="${UPDATE_FLAGS}"
+function emerge_pretend() {
+    echo -e "{{ PRETEND EMERGE }}"
 
-    # Do a full system update
-    echo "Running Update: Check Pretend First"
-    if emerge --pretend --update --newuse --deep @world; then
-        echo "emerge pretend was successful, updating..."
-        emerge_full "${update_flags}"
+    # run emerge in pretend mode to detect some issues before updating
+    update_mode="${UPDATE_MODE}"
+
+    if [[ "${update_mode}" == 'full' ]]; then
+        echo "Running emerge with --pretend"
+        if emerge --pretend --update --newuse --deep @world; then
+            echo "emerge pretend was successful, updating..."
+        else
+            echo "emerge pretend has failed, exiting"
+            exit 1
+        fi
     else
-        echo "emerge pretend has failed, not updating"
+        echo "Security update dont have pretend mode, skipping..."
     fi
 }
 
 function update() {
+    echo -e "{{ UPDATE SYSTEM }}\n"
+
     update_mode="${UPDATE_MODE}"
+    update_flags="${UPDATE_FLAGS}"
+
     # Do security updates or full system updates
     if [[ "${update_mode}" == 'security' ]]; then
-        echo -e "installing security updates only\n"
+        echo -e "updating GLSA\n"
         update_security
         echo ""
+        echo "update was successful"
+        echo ""
 
     elif [[ "${update_mode}" == 'full' ]]; then
         echo -e "updating @world\n"
-        update_full
+        emerge_full "${update_flags}"
+        echo ""
+        echo "update was successful"
         echo ""
 
     else
         echo "Invalid update mode, exiting...."
         exit 1
     fi
 }
 
 # ---------------- UPDATE_CONFIGURATIONS ----------------- #
 function config_update() {
+    echo -e "\n{{ UPDATE SYSTEM CONFIGURATION FILES }}\n"
+
     update_mode="${CONFIG_UPDATE_MODE}"
 
     # Perform the update based on the update mode
     if [[ "${update_mode}" == "merge" ]]; then
         etc-update --automode -5
-    elif [[ "${update_mode}" == "interactive" ]]; then
-        etc-update
-    elif [[ "${update_mode}" == "dispatch" ]]; then
-        dispatch-conf
     elif [[ "${update_mode}" == "ignore" ]]; then
         echo "Ignoring configuration update for now..."
         echo "Please UPDATE IT MANUALLY LATER"
     else
         echo "Invalid update mode: ${update_mode}" >&2
-        echo "Please set UPDATE_MODE to 'merge', 'interactive', 'dispatch' or 'ignore'." >&2
+        echo "Please set UPDATE_MODE to 'merge' or 'ignore'." >&2
     fi
 }
 
 # ----------------------- CLEAN_UP ----------------------- #
 function clean_up() {
+    echo -e "\n{{ CLEAN UP }}\n"
+
     clean="${CLEAN}"
+
     if [[ "${clean}" == 'y' ]]; then
         echo "Cleaning packages that are not part of the tree..."
         emerge --depclean
 
         if command -v revdep-rebuild >/dev/null 2>&1; then
             echo "Checking reverse dependencies..."
             revdep-rebuild
@@ -115,14 +135,16 @@
     else
         echo "Clean up is not enabled."
     fi
 }
 
 # -------------------- CHECK_RESTART --------------------- #
 function check_restart() {
+    echo -e "\n{{ RESTART SERVICES }}\n"
+
     restart="${DAEMON_RESTART}"
 
     if command -v needrestart >/dev/null 2>&1; then
         echo "Checking is any service needs a restart"
         if [[ "${restart}" == 'y' ]]; then
             # automatically restart all services
             needrestart -r a
@@ -160,54 +182,68 @@
                 echo ">>> Log end <<<"
                 echo ""
             fi
         done
 }
 
 function get_logs() {
+    echo -e "\n{{ READ ELOGS }}\n"
+
     read_elogs="${READ_ELOGS}"
+
     if [[ "${read_elogs}" == 'y' ]]; then
         echo "reading elogs"
         read_elogs
     else
         echo "not reading elogs"
     fi
 }
 
 # ----------------------- GET_NEWS ----------------------- #
 function get_news() {
+    echo -e "\n{{ READ NEWS }}\n"
+
     read_news="${READ_NEWS}"
+
     if [[ "${read_news}" == 'y' ]]; then
         echo "Getting important news"
         eselect news read new
     else
         echo "not reading news"
     fi
 }
 
 # --------------------- RUN_PROGRAM ---------------------- #
-echo -e "{{ SYNC PORTAGE TREE }}\n"
-sync_tree
-
-echo -e "{{ UPDATE SYSTEM }}\n"
-update
-echo ""
-
-echo -e "\n{{ UPDATE SYSTEM CONFIGURATION FILES }}\n"
-config_update
-echo ""
-
-echo -e "\n{{ CLEAN UP }}\n"
-clean_up
-echo ""
-
-echo -e "\n{{ RESTART SERVICES }}\n"
-check_restart
-echo ""
-
-echo -e "\n{{ READ ELOGS }}\n"
-get_logs
-echo ""
-
-echo -e "\n{{ READ NEWS }}\n"
-get_news
-echo -e "\n"
+case ${FUNCTION} in
+sync_tree)
+    "$@"
+    exit
+    ;;
+emerge_pretend)
+    "$@"
+    exit
+    ;;
+update)
+    "$@"
+    exit
+    ;;
+config_update)
+    "$@"
+    exit
+    ;;
+clean_up)
+    "$@"
+    exit
+    ;;
+check_restart)
+    "$@"
+    exit
+    ;;
+get_logs)
+    "$@"
+    exit
+    ;;
+get_news)
+    "$@"
+    exit
+    ;;
+esac
```

### Comparing `gentoo-update-0.1.6/gentoo_update/shell_runner.py` & `gentoo-update-0.1.7/gentoo_update/shell_runner.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 import os
 import sys
 import logging
 import subprocess
+import pprint
 from configparser import ConfigParser
 from datetime import datetime
 from typing import Tuple, List
+from .parser import Parser
 
 
 class ShellRunner:
-    def __init__(self, quiet: str) -> None:
+    def __init__(self, quiet: str, report: str) -> None:
         self.quiet = True if quiet == "y" else False
 
         self.timestamp = datetime.now().strftime("%Y-%m-%d-%H-%M")
         self.make_conf = self.make_conf_reader()
         self.log_dir, self.log_dir_messages = self.initiate_log_directory()
+
+        self.report = True if report == "y" else False
+        if self.report:
+            self.show_last_report()
+
         self.log_filename = f"{self.log_dir}/log_{self.timestamp}"
         self.logger = self.initiate_logger()
 
         self.script_dir = os.path.join(os.path.dirname(__file__), "scripts")
         self.script_path = os.path.join(self.script_dir, "updater.sh")
 
     def make_conf_reader(self) -> ConfigParser:
@@ -59,14 +66,25 @@
 
         if not os.path.exists(log_dir):
             os.mkdir(log_dir)
             log_dir_messages.append(f"Created log directory: {log_dir}")
 
         return log_dir, log_dir_messages
 
+    def show_last_report(self):
+        """
+        Show report for the last log located in $PORTAGE_LOGDIR.
+        """
+        files = os.listdir(self.log_dir)
+        paths = [os.path.join(self.log_dir, basename) for basename in files]
+        last_log = max(paths, key=os.path.getctime)
+        report = Parser(last_log).extract_info_for_report()
+        pprint.pprint(report)
+        sys.exit(0)
+
     def initiate_logger(self) -> logging.Logger:
         """
         Create a logger with two handlers:
             1. terminal output
             2. file output
         Both handlers have the same logging level (INFO)
         and share the same formatter.
@@ -145,45 +163,68 @@
             stderr_output_message = "n".join(self.stderr_output)
             error_message += (
                 f"\nStandard error output:\n{stderr_output_message}"
             )
         self.logger.error(error_message)
         sys.exit(stream.returncode)
 
-    def run_shell_script(self, *args: str) -> None:
+    def run_shell_function(self, command: List) -> None:
         """
         Run a shell script and stream standard output
         and standard error to terminal and a log file.
 
         Args:
-            script_path (str): Shell script path.
-            *args (str): Arguments for the shell script.
-                         They need to be handled by the script.
+            command (List(str)): A call to specific function in
+                                 update.sh with all parameters.
         """
-        command = [self.script_path] + list(args)
         with subprocess.Popen(
             command, stdout=subprocess.PIPE, stderr=subprocess.PIPE
         ) as script_stream:
             self.stdout_output = self._log_stream_output(
                 script_stream, "stdout"
             )
             self.stderr_output = self._log_stream_output(
                 script_stream, "stderr"
             )
             script_stream.wait()
 
             if script_stream.returncode != 0:
                 self._exit_with_error_message(script_stream)
 
+    def run_shell_script(self, *args: str) -> None:
+        """
+        Run every function in update.sh one by one.
+
+        Args:
+            *args (str): Arguments for the shell script.
+                         They need to be handled by the script.
+        """
+        script_stages = [
+            "sync_tree",
+            "emerge_pretend",
+            "update",
+            "config_update",
+            "clean_up",
+            "check_restart",
+            "get_logs",
+            "get_news",
+        ]
+        for stage in script_stages:
+            command = [self.script_path] + [stage] + list(args)
+            self.run_shell_function(command)
+
         final_message = f"gentoo-update is done! Log:file: {self.log_filename}"
         self.logger.info(final_message)
         if self.quiet:
             print(final_message)
 
     def __del__(self) -> None:
         """
         Closed all file handlers after ShellRunner is closed.
         """
-        if self.logger:
-            for handler in self.logger.handlers:
-                handler.close()
-                self.logger.removeHandler(handler)
+        try:
+            if self.logger:
+                for handler in self.logger.handlers:
+                    handler.close()
+                    self.logger.removeHandler(handler)
+        except AttributeError:
+            pass
```

### Comparing `gentoo-update-0.1.6/gentoo_update.egg-info/PKG-INFO` & `gentoo-update-0.1.7/gentoo_update.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gentoo-update
-Version: 0.1.6
+Version: 0.1.7
 Summary: Gentoo Linux updater
 Home-page: https://github.com/Lab-Brat/gentoo_update
 Author: Lab-Brat
 Author-email: labbrat_social@pm.me
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
@@ -17,27 +17,31 @@
 
 `gentoo-update` is a tool that automates updates on Gentoo Linux. 
 By default it only installs security updates from [GLSA](https://security.gentoo.org/glsa/), 
 but it can also be used to update all packages on the system. i.e. `@world`.  
 
 This project 
 [originates](https://wiki.gentoo.org/wiki/Google_Summer_of_Code/2023/Ideas/Automated_Gentoo_system_updater) 
-from 2023 Google Summer of Code.
+from 2023 Google Summer of Code, more about it can be found in the 
+[blog post](https://labbrat.net/blog/gsoc2023/gentoo_update_intro/) and 
+[Gentoo Forums](https://forums.gentoo.org/viewtopic-p-8793827.html#8793827).  
 
 
 #### Usage
 `gentoo-update` is in [GURU](https://wiki.gentoo.org/wiki/Project:GURU) 
 overlay, and can be installed using `emerge`:
 ```bash
 emerge --ask app-admin/gentoo_update
 ```
 
-Alternatively, updater can be installed with pip:
-```
-pip install gentoo_update --break-system-packages
+Alternatively, it can be installed with pip in a virtual environment:
+```bash
+python -m venv gentoo_update
+source gentoo_update/bin/activate
+python -m pip install gentoo_update
 ```
 
 The updater creates a subdirectory in Portage's default `PORTAGE_LOGDIR` located at `/var/log/portage/gentoo-update`. 
 However, if this variable is set to a different value in `make.conf`, it will use the new location instead of the default.  
 
 Here are some usage examples:
 * Basic security update
```

### Comparing `gentoo-update-0.1.6/setup.cfg` & `gentoo-update-0.1.7/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -10,17 +10,21 @@
 classifiers = 
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3.10
 	Operating System :: POSIX :: Linux
 
 [options]
 python_requires = >=3.10
-packages = find_namespace:
 include_package_data = True
 
+[options.packages.find]
+exclude = 
+	tests
+	tests.*
+
 [options.entry_points]
 console_scripts = 
 	gentoo-update = gentoo_update.gentoo_update:main
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `gentoo-update-0.1.6/tests/test_updater.py` & `gentoo-update-0.1.7/tests/test_updater.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from unittest.mock import patch, Mock, MagicMock
 import gentoo_update
 from gentoo_update import create_cli, add_prefixes
 
 
 class TestGentooUpdate(unittest.TestCase):
     def test_add_prefixes(self):
-        input_args = ["a", "bc"]
-        expected_output = ["-a", "--bc"]
+        input_args = "a bc"
+        expected_output = "-a --bc"
         self.assertEqual(add_prefixes(input_args), expected_output)
 
     @patch("argparse.ArgumentParser.parse_args")
     def test_create_cli(self, mock_parse_args):
         mock_args = Mock()
         mock_parse_args.return_value = mock_args
         args = create_cli()
```

