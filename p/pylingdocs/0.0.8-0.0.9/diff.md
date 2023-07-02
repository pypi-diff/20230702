# Comparing `tmp/pylingdocs-0.0.8.tar.gz` & `tmp/pylingdocs-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pylingdocs-0.0.8.tar", last modified: Tue Aug 23 07:13:16 2022, max compression
+gzip compressed data, was "dist/pylingdocs-0.0.9.tar", last modified: Tue Sep 20 03:32:01 2022, max compression
```

## Comparing `pylingdocs-0.0.8.tar` & `pylingdocs-0.0.9.tar`

### file list

```diff
@@ -1,140 +1,139 @@
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      409 2022-08-23 07:13:11.000000 pylingdocs-0.0.8/CITATION.cff
--rw-rw-r--   0 florianm  (1000) florianm  (1000)    11359 2022-04-05 20:55:32.000000 pylingdocs-0.0.8/LICENSE
--rw-rw-r--   0 florianm  (1000) florianm  (1000)       94 2022-04-09 08:02:01.000000 pylingdocs-0.0.8/MANIFEST.in
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     2740 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/PKG-INFO
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1825 2022-08-20 07:32:37.000000 pylingdocs-0.0.8/README.md
--rw-r--r--   0 florianm  (1000) florianm  (1000)      568 2022-07-24 20:14:46.000000 pylingdocs-0.0.8/pyproject.toml
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1941 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/setup.cfg
--rw-rw-r--   0 florianm  (1000) florianm  (1000)       93 2022-04-07 19:28:48.000000 pylingdocs-0.0.8/setup.py
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/src/
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/src/pylingdocs/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      418 2022-08-23 07:12:47.000000 pylingdocs-0.0.8/src/pylingdocs/__init__.py
--rw-r--r--   0 florianm  (1000) florianm  (1000)     1514 2022-08-23 07:09:44.000000 pylingdocs-0.0.8/src/pylingdocs/cldf.py
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     6375 2022-08-23 06:55:37.000000 pylingdocs-0.0.8/src/pylingdocs/cli.py
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     2378 2022-08-20 06:36:10.000000 pylingdocs-0.0.8/src/pylingdocs/config.py
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/src/pylingdocs/data/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     3544 2022-04-13 08:24:24.000000 pylingdocs-0.0.8/src/pylingdocs/data/bibtex_schemes.json
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/src/pylingdocs/data/cldf/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1016 2022-05-30 16:52:50.000000 pylingdocs-0.0.8/src/pylingdocs/data/cldf/ChapterTable-metadata.json
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      745 2022-05-30 17:07:50.000000 pylingdocs-0.0.8/src/pylingdocs/data/cldf/ContributorTable-metadata.json
--rw-r--r--   0 florianm  (1000) florianm  (1000)     1362 2022-05-10 06:45:09.000000 pylingdocs-0.0.8/src/pylingdocs/data/cldf/ExampleSlices-metadata.json
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1575 2022-08-20 06:36:10.000000 pylingdocs-0.0.8/src/pylingdocs/data/config.cfg
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/github/
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/github/basic/
--rw-r--r--   0 florianm  (1000) florianm  (1000)      285 2022-04-28 16:29:26.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/github/basic/cookiecutter.json
--rw-r--r--   0 florianm  (1000) florianm  (1000)       13 2022-04-08 15:52:24.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/github/basic/part_template
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/github/basic/{{cookiecutter.name}}/
--rw-r--r--   0 florianm  (1000) florianm  (1000)       60 2022-04-13 15:45:09.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/github/basic/{{cookiecutter.name}}/README.md
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/html/
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/html/basic/
--rw-r--r--   0 florianm  (1000) florianm  (1000)      371 2022-06-10 23:52:16.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/html/basic/cookiecutter.json
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/html/basic/hooks/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      510 2022-08-20 06:36:10.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/html/basic/hooks/post_gen_project.py
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      127 2022-04-13 06:10:44.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/html/basic/part_template
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/html/basic/{{cookiecutter.name}}/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1257 2022-08-20 06:36:10.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/html/basic/{{cookiecutter.name}}/index.html
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/html/slides/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      371 2022-08-20 06:36:10.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/html/slides/cookiecutter.json
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/html/slides/hooks/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      510 2022-08-20 06:36:10.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/html/slides/hooks/post_gen_project.py
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/html/slides/{{cookiecutter.name}}/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     7078 2022-08-20 06:36:10.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/html/slides/{{cookiecutter.name}}/index.html
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/latex/
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/latex/article/
--rw-r--r--   0 florianm  (1000) florianm  (1000)      466 2022-06-11 20:38:07.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/latex/article/cookiecutter.json
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/latex/article/hooks/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      221 2022-05-26 18:06:31.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/latex/article/hooks/post_gen_project.py
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/latex/article/{{cookiecutter.name}}/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)    28122 2022-05-24 00:24:06.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/latex/article/{{cookiecutter.name}}/expex-acro.sty
--rw-r--r--   0 florianm  (1000) florianm  (1000)      686 2022-06-11 20:46:03.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/latex/article/{{cookiecutter.name}}/main.tex
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/latex/handout/
--rw-r--r--   0 florianm  (1000) florianm  (1000)      444 2022-05-25 21:40:10.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/latex/handout/cookiecutter.json
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/latex/handout/hooks/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      221 2022-05-26 18:06:31.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/latex/handout/hooks/post_gen_project.py
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/latex/handout/{{cookiecutter.name}}/
--rw-r--r--   0 florianm  (1000) florianm  (1000)      622 2022-06-03 20:41:16.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/latex/handout/{{cookiecutter.name}}/main.tex
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/latex/memoir/
--rw-r--r--   0 florianm  (1000) florianm  (1000)      444 2022-05-20 22:42:54.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/latex/memoir/cookiecutter.json
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/latex/memoir/hooks/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      221 2022-05-26 18:06:31.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/latex/memoir/hooks/post_gen_project.py
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/latex/memoir/{{cookiecutter.name}}/
--rw-r--r--   0 florianm  (1000) florianm  (1000)      910 2022-06-03 20:41:19.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/latex/memoir/{{cookiecutter.name}}/main.tex
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      512 2022-05-25 21:18:24.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/latex/memoir/{{cookiecutter.name}}/titlepage.tex
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      268 2022-06-11 01:27:27.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/latex/shared_preamble.tex
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/plain/
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/plain/basic/
--rw-r--r--   0 florianm  (1000) florianm  (1000)       89 2022-04-28 16:28:57.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/plain/basic/cookiecutter.json
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/plain/basic/{{cookiecutter.name}}/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)       30 2022-04-10 19:33:10.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/plain/basic/{{cookiecutter.name}}/.gitignore
--rw-rw-r--   0 florianm  (1000) florianm  (1000)       26 2022-04-13 15:40:30.000000 pylingdocs-0.0.8/src/pylingdocs/data/format_templates/plain/basic/{{cookiecutter.name}}/document.txt
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/src/pylingdocs/data/model_templates/
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/src/pylingdocs/data/model_templates/base/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      318 2022-04-26 12:47:49.000000 pylingdocs-0.0.8/src/pylingdocs/data/model_templates/base/inline_list.md
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      315 2022-04-26 12:48:06.000000 pylingdocs-0.0.8/src/pylingdocs/data/model_templates/base/inline_list_orm.md
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/src/pylingdocs/data/model_templates/cognateset/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      653 2022-08-20 06:36:10.000000 pylingdocs-0.0.8/src/pylingdocs/data/model_templates/cognateset/html_detail.md
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/src/pylingdocs/data/model_templates/example/
--rw-r--r--   0 florianm  (1000) florianm  (1000)      340 2022-06-13 01:32:18.000000 pylingdocs-0.0.8/src/pylingdocs/data/model_templates/example/html.md
--rw-r--r--   0 florianm  (1000) florianm  (1000)      623 2022-05-31 02:07:21.000000 pylingdocs-0.0.8/src/pylingdocs/data/model_templates/example/html_index.md
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1426 2022-06-07 15:34:25.000000 pylingdocs-0.0.8/src/pylingdocs/data/model_templates/example/latex_expex.md
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1612 2022-08-20 06:36:10.000000 pylingdocs-0.0.8/src/pylingdocs/data/model_templates/example/latex_index_expex.md
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      698 2022-06-10 22:09:15.000000 pylingdocs-0.0.8/src/pylingdocs/data/model_templates/example/plain.md
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      730 2022-06-08 19:53:42.000000 pylingdocs-0.0.8/src/pylingdocs/data/model_templates/example/plain_index.md
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1075 2022-06-13 16:40:18.000000 pylingdocs-0.0.8/src/pylingdocs/data/model_templates/html_util.md
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      347 2022-06-07 15:34:25.000000 pylingdocs-0.0.8/src/pylingdocs/data/model_templates/latex_util.md
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/src/pylingdocs/data/model_templates/morpheme/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      298 2022-07-21 15:44:48.000000 pylingdocs-0.0.8/src/pylingdocs/data/model_templates/morpheme/github.md
--rw-r--r--   0 florianm  (1000) florianm  (1000)      292 2022-05-24 21:46:30.000000 pylingdocs-0.0.8/src/pylingdocs/data/model_templates/morpheme/github_index.md
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      277 2022-06-13 19:01:23.000000 pylingdocs-0.0.8/src/pylingdocs/data/model_templates/morpheme/html.md
--rw-r--r--   0 florianm  (1000) florianm  (1000)      297 2022-05-24 21:46:26.000000 pylingdocs-0.0.8/src/pylingdocs/data/model_templates/morpheme/html_index.md
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      302 2022-06-13 19:01:35.000000 pylingdocs-0.0.8/src/pylingdocs/data/model_templates/morpheme/latex.md
--rw-r--r--   0 florianm  (1000) florianm  (1000)      297 2022-05-24 21:46:24.000000 pylingdocs-0.0.8/src/pylingdocs/data/model_templates/morpheme/latex_index.md
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      260 2022-07-21 15:27:26.000000 pylingdocs-0.0.8/src/pylingdocs/data/model_templates/morpheme/plain.md
--rw-r--r--   0 florianm  (1000) florianm  (1000)      284 2022-07-21 15:47:38.000000 pylingdocs-0.0.8/src/pylingdocs/data/model_templates/morpheme/plain_index.md
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/src/pylingdocs/data/model_templates/wordform/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      286 2022-06-13 15:38:55.000000 pylingdocs-0.0.8/src/pylingdocs/data/model_templates/wordform/html.md
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      409 2022-06-13 19:39:47.000000 pylingdocs-0.0.8/src/pylingdocs/data/model_templates/wordform/html_index.md
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      320 2022-06-13 18:50:55.000000 pylingdocs-0.0.8/src/pylingdocs/data/model_templates/wordform/latex.md
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      438 2022-06-13 19:43:43.000000 pylingdocs-0.0.8/src/pylingdocs/data/model_templates/wordform/latex_index.md
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      269 2022-06-13 16:43:39.000000 pylingdocs-0.0.8/src/pylingdocs/data/model_templates/wordform/plain.md
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      396 2022-06-13 19:43:18.000000 pylingdocs-0.0.8/src/pylingdocs/data/model_templates/wordform/plain_index.md
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/src/pylingdocs/data/project_template/
--rw-r--r--   0 florianm  (1000) florianm  (1000)      563 2022-04-28 09:39:05.000000 pylingdocs-0.0.8/src/pylingdocs/data/project_template/cookiecutter.json
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/src/pylingdocs/data/project_template/hooks/
--rw-r--r--   0 florianm  (1000) florianm  (1000)      562 2022-07-22 15:43:53.000000 pylingdocs-0.0.8/src/pylingdocs/data/project_template/hooks/post_gen_project.py
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/src/pylingdocs/data/project_template/{{cookiecutter.name}}/
--rw-r--r--   0 florianm  (1000) florianm  (1000)    45999 2022-04-28 09:09:21.000000 pylingdocs-0.0.8/src/pylingdocs/data/project_template/{{cookiecutter.name}}/LICENSE
--rw-r--r--   0 florianm  (1000) florianm  (1000)      127 2022-04-28 09:35:16.000000 pylingdocs-0.0.8/src/pylingdocs/data/project_template/{{cookiecutter.name}}/README.md
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/src/pylingdocs/data/project_template/{{cookiecutter.name}}/content/
--rw-r--r--   0 florianm  (1000) florianm  (1000)      152 2022-04-28 09:39:26.000000 pylingdocs-0.0.8/src/pylingdocs/data/project_template/{{cookiecutter.name}}/content/structure.yaml
--rw-r--r--   0 florianm  (1000) florianm  (1000)      240 2022-04-29 09:45:15.000000 pylingdocs-0.0.8/src/pylingdocs/data/project_template/{{cookiecutter.name}}/content/{{cookiecutter.name}}.sublime-project
--rw-r--r--   0 florianm  (1000) florianm  (1000)      783 2022-04-28 09:27:14.000000 pylingdocs-0.0.8/src/pylingdocs/data/project_template/{{cookiecutter.name}}/metadata.yaml
--rw-r--r--   0 florianm  (1000) florianm  (1000)       92 2022-04-28 09:33:59.000000 pylingdocs-0.0.8/src/pylingdocs/data/project_template/{{cookiecutter.name}}/pylingdocs.cfg
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/src/pylingdocs/data/project_template/{{cookiecutter.name}}/tables/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)       60 2022-06-08 21:10:13.000000 pylingdocs-0.0.8/src/pylingdocs/data/project_template/{{cookiecutter.name}}/tables/table_metadata.yaml
--rw-r--r--   0 florianm  (1000) florianm  (1000)       53 2022-04-28 09:33:24.000000 pylingdocs-0.0.8/src/pylingdocs/data/project_template/{{cookiecutter.name}}/tables/verb_templ.csv
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1883 2022-06-13 21:44:19.000000 pylingdocs-0.0.8/src/pylingdocs/data/util.md
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/src/pylingdocs/data/web/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     3513 2022-08-20 06:36:10.000000 pylingdocs-0.0.8/src/pylingdocs/data/web/alignment.css
--rw-rw-r--   0 florianm  (1000) florianm  (1000)    14864 2022-08-20 06:36:10.000000 pylingdocs-0.0.8/src/pylingdocs/data/web/alignment.js
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     3591 2022-08-20 06:36:10.000000 pylingdocs-0.0.8/src/pylingdocs/data/web/crossref.js
--rw-r--r--   0 florianm  (1000) florianm  (1000)      505 2022-05-04 10:39:17.000000 pylingdocs-0.0.8/src/pylingdocs/data/web/examples.css
--rw-r--r--   0 florianm  (1000) florianm  (1000)     1509 2022-07-30 19:12:29.000000 pylingdocs-0.0.8/src/pylingdocs/data/web/examples.js
--rw-r--r--   0 florianm  (1000) florianm  (1000)      494 2022-05-26 04:24:27.000000 pylingdocs-0.0.8/src/pylingdocs/data/web/glossing.js
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     3538 2022-08-20 06:36:10.000000 pylingdocs-0.0.8/src/pylingdocs/data/web/styling.css
--rw-rw-r--   0 florianm  (1000) florianm  (1000)    12891 2022-08-23 06:59:57.000000 pylingdocs-0.0.8/src/pylingdocs/helpers.py
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     3664 2022-05-30 18:45:03.000000 pylingdocs-0.0.8/src/pylingdocs/metadata.py
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     7589 2022-08-20 06:36:10.000000 pylingdocs-0.0.8/src/pylingdocs/models.py
--rw-rw-r--   0 florianm  (1000) florianm  (1000)    29641 2022-08-23 06:46:42.000000 pylingdocs-0.0.8/src/pylingdocs/output.py
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      994 2022-04-14 09:08:11.000000 pylingdocs-0.0.8/src/pylingdocs/pandoc_filters.py
--rw-rw-r--   0 florianm  (1000) florianm  (1000)    12121 2022-07-21 18:15:23.000000 pylingdocs-0.0.8/src/pylingdocs/preprocessing.py
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/src/pylingdocs.egg-info/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     2740 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/src/pylingdocs.egg-info/PKG-INFO
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     5170 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/src/pylingdocs.egg-info/SOURCES.txt
--rw-rw-r--   0 florianm  (1000) florianm  (1000)        1 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/src/pylingdocs.egg-info/dependency_links.txt
--rw-rw-r--   0 florianm  (1000) florianm  (1000)       51 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/src/pylingdocs.egg-info/entry_points.txt
--rw-rw-r--   0 florianm  (1000) florianm  (1000)        1 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/src/pylingdocs.egg-info/not-zip-safe
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      387 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/src/pylingdocs.egg-info/requires.txt
--rw-rw-r--   0 florianm  (1000) florianm  (1000)       11 2022-08-23 07:13:16.000000 pylingdocs-0.0.8/src/pylingdocs.egg-info/top_level.txt
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      409 2022-09-20 03:31:57.000000 pylingdocs-0.0.9/CITATION.cff
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)    11359 2022-04-05 20:55:32.000000 pylingdocs-0.0.9/LICENSE
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)       94 2022-04-09 08:02:01.000000 pylingdocs-0.0.9/MANIFEST.in
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     2740 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/PKG-INFO
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1825 2022-08-20 07:32:37.000000 pylingdocs-0.0.9/README.md
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      568 2022-07-24 20:14:46.000000 pylingdocs-0.0.9/pyproject.toml
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1941 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/setup.cfg
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)       93 2022-04-07 19:28:48.000000 pylingdocs-0.0.9/setup.py
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/src/
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/src/pylingdocs/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      418 2022-09-20 03:31:40.000000 pylingdocs-0.0.9/src/pylingdocs/__init__.py
+-rw-r--r--   0 florianm  (1000) florianm  (1000)     1514 2022-08-23 07:09:44.000000 pylingdocs-0.0.9/src/pylingdocs/cldf.py
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     6395 2022-09-18 15:04:28.000000 pylingdocs-0.0.9/src/pylingdocs/cli.py
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     2118 2022-09-19 18:42:14.000000 pylingdocs-0.0.9/src/pylingdocs/config.py
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/src/pylingdocs/data/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     3544 2022-04-13 08:24:24.000000 pylingdocs-0.0.9/src/pylingdocs/data/bibtex_schemes.json
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/src/pylingdocs/data/cldf/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1016 2022-05-30 16:52:50.000000 pylingdocs-0.0.9/src/pylingdocs/data/cldf/ChapterTable-metadata.json
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      745 2022-05-30 17:07:50.000000 pylingdocs-0.0.9/src/pylingdocs/data/cldf/ContributorTable-metadata.json
+-rw-r--r--   0 florianm  (1000) florianm  (1000)     1362 2022-05-10 06:45:09.000000 pylingdocs-0.0.9/src/pylingdocs/data/cldf/ExampleSlices-metadata.json
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1576 2022-09-19 18:41:46.000000 pylingdocs-0.0.9/src/pylingdocs/data/config.cfg
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/github/
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/github/basic/
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      285 2022-04-28 16:29:26.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/github/basic/cookiecutter.json
+-rw-r--r--   0 florianm  (1000) florianm  (1000)       13 2022-04-08 15:52:24.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/github/basic/part_template
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/github/basic/{{cookiecutter.name}}/
+-rw-r--r--   0 florianm  (1000) florianm  (1000)       60 2022-04-13 15:45:09.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/github/basic/{{cookiecutter.name}}/README.md
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/html/
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/html/basic/
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      371 2022-06-10 23:52:16.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/html/basic/cookiecutter.json
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/html/basic/hooks/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      510 2022-08-20 06:36:10.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/html/basic/hooks/post_gen_project.py
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      127 2022-04-13 06:10:44.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/html/basic/part_template
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/html/basic/{{cookiecutter.name}}/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1245 2022-09-18 00:06:42.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/html/basic/{{cookiecutter.name}}/index.html
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/html/slides/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      371 2022-08-20 06:36:10.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/html/slides/cookiecutter.json
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/html/slides/hooks/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      510 2022-08-20 06:36:10.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/html/slides/hooks/post_gen_project.py
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/html/slides/{{cookiecutter.name}}/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     7078 2022-08-20 06:36:10.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/html/slides/{{cookiecutter.name}}/index.html
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/latex/
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/latex/article/
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      466 2022-06-11 20:38:07.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/latex/article/cookiecutter.json
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/latex/article/hooks/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      221 2022-05-26 18:06:31.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/latex/article/hooks/post_gen_project.py
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/latex/article/{{cookiecutter.name}}/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)    28122 2022-05-24 00:24:06.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/latex/article/{{cookiecutter.name}}/expex-acro.sty
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      686 2022-06-11 20:46:03.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/latex/article/{{cookiecutter.name}}/main.tex
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/latex/handout/
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      444 2022-05-25 21:40:10.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/latex/handout/cookiecutter.json
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/latex/handout/hooks/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      221 2022-05-26 18:06:31.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/latex/handout/hooks/post_gen_project.py
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/latex/handout/{{cookiecutter.name}}/
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      622 2022-06-03 20:41:16.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/latex/handout/{{cookiecutter.name}}/main.tex
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/latex/memoir/
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      444 2022-05-20 22:42:54.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/latex/memoir/cookiecutter.json
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/latex/memoir/hooks/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      221 2022-05-26 18:06:31.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/latex/memoir/hooks/post_gen_project.py
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/latex/memoir/{{cookiecutter.name}}/
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      910 2022-06-03 20:41:19.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/latex/memoir/{{cookiecutter.name}}/main.tex
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      512 2022-05-25 21:18:24.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/latex/memoir/{{cookiecutter.name}}/titlepage.tex
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      268 2022-06-11 01:27:27.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/latex/shared_preamble.tex
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/plain/
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/plain/basic/
+-rw-r--r--   0 florianm  (1000) florianm  (1000)       89 2022-04-28 16:28:57.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/plain/basic/cookiecutter.json
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/plain/basic/{{cookiecutter.name}}/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)       30 2022-04-10 19:33:10.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/plain/basic/{{cookiecutter.name}}/.gitignore
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)       26 2022-04-13 15:40:30.000000 pylingdocs-0.0.9/src/pylingdocs/data/format_templates/plain/basic/{{cookiecutter.name}}/document.txt
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/src/pylingdocs/data/model_templates/
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/src/pylingdocs/data/model_templates/base/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      318 2022-04-26 12:47:49.000000 pylingdocs-0.0.9/src/pylingdocs/data/model_templates/base/inline_list.md
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      315 2022-04-26 12:48:06.000000 pylingdocs-0.0.9/src/pylingdocs/data/model_templates/base/inline_list_orm.md
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/src/pylingdocs/data/model_templates/cognateset/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      653 2022-08-20 06:36:10.000000 pylingdocs-0.0.9/src/pylingdocs/data/model_templates/cognateset/html_detail.md
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/src/pylingdocs/data/model_templates/example/
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      340 2022-06-13 01:32:18.000000 pylingdocs-0.0.9/src/pylingdocs/data/model_templates/example/html.md
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      623 2022-05-31 02:07:21.000000 pylingdocs-0.0.9/src/pylingdocs/data/model_templates/example/html_index.md
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1426 2022-06-07 15:34:25.000000 pylingdocs-0.0.9/src/pylingdocs/data/model_templates/example/latex_expex.md
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1612 2022-08-20 06:36:10.000000 pylingdocs-0.0.9/src/pylingdocs/data/model_templates/example/latex_index_expex.md
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      698 2022-06-10 22:09:15.000000 pylingdocs-0.0.9/src/pylingdocs/data/model_templates/example/plain.md
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      730 2022-06-08 19:53:42.000000 pylingdocs-0.0.9/src/pylingdocs/data/model_templates/example/plain_index.md
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1075 2022-06-13 16:40:18.000000 pylingdocs-0.0.9/src/pylingdocs/data/model_templates/html_util.md
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      347 2022-06-07 15:34:25.000000 pylingdocs-0.0.9/src/pylingdocs/data/model_templates/latex_util.md
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/src/pylingdocs/data/model_templates/morpheme/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      298 2022-07-21 15:44:48.000000 pylingdocs-0.0.9/src/pylingdocs/data/model_templates/morpheme/github.md
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      292 2022-05-24 21:46:30.000000 pylingdocs-0.0.9/src/pylingdocs/data/model_templates/morpheme/github_index.md
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      277 2022-06-13 19:01:23.000000 pylingdocs-0.0.9/src/pylingdocs/data/model_templates/morpheme/html.md
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      297 2022-05-24 21:46:26.000000 pylingdocs-0.0.9/src/pylingdocs/data/model_templates/morpheme/html_index.md
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      302 2022-06-13 19:01:35.000000 pylingdocs-0.0.9/src/pylingdocs/data/model_templates/morpheme/latex.md
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      297 2022-05-24 21:46:24.000000 pylingdocs-0.0.9/src/pylingdocs/data/model_templates/morpheme/latex_index.md
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      260 2022-07-21 15:27:26.000000 pylingdocs-0.0.9/src/pylingdocs/data/model_templates/morpheme/plain.md
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      284 2022-07-21 15:47:38.000000 pylingdocs-0.0.9/src/pylingdocs/data/model_templates/morpheme/plain_index.md
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/src/pylingdocs/data/model_templates/wordform/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      286 2022-06-13 15:38:55.000000 pylingdocs-0.0.9/src/pylingdocs/data/model_templates/wordform/html.md
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      409 2022-06-13 19:39:47.000000 pylingdocs-0.0.9/src/pylingdocs/data/model_templates/wordform/html_index.md
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      320 2022-06-13 18:50:55.000000 pylingdocs-0.0.9/src/pylingdocs/data/model_templates/wordform/latex.md
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      438 2022-06-13 19:43:43.000000 pylingdocs-0.0.9/src/pylingdocs/data/model_templates/wordform/latex_index.md
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      269 2022-06-13 16:43:39.000000 pylingdocs-0.0.9/src/pylingdocs/data/model_templates/wordform/plain.md
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      396 2022-06-13 19:43:18.000000 pylingdocs-0.0.9/src/pylingdocs/data/model_templates/wordform/plain_index.md
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/src/pylingdocs/data/project_template/
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      563 2022-04-28 09:39:05.000000 pylingdocs-0.0.9/src/pylingdocs/data/project_template/cookiecutter.json
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/src/pylingdocs/data/project_template/hooks/
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      856 2022-09-19 20:12:46.000000 pylingdocs-0.0.9/src/pylingdocs/data/project_template/hooks/post_gen_project.py
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/src/pylingdocs/data/project_template/{{cookiecutter.name}}/
+-rw-r--r--   0 florianm  (1000) florianm  (1000)    45999 2022-04-28 09:09:21.000000 pylingdocs-0.0.9/src/pylingdocs/data/project_template/{{cookiecutter.name}}/LICENSE
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      127 2022-04-28 09:35:16.000000 pylingdocs-0.0.9/src/pylingdocs/data/project_template/{{cookiecutter.name}}/README.md
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/src/pylingdocs/data/project_template/{{cookiecutter.name}}/content/
+-rw-r--r--   0 florianm  (1000) florianm  (1000)       88 2022-09-18 00:19:51.000000 pylingdocs-0.0.9/src/pylingdocs/data/project_template/{{cookiecutter.name}}/content/structure.yaml
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      240 2022-04-29 09:45:15.000000 pylingdocs-0.0.9/src/pylingdocs/data/project_template/{{cookiecutter.name}}/content/{{cookiecutter.name}}.sublime-project
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      783 2022-04-28 09:27:14.000000 pylingdocs-0.0.9/src/pylingdocs/data/project_template/{{cookiecutter.name}}/metadata.yaml
+-rw-r--r--   0 florianm  (1000) florianm  (1000)       92 2022-09-19 18:42:45.000000 pylingdocs-0.0.9/src/pylingdocs/data/project_template/{{cookiecutter.name}}/pylingdocs.cfg
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/src/pylingdocs/data/project_template/{{cookiecutter.name}}/tables/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)       60 2022-06-08 21:10:13.000000 pylingdocs-0.0.9/src/pylingdocs/data/project_template/{{cookiecutter.name}}/tables/table_metadata.yaml
+-rw-r--r--   0 florianm  (1000) florianm  (1000)       53 2022-04-28 09:33:24.000000 pylingdocs-0.0.9/src/pylingdocs/data/project_template/{{cookiecutter.name}}/tables/verb_templ.csv
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1883 2022-06-13 21:44:19.000000 pylingdocs-0.0.9/src/pylingdocs/data/util.md
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/src/pylingdocs/data/web/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     3513 2022-08-20 06:36:10.000000 pylingdocs-0.0.9/src/pylingdocs/data/web/alignment.css
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)    14864 2022-08-20 06:36:10.000000 pylingdocs-0.0.9/src/pylingdocs/data/web/alignment.js
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     3591 2022-08-20 06:36:10.000000 pylingdocs-0.0.9/src/pylingdocs/data/web/crossref.js
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      505 2022-05-04 10:39:17.000000 pylingdocs-0.0.9/src/pylingdocs/data/web/examples.css
+-rw-r--r--   0 florianm  (1000) florianm  (1000)     1509 2022-07-30 19:12:29.000000 pylingdocs-0.0.9/src/pylingdocs/data/web/examples.js
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      524 2022-09-18 18:42:57.000000 pylingdocs-0.0.9/src/pylingdocs/data/web/glossing.js
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     3538 2022-08-20 06:36:10.000000 pylingdocs-0.0.9/src/pylingdocs/data/web/styling.css
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)    12889 2022-09-18 22:22:38.000000 pylingdocs-0.0.9/src/pylingdocs/helpers.py
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     3434 2022-09-19 00:51:25.000000 pylingdocs-0.0.9/src/pylingdocs/metadata.py
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     7589 2022-08-20 06:36:10.000000 pylingdocs-0.0.9/src/pylingdocs/models.py
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)    28641 2022-09-19 01:12:46.000000 pylingdocs-0.0.9/src/pylingdocs/output.py
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)    12041 2022-09-18 17:02:32.000000 pylingdocs-0.0.9/src/pylingdocs/preprocessing.py
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/src/pylingdocs.egg-info/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     2740 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/src/pylingdocs.egg-info/PKG-INFO
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     5137 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/src/pylingdocs.egg-info/SOURCES.txt
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)        1 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/src/pylingdocs.egg-info/dependency_links.txt
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)       51 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/src/pylingdocs.egg-info/entry_points.txt
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)        1 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/src/pylingdocs.egg-info/not-zip-safe
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      387 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/src/pylingdocs.egg-info/requires.txt
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)       11 2022-09-20 03:32:01.000000 pylingdocs-0.0.9/src/pylingdocs.egg-info/top_level.txt
```

### Comparing `pylingdocs-0.0.8/LICENSE` & `pylingdocs-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pylingdocs-0.0.8/PKG-INFO` & `pylingdocs-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylingdocs
-Version: 0.0.8
+Version: 0.0.9
 Summary: Create data-rich linguistic documents.
 Home-page: https://github.com/fmatter/pylingdocs
 Author: Florian Matter
 Author-email: florianmatter@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/fmatter/pylingdocs/issues
 Keywords: digital linguistics,CLDF
