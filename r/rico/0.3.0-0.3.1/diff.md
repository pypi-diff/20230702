# Comparing `tmp/rico-0.3.0.tar.gz` & `tmp/rico-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rico-0.3.0.tar", last modified: Sat Jun 24 08:02:03 2023, max compression
+gzip compressed data, was "rico-0.3.1.tar", last modified: Sun Jul  2 10:43:10 2023, max compression
```

## Comparing `rico-0.3.0.tar` & `rico-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1070 2023-06-24 08:01:28.246842 rico-0.3.0/LICENSE
--rw-r--r--   0        0        0    15333 2023-06-24 08:01:28.246842 rico-0.3.0/README.md
--rw-r--r--   0        0        0     2955 2023-06-24 08:02:03.107859 rico-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      710 2023-06-24 08:01:28.246842 rico-0.3.0/src/rico/__init__.py
--rw-r--r--   0        0        0     5469 2023-06-24 08:01:28.246842 rico-0.3.0/src/rico/_config.py
--rw-r--r--   0        0        0     5629 2023-06-24 08:01:28.246842 rico-0.3.0/src/rico/_container.py
--rw-r--r--   0        0        0    14852 2023-06-24 08:01:28.246842 rico-0.3.0/src/rico/_content.py
--rw-r--r--   0        0        0     7031 2023-06-24 08:01:28.246842 rico-0.3.0/src/rico/_html.py
--rw-r--r--   0        0        0      340 2023-06-24 08:01:28.246842 rico-0.3.0/src/rico/_version.py
--rw-r--r--   0        0        0       18 2023-06-24 08:01:28.246842 rico-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0     1476 2023-06-24 08:01:28.246842 rico-0.3.0/tests/test__config.py
--rw-r--r--   0        0        0    10248 2023-06-24 08:01:28.246842 rico-0.3.0/tests/test__container.py
--rw-r--r--   0        0        0    17099 2023-06-24 08:01:28.246842 rico-0.3.0/tests/test__content.py
--rw-r--r--   0        0        0     8907 2023-06-24 08:01:28.246842 rico-0.3.0/tests/test__html.py
--rw-r--r--   0        0        0      730 2023-06-24 08:01:28.246842 rico-0.3.0/tests/test__version.py
--rw-r--r--   0        0        0    16989 1970-01-01 00:00:00.000000 rico-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-02 10:42:37.317854 rico-0.3.1/LICENSE
+-rw-r--r--   0        0        0    16506 2023-07-02 10:42:37.317854 rico-0.3.1/README.md
+-rw-r--r--   0        0        0     2955 2023-07-02 10:43:10.933957 rico-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      710 2023-07-02 10:42:37.321854 rico-0.3.1/src/rico/__init__.py
+-rw-r--r--   0        0        0     6399 2023-07-02 10:42:37.321854 rico-0.3.1/src/rico/_config.py
+-rw-r--r--   0        0        0     5509 2023-07-02 10:42:37.321854 rico-0.3.1/src/rico/_container.py
+-rw-r--r--   0        0        0    13794 2023-07-02 10:42:37.321854 rico-0.3.1/src/rico/_content.py
+-rw-r--r--   0        0        0     7951 2023-07-02 10:42:37.321854 rico-0.3.1/src/rico/_html.py
+-rw-r--r--   0        0        0      340 2023-07-02 10:42:37.321854 rico-0.3.1/src/rico/_version.py
+-rw-r--r--   0        0        0       18 2023-07-02 10:42:37.321854 rico-0.3.1/tests/__init__.py
+-rw-r--r--   0        0        0     1476 2023-07-02 10:42:37.321854 rico-0.3.1/tests/test__config.py
+-rw-r--r--   0        0        0    10250 2023-07-02 10:42:37.321854 rico-0.3.1/tests/test__container.py
+-rw-r--r--   0        0        0    17254 2023-07-02 10:42:37.321854 rico-0.3.1/tests/test__content.py
+-rw-r--r--   0        0        0    10803 2023-07-02 10:42:37.321854 rico-0.3.1/tests/test__html.py
+-rw-r--r--   0        0        0      730 2023-07-02 10:42:37.321854 rico-0.3.1/tests/test__version.py
+-rw-r--r--   0        0        0    18162 1970-01-01 00:00:00.000000 rico-0.3.1/PKG-INFO
```

### Comparing `rico-0.3.0/LICENSE` & `rico-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rico-0.3.0/README.md` & `rico-0.3.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 # rico: rich content to HTML as easy as Doc(df, plot)
 
 **rico** is a Python package for creating HTML documents from rich content: dataframes, plots, images, markdown etc. It provides a high-level, easy-to-use API with reasonable defaults, as well as low-level access for better control.
 
