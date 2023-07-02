# Comparing `tmp/maxgradient-0.1.4.tar.gz` & `tmp/maxgradient-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maxgradient-0.1.4.tar", last modified: Thu Jun 22 08:27:24 2023, max compression
+gzip compressed data, was "maxgradient-0.1.5.tar", last modified: Sun Jul  2 03:26:30 2023, max compression
```

## Comparing `maxgradient-0.1.4.tar` & `maxgradient-0.1.5.tar`

### file list

```diff
@@ -1,22 +1,26 @@
--rw-r--r--   0        0        0     1066 2023-05-20 01:18:06.237490 maxgradient-0.1.4/LICENSE
--rw-r--r--   0        0        0     4932 2023-06-22 08:26:27.451481 maxgradient-0.1.4/README.md
--rw-r--r--   0        0        0      735 2023-06-19 17:15:40.456613 maxgradient-0.1.4/maxgradient/__init__.py
--rw-r--r--   0        0        0    10879 2023-06-18 19:16:19.295760 maxgradient-0.1.4/maxgradient/_gradient_substring.py
--rw-r--r--   0        0        0     1886 2023-06-14 20:46:22.513323 maxgradient-0.1.4/maxgradient/_mode.py
--rw-r--r--   0        0        0    16154 2023-06-16 21:20:44.170100 maxgradient-0.1.4/maxgradient/_rich.py
--rw-r--r--   0        0        0    12225 2023-06-16 21:17:22.440850 maxgradient-0.1.4/maxgradient/_x11.py
--rw-r--r--   0        0        0     2395 2023-06-20 03:47:24.996801 maxgradient-0.1.4/maxgradient/cli.py
--rw-r--r--   0        0        0    19133 2023-06-19 01:34:58.510343 maxgradient-0.1.4/maxgradient/color.py
--rw-r--r--   0        0        0     3294 2023-06-16 21:20:58.780049 maxgradient-0.1.4/maxgradient/color_list.py
--rw-r--r--   0        0        0    10462 2023-06-19 00:24:10.378696 maxgradient-0.1.4/maxgradient/console.py
--rw-r--r--   0        0        0    30263 2023-06-16 16:09:50.267902 maxgradient-0.1.4/maxgradient/default_styles.py
--rw-r--r--   0        0        0    20228 2023-06-19 03:17:18.349630 maxgradient-0.1.4/maxgradient/gradient.py
--rw-r--r--   0        0        0    13231 2023-06-18 15:30:08.337049 maxgradient-0.1.4/maxgradient/log.py
--rw-r--r--   0        0        0     1473 2023-06-19 17:26:36.354259 maxgradient-0.1.4/maxgradient/logs/debug.log
--rw-r--r--   0        0        0       87 2023-06-19 17:26:36.354163 maxgradient-0.1.4/maxgradient/logs/info.log
--rw-r--r--   0        0        0     2649 2023-06-18 18:22:16.438034 maxgradient-0.1.4/maxgradient/theme.py
--rw-r--r--   0        0        0      876 2023-06-22 08:27:24.357322 maxgradient-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2284 2023-06-20 04:32:57.158944 maxgradient-0.1.4/tests/test_color.py
--rw-r--r--   0        0        0      658 2023-06-20 04:22:37.208149 maxgradient-0.1.4/tests/test_rich_colors.py
--rw-r--r--   0        0        0      654 2023-06-20 04:18:31.642710 maxgradient-0.1.4/tests/test_x11_colors.py
--rw-r--r--   0        0        0     5484 1970-01-01 00:00:00.000000 maxgradient-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-05-20 01:18:06.237490 maxgradient-0.1.5/LICENSE
+-rw-r--r--   0        0        0     4999 2023-06-30 08:37:31.254788 maxgradient-0.1.5/README.md
+-rw-r--r--   0        0        0      900 2023-07-02 02:42:12.536125 maxgradient-0.1.5/maxgradient/__init__.py
+-rw-r--r--   0        0        0       82 2023-07-02 02:35:25.026917 maxgradient-0.1.5/maxgradient/__main__.py
+-rw-r--r--   0        0        0     5006 2023-07-01 23:02:07.258870 maxgradient-0.1.5/maxgradient/_gc.py
+-rw-r--r--   0        0        0     5209 2023-07-01 20:41:45.226588 maxgradient-0.1.5/maxgradient/_hex.py
+-rw-r--r--   0        0        0    15636 2023-07-01 20:31:12.741523 maxgradient-0.1.5/maxgradient/_log.py
+-rw-r--r--   0        0        0     1199 2023-06-28 08:27:11.422997 maxgradient-0.1.5/maxgradient/_mode.py
+-rw-r--r--   0        0        0     6606 2023-07-01 21:19:47.130657 maxgradient-0.1.5/maxgradient/_rgb.py
+-rw-r--r--   0        0        0    24273 2023-07-01 22:41:07.266394 maxgradient-0.1.5/maxgradient/_rich.py
+-rw-r--r--   0        0        0    18993 2023-07-01 21:26:33.418662 maxgradient-0.1.5/maxgradient/_x11.py
+-rwxr-xr-x   0        0        0     8774 2023-07-02 02:33:13.404361 maxgradient-0.1.5/maxgradient/cli.py
+-rw-r--r--   0        0        0    25708 2023-07-02 02:50:12.928824 maxgradient-0.1.5/maxgradient/color.py
+-rw-r--r--   0        0        0     3282 2023-07-01 21:24:43.063498 maxgradient-0.1.5/maxgradient/color_list.py
+-rw-r--r--   0        0        0    10162 2023-07-02 02:58:22.448387 maxgradient-0.1.5/maxgradient/console.py
+-rw-r--r--   0        0        0    30263 2023-06-16 16:09:50.267902 maxgradient-0.1.5/maxgradient/default_styles.py
+-rw-r--r--   0        0        0    21150 2023-07-01 22:39:37.330449 maxgradient-0.1.5/maxgradient/gradient.py
+-rw-r--r--   0        0        0    14964 2023-07-02 03:23:36.000529 maxgradient-0.1.5/maxgradient/logs/debug.log
+-rw-r--r--   0        0        0     1070 2023-07-02 03:23:35.999211 maxgradient-0.1.5/maxgradient/logs/info.log
+-rw-r--r--   0        0        0     2649 2023-06-18 18:22:16.438034 maxgradient-0.1.5/maxgradient/theme.py
+-rw-r--r--   0        0        0      646 2023-07-02 03:26:30.086912 maxgradient-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     4588 2023-07-01 18:46:15.391524 maxgradient-0.1.5/tests/test_color.py
+-rw-r--r--   0        0        0     2032 2023-07-01 22:55:35.512952 maxgradient-0.1.5/tests/test_gc.py
+-rw-r--r--   0        0        0      658 2023-06-20 04:22:37.208149 maxgradient-0.1.5/tests/test_rich_colors.py
+-rw-r--r--   0        0        0      654 2023-06-20 04:18:31.642710 maxgradient-0.1.5/tests/test_x11_colors.py
+-rw-r--r--   0        0        0     5435 1970-01-01 00:00:00.000000 maxgradient-0.1.5/PKG-INFO
```

### Comparing `maxgradient-0.1.4/LICENSE` & `maxgradient-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `maxgradient-0.1.4/README.md` & `maxgradient-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 <html>
     <head>
         <link href="styles/gradient.css" rel="stylesheet">
     </head>
     <body>
+        <!--MaxGradient Banner-->
         <img src="https://raw.githubusercontent.com/maxludden/maxludden/621fcb611c1e52160d89d33e1441b34948c37752/maxgradient_banner.svg" alt="MaxGradient" width="100%">
+        <!--End of Banner-->
 ​        <div class="badges">
 ​            <a href="https://GitHub.com/maxludden/maxgradient"><img  class="badge" src="https://img.shields.io/badge/Python-3.9 | 3.10 | 3.11-blue?logo=python" alt="PyPI - MaxGradient"></a>
 ​            <a href="https://GitHub.com/maxludden/maxgradient"><img  class="badge" src="https://img.shields.io/badge/PyPI-MaxGradient-blue?" alt="PyPI - MaxGradient"></a>
-​            <a href="https://GitHub.com/maxludden/maxgradient"><img  class="badge" src="https://img.shields.io/badge/Version-0.1.4-bbbbbb" alt="Version - 0.1.3"></a>
+​            <a href="https://GitHub.com/maxludden/maxgradient"><img  class="badge" src="https://img.shields.io/badge/Version-0.1.4-bbbbbb" alt="Version - 0.1.5"></a>
 ​            <a href="https://pdm.fming.dev/"><img class="badge" src="https://camo.githubusercontent.com/acf0526fc1f541f9d980d7983ff5ab8e540cf2136206c2b5dc740f658a37fac0/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f70646d2d6d616e616765642d626c756576696f6c6574"></a>
 ​        </div>
         <!--End of badges-->
 ​        <div class="summary">
             <p><span class="mg">MaxGradient</span> automates the printing gradient colored text to the console. It's built upon the great <a href="https://rich.readthedocs.io/en/latest/introduction.html"> <span class="warm-wipe">rich library</span></a>. It contains a Console that can serve as a drop in replacement for <span class="lightblue-cyan-wipe">rich.rich.Console</span> and has an expanded Color class which can parse X11 color names on top of rich's standard colors. <span class="mg">MaxGradient</span> is a work in progress and I'm open to any suggestions or contributions.</span></p>
         </div>
 ​        <div class="body">
@@ -58,15 +60,15 @@
 
 ```python
 class Gradient(rich.rich.Text):
     """Text with gradient color / style."""
 
     def __init__ (
         ext: Optional[str | Text] = "",
-        colors: Optional[List[Color | Tuple | str]] = None,
+        colors: Optional[str|List[Color | Tuple | str]] = None,
         rainbow: bool = False,
         invert: bool = False,
         hues: Optional[int] = None,
         color_sample: bool = False,
         style: StyleType = Style.null(),
         *,
         # The arguments below are used directly by Text
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-[MaxGradient] â
-â [PyPI_-_MaxGradient] â [PyPI_-_MaxGradient] â [Version_-_0.1.3] â
+ [MaxGradient]  â
+â [PyPI_-_MaxGradient] â [PyPI_-_MaxGradient] â [Version_-_0.1.5] â
 [https://camo.githubusercontent.com/
 acf0526fc1f541f9d980d7983ff5ab8e540cf2136206c2b5dc740f658a37fac0/
 68747470733a2f2f696d672e736869656c64732e696f2f62616467652f70646d2d6d616e616765642d626c756576696f6c6574]
 â
  â
 MaxGradient automates the printing gradient colored text to the console. It's
 built upon the great rich_library. It contains a Console that can serve as a
@@ -20,18 +20,18 @@
 text:
 ```python import maxgradient as mg console = mg.Console() console.gradient
 ("Hello, World!") ``` [Hello, World!] --- ## Gradient
 You may also instantiate a Gradient Object. The Gradient class is a subclass of
 the rich.text.Text class, and can be used in the same way. The Gradient class
 has a few extra arguments available though.
 ```python class Gradient(rich.rich.Text): """Text with gradient color /
-style.""" def __init__ ( ext: Optional[str | Text] = "", colors: Optional[List
-[Color | Tuple | str]] = None, rainbow: bool = False, invert: bool = False,
-hues: Optional[int] = None, color_sample: bool = False, style: StyleType =
-Style.null(), *, # The arguments below are used directly by Text # so I won't
+style.""" def __init__ ( ext: Optional[str | Text] = "", colors: Optional
+[str|List[Color | Tuple | str]] = None, rainbow: bool = False, invert: bool =
+False, hues: Optional[int] = None, color_sample: bool = False, style: StyleType
+= Style.null(), *, # The arguments below are used directly by Text # so I won't
 cover them here. If you have # questions check out the rich documentation.
 justify: Optional[JustifyMethod] = None, overflow: Optional[OverflowMethod] =
 None, no_wrap: Optional[bool] = None, end: str = "\n", tab_size: Optional[int]
 = 8, spans: Optional[List[Span]] = None,) -> None: ``` The Gradient class can
 utilize the above arguments to get a plethora of different gradients. [Gradient
 Examples])
