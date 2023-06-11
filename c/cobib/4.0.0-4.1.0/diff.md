# Comparing `tmp/cobib-4.0.0.tar.gz` & `tmp/cobib-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cobib-4.0.0.tar", last modified: Sat May 20 14:28:46 2023, max compression
+gzip compressed data, was "cobib-4.1.0.tar", last modified: Sun Jun 11 11:20:21 2023, max compression
```

## Comparing `cobib-4.0.0.tar` & `cobib-4.1.0.tar`

### file list

```diff
@@ -1,178 +1,180 @@
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-20 14:28:46.008988 cobib-4.0.0/
--rw-r--r--   0 max       (1000) max       (1000)      217 2021-09-20 21:31:31.000000 cobib-4.0.0/.coveragerc
--rw-r--r--   0 max       (1000) max       (1000)      268 2023-04-15 10:28:42.000000 cobib-4.0.0/.gitignore
--rw-r--r--   0 max       (1000) max       (1000)     2718 2023-04-15 20:38:04.000000 cobib-4.0.0/.gitlab-ci.yml
--rw-r--r--   0 max       (1000) max       (1000)       75 2023-05-14 13:30:20.000000 cobib-4.0.0/.pydocstylerc
--rw-r--r--   0 max       (1000) max       (1000)      888 2023-05-20 12:00:53.000000 cobib-4.0.0/.pylintdict
--rw-r--r--   0 max       (1000) max       (1000)    11236 2023-04-15 10:28:42.000000 cobib-4.0.0/.pylintrc
--rw-r--r--   0 max       (1000) max       (1000)    28312 2023-05-20 14:26:11.000000 cobib-4.0.0/CHANGELOG.md
--rw-r--r--   0 max       (1000) max       (1000)     2247 2023-05-01 17:07:35.000000 cobib-4.0.0/CONTRIBUTING.md
--rw-r--r--   0 max       (1000) max       (1000)     1076 2023-04-28 18:20:00.000000 cobib-4.0.0/LICENSE.txt
--rw-r--r--   0 max       (1000) max       (1000)      115 2021-09-20 21:31:31.000000 cobib-4.0.0/MANIFEST.in
--rw-r--r--   0 max       (1000) max       (1000)      187 2021-09-20 21:31:31.000000 cobib-4.0.0/Makefile
--rw-r--r--   0 max       (1000) max       (1000)    37193 2023-05-20 14:28:46.008988 cobib-4.0.0/PKG-INFO
--rw-r--r--   0 max       (1000) max       (1000)     7871 2023-05-20 12:00:53.000000 cobib-4.0.0/README.md
--rw-r--r--   0 max       (1000) max       (1000)      563 2021-09-20 21:31:31.000000 cobib-4.0.0/_cobib
--rw-r--r--   0 max       (1000) max       (1000)    24744 2023-05-20 14:26:50.000000 cobib-4.0.0/cobib.1
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-20 14:28:45.972322 cobib-4.0.0/html/
--rw-r--r--   0 max       (1000) max       (1000)    34915 2023-05-07 10:49:25.000000 cobib-4.0.0/html/cobib_book.svg
--rw-r--r--   0 max       (1000) max       (1000)    61955 2023-05-07 10:49:25.000000 cobib-4.0.0/html/cobib_logo.svg
--rw-r--r--   0 max       (1000) max       (1000)      554 2023-05-07 10:49:25.000000 cobib-4.0.0/html/index.html.jinja2
--rw-r--r--   0 max       (1000) max       (1000)      398 2023-05-07 10:49:25.000000 cobib-4.0.0/html/module.html.jinja2
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-20 14:28:45.972322 cobib-4.0.0/logo/
--rw-r--r--   0 max       (1000) max       (1000)    44669 2021-09-20 21:31:31.000000 cobib-4.0.0/logo/cobib_book-squared.png
--rw-r--r--   0 max       (1000) max       (1000)    40896 2021-09-20 21:31:31.000000 cobib-4.0.0/logo/cobib_book.png
--rw-r--r--   0 max       (1000) max       (1000)    34915 2021-09-20 21:31:31.000000 cobib-4.0.0/logo/cobib_book.svg
--rw-r--r--   0 max       (1000) max       (1000)    74851 2021-09-20 21:31:31.000000 cobib-4.0.0/logo/cobib_byline.png
--rw-r--r--   0 max       (1000) max       (1000)    27555 2021-09-20 21:31:31.000000 cobib-4.0.0/logo/cobib_byline.svg
--rw-r--r--   0 max       (1000) max       (1000)   126027 2021-09-20 21:31:31.000000 cobib-4.0.0/logo/cobib_logo.png
--rw-r--r--   0 max       (1000) max       (1000)    61955 2021-09-20 21:31:31.000000 cobib-4.0.0/logo/cobib_logo.svg
--rw-r--r--   0 max       (1000) max       (1000)      507 2023-04-15 20:38:04.000000 cobib-4.0.0/mypy.ini
--rw-r--r--   0 max       (1000) max       (1000)      356 2023-04-15 20:14:50.000000 cobib-4.0.0/pyproject.toml
--rw-r--r--   0 max       (1000) max       (1000)       27 2021-09-20 21:31:31.000000 cobib-4.0.0/pytest.ini
--rw-r--r--   0 max       (1000) max       (1000)      115 2023-05-14 13:30:20.000000 cobib-4.0.0/requirements.txt
--rw-r--r--   0 max       (1000) max       (1000)     1221 2023-05-20 14:28:46.012322 cobib-4.0.0/setup.cfg
--rw-r--r--   0 max       (1000) max       (1000)      296 2021-09-20 21:31:31.000000 cobib-4.0.0/setup.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-20 14:28:45.958988 cobib-4.0.0/src/
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-20 14:28:45.975655 cobib-4.0.0/src/cobib/
--rw-r--r--   0 max       (1000) max       (1000)      474 2023-05-20 14:27:06.000000 cobib-4.0.0/src/cobib/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)      648 2023-05-20 12:00:53.000000 cobib-4.0.0/src/cobib/__main__.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-20 14:28:45.978988 cobib-4.0.0/src/cobib/commands/
--rw-r--r--   0 max       (1000) max       (1000)      903 2023-05-20 12:00:53.000000 cobib-4.0.0/src/cobib/commands/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)    20549 2023-05-14 19:24:23.000000 cobib-4.0.0/src/cobib/commands/add.py
--rw-r--r--   0 max       (1000) max       (1000)     7832 2023-05-20 13:33:32.000000 cobib-4.0.0/src/cobib/commands/base_command.py
--rw-r--r--   0 max       (1000) max       (1000)     2983 2023-05-14 13:30:20.000000 cobib-4.0.0/src/cobib/commands/delete.py
--rw-r--r--   0 max       (1000) max       (1000)     6675 2023-05-14 13:30:20.000000 cobib-4.0.0/src/cobib/commands/edit.py
--rw-r--r--   0 max       (1000) max       (1000)     7740 2023-05-20 13:36:34.000000 cobib-4.0.0/src/cobib/commands/export.py
--rw-r--r--   0 max       (1000) max       (1000)     6083 2023-05-14 20:12:11.000000 cobib-4.0.0/src/cobib/commands/import_.py
--rw-r--r--   0 max       (1000) max       (1000)     4786 2023-05-14 13:30:20.000000 cobib-4.0.0/src/cobib/commands/init.py
--rw-r--r--   0 max       (1000) max       (1000)    12093 2023-05-20 13:30:05.000000 cobib-4.0.0/src/cobib/commands/list_.py
--rw-r--r--   0 max       (1000) max       (1000)    16872 2023-05-20 13:36:20.000000 cobib-4.0.0/src/cobib/commands/modify.py
--rw-r--r--   0 max       (1000) max       (1000)     9080 2023-05-14 13:30:20.000000 cobib-4.0.0/src/cobib/commands/open.py
--rw-r--r--   0 max       (1000) max       (1000)     4772 2023-05-14 13:30:20.000000 cobib-4.0.0/src/cobib/commands/redo.py
--rw-r--r--   0 max       (1000) max       (1000)     9070 2023-05-20 13:40:05.000000 cobib-4.0.0/src/cobib/commands/search.py
--rw-r--r--   0 max       (1000) max       (1000)     2369 2023-05-14 13:30:20.000000 cobib-4.0.0/src/cobib/commands/show.py
--rw-r--r--   0 max       (1000) max       (1000)     5469 2023-05-14 13:30:20.000000 cobib-4.0.0/src/cobib/commands/undo.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-20 14:28:45.978988 cobib-4.0.0/src/cobib/config/
--rw-r--r--   0 max       (1000) max       (1000)     1210 2022-01-13 20:47:42.000000 cobib-4.0.0/src/cobib/config/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)    23787 2023-05-14 13:30:20.000000 cobib-4.0.0/src/cobib/config/config.py
--rw-r--r--   0 max       (1000) max       (1000)    29728 2023-05-15 16:25:02.000000 cobib-4.0.0/src/cobib/config/event.py
--rw-r--r--   0 max       (1000) max       (1000)     8140 2023-05-11 19:09:33.000000 cobib-4.0.0/src/cobib/config/example.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-20 14:28:45.982322 cobib-4.0.0/src/cobib/database/
--rw-r--r--   0 max       (1000) max       (1000)      283 2021-09-20 21:31:31.000000 cobib-4.0.0/src/cobib/database/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     9818 2023-05-11 19:09:33.000000 cobib-4.0.0/src/cobib/database/database.py
--rw-r--r--   0 max       (1000) max       (1000)    17670 2023-05-14 13:30:20.000000 cobib-4.0.0/src/cobib/database/entry.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-20 14:28:45.982322 cobib-4.0.0/src/cobib/importers/
--rw-r--r--   0 max       (1000) max       (1000)      275 2021-12-01 20:44:34.000000 cobib-4.0.0/src/cobib/importers/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     3086 2023-05-20 12:00:53.000000 cobib-4.0.0/src/cobib/importers/base_importer.py
--rw-r--r--   0 max       (1000) max       (1000)    12858 2023-05-20 12:00:53.000000 cobib-4.0.0/src/cobib/importers/zotero.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-20 14:28:45.985655 cobib-4.0.0/src/cobib/parsers/
--rw-r--r--   0 max       (1000) max       (1000)      520 2021-09-25 22:36:09.000000 cobib-4.0.0/src/cobib/parsers/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     5039 2023-05-14 13:30:20.000000 cobib-4.0.0/src/cobib/parsers/arxiv.py
--rw-r--r--   0 max       (1000) max       (1000)     2053 2021-09-20 21:31:31.000000 cobib-4.0.0/src/cobib/parsers/base_parser.py
--rw-r--r--   0 max       (1000) max       (1000)     2994 2023-05-14 13:30:20.000000 cobib-4.0.0/src/cobib/parsers/bibtex.py
--rw-r--r--   0 max       (1000) max       (1000)     3267 2023-05-14 13:30:20.000000 cobib-4.0.0/src/cobib/parsers/doi.py
--rw-r--r--   0 max       (1000) max       (1000)     4559 2023-05-14 13:30:20.000000 cobib-4.0.0/src/cobib/parsers/isbn.py
--rw-r--r--   0 max       (1000) max       (1000)     3522 2023-05-14 13:30:20.000000 cobib-4.0.0/src/cobib/parsers/url.py
--rw-r--r--   0 max       (1000) max       (1000)     2996 2023-05-14 13:30:20.000000 cobib-4.0.0/src/cobib/parsers/yaml.py
--rw-r--r--   0 max       (1000) max       (1000)        0 2021-09-20 21:31:31.000000 cobib-4.0.0/src/cobib/py.typed
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-20 14:28:45.985655 cobib-4.0.0/src/cobib/ui/
--rw-r--r--   0 max       (1000) max       (1000)      611 2023-05-20 12:00:53.000000 cobib-4.0.0/src/cobib/ui/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     3395 2023-05-20 12:00:53.000000 cobib-4.0.0/src/cobib/ui/cli.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-20 14:28:45.988988 cobib-4.0.0/src/cobib/ui/components/
--rw-r--r--   0 max       (1000) max       (1000)      991 2023-05-20 12:00:53.000000 cobib-4.0.0/src/cobib/ui/components/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     1448 2023-05-20 12:00:53.000000 cobib-4.0.0/src/cobib/ui/components/argument_parser.py
--rw-r--r--   0 max       (1000) max       (1000)      963 2023-05-20 12:00:53.000000 cobib-4.0.0/src/cobib/ui/components/entry_view.py
--rw-r--r--   0 max       (1000) max       (1000)     2673 2023-05-20 12:00:53.000000 cobib-4.0.0/src/cobib/ui/components/help_popup.py
--rw-r--r--   0 max       (1000) max       (1000)     1438 2023-05-20 12:00:53.000000 cobib-4.0.0/src/cobib/ui/components/input.py
--rw-r--r--   0 max       (1000) max       (1000)     1173 2023-05-20 12:00:53.000000 cobib-4.0.0/src/cobib/ui/components/main_view.py
--rw-r--r--   0 max       (1000) max       (1000)     2035 2023-05-20 12:00:53.000000 cobib-4.0.0/src/cobib/ui/components/popup.py
--rw-r--r--   0 max       (1000) max       (1000)     1405 2023-05-20 12:00:53.000000 cobib-4.0.0/src/cobib/ui/components/popup_logging_handler.py
--rw-r--r--   0 max       (1000) max       (1000)      668 2023-05-20 12:00:53.000000 cobib-4.0.0/src/cobib/ui/components/popup_panel.py
--rw-r--r--   0 max       (1000) max       (1000)     1082 2023-05-20 12:00:53.000000 cobib-4.0.0/src/cobib/ui/components/progress.py
--rw-r--r--   0 max       (1000) max       (1000)     3482 2023-05-20 12:00:53.000000 cobib-4.0.0/src/cobib/ui/components/prompt.py
--rw-r--r--   0 max       (1000) max       (1000)     1415 2023-05-20 12:00:53.000000 cobib-4.0.0/src/cobib/ui/components/selection_filter.py
--rw-r--r--   0 max       (1000) max       (1000)     1733 2023-05-20 12:00:53.000000 cobib-4.0.0/src/cobib/ui/shell_helper.py
--rw-r--r--   0 max       (1000) max       (1000)    20649 2023-05-20 12:00:53.000000 cobib-4.0.0/src/cobib/ui/tui.py
--rw-r--r--   0 max       (1000) max       (1000)     4273 2023-05-20 12:00:53.000000 cobib-4.0.0/src/cobib/ui/ui.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-20 14:28:45.992322 cobib-4.0.0/src/cobib/utils/
--rw-r--r--   0 max       (1000) max       (1000)      242 2021-09-20 21:31:31.000000 cobib-4.0.0/src/cobib/utils/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     6731 2023-05-14 19:24:23.000000 cobib-4.0.0/src/cobib/utils/diff_renderer.py
--rw-r--r--   0 max       (1000) max       (1000)     8653 2023-05-14 19:24:23.000000 cobib-4.0.0/src/cobib/utils/file_downloader.py
--rw-r--r--   0 max       (1000) max       (1000)     4533 2021-09-20 21:32:23.000000 cobib-4.0.0/src/cobib/utils/journal_abbreviations.py
--rw-r--r--   0 max       (1000) max       (1000)     5128 2023-05-14 13:30:20.000000 cobib-4.0.0/src/cobib/utils/logging.py
--rw-r--r--   0 max       (1000) max       (1000)     1837 2021-09-20 21:31:31.000000 cobib-4.0.0/src/cobib/utils/rel_path.py
--rw-r--r--   0 max       (1000) max       (1000)     8212 2023-05-14 13:30:20.000000 cobib-4.0.0/src/cobib/utils/shell_helper.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-20 14:28:45.975655 cobib-4.0.0/src/cobib.egg-info/
--rw-r--r--   0 max       (1000) max       (1000)    37193 2023-05-20 14:28:45.000000 cobib-4.0.0/src/cobib.egg-info/PKG-INFO
--rw-r--r--   0 max       (1000) max       (1000)     4226 2023-05-20 14:28:45.000000 cobib-4.0.0/src/cobib.egg-info/SOURCES.txt
--rw-r--r--   0 max       (1000) max       (1000)        1 2023-05-20 14:28:45.000000 cobib-4.0.0/src/cobib.egg-info/dependency_links.txt
--rw-r--r--   0 max       (1000) max       (1000)       47 2023-05-20 14:28:45.000000 cobib-4.0.0/src/cobib.egg-info/entry_points.txt
--rw-r--r--   0 max       (1000) max       (1000)      115 2023-05-20 14:28:45.000000 cobib-4.0.0/src/cobib.egg-info/requires.txt
--rw-r--r--   0 max       (1000) max       (1000)        6 2023-05-20 14:28:45.000000 cobib-4.0.0/src/cobib.egg-info/top_level.txt
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-20 14:28:45.995655 cobib-4.0.0/tests/
--rw-r--r--   0 max       (1000) max       (1000)     1508 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)      872 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/cmdline_test.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-20 14:28:46.002322 cobib-4.0.0/tests/commands/
--rw-r--r--   0 max       (1000) max       (1000)       68 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/commands/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     5831 2023-05-14 13:30:20.000000 cobib-4.0.0/tests/commands/command_test.py
--rw-r--r--   0 max       (1000) max       (1000)      248 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/commands/example_duplicate_entry.bib
--rw-r--r--   0 max       (1000) max       (1000)      261 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/commands/example_duplicate_entry.yaml
--rw-r--r--   0 max       (1000) max       (1000)      134 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/commands/example_multi_file_entry.bib
--rw-r--r--   0 max       (1000) max       (1000)      155 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/commands/example_multi_file_entry.yaml
--rw-r--r--   0 max       (1000) max       (1000)    24929 2023-05-14 13:30:20.000000 cobib-4.0.0/tests/commands/test_add.py
--rw-r--r--   0 max       (1000) max       (1000)     6251 2023-05-14 13:30:20.000000 cobib-4.0.0/tests/commands/test_delete.py
--rw-r--r--   0 max       (1000) max       (1000)     7555 2023-05-14 13:30:20.000000 cobib-4.0.0/tests/commands/test_edit.py
--rw-r--r--   0 max       (1000) max       (1000)     8218 2023-05-14 13:30:20.000000 cobib-4.0.0/tests/commands/test_export.py
--rw-r--r--   0 max       (1000) max       (1000)     3058 2023-05-14 13:30:20.000000 cobib-4.0.0/tests/commands/test_git_commit_event.py
--rw-r--r--   0 max       (1000) max       (1000)     2167 2023-05-14 19:24:23.000000 cobib-4.0.0/tests/commands/test_import.py
--rw-r--r--   0 max       (1000) max       (1000)     6102 2023-05-14 13:30:20.000000 cobib-4.0.0/tests/commands/test_init.py
--rw-r--r--   0 max       (1000) max       (1000)     9171 2023-05-14 13:30:20.000000 cobib-4.0.0/tests/commands/test_list.py
--rw-r--r--   0 max       (1000) max       (1000)     8757 2023-05-14 13:30:20.000000 cobib-4.0.0/tests/commands/test_modify.py
--rw-r--r--   0 max       (1000) max       (1000)    14520 2023-05-14 13:30:20.000000 cobib-4.0.0/tests/commands/test_open.py
--rw-r--r--   0 max       (1000) max       (1000)     8550 2023-05-14 13:30:20.000000 cobib-4.0.0/tests/commands/test_redo.py
--rw-r--r--   0 max       (1000) max       (1000)     7131 2023-05-20 13:40:09.000000 cobib-4.0.0/tests/commands/test_search.py
--rw-r--r--   0 max       (1000) max       (1000)     4232 2023-05-14 13:30:20.000000 cobib-4.0.0/tests/commands/test_show.py
--rw-r--r--   0 max       (1000) max       (1000)     7831 2023-05-14 13:30:20.000000 cobib-4.0.0/tests/commands/test_undo.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-20 14:28:46.002322 cobib-4.0.0/tests/config/
--rw-r--r--   0 max       (1000) max       (1000)       28 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/config/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)      147 2023-05-11 19:09:33.000000 cobib-4.0.0/tests/config/broken_config.py
--rw-r--r--   0 max       (1000) max       (1000)     3312 2023-05-11 19:09:33.000000 cobib-4.0.0/tests/config/test_config.py
--rw-r--r--   0 max       (1000) max       (1000)     2401 2023-05-11 19:09:33.000000 cobib-4.0.0/tests/config/test_event.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-20 14:28:46.002322 cobib-4.0.0/tests/database/
--rw-r--r--   0 max       (1000) max       (1000)       30 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/database/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)       59 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/database/example_entry_umlaut.bib
--rw-r--r--   0 max       (1000) max       (1000)     8136 2023-05-11 19:09:33.000000 cobib-4.0.0/tests/database/test_database.py
--rw-r--r--   0 max       (1000) max       (1000)    14623 2023-05-08 19:51:42.000000 cobib-4.0.0/tests/database/test_entry.py
--rw-r--r--   0 max       (1000) max       (1000)      444 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/debug.py
--rw-r--r--   0 max       (1000) max       (1000)      651 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/example_entry.bib
--rw-r--r--   0 max       (1000) max       (1000)      621 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/example_entry.yaml
--rw-r--r--   0 max       (1000) max       (1000)      723 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/example_literature.bib
--rw-r--r--   0 max       (1000) max       (1000)      636 2023-05-08 19:47:05.000000 cobib-4.0.0/tests/example_literature.yaml
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-20 14:28:46.005655 cobib-4.0.0/tests/importers/
--rw-r--r--   0 max       (1000) max       (1000)       71 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/importers/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)      274 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/importers/importer_test.py
--rw-r--r--   0 max       (1000) max       (1000)     4802 2023-05-14 20:12:11.000000 cobib-4.0.0/tests/importers/test_zotero.py
--rw-r--r--   0 max       (1000) max       (1000)     2609 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/importers/zotero_database.yaml
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-20 14:28:46.005655 cobib-4.0.0/tests/parsers/
--rw-r--r--   0 max       (1000) max       (1000)       65 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/parsers/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     1395 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/parsers/parser_test.py
--rw-r--r--   0 max       (1000) max       (1000)     5763 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/parsers/test_arxiv.py
--rw-r--r--   0 max       (1000) max       (1000)     3224 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/parsers/test_bibtex.py
--rw-r--r--   0 max       (1000) max       (1000)     5017 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/parsers/test_doi.py
--rw-r--r--   0 max       (1000) max       (1000)     5562 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/parsers/test_isbn.py
--rw-r--r--   0 max       (1000) max       (1000)     4374 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/parsers/test_url.py
--rw-r--r--   0 max       (1000) max       (1000)     3251 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/parsers/test_yaml.py
--rw-r--r--   0 max       (1000) max       (1000)     4353 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/test_main.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-20 14:28:46.008988 cobib-4.0.0/tests/utils/
--rw-r--r--   0 max       (1000) max       (1000)       29 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/utils/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)      172 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/utils/fixed_database.yaml
--rw-r--r--   0 max       (1000) max       (1000)      163 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/utils/linting_database.yaml
--rw-r--r--   0 max       (1000) max       (1000)     8992 2023-05-14 19:24:23.000000 cobib-4.0.0/tests/utils/test_file_downloader.py
--rw-r--r--   0 max       (1000) max       (1000)     3216 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/utils/test_journal_abbreviations.py
--rw-r--r--   0 max       (1000) max       (1000)     2990 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/utils/test_logging.py
--rw-r--r--   0 max       (1000) max       (1000)      964 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/utils/test_rel_path.py
--rw-r--r--   0 max       (1000) max       (1000)    13477 2023-05-14 13:30:20.000000 cobib-4.0.0/tests/utils/test_shell_helper.py
--rw-r--r--   0 max       (1000) max       (1000)     1909 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/utils/unified_database.yaml
--rw-r--r--   0 max       (1000) max       (1000)     1907 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/utils/unifying_database.yaml
--rw-r--r--   0 max       (1000) max       (1000)     1287 2023-05-11 19:09:33.000000 cobib-4.0.0/tox.ini
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-06-11 11:20:21.174786 cobib-4.1.0/
+-rw-r--r--   0 max       (1000) max       (1000)      217 2021-09-20 21:31:31.000000 cobib-4.1.0/.coveragerc
+-rw-r--r--   0 max       (1000) max       (1000)      268 2023-04-15 10:28:42.000000 cobib-4.1.0/.gitignore
+-rw-r--r--   0 max       (1000) max       (1000)     2718 2023-05-27 21:00:12.000000 cobib-4.1.0/.gitlab-ci.yml
+-rw-r--r--   0 max       (1000) max       (1000)       75 2023-05-27 21:00:12.000000 cobib-4.1.0/.pydocstylerc
+-rw-r--r--   0 max       (1000) max       (1000)      924 2023-06-07 20:33:04.000000 cobib-4.1.0/.pylintdict
+-rw-r--r--   0 max       (1000) max       (1000)    11236 2023-04-15 10:28:42.000000 cobib-4.1.0/.pylintrc
+-rw-r--r--   0 max       (1000) max       (1000)    31219 2023-06-11 11:18:49.000000 cobib-4.1.0/CHANGELOG.md
+-rw-r--r--   0 max       (1000) max       (1000)     2247 2023-05-27 21:00:12.000000 cobib-4.1.0/CONTRIBUTING.md
+-rw-r--r--   0 max       (1000) max       (1000)     1076 2023-05-27 21:00:12.000000 cobib-4.1.0/LICENSE.txt
+-rw-r--r--   0 max       (1000) max       (1000)      100 2023-05-27 21:00:12.000000 cobib-4.1.0/MANIFEST.in
+-rw-r--r--   0 max       (1000) max       (1000)      105 2023-05-27 21:00:12.000000 cobib-4.1.0/Makefile
+-rw-r--r--   0 max       (1000) max       (1000)    40072 2023-06-11 11:20:21.174786 cobib-4.1.0/PKG-INFO
+-rw-r--r--   0 max       (1000) max       (1000)     7843 2023-05-27 21:00:12.000000 cobib-4.1.0/README.md
+-rw-r--r--   0 max       (1000) max       (1000)    27762 2023-06-11 11:18:21.000000 cobib-4.1.0/cobib.1
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-06-11 11:20:21.131452 cobib-4.1.0/html/
+-rw-r--r--   0 max       (1000) max       (1000)    34915 2023-05-07 10:49:25.000000 cobib-4.1.0/html/cobib_book.svg
+-rw-r--r--   0 max       (1000) max       (1000)    61955 2023-05-07 10:49:25.000000 cobib-4.1.0/html/cobib_logo.svg
+-rw-r--r--   0 max       (1000) max       (1000)      554 2023-05-27 21:00:12.000000 cobib-4.1.0/html/index.html.jinja2
+-rw-r--r--   0 max       (1000) max       (1000)      398 2023-05-20 15:19:20.000000 cobib-4.1.0/html/module.html.jinja2
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-06-11 11:20:21.134786 cobib-4.1.0/logo/
+-rw-r--r--   0 max       (1000) max       (1000)    44669 2021-09-20 21:31:31.000000 cobib-4.1.0/logo/cobib_book-squared.png
+-rw-r--r--   0 max       (1000) max       (1000)    40896 2021-09-20 21:31:31.000000 cobib-4.1.0/logo/cobib_book.png
+-rw-r--r--   0 max       (1000) max       (1000)    34915 2021-09-20 21:31:31.000000 cobib-4.1.0/logo/cobib_book.svg
+-rw-r--r--   0 max       (1000) max       (1000)    74851 2021-09-20 21:31:31.000000 cobib-4.1.0/logo/cobib_byline.png
+-rw-r--r--   0 max       (1000) max       (1000)    27555 2021-09-20 21:31:31.000000 cobib-4.1.0/logo/cobib_byline.svg
+-rw-r--r--   0 max       (1000) max       (1000)   126027 2021-09-20 21:31:31.000000 cobib-4.1.0/logo/cobib_logo.png
+-rw-r--r--   0 max       (1000) max       (1000)    61955 2021-09-20 21:31:31.000000 cobib-4.1.0/logo/cobib_logo.svg
+-rw-r--r--   0 max       (1000) max       (1000)      507 2023-05-27 21:00:12.000000 cobib-4.1.0/mypy.ini
+-rw-r--r--   0 max       (1000) max       (1000)      356 2023-05-27 21:00:12.000000 cobib-4.1.0/pyproject.toml
+-rw-r--r--   0 max       (1000) max       (1000)       27 2021-09-20 21:31:31.000000 cobib-4.1.0/pytest.ini
+-rw-r--r--   0 max       (1000) max       (1000)      120 2023-06-06 19:52:56.000000 cobib-4.1.0/requirements.txt
+-rw-r--r--   0 max       (1000) max       (1000)     1221 2023-06-11 11:20:21.174786 cobib-4.1.0/setup.cfg
+-rw-r--r--   0 max       (1000) max       (1000)      296 2021-09-20 21:31:31.000000 cobib-4.1.0/setup.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-06-11 11:20:21.118119 cobib-4.1.0/src/
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-06-11 11:20:21.138119 cobib-4.1.0/src/cobib/
+-rw-r--r--   0 max       (1000) max       (1000)      474 2023-06-11 11:18:13.000000 cobib-4.1.0/src/cobib/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)      648 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/__main__.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-06-11 11:20:21.141453 cobib-4.1.0/src/cobib/commands/
+-rw-r--r--   0 max       (1000) max       (1000)      903 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/commands/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)    22162 2023-06-11 11:12:00.000000 cobib-4.1.0/src/cobib/commands/add.py
+-rw-r--r--   0 max       (1000) max       (1000)     7858 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/commands/base_command.py
+-rw-r--r--   0 max       (1000) max       (1000)     7187 2023-06-05 20:50:22.000000 cobib-4.1.0/src/cobib/commands/delete.py
+-rw-r--r--   0 max       (1000) max       (1000)     8026 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/commands/edit.py
+-rw-r--r--   0 max       (1000) max       (1000)     7759 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/commands/export.py
+-rw-r--r--   0 max       (1000) max       (1000)     7284 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/commands/import_.py
+-rw-r--r--   0 max       (1000) max       (1000)     4805 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/commands/init.py
+-rw-r--r--   0 max       (1000) max       (1000)    13208 2023-06-06 19:25:20.000000 cobib-4.1.0/src/cobib/commands/list_.py
+-rw-r--r--   0 max       (1000) max       (1000)    18390 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/commands/modify.py
+-rw-r--r--   0 max       (1000) max       (1000)     9080 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/commands/open.py
+-rw-r--r--   0 max       (1000) max       (1000)     4791 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/commands/redo.py
+-rw-r--r--   0 max       (1000) max       (1000)    10393 2023-06-05 20:50:22.000000 cobib-4.1.0/src/cobib/commands/search.py
+-rw-r--r--   0 max       (1000) max       (1000)     2388 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/commands/show.py
+-rw-r--r--   0 max       (1000) max       (1000)     5488 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/commands/undo.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-06-11 11:20:21.141453 cobib-4.1.0/src/cobib/config/
+-rw-r--r--   0 max       (1000) max       (1000)     1210 2022-01-13 20:47:42.000000 cobib-4.1.0/src/cobib/config/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)    27574 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/config/config.py
+-rw-r--r--   0 max       (1000) max       (1000)    29728 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/config/event.py
+-rw-r--r--   0 max       (1000) max       (1000)     9145 2023-06-06 19:19:55.000000 cobib-4.1.0/src/cobib/config/example.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-06-11 11:20:21.141453 cobib-4.1.0/src/cobib/database/
+-rw-r--r--   0 max       (1000) max       (1000)      283 2021-09-20 21:31:31.000000 cobib-4.1.0/src/cobib/database/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)    10104 2023-06-10 21:09:16.000000 cobib-4.1.0/src/cobib/database/database.py
+-rw-r--r--   0 max       (1000) max       (1000)    17670 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/database/entry.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-06-11 11:20:21.144786 cobib-4.1.0/src/cobib/importers/
+-rw-r--r--   0 max       (1000) max       (1000)      275 2021-12-01 20:44:34.000000 cobib-4.1.0/src/cobib/importers/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     3086 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/importers/base_importer.py
+-rw-r--r--   0 max       (1000) max       (1000)    12878 2023-06-11 11:12:00.000000 cobib-4.1.0/src/cobib/importers/zotero.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-06-11 11:20:21.144786 cobib-4.1.0/src/cobib/parsers/
+-rw-r--r--   0 max       (1000) max       (1000)      520 2021-09-25 22:36:09.000000 cobib-4.1.0/src/cobib/parsers/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     5019 2023-06-06 20:01:42.000000 cobib-4.1.0/src/cobib/parsers/arxiv.py
+-rw-r--r--   0 max       (1000) max       (1000)     2053 2021-09-20 21:31:31.000000 cobib-4.1.0/src/cobib/parsers/base_parser.py
+-rw-r--r--   0 max       (1000) max       (1000)     2994 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/parsers/bibtex.py
+-rw-r--r--   0 max       (1000) max       (1000)     3267 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/parsers/doi.py
+-rw-r--r--   0 max       (1000) max       (1000)     4559 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/parsers/isbn.py
+-rw-r--r--   0 max       (1000) max       (1000)     3522 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/parsers/url.py
+-rw-r--r--   0 max       (1000) max       (1000)     2996 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/parsers/yaml.py
+-rw-r--r--   0 max       (1000) max       (1000)        0 2021-09-20 21:31:31.000000 cobib-4.1.0/src/cobib/py.typed
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-06-11 11:20:21.148119 cobib-4.1.0/src/cobib/ui/
+-rw-r--r--   0 max       (1000) max       (1000)      611 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/ui/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     3391 2023-06-06 19:41:19.000000 cobib-4.1.0/src/cobib/ui/cli.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-06-11 11:20:21.151453 cobib-4.1.0/src/cobib/ui/components/
+-rw-r--r--   0 max       (1000) max       (1000)     1163 2023-06-05 20:50:22.000000 cobib-4.1.0/src/cobib/ui/components/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     1448 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/ui/components/argument_parser.py
+-rw-r--r--   0 max       (1000) max       (1000)      705 2023-06-05 20:50:22.000000 cobib-4.1.0/src/cobib/ui/components/entry_view.py
+-rw-r--r--   0 max       (1000) max       (1000)     2946 2023-06-05 20:50:22.000000 cobib-4.1.0/src/cobib/ui/components/help_screen.py
+-rw-r--r--   0 max       (1000) max       (1000)     2865 2023-06-05 20:50:22.000000 cobib-4.1.0/src/cobib/ui/components/input_screen.py
+-rw-r--r--   0 max       (1000) max       (1000)     2935 2023-06-05 20:50:22.000000 cobib-4.1.0/src/cobib/ui/components/list_view.py
+-rw-r--r--   0 max       (1000) max       (1000)     2120 2023-06-05 21:09:33.000000 cobib-4.1.0/src/cobib/ui/components/main_content.py
+-rw-r--r--   0 max       (1000) max       (1000)      565 2023-06-05 20:50:22.000000 cobib-4.1.0/src/cobib/ui/components/motion_key.py
+-rw-r--r--   0 max       (1000) max       (1000)     2035 2023-06-07 18:57:00.000000 cobib-4.1.0/src/cobib/ui/components/popup.py
+-rw-r--r--   0 max       (1000) max       (1000)     1405 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/ui/components/popup_logging_handler.py
+-rw-r--r--   0 max       (1000) max       (1000)      668 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/ui/components/popup_panel.py
+-rw-r--r--   0 max       (1000) max       (1000)     2054 2023-06-11 11:12:00.000000 cobib-4.1.0/src/cobib/ui/components/progress.py
+-rw-r--r--   0 max       (1000) max       (1000)     3313 2023-06-05 20:50:22.000000 cobib-4.1.0/src/cobib/ui/components/prompt.py
+-rw-r--r--   0 max       (1000) max       (1000)     2890 2023-06-05 20:50:22.000000 cobib-4.1.0/src/cobib/ui/components/search_view.py
+-rw-r--r--   0 max       (1000) max       (1000)     1415 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/ui/components/selection_filter.py
+-rw-r--r--   0 max       (1000) max       (1000)     1733 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/ui/shell_helper.py
+-rw-r--r--   0 max       (1000) max       (1000)    18572 2023-06-11 11:12:00.000000 cobib-4.1.0/src/cobib/ui/tui.py
+-rw-r--r--   0 max       (1000) max       (1000)     4273 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/ui/ui.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-06-11 11:20:21.151453 cobib-4.1.0/src/cobib/utils/
+-rw-r--r--   0 max       (1000) max       (1000)      242 2021-09-20 21:31:31.000000 cobib-4.1.0/src/cobib/utils/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     6731 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/utils/diff_renderer.py
+-rw-r--r--   0 max       (1000) max       (1000)     8237 2023-06-11 11:12:00.000000 cobib-4.1.0/src/cobib/utils/file_downloader.py
+-rw-r--r--   0 max       (1000) max       (1000)     4533 2021-09-20 21:32:23.000000 cobib-4.1.0/src/cobib/utils/journal_abbreviations.py
+-rw-r--r--   0 max       (1000) max       (1000)     4505 2023-06-06 19:45:15.000000 cobib-4.1.0/src/cobib/utils/logging.py
+-rw-r--r--   0 max       (1000) max       (1000)     1837 2021-09-20 21:31:31.000000 cobib-4.1.0/src/cobib/utils/rel_path.py
+-rw-r--r--   0 max       (1000) max       (1000)     8644 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/utils/shell_helper.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-06-11 11:20:21.138119 cobib-4.1.0/src/cobib.egg-info/
+-rw-r--r--   0 max       (1000) max       (1000)    40072 2023-06-11 11:20:21.000000 cobib-4.1.0/src/cobib.egg-info/PKG-INFO
+-rw-r--r--   0 max       (1000) max       (1000)     4344 2023-06-11 11:20:21.000000 cobib-4.1.0/src/cobib.egg-info/SOURCES.txt
+-rw-r--r--   0 max       (1000) max       (1000)        1 2023-06-11 11:20:21.000000 cobib-4.1.0/src/cobib.egg-info/dependency_links.txt
+-rw-r--r--   0 max       (1000) max       (1000)       47 2023-06-11 11:20:21.000000 cobib-4.1.0/src/cobib.egg-info/entry_points.txt
+-rw-r--r--   0 max       (1000) max       (1000)      120 2023-06-11 11:20:21.000000 cobib-4.1.0/src/cobib.egg-info/requires.txt
+-rw-r--r--   0 max       (1000) max       (1000)        6 2023-06-11 11:20:21.000000 cobib-4.1.0/src/cobib.egg-info/top_level.txt
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-06-11 11:20:21.158119 cobib-4.1.0/tests/
+-rw-r--r--   0 max       (1000) max       (1000)     1508 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)      872 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/cmdline_test.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-06-11 11:20:21.164786 cobib-4.1.0/tests/commands/
+-rw-r--r--   0 max       (1000) max       (1000)       68 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/commands/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     5878 2023-05-27 21:00:12.000000 cobib-4.1.0/tests/commands/command_test.py
+-rw-r--r--   0 max       (1000) max       (1000)      248 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/commands/example_duplicate_entry.bib
+-rw-r--r--   0 max       (1000) max       (1000)      261 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/commands/example_duplicate_entry.yaml
+-rw-r--r--   0 max       (1000) max       (1000)      134 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/commands/example_multi_file_entry.bib
+-rw-r--r--   0 max       (1000) max       (1000)      155 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/commands/example_multi_file_entry.yaml
+-rw-r--r--   0 max       (1000) max       (1000)    24454 2023-06-06 20:01:35.000000 cobib-4.1.0/tests/commands/test_add.py
+-rw-r--r--   0 max       (1000) max       (1000)     8961 2023-05-27 21:00:12.000000 cobib-4.1.0/tests/commands/test_delete.py
+-rw-r--r--   0 max       (1000) max       (1000)     7992 2023-05-27 21:00:12.000000 cobib-4.1.0/tests/commands/test_edit.py
+-rw-r--r--   0 max       (1000) max       (1000)     8218 2023-05-27 21:00:12.000000 cobib-4.1.0/tests/commands/test_export.py
+-rw-r--r--   0 max       (1000) max       (1000)     3077 2023-05-27 21:00:12.000000 cobib-4.1.0/tests/commands/test_git_commit_event.py
+-rw-r--r--   0 max       (1000) max       (1000)     2167 2023-05-27 21:00:12.000000 cobib-4.1.0/tests/commands/test_import.py
+-rw-r--r--   0 max       (1000) max       (1000)     6102 2023-05-27 21:00:12.000000 cobib-4.1.0/tests/commands/test_init.py
+-rw-r--r--   0 max       (1000) max       (1000)    10180 2023-06-06 19:28:09.000000 cobib-4.1.0/tests/commands/test_list.py
+-rw-r--r--   0 max       (1000) max       (1000)     9207 2023-05-27 21:00:12.000000 cobib-4.1.0/tests/commands/test_modify.py
+-rw-r--r--   0 max       (1000) max       (1000)    14520 2023-05-27 21:00:12.000000 cobib-4.1.0/tests/commands/test_open.py
+-rw-r--r--   0 max       (1000) max       (1000)     8550 2023-05-27 21:00:12.000000 cobib-4.1.0/tests/commands/test_redo.py
+-rw-r--r--   0 max       (1000) max       (1000)     8095 2023-05-27 21:00:12.000000 cobib-4.1.0/tests/commands/test_search.py
+-rw-r--r--   0 max       (1000) max       (1000)     4232 2023-05-27 21:00:12.000000 cobib-4.1.0/tests/commands/test_show.py
+-rw-r--r--   0 max       (1000) max       (1000)     7831 2023-05-27 21:00:12.000000 cobib-4.1.0/tests/commands/test_undo.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-06-11 11:20:21.168119 cobib-4.1.0/tests/config/
+-rw-r--r--   0 max       (1000) max       (1000)       28 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/config/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)      147 2023-05-27 21:00:12.000000 cobib-4.1.0/tests/config/broken_config.py
+-rw-r--r--   0 max       (1000) max       (1000)     3312 2023-05-27 21:00:12.000000 cobib-4.1.0/tests/config/test_config.py
+-rw-r--r--   0 max       (1000) max       (1000)     2401 2023-05-27 21:00:12.000000 cobib-4.1.0/tests/config/test_event.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-06-11 11:20:21.168119 cobib-4.1.0/tests/database/
+-rw-r--r--   0 max       (1000) max       (1000)       30 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/database/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)       59 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/database/example_entry_umlaut.bib
+-rw-r--r--   0 max       (1000) max       (1000)     8158 2023-06-10 20:57:45.000000 cobib-4.1.0/tests/database/test_database.py
+-rw-r--r--   0 max       (1000) max       (1000)    14623 2023-05-27 21:00:12.000000 cobib-4.1.0/tests/database/test_entry.py
+-rw-r--r--   0 max       (1000) max       (1000)      444 2023-06-06 19:45:30.000000 cobib-4.1.0/tests/debug.py
+-rw-r--r--   0 max       (1000) max       (1000)      651 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/example_entry.bib
+-rw-r--r--   0 max       (1000) max       (1000)      621 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/example_entry.yaml
+-rw-r--r--   0 max       (1000) max       (1000)      723 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/example_literature.bib
+-rw-r--r--   0 max       (1000) max       (1000)      636 2023-06-10 21:12:23.000000 cobib-4.1.0/tests/example_literature.yaml
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-06-11 11:20:21.168119 cobib-4.1.0/tests/importers/
+-rw-r--r--   0 max       (1000) max       (1000)       71 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/importers/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)      274 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/importers/importer_test.py
+-rw-r--r--   0 max       (1000) max       (1000)     4801 2023-05-27 21:00:12.000000 cobib-4.1.0/tests/importers/test_zotero.py
+-rw-r--r--   0 max       (1000) max       (1000)     2609 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/importers/zotero_database.yaml
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-06-11 11:20:21.171453 cobib-4.1.0/tests/parsers/
+-rw-r--r--   0 max       (1000) max       (1000)       65 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/parsers/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     1395 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/parsers/parser_test.py
+-rw-r--r--   0 max       (1000) max       (1000)     5763 2023-06-06 19:54:06.000000 cobib-4.1.0/tests/parsers/test_arxiv.py
+-rw-r--r--   0 max       (1000) max       (1000)     3224 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/parsers/test_bibtex.py
+-rw-r--r--   0 max       (1000) max       (1000)     5017 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/parsers/test_doi.py
+-rw-r--r--   0 max       (1000) max       (1000)     5562 2023-05-27 21:00:12.000000 cobib-4.1.0/tests/parsers/test_isbn.py
+-rw-r--r--   0 max       (1000) max       (1000)     4374 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/parsers/test_url.py
+-rw-r--r--   0 max       (1000) max       (1000)     3251 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/parsers/test_yaml.py
+-rw-r--r--   0 max       (1000) max       (1000)     4353 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/test_main.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-06-11 11:20:21.174786 cobib-4.1.0/tests/utils/
+-rw-r--r--   0 max       (1000) max       (1000)       29 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/utils/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)      172 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/utils/fixed_database.yaml
+-rw-r--r--   0 max       (1000) max       (1000)      163 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/utils/linting_database.yaml
+-rw-r--r--   0 max       (1000) max       (1000)     8992 2023-05-27 21:00:12.000000 cobib-4.1.0/tests/utils/test_file_downloader.py
+-rw-r--r--   0 max       (1000) max       (1000)     3216 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/utils/test_journal_abbreviations.py
+-rw-r--r--   0 max       (1000) max       (1000)     2990 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/utils/test_logging.py
+-rw-r--r--   0 max       (1000) max       (1000)      964 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/utils/test_rel_path.py
+-rw-r--r--   0 max       (1000) max       (1000)    13535 2023-05-27 21:00:12.000000 cobib-4.1.0/tests/utils/test_shell_helper.py
+-rw-r--r--   0 max       (1000) max       (1000)     1909 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/utils/unified_database.yaml
+-rw-r--r--   0 max       (1000) max       (1000)     1907 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/utils/unifying_database.yaml
+-rw-r--r--   0 max       (1000) max       (1000)     1287 2023-05-27 21:00:12.000000 cobib-4.1.0/tox.ini
```

### Comparing `cobib-4.0.0/.gitlab-ci.yml` & `cobib-4.1.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/.pylintdict` & `cobib-4.1.0/.pylintdict`

 * *Files 6% similar despite different names*

```diff
@@ -20,18 +20,20 @@
 changelog
 cli
 cmd
 cobib
 config
 configfile
 configpath
