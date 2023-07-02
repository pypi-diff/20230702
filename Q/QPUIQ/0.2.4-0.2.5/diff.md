# Comparing `tmp/QPUIQ-0.2.4.tar.gz` & `tmp/QPUIQ-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QPUIQ-0.2.4.tar", last modified: Mon Jun 19 04:17:46 2023, max compression
+gzip compressed data, was "QPUIQ-0.2.5.tar", last modified: Sun Jul  2 19:32:46 2023, max compression
```

## Comparing `QPUIQ-0.2.4.tar` & `QPUIQ-0.2.5.tar`

### file list

```diff
@@ -1,87 +1,89 @@
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-06-19 04:17:46.499378 QPUIQ-0.2.4/
--rw-r--r--   0 Bug        (504) staff       (20)     1072 2023-06-05 21:02:12.000000 QPUIQ-0.2.4/LICENSE.txt
--rw-r--r--   0 Bug        (504) staff       (20)     7141 2023-06-19 04:17:46.499244 QPUIQ-0.2.4/PKG-INFO
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-06-19 04:17:46.488068 QPUIQ-0.2.4/PUI/
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-06-19 04:17:46.491257 QPUIQ-0.2.4/PUI/PySide6/
--rw-r--r--   0 Bug        (504) staff       (20)      860 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/PySide6/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      496 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/PySide6/application.py
--rw-r--r--   0 Bug        (504) staff       (20)     5105 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/PySide6/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      561 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/PySide6/button.py
--rw-r--r--   0 Bug        (504) staff       (20)     2765 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/PySide6/canvas.py
--rw-r--r--   0 Bug        (504) staff       (20)      750 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/PySide6/checkbox.py
--rw-r--r--   0 Bug        (504) staff       (20)     2327 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/PySide6/combobox.py
--rw-r--r--   0 Bug        (504) staff       (20)      708 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/PySide6/label.py
--rw-r--r--   0 Bug        (504) staff       (20)     1561 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/PySide6/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      801 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/PySide6/mdi.py
--rw-r--r--   0 Bug        (504) staff       (20)     2780 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/PySide6/menu.py
--rw-r--r--   0 Bug        (504) staff       (20)      479 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/PySide6/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      770 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/PySide6/radiobutton.py
--rw-r--r--   0 Bug        (504) staff       (20)     2903 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/PySide6/scroll.py
--rw-r--r--   0 Bug        (504) staff       (20)      793 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/PySide6/splitter.py
--rw-r--r--   0 Bug        (504) staff       (20)     1192 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/PySide6/tab.py
--rw-r--r--   0 Bug        (504) staff       (20)     1418 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/PySide6/text.py
--rw-r--r--   0 Bug        (504) staff       (20)     1286 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/PySide6/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)     1899 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/PySide6/window.py
--rw-r--r--   0 Bug        (504) staff       (20)      557 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      432 2023-06-05 21:02:12.000000 QPUIQ-0.2.4/PUI/decorator.py
--rw-r--r--   0 Bug        (504) staff       (20)     3705 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/dom.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-06-19 04:17:46.493844 QPUIQ-0.2.4/PUI/flet/
--rw-r--r--   0 Bug        (504) staff       (20)      421 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/flet/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      587 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/flet/application.py
--rw-r--r--   0 Bug        (504) staff       (20)      848 2023-06-05 21:02:12.000000 QPUIQ-0.2.4/PUI/flet/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      540 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/flet/button.py
--rw-r--r--   0 Bug        (504) staff       (20)     2066 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/flet/canvas.py
--rw-r--r--   0 Bug        (504) staff       (20)      633 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/flet/checkbox.py
--rw-r--r--   0 Bug        (504) staff       (20)      678 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/flet/label.py
--rw-r--r--   0 Bug        (504) staff       (20)     1201 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/flet/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      620 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/flet/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      830 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/flet/radiobutton.py
--rw-r--r--   0 Bug        (504) staff       (20)     1664 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/flet/scroll.py
--rw-r--r--   0 Bug        (504) staff       (20)     1003 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/flet/tab.py
--rw-r--r--   0 Bug        (504) staff       (20)     1457 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/flet/text.py
--rw-r--r--   0 Bug        (504) staff       (20)      838 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/flet/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)      750 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/flet/window.py
--rw-r--r--   0 Bug        (504) staff       (20)     5593 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/node.py
--rw-r--r--   0 Bug        (504) staff       (20)    13538 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/state.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-06-19 04:17:46.496247 QPUIQ-0.2.4/PUI/textual/
--rw-r--r--   0 Bug        (504) staff       (20)      685 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/textual/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)     2144 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/textual/application.py
--rw-r--r--   0 Bug        (504) staff       (20)     2950 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/textual/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      436 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/textual/button.py
--rw-r--r--   0 Bug        (504) staff       (20)      518 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/textual/checkbox.py
--rw-r--r--   0 Bug        (504) staff       (20)     1299 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/textual/label.py
--rw-r--r--   0 Bug        (504) staff       (20)     1548 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/textual/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      501 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/textual/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      621 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/textual/radiobutton.py
--rw-r--r--   0 Bug        (504) staff       (20)     1611 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/textual/scroll.py
--rw-r--r--   0 Bug        (504) staff       (20)     2280 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/textual/tab.py
--rw-r--r--   0 Bug        (504) staff       (20)      473 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/textual/text.py
--rw-r--r--   0 Bug        (504) staff       (20)      785 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/textual/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)      380 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/textual/window.py
--rw-r--r--   0 Bug        (504) staff       (20)     1005 2023-06-05 21:02:12.000000 QPUIQ-0.2.4/PUI/timeline.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-06-19 04:17:46.498522 QPUIQ-0.2.4/PUI/tkinter/
--rw-r--r--   0 Bug        (504) staff       (20)      495 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/tkinter/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      951 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/tkinter/application.py
--rw-r--r--   0 Bug        (504) staff       (20)     2416 2023-06-08 11:30:01.000000 QPUIQ-0.2.4/PUI/tkinter/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      467 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/tkinter/button.py
--rw-r--r--   0 Bug        (504) staff       (20)     1127 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/tkinter/canvas.py
--rw-r--r--   0 Bug        (504) staff       (20)      741 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/tkinter/checkbox.py
--rw-r--r--   0 Bug        (504) staff       (20)      536 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/tkinter/label.py
--rw-r--r--   0 Bug        (504) staff       (20)     2698 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/tkinter/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      488 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/tkinter/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      750 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/tkinter/radiobutton.py
--rw-r--r--   0 Bug        (504) staff       (20)     3669 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/tkinter/scroll.py
--rw-r--r--   0 Bug        (504) staff       (20)     1743 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/tkinter/tab.py
--rw-r--r--   0 Bug        (504) staff       (20)      475 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/tkinter/text.py
--rw-r--r--   0 Bug        (504) staff       (20)      862 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/tkinter/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)     1548 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/tkinter/window.py
--rw-r--r--   0 Bug        (504) staff       (20)      505 2023-06-05 21:02:12.000000 QPUIQ-0.2.4/PUI/utils.py
--rw-r--r--   0 Bug        (504) staff       (20)     2929 2023-06-08 11:30:01.000000 QPUIQ-0.2.4/PUI/view.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-06-19 04:17:46.499053 QPUIQ-0.2.4/QPUIQ.egg-info/
--rw-r--r--   0 Bug        (504) staff       (20)     7141 2023-06-19 04:17:46.000000 QPUIQ-0.2.4/QPUIQ.egg-info/PKG-INFO
--rw-r--r--   0 Bug        (504) staff       (20)     1652 2023-06-19 04:17:46.000000 QPUIQ-0.2.4/QPUIQ.egg-info/SOURCES.txt
--rw-r--r--   0 Bug        (504) staff       (20)        1 2023-06-19 04:17:46.000000 QPUIQ-0.2.4/QPUIQ.egg-info/dependency_links.txt
--rw-r--r--   0 Bug        (504) staff       (20)        4 2023-06-19 04:17:46.000000 QPUIQ-0.2.4/QPUIQ.egg-info/top_level.txt
--rw-r--r--   0 Bug        (504) staff       (20)     6881 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/README.md
--rw-r--r--   0 Bug        (504) staff       (20)       38 2023-06-19 04:17:46.499414 QPUIQ-0.2.4/setup.cfg
--rw-r--r--   0 Bug        (504) staff       (20)      539 2023-06-05 21:02:12.000000 QPUIQ-0.2.4/setup.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-07-02 19:32:46.337212 QPUIQ-0.2.5/
+-rw-r--r--   0 Bug        (504) staff       (20)     1072 2023-06-05 21:02:12.000000 QPUIQ-0.2.5/LICENSE.txt
+-rw-r--r--   0 Bug        (504) staff       (20)     7847 2023-07-02 19:32:46.337084 QPUIQ-0.2.5/PKG-INFO
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-07-02 19:32:46.323477 QPUIQ-0.2.5/PUI/
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-07-02 19:32:46.327410 QPUIQ-0.2.5/PUI/PySide6/
+-rw-r--r--   0 Bug        (504) staff       (20)      925 2023-06-30 19:44:46.000000 QPUIQ-0.2.5/PUI/PySide6/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      497 2023-06-30 19:44:46.000000 QPUIQ-0.2.5/PUI/PySide6/application.py
+-rw-r--r--   0 Bug        (504) staff       (20)     5783 2023-07-02 15:30:26.000000 QPUIQ-0.2.5/PUI/PySide6/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      561 2023-06-19 04:17:18.000000 QPUIQ-0.2.5/PUI/PySide6/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2765 2023-06-19 04:17:18.000000 QPUIQ-0.2.5/PUI/PySide6/canvas.py
+-rw-r--r--   0 Bug        (504) staff       (20)      750 2023-06-19 04:17:18.000000 QPUIQ-0.2.5/PUI/PySide6/checkbox.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2327 2023-06-19 04:17:18.000000 QPUIQ-0.2.5/PUI/PySide6/combobox.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2197 2023-07-02 19:31:49.000000 QPUIQ-0.2.5/PUI/PySide6/dialog.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1032 2023-06-30 19:44:46.000000 QPUIQ-0.2.5/PUI/PySide6/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1561 2023-06-19 04:17:18.000000 QPUIQ-0.2.5/PUI/PySide6/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      801 2023-06-19 04:17:18.000000 QPUIQ-0.2.5/PUI/PySide6/mdi.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2802 2023-06-30 19:44:46.000000 QPUIQ-0.2.5/PUI/PySide6/menu.py
+-rw-r--r--   0 Bug        (504) staff       (20)     4366 2023-06-30 19:44:46.000000 QPUIQ-0.2.5/PUI/PySide6/modal.py
+-rw-r--r--   0 Bug        (504) staff       (20)      479 2023-06-19 04:17:18.000000 QPUIQ-0.2.5/PUI/PySide6/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      770 2023-06-19 04:17:18.000000 QPUIQ-0.2.5/PUI/PySide6/radiobutton.py
+-rw-r--r--   0 Bug        (504) staff       (20)     5566 2023-06-30 19:44:46.000000 QPUIQ-0.2.5/PUI/PySide6/scroll.py
+-rw-r--r--   0 Bug        (504) staff       (20)      793 2023-06-19 04:17:18.000000 QPUIQ-0.2.5/PUI/PySide6/splitter.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1192 2023-06-19 04:17:18.000000 QPUIQ-0.2.5/PUI/PySide6/tab.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1706 2023-06-30 19:44:46.000000 QPUIQ-0.2.5/PUI/PySide6/text.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1508 2023-07-02 19:31:49.000000 QPUIQ-0.2.5/PUI/PySide6/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2032 2023-06-30 19:44:46.000000 QPUIQ-0.2.5/PUI/PySide6/window.py
+-rw-r--r--   0 Bug        (504) staff       (20)      557 2023-07-02 19:31:49.000000 QPUIQ-0.2.5/PUI/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      432 2023-06-05 21:02:12.000000 QPUIQ-0.2.5/PUI/decorator.py
+-rw-r--r--   0 Bug        (504) staff       (20)     3984 2023-06-30 19:44:46.000000 QPUIQ-0.2.5/PUI/dom.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-07-02 19:32:46.330031 QPUIQ-0.2.5/PUI/flet/
+-rw-r--r--   0 Bug        (504) staff       (20)      421 2023-06-19 04:17:18.000000 QPUIQ-0.2.5/PUI/flet/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      587 2023-06-19 04:17:18.000000 QPUIQ-0.2.5/PUI/flet/application.py
+-rw-r--r--   0 Bug        (504) staff       (20)      848 2023-06-05 21:02:12.000000 QPUIQ-0.2.5/PUI/flet/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      540 2023-06-19 04:17:18.000000 QPUIQ-0.2.5/PUI/flet/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2066 2023-06-19 04:17:18.000000 QPUIQ-0.2.5/PUI/flet/canvas.py
+-rw-r--r--   0 Bug        (504) staff       (20)      633 2023-06-19 04:17:18.000000 QPUIQ-0.2.5/PUI/flet/checkbox.py
+-rw-r--r--   0 Bug        (504) staff       (20)      678 2023-06-30 19:44:46.000000 QPUIQ-0.2.5/PUI/flet/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1201 2023-06-19 04:17:18.000000 QPUIQ-0.2.5/PUI/flet/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      620 2023-06-19 04:17:18.000000 QPUIQ-0.2.5/PUI/flet/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      830 2023-06-19 04:17:18.000000 QPUIQ-0.2.5/PUI/flet/radiobutton.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2212 2023-06-30 19:44:46.000000 QPUIQ-0.2.5/PUI/flet/scroll.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1003 2023-06-19 04:17:18.000000 QPUIQ-0.2.5/PUI/flet/tab.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1457 2023-06-30 19:44:46.000000 QPUIQ-0.2.5/PUI/flet/text.py
+-rw-r--r--   0 Bug        (504) staff       (20)      838 2023-06-19 04:17:18.000000 QPUIQ-0.2.5/PUI/flet/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)      750 2023-06-19 04:17:18.000000 QPUIQ-0.2.5/PUI/flet/window.py
+-rw-r--r--   0 Bug        (504) staff       (20)     5653 2023-06-30 19:44:46.000000 QPUIQ-0.2.5/PUI/node.py
+-rw-r--r--   0 Bug        (504) staff       (20)    13523 2023-06-30 19:44:46.000000 QPUIQ-0.2.5/PUI/state.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-07-02 19:32:46.334237 QPUIQ-0.2.5/PUI/textual/
+-rw-r--r--   0 Bug        (504) staff       (20)      685 2023-06-19 04:17:18.000000 QPUIQ-0.2.5/PUI/textual/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2144 2023-06-19 04:17:18.000000 QPUIQ-0.2.5/PUI/textual/application.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2950 2023-06-19 04:17:18.000000 QPUIQ-0.2.5/PUI/textual/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      436 2023-06-19 04:17:18.000000 QPUIQ-0.2.5/PUI/textual/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)      518 2023-06-19 04:17:18.000000 QPUIQ-0.2.5/PUI/textual/checkbox.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1299 2023-06-30 19:44:46.000000 QPUIQ-0.2.5/PUI/textual/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1536 2023-06-30 19:44:46.000000 QPUIQ-0.2.5/PUI/textual/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      501 2023-06-19 04:17:18.000000 QPUIQ-0.2.5/PUI/textual/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      621 2023-06-19 04:17:18.000000 QPUIQ-0.2.5/PUI/textual/radiobutton.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2158 2023-06-30 19:44:46.000000 QPUIQ-0.2.5/PUI/textual/scroll.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2280 2023-06-19 04:17:18.000000 QPUIQ-0.2.5/PUI/textual/tab.py
+-rw-r--r--   0 Bug        (504) staff       (20)      778 2023-06-30 19:44:46.000000 QPUIQ-0.2.5/PUI/textual/text.py
+-rw-r--r--   0 Bug        (504) staff       (20)      785 2023-06-19 04:17:18.000000 QPUIQ-0.2.5/PUI/textual/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)      380 2023-06-19 04:17:18.000000 QPUIQ-0.2.5/PUI/textual/window.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1005 2023-06-05 21:02:12.000000 QPUIQ-0.2.5/PUI/timeline.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-07-02 19:32:46.336360 QPUIQ-0.2.5/PUI/tkinter/
+-rw-r--r--   0 Bug        (504) staff       (20)      514 2023-06-30 19:44:46.000000 QPUIQ-0.2.5/PUI/tkinter/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      791 2023-06-30 19:44:46.000000 QPUIQ-0.2.5/PUI/tkinter/application.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2602 2023-06-30 19:44:46.000000 QPUIQ-0.2.5/PUI/tkinter/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      467 2023-06-19 04:17:18.000000 QPUIQ-0.2.5/PUI/tkinter/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1127 2023-06-19 04:17:18.000000 QPUIQ-0.2.5/PUI/tkinter/canvas.py
+-rw-r--r--   0 Bug        (504) staff       (20)      741 2023-06-19 04:17:18.000000 QPUIQ-0.2.5/PUI/tkinter/checkbox.py
+-rw-r--r--   0 Bug        (504) staff       (20)      554 2023-06-30 19:44:46.000000 QPUIQ-0.2.5/PUI/tkinter/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2698 2023-06-19 04:17:18.000000 QPUIQ-0.2.5/PUI/tkinter/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      488 2023-06-19 04:17:18.000000 QPUIQ-0.2.5/PUI/tkinter/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      750 2023-06-19 04:17:18.000000 QPUIQ-0.2.5/PUI/tkinter/radiobutton.py
+-rw-r--r--   0 Bug        (504) staff       (20)     6659 2023-06-30 19:44:46.000000 QPUIQ-0.2.5/PUI/tkinter/scroll.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1743 2023-06-19 04:17:18.000000 QPUIQ-0.2.5/PUI/tkinter/tab.py
+-rw-r--r--   0 Bug        (504) staff       (20)      493 2023-06-30 19:44:46.000000 QPUIQ-0.2.5/PUI/tkinter/text.py
+-rw-r--r--   0 Bug        (504) staff       (20)      862 2023-06-19 04:17:18.000000 QPUIQ-0.2.5/PUI/tkinter/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1548 2023-06-19 04:17:18.000000 QPUIQ-0.2.5/PUI/tkinter/window.py
+-rw-r--r--   0 Bug        (504) staff       (20)      505 2023-06-05 21:02:12.000000 QPUIQ-0.2.5/PUI/utils.py
+-rw-r--r--   0 Bug        (504) staff       (20)     3021 2023-06-30 19:44:46.000000 QPUIQ-0.2.5/PUI/view.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-07-02 19:32:46.336885 QPUIQ-0.2.5/QPUIQ.egg-info/
+-rw-r--r--   0 Bug        (504) staff       (20)     7847 2023-07-02 19:32:46.000000 QPUIQ-0.2.5/QPUIQ.egg-info/PKG-INFO
+-rw-r--r--   0 Bug        (504) staff       (20)     1695 2023-07-02 19:32:46.000000 QPUIQ-0.2.5/QPUIQ.egg-info/SOURCES.txt
+-rw-r--r--   0 Bug        (504) staff       (20)        1 2023-07-02 19:32:46.000000 QPUIQ-0.2.5/QPUIQ.egg-info/dependency_links.txt
+-rw-r--r--   0 Bug        (504) staff       (20)        4 2023-07-02 19:32:46.000000 QPUIQ-0.2.5/QPUIQ.egg-info/top_level.txt
+-rw-r--r--   0 Bug        (504) staff       (20)     7587 2023-07-02 15:30:26.000000 QPUIQ-0.2.5/README.md
+-rw-r--r--   0 Bug        (504) staff       (20)       38 2023-07-02 19:32:46.337258 QPUIQ-0.2.5/setup.cfg
+-rw-r--r--   0 Bug        (504) staff       (20)      539 2023-06-05 21:02:12.000000 QPUIQ-0.2.5/setup.py
```

### Comparing `QPUIQ-0.2.4/LICENSE.txt` & `QPUIQ-0.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.4/PKG-INFO` & `QPUIQ-0.2.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QPUIQ
-Version: 0.2.4
+Version: 0.2.5
 Summary: "PUI" Python Declarative UI Framework
 Home-page: https://github.com/buganini/PUI
 Author: Buganini Chiu
 Author-email: buganini@b612.tw
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -179,15 +179,15 @@
 ## Lower Priority
 * tkinter
     * or https://github.com/rdbende/Sun-Valley-ttk-theme
 * flet
 * textual (Text Mode)
     * no canvas
 