```

### Comparing `maxgradient-0.1.4/maxgradient/_mode.py` & `maxgradient-0.1.5/maxgradient/_mode.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,58 +4,38 @@
 from rich.text import Text
 
 
 class Mode(Enum):
     """A color mode. Used to determine how a color was parsed."""
 
     COLOR = "COLOR"
-    NAMED = "NAMED"
-    X11 = "X11"
-    RICH = "RICH"
+    GC = "GC"
     HEX = "HEX"
+    INIT = "INIT"
+    INVALID = "INVALID"
     RGB = "RGB"
     RGB_TUPLE = "RGB_TUPLE"
-
-    @property
-    def color_mode(self) -> str:
-        """Return the color mode."""
-        if self.value == Mode.COLOR:
-            return str("color")
-        if self.value == Mode.NAMED:
-            return str("named")
-        if self.value == Mode.X11:
-            return str("x11")
-        if self.value == Mode.RICH:
-            return str("rich")
-        if self.value == Mode.HEX:
-            return str("hex")
-        if self.value == Mode.RGB:
-            return str("rgb")
-        if self.value == Mode.RGB_TUPLE:
-            return str("rgb_tuple")
-        raise ValueError(f"Invalid mode: {self}")
+    RICH_COLOR = "RICH_COLOR"
+    RICH = "RICH"
+    X11 = "X11"
 
     def __eq__(self, other: "Mode") -> bool:
         """Return True if the color mode is equal to another."""
         if isinstance(other, Mode):
             return self.value == other.value
         elif isinstance(other, str):
             return self.color_mode == other
         else:
             return False
 
     def __repr__(self) -> str:
         """Return a representation of the color mode."""
         return f"Mode.{str(self.value).upper()}"
 
