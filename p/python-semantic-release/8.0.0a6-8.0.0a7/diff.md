# Comparing `tmp/python-semantic-release-8.0.0a6.tar.gz` & `tmp/python-semantic-release-8.0.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-semantic-release-8.0.0a6.tar", last modified: Sun Jun  4 17:38:36 2023, max compression
+gzip compressed data, was "python-semantic-release-8.0.0a7.tar", last modified: Sun Jun 11 19:23:09 2023, max compression
```

## Comparing `python-semantic-release-8.0.0a6.tar` & `python-semantic-release-8.0.0a7.tar`

### file list

```diff
@@ -1,129 +1,130 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 17:38:36.173791 python-semantic-release-8.0.0a6/
--rw-r--r--   0 root         (0) root         (0)      230 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/AUTHORS.rst
--rw-r--r--   0 root         (0) root         (0)     1084 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/LICENSE
--rw-r--r--   0 root         (0) root         (0)      153 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3110 2023-06-04 17:38:36.173791 python-semantic-release-8.0.0a6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2272 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/README.rst
--rw-r--r--   0 root         (0) root         (0)     4632 2023-06-04 17:38:28.000000 python-semantic-release-8.0.0a6/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 17:38:36.161791 python-semantic-release-8.0.0a6/python_semantic_release.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3110 2023-06-04 17:38:36.000000 python-semantic-release-8.0.0a6/python_semantic_release.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4186 2023-06-04 17:38:36.000000 python-semantic-release-8.0.0a6/python_semantic_release.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-04 17:38:36.000000 python-semantic-release-8.0.0a6/python_semantic_release.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-06-04 17:38:36.000000 python-semantic-release-8.0.0a6/python_semantic_release.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      582 2023-06-04 17:38:36.000000 python-semantic-release-8.0.0a6/python_semantic_release.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-04 17:38:36.000000 python-semantic-release-8.0.0a6/python_semantic_release.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 17:38:36.161791 python-semantic-release-8.0.0a6/semantic_release/
--rw-r--r--   0 root         (0) root         (0)     1093 2023-06-04 17:38:28.000000 python-semantic-release-8.0.0a6/semantic_release/__init__.py
--rw-r--r--   0 root         (0) root         (0)      106 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 17:38:36.161791 python-semantic-release-8.0.0a6/semantic_release/changelog/
--rw-r--r--   0 root         (0) root         (0)      361 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/changelog/__init__.py
--rw-r--r--   0 root         (0) root         (0)      941 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/changelog/context.py
--rw-r--r--   0 root         (0) root         (0)     6470 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/changelog/release_history.py
--rw-r--r--   0 root         (0) root         (0)     4328 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/changelog/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 17:38:36.165791 python-semantic-release-8.0.0a6/semantic_release/cli/
--rw-r--r--   0 root         (0) root         (0)      451 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 17:38:36.165791 python-semantic-release-8.0.0a6/semantic_release/cli/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/cli/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3246 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/cli/commands/changelog.py
--rw-r--r--   0 root         (0) root         (0)     1448 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/cli/commands/generate_config.py
--rw-r--r--   0 root         (0) root         (0)     4451 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/cli/commands/main.py
--rw-r--r--   0 root         (0) root         (0)     1133 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/cli/commands/publish.py
--rw-r--r--   0 root         (0) root         (0)    18060 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/cli/commands/version.py
--rw-r--r--   0 root         (0) root         (0)      929 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/cli/common.py
--rw-r--r--   0 root         (0) root         (0)    13693 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/cli/config.py
--rw-r--r--   0 root         (0) root         (0)       39 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/cli/const.py
--rw-r--r--   0 root         (0) root         (0)     2105 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/cli/github_actions_output.py
--rw-r--r--   0 root         (0) root         (0)     2875 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/cli/masking_filter.py
--rw-r--r--   0 root         (0) root         (0)      935 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/cli/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 17:38:36.165791 python-semantic-release-8.0.0a6/semantic_release/commit_parser/
--rw-r--r--   0 root         (0) root         (0)      884 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/commit_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2569 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/commit_parser/_base.py
--rw-r--r--   0 root         (0) root         (0)     4364 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/commit_parser/angular.py
--rw-r--r--   0 root         (0) root         (0)     3288 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/commit_parser/emoji.py
--rw-r--r--   0 root         (0) root         (0)     5713 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/commit_parser/scipy.py
--rw-r--r--   0 root         (0) root         (0)     3193 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/commit_parser/tag.py
--rw-r--r--   0 root         (0) root         (0)     1456 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/commit_parser/token.py
--rw-r--r--   0 root         (0) root         (0)      529 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/commit_parser/util.py
--rw-r--r--   0 root         (0) root         (0)      831 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/const.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 17:38:36.157791 python-semantic-release-8.0.0a6/semantic_release/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 17:38:36.165791 python-semantic-release-8.0.0a6/semantic_release/data/templates/
--rw-r--r--   0 root         (0) root         (0)     1059 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/data/templates/CHANGELOG.md.j2
--rw-r--r--   0 root         (0) root         (0)      465 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/data/templates/release_notes.md.j2
--rw-r--r--   0 root         (0) root         (0)     1020 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/enums.py
--rw-r--r--   0 root         (0) root         (0)      674 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/errors.py
--rw-r--r--   0 root         (0) root         (0)     4088 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 17:38:36.165791 python-semantic-release-8.0.0a6/semantic_release/hvcs/
--rw-r--r--   0 root         (0) root         (0)      300 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/hvcs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5579 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/hvcs/_base.py
--rw-r--r--   0 root         (0) root         (0)     8285 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/hvcs/gitea.py
--rw-r--r--   0 root         (0) root         (0)    10154 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/hvcs/github.py
--rw-r--r--   0 root         (0) root         (0)     5029 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/hvcs/gitlab.py
--rw-r--r--   0 root         (0) root         (0)      681 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/hvcs/token_auth.py
--rw-r--r--   0 root         (0) root         (0)     2774 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/hvcs/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 17:38:36.165791 python-semantic-release-8.0.0a6/semantic_release/version/
--rw-r--r--   0 root         (0) root         (0)      339 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/version/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14177 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/version/algorithm.py
--rw-r--r--   0 root         (0) root         (0)     7267 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/version/declaration.py
--rw-r--r--   0 root         (0) root         (0)     3103 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/version/translator.py
--rw-r--r--   0 root         (0) root         (0)    14060 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/version/version.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-04 17:38:36.173791 python-semantic-release-8.0.0a6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      466 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 17:38:36.161791 python-semantic-release-8.0.0a6/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 17:38:36.169791 python-semantic-release-8.0.0a6/tests/command_line/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/command_line/__init__.py
--rw-r--r--   0 root         (0) root         (0)      174 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/command_line/conftest.py
--rw-r--r--   0 root         (0) root         (0)     5707 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/command_line/test_changelog.py
--rw-r--r--   0 root         (0) root         (0)     1320 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/command_line/test_generate_config.py
--rw-r--r--   0 root         (0) root         (0)      641 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/command_line/test_help.py
--rw-r--r--   0 root         (0) root         (0)      501 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/command_line/test_main.py
--rw-r--r--   0 root         (0) root         (0)    25217 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/command_line/test_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 17:38:36.169791 python-semantic-release-8.0.0a6/tests/fixtures/
--rw-r--r--   0 root         (0) root         (0)      106 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/fixtures/__init__.py
--rw-r--r--   0 root         (0) root         (0)      906 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/fixtures/commit_parsers.py
--rw-r--r--   0 root         (0) root         (0)     2235 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/fixtures/example_project.py
--rw-r--r--   0 root         (0) root         (0)    45283 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/fixtures/git_repo.py
--rw-r--r--   0 root         (0) root         (0)     4424 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/fixtures/scipy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 17:38:36.169791 python-semantic-release-8.0.0a6/tests/scenario/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/scenario/__init__.py
--rw-r--r--   0 root         (0) root         (0)    46838 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/scenario/test_next_version.py
--rw-r--r--   0 root         (0) root         (0)    12186 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/scenario/test_release_history.py
--rw-r--r--   0 root         (0) root         (0)     3513 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/scenario/test_template_render.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 17:38:36.169791 python-semantic-release-8.0.0a6/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 17:38:36.169791 python-semantic-release-8.0.0a6/tests/unit/semantic_release/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 17:38:36.169791 python-semantic-release-8.0.0a6/tests/unit/semantic_release/changelog/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/changelog/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5005 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/changelog/test_changelog_context.py
--rw-r--r--   0 root         (0) root         (0)     2540 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/changelog/test_default_changelog.py
--rw-r--r--   0 root         (0) root         (0)     1747 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/changelog/test_release_notes.py
--rw-r--r--   0 root         (0) root         (0)     2102 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/changelog/test_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 17:38:36.169791 python-semantic-release-8.0.0a6/tests/unit/semantic_release/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1730 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/cli/test_config.py
--rw-r--r--   0 root         (0) root         (0)     1784 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/cli/test_github_actions_output.py
--rw-r--r--   0 root         (0) root         (0)     5768 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/cli/test_masking_filter.py
--rw-r--r--   0 root         (0) root         (0)      799 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/cli/test_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 17:38:36.169791 python-semantic-release-8.0.0a6/tests/unit/semantic_release/commit_parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/commit_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)      140 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/commit_parser/helper.py
--rw-r--r--   0 root         (0) root         (0)     5969 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/commit_parser/test_angular.py
--rw-r--r--   0 root         (0) root         (0)     2487 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/commit_parser/test_emoji.py
--rw-r--r--   0 root         (0) root         (0)      500 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/commit_parser/test_scipy.py
--rw-r--r--   0 root         (0) root         (0)     2173 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/commit_parser/test_tag.py
--rw-r--r--   0 root         (0) root         (0)      648 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/commit_parser/test_token.py
--rw-r--r--   0 root         (0) root         (0)      442 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/commit_parser/test_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 17:38:36.173791 python-semantic-release-8.0.0a6/tests/unit/semantic_release/hvcs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/hvcs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1349 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/hvcs/test__base.py
--rw-r--r--   0 root         (0) root         (0)    22874 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/hvcs/test_gitea.py
--rw-r--r--   0 root         (0) root         (0)    24334 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/hvcs/test_github.py
--rw-r--r--   0 root         (0) root         (0)    10021 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/hvcs/test_gitlab.py
--rw-r--r--   0 root         (0) root         (0)      965 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/hvcs/test_token_auth.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/hvcs/test_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 17:38:36.173791 python-semantic-release-8.0.0a6/tests/unit/semantic_release/version/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/version/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7319 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/version/test_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     3715 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/version/test_declaration.py
--rw-r--r--   0 root         (0) root         (0)     2996 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/version/test_translator.py
--rw-r--r--   0 root         (0) root         (0)     9640 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/version/test_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 19:23:09.863366 python-semantic-release-8.0.0a7/
+-rw-r--r--   0 root         (0) root         (0)      230 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/AUTHORS.rst
+-rw-r--r--   0 root         (0) root         (0)     1084 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      153 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3110 2023-06-11 19:23:09.863366 python-semantic-release-8.0.0a7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2272 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/README.rst
+-rw-r--r--   0 root         (0) root         (0)     4687 2023-06-11 19:23:01.000000 python-semantic-release-8.0.0a7/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 19:23:09.843366 python-semantic-release-8.0.0a7/python_semantic_release.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3110 2023-06-11 19:23:09.000000 python-semantic-release-8.0.0a7/python_semantic_release.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4221 2023-06-11 19:23:09.000000 python-semantic-release-8.0.0a7/python_semantic_release.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-11 19:23:09.000000 python-semantic-release-8.0.0a7/python_semantic_release.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       95 2023-06-11 19:23:09.000000 python-semantic-release-8.0.0a7/python_semantic_release.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      598 2023-06-11 19:23:09.000000 python-semantic-release-8.0.0a7/python_semantic_release.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-06-11 19:23:09.000000 python-semantic-release-8.0.0a7/python_semantic_release.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 19:23:09.843366 python-semantic-release-8.0.0a7/semantic_release/
+-rw-r--r--   0 root         (0) root         (0)     1093 2023-06-11 19:23:01.000000 python-semantic-release-8.0.0a7/semantic_release/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      106 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 19:23:09.847366 python-semantic-release-8.0.0a7/semantic_release/changelog/
+-rw-r--r--   0 root         (0) root         (0)      361 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/changelog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      941 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/changelog/context.py
+-rw-r--r--   0 root         (0) root         (0)     6470 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/changelog/release_history.py
+-rw-r--r--   0 root         (0) root         (0)     4328 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/changelog/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 19:23:09.847366 python-semantic-release-8.0.0a7/semantic_release/cli/
+-rw-r--r--   0 root         (0) root         (0)      451 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 19:23:09.847366 python-semantic-release-8.0.0a7/semantic_release/cli/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/cli/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3246 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/cli/commands/changelog.py
+-rw-r--r--   0 root         (0) root         (0)     1448 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/cli/commands/generate_config.py
+-rw-r--r--   0 root         (0) root         (0)     4978 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/cli/commands/main.py
+-rw-r--r--   0 root         (0) root         (0)     1298 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/cli/commands/publish.py
+-rw-r--r--   0 root         (0) root         (0)    18650 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/cli/commands/version.py
+-rw-r--r--   0 root         (0) root         (0)      929 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/cli/common.py
+-rw-r--r--   0 root         (0) root         (0)    13718 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/cli/config.py
+-rw-r--r--   0 root         (0) root         (0)       39 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/cli/const.py
+-rw-r--r--   0 root         (0) root         (0)     2105 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/cli/github_actions_output.py
+-rw-r--r--   0 root         (0) root         (0)     2875 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/cli/masking_filter.py
+-rw-r--r--   0 root         (0) root         (0)      935 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/cli/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 19:23:09.851366 python-semantic-release-8.0.0a7/semantic_release/commit_parser/
+-rw-r--r--   0 root         (0) root         (0)      884 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/commit_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2569 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/commit_parser/_base.py
+-rw-r--r--   0 root         (0) root         (0)     4364 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/commit_parser/angular.py
+-rw-r--r--   0 root         (0) root         (0)     3288 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/commit_parser/emoji.py
+-rw-r--r--   0 root         (0) root         (0)     5713 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/commit_parser/scipy.py
+-rw-r--r--   0 root         (0) root         (0)     3193 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/commit_parser/tag.py
+-rw-r--r--   0 root         (0) root         (0)     1456 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/commit_parser/token.py
+-rw-r--r--   0 root         (0) root         (0)      529 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/commit_parser/util.py
+-rw-r--r--   0 root         (0) root         (0)      831 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/const.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 19:23:09.839366 python-semantic-release-8.0.0a7/semantic_release/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 19:23:09.851366 python-semantic-release-8.0.0a7/semantic_release/data/templates/
+-rw-r--r--   0 root         (0) root         (0)     1059 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/data/templates/CHANGELOG.md.j2
+-rw-r--r--   0 root         (0) root         (0)      465 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/data/templates/release_notes.md.j2
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/enums.py
+-rw-r--r--   0 root         (0) root         (0)      674 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/errors.py
+-rw-r--r--   0 root         (0) root         (0)     4088 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 19:23:09.851366 python-semantic-release-8.0.0a7/semantic_release/hvcs/
+-rw-r--r--   0 root         (0) root         (0)      300 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/hvcs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5579 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/hvcs/_base.py
+-rw-r--r--   0 root         (0) root         (0)     8285 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/hvcs/gitea.py
+-rw-r--r--   0 root         (0) root         (0)    10154 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/hvcs/github.py
+-rw-r--r--   0 root         (0) root         (0)     5029 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/hvcs/gitlab.py
+-rw-r--r--   0 root         (0) root         (0)      681 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/hvcs/token_auth.py
+-rw-r--r--   0 root         (0) root         (0)     2774 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/hvcs/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 19:23:09.851366 python-semantic-release-8.0.0a7/semantic_release/version/
+-rw-r--r--   0 root         (0) root         (0)      339 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/version/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14177 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/version/algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     7267 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/version/declaration.py
+-rw-r--r--   0 root         (0) root         (0)     3103 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/version/translator.py
+-rw-r--r--   0 root         (0) root         (0)    14060 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/version/version.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-11 19:23:09.863366 python-semantic-release-8.0.0a7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      466 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 19:23:09.839366 python-semantic-release-8.0.0a7/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 19:23:09.855366 python-semantic-release-8.0.0a7/tests/command_line/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/command_line/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      174 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/command_line/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     5707 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/command_line/test_changelog.py
+-rw-r--r--   0 root         (0) root         (0)     1320 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/command_line/test_generate_config.py
+-rw-r--r--   0 root         (0) root         (0)      641 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/command_line/test_help.py
+-rw-r--r--   0 root         (0) root         (0)     1167 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/command_line/test_main.py
+-rw-r--r--   0 root         (0) root         (0)     1430 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/command_line/test_publish.py
+-rw-r--r--   0 root         (0) root         (0)    19966 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/command_line/test_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 19:23:09.855366 python-semantic-release-8.0.0a7/tests/fixtures/
+-rw-r--r--   0 root         (0) root         (0)      106 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/fixtures/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      906 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/fixtures/commit_parsers.py
+-rw-r--r--   0 root         (0) root         (0)     2235 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/fixtures/example_project.py
+-rw-r--r--   0 root         (0) root         (0)    45283 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/fixtures/git_repo.py
+-rw-r--r--   0 root         (0) root         (0)     4424 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/fixtures/scipy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 19:23:09.855366 python-semantic-release-8.0.0a7/tests/scenario/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/scenario/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    46838 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/scenario/test_next_version.py
+-rw-r--r--   0 root         (0) root         (0)    12186 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/scenario/test_release_history.py
+-rw-r--r--   0 root         (0) root         (0)     3513 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/scenario/test_template_render.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 19:23:09.855366 python-semantic-release-8.0.0a7/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 19:23:09.855366 python-semantic-release-8.0.0a7/tests/unit/semantic_release/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 19:23:09.859366 python-semantic-release-8.0.0a7/tests/unit/semantic_release/changelog/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/changelog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5005 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/changelog/test_changelog_context.py
+-rw-r--r--   0 root         (0) root         (0)     2540 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/changelog/test_default_changelog.py
+-rw-r--r--   0 root         (0) root         (0)     1747 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/changelog/test_release_notes.py
+-rw-r--r--   0 root         (0) root         (0)     2102 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/changelog/test_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 19:23:09.859366 python-semantic-release-8.0.0a7/tests/unit/semantic_release/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/cli/test_config.py
+-rw-r--r--   0 root         (0) root         (0)     1784 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/cli/test_github_actions_output.py
+-rw-r--r--   0 root         (0) root         (0)     5768 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/cli/test_masking_filter.py
+-rw-r--r--   0 root         (0) root         (0)      799 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/cli/test_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 19:23:09.859366 python-semantic-release-8.0.0a7/tests/unit/semantic_release/commit_parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/commit_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      140 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/commit_parser/helper.py
+-rw-r--r--   0 root         (0) root         (0)     5969 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/commit_parser/test_angular.py
+-rw-r--r--   0 root         (0) root         (0)     2487 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/commit_parser/test_emoji.py
+-rw-r--r--   0 root         (0) root         (0)      500 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/commit_parser/test_scipy.py
+-rw-r--r--   0 root         (0) root         (0)     2173 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/commit_parser/test_tag.py
+-rw-r--r--   0 root         (0) root         (0)      648 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/commit_parser/test_token.py
+-rw-r--r--   0 root         (0) root         (0)      442 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/commit_parser/test_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 19:23:09.863366 python-semantic-release-8.0.0a7/tests/unit/semantic_release/hvcs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/hvcs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1349 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/hvcs/test__base.py
+-rw-r--r--   0 root         (0) root         (0)    22874 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/hvcs/test_gitea.py
+-rw-r--r--   0 root         (0) root         (0)    24334 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/hvcs/test_github.py
+-rw-r--r--   0 root         (0) root         (0)    10021 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/hvcs/test_gitlab.py
+-rw-r--r--   0 root         (0) root         (0)      965 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/hvcs/test_token_auth.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/hvcs/test_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 19:23:09.863366 python-semantic-release-8.0.0a7/tests/unit/semantic_release/version/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/version/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7319 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/version/test_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     3715 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/version/test_declaration.py
+-rw-r--r--   0 root         (0) root         (0)     2996 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/version/test_translator.py
+-rw-r--r--   0 root         (0) root         (0)     9640 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/version/test_version.py
```

### Comparing `python-semantic-release-8.0.0a6/LICENSE` & `python-semantic-release-8.0.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/PKG-INFO` & `python-semantic-release-8.0.0a7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-semantic-release
-Version: 8.0.0a6
+Version: 8.0.0a7
 Summary: Automatic Semantic Versioning for Python projects
 Author-email: Rolf Erik Lekang <me@rolflekang.com>
 License: MIT
 Project-URL: Project Url, http://github.com/python-semantic-release/python-semantic-release
 Project-URL: Homepage, https://python-semantic-release.readthedocs.io
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `python-semantic-release-8.0.0a6/README.rst` & `python-semantic-release-8.0.0a7/README.rst`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/pyproject.toml` & `python-semantic-release-8.0.0a7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # and https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-semantic-release"
-version = "8.0.0-alpha.6"
+version = "8.0.0-alpha.7"
 description = "Automatic Semantic Versioning for Python projects"
 requires-python = ">=3.7"
 license = { text = "MIT" }
 classifiers = [
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.7",
@@ -33,24 +33,26 @@
   "pydantic>=1.10.2,<2",
   "rich>=12.5.1",
   "shellingham>=1.5.0.post1",
 ]
 
 [project.scripts]
 semantic-release = "semantic_release.cli:main"