-# Components
+# Declarative Components
 |Generic|PySide6|flet|tkinter|textual|
 |-------|-------|----|-------|-------|
 |Application|QApplication|Page|Tk|App|
 |Window|QMainWindow|✓(Single)|Toplevel|✓(Single)|
 |HBox|QHBoxLayout|Row|Frame(grid)|Horizontal|
 |VBox|QVBoxLayout|Column|Frame(grid)|Vertical|
 |Spacer|QSpacerItem|✓|✓|✓|
@@ -197,27 +197,41 @@
 |RadioButton|QRadioButton|Radio|Radiobutton|RadioButton|
 |Canvas|✓(QWidget)|Canvas|Canvas|-|
 |TextField|QLineEdit|TextField|Entry|Input|
 |ProgressBar|QProgressBar|ProgressBar|Progressbar|ProgressBar|
 |Scroll|QScrollArea|✓|✓|ScrollableContainer|
 |Text|QLabel|Text|Label|Text|
 |Html|QLabel|⚠ Text|⚠ Label|⚠ Text|
-|MarkDown|QLabel|Markdown|⚠ Label|⚠ Text|
+|MarkDown|QLabel|Markdown|⚠ Label|Markdown|
 |Combobox|QComboBox|-|-|-|
 |ComboboxItem|✓|-|-|-|
 |Tabs|QTabWidget|Tabs|Notebook|Tabs|
 |Tab|✓|Tab|✓|✓|
 |MenuBar|QMenuBar|-|-|-|
 |Menu|QMenu|-|-|-|
 |MenuAction|QAction|-|-|-|
 |MdiArea|QMdiArea|-|-|-|
 |MdiSubWindow|QMdiSubWindow|-|-|-|
 |Splitter|QSplitter|-|-|-|
