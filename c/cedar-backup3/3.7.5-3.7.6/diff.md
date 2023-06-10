# Comparing `tmp/cedar_backup3-3.7.5.tar.gz` & `tmp/cedar_backup3-3.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cedar_backup3-3.7.5.tar", max compression
+gzip compressed data, was "cedar_backup3-3.7.6.tar", max compression
```

## Comparing `cedar_backup3-3.7.5.tar` & `cedar_backup3-3.7.6.tar`

### file list

```diff
@@ -1,188 +1,188 @@
--rw-r--r--   0        0        0    42395 2023-06-07 23:11:51.191817 cedar_backup3-3.7.5/Changelog
--rw-r--r--   0        0        0    17989 2023-06-07 23:11:51.191817 cedar_backup3-3.7.5/LICENSE
--rw-r--r--   0        0        0     9056 2023-06-07 23:11:51.191817 cedar_backup3-3.7.5/NOTICE
--rw-r--r--   0        0        0     2712 2023-06-07 23:11:51.191817 cedar_backup3-3.7.5/PyPI.md
--rw-r--r--   0        0        0     5611 2023-06-07 23:11:51.191817 cedar_backup3-3.7.5/README.md
--rw-r--r--   0        0        0       22 2023-06-07 23:11:51.191817 cedar_backup3-3.7.5/docs/.gitignore
--rw-r--r--   0        0        0      142 2023-06-07 23:11:51.191817 cedar_backup3-3.7.5/docs/.sphinxignore
--rw-r--r--   0        0        0     6814 2023-06-07 23:11:51.191817 cedar_backup3-3.7.5/docs/Makefile
--rw-r--r--   0        0        0      120 2023-06-07 23:11:51.191817 cedar_backup3-3.7.5/docs/README.md
--rw-r--r--   0        0        0      130 2023-06-07 23:11:51.191817 cedar_backup3-3.7.5/docs/_static/custom.css
--rw-r--r--   0        0        0     1861 2023-06-07 23:11:51.191817 cedar_backup3-3.7.5/docs/_themes/LICENSE
--rw-r--r--   0        0        0     3905 2023-06-07 23:11:51.191817 cedar_backup3-3.7.5/docs/_themes/flask_theme_support.py
--rw-r--r--   0        0        0    13036 2023-06-07 23:11:51.191817 cedar_backup3-3.7.5/docs/conf.py
--rw-r--r--   0        0        0     5799 2023-06-07 23:11:51.191817 cedar_backup3-3.7.5/docs/index.rst
--rw-r--r--   0        0        0     6709 2023-06-07 23:11:51.191817 cedar_backup3-3.7.5/docs/make.bat
--rw-r--r--   0        0        0    24291 2023-06-07 23:11:51.191817 cedar_backup3-3.7.5/docs/manual/basic.rst
--rw-r--r--   0        0        0    29210 2023-06-07 23:11:51.191817 cedar_backup3-3.7.5/docs/manual/commandline.rst
--rw-r--r--   0        0        0   108760 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/docs/manual/config.rst
--rw-r--r--   0        0        0    17277 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/docs/manual/copyright.rst
--rw-r--r--   0        0        0    11671 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/docs/manual/depends.rst
--rw-r--r--   0        0        0    43604 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/docs/manual/extensions.rst
--rw-r--r--   0        0        0     5437 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/docs/manual/extenspec.rst
--rw-r--r--   0        0        0     1658 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/docs/manual/images/note.png
--rw-r--r--   0        0        0     2331 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/docs/manual/images/tip.png
--rw-r--r--   0        0        0     1550 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/docs/manual/images/warning.png
--rw-r--r--   0        0        0      240 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/docs/manual/index.rst
--rw-r--r--   0        0        0     4895 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/docs/manual/install.rst
--rw-r--r--   0        0        0    10705 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/docs/manual/intro.rst
--rw-r--r--   0        0        0     3068 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/docs/manual/preface.rst
--rw-r--r--   0        0        0    21331 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/docs/manual/recovering.rst
--rw-r--r--   0        0        0     8372 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/docs/manual/securingssh.rst
--rw-r--r--   0        0        0     7391 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/manpages/cback3-amazons3-sync.1
--rw-r--r--   0        0        0     5942 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/manpages/cback3-span.1
--rw-r--r--   0        0        0    11987 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/manpages/cback3.1
--rw-r--r--   0        0        0     2847 2023-06-07 23:12:26.167810 cedar_backup3-3.7.5/pyproject.toml
--rw-r--r--   0        0        0     4608 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/samples/cback3.conf.sample
--rw-r--r--   0        0        0     2401 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/src/CedarBackup3/__init__.py
--rw-r--r--   0        0        0     1661 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/src/CedarBackup3/action.py
--rw-r--r--   0        0        0     2017 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/src/CedarBackup3/actions/__init__.py
--rw-r--r--   0        0        0    23235 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/src/CedarBackup3/actions/collect.py
--rw-r--r--   0        0        0     1230 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/src/CedarBackup3/actions/constants.py
--rw-r--r--   0        0        0     3109 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/src/CedarBackup3/actions/initialize.py
--rw-r--r--   0        0        0     3501 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/src/CedarBackup3/actions/purge.py
--rw-r--r--   0        0        0     6345 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/src/CedarBackup3/actions/rebuild.py
--rw-r--r--   0        0        0    12881 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/src/CedarBackup3/actions/stage.py
--rw-r--r--   0        0        0    17815 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/src/CedarBackup3/actions/store.py
--rw-r--r--   0        0        0    13494 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/src/CedarBackup3/actions/util.py
--rw-r--r--   0        0        0    12100 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/src/CedarBackup3/actions/validate.py
--rw-r--r--   0        0        0    82264 2023-06-07 23:11:51.199818 cedar_backup3-3.7.5/src/CedarBackup3/cli.py
--rw-r--r--   0        0        0   250415 2023-06-07 23:11:51.199818 cedar_backup3-3.7.5/src/CedarBackup3/config.py
--rw-r--r--   0        0        0     3459 2023-06-07 23:11:51.199818 cedar_backup3-3.7.5/src/CedarBackup3/customize.py
--rw-r--r--   0        0        0     1695 2023-06-07 23:11:51.199818 cedar_backup3-3.7.5/src/CedarBackup3/extend/__init__.py
--rw-r--r--   0        0        0    36418 2023-06-07 23:11:51.199818 cedar_backup3-3.7.5/src/CedarBackup3/extend/amazons3.py
--rw-r--r--   0        0        0    22064 2023-06-07 23:11:51.199818 cedar_backup3-3.7.5/src/CedarBackup3/extend/capacity.py
--rw-r--r--   0        0        0    21388 2023-06-07 23:11:51.199818 cedar_backup3-3.7.5/src/CedarBackup3/extend/encrypt.py
--rw-r--r--   0        0        0    59655 2023-06-07 23:11:51.199818 cedar_backup3-3.7.5/src/CedarBackup3/extend/mbox.py
--rw-r--r--   0        0        0    28214 2023-06-07 23:11:51.199818 cedar_backup3-3.7.5/src/CedarBackup3/extend/mysql.py
--rw-r--r--   0        0        0    25473 2023-06-07 23:11:51.199818 cedar_backup3-3.7.5/src/CedarBackup3/extend/postgresql.py
--rw-r--r--   0        0        0    20096 2023-06-07 23:11:51.199818 cedar_backup3-3.7.5/src/CedarBackup3/extend/split.py
--rw-r--r--   0        0        0    63173 2023-06-07 23:11:51.199818 cedar_backup3-3.7.5/src/CedarBackup3/extend/subversion.py
--rw-r--r--   0        0        0     9075 2023-06-07 23:11:51.199818 cedar_backup3-3.7.5/src/CedarBackup3/extend/sysinfo.py
--rw-r--r--   0        0        0    65886 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/src/CedarBackup3/filesystem.py
--rw-r--r--   0        0        0     1326 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/src/CedarBackup3/image.py
--rw-r--r--   0        0        0    13471 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/src/CedarBackup3/knapsack.py
--rw-r--r--   0        0        0    52142 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/src/CedarBackup3/peer.py
--rw-r--r--   0        0        0     2116 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/src/CedarBackup3/release.py
--rw-r--r--   0        0        0     1281 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/src/CedarBackup3/scripts.py
--rw-r--r--   0        0        0    16088 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/src/CedarBackup3/testutil.py
--rw-r--r--   0        0        0     1813 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/src/CedarBackup3/tools/__init__.py
--rw-r--r--   0        0        0    48194 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/src/CedarBackup3/tools/amazons3.py
--rw-r--r--   0        0        0    26111 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/src/CedarBackup3/tools/span.py
--rw-r--r--   0        0        0    75364 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/src/CedarBackup3/util.py
--rw-r--r--   0        0        0     1551 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/src/CedarBackup3/writer.py
--rw-r--r--   0        0        0     1398 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/src/CedarBackup3/writers/__init__.py
--rw-r--r--   0        0        0    55149 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/src/CedarBackup3/writers/cdwriter.py
--rw-r--r--   0        0        0    41297 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/src/CedarBackup3/writers/dvdwriter.py
--rw-r--r--   0        0        0    28675 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/src/CedarBackup3/writers/util.py
--rw-r--r--   0        0        0    27076 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/src/CedarBackup3/xmlutil.py
--rw-r--r--   0        0        0      797 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/__init__.py
--rw-r--r--   0        0        0       59 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/amazons3.conf.1
--rw-r--r--   0        0        0      340 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/amazons3.conf.2
--rw-r--r--   0        0        0      304 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/amazons3.conf.3
--rw-r--r--   0        0        0       59 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/capacity.conf.1
--rw-r--r--   0        0        0      172 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/capacity.conf.2
--rw-r--r--   0        0        0      170 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/capacity.conf.3
--rw-r--r--   0        0        0      172 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/capacity.conf.4
--rw-r--r--   0        0        0     2052 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/cback.conf.1
--rw-r--r--   0        0        0      915 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/cback.conf.10
--rw-r--r--   0        0        0      291 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/cback.conf.11
--rw-r--r--   0        0        0      753 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/cback.conf.12
--rw-r--r--   0        0        0      265 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/cback.conf.13
--rw-r--r--   0        0        0      501 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/cback.conf.14
--rw-r--r--   0        0        0     5175 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/cback.conf.15
--rw-r--r--   0        0        0      340 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/cback.conf.16
--rw-r--r--   0        0        0      396 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/cback.conf.17
--rw-r--r--   0        0        0      390 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/cback.conf.18
--rw-r--r--   0        0        0     1904 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/cback.conf.19
--rw-r--r--   0        0        0       59 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/cback.conf.2
--rw-r--r--   0        0        0     5271 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/cback.conf.20
--rw-r--r--   0        0        0     5848 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/cback.conf.21
--rw-r--r--   0        0        0      297 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/cback.conf.22
--rw-r--r--   0        0        0     1408 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/cback.conf.23
--rw-r--r--   0        0        0      166 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/cback.conf.3
--rw-r--r--   0        0        0      354 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/cback.conf.4
--rw-r--r--   0        0        0      386 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/cback.conf.5
--rw-r--r--   0        0        0     1010 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/cback.conf.6
--rw-r--r--   0        0        0      394 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/cback.conf.7
--rw-r--r--   0        0        0     2005 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/cback.conf.8
--rw-r--r--   0        0        0      350 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/cback.conf.9
--rw-r--r--   0        0        0       59 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/encrypt.conf.1
--rw-r--r--   0        0        0      188 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/encrypt.conf.2
--rw-r--r--   0        0        0      605 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/lotsoflines.py
--rw-r--r--   0        0        0       59 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/mbox.conf.1
--rw-r--r--   0        0        0      397 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/mbox.conf.2
--rw-r--r--   0        0        0      496 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/mbox.conf.3
--rw-r--r--   0        0        0     1355 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/mbox.conf.4
--rw-r--r--   0        0        0       59 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/mysql.conf.1
--rw-r--r--   0        0        0      263 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/mysql.conf.2
--rw-r--r--   0        0        0      303 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/mysql.conf.3
--rw-r--r--   0        0        0      346 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/mysql.conf.4
--rw-r--r--   0        0        0      307 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/mysql.conf.5
--rw-r--r--   0        0        0       59 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/postgresql.conf.1
--rw-r--r--   0        0        0      242 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/postgresql.conf.2
--rw-r--r--   0        0        0      282 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/postgresql.conf.3
--rw-r--r--   0        0        0      325 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/postgresql.conf.4
--rw-r--r--   0        0        0      310 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/postgresql.conf.5
--rw-r--r--   0        0        0       59 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/split.conf.1
--rw-r--r--   0        0        0      170 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/split.conf.2
--rw-r--r--   0        0        0      170 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/split.conf.3
--rw-r--r--   0        0        0      180 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/split.conf.4
--rw-r--r--   0        0        0      171 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/split.conf.5
--rw-r--r--   0        0        0       59 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/subversion.conf.1
--rw-r--r--   0        0        0      311 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/subversion.conf.2
--rw-r--r--   0        0        0      319 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/subversion.conf.3
--rw-r--r--   0        0        0      838 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/subversion.conf.4
--rw-r--r--   0        0        0      323 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/subversion.conf.5
--rw-r--r--   0        0        0      331 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/subversion.conf.6
--rw-r--r--   0        0        0     1243 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/subversion.conf.7
--rw-r--r--   0        0        0      263 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree1.ini
--rw-r--r--   0        0        0     1021 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree1.tar.gz
--rw-r--r--   0        0        0      391 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree10.tar.gz
--rw-r--r--   0        0        0      641 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree11.tar.gz
--rw-r--r--   0        0        0    75185 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree12.tar.gz
--rw-r--r--   0        0        0      422 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree13.tar.gz
--rw-r--r--   0        0        0      700 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree15.tar.gz
--rw-r--r--   0        0        0     8971 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree16.tar.gz
--rw-r--r--   0        0        0      997 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree17.tar.gz
--rw-r--r--   0        0        0      968 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree18.tar.gz
--rw-r--r--   0        0        0      939 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree19.tar.gz
--rw-r--r--   0        0        0      269 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree2.ini
--rw-r--r--   0        0        0      224 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree2.tar.gz
--rw-r--r--   0        0        0      976 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree20.tar.gz
--rw-r--r--   0        0        0     3557 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree21.tar.gz
--rw-r--r--   0        0        0     6158 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree22.tar.gz
--rw-r--r--   0        0        0      270 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree3.ini
--rw-r--r--   0        0        0      604 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree3.tar.gz
--rw-r--r--   0        0        0      275 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree4.ini
--rw-r--r--   0        0        0     9120 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree4.tar.gz
--rw-r--r--   0        0        0      282 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree5.ini
--rw-r--r--   0        0        0    13611 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree5.tar.gz
--rw-r--r--   0        0        0      274 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree6.ini
--rw-r--r--   0        0        0    28998 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree6.tar.gz
--rw-r--r--   0        0        0      178 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree7.tar.gz
--rw-r--r--   0        0        0      148 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree8.tar.gz
--rw-r--r--   0        0        0      272 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree9.ini
--rw-r--r--   0        0        0     1394 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree9.tar.gz
--rw-r--r--   0        0        0     9503 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/test_actions_util.py
--rw-r--r--   0        0        0    36813 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/test_amazons3.py
--rw-r--r--   0        0        0    33089 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/test_capacity.py
--rw-r--r--   0        0        0    80468 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/test_cdwriter.py
--rw-r--r--   0        0        0   674560 2023-06-07 23:11:51.211818 cedar_backup3-3.7.5/tests/test_cli.py
--rw-r--r--   0        0        0   542233 2023-06-07 23:11:51.211818 cedar_backup3-3.7.5/tests/test_config.py
--rw-r--r--   0        0        0     8124 2023-06-07 23:11:51.211818 cedar_backup3-3.7.5/tests/test_customize.py
--rw-r--r--   0        0        0    51496 2023-06-07 23:11:51.211818 cedar_backup3-3.7.5/tests/test_dvdwriter.py
--rw-r--r--   0        0        0    54326 2023-06-07 23:11:51.211818 cedar_backup3-3.7.5/tests/test_encrypt.py
--rw-r--r--   0        0        0  1291994 2023-06-07 23:11:51.215818 cedar_backup3-3.7.5/tests/test_filesystem.py
--rw-r--r--   0        0        0    99436 2023-06-07 23:11:51.219817 cedar_backup3-3.7.5/tests/test_knapsack.py
--rw-r--r--   0        0        0    84647 2023-06-07 23:11:51.219817 cedar_backup3-3.7.5/tests/test_mbox.py
--rw-r--r--   0        0        0    40974 2023-06-07 23:11:51.219817 cedar_backup3-3.7.5/tests/test_mysql.py
--rw-r--r--   0        0        0    68089 2023-06-07 23:11:51.219817 cedar_backup3-3.7.5/tests/test_peer.py
--rw-r--r--   0        0        0    39155 2023-06-07 23:11:51.219817 cedar_backup3-3.7.5/tests/test_postgresql.py
--rw-r--r--   0        0        0     4905 2023-06-07 23:11:51.219817 cedar_backup3-3.7.5/tests/test_span.py
--rw-r--r--   0        0        0    46613 2023-06-07 23:11:51.219817 cedar_backup3-3.7.5/tests/test_split.py
--rw-r--r--   0        0        0   108595 2023-06-07 23:11:51.219817 cedar_backup3-3.7.5/tests/test_subversion.py
--rw-r--r--   0        0        0   153535 2023-06-07 23:11:51.219817 cedar_backup3-3.7.5/tests/test_sync.py
--rw-r--r--   0        0        0   149942 2023-06-07 23:11:51.219817 cedar_backup3-3.7.5/tests/test_util.py
--rw-r--r--   0        0        0    70705 2023-06-07 23:11:51.219817 cedar_backup3-3.7.5/tests/test_writers_util.py
--rw-r--r--   0        0        0     4072 1970-01-01 00:00:00.000000 cedar_backup3-3.7.5/PKG-INFO
+-rw-r--r--   0        0        0    42491 2023-06-10 22:14:59.411084 cedar_backup3-3.7.6/Changelog
+-rw-r--r--   0        0        0    17989 2023-06-10 22:14:59.411084 cedar_backup3-3.7.6/LICENSE
+-rw-r--r--   0        0        0     9056 2023-06-10 22:14:59.411084 cedar_backup3-3.7.6/NOTICE
+-rw-r--r--   0        0        0     2712 2023-06-10 22:14:59.411084 cedar_backup3-3.7.6/PyPI.md
+-rw-r--r--   0        0        0     5611 2023-06-10 22:14:59.411084 cedar_backup3-3.7.6/README.md
+-rw-r--r--   0        0        0       22 2023-06-10 22:14:59.411084 cedar_backup3-3.7.6/docs/.gitignore
+-rw-r--r--   0        0        0      142 2023-06-10 22:14:59.411084 cedar_backup3-3.7.6/docs/.sphinxignore
+-rw-r--r--   0        0        0     6814 2023-06-10 22:14:59.411084 cedar_backup3-3.7.6/docs/Makefile
+-rw-r--r--   0        0        0      120 2023-06-10 22:14:59.411084 cedar_backup3-3.7.6/docs/README.md
+-rw-r--r--   0        0        0      130 2023-06-10 22:14:59.411084 cedar_backup3-3.7.6/docs/_static/custom.css
+-rw-r--r--   0        0        0     1861 2023-06-10 22:14:59.411084 cedar_backup3-3.7.6/docs/_themes/LICENSE
+-rw-r--r--   0        0        0     3905 2023-06-10 22:14:59.411084 cedar_backup3-3.7.6/docs/_themes/flask_theme_support.py
+-rw-r--r--   0        0        0    13036 2023-06-10 22:14:59.411084 cedar_backup3-3.7.6/docs/conf.py
+-rw-r--r--   0        0        0     5799 2023-06-10 22:14:59.411084 cedar_backup3-3.7.6/docs/index.rst
+-rw-r--r--   0        0        0     6709 2023-06-10 22:14:59.411084 cedar_backup3-3.7.6/docs/make.bat
+-rw-r--r--   0        0        0    24291 2023-06-10 22:14:59.415084 cedar_backup3-3.7.6/docs/manual/basic.rst
+-rw-r--r--   0        0        0    29210 2023-06-10 22:14:59.415084 cedar_backup3-3.7.6/docs/manual/commandline.rst
+-rw-r--r--   0        0        0   108760 2023-06-10 22:14:59.415084 cedar_backup3-3.7.6/docs/manual/config.rst
+-rw-r--r--   0        0        0    17277 2023-06-10 22:14:59.415084 cedar_backup3-3.7.6/docs/manual/copyright.rst
+-rw-r--r--   0        0        0    11671 2023-06-10 22:14:59.415084 cedar_backup3-3.7.6/docs/manual/depends.rst
+-rw-r--r--   0        0        0    43604 2023-06-10 22:14:59.415084 cedar_backup3-3.7.6/docs/manual/extensions.rst
+-rw-r--r--   0        0        0     5437 2023-06-10 22:14:59.415084 cedar_backup3-3.7.6/docs/manual/extenspec.rst
+-rw-r--r--   0        0        0     1658 2023-06-10 22:14:59.415084 cedar_backup3-3.7.6/docs/manual/images/note.png
+-rw-r--r--   0        0        0     2331 2023-06-10 22:14:59.415084 cedar_backup3-3.7.6/docs/manual/images/tip.png
+-rw-r--r--   0        0        0     1550 2023-06-10 22:14:59.415084 cedar_backup3-3.7.6/docs/manual/images/warning.png
+-rw-r--r--   0        0        0      240 2023-06-10 22:14:59.415084 cedar_backup3-3.7.6/docs/manual/index.rst
+-rw-r--r--   0        0        0     4895 2023-06-10 22:14:59.415084 cedar_backup3-3.7.6/docs/manual/install.rst
+-rw-r--r--   0        0        0    10705 2023-06-10 22:14:59.415084 cedar_backup3-3.7.6/docs/manual/intro.rst
+-rw-r--r--   0        0        0     3068 2023-06-10 22:14:59.415084 cedar_backup3-3.7.6/docs/manual/preface.rst
+-rw-r--r--   0        0        0    21331 2023-06-10 22:14:59.415084 cedar_backup3-3.7.6/docs/manual/recovering.rst
+-rw-r--r--   0        0        0     8372 2023-06-10 22:14:59.415084 cedar_backup3-3.7.6/docs/manual/securingssh.rst
+-rw-r--r--   0        0        0     7391 2023-06-10 22:14:59.415084 cedar_backup3-3.7.6/manpages/cback3-amazons3-sync.1
+-rw-r--r--   0        0        0     5942 2023-06-10 22:14:59.415084 cedar_backup3-3.7.6/manpages/cback3-span.1
+-rw-r--r--   0        0        0    11987 2023-06-10 22:14:59.415084 cedar_backup3-3.7.6/manpages/cback3.1
+-rw-r--r--   0        0        0     2937 2023-06-10 22:15:37.081955 cedar_backup3-3.7.6/pyproject.toml
+-rw-r--r--   0        0        0     4608 2023-06-10 22:14:59.415084 cedar_backup3-3.7.6/samples/cback3.conf.sample
+-rw-r--r--   0        0        0     2401 2023-06-10 22:14:59.415084 cedar_backup3-3.7.6/src/CedarBackup3/__init__.py
+-rw-r--r--   0        0        0     1661 2023-06-10 22:14:59.415084 cedar_backup3-3.7.6/src/CedarBackup3/action.py
+-rw-r--r--   0        0        0     2017 2023-06-10 22:14:59.419085 cedar_backup3-3.7.6/src/CedarBackup3/actions/__init__.py
+-rw-r--r--   0        0        0    23235 2023-06-10 22:14:59.419085 cedar_backup3-3.7.6/src/CedarBackup3/actions/collect.py
+-rw-r--r--   0        0        0     1230 2023-06-10 22:14:59.419085 cedar_backup3-3.7.6/src/CedarBackup3/actions/constants.py
+-rw-r--r--   0        0        0     3109 2023-06-10 22:14:59.419085 cedar_backup3-3.7.6/src/CedarBackup3/actions/initialize.py
+-rw-r--r--   0        0        0     3501 2023-06-10 22:14:59.419085 cedar_backup3-3.7.6/src/CedarBackup3/actions/purge.py
+-rw-r--r--   0        0        0     6345 2023-06-10 22:14:59.419085 cedar_backup3-3.7.6/src/CedarBackup3/actions/rebuild.py
+-rw-r--r--   0        0        0    12881 2023-06-10 22:14:59.419085 cedar_backup3-3.7.6/src/CedarBackup3/actions/stage.py
+-rw-r--r--   0        0        0    17815 2023-06-10 22:14:59.419085 cedar_backup3-3.7.6/src/CedarBackup3/actions/store.py
+-rw-r--r--   0        0        0    13494 2023-06-10 22:14:59.419085 cedar_backup3-3.7.6/src/CedarBackup3/actions/util.py
+-rw-r--r--   0        0        0    12100 2023-06-10 22:14:59.419085 cedar_backup3-3.7.6/src/CedarBackup3/actions/validate.py
+-rw-r--r--   0        0        0    82264 2023-06-10 22:14:59.419085 cedar_backup3-3.7.6/src/CedarBackup3/cli.py
+-rw-r--r--   0        0        0   250415 2023-06-10 22:14:59.419085 cedar_backup3-3.7.6/src/CedarBackup3/config.py
+-rw-r--r--   0        0        0     3459 2023-06-10 22:14:59.419085 cedar_backup3-3.7.6/src/CedarBackup3/customize.py
+-rw-r--r--   0        0        0     1695 2023-06-10 22:14:59.419085 cedar_backup3-3.7.6/src/CedarBackup3/extend/__init__.py
+-rw-r--r--   0        0        0    36418 2023-06-10 22:14:59.423085 cedar_backup3-3.7.6/src/CedarBackup3/extend/amazons3.py
+-rw-r--r--   0        0        0    22064 2023-06-10 22:14:59.423085 cedar_backup3-3.7.6/src/CedarBackup3/extend/capacity.py
+-rw-r--r--   0        0        0    21388 2023-06-10 22:14:59.423085 cedar_backup3-3.7.6/src/CedarBackup3/extend/encrypt.py
+-rw-r--r--   0        0        0    59655 2023-06-10 22:14:59.423085 cedar_backup3-3.7.6/src/CedarBackup3/extend/mbox.py
+-rw-r--r--   0        0        0    28214 2023-06-10 22:14:59.423085 cedar_backup3-3.7.6/src/CedarBackup3/extend/mysql.py
+-rw-r--r--   0        0        0    25473 2023-06-10 22:14:59.423085 cedar_backup3-3.7.6/src/CedarBackup3/extend/postgresql.py
+-rw-r--r--   0        0        0    20096 2023-06-10 22:14:59.423085 cedar_backup3-3.7.6/src/CedarBackup3/extend/split.py
+-rw-r--r--   0        0        0    63173 2023-06-10 22:14:59.423085 cedar_backup3-3.7.6/src/CedarBackup3/extend/subversion.py
+-rw-r--r--   0        0        0     9075 2023-06-10 22:14:59.423085 cedar_backup3-3.7.6/src/CedarBackup3/extend/sysinfo.py
+-rw-r--r--   0        0        0    65886 2023-06-10 22:14:59.423085 cedar_backup3-3.7.6/src/CedarBackup3/filesystem.py
+-rw-r--r--   0        0        0     1326 2023-06-10 22:14:59.423085 cedar_backup3-3.7.6/src/CedarBackup3/image.py
+-rw-r--r--   0        0        0    13471 2023-06-10 22:14:59.423085 cedar_backup3-3.7.6/src/CedarBackup3/knapsack.py
+-rw-r--r--   0        0        0    52142 2023-06-10 22:14:59.423085 cedar_backup3-3.7.6/src/CedarBackup3/peer.py
+-rw-r--r--   0        0        0     2116 2023-06-10 22:14:59.423085 cedar_backup3-3.7.6/src/CedarBackup3/release.py
+-rw-r--r--   0        0        0     1281 2023-06-10 22:14:59.423085 cedar_backup3-3.7.6/src/CedarBackup3/scripts.py
+-rw-r--r--   0        0        0    16088 2023-06-10 22:14:59.423085 cedar_backup3-3.7.6/src/CedarBackup3/testutil.py
+-rw-r--r--   0        0        0     1813 2023-06-10 22:14:59.423085 cedar_backup3-3.7.6/src/CedarBackup3/tools/__init__.py
+-rw-r--r--   0        0        0    48194 2023-06-10 22:14:59.423085 cedar_backup3-3.7.6/src/CedarBackup3/tools/amazons3.py
+-rw-r--r--   0        0        0    26111 2023-06-10 22:14:59.423085 cedar_backup3-3.7.6/src/CedarBackup3/tools/span.py
+-rw-r--r--   0        0        0    75364 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/src/CedarBackup3/util.py
+-rw-r--r--   0        0        0     1551 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/src/CedarBackup3/writer.py
+-rw-r--r--   0        0        0     1398 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/src/CedarBackup3/writers/__init__.py
+-rw-r--r--   0        0        0    55149 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/src/CedarBackup3/writers/cdwriter.py
+-rw-r--r--   0        0        0    41297 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/src/CedarBackup3/writers/dvdwriter.py
+-rw-r--r--   0        0        0    28675 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/src/CedarBackup3/writers/util.py
+-rw-r--r--   0        0        0    27076 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/src/CedarBackup3/xmlutil.py
+-rw-r--r--   0        0        0      797 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/__init__.py
+-rw-r--r--   0        0        0       59 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/amazons3.conf.1
+-rw-r--r--   0        0        0      340 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/amazons3.conf.2
+-rw-r--r--   0        0        0      304 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/amazons3.conf.3
+-rw-r--r--   0        0        0       59 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/capacity.conf.1
+-rw-r--r--   0        0        0      172 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/capacity.conf.2
+-rw-r--r--   0        0        0      170 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/capacity.conf.3
+-rw-r--r--   0        0        0      172 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/capacity.conf.4
+-rw-r--r--   0        0        0     2052 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/cback.conf.1
+-rw-r--r--   0        0        0      915 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/cback.conf.10
+-rw-r--r--   0        0        0      291 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/cback.conf.11
+-rw-r--r--   0        0        0      753 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/cback.conf.12
+-rw-r--r--   0        0        0      265 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/cback.conf.13
+-rw-r--r--   0        0        0      501 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/cback.conf.14
+-rw-r--r--   0        0        0     5175 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/cback.conf.15
+-rw-r--r--   0        0        0      340 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/cback.conf.16
+-rw-r--r--   0        0        0      396 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/cback.conf.17
+-rw-r--r--   0        0        0      390 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/cback.conf.18
+-rw-r--r--   0        0        0     1904 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/cback.conf.19
+-rw-r--r--   0        0        0       59 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/cback.conf.2
+-rw-r--r--   0        0        0     5271 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/cback.conf.20
+-rw-r--r--   0        0        0     5848 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/cback.conf.21
+-rw-r--r--   0        0        0      297 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/cback.conf.22
+-rw-r--r--   0        0        0     1408 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/cback.conf.23
+-rw-r--r--   0        0        0      166 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/cback.conf.3
+-rw-r--r--   0        0        0      354 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/cback.conf.4
+-rw-r--r--   0        0        0      386 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/cback.conf.5
+-rw-r--r--   0        0        0     1010 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/cback.conf.6
+-rw-r--r--   0        0        0      394 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/cback.conf.7
+-rw-r--r--   0        0        0     2005 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/cback.conf.8
+-rw-r--r--   0        0        0      350 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/cback.conf.9
+-rw-r--r--   0        0        0       59 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/encrypt.conf.1
+-rw-r--r--   0        0        0      188 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/encrypt.conf.2
+-rw-r--r--   0        0        0      605 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/lotsoflines.py
+-rw-r--r--   0        0        0       59 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/mbox.conf.1
+-rw-r--r--   0        0        0      397 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/mbox.conf.2
+-rw-r--r--   0        0        0      496 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/mbox.conf.3
+-rw-r--r--   0        0        0     1355 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/mbox.conf.4
+-rw-r--r--   0        0        0       59 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/mysql.conf.1
+-rw-r--r--   0        0        0      263 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/mysql.conf.2
+-rw-r--r--   0        0        0      303 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/mysql.conf.3
+-rw-r--r--   0        0        0      346 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/mysql.conf.4
+-rw-r--r--   0        0        0      307 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/mysql.conf.5
+-rw-r--r--   0        0        0       59 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/postgresql.conf.1
+-rw-r--r--   0        0        0      242 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/postgresql.conf.2
+-rw-r--r--   0        0        0      282 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/postgresql.conf.3
+-rw-r--r--   0        0        0      325 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/postgresql.conf.4
+-rw-r--r--   0        0        0      310 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/postgresql.conf.5
+-rw-r--r--   0        0        0       59 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/split.conf.1
+-rw-r--r--   0        0        0      170 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/split.conf.2
+-rw-r--r--   0        0        0      170 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/split.conf.3
+-rw-r--r--   0        0        0      180 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/split.conf.4
+-rw-r--r--   0        0        0      171 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/split.conf.5
+-rw-r--r--   0        0        0       59 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/subversion.conf.1
+-rw-r--r--   0        0        0      311 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/subversion.conf.2
+-rw-r--r--   0        0        0      319 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/subversion.conf.3
+-rw-r--r--   0        0        0      838 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/subversion.conf.4
+-rw-r--r--   0        0        0      323 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/subversion.conf.5
+-rw-r--r--   0        0        0      331 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/subversion.conf.6
+-rw-r--r--   0        0        0     1243 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/subversion.conf.7
+-rw-r--r--   0        0        0      263 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/tree1.ini
+-rw-r--r--   0        0        0     1021 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/tree1.tar.gz
+-rw-r--r--   0        0        0      391 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/tree10.tar.gz
+-rw-r--r--   0        0        0      641 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/tree11.tar.gz
+-rw-r--r--   0        0        0    75185 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/tree12.tar.gz
+-rw-r--r--   0        0        0      422 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/tree13.tar.gz
+-rw-r--r--   0        0        0      700 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/tree15.tar.gz
+-rw-r--r--   0        0        0     8971 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/tree16.tar.gz
+-rw-r--r--   0        0        0      997 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/tree17.tar.gz
+-rw-r--r--   0        0        0      968 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/tree18.tar.gz
+-rw-r--r--   0        0        0      939 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/tree19.tar.gz
+-rw-r--r--   0        0        0      269 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/tree2.ini
+-rw-r--r--   0        0        0      224 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/tree2.tar.gz
+-rw-r--r--   0        0        0      976 2023-06-10 22:14:59.427085 cedar_backup3-3.7.6/tests/data/tree20.tar.gz
+-rw-r--r--   0        0        0     3557 2023-06-10 22:14:59.431086 cedar_backup3-3.7.6/tests/data/tree21.tar.gz
+-rw-r--r--   0        0        0     6158 2023-06-10 22:14:59.431086 cedar_backup3-3.7.6/tests/data/tree22.tar.gz
+-rw-r--r--   0        0        0      270 2023-06-10 22:14:59.431086 cedar_backup3-3.7.6/tests/data/tree3.ini
+-rw-r--r--   0        0        0      604 2023-06-10 22:14:59.431086 cedar_backup3-3.7.6/tests/data/tree3.tar.gz
+-rw-r--r--   0        0        0      275 2023-06-10 22:14:59.431086 cedar_backup3-3.7.6/tests/data/tree4.ini
+-rw-r--r--   0        0        0     9120 2023-06-10 22:14:59.431086 cedar_backup3-3.7.6/tests/data/tree4.tar.gz
+-rw-r--r--   0        0        0      282 2023-06-10 22:14:59.431086 cedar_backup3-3.7.6/tests/data/tree5.ini
+-rw-r--r--   0        0        0    13611 2023-06-10 22:14:59.431086 cedar_backup3-3.7.6/tests/data/tree5.tar.gz
+-rw-r--r--   0        0        0      274 2023-06-10 22:14:59.431086 cedar_backup3-3.7.6/tests/data/tree6.ini
+-rw-r--r--   0        0        0    28998 2023-06-10 22:14:59.431086 cedar_backup3-3.7.6/tests/data/tree6.tar.gz
+-rw-r--r--   0        0        0      178 2023-06-10 22:14:59.431086 cedar_backup3-3.7.6/tests/data/tree7.tar.gz
+-rw-r--r--   0        0        0      148 2023-06-10 22:14:59.431086 cedar_backup3-3.7.6/tests/data/tree8.tar.gz
+-rw-r--r--   0        0        0      272 2023-06-10 22:14:59.431086 cedar_backup3-3.7.6/tests/data/tree9.ini
+-rw-r--r--   0        0        0     1394 2023-06-10 22:14:59.431086 cedar_backup3-3.7.6/tests/data/tree9.tar.gz
+-rw-r--r--   0        0        0     9503 2023-06-10 22:14:59.431086 cedar_backup3-3.7.6/tests/test_actions_util.py
+-rw-r--r--   0        0        0    36813 2023-06-10 22:14:59.431086 cedar_backup3-3.7.6/tests/test_amazons3.py
+-rw-r--r--   0        0        0    33089 2023-06-10 22:14:59.431086 cedar_backup3-3.7.6/tests/test_capacity.py
+-rw-r--r--   0        0        0    80468 2023-06-10 22:14:59.431086 cedar_backup3-3.7.6/tests/test_cdwriter.py
+-rw-r--r--   0        0        0   674560 2023-06-10 22:14:59.431086 cedar_backup3-3.7.6/tests/test_cli.py
+-rw-r--r--   0        0        0   542233 2023-06-10 22:14:59.435086 cedar_backup3-3.7.6/tests/test_config.py
+-rw-r--r--   0        0        0     8124 2023-06-10 22:14:59.435086 cedar_backup3-3.7.6/tests/test_customize.py
+-rw-r--r--   0        0        0    51496 2023-06-10 22:14:59.435086 cedar_backup3-3.7.6/tests/test_dvdwriter.py
+-rw-r--r--   0        0        0    54326 2023-06-10 22:14:59.435086 cedar_backup3-3.7.6/tests/test_encrypt.py
+-rw-r--r--   0        0        0  1291994 2023-06-10 22:14:59.443086 cedar_backup3-3.7.6/tests/test_filesystem.py
+-rw-r--r--   0        0        0    99436 2023-06-10 22:14:59.443086 cedar_backup3-3.7.6/tests/test_knapsack.py
+-rw-r--r--   0        0        0    84647 2023-06-10 22:14:59.443086 cedar_backup3-3.7.6/tests/test_mbox.py
+-rw-r--r--   0        0        0    40974 2023-06-10 22:14:59.443086 cedar_backup3-3.7.6/tests/test_mysql.py
+-rw-r--r--   0        0        0    68089 2023-06-10 22:14:59.443086 cedar_backup3-3.7.6/tests/test_peer.py
+-rw-r--r--   0        0        0    39155 2023-06-10 22:14:59.443086 cedar_backup3-3.7.6/tests/test_postgresql.py
+-rw-r--r--   0        0        0     4905 2023-06-10 22:14:59.443086 cedar_backup3-3.7.6/tests/test_span.py
+-rw-r--r--   0        0        0    46613 2023-06-10 22:14:59.443086 cedar_backup3-3.7.6/tests/test_split.py
+-rw-r--r--   0        0        0   108595 2023-06-10 22:14:59.443086 cedar_backup3-3.7.6/tests/test_subversion.py
+-rw-r--r--   0        0        0   153535 2023-06-10 22:14:59.443086 cedar_backup3-3.7.6/tests/test_sync.py
+-rw-r--r--   0        0        0   149942 2023-06-10 22:14:59.447087 cedar_backup3-3.7.6/tests/test_util.py
+-rw-r--r--   0        0        0    70705 2023-06-10 22:14:59.447087 cedar_backup3-3.7.6/tests/test_writers_util.py
+-rw-r--r--   0        0        0     4073 1970-01-01 00:00:00.000000 cedar_backup3-3.7.6/PKG-INFO
```

### Comparing `cedar_backup3-3.7.5/Changelog` & `cedar_backup3-3.7.6/Changelog`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+Version 3.7.6     10 Jun 2023
+
+	* Pin chardet and importlib-metadata to match Debian bookworm.
+
 Version 3.7.5     07 Jun 2023
 
 	* Fix checktabs to be safe for file named '-'.
 	* Upgrade all dependencies to the latest major version.
 	* Upgrade to Poetry v1.5.1 and make related adjustments.
 
 Version 3.7.4     31 Dec 2022
```