```

### Comparing `pylingdocs-0.0.8/README.md` & `pylingdocs-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pylingdocs-0.0.8/pyproject.toml` & `pylingdocs-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pylingdocs-0.0.8/setup.cfg` & `pylingdocs-0.0.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 	CLDF
 long_description = file: README.md
 long_description_content_type = text/markdown
 name = pylingdocs
 project_urls = 
 	Bug Tracker = https://github.com/fmatter/pylingdocs/issues
 url = https://github.com/fmatter/pylingdocs
-version = 0.0.8
+version = 0.0.9
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 package_dir = 
 	=src
```

### Comparing `pylingdocs-0.0.8/src/pylingdocs/cldf.py` & `pylingdocs-0.0.9/src/pylingdocs/cldf.py`

 * *Files identical despite different names*

### Comparing `pylingdocs-0.0.8/src/pylingdocs/cli.py` & `pylingdocs-0.0.9/src/pylingdocs/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from pylingdocs.config import CREATE_README
 from pylingdocs.config import METADATA_FILE
 from pylingdocs.config import OUTPUT_DIR
 from pylingdocs.config import PREVIEW
 from pylingdocs.config import STRUCTURE_FILE
 from pylingdocs.helpers import _get_relative_file
 from pylingdocs.helpers import _load_cldf_dataset