+|Modal|✓(QWidget)|-|-|-|
 |(Wrapper)|`QtWrapper`|-|-|-|
 
+# Imperative Dialogs
+|Generic|PySide6|flet|tkinter|textual|
+|-------|-------|----|-------|-------|
+|OpenDirectory|QFileDialog.getExistingDirectory|-|-|-|
+|OpenFile|QFileDialog.getOpenFileName|-|-|-|
+|OpenFiles|QFileDialog.getOpenFileNames|-|-|-|
+|SaveFile|QFileDialog.getSaveFileName|-|-|-|
+|Information|QMessageBox|-|-|-|
+|Warning|QMessageBox|-|-|-|
+|Critical|QMessageBox|-|-|-|
+|Confirm|QMessageBox|-|-|-|
+|Prompt|QInputDialog|-|-|-|
+
 ## Interfaces
 * Button(text)
     * .click(callback, *cb_args, **cb_kwargs)
 * Label(text)
     * .click(callback, *cb_args, **cb_kwargs)
 * TextField(binding)
 * ProgressBar(progress `0-1`)
@@ -241,14 +255,20 @@
 # reloadium: after_reload
 def after_reload(actions):
     PUIView.reload()
 ```
 
 
 # TODO
+* [ISSUE] empty virtual node
+* [ISSUE] textual layout sizing (cookbook scroll example)
+* [ISSUE] flet layout sizing (cookbook scroll example)
+* nested state trigger
+    * set state in PUIView __init__
+    * set state in setup() ?
 * Tabs(`tabposition`)
 * Lazy List
 * StateObject decorator
 * UI Flow
     * Navigation Stack
     * View Router
     * Model Window/Dialog
```