+psr = "semantic_release.cli:main"
 
 [project.urls]
 "Project Url" = "http://github.com/python-semantic-release/python-semantic-release"
 Homepage = "https://python-semantic-release.readthedocs.io"
 
 [project.optional-dependencies]
 docs = [
   "Sphinx==5.2.3",
   "sphinxcontrib-apidoc==0.3.0",
   "sphinx-autobuild==2021.03.14",
+  "furo>=2023.5.20",
 ]
 test = [
   "coverage[toml]>=6,<7",
   "pytest>=7,<8",
   "pytest-xdist>=2,<3",
   "pytest-mock>=3,<4",
   "pytest-lazy-fixture~=0.6.3",
```

### Comparing `python-semantic-release-8.0.0a6/python_semantic_release.egg-info/PKG-INFO` & `python-semantic-release-8.0.0a7/python_semantic_release.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-semantic-release
-Version: 8.0.0a6
+Version: 8.0.0a7
 Summary: Automatic Semantic Versioning for Python projects
 Author-email: Rolf Erik Lekang <me@rolflekang.com>
 License: MIT
 Project-URL: Project Url, http://github.com/python-semantic-release/python-semantic-release
 Project-URL: Homepage, https://python-semantic-release.readthedocs.io
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `python-semantic-release-8.0.0a6/python_semantic_release.egg-info/SOURCES.txt` & `python-semantic-release-8.0.0a7/python_semantic_release.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 semantic_release/version/version.py
 tests/command_line/__init__.py
 tests/command_line/conftest.py
 tests/command_line/test_changelog.py
 tests/command_line/test_generate_config.py
 tests/command_line/test_help.py
 tests/command_line/test_main.py
+tests/command_line/test_publish.py
 tests/command_line/test_version.py
 tests/fixtures/__init__.py
 tests/fixtures/commit_parsers.py
 tests/fixtures/example_project.py
 tests/fixtures/git_repo.py
 tests/fixtures/scipy.py
 tests/scenario/__init__.py
```

### Comparing `python-semantic-release-8.0.0a6/python_semantic_release.egg-info/requires.txt` & `python-semantic-release-8.0.0a7/python_semantic_release.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 isort
 black
 
 [docs]
 Sphinx==5.2.3
 sphinxcontrib-apidoc==0.3.0
 sphinx-autobuild==2021.03.14
+furo>=2023.5.20
 
 [mypy]
 mypy
 types-requests
 
 [test]
 coverage[toml]<7,>=6
```

### Comparing `python-semantic-release-8.0.0a6/semantic_release/__init__.py` & `python-semantic-release-8.0.0a7/semantic_release/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from semantic_release.version import (
     Version as Version,
     VersionTranslator as VersionTranslator,
     next_version as next_version,
     tags_and_versions as tags_and_versions,
 )
 
-__version__ = "8.0.0-alpha.6"
+__version__ = "8.0.0-alpha.7"
 
 
 def setup_hook(argv: list[str]) -> None:
     """
     A hook to be used in setup.py to enable `python setup.py publish`.
 
     :param argv: sys.argv
```

### Comparing `python-semantic-release-8.0.0a6/semantic_release/changelog/context.py` & `python-semantic-release-8.0.0a7/semantic_release/changelog/context.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/semantic_release/changelog/release_history.py` & `python-semantic-release-8.0.0a7/semantic_release/changelog/release_history.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/semantic_release/changelog/template.py` & `python-semantic-release-8.0.0a7/semantic_release/changelog/template.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/semantic_release/cli/commands/changelog.py` & `python-semantic-release-8.0.0a7/semantic_release/cli/commands/changelog.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/semantic_release/cli/commands/generate_config.py` & `python-semantic-release-8.0.0a7/semantic_release/cli/commands/generate_config.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/semantic_release/cli/commands/main.py` & `python-semantic-release-8.0.0a7/semantic_release/cli/commands/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,20 +50,28 @@
     "verbosity",
     help="Set logging verbosity",
     default=0,
     count=True,
     show_default=True,
     type=click.IntRange(0, 2, clamp=True),
 )
+@click.option(
+    "--strict",
+    "strict",
+    is_flag=True,
+    default=False,
+    help="Enable strict mode",
+)
 @click.pass_context
 def main(
     ctx: click.Context,
     config_file: str = DEFAULT_CONFIG_FILE,
     verbosity: int = 0,
     noop: bool = False,
+    strict: bool = False,
 ) -> None:
     """
     Python Semantic Release
 
     Automated Semantic Versioning based on version 2.0.0 of the Semantic Versioning
     specification, which can be found at https://semver.org/spec/v2.0.0.html.
 
@@ -102,17 +110,22 @@
         ctx.fail("Not in a valid Git repository")
 
     if noop:
         rprint(
             ":shield: [bold cyan]You are running in no-operation mode, because the "
             "'--noop' flag was supplied"
         )
+
     cli_options = GlobalCommandLineOptions(
-        noop=noop, verbosity=verbosity, config_file=config_file
+        noop=noop,
+        verbosity=verbosity,
+        config_file=config_file,
+        strict=strict,
     )
+    log.debug("global cli options: %s", cli_options)
 
     try:
         if config_file.endswith(".toml"):
             log.info(f"Loading TOML configuration from {config_file}")
             config_text = read_toml(config_file)
         elif config_file.endswith(".json"):
             log.info(f"Loading JSON configuration from {config_file}")
@@ -126,16 +139,19 @@
 
     raw_config = RawConfig.parse_obj(config_text)
     try:
         runtime = RuntimeContext.from_raw_config(
             raw_config, repo=repo, global_cli_options=cli_options
         )
     except NotAReleaseBranch as exc:
-        rprint(f"[bold red]{str(exc)}")
-        ctx.exit(2)
+        rprint(f"[bold {'red' if strict else 'orange1'}]{str(exc)}")
+        # If not strict, exit 0 so other processes can continue. For example, in
+        # multibranch CI it might be desirable to run a non-release branch's pipeline
+        # without specifying conditional execution of PSR based on branch name
+        ctx.exit(2 if strict else 0)
     except InvalidConfiguration as exc:
         ctx.fail(str(exc))
     ctx.obj = runtime
 
     # This allows us to mask secrets in the logging
     # by applying it to all the configured handlers
     for handler in logging.getLogger().handlers:
```

### Comparing `python-semantic-release-8.0.0a6/semantic_release/cli/commands/publish.py` & `python-semantic-release-8.0.0a7/semantic_release/cli/commands/publish.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,30 +10,37 @@
 
 @click.command(
     short_help="Publish distributions to VCS Releases",
     context_settings={
         "help_option_names": ["-h", "--help"],
     },
 )
+@click.option(
+    "--tag",
+    "tag",
+    help="The tag associated with the release to publish to",
+    default="latest",
+)
 @click.pass_context
-def publish(ctx: click.Context) -> None:
+def publish(ctx: click.Context, tag: str = "latest") -> None:
     """
     Build and publish a distribution to a VCS release.
     """
     runtime = ctx.obj
     repo = runtime.repo
     hvcs_client = runtime.hvcs_client
     translator = runtime.version_translator
     dist_glob_patterns = runtime.dist_glob_patterns
 
-    latest_tag = tags_and_versions(repo.tags, translator)[0][0]
+    if tag == "latest":
+        tag = str(tags_and_versions(repo.tags, translator)[0][0])
     if runtime.global_cli_options.noop:
         noop_report(
             "would have uploaded files matching any of the globs "
             + ", ".join(repr(g) for g in dist_glob_patterns)
             + " to a remote VCS release, if supported"
         )
         ctx.exit(0)
 
     log.info("Uploading distributions to release")
     for pattern in dist_glob_patterns:
-        hvcs_client.upload_dists(tag=latest_tag, dist_glob=pattern)
+        hvcs_client.upload_dists(tag=tag, dist_glob=pattern)
```

### Comparing `python-semantic-release-8.0.0a6/semantic_release/cli/commands/version.py` & `python-semantic-release-8.0.0a7/semantic_release/cli/commands/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,26 +168,34 @@
 )
 @click.option(
     "--build-metadata",
     "build_metadata",
     default=os.getenv("PSR_BUILD_METADATA"),
     help="Build metadata to append to the new version",
 )
