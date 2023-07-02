# Comparing `tmp/Rickrack-2.8.27.tar.gz` & `tmp/Rickrack-2.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Rickrack-2.8.27.tar", last modified: Sun Jul  2 04:39:56 2023, max compression
+gzip compressed data, was "dist\Rickrack-2.8.5.tar", last modified: Sat Jun  3 16:03:49 2023, max compression
```

## Comparing `Rickrack-2.8.27.tar` & `Rickrack-2.8.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 04:39:56.000000 Rickrack-2.8.27/
--rw-rw-rw-   0        0        0       30 2023-07-02 04:39:55.000000 Rickrack-2.8.27/MANIFEST.in
--rw-rw-rw-   0        0        0    30731 2023-07-02 04:39:56.000000 Rickrack-2.8.27/PKG-INFO
--rw-rw-rw-   0        0        0    26603 2023-07-02 04:39:55.000000 Rickrack-2.8.27/README.md
-drwxrwxrwx   0        0        0        0 2023-07-02 04:39:56.000000 Rickrack-2.8.27/rickrack/
--rw-rw-rw-   0        0        0    36393 2023-07-02 04:39:55.000000 Rickrack-2.8.27/rickrack/color.py
--rw-rw-rw-   0        0        0     9994 2023-04-07 06:01:22.000000 Rickrack-2.8.27/rickrack/result.py
--rw-rw-rw-   0        0        0    32828 2023-06-22 13:48:06.000000 Rickrack-2.8.27/rickrack/rickrack.py
--rw-rw-rw-   0        0        0      600 2023-01-09 01:58:26.000000 Rickrack-2.8.27/rickrack/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-02 04:39:56.000000 Rickrack-2.8.27/Rickrack.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-02 04:39:55.000000 Rickrack-2.8.27/Rickrack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      112 2023-07-02 04:39:55.000000 Rickrack-2.8.27/Rickrack.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0    30731 2023-07-02 04:39:55.000000 Rickrack-2.8.27/Rickrack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0        6 2023-07-02 04:39:55.000000 Rickrack-2.8.27/Rickrack.egg-info/requires.txt
--rw-rw-rw-   0        0        0      303 2023-07-02 04:39:55.000000 Rickrack-2.8.27/Rickrack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2023-07-02 04:39:55.000000 Rickrack-2.8.27/Rickrack.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-02 04:39:56.000000 Rickrack-2.8.27/setup.cfg
--rw-rw-rw-   0        0        0     2070 2023-07-02 04:39:55.000000 Rickrack-2.8.27/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 16:03:49.000000 Rickrack-2.8.5/
+-rw-rw-rw-   0        0        0       30 2023-06-03 16:03:48.000000 Rickrack-2.8.5/MANIFEST.in
+-rw-rw-rw-   0        0        0    30704 2023-06-03 16:03:49.000000 Rickrack-2.8.5/PKG-INFO
+-rw-rw-rw-   0        0        0    26627 2023-06-03 16:03:48.000000 Rickrack-2.8.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-03 16:03:49.000000 Rickrack-2.8.5/rickrack/
+-rw-rw-rw-   0        0        0    35477 2023-06-03 16:03:48.000000 Rickrack-2.8.5/rickrack/color.py
+-rw-rw-rw-   0        0        0     9994 2023-04-07 06:01:22.000000 Rickrack-2.8.5/rickrack/result.py
+-rw-rw-rw-   0        0        0    32826 2023-06-03 14:03:45.000000 Rickrack-2.8.5/rickrack/rickrack.py
+-rw-rw-rw-   0        0        0      600 2023-01-09 01:58:26.000000 Rickrack-2.8.5/rickrack/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-03 16:03:49.000000 Rickrack-2.8.5/Rickrack.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-06-03 16:03:49.000000 Rickrack-2.8.5/Rickrack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      112 2023-06-03 16:03:49.000000 Rickrack-2.8.5/Rickrack.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0    30704 2023-06-03 16:03:49.000000 Rickrack-2.8.5/Rickrack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0        6 2023-06-03 16:03:49.000000 Rickrack-2.8.5/Rickrack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      303 2023-06-03 16:03:49.000000 Rickrack-2.8.5/Rickrack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        9 2023-06-03 16:03:49.000000 Rickrack-2.8.5/Rickrack.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-03 16:03:49.000000 Rickrack-2.8.5/setup.cfg
+-rw-rw-rw-   0        0        0     2075 2023-06-03 16:03:48.000000 Rickrack-2.8.5/setup.py
```

### Comparing `Rickrack-2.8.27/PKG-INFO` & `Rickrack-2.8.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: Rickrack
-Version: 2.8.27
+Version: 2.8.5
 Summary: Generate harmonious colors freely.
-Home-page: https://eigenmiao.com/rickrack/
+Home-page: https://eigenmiao.github.io/rickrack/
 Author: Eigenmiao
 Author-email: eigenmiao@outlook.com
 License: UNKNOWN
 Description: <div align="center">
         <img width="100%" align="center" src="https://raw.githubusercontent.com/eigenmiao/Rickrack/master/src/main/icons/logo_long.png" alt="Rickrack">
         <br/><br/>
         Rickrack<br/>焰火十二卷<br/> ----- ----- ----- ----- ----- ----- ----- ----- <br/>
@@ -17,26 +17,22 @@
         </div>
         
         # Rickrack
         In the age of digital creativity, the color palette has become an indispensable tool for designers. A good color palette can make a design more attractive and coordinated. Rickrack is designed for you if you are looking for an excellent color palette software! Rickrack has various color mixing functions and is suitable for various scenes. Rickrack is easy to use, and more importantly, it's completely free without networking or registration required.
         
         Rickrack (**R**e**a**l-t**i**me **C**olor **K**it) is a free and user-friendly color editor. It is designed to generate a set of harmonious colors from the color wheel or other places. You can share these colors with your friends, or apply them into your creative works. What’s more, you can export them into individual files and import them into other softwares such as Adobe Photoshop, GIMP, Krita, Pencil 2D and Clip Studio Paint. Rickrack can run normally on operating systems such as Windows, Linux, and macOS.
         