-from pylingdocs.helpers import _load_structure
 from pylingdocs.helpers import load_content
 from pylingdocs.helpers import new as create_new
 from pylingdocs.helpers import write_readme
 from pylingdocs.metadata import _load_metadata
 from pylingdocs.output import check_ids
 from pylingdocs.output import clean_output
 from pylingdocs.output import compile_latex as cmplatex
@@ -146,18 +145,21 @@
 
 
 @main.command(cls=BuildCommand)
 def check(source, cldf, output_dir, latex):
     del output_dir
     del latex
     ds = _load_cldf_dataset(cldf)
-    structure = _load_structure(
-        _get_relative_file(folder=source / CONTENT_FOLDER, file=STRUCTURE_FILE)
+    contents = load_content(
+        source_dir=source / CONTENT_FOLDER,
+        structure_file=_get_relative_file(
+            folder=source / CONTENT_FOLDER, file=STRUCTURE_FILE
+        ),
     )
-    check_ids(source, ds, structure=structure)
+    check_ids(contents, ds, source)
 
 
 @main.command()
 def update_structure():
     do_update_structure()
```

### Comparing `pylingdocs-0.0.8/src/pylingdocs/data/bibtex_schemes.json` & `pylingdocs-0.0.9/src/pylingdocs/data/bibtex_schemes.json`

 * *Files identical despite different names*

### Comparing `pylingdocs-0.0.8/src/pylingdocs/data/cldf/ChapterTable-metadata.json` & `pylingdocs-0.0.9/src/pylingdocs/data/cldf/ChapterTable-metadata.json`

 * *Files identical despite different names*

### Comparing `pylingdocs-0.0.8/src/pylingdocs/data/cldf/ContributorTable-metadata.json` & `pylingdocs-0.0.9/src/pylingdocs/data/cldf/ContributorTable-metadata.json`

 * *Files identical despite different names*

### Comparing `pylingdocs-0.0.8/src/pylingdocs/data/cldf/ExampleSlices-metadata.json` & `pylingdocs-0.0.9/src/pylingdocs/data/cldf/ExampleSlices-metadata.json`

 * *Files identical despite different names*

### Comparing `pylingdocs-0.0.8/src/pylingdocs/data/config.cfg` & `pylingdocs-0.0.9/src/pylingdocs/data/config.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[PATHS]
+[paths]
 
 # the folder containing your text files
 content = content
 
 # the folder containing text files not (currently) included in the project
 bench = bench
 
@@ -13,30 +13,30 @@
 # the folder to which output is written 
 output = output
 
 # the folder where CSV for tables are stored
 tables = tables 
 
 # the folder where your images are stored
-figures = images
+figures = figures
 
 # the table metadata file
 # if this is a plain filename, it is assumed to be in the tables folder
 table_metadata = table_metadata.yaml
 
 # the path to the CLDF metadata file 
 cldf = ./cldf/metadata.json
 
 # the path to the manual example folder
 manual_examples = ./manual_examples
 
 # path to bibfile not contained in the dataset
 add_bib = additional_refs.bib
 
-[OUTPUT]
+[output]
 
 # what formats should be built
 builders = plain github html latex
 
 # what formats should be built as preview
 preview = plain html
```

### Comparing `pylingdocs-0.0.8/src/pylingdocs/data/format_templates/html/basic/{{cookiecutter.name}}/index.html` & `pylingdocs-0.0.9/src/pylingdocs/data/format_templates/html/basic/{{cookiecutter.name}}/index.html`

 * *Files 16% similar despite different names*

```diff
@@ -23,18 +23,18 @@
     </article>
     <script src="examples.js"></script> 
     <script src="glossing.js"></script> 
     <script src="crossref.js"></script>
     <script src="alignment.js"></script>
     <script type="text/javascript" src="https://livejs.com/live.js"></script>
     <script>
-// number_examples()
-// number_sections()
-// number_captions()
-// resolve_crossrefs()
+number_examples()
+number_sections()
+number_captions()
+resolve_crossrefs()
 </script>
 <script>
     var alignments = document.getElementsByClassName("alignment");
     for (var i=0,alignment; alignment=alignments[i]; i++) {
         alignment.innerHTML = plotWord(alignment.innerHTML, 'span');
     }
 </script>
```

### Comparing `pylingdocs-0.0.8/src/pylingdocs/data/format_templates/html/slides/{{cookiecutter.name}}/index.html` & `pylingdocs-0.0.9/src/pylingdocs/data/format_templates/html/slides/{{cookiecutter.name}}/index.html`

 * *Files identical despite different names*

### Comparing `pylingdocs-0.0.8/src/pylingdocs/data/format_templates/latex/article/{{cookiecutter.name}}/expex-acro.sty` & `pylingdocs-0.0.9/src/pylingdocs/data/format_templates/latex/article/{{cookiecutter.name}}/expex-acro.sty`

 * *Files identical despite different names*

### Comparing `pylingdocs-0.0.8/src/pylingdocs/data/format_templates/latex/article/{{cookiecutter.name}}/main.tex` & `pylingdocs-0.0.9/src/pylingdocs/data/format_templates/latex/article/{{cookiecutter.name}}/main.tex`

 * *Files identical despite different names*

### Comparing `pylingdocs-0.0.8/src/pylingdocs/data/format_templates/latex/handout/{{cookiecutter.name}}/main.tex` & `pylingdocs-0.0.9/src/pylingdocs/data/format_templates/latex/handout/{{cookiecutter.name}}/main.tex`

 * *Files identical despite different names*

### Comparing `pylingdocs-0.0.8/src/pylingdocs/data/format_templates/latex/memoir/{{cookiecutter.name}}/main.tex` & `pylingdocs-0.0.9/src/pylingdocs/data/format_templates/latex/memoir/{{cookiecutter.name}}/main.tex`

 * *Files identical despite different names*

### Comparing `pylingdocs-0.0.8/src/pylingdocs/data/format_templates/latex/memoir/{{cookiecutter.name}}/titlepage.tex` & `pylingdocs-0.0.9/src/pylingdocs/data/format_templates/latex/memoir/{{cookiecutter.name}}/titlepage.tex`

 * *Files identical despite different names*

### Comparing `pylingdocs-0.0.8/src/pylingdocs/data/model_templates/cognateset/html_detail.md` & `pylingdocs-0.0.9/src/pylingdocs/data/model_templates/cognateset/html_detail.md`

 * *Files identical despite different names*

### Comparing `pylingdocs-0.0.8/src/pylingdocs/data/model_templates/example/html_index.md` & `pylingdocs-0.0.9/src/pylingdocs/data/model_templates/example/html_index.md`

 * *Files identical despite different names*

### Comparing `pylingdocs-0.0.8/src/pylingdocs/data/model_templates/example/latex_expex.md` & `pylingdocs-0.0.9/src/pylingdocs/data/model_templates/example/latex_expex.md`

 * *Files identical despite different names*

### Comparing `pylingdocs-0.0.8/src/pylingdocs/data/model_templates/example/latex_index_expex.md` & `pylingdocs-0.0.9/src/pylingdocs/data/model_templates/example/latex_index_expex.md`

 * *Files identical despite different names*

### Comparing `pylingdocs-0.0.8/src/pylingdocs/data/model_templates/example/plain.md` & `pylingdocs-0.0.9/src/pylingdocs/data/model_templates/example/plain.md`

 * *Files identical despite different names*

### Comparing `pylingdocs-0.0.8/src/pylingdocs/data/model_templates/example/plain_index.md` & `pylingdocs-0.0.9/src/pylingdocs/data/model_templates/example/plain_index.md`

 * *Files identical despite different names*

### Comparing `pylingdocs-0.0.8/src/pylingdocs/data/model_templates/html_util.md` & `pylingdocs-0.0.9/src/pylingdocs/data/model_templates/html_util.md`

 * *Files identical despite different names*

### Comparing `pylingdocs-0.0.8/src/pylingdocs/data/project_template/cookiecutter.json` & `pylingdocs-0.0.9/src/pylingdocs/data/project_template/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `pylingdocs-0.0.8/src/pylingdocs/data/project_template/{{cookiecutter.name}}/LICENSE` & `pylingdocs-0.0.9/src/pylingdocs/data/project_template/{{cookiecutter.name}}/LICENSE`

 * *Files identical despite different names*

### Comparing `pylingdocs-0.0.8/src/pylingdocs/data/project_template/{{cookiecutter.name}}/metadata.yaml` & `pylingdocs-0.0.9/src/pylingdocs/data/project_template/{{cookiecutter.name}}/metadata.yaml`

 * *Files identical despite different names*

### Comparing `pylingdocs-0.0.8/src/pylingdocs/data/util.md` & `pylingdocs-0.0.9/src/pylingdocs/data/util.md`

 * *Files identical despite different names*

### Comparing `pylingdocs-0.0.8/src/pylingdocs/data/web/alignment.css` & `pylingdocs-0.0.9/src/pylingdocs/data/web/alignment.css`

 * *Files identical despite different names*

### Comparing `pylingdocs-0.0.8/src/pylingdocs/data/web/alignment.js` & `pylingdocs-0.0.9/src/pylingdocs/data/web/alignment.js`

 * *Files identical despite different names*

### Comparing `pylingdocs-0.0.8/src/pylingdocs/data/web/crossref.js` & `pylingdocs-0.0.9/src/pylingdocs/data/web/crossref.js`

 * *Files identical despite different names*

### Comparing `pylingdocs-0.0.8/src/pylingdocs/data/web/examples.js` & `pylingdocs-0.0.9/src/pylingdocs/data/web/examples.js`

 * *Files identical despite different names*

### Comparing `pylingdocs-0.0.8/src/pylingdocs/data/web/styling.css` & `pylingdocs-0.0.9/src/pylingdocs/data/web/styling.css`

 * *Files identical despite different names*

### Comparing `pylingdocs-0.0.8/src/pylingdocs/helpers.py` & `pylingdocs-0.0.9/src/pylingdocs/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,14 +110,19 @@
         ("&", "\\&"),
         ("~", "\\textasciitilde{}"),
     ):
         unsafe_str = unsafe_str.replace(o, r)
     return unsafe_str
 
 
