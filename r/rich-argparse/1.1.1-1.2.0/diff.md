# Comparing `tmp/rich_argparse-1.1.1.tar.gz` & `tmp/rich_argparse-1.2.0.tar.gz`

## Comparing `rich_argparse-1.1.1.tar` & `rich_argparse-1.2.0.tar`

### file list

```diff
@@ -1,7 +1,11 @@
--rw-r--r--   0        0        0    21224 2020-02-02 00:00:00.000000 rich_argparse-1.1.1/rich_argparse.py
--rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 rich_argparse-1.1.1/rich_argparse-stubs/__init__.pyi
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 rich_argparse-1.1.1/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 rich_argparse-1.1.1/LICENSE
--rw-r--r--   0        0        0     8599 2020-02-02 00:00:00.000000 rich_argparse-1.1.1/README.md
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 rich_argparse-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     9841 2020-02-02 00:00:00.000000 rich_argparse-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    16607 2020-02-02 00:00:00.000000 rich_argparse-1.2.0/rich_argparse/__init__.py
+-rw-r--r--   0        0        0     3679 2020-02-02 00:00:00.000000 rich_argparse-1.2.0/rich_argparse/__main__.py
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 rich_argparse-1.2.0/rich_argparse/_common.py
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 rich_argparse-1.2.0/rich_argparse/_lazy_rich.py
+-rw-r--r--   0        0        0    10627 2020-02-02 00:00:00.000000 rich_argparse-1.2.0/rich_argparse/optparse.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rich_argparse-1.2.0/rich_argparse/py.typed
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 rich_argparse-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 rich_argparse-1.2.0/LICENSE
+-rw-r--r--   0        0        0     9868 2020-02-02 00:00:00.000000 rich_argparse-1.2.0/README.md
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 rich_argparse-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0    11131 2020-02-02 00:00:00.000000 rich_argparse-1.2.0/PKG-INFO
```

### Comparing `rich_argparse-1.1.1/rich_argparse.py` & `rich_argparse-1.2.0/rich_argparse/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,40 +3,35 @@
 from __future__ import annotations
 
 import argparse
 import re
 import sys
 from typing import TYPE_CHECKING, Callable, ClassVar, Iterable, Iterator
 
-# rich is only used to display help. It is imported inside the functions in order
-# not to add delays to command line tools that use this formatter.
+import rich_argparse._lazy_rich as r
+from rich_argparse._common import _HIGHLIGHTS, _rich_fill, _rich_wrap
+
 if TYPE_CHECKING:
-    from argparse import Action, _ArgumentGroup
     from typing_extensions import Self
 
-    from rich.console import Console, ConsoleOptions, RenderableType, RenderResult
-    from rich.containers import Lines
-    from rich.style import StyleType
-    from rich.text import Span, Text
-
 __all__ = [
     "RichHelpFormatter",
     "RawDescriptionRichHelpFormatter",
     "RawTextRichHelpFormatter",
     "ArgumentDefaultsRichHelpFormatter",
     "MetavarTypeRichHelpFormatter",
 ]
 
 
 class RichHelpFormatter(argparse.HelpFormatter):
     """An argparse HelpFormatter class that renders using rich."""
 
     group_name_formatter: ClassVar[Callable[[str], str]] = str.title
     """A function that formats group names. Defaults to ``str.title``."""
