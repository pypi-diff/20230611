# Comparing `tmp/scicookie-0.1.0.tar.gz` & `tmp/scicookie-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scicookie-0.1.0.tar", max compression
+gzip compressed data, was "scicookie-0.1.1.tar", max compression
```

## Comparing `scicookie-0.1.0.tar` & `scicookie-0.1.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0     1551 2023-03-31 01:35:05.906450 scicookie-0.1.0/LICENSE
--rw-r--r--   0        0        0     1691 2023-06-10 03:13:10.542077 scicookie-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-09 16:16:30.770946 scicookie-0.1.0/src/scicookie/__init__.py
--rw-r--r--   0        0        0       68 2023-06-10 03:10:20.497924 scicookie-0.1.0/src/scicookie/__main__.py
--rw-r--r--   0        0        0     3058 2023-06-10 20:03:35.174723 scicookie-0.1.0/src/scicookie/cli.py
--rw-r--r--   0        0        0     1683 2023-06-10 02:42:09.747457 scicookie-0.1.0/src/scicookie/cookiecutter.json
--rw-r--r--   0        0        0     5768 2023-06-10 02:42:47.302727 scicookie-0.1.0/src/scicookie/hooks/post_gen_project.py
--rw-r--r--   0        0        0      359 2023-03-31 01:35:05.926450 scicookie-0.1.0/src/scicookie/hooks/pre_gen_project.py
--rw-r--r--   0        0        0      657 2023-06-10 03:10:19.453895 scicookie-0.1.0/src/scicookie/logs.py
--rw-r--r--   0        0        0     1207 2023-06-10 03:10:44.538589 scicookie-0.1.0/src/scicookie/profile.py
--rw-r--r--   0        0        0     3686 2023-06-10 02:40:31.065604 scicookie-0.1.0/src/scicookie/profiles/base.yaml
--rw-r--r--   0        0        0      739 2023-06-10 02:41:11.028692 scicookie-0.1.0/src/scicookie/profiles/osl.yaml
--rw-r--r--   0        0        0     1871 2023-06-10 03:10:57.546937 scicookie-0.1.0/src/scicookie/ui.py
--rw-r--r--   0        0        0       67 2023-06-08 00:09:47.410403 scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/.bandit
--rw-r--r--   0        0        0      292 2023-03-31 01:35:05.954450 scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/.editorconfig
--rw-r--r--   0        0        0     4617 2023-06-08 00:09:47.410403 scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0        0        0      892 2023-06-08 00:09:47.410403 scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1712 2023-06-08 00:09:47.410403 scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/documentation-report.yml
--rw-r--r--   0        0        0     2550 2023-06-08 00:09:47.418403 scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/feature-request.yml
--rw-r--r--   0        0        0      342 2023-03-31 01:35:05.958449 scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0     1387 2023-06-08 00:09:47.418403 scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      814 2023-05-03 14:26:42.182726 scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/main.yaml
--rw-r--r--   0        0        0     1666 2023-06-08 00:09:47.418403 scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1274 2023-03-31 01:35:05.962449 scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/.gitignore
--rw-r--r--   0        0        0     3198 2023-06-09 01:51:29.564476 scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2295 2023-06-08 00:58:27.913254 scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/.releaserc.json
--rw-r--r--   0        0        0     5996 2023-03-31 01:35:05.962449 scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/LICENSE
--rw-r--r--   0        0        0     2637 2023-06-08 16:24:02.893195 scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/Makefile
--rw-r--r--   0        0        0     3325 2023-06-10 02:40:03.810262 scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/README.md
--rw-r--r--   0        0        0     6433 2023-03-31 01:35:05.966449 scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CITIZEN.md
--rw-r--r--   0        0        0     6434 2023-03-31 01:35:05.966449 scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     5488 2023-03-31 01:35:05.966449 scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_CONVENANT.md
--rw-r--r--   0        0        0     5488 2023-03-31 01:35:05.966449 scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_COVENANT.md
--rw-r--r--   0        0        0      175 2023-06-08 00:09:47.418403 scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/conda/dev.yaml
--rw-r--r--   0        0        0     1998 2023-06-10 02:40:03.834261 scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/containers/Dockerfile
--rw-r--r--   0        0        0      300 2023-06-08 00:09:47.422403 scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/containers/compose.yaml
--rw-r--r--   0        0        0       20 2023-03-31 01:35:05.970449 scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/docs/changelog.md
--rw-r--r--   0        0        0     5666 2023-06-08 00:09:47.422403 scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/docs/contributing.md
--rw-r--r--   0        0        0     1001 2023-03-31 01:35:05.970449 scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/docs/example.ipynb
--rw-r--r--   0        0        0    72342 2023-03-31 01:35:05.974449 scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/docs/images/favicon.ico
--rw-r--r--   0        0        0    20402 2023-03-31 01:35:05.974449 scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/docs/images/logo.png
--rw-r--r--   0        0        0     3386 2023-06-10 02:40:03.830261 scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/docs/index.md
--rw-r--r--   0        0        0      996 2023-03-31 01:35:05.974449 scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/docs/installation.md
--rw-r--r--   0        0        0      967 2023-03-31 01:35:05.970449 scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/docs-jupyter-book/_config.yaml
--rw-r--r--   0        0        0      151 2023-03-31 01:35:05.970449 scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/docs-jupyter-book/_toc.yml
--rw-r--r--   0        0        0     4055 2023-03-31 01:35:05.970449 scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/docs-mkdocs/mkdocs.yaml
--rwxr-xr-x   0        0        0     5217 2023-06-08 00:09:47.422403 scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/conf.py
--rw-r--r--   0        0        0      311 2023-03-31 01:35:05.970449 scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/index.rst
--rw-r--r--   0        0        0      829 2023-03-31 01:35:05.970449 scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/make.bat
--rw-r--r--   0        0        0       26 2023-03-31 01:35:05.970449 scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/readme.rst
--rw-r--r--   0        0        0    16493 2023-06-08 00:09:47.422403 scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/governance/numpy_governance.md
--rw-r--r--   0        0        0     6843 2023-06-08 00:09:47.422403 scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/governance/sciml_governance.md
--rw-r--r--   0        0        0     3247 2023-06-10 02:40:03.766263 scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/pyproject.toml
--rw-r--r--   0        0        0     1558 2023-06-08 00:09:47.422403 scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/roadmap/ignite_roadmap.md
--rw-r--r--   0        0        0       61 2023-03-31 01:35:05.974449 scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/tests/__init__.py
--rw-r--r--   0        0        0      317 2023-03-31 01:35:05.978449 scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.project_slug}}.py
--rw-r--r--   0        0        0      796 2023-06-09 02:09:33.606669 scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__init__.py
--rw-r--r--   0        0        0      631 2023-06-09 02:09:46.798522 scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__main__.py
--rw-r--r--   0        0        0       19 2023-03-31 01:35:05.978449 scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/{{cookiecutter.package_slug}}.py
--rw-r--r--   0        0        0      644 1970-01-01 00:00:00.000000 scicookie-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1551 2023-03-31 01:35:05.906450 scicookie-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1711 2023-06-11 00:16:35.923043 scicookie-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-09 16:16:30.770946 scicookie-0.1.1/src/scicookie/__init__.py
+-rw-r--r--   0        0        0       68 2023-06-10 22:35:28.903163 scicookie-0.1.1/src/scicookie/__main__.py
+-rw-r--r--   0        0        0     3030 2023-06-10 23:23:24.579054 scicookie-0.1.1/src/scicookie/cli.py
+-rw-r--r--   0        0        0     1683 2023-06-10 02:42:09.747457 scicookie-0.1.1/src/scicookie/cookiecutter.json
+-rw-r--r--   0        0        0     5768 2023-06-10 02:42:47.302727 scicookie-0.1.1/src/scicookie/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      359 2023-03-31 01:35:05.926450 scicookie-0.1.1/src/scicookie/hooks/pre_gen_project.py
+-rw-r--r--   0        0        0      657 2023-06-10 03:10:19.453895 scicookie-0.1.1/src/scicookie/logs.py
+-rw-r--r--   0        0        0     1207 2023-06-10 03:10:44.538589 scicookie-0.1.1/src/scicookie/profile.py
+-rw-r--r--   0        0        0     3686 2023-06-10 02:40:31.065604 scicookie-0.1.1/src/scicookie/profiles/base.yaml
+-rw-r--r--   0        0        0      739 2023-06-10 02:41:11.028692 scicookie-0.1.1/src/scicookie/profiles/osl.yaml
+-rw-r--r--   0        0        0     1871 2023-06-10 03:10:57.546937 scicookie-0.1.1/src/scicookie/ui.py
+-rw-r--r--   0        0        0       67 2023-06-08 00:09:47.410403 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/.bandit
+-rw-r--r--   0        0        0      292 2023-03-31 01:35:05.954450 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/.editorconfig
+-rw-r--r--   0        0        0     4617 2023-06-08 00:09:47.410403 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0        0        0      892 2023-06-08 00:09:47.410403 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1712 2023-06-08 00:09:47.410403 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/documentation-report.yml
+-rw-r--r--   0        0        0     2550 2023-06-08 00:09:47.418403 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/feature-request.yml
+-rw-r--r--   0        0        0      342 2023-03-31 01:35:05.958449 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0     1387 2023-06-08 00:09:47.418403 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      814 2023-05-03 14:26:42.182726 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/main.yaml
+-rw-r--r--   0        0        0     1666 2023-06-08 00:09:47.418403 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1274 2023-03-31 01:35:05.962449 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/.gitignore
+-rw-r--r--   0        0        0     3198 2023-06-09 01:51:29.564476 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2295 2023-06-08 00:58:27.913254 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/.releaserc.json
+-rw-r--r--   0        0        0     5996 2023-03-31 01:35:05.962449 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/LICENSE
+-rw-r--r--   0        0        0     2637 2023-06-08 16:24:02.893195 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/Makefile
+-rw-r--r--   0        0        0     3325 2023-06-10 02:40:03.810262 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/README.md
+-rw-r--r--   0        0        0     6433 2023-03-31 01:35:05.966449 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/coc/CITIZEN.md
+-rw-r--r--   0        0        0     6434 2023-03-31 01:35:05.966449 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/coc/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     5488 2023-03-31 01:35:05.966449 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_CONVENANT.md
+-rw-r--r--   0        0        0     5488 2023-03-31 01:35:05.966449 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_COVENANT.md
+-rw-r--r--   0        0        0      175 2023-06-08 00:09:47.418403 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/conda/dev.yaml
+-rw-r--r--   0        0        0     1998 2023-06-10 02:40:03.834261 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/containers/Dockerfile
+-rw-r--r--   0        0        0      300 2023-06-08 00:09:47.422403 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/containers/compose.yaml
+-rw-r--r--   0        0        0       20 2023-03-31 01:35:05.970449 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/docs/changelog.md
+-rw-r--r--   0        0        0     5666 2023-06-08 00:09:47.422403 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/docs/contributing.md
+-rw-r--r--   0        0        0     1001 2023-03-31 01:35:05.970449 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/docs/example.ipynb
+-rw-r--r--   0        0        0    72342 2023-03-31 01:35:05.974449 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/docs/images/favicon.ico
+-rw-r--r--   0        0        0    20402 2023-03-31 01:35:05.974449 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/docs/images/logo.png
+-rw-r--r--   0        0        0     3386 2023-06-10 02:40:03.830261 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/docs/index.md
+-rw-r--r--   0        0        0      996 2023-03-31 01:35:05.974449 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/docs/installation.md
+-rw-r--r--   0        0        0      967 2023-03-31 01:35:05.970449 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/docs-jupyter-book/_config.yaml
+-rw-r--r--   0        0        0      151 2023-03-31 01:35:05.970449 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/docs-jupyter-book/_toc.yml
+-rw-r--r--   0        0        0     4055 2023-03-31 01:35:05.970449 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/docs-mkdocs/mkdocs.yaml
+-rwxr-xr-x   0        0        0     5217 2023-06-08 00:09:47.422403 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/conf.py
+-rw-r--r--   0        0        0      311 2023-03-31 01:35:05.970449 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/index.rst
+-rw-r--r--   0        0        0      829 2023-03-31 01:35:05.970449 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/make.bat
+-rw-r--r--   0        0        0       26 2023-03-31 01:35:05.970449 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/readme.rst
+-rw-r--r--   0        0        0    16493 2023-06-08 00:09:47.422403 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/governance/numpy_governance.md
+-rw-r--r--   0        0        0     6843 2023-06-08 00:09:47.422403 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/governance/sciml_governance.md
+-rw-r--r--   0        0        0     3247 2023-06-10 02:40:03.766263 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/pyproject.toml
+-rw-r--r--   0        0        0     1558 2023-06-08 00:09:47.422403 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/roadmap/ignite_roadmap.md
+-rw-r--r--   0        0        0       61 2023-03-31 01:35:05.974449 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0      317 2023-03-31 01:35:05.978449 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.project_slug}}.py
+-rw-r--r--   0        0        0      796 2023-06-09 02:09:33.606669 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__init__.py
+-rw-r--r--   0        0        0      631 2023-06-09 02:09:46.798522 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__main__.py
+-rw-r--r--   0        0        0       19 2023-03-31 01:35:05.978449 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/{{cookiecutter.package_slug}}.py
+-rw-r--r--   0        0        0      644 1970-01-01 00:00:00.000000 scicookie-0.1.1/PKG-INFO
```

### Comparing `scicookie-0.1.0/LICENSE` & `scicookie-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.0/pyproject.toml` & `scicookie-0.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scicookie"
-version = "0.1.0"
+version = "0.1.1"  # semantic-release
 description = "Cookiecutter template for a Python package"
 authors = ["Ivan Ogasawara <ivan.ogasawara@gmail.com>"]
 license = "BSD"
 include = [
     {path = "src/scicookie/cookiecutter.json"},
     {path = "src/scicookie/{{cookiecutter.project_slug}}"},
     {path = "src/scicookie/hooks"},
```

### Comparing `scicookie-0.1.0/src/scicookie/cli.py` & `scicookie-0.1.1/src/scicookie/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -63,29 +63,27 @@
             continue
 
         for choice in answer:
             choice_id = f"use_{choice.replace('-', '_')}"
             answers_profile[choice_id] = "yes"
 
     for question_id, answer in answers_profile.items():
-        cookie_args.append(f'{question_id}="{answer}"')
+        cookie_args.append(f"{question_id}={answer}")
 
     sh_extras = {
         "_in": sys.stdin,
         "_out": sys.stdout,
         "_err": sys.stderr,
         "_no_err": True,
         "_env": os.environ,
         "_bg": True,
         "_bg_exc": False,
     }
 
-    p = sh.cookieninja(
-        "--no-input", PACKAGE_PATH, *[" ".join(cookie_args)], **sh_extras
-    )
+    p = sh.cookieninja("--no-input", PACKAGE_PATH, *cookie_args, **sh_extras)
 
     try:
         p.wait()
     except sh.ErrorReturnCode as e:
         SciCookieLogs.raise_error(
             str(e), SciCookieErrorType.SH_ERROR_RETURN_CODE
         )
```

### Comparing `scicookie-0.1.0/src/scicookie/cookiecutter.json` & `scicookie-0.1.1/src/scicookie/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.0/src/scicookie/hooks/post_gen_project.py` & `scicookie-0.1.1/src/scicookie/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.0/src/scicookie/logs.py` & `scicookie-0.1.1/src/scicookie/logs.py`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.0/src/scicookie/profile.py` & `scicookie-0.1.1/src/scicookie/profile.py`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.0/src/scicookie/profiles/base.yaml` & `scicookie-0.1.1/src/scicookie/profiles/base.yaml`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.0/src/scicookie/profiles/osl.yaml` & `scicookie-0.1.1/src/scicookie/profiles/osl.yaml`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.0/src/scicookie/ui.py` & `scicookie-0.1.1/src/scicookie/ui.py`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/bug-report.yml` & `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/config.yml` & `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/documentation-report.yml` & `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/documentation-report.yml`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/feature-request.yml` & `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/.github/PULL_REQUEST_TEMPLATE.md` & `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/main.yaml` & `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/main.yaml`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/release.yaml` & `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/.gitignore` & `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/.pre-commit-config.yaml` & `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/.releaserc.json` & `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/.releaserc.json`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/LICENSE` & `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/LICENSE`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/Makefile` & `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/Makefile`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/README.md` & `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/README.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CITIZEN.md` & `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/coc/CITIZEN.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CODE_OF_CONDUCT.md` & `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/coc/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_CONVENANT.md` & `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_CONVENANT.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_COVENANT.md` & `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_COVENANT.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/containers/Dockerfile` & `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/containers/Dockerfile`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/docs/contributing.md` & `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/docs/example.ipynb` & `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/docs/example.ipynb`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/docs/images/favicon.ico` & `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/docs/images/logo.png` & `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/docs/index.md` & `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/docs/index.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/docs/installation.md` & `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/docs/installation.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/docs-jupyter-book/_config.yaml` & `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/docs-jupyter-book/_config.yaml`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/docs-mkdocs/mkdocs.yaml` & `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/docs-mkdocs/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/conf.py` & `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/conf.py`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/make.bat` & `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/make.bat`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/governance/numpy_governance.md` & `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/governance/numpy_governance.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/governance/sciml_governance.md` & `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/governance/sciml_governance.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/pyproject.toml` & `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/roadmap/ignite_roadmap.md` & `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/roadmap/ignite_roadmap.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__init__.py` & `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__init__.py`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.0/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__main__.py` & `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__main__.py`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.0/PKG-INFO` & `scicookie-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scicookie
-Version: 0.1.0
+Version: 0.1.1
 Summary: Cookiecutter template for a Python package
 License: BSD
 Author: Ivan Ogasawara
 Author-email: ivan.ogasawara@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