### Comparing `QPUIQ-0.2.4/PUI/PySide6/__init__.py` & `QPUIQ-0.2.5/PUI/PySide6/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 from PySide6.QtWidgets import QSizePolicy, QLayout
 
 from .application import *
 from .button import *
 from .canvas import *
 from .checkbox import *
 from .combobox import *
+from .dialog import *
 from .label import *
 from .layout import *
+from .modal import *
 from .progressbar import *
 from .radiobutton import *
 from .scroll import *
 from .splitter import *
 from .tab import *
 from .text import *
 from .textfield import *
 from .window import *
 from .mdi import *
 
+PUIView = QtPUIView
+
 def PUI(func):
     """
     PUI.PySide6.PUI triggers update() by signal/slot
     """
     def func_wrapper(*args):
-        class PUIViewWrapper(QPUIView):
+        class PUIViewWrapper(QtPUIView):
             def __init__(self, name):
                 self.name = name
                 super().__init__()
 
             def content(self):
                 return func(*args)
```

### Comparing `QPUIQ-0.2.4/PUI/PySide6/base.py` & `QPUIQ-0.2.5/PUI/PySide6/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from .. import *
-
 from PySide6 import QtCore, QtWidgets, QtGui
 
 class QtViewSignal(QtCore.QObject):
     redraw = QtCore.Signal()
 
 def _apply_params(ui, node):
     styles = {}
     if node.style_fontsize:
         styles["font"] = f"{node.style_fontsize}pt"
+    if node.style_fontfamily:
+        styles["font-family"] = node.style_fontfamily
     if node.style_color:
         styles["color"] = f"#{node.style_color:06X}"
     if node.style_bgcolor:
         styles["background-color"] = f"#{node.style_bgcolor:06X}"
 
     HorizontalPolicy = node.qt_params.get("HorizontalPolicy")
     if not HorizontalPolicy is None:
@@ -32,34 +33,34 @@
 
     if hasattr(ui, "setStyleSheet"):
         ui.setStyleSheet("".join([f"{k}:{v};" for k,v in styles.items()]))
 
     if node.layout_padding:
         ui.setContentsMargins(*trbl2ltrb(node.layout_padding))
 
-class QPUIView(PUIView):
-    def __init__(self):
-        super().__init__()
+class QtPUIView(PUIView):
+    def __init__(self, *args):
+        super().__init__(*args)
         self.qt_params = {}
-        self.signal = QtViewSignal()
-        self.signal.redraw.connect(self.update)
+        self._qtsignal = QtViewSignal()
+        self._qtsignal.redraw.connect(self.update)
 
     def destroy(self, direct):
         if direct:
             if self.ui: # PUIView doesn't have ui
                 self.ui.deleteLater()
         self.ui = None
         super().destroy(direct)
 
     def redraw(self):
         self.dirty = True
         if self.updating:
             return
         self.updating = True
-        self.signal.redraw.emit()
+        self._qtsignal.redraw.emit()
 
     def update(self, prev=None):
         if self.retired_by:
             return
         self.dirty = False
         super().update(prev)
         _apply_params(self.ui, self)
@@ -83,16 +84,30 @@
         if direct:
             self.ui.deleteLater()
         self.ui = None
         super().destroy(direct)
 
     def update(self, prev=None):
         super().update(prev)
+        if not hasattr(self.ui, "origSizeHint"):
+            self.ui.origSizeHint = self.ui.sizeHint
+        self.ui.sizeHint = self.qtSizeHint
         _apply_params(self.ui, self)
 
+    def qtSizeHint(self):
+        node = self.get_node()
+        sh = node.ui.origSizeHint()
+        w = sh.width()
+        h = sh.height()
+        if not node.layout_width is None:
+            w = node.layout_width
+        if not node.layout_height is None:
+            h = node.layout_height
+        return QtCore.QSize(w, h)
+
     def qt(self, **kwargs):
         for k,v in kwargs.items():
             self.qt_params[k] = v
         return self
 
 class QtBaseLayout(PUINode):
     def __init__(self):
@@ -105,41 +120,45 @@
 
     @property
     def inner(self):
         return self.layout
 
     def destroy(self, direct):
         if direct:
-            self.layout.setParent(None)
-            self.layout.deleteLater()
             self.ui.deleteLater()
         self.layout = None
         self.ui = None
         super().destroy(direct)
 
     def update(self, prev=None):
         super().update(prev)
         _apply_params(self.ui, self)
 
     def addChild(self, idx, child):
+        from .modal import Modal
         from .layout import Spacer
         if isinstance(child, Spacer):
             self.layout.insertItem(idx, child.outer)
+        elif isinstance(child, Modal):
+            pass
         elif isinstance(child, QtBaseWidget) or isinstance(child, QtBaseLayout):
             params = {}
             if not child.layout_weight is None:
                 params["stretch"] = child.layout_weight
             self.layout.insertWidget(idx, child.outer, **params)
         elif child.children:
             self.addChild(idx, child.children[0])
 
     def removeChild(self, idx, child):
+        from .modal import Modal
         from .layout import Spacer
         if isinstance(child, Spacer):
             self.layout.removeItem(child.outer)
+        elif isinstance(child, Modal):
+            pass
         elif isinstance(child, QtBaseWidget) or isinstance(child, QtBaseLayout):
             child.outer.setParent(None)
         elif child.children:
             self.removeChild(idx, child.children[0])
 
     def qt(self, **kwargs):
         for k,v in kwargs.items():
```

### Comparing `QPUIQ-0.2.4/PUI/PySide6/button.py` & `QPUIQ-0.2.5/PUI/PySide6/button.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.4/PUI/PySide6/canvas.py` & `QPUIQ-0.2.5/PUI/PySide6/canvas.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.4/PUI/PySide6/checkbox.py` & `QPUIQ-0.2.5/PUI/PySide6/checkbox.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.4/PUI/PySide6/combobox.py` & `QPUIQ-0.2.5/PUI/PySide6/combobox.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.4/PUI/PySide6/label.py` & `QPUIQ-0.2.5/PUI/PySide6/label.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,25 +2,32 @@
 from .base import *
 
 class ClickableQLabel(QtWidgets.QLabel):
     clicked  = QtCore.Signal()
 
     def mousePressEvent(self, ev):
         self.clicked.emit()
+        super().mousePressEvent(ev)
 
 class Label(QtBaseWidget):
-    def __init__(self, text):
+    def __init__(self, text, selectable=False):
         super().__init__()
         self.text = text
+        self.selectable = selectable
 
     def update(self, prev):
         if prev and prev.ui:
             self.ui = prev.ui
             self.ui.setText(self.text)
         else:
             self.ui = ClickableQLabel(self.text)
             self.ui.setTextFormat(QtCore.Qt.TextFormat.PlainText)
             self.ui.clicked.connect(self._clicked)
         if self.onClicked:
             self.ui.setCursor(QtCore.Qt.PointingHandCursor)
 
+        if self.selectable:
+            self.ui.setTextInteractionFlags(QtCore.Qt.TextInteractionFlag.TextSelectableByMouse)
+        else:
+            self.ui.setTextInteractionFlags(QtCore.Qt.TextInteractionFlag.NoTextInteraction)
+
         super().update(prev)
```

### Comparing `QPUIQ-0.2.4/PUI/PySide6/layout.py` & `QPUIQ-0.2.5/PUI/PySide6/layout.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.4/PUI/PySide6/mdi.py` & `QPUIQ-0.2.5/PUI/PySide6/mdi.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.4/PUI/PySide6/menu.py` & `QPUIQ-0.2.5/PUI/PySide6/menu.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from .. import *
 from .base import *
 
 class MenuBar(PUINode):
+    outoforder = True
     def update(self, prev):
         if prev and prev.ui:
             self.ui = prev.ui
             self.actions = prev.actions
         else:
             self.ui = QtWidgets.QMenuBar()
             self.actions = []