### Comparing `cedar_backup3-3.7.5/LICENSE` & `cedar_backup3-3.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/NOTICE` & `cedar_backup3-3.7.6/NOTICE`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/PyPI.md` & `cedar_backup3-3.7.6/PyPI.md`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/README.md` & `cedar_backup3-3.7.6/README.md`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/docs/Makefile` & `cedar_backup3-3.7.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/docs/_themes/LICENSE` & `cedar_backup3-3.7.6/docs/_themes/LICENSE`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/docs/_themes/flask_theme_support.py` & `cedar_backup3-3.7.6/docs/_themes/flask_theme_support.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/docs/conf.py` & `cedar_backup3-3.7.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/docs/index.rst` & `cedar_backup3-3.7.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/docs/make.bat` & `cedar_backup3-3.7.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/docs/manual/basic.rst` & `cedar_backup3-3.7.6/docs/manual/basic.rst`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/docs/manual/commandline.rst` & `cedar_backup3-3.7.6/docs/manual/commandline.rst`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/docs/manual/config.rst` & `cedar_backup3-3.7.6/docs/manual/config.rst`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/docs/manual/copyright.rst` & `cedar_backup3-3.7.6/docs/manual/copyright.rst`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/docs/manual/depends.rst` & `cedar_backup3-3.7.6/docs/manual/depends.rst`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/docs/manual/extensions.rst` & `cedar_backup3-3.7.6/docs/manual/extensions.rst`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/docs/manual/extenspec.rst` & `cedar_backup3-3.7.6/docs/manual/extenspec.rst`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/docs/manual/images/note.png` & `cedar_backup3-3.7.6/docs/manual/images/note.png`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/docs/manual/images/tip.png` & `cedar_backup3-3.7.6/docs/manual/images/tip.png`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/docs/manual/images/warning.png` & `cedar_backup3-3.7.6/docs/manual/images/warning.png`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/docs/manual/install.rst` & `cedar_backup3-3.7.6/docs/manual/install.rst`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/docs/manual/intro.rst` & `cedar_backup3-3.7.6/docs/manual/intro.rst`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/docs/manual/preface.rst` & `cedar_backup3-3.7.6/docs/manual/preface.rst`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/docs/manual/recovering.rst` & `cedar_backup3-3.7.6/docs/manual/recovering.rst`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/docs/manual/securingssh.rst` & `cedar_backup3-3.7.6/docs/manual/securingssh.rst`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/manpages/cback3-amazons3-sync.1` & `cedar_backup3-3.7.6/manpages/cback3-amazons3-sync.1`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/manpages/cback3-span.1` & `cedar_backup3-3.7.6/manpages/cback3-span.1`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/manpages/cback3.1` & `cedar_backup3-3.7.6/manpages/cback3.1`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/pyproject.toml` & `cedar_backup3-3.7.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cedar-backup3"
-version = "3.7.5" # published version is managed using Git tags (see below)
+version = "3.7.6" # published version is managed using Git tags (see below)
 description = "Implements local and remote backups to CD/DVD and Amazon S3"
 keywords = [ 'local', 'remote', 'backup', 'scp' ]
 authors = ["Kenneth J. Pronovici <pronovic@ieee.org>"]
 license = "GPL-2.0-only"
 readme = "PyPI.md"
 homepage = "https://pypi.org/project/cedar-backup3/"
 repository = "https://github.com/pronovic/cedar-backup3"
