# Comparing `tmp/jalali_calendar_cli-0.1.5.tar.gz` & `tmp/jalali_calendar_cli-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jalali_calendar_cli-0.1.5.tar", max compression
+gzip compressed data, was "jalali_calendar_cli-0.1.6.tar", max compression
```

## Comparing `jalali_calendar_cli-0.1.5.tar` & `jalali_calendar_cli-0.1.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-05-23 20:42:38.619220 jalali_calendar_cli-0.1.5/jalali_calendar_cli/__init__.py
--rw-r--r--   0        0        0     3653 2023-05-23 20:16:16.981447 jalali_calendar_cli-0.1.5/jalali_calendar_cli/holidays.json
--rwxr-xr-x   0        0        0    13794 2023-06-06 09:51:22.047303 jalali_calendar_cli-0.1.5/jalali_calendar_cli/jalali_calendar.py
--rw-r--r--   0        0        0      567 2023-06-06 09:52:10.604481 jalali_calendar_cli-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     4632 2023-06-06 09:51:51.076976 jalali_calendar_cli-0.1.5/readme.org
--rw-r--r--   0        0        0     5720 1970-01-01 00:00:00.000000 jalali_calendar_cli-0.1.5/setup.py
--rw-r--r--   0        0        0     5124 1970-01-01 00:00:00.000000 jalali_calendar_cli-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-23 20:42:38.619220 jalali_calendar_cli-0.1.6/jalali_calendar_cli/__init__.py
+-rw-r--r--   0        0        0     3653 2023-05-23 20:16:16.981447 jalali_calendar_cli-0.1.6/jalali_calendar_cli/holidays.json
+-rwxr-xr-x   0        0        0    15485 2023-06-30 02:34:46.148510 jalali_calendar_cli-0.1.6/jalali_calendar_cli/jalali_calendar.py
+-rw-r--r--   0        0        0      567 2023-07-02 17:56:54.099305 jalali_calendar_cli-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     8001 2023-06-30 02:35:11.587995 jalali_calendar_cli-0.1.6/readme.org
+-rw-r--r--   0        0        0     9144 1970-01-01 00:00:00.000000 jalali_calendar_cli-0.1.6/setup.py
+-rw-r--r--   0        0        0     8493 1970-01-01 00:00:00.000000 jalali_calendar_cli-0.1.6/PKG-INFO
```

### Comparing `jalali_calendar_cli-0.1.5/jalali_calendar_cli/holidays.json` & `jalali_calendar_cli-0.1.6/jalali_calendar_cli/holidays.json`

 * *Files identical despite different names*

### Comparing `jalali_calendar_cli-0.1.5/jalali_calendar_cli/jalali_calendar.py` & `jalali_calendar_cli-0.1.6/jalali_calendar_cli/jalali_calendar.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,30 +14,37 @@
     from icecream import ic, colorize as ic_colorize
 
     ic.configureOutput(outputFunction=lambda s: print(ic_colorize(s)))
 except ImportError:
     ic = lambda *a: None if not a else (a[0] if len(a) == 1 else a)
 
 