```

### Comparing `QPUIQ-0.2.4/PUI/PySide6/radiobutton.py` & `QPUIQ-0.2.5/PUI/PySide6/radiobutton.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.4/PUI/PySide6/splitter.py` & `QPUIQ-0.2.5/PUI/PySide6/splitter.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.4/PUI/PySide6/tab.py` & `QPUIQ-0.2.5/PUI/PySide6/tab.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.4/PUI/PySide6/text.py` & `QPUIQ-0.2.5/PUI/PySide6/text.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,31 +17,37 @@
     def setSizeHint(self, sizeHint):
         if sizeHint != self._sizehint:
             self._sizehint = sizeHint
             self.adjustSize()
 
 class Text(QtBaseWidget):
     textformat = QtCore.Qt.TextFormat.PlainText
-    def __init__(self, text, sizeHint=(120,320)):
+    def __init__(self, text, selectable=False, sizeHint=(120,320)):
         super().__init__()
         self.text = text
+        self.selectable = selectable
         self.sizeHint = sizeHint
 
     def update(self, prev):
         if prev and prev.ui:
             self.ui = prev.ui
             self.ui.setText(self.text)
             self.ui.setSizeHint(self.sizeHint)
         else:
             self.ui = QText(self.text, self.sizeHint)
             self.ui.setTextFormat(self.textformat)
             self.ui.setAlignment(QtCore.Qt.AlignmentFlag.AlignTop)
             self.ui.setWordWrap(True)
             self.ui.setSizePolicy(QSizePolicy(QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Ignored))
 
+        if self.selectable:
+            self.ui.setTextInteractionFlags(QtCore.Qt.TextInteractionFlag.TextSelectableByMouse)
+        else:
+            self.ui.setTextInteractionFlags(QtCore.Qt.TextInteractionFlag.NoTextInteraction)
+
         super().update(prev)
 
 
 class Html(Text):
     textformat = QtCore.Qt.TextFormat.RichText
 
 class MarkDown(Text):
```

### Comparing `QPUIQ-0.2.4/PUI/PySide6/textfield.py` & `QPUIQ-0.2.5/PUI/PySide6/textfield.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from .base import *
 
 class TextField(QtBaseWidget):
     def __init__(self, model):
         super().__init__()
         self.model = model
         self.editing = False
+        self.changed_cb = None
 
     def update(self, prev):
         value = self.model.value
         if prev and prev.ui:
             self.editing = prev.editing
             self.ui = prev.ui
             self.ui.focusOutEvent = self.focusOutEvent
@@ -24,16 +25,21 @@
             self.ui = QtWidgets.QLineEdit()
             self.ui.origFocusOutEvent = self.ui.focusOutEvent
             self.ui.focusOutEvent = self.focusOutEvent
             self.ui.setText(str(value))
             self.ui.textChanged.connect(self.on_textchanged)
         super().update(prev)
 
+    def change(self, cb, *args, **kwargs):
+        self.changed_cb = (cb, args, kwargs)
+
     def on_textchanged(self):
         node = self.get_node()
         node.editing = True
         node.model.value = self.ui.text()
+        if node.changed_cb:
+            node.changed_cb[0](*node.changed_cb[1], **node.changed_cb[2])
 
     def focusOutEvent(self, event):
         node = self.get_node()
         node.editing = False
         node.ui.origFocusOutEvent(event)
```

### Comparing `QPUIQ-0.2.4/PUI/PySide6/window.py` & `QPUIQ-0.2.5/PUI/PySide6/window.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from .. import *
 from .base import *
 from .menu import *
+from .modal import *
 
 class Window(QtBaseWidget):
     terminal = False
 
     def __init__(self, title=None, size=None, maximize=None, fullscreen=None):
         super().__init__()
         self.title = title
@@ -37,19 +38,23 @@
         if not self.title is None:
             self.ui.setWindowTitle(self.title)
         super().update(prev)
 
     def addChild(self, idx, child):
         if isinstance(child, MenuBar):
             self.ui.setMenuBar(child.outer)
+        elif isinstance(child, Modal):
+            pass
         elif isinstance(child, QtBaseWidget) or isinstance(child, QtBaseLayout):
             self.ui.setCentralWidget(child.outer)
         else:
             self.addChild(idx, child.children[0])
 
     def removeChild(self, idx, child):
         if isinstance(child, MenuBar):
             child.outer.close()
+        elif isinstance(child, Modal):
+            pass
         elif isinstance(child, QtBaseWidget) or isinstance(child, QtBaseLayout):
             child.outer.setParent(None)
         else:
             self.removeChild(idx, child.children[0])
```

### Comparing `QPUIQ-0.2.4/PUI/__init__.py` & `QPUIQ-0.2.5/PUI/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.4"
+__version__ = "0.2.5"
 
 from .node import *
 from .view import *
 from .state import *
 from .timeline import *
 from .decorator import *
```

### Comparing `QPUIQ-0.2.4/PUI/dom.py` & `QPUIQ-0.2.5/PUI/dom.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,27 +3,42 @@
 
 def recur_delete(node, child, direct):
     child.destroyed = True
     for sc in child.children:
         recur_delete(child, sc, False)
     child.destroy(direct)
 
+def sortDOM(dom):
+    sorted = []
+    ooo = []
+    for e in dom:
+        if e.outoforder:
+            ooo.append(e)
+        else:
+            sorted.append(e)
+    sorted.extend(ooo)
+    return sorted
+
 def sync(node, oldDOM, newDOM):
+    oldDOM = sortDOM(oldDOM)
+    newDOM = sortDOM(newDOM)
     dprint("syncing", node.key, len(oldDOM), len(newDOM))
 
     dprint("  ===OLD===")
     for c in oldDOM:
         dprint("   ", c.key)
 
     dprint("  ===NEW===")
     for c in newDOM:
         dprint("   ", c.key)
     oldMap = [x.key for x in oldDOM]
     newMap = [x.key for x in newDOM]
 
+    node.preSync()
+
     tbd = []
     for i,new in enumerate(newDOM):
         while True:
             if i < len(oldDOM) and oldMap[i] == new.key: # matched
                 dprint(f"MATCHED {i} {new.key}")
                 old = oldDOM[i]
```

### Comparing `QPUIQ-0.2.4/PUI/flet/application.py` & `QPUIQ-0.2.5/PUI/flet/application.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.4/PUI/flet/base.py` & `QPUIQ-0.2.5/PUI/flet/base.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.4/PUI/flet/button.py` & `QPUIQ-0.2.5/PUI/flet/button.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.4/PUI/flet/canvas.py` & `QPUIQ-0.2.5/PUI/flet/canvas.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.4/PUI/flet/checkbox.py` & `QPUIQ-0.2.5/PUI/flet/checkbox.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.4/PUI/flet/label.py` & `QPUIQ-0.2.5/PUI/textual/text.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 from .. import *
 from .base import *
 
-class Label(FBase):
-    def __init__(self, text, **kwargs):
-        super().__init__(**kwargs)
+class Text(TBase):
+    def __init__(self, text, selectable=False):
+        super().__init__()
         self.text = text
 
     def update(self, prev):
         if prev and prev.ui:
             self.ui = prev.ui
+            self.ui.update(self.text)
         else:
-            self.ui = ft.Text(spans=[])
-        self.ui.expand = self.layout_weight
-        if self.onClicked:
-            self.ui.spans = [
-                ft.TextSpan(self.text, on_click=self._clicked)
-            ]
+            self.ui = widgets.Label(self.text, markup=False)
+        super().update(prev)
+
+class Html(Text):
+    supported = False
+
+class MarkDown(TBase):
+    weak_expand_x = True
+    def __init__(self, text):
+        super().__init__()
+        self.text = text
+
+    def update(self, prev):
+        if prev and prev.ui:
+            self.ui = prev.ui
+            self.ui.update(self.text)
         else:
-            self.ui.spans = [
-                ft.TextSpan(self.text)
-            ]
-        try:
-            self.ui.update()
-        except:
-            pass
-        super().update(prev)
+            self.ui = widgets.Markdown(self.text)
+        super().update(prev)
```

### Comparing `QPUIQ-0.2.4/PUI/flet/layout.py` & `QPUIQ-0.2.5/PUI/flet/layout.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.4/PUI/flet/progressbar.py` & `QPUIQ-0.2.5/PUI/flet/progressbar.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.4/PUI/flet/radiobutton.py` & `QPUIQ-0.2.5/PUI/flet/radiobutton.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.4/PUI/flet/scroll.py` & `QPUIQ-0.2.5/PUI/flet/text.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,55 @@
 from .. import *
 from .base import *
 
