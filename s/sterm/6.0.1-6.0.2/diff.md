# Comparing `tmp/sterm-6.0.1.tar.gz` & `tmp/sterm-6.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sterm-6.0.1.tar", last modified: Sat Mar  7 08:15:54 2020, max compression
+gzip compressed data, was "sterm-6.0.2.tar", last modified: Sun Jul  2 11:02:46 2023, max compression
```

## Comparing `sterm-6.0.1.tar` & `sterm-6.0.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 redeagle  (1000) redeagle  (1000)        0 2020-03-07 08:15:54.813616 sterm-6.0.1/
--rw-r--r--   0 redeagle  (1000) redeagle  (1000)       16 2020-01-17 12:55:33.000000 sterm-6.0.1/MANIFEST.in
--rw-r--r--   0 redeagle  (1000) redeagle  (1000)     8081 2020-03-07 08:15:54.813616 sterm-6.0.1/PKG-INFO
--rw-r--r--   0 redeagle  (1000) redeagle  (1000)     4896 2020-03-07 08:06:32.000000 sterm-6.0.1/README.md
--rw-r--r--   0 redeagle  (1000) redeagle  (1000)       38 2020-03-07 08:15:54.813616 sterm-6.0.1/setup.cfg
--rw-r--r--   0 redeagle  (1000) redeagle  (1000)     2668 2020-03-07 08:10:20.000000 sterm-6.0.1/setup.py
-drwxr-xr-x   0 redeagle  (1000) redeagle  (1000)        0 2020-03-07 08:15:54.810283 sterm-6.0.1/sterm/
--rw-r--r--   0 redeagle  (1000) redeagle  (1000)       49 2020-01-17 12:55:33.000000 sterm-6.0.1/sterm/__init__.py
--rw-r--r--   0 redeagle  (1000) redeagle  (1000)     8221 2020-03-07 08:14:18.000000 sterm-6.0.1/sterm/cli.py
--rw-r--r--   0 redeagle  (1000) redeagle  (1000)     5695 2020-01-17 12:55:33.000000 sterm-6.0.1/sterm/terminal.py
--rw-r--r--   0 redeagle  (1000) redeagle  (1000)     8487 2020-01-17 12:55:33.000000 sterm-6.0.1/sterm/uart.py
--rw-r--r--   0 redeagle  (1000) redeagle  (1000)     3511 2020-03-07 08:14:00.000000 sterm-6.0.1/sterm.1
-drwxr-xr-x   0 redeagle  (1000) redeagle  (1000)        0 2020-03-07 08:15:54.813616 sterm-6.0.1/sterm.egg-info/
--rw-r--r--   0 redeagle  (1000) redeagle  (1000)     8081 2020-03-07 08:15:54.000000 sterm-6.0.1/sterm.egg-info/PKG-INFO
--rw-r--r--   0 redeagle  (1000) redeagle  (1000)      277 2020-03-07 08:15:54.000000 sterm-6.0.1/sterm.egg-info/SOURCES.txt
--rw-r--r--   0 redeagle  (1000) redeagle  (1000)        1 2020-03-07 08:15:54.000000 sterm-6.0.1/sterm.egg-info/dependency_links.txt
--rw-r--r--   0 redeagle  (1000) redeagle  (1000)       42 2020-03-07 08:15:54.000000 sterm-6.0.1/sterm.egg-info/entry_points.txt
--rw-r--r--   0 redeagle  (1000) redeagle  (1000)        9 2020-03-07 08:15:54.000000 sterm-6.0.1/sterm.egg-info/requires.txt
--rw-r--r--   0 redeagle  (1000) redeagle  (1000)        6 2020-03-07 08:15:54.000000 sterm-6.0.1/sterm.egg-info/top_level.txt
+drwxr-xr-x   0 ralf      (1000) ralf      (1000)        0 2023-07-02 11:02:46.691745 sterm-6.0.2/
+-rw-r--r--   0 ralf      (1000) ralf      (1000)    35141 2023-07-02 10:57:03.000000 sterm-6.0.2/LICENSE
+-rw-r--r--   0 ralf      (1000) ralf      (1000)       16 2023-07-02 10:57:03.000000 sterm-6.0.2/MANIFEST.in
+-rw-r--r--   0 ralf      (1000) ralf      (1000)     8838 2023-07-02 11:02:46.691745 sterm-6.0.2/PKG-INFO
+-rw-r--r--   0 ralf      (1000) ralf      (1000)     6985 2023-07-02 10:57:03.000000 sterm-6.0.2/README.md
+-rw-r--r--   0 ralf      (1000) ralf      (1000)       38 2023-07-02 11:02:46.691745 sterm-6.0.2/setup.cfg
+-rw-r--r--   0 ralf      (1000) ralf      (1000)     2775 2023-07-02 10:59:37.000000 sterm-6.0.2/setup.py
+drwxr-xr-x   0 ralf      (1000) ralf      (1000)        0 2023-07-02 11:02:46.691745 sterm-6.0.2/sterm/
+-rw-r--r--   0 ralf      (1000) ralf      (1000)       49 2023-07-02 10:57:03.000000 sterm-6.0.2/sterm/__init__.py
+-rw-r--r--   0 ralf      (1000) ralf      (1000)     8221 2023-07-02 10:58:41.000000 sterm-6.0.2/sterm/cli.py
+-rw-r--r--   0 ralf      (1000) ralf      (1000)     5695 2023-07-02 10:57:03.000000 sterm-6.0.2/sterm/terminal.py
+-rw-r--r--   0 ralf      (1000) ralf      (1000)     8505 2023-07-02 10:57:03.000000 sterm-6.0.2/sterm/uart.py
+-rw-r--r--   0 ralf      (1000) ralf      (1000)     3510 2023-07-02 10:57:53.000000 sterm-6.0.2/sterm.1
+drwxr-xr-x   0 ralf      (1000) ralf      (1000)        0 2023-07-02 11:02:46.691745 sterm-6.0.2/sterm.egg-info/
+-rw-r--r--   0 ralf      (1000) ralf      (1000)     8838 2023-07-02 11:02:46.000000 sterm-6.0.2/sterm.egg-info/PKG-INFO
+-rw-r--r--   0 ralf      (1000) ralf      (1000)      285 2023-07-02 11:02:46.000000 sterm-6.0.2/sterm.egg-info/SOURCES.txt
+-rw-r--r--   0 ralf      (1000) ralf      (1000)        1 2023-07-02 11:02:46.000000 sterm-6.0.2/sterm.egg-info/dependency_links.txt
+-rw-r--r--   0 ralf      (1000) ralf      (1000)       41 2023-07-02 11:02:46.000000 sterm-6.0.2/sterm.egg-info/entry_points.txt
+-rw-r--r--   0 ralf      (1000) ralf      (1000)        9 2023-07-02 11:02:46.000000 sterm-6.0.2/sterm.egg-info/requires.txt
+-rw-r--r--   0 ralf      (1000) ralf      (1000)        6 2023-07-02 11:02:46.000000 sterm-6.0.2/sterm.egg-info/top_level.txt
```

### Comparing `sterm-6.0.1/PKG-INFO` & `sterm-6.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,205 +1,27 @@
 Metadata-Version: 2.1
 Name: sterm