-    styles: ClassVar[dict[str, StyleType]] = {
+    styles: ClassVar[dict[str, r.StyleType]] = {
         "argparse.args": "cyan",
         "argparse.groups": "dark_orange",
         "argparse.help": "default",
         "argparse.metavar": "dark_cyan",
         "argparse.syntax": "bold",
         "argparse.text": "default",
         "argparse.prog": "grey50",
@@ -49,18 +44,15 @@
     - ``argparse.groups``: for group names (e.g. "positional arguments")
     - ``argparse.help``: for argument's help text (e.g. "show this help message and exit")
     - ``argparse.metavar``: for meta variables (e.g. "FILE" in "--file FILE")
     - ``argparse.prog``: for %(prog)s in the usage (e.g. "foo" in "Usage: foo [options]")
     - ``argparse.syntax``: for highlights of back-tick quoted text (e.g. "``` `some text` ```"),
     - ``argparse.text``: for the descriptions and epilog (e.g. "A foo program")
     """
-    highlights: ClassVar[list[str]] = [
-        r"(?:^|\s)(?P<args>-{1,2}[\w]+[\w-]*)",  # highlight --words-with-dashes as args
-        r"`(?P<syntax>[^`]*)`",  # highlight `text in backquotes` as syntax
-    ]
+    highlights: ClassVar[list[str]] = _HIGHLIGHTS[:]
     """A list of regex patterns to highlight in the help text.
 
     It is used in the description, epilog, groups descriptions, and arguments' help. By default,
     it highlights ``--words-with-dashes`` with the `argparse.args` style and
     ``` `text in backquotes` ``` with the `argparse.syntax` style.
 
     To disable highlighting, clear this list (``RichHelpFormatter.highlights.clear()``).
@@ -80,15 +72,15 @@
         self,
         prog: str,
         indent_increment: int = 2,
         max_help_position: int = 24,
         width: int | None = None,
     ) -> None:
         super().__init__(prog, indent_increment, max_help_position, width)
-        self._console: Console | None = None
+        self._console: r.Console | None = None
 
         # https://docs.python.org/3/library/stdtypes.html#printf-style-string-formatting
         self._printf_style_pattern = re.compile(
             r"""
             %                               # Percent character
             (?:\((?P<mapping>[^)]*)\))?     # Mapping key
             (?P<flag>[#0\-+ ])?             # Conversion Flags
@@ -97,59 +89,51 @@
             [hlL]?                          # Length modifier (ignored)
             (?P<format>[diouxXeEfFgGcrsa%]) # Conversion type
             """,
             re.VERBOSE,
         )
 
     @property
-    def console(self) -> Console:  # deprecate?
+    def console(self) -> r.Console:  # deprecate?
         if self._console is None:
-            from rich.console import Console
-            from rich.theme import Theme
-
-            self._console = Console(theme=Theme(self.styles))
+            self._console = r.Console(theme=r.Theme(self.styles))
         return self._console
 
     @console.setter
-    def console(self, console: Console) -> None:  # is this needed?
+    def console(self, console: r.Console) -> None:  # is this needed?
         self._console = console
 
-    class _Section(argparse.HelpFormatter._Section):  # type: ignore[misc]
+    class _Section(argparse.HelpFormatter._Section):
         def __init__(
             self, formatter: RichHelpFormatter, parent: Self | None, heading: str | None = None
         ) -> None:
             if heading is not None:
                 heading = f"{type(formatter).group_name_formatter(heading)}:"
             super().__init__(formatter, parent, heading)
-            self.rich_items: list[RenderableType] = []
-            self.rich_actions: list[tuple[Text, Text | None]] = []
+            self.formatter: RichHelpFormatter
+            self.rich_items: list[r.RenderableType] = []
+            self.rich_actions: list[tuple[r.Text, r.Text | None]] = []
             if parent is not None:
                 parent.rich_items.append(self)
-            if TYPE_CHECKING:  # already assigned in super().__init__ but not present in typeshed
-                self.formatter = formatter
-                self.heading = heading
-                self.parent = parent
-
-        def __rich_console__(self, console: Console, options: ConsoleOptions) -> RenderResult:
-            from rich.text import Text
 
+        def __rich_console__(self, console: r.Console, options: r.ConsoleOptions) -> r.RenderResult:
             # empty section
             if not self.rich_items and not self.rich_actions:
                 return
             # root section
             if self is self.formatter._root_section:
                 yield from self.rich_items
                 return
             # group section
             help_pos = min(self.formatter._action_max_length + 2, self.formatter._max_help_position)
             help_width = max(self.formatter._width - help_pos, 11)
             if self.heading:
-                yield Text(self.heading, style="argparse.groups")
+                yield r.Text(self.heading, style="argparse.groups")
             yield from self.rich_items  # (optional) group description
-            indent = Text(" " * help_pos)
+            indent = r.Text(" " * help_pos)
             for action_header, action_help in self.rich_actions:
                 if not action_help:
                     yield action_header  # no help, yield the header and finish
                     continue
                 action_help_lines = self.formatter._rich_split_lines(action_help, help_width)
                 if len(action_header) > help_pos - 2:
                     yield action_header  # the header is too long, put it on its own line
@@ -165,54 +149,57 @@
     def add_text(self, text: str | None) -> None:
         if text is not argparse.SUPPRESS and text is not None:
             self._current_section.rich_items.append(self._rich_format_text(text))
 
     def add_usage(
         self,
         usage: str | None,
-        actions: Iterable[Action],
-        groups: Iterable[_ArgumentGroup],
+        actions: Iterable[argparse.Action],
+        groups: Iterable[argparse._MutuallyExclusiveGroup],
         prefix: str | None = None,
     ) -> None:
         if usage is argparse.SUPPRESS:
             return
-        from rich.text import Span, Text
-
         if prefix is None:
             prefix = self._format_usage(usage="", actions=(), groups=(), prefix=None).rstrip("\n")
         prefix_end = ": " if prefix.endswith(": ") else ""
         prefix = prefix[: len(prefix) - len(prefix_end)]
-        prefix = type(self).group_name_formatter(prefix) + prefix_end
+        prefix = (
+            type(self).group_name_formatter(prefix).translate(r.CONTROL_STRIP_TRANSLATE)
+            + prefix_end
+        )
 
-        usage_spans = [Span(0, len(prefix.rstrip()), "argparse.groups")]
-        usage_text = self._format_usage(usage, actions, groups, prefix=prefix)
+        usage_spans = [r.Span(0, len(prefix.rstrip()), "argparse.groups")]
+        usage_text = self._format_usage(usage, actions, groups, prefix=prefix).translate(
+            r.CONTROL_STRIP_TRANSLATE
+        )
         if usage is None:  # get colour spans for generated usage
-            prog = f"{self._prog}"
+            prog = f"{self._prog}".translate(r.CONTROL_STRIP_TRANSLATE)
             if actions:
                 prog_start = usage_text.index(prog, len(prefix))
-                usage_spans.append(Span(prog_start, prog_start + len(prog), "argparse.prog"))
+                usage_spans.append(r.Span(prog_start, prog_start + len(prog), "argparse.prog"))
             actions_start = len(prefix) + len(prog) + 1
             try:
                 spans = list(self._rich_usage_spans(usage_text, actions_start, actions=actions))
             except ValueError:
                 spans = []
             usage_spans.extend(spans)
-            rich_usage = Text(usage_text)
+            rich_usage = r.Text(usage_text)
         elif self.usage_markup:  # treat user provided usage as markup
-            usage_spans.extend(self._rich_prog_spans(prefix + Text.from_markup(usage).plain))
-            rich_usage = Text.from_markup(usage_text)
+            usage_spans.extend(self._rich_prog_spans(prefix + r.Text.from_markup(usage).plain))
+            rich_usage = r.Text.from_markup(usage_text)
             usage_spans.extend(rich_usage.spans)
             rich_usage.spans.clear()
         else:  # treat user provided usage as plain text
             usage_spans.extend(self._rich_prog_spans(prefix + usage))
-            rich_usage = Text(usage_text)
+            rich_usage = r.Text(usage_text)
         rich_usage.spans.extend(usage_spans)
         self._root_section.rich_items.append(rich_usage)
 
-    def add_argument(self, action: Action) -> None:
+    def add_argument(self, action: argparse.Action) -> None:
         super().add_argument(action)
         if action.help is not argparse.SUPPRESS:
             self._current_section.rich_actions.extend(self._rich_format_action(action))
 
     def format_help(self) -> str:
         with self.console.capture() as capture:
             self.console.print(self._root_section, highlight=False, soft_wrap=True)
@@ -220,70 +207,71 @@
         if help:
             help = self._long_break_matcher.sub("\n\n", help).rstrip() + "\n"
         return help
 
     # ===============
     # Utility methods
     # ===============
-    def _rich_prog_spans(self, usage: str) -> Iterator[Span]:
-        from rich.text import Span
-
+    def _rich_prog_spans(self, usage: str) -> Iterator[r.Span]:
         if "%(prog)" not in usage:
             return
         params = {"prog": self._prog}
         formatted_usage = ""
         last = 0
         for m in self._printf_style_pattern.finditer(usage):
             start, end = m.span()
             formatted_usage += usage[last:start]
             sub = usage[start:end] % params
             prog_start = len(formatted_usage)
             prog_end = prog_start + len(sub)
             formatted_usage += sub
             last = end
-            yield Span(prog_start, prog_end, "argparse.prog")
+            yield r.Span(prog_start, prog_end, "argparse.prog")
 
-    def _rich_usage_spans(self, text: str, start: int, actions: Iterable[Action]) -> Iterator[Span]:
-        from rich.text import Span
-
-        options: list[Action] = []
-        positionals: list[Action] = []
+    def _rich_usage_spans(
+        self, text: str, start: int, actions: Iterable[argparse.Action]
+    ) -> Iterator[r.Span]:
+        options: list[argparse.Action] = []
+        positionals: list[argparse.Action] = []
         for action in actions:
             if action.help is not argparse.SUPPRESS:
                 options.append(action) if action.option_strings else positionals.append(action)
         pos = start
+
+        def find_span(_string: str) -> tuple[int, int]:
+            stripped = _string.translate(r.CONTROL_STRIP_TRANSLATE)
+            _start = text.index(stripped, pos)
+            _end = _start + len(stripped)
+            return _start, _end
+
         for action in options:  # start with the options
             if sys.version_info >= (3, 9):  # pragma: >=3.9 cover
                 usage = action.format_usage()
                 if isinstance(action, argparse.BooleanOptionalAction):
                     for option_string in action.option_strings:
-                        start = text.index(option_string, pos)
-                        end = start + len(option_string)
-                        yield Span(start, end, "argparse.args")
+                        start, end = find_span(option_string)
+                        yield r.Span(start, end, "argparse.args")
                         pos = end + 1
                     continue
             else:  # pragma: <3.9 cover
                 usage = action.option_strings[0]
-            start = text.index(usage, pos)
-            end = start + len(usage)
-            yield Span(start, end, "argparse.args")
+            start, end = find_span(usage)
+            yield r.Span(start, end, "argparse.args")
             if action.nargs != 0:
                 metavar = self._format_args(action, self._get_default_metavar_for_optional(action))
-                start = text.index(metavar, end)
-                end = start + len(metavar)
-                yield Span(start, end, "argparse.metavar")
+                start, end = find_span(metavar)
+                yield r.Span(start, end, "argparse.metavar")
             pos = end + 1
         for action in positionals:  # positionals come at the end
             usage = self._format_args(action, self._get_default_metavar_for_positional(action))
-            start = text.index(usage, pos)
-            end = start + len(usage)
-            yield Span(start, end, "argparse.args")
+            start, end = find_span(usage)
+            yield r.Span(start, end, "argparse.args")
             pos = end + 1
 
-    def _rich_whitespace_sub(self, text: Text) -> Text:
+    def _rich_whitespace_sub(self, text: r.Text) -> r.Text:
         # do this `self._whitespace_matcher.sub(' ', text).strip()` but text is Text
         spans = [m.span() for m in self._whitespace_matcher.finditer(text.plain)]
         for start, end in reversed(spans):
             if end - start > 1:  # slow path
                 space = text[start : start + 1]
                 space.plain = " "
                 text = text[:start] + space + text[end:]
@@ -295,194 +283,95 @@
             text = text[lstrip_at:]
         text.rstrip()
         return text
 
     # =====================================
     # Rich version of HelpFormatter methods
     # =====================================
-    def _rich_expand_help(self, action: Action) -> Text:
-        from rich.markup import escape
-        from rich.text import Text
-
+    def _rich_expand_help(self, action: argparse.Action) -> r.Text:
         params = dict(vars(action), prog=self._prog)
         for name in list(params):
             if params[name] is argparse.SUPPRESS:
                 del params[name]
             elif hasattr(params[name], "__name__"):
                 params[name] = params[name].__name__
         if params.get("choices") is not None:
             params["choices"] = ", ".join([str(c) for c in params["choices"]])
         help_string = self._get_help_string(action)
         assert help_string is not None
-        help_string % params  # pyright: ignore[reportUnusedExpression] # raise ValueError if needed
+        # raise ValueError if needed
+        help_string % params  # pyright: ignore[reportUnusedExpression]
         parts = []
         last = 0
         for m in self._printf_style_pattern.finditer(help_string):
             start, end = m.span()
             parts.append(help_string[last:start])
-            parts.append(escape(help_string[start:end] % params))
+            parts.append(r.escape(help_string[start:end] % params))
             last = end
         parts.append(help_string[last:])
-        rich_help = Text.from_markup("".join(parts), style="argparse.help")
+        rich_help = r.Text.from_markup("".join(parts), style="argparse.help")
         for highlight in self.highlights:
             rich_help.highlight_regex(highlight, style_prefix="argparse.")
         return rich_help
 
-    def _rich_format_text(self, text: str) -> Text:
-        from rich.markup import escape
-        from rich.text import Text
-
+    def _rich_format_text(self, text: str) -> r.Text:
         if "%(prog)" in text:
-            text = text % {"prog": escape(self._prog)}
-        rich_text = Text.from_markup(text, style="argparse.text")
+            text = text % {"prog": r.escape(self._prog)}
+        rich_text = r.Text.from_markup(text, style="argparse.text")
         for highlight in self.highlights:
             rich_text.highlight_regex(highlight, style_prefix="argparse.")
         text_width = max(self._width - self._current_indent * 2, 11)
-        indent = Text(" " * self._current_indent)
+        indent = r.Text(" " * self._current_indent)
         return self._rich_fill_text(rich_text, text_width, indent)
 
-    def _rich_format_action(self, action: Action) -> Iterator[tuple[Text, Text | None]]:
+    def _rich_format_action(
+        self, action: argparse.Action
+    ) -> Iterator[tuple[r.Text, r.Text | None]]:
         header = self._rich_format_action_invocation(action)
         header.pad_left(self._current_indent)
         help = self._rich_expand_help(action) if action.help and action.help.strip() else None
         yield header, help
         for subaction in self._iter_indented_subactions(action):
             yield from self._rich_format_action(subaction)
 
-    def _rich_format_action_invocation(self, action: Action) -> Text:
-        from rich.text import Text
-
+    def _rich_format_action_invocation(self, action: argparse.Action) -> r.Text:
         if not action.option_strings:
-            return Text().append(self._format_action_invocation(action), style="argparse.args")
+            return r.Text().append(self._format_action_invocation(action), style="argparse.args")
         else:
-            action_header = Text(", ").join(Text(o, "argparse.args") for o in action.option_strings)
+            action_header = r.Text(", ").join(
+                r.Text(o, "argparse.args") for o in action.option_strings
+            )
             if action.nargs != 0:
                 default = self._get_default_metavar_for_optional(action)
                 args_string = self._format_args(action, default)
-                action_header.append_tokens(((" ", None), (args_string, "argparse.metavar")))
+                action_header.append(" ").append(args_string, style="argparse.metavar")
             return action_header
 
-    def _rich_split_lines(self, text: Text, width: int) -> Lines:
-        return self._rich_whitespace_sub(text).wrap(self.console, width)
+    def _rich_split_lines(self, text: r.Text, width: int) -> r.Lines:
+        return _rich_wrap(self.console, self._rich_whitespace_sub(text), width)
 
-    def _rich_fill_text(self, text: Text, width: int, indent: Text) -> Text:
-        lines = self._rich_whitespace_sub(text).wrap(self.console, width)
-        return type(text)("\n").join(indent + line for line in lines) + "\n\n"
+    def _rich_fill_text(self, text: r.Text, width: int, indent: r.Text) -> r.Text:
+        return _rich_fill(self.console, self._rich_whitespace_sub(text), width, indent) + "\n\n"
 
 
 class RawDescriptionRichHelpFormatter(RichHelpFormatter):
     """Rich help message formatter which retains any formatting in descriptions."""
 
-    def _rich_fill_text(self, text: Text, width: int, indent: Text) -> Text:
-        return type(text)("\n").join(indent + line for line in text.split()) + "\n\n"
+    def _rich_fill_text(self, text: r.Text, width: int, indent: r.Text) -> r.Text:
+        return r.Text("\n").join(indent + line for line in text.split()) + "\n\n"
 
 
 class RawTextRichHelpFormatter(RawDescriptionRichHelpFormatter):
     """Rich help message formatter which retains formatting of all help text."""
 
-    def _rich_split_lines(self, text: Text, width: int) -> Lines:
+    def _rich_split_lines(self, text: r.Text, width: int) -> r.Lines:
         return text.split()
 
 
 class ArgumentDefaultsRichHelpFormatter(argparse.ArgumentDefaultsHelpFormatter, RichHelpFormatter):
     """Rich help message formatter which adds default values to argument help."""
 
 
 class MetavarTypeRichHelpFormatter(argparse.MetavarTypeHelpFormatter, RichHelpFormatter):
     """Rich help message formatter which uses the argument 'type' as the default
     metavar value (instead of the argument 'dest').
     """
-
-
-if __name__ == "__main__":
-    RichHelpFormatter.highlights.append(r"(?:^|\s)-{1,2}[\w]+[\w-]* (?P<metavar>METAVAR)\b")
-    parser = argparse.ArgumentParser(
-        prog="python -m rich_argparse",
-        formatter_class=RichHelpFormatter,
-        description=(
-            "This is a [link https://pypi.org/project/rich]rich[/]-based formatter for "
-            "[link https://docs.python.org/3/library/argparse.html#formatter-class]"
-            "argparse's help output[/].\n\n"
-            "It enables you to use the powers of rich like markup and highlights in your CLI help. "
-            "Read below for a glance at available features."
-        ),
-        epilog=":link: Read more at https://github.com/hamdanal/rich-argparse#usage.",
-    )
-    parser.add_argument(
-        "formatter-class",
-        help=(
-            "All you need to make your argparse.ArgumentParser output colorful text like this is to "
-            "pass it `formatter_class=RichHelpFormatter` or any of the available variants."
-        ),
-    )
-    parser.add_argument(
-        "styles",
-        help=(
-            "All the styles used by this formatter are defined in `RichHelpFormatter.styles`. "
-            "Modify this dictionary with any rich style to change the look of your CLI's help text."
-        ),
-    )
-    parser.add_argument(
-        "--highlights",
-        metavar="REGEXES",
-        help=(
-            "Highlighting the help text is managed by the list of regular expressions "
-            "`RichHelpFormatter.highlights`. Set to empty list to turn off highlighting.\n"
-            "See the next two options for default values."
-        ),
-    )
-    parser.add_argument(
-        "--syntax",
-        default=RichHelpFormatter.styles["argparse.syntax"],
-        help=(
-            "Text inside backticks is highlighted using the `argparse.syntax` style "
-            "(default: '%(default)s')"
-        ),
-    )
-    parser.add_argument(
-        "-s",
-        "--long-option",
-        metavar="METAVAR",
-        help=(
-            "Words that look like --command-line-options are highlighted using the `argparse.args` "
-            "style. In addition, this example, adds a highlighter regex for the word 'METAVAR' "
-            "following an option for the sake of demonstrating custom highlights.\n"
-            "Notice also that if an option takes a value and has short and long options, it is "
-            "printed as -s, --long-option METAVAR instead of -s METAVAR, --long-option METAVAR."
-        ),
-    )
-    group = parser.add_argument_group(
-        "more arguments",
-        description=(
-            "This is a custom group. Group names are [italic]*Title Cased*[/] by default. Use the "
-            "`RichHelpFormatter.group_name_formatter` function to change their format."
-        ),
-    )
-    group.add_argument(
-        "--more",
-        nargs="*",
-        help="This formatter works with subparsers, mutually exclusive groups and hidden arguments.",
-    )
-    mutex = group.add_mutually_exclusive_group()
-    mutex.add_argument(
-        "--rich",
-        action="store_true",
-        help="Rich and poor are mutually exclusive. Choose either one but not both.",
-    )
-    mutex.add_argument(
-        "--poor", action="store_false", dest="rich", help="Does poor mean --not-rich 😉?"
-    )
-    mutex.add_argument("--not-rich", action="store_false", dest="rich", help=argparse.SUPPRESS)
-
-    if "--generate-rich-argparse-preview" in sys.argv:  # for internal use only
-        from rich.console import Console  # noqa: F811
-        from rich.terminal_theme import DIMMED_MONOKAI
-        from rich.text import Text  # noqa: F811
-
-        width = 128
-        parser.formatter_class = lambda prog: RichHelpFormatter(prog, width=width)
-        text = Text.from_ansi(parser.format_help())
-        console = Console(record=True, width=width)
-        console.print(text)
-        console.save_svg("rich-argparse.svg", title="", theme=DIMMED_MONOKAI)
-    else:
-        parser.print_help()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `rich_argparse-1.1.1/LICENSE` & `rich_argparse-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rich_argparse-1.1.1/README.md` & `rich_argparse-1.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -8,26 +8,37 @@
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/hamdanal/rich-argparse/main.svg)
 ](https://results.pre-commit.ci/latest/github/hamdanal/rich-argparse/main)
 [![Python Version](https://img.shields.io/pypi/pyversions/rich-argparse)
 ![Release](https://img.shields.io/github/v/release/hamdanal/rich-argparse?sort=semver)
 ![Downloads](https://pepy.tech/badge/rich-argparse/month)
 ](https://pypi.org/project/rich-argparse/)
 
-Format argparse help output using [rich](https://pypi.org/project/rich).
+Format argparse and optparse help using [rich](https://pypi.org/project/rich).
+
+## Table of contents
+
+* [Installation](#installation)
+* [Usage](#usage)
+* [Output styles](#output-styles)
+  * [Colors](#customize-the-colors)
+  * [Group names](#customize-group-name-formatting)
+  * [Syntax highlighting](#special-text-highlighting)
+  * [Usage colors](#colors-in-the-usage)
+* [Subparsers](#working-with-subparsers)
+* [Third party formatters](#working-with-third-party-formatters)
+* [Optparse](#optparse-support) (experimental)
 
 ## Installation
 
 Install from PyPI with pip or your favorite tool.
 
 ```sh
 pip install rich-argparse
 ```
 
-Or copy the file `rich_argparse.py` to your project provided you have `rich` already installed.
-
 ## Usage
 
 Simply pass `formatter_class` to the argument parser
 ```python
 import argparse
 from rich_argparse import RichHelpFormatter
 
@@ -198,7 +209,35 @@
 
  if __name__ == '__main__':
      main()
 ```
 
 Now try out some command like: `python manage.py runserver --help`. Notice how the special
 ordering of the arguments applied by django is respected by the new help formatter.
+
+## Optparse support
+rich-argparse now ships with experimental support for [optparse]. Import optparse help formatters
+from `rich_argparse.optparse`:
+
+```python
+import optparse
+from rich_argparse.optparse import IndentedRichHelpFormatter
+
+parser = optparse.OptionParser(formatter=IndentedRichHelpFormatter())
+...
+```
+
+Similar to `argparse`, you can customize the styles used by the formatter by modifying the
+`RichHelpFormatter.styles` dictionary. These are the same styles used by `argparse` but with
+the `optparse.` prefix. For example, to change the style used for the metavar of an option:
+
+```python
+RichHelpFormatter.styles["optparse.metavar"] = "italic"
+```
+
+Syntax highlighting works the same way as `argparse`.
+
+Colors in the `usage` are not supported yet.
+
+Customizing the group name format is not supported. optparse uses title case by default.
+
+[optparse]: https://docs.python.org/3/library/optparse.html
```

### Comparing `rich_argparse-1.1.1/pyproject.toml` & `rich_argparse-1.2.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling>=1.11.0"]
 build-backend = "hatchling.build"
 
 [project]
-name = "rich_argparse"
-version = "1.1.1"
-description = "A rich help formatter for argparse"
+name = "rich-argparse"
+version = "1.2.0"
+description = "Rich help formatters for argparse and optparse"
 authors = [
   {name="Ali Hamdan", email="ali.hamdan.dev@gmail.com"},
 ]
 readme = "README.md"
 license = "MIT"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
@@ -21,32 +21,28 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Topic :: Software Development :: User Interfaces",
 ]