-class Scroll(FBase):
-    def __init__(self, vertical=None, horizontal=False):
-        self.vertical = vertical
-        self.horizontal = horizontal
-        self.widget = None
+class Text(FBase):
+    def __init__(self, text, selectable=False):
         super().__init__()
-        self.layout_weight = 1
+        self.text = text
 
     def update(self, prev):
-        if prev and hasattr(prev, "hframe"):
-            self.vframe = prev.vframe
-            self.hframe = prev.hframe
+        if prev and prev.ui:
+            self.ui = prev.ui
+            self.ui.value = self.text
+            try:
+                self.ui.update()
+            except:
+                pass
         else:
-            self.vframe = ft.Column() # outer
-            self.hframe = ft.Row() # inner
-            self.vframe.controls.append(self.hframe)
-        self.vframe.expand = self.layout_weight
-        if self.vertical is None:
-            self.vframe.scroll = ft.ScrollMode.AUTO
-        elif self.vertical:
-            self.vframe.scroll = ft.ScrollMode.ADAPTIVE
-        else:
-            self.vframe.scroll = None
-        if self.horizontal is None:
-            self.hframe.scroll = ft.ScrollMode.AUTO
-        elif self.horizontal:
-            self.hframe.scroll = ft.ScrollMode.ADAPTIVE
+            self.ui = ft.Text(self.text, expand=self.layout_weight)
+        super().update(prev)
+
+class Html(FBase):
+    supported = False
+    def __init__(self, text, **kwargs):
+        super().__init__(**kwargs)
+        self.text = text
+
+    def update(self, prev):
+        if prev and prev.ui:
+            self.ui = prev.ui
+            self.ui.value = self.text
+            try:
+                self.ui.update()
+            except:
+                pass
         else:
-            self.hframe.scroll = None
-        try:
-            self.vframe.update()
-        except:
-            pass
+            self.ui = ft.Text(self.text, expand=self.layout_weight)
         super().update(prev)
 
-    def addChild(self, idx, child):
-        if idx != 0:
-            return
-        self.hframe.controls.insert(idx, child.outer)
-        try:
-            self.hframe.update()
-        except:
-            pass
-
-    def removeChild(self, idx, child):
-        if idx != 0:
-            return
-        self.hframe.controls.pop(idx)
-        self.hframe.update()
-
-    @property
-    def outer(self):
-        return self.vframe
-
-    @property
-    def inner(self):
-        return self.hframe
+class MarkDown(FBase):
+    supported = False
+    def __init__(self, text, **kwargs):
+        super().__init__(**kwargs)
+        self.text = text
+
+    def update(self, prev):
+        if prev and prev.ui:
+            self.ui = prev.ui
+            self.ui.value = self.text
+            try:
+                self.ui.update()
+            except:
+                pass
+        else:
+            self.ui = ft.Markdown(self.text, expand=self.layout_weight, auto_follow_links=True)
+        super().update(prev)
```

### Comparing `QPUIQ-0.2.4/PUI/flet/tab.py` & `QPUIQ-0.2.5/PUI/flet/tab.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.4/PUI/flet/text.py` & `QPUIQ-0.2.5/PUI/flet/label.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,55 +1,27 @@
 from .. import *
 from .base import *
 
-class Text(FBase):
-    def __init__(self, text, **kwargs):
-        super().__init__(**kwargs)
+class Label(FBase):
+    def __init__(self, text, selectable=False):
+        super().__init__()
         self.text = text
 
     def update(self, prev):
         if prev and prev.ui:
             self.ui = prev.ui
-            self.ui.value = self.text
-            try:
-                self.ui.update()
-            except:
-                pass
         else:
-            self.ui = ft.Text(self.text, expand=self.layout_weight)
-        super().update(prev)
-
-class Html(FBase):
-    supported = False
-    def __init__(self, text, **kwargs):
-        super().__init__(**kwargs)
-        self.text = text
-
-    def update(self, prev):
-        if prev and prev.ui:
-            self.ui = prev.ui
-            self.ui.value = self.text
-            try:
-                self.ui.update()
-            except:
-                pass
-        else:
-            self.ui = ft.Text(self.text, expand=self.layout_weight)
-        super().update(prev)
-
-class MarkDown(FBase):
-    supported = False
-    def __init__(self, text, **kwargs):
-        super().__init__(**kwargs)
-        self.text = text
-
-    def update(self, prev):
-        if prev and prev.ui:
-            self.ui = prev.ui
-            self.ui.value = self.text
-            try:
-                self.ui.update()
-            except:
-                pass
+            self.ui = ft.Text(spans=[])
+        self.ui.expand = self.layout_weight
+        if self.onClicked:
+            self.ui.spans = [
+                ft.TextSpan(self.text, on_click=self._clicked)
+            ]
         else:
-            self.ui = ft.Markdown(self.text, expand=self.layout_weight, auto_follow_links=True)
-        super().update(prev)
+            self.ui.spans = [
+                ft.TextSpan(self.text)
+            ]
+        try:
+            self.ui.update()
+        except:
+            pass
+        super().update(prev)
```

### Comparing `QPUIQ-0.2.4/PUI/flet/textfield.py` & `QPUIQ-0.2.5/PUI/flet/textfield.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.4/PUI/flet/window.py` & `QPUIQ-0.2.5/PUI/flet/window.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.4/PUI/node.py` & `QPUIQ-0.2.5/PUI/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
         return tls.puistack[-1]
     except:
         raise PuiViewNotFoundError()
 
 class PUINode():
     supported = True
     terminal = False
+    outoforder = False
     def __init__(self, *args):
         from .view import PUIView
 
         if not hasattr(self, "name"):
             self.name = None
 
         self.destroyed = False
@@ -99,14 +100,17 @@
     def update(self, prev):
         if prev:
             prev.retired_by = self
 
     def postUpdate(self):
         pass
 
+    def preSync(self):
+        pass
+
     def postSync(self):
         pass
 
     def destroy(self, direct):
         self.root = None
         self.parent = None
 
@@ -195,15 +199,15 @@
         self.click_args = cb_args
         self.click_kwargs = cb_kwargs
         return self
 
     def _clicked(self, *args, **kwargs):
         node = self.get_node()
         if node.onClicked:
-            node.onClicked(*self.click_args, **self.click_kwargs)
+            node.onClicked(*node.click_args, **node.click_kwargs)
 
     def flet(self, **kwargs):
         return self
 
     def textual(self, **kwargs):
         return self
```

### Comparing `QPUIQ-0.2.4/PUI/state.py` & `QPUIQ-0.2.5/PUI/state.py`

 * *Files 0% similar despite different names*

```diff
@@ -357,24 +357,24 @@
         _notify(self.__listeners)
         for cb in self.__callbacks[None]:
             cb(self.__values)
 
     def __getitem__(self, key):
         try:
             view = find_puiview()
-            self.__listeners[key].add(view)
+            self.__listeners.add(view)
         except PuiViewNotFoundError:
             pass
         return self.__values[key]
 
     def __getattr__(self, key):
         if not key.startswith("_"):
             try:
                 view = find_puiview()
-                self.__listeners[key].add(view)
+                self.__listeners.add(view)
             except PuiViewNotFoundError:
                 pass
         return getattr(self.__values, key)
 
 
     def __setattr__(self, key, value):
         if key.startswith("_"):
@@ -425,15 +425,15 @@
         _notify(self.__listeners)
         for cb in self.__callbacks[None]:
             cb(self.__values)
 
     def get(self, key, default=None):
         try:
             view = find_puiview()
-            self.__listeners[key].add(view)
+            self.__listeners.add(view)
         except PuiViewNotFoundError:
             pass
         return self.__values.get(key, default)
 
     def items(self):
         try:
             view = find_puiview()