+@click.option(
+    "--skip-build",
+    "skip_build",
+    default=False,
+    is_flag=True,
+    help="Skip building the current project",
+)
 @click.pass_context
 def version(
     ctx: click.Context,
     print_only: bool = False,
     force_prerelease: bool = False,
     prerelease_token: str | None = None,
     force_level: str | None = None,
     commit_changes: bool = True,
     update_changelog: bool = True,
     push_changes: bool = True,
     make_vcs_release: bool = True,
     build_metadata: str | None = None,
+    skip_build: bool = False,
 ) -> str:
     """
     Detect the semantically correct next version that should be applied to your
     project.
 
     \b
     By default:
@@ -274,22 +282,32 @@
         )
 
     if build_metadata:
         new_version.build_metadata = build_metadata
 
     gha_output.released = False
     gha_output.version = new_version
-    # If the new version has already been released, we fail and abort
+
+    # Print the new version so that command-line output capture will work
+    click.echo(str(new_version))
+
+    # If the new version has already been released, we fail and abort if strict;
+    # otherwise we exit with 0.
     if new_version in {v for _, v in tags_and_versions(repo.tags, translator)}:
-        ctx.fail(
-            f"No release will be made, {str(new_version)} has already been released!"
-        )
+        if opts.strict:
+            ctx.fail(
+                f"No release will be made, {str(new_version)} has already been released!"
+            )
+        else:
+            rprint(
+                f"[bold orange1]No release will be made, {str(new_version)} has already been released!"
+            )
+            ctx.exit(0)
 
     if print_only:
-        click.echo(str(new_version))
         ctx.exit(0)
 
     rprint(
         f"[bold green]The next version is: [white]{str(new_version)}[/white]! :rocket:"
     )
 
     files_with_new_version_written = apply_version_to_source_files(
@@ -298,17 +316,19 @@
         version=new_version,
         noop=opts.noop,
     )
     all_paths_to_add = files_with_new_version_written + (assets or [])
 
     # Build distributions before committing any changes - this way if the
     # build fails, modifications to the source code won't be committed
-    if not build_command:
+    if skip_build:
+        rprint("[bold orange1]Skipping build due to --skip-build flag")
+    elif not build_command:
         rprint("[green]No build command specified, skipping")
-    if runtime.global_cli_options.noop:
+    elif runtime.global_cli_options.noop:
         noop_report(f"would have run the build_command {build_command}")
     else:
         try:
             log.info("Running build command %s", build_command)
             rprint(
                 f"[bold green]:hammer_and_wrench: Running build command: {build_command}"
             )
```

### Comparing `python-semantic-release-8.0.0a6/semantic_release/cli/common.py` & `python-semantic-release-8.0.0a7/semantic_release/cli/common.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/semantic_release/cli/config.py` & `python-semantic-release-8.0.0a7/semantic_release/cli/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,14 +167,15 @@
     A dataclass to hold all the command line options that
     should be set in the RuntimeContext
     """
 
     noop: bool = False
     verbosity: int = 0
     config_file: str = DEFAULT_CONFIG_FILE