+def get_prefixed_filename(structure, file_id):
+    print(file_id)
+    return structure
+
+
 def split_ref(s):
     if "[" in s:
         bibkey, pages = s.split("[")
         pages = pages.rstrip("]")
     else:
         bibkey, pages = s, None
     return bibkey, pages
@@ -179,16 +184,14 @@
 def load_content(source_dir=CONTENT_FOLDER, structure_file=STRUCTURE_FILE):
     contents = get_structure(
         prefix_mode=CONTENT_FILE_PREFIX, structure_file=structure_file
     )
     for data in contents.values():
         with open(Path(source_dir) / data["filename"], "r", encoding="utf-8") as f:
             data["content"] = f.read()
-        if "title" not in data:
-            data["title"] = "TODO MAKE THIS THE TITLE PLS"
     return contents
 
 
 def write_file(
     file_id,
     content,
     prefix_mode=CONTENT_FILE_PREFIX,
```

### Comparing `pylingdocs-0.0.8/src/pylingdocs/metadata.py` & `pylingdocs-0.0.9/src/pylingdocs/metadata.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,22 +25,29 @@
             f"Metadata file {metadata_file.resolve()} not found, please create one."
         )
         return {}
 
 
 bibtex_repl = {"location": "address"}
 bibtex_rev = {y: x for x, y in bibtex_repl.items()}