+Use **rico** if you want to create an HTML document from objects created in a Python script.
+
+With **rico** you can *avoid*:
+* Writing data to intermediate files or a database from a script.
+* Loading data into a Jupyter notebook from intermediate files or a database.
+* Using nbconvert or similar tools for creating HTML files.
+
+More on the topic:
+* [Pass pandas dataframe to notebook via nbconvert](https://github.com/jupyter/nbconvert/issues/1070).
+* [Could Papermill pass an in-memory dataframe to a notebook?](https://github.com/nteract/papermill/issues/406)
+
 [![CI](https://github.com/e10v/rico/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/e10v/rico/actions/workflows/ci.yml)
 [![Coverage](https://codecov.io/github/e10v/rico/coverage.svg?branch=main)](https://codecov.io/gh/e10v/rico)
 [![License](https://img.shields.io/github/license/e10v/rico)](https://github.com/e10v/rico/blob/main/LICENSE)
 [![Version](https://img.shields.io/pypi/v/rico.svg)](https://pypi.org/project/rico/)
 [![Package Status](https://img.shields.io/pypi/status/rico.svg)](https://pypi.org/project/rico/)
 [![PyPI Python Versions](https://img.shields.io/pypi/pyversions/rico.svg)](https://pypi.org/project/rico/)
 
@@ -38,15 +49,15 @@
 ```
 
 [Seaborn](https://seaborn.pydata.org/):
 ```bash
 pip install rico[seaborn]
 ```
 
-Install `rico[seaborn]` extra only to use the [seaborn.objects](https://seaborn.pydata.org/tutorial/objects_interface.html) interface. Otherwise install `rico[pyplot]` as the old plotting functions return Matplotlib Pyplot Axes objects.
+Install `rico[seaborn]` extra only to use the [seaborn.objects](https://seaborn.pydata.org/tutorial/objects_interface.html) interface. Otherwise install `rico[pyplot]` as the old Seaborn plotting functions return Matplotlib Pyplot Axes objects.
 
 All extras:
 ```bash
 pip install rico[complete]
 ```
 
 ## User guide
@@ -99,27 +110,27 @@
 
 Implicit serialization:
 ```python
 with open("doc.html", "w") as f:
     print(doc, file=f)
 ```
 
-Internally, `str(doc)` calls `doc.serialize()` with default parameter values. Call `doc.serialize()` to indent the HTML element tree visually:
+Internally, `str(doc)` calls `doc.serialize()` with default parameter values. Call `doc.serialize(indent=True)` to indent the HTML element tree visually:
 ```python
 with open("doc.html", "w") as f:
     f.write(doc.serialize(indent=True))
 ```
 
 Set custom whitespace for indentation using the `space` parameter:
 ```python
 with open("doc.html", "w") as f:
     f.write(doc.serialize(indent=True, space="    "))
 ```
 
-Remove unnecessary whitespace between tags by setting `strip` to `True`:
+Remove unnecessary whitespace by setting `strip` to `True`:
 ```python
 with open("doc.html", "w") as f:
     f.write(doc.serialize(strip=True))
 ```
 
 Control the default behavior of `str(doc)` and `doc.serialize()` using the global options `indent_html`, `indent_space`, and `strip_html`:
 ```python
@@ -146,15 +157,15 @@
     rico.Text("Hello world!", mono=True),  # The default value is False.
     df,
     rico.Plot(plot, format="png"),  # The default value is "svg".
     title="My doc",
 )
 ```
 
-Or:
+The following code gives the same result as the code above:
 ```python
 doc = rico.Doc(title="My doc")
 doc.append_text("Hello world!", mono=True)
 doc.append(df)
 doc.append_plot(plot, format="png")
 ```
 
@@ -167,41 +178,41 @@
 Use specific classes and methods for other content types:
 * Images: `Image` or `Doc.append_image`.
 * Code: `Code` or `Doc.append_code`.
 * Markdown: `Markdown` or `Doc.append_markdown`.
 * HTML tag: `Tag` or `Doc.append_tag`.
 * Raw HTML: `HTML` or `Doc.append_html`.
 
-Example:
+For example:
 ```python
 doc = rico.Doc(
     rico.Markdown("## Dataframe"),
     df,
     rico.Tag("h2", "Plot"),  # An alternative way to add a header.
     plot,
     rico.HTML("<h2>Code</h2>"),  # Another way to add a header.
     rico.Code("print('Hello world!')"),
     title="My doc",
 )
 ```
 
-Or:
+The following code gives the same result as the code above:
 ```python
 doc = rico.Doc(title="My doc")
 doc.append_markdown("## Dataframe")
 doc.append(df)
 doc.append_tag("h2", "Plot")
 doc.append(plot)
 doc.append_html("<h2>Code</h2>")
 doc.append_code("print('Hello world!')")
 ```
 
-Check the docstrings for additional parameters.
+Check the docstrings for details.
 
-Serialize content to HTML using `str()` or `object.serialize()`:
+Serialize content to HTML using `str(object)` or `object.serialize()`:
 ```python
 obj = rico.Tag("p", "Hello world!")
 
 print(obj)
 # <div><p>Hello world!</p></div>
 
 print(obj.serialize(indent=True, space="    "))
@@ -213,18 +224,17 @@
 ### Bootstrap, HTML classes and document layout
 
 By default, [Bootstrap](https://getbootstrap.com/) styles are included in the document. Change the default behavior using the `bootstrap` parameter:
 ```python
 doc = rico.Doc("Hello world!", bootstrap="full")
 ```
 
-The possible values are:
-* `"css"` (default) -- include only CSS.
-* `"full"` -- include both the CSS and JS.
-* `"none"` -- don't include Bootstrap*.
+* Set `bootstrap` to `"css"` (default) to include only CSS.
+* Set `bootstrap` to `"full"` to include both the CSS and JS.
+* Set `bootstrap` to `"none"` to not include Bootstrap*.
 
 *Keep in mind that **rico** relies on Bootstrap classes and styles. For example:
 * The `mono` and `wrap` parameters of the `Text` class use Bootstrap's `font-monospace` and `font-monospace` classes.
 * **rico**'s dataframe style definition uses Bootstrap variables.
 
 Each content element is wrapped in a `<div>` container. Specify the element's container class using the `class_` parameter:
 ```python
@@ -260,15 +270,15 @@
         rico.Obj("Plot", plot, class_="col"),
         class_="row row-cols-auto",
     ),
     title="My doc",
 )
 ```
 
-Or:
+The following code gives the same result as the code above:
 ```python
 doc = rico.Doc(title="My doc")
 doc.append_tag("h1", "My doc")
 doc.append_tag("h2", "Description")
 doc.append("This is an example of custom document layout using Bootstrap classes.")
 doc.append_tag("h2", "Data")
 div = rico.Div(class_="row row-cols-auto")
@@ -302,86 +312,97 @@
 ```python
 with rico.config_context(dataframe_style=""):
     doc = rico.Doc(df)
 ```
 
 Include custom styles and scripts using the `Style` and `Script` classes:
 ```python
-css = "https://cdn.jsdelivr.net/npm/bootstrap-icons@1/font/bootstrap-icons.css"
-js = "https://cdn.jsdelivr.net/npm/jquery@3.7.0/dist/jquery.min.js"
+dark_theme = "https://cdn.jsdelivr.net/npm/bootswatch@5/dist/darkly/bootstrap.min.css"
+jquery = "https://cdn.jsdelivr.net/npm/jquery@3/dist/jquery.min.js"
 
 doc = rico.Doc(
-    "Hello world",
+    rico.Text("Click me", class_="click"),
     extra_styles=(
-        rico.Style("p {color: red;}"),
-        rico.Style(src=css),
+        rico.Style(src=dark_theme),
+        rico.Style(".click {color: red;}"),
     ),
     extra_scripts=(
-        rico.Script("alert('Hello World!');"),
-        rico.Script(src=js),
+        rico.Script(src=jquery),
+        rico.Script(
+            "$('p').on('click', function() {alert('Hello world!');})",
+            defer=True,
+        ),
     ),
 )
 ```
 
+The `defer` parameter adds the `defer` attribute to the `<script>` tag if the `src` parameter is used. Otherwise, if the `text` parameter is used, the script is placed in the footer of the document.
+
 By default, external styles and scripts are included as file links. This means that these files must be available when someone opens the document. Include the contents of these files in the document using the `inline` parameter:
 ```python
 doc = rico.Doc(
-    "Hello world",
+    rico.Text("Click me", class_="click"),
     extra_styles=(
-        rico.Style("p {color: red;}"),
-        rico.Style(src=css, inline=True),
+        rico.Style(src=dark_theme, inline=True),
+        rico.Style(".click {color: red;}"),
     ),
     extra_scripts=(
-        rico.Script("alert('Hello World!');"),
-        rico.Script(src=js, inline=True),
+        rico.Script(src=jquery, inline=True),
+        rico.Script(
+            "$('p').on('click', function() {alert('Hello world!');})",
+            defer=True,
+        ),
     ),
 )
 ```
 
 In the example above, the Bootstrap styles are still included as a link. Use the global options `inline_styles` and `inline_scripts` to include the contents of the style and script files in the document:
 ```python
 with rico.config_context(inline_styles=True, inline_scripts=True):
     doc = rico.Doc(
-        "Hello world",
+        rico.Text("Click me", class_="click"),
         extra_styles=(
-            rico.Style("p {color: red;}"),
-            rico.Style(src=css),
+            rico.Style(src=dark_theme),
+            rico.Style(".click {color: red;}"),
         ),
         extra_scripts=(
-            rico.Script("alert('Hello World!');"),
-            rico.Script(src=js),
+            rico.Script(src=jquery),
+            rico.Script(
+                "$('p').on('click', function() {alert('Hello world!');})",
+                defer=True,
+            ),
         ),
     )
 ```
 
 ### Global configuration
 
 Use global configuration to:
 * Get or set default parameter values.
 * Get or set document properties.
 
-The following globals options define the default parameter values:
+The following global options define the default parameter values:
 
 | Global option    | Parameter | Classes, methods, functions       |
 |:-----------------|:----------|:----------------------------------|
 | `indent_html`    | `indent`  | `obj.serialize`, `serialize_html` |
 | `indent_space`   | `space`   | `obj.serialize`, `serialize_html` |
 | `strip_html`     | `strip`   | `obj.serialize`, `serialize_html` |
 | `text_mono`      | `mono`    | `Text`, `obj.append_text`         |
 | `text_wrap`      | `wrap`    | `Text`, `obj.append_text`         |
 | `image_format`   | `format`  | `Plot`, `obj.append_plot`         |
 | `inline_styles`  | `inline`  | `Style`                           |
 | `inline_scripts` | `inline`  | `Script`                          |
 
-The following globals options define document properties:
-* `meta_charset` defines a document [charset](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/meta#charset) metadata.
-* `meta_viewport` defines a document [viewport](https://developer.mozilla.org/en-US/docs/Web/HTML/Viewport_meta_tag) metadata.
+The following global options define document properties:
+* `meta_charset` defines a document [charset](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/meta#charset) metadata. Set it to `""` to disable.
+* `meta_viewport` defines a document [viewport](https://developer.mozilla.org/en-US/docs/Web/HTML/Viewport_meta_tag) metadata. Set it to `""` to disable.
 * `bootstrap_css` defines a link to the Bootstrap CSS file.
 * `bootstrap_js` defines a link to the Bootstrap JS file.
-* `dataframe_style` defines a dataframe style.
+* `dataframe_style` defines a dataframe style. Set it to `""` to disable.
 
 Get a dictionary with global options using `get_config` without parameters:
 ```python
 global_config = rico.get_config()
 print(global_config["indent_html"])
 # False
 ```
@@ -414,36 +435,33 @@
 
 Internally, **rico** uses the standard [xml.etree.ElementTree](https://docs.python.org/3/library/xml.etree.elementtree.html) module:
 * Every content object (`Tag`, `Text`, `Div` etc.) has a `container` attribute of type `xml.etree.ElementTree.Element`. The value is a `<div>` container element.
 * `Doc` objects has additional attributes `html`, `head`, and `body` of type `xml.etree.ElementTree.Element`. They represent the `<html>`, `<head>`, and `<body>` elements, respectively.
 
 Access these attributes and use `xml.etree.ElementTree` API to gain low-level control over the document and its elements.
 
-## Use case and alternatives
+Also, **rico** provides the following functions for working with `xml.etree.ElementTree.Element` objects:
+* `parse_html` parses HTML from a string.
+* `indent_html` indents an HTML element tree visually.
+* `strip_html` removes unnecessary whitespace.
+* `serialize_html` serializes `xml.etree.ElementTree.Element` object.
 
-Use **rico** if you want to create an HTML document from objects created in a Python script.
+Check the docstrings for details.
 
-With **rico** you can avoid:
-* Writing data to intermediate files or a database from a script.
-* Loading data into a Jupyter notebook.
-* Using [nbconvert](https://nbconvert.readthedocs.io/) or similar tools.
+## Alternatives
 
-Alternatives:
 * Use [Jupyter Notebook](https://jupyter.org/) for interactive computing.
 * Use [nbconvert](https://nbconvert.readthedocs.io/) or [papermill](https://papermill.readthedocs.io/) if you're processing data and creating objects for a document in a Jupyter notebook.
 * Use [Quarto](https://quarto.org/) if you prefer R Markdown style notebooks and a variety of output formats.
 * Use [xml.etree.ElementTree](https://docs.python.org/3/library/xml.etree.elementtree.html), [lxml](https://lxml.de/), [Yattag](https://www.yattag.org/), or [Airium](https://gitlab.com/kamichal/airium) if you need low-level control.
 
 More on the topic:
-* [Pass pandas dataframe to notebook via nbconvert](https://github.com/jupyter/nbconvert/issues/1070).
-* [Could Papermill pass an in-memory dataframe to a notebook?](https://github.com/nteract/papermill/issues/406)
 * "I Don’t Like Notebooks": [video](https://www.youtube.com/watch?v=7jiPeIFXb6U), [slides](https://docs.google.com/presentation/d/1n2RlMdmv1p25Xy5thJUhkKGvjtV-dkAIsUXP-AL4ffI/edit#slide=id.g362da58057_0_1).
 * [The First Notebook War](https://yihui.org/en/2018/09/notebook-war/).
 
 ## Roadmap
 
+* Support most of IPython rich representation [methods](https://ipython.readthedocs.io/en/stable/config/integrating.html#rich-display).
 * Create docs with [MkDocs](https://www.mkdocs.org/) and [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/).
+* Create short quick start.
+* Create examples with resulting HTML files.
 * Support math with [KaTeX](https://katex.org/).
-* Save Altair Charts in [Vega-Lite](https://vega.github.io/vega-lite/) format.
-* Save SVG images in XML format.
-* Support diagrams with [Mermaid.js](https://mermaid.js.org/).
-* Support other plot types: [Plotly](https://plotly.com/python/), [Bokeh](https://bokeh.org/).
```

### Comparing `rico-0.3.0/pyproject.toml` & `rico-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Visualization",
     "Topic :: Text Processing",
     "Topic :: Text Processing :: Markup",
     "Topic :: Text Processing :: Markup :: HTML",
     "Topic :: Text Processing :: Markup :: Markdown",
 ]
-version = "0.3.0"
+version = "0.3.1"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 source = "https://github.com/e10v/rico"
 "release notes" = "https://github.com/e10v/rico/releases"
```

### Comparing `rico-0.3.0/src/rico/__init__.py` & `rico-0.3.1/src/rico/__init__.py`

 * *Files identical despite different names*

### Comparing `rico-0.3.0/src/rico/_config.py` & `rico-0.3.1/src/rico/_config.py`

 * *Files 21% similar despite different names*

```diff
@@ -63,25 +63,26 @@
     "meta_viewport": "width=device-width, initial-scale=1",
     "strip_html": False,
     "text_mono": False,
     "text_wrap": False,
 }
 
 
-def get_config(param: str | None = None) -> Any:
+def get_config(option: str | None = None) -> Any:
     """Get global configuration.
 
     Args:
-        param: Paramater name.
+        option: The option name.
 
     Returns:
-        Parameter value if `param` is not None, or dict with all parameters otherwise.
+        The value of the option if it's not None,
+        or a dictionary with all options otherwise.
     """
-    if param is not None:
-        return _global_config[param]
+    if option is not None:
+        return _global_config[option]
     return _global_config.copy()
 
 
 def set_config(
     bootstrap_css: str | None = None,
     bootstrap_js: str | None = None,
     dataframe_style: str | None = None,
@@ -95,32 +96,36 @@
     strip_html: bool | None = None,
     text_mono: bool | None = None,
     text_wrap: bool | None = None,
 ) -> None:
     """Set global configuration.
 
     Args:
-        bootstrap_css: A link to a bootstrap css file.
-            If empty then bootstrap css is not loaded.
-        bootstrap_js: A link to a bootstrap javascript file.
-            If empty then bootstrap javascript is not loaded.
-        dataframe_style: A dataframe table stylesheet.
-            If empty then it's not used.
+        bootstrap_css: A link to the Bootstrap CSS file.
+            If empty, then the Bootstrap CSS is not loaded.
+        bootstrap_js: A link to the Bootstrap JS file.
+            If empty, then the Bootstrap JS is not loaded.
+        dataframe_style: A dataframe style. If empty, then it's not used.
         image_format: Default plot image format.
-        indent_html: Indent HTML elements in serialization methods.
-        indent_space: Default indent space.
-        inline_scripts: If True then scripts are loaded inline.
-        inline_styles: If True then styles are loaded inline.
-        meta_charset: An HTML document charset.
-            If empty then it's not used.
-        meta_viewport: An HTML document viewport property.
-            If empty then it's not used.
-        strip_html: Strip HTML elements in serialization methods.
-        text_mono: Default value for the `mono` arg of the Text class.
-        text_wrap: Default value for the `wrap` arg of the Text class.
+        indent_html: Default value of the `indent` parameter for serialization methods.
+            If True, indent the elements.
+        indent_space: Default value of the `space` parameter for serialization methods.
+            Whitespace for indentation.
+        inline_scripts: Default value of the `inline` parameter of the Script class.
+            If True, load script inline, downdload it from source link.
+        inline_styles: Default value of the `inline` parameter of the Style class.
+            If True, load stylesheet inline, downdload it from source link.
+        meta_charset: HTML document charset. If empty, then it's not used.
+        meta_viewport: HTML document viewport property. If empty, then it's not used.
+        strip_html: Default value of the `strip` parameter for serialization methods.
+            If True, strip unnecessary whitespace.
+        text_mono: Default value of the `mono` parameter of the Text class.
+            If True, set the text font to monospaced.
+        text_wrap: Default value of the `wrap` parameter of the Text class.
+            If True, wrap the text.
     """
     for param, value in locals().items():
         if value is not None:
             _global_config[param] = value
 
 
 @contextlib.contextmanager
@@ -138,32 +143,36 @@
     strip_html: bool | None = None,
     text_mono: bool | None = None,
     text_wrap: bool | None = None,
 ) -> Generator[None, Any, None]:
     """Context manager for configuration.
 
     Args:
-        bootstrap_css: A link to a bootstrap css file.
-            If empty then bootstrap css is not loaded.
-        bootstrap_js: A link to a bootstrap javascript file.
-            If empty then bootstrap javascript is not loaded.
-        dataframe_style: A dataframe table stylesheet.
-            If empty then it's not used.
+        bootstrap_css: A link to the Bootstrap CSS file.
+            If empty, then the Bootstrap CSS is not loaded.
+        bootstrap_js: A link to the Bootstrap JS file.
+            If empty, then the Bootstrap JS is not loaded.
+        dataframe_style: A dataframe style. If empty, then it's not used.
         image_format: Default plot image format.
-        indent_html: Indent HTML elements in serialization methods.
-        indent_space: Default indent space.
-        inline_scripts: If True then scripts are loaded inline.
-        inline_styles: If True then styles are loaded inline.
-        meta_charset: An HTML document charset.
-            If empty then it's not used.
-        meta_viewport: An HTML document viewport property.
-            If empty then it's not used.
-        strip_html: Strip HTML elements in serialization methods.
-        text_mono: Default value for the `mono` arg of the Text class.
-        text_wrap: Default value for the `wrap` arg of the Text class.
+        indent_html: Default value of the `indent` parameter for serialization methods.
+            If True, indent the elements.
+        indent_space: Default value of the `space` parameter for serialization methods.
+            Whitespace for indentation.
+        inline_scripts: Default value of the `inline` parameter of the Script class.
+            If True, load script inline, downdload it from source link.
+        inline_styles: Default value of the `inline` parameter of the Style class.
+            If True, load stylesheet inline, downdload it from source link.
+        meta_charset: HTML document charset. If empty, then it's not used.
+        meta_viewport: HTML document viewport property. If empty, then it's not used.
+        strip_html: Default value of the `strip` parameter for serialization methods.
+            If True, strip unnecessary whitespace.
+        text_mono: Default value of the `mono` parameter of the Text class.
+            If True, set the text font to monospaced.
+        text_wrap: Default value of the `wrap` parameter of the Text class.
+            If True, wrap the text.
     """
     new_config = locals()
     old_config = get_config()
     set_config(**new_config)
 
     try:
         yield
```

### Comparing `rico-0.3.0/src/rico/_container.py` & `rico-0.3.1/src/rico/_container.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,23 +31,21 @@
         content = content_type(*args, **kwargs)
         self.container.append(content.container)
 
     return method
 
 
 class Div(rico._content.ContentBase):
-    """A <div> container definition.
-
-    Creates <div> container with content based on arbitrary objects.
-    """
     def __init__(self, *objects: Any, class_: str | None = None):
-        """Create <div> container with content from arbitrary objects.
+        """Create a <div> container, create HTML elements and add them to the container.
+
+        Each HTML element is also wrapped in a separate <div> container.
 
         Args:
-            *objects: The objects which are used to create a content.
+            *objects: Objects that are used to create HTML elements.
             class_: The container class attribute.
         """
         super().__init__(class_=class_)
         for obj in objects:
             if isinstance(obj, rico._content.ContentBase):
                 self.container.append(obj.container)
             else:
@@ -61,46 +59,42 @@
     append_image = _append(rico._content.Image, rico._content.Image.__init__)
     append_plot = _append(rico._content.Plot, rico._content.Plot.__init__)
     append_chart = _append(rico._content.Chart, rico._content.Chart.__init__)
     append = _append(rico._content.Obj, rico._content.Obj.__init__)
 
 
 class Doc(Div):
-    """Creates an HTML document.
-
-    Creates and HTML document with content based on arbitrary objects.
-
-    Attributes:
-        html (Element): The <html> element.
-        head (Element): The <head> element.
-        body (Element): The <body> element.
-        container (Element): The <div> container element.
-    """
     html: ET.Element
     head: ET.Element
     body: ET.Element
-    container: ET.Element
 
     def __init__(
         self,
         *objects: Any,
         title: str | None = None,
         bootstrap: Literal["css", "full", "none"] = "css",
         extra_styles: Iterable[rico._content.Style] = (),
         extra_scripts: Iterable[rico._content.Script] = (),
         class_: str | None = "container",
     ):
-        """Create an HTML document with content from arbitrary objects.
+        """Create an HTML document.
+
+        Creates a <div> container inside the <body> element.
+        Create HTML elements and add them to the container.
+        Each HTML element is also wrapped in a separate <div> container.
 
         Args:
-            *objects: The objects which are used to create a content.
+            *objects: Objects that are used to create HTML elements.
             title: The document title.
-            bootstrap: If True then Bootstrap included to the document.
-            extra_styles: Extra styles to be included to the document.
-            extra_scripts: Extra scripts to be included to the document.
+            bootstrap: Defines which Bootatrap files are included in the document.
+                If "css", include only CSS.
+                If "full", include both the CSS and JS.
+                If "none", don'e include Bootstrap.
+            extra_styles: Extra styles to include in the document.
+            extra_scripts: Extra scripts to include in the document.
             class_: The container class attribute.
         """
         super().__init__(*objects, class_=class_)
         self.html = ET.Element("html")
         self.head = ET.Element("head")
         self.body = ET.Element("body")
         self.html.append(self.head)
@@ -143,21 +137,19 @@
 
     def serialize(
         self,
         indent: bool | None = None,
         space: str | None = None,
         strip: bool | None = None,
     ) -> str:
-        """Serialize the document to string in HTML format.
-
-        Indent the object if `indent_space` is not None.
+        """Serialize the HTML document to s string.
 
         Args:
-            indent: If True, indent the element.
-            space: The whitespace for indentation.
+            indent: If True, indent the elements.
+            space: Whitespace for indentation.
             strip: If True, strip unnecessary whitespace.
 
         Returns:
-            The serialized document.
+            A string with serialized HTML.
         """
         return "<!doctype html>\n" + rico._html.serialize_html(
             self.html, indent=indent, space=space, strip=strip)
```

### Comparing `rico-0.3.0/src/rico/_content.py` & `rico-0.3.1/src/rico/_content.py`

 * *Files 14% similar despite different names*

```diff
@@ -36,114 +36,95 @@
 try:
     import seaborn.objects as so
 except ImportError:
     so = None
 
 
 class ContentBase:
-    """A base content definition.
-
-    Creates a container element on init.
-    Defines serialization method and string representation.
-
-    Attributes:
-        container (Element): The container element.
-    """
     container: ET.Element
 
     def __init__(self, class_: str | None = None):
-        """Create base content.
+        """Create an empty <div> container.
 
         Args:
-            class_: The container element's class attribute.
+            class_: The container class attribute.
         """
         attrib = {"class": class_} if class_ is not None else {}
         self.container = ET.Element("div", attrib=attrib)
 
     def serialize(
         self,
         indent: bool | None = None,
         space: str | None = None,
         strip: bool | None = None,
     ) -> str:
-        """Serialize the object to string in HTML format.
-
-        Indent the object if `indent_space` is not None.
+        """Serialize the object's HTML elements to a string.
 
         Args:
-            indent: If True, indent the element.
-            space: The whitespace for indentation.
+            indent: If True, indent the elements.
+            space: Whitespace for indentation.
             strip: If True, strip unnecessary whitespace.
 
         Returns:
-            The serialized object.
+            A string with serialized HTML.
         """
         return rico._html.serialize_html(
             self.container, indent=indent, space=space, strip=strip)
 
     def __str__(self) -> str:
-        """Serialize the object to string in HTML format."""
+        """Serialize the object's HTML elements to a string."""
         return self.serialize()
 
 
 class Tag(ContentBase):
-    """A Tag content definition.
-
-    Creates a content element using tag parameters and appends it to the container.
-    """
-
     def __init__(
         self,
         tag: str,
         text: str | None = None,
         tail: str | None = None,
         attrib: dict[str, Any] = {},
         class_: str | None = None,
         **extra: Any,
     ):
-        """Create content using tag parameters.
+        """Create an HTML element using tag parameters and wrap it in a <div> container.
 
         Args:
-            tag: The content element's tag.
+            tag: The tag name.
             text: Text before first subelement.
-            tail: Text after the end tag.
+            tail: Text after the closing tag.
             attrib: The tag's attributes.
             extra: Extra attributes.
             class_: The container class attribute.
         """
         super().__init__(class_)
         element = ET.Element(tag, attrib={**attrib, **extra})
         element.text = text
         element.tail = tail
         self.container.append(element)
 
 
 class Text(ContentBase):
-    """A Text content definition.
-
-    Creates a content element from a text and appends it to the container.
-    """
     def __init__(
         self,
         obj: Any,
         mono: bool | None = None,
         wrap: bool | None = None,
         class_: str | None = None,
     ):
-        """Create content from a text.
+        """Create an HTML element from text and wrap it in a <div> container.
 
-        The default tag is <p> unless the text contains a line break.
-        Then the <pre> tag is used.
+        The default tag is <p> if the text doesn't contains a line break.
+        Otherwise, the <pre> tag is used.
 
         The `mono` and `wrap` parameters rely on Bootstrap CSS.
 
         Args:
             obj: The text. If it's not an instance of str, then it's converted to str.
-            mono: If True then "font-monospace" class is assigned to the text element.
-            wrap: If True then "text-wrap" class is assigned to the text element.
+            mono: If True, set the text font to monospaced.
+            wrap: If True, wrap the text.
             class_: The container class attribute.
         """
         super().__init__(class_)
 
         global_config = rico._config.get_config()
         if mono is None:
             mono = global_config["text_mono"]
@@ -163,49 +144,41 @@
         attrib = {"class": text_class} if text_class else {}
         element = ET.Element(tag, attrib=attrib)
         element.text = obj
         self.container.append(element)
 
 
 class Code(ContentBase):
-    """A Code content definition.
-
-    Creates content elements from a code and appends them to the container.
-    """
     def __init__(self, text: str, class_: str | None = None):
-        """Create content from a code.
+        """Create HTML elements from code and wrap them in a <div> container.
 
         Args:
             text: The code.
             class_: The container class attribute.
         """
         super().__init__(class_)
         pre = ET.Element("pre")
         code = ET.Element("code")
         code.text = text
         pre.append(code)
         self.container.append(pre)
 
 
 class HTML(ContentBase):
-    """An HTML content definition.
-
-    Creates content elements from an HTML text and appends them to the container.
-    """
     def __init__(
         self,
         text: str,
         strip_dataframe_borders: bool = False,
         class_: str | None = None,
     ):
-        """Create content from an HTML text.
+        """Create HTML elements from raw HTML and wrap them in a <div> container.
 
         Args:
-            text: The HTML text.
-            strip_dataframe_borders: Delete borders attributes from dataframes.
+            text: A string with raw HTML.
+            strip_dataframe_borders: If True, remove borders attributes from dataframes.
             class_: The container class attribute.
         """
         super().__init__(class_)
 
         for element in rico._html.parse_html(text):
             self.container.append(element)
 
@@ -213,53 +186,47 @@
             for table in self.container.iterfind(
                 './/table[@class="dataframe"][@border]',
             ):
                 del table.attrib["border"]
 
 
 class Markdown(ContentBase):
-    """A Markdown content definition.
-
-    Creates content elements from a markdown text and appends them to the container.
-    """
     def __init__(
         self,
         text: str,
         class_: str | None = None,
         **kwargs: Any,
     ):
-        """Create content from a markdown text.
+        """Create HTML elements from Markdown text and wrap them in a <div> container.
 
         Args:
-            text: The markdown text.
+            text: The Markdown text.
             class_: The container class attribute.
             **kwargs: Keyword arguments passed to the `markdown.markdown` function.
 
         Raises:
             ImportError: The markdown package is not installed.
         """
         if markdown is None:
             raise ImportError("The markdown package is not installed.")
 
         content = HTML(markdown.markdown(text, **kwargs), class_=class_)
         self.container = content.container
 
 
 class Image(ContentBase):
-    """An Image content definition.
-
-    Creates content elements using an image data and appends them to the container.
-    """
     def __init__(
         self,
         data: bytes | str,
         mime_subtype: str,
         class_: str | None = None,
     ):
-        """Create content using image data.
+        """Create an HTML element from image data and wrap it in a <div> container.
+
+        The image is byte64-encoded.
 
         Args:
             data: The image data.
             mime_subtype: The image MIME subtype. Examples: "png", "svg+xml".
             class_: The container class attribute.
         """
         super().__init__(class_)
@@ -272,42 +239,38 @@
             "img",
             attrib={"src": f"data:image/{mime_subtype};base64,{encoded_image}"},
         )
         self.container.append(element)
 
 
 class Plot(ContentBase):
-    """A Plot content definition.
-
-    Creates content elements from a plot object and appends them to the container.
-
-    The supported plot types are the following:
-    - Altair Chart,
-    - Pyplot Axes and Figure,
-    - Seaborn Plot (seaborn.objects interface).
-    """
     def __init__(
         self,
         obj: Any,
         format: Literal["svg", "png"] | None = None,  # noqa: A002
         class_: str | None = None,
         **kwargs: Any,
     ):
-        """Create content from a plot object.
+        """Create an HTML element from a plot object and wrap it in a <div> container.
+
+        The supported plot types are the following:
+        - Altair Chart,
+        - Pyplot Axes and Figure,
+        - Seaborn Plot (seaborn.objects interface).
 
         Args:
             obj: The plot object.
-            format: The image format.
+            format: Image format.
             class_: The container class attribute.
-            **kwargs: Keyword arguments passed to a function
-                which converts object to an image.
+            **kwargs: Keyword arguments passed to the function
+                which converts the object to an image.
 
         Raises:
-            TypeError: Plot type is not supported
-                or required extra package is not installed.
+            TypeError: The plot type is not supported
+                or a required extra package is not installed.
         """
         if format is None:
             format = rico._config.get_config("image_format")  # noqa: A001
 
         if plt is not None and isinstance(obj, plt.Axes):
             obj = obj.figure
 
@@ -324,38 +287,39 @@
             image = convert(  # type: ignore
                 obj.to_json(),  # type: ignore
                 vl_version="_".join(alt.SCHEMA_VERSION.split(".")[:2]),
                 **kwargs,
             )
         else:
             error_msg = (
-                f"Plot type {type(obj)} is not supported "
-                "or required extra package is not installed."
+                f"The plot type {type(obj)} is not supported "
+                "or a required extra package is not installed."
             )
             raise TypeError(error_msg)
 
         mime_subtype = "svg+xml" if format == "svg" else format
         content = Image(data=image, mime_subtype=mime_subtype, class_=class_)  # type: ignore  # noqa: E501
         self.container = content.container
 
 Chart = Plot
 
 
 class Obj(ContentBase):
-    """An arbitrary content definition.
-
-    Creates content elements from arbitrary objects and appends them to the container.
-
-    Automatically determines the content type.
-    """
     def __init__(self, *objects: Any, class_: str | None = None):
-        """Create content from arbitrary objects.
+        """Create HTML elements from objects and wrap them in a <div> container.
+
+        Automatically determines the content type in the following order:
+        1. `rico` content classes (subclasses of `ContentBase`).
+        2. Plots.
+        3. Dataframes and other types with `_repr_html_` method.
+        4. Text.
+        All other types are converted to text.
 
         Args:
-            *objects: The objects which are used to create a content.
+            *objects: The objects.
             class_: The container class attribute.
         """
         super().__init__(class_=class_)
         for obj in objects:
             if isinstance(obj, ContentBase):
                 elements = (obj.container,)
             elif (
@@ -373,44 +337,37 @@
                 elements = Text(obj).container
 
             for element in elements:
                 self.container.append(element)
 
 
 class Script(ContentBase):
-    """A script definition.
-
-    Attributes:
-        script (Element): The script element.
-        footer (bool): Defines whether the script should be placed at a document footer,
-            aftert all other content.
-    """
-    container: ET.Element
     footer: bool = False
 
     def __init__(
         self,
         text: str | None = None,
         src: str | None = None,
         inline: bool | None = None,
         defer: bool = False,
         attrib: dict[str, Any] = {},
         **extra: Any,
     ):
-        """Create script.
+        """Create an HTML script element.
 
         Either `text` or `src` should be used.
 
         Args:
             text: The script text.
             src: The script source link.
             inline: If True, load script inline, downdload it from source link
-                and use it as a text.
-            defer: The script "defer" attribute. For inline script defines whether
-                it should be placed at a document footer, aftert all other content.
+                and use it as `text`.
+            defer: The "defer" attribute of the script. For an inline script, defines
+                whether it should be placed in the footer of the document aftert all
+                other content.
             attrib: The script attributes.
             **extra: Extra attributes.
 
         Raises:
             ValueError: Both text and src are not None.
             ValueError: Both text and src are None.
         """
@@ -436,38 +393,31 @@
             self.footer = defer
 
         self.container = ET.Element("script", {**attrib, **extra})
         self.container.text = text
 
 
 class Style(ContentBase):
-    """A stylesheet definition.
-
-    Attributes:
-        style (Element): The style element.
-    """
-    container: ET.Element
-
     def __init__(
         self,
         text: str | None = None,
         src: str | None = None,
         inline: bool | None = None,
         attrib: dict[str, Any] = {},
         **extra: Any,
     ):
-        """Create stylesheet.
+        """Create an HTML style element.
 
         Either `text` or `src` should be used.
 
         Args:
             text: The stylesheet text.
             src: The stylesheet source link.
             inline: If True, load stylesheet inline, downdload it from source link
-                and use it as a text.
+                and use it as `text`.
             attrib: The stylesheet attributes.
             **extra: Extra attributes.
 
         Raises:
             ValueError: Both text and src are not None.
             ValueError: Both text and src are None.
         """
```

### Comparing `rico-0.3.0/src/rico/_html.py` & `rico-0.3.1/src/rico/_html.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """HTML parser and serializer."""
 
 from __future__ import annotations
 
 import html.parser
+import textwrap
 import xml.etree.ElementTree as ET
 
 import rico._config
 
 
 TAGS_EMPTY = {
     "area", "base", "basefont", "br", "col", "embed", "frame", "hr", "img",
@@ -19,149 +20,165 @@
     "strong", "sub", "sup", "time", "u", "var", "wbr",
 }
 
 TAGS_NOT_ESCAPED = {"script", "style"}
 TAGS_PREFORMATTED = {"pre"}
 
 
-class HTMLParser(html.parser.HTMLParser):
-    """Simple HTML parser. Returns a list of instances of ET.Element on close().
-
-    Assigns None values to boolean attributes.
-
-    Ignores comments, doctype declaration and processing instructions.
-    Converts attribute names to lower case, even for SVG.
-    """
-
+class _HTMLParser(html.parser.HTMLParser):
     def __init__(self):
         super().__init__()
         self._root = "root"
         self._builder = ET.TreeBuilder()
         self._builder.start(self._root, {})
+        self._empty_tag = None
 
     def handle_starttag(
         self,
         tag: str,
         attrs: list[tuple[str, str | None]],
     ) -> None:
+        if self._empty_tag:
+            self._builder.end(self._empty_tag)
+        self._empty_tag = tag if tag.lower() in TAGS_EMPTY else None
         self._builder.start(tag, dict(attrs))
 
     def handle_endtag(self, tag: str) -> None:
+        if self._empty_tag:
+            if self._empty_tag.lower() != tag.lower():
+                self._builder.end(self._empty_tag)
+            self._empty_tag = None
         self._builder.end(tag)
 
     def handle_data(self, data: str) -> None:
+        if self._empty_tag:
+            self._builder.end(self._empty_tag)
+            self._empty_tag = None
         self._builder.data(data)
 
     def close(self) -> tuple[ET.Element]:  # type: ignore
         super().close()
         self._builder.end(self._root)
         return tuple(self._builder.close())
 
 
 def parse_html(data: str) -> tuple[ET.Element]:
-    """Parse an HTML document from a string.
+    """Parse HTML from a string.
 
-    Assign None values to boolean attributes.
+    Assigns None values to boolean attributes.
 
-    Ignore comments, doctype declaration and processing instructions.
-    Convert attribute names to lower case, even for SVG.
+    Ignores comments, doctype declaration and processing instructions.
+    Converts attribute names to lower case, even for SVG.
 
     Args:
-        data: The HTML data.
+        data: The string containing HTML data.
 
     Returns:
-        The parsed HTML document.
+        HTML elements parsed from the string.
     """
-    parser = HTMLParser()
+    parser = _HTMLParser()
     parser.feed(data)
     return parser.close()
 
 
 def indent_html(
     element: ET.Element,
     space: str = "  ",
     level: int = 0,
 ) -> ET.Element:
-    """Indent an HTML element.
+    """Indent an HTML element and its chidren.
 
-    Tnsert newlines and indentation space after elements.
-    Create a new element instead of updating inplace.
-    Do not indent elements inside <pre> tag.
+    Tnserts newlines and indentation space after elements.
+    Creates a new element instead of updating in place.
+    Doesn't indent elements inside the <pre> tag or inside inline tags.
 
     Args:
         element: The element to indent.
-        space: The whitespace to insert for each indentation level.
+        space: Whitespace to insert for each indentation level.
         level: The initial indentation level. Should always be 0.
 
     Returns:
-        The indented HTML element.
+        Indented HTML element.
     """
-    if element.tag.lower() in TAGS_PREFORMATTED or not len(element):
-        return element
-
     indented_element = ET.Element(element.tag, attrib=element.attrib)
     indented_element.text = element.text
     indented_element.tail = element.tail
 
-    if not element.text or not element.text.strip():
-        indented_element.text = "\n" + space * (level + 1)
-
-    for child in element:
-        indented_child = indent_html(child, space=space, level=level + 1)
-
-        if not indented_child.tail or not indented_child.tail.strip():
-            indented_child.tail = "\n" + space * (level + 1)
-
-        indented_element.append(indented_child)
+    if element.tag.lower() in TAGS_PREFORMATTED | TAGS_INLINE:
+        for child in element:
+            indented_element.append(child)
+    else:
+        has_children = len(element) > 0
+        left_stripped_text = (
+            indented_element.text.lstrip()
+            if indented_element.text else
+            indented_element.text
+        )
+        if (
+            not has_children and
+            indented_element.text is not None and
+            left_stripped_text
+        ):
+            if "\n" in left_stripped_text:
+                indented_element.text = "\n" + textwrap.indent(
+                    textwrap.dedent(indented_element.text).strip(),
+                    space * (level + 1),
+                ) + "\n" + space * level
+            else:
+                indented_element.text = left_stripped_text
+        elif not left_stripped_text:
+            indented_element.text = "\n" + space * (level + 1) if has_children else None
 
-    if not indented_child.tail or not indented_child.tail.strip():  # type: ignore
-        indented_child.tail = "\n" + space * level  # type: ignore
+        for child in element:
+            indented_child = indent_html(child, space=space, level=level + 1)
+            indented_element.append(indented_child)
+            if not indented_child.tail or not indented_child.tail.strip():
+                indented_child.tail = "\n" + space * (level + 1)
+
+        if has_children:
+            last_child = indented_element[-1]
+            if not last_child.tail or not last_child.tail.strip():
+                last_child.tail = "\n" + space * level
 
     return indented_element
 
 
 def strip_html(element: ET.Element) -> ET.Element:
-    """Strip an HTML element.
+    """Remove unnecessary whitespace from an HTML element and its children.
 
-    Remove unnecessary whitespaces from the element by strippping elements'
-    text and tail.
-    Do not strip elements inside <pre> tag or inside inline tags.
+    Removes leading whitespace from elements' text.
+    Doesn't strip elements inside the <pre> tag or inside inline tags.
 
     Args:
         element: The element to strip.
 
     Returns:
-        The stripped HTML element.
+        An HTML element with stripped leading and trailing whitespace.
     """
     stripped_element = ET.Element(element.tag, attrib=element.attrib)
     stripped_element.text = element.text
     stripped_element.tail = element.tail
 
     if element.tag.lower() in TAGS_INLINE | TAGS_PREFORMATTED:
         for child in element:
             stripped_element.append(child)
     else:
+        stripped_element.text = (
+            stripped_element.text.lstrip()
+            if stripped_element.text else
+            stripped_element.text
+        )
+
+        has_children = len(element) > 0
+        if stripped_element.text and not has_children:
+            stripped_element.text = stripped_element.text.rstrip()
+
         for child in element:
             stripped_element.append(strip_html(child))
 
-        if stripped_element.text:
-            if len(stripped_element) == 0 and (
-                not stripped_element.tail or
-                not stripped_element.tail.strip()
-            ):
-                stripped_element.text = stripped_element.text.strip()
-            else:
-                stripped_element.text = stripped_element.text.lstrip()
-
-    if stripped_element.tail:
-        if len(stripped_element) == 0 and not stripped_element.text:
-            stripped_element.tail = stripped_element.tail.strip()
-        else:
-            stripped_element.tail = stripped_element.tail.rstrip()
-
     return stripped_element
 
 
 def _escape_cdata(text: str) -> str:
     """Copy of xml.etree.ElementTree._escape_cdata."""
     if "&" in text:
         text = text.replace("&", "&amp;")
@@ -183,26 +200,26 @@
 
 def serialize_html(
     element: ET.Element,
     indent: bool | None = None,
     space: str | None = None,
     strip: bool | None = None,
 ) -> str:
-    """Serialize an HTML element to a string.
+    """Serialize an HTML element and its children to a string.
 
-    Serialize attributes with None values as boolean.
+    Serializes attributes with None values as boolean.
 
     Args:
         element: The HTML element.
         indent: If True, indent the element.
-        space: The whitespace for indentation.
+        space: Whitespace for indentation.
         strip: If True, strip unnecessary whitespace.
 
     Returns:
-        The serialized HTML element.
+        A string with serialized HTML.
     """
     global_config = rico._config.get_config()
     if indent is None:
         indent = global_config["indent_html"]
     if space is None:
         space = global_config["indent_space"]
     if strip is None:
@@ -218,16 +235,17 @@
         if v is not None and not isinstance(v, bool)  # type: ignore
         # Serialize attributes with None values as boolean.
         else f" {k}"
         for k, v in element.items()
         if not isinstance(v, bool) or v
     )
 
-    opening_tag = f"<{element.tag}{attrib}>"
     ltag = element.tag.lower()
+    closing_slash = "/" if ltag in TAGS_EMPTY else ""
+    opening_tag = f"<{element.tag}{attrib}{closing_slash}>"
 
     if element.text is not None:
         text = element.text if ltag in TAGS_NOT_ESCAPED else _escape_cdata(element.text)
     else:
         text = ""
 
     children = "".join(serialize_html(e) for e in element)
```

### Comparing `rico-0.3.0/tests/test__config.py` & `rico-0.3.1/tests/test__config.py`

 * *Files identical despite different names*

### Comparing `rico-0.3.0/tests/test__container.py` & `rico-0.3.1/tests/test__container.py`

 * *Files 1% similar despite different names*

```diff
@@ -340,11 +340,11 @@
 
 
 def test_doc_serialize():
     with rico._config.config_context(dataframe_style=""):
         doc = rico._container.Doc("Hello world", bootstrap="none")
 
     assert doc.serialize() == (
-        '<!doctype html>\n<html><head><meta charset="utf-8">'
-        '<meta name="viewport" content="width=device-width, initial-scale=1"></head>'
+        '<!doctype html>\n<html><head><meta charset="utf-8"/>'
+        '<meta name="viewport" content="width=device-width, initial-scale=1"/></head>'
         '<body><div class="container"><div><p>Hello world</p></div></div></body></html>'
     )
```

### Comparing `rico-0.3.0/tests/test__content.py` & `rico-0.3.1/tests/test__content.py`

 * *Files 1% similar despite different names*

```diff
@@ -420,21 +420,21 @@
 
 
 def test_obj():
     class ReprHTML:
         def _repr_html_(self) -> str:
             return "<h1>Hello</h1>"
 
-    content_base = rico._content.ContentBase(class_="col")
+    text = rico._content.Text("Hi")
 
     content = rico._content.Obj(
         ReprHTML(),
         "world",
         pyplot_axes,
-        content_base,
+        text,
         class_="row",
     )
 
     div0 = content.container
     assert isinstance(div0, ET.Element)
     assert div0.tag == "div"
     assert div0.attrib == {"class": "row"}
@@ -446,33 +446,41 @@
     assert isinstance(h1, ET.Element)
     assert h1.tag == "h1"
     assert h1.attrib == {}
     assert h1.text == "Hello"
     assert h1.tail is None
     assert len(h1) == 0
 
-    p = tuple(div0)[1]
-    assert isinstance(p, ET.Element)
-    assert p.tag == "p"
-    assert p.attrib == {}
-    assert p.text == "world"
-    assert p.tail is None
-    assert len(p) == 0
+    p0 = tuple(div0)[1]
+    assert isinstance(p0, ET.Element)
+    assert p0.tag == "p"
+    assert p0.attrib == {}
+    assert p0.text == "world"
+    assert p0.tail is None
+    assert len(p0) == 0
 
     img = tuple(div0)[2]
     assert isinstance(img, ET.Element)
     assert img.tag == "img"
 
     div1 = tuple(div0)[3]
     assert isinstance(div1, ET.Element)
     assert div1.tag == "div"
-    assert div1.attrib == {"class": "col"}
+    assert div1.attrib == {}
     assert div1.text is None
     assert div1.tail is None
-    assert len(div1) == 0
+    assert len(div1) == 1
+
+    p1 = tuple(div1)[0]
+    assert isinstance(p1, ET.Element)
+    assert p1.tag == "p"
+    assert p1.attrib == {}
+    assert p1.text == "Hi"
+    assert p1.tail is None
+    assert len(p1) == 0
 
 
 @pytest.mark.parametrize("defer", [True, False], ids=["defer", "not defer"])
 def test_script_text(defer: bool):
     text = "alert('Hello World!');"
     attrib = {"async": True}
     content = rico._content.Script(text=text, defer=defer, attrib=attrib)
```

### Comparing `rico-0.3.0/tests/test__html.py` & `rico-0.3.1/tests/test__html.py`

 * *Files 15% similar despite different names*

```diff
@@ -128,18 +128,64 @@
         "d": "M4 8a.5.5 0 0 1 .5-.5h7a.5.5 0 0 1 0 1h-7A.5.5 0 0 1 4 8z",
     }
     assert path.text is None
     assert path.tail is None
     assert len(path) == 0
 
 
+def test_parse_html_empty_tag():
+    text = "<p>Hello<br><br>world<br></p>"
+    elements = rico._html.parse_html(text)
+
+    assert elem_to_string(elements) == text
+    assert isinstance(elements, tuple)
+    assert len(elements) == 1
+
+    p = elements[0]
+    assert isinstance(p, ET.Element)
+    assert p.tag == "p"
+    assert p.attrib == {}
+    assert p.text == "Hello"
+    assert p.tail is None
+    assert len(p) == 3
+
+    br0 = p[0]
+    assert isinstance(br0, ET.Element)
+    assert br0.tag == "br"
+    assert br0.attrib == {}
+    assert br0.text is None
+    assert br0.tail is None
+    assert len(br0) == 0
+
+    br1 = p[1]
+    assert isinstance(br1, ET.Element)
+    assert br1.tag == "br"
+    assert br1.attrib == {}
+    assert br1.text is None
+    assert br1.tail == "world"
+    assert len(br1) == 0
+
+    br2 = p[2]
+    assert isinstance(br2, ET.Element)
+    assert br2.tag == "br"
+    assert br2.attrib == {}
+    assert br2.text is None
+    assert br2.tail is None
+    assert len(br2) == 0
+
+
 @pytest.fixture
 def sample_elem():
     div0 = ET.Element("div", {"class": "container"})
     div0.text = "\n"
+    style = ET.SubElement(div0, "style")
+    style.text = textwrap.dedent("""\
+        strong {color: red;}
+        code {color: blue;}
+    """)
     p0 = ET.SubElement(div0, "p")
     p0.text = " Hello "
     p0.tail = "\n"
     strong = ET.SubElement(p0, "strong")
     strong.text = " world "
     strong.tail = " ! "
     div1 = ET.SubElement(div0, "div", {"class": '>&"'})
@@ -161,14 +207,18 @@
     br.tail = " world again "
     return div0
 
 
 def test_indent_html_default(sample_elem: ET.Element):
     expectation = textwrap.dedent("""\
         <div class="container">
+          <style>
+            strong {color: red;}
+            code {color: blue;}
+          </style>
           <p> Hello <strong> world </strong> ! </p>
           <div class="&gt;&amp;&quot;">
             <code> should be indented </code>
           </div>
           <pre>
         <code> should not be indented </code>
         </pre>
@@ -177,14 +227,18 @@
 
     assert elem_to_string(rico._html.indent_html(sample_elem)) == expectation
 
 
 def test_indent_html_custom_space(sample_elem: ET.Element):
     expectation = textwrap.dedent("""\
         <div class="container">
+            <style>
+                strong {color: red;}
+                code {color: blue;}
+            </style>
             <p> Hello <strong> world </strong> ! </p>
             <div class="&gt;&amp;&quot;">
                 <code> should be indented </code>
             </div>
             <pre>
         <code> should not be indented </code>
         </pre>
@@ -196,98 +250,115 @@
 
 
 def test_strip_html(sample_elem: ET.Element):
     p = ET.Element("p")
     p.text = " Hello world again again "
     sample_elem.append(p)
 
-    expectation = (
-        '<div class="container"><p>Hello <strong> world </strong> !</p>'
-        '<div class="&gt;&amp;&quot;"><code> should be indented </code></div><pre>\n'
-        "<code> should not be indented </code>\n"
-        "</pre><p>Hello &gt;&amp;&lt; <br>world again</p>"
-        "<p>Hello world again again</p></div>"
-    )
+    expectation = textwrap.dedent("""\
+        <div class="container"><style>strong {color: red;}
+        code {color: blue;}</style><p>Hello <strong> world </strong> ! </p>
+        <div class="&gt;&amp;&quot;"><code> should be indented </code>
+        </div>
+        <pre>
+        <code> should not be indented </code>
+        </pre>
+        <p>Hello &gt;&amp;&lt; <br> world again </p>
+        <p>Hello world again again</p></div>""")
 
     assert elem_to_string(rico._html.strip_html(sample_elem)) == expectation
 
 
 def test_serialize_html_default(sample_elem: ET.Element):
     expectation = textwrap.dedent("""\
         <div class="container">
-        <p> Hello <strong> world </strong> ! </p>
+        <style>strong {color: red;}
+        code {color: blue;}
+        </style><p> Hello <strong> world </strong> ! </p>
         <div class="&gt;&amp;&quot;">
         <code> should be indented </code>
         </div>
         <pre>
         <code> should not be indented </code>
         </pre>
-        <p> Hello &gt;&amp;&lt; <br> world again </p>
+        <p> Hello &gt;&amp;&lt; <br/> world again </p>
         </div>""")
 
     assert rico._html.serialize_html(sample_elem) == expectation
 
 
 def test_serialize_html_indent(sample_elem: ET.Element):
     expectation = textwrap.dedent("""\
         <div class="container">
+            <style>
+                strong {color: red;}
+                code {color: blue;}
+            </style>
             <p> Hello <strong> world </strong> ! </p>
             <div class="&gt;&amp;&quot;">
                 <code> should be indented </code>
             </div>
             <pre>
         <code> should not be indented </code>
         </pre>
-            <p> Hello &gt;&amp;&lt; <br> world again </p>
+            <p> Hello &gt;&amp;&lt; <br/> world again </p>
         </div>""")
 
     assert rico._html.serialize_html(
         sample_elem, indent=True, space="    ") == expectation
 
 
 def test_serialize_html_strip(sample_elem: ET.Element):
-    expectation = (
-        '<div class="container"><p>Hello <strong> world </strong> !</p>'
-        '<div class="&gt;&amp;&quot;"><code> should be indented </code></div><pre>\n'
-        "<code> should not be indented </code>\n"
-        "</pre><p>Hello &gt;&amp;&lt; <br>world again</p></div>"
-    )
+    expectation = textwrap.dedent("""\
+        <div class="container"><style>strong {color: red;}
+        code {color: blue;}</style><p>Hello <strong> world </strong> ! </p>
+        <div class="&gt;&amp;&quot;"><code> should be indented </code>
+        </div>
+        <pre>
+        <code> should not be indented </code>
+        </pre>
+        <p>Hello &gt;&amp;&lt; <br/> world again </p>
+        </div>""")
 
     assert rico._html.serialize_html(sample_elem, strip=True) == expectation
 
 
 def test_serialize_html_bool_attr(sample_elem: ET.Element):
     sample_elem.set("autofocus", None)  # type: ignore
     expectation = textwrap.dedent("""\
         <div class="container" autofocus>
-        <p> Hello <strong> world </strong> ! </p>
+        <style>strong {color: red;}
+        code {color: blue;}
+        </style><p> Hello <strong> world </strong> ! </p>
         <div class="&gt;&amp;&quot;">
         <code> should be indented </code>
         </div>
         <pre>
         <code> should not be indented </code>
         </pre>
-        <p> Hello &gt;&amp;&lt; <br> world again </p>
+        <p> Hello &gt;&amp;&lt; <br/> world again </p>
         </div>""")
 
     assert rico._html.serialize_html(sample_elem) == expectation
     sample_elem.set("autofocus", True)  # type: ignore
     assert rico._html.serialize_html(sample_elem) == expectation
 
     sample_elem.set("autofocus", False)  # type: ignore
     expectation = textwrap.dedent("""\
         <div class="container">
-        <p> Hello <strong> world </strong> ! </p>
+        <style>strong {color: red;}
+        code {color: blue;}
+        </style><p> Hello <strong> world </strong> ! </p>
         <div class="&gt;&amp;&quot;">
         <code> should be indented </code>
         </div>
         <pre>
         <code> should not be indented </code>
         </pre>
-        <p> Hello &gt;&amp;&lt; <br> world again </p>
+        <p> Hello &gt;&amp;&lt; <br/> world again </p>
         </div>""")
     assert rico._html.serialize_html(sample_elem) == expectation
 
 
 def test_serialize_html_style():
     elem = ET.Element("style")
     elem.text = ".>&< {border: none;}"
```

### Comparing `rico-0.3.0/tests/test__version.py` & `rico-0.3.1/tests/test__version.py`

 * *Files identical despite different names*

### Comparing `rico-0.3.0/PKG-INFO` & `rico-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rico
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Python package for creating HTML documents from rich content: dataframes, plots, images, markdown etc. It provides a high-level, easy-to-use API with reasonable defaults, as well as low-level access for better control.
 Author-Email: Evgeny Ivanov <ivanov.evgeny.n@gmail.com>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -34,14 +34,25 @@
 Requires-Dist: rico[altair,markdown,pyplot,seaborn]; extra == "complete"
 Description-Content-Type: text/markdown
 
 # rico: rich content to HTML as easy as Doc(df, plot)
 
 **rico** is a Python package for creating HTML documents from rich content: dataframes, plots, images, markdown etc. It provides a high-level, easy-to-use API with reasonable defaults, as well as low-level access for better control.
 
+Use **rico** if you want to create an HTML document from objects created in a Python script.
+
+With **rico** you can *avoid*:
+* Writing data to intermediate files or a database from a script.
+* Loading data into a Jupyter notebook from intermediate files or a database.
+* Using nbconvert or similar tools for creating HTML files.
+
+More on the topic:
+* [Pass pandas dataframe to notebook via nbconvert](https://github.com/jupyter/nbconvert/issues/1070).
+* [Could Papermill pass an in-memory dataframe to a notebook?](https://github.com/nteract/papermill/issues/406)
+
 [![CI](https://github.com/e10v/rico/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/e10v/rico/actions/workflows/ci.yml)
 [![Coverage](https://codecov.io/github/e10v/rico/coverage.svg?branch=main)](https://codecov.io/gh/e10v/rico)
 [![License](https://img.shields.io/github/license/e10v/rico)](https://github.com/e10v/rico/blob/main/LICENSE)
 [![Version](https://img.shields.io/pypi/v/rico.svg)](https://pypi.org/project/rico/)
 [![Package Status](https://img.shields.io/pypi/status/rico.svg)](https://pypi.org/project/rico/)
 [![PyPI Python Versions](https://img.shields.io/pypi/pyversions/rico.svg)](https://pypi.org/project/rico/)
 
@@ -74,15 +85,15 @@
 ```
 
 [Seaborn](https://seaborn.pydata.org/):
 ```bash
 pip install rico[seaborn]
 ```
 
-Install `rico[seaborn]` extra only to use the [seaborn.objects](https://seaborn.pydata.org/tutorial/objects_interface.html) interface. Otherwise install `rico[pyplot]` as the old plotting functions return Matplotlib Pyplot Axes objects.
+Install `rico[seaborn]` extra only to use the [seaborn.objects](https://seaborn.pydata.org/tutorial/objects_interface.html) interface. Otherwise install `rico[pyplot]` as the old Seaborn plotting functions return Matplotlib Pyplot Axes objects.
 
 All extras:
 ```bash
 pip install rico[complete]
 ```
 
 ## User guide
@@ -135,27 +146,27 @@
 
 Implicit serialization:
 ```python
 with open("doc.html", "w") as f:
     print(doc, file=f)
 ```
 
-Internally, `str(doc)` calls `doc.serialize()` with default parameter values. Call `doc.serialize()` to indent the HTML element tree visually:
+Internally, `str(doc)` calls `doc.serialize()` with default parameter values. Call `doc.serialize(indent=True)` to indent the HTML element tree visually:
 ```python
 with open("doc.html", "w") as f:
     f.write(doc.serialize(indent=True))
 ```
 
 Set custom whitespace for indentation using the `space` parameter:
 ```python
 with open("doc.html", "w") as f:
     f.write(doc.serialize(indent=True, space="    "))
 ```
 
-Remove unnecessary whitespace between tags by setting `strip` to `True`:
+Remove unnecessary whitespace by setting `strip` to `True`:
 ```python
 with open("doc.html", "w") as f:
     f.write(doc.serialize(strip=True))
 ```
 
 Control the default behavior of `str(doc)` and `doc.serialize()` using the global options `indent_html`, `indent_space`, and `strip_html`:
 ```python
@@ -182,15 +193,15 @@
     rico.Text("Hello world!", mono=True),  # The default value is False.
     df,
     rico.Plot(plot, format="png"),  # The default value is "svg".
     title="My doc",
 )
 ```
 
-Or:
+The following code gives the same result as the code above:
 ```python
 doc = rico.Doc(title="My doc")
 doc.append_text("Hello world!", mono=True)
 doc.append(df)
 doc.append_plot(plot, format="png")
 ```
 
@@ -203,41 +214,41 @@
 Use specific classes and methods for other content types:
 * Images: `Image` or `Doc.append_image`.
 * Code: `Code` or `Doc.append_code`.
 * Markdown: `Markdown` or `Doc.append_markdown`.
 * HTML tag: `Tag` or `Doc.append_tag`.
 * Raw HTML: `HTML` or `Doc.append_html`.
 
-Example:
+For example:
 ```python
 doc = rico.Doc(
     rico.Markdown("## Dataframe"),
     df,
     rico.Tag("h2", "Plot"),  # An alternative way to add a header.
     plot,
     rico.HTML("<h2>Code</h2>"),  # Another way to add a header.
     rico.Code("print('Hello world!')"),
     title="My doc",
 )
 ```
 
-Or:
+The following code gives the same result as the code above:
 ```python
 doc = rico.Doc(title="My doc")
 doc.append_markdown("## Dataframe")
 doc.append(df)
 doc.append_tag("h2", "Plot")
 doc.append(plot)
 doc.append_html("<h2>Code</h2>")
 doc.append_code("print('Hello world!')")
 ```
 
-Check the docstrings for additional parameters.
+Check the docstrings for details.
 
-Serialize content to HTML using `str()` or `object.serialize()`:
+Serialize content to HTML using `str(object)` or `object.serialize()`:
 ```python
 obj = rico.Tag("p", "Hello world!")
 
 print(obj)
 # <div><p>Hello world!</p></div>
 
 print(obj.serialize(indent=True, space="    "))
@@ -249,18 +260,17 @@
 ### Bootstrap, HTML classes and document layout
 
 By default, [Bootstrap](https://getbootstrap.com/) styles are included in the document. Change the default behavior using the `bootstrap` parameter:
 ```python
 doc = rico.Doc("Hello world!", bootstrap="full")
 ```
 
-The possible values are:
-* `"css"` (default) -- include only CSS.
-* `"full"` -- include both the CSS and JS.
-* `"none"` -- don't include Bootstrap*.
+* Set `bootstrap` to `"css"` (default) to include only CSS.
+* Set `bootstrap` to `"full"` to include both the CSS and JS.
+* Set `bootstrap` to `"none"` to not include Bootstrap*.
 
 *Keep in mind that **rico** relies on Bootstrap classes and styles. For example:
 * The `mono` and `wrap` parameters of the `Text` class use Bootstrap's `font-monospace` and `font-monospace` classes.
 * **rico**'s dataframe style definition uses Bootstrap variables.
 
 Each content element is wrapped in a `<div>` container. Specify the element's container class using the `class_` parameter:
 ```python
@@ -296,15 +306,15 @@
         rico.Obj("Plot", plot, class_="col"),
         class_="row row-cols-auto",
     ),
     title="My doc",
 )
 ```
 
-Or:
+The following code gives the same result as the code above:
 ```python
 doc = rico.Doc(title="My doc")
 doc.append_tag("h1", "My doc")
 doc.append_tag("h2", "Description")
 doc.append("This is an example of custom document layout using Bootstrap classes.")
 doc.append_tag("h2", "Data")
 div = rico.Div(class_="row row-cols-auto")
@@ -338,86 +348,97 @@
 ```python
 with rico.config_context(dataframe_style=""):
     doc = rico.Doc(df)
 ```
 
 Include custom styles and scripts using the `Style` and `Script` classes:
 ```python
-css = "https://cdn.jsdelivr.net/npm/bootstrap-icons@1/font/bootstrap-icons.css"
-js = "https://cdn.jsdelivr.net/npm/jquery@3.7.0/dist/jquery.min.js"
+dark_theme = "https://cdn.jsdelivr.net/npm/bootswatch@5/dist/darkly/bootstrap.min.css"
+jquery = "https://cdn.jsdelivr.net/npm/jquery@3/dist/jquery.min.js"
 
 doc = rico.Doc(
-    "Hello world",
+    rico.Text("Click me", class_="click"),
     extra_styles=(
-        rico.Style("p {color: red;}"),
-        rico.Style(src=css),
+        rico.Style(src=dark_theme),
+        rico.Style(".click {color: red;}"),
     ),
     extra_scripts=(
-        rico.Script("alert('Hello World!');"),
-        rico.Script(src=js),
+        rico.Script(src=jquery),
+        rico.Script(
+            "$('p').on('click', function() {alert('Hello world!');})",
+            defer=True,
+        ),
     ),
 )
 ```
 
+The `defer` parameter adds the `defer` attribute to the `<script>` tag if the `src` parameter is used. Otherwise, if the `text` parameter is used, the script is placed in the footer of the document.
+
 By default, external styles and scripts are included as file links. This means that these files must be available when someone opens the document. Include the contents of these files in the document using the `inline` parameter:
 ```python
 doc = rico.Doc(
-    "Hello world",
+    rico.Text("Click me", class_="click"),
     extra_styles=(
-        rico.Style("p {color: red;}"),
-        rico.Style(src=css, inline=True),
+        rico.Style(src=dark_theme, inline=True),
+        rico.Style(".click {color: red;}"),
     ),
     extra_scripts=(
-        rico.Script("alert('Hello World!');"),
-        rico.Script(src=js, inline=True),
+        rico.Script(src=jquery, inline=True),
+        rico.Script(
+            "$('p').on('click', function() {alert('Hello world!');})",
+            defer=True,
+        ),
     ),
 )
 ```
 
 In the example above, the Bootstrap styles are still included as a link. Use the global options `inline_styles` and `inline_scripts` to include the contents of the style and script files in the document:
 ```python
 with rico.config_context(inline_styles=True, inline_scripts=True):
     doc = rico.Doc(
-        "Hello world",
+        rico.Text("Click me", class_="click"),
         extra_styles=(
-            rico.Style("p {color: red;}"),
-            rico.Style(src=css),
+            rico.Style(src=dark_theme),
+            rico.Style(".click {color: red;}"),
         ),
         extra_scripts=(
-            rico.Script("alert('Hello World!');"),
-            rico.Script(src=js),
+            rico.Script(src=jquery),
+            rico.Script(
+                "$('p').on('click', function() {alert('Hello world!');})",
+                defer=True,
+            ),
         ),
     )
 ```
 
 ### Global configuration
 
 Use global configuration to:
 * Get or set default parameter values.
 * Get or set document properties.
 
-The following globals options define the default parameter values:
+The following global options define the default parameter values:
 
 | Global option    | Parameter | Classes, methods, functions       |
 |:-----------------|:----------|:----------------------------------|
 | `indent_html`    | `indent`  | `obj.serialize`, `serialize_html` |
 | `indent_space`   | `space`   | `obj.serialize`, `serialize_html` |
 | `strip_html`     | `strip`   | `obj.serialize`, `serialize_html` |
 | `text_mono`      | `mono`    | `Text`, `obj.append_text`         |
 | `text_wrap`      | `wrap`    | `Text`, `obj.append_text`         |
 | `image_format`   | `format`  | `Plot`, `obj.append_plot`         |
 | `inline_styles`  | `inline`  | `Style`                           |
 | `inline_scripts` | `inline`  | `Script`                          |
 
-The following globals options define document properties:
-* `meta_charset` defines a document [charset](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/meta#charset) metadata.
-* `meta_viewport` defines a document [viewport](https://developer.mozilla.org/en-US/docs/Web/HTML/Viewport_meta_tag) metadata.
+The following global options define document properties:
+* `meta_charset` defines a document [charset](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/meta#charset) metadata. Set it to `""` to disable.
+* `meta_viewport` defines a document [viewport](https://developer.mozilla.org/en-US/docs/Web/HTML/Viewport_meta_tag) metadata. Set it to `""` to disable.
 * `bootstrap_css` defines a link to the Bootstrap CSS file.
 * `bootstrap_js` defines a link to the Bootstrap JS file.
-* `dataframe_style` defines a dataframe style.
+* `dataframe_style` defines a dataframe style. Set it to `""` to disable.
 
 Get a dictionary with global options using `get_config` without parameters:
 ```python
 global_config = rico.get_config()
 print(global_config["indent_html"])
 # False
 ```
@@ -450,36 +471,33 @@
 
 Internally, **rico** uses the standard [xml.etree.ElementTree](https://docs.python.org/3/library/xml.etree.elementtree.html) module:
 * Every content object (`Tag`, `Text`, `Div` etc.) has a `container` attribute of type `xml.etree.ElementTree.Element`. The value is a `<div>` container element.
 * `Doc` objects has additional attributes `html`, `head`, and `body` of type `xml.etree.ElementTree.Element`. They represent the `<html>`, `<head>`, and `<body>` elements, respectively.
 
 Access these attributes and use `xml.etree.ElementTree` API to gain low-level control over the document and its elements.
 
-## Use case and alternatives
+Also, **rico** provides the following functions for working with `xml.etree.ElementTree.Element` objects:
+* `parse_html` parses HTML from a string.
+* `indent_html` indents an HTML element tree visually.
+* `strip_html` removes unnecessary whitespace.
+* `serialize_html` serializes `xml.etree.ElementTree.Element` object.
 
-Use **rico** if you want to create an HTML document from objects created in a Python script.
+Check the docstrings for details.
 
-With **rico** you can avoid:
-* Writing data to intermediate files or a database from a script.
-* Loading data into a Jupyter notebook.
-* Using [nbconvert](https://nbconvert.readthedocs.io/) or similar tools.
+## Alternatives
 
-Alternatives:
 * Use [Jupyter Notebook](https://jupyter.org/) for interactive computing.
 * Use [nbconvert](https://nbconvert.readthedocs.io/) or [papermill](https://papermill.readthedocs.io/) if you're processing data and creating objects for a document in a Jupyter notebook.
 * Use [Quarto](https://quarto.org/) if you prefer R Markdown style notebooks and a variety of output formats.
 * Use [xml.etree.ElementTree](https://docs.python.org/3/library/xml.etree.elementtree.html), [lxml](https://lxml.de/), [Yattag](https://www.yattag.org/), or [Airium](https://gitlab.com/kamichal/airium) if you need low-level control.
 
 More on the topic:
-* [Pass pandas dataframe to notebook via nbconvert](https://github.com/jupyter/nbconvert/issues/1070).
-* [Could Papermill pass an in-memory dataframe to a notebook?](https://github.com/nteract/papermill/issues/406)
 * "I Don’t Like Notebooks": [video](https://www.youtube.com/watch?v=7jiPeIFXb6U), [slides](https://docs.google.com/presentation/d/1n2RlMdmv1p25Xy5thJUhkKGvjtV-dkAIsUXP-AL4ffI/edit#slide=id.g362da58057_0_1).
 * [The First Notebook War](https://yihui.org/en/2018/09/notebook-war/).
 
 ## Roadmap
 
+* Support most of IPython rich representation [methods](https://ipython.readthedocs.io/en/stable/config/integrating.html#rich-display).
 * Create docs with [MkDocs](https://www.mkdocs.org/) and [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/).
+* Create short quick start.
+* Create examples with resulting HTML files.
 * Support math with [KaTeX](https://katex.org/).
-* Save Altair Charts in [Vega-Lite](https://vega.github.io/vega-lite/) format.
-* Save SVG images in XML format.
-* Support diagrams with [Mermaid.js](https://mermaid.js.org/).
-* Support other plot types: [Plotly](https://plotly.com/python/), [Bokeh](https://bokeh.org/).
```