-    def __rich_repr__(self) -> Text:
+    def __rich__(self) -> Text:
         """Return a rich text representation of the color mode."""
         mode = Text("Mode", style="bold italic #7FD6E8")
         dot = Text(".", style="bold.white")
         value: str = str(self.value).upper()
         formatted_value = Text(value, style="bold lime")
         rich_repr = Text.assemble(mode, dot, formatted_value)
         return rich_repr
-
-    def __rich__(self) -> Text:
-        """Return a rich text representation of the color mode."""
-        return self.__rich_repr__()
```

### Comparing `maxgradient-0.1.4/maxgradient/color_list.py` & `maxgradient-0.1.5/maxgradient/color_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 from itertools import cycle
 from random import randint
 from typing import List
 
 from rich.table import Table
 from rich.text import Text
 
+from maxgradient._log import Log, Console
 from maxgradient.color import Color
-from maxgradient.log import LogConsole, Log
 
-console = LogConsole()
-log = Log(console)
+console = Console()
+log = Log()
 
 
 class ColorList(list):
     """ColorList is a list of colors. It is used to generate a spectrum of\
         colors for use in gradient generation. It consists of a list of\
         `Color` objects."""
```

### Comparing `maxgradient-0.1.4/maxgradient/console.py` & `maxgradient-0.1.5/maxgradient/console.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 """MaxConsole is a custom themed class inheriting from rich.console.Console."""
 # pylint: disable=E0401, R0913, R0914
 import os
 from datetime import datetime
-from typing import IO, Callable, Literal, Mapping, Optional, Union, List, Tuple
+from typing import IO, Callable, List, Literal, Mapping, Optional, Tuple, Union
 
 from rich._log_render import FormatTimeCallable
 from rich.console import Console as RichConsole
 from rich.console import ConsoleRenderable, RichCast
 from rich.emoji import EmojiVariant
 from rich.highlighter import ReprHighlighter
 from rich.panel import Panel
-from rich.style import StyleType, Style
-from rich.text import Text, Span
+from rich.style import Style, StyleType
+from rich.text import Span, Text
 from rich.theme import Theme
 from rich.traceback import install as install_traceback
 
+# from maxgradient.color import Color
+from maxgradient.gradient import Gradient
 from maxgradient.theme import GradientTheme
 from maxgradient.color import Color
-from maxgradient.gradient import Gradient
 
 RenderableType = ConsoleRenderable | RichCast | str
 HighlighterType = Callable[[Union[str, "Text"]], "Text"]
 JustifyMethod = Literal["default", "left", "center", "right", "full"]
 OverflowMethod = Literal["fold", "crop", "ellipsis", "ignore"]
 
 
@@ -66,15 +67,15 @@
         height (int, optional): The height of the terminal. Leave \
             as default to auto-detect height.
         style (StyleType, optional): Style to apply to all output, \
             or None for no style. Defaults to None.
         no_color (Optional[bool], optional): Enabled no color \
             mode, or None to auto detect. Defaults to None.
         tab_size (int, optional): Number of spaces used to replace \
-            a tab character. Defaults to 8.
+            a tab character. Defaults to 4.
         record (bool, optional): Boolean to enable recording of \
             terminal output,
                 required to call export_html, export_svg, and \
                     export_text. Defaults to False.
         markup (bool, optional): Boolean to enable console_markup. \
             Defaults to True.
         emoji (bool, optional): Enable emoji code. Defaults to True.
@@ -118,15 +119,15 @@
         stderr: bool = False,
         file: Optional[IO[str]] = None,
         quiet: bool = False,
         width: Optional[int] = None,
         height: Optional[int] = None,
         style: Optional[StyleType] = None,
         no_color: Optional[bool] = None,
