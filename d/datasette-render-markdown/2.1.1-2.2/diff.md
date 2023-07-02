# Comparing `tmp/datasette-render-markdown-2.1.1.tar.gz` & `tmp/datasette-render-markdown-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasette-render-markdown-2.1.1.tar", last modified: Fri Jan 27 23:32:29 2023, max compression
+gzip compressed data, was "datasette-render-markdown-2.2.tar", last modified: Sun Jul  2 00:45:37 2023, max compression
```

## Comparing `datasette-render-markdown-2.1.1.tar` & `datasette-render-markdown-2.2.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 23:32:29.918528 datasette-render-markdown-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-01-27 23:32:14.000000 datasette-render-markdown-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7169 2023-01-27 23:32:29.918528 datasette-render-markdown-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-01-27 23:32:14.000000 datasette-render-markdown-2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 23:32:29.918528 datasette-render-markdown-2.1.1/datasette_render_markdown/
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-01-27 23:32:14.000000 datasette-render-markdown-2.1.1/datasette_render_markdown/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 23:32:29.918528 datasette-render-markdown-2.1.1/datasette_render_markdown.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7169 2023-01-27 23:32:29.000000 datasette-render-markdown-2.1.1/datasette_render_markdown.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-01-27 23:32:29.000000 datasette-render-markdown-2.1.1/datasette_render_markdown.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 23:32:29.000000 datasette-render-markdown-2.1.1/datasette_render_markdown.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-01-27 23:32:29.000000 datasette-render-markdown-2.1.1/datasette_render_markdown.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-01-27 23:32:29.000000 datasette-render-markdown-2.1.1/datasette_render_markdown.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-01-27 23:32:29.000000 datasette-render-markdown-2.1.1/datasette_render_markdown.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-27 23:32:29.918528 datasette-render-markdown-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-01-27 23:32:14.000000 datasette-render-markdown-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 00:45:37.265359 datasette-render-markdown-2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-02 00:45:17.000000 datasette-render-markdown-2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-07-02 00:45:37.265359 datasette-render-markdown-2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7690 2023-07-02 00:45:17.000000 datasette-render-markdown-2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 00:45:37.265359 datasette-render-markdown-2.2/datasette_render_markdown/
+-rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-07-02 00:45:17.000000 datasette-render-markdown-2.2/datasette_render_markdown/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 00:45:37.265359 datasette-render-markdown-2.2/datasette_render_markdown.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-07-02 00:45:37.000000 datasette-render-markdown-2.2/datasette_render_markdown.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-02 00:45:37.000000 datasette-render-markdown-2.2/datasette_render_markdown.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 00:45:37.000000 datasette-render-markdown-2.2/datasette_render_markdown.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-02 00:45:37.000000 datasette-render-markdown-2.2/datasette_render_markdown.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-02 00:45:37.000000 datasette-render-markdown-2.2/datasette_render_markdown.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-02 00:45:37.000000 datasette-render-markdown-2.2/datasette_render_markdown.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 00:45:37.265359 datasette-render-markdown-2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-02 00:45:17.000000 datasette-render-markdown-2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 00:45:37.265359 datasette-render-markdown-2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-07-02 00:45:17.000000 datasette-render-markdown-2.2/tests/test_markdown_jinja_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8970 2023-07-02 00:45:17.000000 datasette-render-markdown-2.2/tests/test_render_markdown.py
```

### Comparing `datasette-render-markdown-2.1.1/LICENSE` & `datasette-render-markdown-2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `datasette-render-markdown-2.1.1/PKG-INFO` & `datasette-render-markdown-2.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: datasette-render-markdown
-Version: 2.1.1
-Summary: Datasette plugin for rendering Markdown
-Home-page: https://github.com/simonw/datasette-render-markdown
-Author: Simon Willison
-License: Apache License, Version 2.0
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 # datasette-render-markdown
 
 [![PyPI](https://img.shields.io/pypi/v/datasette-render-markdown.svg)](https://pypi.org/project/datasette-render-markdown/)
 [![Changelog](https://img.shields.io/github/v/release/simonw/datasette-render-markdown?include_prereleases&label=changelog)](https://github.com/simonw/datasette-render-markdown/releases)
 [![Tests](https://github.com/simonw/datasette-render-markdown/workflows/Test/badge.svg)](https://github.com/simonw/datasette-render-markdown/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/datasette-render-markdown/blob/main/LICENSE)
 
@@ -117,15 +105,15 @@
 
 ## Markdown extensions
 
 The [Python-Markdown library](https://python-markdown.github.io/) that powers this plugin supports extensions, both [bundled](https://python-markdown.github.io/extensions/) and [third-party](https://github.com/Python-Markdown/markdown/wiki/Third-Party-Extensions). These can be used to enable additional Markdown features such as [table support](https://python-markdown.github.io/extensions/tables/).
 
 You can configure support for extensions using the `"extensions"` key in your plugin metadata configuration.
 
-Since extensions may introduce new HTML tags, you will also need to add those tags to the list of tags that are allowed by the [Bleach](https://bleach.readthedocs.io/) sanitizer. You can do that using the `"extra_tags"` key, and you can whitelist additional HTML attributes using `"extra_attrs"`. See [the Bleach documentation](https://bleach.readthedocs.io/en/latest/clean.html#allowed-tags-tags) for more information on this.
+Since extensions may introduce new HTML tags, you will also need to add those tags to the list of tags that are allowed by the [Bleach](https://bleach.readthedocs.io/) sanitizer. You can do that using the `"extra_tags"` key, and you can allow-list additional HTML attributes using `"extra_attrs"`. See [the Bleach documentation](https://bleach.readthedocs.io/en/latest/clean.html#allowed-tags-tags) for more information on this.
 
 Here's how to enable support for [Markdown tables](https://python-markdown.github.io/extensions/tables/):
 
 ```json
 {
     "plugins": {
         "datasette-render-markdown": {
@@ -142,15 +130,15 @@
 
 First, you will need to install the [py-gfm](https://py-gfm.readthedocs.io) package:
 
     $ pip install py-gfm
 
 Note that `py-gfm` has [a bug](https://github.com/Zopieux/py-gfm/issues/13) that causes it to pin to `Markdown<3.0` - so if you are using it you should install it _before_ installing `datasette-render-markdown` to ensure you get a compatibly version of that dependency.
 
-Now you can configure it like this. Note that the extension name is `mdx_gfm:GithubFlavoredMarkdownExtension` and you need to whitelist several extra HTML tags and attributes:
+Now you can configure it like this. Note that the extension name is `mdx_gfm:GithubFlavoredMarkdownExtension` and you need to allow-list several extra HTML tags and attributes:
 
 ```json
 {
     "plugins": {
         "datasette-render-markdown": {
             "extra_tags": [
                 "hr",
@@ -174,32 +162,50 @@
 }
 ```
 
 The `<input type="" checked disabled>` attributes are needed to support rendering checkboxes in issue descriptions.
 
 ## Markdown in templates
 
-The plugin also adds a new template function: `render_markdown(value)`. You can use this in your templates like so:
+The plugin introduces a new template tag: `{% markdown %}...{% endmarkdown %}` - which can be used to render Markdown in your Jinja templates.
 
 ```html+jinja
-{{ render_markdown("""
-# This is markdown
+{% markdown %}
+# This will be rendered as markdown
+{% endmarkdown %}
+```
+You can use attributes on the `{% markdown %}` tag to enable extensions and allow-list additional tags and attributes:
+```html+jinja
+{% markdown
+  extensions="tables"
+  extra_tags="table thead tr th td tbody" 
+  extra_attrs="p:id,class a:name,href" %}
+## Markdown table
+
+First Header  | Second Header
+------------- | -------------
+Content Cell  | Content Cell
+Content Cell  | Content Cell
 
-* One
-* Two
-* Three
-""") }}
+<a href="https://www.example.com/" name="namehere">Example</a>
+<p id="paragraph" class="klass">Paragraph</p>
+{% endmarkdown %}
 ```
+The `extensions=` and `extra_tags=` attributes accept a space-separated list of values.
+
+The `extra_attrs=` attribute accepts a space-separated list of `tag:attr1,attr2` values - each tag can specify one or more attributes that should be allowed.
 
-You can load additional extensions and whitelist tags by passing extra arguments to the function like this:
+You can also use the `{{ render_template(...) }}` function, like this:
 
 ```html+jinja
 {{ render_markdown("""
 ## Markdown table
 
 First Header  | Second Header
 ------------- | -------------
 Content Cell  | Content Cell
 Content Cell  | Content Cell
 """, extensions=["tables"],
     extra_tags=["table", "thead", "tr", "th", "td", "tbody"])) }}
 ```
+
+The `{% markdown %}` tag is recommended, as it avoids the need to `\"` escape quotes in your Markdown content.
```

### Comparing `datasette-render-markdown-2.1.1/README.md` & `datasette-render-markdown-2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: datasette-render-markdown
+Version: 2.2
+Summary: Datasette plugin for rendering Markdown
+Home-page: https://github.com/simonw/datasette-render-markdown
+Author: Simon Willison
+License: Apache License, Version 2.0
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
 # datasette-render-markdown
 
 [![PyPI](https://img.shields.io/pypi/v/datasette-render-markdown.svg)](https://pypi.org/project/datasette-render-markdown/)
 [![Changelog](https://img.shields.io/github/v/release/simonw/datasette-render-markdown?include_prereleases&label=changelog)](https://github.com/simonw/datasette-render-markdown/releases)
 [![Tests](https://github.com/simonw/datasette-render-markdown/workflows/Test/badge.svg)](https://github.com/simonw/datasette-render-markdown/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/datasette-render-markdown/blob/main/LICENSE)
 
@@ -105,15 +117,15 @@
 
 ## Markdown extensions
 
 The [Python-Markdown library](https://python-markdown.github.io/) that powers this plugin supports extensions, both [bundled](https://python-markdown.github.io/extensions/) and [third-party](https://github.com/Python-Markdown/markdown/wiki/Third-Party-Extensions). These can be used to enable additional Markdown features such as [table support](https://python-markdown.github.io/extensions/tables/).
 
 You can configure support for extensions using the `"extensions"` key in your plugin metadata configuration.
 
-Since extensions may introduce new HTML tags, you will also need to add those tags to the list of tags that are allowed by the [Bleach](https://bleach.readthedocs.io/) sanitizer. You can do that using the `"extra_tags"` key, and you can whitelist additional HTML attributes using `"extra_attrs"`. See [the Bleach documentation](https://bleach.readthedocs.io/en/latest/clean.html#allowed-tags-tags) for more information on this.
+Since extensions may introduce new HTML tags, you will also need to add those tags to the list of tags that are allowed by the [Bleach](https://bleach.readthedocs.io/) sanitizer. You can do that using the `"extra_tags"` key, and you can allow-list additional HTML attributes using `"extra_attrs"`. See [the Bleach documentation](https://bleach.readthedocs.io/en/latest/clean.html#allowed-tags-tags) for more information on this.
 
 Here's how to enable support for [Markdown tables](https://python-markdown.github.io/extensions/tables/):
 
 ```json
 {
     "plugins": {
         "datasette-render-markdown": {
@@ -130,15 +142,15 @@
 
 First, you will need to install the [py-gfm](https://py-gfm.readthedocs.io) package:
 
     $ pip install py-gfm
 
 Note that `py-gfm` has [a bug](https://github.com/Zopieux/py-gfm/issues/13) that causes it to pin to `Markdown<3.0` - so if you are using it you should install it _before_ installing `datasette-render-markdown` to ensure you get a compatibly version of that dependency.
 
-Now you can configure it like this. Note that the extension name is `mdx_gfm:GithubFlavoredMarkdownExtension` and you need to whitelist several extra HTML tags and attributes:
+Now you can configure it like this. Note that the extension name is `mdx_gfm:GithubFlavoredMarkdownExtension` and you need to allow-list several extra HTML tags and attributes:
 
 ```json
 {
     "plugins": {
         "datasette-render-markdown": {
             "extra_tags": [
                 "hr",
@@ -162,32 +174,50 @@
 }
 ```
 
 The `<input type="" checked disabled>` attributes are needed to support rendering checkboxes in issue descriptions.
 
 ## Markdown in templates
 
-The plugin also adds a new template function: `render_markdown(value)`. You can use this in your templates like so:
+The plugin introduces a new template tag: `{% markdown %}...{% endmarkdown %}` - which can be used to render Markdown in your Jinja templates.
 
 ```html+jinja
-{{ render_markdown("""
-# This is markdown
+{% markdown %}
+# This will be rendered as markdown
+{% endmarkdown %}
+```
+You can use attributes on the `{% markdown %}` tag to enable extensions and allow-list additional tags and attributes:
+```html+jinja
+{% markdown
+  extensions="tables"
+  extra_tags="table thead tr th td tbody" 
+  extra_attrs="p:id,class a:name,href" %}
+## Markdown table
+
+First Header  | Second Header
+------------- | -------------
+Content Cell  | Content Cell
+Content Cell  | Content Cell
 
-* One
-* Two
-* Three
-""") }}
+<a href="https://www.example.com/" name="namehere">Example</a>
+<p id="paragraph" class="klass">Paragraph</p>
+{% endmarkdown %}
 ```
+The `extensions=` and `extra_tags=` attributes accept a space-separated list of values.
+
+The `extra_attrs=` attribute accepts a space-separated list of `tag:attr1,attr2` values - each tag can specify one or more attributes that should be allowed.
 
-You can load additional extensions and whitelist tags by passing extra arguments to the function like this:
+You can also use the `{{ render_template(...) }}` function, like this:
 
 ```html+jinja
 {{ render_markdown("""
 ## Markdown table
 
 First Header  | Second Header
 ------------- | -------------
 Content Cell  | Content Cell
 Content Cell  | Content Cell
 """, extensions=["tables"],
     extra_tags=["table", "thead", "tr", "th", "td", "tbody"])) }}
 ```
+
+The `{% markdown %}` tag is recommended, as it avoids the need to `\"` escape quotes in your Markdown content.
```

### Comparing `datasette-render-markdown-2.1.1/datasette_render_markdown.egg-info/PKG-INFO` & `datasette-render-markdown-2.2/datasette_render_markdown.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-render-markdown
-Version: 2.1.1
+Version: 2.2
 Summary: Datasette plugin for rendering Markdown
 Home-page: https://github.com/simonw/datasette-render-markdown
 Author: Simon Willison
 License: Apache License, Version 2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
@@ -117,15 +117,15 @@
 
 ## Markdown extensions
 
 The [Python-Markdown library](https://python-markdown.github.io/) that powers this plugin supports extensions, both [bundled](https://python-markdown.github.io/extensions/) and [third-party](https://github.com/Python-Markdown/markdown/wiki/Third-Party-Extensions). These can be used to enable additional Markdown features such as [table support](https://python-markdown.github.io/extensions/tables/).
 
 You can configure support for extensions using the `"extensions"` key in your plugin metadata configuration.
 
-Since extensions may introduce new HTML tags, you will also need to add those tags to the list of tags that are allowed by the [Bleach](https://bleach.readthedocs.io/) sanitizer. You can do that using the `"extra_tags"` key, and you can whitelist additional HTML attributes using `"extra_attrs"`. See [the Bleach documentation](https://bleach.readthedocs.io/en/latest/clean.html#allowed-tags-tags) for more information on this.
+Since extensions may introduce new HTML tags, you will also need to add those tags to the list of tags that are allowed by the [Bleach](https://bleach.readthedocs.io/) sanitizer. You can do that using the `"extra_tags"` key, and you can allow-list additional HTML attributes using `"extra_attrs"`. See [the Bleach documentation](https://bleach.readthedocs.io/en/latest/clean.html#allowed-tags-tags) for more information on this.
 
 Here's how to enable support for [Markdown tables](https://python-markdown.github.io/extensions/tables/):
 
 ```json
 {
     "plugins": {
         "datasette-render-markdown": {
@@ -142,15 +142,15 @@
 
 First, you will need to install the [py-gfm](https://py-gfm.readthedocs.io) package:
 
     $ pip install py-gfm
 
 Note that `py-gfm` has [a bug](https://github.com/Zopieux/py-gfm/issues/13) that causes it to pin to `Markdown<3.0` - so if you are using it you should install it _before_ installing `datasette-render-markdown` to ensure you get a compatibly version of that dependency.
 
-Now you can configure it like this. Note that the extension name is `mdx_gfm:GithubFlavoredMarkdownExtension` and you need to whitelist several extra HTML tags and attributes:
+Now you can configure it like this. Note that the extension name is `mdx_gfm:GithubFlavoredMarkdownExtension` and you need to allow-list several extra HTML tags and attributes:
 
 ```json
 {
     "plugins": {
         "datasette-render-markdown": {
             "extra_tags": [
                 "hr",
@@ -174,32 +174,50 @@
 }
 ```
 
 The `<input type="" checked disabled>` attributes are needed to support rendering checkboxes in issue descriptions.
 
 ## Markdown in templates
 
-The plugin also adds a new template function: `render_markdown(value)`. You can use this in your templates like so:
+The plugin introduces a new template tag: `{% markdown %}...{% endmarkdown %}` - which can be used to render Markdown in your Jinja templates.
 
 ```html+jinja
-{{ render_markdown("""
-# This is markdown
+{% markdown %}
+# This will be rendered as markdown
+{% endmarkdown %}
+```
+You can use attributes on the `{% markdown %}` tag to enable extensions and allow-list additional tags and attributes:
+```html+jinja
+{% markdown
+  extensions="tables"
+  extra_tags="table thead tr th td tbody" 
+  extra_attrs="p:id,class a:name,href" %}
+## Markdown table
 
-* One
-* Two
-* Three
-""") }}
+First Header  | Second Header
+------------- | -------------
+Content Cell  | Content Cell
+Content Cell  | Content Cell
+
+<a href="https://www.example.com/" name="namehere">Example</a>
+<p id="paragraph" class="klass">Paragraph</p>
+{% endmarkdown %}
 ```
+The `extensions=` and `extra_tags=` attributes accept a space-separated list of values.
 
-You can load additional extensions and whitelist tags by passing extra arguments to the function like this:
+The `extra_attrs=` attribute accepts a space-separated list of `tag:attr1,attr2` values - each tag can specify one or more attributes that should be allowed.
+
+You can also use the `{{ render_template(...) }}` function, like this:
 
 ```html+jinja
 {{ render_markdown("""
 ## Markdown table
 
 First Header  | Second Header
 ------------- | -------------
 Content Cell  | Content Cell
 Content Cell  | Content Cell
 """, extensions=["tables"],
     extra_tags=["table", "thead", "tr", "th", "td", "tbody"])) }}
 ```
+
+The `{% markdown %}` tag is recommended, as it avoids the need to `\"` escape quotes in your Markdown content.
```

### Comparing `datasette-render-markdown-2.1.1/setup.py` & `datasette-render-markdown-2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "2.1.1"
+VERSION = "2.2"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
```