+    strict: bool = False
 
 
 ######
 # RuntimeContext
 ######
 # This is what we want to attach to `click.Context.obj`
 # There are currently no defaults here - this is on purpose,
```

### Comparing `python-semantic-release-8.0.0a6/semantic_release/cli/github_actions_output.py` & `python-semantic-release-8.0.0a7/semantic_release/cli/github_actions_output.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/semantic_release/cli/masking_filter.py` & `python-semantic-release-8.0.0a7/semantic_release/cli/masking_filter.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/semantic_release/cli/util.py` & `python-semantic-release-8.0.0a7/semantic_release/cli/util.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/semantic_release/commit_parser/__init__.py` & `python-semantic-release-8.0.0a7/semantic_release/commit_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/semantic_release/commit_parser/_base.py` & `python-semantic-release-8.0.0a7/semantic_release/commit_parser/_base.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/semantic_release/commit_parser/angular.py` & `python-semantic-release-8.0.0a7/semantic_release/commit_parser/angular.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/semantic_release/commit_parser/emoji.py` & `python-semantic-release-8.0.0a7/semantic_release/commit_parser/emoji.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/semantic_release/commit_parser/scipy.py` & `python-semantic-release-8.0.0a7/semantic_release/commit_parser/scipy.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/semantic_release/commit_parser/tag.py` & `python-semantic-release-8.0.0a7/semantic_release/commit_parser/tag.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/semantic_release/commit_parser/token.py` & `python-semantic-release-8.0.0a7/semantic_release/commit_parser/token.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/semantic_release/commit_parser/util.py` & `python-semantic-release-8.0.0a7/semantic_release/commit_parser/util.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/semantic_release/const.py` & `python-semantic-release-8.0.0a7/semantic_release/const.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/semantic_release/data/templates/CHANGELOG.md.j2` & `python-semantic-release-8.0.0a7/semantic_release/data/templates/CHANGELOG.md.j2`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/semantic_release/enums.py` & `python-semantic-release-8.0.0a7/semantic_release/enums.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/semantic_release/errors.py` & `python-semantic-release-8.0.0a7/semantic_release/errors.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/semantic_release/helpers.py` & `python-semantic-release-8.0.0a7/semantic_release/helpers.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/semantic_release/hvcs/_base.py` & `python-semantic-release-8.0.0a7/semantic_release/hvcs/_base.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/semantic_release/hvcs/gitea.py` & `python-semantic-release-8.0.0a7/semantic_release/hvcs/gitea.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/semantic_release/hvcs/github.py` & `python-semantic-release-8.0.0a7/semantic_release/hvcs/github.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/semantic_release/hvcs/gitlab.py` & `python-semantic-release-8.0.0a7/semantic_release/hvcs/gitlab.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/semantic_release/hvcs/token_auth.py` & `python-semantic-release-8.0.0a7/semantic_release/hvcs/token_auth.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/semantic_release/hvcs/util.py` & `python-semantic-release-8.0.0a7/semantic_release/hvcs/util.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/semantic_release/version/algorithm.py` & `python-semantic-release-8.0.0a7/semantic_release/version/algorithm.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/semantic_release/version/declaration.py` & `python-semantic-release-8.0.0a7/semantic_release/version/declaration.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/semantic_release/version/translator.py` & `python-semantic-release-8.0.0a7/semantic_release/version/translator.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/semantic_release/version/version.py` & `python-semantic-release-8.0.0a7/semantic_release/version/version.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/tests/command_line/test_changelog.py` & `python-semantic-release-8.0.0a7/tests/command_line/test_changelog.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/tests/command_line/test_generate_config.py` & `python-semantic-release-8.0.0a7/tests/command_line/test_generate_config.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/tests/command_line/test_help.py` & `python-semantic-release-8.0.0a7/tests/command_line/test_help.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/tests/command_line/test_version.py` & `python-semantic-release-8.0.0a7/tests/command_line/test_version.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
 import difflib
 import filecmp
 import re
-import shlex
 import shutil
 from subprocess import CompletedProcess
 from unittest import mock
 
 import pytest
 import tomlkit
 from pytest_lazyfixture import lazy_fixture
@@ -236,15 +235,15 @@
         lazy_fixture("repo_with_git_flow_and_release_channels_angular_commits"),
     ],
 )
 def test_version_already_released_no_push(repo, cli_runner):
     # In these tests, unless arguments are supplied then the latest version
     # has already been released, so we expect an exit code of 2 with the message
     # to indicate that no release will be made
-    result = cli_runner.invoke(main, [version.name, "--no-push"])
+    result = cli_runner.invoke(main, ["--strict", version.name, "--no-push"])
     assert result.exit_code == 2
     assert "no release will be made" in result.output.lower()
 
 
 @pytest.mark.parametrize(
     "repo, cli_args, expected_new_version",
     [
@@ -437,188 +436,28 @@
     removed = [line[2:] for line in diff if line.startswith("- ")]
 
     assert len(removed) == 1 and re.match('__version__ = ".*"', removed[0])
     assert added == [f'__version__ = "{expected_new_version}"\n']
 
 
 @pytest.mark.parametrize(
-    "repo, cli_args, expected_stdout",
-    [
-        *[
-            (
-                lazy_fixture("repo_with_no_tags_angular_commits"),
-                cli_args,
-                expected_stdout,
-            )
-            for cli_args, expected_stdout in (
-                ([], "0.1.0"),
-                (["--build-metadata", "build.12345"], "0.1.0+build.12345"),
-                (["--patch"], "0.0.1"),
-                (["--minor"], "0.1.0"),
-                (["--major"], "1.0.0"),
-                (["--patch", "--prerelease"], "0.0.1-rc.1"),
-                (["--minor", "--prerelease"], "0.1.0-rc.1"),
-                (["--major", "--prerelease"], "1.0.0-rc.1"),
-                (
-                    ["--patch", "--prerelease", "--prerelease-token", "beta"],
-                    "0.0.1-beta.1",
-                ),
-            )
-        ],
-        *[
-            (
-                lazy_fixture("repo_with_single_branch_angular_commits"),
-                cli_args,
-                expected_stdout,
-            )
-            for cli_args, expected_stdout in (
-                ([], "0.1.2"),
-                (["--build-metadata", "build.12345"], "0.1.2+build.12345"),
-                (["--patch"], "0.1.2"),
-                (["--minor"], "0.2.0"),
-                (["--major"], "1.0.0"),
-                (["--patch", "--prerelease"], "0.1.2-rc.1"),
-                (["--minor", "--prerelease"], "0.2.0-rc.1"),
-                (["--major", "--prerelease"], "1.0.0-rc.1"),
-                (
-                    ["--patch", "--prerelease", "--prerelease-token", "beta"],
-                    "0.1.2-beta.1",
-                ),
-            )
-        ],
-        *[
-            (
-                lazy_fixture("repo_with_single_branch_and_prereleases_angular_commits"),
-                cli_args,
-                expected_stdout,
-            )
-            for cli_args, expected_stdout in (
-                ([], "0.2.1"),
-                (["--build-metadata", "build.12345"], "0.2.1+build.12345"),
-                (["--patch"], "0.2.1"),
-                (["--minor"], "0.3.0"),
-                (["--major"], "1.0.0"),
-                (["--patch", "--prerelease"], "0.2.1-rc.1"),
-                (["--minor", "--prerelease"], "0.3.0-rc.1"),
-                (["--major", "--prerelease"], "1.0.0-rc.1"),
-                (
-                    ["--patch", "--prerelease", "--prerelease-token", "beta"],
-                    "0.2.1-beta.1",
-                ),
-            )
-        ],
-        *[
-            (
-                lazy_fixture("repo_with_main_and_feature_branches_angular_commits"),
-                cli_args,
-                expected_stdout,
-            )
-            for cli_args, expected_stdout in (
-                ([], "0.3.0-beta.2"),
-                (["--build-metadata", "build.12345"], "0.3.0-beta.2+build.12345"),
-                (["--patch"], "0.3.1"),
-                (["--minor"], "0.4.0"),
-                (["--major"], "1.0.0"),
-                (["--patch", "--prerelease"], "0.3.1-beta.1"),
-                (["--minor", "--prerelease"], "0.4.0-beta.1"),
-                (["--major", "--prerelease"], "1.0.0-beta.1"),
-                (
-                    ["--patch", "--prerelease", "--prerelease-token", "beta"],
-                    "0.3.1-beta.1",
-                ),
-            )
-        ],
-        *[
-            (
-                lazy_fixture("repo_with_git_flow_angular_commits"),
-                cli_args,
-                expected_stdout,
-            )
-            for cli_args, expected_stdout in (
-                ([], "1.2.0-alpha.3"),
-                (["--build-metadata", "build.12345"], "1.2.0-alpha.3+build.12345"),
-                (["--patch"], "1.2.1"),
-                (["--minor"], "1.3.0"),
-                (["--major"], "2.0.0"),
-                (["--patch", "--prerelease"], "1.2.1-alpha.1"),
-                (["--minor", "--prerelease"], "1.3.0-alpha.1"),
-                (["--major", "--prerelease"], "2.0.0-alpha.1"),
-                (
-                    ["--patch", "--prerelease", "--prerelease-token", "beta"],
-                    "1.2.1-beta.1",
-                ),
-            )
-        ],
-        *[
-            (
-                lazy_fixture("repo_with_git_flow_and_release_channels_angular_commits"),
-                cli_args,
-                expected_stdout,
-            )
-            for cli_args, expected_stdout in (
-                ([], "1.1.0-alpha.4"),
-                (["--build-metadata", "build.12345"], "1.1.0-alpha.4+build.12345"),
-                (["--patch"], "1.1.1"),
-                (["--minor"], "1.2.0"),
-                (["--major"], "2.0.0"),
-                (["--patch", "--prerelease"], "1.1.1-alpha.1"),
-                (["--minor", "--prerelease"], "1.2.0-alpha.1"),
-                (["--major", "--prerelease"], "2.0.0-alpha.1"),
-                (
-                    ["--patch", "--prerelease", "--prerelease-token", "beta"],
-                    "1.1.1-beta.1",
-                ),
-            )
-        ],
-    ],
-)
-def test_version_print(
-    repo, cli_args, expected_stdout, example_project, tmp_path_factory, cli_runner
-):
-    # Make a commit to ensure we have something to release
-    # otherwise the "no release will be made" logic will kick in first
-    new_file = example_project / "temp.txt"
-    new_file.write_text("noop version test")
-
-    repo.git.add(str(new_file.resolve()))
-    repo.git.commit(m="fix: temp new file")
-
-    tempdir = tmp_path_factory.mktemp("test_version_print")
-    shutil.rmtree(str(tempdir.resolve()))
-    shutil.copytree(src=str(example_project.resolve()), dst=tempdir)
-    head_before = repo.head.commit
-    tags_before = sorted(list(repo.tags), key=lambda tag: tag.name)
-
-    result = cli_runner.invoke(main, [version.name, *cli_args, "--print"])
-
-    tags_after = sorted(list(repo.tags), key=lambda tag: tag.name)
-    head_after = repo.head.commit
-
-    assert result.exit_code == 0
-    assert tags_before == tags_after
-    assert head_before == head_after
-    assert result.output.rstrip("\n") == expected_stdout
-    dcmp = filecmp.dircmp(str(example_project.resolve()), tempdir)
-    differing_files = flatten_dircmp(dcmp)
-    assert not differing_files
-
-
-@pytest.mark.parametrize(
     "repo",
     [
         lazy_fixture("repo_with_single_branch_angular_commits"),
         lazy_fixture("repo_with_single_branch_and_prereleases_angular_commits"),
         lazy_fixture("repo_with_main_and_feature_branches_angular_commits"),
         lazy_fixture("repo_with_git_flow_angular_commits"),
         lazy_fixture("repo_with_git_flow_and_release_channels_angular_commits"),
     ],
 )
 def test_version_build_metadata_triggers_new_version(repo, cli_runner):
     # Verify we get "no version to release" without build metadata
-    no_metadata_result = cli_runner.invoke(main, [version.name, "--no-push"])
+    no_metadata_result = cli_runner.invoke(
+        main, ["--strict", version.name, "--no-push"]
+    )
     assert no_metadata_result.exit_code == 2
     assert "no release will be made" in no_metadata_result.output.lower()
 
     metadata_suffix = "build.abc-12345"
     result = cli_runner.invoke(
         main, [version.name, "--no-push", "--build-metadata", metadata_suffix]
     )
@@ -644,14 +483,28 @@
         assert result.exit_code == 0
 
         patched_subprocess_run.assert_called_once_with(
             [exe, "-c", build_command], check=True
         )
 
 
+def test_version_skips_build_command_with_skip_build(
+    repo_with_git_flow_angular_commits, cli_runner
+):
+    with mock.patch(
+        "subprocess.run", return_value=CompletedProcess(args=(), returncode=0)
+    ) as patched_subprocess_run:
+        result = cli_runner.invoke(
+            main, [version.name, "--patch", "--no-push", "--skip-build"]
+        )  # force a new version
+        assert result.exit_code == 0
+
+        patched_subprocess_run.assert_not_called()
+
+
 def test_version_writes_github_actions_output(
     repo_with_git_flow_angular_commits, cli_runner, monkeypatch, tmp_path
 ):
     mock_output_file = tmp_path / "action.out"
     monkeypatch.setenv("GITHUB_OUTPUT", str(mock_output_file.resolve()))
     result = cli_runner.invoke(main, [version.name, "--patch", "--no-push"])
     assert result.exit_code == 0
@@ -661,7 +514,20 @@
     )
     assert "released" in action_outputs
     assert action_outputs["released"] == "true"
     assert "version" in action_outputs
     assert action_outputs["version"] == "1.2.1"
     assert "tag" in action_outputs
     assert action_outputs["tag"] == "v1.2.1"
+
+
+def test_version_exit_code_when_strict(repo_with_git_flow_angular_commits, cli_runner):
+    result = cli_runner.invoke(main, ["--strict", version.name, "--no-push"])
+    assert result.exit_code != 0
+
+
+def test_version_exit_code_when_not_strict(
+    repo_with_git_flow_angular_commits, cli_runner
+):
+    # Testing "no release will be made"
+    result = cli_runner.invoke(main, [version.name, "--no-push"])
+    assert result.exit_code == 0
```