```

### Comparing `QPUIQ-0.2.4/PUI/textual/__init__.py` & `QPUIQ-0.2.5/PUI/textual/__init__.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.4/PUI/textual/application.py` & `QPUIQ-0.2.5/PUI/textual/application.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.4/PUI/textual/base.py` & `QPUIQ-0.2.5/PUI/textual/base.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.4/PUI/textual/checkbox.py` & `QPUIQ-0.2.5/PUI/textual/checkbox.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.4/PUI/textual/label.py` & `QPUIQ-0.2.5/PUI/textual/label.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .. import *
 from .base import *
 
 class Label(TBase):
-    def __init__(self, text, **kwargs):
-        super().__init__(**kwargs)
+    def __init__(self, text, selectable=False):
+        super().__init__()
         self.widget = None
         self.text = text
 
     def update(self, prev):
         if prev and prev.ui:
             self.ui = prev.ui
             self.widget = prev.widget
```

### Comparing `QPUIQ-0.2.4/PUI/textual/layout.py` & `QPUIQ-0.2.5/PUI/textual/layout.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,16 +40,16 @@
     def removeChild(self, idx, child):
         if isinstance(child, TBase):
             child.tremove()
         elif child.children:
             self.removeChild(idx, child.children[0])
 
 class Spacer(TBase):
-    def __init__(self, *args):
-        super().__init__(*args)
+    def __init__(self):
+        super().__init__()
         self.layout_weight = 1
 
     def update(self, prev):
         if prev and prev.ui:
             self.ui = prev.ui
         else:
             self.ui = widgets.Static("")
```

### Comparing `QPUIQ-0.2.4/PUI/textual/radiobutton.py` & `QPUIQ-0.2.5/PUI/textual/radiobutton.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.4/PUI/textual/scroll.py` & `QPUIQ-0.2.5/PUI/textual/scroll.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from .. import *
 from .base import *
+import math
 
 class Scroll(TBase):
+    END = -0.0
     weak_expand_x = True
     weak_expand_y = True
     def __init__(self, vertical=None, horizontal=False):
         self.vertical = vertical
         self.horizontal = horizontal
+        self.align_x = 0
+        self.align_y = 0
         super().__init__()
 
     def update(self, prev):
         if prev and prev.ui:
             self.ui = prev.ui
         else:
             self.ui = containers.ScrollableContainer()
@@ -50,7 +54,25 @@
             self.addChild(idx, child.children[0])
 
     def removeChild(self, idx, child):
         if isinstance(child, TBase):
             child.tremove()
         else:
             self.removeChild(idx, child.children[0])
+
+    def scrollX(self, pos=0):
+        if math.copysign(1, pos) >= 0:
+            self.align_x = 0
+            self.hsb_offset = pos
+        else:
+            self.align_x = 1
+            self.hsb_offset = abs(pos)
+        return self
+
+    def scrollY(self, pos=0):
+        if math.copysign(1, pos) >= 0:
+            self.align_y = 0
+            self.vsb_offset = pos
+        else:
+            self.align_y = 1
+            self.vsb_offset = abs(pos)
+        return self
```

### Comparing `QPUIQ-0.2.4/PUI/textual/tab.py` & `QPUIQ-0.2.5/PUI/textual/tab.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.4/PUI/textual/textfield.py` & `QPUIQ-0.2.5/PUI/textual/textfield.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.4/PUI/timeline.py` & `QPUIQ-0.2.5/PUI/timeline.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.4/PUI/tkinter/application.py` & `QPUIQ-0.2.5/PUI/tkinter/application.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,15 @@
 from .. import *
 from .base import *
-import functools
 
-class Application(PUIView):
+class Application(TPUIView):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.theme = None
 
-    def redraw(self):
-        if self.ui:
-            self.ui.after(0, functools.partial(self.update))
-        else:
-            self.update()
-
     def tkinter(self, theme=None, **kwargs):
         super().tkinter(**kwargs)
         if theme:
             self.theme = theme
         return self
 
     def update(self, prev=None):
```

### Comparing `QPUIQ-0.2.4/PUI/tkinter/base.py` & `QPUIQ-0.2.5/PUI/tkinter/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 from .. import *
 import tkinter as tk
 from tkinter import ttk
 from tkinter import font as tkFont
+import functools
+
+class TPUIView(PUIView):
+    def redraw(self):
+        if self.ui:
+            self.ui.after(0, functools.partial(self.update))
+        else:
+            self.update()
 
 class TkBaseWidget(PUINode):
     use_ttk = False
     def __init__(self, layout=None, side=None):
         super().__init__()
         self.layout_type = layout
         self.side = side
```

### Comparing `QPUIQ-0.2.4/PUI/tkinter/canvas.py` & `QPUIQ-0.2.5/PUI/tkinter/canvas.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.4/PUI/tkinter/checkbox.py` & `QPUIQ-0.2.5/PUI/tkinter/checkbox.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.4/PUI/tkinter/label.py` & `QPUIQ-0.2.5/PUI/tkinter/label.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .. import *
 from .base import *
 class Label(TkBaseWidget):
-    def __init__(self, text):
+    def __init__(self, text, selectable=False):
         super().__init__()
         self.text = text
 
     def update(self, prev):
         if prev and prev.ui:
             self.ui = prev.ui
             self.ui.config(text = self.text)
```

### Comparing `QPUIQ-0.2.4/PUI/tkinter/layout.py` & `QPUIQ-0.2.5/PUI/tkinter/layout.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.4/PUI/tkinter/radiobutton.py` & `QPUIQ-0.2.5/PUI/tkinter/radiobutton.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.4/PUI/tkinter/tab.py` & `QPUIQ-0.2.5/PUI/tkinter/tab.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.4/PUI/tkinter/textfield.py` & `QPUIQ-0.2.5/PUI/tkinter/textfield.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.4/PUI/tkinter/window.py` & `QPUIQ-0.2.5/PUI/tkinter/window.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.4/PUI/view.py` & `QPUIQ-0.2.5/PUI/view.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,19 +10,19 @@
     __ALLVIEWS__  = []
 
     @staticmethod
     def reload():
         for v in PUIView.__ALLVIEWS__:
             v.redraw()
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args):
         self.frames = []
         self.dirty = False
         self.updating = False
-        super().__init__(*args, **kwargs)
+        super().__init__(*args)
         PUIView.__ALLVIEWS__.append(self)
 
     def __enter__(self):
         if not hasattr(tls, "puistack"):
             tls.puistack = []
         tls.puistack.append(self)
         # print("enter", type(self).__name__, id(self))
@@ -44,15 +44,18 @@
         start = time.time()
         with self as scope:
             self.content()
         dprint(f"content() time: {time.time()-start:.5f}", self.key)
         return scope
 
     def destroy(self, direct):
-        PUIView.__ALLVIEWS__.remove(self)
+        try:
+            PUIView.__ALLVIEWS__.remove(self)
+        except:
+            pass
         return super().destroy(direct)
 
     def redraw(self):
         self.update()
 
     def update(self, prev=None):
         if self.retired_by:
@@ -66,15 +69,18 @@
         else:
             self.setup = None
         update_start = time.time()
         dprint("update()", self.key)
         if prev:
             self.children = prev.children
             prev.retired_by = self
-            PUIView.__ALLVIEWS__.remove(prev)
+            try:
+                PUIView.__ALLVIEWS__.remove(prev)
+            except:
+                pass
 
         last_children = self.children
         self.children = []
         try:
             dprint(f"content() start", self.key)
             start = time.time()
             with self as scope: # init frame stack
```

### Comparing `QPUIQ-0.2.4/QPUIQ.egg-info/PKG-INFO` & `QPUIQ-0.2.5/QPUIQ.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QPUIQ
-Version: 0.2.4
+Version: 0.2.5
 Summary: "PUI" Python Declarative UI Framework
 Home-page: https://github.com/buganini/PUI
 Author: Buganini Chiu
 Author-email: buganini@b612.tw
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -179,15 +179,15 @@
 ## Lower Priority
 * tkinter
     * or https://github.com/rdbende/Sun-Valley-ttk-theme
 * flet
 * textual (Text Mode)
     * no canvas
 