-        [:rocket: v2.8.27 Update Notes](https://github.com/eigenmiao/Rickrack/releases/tag/v2.8.27)
-        
         [:house: Rickrack](https://eigenmiao.com/rickrack)
         
         [:arrow_down: Translations of the Introduction in Other Languages :arrow_down:](#introduction-translations)
         
         # 焰火十二卷
         在数字创意的时代，调色板成为了设计师不可或缺的工具。一个好的调色板可以让设计更加有吸引力和协调性。如果你正在寻找一款优秀的调色板软件，那就试试焰火十二卷吧！焰火十二卷具有多种配色功能，适用于多种场景。焰火十二卷简单易上手，更重要的是，它完全免费，无需联网或注册。
         
-        焰火十二卷（实时色彩工具箱）是一款免费且实用的色彩编辑器。它可以帮助你从色轮或者其他地方生成一组和谐的色彩。你可以将这些色彩分享给其他人，或者应用到你自己的创作当中。此外，你也可以将色彩组或者色库导出为单独的色彩文档并导入其他软件中（如 Adobe Photoshop、GIMP、Krita、Pencil 2D 以及优动漫 Paint 等）。焰火十二卷可以在 Windows、Linux、macOS 等操作系统上正常运行。
-        
-        [:rocket: v2.8.27 更新说明](https://github.com/eigenmiao/Rickrack/releases/tag/v2.8.27)
+        焰火十二卷（实时色彩工具箱）是一款免费且实用的色彩编辑器。它可以帮助你从色轮或者其他地方生成一组和谐的色彩。你可以将这些色彩分享给其他人，或者应用到你自己的创作当中。此外，你也可以将色彩组或者色彩仓库导出为单独的色彩文档并导入其他软件中（如 Adobe Photoshop、GIMP、Krita、Pencil 2D 以及优动漫 Paint 等）。焰火十二卷可以在 Windows、Linux、macOS 等操作系统上正常运行。
         
         [:house: 焰火十二卷](https://eigenmiao.com/yanhuo)
         
         [:arrow_down: 简介的其他语言翻译 :arrow_down:](#introduction-translations)
         
         # Table of Content
         * [Introduction Translations](#introduction-translations)
@@ -199,24 +195,24 @@
         * [:hugs: 本征喵函数 @ 爱发电](https://afdian.net/a/eigenmiao)
         * [:hugs: Eigenmiao @ Ko-fi](https://ko-fi.com/eigenmiao)
         
         <div align="right"><a href="#table-of-content">:arrow_up: Back to TOC  :arrow_up:</a></div>
         
         # Installation
         ## Current Release
-        The latest preview version is [v2.8.27](https://github.com/eigenmiao/Rickrack/releases/tag/v2.8.27).
+        The latest preview version is [v2.8.5](https://github.com/eigenmiao/Rickrack/releases/tag/v2.8.5).
         
         ## Install Software
         ### Recommend: Install on Windows 10 or 11 via WinGet tool
         ```
         winget install rickrack
         ```
         
         ## Install on other platforms
-        Download Software from [Github](https://github.com/eigenmiao/Rickrack/releases/tag/v2.8.27) or [Sourceforge](https://sourceforge.net/projects/rickrack/files/v2.8.27/). The installation steps are presented in [tutorials](https://eigenmiao.com/2021/12/12/rickrack-tutorial-en-v2.3.4/#Installation).
+        Download Software from [Github](https://github.com/eigenmiao/Rickrack/releases/tag/v2.8.5) or [Sourceforge](https://sourceforge.net/projects/rickrack/files/v2.8.5/). The installation steps are presented in [tutorials](https://eigenmiao.com/2021/12/12/rickrack-tutorial-en-v2.3.4/#Installation).
         
         Here is a [video tutorial](https://www.bilibili.com/video/BV17r4y1L7R6/).
         
         ## Install Module
         Install the latest [Rickrack](https://pypi.org/project/Rickrack/) from PyPI!
         
         ```Bash
@@ -229,24 +225,24 @@
         
         <div align="right"><a href="#table-of-content">:arrow_up: Back to TOC  :arrow_up:</a></div>
         
         # Usage
         ## How to Use the Software
         Visit https://eigenmiao.com/rickrack/ for tutorials. Just feel free to click anywhere in the interface!
         
-        Here is a [video tutorial](https://www.bilibili.com/video/BV1BM411L75t/).
+        Here is a [video tutorial](https://www.bilibili.com/video/BV17L4y1A7P9/).
         
-        Here is a [demo](https://eigenmiao.com/2023/01/29/color-palette-generator-rickrack-en/).
+        Here is a [demo](https://eigenmiao.com/2023/01/29/rickrack-alternative-to-adobe-color-en/).
         
         ## How to Use the Module
         Include Rickrack in other Python scripts, programs and softwares!
         
         Here is a [video tutorial](https://www.bilibili.com/video/BV1VD4y157tX/).
         
-        Here is a [demo](demo/03_plot_scripts).
+        Here is a [demo](demo/).
         
         ```Python
         # Use Rickrack module in code.
         # This code fragment could be reused.
         
         from rickrack import Rickrack
         
@@ -258,14 +254,18 @@
         dp_argv = dict()
         dp_argv["help"] = True
         
         # Run and see the full contents and examples.
         rr.run(dp_argv=dp_argv, dp_proj=dp_proj)
         ```
         
+        ## Notice
+        * Please read the documents and tutorials when you encounter any difficulties.
+        * The socket server is designed for obtaining colors from the Rickrack software in real-time. By default, this server is disabled and can only be started from the command line.
+        
         <div align="right"><a href="#table-of-content">:arrow_up: Back to TOC  :arrow_up:</a></div>
         
         # Development
         ## Install Requirement
         * Python 3.6
         * Git version control system
         * Additional modules listed in requirements folder
@@ -274,22 +274,19 @@
         ```bash
         # Download the Rickrack source code.
         git clone https://github.com/eigenmiao/Rickrack.git
         
         # Change into the directory.
         cd Rickrack
         
-        # Install the Rickrack starter.
-        pip install rickrack
-        
-        # Display the help information.
-        rickrack -h
-        
         # Run Rickrack.
-        rickrack
+        python src/main/python/main.py
+        
+        # Generate the installer for Rickrack.
+        fbs freeze && fbs installer
         ```
         
         ## How to Build the Module
         ```bash
         # Download the Rickrack source code.
         git clone https://github.com/eigenmiao/Rickrack.git
         
@@ -303,21 +300,24 @@
         <div align="right"><a href="#table-of-content">:arrow_up: Back to TOC  :arrow_up:</a></div>
         
         # Copyright
         Copyright (c) 2019-2023 [Eigenmiao](mailto:eigenmiao@outlook.com). All Rights Reserved.
         
         <div align="right"><a href="#table-of-content">:arrow_up: Back to TOC  :arrow_up:</a></div>
         
+        # Contributing
+        This project welcomes contributions of all types. Recommending Rickrack to people you know, writing reviews for Rickrack on websites, help spec'ing, design, documentation, finding bugs, etc. can all help the project grow better.
+        
         # License
         ## License for Rickrack
         Rickrack is a free software, which is distributed in the hope that it will be useful, but without any warranty. You can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation. See the [GNU General Public License 3.0 (GPL 3.0)](https://www.gnu.org/licenses/) for more details.
         
         All images, documents and translations in Rickrack [code repository](https://github.com/eigenmiao/Rickrack) are licensed under [Creative Commons Attribution-NonCommercial-ShareAlike License 4.0 (CC BY-NC-SA 4.0)](https://creativecommons.org/licenses/by-nc-sa/4.0/) unless stating additionally.
         
-        Rickrack default uses [LXGW WenKai](https://github.com/lxgw/LxgwWenKai) font for interface display, which is an open-source Chinese font derived from Fontworks' Klee One. This font is open-sourced under [SIL Open Font License 1.1](http://scripts.sil.org/OFL).
+        Rickrack default uses [Noto Serif](https://fonts.google.com/specimen/Noto+Serif) ([SC](https://fonts.google.com/specimen/Noto+Serif+SC)) fonts and [Noto Sans](https://fonts.google.com/specimen/Noto+Sans) ([SC](https://fonts.google.com/specimen/Noto+Sans+SC)) fonts for interface display, which are designed by Google and published in website [Google Fonts](https://fonts.google.com/). These fonts are open-sourced under [Apache 2.0](http://www.apache.org/licenses/) and [SIL Open Font License 1.1](http://scripts.sil.org/OFL), respectively.
         
         ## License for Required Packages
         | Package        | Version  | License          |
         |----------------|----------|------------------|
         | altgraph       | 0.17.2   | MIT              |
         | fbs            | 0.8.9    | GPLv3 or Later   |
         | future         | 0.18.2   | MIT              |
@@ -335,43 +335,36 @@
         | ricore         | 0.0.0    | Not Open-sourced |
         | setuptools     | 40.6.2   | MIT              |
         | swatch         | 0.4.0    | MIT              |
         
         <div align="right"><a href="#table-of-content">:arrow_up: Back to TOC  :arrow_up:</a></div>
         
         # More Information
-        * Documentation: https://eigenmiao.com/2021/12/12/rickrack-tutorial-en-v2.3.4/ .
-        * The installation package can be unzipped and run directly. This method does not require administrator privileges and can solve some installation failure problems.
-        * The socket server is designed for obtaining colors from the Rickrack software in real-time. By default, this server is disabled and can only be started from the command line.
         * Rickrack is written in [Python](https://www.python.org/), constructed based on [PyQt5](https://www.qt.io/qt-for-python) and packed up by [fbs (free edition)](https://build-system.fman.io/).
         * The code repository of Rickrack is deposited on [Github](https://github.com/eigenmiao/Rickrack) and [Gitee](https://gitee.com/eigenmiao/Rickrack).
         * The localization (l10n) and internationalization (i18n) of Rickrack is based on [Google Translate](https://translate.google.cn/) and [Microsoft Translator](https://cn.bing.com/translator), deployed on [POEditor](https://poeditor.com/join/project?hash=kBeQjfxCES).
         * The cover image uses images from [Pixabay, which is created by martynaszulist](https://pixabay.com/zh/photos/pattern-the-palette-web-1508277/).
         * In some demo animations, [images of Ghibli](https://www.ghibli.jp/info/013409/) were used.
-        
-        <div align="right"><a href="#table-of-content">:arrow_up: Back to TOC  :arrow_up:</a></div>
-        
-        # Contributing
-        This project welcomes contributions of all types. If you want to contribute code (new features, or bug fixes) to this project, please contact me first. Thanks.
+        * The interface display in demo animations uses the [LXGWWenKai font](https://lxgw.github.io/2021/01/28/Klee-Simpchin/).
         
         <div align="right"><a href="#table-of-content">:arrow_up: Back to TOC  :arrow_up:</a></div>
         
         # Acknowledgment
-        ## Reviews
+        ## Publicity & Promotion
         <table>
           <tbody>
             <tr>
             <td align="center" valign="top" width="20%"><a href="https://www.youtube.com/watch?v=OUnktTCtv3E"><img src="https://yt3.googleusercontent.com/ytc/AGIKgqPSY98ka46AxjcUBDDntl1NHA8lL4PFMZt6g75TFA=s176-c-k-c0x00ffffff-no-rj" width="90px;"/><br /><sub><b>TJ&nbsp;FREE@Youtube</b></sub></a></td>
             <td align="center" valign="top" width="20%"><a href="https://www.softpedia.com/get/Multimedia/Graphic/Graphic-Others/RickRack.shtml"><img src="https://cdnssl.softpedia.com/_img/editors/Robert%20Condorache.jpg?v=2020" width="90px;"/><br /><sub><b>Robert&nbsp;Condorache@Softpedia</b></sub></a></td>
             <td align="center" valign="top" width="20%"><a href="https://sspai.com/u/eigenmiao/updates"><img src="https://cdn.sspai.com/2023/01/14/eab0a38256bc3a045f8d5bf76dd30072.png?imageMogr2/auto-orient/quality/95/thumbnail/!200x200r/gravity/Center/crop/200x200/interlace/1" width="90px;"/><br /><sub><b>本征喵函数@少数派</b></sub></a></td>
             </tr>
           </tbody>
         </table>
         
-        ## Translators
+        ## l10n & i18n
         <table>
           <tbody>
             <tr>
             <td align="center" valign="top" width="20%"><a href="https://poeditor.com/join/project?hash=kBeQjfxCES"><img src="https://avatars.githubusercontent.com/u/59333735?v=4" width="90px;"/><br /><sub><b>Eigenmiao@POEditor</b></sub></a></td>
             </tr>
           </tbody>
         </table>
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
-Metadata-Version: 2.1 Name: Rickrack Version: 2.8.27 Summary: Generate
-harmonious colors freely. Home-page: https://eigenmiao.com/rickrack/ Author:
-Eigenmiao Author-email: eigenmiao@outlook.com License: UNKNOWN Description:
+Metadata-Version: 2.1 Name: Rickrack Version: 2.8.5 Summary: Generate
+harmonious colors freely. Home-page: https://eigenmiao.github.io/rickrack/
+Author: Eigenmiao Author-email: eigenmiao@outlook.com License: UNKNOWN
+Description:
                                   [Rickrack]
 
                                    Rickrack
                                 ç°ç«åäºå·
                ----- ----- ----- ----- ----- ----- ----- -----
                       Generate Harmonious Colors Freely.
                       èªç±èªå¨çæåè°è²å½©ã
@@ -22,62 +23,59 @@
 importantly, it's completely free without networking or registration required.
 Rickrack (**R**e**a**l-t**i**me **C**olor **K**it) is a free and user-friendly
 color editor. It is designed to generate a set of harmonious colors from the
 color wheel or other places. You can share these colors with your friends, or
 apply them into your creative works. Whatâs more, you can export them into
 individual files and import them into other softwares such as Adobe Photoshop,
 GIMP, Krita, Pencil 2D and Clip Studio Paint. Rickrack can run normally on
-operating systems such as Windows, Linux, and macOS. [:rocket: v2.8.27 Update
-Notes](https://github.com/eigenmiao/Rickrack/releases/tag/v2.8.27) [:house:
-Rickrack](https://eigenmiao.com/rickrack) [:arrow_down: Translations of the
-Introduction in Other Languages :arrow_down:](#introduction-translations) #
-ç°ç«åäºå·
+operating systems such as Windows, Linux, and macOS. [:house: Rickrack](https:/
+/eigenmiao.com/rickrack) [:arrow_down: Translations of the Introduction in
+Other Languages :arrow_down:](#introduction-translations) # ç°ç«åäºå·
 å¨æ°å­åæçæ¶ä»£ï¼è°è²æ¿æä¸ºäºè®¾è®¡å¸ä¸å¯æç¼ºçå·¥å·ãä¸ä¸ªå¥½çè°è²æ¿å¯ä»¥è®©è®¾è®¡æ´å æå¸å¼åååè°æ§ãå¦æä½ æ­£å¨å¯»æ¾ä¸æ¬¾ä¼ç§çè°è²æ¿è½¯ä»¶ï¼é£å°±è¯è¯ç°ç«åäºå·å§ï¼ç°ç«åäºå·å·æå¤ç§éè²åè½ï¼éç¨äºå¤ç§åºæ¯ãç°ç«åäºå·ç®åæä¸æï¼æ´éè¦çæ¯ï¼å®å®å¨åè´¹ï¼æ éèç½ææ³¨åã
-ç°ç«åäºå·ï¼å®æ¶è²å½©å·¥å·ç®±ï¼æ¯ä¸æ¬¾åè´¹ä¸å®ç¨çè²å½©ç¼è¾å¨ãå®å¯ä»¥å¸®å©ä½ ä»è²è½®æèå¶ä»å°æ¹çæä¸ç»åè°çè²å½©ãä½ å¯ä»¥å°è¿äºè²å½©åäº«ç»å¶ä»äººï¼æèåºç¨å°ä½ èªå·±çåä½å½ä¸­ãæ­¤å¤ï¼ä½ ä¹å¯ä»¥å°è²å½©ç»æèè²åºå¯¼åºä¸ºåç¬çè²å½©ææ¡£å¹¶å¯¼å¥å¶ä»è½¯ä»¶ä¸­ï¼å¦
+ç°ç«åäºå·ï¼å®æ¶è²å½©å·¥å·ç®±ï¼æ¯ä¸æ¬¾åè´¹ä¸å®ç¨çè²å½©ç¼è¾å¨ãå®å¯ä»¥å¸®å©ä½ ä»è²è½®æèå¶ä»å°æ¹çæä¸ç»åè°çè²å½©ãä½ å¯ä»¥å°è¿äºè²å½©åäº«ç»å¶ä»äººï¼æèåºç¨å°ä½ èªå·±çåä½å½ä¸­ãæ­¤å¤ï¼ä½ ä¹å¯ä»¥å°è²å½©ç»æèè²å½©ä»åºå¯¼åºä¸ºåç¬çè²å½©ææ¡£å¹¶å¯¼å¥å¶ä»è½¯ä»¶ä¸­ï¼å¦
 Adobe PhotoshopãGIMPãKritaãPencil 2D ä»¥åä¼å¨æ¼« Paint
 ç­ï¼ãç°ç«åäºå·å¯ä»¥å¨ WindowsãLinuxãmacOS
-ç­æä½ç³»ç»ä¸æ­£å¸¸è¿è¡ã [:rocket: v2.8.27 æ´æ°è¯´æ](https://
-github.com/eigenmiao/Rickrack/releases/tag/v2.8.27) [:house: ç°ç«åäºå·]
-(https://eigenmiao.com/yanhuo) [:arrow_down: ç®ä»çå¶ä»è¯­è¨ç¿»è¯ :
-arrow_down:](#introduction-translations) # Table of Content * [Introduction
-Translations](#introduction-translations) * [Features](#features) * [Demo]
-(#demo) * [Basic Functions](#basic-functions) * [Reference Colors](#reference-
-colors) * [Color Palettes](#color-palettes) * [Export and Import Colors]
-(#export-and-import-colors) * [Languages and Settings](#languages-and-settings)
-* [Reviews about Rickrack](#reviews-about-rickrack) * [Information]
-(#information) * [Website](#website) * [Repository](#repository) * [Author]
-(#author) * [Support](#support) * [Installation](#installation) * [Current
-Release](#current-release) * [Download Software](#download-software) * [Install
-Software](#install-software) * [Install Module](#install-module) * [Usage]
-(#usage) * [How to Use the Software](#how-to-use-the-software) * [How to Use
-the Module](#how-to-use-the-module) * [Development](#development) * [Install
-Requirement](#install-requirement) * [How to Build the Software](#how-to-build-
-the-software) * [How to Build the Module](#how-to-build-the-module) *
-[Copyright](#copyright) * [License](#license) * [License for Rickrack]
-(#license-for-rickrack) * [License for Required Packages](#license-for-
-required-packages) * [More Information](#more-information) * [Acknowledgment]
-(#acknowledgment) # Introduction Translations ## Rickrack (Esperanto) En la
-epoko de cifereca kreemo, la kolora paletro fariÄis nemalhavebla ilo por
-dezajnistoj. Bona kolora paletro povas fari dezajnon pli alloga kaj
-kunordigita. Rickrack estas desegnita por vi, se vi serÄas bonegan programaron
-de kolora paletro! Rickrack havas diversajn kolorajn miksajn funkciojn kaj
-taÅ­gas por diversaj scenoj. Rickrack estas facile uzebla, kaj pli grave, Äi
-estas tute senpaga sen interkonektado aÅ­ registriÄo necesa. Rickrack estas
-senpaga kaj amika kolorredaktilo. Äi estas desegnita por generi aron da
-harmoniaj koloroj de la kolorrado aÅ­ aliaj lokoj. Vi povas dividi Äi tiujn
-kolorojn kun viaj amikoj, aÅ­ apliki ilin en viajn kreajn verkojn. Krome, vi
-povas eksporti ilin en individuajn dosierojn kaj importi ilin en aliajn
-programojn kiel Adobe Photoshop, GIMP, Krita, Pencil 2D kaj Clip Studio Paint.
-Rickrack povas funkcii normale per operaciumoj kiel Vindozo, Linukso kaj macOS.
-(Tradukoj supre baziÄas sur Google Translate.) [:house: Rickrack](https://
-eigenmiao.com/yanhuo/eo.html) ## Rickrack (Ð ÑÑÑÐºÐ¸Ð¹) Ð Ð²ÐµÐº
-ÑÐ¸ÑÑÐ¾Ð²Ð¾Ð³Ð¾ ÑÐ²Ð¾ÑÑÐµÑÑÐ²Ð° ÑÐ²ÐµÑÐ¾Ð²Ð°Ñ Ð¿Ð°Ð»Ð¸ÑÑÐ°
-ÑÑÐ°Ð»Ð° Ð½ÐµÐ·Ð°Ð¼ÐµÐ½Ð¸Ð¼ÑÐ¼ Ð¸Ð½ÑÑÑÑÐ¼ÐµÐ½ÑÐ¾Ð¼ Ð´Ð»Ñ
-Ð´Ð¸Ð·Ð°Ð¹Ð½ÐµÑÐ¾Ð². Ð¥Ð¾ÑÐ¾ÑÐ°Ñ ÑÐ²ÐµÑÐ¾Ð²Ð°Ñ Ð¿Ð°Ð»Ð¸ÑÑÐ° Ð¼Ð¾Ð¶ÐµÑ
-ÑÐ´ÐµÐ»Ð°ÑÑ Ð´Ð¸Ð·Ð°Ð¹Ð½ Ð±Ð¾Ð»ÐµÐµ Ð¿ÑÐ¸Ð²Ð»ÐµÐºÐ°ÑÐµÐ»ÑÐ½ÑÐ¼ Ð¸
+ç­æä½ç³»ç»ä¸æ­£å¸¸è¿è¡ã [:house: ç°ç«åäºå·](https://
+eigenmiao.com/yanhuo) [:arrow_down: ç®ä»çå¶ä»è¯­è¨ç¿»è¯ :arrow_down:]
+(#introduction-translations) # Table of Content * [Introduction Translations]
+(#introduction-translations) * [Features](#features) * [Demo](#demo) * [Basic
+Functions](#basic-functions) * [Reference Colors](#reference-colors) * [Color
+Palettes](#color-palettes) * [Export and Import Colors](#export-and-import-
+colors) * [Languages and Settings](#languages-and-settings) * [Reviews about
+Rickrack](#reviews-about-rickrack) * [Information](#information) * [Website]
+(#website) * [Repository](#repository) * [Author](#author) * [Support]
+(#support) * [Installation](#installation) * [Current Release](#current-
+release) * [Download Software](#download-software) * [Install Software]
+(#install-software) * [Install Module](#install-module) * [Usage](#usage) *
+[How to Use the Software](#how-to-use-the-software) * [How to Use the Module]
+(#how-to-use-the-module) * [Development](#development) * [Install Requirement]
+(#install-requirement) * [How to Build the Software](#how-to-build-the-
+software) * [How to Build the Module](#how-to-build-the-module) * [Copyright]
+(#copyright) * [License](#license) * [License for Rickrack](#license-for-
+rickrack) * [License for Required Packages](#license-for-required-packages) *
+[More Information](#more-information) * [Acknowledgment](#acknowledgment) #
+Introduction Translations ## Rickrack (Esperanto) En la epoko de cifereca
+kreemo, la kolora paletro fariÄis nemalhavebla ilo por dezajnistoj. Bona
+kolora paletro povas fari dezajnon pli alloga kaj kunordigita. Rickrack estas
+desegnita por vi, se vi serÄas bonegan programaron de kolora paletro! Rickrack
+havas diversajn kolorajn miksajn funkciojn kaj taÅ­gas por diversaj scenoj.
+Rickrack estas facile uzebla, kaj pli grave, Äi estas tute senpaga sen
+interkonektado aÅ­ registriÄo necesa. Rickrack estas senpaga kaj amika
+kolorredaktilo. Äi estas desegnita por generi aron da harmoniaj koloroj de la
+kolorrado aÅ­ aliaj lokoj. Vi povas dividi Äi tiujn kolorojn kun viaj amikoj,
+aÅ­ apliki ilin en viajn kreajn verkojn. Krome, vi povas eksporti ilin en
+individuajn dosierojn kaj importi ilin en aliajn programojn kiel Adobe
+Photoshop, GIMP, Krita, Pencil 2D kaj Clip Studio Paint. Rickrack povas funkcii
+normale per operaciumoj kiel Vindozo, Linukso kaj macOS. (Tradukoj supre
+baziÄas sur Google Translate.) [:house: Rickrack](https://eigenmiao.com/
+yanhuo/eo.html) ## Rickrack (Ð ÑÑÑÐºÐ¸Ð¹) Ð Ð²ÐµÐº ÑÐ¸ÑÑÐ¾Ð²Ð¾Ð³Ð¾
+ÑÐ²Ð¾ÑÑÐµÑÑÐ²Ð° ÑÐ²ÐµÑÐ¾Ð²Ð°Ñ Ð¿Ð°Ð»Ð¸ÑÑÐ° ÑÑÐ°Ð»Ð°
+Ð½ÐµÐ·Ð°Ð¼ÐµÐ½Ð¸Ð¼ÑÐ¼ Ð¸Ð½ÑÑÑÑÐ¼ÐµÐ½ÑÐ¾Ð¼ Ð´Ð»Ñ Ð´Ð¸Ð·Ð°Ð¹Ð½ÐµÑÐ¾Ð².
+Ð¥Ð¾ÑÐ¾ÑÐ°Ñ ÑÐ²ÐµÑÐ¾Ð²Ð°Ñ Ð¿Ð°Ð»Ð¸ÑÑÐ° Ð¼Ð¾Ð¶ÐµÑ ÑÐ´ÐµÐ»Ð°ÑÑ
+Ð´Ð¸Ð·Ð°Ð¹Ð½ Ð±Ð¾Ð»ÐµÐµ Ð¿ÑÐ¸Ð²Ð»ÐµÐºÐ°ÑÐµÐ»ÑÐ½ÑÐ¼ Ð¸
 Ð³Ð°ÑÐ¼Ð¾Ð½Ð¸ÑÐ½ÑÐ¼. Rickrack ÑÐ°Ð·ÑÐ°Ð±Ð¾ÑÐ°Ð½ Ð´Ð»Ñ Ð²Ð°Ñ, ÐµÑÐ»Ð¸
 Ð²Ñ Ð¸ÑÐµÑÐµ Ð¾ÑÐ»Ð¸ÑÐ½Ð¾Ðµ Ð¿ÑÐ¾Ð³ÑÐ°Ð¼Ð¼Ð½Ð¾Ðµ Ð¾Ð±ÐµÑÐ¿ÐµÑÐµÐ½Ð¸Ðµ
 Ð´Ð»Ñ ÑÐ²ÐµÑÐ¾Ð²Ð¾Ð¹ Ð¿Ð°Ð»Ð¸ÑÑÑ! Rickrack Ð¸Ð¼ÐµÐµÑ ÑÐ°Ð·Ð»Ð¸ÑÐ½ÑÐµ
 ÑÑÐ½ÐºÑÐ¸Ð¸ ÑÐ¼ÐµÑÐ¸Ð²Ð°Ð½Ð¸Ñ ÑÐ²ÐµÑÐ¾Ð² Ð¸ Ð¿Ð¾Ð´ÑÐ¾Ð´Ð¸Ñ Ð´Ð»Ñ
 ÑÐ°Ð·Ð»Ð¸ÑÐ½ÑÑ ÑÑÐµÐ½. Rickrack Ð¿ÑÐ¾ÑÑ Ð² Ð¸ÑÐ¿Ð¾Ð»ÑÐ·Ð¾Ð²Ð°Ð½Ð¸Ð¸
 Ð¸, ÑÑÐ¾ Ð±Ð¾Ð»ÐµÐµ Ð²Ð°Ð¶Ð½Ð¾, ÑÐ¾Ð²ÐµÑÑÐµÐ½Ð½Ð¾ Ð±ÐµÑÐ¿Ð»Ð°ÑÐµÐ½, Ð½Ðµ
 ÑÑÐµÐ±ÑÐµÑ Ð¿Ð¾Ð´ÐºÐ»ÑÑÐµÐ½Ð¸Ñ Ðº ÑÐµÑÐ¸ Ð¸Ð»Ð¸
@@ -213,104 +211,107 @@
                                               :arrow_up:_Back_to_TOC_:arrow_up:
 # Information ## Website https://eigenmiao.com/rickrack ## Repository https://
 github.com/eigenmiao/Rickrack ## Author [Eigenmiao](mailto:
 eigenmiao@outlook.com) ## Support Support the continuous development of
 Rickrack! * [:hugs: æ¬å¾åµå½æ° @ ç±åçµ](https://afdian.net/a/
 eigenmiao) * [:hugs: Eigenmiao @ Ko-fi](https://ko-fi.com/eigenmiao)
                                               :arrow_up:_Back_to_TOC_:arrow_up:
-# Installation ## Current Release The latest preview version is [v2.8.27]
-(https://github.com/eigenmiao/Rickrack/releases/tag/v2.8.27). ## Install
-Software ### Recommend: Install on Windows 10 or 11 via WinGet tool ``` winget
-install rickrack ``` ## Install on other platforms Download Software from
-[Github](https://github.com/eigenmiao/Rickrack/releases/tag/v2.8.27) or
-[Sourceforge](https://sourceforge.net/projects/rickrack/files/v2.8.27/). The
-installation steps are presented in [tutorials](https://eigenmiao.com/2021/12/
-12/rickrack-tutorial-en-v2.3.4/#Installation). Here is a [video tutorial]
-(https://www.bilibili.com/video/BV17r4y1L7R6/). ## Install Module Install the
-latest [Rickrack](https://pypi.org/project/Rickrack/) from PyPI! ```Bash #
-Install Rickrack. pip install Rickrack # Start the installed software. rickrack
--d "/PATH/TO/RICKRACK/SOFTWARE" ```
+# Installation ## Current Release The latest preview version is [v2.8.5](https:
+//github.com/eigenmiao/Rickrack/releases/tag/v2.8.5). ## Install Software ###
+Recommend: Install on Windows 10 or 11 via WinGet tool ``` winget install
+rickrack ``` ## Install on other platforms Download Software from [Github]
+(https://github.com/eigenmiao/Rickrack/releases/tag/v2.8.5) or [Sourceforge]
+(https://sourceforge.net/projects/rickrack/files/v2.8.5/). The installation
+steps are presented in [tutorials](https://eigenmiao.com/2021/12/12/rickrack-
+tutorial-en-v2.3.4/#Installation). Here is a [video tutorial](https://
+www.bilibili.com/video/BV17r4y1L7R6/). ## Install Module Install the latest
+[Rickrack](https://pypi.org/project/Rickrack/) from PyPI! ```Bash # Install
+Rickrack. pip install Rickrack # Start the installed software. rickrack -d "/
+PATH/TO/RICKRACK/SOFTWARE" ```
                                               :arrow_up:_Back_to_TOC_:arrow_up:
 # Usage ## How to Use the Software Visit https://eigenmiao.com/rickrack/ for
 tutorials. Just feel free to click anywhere in the interface! Here is a [video
-tutorial](https://www.bilibili.com/video/BV1BM411L75t/). Here is a [demo]
-(https://eigenmiao.com/2023/01/29/color-palette-generator-rickrack-en/). ## How
-to Use the Module Include Rickrack in other Python scripts, programs and
+tutorial](https://www.bilibili.com/video/BV17L4y1A7P9/). Here is a [demo]
+(https://eigenmiao.com/2023/01/29/rickrack-alternative-to-adobe-color-en/). ##
+How to Use the Module Include Rickrack in other Python scripts, programs and
 softwares! Here is a [video tutorial](https://www.bilibili.com/video/
-BV1VD4y157tX/). Here is a [demo](demo/03_plot_scripts). ```Python # Use
-Rickrack module in code. # This code fragment could be reused. from rickrack
-import Rickrack # Init Rickrack. rr = Rickrack() # Display the help
-information. dp_proj = "/PATH/TO/RICKRACK/PROJECT" dp_argv = dict() dp_argv
-["help"] = True # Run and see the full contents and examples. rr.run
-(dp_argv=dp_argv, dp_proj=dp_proj) ```
+BV1VD4y157tX/). Here is a [demo](demo/). ```Python # Use Rickrack module in
+code. # This code fragment could be reused. from rickrack import Rickrack #
+Init Rickrack. rr = Rickrack() # Display the help information. dp_proj = "/
+PATH/TO/RICKRACK/PROJECT" dp_argv = dict() dp_argv["help"] = True # Run and see
+the full contents and examples. rr.run(dp_argv=dp_argv, dp_proj=dp_proj) ``` ##
+Notice * Please read the documents and tutorials when you encounter any
+difficulties. * The socket server is designed for obtaining colors from the
+Rickrack software in real-time. By default, this server is disabled and can
+only be started from the command line.
                                               :arrow_up:_Back_to_TOC_:arrow_up:
 # Development ## Install Requirement * Python 3.6 * Git version control system
 * Additional modules listed in requirements folder ## How to Build the Software
 ```bash # Download the Rickrack source code. git clone https://github.com/
-eigenmiao/Rickrack.git # Change into the directory. cd Rickrack # Install the
-Rickrack starter. pip install rickrack # Display the help information. rickrack
--h # Run Rickrack. rickrack ``` ## How to Build the Module ```bash # Download
-the Rickrack source code. git clone https://github.com/eigenmiao/Rickrack.git #
+eigenmiao/Rickrack.git # Change into the directory. cd Rickrack # Run Rickrack.
+python src/main/python/main.py # Generate the installer for Rickrack. fbs
+freeze && fbs installer ``` ## How to Build the Module ```bash # Download the
+Rickrack source code. git clone https://github.com/eigenmiao/Rickrack.git #
 Change into the directory. cd Rickrack # Generate the package for Rickrack.
 python setup.py sdist --formats=gztar,zip ```
                                               :arrow_up:_Back_to_TOC_:arrow_up:
 # Copyright Copyright (c) 2019-2023 [Eigenmiao](mailto:eigenmiao@outlook.com).
 All Rights Reserved.
                                               :arrow_up:_Back_to_TOC_:arrow_up:
-# License ## License for Rickrack Rickrack is a free software, which is
-distributed in the hope that it will be useful, but without any warranty. You
-can redistribute it and/or modify it under the terms of the GNU General Public
-License as published by the Free Software Foundation. See the [GNU General
-Public License 3.0 (GPL 3.0)](https://www.gnu.org/licenses/) for more details.
-All images, documents and translations in Rickrack [code repository](https://
-github.com/eigenmiao/Rickrack) are licensed under [Creative Commons
-Attribution-NonCommercial-ShareAlike License 4.0 (CC BY-NC-SA 4.0)](https://
-creativecommons.org/licenses/by-nc-sa/4.0/) unless stating additionally.
-Rickrack default uses [LXGW WenKai](https://github.com/lxgw/LxgwWenKai) font
-for interface display, which is an open-source Chinese font derived from
-Fontworks' Klee One. This font is open-sourced under [SIL Open Font License
-1.1](http://scripts.sil.org/OFL). ## License for Required Packages | Package |
-Version | License | |----------------|----------|------------------| | altgraph
-| 0.17.2 | MIT | | fbs | 0.8.9 | GPLv3 or Later | | future | 0.18.2 | MIT | |
-lxml | 4.6.3 | BSD | | macholib | 1.15.2 | MIT | | numpy | 1.19.5 | BSD | |
-pefile | 2021.9.3 | MIT | | Pillow | 8.4.0 | HPND | | pip | 21.3.1 | MIT | |
-PyInstaller | 3.4 | GPLv2 or Later | | PyQt5 | 5.12.1 | GPLv3 | | PyQt5_sip |
+# Contributing This project welcomes contributions of all types. Recommending
+Rickrack to people you know, writing reviews for Rickrack on websites, help
+spec'ing, design, documentation, finding bugs, etc. can all help the project
+grow better. # License ## License for Rickrack Rickrack is a free software,
+which is distributed in the hope that it will be useful, but without any
+warranty. You can redistribute it and/or modify it under the terms of the GNU
+General Public License as published by the Free Software Foundation. See the
+[GNU General Public License 3.0 (GPL 3.0)](https://www.gnu.org/licenses/) for
+more details. All images, documents and translations in Rickrack [code
+repository](https://github.com/eigenmiao/Rickrack) are licensed under [Creative
+Commons Attribution-NonCommercial-ShareAlike License 4.0 (CC BY-NC-SA 4.0)]
+(https://creativecommons.org/licenses/by-nc-sa/4.0/) unless stating
+additionally. Rickrack default uses [Noto Serif](https://fonts.google.com/
+specimen/Noto+Serif) ([SC](https://fonts.google.com/specimen/Noto+Serif+SC))
+fonts and [Noto Sans](https://fonts.google.com/specimen/Noto+Sans) ([SC](https:
+//fonts.google.com/specimen/Noto+Sans+SC)) fonts for interface display, which
+are designed by Google and published in website [Google Fonts](https://
+fonts.google.com/). These fonts are open-sourced under [Apache 2.0](http://
+www.apache.org/licenses/) and [SIL Open Font License 1.1](http://
+scripts.sil.org/OFL), respectively. ## License for Required Packages | Package
+| Version | License | |----------------|----------|------------------| |
+altgraph | 0.17.2 | MIT | | fbs | 0.8.9 | GPLv3 or Later | | future | 0.18.2 |
+MIT | | lxml | 4.6.3 | BSD | | macholib | 1.15.2 | MIT | | numpy | 1.19.5 | BSD
+| | pefile | 2021.9.3 | MIT | | Pillow | 8.4.0 | HPND | | pip | 21.3.1 | MIT |
+| PyInstaller | 3.4 | GPLv2 or Later | | PyQt5 | 5.12.1 | GPLv3 | | PyQt5_sip |
 4.19.19 | SIP | | pywin32 | 302 | PSF | | pywin32-ctypes | 0.2.0 | BSD | |
 ricore | 0.0.0 | Not Open-sourced | | setuptools | 40.6.2 | MIT | | swatch |
 0.4.0 | MIT |
                                               :arrow_up:_Back_to_TOC_:arrow_up:
-# More Information * Documentation: https://eigenmiao.com/2021/12/12/rickrack-
-tutorial-en-v2.3.4/ . * The installation package can be unzipped and run
-directly. This method does not require administrator privileges and can solve
-some installation failure problems. * The socket server is designed for
-obtaining colors from the Rickrack software in real-time. By default, this
-server is disabled and can only be started from the command line. * Rickrack is
-written in [Python](https://www.python.org/), constructed based on [PyQt5]
-(https://www.qt.io/qt-for-python) and packed up by [fbs (free edition)](https:/
-/build-system.fman.io/). * The code repository of Rickrack is deposited on
-[Github](https://github.com/eigenmiao/Rickrack) and [Gitee](https://gitee.com/
-eigenmiao/Rickrack). * The localization (l10n) and internationalization (i18n)
-of Rickrack is based on [Google Translate](https://translate.google.cn/) and
-[Microsoft Translator](https://cn.bing.com/translator), deployed on [POEditor]
-(https://poeditor.com/join/project?hash=kBeQjfxCES). * The cover image uses
-images from [Pixabay, which is created by martynaszulist](https://pixabay.com/
-zh/photos/pattern-the-palette-web-1508277/). * In some demo animations, [images
-of Ghibli](https://www.ghibli.jp/info/013409/) were used.
-                                              :arrow_up:_Back_to_TOC_:arrow_up:
-# Contributing This project welcomes contributions of all types. If you want to
-contribute code (new features, or bug fixes) to this project, please contact me
-first. Thanks.
+# More Information * Rickrack is written in [Python](https://www.python.org/),
+constructed based on [PyQt5](https://www.qt.io/qt-for-python) and packed up by
+[fbs (free edition)](https://build-system.fman.io/). * The code repository of
+Rickrack is deposited on [Github](https://github.com/eigenmiao/Rickrack) and
+[Gitee](https://gitee.com/eigenmiao/Rickrack). * The localization (l10n) and
+internationalization (i18n) of Rickrack is based on [Google Translate](https://
+translate.google.cn/) and [Microsoft Translator](https://cn.bing.com/
+translator), deployed on [POEditor](https://poeditor.com/join/
+project?hash=kBeQjfxCES). * The cover image uses images from [Pixabay, which is
+created by martynaszulist](https://pixabay.com/zh/photos/pattern-the-palette-
+web-1508277/). * In some demo animations, [images of Ghibli](https://
+www.ghibli.jp/info/013409/) were used. * The interface display in demo
+animations uses the [LXGWWenKai font](https://lxgw.github.io/2021/01/28/Klee-
+Simpchin/).
                                               :arrow_up:_Back_to_TOC_:arrow_up:
-# Acknowledgment ## Reviews
+# Acknowledgment ## Publicity & Promotion
       [https://yt3.googleusercontent.com/ytc/        [https://cdnssl.softpedia.com/         [https://cdn.sspai.com/2023/01/14/
 AGIKgqPSY98ka46AxjcUBDDntl1NHA8lL4PFMZt6g75TFA=s176-          _img/editors/          eab0a38256bc3a045f8d5bf76dd30072.png?imageMogr2/
                c-k-c0x00ffffff-no-rj]                Robert%20Condorache.jpg?v=2020]    auto-orient/quality/95/thumbnail/!200x200r/
                   TJ FREE@Youtube                     Robert Condorache@Softpedia      gravity/Center/crop/200x200/interlace/1]
                                                                                                  æ¬å¾åµå½æ°@å°æ°æ´¾
-## Translators
+## l10n & i18n
 [https://avatars.githubusercontent.com/u/59333735?v=4]
                   Eigenmiao@POEditor
 ## Feature Implementation & Bug Fix
 [https://avatars.githubusercontent.com/u/59333735?v=4]
                    Eigenmiao@Github
 ## Software Dependency
           [https://                      [https://                      [https://
```

### Comparing `Rickrack-2.8.27/README.md` & `Rickrack-2.8.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -9,26 +9,22 @@
 </div>
 
 # Rickrack
 In the age of digital creativity, the color palette has become an indispensable tool for designers. A good color palette can make a design more attractive and coordinated. Rickrack is designed for you if you are looking for an excellent color palette software! Rickrack has various color mixing functions and is suitable for various scenes. Rickrack is easy to use, and more importantly, it's completely free without networking or registration required.
 
 Rickrack (**R**e**a**l-t**i**me **C**olor **K**it) is a free and user-friendly color editor. It is designed to generate a set of harmonious colors from the color wheel or other places. You can share these colors with your friends, or apply them into your creative works. What’s more, you can export them into individual files and import them into other softwares such as Adobe Photoshop, GIMP, Krita, Pencil 2D and Clip Studio Paint. Rickrack can run normally on operating systems such as Windows, Linux, and macOS.
 
-[:rocket: v2.8.27 Update Notes](https://github.com/eigenmiao/Rickrack/releases/tag/v2.8.27)
-
 [:house: Rickrack](https://eigenmiao.com/rickrack)
 
 [:arrow_down: Translations of the Introduction in Other Languages :arrow_down:](#introduction-translations)
 
 # 焰火十二卷
 在数字创意的时代，调色板成为了设计师不可或缺的工具。一个好的调色板可以让设计更加有吸引力和协调性。如果你正在寻找一款优秀的调色板软件，那就试试焰火十二卷吧！焰火十二卷具有多种配色功能，适用于多种场景。焰火十二卷简单易上手，更重要的是，它完全免费，无需联网或注册。
 
-焰火十二卷（实时色彩工具箱）是一款免费且实用的色彩编辑器。它可以帮助你从色轮或者其他地方生成一组和谐的色彩。你可以将这些色彩分享给其他人，或者应用到你自己的创作当中。此外，你也可以将色彩组或者色库导出为单独的色彩文档并导入其他软件中（如 Adobe Photoshop、GIMP、Krita、Pencil 2D 以及优动漫 Paint 等）。焰火十二卷可以在 Windows、Linux、macOS 等操作系统上正常运行。
-
-[:rocket: v2.8.27 更新说明](https://github.com/eigenmiao/Rickrack/releases/tag/v2.8.27)
+焰火十二卷（实时色彩工具箱）是一款免费且实用的色彩编辑器。它可以帮助你从色轮或者其他地方生成一组和谐的色彩。你可以将这些色彩分享给其他人，或者应用到你自己的创作当中。此外，你也可以将色彩组或者色彩仓库导出为单独的色彩文档并导入其他软件中（如 Adobe Photoshop、GIMP、Krita、Pencil 2D 以及优动漫 Paint 等）。焰火十二卷可以在 Windows、Linux、macOS 等操作系统上正常运行。
 
 [:house: 焰火十二卷](https://eigenmiao.com/yanhuo)
 
 [:arrow_down: 简介的其他语言翻译 :arrow_down:](#introduction-translations)
 
 # Table of Content
 * [Introduction Translations](#introduction-translations)
@@ -191,24 +187,24 @@
 * [:hugs: 本征喵函数 @ 爱发电](https://afdian.net/a/eigenmiao)
 * [:hugs: Eigenmiao @ Ko-fi](https://ko-fi.com/eigenmiao)
 
 <div align="right"><a href="#table-of-content">:arrow_up: Back to TOC  :arrow_up:</a></div>
 
 # Installation
 ## Current Release
-The latest preview version is [v2.8.27](https://github.com/eigenmiao/Rickrack/releases/tag/v2.8.27).
+The latest preview version is [v2.8.5](https://github.com/eigenmiao/Rickrack/releases/tag/v2.8.5).
 
 ## Install Software
 ### Recommend: Install on Windows 10 or 11 via WinGet tool
 ```
 winget install rickrack
 ```
 
 ## Install on other platforms
-Download Software from [Github](https://github.com/eigenmiao/Rickrack/releases/tag/v2.8.27) or [Sourceforge](https://sourceforge.net/projects/rickrack/files/v2.8.27/). The installation steps are presented in [tutorials](https://eigenmiao.com/2021/12/12/rickrack-tutorial-en-v2.3.4/#Installation).
+Download Software from [Github](https://github.com/eigenmiao/Rickrack/releases/tag/v2.8.5) or [Sourceforge](https://sourceforge.net/projects/rickrack/files/v2.8.5/). The installation steps are presented in [tutorials](https://eigenmiao.com/2021/12/12/rickrack-tutorial-en-v2.3.4/#Installation).
 
 Here is a [video tutorial](https://www.bilibili.com/video/BV17r4y1L7R6/).
 
 ## Install Module
 Install the latest [Rickrack](https://pypi.org/project/Rickrack/) from PyPI!
 
 ```Bash
@@ -221,24 +217,24 @@
 
 <div align="right"><a href="#table-of-content">:arrow_up: Back to TOC  :arrow_up:</a></div>
 
 # Usage
 ## How to Use the Software
 Visit https://eigenmiao.com/rickrack/ for tutorials. Just feel free to click anywhere in the interface!
 
-Here is a [video tutorial](https://www.bilibili.com/video/BV1BM411L75t/).
+Here is a [video tutorial](https://www.bilibili.com/video/BV17L4y1A7P9/).
 
-Here is a [demo](https://eigenmiao.com/2023/01/29/color-palette-generator-rickrack-en/).
+Here is a [demo](https://eigenmiao.com/2023/01/29/rickrack-alternative-to-adobe-color-en/).
 
 ## How to Use the Module
 Include Rickrack in other Python scripts, programs and softwares!
 
 Here is a [video tutorial](https://www.bilibili.com/video/BV1VD4y157tX/).
 
-Here is a [demo](demo/03_plot_scripts).
+Here is a [demo](demo/).
 
 ```Python
 # Use Rickrack module in code.
 # This code fragment could be reused.
 
 from rickrack import Rickrack
 
@@ -250,14 +246,18 @@
 dp_argv = dict()
 dp_argv["help"] = True
 
 # Run and see the full contents and examples.
 rr.run(dp_argv=dp_argv, dp_proj=dp_proj)
 ```
 
+## Notice
+* Please read the documents and tutorials when you encounter any difficulties.
+* The socket server is designed for obtaining colors from the Rickrack software in real-time. By default, this server is disabled and can only be started from the command line.
+
 <div align="right"><a href="#table-of-content">:arrow_up: Back to TOC  :arrow_up:</a></div>
 
 # Development
 ## Install Requirement
 * Python 3.6
 * Git version control system
 * Additional modules listed in requirements folder
@@ -266,22 +266,19 @@
 ```bash
 # Download the Rickrack source code.
 git clone https://github.com/eigenmiao/Rickrack.git
 
 # Change into the directory.
 cd Rickrack
 
-# Install the Rickrack starter.
-pip install rickrack
-
-# Display the help information.
-rickrack -h
-
 # Run Rickrack.
-rickrack
+python src/main/python/main.py
+
+# Generate the installer for Rickrack.
+fbs freeze && fbs installer
 ```
 
 ## How to Build the Module
 ```bash
 # Download the Rickrack source code.
 git clone https://github.com/eigenmiao/Rickrack.git
 
@@ -295,21 +292,24 @@
 <div align="right"><a href="#table-of-content">:arrow_up: Back to TOC  :arrow_up:</a></div>
 
 # Copyright
 Copyright (c) 2019-2023 [Eigenmiao](mailto:eigenmiao@outlook.com). All Rights Reserved.
 
 <div align="right"><a href="#table-of-content">:arrow_up: Back to TOC  :arrow_up:</a></div>
 
+# Contributing
+This project welcomes contributions of all types. Recommending Rickrack to people you know, writing reviews for Rickrack on websites, help spec'ing, design, documentation, finding bugs, etc. can all help the project grow better.
+
 # License
 ## License for Rickrack
 Rickrack is a free software, which is distributed in the hope that it will be useful, but without any warranty. You can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation. See the [GNU General Public License 3.0 (GPL 3.0)](https://www.gnu.org/licenses/) for more details.
 
 All images, documents and translations in Rickrack [code repository](https://github.com/eigenmiao/Rickrack) are licensed under [Creative Commons Attribution-NonCommercial-ShareAlike License 4.0 (CC BY-NC-SA 4.0)](https://creativecommons.org/licenses/by-nc-sa/4.0/) unless stating additionally.
 
-Rickrack default uses [LXGW WenKai](https://github.com/lxgw/LxgwWenKai) font for interface display, which is an open-source Chinese font derived from Fontworks' Klee One. This font is open-sourced under [SIL Open Font License 1.1](http://scripts.sil.org/OFL).
+Rickrack default uses [Noto Serif](https://fonts.google.com/specimen/Noto+Serif) ([SC](https://fonts.google.com/specimen/Noto+Serif+SC)) fonts and [Noto Sans](https://fonts.google.com/specimen/Noto+Sans) ([SC](https://fonts.google.com/specimen/Noto+Sans+SC)) fonts for interface display, which are designed by Google and published in website [Google Fonts](https://fonts.google.com/). These fonts are open-sourced under [Apache 2.0](http://www.apache.org/licenses/) and [SIL Open Font License 1.1](http://scripts.sil.org/OFL), respectively.
 
 ## License for Required Packages
 | Package        | Version  | License          |
 |----------------|----------|------------------|
 | altgraph       | 0.17.2   | MIT              |
 | fbs            | 0.8.9    | GPLv3 or Later   |
 | future         | 0.18.2   | MIT              |
@@ -327,43 +327,36 @@
 | ricore         | 0.0.0    | Not Open-sourced |
 | setuptools     | 40.6.2   | MIT              |
 | swatch         | 0.4.0    | MIT              |
 
 <div align="right"><a href="#table-of-content">:arrow_up: Back to TOC  :arrow_up:</a></div>
 
 # More Information
-* Documentation: https://eigenmiao.com/2021/12/12/rickrack-tutorial-en-v2.3.4/ .
-* The installation package can be unzipped and run directly. This method does not require administrator privileges and can solve some installation failure problems.
-* The socket server is designed for obtaining colors from the Rickrack software in real-time. By default, this server is disabled and can only be started from the command line.
 * Rickrack is written in [Python](https://www.python.org/), constructed based on [PyQt5](https://www.qt.io/qt-for-python) and packed up by [fbs (free edition)](https://build-system.fman.io/).
 * The code repository of Rickrack is deposited on [Github](https://github.com/eigenmiao/Rickrack) and [Gitee](https://gitee.com/eigenmiao/Rickrack).
 * The localization (l10n) and internationalization (i18n) of Rickrack is based on [Google Translate](https://translate.google.cn/) and [Microsoft Translator](https://cn.bing.com/translator), deployed on [POEditor](https://poeditor.com/join/project?hash=kBeQjfxCES).
 * The cover image uses images from [Pixabay, which is created by martynaszulist](https://pixabay.com/zh/photos/pattern-the-palette-web-1508277/).
 * In some demo animations, [images of Ghibli](https://www.ghibli.jp/info/013409/) were used.
-
-<div align="right"><a href="#table-of-content">:arrow_up: Back to TOC  :arrow_up:</a></div>
-
-# Contributing
-This project welcomes contributions of all types. If you want to contribute code (new features, or bug fixes) to this project, please contact me first. Thanks.
+* The interface display in demo animations uses the [LXGWWenKai font](https://lxgw.github.io/2021/01/28/Klee-Simpchin/).
 
 <div align="right"><a href="#table-of-content">:arrow_up: Back to TOC  :arrow_up:</a></div>
 
 # Acknowledgment
-## Reviews
+## Publicity & Promotion
 <table>
   <tbody>
     <tr>
     <td align="center" valign="top" width="20%"><a href="https://www.youtube.com/watch?v=OUnktTCtv3E"><img src="https://yt3.googleusercontent.com/ytc/AGIKgqPSY98ka46AxjcUBDDntl1NHA8lL4PFMZt6g75TFA=s176-c-k-c0x00ffffff-no-rj" width="90px;"/><br /><sub><b>TJ&nbsp;FREE@Youtube</b></sub></a></td>
     <td align="center" valign="top" width="20%"><a href="https://www.softpedia.com/get/Multimedia/Graphic/Graphic-Others/RickRack.shtml"><img src="https://cdnssl.softpedia.com/_img/editors/Robert%20Condorache.jpg?v=2020" width="90px;"/><br /><sub><b>Robert&nbsp;Condorache@Softpedia</b></sub></a></td>
     <td align="center" valign="top" width="20%"><a href="https://sspai.com/u/eigenmiao/updates"><img src="https://cdn.sspai.com/2023/01/14/eab0a38256bc3a045f8d5bf76dd30072.png?imageMogr2/auto-orient/quality/95/thumbnail/!200x200r/gravity/Center/crop/200x200/interlace/1" width="90px;"/><br /><sub><b>本征喵函数@少数派</b></sub></a></td>
     </tr>
   </tbody>
 </table>
 
-## Translators
+## l10n & i18n
 <table>
   <tbody>
     <tr>
     <td align="center" valign="top" width="20%"><a href="https://poeditor.com/join/project?hash=kBeQjfxCES"><img src="https://avatars.githubusercontent.com/u/59333735?v=4" width="90px;"/><br /><sub><b>Eigenmiao@POEditor</b></sub></a></td>
     </tr>
   </tbody>
 </table>
```

#### html2text {}

```diff
@@ -19,62 +19,59 @@
 importantly, it's completely free without networking or registration required.
 Rickrack (**R**e**a**l-t**i**me **C**olor **K**it) is a free and user-friendly
 color editor. It is designed to generate a set of harmonious colors from the
 color wheel or other places. You can share these colors with your friends, or
 apply them into your creative works. Whatâs more, you can export them into
 individual files and import them into other softwares such as Adobe Photoshop,
 GIMP, Krita, Pencil 2D and Clip Studio Paint. Rickrack can run normally on
-operating systems such as Windows, Linux, and macOS. [:rocket: v2.8.27 Update
-Notes](https://github.com/eigenmiao/Rickrack/releases/tag/v2.8.27) [:house:
-Rickrack](https://eigenmiao.com/rickrack) [:arrow_down: Translations of the
-Introduction in Other Languages :arrow_down:](#introduction-translations) #
-ç°ç«åäºå·
+operating systems such as Windows, Linux, and macOS. [:house: Rickrack](https:/
+/eigenmiao.com/rickrack) [:arrow_down: Translations of the Introduction in
+Other Languages :arrow_down:](#introduction-translations) # ç°ç«åäºå·
 å¨æ°å­åæçæ¶ä»£ï¼è°è²æ¿æä¸ºäºè®¾è®¡å¸ä¸å¯æç¼ºçå·¥å·ãä¸ä¸ªå¥½çè°è²æ¿å¯ä»¥è®©è®¾è®¡æ´å æå¸å¼åååè°æ§ãå¦æä½ æ­£å¨å¯»æ¾ä¸æ¬¾ä¼ç§çè°è²æ¿è½¯ä»¶ï¼é£å°±è¯è¯ç°ç«åäºå·å§ï¼ç°ç«åäºå·å·æå¤ç§éè²åè½ï¼éç¨äºå¤ç§åºæ¯ãç°ç«åäºå·ç®åæä¸æï¼æ´éè¦çæ¯ï¼å®å®å¨åè´¹ï¼æ éèç½ææ³¨åã
-ç°ç«åäºå·ï¼å®æ¶è²å½©å·¥å·ç®±ï¼æ¯ä¸æ¬¾åè´¹ä¸å®ç¨çè²å½©ç¼è¾å¨ãå®å¯ä»¥å¸®å©ä½ ä»è²è½®æèå¶ä»å°æ¹çæä¸ç»åè°çè²å½©ãä½ å¯ä»¥å°è¿äºè²å½©åäº«ç»å¶ä»äººï¼æèåºç¨å°ä½ èªå·±çåä½å½ä¸­ãæ­¤å¤ï¼ä½ ä¹å¯ä»¥å°è²å½©ç»æèè²åºå¯¼åºä¸ºåç¬çè²å½©ææ¡£å¹¶å¯¼å¥å¶ä»è½¯ä»¶ä¸­ï¼å¦
+ç°ç«åäºå·ï¼å®æ¶è²å½©å·¥å·ç®±ï¼æ¯ä¸æ¬¾åè´¹ä¸å®ç¨çè²å½©ç¼è¾å¨ãå®å¯ä»¥å¸®å©ä½ ä»è²è½®æèå¶ä»å°æ¹çæä¸ç»åè°çè²å½©ãä½ å¯ä»¥å°è¿äºè²å½©åäº«ç»å¶ä»äººï¼æèåºç¨å°ä½ èªå·±çåä½å½ä¸­ãæ­¤å¤ï¼ä½ ä¹å¯ä»¥å°è²å½©ç»æèè²å½©ä»åºå¯¼åºä¸ºåç¬çè²å½©ææ¡£å¹¶å¯¼å¥å¶ä»è½¯ä»¶ä¸­ï¼å¦
 Adobe PhotoshopãGIMPãKritaãPencil 2D ä»¥åä¼å¨æ¼« Paint
 ç­ï¼ãç°ç«åäºå·å¯ä»¥å¨ WindowsãLinuxãmacOS
-ç­æä½ç³»ç»ä¸æ­£å¸¸è¿è¡ã [:rocket: v2.8.27 æ´æ°è¯´æ](https://
-github.com/eigenmiao/Rickrack/releases/tag/v2.8.27) [:house: ç°ç«åäºå·]
-(https://eigenmiao.com/yanhuo) [:arrow_down: ç®ä»çå¶ä»è¯­è¨ç¿»è¯ :
-arrow_down:](#introduction-translations) # Table of Content * [Introduction
-Translations](#introduction-translations) * [Features](#features) * [Demo]
-(#demo) * [Basic Functions](#basic-functions) * [Reference Colors](#reference-
-colors) * [Color Palettes](#color-palettes) * [Export and Import Colors]
-(#export-and-import-colors) * [Languages and Settings](#languages-and-settings)
-* [Reviews about Rickrack](#reviews-about-rickrack) * [Information]
-(#information) * [Website](#website) * [Repository](#repository) * [Author]
-(#author) * [Support](#support) * [Installation](#installation) * [Current
-Release](#current-release) * [Download Software](#download-software) * [Install
-Software](#install-software) * [Install Module](#install-module) * [Usage]
-(#usage) * [How to Use the Software](#how-to-use-the-software) * [How to Use
-the Module](#how-to-use-the-module) * [Development](#development) * [Install
-Requirement](#install-requirement) * [How to Build the Software](#how-to-build-
-the-software) * [How to Build the Module](#how-to-build-the-module) *
-[Copyright](#copyright) * [License](#license) * [License for Rickrack]
-(#license-for-rickrack) * [License for Required Packages](#license-for-
-required-packages) * [More Information](#more-information) * [Acknowledgment]
-(#acknowledgment) # Introduction Translations ## Rickrack (Esperanto) En la
-epoko de cifereca kreemo, la kolora paletro fariÄis nemalhavebla ilo por
-dezajnistoj. Bona kolora paletro povas fari dezajnon pli alloga kaj
-kunordigita. Rickrack estas desegnita por vi, se vi serÄas bonegan programaron
-de kolora paletro! Rickrack havas diversajn kolorajn miksajn funkciojn kaj
-taÅ­gas por diversaj scenoj. Rickrack estas facile uzebla, kaj pli grave, Äi
-estas tute senpaga sen interkonektado aÅ­ registriÄo necesa. Rickrack estas
-senpaga kaj amika kolorredaktilo. Äi estas desegnita por generi aron da
-harmoniaj koloroj de la kolorrado aÅ­ aliaj lokoj. Vi povas dividi Äi tiujn
-kolorojn kun viaj amikoj, aÅ­ apliki ilin en viajn kreajn verkojn. Krome, vi
-povas eksporti ilin en individuajn dosierojn kaj importi ilin en aliajn
-programojn kiel Adobe Photoshop, GIMP, Krita, Pencil 2D kaj Clip Studio Paint.
-Rickrack povas funkcii normale per operaciumoj kiel Vindozo, Linukso kaj macOS.
-(Tradukoj supre baziÄas sur Google Translate.) [:house: Rickrack](https://
-eigenmiao.com/yanhuo/eo.html) ## Rickrack (Ð ÑÑÑÐºÐ¸Ð¹) Ð Ð²ÐµÐº
-ÑÐ¸ÑÑÐ¾Ð²Ð¾Ð³Ð¾ ÑÐ²Ð¾ÑÑÐµÑÑÐ²Ð° ÑÐ²ÐµÑÐ¾Ð²Ð°Ñ Ð¿Ð°Ð»Ð¸ÑÑÐ°
-ÑÑÐ°Ð»Ð° Ð½ÐµÐ·Ð°Ð¼ÐµÐ½Ð¸Ð¼ÑÐ¼ Ð¸Ð½ÑÑÑÑÐ¼ÐµÐ½ÑÐ¾Ð¼ Ð´Ð»Ñ
-Ð´Ð¸Ð·Ð°Ð¹Ð½ÐµÑÐ¾Ð². Ð¥Ð¾ÑÐ¾ÑÐ°Ñ ÑÐ²ÐµÑÐ¾Ð²Ð°Ñ Ð¿Ð°Ð»Ð¸ÑÑÐ° Ð¼Ð¾Ð¶ÐµÑ
-ÑÐ´ÐµÐ»Ð°ÑÑ Ð´Ð¸Ð·Ð°Ð¹Ð½ Ð±Ð¾Ð»ÐµÐµ Ð¿ÑÐ¸Ð²Ð»ÐµÐºÐ°ÑÐµÐ»ÑÐ½ÑÐ¼ Ð¸
+ç­æä½ç³»ç»ä¸æ­£å¸¸è¿è¡ã [:house: ç°ç«åäºå·](https://
+eigenmiao.com/yanhuo) [:arrow_down: ç®ä»çå¶ä»è¯­è¨ç¿»è¯ :arrow_down:]
+(#introduction-translations) # Table of Content * [Introduction Translations]
+(#introduction-translations) * [Features](#features) * [Demo](#demo) * [Basic
+Functions](#basic-functions) * [Reference Colors](#reference-colors) * [Color
+Palettes](#color-palettes) * [Export and Import Colors](#export-and-import-
+colors) * [Languages and Settings](#languages-and-settings) * [Reviews about
+Rickrack](#reviews-about-rickrack) * [Information](#information) * [Website]
+(#website) * [Repository](#repository) * [Author](#author) * [Support]
+(#support) * [Installation](#installation) * [Current Release](#current-
+release) * [Download Software](#download-software) * [Install Software]
+(#install-software) * [Install Module](#install-module) * [Usage](#usage) *
+[How to Use the Software](#how-to-use-the-software) * [How to Use the Module]
+(#how-to-use-the-module) * [Development](#development) * [Install Requirement]
+(#install-requirement) * [How to Build the Software](#how-to-build-the-
+software) * [How to Build the Module](#how-to-build-the-module) * [Copyright]
+(#copyright) * [License](#license) * [License for Rickrack](#license-for-
+rickrack) * [License for Required Packages](#license-for-required-packages) *
+[More Information](#more-information) * [Acknowledgment](#acknowledgment) #
+Introduction Translations ## Rickrack (Esperanto) En la epoko de cifereca
+kreemo, la kolora paletro fariÄis nemalhavebla ilo por dezajnistoj. Bona
+kolora paletro povas fari dezajnon pli alloga kaj kunordigita. Rickrack estas
+desegnita por vi, se vi serÄas bonegan programaron de kolora paletro! Rickrack
+havas diversajn kolorajn miksajn funkciojn kaj taÅ­gas por diversaj scenoj.
+Rickrack estas facile uzebla, kaj pli grave, Äi estas tute senpaga sen
+interkonektado aÅ­ registriÄo necesa. Rickrack estas senpaga kaj amika
+kolorredaktilo. Äi estas desegnita por generi aron da harmoniaj koloroj de la
+kolorrado aÅ­ aliaj lokoj. Vi povas dividi Äi tiujn kolorojn kun viaj amikoj,
+aÅ­ apliki ilin en viajn kreajn verkojn. Krome, vi povas eksporti ilin en
+individuajn dosierojn kaj importi ilin en aliajn programojn kiel Adobe
+Photoshop, GIMP, Krita, Pencil 2D kaj Clip Studio Paint. Rickrack povas funkcii
+normale per operaciumoj kiel Vindozo, Linukso kaj macOS. (Tradukoj supre
+baziÄas sur Google Translate.) [:house: Rickrack](https://eigenmiao.com/
+yanhuo/eo.html) ## Rickrack (Ð ÑÑÑÐºÐ¸Ð¹) Ð Ð²ÐµÐº ÑÐ¸ÑÑÐ¾Ð²Ð¾Ð³Ð¾
+ÑÐ²Ð¾ÑÑÐµÑÑÐ²Ð° ÑÐ²ÐµÑÐ¾Ð²Ð°Ñ Ð¿Ð°Ð»Ð¸ÑÑÐ° ÑÑÐ°Ð»Ð°
+Ð½ÐµÐ·Ð°Ð¼ÐµÐ½Ð¸Ð¼ÑÐ¼ Ð¸Ð½ÑÑÑÑÐ¼ÐµÐ½ÑÐ¾Ð¼ Ð´Ð»Ñ Ð´Ð¸Ð·Ð°Ð¹Ð½ÐµÑÐ¾Ð².
+Ð¥Ð¾ÑÐ¾ÑÐ°Ñ ÑÐ²ÐµÑÐ¾Ð²Ð°Ñ Ð¿Ð°Ð»Ð¸ÑÑÐ° Ð¼Ð¾Ð¶ÐµÑ ÑÐ´ÐµÐ»Ð°ÑÑ
+Ð´Ð¸Ð·Ð°Ð¹Ð½ Ð±Ð¾Ð»ÐµÐµ Ð¿ÑÐ¸Ð²Ð»ÐµÐºÐ°ÑÐµÐ»ÑÐ½ÑÐ¼ Ð¸
 Ð³Ð°ÑÐ¼Ð¾Ð½Ð¸ÑÐ½ÑÐ¼. Rickrack ÑÐ°Ð·ÑÐ°Ð±Ð¾ÑÐ°Ð½ Ð´Ð»Ñ Ð²Ð°Ñ, ÐµÑÐ»Ð¸
 Ð²Ñ Ð¸ÑÐµÑÐµ Ð¾ÑÐ»Ð¸ÑÐ½Ð¾Ðµ Ð¿ÑÐ¾Ð³ÑÐ°Ð¼Ð¼Ð½Ð¾Ðµ Ð¾Ð±ÐµÑÐ¿ÐµÑÐµÐ½Ð¸Ðµ
 Ð´Ð»Ñ ÑÐ²ÐµÑÐ¾Ð²Ð¾Ð¹ Ð¿Ð°Ð»Ð¸ÑÑÑ! Rickrack Ð¸Ð¼ÐµÐµÑ ÑÐ°Ð·Ð»Ð¸ÑÐ½ÑÐµ
 ÑÑÐ½ÐºÑÐ¸Ð¸ ÑÐ¼ÐµÑÐ¸Ð²Ð°Ð½Ð¸Ñ ÑÐ²ÐµÑÐ¾Ð² Ð¸ Ð¿Ð¾Ð´ÑÐ¾Ð´Ð¸Ñ Ð´Ð»Ñ
 ÑÐ°Ð·Ð»Ð¸ÑÐ½ÑÑ ÑÑÐµÐ½. Rickrack Ð¿ÑÐ¾ÑÑ Ð² Ð¸ÑÐ¿Ð¾Ð»ÑÐ·Ð¾Ð²Ð°Ð½Ð¸Ð¸
 Ð¸, ÑÑÐ¾ Ð±Ð¾Ð»ÐµÐµ Ð²Ð°Ð¶Ð½Ð¾, ÑÐ¾Ð²ÐµÑÑÐµÐ½Ð½Ð¾ Ð±ÐµÑÐ¿Ð»Ð°ÑÐµÐ½, Ð½Ðµ
 ÑÑÐµÐ±ÑÐµÑ Ð¿Ð¾Ð´ÐºÐ»ÑÑÐµÐ½Ð¸Ñ Ðº ÑÐµÑÐ¸ Ð¸Ð»Ð¸
@@ -210,104 +207,107 @@
                                               :arrow_up:_Back_to_TOC_:arrow_up:
 # Information ## Website https://eigenmiao.com/rickrack ## Repository https://
 github.com/eigenmiao/Rickrack ## Author [Eigenmiao](mailto:
 eigenmiao@outlook.com) ## Support Support the continuous development of
 Rickrack! * [:hugs: æ¬å¾åµå½æ° @ ç±åçµ](https://afdian.net/a/
 eigenmiao) * [:hugs: Eigenmiao @ Ko-fi](https://ko-fi.com/eigenmiao)
                                               :arrow_up:_Back_to_TOC_:arrow_up:
-# Installation ## Current Release The latest preview version is [v2.8.27]
-(https://github.com/eigenmiao/Rickrack/releases/tag/v2.8.27). ## Install
-Software ### Recommend: Install on Windows 10 or 11 via WinGet tool ``` winget
-install rickrack ``` ## Install on other platforms Download Software from
-[Github](https://github.com/eigenmiao/Rickrack/releases/tag/v2.8.27) or
-[Sourceforge](https://sourceforge.net/projects/rickrack/files/v2.8.27/). The
-installation steps are presented in [tutorials](https://eigenmiao.com/2021/12/
-12/rickrack-tutorial-en-v2.3.4/#Installation). Here is a [video tutorial]
-(https://www.bilibili.com/video/BV17r4y1L7R6/). ## Install Module Install the
-latest [Rickrack](https://pypi.org/project/Rickrack/) from PyPI! ```Bash #
-Install Rickrack. pip install Rickrack # Start the installed software. rickrack
--d "/PATH/TO/RICKRACK/SOFTWARE" ```
+# Installation ## Current Release The latest preview version is [v2.8.5](https:
+//github.com/eigenmiao/Rickrack/releases/tag/v2.8.5). ## Install Software ###
+Recommend: Install on Windows 10 or 11 via WinGet tool ``` winget install
+rickrack ``` ## Install on other platforms Download Software from [Github]
+(https://github.com/eigenmiao/Rickrack/releases/tag/v2.8.5) or [Sourceforge]
+(https://sourceforge.net/projects/rickrack/files/v2.8.5/). The installation
+steps are presented in [tutorials](https://eigenmiao.com/2021/12/12/rickrack-
+tutorial-en-v2.3.4/#Installation). Here is a [video tutorial](https://
+www.bilibili.com/video/BV17r4y1L7R6/). ## Install Module Install the latest
+[Rickrack](https://pypi.org/project/Rickrack/) from PyPI! ```Bash # Install
+Rickrack. pip install Rickrack # Start the installed software. rickrack -d "/
+PATH/TO/RICKRACK/SOFTWARE" ```
                                               :arrow_up:_Back_to_TOC_:arrow_up:
 # Usage ## How to Use the Software Visit https://eigenmiao.com/rickrack/ for
 tutorials. Just feel free to click anywhere in the interface! Here is a [video
-tutorial](https://www.bilibili.com/video/BV1BM411L75t/). Here is a [demo]
-(https://eigenmiao.com/2023/01/29/color-palette-generator-rickrack-en/). ## How
-to Use the Module Include Rickrack in other Python scripts, programs and
+tutorial](https://www.bilibili.com/video/BV17L4y1A7P9/). Here is a [demo]
+(https://eigenmiao.com/2023/01/29/rickrack-alternative-to-adobe-color-en/). ##
+How to Use the Module Include Rickrack in other Python scripts, programs and
 softwares! Here is a [video tutorial](https://www.bilibili.com/video/
-BV1VD4y157tX/). Here is a [demo](demo/03_plot_scripts). ```Python # Use
-Rickrack module in code. # This code fragment could be reused. from rickrack
-import Rickrack # Init Rickrack. rr = Rickrack() # Display the help
-information. dp_proj = "/PATH/TO/RICKRACK/PROJECT" dp_argv = dict() dp_argv
-["help"] = True # Run and see the full contents and examples. rr.run
-(dp_argv=dp_argv, dp_proj=dp_proj) ```
+BV1VD4y157tX/). Here is a [demo](demo/). ```Python # Use Rickrack module in
+code. # This code fragment could be reused. from rickrack import Rickrack #
+Init Rickrack. rr = Rickrack() # Display the help information. dp_proj = "/
+PATH/TO/RICKRACK/PROJECT" dp_argv = dict() dp_argv["help"] = True # Run and see
+the full contents and examples. rr.run(dp_argv=dp_argv, dp_proj=dp_proj) ``` ##
+Notice * Please read the documents and tutorials when you encounter any
+difficulties. * The socket server is designed for obtaining colors from the
+Rickrack software in real-time. By default, this server is disabled and can
+only be started from the command line.
                                               :arrow_up:_Back_to_TOC_:arrow_up:
 # Development ## Install Requirement * Python 3.6 * Git version control system
 * Additional modules listed in requirements folder ## How to Build the Software
 ```bash # Download the Rickrack source code. git clone https://github.com/
-eigenmiao/Rickrack.git # Change into the directory. cd Rickrack # Install the
-Rickrack starter. pip install rickrack # Display the help information. rickrack
--h # Run Rickrack. rickrack ``` ## How to Build the Module ```bash # Download
-the Rickrack source code. git clone https://github.com/eigenmiao/Rickrack.git #
+eigenmiao/Rickrack.git # Change into the directory. cd Rickrack # Run Rickrack.
+python src/main/python/main.py # Generate the installer for Rickrack. fbs
+freeze && fbs installer ``` ## How to Build the Module ```bash # Download the
+Rickrack source code. git clone https://github.com/eigenmiao/Rickrack.git #
 Change into the directory. cd Rickrack # Generate the package for Rickrack.
 python setup.py sdist --formats=gztar,zip ```
                                               :arrow_up:_Back_to_TOC_:arrow_up:
 # Copyright Copyright (c) 2019-2023 [Eigenmiao](mailto:eigenmiao@outlook.com).
 All Rights Reserved.
                                               :arrow_up:_Back_to_TOC_:arrow_up:
-# License ## License for Rickrack Rickrack is a free software, which is
-distributed in the hope that it will be useful, but without any warranty. You
-can redistribute it and/or modify it under the terms of the GNU General Public
-License as published by the Free Software Foundation. See the [GNU General
-Public License 3.0 (GPL 3.0)](https://www.gnu.org/licenses/) for more details.
-All images, documents and translations in Rickrack [code repository](https://
-github.com/eigenmiao/Rickrack) are licensed under [Creative Commons
-Attribution-NonCommercial-ShareAlike License 4.0 (CC BY-NC-SA 4.0)](https://
-creativecommons.org/licenses/by-nc-sa/4.0/) unless stating additionally.
-Rickrack default uses [LXGW WenKai](https://github.com/lxgw/LxgwWenKai) font
-for interface display, which is an open-source Chinese font derived from
-Fontworks' Klee One. This font is open-sourced under [SIL Open Font License
-1.1](http://scripts.sil.org/OFL). ## License for Required Packages | Package |
-Version | License | |----------------|----------|------------------| | altgraph
-| 0.17.2 | MIT | | fbs | 0.8.9 | GPLv3 or Later | | future | 0.18.2 | MIT | |
-lxml | 4.6.3 | BSD | | macholib | 1.15.2 | MIT | | numpy | 1.19.5 | BSD | |
-pefile | 2021.9.3 | MIT | | Pillow | 8.4.0 | HPND | | pip | 21.3.1 | MIT | |
-PyInstaller | 3.4 | GPLv2 or Later | | PyQt5 | 5.12.1 | GPLv3 | | PyQt5_sip |
+# Contributing This project welcomes contributions of all types. Recommending
+Rickrack to people you know, writing reviews for Rickrack on websites, help
+spec'ing, design, documentation, finding bugs, etc. can all help the project
+grow better. # License ## License for Rickrack Rickrack is a free software,
+which is distributed in the hope that it will be useful, but without any
+warranty. You can redistribute it and/or modify it under the terms of the GNU
+General Public License as published by the Free Software Foundation. See the
+[GNU General Public License 3.0 (GPL 3.0)](https://www.gnu.org/licenses/) for
+more details. All images, documents and translations in Rickrack [code
+repository](https://github.com/eigenmiao/Rickrack) are licensed under [Creative
+Commons Attribution-NonCommercial-ShareAlike License 4.0 (CC BY-NC-SA 4.0)]
+(https://creativecommons.org/licenses/by-nc-sa/4.0/) unless stating
+additionally. Rickrack default uses [Noto Serif](https://fonts.google.com/
+specimen/Noto+Serif) ([SC](https://fonts.google.com/specimen/Noto+Serif+SC))
+fonts and [Noto Sans](https://fonts.google.com/specimen/Noto+Sans) ([SC](https:
+//fonts.google.com/specimen/Noto+Sans+SC)) fonts for interface display, which
+are designed by Google and published in website [Google Fonts](https://
+fonts.google.com/). These fonts are open-sourced under [Apache 2.0](http://
+www.apache.org/licenses/) and [SIL Open Font License 1.1](http://
+scripts.sil.org/OFL), respectively. ## License for Required Packages | Package
+| Version | License | |----------------|----------|------------------| |
+altgraph | 0.17.2 | MIT | | fbs | 0.8.9 | GPLv3 or Later | | future | 0.18.2 |
+MIT | | lxml | 4.6.3 | BSD | | macholib | 1.15.2 | MIT | | numpy | 1.19.5 | BSD
+| | pefile | 2021.9.3 | MIT | | Pillow | 8.4.0 | HPND | | pip | 21.3.1 | MIT |
+| PyInstaller | 3.4 | GPLv2 or Later | | PyQt5 | 5.12.1 | GPLv3 | | PyQt5_sip |
 4.19.19 | SIP | | pywin32 | 302 | PSF | | pywin32-ctypes | 0.2.0 | BSD | |
 ricore | 0.0.0 | Not Open-sourced | | setuptools | 40.6.2 | MIT | | swatch |
 0.4.0 | MIT |
                                               :arrow_up:_Back_to_TOC_:arrow_up:
-# More Information * Documentation: https://eigenmiao.com/2021/12/12/rickrack-
-tutorial-en-v2.3.4/ . * The installation package can be unzipped and run
-directly. This method does not require administrator privileges and can solve
-some installation failure problems. * The socket server is designed for
-obtaining colors from the Rickrack software in real-time. By default, this
-server is disabled and can only be started from the command line. * Rickrack is
-written in [Python](https://www.python.org/), constructed based on [PyQt5]
-(https://www.qt.io/qt-for-python) and packed up by [fbs (free edition)](https:/
-/build-system.fman.io/). * The code repository of Rickrack is deposited on
-[Github](https://github.com/eigenmiao/Rickrack) and [Gitee](https://gitee.com/
-eigenmiao/Rickrack). * The localization (l10n) and internationalization (i18n)
-of Rickrack is based on [Google Translate](https://translate.google.cn/) and
-[Microsoft Translator](https://cn.bing.com/translator), deployed on [POEditor]
-(https://poeditor.com/join/project?hash=kBeQjfxCES). * The cover image uses
-images from [Pixabay, which is created by martynaszulist](https://pixabay.com/
-zh/photos/pattern-the-palette-web-1508277/). * In some demo animations, [images
-of Ghibli](https://www.ghibli.jp/info/013409/) were used.
-                                              :arrow_up:_Back_to_TOC_:arrow_up:
-# Contributing This project welcomes contributions of all types. If you want to
-contribute code (new features, or bug fixes) to this project, please contact me
-first. Thanks.
+# More Information * Rickrack is written in [Python](https://www.python.org/),
+constructed based on [PyQt5](https://www.qt.io/qt-for-python) and packed up by
+[fbs (free edition)](https://build-system.fman.io/). * The code repository of
+Rickrack is deposited on [Github](https://github.com/eigenmiao/Rickrack) and
+[Gitee](https://gitee.com/eigenmiao/Rickrack). * The localization (l10n) and
+internationalization (i18n) of Rickrack is based on [Google Translate](https://
+translate.google.cn/) and [Microsoft Translator](https://cn.bing.com/
+translator), deployed on [POEditor](https://poeditor.com/join/
+project?hash=kBeQjfxCES). * The cover image uses images from [Pixabay, which is
+created by martynaszulist](https://pixabay.com/zh/photos/pattern-the-palette-
+web-1508277/). * In some demo animations, [images of Ghibli](https://
+www.ghibli.jp/info/013409/) were used. * The interface display in demo
+animations uses the [LXGWWenKai font](https://lxgw.github.io/2021/01/28/Klee-
+Simpchin/).
                                               :arrow_up:_Back_to_TOC_:arrow_up:
-# Acknowledgment ## Reviews
+# Acknowledgment ## Publicity & Promotion
       [https://yt3.googleusercontent.com/ytc/        [https://cdnssl.softpedia.com/         [https://cdn.sspai.com/2023/01/14/
 AGIKgqPSY98ka46AxjcUBDDntl1NHA8lL4PFMZt6g75TFA=s176-          _img/editors/          eab0a38256bc3a045f8d5bf76dd30072.png?imageMogr2/
                c-k-c0x00ffffff-no-rj]                Robert%20Condorache.jpg?v=2020]    auto-orient/quality/95/thumbnail/!200x200r/
                   TJ FREE@Youtube                     Robert Condorache@Softpedia      gravity/Center/crop/200x200/interlace/1]
                                                                                                  æ¬å¾åµå½æ°@å°æ°æ´¾
-## Translators
+## l10n & i18n
 [https://avatars.githubusercontent.com/u/59333735?v=4]
                   Eigenmiao@POEditor
 ## Feature Implementation & Bug Fix
 [https://avatars.githubusercontent.com/u/59333735?v=4]
                    Eigenmiao@Github
 ## Software Dependency
           [https://                      [https://                      [https://
```

### Comparing `Rickrack-2.8.27/rickrack/color.py` & `Rickrack-2.8.5/rickrack/color.py`

 * *Files 2% similar despite different names*

```diff
@@ -621,48 +621,14 @@
 
         while "" in _hec:
             _hec.remove("")
 
         return _hec
 
     @classmethod
-    def sys_rgb2ryb(cls, h):
-        """
-        Class method. Transfer hue of rgb to hue of ryb.
-        """
-
-        _h = h % 360
-
-        if 0 <= _h < 60:
-            return _h / 60 * 120
-
-        elif 60 <= _h < 240:
-            return (_h - 60) / 180 * 120 + 120
-
-        else:
-            return _h
-
-    @classmethod
-    def sys_ryb2rgb(cls, h):
-        """
-        Class method. Transfer hue of ryb to hue of rgb.
-        """
-
-        _h = h % 360
-
-        if 0 <= _h < 120:
-            return _h / 120 * 60
-
-        elif 120 <= _h < 240:
-            return (_h - 120) / 120 * 180 + 60
-
-        else:
-            return _h
-
-    @classmethod
     def stri2color(cls, stri):
         """
         Find the first possible color in string.
 
         Args:
             stri (str): rgb, hsv or hec color string.
 
@@ -1175,20 +1141,15 @@
 
         if v < 0.08:
             return (0, 0)
 
         if v > 0.95 and s < 0.05:
             return (1, 1)
 
-        prefix = 2
-
-        for start, end, idx in ((0, 20, 0), (20, 40, 6), (40, 70, 1), (70, 160, 2), (160, 190, 3), (190, 250, 4), (250, 310, 5), (310, 340, 7), (340, 360, 0)):
-            if start <= h % 360 < end:
-                prefix = idx + 2
-                break
+        prefix = int((h + 30) // 60 % 6) + 2
 
         if 0.0 <= v < 0.25:
             return (2, prefix)
 
         elif 0.25 <= v < 0.5:
             if 0 <= s < 0.25:
                 return (4, prefix)
```

### Comparing `Rickrack-2.8.27/rickrack/result.py` & `Rickrack-2.8.5/rickrack/result.py`

 * *Files identical despite different names*

### Comparing `Rickrack-2.8.27/rickrack/rickrack.py` & `Rickrack-2.8.5/rickrack/rickrack.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 """
 
 __WEBSITE__ = """
 https://github.com/eigenmiao/Rickrack
 """
 
 __VERSION__ = """
-v2.8.27-x2d3s3-pre
+v2.8.5-x2d3s3-pre
 """
 
 __AUTHOR__ = """
 Eigenmiao (eigenmiao@outlook.com)
 """
 
 __DATE__ = """
-June 25, 2023
+May 21, 2023
 """
 
 __HELP__ = """
 INTRODUCTION:
   Rickrack-Startup provides the ability to operate Rickrack from the 
   command line or through Python code, allowing you to start it, close it, 
   and obtain color results from Rickrack.
```

### Comparing `Rickrack-2.8.27/rickrack/__init__.py` & `Rickrack-2.8.5/rickrack/__init__.py`

 * *Files identical despite different names*

### Comparing `Rickrack-2.8.27/Rickrack.egg-info/PKG-INFO` & `Rickrack-2.8.5/Rickrack.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: Rickrack
-Version: 2.8.27
+Version: 2.8.5
 Summary: Generate harmonious colors freely.
-Home-page: https://eigenmiao.com/rickrack/
+Home-page: https://eigenmiao.github.io/rickrack/
 Author: Eigenmiao
 Author-email: eigenmiao@outlook.com
 License: UNKNOWN
 Description: <div align="center">
         <img width="100%" align="center" src="https://raw.githubusercontent.com/eigenmiao/Rickrack/master/src/main/icons/logo_long.png" alt="Rickrack">
         <br/><br/>
         Rickrack<br/>焰火十二卷<br/> ----- ----- ----- ----- ----- ----- ----- ----- <br/>
@@ -17,26 +17,22 @@
         </div>
         
         # Rickrack
         In the age of digital creativity, the color palette has become an indispensable tool for designers. A good color palette can make a design more attractive and coordinated. Rickrack is designed for you if you are looking for an excellent color palette software! Rickrack has various color mixing functions and is suitable for various scenes. Rickrack is easy to use, and more importantly, it's completely free without networking or registration required.
         
         Rickrack (**R**e**a**l-t**i**me **C**olor **K**it) is a free and user-friendly color editor. It is designed to generate a set of harmonious colors from the color wheel or other places. You can share these colors with your friends, or apply them into your creative works. What’s more, you can export them into individual files and import them into other softwares such as Adobe Photoshop, GIMP, Krita, Pencil 2D and Clip Studio Paint. Rickrack can run normally on operating systems such as Windows, Linux, and macOS.
         
-        [:rocket: v2.8.27 Update Notes](https://github.com/eigenmiao/Rickrack/releases/tag/v2.8.27)
-        
         [:house: Rickrack](https://eigenmiao.com/rickrack)
         
         [:arrow_down: Translations of the Introduction in Other Languages :arrow_down:](#introduction-translations)
         
         # 焰火十二卷
         在数字创意的时代，调色板成为了设计师不可或缺的工具。一个好的调色板可以让设计更加有吸引力和协调性。如果你正在寻找一款优秀的调色板软件，那就试试焰火十二卷吧！焰火十二卷具有多种配色功能，适用于多种场景。焰火十二卷简单易上手，更重要的是，它完全免费，无需联网或注册。
         
-        焰火十二卷（实时色彩工具箱）是一款免费且实用的色彩编辑器。它可以帮助你从色轮或者其他地方生成一组和谐的色彩。你可以将这些色彩分享给其他人，或者应用到你自己的创作当中。此外，你也可以将色彩组或者色库导出为单独的色彩文档并导入其他软件中（如 Adobe Photoshop、GIMP、Krita、Pencil 2D 以及优动漫 Paint 等）。焰火十二卷可以在 Windows、Linux、macOS 等操作系统上正常运行。
-        
-        [:rocket: v2.8.27 更新说明](https://github.com/eigenmiao/Rickrack/releases/tag/v2.8.27)
+        焰火十二卷（实时色彩工具箱）是一款免费且实用的色彩编辑器。它可以帮助你从色轮或者其他地方生成一组和谐的色彩。你可以将这些色彩分享给其他人，或者应用到你自己的创作当中。此外，你也可以将色彩组或者色彩仓库导出为单独的色彩文档并导入其他软件中（如 Adobe Photoshop、GIMP、Krita、Pencil 2D 以及优动漫 Paint 等）。焰火十二卷可以在 Windows、Linux、macOS 等操作系统上正常运行。
         
         [:house: 焰火十二卷](https://eigenmiao.com/yanhuo)
         
         [:arrow_down: 简介的其他语言翻译 :arrow_down:](#introduction-translations)
         
         # Table of Content
         * [Introduction Translations](#introduction-translations)
@@ -199,24 +195,24 @@
         * [:hugs: 本征喵函数 @ 爱发电](https://afdian.net/a/eigenmiao)
         * [:hugs: Eigenmiao @ Ko-fi](https://ko-fi.com/eigenmiao)
         
         <div align="right"><a href="#table-of-content">:arrow_up: Back to TOC  :arrow_up:</a></div>
         
         # Installation
         ## Current Release
-        The latest preview version is [v2.8.27](https://github.com/eigenmiao/Rickrack/releases/tag/v2.8.27).
+        The latest preview version is [v2.8.5](https://github.com/eigenmiao/Rickrack/releases/tag/v2.8.5).
         
         ## Install Software
         ### Recommend: Install on Windows 10 or 11 via WinGet tool
         ```
         winget install rickrack
         ```
         
         ## Install on other platforms
-        Download Software from [Github](https://github.com/eigenmiao/Rickrack/releases/tag/v2.8.27) or [Sourceforge](https://sourceforge.net/projects/rickrack/files/v2.8.27/). The installation steps are presented in [tutorials](https://eigenmiao.com/2021/12/12/rickrack-tutorial-en-v2.3.4/#Installation).
+        Download Software from [Github](https://github.com/eigenmiao/Rickrack/releases/tag/v2.8.5) or [Sourceforge](https://sourceforge.net/projects/rickrack/files/v2.8.5/). The installation steps are presented in [tutorials](https://eigenmiao.com/2021/12/12/rickrack-tutorial-en-v2.3.4/#Installation).
         
         Here is a [video tutorial](https://www.bilibili.com/video/BV17r4y1L7R6/).
         
         ## Install Module
         Install the latest [Rickrack](https://pypi.org/project/Rickrack/) from PyPI!
         
         ```Bash
@@ -229,24 +225,24 @@
         
         <div align="right"><a href="#table-of-content">:arrow_up: Back to TOC  :arrow_up:</a></div>
         
         # Usage
         ## How to Use the Software
         Visit https://eigenmiao.com/rickrack/ for tutorials. Just feel free to click anywhere in the interface!
         
-        Here is a [video tutorial](https://www.bilibili.com/video/BV1BM411L75t/).
+        Here is a [video tutorial](https://www.bilibili.com/video/BV17L4y1A7P9/).
         
-        Here is a [demo](https://eigenmiao.com/2023/01/29/color-palette-generator-rickrack-en/).
+        Here is a [demo](https://eigenmiao.com/2023/01/29/rickrack-alternative-to-adobe-color-en/).
         
         ## How to Use the Module
         Include Rickrack in other Python scripts, programs and softwares!
         
         Here is a [video tutorial](https://www.bilibili.com/video/BV1VD4y157tX/).
         
-        Here is a [demo](demo/03_plot_scripts).
+        Here is a [demo](demo/).
         
         ```Python
         # Use Rickrack module in code.
         # This code fragment could be reused.
         
         from rickrack import Rickrack
         
@@ -258,14 +254,18 @@
         dp_argv = dict()
         dp_argv["help"] = True
         
         # Run and see the full contents and examples.
         rr.run(dp_argv=dp_argv, dp_proj=dp_proj)
         ```
         
+        ## Notice
+        * Please read the documents and tutorials when you encounter any difficulties.
+        * The socket server is designed for obtaining colors from the Rickrack software in real-time. By default, this server is disabled and can only be started from the command line.
+        
         <div align="right"><a href="#table-of-content">:arrow_up: Back to TOC  :arrow_up:</a></div>
         
         # Development
         ## Install Requirement
         * Python 3.6
         * Git version control system
         * Additional modules listed in requirements folder
@@ -274,22 +274,19 @@
         ```bash
         # Download the Rickrack source code.
         git clone https://github.com/eigenmiao/Rickrack.git
         
         # Change into the directory.
         cd Rickrack
         
-        # Install the Rickrack starter.
-        pip install rickrack
-        
-        # Display the help information.
-        rickrack -h
-        
         # Run Rickrack.
-        rickrack
+        python src/main/python/main.py
+        
+        # Generate the installer for Rickrack.
+        fbs freeze && fbs installer
         ```
         
         ## How to Build the Module
         ```bash
         # Download the Rickrack source code.
         git clone https://github.com/eigenmiao/Rickrack.git
         
@@ -303,21 +300,24 @@
         <div align="right"><a href="#table-of-content">:arrow_up: Back to TOC  :arrow_up:</a></div>
         
         # Copyright
         Copyright (c) 2019-2023 [Eigenmiao](mailto:eigenmiao@outlook.com). All Rights Reserved.
         
         <div align="right"><a href="#table-of-content">:arrow_up: Back to TOC  :arrow_up:</a></div>
         
+        # Contributing
+        This project welcomes contributions of all types. Recommending Rickrack to people you know, writing reviews for Rickrack on websites, help spec'ing, design, documentation, finding bugs, etc. can all help the project grow better.
+        
         # License
         ## License for Rickrack
         Rickrack is a free software, which is distributed in the hope that it will be useful, but without any warranty. You can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation. See the [GNU General Public License 3.0 (GPL 3.0)](https://www.gnu.org/licenses/) for more details.
         
         All images, documents and translations in Rickrack [code repository](https://github.com/eigenmiao/Rickrack) are licensed under [Creative Commons Attribution-NonCommercial-ShareAlike License 4.0 (CC BY-NC-SA 4.0)](https://creativecommons.org/licenses/by-nc-sa/4.0/) unless stating additionally.
         
-        Rickrack default uses [LXGW WenKai](https://github.com/lxgw/LxgwWenKai) font for interface display, which is an open-source Chinese font derived from Fontworks' Klee One. This font is open-sourced under [SIL Open Font License 1.1](http://scripts.sil.org/OFL).
+        Rickrack default uses [Noto Serif](https://fonts.google.com/specimen/Noto+Serif) ([SC](https://fonts.google.com/specimen/Noto+Serif+SC)) fonts and [Noto Sans](https://fonts.google.com/specimen/Noto+Sans) ([SC](https://fonts.google.com/specimen/Noto+Sans+SC)) fonts for interface display, which are designed by Google and published in website [Google Fonts](https://fonts.google.com/). These fonts are open-sourced under [Apache 2.0](http://www.apache.org/licenses/) and [SIL Open Font License 1.1](http://scripts.sil.org/OFL), respectively.
         
         ## License for Required Packages
         | Package        | Version  | License          |
         |----------------|----------|------------------|
         | altgraph       | 0.17.2   | MIT              |
         | fbs            | 0.8.9    | GPLv3 or Later   |
         | future         | 0.18.2   | MIT              |
@@ -335,43 +335,36 @@
         | ricore         | 0.0.0    | Not Open-sourced |
         | setuptools     | 40.6.2   | MIT              |
         | swatch         | 0.4.0    | MIT              |
         
         <div align="right"><a href="#table-of-content">:arrow_up: Back to TOC  :arrow_up:</a></div>
         
         # More Information
-        * Documentation: https://eigenmiao.com/2021/12/12/rickrack-tutorial-en-v2.3.4/ .
-        * The installation package can be unzipped and run directly. This method does not require administrator privileges and can solve some installation failure problems.
-        * The socket server is designed for obtaining colors from the Rickrack software in real-time. By default, this server is disabled and can only be started from the command line.
         * Rickrack is written in [Python](https://www.python.org/), constructed based on [PyQt5](https://www.qt.io/qt-for-python) and packed up by [fbs (free edition)](https://build-system.fman.io/).
         * The code repository of Rickrack is deposited on [Github](https://github.com/eigenmiao/Rickrack) and [Gitee](https://gitee.com/eigenmiao/Rickrack).
         * The localization (l10n) and internationalization (i18n) of Rickrack is based on [Google Translate](https://translate.google.cn/) and [Microsoft Translator](https://cn.bing.com/translator), deployed on [POEditor](https://poeditor.com/join/project?hash=kBeQjfxCES).
         * The cover image uses images from [Pixabay, which is created by martynaszulist](https://pixabay.com/zh/photos/pattern-the-palette-web-1508277/).
         * In some demo animations, [images of Ghibli](https://www.ghibli.jp/info/013409/) were used.
-        
-        <div align="right"><a href="#table-of-content">:arrow_up: Back to TOC  :arrow_up:</a></div>
-        
-        # Contributing
-        This project welcomes contributions of all types. If you want to contribute code (new features, or bug fixes) to this project, please contact me first. Thanks.
+        * The interface display in demo animations uses the [LXGWWenKai font](https://lxgw.github.io/2021/01/28/Klee-Simpchin/).
         
         <div align="right"><a href="#table-of-content">:arrow_up: Back to TOC  :arrow_up:</a></div>
         
         # Acknowledgment
-        ## Reviews
+        ## Publicity & Promotion
         <table>
           <tbody>
             <tr>
             <td align="center" valign="top" width="20%"><a href="https://www.youtube.com/watch?v=OUnktTCtv3E"><img src="https://yt3.googleusercontent.com/ytc/AGIKgqPSY98ka46AxjcUBDDntl1NHA8lL4PFMZt6g75TFA=s176-c-k-c0x00ffffff-no-rj" width="90px;"/><br /><sub><b>TJ&nbsp;FREE@Youtube</b></sub></a></td>
             <td align="center" valign="top" width="20%"><a href="https://www.softpedia.com/get/Multimedia/Graphic/Graphic-Others/RickRack.shtml"><img src="https://cdnssl.softpedia.com/_img/editors/Robert%20Condorache.jpg?v=2020" width="90px;"/><br /><sub><b>Robert&nbsp;Condorache@Softpedia</b></sub></a></td>
             <td align="center" valign="top" width="20%"><a href="https://sspai.com/u/eigenmiao/updates"><img src="https://cdn.sspai.com/2023/01/14/eab0a38256bc3a045f8d5bf76dd30072.png?imageMogr2/auto-orient/quality/95/thumbnail/!200x200r/gravity/Center/crop/200x200/interlace/1" width="90px;"/><br /><sub><b>本征喵函数@少数派</b></sub></a></td>
             </tr>
           </tbody>
         </table>
         
-        ## Translators
+        ## l10n & i18n
         <table>
           <tbody>
             <tr>
             <td align="center" valign="top" width="20%"><a href="https://poeditor.com/join/project?hash=kBeQjfxCES"><img src="https://avatars.githubusercontent.com/u/59333735?v=4" width="90px;"/><br /><sub><b>Eigenmiao@POEditor</b></sub></a></td>
             </tr>
           </tbody>
         </table>
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
-Metadata-Version: 2.1 Name: Rickrack Version: 2.8.27 Summary: Generate
-harmonious colors freely. Home-page: https://eigenmiao.com/rickrack/ Author:
-Eigenmiao Author-email: eigenmiao@outlook.com License: UNKNOWN Description:
+Metadata-Version: 2.1 Name: Rickrack Version: 2.8.5 Summary: Generate
+harmonious colors freely. Home-page: https://eigenmiao.github.io/rickrack/
+Author: Eigenmiao Author-email: eigenmiao@outlook.com License: UNKNOWN
+Description:
                                   [Rickrack]
 
                                    Rickrack
                                 ç°ç«åäºå·
                ----- ----- ----- ----- ----- ----- ----- -----
                       Generate Harmonious Colors Freely.
                       èªç±èªå¨çæåè°è²å½©ã
@@ -22,62 +23,59 @@
 importantly, it's completely free without networking or registration required.
 Rickrack (**R**e**a**l-t**i**me **C**olor **K**it) is a free and user-friendly
 color editor. It is designed to generate a set of harmonious colors from the
 color wheel or other places. You can share these colors with your friends, or
 apply them into your creative works. Whatâs more, you can export them into
 individual files and import them into other softwares such as Adobe Photoshop,
 GIMP, Krita, Pencil 2D and Clip Studio Paint. Rickrack can run normally on
-operating systems such as Windows, Linux, and macOS. [:rocket: v2.8.27 Update
-Notes](https://github.com/eigenmiao/Rickrack/releases/tag/v2.8.27) [:house:
-Rickrack](https://eigenmiao.com/rickrack) [:arrow_down: Translations of the
-Introduction in Other Languages :arrow_down:](#introduction-translations) #
-ç°ç«åäºå·
+operating systems such as Windows, Linux, and macOS. [:house: Rickrack](https:/
+/eigenmiao.com/rickrack) [:arrow_down: Translations of the Introduction in
+Other Languages :arrow_down:](#introduction-translations) # ç°ç«åäºå·
 å¨æ°å­åæçæ¶ä»£ï¼è°è²æ¿æä¸ºäºè®¾è®¡å¸ä¸å¯æç¼ºçå·¥å·ãä¸ä¸ªå¥½çè°è²æ¿å¯ä»¥è®©è®¾è®¡æ´å æå¸å¼åååè°æ§ãå¦æä½ æ­£å¨å¯»æ¾ä¸æ¬¾ä¼ç§çè°è²æ¿è½¯ä»¶ï¼é£å°±è¯è¯ç°ç«åäºå·å§ï¼ç°ç«åäºå·å·æå¤ç§éè²åè½ï¼éç¨äºå¤ç§åºæ¯ãç°ç«åäºå·ç®åæä¸æï¼æ´éè¦çæ¯ï¼å®å®å¨åè´¹ï¼æ éèç½ææ³¨åã
-ç°ç«åäºå·ï¼å®æ¶è²å½©å·¥å·ç®±ï¼æ¯ä¸æ¬¾åè´¹ä¸å®ç¨çè²å½©ç¼è¾å¨ãå®å¯ä»¥å¸®å©ä½ ä»è²è½®æèå¶ä»å°æ¹çæä¸ç»åè°çè²å½©ãä½ å¯ä»¥å°è¿äºè²å½©åäº«ç»å¶ä»äººï¼æèåºç¨å°ä½ èªå·±çåä½å½ä¸­ãæ­¤å¤ï¼ä½ ä¹å¯ä»¥å°è²å½©ç»æèè²åºå¯¼åºä¸ºåç¬çè²å½©ææ¡£å¹¶å¯¼å¥å¶ä»è½¯ä»¶ä¸­ï¼å¦
+ç°ç«åäºå·ï¼å®æ¶è²å½©å·¥å·ç®±ï¼æ¯ä¸æ¬¾åè´¹ä¸å®ç¨çè²å½©ç¼è¾å¨ãå®å¯ä»¥å¸®å©ä½ ä»è²è½®æèå¶ä»å°æ¹çæä¸ç»åè°çè²å½©ãä½ å¯ä»¥å°è¿äºè²å½©åäº«ç»å¶ä»äººï¼æèåºç¨å°ä½ èªå·±çåä½å½ä¸­ãæ­¤å¤ï¼ä½ ä¹å¯ä»¥å°è²å½©ç»æèè²å½©ä»åºå¯¼åºä¸ºåç¬çè²å½©ææ¡£å¹¶å¯¼å¥å¶ä»è½¯ä»¶ä¸­ï¼å¦
 Adobe PhotoshopãGIMPãKritaãPencil 2D ä»¥åä¼å¨æ¼« Paint
 ç­ï¼ãç°ç«åäºå·å¯ä»¥å¨ WindowsãLinuxãmacOS
-ç­æä½ç³»ç»ä¸æ­£å¸¸è¿è¡ã [:rocket: v2.8.27 æ´æ°è¯´æ](https://
-github.com/eigenmiao/Rickrack/releases/tag/v2.8.27) [:house: ç°ç«åäºå·]
-(https://eigenmiao.com/yanhuo) [:arrow_down: ç®ä»çå¶ä»è¯­è¨ç¿»è¯ :
-arrow_down:](#introduction-translations) # Table of Content * [Introduction
-Translations](#introduction-translations) * [Features](#features) * [Demo]
-(#demo) * [Basic Functions](#basic-functions) * [Reference Colors](#reference-
-colors) * [Color Palettes](#color-palettes) * [Export and Import Colors]
-(#export-and-import-colors) * [Languages and Settings](#languages-and-settings)
-* [Reviews about Rickrack](#reviews-about-rickrack) * [Information]
-(#information) * [Website](#website) * [Repository](#repository) * [Author]
-(#author) * [Support](#support) * [Installation](#installation) * [Current
-Release](#current-release) * [Download Software](#download-software) * [Install
-Software](#install-software) * [Install Module](#install-module) * [Usage]
-(#usage) * [How to Use the Software](#how-to-use-the-software) * [How to Use
-the Module](#how-to-use-the-module) * [Development](#development) * [Install
-Requirement](#install-requirement) * [How to Build the Software](#how-to-build-
-the-software) * [How to Build the Module](#how-to-build-the-module) *
-[Copyright](#copyright) * [License](#license) * [License for Rickrack]
-(#license-for-rickrack) * [License for Required Packages](#license-for-
-required-packages) * [More Information](#more-information) * [Acknowledgment]
-(#acknowledgment) # Introduction Translations ## Rickrack (Esperanto) En la
-epoko de cifereca kreemo, la kolora paletro fariÄis nemalhavebla ilo por
-dezajnistoj. Bona kolora paletro povas fari dezajnon pli alloga kaj
-kunordigita. Rickrack estas desegnita por vi, se vi serÄas bonegan programaron
-de kolora paletro! Rickrack havas diversajn kolorajn miksajn funkciojn kaj
-taÅ­gas por diversaj scenoj. Rickrack estas facile uzebla, kaj pli grave, Äi
-estas tute senpaga sen interkonektado aÅ­ registriÄo necesa. Rickrack estas
-senpaga kaj amika kolorredaktilo. Äi estas desegnita por generi aron da
-harmoniaj koloroj de la kolorrado aÅ­ aliaj lokoj. Vi povas dividi Äi tiujn
-kolorojn kun viaj amikoj, aÅ­ apliki ilin en viajn kreajn verkojn. Krome, vi
-povas eksporti ilin en individuajn dosierojn kaj importi ilin en aliajn
-programojn kiel Adobe Photoshop, GIMP, Krita, Pencil 2D kaj Clip Studio Paint.
-Rickrack povas funkcii normale per operaciumoj kiel Vindozo, Linukso kaj macOS.
-(Tradukoj supre baziÄas sur Google Translate.) [:house: Rickrack](https://
-eigenmiao.com/yanhuo/eo.html) ## Rickrack (Ð ÑÑÑÐºÐ¸Ð¹) Ð Ð²ÐµÐº
-ÑÐ¸ÑÑÐ¾Ð²Ð¾Ð³Ð¾ ÑÐ²Ð¾ÑÑÐµÑÑÐ²Ð° ÑÐ²ÐµÑÐ¾Ð²Ð°Ñ Ð¿Ð°Ð»Ð¸ÑÑÐ°
-ÑÑÐ°Ð»Ð° Ð½ÐµÐ·Ð°Ð¼ÐµÐ½Ð¸Ð¼ÑÐ¼ Ð¸Ð½ÑÑÑÑÐ¼ÐµÐ½ÑÐ¾Ð¼ Ð´Ð»Ñ
-Ð´Ð¸Ð·Ð°Ð¹Ð½ÐµÑÐ¾Ð². Ð¥Ð¾ÑÐ¾ÑÐ°Ñ ÑÐ²ÐµÑÐ¾Ð²Ð°Ñ Ð¿Ð°Ð»Ð¸ÑÑÐ° Ð¼Ð¾Ð¶ÐµÑ
-ÑÐ´ÐµÐ»Ð°ÑÑ Ð´Ð¸Ð·Ð°Ð¹Ð½ Ð±Ð¾Ð»ÐµÐµ Ð¿ÑÐ¸Ð²Ð»ÐµÐºÐ°ÑÐµÐ»ÑÐ½ÑÐ¼ Ð¸
+ç­æä½ç³»ç»ä¸æ­£å¸¸è¿è¡ã [:house: ç°ç«åäºå·](https://
+eigenmiao.com/yanhuo) [:arrow_down: ç®ä»çå¶ä»è¯­è¨ç¿»è¯ :arrow_down:]
+(#introduction-translations) # Table of Content * [Introduction Translations]
+(#introduction-translations) * [Features](#features) * [Demo](#demo) * [Basic
+Functions](#basic-functions) * [Reference Colors](#reference-colors) * [Color
+Palettes](#color-palettes) * [Export and Import Colors](#export-and-import-
+colors) * [Languages and Settings](#languages-and-settings) * [Reviews about
+Rickrack](#reviews-about-rickrack) * [Information](#information) * [Website]
+(#website) * [Repository](#repository) * [Author](#author) * [Support]
+(#support) * [Installation](#installation) * [Current Release](#current-
+release) * [Download Software](#download-software) * [Install Software]
+(#install-software) * [Install Module](#install-module) * [Usage](#usage) *
+[How to Use the Software](#how-to-use-the-software) * [How to Use the Module]
+(#how-to-use-the-module) * [Development](#development) * [Install Requirement]
+(#install-requirement) * [How to Build the Software](#how-to-build-the-
+software) * [How to Build the Module](#how-to-build-the-module) * [Copyright]
+(#copyright) * [License](#license) * [License for Rickrack](#license-for-
+rickrack) * [License for Required Packages](#license-for-required-packages) *
+[More Information](#more-information) * [Acknowledgment](#acknowledgment) #
+Introduction Translations ## Rickrack (Esperanto) En la epoko de cifereca
+kreemo, la kolora paletro fariÄis nemalhavebla ilo por dezajnistoj. Bona
+kolora paletro povas fari dezajnon pli alloga kaj kunordigita. Rickrack estas
+desegnita por vi, se vi serÄas bonegan programaron de kolora paletro! Rickrack
+havas diversajn kolorajn miksajn funkciojn kaj taÅ­gas por diversaj scenoj.
+Rickrack estas facile uzebla, kaj pli grave, Äi estas tute senpaga sen
+interkonektado aÅ­ registriÄo necesa. Rickrack estas senpaga kaj amika
+kolorredaktilo. Äi estas desegnita por generi aron da harmoniaj koloroj de la
+kolorrado aÅ­ aliaj lokoj. Vi povas dividi Äi tiujn kolorojn kun viaj amikoj,
+aÅ­ apliki ilin en viajn kreajn verkojn. Krome, vi povas eksporti ilin en
+individuajn dosierojn kaj importi ilin en aliajn programojn kiel Adobe
+Photoshop, GIMP, Krita, Pencil 2D kaj Clip Studio Paint. Rickrack povas funkcii
+normale per operaciumoj kiel Vindozo, Linukso kaj macOS. (Tradukoj supre
+baziÄas sur Google Translate.) [:house: Rickrack](https://eigenmiao.com/
+yanhuo/eo.html) ## Rickrack (Ð ÑÑÑÐºÐ¸Ð¹) Ð Ð²ÐµÐº ÑÐ¸ÑÑÐ¾Ð²Ð¾Ð³Ð¾
+ÑÐ²Ð¾ÑÑÐµÑÑÐ²Ð° ÑÐ²ÐµÑÐ¾Ð²Ð°Ñ Ð¿Ð°Ð»Ð¸ÑÑÐ° ÑÑÐ°Ð»Ð°
+Ð½ÐµÐ·Ð°Ð¼ÐµÐ½Ð¸Ð¼ÑÐ¼ Ð¸Ð½ÑÑÑÑÐ¼ÐµÐ½ÑÐ¾Ð¼ Ð´Ð»Ñ Ð´Ð¸Ð·Ð°Ð¹Ð½ÐµÑÐ¾Ð².
+Ð¥Ð¾ÑÐ¾ÑÐ°Ñ ÑÐ²ÐµÑÐ¾Ð²Ð°Ñ Ð¿Ð°Ð»Ð¸ÑÑÐ° Ð¼Ð¾Ð¶ÐµÑ ÑÐ´ÐµÐ»Ð°ÑÑ
+Ð´Ð¸Ð·Ð°Ð¹Ð½ Ð±Ð¾Ð»ÐµÐµ Ð¿ÑÐ¸Ð²Ð»ÐµÐºÐ°ÑÐµÐ»ÑÐ½ÑÐ¼ Ð¸
 Ð³Ð°ÑÐ¼Ð¾Ð½Ð¸ÑÐ½ÑÐ¼. Rickrack ÑÐ°Ð·ÑÐ°Ð±Ð¾ÑÐ°Ð½ Ð´Ð»Ñ Ð²Ð°Ñ, ÐµÑÐ»Ð¸
 Ð²Ñ Ð¸ÑÐµÑÐµ Ð¾ÑÐ»Ð¸ÑÐ½Ð¾Ðµ Ð¿ÑÐ¾Ð³ÑÐ°Ð¼Ð¼Ð½Ð¾Ðµ Ð¾Ð±ÐµÑÐ¿ÐµÑÐµÐ½Ð¸Ðµ
 Ð´Ð»Ñ ÑÐ²ÐµÑÐ¾Ð²Ð¾Ð¹ Ð¿Ð°Ð»Ð¸ÑÑÑ! Rickrack Ð¸Ð¼ÐµÐµÑ ÑÐ°Ð·Ð»Ð¸ÑÐ½ÑÐµ
 ÑÑÐ½ÐºÑÐ¸Ð¸ ÑÐ¼ÐµÑÐ¸Ð²Ð°Ð½Ð¸Ñ ÑÐ²ÐµÑÐ¾Ð² Ð¸ Ð¿Ð¾Ð´ÑÐ¾Ð´Ð¸Ñ Ð´Ð»Ñ
 ÑÐ°Ð·Ð»Ð¸ÑÐ½ÑÑ ÑÑÐµÐ½. Rickrack Ð¿ÑÐ¾ÑÑ Ð² Ð¸ÑÐ¿Ð¾Ð»ÑÐ·Ð¾Ð²Ð°Ð½Ð¸Ð¸
 Ð¸, ÑÑÐ¾ Ð±Ð¾Ð»ÐµÐµ Ð²Ð°Ð¶Ð½Ð¾, ÑÐ¾Ð²ÐµÑÑÐµÐ½Ð½Ð¾ Ð±ÐµÑÐ¿Ð»Ð°ÑÐµÐ½, Ð½Ðµ
 ÑÑÐµÐ±ÑÐµÑ Ð¿Ð¾Ð´ÐºÐ»ÑÑÐµÐ½Ð¸Ñ Ðº ÑÐµÑÐ¸ Ð¸Ð»Ð¸
@@ -213,104 +211,107 @@
                                               :arrow_up:_Back_to_TOC_:arrow_up:
 # Information ## Website https://eigenmiao.com/rickrack ## Repository https://
 github.com/eigenmiao/Rickrack ## Author [Eigenmiao](mailto:
 eigenmiao@outlook.com) ## Support Support the continuous development of
 Rickrack! * [:hugs: æ¬å¾åµå½æ° @ ç±åçµ](https://afdian.net/a/
 eigenmiao) * [:hugs: Eigenmiao @ Ko-fi](https://ko-fi.com/eigenmiao)
                                               :arrow_up:_Back_to_TOC_:arrow_up:
-# Installation ## Current Release The latest preview version is [v2.8.27]
-(https://github.com/eigenmiao/Rickrack/releases/tag/v2.8.27). ## Install
-Software ### Recommend: Install on Windows 10 or 11 via WinGet tool ``` winget
-install rickrack ``` ## Install on other platforms Download Software from
-[Github](https://github.com/eigenmiao/Rickrack/releases/tag/v2.8.27) or
-[Sourceforge](https://sourceforge.net/projects/rickrack/files/v2.8.27/). The
-installation steps are presented in [tutorials](https://eigenmiao.com/2021/12/
-12/rickrack-tutorial-en-v2.3.4/#Installation). Here is a [video tutorial]
-(https://www.bilibili.com/video/BV17r4y1L7R6/). ## Install Module Install the
-latest [Rickrack](https://pypi.org/project/Rickrack/) from PyPI! ```Bash #
-Install Rickrack. pip install Rickrack # Start the installed software. rickrack
--d "/PATH/TO/RICKRACK/SOFTWARE" ```
+# Installation ## Current Release The latest preview version is [v2.8.5](https:
+//github.com/eigenmiao/Rickrack/releases/tag/v2.8.5). ## Install Software ###
+Recommend: Install on Windows 10 or 11 via WinGet tool ``` winget install
+rickrack ``` ## Install on other platforms Download Software from [Github]
+(https://github.com/eigenmiao/Rickrack/releases/tag/v2.8.5) or [Sourceforge]
+(https://sourceforge.net/projects/rickrack/files/v2.8.5/). The installation
+steps are presented in [tutorials](https://eigenmiao.com/2021/12/12/rickrack-
+tutorial-en-v2.3.4/#Installation). Here is a [video tutorial](https://
+www.bilibili.com/video/BV17r4y1L7R6/). ## Install Module Install the latest
+[Rickrack](https://pypi.org/project/Rickrack/) from PyPI! ```Bash # Install
+Rickrack. pip install Rickrack # Start the installed software. rickrack -d "/
+PATH/TO/RICKRACK/SOFTWARE" ```
                                               :arrow_up:_Back_to_TOC_:arrow_up:
 # Usage ## How to Use the Software Visit https://eigenmiao.com/rickrack/ for
 tutorials. Just feel free to click anywhere in the interface! Here is a [video
-tutorial](https://www.bilibili.com/video/BV1BM411L75t/). Here is a [demo]
-(https://eigenmiao.com/2023/01/29/color-palette-generator-rickrack-en/). ## How
-to Use the Module Include Rickrack in other Python scripts, programs and
+tutorial](https://www.bilibili.com/video/BV17L4y1A7P9/). Here is a [demo]
+(https://eigenmiao.com/2023/01/29/rickrack-alternative-to-adobe-color-en/). ##
+How to Use the Module Include Rickrack in other Python scripts, programs and
 softwares! Here is a [video tutorial](https://www.bilibili.com/video/
-BV1VD4y157tX/). Here is a [demo](demo/03_plot_scripts). ```Python # Use
-Rickrack module in code. # This code fragment could be reused. from rickrack
-import Rickrack # Init Rickrack. rr = Rickrack() # Display the help
-information. dp_proj = "/PATH/TO/RICKRACK/PROJECT" dp_argv = dict() dp_argv
-["help"] = True # Run and see the full contents and examples. rr.run
-(dp_argv=dp_argv, dp_proj=dp_proj) ```
+BV1VD4y157tX/). Here is a [demo](demo/). ```Python # Use Rickrack module in
+code. # This code fragment could be reused. from rickrack import Rickrack #
+Init Rickrack. rr = Rickrack() # Display the help information. dp_proj = "/
+PATH/TO/RICKRACK/PROJECT" dp_argv = dict() dp_argv["help"] = True # Run and see
+the full contents and examples. rr.run(dp_argv=dp_argv, dp_proj=dp_proj) ``` ##
+Notice * Please read the documents and tutorials when you encounter any
+difficulties. * The socket server is designed for obtaining colors from the
+Rickrack software in real-time. By default, this server is disabled and can
+only be started from the command line.
                                               :arrow_up:_Back_to_TOC_:arrow_up:
 # Development ## Install Requirement * Python 3.6 * Git version control system
 * Additional modules listed in requirements folder ## How to Build the Software
 ```bash # Download the Rickrack source code. git clone https://github.com/
-eigenmiao/Rickrack.git # Change into the directory. cd Rickrack # Install the
-Rickrack starter. pip install rickrack # Display the help information. rickrack
--h # Run Rickrack. rickrack ``` ## How to Build the Module ```bash # Download
-the Rickrack source code. git clone https://github.com/eigenmiao/Rickrack.git #
+eigenmiao/Rickrack.git # Change into the directory. cd Rickrack # Run Rickrack.
+python src/main/python/main.py # Generate the installer for Rickrack. fbs
+freeze && fbs installer ``` ## How to Build the Module ```bash # Download the
+Rickrack source code. git clone https://github.com/eigenmiao/Rickrack.git #
 Change into the directory. cd Rickrack # Generate the package for Rickrack.
 python setup.py sdist --formats=gztar,zip ```
                                               :arrow_up:_Back_to_TOC_:arrow_up:
 # Copyright Copyright (c) 2019-2023 [Eigenmiao](mailto:eigenmiao@outlook.com).
 All Rights Reserved.
                                               :arrow_up:_Back_to_TOC_:arrow_up:
-# License ## License for Rickrack Rickrack is a free software, which is
-distributed in the hope that it will be useful, but without any warranty. You
-can redistribute it and/or modify it under the terms of the GNU General Public
-License as published by the Free Software Foundation. See the [GNU General
-Public License 3.0 (GPL 3.0)](https://www.gnu.org/licenses/) for more details.
-All images, documents and translations in Rickrack [code repository](https://
-github.com/eigenmiao/Rickrack) are licensed under [Creative Commons
-Attribution-NonCommercial-ShareAlike License 4.0 (CC BY-NC-SA 4.0)](https://
-creativecommons.org/licenses/by-nc-sa/4.0/) unless stating additionally.
-Rickrack default uses [LXGW WenKai](https://github.com/lxgw/LxgwWenKai) font
-for interface display, which is an open-source Chinese font derived from
-Fontworks' Klee One. This font is open-sourced under [SIL Open Font License
-1.1](http://scripts.sil.org/OFL). ## License for Required Packages | Package |
-Version | License | |----------------|----------|------------------| | altgraph
-| 0.17.2 | MIT | | fbs | 0.8.9 | GPLv3 or Later | | future | 0.18.2 | MIT | |
-lxml | 4.6.3 | BSD | | macholib | 1.15.2 | MIT | | numpy | 1.19.5 | BSD | |
-pefile | 2021.9.3 | MIT | | Pillow | 8.4.0 | HPND | | pip | 21.3.1 | MIT | |
-PyInstaller | 3.4 | GPLv2 or Later | | PyQt5 | 5.12.1 | GPLv3 | | PyQt5_sip |
+# Contributing This project welcomes contributions of all types. Recommending
+Rickrack to people you know, writing reviews for Rickrack on websites, help
+spec'ing, design, documentation, finding bugs, etc. can all help the project
+grow better. # License ## License for Rickrack Rickrack is a free software,
+which is distributed in the hope that it will be useful, but without any
+warranty. You can redistribute it and/or modify it under the terms of the GNU
+General Public License as published by the Free Software Foundation. See the
+[GNU General Public License 3.0 (GPL 3.0)](https://www.gnu.org/licenses/) for
+more details. All images, documents and translations in Rickrack [code
+repository](https://github.com/eigenmiao/Rickrack) are licensed under [Creative
+Commons Attribution-NonCommercial-ShareAlike License 4.0 (CC BY-NC-SA 4.0)]
+(https://creativecommons.org/licenses/by-nc-sa/4.0/) unless stating
+additionally. Rickrack default uses [Noto Serif](https://fonts.google.com/
+specimen/Noto+Serif) ([SC](https://fonts.google.com/specimen/Noto+Serif+SC))
+fonts and [Noto Sans](https://fonts.google.com/specimen/Noto+Sans) ([SC](https:
+//fonts.google.com/specimen/Noto+Sans+SC)) fonts for interface display, which
+are designed by Google and published in website [Google Fonts](https://
+fonts.google.com/). These fonts are open-sourced under [Apache 2.0](http://
+www.apache.org/licenses/) and [SIL Open Font License 1.1](http://
+scripts.sil.org/OFL), respectively. ## License for Required Packages | Package
+| Version | License | |----------------|----------|------------------| |
+altgraph | 0.17.2 | MIT | | fbs | 0.8.9 | GPLv3 or Later | | future | 0.18.2 |
+MIT | | lxml | 4.6.3 | BSD | | macholib | 1.15.2 | MIT | | numpy | 1.19.5 | BSD
+| | pefile | 2021.9.3 | MIT | | Pillow | 8.4.0 | HPND | | pip | 21.3.1 | MIT |
+| PyInstaller | 3.4 | GPLv2 or Later | | PyQt5 | 5.12.1 | GPLv3 | | PyQt5_sip |
 4.19.19 | SIP | | pywin32 | 302 | PSF | | pywin32-ctypes | 0.2.0 | BSD | |
 ricore | 0.0.0 | Not Open-sourced | | setuptools | 40.6.2 | MIT | | swatch |
 0.4.0 | MIT |
                                               :arrow_up:_Back_to_TOC_:arrow_up:
-# More Information * Documentation: https://eigenmiao.com/2021/12/12/rickrack-
-tutorial-en-v2.3.4/ . * The installation package can be unzipped and run
-directly. This method does not require administrator privileges and can solve
-some installation failure problems. * The socket server is designed for
-obtaining colors from the Rickrack software in real-time. By default, this
-server is disabled and can only be started from the command line. * Rickrack is
-written in [Python](https://www.python.org/), constructed based on [PyQt5]
-(https://www.qt.io/qt-for-python) and packed up by [fbs (free edition)](https:/
-/build-system.fman.io/). * The code repository of Rickrack is deposited on
-[Github](https://github.com/eigenmiao/Rickrack) and [Gitee](https://gitee.com/
-eigenmiao/Rickrack). * The localization (l10n) and internationalization (i18n)
-of Rickrack is based on [Google Translate](https://translate.google.cn/) and
-[Microsoft Translator](https://cn.bing.com/translator), deployed on [POEditor]
-(https://poeditor.com/join/project?hash=kBeQjfxCES). * The cover image uses
-images from [Pixabay, which is created by martynaszulist](https://pixabay.com/
-zh/photos/pattern-the-palette-web-1508277/). * In some demo animations, [images
-of Ghibli](https://www.ghibli.jp/info/013409/) were used.
-                                              :arrow_up:_Back_to_TOC_:arrow_up:
-# Contributing This project welcomes contributions of all types. If you want to
-contribute code (new features, or bug fixes) to this project, please contact me
-first. Thanks.
+# More Information * Rickrack is written in [Python](https://www.python.org/),
+constructed based on [PyQt5](https://www.qt.io/qt-for-python) and packed up by
+[fbs (free edition)](https://build-system.fman.io/). * The code repository of
+Rickrack is deposited on [Github](https://github.com/eigenmiao/Rickrack) and
+[Gitee](https://gitee.com/eigenmiao/Rickrack). * The localization (l10n) and
+internationalization (i18n) of Rickrack is based on [Google Translate](https://
+translate.google.cn/) and [Microsoft Translator](https://cn.bing.com/
+translator), deployed on [POEditor](https://poeditor.com/join/
+project?hash=kBeQjfxCES). * The cover image uses images from [Pixabay, which is
+created by martynaszulist](https://pixabay.com/zh/photos/pattern-the-palette-
+web-1508277/). * In some demo animations, [images of Ghibli](https://
+www.ghibli.jp/info/013409/) were used. * The interface display in demo
+animations uses the [LXGWWenKai font](https://lxgw.github.io/2021/01/28/Klee-
+Simpchin/).
                                               :arrow_up:_Back_to_TOC_:arrow_up:
-# Acknowledgment ## Reviews
+# Acknowledgment ## Publicity & Promotion
       [https://yt3.googleusercontent.com/ytc/        [https://cdnssl.softpedia.com/         [https://cdn.sspai.com/2023/01/14/
 AGIKgqPSY98ka46AxjcUBDDntl1NHA8lL4PFMZt6g75TFA=s176-          _img/editors/          eab0a38256bc3a045f8d5bf76dd30072.png?imageMogr2/
                c-k-c0x00ffffff-no-rj]                Robert%20Condorache.jpg?v=2020]    auto-orient/quality/95/thumbnail/!200x200r/
                   TJ FREE@Youtube                     Robert Condorache@Softpedia      gravity/Center/crop/200x200/interlace/1]
                                                                                                  æ¬å¾åµå½æ°@å°æ°æ´¾
-## Translators
+## l10n & i18n
 [https://avatars.githubusercontent.com/u/59333735?v=4]
                   Eigenmiao@POEditor
 ## Feature Implementation & Bug Fix
 [https://avatars.githubusercontent.com/u/59333735?v=4]
                    Eigenmiao@Github
 ## Software Dependency
           [https://                      [https://                      [https://
```

### Comparing `Rickrack-2.8.27/setup.py` & `Rickrack-2.8.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,21 +14,21 @@
 """
 
 from setuptools import setup
 
 
 setup(
     name="Rickrack",
-    version="2.8.27",
+    version="2.8.5",
     author="Eigenmiao",
     author_email="eigenmiao@outlook.com",
     description="Generate harmonious colors freely.",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
-    url="https://eigenmiao.com/rickrack/",
+    url="https://eigenmiao.github.io/rickrack/",
     classifiers=[
         "Topic :: Multimedia :: Graphics",
         "Topic :: Utilities",
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Programming Language :: Python :: 3",
         "Operating System :: Microsoft :: Windows",
```