-Version: 6.0.1
+Version: 6.0.2
 Summary: A minimal serial / UART command line terminal that focus on being easy to use.
 Home-page: https://github.com/rstemmer/sterm
 Author: Ralf Stemmer
 Author-email: ralf.stemmer@gmx.net
 License: GPL
 Project-URL: Documentation, https://github.com/rstemmer/sterm
 Project-URL: Source, https://github.com/rstemmer/sterm
 Project-URL: Tracker, https://github.com/rstemmer/sterm/issues
-Description: <h3 align="center">sterm</h3>
-        
-        <div align="center">
-          Status: Active - License: GPL v3
-        </div>
-        
-        ---
-        
-        <p align="center"> sterm is a minimal serial terminal that focus on being easy to use. - This client just does its job.
-            <br/>
-        </p>
-        
-        
-        ## 📝 Table of Contents
-        - [About](#about)
-        - [Getting Started](#getting_started)
-        - [Usage](#usage)
-        - [Built Using](#built_using)
-        - [Acknowledgments](#acknowledgement)
-        
-        
-        ## 🧐 About <a name = "about"></a>
-        
-        **sterm** is a minimal serial terminal that focus on being easy to use and not sucking. - This client simply works.
-        It has inline input and supports Unicode (utf-8).
-        Each character typed gets directly send to the connected device without buffering.
-        It writes whatever it receives to *stdout* so that also Unicode and ANSI escape sequences work as expected.
-        
-        ### Core Use-Cases
-        
-        *Ideal for debugging:*<br/>
-        With the ``--binary`` option, the received data will be output byte wise as hexadecimal numbers.
-        
-        *Ideal for a remote Linux shell:*<br/>
-        With the ``--noecho`` option, each character typed gets directly send to the connected device without buffering and echoing.
-        This makes the Linux console usage seamlessly like using telnet or ssh.
-        
-        ### Core Features
-        
-        - Inline input
-        - No line buffering
-        - Unicode support
-        - ANSI Escape Sequences supported
-        - No GUI
-        
-        
-        ## 🏁 Getting Started <a name = "getting_started"></a>
-        
-        There are two ways to install _sterm_.
-        Directly using `pip` or from the cloned repository.
-        
-        ### Installation using pip
-        
-        ```bash
-        pip install sterm
-        ```
-        
-        ### Installation from Repository
-        
-        ```bash
-        # Download
-        git clone https://github.com/rstemmer/sterm.git
-        cd sterm
-        
-        # Dependencies
-        pip install pyserial
-        
-        # Install Package
-        pip install .
-        
-        ```
-        
-        
-        ## 🎈 Usage <a name="usage"></a>
-        
-        *sterm* has three interfaces:
-        
-        1. Configuration files
-        2. The command line interface
-        3. Escape commands
-        
-        ### Configuration via files
-        
-        TODO - Not yet implemented.
-        
-        ### Command Line Arguments
-        
-        ```bash
-        sterm [-h] [--noecho] [--escape character] [--binary] [-b BAUDRATE] [-f FORMAT] [-w logfile] DEVICE
-        ```
-        
-        When a command line argument is contradictory to a setting in the configuration files, the command line argument has higher priority.
-        
-          * __-h__: Print help.
-          * __-n__: Enable _noecho_ mode. _Default_ is echoing each entered key to _stdout_.
-          * __--escape__: Define an alternative escape character. _Default_ is escape ("\e").
-          * __--binary__: Print hexadecimal values instead of Unicode characters. (Only applied on output, input will still be UTF-8)
-          * __-b__: Baudrate. _Default:_ 115200 baud.
-          * __-f__: Configuration-triple: xyz with x = bytelength in bits {5,6,7,8}; y = parity {N,E,O}; z = stopbits {1,2}. _Default:_ "8N1" - _8_ data bits, _no_ parity bits and _1_ stop bit.
-          * __-w__: Write received data into a file.
-        
-        _DEVICE_ is the path to the serial terminal.
-        For example _/dev/ttyS0_, _/dev/ttyUSB0_, _/dev/ttyUART0_, _/dev/ttyACM0_, _/dev/pts/42_.
-        
-        For details read the man-page.
-        
-        ### Escape commands
-        
-        The following strings can be entered while _sterm_ is running.
-        Just hit the escape-key and then enter the commands.
-        They get not send to the device.
-        Instead they are interpreted by _sterm_.
-        The preceded escape character can be defined with --escape.
-        Default is the escape key ("\e").
-        
-          * __exit__: quit sterm
-          * __version__: print version
-        
-        ### Examples
-        
-        Send _ping_ to UART0 and exit:
-        ```
-        sterm /dev/ttyUART0
-        ping
-        pong
-        ^[exit
-        ```
-        
-        Send _hello_ to a serial device with 9600 baud, 7 data bits, even parity, and 2 stop bits. Then exit:
-        ```
-        sterm -b 9600 -f 7E2 /dev/ttyS0
-        hello
-        world
-        ^[exit
-        ```
-        
-        Connecting to a Linux device
-        ```
-        sterm --noecho --escape _ /dev/ttyUSB0
-        ~# whoami
-        root
-        ~# _exit
-        ```
-        
-        Communicating with two _sterm_ instances via a pseudo terminal for testing:
-        ![A picture that demonstrates the possibility of receiving ANSI escape sequences and unicode charaters](/stermscreenshot.png?raw=true "Testrun showing some capabilities of sterm")
-        
-        
-        ## ⛏️ Building and Testing <a name = "built_using"></a>
-        
-        ### Testing
-        
-        To test _sterm_ from the sources, just call the `test.py` script.
-        It runs the command line interface of _sterm_.
-        
-        You can use `socat` to create a virtual serial connection with two endings, so that you can use two `sterm` processes to communicate with each other:
-        
-        ```bash
-        socat -d -d pty,raw,echo=0 pty,raw,echo=0
-        ```
-        
-        ### Building a new Package
-        
-        To build a new package from the source code, just execute the `pkg-make.sh` script.
-        Make sure to update the version number in the `sterm/cli.py` file.
-        This version number, as well as the README.md file gets read by the setup.py file.
-        
-        ```bash
-        vim sterm/cli.py
-        ./pkg-make.sh
-        ```
-        
-        
-        ## 🎉 Acknowledgements <a name = "acknowledgement"></a>
-        
-        - [@kylelobo](https://github.com/kylelobo) for [this README template](https://github.com/kylelobo/The-Documentation-Compendium)
-        - [The pyserial project](https://github.com/pyserial/pyserial) that is the base of _sterm_
-        
-        
 Keywords: serial-communication serial-terminal terminal uart rs232 monitoring tty pyserial serial
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
@@ -212,7 +34,239 @@
 Classifier: Topic :: Software Development :: Debuggers
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Logging
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: Utilities
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<h3 align="center">sterm</h3>
+
+<div align="center">
+  Status: 🟢 Active - License: GPL v3
+</div>
+
+---
+
+<p align="center"> sterm is a minimal serial terminal that focus on being easy to use. - This client just does its job.
+    <br/>
+</p>
+
+```bash
+pip install sterm
+sterm --help
+sterm /dev/ttyUSB0
+```
+
+
+## 📝 Table of Contents
+- [About](#about)
+- [Getting Started](#getting_started)
+- [Usage](#usage)
+- [Built Using](#built_using)
+- [Related Work](#related_work)
+- [Acknowledgments](#acknowledgement)
+
+
+## 🧐 About <a name = "about"></a>
+
+**sterm** is a minimal serial terminal that focus on being easy to use and not sucking. - This client simply works.
+It has inline input and supports Unicode (utf-8).
+Each character typed gets directly send to the connected device without buffering.
+It writes whatever it receives to *stdout* so that also Unicode and ANSI escape sequences work as expected.
+
+### Core Use-Cases
+
+*Ideal for debugging:*<br/>
+With the ``--binary`` option, the received data will be output byte wise as hexadecimal numbers.
+
+*Ideal for a remote Linux shell:*<br/>
+With the ``--noecho`` option, each character typed gets directly send to the connected device without buffering and echoing.
+This makes the Linux console usage seamlessly like using telnet or ssh.
+
+### Core Features
+
+- Inline input
+- No line buffering
+- Unicode support
+- ANSI Escape Sequences supported
+- No GUI
+
+
+## 🏁 Getting Started <a name = "getting_started"></a>
+
+There are two ways to install _sterm_.
+**A:** Directly using `pip` or **B:** from the cloned repository.
+
+### Precondition
+
+_sterm_ requires Python 3 to run.
+Before you start installing _sterm_ make sure you use the correct version.
+Depending on your distribution, the you may need to use `pip3` instead of `pip`.
+You can check your Python version by executing the following commands:
+
+```bash
+python --version
+pip --version
+```
+
+Both should print a version number beginning with 3.
+If not, you need to use `pip3` to explicit use Python 3.
+
+For a user-only installation, call `pip ...` as user.
+For a system-wide installation you need to be root, or call `sudo pip ...`.
+
+### A: Installation using pip
+
+```bash
+pip install sterm
+```
+
+### B: Installation from Repository
+
+```bash
+# Download
+git clone https://github.com/rstemmer/sterm.git
+cd sterm
+
+# Dependencies
+pip install pyserial
+
+# Install Package
+pip install .
+
+```
+
+### Check installation
+
+After installation you can check if _sterm_ is successfully installed using `whereis`.
+```bash
+whereis sterm
+#Outpu: sterm: /usr/bin/sterm /usr/man/man1/sterm.1
+```
+There should be two files listed.
+ - `sterm` is the executable, the command you run.
+ - `sterm.1` is the manual for `sterm` that can be read by executing `man sterm` on the command line.
+
+On a system-wide installation, _sterm_ is usually installed to /usr/bin.
+If you only installed to for a single user, it is usually installed to ~/.local/bin
+
+During the installation process, `pip` should install all dependencies recursively.
+To be sure nothing is missing, you can run `pip check sterm`.
+It prints all missing dependencies or version conflicts.
+You can install missing dependencies via `pip`.
+When version conflicts are listed, you can hope they do not matter or install an explicit version via `pip` as well.
+
+
+## 🎈 Usage <a name="usage"></a>
+
+To execute _sterm_ you just have to call the `sterm` command in your shell.
+`sterm` requires one argument, the device you want to access.
+All other arguments listed in the subsection below are optional.
+
+UART-Devices are listed in the /dev directory with the prefix `tty`.
+Most UART-Devices are addressable via /dev/ttyUSBx or /dev/ttyACMx were x is a number depending on the order they got recognized by the Linux kernel.
+
+
+*sterm* has two interfaces:
+
+1. The command line interface
+2. Escape commands
+
+
+### Command Line Arguments
+
+```bash
+sterm [-h] [--noecho] [--escape character] [--binary] [-b BAUDRATE] [-f FORMAT] [-w logfile] DEVICE
+```
+
+When a command line argument is contradictory to a setting in the configuration files, the command line argument has higher priority.
+
+  * __-h__: Print help.
+  * __-n__: Enable _noecho_ mode. _Default_ is echoing each entered key to _stdout_.
+  * __--escape__: Define an alternative escape character. _Default_ is escape ("\e").
+  * __--binary__: Print hexadecimal values instead of Unicode characters. (Only applied on output, input will still be UTF-8)
+  * __-b__: Baudrate. _Default:_ 115200 baud.
+  * __-f__: Configuration-triple: xyz with x = bytelength in bits {5,6,7,8}; y = parity {N,E,O}; z = stopbits {1,2}. _Default:_ "8N1" - _8_ data bits, _no_ parity bits and _1_ stop bit.
+  * __-w__: Write received data into a file.
+
+_DEVICE_ is the path to the serial terminal.
+For example _/dev/ttyS0_, _/dev/ttyUSB0_, _/dev/ttyUART0_, _/dev/ttyACM0_, _/dev/pts/42_.
+
+For details read the man-page.
+
+### Escape commands
+
+The following strings can be entered while _sterm_ is running.
+Just hit the escape-key and then enter the commands.
+They get not send to the device.
+Instead they are interpreted by _sterm_.
+The preceded escape character can be defined with --escape.
+Default is the escape key ("\e").
+
+  * __exit__: quit sterm
+  * __version__: print version
+
+### Examples
+
+Send _ping_ to UART0 and exit:
+```
+sterm /dev/ttyUART0
+ping
+pong
+^[exit
+```
+
+Send _hello_ to a serial device with 9600 baud, 7 data bits, even parity, and 2 stop bits. Then exit:
+```
+sterm -b 9600 -f 7E2 /dev/ttyS0
+hello
+world
+^[exit
+```
+
+Connecting to a Linux device
+```
+sterm --noecho --escape _ /dev/ttyUSB0
+~# whoami
+root
+~# _exit
+```
+
+Communicating with two _sterm_ instances via a pseudo terminal for testing:
+![A picture that demonstrates the possibility of receiving ANSI escape sequences and unicode charaters](/stermscreenshot.png?raw=true "Testrun showing some capabilities of sterm")
+
+
+## ⛏️ Building and Testing <a name = "built_using"></a>
+
+### Testing
+
+To test _sterm_ from the sources, just call the `test.py` script.
+It runs the command line interface of _sterm_.
+
+You can use `socat` to create a virtual serial connection with two endings, so that you can use two `sterm` processes to communicate with each other:
+
+```bash
+socat -d -d pty,raw,echo=0 pty,raw,echo=0
+```
+
+### Building a new Package
+
+To build a new package from the source code, just execute the `pkg-make.sh` script.
+Make sure to update the version number in the `sterm/cli.py` file.
+This version number, as well as the README.md file gets read by the setup.py file.
+
+```bash
+vim sterm/cli.py
+./pkg-make.sh
+```
+
+## ⛓ Related Work <a name ="related_work"></a>
+
+ - [tio](https://github.com/tio/tio) A more feature rich alternative to `sterm` with a similar motivation
+
+## 🎉 Acknowledgements <a name = "acknowledgement"></a>
+
+- [@kylelobo](https://github.com/kylelobo) for [this README template](https://github.com/kylelobo/The-Documentation-Compendium)
+- [The pyserial project](https://github.com/pyserial/pyserial) that is the base of _sterm_
+
```

### Comparing `sterm-6.0.1/README.md` & `sterm-6.0.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 <h3 align="center">sterm</h3>
 
 <div align="center">
-  Status: Active - License: GPL v3
+  Status: 🟢 Active - License: GPL v3
 </div>
 
 ---
 
 <p align="center"> sterm is a minimal serial terminal that focus on being easy to use. - This client just does its job.
     <br/>
 </p>
 
+```bash
+pip install sterm
+sterm --help
+sterm /dev/ttyUSB0
+```
+
 
 ## 📝 Table of Contents
 - [About](#about)
 - [Getting Started](#getting_started)
 - [Usage](#usage)
 - [Built Using](#built_using)
+- [Related Work](#related_work)
 - [Acknowledgments](#acknowledgement)
 
 
 ## 🧐 About <a name = "about"></a>
 
 **sterm** is a minimal serial terminal that focus on being easy to use and not sucking. - This client simply works.
 It has inline input and supports Unicode (utf-8).
@@ -43,49 +50,91 @@
 - ANSI Escape Sequences supported
 - No GUI
 
 
 ## 🏁 Getting Started <a name = "getting_started"></a>
 
 There are two ways to install _sterm_.
-Directly using `pip` or from the cloned repository.
+**A:** Directly using `pip` or **B:** from the cloned repository.
+
+### Precondition
+
+_sterm_ requires Python 3 to run.
+Before you start installing _sterm_ make sure you use the correct version.
+Depending on your distribution, the you may need to use `pip3` instead of `pip`.
+You can check your Python version by executing the following commands:
+
+```bash
+python --version
+pip --version
+```
 
-### Installation using pip
+Both should print a version number beginning with 3.
+If not, you need to use `pip3` to explicit use Python 3.
+
+For a user-only installation, call `pip ...` as user.
+For a system-wide installation you need to be root, or call `sudo pip ...`.
+
+### A: Installation using pip
 
 ```bash
 pip install sterm
 ```
 
-### Installation from Repository
+### B: Installation from Repository
 
 ```bash
 # Download
 git clone https://github.com/rstemmer/sterm.git
 cd sterm
 
 # Dependencies
 pip install pyserial
 
 # Install Package
 pip install .
 
 ```
 
+### Check installation
+
+After installation you can check if _sterm_ is successfully installed using `whereis`.
+```bash
+whereis sterm
+#Outpu: sterm: /usr/bin/sterm /usr/man/man1/sterm.1
+```
+There should be two files listed.
+ - `sterm` is the executable, the command you run.
+ - `sterm.1` is the manual for `sterm` that can be read by executing `man sterm` on the command line.
+
+On a system-wide installation, _sterm_ is usually installed to /usr/bin.
+If you only installed to for a single user, it is usually installed to ~/.local/bin
+
+During the installation process, `pip` should install all dependencies recursively.
+To be sure nothing is missing, you can run `pip check sterm`.
+It prints all missing dependencies or version conflicts.
+You can install missing dependencies via `pip`.
+When version conflicts are listed, you can hope they do not matter or install an explicit version via `pip` as well.
+
 
 ## 🎈 Usage <a name="usage"></a>
 
-*sterm* has three interfaces:
+To execute _sterm_ you just have to call the `sterm` command in your shell.
+`sterm` requires one argument, the device you want to access.
+All other arguments listed in the subsection below are optional.
+
+UART-Devices are listed in the /dev directory with the prefix `tty`.
+Most UART-Devices are addressable via /dev/ttyUSBx or /dev/ttyACMx were x is a number depending on the order they got recognized by the Linux kernel.
 
-1. Configuration files
-2. The command line interface
-3. Escape commands
 
-### Configuration via files
+*sterm* has two interfaces:
+
+1. The command line interface
+2. Escape commands
 
-TODO - Not yet implemented.
 
 ### Command Line Arguments
 
 ```bash
 sterm [-h] [--noecho] [--escape character] [--binary] [-b BAUDRATE] [-f FORMAT] [-w logfile] DEVICE
 ```
 
@@ -166,13 +215,16 @@
 This version number, as well as the README.md file gets read by the setup.py file.
 
 ```bash
 vim sterm/cli.py
 ./pkg-make.sh
 ```
 
+## ⛓ Related Work <a name ="related_work"></a>
+
+ - [tio](https://github.com/tio/tio) A more feature rich alternative to `sterm` with a similar motivation
 
 ## 🎉 Acknowledgements <a name = "acknowledgement"></a>
 
 - [@kylelobo](https://github.com/kylelobo) for [this README template](https://github.com/kylelobo/The-Documentation-Compendium)
 - [The pyserial project](https://github.com/pyserial/pyserial) that is the base of _sterm_
```

### Comparing `sterm-6.0.1/setup.py` & `sterm-6.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,14 +34,16 @@
         classifiers     = [
             "Programming Language :: Python :: 3",
             "Programming Language :: Python :: 3.4",
             "Programming Language :: Python :: 3.5",
             "Programming Language :: Python :: 3.6",
             "Programming Language :: Python :: 3.7",
             "Programming Language :: Python :: 3.8",
+            "Programming Language :: Python :: 3.9",
+            "Programming Language :: Python :: 3.10",
             "Development Status :: 5 - Production/Stable",
             "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
             "Operating System :: POSIX :: Linux",
             "Environment :: Console",
             "Intended Audience :: End Users/Desktop",
             "Intended Audience :: Developers",
             "Intended Audience :: System Administrators",
```

### Comparing `sterm-6.0.1/sterm/cli.py` & `sterm-6.0.2/sterm/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 # STERM, a serial communication terminal with server capabilities        #
-# Copyright (C) 2013-2020  Ralf Stemmer (ralf.stemmer@gmx.net)           #
+# Copyright (C) 2013-2023  Ralf Stemmer (ralf.stemmer@gmx.net)           #
 #                                                                        #
 # This program is free software: you can redistribute it and/or modify   #
 # it under the terms of the GNU General Public License as published by   #
 # the Free Software Foundation, either version 3 of the License, or      #
 # (at your option) any later version.                                    #
 #                                                                        #
 # This program is distributed in the hope that it will be useful,        #
@@ -24,15 +24,15 @@
 import tty
 from threading      import Thread
 from sterm.uart     import UART, UARTMode
 from sterm.terminal import Terminal
 
 
 
-VERSION = "6.0.1"
+VERSION = "6.0.2"
 
 
 # This global variable is used to shutdown the thread used
 # for the ReceiveData function.
 ShutdownReceiver = False
```

### Comparing `sterm-6.0.1/sterm/terminal.py` & `sterm-6.0.2/sterm/terminal.py`

 * *Files identical despite different names*

### Comparing `sterm-6.0.1/sterm/uart.py` & `sterm-6.0.2/sterm/uart.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,17 +194,17 @@
 
         else:
             raise ValueError("Unknown/Unsupported UARMode!")
 
 
         if self.logfile:
             if self.uartmode == UARTMode.TEXT:
-                log.write(string)
+                self.logfile.write(string)
             else:
-                log.write(data)
+                self.logfile.write(data)
 
         return string
 
 
 
     def Transmit(self, string):
         """
```

### Comparing `sterm-6.0.1/sterm.1` & `sterm-6.0.2/sterm.1`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH STERM 1 "07 March 2020" "6.0.1" "sterm Manual"
+.TH STERM 1 "02 June 2023" "6.0.2" "sterm Manual"
 .SH NAME
 sterm \- a minimal serial terminal that focus on being easy to use. A client simply works.
 
 .SH SYNOPSIS
 .B sterm
 [\fB\-h\fR | \fB\-\-help\fR] 
 [\fB\-n\fR | \fB\-\-noecho\fR]
@@ -99,15 +99,15 @@
 .SH AUTHOR
 Written by Ralf Stemmer <ralf.stemmer@gmx.net>
 
 .SH REPORTING BUGS
 GitHub: <https://github.com/rstemmer/sterm/issues>
 
 .SH COPYRIGHT
-sterm  Copyright (C) 2013-2019  Ralf Stemmer <ralf.stemmer@gmx.net>
+sterm  Copyright (C) 2013-2023  Ralf Stemmer <ralf.stemmer@gmx.net>
 .br
 License GPLv3+: GNU GPL version 3 or later <http://gnu.org/licenses/gpl.html>.
 .br
 This program comes with ABSOLUTELY NO WARRANTY
 .br
 This is free software, and you are welcome to redistribute it
 under certain conditions.
```

### Comparing `sterm-6.0.1/sterm.egg-info/PKG-INFO` & `sterm-6.0.2/sterm.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,205 +1,27 @@
 Metadata-Version: 2.1
 Name: sterm
-Version: 6.0.1
+Version: 6.0.2
 Summary: A minimal serial / UART command line terminal that focus on being easy to use.
 Home-page: https://github.com/rstemmer/sterm
 Author: Ralf Stemmer
 Author-email: ralf.stemmer@gmx.net
 License: GPL
 Project-URL: Documentation, https://github.com/rstemmer/sterm
 Project-URL: Source, https://github.com/rstemmer/sterm
 Project-URL: Tracker, https://github.com/rstemmer/sterm/issues
-Description: <h3 align="center">sterm</h3>
-        
-        <div align="center">
-          Status: Active - License: GPL v3
-        </div>
-        
-        ---
-        
-        <p align="center"> sterm is a minimal serial terminal that focus on being easy to use. - This client just does its job.
-            <br/>
-        </p>
-        
-        
-        ## 📝 Table of Contents
-        - [About](#about)
-        - [Getting Started](#getting_started)
-        - [Usage](#usage)
-        - [Built Using](#built_using)
-        - [Acknowledgments](#acknowledgement)
-        
-        
-        ## 🧐 About <a name = "about"></a>
-        
-        **sterm** is a minimal serial terminal that focus on being easy to use and not sucking. - This client simply works.
-        It has inline input and supports Unicode (utf-8).
-        Each character typed gets directly send to the connected device without buffering.
-        It writes whatever it receives to *stdout* so that also Unicode and ANSI escape sequences work as expected.
-        
-        ### Core Use-Cases
-        
-        *Ideal for debugging:*<br/>
-        With the ``--binary`` option, the received data will be output byte wise as hexadecimal numbers.
-        
-        *Ideal for a remote Linux shell:*<br/>
-        With the ``--noecho`` option, each character typed gets directly send to the connected device without buffering and echoing.
-        This makes the Linux console usage seamlessly like using telnet or ssh.
-        
-        ### Core Features
-        
-        - Inline input
-        - No line buffering
-        - Unicode support
-        - ANSI Escape Sequences supported
-        - No GUI
-        
-        
-        ## 🏁 Getting Started <a name = "getting_started"></a>
-        
-        There are two ways to install _sterm_.
-        Directly using `pip` or from the cloned repository.
-        
-        ### Installation using pip
-        
-        ```bash
-        pip install sterm
-        ```
-        
-        ### Installation from Repository
-        
-        ```bash
-        # Download
-        git clone https://github.com/rstemmer/sterm.git
-        cd sterm
-        
-        # Dependencies
-        pip install pyserial
-        
-        # Install Package
-        pip install .
-        
-        ```
-        
-        
-        ## 🎈 Usage <a name="usage"></a>
-        
-        *sterm* has three interfaces:
-        
-        1. Configuration files
-        2. The command line interface
-        3. Escape commands
-        
-        ### Configuration via files
-        
-        TODO - Not yet implemented.
-        
-        ### Command Line Arguments
-        
-        ```bash
-        sterm [-h] [--noecho] [--escape character] [--binary] [-b BAUDRATE] [-f FORMAT] [-w logfile] DEVICE
-        ```
-        
-        When a command line argument is contradictory to a setting in the configuration files, the command line argument has higher priority.
-        
-          * __-h__: Print help.
-          * __-n__: Enable _noecho_ mode. _Default_ is echoing each entered key to _stdout_.
-          * __--escape__: Define an alternative escape character. _Default_ is escape ("\e").
-          * __--binary__: Print hexadecimal values instead of Unicode characters. (Only applied on output, input will still be UTF-8)
-          * __-b__: Baudrate. _Default:_ 115200 baud.
-          * __-f__: Configuration-triple: xyz with x = bytelength in bits {5,6,7,8}; y = parity {N,E,O}; z = stopbits {1,2}. _Default:_ "8N1" - _8_ data bits, _no_ parity bits and _1_ stop bit.
-          * __-w__: Write received data into a file.
-        
-        _DEVICE_ is the path to the serial terminal.
-        For example _/dev/ttyS0_, _/dev/ttyUSB0_, _/dev/ttyUART0_, _/dev/ttyACM0_, _/dev/pts/42_.
-        
-        For details read the man-page.
-        
-        ### Escape commands
-        
-        The following strings can be entered while _sterm_ is running.
-        Just hit the escape-key and then enter the commands.
-        They get not send to the device.
-        Instead they are interpreted by _sterm_.
-        The preceded escape character can be defined with --escape.
-        Default is the escape key ("\e").
-        
-          * __exit__: quit sterm
-          * __version__: print version
-        
-        ### Examples
-        
-        Send _ping_ to UART0 and exit:
-        ```
-        sterm /dev/ttyUART0
-        ping
-        pong
-        ^[exit
-        ```
-        
-        Send _hello_ to a serial device with 9600 baud, 7 data bits, even parity, and 2 stop bits. Then exit:
-        ```
-        sterm -b 9600 -f 7E2 /dev/ttyS0
-        hello
-        world
-        ^[exit
-        ```
-        
-        Connecting to a Linux device
-        ```
-        sterm --noecho --escape _ /dev/ttyUSB0
-        ~# whoami
-        root
-        ~# _exit
-        ```
-        
-        Communicating with two _sterm_ instances via a pseudo terminal for testing:
-        ![A picture that demonstrates the possibility of receiving ANSI escape sequences and unicode charaters](/stermscreenshot.png?raw=true "Testrun showing some capabilities of sterm")
-        
-        
-        ## ⛏️ Building and Testing <a name = "built_using"></a>
-        
-        ### Testing
-        
-        To test _sterm_ from the sources, just call the `test.py` script.
-        It runs the command line interface of _sterm_.
-        
-        You can use `socat` to create a virtual serial connection with two endings, so that you can use two `sterm` processes to communicate with each other:
-        
-        ```bash
-        socat -d -d pty,raw,echo=0 pty,raw,echo=0
-        ```
-        
-        ### Building a new Package
-        
-        To build a new package from the source code, just execute the `pkg-make.sh` script.
-        Make sure to update the version number in the `sterm/cli.py` file.
-        This version number, as well as the README.md file gets read by the setup.py file.
-        
-        ```bash
-        vim sterm/cli.py
-        ./pkg-make.sh
-        ```
-        
-        
-        ## 🎉 Acknowledgements <a name = "acknowledgement"></a>
-        
-        - [@kylelobo](https://github.com/kylelobo) for [this README template](https://github.com/kylelobo/The-Documentation-Compendium)
-        - [The pyserial project](https://github.com/pyserial/pyserial) that is the base of _sterm_
-        
-        
 Keywords: serial-communication serial-terminal terminal uart rs232 monitoring tty pyserial serial
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
@@ -212,7 +34,239 @@
 Classifier: Topic :: Software Development :: Debuggers
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Logging
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: Utilities
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<h3 align="center">sterm</h3>
+
+<div align="center">
+  Status: 🟢 Active - License: GPL v3
+</div>
+
+---
+
+<p align="center"> sterm is a minimal serial terminal that focus on being easy to use. - This client just does its job.
+    <br/>
+</p>
+
+```bash
+pip install sterm
+sterm --help
+sterm /dev/ttyUSB0
+```
+
+
+## 📝 Table of Contents
+- [About](#about)
+- [Getting Started](#getting_started)
+- [Usage](#usage)
+- [Built Using](#built_using)
+- [Related Work](#related_work)
+- [Acknowledgments](#acknowledgement)
+
+
+## 🧐 About <a name = "about"></a>
+
+**sterm** is a minimal serial terminal that focus on being easy to use and not sucking. - This client simply works.
+It has inline input and supports Unicode (utf-8).
+Each character typed gets directly send to the connected device without buffering.
+It writes whatever it receives to *stdout* so that also Unicode and ANSI escape sequences work as expected.
+
+### Core Use-Cases
+
+*Ideal for debugging:*<br/>
+With the ``--binary`` option, the received data will be output byte wise as hexadecimal numbers.
+
+*Ideal for a remote Linux shell:*<br/>
+With the ``--noecho`` option, each character typed gets directly send to the connected device without buffering and echoing.
+This makes the Linux console usage seamlessly like using telnet or ssh.
+
+### Core Features
+
+- Inline input
+- No line buffering
+- Unicode support
+- ANSI Escape Sequences supported
+- No GUI
+
+
+## 🏁 Getting Started <a name = "getting_started"></a>
+
+There are two ways to install _sterm_.
+**A:** Directly using `pip` or **B:** from the cloned repository.
+
+### Precondition
+
+_sterm_ requires Python 3 to run.
+Before you start installing _sterm_ make sure you use the correct version.
+Depending on your distribution, the you may need to use `pip3` instead of `pip`.
+You can check your Python version by executing the following commands:
+
+```bash
+python --version
+pip --version
+```
+
+Both should print a version number beginning with 3.
+If not, you need to use `pip3` to explicit use Python 3.
+
+For a user-only installation, call `pip ...` as user.
+For a system-wide installation you need to be root, or call `sudo pip ...`.
+
+### A: Installation using pip
+
+```bash
+pip install sterm
+```
+
+### B: Installation from Repository
+
+```bash
+# Download
+git clone https://github.com/rstemmer/sterm.git
+cd sterm
+
+# Dependencies
+pip install pyserial
+
+# Install Package
+pip install .
+
+```
+
+### Check installation
+
+After installation you can check if _sterm_ is successfully installed using `whereis`.
+```bash
+whereis sterm
+#Outpu: sterm: /usr/bin/sterm /usr/man/man1/sterm.1
+```
+There should be two files listed.
+ - `sterm` is the executable, the command you run.
+ - `sterm.1` is the manual for `sterm` that can be read by executing `man sterm` on the command line.
+
+On a system-wide installation, _sterm_ is usually installed to /usr/bin.
+If you only installed to for a single user, it is usually installed to ~/.local/bin
+
+During the installation process, `pip` should install all dependencies recursively.
+To be sure nothing is missing, you can run `pip check sterm`.
+It prints all missing dependencies or version conflicts.
+You can install missing dependencies via `pip`.
+When version conflicts are listed, you can hope they do not matter or install an explicit version via `pip` as well.
+
+
+## 🎈 Usage <a name="usage"></a>
+
+To execute _sterm_ you just have to call the `sterm` command in your shell.
+`sterm` requires one argument, the device you want to access.
+All other arguments listed in the subsection below are optional.
+
+UART-Devices are listed in the /dev directory with the prefix `tty`.
+Most UART-Devices are addressable via /dev/ttyUSBx or /dev/ttyACMx were x is a number depending on the order they got recognized by the Linux kernel.
+
+
+*sterm* has two interfaces:
+
+1. The command line interface
+2. Escape commands
+
+
+### Command Line Arguments
+
+```bash
+sterm [-h] [--noecho] [--escape character] [--binary] [-b BAUDRATE] [-f FORMAT] [-w logfile] DEVICE
+```
+
+When a command line argument is contradictory to a setting in the configuration files, the command line argument has higher priority.
+
+  * __-h__: Print help.
+  * __-n__: Enable _noecho_ mode. _Default_ is echoing each entered key to _stdout_.
+  * __--escape__: Define an alternative escape character. _Default_ is escape ("\e").
+  * __--binary__: Print hexadecimal values instead of Unicode characters. (Only applied on output, input will still be UTF-8)
+  * __-b__: Baudrate. _Default:_ 115200 baud.
+  * __-f__: Configuration-triple: xyz with x = bytelength in bits {5,6,7,8}; y = parity {N,E,O}; z = stopbits {1,2}. _Default:_ "8N1" - _8_ data bits, _no_ parity bits and _1_ stop bit.
+  * __-w__: Write received data into a file.
+
+_DEVICE_ is the path to the serial terminal.
+For example _/dev/ttyS0_, _/dev/ttyUSB0_, _/dev/ttyUART0_, _/dev/ttyACM0_, _/dev/pts/42_.
+
+For details read the man-page.
+
+### Escape commands
+
+The following strings can be entered while _sterm_ is running.
+Just hit the escape-key and then enter the commands.
+They get not send to the device.
+Instead they are interpreted by _sterm_.
+The preceded escape character can be defined with --escape.
+Default is the escape key ("\e").
+
+  * __exit__: quit sterm
+  * __version__: print version
+
+### Examples
+
+Send _ping_ to UART0 and exit:
+```
+sterm /dev/ttyUART0
+ping
+pong
+^[exit
+```
+
+Send _hello_ to a serial device with 9600 baud, 7 data bits, even parity, and 2 stop bits. Then exit:
+```
+sterm -b 9600 -f 7E2 /dev/ttyS0
+hello
+world
+^[exit
+```
+
+Connecting to a Linux device
+```
+sterm --noecho --escape _ /dev/ttyUSB0
+~# whoami
+root
+~# _exit
+```
+
+Communicating with two _sterm_ instances via a pseudo terminal for testing:
+![A picture that demonstrates the possibility of receiving ANSI escape sequences and unicode charaters](/stermscreenshot.png?raw=true "Testrun showing some capabilities of sterm")
+
+
+## ⛏️ Building and Testing <a name = "built_using"></a>
+
+### Testing
+
+To test _sterm_ from the sources, just call the `test.py` script.
+It runs the command line interface of _sterm_.
+
+You can use `socat` to create a virtual serial connection with two endings, so that you can use two `sterm` processes to communicate with each other:
+
+```bash
+socat -d -d pty,raw,echo=0 pty,raw,echo=0
+```
+
+### Building a new Package
+
+To build a new package from the source code, just execute the `pkg-make.sh` script.
+Make sure to update the version number in the `sterm/cli.py` file.
+This version number, as well as the README.md file gets read by the setup.py file.
+
+```bash
+vim sterm/cli.py
+./pkg-make.sh
+```
+
+## ⛓ Related Work <a name ="related_work"></a>
+
+ - [tio](https://github.com/tio/tio) A more feature rich alternative to `sterm` with a similar motivation
+
+## 🎉 Acknowledgements <a name = "acknowledgement"></a>
+
+- [@kylelobo](https://github.com/kylelobo) for [this README template](https://github.com/kylelobo/The-Documentation-Compendium)
+- [The pyserial project](https://github.com/pyserial/pyserial) that is the base of _sterm_
+
```