-# Components
+# Declarative Components
 |Generic|PySide6|flet|tkinter|textual|
 |-------|-------|----|-------|-------|
 |Application|QApplication|Page|Tk|App|
 |Window|QMainWindow|✓(Single)|Toplevel|✓(Single)|
 |HBox|QHBoxLayout|Row|Frame(grid)|Horizontal|
 |VBox|QVBoxLayout|Column|Frame(grid)|Vertical|
 |Spacer|QSpacerItem|✓|✓|✓|
@@ -197,27 +197,41 @@
 |RadioButton|QRadioButton|Radio|Radiobutton|RadioButton|
 |Canvas|✓(QWidget)|Canvas|Canvas|-|
 |TextField|QLineEdit|TextField|Entry|Input|
 |ProgressBar|QProgressBar|ProgressBar|Progressbar|ProgressBar|
 |Scroll|QScrollArea|✓|✓|ScrollableContainer|
 |Text|QLabel|Text|Label|Text|
 |Html|QLabel|⚠ Text|⚠ Label|⚠ Text|
-|MarkDown|QLabel|Markdown|⚠ Label|⚠ Text|
+|MarkDown|QLabel|Markdown|⚠ Label|Markdown|
 |Combobox|QComboBox|-|-|-|
 |ComboboxItem|✓|-|-|-|
 |Tabs|QTabWidget|Tabs|Notebook|Tabs|
 |Tab|✓|Tab|✓|✓|
 |MenuBar|QMenuBar|-|-|-|
 |Menu|QMenu|-|-|-|
 |MenuAction|QAction|-|-|-|
 |MdiArea|QMdiArea|-|-|-|
 |MdiSubWindow|QMdiSubWindow|-|-|-|
 |Splitter|QSplitter|-|-|-|
+|Modal|✓(QWidget)|-|-|-|
 |(Wrapper)|`QtWrapper`|-|-|-|
 
+# Imperative Dialogs
+|Generic|PySide6|flet|tkinter|textual|
+|-------|-------|----|-------|-------|
+|OpenDirectory|QFileDialog.getExistingDirectory|-|-|-|
+|OpenFile|QFileDialog.getOpenFileName|-|-|-|
+|OpenFiles|QFileDialog.getOpenFileNames|-|-|-|
+|SaveFile|QFileDialog.getSaveFileName|-|-|-|
+|Information|QMessageBox|-|-|-|
+|Warning|QMessageBox|-|-|-|
+|Critical|QMessageBox|-|-|-|
+|Confirm|QMessageBox|-|-|-|
+|Prompt|QInputDialog|-|-|-|
+
 ## Interfaces
 * Button(text)
     * .click(callback, *cb_args, **cb_kwargs)
 * Label(text)
     * .click(callback, *cb_args, **cb_kwargs)
 * TextField(binding)
 * ProgressBar(progress `0-1`)
@@ -241,14 +255,20 @@
 # reloadium: after_reload
 def after_reload(actions):
     PUIView.reload()
 ```
 
 
 # TODO
+* [ISSUE] empty virtual node
+* [ISSUE] textual layout sizing (cookbook scroll example)
+* [ISSUE] flet layout sizing (cookbook scroll example)
+* nested state trigger
+    * set state in PUIView __init__
+    * set state in setup() ?
 * Tabs(`tabposition`)
 * Lazy List
 * StateObject decorator
 * UI Flow
     * Navigation Stack
     * View Router
     * Model Window/Dialog
```

### Comparing `QPUIQ-0.2.4/QPUIQ.egg-info/SOURCES.txt` & `QPUIQ-0.2.5/QPUIQ.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -12,18 +12,20 @@
 PUI/PySide6/__init__.py
 PUI/PySide6/application.py
 PUI/PySide6/base.py
 PUI/PySide6/button.py
 PUI/PySide6/canvas.py
 PUI/PySide6/checkbox.py
 PUI/PySide6/combobox.py
+PUI/PySide6/dialog.py
 PUI/PySide6/label.py
 PUI/PySide6/layout.py
 PUI/PySide6/mdi.py
 PUI/PySide6/menu.py
+PUI/PySide6/modal.py
 PUI/PySide6/progressbar.py
 PUI/PySide6/radiobutton.py
 PUI/PySide6/scroll.py
 PUI/PySide6/splitter.py
 PUI/PySide6/tab.py
 PUI/PySide6/text.py
 PUI/PySide6/textfield.py
```

### Comparing `QPUIQ-0.2.4/README.md` & `QPUIQ-0.2.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -169,15 +169,15 @@
 ## Lower Priority
 * tkinter
     * or https://github.com/rdbende/Sun-Valley-ttk-theme
 * flet
 * textual (Text Mode)
     * no canvas
 
-# Components
+# Declarative Components
 |Generic|PySide6|flet|tkinter|textual|
 |-------|-------|----|-------|-------|
 |Application|QApplication|Page|Tk|App|
 |Window|QMainWindow|✓(Single)|Toplevel|✓(Single)|
 |HBox|QHBoxLayout|Row|Frame(grid)|Horizontal|
 |VBox|QVBoxLayout|Column|Frame(grid)|Vertical|
 |Spacer|QSpacerItem|✓|✓|✓|
@@ -187,27 +187,41 @@
 |RadioButton|QRadioButton|Radio|Radiobutton|RadioButton|
 |Canvas|✓(QWidget)|Canvas|Canvas|-|
 |TextField|QLineEdit|TextField|Entry|Input|
 |ProgressBar|QProgressBar|ProgressBar|Progressbar|ProgressBar|
 |Scroll|QScrollArea|✓|✓|ScrollableContainer|
 |Text|QLabel|Text|Label|Text|
 |Html|QLabel|⚠ Text|⚠ Label|⚠ Text|
-|MarkDown|QLabel|Markdown|⚠ Label|⚠ Text|
+|MarkDown|QLabel|Markdown|⚠ Label|Markdown|
 |Combobox|QComboBox|-|-|-|
 |ComboboxItem|✓|-|-|-|
 |Tabs|QTabWidget|Tabs|Notebook|Tabs|
 |Tab|✓|Tab|✓|✓|
 |MenuBar|QMenuBar|-|-|-|
 |Menu|QMenu|-|-|-|
 |MenuAction|QAction|-|-|-|
 |MdiArea|QMdiArea|-|-|-|
 |MdiSubWindow|QMdiSubWindow|-|-|-|
 |Splitter|QSplitter|-|-|-|
+|Modal|✓(QWidget)|-|-|-|
 |(Wrapper)|`QtWrapper`|-|-|-|
 
+# Imperative Dialogs
+|Generic|PySide6|flet|tkinter|textual|
+|-------|-------|----|-------|-------|
+|OpenDirectory|QFileDialog.getExistingDirectory|-|-|-|
+|OpenFile|QFileDialog.getOpenFileName|-|-|-|
+|OpenFiles|QFileDialog.getOpenFileNames|-|-|-|
+|SaveFile|QFileDialog.getSaveFileName|-|-|-|
+|Information|QMessageBox|-|-|-|
+|Warning|QMessageBox|-|-|-|
+|Critical|QMessageBox|-|-|-|
+|Confirm|QMessageBox|-|-|-|
+|Prompt|QInputDialog|-|-|-|
+
 ## Interfaces
 * Button(text)
     * .click(callback, *cb_args, **cb_kwargs)
 * Label(text)
     * .click(callback, *cb_args, **cb_kwargs)
 * TextField(binding)
 * ProgressBar(progress `0-1`)
@@ -231,14 +245,20 @@
 # reloadium: after_reload
 def after_reload(actions):
     PUIView.reload()
 ```
 
 
 # TODO
+* [ISSUE] empty virtual node
+* [ISSUE] textual layout sizing (cookbook scroll example)
+* [ISSUE] flet layout sizing (cookbook scroll example)
+* nested state trigger
+    * set state in PUIView __init__
+    * set state in setup() ?
 * Tabs(`tabposition`)
 * Lazy List
 * StateObject decorator
 * UI Flow
     * Navigation Stack
     * View Router
     * Model Window/Dialog
```

### Comparing `QPUIQ-0.2.4/setup.py` & `QPUIQ-0.2.5/setup.py`

 * *Files identical despite different names*