-remove_fields = []
 
 
 def _license_url(s):
     license_dic = {"CC-BY-SA-4.0": "http://creativecommons.org/licenses/by/4.0/"}
     return license_dic.get(s, "")
 
 
+def _fill_repo(md):
+    if "repository" in md:
+        if "version" in md:
+            md["url"] = md["repository"] + f"/tree/{md['version']}"
+        elif "url" not in md:
+            md["url"] = md["repository"]
+
+
 def _load_bib(metadata_file=METADATA_FILE):
     md = _read_metadata_file(metadata_file)
     entry_type = md.get("type", "article")
     with open(DATA_DIR / "bibtex_schemes.json", "r", encoding="utf-8") as f:
         bibschemes = json.loads(f.read())
     if entry_type not in bibschemes:
         log.error(
@@ -68,42 +75,32 @@
         md["authors"] = [{"family-names": "Anonymous", "given-names": "A."}]
 
     md["title"] = md.get("title", "Put your title here.")
     if "version" in md:
         md["title"] += f' (version {md["version"]})'
     else:
         md["version"] = "0.0.0"
-    if "repository" in md:
-        if "version" in md:
-            md["url"] = md["repository"] + f"/tree/{md['version']}"
-        elif "url" not in md:
-            md["url"] = md["repository"]
+    _fill_repo(md)
     bibtex_fields = {
         "author": " and ".join(author_string),
         "year": year,
         "urldate": date,
     }
     for field, value in md.items():
         if field in good_fields:
             bibtex_fields[field] = value
-    for field in remove_fields:
-        bibtex_fields[field] = md.pop(field)
     bib_data = BibliographyData(
         {bibkey: Entry(entry_type, list(bibtex_fields.items()))}
     )
     return bib_data
 
 
 def _load_metadata(metadata_file=METADATA_FILE):
     md = _read_metadata_file(metadata_file)
-    if "repository" in md:
-        if "version" in md:
-            md["url"] = md["repository"] + f"/tree/{md['version']}"
-        elif "url" not in md:
-            md["url"] = md["repository"]
+    _fill_repo(md)
     if "authors" in md:
         for author in md["authors"]:
             if "orcid" in author and "http" not in author["orcid"]:
                 author["orcid"] = ORCID_STR + author["orcid"]
     if "license" in md:
         md["license"] = _license_url(md["license"])
     return md
```

### Comparing `pylingdocs-0.0.8/src/pylingdocs/models.py` & `pylingdocs-0.0.9/src/pylingdocs/models.py`

 * *Files identical despite different names*

### Comparing `pylingdocs-0.0.8/src/pylingdocs/output.py` & `pylingdocs-0.0.9/src/pylingdocs/output.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 """Builders producing different output formats"""
 import logging
 import re
 import shutil
 import subprocess
-import sys
 import threading
 from http.server import SimpleHTTPRequestHandler
 from http.server import test
 from pathlib import Path
 from pathlib import PosixPath
 import hupper
 import pandas as pd
 import panflute
 from cookiecutter.main import cookiecutter
 from jinja2 import Environment
 from jinja2 import PackageLoader
 from jinja2.exceptions import TemplateNotFound
 from slugify import slugify
 from pylingdocs.config import BENCH
+from pylingdocs.config import CONTENT_FILE_PREFIX
 from pylingdocs.config import CONTENT_FOLDER
 from pylingdocs.config import DATA_DIR
 from pylingdocs.config import FIGURE_DIR
-from pylingdocs.config import GLOSS_ABBREVS
+from pylingdocs.config import GLOSS_FILE_ADDRESS
 from pylingdocs.config import LATEX_TOPLEVEL
 from pylingdocs.config import OUTPUT_DIR
 from pylingdocs.config import OUTPUT_TEMPLATES
 from pylingdocs.config import STRUCTURE_FILE
 from pylingdocs.helpers import _get_relative_file
 from pylingdocs.helpers import _load_cldf_dataset
-from pylingdocs.helpers import _load_structure
 from pylingdocs.helpers import decorate_gloss_string
+from pylingdocs.helpers import get_structure
 from pylingdocs.helpers import html_example_wrap
 from pylingdocs.helpers import html_gloss
 from pylingdocs.helpers import latexify_table
 from pylingdocs.helpers import load_content
 from pylingdocs.helpers import refresh_clld_db
 from pylingdocs.helpers import src
 from pylingdocs.metadata import _load_metadata
@@ -41,14 +41,15 @@
 from pylingdocs.preprocessing import MD_LINK_PATTERN
 from pylingdocs.preprocessing import postprocess
 from pylingdocs.preprocessing import preprocess
 from pylingdocs.preprocessing import render_markdown
 
 
 NUM_PRE = re.compile(r"[\d]+\ ")
+ABC_PRE = re.compile(r"[A-Z]+\ ")
 
 log = logging.getLogger(__name__)
 
 
 def blank_todo(url, **_kwargs):
     del url
     return ""
@@ -408,16 +409,17 @@
 
     @classmethod
     def table(cls, df, caption, label):
         if not caption:
             if len(df) == 0:
                 df = df.append({x: "" for x in df.columns}, ignore_index=True)
             return df.to_markdown(index=False)
+        cap = "".join(cls.replace_commands(caption))
         return (
-            f"<a id='tab:{label}'></a><div class='caption table' id='tab:{label}'>{caption}</div>\n\n"
+            f"<a id='tab:{label}'></a><div class='caption table' id='tab:{label}'>{cap}</div>\n\n"
             + df.to_markdown(index=False)
         )
 
     @classmethod
     def reference_list(cls):
         return ""
 
@@ -439,14 +441,15 @@
             "![](", "![](/static/images/"
         )  # rudely assume that all images live in the static dir
         delim = "\n# "
         parts = tent.split(delim)[1::]
         if len(parts) == 0 or OUTPUT_TEMPLATES["clld"] in ["slides", "article"]:
             # these use # as section markers, so we add a level for the html output
             tent = tent.replace("\n#", "\n##")