-init(autoreset=False)
+# init(autoreset=False)
+#: This actually causes 'print' to be monkey-patched to not print ANSI codes when piping.
 
 
 # Color presets for different themes
 COLOR_PRESETS = {
     "light": {
         "weekend": {"name": "LIGHTMAGENTA_EX", "true": (85, 26, 139)},
         "holiday": {"name": "LIGHTRED_EX", "true": (230, 69, 0)},
         "footnote": {"name": "LIGHTBLACK_EX", "true": (170, 170, 170)},
         "header": {"name": "BLACK", "true": (50, 50, 50)},
+        # "today": {"name": "CYAN", "true": (50, 230, 230)},
+        "today": {"name": "CYAN", "true": (255, 255, 255)},
     },
     "dark": {
         "weekend": {"name": "LIGHTMAGENTA_EX", "true": (255, 0, 255)},
         "holiday": {"name": "LIGHTRED_EX", "true": (255, 0, 0)},
         "footnote": {"name": "LIGHTBLACK_EX", "true": (128, 128, 128)},
         "header": {"name": "WHITE", "true": (255, 255, 255)},
+
+        # "today": {"name": "CYAN", "true": (30, 200, 200)},
+        "today": {"name": "CYAN", "true": (255, 120, 0)},
+        # "today": {"name": "WHITE", "true": (255, 255, 255)},
     },
 }
 
 
 def jmonth_name(month: int) -> str:
     month_names = [
         "Farvardin",
@@ -74,30 +81,35 @@
 
 def prefix_lines(text, prefix=""):
     lines = text.split("\n")  # Split text into lines
     prefixed_lines = [prefix + line for line in lines]  # Add prefix to each line
     return "\n".join(prefixed_lines)  # Join lines back into text with prefixed lines
 
 
-def generate_true_color_code(red: int, green: int, blue: int) -> str:
+def generate_true_color_code(red: int, green: int, blue: int, back=False) -> str:
     """
     Generates ANSI escape code for 24-bit true colors.
 
     Args:
         red (int): The intensity of the red color component (0-255).
         green (int): The intensity of the green color component (0-255).
         blue (int): The intensity of the blue color component (0-255).
 
     Returns:
         str: The ANSI escape code for the specified true color.
 
     """
 
-    # ANSI escape code format: \x1b[38;2;<r>;<g>;<b>m
-    escape_code = f"\x1b[38;2;{red};{green};{blue}m"
+    if back:
+        code = 48
+    else:
+        code = 38
+
+    #: @seeAlso `wh colorfg colorbg`
+    escape_code = f"\x1b[{code};2;{red};{green};{blue}m"
     return escape_code
 
 
 def get_jalali_days(year: int, month: int) -> int:
     if month <= 6:
         num_days = 31
     elif month <= 11:
@@ -105,30 +117,34 @@
     else:  # Esfand
         j_date = jdatetime.date(year, month, 1)
         num_days = 29 if not j_date.isleap() else 30
     return num_days
 
 
 def generate_calendar(
+    today: datetime,
     year: int,
     month: int,
     first_day_of_month: int,
     num_days: int,
     holidays: dict,
     indentation: int = 5,
     color: bool = False,
     unicode_p: bool = True,
     true_color: bool = False,
     color_preset: str = "light",
     weekend_color=None,
     holiday_color=None,
     footnote_color=None,
     header_color=None,
+    today_color=None,
 ) -> List[str]:
-    assert indentation >= 4
+    assert indentation >= 3
+
+    # ic(color)
 
     weekdays = [
         "Sat",
         "Sun",
         "Mon",
         "Tue",
         "Wed",
@@ -145,36 +161,50 @@
     preset = COLOR_PRESETS[color_preset]
 
     # Determine color options
     weekend_color = weekend_color if weekend_color else preset["weekend"]
     holiday_color = holiday_color if holiday_color else preset["holiday"]
     footnote_color = footnote_color if footnote_color else preset["footnote"]
     header_color = header_color if header_color else preset["header"]
+    today_color = today_color if today_color else preset["today"]
 
-    # Determine color start values
-    if true_color:
+    if not color:
+        weekend_color_ansi = ""
+        holiday_color_ansi = ""
+        footnote_color_ansi = ""
+        header_color_ansi = ""
+        today_color_ansi = ""
+    elif true_color:
         weekend_color_ansi = generate_true_color_code(*weekend_color["true"])
         holiday_color_ansi = generate_true_color_code(*holiday_color["true"])
         footnote_color_ansi = generate_true_color_code(*footnote_color["true"])
         header_color_ansi = generate_true_color_code(*header_color["true"])
+        today_color_ansi = generate_true_color_code(*today_color["true"], back=True)
     else:
         weekend_color_ansi = getattr(colorama.Fore, weekend_color["name"])
         holiday_color_ansi = getattr(colorama.Fore, holiday_color["name"])
         footnote_color_ansi = getattr(colorama.Fore, footnote_color["name"])
         header_color_ansi = getattr(colorama.Fore, header_color["name"])
+        today_color_ansi = getattr(colorama.Back, today_color["name"])
 
     bold_ansi = Style.BRIGHT if color else ""
     reset_color = Style.RESET_ALL if color else ""
 
     last_indentation_debt = header_indentation_len
     for day in range(1, num_days + 1):
         weekday = (day + first_day_of_month) % 7
         day_str = str(day)
+        day_str_orig_len = len(day_str)
         day_str = day_str.rjust(indentation - last_indentation_debt)
         last_indentation_debt = 0
+        if today.date().year == year and today.date().month == month and today.date().day == day:
+            # bg_len = (day_str_orig_len + 1)
+            bg_len = 3
+
+            day_str = f"{day_str[:-bg_len]}{bold_ansi}{today_color_ansi}{day_str[-bg_len:]}{reset_color}"
 
         if day in holidays:
             footnotes.append(f"{day:2d}: {holidays[day]}")
 
             if (
                 False
             ):  #: @cruft no need to use footnotes when the days can act as indices already
@@ -224,33 +254,36 @@
         }
         return holidays
     else:
         return dict()
 
 
 def jalali_calendar(
+    today: datetime,
     year: int,
     month: int,
     color: bool,
     unicode_p: bool,
     indentation: int,
     true_color: bool,
     holidays_data,
     footnotes_p: bool = True,
     color_preset: str = "light",
     weekend_color=None,
     holiday_color=None,
     footnote_color=None,
     header_color=None,
+    today_color=None,
 ) -> None:
     j_date = jdatetime.date(year, month, 1)
     first_day_of_month = j_date.weekday()
     num_days = get_jalali_days(year, month)
     holidays = load_holidays(holidays_data, year, month)
     calendar, footnotes = generate_calendar(
+        today,
         year,
         month,
         first_day_of_month,
         num_days,
         holidays,
         indentation=indentation,
         color=color,
@@ -377,14 +410,20 @@
     )
     true_color_group.add_argument(
         "--header-true-color",
         type=str,
         default=None,
         help="RGB values for header color in 24-bit true color",
     )
+    true_color_group.add_argument(
+        "--today-true-color",
+        type=str,
+        default=None,
+        help="RGB values for the current day's color",
+    )
 
     colorama_color_group = parser.add_argument_group("colorama 256 color options")
     colorama_color_group.add_argument(
         "--weekend-color",
         type=str,
         default=None,
         help="colorama color name for weekend color",
@@ -404,21 +443,27 @@
     )
     colorama_color_group.add_argument(
         "--header-color",
         type=str,
         default=None,
         help="colorama color name for header color",
     )
+    colorama_color_group.add_argument(
+        "--today-color",
+        type=str,
+        default=None,
+        help="colorama color name for the current day",
+    )
 
     args = parser.parse_args()
 
-    color = args.color == "always" or (args.color == "auto" and sys.stdout.isatty())
+    color = (args.color == "always") or (args.color == "auto" and sys.stdout.isatty())
 
     colors = dict()
-    color_keys = ["weekend", "holiday", "footnote", "header"]
+    color_keys = ["weekend", "holiday", "footnote", "header", "today"]
     if args.true_color:
         for color_key in color_keys:
             color_arg = getattr(args, f"{color_key}_true_color", None)
             if color_arg:
                 if color_key not in colors:
                     colors[color_key] = dict()
                 colors[color_key]["true"] = tuple(map(int, color_arg.split(",")))
@@ -430,33 +475,36 @@
                     colors[color_key] = dict()
                 colors[color_key]["name"] = color_arg.upper()
 
     weekend_color = colors.get("weekend", None)
     holiday_color = colors.get("holiday", None)
     footnote_color = colors.get("footnote", None)
     header_color = colors.get("header", None)
+    today_color= colors.get("today", None)
 
     unicode_p = True
     # unicode_p = args.unicode
 
     with open(args.holidays_json_path) as f:
         holidays_data = json.load(f)
 
     jalali_calendar(
+        now_jalali,
         args.year,
         args.month,
         color,
         unicode_p,
         args.indentation,
         args.true_color,
         holidays_data=holidays_data,
         footnotes_p=args.footnotes,
         color_preset=args.color_preset,
         weekend_color=weekend_color,
         holiday_color=holiday_color,
         footnote_color=footnote_color,
         header_color=header_color,
+        today_color=today_color,
     )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `jalali_calendar_cli-0.1.5/pyproject.toml` & `jalali_calendar_cli-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jalali-calendar-cli"
-version = "0.1.5"
+version = "0.1.6"
 description = "Jalali (Shamsi) calendar in your terminal, with holidays"
 authors = ["NightMachinery <feraidoonmehri@gmail.com>"]
 readme = "readme.org"
 packages = [{include = "jalali_calendar_cli"}]
 
 
 [tool.poetry.scripts]
```