+coroutine
 dat
 dataclass
 dataclasses
 deepcopied
+devtools
 diff
 disambiguated
 docstring
 doi
 dotless
 downloader
 enum
@@ -71,14 +73,15 @@
 postarxivparse
 postdoiparse
 postgitcommit
 postinitcommand
 postisbnparse
 pragma
 pre
+programmatically
 py
 pypi
 pytest
 readme
 readthedocs
 renderable
 renderer
```

### Comparing `cobib-4.0.0/.pylintrc` & `cobib-4.1.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/CHANGELOG.md` & `cobib-4.1.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,17 +3,74 @@
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
 
+## [4.1.0] - 2023-06-11
+
+Pypi: https://pypi.org/project/cobib/4.1.0/
+
+### Added
+- added the following settings which specify whether or not to preserve
+  associated files during the respective commands being run:
+  - `config.commands.delete.preserve_files`
+  - `config.commands.edit.preserve_files`
+  - `config.commands.modify.preserve_files`
+- added a confirmation prompt before deleting an entry (#110)
+  - this prompt can be disabled by setting `config.commands.delete.confirm` to `False`
+- added the `--no-ignore-case` (`-I` for short) command line options to the
+  `list` and `search` command (#116)
+- added the `--no-preserve-files` command line options to the `delete`, `edit`
+  and `modify` command (#116)
+- added the `config.commands.search.context` setting which configures the
+  default number of context lines to be provided for search query matches
+- added more options to configure the automatic download behavior:
+  - the new `config.commands.add.skip_download` setting
+  - the new `--force-download` option of the `add` command
+  - the new `config.commands.import_.skip_download` setting
+  - the new `--force-download` option of the `import` command
+- the user is asked for confirmation when quitting the TUI (!71)
+
+### Changed
+- refactored the TUI by leveraging textual's `Screen` concept (#111,!71)
+  - this means the TUI will look slightly different but no real functional change has occurred
+  - the view of an `Entry` can now be scrolled when the output exceeds the available space
+- switched from the `BeautifulSoup` HTML parser to `lxml`
+  - this is supposed to give more accurate results but adds an extra dependency
+
+### Deprecated
+- The following shell helpers are no longer used with the zsh completion being
+  removed. Thus, these methods will be removed in the future:
+  - `cobib _list_commands`
+  - `cobib _list_filters`
+  - `cobib _list_labels`
+  - If you see warnings because of this while you are using the CLI, you
+    probably still have the (now removed) zsh completion script installed. You
+    should remove the `_cobib` file which will be located in one of the
+    directories listed in your `$FPATH` environment variable.
+
+### Fixed
+- the proper pre-population of the TUI prompt during the sorting action (#117)
+- preserves the value of `config.commands.list_.default_columns` and
+  properly removes a field if it is no longer sorted by in the TUI (#117)
+- properly updates the list of entries in the TUI after changing the database contents;
+  for example via `add` (#113) or `delete` (#113) or `edit` (#118)
+- an issue where file-accessing operations performed on a newly added entry within
+  the same TUI session would fail because the path would not be iterated correctly
+- the live updating of the download progress bar inside the TUI (#112)
+
+### Removed
+- the crude and very slow zsh completion script
+
+
 ## [4.0.0] - 2023-05-20
 
-Pypi: https://pypi.org/project/cobib/3.5.5/
+Pypi: https://pypi.org/project/cobib/4.0.0/
 
 ### **Breaking Changes**
 - Configuration settings can no longer be set by item access and instead must
   use attribute syntax. For example you need to change:
   ```python
   config["database"]["git"] = True
   ```
@@ -706,15 +763,16 @@
 
 ## [0.1] - 2019-04-29
 
 ### Added
 - initial version with a basic `sqlite3`-based database
 
 
-[Unreleased]: https://gitlab.com/cobib/cobib/-/compare/v4.0.0...master
+[Unreleased]: https://gitlab.com/cobib/cobib/-/compare/v4.1.0...master
+[4.1.0]: https://gitlab.com/cobib/cobib/-/compare/v4.1.0
 [4.0.0]: https://gitlab.com/cobib/cobib/-/compare/v4.0.0
 [3.5.5]: https://gitlab.com/cobib/cobib/-/compare/v3.5.5
 [3.5.4]: https://gitlab.com/cobib/cobib/-/compare/v3.5.4
 [3.5.3]: https://gitlab.com/cobib/cobib/-/compare/v3.5.3
 [3.5.2]: https://gitlab.com/cobib/cobib/-/compare/v3.5.2
 [3.5.1]: https://gitlab.com/cobib/cobib/-/compare/v3.5.1
 [3.5.0]: https://gitlab.com/cobib/cobib/-/compare/v3.5.0
```

### Comparing `cobib-4.0.0/CONTRIBUTING.md` & `cobib-4.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/LICENSE.txt` & `cobib-4.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/PKG-INFO` & `cobib-4.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cobib
-Version: 4.0.0
+Version: 4.1.0
 Summary: Console Bibliography
 Home-page: https://gitlab.com/cobib/cobib
 Author: Max Rossmannek
 Author-email: max.rossmannek@uzh.ch
 License: MIT License
 Project-URL: Bug Tracker, https://gitlab.com/cobib/cobib/-/issues
 Project-URL: Documentation, https://cobib.gitlab.io/cobib/cobib.html
@@ -51,16 +51,16 @@
 
 ```
 pip install cobib
 ```
 
 Note: Use `pip3` if you still have Python 2 installed.
 
-If you would also like to install the man-page and (crude!) Zsh completion,
-you need to download the source code and do the following:
+If you would also like to install the man-page, you need to download the source
+code and do the following:
 
 ```
 git clone https://gitlab.com/cobib/cobib
 cd cobib
 make install_extras
 ```
 
@@ -289,17 +289,74 @@
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
 
+## [4.1.0] - 2023-06-11
+
+Pypi: https://pypi.org/project/cobib/4.1.0/
+
+### Added
+- added the following settings which specify whether or not to preserve
+  associated files during the respective commands being run:
+  - `config.commands.delete.preserve_files`
+  - `config.commands.edit.preserve_files`
+  - `config.commands.modify.preserve_files`
+- added a confirmation prompt before deleting an entry (#110)
+  - this prompt can be disabled by setting `config.commands.delete.confirm` to `False`
+- added the `--no-ignore-case` (`-I` for short) command line options to the
+  `list` and `search` command (#116)
+- added the `--no-preserve-files` command line options to the `delete`, `edit`
+  and `modify` command (#116)
+- added the `config.commands.search.context` setting which configures the
+  default number of context lines to be provided for search query matches
+- added more options to configure the automatic download behavior:
+  - the new `config.commands.add.skip_download` setting
+  - the new `--force-download` option of the `add` command
+  - the new `config.commands.import_.skip_download` setting
+  - the new `--force-download` option of the `import` command
+- the user is asked for confirmation when quitting the TUI (!71)
+
+### Changed
+- refactored the TUI by leveraging textual's `Screen` concept (#111,!71)
+  - this means the TUI will look slightly different but no real functional change has occurred
+  - the view of an `Entry` can now be scrolled when the output exceeds the available space
+- switched from the `BeautifulSoup` HTML parser to `lxml`
+  - this is supposed to give more accurate results but adds an extra dependency
+
+### Deprecated
+- The following shell helpers are no longer used with the zsh completion being
+  removed. Thus, these methods will be removed in the future:
+  - `cobib _list_commands`
+  - `cobib _list_filters`
+  - `cobib _list_labels`
+  - If you see warnings because of this while you are using the CLI, you
+    probably still have the (now removed) zsh completion script installed. You
+    should remove the `_cobib` file which will be located in one of the
+    directories listed in your `$FPATH` environment variable.
+
+### Fixed
+- the proper pre-population of the TUI prompt during the sorting action (#117)
+- preserves the value of `config.commands.list_.default_columns` and
+  properly removes a field if it is no longer sorted by in the TUI (#117)
+- properly updates the list of entries in the TUI after changing the database contents;
+  for example via `add` (#113) or `delete` (#113) or `edit` (#118)
+- an issue where file-accessing operations performed on a newly added entry within
+  the same TUI session would fail because the path would not be iterated correctly
+- the live updating of the download progress bar inside the TUI (#112)
+
+### Removed
+- the crude and very slow zsh completion script
+
+
 ## [4.0.0] - 2023-05-20
 
-Pypi: https://pypi.org/project/cobib/3.5.5/
+Pypi: https://pypi.org/project/cobib/4.0.0/
 
 ### **Breaking Changes**
 - Configuration settings can no longer be set by item access and instead must
   use attribute syntax. For example you need to change:
   ```python
   config["database"]["git"] = True
   ```
@@ -992,15 +1049,16 @@
 
 ## [0.1] - 2019-04-29
 
 ### Added
 - initial version with a basic `sqlite3`-based database
 
 
-[Unreleased]: https://gitlab.com/cobib/cobib/-/compare/v4.0.0...master
+[Unreleased]: https://gitlab.com/cobib/cobib/-/compare/v4.1.0...master
+[4.1.0]: https://gitlab.com/cobib/cobib/-/compare/v4.1.0
 [4.0.0]: https://gitlab.com/cobib/cobib/-/compare/v4.0.0
 [3.5.5]: https://gitlab.com/cobib/cobib/-/compare/v3.5.5
 [3.5.4]: https://gitlab.com/cobib/cobib/-/compare/v3.5.4
 [3.5.3]: https://gitlab.com/cobib/cobib/-/compare/v3.5.3
 [3.5.2]: https://gitlab.com/cobib/cobib/-/compare/v3.5.2
 [3.5.1]: https://gitlab.com/cobib/cobib/-/compare/v3.5.1
 [3.5.0]: https://gitlab.com/cobib/cobib/-/compare/v3.5.0
```

### Comparing `cobib-4.0.0/README.md` & `cobib-4.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 
 ```
 pip install cobib
 ```
 
 Note: Use `pip3` if you still have Python 2 installed.
 
-If you would also like to install the man-page and (crude!) Zsh completion,
-you need to download the source code and do the following:
+If you would also like to install the man-page, you need to download the source
+code and do the following:
 
 ```
 git clone https://gitlab.com/cobib/cobib
 cd cobib
 make install_extras
 ```
```

### Comparing `cobib-4.0.0/cobib.1` & `cobib-4.1.0/cobib.1`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH COBIB 1 2023-05-20 v4.0.0
+.TH COBIB 1 2023-06-11 v4.1.0
 .SH NAME
 coBib \- Console-based Bibliography Management
 .SH SYNOPSIS
 .B cobib
 [\fB\-\-version\fR]
 [\fB\-h\fR|\fB\-\-help\fR]
 [\fB\-v\fR|\fB\-\-verbose\fR]
@@ -93,14 +93,20 @@
 .PP
 .in +8n
 .BR \-\-url " " \fI<URL>\fR
 .in +4n
 Attempts to extract an entry from the \fI<URL>\fR.
 .PP
 .in +8n
+.BR \-y ", " \-\-yaml " " \fI<path>\fR
+.in +4n
+Adds the bibliography data from the \fIYAML\fR file at the provided path.
+The only supported YAML format is that of a coBib database file.
+.PP
+.in +8n
 .BR \-l ", " \-\-label  " " \fI<label>\fR
 .in +4n
 Store the newly added entry under the specified \fIlabel\fR.
 .PP
 .in +8n
 .BR \-f ", " \-\-file " " \fI<path>\fR
 .in +4n
@@ -132,22 +138,38 @@
 to disambiguate the new label from the existing one by adding a label suffix
 (see also \fIconfig.database.format.label_suffix\fR)
 .PP
 .in +8n
 .BR \-\-skip\-download
 .in +4n
 Skips attempting to automatically download an associated file for the entry.
+This takes precedence over the \fIconfig.commands.add.skip_download\fR setting.
+.PP
+.in +8n
+.BR \-\-force\-download
+.in +4n
+Forces attempting to automatically download an associated file for the entry.
+This takes precedence over the \fIconfig.commands.add.skip_download\fR setting.
 .TP
 .B cobib delete \fI<label>\fR
 Deletes the entry with the given \fIlabel\fR.
 .PP
 .in +8n
 .BR \-\-preserve\-files
 .in +4n
-Only if this is set, associated files will be preserved and \fInot\fR deleted.
+If specified, associated files will be preserved and \fInot\fR deleted.
+This takes precedence over the \fIconfig.commands.delete.preserve_files\fR
+setting.
+.PP
+.in +8n
+.BR \-\-no\-preserve\-files
+.in +4n
+If specified, associated files will \fInot\fR be preserved.
+This takes precedence over the \fIconfig.commands.delete.preserve_files\fR
+setting.
 .TP
 .B cobib edit \fI<label>\fR
 Opens the entry with the given \fIlabel\fR in an external editor.
 The entry is copied verbatim in \fIYAML\fR format from and to the database file.
 The editor respects the \fI$EDITOR\fR environment variable unless overwritten by
 \fIconfig.commands.edit.editor\fR. It will fallback to \fIvim\fR if neither is
 configured.
@@ -156,16 +178,24 @@
 .BR \-a ", " \-\-add " " \fI<path>\fR
 .in +4n
 Allows editing a non-existing label to manually add it to the database.
 .PP
 .in +8n
 .BR \-\-preserve\-files
 .in +4n
-Only if this is set, associated files will be preserved and \fInot\fR renamed if
-the edit happens to rename the entry.
+If specified, associated files will be preserved and \fInot\fR be renamed if the
+edit happens to rename the entry. This takes precedence over the
+\fIconfig.commands.edit.preserve_files\fR setting.
+.PP
+.in +8n
+.BR \-\-no\-preserve\-files
+.in +4n
+If specified, associated files will \fInot\fR be preserved and be renamed if the
+edit happens to rename the entry. This takes precedence over the
+\fIconfig.commands.edit.preserve_files\fR setting.
 .TP
 .B cobib modify \fI<modification>\fR \fI<args>\fR ...
 Applies a modification to multiple entries at once.
 The positional arguments may be used to provide \fBFILTERS\fR which the entries
 must match in order to be modified \fIor\fR to provide a list of labels of the
 entries which are to be modified (this requires the \fI-s\fR flag to be set).
 The \fI<args>\fR may be any of the following:
@@ -205,16 +235,24 @@
 This boolean flag enables the \fIselection\fR mode in which the positional args
 are interpreted as a list of labels which are to be exported. The name for this
 argument is a result of the TUI's selection interface.
 .PP
 .in +8n
 .BR \-\-preserve\-files
 .in +4n
-Only if this is set, associated files will be preserved and \fInot\fR renamed if
-the modification happens to rename the entry.
+If specified, associated files will be preserved and \fInot\fR be renamed if
+the modification happens to rename the entry. This takes precedence over the
+\fIconfig.commands.modify.preserve_files\fR setting.
+.PP
+.in +8n
+.BR \-\-no\-preserve\-files
+.in +4n
+If specified, associated files will \fInot\fR be preserved and be renamed if
+the modification happens to rename the entry. This takes precedence over the
+\fIconfig.commands.modify.preserve_files\fR setting.
 .TP
 .B cobib undo \fI<args>\fR
 If you enabled the git-integration of coBib (available since v2.6.0) you can
 undo the changes done to your database file by commands such as add, edit and
 delete. See also \fIDATABASE/git\fR in the \fBCONFIGURATION\fR section for more
 information.
 .PP
@@ -239,33 +277,34 @@
 .TP
 .B cobib list \fI<args>\fR
 Lists all entries of the database in a basic table format to stdout which match
 the specified \fBFILTERS\fR (more information is provided in that section).
 Additionally, the following \fI<args>\fR are also allowed:
 .PP
 .in +8n
-.BR \-l ", " \-\-long
-.in +4n
-Print the table in \fIlong\fR format, i.e. without wrapping the lines to fit the
-current terminal width.
-.PP
-.in +8n
 .BR \-s ", " \-\-sort " " \fI<field>\fI
 .in +4n
 Specify the entry field to use as the \fIsorting column\fR of the table.
 .PP
 .in +8n
 .BR \-r ", " \-\-reverse
 .in +4n
 Reverses the sorting order.
 .PP
 .in +8n
-.BR \-i ", " \-\-ignore-case
+.BR \-i ", " \-\-ignore\-case
 .in +4n
 Makes the entry matching case-insensitive.
+This takes precedence over the \fIconfig.commands.list_.ignore_case\fR setting.
+.PP
+.in +8n
+.BR \-I ", " \-\-no\-ignore\-case
+.in +4n
+Makes the entry matching case-sensitive.
+This takes precedence over the \fIconfig.commands.list_.ignore_case\fR setting.
 .PP
 .in +8n
 .BR \-x ", " \-\-or
 .in +4n
 Concatenate the filters using logical \fIOR\fR rather than the default
 \fIAND\fR.
 .TP
@@ -276,20 +315,28 @@
 must match in order to be included in the export.
 Additionally, the following \fI<args>\fR are also allowed:
 .PP
 .in +8n
 .BR \-c ", " \-\-context " " \fI<int>\fI
 .in +4n
 Specify the number of context lines to provide for each match.
-This values defaults to 1.
+The default value is 1 but can be configured via
+\fIconfig.commands.search.context\fR.
 .PP
 .in +8n
-.BR \-i ", " \-\-ignore-case
+.BR \-i ", " \-\-ignore\-case
 .in +4n
 Makes the search case-insensitive.
+This takes precedence over the \fIconfig.commands.search.ignore_case\fR setting.
+.PP
+.in +8n
+.BR \-I ", " \-\-no\-ignore\-case
+.in +4n
+Makes the search case-insensitive.
+This takes precedence over the \fIconfig.commands.list_.ignore_case\fR setting.
 .TP
 .B cobib export \fI<args>\fR ...
 Exports the database.
 The positional arguments may be used to provide \fBFILTERS\fR which the entries
 must match in order to be included in the export \fIor\fR to provide a list of
 labels of the entries which are to be exported (this requires the \fI-s\fR flag
 to be set).
@@ -331,14 +378,23 @@
 this command once.
 The \fI<args>\fR may be any of the following:
 .PP
 .in +8n
 .BR \-\-skip\-download
 .in +4n
 Skips downloading of attachments encountered during the library import.
+This takes precedence over the \fIconfig.commands.import_.skip_download\fR
+setting.
+.PP
+.in +8n
+.BR \-\-force\-download
+.in +4n
+Forces downloading of attachments encountered during the library import.
+This takes precedence over the \fIconfig.commands.import_.skip_download\fR
+setting.
 .PP
 .in +8n
 Furthermore you can specify one of the following sources from which to import
 your library. Each of those sources can optionally take further arguments via
 positional arguments following a \fI--\fR separator.
 .PP
 .in +8n
@@ -517,36 +573,59 @@
 .IR config.logging.version = '~/.cache/cobib/version'
 In this file, the last run version of coBib gets cached. After an update, coBib
 automtically prints the newest section of the Changelog. To disable this
 functionality entirely, set this option to \fINone\fR.
 .PP
 .BR COMMANDS
 .TP
+.IR config.commands.add.skip_download = False
+Specifies whether to skip the attempt of downloading PDF files of added entries.
+.TP
+.IR config.commands.delete.confirm = True
+Specifies whether or not to prompt for confirmation before deleting an entry.
+.TP
+.IR config.commands.delete.preserve_files = False
+Specifies whether associates files should be preserved during deletion.
+.TP
 .IR config.commands.edit.default_entry_type = 'article'
 This setting indicates the default entry type which will be used for manually
 entered entries.
 .TP
 .IR config.commands.edit.editor = $EDITOR " if available else " 'vim'
 This setting can be used to overwrite the external editor used for manual
 editing of database entries. It defaults to the environment variable
 \fI$EDITOR\fR and falls back to \fIvim\fR if that is not set either.
 .TP
+.IR config.commands.edit.preserve_files = False
+Specifies whether associates files should be preserved during renaming.
+.TP
+.IR config.commands.import_.skip_download = False
+Specifies whether to skip downloading of attachments encountered during the
+library import.
+.TP
 .IR config.commands.list_.default_columns = ['label',\ 'title']
 Specifies the default columns displayed during the \fIlist\fR command.
 .TP
 .IR config.commands.list_.ignore_case = False
 Specifies whether filter matching should be performed case-insensitive.
 .TP
+.IR config.commands.modify.preserve_files = False
+Specifies whether associates files should be preserved during renaming.
+.TP
 .IR config.commands.open.command = 'xdg-open' " (on Linux); " 'open' " (on Mac OS)"
 Specifies the program used to open associated files.
 .TP
 .IR config.commands.open.fields = ['file',\ 'url']
 Specifies the names of the data fields which are to be checked for openable
 URLs.
 .TP
+.IR config.commands.search.context = 1
+Specifies the default number of context lines to provide for each search query
+match.
+.TP
 .IR config.commands.search.grep = 'grep'
 Specifies the program used to search in associated files.
 .TP
 .IR config.commands.search.grep_args = []
 Allows the specification of additional arguments for the \fIgrep\fR command.
 .TP
 .IR config.commands.search.ignore_case = False
```

### Comparing `cobib-4.0.0/html/cobib_book.svg` & `cobib-4.1.0/html/cobib_book.svg`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/html/cobib_logo.svg` & `cobib-4.1.0/html/cobib_logo.svg`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/html/index.html.jinja2` & `cobib-4.1.0/html/index.html.jinja2`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/logo/cobib_book-squared.png` & `cobib-4.1.0/logo/cobib_book-squared.png`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/logo/cobib_book.png` & `cobib-4.1.0/logo/cobib_book.png`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/logo/cobib_book.svg` & `cobib-4.1.0/logo/cobib_book.svg`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/logo/cobib_byline.png` & `cobib-4.1.0/logo/cobib_byline.png`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/logo/cobib_byline.svg` & `cobib-4.1.0/logo/cobib_byline.svg`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/logo/cobib_logo.png` & `cobib-4.1.0/logo/cobib_logo.png`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/logo/cobib_logo.svg` & `cobib-4.1.0/logo/cobib_logo.svg`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/setup.cfg` & `cobib-4.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/src/cobib/__main__.py` & `cobib-4.1.0/src/cobib/__main__.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/src/cobib/commands/__init__.py` & `cobib-4.1.0/src/cobib/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/src/cobib/commands/add.py` & `cobib-4.1.0/src/cobib/commands/add.py`

 * *Files 10% similar despite different names*

```diff
@@ -68,18 +68,27 @@
 Since v3.2.0 coBib attempts to download PDF files for newly added entries (if the corresponding
 parser supports this feature). The default location where this file will be stored can be configured
 via `cobib.config.config.FileDownloaderConfig.default_location`, but it can be changed at runtime
 using the `--path` argument like so:
 ```
 cobib add --path <some custom path> --arxiv <some arXiv ID>
 ```
-If you want to manually suppress the automatic download, specify the `--skip-download` argument:
+Since v4.1.0 you can suppress the automatic download via the
+`cobib.config.config.AddCommandConfig.skip_download` setting. It defaults to `False` meaning that
+the download will be attempted.
+If you want to manually overwrite the configuration setting you can do so with the `--skip-download`
+and `--force-download` arguments, respectively.
+I.e. the following will **not** attempt the automatic download:
 ```
 cobib add --skip-download --arxiv <some arXiv ID>
 ```
+While the next command will always attempt the automatic download:
+```
+cobib add --force-download --arxiv <some arXiv ID>
+```
 
 Since v4.0.0 coBib will ask you what to do when encountering a conflict at runtime. That means, when
 a label already exists in your database, you have various choices how to handle it:
 
 1. you can `keep` the existing entry and skip the addition of the new one.
    .. note::
       This is equivalent to the old `--skip-existing` argument (added in v3.3.0) which is now
@@ -129,20 +138,19 @@
 
 import argparse
 import asyncio
 import inspect
 import logging
 from collections import OrderedDict
 from functools import wraps
-from typing import Callable, Dict, Tuple, Type, cast
+from typing import Callable, Dict, Type, cast
 
 from rich.console import Console
 from rich.prompt import InvalidResponse, Prompt, PromptBase, PromptType
 from textual.app import App
-from textual.widget import AwaitMount, Widget
 from typing_extensions import override
 
 from cobib import parsers
 from cobib.config import Event, config
 from cobib.database import Database, Entry
 from cobib.parsers import BibtexParser
 from cobib.utils.diff_renderer import Differ
@@ -165,14 +173,15 @@
         * `-d`, `--disambiguation`: hard-codes the reply to be used if a disambiguation prompt would
           occur.
         * `-f`, `--file`: one or multiple files to associate with this entry. This data will be
           stored in the `cobib.database.Entry.file` property.
         * `-p`, `--path`: the path to store the downloaded associated file in. This can be used to
           overwrite the `cobib.config.config.FileDownloaderConfig.default_location`.
         * `--skip-download`: skips the automatic download of an associated file.
+        * `--force-download`: forces the automatic download of an associated file.
         * `--skip-existing`: **DEPRECATED** use `--disambiguation keep` instead!
         * `-u`, `--update`: **DEPRECATED** use `--disambiguation update` instead!
         * in addition to the options above, a *mutually exclusive group* of keyword arguments for
           all available `cobib.parsers` are registered at runtime. Please check the output of
           `cobib add --help` for the exact list.
         * any *positional* arguments (i.e. those, not preceded by a keyword) are interpreted as tags
           and will be stored in the `cobib.database.Entry.tags` property.
@@ -186,15 +195,15 @@
     """The available parsers."""
 
     @override
     def __init__(
         self,
         *args: str,
         console: Console | App[None] | None = None,
-        prompt: Type[PromptBase[str]] | None = None,
+        prompt: Type[PromptBase[PromptType]] | None = None,
     ) -> None:
         super().__init__(*args, console=console, prompt=prompt)
 
         self.new_entries: Dict[str, Entry] = OrderedDict()
         """An `OrderedDict` mapping labels to `cobib.database.Entry` instances which were added by
         this command."""
 
@@ -214,19 +223,28 @@
         parser.add_argument("-p", "--path", type=str, help="the path for the downloaded file")
         parser.add_argument(
             "--disambiguation",
             type=str,
             choices=["keep", "replace", "update", "disambiguate"],
             help="the reply in case of a disambiguation prompt",
         )
-        parser.add_argument(
+        skip_download_group = parser.add_mutually_exclusive_group()
+        skip_download_group.add_argument(
             "--skip-download",
             action="store_true",
+            default=None,
             help="skip the automatic download of an associated file",
         )
+        skip_download_group.add_argument(
+            "--force-download",
+            dest="skip_download",
+            action="store_false",
+            default=None,
+            help="force the automatic download of an associated file",
+        )
         parser.add_argument(
             "--skip-existing",
             action="store_true",
             help="DEPRECATED: use '--disambiguation keep' instead!",
         )
         parser.add_argument(
             "-u",
@@ -272,15 +290,15 @@
                 "Instead you should use '--disambiguation update'."
             )
             LOGGER.warning(msg)
             largs.disambiguation = "update"
 
         return largs
 
-    # pylint: disable=invalid-overridden-method,too-many-statements,too-many-branches
+    # pylint: disable=invalid-overridden-method,too-many-statements,too-many-branches,too-many-locals
     @override
     async def execute(self) -> None:  # type: ignore[override]
         LOGGER.debug("Starting Add command.")
 
         Event.PreAddCommand.fire(self)
 
         edit_entries = False
@@ -334,14 +352,19 @@
 
         if self.largs.tags != []:
             assert len(self.new_entries.values()) == 1
             for value in self.new_entries.values():
                 # logging done by cobib/database/entry.py
                 value.tags = self.largs.tags
 
+        skip_download = config.commands.add.skip_download
+        if self.largs.skip_download is not None:
+            skip_download = self.largs.skip_download
+        LOGGER.info("Automatic file download will%s be attempted.", " not" if skip_download else "")
+
         bib = Database()
         existing_labels = set(bib.keys())
 
         for lbl, entry in self.new_entries.copy().items():
             overwrite_file = False
             # check if label already exists
             if lbl in existing_labels:
@@ -366,36 +389,46 @@
                     parser = BibtexParser()
                     left = parser.dump(bib[lbl])
                     right = parser.dump(entry)
                     diff = Differ(left, right)
                     diff.compute()
                     table = diff.render("bibtex")
 
-                    # pylint: disable=assignment-from-no-return
-                    print_ret = self.console.print(table)  # type: ignore[union-attr]
-
                     prompt_text = "How would you like to handle this conflict?"
                     choices = ["keep", "replace", "update", "disambiguate", "help"]
                     default = "keep"
 
                     # pylint: disable=line-too-long
                     self.prompt.process_response = self._wrap_prompt_process_response(  # type: ignore[method-assign]
                         self.prompt.process_response  # type: ignore[assignment]
                     )
 
                     if self.prompt is not Prompt:
+
+                        @wraps(self.prompt.pre_prompt)
+                        def pre_prompt(_prompt: PromptBase[PromptType]) -> None:
+                            _prompt.console.push_screen("input")  # type: ignore[attr-defined]
+                            _prompt.console.print(table)  # pylint: disable=cell-var-from-loop
+
+                        # pylint: disable=line-too-long
+                        self.prompt.pre_prompt = pre_prompt  # type: ignore[assignment,method-assign]
+
                         res = await self.prompt.ask(  # type: ignore[call-overload]
                             prompt_text,
                             choices=choices,
                             default=default,
                             console=cast(App[None], self.console),
                         )
-                        popup, _ = cast(Tuple[Widget, AwaitMount], print_ret)
-                        popup.remove()
+
+                        self.prompt.pre_prompt = (  # type: ignore[method-assign]
+                            self.prompt.pre_prompt.__wrapped__  # type: ignore[attr-defined]
+                        )
                     else:
+                        self.console.print(table)  # type: ignore[union-attr]
+
                         res = self.prompt.ask(
                             prompt_text,
                             choices=choices,
                             default=default,
                             console=cast(Console, self.console),
                         )
 
@@ -427,28 +460,28 @@
                     msg = f"Skipping addition of the already existing entry '{lbl}'."
                     LOGGER.info(msg)
                     self.new_entries.pop(lbl)
                     continue
 
             # download associated file (if requested)
             if "_download" in entry.data.keys():
-                if self.largs.skip_download:
+                if skip_download:
                     entry.data.pop("_download")
                 else:
                     task = asyncio.create_task(
                         FileDownloader().download(
                             entry.data.pop("_download"),
                             entry.label,
                             folder=self.largs.path,
                             overwrite=overwrite_file,
                         )
                     )
                     path = await task
                     if path is not None:
-                        entry.data["file"] = str(path)
+                        entry.file = str(path)  # type: ignore[assignment]
             # check journal abbreviation
             if "journal" in entry.data.keys():
                 entry.data["journal"] = JournalAbbreviations.elongate(entry.data["journal"])
 
         Event.PostAddCommand.fire(self)
 
         bib.update(self.new_entries)
```

### Comparing `cobib-4.0.0/src/cobib/commands/base_command.py` & `cobib-4.1.0/src/cobib/commands/base_command.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import os
 import shlex
 import sys
 from abc import ABC, abstractmethod
 from typing import List, Optional, Type
 
 from rich.console import Console, ConsoleRenderable
-from rich.prompt import Prompt, PromptBase
+from rich.prompt import Prompt, PromptBase, PromptType
 from textual.app import App
 from textual.widget import Widget
 
 from cobib.config import Event, config
 from cobib.ui.components import ArgumentParser as ArgumentParser
 from cobib.utils.rel_path import RelPath
 
@@ -38,15 +38,15 @@
     provided to the command. This is done no matter how the command is executed, whether
     programmatically via Python, from the command-line or any other UI."""
 
     def __init__(
         self,
         *args: str,
         console: Console | App[None] | None = None,
-        prompt: Type[PromptBase[str]] | None = None,
+        prompt: Type[PromptBase[PromptType]] | None = None,
     ) -> None:
         """Initializes a command instance.
 
         Args:
             *args: the sequence of additional command arguments. These will be passed on to the
                 `argparser` of this command for further parsing.
             console: a command may be in need of printing something for the user during its
@@ -61,15 +61,15 @@
 
         self.largs: argparse.Namespace = self.__class__._parse_args(args)
         """The parsed (local) arguments."""
 
         self.console: Console | App[None] = console if console is not None else Console()
         """The object via which to print output to the user during runtime execution."""
 
-        self.prompt: Type[PromptBase[str]] = prompt if prompt is not None else Prompt
+        self.prompt: Type[PromptBase[PromptType]] = prompt if prompt is not None else Prompt
         """The object via which to prompt the user for input during runtime execution."""
 
     @classmethod
     @abstractmethod
     def init_argparser(cls) -> None:
         """Initializes this command's `argparse.ArgumentParser`.
```

### Comparing `cobib-4.0.0/src/cobib/commands/edit.py` & `cobib-4.1.0/src/cobib/commands/edit.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,19 +16,27 @@
 ```
 cobib edit --add <new label>
 ```
 This entry will be entirely empty except for the one field which is always present:
     * `ENTRYTYPE`: set to the default value configured via
       `cobib.config.config.EditCommandConfig.default_entry_type`.
 
-If you change the label of the entry during editing and you do *not* want your associated files to
-automatically be renamed, you can provide the `--preserve-files` argument like so:
+If you change the label of the entry during editing, the value of the
+`cobib.config.config.EditCommandConfig.preserve_files` setting (added in v4.1.0) determines whether
+the associated files will be renamed automatically. This defaults to `False`, meaning that they
+*will* be renamed. You can overwrite the value of this setting at runtime with the
+`--preserve-files` and `--no-preserve-files` arguments, respectively.
+I.e. the following will **not** rename your files:
 ```
 cobib edit --preserve-files <label>
 ```
+While this command will always rename them:
+```
+cobib edit --no-preserve-files <label>
+```
 
 ### TUI
 
 You can also trigger this command from the `cobib.ui.tui.TUI`.
 By default, it is bound to the `e` key.
 If you want to add a new entry manually, you will have to enter the prompt (defaults to `:`) and
 then type out the command mentioned above:
@@ -42,15 +50,15 @@
 import logging
 import os
 import tempfile
 from pathlib import Path
 from typing import Type
 
 from rich.console import Console
-from rich.prompt import PromptBase
+from rich.prompt import PromptBase, PromptType
 from textual.app import App
 from typing_extensions import override
 
 from cobib.config import Event, config
 from cobib.database import Database, Entry
 from cobib.parsers.yaml import YAMLParser
 from cobib.utils.rel_path import RelPath
@@ -66,25 +74,29 @@
     This command can parse the following arguments:
 
         * `label`: the label of the entry to edit.
         * `-a`, `--add`: if specified, allows adding a new entry for a non-existent label. The
           default entry type of this new entry can be configured via
           `cobib.config.config.EditCommandConfig.default_entry_type`.
         * `--preserve-files`: skips the renaming of any associated files in case you manually rename
-            the entry label during editing.
+          the entry label during editing. This overwrites the
+          `cobib.config.config.EditCommandConfig.preserve_files` setting.
+        * `--no-preserve-files`: does NOT skip the renaming of any associated files in case you
+          manually rename the entry label during editing. This overwrites the
+          `cobib.config.config.EditCommandConfig.preserve_files` setting.
     """
 
     name = "edit"
 
     @override
     def __init__(
         self,
         *args: str,
         console: Console | App[None] | None = None,
-        prompt: Type[PromptBase[str]] | None = None,
+        prompt: Type[PromptBase[PromptType]] | None = None,
     ) -> None:
         super().__init__(*args, console=console, prompt=prompt)
 
         self.new_entry: Entry
         """A `cobib.database.Entry` instance edited by this command."""
 
     @override
@@ -94,16 +106,27 @@
         parser.add_argument("label", type=str, help="label of the entry")
         parser.add_argument(
             "-a",
             "--add",
             action="store_true",
             help="if specified, will add a new entry for unknown labels",
         )
-        parser.add_argument(
-            "--preserve-files", action="store_true", help="do not rename associated files"
+        preserve_files_group = parser.add_mutually_exclusive_group()
+        preserve_files_group.add_argument(
+            "--preserve-files",
+            action="store_true",
+            default=None,
+            help="do NOT rename associated files",
+        )
+        preserve_files_group.add_argument(
+            "--no-preserve-files",
+            dest="preserve_files",
+            action="store_false",
+            default=None,
+            help="rename associated files",
         )
         cls.argparser = parser
 
     @override
     def execute(self) -> None:
         LOGGER.debug("Starting Edit command.")
 
@@ -155,17 +178,23 @@
             self.new_entry = list(new_entries.values())[0]
         assert not Path(tmp_file_name).exists()
         if entry == self.new_entry and not self.largs.add:
             LOGGER.info("No changes detected.")
             return
 
         bib.update({self.new_entry.label: self.new_entry})
+
+        preserve_files = config.commands.edit.preserve_files
+        if self.largs.preserve_files is not None:
+            preserve_files = self.largs.preserve_files
+        LOGGER.info("Associated files will%s be preserved.", "" if preserve_files else " not")
+
         if self.new_entry.label != self.largs.label:
             bib.rename(self.largs.label, self.new_entry.label)
-            if not self.largs.preserve_files:
+            if not preserve_files:
                 new_files = []
                 for file in self.new_entry.file:
                     path = RelPath(file)
                     if path.path.stem == self.largs.label:
                         LOGGER.info("Also renaming associated file '%s'.", str(path))
                         target = RelPath(path.path.parent / f"{self.new_entry.label}.pdf")
                         if target.path.exists():
```

### Comparing `cobib-4.0.0/src/cobib/commands/export.py` & `cobib-4.1.0/src/cobib/commands/export.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
 import argparse
 import logging
 from typing import List, Type
 from zipfile import ZipFile
 
 from rich.console import Console
-from rich.prompt import PromptBase
+from rich.prompt import PromptBase, PromptType
 from textual.app import App
 from typing_extensions import override
 
 from cobib.config import Event
 from cobib.database import Database, Entry
 from cobib.parsers.bibtex import BibtexParser
 from cobib.utils.journal_abbreviations import JournalAbbreviations
@@ -102,15 +102,15 @@
     name = "export"
 
     @override
     def __init__(
         self,
         *args: str,
         console: Console | App[None] | None = None,
-        prompt: Type[PromptBase[str]] | None = None,
+        prompt: Type[PromptBase[PromptType]] | None = None,
     ) -> None:
         super().__init__(*args, console=console, prompt=prompt)
 
         self.exported_entries: List[Entry] = []
         """A list of `cobib.database.Entry` objects which were exported by this command."""
 
     @override
```

### Comparing `cobib-4.0.0/src/cobib/commands/import_.py` & `cobib-4.1.0/src/cobib/commands/import_.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,19 +23,27 @@
    config.database.stringify.list_separator.file = ", "
    ```
    The above will separate file paths using `, ` but if you use a different separator (for example
    `;`) be sure to update this setting accordingly.
 
 ### Additional Options
 
-If you want to suppress the automatic download of attachments, specify the `--skip-download`
-argument like so:
+Since v4.1.0 you can suppress the automatic download of attachments via the
+`cobib.config.config.ImportCommandConfig.skip_download` setting. It defaults to `False` meaning that
+the attachments will be downloaded
+If you want to manually overwrite the configuration setting you can do so with the `--skip-download`
+and `--force-download` arguments, respectively.
+I.e. the following will **not** download attachments:
 ```
 cobib import --skip-download --zotero
 ```
+While the next command will always download attachments:
+```
+cobib import --force-download --zotero
+```
 
 The various importers may take even more command line arguments. Please check out their
 documentation at `cobib.importers` for more details.
 
 ### TUI
 
 You can also trigger this command from the `cobib.ui.tui.TUI`.
@@ -51,33 +59,34 @@
 import argparse
 import inspect
 import logging
 from collections import OrderedDict
 from typing import Dict, List, Type
 
 from rich.console import Console
-from rich.prompt import PromptBase
+from rich.prompt import PromptBase, PromptType
 from textual.app import App
 from typing_extensions import override
 
 from cobib import importers
-from cobib.config import Event
+from cobib.config import Event, config
 from cobib.database import Database, Entry
 
 from .base_command import ArgumentParser, Command
 
 LOGGER = logging.getLogger(__name__)
 
 
 class ImportCommand(Command):
     """The ImportCommand.
 
     This command can parse the following arguments:
 
         * `--skip-download`: skips the automatic download of attached files (like PDFs).
+        * `--force-download`: forces the automatic download of attached files (like PDFs).
         * in addition to the options above, a *mutually exclusive group* of keyword arguments for
           all available `cobib.importers` are registered at runtime. Please check the output of
           `cobib import --help` for the exact list.
         * finally, you can add another set of positional arguments (preceded by `--`) which will be
           passed on to the chosen importer. For more details see for example
           `cobib import --zotero -- --help`.
     """
@@ -90,31 +99,40 @@
     """The available importers."""
 
     @override
     def __init__(
         self,
         *args: str,
         console: Console | App[None] | None = None,
-        prompt: Type[PromptBase[str]] | None = None,
+        prompt: Type[PromptBase[PromptType]] | None = None,
     ) -> None:
         super().__init__(*args, console=console, prompt=prompt)
 
         self.new_entries: Dict[str, Entry] = OrderedDict()
         """An `OrderedDict` mapping labels to `cobib.database.Entry` instances which were imported
         by this command."""
 
     @override
     @classmethod
     def init_argparser(cls) -> None:
         parser = ArgumentParser(prog="import", description="Import subcommand parser.")
-        parser.add_argument(
+        skip_download_group = parser.add_mutually_exclusive_group()
+        skip_download_group.add_argument(
             "--skip-download",
             action="store_true",
+            default=None,
             help="skip the automatic download of encountered PDF attachments",
         )
+        skip_download_group.add_argument(
+            "--force-download",
+            dest="skip_download",
+            action="store_false",
+            default=None,
+            help="force the automatic download of encountered PDF attachments",
+        )
         parser.add_argument(
             "importer_arguments",
             nargs="*",
             help="You can pass additional arguments to the chosen importer. To ensure this works as"
             " expected you should add the pseudo-argument '--' before the remaining arguments.",
         )
         group_import = parser.add_mutually_exclusive_group()
@@ -130,21 +148,29 @@
         # pylint: disable=invalid-overridden-method
         LOGGER.debug("Starting Import command.")
 
         Event.PreImportCommand.fire(self)
 
         imported_entries: List[Entry] = []
 
+        skip_download = config.commands.import_.skip_download
+        if self.largs.skip_download is not None:
+            skip_download = self.largs.skip_download
+        LOGGER.info(
+            "Associated files will%s be downloaded from the imported library.",
+            "" if skip_download else " not",
+        )
+
         for name, cls in ImportCommand._avail_importers.items():
             enabled = getattr(self.largs, name, False)
             if not enabled:
                 continue
             LOGGER.debug("Importing entries from %s.", name)
             imported_entries = await cls(
-                *self.largs.importer_arguments, skip_download=self.largs.skip_download
+                *self.largs.importer_arguments, skip_download=skip_download
             ).fetch()
             break
 
         bib = Database()
         existing_labels = set(bib.keys())
 
         for entry in imported_entries:
```

### Comparing `cobib-4.0.0/src/cobib/commands/init.py` & `cobib-4.1.0/src/cobib/commands/init.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 import logging
 import os
 import sys
 from pathlib import Path
 from typing import Type
 
 from rich.console import Console
-from rich.prompt import PromptBase
+from rich.prompt import PromptBase, PromptType
 from textual.app import App
 from typing_extensions import override
 
 from cobib.config import Event, config
 from cobib.utils.rel_path import RelPath
 
 from .base_command import ArgumentParser, Command
@@ -57,15 +57,15 @@
     name = "init"
 
     @override
     def __init__(
         self,
         *args: str,
         console: Console | App[None] | None = None,
-        prompt: Type[PromptBase[str]] | None = None,
+        prompt: Type[PromptBase[PromptType]] | None = None,
     ) -> None:
         super().__init__(*args, console=console, prompt=prompt)
 
         self.file: Path
         """The path to the database file."""
 
         self.root: Path
```

### Comparing `cobib-4.0.0/src/cobib/commands/list_.py` & `cobib-4.1.0/src/cobib/commands/list_.py`

 * *Files 14% similar despite different names*

```diff
@@ -67,44 +67,51 @@
 As of version v3.2.0, the filter arguments are evaluated as regex patterns allowing you to do things
 like the following:
 ```
 cobib list ++label "\D+_\d+"
 ```
 This will list all entries whose labels are formatted as `"<non-digit characters>_<digits>"`.
 
-As of version v4.0.0, you can provide the `--ignore-case` (or `-i`) argument to perform the filter
-matching case-**in**sensitive.
+As of version v4.0.0, you can make the filter matching case-**in**sensitive via the
+`cobib.config.config.ListCommandConfig.ignore_case` setting which defaults to being `False`.
+Besides this setting, you can always overwrite its value on the command line with the
+`--ignore-case` (`-i` for short) and `--no-ignore-case` (`-I` for short; since v4.1.0) options.
+Providing these options takes precedence over your configuration value.
+Thus, the following will *always* still match entries where `Rossmannek` is contained in the author
+field:
 ```
 cobib list --ignore-case ++author rossmannek
 ```
-This will still match entries where `Rossmannek` is contained in the author field.
-You can even enable this behavior by default using the
-`cobib.config.config.ListCommandConfig.ignore_case` setting.
+And the following will *always* be sensitive to case:
+```
+cobib list --no-ignore-case ++author rossmannek
+```
 
 .. note::
    For more information on the filtering mechanisms see also `cobib.database.Entry.matches`.
 """
 
 from __future__ import annotations
 
 import argparse
 import logging
 from collections import defaultdict
+from copy import copy
 from typing import Any, Dict, List, Optional, Set, Tuple, Type
 
 from rich.console import Console, ConsoleRenderable
-from rich.prompt import PromptBase
+from rich.prompt import PromptBase, PromptType
 from rich.table import Table
 from rich.text import Text
 from textual.app import App
-from textual.widgets import DataTable
 from typing_extensions import override
 
 from cobib.config import Event, config
 from cobib.database import Database, Entry
+from cobib.ui.components import ListView
 
 from .base_command import ArgumentParser, Command
 
 LOGGER = logging.getLogger(__name__)
 
 
 class ListCommand(Command):
@@ -116,32 +123,33 @@
           should be used for sorting the listed entries. This will automatically include a column
           for this field in the output table.
         * `-r`, `--reverse`: if specified, the entries will be listed in reverse order. This is
           especially useful in the TUI (where it is enabled by default) because it puts the last
           added entries at the top of the window. When using the command-line interface it is
           disabled by default, because this puts the last added entries at the bottom, just above
           the new command-line prompt.
-        * `-i`, `--ignore-case`: if specified, the entry matching will be case **in**sensitive. You
-          can enable this setting permanently via the
-          `cobib.config.config.ListCommandConfig.ignore_case` setting.
+        * `-i`, `--ignore-case`: if specified, the entry matching will be case-**in**sensitive. This
+          overwrites the `cobib.config.config.ListCommandConfig.ignore_case` setting.
+        * `-I`, `--no-ignore-case`: if specified, the entry matching will be case-sensitive. This
+          overwrites the `cobib.config.config.ListCommandConfig.ignore_case` setting.
         * `-x`, `--or`: if specified, multiple filters will be combined with logical OR rather than
           the default logical AND.
         * in addition to the options above, [Filter keyword arguments](#filters) are registered at
           runtime based on the fields available in the database. Please refer that section or the
           output of `cobib list --help` for more information.
     """
 
     name = "list"
 
     @override
     def __init__(
         self,
         *args: str,
         console: Console | App[None] | None = None,
-        prompt: Type[PromptBase[str]] | None = None,
+        prompt: Type[PromptBase[PromptType]] | None = None,
     ) -> None:
         super().__init__(*args, console=console, prompt=prompt)
 
         self.entries: List[Entry] = []
         """A list of entries, filtered and sorted according to the provided command arguments."""
 
         self.columns: List[str] = []
@@ -153,16 +161,29 @@
         parser = ArgumentParser(
             prog="list", description="List subcommand parser.", prefix_chars="+-"
         )
         parser.add_argument("-s", "--sort", help="specify column along which to sort the list")
         parser.add_argument(
             "-r", "--reverse", action="store_true", help="reverses the listing order"
         )
-        parser.add_argument(
-            "-i", "--ignore-case", action="store_true", help="ignore case for entry matching"
+        ignore_case_group = parser.add_mutually_exclusive_group()
+        ignore_case_group.add_argument(
+            "-i",
+            "--ignore-case",
+            action="store_true",
+            default=None,
+            help="ignore case for entry matching",
+        )
+        ignore_case_group.add_argument(
+            "-I",
+            "--no-ignore-case",
+            dest="ignore_case",
+            action="store_false",
+            default=None,
+            help="do NOT ignore case for entry matching",
         )
         parser.add_argument(
             "-x",
             "--or",
             dest="OR",
             action="store_true",
             help="concatenate filters with OR instead of AND",
@@ -195,19 +216,22 @@
         Event.PreListCommand.fire(self)
 
         filtered_entries, filtered_keys = self.filter_entries()
 
         self.entries = self._sort_entries(filtered_entries, self.largs.sort, self.largs.reverse)
 
         # construct list of columns to be displayed
-        self.columns = config.commands.list_.default_columns
+        self.columns = copy(config.commands.list_.default_columns)
+        LOGGER.debug("Listing the default columns: %s", str(self.columns))
         # display the column along which was sorted
         if self.largs.sort and self.largs.sort not in self.columns:
+            LOGGER.debug("Appending the column which is sorted by: %s", str(self.largs.sort))
             self.columns.append(self.largs.sort)
         # also display the keys which were used to filter
+        LOGGER.debug("Extendings the columns which are filtered by: %s", str(filtered_keys))
         self.columns.extend(col for col in filtered_keys if col not in self.columns)
 
         Event.PostListCommand.fire(self)
 
     def filter_entries(self) -> Tuple[List[Entry], Set[str]]:
         """The filtering method.
 
@@ -247,15 +271,20 @@
                         break
 
         LOGGER.debug("Final filter configuration: %s", dict(_filter))
 
         if self.largs.OR:
             LOGGER.debug("Filters are combined with logical ORs!")
 
-        ignore_case = config.commands.list_.ignore_case or self.largs.ignore_case
+        ignore_case = config.commands.list_.ignore_case
+        if self.largs.ignore_case is not None:
+            ignore_case = self.largs.ignore_case
+        LOGGER.debug(
+            "The entry matching will be performed case %ssensitive", "in" if ignore_case else ""
+        )
 
         for key, entry in Database().items():
             if entry.matches(_filter, self.largs.OR, ignore_case):
                 LOGGER.debug('Entry "%s" matches the filter.', key)
                 self.entries.append(entry)
 
         return self.entries, filtered_keys
@@ -272,19 +301,24 @@
             entries: the list of entries to be sorted.
             sort: the optional key by which to sort.
             reverse: whether or not to sort in reverse order.
 
         Returns:
             The sorted list of entries.
         """
+        if reverse:
+            LOGGER.debug("Reversing the entry order.")
+
         if sort is None:
             if reverse:
                 return entries[::-1]
             return entries
 
+        LOGGER.debug("Sorting entries by key '%s'.", sort)
+
         sorted_entries: List[Entry] = sorted(
             entries, reverse=reverse, key=lambda entry: entry.stringify().get(str(sort), "")
         )
 
         return sorted_entries
 
     @override
@@ -311,22 +345,16 @@
             stringified: Dict[str, str] = entry.stringify()
 
             rich_table.add_row(*(stringified.get(col, "") for col in self.columns))
 
         return rich_table
 
     @override
-    def render_textual(self) -> DataTable[Text]:
-        textual_table: DataTable[Text] = DataTable(id="cobib")
-        textual_table.cursor_type = "row"
-        textual_table.fixed_columns += 1
-        textual_table.zebra_stripes = True
-        # TODO: figure out why the following is necessary since the following commit:
-        # https://github.com/Textualize/textual/commit/a4252a5760539177f6db8231d4229e8eada923e7
-        textual_table.styles.height = "1fr"
+    def render_textual(self) -> ListView:
+        textual_table = ListView()
 
         for col in self.columns:
             textual_table.add_column(col, width=None)
 
         for entry in self.entries:
             stringified: Dict[str, str] = entry.stringify()
```

### Comparing `cobib-4.0.0/src/cobib/commands/modify.py` & `cobib-4.1.0/src/cobib/commands/modify.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,20 +30,29 @@
 # Rewrite the 'pages' field with a single-dash separator
 cobib modify "pages:{pages.replace('--', '-')}" -- ...
 
 # Rename an entry according to the first author's surname and year
 cobib modify "label:{author.split()[1]}{year}" -- ...
 ```
 
-In case you are applying a modification to your entry labels, but you want to avoid renaming all of
-your associated files, you can use the `--preserve-files` argument, like so:
+In case you are applying a modification to your entry labels, the value of the
+`cobib.config.config.ModifyCommandConfig.preserve_files` setting (added in v4.1.0) determines
+whether all of your associated files will be renamed accordingly. This defaults to `False`, meaning
+that they *will* be renamed. You can overwrite the value of this setting at runtime with the
+`--preserve-files` and `--no-preserve-files` arguments, respectively.
+I.e. the following will **not** rename your files:
 ```
 # Rename an entry according to the first author's surname and year, but preserve the original file
 cobib modify "label:{author.split()[1]}{year}" --preserve-files -- ...
 ```
+While this command will always rename them:
+```
+# Rename an entry according to the first author's surname and year, and rename the original file
+cobib modify "label:{author.split()[1]}{year}" --no-preserve-files -- ...
+```
 
 In combination with the regex-support for filters added during the same release, you can even unify
 your database's label convention:
 ```
 cobib modify "label:{label.replace('_', '')}" -- ++label "\D+_\d+"
 ```
 
@@ -78,19 +87,19 @@
 from __future__ import annotations
 
 import ast
 import logging
 from typing import Any, Callable, Dict, List, Optional, Tuple, Type
 
 from rich.console import Console
-from rich.prompt import PromptBase
+from rich.prompt import PromptBase, PromptType
 from textual.app import App
 from typing_extensions import override
 
-from cobib.config import Event
+from cobib.config import Event, config
 from cobib.database import Database, Entry
 from cobib.utils.logging import get_stream_handler
 from cobib.utils.rel_path import RelPath
 
 from .base_command import ArgumentParser, Command
 from .list_ import ListCommand
 
@@ -106,30 +115,34 @@
           should be applied to all matching entries. By default, the modification will overwrite any
           existing data in the specified `field` with the new `value`. For more information about
           formatting options of `<value>` refer to the module documentation or the man-page.
         * `--dry`: run in "dry"-mode which lists modifications without applying them.
         * `-a`, `--add`: when specified, the modification's value will be added to the entry's field
           rather than overwrite it. If the field in question is numeric, the numbers will be added.
         * `--preserve-files`: skips the renaming of any associated files in case the applied
-            modification acted on the entry labels.
+          modification acted on the entry labels. This overwrites the
+          `cobib.config.config.ModifyCommandConfig.preserve_files` setting.
+        * `--no-preserve-files`: does NOT skip the renaming of any associated files in case the
+          applied modification acted on the entry labels. This overwrites the
+          `cobib.config.config.ModifyCommandConfig.preserve_files` setting.
         * `-s`, `--selection`: when specified, the positional arguments will *not* be interpreted as
           filters but rather as a direct list of entry labels. This can be used on the command-line
           but is mainly meant for the TUIs visual selection interface (hence the name).
         * in addition to the above, you can add `filters` to specify a subset of your database for
           exporting. For more information refer to `cobib.commands.list_`.
     """
 
     name = "modify"
 
     @override
     def __init__(
         self,
         *args: str,
         console: Console | App[None] | None = None,
-        prompt: Type[PromptBase[str]] | None = None,
+        prompt: Type[PromptBase[PromptType]] | None = None,
     ) -> None:
         super().__init__(*args, console=console, prompt=prompt)
 
         self.modified_entries: List[Entry] = []
         """A list of `cobib.database.Entry` objects which were modified by this command."""
 
     @staticmethod
@@ -172,16 +185,27 @@
         )
         parser.add_argument(
             "-a",
             "--add",
             action="store_true",
             help="Adds to the modified field rather than overwriting it.",
         )
-        parser.add_argument(
-            "--preserve-files", action="store_true", help="do not rename associated files"
+        preserve_files_group = parser.add_mutually_exclusive_group()
+        preserve_files_group.add_argument(
+            "--preserve-files",
+            action="store_true",
+            default=None,
+            help="do NOT rename associated files",
+        )
+        preserve_files_group.add_argument(
+            "--no-preserve-files",
+            dest="preserve_files",
+            action="store_false",
+            default=None,
+            help="rename associated files",
         )
         parser.add_argument(
             "-s",
             "--selection",
             action="store_true",
             help="When specified, the `filter` argument will be interpreted as a list of entry "
             "labels rather than arguments for the `list` command.",
@@ -222,14 +246,19 @@
         else:
             LOGGER.debug("Gathering filtered list of entries to be modified.")
             filtered_entries, _ = ListCommand(*self.largs.filter).filter_entries()
             labels = [entry.label for entry in filtered_entries]
 
         field, value = self.largs.modification
 
+        preserve_files = config.commands.modify.preserve_files
+        if self.largs.preserve_files is not None:
+            preserve_files = self.largs.preserve_files
+        LOGGER.info("Associated files will%s be preserved.", "" if preserve_files else " not")
+
         bib = Database()
 
         for label in labels:  # pylint: disable=too-many-nested-blocks
             try:
                 entry = bib[label]
                 local_value = evaluate_as_f_string(value, {"label": label, **entry.data.copy()})
 
@@ -297,15 +326,15 @@
                         )
                     entry.data[field] = new_value
 
                 bib.update({entry.label: entry})
 
                 if entry.label != label:
                     bib.rename(label, entry.label)
-                    if not self.largs.preserve_files:
+                    if not preserve_files:
                         new_files = []
                         for file in entry.file:
                             path = RelPath(file)
                             if path.path.stem == label:
                                 LOGGER.info("Also renaming associated file '%s'.", str(path))
                                 target = RelPath(path.path.parent / f"{entry.label}.pdf")
                                 if target.path.exists():
```

### Comparing `cobib-4.0.0/src/cobib/commands/open.py` & `cobib-4.1.0/src/cobib/commands/open.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/src/cobib/commands/redo.py` & `cobib-4.1.0/src/cobib/commands/redo.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import logging
 import subprocess
 import sys
 from pathlib import Path
 from typing import Type
 
 from rich.console import Console
-from rich.prompt import PromptBase
+from rich.prompt import PromptBase, PromptType
 from textual.app import App
 from typing_extensions import override
 
 from cobib.config import Event, config
 from cobib.database import Database
 from cobib.utils.rel_path import RelPath
 
@@ -50,15 +50,15 @@
     name = "redo"
 
     @override
     def __init__(
         self,
         *args: str,
         console: Console | App[None] | None = None,
-        prompt: Type[PromptBase[str]] | None = None,
+        prompt: Type[PromptBase[PromptType]] | None = None,
     ) -> None:
         super().__init__(*args, console=console, prompt=prompt)
 
         self.root: Path
         """The path to the root of the git repository tracking the database."""
 
         self.sha: str
```

### Comparing `cobib-4.0.0/src/cobib/commands/search.py` & `cobib-4.1.0/src/cobib/commands/search.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,28 +4,36 @@
 While doing so, it uses the `cobib.config.config.SearchCommandConfig.grep` tool to search associated
 files, too.
 
 As a simple example, you can query for a simple author name like so:
 ```
 cobib search Einstein
 ```
-You can make the search case *in*sensitive in two ways:
-
-1. By enabling `cobib.config.config.SearchCommandConfig.ignore_case`.
-
-2. By providing the `--ignore-case` command-line argument:
+You can also control whether the search is performed case *in*sensitive.
+This is done via the `cobib.config.config.SearchCommandConfig.ignore_case` setting which defaults to
+being `False`.
+Besides this setting, you can always overwrite its value on the command line with the
+`--ignore-case` (`-i` for short) and `--no-ignore-case` (`-I` for short; since v4.1.0) options.
+Providing these options takes precedence over your configuration value.
+Thus, the following is *always* case *in*sensitive, irrespective of your configuration.
 ```
 cobib search --ignore-case Einstein
 ```
+And the following is *always* sensitive to case:
+```
+cobib search --no-ignore-case Einstein
+```
 
 By default, the search command will provide you with 1 line of context above and below the actual
 matches. You can change this number of lines by setting the `--context` option:
 ```
 cobib search --context 4 Einstein
 ```
+You can also permanently change the default value via the
+`cobib.config.config.SearchCommandConfig.context` setting.
 
 Finally, you can also combine the search with coBib's filtering mechanism to narrow your search down
 to a subset of your database:
 ```
 cobib search Einstein -- ++year 2020
 ```
 Note, that we use the auxiliary `--` argument to separate the filters from the actual arguments.
@@ -49,24 +57,24 @@
 from __future__ import annotations
 
 import argparse
 import logging
 from typing import List, Type
 
 from rich.console import Console, ConsoleRenderable
-from rich.prompt import PromptBase
+from rich.prompt import PromptBase, PromptType
 from rich.text import Text
-from rich.tree import Tree as RichTree
+from rich.tree import Tree
 from textual.app import App
-from textual.widgets import Tree as TextualTree
 from typing_extensions import override
 
 from cobib import __version__
 from cobib.config import Event, config
 from cobib.database import Entry
+from cobib.ui.components import SearchView
 
 from .base_command import ArgumentParser, Command
 from .list_ import ListCommand
 
 LOGGER = logging.getLogger(__name__)
 
 
@@ -74,31 +82,34 @@
     """The Search Command.
 
     This command can parse the following arguments:
 
         * `query`: the required positional argument corresponds to the regex-interpreted text which
           will be searched for. You may provide multiple separate queries which will be searched for
           independently.
-        * `-i`, `--ignore-case`: if specified, the search will be case *in*sensitive. You can enable
-          this setting permanently with `cobib.config.config.SearchCommandConfig.ignore_case`.
+        * `-i`, `--ignore-case`: if specified, the search will be case-**in**sensitive. This
+          overwrites the `cobib.config.config.SearchCommandConfig.ignore_case` setting.
+        * `-I`, `--no-ignore-case`: if specified, the search will be case-sensitive. This
+          overwrites the `cobib.config.config.SearchCommandConfig.ignore_case` setting.
         * `-c`, `--context`: you can specify the number of lines of "context" which is the number of
           lines before and after the actual match to be included in the output. This is similar to
-          the `-C` option of `grep`.
+          the `-C` option of `grep`. You can configure the default value via the
+          `cobib.config.config.SearchCommandConfig.context` setting.
         * in addition to the above, you can add `filters` to narrow the search down to a subset of
           your database. For more information refer to `cobib.commands.list_`.
     """
 
     name = "search"
 
     @override
     def __init__(
         self,
         *args: str,
         console: Console | App[None] | None = None,
-        prompt: Type[PromptBase[str]] | None = None,
+        prompt: Type[PromptBase[PromptType]] | None = None,
     ) -> None:
         super().__init__(*args, console=console, prompt=prompt)
 
         self.entries: List[Entry] = []
         """A filtered list of entries searched over by this command."""
 
         self.matches: List[List[List[str]]] = []
@@ -111,22 +122,35 @@
         """The number of search hits detected by this command."""
 
     @override
     @classmethod
     def init_argparser(cls) -> None:
         parser = ArgumentParser(prog="search", description="Search subcommand parser.")
         parser.add_argument("query", type=str, nargs="+", help="text to search for")
-        parser.add_argument(
-            "-i", "--ignore-case", action="store_true", help="ignore case for searching"
+        ignore_case_group = parser.add_mutually_exclusive_group()
+        ignore_case_group.add_argument(
+            "-i",
+            "--ignore-case",
+            action="store_true",
+            default=None,
+            help="ignore case for searching",
+        )
+        ignore_case_group.add_argument(
+            "-I",
+            "--no-ignore-case",
+            dest="ignore_case",
+            action="store_false",
+            default=None,
+            help="do NOT ignore case for searching",
         )
         parser.add_argument(
             "-c",
             "--context",
             type=int,
-            default=1,
+            default=config.commands.search.context,
             help="number of context lines to provide for each match",
         )
         parser.add_argument(
             "filter",
             nargs="*",
             help="You can specify filters as used by the `list` command in order to select a "
             "subset of labels to be modified. To ensure this works as expected you should add the "
@@ -158,15 +182,17 @@
     def execute(self) -> None:
         LOGGER.debug("Starting Search command.")
 
         Event.PreSearchCommand.fire(self)
 
         self.entries, _ = ListCommand(*self.largs.filter).filter_entries()
 
-        ignore_case = config.commands.search.ignore_case or self.largs.ignore_case
+        ignore_case = config.commands.search.ignore_case
+        if self.largs.ignore_case is not None:
+            ignore_case = self.largs.ignore_case
         LOGGER.debug("The search will be performed case %ssensitive", "in" if ignore_case else "")
 
         for entry in self.entries.copy():
             matches = entry.search(self.largs.query, self.largs.context, ignore_case)
             if not matches:
                 self.entries.remove(entry)
                 continue
@@ -189,17 +215,19 @@
                 for line in match:
                     output.append(f"{idx+1}::" + line.strip())
 
         return output
 
     @override
     def render_rich(self) -> ConsoleRenderable:
-        ignore_case = config.commands.search.ignore_case or self.largs.ignore_case
+        ignore_case = config.commands.search.ignore_case
+        if self.largs.ignore_case is not None:
+            ignore_case = self.largs.ignore_case
 
-        tree = RichTree(".", hide_root=True)
+        tree = Tree(".", hide_root=True)
         for entry, matches in zip(self.entries, self.matches):
             subtree = tree.add(
                 Text.assemble(
                     (entry.label, config.commands.search.highlights.label),
                     f" - {len(matches)} match" + ("es" if len(matches) > 1 else ""),
                 )
             )
@@ -214,20 +242,20 @@
                         case_sensitive=not ignore_case,
                     )
                     matchtree.add(line_text)
 
         return tree
 
     @override
-    def render_textual(self) -> TextualTree[Text]:
-        ignore_case = config.commands.search.ignore_case or self.largs.ignore_case
+    def render_textual(self) -> SearchView:
+        ignore_case = config.commands.search.ignore_case
+        if self.largs.ignore_case is not None:
+            ignore_case = self.largs.ignore_case
 
-        # TODO: figure out how to deal with multi-line tree node contents
-        tree: TextualTree[Text] = TextualTree(".")
-        tree.show_root = False
+        tree = SearchView(".")
         for entry, matches in zip(self.entries, self.matches):
             subtree = tree.root.add(
                 Text.assemble(
                     (entry.label, config.commands.search.highlights.label),
                     f" - {len(matches)} match" + ("es" if len(matches) > 1 else ""),
                 ),
                 # TODO: make configurable
```

### Comparing `cobib-4.0.0/src/cobib/commands/show.py` & `cobib-4.1.0/src/cobib/commands/show.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from __future__ import annotations
 
 import logging
 from typing import List, Type
 
 from rich.console import Console, ConsoleRenderable
-from rich.prompt import PromptBase
+from rich.prompt import PromptBase, PromptType
 from rich.syntax import Syntax
 from textual.app import App
 from typing_extensions import override
 
 from cobib import __version__
 from cobib.config import Event
 from cobib.database import Database
@@ -43,15 +43,15 @@
     name = "show"
 
     @override
     def __init__(
         self,
         *args: str,
         console: Console | App[None] | None = None,
-        prompt: Type[PromptBase[str]] | None = None,
+        prompt: Type[PromptBase[PromptType]] | None = None,
     ) -> None:
         super().__init__(*args, console=console, prompt=prompt)
 
         self.entry_str: str = ""
         """The string-formatted `cobib.database.Entry` shown by this command."""
 
     @override
```

### Comparing `cobib-4.0.0/src/cobib/commands/undo.py` & `cobib-4.1.0/src/cobib/commands/undo.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 import logging
 import subprocess
 import sys
 from pathlib import Path
 from typing import Type
 
 from rich.console import Console
-from rich.prompt import PromptBase
+from rich.prompt import PromptBase, PromptType
 from textual.app import App
 from typing_extensions import override
 
 from cobib.config import Event, config
 from cobib.database import Database
 from cobib.utils.rel_path import RelPath
 
@@ -57,15 +57,15 @@
     name = "undo"
 
     @override
     def __init__(
         self,
         *args: str,
         console: Console | App[None] | None = None,
-        prompt: Type[PromptBase[str]] | None = None,
+        prompt: Type[PromptBase[PromptType]] | None = None,
     ) -> None:
         super().__init__(*args, console=console, prompt=prompt)
 
         self.root: Path
         """The path to the root of the git repository tracking the database."""
 
         self.sha: str
```

### Comparing `cobib-4.0.0/src/cobib/config/__init__.py` & `cobib-4.1.0/src/cobib/config/__init__.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/src/cobib/config/config.py` & `cobib-4.1.0/src/cobib/config/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -90,34 +90,96 @@
         self._assert(
             self.version is None or isinstance(self.version, str),
             "config.logging.version should be a string or `None`.",
         )
 
 
 @dataclass
+class AddCommandConfig(_ConfigBase):
+    """The `config.commands.add` section."""
+
+    skip_download: bool = False
+    """Specifies whether to skip the attempt of downloading PDF files of added entries."""
+
+    @override
+    def validate(self) -> None:
+        LOGGER.debug("Validating the COMMANDS.ADD configuration section.")
+        self._assert(
+            isinstance(self.skip_download, bool),
+            "config.commands.add.skip_download should be a boolean.",
+        )
+
+
+@dataclass
+class DeleteCommandConfig(_ConfigBase):
+    """The `config.commands.delete` section."""
+
+    confirm: bool = True
+    """Whether or not to confirm before deleting an entry."""
+
+    preserve_files: bool = False
+    """Specifies whether associated files should be preserved when deleting an entry."""
+
+    @override
+    def validate(self) -> None:
+        LOGGER.debug("Validating the COMMANDS.DELETE configuration section.")
+        self._assert(
+            isinstance(self.confirm, bool),
+            "config.commands.delete.confirm should be a boolean.",
+        )
+        self._assert(
+            isinstance(self.preserve_files, bool),
+            "config.commands.delete.preserve_files should be a boolean.",
+        )
+
+
+@dataclass
 class EditCommandConfig(_ConfigBase):
     """The `config.commands.edit` section."""
 
     default_entry_type: str = "article"
     """Specifies the default bibtex entry type."""
     editor: str = os.environ.get("EDITOR", "vim")
     """Specifies the editor program. Note, that this default will respect your `$EDITOR`
     environment setting and fall back to `vim` if that variable is not set."""
+    preserve_files: bool = False
+    """Specifies whether associated files should be preserved when renaming an entry during
+    editing."""
 
     @override
     def validate(self) -> None:
         LOGGER.debug("Validating the COMMANDS.EDIT configuration section.")
         self._assert(
             isinstance(self.default_entry_type, str),
             "config.commands.edit.default_entry_type should be a string.",
         )
         self._assert(
             isinstance(self.editor, str),
             "config.commands.edit.editor should be a string.",
         )
+        self._assert(
+            isinstance(self.preserve_files, bool),
+            "config.commands.edit.preserve_files should be a boolean.",
+        )
+
+
+@dataclass
+class ImportCommandConfig(_ConfigBase):
+    """The `config.commands.import` section."""
+
+    skip_download: bool = False
+    """Specifies whether to skip the attempt of downloading PDF files of imported entries."""
+
+    @override
+    def validate(self) -> None:
+        LOGGER.debug("Validating the COMMANDS.IMPORT configuration section.")
+        self._assert(
+            isinstance(self.skip_download, bool),
+            "config.commands.import.skip_download should be a boolean.",
+        )
 
 
 @dataclass
 class ListCommandConfig(_ConfigBase):
     """The `config.commands.list_` section."""
 
     default_columns: list[str] = field(default_factory=lambda: ["label", "title"])
@@ -135,14 +197,31 @@
         self._assert(
             isinstance(self.ignore_case, bool),
             "config.commands.list_.ignore_case should be a boolean.",
         )
 
 
 @dataclass
+class ModifyCommandConfig(_ConfigBase):
+    """The `config.commands.modify` section."""
+
+    preserve_files: bool = False
+    """Specifies whether associated files should be preserved when renaming an entry during
+    modifying."""
+
+    @override
+    def validate(self) -> None:
+        LOGGER.debug("Validating the COMMANDS.MODIFY configuration section.")
+        self._assert(
+            isinstance(self.preserve_files, bool),
+            "config.commands.modify.preserve_files should be a boolean.",
+        )
+
+
+@dataclass
 class OpenCommandConfig(_ConfigBase):
     """The `config.commands.open` section."""
 
     command: str = "xdg-open" if sys.platform.lower() == "linux" else "open"
     """Specifies the command used for opening files associated with your entries."""
     fields: list[str] = field(default_factory=lambda: ["file", "url"])
     """Specifies the entry fields which are to be checked for openable URLs."""
@@ -182,14 +261,17 @@
         )
 
 
 @dataclass
 class SearchCommandConfig(_ConfigBase):
     """The `config.commands.search` section."""
 
+    context: int = 1
+    """Specifies the default number of context line to provide for each search query match. This is
+    similar to the `-C` option of `grep`."""
     grep: str = "grep"
     """Specifies the grep tool used for searching through your database and associated files. The
     default tool (`grep`) will not provide results for attached PDFs but other tools such as
     [ripgrep-all](https://github.com/phiresky/ripgrep-all) will."""
     grep_args: list[str] = field(default_factory=list)
     """Specifies additional arguments for your grep command. Note, that GNU's grep understands
     extended regex patterns even without specifying `-E`."""
@@ -198,14 +280,18 @@
     highlights: SearchHighlightConfig = field(default_factory=lambda: SearchHighlightConfig())
     """The nested section for highlights used when displaying search results."""
 
     @override
     def validate(self) -> None:
         LOGGER.debug("Validating the COMMANDS.SEARCH configuration section.")
         self._assert(
+            isinstance(self.context, int) and self.context >= 0,
+            "config.commands.search.context should be a non-negative integer.",
+        )
+        self._assert(
             isinstance(self.grep, str),
             "config.commands.search.grep should be a string.",
         )
         self._assert(
             isinstance(self.grep_args, list),
             "config.commands.search.grep_args should be a list.",
         )
@@ -216,29 +302,42 @@
         self.highlights.validate()
 
 
 @dataclass
 class CommandConfig(_ConfigBase):
     """The `config.commands` section."""
 
+    add: AddCommandConfig = field(default_factory=lambda: AddCommandConfig())
+    """The nested section for settings related to the `add` command."""
+    delete: DeleteCommandConfig = field(default_factory=lambda: DeleteCommandConfig())
+    """The nested section for settings related to the `delete` command."""
     edit: EditCommandConfig = field(default_factory=lambda: EditCommandConfig())
     """The nested section for settings related to the `edit` command."""
+    import_: ImportCommandConfig = field(default_factory=lambda: ImportCommandConfig())
+    """The nested section for settings related to the `import` command. Note the trailing underscore
+    of its name, since this attribute would otherwise clash with the builtin `import` keyword."""
     list_: ListCommandConfig = field(default_factory=lambda: ListCommandConfig())
     """The nested section for settings related to the `list` command. Note the trailing underscore
     of its name, since this attribute would otherwise clash with the builtin `list` keyword."""
+    modify: ModifyCommandConfig = field(default_factory=lambda: ModifyCommandConfig())
+    """The nested section for settings related to the `modify` command."""
     open: OpenCommandConfig = field(default_factory=lambda: OpenCommandConfig())
     """The nested section for settings related to the `open` command."""
     search: SearchCommandConfig = field(default_factory=lambda: SearchCommandConfig())
     """The nested section for settings related to the `search` command."""
 
     @override
     def validate(self) -> None:
         LOGGER.debug("Validating the COMMANDS configuration section.")
+        self.add.validate()
+        self.delete.validate()
         self.edit.validate()
+        self.import_.validate()
         self.list_.validate()
+        self.modify.validate()
         self.open.validate()
         self.search.validate()
 
 
 class LabelSuffix(Enum):
     """Suffixes to disambiguate `cobib.database.Entry` labels."""
```

### Comparing `cobib-4.0.0/src/cobib/config/event.py` & `cobib-4.1.0/src/cobib/config/event.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/src/cobib/config/example.py` & `cobib-4.1.0/src/cobib/config/example.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,32 +30,49 @@
 # You can also set the location for the cached version number based on which coBib shows you the
 # latest changes. You can set this to `None` to disable this functionality entirely.
 config.logging.version = "~/.cache/cobib/version"
 
 # COMMANDS
 # These settings affect some command specific behavior.
 
+# You can specify whether the automatic file download should be skipped during entry addition.
+config.commands.add.skip_download = False
+
+# You can specify whether you should be prompted for confirmation before deleting an entry.
+config.commands.delete.confirm = True
+# You can specify whether associated files should be preserved during entry deletion.
+config.commands.delete.preserve_files = False
+
 # You can specify the default bibtex entry type.
 config.commands.edit.default_entry_type = "article"
-
-# You can specify the editor program.
+# You can specify the editor program. Note, that this default will respect your `$EDITOR`
+# environment setting and fall back to `vim` if that variable is not set.
 config.commands.edit.editor = os.environ.get("EDITOR", "vim")
-# Note, that this default will respect your `$EDITOR` environment setting and fall back to `vim` if
-# that variable is not set.
+# You can specify whether associated files should be preserved when renaming during editing.
+config.commands.edit.preserve_files = False
+
+# You can specify whether downloading of attachments inside the imported library should be skipped.
+config.commands.import_.skip_download = False
 
 # You can configure the default columns displayed during the list command.
 config.commands.list_.default_columns = ["label", "title"]
 # You can specify whether filter matching should be performed case-insensitive.
 config.commands.list_.ignore_case = False
 
+# You can specify whether associated files should be preserved when renaming during modifying.
+config.commands.modify.preserve_files = False
+
 # You can specify a custom command which will be used to `open` files associated with your entries.
 config.commands.open.command = "xdg-open" if sys.platform.lower() == "linux" else "open"
 # You can specify the names of the data fields which are to be checked for openable URLs.
 config.commands.open.fields = ["file", "url"]
 
+# You can specify the default number of context lines to be provided for each search query match.
+# This is similar to the `-C` option of `grep`.
+config.commands.search.context = 1
 # You can specify a custom grep tool which will be used to search through your database and any
 # associated files. The default tool (`grep`) will not provide results for attached PDFs but other
 # tools such as [ripgrep-all](https://github.com/phiresky/ripgrep-all) will.
 config.commands.search.grep = "grep"
 # If you want to specify additional arguments for your grep command, you can specify them as a list
 # of strings in the following setting. Note, that GNU's grep understands extended regex patterns
 # even without specifying `-E`.
```

### Comparing `cobib-4.0.0/src/cobib/database/database.py` & `cobib-4.1.0/src/cobib/database/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,19 @@
 
         Args:
             old_label: the previous label.
             new_label: the new label.
         """
         LOGGER.debug("Renaming entry '%s' to '%s'.", old_label, new_label)
         Database._unsaved_entries[old_label] = new_label
+        if new_label != old_label:
+            # NOTE: this is not technically needed but the rename method is exploited during
+            # database linting with "fake" renames in order to register entries for re-writing
+            # during saving
+            super().pop(old_label)
 
     def disambiguate_label(self, label: str, entry: cobib.database.Entry) -> str:
         """Disambiguate a given label to ensure it becomes unique.
 
         This function ensures that a label is unique by appending a configurable suffix to a label
         if it is already present in the database at runtime.
```

### Comparing `cobib-4.0.0/src/cobib/database/entry.py` & `cobib-4.1.0/src/cobib/database/entry.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/src/cobib/importers/base_importer.py` & `cobib-4.1.0/src/cobib/importers/base_importer.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/src/cobib/importers/zotero.py` & `cobib-4.1.0/src/cobib/importers/zotero.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,15 +198,15 @@
                 continue
 
             url = encountered_attachments[key]["href"]
             filename = encountered_attachments[key]["title"]
 
             path = await FileDownloader().download(url, filename, headers=self.authentication)
             if path is not None:
-                entry.data["file"] = str(path)
+                entry.file = str(path)  # type: ignore[assignment]
 
         Event.PostZoteroImport.fire(self)
 
         return self.imported_entries
 
     @staticmethod
     def _get_fresh_oauth_tokens() -> Dict[str, str]:  # pragma: no cover
```

### Comparing `cobib-4.0.0/src/cobib/parsers/__init__.py` & `cobib-4.1.0/src/cobib/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/src/cobib/parsers/arxiv.py` & `cobib-4.1.0/src/cobib/parsers/arxiv.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,31 +59,31 @@
         LOGGER.info("Gathering BibTex data for arXiv ID: %s.", arxiv_id)
         try:
             page = requests.get(ARXIV_URL + arxiv_id, timeout=10)
         except requests.exceptions.RequestException as err:
             LOGGER.error("An Exception occurred while trying to query the arXiv ID: %s.", arxiv_id)
             LOGGER.error(err)
             return OrderedDict()
-        xml = BeautifulSoup(page.text, features="html.parser")
+        xml = BeautifulSoup(page.text, features="xml")
         if xml.feed.entry.title.contents[0] == "Error":
             msg = (
                 "The arXiv API returned the following error: " + xml.feed.entry.summary.contents[0]
             )
             LOGGER.warning(msg)
             return OrderedDict()
         label = ""
         entry: Dict[str, Any] = {}
         entry["archivePrefix"] = "arXiv"
         for key in xml.feed.entry.findChildren(recursive=False):
-            if key.name == "arxiv:doi":
+            if "doi" in key.name:
                 entry["doi"] = str(key.contents[0])
             elif key.name == "id":
                 entry["arxivid"] = str(key.contents[0]).replace("http://arxiv.org/abs/", "")
                 entry["eprint"] = str(key.contents[0])
-            elif key.name == "arxiv:primary_category":
+            elif key.name == "primary_category":
                 entry["primaryClass"] = str(key.attrs["term"])
             elif key.name == "published":
                 # The year must also be stored as a string for compatibility reasons with
                 # bibtexparser. However, we perform a conversion to an integer first, to ensure that
                 # the year can actually be represented as such.
                 entry["year"] = int(key.contents[0].split("-")[0])
                 label += str(entry["year"])
```

### Comparing `cobib-4.0.0/src/cobib/parsers/base_parser.py` & `cobib-4.1.0/src/cobib/parsers/base_parser.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/src/cobib/parsers/bibtex.py` & `cobib-4.1.0/src/cobib/parsers/bibtex.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/src/cobib/parsers/doi.py` & `cobib-4.1.0/src/cobib/parsers/doi.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/src/cobib/parsers/isbn.py` & `cobib-4.1.0/src/cobib/parsers/isbn.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/src/cobib/parsers/url.py` & `cobib-4.1.0/src/cobib/parsers/url.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/src/cobib/parsers/yaml.py` & `cobib-4.1.0/src/cobib/parsers/yaml.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/src/cobib/ui/__init__.py` & `cobib-4.1.0/src/cobib/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/src/cobib/ui/cli.py` & `cobib-4.1.0/src/cobib/ui/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 This class provides the main entry point to coBib. It exposes all the commands implemented in
 `cobib.commands` to the end-user and leverages [`rich`](https://github.com/textualize/rich) to
 produce beautiful output.
 """
 
 import argparse
 import asyncio
+import inspect
 import logging
 import sys
 from inspect import iscoroutinefunction
 from typing import Any
 
 from rich.console import Console
 from typing_extensions import override
 
 from cobib import __version__, commands
 from cobib.config import config
 from cobib.database import Database
 from cobib.ui.tui import TUI
 from cobib.ui.ui import UI
-from cobib.utils import shell_helper
 from cobib.utils.logging import print_changelog
 
 LOGGER = logging.getLogger(__name__)
 
 
 class CLI(UI):
     """The CLI class.
@@ -36,15 +36,15 @@
         is omitted, the `cobib.ui.tui.TUI` gets started.
     """
 
     @override
     def add_extra_parser_arguments(self) -> None:
         self.parser.add_argument("--version", action="version", version=f"%(prog)s v{__version__}")
 
-        subcommands = [cmd.split(":")[0] for cmd in shell_helper.list_commands()]
+        subcommands = [cls.name for _, cls in inspect.getmembers(commands) if inspect.isclass(cls)]
         self.parser.add_argument(
             "command", help="subcommand to be called", choices=subcommands, nargs="?"
         )
         self.parser.add_argument("args", nargs=argparse.REMAINDER)
 
     @override
     def __init__(self, *args: Any, **kwargs: Any) -> None:
```

### Comparing `cobib-4.0.0/src/cobib/ui/components/__init__.py` & `cobib-4.1.0/src/cobib/ui/components/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,16 +8,19 @@
    [`textual`](https://textual.textualize.io/) which is still in very early stages of its
    development, breaking API changes in this module might be released as part of coBib's feature
    releases. You have been warned.
 """
 
 from .argument_parser import ArgumentParser as ArgumentParser
 from .entry_view import EntryView as EntryView
-from .help_popup import HelpPopup as HelpPopup
-from .input import Input as Input
-from .main_view import MainView as MainView
+from .help_screen import HelpScreen as HelpScreen
+from .input_screen import InputScreen as InputScreen
+from .list_view import ListView as ListView
+from .main_content import MainContent as MainContent
+from .motion_key import MotionKey as MotionKey
 from .popup import Popup as Popup
 from .popup_logging_handler import PopupLoggingHandler as PopupLoggingHandler
 from .popup_panel import PopupPanel as PopupPanel
 from .progress import Progress as Progress
 from .prompt import Prompt as Prompt
+from .search_view import SearchView as SearchView
 from .selection_filter import SelectionFilter as SelectionFilter
```

### Comparing `cobib-4.0.0/src/cobib/ui/components/argument_parser.py` & `cobib-4.1.0/src/cobib/ui/components/argument_parser.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/src/cobib/ui/components/help_popup.py` & `cobib-4.1.0/src/cobib/ui/components/help_screen.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,53 +1,60 @@
-"""coBib's help popup.
+"""coBib's help screen.
 
-This widget renders a popup with the current key bindings and action descriptions.
+This screen renders a help information with the current key bindings and action descriptions.
 
 .. warning::
 
    This module makes no API stability guarantees! Refer to `cobib.ui.components` for more details.
 """
 
 from __future__ import annotations
 
-from typing import cast
-
 from rich.table import Table
-from textual.app import App, ComposeResult
-from textual.containers import Container
+from textual.app import ComposeResult
+from textual.screen import ModalScreen
 from textual.widgets import Static
 from typing_extensions import override
 
 
-class HelpPopup(Container, can_focus=False, can_focus_children=False):
-    """coBib's help popup."""
+class HelpScreen(ModalScreen[None]):
+    """coBib's help screen."""
+
+    BINDINGS = [
+        ("question_mark", "toggle_help", "Help"),
+    ]
+    """
+    | Key(s) | Description |
+    | :- | :- |
+    | ? | Toggles the help screen. |
+    """
 
     DEFAULT_CSS = """
-        HelpPopup {
-            layer: overlay;
-            background: blue 25%;
-            height: auto;
-            width: 100%;
+        HelpScreen {
+            align: center middle;
         }
 
-        HelpPopup.-hidden {
-            offset-y: 100%;
+        #help {
+            padding: 1 2;
+            width: auto;
+            height: auto;
+            background: $surface;
         }
     """
 
     HELP_DESCRIPTIONS = [
         ("q", "Quit's coBib"),
-        ("question_mark", "Toggles the help page"),
+        ("question_mark", "Toggles the help screen"),
         ("underscore", "Toggles between the horizontal and vertical layout"),
         ("space", "Toggles folding of a search result"),
         ("colon", "Starts the prompt for an arbitrary coBib command"),
         ("v", "Selects the current entry"),
         ("slash", "Searches the database for the provided string"),
         ("a", "Prompts for a new entry to be added to the database"),
-        ("d", "Delete the current (or selected) entries"),
+        ("d", "Deletes the current (or selected) entries"),
         ("e", "Edits the current entry"),
         ("f", "Allows filtering the table using `++/--` keywords"),
         ("i", "Imports entries from another source"),
         ("m", "Prompts for a modification (respects selection)"),
         ("o", "Opens the current (or selected) entries"),
         ("r", "Redoes the last undone change. Requires git-tracking!"),
         ("s", "Prompts for the field to sort by (use -r to list in reverse)"),
@@ -58,18 +65,22 @@
         ("h", "Moves to the left"),
         ("l", "Moves to the right"),
     ]
     """The key binding help descriptions."""
 
     @override
     def compose(self) -> ComposeResult:
-        help_table = Table(title="coBib TUI Help")
+        help_table = Table(title="coBib TUI Help", caption="Close this help by pressing '?'")
         help_table.add_column("Key")
         help_table.add_column("Description")
-        if self.parent is None:
-            raise KeyError
-        app = cast(App[None], self.parent.parent)
         for key, description in self.HELP_DESCRIPTIONS:
-            help_table.add_row(app.get_key_display(key), description)
-        static = Static(help_table)
+            help_table.add_row(self.app.get_key_display(key), description)
+        static = Static(help_table, id="help")
         static.styles.content_align = ("center", "middle")
         yield static
+
+    def action_toggle_help(self) -> None:
+        """Toggles the help information.
+
+        Since this is the action of the `HelpScreen`, it simply pops the screen.
+        """
+        self.app.pop_screen()
```

### Comparing `cobib-4.0.0/src/cobib/ui/components/popup.py` & `cobib-4.1.0/src/cobib/ui/components/popup.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/src/cobib/ui/components/popup_logging_handler.py` & `cobib-4.1.0/src/cobib/ui/components/popup_logging_handler.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/src/cobib/ui/components/popup_panel.py` & `cobib-4.1.0/src/cobib/ui/components/popup_panel.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/src/cobib/ui/components/selection_filter.py` & `cobib-4.1.0/src/cobib/ui/components/selection_filter.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/src/cobib/ui/shell_helper.py` & `cobib-4.1.0/src/cobib/ui/shell_helper.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/src/cobib/ui/tui.py` & `cobib-4.1.0/src/cobib/ui/tui.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,138 +15,159 @@
 
 import asyncio
 import io
 import logging
 import shlex
 import sys
 from contextlib import contextmanager, redirect_stderr, redirect_stdout
-from typing import Any, Iterator
+from typing import Any, Awaitable, Callable, Coroutine, Iterator, cast
 
 from rich.console import RenderableType
 from textual.app import App, ComposeResult
-from textual.binding import Binding
-from textual.coordinate import Coordinate
 from textual.css.query import NoMatches
+from textual.keys import Keys
+from textual.logging import TextualHandler
 from textual.widget import AwaitMount, Widget
-from textual.widgets import DataTable, Footer, Header, Tree
+from textual.widgets import Footer, Header, Input, Static
 from typing_extensions import override
 
 from cobib import commands
 from cobib.ui.components import (
     EntryView,
-    HelpPopup,
-    Input,
-    MainView,
+    HelpScreen,
+    InputScreen,
+    ListView,
+    MainContent,
+    MotionKey,
     Popup,
     PopupLoggingHandler,
     PopupPanel,
     Progress,
     Prompt,
+    SearchView,
     SelectionFilter,
 )
 from cobib.ui.ui import UI
 from cobib.utils.file_downloader import FileDownloader
 
 
 # NOTE: pylint and mypy are unable to understand that the `App` interface actually implements `run`
 # pylint: disable=abstract-method
 class TUI(UI, App[None]):  # type: ignore[misc]
     """The TUI class.
 
     This class does not support any extra command-line arguments compared to the base class.
     However, it also extends the `textual.app.App` interface. It can be used with the debugging
-    tools of textual but starting it requires a little bit of care because it depends on some setup
-    being done during `cobib.ui.cli.CLI.run` (which is the method from which the TUI gets started
-    during normal operation).
+    tools of textual but starting it requires you to use the `-c` (a.k.a. `--command`) argument of
+    `textual run` since `cobib` is installed as a command-line script.
 
     In short, here is how you can start the TUI using textual:
     ```
-    textual run "src/cobib/__main__.py"
+    textual run -c cobib
     ```
     This assumes that you are at the root of the cobib development folder. You can include
-    additional command-line arguments within the quotes as you desire.
+    additional command-line arguments after `cobib`, but when doing so you will need to put the
+    entire command in quotes, like this:
+    ```
+    textual run -c "cobib -v"
+    ```
 
     Adding the `--dev` argument to `textual run` will connect it to the debugging console which you
     can start in a separate shell via `textual console`.
+
+    For more information on how to debug a textual app, please refer to
+    [their documentation](https://textual.textualize.io/guide/devtools/).
     """
 
     DEFAULT_CSS = """
-    Screen {
-        layers: default popup overlay;
-        align-vertical: bottom;
-    }
+        Screen {
+            layers: default popup overlay;
+            align-vertical: bottom;
+        }
     """
 
-    # TODO: extract key bindings to widgets where appropriate
     BINDINGS = [
         ("q", "quit", "Quit"),
-        ("question_mark", "toggle_help", "Help"),
+        ("question_mark", "push_screen('help')", "Help"),
         ("underscore", "toggle_layout", "Layout"),
-        ("space", "toggle_fold", "Fold"),
         ("colon", "prompt(':')", "Prompt"),
         ("v", "select", "Select"),
         ("slash", "prompt('/')", "Search"),
         ("a", "prompt('add ')", "Add"),
         ("d", "delete", "Delete"),
         ("e", "edit", "Edit"),
         ("f", "filter", "Filter"),
         ("i", "prompt('import ')", "Import"),
         ("m", "prompt('modify ', False, True)", "Modify"),
         ("o", "open", "Open"),
         ("r", "prompt('redo', True)", "Redo"),
         ("s", "sort", "Sort"),
         ("u", "prompt('undo', True)", "Undo"),
         ("x", "prompt('export ', False, True)", "Export"),
-        Binding("j", "arrow_key('down')", "Down", show=False),
-        Binding("k", "arrow_key('up')", "Up", show=False),
-        Binding("h", "arrow_key('left')", "Left", show=False),
-        Binding("l", "arrow_key('right')", "Right", show=False),
-        Binding("down", "arrow_key('down')", "Down", show=False),
-        Binding("up", "arrow_key('up')", "Up", show=False),
-        Binding("left", "arrow_key('left')", "Left", show=False),
-        Binding("right", "arrow_key('right')", "Right", show=False),
     ]
+    """
+    | Key(s) | Description |
+    | :- | :- |
+    | q | Quit's coBib. |
+    | ? | Toggles the help screen. |
+    | _ | Toggles between the horizontal and vertical layout. |
+    | space | Toggles folding of a search result. |
+    | : | Starts the prompt for an arbitrary coBib command. |
+    | v | Selects the current entry. |
+    | / | Searches the database for the provided string. |
+    | a | Prompts for a new entry to be added to the database. |
+    | d | Deletes the current (or selected) entries. |
+    | e | Edits the current entry. |
+    | f | Allows filtering the table using `++/--` keywords. |
+    | i | Imports entries from another source. |
+    | m | Prompts for a modification (respects selection). |
+    | o | Opens the current (or selected) entries. |
+    | r | Redoes the last undone change. Requires git-tracking! |
+    | s | Prompts for the field to sort by (use -r to list in reverse). |
+    | u | Undes the last change. Requires git-tracking! |
+    | x | Exports the current (or selected) entries. |
+    """
+
+    SCREENS = {
+        "help": HelpScreen,
+        "input": InputScreen,
+    }
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         """Initializes the TUI.
 
         Args:
             *args: any positional arguments for textual's underlying `App` class.
             **kwargs: any keyword arguments for textual's underlying `App` class.
         """
         super().__init__(*args, **kwargs)
+        self.root_logger.addHandler(TextualHandler())
         self.title = "coBib"
         self.sub_title = "The Console Bibliography Manager"
         self._list_args = ["-r"]
         self._filter: SelectionFilter = SelectionFilter()
+        self._filters.append(self._filter)
         self._background_tasks: set[asyncio.Task] = set()  # type: ignore[type-arg]
         PopupLoggingHandler(self, level=logging.INFO)
-        Progress.console = self
+        FileDownloader.console = self
         FileDownloader.progress = Progress
 
     @override
     def compose(self) -> ComposeResult:
-        yield HelpPopup(classes="-hidden")
-
-        main = MainView()
-        yield main
+        with MainContent(initial=ListView.id):
+            yield ListView()
+            yield SearchView(".")
 
-        entry = EntryView()
-        yield entry
+        yield EntryView()
 
         yield PopupPanel()
 
         yield Header()
         yield Footer()
 
-        command = commands.ListCommand(*self._list_args)
-        command.execute()
-        table = command.render_textual()
-        main.mount(table)
-
     # TODO: remove once https://github.com/Textualize/textual/pull/1541 is merged into Textual
     @contextmanager
     def suspend(self) -> Iterator[None]:
         """Temporarily suspends the application.
 
         .. warning::
 
@@ -174,140 +195,84 @@
             action.
         """
         if isinstance(renderable, Widget):
             popup = renderable
         else:
             popup = Popup(renderable, level=0, timer=None)
 
-        await_mount = self.query_one(PopupPanel).mount(popup)
+        panel = self.screen.query_one(PopupPanel)
+
+        try:
+            await_mount = panel.mount(popup, before="#live")
+        except NoMatches:
+            await_mount = panel.mount(popup)
 
         return popup, await_mount
 
     # Event reaction methods
 
-    def on_mount(self) -> None:
+    def on_motion_key(self, event: MotionKey) -> None:
+        """Triggers on the custom `cobib.ui.components.motion_key.MotionKey` event.
+
+        This function will update the entry shown in the `cobib.ui.components.entry_view.EntryView`
+        widget. It only triggers on vertical motion keys.
+
+        Args:
+            event: the motion event.
+        """
+        if event.key in {Keys.Down, Keys.Up, Keys.PageDown, Keys.PageUp, Keys.Home, Keys.End}:
+            self._show_entry()
+
+    async def on_mount(self) -> None:
         """Triggers on the [`Mount`][1] event.
 
         This method takes care of initializing the desired layout and seeds the `EntryView` widget.
 
         [1]: https://textual.textualize.io/api/events/#textual.events.Mount
         """
         self.screen.styles.layout = "horizontal"
+        await self._update_table()
         self._show_entry()
 
-    def on_input_submitted(self, event: Input.Submitted) -> None:
-        """Triggers on the `cobib.ui.components.input.Input.Submitted` event.
-
-        This method parses the input value and extracts the command to be triggered as well as all
-        its arguments.
-
-        Args:
-            event: the triggering event.
-        """
-        event.input.remove()
-        if event.value[0] == "/":
-            event.value = "search " + event.value[1:]
-        elif event.value[0] == ":":
-            event.value = event.value[1:]
-
-        command = shlex.split(event.value)
-
-        if self._filter.active:
-            command += ["--"]
-            command.extend(list(self._filter.selection))
-            self._filter.active = False
-
-        if command and command[0]:
-            if command[0].lower() == "list":
-                self._list_args = command[1:]
-                self._update_table()
-            elif command[0].lower() == "search":
-                main = self.query_one(MainView)
-                main.clear()
-                subcmd = commands.SearchCommand(*command[1:])
-                subcmd.execute()
-                tree = subcmd.render_textual()
-                main.mount(tree)
-                self.refresh(layout=True)
-            else:
-                with redirect_stdout(io.StringIO()) as stdout:
-                    with redirect_stderr(io.StringIO()) as stderr:
-                        try:
-                            subcmd = getattr(commands, command[0].title() + "Command")(
-                                *command[1:], prompt=Prompt, console=self
-                            )
-
-                            task = asyncio.create_task(  # type: ignore[var-annotated]
-                                subcmd.execute()  # type: ignore[arg-type]
-                            )
-                            self._background_tasks.add(task)
-                            task.add_done_callback(self._background_tasks.discard)
-                            task.add_done_callback(lambda _: self._update_table)
-                        except SystemExit:
-                            pass
-                stdout_val = stdout.getvalue().strip()
-                if stdout_val:
-                    self.print(Popup(stdout_val, level=logging.INFO))
-                stderr_val = stderr.getvalue().strip()
-                if stderr_val:
-                    self.print(Popup(stderr_val, level=logging.CRITICAL))
-                self._update_table()
-
     # Action methods
 
-    def action_arrow_key(self, key_name: str) -> None:
-        """The movement action.
-
-        This method currently redirects to the widget mounted in the `MainView`.
-        The movement keys `h`, `j`, `k`, and `l` also redirect here.
-
-        .. warning::
-
-           This method is pending a refactoring during which the layouting will be redesigned in
-           favor of screens. Once that happens, the movement key bindings will be handled by the
-           widgets directly.
+    async def action_quit(self) -> None:
+        """Action to display the quit dialog."""
 
-           For more information refer to [this issue](https://gitlab.com/cobib/cobib/-/issues/111).
+        async def _prompt_quit() -> None:
+            res = await Prompt.ask(  # type: ignore[call-overload]
+                "Are you sure you want to quit?",
+                choices=["y", "n"],
+                default="y",
+                console=self,
+            )
+            if res == "y":
+                self.exit()
 
-        Args:
-            key_name: the name of the key triggering this action.
-        """
-        # TODO: handle scroll offset
-        main = self.query_one(MainView).children[0]
-        cursor_func = getattr(main, f"action_cursor_{key_name}", None)
-        if cursor_func is None:
-            return
-        cursor_func()
-        self._show_entry()
+        task = asyncio.create_task(_prompt_quit())
+        self._background_tasks.add(task)
+        task.add_done_callback(self._background_tasks.discard)
 
     def action_toggle_layout(self) -> None:
         """The layout toggling action.
 
         This action will toggle between a horizontal and vertical layout.
         """
-        # TODO: refactor how layout is done
         layout = self.screen.styles.layout
         if layout is None:
             return
+        main = self.query_one(MainContent)
         if layout.name.lower().startswith("horizontal"):
             self.screen.styles.layout = "vertical"
-            main = self.query_one(MainView)
             main.styles.height = "2fr"
             main.styles.width = "1fr"
-            entry = self.query_one(EntryView)
-            entry.styles.height = "1fr"
-            entry.styles.width = "1fr"
         elif layout.name.lower().startswith("vertical"):
             self.screen.styles.layout = "horizontal"
-            main = self.query_one(MainView)
             main.styles.width = "2fr"
             main.styles.height = "1fr"
-            entry = self.query_one(EntryView)
-            entry.styles.width = "1fr"
-            entry.styles.height = "1fr"
         self.refresh(layout=True)
 
     async def action_prompt(
         self, value: str, submit: bool = False, check_selection: bool = False
     ) -> None:
         """The prompt action.
 
@@ -323,105 +288,79 @@
                 immediately (i.e. `value` gets parsed directly).
             check_selection: whether or not to check for a visual selection.
         """
         if check_selection and self._filter.selection:
             self._filter.active = True
             value += "-s "
 
-        prompt = Input(value=value)
-        prompt.styles.layer = "overlay"
-        prompt.styles.dock = "bottom"  # type: ignore[arg-type]
-        prompt.styles.border = (None, None)
-        prompt.styles.padding = (0, 0)
-
-        await self.mount(prompt)
         if submit:
-            await prompt.action_submit()
+            await self._process_input(value)
         else:
-            prompt.focus()
-
-    def action_toggle_help(self) -> None:
-        """The help action.
-
-        This action toggles a help popup. Once opened, the same keybind needs to be pressed to close
-        it.
-        """
-        help_sidebar = self.query_one(HelpPopup)
-        self.set_focus(None)
-        if help_sidebar.has_class("-hidden"):
-            help_sidebar.remove_class("-hidden")
-        else:
-            help_sidebar.add_class("-hidden")
+            await_mount = self.push_screen("input", self._process_input)
+            inp_screen = cast(InputScreen, self.get_screen("input"))
+            inp_screen.escape_enabled = True
+            await await_mount
+            inp = inp_screen.query_one(Input)
+            inp.value = value
+            inp.action_end()
 
     async def action_select(self) -> None:
         """The selection action.
 
         This action adds the entry currently under the cursor to the visual selection.
         """
-        self._select_entry()
-
-    def action_toggle_fold(self) -> None:
-        """The folding action.
-
-        This action toggles the display of a node in the results tree of the
-        `cobib.commands.search.SearchCommand.render_textual`.
-
-        .. warning::
+        main = self.query_one(MainContent)
+        label = main.get_current_label()
 
-           This method is pending a refactoring during which the layouting will be redesigned in
-           favor of screens. Once that happens, this action will be moved to the widget returned by
-            `cobib.commands.search.SearchCommand.render_textual`.
+        if label in self._filter.selection:
+            self._filter.selection.remove(label)
+        else:
+            self._filter.selection.add(label)
 
-           For more information refer to [this issue](https://gitlab.com/cobib/cobib/-/issues/111).
-        """
-        # TODO: provide more ways to fold (e.g. recursively)
-        try:
-            main = self.query_one(MainView).query_one(Tree)
-            main.action_toggle_node()
-        except NoMatches:
-            pass
+        main.notify_style_update()
+        main.refresh()
+        self.query_one(EntryView).query_one(Static).refresh()
 
-    async def action_delete(self) -> None:
+    def action_delete(self) -> None:
         """The delete action.
 
         This action triggers the `cobib.commands.delete.DeleteCommand`.
         """
+        main = self.query_one(MainContent)
         labels: list[str]
         if self._filter.selection:
             labels = list(self._filter.selection)
             self._filter.selection.clear()
         else:
-            labels = [self._get_current_label()]
+            labels = [main.get_current_label()]
 
-        commands.DeleteCommand(*labels).execute()
-        self._update_table()
+        self._run_command(["delete"] + labels)
 
     async def action_edit(self) -> None:
         """The edit action.
 
         This action triggers the `cobib.commands.edit.EditCommand`.
         """
         self._edit_entry()
+        await self._update_table()
 
-    async def action_open(self) -> None:
+    def action_open(self) -> None:
         """The open action.
 
         This action triggers the `cobib.commands.open.OpenCommand`.
         """
+        main = self.query_one(MainContent)
         labels: list[str]
         if self._filter.selection:
             labels = list(self._filter.selection)
             self._filter.selection.clear()
         else:
-            labels = [self._get_current_label()]
+            labels = [main.get_current_label()]
 
-        open_cmd = commands.OpenCommand(*labels, prompt=Prompt, console=self)
-        task = asyncio.create_task(open_cmd.execute())
-        self._background_tasks.add(task)
-        task.add_done_callback(self._background_tasks.discard)
+        self._run_command(["open"] + labels)
 
     async def action_filter(self) -> None:
         """The filter action.
 
         This action triggers the `cobib.commands.list.ListCommand` via the `action_prompt` and
         allows the user to provide additional filters.
         """
@@ -433,14 +372,17 @@
         This action triggers the `cobib.commands.list.ListCommand` via the `action_prompt` and
         allows the user to provide a field to be sorted by. This command is handled specially
         because it ensures that only a single sort argument can be given at a time.
         """
         try:
             # first, remove any previously used sort argument
             sort_arg_idx = self._list_args.index("-s")
+            # NOTE: we need to pop twice in order to remove both: the `-s` option and the key which
+            # was sorted by
+            self._list_args.pop(sort_arg_idx)
             self._list_args.pop(sort_arg_idx)
         except ValueError:
             pass
 
         # add the sort option to the arguments
         self._list_args += ["-s"]
 
@@ -449,104 +391,129 @@
     # Utility methods
 
     def _edit_entry(self) -> None:
         """Edits the current entry.
 
         This method takes care of suspending the application in favor of the editor.
         """
-        label = self._get_current_label()
+        main = self.query_one(MainContent)
+        label = main.get_current_label()
         with self.suspend():
             commands.EditCommand(label).execute()
-        self.refresh(layout=True)
-
-    def _get_current_label(self) -> str:
-        """Gets the label of the entry currently under the cursor.
-
-        .. warning::
-
-           This method is pending a refactoring during which the layouting will be redesigned in
-           favor of screens. Once that happens, the responsibility of detecting the current label
-           will be delegated to the widget subclasses to be mounted on the respective screens.
-
-           For more information refer to [this issue](https://gitlab.com/cobib/cobib/-/issues/111).
-
-        Returns:
-            The label of the entry currently under the cursor.
-        """
-        label: str
-        try:
-            table = self.query_one(MainView).query_one(DataTable)
-            label = table.get_cell_at(Coordinate(table.cursor_row, 0)).plain
-        except NoMatches:
-            try:
-                tree = self.query_one(MainView).query_one(Tree)
-                previous_node, current_node = tree.cursor_node, tree.cursor_node
-                if current_node is None:
-                    raise NoMatches  # pylint: disable=raise-missing-from
-                while current_node.parent is not None:
-                    previous_node, current_node = current_node, current_node.parent
-                if previous_node is None:
-                    raise NoMatches  # pylint: disable=raise-missing-from
-                label = str(previous_node.label).split(" - ", maxsplit=1)[0]
-            except NoMatches as exc:
-                raise NoMatches from exc
-        return label
-
-    def _select_entry(self) -> None:
-        """Adds the entry currently under the cursor to the visual selection."""
-        try:
-            table = self.query_one(MainView).query_one(DataTable)
-            label = table.get_cell_at(Coordinate(table.cursor_row, 0)).plain
-            if label in self._filter.selection:
-                self._filter.selection.remove(label)
-            else:
-                self._filter.selection.add(label)
-            table.notify_style_update()
-            table.refresh()
-            self.query_one(EntryView).refresh()
-
-        except NoMatches:
-            try:
-                tree = self.query_one(MainView).query_one(Tree)
-                previous_node, current_node = tree.cursor_node, tree.cursor_node
-                if current_node is None:
-                    raise NoMatches  # pylint: disable=raise-missing-from
-                while current_node.parent is not None:
-                    previous_node, current_node = current_node, current_node.parent
-                if previous_node is None:
-                    raise NoMatches  # pylint: disable=raise-missing-from
-
-                label = str(previous_node.label).split(" - ", maxsplit=1)[0]
-
-                if label in self._filter.selection:
-                    self._filter.selection.remove(label)
-                else:
-                    self._filter.selection.add(label)
-
-                tree.notify_style_update()
-                tree.refresh()
-                self.query_one(EntryView).refresh()
-
-            except NoMatches as exc:
-                raise NoMatches from exc
 
     def _show_entry(self) -> None:
         """Renders the entry currently under the cursor in the `EntryView` widget."""
-        label = self._get_current_label()
+        main = self.query_one(MainContent)
+        label = main.get_current_label()
         show_cmd = commands.ShowCommand(label)
         show_cmd.execute()
         entry = self.query_one(EntryView)
-        entry.string = show_cmd.render_rich(
-            background_color=entry.background_colors[1].rich_color.name,
+        static = entry.query_one(Static)
+        static.update(
+            show_cmd.render_rich(
+                background_color=entry.background_colors[1].rich_color.name,
+            )
         )
 
-    def _update_table(self) -> None:
-        """Updates the list of entries displayed in the `MainView`."""
+    async def _update_table(self) -> None:
+        """Updates the list of entries displayed in the `MainContent`."""
         # TODO: retain scroll position
-        main = self.query_one(MainView)
-        main.clear()
         command = commands.ListCommand(*self._list_args)
         command.execute()
         table = command.render_textual()
-        main.mount(table)
-        main.focus()
+        main = self.query_one(MainContent)
+        await main.replace_widget(table)
+        table.focus()
+        self.refresh(layout=True)
+
+    async def _update_tree(self, command: list[str]) -> None:
+        """Updates the tree of search results displayed in the `MainContent`."""
+        subcmd = commands.SearchCommand(*command)
+        subcmd.execute()
+        tree = subcmd.render_textual()
+        main = self.query_one(MainContent)
+        await main.replace_widget(tree)
+        tree.focus()
         self.refresh(layout=True)
+
+    async def _process_input(self, value: str) -> None:
+        """Processes the input returned from the `cobib.ui.components.input_screen.InputScreen`.
+
+        Args:
+            value: the value put into the `Input` widget by the user.
+        """
+        if not value:
+            return
+
+        if value[0] == "/":
+            value = "search " + value[1:]
+        elif value[0] == ":":
+            value = value[1:]
+
+        command = shlex.split(value)
+
+        if self._filter.active:
+            command += ["--"]
+            command.extend(list(self._filter.selection))
+            self._filter.active = False
+
+        if command and command[0]:
+            if command[0].lower() == "list":
+                self._list_args = command[1:]
+                await self._update_table()
+            elif command[0].lower() == "search":
+                await self._update_tree(command[1:])
+            else:
+                self._run_command(command)
+
+    @staticmethod
+    async def _async_done_callback(
+        task: Awaitable[None], async_callback: Callable[[], Coroutine[Any, Any, None]]
+    ) -> None:
+        """Adds an asynchronous callback for when the provided task is done.
+
+        Args:
+            task: the Task to await before running the next coroutine.
+            async_callback: the asynchronous callback to run after the `task` has completed.
+        """
+        await task
+        await async_callback()
+
+    def _run_command(self, command: list[str]) -> None:
+        """Parses and executes a cobib command with its arguments.
+
+        This method also redirects `stdout` and `stderr` and captures their contents to be displayed
+        as popups in the TUI.
+
+        Args:
+            command: the list of command and its arguments.
+        """
+        with redirect_stdout(io.StringIO()) as stdout:
+            with redirect_stderr(io.StringIO()) as stderr:
+                try:
+                    subcmd = getattr(commands, command[0].title() + "Command")(
+                        *command[1:], prompt=Prompt, console=self
+                    )
+
+                    # 1. create subcommand execution task
+                    task1 = asyncio.create_task(subcmd.execute())
+
+                    # 2. create another task which chains an asynchronous callback after the
+                    #    previous one
+                    task2 = asyncio.create_task(TUI._async_done_callback(task1, self._update_table))
+
+                    # 3. ensure proper clean-up of all created tasks
+                    self._background_tasks.add(task1)
+                    task1.add_done_callback(self._background_tasks.discard)
+                    self._background_tasks.add(task2)
+                    task2.add_done_callback(self._background_tasks.discard)
+
+                except SystemExit:
+                    pass
+
+        stdout_val = stdout.getvalue().strip()
+        if stdout_val:
+            self.print(Popup(stdout_val, level=logging.INFO))
+
+        stderr_val = stderr.getvalue().strip()
+        if stderr_val:
+            self.print(Popup(stderr_val, level=logging.CRITICAL))
```

### Comparing `cobib-4.0.0/src/cobib/ui/ui.py` & `cobib-4.1.0/src/cobib/ui/ui.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/src/cobib/utils/diff_renderer.py` & `cobib-4.1.0/src/cobib/utils/diff_renderer.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/src/cobib/utils/file_downloader.py` & `cobib-4.1.0/src/cobib/utils/file_downloader.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """coBib's file downloader utility."""
 
 from __future__ import annotations
 
+import asyncio
 import logging
 import re
 import tempfile
-from functools import partial
 from pathlib import Path
-from typing import Callable, Dict, Optional, Type
+from typing import Dict, Optional, Type
 
 import requests
 from rich.console import Console
 from rich.progress import DownloadColumn, Progress, SpinnerColumn, TimeElapsedColumn
-from textual.widgets import ProgressBar
+from textual.app import App
 
 from cobib.config import Event, config
 
 from .rel_path import RelPath
 
 LOGGER = logging.getLogger(__name__)
 
@@ -36,17 +36,20 @@
         This method gets called when accessing `FileDownloader` and enforces the singleton pattern
         implemented by this class.
         """
         if cls._instance is None:
             cls._instance = super().__new__(cls)
         return cls._instance
 
-    progress: Type[Progress] | Type[ProgressBar] = Progress
+    progress: Type[Progress] = Progress
     """The type of progress bar to use when displaying the downloading progress."""
 
+    console: Console | App[None] = Console()
+    """The object via which to print output."""
+
     _PDF_MARKER = bytes("%PDF", "utf-8")
     """A marker which the downloaded file's beginning is checked against, to determine that it is
     indeed a PDF file."""
 
     @staticmethod
     def _assert_pdf(content: bytes) -> bool:
         """Asserts that the `content` starts with the `_PDF_MARKER`.
@@ -126,59 +129,53 @@
             except requests.exceptions.RequestException as err:
                 msg = f"An Exception occurred while downloading the file located at {url}"
                 LOGGER.warning(msg)
                 LOGGER.error(err)
                 FileDownloader._recover(path, backup)
                 return None
 
-            advance: Callable[[int], None]
-            progress_bar: Progress | ProgressBar
-            if issubclass(FileDownloader.progress, ProgressBar):
-                progress_bar = FileDownloader.progress(total_length)
-                _, await_mount = progress_bar.console.print(  # type: ignore[attr-defined]
+            progress_bar = FileDownloader.progress(
+                SpinnerColumn(),
+                *Progress.get_default_columns(),
+                TimeElapsedColumn(),
+                DownloadColumn(),
+            )
+            progress_bar.start()
+
+            if isinstance(FileDownloader.console, App):
+                # pylint: disable=assignment-from-no-return,unpacking-non-sequence
+                _, await_mount = FileDownloader.console.print(  # type: ignore[attr-defined]
                     progress_bar
                 )
                 await await_mount
-                advance = progress_bar.advance
-            else:
-                progress_bar = FileDownloader.progress(
-                    SpinnerColumn(),
-                    *Progress.get_default_columns(),
-                    TimeElapsedColumn(),
-                    DownloadColumn(),
-                    transient=False,
-                    # TODO: the unittests fail when this remains `None` because it appears as though
-                    # too many Live sessions are opened at once. How can we deal with this properly?
-                    # Can we simply assume the user is not going to do this in parallel?
-                    console=Console(),
-                )
-                progress_bar.start()
-                task = progress_bar.add_task("Downloading...", total=total_length)
-                advance = partial(progress_bar.advance, task)
+
+            task = progress_bar.add_task("Downloading...", total=total_length)
 
             accumulated_length = 0
 
             if total_length is None:
                 if not FileDownloader._assert_pdf(response.content):
                     FileDownloader._recover(path, backup)
+                    progress_bar.stop()
                     return None
                 file.write(response.content)
             else:
                 for data in response.iter_content(chunk_size=4096):
                     if accumulated_length == 0 and not FileDownloader._assert_pdf(data):
                         FileDownloader._recover(path, backup)
+                        progress_bar.stop()
                         return None
                     accumulated_length += len(data)
-                    advance(len(data))
+                    progress_bar.advance(task, len(data))
+                    await asyncio.sleep(0)
                     file.write(data)
 
-            if isinstance(progress_bar, ProgressBar):
-                progress_bar.set_timer(5.0, progress_bar.remove)
-            else:
-                progress_bar.stop()
+            progress_bar.stop()
+            if isinstance(FileDownloader.console, App):
+                progress_bar.set_timer(5.0, progress_bar.remove)  # type: ignore[attr-defined]
 
             msg = f"Successfully downloaded {path}"
             print(msg)
             LOGGER.info(msg)
 
             path = Event.PostFileDownload.fire(path) or path
```

### Comparing `cobib-4.0.0/src/cobib/utils/journal_abbreviations.py` & `cobib-4.1.0/src/cobib/utils/journal_abbreviations.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/src/cobib/utils/rel_path.py` & `cobib-4.1.0/src/cobib/utils/rel_path.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/src/cobib/utils/shell_helper.py` & `cobib-4.1.0/src/cobib/utils/shell_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,29 +10,34 @@
 import contextlib
 import inspect
 import logging
 from io import StringIO
 from typing import List, Set, Type
 
 from rich.console import Console
-from rich.prompt import PromptBase
+from rich.prompt import PromptBase, PromptType
 from textual.app import App
 
 from .rel_path import RelPath
 
+LOGGER = logging.getLogger(__name__)
+
 
 def list_commands(*args: str) -> List[str]:
     """Lists all available subcommands.
 
     Args:
         args: a sequence of additional arguments used for the execution. None are supported yet.
 
     Returns:
         The list of available commands.
     """
+    msg = "The _list_commands shell helper utility is deprecated and will be removed in the future!"
+    LOGGER.warning(msg)
+
     # pylint: disable=import-outside-toplevel
     from cobib import commands
 
     return [cls.name for _, cls in inspect.getmembers(commands) if inspect.isclass(cls)]
 
 
 def list_labels(*args: str) -> List[str]:
@@ -40,14 +45,17 @@
 
     Args:
         args: a sequence of additional arguments used for the execution. None are supported yet.
 
     Returns:
         The list of all labels.
     """
+    msg = "The _list_labels shell helper utility is deprecated and will be removed in the future!"
+    LOGGER.warning(msg)
+
     # pylint: disable=import-outside-toplevel
     from cobib.database import Database
 
     labels = list(Database().keys())
     return labels
 
 
@@ -56,14 +64,17 @@
 
     Args:
         args: a sequence of additional arguments used for the execution. None are supported yet.
 
     Returns:
         The list of all available filters.
     """
+    msg = "The _list_filters shell helper utility is deprecated and will be removed in the future!"
+    LOGGER.warning(msg)
+
     # pylint: disable=import-outside-toplevel
     from cobib.database import Database
 
     filters: Set[str] = {"label"}
     for entry in Database().values():
         filters.update(entry.data.keys())
     return filters
@@ -196,15 +207,15 @@
 
             name = "lint"
 
             def __init__(
                 self,
                 *args: str,
                 console: Console | App[None] | None = None,
-                prompt: Type[PromptBase[str]] | None = None,
+                prompt: Type[PromptBase[PromptType]] | None = None,
             ) -> None:
                 # pylint: disable=super-init-not-called
                 self.largs = largs
 
             @classmethod
             def init_argparser(cls) -> None:
                 pass
```

### Comparing `cobib-4.0.0/src/cobib.egg-info/PKG-INFO` & `cobib-4.1.0/src/cobib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cobib
-Version: 4.0.0
+Version: 4.1.0
 Summary: Console Bibliography
 Home-page: https://gitlab.com/cobib/cobib
 Author: Max Rossmannek
 Author-email: max.rossmannek@uzh.ch
 License: MIT License
 Project-URL: Bug Tracker, https://gitlab.com/cobib/cobib/-/issues
 Project-URL: Documentation, https://cobib.gitlab.io/cobib/cobib.html
@@ -51,16 +51,16 @@
 
 ```
 pip install cobib
 ```
 
 Note: Use `pip3` if you still have Python 2 installed.
 
-If you would also like to install the man-page and (crude!) Zsh completion,
-you need to download the source code and do the following:
+If you would also like to install the man-page, you need to download the source
+code and do the following:
 
 ```
 git clone https://gitlab.com/cobib/cobib
 cd cobib
 make install_extras
 ```
 
@@ -289,17 +289,74 @@
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
 
+## [4.1.0] - 2023-06-11
+
+Pypi: https://pypi.org/project/cobib/4.1.0/
+
+### Added
+- added the following settings which specify whether or not to preserve
+  associated files during the respective commands being run:
+  - `config.commands.delete.preserve_files`
+  - `config.commands.edit.preserve_files`
+  - `config.commands.modify.preserve_files`
+- added a confirmation prompt before deleting an entry (#110)
+  - this prompt can be disabled by setting `config.commands.delete.confirm` to `False`
+- added the `--no-ignore-case` (`-I` for short) command line options to the
+  `list` and `search` command (#116)
+- added the `--no-preserve-files` command line options to the `delete`, `edit`
+  and `modify` command (#116)
+- added the `config.commands.search.context` setting which configures the
+  default number of context lines to be provided for search query matches
+- added more options to configure the automatic download behavior:
+  - the new `config.commands.add.skip_download` setting
+  - the new `--force-download` option of the `add` command
+  - the new `config.commands.import_.skip_download` setting
+  - the new `--force-download` option of the `import` command
+- the user is asked for confirmation when quitting the TUI (!71)
+
+### Changed
+- refactored the TUI by leveraging textual's `Screen` concept (#111,!71)
+  - this means the TUI will look slightly different but no real functional change has occurred
+  - the view of an `Entry` can now be scrolled when the output exceeds the available space
+- switched from the `BeautifulSoup` HTML parser to `lxml`
+  - this is supposed to give more accurate results but adds an extra dependency
+
+### Deprecated
+- The following shell helpers are no longer used with the zsh completion being
+  removed. Thus, these methods will be removed in the future:
+  - `cobib _list_commands`
+  - `cobib _list_filters`
+  - `cobib _list_labels`
+  - If you see warnings because of this while you are using the CLI, you
+    probably still have the (now removed) zsh completion script installed. You
+    should remove the `_cobib` file which will be located in one of the
+    directories listed in your `$FPATH` environment variable.
+
+### Fixed
+- the proper pre-population of the TUI prompt during the sorting action (#117)
+- preserves the value of `config.commands.list_.default_columns` and
+  properly removes a field if it is no longer sorted by in the TUI (#117)
+- properly updates the list of entries in the TUI after changing the database contents;
+  for example via `add` (#113) or `delete` (#113) or `edit` (#118)
+- an issue where file-accessing operations performed on a newly added entry within
+  the same TUI session would fail because the path would not be iterated correctly
+- the live updating of the download progress bar inside the TUI (#112)
+
+### Removed
+- the crude and very slow zsh completion script
+
+
 ## [4.0.0] - 2023-05-20
 
-Pypi: https://pypi.org/project/cobib/3.5.5/
+Pypi: https://pypi.org/project/cobib/4.0.0/
 
 ### **Breaking Changes**
 - Configuration settings can no longer be set by item access and instead must
   use attribute syntax. For example you need to change:
   ```python
   config["database"]["git"] = True
   ```
@@ -992,15 +1049,16 @@
 
 ## [0.1] - 2019-04-29
 
 ### Added
 - initial version with a basic `sqlite3`-based database
 
 
-[Unreleased]: https://gitlab.com/cobib/cobib/-/compare/v4.0.0...master
+[Unreleased]: https://gitlab.com/cobib/cobib/-/compare/v4.1.0...master
+[4.1.0]: https://gitlab.com/cobib/cobib/-/compare/v4.1.0
 [4.0.0]: https://gitlab.com/cobib/cobib/-/compare/v4.0.0
 [3.5.5]: https://gitlab.com/cobib/cobib/-/compare/v3.5.5
 [3.5.4]: https://gitlab.com/cobib/cobib/-/compare/v3.5.4
 [3.5.3]: https://gitlab.com/cobib/cobib/-/compare/v3.5.3
 [3.5.2]: https://gitlab.com/cobib/cobib/-/compare/v3.5.2
 [3.5.1]: https://gitlab.com/cobib/cobib/-/compare/v3.5.1
 [3.5.0]: https://gitlab.com/cobib/cobib/-/compare/v3.5.0
```

### Comparing `cobib-4.0.0/src/cobib.egg-info/SOURCES.txt` & `cobib-4.1.0/src/cobib.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 .pylintrc
 CHANGELOG.md
 CONTRIBUTING.md
 LICENSE.txt
 MANIFEST.in
 Makefile
 README.md
-_cobib
 cobib.1
 mypy.ini
 pyproject.toml
 pytest.ini
 requirements.txt
 setup.cfg
 setup.py
@@ -76,22 +75,25 @@
 src/cobib/ui/cli.py
 src/cobib/ui/shell_helper.py
 src/cobib/ui/tui.py
 src/cobib/ui/ui.py
 src/cobib/ui/components/__init__.py
 src/cobib/ui/components/argument_parser.py
 src/cobib/ui/components/entry_view.py
-src/cobib/ui/components/help_popup.py
-src/cobib/ui/components/input.py
-src/cobib/ui/components/main_view.py
+src/cobib/ui/components/help_screen.py
+src/cobib/ui/components/input_screen.py
+src/cobib/ui/components/list_view.py
+src/cobib/ui/components/main_content.py
+src/cobib/ui/components/motion_key.py
 src/cobib/ui/components/popup.py
 src/cobib/ui/components/popup_logging_handler.py
 src/cobib/ui/components/popup_panel.py
 src/cobib/ui/components/progress.py
 src/cobib/ui/components/prompt.py
+src/cobib/ui/components/search_view.py
 src/cobib/ui/components/selection_filter.py
 src/cobib/utils/__init__.py
 src/cobib/utils/diff_renderer.py
 src/cobib/utils/file_downloader.py
 src/cobib/utils/journal_abbreviations.py
 src/cobib/utils/logging.py
 src/cobib/utils/rel_path.py
```

### Comparing `cobib-4.0.0/tests/__init__.py` & `cobib-4.1.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/tests/cmdline_test.py` & `cobib-4.1.0/tests/cmdline_test.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/tests/commands/command_test.py` & `cobib-4.1.0/tests/commands/command_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,15 @@
             The internally used parameters for potential later re-use during the actual test.
         """
         if not hasattr(request, "param"):
             # use default settings
             request.param = {"git": False, "database": True}
 
         # use temporary config
+        config.commands.delete.confirm = False
         config.commands.edit.editor = "cat"
         config.commands.open.command = "cat"
         config.database.file = str(self.COBIB_TEST_DIR / "database.yaml")
         config.database.git = request.param.get("git", False)
         config.utils.file_downloader.default_location = "/tmp"
         config.logging.version = None
```

### Comparing `cobib-4.0.0/tests/commands/test_add.py` & `cobib-4.1.0/tests/commands/test_add.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,39 +166,53 @@
             assert dummy_start > 0
             assert lines[dummy_start - 1] == "---\n"
             assert lines[dummy_start + 1] == "  ENTRYTYPE: article\n"
             assert lines[dummy_start + 2] == "...\n"
 
     @pytest.mark.asyncio
     @pytest.mark.parametrize("folder", [None, "."])
+    @pytest.mark.parametrize("skip_download", [None, True, False])
+    @pytest.mark.parametrize("config_overwrite", [True, False])
     async def test_add_with_download(
         self,
-        folder: Optional[str],
         setup: Any,
+        folder: Optional[str],
+        skip_download: Optional[bool],
+        config_overwrite: bool,
         capsys: pytest.CaptureFixture[str],
         caplog: pytest.LogCaptureFixture,
     ) -> None:
-        """Test adding a new entry with an associated file automatically downloaded.
+        """Test adding a new entry with possibly an associated file automatically downloaded.
 
         Args:
-            folder: the folder for the downloaded file.
             setup: the `tests.commands.command_test.CommandTest.setup` fixture.
+            folder: the folder for the downloaded file.
+            skip_download: argument to `AddCommand`.
+            config_overwrite: what to overwrite `config.commands.add.skip_download` with.
             capsys: the built-in pytest fixture.
             caplog: the built-in pytest fixture.
         """
+        config.commands.add.skip_download = config_overwrite
+
+        should_download = not config_overwrite
+        if skip_download is not None:
+            should_download = not skip_download
+
         path = RelPath(f"{'/tmp' if folder is None else folder}/Cao2018.pdf")
         try:
             # ensure file does not exist yet
             os.remove(path.path)
         except FileNotFoundError:
             pass
         try:
             args = ["-a", "1812.09976"]
             if folder:
                 args += ["-p", folder]
+            if skip_download is not None:
+                args.append(f"--{'skip' if skip_download else 'force'}-download")
 
             await AddCommand(*args).execute()
 
             if (
                 "cobib.parsers.arxiv",
                 logging.ERROR,
                 "An Exception occurred while trying to query the arXiv ID: 1812.09976.",
@@ -206,49 +220,20 @@
                 pytest.skip("The requests API encountered an error. Skipping test.")
 
             entry = Database()["Cao2018"]
             assert entry.label == "Cao2018"
             assert entry.data["archivePrefix"] == "arXiv"
             assert entry.data["arxivid"].startswith("1812.09976")
             assert "_download" not in entry.data.keys()
-            assert f"Successfully downloaded {path}" in capsys.readouterr().out
-            assert os.path.exists(path.path)
-        finally:
-            try:
-                os.remove(path.path)
-            except FileNotFoundError:
-                pass
-
-    @pytest.mark.asyncio
-    async def test_add_skip_download(self, setup: Any, caplog: pytest.LogCaptureFixture) -> None:
-        """Test adding a new entry and skipping the automatic download.
 
-        Args:
-            setup: the `tests.commands.command_test.CommandTest.setup` fixture.
-            caplog: the built-in pytest fixture.
-        """
-        path = RelPath("/tmp/Cao2018.pdf")
-        try:
-            args = ["-a", "1812.09976", "--skip-download"]
-
-            await AddCommand(*args).execute()
-
-            if (
-                "cobib.parsers.arxiv",
-                logging.ERROR,
-                "An Exception occurred while trying to query the arXiv ID: 1812.09976.",
-            ) in caplog.record_tuples:
-                pytest.skip("The requests API encountered an error. Skipping test.")
-
-            entry = Database()["Cao2018"]
-            assert entry.label == "Cao2018"
-            assert entry.data["archivePrefix"] == "arXiv"
-            assert entry.data["arxivid"].startswith("1812.09976")
-            assert "_download" not in entry.data.keys()
-            assert not os.path.exists(path.path)
+            if should_download:
+                assert f"Successfully downloaded {path}" in capsys.readouterr().out
+                assert os.path.exists(path.path)
+            else:
+                assert not os.path.exists(path.path)
         finally:
             try:
                 os.remove(path.path)
             except FileNotFoundError:
                 pass
 
     @pytest.mark.asyncio
```

### Comparing `cobib-4.0.0/tests/commands/test_edit.py` & `cobib-4.1.0/tests/commands/test_edit.py`

 * *Files 14% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
         assert true_log[0:4] == expected_log
         self._assert(changes=changes, logs=true_log)
 
         if git and changes:
             # assert the git commit message
             self.assert_git_commit_message(
-                "edit", {"label": args[-1], "add": "-a" in args, "preserve_files": False}
+                "edit", {"label": args[-1], "add": "-a" in args, "preserve_files": None}
             )
 
     def test_ignore_add_if_label_exists(self, setup: Any, caplog: pytest.LogCaptureFixture) -> None:
         """Test that the `add` argument is ignored if the label already exists.
 
         Args:
             setup: the `tests.commands.command_test.CommandTest.setup` fixture.
@@ -120,41 +120,52 @@
         EditCommand("-a", "einstein").execute()
         assert (
             "cobib.commands.edit",
             30,
             "Entry 'einstein' already exists! Ignoring the `--add` argument.",
         ) in caplog.record_tuples
 
-    @pytest.mark.parametrize("preserve_files", [True, False])
-    def test_rename_associated_file(self, setup: Any, preserve_files: bool) -> None:
+    @pytest.mark.parametrize("preserve_files", [None, True, False])
+    @pytest.mark.parametrize("config_overwrite", [True, False])
+    def test_rename_associated_file(
+        self, setup: Any, preserve_files: bool, config_overwrite: bool
+    ) -> None:
         """Test removing associated files.
 
         Args:
             setup: the `tests.commands.command_test.CommandTest.setup` fixture.
-            preserve_files: argument to `DeleteCommand`.
+            preserve_files: argument to `EditCommand`.
+            config_overwrite: what to overwrite `config.commands.edit.preserve_files` with.
         """
+        config.commands.edit.preserve_files = config_overwrite
+
+        should_preserve = config_overwrite
+        if preserve_files is not None:
+            should_preserve = preserve_files
+
         try:
             config.commands.edit.editor = "sed -i 's/einstein:/dummy:/'"
 
             with tempfile.TemporaryDirectory() as tmpdirname:
                 path = RelPath(tmpdirname + "/einstein.pdf")
                 open(  # pylint: disable=consider-using-with
                     path.path, "w", encoding="utf-8"
                 ).close()
 
                 Database()["einstein"].file = str(path)
 
                 args = ["einstein"]
-                if preserve_files:
-                    args.insert(2, "--preserve-files")
+                if preserve_files is not None:
+                    args.insert(2, f"--{'' if preserve_files else 'no-'}preserve-files")
                 EditCommand(*args).execute()
                 assert "dummy" in Database().keys()
 
                 target = RelPath(tmpdirname + "/dummy.pdf")
-                if preserve_files:
+
+                if should_preserve:
                     assert path.path.exists()
                 else:
                     assert target.path.exists()
         finally:
             config.defaults()
 
     def test_warning_missing_label(self, setup: Any, caplog: pytest.LogCaptureFixture) -> None:
```

### Comparing `cobib-4.0.0/tests/commands/test_export.py` & `cobib-4.1.0/tests/commands/test_export.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/tests/commands/test_git_commit_event.py` & `cobib-4.1.0/tests/commands/test_git_commit_event.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import argparse
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Dict, Optional, Type
 
 import pytest
 from rich.console import Console
-from rich.prompt import PromptBase
+from rich.prompt import PromptBase, PromptType
 from textual.app import App
 from typing_extensions import override
 
 from cobib.commands.base_command import Command
 from cobib.config import Event, config
 from cobib.utils.rel_path import RelPath
 
@@ -29,15 +29,15 @@
     name = "dummy"
 
     @override
     def __init__(
         self,
         *args: str,
         console: Console | App[None] | None = None,
-        prompt: Type[PromptBase[str]] | None = None,
+        prompt: Type[PromptBase[PromptType]] | None = None,
     ) -> None:
         # pylint: disable=super-init-not-called
         self.largs = argparse.Namespace()
 
     @override
     @classmethod
     def init_argparser(cls) -> None:
```

### Comparing `cobib-4.0.0/tests/commands/test_import.py` & `cobib-4.1.0/tests/commands/test_import.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/tests/commands/test_init.py` & `cobib-4.1.0/tests/commands/test_init.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/tests/commands/test_list.py` & `cobib-4.1.0/tests/commands/test_list.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Tests for coBib's ListCommand."""
 # pylint: disable=unused-argument
 
 from __future__ import annotations
 
 import contextlib
 import os
+from copy import copy
 from io import StringIO
 from itertools import zip_longest
 from shutil import copyfile
 from typing import TYPE_CHECKING, Any, List, Set, Type
 
 import pytest
 from rich.table import Table
@@ -29,65 +30,88 @@
     """Tests for coBib's ListCommand."""
 
     @override
     def get_command(self) -> Type[cobib.commands.base_command.Command]:
         return ListCommand
 
     @pytest.mark.parametrize(
-        ["args", "expected_labels"],
+        ["args", "expected_labels", "config_overwrite"],
         [
-            [[], ["einstein", "latexcompanion", "knuthwebsite"]],
-            [["-r"], ["knuthwebsite", "latexcompanion", "einstein"]],
-            [["-s", "year"], ["knuthwebsite", "einstein", "latexcompanion"]],
-            [["-r", "-s", "year"], ["latexcompanion", "einstein", "knuthwebsite"]],
-            [["++author", "Einstein"], ["einstein"]],
-            [["++author", "einstein", "--ignore-case"], ["einstein"]],
-            [["--author", "Einstein"], ["latexcompanion", "knuthwebsite"]],
-            [["++author", "Einstein", "++author", "Knuth"], []],
-            [["-x", "++author", "Einstein", "++author", "Knuth"], ["einstein", "knuthwebsite"]],
+            [[], ["einstein", "latexcompanion", "knuthwebsite"], False],
+            [["-r"], ["knuthwebsite", "latexcompanion", "einstein"], False],
+            [["-s", "year"], ["knuthwebsite", "einstein", "latexcompanion"], False],
+            [["-r", "-s", "year"], ["latexcompanion", "einstein", "knuthwebsite"], False],
+            [["++author", "Einstein"], ["einstein"], False],
+            [["++author", "einstein", "-i"], ["einstein"], False],
+            [["++author", "einstein", "-I"], [], True],
+            [["--author", "Einstein"], ["latexcompanion", "knuthwebsite"], False],
+            [["++author", "Einstein", "++author", "Knuth"], [], False],
+            [
+                ["-x", "++author", "Einstein", "++author", "Knuth"],
+                ["einstein", "knuthwebsite"],
+                False,
+            ],
         ],
     )
-    def test_command(self, setup: Any, args: List[str], expected_labels: List[str]) -> None:
+    def test_command(
+        self, setup: Any, args: List[str], expected_labels: List[str], config_overwrite: bool
+    ) -> None:
         """Test the command itself.
 
         Args:
             setup: the `tests.commands.command_test.CommandTest.setup` fixture.
             args: the arguments to pass to the command.
             expected_labels: the expected list of labels.
+            config_overwrite: what to overwrite `config.commands.list_.ignore_case` with.
         """
+        config.commands.list_.ignore_case = config_overwrite
+        original_default_columns = copy(config.commands.list_.default_columns)
+
         cmd = ListCommand(*args)
         cmd.execute()
         assert [entry.label for entry in cmd.entries] == expected_labels
+        # NOTE: this is a regression test against https://gitlab.com/cobib/cobib/-/issues/117
+        assert original_default_columns == config.commands.list_.default_columns
 
     @pytest.mark.parametrize(
-        ["args", "expected_labels", "expected_keys"],
+        ["args", "expected_labels", "expected_keys", "config_overwrite"],
         [
-            [[], ["einstein", "latexcompanion", "knuthwebsite"], set()],
-            [["++author", "Einstein"], ["einstein"], {"author"}],
-            [["++author", "einstein", "--ignore-case"], ["einstein"], {"author"}],
-            [["--author", "Einstein"], ["latexcompanion", "knuthwebsite"], {"author"}],
-            [["++author", "Einstein", "++author", "Knuth"], [], {"author"}],
+            [[], ["einstein", "latexcompanion", "knuthwebsite"], set(), False],
+            [["++author", "Einstein"], ["einstein"], {"author"}, False],
+            [["++author", "einstein", "-i"], ["einstein"], {"author"}, False],
+            [["++author", "einstein", "-I"], [], {"author"}, True],
+            [["--author", "Einstein"], ["latexcompanion", "knuthwebsite"], {"author"}, False],
+            [["++author", "Einstein", "++author", "Knuth"], [], {"author"}, False],
             [
                 ["-x", "++author", "Einstein", "++author", "Knuth"],
                 ["einstein", "knuthwebsite"],
                 {"author"},
+                False,
             ],
         ],
     )
     def test_filter_entries(
-        self, setup: Any, args: List[str], expected_labels: List[str], expected_keys: Set[str]
+        self,
+        setup: Any,
+        args: List[str],
+        expected_labels: List[str],
+        expected_keys: Set[str],
+        config_overwrite: bool,
     ) -> None:
         """Tests the filtering methods.
 
         Args:
             setup: the `tests.commands.command_test.CommandTest.setup` fixture.
             args: the arguments to pass to the command.
             expected_labels: the expected list of labels which match the filter.
             expected_keys: the expected keys which were filtered on.
+            config_overwrite: what to overwrite `config.commands.list_.ignore_case` with.
         """
+        config.commands.list_.ignore_case = config_overwrite
+
         filtered_entries, filtered_keys = ListCommand(*args).filter_entries()
         assert filtered_keys == expected_keys
         assert [entry.label for entry in filtered_entries] == expected_labels
 
     def test_missing_keys(self, setup: Any) -> None:
         """Asserts issue #1 is fixed.
```

### Comparing `cobib-4.0.0/tests/commands/test_modify.py` & `cobib-4.1.0/tests/commands/test_modify.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from io import StringIO
 from typing import TYPE_CHECKING, Any, List, Type
 
 import pytest
 from typing_extensions import override
 
 from cobib.commands import ModifyCommand
-from cobib.config import Event
+from cobib.config import Event, config
 from cobib.database import Database
 from cobib.utils.rel_path import RelPath
 
 from .command_test import CommandTest
 
 if TYPE_CHECKING:
     import cobib.commands
@@ -98,15 +98,15 @@
                 # assert the git commit message
                 self.assert_git_commit_message(
                     "modify",
                     {
                         "modification": modification.split(":"),
                         "dry": False,
                         "add": add,
-                        "preserve_files": False,
+                        "preserve_files": None,
                         "selection": selection,
                         "filter": filters,
                     },
                 )
             except AssertionError:
                 assert dry
 
@@ -165,36 +165,46 @@
         if field != "label":
             assert Database()["einstein"].data[field] == expected
         else:
             assert "eistein" not in Database().keys()
             assert expected in Database().keys()
             assert Database()[expected].label == expected
 
-    @pytest.mark.parametrize("preserve_files", [True, False])
-    def test_rename_associated_file(self, setup: Any, preserve_files: bool) -> None:
+    @pytest.mark.parametrize("preserve_files", [None, True, False])
+    @pytest.mark.parametrize("config_overwrite", [True, False])
+    def test_rename_associated_file(
+        self, setup: Any, preserve_files: bool, config_overwrite: bool
+    ) -> None:
         """Test removing associated files.
 
         Args:
             setup: the `tests.commands.command_test.CommandTest.setup` fixture.
-            preserve_files: argument to `DeleteCommand`.
+            preserve_files: argument to `ModifyCommand`.
+            config_overwrite: what to overwrite `config.commands.modify.preserve_files` with.
         """
+        config.commands.modify.preserve_files = config_overwrite
+
+        should_preserve = config_overwrite
+        if preserve_files is not None:
+            should_preserve = preserve_files
+
         with tempfile.TemporaryDirectory() as tmpdirname:
             path = RelPath(tmpdirname + "/knuthwebsite.pdf")
             open(path.path, "w", encoding="utf-8").close()  # pylint: disable=consider-using-with
 
             Database()["knuthwebsite"].file = str(path)
 
             args = ["label:dummy", "-s", "--", "knuthwebsite"]
-            if preserve_files:
-                args.insert(2, "--preserve-files")
+            if preserve_files is not None:
+                args.insert(2, f"--{'' if preserve_files else 'no-'}preserve-files")
             ModifyCommand(*args).execute()
             assert "dummy" in Database().keys()
 
             target = RelPath(tmpdirname + "/dummy.pdf")
-            if preserve_files:
+            if should_preserve:
                 assert path.path.exists()
             else:
                 assert target.path.exists()
 
     def test_warning_missing_label(self, setup: Any, caplog: pytest.LogCaptureFixture) -> None:
         """Test warning for missing label.
```

### Comparing `cobib-4.0.0/tests/commands/test_open.py` & `cobib-4.1.0/tests/commands/test_open.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/tests/commands/test_redo.py` & `cobib-4.1.0/tests/commands/test_redo.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/tests/commands/test_search.py` & `cobib-4.1.0/tests/commands/test_search.py`

 * *Files 9% similar despite different names*

```diff
@@ -112,14 +112,19 @@
                 False,
             ],
             [
                 ["einstein", "Elektro", "--", "--label", "einstein"],
                 [],
                 False,
             ],
+            [
+                ["einstein", "-I"],
+                ["einstein::1", "1::@article{einstein,", "1::author = {Albert Einstein},"],
+                True,
+            ],
         ],
     )
     def test_command(
         self, setup: Any, args: List[str], expected: List[str], config_overwrite: bool
     ) -> None:
         """Test the command itself.
 
@@ -132,14 +137,41 @@
         config.commands.search.ignore_case = config_overwrite
 
         cmd = SearchCommand(*args)
         cmd.execute()
         output = cmd.render_porcelain()
         self._assert(output, expected)
 
+    def test_context_configuration(self, setup: Any) -> None:
+        """Test the `config.commands.search.context` setting.
+
+        Args:
+            setup: the `tests.commands.command_test.CommandTest.setup` fixture.
+        """
+        config.commands.search.context = 2
+
+        cmd = SearchCommand(
+            "einstein",
+            "-i",
+            "-c",
+            "2",
+        )
+        cmd.execute()
+        output = cmd.render_porcelain()
+        self._assert(
+            output,
+            [
+                "einstein::2",
+                "1::@article{einstein,",
+                "2::author = {Albert Einstein},",
+                "2::doi = {http://dx.doi.org/10.1002/andp.19053221004},",
+                "2::journal = {Annalen der Physik},",
+            ],
+        )
+
     def test_render_rich(self, setup: Any) -> None:
         """Test the rich rendering.
 
         Args:
             setup: the `tests.commands.command_test.CommandTest.setup` fixture.
         """
         cmd = SearchCommand("einstein", "-i")
```

### Comparing `cobib-4.0.0/tests/commands/test_show.py` & `cobib-4.1.0/tests/commands/test_show.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/tests/commands/test_undo.py` & `cobib-4.1.0/tests/commands/test_undo.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/tests/config/test_config.py` & `cobib-4.1.0/tests/config/test_config.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/tests/config/test_event.py` & `cobib-4.1.0/tests/config/test_event.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/tests/database/test_database.py` & `cobib-4.1.0/tests/database/test_database.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 
     Yields:
         Access to the local fixture variables.
     """
     config.load(get_resource("debug.py"))
     yield
     Database().clear()
+    Database().read()
     config.defaults()
 
 
 def test_database_singleton() -> None:
     """Test the Database is a Singleton."""
     bib = Database()
     bib2 = Database()
```

### Comparing `cobib-4.0.0/tests/database/test_entry.py` & `cobib-4.1.0/tests/database/test_entry.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/tests/example_entry.bib` & `cobib-4.1.0/tests/example_entry.bib`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/tests/example_entry.yaml` & `cobib-4.1.0/tests/example_entry.yaml`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/tests/example_literature.bib` & `cobib-4.1.0/tests/example_literature.bib`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/tests/example_literature.yaml` & `cobib-4.1.0/tests/example_literature.yaml`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/tests/importers/test_zotero.py` & `cobib-4.1.0/tests/importers/test_zotero.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
                 imported_database.splitlines(keepends=True), expected.readlines()
             ):
                 assert line == truth
 
     @pytest.mark.asyncio
     async def test_fetch(self) -> None:
         """Test fetching entries from the Zotero API."""
-        importer = MockZoteroImporter(skip_download=False)
+        importer = MockZoteroImporter(skip_download=True)
         # NOTE: even though attachments are not accessible via public libraries, we explicitly skip
         # downloading them, just to be sure.
         imported_entries = await importer.fetch()
 
         self._assert_results(imported_entries)
 
     @pytest.mark.asyncio
```

### Comparing `cobib-4.0.0/tests/importers/zotero_database.yaml` & `cobib-4.1.0/tests/importers/zotero_database.yaml`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/tests/parsers/parser_test.py` & `cobib-4.1.0/tests/parsers/parser_test.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/tests/parsers/test_arxiv.py` & `cobib-4.1.0/tests/parsers/test_arxiv.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/tests/parsers/test_bibtex.py` & `cobib-4.1.0/tests/parsers/test_bibtex.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/tests/parsers/test_doi.py` & `cobib-4.1.0/tests/parsers/test_doi.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/tests/parsers/test_isbn.py` & `cobib-4.1.0/tests/parsers/test_isbn.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/tests/parsers/test_url.py` & `cobib-4.1.0/tests/parsers/test_url.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/tests/parsers/test_yaml.py` & `cobib-4.1.0/tests/parsers/test_yaml.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/tests/test_main.py` & `cobib-4.1.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/tests/utils/test_file_downloader.py` & `cobib-4.1.0/tests/utils/test_file_downloader.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/tests/utils/test_journal_abbreviations.py` & `cobib-4.1.0/tests/utils/test_journal_abbreviations.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/tests/utils/test_logging.py` & `cobib-4.1.0/tests/utils/test_logging.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/tests/utils/test_rel_path.py` & `cobib-4.1.0/tests/utils/test_rel_path.py`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/tests/utils/test_shell_helper.py` & `cobib-4.1.0/tests/utils/test_shell_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -286,14 +286,15 @@
 
 class TestUnifyLabels(ShellHelperTest):
     """Tests for the shell helper which unifies all database labels."""
 
     COMMAND = "unify_labels"
     REL_PATH = RelPath(get_resource("unifying_database.yaml", "utils"))
     EXPECTED: List[str] = [
+        "[INFO] Associated files will not be preserved.",
         "[INFO] einstein: changing field 'label' from einstein to Einstein1905_a",
         "[INFO] latexcompanion: changing field 'label' from latexcompanion to Goossens1993",
         "[INFO] knuthwebsite: changing field 'label' from knuthwebsite to Knuth",
         "[INFO] Einstein_1905: changing field 'label' from Einstein_1905 to Einstein1905_b",
         "[INFO] New and previous values match. Skipping modification of entry 'Einstein1905'.",
         "[INFO] einstein_2: changing field 'label' from einstein_2 to Einstein1905_c",
         "[INFO] New and previous values match. Skipping modification of entry 'Author2021'.",
```

### Comparing `cobib-4.0.0/tests/utils/unified_database.yaml` & `cobib-4.1.0/tests/utils/unified_database.yaml`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/tests/utils/unifying_database.yaml` & `cobib-4.1.0/tests/utils/unifying_database.yaml`

 * *Files identical despite different names*

### Comparing `cobib-4.0.0/tox.ini` & `cobib-4.1.0/tox.ini`

 * *Files identical despite different names*