+            tent = f"# {metadata['title']}\n\n" + tent
             with open(my_output_dir / "content.txt", "w", encoding="utf-8") as f:
                 f.write(tent)
         else:
             tag_dic = {}
             content_dic = {}
             for (i, part) in enumerate(parts):
                 title, content = part.split("\n", 1)
@@ -640,60 +643,46 @@
                 yield content[m.start() : m.end()]
         yield content[current:]
 
 
 builders = {x.name: x for x in [PlainText, GitHub, Latex, HTML, CLLD]}
 
 
-def _iterate_structure(structure, level, depths):
-    for child_id, child_data in structure.items():
-        depths[level] += 1
-        yield child_id, level, child_data["title"], "".join(
-            [str(x) for x in depths.values()]
-        )
-        if isinstance(child_data, dict) and "parts" in child_data:
-            for x in _iterate_structure(child_data["parts"], level + 1, depths):
-                yield x
-
-
-def iterate_structure(structure):
-    for x in _iterate_structure(
-        structure["document"]["parts"], level=0, depths={0: 0, 1: 0, 2: 0, 3: 0}
-    ):
-        yield x
-
-
 def update_structure(
-    content_dir=CONTENT_FOLDER, bench_dir=BENCH, structure_file=STRUCTURE_FILE
+    content_dir=CONTENT_FOLDER,
+    bench_dir=BENCH,
+    structure_file=STRUCTURE_FILE,
+    prefix_mode=CONTENT_FILE_PREFIX,
 ):
     log.info("Updating document structure")
 
     content_files = {}
     for file in content_dir.iterdir():
         if ".md" not in file.name:
             continue
         name = re.sub(NUM_PRE, "", file.stem)
