# Comparing `tmp/python-semantic-release-8.0.0rc2.tar.gz` & `tmp/python-semantic-release-8.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-semantic-release-8.0.0rc2.tar", last modified: Wed Jun 28 08:39:57 2023, max compression
+gzip compressed data, was "python-semantic-release-8.0.0rc3.tar", last modified: Sat Jul  1 23:23:53 2023, max compression
```

## Comparing `python-semantic-release-8.0.0rc2.tar` & `python-semantic-release-8.0.0rc3.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 08:39:57.636877 python-semantic-release-8.0.0rc2/
--rw-r--r--   0 root         (0) root         (0)      230 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/AUTHORS.rst
--rw-r--r--   0 root         (0) root         (0)     1084 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      153 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3111 2023-06-28 08:39:57.636877 python-semantic-release-8.0.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2272 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/README.rst
--rw-r--r--   0 root         (0) root         (0)     4681 2023-06-28 08:39:49.000000 python-semantic-release-8.0.0rc2/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 08:39:57.624876 python-semantic-release-8.0.0rc2/python_semantic_release.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3111 2023-06-28 08:39:57.000000 python-semantic-release-8.0.0rc2/python_semantic_release.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4221 2023-06-28 08:39:57.000000 python-semantic-release-8.0.0rc2/python_semantic_release.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 08:39:57.000000 python-semantic-release-8.0.0rc2/python_semantic_release.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       95 2023-06-28 08:39:57.000000 python-semantic-release-8.0.0rc2/python_semantic_release.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      598 2023-06-28 08:39:57.000000 python-semantic-release-8.0.0rc2/python_semantic_release.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-28 08:39:57.000000 python-semantic-release-8.0.0rc2/python_semantic_release.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 08:39:57.624876 python-semantic-release-8.0.0rc2/semantic_release/
--rw-r--r--   0 root         (0) root         (0)     1090 2023-06-28 08:39:49.000000 python-semantic-release-8.0.0rc2/semantic_release/__init__.py
--rw-r--r--   0 root         (0) root         (0)      106 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/semantic_release/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 08:39:57.624876 python-semantic-release-8.0.0rc2/semantic_release/changelog/
--rw-r--r--   0 root         (0) root         (0)      361 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/semantic_release/changelog/__init__.py
--rw-r--r--   0 root         (0) root         (0)      941 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/semantic_release/changelog/context.py
--rw-r--r--   0 root         (0) root         (0)     6470 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/semantic_release/changelog/release_history.py
--rw-r--r--   0 root         (0) root         (0)     4328 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/semantic_release/changelog/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 08:39:57.624876 python-semantic-release-8.0.0rc2/semantic_release/cli/
--rw-r--r--   0 root         (0) root         (0)      451 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/semantic_release/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 08:39:57.628877 python-semantic-release-8.0.0rc2/semantic_release/cli/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/semantic_release/cli/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3246 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/semantic_release/cli/commands/changelog.py
--rw-r--r--   0 root         (0) root         (0)     1448 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/semantic_release/cli/commands/generate_config.py
--rw-r--r--   0 root         (0) root         (0)     4978 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/semantic_release/cli/commands/main.py
--rw-r--r--   0 root         (0) root         (0)     1298 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/semantic_release/cli/commands/publish.py
--rw-r--r--   0 root         (0) root         (0)    18649 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/semantic_release/cli/commands/version.py
--rw-r--r--   0 root         (0) root         (0)      929 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/semantic_release/cli/common.py
--rw-r--r--   0 root         (0) root         (0)    13706 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/semantic_release/cli/config.py
--rw-r--r--   0 root         (0) root         (0)       39 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/semantic_release/cli/const.py
--rw-r--r--   0 root         (0) root         (0)     2105 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/semantic_release/cli/github_actions_output.py
--rw-r--r--   0 root         (0) root         (0)     2875 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/semantic_release/cli/masking_filter.py
--rw-r--r--   0 root         (0) root         (0)      935 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/semantic_release/cli/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 08:39:57.628877 python-semantic-release-8.0.0rc2/semantic_release/commit_parser/
--rw-r--r--   0 root         (0) root         (0)      884 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/semantic_release/commit_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2569 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/semantic_release/commit_parser/_base.py
--rw-r--r--   0 root         (0) root         (0)     4364 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/semantic_release/commit_parser/angular.py
--rw-r--r--   0 root         (0) root         (0)     3288 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/semantic_release/commit_parser/emoji.py
--rw-r--r--   0 root         (0) root         (0)     5713 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/semantic_release/commit_parser/scipy.py
--rw-r--r--   0 root         (0) root         (0)     3193 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/semantic_release/commit_parser/tag.py
--rw-r--r--   0 root         (0) root         (0)     1456 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/semantic_release/commit_parser/token.py
--rw-r--r--   0 root         (0) root         (0)      529 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/semantic_release/commit_parser/util.py
--rw-r--r--   0 root         (0) root         (0)      831 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/semantic_release/const.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 08:39:57.620876 python-semantic-release-8.0.0rc2/semantic_release/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 08:39:57.628877 python-semantic-release-8.0.0rc2/semantic_release/data/templates/
--rw-r--r--   0 root         (0) root         (0)     1059 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/semantic_release/data/templates/CHANGELOG.md.j2
--rw-r--r--   0 root         (0) root         (0)      465 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/semantic_release/data/templates/release_notes.md.j2
--rw-r--r--   0 root         (0) root         (0)     1020 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/semantic_release/enums.py
--rw-r--r--   0 root         (0) root         (0)      674 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/semantic_release/errors.py
--rw-r--r--   0 root         (0) root         (0)     4088 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/semantic_release/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 08:39:57.628877 python-semantic-release-8.0.0rc2/semantic_release/hvcs/
--rw-r--r--   0 root         (0) root         (0)      300 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/semantic_release/hvcs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5579 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/semantic_release/hvcs/_base.py
--rw-r--r--   0 root         (0) root         (0)     8285 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/semantic_release/hvcs/gitea.py
--rw-r--r--   0 root         (0) root         (0)    10154 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/semantic_release/hvcs/github.py
--rw-r--r--   0 root         (0) root         (0)     5029 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/semantic_release/hvcs/gitlab.py
--rw-r--r--   0 root         (0) root         (0)      681 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/semantic_release/hvcs/token_auth.py
--rw-r--r--   0 root         (0) root         (0)     2774 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/semantic_release/hvcs/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 08:39:57.628877 python-semantic-release-8.0.0rc2/semantic_release/version/
--rw-r--r--   0 root         (0) root         (0)      339 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/semantic_release/version/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14177 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/semantic_release/version/algorithm.py
--rw-r--r--   0 root         (0) root         (0)     7267 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/semantic_release/version/declaration.py
--rw-r--r--   0 root         (0) root         (0)     3103 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/semantic_release/version/translator.py
--rw-r--r--   0 root         (0) root         (0)    14060 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/semantic_release/version/version.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-28 08:39:57.636877 python-semantic-release-8.0.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      466 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 08:39:57.620876 python-semantic-release-8.0.0rc2/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 08:39:57.632877 python-semantic-release-8.0.0rc2/tests/command_line/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/command_line/__init__.py
--rw-r--r--   0 root         (0) root         (0)      190 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/command_line/conftest.py
--rw-r--r--   0 root         (0) root         (0)     5707 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/command_line/test_changelog.py
--rw-r--r--   0 root         (0) root         (0)     1320 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/command_line/test_generate_config.py
--rw-r--r--   0 root         (0) root         (0)      641 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/command_line/test_help.py
--rw-r--r--   0 root         (0) root         (0)     1167 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/command_line/test_main.py
--rw-r--r--   0 root         (0) root         (0)     1430 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/command_line/test_publish.py
--rw-r--r--   0 root         (0) root         (0)    20288 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/command_line/test_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 08:39:57.632877 python-semantic-release-8.0.0rc2/tests/fixtures/
--rw-r--r--   0 root         (0) root         (0)      106 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/fixtures/__init__.py
--rw-r--r--   0 root         (0) root         (0)      906 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/fixtures/commit_parsers.py
--rw-r--r--   0 root         (0) root         (0)     2235 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/fixtures/example_project.py
--rw-r--r--   0 root         (0) root         (0)    45283 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/fixtures/git_repo.py
--rw-r--r--   0 root         (0) root         (0)     4424 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/fixtures/scipy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 08:39:57.632877 python-semantic-release-8.0.0rc2/tests/scenario/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/scenario/__init__.py
--rw-r--r--   0 root         (0) root         (0)    46838 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/scenario/test_next_version.py
--rw-r--r--   0 root         (0) root         (0)    12186 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/scenario/test_release_history.py
--rw-r--r--   0 root         (0) root         (0)     3513 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/scenario/test_template_render.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 08:39:57.632877 python-semantic-release-8.0.0rc2/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 08:39:57.632877 python-semantic-release-8.0.0rc2/tests/unit/semantic_release/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/unit/semantic_release/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 08:39:57.632877 python-semantic-release-8.0.0rc2/tests/unit/semantic_release/changelog/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/unit/semantic_release/changelog/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5005 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/unit/semantic_release/changelog/test_changelog_context.py
--rw-r--r--   0 root         (0) root         (0)     2540 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/unit/semantic_release/changelog/test_default_changelog.py
--rw-r--r--   0 root         (0) root         (0)     1747 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/unit/semantic_release/changelog/test_release_notes.py
--rw-r--r--   0 root         (0) root         (0)     2102 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/unit/semantic_release/changelog/test_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 08:39:57.632877 python-semantic-release-8.0.0rc2/tests/unit/semantic_release/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/unit/semantic_release/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1709 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/unit/semantic_release/cli/test_config.py
--rw-r--r--   0 root         (0) root         (0)     1784 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/unit/semantic_release/cli/test_github_actions_output.py
--rw-r--r--   0 root         (0) root         (0)     5768 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/unit/semantic_release/cli/test_masking_filter.py
--rw-r--r--   0 root         (0) root         (0)      799 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/unit/semantic_release/cli/test_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 08:39:57.636877 python-semantic-release-8.0.0rc2/tests/unit/semantic_release/commit_parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/unit/semantic_release/commit_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)      140 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/unit/semantic_release/commit_parser/helper.py
--rw-r--r--   0 root         (0) root         (0)     5969 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/unit/semantic_release/commit_parser/test_angular.py
--rw-r--r--   0 root         (0) root         (0)     2487 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/unit/semantic_release/commit_parser/test_emoji.py
--rw-r--r--   0 root         (0) root         (0)      500 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/unit/semantic_release/commit_parser/test_scipy.py
--rw-r--r--   0 root         (0) root         (0)     2173 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/unit/semantic_release/commit_parser/test_tag.py
--rw-r--r--   0 root         (0) root         (0)      648 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/unit/semantic_release/commit_parser/test_token.py
--rw-r--r--   0 root         (0) root         (0)      442 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/unit/semantic_release/commit_parser/test_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 08:39:57.636877 python-semantic-release-8.0.0rc2/tests/unit/semantic_release/hvcs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/unit/semantic_release/hvcs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1349 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/unit/semantic_release/hvcs/test__base.py
--rw-r--r--   0 root         (0) root         (0)    22874 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/unit/semantic_release/hvcs/test_gitea.py
--rw-r--r--   0 root         (0) root         (0)    24334 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/unit/semantic_release/hvcs/test_github.py
--rw-r--r--   0 root         (0) root         (0)    10021 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/unit/semantic_release/hvcs/test_gitlab.py
--rw-r--r--   0 root         (0) root         (0)      965 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/unit/semantic_release/hvcs/test_token_auth.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/unit/semantic_release/hvcs/test_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 08:39:57.636877 python-semantic-release-8.0.0rc2/tests/unit/semantic_release/version/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/unit/semantic_release/version/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7319 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/unit/semantic_release/version/test_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     3715 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/unit/semantic_release/version/test_declaration.py
--rw-r--r--   0 root         (0) root         (0)     2996 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/unit/semantic_release/version/test_translator.py
--rw-r--r--   0 root         (0) root         (0)     9640 2023-06-28 08:38:57.000000 python-semantic-release-8.0.0rc2/tests/unit/semantic_release/version/test_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:23:53.753641 python-semantic-release-8.0.0rc3/
+-rw-r--r--   0 root         (0) root         (0)      230 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/AUTHORS.rst
+-rw-r--r--   0 root         (0) root         (0)     1084 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      153 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3111 2023-07-01 23:23:53.753641 python-semantic-release-8.0.0rc3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2272 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/README.rst
+-rw-r--r--   0 root         (0) root         (0)     4681 2023-07-01 23:23:45.000000 python-semantic-release-8.0.0rc3/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:23:53.733640 python-semantic-release-8.0.0rc3/python_semantic_release.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3111 2023-07-01 23:23:53.000000 python-semantic-release-8.0.0rc3/python_semantic_release.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4221 2023-07-01 23:23:53.000000 python-semantic-release-8.0.0rc3/python_semantic_release.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-01 23:23:53.000000 python-semantic-release-8.0.0rc3/python_semantic_release.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       95 2023-07-01 23:23:53.000000 python-semantic-release-8.0.0rc3/python_semantic_release.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      598 2023-07-01 23:23:53.000000 python-semantic-release-8.0.0rc3/python_semantic_release.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-01 23:23:53.000000 python-semantic-release-8.0.0rc3/python_semantic_release.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:23:53.733640 python-semantic-release-8.0.0rc3/semantic_release/
+-rw-r--r--   0 root         (0) root         (0)     1090 2023-07-01 23:23:45.000000 python-semantic-release-8.0.0rc3/semantic_release/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      106 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:23:53.733640 python-semantic-release-8.0.0rc3/semantic_release/changelog/
+-rw-r--r--   0 root         (0) root         (0)      361 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/changelog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      941 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/changelog/context.py
+-rw-r--r--   0 root         (0) root         (0)     6470 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/changelog/release_history.py
+-rw-r--r--   0 root         (0) root         (0)     4328 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/changelog/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:23:53.737640 python-semantic-release-8.0.0rc3/semantic_release/cli/
+-rw-r--r--   0 root         (0) root         (0)      451 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:23:53.737640 python-semantic-release-8.0.0rc3/semantic_release/cli/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/cli/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3246 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/cli/commands/changelog.py
+-rw-r--r--   0 root         (0) root         (0)     1448 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/cli/commands/generate_config.py
+-rw-r--r--   0 root         (0) root         (0)     4978 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/cli/commands/main.py
+-rw-r--r--   0 root         (0) root         (0)     1298 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/cli/commands/publish.py
+-rw-r--r--   0 root         (0) root         (0)    18649 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/cli/commands/version.py
+-rw-r--r--   0 root         (0) root         (0)      929 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/cli/common.py
+-rw-r--r--   0 root         (0) root         (0)    13706 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/cli/config.py
+-rw-r--r--   0 root         (0) root         (0)       39 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/cli/const.py
+-rw-r--r--   0 root         (0) root         (0)     2105 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/cli/github_actions_output.py
+-rw-r--r--   0 root         (0) root         (0)     2875 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/cli/masking_filter.py
+-rw-r--r--   0 root         (0) root         (0)      935 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/cli/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:23:53.741640 python-semantic-release-8.0.0rc3/semantic_release/commit_parser/
+-rw-r--r--   0 root         (0) root         (0)      884 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/commit_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2569 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/commit_parser/_base.py
+-rw-r--r--   0 root         (0) root         (0)     4364 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/commit_parser/angular.py
+-rw-r--r--   0 root         (0) root         (0)     3288 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/commit_parser/emoji.py
+-rw-r--r--   0 root         (0) root         (0)     5713 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/commit_parser/scipy.py
+-rw-r--r--   0 root         (0) root         (0)     3193 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/commit_parser/tag.py
+-rw-r--r--   0 root         (0) root         (0)     1456 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/commit_parser/token.py
+-rw-r--r--   0 root         (0) root         (0)      529 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/commit_parser/util.py
+-rw-r--r--   0 root         (0) root         (0)      831 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/const.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:23:53.729639 python-semantic-release-8.0.0rc3/semantic_release/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:23:53.741640 python-semantic-release-8.0.0rc3/semantic_release/data/templates/
+-rw-r--r--   0 root         (0) root         (0)     1059 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/data/templates/CHANGELOG.md.j2
+-rw-r--r--   0 root         (0) root         (0)      465 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/data/templates/release_notes.md.j2
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/enums.py
+-rw-r--r--   0 root         (0) root         (0)      674 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/errors.py
+-rw-r--r--   0 root         (0) root         (0)     4088 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:23:53.741640 python-semantic-release-8.0.0rc3/semantic_release/hvcs/
+-rw-r--r--   0 root         (0) root         (0)      300 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/hvcs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5595 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/hvcs/_base.py
+-rw-r--r--   0 root         (0) root         (0)     8285 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/hvcs/gitea.py
+-rw-r--r--   0 root         (0) root         (0)    10146 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/hvcs/github.py
+-rw-r--r--   0 root         (0) root         (0)     5898 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/hvcs/gitlab.py
+-rw-r--r--   0 root         (0) root         (0)      681 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/hvcs/token_auth.py
+-rw-r--r--   0 root         (0) root         (0)     2774 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/hvcs/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:23:53.741640 python-semantic-release-8.0.0rc3/semantic_release/version/
+-rw-r--r--   0 root         (0) root         (0)      339 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/version/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14177 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/version/algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     7267 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/version/declaration.py
+-rw-r--r--   0 root         (0) root         (0)     3103 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/version/translator.py
+-rw-r--r--   0 root         (0) root         (0)    14060 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/semantic_release/version/version.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-01 23:23:53.753641 python-semantic-release-8.0.0rc3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      466 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:23:53.729639 python-semantic-release-8.0.0rc3/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:23:53.745640 python-semantic-release-8.0.0rc3/tests/command_line/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/command_line/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      190 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/command_line/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     5707 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/command_line/test_changelog.py
+-rw-r--r--   0 root         (0) root         (0)     1320 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/command_line/test_generate_config.py
+-rw-r--r--   0 root         (0) root         (0)      641 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/command_line/test_help.py
+-rw-r--r--   0 root         (0) root         (0)     1167 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/command_line/test_main.py
+-rw-r--r--   0 root         (0) root         (0)     1430 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/command_line/test_publish.py
+-rw-r--r--   0 root         (0) root         (0)    20288 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/command_line/test_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:23:53.745640 python-semantic-release-8.0.0rc3/tests/fixtures/
+-rw-r--r--   0 root         (0) root         (0)      106 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/fixtures/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      906 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/fixtures/commit_parsers.py
+-rw-r--r--   0 root         (0) root         (0)     2235 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/fixtures/example_project.py
+-rw-r--r--   0 root         (0) root         (0)    45283 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/fixtures/git_repo.py
+-rw-r--r--   0 root         (0) root         (0)     4424 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/fixtures/scipy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:23:53.745640 python-semantic-release-8.0.0rc3/tests/scenario/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/scenario/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    46838 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/scenario/test_next_version.py
+-rw-r--r--   0 root         (0) root         (0)    12186 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/scenario/test_release_history.py
+-rw-r--r--   0 root         (0) root         (0)     3513 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/scenario/test_template_render.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:23:53.745640 python-semantic-release-8.0.0rc3/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:23:53.749641 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:23:53.749641 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/changelog/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/changelog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5005 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/changelog/test_changelog_context.py
+-rw-r--r--   0 root         (0) root         (0)     2540 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/changelog/test_default_changelog.py
+-rw-r--r--   0 root         (0) root         (0)     1747 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/changelog/test_release_notes.py
+-rw-r--r--   0 root         (0) root         (0)     2102 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/changelog/test_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:23:53.749641 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/cli/test_config.py
+-rw-r--r--   0 root         (0) root         (0)     1784 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/cli/test_github_actions_output.py
+-rw-r--r--   0 root         (0) root         (0)     5768 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/cli/test_masking_filter.py
+-rw-r--r--   0 root         (0) root         (0)      799 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/cli/test_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:23:53.753641 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/commit_parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/commit_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      140 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/commit_parser/helper.py
+-rw-r--r--   0 root         (0) root         (0)     5969 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/commit_parser/test_angular.py
+-rw-r--r--   0 root         (0) root         (0)     2487 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/commit_parser/test_emoji.py
+-rw-r--r--   0 root         (0) root         (0)      500 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/commit_parser/test_scipy.py
+-rw-r--r--   0 root         (0) root         (0)     2173 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/commit_parser/test_tag.py
+-rw-r--r--   0 root         (0) root         (0)      648 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/commit_parser/test_token.py
+-rw-r--r--   0 root         (0) root         (0)      442 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/commit_parser/test_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:23:53.753641 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/hvcs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/hvcs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1349 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/hvcs/test__base.py
+-rw-r--r--   0 root         (0) root         (0)    22533 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/hvcs/test_gitea.py
+-rw-r--r--   0 root         (0) root         (0)    23987 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/hvcs/test_github.py
+-rw-r--r--   0 root         (0) root         (0)    13407 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/hvcs/test_gitlab.py
+-rw-r--r--   0 root         (0) root         (0)      965 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/hvcs/test_token_auth.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/hvcs/test_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:23:53.753641 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/version/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/version/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7319 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/version/test_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     3715 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/version/test_declaration.py
+-rw-r--r--   0 root         (0) root         (0)     2996 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/version/test_translator.py
+-rw-r--r--   0 root         (0) root         (0)     9640 2023-07-01 23:22:54.000000 python-semantic-release-8.0.0rc3/tests/unit/semantic_release/version/test_version.py
```

### Comparing `python-semantic-release-8.0.0rc2/LICENSE` & `python-semantic-release-8.0.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/PKG-INFO` & `python-semantic-release-8.0.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-semantic-release
-Version: 8.0.0rc2
+Version: 8.0.0rc3
 Summary: Automatic Semantic Versioning for Python projects
 Author-email: Rolf Erik Lekang <me@rolflekang.com>
 License: MIT
 Project-URL: Project Url, http://github.com/python-semantic-release/python-semantic-release
 Project-URL: Homepage, https://python-semantic-release.readthedocs.io
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `python-semantic-release-8.0.0rc2/README.rst` & `python-semantic-release-8.0.0rc3/README.rst`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/pyproject.toml` & `python-semantic-release-8.0.0rc3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # and https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-semantic-release"
-version = "8.0.0-rc.2"
+version = "8.0.0-rc.3"
 description = "Automatic Semantic Versioning for Python projects"
 requires-python = ">=3.7"
 license = { text = "MIT" }
 classifiers = [
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.7",
@@ -41,15 +41,15 @@
 
 [project.urls]
 "Project Url" = "http://github.com/python-semantic-release/python-semantic-release"
 Homepage = "https://python-semantic-release.readthedocs.io"
 
 [project.optional-dependencies]
 docs = [
-  "Sphinx==5.2.3",
+  "Sphinx<=8.0.0",
   "sphinxcontrib-apidoc==0.3.0",
   "sphinx-autobuild==2021.03.14",
   "furo>=2023.5.20",
 ]
 test = [
   "coverage[toml]>=6,<7",
   "pytest>=7,<8",
```

### Comparing `python-semantic-release-8.0.0rc2/python_semantic_release.egg-info/PKG-INFO` & `python-semantic-release-8.0.0rc3/python_semantic_release.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-semantic-release
-Version: 8.0.0rc2
+Version: 8.0.0rc3
 Summary: Automatic Semantic Versioning for Python projects
 Author-email: Rolf Erik Lekang <me@rolflekang.com>
 License: MIT
 Project-URL: Project Url, http://github.com/python-semantic-release/python-semantic-release
 Project-URL: Homepage, https://python-semantic-release.readthedocs.io
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `python-semantic-release-8.0.0rc2/python_semantic_release.egg-info/SOURCES.txt` & `python-semantic-release-8.0.0rc3/python_semantic_release.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/python_semantic_release.egg-info/requires.txt` & `python-semantic-release-8.0.0rc3/python_semantic_release.egg-info/requires.txt`

 * *Files 24% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 [dev]
 tox
 isort
 black
 
 [docs]
-Sphinx==5.2.3
+Sphinx<=8.0.0
 sphinxcontrib-apidoc==0.3.0
 sphinx-autobuild==2021.03.14
 furo>=2023.5.20
 
 [mypy]
 mypy
 types-requests
```

### Comparing `python-semantic-release-8.0.0rc2/semantic_release/__init__.py` & `python-semantic-release-8.0.0rc3/semantic_release/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from semantic_release.version import (
     Version as Version,
     VersionTranslator as VersionTranslator,
     next_version as next_version,
     tags_and_versions as tags_and_versions,
 )
 
-__version__ = "8.0.0-rc.2"
+__version__ = "8.0.0-rc.3"
 
 
 def setup_hook(argv: list[str]) -> None:
     """
     A hook to be used in setup.py to enable `python setup.py publish`.
 
     :param argv: sys.argv
```

### Comparing `python-semantic-release-8.0.0rc2/semantic_release/changelog/context.py` & `python-semantic-release-8.0.0rc3/semantic_release/changelog/context.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/semantic_release/changelog/release_history.py` & `python-semantic-release-8.0.0rc3/semantic_release/changelog/release_history.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/semantic_release/changelog/template.py` & `python-semantic-release-8.0.0rc3/semantic_release/changelog/template.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/semantic_release/cli/commands/changelog.py` & `python-semantic-release-8.0.0rc3/semantic_release/cli/commands/changelog.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/semantic_release/cli/commands/generate_config.py` & `python-semantic-release-8.0.0rc3/semantic_release/cli/commands/generate_config.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/semantic_release/cli/commands/main.py` & `python-semantic-release-8.0.0rc3/semantic_release/cli/commands/main.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/semantic_release/cli/commands/publish.py` & `python-semantic-release-8.0.0rc3/semantic_release/cli/commands/publish.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/semantic_release/cli/commands/version.py` & `python-semantic-release-8.0.0rc3/semantic_release/cli/commands/version.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/semantic_release/cli/common.py` & `python-semantic-release-8.0.0rc3/semantic_release/cli/common.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/semantic_release/cli/config.py` & `python-semantic-release-8.0.0rc3/semantic_release/cli/config.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/semantic_release/cli/github_actions_output.py` & `python-semantic-release-8.0.0rc3/semantic_release/cli/github_actions_output.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/semantic_release/cli/masking_filter.py` & `python-semantic-release-8.0.0rc3/semantic_release/cli/masking_filter.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/semantic_release/cli/util.py` & `python-semantic-release-8.0.0rc3/semantic_release/cli/util.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/semantic_release/commit_parser/__init__.py` & `python-semantic-release-8.0.0rc3/semantic_release/commit_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/semantic_release/commit_parser/_base.py` & `python-semantic-release-8.0.0rc3/semantic_release/commit_parser/_base.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/semantic_release/commit_parser/angular.py` & `python-semantic-release-8.0.0rc3/semantic_release/commit_parser/angular.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/semantic_release/commit_parser/emoji.py` & `python-semantic-release-8.0.0rc3/semantic_release/commit_parser/emoji.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/semantic_release/commit_parser/scipy.py` & `python-semantic-release-8.0.0rc3/semantic_release/commit_parser/scipy.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/semantic_release/commit_parser/tag.py` & `python-semantic-release-8.0.0rc3/semantic_release/commit_parser/tag.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/semantic_release/commit_parser/token.py` & `python-semantic-release-8.0.0rc3/semantic_release/commit_parser/token.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/semantic_release/commit_parser/util.py` & `python-semantic-release-8.0.0rc3/semantic_release/commit_parser/util.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/semantic_release/const.py` & `python-semantic-release-8.0.0rc3/semantic_release/const.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/semantic_release/data/templates/CHANGELOG.md.j2` & `python-semantic-release-8.0.0rc3/semantic_release/data/templates/CHANGELOG.md.j2`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/semantic_release/enums.py` & `python-semantic-release-8.0.0rc3/semantic_release/enums.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/semantic_release/errors.py` & `python-semantic-release-8.0.0rc3/semantic_release/errors.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/semantic_release/helpers.py` & `python-semantic-release-8.0.0rc3/semantic_release/helpers.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/semantic_release/hvcs/_base.py` & `python-semantic-release-8.0.0rc3/semantic_release/hvcs/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,39 +85,39 @@
         supports such uploads
         """
         _not_supported(self, "upload_dists")
         return 0
 
     def create_release(
         self, tag: str, release_notes: str, prerelease: bool = False
-    ) -> int:
+    ) -> int | str:
         """
         Create a release in a remote VCS, if supported
         """
         _not_supported(self, "create_release")
         return -1
 
     def get_release_id_by_tag(self, tag: str) -> int | None:
         """
         Given a Git tag, return the ID (as the remote VCS defines it) of a corrsponding
         release in the remove VCS, if supported
         """
         _not_supported(self, "get_release_id_by_tag")
         return None
 
-    def edit_release_notes(self, release_id: int, changelog: str) -> int:
+    def edit_release_notes(self, release_id: int, release_notes: str) -> int:
         """
         Edit the changelog associated with a release, if supported
         """
         _not_supported(self, "edit_release_notes")
         return -1
 
     def create_or_update_release(
         self, tag: str, release_notes: str, prerelease: bool = False
-    ) -> int:
+    ) -> int | str:
         """
         Create or update a release for the given tag in a remote VCS, attaching the
         given changelog, if supported
         """
         _not_supported(self, "create_or_update_release")
         return -1