-keywords = ["argparse", "rich", "help-formatter"]
+keywords = ["argparse", "rich", "help-formatter", "optparse"]
 dependencies = [
   "rich >= 11.0.0",
 ]
 requires-python = ">=3.7"
 
 [project.urls]
 Homepage = "https://github.com/hamdanal/rich-argparse"
 Documentation = "https://github.com/hamdanal/rich-argparse#rich-argparse"
 Issue-Tracker = "https://github.com/hamdanal/rich-argparse/issues"
 Changelog = "https://github.com/hamdanal/rich-argparse/blob/main/CHANGELOG.md"
 
-[tool.hatch.build]
-sources = ["stubs"]
-include = [
-  "rich_argparse-stubs",
-  "rich_argparse.py",
-]
+[tool.hatch]
+build.packages = ["rich_argparse"]
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 envlist = py37,py38,py39,py310,py311,py312
 skip_missing_interpreters = true
 
@@ -57,38 +53,31 @@
   coverage report
   coverage html
 """
 
 [tool.black]
 line_length = 100
 
-[tool.isort]
-py_version = 37
-profile = "black"
-line_length = 100
-extra_standard_library = ["typing_extensions"]
+[tool.ruff]
+line-length = 100
+select = ["E", "F", "C", "B", "UP", "RUF100", "TID"]
+unfixable = ["B"]
+ignore = ["E501"]
+isort.required-imports = ["from __future__ import annotations"]
+flake8-tidy-imports.ban-relative-imports = "all"
 
 [tool.mypy]
 python_version = "3.7"
 strict = true
-explicit_package_bases = true
 
 [[tool.mypy.overrides]]
 module = ["tests.*"]
 check_untyped_defs = false
 disallow_untyped_defs = false
 disallow_incomplete_defs = false
 
-[tool.pyright]
-stubPath = "stubs"
-include = ["rich_argparse.py"]
-
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 
 [tool.coverage.run]
 plugins = ["covdefaults"]
 source = ["rich_argparse", "tests"]
-
-[tool.coverage.report]
-ignore_errors = true
-fail_under = 100
```

### Comparing `rich_argparse-1.1.1/PKG-INFO` & `rich_argparse-1.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
-Name: rich_argparse
-Version: 1.1.1
-Summary: A rich help formatter for argparse
+Name: rich-argparse
+Version: 1.2.0
+Summary: Rich help formatters for argparse and optparse
 Project-URL: Homepage, https://github.com/hamdanal/rich-argparse
 Project-URL: Documentation, https://github.com/hamdanal/rich-argparse#rich-argparse
 Project-URL: Issue-Tracker, https://github.com/hamdanal/rich-argparse/issues
 Project-URL: Changelog, https://github.com/hamdanal/rich-argparse/blob/main/CHANGELOG.md
 Author-email: Ali Hamdan <ali.hamdan.dev@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
-Keywords: argparse,help-formatter,rich
+Keywords: argparse,help-formatter,optparse,rich
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -36,26 +36,37 @@
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/hamdanal/rich-argparse/main.svg)
 ](https://results.pre-commit.ci/latest/github/hamdanal/rich-argparse/main)
 [![Python Version](https://img.shields.io/pypi/pyversions/rich-argparse)
 ![Release](https://img.shields.io/github/v/release/hamdanal/rich-argparse?sort=semver)
 ![Downloads](https://pepy.tech/badge/rich-argparse/month)
 ](https://pypi.org/project/rich-argparse/)
 
-Format argparse help output using [rich](https://pypi.org/project/rich).
+Format argparse and optparse help using [rich](https://pypi.org/project/rich).
+
+## Table of contents
+
+* [Installation](#installation)
+* [Usage](#usage)
+* [Output styles](#output-styles)
+  * [Colors](#customize-the-colors)
+  * [Group names](#customize-group-name-formatting)
+  * [Syntax highlighting](#special-text-highlighting)
+  * [Usage colors](#colors-in-the-usage)
+* [Subparsers](#working-with-subparsers)
+* [Third party formatters](#working-with-third-party-formatters)
+* [Optparse](#optparse-support) (experimental)
 
 ## Installation
 
 Install from PyPI with pip or your favorite tool.
 
 ```sh
 pip install rich-argparse
 ```
 
-Or copy the file `rich_argparse.py` to your project provided you have `rich` already installed.
-
 ## Usage
 
 Simply pass `formatter_class` to the argument parser
 ```python
 import argparse
 from rich_argparse import RichHelpFormatter
 
@@ -226,7 +237,35 @@
 
  if __name__ == '__main__':
      main()
 ```
 
 Now try out some command like: `python manage.py runserver --help`. Notice how the special
 ordering of the arguments applied by django is respected by the new help formatter.
+
+## Optparse support
+rich-argparse now ships with experimental support for [optparse]. Import optparse help formatters
+from `rich_argparse.optparse`:
+
+```python
+import optparse
+from rich_argparse.optparse import IndentedRichHelpFormatter
+
+parser = optparse.OptionParser(formatter=IndentedRichHelpFormatter())
+...
+```
+
+Similar to `argparse`, you can customize the styles used by the formatter by modifying the
+`RichHelpFormatter.styles` dictionary. These are the same styles used by `argparse` but with
+the `optparse.` prefix. For example, to change the style used for the metavar of an option:
+
+```python
+RichHelpFormatter.styles["optparse.metavar"] = "italic"
+```
+
+Syntax highlighting works the same way as `argparse`.
+
+Colors in the `usage` are not supported yet.
+
+Customizing the group name format is not supported. optparse uses title case by default.
+
+[optparse]: https://docs.python.org/3/library/optparse.html
```