### Comparing `python-semantic-release-8.0.0a6/tests/fixtures/commit_parsers.py` & `python-semantic-release-8.0.0a7/tests/fixtures/commit_parsers.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/tests/fixtures/example_project.py` & `python-semantic-release-8.0.0a7/tests/fixtures/example_project.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/tests/fixtures/git_repo.py` & `python-semantic-release-8.0.0a7/tests/fixtures/git_repo.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/tests/fixtures/scipy.py` & `python-semantic-release-8.0.0a7/tests/fixtures/scipy.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/tests/scenario/test_next_version.py` & `python-semantic-release-8.0.0a7/tests/scenario/test_next_version.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/tests/scenario/test_release_history.py` & `python-semantic-release-8.0.0a7/tests/scenario/test_release_history.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/tests/scenario/test_template_render.py` & `python-semantic-release-8.0.0a7/tests/scenario/test_template_render.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/tests/unit/semantic_release/changelog/test_changelog_context.py` & `python-semantic-release-8.0.0a7/tests/unit/semantic_release/changelog/test_changelog_context.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/tests/unit/semantic_release/changelog/test_default_changelog.py` & `python-semantic-release-8.0.0a7/tests/unit/semantic_release/changelog/test_default_changelog.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/tests/unit/semantic_release/changelog/test_release_notes.py` & `python-semantic-release-8.0.0a7/tests/unit/semantic_release/changelog/test_release_notes.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/tests/unit/semantic_release/changelog/test_template.py` & `python-semantic-release-8.0.0a7/tests/unit/semantic_release/changelog/test_template.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/tests/unit/semantic_release/cli/test_config.py` & `python-semantic-release-8.0.0a7/tests/unit/semantic_release/cli/test_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from unittest import mock
 
 import pytest
 import tomlkit