```

### Comparing `python-semantic-release-8.0.0rc2/semantic_release/hvcs/gitea.py` & `python-semantic-release-8.0.0rc3/semantic_release/hvcs/gitea.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/semantic_release/hvcs/github.py` & `python-semantic-release-8.0.0rc3/semantic_release/hvcs/github.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         self, tag: str, release_notes: str, prerelease: bool = False
     ) -> int:
         """Create a new release
         https://docs.github.com/rest/reference/repos#create-a-release
         :param tag: Tag to create release for
         :param release_notes: The release notes for this version
         :param prerelease: Whether or not this release should be created as a prerelease
-        :return: Whether the request succeeded
+        :return: the ID of the release
         """
         log.info("Creating release for tag %s", tag)
         resp = self.session.post(
             f"{self.api_url}/repos/{self.owner}/{self.repo_name}/releases",
             json={
                 "tag_name": tag,
                 "name": tag,
```

### Comparing `python-semantic-release-8.0.0rc2/semantic_release/hvcs/token_auth.py` & `python-semantic-release-8.0.0rc3/semantic_release/hvcs/token_auth.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/semantic_release/hvcs/util.py` & `python-semantic-release-8.0.0rc3/semantic_release/hvcs/util.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/semantic_release/version/algorithm.py` & `python-semantic-release-8.0.0rc3/semantic_release/version/algorithm.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/semantic_release/version/declaration.py` & `python-semantic-release-8.0.0rc3/semantic_release/version/declaration.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/semantic_release/version/translator.py` & `python-semantic-release-8.0.0rc3/semantic_release/version/translator.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/semantic_release/version/version.py` & `python-semantic-release-8.0.0rc3/semantic_release/version/version.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/tests/command_line/test_changelog.py` & `python-semantic-release-8.0.0rc3/tests/command_line/test_changelog.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/tests/command_line/test_generate_config.py` & `python-semantic-release-8.0.0rc3/tests/command_line/test_generate_config.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/tests/command_line/test_help.py` & `python-semantic-release-8.0.0rc3/tests/command_line/test_help.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/tests/command_line/test_main.py` & `python-semantic-release-8.0.0rc3/tests/command_line/test_main.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/tests/command_line/test_publish.py` & `python-semantic-release-8.0.0rc3/tests/command_line/test_publish.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/tests/command_line/test_version.py` & `python-semantic-release-8.0.0rc3/tests/command_line/test_version.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/tests/fixtures/commit_parsers.py` & `python-semantic-release-8.0.0rc3/tests/fixtures/commit_parsers.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/tests/fixtures/example_project.py` & `python-semantic-release-8.0.0rc3/tests/fixtures/example_project.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/tests/fixtures/git_repo.py` & `python-semantic-release-8.0.0rc3/tests/fixtures/git_repo.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/tests/fixtures/scipy.py` & `python-semantic-release-8.0.0rc3/tests/fixtures/scipy.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/tests/scenario/test_next_version.py` & `python-semantic-release-8.0.0rc3/tests/scenario/test_next_version.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/tests/scenario/test_release_history.py` & `python-semantic-release-8.0.0rc3/tests/scenario/test_release_history.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/tests/scenario/test_template_render.py` & `python-semantic-release-8.0.0rc3/tests/scenario/test_template_render.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/tests/unit/semantic_release/changelog/test_changelog_context.py` & `python-semantic-release-8.0.0rc3/tests/unit/semantic_release/changelog/test_changelog_context.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/tests/unit/semantic_release/changelog/test_default_changelog.py` & `python-semantic-release-8.0.0rc3/tests/unit/semantic_release/changelog/test_default_changelog.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/tests/unit/semantic_release/changelog/test_release_notes.py` & `python-semantic-release-8.0.0rc3/tests/unit/semantic_release/changelog/test_release_notes.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/tests/unit/semantic_release/changelog/test_template.py` & `python-semantic-release-8.0.0rc3/tests/unit/semantic_release/changelog/test_template.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/tests/unit/semantic_release/cli/test_config.py` & `python-semantic-release-8.0.0rc3/tests/unit/semantic_release/cli/test_config.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/tests/unit/semantic_release/cli/test_github_actions_output.py` & `python-semantic-release-8.0.0rc3/tests/unit/semantic_release/cli/test_github_actions_output.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/tests/unit/semantic_release/cli/test_masking_filter.py` & `python-semantic-release-8.0.0rc3/tests/unit/semantic_release/cli/test_masking_filter.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/tests/unit/semantic_release/cli/test_version.py` & `python-semantic-release-8.0.0rc3/tests/unit/semantic_release/cli/test_version.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/tests/unit/semantic_release/commit_parser/test_angular.py` & `python-semantic-release-8.0.0rc3/tests/unit/semantic_release/commit_parser/test_angular.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/tests/unit/semantic_release/commit_parser/test_emoji.py` & `python-semantic-release-8.0.0rc3/tests/unit/semantic_release/commit_parser/test_emoji.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/tests/unit/semantic_release/commit_parser/test_tag.py` & `python-semantic-release-8.0.0rc3/tests/unit/semantic_release/commit_parser/test_tag.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/tests/unit/semantic_release/commit_parser/test_token.py` & `python-semantic-release-8.0.0rc3/tests/unit/semantic_release/commit_parser/test_token.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/tests/unit/semantic_release/hvcs/test__base.py` & `python-semantic-release-8.0.0rc3/tests/unit/semantic_release/hvcs/test__base.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/tests/unit/semantic_release/hvcs/test_gitea.py` & `python-semantic-release-8.0.0rc3/tests/unit/semantic_release/hvcs/test_gitea.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import pytest
 import requests_mock
 from requests import HTTPError, Response, Session
 
 from semantic_release.hvcs.gitea import Gitea
 from semantic_release.hvcs.token_auth import TokenAuth
 
-from tests.const import EXAMPLE_REPO_NAME, EXAMPLE_REPO_OWNER
+from tests.const import EXAMPLE_REPO_NAME, EXAMPLE_REPO_OWNER, RELEASE_NOTES
 from tests.util import netrc_file
 
 
 @pytest.fixture
 def default_gitea_client():
     remote_url = f"git@gitea.com:{EXAMPLE_REPO_OWNER}/{EXAMPLE_REPO_NAME}.git"
     yield Gitea(remote_url=remote_url)
@@ -195,24 +195,23 @@
 @pytest.mark.parametrize("status_code", (201,))
 @pytest.mark.parametrize("mock_release_id", range(3))
 @pytest.mark.parametrize("prerelease", (True, False))
 def test_create_release_succeeds(
     default_gitea_client, status_code, prerelease, mock_release_id
 ):
     tag = "v1.0.0"
-    release_notes = "#TODO: Release Notes"
     with requests_mock.Mocker(session=default_gitea_client.session) as m:
         m.register_uri(
             "POST",
             gitea_api_matcher,
             json={"id": mock_release_id},
             status_code=status_code,
         )
         assert (
-            default_gitea_client.create_release(tag, release_notes, prerelease)
+            default_gitea_client.create_release(tag, RELEASE_NOTES, prerelease)
             == mock_release_id
         )
         assert m.called
         assert len(m.request_history) == 1
         assert m.last_request.method == "POST"
         assert (
             m.last_request.url
@@ -221,38 +220,37 @@
                 owner=default_gitea_client.owner,
                 repo_name=default_gitea_client.repo_name,
             )
         )
         assert m.last_request.json() == {
             "tag_name": tag,
             "name": tag,
-            "body": release_notes,
+            "body": RELEASE_NOTES,
             "draft": False,
             "prerelease": prerelease,
         }
 
 
 @pytest.mark.parametrize("status_code", (400, 409))
 @pytest.mark.parametrize("mock_release_id", range(3))
 @pytest.mark.parametrize("prerelease", (True, False))
 def test_create_release_fails(
     default_gitea_client, status_code, prerelease, mock_release_id
 ):
     tag = "v1.0.0"
-    release_notes = "#TODO: Release Notes"
     with requests_mock.Mocker(session=default_gitea_client.session) as m:
         m.register_uri(
             "POST",
             gitea_api_matcher,
             json={"id": mock_release_id},
             status_code=status_code,
         )
 
         with pytest.raises(HTTPError):
-            default_gitea_client.create_release(tag, release_notes, prerelease)
+            default_gitea_client.create_release(tag, RELEASE_NOTES, prerelease)
 
         assert m.called
         assert len(m.request_history) == 1
         assert m.last_request.method == "POST"
         assert (
             m.last_request.url
             == "{api_url}/repos/{owner}/{repo_name}/releases".format(
@@ -260,34 +258,33 @@
                 owner=default_gitea_client.owner,
                 repo_name=default_gitea_client.repo_name,
             )
         )
         assert m.last_request.json() == {
             "tag_name": tag,
             "name": tag,
-            "body": release_notes,
+            "body": RELEASE_NOTES,
             "draft": False,
             "prerelease": prerelease,
         }
 
 
 @pytest.mark.parametrize("token", (None, "super-token"))
 def test_should_create_release_using_token_or_netrc(default_gitea_client, token):
     default_gitea_client.token = token
     default_gitea_client.session.auth = None if not token else TokenAuth(token)
     tag = "v1.0.0"
-    release_notes = "#TODO: Release Notes"
 
     # Note write netrc file with DEFAULT_DOMAIN not DEFAULT_API_DOMAIN as can't
     # handle /api/v1 in file
     with requests_mock.Mocker(session=default_gitea_client.session) as m, netrc_file(
         machine=default_gitea_client.DEFAULT_DOMAIN
     ) as netrc, mock.patch.dict(os.environ, {"NETRC": netrc.name}, clear=True):
         m.register_uri("POST", gitea_api_matcher, json={"id": 1}, status_code=201)
-        assert default_gitea_client.create_release(tag, release_notes) == 1
+        assert default_gitea_client.create_release(tag, RELEASE_NOTES) == 1
         assert m.called
         assert len(m.request_history) == 1
         assert m.last_request.method == "POST"
         if not token:
             assert {
                 "Authorization": "Basic "
                 + base64.encodebytes(
@@ -307,27 +304,27 @@
                 owner=default_gitea_client.owner,
                 repo_name=default_gitea_client.repo_name,
             )
         )
         assert m.last_request.json() == {
             "tag_name": tag,
             "name": tag,
-            "body": release_notes,
+            "body": RELEASE_NOTES,
             "draft": False,
             "prerelease": False,
         }
 
 
 def test_request_has_no_auth_header_if_no_token_or_netrc():
     with mock.patch.dict(os.environ, {}, clear=True):
         client = Gitea(remote_url="git@gitea.com:something/somewhere.git")
 
         with requests_mock.Mocker(session=client.session) as m:
             m.register_uri("POST", gitea_api_matcher, json={"id": 1}, status_code=201)
-            assert client.create_release("v1.0.0", "#TODO: Release Notes") == 1
+            assert client.create_release("v1.0.0", RELEASE_NOTES) == 1
             assert m.called
             assert len(m.request_history) == 1
             assert m.last_request.method == "POST"
             assert (
                 m.last_request.url
                 == "{api_url}/repos/{owner}/{repo_name}/releases".format(
                     api_url=client.api_url,
@@ -369,115 +366,111 @@
 
 
 @pytest.mark.parametrize("status_code", [201])
 @pytest.mark.parametrize("mock_release_id", range(3))
 def test_edit_release_notes_succeeds(
     default_gitea_client, status_code, mock_release_id
 ):
-    release_notes = "#TODO: Release Notes"
     with requests_mock.Mocker(session=default_gitea_client.session) as m:
         m.register_uri(
             "PATCH",
             gitea_api_matcher,
             json={"id": mock_release_id},
             status_code=status_code,
         )
         assert (
-            default_gitea_client.edit_release_notes(mock_release_id, release_notes)
+            default_gitea_client.edit_release_notes(mock_release_id, RELEASE_NOTES)
             == mock_release_id
         )
         assert m.called
         assert len(m.request_history) == 1
         assert m.last_request.method == "PATCH"
         assert (
             m.last_request.url
             == "{api_url}/repos/{owner}/{repo_name}/releases/{release_id}".format(
                 api_url=default_gitea_client.api_url,
                 owner=default_gitea_client.owner,
                 repo_name=default_gitea_client.repo_name,
                 release_id=mock_release_id,
             )
         )
-        assert m.last_request.json() == {"body": release_notes}
+        assert m.last_request.json() == {"body": RELEASE_NOTES}
 
 
 @pytest.mark.parametrize("status_code", (400, 404, 429, 500, 503))
 @pytest.mark.parametrize("mock_release_id", range(3))
 def test_edit_release_notes_fails(default_gitea_client, status_code, mock_release_id):
-    release_notes = "#TODO: Release Notes"
     with requests_mock.Mocker(session=default_gitea_client.session) as m:
         m.register_uri(
             "PATCH",
             gitea_api_matcher,
             json={"id": mock_release_id},
             status_code=status_code,
         )
 
         with pytest.raises(HTTPError):
-            default_gitea_client.edit_release_notes(mock_release_id, release_notes)
+            default_gitea_client.edit_release_notes(mock_release_id, RELEASE_NOTES)
 
         assert m.called
         assert len(m.request_history) == 1
         assert m.last_request.method == "PATCH"
         assert (
             m.last_request.url
             == "{api_url}/repos/{owner}/{repo_name}/releases/{release_id}".format(
                 api_url=default_gitea_client.api_url,
                 owner=default_gitea_client.owner,
                 repo_name=default_gitea_client.repo_name,
                 release_id=mock_release_id,
             )
         )
-        assert m.last_request.json() == {"body": release_notes}
+        assert m.last_request.json() == {"body": RELEASE_NOTES}
 
 
 # Note - mocking as the logic for the create/update of a release
 # is covered by testing above, no point re-testing.
 
 
 @pytest.mark.parametrize("mock_release_id", range(3))
 @pytest.mark.parametrize("prerelease", (True, False))
 def test_create_or_update_release_when_create_succeeds(
     default_gitea_client,
     mock_release_id,
     prerelease,
 ):
     tag = "v1.0.0"
-    release_notes = "# TODO: Release Notes"
     with mock.patch.object(
         default_gitea_client, "create_release"
     ) as mock_create_release, mock.patch.object(
         default_gitea_client, "get_release_id_by_tag"
     ) as mock_get_release_id_by_tag, mock.patch.object(
         default_gitea_client, "edit_release_notes"
     ) as mock_edit_release_notes:
         mock_create_release.return_value = mock_release_id
         mock_get_release_id_by_tag.return_value = mock_release_id
         mock_edit_release_notes.return_value = mock_release_id
         # client = Github(remote_url="git@github.com:something/somewhere.git")
         assert (
             default_gitea_client.create_or_update_release(
-                tag, release_notes, prerelease
+                tag, RELEASE_NOTES, prerelease
             )
             == mock_release_id
         )
-        mock_create_release.assert_called_once_with(tag, release_notes, prerelease)
+        mock_create_release.assert_called_once_with(tag, RELEASE_NOTES, prerelease)
         mock_get_release_id_by_tag.assert_not_called()
         mock_edit_release_notes.assert_not_called()
 
 
 @pytest.mark.parametrize("mock_release_id", range(3))
 @pytest.mark.parametrize("prerelease", (True, False))
 def test_create_or_update_release_when_create_fails_and_update_succeeds(
     default_gitea_client,
     mock_release_id,
     prerelease,
 ):
     tag = "v1.0.0"
-    release_notes = "# TODO: Release Notes"
     not_found = HTTPError("404 Not Found", response=Response())
     not_found.response.status_code = 404
     with mock.patch.object(
         default_gitea_client, "create_release"
     ) as mock_create_release, mock.patch.object(
         default_gitea_client, "get_release_id_by_tag"
     ) as mock_get_release_id_by_tag, mock.patch.object(
@@ -485,28 +478,27 @@
     ) as mock_edit_release_notes:
         mock_create_release.side_effect = not_found
         mock_get_release_id_by_tag.return_value = mock_release_id
         mock_edit_release_notes.return_value = mock_release_id
         # client = Github(remote_url="git@github.com:something/somewhere.git")
         assert (
             default_gitea_client.create_or_update_release(
-                tag, release_notes, prerelease
+                tag, RELEASE_NOTES, prerelease
             )
             == mock_release_id
         )
         mock_get_release_id_by_tag.assert_called_once_with(tag)
-        mock_edit_release_notes.assert_called_once_with(mock_release_id, release_notes)
+        mock_edit_release_notes.assert_called_once_with(mock_release_id, RELEASE_NOTES)
 
 
 @pytest.mark.parametrize("prerelease", (True, False))
 def test_create_or_update_release_when_create_fails_and_no_release_for_tag(
     default_gitea_client, prerelease
 ):
     tag = "v1.0.0"
-    release_notes = "# TODO: Release Notes"
     not_found = HTTPError("404 Not Found", response=Response())
     not_found.response.status_code = 404
     with mock.patch.object(
         default_gitea_client, "create_release"
     ) as mock_create_release, mock.patch.object(
         default_gitea_client, "get_release_id_by_tag"
     ) as mock_get_release_id_by_tag, mock.patch.object(
@@ -514,15 +506,15 @@
     ) as mock_edit_release_notes:
         mock_create_release.side_effect = not_found
         mock_get_release_id_by_tag.return_value = None
         mock_edit_release_notes.return_value = None
 
         with pytest.raises(ValueError):
             default_gitea_client.create_or_update_release(
-                tag, release_notes, prerelease
+                tag, RELEASE_NOTES, prerelease
             )
 
         mock_get_release_id_by_tag.assert_called_once_with(tag)
         mock_edit_release_notes.assert_not_called()
 
 
 @pytest.mark.parametrize("status_code", (200, 201))
```

### Comparing `python-semantic-release-8.0.0rc2/tests/unit/semantic_release/hvcs/test_github.py` & `python-semantic-release-8.0.0rc3/tests/unit/semantic_release/hvcs/test_github.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import pytest
 import requests_mock
 from requests import HTTPError, Response, Session
 
 from semantic_release.hvcs.github import Github
 from semantic_release.hvcs.token_auth import TokenAuth
 
-from tests.const import EXAMPLE_REPO_NAME, EXAMPLE_REPO_OWNER
+from tests.const import EXAMPLE_REPO_NAME, EXAMPLE_REPO_OWNER, RELEASE_NOTES
 from tests.util import netrc_file
 
 
 @pytest.fixture
 def default_gh_client():
     remote_url = f"git@github.com:{EXAMPLE_REPO_OWNER}/{EXAMPLE_REPO_NAME}.git"
     yield Github(remote_url=remote_url)
@@ -236,24 +236,23 @@
 @pytest.mark.parametrize("status_code", (200, 201))
 @pytest.mark.parametrize("mock_release_id", range(3))
 @pytest.mark.parametrize("prerelease", (True, False))
 def test_create_release_succeeds(
     default_gh_client, status_code, prerelease, mock_release_id
 ):
     tag = "v1.0.0"
-    release_notes = "# TODO: Release Notes"
     with requests_mock.Mocker(session=default_gh_client.session) as m:
         m.register_uri(
             "POST",
             github_api_matcher,
             json={"id": mock_release_id},
             status_code=status_code,
         )
         assert (
-            default_gh_client.create_release(tag, release_notes, prerelease)
+            default_gh_client.create_release(tag, RELEASE_NOTES, prerelease)
             == mock_release_id
         )
         assert m.called
         assert len(m.request_history) == 1
         assert m.last_request.method == "POST"
         assert (
             m.last_request.url
@@ -262,32 +261,31 @@
                 owner=default_gh_client.owner,
                 repo_name=default_gh_client.repo_name,
             )
         )
         assert m.last_request.json() == {
             "tag_name": tag,
             "name": tag,
-            "body": release_notes,
+            "body": RELEASE_NOTES,
             "draft": False,
             "prerelease": prerelease,
         }
 
 
 @pytest.mark.parametrize("status_code", (400, 404, 429, 500, 503))
 @pytest.mark.parametrize("prerelease", (True, False))
 def test_create_release_fails(default_gh_client, prerelease, status_code):
     tag = "v1.0.0"
-    release_notes = "# TODO: Release Notes"
     with requests_mock.Mocker(session=default_gh_client.session) as m:
         m.register_uri(
             "POST", github_api_matcher, json={"id": 1}, status_code=status_code
         )
 
         with pytest.raises(HTTPError):
-            default_gh_client.create_release(tag, release_notes, prerelease)
+            default_gh_client.create_release(tag, RELEASE_NOTES, prerelease)
 
         assert m.called
         assert len(m.request_history) == 1
         assert m.last_request.method == "POST"
         assert (
             m.last_request.url
             == "{api_url}/repos/{owner}/{repo_name}/releases".format(
@@ -295,31 +293,30 @@
                 owner=default_gh_client.owner,
                 repo_name=default_gh_client.repo_name,
             )
         )
         assert m.last_request.json() == {
             "tag_name": tag,
             "name": tag,
-            "body": release_notes,
+            "body": RELEASE_NOTES,
             "draft": False,
             "prerelease": prerelease,
         }
 
 
 @pytest.mark.parametrize("token", (None, "super-token"))
 def test_should_create_release_using_token_or_netrc(default_gh_client, token):
     default_gh_client.token = token
     default_gh_client.session.auth = None if not token else TokenAuth(token)
     tag = "v1.0.0"
-    release_notes = "# TODO: Release Notes"
     with requests_mock.Mocker(session=default_gh_client.session) as m, netrc_file(
         machine=default_gh_client.DEFAULT_API_DOMAIN
     ) as netrc, mock.patch.dict(os.environ, {"NETRC": netrc.name}, clear=True):
         m.register_uri("POST", github_api_matcher, json={"id": 1}, status_code=201)
-        assert default_gh_client.create_release(tag, release_notes) == 1
+        assert default_gh_client.create_release(tag, RELEASE_NOTES) == 1
         assert m.called
         assert len(m.request_history) == 1
         assert m.last_request.method == "POST"
         if not token:
             assert {
                 "Authorization": "Basic "
                 + base64.encodebytes(
@@ -339,27 +336,27 @@
                 owner=default_gh_client.owner,
                 repo_name=default_gh_client.repo_name,
             )
         )
         assert m.last_request.json() == {
             "tag_name": tag,
             "name": tag,
-            "body": release_notes,
+            "body": RELEASE_NOTES,
             "draft": False,
             "prerelease": False,
         }
 
 
 def test_request_has_no_auth_header_if_no_token_or_netrc():
     with mock.patch.dict(os.environ, {}, clear=True):
         client = Github(remote_url="git@github.com:something/somewhere.git")
 
         with requests_mock.Mocker(session=client.session) as m:
             m.register_uri("POST", github_api_matcher, json={"id": 1}, status_code=201)
-            assert client.create_release("v1.0.0", "# TODO: Release Notes") == 1
+            assert client.create_release("v1.0.0", RELEASE_NOTES) == 1
             assert m.called
             assert len(m.request_history) == 1
             assert m.last_request.method == "POST"
             assert (
                 m.last_request.url
                 == "{api_url}/repos/{owner}/{repo_name}/releases".format(
                     api_url=client.api_url,
@@ -369,66 +366,64 @@
             )
             assert "Authorization" not in m.last_request.headers
 
 
 @pytest.mark.parametrize("status_code", [201])
 @pytest.mark.parametrize("mock_release_id", range(3))
 def test_edit_release_notes_succeeds(default_gh_client, status_code, mock_release_id):
-    release_notes = "# TODO: Release Notes"
     with requests_mock.Mocker(session=default_gh_client.session) as m:
         m.register_uri(
             "POST",
             github_api_matcher,
             json={"id": mock_release_id},
             status_code=status_code,
         )
         assert (
-            default_gh_client.edit_release_notes(mock_release_id, release_notes)
+            default_gh_client.edit_release_notes(mock_release_id, RELEASE_NOTES)
             == mock_release_id
         )
         assert m.called
         assert len(m.request_history) == 1
         assert m.last_request.method == "POST"
         assert (
             m.last_request.url
             == "{api_url}/repos/{owner}/{repo_name}/releases/{release_id}".format(
                 api_url=default_gh_client.api_url,
                 owner=default_gh_client.owner,
                 repo_name=default_gh_client.repo_name,
                 release_id=mock_release_id,
             )
         )
-        assert m.last_request.json() == {"body": release_notes}
+        assert m.last_request.json() == {"body": RELEASE_NOTES}
 
 
 @pytest.mark.parametrize("status_code", (400, 404, 429, 500, 503))
 def test_edit_release_notes_fails(default_gh_client, status_code):
     release_id = 420
-    release_notes = "# TODO: Release Notes"
     with requests_mock.Mocker(session=default_gh_client.session) as m:
         m.register_uri(
             "POST", github_api_matcher, json={"id": release_id}, status_code=status_code
         )
 
         with pytest.raises(HTTPError):
-            default_gh_client.edit_release_notes(release_id, release_notes)
+            default_gh_client.edit_release_notes(release_id, RELEASE_NOTES)
 
         assert m.called
         assert len(m.request_history) == 1
         assert m.last_request.method == "POST"
         assert (
             m.last_request.url
             == "{api_url}/repos/{owner}/{repo_name}/releases/{release_id}".format(
                 api_url=default_gh_client.api_url,
                 owner=default_gh_client.owner,
                 repo_name=default_gh_client.repo_name,
                 release_id=release_id,
             )
         )
-        assert m.last_request.json() == {"body": release_notes}
+        assert m.last_request.json() == {"body": RELEASE_NOTES}
 
 
 @pytest.mark.parametrize(
     "resp_payload, status_code, expected",
     [
         ({"id": 420, "status": "success"}, 200, 420),
         ({"error": "not found"}, 404, None),
@@ -466,86 +461,83 @@
 @pytest.mark.parametrize("prerelease", (True, False))
 def test_create_or_update_release_when_create_succeeds(
     default_gh_client,
     mock_release_id,
     prerelease,
 ):
     tag = "v1.0.0"
-    release_notes = "# TODO: Release Notes"
     with mock.patch.object(
         default_gh_client, "create_release"
     ) as mock_create_release, mock.patch.object(
         default_gh_client, "get_release_id_by_tag"
     ) as mock_get_release_id_by_tag, mock.patch.object(
         default_gh_client, "edit_release_notes"
     ) as mock_edit_release_notes:
         mock_create_release.return_value = mock_release_id
         mock_get_release_id_by_tag.return_value = mock_release_id
         mock_edit_release_notes.return_value = mock_release_id
         # client = Github(remote_url="git@github.com:something/somewhere.git")
         assert (
-            default_gh_client.create_or_update_release(tag, release_notes, prerelease)
+            default_gh_client.create_or_update_release(tag, RELEASE_NOTES, prerelease)
             == mock_release_id
         )
-        mock_create_release.assert_called_once_with(tag, release_notes, prerelease)
+        mock_create_release.assert_called_once_with(tag, RELEASE_NOTES, prerelease)
         mock_get_release_id_by_tag.assert_not_called()
         mock_edit_release_notes.assert_not_called()
 
 
 @pytest.mark.parametrize("mock_release_id", range(3))
 @pytest.mark.parametrize("prerelease", (True, False))
 def test_create_or_update_release_when_create_fails_and_update_succeeds(
     default_gh_client,
     mock_release_id,
     prerelease,
 ):
     tag = "v1.0.0"
-    release_notes = "# TODO: Release Notes"
     not_found = HTTPError("404 Not Found", response=Response())
     not_found.response.status_code = 404
     with mock.patch.object(
         default_gh_client, "create_release"
     ) as mock_create_release, mock.patch.object(
         default_gh_client, "get_release_id_by_tag"
     ) as mock_get_release_id_by_tag, mock.patch.object(
         default_gh_client, "edit_release_notes"
     ) as mock_edit_release_notes:
         mock_create_release.side_effect = not_found
         mock_get_release_id_by_tag.return_value = mock_release_id
         mock_edit_release_notes.return_value = mock_release_id
         # client = Github(remote_url="git@github.com:something/somewhere.git")
         assert (
-            default_gh_client.create_or_update_release(tag, release_notes, prerelease)
+            default_gh_client.create_or_update_release(tag, RELEASE_NOTES, prerelease)
             == mock_release_id
         )
         mock_get_release_id_by_tag.assert_called_once_with(tag)
-        mock_edit_release_notes.assert_called_once_with(mock_release_id, release_notes)
+        mock_edit_release_notes.assert_called_once_with(mock_release_id, RELEASE_NOTES)
 
 
 @pytest.mark.parametrize("prerelease", (True, False))
 def test_create_or_update_release_when_create_fails_and_no_release_for_tag(
     default_gh_client, prerelease
 ):
     tag = "v1.0.0"
-    release_notes = "# TODO: Release Notes"
     not_found = HTTPError("404 Not Found", response=Response())
     not_found.response.status_code = 404
     with mock.patch.object(
         default_gh_client, "create_release"
     ) as mock_create_release, mock.patch.object(
         default_gh_client, "get_release_id_by_tag"
     ) as mock_get_release_id_by_tag, mock.patch.object(
         default_gh_client, "edit_release_notes"
     ) as mock_edit_release_notes:
         mock_create_release.side_effect = not_found
         mock_get_release_id_by_tag.return_value = None
         mock_edit_release_notes.return_value = None
 
         with pytest.raises(ValueError):
-            default_gh_client.create_or_update_release(tag, release_notes, prerelease)
+            default_gh_client.create_or_update_release(tag, RELEASE_NOTES, prerelease)
 
         mock_get_release_id_by_tag.assert_called_once_with(tag)
         mock_edit_release_notes.assert_not_called()
 
 
 @pytest.mark.parametrize("status_code", (200, 201))
 @pytest.mark.parametrize("mock_release_id", range(3))
```

### Comparing `python-semantic-release-8.0.0rc2/tests/unit/semantic_release/hvcs/test_gitlab.py` & `python-semantic-release-8.0.0rc3/tests/unit/semantic_release/hvcs/test_gitlab.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,23 +4,25 @@
 
 import gitlab
 import pytest
 from requests import Session
 
 from semantic_release.hvcs.gitlab import Gitlab
 
-from tests.const import EXAMPLE_REPO_NAME, EXAMPLE_REPO_OWNER
+from tests.const import EXAMPLE_REPO_NAME, EXAMPLE_REPO_OWNER, RELEASE_NOTES
 
 gitlab.Gitlab("")  # instantiation necessary to discover gitlab ProjectManager
 
 # Note: there's nothing special about the value of these variables,
 # they're just constants for easier consistency with the faked objects
 A_GOOD_TAG = "v1.2.3"
 A_BAD_TAG = "v2.1.1-rc.1"
 A_LOCKED_TAG = "v0.9.0"
+A_MISSING_TAG = "v1.0.0+missing"
+AN_EXISTING_TAG = "v2.3.4+existing"
 # But note this is the only ref we're making a "fake" commit for, so
 # tests which need to query the remote for "a" ref, the exact sha for
 # which doesn't matter, all use this constant
 REF = "hashashash"
 
 
 class _GitlabProject:
@@ -88,38 +90,43 @@
                 return self.jobs
 
     class _Tags:
         def __init__(self):
             pass
 
         def get(self, tag):
-            if tag == A_GOOD_TAG:
+            if tag in (A_GOOD_TAG, AN_EXISTING_TAG):
                 return self._Tag()
             elif tag == A_LOCKED_TAG:
                 return self._Tag(locked=True)
             else:
-                raise gitlab.exceptions.GitlabGetError
+                raise gitlab.exceptions.GitlabGetError()
 
         class _Tag:
             def __init__(self, locked=False):
                 self.locked = locked
 
             def set_release_description(self, release_notes):
                 if self.locked:
-                    raise gitlab.exceptions.GitlabUpdateError
+                    raise gitlab.exceptions.GitlabUpdateError()
 
     class _Releases:
         def __init__(self):
             pass
 
         def create(self, input_):
             if input_["name"] and input_["tag_name"]:
                 if input_["tag_name"] in (A_GOOD_TAG, A_LOCKED_TAG):
                     return self._Release()
-            raise gitlab.exceptions.GitlabCreateError
+            raise gitlab.exceptions.GitlabCreateError()
+
+        def update(self, tag, new_data):
+            if tag == A_MISSING_TAG:
+                raise gitlab.exceptions.GitlabUpdateError()
+            return self._Release()
 
         class _Release:
             def __init__(self, locked=False):
                 pass
 
 
 @contextmanager
@@ -310,19 +317,93 @@
         domain=default_gl_client.hvcs_domain,
         owner=default_gl_client.owner,
         repo=default_gl_client.repo_name,
         pr_number=pr_number,
     )
 
 
-@pytest.mark.parametrize(
-    "tag, expected",
-    [
-        (A_GOOD_TAG, True),
-        (A_LOCKED_TAG, True),
-        (A_BAD_TAG, False),
-    ],
-)
-def test_create_release(default_gl_client, tag, expected):
-    release_notes = "# TODO: Release Notes"
+@pytest.mark.parametrize("tag", (A_GOOD_TAG, A_LOCKED_TAG))
+def test_create_release_succeeds(default_gl_client, tag):
     with mock_gitlab():
-        assert default_gl_client.create_release(tag, release_notes) == expected
+        assert default_gl_client.create_release(tag, RELEASE_NOTES) == tag
+
+
+def test_create_release_fails_with_bad_tag(default_gl_client):
+    with mock_gitlab(), pytest.raises(gitlab.GitlabCreateError):
+        default_gl_client.create_release(A_BAD_TAG, RELEASE_NOTES)
+
+
+@pytest.mark.parametrize("tag", (A_GOOD_TAG, A_LOCKED_TAG))
+def test_update_release_succeeds(default_gl_client, tag):
+    with mock_gitlab():
+        assert default_gl_client.edit_release_notes(tag, RELEASE_NOTES) == tag
+
+
+def test_update_release_fails_with_missing_tag(default_gl_client):
+    with mock_gitlab(), pytest.raises(gitlab.GitlabUpdateError):
+        default_gl_client.edit_release_notes(A_MISSING_TAG, RELEASE_NOTES)
+
+
+@pytest.mark.parametrize("prerelease", (True, False))
+def test_create_or_update_release_when_create_succeeds(default_gl_client, prerelease):
+    with mock.patch.object(
+        default_gl_client, "create_release"
+    ) as mock_create_release, mock.patch.object(
+        default_gl_client, "edit_release_notes"
+    ) as mock_edit_release_notes:
+        mock_create_release.return_value = A_GOOD_TAG
+        mock_edit_release_notes.return_value = A_GOOD_TAG
+        # client = Github(remote_url="git@github.com:something/somewhere.git")
+        assert (
+            default_gl_client.create_or_update_release(
+                A_GOOD_TAG, RELEASE_NOTES, prerelease
+            )
+            == A_GOOD_TAG
+        )
+        mock_create_release.assert_called_once_with(
+            tag=A_GOOD_TAG, release_notes=RELEASE_NOTES, prerelease=prerelease
+        )
+        mock_edit_release_notes.assert_not_called()
+
+
+@pytest.mark.parametrize("prerelease", (True, False))
+def test_create_or_update_release_when_create_fails_and_update_succeeds(
+    default_gl_client, prerelease
+):
+    bad_request = gitlab.GitlabCreateError("400 Bad Request")
+    with mock.patch.object(
+        default_gl_client, "create_release"
+    ) as mock_create_release, mock.patch.object(
+        default_gl_client, "edit_release_notes"
+    ) as mock_edit_release_notes:
+        mock_create_release.side_effect = bad_request
+        mock_edit_release_notes.return_value = A_GOOD_TAG
+        # client = Github(remote_url="git@github.com:something/somewhere.git")
+        assert (
+            default_gl_client.create_or_update_release(
+                A_GOOD_TAG, RELEASE_NOTES, prerelease
+            )
+            == A_GOOD_TAG
+        )
+        mock_edit_release_notes.assert_called_once_with(
+            release_id=A_GOOD_TAG, release_notes=RELEASE_NOTES
+        )
+
+
+@pytest.mark.parametrize("prerelease", (True, False))
+def test_create_or_update_release_when_create_fails_and_update_fails(
+    default_gl_client, prerelease
+):
+    bad_request = gitlab.GitlabCreateError("400 Bad Request")
+    not_found = gitlab.GitlabUpdateError("404 Not Found")
+    with mock.patch.object(
+        default_gl_client, "create_release"
+    ) as mock_create_release, mock.patch.object(
+        default_gl_client, "edit_release_notes"
+    ) as mock_edit_release_notes:
+        mock_create_release.side_effect = bad_request
+        mock_edit_release_notes.side_effect = not_found
+
+        with pytest.raises(gitlab.GitlabUpdateError):
+            default_gl_client.create_or_update_release(
+                A_GOOD_TAG, RELEASE_NOTES, prerelease
+            )
```

### Comparing `python-semantic-release-8.0.0rc2/tests/unit/semantic_release/hvcs/test_token_auth.py` & `python-semantic-release-8.0.0rc3/tests/unit/semantic_release/hvcs/test_token_auth.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/tests/unit/semantic_release/version/test_algorithm.py` & `python-semantic-release-8.0.0rc3/tests/unit/semantic_release/version/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/tests/unit/semantic_release/version/test_declaration.py` & `python-semantic-release-8.0.0rc3/tests/unit/semantic_release/version/test_declaration.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/tests/unit/semantic_release/version/test_translator.py` & `python-semantic-release-8.0.0rc3/tests/unit/semantic_release/version/test_translator.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0rc2/tests/unit/semantic_release/version/test_version.py` & `python-semantic-release-8.0.0rc3/tests/unit/semantic_release/version/test_version.py`

 * *Files identical despite different names*