+        name = re.sub(ABC_PRE, "", name)
         content_files[name] = file
 
     bench_files = {}
-    for file in bench_dir.iterdir():
-        if ".md" not in file.name:
-            continue
-        name = re.sub(NUM_PRE, "", file.stem)
-        bench_files[name] = file
-
-    structure = _load_structure(
-        _get_relative_file(folder=content_dir, file=structure_file)
+    if Path(bench_dir).is_dir():
+        for file in bench_dir.iterdir():
+            if ".md" not in file.name:
+                continue
+            name = re.sub(NUM_PRE, "", file.stem)
+            name = re.sub(ABC_PRE, "", name)
+            bench_files[name] = file
+
+    structure = get_structure(
+        prefix_mode=prefix_mode,
+        structure_file=_get_relative_file(content_dir, structure_file),
     )
 
-    for part_id, level, title, fileno in iterate_structure(structure):
-        del level  # unused
-        del title  # unused
-        fname = f"{fileno} {part_id}.md"
-        new_path = Path(content_dir, fname)
+    for part_id, data in structure.items():
+        new_path = Path(content_dir, data["filename"])
         if part_id in content_files:
             if part_id in bench_files:
                 log.warning(f"Conflict: {part_id}. Resolve manually.")
             else:
                 if content_files[part_id] != new_path:
                     log.info(f"'{part_id}': {content_files[part_id]} > {new_path}")
                     content_files[part_id].rename(new_path)
@@ -720,32 +709,14 @@
     log.info("Compiling LaTeX document.")
     with subprocess.Popen(
         "latexmk --quiet --xelatex main.tex", shell=True, cwd=output_dir / "latex"
     ) as proc:
         del proc  # help, prospector is forcing me
 
 
-def _load_content(structure, source_dir=CONTENT_FOLDER):
-    source_dir = Path(source_dir)
-    contents = {}
-    parts = {}
-    for part_id, level, title, fileno in iterate_structure(structure):
-        del level  # unused
-        filename = f"{fileno} {part_id}.md"
-        try:
-            with open(source_dir / filename, "r", encoding="utf-8") as f:
-                content = f.read()
-        except FileNotFoundError:
-            log.error(f"File {(source_dir/filename).resolve()} does not exist.")
-            sys.exit(1)
-        contents[part_id] = content
-        parts[part_id] = title
-    return contents, parts
-
-
 class Handler(SimpleHTTPRequestHandler):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, directory=str(OUTPUT_DIR / "html"), **kwargs)
 
 
 def run_server():
     test(Handler)