-from git import Repo
 
 from semantic_release.cli.config import (
     GlobalCommandLineOptions,
     RawConfig,
     RuntimeContext,
 )
 from semantic_release.const import DEFAULT_COMMIT_AUTHOR
```

### Comparing `python-semantic-release-8.0.0a6/tests/unit/semantic_release/cli/test_github_actions_output.py` & `python-semantic-release-8.0.0a7/tests/unit/semantic_release/cli/test_github_actions_output.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/tests/unit/semantic_release/cli/test_masking_filter.py` & `python-semantic-release-8.0.0a7/tests/unit/semantic_release/cli/test_masking_filter.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/tests/unit/semantic_release/cli/test_version.py` & `python-semantic-release-8.0.0a7/tests/unit/semantic_release/cli/test_version.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/tests/unit/semantic_release/commit_parser/test_angular.py` & `python-semantic-release-8.0.0a7/tests/unit/semantic_release/commit_parser/test_angular.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/tests/unit/semantic_release/commit_parser/test_emoji.py` & `python-semantic-release-8.0.0a7/tests/unit/semantic_release/commit_parser/test_emoji.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/tests/unit/semantic_release/commit_parser/test_tag.py` & `python-semantic-release-8.0.0a7/tests/unit/semantic_release/commit_parser/test_tag.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/tests/unit/semantic_release/commit_parser/test_token.py` & `python-semantic-release-8.0.0a7/tests/unit/semantic_release/commit_parser/test_token.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/tests/unit/semantic_release/hvcs/test__base.py` & `python-semantic-release-8.0.0a7/tests/unit/semantic_release/hvcs/test__base.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/tests/unit/semantic_release/hvcs/test_gitea.py` & `python-semantic-release-8.0.0a7/tests/unit/semantic_release/hvcs/test_gitea.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/tests/unit/semantic_release/hvcs/test_github.py` & `python-semantic-release-8.0.0a7/tests/unit/semantic_release/hvcs/test_github.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/tests/unit/semantic_release/hvcs/test_gitlab.py` & `python-semantic-release-8.0.0a7/tests/unit/semantic_release/hvcs/test_gitlab.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/tests/unit/semantic_release/hvcs/test_token_auth.py` & `python-semantic-release-8.0.0a7/tests/unit/semantic_release/hvcs/test_token_auth.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/tests/unit/semantic_release/version/test_algorithm.py` & `python-semantic-release-8.0.0a7/tests/unit/semantic_release/version/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/tests/unit/semantic_release/version/test_declaration.py` & `python-semantic-release-8.0.0a7/tests/unit/semantic_release/version/test_declaration.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/tests/unit/semantic_release/version/test_translator.py` & `python-semantic-release-8.0.0a7/tests/unit/semantic_release/version/test_translator.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a6/tests/unit/semantic_release/version/test_version.py` & `python-semantic-release-8.0.0a7/tests/unit/semantic_release/version/test_version.py`

 * *Files identical despite different names*