@@ -43,16 +43,16 @@
 [tool.poetry.scripts]
 cback3 = 'CedarBackup3.scripts:cback3' 
 cback3-amazons3-sync = 'CedarBackup3.scripts:amazons3' 
 cback3-span = 'CedarBackup3.scripts:span' 
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4"
-chardet = "^5.1.0"
-importlib-metadata = "^6.0.0"
+chardet = "^5.1.0,<6"               # Debian bookworm only has 5.1.0
+importlib-metadata = "^4.12.0,<5"   # Debian bookworm only has 4.12.0
 sphinx = { version="^6.1.3", optional=true }
 sphinx-autoapi = { version="^2.0.1", optional=true }
 
 [tool.poetry.extras]
 docs = [ "sphinx", "sphinx-autoapi" ]
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `cedar_backup3-3.7.5/samples/cback3.conf.sample` & `cedar_backup3-3.7.6/samples/cback3.conf.sample`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/src/CedarBackup3/__init__.py` & `cedar_backup3-3.7.6/src/CedarBackup3/__init__.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/src/CedarBackup3/action.py` & `cedar_backup3-3.7.6/src/CedarBackup3/action.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/src/CedarBackup3/actions/__init__.py` & `cedar_backup3-3.7.6/src/CedarBackup3/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/src/CedarBackup3/actions/collect.py` & `cedar_backup3-3.7.6/src/CedarBackup3/actions/collect.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/src/CedarBackup3/actions/constants.py` & `cedar_backup3-3.7.6/src/CedarBackup3/actions/constants.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/src/CedarBackup3/actions/initialize.py` & `cedar_backup3-3.7.6/src/CedarBackup3/actions/initialize.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/src/CedarBackup3/actions/purge.py` & `cedar_backup3-3.7.6/src/CedarBackup3/actions/purge.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/src/CedarBackup3/actions/rebuild.py` & `cedar_backup3-3.7.6/src/CedarBackup3/actions/rebuild.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/src/CedarBackup3/actions/stage.py` & `cedar_backup3-3.7.6/src/CedarBackup3/actions/stage.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/src/CedarBackup3/actions/store.py` & `cedar_backup3-3.7.6/src/CedarBackup3/actions/store.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/src/CedarBackup3/actions/util.py` & `cedar_backup3-3.7.6/src/CedarBackup3/actions/util.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/src/CedarBackup3/actions/validate.py` & `cedar_backup3-3.7.6/src/CedarBackup3/actions/validate.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/src/CedarBackup3/cli.py` & `cedar_backup3-3.7.6/src/CedarBackup3/cli.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/src/CedarBackup3/config.py` & `cedar_backup3-3.7.6/src/CedarBackup3/config.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/src/CedarBackup3/customize.py` & `cedar_backup3-3.7.6/src/CedarBackup3/customize.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/src/CedarBackup3/extend/__init__.py` & `cedar_backup3-3.7.6/src/CedarBackup3/extend/__init__.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/src/CedarBackup3/extend/amazons3.py` & `cedar_backup3-3.7.6/src/CedarBackup3/extend/amazons3.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/src/CedarBackup3/extend/capacity.py` & `cedar_backup3-3.7.6/src/CedarBackup3/extend/capacity.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/src/CedarBackup3/extend/encrypt.py` & `cedar_backup3-3.7.6/src/CedarBackup3/extend/encrypt.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/src/CedarBackup3/extend/mbox.py` & `cedar_backup3-3.7.6/src/CedarBackup3/extend/mbox.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/src/CedarBackup3/extend/mysql.py` & `cedar_backup3-3.7.6/src/CedarBackup3/extend/mysql.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/src/CedarBackup3/extend/postgresql.py` & `cedar_backup3-3.7.6/src/CedarBackup3/extend/postgresql.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/src/CedarBackup3/extend/split.py` & `cedar_backup3-3.7.6/src/CedarBackup3/extend/split.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/src/CedarBackup3/extend/subversion.py` & `cedar_backup3-3.7.6/src/CedarBackup3/extend/subversion.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/src/CedarBackup3/extend/sysinfo.py` & `cedar_backup3-3.7.6/src/CedarBackup3/extend/sysinfo.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/src/CedarBackup3/filesystem.py` & `cedar_backup3-3.7.6/src/CedarBackup3/filesystem.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/src/CedarBackup3/image.py` & `cedar_backup3-3.7.6/src/CedarBackup3/image.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/src/CedarBackup3/knapsack.py` & `cedar_backup3-3.7.6/src/CedarBackup3/knapsack.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/src/CedarBackup3/peer.py` & `cedar_backup3-3.7.6/src/CedarBackup3/peer.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/src/CedarBackup3/release.py` & `cedar_backup3-3.7.6/src/CedarBackup3/release.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/src/CedarBackup3/scripts.py` & `cedar_backup3-3.7.6/src/CedarBackup3/scripts.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/src/CedarBackup3/testutil.py` & `cedar_backup3-3.7.6/src/CedarBackup3/testutil.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/src/CedarBackup3/tools/__init__.py` & `cedar_backup3-3.7.6/src/CedarBackup3/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/src/CedarBackup3/tools/amazons3.py` & `cedar_backup3-3.7.6/src/CedarBackup3/tools/amazons3.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/src/CedarBackup3/tools/span.py` & `cedar_backup3-3.7.6/src/CedarBackup3/tools/span.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/src/CedarBackup3/util.py` & `cedar_backup3-3.7.6/src/CedarBackup3/util.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/src/CedarBackup3/writer.py` & `cedar_backup3-3.7.6/src/CedarBackup3/writer.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/src/CedarBackup3/writers/__init__.py` & `cedar_backup3-3.7.6/src/CedarBackup3/writers/__init__.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/src/CedarBackup3/writers/cdwriter.py` & `cedar_backup3-3.7.6/src/CedarBackup3/writers/cdwriter.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/src/CedarBackup3/writers/dvdwriter.py` & `cedar_backup3-3.7.6/src/CedarBackup3/writers/dvdwriter.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/src/CedarBackup3/writers/util.py` & `cedar_backup3-3.7.6/src/CedarBackup3/writers/util.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/src/CedarBackup3/xmlutil.py` & `cedar_backup3-3.7.6/src/CedarBackup3/xmlutil.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/__init__.py` & `cedar_backup3-3.7.6/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/data/cback.conf.1` & `cedar_backup3-3.7.6/tests/data/cback.conf.1`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/data/cback.conf.10` & `cedar_backup3-3.7.6/tests/data/cback.conf.10`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/data/cback.conf.12` & `cedar_backup3-3.7.6/tests/data/cback.conf.12`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/data/cback.conf.15` & `cedar_backup3-3.7.6/tests/data/cback.conf.15`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/data/cback.conf.19` & `cedar_backup3-3.7.6/tests/data/cback.conf.19`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/data/cback.conf.20` & `cedar_backup3-3.7.6/tests/data/cback.conf.20`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/data/cback.conf.21` & `cedar_backup3-3.7.6/tests/data/cback.conf.21`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/data/cback.conf.23` & `cedar_backup3-3.7.6/tests/data/cback.conf.23`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/data/cback.conf.6` & `cedar_backup3-3.7.6/tests/data/cback.conf.6`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/data/cback.conf.8` & `cedar_backup3-3.7.6/tests/data/cback.conf.8`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/data/lotsoflines.py` & `cedar_backup3-3.7.6/tests/data/lotsoflines.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/data/mbox.conf.4` & `cedar_backup3-3.7.6/tests/data/mbox.conf.4`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/data/subversion.conf.4` & `cedar_backup3-3.7.6/tests/data/subversion.conf.4`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/data/subversion.conf.7` & `cedar_backup3-3.7.6/tests/data/subversion.conf.7`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/data/tree1.tar.gz` & `cedar_backup3-3.7.6/tests/data/tree1.tar.gz`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/data/tree11.tar.gz` & `cedar_backup3-3.7.6/tests/data/tree11.tar.gz`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/data/tree12.tar.gz` & `cedar_backup3-3.7.6/tests/data/tree12.tar.gz`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/data/tree15.tar.gz` & `cedar_backup3-3.7.6/tests/data/tree15.tar.gz`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/data/tree16.tar.gz` & `cedar_backup3-3.7.6/tests/data/tree16.tar.gz`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/data/tree17.tar.gz` & `cedar_backup3-3.7.6/tests/data/tree17.tar.gz`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/data/tree18.tar.gz` & `cedar_backup3-3.7.6/tests/data/tree18.tar.gz`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/data/tree19.tar.gz` & `cedar_backup3-3.7.6/tests/data/tree19.tar.gz`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/data/tree20.tar.gz` & `cedar_backup3-3.7.6/tests/data/tree20.tar.gz`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/data/tree21.tar.gz` & `cedar_backup3-3.7.6/tests/data/tree21.tar.gz`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/data/tree22.tar.gz` & `cedar_backup3-3.7.6/tests/data/tree22.tar.gz`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/data/tree3.tar.gz` & `cedar_backup3-3.7.6/tests/data/tree3.tar.gz`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/data/tree4.tar.gz` & `cedar_backup3-3.7.6/tests/data/tree4.tar.gz`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/data/tree5.tar.gz` & `cedar_backup3-3.7.6/tests/data/tree5.tar.gz`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/data/tree6.tar.gz` & `cedar_backup3-3.7.6/tests/data/tree6.tar.gz`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/data/tree9.tar.gz` & `cedar_backup3-3.7.6/tests/data/tree9.tar.gz`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/test_actions_util.py` & `cedar_backup3-3.7.6/tests/test_actions_util.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/test_amazons3.py` & `cedar_backup3-3.7.6/tests/test_amazons3.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/test_capacity.py` & `cedar_backup3-3.7.6/tests/test_capacity.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/test_cdwriter.py` & `cedar_backup3-3.7.6/tests/test_cdwriter.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/test_cli.py` & `cedar_backup3-3.7.6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/test_config.py` & `cedar_backup3-3.7.6/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/test_customize.py` & `cedar_backup3-3.7.6/tests/test_customize.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/test_dvdwriter.py` & `cedar_backup3-3.7.6/tests/test_dvdwriter.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/test_encrypt.py` & `cedar_backup3-3.7.6/tests/test_encrypt.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/test_filesystem.py` & `cedar_backup3-3.7.6/tests/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/test_knapsack.py` & `cedar_backup3-3.7.6/tests/test_knapsack.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/test_mbox.py` & `cedar_backup3-3.7.6/tests/test_mbox.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/test_mysql.py` & `cedar_backup3-3.7.6/tests/test_mysql.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/test_peer.py` & `cedar_backup3-3.7.6/tests/test_peer.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/test_postgresql.py` & `cedar_backup3-3.7.6/tests/test_postgresql.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/test_span.py` & `cedar_backup3-3.7.6/tests/test_span.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/test_split.py` & `cedar_backup3-3.7.6/tests/test_split.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/test_subversion.py` & `cedar_backup3-3.7.6/tests/test_subversion.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/test_sync.py` & `cedar_backup3-3.7.6/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/test_util.py` & `cedar_backup3-3.7.6/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/tests/test_writers_util.py` & `cedar_backup3-3.7.6/tests/test_writers_util.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.5/PKG-INFO` & `cedar_backup3-3.7.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cedar-backup3
-Version: 3.7.5
+Version: 3.7.6
 Summary: Implements local and remote backups to CD/DVD and Amazon S3
 Home-page: https://pypi.org/project/cedar-backup3/
 License: GPL-2.0-only
 Keywords: local,remote,backup,scp
 Author: Kenneth J. Pronovici
 Author-email: pronovic@ieee.org
 Requires-Python: >=3.8,<4
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Archiving :: Backup
 Classifier: Topic :: Utilities
 Provides-Extra: docs
 Requires-Dist: chardet (>=5.1.0,<6.0.0)
-Requires-Dist: importlib-metadata (>=6.0.0,<7.0.0)
+Requires-Dist: importlib-metadata (>=4.12.0,<5.0.0)
 Requires-Dist: sphinx (>=6.1.3,<7.0.0) ; extra == "docs"
 Requires-Dist: sphinx-autoapi (>=2.0.1,<3.0.0) ; extra == "docs"
 Project-URL: Repository, https://github.com/pronovic/cedar-backup3
 Description-Content-Type: text/markdown
 
 [![pypi](https://img.shields.io/pypi/v/cedar-backup3.svg)](https://pypi.org/project/cedar-backup3/)
 [![license](https://img.shields.io/pypi/l/cedar-backup3.svg)](https://github.com/pronovic/cedar-backup3/blob/master/LICENSE)
```