@@ -758,14 +729,15 @@
     ds = _load_cldf_dataset(cldf)
     structure_file = _get_relative_file(
         folder=source_dir / CONTENT_FOLDER, file=STRUCTURE_FILE
     )
     contents = load_content(
         structure_file=structure_file, source_dir=source_dir / CONTENT_FOLDER
     )
+    kwargs["cldf"] = cldf
     kwargs["dataset"] = ds
     kwargs["source_dir"] = source_dir
     kwargs["output_dir"] = output_dir
     if refresh:
         wkwargs = kwargs.copy()
         reloader = hupper.start_reloader(
             "pylingdocs.output.run_preview", worker_kwargs=wkwargs
@@ -795,43 +767,28 @@
     output_dir.mkdir()
 
 
 def _write_file(part_id):
     log.debug(f"Writing {part_id}")
 
 
-def check_ids(source_dir, dataset, structure):
-
-    if isinstance(structure, (str, PosixPath)):
-        structure = _load_structure(source_dir / CONTENT_FOLDER / structure)
-
-    source_dir = Path(source_dir)
-    contents, parts = _load_content(structure, source_dir / CONTENT_FOLDER)
-    del parts
-
+def check_ids(contents, dataset, source_dir):
     builder = builders["plain"]
-    content = "\n\n".join(contents.values())
-    preprocessed = preprocess(content, source_dir)
-    preprocessed = builder.preprocess_commands(preprocessed)
-    running = True
-    bad_ids = []
-    while running:
-        try:
-            render_markdown(preprocessed, dataset, output_format="plain")
-        except KeyError as e:
-            bad_id = str(e).strip("'")
-            preprocessed = preprocessed.replace(bad_id, "")
-            bad_ids.append(bad_id)
-        else:
-            running = False
-    if len(bad_ids) > 0:
-        bad_ids = "\n".join(bad_ids)
-        log.error(f"""IDs missing from the dataset:\n{bad_ids}""")
-    else:
-        log.info("All good!")
+    found = False
+    for filename, x in contents.items():
+        preprocessed = preprocess(x["content"], source_dir)
+        preprocessed = builder.preprocess_commands(preprocessed)
+        for i, line in enumerate(preprocessed.split("\n")):
+            try:
+                render_markdown(line, dataset, output_format="plain")
+            except KeyError as e:
+                log.error(f"Missing ID in file {filename}, L{i+1}:\n{str(e)} in {line}")
+                found = True
+    if not found:
+        log.info("No missing IDs found.")
 
 
 def create_output(
     contents,
     source_dir,
     formats,
     dataset,
@@ -857,14 +814,22 @@
     if metadata is None:
         metadata = {}
     metadata.update({"bibfile": Path(dataset.bibpath).resolve()})
     output_dir = Path(output_dir)
     if not output_dir.is_dir():
         log.info(f"Creating output folder {output_dir.resolve()}")
         output_dir.mkdir()
+    if "cldf:" in GLOSS_FILE_ADDRESS:
+        gloss_dict = {}
+    elif (Path(source_dir) / GLOSS_FILE_ADDRESS).is_file():
+        df = pd.read_csv(Path(source_dir) / GLOSS_FILE_ADDRESS)
+        gloss_dict = dict(zip(df["ID"].str.lower(), df["Description"]))
+    else:
+        gloss_dict = {}
+
     for output_format in formats:
         for m in models:
             m.reset_cnt()
         log.info(f"Rendering format [{output_format}]")
         builder = builders[output_format]
         content = "\n\n".join([x["content"] for x in contents.values()])
         preprocessed = preprocess(content, source_dir)
@@ -884,22 +849,22 @@
         )
         preprocessed = postprocess(preprocessed, builder, source_dir)
         if builder.single_output:
             builder.write_folder(
                 output_dir,
                 content=preprocessed,
                 metadata=metadata,
-                abbrev_dict=GLOSS_ABBREVS,
+                abbrev_dict=gloss_dict,
             )
         elif builder.name == "clld":
             builder.write_folder(
                 output_dir,
                 content=preprocessed,
                 metadata=metadata,
-                abbrev_dict=GLOSS_ABBREVS,
+                abbrev_dict=gloss_dict,
             )
             # builder.create_app()
             # write_clld(preprocessed)
             # with open("clld_output.txt", "w", encoding="utf-8") as f:
             #     f.write(preprocessed)
         else:
             pass
```

### Comparing `pylingdocs-0.0.8/src/pylingdocs/preprocessing.py` & `pylingdocs-0.0.9/src/pylingdocs/preprocessing.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,37 +195,38 @@
             preprocessed = "".join(preprocess_cldfviz(md_str))
         return preprocessed
     log.error(f"Unknown data format {data_format}")
     return ""
 
 
 def load_tables(md, tables, source_dir="."):
+    def decorate_cell(x):
+        if x != "":
+            return (
+                this_table_metadata.get("pre_cell", "")
+                + x
+                + this_table_metadata.get("post_cell", "")
+            )
+        return x
+
     current = 0
     for m in MD_LINK_PATTERN.finditer(md):
         yield md[current : m.start()]
         current, key, url = get_md_pattern(m)
         if key == "table":
             table_path = source_dir / TABLE_DIR / f"{url}.csv"
             if not table_path.is_file():
                 log.error(f"Table file <{table_path.resolve()}> does not exist.")
                 sys.exit(1)
             else:
-                temp_df = pd.read_csv(table_path, keep_default_na=False)
+                temp_df = pd.read_csv(table_path, index_col=0, keep_default_na=False)
                 this_table_metadata = tables.get(url, {})
-                temp_df = temp_df.apply(
-                    lambda x: this_table_metadata.get(  # pylint: disable=cell-var-from-loop
-                        "pre_cell", ""
-                    )
-                    + x
-                    + this_table_metadata.get(  # pylint: disable=cell-var-from-loop
-                        "post_cell", ""
-                    )
-                )
+                temp_df = temp_df.applymap(decorate_cell)
                 csv_buffer = StringIO()
-                temp_df.to_csv(csv_buffer, index=False)
+                temp_df.to_csv(csv_buffer, index=True)
                 csv_buffer.seek(0)
                 yield "\nPYLINGDOCS_RAW_TABLE_START" + url + "CONTENT_START" + csv_buffer.read() + "PYLINGDOCS_RAW_TABLE_END"  # noqa: E501
         else:
             yield md[m.start() : m.end()]
     yield md[current:]
```

### Comparing `pylingdocs-0.0.8/src/pylingdocs.egg-info/PKG-INFO` & `pylingdocs-0.0.9/src/pylingdocs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylingdocs
-Version: 0.0.8
+Version: 0.0.9
 Summary: Create data-rich linguistic documents.
 Home-page: https://github.com/fmatter/pylingdocs
 Author: Florian Matter
 Author-email: florianmatter@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/fmatter/pylingdocs/issues
 Keywords: digital linguistics,CLDF
```

### Comparing `pylingdocs-0.0.8/src/pylingdocs.egg-info/SOURCES.txt` & `pylingdocs-0.0.9/src/pylingdocs.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 src/pylingdocs/cldf.py
 src/pylingdocs/cli.py
 src/pylingdocs/config.py
 src/pylingdocs/helpers.py
 src/pylingdocs/metadata.py
 src/pylingdocs/models.py
 src/pylingdocs/output.py
-src/pylingdocs/pandoc_filters.py
 src/pylingdocs/preprocessing.py
 src/pylingdocs.egg-info/PKG-INFO
 src/pylingdocs.egg-info/SOURCES.txt
 src/pylingdocs.egg-info/dependency_links.txt
 src/pylingdocs.egg-info/entry_points.txt
 src/pylingdocs.egg-info/not-zip-safe
 src/pylingdocs.egg-info/requires.txt
```