-        tab_size: int = 8,
+        tab_size: int = 4,
         record: bool = False,
         markup: bool = True,
         emoji: bool = True,
         emoji_variant: Optional[EmojiVariant] = None,
         highlight: bool = True,
         log_time: bool = True,
         log_path: bool = True,
@@ -186,74 +187,73 @@
         style: StyleType = Style.null(),
         *,
         justify: Optional[JustifyMethod] = None,
         overflow: Optional[OverflowMethod] = None,
         no_wrap: Optional[bool] = None,
         end: str = "\n",
         tab_size: Optional[int] = 8,
-        spans: Optional[List[Span]] = None) -> None:
+        spans: Optional[List[Span]] = None,
+    ) -> None:
         """Return a gradient used by the console."""
-        console_gradient = Gradient(
-            text=text,
-            colors=colors,
-            rainbow=rainbow,
-            invert=invert,
-            hues=hues,
-            color_sample=color_sample,
-            style=style,
-            justify=justify,
-            overflow=overflow,
-            no_wrap=no_wrap,
-            end=end,
-            tab_size=tab_size,
-            spans=spans
+        self.print(
+            Gradient(
+                text=text,
+                colors=colors,
+                rainbow=rainbow,
+                invert=invert,
+                hues=hues,
+                color_sample=color_sample,
+                style=style,
+                justify=justify,
+                overflow=overflow,
+                no_wrap=no_wrap,
+                end=end,
+                tab_size=tab_size,
+                spans=spans,
+            )
         )
-        self.print(console_gradient)
 
     @staticmethod
-    def formatted_console() -> Text:
+    def get_title() -> Text:
         """Print out `MaxConsole` in a manual gradient"""
-        letters = [
-            Text("Gr", style="bold.blue"),
-            Text("a", style="bold.lightblue"),
-            Text("d", style="bold.cyan"),
-            Text("ie", style="bold.lime"),
-            Text("n", style="bold.yellow"),
-            Text("t", style="bold.orange"),
-            Text("C", style="bold.red"),
-            Text("o", style="bold.lightblue"),
-            Text("n", style="bold.blue"),
-            Text("s", style="bold.purple"),
-            Text("o", style="bold.violet"),
-            Text("l", style="bold.magenta"),
-            Text("e", style="bold.red"),
-        ]
-        return Text.assemble(*letters)
-
+        return Gradient(
+            "GradientConsole",
+            colors=["#5f00ff", "#af00ff", "#ff00ff"],
+            style="bold italic"
+        )
     @classmethod
     def generate_example(cls) -> Text:
         """Generate an explanation of MaxConsole for demonstration."""
-        formatted_console = cls.formatted_console()
-        explanation_text = Text.from_markup(
-            " is a custom themed terminal console class inheriting from \
-[italic bold #00ffff]rich.console.Console[/]. It is a [bold.lightpurple]global singleton \
-[/]class that can be imported and used anywhere in the project and \
-used as a drop in replacement for [italic bold #00ffff]rich.console.Console[/]."
+        rich = Gradient(
+            "rich.console.Console",
+            colors=["#0000ff", "#0044ff", "#1199ff", "#44bbff", "#66ffff"],
+            style="bold italic"
+        )
+        text1 = Text(" is a custom themed terminal console class inheriting from")
+        text2 = Text.from_markup(". It is a [i #66EE35] global singleton [/]class that can be \
+imported and used anywhere in the project and used as a drop in replacement for "
+        )
+        text3 = Text(".")
+        combine_explanation = Text.assemble(
+            cls.get_title(),
+            text1,
+            rich,
+            text2,
+            rich,
+            text3
         )
-        combine_explanation = Text.assemble(formatted_console, explanation_text)
         return combine_explanation
 
 
 if __name__ == "__main__":
     console = Console()
     example = console.generate_example()
-    title = console.formatted_console()
+    title = console.get_title()
     console.line(2)
     console.print(
         Panel(
             example,
-            # title=title,
             width=100,
         ),
         justify="center",
     )
     console.line()
```

### Comparing `maxgradient-0.1.4/maxgradient/default_styles.py` & `maxgradient-0.1.5/maxgradient/default_styles.py`

 * *Files identical despite different names*

### Comparing `maxgradient-0.1.4/maxgradient/gradient.py` & `maxgradient-0.1.5/maxgradient/gradient.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,36 @@
 """Defines the Gradient class which is used to print text with a gradient. \
     It inherits from the Rich Text class."""
 # pylint: disable=W0611,C0103, E0401, C0301
 import re
-from concurrent.futures import Future, ProcessPoolExecutor, as_completed
-from functools import lru_cache
-from multiprocessing import cpu_count
 from typing import List, Optional, Tuple
 
 import numpy as np
-from loguru import logger
 from lorem_text import lorem
+from nptyping import NDArray, Shape
 from numpy import ndarray
-from rich import inspect
-from rich.columns import Columns
-from rich.console import Console, JustifyMethod, OverflowMethod
+from rich.console import JustifyMethod, OverflowMethod
 from rich.control import strip_control_codes
 from rich.layout import Layout
 from rich.panel import Panel
-from rich.pretty import Pretty
 from rich.style import Style, StyleType
-from rich.table import Table
 from rich.text import Span, Text
 
-from maxgradient._gradient_substring import GradientSubstring
+from maxgradient._log import Console, Log
 from maxgradient.color import Color, ColorParseError
 from maxgradient.color_list import ColorList
-from maxgradient.log import Log, LogConsole
+from maxgradient._gc import GradientColor as GC
 from maxgradient.theme import GradientTheme
 
 DEFAULT_JUSTIFY: "JustifyMethod" = "default"
 DEFAULT_OVERFLOW: "OverflowMethod" = "fold"
 WHITESPACE_REGEX = re.compile(r"^\s+$")
 VERBOSE: bool = False
-console = LogConsole()
-log = Log(console=console)
+console = Console()
+log = Log()
 
 
 class Gradient(Text):
     """Text with gradient color / style.
 
         Args:
             text(`text): The text to print. Defaults to `""`.\n
@@ -58,21 +51,21 @@
                 Defaults to None.\n
             tab_size (int): Number of spaces per tab, or `None` to use `console.tab_size`.\
                 Defaults to 8.\n
             spans (List[Span], optional). A list of predefined style spans. Defaults to None.\n
 
     """
 
-    __slots__ = ["colors", "_color_sample", "_hues", "_style"]
+    __slots__ = ["colors", "_color_sample", "_hues", "_style", "_color_sample"]
 
     # @snoop(watch=("gradient_spans", "substrings"))
     def __init__(
         self,
         text: Optional[str | Text] = "",
-        colors: Optional[List[Color | Tuple | str]] = None,
+        colors: Optional[List[Color | Tuple | str] | str] = None,
         rainbow: bool = False,
         invert: bool = False,
         hues: Optional[int] = None,
         color_sample: bool = False,
         style: StyleType = Style.null(),
         *,
         justify: Optional[JustifyMethod] = None,
@@ -104,18 +97,18 @@
             tab_size (int): Number of spaces per tab, or `None` to use `console.tab_size`.\
                 Defaults to 8.\n
             spans (List[Span], optional). A list of predefined style spans. Defaults to None.\n
 
     """
 
         if isinstance(text, Text):
-            self._spans: List[Span] = text.spans
+            self._spans = text.spans
             text = strip_control_codes(text.plain)
         else:
-            self._spans = spans
+            self._spans = spans  # type: ignore
         assert isinstance(text, str), f"Text must be a string or Text, not {type(text)}"
         self._text: str = text
         self._length: int = len(text)
 
         super().__init__(
             text=text,
             style=style,
@@ -135,52 +128,82 @@
 
         gradient_substring: Text = self.generate_substrings()
         console.line(2)
         self._spans = gradient_substring.spans
 
     # @snoop(watch_explode=["colors", "self.colors"])
     def get_colors(
-        self, colors: Optional[List[Color | Tuple | str]], rainbow: bool, invert: bool
+        self,
+        colors: Optional[str | List[Color | Tuple | str]],
+        rainbow: bool,
+        invert: bool,
     ) -> List[Color]:
         """Get the colors for the gradient.
 
         Args:
             colors(`List[Optional[Color|Tuple|str|int]]`): A list of colors to use \
                 for the gradient. Defaults to None.\n
             rainbow(`bool`): Whether to print the gradient text in rainbow colors across \
                 the spectrum. Defaults to False.\n
             invert(`bool`): Reverse the color gradient. Defaults to False.\n
             verbose(`bool`): Whether to print verbose output. Defaults to True.\n
 
         Returns:
             List[Color]: A list of colors for the gradient.
         """
-        if rainbow:
-            self.hues = 10
-            color_list = ColorList(self.hues, invert).color_list
-            colors_ = color_list
-            if self.validate_colors(colors_):
-                return colors_
+        if isinstance(colors, str):
+            return self.mono(colors)
         else:
-            if colors is not None:
-                colors_: List[Color] = []
-                for color in colors:
-                    try:
-                        color = Color(color)
-                        colors_.append(color)
-                    except ColorParseError as error:
-                        raise ColorParseError(f"Can't parse color: {color}") from error
-                if self.validate_colors(colors_):
-                    return colors_
-            else:
+            if rainbow:
+                self.hues = 10
                 color_list = ColorList(self.hues, invert).color_list
-                colors_ = color_list[: self.hues]
+                colors_ = color_list
                 if self.validate_colors(colors_):
                     return colors_
 
+            else:
+                if colors is not None:
+                    colors_: List[Color] = []
+                    for color in colors:
+                        try:
+                            color = Color(color)
+                            colors_.append(color)
+                        except ColorParseError as error:
+                            raise ColorParseError(
+                                f"Can't parse color: {color}"
+                            ) from error
+                    if self.validate_colors(colors_):
+                        return colors_
+                else:
+                    color_list = ColorList(self.hues, invert).color_list
+                    colors_ = color_list[: self.hues]
+                    if self.validate_colors(colors_):
+                        return colors_
+
+    def mono(self, color: str | Color) -> List[Color]:
+        """Create a list of monochromatic hues from a color.
+
+        Args:
+            color (str|Color): The color to generate monochromatic hues from.
+        """
+        log.debug(f"Called Gradient.mono({color})")
+        if isinstance(color, str):
+            try:
+                color = Color(color)
+            except ColorParseError as cpe:
+                raise ColorParseError(f"Could not parse color: {color}") from cpe
+            else:
+                return [
+                    # Color(color.darken(0.4)),
+                    Color(color.darken(0.2)),
+                    color,
+                    Color(color.lighten(0.2)),
+                    Color(color.lighten(0.6)),
+                ]
+
     def get_text(self) -> str:
         """Get the gradient text.
 
         Returns:
             str: The gradient text.
         """
         if isinstance(self._text, str):
@@ -201,15 +224,17 @@
 
     def get_indexes(self, verbose: bool = False) -> List[List[int]]:
         """Generate the indexes for the gradient substring.
 
         Returns:
             List[List[int]]: The indexes for the gradient substring.
         """
-        result: ndarray = np.array_split(np.arange(self._length), self.hues - 1)
+        result: NDArray[Shape["*, *"], int] = np.array_split(
+            np.arange(self._length), self.hues - 1
+        )
         indexes: List[List[int]] = [sublist.tolist() for sublist in result]
         for count, index in enumerate(indexes):
             msg = f"[b white]Index {count}:[/]{', '.join([str(i) for i in index])}\n\n"
             if verbose:
                 log.success(msg)
             else:
                 log.info(msg)
@@ -267,17 +292,17 @@
                 r2, g2, b2 = color2.rgb_tuple
                 dr = r2 - r1
                 dg = g2 - g1
                 db = b2 - b1
 
             for subindex in range(gradient_length):
                 blend = subindex / gradient_length
-                red = int(r1 + (blend * dr))
-                green = int(g1 + (blend * dg))
-                blue = int(b1 + (blend * db))
+                red = int(r1 + (blend * dr))  # type: ignore
+                green = int(g1 + (blend * dg))  # type: ignore
+                blue = int(b1 + (blend * db))  # type: ignore
                 color = f"#{red:02X}{green:02X}{blue:02X}"
                 substring.stylize(color, subindex, subindex + 1)
 
             gradient_string = Text.assemble(
                 gradient_string,
                 substring,
                 style=self.style,
@@ -332,45 +357,45 @@
     @text.setter
     def text(self, text: Optional[str | Text]) -> None:
         """Set the text of the gradient."""
         log.debug(f"Setting gradient._text: {text}")
         if isinstance(text, Text):
             sanitized_text = strip_control_codes(text.plain)
             self._length = len(sanitized_text)
-            self._text = [sanitized_text]
+            self._text = sanitized_text
             self._spans: List[Span] = text.spans
         if isinstance(text, str):
             if text == "":
                 raise ValueError("Text cannot be empty.")
             sanitized_text = strip_control_codes(text)
             self._length = len(sanitized_text)
             self._text = sanitized_text
 
     @property
-    def hues(self) -> int:
+    def hues(self) -> int:  # type: ignore
         """The number of colors in the gradient."""
         log.debug(f"Retrieving gradient._hues: {self._hues}")
         return self._hues
 
     @hues.setter
-    def hues(self, hues: int) -> None:
+    def hues(self, hues: int) -> None:  # type: ignore
         """Set the number of colors in the gradient."""
         log.debug(f"Setting gradient._hues: {hues}")
         if hues < 2:
             raise ValueError("Gradient must have at least two colors.")
         self._hues = hues
 
     @property
-    def color_sample(self) -> bool:
+    def color_sample(self) -> bool:  # type: ignore
         """Whether the gradient is a color sample."""
         log.debug(f"Retrieving gradient._color_sample: {self._color_sample}")
         return self._color_sample
 
-    @color_sample.setter
-    def color_sample(self, color_sample: bool) -> None:
+    @color_sample.setter  # type: ignore
+    def color_sample(self, color_sample: bool) -> None:  # type: ignore
         """Set whether the gradient is a color sample."""
         log.debug(f"Setting gradient._color_sample: {color_sample}")
         if color_sample:
             self.text = "█" * self._length
         self._color_sample = color_sample
 
     @property
@@ -397,15 +422,15 @@
     def generate_style(self, color: str) -> Style:
         """Generate a style for a color."""
         new_style = self.style + Style(color=color)
         log.debug(f"Generating style for `{color}`: {new_style}")
         return new_style
 
 
-def gradient_color() -> Layout:
+def examples() -> Layout:
     """Generate a layout for the examples of gradients."""
     TEXT = lorem.paragraphs(2)
     gradient_random = Gradient(TEXT)
     panel_random = Panel(
         gradient_random,
         title=Gradient("Random Gradient"),
         padding=(2, 4),
@@ -526,15 +551,15 @@
             record=record,
         )
     else:
         example_console = Console(
             theme=GradientTheme(),
         )
     console.rule(Gradient("Color Gradient Examples"))
-    example_console.print(gradient_color())
+    example_console.print(examples())
     example_console.line()
     example_console.print(style_layout())
     if record:
         example_console.save_svg("Images/gradient.svg", title="Gradient Examples")
 
 
 if __name__ == "__main__":
```

### Comparing `maxgradient-0.1.4/maxgradient/log.py` & `maxgradient-0.1.5/maxgradient/_log.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 """Gradient logging module"""
 # pylint: disable=E0401,W0611,C0103
 from __future__ import annotations
 
 import re
 from datetime import datetime
+from functools import wraps
+from os import environ
 from pathlib import Path
-from typing import Optional, Self, Any
+from sys import stderr, stdout
+from typing import Any, Optional, Self
 
 import loguru
 from loguru import logger
 from rich.abc import RichRenderable
-from rich.console import Console as RichConsole
-from rich.highlighter import ReprHighlighter, RegexHighlighter
+from rich.console import Console
+from rich.highlighter import RegexHighlighter
 from rich.table import Table
 from rich.traceback import install as install_rich_traceback
 
 from maxgradient.theme import GradientTheme
 
 CWD = Path.cwd()
 DEBUG_LOG = CWD / "logs" / "debug.log"
@@ -39,29 +42,34 @@
 class LogHighlighter(RegexHighlighter):
     """Apply style to anything that looks like an email."""
 
     base_style = "log."
     highlights = [
         r"(?P<keyword>.+(?=\d+)) ?(?P<index>\d+)?(?P<separator>:) ",
         r"(?P<keyword>[A-Za-z_()]+)(?P<separator>:) ",
-        r"^[^\d:]+:"
+        r"^[^\d:]+:",
     ]
 
 
-class LogConsole(RichConsole, metaclass=Singleton):
+class Console(Console, metaclass=Singleton):
     """A Console to log to. Inherits from rich.console.Console.\
         This class is a singleton which removes the need to pass\
         around a console object or use the `get_console` method."""
 
     def __init__(self) -> None:
-        super().__init__(theme=GradientTheme(), highlighter=LogHighlighter())
+        super().__init__(
+            theme=GradientTheme(),
+            highlighter=LogHighlighter(),
+            stderr=True,
+            tab_size=4,
+        )
         install_rich_traceback(console=self)
 
 
-console_ = LogConsole()
+console_ = Console()
 
 
 class Log:
     """Logging class of MaxGradient. It utilizes the loguru library as well as rich.\
         It can be called and used without any arguments, but it can also be\
         instantiated with a rich_level argument. This will set the level of\
         logs that are printed to the console. The default is "SUCCESS", which\
@@ -78,18 +86,21 @@
                 to _console, which is a console with the GradientTheme and a\
                 ReprHighlighter.
     """
 
     rich_level: str
 
     def __init__(
-        self, console: LogConsole = console_, rich_level: str = "SUCCESS"
+        self, console: Optional[Console] = None, rich_level: str = "SUCCESS"
     ) -> None:
         self.rich_level = rich_level
-        self.console: LogConsole = console
+        if console is None:
+            console = Console()
+            install_rich_traceback(console=console)
+        self.console: Console = console
         logger.remove()
         logger.configure(
             handlers=[
                 {
                     "sink": DEBUG_LOG,
                     "level": "DEBUG",
                     "format": FORMAT,
@@ -240,16 +251,16 @@
         return f"[bold {color}]{file}[/]"
 
     @staticmethod
     def _get_line(record: loguru.Record) -> str:
         """Return the line the record was logged from with color."""
         line: int = record["line"]
         color = "#7FD6E8"
-        line = f"[bold {color}]Line {line}[/]"
-        return line
+        line_str = f"[bold {color}]Line {line}[/]"
+        return line_str
 
     @classmethod
     def _get_msg(cls, record: loguru.Record) -> str:
         """Return the message of the record with color."""
         level_color = cls._get_level_color(record)
         msg: str = record["message"]
         return f"[bold {level_color}]{msg}[/]"
@@ -264,15 +275,15 @@
             title_style="bold #ff8800",
             show_lines=True,
             show_edge=False,
             padding=(0, 1),
             expand=False,
         )
 
-    def rich_sink(self, message: loguru.Message, console: LogConsole = console_) -> None:
+    def rich_sink(self, message: loguru.Message) -> None:
         """Log to console.
 
         Args:
             message (loguru.Message): Message to log.
             console (rich.console.Console, optional): Console to log to.
         """
         # format the components of the log message
@@ -284,15 +295,15 @@
         msg: str = self._get_msg(record)
 
         # generate the log table
         log_table = self._generate_log_table()
         log_table.add_row(time, file, line, level, msg)
 
         # print the log table
-        console.print(
+        self.console.print(
             log_table,
             justify="left",
             # width=int(console.width * 0.8),
         )
 
     def rich_filter(self, record: loguru.Record) -> bool:
         """Filter logs to print to the console."""
@@ -318,64 +329,66 @@
         """Log to success.log.
 
         Args:
             msg (str): Message to log.
         """
         self.logger.success(msg)
 
-    def key(self, key:str, value: Any) -> None:
+    def key(self, key: str, value: Any) -> None:
         """Log to debug.log
 
         Args:
             msg (str): Message to log.
         """
         key_markup = f"[bold #E3EC84]{key}[/]"
         sep = "[bold #ffffff]: [/]"
         value_markup = f"[bold #00ff00]{value}[/]"
         msg = f"{key_markup}{sep}{value_markup}"
         self.logger.debug(msg)
 
-    def key_index(self, key:str, index: int, value: Any) -> None:
+    def key_index(self, key: str, index: int, value: Any) -> None:
         """Log to debug.log
 
         Args:
             msg (str): Message to log.
         """
         key_markup = f"[bold ##E3EC84]{key}[/]"
         index_markup = f"[bold #7FD6E8] {index}[/]"
         sep = "[bold #ffffff]: [/]"
         value_markup = f"[bold #00ff00]{value}[/]"
         msg = f"{key_markup}{index_markup}{sep}{value_markup}"
         self.logger.debug(msg)
 
-    def warning(self, msg: RichRenderable) -> None:
+    def warning(self, msg: str | RichRenderable) -> None:
         """Log to console.
 
         Args:
             msg (str): Message to log.
         """
         self.logger.log("WARNING", msg)
 
-    def error(self, msg: RichRenderable) -> None:
+    def error(self, msg: str | RichRenderable) -> None:
         """Log to console.
 
         Args:
             msg (str): Message to log.
         """
         self.logger.log("ERROR", msg)
 
-    def critical(self, msg: RichRenderable) -> None:
+    def critical(self, msg: str | RichRenderable) -> None:
         """Log to console.
 
         Args:
             msg (str): Message to log.
         """
         self.logger.log("CRITICAL", msg)
 
-    def log(self, level: str, msg: str, verbose: bool = VERBOSE) -> None:
+    def log(
+        self, level: str, msg: str | RichRenderable, verbose: bool = VERBOSE
+    ) -> None:
         """Log to console or log file.
 
         Args:
             level (str): Log level.
             msg (str): Message to log.
         """
         if verbose:
@@ -383,24 +396,93 @@
                 level = "SUCCESS"
             self.logger.log(level, msg)
         else:
             if level not in ["DEBUG", "INFO"]:
                 level = "DEBUG"
             self.logger.log(level, msg)
 
-log = Log(console_)
+    def opt(self, *kwargs, depth: int = 0) -> "Log":
+        """Return a new logger with the specified depth offset."""
+        return self.logger.opt(depth=depth, *kwargs)  # type: ignore
+
+    @staticmethod
+    def _combine_regex(*regexes: str) -> str:
+        """Combine a number of regexes in to a single regex.
+
+        Returns:
+            str: New regex with all regexes ORed together.
+        """
+        return "|".join(regexes)
+
+    def trace(*, level="DEBUG", depth: int = 1, entry: bool = True, exit: bool = True):
+        def wrapper(func):
+            name = func.__name__
+
+            @wraps(func)
+            def wrapped(*args, **kwargs):
+                logger_ = log.opt(depth=1)
+                if entry:
+                    logger_.log(
+                        level,
+                        "Entering '{}' (Args={}, Kwargs={})",
+                        name,
+                        *args,
+                        *kwargs,
+                    )
+                result = func(*args, **kwargs)
+                if exit:
+                    logger_.log(level, "Exiting '{name}' (Result={result})")
+                return result
+
+            return wrapped
+
+        return wrapper
+
+    def disable(self) -> None:
+        """Disable logging."""
+        self.logger.disable("maxgradient")
+
+    def enable(self, module: str = "maxgradient") -> None:
+        """Enable logging.
+
+        Args:
+            module (str, optional): Module to enable logging for. Defaults to "maxgradient".
+        """
+        self.logger.enable(module)
+
+
+def debug(*, level="DEBUG", depth: int = 1, entry: bool = True, exit: bool = True):
+    def wrapper(func):
+        name = func.__name__
+
+        @wraps(func)
+        def wrapped(*args, **kwargs):
+            logger_ = log.opt(depth=depth)
+            if entry:
+                logger_.log(
+                    level, "Entering '{}' (Args={}, Kwargs={})", name, *args, *kwargs
+                )
+            result = func(*args, **kwargs)
+            if exit:
+                logger_.log(level, "Exiting '{name}' (Result={result})")
+            return result
+
+        return wrapped
+
+    return wrapper
 
 
 def test_logger():
     """Text log handlers"""
     console_.line(2)
-    text_log = Log("DEBUG")
+    text_log = Log()
     text_log.info("Initialize DEBUG Log")
     text_log.debug("Initialize INFO Log")
     text_log.success("Initialize SUCCESS Log")
     text_log.warning("Initialize WARNING Log")
     text_log.error("Initialize ERROR Log")
     text_log.critical("Initialize CRITICAL Log")
 
 
 if __name__ == "__main__":
+    log = Log()
     test_logger()
```

### Comparing `maxgradient-0.1.4/maxgradient/theme.py` & `maxgradient-0.1.5/maxgradient/theme.py`

 * *Files identical despite different names*

### Comparing `maxgradient-0.1.4/tests/test_rich_colors.py` & `maxgradient-0.1.5/tests/test_rich_colors.py`

 * *Files identical despite different names*

### Comparing `maxgradient-0.1.4/tests/test_x11_colors.py` & `maxgradient-0.1.5/tests/test_x11_colors.py`

 * *Files identical despite different names*

### Comparing `maxgradient-0.1.4/PKG-INFO` & `maxgradient-0.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
-Name: maxgradient
-Version: 0.1.4
-Summary: A library to make printing gradient color to the terminal a lot easier. Think `lolcat` but utilizing python's `rich` library so you can use it anywhere.
+Name: MaxGradient
+Version: 0.1.5
+Summary: MaxGradient automates the printing gradient colored text to the console.
 Author-Email: maxludden <dev@maxludden.com>
 License: MIT
-Requires-Python: >=3.9
-Requires-Dist: rich>=13.3.5
-Requires-Dist: lorem-text>=2.1
-Requires-Dist: numpy>=1.24.3
+Requires-Python: >=3.10
 Requires-Dist: loguru>=0.7.0
+Requires-Dist: rich>=13.4.2
+Requires-Dist: typer-cli>=0.0.1
+Requires-Dist: nptyping>=2.5.0
 Requires-Dist: typer>=0.9.0
-Requires-Dist: typer[all]>=0.9.0; extra == "cli"
-Provides-Extra: cli
+Requires-Dist: numpy>=1.25.0
 Description-Content-Type: text/markdown
 
 <html>
     <head>
         <link href="styles/gradient.css" rel="stylesheet">
     </head>
     <body>
+        <!--MaxGradient Banner-->
         <img src="https://raw.githubusercontent.com/maxludden/maxludden/621fcb611c1e52160d89d33e1441b34948c37752/maxgradient_banner.svg" alt="MaxGradient" width="100%">
+        <!--End of Banner-->
 ​        <div class="badges">
 ​            <a href="https://GitHub.com/maxludden/maxgradient"><img  class="badge" src="https://img.shields.io/badge/Python-3.9 | 3.10 | 3.11-blue?logo=python" alt="PyPI - MaxGradient"></a>
 ​            <a href="https://GitHub.com/maxludden/maxgradient"><img  class="badge" src="https://img.shields.io/badge/PyPI-MaxGradient-blue?" alt="PyPI - MaxGradient"></a>
-​            <a href="https://GitHub.com/maxludden/maxgradient"><img  class="badge" src="https://img.shields.io/badge/Version-0.1.4-bbbbbb" alt="Version - 0.1.3"></a>
+​            <a href="https://GitHub.com/maxludden/maxgradient"><img  class="badge" src="https://img.shields.io/badge/Version-0.1.4-bbbbbb" alt="Version - 0.1.5"></a>
 ​            <a href="https://pdm.fming.dev/"><img class="badge" src="https://camo.githubusercontent.com/acf0526fc1f541f9d980d7983ff5ab8e540cf2136206c2b5dc740f658a37fac0/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f70646d2d6d616e616765642d626c756576696f6c6574"></a>
 ​        </div>
         <!--End of badges-->
 ​        <div class="summary">
             <p><span class="mg">MaxGradient</span> automates the printing gradient colored text to the console. It's built upon the great <a href="https://rich.readthedocs.io/en/latest/introduction.html"> <span class="warm-wipe">rich library</span></a>. It contains a Console that can serve as a drop in replacement for <span class="lightblue-cyan-wipe">rich.rich.Console</span> and has an expanded Color class which can parse X11 color names on top of rich's standard colors. <span class="mg">MaxGradient</span> is a work in progress and I'm open to any suggestions or contributions.</span></p>
         </div>
 ​        <div class="body">
@@ -74,15 +75,15 @@
 
 ```python
 class Gradient(rich.rich.Text):
     """Text with gradient color / style."""
 
     def __init__ (
         ext: Optional[str | Text] = "",
-        colors: Optional[List[Color | Tuple | str]] = None,
+        colors: Optional[str|List[Color | Tuple | str]] = None,
         rainbow: bool = False,
         invert: bool = False,
         hues: Optional[int] = None,
         color_sample: bool = False,
         style: StyleType = Style.null(),
         *,
         # The arguments below are used directly by Text
```

