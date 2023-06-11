# Comparing `tmp/oemof.solph-0.5.1.dev0.tar.gz` & `tmp/oemof.solph-0.5.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oemof.solph-0.5.1.dev0.tar", last modified: Fri Mar 24 19:10:13 2023, max compression
+gzip compressed data, was "oemof.solph-0.5.1.dev1.tar", last modified: Sun Jun 11 18:27:30 2023, max compression
```

## Comparing `oemof.solph-0.5.1.dev0.tar` & `oemof.solph-0.5.1.dev1.tar`

### file list

```diff
@@ -1,305 +1,386 @@
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-03-24 19:10:13.604283 oemof.solph-0.5.1.dev0/
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      513 2023-03-24 19:08:46.000000 oemof.solph-0.5.1.dev0/.bumpversion.cfg
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     2777 2023-03-24 19:08:46.000000 oemof.solph-0.5.1.dev0/.cookiecutterrc
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      187 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/.coveragerc
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      217 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev0/.editorconfig
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      309 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/.pep8speaks.yml
--rw-rw-r--   0 patrik    (1001) patrik    (1001)       74 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev0/.prospector.yml
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      288 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/.readthedocs.yml
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      701 2023-02-22 20:48:01.000000 oemof.solph-0.5.1.dev0/AUTHORS.rst
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     3091 2023-02-22 20:48:01.000000 oemof.solph-0.5.1.dev0/CITATION.cff
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     3243 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/CODE_OF_CONDUCT.md
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     3319 2023-02-22 20:48:01.000000 oemof.solph-0.5.1.dev0/CONTRIBUTING.rst
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     1084 2023-03-24 19:08:46.000000 oemof.solph-0.5.1.dev0/LICENSE
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      490 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/MANIFEST.in
--rw-rw-r--   0 patrik    (1001) patrik    (1001)    13182 2023-03-24 19:10:13.604283 oemof.solph-0.5.1.dev0/PKG-INFO
--rw-rw-r--   0 patrik    (1001) patrik    (1001)    11790 2023-03-24 19:08:46.000000 oemof.solph-0.5.1.dev0/README.rst
--rw-rw-r--   0 patrik    (1001) patrik    (1001)       27 2023-03-24 19:08:46.000000 oemof.solph-0.5.1.dev0/VERSION
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-03-24 19:10:13.576283 oemof.solph-0.5.1.dev0/ci/
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      763 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev0/ci/appveyor-with-compiler.cmd
--rwxrwxr-x   0 patrik    (1001) patrik    (1001)     3077 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev0/ci/bootstrap.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)       62 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev0/ci/requirements.txt
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-03-24 19:10:13.576283 oemof.solph-0.5.1.dev0/ci/templates/
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     1887 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev0/ci/templates/.appveyor.yml
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     1440 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev0/ci/templates/.travis.yml
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     2138 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev0/ci/templates/tox.ini
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-03-24 19:10:13.576283 oemof.solph-0.5.1.dev0/docs/
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-03-24 19:10:13.584283 oemof.solph-0.5.1.dev0/docs/_files/
--rw-rw-r--   0 patrik    (1001) patrik    (1001)    25411 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev0/docs/_files/ExtractionTurbine_range_of_operation.svg
--rwxrwxr-x   0 patrik    (1001) patrik    (1001)    23219 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev0/docs/_files/GenericCHP.svg
--rw-rw-r--   0 patrik    (1001) patrik    (1001)    45060 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev0/docs/_files/OffsetTransformer_efficiency.svg
--rw-rw-r--   0 patrik    (1001) patrik    (1001)    44787 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev0/docs/_files/OffsetTransformer_power_relation.svg
--rw-rw-r--   0 patrik    (1001) patrik    (1001)    47077 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev0/docs/_files/Plot_delay_2013-01-01.svg
--rw-rw-r--   0 patrik    (1001) patrik    (1001)   988676 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/docs/_files/diesel_genset_investment_flow.svg
--rw-rw-r--   0 patrik    (1001) patrik    (1001)   983065 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/docs/_files/diesel_genset_nonconvex_flow.svg
--rw-rw-r--   0 patrik    (1001) patrik    (1001)  2006893 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/docs/_files/diesel_genset_nonconvex_invest_flow.svg
--rw-rw-r--   0 patrik    (1001) patrik    (1001)   104510 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev0/docs/_files/example_figures.png
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     4837 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev0/docs/_files/example_network.svg
--rw-rw-r--   0 patrik    (1001) patrik    (1001)    23158 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev0/docs/_files/example_variable_chp.svg
--rw-rw-r--   0 patrik    (1001) patrik    (1001)    34377 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev0/docs/_files/framework_concept.svg
--rw-rw-r--   0 patrik    (1001) patrik    (1001)    52711 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev0/docs/_files/nonconvex_invest_investcosts_power.svg
--rw-rw-r--   0 patrik    (1001) patrik    (1001)    36889 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev0/docs/_files/nonconvex_invest_specific_costs.svg
--rw-rw-r--   0 patrik    (1001) patrik    (1001)    20370 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev0/docs/_files/oemof_solph_example.svg
--rw-rw-r--   0 patrik    (1001) patrik    (1001)        0 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev0/docs/_files/pahesmf_init.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)   406713 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev0/docs/_files/variable_chp_plot.svg
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-03-24 19:10:13.584283 oemof.solph-0.5.1.dev0/docs/_logo/
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      621 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/docs/_logo/README.rst
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-03-24 19:10:13.584283 oemof.solph-0.5.1.dev0/docs/_logo/editable_fonts/
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     6966 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/docs/_logo/editable_fonts/logo_oemof_solph_COMPACT_editable_fonts.svg
--rw-rw-r--   0 patrik    (1001) patrik    (1001)    12120 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/docs/_logo/editable_fonts/logo_oemof_solph_FULL_editable_fonts.svg
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     2987 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/docs/_logo/editable_fonts/logo_oemof_solph_ICON_editable_fonts.svg
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     9778 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/docs/_logo/editable_fonts/logo_oemof_solph_NOTEXT_editable_fonts.svg
--rw-rw-r--   0 patrik    (1001) patrik    (1001)    11285 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/docs/_logo/logo_oemof_solph_COMPACT.svg
--rw-rw-r--   0 patrik    (1001) patrik    (1001)    12456 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/docs/_logo/logo_oemof_solph_COMPACT_bg.svg
--rw-rw-r--   0 patrik    (1001) patrik    (1001)    30395 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/docs/_logo/logo_oemof_solph_FULL.svg
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     3802 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/docs/_logo/logo_oemof_solph_ICON.svg
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     9669 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/docs/_logo/logo_oemof_solph_NOTEXT.svg
--rw-rw-r--   0 patrik    (1001) patrik    (1001)       28 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev0/docs/authors.rst
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      941 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/docs/changelog.rst
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     2034 2023-03-24 19:08:46.000000 oemof.solph-0.5.1.dev0/docs/conf.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)       33 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev0/docs/contributing.rst
--rw-rw-r--   0 patrik    (1001) patrik    (1001)       52 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev0/docs/docutils.conf
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-03-24 19:10:13.584283 oemof.solph-0.5.1.dev0/docs/examples/
--rw-rw-r--   0 patrik    (1001) patrik    (1001)       85 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/docs/examples/index.rst
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     2410 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/docs/examples/solph.examples.rst
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      558 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/docs/index.rst
--rw-rw-r--   0 patrik    (1001) patrik    (1001)       27 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev0/docs/readme.rst
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-03-24 19:10:13.584283 oemof.solph-0.5.1.dev0/docs/reference/
--rw-rw-r--   0 patrik    (1001) patrik    (1001)       97 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev0/docs/reference/index.rst
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      141 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/docs/reference/oemof.solph.busses.rst
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     1903 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev0/docs/reference/oemof.solph.components.rst
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      161 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/docs/reference/oemof.solph.console_scripts.rst
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      344 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/docs/reference/oemof.solph.constraints.rst
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      151 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/docs/reference/oemof.solph.energy_system.rst
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      729 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/docs/reference/oemof.solph.flow.rst
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      141 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/docs/reference/oemof.solph.groupings.rst
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      135 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/docs/reference/oemof.solph.helpers.rst
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      132 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/docs/reference/oemof.solph.models.rst
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      135 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/docs/reference/oemof.solph.options.rst
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      138 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/docs/reference/oemof.solph.plumbing.rst
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      143 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/docs/reference/oemof.solph.processing.rst
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      128 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/docs/reference/oemof.solph.views.rst
--rw-rw-r--   0 patrik    (1001) patrik    (1001)       51 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/docs/requirements.txt
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      109 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev0/docs/spelling_wordlist.txt
--rw-rw-r--   0 patrik    (1001) patrik    (1001)    63717 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev0/docs/usage.rst
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-03-24 19:10:13.588283 oemof.solph-0.5.1.dev0/docs/whatsnew/
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      100 2023-01-24 16:30:15.000000 oemof.solph-0.5.1.dev0/docs/whatsnew/v0-0-1.rst
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     2744 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/docs/whatsnew/v0-0-2.rst
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     1869 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/docs/whatsnew/v0-0-3.rst
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      900 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/docs/whatsnew/v0-0-4.rst
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     1781 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/docs/whatsnew/v0-0-5.rst
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     1145 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/docs/whatsnew/v0-0-6.rst
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      115 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/docs/whatsnew/v0-0-7.rst
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     2938 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/docs/whatsnew/v0-1-0.rst
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      446 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/docs/whatsnew/v0-1-1.rst
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     1852 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/docs/whatsnew/v0-1-2.rst
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      296 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/docs/whatsnew/v0-1-4.rst
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     8202 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/docs/whatsnew/v0-2-0.rst
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     3618 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/docs/whatsnew/v0-2-1.rst
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     3980 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/docs/whatsnew/v0-2-2.rst
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      390 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/docs/whatsnew/v0-2-3.rst
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     4258 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/docs/whatsnew/v0-3-0.rst
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      522 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/docs/whatsnew/v0-3-1.rst
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     1096 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/docs/whatsnew/v0-3-2.rst
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     3847 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/docs/whatsnew/v0-4-0.rst
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      506 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/docs/whatsnew/v0-4-1.rst
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      156 2023-01-24 16:30:15.000000 oemof.solph-0.5.1.dev0/docs/whatsnew/v0-4-2.rst
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     1634 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/docs/whatsnew/v0-4-4.rst
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     1051 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/docs/whatsnew/v0-4-5.rst
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     1843 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/docs/whatsnew/v0-5-0.rst
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      293 2023-02-22 20:48:01.000000 oemof.solph-0.5.1.dev0/docs/whatsnew/v0-5-1.rst
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-03-24 19:10:13.572283 oemof.solph-0.5.1.dev0/examples/
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-03-24 19:10:13.588283 oemof.solph-0.5.1.dev0/examples/basic_example/
--rw-rw-r--   0 patrik    (1001) patrik    (1001)   288296 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/examples/basic_example/basic_example.csv
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-03-24 19:10:13.588283 oemof.solph-0.5.1.dev0/examples/excel_reader/
--rwxrwxr-x   0 patrik    (1001) patrik    (1001)   577434 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/examples/excel_reader/scenario.xlsx
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-03-24 19:10:13.588283 oemof.solph-0.5.1.dev0/examples/invest_nonconvex_flow_examples/
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     2995 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/examples/invest_nonconvex_flow_examples/solar_generation.csv
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-03-24 19:10:13.588283 oemof.solph-0.5.1.dev0/examples/simple_dispatch/
--rw-rw-r--   0 patrik    (1001) patrik    (1001)   401132 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/examples/simple_dispatch/input_data.csv
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-03-24 19:10:13.588283 oemof.solph-0.5.1.dev0/examples/storage_investment/
--rw-rw-r--   0 patrik    (1001) patrik    (1001)   288296 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/examples/storage_investment/storage_investment.csv
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-03-24 19:10:13.592283 oemof.solph-0.5.1.dev0/examples/tuple_as_labels/
--rw-rw-r--   0 patrik    (1001) patrik    (1001)   288296 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/examples/tuple_as_labels/tuple_as_label.csv
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-03-24 19:10:13.592283 oemof.solph-0.5.1.dev0/examples/variable_chp/
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     6335 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/examples/variable_chp/variable_chp.csv
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      322 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev0/pyproject.toml
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      945 2023-03-24 19:10:13.604283 oemof.solph-0.5.1.dev0/setup.cfg
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     3100 2023-03-24 19:08:46.000000 oemof.solph-0.5.1.dev0/setup.py
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-03-24 19:10:13.572283 oemof.solph-0.5.1.dev0/src/
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-03-24 19:10:13.572283 oemof.solph-0.5.1.dev0/src/oemof/
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-03-24 19:10:13.592283 oemof.solph-0.5.1.dev0/src/oemof/solph/
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      818 2023-03-24 19:08:46.000000 oemof.solph-0.5.1.dev0/src/oemof/solph/__init__.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     1832 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev0/src/oemof/solph/_console_scripts.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     6728 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/src/oemof/solph/_energy_system.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     3655 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/src/oemof/solph/_groupings.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     1222 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/src/oemof/solph/_helpers.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)    14576 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev0/src/oemof/solph/_models.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     8129 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/src/oemof/solph/_options.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     2091 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/src/oemof/solph/_plumbing.py
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-03-24 19:10:13.592283 oemof.solph-0.5.1.dev0/src/oemof/solph/buses/
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      445 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/src/oemof/solph/buses/__init__.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     3685 2023-03-24 19:00:19.000000 oemof.solph-0.5.1.dev0/src/oemof/solph/buses/_bus.py
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-03-24 19:10:13.592283 oemof.solph-0.5.1.dev0/src/oemof/solph/buses/experimental/
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      385 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/src/oemof/solph/buses/experimental/__init__.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     1495 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/src/oemof/solph/buses/experimental/_electrical_bus.py
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-03-24 19:10:13.592283 oemof.solph-0.5.1.dev0/src/oemof/solph/components/
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      835 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev0/src/oemof/solph/components/__init__.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     8585 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev0/src/oemof/solph/components/_extraction_turbine_chp.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)    18657 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/src/oemof/solph/components/_generic_chp.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)    38990 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/src/oemof/solph/components/_generic_storage.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     6323 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev0/src/oemof/solph/components/_offset_transformer.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     1854 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/src/oemof/solph/components/_sink.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     2046 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/src/oemof/solph/components/_source.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     8406 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev0/src/oemof/solph/components/_transformer.py
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-03-24 19:10:13.592283 oemof.solph-0.5.1.dev0/src/oemof/solph/components/experimental/
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      565 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev0/src/oemof/solph/components/experimental/__init__.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)    25057 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/src/oemof/solph/components/experimental/_generic_caes.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     5699 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/src/oemof/solph/components/experimental/_link.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     6413 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev0/src/oemof/solph/components/experimental/_piecewise_linear_transformer.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)   175821 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/src/oemof/solph/components/experimental/_sink_dsm.py
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-03-24 19:10:13.592283 oemof.solph-0.5.1.dev0/src/oemof/solph/constraints/
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      890 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/src/oemof/solph/constraints/__init__.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     2873 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/src/oemof/solph/constraints/equate_flows.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     5642 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev0/src/oemof/solph/constraints/equate_variables.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     4450 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/src/oemof/solph/constraints/flow_count_limit.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     4477 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/src/oemof/solph/constraints/integral_limit.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     5338 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/src/oemof/solph/constraints/investment_limit.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     3495 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/src/oemof/solph/constraints/shared_limit.py
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-03-24 19:10:13.596283 oemof.solph-0.5.1.dev0/src/oemof/solph/flows/
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      508 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/src/oemof/solph/flows/__init__.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)    10315 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/src/oemof/solph/flows/_flow.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)    10509 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/src/oemof/solph/flows/_invest_non_convex_flow_block.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)    12866 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/src/oemof/solph/flows/_investment_flow_block.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)    24172 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/src/oemof/solph/flows/_non_convex_flow_block.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)    10538 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/src/oemof/solph/flows/_simple_flow_block.py
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-03-24 19:10:13.596283 oemof.solph-0.5.1.dev0/src/oemof/solph/flows/experimental/
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      388 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/src/oemof/solph/flows/experimental/__init__.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     6880 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/src/oemof/solph/flows/experimental/_electrical_line.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     1777 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/src/oemof/solph/helpers.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)    16539 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/src/oemof/solph/processing.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)    12437 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev0/src/oemof/solph/views.py
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-03-24 19:10:13.592283 oemof.solph-0.5.1.dev0/src/oemof.solph.egg-info/
--rw-rw-r--   0 patrik    (1001) patrik    (1001)    13182 2023-03-24 19:10:13.000000 oemof.solph-0.5.1.dev0/src/oemof.solph.egg-info/PKG-INFO
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     9848 2023-03-24 19:10:13.000000 oemof.solph-0.5.1.dev0/src/oemof.solph.egg-info/SOURCES.txt
--rw-rw-r--   0 patrik    (1001) patrik    (1001)        1 2023-03-24 19:10:13.000000 oemof.solph-0.5.1.dev0/src/oemof.solph.egg-info/dependency_links.txt
--rw-rw-r--   0 patrik    (1001) patrik    (1001)       98 2023-03-24 19:10:13.000000 oemof.solph-0.5.1.dev0/src/oemof.solph.egg-info/entry_points.txt
--rw-rw-r--   0 patrik    (1001) patrik    (1001)        1 2022-10-04 09:53:33.000000 oemof.solph-0.5.1.dev0/src/oemof.solph.egg-info/not-zip-safe
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      208 2023-03-24 19:10:13.000000 oemof.solph-0.5.1.dev0/src/oemof.solph.egg-info/requires.txt
--rw-rw-r--   0 patrik    (1001) patrik    (1001)        6 2023-03-24 19:10:13.000000 oemof.solph-0.5.1.dev0/src/oemof.solph.egg-info/top_level.txt
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-03-24 19:10:13.596283 oemof.solph-0.5.1.dev0/tests/
--rw-rw-r--   0 patrik    (1001) patrik    (1001)    57301 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev0/tests/constraint_tests.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     2457 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/tests/flow_tests.py
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-03-24 19:10:13.600283 oemof.solph-0.5.1.dev0/tests/lp_files/
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     3363 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/tests/lp_files/activity_costs.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     6219 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/tests/lp_files/connect_investment.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     5321 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/tests/lp_files/dsm_module_DIW.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     6910 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/tests/lp_files/dsm_module_DIW_invest.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)    12736 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/tests/lp_files/dsm_module_DLR.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)    16039 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/tests/lp_files/dsm_module_DLR_invest.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     3225 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/tests/lp_files/dsm_module_oemof.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     4247 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/tests/lp_files/dsm_module_oemof_invest.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     1262 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/tests/lp_files/emission_limit.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     1246 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/tests/lp_files/equate_flows.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     1501 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/tests/lp_files/fixed_source_invest_sink.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      611 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/tests/lp_files/fixed_source_variable_sink.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     7709 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/tests/lp_files/flow_count_limit.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     2591 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/tests/lp_files/flow_invest_with_offset.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     2517 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/tests/lp_files/flow_invest_with_offset_no_minimum.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     2449 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/tests/lp_files/flow_invest_without_offset.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     7311 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev0/tests/lp_files/flow_nonconvex_invest_bounded_transformer.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     2400 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/tests/lp_files/generic_invest_limit.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     3479 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/tests/lp_files/inactivity_costs.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     3825 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/tests/lp_files/invest_non_convex_flow.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     1090 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/tests/lp_files/invest_source_fixed_sink.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     5508 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/tests/lp_files/investment_limit.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     1424 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev0/tests/lp_files/linear_transformer.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     2378 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev0/tests/lp_files/linear_transformer_chp.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     3037 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev0/tests/lp_files/linear_transformer_chp_invest.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     2040 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev0/tests/lp_files/linear_transformer_invest.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     1642 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/tests/lp_files/link.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      932 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/tests/lp_files/max_source_min_sink.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     4856 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/tests/lp_files/maximum_shutdowns.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     4774 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/tests/lp_files/maximum_startups.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     7446 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/tests/lp_files/min_max_runtime.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      478 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/tests/lp_files/nominal_value_to_zero.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     6239 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev0/tests/lp_files/nonequidistant_timeindex.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     3347 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev0/tests/lp_files/offsettransformer.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)    13482 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev0/tests/lp_files/piecewise_linear_transformer_cc.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)    14100 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev0/tests/lp_files/piecewise_linear_transformer_dcc.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     3571 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/tests/lp_files/shared_limit.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     1902 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/tests/lp_files/source_with_gradient.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     4418 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/tests/lp_files/source_with_nonconvex_gradient.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     2349 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/tests/lp_files/storage.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     2358 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/tests/lp_files/storage_fixed_losses.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     5273 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/tests/lp_files/storage_invest_1.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     5435 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/tests/lp_files/storage_invest_1_fixed_losses.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     3994 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/tests/lp_files/storage_invest_2.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     3001 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/tests/lp_files/storage_invest_3.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     2820 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/tests/lp_files/storage_invest_4.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     3166 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/tests/lp_files/storage_invest_5.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     4182 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/tests/lp_files/storage_invest_6.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     6312 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/tests/lp_files/storage_invest_all_nonconvex.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     2831 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/tests/lp_files/storage_invest_minimum.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     4062 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/tests/lp_files/storage_invest_unbalanced.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     6685 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/tests/lp_files/storage_invest_with_offset.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     6714 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/tests/lp_files/storage_invest_without_offset.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     1699 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/tests/lp_files/storage_unbalanced.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     4271 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev0/tests/lp_files/transformer.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     5023 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev0/tests/lp_files/transformer_invest.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     5029 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev0/tests/lp_files/transformer_invest_with_existing.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     4609 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/tests/lp_files/variable_chp.lp
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      899 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/tests/regression_tests.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     9920 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev0/tests/test_components.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      493 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/tests/test_console_scripts.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     2045 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev0/tests/test_constraints_module.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     2172 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/tests/test_grouping.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      434 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/tests/test_helpers.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     1904 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/tests/test_models.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     8094 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev0/tests/test_non_equidistant_time_index.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      189 2023-02-22 20:48:11.000000 oemof.solph-0.5.1.dev0/tests/test_oemof_installation_test.py
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-03-24 19:10:13.600283 oemof.solph-0.5.1.dev0/tests/test_outputlib/
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     3500 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev0/tests/test_outputlib/__init__.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     5522 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev0/tests/test_outputlib/input_data.csv
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     2179 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/tests/test_outputlib/test_views.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)    12169 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev0/tests/test_processing.py
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-03-24 19:10:13.572283 oemof.solph-0.5.1.dev0/tests/test_scripts/
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-03-24 19:10:13.572283 oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-03-24 19:10:13.600283 oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_connect_invest/
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     5179 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_connect_invest/connect_invest.csv
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     4210 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_connect_invest/test_connect_invest.py
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-03-24 19:10:13.600283 oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_flexible_modelling/
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     4279 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_flexible_modelling/test_add_constraints.py
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-03-24 19:10:13.600283 oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_generic_caes/
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     3871 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_generic_caes/generic_caes.csv
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     4398 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_generic_caes/test_generic_caes.py
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-03-24 19:10:13.600283 oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_generic_chp/
--rw-rw-r--   0 patrik    (1001) patrik    (1001)    10281 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_generic_chp/ccet.csv
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     3485 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_generic_chp/test_generic_chp.py
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-03-24 19:10:13.600283 oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_invest_fix_flow/
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      100 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_invest_fix_flow/input_data.csv
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     2987 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_invest_fix_flow/test_simple_invest_fixed.py
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-03-24 19:10:13.600283 oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_lopf/
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     3918 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_lopf/test_lopf.py
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-03-24 19:10:13.600283 oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_options/
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     1126 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_options/test_non_convex.py
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-03-24 19:10:13.600283 oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_piecewiselineartransformer/
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     3315 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_piecewiselineartransformer/test_piecewiselineartransformer.py
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-03-24 19:10:13.600283 oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_simple_model/
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     5522 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_simple_model/input_data.csv
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     5821 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_simple_model/test_simple_dispatch.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     3640 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_simple_model/test_simple_dispatch_one.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     3640 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_simple_model/test_simple_dispatch_one_explicit_timemode.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     6412 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_simple_model/test_simple_invest.py
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-03-24 19:10:13.604283 oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_storage_investment/
--rw-rw-r--   0 patrik    (1001) patrik    (1001)    15331 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_storage_investment/storage_investment.csv
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     2868 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_storage_investment/test_invest_storage_regression.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     6541 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_storage_investment/test_storage_investment.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     7115 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_storage_investment/test_storage_with_tuple_label.py
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-03-24 19:10:13.604283 oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_variable_chp/
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     6542 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_variable_chp/test_variable_chp.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      193 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_variable_chp/variable_chp.csv
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     4472 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev0/tests/test_solph_network_classes.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     5750 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev0/tests/test_time_index.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     5307 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev0/tests/test_warnings.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     2180 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev0/tox.ini
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-06-11 18:27:30.612211 oemof.solph-0.5.1.dev1/
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      513 2023-05-04 19:13:57.000000 oemof.solph-0.5.1.dev1/.bumpversion.cfg
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     2777 2023-05-04 19:13:57.000000 oemof.solph-0.5.1.dev1/.cookiecutterrc
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      187 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/.coveragerc
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      217 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev1/.editorconfig
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      309 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/.pep8speaks.yml
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)       74 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev1/.prospector.yml
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      288 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/.readthedocs.yml
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      701 2023-02-22 20:48:01.000000 oemof.solph-0.5.1.dev1/AUTHORS.rst
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     3091 2023-02-22 20:48:01.000000 oemof.solph-0.5.1.dev1/CITATION.cff
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     3243 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     3212 2023-05-11 14:57:44.000000 oemof.solph-0.5.1.dev1/CONTRIBUTING.rst
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     1084 2023-05-04 19:13:57.000000 oemof.solph-0.5.1.dev1/LICENSE
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      490 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/MANIFEST.in
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    13182 2023-06-11 18:27:30.612211 oemof.solph-0.5.1.dev1/PKG-INFO
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    11790 2023-05-04 19:13:57.000000 oemof.solph-0.5.1.dev1/README.rst
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)       27 2023-05-04 19:13:57.000000 oemof.solph-0.5.1.dev1/VERSION
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-06-11 18:27:30.556212 oemof.solph-0.5.1.dev1/ci/
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      763 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev1/ci/appveyor-with-compiler.cmd
+-rwxrwxr-x   0 patrik    (1001) patrik    (1001)     3077 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev1/ci/bootstrap.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)       62 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev1/ci/requirements.txt
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-06-11 18:27:30.556212 oemof.solph-0.5.1.dev1/ci/templates/
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     1887 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev1/ci/templates/.appveyor.yml
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     1440 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev1/ci/templates/.travis.yml
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     2138 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev1/ci/templates/tox.ini
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-06-11 18:27:30.560212 oemof.solph-0.5.1.dev1/docs/
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-06-11 18:27:30.572212 oemof.solph-0.5.1.dev1/docs/_files/
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    25411 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev1/docs/_files/ExtractionTurbine_range_of_operation.svg
+-rwxrwxr-x   0 patrik    (1001) patrik    (1001)    23219 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev1/docs/_files/GenericCHP.svg
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    45060 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev1/docs/_files/OffsetTransformer_efficiency.svg
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    44787 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev1/docs/_files/OffsetTransformer_power_relation.svg
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    47077 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev1/docs/_files/Plot_delay_2013-01-01.svg
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)   988676 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev1/docs/_files/diesel_genset_investment_flow.svg
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)   983065 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev1/docs/_files/diesel_genset_nonconvex_flow.svg
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)  2006893 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev1/docs/_files/diesel_genset_nonconvex_invest_flow.svg
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)   104510 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev1/docs/_files/example_figures.png
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     4837 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev1/docs/_files/example_network.svg
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    23158 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev1/docs/_files/example_variable_chp.svg
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    34377 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev1/docs/_files/framework_concept.svg
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    52711 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev1/docs/_files/nonconvex_invest_investcosts_power.svg
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    36889 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev1/docs/_files/nonconvex_invest_specific_costs.svg
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    20370 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev1/docs/_files/oemof_solph_example.svg
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)        0 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev1/docs/_files/pahesmf_init.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)   406713 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev1/docs/_files/variable_chp_plot.svg
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-06-11 18:27:30.572212 oemof.solph-0.5.1.dev1/docs/_logo/
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      621 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev1/docs/_logo/README.rst
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-06-11 18:27:30.572212 oemof.solph-0.5.1.dev1/docs/_logo/editable_fonts/
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     6966 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev1/docs/_logo/editable_fonts/logo_oemof_solph_COMPACT_editable_fonts.svg
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    12120 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev1/docs/_logo/editable_fonts/logo_oemof_solph_FULL_editable_fonts.svg
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     2987 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev1/docs/_logo/editable_fonts/logo_oemof_solph_ICON_editable_fonts.svg
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     9778 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev1/docs/_logo/editable_fonts/logo_oemof_solph_NOTEXT_editable_fonts.svg
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    11285 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev1/docs/_logo/logo_oemof_solph_COMPACT.svg
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    12456 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev1/docs/_logo/logo_oemof_solph_COMPACT_bg.svg
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    30395 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev1/docs/_logo/logo_oemof_solph_FULL.svg
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     3802 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev1/docs/_logo/logo_oemof_solph_ICON.svg
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     9669 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev1/docs/_logo/logo_oemof_solph_NOTEXT.svg
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)       28 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev1/docs/authors.rst
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      975 2023-05-15 14:22:45.000000 oemof.solph-0.5.1.dev1/docs/changelog.rst
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     2034 2023-05-04 19:13:57.000000 oemof.solph-0.5.1.dev1/docs/conf.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)       33 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev1/docs/contributing.rst
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)       52 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev1/docs/docutils.conf
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-06-11 18:27:30.572212 oemof.solph-0.5.1.dev1/docs/examples/
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)       85 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/docs/examples/index.rst
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     2410 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/docs/examples/solph.examples.rst
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      558 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/docs/index.rst
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)       27 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev1/docs/readme.rst
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-06-11 18:27:30.576212 oemof.solph-0.5.1.dev1/docs/reference/
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)       97 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev1/docs/reference/index.rst
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      141 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev1/docs/reference/oemof.solph.busses.rst
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     1903 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev1/docs/reference/oemof.solph.components.rst
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      161 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev1/docs/reference/oemof.solph.console_scripts.rst
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      370 2023-05-28 19:15:14.000000 oemof.solph-0.5.1.dev1/docs/reference/oemof.solph.constraints.rst
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      151 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev1/docs/reference/oemof.solph.energy_system.rst
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      729 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev1/docs/reference/oemof.solph.flow.rst
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      141 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev1/docs/reference/oemof.solph.groupings.rst
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      135 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev1/docs/reference/oemof.solph.helpers.rst
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      132 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev1/docs/reference/oemof.solph.models.rst
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      135 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev1/docs/reference/oemof.solph.options.rst
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      138 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev1/docs/reference/oemof.solph.plumbing.rst
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      143 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev1/docs/reference/oemof.solph.processing.rst
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      128 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev1/docs/reference/oemof.solph.views.rst
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)       51 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/docs/requirements.txt
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      109 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev1/docs/spelling_wordlist.txt
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    76835 2023-05-15 14:22:45.000000 oemof.solph-0.5.1.dev1/docs/usage.rst
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-06-11 18:27:30.580212 oemof.solph-0.5.1.dev1/docs/whatsnew/
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      100 2023-01-24 16:30:15.000000 oemof.solph-0.5.1.dev1/docs/whatsnew/v0-0-1.rst
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     2744 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/docs/whatsnew/v0-0-2.rst
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     1869 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/docs/whatsnew/v0-0-3.rst
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      900 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/docs/whatsnew/v0-0-4.rst
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     1781 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/docs/whatsnew/v0-0-5.rst
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     1145 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/docs/whatsnew/v0-0-6.rst
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      115 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/docs/whatsnew/v0-0-7.rst
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     2938 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/docs/whatsnew/v0-1-0.rst
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      446 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/docs/whatsnew/v0-1-1.rst
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     1852 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/docs/whatsnew/v0-1-2.rst
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      296 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/docs/whatsnew/v0-1-4.rst
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     8202 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/docs/whatsnew/v0-2-0.rst
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     3618 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/docs/whatsnew/v0-2-1.rst
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     3980 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/docs/whatsnew/v0-2-2.rst
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      390 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/docs/whatsnew/v0-2-3.rst
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     4258 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/docs/whatsnew/v0-3-0.rst
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      522 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/docs/whatsnew/v0-3-1.rst
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     1096 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/docs/whatsnew/v0-3-2.rst
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     3847 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/docs/whatsnew/v0-4-0.rst
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      506 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/docs/whatsnew/v0-4-1.rst
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      156 2023-01-24 16:30:15.000000 oemof.solph-0.5.1.dev1/docs/whatsnew/v0-4-2.rst
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     1634 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/docs/whatsnew/v0-4-4.rst
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     1051 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/docs/whatsnew/v0-4-5.rst
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     1876 2023-05-15 14:22:45.000000 oemof.solph-0.5.1.dev1/docs/whatsnew/v0-5-0.rst
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     2460 2023-06-02 14:48:15.000000 oemof.solph-0.5.1.dev1/docs/whatsnew/v0-5-1.rst
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-06-11 18:27:30.552212 oemof.solph-0.5.1.dev1/examples/
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-06-11 18:27:30.580212 oemof.solph-0.5.1.dev1/examples/basic_example/
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)   288296 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/examples/basic_example/basic_example.csv
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-06-11 18:27:30.580212 oemof.solph-0.5.1.dev1/examples/excel_reader/
+-rwxrwxr-x   0 patrik    (1001) patrik    (1001)   577434 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/examples/excel_reader/scenario.xlsx
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-06-11 18:27:30.580212 oemof.solph-0.5.1.dev1/examples/invest_nonconvex_flow_examples/
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     2995 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev1/examples/invest_nonconvex_flow_examples/solar_generation.csv
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-06-11 18:27:30.580212 oemof.solph-0.5.1.dev1/examples/simple_dispatch/
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)   401132 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/examples/simple_dispatch/input_data.csv
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-06-11 18:27:30.584212 oemof.solph-0.5.1.dev1/examples/storage_investment/
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)   288296 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/examples/storage_investment/storage_investment.csv
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-06-11 18:27:30.584212 oemof.solph-0.5.1.dev1/examples/tuple_as_labels/
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)   288296 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/examples/tuple_as_labels/tuple_as_label.csv
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-06-11 18:27:30.584212 oemof.solph-0.5.1.dev1/examples/variable_chp/
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     6335 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/examples/variable_chp/variable_chp.csv
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      322 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev1/pyproject.toml
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      945 2023-06-11 18:27:30.616211 oemof.solph-0.5.1.dev1/setup.cfg
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     3100 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/setup.py
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-06-11 18:27:30.552212 oemof.solph-0.5.1.dev1/src/
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-06-11 18:27:30.552212 oemof.solph-0.5.1.dev1/src/oemof/
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-06-11 18:27:30.588212 oemof.solph-0.5.1.dev1/src/oemof/solph/
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      818 2023-05-04 19:13:57.000000 oemof.solph-0.5.1.dev1/src/oemof/solph/__init__.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     1832 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev1/src/oemof/solph/_console_scripts.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     9146 2023-06-02 14:48:15.000000 oemof.solph-0.5.1.dev1/src/oemof/solph/_energy_system.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     3655 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/src/oemof/solph/_groupings.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     1222 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/src/oemof/solph/_helpers.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    17457 2023-05-15 14:22:45.000000 oemof.solph-0.5.1.dev1/src/oemof/solph/_models.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    11190 2023-05-15 14:22:45.000000 oemof.solph-0.5.1.dev1/src/oemof/solph/_options.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     2091 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/src/oemof/solph/_plumbing.py
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-06-11 18:27:30.588212 oemof.solph-0.5.1.dev1/src/oemof/solph/buses/
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      445 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev1/src/oemof/solph/buses/__init__.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     3946 2023-05-15 14:22:45.000000 oemof.solph-0.5.1.dev1/src/oemof/solph/buses/_bus.py
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-06-11 18:27:30.588212 oemof.solph-0.5.1.dev1/src/oemof/solph/buses/experimental/
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      385 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev1/src/oemof/solph/buses/experimental/__init__.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     1606 2023-05-15 14:22:45.000000 oemof.solph-0.5.1.dev1/src/oemof/solph/buses/experimental/_electrical_bus.py
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-06-11 18:27:30.588212 oemof.solph-0.5.1.dev1/src/oemof/solph/components/
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      835 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev1/src/oemof/solph/components/__init__.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    10279 2023-05-15 14:22:45.000000 oemof.solph-0.5.1.dev1/src/oemof/solph/components/_extraction_turbine_chp.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    18787 2023-05-15 14:22:45.000000 oemof.solph-0.5.1.dev1/src/oemof/solph/components/_generic_chp.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    63996 2023-06-02 14:48:15.000000 oemof.solph-0.5.1.dev1/src/oemof/solph/components/_generic_storage.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     6395 2023-05-15 14:22:45.000000 oemof.solph-0.5.1.dev1/src/oemof/solph/components/_offset_transformer.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     1854 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/src/oemof/solph/components/_sink.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     2046 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/src/oemof/solph/components/_source.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     8686 2023-05-15 14:22:45.000000 oemof.solph-0.5.1.dev1/src/oemof/solph/components/_transformer.py
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-06-11 18:27:30.588212 oemof.solph-0.5.1.dev1/src/oemof/solph/components/experimental/
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      565 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev1/src/oemof/solph/components/experimental/__init__.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    25084 2023-05-15 14:22:45.000000 oemof.solph-0.5.1.dev1/src/oemof/solph/components/experimental/_generic_caes.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     5762 2023-05-15 14:22:45.000000 oemof.solph-0.5.1.dev1/src/oemof/solph/components/experimental/_link.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     6474 2023-05-15 14:22:45.000000 oemof.solph-0.5.1.dev1/src/oemof/solph/components/experimental/_piecewise_linear_transformer.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)   218756 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/src/oemof/solph/components/experimental/_sink_dsm.py
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-06-11 18:27:30.592212 oemof.solph-0.5.1.dev1/src/oemof/solph/constraints/
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     1257 2023-05-28 19:15:14.000000 oemof.solph-0.5.1.dev1/src/oemof/solph/constraints/__init__.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     2887 2023-05-15 14:22:45.000000 oemof.solph-0.5.1.dev1/src/oemof/solph/constraints/equate_flows.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     5648 2023-05-15 14:22:45.000000 oemof.solph-0.5.1.dev1/src/oemof/solph/constraints/equate_variables.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     4451 2023-05-15 14:22:45.000000 oemof.solph-0.5.1.dev1/src/oemof/solph/constraints/flow_count_limit.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     8238 2023-05-15 14:22:45.000000 oemof.solph-0.5.1.dev1/src/oemof/solph/constraints/integral_limit.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     8047 2023-05-15 14:22:45.000000 oemof.solph-0.5.1.dev1/src/oemof/solph/constraints/investment_limit.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     3496 2023-05-15 14:22:45.000000 oemof.solph-0.5.1.dev1/src/oemof/solph/constraints/shared_limit.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     5334 2023-05-28 19:15:14.000000 oemof.solph-0.5.1.dev1/src/oemof/solph/constraints/storage_level.py
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-06-11 18:27:30.592212 oemof.solph-0.5.1.dev1/src/oemof/solph/flows/
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      508 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev1/src/oemof/solph/flows/__init__.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    12045 2023-06-02 14:48:15.000000 oemof.solph-0.5.1.dev1/src/oemof/solph/flows/_flow.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    11399 2023-05-15 14:22:45.000000 oemof.solph-0.5.1.dev1/src/oemof/solph/flows/_invest_non_convex_flow_block.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    34141 2023-05-15 14:22:45.000000 oemof.solph-0.5.1.dev1/src/oemof/solph/flows/_investment_flow_block.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    29671 2023-05-15 14:22:45.000000 oemof.solph-0.5.1.dev1/src/oemof/solph/flows/_non_convex_flow_block.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    19557 2023-05-15 14:22:45.000000 oemof.solph-0.5.1.dev1/src/oemof/solph/flows/_simple_flow_block.py
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-06-11 18:27:30.592212 oemof.solph-0.5.1.dev1/src/oemof/solph/flows/experimental/
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      388 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev1/src/oemof/solph/flows/experimental/__init__.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     6929 2023-05-15 14:22:45.000000 oemof.solph-0.5.1.dev1/src/oemof/solph/flows/experimental/_electrical_line.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     1777 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/src/oemof/solph/helpers.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    22046 2023-05-15 14:22:45.000000 oemof.solph-0.5.1.dev1/src/oemof/solph/processing.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    13938 2023-05-15 14:22:45.000000 oemof.solph-0.5.1.dev1/src/oemof/solph/views.py
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-06-11 18:27:30.584212 oemof.solph-0.5.1.dev1/src/oemof.solph.egg-info/
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    13182 2023-06-11 18:27:30.000000 oemof.solph-0.5.1.dev1/src/oemof.solph.egg-info/PKG-INFO
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    13909 2023-06-11 18:27:30.000000 oemof.solph-0.5.1.dev1/src/oemof.solph.egg-info/SOURCES.txt
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)        1 2023-06-11 18:27:30.000000 oemof.solph-0.5.1.dev1/src/oemof.solph.egg-info/dependency_links.txt
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)       98 2023-06-11 18:27:30.000000 oemof.solph-0.5.1.dev1/src/oemof.solph.egg-info/entry_points.txt
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)        1 2022-10-04 09:53:33.000000 oemof.solph-0.5.1.dev1/src/oemof.solph.egg-info/not-zip-safe
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      208 2023-06-11 18:27:30.000000 oemof.solph-0.5.1.dev1/src/oemof.solph.egg-info/requires.txt
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)        6 2023-06-11 18:27:30.000000 oemof.solph-0.5.1.dev1/src/oemof.solph.egg-info/top_level.txt
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-06-11 18:27:30.596212 oemof.solph-0.5.1.dev1/tests/
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    69026 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/constraint_tests.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     2457 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/tests/flow_tests.py
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-06-11 18:27:30.608211 oemof.solph-0.5.1.dev1/tests/lp_files/
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     3372 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/activity_costs.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     6792 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/activity_costs_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     6532 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/connect_investment.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    23150 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/connect_investment_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     5306 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/dsm_module_DIW.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     6089 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/dsm_module_DIW_extended.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    15070 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/dsm_module_DIW_extended_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     7607 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/dsm_module_DIW_invest.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    21666 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/dsm_module_DIW_invest_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    13295 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/dsm_module_DIW_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    12721 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/dsm_module_DLR.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    12603 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/dsm_module_DLR_delay_time.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    11806 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/dsm_module_DLR_extended.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    27864 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/dsm_module_DLR_extended_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    16526 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/dsm_module_DLR_invest.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    37082 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/dsm_module_DLR_invest_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    25833 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/dsm_module_DLR_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     3178 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/dsm_module_oemof.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     3145 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/dsm_module_oemof_extended.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     6661 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/dsm_module_oemof_extended_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     4252 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/dsm_module_oemof_invest.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    12173 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/dsm_module_oemof_invest_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     6595 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/dsm_module_oemof_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     1207 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/emission_budget_limit.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     1305 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/emission_limit.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      939 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/emission_limit_no_error.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     1283 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/equate_flows.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     3607 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/fixed_costs_sources.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     1673 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/fixed_source_invest_sink.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     5995 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/fixed_source_invest_sink_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      596 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/fixed_source_variable_sink.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     1181 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/fixed_source_variable_sink_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     7826 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/flow_count_limit.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    14066 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/flow_count_limit_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     2860 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/flow_invest_with_offset.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     9841 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/flow_invest_with_offset_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     2784 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/flow_invest_with_offset_no_minimum.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     9613 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/flow_invest_with_offset_no_minimum_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     2708 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/flow_invest_without_offset.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     9328 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/flow_invest_without_offset_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     7392 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/flow_nonconvex_invest_bounded_transformer.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     1341 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/flow_reaching_lifetime.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     1567 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/flow_reaching_lifetime_initial_age.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     3103 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/generic_invest_limit.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     3518 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/inactivity_costs.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     7051 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/inactivity_costs_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     1450 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/integer_source.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     3900 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/invest_non_convex_flow.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     1321 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/invest_source_fixed_sink.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     5130 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/invest_source_fixed_sink_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     6577 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/investment_limit.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     8411 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/investment_limit_with_dsm_DIW.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    12526 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/investment_limit_with_dsm_DLR.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     5766 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/investment_limit_with_dsm_oemof.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     1406 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/linear_transformer.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     2393 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/linear_transformer_chp.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     3318 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/linear_transformer_chp_invest.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     9471 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/linear_transformer_chp_invest_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     4777 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/linear_transformer_chp_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     2292 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/linear_transformer_invest.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     8022 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/linear_transformer_invest_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     8083 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/linear_transformer_invest_multi_period_old.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     2803 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/linear_transformer_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     1627 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/link.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      843 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/max_source_min_sink.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     1714 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/max_source_min_sink_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     4865 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/maximum_shutdowns.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     9690 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/maximum_shutdowns_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     4783 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/maximum_startups.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     9527 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/maximum_startups_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     7455 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/min_max_runtime.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    15159 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/min_max_runtime_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      481 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/nominal_value_to_zero.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      841 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/nominal_value_to_zero_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     6473 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/nonequidistant_timeindex.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     3317 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/offsettransformer.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     6506 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/offsettransformer_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     1280 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/periodical_emission_limit.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    23238 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/periodical_investment_limit.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    25743 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/periodical_investment_limit_with_dsm_DIW.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    30977 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/periodical_investment_limit_with_dsm_DLR.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    17747 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/periodical_investment_limit_with_dsm_oemof.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    13503 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/piecewise_linear_transformer_cc.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    26996 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/piecewise_linear_transformer_cc_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    14121 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/piecewise_linear_transformer_dcc.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    28232 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/piecewise_linear_transformer_dcc_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     3644 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/shared_limit.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     6733 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/shared_limit_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     2295 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/source_with_gradient.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     4739 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/source_with_gradient_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     4903 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/source_with_nonconvex_gradient.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    10188 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/source_with_nonconvex_gradient_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     2334 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/storage.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     2346 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/storage_fixed_losses.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     4674 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/storage_fixed_losses_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     5952 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/storage_invest_1.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     6124 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/storage_invest_1_fixed_losses.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    19591 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/storage_invest_1_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     4789 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/storage_invest_2.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    16467 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/storage_invest_2_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     3542 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/storage_invest_3.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    12368 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/storage_invest_3_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     3075 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/storage_invest_4.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     7569 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/storage_invest_4_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     3664 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/storage_invest_5.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    12614 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/storage_invest_5_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     4926 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/storage_invest_6.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    16794 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/storage_invest_6_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     7237 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/storage_invest_all_nonconvex.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    23916 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/storage_invest_all_nonconvex_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     3086 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/storage_invest_minimum.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     7537 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/storage_invest_minimum_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     8103 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/storage_invest_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     4861 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/storage_invest_unbalanced.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     7600 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/storage_invest_with_offset.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    24169 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/storage_invest_with_offset_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     7529 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/storage_invest_without_offset.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    23923 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/storage_invest_without_offset_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     4003 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/storage_level_constraint.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     4644 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/storage_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     1730 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/storage_unbalanced.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     3277 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/storage_unbalanced_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      937 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/summed_min_source.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     1709 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/summed_min_source_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     4304 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/transformer.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     5166 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/transformer_invest.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    13614 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/transformer_invest_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     5168 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/transformer_invest_with_existing.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    13685 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/transformer_invest_with_existing_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     8659 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/transformer_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     4600 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/variable_chp.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     9079 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/lp_files/variable_chp_multi_period.lp
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    71320 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/multi_period_constraint_tests.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      899 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev1/tests/regression_tests.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     9979 2023-06-02 14:48:15.000000 oemof.solph-0.5.1.dev1/tests/test_components.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      493 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev1/tests/test_console_scripts.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     2051 2023-05-15 19:57:50.000000 oemof.solph-0.5.1.dev1/tests/test_constraints_module.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     1622 2023-05-15 14:22:45.000000 oemof.solph-0.5.1.dev1/tests/test_energy_system.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     2172 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/tests/test_grouping.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      434 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev1/tests/test_helpers.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     2932 2023-05-15 14:22:45.000000 oemof.solph-0.5.1.dev1/tests/test_models.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     8094 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev1/tests/test_non_equidistant_time_index.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      189 2023-02-22 20:48:11.000000 oemof.solph-0.5.1.dev1/tests/test_oemof_installation_test.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      616 2023-05-15 14:22:45.000000 oemof.solph-0.5.1.dev1/tests/test_options.py
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-06-11 18:27:30.608211 oemof.solph-0.5.1.dev1/tests/test_outputlib/
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     3500 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev1/tests/test_outputlib/__init__.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     5522 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev1/tests/test_outputlib/input_data.csv
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     2179 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/tests/test_outputlib/test_views.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    12619 2023-05-15 14:22:45.000000 oemof.solph-0.5.1.dev1/tests/test_processing.py
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-06-11 18:27:30.552212 oemof.solph-0.5.1.dev1/tests/test_scripts/
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-06-11 18:27:30.552212 oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-06-11 18:27:30.608211 oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_connect_invest/
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     5179 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_connect_invest/connect_invest.csv
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     4396 2023-05-15 14:22:45.000000 oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_connect_invest/test_connect_invest.py
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-06-11 18:27:30.608211 oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_flexible_modelling/
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     4294 2023-05-15 14:22:45.000000 oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_flexible_modelling/test_add_constraints.py
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-06-11 18:27:30.608211 oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_generic_caes/
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     3871 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_generic_caes/generic_caes.csv
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     4398 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_generic_caes/test_generic_caes.py
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-06-11 18:27:30.612211 oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_generic_chp/
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    10281 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_generic_chp/ccet.csv
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     3485 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_generic_chp/test_generic_chp.py
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-06-11 18:27:30.612211 oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_invest_fix_flow/
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      100 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_invest_fix_flow/input_data.csv
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     2987 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_invest_fix_flow/test_simple_invest_fixed.py
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-06-11 18:27:30.612211 oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_lopf/
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     3918 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_lopf/test_lopf.py
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-06-11 18:27:30.612211 oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_multi_period_model/
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     8612 2023-05-15 14:22:45.000000 oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_multi_period_model/test_multi_period_dispatch_model.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    12592 2023-05-15 14:22:45.000000 oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_multi_period_model/test_multi_period_investment_model.py
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-06-11 18:27:30.612211 oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_options/
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     1126 2023-02-10 10:19:17.000000 oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_options/test_non_convex.py
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-06-11 18:27:30.612211 oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_piecewiselineartransformer/
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     3315 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_piecewiselineartransformer/test_piecewiselineartransformer.py
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-06-11 18:27:30.612211 oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_simple_model/
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     5522 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_simple_model/input_data.csv
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     5821 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_simple_model/test_simple_dispatch.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     3640 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_simple_model/test_simple_dispatch_one.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     3640 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_simple_model/test_simple_dispatch_one_explicit_timemode.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     6412 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_simple_model/test_simple_invest.py
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-06-11 18:27:30.612211 oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_storage_investment/
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    15331 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_storage_investment/storage_investment.csv
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     2868 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_storage_investment/test_invest_storage_regression.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     6607 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_storage_investment/test_storage_investment.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     7115 2023-06-11 18:25:39.000000 oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_storage_investment/test_storage_with_tuple_label.py
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-06-11 18:27:30.612211 oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_variable_chp/
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     6542 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_variable_chp/test_variable_chp.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      193 2022-10-04 09:26:46.000000 oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_variable_chp/variable_chp.csv
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     5154 2023-06-02 14:48:15.000000 oemof.solph-0.5.1.dev1/tests/test_solph_network_classes.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     5750 2023-02-03 19:01:41.000000 oemof.solph-0.5.1.dev1/tests/test_time_index.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     5307 2023-02-17 18:33:53.000000 oemof.solph-0.5.1.dev1/tests/test_warnings.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     2180 2023-05-28 19:31:23.000000 oemof.solph-0.5.1.dev1/tox.ini
```

### Comparing `oemof.solph-0.5.1.dev0/.bumpversion.cfg` & `oemof.solph-0.5.1.dev1/.bumpversion.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.5.1.dev0
+current_version = 0.5.1.dev1
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
```

### Comparing `oemof.solph-0.5.1.dev0/.cookiecutterrc` & `oemof.solph-0.5.1.dev1/.cookiecutterrc`

 * *Files 4% similar despite different names*

```diff
@@ -59,11 +59,11 @@
     sphinx_doctest:            'no'
     sphinx_theme:              'sphinx-rtd-theme'
     test_matrix_configurator:  'yes'
     test_matrix_separate_coverage: 'no'
     test_runner:               'pytest'
     travis:                    'yes'
     travis_osx:                'yes'
-    version:                   '0.4.0.dev0'
+    version:                   '0.4.0.dev1'
     website:                   'https://oemof.org'
     year_from:                 '2014'
     year_to:                   '2020'
```

### Comparing `oemof.solph-0.5.1.dev0/AUTHORS.rst` & `oemof.solph-0.5.1.dev1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/CITATION.cff` & `oemof.solph-0.5.1.dev1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/CODE_OF_CONDUCT.md` & `oemof.solph-0.5.1.dev1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/CONTRIBUTING.rst` & `oemof.solph-0.5.1.dev1/CONTRIBUTING.rst`

 * *Files 9% similar despite different names*

```diff
@@ -71,16 +71,16 @@
 For merging, you should:
 
 1. Include passing tests (run ``tox``) [1]_.
 2. Update documentation when there's new API, functionality etc.
 3. Add a note about the changes to ``docs/whatsnew/next_version.rst``.
 4. Add your name to ``AUTHORS.rst`` and ``CITATION.cff``.
 
-.. [1] If you don't have all the necessary python versions available locally you can rely on Travis - it will
-       `run the tests <https://travis-ci.org/oemof/oemof-solph/pull_requests>`_ for each change you add in the pull request.
+.. [1] If you don't have all the necessary python versions available locally,
+       you can rely on the CI pipeline at GitHub.
 
        It will be slower though ...
 
 
 Tests
 -----
```

### Comparing `oemof.solph-0.5.1.dev0/LICENSE` & `oemof.solph-0.5.1.dev1/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 MIT License
 
-Copyright (c) 2014-2022, oemof developer group
+Copyright (c) 2014-2023, oemof developer group
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `oemof.solph-0.5.1.dev0/PKG-INFO` & `oemof.solph-0.5.1.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oemof.solph
-Version: 0.5.1.dev0
+Version: 0.5.1.dev1
 Summary: A model generator for energy system modelling and optimisation.
 Home-page: https://oemof.org
 Author: oemof developer group
 Author-email: contact@oemof.org
 License: MIT
 Project-URL: Documentation, https://oemof-solph.readthedocs.io/
 Project-URL: Changelog, https://oemof-solph.readthedocs.io/en/latest/changelog.html
@@ -297,15 +297,15 @@
 The repository has sections for each major release.
 
 You are welcome to contribute your own examples via a `pull request <https://github.com/oemof/oemof-examples/pulls>`_ or by sending us an e-mail (see `here <https://oemof.org/contact/>`_ for contact information).
 
 License
 =======
 
-Copyright (c) 2022 oemof developer group
+Copyright (c) 2023 oemof developer group
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `oemof.solph-0.5.1.dev0/README.rst` & `oemof.solph-0.5.1.dev1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -262,15 +262,15 @@
 The repository has sections for each major release.
 
 You are welcome to contribute your own examples via a `pull request <https://github.com/oemof/oemof-examples/pulls>`_ or by sending us an e-mail (see `here <https://oemof.org/contact/>`_ for contact information).
 
 License
 =======
 
-Copyright (c) 2022 oemof developer group
+Copyright (c) 2023 oemof developer group
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `oemof.solph-0.5.1.dev0/ci/appveyor-with-compiler.cmd` & `oemof.solph-0.5.1.dev1/ci/appveyor-with-compiler.cmd`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/ci/bootstrap.py` & `oemof.solph-0.5.1.dev1/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/ci/templates/.appveyor.yml` & `oemof.solph-0.5.1.dev1/ci/templates/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/ci/templates/.travis.yml` & `oemof.solph-0.5.1.dev1/ci/templates/.travis.yml`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/ci/templates/tox.ini` & `oemof.solph-0.5.1.dev1/ci/templates/tox.ini`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/docs/_files/ExtractionTurbine_range_of_operation.svg` & `oemof.solph-0.5.1.dev1/docs/_files/ExtractionTurbine_range_of_operation.svg`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/docs/_files/GenericCHP.svg` & `oemof.solph-0.5.1.dev1/docs/_files/GenericCHP.svg`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/docs/_files/OffsetTransformer_efficiency.svg` & `oemof.solph-0.5.1.dev1/docs/_files/OffsetTransformer_efficiency.svg`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/docs/_files/OffsetTransformer_power_relation.svg` & `oemof.solph-0.5.1.dev1/docs/_files/OffsetTransformer_power_relation.svg`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/docs/_files/Plot_delay_2013-01-01.svg` & `oemof.solph-0.5.1.dev1/docs/_files/Plot_delay_2013-01-01.svg`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/docs/_files/diesel_genset_investment_flow.svg` & `oemof.solph-0.5.1.dev1/docs/_files/diesel_genset_investment_flow.svg`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/docs/_files/diesel_genset_nonconvex_flow.svg` & `oemof.solph-0.5.1.dev1/docs/_files/diesel_genset_nonconvex_flow.svg`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/docs/_files/diesel_genset_nonconvex_invest_flow.svg` & `oemof.solph-0.5.1.dev1/docs/_files/diesel_genset_nonconvex_invest_flow.svg`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/docs/_files/example_figures.png` & `oemof.solph-0.5.1.dev1/docs/_files/example_figures.png`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/docs/_files/example_network.svg` & `oemof.solph-0.5.1.dev1/docs/_files/example_network.svg`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/docs/_files/example_variable_chp.svg` & `oemof.solph-0.5.1.dev1/docs/_files/example_variable_chp.svg`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/docs/_files/framework_concept.svg` & `oemof.solph-0.5.1.dev1/docs/_files/framework_concept.svg`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/docs/_files/nonconvex_invest_investcosts_power.svg` & `oemof.solph-0.5.1.dev1/docs/_files/nonconvex_invest_investcosts_power.svg`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/docs/_files/nonconvex_invest_specific_costs.svg` & `oemof.solph-0.5.1.dev1/docs/_files/nonconvex_invest_specific_costs.svg`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/docs/_files/oemof_solph_example.svg` & `oemof.solph-0.5.1.dev1/docs/_files/oemof_solph_example.svg`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/docs/_files/variable_chp_plot.svg` & `oemof.solph-0.5.1.dev1/docs/_files/variable_chp_plot.svg`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/docs/_logo/README.rst` & `oemof.solph-0.5.1.dev1/docs/_logo/README.rst`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/docs/_logo/editable_fonts/logo_oemof_solph_COMPACT_editable_fonts.svg` & `oemof.solph-0.5.1.dev1/docs/_logo/editable_fonts/logo_oemof_solph_COMPACT_editable_fonts.svg`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/docs/_logo/editable_fonts/logo_oemof_solph_FULL_editable_fonts.svg` & `oemof.solph-0.5.1.dev1/docs/_logo/editable_fonts/logo_oemof_solph_FULL_editable_fonts.svg`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/docs/_logo/editable_fonts/logo_oemof_solph_ICON_editable_fonts.svg` & `oemof.solph-0.5.1.dev1/docs/_logo/editable_fonts/logo_oemof_solph_ICON_editable_fonts.svg`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/docs/_logo/editable_fonts/logo_oemof_solph_NOTEXT_editable_fonts.svg` & `oemof.solph-0.5.1.dev1/docs/_logo/editable_fonts/logo_oemof_solph_NOTEXT_editable_fonts.svg`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/docs/_logo/logo_oemof_solph_COMPACT.svg` & `oemof.solph-0.5.1.dev1/docs/_logo/logo_oemof_solph_COMPACT.svg`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/docs/_logo/logo_oemof_solph_COMPACT_bg.svg` & `oemof.solph-0.5.1.dev1/docs/_logo/logo_oemof_solph_COMPACT_bg.svg`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/docs/_logo/logo_oemof_solph_FULL.svg` & `oemof.solph-0.5.1.dev1/docs/_logo/logo_oemof_solph_FULL.svg`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/docs/_logo/logo_oemof_solph_ICON.svg` & `oemof.solph-0.5.1.dev1/docs/_logo/logo_oemof_solph_ICON.svg`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/docs/_logo/logo_oemof_solph_NOTEXT.svg` & `oemof.solph-0.5.1.dev1/docs/_logo/logo_oemof_solph_NOTEXT.svg`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/docs/changelog.rst` & `oemof.solph-0.5.1.dev1/docs/changelog.rst`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 .. contents:: `Releases`
     :depth: 1
     :local:
     :backlinks: top
 
 
+.. include::  whatsnew/v0-5-0.rst
 .. include::  whatsnew/v0-4-5.rst
 .. include::  whatsnew/v0-4-4.rst
 .. include::  whatsnew/v0-4-2.rst
 .. include::  whatsnew/v0-4-1.rst
 .. include::  whatsnew/v0-4-0.rst
 .. include::  whatsnew/v0-3-2.rst
 .. include::  whatsnew/v0-3-1.rst
```

### Comparing `oemof.solph-0.5.1.dev0/docs/conf.py` & `oemof.solph-0.5.1.dev1/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,18 +27,18 @@
     "sphinx.ext.napoleon",
     "sphinx.ext.todo",
     "sphinx.ext.viewcode",
 ]
 source_suffix = ".rst"
 master_doc = "index"
 project = "oemof.solph"
-year = "2014-2022"
+year = "2014-2023"
 author = "oemof-developer-group"
 copyright = "{0}, {1}".format(year, author)
-version = release = "0.5.1.dev0"
+version = release = "0.5.1.dev1"
 
 pygments_style = "trac"
 templates_path = ["."]
 extlinks = {
     "issue": ("https://github.com/oemof/oemof-solph/issues/%s", "#%s"),
     "pr": ("https://github.com/oemof/oemof-solph/pull/%s", "PR #%s"),
 }
```

### Comparing `oemof.solph-0.5.1.dev0/docs/examples/solph.examples.rst` & `oemof.solph-0.5.1.dev1/docs/examples/solph.examples.rst`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/docs/index.rst` & `oemof.solph-0.5.1.dev1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/docs/reference/oemof.solph.components.rst` & `oemof.solph-0.5.1.dev1/docs/reference/oemof.solph.components.rst`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/docs/reference/oemof.solph.flow.rst` & `oemof.solph-0.5.1.dev1/docs/reference/oemof.solph.flow.rst`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/docs/usage.rst` & `oemof.solph-0.5.1.dev1/docs/usage.rst`

 * *Files 10% similar despite different names*

```diff
@@ -6,54 +6,54 @@
 User's guide
 ~~~~~~~~~~~~
 
 Solph is an oemof-package, designed to create and solve linear or mixed-integer linear optimization problems. The package is based on pyomo. To create an energy system model generic and specific components are available. To get started with solph, checkout the examples in the :ref:`solph_examples_label` section.
 
 This User's guide provides a user-friendly introduction into oemof-solph,
 which includes small examples and nice illustrations.
-However, the functionality of oemof-solph go beyond the content of this User's guide section.
+However, the functionalities of oemof-solph go beyond the content of this User's guide section.
 So, if you want to know all details of a certain component or a function,
 please go the :ref:`api_reference_label`. There, you will find
 a detailed and complete description of all oemof-solph modules.
 
 .. contents::
     :depth: 2
     :local:
     :backlinks: top
 
 
 How can I use solph?
 --------------------
 
-To use solph you have to install oemof and at least one solver (see :ref:`installation_label`), which can be used together with pyomo (e.g. CBC, GLPK, Gurobi, Cplex). See the `pyomo installation guide <https://pyomo.readthedocs.io/en/stable/solving_pyomo_models.html#supported-solvers>`_ for all supported solver.
+To use solph you have to install oemof.solph and at least one solver (see :ref:`installation_label`), which can be used together with pyomo (e.g. CBC, GLPK, Gurobi, Cplex). See the `pyomo installation guide <https://pyomo.readthedocs.io/en/stable/solving_pyomo_models.html#supported-solvers>`_ for all supported solvers.
 You can test it by executing one of the existing examples (see :ref:`solph_examples_label`, or directly `oemof's example repository <https://github.com/oemof/oemof-examples>`__). Be aware that the examples require the CBC solver but you can change the solver name in the example files to your solver.
 
-Once the example work you are close to your first energy model.
+Once the examples work you are close to your first energy model.
 
 
 Handling of Warnings
 ^^^^^^^^^^^^^^^^^^^^
 
 The solph library is designed to be as generic as possible to make it possible
 to use it in different use cases. This concept makes it difficult to raise
-Error or Warnings because sometimes untypical combinations of parameters are
+Errors or Warnings because sometimes untypical combinations of parameters are
 allowed even though they might be wrong in over 99% of the use cases.
 
 Therefore, a SuspiciousUsageWarning was introduced. This warning will warn you
 if you do something untypical. If you are sure that you know what you are doing
 you can switch the warning off.
 
 See `the debugging module of oemof-tools <https://oemof-tools.readthedocs.io/en/latest/usage.html#debugging>`_ for more
 information.
 
 
 Set up an energy system
 ^^^^^^^^^^^^^^^^^^^^^^^
 
-In most cases an EnergySystem object is defined when we start to build up an energy system model. The EnergySystem object will be the main container for the model.
+In most cases an EnergySystem object is defined when we start to build up an energy system model. The EnergySystem object will be the main container for the model's elements.
 
 The model time is defined by the number of intervals and the length of intervals. The length of each interval does not have to be the same. This can be defined in two ways:
 
 1. Define the length of each interval in an array/Series where the number of the elements is the number of intervals.
 2. Define a `pandas.DatetimeIndex` with all time steps that encloses an interval. Be aware that you have to define n+1 time points to get n intervals. For non-leap year with hourly values that means 8761 time points to get 8760 interval e.g. 2018-01-01 00:00 to 2019-01-01 00:00.
 
 The index will also be used for the results. For a numeric index the resulting time series will indexed with a numeric index starting with 0.
@@ -84,15 +84,15 @@
 
 Now you can start to add the components of the network.
 
 
 Add components to the energy system
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-After defining an instance of the EnergySystem class you have to add all nodes you define in the following to your EnergySystem.
+After defining an instance of the EnergySystem class, in the following you have to add all nodes you define  to your EnergySystem.
 
 Basically, there are two types of *nodes* - *components* and *buses*. Every Component has to be connected with one or more *buses*. The connection between a *component* and a *bus* is the *flow*.
 
 All solph *components* can be used to set up an energy system model but you should read the documentation of each *component* to learn about usage and restrictions. For example it is not possible to combine every *component* with every *flow*. Furthermore, you can add your own *components* in your application (see below) but we would be pleased to integrate them into solph if they are of general interest (see :ref:`feature_requests_and_feedback`).
 
 An example of a simple energy system shows the usage of the nodes for
 real world representations:
@@ -129,61 +129,64 @@
     # add a dictionary
     my_energysystem.add(*my_dictionary.values())
 
 
 Bus
 +++
 
-All flows into and out of a *bus* are balanced. Therefore an instance of the Bus class represents a grid or network without losses. To define an instance of a Bus only a unique label is necessary. If you do not set a label a random label is used but this makes it difficult to get the results later on.
+All flows into and out of a *bus* are balanced (by default). Therefore an instance of the Bus class represents a grid or network without losses. To define an instance of a Bus only a unique label is necessary. If you do not set a label a random label is used but this makes it difficult to get the results later on.
 
 To make it easier to connect the bus to a component you can optionally assign a variable for later use.
 
 .. code-block:: python
 
     solph.buses.Bus(label='natural_gas')
     electricity_bus = solph.buses.Bus(label='electricity')
 
-.. note:: See the :py:class:`~oemof.solph.network.bus.Bus` class for all parameters and the mathematical background.
+.. note:: See the :py:class:`~oemof.solph.buses._bus.Bus` class for all parameters and the mathematical background.
 
 
 Flow
 ++++
 
-The flow class has to be used to connect. An instance of the Flow class is normally used in combination with the definition of a component.
+The flow class has to be used to connect nodes and buses. An instance of the Flow class is normally used in combination with the definition of a component.
 A Flow can be limited by upper and lower bounds (constant or time-dependent) or by summarised limits.
-For all parameters see the API documentation of the :py:class:`~oemof.solph.network.flow.Flow` class or the examples of the nodes below. A basic flow can be defined without any parameter.
+For all parameters see the API documentation of the :py:class:`~oemof.solph.flows._flow.Flow` class or the examples of the nodes below. A basic flow can be defined without any parameter.
 
 .. code-block:: python
 
     solph.flows.Flow()
 
 Oemof has different types of *flows* but you should be aware that you cannot connect every *flow* type with every *component*.
 
-.. note:: See the :py:class:`~oemof.solph.network.flow.Flow` class for all parameters and the mathematical background.
+.. note:: See the :py:class:`~oemof.solph.flows._flow.Flow` class for all parameters and the mathematical background.
 
 Components
 ++++++++++
 
-Components can be classified into three categories. Basic components, detailed components, and experimental components. The experimental section was created to lower the entry barrier for new components. Be aware that these components might not be properly documented or even sometimes do not even work as intended. Let us know if you have used and tested these components. This is the first step to remove the experimental disclaimer.
+Components are divided in two categories. Well-tested components (solph.components) and experimental components (solph.components.experimental). The experimental section was created to lower the entry barrier for new components. Be aware that these components might not be properly documented or even sometimes do not even work as intended. Let us know if you have successfully used and tested these components. This is the first step to move them to the regular components section.
 
 See :ref:`oemof_solph_components_label` for a list of all components.
 
 
 .. _oemof_solph_optimise_es_label:
 
 Optimise your energy system
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 The typical optimisation of an energy system in solph is the dispatch optimisation, which means that the use of the sources is optimised to satisfy the demand at least costs.
 Therefore, variable cost can be defined for all components. The cost for gas should be defined in the gas source while the variable costs of the gas power plant are caused by operating material.
+The actual fuel cost in turn is calculated in the framework itself considering the efficiency of the power plant.
 You can deviate from this scheme but you should keep it consistent to make it understandable for others.
 
 Costs do not have to be monetary costs but could be emissions or other variable units.
 
-Furthermore, it is possible to optimise the capacity of different components (see :ref:`investment_mode_label`).
+Furthermore, it is possible to optimise the capacity of different components using the investment mode (see :ref:`investment_mode_label`).
+
+Since v0.5.1, there also is the possibility to have multi-period (i.e. dynamic) investments over longer-time horizon which is in experimental state (see :ref:`multi_period_mode_label`).
 
 .. code-block:: python
 
     # set up a simple least cost optimisation
     om = solph.Model(my_energysystem)
 
     # solve the energy model using the CBC solver
@@ -198,15 +201,15 @@
 
     # write the lp file for debugging or other reasons
     om.write('path/my_model.lp', io_options={'symbolic_solver_labels': True})
 
 Analysing your results
 ^^^^^^^^^^^^^^^^^^^^^^
 
-If you want to analyse your results, you should first dump your EnergySystem instance, otherwise you have to run the simulation again.
+If you want to analyse your results, you should first dump your EnergySystem instance to permanently store results. Otherwise you would have to run the simulation again.
 
 .. code-block:: python
 
     my_energysystem.results = processing.results(om)
     my_energysystem.dump('my_path', 'my_dump.oemof')
 
 If you need the meta results of the solver you can do the following:
@@ -864,29 +867,37 @@
 
 .. _investment_mode_label:
 
 Investment optimisation
 -------------------------
 
 As described in :ref:`oemof_solph_optimise_es_label` the typical way to optimise an energy system is the dispatch optimisation based on marginal costs. Solph also provides a combined dispatch and investment optimisation.
-Based on investment costs you can compare the usage of existing components against building up new capacity.
-The annual savings by building up new capacity must therefore compensate the annuity of the investment costs (the time period does not have to be one year but depends on your Datetime index).
+This standard investment mode is limited to one period where all investments happen at the start of the optimization time frame. If you want to optimize longer-term horizons and allow investments at the beginning
+of each of multiple periods, also taking into account units lifetimes, you can try the :ref:`multi_period_mode_label`. Please be aware that the multi-period feature is experimental. If you experience any bugs or unexpected
+behaviour, please report them.
+
+In the standard investment mode, based on investment costs you can compare the usage of existing components against building up new capacity.
+The annual savings by building up new capacity must therefore compensate the annuity of the investment costs (the time period does not have to be one year, but depends on your Datetime index).
 
 See the API of the :py:class:`~oemof.solph.options.Investment` class to see all possible parameters.
 
-Basically, an instance of the investment class can be added to a Flow or a
-Storage. All parameters that usually refer to the *nominal_value/capacity* will
+Basically, an instance of the Investment class can be added to a Flow, a
+Storage or a DSM Sink. All parameters that usually refer to the *nominal_value/capacity* will
 now refer to the investment variables and existing capacity. It is also
 possible to set a maximum limit for the capacity that can be build.
 If existing capacity is considered for a component with investment mode enabled,
-the *ep_costs* still apply only to the newly built capacity.
+the *ep_costs* still apply only to the newly built capacity, i.e. the existing capacity
+comes at no costs.
 
 The investment object can be used in Flows and some components. See the
 :ref:`oemof_solph_components_label` section for detailed information of each
-component.
+component. Besides the flows, it can be invested into
+
+* :ref:`oemof_solph_components_generic_storage_label` and
+* :ref:`oemof_solph_custom_sinkdsm_label`
 
 For example if you want to find out what would be the optimal capacity of a wind
 power plant to decrease the costs of an existing energy system, you can define
 this model and add an investment source.
 The *wind_power_time_series* has to be a normalised feed-in time series of you
 wind power plant. The maximum value might be caused by limited space for wind
 turbines.
@@ -905,15 +916,15 @@
 
     solph.components.Source(label='new_wind_pp', outputs={electricity: solph.flows.Flow(
         fix=wind_power_time_series,
 	    investment=solph.Investment(ep_costs=epc,
 	                                maximum=30000,
 	                                existing=20000))})
 
-The periodical costs (*ep_costs*) are typically calculated as follows:
+The periodical costs (*ep_costs*) are typically calculated as annuities, i.e. as follows:
 
 .. code-block:: python
 
     capex = 1000  # investment cost
     lifetime = 20  # life expectancy
     wacc = 0.05  # weighted average of capital cost
     epc = capex * (wacc * (1 + wacc) ** lifetime) / ((1 + wacc) ** lifetime - 1)
@@ -963,15 +974,15 @@
 
 .. 	image:: _files/nonconvex_invest_investcosts_power.svg
    :width: 70 %
    :alt: nonconvex_invest_investcosts_power.svg
    :align: center
 
 In case of a convex investment (which is the default setting
-`nonconvex=Flase`), the *minimum* attribute leads to a forced investment,
+`nonconvex=False`), the *minimum* attribute leads to a forced investment,
 whereas in the nonconvex case, the investment can become zero as well.
 
 The calculation of the specific costs per kilowatt installed capacity results
 in the following relation for convex and nonconvex investments:
 
 .. 	image:: _files/nonconvex_invest_specific_costs.svg
    :width: 70 %
@@ -981,14 +992,282 @@
 See :py:class:`~oemof.solph.blocks.investment_flow.InvestmentFlow` and
 :py:class:`~oemof.solph.components._generic_storage.GenericInvestmentStorageBlock` for all the
 mathematical background, like variables and constraints, which are used.
 
 .. note:: At the moment the investment class is not compatible with the MIP classes :py:class:`~oemof.solph.options.NonConvex`.
 
 
+.. _multi_period_mode_label:
+
+Using the multi-period (investment) mode (experimental)
+-------------------------------------------------------
+Sometimes you might be interested in how energy systems could evolve in the longer-term, e.g. until 2045 or 2050 to meet some
+carbon neutrality and climate protection or RES and energy efficiency targets.
+
+While in principle, you could try to model this in oemof using the standard investment mode described above (see :ref:`investment_mode_label`),
+you would make the implicit assumption that your entire system is built at the start of your optimization and doesn't change over time.
+To address this shortcoming, the multi-period (investment) feature has been introduced. Be aware that it is still experimental.
+So feel free to report any bugs or unexpected behaviour if you come across them.
+
+While in principle, you can define a dispatch-only multi-period system, this doesn't make much sense. The power of the multi-period feature
+only unfolds if you look at long-term investments. Let's see how.
+
+First, you start by defining your energy system as you might have done before, but you
+
+* choose a longer-term time horizon (spanning multiple years, i.e. multiple periods) and
+* explicitly define the `periods` attribute of your energy system which maps time steps to the simulated period.
+
+.. code-block:: python
+
+    import pandas as pd
+    import oemof.solph as solph
+
+    my_index = pd.date_range('1/1/2013', periods=17520, freq='H')
+    periods = {
+        0: pd.date_range('1/1/2013', periods=8760, freq='H'),
+        1: pd.date_range('1/1/2013', periods=8760, freq='H'),
+    }
+    my_energysystem = solph.EnergySystem(timeindex=my_index, periods=periods)
+
+If you want to use a multi-period model you have define periods of your energy system explicitly. This way,
+you are forced to critically think, e.g. about handling leap years, and take some design decisions.
+
+To assist you, here is a plain python snippet that includes leap years which you can just copy
+and adjust to your needs:
+
+.. code-block:: python
+
+    def determine_periods(datetimeindex):
+        """Explicitly define and return periods of the energy system
+
+        Leap years have 8784 hourly time steps, regular years 8760.
+
+        Parameters
+        ----------
+        datetimeindex : pd.date_range
+            DatetimeIndex of the model comprising all time steps
+
+        Returns
+        -------
+        periods : dict
+            pd.date_ranges defining the time stamps for the respective period,
+            starting with period 0
+        """
+        years = sorted(list(set(getattr(datetimeindex, "year"))))
+        periods = {}
+        filter_series = datetimeindex.to_series()
+        for number, year in enumerate(years):
+            start = filter_series.loc[filter_series.index.year == year].min()
+            end = filter_series.loc[filter_series.index.year == year].max()
+            periods[number] = pd.date_range(start, end, freq=datetimeindex.freq)
+
+        return periods
+
+So if you want to use this, the above would simplify to:
+
+.. code-block:: python
+
+    import pandas as pd
+    import oemof.solph as solph
+
+    # Define your method (or import it from somewhere else)
+    def determine_periods(datetimeindex):
+        ...
+
+    my_index = pd.date_range('1/1/2013', periods=17520, freq='H')
+    periods = determine_periods(my_index)  # Make use of method
+    my_energysystem = solph.EnergySystem(timeindex=my_index, periods=periods)
+
+
+Then you add all the *components* and *buses* to your energy system, just as you are used to with, but with few additions.
+
+.. code-block:: python
+
+    hydrogen_bus = solph.buses.Bus(label="hydrogen")
+    coal_bus = solph.buses.Bus(label="coal")
+    electricity_bus = solph.buses.Bus(label="electricity")
+
+    hydrogen_source = solph.components.Source(
+        label="green_hydrogen",
+        outputs={
+            hydrogen_bus: solph.flows.Flow(
+                variable_costs=[25] * 8760 + [30] * 8760
+            )
+        },
+    )
+
+    coal_source = solph.components.Source(
+        label="hardcoal",
+        outputs={
+            coal_bus: solph.flows.Flow(variable_costs=[20] * 8760 + [24] * 8760)
+        },
+    )
+
+    electrical_sink = solph.components.Sink(
+        label="electricity_demand",
+        inputs={
+            electricity_bus: solph.flows.Flow(
+                nominal_value=1000, fix=[0.8] * len(my_index)
+            )
+        },
+    )
+
+So defining buses is the same as for standard models. Also defining components that do not have any investments associated with
+them or any lifetime limitations is the same.
+
+Now if you want to have components that can be invested into, you use the investment option, just as in :ref:`investment_mode_label`,
+but with a few minor additions and modifications in the investment object itself which you specify by additional attributes:
+
+* You have to specify a `lifetime` attribute. This is the components assumed technical lifetime in years. If it is 20 years,
+  the model invests into it and your simulation has a 30 years horizon, the plant will be decommissioned. Now the model is
+  free to reinvest or choose another option to fill up the missing capacity.
+* You can define an initial `age` if you have `existing` capacity. If you do not specify anything, the default value 0 will be used,
+  meaning your `existing` capacity has just been newly invested.
+* You can define an `interest_rate` that the investor you model has, i.e. the return he desires expressed as the weighted
+  average osts of capital (wacc) and used for calculating annuities in the model itself.
+* You also can define `fixed_costs`, i.e. costs that occur every period independent of the plants usage.
+
+Here is an example
+
+.. code-block:: python
+
+    hydrogen_power_plant = solph.components.Transformer(
+        label="hydrogen_pp",
+        inputs={hydrogen_bus: solph.flows.Flow()},
+        outputs={
+            electricity_bus: solph.flows.Flow(
+                investment=solph.Investment(
+                    maximum=1000,
+                    ep_costs=1e6,
+                    lifetime=30,
+                    interest_rate=0.06,
+                    fixed_costs=100,
+                ),
+                variable_costs=3,
+            )
+        },
+        conversion_factors={electricity_bus: 0.6},
+    )
+
+.. warning::
+
+    The `ep_costs` attribute for investments is used in a different way in a multi-period model. Instead
+    of periodical costs, it depicts (nominal or real) investment expenses, so actual Euros you have to pay per kW or MW
+    (or whatever power or energy unit) installed. Also, you can depict a change in investment expenses over time,
+    so instead of providing a scalar value, you could define a list with investment expenses with one value for each period modelled.
+
+    Annuities are calculated within the model. You do not have to do that.
+    Also the model takes care of discounting future expenses / cashflows.
+
+Below is what it would look like if you altered `ep_costs` and `fixed_costs` per period. This can be done by simply
+providing a list. Note that the length of the list must equal the number of periods of your model.
+This would mean that for investments in the particular period, these values would be the one that are applied over their lifetime.
+
+.. code-block:: python
+
+    hydrogen_power_plant = solph.components.Transformer(
+        label="hydrogen_pp",
+        inputs={hydrogen_bus: solph.flows.Flow()},
+        outputs={
+            electricity_bus: solph.flows.Flow(
+                investment=solph.Investment(
+                    maximum=1000,
+                    ep_costs=[1e6, 1.1e6],
+                    lifetime=30,
+                    interest_rate=0.06,
+                    fixed_costs=[100, 110],
+                ),
+                variable_costs=3,
+            )
+        },
+        conversion_factors={electricity_bus: 0.6},
+    )
+
+For components that is not invested into, you also can specify some additional attributes for their inflows and outflows:
+
+* You can specify a `lifetime` attribute. This can be used to depict existing plants going offline when reaching their lifetime.
+* You can define an initial `age`. Also, this can be used for existing plants.
+* You also can define `fixed_costs`, i.e. costs that occur every period independent of the plants usage. How they are handled
+  depends on whether the flow has a limited or an unlimited lifetime.
+
+.. code-block:: python
+
+    coal_power_plant = solph.components.Transformer(
+        label="existing_coal_pp",
+        inputs={coal_bus: solph.flows.Flow()},
+        outputs={
+            electricity_bus: solph.flows.Flow(
+                nominal_value=600,
+                max=1,
+                min=0.4,
+                lifetime=50,
+                age=46,
+                fixed_costs=100,
+                variable_costs=3,
+            )
+        },
+        conversion_factors={electricity_bus: 0.36},
+    )
+
+To solve our model and retrieve results, you basically perform the same operations as for standard models.
+So it works like this:
+
+.. code-block:: python
+
+    my_energysystem.add(
+        hydrogen_bus,
+        coal_bus,
+        electricity_bus,
+        hydrogen_source,
+        coal_source,
+        electrical_sink,
+        hydrogen_power_plant,
+        coal_power_plant,
+    )
+
+    om = solph.Model(my_energysystem)
+    om.solve(solver="cbc", solve_kwargs={"tee": True})
+
+    # Obtain results
+    results = solph.processing.results(om)
+    hydrogen_results = solph.views.node(results, "hydrogen_pp")
+
+    # Show investment plan for hydrogen power plants
+    print(hydrogen_results["period_scalars"])
+
+The keys in the results dict in a multi-period model are "sequences" and "period_scalars".
+So for sequences, it is all the same, while for scalar values, we now have values for each period.
+
+Besides the `invest` variable, new variables are introduced as well. These are:
+
+* `total`: The total capacity installed, i.e. how much is actually there in a given period.
+* `old`: (Overall) capacity to be decommissioned in a given period.
+* `old_end`: Endogenous capacity to be decommissioned in a given period. This is capacity that has been invested into
+  in the model itself.
+* `old_exo`: Exogenous capacity to be decommissioned in a given period. This is capacity that was already existing and
+  given by the `existing` attribute.
+
+.. note::
+
+    * You can specify a `discount_rate` for the model. If you do not do so, 0.02 will be used as a default, corresponding
+      to sort of a social discount rate. If you work with costs in real terms, discounting is obsolete, so define
+      `discount_rate = 0` in that case.
+    * You can specify an `interest_rate` for every investment object. If you do not do so, it will be chosen the same
+      as the model's `discount_rate`. You could use this default to model a perfect competition administered by some sort of
+      social planner, but even in a social planner setting, you might want to deviate from the `discount_rate`
+      value and/or discriminate among technologies with different risk profiles and hence different interest requirements.
+    * For storage units, the `initial_content` is not allowed combined with multi-period investments.
+      The storage inflow and outflow are forced to zero until the storage unit is invested into.
+    * You can specify periods of different lengths, but the frequency of your timeindex needs to be consistent. Also,
+      you could use the `timeincrement` attribute of the energy system to model different weightings. Be aware that this
+      has not yet been tested.
+    * Also please be aware, that periods correspond to years by default. You could also choose
+      monthly periods, but you would need to be very careful in parameterizing your energy system and your model and also,
+      this would mean monthly discounting (if applicable) as well as specifying your plants lifetimes in months.
+
 Mixed Integer (Linear) Problems
 -------------------------------
 
 Solph also allows you to model components with respect to more technical details,
 such as minimum power production. This can be done in both possible combinations,
 as dispatch optimization with fixed capacities or combined dispatch and investment optimization.
 
@@ -1033,15 +1312,15 @@
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 Since version 'v0.5', it is also possilbe to combine the investment and nonconvex option.
 Therefore, a new constraint block for flows, called :py:class:`~oemof.solph.flows._invest_non_convex_flow_block.InvestNonConvexFlowBlock` has been developed,
 which combines both :py:class:`~oemof.solph._options.Investment` and :py:class:`~oemof.solph._options.NonConvex` classes.
 The new class offers the possibility to perform the investment optimization of an asset considering `min`/`max` values of the flow
 as fractions of the optimal capacity. Moreover, it obtains the optimal 'status' of the flow during the simulation period.
 
-It must be noted that in a streighforward implementation, a binary variable
+It must be noted that in a straighforward implementation, a binary variable
 representing the 'status' of the flow at each time is multiplied by the 'invest' parameter,
 which is a continuous variable representing the capacity of the asset being optimized (i.e., :math:`status \times invest`).
 This nonlinearity is linearised in the
 :py:class:`~oemof.solph.flows._invest_non_convex_flow_block.InvestNonConvexFlowBlock`
 
 .. code-block:: python
```

### Comparing `oemof.solph-0.5.1.dev0/docs/whatsnew/v0-0-2.rst` & `oemof.solph-0.5.1.dev1/docs/whatsnew/v0-0-2.rst`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/docs/whatsnew/v0-0-3.rst` & `oemof.solph-0.5.1.dev1/docs/whatsnew/v0-0-3.rst`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/docs/whatsnew/v0-0-4.rst` & `oemof.solph-0.5.1.dev1/docs/whatsnew/v0-0-4.rst`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/docs/whatsnew/v0-0-5.rst` & `oemof.solph-0.5.1.dev1/docs/whatsnew/v0-0-5.rst`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/docs/whatsnew/v0-0-6.rst` & `oemof.solph-0.5.1.dev1/docs/whatsnew/v0-0-6.rst`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/docs/whatsnew/v0-1-0.rst` & `oemof.solph-0.5.1.dev1/docs/whatsnew/v0-1-0.rst`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/docs/whatsnew/v0-1-2.rst` & `oemof.solph-0.5.1.dev1/docs/whatsnew/v0-1-2.rst`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/docs/whatsnew/v0-2-0.rst` & `oemof.solph-0.5.1.dev1/docs/whatsnew/v0-2-0.rst`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/docs/whatsnew/v0-2-1.rst` & `oemof.solph-0.5.1.dev1/docs/whatsnew/v0-2-1.rst`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/docs/whatsnew/v0-2-2.rst` & `oemof.solph-0.5.1.dev1/docs/whatsnew/v0-2-2.rst`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/docs/whatsnew/v0-3-0.rst` & `oemof.solph-0.5.1.dev1/docs/whatsnew/v0-3-0.rst`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/docs/whatsnew/v0-3-1.rst` & `oemof.solph-0.5.1.dev1/docs/whatsnew/v0-3-1.rst`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/docs/whatsnew/v0-3-2.rst` & `oemof.solph-0.5.1.dev1/docs/whatsnew/v0-3-2.rst`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/docs/whatsnew/v0-4-0.rst` & `oemof.solph-0.5.1.dev1/docs/whatsnew/v0-4-0.rst`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/docs/whatsnew/v0-4-4.rst` & `oemof.solph-0.5.1.dev1/docs/whatsnew/v0-4-4.rst`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/docs/whatsnew/v0-4-5.rst` & `oemof.solph-0.5.1.dev1/docs/whatsnew/v0-4-5.rst`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/docs/whatsnew/v0-5-0.rst` & `oemof.solph-0.5.1.dev1/docs/whatsnew/v0-5-0.rst`

 * *Files 9% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 * The flow arguments `summed_min`and `summed_max` now have the more descriptive names `full_load_time_min` and `full_load_time_max`.
 * Keyword arguments are now explicit. This will i.e. catch typos. Custom attributes can be added using the argument `custom_attributes`. Those will be passed down the class hierachy and can (possibly) be handled in parent classes.
 
 
 New features
 ############
 
-* Add `inactivity_costs` as an option for `Flow`s. Inactivity costs is a cost for times where a Flow is not operated.
-* It is now possible to optimise the size of `Flow`s that have a status variable. Internally, this is done by the `InvestNonConvexFlowBlock` which provides the possibility to perform capacity optimization of assets considering their min/max loads, as well as their operation status.
+* Add `inactivity_costs` as an option for `Flow` objects. Inactivity costs is a cost for times where a Flow is not operated.
+* It is now possible to optimise the size of `Flow` objects that have a status variable. Internally, this is done by the `InvestNonConvexFlowBlock` which provides the possibility to perform capacity optimization of assets considering their min/max loads, as well as their operation status.
 
 Documentation
 #############
 
 * Examples are added to the documentation.
 
 
@@ -48,7 +48,8 @@
 * David Fuhrländer
 * "lensum"
 * Jan Launner
 * Hendrik Huyskens
 * Ekaterina Zolotarevskaia
 * Sarah Berendes
 * Francesco Witte
+* Johannes Kochems
```

### Comparing `oemof.solph-0.5.1.dev0/examples/basic_example/basic_example.csv` & `oemof.solph-0.5.1.dev1/examples/basic_example/basic_example.csv`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/examples/excel_reader/scenario.xlsx` & `oemof.solph-0.5.1.dev1/examples/excel_reader/scenario.xlsx`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/examples/invest_nonconvex_flow_examples/solar_generation.csv` & `oemof.solph-0.5.1.dev1/examples/invest_nonconvex_flow_examples/solar_generation.csv`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/examples/simple_dispatch/input_data.csv` & `oemof.solph-0.5.1.dev1/examples/simple_dispatch/input_data.csv`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/examples/storage_investment/storage_investment.csv` & `oemof.solph-0.5.1.dev1/examples/storage_investment/storage_investment.csv`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/examples/tuple_as_labels/tuple_as_label.csv` & `oemof.solph-0.5.1.dev1/examples/tuple_as_labels/tuple_as_label.csv`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/examples/variable_chp/variable_chp.csv` & `oemof.solph-0.5.1.dev1/examples/variable_chp/variable_chp.csv`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/setup.cfg` & `oemof.solph-0.5.1.dev1/setup.cfg`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/setup.py` & `oemof.solph-0.5.1.dev1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         "", read("README.rst")
     )
 )
 
 
 setup(
     name="oemof.solph",
-    version="0.5.1.dev0",
+    version="0.5.1.dev1",
     license="MIT",
     description=(
         "A model generator for energy system modelling and optimisation."
     ),
     long_description=long_description,
     long_description_content_type="text/x-rst",
     author="oemof developer group",
@@ -76,15 +76,15 @@
     ],
     python_requires=">=3.8",
     install_requires=[
         "blinker",
         "dill",
         "numpy",
         "pandas >= 1.5.3",
-        "pyomo >= 6.0.0, < 7.0",
+        "pyomo >= 6.6.0, < 7.0",
         "networkx",
         "oemof.tools >= 0.4.2",
         "oemof.network >= 0.5.0a1",
     ],
     extras_require={
         "dev": [
             "pytest",
```

### Comparing `oemof.solph-0.5.1.dev0/src/oemof/solph/__init__.py` & `oemof.solph-0.5.1.dev1/src/oemof/solph/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.5.1.dev0"
+__version__ = "0.5.1.dev1"
 
 from . import buses
 from . import components
 from . import constraints
 from . import flows
 from . import helpers
 from . import processing
```

### Comparing `oemof.solph-0.5.1.dev0/src/oemof/solph/_console_scripts.py` & `oemof.solph-0.5.1.dev1/src/oemof/solph/_console_scripts.py`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/src/oemof/solph/_energy_system.py` & `oemof.solph-0.5.1.dev1/src/oemof/solph/_energy_system.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,26 +4,28 @@
 solph version of oemof.network.energy_system
 
 SPDX-FileCopyrightText: Uwe Krien <krien@uni-bremen.de>
 SPDX-FileCopyrightText: Simon Hilpert
 SPDX-FileCopyrightText: Cord Kaldemeyer
 SPDX-FileCopyrightText: Stephan Günther
 SPDX-FileCopyrightText: Birgit Schachler
+SPDX-FileCopyrightText: Johannes Kochems
 
 SPDX-License-Identifier: MIT
 
 """
 
 import calendar
 import datetime
 import warnings
 
 import numpy as np
 import pandas as pd
 from oemof.network import energy_system as es
+from oemof.tools import debugging
 
 
 class EnergySystem(es.EnergySystem):
     """A variant of the class EnergySystem from
     <oemof.network.network.energy_system.EnergySystem> specially tailored to
     solph.
 
@@ -44,22 +46,35 @@
     timeincrement : iterable
 
     infer_last_interval : bool
         Add an interval to the last time point. The end time of this interval
         is unknown so it does only work for an equidistant DatetimeIndex with
         a 'freq' attribute that is not None. The parameter has no effect on the
         timeincrement parameter.
+
+    periods : list or None
+        The periods of a multi-period model.
+        If this is explicitly specified, it leads to creating a multi-period
+        model, providing a respective user warning as a feedback.
+
+        list of pd.date_range objects carrying the timeindex for the
+        respective period;
+
+        For a standard model, periods are not (to be) declared, i.e. None.
+        A list with one entry is derived, i.e. [0].
+
     kwargs
     """
 
     def __init__(
         self,
         timeindex=None,
         timeincrement=None,
         infer_last_interval=None,
+        periods=None,
         **kwargs,
     ):
         # Doing imports at runtime is generally frowned upon, but should work
         # for now. See the TODO in :func:`constraint_grouping
         # <oemof.solph.groupings.constraint_grouping>` for more information.
         from oemof.solph import GROUPINGS
 
@@ -104,40 +119,83 @@
                     periods=1,
                     freq=timeindex.freq,
                 )
             )
 
         # catch wrong combinations and infer timeincrement from timeindex.
         if timeincrement is not None and timeindex is not None:
-            msg = (
-                "Specifying the timeincrement and the timeindex parameter at "
-                "the same time is not allowed since these might be "
-                "conflicting to each other."
-            )
-            raise AttributeError(msg)
+            if periods is None:
+                msg = (
+                    "Specifying the timeincrement and the timeindex parameter "
+                    "at the same time is not allowed since these might be "
+                    "conflicting to each other."
+                )
+                raise AttributeError(msg)
+            else:
+                msg = (
+                    "Ensure that your timeindex and timeincrement are "
+                    "consistent.\nIf you are not considering non-equidistant "
+                    "timeindices, consider only specifying a timeindex."
+                )
+                warnings.warn(msg, debugging.SuspiciousUsageWarning)
 
         elif timeindex is not None and timeincrement is None:
             df = pd.DataFrame(timeindex)
             timedelta = df.diff()
-            timeincrement = pd.Series(
-                (timedelta / np.timedelta64(1, "h"))[1:].set_index(0).index
-            )
+            timeincrement = timedelta / np.timedelta64(1, "h")
+
+            # we want a series (squeeze)
+            # without the first item (no delta defined for first entry)
+            # but starting with index 0 (reset)
+            timeincrement = timeincrement.squeeze()[1:].reset_index(drop=True)
 
         if timeincrement is not None and (pd.Series(timeincrement) <= 0).any():
             msg = (
                 "The time increment is inconsistent. Negative values and zero "
                 "is not allowed.\nThis is caused by a inconsistent "
                 "timeincrement parameter or an incorrect timeindex."
             )
             raise TypeError(msg)
 
         super().__init__(
             timeindex=timeindex, timeincrement=timeincrement, **kwargs
         )
 
+        if periods is not None:
+            msg = (
+                "CAUTION! You specified the 'periods' attribute for your "
+                "energy system.\n This will lead to creating "
+                "a multi-period optimization modeling which can be "
+                "used e.g. for long-term investment modeling.\n"
+                "Please be aware that the feature is experimental as of "
+                "now. If you find anything suspicious or any bugs, "
+                "please report them."
+            )
+            warnings.warn(msg, debugging.SuspiciousUsageWarning)
+        self.periods = periods
+        self._extract_periods_years()
+
+    def _extract_periods_years(self):
+        """Map simulation years to the respective period based on time indices
+
+        Returns
+        -------
+        periods_years: dict
+            the simulation year of the start of each a period,
+            relative to the start of the optimization run and starting with 0
+        """
+        periods_years = [0]
+        if self.periods is not None:
+            start_year = self.periods[0].min().year
+            for k, v in enumerate(self.periods):
+                if k >= 1:
+                    periods_years.append(v.min().year - start_year)
+
+            self.periods_years = periods_years
+
 
 def create_time_index(
     year: int = None,
     interval: float = 1,
     number: int = None,
     start: datetime.datetime or datetime.date = None,
 ):
```

### Comparing `oemof.solph-0.5.1.dev0/src/oemof/solph/_groupings.py` & `oemof.solph-0.5.1.dev1/src/oemof/solph/_groupings.py`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/src/oemof/solph/_helpers.py` & `oemof.solph-0.5.1.dev1/src/oemof/solph/_helpers.py`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/src/oemof/solph/_models.py` & `oemof.solph-0.5.1.dev1/src/oemof/solph/_models.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 SPDX-License-Identifier: MIT
 
 """
 import logging
 import warnings
 from logging import getLogger
 
+from oemof.tools import debugging
 from pyomo import environ as po
 from pyomo.core.plugins.transform.relax_integrality import RelaxIntegrality
 from pyomo.opt import SolverFactory
 
 from oemof.solph import processing
 from oemof.solph.buses._bus import BusBlock
 from oemof.solph.components._transformer import TransformerBlock
@@ -35,61 +36,61 @@
 class LoggingError(BaseException):
     """Raised when the wrong logging level is used."""
 
     pass
 
 
 class BaseModel(po.ConcreteModel):
-    """The BaseModel for other solph-models (Model, MultiPeriodModel, etc.)
+    """The BaseModel for other solph-models (Model)
 
     Parameters
     ----------
     energysystem : EnergySystem object
         Object that holds the nodes of an oemof energy system graph
     constraint_groups : list (optional)
         Solph looks for these groups in the given energy system and uses them
         to create the constraints of the optimization problem.
         Defaults to `Model.CONSTRAINTS`
     objective_weighting : array like (optional)
         Weights used for temporal objective function
-        expressions. If nothing is passed `timeincrement` will be used which
+        expressions. If nothing is passed, `timeincrement` will be used which
         is calculated from the freq length of the energy system timeindex or
         can be directly passed as a sequence.
     auto_construct : boolean
         If this value is true, the set, variables, constraints, etc. are added,
         automatically when instantiating the model. For sequential model
         building process set this value to False
         and use methods `_add_parent_block_sets`,
         `_add_parent_block_variables`, `_add_blocks`, `_add_objective`
 
     Attributes
     ----------
     timeincrement : sequence
-        Time increments.
+        Time increments
     flows : dict
-        Flows of the model.
+        Flows of the model
     name : str
-        Name of the model.
+        Name of the model
     es : solph.EnergySystem
-        Energy system of the model.
+        Energy system of the model
     meta : `pyomo.opt.results.results_.SolverResults` or None
-        Solver results.
+        Solver results
     dual : `pyomo.core.base.suffix.Suffix` or None
         Store the dual variables of the model if pyomo suffix is set to IMPORT
     rc : `pyomo.core.base.suffix.Suffix` or None
         Store the reduced costs of the model if pyomo suffix is set to IMPORT
     """
 
-    # The default list of constraint groups to be used for a model.
+    # The default list of constraint groups to be used for a model
     CONSTRAINT_GROUPS = []
 
     def __init__(self, energysystem, **kwargs):
         """Initialize a BaseModel, using its energysystem as well as
-        optional kwargs for specifying the timeincrement, objective_weigting
-        and constraint groups."""
+        optional kwargs for specifying the timeincrement, objective_weighting
+        and constraint_groups."""
         super().__init__()
 
         # Check root logger. Due to a problem with pyomo the building of the
         # model will take up to a 100 times longer if the root logger is set
         # to DEBUG
 
         if getLogger().level <= 10 and kwargs.get("debug", False) is False:
@@ -134,24 +135,26 @@
         self.rc = None
 
         if kwargs.get("auto_construct", True):
             self._construct()
 
     def _construct(self):
         """Construct a BaseModel by adding parent block sets and variables
-        as well as child blocks and variables to it."""
+        as well as child blocks and variables to it.
+        """
         self._add_parent_block_sets()
         self._add_parent_block_variables()
         self._add_child_blocks()
         self._add_objective()
 
     def _add_parent_block_sets(self):
         """Method to create all sets located at the parent block, i.e. in the
         model itself, as they are to be shared across all model components.
-        See the class :py:class:~oemof.solph.models.Model for the sets created.
+        See the class :py:class:~oemof.solph._models.Model
+        for the sets created.
         """
         pass
 
     def _add_parent_block_variables(self):
         """Method to create all variables located at the parent block,
         i.e. the model itself as these variables  are to be shared across
         all model components.
@@ -159,15 +162,16 @@
         for the `flow` variable created.
         """
         pass
 
     def _add_child_blocks(self):
         """Method to add the defined child blocks for components that have
         been grouped in the defined constraint groups. This collects all the
-        constraints from the component blocks and adds them to the model.
+        constraints from the buses, components and flows blocks
+        and adds them to the model.
         """
         for group in self._constraint_groups:
             # create instance for block
             block = group()
             # Add block to model
             self.add_component(str(block), block)
             # create constraints etc. related with block for all nodes
@@ -267,61 +271,97 @@
         relaxer = RelaxIntegrality()
         relaxer._apply_to(self)
 
         return self
 
 
 class Model(BaseModel):
-    """An  energy system model for operational and/or investment
+    """An energy system model for operational and/or investment
     optimization.
 
     Parameters
     ----------
     energysystem : EnergySystem object
         Object that holds the nodes of an oemof energy system graph
     constraint_groups : list
         Solph looks for these groups in the given energy system and uses them
         to create the constraints of the optimization problem.
         Defaults to `Model.CONSTRAINT_GROUPS`
+    discount_rate : float or None
+        The rate used for discounting in a multi-period model.
+        A 2% discount rate needs to be defined as 0.02.
+
+    Note
+    ----
+
+    * The discount rate is only applicable for a multi-period model.
+    * If you want to work with costs data in nominal terms,
+      you should specify a discount rate.
+    * By default, there is a discount rate of 2% in a multi-period model.
+    * If you want to provide your costs data in real terms,
+      just specify `discount_rate = 0`, i.e. effectively there will be
+      no discounting.
 
 
     **The following basic sets are created**:
 
     NODES
         A set with all nodes of the given energy system.
 
     TIMESTEPS
         A set with all timesteps of the given time horizon.
 
+    PERIODS
+        A set with all investment periods of the given time horizon.
+
+    TIMEINDEX
+        A set with all time indices of the given time horizon, whereby
+        time indices are defined as a tuple consisting of the period and the
+        timestep. E.g. (2, 10) would be timestep 10 (which is exactly the same
+        as in the TIMESTEPS set) and which is in period 2.
+
     FLOWS
         A 2 dimensional set with all flows. Index: `(source, target)`
 
     **The following basic variables are created**:
 
     flow
-        Flow from source to target indexed by FLOWS, TIMESTEPS.
+        Flow from source to target indexed by FLOWS, TIMEINDEX.
         Note: Bounds of this variable are set depending on attributes of
         the corresponding flow object.
 
     """
 
     CONSTRAINT_GROUPS = [
         BusBlock,
         TransformerBlock,
         InvestmentFlowBlock,
         SimpleFlowBlock,
         NonConvexFlowBlock,
         InvestNonConvexFlowBlock,
     ]
 
-    def __init__(self, energysystem, **kwargs):
+    def __init__(self, energysystem, discount_rate=None, **kwargs):
+        if discount_rate is not None:
+            self.discount_rate = discount_rate
+        elif energysystem.periods is not None:
+            self.discount_rate = 0.02
+            msg = (
+                f"By default, a discount_rate of {self.discount_rate} "
+                f"is used for a multi-period model. "
+                f"If you want to use another value, "
+                f"you have to specify the `discount_rate` attribute."
+            )
+            warnings.warn(msg, debugging.SuspiciousUsageWarning)
         super().__init__(energysystem, **kwargs)
 
     def _add_parent_block_sets(self):
-        """Add all basic sets to the model, i.e. NODES, TIMESTEPS and FLOWS."""
+        """Add all basic sets to the model, i.e. NODES, TIMESTEPS and FLOWS.
+        Also create sets PERIODS and TIMEINDEX used for multi-period models.
+        """
         # set with all nodes
         self.NODES = po.Set(initialize=[n for n in self.es.nodes])
 
         if self.es.timeincrement is None:
             msg = (
                 "The EnergySystem needs to have a valid 'timeincrement' "
                 "attribute to build a model."
@@ -332,14 +372,49 @@
         self.TIMESTEPS = po.Set(
             initialize=range(len(self.es.timeincrement)), ordered=True
         )
         self.TIMEPOINTS = po.Set(
             initialize=range(len(self.es.timeincrement) + 1), ordered=True
         )
 
+        if self.es.periods is None:
+            self.TIMEINDEX = po.Set(
+                initialize=list(
+                    zip(
+                        [0] * len(self.es.timeincrement),
+                        range(len(self.es.timeincrement)),
+                    )
+                ),
+                ordered=True,
+            )
+            self.PERIODS = po.Set(initialize=[0])
+        else:
+            nested_list = [
+                [k] * len(self.es.periods[k])
+                for k in range(len(self.es.periods))
+            ]
+            flattened_list = [
+                item for sublist in nested_list for item in sublist
+            ]
+            self.TIMEINDEX = po.Set(
+                initialize=list(
+                    zip(flattened_list, range(len(self.es.timeincrement)))
+                ),
+                ordered=True,
+            )
+            self.PERIODS = po.Set(
+                initialize=sorted(list(set(range(len(self.es.periods)))))
+            )
+
+        # (Re-)Map timesteps to periods
+        timesteps_in_period = {p: [] for p in self.PERIODS}
+        for p, t in self.TIMEINDEX:
+            timesteps_in_period[p].append(t)
+        self.TIMESTEPS_IN_PERIOD = timesteps_in_period
+
         # previous timesteps
         previous_timesteps = [x - 1 for x in self.TIMESTEPS]
         previous_timesteps[0] = self.TIMESTEPS.last()
 
         self.previous_timesteps = dict(zip(self.TIMESTEPS, previous_timesteps))
 
         # pyomo set for all flows in the energy system graph
@@ -361,39 +436,39 @@
             ordered=True,
             dimen=2,
             within=self.FLOWS,
         )
 
     def _add_parent_block_variables(self):
         """Add the parent block variables, which is the `flow` variable,
-        indexed by FLOWS and TIMESTEPS."""
-        self.flow = po.Var(self.FLOWS, self.TIMESTEPS, within=po.Reals)
+        indexed by FLOWS and TIMEINDEX."""
+        self.flow = po.Var(self.FLOWS, self.TIMEINDEX, within=po.Reals)
 
         for o, i in self.FLOWS:
             if self.flows[o, i].nominal_value is not None:
                 if self.flows[o, i].fix[self.TIMESTEPS.at(1)] is not None:
-                    for t in self.TIMESTEPS:
-                        self.flow[o, i, t].value = (
+                    for p, t in self.TIMEINDEX:
+                        self.flow[o, i, p, t].value = (
                             self.flows[o, i].fix[t]
                             * self.flows[o, i].nominal_value
                         )
-                        self.flow[o, i, t].fix()
+                        self.flow[o, i, p, t].fix()
                 else:
-                    for t in self.TIMESTEPS:
-                        self.flow[o, i, t].setub(
+                    for p, t in self.TIMEINDEX:
+                        self.flow[o, i, p, t].setub(
                             self.flows[o, i].max[t]
                             * self.flows[o, i].nominal_value
                         )
 
                     if not self.flows[o, i].nonconvex:
-                        for t in self.TIMESTEPS:
-                            self.flow[o, i, t].setlb(
+                        for p, t in self.TIMEINDEX:
+                            self.flow[o, i, p, t].setlb(
                                 self.flows[o, i].min[t]
                                 * self.flows[o, i].nominal_value
                             )
                     elif (o, i) in self.UNIDIRECTIONAL_FLOWS:
-                        for t in self.TIMESTEPS:
-                            self.flow[o, i, t].setlb(0)
+                        for p, t in self.TIMEINDEX:
+                            self.flow[o, i, p, t].setlb(0)
             else:
                 if (o, i) in self.UNIDIRECTIONAL_FLOWS:
-                    for t in self.TIMESTEPS:
-                        self.flow[o, i, t].setlb(0)
+                    for p, t in self.TIMEINDEX:
+                        self.flow[o, i, p, t].setlb(0)
```

### Comparing `oemof.solph-0.5.1.dev0/src/oemof/solph/_plumbing.py` & `oemof.solph-0.5.1.dev1/src/oemof/solph/_plumbing.py`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/src/oemof/solph/buses/_bus.py` & `oemof.solph-0.5.1.dev1/src/oemof/solph/buses/_bus.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 SPDX-FileCopyrightText: Simon Hilpert
 SPDX-FileCopyrightText: Cord Kaldemeyer
 SPDX-FileCopyrightText: Stephan Günther
 SPDX-FileCopyrightText: Patrik Schönfeldt
 SPDX-FileCopyrightText: Birgit Schachler
 SPDX-FileCopyrightText: jnnr
 SPDX-FileCopyrightText: jmloenneberga
+SPDX-FileCopyrightText: Johannes Kochems
 
 SPDX-License-Identifier: MIT
 
 """
 
 from oemof.network import network as on
 from pyomo.core import BuildAction
@@ -22,14 +23,20 @@
 
 class Bus(on.Bus):
     """A balance object. Every component has to be connected to buses.
 
     The sum of all inputs of a Bus object must equal the sum of all outputs
     within one time step.
 
+    Attributes
+    ----------
+    balanced: boolean
+        Indicates if bus is balanced, i.e. if the sum of inflows equals to
+        the sum of outflows for each timestep; defaults to True
+
     Notes
     -----
     The following sets, variables, constraints and objective parts are created
      * :py:class:`~oemof.solph.buses._bus.BusBlock`
 
     """
 
@@ -50,34 +57,34 @@
      The sum of all inputs of a Bus object must equal the sum of all outputs
      within one time step.
 
      **The following constraints are build:**
 
      Bus balance: `om.Bus.balance[i, o, t]`
        .. math::
-         \sum_{i \in INPUTS(n)} P_{i}(t) =
-         \sum_{o \in OUTPUTS(n)} P_{o}(t), \\
-         \forall t \in \textrm{TIMESTEPS}, \\
+         \sum_{i \in INPUTS(n)} P_{i}(p, t) =
+         \sum_{o \in OUTPUTS(n)} P_{o}(p, t), \\
+         \forall p, t \in \textrm{TIMEINDEX}, \\
          \forall i \in \textrm{INPUTS}, \\
          \forall o \in \textrm{OUTPUTS}
 
      While INPUTS is the set of Component objects connected with the input of
      the Bus object and OUPUTS the set of Component objects connected with the
      output of the Bus object.
 
      The index :math:`n` is the index for the Bus node itself. Therefore,
-     a :math:`flow[i, n, t]` is a flow from the Component i to the Bus n at
-     time step t.
+     a :math:`flow[i, n, p, t]` is a flow from the Component i to the Bus n at
+     time index p, t.
 
      ======================  ============================  ====================
      symbol                  attribute                     explanation
      ======================  ============================  ====================
-     :math:`P_{i}(t)`        `flow[i, n, t]`               Bus, inflow
+     :math:`P_{i}(p, t)`     `flow[i, n, p, t]`            Bus, inflow
 
-     :math:`P_{o}(t)`        `flow[n, o, t]`               Bus, outflow
+     :math:`P_{o}(p, t)`     `flow[n, o, p, t]`            Bus, outflow
 
      ======================  ============================  ====================
      """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
@@ -98,18 +105,18 @@
         ins = {}
         outs = {}
         for n in group:
             ins[n] = [i for i in n.inputs]
             outs[n] = [o for o in n.outputs]
 
         def _busbalance_rule(block):
-            for t in m.TIMESTEPS:
+            for p, t in m.TIMEINDEX:
                 for g in group:
-                    lhs = sum(m.flow[i, g, t] for i in ins[g])
-                    rhs = sum(m.flow[g, o, t] for o in outs[g])
+                    lhs = sum(m.flow[i, g, p, t] for i in ins[g])
+                    rhs = sum(m.flow[g, o, p, t] for o in outs[g])
                     expr = lhs == rhs
                     # no inflows no outflows yield: 0 == 0 which is True
                     if expr is not True:
-                        block.balance.add((g, t), expr)
+                        block.balance.add((g, p, t), expr)
 
-        self.balance = Constraint(group, m.TIMESTEPS, noruleinit=True)
+        self.balance = Constraint(group, m.TIMEINDEX, noruleinit=True)
         self.balance_build = BuildAction(rule=_busbalance_rule)
```

### Comparing `oemof.solph-0.5.1.dev0/src/oemof/solph/buses/experimental/_electrical_bus.py` & `oemof.solph-0.5.1.dev1/src/oemof/solph/buses/experimental/_electrical_bus.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,31 +7,34 @@
 SPDX-FileCopyrightText: Simon Hilpert
 SPDX-FileCopyrightText: Cord Kaldemeyer
 SPDX-FileCopyrightText: Patrik Schönfeldt
 SPDX-FileCopyrightText: Johannes Röder
 SPDX-FileCopyrightText: jakob-wo
 SPDX-FileCopyrightText: gplssm
 SPDX-FileCopyrightText: jnnr
+SPDX-FileCopyrightText: Johannes Kochems
 
 SPDX-License-Identifier: MIT
 
 """
 
 from oemof.solph.buses._bus import Bus
 
 
 class ElectricalBus(Bus):
-    r"""A electrical bus object. Every node has to be connected to BusBlock.
+    r"""An electrical bus object used for linear optimal power flow (LOPF)
+
+    Every (spatial) node has to be connected to a BusBlock.
     This BusBlock is used in combination with ElectricalLine objects
     for linear optimal power flow (lopf) calculations.
 
     Parameters
     ----------
     slack: boolean
-        If True BusBlock is slack bus for network
+        If True BusBlock is slack bus for electrical network
     v_max: numeric
         Maximum value of voltage angle at electrical bus
     v_min: numeric
         Mininum value of voltage angle at electrical bus
 
     Note: This component is experimental. Use it with care.
```

### Comparing `oemof.solph-0.5.1.dev0/src/oemof/solph/components/__init__.py` & `oemof.solph-0.5.1.dev1/src/oemof/solph/components/__init__.py`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/src/oemof/solph/components/_extraction_turbine_chp.py` & `oemof.solph-0.5.1.dev1/src/oemof/solph/components/_extraction_turbine_chp.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 SPDX-FileCopyrightText: Cord Kaldemeyer
 SPDX-FileCopyrightText: Patrik Schönfeldt
 SPDX-FileCopyrightText: FranziPl
 SPDX-FileCopyrightText: jnnr
 SPDX-FileCopyrightText: Stephan Günther
 SPDX-FileCopyrightText: FabianTU
 SPDX-FileCopyrightText: Johannes Röder
+SPDX-FileCopyrightText: Johannes Kochems
 
 SPDX-License-Identifier: MIT
 
 """
 
 from pyomo.core.base.block import ScalarBlock
 from pyomo.environ import BuildAction
@@ -24,20 +25,21 @@
 
 from oemof.solph._plumbing import sequence as solph_sequence
 from oemof.solph.components._transformer import Transformer
 
 
 class ExtractionTurbineCHP(Transformer):
     r"""
-    A CHP with an extraction turbine in a linear model. For more options see
-    the :class:`~oemof.solph.components.GenericCHP` class.
+    A CHP with an extraction turbine in a linear model. For a more
+    detailled modelling approach providing more options, also see
+    the :class:`.GenericCHP` class.
 
     One main output flow has to be defined and is tapped by the remaining flow.
     The conversion factors have to be defined for the maximum tapped flow (
-    full CHP mode) and for no tapped flow (full condensing mode). Even though
+    full CHP mode) and for no tapped flow (full condensing mode). Even though,
     it is possible to limit the variability of the tapped flow, so that the
     full condensing mode will never be reached.
 
     Parameters
     ----------
     conversion_factors : dict
         Dictionary containing conversion factors for conversion of inflow
@@ -91,33 +93,33 @@
 
     def constraint_group(self):
         return ExtractionTurbineCHPBlock
 
 
 class ExtractionTurbineCHPBlock(ScalarBlock):
     r"""Block for all instances of
-    :class:`~oemof.solph.components.ExtractionTurbineCHP`
+    :class:`~oemof.solph.components.experimental._ExtractionTurbineCHP`
 
     **Variables**
 
     The following variables are used:
 
     * :math:`\dot H_{Fuel}`
 
-        Fuel input flow, represented in code as `flow[i,n,t]`
+        Fuel input flow, represented in code as `flow[i, n, p, t]`
 
     * :math:`P_{el}`
 
         Electric power outflow, represented in code as
-        `flow[n, main_output, t]`
+        `flow[n, main_output, p, t]`
 
     * :math:`\dot Q_{th}`
 
         Thermal output flow, represented in code as
-        `flow[n, tapped_output, t]`
+        `flow[n, tapped_output, p, t]`
 
     **Parameters**
 
     The following parameters are created as attributes of
     :attr:`om.ExtractionTurbineCHP`:
 
     * :math:`\eta_{el,woExtr}`
@@ -141,16 +143,16 @@
     instances of :class:`oemof.solph.components.ExtractionTurbineCHP`:
 
     .. _ETCHP-equations:
 
         .. math::
             &
             (1)\dot H_{Fuel}(t) =
-                \frac{P_{el}(t) + \dot Q_{th}(t) \cdot \beta(t)}
-                    {\eta_{el,woExtr}(t)} \\
+               \frac{P_{el}(t) + \dot Q_{th}(t) \cdot \beta(t)}
+                 {\eta_{el,woExtr}(t)} \\
             &
             (2)P_{el}(t) \geq \dot Q_{th}(t) \cdot C_b
 
     where:
 
     .. math::
 
@@ -161,36 +163,57 @@
 
     .. math::
 
         C_b = \frac{\eta_{el,maxExtr}(t)}{\eta_{th,maxExtr}(t)}
 
     The first equation is the result of the relation between the input
     flow and the two output flows, the second equation stems from how the two
-    output flows relate to each other.
+    output flows relate to each other, and the symbols used are defined as
+    follows (with Variables (V) and Parameters (P)):
+
+    ========================= ============================================ ==== =========
+    symbol                    attribute                                    type explanation
+    ========================= ============================================ ==== =========
+    :math:`\dot H_{Fuel}`     `flow[i, n, t]`                              V    fuel input flow
+
+    :math:`P_{el}`            `flow[n, main_output, t]`                    V    electric power
+
+    :math:`\dot Q_{th}`       `flow[n, tapped_output, t]`                  V    thermal output
+
+    :math:`\beta`             `main_flow_loss_index[n, t]`                 P    power loss index
+
+    :math:`\eta_{el,woExtr}`  `conversion_factor_full_condensation[n, t]`  P    electric efficiency
+                                                                                        without heat extraction
+    :math:`\eta_{el,maxExtr}` `conversion_factors[main_output][n, t]`      P    electric efficiency
+                                                                                        with max heat extraction
+    :math:`\eta_{th,maxExtr}` `conversion_factors[tapped_output][n, t]`    P    thermal efficiency with
+                                                                                        maximal heat extraction
+    ========================= ============================================ ==== =========
 
     """  # noqa: E501
 
     CONSTRAINT_GROUP = True
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def _create(self, group=None):
-        """Creates the linear constraint for the
-        :class:`oemof.solph.components.TransformerBlock` block.
+        """Creates the constraints for
+        :class:`oemof.solph.components.experimental._extraction_turbine_chp.ExtractionTurbineCHPBlock`.
 
         Parameters
         ----------
         group : list
-            List of :class:`oemof.solph.components.ExtractionTurbineCHP`
-            (trsf) objects for which the linear relation of inputs and outputs
-            is created e.g. group = [trsf1, trsf2, trsf3, ...]. Note that the
-            relation is created for all existing relations of the inputs and
-            all outputs of the transformer. The components inside the list need
-            to hold all needed attributes.
+            List of
+            :class:`oemof.solph.components.experimental._extraction_turbine_chp.ExtractionTurbineCHP`
+            (trsf) objects for which the linear relation of inputs
+            and outputs is created e.g. group = [trsf1, trsf2, trsf3, ...].
+            Note that the relation is created for all existing relations
+            of the inputs and all outputs of the transformer-like object.
+            The components inside the list need to hold all needed attributes.
         """
         if group is None:
             return None
 
         m = self.parent_block()
 
         for n in group:
@@ -215,41 +238,41 @@
                 )
                 / n.conversion_factors[n.tapped_output][t]
                 for t in m.TIMESTEPS
             ]
 
         def _input_output_relation_rule(block):
             """Connection between input, main output and tapped output."""
-            for t in m.TIMESTEPS:
+            for p, t in m.TIMEINDEX:
                 for g in group:
-                    lhs = m.flow[g.inflow, g, t]
+                    lhs = m.flow[g.inflow, g, p, t]
                     rhs = (
-                        m.flow[g, g.main_output, t]
-                        + m.flow[g, g.tapped_output, t]
+                        m.flow[g, g.main_output, p, t]
+                        + m.flow[g, g.tapped_output, p, t]
                         * g.main_flow_loss_index[t]
                     ) / g.conversion_factor_full_condensation_sq[t]
-                    block.input_output_relation.add((g, t), (lhs == rhs))
+                    block.input_output_relation.add((g, p, t), (lhs == rhs))
 
         self.input_output_relation = Constraint(
-            group, m.TIMESTEPS, noruleinit=True
+            group, m.TIMEINDEX, noruleinit=True
         )
         self.input_output_relation_build = BuildAction(
             rule=_input_output_relation_rule
         )
 
         def _out_flow_relation_rule(block):
             """Relation between main and tapped output in full chp mode."""
-            for t in m.TIMESTEPS:
+            for p, t in m.TIMEINDEX:
                 for g in group:
-                    lhs = m.flow[g, g.main_output, t]
+                    lhs = m.flow[g, g.main_output, p, t]
                     rhs = (
-                        m.flow[g, g.tapped_output, t]
+                        m.flow[g, g.tapped_output, p, t]
                         * g.flow_relation_index[t]
                     )
-                    block.out_flow_relation.add((g, t), (lhs >= rhs))
+                    block.out_flow_relation.add((g, p, t), (lhs >= rhs))
 
         self.out_flow_relation = Constraint(
-            group, m.TIMESTEPS, noruleinit=True
+            group, m.TIMEINDEX, noruleinit=True
         )
         self.out_flow_relation_build = BuildAction(
             rule=_out_flow_relation_rule
         )
```

### Comparing `oemof.solph-0.5.1.dev0/src/oemof/solph/components/_generic_chp.py` & `oemof.solph-0.5.1.dev1/src/oemof/solph/components/_generic_chp.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 SPDX-FileCopyrightText: Cord Kaldemeyer
 SPDX-FileCopyrightText: Patrik Schönfeldt
 SPDX-FileCopyrightText: FranziPl
 SPDX-FileCopyrightText: jnnr
 SPDX-FileCopyrightText: Stephan Günther
 SPDX-FileCopyrightText: FabianTU
 SPDX-FileCopyrightText: Johannes Röder
+SPDX-FileCopyrightText: Johannes Kochems
 
 SPDX-License-Identifier: MIT
 
 """
 
 import numpy as np
 from oemof.network import network
@@ -51,37 +52,39 @@
     Electric Power Systems Research (2007)
     Electric Power Systems Research
     Volume 78, Issue 5, May 2008, Pages 835-848
     https://doi.org/10.1016/j.epsr.2007.06.001
 
     Note
     ----
-    An adaption for the flow parameter `H_L_FG_share_max` has been made to
-    set the flue gas losses at maximum heat extraction `H_L_FG_max` as share of
-    the fuel flow `H_F` e.g. for combined cycle extraction turbines.
-    The flow parameter `H_L_FG_share_min` can be used to set the flue gas
-    losses at minimum heat extraction `H_L_FG_min` as share of
-    the fuel flow `H_F` e.g. for motoric CHPs.
-    The boolean component parameter `back_pressure` can be set to model
-    back-pressure characteristics.
+    * An adaption for the flow parameter `H_L_FG_share_max` has been made to
+      set the flue gas losses at maximum heat extraction `H_L_FG_max` as share
+      of the fuel flow `H_F` e.g. for combined cycle extraction turbines.
+    * The flow parameter `H_L_FG_share_min` can be used to set the flue gas
+      losses at minimum heat extraction `H_L_FG_min` as share of
+      the fuel flow `H_F` e.g. for motoric CHPs.
+    * The boolean component parameter `back_pressure` can be set to model
+      back-pressure characteristics.
 
     Also have a look at the examples on how to use it.
 
     Parameters
     ----------
     fuel_input : dict
-        Dictionary with key-value-pair of `oemof.Bus` and `oemof.Flow` object
-        for the fuel input.
+        Dictionary with key-value-pair of `oemof.solph.Bus` and
+        `oemof.solph.Flow` objects for the fuel input.
     electrical_output : dict
-        Dictionary with key-value-pair of `oemof.Bus` and `oemof.Flow` object
-        for the electrical output. Related parameters like `P_max_woDH` are
-        passed as attributes of the `oemof.Flow` object.
+        Dictionary with key-value-pair of `oemof.solph.Bus` and
+        `oemof.solph.Flow` objects for the electrical output.
+        Related parameters like `P_max_woDH` are passed as
+        attributes of the `oemof.Flow` object.
     heat_output : dict
-        Dictionary with key-value-pair of `oemof.Bus` and `oemof.Flow` object
-        for the heat output. Related parameters like `Q_CW_min` are passed as
+        Dictionary with key-value-pair of `oemof.solph.Bus`
+        and `oemof.solph.Flow` objects for the heat output.
+        Related parameters like `Q_CW_min` are passed as
         attributes of the `oemof.Flow` object.
     beta : list of numerical values
         beta values in same dimension as all other parameters (length of
         optimization period).
     back_pressure : boolean
         Flag to use back-pressure characteristics. Set to `True` and
         `Q_CW_min` to zero for back-pressure turbines. See paper above for more
@@ -330,45 +333,45 @@
             self.GENERICCHPS, m.TIMESTEPS, within=NonNegativeReals
         )
         self.P = Var(self.GENERICCHPS, m.TIMESTEPS, within=NonNegativeReals)
         self.Q = Var(self.GENERICCHPS, m.TIMESTEPS, within=NonNegativeReals)
         self.Y = Var(self.GENERICCHPS, m.TIMESTEPS, within=Binary)
 
         # constraint rules
-        def _H_flow_rule(block, n, t):
+        def _H_flow_rule(block, n, p, t):
             """Link fuel consumption to component inflow."""
             expr = 0
             expr += self.H_F[n, t]
-            expr += -m.flow[list(n.fuel_input.keys())[0], n, t]
+            expr += -m.flow[list(n.fuel_input.keys())[0], n, p, t]
             return expr == 0
 
         self.H_flow = Constraint(
-            self.GENERICCHPS, m.TIMESTEPS, rule=_H_flow_rule
+            self.GENERICCHPS, m.TIMEINDEX, rule=_H_flow_rule
         )
 
-        def _Q_flow_rule(block, n, t):
+        def _Q_flow_rule(block, n, p, t):
             """Link heat flow to component outflow."""
             expr = 0
             expr += self.Q[n, t]
-            expr += -m.flow[n, list(n.heat_output.keys())[0], t]
+            expr += -m.flow[n, list(n.heat_output.keys())[0], p, t]
             return expr == 0
 
         self.Q_flow = Constraint(
-            self.GENERICCHPS, m.TIMESTEPS, rule=_Q_flow_rule
+            self.GENERICCHPS, m.TIMEINDEX, rule=_Q_flow_rule
         )
 
-        def _P_flow_rule(block, n, t):
+        def _P_flow_rule(block, n, p, t):
             """Link power flow to component outflow."""
             expr = 0
             expr += self.P[n, t]
-            expr += -m.flow[n, list(n.electrical_output.keys())[0], t]
+            expr += -m.flow[n, list(n.electrical_output.keys())[0], p, t]
             return expr == 0
 
         self.P_flow = Constraint(
-            self.GENERICCHPS, m.TIMESTEPS, rule=_P_flow_rule
+            self.GENERICCHPS, m.TIMEINDEX, rule=_P_flow_rule
         )
 
         def _H_F_1_rule(block, n, t):
             """Set P_woDH depending on H_F."""
             expr = 0
             expr += -self.H_F[n, t]
             expr += n.alphas[0][t] * self.Y[n, t]
```

### Comparing `oemof.solph-0.5.1.dev0/src/oemof/solph/components/_offset_transformer.py` & `oemof.solph-0.5.1.dev1/src/oemof/solph/components/_offset_transformer.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 SPDX-FileCopyrightText: Cord Kaldemeyer
 SPDX-FileCopyrightText: Patrik Schönfeldt
 SPDX-FileCopyrightText: FranziPl
 SPDX-FileCopyrightText: jnnr
 SPDX-FileCopyrightText: Stephan Günther
 SPDX-FileCopyrightText: FabianTU
 SPDX-FileCopyrightText: Johannes Röder
+SPDX-FileCopyrightText: Johannes Kochems
 
 SPDX-License-Identifier: MIT
 
 """
 
 from oemof.network import network
 from pyomo.core.base.block import ScalarBlock
@@ -109,25 +110,25 @@
 
     **The following constraints are created:**
 
     .. _OffsetTransformer-equations:
 
     .. math::
         &
-        P_{out}(t) = C_1(t) \cdot P_{in}(t) + C_0(t) \cdot Y(t) \\
+        P_{out}(p, t) = C_1(t) \cdot P_{in}(p, t) + C_0(t) \cdot Y(t) \\
 
 
     The symbols used are defined as follows (with Variables (V) and Parameters (P)):
 
     +--------------------+------------------------+------+--------------------------------------------+
     | symbol             | attribute              | type | explanation                                |
     +====================+========================+======+============================================+
-    | :math:`P_{out}(t)` | `flow[n,o,t]`          | V    | Outflow of transformer                     |
+    | :math:`P_{out}(t)` | `flow[n,o,p,t]`        | V    | Outflow of transformer                     |
     +--------------------+------------------------+------+--------------------------------------------+
-    | :math:`P_{in}(t)`  | `flow[i,n,t]`          | V    | Inflow of transformer                      |
+    | :math:`P_{in}(t)`  | `flow[i,n,p,t]`        | V    | Inflow of transformer                      |
     +--------------------+------------------------+------+--------------------------------------------+
     | :math:`Y(t)`       | `status[i,n,t]`        | V    | Binary status variable of nonconvex inflow |
     +--------------------+------------------------+------+--------------------------------------------+
     | :math:`C_1(t)`     | `coefficients[1][n,t]` | P    | Linear coefficient 1 (slope)               |
     +--------------------+------------------------+------+--------------------------------------------+
     | :math:`C_0(t)`     | `coefficients[0][n,t]` | P    | Linear coefficient 0 (y-intersection)      |
     +--------------------+------------------------+------+--------------------------------------------+
@@ -152,23 +153,24 @@
         if group is None:
             return None
 
         m = self.parent_block()
 
         self.OFFSETTRANSFORMERS = Set(initialize=[n for n in group])
 
-        def _relation_rule(block, n, t):
+        def _relation_rule(block, n, p, t):
             """Link binary input and output flow to component outflow."""
             expr = 0
-            expr += -m.flow[n, list(n.outputs.keys())[0], t]
+            expr += -m.flow[n, list(n.outputs.keys())[0], p, t]
             expr += (
-                m.flow[list(n.inputs.keys())[0], n, t] * n.coefficients[1][t]
+                m.flow[list(n.inputs.keys())[0], n, p, t]
+                * n.coefficients[1][t]
             )
             expr += (
                 m.NonConvexFlowBlock.status[list(n.inputs.keys())[0], n, t]
                 * n.coefficients[0][t]
             )
             return expr == 0
 
         self.relation = Constraint(
-            self.OFFSETTRANSFORMERS, m.TIMESTEPS, rule=_relation_rule
+            self.OFFSETTRANSFORMERS, m.TIMEINDEX, rule=_relation_rule
         )
```

### Comparing `oemof.solph-0.5.1.dev0/src/oemof/solph/components/_sink.py` & `oemof.solph-0.5.1.dev1/src/oemof/solph/components/_sink.py`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/src/oemof/solph/components/_source.py` & `oemof.solph-0.5.1.dev1/src/oemof/solph/components/_source.py`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/src/oemof/solph/components/_transformer.py` & `oemof.solph-0.5.1.dev1/src/oemof/solph/components/_transformer.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 SPDX-FileCopyrightText: Patrik Schönfeldt
 SPDX-FileCopyrightText: Stephan Günther
 SPDX-FileCopyrightText: Birgit Schachler
 SPDX-FileCopyrightText: jnnr
 SPDX-FileCopyrightText: jmloenneberga
 SPDX-FileCopyrightText: David Fuhrländer
 SPDX-FileCopyrightText: Johannes Röder
+SPDX-FileCopyrightText: Johannes Kochems
 
 SPDX-License-Identifier: MIT
 
 """
 
 from oemof.network import network as on
 from pyomo.core import BuildAction
@@ -132,45 +133,51 @@
             self.conversion_factors[cf] = sequence(1)
 
     def constraint_group(self):
         return TransformerBlock
 
 
 class TransformerBlock(ScalarBlock):
-    r"""
-    Block for the linear relation of nodes with type
-    :class:`~oemof.solph.network.transformer.Transformer`
+    r"""Block for the linear relation of nodes with type
+    :class:`~oemof.solph.components._transformer.TransformerBlock`
+
+    **The following sets are created:** (-> see basic sets at
+    :class:`.Model` )
+
+    TRANSFORMERS
+        A set with all
+        :class:`~oemof.solph.components._transformer.Transformer` objects.
 
     **The following constraints are created:**
 
     Linear relation `om.Transformer.relation[i,o,t]`
         .. math::
-            P_{i}(t) \cdot \eta_{o}(t) =
-            P_{o}(t) \cdot \eta_{i}(t), \\
-            \forall t \in \textrm{TIMESTEPS}, \\
+            P_{i}(p, t) \cdot \eta_{o}(t) =
+            P_{o}(p, t) \cdot \eta_{i}(t), \\
+            \forall p, t \in \textrm{TIMEINDEX}, \\
             \forall i \in \textrm{INPUTS}, \\
             \forall o \in \textrm{OUTPUTS}
 
     While INPUTS is the set of Bus objects connected with the input of the
     Transformer and OUPUTS the set of Bus objects connected with the output of
     the Transformer. The constraint above will be created for all combinations
     of INPUTS and OUTPUTS for all TIMESTEPS. A Transformer with two inflows and
     two outflows for one day with an hourly resolution will lead to 96
     constraints.
 
     The index :math: n is the index for the Transformer node itself. Therefore,
-    a `flow[i, n, t]` is a flow from the Bus i to the Transformer n at
-    time step t.
+    a `flow[i, n, p, t]` is a flow from the Bus i to the Transformer n at
+    time index p, t.
 
     ======================  ============================  ====================
     symbol                  attribute                     explanation
     ======================  ============================  ====================
-    :math:`P_{i}(t)`        `flow[i, n, t]`               Transformer, inflow
+    :math:`P_{i,n}(p, t)`   `flow[i, n, p, t]`            Transformer, inflow
 
-    :math:`P_{o}(t)`        `flow[n, o, t]`               Transformer, outflow
+    :math:`P_{n,o}(p, t)`   `flow[n, o, p, t]`            Transformer, outflow
 
     :math:`\eta_{i}(t)`     `conversion_factor[i, n, t]`  Inflow, efficiency
 
     :math:`\eta_{o}(t)`     `conversion_factor[n, o, t]`  Outflow, efficiency
 
     ======================  ============================  ====================
 
@@ -201,40 +208,40 @@
         m = self.parent_block()
 
         in_flows = {n: [i for i in n.inputs.keys()] for n in group}
         out_flows = {n: [o for o in n.outputs.keys()] for n in group}
 
         self.relation = Constraint(
             [
-                (n, i, o, t)
-                for t in m.TIMESTEPS
+                (n, i, o, p, t)
+                for p, t in m.TIMEINDEX
                 for n in group
                 for o in out_flows[n]
                 for i in in_flows[n]
             ],
             noruleinit=True,
         )
 
         def _input_output_relation(block):
-            for t in m.TIMESTEPS:
+            for p, t in m.TIMEINDEX:
                 for n in group:
                     for o in out_flows[n]:
                         for i in in_flows[n]:
                             try:
                                 lhs = (
-                                    m.flow[i, n, t]
+                                    m.flow[i, n, p, t]
                                     * n.conversion_factors[o][t]
                                 )
                                 rhs = (
-                                    m.flow[n, o, t]
+                                    m.flow[n, o, p, t]
                                     * n.conversion_factors[i][t]
                                 )
                             except ValueError:
                                 raise ValueError(
                                     "Error in constraint creation",
                                     "source: {0}, target: {1}".format(
                                         n.label, o.label
                                     ),
                                 )
-                            block.relation.add((n, i, o, t), (lhs == rhs))
+                            block.relation.add((n, i, o, p, t), (lhs == rhs))
 
         self.relation_build = BuildAction(rule=_input_output_relation)
```

### Comparing `oemof.solph-0.5.1.dev0/src/oemof/solph/components/experimental/__init__.py` & `oemof.solph-0.5.1.dev1/src/oemof/solph/components/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/src/oemof/solph/components/experimental/_generic_caes.py` & `oemof.solph-0.5.1.dev1/src/oemof/solph/components/experimental/_generic_caes.py`

 * *Files 2% similar despite different names*

```diff
@@ -301,21 +301,21 @@
         filling level of TES"
         ":math:`CAS_{fil\_max}`", "`cav_level_max[n,t]`", "P", "Max.
         filling level of TES"
         ":math:`\tau`", "`cav_eta_tmp[n,t]`", "P", "
         | Temporal efficiency
         | (loss factor to take intertemporal losses into account)"
         ":math:`electrical\_input`", "
-        `flow[list(n.electrical_input.keys())[0], n, t]`", "P", "
+        `flow[list(n.electrical_input.keys())[0], p, n, t]`", "P", "
         Electr. power input into compression"
         ":math:`electrical\_output`", "
-        `flow[n, list(n.electrical_output.keys())[0], t]`", "P", "
+        `flow[n, list(n.electrical_output.keys())[0], p, t]`", "P", "
         Electr. power output of expansion"
         ":math:`fuel\_input`", "
-        `flow[list(n.fuel_input.keys())[0], n, t]`", "P", "Heat input
+        `flow[list(n.fuel_input.keys())[0], n, p, t]`", "P", "Heat input
         (external) into Expansion"
 
     """
 
     CONSTRAINT_GROUP = True
 
     def __init__(self, *args, **kwargs):
@@ -426,22 +426,22 @@
 
         # Spot market: Negative capacity
         self.cmp_p_spot = Var(
             self.GENERICCAES, m.TIMESTEPS, within=NonNegativeReals
         )
 
         # Compression: Capacity on markets
-        def cmp_p_constr_rule(block, n, t):
+        def cmp_p_constr_rule(block, n, p, t):
             expr = 0
             expr += -self.cmp_p[n, t]
-            expr += m.flow[list(n.electrical_input.keys())[0], n, t]
+            expr += m.flow[list(n.electrical_input.keys())[0], n, p, t]
             return expr == 0
 
         self.cmp_p_constr = Constraint(
-            self.GENERICCAES, m.TIMESTEPS, rule=cmp_p_constr_rule
+            self.GENERICCAES, m.TIMEINDEX, rule=cmp_p_constr_rule
         )
 
         # Compression: Max. capacity depending on cavern filling level
         def cmp_p_max_constr_rule(block, n, t):
             if t != 0:
                 return (
                     self.cmp_p_max[n, t]
@@ -516,22 +516,22 @@
             ] == self.tes_e_in[n, t] * (1 - n.params["cmp_q_tes_share"])
 
         self.cmp_q_out_shr_constr = Constraint(
             self.GENERICCAES, m.TIMESTEPS, rule=cmp_q_out_shr_constr_rule
         )
 
         # (10) Expansion: Capacity on markets
-        def exp_p_constr_rule(block, n, t):
+        def exp_p_constr_rule(block, n, p, t):
             expr = 0
             expr += -self.exp_p[n, t]
-            expr += m.flow[n, list(n.electrical_output.keys())[0], t]
+            expr += m.flow[n, list(n.electrical_output.keys())[0], p, t]
             return expr == 0
 
         self.exp_p_constr = Constraint(
-            self.GENERICCAES, m.TIMESTEPS, rule=exp_p_constr_rule
+            self.GENERICCAES, m.TIMEINDEX, rule=exp_p_constr_rule
         )
 
         # (11-12) Expansion: Max. capacity depending on cavern filling level
         def exp_p_max_constr_rule(block, n, t):
             if t != 0:
                 return (
                     self.exp_p_max[n, t]
@@ -587,22 +587,22 @@
             )
 
         self.exp_q_in_constr = Constraint(
             self.GENERICCAES, m.TIMESTEPS, rule=exp_q_in_constr_rule
         )
 
         # (17) Expansion: Fuel allocation
-        def exp_q_fuel_constr_rule(block, n, t):
+        def exp_q_fuel_constr_rule(block, n, p, t):
             expr = 0
             expr += -self.exp_q_fuel_in[n, t]
-            expr += m.flow[list(n.fuel_input.keys())[0], n, t]
+            expr += m.flow[list(n.fuel_input.keys())[0], n, p, t]
             return expr == 0
 
         self.exp_q_fuel_constr = Constraint(
-            self.GENERICCAES, m.TIMESTEPS, rule=exp_q_fuel_constr_rule
+            self.GENERICCAES, m.TIMEINDEX, rule=exp_q_fuel_constr_rule
         )
 
         # (18) Expansion: Definition of single heat flows
         def exp_q_in_sum_constr_rule(block, n, t):
             return (
                 self.exp_q_in_sum[n, t]
                 == self.exp_q_fuel_in[n, t]
```

### Comparing `oemof.solph-0.5.1.dev0/src/oemof/solph/components/experimental/_link.py` & `oemof.solph-0.5.1.dev1/src/oemof/solph/components/experimental/_link.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 SPDX-FileCopyrightText: Simon Hilpert
 SPDX-FileCopyrightText: Cord Kaldemeyer
 SPDX-FileCopyrightText: Patrik Schönfeldt
 SPDX-FileCopyrightText: Johannes Röder
 SPDX-FileCopyrightText: jakob-wo
 SPDX-FileCopyrightText: gplssm
 SPDX-FileCopyrightText: jnnr
+SPDX-FileCopyrightText: Johannes Kochems
 
 SPDX-License-Identifier: MIT
 
 """
 from warnings import warn
 
 from oemof.network import network as on
@@ -25,15 +26,15 @@
 from pyomo.environ import BuildAction
 from pyomo.environ import Constraint
 
 from oemof.solph._plumbing import sequence
 
 
 class Link(on.Transformer):
-    """A Link object with 1...2 inputs and 1...2 outputs.
+    """A Link object with 2 inputs and 2 outputs.
 
     Parameters
     ----------
     conversion_factors : dict
         Dictionary containing conversion factors for conversion of each flow.
         Keys are the connected tuples (input, output) bus objects.
         The dictionary values can either be a scalar or an iterable with length
@@ -109,15 +110,16 @@
 
     **The following constraints are created:**
 
     .. _Link-equations:
 
     .. math::
         &
-        (1) \qquad P_{\mathrm{in},n}(t) = c_n(t) \times P_{\mathrm{out},n}(t)
+        (1) \qquad P_{\mathrm{in},n}(p, t) = c_n(t)
+        \times P_{\mathrm{out},n}(p, t)
             \quad \forall t \in T, \forall n in {1,2} \\
         &
 
     """
     CONSTRAINT_GROUP = True
 
     def __init__(self, *args, **kwargs):
@@ -145,34 +147,34 @@
             all_conversions[n] = {
                 k: v for k, v in n.conversion_factors.items()
             }
 
         self.LINKS = Set(initialize=[g for g in group])
 
         def _input_output_relation(block):
-            for t in m.TIMESTEPS:
+            for p, t in m.TIMEINDEX:
                 for n, conversion in all_conversions.items():
                     for cidx, c in conversion.items():
                         try:
                             expr = (
-                                m.flow[n, cidx[1], t]
-                                == c[t] * m.flow[cidx[0], n, t]
+                                m.flow[n, cidx[1], p, t]
+                                == c[t] * m.flow[cidx[0], n, p, t]
                             )
                         except ValueError:
                             raise ValueError(
                                 "Error in constraint creation",
                                 "from: {0}, to: {1}, via: {2}".format(
                                     cidx[0], cidx[1], n
                                 ),
                             )
-                        block.relation.add((n, cidx[0], cidx[1], t), (expr))
+                        block.relation.add((n, cidx[0], cidx[1], p, t), expr)
 
         self.relation = Constraint(
             [
-                (n, cidx[0], cidx[1], t)
-                for t in m.TIMESTEPS
+                (n, cidx[0], cidx[1], p, t)
+                for p, t in m.TIMEINDEX
                 for n, conversion in all_conversions.items()
                 for cidx, c in conversion.items()
             ],
             noruleinit=True,
         )
         self.relation_build = BuildAction(rule=_input_output_relation)
```

### Comparing `oemof.solph-0.5.1.dev0/src/oemof/solph/components/experimental/_piecewise_linear_transformer.py` & `oemof.solph-0.5.1.dev1/src/oemof/solph/components/experimental/_piecewise_linear_transformer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # -*- coding: utf-8 -*-
 
 """
-In-development transfomer with piecewise linar efficiencies.
+In-development transformer with piecewise linear efficiencies.
 
 SPDX-FileCopyrightText: Uwe Krien <krien@uni-bremen.de>
 SPDX-FileCopyrightText: Simon Hilpert
 SPDX-FileCopyrightText: Cord Kaldemeyer
 SPDX-FileCopyrightText: Patrik Schönfeldt
 SPDX-FileCopyrightText: Johannes Röder
 SPDX-FileCopyrightText: jakob-wo
 SPDX-FileCopyrightText: gplssm
 SPDX-FileCopyrightText: jnnr
+SPDX-FileCopyrightText: Johannes Kochems
 
 SPDX-License-Identifier: MIT
 
 """
 
 from oemof.network import network as on
 from pyomo.core.base.block import ScalarBlock
@@ -121,15 +122,15 @@
         self.PWLINEARTRANSFORMERS = Set(initialize=[n for n in group])
 
         pw_repns = [n.pw_repn for n in group]
         if all(x == pw_repns[0] for x in pw_repns):
             self.pw_repn = pw_repns[0]
         else:
             print(
-                "Cannot different piecewise representations ",
+                "Cannot model different piecewise representations ",
                 [n.pw_repn for n in group],
             )
 
         self.breakpoints = {}
 
         def build_breakpoints(block, n):
             for t in m.TIMESTEPS:
@@ -164,34 +165,34 @@
         self.inflow = Var(
             self.PWLINEARTRANSFORMERS, m.TIMESTEPS, bounds=get_inflow_bounds
         )
         self.outflow = Var(
             self.PWLINEARTRANSFORMERS, m.TIMESTEPS, bounds=get_outflow_bounds
         )
 
-        def _in_equation(block, n, t):
+        def _in_equation(block, n, p, t):
             """Link binary input and output flow to component outflow."""
             expr = 0
-            expr += -m.flow[list(n.inputs.keys())[0], n, t]
+            expr += -m.flow[list(n.inputs.keys())[0], n, p, t]
             expr += self.inflow[n, t]
             return expr == 0
 
         self.equate_in = Constraint(
-            self.PWLINEARTRANSFORMERS, m.TIMESTEPS, rule=_in_equation
+            self.PWLINEARTRANSFORMERS, m.TIMEINDEX, rule=_in_equation
         )
 
-        def _out_equation(block, n, t):
+        def _out_equation(block, n, p, t):
             """Link binary input and output flow to component outflow."""
             expr = 0
-            expr += -m.flow[n, list(n.outputs.keys())[0], t]
+            expr += -m.flow[n, list(n.outputs.keys())[0], p, t]
             expr += self.outflow[n, t]
             return expr == 0
 
         self.equate_out = Constraint(
-            self.PWLINEARTRANSFORMERS, m.TIMESTEPS, rule=_out_equation
+            self.PWLINEARTRANSFORMERS, m.TIMEINDEX, rule=_out_equation
         )
 
         self.piecewise = Piecewise(
             self.PWLINEARTRANSFORMERS,
             m.TIMESTEPS,
             self.outflow,
             self.inflow,
```

### Comparing `oemof.solph-0.5.1.dev0/src/oemof/solph/components/experimental/_sink_dsm.py` & `oemof.solph-0.5.1.dev1/src/oemof/solph/components/experimental/_sink_dsm.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,22 +13,25 @@
 SPDX-FileCopyrightText: Cord Kaldemeyer
 SPDX-FileCopyrightText: Patrik Schönfeldt
 SPDX-FileCopyrightText: Johannes Röder
 SPDX-FileCopyrightText: jakob-wo
 SPDX-FileCopyrightText: gplssm
 SPDX-FileCopyrightText: jnnr
 SPDX-FileCopyrightText: Julian Endres
-SPDX-FileCopyrightText: Johannes Kochems (jokochems)
+SPDX-FileCopyrightText: Johannes Kochems
 
 SPDX-License-Identifier: MIT
 
 """
 import itertools
+from warnings import warn
 
 from numpy import mean
+from oemof.tools import debugging
+from oemof.tools import economics
 from pyomo.core.base.block import ScalarBlock
 from pyomo.environ import BuildAction
 from pyomo.environ import Constraint
 from pyomo.environ import Expression
 from pyomo.environ import NonNegativeReals
 from pyomo.environ import Set
 from pyomo.environ import Var
@@ -83,18 +86,18 @@
     Parameters
     ----------
     demand: numeric
         original electrical demand (normalized)
         For investment modeling, it is advised to use the maximum of the
         demand timeseries and the cumulated (fixed) infeed time series
         for normalization, because the balancing potential may be determined by
-        both. Elsewhise, underinvestments may occur.
-    capacity_up: int or array
+        both. Else, underinvestments may occur.
+    capacity_up: int or iterable
         maximum DSM capacity that may be increased (normalized)
-    capacity_down: int or array
+    capacity_down: int or iterable
         maximum DSM capacity that may be reduced (normalized)
     approach: str, one of 'oemof', 'DIW', 'DLR'
         Choose one of the DSM modeling approaches. Read notes about which
         parameters to be applied for which approach.
 
         oemof :
 
@@ -125,50 +128,45 @@
             :class:`~SinkDSMDLRBlock` resp.
             :class:`~SinkDSMDLRInvestmentBlock`.
     shift_interval: int
         Only used when `approach` is set to "oemof". Otherwise, can be
         None.
         It's the interval in which between :math:`DSM_{t}^{up}` and
         :math:`DSM_{t}^{down}` have to be compensated.
-    delay_time: int
-        Only used when `approach` is set to "DIW" or "DLR". Otherwise,
-        can be None.
+    delay_time: int or iterable
+        Only used when :attr:`~approach` is set to "DIW" or "DLR". Otherwise,
+        can be None. Iterable only allowed in case approach "DLR" is used.
         Length of symmetrical time windows around :math:`t` in which
         :math:`DSM_{t}^{up}` and :math:`DSM_{t,tt}^{down}` have to be
         compensated.
-        Note: For approach 'DLR', an iterable is constructed in order
-        to model flexible delay times
+        Note: For approach 'DLR', if an integer is passed,
+        an iterable is constructed in order to model flexible delay times.
+        In case an iterable is passed, this will be used directly.
     shift_time: int
         Only used when `approach` is set to "DLR".
         Duration of a single upwards or downwards shift (half a shifting cycle
         if there is immediate compensation)
     shed_time: int
         Only used when `shed_eligibility` is set to True.
         Maximum length of a load shedding process at full capacity
         (used within energy limit constraint)
-    max_demand: numeric
-        Maximum demand prior to demand response
+    max_demand: numeric or iterable
+        Maximum demand prior to demand response (per period)
     max_capacity_down: numeric
         Maximum capacity eligible for downshifts
-        prior to demand response (used for dispatch mode)
+        prior to demand response (used only for dispatch mode)
     max_capacity_up: numeric
         Maximum capacity eligible for upshifts
-        prior to demand response (used for dispatch mode)
-    flex_share_down: float
-        Flexible share of installed capacity
-        eligible for downshifts (used for invest mode)
-    flex_share_up: float
-        Flexible share of installed capacity
-        eligible for upshifts (used for invest mode)
-    cost_dsm_up : int
+        prior to demand response (used only for dispatch mode)
+    cost_dsm_up : float
         Cost per unit of DSM activity that increases the demand
-    cost_dsm_down_shift : int
+    cost_dsm_down_shift : float
         Cost per unit of DSM activity that decreases the demand
         for load shifting
-    cost_dsm_down_shed : int
+    cost_dsm_down_shed : float
         Cost per unit of DSM activity that decreases the demand
         for load shedding
     efficiency : float
         Efficiency factor for load shifts (between 0 and 1)
     recovery_time_shift : int
         Only used when `approach` is set to "DIW".
         Minimum time between the end of one load shifting process
@@ -209,24 +207,20 @@
         within the optimization timeframe
     shed_eligibility : boolean
         Boolean parameter indicating whether unit is eligible for
         load shedding
     shift_eligibility : boolean
         Boolean parameter indicating whether unit is eligible for
         load shifting
+    fixed_costs : numeric
+        Nominal value of fixed costs (per period)
 
     Note
     ----
 
-    * When you set up a dispatch model, you have to specify `max_capacity_up`,
-      `max_capacity_down` and `max_demand`. Don't set `flex_share_up`
-      and `flex_share_down` which shall only used for investment modeling.
-    * When using the investment mode, you have to specify `flex_share_up`
-      and `flex_share_down` instead of `max_capacity_up`,
-      `max_capacity_down` and `max_demand`.
     * `method` has been renamed to `approach`.
     * As many constraints and dependencies are created in approach "DIW",
       computational cost might be high with a large `delay_time` and with model
       of high temporal resolution.
     * The approach "DLR" preforms better in terms of calculation time,
       compared to the approach "DIW".
     * Using `approach` "DIW" or "DLR" might result in demand shifts that
@@ -255,16 +249,14 @@
         shift_interval=None,
         delay_time=None,
         shift_time=None,
         shed_time=None,
         max_demand=None,
         max_capacity_down=None,
         max_capacity_up=None,
-        flex_share_down=None,
-        flex_share_up=None,
         cost_dsm_up=0,
         cost_dsm_down_shift=0,
         cost_dsm_down_shed=0,
         efficiency=1,
         recovery_time_shift=None,
         recovery_time_shed=None,
         ActivateYearLimit=False,
@@ -272,14 +264,15 @@
         n_yearLimit_shift=None,
         n_yearLimit_shed=None,
         t_dayLimit=None,
         addition=True,
         fixes=True,
         shed_eligibility=True,
         shift_eligibility=True,
+        fixed_costs=0,
         investment=None,
         custom_attributes=None,
     ):
         if custom_attributes is None:
             custom_attributes = {}
         super().__init__(
             label=label, inputs=inputs, custom_attributes=custom_attributes
@@ -287,75 +280,31 @@
 
         self.capacity_up = sequence(capacity_up)
         self.capacity_down = sequence(capacity_down)
         self.demand = sequence(demand)
         self.approach = approach
         self.shift_interval = shift_interval
         if not approach == "DLR":
+            if approach == "DIW":
+                if not isinstance(delay_time, int):
+                    raise ValueError(
+                        "If approach 'DIW' is used, "
+                        "delay time has to be of type int."
+                    )
             self.delay_time = delay_time
         else:
-            self.delay_time = [el for el in range(1, delay_time + 1)]
+            if isinstance(delay_time, int):
+                self.delay_time = [el for el in range(1, delay_time + 1)]
+            else:
+                self.delay_time = delay_time
         self.shift_time = shift_time
         self.shed_time = shed_time
-
-        # Attributes are only needed if no investments occur
         self.max_capacity_down = max_capacity_down
         self.max_capacity_up = max_capacity_up
-        self.max_demand = max_demand
-
-        # Attributes for investment modeling
-        if flex_share_down is not None:
-            if max_capacity_down is None and max_demand is None:
-                self.flex_share_down = flex_share_down
-            else:
-                e1 = (
-                    "Please determine either **flex_share_down "
-                    "(investment modeling)\n or set "
-                    "**max_demand and **max_capacity_down "
-                    "(dispatch modeling).\n"
-                    "Otherwise, overdetermination occurs."
-                )
-                raise AttributeError(e1)
-        else:
-            if max_capacity_down is None or max_demand is None:
-                e2 = (
-                    "If you do not specify **flex_share_down\n"
-                    "which should be used for investment modeling,\n"
-                    "you have to specify **max_capacity_down "
-                    "and **max_demand\n"
-                    "instead which should be used for dispatch modeling."
-                )
-                raise AttributeError(e2)
-            else:
-                self.flex_share_down = self.max_capacity_down / self.max_demand
-
-        if flex_share_up is not None:
-            if max_capacity_up is None and max_demand is None:
-                self.flex_share_up = flex_share_up
-            else:
-                e3 = (
-                    "Please determine either flex_share_up "
-                    "(investment modeling)\n or set "
-                    "max_demand and max_capacity_up (dispatch modeling).\n"
-                    "Otherwise, overdetermination occurs."
-                )
-                raise AttributeError(e3)
-        else:
-            if max_capacity_up is None or max_demand is None:
-                e4 = (
-                    "If you do not specify **flex_share_up\n"
-                    "which should be used for investment modeling,\n"
-                    "you have to specify **max_capacity_up "
-                    "and **max_demand\n"
-                    "instead which should be used for dispatch modeling."
-                )
-                raise AttributeError(e4)
-            else:
-                self.flex_share_up = self.max_capacity_up / self.max_demand
-
+        self.max_demand = sequence(max_demand)
         self.cost_dsm_up = sequence(cost_dsm_up)
         self.cost_dsm_down_shift = sequence(cost_dsm_down_shift)
         self.cost_dsm_down_shed = sequence(cost_dsm_down_shed)
         self.efficiency = efficiency
         self.capacity_down_mean = mean(capacity_down)
         self.capacity_up_mean = mean(capacity_up)
         self.recovery_time_shift = recovery_time_shift
@@ -365,76 +314,68 @@
         self.n_yearLimit_shift = n_yearLimit_shift
         self.n_yearLimit_shed = n_yearLimit_shed
         self.t_dayLimit = t_dayLimit
         self.addition = addition
         self.fixes = fixes
         self.shed_eligibility = shed_eligibility
         self.shift_eligibility = shift_eligibility
+        self.fixed_costs = sequence(fixed_costs)
 
         # Check whether investment mode is active or not
         self.investment = investment
         self._invest_group = isinstance(self.investment, Investment)
 
         if (
-            self.max_demand is None
-            or self.max_capacity_up is None
-            or self.max_capacity_down is None
+            self.max_capacity_up is None or self.max_capacity_down is None
         ) and not self._invest_group:
-            e5 = (
-                "If you are setting up a dispatch model, "
-                "you have to specify **max_demand**, **max_capacity_up** "
-                "and **max_capacity_down**.\n"
-                "The values you might have passed for **flex_share_up** "
-                "and **flex_share_down** will be ignored and only used in "
-                "an investment model."
+            e1 = (
+                "If you are using the dispatch mode, "
+                "you have to specify `max_capacity_up` "
+                "and `max_capacity_down`."
             )
-            raise AttributeError(e5)
+            raise AttributeError(e1)
 
         if self._invest_group:
             self._check_invest_attributes()
 
     def _check_invest_attributes(self):
         if (
-            self.investment is not None
-            and (
-                self.max_demand
-                or self.max_capacity_down
-                or self.max_capacity_up
-            )
-            is not None
-        ):
-            e6 = (
-                "If an investment object is defined, the invest variable "
-                "replaces the **max_demand, the **max_capacity_down "
-                "as well as\n"
-                "the **max_capacity_up values. Therefore, **max_demand,\n"
-                "**max_capacity_up and **max_capacity_down values should be "
-                "'None'.\n"
+            self.max_capacity_down or self.max_capacity_up
+        ) and self.investment is not None:
+            e2 = (
+                "If you are using the investment mode, the invest variable "
+                "replaces the `max_capacity_down` "
+                "as well as the `max_capacity_up` values.\n"
+                "Therefore, `max_capacity_up` and `max_capacity_down` "
+                "values should be None (which is their default value)."
             )
-            raise AttributeError(e6)
+            raise AttributeError(e2)
 
     def constraint_group(self):
         possible_approaches = ["DIW", "DLR", "oemof"]
 
-        if self.approach in [possible_approaches[0], possible_approaches[1]]:
-            if self.delay_time is None:
+        if not self.shed_eligibility and not self.shift_eligibility:
+            raise ValueError(
+                "At least one of shed_eligibility"
+                " and shift_eligibility must be True"
+            )
+        if self.shed_eligibility:
+            if self.recovery_time_shed is None:
                 raise ValueError(
-                    "Please define: **delay_time" " is a mandatory parameter"
+                    "If unit is eligible for load shedding,"
+                    " recovery_time_shed must be defined"
                 )
-            if not self.shed_eligibility and not self.shift_eligibility:
+
+        if self.approach in [possible_approaches[0], possible_approaches[1]]:
+            if self.delay_time is None:
                 raise ValueError(
-                    "At least one of **shed_eligibility"
-                    " and **shift_eligibility must be True"
+                    f"Please define: delay_time.\n"
+                    f"It is a mandatory parameter when using"
+                    f" approach {self.approach}."
                 )
-            if self.shed_eligibility:
-                if self.recovery_time_shed is None:
-                    raise ValueError(
-                        "If unit is eligible for load shedding,"
-                        " **recovery_time_shed must be defined"
-                    )
 
         if self.approach == possible_approaches[0]:
             if self._invest_group is True:
                 return SinkDSMDIWInvestmentBlock
             else:
                 return SinkDSMDIWBlock
 
@@ -443,16 +384,17 @@
                 return SinkDSMDLRInvestmentBlock
             else:
                 return SinkDSMDLRBlock
 
         elif self.approach == possible_approaches[2]:
             if self.shift_interval is None:
                 raise ValueError(
-                    "Please define: **shift_interval"
-                    " is a mandatory parameter"
+                    f"Please define: shift_interval.\n"
+                    f"It is a mandatory parameter when using"
+                    f" approach {self.approach}."
                 )
             if self._invest_group is True:
                 return SinkDSMOemofInvestmentBlock
             else:
                 return SinkDSMOemofBlock
         else:
             raise ValueError(
@@ -507,36 +449,36 @@
         + DSM_{t}^{do, shift} \cdot cost_{t}^{dsm, do, shift}
         + DSM_{t}^{do, shed} \cdot cost_{t}^{dsm, do, shed})
         \cdot \omega_{t} \\
         & \quad \quad \quad \quad \forall t \in \mathbb{T} \\
 
     **Table: Symbols and attribute names of variables and parameters**
 
-    .. table:: Variables (V) and Parameters (P)
-        :widths: 1, 1, 1, 1
+    .. table:: Variables (V), Parameters (P) and Sets (S)
+        :widths: 25, 25, 10, 40
 
         ================================= ======================== ==== =======================================
         symbol                            attribute                type explanation
         ================================= ======================== ==== =======================================
         :math:`DSM_{t}^{up}`              `dsm_up[g, t]`           V    DSM up shift (capacity shifted upwards)
         :math:`DSM_{t}^{do, shift}`       `dsm_do_shift[g, t]`     V    DSM down shift (capacity shifted downwards)
         :math:`DSM_{t}^{do, shed}`        `dsm_do_shed[g, t]`      V    DSM shedded (capacity shedded, i.e. not compensated for)
         :math:`\dot{E}_{t}`               `SinkDSM.inputs`         V    Energy flowing in from (electrical) inflow bus
-        :math:`demand_{t}`                `demand[t]`              P    (Electrical) demand series (normalized)
-        :math:`demand_{max}`              `max_demand`             P    Maximum demand value
+        :math:`demand_{t}`                `demand[t]`              P    (Electrical) demand series before shifting (normalized)
+        :math:`demand_{max}(p)`           `max_demand`             P    Maximum demand value in period p
         :math:`E_{t}^{do}`                `capacity_down[t]`       P    | Capacity  allowed for a load adjustment downwards
                                                                         | (normalized; shifting + shedding)
         :math:`E_{t}^{up}`                `capacity_up[t]`         P    Capacity allowed for a shift upwards (normalized)
         :math:`E_{do, max}`               `max_capacity_down`      P    | Maximum capacity allowed for a load adjustment downwards
                                                                         | (shifting + shedding)
         :math:`E_{up, max}`               `max_capacity_up`        P    Maximum capacity allowed for a shift upwards
         :math:`\tau`                      `shift_interval`         P    | interval (time within which the
                                                                         | energy balance must be levelled out)
         :math:`\eta`                      `efficiency`             P    Efficiency for load shifting processes
-        :math:`\mathbb{T}`                                         P    Time steps of the model
+        :math:`\mathbb{T}`                                         S    Time steps of the model
         :math:`e_{shift}`                 `shift_eligibility`      P    | Boolean parameter indicating if unit can be used
                                                                         | for load shifting
         :math:`e_{shed}`                  `shed_eligibility`       P    | Boolean parameter indicating if unit can be used
                                                                         | for load shedding
         :math:`cost_{t}^{dsm, up}`        `cost_dsm_up[t]`         P    Variable costs for an upwards shift
         :math:`cost_{t}^{dsm, do, shift}` `cost_dsm_down_shift[t]` P    Variable costs for a downwards shift (load shifting)
         :math:`cost_{t}^{dsm, do, shed}`  `cost_dsm_down_shift[t]` P    Variable costs for shedding load
@@ -607,32 +549,32 @@
 
         # Demand Production Relation
         def _input_output_relation_rule(block):
             """Relation between input data and pyomo variables.
             The actual demand after DSM.
             Generator Production == Demand_el +- DSM
             """
-            for t in m.TIMESTEPS:
+            for p, t in m.TIMEINDEX:
                 for g in group:
                     # Inflow from bus
-                    lhs = m.flow[g.inflow, g, t]
+                    lhs = m.flow[g.inflow, g, p, t]
 
                     # Demand + DSM_up - DSM_down
                     rhs = (
-                        g.demand[t] * g.max_demand
+                        g.demand[t] * g.max_demand[p]
                         + self.dsm_up[g, t]
                         - self.dsm_do_shift[g, t]
                         - self.dsm_do_shed[g, t]
                     )
 
                     # add constraint
-                    block.input_output_relation.add((g, t), (lhs == rhs))
+                    block.input_output_relation.add((g, p, t), (lhs == rhs))
 
         self.input_output_relation = Constraint(
-            group, m.TIMESTEPS, noruleinit=True
+            group, m.TIMEINDEX, noruleinit=True
         )
         self.input_output_relation_build = BuildAction(
             rule=_input_output_relation_rule
         )
 
         # Upper bounds relation
         def dsm_up_constraint_rule(block):
@@ -680,20 +622,20 @@
             """Relation to compensate the total amount of positive
             and negative DSM in between the shift_interval.
             This constraint is building balance in full intervals starting
             with index 0. The last interval might not be full.
             """
             for g in group:
                 intervals = range(
-                    m.TIMESTEPS[1], m.TIMESTEPS[-1], g.shift_interval
+                    m.TIMESTEPS.at(1), m.TIMESTEPS.at(-1), g.shift_interval
                 )
 
                 for interval in intervals:
-                    if (interval + g.shift_interval - 1) > m.TIMESTEPS[-1]:
-                        timesteps = range(interval, m.TIMESTEPS[-1] + 1)
+                    if (interval + g.shift_interval - 1) > m.TIMESTEPS.at(-1):
+                        timesteps = range(interval, m.TIMESTEPS.at(-1) + 1)
                     else:
                         timesteps = range(
                             interval, interval + g.shift_interval
                         )
 
                     # DSM up/down
                     lhs = (
@@ -714,121 +656,198 @@
         )
 
     def _objective_expression(self):
         r"""Objective expression with variable costs for DSM activity"""
 
         m = self.parent_block()
 
-        dsm_cost = 0
+        variable_costs = 0
+        fixed_costs = 0
+
+        if m.es.periods is None:
+            for t in m.TIMESTEPS:
+                for g in self.dsm:
+                    variable_costs += (
+                        self.dsm_up[g, t]
+                        * g.cost_dsm_up[t]
+                        * m.objective_weighting[t]
+                    )
+                    variable_costs += (
+                        self.dsm_do_shift[g, t] * g.cost_dsm_down_shift[t]
+                        + self.dsm_do_shed[g, t] * g.cost_dsm_down_shed[t]
+                    ) * m.objective_weighting[t]
 
-        for t in m.TIMESTEPS:
+        else:
             for g in self.dsm:
-                dsm_cost += (
-                    self.dsm_up[g, t]
-                    * g.cost_dsm_up[t]
-                    * m.objective_weighting[t]
-                )
-                dsm_cost += (
-                    self.dsm_do_shift[g, t] * g.cost_dsm_down_shift[t]
-                    + self.dsm_do_shed[g, t] * g.cost_dsm_down_shed[t]
-                ) * m.objective_weighting[t]
+                for p, t in m.TIMEINDEX:
+                    variable_costs += (
+                        self.dsm_up[g, t]
+                        * m.objective_weighting[t]
+                        * g.cost_dsm_up[t]
+                        * ((1 + m.discount_rate) ** -m.es.periods_years[p])
+                    )
+                    variable_costs += (
+                        (
+                            self.dsm_do_shift[g, t] * g.cost_dsm_down_shift[t]
+                            + self.dsm_do_shed[g, t] * g.cost_dsm_down_shed[t]
+                        )
+                        * m.objective_weighting[t]
+                        * ((1 + m.discount_rate) ** -m.es.periods_years[p])
+                    )
 
-        self.cost = Expression(expr=dsm_cost)
+                if g.fixed_costs[0] is not None:
+                    for p in m.PERIODS:
+                        fixed_costs += (
+                            max(g.max_capacity_up, g.max_capacity_down)
+                            * g.fixed_costs[p]
+                            * ((1 + m.discount_rate) ** -m.es.periods_years[p])
+                        )
+
+        self.variable_costs = Expression(expr=variable_costs)
+        self.fixed_costs = Expression(expr=fixed_costs)
+        self.costs = Expression(expr=variable_costs + fixed_costs)
 
-        return self.cost
+        return self.costs
 
 
 class SinkDSMOemofInvestmentBlock(ScalarBlock):
     r"""Constraints for SinkDSM with "oemof" approach and `investment`
     defined
 
     **The following constraints are created for approach = "oemof"
     with an investment object defined:**
 
     .. _SinkDSMOemofInvestmentBlock equations:
 
     .. math::
         &
-        (1) \quad invest_{min} \leq invest \leq invest_{max} \\
+        (1) \quad invest_{min}(p) \leq invest(p) \leq invest_{max}(p) \\
+        & \quad \quad \quad \quad \forall p \in \mathbb{P}
         & \\
         &
         (2) \quad DSM_{t}^{up} = 0 \\
         & \quad \quad \quad \quad \forall t \in \mathbb{T}
         \quad \textrm{if} \quad e_{shift} = \textrm{False} \\
         & \\
         &
         (3) \quad DSM_{t}^{do, shed} = 0 \\
         & \quad \quad \quad \quad \forall t \in \mathbb{T}
         \quad \textrm{if} \quad e_{shed} = \textrm{False} \\
         & \\
         &
-        (4) \quad \dot{E}_{t} = demand_{t} \cdot (invest + E_{exist})
-        + DSM_{t}^{up} - DSM_{t}^{do, shift} - DSM_{t}^{do, shed} \\
-        & \quad \quad \quad \quad \forall t \in \mathbb{T} \\
+        (4) \quad \dot{E}_{t} = demand_{t} \cdot demand_{max}(p)
+        + DSM_{t}^{up}
+        - DSM_{t}^{do, shift} - DSM_{t}^{do, shed} \\
+        & \quad \quad \quad \quad \forall p, t \in \textrm{TIMEINDEX} \\
         & \\
         &
-        (5) \quad  DSM_{t}^{up} \leq E_{t}^{up} \cdot (invest + E_{exist})
-        \cdot s_{flex, up} \\
-        & \quad \quad \quad \quad \forall t \in \mathbb{T} \\
+        (5) \quad  DSM_{t}^{up} \leq E_{t}^{up} \cdot P_{total}(p) \\
+        & \quad \quad \quad \quad \forall p, t \in \textrm{TIMEINDEX} \\
         & \\
         &
         (6) \quad DSM_{t}^{do, shift} +  DSM_{t}^{do, shed} \leq
-        E_{t}^{do} \cdot (invest + E_{exist}) \cdot s_{flex, do} \\
-        & \quad \quad \quad \quad \forall t \in \mathbb{T} \\
+        E_{t}^{do} \cdot P_{total}(p) \\
+        & \quad \quad \quad \quad \forall p, t \in \textrm{TIMEINDEX} \\
         & \\
         &
         (7) \quad  \sum_{t=t_s}^{t_s+\tau} DSM_{t}^{up} \cdot \eta =
         \sum_{t=t_s}^{t_s+\tau} DSM_{t}^{do, shift} \\
         & \quad \quad \quad \quad \forall t_s \in
         \{k \in \mathbb{T} \mid k \mod \tau = 0\} \\
 
+
     **The following parts of the objective function are created:**
 
-    * Investment annuity:
+    *Standard model*
 
-    .. math::
-        &
-        invest \cdot costs_{invest} \\
+        * Investment annuity:
 
-    * Variable costs:
+            .. math::
+                P_{invest}(0) \cdot c_{invest}(0)
 
-    .. math::
-        &
-        (DSM_{t}^{up} \cdot cost_{t}^{dsm, up}
-        + DSM_{t}^{do, shift} \cdot cost_{t}^{dsm, do, shift}
-        + DSM_{t}^{do, shed} \cdot cost_{t}^{dsm, do, shed})
-        \cdot \omega_{t} \\
-        & \quad \quad \quad \quad \forall t \in \mathbb{T} \\
+        * Variable costs:
+
+            .. math::
+                &
+                (DSM_{t}^{up} \cdot cost_{t}^{dsm, up}
+                + DSM_{t}^{do, shift} \cdot cost_{t}^{dsm, do, shift} \\
+                & + DSM_{t}^{do, shed} \cdot cost_{t}^{dsm, do, shed})
+                \cdot \omega_{t} \\
+                & \quad \quad \quad \quad \forall t \in \mathbb{T} \\
+
+    *Multi-period model*
+
+        * Investment annuity:
+
+            .. math::
+                &
+                P_{invest}(p) \cdot A(c_{invest}(p), l, ir) \cdot l
+                \cdot DF^{-p} \\
+                &\\
+                &
+                \forall p \in \mathbb{P}
+
+        * :attr:`fixed_costs` not None for investments
+
+            .. math::
+                &
+                (\sum_{pp=year(p)}^{year(p)+l}
+                P_{invest}(p) \cdot c_{fixed}(pp) \cdot DF^{-pp})
+                \cdot DF^{-p} \\
+                &\\
+                &
+                \forall p \in \mathbb{P}
+
+        * Variable costs:
+
+            .. math::
+                &
+                (DSM_{t}^{up} \cdot cost_{t}^{dsm, up}
+                + DSM_{t}^{do, shift} \cdot cost_{t}^{dsm, do, shift} \\
+                & + DSM_{t}^{do, shed} \cdot cost_{t}^{dsm, do, shed})
+                \cdot \omega_{t}
+                \cdot DF^{-p} \\
+                & \quad \quad \quad \quad
+                \forall p, t \in \textrm{TIMEINDEX} \\
+
+    whereby:
+
+    * :math:`A(c_{invest,var}(p), l, ir)` A is the annuity for
+      investment expenses :math:`c_{invest}(p)` lifetime :math:`l`
+      and interest rate :math:`ir`
+    * :math:`DF=(1+dr)` is the discount factor with discount rate
+      :math:`dr`
 
     See remarks in
     :class:`oemof.solph.components.experimental._sink_dsm.SinkDSMOemofBlock`.
 
+
     **Symbols and attribute names of variables and parameters**
 
     * Please refer to
       :class:`oemof.solph.components.experimental._sink_dsm.SinkDSMOemofBlock`.
       for a variables and parameter description.
     * The following variables and parameters are exclusively used for
       investment modeling:
 
-    .. table:: Variables (V) and Parameters (P)
-        :widths: 1, 1, 1, 1
+    .. table:: Variables (V), Parameters (P) and Sets (S)
+        :widths: 25, 25, 10, 40
 
         ================================= ======================== ==== =======================================
         symbol                            attribute                type explanation
         ================================= ======================== ==== =======================================
-        :math:`invest`                    `invest`                 V    | DSM capacity invested in
-                                                                        | Equals to the additionally installed capacity.
-                                                                        | The capacity share eligible for a shift is determined by flex share(s).
-        :math:`invest_{min}`              `investment.minimum`     P    minimum investment
-        :math:`invest_{max}`              `investment.maximum`     P    maximum investment
-        :math:`E_{exist}`                 `investment.existing`    P    existing DSM capacity
-        :math:`s_{flex, up}`              `flex_share_up`          P    share of invested capacity that may be shift upwards at maximum
-        :math:`s_{flex, do}`              `flex_share_do`          P    share of invested capacity that may be shift downwards at maximum
-        :math:`costs_{invest}`            `investment.ep_costs`    P    specific investment annuity
+        :math:`P_{invest}(p)`             `invest[p]`              V    | DSM capacity invested into in period p.
+                                                                        | Equals to the additionally shiftable resp. sheddable capacity.
+        :math:`invest_{min}(p)`           `investment.minimum[p]`  P    minimum investment in period p
+        :math:`invest_{max}(p)`           `investment.maximum[p]`  P    maximum investment in period p
+        :math:`P_{total}`                 `investment.total[p]`    P    total DSM capacity
+        :math:`costs_{invest}(p)`         `investment.ep_costs[p]` P    | specific investment annuity (standard model) resp.
+                                                                        | specific investment expenses (multi-period model)
+        :math:`\mathbb{P}`                                         S    Periods of the model
+        :math:`\textrm{TIMEINDEX}`                                 S    Timeindex set of the model (periods, timesteps)
         ================================= ======================== ==== =======================================
 
     """  # noqa: E501
     CONSTRAINT_GROUP = True
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -844,30 +863,64 @@
             n.inflow = list(n.inputs)[0]
 
         #  ************* SETS *********************************
 
         # Set of DSM Components
         self.investdsm = Set(initialize=[n for n in group])
 
+        self.OVERALL_MAXIMUM_INVESTDSM = Set(
+            initialize=[
+                g for g in group if g.investment.overall_maximum is not None
+            ]
+        )
+
+        self.OVERALL_MINIMUM_INVESTDSM = Set(
+            initialize=[
+                g for g in group if g.investment.overall_minimum is not None
+            ]
+        )
+
+        self.EXISTING_INVESTDSM = Set(
+            initialize=[g for g in group if g.investment.existing is not None]
+        )
+
         #  ************* VARIABLES *****************************
 
         # Define bounds for investments in demand response
-        def _dsm_investvar_bound_rule(block, g):
+        def _dsm_investvar_bound_rule(block, g, p):
             """Rule definition to bound the
             invested demand response capacity `invest`.
             """
-            return g.investment.minimum, g.investment.maximum
+            return g.investment.minimum[p], g.investment.maximum[p]
 
         # Investment in DR capacity
         self.invest = Var(
             self.investdsm,
+            m.PERIODS,
             within=NonNegativeReals,
             bounds=_dsm_investvar_bound_rule,
         )
 
+        # Total capacity
+        self.total = Var(self.investdsm, m.PERIODS, within=NonNegativeReals)
+
+        if m.es.periods is not None:
+            # Old capacity to be decommissioned (due to lifetime)
+            self.old = Var(self.investdsm, m.PERIODS, within=NonNegativeReals)
+
+            # Old endogenous capacity to be decommissioned (due to lifetime)
+            self.old_end = Var(
+                self.investdsm, m.PERIODS, within=NonNegativeReals
+            )
+
+            # Old exogenous capacity to be decommissioned (due to lifetime)
+            self.old_exo = Var(
+                self.investdsm, m.PERIODS, within=NonNegativeReals
+            )
+
         # Variable load shift down
         self.dsm_do_shift = Var(
             self.investdsm, m.TIMESTEPS, initialize=0, within=NonNegativeReals
         )
 
         # Variable load shedding
         self.dsm_do_shed = Var(
@@ -877,14 +930,122 @@
         # Variable load shift up
         self.dsm_up = Var(
             self.investdsm, m.TIMESTEPS, initialize=0, within=NonNegativeReals
         )
 
         #  ************* CONSTRAINTS *****************************
 
+        # Handle unit lifetimes
+        def _total_dsm_capacity_rule(block):
+            """Rule definition for determining total installed
+            capacity (taking decommissioning into account)
+            """
+            for g in group:
+                for p in m.PERIODS:
+                    if p == 0:
+                        expr = (
+                            self.total[g, p]
+                            == self.invest[g, p] + g.investment.existing
+                        )
+                        self.total_dsm_rule.add((g, p), expr)
+                    else:
+                        expr = (
+                            self.total[g, p]
+                            == self.invest[g, p]
+                            + self.total[g, p - 1]
+                            - self.old[g, p]
+                        )
+                        self.total_dsm_rule.add((g, p), expr)
+
+        self.total_dsm_rule = Constraint(group, m.PERIODS, noruleinit=True)
+        self.total_dsm_rule_build = BuildAction(rule=_total_dsm_capacity_rule)
+
+        if m.es.periods is not None:
+
+            def _old_dsm_capacity_rule_end(block):
+                """Rule definition for determining old endogenously installed
+                capacity to be decommissioned due to reaching its lifetime
+                """
+                for g in group:
+                    lifetime = g.investment.lifetime
+                    for p in m.PERIODS:
+                        # No shutdown in first period
+                        if p == 0:
+                            expr = self.old_end[g, p] == 0
+                            self.old_dsm_rule_end.add((g, p), expr)
+                        elif lifetime <= m.es.periods_years[p]:
+                            # Obtain commissioning period
+                            comm_p = 0
+                            for k, v in enumerate(m.es.periods_years):
+                                if m.es.periods_years[p] - lifetime - v < 0:
+                                    # change of sign is detected
+                                    comm_p = k - 1
+                                    break
+                            expr = self.old_end[g, p] == self.invest[g, comm_p]
+                            self.old_dsm_rule_end.add((g, p), expr)
+                        else:
+                            expr = self.old_end[g, p] == 0
+                            self.old_dsm_rule_end.add((g, p), expr)
+
+            self.old_dsm_rule_end = Constraint(
+                group, m.PERIODS, noruleinit=True
+            )
+            self.old_dsm_rule_end_build = BuildAction(
+                rule=_old_dsm_capacity_rule_end
+            )
+
+            def _old_dsm_capacity_rule_exo(block):
+                """Rule definition for determining old exogenously given
+                capacity to be decommissioned due to reaching its lifetime
+                """
+                for g in group:
+                    age = g.investment.age
+                    lifetime = g.investment.lifetime
+                    is_decommissioned = False
+                    for p in m.PERIODS:
+                        # No shutdown in first period
+                        if p == 0:
+                            expr = self.old_exo[g, p] == 0
+                            self.old_dsm_rule_exo.add((g, p), expr)
+                        elif lifetime - age <= m.es.periods_years[p]:
+                            # Track decommissioning status
+                            if not is_decommissioned:
+                                expr = (
+                                    self.old_exo[g, p] == g.investment.existing
+                                )
+                                is_decommissioned = True
+                            else:
+                                expr = self.old_exo[g, p] == 0
+                            self.old_dsm_rule_exo.add((g, p), expr)
+                        else:
+                            expr = self.old_exo[g, p] == 0
+                            self.old_dsm_rule_exo.add((g, p), expr)
+
+            self.old_dsm_rule_exo = Constraint(
+                group, m.PERIODS, noruleinit=True
+            )
+            self.old_dsm_rule_exo_build = BuildAction(
+                rule=_old_dsm_capacity_rule_exo
+            )
+
+            def _old_dsm_capacity_rule(block):
+                """Rule definition for determining (overall) old capacity
+                to be decommissioned due to reaching its lifetime
+                """
+                for g in group:
+                    for p in m.PERIODS:
+                        expr = (
+                            self.old[g, p]
+                            == self.old_end[g, p] + self.old_exo[g, p]
+                        )
+                        self.old_dsm_rule.add((g, p), expr)
+
+            self.old_dsm_rule = Constraint(group, m.PERIODS, noruleinit=True)
+            self.old_dsm_rule_build = BuildAction(rule=_old_dsm_capacity_rule)
+
         def _shift_shed_vars_rule(block):
             """Force shifting resp. shedding variables to zero dependent
             on how boolean parameters for shift resp. shed eligibility
             are set.
             """
             for t in m.TIMESTEPS:
                 for g in group:
@@ -905,101 +1066,93 @@
 
         # Demand Production Relation
         def _input_output_relation_rule(block):
             """Relation between input data and pyomo variables.
             The actual demand after DSM.
             Generator Production == Demand_el +- DSM
             """
-            for t in m.TIMESTEPS:
+            for p, t in m.TIMEINDEX:
                 for g in group:
                     # Inflow from bus
-                    lhs = m.flow[g.inflow, g, t]
+                    lhs = m.flow[g.inflow, g, p, t]
 
                     # Demand + DSM_up - DSM_down
                     rhs = (
-                        g.demand[t] * (self.invest[g] + g.investment.existing)
+                        g.demand[t] * g.max_demand[p]
                         + self.dsm_up[g, t]
                         - self.dsm_do_shift[g, t]
                         - self.dsm_do_shed[g, t]
                     )
 
                     # add constraint
-                    block.input_output_relation.add((g, t), (lhs == rhs))
+                    block.input_output_relation.add((g, p, t), (lhs == rhs))
 
         self.input_output_relation = Constraint(
-            group, m.TIMESTEPS, noruleinit=True
+            group, m.TIMEINDEX, noruleinit=True
         )
         self.input_output_relation_build = BuildAction(
             rule=_input_output_relation_rule
         )
 
         # Upper bounds relation
         def dsm_up_constraint_rule(block):
             """Realised upward load shift at time t has to be smaller than
             upward DSM capacity at time t.
             """
-            for t in m.TIMESTEPS:
+            for p, t in m.TIMEINDEX:
                 for g in group:
                     # DSM up
                     lhs = self.dsm_up[g, t]
                     # Capacity dsm_up
-                    rhs = (
-                        g.capacity_up[t]
-                        * (self.invest[g] + g.investment.existing)
-                        * g.flex_share_up
-                    )
+                    rhs = g.capacity_up[t] * self.total[g, p]
 
                     # add constraint
-                    block.dsm_up_constraint.add((g, t), (lhs <= rhs))
+                    block.dsm_up_constraint.add((g, p, t), (lhs <= rhs))
 
         self.dsm_up_constraint = Constraint(
-            group, m.TIMESTEPS, noruleinit=True
+            group, m.TIMEINDEX, noruleinit=True
         )
         self.dsm_up_constraint_build = BuildAction(rule=dsm_up_constraint_rule)
 
         # Upper bounds relation
         def dsm_down_constraint_rule(block):
             """Realised downward load shift at time t has to be smaller than
             downward DSM capacity at time t.
             """
-            for t in m.TIMESTEPS:
+            for p, t in m.TIMEINDEX:
                 for g in group:
                     # DSM down
                     lhs = self.dsm_do_shift[g, t] + self.dsm_do_shed[g, t]
                     # Capacity dsm_down
-                    rhs = (
-                        g.capacity_down[t]
-                        * (self.invest[g] + g.investment.existing)
-                        * g.flex_share_down
-                    )
+                    rhs = g.capacity_down[t] * self.total[g, p]
 
                     # add constraint
-                    block.dsm_down_constraint.add((g, t), (lhs <= rhs))
+                    block.dsm_down_constraint.add((g, p, t), (lhs <= rhs))
 
         self.dsm_down_constraint = Constraint(
-            group, m.TIMESTEPS, noruleinit=True
+            group, m.TIMEINDEX, noruleinit=True
         )
         self.dsm_down_constraint_build = BuildAction(
             rule=dsm_down_constraint_rule
         )
 
         def dsm_sum_constraint_rule(block):
             """Relation to compensate the total amount of positive
             and negative DSM in between the shift_interval.
             This constraint is building balance in full intervals starting
             with index 0. The last interval might not be full.
             """
             for g in group:
                 intervals = range(
-                    m.TIMESTEPS[1], m.TIMESTEPS[-1], g.shift_interval
+                    m.TIMESTEPS.at(1), m.TIMESTEPS.at(-1), g.shift_interval
                 )
 
                 for interval in intervals:
-                    if (interval + g.shift_interval - 1) > m.TIMESTEPS[-1]:
-                        timesteps = range(interval, m.TIMESTEPS[-1] + 1)
+                    if (interval + g.shift_interval - 1) > m.TIMESTEPS.at(-1):
+                        timesteps = range(interval, m.TIMESTEPS.at(-1) + 1)
                     else:
                         timesteps = range(
                             interval, interval + g.shift_interval
                         )
 
                     # DSM up/down
                     lhs = (
@@ -1015,41 +1168,171 @@
         self.dsm_sum_constraint = Constraint(
             group, m.TIMESTEPS, noruleinit=True
         )
         self.dsm_sum_constraint_build = BuildAction(
             rule=dsm_sum_constraint_rule
         )
 
+        if m.es.periods is not None:
+
+            def _overall_dsm_maximum_investflow_rule(block):
+                """Rule definition for maximum overall investment
+                in investment case.
+                """
+                for g in self.OVERALL_MAXIMUM_INVESTDSM:
+                    for p in m.PERIODS:
+                        expr = self.total[g, p] <= g.investment.overall_maximum
+                        self.overall_dsm_maximum.add((g, p), expr)
+
+            self.overall_dsm_maximum = Constraint(
+                self.OVERALL_MAXIMUM_INVESTDSM, m.PERIODS, noruleinit=True
+            )
+
+            self.overall_maximum_build = BuildAction(
+                rule=_overall_dsm_maximum_investflow_rule
+            )
+
+            def _overall_minimum_dsm_investflow_rule(block):
+                """Rule definition for minimum overall investment
+                in investment case.
+
+                Note: This is only applicable for the last period
+                """
+                for g in self.OVERALL_MINIMUM_INVESTDSM:
+                    expr = (
+                        g.investment.overall_minimum
+                        <= self.total[g, m.PERIODS.at(-1)]
+                    )
+                    self.overall_minimum.add(g, expr)
+
+            self.overall_minimum = Constraint(
+                self.OVERALL_MINIMUM_INVESTDSM, noruleinit=True
+            )
+
+            self.overall_minimum_build = BuildAction(
+                rule=_overall_minimum_dsm_investflow_rule
+            )
+
     def _objective_expression(self):
         r"""Objective expression with variable and investment costs for DSM"""
 
         m = self.parent_block()
 
         investment_costs = 0
+        period_investment_costs = {p: 0 for p in m.PERIODS}
         variable_costs = 0
+        fixed_costs = 0
 
-        for g in self.investdsm:
-            if g.investment.ep_costs is not None:
-                investment_costs += self.invest[g] * g.investment.ep_costs
-            else:
-                raise ValueError("Missing value for investment costs!")
-            for t in m.TIMESTEPS:
-                variable_costs += (
-                    self.dsm_up[g, t]
-                    * g.cost_dsm_up[t]
-                    * m.objective_weighting[t]
-                )
-                variable_costs += (
-                    self.dsm_do_shift[g, t] * g.cost_dsm_down_shift[t]
-                    + self.dsm_do_shed[g, t] * g.cost_dsm_down_shed[t]
-                ) * m.objective_weighting[t]
+        if m.es.periods is None:
+            for g in self.investdsm:
+                for p in m.PERIODS:
+                    if g.investment.ep_costs is not None:
+                        investment_costs += (
+                            self.invest[g, p] * g.investment.ep_costs[p]
+                        )
+                    else:
+                        raise ValueError("Missing value for investment costs!")
+
+                for t in m.TIMESTEPS:
+                    variable_costs += (
+                        self.dsm_up[g, t]
+                        * g.cost_dsm_up[t]
+                        * m.objective_weighting[t]
+                    )
+                    variable_costs += (
+                        self.dsm_do_shift[g, t] * g.cost_dsm_down_shift[t]
+                        + self.dsm_do_shed[g, t] * g.cost_dsm_down_shed[t]
+                    ) * m.objective_weighting[t]
 
-        self.cost = Expression(expr=investment_costs + variable_costs)
+        else:
+            msg = (
+                "You did not specify an interest rate.\n"
+                "It will be set equal to the discount_rate of {} "
+                "of the model as a default.\nThis corresponds to a "
+                "social planner point of view and does not reflect "
+                "microeconomic interest requirements."
+            )
+            for g in self.investdsm:
+                if g.investment.ep_costs is not None:
+                    lifetime = g.investment.lifetime
+                    interest = g.investment.interest_rate
+                    if interest == 0:
+                        warn(
+                            msg.format(m.discount_rate),
+                            debugging.SuspiciousUsageWarning,
+                        )
+                        interest = m.discount_rate
+                    for p in m.PERIODS:
+                        annuity = economics.annuity(
+                            capex=g.investment.ep_costs[p],
+                            n=lifetime,
+                            wacc=interest,
+                        )
+                        investment_costs_increment = (
+                            self.invest[g, p]
+                            * annuity
+                            * lifetime
+                            * ((1 + m.discount_rate) ** -m.es.periods_years[p])
+                        )
+                        investment_costs += investment_costs_increment
+                        period_investment_costs[
+                            p
+                        ] += investment_costs_increment
+                else:
+                    raise ValueError("Missing value for investment costs!")
 
-        return self.cost
+                for p, t in m.TIMEINDEX:
+                    variable_costs += (
+                        self.dsm_up[g, t]
+                        * m.objective_weighting[t]
+                        * g.cost_dsm_up[t]
+                        * ((1 + m.discount_rate) ** -m.es.periods_years[p])
+                    )
+                    variable_costs += (
+                        (
+                            self.dsm_do_shift[g, t] * g.cost_dsm_down_shift[t]
+                            + self.dsm_do_shed[g, t] * g.cost_dsm_down_shed[t]
+                        )
+                        * m.objective_weighting[t]
+                        * ((1 + m.discount_rate) ** -m.es.periods_years[p])
+                    )
+
+                if g.investment.fixed_costs[0] is not None:
+                    lifetime = g.investment.lifetime
+                    for p in m.PERIODS:
+                        fixed_costs += sum(
+                            self.invest[g, p]
+                            * g.investment.fixed_costs[pp]
+                            * ((1 + m.discount_rate) ** (-pp))
+                            for pp in range(
+                                m.es.periods_years[p],
+                                m.es.periods_years[p] + lifetime,
+                            )
+                        ) * ((1 + m.discount_rate) ** -m.es.periods_years[p])
+
+            for g in self.EXISTING_INVESTDSM:
+                if g.investment.fixed_costs[0] is not None:
+                    lifetime = g.investment.lifetime
+                    age = g.investment.age
+                    fixed_costs += sum(
+                        g.investment.existing
+                        * g.investment.fixed_costs[pp]
+                        * ((1 + m.discount_rate) ** (-pp))
+                        for pp in range(0, lifetime - age)
+                    )
+
+        self.variable_costs = Expression(expr=variable_costs)
+        self.fixed_costs = Expression(expr=fixed_costs)
+        self.investment_costs = Expression(expr=investment_costs)
+        self.period_investment_costs = period_investment_costs
+        self.costs = Expression(
+            expr=investment_costs + variable_costs + fixed_costs
+        )
+
+        return self.costs
 
 
 class SinkDSMDIWBlock(ScalarBlock):
     r"""Constraints for SinkDSM with "DIW" approach
 
     **The following constraints are created for approach = "DIW":**
 
@@ -1114,25 +1397,25 @@
     themselves.
 
 
     **The following parts of the objective function are created:**
 
     .. math::
         &
-        (DSM_{t}^{up} \cdot cost_{t}^{dsm, up}
-        + \sum_{tt=0}^{T} DSM_{t, tt}^{do, shift} \cdot
+        DSM_{t}^{up} \cdot cost_{t}^{dsm, up}
+        + \sum_{tt=0}^{|T|} DSM_{tt, t}^{do, shift} \cdot
         cost_{t}^{dsm, do, shift}
         + DSM_{t}^{do, shed} \cdot cost_{t}^{dsm, do, shed})
         \cdot \omega_{t} \\
         & \quad \quad \quad \quad \forall t \in \mathbb{T} \\
 
     **Table: Symbols and attribute names of variables and parameters**
 
-    .. table:: Variables (V) and Parameters (P)
-        :widths: 1, 1, 1, 1
+    .. table:: Variables (V), Parameters (P) and Sets (S)
+        :widths: 25, 25, 10, 40
 
         ================================= ======================== ==== =======================================
         symbol                            attribute                type explanation
         ================================= ======================== ==== =======================================
         :math:`DSM_{t}^{up}`              `dsm_up[g, t]`           V    DSM up shift (additional load) in hour t
         :math:`DSM_{t, tt}^{do, shift}`   `dsm_do_shift[g, t, tt]` V    | DSM down shift (less load) in hour tt
                                                                         | to compensate for upwards shifts in hour t
@@ -1148,15 +1431,15 @@
         :math:`E_{t}^{do}`                `capacity_down[t]`       P    | Capacity  allowed for a load adjustment downwards
                                                                         | (normalized; shifting + shedding)
         :math:`E_{t}^{up}`                `capacity_up[t]`         P    Capacity allowed for a shift upwards (normalized)
         :math:`E_{do, max}`               `max_capacity_down`      P    | Maximum capacity allowed for a load adjustment downwards
                                                                         | (shifting + shedding)
         :math:`E_{up, max}`               `max_capacity_up`        P    Maximum capacity allowed for a shift upwards
         :math:`\eta`                      `efficiency`             P    Efficiency for load shifting processes
-        :math:`\mathbb{T}`                                         P    Time steps of the model
+        :math:`\mathbb{T}`                                         S    Time steps of the model
         :math:`e_{shift}`                 `shift_eligibility`      P    | Boolean parameter indicating if unit can be used
                                                                         | for load shifting
         :math:`e_{shed}`                  `shed_eligibility`       P    | Boolean parameter indicating if unit can be used
                                                                         | for load shedding
         :math:`cost_{t}^{dsm, up}`        `cost_dsm_up[t]`         P    Variable costs for an upwards shift
         :math:`cost_{t}^{dsm, do, shift}` `cost_dsm_down_shift[t]` P    Variable costs for a downwards shift (load shifting)
         :math:`cost_{t}^{dsm, do, shed}`  `cost_dsm_down_shift[t]` P    Variable costs for shedding load
@@ -1237,76 +1520,82 @@
 
         # Demand Production Relation
         def _input_output_relation_rule(block):
             """Relation between input data and pyomo variables.
             The actual demand after DSM.
             Sink Inflow == Demand +- DSM
             """
-            for t in m.TIMESTEPS:
+            for p, t in m.TIMEINDEX:
                 for g in group:
                     # first time steps: 0 + delay time
                     if t <= g.delay_time:
                         # Inflow from bus
-                        lhs = m.flow[g.inflow, g, t]
+                        lhs = m.flow[g.inflow, g, p, t]
                         # Demand +- DSM
                         rhs = (
-                            g.demand[t] * g.max_demand
+                            g.demand[t] * g.max_demand[p]
                             + self.dsm_up[g, t]
                             - sum(
                                 self.dsm_do_shift[g, tt, t]
                                 for tt in range(t + g.delay_time + 1)
                             )
                             - self.dsm_do_shed[g, t]
                         )
 
                         # add constraint
-                        block.input_output_relation.add((g, t), (lhs == rhs))
+                        block.input_output_relation.add(
+                            (g, p, t), (lhs == rhs)
+                        )
 
                     # main use case
-                    elif g.delay_time < t <= m.TIMESTEPS[-1] - g.delay_time:
+                    elif g.delay_time < t <= m.TIMESTEPS.at(-1) - g.delay_time:
                         # Inflow from bus
-                        lhs = m.flow[g.inflow, g, t]
+                        lhs = m.flow[g.inflow, g, p, t]
                         # Demand +- DSM
                         rhs = (
-                            g.demand[t] * g.max_demand
+                            g.demand[t] * g.max_demand[p]
                             + self.dsm_up[g, t]
                             - sum(
                                 self.dsm_do_shift[g, tt, t]
                                 for tt in range(
                                     t - g.delay_time, t + g.delay_time + 1
                                 )
                             )
                             - self.dsm_do_shed[g, t]
                         )
 
                         # add constraint
-                        block.input_output_relation.add((g, t), (lhs == rhs))
+                        block.input_output_relation.add(
+                            (g, p, t), (lhs == rhs)
+                        )
 
                     # last time steps: end - delay time
                     else:
                         # Inflow from bus
-                        lhs = m.flow[g.inflow, g, t]
+                        lhs = m.flow[g.inflow, g, p, t]
                         # Demand +- DSM
                         rhs = (
-                            g.demand[t] * g.max_demand
+                            g.demand[t] * g.max_demand[p]
                             + self.dsm_up[g, t]
                             - sum(
                                 self.dsm_do_shift[g, tt, t]
                                 for tt in range(
-                                    t - g.delay_time, m.TIMESTEPS[-1] + 1
+                                    t - g.delay_time, m.TIMESTEPS.at(-1) + 1
                                 )
                             )
                             - self.dsm_do_shed[g, t]
                         )
 
                         # add constraint
-                        block.input_output_relation.add((g, t), (lhs == rhs))
+                        block.input_output_relation.add(
+                            (g, p, t), (lhs == rhs)
+                        )
 
         self.input_output_relation = Constraint(
-            group, m.TIMESTEPS, noruleinit=True
+            group, m.TIMEINDEX, noruleinit=True
         )
         self.input_output_relation_build = BuildAction(
             rule=_input_output_relation_rule
         )
 
         # Equation 7 (resp. 7')
         def dsm_up_down_constraint_rule(block):
@@ -1329,15 +1618,15 @@
                             for tt in range(t + g.delay_time + 1)
                         )
 
                         # add constraint
                         block.dsm_updo_constraint.add((g, t), (lhs == rhs))
 
                     # main use case
-                    elif g.delay_time < t <= m.TIMESTEPS[-1] - g.delay_time:
+                    elif g.delay_time < t <= m.TIMESTEPS.at(-1) - g.delay_time:
                         # DSM up
                         lhs = self.dsm_up[g, t] * g.efficiency
                         # DSM down
                         rhs = sum(
                             self.dsm_do_shift[g, t, tt]
                             for tt in range(
                                 t - g.delay_time, t + g.delay_time + 1
@@ -1351,15 +1640,15 @@
                     else:
                         # DSM up
                         lhs = self.dsm_up[g, t] * g.efficiency
                         # DSM down
                         rhs = sum(
                             self.dsm_do_shift[g, t, tt]
                             for tt in range(
-                                t - g.delay_time, m.TIMESTEPS[-1] + 1
+                                t - g.delay_time, m.TIMESTEPS.at(-1) + 1
                             )
                         )
 
                         # add constraint
                         block.dsm_updo_constraint.add((g, t), (lhs == rhs))
 
         self.dsm_updo_constraint = Constraint(
@@ -1411,15 +1700,17 @@
                         # Capacity DSM down
                         rhs = g.capacity_down[tt] * g.max_capacity_down
 
                         # add constraint
                         block.dsm_do_constraint.add((g, tt), (lhs <= rhs))
 
                     # main use case
-                    elif g.delay_time < tt <= m.TIMESTEPS[-1] - g.delay_time:
+                    elif (
+                        g.delay_time < tt <= m.TIMESTEPS.at(-1) - g.delay_time
+                    ):
                         # DSM down
                         lhs = (
                             sum(
                                 self.dsm_do_shift[g, t, tt]
                                 for t in range(
                                     tt - g.delay_time, tt + g.delay_time + 1
                                 )
@@ -1435,15 +1726,15 @@
                     # last time steps: end - delay time
                     else:
                         # DSM down
                         lhs = (
                             sum(
                                 self.dsm_do_shift[g, t, tt]
                                 for t in range(
-                                    tt - g.delay_time, m.TIMESTEPS[-1] + 1
+                                    tt - g.delay_time, m.TIMESTEPS.at(-1) + 1
                                 )
                             )
                             + self.dsm_do_shed[g, tt]
                         )
                         # Capacity DSM down
                         rhs = g.capacity_down[tt] * g.max_capacity_down
 
@@ -1481,15 +1772,17 @@
                             g.capacity_up[tt] * g.max_capacity_up,
                             g.capacity_down[tt] * g.max_capacity_down,
                         )
 
                         # add constraint
                         block.C2_constraint.add((g, tt), (lhs <= rhs))
 
-                    elif g.delay_time < tt <= m.TIMESTEPS[-1] - g.delay_time:
+                    elif (
+                        g.delay_time < tt <= m.TIMESTEPS.at(-1) - g.delay_time
+                    ):
                         # DSM up/down
                         lhs = (
                             self.dsm_up[g, tt]
                             + sum(
                                 self.dsm_do_shift[g, t, tt]
                                 for t in range(
                                     tt - g.delay_time, tt + g.delay_time + 1
@@ -1509,15 +1802,15 @@
                     else:
                         # DSM up/down
                         lhs = (
                             self.dsm_up[g, tt]
                             + sum(
                                 self.dsm_do_shift[g, t, tt]
                                 for t in range(
-                                    tt - g.delay_time, m.TIMESTEPS[-1] + 1
+                                    tt - g.delay_time, m.TIMESTEPS.at(-1) + 1
                                 )
                             )
                             + self.dsm_do_shed[g, tt]
                         )
                         # max capacity at tt
                         rhs = max(
                             g.capacity_up[tt] * g.max_capacity_up,
@@ -1539,15 +1832,15 @@
             """
             for t in m.TIMESTEPS:
                 for g in group:
                     # No need to build constraint if no recovery
                     # time is defined.
                     if g.recovery_time_shift not in [None, 0]:
                         # main use case
-                        if t <= m.TIMESTEPS[-1] - g.recovery_time_shift:
+                        if t <= m.TIMESTEPS.at(-1) - g.recovery_time_shift:
                             # DSM up
                             lhs = sum(
                                 self.dsm_up[g, tt]
                                 for tt in range(t, t + g.recovery_time_shift)
                             )
                             # max energy shift for shifting process
                             rhs = (
@@ -1560,15 +1853,15 @@
                             block.recovery_constraint.add((g, t), (lhs <= rhs))
 
                         # last time steps: end - recovery time
                         else:
                             # DSM up
                             lhs = sum(
                                 self.dsm_up[g, tt]
-                                for tt in range(t, m.TIMESTEPS[-1] + 1)
+                                for tt in range(t, m.TIMESTEPS.at(-1) + 1)
                             )
                             # max energy shift for shifting process
                             rhs = (
                                 g.capacity_up[t]
                                 * g.max_capacity_up
                                 * g.delay_time
                                 * m.timeincrement[t]
@@ -1594,15 +1887,15 @@
             of shedded energy.
             """
             for t in m.TIMESTEPS:
                 for g in group:
                     # Only applicable for load shedding
                     if g.shed_eligibility:
                         # main use case
-                        if t <= m.TIMESTEPS[-1] - g.recovery_time_shed:
+                        if t <= m.TIMESTEPS.at(-1) - g.recovery_time_shed:
                             # DSM up
                             lhs = sum(
                                 self.dsm_do_shed[g, tt]
                                 for tt in range(t, t + g.recovery_time_shed)
                             )
                             # max energy shift for shifting process
                             rhs = (
@@ -1617,15 +1910,15 @@
                             )
 
                         # last time steps: end - recovery time
                         else:
                             # DSM up
                             lhs = sum(
                                 self.dsm_do_shed[g, tt]
-                                for tt in range(t, m.TIMESTEPS[-1] + 1)
+                                for tt in range(t, m.TIMESTEPS.at(-1) + 1)
                             )
                             # max energy shift for shifting process
                             rhs = (
                                 g.capacity_down[t]
                                 * g.max_capacity_down
                                 * g.shed_time
                                 * m.timeincrement[t]
@@ -1646,152 +1939,230 @@
         )
 
     def _objective_expression(self):
         r"""Objective expression with variable costs for DSM activity"""
 
         m = self.parent_block()
 
-        dsm_cost = 0
+        variable_costs = 0
+        fixed_costs = 0
 
-        for t in m.TIMESTEPS:
+        if m.es.periods is None:
+            for t in m.TIMESTEPS:
+                for g in self.dsm:
+                    variable_costs += (
+                        self.dsm_up[g, t]
+                        * g.cost_dsm_up[t]
+                        * m.objective_weighting[t]
+                    )
+                    variable_costs += (
+                        sum(self.dsm_do_shift[g, tt, t] for tt in m.TIMESTEPS)
+                        * g.cost_dsm_down_shift[t]
+                        + self.dsm_do_shed[g, t] * g.cost_dsm_down_shed[t]
+                    ) * m.objective_weighting[t]
+
+        else:
             for g in self.dsm:
-                dsm_cost += (
-                    self.dsm_up[g, t]
-                    * g.cost_dsm_up[t]
-                    * m.objective_weighting[t]
-                )
-                dsm_cost += (
-                    sum(self.dsm_do_shift[g, tt, t] for tt in m.TIMESTEPS)
-                    * g.cost_dsm_down_shift[t]
-                    + self.dsm_do_shed[g, t] * g.cost_dsm_down_shed[t]
-                ) * m.objective_weighting[t]
+                for p, t in m.TIMEINDEX:
+                    variable_costs += (
+                        self.dsm_up[g, t]
+                        * m.objective_weighting[t]
+                        * g.cost_dsm_up[t]
+                        * ((1 + m.discount_rate) ** -m.es.periods_years[p])
+                    )
+                    variable_costs += (
+                        (
+                            sum(
+                                self.dsm_do_shift[g, tt, t]
+                                for tt in m.TIMESTEPS
+                            )
+                            * g.cost_dsm_down_shift[t]
+                            + self.dsm_do_shed[g, t] * g.cost_dsm_down_shed[t]
+                        )
+                        * m.objective_weighting[t]
+                        * ((1 + m.discount_rate) ** -m.es.periods_years[p])
+                    )
+
+                if g.fixed_costs[0] is not None:
+                    for p in m.PERIODS:
+                        fixed_costs += (
+                            max(g.max_capacity_up, g.max_capacity_down)
+                            * g.fixed_costs[p]
+                            * ((1 + m.discount_rate) ** -m.es.periods_years[p])
+                        )
 
-        self.cost = Expression(expr=dsm_cost)
+        self.variable_costs = Expression(expr=variable_costs)
+        self.fixed_costs = Expression(expr=fixed_costs)
+        self.costs = Expression(expr=variable_costs + fixed_costs)
 
-        return self.cost
+        return self.costs
 
 
 class SinkDSMDIWInvestmentBlock(ScalarBlock):
     r"""Constraints for SinkDSM with "DIW" approach and `investment` defined
 
     **The following constraints are created for approach = "DIW" with an
     investment object defined:**
 
     .. _SinkDSMDIWInvestmentBlock equations:
 
     .. math::
         &
-        (1) \quad invest_{min} \leq invest \leq invest_{max} \\
+        (1) \quad invest_{min}(p) \leq invest(p) \leq invest_{max}(p) \\
+        & \quad \quad \quad \quad \forall p \in \mathbb{P}
         & \\
         &
         (2) \quad DSM_{t}^{up} = 0 \\
         & \quad \quad \quad \quad \forall t \in \mathbb{T}
         \quad \textrm{if} \quad e_{shift} = \textrm{False} \\
         & \\
         &
         (3) \quad DSM_{t}^{do, shed} = 0 \\
         & \quad \quad \quad \quad \forall t \in \mathbb{T}
         \quad \textrm{if} \quad e_{shed} = \textrm{False} \\
         & \\
         &
-        (4) \quad \dot{E}_{t} = demand_{t} \cdot (invest + E_{exist})
+        (4) \quad \dot{E}_{t} = demand_{t} \cdot demand_{max}(p)
         + DSM_{t}^{up} -
         \sum_{tt=t-L}^{t+L} DSM_{tt,t}^{do, shift} - DSM_{t}^{do, shed} \\
-        & \quad \quad \quad \quad \forall t \in \mathbb{T} \\
+        & \quad \quad \quad \quad \forall p, t \in \textrm{TIMEINDEX} \\
         & \\
         &
         (5) \quad DSM_{t}^{up} \cdot \eta =
         \sum_{tt=t-L}^{t+L} DSM_{t,tt}^{do, shift} \\
         & \quad \quad \quad \quad \forall t \in \mathbb{T} \\
         & \\
         &
-        (6) \quad DSM_{t}^{up} \leq E_{t}^{up} \cdot (invest + E_{exist})
-        \ s_{flex, up} \\
+        (6) \quad DSM_{t}^{up} \leq E_{t}^{up} \cdot P_{total}(p) \\
         & \quad \quad \quad \quad \forall t \in \mathbb{T} \\
         & \\
         &
         (7) \quad \sum_{t=tt-L}^{tt+L} DSM_{t,tt}^{do, shift}
-        + DSM_{tt}^{do, shed} \leq E_{tt}^{do} \cdot (invest + E_{exist})
-        \cdot s_{flex, do} \\
-        & \quad \quad \quad \quad \forall tt \in \mathbb{T} \\
+        + DSM_{tt}^{do, shed} \leq E_{tt}^{do} \cdot P_{total}(p) \\
+        & \quad \quad \quad \quad \forall p, t \in \textrm{TIMEINDEX} \\
         & \\
         &
         (8) \quad DSM_{tt}^{up} + \sum_{t=tt-L}^{tt+L} DSM_{t,tt}^{do, shift}
         + DSM_{tt}^{do, shed} \\
-        & \quad \quad \leq max \{ E_{tt}^{up} \cdot s_{flex, up},
-        E_{tt}^{do} \cdot s_{flex, do} \} \cdot (invest + E_{exist}) \\
-        & \quad \quad \quad \quad \forall tt \in \mathbb{T} \\
+        & \quad \quad \leq max \{ E_{tt}^{up}, E_{tt}^{do} \}
+        \cdot P_{total}(p) \\
+        & \quad \quad \quad \quad \forall p, t \in \textrm{TIMEINDEX} \\
         & \\
         &
         (9) \quad \sum_{tt=t}^{t+R-1} DSM_{tt}^{up}
-        \leq E_{t}^{up} \cdot (invest + E_{exist})
-        \cdot s_{flex, up} \cdot L \cdot \Delta t \\
-        & \quad \quad \quad \quad \forall tt \in \mathbb{T} \\
+        \leq E_{t}^{up} \cdot P_{total}(p)
+        \cdot L \cdot \Delta t \\
+        & \quad \quad \quad \quad \forall p, t \in \textrm{TIMEINDEX} \\
+        & \quad \quad \quad \quad \forall p, t \in \textrm{TIMEINDEX} \\
         & \\
         &
         (10) \quad \sum_{tt=t}^{t+R-1} DSM_{tt}^{do, shed}
-        \leq E_{t}^{do} \cdot (invest + E_{exist})
-        \cdot s_{flex, do} \cdot t_{shed}
+        \leq E_{t}^{do} \cdot P_{total}(p)
+        \cdot t_{shed}
         \cdot \Delta t \\
-        & \quad \quad \quad \quad \forall tt \in \mathbb{T} \\
-
+        & \quad \quad \quad \quad \forall p, t \in \textrm{TIMEINDEX} \\
 
     Note
     ----
 
     For the sake of readability, the handling of indices is not
     displayed here. E.g. evaluating a variable for `t-L` may lead to a negative
     and therefore infeasible index.
     This is addressed by limiting the sums to non-negative indices within the
     model index bounds. Please refer to the constraints implementation
     themselves.
 
 
     **The following parts of the objective function are created:**
 
-    * Investment annuity:
+    *Standard model*
 
-    .. math::
-        &
-        invest \cdot costs_{invest} \\
+        * Investment annuity:
 
-    * Variable costs:
+            .. math::
+                P_{invest}(0) \cdot c_{invest}(0)
+
+        * Variable costs:
+
+            .. math::
+                &
+                (DSM_{t}^{up} \cdot cost_{t}^{dsm, up}
+                + DSM_{t}^{do, shift} \cdot cost_{t}^{dsm, do, shift} \\
+                & + DSM_{t}^{do, shed} \cdot cost_{t}^{dsm, do, shed})
+                \cdot \omega_{t} \\
+                & \quad \quad \quad \quad \forall t \in \mathbb{T} \\
+
+    *Multi-period model*
+
+        * Investment annuity:
+
+            .. math::
+                &
+                P_{invest}(p) \cdot A(c_{invest}(p), l, ir) \cdot l
+                \cdot DF^{-p} \\
+                &\\
+                & \quad \quad \quad \quad \forall p \in \mathbb{P}
+
+        * :attr:`fixed_costs` not None for investments
+
+            .. math::
+                &
+                (\sum_{pp=year(p)}^{year(p)+l}
+                P_{invest}(p) \cdot c_{fixed}(pp) \cdot DF^{-pp})
+                \cdot DF^{-p} \\
+                &\\
+                & \quad \quad \quad \quad \forall p \in \mathbb{P}
+
+        * Variable costs:
+
+            .. math::
+                &
+                (DSM_{t}^{up} \cdot cost_{t}^{dsm, up}
+                + DSM_{t}^{do, shift} \cdot cost_{t}^{dsm, do, shift} \\
+                & + DSM_{t}^{do, shed} \cdot cost_{t}^{dsm, do, shed})
+                \cdot \omega_{t}
+                \cdot DF^{-p} \\
+                & \quad \quad \quad \quad
+                \forall p, t \in \textrm{TIMEINDEX} \\
+
+    whereby:
+
+    * :math:`A(c_{invest,var}(p), l, ir)` is the annuity for
+      investment expenses :math:`c_{invest}(p)` lifetime :math:`l`
+      and interest rate :math:`ir`
+    * :math:`DF=(1+dr)` is the discount factor with discount rate
+      :math:`dr`
+
+    See remarks in
+    :class:`oemof.solph.components.experimental._sink_dsm.SinkDSMOemofBlock`.
 
-    .. math::
-        &
-        (DSM_{t}^{up} \cdot cost_{t}^{dsm, up}
-        + \sum_{tt=0}^{T} DSM_{t, tt}^{do, shift} \cdot
-        cost_{t}^{dsm, do, shift}
-        + DSM_{t}^{do, shed} \cdot cost_{t}^{dsm, do, shed})
-        \cdot \omega_{t} \\
-        & \quad \quad \quad \quad \forall t \in \mathbb{T} \\
 
     **Table: Symbols and attribute names of variables and parameters**
 
     * Please refer to
       :class:`oemof.solph.components.experimental._sink_dsm.SinkDSMDIWBlock`
       for a variables and parameter description.
     * The following variables and parameters are exclusively used for
       investment modeling:
 
-    .. table:: Variables (V) and Parameters (P)
-        :widths: 1, 1, 1, 1
+    .. table:: Variables (V), Parameters (P) and Sets (S)
+        :widths: 25, 25, 10, 40
 
         ================================= ======================== ==== =======================================
         symbol                            attribute                type explanation
         ================================= ======================== ==== =======================================
-        :math:`invest`                    `invest`                 V    | DSM capacity invested in
-                                                                        | Equals to the additionally installed capacity.
-                                                                        | The capacity share eligible for a shift is determined by flex share(s).
-        :math:`invest_{min}`              `investment.minimum`     P    minimum investment
-        :math:`invest_{max}`              `investment.maximum`     P    maximum investment
-        :math:`E_{exist}`                 `investment.existing`    P    existing DSM capacity
-        :math:`s_{flex, up}`              `flex_share_up`          P    share of invested capacity that may be shift upwards at maximum
-        :math:`s_{flex, do}`              `flex_share_do`          P    share of invested capacity that may be shift downwards at maximum
-        :math:`costs_{invest}`            `investment.ep_costs`    P    specific investment annuity
+        :math:`P_{invest}(p)`             `invest[p]`              V    | DSM capacity invested into in period p.
+                                                                        | Equals to the additionally shiftable resp. sheddable capacity.
+        :math:`invest_{min}(p)`           `investment.minimum[p]`  P    minimum investment in period p
+        :math:`invest_{max}(p)`           `investment.maximum[p]`  P    maximum investment in period p
+        :math:`P_{total}`                 `investment.total[p]`    P    total DSM capacity
+        :math:`costs_{invest}(p)`         `investment.ep_costs[p]` P    | specific investment annuity (standard model) resp.
+                                                                        | specific investment expenses (multi-period model)
+        :math:`\mathbb{P}`                                         S    Periods of the model
+        :math:`\textrm{TIMEINDEX}`                                 S    Timeindex set of the model (periods, timesteps)
         ================================= ======================== ==== =======================================
 
     """  # noqa: E501
     CONSTRAINT_GROUP = True
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -1807,30 +2178,65 @@
             n.inflow = list(n.inputs)[0]
 
         #  ************* SETS *********************************
 
         # Set of DSM Components
         self.investdsm = Set(initialize=[g for g in group])
 
+        self.OVERALL_MAXIMUM_INVESTDSM = Set(
+            initialize=[
+                g for g in group if g.investment.overall_maximum is not None
+            ]
+        )
+
+        self.OVERALL_MINIMUM_INVESTDSM = Set(
+            initialize=[
+                g for g in group if g.investment.overall_minimum is not None
+            ]
+        )
+
+        self.EXISTING_INVESTDSM = Set(
+            initialize=[g for g in group if g.investment.existing is not None]
+        )
+
         #  ************* VARIABLES *****************************
 
         # Define bounds for investments in demand response
-        def _dsm_investvar_bound_rule(block, g):
+        def _dsm_investvar_bound_rule(block, g, p):
             """Rule definition to bound the
             demand response capacity invested in (`invest`).
             """
-            return g.investment.minimum, g.investment.maximum
+            return g.investment.minimum[p], g.investment.maximum[p]
 
         # Investment in DR capacity
         self.invest = Var(
             self.investdsm,
+            m.PERIODS,
             within=NonNegativeReals,
             bounds=_dsm_investvar_bound_rule,
         )
 
+        # Total capacity
+        self.total = Var(self.investdsm, m.PERIODS, within=NonNegativeReals)
+
+        if m.es.periods is not None:
+            # Old capacity to be decommissioned (due to lifetime)
+            # Old capacity built out of old exogenous and endogenous capacities
+            self.old = Var(self.investdsm, m.PERIODS, within=NonNegativeReals)
+
+            # Old endogenous capacity to be decommissioned (due to lifetime)
+            self.old_end = Var(
+                self.investdsm, m.PERIODS, within=NonNegativeReals
+            )
+
+            # Old exogenous capacity to be decommissioned (due to lifetime)
+            self.old_exo = Var(
+                self.investdsm, m.PERIODS, within=NonNegativeReals
+            )
+
         # Variable load shift down
         self.dsm_do_shift = Var(
             self.investdsm,
             m.TIMESTEPS,
             m.TIMESTEPS,
             initialize=0,
             within=NonNegativeReals,
@@ -1844,14 +2250,122 @@
         # Variable load shift up
         self.dsm_up = Var(
             self.investdsm, m.TIMESTEPS, initialize=0, within=NonNegativeReals
         )
 
         #  ************* CONSTRAINTS *****************************
 
+        # Handle unit lifetimes
+        def _total_dsm_capacity_rule(block):
+            """Rule definition for determining total installed
+            capacity (taking decommissioning into account)
+            """
+            for g in group:
+                for p in m.PERIODS:
+                    if p == 0:
+                        expr = (
+                            self.total[g, p]
+                            == self.invest[g, p] + g.investment.existing
+                        )
+                        self.total_dsm_rule.add((g, p), expr)
+                    else:
+                        expr = (
+                            self.total[g, p]
+                            == self.invest[g, p]
+                            + self.total[g, p - 1]
+                            - self.old[g, p]
+                        )
+                        self.total_dsm_rule.add((g, p), expr)
+
+        self.total_dsm_rule = Constraint(group, m.PERIODS, noruleinit=True)
+        self.total_dsm_rule_build = BuildAction(rule=_total_dsm_capacity_rule)
+
+        if m.es.periods is not None:
+
+            def _old_dsm_capacity_rule_end(block):
+                """Rule definition for determining old endogenously installed
+                capacity to be decommissioned due to reaching its lifetime
+                """
+                for g in group:
+                    lifetime = g.investment.lifetime
+                    for p in m.PERIODS:
+                        # No shutdown in first period
+                        if p == 0:
+                            expr = self.old_end[g, p] == 0
+                            self.old_dsm_rule_end.add((g, p), expr)
+                        elif lifetime <= m.es.periods_years[p]:
+                            # Obtain commissioning period
+                            comm_p = 0
+                            for k, v in enumerate(m.es.periods_years):
+                                if m.es.periods_years[p] - lifetime - v < 0:
+                                    # change of sign is detected
+                                    comm_p = k - 1
+                                    break
+                            expr = self.old_end[g, p] == self.invest[g, comm_p]
+                            self.old_dsm_rule_end.add((g, p), expr)
+                        else:
+                            expr = self.old_end[g, p] == 0
+                            self.old_dsm_rule_end.add((g, p), expr)
+
+            self.old_dsm_rule_end = Constraint(
+                group, m.PERIODS, noruleinit=True
+            )
+            self.old_dsm_rule_end_build = BuildAction(
+                rule=_old_dsm_capacity_rule_end
+            )
+
+            def _old_dsm_capacity_rule_exo(block):
+                """Rule definition for determining old exogenously given
+                capacity to be decommissioned due to reaching its lifetime
+                """
+                for g in group:
+                    age = g.investment.age
+                    lifetime = g.investment.lifetime
+                    is_decommissioned = False
+                    for p in m.PERIODS:
+                        # No shutdown in first period
+                        if p == 0:
+                            expr = self.old_exo[g, p] == 0
+                            self.old_dsm_rule_exo.add((g, p), expr)
+                        elif lifetime - age <= m.es.periods_years[p]:
+                            # Track decommissioning status
+                            if not is_decommissioned:
+                                expr = (
+                                    self.old_exo[g, p] == g.investment.existing
+                                )
+                                is_decommissioned = True
+                            else:
+                                expr = self.old_exo[g, p] == 0
+                            self.old_dsm_rule_exo.add((g, p), expr)
+                        else:
+                            expr = self.old_exo[g, p] == 0
+                            self.old_dsm_rule_exo.add((g, p), expr)
+
+            self.old_dsm_rule_exo = Constraint(
+                group, m.PERIODS, noruleinit=True
+            )
+            self.old_dsm_rule_exo_build = BuildAction(
+                rule=_old_dsm_capacity_rule_exo
+            )
+
+            def _old_dsm_capacity_rule(block):
+                """Rule definition for determining (overall) old capacity
+                to be decommissioned due to reaching its lifetime
+                """
+                for g in group:
+                    for p in m.PERIODS:
+                        expr = (
+                            self.old[g, p]
+                            == self.old_end[g, p] + self.old_exo[g, p]
+                        )
+                        self.old_dsm_rule.add((g, p), expr)
+
+            self.old_dsm_rule = Constraint(group, m.PERIODS, noruleinit=True)
+            self.old_dsm_rule_build = BuildAction(rule=_old_dsm_capacity_rule)
+
         def _shift_shed_vars_rule(block):
             """Force shifting resp. shedding variables to zero dependent
             on how boolean parameters for shift resp. shed eligibility
             are set.
             """
             for t in m.TIMESTEPS:
                 for g in group:
@@ -1872,79 +2386,82 @@
 
         # Demand Production Relation
         def _input_output_relation_rule(block):
             """Relation between input data and pyomo variables.
             The actual demand after DSM.
             Sink Inflow == Demand +- DSM
             """
-            for t in m.TIMESTEPS:
+            for p, t in m.TIMEINDEX:
                 for g in group:
                     # first time steps: 0 + delay time
                     if t <= g.delay_time:
                         # Inflow from bus
-                        lhs = m.flow[g.inflow, g, t]
+                        lhs = m.flow[g.inflow, g, p, t]
                         # Demand +- DSM
                         rhs = (
-                            g.demand[t]
-                            * (self.invest[g] + g.investment.existing)
+                            g.demand[t] * g.max_demand[p]
                             + self.dsm_up[g, t]
                             - sum(
                                 self.dsm_do_shift[g, tt, t]
                                 for tt in range(t + g.delay_time + 1)
                             )
                             - self.dsm_do_shed[g, t]
                         )
 
                         # add constraint
-                        block.input_output_relation.add((g, t), (lhs == rhs))
+                        block.input_output_relation.add(
+                            (g, p, t), (lhs == rhs)
+                        )
 
                     # main use case
-                    elif g.delay_time < t <= m.TIMESTEPS[-1] - g.delay_time:
+                    elif g.delay_time < t <= m.TIMESTEPS.at(-1) - g.delay_time:
                         # Inflow from bus
-                        lhs = m.flow[g.inflow, g, t]
+                        lhs = m.flow[g.inflow, g, p, t]
                         # Demand +- DSM
                         rhs = (
-                            g.demand[t]
-                            * (self.invest[g] + g.investment.existing)
+                            g.demand[t] * g.max_demand[p]
                             + self.dsm_up[g, t]
                             - sum(
                                 self.dsm_do_shift[g, tt, t]
                                 for tt in range(
                                     t - g.delay_time, t + g.delay_time + 1
                                 )
                             )
                             - self.dsm_do_shed[g, t]
                         )
 
                         # add constraint
-                        block.input_output_relation.add((g, t), (lhs == rhs))
+                        block.input_output_relation.add(
+                            (g, p, t), (lhs == rhs)
+                        )
 
                     # last time steps: end - delay time
                     else:
                         # Inflow from bus
-                        lhs = m.flow[g.inflow, g, t]
+                        lhs = m.flow[g.inflow, g, p, t]
                         # Demand +- DSM
                         rhs = (
-                            g.demand[t]
-                            * (self.invest[g] + g.investment.existing)
+                            g.demand[t] * g.max_demand[p]
                             + self.dsm_up[g, t]
                             - sum(
                                 self.dsm_do_shift[g, tt, t]
                                 for tt in range(
-                                    t - g.delay_time, m.TIMESTEPS[-1] + 1
+                                    t - g.delay_time, m.TIMESTEPS.at(-1) + 1
                                 )
                             )
                             - self.dsm_do_shed[g, t]
                         )
 
                         # add constraint
-                        block.input_output_relation.add((g, t), (lhs == rhs))
+                        block.input_output_relation.add(
+                            (g, p, t), (lhs == rhs)
+                        )
 
         self.input_output_relation = Constraint(
-            group, m.TIMESTEPS, noruleinit=True
+            group, m.TIMEINDEX, noruleinit=True
         )
         self.input_output_relation_build = BuildAction(
             rule=_input_output_relation_rule
         )
 
         # Equation 7 (resp. 7')
         def dsm_up_down_constraint_rule(block):
@@ -1967,15 +2484,15 @@
                             for tt in range(t + g.delay_time + 1)
                         )
 
                         # add constraint
                         block.dsm_updo_constraint.add((g, t), (lhs == rhs))
 
                     # main use case
-                    elif g.delay_time < t <= m.TIMESTEPS[-1] - g.delay_time:
+                    elif g.delay_time < t <= m.TIMESTEPS.at(-1) - g.delay_time:
                         # DSM up
                         lhs = self.dsm_up[g, t] * g.efficiency
                         # DSM down
                         rhs = sum(
                             self.dsm_do_shift[g, t, tt]
                             for tt in range(
                                 t - g.delay_time, t + g.delay_time + 1
@@ -1989,15 +2506,15 @@
                     else:
                         # DSM up
                         lhs = self.dsm_up[g, t] * g.efficiency
                         # DSM down
                         rhs = sum(
                             self.dsm_do_shift[g, t, tt]
                             for tt in range(
-                                t - g.delay_time, m.TIMESTEPS[-1] + 1
+                                t - g.delay_time, m.TIMESTEPS.at(-1) + 1
                             )
                         )
 
                         # add constraint
                         block.dsm_updo_constraint.add((g, t), (lhs == rhs))
 
         self.dsm_updo_constraint = Constraint(
@@ -2009,333 +2526,463 @@
 
         # Equation 8
         def dsm_up_constraint_rule(block):
             """Equation 8 by Zerrahn & Schill:
             Realised upward load shift at time t has to be smaller than
             upward DSM capacity at time t.
             """
-            for t in m.TIMESTEPS:
+            for p, t in m.TIMEINDEX:
                 for g in group:
                     # DSM up
                     lhs = self.dsm_up[g, t]
                     # Capacity dsm_up
-                    rhs = (
-                        g.capacity_up[t]
-                        * (self.invest[g] + g.investment.existing)
-                        * g.flex_share_up
-                    )
+                    rhs = g.capacity_up[t] * self.total[g, p]
 
                     # add constraint
-                    block.dsm_up_constraint.add((g, t), (lhs <= rhs))
+                    block.dsm_up_constraint.add((g, p, t), (lhs <= rhs))
 
         self.dsm_up_constraint = Constraint(
-            group, m.TIMESTEPS, noruleinit=True
+            group, m.TIMEINDEX, noruleinit=True
         )
         self.dsm_up_constraint_build = BuildAction(rule=dsm_up_constraint_rule)
 
         # Equation 9 (modified)
         def dsm_do_constraint_rule(block):
             """Equation 9 by Zerrahn & Schill:
             Realised downward load shift at time t has to be smaller than
             downward DSM capacity at time t.
             """
-            for tt in m.TIMESTEPS:
+            for p, tt in m.TIMEINDEX:
                 for g in group:
                     # first times steps: 0 + delay
                     if tt <= g.delay_time:
                         # DSM down
                         lhs = (
                             sum(
                                 self.dsm_do_shift[g, t, tt]
                                 for t in range(tt + g.delay_time + 1)
                             )
                             + self.dsm_do_shed[g, tt]
                         )
                         # Capacity DSM down
-                        rhs = (
-                            g.capacity_down[tt]
-                            * (self.invest[g] + g.investment.existing)
-                            * g.flex_share_down
-                        )
+                        rhs = g.capacity_down[tt] * self.total[g, p]
 
                         # add constraint
-                        block.dsm_do_constraint.add((g, tt), (lhs <= rhs))
+                        block.dsm_do_constraint.add((g, p, tt), (lhs <= rhs))
 
                     # main use case
-                    elif g.delay_time < tt <= m.TIMESTEPS[-1] - g.delay_time:
+                    elif (
+                        g.delay_time < tt <= m.TIMESTEPS.at(-1) - g.delay_time
+                    ):
                         # DSM down
                         lhs = (
                             sum(
                                 self.dsm_do_shift[g, t, tt]
                                 for t in range(
                                     tt - g.delay_time, tt + g.delay_time + 1
                                 )
                             )
                             + self.dsm_do_shed[g, tt]
                         )
                         # Capacity DSM down
-                        rhs = (
-                            g.capacity_down[tt]
-                            * (self.invest[g] + g.investment.existing)
-                            * g.flex_share_down
-                        )
+                        rhs = g.capacity_down[tt] * self.total[g, p]
 
                         # add constraint
-                        block.dsm_do_constraint.add((g, tt), (lhs <= rhs))
+                        block.dsm_do_constraint.add((g, p, tt), (lhs <= rhs))
 
                     # last time steps: end - delay time
                     else:
                         # DSM down
                         lhs = (
                             sum(
                                 self.dsm_do_shift[g, t, tt]
                                 for t in range(
-                                    tt - g.delay_time, m.TIMESTEPS[-1] + 1
+                                    tt - g.delay_time, m.TIMESTEPS.at(-1) + 1
                                 )
                             )
                             + self.dsm_do_shed[g, tt]
                         )
                         # Capacity DSM down
-                        rhs = (
-                            g.capacity_down[tt]
-                            * (self.invest[g] + g.investment.existing)
-                            * g.flex_share_down
-                        )
+                        rhs = g.capacity_down[tt] * self.total[g, p]
 
                         # add constraint
-                        block.dsm_do_constraint.add((g, tt), (lhs <= rhs))
+                        block.dsm_do_constraint.add((g, p, tt), (lhs <= rhs))
 
         self.dsm_do_constraint = Constraint(
-            group, m.TIMESTEPS, noruleinit=True
+            group, m.TIMEINDEX, noruleinit=True
         )
         self.dsm_do_constraint_build = BuildAction(rule=dsm_do_constraint_rule)
 
         # Equation 10
         def c2_constraint_rule(block):
             """Equation 10 by Zerrahn & Schill:
             The realised DSM up or down at time T has to be smaller than
             the maximum downward or upward capacity at time T. Therefore, in
             total each individual DSM unit within the modeled portfolio
             can only be shifted up OR down at a given time.
             """
-            for tt in m.TIMESTEPS:
+            for p, tt in m.TIMEINDEX:
                 for g in group:
                     # first times steps: 0 + delay time
                     if tt <= g.delay_time:
                         # DSM up/down
                         lhs = (
                             self.dsm_up[g, tt]
                             + sum(
                                 self.dsm_do_shift[g, t, tt]
                                 for t in range(tt + g.delay_time + 1)
                             )
                             + self.dsm_do_shed[g, tt]
                         )
                         # max capacity at tt
-                        rhs = max(
-                            g.capacity_up[tt] * g.flex_share_up,
-                            g.capacity_down[tt] * g.flex_share_down,
-                        ) * (self.invest[g] + g.investment.existing)
+                        rhs = (
+                            max(
+                                g.capacity_up[tt],
+                                g.capacity_down[tt],
+                            )
+                            * self.total[g, p]
+                        )
 
                         # add constraint
-                        block.C2_constraint.add((g, tt), (lhs <= rhs))
+                        block.C2_constraint.add((g, p, tt), (lhs <= rhs))
 
-                    elif g.delay_time < tt <= m.TIMESTEPS[-1] - g.delay_time:
+                    elif (
+                        g.delay_time < tt <= m.TIMESTEPS.at(-1) - g.delay_time
+                    ):
                         # DSM up/down
                         lhs = (
                             self.dsm_up[g, tt]
                             + sum(
                                 self.dsm_do_shift[g, t, tt]
                                 for t in range(
                                     tt - g.delay_time, tt + g.delay_time + 1
                                 )
                             )
                             + self.dsm_do_shed[g, tt]
                         )
                         # max capacity at tt
-                        rhs = max(
-                            g.capacity_up[tt] * g.flex_share_up,
-                            g.capacity_down[tt] * g.flex_share_down,
-                        ) * (self.invest[g] + g.investment.existing)
+                        rhs = (
+                            max(
+                                g.capacity_up[tt],
+                                g.capacity_down[tt],
+                            )
+                            * self.total[g, p]
+                        )
 
                         # add constraint
-                        block.C2_constraint.add((g, tt), (lhs <= rhs))
+                        block.C2_constraint.add((g, p, tt), (lhs <= rhs))
 
                     else:
                         # DSM up/down
                         lhs = (
                             self.dsm_up[g, tt]
                             + sum(
                                 self.dsm_do_shift[g, t, tt]
                                 for t in range(
-                                    tt - g.delay_time, m.TIMESTEPS[-1] + 1
+                                    tt - g.delay_time, m.TIMESTEPS.at(-1) + 1
                                 )
                             )
                             + self.dsm_do_shed[g, tt]
                         )
                         # max capacity at tt
-                        rhs = max(
-                            g.capacity_up[tt] * g.flex_share_up,
-                            g.capacity_down[tt] * g.flex_share_down,
-                        ) * (self.invest[g] + g.investment.existing)
+                        rhs = (
+                            max(
+                                g.capacity_up[tt],
+                                g.capacity_down[tt],
+                            )
+                            * self.total[g, p]
+                        )
 
                         # add constraint
-                        block.C2_constraint.add((g, tt), (lhs <= rhs))
+                        block.C2_constraint.add((g, p, tt), (lhs <= rhs))
 
-        self.C2_constraint = Constraint(group, m.TIMESTEPS, noruleinit=True)
+        self.C2_constraint = Constraint(group, m.TIMEINDEX, noruleinit=True)
         self.C2_constraint_build = BuildAction(rule=c2_constraint_rule)
 
         def recovery_constraint_rule(block):
             """Equation 11 by Zerrahn & Schill:
             A recovery time is introduced to account for the fact that
             there may be some restrictions before the next load shift
             may take place. Rule is only applicable if a recovery time
             is defined.
             """
-            for t in m.TIMESTEPS:
+            for p, t in m.TIMEINDEX:
                 for g in group:
                     # No need to build constraint if no recovery
                     # time is defined.
                     if g.recovery_time_shift not in [None, 0]:
                         # main use case
-                        if t <= m.TIMESTEPS[-1] - g.recovery_time_shift:
+                        if t <= m.TIMESTEPS.at(-1) - g.recovery_time_shift:
                             # DSM up
                             lhs = sum(
                                 self.dsm_up[g, tt]
                                 for tt in range(t, t + g.recovery_time_shift)
                             )
                             # max energy shift for shifting process
                             rhs = (
                                 g.capacity_up[t]
-                                * (self.invest[g] + g.investment.existing)
-                                * g.flex_share_up
+                                * self.total[g, p]
                                 * g.delay_time
                                 * m.timeincrement[t]
                             )
                             # add constraint
-                            block.recovery_constraint.add((g, t), (lhs <= rhs))
+                            block.recovery_constraint.add(
+                                (g, p, t), (lhs <= rhs)
+                            )
 
                         # last time steps: end - recovery time
                         else:
                             # DSM up
                             lhs = sum(
                                 self.dsm_up[g, tt]
-                                for tt in range(t, m.TIMESTEPS[-1] + 1)
+                                for tt in range(t, m.TIMESTEPS.at(-1) + 1)
                             )
                             # max energy shift for shifting process
                             rhs = (
                                 g.capacity_up[t]
-                                * (self.invest[g] + g.investment.existing)
-                                * g.flex_share_up
+                                * self.total[g, p]
                                 * g.delay_time
                                 * m.timeincrement[t]
                             )
                             # add constraint
-                            block.recovery_constraint.add((g, t), (lhs <= rhs))
+                            block.recovery_constraint.add(
+                                (g, p, t), (lhs <= rhs)
+                            )
 
                     else:
                         pass  # return(Constraint.Skip)
 
         self.recovery_constraint = Constraint(
-            group, m.TIMESTEPS, noruleinit=True
+            group, m.TIMEINDEX, noruleinit=True
         )
         self.recovery_constraint_build = BuildAction(
             rule=recovery_constraint_rule
         )
 
         # Equation 9a from Zerrahn and Schill (2015b)
         def shed_limit_constraint_rule(block):
             """The following constraint is highly similar to equation 9a
             from Zerrahn and Schill (2015b): A recovery time for load
             shedding is introduced in order to limit the overall amount
             of shedded energy.
             """
-            for t in m.TIMESTEPS:
+            for p, t in m.TIMEINDEX:
                 for g in group:
                     # Only applicable for load shedding
                     if g.shed_eligibility:
                         # main use case
-                        if t <= m.TIMESTEPS[-1] - g.recovery_time_shed:
+                        if t <= m.TIMESTEPS.at(-1) - g.recovery_time_shed:
                             # DSM up
                             lhs = sum(
                                 self.dsm_do_shed[g, tt]
                                 for tt in range(t, t + g.recovery_time_shed)
                             )
                             # max energy shift for shifting process
                             rhs = (
                                 g.capacity_down[t]
-                                * (self.invest[g] + g.investment.existing)
-                                * g.flex_share_down
+                                * self.total[g, p]
                                 * g.shed_time
                                 * m.timeincrement[t]
                             )
                             # add constraint
                             block.shed_limit_constraint.add(
-                                (g, t), (lhs <= rhs)
+                                (g, p, t), (lhs <= rhs)
                             )
 
                         # last time steps: end - recovery time
                         else:
                             # DSM up
                             lhs = sum(
                                 self.dsm_do_shed[g, tt]
-                                for tt in range(t, m.TIMESTEPS[-1] + 1)
+                                for tt in range(t, m.TIMESTEPS.at(-1) + 1)
                             )
                             # max energy shift for shifting process
                             rhs = (
                                 g.capacity_down[t]
-                                * (self.invest[g] + g.investment.existing)
-                                * g.flex_share_down
+                                * self.total[g, p]
                                 * g.shed_time
                                 * m.timeincrement[t]
                             )
                             # add constraint
                             block.shed_limit_constraint.add(
-                                (g, t), (lhs <= rhs)
+                                (g, p, t), (lhs <= rhs)
                             )
 
                     else:
                         pass  # return(Constraint.Skip)
 
         self.shed_limit_constraint = Constraint(
-            group, m.TIMESTEPS, noruleinit=True
+            group, m.TIMEINDEX, noruleinit=True
         )
         self.shed_limit_constraint_build = BuildAction(
             rule=shed_limit_constraint_rule
         )
 
+        if m.es.periods is not None:
+
+            def _overall_dsm_maximum_investflow_rule(block):
+                """Rule definition for maximum overall investment
+                in investment case.
+                """
+                for g in self.OVERALL_MAXIMUM_INVESTDSM:
+                    for p in m.PERIODS:
+                        expr = self.total[g, p] <= g.investment.overall_maximum
+                        self.overall_dsm_maximum.add((g, p), expr)
+
+            self.overall_dsm_maximum = Constraint(
+                self.OVERALL_MAXIMUM_INVESTDSM, m.PERIODS, noruleinit=True
+            )
+
+            self.overall_maximum_build = BuildAction(
+                rule=_overall_dsm_maximum_investflow_rule
+            )
+
+            def _overall_minimum_dsm_investflow_rule(block):
+                """Rule definition for minimum overall investment
+                in investment case.
+
+                Note: This is only applicable for the last period
+                """
+                for g in self.OVERALL_MINIMUM_INVESTDSM:
+                    expr = (
+                        g.investment.overall_minimum
+                        <= self.total[g, m.PERIODS.at(-1)]
+                    )
+                    self.overall_minimum.add(g, expr)
+
+            self.overall_minimum = Constraint(
+                self.OVERALL_MINIMUM_INVESTDSM, noruleinit=True
+            )
+
+            self.overall_minimum_build = BuildAction(
+                rule=_overall_minimum_dsm_investflow_rule
+            )
+
     def _objective_expression(self):
         r"""Objective expression with variable and investment costs for DSM"""
 
         m = self.parent_block()
 
         investment_costs = 0
+        period_investment_costs = {p: 0 for p in m.PERIODS}
         variable_costs = 0
+        fixed_costs = 0
 
-        for g in self.investdsm:
-            if g.investment.ep_costs is not None:
-                investment_costs += self.invest[g] * g.investment.ep_costs
-            else:
-                raise ValueError("Missing value for investment costs!")
+        if m.es.periods is None:
+            for g in self.investdsm:
+                for p in m.PERIODS:
+                    if g.investment.ep_costs is not None:
+                        investment_costs += (
+                            self.invest[g, p] * g.investment.ep_costs[p]
+                        )
+                    else:
+                        raise ValueError("Missing value for investment costs!")
 
-            for t in m.TIMESTEPS:
-                variable_costs += (
-                    self.dsm_up[g, t]
-                    * g.cost_dsm_up[t]
-                    * m.objective_weighting[t]
-                )
-                variable_costs += (
-                    sum(self.dsm_do_shift[g, tt, t] for tt in m.TIMESTEPS)
-                    * g.cost_dsm_down_shift[t]
-                    + self.dsm_do_shed[g, t] * g.cost_dsm_down_shed[t]
-                ) * m.objective_weighting[t]
+                for t in m.TIMESTEPS:
+                    variable_costs += (
+                        self.dsm_up[g, t]
+                        * g.cost_dsm_up[t]
+                        * m.objective_weighting[t]
+                    )
+                    variable_costs += (
+                        sum(self.dsm_do_shift[g, tt, t] for tt in m.TIMESTEPS)
+                        * g.cost_dsm_down_shift[t]
+                        + self.dsm_do_shed[g, t] * g.cost_dsm_down_shed[t]
+                    ) * m.objective_weighting[t]
+
+        else:
+            msg = (
+                "You did not specify an interest rate.\n"
+                "It will be set equal to the discount_rate of {} "
+                "of the model as a default.\nThis corresponds to a "
+                "social planner point of view and does not reflect "
+                "microeconomic interest requirements."
+            )
+            for g in self.investdsm:
+                if g.investment.ep_costs is not None:
+                    lifetime = g.investment.lifetime
+                    interest = g.investment.interest_rate
+                    if interest == 0:
+                        warn(
+                            msg.format(m.discount_rate),
+                            debugging.SuspiciousUsageWarning,
+                        )
+                        interest = m.discount_rate
+                    for p in m.PERIODS:
+                        annuity = economics.annuity(
+                            capex=g.investment.ep_costs[p],
+                            n=lifetime,
+                            wacc=interest,
+                        )
+                        investment_costs_increment = (
+                            self.invest[g, p]
+                            * annuity
+                            * lifetime
+                            * ((1 + m.discount_rate) ** -m.es.periods_years[p])
+                        )
+                        investment_costs += investment_costs_increment
+                        period_investment_costs[
+                            p
+                        ] += investment_costs_increment
+                else:
+                    raise ValueError("Missing value for investment costs!")
+
+                for p, t in m.TIMEINDEX:
+                    variable_costs += (
+                        self.dsm_up[g, t]
+                        * m.objective_weighting[t]
+                        * g.cost_dsm_up[t]
+                        * ((1 + m.discount_rate) ** -m.es.periods_years[p])
+                    )
+                    variable_costs += (
+                        (
+                            sum(
+                                self.dsm_do_shift[g, tt, t]
+                                for tt in m.TIMESTEPS
+                            )
+                            * g.cost_dsm_down_shift[t]
+                            + self.dsm_do_shed[g, t] * g.cost_dsm_down_shed[t]
+                        )
+                        * m.objective_weighting[t]
+                        * ((1 + m.discount_rate) ** -m.es.periods_years[p])
+                    )
+
+                if g.investment.fixed_costs[0] is not None:
+                    lifetime = g.investment.lifetime
+                    for p in m.PERIODS:
+                        fixed_costs += sum(
+                            self.invest[g, p]
+                            * g.investment.fixed_costs[pp]
+                            * ((1 + m.discount_rate) ** (-pp))
+                            for pp in range(
+                                m.es.periods_years[p],
+                                m.es.periods_years[p] + lifetime,
+                            )
+                        ) * ((1 + m.discount_rate) ** -m.es.periods_years[p])
+
+            for g in self.EXISTING_INVESTDSM:
+                if g.investment.fixed_costs[0] is not None:
+                    lifetime = g.investment.lifetime
+                    age = g.investment.age
+                    fixed_costs += sum(
+                        g.investment.existing
+                        * g.investment.fixed_costs[pp]
+                        * ((1 + m.discount_rate) ** (-pp))
+                        for pp in range(0, lifetime - age)
+                    )
 
-        self.cost = Expression(expr=investment_costs + variable_costs)
+        self.variable_costs = Expression(expr=variable_costs)
+        self.fixed_costs = Expression(expr=fixed_costs)
+        self.investment_costs = Expression(expr=investment_costs)
+        self.period_investment_costs = period_investment_costs
+        self.costs = Expression(
+            expr=investment_costs + variable_costs + fixed_costs
+        )
 
-        return self.cost
+        return self.costs
 
 
 class SinkDSMDLRBlock(ScalarBlock):
     r"""Constraints for SinkDSM with "DLR" approach
 
     **The following constraints are created for approach = "DLR":**
 
@@ -2484,21 +3131,21 @@
         \cdot cost_{t}^{dsm, do, shift} \\
         & + DSM_{t}^{do, shed} \cdot cost_{t}^{dsm, do, shed})
         \cdot \omega_{t} \\
         & \quad \quad \quad \quad \forall t \in \mathbb{T} \\
 
     **Table: Symbols and attribute names of variables and parameters**
 
-        .. table:: Variables (V), Parameters (P) and additional Sets (S)
-            :widths: 1, 1, 1, 1
+        .. table:: Variables (V), Parameters (P) and (additional) Sets (S)
+            :widths: 25, 25, 10, 40
 
             =========================================== ================================= ==== =======================================
             symbol                                      attribute                         type explanation
             =========================================== ================================= ==== =======================================
-            :math:`DSM_{h, t}^{up}`                     `dsm_up[g,h,t]`                   V    DSM up shift (additional load) in hour t with delay time h
+            :math:`DSM_{h, t}^{up}`                     `dsm_up[g, h, t]`                 V    DSM up shift (additional load) in hour t with delay time h
             :math:`DSM_{h, t}^{do, shift}`              `dsm_do_shift[g, h, t]`           V    DSM down shift (less load) in hour t with delay time h
             :math:`DSM_{h, t}^{balanceUp}`              `balance_dsm_up[g, h, t]`         V    | DSM down shift (less load) in hour t with delay time h
                                                                                                | to balance previous upshift
             :math:`DSM_{h, t}^{balanceDo}`              `balance_dsm_do[g, h, t]`         V    | DSM up shift (additional load) in hour t with delay time h
                                                                                                | to balance previous downshift
             :math:`DSM_{t}^{do, shed}`                  `dsm_do_shed[g, t]`               V    DSM shedded (capacity shedded, i.e. not compensated for)
             :math:`\dot{E}_{t}`                         `SinkDSM.inputs`                  V    Energy flowing in from (electrical) inflow bus
@@ -2518,15 +3165,15 @@
             :math:`E_{t}^{do}`                          `capacity_down[t]`                P    | Capacity  allowed for a load adjustment downwards
                                                                                                | (normalized; shifting + shedding)
             :math:`E_{t}^{up}`                          `capacity_up[t]`                  P    Capacity allowed for a shift upwards (normalized)
             :math:`E_{do, max}`                         `max_capacity_down`               P    | Maximum capacity allowed for a load adjustment downwards
                                                                                                | (shifting + shedding)
             :math:`E_{up, max}`                         `max_capacity_up`                 P    Maximum capacity allowed for a shift upwards
             :math:`\eta`                                `efficiency`                      P    Efficiency for load shifting processes
-            :math:`\mathbb{T}`                                                            P    Time steps of the model
+            :math:`\mathbb{T}`                                                            S    Time steps of the model
             :math:`e_{shift}`                           `shift_eligibility`               P    | Boolean parameter indicating if unit can be used
                                                                                                | for load shifting
             :math:`e_{shed}`                            `shed_eligibility`                P    | Boolean parameter indicating if unit can be used
                                                                                                | for load shedding
             :math:`cost_{t}^{dsm, up}`                  `cost_dsm_up[t]`                  P    Variable costs for an upwards shift
             :math:`cost_{t}^{dsm, do, shift}`           `cost_dsm_down_shift[t]`          P    Variable costs for a downwards shift (load shifting)
             :math:`cost_{t}^{dsm, do, shed}`            `cost_dsm_down_shift[t]`          P    Variable costs for shedding load
@@ -2646,37 +3293,37 @@
 
         # Relation between inflow and effective Sink consumption
         def _input_output_relation_rule(block):
             """Relation between input data and pyomo variables.
             The actual demand after DR.
             BusBlock outflow == Demand +- DR (i.e. effective Sink consumption)
             """
-            for t in m.TIMESTEPS:
+            for p, t in m.TIMEINDEX:
                 for g in group:
                     # outflow from bus
-                    lhs = m.flow[g.inflow, g, t]
+                    lhs = m.flow[g.inflow, g, p, t]
 
                     # Demand +- DR
                     rhs = (
-                        g.demand[t] * g.max_demand
+                        g.demand[t] * g.max_demand[p]
                         + sum(
                             self.dsm_up[g, h, t]
                             + self.balance_dsm_do[g, h, t]
                             - self.dsm_do_shift[g, h, t]
                             - self.balance_dsm_up[g, h, t]
                             for h in g.delay_time
                         )
                         - self.dsm_do_shed[g, t]
                     )
 
                     # add constraint
-                    block.input_output_relation.add((g, t), (lhs == rhs))
+                    block.input_output_relation.add((g, p, t), (lhs == rhs))
 
         self.input_output_relation = Constraint(
-            group, m.TIMESTEPS, noruleinit=True
+            group, m.TIMEINDEX, noruleinit=True
         )
         self.input_output_relation_build = BuildAction(
             rule=_input_output_relation_rule
         )
 
         # Equation 4.8
         def capacity_balance_red_rule(block):
@@ -2700,15 +3347,15 @@
 
                                 # add constraint
                                 block.capacity_balance_red.add(
                                     (g, h, t), (lhs == rhs)
                                 )
 
                             # no balancing for the first timestep
-                            elif t == m.TIMESTEPS[1]:
+                            elif t == m.TIMESTEPS.at(1):
                                 lhs = self.balance_dsm_do[g, h, t]
                                 rhs = 0
 
                                 block.capacity_balance_red.add(
                                     (g, h, t), (lhs == rhs)
                                 )
 
@@ -2750,15 +3397,15 @@
 
                                 # add constraint
                                 block.capacity_balance_inc.add(
                                     (g, h, t), (lhs == rhs)
                                 )
 
                             # no balancing for the first timestep
-                            elif t == m.TIMESTEPS[1]:
+                            elif t == m.TIMESTEPS.at(1):
                                 lhs = self.balance_dsm_up[g, h, t]
                                 rhs = 0
 
                                 block.capacity_balance_inc.add(
                                     (g, h, t), (lhs == rhs)
                                 )
 
@@ -2786,15 +3433,15 @@
             """Prevent downwards shifts that cannot be balanced anymore
             within the optimization timeframe
             """
             for t in m.TIMESTEPS:
                 for g in group:
                     if g.fixes:
                         for h in g.delay_time:
-                            if t > m.TIMESTEPS[-1] - h:
+                            if t > m.TIMESTEPS.at(-1) - h:
                                 # no load reduction anymore (dsm_do_shift = 0)
                                 lhs = self.dsm_do_shift[g, h, t]
                                 rhs = 0
                                 block.no_comp_red.add((g, h, t), (lhs == rhs))
 
                     else:
                         pass  # return(Constraint.Skip)
@@ -2809,15 +3456,15 @@
             """Prevent upwards shifts that cannot be balanced anymore
             within the optimization timeframe
             """
             for t in m.TIMESTEPS:
                 for g in group:
                     if g.fixes:
                         for h in g.delay_time:
-                            if t > m.TIMESTEPS[-1] - h:
+                            if t > m.TIMESTEPS.at(-1) - h:
                                 # no load increase anymore (dsm_up = 0)
                                 lhs = self.dsm_up[g, h, t]
                                 rhs = 0
                                 block.no_comp_inc.add((g, h, t), (lhs == rhs))
 
                     else:
                         pass  # return(Constraint.Skip)
@@ -3015,105 +3662,123 @@
             overall limit for optimization timeframe considered
             A year limit in contrast to Gils (2015) is defined a mandatory
             parameter here in order to achieve an approach comparable
             to the others.
             """
             for g in group:
                 if g.shed_eligibility:
-                    # sum of all load reductions
-                    lhs = sum(self.dsm_do_shed[g, t] for t in m.TIMESTEPS)
+                    for p in m.PERIODS:
+                        # sum of all load reductions
+                        lhs = sum(
+                            self.dsm_do_shed[g, t]
+                            for pp, t in m.TIMEINDEX
+                            if pp == p
+                        )
 
-                    # year limit
-                    rhs = (
-                        g.capacity_down_mean
-                        * g.max_capacity_down
-                        * g.shed_time
-                        * g.n_yearLimit_shed
-                    )
+                        # year limit
+                        rhs = (
+                            g.capacity_down_mean
+                            * g.max_capacity_down
+                            * g.shed_time
+                            * g.n_yearLimit_shed
+                        )
 
-                    # add constraint
-                    block.dr_yearly_limit_shed.add(g, (lhs <= rhs))
+                        # add constraint
+                        block.dr_yearly_limit_shed.add((g, p), (lhs <= rhs))
 
                 else:
                     pass  # return(Constraint.Skip)
 
-        self.dr_yearly_limit_shed = Constraint(group, noruleinit=True)
+        self.dr_yearly_limit_shed = Constraint(
+            group, m.PERIODS, noruleinit=True
+        )
         self.dr_yearly_limit_shed_build = BuildAction(
             rule=dr_yearly_limit_shed_rule
         )
 
         # ************* Optional Constraints *****************************
 
         # Equation 4.17
         def dr_yearly_limit_red_rule(block):
             """Introduce overall annual (energy) limit for load reductions
             resp. overall limit for optimization timeframe considered
             """
             for g in group:
                 if g.ActivateYearLimit:
-                    # sum of all load reductions
-                    lhs = sum(
-                        sum(self.dsm_do_shift[g, h, t] for h in g.delay_time)
-                        for t in m.TIMESTEPS
-                    )
+                    for p in m.PERIODS:
+                        # sum of all load reductions
+                        lhs = sum(
+                            sum(
+                                self.dsm_do_shift[g, h, t]
+                                for h in g.delay_time
+                            )
+                            for pp, t in m.TIMEINDEX
+                            if pp == p
+                        )
 
-                    # year limit
-                    rhs = (
-                        g.capacity_down_mean
-                        * g.max_capacity_down
-                        * g.shift_time
-                        * g.n_yearLimit_shift
-                    )
+                        # year limit
+                        rhs = (
+                            g.capacity_down_mean
+                            * g.max_capacity_down
+                            * g.shift_time
+                            * g.n_yearLimit_shift
+                        )
 
-                    # add constraint
-                    block.dr_yearly_limit_red.add(g, (lhs <= rhs))
+                        # add constraint
+                        block.dr_yearly_limit_red.add((g, p), (lhs <= rhs))
 
                 else:
                     pass  # return(Constraint.Skip)
 
-        self.dr_yearly_limit_red = Constraint(group, noruleinit=True)
+        self.dr_yearly_limit_red = Constraint(
+            group, m.PERIODS, noruleinit=True
+        )
         self.dr_yearly_limit_red_build = BuildAction(
             rule=dr_yearly_limit_red_rule
         )
 
         # Equation 4.18
         def dr_yearly_limit_inc_rule(block):
             """Introduce overall annual (energy) limit for load increases
             resp. overall limit for optimization timeframe considered
             """
             for g in group:
                 if g.ActivateYearLimit:
-                    # sum of all load increases
-                    lhs = sum(
-                        sum(self.dsm_up[g, h, t] for h in g.delay_time)
-                        for t in m.TIMESTEPS
-                    )
+                    for p in m.PERIODS:
+                        # sum of all load increases
+                        lhs = sum(
+                            sum(self.dsm_up[g, h, t] for h in g.delay_time)
+                            for pp, t in m.TIMEINDEX
+                            if pp == p
+                        )
 
-                    # year limit
-                    rhs = (
-                        g.capacity_up_mean
-                        * g.max_capacity_up
-                        * g.shift_time
-                        * g.n_yearLimit_shift
-                    )
+                        # year limit
+                        rhs = (
+                            g.capacity_up_mean
+                            * g.max_capacity_up
+                            * g.shift_time
+                            * g.n_yearLimit_shift
+                        )
 
-                    # add constraint
-                    block.dr_yearly_limit_inc.add(g, (lhs <= rhs))
+                        # add constraint
+                        block.dr_yearly_limit_inc.add((g, p), (lhs <= rhs))
 
                 else:
                     pass  # return(Constraint.Skip)
 
-        self.dr_yearly_limit_inc = Constraint(group, noruleinit=True)
+        self.dr_yearly_limit_inc = Constraint(
+            group, m.PERIODS, noruleinit=True
+        )
         self.dr_yearly_limit_inc_build = BuildAction(
             rule=dr_yearly_limit_inc_rule
         )
 
         # Equation 4.19
         def dr_daily_limit_red_rule(block):
-            """ "Introduce rolling (energy) limit for load reductions
+            """Introduce rolling (energy) limit for load reductions
             This effectively limits DR utilization dependent on
             activations within previous hours.
             """
             for t in m.TIMESTEPS:
                 for g in group:
                     if g.ActivateDayLimit:
                         # main use case
@@ -3247,69 +3912,110 @@
     # Equation 4.23
     def _objective_expression(self):
         r"""Objective expression with variable costs for DSM activity;
         Equation 4.23 from Gils (2015)
         """
         m = self.parent_block()
 
-        dr_cost = 0
+        variable_costs = 0
+        fixed_costs = 0
+
+        if m.es.periods is None:
+            for t in m.TIMESTEPS:
+                for g in self.DR:
+                    variable_costs += (
+                        sum(
+                            self.dsm_up[g, h, t] + self.balance_dsm_do[g, h, t]
+                            for h in g.delay_time
+                        )
+                        * g.cost_dsm_up[t]
+                        * m.objective_weighting[t]
+                    )
+                    variable_costs += (
+                        sum(
+                            self.dsm_do_shift[g, h, t]
+                            + self.balance_dsm_up[g, h, t]
+                            for h in g.delay_time
+                        )
+                        * g.cost_dsm_down_shift[t]
+                        + self.dsm_do_shed[g, t] * g.cost_dsm_down_shed[t]
+                    ) * m.objective_weighting[t]
 
-        for t in m.TIMESTEPS:
+        else:
             for g in self.DR:
-                dr_cost += (
-                    sum(
-                        self.dsm_up[g, h, t] + self.balance_dsm_do[g, h, t]
-                        for h in g.delay_time
+                for p, t in m.TIMEINDEX:
+                    variable_costs += (
+                        (
+                            sum(
+                                self.dsm_up[g, h, t]
+                                + self.balance_dsm_do[g, h, t]
+                                for h in g.delay_time
+                            )
+                            * g.cost_dsm_up[t]
+                        )
+                        * m.objective_weighting[t]
+                        * ((1 + m.discount_rate) ** -m.es.periods_years[p])
                     )
-                    * g.cost_dsm_up[t]
-                    * m.objective_weighting[t]
-                )
-                dr_cost += (
-                    sum(
-                        self.dsm_do_shift[g, h, t]
-                        + self.balance_dsm_up[g, h, t]
-                        for h in g.delay_time
+                    variable_costs += (
+                        (
+                            sum(
+                                self.dsm_do_shift[g, h, t]
+                                + self.balance_dsm_up[g, h, t]
+                                for h in g.delay_time
+                            )
+                            * g.cost_dsm_down_shift[t]
+                            + self.dsm_do_shed[g, t] * g.cost_dsm_down_shed[t]
+                        )
+                        * m.objective_weighting[t]
+                        * ((1 + m.discount_rate) ** -m.es.periods_years[p])
                     )
-                    * g.cost_dsm_down_shift[t]
-                    + self.dsm_do_shed[g, t] * g.cost_dsm_down_shed[t]
-                ) * m.objective_weighting[t]
 
-        self.cost = Expression(expr=dr_cost)
+                if g.fixed_costs[0] is not None:
+                    for p in m.PERIODS:
+                        fixed_costs += (
+                            max(g.max_capacity_up, g.max_capacity_down)
+                            * g.fixed_costs[p]
+                            * ((1 + m.discount_rate) ** -m.es.periods_years[p])
+                        )
+
+        self.variable_costs = Expression(expr=variable_costs)
+        self.fixed_costs = Expression(expr=fixed_costs)
+        self.costs = Expression(expr=variable_costs + fixed_costs)
 
-        return self.cost
+        return self.costs
 
 
 class SinkDSMDLRInvestmentBlock(ScalarBlock):
     r"""Constraints for SinkDSM with "DLR" approach and `investment` defined
 
     **The following constraints are created for approach = "DLR" with an
     investment object defined:**
 
     .. _SinkDSMDLRInvestmentBlock equations:
 
     .. math::
         &
-        (1) \quad invest_{min} \leq invest \leq invest_{max} \\
+        (1) \quad invest_{min}(p) \leq invest(p) \leq invest_{max}(p) \\
+        & \quad \quad \quad \quad \forall p \in \mathbb{P}
         & \\
         &
         (2) \quad DSM_{h, t}^{up} = 0 \\
         & \quad \quad \quad \quad \forall h \in H_{DR}, t \in \mathbb{T}
         \quad \textrm{if} \quad e_{shift} = \textrm{False} \\
         &
         (3) \quad DSM_{t}^{do, shed} = 0 \\
         & \quad \quad \quad \quad \forall t \in \mathbb{T}
         \quad \textrm{if} \quad e_{shed} = \textrm{False} \\
         & \\
         &
-        (4) \quad \dot{E}_{t} = demand_{t} \cdot (invest + E_{exist}) \\
-        & \quad \quad \quad \quad + \displaystyle\sum_{h=1}^{H_{DR}}
-        (DSM_{h, t}^{up}
+        (4) \quad \dot{E}_{t} = demand_{t} \cdot demand_{max}(p) \\
+        & \displaystyle\sum_{h=1}^{H_{DR}} (DSM_{h, t}^{up}
         + DSM_{h, t}^{balanceDo} - DSM_{h, t}^{do, shift}
         - DSM_{h, t}^{balanceUp}) - DSM_{t}^{do, shed} \\
-        & \quad \quad \quad \quad \forall t \in \mathbb{T} \\
+        & \quad \quad \quad \quad \forall p, t \in \textrm{TIMEINDEX} \\
         & \\
         &
         (5) \quad DSM_{h, t}^{balanceDo} =
         \frac{DSM_{h, t - h}^{do, shift}}{\eta} \\
         & \quad \quad \quad \quad \forall h \in H_{DR}, t \in [h..T] \\
         & \\
         &
@@ -3325,24 +4031,22 @@
         &
         (8) \quad DSM_{h, t}^{up} = 0 \\
         & \quad \quad \quad \quad \forall h \in H_{DR}, t \in [T - h..T] \\
         & \\
         &
         (9) \quad \displaystyle\sum_{h=1}^{H_{DR}} (DSM_{h, t}^{do, shift}
         + DSM_{h, t}^{balanceUp}) + DSM_{t}^{do, shed}
-        \leq E_{t}^{do} \cdot (invest + E_{exist})
-        \cdot s_{flex, do} \\
-        & \quad \quad \quad \quad  \forall t \in \mathbb{T} \\
+        \leq E_{t}^{do} \cdot P_{total}(p) \\
+        & \quad \quad \quad \quad  \forall p, t \in \textrm{TIMEINDEX} \\
         & \\
         &
         (10) \quad \displaystyle\sum_{h=1}^{H_{DR}} (DSM_{h, t}^{up}
         + DSM_{h, t}^{balanceDo})
-        \leq E_{t}^{up} \cdot (invest + E_{exist})
-        \cdot s_{flex, up} \\
-        & \quad \quad \quad \quad \forall t \in \mathbb{T} \\
+        \leq E_{t}^{up} \cdot P_{total}(p) \\
+        & \quad \quad \quad \quad  \forall p, t \in \textrm{TIMEINDEX} \\
         & \\
         &
         (11) \quad \Delta t \cdot \displaystyle\sum_{h=1}^{H_{DR}}
         (DSM_{h, t}^{do, shift} - DSM_{h, t}^{balanceDo} \cdot \eta)
         = W_{t}^{levelDo} - W_{t-1}^{levelDo} \\
         & \quad \quad \quad \quad \forall t \in [1..T] \\
         & \\
@@ -3350,134 +4054,179 @@
         (12) \quad \Delta t \cdot \displaystyle\sum_{h=1}^{H_{DR}}
         (DSM_{h, t}^{up} \cdot \eta - DSM_{h, t}^{balanceUp})
         = W_{t}^{levelUp} - W_{t-1}^{levelUp} \\
         & \quad \quad \quad \quad \forall t \in [1..T] \\
         & \\
         &
         (13) \quad W_{t}^{levelDo} \leq \overline{E}_{t}^{do}
-        \cdot (invest + E_{exist})
-        \cdot s_{flex, do} \cdot t_{shift} \\
-        & \quad \quad \quad \quad \forall t \in \mathbb{T} \\
+        \cdot P_{total}(p) \cdot t_{shift} \\
+        & \quad \quad \quad \quad \forall p, t \in \textrm{TIMEINDEX} \\
         & \\
         &
         (14) \quad W_{t}^{levelUp} \leq \overline{E}_{t}^{up}
-        \cdot (invest + E_{exist})
-        \cdot s_{flex, up} \cdot t_{shift} \\
-        & \quad \quad \quad \quad \forall t \in \mathbb{T} \\
+        \cdot P_{total}(p)  \cdot t_{shift} \\
+        & \quad \quad \quad \quad \forall p, t \in \textrm{TIMEINDEX} \\
         & \\
         &
         (15) \quad \displaystyle\sum_{t=0}^{T} DSM_{t}^{do, shed}
-        \leq (invest + E_{exist})
-        \cdot s_{flex, do} \cdot \overline{E}_{t}^{do}
+        \leq P_{total}(p) \cdot \overline{E}_{t}^{do}
         \cdot t_{shed}
         \cdot n^{yearLimitShed} \\
         & \\
         &
         (16) \quad \displaystyle\sum_{t=0}^{T} \sum_{h=1}^{H_{DR}}
         DSM_{h, t}^{do, shift}
-        \leq (invest + E_{exist})
-        \cdot s_{flex, do} \cdot \overline{E}_{t}^{do}
+        \leq P_{total}(p)
+        \cdot \overline{E}_{t}^{do}
         \cdot t_{shift}
         \cdot n^{yearLimitShift} \\
         & \quad \quad \textrm{(optional constraint)} \\
         & \\
         &
         (17) \quad \displaystyle\sum_{t=0}^{T} \sum_{h=1}^{H_{DR}}
         DSM_{h, t}^{up}
-        \leq (invest + E_{exist})
-        \cdot s_{flex, up} \cdot \overline{E}_{t}^{up}
+        \leq P_{total}(p)
+        \cdot \overline{E}_{t}^{up}
         \cdot t_{shift}
         \cdot n^{yearLimitShift} \\
         & \quad \quad \textrm{(optional constraint)} \\
         &
         (18) \quad \displaystyle\sum_{h=1}^{H_{DR}} DSM_{h, t}^{do, shift}
-        \leq (invest + E_{exist})
-        \cdot s_{flex, do} \cdot \overline{E}_{t}^{do}
+        \leq P_{total}(p)
+        \cdot \overline{E}_{t}^{do}
         \cdot t_{shift} -
         \displaystyle\sum_{t'=1}^{t_{dayLimit}} \sum_{h=1}^{H_{DR}}
         DSM_{h, t - t'}^{do, shift} \\
         & \quad \quad \quad \quad \forall t \in [t-t_{dayLimit}..T] \\
         & \quad \quad \textrm{(optional constraint)} \\
         & \\
         &
         (19) \quad \displaystyle\sum_{h=1}^{H_{DR}} DSM_{h, t}^{up}
         \leq (invest + E_{exist})
-        \cdot s_{flex, up} \cdot \overline{E}_{t}^{up}
+        \cdot \overline{E}_{t}^{up}
         \cdot t_{shift} -
         \displaystyle\sum_{t'=1}^{t_{dayLimit}} \sum_{h=1}^{H_{DR}}
         DSM_{h, t - t'}^{up} \\
         & \quad \quad \quad \quad \forall t \in [t-t_{dayLimit}..T] \\
         & \quad \quad \textrm{(optional constraint)} \\
         & \\
         &
         (20) \quad \displaystyle\sum_{h=1}^{H_{DR}} (DSM_{h, t}^{up}
         + DSM_{h, t}^{balanceDo}
-        + DSM_{h, t}^{do, shift} + DSM_{h, t}^{balanceUp})
-        + DSM_{t}^{shed} \\
-        & \quad \quad \leq \max \{E_{t}^{up} \cdot s_{flex, up},
-        E_{t}^{do} \cdot s_{flex, do} \} \cdot (invest + E_{exist}) \\
-        & \quad \quad \quad \quad \forall t \in \mathbb{T} \\
+        + DSM_{h, t}^{do, shift} + DSM_{h, t}^{balanceUp}) \\
+        & + DSM_{t}^{shed}
+        \leq \max \{E_{t}^{up}, E_{t}^{do} \} \cdot P_{total}(p) \\
+        & \quad \quad \quad \quad \forall p, t \in \textrm{TIMEINDEX} \\
         & \quad \quad \textrm{(optional constraint)} \\
-
+        &
 
     Note
     ----
 
     For the sake of readability, the handling of indices is not
     displayed here. E.g. evaluating a variable for `t-L` may lead to a negative
     and therefore infeasible index.
     This is addressed by limiting the sums to non-negative indices within the
     model index bounds. Please refer to the constraints implementation
     themselves.
 
 
     **The following parts of the objective function are created:**
 
-    * Investment annuity:
+    *Standard model*
 
-    .. math::
-        &
-        invest \cdot costs_{invest} \\
+        * Investment annuity:
 
-    * Variable costs:
+            .. math::
+                P_{invest}(0) \cdot c_{invest}(0)
+
+        * Variable costs:
+
+            .. math::
+                &
+                (\sum_{h=1}^{H_{DR}} (DSM_{h, t}^{up} + DSM_{h, t}^{balanceDo})
+                \cdot cost_{t}^{dsm, up} \\
+                & + \sum_{h=1}^{H_{DR}} (DSM_{h, t}^{do, shift}
+                + DSM_{h, t}^{balanceUp})
+                \cdot cost_{t}^{dsm, do, shift} \\
+                & + DSM_{t}^{do, shed} \cdot cost_{t}^{dsm, do, shed})
+                \cdot \omega_{t} \\
+                & \quad \quad \quad \quad \forall t \in \mathbb{T} \\
+
+    *Multi-period model*
+
+        * Investment annuity:
+
+            .. math::
+                &
+                P_{invest}(p) \cdot A(c_{invest}(p), l, ir) \cdot l
+                \cdot DF^{-p} \\
+                &\\
+                &
+                \forall p \in \mathbb{P}
+
+        * :attr:`fixed_costs` not None for investments
+
+            .. math::
+                &
+                (\sum_{pp=year(p)}^{year(p)+l}
+                P_{invest}(p) \cdot c_{fixed}(pp) \cdot DF^{-pp})
+                \cdot DF^{-p} \\
+                &\\
+                &
+                \forall p \in \mathbb{P}
+
+        * Variable costs:
+
+            .. math::
+                &
+                (\sum_{h=1}^{H_{DR}} (DSM_{h, t}^{up} + DSM_{h, t}^{balanceDo})
+                \cdot cost_{t}^{dsm, up} \\
+                & + \sum_{h=1}^{H_{DR}} (DSM_{h, t}^{do, shift}
+                + DSM_{h, t}^{balanceUp})
+                \cdot cost_{t}^{dsm, do, shift} \\
+                & + DSM_{t}^{do, shed} \cdot cost_{t}^{dsm, do, shed})
+                \cdot \omega_{t} \cdot DF^{-p} \\
+                & \quad \quad \quad \quad \forall p, t \in \textrm{TIMEINDEX} \\
+
+    whereby:
+
+    * :math:`A(c_{invest,var}(p), l, ir)` A is the annuity for
+      investment expenses :math:`c_{invest}(p)` lifetime :math:`l`
+      and interest rate :math:`ir`
+    * :math:`DF=(1+dr)` is the discount factor with discount rate
+      :math:`dr`
+
+    See remarks in
+    :class:`oemof.solph.components.experimental._sink_dsm.SinkDSMOemofBlock`.
 
-    .. math::
-        &
-        (\sum_{h=1}^{H_{DR}} (DSM_{h, t}^{up} + DSM_{h, t}^{balanceDo})
-        \cdot cost_{t}^{dsm, up} \\
-        & + \sum_{h=1}^{H_{DR}} (DSM_{h, t}^{do, shift}
-        + DSM_{h, t}^{balanceUp})
-        \cdot cost_{t}^{dsm, do, shift} \\
-        & + DSM_{t}^{do, shed} \cdot cost_{t}^{dsm, do, shed})
-        \cdot \omega_{t} \\
-        & \quad \quad \quad \quad \forall t \in \mathbb{T} \\
 
     **Table: Symbols and attribute names of variables and parameters**
 
     * Please refer to
       :class:`oemof.solph.components.experimental._sink_dsm.SinkDSMDLRBlock`.
     * The following variables and parameters are exclusively used for
       investment modeling:
 
-        .. table:: Variables (V) and Parameters (P)
-            :widths: 1, 1, 1, 1
+    .. table:: Variables (V), Parameters (P) and Sets (S)
+        :widths: 25, 25, 10, 40
 
-            ================================= ======================== ==== =======================================
-            symbol                            attribute                type explanation
-            ================================= ======================== ==== =======================================
-            :math:`invest`                    `invest`                 V    | DSM capacity invested in
-                                                                            | Equals to the additionally installed capacity.
-                                                                            | The capacity share eligible for a shift is determined by flex share(s).
-            :math:`invest_{min}`              `investment.minimum`     P    minimum investment
-            :math:`invest_{max}`              `investment.maximum`     P    maximum investment
-            :math:`E_{exist}`                 `investment.existing`    P    existing DSM capacity
-            :math:`s_{flex, up}`              `flex_share_up`          P    share of invested capacity that may be shift upwards at maximum
-            :math:`s_{flex, do}`              `flex_share_do`          P    share of invested capacity that may be shift downwards at maximum
-            :math:`costs_{invest}`            `investment.ep_costs`    P    specific investment annuity
-            ================================= ======================== ==== =======================================
+        ================================= ======================== ==== =======================================
+        symbol                            attribute                type explanation
+        ================================= ======================== ==== =======================================
+        :math:`P_{invest}(p)`             `invest[p]`              V    | DSM capacity invested into in period p.
+                                                                        | Equals to the additionally shiftable resp. sheddable capacity.
+        :math:`invest_{min}(p)`           `investment.minimum[p]`  P    minimum investment in period p
+        :math:`invest_{max}(p)`           `investment.maximum[p]`  P    maximum investment in period p
+        :math:`P_{total}`                 `investment.total[p]`    P    total DSM capacity
+        :math:`costs_{invest}(p)`         `investment.ep_costs[p]` P    | specific investment annuity (standard model) resp.
+                                                                        | specific investment expenses (multi-period model)
+        :math:`\mathbb{P}`                                         S    Periods of the model
+        :math:`\textrm{TIMEINDEX}`                                 S    Timeindex set of the model (periods, timesteps)
+        ================================= ======================== ==== =======================================
 
     """  # noqa: E501
     CONSTRAINT_GROUP = True
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
@@ -3509,30 +4258,64 @@
         self.INVESTDR_H = Set(
             within=self.INVESTDR * self.H,
             initialize=[
                 (dr, h) for dr in map_INVESTDR_H for h in map_INVESTDR_H[dr]
             ],
         )
 
+        self.OVERALL_MAXIMUM_INVESTDSM = Set(
+            initialize=[
+                g for g in group if g.investment.overall_maximum is not None
+            ]
+        )
+
+        self.OVERALL_MINIMUM_INVESTDSM = Set(
+            initialize=[
+                g for g in group if g.investment.overall_minimum is not None
+            ]
+        )
+
+        self.EXISTING_INVESTDSM = Set(
+            initialize=[g for g in group if g.investment.existing is not None]
+        )
+
         #  ************* VARIABLES *****************************
 
         # Define bounds for investments in demand response
-        def _dr_investvar_bound_rule(block, g):
+        def _dr_investvar_bound_rule(block, g, p):
             """Rule definition to bound the
             invested demand response capacity `invest`.
             """
-            return g.investment.minimum, g.investment.maximum
+            return g.investment.minimum[p], g.investment.maximum[p]
 
         # Investment in DR capacity
         self.invest = Var(
             self.INVESTDR,
+            m.PERIODS,
             within=NonNegativeReals,
             bounds=_dr_investvar_bound_rule,
         )
 
+        # Total capacity
+        self.total = Var(self.INVESTDR, m.PERIODS, within=NonNegativeReals)
+
+        if m.es.periods is not None:
+            # Old capacity to be decommissioned (due to lifetime)
+            self.old = Var(self.INVESTDR, m.PERIODS, within=NonNegativeReals)
+
+            # Old endogenous capacity to be decommissioned (due to lifetime)
+            self.old_end = Var(
+                self.INVESTDR, m.PERIODS, within=NonNegativeReals
+            )
+
+            # Old exogenous capacity to be decommissioned (due to lifetime)
+            self.old_exo = Var(
+                self.INVESTDR, m.PERIODS, within=NonNegativeReals
+            )
+
         # Variable load shift down (capacity)
         self.dsm_do_shift = Var(
             self.INVESTDR_H, m.TIMESTEPS, initialize=0, within=NonNegativeReals
         )
 
         # Variable for load shedding (capacity)
         self.dsm_do_shed = Var(
@@ -3562,14 +4345,122 @@
         # Variable fictious DR storage level for upwards load shifts (energy)
         self.dsm_up_level = Var(
             self.INVESTDR, m.TIMESTEPS, initialize=0, within=NonNegativeReals
         )
 
         #  ************* CONSTRAINTS *****************************
 
+        # Handle unit lifetimes
+        def _total_capacity_rule(block):
+            """Rule definition for determining total installed
+            capacity (taking decommissioning into account)
+            """
+            for g in group:
+                for p in m.PERIODS:
+                    if p == 0:
+                        expr = (
+                            self.total[g, p]
+                            == self.invest[g, p] + g.investment.existing
+                        )
+                        self.total_dsm_rule.add((g, p), expr)
+                    else:
+                        expr = (
+                            self.total[g, p]
+                            == self.invest[g, p]
+                            + self.total[g, p - 1]
+                            - self.old[g, p]
+                        )
+                        self.total_dsm_rule.add((g, p), expr)
+
+        self.total_dsm_rule = Constraint(group, m.PERIODS, noruleinit=True)
+        self.total_dsm_rule_build = BuildAction(rule=_total_capacity_rule)
+
+        if m.es.periods is not None:
+
+            def _old_dsm_capacity_rule_end(block):
+                """Rule definition for determining old endogenously installed
+                capacity to be decommissioned due to reaching its lifetime
+                """
+                for g in group:
+                    lifetime = g.investment.lifetime
+                    for p in m.PERIODS:
+                        # No shutdown in first period
+                        if p == 0:
+                            expr = self.old_end[g, p] == 0
+                            self.old_dsm_rule_end.add((g, p), expr)
+                        elif lifetime <= m.es.periods_years[p]:
+                            # Obtain commissioning period
+                            comm_p = 0
+                            for k, v in enumerate(m.es.periods_years):
+                                if m.es.periods_years[p] - lifetime - v < 0:
+                                    # change of sign is detected
+                                    comm_p = k - 1
+                                    break
+                            expr = self.old_end[g, p] == self.invest[g, comm_p]
+                            self.old_dsm_rule_end.add((g, p), expr)
+                        else:
+                            expr = self.old_end[g, p] == 0
+                            self.old_dsm_rule_end.add((g, p), expr)
+
+            self.old_dsm_rule_end = Constraint(
+                group, m.PERIODS, noruleinit=True
+            )
+            self.old_dsm_rule_end_build = BuildAction(
+                rule=_old_dsm_capacity_rule_end
+            )
+
+            def _old_dsm_capacity_rule_exo(block):
+                """Rule definition for determining old exogenously given
+                capacity to be decommissioned due to reaching its lifetime
+                """
+                for g in group:
+                    age = g.investment.age
+                    lifetime = g.investment.lifetime
+                    is_decommissioned = False
+                    for p in m.PERIODS:
+                        # No shutdown in first period
+                        if p == 0:
+                            expr = self.old_exo[g, p] == 0
+                            self.old_dsm_rule_exo.add((g, p), expr)
+                        elif lifetime - age <= m.es.periods_years[p]:
+                            # Track decommissioning status
+                            if not is_decommissioned:
+                                expr = (
+                                    self.old_exo[g, p] == g.investment.existing
+                                )
+                                is_decommissioned = True
+                            else:
+                                expr = self.old_exo[g, p] == 0
+                            self.old_dsm_rule_exo.add((g, p), expr)
+                        else:
+                            expr = self.old_exo[g, p] == 0
+                            self.old_dsm_rule_exo.add((g, p), expr)
+
+            self.old_dsm_rule_exo = Constraint(
+                group, m.PERIODS, noruleinit=True
+            )
+            self.old_dsm_rule_exo_build = BuildAction(
+                rule=_old_dsm_capacity_rule_exo
+            )
+
+            def _old_dsm_capacity_rule(block):
+                """Rule definition for determining (overall) old capacity
+                to be decommissioned due to reaching its lifetime
+                """
+                for g in group:
+                    for p in m.PERIODS:
+                        expr = (
+                            self.old[g, p]
+                            == self.old_end[g, p] + self.old_exo[g, p]
+                        )
+                        self.old_dsm_rule.add((g, p), expr)
+
+            self.old_dsm_rule = Constraint(group, m.PERIODS, noruleinit=True)
+            self.old_dsm_rule_build = BuildAction(rule=_old_dsm_capacity_rule)
+
         def _shift_shed_vars_rule(block):
             """Force shifting resp. shedding variables to zero dependent
             on how boolean parameters for shift resp. shed eligibility
             are set.
             """
             for t in m.TIMESTEPS:
                 for g in group:
@@ -3593,37 +4484,37 @@
 
         # Relation between inflow and effective Sink consumption
         def _input_output_relation_rule(block):
             """Relation between input data and pyomo variables.
             The actual demand after DR.
             BusBlock outflow == Demand +- DR (i.e. effective Sink consumption)
             """
-            for t in m.TIMESTEPS:
+            for p, t in m.TIMEINDEX:
                 for g in group:
                     # outflow from bus
-                    lhs = m.flow[g.inflow, g, t]
+                    lhs = m.flow[g.inflow, g, p, t]
 
                     # Demand +- DR
                     rhs = (
-                        g.demand[t] * (self.invest[g] + g.investment.existing)
+                        g.demand[t] * g.max_demand[p]
                         + sum(
                             self.dsm_up[g, h, t]
                             + self.balance_dsm_do[g, h, t]
                             - self.dsm_do_shift[g, h, t]
                             - self.balance_dsm_up[g, h, t]
                             for h in g.delay_time
                         )
                         - self.dsm_do_shed[g, t]
                     )
 
                     # add constraint
-                    block.input_output_relation.add((g, t), (lhs == rhs))
+                    block.input_output_relation.add((g, p, t), (lhs == rhs))
 
         self.input_output_relation = Constraint(
-            group, m.TIMESTEPS, noruleinit=True
+            group, m.TIMEINDEX, noruleinit=True
         )
         self.input_output_relation_build = BuildAction(
             rule=_input_output_relation_rule
         )
 
         # Equation 4.8
         def capacity_balance_red_rule(block):
@@ -3647,15 +4538,15 @@
 
                                 # add constraint
                                 block.capacity_balance_red.add(
                                     (g, h, t), (lhs == rhs)
                                 )
 
                             # no balancing for the first timestep
-                            elif t == m.TIMESTEPS[1]:
+                            elif t == m.TIMESTEPS.at(1):
                                 lhs = self.balance_dsm_do[g, h, t]
                                 rhs = 0
 
                                 block.capacity_balance_red.add(
                                     (g, h, t), (lhs == rhs)
                                 )
 
@@ -3697,15 +4588,15 @@
 
                                 # add constraint
                                 block.capacity_balance_inc.add(
                                     (g, h, t), (lhs == rhs)
                                 )
 
                             # no balancing for the first timestep
-                            elif t == m.TIMESTEPS[1]:
+                            elif t == m.TIMESTEPS.at(1):
                                 lhs = self.balance_dsm_up[g, h, t]
                                 rhs = 0
 
                                 block.capacity_balance_inc.add(
                                     (g, h, t), (lhs == rhs)
                                 )
 
@@ -3733,15 +4624,15 @@
             """Prevent downwards shifts that cannot be balanced anymore
             within the optimization timeframe
             """
             for t in m.TIMESTEPS:
                 for g in group:
                     if g.fixes:
                         for h in g.delay_time:
-                            if t > m.TIMESTEPS[-1] - h:
+                            if t > m.TIMESTEPS.at(-1) - h:
                                 # no load reduction anymore (dsm_do_shift = 0)
                                 lhs = self.dsm_do_shift[g, h, t]
                                 rhs = 0
                                 block.no_comp_red.add((g, h, t), (lhs == rhs))
 
                     else:
                         pass  # return(Constraint.Skip)
@@ -3756,15 +4647,15 @@
             """Prevent upwards shifts that cannot be balanced anymore
             within the optimization timeframe
             """
             for t in m.TIMESTEPS:
                 for g in group:
                     if g.fixes:
                         for h in g.delay_time:
-                            if t > m.TIMESTEPS[-1] - h:
+                            if t > m.TIMESTEPS.at(-1) - h:
                                 # no load increase anymore (dsm_up = 0)
                                 lhs = self.dsm_up[g, h, t]
                                 rhs = 0
                                 block.no_comp_inc.add((g, h, t), (lhs == rhs))
 
                     else:
                         pass  # return(Constraint.Skip)
@@ -3775,63 +4666,55 @@
         self.no_comp_inc_build = BuildAction(rule=no_comp_inc_rule)
 
         # Equation 4.11
         def availability_red_rule(block):
             """Load reduction must be smaller than or equal to the
             (time-dependent) capacity limit
             """
-            for t in m.TIMESTEPS:
+            for p, t in m.TIMEINDEX:
                 for g in group:
                     # load reduction
                     lhs = (
                         sum(
                             self.dsm_do_shift[g, h, t]
                             + self.balance_dsm_up[g, h, t]
                             for h in g.delay_time
                         )
                         + self.dsm_do_shed[g, t]
                     )
 
                     # upper bound
-                    rhs = (
-                        g.capacity_down[t]
-                        * (self.invest[g] + g.investment.existing)
-                        * g.flex_share_down
-                    )
+                    rhs = g.capacity_down[t] * self.total[g, p]
 
                     # add constraint
-                    block.availability_red.add((g, t), (lhs <= rhs))
+                    block.availability_red.add((g, p, t), (lhs <= rhs))
 
-        self.availability_red = Constraint(group, m.TIMESTEPS, noruleinit=True)
+        self.availability_red = Constraint(group, m.TIMEINDEX, noruleinit=True)
         self.availability_red_build = BuildAction(rule=availability_red_rule)
 
         # Equation 4.12
         def availability_inc_rule(block):
             """Load increase must be smaller than or equal to the
             (time-dependent) capacity limit
             """
-            for t in m.TIMESTEPS:
+            for p, t in m.TIMEINDEX:
                 for g in group:
                     # load increase
                     lhs = sum(
                         self.dsm_up[g, h, t] + self.balance_dsm_do[g, h, t]
                         for h in g.delay_time
                     )
 
                     # upper bound
-                    rhs = (
-                        g.capacity_up[t]
-                        * (self.invest[g] + g.investment.existing)
-                        * g.flex_share_up
-                    )
+                    rhs = g.capacity_up[t] * self.total[g, p]
 
                     # add constraint
-                    block.availability_inc.add((g, t), (lhs <= rhs))
+                    block.availability_inc.add((g, p, t), (lhs <= rhs))
 
-        self.availability_inc = Constraint(group, m.TIMESTEPS, noruleinit=True)
+        self.availability_inc = Constraint(group, m.TIMEINDEX, noruleinit=True)
         self.availability_inc_build = BuildAction(rule=availability_inc_rule)
 
         # Equation 4.13
         def dr_storage_red_rule(block):
             """Fictious demand response storage level for load reductions
             transition equation
             """
@@ -3907,266 +4790,278 @@
         self.dr_storage_inc_build = BuildAction(rule=dr_storage_inc_rule)
 
         # Equation 4.15
         def dr_storage_limit_red_rule(block):
             """
             Fictious demand response storage level for load reduction limit
             """
-            for t in m.TIMESTEPS:
+            for p, t in m.TIMEINDEX:
                 for g in group:
                     if g.shift_eligibility:
                         # fictious demand response load reduction storage level
                         lhs = self.dsm_do_level[g, t]
 
                         # maximum (time-dependent) available shifting capacity
                         rhs = (
                             g.capacity_down_mean
-                            * (self.invest[g] + g.investment.existing)
-                            * g.flex_share_down
+                            * self.total[g, p]
                             * g.shift_time
                         )
 
                         # add constraint
-                        block.dr_storage_limit_red.add((g, t), (lhs <= rhs))
+                        block.dr_storage_limit_red.add((g, p, t), (lhs <= rhs))
 
                     else:
                         lhs = self.dsm_do_level[g, t]
                         # Force storage level and thus dsm_do_shift to 0
                         rhs = 0
 
                         # add constraint
-                        block.dr_storage_limit_red.add((g, t), (lhs <= rhs))
+                        block.dr_storage_limit_red.add((g, p, t), (lhs <= rhs))
 
         self.dr_storage_limit_red = Constraint(
-            group, m.TIMESTEPS, noruleinit=True
+            group, m.TIMEINDEX, noruleinit=True
         )
         self.dr_storage_level_red_build = BuildAction(
             rule=dr_storage_limit_red_rule
         )
 
         # Equation 4.16
         def dr_storage_limit_inc_rule(block):
-            """
-            Fictious demand response storage level for load increase limit
-            """
-            for t in m.TIMESTEPS:
+            """Fictious demand response storage level
+            for load increase limit"""
+            for p, t in m.TIMEINDEX:
                 for g in group:
                     # fictious demand response load reduction storage level
                     lhs = self.dsm_up_level[g, t]
 
                     # maximum (time-dependent) available shifting capacity
-                    rhs = (
-                        g.capacity_up_mean
-                        * (self.invest[g] + g.investment.existing)
-                        * g.flex_share_up
-                        * g.shift_time
-                    )
+                    rhs = g.capacity_up_mean * self.total[g, p] * g.shift_time
 
                     # add constraint
-                    block.dr_storage_limit_inc.add((g, t), (lhs <= rhs))
+                    block.dr_storage_limit_inc.add((g, p, t), (lhs <= rhs))
 
         self.dr_storage_limit_inc = Constraint(
-            group, m.TIMESTEPS, noruleinit=True
+            group, m.TIMEINDEX, noruleinit=True
         )
         self.dr_storage_level_inc_build = BuildAction(
             rule=dr_storage_limit_inc_rule
         )
 
         # Equation 4.17' -> load shedding
         def dr_yearly_limit_shed_rule(block):
             """Introduce overall annual (energy) limit for load shedding
             resp. overall limit for optimization timeframe considered
             A year limit in contrast to Gils (2015) is defined a mandatory
             parameter here in order to achieve an approach comparable
             to the others.
             """
             for g in group:
-                if g.shed_eligibility:
-                    # sum of all load reductions
-                    lhs = sum(self.dsm_do_shed[g, t] for t in m.TIMESTEPS)
+                for p in m.PERIODS:
+                    if g.shed_eligibility:
+                        # sum of all load reductions
+                        lhs = sum(
+                            self.dsm_do_shed[g, t]
+                            for pp, t in m.TIMEINDEX
+                            if pp == p
+                        )
 
-                    # year limit
-                    rhs = (
-                        g.capacity_down_mean
-                        * (self.invest[g] + g.investment.existing)
-                        * g.flex_share_down
-                        * g.shed_time
-                        * g.n_yearLimit_shed
-                    )
+                        # year limit
+                        rhs = (
+                            g.capacity_down_mean
+                            * self.total[g, p]
+                            * g.shed_time
+                            * g.n_yearLimit_shed
+                        )
 
-                    # add constraint
-                    block.dr_yearly_limit_shed.add(g, (lhs <= rhs))
+                        # add constraint
+                        block.dr_yearly_limit_shed.add((g, p), (lhs <= rhs))
 
-        self.dr_yearly_limit_shed = Constraint(group, noruleinit=True)
+        self.dr_yearly_limit_shed = Constraint(
+            group, m.PERIODS, noruleinit=True
+        )
         self.dr_yearly_limit_shed_build = BuildAction(
             rule=dr_yearly_limit_shed_rule
         )
 
         # ************* Optional Constraints *****************************
 
         # Equation 4.17
         def dr_yearly_limit_red_rule(block):
             """Introduce overall annual (energy) limit for load reductions
             resp. overall limit for optimization timeframe considered
             """
             for g in group:
                 if g.ActivateYearLimit:
-                    # sum of all load reductions
-                    lhs = sum(
-                        sum(self.dsm_do_shift[g, h, t] for h in g.delay_time)
-                        for t in m.TIMESTEPS
-                    )
+                    for p in m.PERIODS:
+                        # sum of all load reductions
+                        lhs = sum(
+                            sum(
+                                self.dsm_do_shift[g, h, t]
+                                for h in g.delay_time
+                            )
+                            for pp, t in m.TIMEINDEX
+                            if pp == p
+                        )
 
-                    # year limit
-                    rhs = (
-                        g.capacity_down_mean
-                        * (self.invest[g] + g.investment.existing)
-                        * g.flex_share_down
-                        * g.shift_time
-                        * g.n_yearLimit_shift
-                    )
+                        # year limit
+                        rhs = (
+                            g.capacity_down_mean
+                            * self.total[g, p]
+                            * g.shift_time
+                            * g.n_yearLimit_shift
+                        )
 
-                    # add constraint
-                    block.dr_yearly_limit_red.add(g, (lhs <= rhs))
+                        # add constraint
+                        block.dr_yearly_limit_red.add((g, p), (lhs <= rhs))
 
                 else:
                     pass  # return(Constraint.Skip)
 
-        self.dr_yearly_limit_red = Constraint(group, noruleinit=True)
+        self.dr_yearly_limit_red = Constraint(
+            group, m.PERIODS, noruleinit=True
+        )
         self.dr_yearly_limit_red_build = BuildAction(
             rule=dr_yearly_limit_red_rule
         )
 
         # Equation 4.18
         def dr_yearly_limit_inc_rule(block):
             """Introduce overall annual (energy) limit for load increases
             resp. overall limit for optimization timeframe considered
             """
             for g in group:
                 if g.ActivateYearLimit:
-                    # sum of all load increases
-                    lhs = sum(
-                        sum(self.dsm_up[g, h, t] for h in g.delay_time)
-                        for t in m.TIMESTEPS
-                    )
+                    for p in m.PERIODS:
+                        # sum of all load increases
+                        lhs = sum(
+                            sum(self.dsm_up[g, h, t] for h in g.delay_time)
+                            for pp, t in m.TIMEINDEX
+                            if pp == p
+                        )
 
-                    # year limit
-                    rhs = (
-                        g.capacity_up_mean
-                        * (self.invest[g] + g.investment.existing)
-                        * g.flex_share_up
-                        * g.shift_time
-                        * g.n_yearLimit_shift
-                    )
+                        # year limit
+                        rhs = (
+                            g.capacity_up_mean
+                            * self.total[g, p]
+                            * g.shift_time
+                            * g.n_yearLimit_shift
+                        )
 
-                    # add constraint
-                    block.dr_yearly_limit_inc.add(g, (lhs <= rhs))
+                        # add constraint
+                        block.dr_yearly_limit_inc.add((g, p), (lhs <= rhs))
 
                 else:
                     pass  # return(Constraint.Skip)
 
-        self.dr_yearly_limit_inc = Constraint(group, noruleinit=True)
+        self.dr_yearly_limit_inc = Constraint(
+            group, m.PERIODS, noruleinit=True
+        )
         self.dr_yearly_limit_inc_build = BuildAction(
             rule=dr_yearly_limit_inc_rule
         )
 
         # Equation 4.19
         def dr_daily_limit_red_rule(block):
             """Introduce rolling (energy) limit for load reductions
             This effectively limits DR utilization dependent on
             activations within previous hours.
             """
-            for t in m.TIMESTEPS:
+            for p, t in m.TIMEINDEX:
                 for g in group:
                     if g.ActivateDayLimit:
                         # main use case
                         if t >= g.t_dayLimit:
                             # load reduction
                             lhs = sum(
                                 self.dsm_do_shift[g, h, t]
                                 for h in g.delay_time
                             )
 
                             # daily limit
-                            rhs = g.capacity_down_mean * (
-                                self.invest[g] + g.investment.existing
-                            ) * g.flex_share_down * g.shift_time - sum(
+                            rhs = g.capacity_down_mean * self.total[
+                                g, p
+                            ] * g.shift_time - sum(
                                 sum(
                                     self.dsm_do_shift[g, h, t - t_dash]
                                     for h in g.delay_time
                                 )
                                 for t_dash in range(1, int(g.t_dayLimit) + 1)
                             )
 
                             # add constraint
-                            block.dr_daily_limit_red.add((g, t), (lhs <= rhs))
+                            block.dr_daily_limit_red.add(
+                                (g, p, t), (lhs <= rhs)
+                            )
 
                         else:
                             pass  # return(Constraint.Skip)
 
                     else:
                         pass  # return(Constraint.Skip)
 
         self.dr_daily_limit_red = Constraint(
-            group, m.TIMESTEPS, noruleinit=True
+            group, m.TIMEINDEX, noruleinit=True
         )
         self.dr_daily_limit_red_build = BuildAction(
             rule=dr_daily_limit_red_rule
         )
 
         # Equation 4.20
         def dr_daily_limit_inc_rule(block):
             """Introduce rolling (energy) limit for load increases
             This effectively limits DR utilization dependent on
             activations within previous hours.
             """
-            for t in m.TIMESTEPS:
+            for p, t in m.TIMEINDEX:
                 for g in group:
                     if g.ActivateDayLimit:
                         # main use case
                         if t >= g.t_dayLimit:
                             # load increase
                             lhs = sum(
                                 self.dsm_up[g, h, t] for h in g.delay_time
                             )
 
                             # daily limit
-                            rhs = g.capacity_up_mean * (
-                                self.invest[g] + g.investment.existing
-                            ) * g.flex_share_up * g.shift_time - sum(
+                            rhs = g.capacity_up_mean * self.total[
+                                g, p
+                            ] * g.shift_time - sum(
                                 sum(
                                     self.dsm_up[g, h, t - t_dash]
                                     for h in g.delay_time
                                 )
                                 for t_dash in range(1, int(g.t_dayLimit) + 1)
                             )
 
                             # add constraint
-                            block.dr_daily_limit_inc.add((g, t), (lhs <= rhs))
+                            block.dr_daily_limit_inc.add(
+                                (g, p, t), (lhs <= rhs)
+                            )
 
                         else:
                             pass  # return(Constraint.Skip)
 
                     else:
                         pass  # return(Constraint.Skip)
 
         self.dr_daily_limit_inc = Constraint(
-            group, m.TIMESTEPS, noruleinit=True
+            group, m.TIMEINDEX, noruleinit=True
         )
         self.dr_daily_limit_inc_build = BuildAction(
             rule=dr_daily_limit_inc_rule
         )
 
         # Addition: avoid simultaneous activations
         def dr_logical_constraint_rule(block):
             """Similar to equation 10 from Zerrahn and Schill (2015):
             The sum of upwards and downwards shifts may not be greater
             than the (bigger) capacity limit.
             """
-            for t in m.TIMESTEPS:
+            for p, t in m.TIMEINDEX:
                 for g in group:
                     if g.addition:
                         # sum of load increases and reductions
                         lhs = (
                             sum(
                                 self.dsm_up[g, h, t]
                                 + self.balance_dsm_do[g, h, t]
@@ -4174,61 +5069,207 @@
                                 + self.balance_dsm_up[g, h, t]
                                 for h in g.delay_time
                             )
                             + self.dsm_do_shed[g, t]
                         )
 
                         # maximum capacity eligibly for load shifting
-                        rhs = max(
-                            g.capacity_down[t] * g.flex_share_down,
-                            g.capacity_up[t] * g.flex_share_up,
-                        ) * (self.invest[g] + g.investment.existing)
+                        rhs = (
+                            max(
+                                g.capacity_down[t],
+                                g.capacity_up[t],
+                            )
+                            * self.total[g, p]
+                        )
 
                         # add constraint
-                        block.dr_logical_constraint.add((g, t), (lhs <= rhs))
+                        block.dr_logical_constraint.add(
+                            (g, p, t), (lhs <= rhs)
+                        )
 
                     else:
                         pass  # return(Constraint.Skip)
 
         self.dr_logical_constraint = Constraint(
-            group, m.TIMESTEPS, noruleinit=True
+            group, m.TIMEINDEX, noruleinit=True
         )
         self.dr_logical_constraint_build = BuildAction(
             rule=dr_logical_constraint_rule
         )
 
+        if m.es.periods is not None:
+
+            def _overall_dsm_maximum_investflow_rule(block):
+                """Rule definition for maximum overall investment
+                in investment case.
+                """
+                for g in self.OVERALL_MAXIMUM_INVESTDSM:
+                    for p in m.PERIODS:
+                        expr = self.total[g, p] <= g.investment.overall_maximum
+                        self.overall_dsm_maximum.add((g, p), expr)
+
+            self.overall_dsm_maximum = Constraint(
+                self.OVERALL_MAXIMUM_INVESTDSM, m.PERIODS, noruleinit=True
+            )
+
+            self.overall_maximum_build = BuildAction(
+                rule=_overall_dsm_maximum_investflow_rule
+            )
+
+            def _overall_minimum_dsm_investflow_rule(block):
+                """Rule definition for minimum overall investment
+                in investment case.
+
+                Note: This is only applicable for the last period
+                """
+                for g in self.OVERALL_MINIMUM_INVESTDSM:
+                    expr = (
+                        g.investment.overall_minimum
+                        <= self.total[g, m.PERIODS.at(-1)]
+                    )
+                    self.overall_minimum.add(g, expr)
+
+            self.overall_minimum = Constraint(
+                self.OVERALL_MINIMUM_INVESTDSM, noruleinit=True
+            )
+
+            self.overall_minimum_build = BuildAction(
+                rule=_overall_minimum_dsm_investflow_rule
+            )
+
     def _objective_expression(self):
         r"""Objective expression with variable and investment costs for DSM;
         Equation 4.23 from Gils (2015)
         """
         m = self.parent_block()
 
         investment_costs = 0
+        period_investment_costs = {p: 0 for p in m.PERIODS}
         variable_costs = 0
+        fixed_costs = 0
 
-        for g in self.INVESTDR:
-            if g.investment.ep_costs is not None:
-                investment_costs += self.invest[g] * g.investment.ep_costs
-            else:
-                raise ValueError("Missing value for investment costs!")
-            for t in m.TIMESTEPS:
-                variable_costs += (
-                    sum(
-                        self.dsm_up[g, h, t] + self.balance_dsm_do[g, h, t]
-                        for h in g.delay_time
+        if m.es.periods is None:
+            for g in self.INVESTDR:
+                for p in m.PERIODS:
+                    if g.investment.ep_costs is not None:
+                        investment_costs += (
+                            self.invest[g, p] * g.investment.ep_costs[p]
+                        )
+                    else:
+                        raise ValueError("Missing value for investment costs!")
+
+                for t in m.TIMESTEPS:
+                    variable_costs += (
+                        sum(
+                            self.dsm_up[g, h, t] + self.balance_dsm_do[g, h, t]
+                            for h in g.delay_time
+                        )
+                        * g.cost_dsm_up[t]
+                        * m.objective_weighting[t]
                     )
-                    * g.cost_dsm_up[t]
-                    * m.objective_weighting[t]
-                )
-                variable_costs += (
-                    sum(
-                        self.dsm_do_shift[g, h, t]
-                        + self.balance_dsm_up[g, h, t]
-                        for h in g.delay_time
+                    variable_costs += (
+                        sum(
+                            self.dsm_do_shift[g, h, t]
+                            + self.balance_dsm_up[g, h, t]
+                            for h in g.delay_time
+                        )
+                        * g.cost_dsm_down_shift[t]
+                        + self.dsm_do_shed[g, t] * g.cost_dsm_down_shed[t]
+                    ) * m.objective_weighting[t]
+
+        else:
+            msg = (
+                "You did not specify an interest rate.\n"
+                "It will be set equal to the discount_rate of {} "
+                "of the model as a default.\nThis corresponds to a "
+                "social planner point of view and does not reflect "
+                "microeconomic interest requirements."
+            )
+            for g in self.INVESTDR:
+                if g.investment.ep_costs is not None:
+                    lifetime = g.investment.lifetime
+                    interest = g.investment.interest_rate
+                    if interest == 0:
+                        warn(
+                            msg.format(m.discount_rate),
+                            debugging.SuspiciousUsageWarning,
+                        )
+                        interest = m.discount_rate
+                    for p in m.PERIODS:
+                        annuity = economics.annuity(
+                            capex=g.investment.ep_costs[p],
+                            n=lifetime,
+                            wacc=interest,
+                        )
+                        investment_costs_increment = (
+                            self.invest[g, p]
+                            * annuity
+                            * lifetime
+                            * ((1 + m.discount_rate) ** -m.es.periods_years[p])
+                        )
+                        investment_costs += investment_costs_increment
+                        period_investment_costs[
+                            p
+                        ] += investment_costs_increment
+                else:
+                    raise ValueError("Missing value for investment costs!")
+
+                for p, t in m.TIMEINDEX:
+                    variable_costs += (
+                        (
+                            sum(
+                                self.dsm_up[g, h, t]
+                                + self.balance_dsm_do[g, h, t]
+                                for h in g.delay_time
+                            )
+                            * g.cost_dsm_up[t]
+                        )
+                        * m.objective_weighting[t]
+                        * ((1 + m.discount_rate) ** -m.es.periods_years[p])
+                    )
+                    variable_costs += (
+                        (
+                            sum(
+                                self.dsm_do_shift[g, h, t]
+                                + self.balance_dsm_up[g, h, t]
+                                for h in g.delay_time
+                            )
+                            * g.cost_dsm_down_shift[t]
+                            + self.dsm_do_shed[g, t] * g.cost_dsm_down_shed[t]
+                        )
+                        * m.objective_weighting[t]
+                        * ((1 + m.discount_rate) ** -m.es.periods_years[p])
+                    )
+
+                if g.investment.fixed_costs[0] is not None:
+                    lifetime = g.investment.lifetime
+                    for p in m.PERIODS:
+                        fixed_costs += sum(
+                            self.invest[g, p]
+                            * g.investment.fixed_costs[pp]
+                            * ((1 + m.discount_rate) ** (-pp))
+                            for pp in range(
+                                m.es.periods_years[p],
+                                m.es.periods_years[p] + lifetime,
+                            )
+                        ) * ((1 + m.discount_rate) ** -m.es.periods_years[p])
+
+            for g in self.EXISTING_INVESTDSM:
+                if g.investment.fixed_costs[0] is not None:
+                    lifetime = g.investment.lifetime
+                    age = g.investment.age
+                    fixed_costs += sum(
+                        g.investment.existing
+                        * g.investment.fixed_costs[pp]
+                        * ((1 + m.discount_rate) ** (-pp))
+                        for pp in range(0, lifetime - age)
                     )
-                    * g.cost_dsm_down_shift[t]
-                    + self.dsm_do_shed[g, t] * g.cost_dsm_down_shed[t]
-                ) * m.objective_weighting[t]
 
-        self.cost = Expression(expr=investment_costs + variable_costs)
+        self.variable_costs = Expression(expr=variable_costs)
+        self.fixed_costs = Expression(expr=fixed_costs)
+        self.investment_costs = Expression(expr=investment_costs)
+        self.period_investment_costs = period_investment_costs
+        self.costs = Expression(
+            expr=investment_costs + variable_costs + fixed_costs
+        )
 
-        return self.cost
+        return self.costs
```

### Comparing `oemof.solph-0.5.1.dev0/src/oemof/solph/constraints/equate_flows.py` & `oemof.solph-0.5.1.dev1/src/oemof/solph/constraints/equate_flows.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,25 +39,25 @@
 
     Returns
     -------
     the updated model.
     """
 
     def _equate_flow_groups_rule(m):
-        for ts in m.TIMESTEPS:
-            sum1_t = sum(m.flow[fi, fo, ts] for fi, fo in flows1)
-            sum2_t = sum(m.flow[fi, fo, ts] for fi, fo in flows2)
+        for p, ts in m.TIMEINDEX:
+            sum1_t = sum(m.flow[fi, fo, p, ts] for fi, fo in flows1)
+            sum2_t = sum(m.flow[fi, fo, p, ts] for fi, fo in flows2)
             expr = sum1_t * factor1 == sum2_t
             if expr is not True:
-                getattr(m, name).add(ts, expr)
+                getattr(m, name).add((p, ts), expr)
 
     setattr(
         model,
         name,
-        po.Constraint(model.TIMESTEPS, noruleinit=True),
+        po.Constraint(model.TIMEINDEX, noruleinit=True),
     )
     setattr(
         model,
         name + "_build",
         po.BuildAction(rule=_equate_flow_groups_rule),
     )
```

### Comparing `oemof.solph-0.5.1.dev0/src/oemof/solph/constraints/equate_variables.py` & `oemof.solph-0.5.1.dev1/src/oemof/solph/constraints/equate_variables.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,16 +78,16 @@
     ...    outputs={bel1: solph.flows.Flow(
     ...        investment=solph.Investment(ep_costs=20))}))
     >>> om = solph.Model(energysystem)
     >>> line12 = energysystem.groups['powerline_1_2']
     >>> line21 = energysystem.groups['powerline_2_1']
     >>> solph.constraints.equate_variables(
     ...    om,
-    ...    om.InvestmentFlowBlock.invest[line12, bel2],
-    ...    om.InvestmentFlowBlock.invest[line21, bel1])
+    ...    om.InvestmentFlowBlock.invest[line12, bel2, 0],
+    ...    om.InvestmentFlowBlock.invest[line21, bel1, 0])
     """  # noqa: E501
     if name is None:
         name = "_".join(["equate", str(var1), str(var2)])
 
     def equate_variables_rule(m):
         return var1 * factor1 == var2
```

### Comparing `oemof.solph-0.5.1.dev0/src/oemof/solph/constraints/flow_count_limit.py` & `oemof.solph-0.5.1.dev1/src/oemof/solph/constraints/flow_count_limit.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     -------
     the updated model
 
     Note
     ----
     SimpleFlowBlock objects required to be NonConvex
 
+
     **Constraint:**
 
     .. math:: N_{X,min} \le \sum_{n \in F} X_n(t)
                         \le N_{X,max} \forall t \in T
 
     With `F` being the set of considered flows and
     `T` being the set of time steps.
```

### Comparing `oemof.solph-0.5.1.dev0/src/oemof/solph/constraints/investment_limit.py` & `oemof.solph-0.5.1.dev1/src/oemof/solph/constraints/investment_limit.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,25 +2,29 @@
 
 """Limits for investments.
 
 SPDX-FileCopyrightText: Uwe Krien <krien@uni-bremen.de>
 SPDX-FileCopyrightText: Simon Hilpert
 SPDX-FileCopyrightText: Patrik Schönfeldt
 SPDX-FileCopyrightText: Johannes Röder
+SPDX-FileCopyrightText: Johannes Kochems
+SPDX-FileCopyrightText: Johannes Giehl
 
 SPDX-License-Identifier: MIT
 
 """
 
 from pyomo import environ as po
 
+from oemof.solph._plumbing import sequence
+
 
 def investment_limit(model, limit=None):
     r"""Set an absolute limit for the total investment costs of an investment
-    optimization problem:
+    optimization problem (over all periods in case of a multi-period model):
 
     .. math:: \sum_{investment\_costs} \leq limit
 
     Parameters
     ----------
     model : oemof.solph._models.Model
         Model to which the constraint is added
@@ -32,50 +36,125 @@
         expr = 0
 
         if hasattr(m, "InvestmentFlowBlock"):
             expr += m.InvestmentFlowBlock.investment_costs
 
         if hasattr(m, "GenericInvestmentStorageBlock"):
             expr += m.GenericInvestmentStorageBlock.investment_costs
+
+        if hasattr(m, "SinkDSMOemofInvestmentBlock"):
+            expr += m.SinkDSMOemofInvestmentBlock.investment_costs
+
+        if hasattr(m, "SinkDSMDIWInvestmentBlock"):
+            expr += m.SinkDSMDIWInvestmentBlock.investment_costs
+
+        if hasattr(m, "SinkDSMDLRInvestmentBlock"):
+            expr += m.SinkDSMDLRInvestmentBlock.investment_costs
+
         return expr <= limit
 
     model.investment_limit = po.Constraint(rule=investment_rule)
 
     return model
 
 
+def investment_limit_per_period(model, limit=None):
+    r"""Set an absolute limit for the total investment costs of a
+    investment optimization problem for each period
+    of the multi-period problem.
+
+    .. math::
+        \sum_{investment\_costs(p)} \leq limit(p)
+        \forall p \in \textrm{PERIODS}
+
+    Parameters
+    ----------
+    model : oemof.solph.Model
+        Model to which the constraint is added
+    limit : sequence of float, :math:`limit(p)`
+        Absolute limit of the investment for each period
+        (i.e. RHS of constraint)
+    """
+
+    if model.es.periods is None:
+        msg = (
+            "investment_limit_per_period is only applicable "
+            "for multi-period models.\nIn order to create such a model, "
+            "explicitly set attribute `periods` of your energy system."
+        )
+        raise ValueError(msg)
+
+    if limit is not None:
+        limit = sequence(limit)
+    else:
+        msg = (
+            "You have to provide an investment limit for each period!\n"
+            "If you provide a scalar value, this will be applied as a "
+            "limit for each period."
+        )
+        raise ValueError(msg)
+
+    def investment_period_rule(m, p):
+        expr = 0
+
+        if hasattr(m, "InvestmentFlowBlock"):
+            expr += m.InvestmentFlowBlock.period_investment_costs[p]
+
+        if hasattr(m, "GenericInvestmentStorageBlock"):
+            expr += m.GenericInvestmentStorageBlock.period_investment_costs[p]
+
+        if hasattr(m, "SinkDSMOemofInvestmentBlock"):
+            expr += m.SinkDSMOemofInvestmentBlock.period_investment_costs[p]
+
+        if hasattr(m, "SinkDSMDIWInvestmentBlock"):
+            expr += m.SinkDSMDIWInvestmentBlock.period_investment_costs[p]
+
+        if hasattr(m, "SinkDSMDLRInvestmentBlock"):
+            expr += m.SinkDSMDLRInvestmentBlock.period_investment_costs[p]
+
+        return expr <= limit[p]
+
+    model.investment_limit_per_period = po.Constraint(
+        model.PERIODS, rule=investment_period_rule
+    )
+
+    return model
+
+
 def additional_investment_flow_limit(model, keyword, limit=None):
     r"""
     Global limit for investment flows weighted by an attribute keyword.
 
     This constraint is only valid for Flows not for components such as an
     investment storage.
 
     The attribute named by keyword has to be added to every Investment
     attribute of the flow you want to take into account.
     Total value of keyword attributes after optimization can be retrieved
     calling the `oemof.solph._models.Model.invest_limit_${keyword}()`.
 
-    .. math:: \sum_{i \in IF}  P_i \cdot w_i \leq limit
+    .. math::
+        \sum_{p \in \textrm{PERIODS}}
+        \sum_{i \in IF}  P_{i}(p) \cdot w_i \leq limit
 
     With `IF` being the set of InvestmentFlows considered for the integral
     limit.
 
     The symbols used are defined as follows
     (with Variables (V) and Parameters (P)):
 
-    +---------------+------------------------------------+------+--------------------------------------------------------------+
-    | symbol        | attribute                          | type | explanation                                                  |
-    +===============+====================================+======+==============================================================+
-    | :math:`P_{i}` | `InvestmentFlowBlock.invest[i, o]` | V    | installed capacity of investment flow                        |
-    +---------------+------------------------------------+------+--------------------------------------------------------------+
-    | :math:`w_i`   | `keyword`                          | P    | weight given to investment flow named according to `keyword` |
-    +---------------+------------------------------------+------+--------------------------------------------------------------+
-    | :math:`limit` | `limit`                            | P    | global limit given by keyword `limit`                        |
-    +---------------+------------------------------------+------+--------------------------------------------------------------+
+    +------------------+---------------------------------------+------+--------------------------------------------------------------+
+    | symbol           | attribute                             | type | explanation                                                  |
+    +==================+=======================================+======+==============================================================+
+    | :math:`P_{i}(p)` | `InvestmentFlowBlock.invest[i, o, p]` | V    | invested capacity of investment flow in period p             |
+    +------------------+---------------------------------------+------+--------------------------------------------------------------+
+    | :math:`w_i`      | `keyword`                             | P    | weight given to investment flow named according to `keyword` |
+    +------------------+---------------------------------------+------+--------------------------------------------------------------+
+    | :math:`limit`    | `limit`                               | P    | global limit given by keyword `limit`                        |
+    +------------------+---------------------------------------+------+--------------------------------------------------------------+
 
     Parameters
     ----------
     model : oemof.solph.Model
         Model to which constraints are added.
     keyword : attribute to consider
         All flows with Investment attribute containing the keyword will be
@@ -126,17 +205,18 @@
     limit_name = "invest_limit_" + keyword
 
     setattr(
         model,
         limit_name,
         po.Expression(
             expr=sum(
-                model.InvestmentFlowBlock.invest[inflow, outflow]
+                model.InvestmentFlowBlock.invest[inflow, outflow, p]
                 * getattr(invest_flows[inflow, outflow], keyword)
                 for (inflow, outflow) in invest_flows
+                for p in model.PERIODS
             )
         ),
     )
 
     setattr(
         model,
         limit_name + "_constraint",
```

### Comparing `oemof.solph-0.5.1.dev0/src/oemof/solph/constraints/shared_limit.py` & `oemof.solph-0.5.1.dev1/src/oemof/solph/constraints/shared_limit.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,29 +29,29 @@
       .. math::
         l_\mathrm{low} \le \sum v_i(t) \times w_i(t) \le l_\mathrm{up}
         \forall t
 
     Parameters
     ----------
     model : oemof.solph.Model
-        Model to which the constraint is added
+        Model to which the constraint is added.
     limit_name : string
         Name of the constraint to create
     quantity : pyomo.core.base.var.IndexedVar
         Shared Pyomo variable for all components of a type.
         (:math:`v_i(t)`)
     components : list of components
         list of components of the same type
     weights : list of numeric values
         has to have the same length as the list of components
         (:math:`w_i(t)`)
     lower_limit : numeric
         the lower limit (:math:`l_\mathrm{low}`)
     upper_limit : numeric
-        the lower limit (:math:`l_\mathrm{up}`)
+        the upper limit (:math:`l_\mathrm{up}`)
 
     Examples
     --------
     The constraint can e.g. be used to define a common storage
     that is shared between parties but that do not exchange
     energy on balance sheet.
     Thus, every party has their own bus and storage, respectively,
```

### Comparing `oemof.solph-0.5.1.dev0/src/oemof/solph/flows/_flow.py` & `oemof.solph-0.5.1.dev1/src/oemof/solph/flows/_flow.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,43 +8,49 @@
 SPDX-FileCopyrightText: Cord Kaldemeyer
 SPDX-FileCopyrightText: Stephan Günther
 SPDX-FileCopyrightText: Birgit Schachler
 SPDX-FileCopyrightText: jnnr
 SPDX-FileCopyrightText: jmloenneberga
 SPDX-FileCopyrightText: Pierre-François Duc
 SPDX-FileCopyrightText: Saeed Sayadi
+SPDX-FileCopyrightText: Johannes Kochems
 
 SPDX-License-Identifier: MIT
 
 """
 import math
+import numbers
 from collections.abc import Iterable
 from warnings import warn
 
 import numpy as np
 from oemof.network import network as on
+from oemof.tools import debugging
 
+from oemof.solph._options import Investment
 from oemof.solph._plumbing import sequence
 
 
 class Flow(on.Edge):
     r"""Defines a flow between two nodes.
 
     Keyword arguments are used to set the attributes of this flow. Parameters
     which are handled specially are noted below.
     For the case where a parameter can be either a scalar or an iterable, a
     scalar value will be converted to a sequence containing the scalar value at
-    every index. This sequence is then stored under the paramter's key.
+    every index. This sequence is then stored under the parameter's key.
 
     Parameters
     ----------
-    nominal_value : numeric, :math:`P_{nom}`
-        The nominal value of the flow. If this value is set the corresponding
-        optimization variable of the flow object will be bounded by this value
-        multiplied with min(lower bound)/max(upper bound).
+    nominal_value : numeric, :math:`P_{nom}` or
+            :class:`Investment <oemof.solph.options.Investment>`
+        The nominal value of the flow, either fixed or as an investement
+        optimisation. If this value is set the corresponding optimization
+        variable of the flow object will be bounded by this value
+        multiplied by min(lower bound)/max(upper bound).
     variable_costs : numeric (iterable or scalar), default: 0, :math:`c`
         The costs associated with one unit of the flow per hour. The
         costs for each timestep (:math:`P_t \cdot c \cdot \delta(t)`)
         will be added to the objective expression of the optimization problem.
     max : numeric (iterable or scalar), :math:`f_{max}`
         Normed maximum value of the flow. The flow absolute maximum will be
         calculated by multiplying :attr:`nominal_value` with :attr:`max`
@@ -55,39 +61,46 @@
         :attr:`nominal_value` to get the absolute value.
     positive_gradient_limit : numeric (iterable, scalar or None)
         the normed *upper bound* on the positive difference
         (`flow[t-1] < flow[t]`) of two consecutive flow values.
     negative_gradient_limit : numeric (iterable, scalar or None)
             the normed *upper bound* on the negative difference
             (`flow[t-1] > flow[t]`) of two consecutive flow values.
-
     full_load_time_max : numeric, :math:`t_{full\_load,max}`
         Upper bound on the summed flow expressed as the equivalent time that
         the flow would have to run at full capacity to yield the same sum. The
         value will be multiplied with the nominal_value to get the absolute
         limit.
     full_load_time_min : numeric, :math:`t_{full\_load,min}`
         Lower bound on the summed flow expressed as the equivalent time that
         the flow would have to run at full capacity to yield the same sum. The
         value will be multiplied with the nominal_value to get the absolute
         limit.
     integer : boolean
         Set True to bound the flow values to integers.
-    investment : :class:`Investment <oemof.solph.options.Investment>`
-        Object indicating if a nominal_value of the flow is determined by
-        the optimization problem. Note: This will refer all attributes to an
-        investment variable rather than to the nominal_value. The nominal_value
-        should not be set (or set to None) if an investment object is used.
     nonconvex : :class:`NonConvex <oemof.solph.options.NonConvex>`
         If a nonconvex flow object is added here, the flow constraints will
         be altered significantly as the mathematical model for the flow
         will be different, i.e. constraint etc. from
         :class:`~oemof.solph.flows._non_convex_flow_block.NonConvexFlowBlock`
         will be used instead of
         :class:`~oemof.solph.flows._simple_flow_block.SimpleFlowBlock`.
+    fixed_costs : numeric (iterable or scalar), :math:`c_{fixed}`
+        The fixed costs associated with a flow.
+        Note: These are only applicable for a multi-period model.
+    lifetime : int, :math:`l`
+        The lifetime of a flow (usually given in years);
+        once it reaches its lifetime (considering also
+        an initial age), the flow is forced to 0.
+        Note: Only applicable for a multi-period model.
+    age : int, :math:`a`
+        The initial age of a flow (usually given in years);
+        once it reaches its lifetime (considering also
+        an initial age), the flow is forced to 0.
+        Note: Only applicable for a multi-period model.
 
     Notes
     -----
     See :py:class:`~oemof.solph.flows._simple_flow.SimpleFlowBlock`
     for the variables, constraints and objective parts, that are created for
     a Flow object.
 
@@ -117,79 +130,108 @@
         fix=None,
         positive_gradient_limit=None,
         negative_gradient_limit=None,
         full_load_time_max=None,
         full_load_time_min=None,
         integer=False,
         bidirectional=False,
-        investment=None,
         nonconvex=None,
+        lifetime=None,
+        age=None,
+        fixed_costs=None,
         # --- BEGIN: To be removed for versions >= v0.6 ---
+        investment=None,
         summed_max=None,
         summed_min=None,
         # --- END ---
         custom_attributes=None,
     ):
         # TODO: Check if we can inherit from pyomo.core.base.var _VarData
         # then we need to create the var object with
         # pyomo.core.base.IndexedVarWithDomain before any SimpleFlowBlock
         # is created. E.g. create the variable in the energy system and
         # populate with information afterwards when creating objects.
 
         # --- BEGIN: The following code can be removed for versions >= v0.6 ---
+        if investment is not None:
+            msg = (
+                "For backward compatibility,"
+                " the option investment overwrites the option nominal_value."
+                + " Both options cannot be set at the same time."
+            )
+            if nominal_value is not None:
+                raise AttributeError(msg)
+            else:
+                warn(msg, FutureWarning)
+            nominal_value = investment
+
         msg = (
-            "\nThe parameter 'summed_{0}' is deprecated and will be removed "
-            "in version v0.6.\nRename the parameter to 'full_load_time_{0}', "
-            "to avoid this warning and future problems. "
+            "\nThe parameter '{0}' is deprecated and will be removed "
+            + "in version v0.6.\nUse the parameter '{1}', "
+            + "to avoid this warning and future problems. "
         )
         if summed_max is not None:
-            warn(msg.format("max"), FutureWarning)
+            warn(msg.format("summed_max", "full_load_time_max"), FutureWarning)
             full_load_time_max = summed_max
         if summed_min is not None:
-            warn(msg.format("min"), FutureWarning)
+            warn(msg.format("summed_min", "full_load_time_min"), FutureWarning)
             full_load_time_min = summed_min
         # --- END ---
 
         super().__init__()
 
         if custom_attributes is not None:
             for attribute, value in custom_attributes.items():
                 setattr(self, attribute, value)
 
+        self.nominal_value = None
+        self.investment = None
+
         infinite_error_msg = (
             "{} must be a finite value. Passing an infinite "
             "value is not allowed."
         )
-        if nominal_value is not None and not math.isfinite(nominal_value):
-            raise ValueError(infinite_error_msg.format("nominal_value"))
-        self.nominal_value = nominal_value
+        if isinstance(nominal_value, numbers.Real):
+            if not math.isfinite(nominal_value):
+                raise ValueError(infinite_error_msg.format("nominal_value"))
+            self.nominal_value = nominal_value
+        elif isinstance(nominal_value, Investment):
+            self.investment = nominal_value
+
+        if fixed_costs is not None:
+            msg = (
+                "Be aware that the fixed costs attribute is only\n"
+                "meant to be used for multi-period models.\n"
+                "If you wish to set up a multi-period model, explicitly "
+                "set the `periods` attribute of your energy system.\n"
+                "It has been decided to remove the `fixed_costs` "
+                "attribute with v0.2 for regular uses.\n"
+                "If you specify `fixed_costs` for a regular model, "
+                "it will simply be ignored."
+            )
+            warn(msg, debugging.SuspiciousUsageWarning)
 
+        self.fixed_costs = sequence(fixed_costs)
         self.positive_gradient_limit = sequence(positive_gradient_limit)
         self.negative_gradient_limit = sequence(negative_gradient_limit)
 
         self.full_load_time_max = full_load_time_max
         self.full_load_time_min = full_load_time_min
         self.integer = integer
-        self.investment = investment
         self.nonconvex = nonconvex
         self.bidirectional = bidirectional
+        self.lifetime = lifetime
+        self.age = age
 
         # It is not allowed to define min or max if fix is defined.
         if fix is not None and (min is not None or max is not None):
             raise AttributeError(
                 "It is not allowed to define `min`/`max` if `fix` is defined."
             )
 
-        # Checking for impossible attribute combinations
-        if self.investment and self.nominal_value is not None:
-            raise ValueError(
-                "Using the investment object the nominal_value"
-                " has to be set to None."
-            )
-
         need_nominal_value = [
             "fix",
             "full_load_time_max",
             "full_load_time_min",
             "min",
             "max",
         ]
@@ -202,15 +244,15 @@
                     the_attr = eval(attr)
                 if the_attr is not None:
                     raise AttributeError(
                         "If {} is set in a flow (except InvestmentFlow), "
                         "nominal_value must be set as well.\n"
                         "Otherwise, it won't have any effect.".format(attr)
                     )
-        # minumum will be set even without nominal limit
+        # minimum will be set even without nominal limit
 
         # maximum and minimum (absolute values) should be always set,
         # as nominal_value or invest might be defined later
         if max is None:
             max = 1
         if min is None:
             if bidirectional:
```

### Comparing `oemof.solph-0.5.1.dev0/src/oemof/solph/flows/_invest_non_convex_flow_block.py` & `oemof.solph-0.5.1.dev1/src/oemof/solph/flows/_invest_non_convex_flow_block.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 SPDX-FileCopyrightText: Saeed Sayadi
 SPDX-FileCopyrightText: Pierre-François Duc
 
 SPDX-License-Identifier: MIT
 
 """
 from pyomo.core import Binary
+from pyomo.core import BuildAction
 from pyomo.core import Constraint
 from pyomo.core import Expression
 from pyomo.core import NonNegativeReals
 from pyomo.core import Set
 from pyomo.core import Var
 
 from ._non_convex_flow_block import NonConvexFlowBlock
@@ -101,22 +102,23 @@
         )
 
         self._variables_for_non_convex_flows()
 
         # Investment-related variable similar to the
         # <class 'oemof.solph.flows.InvestmentFlow'> class.
 
-        def _investvar_bound_rule(block, i, o):
+        def _investvar_bound_rule(block, i, o, p):
             """Rule definition for bounds of the invest variable."""
             if (i, o) in self.INVEST_NON_CONVEX_FLOWS:
-                return 0, m.flows[i, o].investment.maximum
+                return 0, m.flows[i, o].investment.maximum[p]
 
         # Create the `invest` variable for the nonconvex investment flow.
         self.invest = Var(
             self.INVEST_NON_CONVEX_FLOWS,
+            m.PERIODS,
             within=NonNegativeReals,
             bounds=_investvar_bound_rule,
         )
 
         # `status_nominal` is a parameter which represents the
         # multiplication of a binary variable (`status`)
         # and a continuous variable (`invest` or `nominal_value`)
@@ -184,65 +186,66 @@
         r"""
         .. math::
             status\_nominal(i,o,t)
             \leq Y_{status}(t) \cdot P_{invest, max}\quad (1)
         """
         m = self.parent_block()
 
-        def _linearization_rule_invest_non_convex_one(_, i, o, t):
+        def _linearization_rule_invest_non_convex_one(_, i, o, p, t):
             expr = (
-                self.status[i, o, t] * m.flows[i, o].investment.maximum
+                self.status[i, o, t] * m.flows[i, o].investment.maximum[p]
                 >= self.status_nominal[i, o, t]
             )
             return expr
 
         return Constraint(
             self.MIN_FLOWS,
-            m.TIMESTEPS,
+            m.TIMEINDEX,
             rule=_linearization_rule_invest_non_convex_one,
         )
 
     def _linearised_investment_constraint_2(self):
         r"""
         .. math::
             status\_nominal(i,o,t) \leq P_{invest}\quad (2)
         """
 
         m = self.parent_block()
 
-        def _linearization_rule_invest_non_convex_two(_, i, o, t):
-            expr = self.invest[i, o] >= self.status_nominal[i, o, t]
+        def _linearization_rule_invest_non_convex_two(_, i, o, p, t):
+            expr = self.invest[i, o, p] >= self.status_nominal[i, o, t]
             return expr
 
         return Constraint(
             self.MIN_FLOWS,
-            m.TIMESTEPS,
+            m.TIMEINDEX,
             rule=_linearization_rule_invest_non_convex_two,
         )
 
     def _linearised_investment_constraint_3(self):
         r"""
         .. math::
             status\_nominal(i,o,t) \geq
             P_{invest} - (1 - Y_{status}(t)) \cdot P_{invest, max}\quad (3)
         """
 
         m = self.parent_block()
 
-        def _linearization_rule_invest_non_convex_three(_, i, o, t):
+        def _linearization_rule_invest_non_convex_three(_, i, o, p, t):
             expr = (
-                self.invest[i, o]
-                - (1 - self.status[i, o, t]) * m.flows[i, o].investment.maximum
+                self.invest[i, o, p]
+                - (1 - self.status[i, o, t])
+                * m.flows[i, o].investment.maximum[p]
                 <= self.status_nominal[i, o, t]
             )
             return expr
 
         return Constraint(
             self.MIN_FLOWS,
-            m.TIMESTEPS,
+            m.TIMEINDEX,
             rule=_linearization_rule_invest_non_convex_three,
         )
 
     def _objective_expression(self):
         r"""Objective expression for nonconvex investment flows.
 
             If `nonconvex.startup_costs` is set by the user:
@@ -266,18 +269,19 @@
         startup_costs = self._startup_costs()
         shutdown_costs = self._shutdown_costs()
         activity_costs = self._activity_costs()
         inactivity_costs = self._inactivity_costs()
         investment_costs = 0
 
         for i, o in self.INVEST_NON_CONVEX_FLOWS:
-            investment_costs += (
-                self.invest[i, o] * m.flows[i, o].investment.ep_costs
-                + m.flows[i, o].investment.offset
-            )
+            for p in m.PERIODS:
+                investment_costs += (
+                    self.invest[i, o, p] * m.flows[i, o].investment.ep_costs[p]
+                    + m.flows[i, o].investment.offset[p]
+                )
 
         self.investment_costs = Expression(expr=investment_costs)
 
         return (
             startup_costs
             + shutdown_costs
             + activity_costs
@@ -288,27 +292,47 @@
     def _minimum_invest_constraint(self):
         r"""
         .. math::
                 P_{invest, min} \le P_{invest}
         """
         m = self.parent_block()
 
-        def _min_invest_rule(_, i, o):
+        def _min_invest_rule(_):
             """Rule definition for applying a minimum investment"""
-            expr = m.flows[i, o].investment.minimum <= self.invest[i, o]
-            return expr
+            for i, o in self.INVEST_NON_CONVEX_FLOWS:
+                for p in m.PERIODS:
+                    expr = (
+                        m.flows[i, o].investment.minimum[p]
+                        <= self.invest[i, o, p]
+                    )
+                    self.minimum_investment.add((i, o, p), expr)
+
+        self.minimum_investment = Constraint(
+            self.INVEST_NON_CONVEX_FLOWS, m.PERIODS, noruleinit=True
+        )
+        self.minimum_rule_build = BuildAction(rule=_min_invest_rule)
 
-        return Constraint(self.INVEST_NON_CONVEX_FLOWS, rule=_min_invest_rule)
+        return self.minimum_investment
 
     def _maximum_invest_constraint(self):
         r"""
         .. math::
             P_{invest} \le P_{invest, max}
         """
         m = self.parent_block()
 
-        def _max_invest_rule(_, i, o):
+        def _max_invest_rule(_):
             """Rule definition for applying a minimum investment"""
-            expr = self.invest[i, o] <= m.flows[i, o].investment.maximum
-            return expr
+            for i, o in self.INVEST_NON_CONVEX_FLOWS:
+                for p in m.PERIODS:
+                    expr = (
+                        self.invest[i, o, p]
+                        <= m.flows[i, o].investment.maximum[p]
+                    )
+                    self.maximum_investment.add((i, o, p), expr)
+
+        self.maximum_investment = Constraint(
+            self.INVEST_NON_CONVEX_FLOWS, m.PERIODS, noruleinit=True
+        )
+        self.maximum_rule_build = BuildAction(rule=_max_invest_rule)
 
-        return Constraint(self.INVEST_NON_CONVEX_FLOWS, rule=_max_invest_rule)
+        return self.maximum_investment
```

### Comparing `oemof.solph-0.5.1.dev0/src/oemof/solph/flows/_non_convex_flow_block.py` & `oemof.solph-0.5.1.dev1/src/oemof/solph/flows/_non_convex_flow_block.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 SPDX-FileCopyrightText: Uwe Krien <krien@uni-bremen.de>
 SPDX-FileCopyrightText: Simon Hilpert
 SPDX-FileCopyrightText: Cord Kaldemeyer
 SPDX-FileCopyrightText: Patrik Schönfeldt
 SPDX-FileCopyrightText: Birgit Schachler
 SPDX-FileCopyrightText: jnnr
 SPDX-FileCopyrightText: jmloenneberga
-SPDX-FileCopyrightText: Johannes Kochems (jokochems)
+SPDX-FileCopyrightText: Johannes Kochems
 
 SPDX-License-Identifier: MIT
 
 """
 
 from pyomo.core import Binary
 from pyomo.core import BuildAction
@@ -125,18 +125,30 @@
             return 0
 
         startup_costs = self._startup_costs()
         shutdown_costs = self._shutdown_costs()
         activity_costs = self._activity_costs()
         inactivity_costs = self._inactivity_costs()
 
-        return (
-            startup_costs + shutdown_costs + activity_costs + inactivity_costs
+        self.activity_costs = Expression(expr=activity_costs)
+        self.inactivity_costs = Expression(expr=inactivity_costs)
+        self.startup_costs = Expression(expr=startup_costs)
+        self.shutdown_costs = Expression(expr=shutdown_costs)
+
+        self.costs = Expression(
+            expr=(
+                startup_costs
+                + shutdown_costs
+                + activity_costs
+                + inactivity_costs
+            )
         )
 
+        return self.costs
+
     def _sets_for_non_convex_flows(self, group):
         r"""Creates all sets for non-convex flows.
 
         MIN_FLOWS
             A subset of set NONCONVEX_FLOWS with the attribute `min`
             being not None in the first timestep.
         ACTIVITYCOSTFLOWS
@@ -277,40 +289,56 @@
             self.startup = Var(self.STARTUPFLOWS, m.TIMESTEPS, within=Binary)
 
         if self.SHUTDOWNFLOWS:
             self.shutdown = Var(self.SHUTDOWNFLOWS, m.TIMESTEPS, within=Binary)
 
         if self.POSITIVE_GRADIENT_FLOWS:
             self.positive_gradient = Var(
-                self.POSITIVE_GRADIENT_FLOWS, m.TIMESTEPS
+                self.POSITIVE_GRADIENT_FLOWS,
+                m.TIMESTEPS,
+                within=NonNegativeReals,
             )
 
         if self.NEGATIVE_GRADIENT_FLOWS:
             self.negative_gradient = Var(
-                self.NEGATIVE_GRADIENT_FLOWS, m.TIMESTEPS
+                self.NEGATIVE_GRADIENT_FLOWS,
+                m.TIMESTEPS,
+                within=NonNegativeReals,
             )
 
     def _startup_costs(self):
         r"""
         .. math::
             \sum_{i, o \in STARTUPFLOWS} \sum_t  Y_{startup}(t) \
             \cdot c_{startup}
         """
         startup_costs = 0
 
         if self.STARTUPFLOWS:
             m = self.parent_block()
 
-            for i, o in self.STARTUPFLOWS:
-                if m.flows[i, o].nonconvex.startup_costs[0] is not None:
-                    startup_costs += sum(
-                        self.startup[i, o, t]
-                        * m.flows[i, o].nonconvex.startup_costs[t]
-                        for t in m.TIMESTEPS
-                    )
+            if m.es.periods is None:
+                for i, o in self.STARTUPFLOWS:
+                    if m.flows[i, o].nonconvex.startup_costs[0] is not None:
+                        startup_costs += sum(
+                            self.startup[i, o, t]
+                            * m.flows[i, o].nonconvex.startup_costs[t]
+                            for t in m.TIMESTEPS
+                        )
+            else:
+                for i, o in self.STARTUPFLOWS:
+                    if m.flows[i, o].nonconvex.startup_costs[0] is not None:
+                        startup_costs += sum(
+                            self.startup[i, o, t]
+                            * m.flows[i, o].nonconvex.startup_costs[t]
+                            * m.objective_weighting[t]
+                            * ((1 + m.discount_rate) ** -m.es.periods_years[p])
+                            for p, t in m.TIMEINDEX
+                        )
+
             self.startup_costs = Expression(expr=startup_costs)
 
         return startup_costs
 
     def _shutdown_costs(self):
         r"""
         .. math::
@@ -318,21 +346,33 @@
             \cdot c_{shutdown}
         """
         shutdown_costs = 0
 
         if self.SHUTDOWNFLOWS:
             m = self.parent_block()
 
-            for i, o in self.SHUTDOWNFLOWS:
-                if m.flows[i, o].nonconvex.shutdown_costs[0] is not None:
-                    shutdown_costs += sum(
-                        self.shutdown[i, o, t]
-                        * m.flows[i, o].nonconvex.shutdown_costs[t]
-                        for t in m.TIMESTEPS
-                    )
+            if m.es.periods is None:
+                for i, o in self.SHUTDOWNFLOWS:
+                    if m.flows[i, o].nonconvex.shutdown_costs[0] is not None:
+                        shutdown_costs += sum(
+                            self.shutdown[i, o, t]
+                            * m.flows[i, o].nonconvex.shutdown_costs[t]
+                            for t in m.TIMESTEPS
+                        )
+            else:
+                for i, o in self.SHUTDOWNFLOWS:
+                    if m.flows[i, o].nonconvex.shutdown_costs[0] is not None:
+                        shutdown_costs += sum(
+                            self.shutdown[i, o, t]
+                            * m.flows[i, o].nonconvex.shutdown_costs[t]
+                            * m.objective_weighting[t]
+                            * ((1 + m.discount_rate) ** -m.es.periods_years[p])
+                            for p, t in m.TIMEINDEX
+                        )
+
             self.shutdown_costs = Expression(expr=shutdown_costs)
 
         return shutdown_costs
 
     def _activity_costs(self):
         r"""
         .. math::
@@ -340,21 +380,32 @@
             \cdot c_{activity}
         """
         activity_costs = 0
 
         if self.ACTIVITYCOSTFLOWS:
             m = self.parent_block()
 
-            for i, o in self.ACTIVITYCOSTFLOWS:
-                if m.flows[i, o].nonconvex.activity_costs[0] is not None:
-                    activity_costs += sum(
-                        self.status[i, o, t]
-                        * m.flows[i, o].nonconvex.activity_costs[t]
-                        for t in m.TIMESTEPS
-                    )
+            if m.es.periods is None:
+                for i, o in self.ACTIVITYCOSTFLOWS:
+                    if m.flows[i, o].nonconvex.activity_costs[0] is not None:
+                        activity_costs += sum(
+                            self.status[i, o, t]
+                            * m.flows[i, o].nonconvex.activity_costs[t]
+                            for t in m.TIMESTEPS
+                        )
+            else:
+                for i, o in self.ACTIVITYCOSTFLOWS:
+                    if m.flows[i, o].nonconvex.activity_costs[0] is not None:
+                        activity_costs += sum(
+                            self.status[i, o, t]
+                            * m.flows[i, o].nonconvex.activity_costs[t]
+                            * m.objective_weighting[t]
+                            * ((1 + m.discount_rate) ** -m.es.periods_years[p])
+                            for p, t in m.TIMEINDEX
+                        )
 
             self.activity_costs = Expression(expr=activity_costs)
 
         return activity_costs
 
     def _inactivity_costs(self):
         r"""
@@ -362,21 +413,33 @@
             \sum_{INACTIVITYCOSTFLOWS} \sum_t (1 - Y_{status}(t)) \
             \cdot c_{inactivity}
         """
         inactivity_costs = 0
 
         if self.INACTIVITYCOSTFLOWS:
             m = self.parent_block()
-            for i, o in self.INACTIVITYCOSTFLOWS:
-                if m.flows[i, o].nonconvex.inactivity_costs[0] is not None:
-                    inactivity_costs += sum(
-                        (1 - self.status[i, o, t])
-                        * m.flows[i, o].nonconvex.inactivity_costs[t]
-                        for t in m.TIMESTEPS
-                    )
+
+            if m.es.periods is None:
+                for i, o in self.INACTIVITYCOSTFLOWS:
+                    if m.flows[i, o].nonconvex.inactivity_costs[0] is not None:
+                        inactivity_costs += sum(
+                            (1 - self.status[i, o, t])
+                            * m.flows[i, o].nonconvex.inactivity_costs[t]
+                            for t in m.TIMESTEPS
+                        )
+            else:
+                for i, o in self.INACTIVITYCOSTFLOWS:
+                    if m.flows[i, o].nonconvex.inactivity_costs[0] is not None:
+                        inactivity_costs += sum(
+                            (1 - self.status[i, o, t])
+                            * m.flows[i, o].nonconvex.inactivity_costs[t]
+                            * m.objective_weighting[t]
+                            * ((1 + m.discount_rate) ** -m.es.periods_years[p])
+                            for p, t in m.TIMEINDEX
+                        )
 
             self.inactivity_costs = Expression(expr=inactivity_costs)
 
         return inactivity_costs
 
     @staticmethod
     def _time_step_allows_flexibility(t, max_up_down, last_step):
@@ -403,15 +466,15 @@
         m = self.parent_block()
 
         def min_downtime_rule(_, i, o, t):
             """
             Rule definition for min-downtime constraints of non-convex flows.
             """
             if self._time_step_allows_flexibility(
-                t, m.flows[i, o].nonconvex.max_up_down, m.TIMESTEPS[-1]
+                t, m.flows[i, o].nonconvex.max_up_down, m.TIMESTEPS.at(-1)
             ):
                 expr = 0
                 expr += (
                     self.status[i, o, t - 1] - self.status[i, o, t]
                 ) * m.flows[i, o].nonconvex.minimum_downtime
                 expr += -m.flows[i, o].nonconvex.minimum_downtime
                 expr += sum(
@@ -448,15 +511,15 @@
         m = self.parent_block()
 
         def _min_uptime_rule(_, i, o, t):
             """
             Rule definition for min-uptime constraints of non-convex flows.
             """
             if self._time_step_allows_flexibility(
-                t, m.flows[i, o].nonconvex.max_up_down, m.TIMESTEPS[-1]
+                t, m.flows[i, o].nonconvex.max_up_down, m.TIMESTEPS.at(-1)
             ):
                 expr = 0
                 expr += (
                     self.status[i, o, t] - self.status[i, o, t - 1]
                 ) * m.flows[i, o].nonconvex.minimum_uptime
                 expr += -sum(
                     self.status[i, o, t + u]
@@ -480,15 +543,15 @@
             \forall t \in \textrm{TIMESTEPS}, \\
             \forall \textrm{SHUTDOWNFLOWS}.
         """
         m = self.parent_block()
 
         def _shutdown_rule(_, i, o, t):
             """Rule definition for shutdown constraints of non-convex flows."""
-            if t > m.TIMESTEPS[1]:
+            if t > m.TIMESTEPS.at(1):
                 expr = (
                     self.shutdown[i, o, t]
                     >= self.status[i, o, t - 1] - self.status[i, o, t]
                 )
             else:
                 expr = (
                     self.shutdown[i, o, t]
@@ -506,15 +569,15 @@
             \forall t \in \textrm{TIMESTEPS}, \\
             \forall \textrm{STARTUPFLOWS}.
         """
         m = self.parent_block()
 
         def _startup_rule(_, i, o, t):
             """Rule definition for startup constraint of nonconvex flows."""
-            if t > m.TIMESTEPS[1]:
+            if t > m.TIMESTEPS.at(1):
                 expr = (
                     self.startup[i, o, t]
                     >= self.status[i, o, t] - self.status[i, o, t - 1]
                 )
             else:
                 expr = (
                     self.startup[i, o, t]
@@ -563,43 +626,43 @@
             P(t) \leq max(i, o, t) \cdot P_{nom} \
                 \cdot status(t), \\
             \forall t \in \textrm{TIMESTEPS}, \\
             \forall (i, o) \in \textrm{NONCONVEX_FLOWS}.
         """
         m = self.parent_block()
 
-        def _maximum_flow_rule(_, i, o, t):
+        def _maximum_flow_rule(_, i, o, p, t):
             """Rule definition for MILP maximum flow constraints."""
             expr = (
                 self.status_nominal[i, o, t] * m.flows[i, o].max[t]
-                >= m.flow[i, o, t]
+                >= m.flow[i, o, p, t]
             )
             return expr
 
-        return Constraint(self.MIN_FLOWS, m.TIMESTEPS, rule=_maximum_flow_rule)
+        return Constraint(self.MIN_FLOWS, m.TIMEINDEX, rule=_maximum_flow_rule)
 
     def _minimum_flow_constraint(self):
         r"""
         .. math::
             P(t) \geq min(i, o, t) \cdot P_{nom} \
                 \cdot Y_{status}(t), \\
             \forall (i, o) \in \textrm{NONCONVEX_FLOWS}, \\
             \forall t \in \textrm{TIMESTEPS}.
         """
         m = self.parent_block()
 
-        def _minimum_flow_rule(_, i, o, t):
+        def _minimum_flow_rule(_, i, o, p, t):
             """Rule definition for MILP minimum flow constraints."""
             expr = (
                 self.status_nominal[i, o, t] * m.flows[i, o].min[t]
-                <= m.flow[i, o, t]
+                <= m.flow[i, o, p, t]
             )
             return expr
 
-        return Constraint(self.MIN_FLOWS, m.TIMESTEPS, rule=_minimum_flow_rule)
+        return Constraint(self.MIN_FLOWS, m.TIMEINDEX, rule=_minimum_flow_rule)
 
     def _status_nominal_constraint(self):
         r"""
         .. math::
             P_{max,status}(t) =  Y_{status}(t) \cdot P_{nom}, \\
             \forall t \in \textrm{TIMESTEPS}.
         """
@@ -648,51 +711,111 @@
         self.max_startup_constr = self._max_startup_constraint()
         self.shutdown_constr = self._shutdown_constraint()
         self.max_shutdown_constr = self._max_shutdown_constraint()
         self.min_uptime_constr = self._min_uptime_constraint()
         self.min_downtime_constr = self._min_downtime_constraint()
 
         def _positive_gradient_flow_constraint(_):
-            r""" """
+            r"""Rule definition for positive gradient constraint."""
             for i, o in self.POSITIVE_GRADIENT_FLOWS:
-                for t in m.TIMESTEPS:
-                    if t > 0:
+                for index in range(1, len(m.TIMEINDEX) + 1):
+                    if m.TIMEINDEX[index][1] > 0:
                         lhs = (
-                            m.flow[i, o, t] * self.status[i, o, t]
-                            - m.flow[i, o, t - 1] * self.status[i, o, t - 1]
+                            m.flow[
+                                i,
+                                o,
+                                m.TIMEINDEX[index][0],
+                                m.TIMEINDEX[index][1],
+                            ]
+                            * self.status[i, o, m.TIMEINDEX[index][1]]
+                            - m.flow[
+                                i,
+                                o,
+                                m.TIMEINDEX[index - 1][0],
+                                m.TIMEINDEX[index - 1][1],
+                            ]
+                            * self.status[i, o, m.TIMEINDEX[index - 1][1]]
                         )
-                        rhs = self.positive_gradient[i, o, t]
+                        rhs = self.positive_gradient[
+                            i, o, m.TIMEINDEX[index][1]
+                        ]
                         self.positive_gradient_constr.add(
-                            (i, o, t), lhs <= rhs
+                            (
+                                i,
+                                o,
+                                m.TIMEINDEX[index][0],
+                                m.TIMEINDEX[index][1],
+                            ),
+                            lhs <= rhs,
                         )
                     else:
-                        pass  # return(Constraint.Skip)
+                        lhs = self.positive_gradient[i, o, 0]
+                        rhs = 0
+                        self.positive_gradient_constr.add(
+                            (
+                                i,
+                                o,
+                                m.TIMEINDEX[index][0],
+                                m.TIMEINDEX[index][1],
+                            ),
+                            lhs == rhs,
+                        )
 
         self.positive_gradient_constr = Constraint(
-            self.POSITIVE_GRADIENT_FLOWS, m.TIMESTEPS, noruleinit=True
+            self.POSITIVE_GRADIENT_FLOWS, m.TIMEINDEX, noruleinit=True
         )
         self.positive_gradient_build = BuildAction(
             rule=_positive_gradient_flow_constraint
         )
 
         def _negative_gradient_flow_constraint(_):
-            r""" """
+            r"""Rule definition for negative gradient constraint."""
             for i, o in self.NEGATIVE_GRADIENT_FLOWS:
-                for t in m.TIMESTEPS:
-                    if t > 0:
+                for index in range(1, len(m.TIMEINDEX) + 1):
+                    if m.TIMEINDEX[index][1] > 0:
                         lhs = (
-                            m.flow[i, o, t - 1] * self.status[i, o, t - 1]
-                            - m.flow[i, o, t] * self.status[i, o, t]
+                            m.flow[
+                                i,
+                                o,
+                                m.TIMEINDEX[index - 1][0],
+                                m.TIMEINDEX[index - 1][1],
+                            ]
+                            * self.status[i, o, m.TIMEINDEX[index - 1][1]]
+                            - m.flow[
+                                i,
+                                o,
+                                m.TIMEINDEX[index][0],
+                                m.TIMEINDEX[index][1],
+                            ]
+                            * self.status[i, o, m.TIMEINDEX[index][1]]
                         )
-                        rhs = self.negative_gradient[i, o, t]
+                        rhs = self.negative_gradient[
+                            i, o, m.TIMEINDEX[index][1]
+                        ]
                         self.negative_gradient_constr.add(
-                            (i, o, t), lhs <= rhs
+                            (
+                                i,
+                                o,
+                                m.TIMEINDEX[index][0],
+                                m.TIMEINDEX[index][1],
+                            ),
+                            lhs <= rhs,
                         )
                     else:
-                        pass  # return(Constraint.Skip)
+                        lhs = self.negative_gradient[i, o, 0]
+                        rhs = 0
+                        self.negative_gradient_constr.add(
+                            (
+                                i,
+                                o,
+                                m.TIMEINDEX[index][0],
+                                m.TIMEINDEX[index][1],
+                            ),
+                            lhs == rhs,
+                        )
 
         self.negative_gradient_constr = Constraint(
-            self.NEGATIVE_GRADIENT_FLOWS, m.TIMESTEPS, noruleinit=True
+            self.NEGATIVE_GRADIENT_FLOWS, m.TIMEINDEX, noruleinit=True
         )
         self.negative_gradient_build = BuildAction(
             rule=_negative_gradient_flow_constraint
         )
```

### Comparing `oemof.solph-0.5.1.dev0/src/oemof/solph/flows/experimental/_electrical_line.py` & `oemof.solph-0.5.1.dev1/src/oemof/solph/flows/experimental/_electrical_line.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 SPDX-FileCopyrightText: Simon Hilpert
 SPDX-FileCopyrightText: Cord Kaldemeyer
 SPDX-FileCopyrightText: Patrik Schönfeldt
 SPDX-FileCopyrightText: Johannes Röder
 SPDX-FileCopyrightText: jakob-wo
 SPDX-FileCopyrightText: gplssm
 SPDX-FileCopyrightText: jnnr
+SPDX-FileCopyrightText: Johannes Kochems
 
 SPDX-License-Identifier: MIT
 
 """
 
 import logging
 
@@ -102,18 +103,18 @@
 
     Note: This component is experimental. Use it with care.
 
     **The following constraints are created:**
 
     Linear relation :attr:`om.ElectricalLine.electrical_flow[n,t]`
         .. math::
-            flow(n, o, t) =  1 / reactance(n, t) \\cdot ()
-            voltage_angle(i(n), t) - volatage_angle(o(n), t), \\
-            \forall t \\in \\textrm{TIMESTEPS}, \\
-            \forall n \\in \\textrm{ELECTRICAL\_LINES}.
+            flow(n, o, p, t) =  1 / reactance(n, t) \cdot
+            voltage\_angle(i(n), t) - voltage\_angle(o(n), t), \\
+            \forall p, t \in \textrm{TIMEINDEX}, \\
+            \forall n \in \textrm{ELECTRICAL\_LINES}.
 
     TODO: Add equate constraint of flows
 
     **The following variable are created:**
 
     TODO: Add voltage angle variable
 
@@ -165,32 +166,32 @@
                 "No slack bus set,setting bus {0} as slack bus".format(
                     bus.label
                 )
             )
             bus.slack = True
 
         def _voltage_angle_relation(block):
-            for t in m.TIMESTEPS:
+            for p, t in m.TIMEINDEX:
                 for n in group:
                     if n.input.slack is True:
                         self.voltage_angle[n.output, t].value = 0
                         self.voltage_angle[n.output, t].fix()
                     try:
-                        lhs = m.flow[n.input, n.output, t]
+                        lhs = m.flow[n.input, n.output, p, t]
                         rhs = (
                             1
                             / n.reactance[t]
                             * (
                                 self.voltage_angle[n.input, t]
                                 - self.voltage_angle[n.output, t]
                             )
                         )
                     except ValueError:
                         raise ValueError(
                             "Error in constraint creation",
                             "of node {}".format(n.label),
                         )
-                    block.electrical_flow.add((n, t), (lhs == rhs))
+                    block.electrical_flow.add((n, p, t), (lhs == rhs))
 
-        self.electrical_flow = Constraint(group, m.TIMESTEPS, noruleinit=True)
+        self.electrical_flow = Constraint(group, m.TIMEINDEX, noruleinit=True)
 
         self.electrical_flow_build = BuildAction(rule=_voltage_angle_relation)
```

### Comparing `oemof.solph-0.5.1.dev0/src/oemof/solph/helpers.py` & `oemof.solph-0.5.1.dev1/src/oemof/solph/helpers.py`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/src/oemof/solph/processing.py` & `oemof.solph-0.5.1.dev1/src/oemof/solph/processing.py`

 * *Files 19% similar despite different names*

```diff
@@ -24,16 +24,15 @@
 from pyomo.core.base.piecewise import IndexedPiecewise
 from pyomo.core.base.var import Var
 
 from .helpers import flatten
 
 
 def get_tuple(x):
-    """
-    Get oemof tuple within iterable or create it.
+    """Get oemof tuple within iterable or create it
 
     Tuples from Pyomo are of type `(n, n, int)`, `(n, n)` and `(n, int)`.
     For single nodes `n` a tuple with one object `(n,)` is created.
     """
     for i in x:
         if isinstance(i, tuple):
             return i
@@ -42,46 +41,43 @@
 
     # for standalone variables, x is used as identifying tuple
     if isinstance(x, tuple):
         return x
 
 
 def get_timestep(x):
-    """
-    Get the timestep from oemof tuples.
+    """Get the timestep from oemof tuples
 
     The timestep from tuples `(n, n, int)`, `(n, n)`, `(n, int)` and (n,)
     is fetched as the last element. For time-independent data (scalars)
     zero ist returned.
     """
     if all(issubclass(type(n), Entity) for n in x):
         return 0
     else:
         return x[-1]
 
 
 def remove_timestep(x):
-    """
-    Remove the timestep from oemof tuples.
+    """Remove the timestep from oemof tuples
 
     The timestep is removed from tuples of type `(n, n, int)` and `(n, int)`.
     """
     if all(issubclass(type(n), Entity) for n in x):
         return x
     else:
         return x[:-1]
 
 
 def create_dataframe(om):
-    """
-    Create a result dataframe with all optimization data.
+    """Create a result DataFrame with all optimization data
 
-    Results from Pyomo are written into pandas DataFrame where separate columns
-    are created for the variable index e.g. for tuples of the flows and
-    components or the timesteps.
+    Results from Pyomo are written into one common pandas.DataFrame where
+    separate columns are created for the variable index e.g. for tuples
+    of the flows and components or the timesteps.
     """
     # get all pyomo variables including their block
     block_vars = list(
         set([bv.parent_component() for bv in om.component_data_objects(Var)])
     )
     var_dict = {}
     for bv in block_vars:
@@ -107,14 +103,19 @@
     # on which dimension the variable/parameter has (scalar/sequence).
     # columns for the oemof tuple and timestep are created
     df["oemof_tuple"] = df["pyomo_tuple"].map(get_tuple)
     df = df[df["oemof_tuple"].map(lambda x: x is not None)]
     df["timestep"] = df["oemof_tuple"].map(get_timestep)
     df["oemof_tuple"] = df["oemof_tuple"].map(remove_timestep)
 
+    # Use another call of remove timestep to get rid of period not needed
+    df.loc[df["variable_name"] == "flow", "oemof_tuple"] = df.loc[
+        df["variable_name"] == "flow", "oemof_tuple"
+    ].map(remove_timestep)
+
     # order the data by oemof tuple and timestep
     df = df.sort_values(["oemof_tuple", "timestep"], ascending=[True, True])
 
     # drop empty decision variables
     df = df.dropna(subset=["value"])
 
     return df
@@ -168,38 +169,69 @@
                 "in your input data."
             )
             raise type(e)(
                 str(e) + msg.format(k[0].label, k[1].label)
             ).with_traceback(sys.exc_info()[2])
 
 
+def set_sequences_index(df, result_index):
+    try:
+        df.index = result_index
+    except ValueError:
+        try:
+            df = df[:-1]
+            df.index = result_index
+        except ValueError:
+            raise ValueError("Results extraction failed!")
+
+
 def results(model, remove_last_time_point=False):
-    """
-    Create a result dictionary from the result DataFrame.
+    """Create a nested result dictionary from the result DataFrame
 
-    Results from Pyomo are written into a dictionary of pandas objects where
-    a Series holds all scalar values and a dataframe all sequences for nodes
-    and flows.
-    The dictionary is keyed by the nodes e.g. `results[idx]['scalars']`
-    and flows e.g. `results[n, n]['sequences']`.
+    The already rearranged results from Pyomo from the result DataFrame are
+    transferred into a nested dictionary of pandas objects.
+    The first level key of that dictionary is a node (denoting the respective
+    flow or component).
+
+    The second level keys are "sequences" and "scalars" for a *standard model*:
+
+    * A pd.DataFrame holds all results that are time-dependent, i.e. given as
+      a sequence and can be indexed with the energy system's timeindex.
+    * A pd.Series holds all scalar values which are applicable for timestep 0
+      (i.e. investments).
+
+    For a *multi-period model*, the second level key for "sequences" remains
+    the same while instead of "scalars", the key "period_scalars" is used:
+
+    * For sequences, see standard model.
+    * Instead of a pd.Series, a pd.DataFrame holds scalar values indexed
+      by periods. These hold investment-related variables.
+
+    Examples
+    --------
+    * *Standard model*: `results[idx]['scalars']`
+      and flows `results[n, n]['sequences']`.
+    * *Multi-period model*: `results[idx]['period_scalars']`
+      and flows `results[n, n]['sequences']`.
 
     Parameters
     ----------
     model : oemof.solph.BaseModel
         A solved oemof.solph model.
     remove_last_time_point : bool
         The last time point of all TIMEPOINT variables is removed to get the
         same length as the TIMESTEP (interval) variables without getting
         nan-values. By default, the last time point is removed if it has not
         been defined by the user in the EnergySystem but inferred. If all
-        time points has been defined explicitly by the user the last time point
-        will not be removed by default. In that case all interval variables
-        will get one row with nan-values to have the same index for all
-        variables.
+        time points have been defined explicitly by the user the last time
+        point will not be removed by default. In that case all interval
+        variables will get one row with nan-values to have the same index
+        for all variables.
     """
+    # Extraction steps that are the same for both model types
     df = create_dataframe(model)
 
     # create a dict of dataframes keyed by oemof tuples
     df_dict = {
         k
         if len(k) > 1
         else (k[0], None): v[["timestep", "variable_name", "value"]]
@@ -211,15 +243,90 @@
         result_index = list(range(len(model.es.timeincrement) + 1))
     else:
         result_index = model.es.timeindex
 
     # create final result dictionary by splitting up the dataframes in the
     # dataframe dict into a series for scalar data and dataframe for sequences
     result = {}
-    if remove_last_time_point is True:
+
+    # Standard model results extraction
+    if model.es.periods is None:
+        result = _extract_standard_model_result(
+            df_dict, result, result_index, remove_last_time_point
+        )
+        scalars_col = "scalars"
+
+    # Results extraction for a multi-period model
+    else:
+        period_indexed = ["invest", "total", "old", "old_end", "old_exo"]
+
+        result = _extract_multi_period_model_result(
+            model,
+            df_dict,
+            period_indexed,
+            result,
+            result_index,
+            remove_last_time_point,
+        )
+        scalars_col = "period_scalars"
+
+    # add dual variables for bus constraints
+    if model.dual is not None:
+        grouped = groupby(
+            sorted(model.BusBlock.balance.iterkeys()), lambda p: p[0]
+        )
+        for bus, timeindex in grouped:
+            duals = [
+                model.dual[model.BusBlock.balance[bus, p, t]]
+                for _, p, t in timeindex
+            ]
+            if model.es.periods is None:
+                df = pd.DataFrame({"duals": duals}, index=result_index[:-1])
+            # TODO: Align with standard model
+            else:
+                df = pd.DataFrame({"duals": duals}, index=result_index)
+            if (bus, None) not in result.keys():
+                result[(bus, None)] = {
+                    "sequences": df,
+                    scalars_col: pd.Series(dtype=float),
+                }
+            else:
+                result[(bus, None)]["sequences"]["duals"] = duals
+
+    return result
+
+
+def _extract_standard_model_result(
+    df_dict, result, result_index, remove_last_time_point
+):
+    """Extract and return the results of a standard model
+
+    * Optionally remove last time point or include it elsewise.
+    * Set index to timeindex and pivot results such that values are displayed
+      for the respective variables. Reindex with the energy system's timeindex.
+    * Filter for columns with nan values to retrieve scalar variables. Split
+      up the DataFrame into sequences and scalars and return it.
+
+    Parameters
+    ----------
+    df_dict : dict
+        dictionary of results DataFrames
+    result : dict
+        dictionary to store the results
+    result_index : pd.DatetimeIndex
+        timeindex to use for the results (derived from EnergySystem)
+    remove_last_time_point : bool
+        if True, remove the last time point
+
+    Returns
+    -------
+    result : dict
+        dictionary with results stored
+    """
+    if remove_last_time_point:
         # The values of intervals belong to the time at the beginning of the
         # interval.
         for k in df_dict:
             df_dict[k].set_index("timestep", inplace=True)
             df_dict[k] = df_dict[k].pivot(
                 columns="variable_name", values="value"
             )
@@ -233,32 +340,85 @@
             )
             # Add empty row with nan at the end of the table by adding 1 to the
             # last value of the numeric index.
             df_dict[k].loc[df_dict[k].index[-1] + 1, :] = np.nan
             set_result_index(df_dict, k, result_index)
             result[k] = divide_scalars_sequences(df_dict, k)
 
-    # add dual variables for bus constraints
-    if model.dual is not None:
-        grouped = groupby(
-            sorted(model.BusBlock.balance.iterkeys()), lambda p: p[0]
-        )
-        for bus, timesteps in grouped:
-            duals = [
-                model.dual[model.BusBlock.balance[bus, t]]
-                for _, t in timesteps
-            ]
-            df = pd.DataFrame({"duals": duals}, index=result_index[:-1])
-            if (bus, None) not in result.keys():
-                result[(bus, None)] = {
-                    "sequences": df,
-                    "scalars": pd.Series(dtype=float),
-                }
-            else:
-                result[(bus, None)]["sequences"]["duals"] = duals
+    return result
+
+
+def _extract_multi_period_model_result(
+    model,
+    df_dict,
+    period_indexed=None,
+    result=None,
+    result_index=None,
+    remove_last_time_point=False,
+):
+    """Extract and return the results of a multi-period model
+
+    Difference to standard model is in the way, scalar values are extracted
+    since they now depend on periods.
+
+    Parameters
+    ----------
+    model : oemof.solph.models.Model
+        The optimization model
+    df_dict : dict
+        dictionary of results DataFrames
+    period_indexed : list
+        list of variables that are indexed by periods
+    result : dict
+        dictionary to store the results
+    result_index : pd.DatetimeIndex
+        timeindex to use for the results (derived from EnergySystem)
+    remove_last_time_point : bool
+        if True, remove the last time point
+
+    Returns
+    -------
+    result : dict
+        dictionary with results stored
+    """
+    for k in df_dict:
+        df_dict[k].set_index("timestep", inplace=True)
+        df_dict[k] = df_dict[k].pivot(columns="variable_name", values="value")
+        # Split data set
+        period_cols = [
+            col for col in df_dict[k].columns if col in period_indexed
+        ]
+        # map periods to their start years for displaying period results
+        d = {
+            key: val + model.es.periods[0].min().year
+            for key, val in enumerate(model.es.periods_years)
+        }
+        period_scalars = df_dict[k].loc[:, period_cols].dropna()
+        sequences = df_dict[k].loc[
+            :, [col for col in df_dict[k].columns if col not in period_cols]
+        ]
+        if remove_last_time_point:
+            set_sequences_index(sequences, result_index[:-1])
+        else:
+            set_sequences_index(sequences, result_index)
+        if period_scalars.empty:
+            period_scalars = pd.DataFrame(index=d.values())
+        try:
+            period_scalars.rename(index=d, inplace=True)
+            period_scalars.index.name = "period"
+            result[k] = {
+                "period_scalars": period_scalars,
+                "sequences": sequences,
+            }
+        except IndexError:
+            error_message = (
+                "Some indices seem to be not matching.\n"
+                "Cannot properly extract model results."
+            )
+            raise IndexError(error_message)
 
     return result
 
 
 def convert_keys_to_strings(result, keep_none_type=False):
     """
     Convert the dictionary keys to strings.
```

### Comparing `oemof.solph-0.5.1.dev0/src/oemof/solph/views.py` & `oemof.solph-0.5.1.dev1/src/oemof/solph/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 See examples for to learn about the possible usage of the provided functions.
 
 SPDX-FileCopyrightText: Uwe Krien <krien@uni-bremen.de>
 SPDX-FileCopyrightText: Simon Hilpert
 SPDX-FileCopyrightText: Cord Kaldemeyer
 SPDX-FileCopyrightText: Stephan Günther
 SPDX-FileCopyrightText: henhuy
+SPDX-FileCopyrightText: Johannes Kochems
 
 SPDX-License-Identifier: MIT
 
 """
 import logging
 from collections import OrderedDict
 from enum import Enum
@@ -25,16 +26,18 @@
 
 
 def node(results, node, multiindex=False, keep_none_type=False):
     """
     Obtain results for a single node e.g. a Bus or Component.
 
     Either a node or its label string can be passed.
-    Results are written into a dictionary which is keyed by 'scalars' and
-    'sequences' holding respective data in a pandas Series and DataFrame.
+    Results are written into a dictionary which is keyed by 'scalars'
+    (resp. 'periods_scalars' for a multi-period model) and
+    'sequences' holding respective data in a pandas Series (resp. DataFrame)
+    and DataFrame.
     """
 
     def replace_none(col_list, reverse=False):
         replacement = (
             (None, NONE_REPLACEMENT_STR)
             if reverse
             else (NONE_REPLACEMENT_STR, None)
@@ -54,53 +57,58 @@
     # convert to keys if only a string is passed
     if type(node) is str:
         results = convert_keys_to_strings(results, keep_none_type)
 
     filtered = {}
 
     # create a series with tuples as index labels for scalars
+    scalars_col = "scalars"
+    # Check for multi-period model (different naming)
+    if "period_scalars" in list(list(results.values())[0].keys()):
+        scalars_col = "period_scalars"
+
     scalars = {
-        k: v["scalars"]
+        k: v[scalars_col]
         for k, v in results.items()
-        if node in k and not v["scalars"].empty
+        if node in k and not v[scalars_col].empty
     }
     if scalars:
         # aggregate data
-        filtered["scalars"] = pd.concat(scalars.values(), axis=0)
+        filtered[scalars_col] = pd.concat(scalars.values(), axis=0)
         # assign index values
         idx = {
-            k: [c for c in v["scalars"].index]
+            k: [c for c in v[scalars_col].index]
             for k, v in results.items()
-            if node in k and not v["scalars"].empty
+            if node in k and not v[scalars_col].empty
         }
         idx = [tuple((k, m) for m in v) for k, v in idx.items()]
         idx = [i for sublist in idx for i in sublist]
-        filtered["scalars"].index = idx
+        filtered[scalars_col].index = idx
 
         # Sort index
         # (if Nones are present, they have to be replaced while sorting)
         if keep_none_type:
-            filtered["scalars"].index = replace_none(
-                filtered["scalars"].index.tolist()
+            filtered[scalars_col].index = replace_none(
+                filtered[scalars_col].index.tolist()
             )
-        filtered["scalars"].sort_index(axis=0, inplace=True)
+        filtered[scalars_col].sort_index(axis=0, inplace=True)
         if keep_none_type:
-            filtered["scalars"].index = replace_none(
-                filtered["scalars"].index.tolist(), True
+            filtered[scalars_col].index = replace_none(
+                filtered[scalars_col].index.tolist(), True
             )
 
         if multiindex:
             idx = pd.MultiIndex.from_tuples(
                 [
                     tuple([row[0][0], row[0][1], row[1]])
-                    for row in filtered["scalars"].index
+                    for row in filtered[scalars_col].index
                 ]
             )
             idx.set_names(["from", "to", "type"], inplace=True)
-            filtered["scalars"].index = idx
+            filtered[scalars_col].index = idx
 
     # create a dataframe with tuples as column labels for sequences
     sequences = {
         k: v["sequences"]
         for k, v in results.items()
         if node in k and not v["sequences"].empty
     }
@@ -221,14 +229,27 @@
     Parameters
     ----------
     results: dict
         A result dictionary from a solved oemof.solph.Model object
     node_type: oemof.solph class
         Specifies the type for which node weights should be collected,
         e.g. solph.components.GenericStorage
+
+    Example
+    --------
+    ::
+
+        from oemof.solph import views
+
+        # solve oemof model 'm'
+        # Then collect node weights
+        views.node_weight_by_type(
+            m.results(),
+           node_type=solph.components.GenericStorage
+        )
     """
 
     group = {
         k: v["sequences"]
         for k, v in results.items()
         if isinstance(k[0], node_type) and k[1] is None
     }
@@ -252,14 +273,28 @@
     ----------
     results: dict
         A result dictionary from a solved oemof.solph.Model object
     node_type: oemof.solph class
         Specifies the type of the node for that inputs are selected,
         e.g. solph.components.Sink
     droplevel: list
+
+    Examples
+    -----
+    ::
+
+        from oemof import solph
+        from oemof.solph import views
+
+        # solve oemof solph model 'm'
+        # Then collect node weights
+        views.node_input_by_type(
+            m.results(),
+            node_type=solph.components.Sink
+        )
     """
     if droplevel is None:
         droplevel = []
 
     group = {
         k: v["sequences"]
         for k, v in results.items()
@@ -282,14 +317,28 @@
     ----------
     results: dict
         A result dictionary from a solved oemof.solph.Model object
     node_type: oemof.solph class
         Specifies the type of the node for that outputs are selected,
         e.g. solph.components.Transformer
     droplevel: list
+
+    Examples
+    --------
+    ::
+
+        import oemof.solph as solph
+        from oemof.solph import views
+
+        # solve oemof solph model 'm'
+        # Then collect node weights
+        views.node_output_by_type(
+            m.results(),
+            node_type=solph.components.Transformer
+        )
     """
     if droplevel is None:
         droplevel = []
     group = {
         k: v["sequences"]
         for k, v in results.items()
         if isinstance(k[0], node_type) and k[1] is not None
@@ -315,15 +364,29 @@
     node_type: oemof.solph class
         Specifies the type for which (storage) type net flows are calculated,
         e.g. solph.components.GenericStorage
 
     Returns
     -------
     pandas.DataFrame object with multiindex colums. Names of levels of columns
-    are: from, to, net_flow.
+        are: from, to, net_flow.
+
+    Examples
+    --------
+    ::
+
+        import oemof.solph as solph
+        from oemof.solph import views
+
+        # solve oemof solph model 'm'
+        # Then collect node weights
+        views.net_storage_flow(
+            m.results(),
+            node_type=solph.components.GenericStorage
+        )
     """
 
     group = {
         k: v["sequences"]
         for k, v in results.items()
         if isinstance(k[0], node_type) or isinstance(k[1], node_type)
     }
```

### Comparing `oemof.solph-0.5.1.dev0/src/oemof.solph.egg-info/PKG-INFO` & `oemof.solph-0.5.1.dev1/src/oemof.solph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oemof.solph
-Version: 0.5.1.dev0
+Version: 0.5.1.dev1
 Summary: A model generator for energy system modelling and optimisation.
 Home-page: https://oemof.org
 Author: oemof developer group
 Author-email: contact@oemof.org
 License: MIT
 Project-URL: Documentation, https://oemof-solph.readthedocs.io/
 Project-URL: Changelog, https://oemof-solph.readthedocs.io/en/latest/changelog.html
@@ -297,15 +297,15 @@
 The repository has sections for each major release.
 
 You are welcome to contribute your own examples via a `pull request <https://github.com/oemof/oemof-examples/pulls>`_ or by sending us an e-mail (see `here <https://oemof.org/contact/>`_ for contact information).
 
 License
 =======
 
-Copyright (c) 2022 oemof developer group
+Copyright (c) 2023 oemof developer group
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `oemof.solph-0.5.1.dev0/tests/constraint_tests.py` & `oemof.solph-0.5.1.dev1/tests/constraint_tests.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 available from its original location oemof/tests/constraint_tests.py
 
 SPDX-License-Identifier: MIT
 """
 
 import logging
 import re
-from difflib import unified_diff
 from os import path as ospath
 
 import pandas as pd
 import pytest
+from pyomo.repn.tests.lp_diff import lp_diff
 
 from oemof import solph
 
 logging.disable(logging.INFO)
 
 
 class TestsConstraint:
@@ -65,78 +65,37 @@
             with open(
                 ospath.join(
                     ospath.dirname(ospath.realpath(__file__)),
                     "lp_files",
                     filename,
                 )
             ) as expected_file:
+                exp = expected_file.read()
+                gen = generated_file.read()
 
-                def chop_trailing_whitespace(lines):
-                    return [re.sub(r"\s*$", "", ln) for ln in lines]
-
-                def remove(pattern, lines):
-                    if not pattern:
-                        return lines
-                    return re.subn(pattern, "", "\n".join(lines))[0].split(
-                        "\n"
-                    )
-
-                expected = remove(
-                    ignored,
-                    chop_trailing_whitespace(expected_file.readlines()),
-                )
-                generated = remove(
-                    ignored,
-                    chop_trailing_whitespace(generated_file.readlines()),
-                )
-
-                def normalize_to_positive_results(lines):
-                    negative_result_indices = [
-                        n
-                        for n, line in enumerate(lines)
-                        if re.match("^= -", line)
-                    ]
-                    equation_start_indices = [
-                        [
-                            n
-                            for n in reversed(range(0, nri))
-                            if re.match(".*:$", lines[n])
-                        ][0]
-                        + 1
-                        for nri in negative_result_indices
-                    ]
-                    for start, end in zip(
-                        equation_start_indices, negative_result_indices
-                    ):
-                        for n in range(start, end):
-                            lines[n] = (
-                                "-"
-                                if lines[n] and lines[n][0] == "+"
-                                else "+"
-                                if lines[n]
-                                else lines[n]
-                            ) + lines[n][1:]
-                        lines[end] = "= " + lines[end][3:]
-                    return lines
-
-                expected = normalize_to_positive_results(expected)
-                generated = normalize_to_positive_results(generated)
-
-                assert generated == expected, (
-                    "Failed matching expected with generated lp file:\n"
-                    + "\n".join(
-                        unified_diff(
-                            expected,
-                            generated,
-                            fromfile=ospath.relpath(expected_file.name),
-                            tofile=ospath.basename(generated_file.name),
-                            lineterm="",
-                        )
-                    ),
-                )
+                # lp_diff returns two arrays of strings with cleaned lp syntax
+                # It automatically prints the diff
+                exp_diff, gen_diff = lp_diff(exp, gen)
+
+                # sometimes, 0.0 is printed, sometimes 0, harmonise that
+                exp_diff = [
+                    line + " ".replace(" 0.0 ", " 0 ") for line in exp_diff
+                ]
+                gen_diff = [
+                    line + " ".replace(" 0.0 ", " 0 ") for line in gen_diff
+                ]
+
+                assert len(exp_diff) == len(gen_diff)
+
+                # Created the LP files do not have a reproducible
+                # order of the lines. Thus, we sort the lines.
+                for exp, gen in zip(sorted(exp_diff), sorted(gen_diff)):
+                    assert (
+                        exp == gen
+                    ), "Failed matching expected with generated lp file."
 
     def test_linear_transformer(self):
         """Constraint test of a Transformer without Investment."""
         bgas = solph.buses.Bus(label="gas")
 
         bel = solph.buses.Bus(label="electricity")
 
@@ -145,15 +104,14 @@
             inputs={bgas: solph.flows.Flow()},
             outputs={
                 bel: solph.flows.Flow(nominal_value=10e10, variable_costs=50)
             },
             conversion_factors={bel: 0.58},
         )
         self.energysystem.add(bgas, bel, transformer)
-
         self.compare_lp_files("linear_transformer.lp")
 
     def test_linear_transformer_invest(self):
         """Constraint test of a Transformer with Investment."""
 
         bgas = solph.buses.Bus(label="gas")
 
@@ -167,15 +125,14 @@
                     variable_costs=50,
                     investment=solph.Investment(maximum=1000, ep_costs=20),
                 )
             },
             conversion_factors={bel: 0.58},
         )
         self.energysystem.add(bgas, bel, transformer)
-
         self.compare_lp_files("linear_transformer_invest.lp")
 
     def test_nonconvex_invest_transformer(self):
         """Non-convex invest flow with offset, without minimum."""
         bfuel = solph.buses.Bus(label="fuelBus")
         bel = solph.buses.Bus(label="electricityBus")
 
@@ -216,37 +173,35 @@
             inputs={
                 bel: solph.flows.Flow(
                     nominal_value=54, min=(0.84, 0.94, 0.59), variable_costs=14
                 )
             },
         )
         self.energysystem.add(bel, wind, demand)
-
         self.compare_lp_files("max_source_min_sink.lp")
 
     def test_fixed_source_variable_sink(self):
         """Constraint test with a fixed source and a variable sink."""
 
         bel = solph.buses.Bus(label="electricityBus")
 
         wind = solph.components.Source(
             label="wind",
             outputs={
                 bel: solph.flows.Flow(
-                    fix=[0.43, 0.72, 0.29], nominal_value=10e5
+                    fix=[0.43, 0.72, 0.29], nominal_value=1e6
                 )
             },
         )
 
         excess = solph.components.Sink(
             label="excess", inputs={bel: solph.flows.Flow(variable_costs=40)}
         )
 
         self.energysystem.add(bel, wind, excess)
-
         self.compare_lp_files("fixed_source_variable_sink.lp")
 
     def test_nominal_value_to_zero(self):
         """If the nominal value is set to zero nothing should happen."""
         bel = solph.buses.Bus(label="electricityBus")
 
         s1 = solph.components.Source(
@@ -262,33 +217,32 @@
         """
 
         bel = solph.buses.Bus(label="electricityBus")
 
         wind = solph.components.Source(
             label="wind",
             outputs={
-                bel: solph.flows.Flow(fix=[12, 16, 14], nominal_value=1000000)
+                bel: solph.flows.Flow(fix=[12, 16, 14], nominal_value=1e6)
             },
         )
 
         excess = solph.components.Sink(
             label="excess",
             inputs={
                 bel: solph.flows.Flow(
                     full_load_time_max=2.3,
                     variable_costs=25,
                     max=0.8,
                     investment=solph.Investment(
-                        ep_costs=500, maximum=10e5, existing=50
+                        ep_costs=500, maximum=1e6, existing=50
                     ),
                 )
             },
         )
         self.energysystem.add(bel, wind, excess)
-
         self.compare_lp_files("fixed_source_invest_sink.lp")
 
     def test_invest_source_fixed_sink(self):
         """Constraint test with a fixed sink and a dispatch invest source."""
 
         bel = solph.buses.Bus(label="electricityBus")
 
@@ -302,41 +256,39 @@
                 )
             },
         )
 
         excess = solph.components.Sink(
             label="excess",
             inputs={
-                bel: solph.flows.Flow(fix=[0.5, 0.8, 0.3], nominal_value=10e4)
+                bel: solph.flows.Flow(fix=[0.5, 0.8, 0.3], nominal_value=1e5)
             },
         )
         self.energysystem.add(bel, pv, excess)
-
         self.compare_lp_files("invest_source_fixed_sink.lp")
 
     def test_storage(self):
         """ """
         bel = solph.buses.Bus(label="electricityBus")
 
         storage = solph.components.GenericStorage(
             label="storage_no_invest",
             inputs={
                 bel: solph.flows.Flow(nominal_value=16667, variable_costs=56)
             },
             outputs={
                 bel: solph.flows.Flow(nominal_value=16667, variable_costs=24)
             },
-            nominal_storage_capacity=10e4,
+            nominal_storage_capacity=1e5,
             loss_rate=0.13,
             inflow_conversion_factor=0.97,
             outflow_conversion_factor=0.86,
             initial_storage_level=0.4,
         )
         self.energysystem.add(bel, storage)
-
         self.compare_lp_files("storage.lp")
 
     def test_storage_invest_1(self):
         """All invest variables are coupled. The invest variables of the Flows
         will be created during the initialisation of the storage e.g. battery
         """
         bel = solph.buses.Bus(label="electricityBus")
@@ -352,15 +304,14 @@
             invest_relation_input_capacity=1 / 6,
             invest_relation_output_capacity=1 / 6,
             inflow_conversion_factor=0.97,
             outflow_conversion_factor=0.86,
             investment=solph.Investment(ep_costs=145, maximum=234),
         )
         self.energysystem.add(bel, storage)
-
         self.compare_lp_files("storage_invest_1.lp")
 
     def test_storage_invest_2(self):
         """All can be free extended to their own cost."""
         bel = solph.buses.Bus(label="electricityBus")
 
         storage = solph.components.GenericStorage(
@@ -471,15 +422,14 @@
             inputs={bel: solph.flows.Flow()},
             outputs={bel: solph.flows.Flow()},
             investment=solph.Investment(
                 ep_costs=145, minimum=100, maximum=200
             ),
         )
         self.energysystem.add(bel, storage)
-
         self.compare_lp_files("storage_invest_minimum.lp")
 
     def test_storage_unbalanced(self):
         """Testing a unbalanced storage (e.g. battery)."""
         bel = solph.buses.Bus(label="electricityBus")
 
         storage = solph.components.GenericStorage(
@@ -530,15 +480,14 @@
             fixed_losses_relative=0.01,
             fixed_losses_absolute=3,
             inflow_conversion_factor=0.97,
             outflow_conversion_factor=0.86,
             initial_storage_level=0.4,
         )
         self.energysystem.add(bel, storage)
-
         self.compare_lp_files("storage_fixed_losses.lp")
 
     def test_storage_invest_1_fixed_losses(self):
         """All invest variables are coupled. The invest variables of the Flows
         will be created during the initialisation of the storage e.g. battery
         """
         bel = solph.buses.Bus(label="electricityBus")
@@ -556,36 +505,34 @@
             invest_relation_input_capacity=1 / 6,
             invest_relation_output_capacity=1 / 6,
             inflow_conversion_factor=0.97,
             outflow_conversion_factor=0.86,
             investment=solph.Investment(ep_costs=145, maximum=234),
         )
         self.energysystem.add(bel, storage)
-
         self.compare_lp_files("storage_invest_1_fixed_losses.lp")
 
     def test_transformer(self):
         """Constraint test of a LinearN1Transformer without Investment."""
         bgas = solph.buses.Bus(label="gasBus")
         bbms = solph.buses.Bus(label="biomassBus")
         bel = solph.buses.Bus(label="electricityBus")
         bth = solph.buses.Bus(label="thermalBus")
 
         transformer = solph.components.Transformer(
-            label="powerplantGasCoal",
+            label="powerplantGasBiomass",
             inputs={bbms: solph.flows.Flow(), bgas: solph.flows.Flow()},
             outputs={
                 bel: solph.flows.Flow(variable_costs=50),
                 bth: solph.flows.Flow(nominal_value=5e10, variable_costs=20),
             },
             conversion_factors={bgas: 0.4, bbms: 0.1, bel: 0.3, bth: 0.5},
         )
 
         self.energysystem.add(bgas, bbms, bel, bth, transformer)
-
         self.compare_lp_files("transformer.lp")
 
     def test_transformer_invest(self):
         """Constraint test of a LinearN1Transformer with Investment."""
 
         bgas = solph.buses.Bus(label="gasBus")
         bcoal = solph.buses.Bus(label="coalBus")
@@ -601,15 +548,14 @@
                     investment=solph.Investment(maximum=1000, ep_costs=20),
                 ),
                 bth: solph.flows.Flow(variable_costs=20),
             },
             conversion_factors={bgas: 0.58, bcoal: 0.2, bel: 0.3, bth: 0.5},
         )
         self.energysystem.add(bgas, bcoal, bel, bth, transformer)
-
         self.compare_lp_files("transformer_invest.lp")
 
     def test_transformer_invest_with_existing(self):
         """Constraint test of a LinearN1Transformer with Investment."""
 
         bgas = solph.buses.Bus(label="gasBus")
         bcoal = solph.buses.Bus(label="coalBus")
@@ -627,35 +573,33 @@
                     ),
                 ),
                 bth: solph.flows.Flow(variable_costs=20),
             },
             conversion_factors={bgas: 0.58, bcoal: 0.2, bel: 0.3, bth: 0.5},
         )
         self.energysystem.add(bgas, bcoal, bel, bth, transformer)
-
         self.compare_lp_files("transformer_invest_with_existing.lp")
 
     def test_linear_transformer_chp(self):
         """
         Constraint test of a Transformer without Investment (two outputs).
         """
         bgas = solph.buses.Bus(label="gasBus")
         bheat = solph.buses.Bus(label="heatBus")
         bel = solph.buses.Bus(label="electricityBus")
 
         transformer = solph.components.Transformer(
             label="CHPpowerplantGas",
             inputs={
-                bgas: solph.flows.Flow(nominal_value=10e10, variable_costs=50)
+                bgas: solph.flows.Flow(nominal_value=1e11, variable_costs=50)
             },
             outputs={bel: solph.flows.Flow(), bheat: solph.flows.Flow()},
             conversion_factors={bel: 0.4, bheat: 0.5},
         )
         self.energysystem.add(bgas, bheat, bel, transformer)
-
         self.compare_lp_files("linear_transformer_chp.lp")
 
     def test_linear_transformer_chp_invest(self):
         """Constraint test of a Transformer with Investment (two outputs)."""
 
         bgas = solph.buses.Bus(label="gasBus")
         bheat = solph.buses.Bus(label="heatBus")
@@ -669,15 +613,14 @@
                     investment=solph.Investment(maximum=1000, ep_costs=20),
                 )
             },
             outputs={bel: solph.flows.Flow(), bheat: solph.flows.Flow()},
             conversion_factors={bel: 0.4, bheat: 0.5},
         )
         self.energysystem.add(bgas, bheat, bel, transformer)
-
         self.compare_lp_files("linear_transformer_chp_invest.lp")
 
     def test_link(self):
         bel0 = solph.buses.Bus(label="bel0")
         bel1 = solph.buses.Bus(label="bel1")
 
         link = solph.components.experimental.Link(
@@ -686,19 +629,18 @@
                 bel0: solph.Flow(nominal_value=4),
                 bel1: solph.Flow(nominal_value=2),
             },
             outputs={bel0: solph.Flow(), bel1: solph.Flow()},
             conversion_factors={(bel0, bel1): 0.8, (bel1, bel0): 0.9},
         )
         self.energysystem.add(bel0, bel1, link)
-
         self.compare_lp_files("link.lp")
 
     def test_variable_chp(self):
-        """ """
+        """Test ExctractionTurbineCHP basic functionality"""
         bel = solph.buses.Bus(label="electricityBus")
         bth = solph.buses.Bus(label="heatBus")
         bgas = solph.buses.Bus(label="commodityBus")
 
         chp1 = solph.components.ExtractionTurbineCHP(
             label="variable_chp_gas1",
             inputs={bgas: solph.flows.Flow(nominal_value=100)},
@@ -711,19 +653,18 @@
             label="variable_chp_gas2",
             inputs={bgas: solph.flows.Flow(nominal_value=100)},
             outputs={bel: solph.flows.Flow(), bth: solph.flows.Flow()},
             conversion_factors={bel: 0.3, bth: 0.5},
             conversion_factor_full_condensation={bel: 0.5},
         )
         self.energysystem.add(bel, bth, bgas, chp1, chp2)
-
         self.compare_lp_files("variable_chp.lp")
 
     def test_generic_invest_limit(self):
-        """ """
+        """Test a generic keyword investment limit"""
         bus = solph.buses.Bus(label="bus_1")
 
         source_0 = solph.components.Source(
             label="source_0",
             outputs={
                 bus: solph.flows.Flow(
                     investment=solph.Investment(
@@ -759,15 +700,15 @@
         om = solph.constraints.additional_investment_flow_limit(
             om, "space", limit=20
         )
 
         self.compare_lp_files("generic_invest_limit.lp", my_om=om)
 
     def test_emission_constraints(self):
-        """ """
+        """Test emissions constraint"""
         bel = solph.buses.Bus(label="electricityBus")
 
         source1 = solph.components.Source(
             label="source1",
             outputs={
                 bel: solph.flows.Flow(
                     nominal_value=100,
@@ -795,15 +736,15 @@
         om = self.get_om()
 
         solph.constraints.emission_limit(om, limit=777)
 
         self.compare_lp_files("emission_limit.lp", my_om=om)
 
     def test_flow_count_limit(self):
-        """ """
+        """Test limiting the count of nonconvex flows"""
         bel = solph.buses.Bus(label="electricityBus")
 
         source1 = solph.components.Source(
             label="source1",
             outputs={
                 bel: solph.flows.Flow(
                     nonconvex=solph.NonConvex(),
@@ -853,15 +794,15 @@
         solph.constraints.limit_active_flow_count_by_keyword(
             om, "emission_factor", lower_limit=1, upper_limit=2
         )
 
         self.compare_lp_files("flow_count_limit.lp", my_om=om)
 
     def test_shared_limit(self):
-        """ """
+        """Test an overall limit shared among components"""
         b1 = solph.buses.Bus(label="bus")
 
         storage1 = solph.components.GenericStorage(
             label="storage1",
             nominal_storage_capacity=5,
             inputs={b1: solph.flows.Flow()},
             outputs={b1: solph.flows.Flow()},
@@ -887,15 +828,15 @@
             [0.5, 1.25],
             upper_limit=7,
         )
 
         self.compare_lp_files("shared_limit.lp", my_om=model)
 
     def test_flow_without_emission_for_emission_constraint(self):
-        """ """
+        """Test AttributeError if passed flow misses emission attribute"""
         with pytest.raises(AttributeError):
             bel = solph.buses.Bus(label="electricityBus")
             source1 = solph.components.Source(
                 label="source1",
                 outputs={
                     bel: solph.flows.Flow(
                         nominal_value=100,
@@ -908,15 +849,15 @@
                 outputs={bel: solph.flows.Flow(nominal_value=100)},
             )
             self.energysystem.add(bel, source1, source2)
             om = self.get_om()
             solph.constraints.emission_limit(om, om.flows, limit=777)
 
     def test_flow_without_emission_for_emission_constraint_no_error(self):
-        """ """
+        """Test that no error is thrown if no flows are explicitly passed"""
         bel = solph.buses.Bus(label="electricityBus")
         source1 = solph.components.Source(
             label="source1",
             outputs={
                 bel: solph.flows.Flow(
                     nominal_value=100,
                     custom_attributes={"emission_factor": 0.8},
@@ -926,19 +867,21 @@
         source2 = solph.components.Source(
             label="source2", outputs={bel: solph.flows.Flow(nominal_value=100)}
         )
         self.energysystem.add(bel, source1, source2)
         om = self.get_om()
         solph.constraints.emission_limit(om, limit=777)
 
+        self.compare_lp_files("emission_limit_no_error.lp", my_om=om)
+
     def test_equate_variables_constraint(self):
         """Testing the equate_variables function in the constraint module."""
         bus1 = solph.buses.Bus(label="Bus1")
         storage = solph.components.GenericStorage(
-            label="storage_constraint",
+            label="storage",
             invest_relation_input_capacity=0.2,
             invest_relation_output_capacity=0.2,
             inputs={bus1: solph.flows.Flow()},
             outputs={bus1: solph.flows.Flow()},
             investment=solph.Investment(ep_costs=145),
         )
         sink = solph.components.Sink(
@@ -957,22 +900,22 @@
                 )
             },
         )
         self.energysystem.add(bus1, storage, sink, source)
         om = self.get_om()
         solph.constraints.equate_variables(
             om,
-            om.InvestmentFlowBlock.invest[source, bus1],
-            om.InvestmentFlowBlock.invest[bus1, sink],
+            om.InvestmentFlowBlock.invest[source, bus1, 0],
+            om.InvestmentFlowBlock.invest[bus1, sink, 0],
             2,
         )
         solph.constraints.equate_variables(
             om,
-            om.InvestmentFlowBlock.invest[source, bus1],
-            om.GenericInvestmentStorageBlock.invest[storage],
+            om.InvestmentFlowBlock.invest[source, bus1, 0],
+            om.GenericInvestmentStorageBlock.invest[storage, 0],
         )
 
         self.compare_lp_files("connect_investment.lp", my_om=om)
 
     def test_equate_flows_constraint(self):
         """Testing the equate_flows function in the constraint module."""
         bus1 = solph.buses.Bus(label="Bus1")
@@ -1013,34 +956,33 @@
             "incoming_flow",
             "outgoing_flow",
             2,
         )
         self.compare_lp_files("equate_flows.lp", my_om=om)
 
     def test_gradient(self):
-        """Testing gradient constraints and costs."""
+        """Testing gradient constraints"""
         bel = solph.buses.Bus(label="electricityBus")
 
         pp = solph.components.Source(
             label="powerplant",
             outputs={
                 bel: solph.flows.Flow(
                     nominal_value=999,
                     variable_costs=23,
                     positive_gradient_limit=0.03,
                     negative_gradient_limit=0.05,
                 )
             },
         )
         self.energysystem.add(bel, pp)
-
         self.compare_lp_files("source_with_gradient.lp")
 
     def test_nonconvex_gradient(self):
-        """Testing gradient constraints and costs."""
+        """Testing gradient constraints"""
         bel = solph.buses.Bus(label="electricityBus")
 
         pp = solph.components.Source(
             label="powerplant",
             outputs={
                 bel: solph.flows.Flow(
                     nominal_value=999,
@@ -1049,15 +991,14 @@
                         positive_gradient_limit=0.03,
                         negative_gradient_limit=0.05,
                     ),
                 )
             },
         )
         self.energysystem.add(bel, pp)
-
         self.compare_lp_files("source_with_nonconvex_gradient.lp")
 
     def test_nonconvex_positive_gradient_error(self):
         """Testing nonconvex positive gradient error."""
         msg = (
             "You specified a positive gradient in your nonconvex "
             "option. This cannot be combined with a positive or a "
@@ -1109,14 +1050,144 @@
         )
         self.energysystem.add(bus1, storage, source)
         om = self.get_om()
         solph.constraints.investment_limit(om, limit=900)
 
         self.compare_lp_files("investment_limit.lp", my_om=om)
 
+    def test_investment_limit_with_dsm1(self):
+        """Testing the investment_limit function in the constraint module."""
+        bus1 = solph.buses.Bus(label="Bus1")
+        source = solph.components.Source(
+            label="Source",
+            outputs={
+                bus1: solph.flows.Flow(
+                    investment=solph.Investment(ep_costs=123)
+                )
+            },
+        )
+        dsm = solph.components.experimental.SinkDSM(
+            label="sink_dsm_DIW",
+            approach="DIW",
+            inputs={bus1: solph.flows.Flow()},
+            demand=[1] * 3,
+            capacity_up=[0.5] * 3,
+            capacity_down=[0.5] * 3,
+            max_demand=[1] * 3,
+            delay_time=1,
+            cost_dsm_down_shift=0.5,
+            cost_dsm_up=0.5,
+            shed_eligibility=False,
+            investment=solph.Investment(
+                ep_costs=100, existing=50, minimum=33, maximum=100
+            ),
+        )
+        self.energysystem.add(bus1, source, dsm)
+        om = self.get_om()
+        solph.constraints.investment_limit(om, limit=900)
+
+        self.compare_lp_files("investment_limit_with_dsm_DIW.lp", my_om=om)
+
+    def test_investment_limit_with_dsm2(self):
+        """Testing the investment_limit function in the constraint module."""
+        bus1 = solph.buses.Bus(label="Bus1")
+        source = solph.components.Source(
+            label="Source",
+            outputs={
+                bus1: solph.flows.Flow(
+                    investment=solph.Investment(ep_costs=123)
+                )
+            },
+        )
+        dsm = solph.components.experimental.SinkDSM(
+            label="sink_dsm_DLR",
+            approach="DLR",
+            inputs={bus1: solph.flows.Flow()},
+            demand=[1] * 3,
+            capacity_up=[0.5] * 3,
+            capacity_down=[0.5] * 3,
+            max_demand=[1] * 3,
+            delay_time=1,
+            shift_time=1,
+            cost_dsm_down_shift=0.5,
+            cost_dsm_up=0.5,
+            shed_eligibility=False,
+            investment=solph.Investment(
+                ep_costs=100, existing=50, minimum=33, maximum=100
+            ),
+        )
+        self.energysystem.add(bus1, source, dsm)
+        om = self.get_om()
+        solph.constraints.investment_limit(om, limit=900)
+
+        self.compare_lp_files("investment_limit_with_dsm_DLR.lp", my_om=om)
+
+    def test_investment_limit_with_dsm3(self):
+        """Testing the investment_limit function in the constraint module."""
+        bus1 = solph.buses.Bus(label="Bus1")
+        source = solph.components.Source(
+            label="Source",
+            outputs={
+                bus1: solph.flows.Flow(
+                    investment=solph.Investment(ep_costs=123)
+                )
+            },
+        )
+        dsm = solph.components.experimental.SinkDSM(
+            label="sink_dsm_oemof",
+            approach="oemof",
+            inputs={bus1: solph.flows.Flow()},
+            demand=[1] * 3,
+            capacity_up=[0.5] * 3,
+            capacity_down=[0.5] * 3,
+            max_demand=[1] * 3,
+            delay_time=1,
+            shift_interval=2,
+            cost_dsm_down_shift=0.5,
+            cost_dsm_up=0.5,
+            shed_eligibility=False,
+            investment=solph.Investment(
+                ep_costs=100, existing=50, minimum=33, maximum=100
+            ),
+        )
+        self.energysystem.add(bus1, source, dsm)
+        om = self.get_om()
+        solph.constraints.investment_limit(om, limit=900)
+
+        self.compare_lp_files("investment_limit_with_dsm_oemof.lp", my_om=om)
+
+    def test_investment_limit_per_period_error_no_multi_period(self):
+        """Test error being thrown if model is not a multi-period model"""
+        bus1 = solph.buses.Bus(label="Bus1")
+        solph.components.GenericStorage(
+            label="storage_invest_limit",
+            invest_relation_input_capacity=0.2,
+            invest_relation_output_capacity=0.2,
+            inputs={bus1: solph.flows.Flow()},
+            outputs={bus1: solph.flows.Flow()},
+            investment=solph.Investment(ep_costs=145),
+        )
+        solph.components.Source(
+            label="Source",
+            outputs={
+                bus1: solph.flows.Flow(
+                    investment=solph.Investment(ep_costs=123)
+                )
+            },
+        )
+        om = self.get_om()
+
+        msg = (
+            "investment_limit_per_period is only applicable "
+            "for multi-period models.\nIn order to create such a model, "
+            "explicitly set attribute `periods` of your energy system."
+        )
+        with pytest.raises(ValueError, match=msg):
+            solph.constraints.investment_limit_per_period(om, limit=900)
+
     def test_min_max_runtime(self):
         """Testing min and max runtimes for nonconvex flows."""
         bus_t = solph.buses.Bus(label="Bus_T")
         pp = solph.components.Source(
             label="cheap_plant_min_down_constraints",
             outputs={
                 bus_t: solph.flows.Flow(
@@ -1176,43 +1247,43 @@
         self.energysystem.add(bus_t, pp)
         self.compare_lp_files("inactivity_costs.lp")
 
     def test_piecewise_linear_transformer_cc(self):
         """Testing PiecewiseLinearTransformer using CC formulation."""
         bgas = solph.buses.Bus(label="gasBus")
         bel = solph.buses.Bus(label="electricityBus")
-        plt = solph.components.experimental.PiecewiseLinearTransformer(
+        pwltf = solph.components.experimental.PiecewiseLinearTransformer(
             label="pwltf",
             inputs={
                 bgas: solph.flows.Flow(nominal_value=100, variable_costs=1)
             },
             outputs={bel: solph.flows.Flow()},
             in_breakpoints=[0, 25, 50, 75, 100],
             conversion_function=lambda x: x**2,
             pw_repn="CC",
         )
 
-        self.energysystem.add(bgas, bel, plt)
+        self.energysystem.add(bgas, bel, pwltf)
         self.compare_lp_files("piecewise_linear_transformer_cc.lp")
 
     def test_piecewise_linear_transformer_dcc(self):
         """Testing PiecewiseLinearTransformer using DCC formulation."""
         bgas = solph.buses.Bus(label="gasBus")
         bel = solph.buses.Bus(label="electricityBus")
-        plt = solph.components.experimental.PiecewiseLinearTransformer(
+        pwltf = solph.components.experimental.PiecewiseLinearTransformer(
             label="pwltf",
             inputs={
                 bgas: solph.flows.Flow(nominal_value=100, variable_costs=1)
             },
             outputs={bel: solph.flows.Flow()},
             in_breakpoints=[0, 25, 50, 75, 100],
             conversion_function=lambda x: x**2,
             pw_repn="DCC",
         )
-        self.energysystem.add(bgas, bel, plt)
+        self.energysystem.add(bgas, bel, pwltf)
         self.compare_lp_files("piecewise_linear_transformer_dcc.lp")
 
     def test_maximum_startups(self):
         """Testing maximum_startups attribute for nonconvex flows."""
         bus_t = solph.buses.Bus(label="Bus_C")
         pp = solph.components.Source(
             label="cheap_plant_maximum_startups",
@@ -1261,165 +1332,285 @@
                     min=0.32,
                 )
             },
             outputs={bth: solph.flows.Flow()},
             coefficients=[-17, 0.9],
         )
         self.energysystem.add(bgas, bth, transformer)
-
         self.compare_lp_files("offsettransformer.lp")
 
     def test_dsm_module_DIW(self):
         """Constraint test of SinkDSM with approach=DLR"""
 
         b_elec = solph.buses.Bus(label="bus_elec")
-        sink = solph.components.experimental.SinkDSM(
+        sinkdsm = solph.components.experimental.SinkDSM(
             label="demand_dsm",
             inputs={b_elec: solph.flows.Flow()},
             demand=[1] * 3,
             capacity_up=[0.5] * 3,
             capacity_down=[0.5] * 3,
             approach="DIW",
             max_demand=1,
             max_capacity_up=1,
             max_capacity_down=1,
             delay_time=1,
             cost_dsm_down_shift=2,
             shed_eligibility=False,
         )
 
-        self.energysystem.add(b_elec, sink)
+        self.energysystem.add(b_elec, sinkdsm)
         self.compare_lp_files("dsm_module_DIW.lp")
 
     def test_dsm_module_DLR(self):
         """Constraint test of SinkDSM with approach=DLR"""
 
         b_elec = solph.buses.Bus(label="bus_elec")
-        sink = solph.components.experimental.SinkDSM(
+        sinkdsm = solph.components.experimental.SinkDSM(
             label="demand_dsm",
             inputs={b_elec: solph.flows.Flow()},
             demand=[1] * 3,
             capacity_up=[0.5] * 3,
             capacity_down=[0.5] * 3,
             approach="DLR",
             max_demand=1,
             max_capacity_up=1,
             max_capacity_down=1,
             delay_time=2,
             shift_time=1,
             cost_dsm_down_shift=2,
             shed_eligibility=False,
         )
-        self.energysystem.add(b_elec, sink)
+        self.energysystem.add(b_elec, sinkdsm)
         self.compare_lp_files("dsm_module_DLR.lp")
 
     def test_dsm_module_oemof(self):
         """Constraint test of SinkDSM with approach=oemof"""
 
         b_elec = solph.buses.Bus(label="bus_elec")
-        sink = solph.components.experimental.SinkDSM(
+        sinkdsm = solph.components.experimental.SinkDSM(
             label="demand_dsm",
             inputs={b_elec: solph.flows.Flow()},
             demand=[1] * 3,
             capacity_up=[0.5, 0.4, 0.5],
             capacity_down=[0.5, 0.4, 0.5],
             approach="oemof",
             max_demand=1,
             max_capacity_up=1,
             max_capacity_down=1,
             shift_interval=2,
             cost_dsm_down_shift=2,
             shed_eligibility=False,
         )
-        self.energysystem.add(b_elec, sink)
+        self.energysystem.add(b_elec, sinkdsm)
         self.compare_lp_files("dsm_module_oemof.lp")
 
+    def test_dsm_module_DIW_extended(self):
+        """Constraint test of SinkDSM with approach=DLR
+
+        Test all possible parameters and constraints
+        """
+
+        b_elec = solph.buses.Bus(label="bus_elec")
+        sinkdsm = solph.components.experimental.SinkDSM(
+            label="demand_dsm",
+            inputs={b_elec: solph.flows.Flow()},
+            demand=[1, 0.9, 0.8],
+            capacity_up=[0.5, 0.4, 0.5],
+            capacity_down=[0.3, 0.3, 0.4],
+            approach="DIW",
+            max_demand=1,
+            max_capacity_up=1,
+            max_capacity_down=1,
+            delay_time=1,
+            cost_dsm_down_shift=1,
+            cost_dsm_up=1,
+            cost_dsm_down_shed=100,
+            efficiency=0.99,
+            recovery_time_shift=2,
+            recovery_time_shed=2,
+            shed_time=2,
+        )
+        self.energysystem.add(b_elec, sinkdsm)
+        self.compare_lp_files("dsm_module_DIW_extended.lp")
+
+    def test_dsm_module_DLR_extended(self):
+        """Constraint test of SinkDSM with approach=DLR"""
+
+        b_elec = solph.buses.Bus(label="bus_elec")
+        sinkdsm = solph.components.experimental.SinkDSM(
+            label="demand_dsm",
+            inputs={b_elec: solph.flows.Flow()},
+            demand=[1, 0.9, 0.8],
+            capacity_up=[0.5, 0.4, 0.5],
+            capacity_down=[0.3, 0.3, 0.4],
+            approach="DLR",
+            max_demand=1,
+            max_capacity_up=1,
+            max_capacity_down=1,
+            delay_time=2,
+            shift_time=1,
+            cost_dsm_down_shift=1,
+            cost_dsm_up=1,
+            cost_dsm_down_shed=100,
+            efficiency=0.99,
+            recovery_time_shed=2,
+            ActivateYearLimit=True,
+            ActivateDayLimit=True,
+            n_yearLimit_shift=100,
+            n_yearLimit_shed=50,
+            t_dayLimit=3,
+            addition=False,
+            fixes=False,
+            shed_time=2,
+        )
+        self.energysystem.add(b_elec, sinkdsm)
+        self.compare_lp_files("dsm_module_DLR_extended.lp")
+
+    def test_dsm_module_oemof_extended(self):
+        """Constraint test of SinkDSM with approach=oemof"""
+
+        b_elec = solph.buses.Bus(label="bus_elec")
+        sinkdsm = solph.components.experimental.SinkDSM(
+            label="demand_dsm",
+            inputs={b_elec: solph.flows.Flow()},
+            demand=[1, 0.9, 0.8],
+            capacity_up=[0.5, 0.4, 0.5],
+            capacity_down=[0.3, 0.3, 0.4],
+            approach="oemof",
+            shift_interval=2,
+            max_demand=1,
+            max_capacity_up=1,
+            max_capacity_down=1,
+            delay_time=2,
+            cost_dsm_down_shift=1,
+            cost_dsm_up=1,
+            cost_dsm_down_shed=100,
+            efficiency=0.99,
+            recovery_time_shed=2,
+            shed_time=2,
+        )
+        self.energysystem.add(b_elec, sinkdsm)
+        self.compare_lp_files("dsm_module_oemof_extended.lp")
+
     def test_dsm_module_DIW_invest(self):
         """Constraint test of SinkDSM with approach=DLR and investments"""
 
         b_elec = solph.buses.Bus(label="bus_elec")
-        sink = solph.components.experimental.SinkDSM(
+        sinkdsm = solph.components.experimental.SinkDSM(
             label="demand_dsm",
             inputs={b_elec: solph.flows.Flow()},
             demand=[1] * 3,
             capacity_up=[0.5] * 3,
             capacity_down=[0.5] * 3,
             approach="DIW",
-            flex_share_up=1,
-            flex_share_down=1,
+            max_demand=1,
             delay_time=1,
-            cost_dsm_down_shift=2,
-            shed_eligibility=False,
+            cost_dsm_down_shift=1,
+            cost_dsm_up=1,
+            cost_dsm_down_shed=100,
+            shed_eligibility=True,
+            recovery_time_shed=2,
+            shed_time=2,
             investment=solph.Investment(
                 existing=50,
                 minimum=33,
                 maximum=100,
                 custom_attributes={"ep_cost": 100},
             ),
         )
-        self.energysystem.add(b_elec, sink)
+        self.energysystem.add(b_elec, sinkdsm)
         self.compare_lp_files("dsm_module_DIW_invest.lp")
 
     def test_dsm_module_DLR_invest(self):
         """Constraint test of SinkDSM with approach=DLR and investments"""
 
         b_elec = solph.buses.Bus(label="bus_elec")
-        sink = solph.components.experimental.SinkDSM(
+        sinkdsm = solph.components.experimental.SinkDSM(
             label="demand_dsm",
             inputs={b_elec: solph.flows.Flow()},
             demand=[1] * 3,
             capacity_up=[0.5] * 3,
             capacity_down=[0.5] * 3,
             approach="DLR",
-            flex_share_up=1,
-            flex_share_down=1,
+            max_demand=1,
             delay_time=2,
             shift_time=1,
-            cost_dsm_down_shift=2,
-            shed_eligibility=False,
+            cost_dsm_down_shift=1,
+            cost_dsm_up=1,
+            cost_dsm_down_shed=100,
+            shed_eligibility=True,
+            recovery_time_shed=2,
+            shed_time=2,
+            n_yearLimit_shed=50,
             investment=solph.Investment(
                 existing=50,
                 minimum=33,
                 maximum=100,
                 custom_attributes={"ep_cost": 100},
             ),
         )
-        self.energysystem.add(b_elec, sink)
+        self.energysystem.add(b_elec, sinkdsm)
         self.compare_lp_files("dsm_module_DLR_invest.lp")
 
     def test_dsm_module_oemof_invest(self):
         """Constraint test of SinkDSM with approach=oemof and investments"""
 
         b_elec = solph.buses.Bus(label="bus_elec")
-        sink = solph.components.experimental.SinkDSM(
+        sinkdsm = solph.components.experimental.SinkDSM(
             label="demand_dsm",
             inputs={b_elec: solph.flows.Flow()},
             demand=[1] * 3,
             capacity_up=[0.5, 0.4, 0.5],
             capacity_down=[0.5, 0.4, 0.5],
             approach="oemof",
-            flex_share_up=1,
-            flex_share_down=1,
+            max_demand=1,
             shift_interval=2,
-            cost_dsm_down_shift=2,
-            shed_eligibility=False,
+            cost_dsm_down_shift=1,
+            cost_dsm_up=1,
+            cost_dsm_down_shed=100,
+            shed_eligibility=True,
+            recovery_time_shed=2,
+            shed_time=2,
             investment=solph.Investment(
                 existing=50,
                 minimum=33,
                 maximum=100,
                 custom_attributes={"ep_cost": 100},
             ),
         )
-        self.energysystem.add(b_elec, sink)
+        self.energysystem.add(b_elec, sinkdsm)
         self.compare_lp_files("dsm_module_oemof_invest.lp")
 
+    def test_dsm_module_DLR_delay_time(self):
+        """Constraint test of SinkDSM with approach=DLR;
+        testing for passing an iterable for delay_time"""
+
+        b_elec = solph.buses.Bus(label="bus_elec")
+        sinkdsm = solph.components.experimental.SinkDSM(
+            label="demand_dsm",
+            inputs={b_elec: solph.flows.Flow()},
+            demand=[1] * 3,
+            capacity_up=[0.5] * 3,
+            capacity_down=[0.5] * 3,
+            approach="DLR",
+            max_demand=1,
+            max_capacity_up=1,
+            max_capacity_down=1,
+            delay_time=[1, 3],
+            shift_time=1,
+            cost_dsm_down_shift=2,
+            shed_eligibility=False,
+        )
+        self.energysystem.add(b_elec, sinkdsm)
+        self.compare_lp_files("dsm_module_DLR_delay_time.lp")
+
     def test_invest_non_convex_flow(self):
         """Invest into a non-convex Flow"""
         b1 = solph.buses.Bus(label="b1")
-        sink = solph.buses.Bus(
+        b2 = solph.buses.Bus(
             label="b2",
             inputs={
                 b1: solph.Flow(
                     nominal_value=None,
                     variable_costs=8,
                     min=0.25,
                     max=0.5,
@@ -1428,15 +1619,15 @@
                         maximum=10,
                     ),
                     nonconvex=solph.NonConvex(),
                 )
             },
             outputs={b1: solph.Flow()},
         )
-        self.energysystem.add(b1, sink)
+        self.energysystem.add(b1, b2)
         self.compare_lp_files("invest_non_convex_flow.lp")
 
     def test_nonconvex_investment_storage_without_offset(self):
         """All invest variables are coupled. The invest variables of the Flows
         will be created during the initialisation of the storage e.g. battery
         """
         bel = solph.buses.Bus(label="electricityBus")
@@ -1454,25 +1645,24 @@
             inflow_conversion_factor=0.97,
             outflow_conversion_factor=0.86,
             investment=solph.Investment(
                 ep_costs=141, maximum=244, minimum=12, nonconvex=True
             ),
         )
         self.energysystem.add(bel, storage)
-
         self.compare_lp_files("storage_invest_without_offset.lp")
 
     def test_nonconvex_investment_storage_with_offset(self):
         """All invest variables are coupled. The invest variables of the Flows
         will be created during the initialisation of the storage e.g. battery
         """
         bel = solph.buses.Bus(label="electricityBus")
 
         storage = solph.components.GenericStorage(
-            label="storagenon_convex",
+            label="storage_non_convex",
             inputs={bel: solph.flows.Flow(variable_costs=56)},
             outputs={bel: solph.flows.Flow(variable_costs=24)},
             nominal_storage_capacity=None,
             loss_rate=0.13,
             max_storage_level=0.9,
             min_storage_level=0.1,
             invest_relation_input_capacity=1 / 6,
@@ -1484,15 +1674,14 @@
                 minimum=19,
                 offset=5,
                 nonconvex=True,
                 maximum=1454,
             ),
         )
         self.energysystem.add(bel, storage)
-
         self.compare_lp_files("storage_invest_with_offset.lp")
 
     def test_nonconvex_invest_storage_all_nonconvex(self):
         """All invest variables are free and nonconvex."""
         b1 = solph.buses.Bus(label="bus1")
 
         storage = solph.components.GenericStorage(
@@ -1520,15 +1709,14 @@
                 )
             },
             investment=solph.Investment(
                 nonconvex=True, ep_costs=20, offset=30, minimum=20, maximum=100
             ),
         )
         self.energysystem.add(b1, storage)
-
         self.compare_lp_files("storage_invest_all_nonconvex.lp")
 
     def test_nonconvex_invest_sink_without_offset(self):
         """Non-convex invest flow without offset, with minimum."""
         bel = solph.buses.Bus(label="electricityBus")
 
         sink = solph.components.Sink(
@@ -1587,14 +1775,76 @@
                     ),
                 )
             },
         )
         self.energysystem.add(bel, source)
         self.compare_lp_files("flow_invest_with_offset_no_minimum.lp")
 
+    def test_integral_limit_error_no_multi_period(self):
+        """Test error being thrown if model is not a multi-period model"""
+        bel = solph.buses.Bus(label="electricityBus")
+
+        source = solph.components.Source(
+            label="pv_source",
+            outputs={
+                bel: solph.flows.Flow(
+                    nominal_value=100,
+                    variable_costs=20,
+                    fix=[0.3, 0.5, 0.8],
+                    custom_attributes={"space": 40},
+                )
+            },
+        )
+        self.energysystem.add(bel, source)
+        om = self.get_om()
+        msg = (
+            "generic_periodical_integral_limit is only applicable\n"
+            "for multi-period models.\nFor standard models, use "
+            "generic_integral_limit instead."
+        )
+        with pytest.raises(ValueError, match=msg):
+            solph.constraints.generic_periodical_integral_limit(
+                om, keyword="space"
+            )
+
+    def test_summed_min_max_source(self):
+        """Constraints test summed_min and summed_max attribute of flow"""
+
+        bel = solph.buses.Bus(label="electricityBus")
+
+        sink = solph.components.Sink(
+            label="excess",
+            inputs={
+                bel: solph.flows.Flow(
+                    summed_min=3,
+                    summed_max=100,
+                    variable_costs=25,
+                    max=0.8,
+                    nominal_value=10,
+                )
+            },
+        )
+        self.energysystem.add(bel, sink)
+        self.compare_lp_files("summed_min_source.lp")
+
+    def test_integer_flow_source(self):
+        """Test source with integer output"""
+        bel = solph.buses.Bus(label="electricityBus")
+
+        sink = solph.components.Sink(
+            label="excess",
+            inputs={
+                bel: solph.flows.Flow(
+                    variable_costs=25, max=1, nominal_value=10, integer=True
+                )
+            },
+        )
+        self.energysystem.add(bel, sink)
+        self.compare_lp_files("integer_source.lp")
+
     def test_nonequidistant_storage(self):
         """Constraint test of an energy system
         with non-equidistant time index
         """
         idxh = pd.date_range("1/1/2017", periods=3, freq="H")
         idx2h = pd.date_range("1/1/2017 03:00:00", periods=2, freq="2H")
         idx30m = pd.date_range("1/1/2017 07:00:00", periods=4, freq="30min")
@@ -1614,7 +1864,78 @@
             nominal_storage_capacity=300,
             loss_rate=0.1,
             initial_storage_level=1,
         )
         es.add(b_gas, b_th, boiler, storage)
         om = solph.Model(es)
         self.compare_lp_files("nonequidistant_timeindex.lp", my_om=om)
+
+    def test_storage_level_constraint(self):
+        """Constraint test of an energy system
+        with storage_level_constraint
+        """
+        es = solph.EnergySystem(
+            timeindex=pd.date_range("2022-01-01", freq="1H", periods=2),
+            infer_last_interval=True,
+        )
+
+        multiplexer = solph.Bus(
+            label="multiplexer",
+        )
+
+        storage = solph.components.GenericStorage(
+            label="storage",
+            nominal_storage_capacity=4,
+            initial_storage_level=1,
+            balanced=True,
+            loss_rate=0.25,
+            inputs={multiplexer: solph.Flow()},
+            outputs={multiplexer: solph.Flow()},
+        )
+
+        es.add(multiplexer, storage)
+
+        in_0 = solph.components.Source(
+            label="in_0",
+            outputs={
+                multiplexer: solph.Flow(nominal_value=0.5, variable_costs=0.25)
+            },
+        )
+        es.add(in_0)
+
+        in_1 = solph.components.Source(
+            label="in_1",
+            outputs={multiplexer: solph.Flow(nominal_value=0.125)},
+        )
+        es.add(in_1)
+
+        out_0 = solph.components.Sink(
+            label="out_0",
+            inputs={
+                multiplexer: solph.Flow(
+                    nominal_value=0.25, variable_costs=-0.125
+                )
+            },
+        )
+        es.add(out_0)
+
+        out_1 = solph.components.Sink(
+            label="out_1",
+            inputs={
+                multiplexer: solph.Flow(
+                    nominal_value=0.125, variable_costs=-0.125
+                )
+            },
+        )
+        es.add(out_1)
+
+        om = solph.Model(es)
+
+        solph.constraints.storage_level_constraint(
+            model=om,
+            name="multiplexer",
+            storage_component=storage,
+            multiplexer_bus=multiplexer,
+            input_levels={in_1: 1 / 4},  # in_0 is always active
+            output_levels={out_0: 1 / 8, out_1: 1 / 2},
+        )
+        self.compare_lp_files("storage_level_constraint.lp", my_om=om)
```

### Comparing `oemof.solph-0.5.1.dev0/tests/flow_tests.py` & `oemof.solph-0.5.1.dev1/tests/flow_tests.py`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/activity_costs.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/activity_costs.lp`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 \* Source Pyomo model name=Model *\
 
-min
+min 
 objective:
++10 flow(cheap_plant_activity_costs_Bus_C_0_0)
++10 flow(cheap_plant_activity_costs_Bus_C_0_1)
++10 flow(cheap_plant_activity_costs_Bus_C_0_2)
 +2 NonConvexFlowBlock_status(cheap_plant_activity_costs_Bus_C_0)
 +2 NonConvexFlowBlock_status(cheap_plant_activity_costs_Bus_C_1)
 +2 NonConvexFlowBlock_status(cheap_plant_activity_costs_Bus_C_2)
-+10 flow(cheap_plant_activity_costs_Bus_C_0)
-+10 flow(cheap_plant_activity_costs_Bus_C_1)
-+10 flow(cheap_plant_activity_costs_Bus_C_2)
 
 s.t.
 
-c_e_BusBlock_balance(Bus_C_0)_:
-+1 flow(cheap_plant_activity_costs_Bus_C_0)
+c_e_BusBlock_balance(Bus_C_0_0)_:
++1 flow(cheap_plant_activity_costs_Bus_C_0_0)
 = 0
 
-c_e_BusBlock_balance(Bus_C_1)_:
-+1 flow(cheap_plant_activity_costs_Bus_C_1)
+c_e_BusBlock_balance(Bus_C_0_1)_:
++1 flow(cheap_plant_activity_costs_Bus_C_0_1)
 = 0
 
-c_e_BusBlock_balance(Bus_C_2)_:
-+1 flow(cheap_plant_activity_costs_Bus_C_2)
+c_e_BusBlock_balance(Bus_C_0_2)_:
++1 flow(cheap_plant_activity_costs_Bus_C_0_2)
 = 0
 
 c_e_NonConvexFlowBlock_status_nominal_constraint(cheap_plant_activity_costs_Bus_C_0)_:
 -10 NonConvexFlowBlock_status(cheap_plant_activity_costs_Bus_C_0)
 +1 NonConvexFlowBlock_status_nominal(cheap_plant_activity_costs_Bus_C_0)
 = 0
 
@@ -34,51 +34,48 @@
 = 0
 
 c_e_NonConvexFlowBlock_status_nominal_constraint(cheap_plant_activity_costs_Bus_C_2)_:
 -10 NonConvexFlowBlock_status(cheap_plant_activity_costs_Bus_C_2)
 +1 NonConvexFlowBlock_status_nominal(cheap_plant_activity_costs_Bus_C_2)
 = 0
 
-c_u_NonConvexFlowBlock_min(cheap_plant_activity_costs_Bus_C_0)_:
+c_u_NonConvexFlowBlock_min(cheap_plant_activity_costs_Bus_C_0_0)_:
+-1 flow(cheap_plant_activity_costs_Bus_C_0_0)
 +0.5 NonConvexFlowBlock_status_nominal(cheap_plant_activity_costs_Bus_C_0)
--1 flow(cheap_plant_activity_costs_Bus_C_0)
 <= 0
 
-c_u_NonConvexFlowBlock_min(cheap_plant_activity_costs_Bus_C_1)_:
+c_u_NonConvexFlowBlock_min(cheap_plant_activity_costs_Bus_C_0_1)_:
+-1 flow(cheap_plant_activity_costs_Bus_C_0_1)
 +0.5 NonConvexFlowBlock_status_nominal(cheap_plant_activity_costs_Bus_C_1)
--1 flow(cheap_plant_activity_costs_Bus_C_1)
 <= 0
 
-c_u_NonConvexFlowBlock_min(cheap_plant_activity_costs_Bus_C_2)_:
+c_u_NonConvexFlowBlock_min(cheap_plant_activity_costs_Bus_C_0_2)_:
+-1 flow(cheap_plant_activity_costs_Bus_C_0_2)
 +0.5 NonConvexFlowBlock_status_nominal(cheap_plant_activity_costs_Bus_C_2)
--1 flow(cheap_plant_activity_costs_Bus_C_2)
 <= 0
 
-c_u_NonConvexFlowBlock_max(cheap_plant_activity_costs_Bus_C_0)_:
+c_u_NonConvexFlowBlock_max(cheap_plant_activity_costs_Bus_C_0_0)_:
++1 flow(cheap_plant_activity_costs_Bus_C_0_0)
 -1 NonConvexFlowBlock_status_nominal(cheap_plant_activity_costs_Bus_C_0)
-+1 flow(cheap_plant_activity_costs_Bus_C_0)
 <= 0
 
-c_u_NonConvexFlowBlock_max(cheap_plant_activity_costs_Bus_C_1)_:
+c_u_NonConvexFlowBlock_max(cheap_plant_activity_costs_Bus_C_0_1)_:
++1 flow(cheap_plant_activity_costs_Bus_C_0_1)
 -1 NonConvexFlowBlock_status_nominal(cheap_plant_activity_costs_Bus_C_1)
-+1 flow(cheap_plant_activity_costs_Bus_C_1)
 <= 0
 
-c_u_NonConvexFlowBlock_max(cheap_plant_activity_costs_Bus_C_2)_:
+c_u_NonConvexFlowBlock_max(cheap_plant_activity_costs_Bus_C_0_2)_:
++1 flow(cheap_plant_activity_costs_Bus_C_0_2)
 -1 NonConvexFlowBlock_status_nominal(cheap_plant_activity_costs_Bus_C_2)
-+1 flow(cheap_plant_activity_costs_Bus_C_2)
 <= 0
 
-c_e_ONE_VAR_CONSTANT:
-ONE_VAR_CONSTANT = 1.0
-
 bounds
-   0 <= flow(cheap_plant_activity_costs_Bus_C_0) <= 10
-   0 <= flow(cheap_plant_activity_costs_Bus_C_1) <= 10
-   0 <= flow(cheap_plant_activity_costs_Bus_C_2) <= 10
+   0 <= flow(cheap_plant_activity_costs_Bus_C_0_0) <= 10.0
+   0 <= flow(cheap_plant_activity_costs_Bus_C_0_1) <= 10.0
+   0 <= flow(cheap_plant_activity_costs_Bus_C_0_2) <= 10.0
    0 <= NonConvexFlowBlock_status(cheap_plant_activity_costs_Bus_C_0) <= 1
    0 <= NonConvexFlowBlock_status(cheap_plant_activity_costs_Bus_C_1) <= 1
    0 <= NonConvexFlowBlock_status(cheap_plant_activity_costs_Bus_C_2) <= 1
    0 <= NonConvexFlowBlock_status_nominal(cheap_plant_activity_costs_Bus_C_0) <= +inf
    0 <= NonConvexFlowBlock_status_nominal(cheap_plant_activity_costs_Bus_C_1) <= +inf
    0 <= NonConvexFlowBlock_status_nominal(cheap_plant_activity_costs_Bus_C_2) <= +inf
 binary
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/dsm_module_DIW.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/dsm_module_DIW_extended.lp`

 * *Files 3% similar despite different names*

```diff
@@ -1,160 +1,179 @@
 \* Source Pyomo model name=Model *\
 
-min
+min 
 objective:
-+2 SinkDSMDIWBlock_dsm_do_shift(demand_dsm_0_0)
-+2 SinkDSMDIWBlock_dsm_do_shift(demand_dsm_0_1)
-+2 SinkDSMDIWBlock_dsm_do_shift(demand_dsm_0_2)
-+2 SinkDSMDIWBlock_dsm_do_shift(demand_dsm_1_0)
-+2 SinkDSMDIWBlock_dsm_do_shift(demand_dsm_1_1)
-+2 SinkDSMDIWBlock_dsm_do_shift(demand_dsm_1_2)
-+2 SinkDSMDIWBlock_dsm_do_shift(demand_dsm_2_0)
-+2 SinkDSMDIWBlock_dsm_do_shift(demand_dsm_2_1)
-+2 SinkDSMDIWBlock_dsm_do_shift(demand_dsm_2_2)
++1 SinkDSMDIWBlock_dsm_do_shift(demand_dsm_0_0)
++1 SinkDSMDIWBlock_dsm_do_shift(demand_dsm_1_0)
++1 SinkDSMDIWBlock_dsm_do_shift(demand_dsm_2_0)
++100 SinkDSMDIWBlock_dsm_do_shed(demand_dsm_0)
++1 SinkDSMDIWBlock_dsm_up(demand_dsm_0)
++1 SinkDSMDIWBlock_dsm_up(demand_dsm_1)
++1 SinkDSMDIWBlock_dsm_do_shift(demand_dsm_0_1)
++1 SinkDSMDIWBlock_dsm_do_shift(demand_dsm_1_1)
++1 SinkDSMDIWBlock_dsm_do_shift(demand_dsm_2_1)
++100 SinkDSMDIWBlock_dsm_do_shed(demand_dsm_1)
++1 SinkDSMDIWBlock_dsm_up(demand_dsm_2)
++1 SinkDSMDIWBlock_dsm_do_shift(demand_dsm_0_2)
++1 SinkDSMDIWBlock_dsm_do_shift(demand_dsm_1_2)
++1 SinkDSMDIWBlock_dsm_do_shift(demand_dsm_2_2)
++100 SinkDSMDIWBlock_dsm_do_shed(demand_dsm_2)
 
 s.t.
 
-c_e_BusBlock_balance(bus_elec_0)_:
-+1 flow(bus_elec_demand_dsm_0)
-= 0
-
-c_e_BusBlock_balance(bus_elec_1)_:
-+1 flow(bus_elec_demand_dsm_1)
-= 0
-
-c_e_BusBlock_balance(bus_elec_2)_:
-+1 flow(bus_elec_demand_dsm_2)
+c_e_BusBlock_balance(bus_elec_0_0)_:
++1 flow(bus_elec_demand_dsm_0_0)
 = 0
 
-c_e_SinkDSMDIWBlock_shift_shed_vars(demand_dsm_0)_:
-+1 SinkDSMDIWBlock_dsm_do_shed(demand_dsm_0)
+c_e_BusBlock_balance(bus_elec_0_1)_:
++1 flow(bus_elec_demand_dsm_0_1)
 = 0
 
-c_e_SinkDSMDIWBlock_shift_shed_vars(demand_dsm_1)_:
-+1 SinkDSMDIWBlock_dsm_do_shed(demand_dsm_1)
+c_e_BusBlock_balance(bus_elec_0_2)_:
++1 flow(bus_elec_demand_dsm_0_2)
 = 0
 
-c_e_SinkDSMDIWBlock_shift_shed_vars(demand_dsm_2)_:
-+1 SinkDSMDIWBlock_dsm_do_shed(demand_dsm_2)
-= 0
-
-c_e_SinkDSMDIWBlock_input_output_relation(demand_dsm_0)_:
-+1 SinkDSMDIWBlock_dsm_do_shed(demand_dsm_0)
+c_e_SinkDSMDIWBlock_input_output_relation(demand_dsm_0_0)_:
 +1 SinkDSMDIWBlock_dsm_do_shift(demand_dsm_0_0)
 +1 SinkDSMDIWBlock_dsm_do_shift(demand_dsm_1_0)
++1 SinkDSMDIWBlock_dsm_do_shed(demand_dsm_0)
 -1 SinkDSMDIWBlock_dsm_up(demand_dsm_0)
-+1 flow(bus_elec_demand_dsm_0)
++1 flow(bus_elec_demand_dsm_0_0)
 = 1
 
-c_e_SinkDSMDIWBlock_input_output_relation(demand_dsm_1)_:
-+1 SinkDSMDIWBlock_dsm_do_shed(demand_dsm_1)
+c_e_SinkDSMDIWBlock_input_output_relation(demand_dsm_0_1)_:
+-1 SinkDSMDIWBlock_dsm_up(demand_dsm_1)
 +1 SinkDSMDIWBlock_dsm_do_shift(demand_dsm_0_1)
 +1 SinkDSMDIWBlock_dsm_do_shift(demand_dsm_1_1)
 +1 SinkDSMDIWBlock_dsm_do_shift(demand_dsm_2_1)
--1 SinkDSMDIWBlock_dsm_up(demand_dsm_1)
-+1 flow(bus_elec_demand_dsm_1)
-= 1
++1 SinkDSMDIWBlock_dsm_do_shed(demand_dsm_1)
++1 flow(bus_elec_demand_dsm_0_1)
+= 0.9
 
-c_e_SinkDSMDIWBlock_input_output_relation(demand_dsm_2)_:
-+1 SinkDSMDIWBlock_dsm_do_shed(demand_dsm_2)
+c_e_SinkDSMDIWBlock_input_output_relation(demand_dsm_0_2)_:
+-1 SinkDSMDIWBlock_dsm_up(demand_dsm_2)
 +1 SinkDSMDIWBlock_dsm_do_shift(demand_dsm_1_2)
 +1 SinkDSMDIWBlock_dsm_do_shift(demand_dsm_2_2)
--1 SinkDSMDIWBlock_dsm_up(demand_dsm_2)
-+1 flow(bus_elec_demand_dsm_2)
-= 1
++1 SinkDSMDIWBlock_dsm_do_shed(demand_dsm_2)
++1 flow(bus_elec_demand_dsm_0_2)
+= 0.8
 
 c_e_SinkDSMDIWBlock_dsm_updo_constraint(demand_dsm_0)_:
 -1 SinkDSMDIWBlock_dsm_do_shift(demand_dsm_0_0)
++0.99 SinkDSMDIWBlock_dsm_up(demand_dsm_0)
 -1 SinkDSMDIWBlock_dsm_do_shift(demand_dsm_0_1)
-+1 SinkDSMDIWBlock_dsm_up(demand_dsm_0)
 = 0
 
 c_e_SinkDSMDIWBlock_dsm_updo_constraint(demand_dsm_1)_:
 -1 SinkDSMDIWBlock_dsm_do_shift(demand_dsm_1_0)
++0.99 SinkDSMDIWBlock_dsm_up(demand_dsm_1)
 -1 SinkDSMDIWBlock_dsm_do_shift(demand_dsm_1_1)
 -1 SinkDSMDIWBlock_dsm_do_shift(demand_dsm_1_2)
-+1 SinkDSMDIWBlock_dsm_up(demand_dsm_1)
 = 0
 
 c_e_SinkDSMDIWBlock_dsm_updo_constraint(demand_dsm_2)_:
 -1 SinkDSMDIWBlock_dsm_do_shift(demand_dsm_2_1)
++0.99 SinkDSMDIWBlock_dsm_up(demand_dsm_2)
 -1 SinkDSMDIWBlock_dsm_do_shift(demand_dsm_2_2)
-+1 SinkDSMDIWBlock_dsm_up(demand_dsm_2)
 = 0
 
 c_u_SinkDSMDIWBlock_dsm_up_constraint(demand_dsm_0)_:
 +1 SinkDSMDIWBlock_dsm_up(demand_dsm_0)
 <= 0.5
 
 c_u_SinkDSMDIWBlock_dsm_up_constraint(demand_dsm_1)_:
 +1 SinkDSMDIWBlock_dsm_up(demand_dsm_1)
-<= 0.5
+<= 0.4
 
 c_u_SinkDSMDIWBlock_dsm_up_constraint(demand_dsm_2)_:
 +1 SinkDSMDIWBlock_dsm_up(demand_dsm_2)
 <= 0.5
 
 c_u_SinkDSMDIWBlock_dsm_do_constraint(demand_dsm_0)_:
-+1 SinkDSMDIWBlock_dsm_do_shed(demand_dsm_0)
 +1 SinkDSMDIWBlock_dsm_do_shift(demand_dsm_0_0)
 +1 SinkDSMDIWBlock_dsm_do_shift(demand_dsm_1_0)
-<= 0.5
++1 SinkDSMDIWBlock_dsm_do_shed(demand_dsm_0)
+<= 0.3
 
 c_u_SinkDSMDIWBlock_dsm_do_constraint(demand_dsm_1)_:
-+1 SinkDSMDIWBlock_dsm_do_shed(demand_dsm_1)
 +1 SinkDSMDIWBlock_dsm_do_shift(demand_dsm_0_1)
 +1 SinkDSMDIWBlock_dsm_do_shift(demand_dsm_1_1)
 +1 SinkDSMDIWBlock_dsm_do_shift(demand_dsm_2_1)
-<= 0.5
++1 SinkDSMDIWBlock_dsm_do_shed(demand_dsm_1)
+<= 0.3
 
 c_u_SinkDSMDIWBlock_dsm_do_constraint(demand_dsm_2)_:
-+1 SinkDSMDIWBlock_dsm_do_shed(demand_dsm_2)
 +1 SinkDSMDIWBlock_dsm_do_shift(demand_dsm_1_2)
 +1 SinkDSMDIWBlock_dsm_do_shift(demand_dsm_2_2)
-<= 0.5
++1 SinkDSMDIWBlock_dsm_do_shed(demand_dsm_2)
+<= 0.4
 
 c_u_SinkDSMDIWBlock_C2_constraint(demand_dsm_0)_:
-+1 SinkDSMDIWBlock_dsm_do_shed(demand_dsm_0)
 +1 SinkDSMDIWBlock_dsm_do_shift(demand_dsm_0_0)
 +1 SinkDSMDIWBlock_dsm_do_shift(demand_dsm_1_0)
++1 SinkDSMDIWBlock_dsm_do_shed(demand_dsm_0)
 +1 SinkDSMDIWBlock_dsm_up(demand_dsm_0)
 <= 0.5
 
 c_u_SinkDSMDIWBlock_C2_constraint(demand_dsm_1)_:
-+1 SinkDSMDIWBlock_dsm_do_shed(demand_dsm_1)
++1 SinkDSMDIWBlock_dsm_up(demand_dsm_1)
 +1 SinkDSMDIWBlock_dsm_do_shift(demand_dsm_0_1)
 +1 SinkDSMDIWBlock_dsm_do_shift(demand_dsm_1_1)
 +1 SinkDSMDIWBlock_dsm_do_shift(demand_dsm_2_1)
-+1 SinkDSMDIWBlock_dsm_up(demand_dsm_1)
-<= 0.5
++1 SinkDSMDIWBlock_dsm_do_shed(demand_dsm_1)
+<= 0.4
 
 c_u_SinkDSMDIWBlock_C2_constraint(demand_dsm_2)_:
-+1 SinkDSMDIWBlock_dsm_do_shed(demand_dsm_2)
++1 SinkDSMDIWBlock_dsm_up(demand_dsm_2)
 +1 SinkDSMDIWBlock_dsm_do_shift(demand_dsm_1_2)
 +1 SinkDSMDIWBlock_dsm_do_shift(demand_dsm_2_2)
++1 SinkDSMDIWBlock_dsm_do_shed(demand_dsm_2)
+<= 0.5
+
+c_u_SinkDSMDIWBlock_recovery_constraint(demand_dsm_0)_:
++1 SinkDSMDIWBlock_dsm_up(demand_dsm_0)
++1 SinkDSMDIWBlock_dsm_up(demand_dsm_1)
+<= 0.5
+
+c_u_SinkDSMDIWBlock_recovery_constraint(demand_dsm_1)_:
++1 SinkDSMDIWBlock_dsm_up(demand_dsm_1)
++1 SinkDSMDIWBlock_dsm_up(demand_dsm_2)
+<= 0.4
+
+c_u_SinkDSMDIWBlock_recovery_constraint(demand_dsm_2)_:
 +1 SinkDSMDIWBlock_dsm_up(demand_dsm_2)
 <= 0.5
 
-c_e_ONE_VAR_CONSTANT:
-ONE_VAR_CONSTANT = 1.0
+c_u_SinkDSMDIWBlock_shed_limit_constraint(demand_dsm_0)_:
++1 SinkDSMDIWBlock_dsm_do_shed(demand_dsm_0)
++1 SinkDSMDIWBlock_dsm_do_shed(demand_dsm_1)
+<= 0.6
+
+c_u_SinkDSMDIWBlock_shed_limit_constraint(demand_dsm_1)_:
++1 SinkDSMDIWBlock_dsm_do_shed(demand_dsm_1)
++1 SinkDSMDIWBlock_dsm_do_shed(demand_dsm_2)
+<= 0.6
+
+c_u_SinkDSMDIWBlock_shed_limit_constraint(demand_dsm_2)_:
++1 SinkDSMDIWBlock_dsm_do_shed(demand_dsm_2)
+<= 0.8
 
 bounds
-   0 <= flow(bus_elec_demand_dsm_0) <= +inf
-   0 <= flow(bus_elec_demand_dsm_1) <= +inf
-   0 <= flow(bus_elec_demand_dsm_2) <= +inf
    0 <= SinkDSMDIWBlock_dsm_do_shift(demand_dsm_0_0) <= +inf
-   0 <= SinkDSMDIWBlock_dsm_do_shift(demand_dsm_0_1) <= +inf
-   0 <= SinkDSMDIWBlock_dsm_do_shift(demand_dsm_0_2) <= +inf
    0 <= SinkDSMDIWBlock_dsm_do_shift(demand_dsm_1_0) <= +inf
-   0 <= SinkDSMDIWBlock_dsm_do_shift(demand_dsm_1_1) <= +inf
-   0 <= SinkDSMDIWBlock_dsm_do_shift(demand_dsm_1_2) <= +inf
    0 <= SinkDSMDIWBlock_dsm_do_shift(demand_dsm_2_0) <= +inf
-   0 <= SinkDSMDIWBlock_dsm_do_shift(demand_dsm_2_1) <= +inf
-   0 <= SinkDSMDIWBlock_dsm_do_shift(demand_dsm_2_2) <= +inf
    0 <= SinkDSMDIWBlock_dsm_do_shed(demand_dsm_0) <= +inf
-   0 <= SinkDSMDIWBlock_dsm_do_shed(demand_dsm_1) <= +inf
-   0 <= SinkDSMDIWBlock_dsm_do_shed(demand_dsm_2) <= +inf
    0 <= SinkDSMDIWBlock_dsm_up(demand_dsm_0) <= +inf
    0 <= SinkDSMDIWBlock_dsm_up(demand_dsm_1) <= +inf
+   0 <= SinkDSMDIWBlock_dsm_do_shift(demand_dsm_0_1) <= +inf
+   0 <= SinkDSMDIWBlock_dsm_do_shift(demand_dsm_1_1) <= +inf
+   0 <= SinkDSMDIWBlock_dsm_do_shift(demand_dsm_2_1) <= +inf
+   0 <= SinkDSMDIWBlock_dsm_do_shed(demand_dsm_1) <= +inf
    0 <= SinkDSMDIWBlock_dsm_up(demand_dsm_2) <= +inf
+   0 <= SinkDSMDIWBlock_dsm_do_shift(demand_dsm_0_2) <= +inf
+   0 <= SinkDSMDIWBlock_dsm_do_shift(demand_dsm_1_2) <= +inf
+   0 <= SinkDSMDIWBlock_dsm_do_shift(demand_dsm_2_2) <= +inf
+   0 <= SinkDSMDIWBlock_dsm_do_shed(demand_dsm_2) <= +inf
+   0 <= flow(bus_elec_demand_dsm_0_0) <= +inf
+   0 <= flow(bus_elec_demand_dsm_0_1) <= +inf
+   0 <= flow(bus_elec_demand_dsm_0_2) <= +inf
 end
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/dsm_module_DIW_invest.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/dsm_module_DIW_invest.lp`

 * *Files 7% similar despite different names*

```diff
@@ -1,173 +1,184 @@
 \* Source Pyomo model name=Model *\
 
-min
+min 
 objective:
-+2 SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_0_0)
-+2 SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_0_1)
-+2 SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_0_2)
-+2 SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_1_0)
-+2 SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_1_1)
-+2 SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_1_2)
-+2 SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_2_0)
-+2 SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_2_1)
-+2 SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_2_2)
++1 SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_0_0)
++1 SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_1_0)
++1 SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_2_0)
++100 SinkDSMDIWInvestmentBlock_dsm_do_shed(demand_dsm_0)
++1 SinkDSMDIWInvestmentBlock_dsm_up(demand_dsm_0)
++1 SinkDSMDIWInvestmentBlock_dsm_up(demand_dsm_1)
++1 SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_0_1)
++1 SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_1_1)
++1 SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_2_1)
++100 SinkDSMDIWInvestmentBlock_dsm_do_shed(demand_dsm_1)
++1 SinkDSMDIWInvestmentBlock_dsm_up(demand_dsm_2)
++1 SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_0_2)
++1 SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_1_2)
++1 SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_2_2)
++100 SinkDSMDIWInvestmentBlock_dsm_do_shed(demand_dsm_2)
 
 s.t.
 
-c_e_BusBlock_balance(bus_elec_0)_:
-+1 flow(bus_elec_demand_dsm_0)
+c_e_BusBlock_balance(bus_elec_0_0)_:
++1 flow(bus_elec_demand_dsm_0_0)
 = 0
 
-c_e_BusBlock_balance(bus_elec_1)_:
-+1 flow(bus_elec_demand_dsm_1)
+c_e_BusBlock_balance(bus_elec_0_1)_:
++1 flow(bus_elec_demand_dsm_0_1)
 = 0
 
-c_e_BusBlock_balance(bus_elec_2)_:
-+1 flow(bus_elec_demand_dsm_2)
+c_e_BusBlock_balance(bus_elec_0_2)_:
++1 flow(bus_elec_demand_dsm_0_2)
 = 0
 
-c_e_SinkDSMDIWInvestmentBlock_shift_shed_vars(demand_dsm_0)_:
-+1 SinkDSMDIWInvestmentBlock_dsm_do_shed(demand_dsm_0)
-= 0
-
-c_e_SinkDSMDIWInvestmentBlock_shift_shed_vars(demand_dsm_1)_:
-+1 SinkDSMDIWInvestmentBlock_dsm_do_shed(demand_dsm_1)
-= 0
-
-c_e_SinkDSMDIWInvestmentBlock_shift_shed_vars(demand_dsm_2)_:
-+1 SinkDSMDIWInvestmentBlock_dsm_do_shed(demand_dsm_2)
-= 0
+c_e_SinkDSMDIWInvestmentBlock_total_dsm_rule(demand_dsm_0)_:
++1 SinkDSMDIWInvestmentBlock_total(demand_dsm_0)
+-1 SinkDSMDIWInvestmentBlock_invest(demand_dsm_0)
+= 50
 
-c_e_SinkDSMDIWInvestmentBlock_input_output_relation(demand_dsm_0)_:
-+1 SinkDSMDIWInvestmentBlock_dsm_do_shed(demand_dsm_0)
+c_e_SinkDSMDIWInvestmentBlock_input_output_relation(demand_dsm_0_0)_:
 +1 SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_0_0)
 +1 SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_1_0)
++1 SinkDSMDIWInvestmentBlock_dsm_do_shed(demand_dsm_0)
 -1 SinkDSMDIWInvestmentBlock_dsm_up(demand_dsm_0)
--1 SinkDSMDIWInvestmentBlock_invest(demand_dsm)
-+1 flow(bus_elec_demand_dsm_0)
-= 50
++1 flow(bus_elec_demand_dsm_0_0)
+= 1
 
-c_e_SinkDSMDIWInvestmentBlock_input_output_relation(demand_dsm_1)_:
-+1 SinkDSMDIWInvestmentBlock_dsm_do_shed(demand_dsm_1)
+c_e_SinkDSMDIWInvestmentBlock_input_output_relation(demand_dsm_0_1)_:
+-1 SinkDSMDIWInvestmentBlock_dsm_up(demand_dsm_1)
 +1 SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_0_1)
 +1 SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_1_1)
 +1 SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_2_1)
--1 SinkDSMDIWInvestmentBlock_dsm_up(demand_dsm_1)
--1 SinkDSMDIWInvestmentBlock_invest(demand_dsm)
-+1 flow(bus_elec_demand_dsm_1)
-= 50
++1 SinkDSMDIWInvestmentBlock_dsm_do_shed(demand_dsm_1)
++1 flow(bus_elec_demand_dsm_0_1)
+= 1
 
-c_e_SinkDSMDIWInvestmentBlock_input_output_relation(demand_dsm_2)_:
-+1 SinkDSMDIWInvestmentBlock_dsm_do_shed(demand_dsm_2)
+c_e_SinkDSMDIWInvestmentBlock_input_output_relation(demand_dsm_0_2)_:
+-1 SinkDSMDIWInvestmentBlock_dsm_up(demand_dsm_2)
 +1 SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_1_2)
 +1 SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_2_2)
--1 SinkDSMDIWInvestmentBlock_dsm_up(demand_dsm_2)
--1 SinkDSMDIWInvestmentBlock_invest(demand_dsm)
-+1 flow(bus_elec_demand_dsm_2)
-= 50
++1 SinkDSMDIWInvestmentBlock_dsm_do_shed(demand_dsm_2)
++1 flow(bus_elec_demand_dsm_0_2)
+= 1
 
 c_e_SinkDSMDIWInvestmentBlock_dsm_updo_constraint(demand_dsm_0)_:
 -1 SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_0_0)
--1 SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_0_1)
 +1 SinkDSMDIWInvestmentBlock_dsm_up(demand_dsm_0)
+-1 SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_0_1)
 = 0
 
 c_e_SinkDSMDIWInvestmentBlock_dsm_updo_constraint(demand_dsm_1)_:
 -1 SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_1_0)
++1 SinkDSMDIWInvestmentBlock_dsm_up(demand_dsm_1)
 -1 SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_1_1)
 -1 SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_1_2)
-+1 SinkDSMDIWInvestmentBlock_dsm_up(demand_dsm_1)
 = 0
 
 c_e_SinkDSMDIWInvestmentBlock_dsm_updo_constraint(demand_dsm_2)_:
 -1 SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_2_1)
--1 SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_2_2)
 +1 SinkDSMDIWInvestmentBlock_dsm_up(demand_dsm_2)
+-1 SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_2_2)
 = 0
 
-c_u_SinkDSMDIWInvestmentBlock_dsm_up_constraint(demand_dsm_0)_:
+c_u_SinkDSMDIWInvestmentBlock_dsm_up_constraint(demand_dsm_0_0)_:
 +1 SinkDSMDIWInvestmentBlock_dsm_up(demand_dsm_0)
--0.5 SinkDSMDIWInvestmentBlock_invest(demand_dsm)
-<= 25
+-0.5 SinkDSMDIWInvestmentBlock_total(demand_dsm_0)
+<= 0
 
-c_u_SinkDSMDIWInvestmentBlock_dsm_up_constraint(demand_dsm_1)_:
+c_u_SinkDSMDIWInvestmentBlock_dsm_up_constraint(demand_dsm_0_1)_:
 +1 SinkDSMDIWInvestmentBlock_dsm_up(demand_dsm_1)
--0.5 SinkDSMDIWInvestmentBlock_invest(demand_dsm)
-<= 25
+-0.5 SinkDSMDIWInvestmentBlock_total(demand_dsm_0)
+<= 0
 
-c_u_SinkDSMDIWInvestmentBlock_dsm_up_constraint(demand_dsm_2)_:
+c_u_SinkDSMDIWInvestmentBlock_dsm_up_constraint(demand_dsm_0_2)_:
 +1 SinkDSMDIWInvestmentBlock_dsm_up(demand_dsm_2)
--0.5 SinkDSMDIWInvestmentBlock_invest(demand_dsm)
-<= 25
+-0.5 SinkDSMDIWInvestmentBlock_total(demand_dsm_0)
+<= 0
 
-c_u_SinkDSMDIWInvestmentBlock_dsm_do_constraint(demand_dsm_0)_:
-+1 SinkDSMDIWInvestmentBlock_dsm_do_shed(demand_dsm_0)
+c_u_SinkDSMDIWInvestmentBlock_dsm_do_constraint(demand_dsm_0_0)_:
 +1 SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_0_0)
 +1 SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_1_0)
--0.5 SinkDSMDIWInvestmentBlock_invest(demand_dsm)
-<= 25
++1 SinkDSMDIWInvestmentBlock_dsm_do_shed(demand_dsm_0)
+-0.5 SinkDSMDIWInvestmentBlock_total(demand_dsm_0)
+<= 0
 
-c_u_SinkDSMDIWInvestmentBlock_dsm_do_constraint(demand_dsm_1)_:
-+1 SinkDSMDIWInvestmentBlock_dsm_do_shed(demand_dsm_1)
+c_u_SinkDSMDIWInvestmentBlock_dsm_do_constraint(demand_dsm_0_1)_:
 +1 SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_0_1)
 +1 SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_1_1)
 +1 SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_2_1)
--0.5 SinkDSMDIWInvestmentBlock_invest(demand_dsm)
-<= 25
++1 SinkDSMDIWInvestmentBlock_dsm_do_shed(demand_dsm_1)
+-0.5 SinkDSMDIWInvestmentBlock_total(demand_dsm_0)
+<= 0
 
-c_u_SinkDSMDIWInvestmentBlock_dsm_do_constraint(demand_dsm_2)_:
-+1 SinkDSMDIWInvestmentBlock_dsm_do_shed(demand_dsm_2)
+c_u_SinkDSMDIWInvestmentBlock_dsm_do_constraint(demand_dsm_0_2)_:
 +1 SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_1_2)
 +1 SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_2_2)
--0.5 SinkDSMDIWInvestmentBlock_invest(demand_dsm)
-<= 25
++1 SinkDSMDIWInvestmentBlock_dsm_do_shed(demand_dsm_2)
+-0.5 SinkDSMDIWInvestmentBlock_total(demand_dsm_0)
+<= 0
 
-c_u_SinkDSMDIWInvestmentBlock_C2_constraint(demand_dsm_0)_:
-+1 SinkDSMDIWInvestmentBlock_dsm_do_shed(demand_dsm_0)
+c_u_SinkDSMDIWInvestmentBlock_C2_constraint(demand_dsm_0_0)_:
 +1 SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_0_0)
 +1 SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_1_0)
++1 SinkDSMDIWInvestmentBlock_dsm_do_shed(demand_dsm_0)
 +1 SinkDSMDIWInvestmentBlock_dsm_up(demand_dsm_0)
--0.5 SinkDSMDIWInvestmentBlock_invest(demand_dsm)
-<= 25
+-0.5 SinkDSMDIWInvestmentBlock_total(demand_dsm_0)
+<= 0
 
-c_u_SinkDSMDIWInvestmentBlock_C2_constraint(demand_dsm_1)_:
-+1 SinkDSMDIWInvestmentBlock_dsm_do_shed(demand_dsm_1)
+c_u_SinkDSMDIWInvestmentBlock_C2_constraint(demand_dsm_0_1)_:
++1 SinkDSMDIWInvestmentBlock_dsm_up(demand_dsm_1)
 +1 SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_0_1)
 +1 SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_1_1)
 +1 SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_2_1)
-+1 SinkDSMDIWInvestmentBlock_dsm_up(demand_dsm_1)
--0.5 SinkDSMDIWInvestmentBlock_invest(demand_dsm)
-<= 25
++1 SinkDSMDIWInvestmentBlock_dsm_do_shed(demand_dsm_1)
+-0.5 SinkDSMDIWInvestmentBlock_total(demand_dsm_0)
+<= 0
 
-c_u_SinkDSMDIWInvestmentBlock_C2_constraint(demand_dsm_2)_:
-+1 SinkDSMDIWInvestmentBlock_dsm_do_shed(demand_dsm_2)
+c_u_SinkDSMDIWInvestmentBlock_C2_constraint(demand_dsm_0_2)_:
++1 SinkDSMDIWInvestmentBlock_dsm_up(demand_dsm_2)
 +1 SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_1_2)
 +1 SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_2_2)
-+1 SinkDSMDIWInvestmentBlock_dsm_up(demand_dsm_2)
--0.5 SinkDSMDIWInvestmentBlock_invest(demand_dsm)
-<= 25
++1 SinkDSMDIWInvestmentBlock_dsm_do_shed(demand_dsm_2)
+-0.5 SinkDSMDIWInvestmentBlock_total(demand_dsm_0)
+<= 0
+
+c_u_SinkDSMDIWInvestmentBlock_shed_limit_constraint(demand_dsm_0_0)_:
++1 SinkDSMDIWInvestmentBlock_dsm_do_shed(demand_dsm_0)
++1 SinkDSMDIWInvestmentBlock_dsm_do_shed(demand_dsm_1)
+-1.0 SinkDSMDIWInvestmentBlock_total(demand_dsm_0)
+<= 0
+
+c_u_SinkDSMDIWInvestmentBlock_shed_limit_constraint(demand_dsm_0_1)_:
++1 SinkDSMDIWInvestmentBlock_dsm_do_shed(demand_dsm_1)
++1 SinkDSMDIWInvestmentBlock_dsm_do_shed(demand_dsm_2)
+-1.0 SinkDSMDIWInvestmentBlock_total(demand_dsm_0)
+<= 0
 
-c_e_ONE_VAR_CONSTANT:
-ONE_VAR_CONSTANT = 1.0
+c_u_SinkDSMDIWInvestmentBlock_shed_limit_constraint(demand_dsm_0_2)_:
++1 SinkDSMDIWInvestmentBlock_dsm_do_shed(demand_dsm_2)
+-1.0 SinkDSMDIWInvestmentBlock_total(demand_dsm_0)
+<= 0
 
 bounds
-   0 <= flow(bus_elec_demand_dsm_0) <= +inf
-   0 <= flow(bus_elec_demand_dsm_1) <= +inf
-   0 <= flow(bus_elec_demand_dsm_2) <= +inf
-   33 <= SinkDSMDIWInvestmentBlock_invest(demand_dsm) <= 100
    0 <= SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_0_0) <= +inf
-   0 <= SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_0_1) <= +inf
-   0 <= SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_0_2) <= +inf
    0 <= SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_1_0) <= +inf
-   0 <= SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_1_1) <= +inf
-   0 <= SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_1_2) <= +inf
    0 <= SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_2_0) <= +inf
-   0 <= SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_2_1) <= +inf
-   0 <= SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_2_2) <= +inf
    0 <= SinkDSMDIWInvestmentBlock_dsm_do_shed(demand_dsm_0) <= +inf
-   0 <= SinkDSMDIWInvestmentBlock_dsm_do_shed(demand_dsm_1) <= +inf
-   0 <= SinkDSMDIWInvestmentBlock_dsm_do_shed(demand_dsm_2) <= +inf
    0 <= SinkDSMDIWInvestmentBlock_dsm_up(demand_dsm_0) <= +inf
    0 <= SinkDSMDIWInvestmentBlock_dsm_up(demand_dsm_1) <= +inf
+   0 <= SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_0_1) <= +inf
+   0 <= SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_1_1) <= +inf
+   0 <= SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_2_1) <= +inf
+   0 <= SinkDSMDIWInvestmentBlock_dsm_do_shed(demand_dsm_1) <= +inf
    0 <= SinkDSMDIWInvestmentBlock_dsm_up(demand_dsm_2) <= +inf
+   0 <= SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_0_2) <= +inf
+   0 <= SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_1_2) <= +inf
+   0 <= SinkDSMDIWInvestmentBlock_dsm_do_shift(demand_dsm_2_2) <= +inf
+   0 <= SinkDSMDIWInvestmentBlock_dsm_do_shed(demand_dsm_2) <= +inf
+   0 <= flow(bus_elec_demand_dsm_0_0) <= +inf
+   0 <= flow(bus_elec_demand_dsm_0_1) <= +inf
+   0 <= flow(bus_elec_demand_dsm_0_2) <= +inf
+   0 <= SinkDSMDIWInvestmentBlock_total(demand_dsm_0) <= +inf
+   33 <= SinkDSMDIWInvestmentBlock_invest(demand_dsm_0) <= 100
 end
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/dsm_module_DLR.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/dsm_module_DLR_delay_time.lp`

 * *Files 2% similar despite different names*

```diff
@@ -1,260 +1,258 @@
 \* Source Pyomo model name=Model *\
 
-min
+min 
 objective:
-+2 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_1_0)
-+2 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_1_1)
-+2 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_1_2)
-+2 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_2_0)
-+2 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_2_1)
-+2 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_2_2)
 +2 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_1_0)
++2 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_1_0)
++2 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_3_0)
++2 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_3_0)
 +2 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_1_1)
++2 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_1_1)
++2 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_3_1)
++2 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_3_1)
 +2 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_1_2)
-+2 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_2_0)
-+2 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_2_1)
-+2 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_2_2)
++2 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_1_2)
++2 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_3_2)
++2 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_3_2)
 
 s.t.
 
-c_e_BusBlock_balance(bus_elec_0)_:
-+1 flow(bus_elec_demand_dsm_0)
+c_e_BusBlock_balance(bus_elec_0_0)_:
++1 flow(bus_elec_demand_dsm_0_0)
 = 0
 
-c_e_BusBlock_balance(bus_elec_1)_:
-+1 flow(bus_elec_demand_dsm_1)
+c_e_BusBlock_balance(bus_elec_0_1)_:
++1 flow(bus_elec_demand_dsm_0_1)
 = 0
 
-c_e_BusBlock_balance(bus_elec_2)_:
-+1 flow(bus_elec_demand_dsm_2)
+c_e_BusBlock_balance(bus_elec_0_2)_:
++1 flow(bus_elec_demand_dsm_0_2)
 = 0
 
 c_e_SinkDSMDLRBlock_shift_shed_vars(demand_dsm_1_0)_:
 +1 SinkDSMDLRBlock_dsm_do_shed(demand_dsm_0)
 = 0
 
 c_e_SinkDSMDLRBlock_shift_shed_vars(demand_dsm_1_1)_:
 +1 SinkDSMDLRBlock_dsm_do_shed(demand_dsm_1)
 = 0
 
 c_e_SinkDSMDLRBlock_shift_shed_vars(demand_dsm_1_2)_:
 +1 SinkDSMDLRBlock_dsm_do_shed(demand_dsm_2)
 = 0
 
-c_e_SinkDSMDLRBlock_shift_shed_vars(demand_dsm_2_0)_:
+c_e_SinkDSMDLRBlock_shift_shed_vars(demand_dsm_3_0)_:
 +1 SinkDSMDLRBlock_dsm_do_shed(demand_dsm_0)
 = 0
 
-c_e_SinkDSMDLRBlock_shift_shed_vars(demand_dsm_2_1)_:
+c_e_SinkDSMDLRBlock_shift_shed_vars(demand_dsm_3_1)_:
 +1 SinkDSMDLRBlock_dsm_do_shed(demand_dsm_1)
 = 0
 
-c_e_SinkDSMDLRBlock_shift_shed_vars(demand_dsm_2_2)_:
+c_e_SinkDSMDLRBlock_shift_shed_vars(demand_dsm_3_2)_:
 +1 SinkDSMDLRBlock_dsm_do_shed(demand_dsm_2)
 = 0
 
-c_e_SinkDSMDLRBlock_input_output_relation(demand_dsm_0)_:
--1 SinkDSMDLRBlock_balance_dsm_do(demand_dsm_1_0)
--1 SinkDSMDLRBlock_balance_dsm_do(demand_dsm_2_0)
-+1 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_1_0)
-+1 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_2_0)
-+1 SinkDSMDLRBlock_dsm_do_shed(demand_dsm_0)
+c_e_SinkDSMDLRBlock_input_output_relation(demand_dsm_0_0)_:
 +1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_1_0)
-+1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_2_0)
++1 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_1_0)
++1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_3_0)
++1 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_3_0)
 -1 SinkDSMDLRBlock_dsm_up(demand_dsm_1_0)
--1 SinkDSMDLRBlock_dsm_up(demand_dsm_2_0)
-+1 flow(bus_elec_demand_dsm_0)
+-1 SinkDSMDLRBlock_balance_dsm_do(demand_dsm_1_0)
+-1 SinkDSMDLRBlock_dsm_up(demand_dsm_3_0)
+-1 SinkDSMDLRBlock_balance_dsm_do(demand_dsm_3_0)
++1 flow(bus_elec_demand_dsm_0_0)
++1 SinkDSMDLRBlock_dsm_do_shed(demand_dsm_0)
 = 1
 
-c_e_SinkDSMDLRBlock_input_output_relation(demand_dsm_1)_:
+c_e_SinkDSMDLRBlock_input_output_relation(demand_dsm_0_1)_:
+-1 SinkDSMDLRBlock_dsm_up(demand_dsm_1_1)
 -1 SinkDSMDLRBlock_balance_dsm_do(demand_dsm_1_1)
--1 SinkDSMDLRBlock_balance_dsm_do(demand_dsm_2_1)
+-1 SinkDSMDLRBlock_dsm_up(demand_dsm_3_1)
+-1 SinkDSMDLRBlock_balance_dsm_do(demand_dsm_3_1)
++1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_1_1)
 +1 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_1_1)
-+1 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_2_1)
++1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_3_1)
++1 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_3_1)
++1 flow(bus_elec_demand_dsm_0_1)
 +1 SinkDSMDLRBlock_dsm_do_shed(demand_dsm_1)
-+1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_1_1)
-+1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_2_1)
--1 SinkDSMDLRBlock_dsm_up(demand_dsm_1_1)
--1 SinkDSMDLRBlock_dsm_up(demand_dsm_2_1)
-+1 flow(bus_elec_demand_dsm_1)
 = 1
 
-c_e_SinkDSMDLRBlock_input_output_relation(demand_dsm_2)_:
+c_e_SinkDSMDLRBlock_input_output_relation(demand_dsm_0_2)_:
+-1 SinkDSMDLRBlock_dsm_up(demand_dsm_1_2)
 -1 SinkDSMDLRBlock_balance_dsm_do(demand_dsm_1_2)
--1 SinkDSMDLRBlock_balance_dsm_do(demand_dsm_2_2)
+-1 SinkDSMDLRBlock_dsm_up(demand_dsm_3_2)
+-1 SinkDSMDLRBlock_balance_dsm_do(demand_dsm_3_2)
++1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_1_2)
 +1 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_1_2)
-+1 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_2_2)
++1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_3_2)
++1 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_3_2)
++1 flow(bus_elec_demand_dsm_0_2)
 +1 SinkDSMDLRBlock_dsm_do_shed(demand_dsm_2)
-+1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_1_2)
-+1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_2_2)
--1 SinkDSMDLRBlock_dsm_up(demand_dsm_1_2)
--1 SinkDSMDLRBlock_dsm_up(demand_dsm_2_2)
-+1 flow(bus_elec_demand_dsm_2)
 = 1
 
 c_e_SinkDSMDLRBlock_capacity_balance_red(demand_dsm_1_0)_:
 +1 SinkDSMDLRBlock_balance_dsm_do(demand_dsm_1_0)
 = 0
 
 c_e_SinkDSMDLRBlock_capacity_balance_red(demand_dsm_1_1)_:
-+1 SinkDSMDLRBlock_balance_dsm_do(demand_dsm_1_1)
 -1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_1_0)
++1 SinkDSMDLRBlock_balance_dsm_do(demand_dsm_1_1)
 = 0
 
 c_e_SinkDSMDLRBlock_capacity_balance_red(demand_dsm_1_2)_:
-+1 SinkDSMDLRBlock_balance_dsm_do(demand_dsm_1_2)
 -1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_1_1)
++1 SinkDSMDLRBlock_balance_dsm_do(demand_dsm_1_2)
 = 0
 
-c_e_SinkDSMDLRBlock_capacity_balance_red(demand_dsm_2_0)_:
-+1 SinkDSMDLRBlock_balance_dsm_do(demand_dsm_2_0)
-= 0
-
-c_e_SinkDSMDLRBlock_capacity_balance_red(demand_dsm_2_2)_:
-+1 SinkDSMDLRBlock_balance_dsm_do(demand_dsm_2_2)
--1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_2_0)
+c_e_SinkDSMDLRBlock_capacity_balance_red(demand_dsm_3_0)_:
++1 SinkDSMDLRBlock_balance_dsm_do(demand_dsm_3_0)
 = 0
 
 c_e_SinkDSMDLRBlock_capacity_balance_inc(demand_dsm_1_0)_:
 +1 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_1_0)
 = 0
 
 c_e_SinkDSMDLRBlock_capacity_balance_inc(demand_dsm_1_1)_:
-+1 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_1_1)
 -1 SinkDSMDLRBlock_dsm_up(demand_dsm_1_0)
++1 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_1_1)
 = 0
 
 c_e_SinkDSMDLRBlock_capacity_balance_inc(demand_dsm_1_2)_:
-+1 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_1_2)
 -1 SinkDSMDLRBlock_dsm_up(demand_dsm_1_1)
++1 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_1_2)
 = 0
 
-c_e_SinkDSMDLRBlock_capacity_balance_inc(demand_dsm_2_0)_:
-+1 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_2_0)
-= 0
-
-c_e_SinkDSMDLRBlock_capacity_balance_inc(demand_dsm_2_2)_:
-+1 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_2_2)
--1 SinkDSMDLRBlock_dsm_up(demand_dsm_2_0)
+c_e_SinkDSMDLRBlock_capacity_balance_inc(demand_dsm_3_0)_:
++1 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_3_0)
 = 0
 
 c_e_SinkDSMDLRBlock_no_comp_red(demand_dsm_1_2)_:
 +1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_1_2)
 = 0
 
-c_e_SinkDSMDLRBlock_no_comp_red(demand_dsm_2_1)_:
-+1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_2_1)
+c_e_SinkDSMDLRBlock_no_comp_red(demand_dsm_3_0)_:
++1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_3_0)
 = 0
 
-c_e_SinkDSMDLRBlock_no_comp_red(demand_dsm_2_2)_:
-+1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_2_2)
+c_e_SinkDSMDLRBlock_no_comp_red(demand_dsm_3_1)_:
++1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_3_1)
+= 0
+
+c_e_SinkDSMDLRBlock_no_comp_red(demand_dsm_3_2)_:
++1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_3_2)
 = 0
 
 c_e_SinkDSMDLRBlock_no_comp_inc(demand_dsm_1_2)_:
 +1 SinkDSMDLRBlock_dsm_up(demand_dsm_1_2)
 = 0
 
-c_e_SinkDSMDLRBlock_no_comp_inc(demand_dsm_2_1)_:
-+1 SinkDSMDLRBlock_dsm_up(demand_dsm_2_1)
+c_e_SinkDSMDLRBlock_no_comp_inc(demand_dsm_3_0)_:
++1 SinkDSMDLRBlock_dsm_up(demand_dsm_3_0)
 = 0
 
-c_e_SinkDSMDLRBlock_no_comp_inc(demand_dsm_2_2)_:
-+1 SinkDSMDLRBlock_dsm_up(demand_dsm_2_2)
+c_e_SinkDSMDLRBlock_no_comp_inc(demand_dsm_3_1)_:
++1 SinkDSMDLRBlock_dsm_up(demand_dsm_3_1)
+= 0
+
+c_e_SinkDSMDLRBlock_no_comp_inc(demand_dsm_3_2)_:
++1 SinkDSMDLRBlock_dsm_up(demand_dsm_3_2)
 = 0
 
 c_u_SinkDSMDLRBlock_availability_red(demand_dsm_0)_:
++1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_1_0)
 +1 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_1_0)
-+1 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_2_0)
++1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_3_0)
++1 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_3_0)
 +1 SinkDSMDLRBlock_dsm_do_shed(demand_dsm_0)
-+1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_1_0)
-+1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_2_0)
 <= 0.5
 
 c_u_SinkDSMDLRBlock_availability_red(demand_dsm_1)_:
++1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_1_1)
 +1 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_1_1)
-+1 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_2_1)
++1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_3_1)
++1 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_3_1)
 +1 SinkDSMDLRBlock_dsm_do_shed(demand_dsm_1)
-+1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_1_1)
-+1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_2_1)
 <= 0.5
 
 c_u_SinkDSMDLRBlock_availability_red(demand_dsm_2)_:
++1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_1_2)
 +1 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_1_2)
-+1 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_2_2)
++1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_3_2)
++1 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_3_2)
 +1 SinkDSMDLRBlock_dsm_do_shed(demand_dsm_2)
-+1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_1_2)
-+1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_2_2)
 <= 0.5
 
 c_u_SinkDSMDLRBlock_availability_inc(demand_dsm_0)_:
-+1 SinkDSMDLRBlock_balance_dsm_do(demand_dsm_1_0)
-+1 SinkDSMDLRBlock_balance_dsm_do(demand_dsm_2_0)
 +1 SinkDSMDLRBlock_dsm_up(demand_dsm_1_0)
-+1 SinkDSMDLRBlock_dsm_up(demand_dsm_2_0)
++1 SinkDSMDLRBlock_balance_dsm_do(demand_dsm_1_0)
++1 SinkDSMDLRBlock_dsm_up(demand_dsm_3_0)
++1 SinkDSMDLRBlock_balance_dsm_do(demand_dsm_3_0)
 <= 0.5
 
 c_u_SinkDSMDLRBlock_availability_inc(demand_dsm_1)_:
-+1 SinkDSMDLRBlock_balance_dsm_do(demand_dsm_1_1)
-+1 SinkDSMDLRBlock_balance_dsm_do(demand_dsm_2_1)
 +1 SinkDSMDLRBlock_dsm_up(demand_dsm_1_1)
-+1 SinkDSMDLRBlock_dsm_up(demand_dsm_2_1)
++1 SinkDSMDLRBlock_balance_dsm_do(demand_dsm_1_1)
++1 SinkDSMDLRBlock_dsm_up(demand_dsm_3_1)
++1 SinkDSMDLRBlock_balance_dsm_do(demand_dsm_3_1)
 <= 0.5
 
 c_u_SinkDSMDLRBlock_availability_inc(demand_dsm_2)_:
-+1 SinkDSMDLRBlock_balance_dsm_do(demand_dsm_1_2)
-+1 SinkDSMDLRBlock_balance_dsm_do(demand_dsm_2_2)
 +1 SinkDSMDLRBlock_dsm_up(demand_dsm_1_2)
-+1 SinkDSMDLRBlock_dsm_up(demand_dsm_2_2)
++1 SinkDSMDLRBlock_balance_dsm_do(demand_dsm_1_2)
++1 SinkDSMDLRBlock_dsm_up(demand_dsm_3_2)
++1 SinkDSMDLRBlock_balance_dsm_do(demand_dsm_3_2)
 <= 0.5
 
 c_e_SinkDSMDLRBlock_dr_storage_red(demand_dsm_0)_:
-+1 SinkDSMDLRBlock_dsm_do_level(demand_dsm_0)
 -1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_1_0)
--1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_2_0)
+-1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_3_0)
++1 SinkDSMDLRBlock_dsm_do_level(demand_dsm_0)
 = 0
 
 c_e_SinkDSMDLRBlock_dr_storage_red(demand_dsm_1)_:
 -1 SinkDSMDLRBlock_balance_dsm_do(demand_dsm_1_1)
--1 SinkDSMDLRBlock_balance_dsm_do(demand_dsm_2_1)
+-1 SinkDSMDLRBlock_balance_dsm_do(demand_dsm_3_1)
++1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_1_1)
++1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_3_1)
 +1 SinkDSMDLRBlock_dsm_do_level(demand_dsm_0)
 -1 SinkDSMDLRBlock_dsm_do_level(demand_dsm_1)
-+1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_1_1)
-+1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_2_1)
 = 0
 
 c_e_SinkDSMDLRBlock_dr_storage_red(demand_dsm_2)_:
 -1 SinkDSMDLRBlock_balance_dsm_do(demand_dsm_1_2)
--1 SinkDSMDLRBlock_balance_dsm_do(demand_dsm_2_2)
+-1 SinkDSMDLRBlock_balance_dsm_do(demand_dsm_3_2)
++1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_1_2)
++1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_3_2)
 +1 SinkDSMDLRBlock_dsm_do_level(demand_dsm_1)
 -1 SinkDSMDLRBlock_dsm_do_level(demand_dsm_2)
-+1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_1_2)
-+1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_2_2)
 = 0
 
 c_e_SinkDSMDLRBlock_dr_storage_inc(demand_dsm_0)_:
 -1 SinkDSMDLRBlock_dsm_up(demand_dsm_1_0)
--1 SinkDSMDLRBlock_dsm_up(demand_dsm_2_0)
+-1 SinkDSMDLRBlock_dsm_up(demand_dsm_3_0)
 +1 SinkDSMDLRBlock_dsm_up_level(demand_dsm_0)
 = 0
 
 c_e_SinkDSMDLRBlock_dr_storage_inc(demand_dsm_1)_:
--1 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_1_1)
--1 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_2_1)
 +1 SinkDSMDLRBlock_dsm_up(demand_dsm_1_1)
-+1 SinkDSMDLRBlock_dsm_up(demand_dsm_2_1)
++1 SinkDSMDLRBlock_dsm_up(demand_dsm_3_1)
+-1 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_1_1)
+-1 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_3_1)
 +1 SinkDSMDLRBlock_dsm_up_level(demand_dsm_0)
 -1 SinkDSMDLRBlock_dsm_up_level(demand_dsm_1)
 = 0
 
 c_e_SinkDSMDLRBlock_dr_storage_inc(demand_dsm_2)_:
--1 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_1_2)
--1 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_2_2)
 +1 SinkDSMDLRBlock_dsm_up(demand_dsm_1_2)
-+1 SinkDSMDLRBlock_dsm_up(demand_dsm_2_2)
++1 SinkDSMDLRBlock_dsm_up(demand_dsm_3_2)
+-1 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_1_2)
+-1 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_3_2)
 +1 SinkDSMDLRBlock_dsm_up_level(demand_dsm_1)
 -1 SinkDSMDLRBlock_dsm_up_level(demand_dsm_2)
 = 0
 
 c_u_SinkDSMDLRBlock_dr_storage_limit_red(demand_dsm_0)_:
 +1 SinkDSMDLRBlock_dsm_do_level(demand_dsm_0)
 <= 0.5
@@ -276,83 +274,80 @@
 <= 0.5
 
 c_u_SinkDSMDLRBlock_dr_storage_limit_inc(demand_dsm_2)_:
 +1 SinkDSMDLRBlock_dsm_up_level(demand_dsm_2)
 <= 0.5
 
 c_u_SinkDSMDLRBlock_dr_logical_constraint(demand_dsm_0)_:
-+1 SinkDSMDLRBlock_balance_dsm_do(demand_dsm_1_0)
-+1 SinkDSMDLRBlock_balance_dsm_do(demand_dsm_2_0)
-+1 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_1_0)
-+1 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_2_0)
-+1 SinkDSMDLRBlock_dsm_do_shed(demand_dsm_0)
 +1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_1_0)
-+1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_2_0)
++1 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_1_0)
++1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_3_0)
++1 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_3_0)
 +1 SinkDSMDLRBlock_dsm_up(demand_dsm_1_0)
-+1 SinkDSMDLRBlock_dsm_up(demand_dsm_2_0)
++1 SinkDSMDLRBlock_balance_dsm_do(demand_dsm_1_0)
++1 SinkDSMDLRBlock_dsm_up(demand_dsm_3_0)
++1 SinkDSMDLRBlock_balance_dsm_do(demand_dsm_3_0)
++1 SinkDSMDLRBlock_dsm_do_shed(demand_dsm_0)
 <= 0.5
 
 c_u_SinkDSMDLRBlock_dr_logical_constraint(demand_dsm_1)_:
++1 SinkDSMDLRBlock_dsm_up(demand_dsm_1_1)
 +1 SinkDSMDLRBlock_balance_dsm_do(demand_dsm_1_1)
-+1 SinkDSMDLRBlock_balance_dsm_do(demand_dsm_2_1)
++1 SinkDSMDLRBlock_dsm_up(demand_dsm_3_1)
++1 SinkDSMDLRBlock_balance_dsm_do(demand_dsm_3_1)
++1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_1_1)
 +1 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_1_1)
-+1 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_2_1)
++1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_3_1)
++1 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_3_1)
 +1 SinkDSMDLRBlock_dsm_do_shed(demand_dsm_1)
-+1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_1_1)
-+1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_2_1)
-+1 SinkDSMDLRBlock_dsm_up(demand_dsm_1_1)
-+1 SinkDSMDLRBlock_dsm_up(demand_dsm_2_1)
 <= 0.5
 
 c_u_SinkDSMDLRBlock_dr_logical_constraint(demand_dsm_2)_:
++1 SinkDSMDLRBlock_dsm_up(demand_dsm_1_2)
 +1 SinkDSMDLRBlock_balance_dsm_do(demand_dsm_1_2)
-+1 SinkDSMDLRBlock_balance_dsm_do(demand_dsm_2_2)
++1 SinkDSMDLRBlock_dsm_up(demand_dsm_3_2)
++1 SinkDSMDLRBlock_balance_dsm_do(demand_dsm_3_2)
++1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_1_2)
 +1 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_1_2)
-+1 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_2_2)
++1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_3_2)
++1 SinkDSMDLRBlock_balance_dsm_up(demand_dsm_3_2)
 +1 SinkDSMDLRBlock_dsm_do_shed(demand_dsm_2)
-+1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_1_2)
-+1 SinkDSMDLRBlock_dsm_do_shift(demand_dsm_2_2)
-+1 SinkDSMDLRBlock_dsm_up(demand_dsm_1_2)
-+1 SinkDSMDLRBlock_dsm_up(demand_dsm_2_2)
 <= 0.5
 
-c_e_ONE_VAR_CONSTANT:
-ONE_VAR_CONSTANT = 1.0
-
 bounds
-   0 <= flow(bus_elec_demand_dsm_0) <= +inf
-   0 <= flow(bus_elec_demand_dsm_1) <= +inf
-   0 <= flow(bus_elec_demand_dsm_2) <= +inf
    0 <= SinkDSMDLRBlock_dsm_do_shift(demand_dsm_1_0) <= +inf
-   0 <= SinkDSMDLRBlock_dsm_do_shift(demand_dsm_1_1) <= +inf
-   0 <= SinkDSMDLRBlock_dsm_do_shift(demand_dsm_1_2) <= +inf
-   0 <= SinkDSMDLRBlock_dsm_do_shift(demand_dsm_2_0) <= +inf
-   0 <= SinkDSMDLRBlock_dsm_do_shift(demand_dsm_2_1) <= +inf
-   0 <= SinkDSMDLRBlock_dsm_do_shift(demand_dsm_2_2) <= +inf
-   0 <= SinkDSMDLRBlock_dsm_do_shed(demand_dsm_0) <= +inf
-   0 <= SinkDSMDLRBlock_dsm_do_shed(demand_dsm_1) <= +inf
-   0 <= SinkDSMDLRBlock_dsm_do_shed(demand_dsm_2) <= +inf
+   0 <= SinkDSMDLRBlock_balance_dsm_up(demand_dsm_1_0) <= +inf
+   0 <= SinkDSMDLRBlock_dsm_do_shift(demand_dsm_3_0) <= +inf
+   0 <= SinkDSMDLRBlock_balance_dsm_up(demand_dsm_3_0) <= +inf
    0 <= SinkDSMDLRBlock_dsm_up(demand_dsm_1_0) <= +inf
-   0 <= SinkDSMDLRBlock_dsm_up(demand_dsm_1_1) <= +inf
-   0 <= SinkDSMDLRBlock_dsm_up(demand_dsm_1_2) <= +inf
-   0 <= SinkDSMDLRBlock_dsm_up(demand_dsm_2_0) <= +inf
-   0 <= SinkDSMDLRBlock_dsm_up(demand_dsm_2_1) <= +inf
-   0 <= SinkDSMDLRBlock_dsm_up(demand_dsm_2_2) <= +inf
    0 <= SinkDSMDLRBlock_balance_dsm_do(demand_dsm_1_0) <= +inf
+   0 <= SinkDSMDLRBlock_dsm_up(demand_dsm_3_0) <= +inf
+   0 <= SinkDSMDLRBlock_balance_dsm_do(demand_dsm_3_0) <= +inf
+   0 <= SinkDSMDLRBlock_dsm_up(demand_dsm_1_1) <= +inf
    0 <= SinkDSMDLRBlock_balance_dsm_do(demand_dsm_1_1) <= +inf
-   0 <= SinkDSMDLRBlock_balance_dsm_do(demand_dsm_1_2) <= +inf
-   0 <= SinkDSMDLRBlock_balance_dsm_do(demand_dsm_2_0) <= +inf
-   0 <= SinkDSMDLRBlock_balance_dsm_do(demand_dsm_2_1) <= +inf
-   0 <= SinkDSMDLRBlock_balance_dsm_do(demand_dsm_2_2) <= +inf
-   0 <= SinkDSMDLRBlock_balance_dsm_up(demand_dsm_1_0) <= +inf
+   0 <= SinkDSMDLRBlock_dsm_up(demand_dsm_3_1) <= +inf
+   0 <= SinkDSMDLRBlock_balance_dsm_do(demand_dsm_3_1) <= +inf
+   0 <= SinkDSMDLRBlock_dsm_do_shift(demand_dsm_1_1) <= +inf
    0 <= SinkDSMDLRBlock_balance_dsm_up(demand_dsm_1_1) <= +inf
+   0 <= SinkDSMDLRBlock_dsm_do_shift(demand_dsm_3_1) <= +inf
+   0 <= SinkDSMDLRBlock_balance_dsm_up(demand_dsm_3_1) <= +inf
+   0 <= SinkDSMDLRBlock_dsm_up(demand_dsm_1_2) <= +inf
+   0 <= SinkDSMDLRBlock_balance_dsm_do(demand_dsm_1_2) <= +inf
+   0 <= SinkDSMDLRBlock_dsm_up(demand_dsm_3_2) <= +inf
+   0 <= SinkDSMDLRBlock_balance_dsm_do(demand_dsm_3_2) <= +inf
+   0 <= SinkDSMDLRBlock_dsm_do_shift(demand_dsm_1_2) <= +inf
    0 <= SinkDSMDLRBlock_balance_dsm_up(demand_dsm_1_2) <= +inf
-   0 <= SinkDSMDLRBlock_balance_dsm_up(demand_dsm_2_0) <= +inf
-   0 <= SinkDSMDLRBlock_balance_dsm_up(demand_dsm_2_1) <= +inf
-   0 <= SinkDSMDLRBlock_balance_dsm_up(demand_dsm_2_2) <= +inf
+   0 <= SinkDSMDLRBlock_dsm_do_shift(demand_dsm_3_2) <= +inf
+   0 <= SinkDSMDLRBlock_balance_dsm_up(demand_dsm_3_2) <= +inf
+   0 <= flow(bus_elec_demand_dsm_0_0) <= +inf
+   0 <= flow(bus_elec_demand_dsm_0_1) <= +inf
+   0 <= flow(bus_elec_demand_dsm_0_2) <= +inf
+   0 <= SinkDSMDLRBlock_dsm_do_shed(demand_dsm_0) <= +inf
+   0 <= SinkDSMDLRBlock_dsm_do_shed(demand_dsm_1) <= +inf
+   0 <= SinkDSMDLRBlock_dsm_do_shed(demand_dsm_2) <= +inf
    0 <= SinkDSMDLRBlock_dsm_do_level(demand_dsm_0) <= +inf
    0 <= SinkDSMDLRBlock_dsm_do_level(demand_dsm_1) <= +inf
    0 <= SinkDSMDLRBlock_dsm_do_level(demand_dsm_2) <= +inf
    0 <= SinkDSMDLRBlock_dsm_up_level(demand_dsm_0) <= +inf
    0 <= SinkDSMDLRBlock_dsm_up_level(demand_dsm_1) <= +inf
    0 <= SinkDSMDLRBlock_dsm_up_level(demand_dsm_2) <= +inf
 end
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/dsm_module_DLR_invest.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/dsm_module_DLR_invest.lp`

 * *Files 6% similar despite different names*

```diff
@@ -1,148 +1,141 @@
 \* Source Pyomo model name=Model *\
 
-min
+min 
 objective:
-+2 SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_1_0)
-+2 SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_1_1)
-+2 SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_1_2)
-+2 SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_2_0)
-+2 SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_2_1)
-+2 SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_2_2)
-+2 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_1_0)
-+2 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_1_1)
-+2 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_1_2)
-+2 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_2_0)
-+2 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_2_1)
-+2 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_2_2)
++1 SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_1_0)
++1 SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_1_0)
++1 SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_2_0)
++1 SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_2_0)
++1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_1_0)
++1 SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_1_0)
++1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_2_0)
++1 SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_2_0)
++100 SinkDSMDLRInvestmentBlock_dsm_do_shed(demand_dsm_0)
++1 SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_1_1)
++1 SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_1_1)
++1 SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_2_1)
++1 SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_2_1)
++1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_1_1)
++1 SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_1_1)
++1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_2_1)
++1 SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_2_1)
++100 SinkDSMDLRInvestmentBlock_dsm_do_shed(demand_dsm_1)
++1 SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_1_2)
++1 SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_1_2)
++1 SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_2_2)
++1 SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_2_2)
++1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_1_2)
++1 SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_1_2)
++1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_2_2)
++1 SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_2_2)
++100 SinkDSMDLRInvestmentBlock_dsm_do_shed(demand_dsm_2)
 
 s.t.
 
-c_e_BusBlock_balance(bus_elec_0)_:
-+1 flow(bus_elec_demand_dsm_0)
+c_e_BusBlock_balance(bus_elec_0_0)_:
++1 flow(bus_elec_demand_dsm_0_0)
 = 0
 
-c_e_BusBlock_balance(bus_elec_1)_:
-+1 flow(bus_elec_demand_dsm_1)
+c_e_BusBlock_balance(bus_elec_0_1)_:
++1 flow(bus_elec_demand_dsm_0_1)
 = 0
 
-c_e_BusBlock_balance(bus_elec_2)_:
-+1 flow(bus_elec_demand_dsm_2)
+c_e_BusBlock_balance(bus_elec_0_2)_:
++1 flow(bus_elec_demand_dsm_0_2)
 = 0
 
-c_e_SinkDSMDLRInvestmentBlock_shift_shed_vars(demand_dsm_1_0)_:
-+1 SinkDSMDLRInvestmentBlock_dsm_do_shed(demand_dsm_0)
-= 0
-
-c_e_SinkDSMDLRInvestmentBlock_shift_shed_vars(demand_dsm_1_1)_:
-+1 SinkDSMDLRInvestmentBlock_dsm_do_shed(demand_dsm_1)
-= 0
-
-c_e_SinkDSMDLRInvestmentBlock_shift_shed_vars(demand_dsm_1_2)_:
-+1 SinkDSMDLRInvestmentBlock_dsm_do_shed(demand_dsm_2)
-= 0
-
-c_e_SinkDSMDLRInvestmentBlock_shift_shed_vars(demand_dsm_2_0)_:
-+1 SinkDSMDLRInvestmentBlock_dsm_do_shed(demand_dsm_0)
-= 0
-
-c_e_SinkDSMDLRInvestmentBlock_shift_shed_vars(demand_dsm_2_1)_:
-+1 SinkDSMDLRInvestmentBlock_dsm_do_shed(demand_dsm_1)
-= 0
-
-c_e_SinkDSMDLRInvestmentBlock_shift_shed_vars(demand_dsm_2_2)_:
-+1 SinkDSMDLRInvestmentBlock_dsm_do_shed(demand_dsm_2)
-= 0
+c_e_SinkDSMDLRInvestmentBlock_total_dsm_rule(demand_dsm_0)_:
++1 SinkDSMDLRInvestmentBlock_total(demand_dsm_0)
+-1 SinkDSMDLRInvestmentBlock_invest(demand_dsm_0)
+= 50
 
-c_e_SinkDSMDLRInvestmentBlock_input_output_relation(demand_dsm_0)_:
+c_e_SinkDSMDLRInvestmentBlock_input_output_relation(demand_dsm_0_0)_:
+-1 SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_1_0)
 -1 SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_1_0)
+-1 SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_2_0)
 -1 SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_2_0)
++1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_1_0)
 +1 SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_1_0)
++1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_2_0)
 +1 SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_2_0)
 +1 SinkDSMDLRInvestmentBlock_dsm_do_shed(demand_dsm_0)
-+1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_1_0)
-+1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_2_0)
--1 SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_1_0)
--1 SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_2_0)
--1 SinkDSMDLRInvestmentBlock_invest(demand_dsm)
-+1 flow(bus_elec_demand_dsm_0)
-= 50
++1 flow(bus_elec_demand_dsm_0_0)
+= 1
 
-c_e_SinkDSMDLRInvestmentBlock_input_output_relation(demand_dsm_1)_:
+c_e_SinkDSMDLRInvestmentBlock_input_output_relation(demand_dsm_0_1)_:
+-1 SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_1_1)
 -1 SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_1_1)
+-1 SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_2_1)
 -1 SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_2_1)
++1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_1_1)
 +1 SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_1_1)
++1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_2_1)
 +1 SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_2_1)
 +1 SinkDSMDLRInvestmentBlock_dsm_do_shed(demand_dsm_1)
-+1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_1_1)
-+1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_2_1)
--1 SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_1_1)
--1 SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_2_1)
--1 SinkDSMDLRInvestmentBlock_invest(demand_dsm)
-+1 flow(bus_elec_demand_dsm_1)
-= 50
++1 flow(bus_elec_demand_dsm_0_1)
+= 1
 
-c_e_SinkDSMDLRInvestmentBlock_input_output_relation(demand_dsm_2)_:
+c_e_SinkDSMDLRInvestmentBlock_input_output_relation(demand_dsm_0_2)_:
+-1 SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_1_2)
 -1 SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_1_2)
+-1 SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_2_2)
 -1 SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_2_2)
++1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_1_2)
 +1 SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_1_2)
++1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_2_2)
 +1 SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_2_2)
 +1 SinkDSMDLRInvestmentBlock_dsm_do_shed(demand_dsm_2)
-+1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_1_2)
-+1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_2_2)
--1 SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_1_2)
--1 SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_2_2)
--1 SinkDSMDLRInvestmentBlock_invest(demand_dsm)
-+1 flow(bus_elec_demand_dsm_2)
-= 50
++1 flow(bus_elec_demand_dsm_0_2)
+= 1
 
 c_e_SinkDSMDLRInvestmentBlock_capacity_balance_red(demand_dsm_1_0)_:
 +1 SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_1_0)
 = 0
 
 c_e_SinkDSMDLRInvestmentBlock_capacity_balance_red(demand_dsm_1_1)_:
-+1 SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_1_1)
 -1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_1_0)
++1 SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_1_1)
 = 0
 
 c_e_SinkDSMDLRInvestmentBlock_capacity_balance_red(demand_dsm_1_2)_:
-+1 SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_1_2)
 -1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_1_1)
++1 SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_1_2)
 = 0
 
 c_e_SinkDSMDLRInvestmentBlock_capacity_balance_red(demand_dsm_2_0)_:
 +1 SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_2_0)
 = 0
 
 c_e_SinkDSMDLRInvestmentBlock_capacity_balance_red(demand_dsm_2_2)_:
-+1 SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_2_2)
 -1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_2_0)
++1 SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_2_2)
 = 0
 
 c_e_SinkDSMDLRInvestmentBlock_capacity_balance_inc(demand_dsm_1_0)_:
 +1 SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_1_0)
 = 0
 
 c_e_SinkDSMDLRInvestmentBlock_capacity_balance_inc(demand_dsm_1_1)_:
-+1 SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_1_1)
 -1 SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_1_0)
++1 SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_1_1)
 = 0
 
 c_e_SinkDSMDLRInvestmentBlock_capacity_balance_inc(demand_dsm_1_2)_:
-+1 SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_1_2)
 -1 SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_1_1)
++1 SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_1_2)
 = 0
 
 c_e_SinkDSMDLRInvestmentBlock_capacity_balance_inc(demand_dsm_2_0)_:
 +1 SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_2_0)
 = 0
 
 c_e_SinkDSMDLRInvestmentBlock_capacity_balance_inc(demand_dsm_2_2)_:
-+1 SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_2_2)
 -1 SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_2_0)
++1 SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_2_2)
 = 0
 
 c_e_SinkDSMDLRInvestmentBlock_no_comp_red(demand_dsm_1_2)_:
 +1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_1_2)
 = 0
 
 c_e_SinkDSMDLRInvestmentBlock_no_comp_red(demand_dsm_2_1)_:
@@ -161,217 +154,222 @@
 +1 SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_2_1)
 = 0
 
 c_e_SinkDSMDLRInvestmentBlock_no_comp_inc(demand_dsm_2_2)_:
 +1 SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_2_2)
 = 0
 
-c_u_SinkDSMDLRInvestmentBlock_availability_red(demand_dsm_0)_:
+c_u_SinkDSMDLRInvestmentBlock_availability_red(demand_dsm_0_0)_:
++1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_1_0)
 +1 SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_1_0)
++1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_2_0)
 +1 SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_2_0)
 +1 SinkDSMDLRInvestmentBlock_dsm_do_shed(demand_dsm_0)
-+1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_1_0)
-+1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_2_0)
--0.5 SinkDSMDLRInvestmentBlock_invest(demand_dsm)
-<= 25
+-0.5 SinkDSMDLRInvestmentBlock_total(demand_dsm_0)
+<= 0
 
-c_u_SinkDSMDLRInvestmentBlock_availability_red(demand_dsm_1)_:
+c_u_SinkDSMDLRInvestmentBlock_availability_red(demand_dsm_0_1)_:
++1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_1_1)
 +1 SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_1_1)
++1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_2_1)
 +1 SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_2_1)
 +1 SinkDSMDLRInvestmentBlock_dsm_do_shed(demand_dsm_1)
-+1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_1_1)
-+1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_2_1)
--0.5 SinkDSMDLRInvestmentBlock_invest(demand_dsm)
-<= 25
+-0.5 SinkDSMDLRInvestmentBlock_total(demand_dsm_0)
+<= 0
 
-c_u_SinkDSMDLRInvestmentBlock_availability_red(demand_dsm_2)_:
+c_u_SinkDSMDLRInvestmentBlock_availability_red(demand_dsm_0_2)_:
++1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_1_2)
 +1 SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_1_2)
++1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_2_2)
 +1 SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_2_2)
 +1 SinkDSMDLRInvestmentBlock_dsm_do_shed(demand_dsm_2)
-+1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_1_2)
-+1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_2_2)
--0.5 SinkDSMDLRInvestmentBlock_invest(demand_dsm)
-<= 25
+-0.5 SinkDSMDLRInvestmentBlock_total(demand_dsm_0)
+<= 0
 
-c_u_SinkDSMDLRInvestmentBlock_availability_inc(demand_dsm_0)_:
-+1 SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_1_0)
-+1 SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_2_0)
+c_u_SinkDSMDLRInvestmentBlock_availability_inc(demand_dsm_0_0)_:
 +1 SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_1_0)
++1 SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_1_0)
 +1 SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_2_0)
--0.5 SinkDSMDLRInvestmentBlock_invest(demand_dsm)
-<= 25
++1 SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_2_0)
+-0.5 SinkDSMDLRInvestmentBlock_total(demand_dsm_0)
+<= 0
 
-c_u_SinkDSMDLRInvestmentBlock_availability_inc(demand_dsm_1)_:
-+1 SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_1_1)
-+1 SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_2_1)
+c_u_SinkDSMDLRInvestmentBlock_availability_inc(demand_dsm_0_1)_:
 +1 SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_1_1)
++1 SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_1_1)
 +1 SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_2_1)
--0.5 SinkDSMDLRInvestmentBlock_invest(demand_dsm)
-<= 25
++1 SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_2_1)
+-0.5 SinkDSMDLRInvestmentBlock_total(demand_dsm_0)
+<= 0
 
-c_u_SinkDSMDLRInvestmentBlock_availability_inc(demand_dsm_2)_:
-+1 SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_1_2)
-+1 SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_2_2)
+c_u_SinkDSMDLRInvestmentBlock_availability_inc(demand_dsm_0_2)_:
 +1 SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_1_2)
++1 SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_1_2)
 +1 SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_2_2)
--0.5 SinkDSMDLRInvestmentBlock_invest(demand_dsm)
-<= 25
++1 SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_2_2)
+-0.5 SinkDSMDLRInvestmentBlock_total(demand_dsm_0)
+<= 0
 
 c_e_SinkDSMDLRInvestmentBlock_dr_storage_red(demand_dsm_0)_:
-+1 SinkDSMDLRInvestmentBlock_dsm_do_level(demand_dsm_0)
 -1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_1_0)
 -1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_2_0)
++1 SinkDSMDLRInvestmentBlock_dsm_do_level(demand_dsm_0)
 = 0
 
 c_e_SinkDSMDLRInvestmentBlock_dr_storage_red(demand_dsm_1)_:
 -1 SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_1_1)
 -1 SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_2_1)
-+1 SinkDSMDLRInvestmentBlock_dsm_do_level(demand_dsm_0)
--1 SinkDSMDLRInvestmentBlock_dsm_do_level(demand_dsm_1)
 +1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_1_1)
 +1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_2_1)
++1 SinkDSMDLRInvestmentBlock_dsm_do_level(demand_dsm_0)
+-1 SinkDSMDLRInvestmentBlock_dsm_do_level(demand_dsm_1)
 = 0
 
 c_e_SinkDSMDLRInvestmentBlock_dr_storage_red(demand_dsm_2)_:
 -1 SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_1_2)
 -1 SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_2_2)
-+1 SinkDSMDLRInvestmentBlock_dsm_do_level(demand_dsm_1)
--1 SinkDSMDLRInvestmentBlock_dsm_do_level(demand_dsm_2)
 +1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_1_2)
 +1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_2_2)
++1 SinkDSMDLRInvestmentBlock_dsm_do_level(demand_dsm_1)
+-1 SinkDSMDLRInvestmentBlock_dsm_do_level(demand_dsm_2)
 = 0
 
 c_e_SinkDSMDLRInvestmentBlock_dr_storage_inc(demand_dsm_0)_:
 -1 SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_1_0)
 -1 SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_2_0)
 +1 SinkDSMDLRInvestmentBlock_dsm_up_level(demand_dsm_0)
 = 0
 
 c_e_SinkDSMDLRInvestmentBlock_dr_storage_inc(demand_dsm_1)_:
--1 SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_1_1)
--1 SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_2_1)
 +1 SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_1_1)
 +1 SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_2_1)
+-1 SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_1_1)
+-1 SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_2_1)
 +1 SinkDSMDLRInvestmentBlock_dsm_up_level(demand_dsm_0)
 -1 SinkDSMDLRInvestmentBlock_dsm_up_level(demand_dsm_1)
 = 0
 
 c_e_SinkDSMDLRInvestmentBlock_dr_storage_inc(demand_dsm_2)_:
--1 SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_1_2)
--1 SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_2_2)
 +1 SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_1_2)
 +1 SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_2_2)
+-1 SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_1_2)
+-1 SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_2_2)
 +1 SinkDSMDLRInvestmentBlock_dsm_up_level(demand_dsm_1)
 -1 SinkDSMDLRInvestmentBlock_dsm_up_level(demand_dsm_2)
 = 0
 
-c_u_SinkDSMDLRInvestmentBlock_dr_storage_limit_red(demand_dsm_0)_:
+c_u_SinkDSMDLRInvestmentBlock_dr_storage_limit_red(demand_dsm_0_0)_:
+-0.5 SinkDSMDLRInvestmentBlock_total(demand_dsm_0)
 +1 SinkDSMDLRInvestmentBlock_dsm_do_level(demand_dsm_0)
--0.5 SinkDSMDLRInvestmentBlock_invest(demand_dsm)
-<= 25
+<= 0
 
-c_u_SinkDSMDLRInvestmentBlock_dr_storage_limit_red(demand_dsm_1)_:
+c_u_SinkDSMDLRInvestmentBlock_dr_storage_limit_red(demand_dsm_0_1)_:
+-0.5 SinkDSMDLRInvestmentBlock_total(demand_dsm_0)
 +1 SinkDSMDLRInvestmentBlock_dsm_do_level(demand_dsm_1)
--0.5 SinkDSMDLRInvestmentBlock_invest(demand_dsm)
-<= 25
+<= 0
 
-c_u_SinkDSMDLRInvestmentBlock_dr_storage_limit_red(demand_dsm_2)_:
+c_u_SinkDSMDLRInvestmentBlock_dr_storage_limit_red(demand_dsm_0_2)_:
+-0.5 SinkDSMDLRInvestmentBlock_total(demand_dsm_0)
 +1 SinkDSMDLRInvestmentBlock_dsm_do_level(demand_dsm_2)
--0.5 SinkDSMDLRInvestmentBlock_invest(demand_dsm)
-<= 25
+<= 0
 
-c_u_SinkDSMDLRInvestmentBlock_dr_storage_limit_inc(demand_dsm_0)_:
+c_u_SinkDSMDLRInvestmentBlock_dr_storage_limit_inc(demand_dsm_0_0)_:
+-0.5 SinkDSMDLRInvestmentBlock_total(demand_dsm_0)
 +1 SinkDSMDLRInvestmentBlock_dsm_up_level(demand_dsm_0)
--0.5 SinkDSMDLRInvestmentBlock_invest(demand_dsm)
-<= 25
+<= 0
 
-c_u_SinkDSMDLRInvestmentBlock_dr_storage_limit_inc(demand_dsm_1)_:
+c_u_SinkDSMDLRInvestmentBlock_dr_storage_limit_inc(demand_dsm_0_1)_:
+-0.5 SinkDSMDLRInvestmentBlock_total(demand_dsm_0)
 +1 SinkDSMDLRInvestmentBlock_dsm_up_level(demand_dsm_1)
--0.5 SinkDSMDLRInvestmentBlock_invest(demand_dsm)
-<= 25
+<= 0
 
-c_u_SinkDSMDLRInvestmentBlock_dr_storage_limit_inc(demand_dsm_2)_:
+c_u_SinkDSMDLRInvestmentBlock_dr_storage_limit_inc(demand_dsm_0_2)_:
+-0.5 SinkDSMDLRInvestmentBlock_total(demand_dsm_0)
 +1 SinkDSMDLRInvestmentBlock_dsm_up_level(demand_dsm_2)
--0.5 SinkDSMDLRInvestmentBlock_invest(demand_dsm)
-<= 25
+<= 0
+
+c_u_SinkDSMDLRInvestmentBlock_dr_yearly_limit_shed(demand_dsm_0)_:
++1 SinkDSMDLRInvestmentBlock_dsm_do_shed(demand_dsm_0)
++1 SinkDSMDLRInvestmentBlock_dsm_do_shed(demand_dsm_1)
++1 SinkDSMDLRInvestmentBlock_dsm_do_shed(demand_dsm_2)
+-50.0 SinkDSMDLRInvestmentBlock_total(demand_dsm_0)
+<= 0
 
-c_u_SinkDSMDLRInvestmentBlock_dr_logical_constraint(demand_dsm_0)_:
+c_u_SinkDSMDLRInvestmentBlock_dr_logical_constraint(demand_dsm_0_0)_:
++1 SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_1_0)
 +1 SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_1_0)
++1 SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_2_0)
 +1 SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_2_0)
++1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_1_0)
 +1 SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_1_0)
++1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_2_0)
 +1 SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_2_0)
 +1 SinkDSMDLRInvestmentBlock_dsm_do_shed(demand_dsm_0)
-+1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_1_0)
-+1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_2_0)
-+1 SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_1_0)
-+1 SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_2_0)
--0.5 SinkDSMDLRInvestmentBlock_invest(demand_dsm)
-<= 25
+-0.5 SinkDSMDLRInvestmentBlock_total(demand_dsm_0)
+<= 0
 
-c_u_SinkDSMDLRInvestmentBlock_dr_logical_constraint(demand_dsm_1)_:
+c_u_SinkDSMDLRInvestmentBlock_dr_logical_constraint(demand_dsm_0_1)_:
++1 SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_1_1)
 +1 SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_1_1)
++1 SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_2_1)
 +1 SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_2_1)
++1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_1_1)
 +1 SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_1_1)
++1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_2_1)
 +1 SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_2_1)
 +1 SinkDSMDLRInvestmentBlock_dsm_do_shed(demand_dsm_1)
-+1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_1_1)
-+1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_2_1)
-+1 SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_1_1)
-+1 SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_2_1)
--0.5 SinkDSMDLRInvestmentBlock_invest(demand_dsm)
-<= 25
+-0.5 SinkDSMDLRInvestmentBlock_total(demand_dsm_0)
+<= 0
 
-c_u_SinkDSMDLRInvestmentBlock_dr_logical_constraint(demand_dsm_2)_:
+c_u_SinkDSMDLRInvestmentBlock_dr_logical_constraint(demand_dsm_0_2)_:
++1 SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_1_2)
 +1 SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_1_2)
++1 SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_2_2)
 +1 SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_2_2)
++1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_1_2)
 +1 SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_1_2)
++1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_2_2)
 +1 SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_2_2)
 +1 SinkDSMDLRInvestmentBlock_dsm_do_shed(demand_dsm_2)
-+1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_1_2)
-+1 SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_2_2)
-+1 SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_1_2)
-+1 SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_2_2)
--0.5 SinkDSMDLRInvestmentBlock_invest(demand_dsm)
-<= 25
-
-c_e_ONE_VAR_CONSTANT:
-ONE_VAR_CONSTANT = 1.0
+-0.5 SinkDSMDLRInvestmentBlock_total(demand_dsm_0)
+<= 0
 
 bounds
-   0 <= flow(bus_elec_demand_dsm_0) <= +inf
-   0 <= flow(bus_elec_demand_dsm_1) <= +inf
-   0 <= flow(bus_elec_demand_dsm_2) <= +inf
-   33 <= SinkDSMDLRInvestmentBlock_invest(demand_dsm) <= 100
+   0 <= SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_1_0) <= +inf
+   0 <= SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_1_0) <= +inf
+   0 <= SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_2_0) <= +inf
+   0 <= SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_2_0) <= +inf
    0 <= SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_1_0) <= +inf
-   0 <= SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_1_1) <= +inf
-   0 <= SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_1_2) <= +inf
+   0 <= SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_1_0) <= +inf
    0 <= SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_2_0) <= +inf
-   0 <= SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_2_1) <= +inf
-   0 <= SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_2_2) <= +inf
+   0 <= SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_2_0) <= +inf
    0 <= SinkDSMDLRInvestmentBlock_dsm_do_shed(demand_dsm_0) <= +inf
-   0 <= SinkDSMDLRInvestmentBlock_dsm_do_shed(demand_dsm_1) <= +inf
-   0 <= SinkDSMDLRInvestmentBlock_dsm_do_shed(demand_dsm_2) <= +inf
-   0 <= SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_1_0) <= +inf
    0 <= SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_1_1) <= +inf
-   0 <= SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_1_2) <= +inf
-   0 <= SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_2_0) <= +inf
-   0 <= SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_2_1) <= +inf
-   0 <= SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_2_2) <= +inf
-   0 <= SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_1_0) <= +inf
    0 <= SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_1_1) <= +inf
-   0 <= SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_1_2) <= +inf
-   0 <= SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_2_0) <= +inf
+   0 <= SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_2_1) <= +inf
    0 <= SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_2_1) <= +inf
-   0 <= SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_2_2) <= +inf
-   0 <= SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_1_0) <= +inf
+   0 <= SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_1_1) <= +inf
    0 <= SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_1_1) <= +inf
-   0 <= SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_1_2) <= +inf
-   0 <= SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_2_0) <= +inf
+   0 <= SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_2_1) <= +inf
    0 <= SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_2_1) <= +inf
+   0 <= SinkDSMDLRInvestmentBlock_dsm_do_shed(demand_dsm_1) <= +inf
+   0 <= SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_1_2) <= +inf
+   0 <= SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_1_2) <= +inf
+   0 <= SinkDSMDLRInvestmentBlock_dsm_up(demand_dsm_2_2) <= +inf
+   0 <= SinkDSMDLRInvestmentBlock_balance_dsm_do(demand_dsm_2_2) <= +inf
+   0 <= SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_1_2) <= +inf
+   0 <= SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_1_2) <= +inf
+   0 <= SinkDSMDLRInvestmentBlock_dsm_do_shift(demand_dsm_2_2) <= +inf
    0 <= SinkDSMDLRInvestmentBlock_balance_dsm_up(demand_dsm_2_2) <= +inf
+   0 <= SinkDSMDLRInvestmentBlock_dsm_do_shed(demand_dsm_2) <= +inf
+   0 <= flow(bus_elec_demand_dsm_0_0) <= +inf
+   0 <= flow(bus_elec_demand_dsm_0_1) <= +inf
+   0 <= flow(bus_elec_demand_dsm_0_2) <= +inf
+   0 <= SinkDSMDLRInvestmentBlock_total(demand_dsm_0) <= +inf
+   33 <= SinkDSMDLRInvestmentBlock_invest(demand_dsm_0) <= 100
    0 <= SinkDSMDLRInvestmentBlock_dsm_do_level(demand_dsm_0) <= +inf
    0 <= SinkDSMDLRInvestmentBlock_dsm_do_level(demand_dsm_1) <= +inf
    0 <= SinkDSMDLRInvestmentBlock_dsm_do_level(demand_dsm_2) <= +inf
    0 <= SinkDSMDLRInvestmentBlock_dsm_up_level(demand_dsm_0) <= +inf
    0 <= SinkDSMDLRInvestmentBlock_dsm_up_level(demand_dsm_1) <= +inf
    0 <= SinkDSMDLRInvestmentBlock_dsm_up_level(demand_dsm_2) <= +inf
 end
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/dsm_module_oemof.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/dsm_module_oemof.lp`

 * *Files 3% similar despite different names*

```diff
@@ -1,106 +1,103 @@
 \* Source Pyomo model name=Model *\
 
-min
+min 
 objective:
 +2 SinkDSMOemofBlock_dsm_do_shift(demand_dsm_0)
 +2 SinkDSMOemofBlock_dsm_do_shift(demand_dsm_1)
 +2 SinkDSMOemofBlock_dsm_do_shift(demand_dsm_2)
 
 s.t.
 
-c_e_BusBlock_balance(bus_elec_0)_:
-+1 flow(bus_elec_demand_dsm_0)
+c_e_BusBlock_balance(bus_elec_0_0)_:
++1 flow(bus_elec_demand_dsm_0_0)
 = 0
 
-c_e_BusBlock_balance(bus_elec_1)_:
-+1 flow(bus_elec_demand_dsm_1)
+c_e_BusBlock_balance(bus_elec_0_1)_:
++1 flow(bus_elec_demand_dsm_0_1)
 = 0
 
-c_e_BusBlock_balance(bus_elec_2)_:
-+1 flow(bus_elec_demand_dsm_2)
+c_e_BusBlock_balance(bus_elec_0_2)_:
++1 flow(bus_elec_demand_dsm_0_2)
 = 0
 
 c_e_SinkDSMOemofBlock_shift_shed_vars(demand_dsm_0)_:
 +1 SinkDSMOemofBlock_dsm_do_shed(demand_dsm_0)
 = 0
 
 c_e_SinkDSMOemofBlock_shift_shed_vars(demand_dsm_1)_:
 +1 SinkDSMOemofBlock_dsm_do_shed(demand_dsm_1)
 = 0
 
 c_e_SinkDSMOemofBlock_shift_shed_vars(demand_dsm_2)_:
 +1 SinkDSMOemofBlock_dsm_do_shed(demand_dsm_2)
 = 0
 
-c_e_SinkDSMOemofBlock_input_output_relation(demand_dsm_0)_:
-+1 SinkDSMOemofBlock_dsm_do_shed(demand_dsm_0)
+c_e_SinkDSMOemofBlock_input_output_relation(demand_dsm_0_0)_:
 +1 SinkDSMOemofBlock_dsm_do_shift(demand_dsm_0)
++1 flow(bus_elec_demand_dsm_0_0)
++1 SinkDSMOemofBlock_dsm_do_shed(demand_dsm_0)
 -1 SinkDSMOemofBlock_dsm_up(demand_dsm_0)
-+1 flow(bus_elec_demand_dsm_0)
 = 1
 
-c_e_SinkDSMOemofBlock_input_output_relation(demand_dsm_1)_:
-+1 SinkDSMOemofBlock_dsm_do_shed(demand_dsm_1)
+c_e_SinkDSMOemofBlock_input_output_relation(demand_dsm_0_1)_:
 +1 SinkDSMOemofBlock_dsm_do_shift(demand_dsm_1)
++1 flow(bus_elec_demand_dsm_0_1)
++1 SinkDSMOemofBlock_dsm_do_shed(demand_dsm_1)
 -1 SinkDSMOemofBlock_dsm_up(demand_dsm_1)
-+1 flow(bus_elec_demand_dsm_1)
 = 1
 
-c_e_SinkDSMOemofBlock_input_output_relation(demand_dsm_2)_:
-+1 SinkDSMOemofBlock_dsm_do_shed(demand_dsm_2)
+c_e_SinkDSMOemofBlock_input_output_relation(demand_dsm_0_2)_:
 +1 SinkDSMOemofBlock_dsm_do_shift(demand_dsm_2)
++1 flow(bus_elec_demand_dsm_0_2)
++1 SinkDSMOemofBlock_dsm_do_shed(demand_dsm_2)
 -1 SinkDSMOemofBlock_dsm_up(demand_dsm_2)
-+1 flow(bus_elec_demand_dsm_2)
 = 1
 
 c_u_SinkDSMOemofBlock_dsm_up_constraint(demand_dsm_0)_:
 +1 SinkDSMOemofBlock_dsm_up(demand_dsm_0)
 <= 0.5
 
 c_u_SinkDSMOemofBlock_dsm_up_constraint(demand_dsm_1)_:
 +1 SinkDSMOemofBlock_dsm_up(demand_dsm_1)
-<= 0.40000000000000002
+<= 0.4
 
 c_u_SinkDSMOemofBlock_dsm_up_constraint(demand_dsm_2)_:
 +1 SinkDSMOemofBlock_dsm_up(demand_dsm_2)
 <= 0.5
 
 c_u_SinkDSMOemofBlock_dsm_down_constraint(demand_dsm_0)_:
-+1 SinkDSMOemofBlock_dsm_do_shed(demand_dsm_0)
 +1 SinkDSMOemofBlock_dsm_do_shift(demand_dsm_0)
++1 SinkDSMOemofBlock_dsm_do_shed(demand_dsm_0)
 <= 0.5
 
 c_u_SinkDSMOemofBlock_dsm_down_constraint(demand_dsm_1)_:
-+1 SinkDSMOemofBlock_dsm_do_shed(demand_dsm_1)
 +1 SinkDSMOemofBlock_dsm_do_shift(demand_dsm_1)
-<= 0.40000000000000002
++1 SinkDSMOemofBlock_dsm_do_shed(demand_dsm_1)
+<= 0.4
 
 c_u_SinkDSMOemofBlock_dsm_down_constraint(demand_dsm_2)_:
-+1 SinkDSMOemofBlock_dsm_do_shed(demand_dsm_2)
 +1 SinkDSMOemofBlock_dsm_do_shift(demand_dsm_2)
++1 SinkDSMOemofBlock_dsm_do_shed(demand_dsm_2)
 <= 0.5
 
 c_e_SinkDSMOemofBlock_dsm_sum_constraint(demand_dsm_0)_:
 -1 SinkDSMOemofBlock_dsm_do_shift(demand_dsm_0)
 -1 SinkDSMOemofBlock_dsm_do_shift(demand_dsm_1)
 +1 SinkDSMOemofBlock_dsm_up(demand_dsm_0)
 +1 SinkDSMOemofBlock_dsm_up(demand_dsm_1)
 = 0
 
-c_e_ONE_VAR_CONSTANT:
-ONE_VAR_CONSTANT = 1.0
-
 bounds
-   0 <= flow(bus_elec_demand_dsm_0) <= +inf
-   0 <= flow(bus_elec_demand_dsm_1) <= +inf
-   0 <= flow(bus_elec_demand_dsm_2) <= +inf
    0 <= SinkDSMOemofBlock_dsm_do_shift(demand_dsm_0) <= +inf
    0 <= SinkDSMOemofBlock_dsm_do_shift(demand_dsm_1) <= +inf
    0 <= SinkDSMOemofBlock_dsm_do_shift(demand_dsm_2) <= +inf
+   0 <= flow(bus_elec_demand_dsm_0_0) <= +inf
+   0 <= flow(bus_elec_demand_dsm_0_1) <= +inf
+   0 <= flow(bus_elec_demand_dsm_0_2) <= +inf
    0 <= SinkDSMOemofBlock_dsm_do_shed(demand_dsm_0) <= +inf
    0 <= SinkDSMOemofBlock_dsm_do_shed(demand_dsm_1) <= +inf
    0 <= SinkDSMOemofBlock_dsm_do_shed(demand_dsm_2) <= +inf
    0 <= SinkDSMOemofBlock_dsm_up(demand_dsm_0) <= +inf
    0 <= SinkDSMOemofBlock_dsm_up(demand_dsm_1) <= +inf
    0 <= SinkDSMOemofBlock_dsm_up(demand_dsm_2) <= +inf
 end
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/dsm_module_oemof_invest.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/dsm_module_oemof_invest.lp`

 * *Files 5% similar despite different names*

```diff
@@ -1,116 +1,110 @@
 \* Source Pyomo model name=Model *\
 
-min
+min 
 objective:
-+2 SinkDSMOemofInvestmentBlock_dsm_do_shift(demand_dsm_0)
-+2 SinkDSMOemofInvestmentBlock_dsm_do_shift(demand_dsm_1)
-+2 SinkDSMOemofInvestmentBlock_dsm_do_shift(demand_dsm_2)
++1 SinkDSMOemofInvestmentBlock_dsm_do_shift(demand_dsm_0)
++100 SinkDSMOemofInvestmentBlock_dsm_do_shed(demand_dsm_0)
++1 SinkDSMOemofInvestmentBlock_dsm_up(demand_dsm_0)
++1 SinkDSMOemofInvestmentBlock_dsm_up(demand_dsm_1)
++1 SinkDSMOemofInvestmentBlock_dsm_do_shift(demand_dsm_1)
++100 SinkDSMOemofInvestmentBlock_dsm_do_shed(demand_dsm_1)
++1 SinkDSMOemofInvestmentBlock_dsm_up(demand_dsm_2)
++1 SinkDSMOemofInvestmentBlock_dsm_do_shift(demand_dsm_2)
++100 SinkDSMOemofInvestmentBlock_dsm_do_shed(demand_dsm_2)
 
 s.t.
 
-c_e_BusBlock_balance(bus_elec_0)_:
-+1 flow(bus_elec_demand_dsm_0)
+c_e_BusBlock_balance(bus_elec_0_0)_:
++1 flow(bus_elec_demand_dsm_0_0)
 = 0
 
-c_e_BusBlock_balance(bus_elec_1)_:
-+1 flow(bus_elec_demand_dsm_1)
+c_e_BusBlock_balance(bus_elec_0_1)_:
++1 flow(bus_elec_demand_dsm_0_1)
 = 0
 
-c_e_BusBlock_balance(bus_elec_2)_:
-+1 flow(bus_elec_demand_dsm_2)
-= 0
-
-c_e_SinkDSMOemofInvestmentBlock_shift_shed_vars(demand_dsm_0)_:
-+1 SinkDSMOemofInvestmentBlock_dsm_do_shed(demand_dsm_0)
-= 0
-
-c_e_SinkDSMOemofInvestmentBlock_shift_shed_vars(demand_dsm_1)_:
-+1 SinkDSMOemofInvestmentBlock_dsm_do_shed(demand_dsm_1)
+c_e_BusBlock_balance(bus_elec_0_2)_:
++1 flow(bus_elec_demand_dsm_0_2)
 = 0
 
-c_e_SinkDSMOemofInvestmentBlock_shift_shed_vars(demand_dsm_2)_:
-+1 SinkDSMOemofInvestmentBlock_dsm_do_shed(demand_dsm_2)
-= 0
+c_e_SinkDSMOemofInvestmentBlock_total_dsm_rule(demand_dsm_0)_:
++1 SinkDSMOemofInvestmentBlock_total(demand_dsm_0)
+-1 SinkDSMOemofInvestmentBlock_invest(demand_dsm_0)
+= 50
 
-c_e_SinkDSMOemofInvestmentBlock_input_output_relation(demand_dsm_0)_:
-+1 SinkDSMOemofInvestmentBlock_dsm_do_shed(demand_dsm_0)
+c_e_SinkDSMOemofInvestmentBlock_input_output_relation(demand_dsm_0_0)_:
 +1 SinkDSMOemofInvestmentBlock_dsm_do_shift(demand_dsm_0)
++1 SinkDSMOemofInvestmentBlock_dsm_do_shed(demand_dsm_0)
 -1 SinkDSMOemofInvestmentBlock_dsm_up(demand_dsm_0)
--1 SinkDSMOemofInvestmentBlock_invest(demand_dsm)
-+1 flow(bus_elec_demand_dsm_0)
-= 50
++1 flow(bus_elec_demand_dsm_0_0)
+= 1
 
-c_e_SinkDSMOemofInvestmentBlock_input_output_relation(demand_dsm_1)_:
-+1 SinkDSMOemofInvestmentBlock_dsm_do_shed(demand_dsm_1)
-+1 SinkDSMOemofInvestmentBlock_dsm_do_shift(demand_dsm_1)
+c_e_SinkDSMOemofInvestmentBlock_input_output_relation(demand_dsm_0_1)_:
 -1 SinkDSMOemofInvestmentBlock_dsm_up(demand_dsm_1)
--1 SinkDSMOemofInvestmentBlock_invest(demand_dsm)
-+1 flow(bus_elec_demand_dsm_1)
-= 50
++1 SinkDSMOemofInvestmentBlock_dsm_do_shift(demand_dsm_1)
++1 SinkDSMOemofInvestmentBlock_dsm_do_shed(demand_dsm_1)
++1 flow(bus_elec_demand_dsm_0_1)
+= 1
 
-c_e_SinkDSMOemofInvestmentBlock_input_output_relation(demand_dsm_2)_:
-+1 SinkDSMOemofInvestmentBlock_dsm_do_shed(demand_dsm_2)
-+1 SinkDSMOemofInvestmentBlock_dsm_do_shift(demand_dsm_2)
+c_e_SinkDSMOemofInvestmentBlock_input_output_relation(demand_dsm_0_2)_:
 -1 SinkDSMOemofInvestmentBlock_dsm_up(demand_dsm_2)
--1 SinkDSMOemofInvestmentBlock_invest(demand_dsm)
-+1 flow(bus_elec_demand_dsm_2)
-= 50
++1 SinkDSMOemofInvestmentBlock_dsm_do_shift(demand_dsm_2)
++1 SinkDSMOemofInvestmentBlock_dsm_do_shed(demand_dsm_2)
++1 flow(bus_elec_demand_dsm_0_2)
+= 1
 
-c_u_SinkDSMOemofInvestmentBlock_dsm_up_constraint(demand_dsm_0)_:
+c_u_SinkDSMOemofInvestmentBlock_dsm_up_constraint(demand_dsm_0_0)_:
 +1 SinkDSMOemofInvestmentBlock_dsm_up(demand_dsm_0)
--0.5 SinkDSMOemofInvestmentBlock_invest(demand_dsm)
-<= 25
+-0.5 SinkDSMOemofInvestmentBlock_total(demand_dsm_0)
+<= 0
 
-c_u_SinkDSMOemofInvestmentBlock_dsm_up_constraint(demand_dsm_1)_:
+c_u_SinkDSMOemofInvestmentBlock_dsm_up_constraint(demand_dsm_0_1)_:
 +1 SinkDSMOemofInvestmentBlock_dsm_up(demand_dsm_1)
--0.40000000000000002 SinkDSMOemofInvestmentBlock_invest(demand_dsm)
-<= 20
+-0.4 SinkDSMOemofInvestmentBlock_total(demand_dsm_0)
+<= 0
 
-c_u_SinkDSMOemofInvestmentBlock_dsm_up_constraint(demand_dsm_2)_:
+c_u_SinkDSMOemofInvestmentBlock_dsm_up_constraint(demand_dsm_0_2)_:
 +1 SinkDSMOemofInvestmentBlock_dsm_up(demand_dsm_2)
--0.5 SinkDSMOemofInvestmentBlock_invest(demand_dsm)
-<= 25
+-0.5 SinkDSMOemofInvestmentBlock_total(demand_dsm_0)
+<= 0
 
-c_u_SinkDSMOemofInvestmentBlock_dsm_down_constraint(demand_dsm_0)_:
-+1 SinkDSMOemofInvestmentBlock_dsm_do_shed(demand_dsm_0)
+c_u_SinkDSMOemofInvestmentBlock_dsm_down_constraint(demand_dsm_0_0)_:
 +1 SinkDSMOemofInvestmentBlock_dsm_do_shift(demand_dsm_0)
--0.5 SinkDSMOemofInvestmentBlock_invest(demand_dsm)
-<= 25
++1 SinkDSMOemofInvestmentBlock_dsm_do_shed(demand_dsm_0)
+-0.5 SinkDSMOemofInvestmentBlock_total(demand_dsm_0)
+<= 0
 
-c_u_SinkDSMOemofInvestmentBlock_dsm_down_constraint(demand_dsm_1)_:
-+1 SinkDSMOemofInvestmentBlock_dsm_do_shed(demand_dsm_1)
+c_u_SinkDSMOemofInvestmentBlock_dsm_down_constraint(demand_dsm_0_1)_:
 +1 SinkDSMOemofInvestmentBlock_dsm_do_shift(demand_dsm_1)
--0.40000000000000002 SinkDSMOemofInvestmentBlock_invest(demand_dsm)
-<= 20
++1 SinkDSMOemofInvestmentBlock_dsm_do_shed(demand_dsm_1)
+-0.4 SinkDSMOemofInvestmentBlock_total(demand_dsm_0)
+<= 0
 
-c_u_SinkDSMOemofInvestmentBlock_dsm_down_constraint(demand_dsm_2)_:
-+1 SinkDSMOemofInvestmentBlock_dsm_do_shed(demand_dsm_2)
+c_u_SinkDSMOemofInvestmentBlock_dsm_down_constraint(demand_dsm_0_2)_:
 +1 SinkDSMOemofInvestmentBlock_dsm_do_shift(demand_dsm_2)
--0.5 SinkDSMOemofInvestmentBlock_invest(demand_dsm)
-<= 25
++1 SinkDSMOemofInvestmentBlock_dsm_do_shed(demand_dsm_2)
+-0.5 SinkDSMOemofInvestmentBlock_total(demand_dsm_0)
+<= 0
 
 c_e_SinkDSMOemofInvestmentBlock_dsm_sum_constraint(demand_dsm_0)_:
 -1 SinkDSMOemofInvestmentBlock_dsm_do_shift(demand_dsm_0)
--1 SinkDSMOemofInvestmentBlock_dsm_do_shift(demand_dsm_1)
 +1 SinkDSMOemofInvestmentBlock_dsm_up(demand_dsm_0)
 +1 SinkDSMOemofInvestmentBlock_dsm_up(demand_dsm_1)
+-1 SinkDSMOemofInvestmentBlock_dsm_do_shift(demand_dsm_1)
 = 0
 
-c_e_ONE_VAR_CONSTANT:
-ONE_VAR_CONSTANT = 1.0
-
 bounds
-   0 <= flow(bus_elec_demand_dsm_0) <= +inf
-   0 <= flow(bus_elec_demand_dsm_1) <= +inf
-   0 <= flow(bus_elec_demand_dsm_2) <= +inf
-   33 <= SinkDSMOemofInvestmentBlock_invest(demand_dsm) <= 100
    0 <= SinkDSMOemofInvestmentBlock_dsm_do_shift(demand_dsm_0) <= +inf
-   0 <= SinkDSMOemofInvestmentBlock_dsm_do_shift(demand_dsm_1) <= +inf
-   0 <= SinkDSMOemofInvestmentBlock_dsm_do_shift(demand_dsm_2) <= +inf
    0 <= SinkDSMOemofInvestmentBlock_dsm_do_shed(demand_dsm_0) <= +inf
-   0 <= SinkDSMOemofInvestmentBlock_dsm_do_shed(demand_dsm_1) <= +inf
-   0 <= SinkDSMOemofInvestmentBlock_dsm_do_shed(demand_dsm_2) <= +inf
    0 <= SinkDSMOemofInvestmentBlock_dsm_up(demand_dsm_0) <= +inf
    0 <= SinkDSMOemofInvestmentBlock_dsm_up(demand_dsm_1) <= +inf
+   0 <= SinkDSMOemofInvestmentBlock_dsm_do_shift(demand_dsm_1) <= +inf
+   0 <= SinkDSMOemofInvestmentBlock_dsm_do_shed(demand_dsm_1) <= +inf
    0 <= SinkDSMOemofInvestmentBlock_dsm_up(demand_dsm_2) <= +inf
+   0 <= SinkDSMOemofInvestmentBlock_dsm_do_shift(demand_dsm_2) <= +inf
+   0 <= SinkDSMOemofInvestmentBlock_dsm_do_shed(demand_dsm_2) <= +inf
+   0 <= flow(bus_elec_demand_dsm_0_0) <= +inf
+   0 <= flow(bus_elec_demand_dsm_0_1) <= +inf
+   0 <= flow(bus_elec_demand_dsm_0_2) <= +inf
+   0 <= SinkDSMOemofInvestmentBlock_total(demand_dsm_0) <= +inf
+   33 <= SinkDSMOemofInvestmentBlock_invest(demand_dsm_0) <= 100
 end
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/emission_limit.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/emission_limit.lp`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,47 @@
 \* Source Pyomo model name=Model *\
 
-min
+min 
 objective:
 +0 ONE_VAR_CONSTANT
 
 s.t.
 
 c_u_integral_limit_emission_factor_constraint_:
-+0.5 flow(source1_electricityBus_0)
--1 flow(source1_electricityBus_1)
-+2 flow(source1_electricityBus_2)
-+3.5 flow(source2_electricityBus_0)
-+3.5 flow(source2_electricityBus_1)
-+3.5 flow(source2_electricityBus_2)
++0.5 flow(source1_electricityBus_0_0)
+-1.0 flow(source1_electricityBus_0_1)
++2.0 flow(source1_electricityBus_0_2)
++3.5 flow(source2_electricityBus_0_0)
++3.5 flow(source2_electricityBus_0_1)
++3.5 flow(source2_electricityBus_0_2)
 <= 777
 
-c_e_BusBlock_balance(electricityBus_0)_:
-+1 flow(source1_electricityBus_0)
-+1 flow(source2_electricityBus_0)
-+1 flow(source3_electricityBus_0)
+c_e_BusBlock_balance(electricityBus_0_0)_:
++1 flow(source1_electricityBus_0_0)
++1 flow(source2_electricityBus_0_0)
++1 flow(source3_electricityBus_0_0)
 = 0
 
-c_e_BusBlock_balance(electricityBus_1)_:
-+1 flow(source1_electricityBus_1)
-+1 flow(source2_electricityBus_1)
-+1 flow(source3_electricityBus_1)
+c_e_BusBlock_balance(electricityBus_0_1)_:
++1 flow(source1_electricityBus_0_1)
++1 flow(source2_electricityBus_0_1)
++1 flow(source3_electricityBus_0_1)
 = 0
 
-c_e_BusBlock_balance(electricityBus_2)_:
-+1 flow(source1_electricityBus_2)
-+1 flow(source2_electricityBus_2)
-+1 flow(source3_electricityBus_2)
+c_e_BusBlock_balance(electricityBus_0_2)_:
++1 flow(source1_electricityBus_0_2)
++1 flow(source2_electricityBus_0_2)
++1 flow(source3_electricityBus_0_2)
 = 0
 
-c_e_ONE_VAR_CONSTANT:
-ONE_VAR_CONSTANT = 1.0
-
 bounds
-   0 <= flow(source1_electricityBus_0) <= 100
-   0 <= flow(source1_electricityBus_1) <= 100
-   0 <= flow(source1_electricityBus_2) <= 100
-   0 <= flow(source2_electricityBus_0) <= 100
-   0 <= flow(source2_electricityBus_1) <= 100
-   0 <= flow(source2_electricityBus_2) <= 100
-   0 <= flow(source3_electricityBus_0) <= 100
-   0 <= flow(source3_electricityBus_1) <= 100
-   0 <= flow(source3_electricityBus_2) <= 100
+   1 <= ONE_VAR_CONSTANT <= 1
+   0 <= flow(source1_electricityBus_0_0) <= 100
+   0 <= flow(source1_electricityBus_0_1) <= 100
+   0 <= flow(source1_electricityBus_0_2) <= 100
+   0 <= flow(source2_electricityBus_0_0) <= 100
+   0 <= flow(source2_electricityBus_0_1) <= 100
+   0 <= flow(source2_electricityBus_0_2) <= 100
+   0 <= flow(source3_electricityBus_0_0) <= 100
+   0 <= flow(source3_electricityBus_0_1) <= 100
+   0 <= flow(source3_electricityBus_0_2) <= 100
 end
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/equate_flows.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/equate_flows.lp`

 * *Files 14% similar despite different names*

```diff
@@ -1,66 +1,63 @@
 \* Source Pyomo model name=Model *\
 
 min 
 objective:
-+2 flow(Bus1_Sink_0)
-+2 flow(Bus1_Sink_1)
-+2 flow(Bus1_Sink_2)
-+2 flow(Source1_Bus1_0)
-+2 flow(Source1_Bus1_1)
-+2 flow(Source1_Bus1_2)
-+10 flow(Source2_Bus1_0)
-+10 flow(Source2_Bus1_1)
-+10 flow(Source2_Bus1_2)
++2 flow(Bus1_Sink_0_0)
++2 flow(Bus1_Sink_0_1)
++2 flow(Bus1_Sink_0_2)
++2 flow(Source1_Bus1_0_0)
++2 flow(Source1_Bus1_0_1)
++2 flow(Source1_Bus1_0_2)
++10 flow(Source2_Bus1_0_0)
++10 flow(Source2_Bus1_0_1)
++10 flow(Source2_Bus1_0_2)
 
 s.t.
 
-c_e_equate_flows(0)_:
--1 flow(Bus1_Sink_0)
-+2 flow(Source1_Bus1_0)
-+2 flow(Source2_Bus1_0)
+c_e_equate_flows(0_0)_:
+-1 flow(Bus1_Sink_0_0)
++2 flow(Source1_Bus1_0_0)
++2 flow(Source2_Bus1_0_0)
 = 0
 
-c_e_equate_flows(1)_:
--1 flow(Bus1_Sink_1)
-+2 flow(Source1_Bus1_1)
-+2 flow(Source2_Bus1_1)
+c_e_equate_flows(0_1)_:
+-1 flow(Bus1_Sink_0_1)
++2 flow(Source1_Bus1_0_1)
++2 flow(Source2_Bus1_0_1)
 = 0
 
-c_e_equate_flows(2)_:
--1 flow(Bus1_Sink_2)
-+2 flow(Source1_Bus1_2)
-+2 flow(Source2_Bus1_2)
+c_e_equate_flows(0_2)_:
+-1 flow(Bus1_Sink_0_2)
++2 flow(Source1_Bus1_0_2)
++2 flow(Source2_Bus1_0_2)
 = 0
 
-c_e_BusBlock_balance(Bus1_0)_:
--1 flow(Bus1_Sink_0)
-+1 flow(Source1_Bus1_0)
-+1 flow(Source2_Bus1_0)
+c_e_BusBlock_balance(Bus1_0_0)_:
+-1 flow(Bus1_Sink_0_0)
++1 flow(Source1_Bus1_0_0)
++1 flow(Source2_Bus1_0_0)
 = 0
 
-c_e_BusBlock_balance(Bus1_1)_:
--1 flow(Bus1_Sink_1)
-+1 flow(Source1_Bus1_1)
-+1 flow(Source2_Bus1_1)
+c_e_BusBlock_balance(Bus1_0_1)_:
+-1 flow(Bus1_Sink_0_1)
++1 flow(Source1_Bus1_0_1)
++1 flow(Source2_Bus1_0_1)
 = 0
 
-c_e_BusBlock_balance(Bus1_2)_:
--1 flow(Bus1_Sink_2)
-+1 flow(Source1_Bus1_2)
-+1 flow(Source2_Bus1_2)
+c_e_BusBlock_balance(Bus1_0_2)_:
+-1 flow(Bus1_Sink_0_2)
++1 flow(Source1_Bus1_0_2)
++1 flow(Source2_Bus1_0_2)
 = 0
 
-c_e_ONE_VAR_CONSTANT: 
-ONE_VAR_CONSTANT = 1.0
-
 bounds
-   0 <= flow(Bus1_Sink_0) <= 300
-   0 <= flow(Bus1_Sink_1) <= 300
-   0 <= flow(Bus1_Sink_2) <= 300
-   0 <= flow(Source1_Bus1_0) <= 400
-   0 <= flow(Source1_Bus1_1) <= 400
-   0 <= flow(Source1_Bus1_2) <= 400
-   0 <= flow(Source2_Bus1_0) <= 200
-   0 <= flow(Source2_Bus1_1) <= 200
-   0 <= flow(Source2_Bus1_2) <= 200
+   0 <= flow(Bus1_Sink_0_0) <= 300
+   0 <= flow(Bus1_Sink_0_1) <= 300
+   0 <= flow(Bus1_Sink_0_2) <= 300
+   0 <= flow(Source1_Bus1_0_0) <= 400
+   0 <= flow(Source1_Bus1_0_1) <= 400
+   0 <= flow(Source1_Bus1_0_2) <= 400
+   0 <= flow(Source2_Bus1_0_0) <= 200
+   0 <= flow(Source2_Bus1_0_1) <= 200
+   0 <= flow(Source2_Bus1_0_2) <= 200
 end
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/fixed_source_invest_sink.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/fixed_source_invest_sink.lp`

 * *Files 21% similar despite different names*

```diff
@@ -1,54 +1,57 @@
 \* Source Pyomo model name=Model *\
 
 min 
 objective:
-+500 InvestmentFlowBlock_invest(electricityBus_excess)
-+25 flow(electricityBus_excess_0)
-+25 flow(electricityBus_excess_1)
-+25 flow(electricityBus_excess_2)
++500 InvestmentFlowBlock_invest(electricityBus_excess_0)
++25 flow(electricityBus_excess_0_0)
++25 flow(electricityBus_excess_0_1)
++25 flow(electricityBus_excess_0_2)
 
 s.t.
 
-c_e_BusBlock_balance(electricityBus_0)_:
--1 flow(electricityBus_excess_0)
-= -12000000
-
-c_e_BusBlock_balance(electricityBus_1)_:
--1 flow(electricityBus_excess_1)
-= -16000000
-
-c_e_BusBlock_balance(electricityBus_2)_:
--1 flow(electricityBus_excess_2)
-= -14000000
-
-c_u_InvestmentFlowBlock_max(electricityBus_excess_0)_:
--0.80000000000000004 InvestmentFlowBlock_invest(electricityBus_excess)
-+1 flow(electricityBus_excess_0)
-<= 40
-
-c_u_InvestmentFlowBlock_max(electricityBus_excess_1)_:
--0.80000000000000004 InvestmentFlowBlock_invest(electricityBus_excess)
-+1 flow(electricityBus_excess_1)
-<= 40
-
-c_u_InvestmentFlowBlock_max(electricityBus_excess_2)_:
--0.80000000000000004 InvestmentFlowBlock_invest(electricityBus_excess)
-+1 flow(electricityBus_excess_2)
-<= 40
+c_e_BusBlock_balance(electricityBus_0_0)_:
+-1 flow(electricityBus_excess_0_0)
+= -12000000.0
+
+c_e_BusBlock_balance(electricityBus_0_1)_:
+-1 flow(electricityBus_excess_0_1)
+= -16000000.0
+
+c_e_BusBlock_balance(electricityBus_0_2)_:
+-1 flow(electricityBus_excess_0_2)
+= -14000000.0
+
+c_e_InvestmentFlowBlock_total_rule(electricityBus_excess_0)_:
+-1 InvestmentFlowBlock_invest(electricityBus_excess_0)
++1 InvestmentFlowBlock_total(electricityBus_excess_0)
+= 50
+
+c_u_InvestmentFlowBlock_max(electricityBus_excess_0_0)_:
++1 flow(electricityBus_excess_0_0)
+-0.8 InvestmentFlowBlock_total(electricityBus_excess_0)
+<= 0
+
+c_u_InvestmentFlowBlock_max(electricityBus_excess_0_1)_:
++1 flow(electricityBus_excess_0_1)
+-0.8 InvestmentFlowBlock_total(electricityBus_excess_0)
+<= 0
+
+c_u_InvestmentFlowBlock_max(electricityBus_excess_0_2)_:
++1 flow(electricityBus_excess_0_2)
+-0.8 InvestmentFlowBlock_total(electricityBus_excess_0)
+<= 0
 
 c_u_InvestmentFlowBlock_full_load_time_max(electricityBus_excess)_:
--2.2999999999999998 InvestmentFlowBlock_invest(electricityBus_excess)
-+1 flow(electricityBus_excess_0)
-+1 flow(electricityBus_excess_1)
-+1 flow(electricityBus_excess_2)
-<= 114.99999999999999
-
-c_e_ONE_VAR_CONSTANT: 
-ONE_VAR_CONSTANT = 1.0
++1 flow(electricityBus_excess_0_0)
++1 flow(electricityBus_excess_0_1)
++1 flow(electricityBus_excess_0_2)
+-2.3 InvestmentFlowBlock_total(electricityBus_excess_0)
+<= 0
 
 bounds
-   0 <= flow(electricityBus_excess_0) <= +inf
-   0 <= flow(electricityBus_excess_1) <= +inf
-   0 <= flow(electricityBus_excess_2) <= +inf
-   0 <= InvestmentFlowBlock_invest(electricityBus_excess) <= 1000000
+   0 <= InvestmentFlowBlock_invest(electricityBus_excess_0) <= 1000000.0
+   0 <= flow(electricityBus_excess_0_0) <= +inf
+   0 <= flow(electricityBus_excess_0_1) <= +inf
+   0 <= flow(electricityBus_excess_0_2) <= +inf
+   0 <= InvestmentFlowBlock_total(electricityBus_excess_0) <= +inf
 end
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/fixed_source_variable_sink.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/fixed_source_variable_sink.lp`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 \* Source Pyomo model name=Model *\
 
-min
+min 
 objective:
-+40 flow(electricityBus_excess_0)
-+40 flow(electricityBus_excess_1)
-+40 flow(electricityBus_excess_2)
++40 flow(electricityBus_excess_0_0)
++40 flow(electricityBus_excess_0_1)
++40 flow(electricityBus_excess_0_2)
 
 s.t.
 
-c_e_BusBlock_balance(electricityBus_0)_:
--1 flow(electricityBus_excess_0)
-= -430000
-
-c_e_BusBlock_balance(electricityBus_1)_:
--1 flow(electricityBus_excess_1)
-= -720000
-
-c_e_BusBlock_balance(electricityBus_2)_:
--1 flow(electricityBus_excess_2)
-= -290000
-
-c_e_ONE_VAR_CONSTANT:
-ONE_VAR_CONSTANT = 1.0
+c_e_BusBlock_balance(electricityBus_0_0)_:
+-1 flow(electricityBus_excess_0_0)
+= -430000.0
+
+c_e_BusBlock_balance(electricityBus_0_1)_:
+-1 flow(electricityBus_excess_0_1)
+= -720000.0
+
+c_e_BusBlock_balance(electricityBus_0_2)_:
+-1 flow(electricityBus_excess_0_2)
+= -290000.0
 
 bounds
-   0 <= flow(electricityBus_excess_0) <= +inf
-   0 <= flow(electricityBus_excess_1) <= +inf
-   0 <= flow(electricityBus_excess_2) <= +inf
+   0 <= flow(electricityBus_excess_0_0) <= +inf
+   0 <= flow(electricityBus_excess_0_1) <= +inf
+   0 <= flow(electricityBus_excess_0_2) <= +inf
 end
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/flow_count_limit.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/flow_count_limit.lp`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 \* Source Pyomo model name=Model *\
 
-min
+min 
 objective:
 +0 ONE_VAR_CONSTANT
 
 s.t.
 
 c_e_emission_factor_constraint(0)_:
 +1 NonConvexFlowBlock_status(source1_electricityBus_0)
@@ -20,33 +20,33 @@
 
 c_e_emission_factor_constraint(2)_:
 +1 NonConvexFlowBlock_status(source1_electricityBus_2)
 +1 NonConvexFlowBlock_status(source2_electricityBus_2)
 -1 emission_factor(2)
 = 0
 
-c_e_BusBlock_balance(electricityBus_0)_:
-+1 flow(source1_electricityBus_0)
-+1 flow(source2_electricityBus_0)
-+1 flow(source3_electricityBus_0)
-+1 flow(source4_electricityBus_0)
-= 0
-
-c_e_BusBlock_balance(electricityBus_1)_:
-+1 flow(source1_electricityBus_1)
-+1 flow(source2_electricityBus_1)
-+1 flow(source3_electricityBus_1)
-+1 flow(source4_electricityBus_1)
-= 0
-
-c_e_BusBlock_balance(electricityBus_2)_:
-+1 flow(source1_electricityBus_2)
-+1 flow(source2_electricityBus_2)
-+1 flow(source3_electricityBus_2)
-+1 flow(source4_electricityBus_2)
+c_e_BusBlock_balance(electricityBus_0_0)_:
++1 flow(source4_electricityBus_0_0)
++1 flow(source2_electricityBus_0_0)
++1 flow(source1_electricityBus_0_0)
++1 flow(source3_electricityBus_0_0)
+= 0
+
+c_e_BusBlock_balance(electricityBus_0_1)_:
++1 flow(source4_electricityBus_0_1)
++1 flow(source2_electricityBus_0_1)
++1 flow(source1_electricityBus_0_1)
++1 flow(source3_electricityBus_0_1)
+= 0
+
+c_e_BusBlock_balance(electricityBus_0_2)_:
++1 flow(source4_electricityBus_0_2)
++1 flow(source2_electricityBus_0_2)
++1 flow(source1_electricityBus_0_2)
++1 flow(source3_electricityBus_0_2)
 = 0
 
 c_e_NonConvexFlowBlock_status_nominal_constraint(source1_electricityBus_0)_:
 -100 NonConvexFlowBlock_status(source1_electricityBus_0)
 +1 NonConvexFlowBlock_status_nominal(source1_electricityBus_0)
 = 0
 
@@ -56,14 +56,29 @@
 = 0
 
 c_e_NonConvexFlowBlock_status_nominal_constraint(source1_electricityBus_2)_:
 -100 NonConvexFlowBlock_status(source1_electricityBus_2)
 +1 NonConvexFlowBlock_status_nominal(source1_electricityBus_2)
 = 0
 
+c_e_NonConvexFlowBlock_status_nominal_constraint(source3_electricityBus_0)_:
++1 NonConvexFlowBlock_status_nominal(source3_electricityBus_0)
+-100 NonConvexFlowBlock_status(source3_electricityBus_0)
+= 0
+
+c_e_NonConvexFlowBlock_status_nominal_constraint(source3_electricityBus_1)_:
++1 NonConvexFlowBlock_status_nominal(source3_electricityBus_1)
+-100 NonConvexFlowBlock_status(source3_electricityBus_1)
+= 0
+
+c_e_NonConvexFlowBlock_status_nominal_constraint(source3_electricityBus_2)_:
++1 NonConvexFlowBlock_status_nominal(source3_electricityBus_2)
+-100 NonConvexFlowBlock_status(source3_electricityBus_2)
+= 0
+
 c_e_NonConvexFlowBlock_status_nominal_constraint(source2_electricityBus_0)_:
 -100 NonConvexFlowBlock_status(source2_electricityBus_0)
 +1 NonConvexFlowBlock_status_nominal(source2_electricityBus_0)
 = 0
 
 c_e_NonConvexFlowBlock_status_nominal_constraint(source2_electricityBus_1)_:
 -100 NonConvexFlowBlock_status(source2_electricityBus_1)
@@ -71,151 +86,134 @@
 = 0
 
 c_e_NonConvexFlowBlock_status_nominal_constraint(source2_electricityBus_2)_:
 -100 NonConvexFlowBlock_status(source2_electricityBus_2)
 +1 NonConvexFlowBlock_status_nominal(source2_electricityBus_2)
 = 0
 
-c_e_NonConvexFlowBlock_status_nominal_constraint(source3_electricityBus_0)_:
--100 NonConvexFlowBlock_status(source3_electricityBus_0)
-+1 NonConvexFlowBlock_status_nominal(source3_electricityBus_0)
-= 0
+c_u_NonConvexFlowBlock_min(source1_electricityBus_0_0)_:
+-1 flow(source1_electricityBus_0_0)
+<= 0
 
-c_e_NonConvexFlowBlock_status_nominal_constraint(source3_electricityBus_1)_:
--100 NonConvexFlowBlock_status(source3_electricityBus_1)
-+1 NonConvexFlowBlock_status_nominal(source3_electricityBus_1)
-= 0
+c_u_NonConvexFlowBlock_min(source1_electricityBus_0_1)_:
+-1 flow(source1_electricityBus_0_1)
+<= 0
 
-c_e_NonConvexFlowBlock_status_nominal_constraint(source3_electricityBus_2)_:
--100 NonConvexFlowBlock_status(source3_electricityBus_2)
-+1 NonConvexFlowBlock_status_nominal(source3_electricityBus_2)
-= 0
+c_u_NonConvexFlowBlock_min(source1_electricityBus_0_2)_:
+-1 flow(source1_electricityBus_0_2)
+<= 0
 
-c_l_NonConvexFlowBlock_min(source1_electricityBus_0)_:
-+1 flow(source1_electricityBus_0)
->= 0
-
-c_l_NonConvexFlowBlock_min(source1_electricityBus_1)_:
-+1 flow(source1_electricityBus_1)
->= 0
-
-c_l_NonConvexFlowBlock_min(source1_electricityBus_2)_:
-+1 flow(source1_electricityBus_2)
->= 0
-
-c_l_NonConvexFlowBlock_min(source2_electricityBus_0)_:
-+1 flow(source2_electricityBus_0)
->= 0
-
-c_l_NonConvexFlowBlock_min(source2_electricityBus_1)_:
-+1 flow(source2_electricityBus_1)
->= 0
-
-c_l_NonConvexFlowBlock_min(source2_electricityBus_2)_:
-+1 flow(source2_electricityBus_2)
->= 0
-
-c_l_NonConvexFlowBlock_min(source3_electricityBus_0)_:
-+1 flow(source3_electricityBus_0)
->= 0
-
-c_l_NonConvexFlowBlock_min(source3_electricityBus_1)_:
-+1 flow(source3_electricityBus_1)
->= 0
-
-c_l_NonConvexFlowBlock_min(source3_electricityBus_2)_:
-+1 flow(source3_electricityBus_2)
->= 0
+c_u_NonConvexFlowBlock_min(source3_electricityBus_0_0)_:
+-1 flow(source3_electricityBus_0_0)
+<= 0
 
-c_u_NonConvexFlowBlock_max(source1_electricityBus_0)_:
--1 NonConvexFlowBlock_status_nominal(source1_electricityBus_0)
-+1 flow(source1_electricityBus_0)
+c_u_NonConvexFlowBlock_min(source3_electricityBus_0_1)_:
+-1 flow(source3_electricityBus_0_1)
 <= 0
 
-c_u_NonConvexFlowBlock_max(source1_electricityBus_1)_:
--1 NonConvexFlowBlock_status_nominal(source1_electricityBus_1)
-+1 flow(source1_electricityBus_1)
+c_u_NonConvexFlowBlock_min(source3_electricityBus_0_2)_:
+-1 flow(source3_electricityBus_0_2)
 <= 0
 
-c_u_NonConvexFlowBlock_max(source1_electricityBus_2)_:
--1 NonConvexFlowBlock_status_nominal(source1_electricityBus_2)
-+1 flow(source1_electricityBus_2)
+c_u_NonConvexFlowBlock_min(source2_electricityBus_0_0)_:
+-1 flow(source2_electricityBus_0_0)
 <= 0
 
-c_u_NonConvexFlowBlock_max(source2_electricityBus_0)_:
--1 NonConvexFlowBlock_status_nominal(source2_electricityBus_0)
-+1 flow(source2_electricityBus_0)
+c_u_NonConvexFlowBlock_min(source2_electricityBus_0_1)_:
+-1 flow(source2_electricityBus_0_1)
 <= 0
 
-c_u_NonConvexFlowBlock_max(source2_electricityBus_1)_:
--1 NonConvexFlowBlock_status_nominal(source2_electricityBus_1)
-+1 flow(source2_electricityBus_1)
+c_u_NonConvexFlowBlock_min(source2_electricityBus_0_2)_:
+-1 flow(source2_electricityBus_0_2)
 <= 0
 
-c_u_NonConvexFlowBlock_max(source2_electricityBus_2)_:
--1 NonConvexFlowBlock_status_nominal(source2_electricityBus_2)
-+1 flow(source2_electricityBus_2)
+c_u_NonConvexFlowBlock_max(source1_electricityBus_0_0)_:
++1 flow(source1_electricityBus_0_0)
+-1 NonConvexFlowBlock_status_nominal(source1_electricityBus_0)
+<= 0
+
+c_u_NonConvexFlowBlock_max(source1_electricityBus_0_1)_:
++1 flow(source1_electricityBus_0_1)
+-1 NonConvexFlowBlock_status_nominal(source1_electricityBus_1)
+<= 0
+
+c_u_NonConvexFlowBlock_max(source1_electricityBus_0_2)_:
++1 flow(source1_electricityBus_0_2)
+-1 NonConvexFlowBlock_status_nominal(source1_electricityBus_2)
 <= 0
 
-c_u_NonConvexFlowBlock_max(source3_electricityBus_0)_:
+c_u_NonConvexFlowBlock_max(source3_electricityBus_0_0)_:
++1 flow(source3_electricityBus_0_0)
 -1 NonConvexFlowBlock_status_nominal(source3_electricityBus_0)
-+1 flow(source3_electricityBus_0)
 <= 0
 
-c_u_NonConvexFlowBlock_max(source3_electricityBus_1)_:
+c_u_NonConvexFlowBlock_max(source3_electricityBus_0_1)_:
++1 flow(source3_electricityBus_0_1)
 -1 NonConvexFlowBlock_status_nominal(source3_electricityBus_1)
-+1 flow(source3_electricityBus_1)
 <= 0
 
-c_u_NonConvexFlowBlock_max(source3_electricityBus_2)_:
+c_u_NonConvexFlowBlock_max(source3_electricityBus_0_2)_:
++1 flow(source3_electricityBus_0_2)
 -1 NonConvexFlowBlock_status_nominal(source3_electricityBus_2)
-+1 flow(source3_electricityBus_2)
 <= 0
 
-c_e_ONE_VAR_CONSTANT:
-ONE_VAR_CONSTANT = 1.0
+c_u_NonConvexFlowBlock_max(source2_electricityBus_0_0)_:
++1 flow(source2_electricityBus_0_0)
+-1 NonConvexFlowBlock_status_nominal(source2_electricityBus_0)
+<= 0
+
+c_u_NonConvexFlowBlock_max(source2_electricityBus_0_1)_:
++1 flow(source2_electricityBus_0_1)
+-1 NonConvexFlowBlock_status_nominal(source2_electricityBus_1)
+<= 0
+
+c_u_NonConvexFlowBlock_max(source2_electricityBus_0_2)_:
++1 flow(source2_electricityBus_0_2)
+-1 NonConvexFlowBlock_status_nominal(source2_electricityBus_2)
+<= 0
 
 bounds
-   0 <= flow(source1_electricityBus_0) <= 100
-   0 <= flow(source1_electricityBus_1) <= 100
-   0 <= flow(source1_electricityBus_2) <= 100
-   0 <= flow(source2_electricityBus_0) <= 100
-   0 <= flow(source2_electricityBus_1) <= 100
-   0 <= flow(source2_electricityBus_2) <= 100
-   0 <= flow(source3_electricityBus_0) <= 100
-   0 <= flow(source3_electricityBus_1) <= 100
-   0 <= flow(source3_electricityBus_2) <= 100
-   30 <= flow(source4_electricityBus_0) <= 100
-   30 <= flow(source4_electricityBus_1) <= 100
-   30 <= flow(source4_electricityBus_2) <= 100
-   1 <= emission_factor(0) <= 2
-   1 <= emission_factor(1) <= 2
-   1 <= emission_factor(2) <= 2
+   1 <= ONE_VAR_CONSTANT <= 1
    0 <= NonConvexFlowBlock_status(source1_electricityBus_0) <= 1
-   0 <= NonConvexFlowBlock_status(source1_electricityBus_1) <= 1
-   0 <= NonConvexFlowBlock_status(source1_electricityBus_2) <= 1
    0 <= NonConvexFlowBlock_status(source2_electricityBus_0) <= 1
+   1 <= emission_factor(0) <= 2
+   0 <= NonConvexFlowBlock_status(source1_electricityBus_1) <= 1
    0 <= NonConvexFlowBlock_status(source2_electricityBus_1) <= 1
+   1 <= emission_factor(1) <= 2
+   0 <= NonConvexFlowBlock_status(source1_electricityBus_2) <= 1
    0 <= NonConvexFlowBlock_status(source2_electricityBus_2) <= 1
-   0 <= NonConvexFlowBlock_status(source3_electricityBus_0) <= 1
-   0 <= NonConvexFlowBlock_status(source3_electricityBus_1) <= 1
-   0 <= NonConvexFlowBlock_status(source3_electricityBus_2) <= 1
+   1 <= emission_factor(2) <= 2
+   30.0 <= flow(source4_electricityBus_0_0) <= 100
+   0 <= flow(source2_electricityBus_0_0) <= 100
+   0 <= flow(source1_electricityBus_0_0) <= 100
+   0 <= flow(source3_electricityBus_0_0) <= 100
+   30.0 <= flow(source4_electricityBus_0_1) <= 100
+   0 <= flow(source2_electricityBus_0_1) <= 100
+   0 <= flow(source1_electricityBus_0_1) <= 100
+   0 <= flow(source3_electricityBus_0_1) <= 100
+   30.0 <= flow(source4_electricityBus_0_2) <= 100
+   0 <= flow(source2_electricityBus_0_2) <= 100
+   0 <= flow(source1_electricityBus_0_2) <= 100
+   0 <= flow(source3_electricityBus_0_2) <= 100
    0 <= NonConvexFlowBlock_status_nominal(source1_electricityBus_0) <= +inf
    0 <= NonConvexFlowBlock_status_nominal(source1_electricityBus_1) <= +inf
    0 <= NonConvexFlowBlock_status_nominal(source1_electricityBus_2) <= +inf
-   0 <= NonConvexFlowBlock_status_nominal(source2_electricityBus_0) <= +inf
-   0 <= NonConvexFlowBlock_status_nominal(source2_electricityBus_1) <= +inf
-   0 <= NonConvexFlowBlock_status_nominal(source2_electricityBus_2) <= +inf
    0 <= NonConvexFlowBlock_status_nominal(source3_electricityBus_0) <= +inf
+   0 <= NonConvexFlowBlock_status(source3_electricityBus_0) <= 1
    0 <= NonConvexFlowBlock_status_nominal(source3_electricityBus_1) <= +inf
+   0 <= NonConvexFlowBlock_status(source3_electricityBus_1) <= 1
    0 <= NonConvexFlowBlock_status_nominal(source3_electricityBus_2) <= +inf
+   0 <= NonConvexFlowBlock_status(source3_electricityBus_2) <= 1
+   0 <= NonConvexFlowBlock_status_nominal(source2_electricityBus_0) <= +inf
+   0 <= NonConvexFlowBlock_status_nominal(source2_electricityBus_1) <= +inf
+   0 <= NonConvexFlowBlock_status_nominal(source2_electricityBus_2) <= +inf
 binary
   NonConvexFlowBlock_status(source1_electricityBus_0)
-  NonConvexFlowBlock_status(source1_electricityBus_1)
-  NonConvexFlowBlock_status(source1_electricityBus_2)
   NonConvexFlowBlock_status(source2_electricityBus_0)
+  NonConvexFlowBlock_status(source1_electricityBus_1)
   NonConvexFlowBlock_status(source2_electricityBus_1)
+  NonConvexFlowBlock_status(source1_electricityBus_2)
   NonConvexFlowBlock_status(source2_electricityBus_2)
   NonConvexFlowBlock_status(source3_electricityBus_0)
   NonConvexFlowBlock_status(source3_electricityBus_1)
   NonConvexFlowBlock_status(source3_electricityBus_2)
 end
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/flow_invest_with_offset.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/flow_invest_with_offset.lp`

 * *Files 13% similar despite different names*

```diff
@@ -1,68 +1,71 @@
 \* Source Pyomo model name=Model *\
 
 min 
 objective:
-+500 InvestmentFlowBlock_invest(source_nonconvex_invest_electricityBus)
-+34 InvestmentFlowBlock_invest_status(source_nonconvex_invest_electricityBus)
-+25 flow(source_nonconvex_invest_electricityBus_0)
-+25 flow(source_nonconvex_invest_electricityBus_1)
-+25 flow(source_nonconvex_invest_electricityBus_2)
++500 InvestmentFlowBlock_invest(source_nonconvex_invest_electricityBus_0)
++34 InvestmentFlowBlock_invest_status(source_nonconvex_invest_electricityBus_0)
++25 flow(source_nonconvex_invest_electricityBus_0_0)
++25 flow(source_nonconvex_invest_electricityBus_0_1)
++25 flow(source_nonconvex_invest_electricityBus_0_2)
 
 s.t.
 
-c_e_BusBlock_balance(electricityBus_0)_:
-+1 flow(source_nonconvex_invest_electricityBus_0)
+c_e_BusBlock_balance(electricityBus_0_0)_:
++1 flow(source_nonconvex_invest_electricityBus_0_0)
 = 0
 
-c_e_BusBlock_balance(electricityBus_1)_:
-+1 flow(source_nonconvex_invest_electricityBus_1)
+c_e_BusBlock_balance(electricityBus_0_1)_:
++1 flow(source_nonconvex_invest_electricityBus_0_1)
 = 0
 
-c_e_BusBlock_balance(electricityBus_2)_:
-+1 flow(source_nonconvex_invest_electricityBus_2)
+c_e_BusBlock_balance(electricityBus_0_2)_:
++1 flow(source_nonconvex_invest_electricityBus_0_2)
 = 0
 
-c_u_InvestmentFlowBlock_minimum_rule(source_nonconvex_invest_electricityBus)_:
--1 InvestmentFlowBlock_invest(source_nonconvex_invest_electricityBus)
-+15 InvestmentFlowBlock_invest_status(source_nonconvex_invest_electricityBus)
+c_u_InvestmentFlowBlock_minimum_rule(source_nonconvex_invest_electricityBus_0)_:
+-1 InvestmentFlowBlock_invest(source_nonconvex_invest_electricityBus_0)
++15 InvestmentFlowBlock_invest_status(source_nonconvex_invest_electricityBus_0)
 <= 0
 
-c_u_InvestmentFlowBlock_maximum_rule(source_nonconvex_invest_electricityBus)_:
-+1 InvestmentFlowBlock_invest(source_nonconvex_invest_electricityBus)
--20 InvestmentFlowBlock_invest_status(source_nonconvex_invest_electricityBus)
+c_u_InvestmentFlowBlock_maximum_rule(source_nonconvex_invest_electricityBus_0)_:
++1 InvestmentFlowBlock_invest(source_nonconvex_invest_electricityBus_0)
+-20 InvestmentFlowBlock_invest_status(source_nonconvex_invest_electricityBus_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(source_nonconvex_invest_electricityBus_0)_:
--0.80000000000000004 InvestmentFlowBlock_invest(source_nonconvex_invest_electricityBus)
-+1 flow(source_nonconvex_invest_electricityBus_0)
+c_e_InvestmentFlowBlock_total_rule(source_nonconvex_invest_electricityBus_0)_:
+-1 InvestmentFlowBlock_invest(source_nonconvex_invest_electricityBus_0)
++1 InvestmentFlowBlock_total(source_nonconvex_invest_electricityBus_0)
+= 0
+
+c_u_InvestmentFlowBlock_max(source_nonconvex_invest_electricityBus_0_0)_:
++1 flow(source_nonconvex_invest_electricityBus_0_0)
+-0.8 InvestmentFlowBlock_total(source_nonconvex_invest_electricityBus_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(source_nonconvex_invest_electricityBus_1)_:
--0.80000000000000004 InvestmentFlowBlock_invest(source_nonconvex_invest_electricityBus)
-+1 flow(source_nonconvex_invest_electricityBus_1)
+c_u_InvestmentFlowBlock_max(source_nonconvex_invest_electricityBus_0_1)_:
++1 flow(source_nonconvex_invest_electricityBus_0_1)
+-0.8 InvestmentFlowBlock_total(source_nonconvex_invest_electricityBus_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(source_nonconvex_invest_electricityBus_2)_:
--0.80000000000000004 InvestmentFlowBlock_invest(source_nonconvex_invest_electricityBus)
-+1 flow(source_nonconvex_invest_electricityBus_2)
+c_u_InvestmentFlowBlock_max(source_nonconvex_invest_electricityBus_0_2)_:
++1 flow(source_nonconvex_invest_electricityBus_0_2)
+-0.8 InvestmentFlowBlock_total(source_nonconvex_invest_electricityBus_0)
 <= 0
 
 c_u_InvestmentFlowBlock_full_load_time_max(source_nonconvex_invest_electricityBus)_:
--2.2999999999999998 InvestmentFlowBlock_invest(source_nonconvex_invest_electricityBus)
-+1 flow(source_nonconvex_invest_electricityBus_0)
-+1 flow(source_nonconvex_invest_electricityBus_1)
-+1 flow(source_nonconvex_invest_electricityBus_2)
++1 flow(source_nonconvex_invest_electricityBus_0_0)
++1 flow(source_nonconvex_invest_electricityBus_0_1)
++1 flow(source_nonconvex_invest_electricityBus_0_2)
+-2.3 InvestmentFlowBlock_total(source_nonconvex_invest_electricityBus_0)
 <= 0
 
-c_e_ONE_VAR_CONSTANT: 
-ONE_VAR_CONSTANT = 1.0
-
 bounds
-   0 <= flow(source_nonconvex_invest_electricityBus_0) <= +inf
-   0 <= flow(source_nonconvex_invest_electricityBus_1) <= +inf
-   0 <= flow(source_nonconvex_invest_electricityBus_2) <= +inf
-   0 <= InvestmentFlowBlock_invest(source_nonconvex_invest_electricityBus) <= 20
-   0 <= InvestmentFlowBlock_invest_status(source_nonconvex_invest_electricityBus) <= 1
+   0 <= InvestmentFlowBlock_invest(source_nonconvex_invest_electricityBus_0) <= 20
+   0 <= InvestmentFlowBlock_invest_status(source_nonconvex_invest_electricityBus_0) <= 1
+   0 <= flow(source_nonconvex_invest_electricityBus_0_0) <= +inf
+   0 <= flow(source_nonconvex_invest_electricityBus_0_1) <= +inf
+   0 <= flow(source_nonconvex_invest_electricityBus_0_2) <= +inf
+   0 <= InvestmentFlowBlock_total(source_nonconvex_invest_electricityBus_0) <= +inf
 binary
-  InvestmentFlowBlock_invest_status(source_nonconvex_invest_electricityBus)
+  InvestmentFlowBlock_invest_status(source_nonconvex_invest_electricityBus_0)
 end
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/flow_invest_with_offset_no_minimum.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/flow_invest_with_offset_no_minimum.lp`

 * *Files 22% similar despite different names*

```diff
@@ -1,67 +1,70 @@
 \* Source Pyomo model name=Model *\
 
 min 
 objective:
-+500 InvestmentFlowBlock_invest(source_nonconvex_invest_electricityBus)
-+34 InvestmentFlowBlock_invest_status(source_nonconvex_invest_electricityBus)
-+25 flow(source_nonconvex_invest_electricityBus_0)
-+25 flow(source_nonconvex_invest_electricityBus_1)
-+25 flow(source_nonconvex_invest_electricityBus_2)
++500 InvestmentFlowBlock_invest(source_nonconvex_invest_electricityBus_0)
++34 InvestmentFlowBlock_invest_status(source_nonconvex_invest_electricityBus_0)
++25 flow(source_nonconvex_invest_electricityBus_0_0)
++25 flow(source_nonconvex_invest_electricityBus_0_1)
++25 flow(source_nonconvex_invest_electricityBus_0_2)
 
 s.t.
 
-c_e_BusBlock_balance(electricityBus_0)_:
-+1 flow(source_nonconvex_invest_electricityBus_0)
+c_e_BusBlock_balance(electricityBus_0_0)_:
++1 flow(source_nonconvex_invest_electricityBus_0_0)
 = 0
 
-c_e_BusBlock_balance(electricityBus_1)_:
-+1 flow(source_nonconvex_invest_electricityBus_1)
+c_e_BusBlock_balance(electricityBus_0_1)_:
++1 flow(source_nonconvex_invest_electricityBus_0_1)
 = 0
 
-c_e_BusBlock_balance(electricityBus_2)_:
-+1 flow(source_nonconvex_invest_electricityBus_2)
+c_e_BusBlock_balance(electricityBus_0_2)_:
++1 flow(source_nonconvex_invest_electricityBus_0_2)
 = 0
 
-c_l_InvestmentFlowBlock_minimum_rule(source_nonconvex_invest_electricityBus)_:
-+1 InvestmentFlowBlock_invest(source_nonconvex_invest_electricityBus)
->= 0
+c_u_InvestmentFlowBlock_minimum_rule(source_nonconvex_invest_electricityBus_0)_:
+-1 InvestmentFlowBlock_invest(source_nonconvex_invest_electricityBus_0)
+<= 0
 
-c_u_InvestmentFlowBlock_maximum_rule(source_nonconvex_invest_electricityBus)_:
-+1 InvestmentFlowBlock_invest(source_nonconvex_invest_electricityBus)
--1234 InvestmentFlowBlock_invest_status(source_nonconvex_invest_electricityBus)
+c_u_InvestmentFlowBlock_maximum_rule(source_nonconvex_invest_electricityBus_0)_:
++1 InvestmentFlowBlock_invest(source_nonconvex_invest_electricityBus_0)
+-1234 InvestmentFlowBlock_invest_status(source_nonconvex_invest_electricityBus_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(source_nonconvex_invest_electricityBus_0)_:
--0.80000000000000004 InvestmentFlowBlock_invest(source_nonconvex_invest_electricityBus)
-+1 flow(source_nonconvex_invest_electricityBus_0)
+c_e_InvestmentFlowBlock_total_rule(source_nonconvex_invest_electricityBus_0)_:
+-1 InvestmentFlowBlock_invest(source_nonconvex_invest_electricityBus_0)
++1 InvestmentFlowBlock_total(source_nonconvex_invest_electricityBus_0)
+= 0
+
+c_u_InvestmentFlowBlock_max(source_nonconvex_invest_electricityBus_0_0)_:
++1 flow(source_nonconvex_invest_electricityBus_0_0)
+-0.8 InvestmentFlowBlock_total(source_nonconvex_invest_electricityBus_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(source_nonconvex_invest_electricityBus_1)_:
--0.80000000000000004 InvestmentFlowBlock_invest(source_nonconvex_invest_electricityBus)
-+1 flow(source_nonconvex_invest_electricityBus_1)
+c_u_InvestmentFlowBlock_max(source_nonconvex_invest_electricityBus_0_1)_:
++1 flow(source_nonconvex_invest_electricityBus_0_1)
+-0.8 InvestmentFlowBlock_total(source_nonconvex_invest_electricityBus_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(source_nonconvex_invest_electricityBus_2)_:
--0.80000000000000004 InvestmentFlowBlock_invest(source_nonconvex_invest_electricityBus)
-+1 flow(source_nonconvex_invest_electricityBus_2)
+c_u_InvestmentFlowBlock_max(source_nonconvex_invest_electricityBus_0_2)_:
++1 flow(source_nonconvex_invest_electricityBus_0_2)
+-0.8 InvestmentFlowBlock_total(source_nonconvex_invest_electricityBus_0)
 <= 0
 
 c_u_InvestmentFlowBlock_full_load_time_max(source_nonconvex_invest_electricityBus)_:
--2.2999999999999998 InvestmentFlowBlock_invest(source_nonconvex_invest_electricityBus)
-+1 flow(source_nonconvex_invest_electricityBus_0)
-+1 flow(source_nonconvex_invest_electricityBus_1)
-+1 flow(source_nonconvex_invest_electricityBus_2)
++1 flow(source_nonconvex_invest_electricityBus_0_0)
++1 flow(source_nonconvex_invest_electricityBus_0_1)
++1 flow(source_nonconvex_invest_electricityBus_0_2)
+-2.3 InvestmentFlowBlock_total(source_nonconvex_invest_electricityBus_0)
 <= 0
 
-c_e_ONE_VAR_CONSTANT: 
-ONE_VAR_CONSTANT = 1.0
-
 bounds
-   0 <= flow(source_nonconvex_invest_electricityBus_0) <= +inf
-   0 <= flow(source_nonconvex_invest_electricityBus_1) <= +inf
-   0 <= flow(source_nonconvex_invest_electricityBus_2) <= +inf
-   0 <= InvestmentFlowBlock_invest(source_nonconvex_invest_electricityBus) <= 1234
-   0 <= InvestmentFlowBlock_invest_status(source_nonconvex_invest_electricityBus) <= 1
+   0 <= InvestmentFlowBlock_invest(source_nonconvex_invest_electricityBus_0) <= 1234
+   0 <= InvestmentFlowBlock_invest_status(source_nonconvex_invest_electricityBus_0) <= 1
+   0 <= flow(source_nonconvex_invest_electricityBus_0_0) <= +inf
+   0 <= flow(source_nonconvex_invest_electricityBus_0_1) <= +inf
+   0 <= flow(source_nonconvex_invest_electricityBus_0_2) <= +inf
+   0 <= InvestmentFlowBlock_total(source_nonconvex_invest_electricityBus_0) <= +inf
 binary
-  InvestmentFlowBlock_invest_status(source_nonconvex_invest_electricityBus)
+  InvestmentFlowBlock_invest_status(source_nonconvex_invest_electricityBus_0)
 end
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/flow_invest_without_offset.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/flow_invest_without_offset.lp`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,70 @@
 \* Source Pyomo model name=Model *\
 
 min 
 objective:
-+500 InvestmentFlowBlock_invest(electricityBus_sink_nonconvex_invest)
-+25 flow(electricityBus_sink_nonconvex_invest_0)
-+25 flow(electricityBus_sink_nonconvex_invest_1)
-+25 flow(electricityBus_sink_nonconvex_invest_2)
++500 InvestmentFlowBlock_invest(electricityBus_sink_nonconvex_invest_0)
++25 flow(electricityBus_sink_nonconvex_invest_0_0)
++25 flow(electricityBus_sink_nonconvex_invest_0_1)
++25 flow(electricityBus_sink_nonconvex_invest_0_2)
 
 s.t.
 
-c_e_BusBlock_balance(electricityBus_0)_:
-+1 flow(electricityBus_sink_nonconvex_invest_0)
+c_e_BusBlock_balance(electricityBus_0_0)_:
++1 flow(electricityBus_sink_nonconvex_invest_0_0)
 = 0
 
-c_e_BusBlock_balance(electricityBus_1)_:
-+1 flow(electricityBus_sink_nonconvex_invest_1)
+c_e_BusBlock_balance(electricityBus_0_1)_:
++1 flow(electricityBus_sink_nonconvex_invest_0_1)
 = 0
 
-c_e_BusBlock_balance(electricityBus_2)_:
-+1 flow(electricityBus_sink_nonconvex_invest_2)
+c_e_BusBlock_balance(electricityBus_0_2)_:
++1 flow(electricityBus_sink_nonconvex_invest_0_2)
 = 0
 
-c_u_InvestmentFlowBlock_minimum_rule(electricityBus_sink_nonconvex_invest)_:
--1 InvestmentFlowBlock_invest(electricityBus_sink_nonconvex_invest)
-+15 InvestmentFlowBlock_invest_status(electricityBus_sink_nonconvex_invest)
+c_u_InvestmentFlowBlock_minimum_rule(electricityBus_sink_nonconvex_invest_0)_:
+-1 InvestmentFlowBlock_invest(electricityBus_sink_nonconvex_invest_0)
++15 InvestmentFlowBlock_invest_status(electricityBus_sink_nonconvex_invest_0)
 <= 0
 
-c_u_InvestmentFlowBlock_maximum_rule(electricityBus_sink_nonconvex_invest)_:
-+1 InvestmentFlowBlock_invest(electricityBus_sink_nonconvex_invest)
--172 InvestmentFlowBlock_invest_status(electricityBus_sink_nonconvex_invest)
+c_u_InvestmentFlowBlock_maximum_rule(electricityBus_sink_nonconvex_invest_0)_:
++1 InvestmentFlowBlock_invest(electricityBus_sink_nonconvex_invest_0)
+-172 InvestmentFlowBlock_invest_status(electricityBus_sink_nonconvex_invest_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(electricityBus_sink_nonconvex_invest_0)_:
--0.80000000000000004 InvestmentFlowBlock_invest(electricityBus_sink_nonconvex_invest)
-+1 flow(electricityBus_sink_nonconvex_invest_0)
+c_e_InvestmentFlowBlock_total_rule(electricityBus_sink_nonconvex_invest_0)_:
+-1 InvestmentFlowBlock_invest(electricityBus_sink_nonconvex_invest_0)
++1 InvestmentFlowBlock_total(electricityBus_sink_nonconvex_invest_0)
+= 0
+
+c_u_InvestmentFlowBlock_max(electricityBus_sink_nonconvex_invest_0_0)_:
++1 flow(electricityBus_sink_nonconvex_invest_0_0)
+-0.8 InvestmentFlowBlock_total(electricityBus_sink_nonconvex_invest_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(electricityBus_sink_nonconvex_invest_1)_:
--0.80000000000000004 InvestmentFlowBlock_invest(electricityBus_sink_nonconvex_invest)
-+1 flow(electricityBus_sink_nonconvex_invest_1)
+c_u_InvestmentFlowBlock_max(electricityBus_sink_nonconvex_invest_0_1)_:
++1 flow(electricityBus_sink_nonconvex_invest_0_1)
+-0.8 InvestmentFlowBlock_total(electricityBus_sink_nonconvex_invest_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(electricityBus_sink_nonconvex_invest_2)_:
--0.80000000000000004 InvestmentFlowBlock_invest(electricityBus_sink_nonconvex_invest)
-+1 flow(electricityBus_sink_nonconvex_invest_2)
+c_u_InvestmentFlowBlock_max(electricityBus_sink_nonconvex_invest_0_2)_:
++1 flow(electricityBus_sink_nonconvex_invest_0_2)
+-0.8 InvestmentFlowBlock_total(electricityBus_sink_nonconvex_invest_0)
 <= 0
 
 c_u_InvestmentFlowBlock_full_load_time_max(electricityBus_sink_nonconvex_invest)_:
--2.2999999999999998 InvestmentFlowBlock_invest(electricityBus_sink_nonconvex_invest)
-+1 flow(electricityBus_sink_nonconvex_invest_0)
-+1 flow(electricityBus_sink_nonconvex_invest_1)
-+1 flow(electricityBus_sink_nonconvex_invest_2)
++1 flow(electricityBus_sink_nonconvex_invest_0_0)
++1 flow(electricityBus_sink_nonconvex_invest_0_1)
++1 flow(electricityBus_sink_nonconvex_invest_0_2)
+-2.3 InvestmentFlowBlock_total(electricityBus_sink_nonconvex_invest_0)
 <= 0
 
-c_e_ONE_VAR_CONSTANT: 
-ONE_VAR_CONSTANT = 1.0
-
 bounds
-   0 <= flow(electricityBus_sink_nonconvex_invest_0) <= +inf
-   0 <= flow(electricityBus_sink_nonconvex_invest_1) <= +inf
-   0 <= flow(electricityBus_sink_nonconvex_invest_2) <= +inf
-   0 <= InvestmentFlowBlock_invest(electricityBus_sink_nonconvex_invest) <= 172
-   0 <= InvestmentFlowBlock_invest_status(electricityBus_sink_nonconvex_invest) <= 1
+   0 <= InvestmentFlowBlock_invest(electricityBus_sink_nonconvex_invest_0) <= 172
+   0 <= flow(electricityBus_sink_nonconvex_invest_0_0) <= +inf
+   0 <= flow(electricityBus_sink_nonconvex_invest_0_1) <= +inf
+   0 <= flow(electricityBus_sink_nonconvex_invest_0_2) <= +inf
+   0 <= InvestmentFlowBlock_invest_status(electricityBus_sink_nonconvex_invest_0) <= 1
+   0 <= InvestmentFlowBlock_total(electricityBus_sink_nonconvex_invest_0) <= +inf
 binary
-  InvestmentFlowBlock_invest_status(electricityBus_sink_nonconvex_invest)
+  InvestmentFlowBlock_invest_status(electricityBus_sink_nonconvex_invest_0)
 end
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/flow_nonconvex_invest_bounded_transformer.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/flow_nonconvex_invest_bounded_transformer.lp`

 * *Files 3% similar despite different names*

```diff
@@ -1,158 +1,155 @@
 \* Source Pyomo model name=Model *\
 
-min
+min 
 objective:
-+500 InvestNonConvexFlowBlock_invest(transformer_nonconvex_invest_electricityBus)
-+25 flow(transformer_nonconvex_invest_electricityBus_0)
-+25 flow(transformer_nonconvex_invest_electricityBus_1)
-+25 flow(transformer_nonconvex_invest_electricityBus_2)
++25 flow(transformer_nonconvex_invest_electricityBus_0_0)
++25 flow(transformer_nonconvex_invest_electricityBus_0_1)
++25 flow(transformer_nonconvex_invest_electricityBus_0_2)
++500 InvestNonConvexFlowBlock_invest(transformer_nonconvex_invest_electricityBus_0)
 
 s.t.
 
-c_e_BusBlock_balance(electricityBus_0)_:
-+1 flow(transformer_nonconvex_invest_electricityBus_0)
+c_e_BusBlock_balance(electricityBus_0_0)_:
++1 flow(transformer_nonconvex_invest_electricityBus_0_0)
 = 0
 
-c_e_BusBlock_balance(electricityBus_1)_:
-+1 flow(transformer_nonconvex_invest_electricityBus_1)
+c_e_BusBlock_balance(electricityBus_0_1)_:
++1 flow(transformer_nonconvex_invest_electricityBus_0_1)
 = 0
 
-c_e_BusBlock_balance(electricityBus_2)_:
-+1 flow(transformer_nonconvex_invest_electricityBus_2)
+c_e_BusBlock_balance(electricityBus_0_2)_:
++1 flow(transformer_nonconvex_invest_electricityBus_0_2)
 = 0
 
-c_e_BusBlock_balance(fuelBus_0)_:
-+1 flow(fuelBus_transformer_nonconvex_invest_0)
+c_e_BusBlock_balance(fuelBus_0_0)_:
++1 flow(fuelBus_transformer_nonconvex_invest_0_0)
 = 0
 
-c_e_BusBlock_balance(fuelBus_1)_:
-+1 flow(fuelBus_transformer_nonconvex_invest_1)
+c_e_BusBlock_balance(fuelBus_0_1)_:
++1 flow(fuelBus_transformer_nonconvex_invest_0_1)
 = 0
 
-c_e_BusBlock_balance(fuelBus_2)_:
-+1 flow(fuelBus_transformer_nonconvex_invest_2)
+c_e_BusBlock_balance(fuelBus_0_2)_:
++1 flow(fuelBus_transformer_nonconvex_invest_0_2)
 = 0
 
-c_e_TransformerBlock_relation(transformer_nonconvex_invest_fuelBus_electricityBus_0)_:
-+0.5 flow(fuelBus_transformer_nonconvex_invest_0)
--1 flow(transformer_nonconvex_invest_electricityBus_0)
+c_e_TransformerBlock_relation(transformer_nonconvex_invest_fuelBus_electricityBus_0_0)_:
+-1 flow(transformer_nonconvex_invest_electricityBus_0_0)
++0.5 flow(fuelBus_transformer_nonconvex_invest_0_0)
 = 0
 
-c_e_TransformerBlock_relation(transformer_nonconvex_invest_fuelBus_electricityBus_1)_:
-+0.5 flow(fuelBus_transformer_nonconvex_invest_1)
--1 flow(transformer_nonconvex_invest_electricityBus_1)
+c_e_TransformerBlock_relation(transformer_nonconvex_invest_fuelBus_electricityBus_0_1)_:
+-1 flow(transformer_nonconvex_invest_electricityBus_0_1)
++0.5 flow(fuelBus_transformer_nonconvex_invest_0_1)
 = 0
 
-c_e_TransformerBlock_relation(transformer_nonconvex_invest_fuelBus_electricityBus_2)_:
-+0.5 flow(fuelBus_transformer_nonconvex_invest_2)
--1 flow(transformer_nonconvex_invest_electricityBus_2)
+c_e_TransformerBlock_relation(transformer_nonconvex_invest_fuelBus_electricityBus_0_2)_:
+-1 flow(transformer_nonconvex_invest_electricityBus_0_2)
++0.5 flow(fuelBus_transformer_nonconvex_invest_0_2)
 = 0
 
-c_l_InvestNonConvexFlowBlock_minimum_investment(transformer_nonconvex_invest_electricityBus)_:
-+1 InvestNonConvexFlowBlock_invest(transformer_nonconvex_invest_electricityBus)
+c_l_InvestNonConvexFlowBlock_minimum_investment(transformer_nonconvex_invest_electricityBus_0)_:
++1 InvestNonConvexFlowBlock_invest(transformer_nonconvex_invest_electricityBus_0)
 >= 0
 
-c_u_InvestNonConvexFlowBlock_maximum_investment(transformer_nonconvex_invest_electricityBus)_:
-+1 InvestNonConvexFlowBlock_invest(transformer_nonconvex_invest_electricityBus)
+c_u_InvestNonConvexFlowBlock_maximum_investment(transformer_nonconvex_invest_electricityBus_0)_:
++1 InvestNonConvexFlowBlock_invest(transformer_nonconvex_invest_electricityBus_0)
 <= 1234
 
-c_u_InvestNonConvexFlowBlock_min(transformer_nonconvex_invest_electricityBus_0)_:
+c_u_InvestNonConvexFlowBlock_min(transformer_nonconvex_invest_electricityBus_0_0)_:
+-1 flow(transformer_nonconvex_invest_electricityBus_0_0)
 +0.25 InvestNonConvexFlowBlock_status_nominal(transformer_nonconvex_invest_electricityBus_0)
--1 flow(transformer_nonconvex_invest_electricityBus_0)
 <= 0
 
-c_u_InvestNonConvexFlowBlock_min(transformer_nonconvex_invest_electricityBus_1)_:
+c_u_InvestNonConvexFlowBlock_min(transformer_nonconvex_invest_electricityBus_0_1)_:
+-1 flow(transformer_nonconvex_invest_electricityBus_0_1)
 +0.25 InvestNonConvexFlowBlock_status_nominal(transformer_nonconvex_invest_electricityBus_1)
--1 flow(transformer_nonconvex_invest_electricityBus_1)
 <= 0
 
-c_u_InvestNonConvexFlowBlock_min(transformer_nonconvex_invest_electricityBus_2)_:
+c_u_InvestNonConvexFlowBlock_min(transformer_nonconvex_invest_electricityBus_0_2)_:
+-1 flow(transformer_nonconvex_invest_electricityBus_0_2)
 +0.25 InvestNonConvexFlowBlock_status_nominal(transformer_nonconvex_invest_electricityBus_2)
--1 flow(transformer_nonconvex_invest_electricityBus_2)
 <= 0
 
-c_u_InvestNonConvexFlowBlock_max(transformer_nonconvex_invest_electricityBus_0)_:
+c_u_InvestNonConvexFlowBlock_max(transformer_nonconvex_invest_electricityBus_0_0)_:
++1 flow(transformer_nonconvex_invest_electricityBus_0_0)
 -0.5 InvestNonConvexFlowBlock_status_nominal(transformer_nonconvex_invest_electricityBus_0)
-+1 flow(transformer_nonconvex_invest_electricityBus_0)
 <= 0
 
-c_u_InvestNonConvexFlowBlock_max(transformer_nonconvex_invest_electricityBus_1)_:
+c_u_InvestNonConvexFlowBlock_max(transformer_nonconvex_invest_electricityBus_0_1)_:
++1 flow(transformer_nonconvex_invest_electricityBus_0_1)
 -0.5 InvestNonConvexFlowBlock_status_nominal(transformer_nonconvex_invest_electricityBus_1)
-+1 flow(transformer_nonconvex_invest_electricityBus_1)
 <= 0
 
-c_u_InvestNonConvexFlowBlock_max(transformer_nonconvex_invest_electricityBus_2)_:
+c_u_InvestNonConvexFlowBlock_max(transformer_nonconvex_invest_electricityBus_0_2)_:
++1 flow(transformer_nonconvex_invest_electricityBus_0_2)
 -0.5 InvestNonConvexFlowBlock_status_nominal(transformer_nonconvex_invest_electricityBus_2)
-+1 flow(transformer_nonconvex_invest_electricityBus_2)
 <= 0
 
-c_u_InvestNonConvexFlowBlock_invest_nc_one(transformer_nonconvex_invest_electricityBus_0)_:
--1234 InvestNonConvexFlowBlock_status(transformer_nonconvex_invest_electricityBus_0)
+c_u_InvestNonConvexFlowBlock_invest_nc_one(transformer_nonconvex_invest_electricityBus_0_0)_:
 +1 InvestNonConvexFlowBlock_status_nominal(transformer_nonconvex_invest_electricityBus_0)
+-1234 InvestNonConvexFlowBlock_status(transformer_nonconvex_invest_electricityBus_0)
 <= 0
 
-c_u_InvestNonConvexFlowBlock_invest_nc_one(transformer_nonconvex_invest_electricityBus_1)_:
--1234 InvestNonConvexFlowBlock_status(transformer_nonconvex_invest_electricityBus_1)
+c_u_InvestNonConvexFlowBlock_invest_nc_one(transformer_nonconvex_invest_electricityBus_0_1)_:
 +1 InvestNonConvexFlowBlock_status_nominal(transformer_nonconvex_invest_electricityBus_1)
+-1234 InvestNonConvexFlowBlock_status(transformer_nonconvex_invest_electricityBus_1)
 <= 0
 
-c_u_InvestNonConvexFlowBlock_invest_nc_one(transformer_nonconvex_invest_electricityBus_2)_:
--1234 InvestNonConvexFlowBlock_status(transformer_nonconvex_invest_electricityBus_2)
+c_u_InvestNonConvexFlowBlock_invest_nc_one(transformer_nonconvex_invest_electricityBus_0_2)_:
 +1 InvestNonConvexFlowBlock_status_nominal(transformer_nonconvex_invest_electricityBus_2)
+-1234 InvestNonConvexFlowBlock_status(transformer_nonconvex_invest_electricityBus_2)
 <= 0
 
-c_u_InvestNonConvexFlowBlock_invest_nc_two(transformer_nonconvex_invest_electricityBus_0)_:
--1 InvestNonConvexFlowBlock_invest(transformer_nonconvex_invest_electricityBus)
+c_u_InvestNonConvexFlowBlock_invest_nc_two(transformer_nonconvex_invest_electricityBus_0_0)_:
+-1 InvestNonConvexFlowBlock_invest(transformer_nonconvex_invest_electricityBus_0)
 +1 InvestNonConvexFlowBlock_status_nominal(transformer_nonconvex_invest_electricityBus_0)
 <= 0
 
-c_u_InvestNonConvexFlowBlock_invest_nc_two(transformer_nonconvex_invest_electricityBus_1)_:
--1 InvestNonConvexFlowBlock_invest(transformer_nonconvex_invest_electricityBus)
+c_u_InvestNonConvexFlowBlock_invest_nc_two(transformer_nonconvex_invest_electricityBus_0_1)_:
+-1 InvestNonConvexFlowBlock_invest(transformer_nonconvex_invest_electricityBus_0)
 +1 InvestNonConvexFlowBlock_status_nominal(transformer_nonconvex_invest_electricityBus_1)
 <= 0
 
-c_u_InvestNonConvexFlowBlock_invest_nc_two(transformer_nonconvex_invest_electricityBus_2)_:
--1 InvestNonConvexFlowBlock_invest(transformer_nonconvex_invest_electricityBus)
+c_u_InvestNonConvexFlowBlock_invest_nc_two(transformer_nonconvex_invest_electricityBus_0_2)_:
+-1 InvestNonConvexFlowBlock_invest(transformer_nonconvex_invest_electricityBus_0)
 +1 InvestNonConvexFlowBlock_status_nominal(transformer_nonconvex_invest_electricityBus_2)
 <= 0
 
-c_u_InvestNonConvexFlowBlock_invest_nc_three(transformer_nonconvex_invest_electricityBus_0)_:
-+1 InvestNonConvexFlowBlock_invest(transformer_nonconvex_invest_electricityBus)
-+1234 InvestNonConvexFlowBlock_status(transformer_nonconvex_invest_electricityBus_0)
+c_u_InvestNonConvexFlowBlock_invest_nc_three(transformer_nonconvex_invest_electricityBus_0_0)_:
++1 InvestNonConvexFlowBlock_invest(transformer_nonconvex_invest_electricityBus_0)
 -1 InvestNonConvexFlowBlock_status_nominal(transformer_nonconvex_invest_electricityBus_0)
++1234 InvestNonConvexFlowBlock_status(transformer_nonconvex_invest_electricityBus_0)
 <= 1234
 
-c_u_InvestNonConvexFlowBlock_invest_nc_three(transformer_nonconvex_invest_electricityBus_1)_:
-+1 InvestNonConvexFlowBlock_invest(transformer_nonconvex_invest_electricityBus)
-+1234 InvestNonConvexFlowBlock_status(transformer_nonconvex_invest_electricityBus_1)
+c_u_InvestNonConvexFlowBlock_invest_nc_three(transformer_nonconvex_invest_electricityBus_0_1)_:
++1 InvestNonConvexFlowBlock_invest(transformer_nonconvex_invest_electricityBus_0)
 -1 InvestNonConvexFlowBlock_status_nominal(transformer_nonconvex_invest_electricityBus_1)
++1234 InvestNonConvexFlowBlock_status(transformer_nonconvex_invest_electricityBus_1)
 <= 1234
 
-c_u_InvestNonConvexFlowBlock_invest_nc_three(transformer_nonconvex_invest_electricityBus_2)_:
-+1 InvestNonConvexFlowBlock_invest(transformer_nonconvex_invest_electricityBus)
-+1234 InvestNonConvexFlowBlock_status(transformer_nonconvex_invest_electricityBus_2)
+c_u_InvestNonConvexFlowBlock_invest_nc_three(transformer_nonconvex_invest_electricityBus_0_2)_:
++1 InvestNonConvexFlowBlock_invest(transformer_nonconvex_invest_electricityBus_0)
 -1 InvestNonConvexFlowBlock_status_nominal(transformer_nonconvex_invest_electricityBus_2)
++1234 InvestNonConvexFlowBlock_status(transformer_nonconvex_invest_electricityBus_2)
 <= 1234
 
-c_e_ONE_VAR_CONSTANT:
-ONE_VAR_CONSTANT = 1.0
-
 bounds
-   0 <= flow(fuelBus_transformer_nonconvex_invest_0) <= +inf
-   0 <= flow(fuelBus_transformer_nonconvex_invest_1) <= +inf
-   0 <= flow(fuelBus_transformer_nonconvex_invest_2) <= +inf
-   0 <= flow(transformer_nonconvex_invest_electricityBus_0) <= +inf
-   0 <= flow(transformer_nonconvex_invest_electricityBus_1) <= +inf
-   0 <= flow(transformer_nonconvex_invest_electricityBus_2) <= +inf
-   0 <= InvestNonConvexFlowBlock_status(transformer_nonconvex_invest_electricityBus_0) <= 1
-   0 <= InvestNonConvexFlowBlock_status(transformer_nonconvex_invest_electricityBus_1) <= 1
-   0 <= InvestNonConvexFlowBlock_status(transformer_nonconvex_invest_electricityBus_2) <= 1
-   0 <= InvestNonConvexFlowBlock_invest(transformer_nonconvex_invest_electricityBus) <= 1234
+   0 <= flow(transformer_nonconvex_invest_electricityBus_0_0) <= +inf
+   0 <= flow(transformer_nonconvex_invest_electricityBus_0_1) <= +inf
+   0 <= flow(transformer_nonconvex_invest_electricityBus_0_2) <= +inf
+   0 <= InvestNonConvexFlowBlock_invest(transformer_nonconvex_invest_electricityBus_0) <= 1234
+   0 <= flow(fuelBus_transformer_nonconvex_invest_0_0) <= +inf
+   0 <= flow(fuelBus_transformer_nonconvex_invest_0_1) <= +inf
+   0 <= flow(fuelBus_transformer_nonconvex_invest_0_2) <= +inf
    0 <= InvestNonConvexFlowBlock_status_nominal(transformer_nonconvex_invest_electricityBus_0) <= +inf
    0 <= InvestNonConvexFlowBlock_status_nominal(transformer_nonconvex_invest_electricityBus_1) <= +inf
    0 <= InvestNonConvexFlowBlock_status_nominal(transformer_nonconvex_invest_electricityBus_2) <= +inf
+   0 <= InvestNonConvexFlowBlock_status(transformer_nonconvex_invest_electricityBus_0) <= 1
+   0 <= InvestNonConvexFlowBlock_status(transformer_nonconvex_invest_electricityBus_1) <= 1
+   0 <= InvestNonConvexFlowBlock_status(transformer_nonconvex_invest_electricityBus_2) <= 1
 binary
   InvestNonConvexFlowBlock_status(transformer_nonconvex_invest_electricityBus_0)
   InvestNonConvexFlowBlock_status(transformer_nonconvex_invest_electricityBus_1)
   InvestNonConvexFlowBlock_status(transformer_nonconvex_invest_electricityBus_2)
 end
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/inactivity_costs.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/inactivity_costs.lp`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 \* Source Pyomo model name=Model *\
 
-min
+min 
 objective:
++6 ONE_VAR_CONSTANT
++10 flow(cheap_plant_inactivity_costs_Bus_C_0_0)
++10 flow(cheap_plant_inactivity_costs_Bus_C_0_1)
++10 flow(cheap_plant_inactivity_costs_Bus_C_0_2)
 -2 NonConvexFlowBlock_status(cheap_plant_inactivity_costs_Bus_C_0)
 -2 NonConvexFlowBlock_status(cheap_plant_inactivity_costs_Bus_C_1)
 -2 NonConvexFlowBlock_status(cheap_plant_inactivity_costs_Bus_C_2)
-+10 flow(cheap_plant_inactivity_costs_Bus_C_0)
-+10 flow(cheap_plant_inactivity_costs_Bus_C_1)
-+10 flow(cheap_plant_inactivity_costs_Bus_C_2)
-+6 ONE_VAR_CONSTANT
 
 s.t.
 
-c_e_BusBlock_balance(Bus_C_0)_:
-+1 flow(cheap_plant_inactivity_costs_Bus_C_0)
+c_e_BusBlock_balance(Bus_C_0_0)_:
++1 flow(cheap_plant_inactivity_costs_Bus_C_0_0)
 = 0
 
-c_e_BusBlock_balance(Bus_C_1)_:
-+1 flow(cheap_plant_inactivity_costs_Bus_C_1)
+c_e_BusBlock_balance(Bus_C_0_1)_:
++1 flow(cheap_plant_inactivity_costs_Bus_C_0_1)
 = 0
 
-c_e_BusBlock_balance(Bus_C_2)_:
-+1 flow(cheap_plant_inactivity_costs_Bus_C_2)
+c_e_BusBlock_balance(Bus_C_0_2)_:
++1 flow(cheap_plant_inactivity_costs_Bus_C_0_2)
 = 0
 
 c_e_NonConvexFlowBlock_status_nominal_constraint(cheap_plant_inactivity_costs_Bus_C_0)_:
 -10 NonConvexFlowBlock_status(cheap_plant_inactivity_costs_Bus_C_0)
 +1 NonConvexFlowBlock_status_nominal(cheap_plant_inactivity_costs_Bus_C_0)
 = 0
 
@@ -35,51 +35,49 @@
 = 0
 
 c_e_NonConvexFlowBlock_status_nominal_constraint(cheap_plant_inactivity_costs_Bus_C_2)_:
 -10 NonConvexFlowBlock_status(cheap_plant_inactivity_costs_Bus_C_2)
 +1 NonConvexFlowBlock_status_nominal(cheap_plant_inactivity_costs_Bus_C_2)
 = 0
 
-c_u_NonConvexFlowBlock_min(cheap_plant_inactivity_costs_Bus_C_0)_:
+c_u_NonConvexFlowBlock_min(cheap_plant_inactivity_costs_Bus_C_0_0)_:
+-1 flow(cheap_plant_inactivity_costs_Bus_C_0_0)
 +0.5 NonConvexFlowBlock_status_nominal(cheap_plant_inactivity_costs_Bus_C_0)
--1 flow(cheap_plant_inactivity_costs_Bus_C_0)
 <= 0
 
-c_u_NonConvexFlowBlock_min(cheap_plant_inactivity_costs_Bus_C_1)_:
+c_u_NonConvexFlowBlock_min(cheap_plant_inactivity_costs_Bus_C_0_1)_:
+-1 flow(cheap_plant_inactivity_costs_Bus_C_0_1)
 +0.5 NonConvexFlowBlock_status_nominal(cheap_plant_inactivity_costs_Bus_C_1)
--1 flow(cheap_plant_inactivity_costs_Bus_C_1)
 <= 0
 
-c_u_NonConvexFlowBlock_min(cheap_plant_inactivity_costs_Bus_C_2)_:
+c_u_NonConvexFlowBlock_min(cheap_plant_inactivity_costs_Bus_C_0_2)_:
+-1 flow(cheap_plant_inactivity_costs_Bus_C_0_2)
 +0.5 NonConvexFlowBlock_status_nominal(cheap_plant_inactivity_costs_Bus_C_2)
--1 flow(cheap_plant_inactivity_costs_Bus_C_2)
 <= 0
 
-c_u_NonConvexFlowBlock_max(cheap_plant_inactivity_costs_Bus_C_0)_:
+c_u_NonConvexFlowBlock_max(cheap_plant_inactivity_costs_Bus_C_0_0)_:
++1 flow(cheap_plant_inactivity_costs_Bus_C_0_0)
 -1 NonConvexFlowBlock_status_nominal(cheap_plant_inactivity_costs_Bus_C_0)
-+1 flow(cheap_plant_inactivity_costs_Bus_C_0)
 <= 0
 
-c_u_NonConvexFlowBlock_max(cheap_plant_inactivity_costs_Bus_C_1)_:
+c_u_NonConvexFlowBlock_max(cheap_plant_inactivity_costs_Bus_C_0_1)_:
++1 flow(cheap_plant_inactivity_costs_Bus_C_0_1)
 -1 NonConvexFlowBlock_status_nominal(cheap_plant_inactivity_costs_Bus_C_1)
-+1 flow(cheap_plant_inactivity_costs_Bus_C_1)
 <= 0
 
-c_u_NonConvexFlowBlock_max(cheap_plant_inactivity_costs_Bus_C_2)_:
+c_u_NonConvexFlowBlock_max(cheap_plant_inactivity_costs_Bus_C_0_2)_:
++1 flow(cheap_plant_inactivity_costs_Bus_C_0_2)
 -1 NonConvexFlowBlock_status_nominal(cheap_plant_inactivity_costs_Bus_C_2)
-+1 flow(cheap_plant_inactivity_costs_Bus_C_2)
 <= 0
 
-c_e_ONE_VAR_CONSTANT:
-ONE_VAR_CONSTANT = 1.0
-
 bounds
-   0 <= flow(cheap_plant_inactivity_costs_Bus_C_0) <= 10
-   0 <= flow(cheap_plant_inactivity_costs_Bus_C_1) <= 10
-   0 <= flow(cheap_plant_inactivity_costs_Bus_C_2) <= 10
+   1 <= ONE_VAR_CONSTANT <= 1
+   0 <= flow(cheap_plant_inactivity_costs_Bus_C_0_0) <= 10.0
+   0 <= flow(cheap_plant_inactivity_costs_Bus_C_0_1) <= 10.0
+   0 <= flow(cheap_plant_inactivity_costs_Bus_C_0_2) <= 10.0
    0 <= NonConvexFlowBlock_status(cheap_plant_inactivity_costs_Bus_C_0) <= 1
    0 <= NonConvexFlowBlock_status(cheap_plant_inactivity_costs_Bus_C_1) <= 1
    0 <= NonConvexFlowBlock_status(cheap_plant_inactivity_costs_Bus_C_2) <= 1
    0 <= NonConvexFlowBlock_status_nominal(cheap_plant_inactivity_costs_Bus_C_0) <= +inf
    0 <= NonConvexFlowBlock_status_nominal(cheap_plant_inactivity_costs_Bus_C_1) <= +inf
    0 <= NonConvexFlowBlock_status_nominal(cheap_plant_inactivity_costs_Bus_C_2) <= +inf
 binary
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/invest_non_convex_flow.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/invest_non_convex_flow.lp`

 * *Files 15% similar despite different names*

```diff
@@ -1,149 +1,146 @@
 \* Source Pyomo model name=Model *\
 
-min
+min 
 objective:
-+0.75 InvestNonConvexFlowBlock_invest(b1_b2)
-+8 flow(b1_b2_0)
-+8 flow(b1_b2_1)
-+8 flow(b1_b2_2)
++8 flow(b1_b2_0_0)
++8 flow(b1_b2_0_1)
++8 flow(b1_b2_0_2)
++0.75 InvestNonConvexFlowBlock_invest(b1_b2_0)
 
 s.t.
 
-c_e_BusBlock_balance(b1_0)_:
--1 flow(b1_b2_0)
-+1 flow(b2_b1_0)
+c_e_BusBlock_balance(b2_0_0)_:
++1 flow(b1_b2_0_0)
+-1 flow(b2_b1_0_0)
 = 0
 
-c_e_BusBlock_balance(b1_1)_:
--1 flow(b1_b2_1)
-+1 flow(b2_b1_1)
+c_e_BusBlock_balance(b2_0_1)_:
++1 flow(b1_b2_0_1)
+-1 flow(b2_b1_0_1)
 = 0
 
-c_e_BusBlock_balance(b1_2)_:
--1 flow(b1_b2_2)
-+1 flow(b2_b1_2)
+c_e_BusBlock_balance(b2_0_2)_:
++1 flow(b1_b2_0_2)
+-1 flow(b2_b1_0_2)
 = 0
 
-c_e_BusBlock_balance(b2_0)_:
-+1 flow(b1_b2_0)
--1 flow(b2_b1_0)
+c_e_BusBlock_balance(b1_0_0)_:
+-1 flow(b1_b2_0_0)
++1 flow(b2_b1_0_0)
 = 0
 
-c_e_BusBlock_balance(b2_1)_:
-+1 flow(b1_b2_1)
--1 flow(b2_b1_1)
+c_e_BusBlock_balance(b1_0_1)_:
+-1 flow(b1_b2_0_1)
++1 flow(b2_b1_0_1)
 = 0
 
-c_e_BusBlock_balance(b2_2)_:
-+1 flow(b1_b2_2)
--1 flow(b2_b1_2)
+c_e_BusBlock_balance(b1_0_2)_:
+-1 flow(b1_b2_0_2)
++1 flow(b2_b1_0_2)
 = 0
 
-c_l_InvestNonConvexFlowBlock_minimum_investment(b1_b2)_:
-+1 InvestNonConvexFlowBlock_invest(b1_b2)
+c_l_InvestNonConvexFlowBlock_minimum_investment(b1_b2_0)_:
++1 InvestNonConvexFlowBlock_invest(b1_b2_0)
 >= 0
 
-c_u_InvestNonConvexFlowBlock_maximum_investment(b1_b2)_:
-+1 InvestNonConvexFlowBlock_invest(b1_b2)
+c_u_InvestNonConvexFlowBlock_maximum_investment(b1_b2_0)_:
++1 InvestNonConvexFlowBlock_invest(b1_b2_0)
 <= 10
 
-c_u_InvestNonConvexFlowBlock_min(b1_b2_0)_:
+c_u_InvestNonConvexFlowBlock_min(b1_b2_0_0)_:
+-1 flow(b1_b2_0_0)
 +0.25 InvestNonConvexFlowBlock_status_nominal(b1_b2_0)
--1 flow(b1_b2_0)
 <= 0
 
-c_u_InvestNonConvexFlowBlock_min(b1_b2_1)_:
+c_u_InvestNonConvexFlowBlock_min(b1_b2_0_1)_:
+-1 flow(b1_b2_0_1)
 +0.25 InvestNonConvexFlowBlock_status_nominal(b1_b2_1)
--1 flow(b1_b2_1)
 <= 0
 
-c_u_InvestNonConvexFlowBlock_min(b1_b2_2)_:
+c_u_InvestNonConvexFlowBlock_min(b1_b2_0_2)_:
+-1 flow(b1_b2_0_2)
 +0.25 InvestNonConvexFlowBlock_status_nominal(b1_b2_2)
--1 flow(b1_b2_2)
 <= 0
 
-c_u_InvestNonConvexFlowBlock_max(b1_b2_0)_:
+c_u_InvestNonConvexFlowBlock_max(b1_b2_0_0)_:
++1 flow(b1_b2_0_0)
 -0.5 InvestNonConvexFlowBlock_status_nominal(b1_b2_0)
-+1 flow(b1_b2_0)
 <= 0
 
-c_u_InvestNonConvexFlowBlock_max(b1_b2_1)_:
+c_u_InvestNonConvexFlowBlock_max(b1_b2_0_1)_:
++1 flow(b1_b2_0_1)
 -0.5 InvestNonConvexFlowBlock_status_nominal(b1_b2_1)
-+1 flow(b1_b2_1)
 <= 0
 
-c_u_InvestNonConvexFlowBlock_max(b1_b2_2)_:
+c_u_InvestNonConvexFlowBlock_max(b1_b2_0_2)_:
++1 flow(b1_b2_0_2)
 -0.5 InvestNonConvexFlowBlock_status_nominal(b1_b2_2)
-+1 flow(b1_b2_2)
 <= 0
 
-c_u_InvestNonConvexFlowBlock_invest_nc_one(b1_b2_0)_:
--10 InvestNonConvexFlowBlock_status(b1_b2_0)
+c_u_InvestNonConvexFlowBlock_invest_nc_one(b1_b2_0_0)_:
 +1 InvestNonConvexFlowBlock_status_nominal(b1_b2_0)
+-10 InvestNonConvexFlowBlock_status(b1_b2_0)
 <= 0
 
-c_u_InvestNonConvexFlowBlock_invest_nc_one(b1_b2_1)_:
--10 InvestNonConvexFlowBlock_status(b1_b2_1)
+c_u_InvestNonConvexFlowBlock_invest_nc_one(b1_b2_0_1)_:
 +1 InvestNonConvexFlowBlock_status_nominal(b1_b2_1)
+-10 InvestNonConvexFlowBlock_status(b1_b2_1)
 <= 0
 
-c_u_InvestNonConvexFlowBlock_invest_nc_one(b1_b2_2)_:
--10 InvestNonConvexFlowBlock_status(b1_b2_2)
+c_u_InvestNonConvexFlowBlock_invest_nc_one(b1_b2_0_2)_:
 +1 InvestNonConvexFlowBlock_status_nominal(b1_b2_2)
+-10 InvestNonConvexFlowBlock_status(b1_b2_2)
 <= 0
 
-c_u_InvestNonConvexFlowBlock_invest_nc_two(b1_b2_0)_:
--1 InvestNonConvexFlowBlock_invest(b1_b2)
+c_u_InvestNonConvexFlowBlock_invest_nc_two(b1_b2_0_0)_:
+-1 InvestNonConvexFlowBlock_invest(b1_b2_0)
 +1 InvestNonConvexFlowBlock_status_nominal(b1_b2_0)
 <= 0
 
-c_u_InvestNonConvexFlowBlock_invest_nc_two(b1_b2_1)_:
--1 InvestNonConvexFlowBlock_invest(b1_b2)
+c_u_InvestNonConvexFlowBlock_invest_nc_two(b1_b2_0_1)_:
+-1 InvestNonConvexFlowBlock_invest(b1_b2_0)
 +1 InvestNonConvexFlowBlock_status_nominal(b1_b2_1)
 <= 0
 
-c_u_InvestNonConvexFlowBlock_invest_nc_two(b1_b2_2)_:
--1 InvestNonConvexFlowBlock_invest(b1_b2)
+c_u_InvestNonConvexFlowBlock_invest_nc_two(b1_b2_0_2)_:
+-1 InvestNonConvexFlowBlock_invest(b1_b2_0)
 +1 InvestNonConvexFlowBlock_status_nominal(b1_b2_2)
 <= 0
 
-c_u_InvestNonConvexFlowBlock_invest_nc_three(b1_b2_0)_:
-+1 InvestNonConvexFlowBlock_invest(b1_b2)
-+10 InvestNonConvexFlowBlock_status(b1_b2_0)
+c_u_InvestNonConvexFlowBlock_invest_nc_three(b1_b2_0_0)_:
++1 InvestNonConvexFlowBlock_invest(b1_b2_0)
 -1 InvestNonConvexFlowBlock_status_nominal(b1_b2_0)
++10 InvestNonConvexFlowBlock_status(b1_b2_0)
 <= 10
 
-c_u_InvestNonConvexFlowBlock_invest_nc_three(b1_b2_1)_:
-+1 InvestNonConvexFlowBlock_invest(b1_b2)
-+10 InvestNonConvexFlowBlock_status(b1_b2_1)
+c_u_InvestNonConvexFlowBlock_invest_nc_three(b1_b2_0_1)_:
++1 InvestNonConvexFlowBlock_invest(b1_b2_0)
 -1 InvestNonConvexFlowBlock_status_nominal(b1_b2_1)
++10 InvestNonConvexFlowBlock_status(b1_b2_1)
 <= 10
 
-c_u_InvestNonConvexFlowBlock_invest_nc_three(b1_b2_2)_:
-+1 InvestNonConvexFlowBlock_invest(b1_b2)
-+10 InvestNonConvexFlowBlock_status(b1_b2_2)
+c_u_InvestNonConvexFlowBlock_invest_nc_three(b1_b2_0_2)_:
++1 InvestNonConvexFlowBlock_invest(b1_b2_0)
 -1 InvestNonConvexFlowBlock_status_nominal(b1_b2_2)
++10 InvestNonConvexFlowBlock_status(b1_b2_2)
 <= 10
 
-c_e_ONE_VAR_CONSTANT:
-ONE_VAR_CONSTANT = 1.0
-
 bounds
-   0 <= flow(b1_b2_0) <= +inf
-   0 <= flow(b1_b2_1) <= +inf
-   0 <= flow(b1_b2_2) <= +inf
-   0 <= flow(b2_b1_0) <= +inf
-   0 <= flow(b2_b1_1) <= +inf
-   0 <= flow(b2_b1_2) <= +inf
-   0 <= InvestNonConvexFlowBlock_status(b1_b2_0) <= 1
-   0 <= InvestNonConvexFlowBlock_status(b1_b2_1) <= 1
-   0 <= InvestNonConvexFlowBlock_status(b1_b2_2) <= 1
-   0 <= InvestNonConvexFlowBlock_invest(b1_b2) <= 10
+   0 <= flow(b1_b2_0_0) <= +inf
+   0 <= flow(b1_b2_0_1) <= +inf
+   0 <= flow(b1_b2_0_2) <= +inf
+   0 <= InvestNonConvexFlowBlock_invest(b1_b2_0) <= 10
+   0 <= flow(b2_b1_0_0) <= +inf
+   0 <= flow(b2_b1_0_1) <= +inf
+   0 <= flow(b2_b1_0_2) <= +inf
    0 <= InvestNonConvexFlowBlock_status_nominal(b1_b2_0) <= +inf
    0 <= InvestNonConvexFlowBlock_status_nominal(b1_b2_1) <= +inf
    0 <= InvestNonConvexFlowBlock_status_nominal(b1_b2_2) <= +inf
+   0 <= InvestNonConvexFlowBlock_status(b1_b2_0) <= 1
+   0 <= InvestNonConvexFlowBlock_status(b1_b2_1) <= 1
+   0 <= InvestNonConvexFlowBlock_status(b1_b2_2) <= 1
 binary
   InvestNonConvexFlowBlock_status(b1_b2_0)
   InvestNonConvexFlowBlock_status(b1_b2_1)
   InvestNonConvexFlowBlock_status(b1_b2_2)
 end
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/invest_source_fixed_sink.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/invest_source_fixed_sink.lp`

 * *Files 17% similar despite different names*

```diff
@@ -1,47 +1,50 @@
 \* Source Pyomo model name=Model *\
 
-min
+min 
 objective:
-+123 InvestmentFlowBlock_invest(pv_electricityBus)
-+13 flow(pv_electricityBus_0)
-+13 flow(pv_electricityBus_1)
-+13 flow(pv_electricityBus_2)
++123 InvestmentFlowBlock_invest(pv_electricityBus_0)
++13 flow(pv_electricityBus_0_0)
++13 flow(pv_electricityBus_0_1)
++13 flow(pv_electricityBus_0_2)
 
 s.t.
 
-c_e_BusBlock_balance(electricityBus_0)_:
-+1 flow(pv_electricityBus_0)
-= 50000
-
-c_e_BusBlock_balance(electricityBus_1)_:
-+1 flow(pv_electricityBus_1)
-= 80000
-
-c_e_BusBlock_balance(electricityBus_2)_:
-+1 flow(pv_electricityBus_2)
-= 30000
-
-c_u_InvestmentFlowBlock_max(pv_electricityBus_0)_:
--45 InvestmentFlowBlock_invest(pv_electricityBus)
-+1 flow(pv_electricityBus_0)
+c_e_BusBlock_balance(electricityBus_0_0)_:
++1 flow(pv_electricityBus_0_0)
+= 50000.0
+
+c_e_BusBlock_balance(electricityBus_0_1)_:
++1 flow(pv_electricityBus_0_1)
+= 80000.0
+
+c_e_BusBlock_balance(electricityBus_0_2)_:
++1 flow(pv_electricityBus_0_2)
+= 30000.0
+
+c_e_InvestmentFlowBlock_total_rule(pv_electricityBus_0)_:
+-1 InvestmentFlowBlock_invest(pv_electricityBus_0)
++1 InvestmentFlowBlock_total(pv_electricityBus_0)
+= 0
+
+c_u_InvestmentFlowBlock_max(pv_electricityBus_0_0)_:
++1 flow(pv_electricityBus_0_0)
+-45 InvestmentFlowBlock_total(pv_electricityBus_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(pv_electricityBus_1)_:
--83 InvestmentFlowBlock_invest(pv_electricityBus)
-+1 flow(pv_electricityBus_1)
+c_u_InvestmentFlowBlock_max(pv_electricityBus_0_1)_:
++1 flow(pv_electricityBus_0_1)
+-83 InvestmentFlowBlock_total(pv_electricityBus_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(pv_electricityBus_2)_:
--65 InvestmentFlowBlock_invest(pv_electricityBus)
-+1 flow(pv_electricityBus_2)
+c_u_InvestmentFlowBlock_max(pv_electricityBus_0_2)_:
++1 flow(pv_electricityBus_0_2)
+-65 InvestmentFlowBlock_total(pv_electricityBus_0)
 <= 0
 
-c_e_ONE_VAR_CONSTANT:
-ONE_VAR_CONSTANT = 1.0
-
 bounds
-   0 <= flow(pv_electricityBus_0) <= +inf
-   0 <= flow(pv_electricityBus_1) <= +inf
-   0 <= flow(pv_electricityBus_2) <= +inf
-   0 <= InvestmentFlowBlock_invest(pv_electricityBus) <= +inf
+   0 <= InvestmentFlowBlock_invest(pv_electricityBus_0) <= +inf
+   0 <= flow(pv_electricityBus_0_0) <= +inf
+   0 <= flow(pv_electricityBus_0_1) <= +inf
+   0 <= flow(pv_electricityBus_0_2) <= +inf
+   0 <= InvestmentFlowBlock_total(pv_electricityBus_0) <= +inf
 end
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/investment_limit.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/investment_limit.lp`

 * *Files 24% similar despite different names*

```diff
@@ -1,155 +1,176 @@
 \* Source Pyomo model name=Model *\
 
-min
+min 
 objective:
-+145 GenericInvestmentStorageBlock_invest(storage_invest_limit)
-+123 InvestmentFlowBlock_invest(Source_Bus1)
++123 InvestmentFlowBlock_invest(Source_Bus1_0)
++145 GenericInvestmentStorageBlock_invest(storage_invest_limit_0)
 
 s.t.
 
 c_u_investment_limit_:
-+145 GenericInvestmentStorageBlock_invest(storage_invest_limit)
-+123 InvestmentFlowBlock_invest(Source_Bus1)
++123 InvestmentFlowBlock_invest(Source_Bus1_0)
++145 GenericInvestmentStorageBlock_invest(storage_invest_limit_0)
 <= 900
 
-c_e_BusBlock_balance(Bus1_0)_:
--1 flow(Bus1_storage_invest_limit_0)
-+1 flow(Source_Bus1_0)
-+1 flow(storage_invest_limit_Bus1_0)
+c_e_BusBlock_balance(Bus1_0_0)_:
++1 flow(Source_Bus1_0_0)
++1 flow(storage_invest_limit_Bus1_0_0)
+-1 flow(Bus1_storage_invest_limit_0_0)
 = 0
 
-c_e_BusBlock_balance(Bus1_1)_:
--1 flow(Bus1_storage_invest_limit_1)
-+1 flow(Source_Bus1_1)
-+1 flow(storage_invest_limit_Bus1_1)
+c_e_BusBlock_balance(Bus1_0_1)_:
++1 flow(Source_Bus1_0_1)
++1 flow(storage_invest_limit_Bus1_0_1)
+-1 flow(Bus1_storage_invest_limit_0_1)
 = 0
 
-c_e_BusBlock_balance(Bus1_2)_:
--1 flow(Bus1_storage_invest_limit_2)
-+1 flow(Source_Bus1_2)
-+1 flow(storage_invest_limit_Bus1_2)
+c_e_BusBlock_balance(Bus1_0_2)_:
++1 flow(Source_Bus1_0_2)
++1 flow(storage_invest_limit_Bus1_0_2)
+-1 flow(Bus1_storage_invest_limit_0_2)
 = 0
 
-c_u_InvestmentFlowBlock_max(Bus1_storage_invest_limit_0)_:
--1 InvestmentFlowBlock_invest(Bus1_storage_invest_limit)
-+1 flow(Bus1_storage_invest_limit_0)
+c_e_InvestmentFlowBlock_total_rule(Bus1_storage_invest_limit_0)_:
++1 InvestmentFlowBlock_total(Bus1_storage_invest_limit_0)
+-1 InvestmentFlowBlock_invest(Bus1_storage_invest_limit_0)
+= 0
+
+c_e_InvestmentFlowBlock_total_rule(storage_invest_limit_Bus1_0)_:
++1 InvestmentFlowBlock_total(storage_invest_limit_Bus1_0)
+-1 InvestmentFlowBlock_invest(storage_invest_limit_Bus1_0)
+= 0
+
+c_e_InvestmentFlowBlock_total_rule(Source_Bus1_0)_:
+-1 InvestmentFlowBlock_invest(Source_Bus1_0)
++1 InvestmentFlowBlock_total(Source_Bus1_0)
+= 0
+
+c_u_InvestmentFlowBlock_max(Bus1_storage_invest_limit_0_0)_:
++1 flow(Bus1_storage_invest_limit_0_0)
+-1 InvestmentFlowBlock_total(Bus1_storage_invest_limit_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(Bus1_storage_invest_limit_1)_:
--1 InvestmentFlowBlock_invest(Bus1_storage_invest_limit)
-+1 flow(Bus1_storage_invest_limit_1)
+c_u_InvestmentFlowBlock_max(Bus1_storage_invest_limit_0_1)_:
++1 flow(Bus1_storage_invest_limit_0_1)
+-1 InvestmentFlowBlock_total(Bus1_storage_invest_limit_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(Bus1_storage_invest_limit_2)_:
--1 InvestmentFlowBlock_invest(Bus1_storage_invest_limit)
-+1 flow(Bus1_storage_invest_limit_2)
+c_u_InvestmentFlowBlock_max(Bus1_storage_invest_limit_0_2)_:
++1 flow(Bus1_storage_invest_limit_0_2)
+-1 InvestmentFlowBlock_total(Bus1_storage_invest_limit_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(Source_Bus1_0)_:
--1 InvestmentFlowBlock_invest(Source_Bus1)
-+1 flow(Source_Bus1_0)
+c_u_InvestmentFlowBlock_max(storage_invest_limit_Bus1_0_0)_:
++1 flow(storage_invest_limit_Bus1_0_0)
+-1 InvestmentFlowBlock_total(storage_invest_limit_Bus1_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(Source_Bus1_1)_:
--1 InvestmentFlowBlock_invest(Source_Bus1)
-+1 flow(Source_Bus1_1)
+c_u_InvestmentFlowBlock_max(storage_invest_limit_Bus1_0_1)_:
++1 flow(storage_invest_limit_Bus1_0_1)
+-1 InvestmentFlowBlock_total(storage_invest_limit_Bus1_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(Source_Bus1_2)_:
--1 InvestmentFlowBlock_invest(Source_Bus1)
-+1 flow(Source_Bus1_2)
+c_u_InvestmentFlowBlock_max(storage_invest_limit_Bus1_0_2)_:
++1 flow(storage_invest_limit_Bus1_0_2)
+-1 InvestmentFlowBlock_total(storage_invest_limit_Bus1_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(storage_invest_limit_Bus1_0)_:
--1 InvestmentFlowBlock_invest(storage_invest_limit_Bus1)
-+1 flow(storage_invest_limit_Bus1_0)
+c_u_InvestmentFlowBlock_max(Source_Bus1_0_0)_:
++1 flow(Source_Bus1_0_0)
+-1 InvestmentFlowBlock_total(Source_Bus1_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(storage_invest_limit_Bus1_1)_:
--1 InvestmentFlowBlock_invest(storage_invest_limit_Bus1)
-+1 flow(storage_invest_limit_Bus1_1)
+c_u_InvestmentFlowBlock_max(Source_Bus1_0_1)_:
++1 flow(Source_Bus1_0_1)
+-1 InvestmentFlowBlock_total(Source_Bus1_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(storage_invest_limit_Bus1_2)_:
--1 InvestmentFlowBlock_invest(storage_invest_limit_Bus1)
-+1 flow(storage_invest_limit_Bus1_2)
+c_u_InvestmentFlowBlock_max(Source_Bus1_0_2)_:
++1 flow(Source_Bus1_0_2)
+-1 InvestmentFlowBlock_total(Source_Bus1_0)
 <= 0
 
+c_e_GenericInvestmentStorageBlock_total_storage_rule(storage_invest_limit_0)_:
+-1 GenericInvestmentStorageBlock_invest(storage_invest_limit_0)
++1 GenericInvestmentStorageBlock_total(storage_invest_limit_0)
+= 0
+
 c_u_GenericInvestmentStorageBlock_init_content_limit(storage_invest_limit)_:
+-1 GenericInvestmentStorageBlock_invest(storage_invest_limit_0)
 +1 GenericInvestmentStorageBlock_init_content(storage_invest_limit)
--1 GenericInvestmentStorageBlock_invest(storage_invest_limit)
 <= 0
 
 c_e_GenericInvestmentStorageBlock_balance_first(storage_invest_limit)_:
++1 flow(storage_invest_limit_Bus1_0_0)
+-1 flow(Bus1_storage_invest_limit_0_0)
 -1 GenericInvestmentStorageBlock_init_content(storage_invest_limit)
 +1 GenericInvestmentStorageBlock_storage_content(storage_invest_limit_0)
--1 flow(Bus1_storage_invest_limit_0)
-+1 flow(storage_invest_limit_Bus1_0)
 = 0
 
-c_e_GenericInvestmentStorageBlock_balance(storage_invest_limit_1)_:
+c_e_GenericInvestmentStorageBlock_balance(storage_invest_limit_0_1)_:
++1 flow(storage_invest_limit_Bus1_0_1)
+-1 flow(Bus1_storage_invest_limit_0_1)
 -1 GenericInvestmentStorageBlock_storage_content(storage_invest_limit_0)
 +1 GenericInvestmentStorageBlock_storage_content(storage_invest_limit_1)
--1 flow(Bus1_storage_invest_limit_1)
-+1 flow(storage_invest_limit_Bus1_1)
 = 0
 
-c_e_GenericInvestmentStorageBlock_balance(storage_invest_limit_2)_:
+c_e_GenericInvestmentStorageBlock_balance(storage_invest_limit_0_2)_:
++1 flow(storage_invest_limit_Bus1_0_2)
+-1 flow(Bus1_storage_invest_limit_0_2)
 -1 GenericInvestmentStorageBlock_storage_content(storage_invest_limit_1)
 +1 GenericInvestmentStorageBlock_storage_content(storage_invest_limit_2)
--1 flow(Bus1_storage_invest_limit_2)
-+1 flow(storage_invest_limit_Bus1_2)
 = 0
 
 c_e_GenericInvestmentStorageBlock_balanced_cstr(storage_invest_limit)_:
 -1 GenericInvestmentStorageBlock_init_content(storage_invest_limit)
 +1 GenericInvestmentStorageBlock_storage_content(storage_invest_limit_2)
 = 0
 
-c_e_GenericInvestmentStorageBlock_storage_capacity_inflow(storage_invest_limit)_:
--0.20000000000000001 GenericInvestmentStorageBlock_invest(storage_invest_limit)
-+1 InvestmentFlowBlock_invest(Bus1_storage_invest_limit)
+c_e_GenericInvestmentStorageBlock_storage_capacity_inflow(storage_invest_limit_0)_:
++1 InvestmentFlowBlock_total(Bus1_storage_invest_limit_0)
+-0.2 GenericInvestmentStorageBlock_total(storage_invest_limit_0)
 = 0
 
-c_e_GenericInvestmentStorageBlock_storage_capacity_outflow(storage_invest_limit)_:
--0.20000000000000001 GenericInvestmentStorageBlock_invest(storage_invest_limit)
-+1 InvestmentFlowBlock_invest(storage_invest_limit_Bus1)
+c_e_GenericInvestmentStorageBlock_storage_capacity_outflow(storage_invest_limit_0)_:
++1 InvestmentFlowBlock_total(storage_invest_limit_Bus1_0)
+-0.2 GenericInvestmentStorageBlock_total(storage_invest_limit_0)
 = 0
 
-c_u_GenericInvestmentStorageBlock_max_storage_content(storage_invest_limit_0)_:
--1 GenericInvestmentStorageBlock_invest(storage_invest_limit)
+c_u_GenericInvestmentStorageBlock_max_storage_content(storage_invest_limit_0_0)_:
+-1 GenericInvestmentStorageBlock_total(storage_invest_limit_0)
 +1 GenericInvestmentStorageBlock_storage_content(storage_invest_limit_0)
 <= 0
 
-c_u_GenericInvestmentStorageBlock_max_storage_content(storage_invest_limit_1)_:
--1 GenericInvestmentStorageBlock_invest(storage_invest_limit)
+c_u_GenericInvestmentStorageBlock_max_storage_content(storage_invest_limit_0_1)_:
+-1 GenericInvestmentStorageBlock_total(storage_invest_limit_0)
 +1 GenericInvestmentStorageBlock_storage_content(storage_invest_limit_1)
 <= 0
 
-c_u_GenericInvestmentStorageBlock_max_storage_content(storage_invest_limit_2)_:
--1 GenericInvestmentStorageBlock_invest(storage_invest_limit)
+c_u_GenericInvestmentStorageBlock_max_storage_content(storage_invest_limit_0_2)_:
+-1 GenericInvestmentStorageBlock_total(storage_invest_limit_0)
 +1 GenericInvestmentStorageBlock_storage_content(storage_invest_limit_2)
 <= 0
 
-c_e_ONE_VAR_CONSTANT:
-ONE_VAR_CONSTANT = 1.0
-
 bounds
-   0 <= flow(Bus1_storage_invest_limit_0) <= +inf
-   0 <= flow(Bus1_storage_invest_limit_1) <= +inf
-   0 <= flow(Bus1_storage_invest_limit_2) <= +inf
-   0 <= flow(Source_Bus1_0) <= +inf
-   0 <= flow(Source_Bus1_1) <= +inf
-   0 <= flow(Source_Bus1_2) <= +inf
-   0 <= flow(storage_invest_limit_Bus1_0) <= +inf
-   0 <= flow(storage_invest_limit_Bus1_1) <= +inf
-   0 <= flow(storage_invest_limit_Bus1_2) <= +inf
-   0 <= InvestmentFlowBlock_invest(Bus1_storage_invest_limit) <= +inf
-   0 <= InvestmentFlowBlock_invest(Source_Bus1) <= +inf
-   0 <= InvestmentFlowBlock_invest(storage_invest_limit_Bus1) <= +inf
+   0 <= InvestmentFlowBlock_invest(Source_Bus1_0) <= +inf
+   0 <= GenericInvestmentStorageBlock_invest(storage_invest_limit_0) <= +inf
+   0 <= flow(Source_Bus1_0_0) <= +inf
+   0 <= flow(storage_invest_limit_Bus1_0_0) <= +inf
+   0 <= flow(Bus1_storage_invest_limit_0_0) <= +inf
+   0 <= flow(Source_Bus1_0_1) <= +inf
+   0 <= flow(storage_invest_limit_Bus1_0_1) <= +inf
+   0 <= flow(Bus1_storage_invest_limit_0_1) <= +inf
+   0 <= flow(Source_Bus1_0_2) <= +inf
+   0 <= flow(storage_invest_limit_Bus1_0_2) <= +inf
+   0 <= flow(Bus1_storage_invest_limit_0_2) <= +inf
+   0 <= InvestmentFlowBlock_total(Bus1_storage_invest_limit_0) <= +inf
+   0 <= InvestmentFlowBlock_invest(Bus1_storage_invest_limit_0) <= +inf
+   0 <= InvestmentFlowBlock_total(storage_invest_limit_Bus1_0) <= +inf
+   0 <= InvestmentFlowBlock_invest(storage_invest_limit_Bus1_0) <= +inf
+   0 <= InvestmentFlowBlock_total(Source_Bus1_0) <= +inf
+   0 <= GenericInvestmentStorageBlock_total(storage_invest_limit_0) <= +inf
+   0 <= GenericInvestmentStorageBlock_init_content(storage_invest_limit) <= +inf
    0 <= GenericInvestmentStorageBlock_storage_content(storage_invest_limit_0) <= +inf
    0 <= GenericInvestmentStorageBlock_storage_content(storage_invest_limit_1) <= +inf
    0 <= GenericInvestmentStorageBlock_storage_content(storage_invest_limit_2) <= +inf
-   0 <= GenericInvestmentStorageBlock_invest(storage_invest_limit) <= +inf
-   0 <= GenericInvestmentStorageBlock_init_content(storage_invest_limit) <= +inf
 end
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/linear_transformer.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/linear_transformer.lp`

 * *Files 15% similar despite different names*

```diff
@@ -1,60 +1,57 @@
 \* Source Pyomo model name=Model *\
 
-min
+min 
 objective:
-+50 flow(powerplantGas_electricity_0)
-+50 flow(powerplantGas_electricity_1)
-+50 flow(powerplantGas_electricity_2)
++50 flow(powerplantGas_electricity_0_0)
++50 flow(powerplantGas_electricity_0_1)
++50 flow(powerplantGas_electricity_0_2)
 
 s.t.
 
-c_e_BusBlock_balance(electricity_0)_:
-+1 flow(powerplantGas_electricity_0)
+c_e_BusBlock_balance(gas_0_0)_:
++1 flow(gas_powerplantGas_0_0)
 = 0
 
-c_e_BusBlock_balance(electricity_1)_:
-+1 flow(powerplantGas_electricity_1)
+c_e_BusBlock_balance(gas_0_1)_:
++1 flow(gas_powerplantGas_0_1)
 = 0
 
-c_e_BusBlock_balance(electricity_2)_:
-+1 flow(powerplantGas_electricity_2)
+c_e_BusBlock_balance(gas_0_2)_:
++1 flow(gas_powerplantGas_0_2)
 = 0
 
-c_e_BusBlock_balance(gas_0)_:
-+1 flow(gas_powerplantGas_0)
+c_e_BusBlock_balance(electricity_0_0)_:
++1 flow(powerplantGas_electricity_0_0)
 = 0
 
-c_e_BusBlock_balance(gas_1)_:
-+1 flow(gas_powerplantGas_1)
+c_e_BusBlock_balance(electricity_0_1)_:
++1 flow(powerplantGas_electricity_0_1)
 = 0
 
-c_e_BusBlock_balance(gas_2)_:
-+1 flow(gas_powerplantGas_2)
+c_e_BusBlock_balance(electricity_0_2)_:
++1 flow(powerplantGas_electricity_0_2)
 = 0
 
-c_e_TransformerBlock_relation(powerplantGas_gas_electricity_0)_:
-+0.57999999999999996 flow(gas_powerplantGas_0)
--1 flow(powerplantGas_electricity_0)
+c_e_TransformerBlock_relation(powerplantGas_gas_electricity_0_0)_:
+-1 flow(powerplantGas_electricity_0_0)
++0.58 flow(gas_powerplantGas_0_0)
 = 0
 
-c_e_TransformerBlock_relation(powerplantGas_gas_electricity_1)_:
-+0.57999999999999996 flow(gas_powerplantGas_1)
--1 flow(powerplantGas_electricity_1)
+c_e_TransformerBlock_relation(powerplantGas_gas_electricity_0_1)_:
+-1 flow(powerplantGas_electricity_0_1)
++0.58 flow(gas_powerplantGas_0_1)
 = 0
 
-c_e_TransformerBlock_relation(powerplantGas_gas_electricity_2)_:
-+0.57999999999999996 flow(gas_powerplantGas_2)
--1 flow(powerplantGas_electricity_2)
+c_e_TransformerBlock_relation(powerplantGas_gas_electricity_0_2)_:
+-1 flow(powerplantGas_electricity_0_2)
++0.58 flow(gas_powerplantGas_0_2)
 = 0
 
-c_e_ONE_VAR_CONSTANT:
-ONE_VAR_CONSTANT = 1.0
-
 bounds
-   0 <= flow(gas_powerplantGas_0) <= +inf
-   0 <= flow(gas_powerplantGas_1) <= +inf
-   0 <= flow(gas_powerplantGas_2) <= +inf
-   0 <= flow(powerplantGas_electricity_0) <= 100000000000
-   0 <= flow(powerplantGas_electricity_1) <= 100000000000
-   0 <= flow(powerplantGas_electricity_2) <= 100000000000
+   0.0 <= flow(powerplantGas_electricity_0_0) <= 100000000000.0
+   0.0 <= flow(powerplantGas_electricity_0_1) <= 100000000000.0
+   0.0 <= flow(powerplantGas_electricity_0_2) <= 100000000000.0
+   0 <= flow(gas_powerplantGas_0_0) <= +inf
+   0 <= flow(gas_powerplantGas_0_1) <= +inf
+   0 <= flow(gas_powerplantGas_0_2) <= +inf
 end
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/linear_transformer_chp.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/linear_transformer_chp.lp`

 * *Files 26% similar despite different names*

```diff
@@ -1,90 +1,87 @@
 \* Source Pyomo model name=Model *\
 
-min
+min 
 objective:
-+50 flow(gasBus_CHPpowerplantGas_0)
-+50 flow(gasBus_CHPpowerplantGas_1)
-+50 flow(gasBus_CHPpowerplantGas_2)
++50 flow(gasBus_CHPpowerplantGas_0_0)
++50 flow(gasBus_CHPpowerplantGas_0_1)
++50 flow(gasBus_CHPpowerplantGas_0_2)
 
 s.t.
 
-c_e_BusBlock_balance(electricityBus_0)_:
-+1 flow(CHPpowerplantGas_electricityBus_0)
+c_e_BusBlock_balance(gasBus_0_0)_:
++1 flow(gasBus_CHPpowerplantGas_0_0)
 = 0
 
-c_e_BusBlock_balance(electricityBus_1)_:
-+1 flow(CHPpowerplantGas_electricityBus_1)
+c_e_BusBlock_balance(gasBus_0_1)_:
++1 flow(gasBus_CHPpowerplantGas_0_1)
 = 0
 
-c_e_BusBlock_balance(electricityBus_2)_:
-+1 flow(CHPpowerplantGas_electricityBus_2)
+c_e_BusBlock_balance(gasBus_0_2)_:
++1 flow(gasBus_CHPpowerplantGas_0_2)
 = 0
 
-c_e_BusBlock_balance(gasBus_0)_:
-+1 flow(gasBus_CHPpowerplantGas_0)
+c_e_BusBlock_balance(electricityBus_0_0)_:
++1 flow(CHPpowerplantGas_electricityBus_0_0)
 = 0
 
-c_e_BusBlock_balance(gasBus_1)_:
-+1 flow(gasBus_CHPpowerplantGas_1)
+c_e_BusBlock_balance(electricityBus_0_1)_:
++1 flow(CHPpowerplantGas_electricityBus_0_1)
 = 0
 
-c_e_BusBlock_balance(gasBus_2)_:
-+1 flow(gasBus_CHPpowerplantGas_2)
+c_e_BusBlock_balance(electricityBus_0_2)_:
++1 flow(CHPpowerplantGas_electricityBus_0_2)
 = 0
 
-c_e_BusBlock_balance(heatBus_0)_:
-+1 flow(CHPpowerplantGas_heatBus_0)
+c_e_BusBlock_balance(heatBus_0_0)_:
++1 flow(CHPpowerplantGas_heatBus_0_0)
 = 0
 
-c_e_BusBlock_balance(heatBus_1)_:
-+1 flow(CHPpowerplantGas_heatBus_1)
+c_e_BusBlock_balance(heatBus_0_1)_:
++1 flow(CHPpowerplantGas_heatBus_0_1)
 = 0
 
-c_e_BusBlock_balance(heatBus_2)_:
-+1 flow(CHPpowerplantGas_heatBus_2)
+c_e_BusBlock_balance(heatBus_0_2)_:
++1 flow(CHPpowerplantGas_heatBus_0_2)
 = 0
 
-c_e_TransformerBlock_relation(CHPpowerplantGas_gasBus_electricityBus_0)_:
--1 flow(CHPpowerplantGas_electricityBus_0)
-+0.40000000000000002 flow(gasBus_CHPpowerplantGas_0)
+c_e_TransformerBlock_relation(CHPpowerplantGas_gasBus_electricityBus_0_0)_:
++0.4 flow(gasBus_CHPpowerplantGas_0_0)
+-1 flow(CHPpowerplantGas_electricityBus_0_0)
 = 0
 
-c_e_TransformerBlock_relation(CHPpowerplantGas_gasBus_electricityBus_1)_:
--1 flow(CHPpowerplantGas_electricityBus_1)
-+0.40000000000000002 flow(gasBus_CHPpowerplantGas_1)
+c_e_TransformerBlock_relation(CHPpowerplantGas_gasBus_heatBus_0_0)_:
++0.5 flow(gasBus_CHPpowerplantGas_0_0)
+-1 flow(CHPpowerplantGas_heatBus_0_0)
 = 0
 
-c_e_TransformerBlock_relation(CHPpowerplantGas_gasBus_electricityBus_2)_:
--1 flow(CHPpowerplantGas_electricityBus_2)
-+0.40000000000000002 flow(gasBus_CHPpowerplantGas_2)
+c_e_TransformerBlock_relation(CHPpowerplantGas_gasBus_electricityBus_0_1)_:
++0.4 flow(gasBus_CHPpowerplantGas_0_1)
+-1 flow(CHPpowerplantGas_electricityBus_0_1)
 = 0
 
-c_e_TransformerBlock_relation(CHPpowerplantGas_gasBus_heatBus_0)_:
--1 flow(CHPpowerplantGas_heatBus_0)
-+0.5 flow(gasBus_CHPpowerplantGas_0)
+c_e_TransformerBlock_relation(CHPpowerplantGas_gasBus_heatBus_0_1)_:
++0.5 flow(gasBus_CHPpowerplantGas_0_1)
+-1 flow(CHPpowerplantGas_heatBus_0_1)
 = 0
 
-c_e_TransformerBlock_relation(CHPpowerplantGas_gasBus_heatBus_1)_:
--1 flow(CHPpowerplantGas_heatBus_1)
-+0.5 flow(gasBus_CHPpowerplantGas_1)
+c_e_TransformerBlock_relation(CHPpowerplantGas_gasBus_electricityBus_0_2)_:
++0.4 flow(gasBus_CHPpowerplantGas_0_2)
+-1 flow(CHPpowerplantGas_electricityBus_0_2)
 = 0
 
-c_e_TransformerBlock_relation(CHPpowerplantGas_gasBus_heatBus_2)_:
--1 flow(CHPpowerplantGas_heatBus_2)
-+0.5 flow(gasBus_CHPpowerplantGas_2)
+c_e_TransformerBlock_relation(CHPpowerplantGas_gasBus_heatBus_0_2)_:
++0.5 flow(gasBus_CHPpowerplantGas_0_2)
+-1 flow(CHPpowerplantGas_heatBus_0_2)
 = 0
 
-c_e_ONE_VAR_CONSTANT:
-ONE_VAR_CONSTANT = 1.0
-
 bounds
-   0 <= flow(CHPpowerplantGas_electricityBus_0) <= +inf
-   0 <= flow(CHPpowerplantGas_electricityBus_1) <= +inf
-   0 <= flow(CHPpowerplantGas_electricityBus_2) <= +inf
-   0 <= flow(CHPpowerplantGas_heatBus_0) <= +inf
-   0 <= flow(CHPpowerplantGas_heatBus_1) <= +inf
-   0 <= flow(CHPpowerplantGas_heatBus_2) <= +inf
-   0 <= flow(gasBus_CHPpowerplantGas_0) <= 100000000000
-   0 <= flow(gasBus_CHPpowerplantGas_1) <= 100000000000
-   0 <= flow(gasBus_CHPpowerplantGas_2) <= 100000000000
+   0.0 <= flow(gasBus_CHPpowerplantGas_0_0) <= 100000000000.0
+   0.0 <= flow(gasBus_CHPpowerplantGas_0_1) <= 100000000000.0
+   0.0 <= flow(gasBus_CHPpowerplantGas_0_2) <= 100000000000.0
+   0 <= flow(CHPpowerplantGas_electricityBus_0_0) <= +inf
+   0 <= flow(CHPpowerplantGas_electricityBus_0_1) <= +inf
+   0 <= flow(CHPpowerplantGas_electricityBus_0_2) <= +inf
+   0 <= flow(CHPpowerplantGas_heatBus_0_0) <= +inf
+   0 <= flow(CHPpowerplantGas_heatBus_0_1) <= +inf
+   0 <= flow(CHPpowerplantGas_heatBus_0_2) <= +inf
 end
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/linear_transformer_chp_invest.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/linear_transformer_chp_invest.lp`

 * *Files 10% similar despite different names*

```diff
@@ -1,107 +1,110 @@
 \* Source Pyomo model name=Model *\
 
-min
+min 
 objective:
-+20 InvestmentFlowBlock_invest(gasBus_chp_powerplant_gas)
-+50 flow(gasBus_chp_powerplant_gas_0)
-+50 flow(gasBus_chp_powerplant_gas_1)
-+50 flow(gasBus_chp_powerplant_gas_2)
++20 InvestmentFlowBlock_invest(gasBus_chp_powerplant_gas_0)
++50 flow(gasBus_chp_powerplant_gas_0_0)
++50 flow(gasBus_chp_powerplant_gas_0_1)
++50 flow(gasBus_chp_powerplant_gas_0_2)
 
 s.t.
 
-c_e_BusBlock_balance(electricityBus_0)_:
-+1 flow(chp_powerplant_gas_electricityBus_0)
+c_e_BusBlock_balance(gasBus_0_0)_:
++1 flow(gasBus_chp_powerplant_gas_0_0)
 = 0
 
-c_e_BusBlock_balance(electricityBus_1)_:
-+1 flow(chp_powerplant_gas_electricityBus_1)
+c_e_BusBlock_balance(gasBus_0_1)_:
++1 flow(gasBus_chp_powerplant_gas_0_1)
 = 0
 
-c_e_BusBlock_balance(electricityBus_2)_:
-+1 flow(chp_powerplant_gas_electricityBus_2)
+c_e_BusBlock_balance(gasBus_0_2)_:
++1 flow(gasBus_chp_powerplant_gas_0_2)
 = 0
 
-c_e_BusBlock_balance(gasBus_0)_:
-+1 flow(gasBus_chp_powerplant_gas_0)
+c_e_BusBlock_balance(electricityBus_0_0)_:
++1 flow(chp_powerplant_gas_electricityBus_0_0)
 = 0
 
-c_e_BusBlock_balance(gasBus_1)_:
-+1 flow(gasBus_chp_powerplant_gas_1)
+c_e_BusBlock_balance(electricityBus_0_1)_:
++1 flow(chp_powerplant_gas_electricityBus_0_1)
 = 0
 
-c_e_BusBlock_balance(gasBus_2)_:
-+1 flow(gasBus_chp_powerplant_gas_2)
+c_e_BusBlock_balance(electricityBus_0_2)_:
++1 flow(chp_powerplant_gas_electricityBus_0_2)
 = 0
 
-c_e_BusBlock_balance(heatBus_0)_:
-+1 flow(chp_powerplant_gas_heatBus_0)
+c_e_BusBlock_balance(heatBus_0_0)_:
++1 flow(chp_powerplant_gas_heatBus_0_0)
 = 0
 
-c_e_BusBlock_balance(heatBus_1)_:
-+1 flow(chp_powerplant_gas_heatBus_1)
+c_e_BusBlock_balance(heatBus_0_1)_:
++1 flow(chp_powerplant_gas_heatBus_0_1)
 = 0
 
-c_e_BusBlock_balance(heatBus_2)_:
-+1 flow(chp_powerplant_gas_heatBus_2)
+c_e_BusBlock_balance(heatBus_0_2)_:
++1 flow(chp_powerplant_gas_heatBus_0_2)
 = 0
 
-c_e_TransformerBlock_relation(chp_powerplant_gas_gasBus_electricityBus_0)_:
--1 flow(chp_powerplant_gas_electricityBus_0)
-+0.40000000000000002 flow(gasBus_chp_powerplant_gas_0)
+c_e_TransformerBlock_relation(chp_powerplant_gas_gasBus_electricityBus_0_0)_:
++0.4 flow(gasBus_chp_powerplant_gas_0_0)
+-1 flow(chp_powerplant_gas_electricityBus_0_0)
 = 0
 
-c_e_TransformerBlock_relation(chp_powerplant_gas_gasBus_electricityBus_1)_:
--1 flow(chp_powerplant_gas_electricityBus_1)
-+0.40000000000000002 flow(gasBus_chp_powerplant_gas_1)
+c_e_TransformerBlock_relation(chp_powerplant_gas_gasBus_heatBus_0_0)_:
++0.5 flow(gasBus_chp_powerplant_gas_0_0)
+-1 flow(chp_powerplant_gas_heatBus_0_0)
 = 0
 
-c_e_TransformerBlock_relation(chp_powerplant_gas_gasBus_electricityBus_2)_:
--1 flow(chp_powerplant_gas_electricityBus_2)
-+0.40000000000000002 flow(gasBus_chp_powerplant_gas_2)
+c_e_TransformerBlock_relation(chp_powerplant_gas_gasBus_electricityBus_0_1)_:
++0.4 flow(gasBus_chp_powerplant_gas_0_1)
+-1 flow(chp_powerplant_gas_electricityBus_0_1)
 = 0
 
-c_e_TransformerBlock_relation(chp_powerplant_gas_gasBus_heatBus_0)_:
--1 flow(chp_powerplant_gas_heatBus_0)
-+0.5 flow(gasBus_chp_powerplant_gas_0)
+c_e_TransformerBlock_relation(chp_powerplant_gas_gasBus_heatBus_0_1)_:
++0.5 flow(gasBus_chp_powerplant_gas_0_1)
+-1 flow(chp_powerplant_gas_heatBus_0_1)
 = 0
 
-c_e_TransformerBlock_relation(chp_powerplant_gas_gasBus_heatBus_1)_:
--1 flow(chp_powerplant_gas_heatBus_1)
-+0.5 flow(gasBus_chp_powerplant_gas_1)
+c_e_TransformerBlock_relation(chp_powerplant_gas_gasBus_electricityBus_0_2)_:
++0.4 flow(gasBus_chp_powerplant_gas_0_2)
+-1 flow(chp_powerplant_gas_electricityBus_0_2)
 = 0
 
-c_e_TransformerBlock_relation(chp_powerplant_gas_gasBus_heatBus_2)_:
--1 flow(chp_powerplant_gas_heatBus_2)
-+0.5 flow(gasBus_chp_powerplant_gas_2)
+c_e_TransformerBlock_relation(chp_powerplant_gas_gasBus_heatBus_0_2)_:
++0.5 flow(gasBus_chp_powerplant_gas_0_2)
+-1 flow(chp_powerplant_gas_heatBus_0_2)
 = 0
 
-c_u_InvestmentFlowBlock_max(gasBus_chp_powerplant_gas_0)_:
--1 InvestmentFlowBlock_invest(gasBus_chp_powerplant_gas)
-+1 flow(gasBus_chp_powerplant_gas_0)
-<= 0
+c_e_InvestmentFlowBlock_total_rule(gasBus_chp_powerplant_gas_0)_:
+-1 InvestmentFlowBlock_invest(gasBus_chp_powerplant_gas_0)
++1 InvestmentFlowBlock_total(gasBus_chp_powerplant_gas_0)
+= 0
 
-c_u_InvestmentFlowBlock_max(gasBus_chp_powerplant_gas_1)_:
--1 InvestmentFlowBlock_invest(gasBus_chp_powerplant_gas)
-+1 flow(gasBus_chp_powerplant_gas_1)
+c_u_InvestmentFlowBlock_max(gasBus_chp_powerplant_gas_0_0)_:
++1 flow(gasBus_chp_powerplant_gas_0_0)
+-1 InvestmentFlowBlock_total(gasBus_chp_powerplant_gas_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(gasBus_chp_powerplant_gas_2)_:
--1 InvestmentFlowBlock_invest(gasBus_chp_powerplant_gas)
-+1 flow(gasBus_chp_powerplant_gas_2)
+c_u_InvestmentFlowBlock_max(gasBus_chp_powerplant_gas_0_1)_:
++1 flow(gasBus_chp_powerplant_gas_0_1)
+-1 InvestmentFlowBlock_total(gasBus_chp_powerplant_gas_0)
 <= 0
 
-c_e_ONE_VAR_CONSTANT:
-ONE_VAR_CONSTANT = 1.0
+c_u_InvestmentFlowBlock_max(gasBus_chp_powerplant_gas_0_2)_:
++1 flow(gasBus_chp_powerplant_gas_0_2)
+-1 InvestmentFlowBlock_total(gasBus_chp_powerplant_gas_0)
+<= 0
 
 bounds
-   0 <= flow(chp_powerplant_gas_electricityBus_0) <= +inf
-   0 <= flow(chp_powerplant_gas_electricityBus_1) <= +inf
-   0 <= flow(chp_powerplant_gas_electricityBus_2) <= +inf
-   0 <= flow(chp_powerplant_gas_heatBus_0) <= +inf
-   0 <= flow(chp_powerplant_gas_heatBus_1) <= +inf
-   0 <= flow(chp_powerplant_gas_heatBus_2) <= +inf
-   0 <= flow(gasBus_chp_powerplant_gas_0) <= +inf
-   0 <= flow(gasBus_chp_powerplant_gas_1) <= +inf
-   0 <= flow(gasBus_chp_powerplant_gas_2) <= +inf
-   0 <= InvestmentFlowBlock_invest(gasBus_chp_powerplant_gas) <= 1000
+   0 <= InvestmentFlowBlock_invest(gasBus_chp_powerplant_gas_0) <= 1000
+   0 <= flow(gasBus_chp_powerplant_gas_0_0) <= +inf
+   0 <= flow(gasBus_chp_powerplant_gas_0_1) <= +inf
+   0 <= flow(gasBus_chp_powerplant_gas_0_2) <= +inf
+   0 <= flow(chp_powerplant_gas_electricityBus_0_0) <= +inf
+   0 <= flow(chp_powerplant_gas_electricityBus_0_1) <= +inf
+   0 <= flow(chp_powerplant_gas_electricityBus_0_2) <= +inf
+   0 <= flow(chp_powerplant_gas_heatBus_0_0) <= +inf
+   0 <= flow(chp_powerplant_gas_heatBus_0_1) <= +inf
+   0 <= flow(chp_powerplant_gas_heatBus_0_2) <= +inf
+   0 <= InvestmentFlowBlock_total(gasBus_chp_powerplant_gas_0) <= +inf
 end
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/linear_transformer_invest.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/linear_transformer_invest.lp`

 * *Files 10% similar despite different names*

```diff
@@ -1,77 +1,80 @@
 \* Source Pyomo model name=Model *\
 
-min
+min 
 objective:
-+20 InvestmentFlowBlock_invest(powerplant_gas_electricity)
-+50 flow(powerplant_gas_electricity_0)
-+50 flow(powerplant_gas_electricity_1)
-+50 flow(powerplant_gas_electricity_2)
++20 InvestmentFlowBlock_invest(powerplant_gas_electricity_0)
++50 flow(powerplant_gas_electricity_0_0)
++50 flow(powerplant_gas_electricity_0_1)
++50 flow(powerplant_gas_electricity_0_2)
 
 s.t.
 
-c_e_BusBlock_balance(electricity_0)_:
-+1 flow(powerplant_gas_electricity_0)
+c_e_BusBlock_balance(gas_0_0)_:
++1 flow(gas_powerplant_gas_0_0)
 = 0
 
-c_e_BusBlock_balance(electricity_1)_:
-+1 flow(powerplant_gas_electricity_1)
+c_e_BusBlock_balance(gas_0_1)_:
++1 flow(gas_powerplant_gas_0_1)
 = 0
 
-c_e_BusBlock_balance(electricity_2)_:
-+1 flow(powerplant_gas_electricity_2)
+c_e_BusBlock_balance(gas_0_2)_:
++1 flow(gas_powerplant_gas_0_2)
 = 0
 
-c_e_BusBlock_balance(gas_0)_:
-+1 flow(gas_powerplant_gas_0)
+c_e_BusBlock_balance(electricity_0_0)_:
++1 flow(powerplant_gas_electricity_0_0)
 = 0
 
-c_e_BusBlock_balance(gas_1)_:
-+1 flow(gas_powerplant_gas_1)
+c_e_BusBlock_balance(electricity_0_1)_:
++1 flow(powerplant_gas_electricity_0_1)
 = 0
 
-c_e_BusBlock_balance(gas_2)_:
-+1 flow(gas_powerplant_gas_2)
+c_e_BusBlock_balance(electricity_0_2)_:
++1 flow(powerplant_gas_electricity_0_2)
 = 0
 
-c_e_TransformerBlock_relation(powerplant_gas_gas_electricity_0)_:
-+0.57999999999999996 flow(gas_powerplant_gas_0)
--1 flow(powerplant_gas_electricity_0)
+c_e_TransformerBlock_relation(powerplant_gas_gas_electricity_0_0)_:
+-1 flow(powerplant_gas_electricity_0_0)
++0.58 flow(gas_powerplant_gas_0_0)
 = 0
 
-c_e_TransformerBlock_relation(powerplant_gas_gas_electricity_1)_:
-+0.57999999999999996 flow(gas_powerplant_gas_1)
--1 flow(powerplant_gas_electricity_1)
+c_e_TransformerBlock_relation(powerplant_gas_gas_electricity_0_1)_:
+-1 flow(powerplant_gas_electricity_0_1)
++0.58 flow(gas_powerplant_gas_0_1)
 = 0
 
-c_e_TransformerBlock_relation(powerplant_gas_gas_electricity_2)_:
-+0.57999999999999996 flow(gas_powerplant_gas_2)
--1 flow(powerplant_gas_electricity_2)
+c_e_TransformerBlock_relation(powerplant_gas_gas_electricity_0_2)_:
+-1 flow(powerplant_gas_electricity_0_2)
++0.58 flow(gas_powerplant_gas_0_2)
 = 0
 
-c_u_InvestmentFlowBlock_max(powerplant_gas_electricity_0)_:
--1 InvestmentFlowBlock_invest(powerplant_gas_electricity)
-+1 flow(powerplant_gas_electricity_0)
-<= 0
+c_e_InvestmentFlowBlock_total_rule(powerplant_gas_electricity_0)_:
+-1 InvestmentFlowBlock_invest(powerplant_gas_electricity_0)
++1 InvestmentFlowBlock_total(powerplant_gas_electricity_0)
+= 0
 
-c_u_InvestmentFlowBlock_max(powerplant_gas_electricity_1)_:
--1 InvestmentFlowBlock_invest(powerplant_gas_electricity)
-+1 flow(powerplant_gas_electricity_1)
+c_u_InvestmentFlowBlock_max(powerplant_gas_electricity_0_0)_:
++1 flow(powerplant_gas_electricity_0_0)
+-1 InvestmentFlowBlock_total(powerplant_gas_electricity_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(powerplant_gas_electricity_2)_:
--1 InvestmentFlowBlock_invest(powerplant_gas_electricity)
-+1 flow(powerplant_gas_electricity_2)
+c_u_InvestmentFlowBlock_max(powerplant_gas_electricity_0_1)_:
++1 flow(powerplant_gas_electricity_0_1)
+-1 InvestmentFlowBlock_total(powerplant_gas_electricity_0)
 <= 0
 
-c_e_ONE_VAR_CONSTANT:
-ONE_VAR_CONSTANT = 1.0
+c_u_InvestmentFlowBlock_max(powerplant_gas_electricity_0_2)_:
++1 flow(powerplant_gas_electricity_0_2)
+-1 InvestmentFlowBlock_total(powerplant_gas_electricity_0)
+<= 0
 
 bounds
-   0 <= flow(gas_powerplant_gas_0) <= +inf
-   0 <= flow(gas_powerplant_gas_1) <= +inf
-   0 <= flow(gas_powerplant_gas_2) <= +inf
-   0 <= flow(powerplant_gas_electricity_0) <= +inf
-   0 <= flow(powerplant_gas_electricity_1) <= +inf
-   0 <= flow(powerplant_gas_electricity_2) <= +inf
-   0 <= InvestmentFlowBlock_invest(powerplant_gas_electricity) <= 1000
+   0 <= InvestmentFlowBlock_invest(powerplant_gas_electricity_0) <= 1000
+   0 <= flow(powerplant_gas_electricity_0_0) <= +inf
+   0 <= flow(powerplant_gas_electricity_0_1) <= +inf
+   0 <= flow(powerplant_gas_electricity_0_2) <= +inf
+   0 <= flow(gas_powerplant_gas_0_0) <= +inf
+   0 <= flow(gas_powerplant_gas_0_1) <= +inf
+   0 <= flow(gas_powerplant_gas_0_2) <= +inf
+   0 <= InvestmentFlowBlock_total(powerplant_gas_electricity_0) <= +inf
 end
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/link.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/link.lp`

 * *Files 13% similar despite different names*

```diff
@@ -1,85 +1,83 @@
 \* Source Pyomo model name=Model *\
 
-min
+min 
 objective:
 +0 ONE_VAR_CONSTANT
 
 s.t.
 
-c_e_BusBlock_balance(bel0_0)_:
--1 flow(bel0_link_0)
-+1 flow(link_bel0_0)
+c_e_BusBlock_balance(bel0_0_0)_:
++1 flow(link_bel0_0_0)
+-1 flow(bel0_link_0_0)
 = 0
 
-c_e_BusBlock_balance(bel0_1)_:
--1 flow(bel0_link_1)
-+1 flow(link_bel0_1)
+c_e_BusBlock_balance(bel0_0_1)_:
++1 flow(link_bel0_0_1)
+-1 flow(bel0_link_0_1)
 = 0
 
-c_e_BusBlock_balance(bel0_2)_:
--1 flow(bel0_link_2)
-+1 flow(link_bel0_2)
+c_e_BusBlock_balance(bel0_0_2)_:
++1 flow(link_bel0_0_2)
+-1 flow(bel0_link_0_2)
 = 0
 
-c_e_BusBlock_balance(bel1_0)_:
--1 flow(bel1_link_0)
-+1 flow(link_bel1_0)
+c_e_BusBlock_balance(bel1_0_0)_:
++1 flow(link_bel1_0_0)
+-1 flow(bel1_link_0_0)
 = 0
 
-c_e_BusBlock_balance(bel1_1)_:
--1 flow(bel1_link_1)
-+1 flow(link_bel1_1)
+c_e_BusBlock_balance(bel1_0_1)_:
++1 flow(link_bel1_0_1)
+-1 flow(bel1_link_0_1)
 = 0
 
-c_e_BusBlock_balance(bel1_2)_:
--1 flow(bel1_link_2)
-+1 flow(link_bel1_2)
+c_e_BusBlock_balance(bel1_0_2)_:
++1 flow(link_bel1_0_2)
+-1 flow(bel1_link_0_2)
 = 0
 
-c_e_LinkBlock_relation(link_bel0_bel1_0)_:
--0.80000000000000004 flow(bel0_link_0)
-+1 flow(link_bel1_0)
+c_e_LinkBlock_relation(link_bel0_bel1_0_0)_:
+-0.8 flow(bel0_link_0_0)
++1 flow(link_bel1_0_0)
 = 0
 
-c_e_LinkBlock_relation(link_bel0_bel1_1)_:
--0.80000000000000004 flow(bel0_link_1)
-+1 flow(link_bel1_1)
+c_e_LinkBlock_relation(link_bel1_bel0_0_0)_:
++1 flow(link_bel0_0_0)
+-0.9 flow(bel1_link_0_0)
 = 0
 
-c_e_LinkBlock_relation(link_bel0_bel1_2)_:
--0.80000000000000004 flow(bel0_link_2)
-+1 flow(link_bel1_2)
+c_e_LinkBlock_relation(link_bel0_bel1_0_1)_:
+-0.8 flow(bel0_link_0_1)
++1 flow(link_bel1_0_1)
 = 0
 
-c_e_LinkBlock_relation(link_bel1_bel0_0)_:
--0.90000000000000002 flow(bel1_link_0)
-+1 flow(link_bel0_0)
+c_e_LinkBlock_relation(link_bel1_bel0_0_1)_:
++1 flow(link_bel0_0_1)
+-0.9 flow(bel1_link_0_1)
 = 0
 
-c_e_LinkBlock_relation(link_bel1_bel0_1)_:
--0.90000000000000002 flow(bel1_link_1)
-+1 flow(link_bel0_1)
+c_e_LinkBlock_relation(link_bel0_bel1_0_2)_:
+-0.8 flow(bel0_link_0_2)
++1 flow(link_bel1_0_2)
 = 0
 
-c_e_LinkBlock_relation(link_bel1_bel0_2)_:
--0.90000000000000002 flow(bel1_link_2)
-+1 flow(link_bel0_2)
+c_e_LinkBlock_relation(link_bel1_bel0_0_2)_:
++1 flow(link_bel0_0_2)
+-0.9 flow(bel1_link_0_2)
 = 0
 
-c_e_ONE_VAR_CONSTANT:
-ONE_VAR_CONSTANT = 1.0
-
 bounds
-   0 <= flow(bel0_link_0) <= 4
-   0 <= flow(bel0_link_1) <= 4
-   0 <= flow(bel0_link_2) <= 4
-   0 <= flow(bel1_link_0) <= 2
-   0 <= flow(bel1_link_1) <= 2
-   0 <= flow(bel1_link_2) <= 2
-   0 <= flow(link_bel0_0) <= +inf
-   0 <= flow(link_bel0_1) <= +inf
-   0 <= flow(link_bel0_2) <= +inf
-   0 <= flow(link_bel1_0) <= +inf
-   0 <= flow(link_bel1_1) <= +inf
-   0 <= flow(link_bel1_2) <= +inf
+   1 <= ONE_VAR_CONSTANT <= 1
+   0 <= flow(link_bel0_0_0) <= +inf
+   0 <= flow(bel0_link_0_0) <= 4
+   0 <= flow(link_bel0_0_1) <= +inf
+   0 <= flow(bel0_link_0_1) <= 4
+   0 <= flow(link_bel0_0_2) <= +inf
+   0 <= flow(bel0_link_0_2) <= 4
+   0 <= flow(link_bel1_0_0) <= +inf
+   0 <= flow(bel1_link_0_0) <= 2
+   0 <= flow(link_bel1_0_1) <= +inf
+   0 <= flow(bel1_link_0_1) <= 2
+   0 <= flow(link_bel1_0_2) <= +inf
+   0 <= flow(bel1_link_0_2) <= 2
 end
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/max_source_min_sink.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/max_source_min_sink.lp`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 \* Source Pyomo model name=Model *\
 
-min
+min 
 objective:
-+14 flow(electricityBus_minDemand_0)
-+14 flow(electricityBus_minDemand_1)
-+14 flow(electricityBus_minDemand_2)
++14 flow(electricityBus_minDemand_0_0)
++14 flow(electricityBus_minDemand_0_1)
++14 flow(electricityBus_minDemand_0_2)
 
 s.t.
 
-c_e_BusBlock_balance(electricityBus_0)_:
--1 flow(electricityBus_minDemand_0)
-+1 flow(wind_electricityBus_0)
+c_e_BusBlock_balance(electricityBus_0_0)_:
+-1 flow(electricityBus_minDemand_0_0)
++1 flow(wind_electricityBus_0_0)
 = 0
 
-c_e_BusBlock_balance(electricityBus_1)_:
--1 flow(electricityBus_minDemand_1)
-+1 flow(wind_electricityBus_1)
+c_e_BusBlock_balance(electricityBus_0_1)_:
+-1 flow(electricityBus_minDemand_0_1)
++1 flow(wind_electricityBus_0_1)
 = 0
 
-c_e_BusBlock_balance(electricityBus_2)_:
--1 flow(electricityBus_minDemand_2)
-+1 flow(wind_electricityBus_2)
+c_e_BusBlock_balance(electricityBus_0_2)_:
+-1 flow(electricityBus_minDemand_0_2)
++1 flow(wind_electricityBus_0_2)
 = 0
 
-c_e_ONE_VAR_CONSTANT:
-ONE_VAR_CONSTANT = 1.0
-
 bounds
-   45.359999999999999 <= flow(electricityBus_minDemand_0) <= 54
-   50.759999999999998 <= flow(electricityBus_minDemand_1) <= 54
-   31.859999999999999 <= flow(electricityBus_minDemand_2) <= 54
-   0 <= flow(wind_electricityBus_0) <= 45.899999999999999
-   0 <= flow(wind_electricityBus_1) <= 51.299999999999997
-   0 <= flow(wind_electricityBus_2) <= 32.939999999999998
+   45.36 <= flow(electricityBus_minDemand_0_0) <= 54
+   50.76 <= flow(electricityBus_minDemand_0_1) <= 54
+   31.86 <= flow(electricityBus_minDemand_0_2) <= 54
+   0 <= flow(wind_electricityBus_0_0) <= 45.9
+   0 <= flow(wind_electricityBus_0_1) <= 51.3
+   0 <= flow(wind_electricityBus_0_2) <= 32.94
 end
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/maximum_shutdowns.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/maximum_shutdowns.lp`

 * *Files 6% similar despite different names*

```diff
@@ -1,110 +1,107 @@
 \* Source Pyomo model name=Model *\
 
-min
+min 
 objective:
-+10 flow(cheap_plant_maximum_shutdowns_Bus_C_0)
-+10 flow(cheap_plant_maximum_shutdowns_Bus_C_1)
-+10 flow(cheap_plant_maximum_shutdowns_Bus_C_2)
++10 flow(cheap_plant_maximum_shutdowns_Bus_C_0_0)
++10 flow(cheap_plant_maximum_shutdowns_Bus_C_0_1)
++10 flow(cheap_plant_maximum_shutdowns_Bus_C_0_2)
 
 s.t.
 
-c_e_BusBlock_balance(Bus_C_0)_:
-+1 flow(cheap_plant_maximum_shutdowns_Bus_C_0)
+c_e_BusBlock_balance(Bus_C_0_0)_:
++1 flow(cheap_plant_maximum_shutdowns_Bus_C_0_0)
 = 0
 
-c_e_BusBlock_balance(Bus_C_1)_:
-+1 flow(cheap_plant_maximum_shutdowns_Bus_C_1)
+c_e_BusBlock_balance(Bus_C_0_1)_:
++1 flow(cheap_plant_maximum_shutdowns_Bus_C_0_1)
 = 0
 
-c_e_BusBlock_balance(Bus_C_2)_:
-+1 flow(cheap_plant_maximum_shutdowns_Bus_C_2)
+c_e_BusBlock_balance(Bus_C_0_2)_:
++1 flow(cheap_plant_maximum_shutdowns_Bus_C_0_2)
 = 0
 
 c_e_NonConvexFlowBlock_status_nominal_constraint(cheap_plant_maximum_shutdowns_Bus_C_0)_:
--10 NonConvexFlowBlock_status(cheap_plant_maximum_shutdowns_Bus_C_0)
 +1 NonConvexFlowBlock_status_nominal(cheap_plant_maximum_shutdowns_Bus_C_0)
+-10 NonConvexFlowBlock_status(cheap_plant_maximum_shutdowns_Bus_C_0)
 = 0
 
 c_e_NonConvexFlowBlock_status_nominal_constraint(cheap_plant_maximum_shutdowns_Bus_C_1)_:
--10 NonConvexFlowBlock_status(cheap_plant_maximum_shutdowns_Bus_C_1)
 +1 NonConvexFlowBlock_status_nominal(cheap_plant_maximum_shutdowns_Bus_C_1)
+-10 NonConvexFlowBlock_status(cheap_plant_maximum_shutdowns_Bus_C_1)
 = 0
 
 c_e_NonConvexFlowBlock_status_nominal_constraint(cheap_plant_maximum_shutdowns_Bus_C_2)_:
--10 NonConvexFlowBlock_status(cheap_plant_maximum_shutdowns_Bus_C_2)
 +1 NonConvexFlowBlock_status_nominal(cheap_plant_maximum_shutdowns_Bus_C_2)
+-10 NonConvexFlowBlock_status(cheap_plant_maximum_shutdowns_Bus_C_2)
 = 0
 
-c_u_NonConvexFlowBlock_min(cheap_plant_maximum_shutdowns_Bus_C_0)_:
+c_u_NonConvexFlowBlock_min(cheap_plant_maximum_shutdowns_Bus_C_0_0)_:
+-1 flow(cheap_plant_maximum_shutdowns_Bus_C_0_0)
 +0.5 NonConvexFlowBlock_status_nominal(cheap_plant_maximum_shutdowns_Bus_C_0)
--1 flow(cheap_plant_maximum_shutdowns_Bus_C_0)
 <= 0
 
-c_u_NonConvexFlowBlock_min(cheap_plant_maximum_shutdowns_Bus_C_1)_:
+c_u_NonConvexFlowBlock_min(cheap_plant_maximum_shutdowns_Bus_C_0_1)_:
+-1 flow(cheap_plant_maximum_shutdowns_Bus_C_0_1)
 +0.5 NonConvexFlowBlock_status_nominal(cheap_plant_maximum_shutdowns_Bus_C_1)
--1 flow(cheap_plant_maximum_shutdowns_Bus_C_1)
 <= 0
 
-c_u_NonConvexFlowBlock_min(cheap_plant_maximum_shutdowns_Bus_C_2)_:
+c_u_NonConvexFlowBlock_min(cheap_plant_maximum_shutdowns_Bus_C_0_2)_:
+-1 flow(cheap_plant_maximum_shutdowns_Bus_C_0_2)
 +0.5 NonConvexFlowBlock_status_nominal(cheap_plant_maximum_shutdowns_Bus_C_2)
--1 flow(cheap_plant_maximum_shutdowns_Bus_C_2)
 <= 0
 
-c_u_NonConvexFlowBlock_max(cheap_plant_maximum_shutdowns_Bus_C_0)_:
+c_u_NonConvexFlowBlock_max(cheap_plant_maximum_shutdowns_Bus_C_0_0)_:
++1 flow(cheap_plant_maximum_shutdowns_Bus_C_0_0)
 -1 NonConvexFlowBlock_status_nominal(cheap_plant_maximum_shutdowns_Bus_C_0)
-+1 flow(cheap_plant_maximum_shutdowns_Bus_C_0)
 <= 0
 
-c_u_NonConvexFlowBlock_max(cheap_plant_maximum_shutdowns_Bus_C_1)_:
+c_u_NonConvexFlowBlock_max(cheap_plant_maximum_shutdowns_Bus_C_0_1)_:
++1 flow(cheap_plant_maximum_shutdowns_Bus_C_0_1)
 -1 NonConvexFlowBlock_status_nominal(cheap_plant_maximum_shutdowns_Bus_C_1)
-+1 flow(cheap_plant_maximum_shutdowns_Bus_C_1)
 <= 0
 
-c_u_NonConvexFlowBlock_max(cheap_plant_maximum_shutdowns_Bus_C_2)_:
+c_u_NonConvexFlowBlock_max(cheap_plant_maximum_shutdowns_Bus_C_0_2)_:
++1 flow(cheap_plant_maximum_shutdowns_Bus_C_0_2)
 -1 NonConvexFlowBlock_status_nominal(cheap_plant_maximum_shutdowns_Bus_C_2)
-+1 flow(cheap_plant_maximum_shutdowns_Bus_C_2)
 <= 0
 
 c_u_NonConvexFlowBlock_shutdown_constr(cheap_plant_maximum_shutdowns_Bus_C_0)_:
--1 NonConvexFlowBlock_shutdown(cheap_plant_maximum_shutdowns_Bus_C_0)
 -1 NonConvexFlowBlock_status(cheap_plant_maximum_shutdowns_Bus_C_0)
+-1 NonConvexFlowBlock_shutdown(cheap_plant_maximum_shutdowns_Bus_C_0)
 <= 0
 
 c_u_NonConvexFlowBlock_shutdown_constr(cheap_plant_maximum_shutdowns_Bus_C_1)_:
--1 NonConvexFlowBlock_shutdown(cheap_plant_maximum_shutdowns_Bus_C_1)
 +1 NonConvexFlowBlock_status(cheap_plant_maximum_shutdowns_Bus_C_0)
 -1 NonConvexFlowBlock_status(cheap_plant_maximum_shutdowns_Bus_C_1)
+-1 NonConvexFlowBlock_shutdown(cheap_plant_maximum_shutdowns_Bus_C_1)
 <= 0
 
 c_u_NonConvexFlowBlock_shutdown_constr(cheap_plant_maximum_shutdowns_Bus_C_2)_:
--1 NonConvexFlowBlock_shutdown(cheap_plant_maximum_shutdowns_Bus_C_2)
 +1 NonConvexFlowBlock_status(cheap_plant_maximum_shutdowns_Bus_C_1)
 -1 NonConvexFlowBlock_status(cheap_plant_maximum_shutdowns_Bus_C_2)
+-1 NonConvexFlowBlock_shutdown(cheap_plant_maximum_shutdowns_Bus_C_2)
 <= 0
 
 c_u_NonConvexFlowBlock_max_shutdown_constr(cheap_plant_maximum_shutdowns_Bus_C)_:
 +1 NonConvexFlowBlock_shutdown(cheap_plant_maximum_shutdowns_Bus_C_0)
 +1 NonConvexFlowBlock_shutdown(cheap_plant_maximum_shutdowns_Bus_C_1)
 +1 NonConvexFlowBlock_shutdown(cheap_plant_maximum_shutdowns_Bus_C_2)
 <= 2
 
-c_e_ONE_VAR_CONSTANT:
-ONE_VAR_CONSTANT = 1.0
-
 bounds
-   0 <= flow(cheap_plant_maximum_shutdowns_Bus_C_0) <= 10
-   0 <= flow(cheap_plant_maximum_shutdowns_Bus_C_1) <= 10
-   0 <= flow(cheap_plant_maximum_shutdowns_Bus_C_2) <= 10
-   0 <= NonConvexFlowBlock_status(cheap_plant_maximum_shutdowns_Bus_C_0) <= 1
-   0 <= NonConvexFlowBlock_status(cheap_plant_maximum_shutdowns_Bus_C_1) <= 1
-   0 <= NonConvexFlowBlock_status(cheap_plant_maximum_shutdowns_Bus_C_2) <= 1
+   0 <= flow(cheap_plant_maximum_shutdowns_Bus_C_0_0) <= 10.0
+   0 <= flow(cheap_plant_maximum_shutdowns_Bus_C_0_1) <= 10.0
+   0 <= flow(cheap_plant_maximum_shutdowns_Bus_C_0_2) <= 10.0
    0 <= NonConvexFlowBlock_status_nominal(cheap_plant_maximum_shutdowns_Bus_C_0) <= +inf
+   0 <= NonConvexFlowBlock_status(cheap_plant_maximum_shutdowns_Bus_C_0) <= 1
    0 <= NonConvexFlowBlock_status_nominal(cheap_plant_maximum_shutdowns_Bus_C_1) <= +inf
+   0 <= NonConvexFlowBlock_status(cheap_plant_maximum_shutdowns_Bus_C_1) <= 1
    0 <= NonConvexFlowBlock_status_nominal(cheap_plant_maximum_shutdowns_Bus_C_2) <= +inf
+   0 <= NonConvexFlowBlock_status(cheap_plant_maximum_shutdowns_Bus_C_2) <= 1
    0 <= NonConvexFlowBlock_shutdown(cheap_plant_maximum_shutdowns_Bus_C_0) <= 1
    0 <= NonConvexFlowBlock_shutdown(cheap_plant_maximum_shutdowns_Bus_C_1) <= 1
    0 <= NonConvexFlowBlock_shutdown(cheap_plant_maximum_shutdowns_Bus_C_2) <= 1
 binary
   NonConvexFlowBlock_status(cheap_plant_maximum_shutdowns_Bus_C_0)
   NonConvexFlowBlock_status(cheap_plant_maximum_shutdowns_Bus_C_1)
   NonConvexFlowBlock_status(cheap_plant_maximum_shutdowns_Bus_C_2)
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/maximum_startups.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/maximum_startups.lp`

 * *Files 10% similar despite different names*

```diff
@@ -1,110 +1,107 @@
 \* Source Pyomo model name=Model *\
 
-min
+min 
 objective:
-+10 flow(cheap_plant_maximum_startups_Bus_C_0)
-+10 flow(cheap_plant_maximum_startups_Bus_C_1)
-+10 flow(cheap_plant_maximum_startups_Bus_C_2)
++10 flow(cheap_plant_maximum_startups_Bus_C_0_0)
++10 flow(cheap_plant_maximum_startups_Bus_C_0_1)
++10 flow(cheap_plant_maximum_startups_Bus_C_0_2)
 
 s.t.
 
-c_e_BusBlock_balance(Bus_C_0)_:
-+1 flow(cheap_plant_maximum_startups_Bus_C_0)
+c_e_BusBlock_balance(Bus_C_0_0)_:
++1 flow(cheap_plant_maximum_startups_Bus_C_0_0)
 = 0
 
-c_e_BusBlock_balance(Bus_C_1)_:
-+1 flow(cheap_plant_maximum_startups_Bus_C_1)
+c_e_BusBlock_balance(Bus_C_0_1)_:
++1 flow(cheap_plant_maximum_startups_Bus_C_0_1)
 = 0
 
-c_e_BusBlock_balance(Bus_C_2)_:
-+1 flow(cheap_plant_maximum_startups_Bus_C_2)
+c_e_BusBlock_balance(Bus_C_0_2)_:
++1 flow(cheap_plant_maximum_startups_Bus_C_0_2)
 = 0
 
 c_e_NonConvexFlowBlock_status_nominal_constraint(cheap_plant_maximum_startups_Bus_C_0)_:
--10 NonConvexFlowBlock_status(cheap_plant_maximum_startups_Bus_C_0)
 +1 NonConvexFlowBlock_status_nominal(cheap_plant_maximum_startups_Bus_C_0)
+-10 NonConvexFlowBlock_status(cheap_plant_maximum_startups_Bus_C_0)
 = 0
 
 c_e_NonConvexFlowBlock_status_nominal_constraint(cheap_plant_maximum_startups_Bus_C_1)_:
--10 NonConvexFlowBlock_status(cheap_plant_maximum_startups_Bus_C_1)
 +1 NonConvexFlowBlock_status_nominal(cheap_plant_maximum_startups_Bus_C_1)
+-10 NonConvexFlowBlock_status(cheap_plant_maximum_startups_Bus_C_1)
 = 0
 
 c_e_NonConvexFlowBlock_status_nominal_constraint(cheap_plant_maximum_startups_Bus_C_2)_:
--10 NonConvexFlowBlock_status(cheap_plant_maximum_startups_Bus_C_2)
 +1 NonConvexFlowBlock_status_nominal(cheap_plant_maximum_startups_Bus_C_2)
+-10 NonConvexFlowBlock_status(cheap_plant_maximum_startups_Bus_C_2)
 = 0
 
-c_u_NonConvexFlowBlock_min(cheap_plant_maximum_startups_Bus_C_0)_:
+c_u_NonConvexFlowBlock_min(cheap_plant_maximum_startups_Bus_C_0_0)_:
+-1 flow(cheap_plant_maximum_startups_Bus_C_0_0)
 +0.5 NonConvexFlowBlock_status_nominal(cheap_plant_maximum_startups_Bus_C_0)
--1 flow(cheap_plant_maximum_startups_Bus_C_0)
 <= 0
 
-c_u_NonConvexFlowBlock_min(cheap_plant_maximum_startups_Bus_C_1)_:
+c_u_NonConvexFlowBlock_min(cheap_plant_maximum_startups_Bus_C_0_1)_:
+-1 flow(cheap_plant_maximum_startups_Bus_C_0_1)
 +0.5 NonConvexFlowBlock_status_nominal(cheap_plant_maximum_startups_Bus_C_1)
--1 flow(cheap_plant_maximum_startups_Bus_C_1)
 <= 0
 
-c_u_NonConvexFlowBlock_min(cheap_plant_maximum_startups_Bus_C_2)_:
+c_u_NonConvexFlowBlock_min(cheap_plant_maximum_startups_Bus_C_0_2)_:
+-1 flow(cheap_plant_maximum_startups_Bus_C_0_2)
 +0.5 NonConvexFlowBlock_status_nominal(cheap_plant_maximum_startups_Bus_C_2)
--1 flow(cheap_plant_maximum_startups_Bus_C_2)
 <= 0
 
-c_u_NonConvexFlowBlock_max(cheap_plant_maximum_startups_Bus_C_0)_:
+c_u_NonConvexFlowBlock_max(cheap_plant_maximum_startups_Bus_C_0_0)_:
++1 flow(cheap_plant_maximum_startups_Bus_C_0_0)
 -1 NonConvexFlowBlock_status_nominal(cheap_plant_maximum_startups_Bus_C_0)
-+1 flow(cheap_plant_maximum_startups_Bus_C_0)
 <= 0
 
-c_u_NonConvexFlowBlock_max(cheap_plant_maximum_startups_Bus_C_1)_:
+c_u_NonConvexFlowBlock_max(cheap_plant_maximum_startups_Bus_C_0_1)_:
++1 flow(cheap_plant_maximum_startups_Bus_C_0_1)
 -1 NonConvexFlowBlock_status_nominal(cheap_plant_maximum_startups_Bus_C_1)
-+1 flow(cheap_plant_maximum_startups_Bus_C_1)
 <= 0
 
-c_u_NonConvexFlowBlock_max(cheap_plant_maximum_startups_Bus_C_2)_:
+c_u_NonConvexFlowBlock_max(cheap_plant_maximum_startups_Bus_C_0_2)_:
++1 flow(cheap_plant_maximum_startups_Bus_C_0_2)
 -1 NonConvexFlowBlock_status_nominal(cheap_plant_maximum_startups_Bus_C_2)
-+1 flow(cheap_plant_maximum_startups_Bus_C_2)
 <= 0
 
 c_u_NonConvexFlowBlock_startup_constr(cheap_plant_maximum_startups_Bus_C_0)_:
--1 NonConvexFlowBlock_startup(cheap_plant_maximum_startups_Bus_C_0)
 +1 NonConvexFlowBlock_status(cheap_plant_maximum_startups_Bus_C_0)
+-1 NonConvexFlowBlock_startup(cheap_plant_maximum_startups_Bus_C_0)
 <= 0
 
 c_u_NonConvexFlowBlock_startup_constr(cheap_plant_maximum_startups_Bus_C_1)_:
--1 NonConvexFlowBlock_startup(cheap_plant_maximum_startups_Bus_C_1)
 -1 NonConvexFlowBlock_status(cheap_plant_maximum_startups_Bus_C_0)
 +1 NonConvexFlowBlock_status(cheap_plant_maximum_startups_Bus_C_1)
+-1 NonConvexFlowBlock_startup(cheap_plant_maximum_startups_Bus_C_1)
 <= 0
 
 c_u_NonConvexFlowBlock_startup_constr(cheap_plant_maximum_startups_Bus_C_2)_:
--1 NonConvexFlowBlock_startup(cheap_plant_maximum_startups_Bus_C_2)
 -1 NonConvexFlowBlock_status(cheap_plant_maximum_startups_Bus_C_1)
 +1 NonConvexFlowBlock_status(cheap_plant_maximum_startups_Bus_C_2)
+-1 NonConvexFlowBlock_startup(cheap_plant_maximum_startups_Bus_C_2)
 <= 0
 
 c_u_NonConvexFlowBlock_max_startup_constr(cheap_plant_maximum_startups_Bus_C)_:
 +1 NonConvexFlowBlock_startup(cheap_plant_maximum_startups_Bus_C_0)
 +1 NonConvexFlowBlock_startup(cheap_plant_maximum_startups_Bus_C_1)
 +1 NonConvexFlowBlock_startup(cheap_plant_maximum_startups_Bus_C_2)
 <= 2
 
-c_e_ONE_VAR_CONSTANT:
-ONE_VAR_CONSTANT = 1.0
-
 bounds
-   0 <= flow(cheap_plant_maximum_startups_Bus_C_0) <= 10
-   0 <= flow(cheap_plant_maximum_startups_Bus_C_1) <= 10
-   0 <= flow(cheap_plant_maximum_startups_Bus_C_2) <= 10
-   0 <= NonConvexFlowBlock_status(cheap_plant_maximum_startups_Bus_C_0) <= 1
-   0 <= NonConvexFlowBlock_status(cheap_plant_maximum_startups_Bus_C_1) <= 1
-   0 <= NonConvexFlowBlock_status(cheap_plant_maximum_startups_Bus_C_2) <= 1
+   0 <= flow(cheap_plant_maximum_startups_Bus_C_0_0) <= 10.0
+   0 <= flow(cheap_plant_maximum_startups_Bus_C_0_1) <= 10.0
+   0 <= flow(cheap_plant_maximum_startups_Bus_C_0_2) <= 10.0
    0 <= NonConvexFlowBlock_status_nominal(cheap_plant_maximum_startups_Bus_C_0) <= +inf
+   0 <= NonConvexFlowBlock_status(cheap_plant_maximum_startups_Bus_C_0) <= 1
    0 <= NonConvexFlowBlock_status_nominal(cheap_plant_maximum_startups_Bus_C_1) <= +inf
+   0 <= NonConvexFlowBlock_status(cheap_plant_maximum_startups_Bus_C_1) <= 1
    0 <= NonConvexFlowBlock_status_nominal(cheap_plant_maximum_startups_Bus_C_2) <= +inf
+   0 <= NonConvexFlowBlock_status(cheap_plant_maximum_startups_Bus_C_2) <= 1
    0 <= NonConvexFlowBlock_startup(cheap_plant_maximum_startups_Bus_C_0) <= 1
    0 <= NonConvexFlowBlock_startup(cheap_plant_maximum_startups_Bus_C_1) <= 1
    0 <= NonConvexFlowBlock_startup(cheap_plant_maximum_startups_Bus_C_2) <= 1
 binary
   NonConvexFlowBlock_status(cheap_plant_maximum_startups_Bus_C_0)
   NonConvexFlowBlock_status(cheap_plant_maximum_startups_Bus_C_1)
   NonConvexFlowBlock_status(cheap_plant_maximum_startups_Bus_C_2)
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/min_max_runtime.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/min_max_runtime.lp`

 * *Files 4% similar despite different names*

```diff
@@ -1,78 +1,78 @@
 \* Source Pyomo model name=Model *\
 
-min
+min 
 objective:
-+7 NonConvexFlowBlock_shutdown(cheap_plant_min_down_constraints_Bus_T_0)
-+7 NonConvexFlowBlock_shutdown(cheap_plant_min_down_constraints_Bus_T_1)
-+7 NonConvexFlowBlock_shutdown(cheap_plant_min_down_constraints_Bus_T_2)
++10 flow(cheap_plant_min_down_constraints_Bus_T_0_0)
++10 flow(cheap_plant_min_down_constraints_Bus_T_0_1)
++10 flow(cheap_plant_min_down_constraints_Bus_T_0_2)
 +5 NonConvexFlowBlock_startup(cheap_plant_min_down_constraints_Bus_T_0)
 +5 NonConvexFlowBlock_startup(cheap_plant_min_down_constraints_Bus_T_1)
 +5 NonConvexFlowBlock_startup(cheap_plant_min_down_constraints_Bus_T_2)
-+10 flow(cheap_plant_min_down_constraints_Bus_T_0)
-+10 flow(cheap_plant_min_down_constraints_Bus_T_1)
-+10 flow(cheap_plant_min_down_constraints_Bus_T_2)
++7 NonConvexFlowBlock_shutdown(cheap_plant_min_down_constraints_Bus_T_0)
++7 NonConvexFlowBlock_shutdown(cheap_plant_min_down_constraints_Bus_T_1)
++7 NonConvexFlowBlock_shutdown(cheap_plant_min_down_constraints_Bus_T_2)
 
 s.t.
 
-c_e_BusBlock_balance(Bus_T_0)_:
-+1 flow(cheap_plant_min_down_constraints_Bus_T_0)
+c_e_BusBlock_balance(Bus_T_0_0)_:
++1 flow(cheap_plant_min_down_constraints_Bus_T_0_0)
 = 0
 
-c_e_BusBlock_balance(Bus_T_1)_:
-+1 flow(cheap_plant_min_down_constraints_Bus_T_1)
+c_e_BusBlock_balance(Bus_T_0_1)_:
++1 flow(cheap_plant_min_down_constraints_Bus_T_0_1)
 = 0
 
-c_e_BusBlock_balance(Bus_T_2)_:
-+1 flow(cheap_plant_min_down_constraints_Bus_T_2)
+c_e_BusBlock_balance(Bus_T_0_2)_:
++1 flow(cheap_plant_min_down_constraints_Bus_T_0_2)
 = 0
 
 c_e_NonConvexFlowBlock_status_nominal_constraint(cheap_plant_min_down_constraints_Bus_T_0)_:
--10 NonConvexFlowBlock_status(cheap_plant_min_down_constraints_Bus_T_0)
 +1 NonConvexFlowBlock_status_nominal(cheap_plant_min_down_constraints_Bus_T_0)
+-10 NonConvexFlowBlock_status(cheap_plant_min_down_constraints_Bus_T_0)
 = 0
 
 c_e_NonConvexFlowBlock_status_nominal_constraint(cheap_plant_min_down_constraints_Bus_T_1)_:
--10 NonConvexFlowBlock_status(cheap_plant_min_down_constraints_Bus_T_1)
 +1 NonConvexFlowBlock_status_nominal(cheap_plant_min_down_constraints_Bus_T_1)
+-10 NonConvexFlowBlock_status(cheap_plant_min_down_constraints_Bus_T_1)
 = 0
 
 c_e_NonConvexFlowBlock_status_nominal_constraint(cheap_plant_min_down_constraints_Bus_T_2)_:
--10 NonConvexFlowBlock_status(cheap_plant_min_down_constraints_Bus_T_2)
 +1 NonConvexFlowBlock_status_nominal(cheap_plant_min_down_constraints_Bus_T_2)
+-10 NonConvexFlowBlock_status(cheap_plant_min_down_constraints_Bus_T_2)
 = 0
 
-c_u_NonConvexFlowBlock_min(cheap_plant_min_down_constraints_Bus_T_0)_:
+c_u_NonConvexFlowBlock_min(cheap_plant_min_down_constraints_Bus_T_0_0)_:
+-1 flow(cheap_plant_min_down_constraints_Bus_T_0_0)
 +0.5 NonConvexFlowBlock_status_nominal(cheap_plant_min_down_constraints_Bus_T_0)
--1 flow(cheap_plant_min_down_constraints_Bus_T_0)
 <= 0
 
-c_u_NonConvexFlowBlock_min(cheap_plant_min_down_constraints_Bus_T_1)_:
+c_u_NonConvexFlowBlock_min(cheap_plant_min_down_constraints_Bus_T_0_1)_:
+-1 flow(cheap_plant_min_down_constraints_Bus_T_0_1)
 +0.5 NonConvexFlowBlock_status_nominal(cheap_plant_min_down_constraints_Bus_T_1)
--1 flow(cheap_plant_min_down_constraints_Bus_T_1)
 <= 0
 
-c_u_NonConvexFlowBlock_min(cheap_plant_min_down_constraints_Bus_T_2)_:
+c_u_NonConvexFlowBlock_min(cheap_plant_min_down_constraints_Bus_T_0_2)_:
+-1 flow(cheap_plant_min_down_constraints_Bus_T_0_2)
 +0.5 NonConvexFlowBlock_status_nominal(cheap_plant_min_down_constraints_Bus_T_2)
--1 flow(cheap_plant_min_down_constraints_Bus_T_2)
 <= 0
 
-c_u_NonConvexFlowBlock_max(cheap_plant_min_down_constraints_Bus_T_0)_:
+c_u_NonConvexFlowBlock_max(cheap_plant_min_down_constraints_Bus_T_0_0)_:
++1 flow(cheap_plant_min_down_constraints_Bus_T_0_0)
 -1 NonConvexFlowBlock_status_nominal(cheap_plant_min_down_constraints_Bus_T_0)
-+1 flow(cheap_plant_min_down_constraints_Bus_T_0)
 <= 0
 
-c_u_NonConvexFlowBlock_max(cheap_plant_min_down_constraints_Bus_T_1)_:
+c_u_NonConvexFlowBlock_max(cheap_plant_min_down_constraints_Bus_T_0_1)_:
++1 flow(cheap_plant_min_down_constraints_Bus_T_0_1)
 -1 NonConvexFlowBlock_status_nominal(cheap_plant_min_down_constraints_Bus_T_1)
-+1 flow(cheap_plant_min_down_constraints_Bus_T_1)
 <= 0
 
-c_u_NonConvexFlowBlock_max(cheap_plant_min_down_constraints_Bus_T_2)_:
+c_u_NonConvexFlowBlock_max(cheap_plant_min_down_constraints_Bus_T_0_2)_:
++1 flow(cheap_plant_min_down_constraints_Bus_T_0_2)
 -1 NonConvexFlowBlock_status_nominal(cheap_plant_min_down_constraints_Bus_T_2)
-+1 flow(cheap_plant_min_down_constraints_Bus_T_2)
 <= 0
 
 c_u_NonConvexFlowBlock_startup_constr(cheap_plant_min_down_constraints_Bus_T_0)_:
 -1 NonConvexFlowBlock_startup(cheap_plant_min_down_constraints_Bus_T_0)
 +1 NonConvexFlowBlock_status(cheap_plant_min_down_constraints_Bus_T_0)
 <= 2
 
@@ -125,37 +125,34 @@
 +1 NonConvexFlowBlock_status(cheap_plant_min_down_constraints_Bus_T_1)
 = 2
 
 c_e_NonConvexFlowBlock_min_downtime_constr(cheap_plant_min_down_constraints_Bus_T_2)_:
 +1 NonConvexFlowBlock_status(cheap_plant_min_down_constraints_Bus_T_2)
 = 2
 
-c_e_ONE_VAR_CONSTANT:
-ONE_VAR_CONSTANT = 1.0
-
 bounds
-   0 <= flow(cheap_plant_min_down_constraints_Bus_T_0) <= 10
-   0 <= flow(cheap_plant_min_down_constraints_Bus_T_1) <= 10
-   0 <= flow(cheap_plant_min_down_constraints_Bus_T_2) <= 10
-   0 <= NonConvexFlowBlock_status(cheap_plant_min_down_constraints_Bus_T_0) <= 1
-   0 <= NonConvexFlowBlock_status(cheap_plant_min_down_constraints_Bus_T_1) <= 1
-   0 <= NonConvexFlowBlock_status(cheap_plant_min_down_constraints_Bus_T_2) <= 1
-   0 <= NonConvexFlowBlock_status_nominal(cheap_plant_min_down_constraints_Bus_T_0) <= +inf
-   0 <= NonConvexFlowBlock_status_nominal(cheap_plant_min_down_constraints_Bus_T_1) <= +inf
-   0 <= NonConvexFlowBlock_status_nominal(cheap_plant_min_down_constraints_Bus_T_2) <= +inf
+   0 <= flow(cheap_plant_min_down_constraints_Bus_T_0_0) <= 10.0
+   0 <= flow(cheap_plant_min_down_constraints_Bus_T_0_1) <= 10.0
+   0 <= flow(cheap_plant_min_down_constraints_Bus_T_0_2) <= 10.0
    0 <= NonConvexFlowBlock_startup(cheap_plant_min_down_constraints_Bus_T_0) <= 1
    0 <= NonConvexFlowBlock_startup(cheap_plant_min_down_constraints_Bus_T_1) <= 1
    0 <= NonConvexFlowBlock_startup(cheap_plant_min_down_constraints_Bus_T_2) <= 1
    0 <= NonConvexFlowBlock_shutdown(cheap_plant_min_down_constraints_Bus_T_0) <= 1
    0 <= NonConvexFlowBlock_shutdown(cheap_plant_min_down_constraints_Bus_T_1) <= 1
    0 <= NonConvexFlowBlock_shutdown(cheap_plant_min_down_constraints_Bus_T_2) <= 1
+   0 <= NonConvexFlowBlock_status_nominal(cheap_plant_min_down_constraints_Bus_T_0) <= +inf
+   0 <= NonConvexFlowBlock_status(cheap_plant_min_down_constraints_Bus_T_0) <= 1
+   0 <= NonConvexFlowBlock_status_nominal(cheap_plant_min_down_constraints_Bus_T_1) <= +inf
+   0 <= NonConvexFlowBlock_status(cheap_plant_min_down_constraints_Bus_T_1) <= 1
+   0 <= NonConvexFlowBlock_status_nominal(cheap_plant_min_down_constraints_Bus_T_2) <= +inf
+   0 <= NonConvexFlowBlock_status(cheap_plant_min_down_constraints_Bus_T_2) <= 1
 binary
-  NonConvexFlowBlock_status(cheap_plant_min_down_constraints_Bus_T_0)
-  NonConvexFlowBlock_status(cheap_plant_min_down_constraints_Bus_T_1)
-  NonConvexFlowBlock_status(cheap_plant_min_down_constraints_Bus_T_2)
   NonConvexFlowBlock_startup(cheap_plant_min_down_constraints_Bus_T_0)
   NonConvexFlowBlock_startup(cheap_plant_min_down_constraints_Bus_T_1)
   NonConvexFlowBlock_startup(cheap_plant_min_down_constraints_Bus_T_2)
   NonConvexFlowBlock_shutdown(cheap_plant_min_down_constraints_Bus_T_0)
   NonConvexFlowBlock_shutdown(cheap_plant_min_down_constraints_Bus_T_1)
   NonConvexFlowBlock_shutdown(cheap_plant_min_down_constraints_Bus_T_2)
+  NonConvexFlowBlock_status(cheap_plant_min_down_constraints_Bus_T_0)
+  NonConvexFlowBlock_status(cheap_plant_min_down_constraints_Bus_T_1)
+  NonConvexFlowBlock_status(cheap_plant_min_down_constraints_Bus_T_2)
 end
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/nonequidistant_timeindex.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/nonequidistant_timeindex.lp`

 * *Files 25% similar despite different names*

```diff
@@ -1,253 +1,250 @@
 \* Source Pyomo model name=Model *\
 
-min
+min 
 objective:
-+100 flow(gas_boiler_0)
-+100 flow(gas_boiler_1)
-+100 flow(gas_boiler_2)
-+200 flow(gas_boiler_3)
-+200 flow(gas_boiler_4)
-+50 flow(gas_boiler_5)
-+50 flow(gas_boiler_6)
-+50 flow(gas_boiler_7)
-+56 flow(heat_storage_0)
-+56 flow(heat_storage_1)
-+56 flow(heat_storage_2)
-+112 flow(heat_storage_3)
-+112 flow(heat_storage_4)
-+28 flow(heat_storage_5)
-+28 flow(heat_storage_6)
-+28 flow(heat_storage_7)
-+24 flow(storage_heat_0)
-+24 flow(storage_heat_1)
-+24 flow(storage_heat_2)
-+48 flow(storage_heat_3)
-+48 flow(storage_heat_4)
-+12 flow(storage_heat_5)
-+12 flow(storage_heat_6)
-+12 flow(storage_heat_7)
++100 flow(gas_boiler_0_0)
++100 flow(gas_boiler_0_1)
++100 flow(gas_boiler_0_2)
++200.0 flow(gas_boiler_0_3)
++200.0 flow(gas_boiler_0_4)
++50.0 flow(gas_boiler_0_5)
++50.0 flow(gas_boiler_0_6)
++50.0 flow(gas_boiler_0_7)
++56 flow(heat_storage_0_0)
++56 flow(heat_storage_0_1)
++56 flow(heat_storage_0_2)
++112.0 flow(heat_storage_0_3)
++112.0 flow(heat_storage_0_4)
++28.0 flow(heat_storage_0_5)
++28.0 flow(heat_storage_0_6)
++28.0 flow(heat_storage_0_7)
++24 flow(storage_heat_0_0)
++24 flow(storage_heat_0_1)
++24 flow(storage_heat_0_2)
++48.0 flow(storage_heat_0_3)
++48.0 flow(storage_heat_0_4)
++12.0 flow(storage_heat_0_5)
++12.0 flow(storage_heat_0_6)
++12.0 flow(storage_heat_0_7)
 
 s.t.
 
-c_e_BusBlock_balance(gas_0)_:
-+1 flow(gas_boiler_0)
+c_e_BusBlock_balance(heat_0_0)_:
+-1 flow(heat_storage_0_0)
++1 flow(storage_heat_0_0)
++1 flow(boiler_heat_0_0)
 = 0
 
-c_e_BusBlock_balance(gas_1)_:
-+1 flow(gas_boiler_1)
+c_e_BusBlock_balance(heat_0_1)_:
+-1 flow(heat_storage_0_1)
++1 flow(storage_heat_0_1)
++1 flow(boiler_heat_0_1)
 = 0
 
-c_e_BusBlock_balance(gas_2)_:
-+1 flow(gas_boiler_2)
+c_e_BusBlock_balance(heat_0_2)_:
+-1 flow(heat_storage_0_2)
++1 flow(storage_heat_0_2)
++1 flow(boiler_heat_0_2)
 = 0
 
-c_e_BusBlock_balance(gas_3)_:
-+1 flow(gas_boiler_3)
+c_e_BusBlock_balance(heat_0_3)_:
+-1 flow(heat_storage_0_3)
++1 flow(storage_heat_0_3)
++1 flow(boiler_heat_0_3)
 = 0
 
-c_e_BusBlock_balance(gas_4)_:
-+1 flow(gas_boiler_4)
+c_e_BusBlock_balance(heat_0_4)_:
+-1 flow(heat_storage_0_4)
++1 flow(storage_heat_0_4)
++1 flow(boiler_heat_0_4)
 = 0
 
-c_e_BusBlock_balance(gas_5)_:
-+1 flow(gas_boiler_5)
+c_e_BusBlock_balance(heat_0_5)_:
+-1 flow(heat_storage_0_5)
++1 flow(storage_heat_0_5)
++1 flow(boiler_heat_0_5)
 = 0
 
-c_e_BusBlock_balance(gas_6)_:
-+1 flow(gas_boiler_6)
+c_e_BusBlock_balance(heat_0_6)_:
+-1 flow(heat_storage_0_6)
++1 flow(storage_heat_0_6)
++1 flow(boiler_heat_0_6)
 = 0
 
-c_e_BusBlock_balance(gas_7)_:
-+1 flow(gas_boiler_7)
+c_e_BusBlock_balance(heat_0_7)_:
+-1 flow(heat_storage_0_7)
++1 flow(storage_heat_0_7)
++1 flow(boiler_heat_0_7)
 = 0
 
-c_e_BusBlock_balance(heat_0)_:
-+1 flow(boiler_heat_0)
--1 flow(heat_storage_0)
-+1 flow(storage_heat_0)
+c_e_BusBlock_balance(gas_0_0)_:
++1 flow(gas_boiler_0_0)
 = 0
 
-c_e_BusBlock_balance(heat_1)_:
-+1 flow(boiler_heat_1)
--1 flow(heat_storage_1)
-+1 flow(storage_heat_1)
+c_e_BusBlock_balance(gas_0_1)_:
++1 flow(gas_boiler_0_1)
 = 0
 
-c_e_BusBlock_balance(heat_2)_:
-+1 flow(boiler_heat_2)
--1 flow(heat_storage_2)
-+1 flow(storage_heat_2)
+c_e_BusBlock_balance(gas_0_2)_:
++1 flow(gas_boiler_0_2)
 = 0
 
-c_e_BusBlock_balance(heat_3)_:
-+1 flow(boiler_heat_3)
--1 flow(heat_storage_3)
-+1 flow(storage_heat_3)
+c_e_BusBlock_balance(gas_0_3)_:
++1 flow(gas_boiler_0_3)
 = 0
 
-c_e_BusBlock_balance(heat_4)_:
-+1 flow(boiler_heat_4)
--1 flow(heat_storage_4)
-+1 flow(storage_heat_4)
+c_e_BusBlock_balance(gas_0_4)_:
++1 flow(gas_boiler_0_4)
 = 0
 
-c_e_BusBlock_balance(heat_5)_:
-+1 flow(boiler_heat_5)
--1 flow(heat_storage_5)
-+1 flow(storage_heat_5)
+c_e_BusBlock_balance(gas_0_5)_:
++1 flow(gas_boiler_0_5)
 = 0
 
-c_e_BusBlock_balance(heat_6)_:
-+1 flow(boiler_heat_6)
--1 flow(heat_storage_6)
-+1 flow(storage_heat_6)
+c_e_BusBlock_balance(gas_0_6)_:
++1 flow(gas_boiler_0_6)
 = 0
 
-c_e_BusBlock_balance(heat_7)_:
-+1 flow(boiler_heat_7)
--1 flow(heat_storage_7)
-+1 flow(storage_heat_7)
+c_e_BusBlock_balance(gas_0_7)_:
++1 flow(gas_boiler_0_7)
 = 0
 
-c_e_TransformerBlock_relation(boiler_gas_heat_0)_:
--1 flow(boiler_heat_0)
-+1 flow(gas_boiler_0)
+c_e_TransformerBlock_relation(boiler_gas_heat_0_0)_:
++1 flow(gas_boiler_0_0)
+-1 flow(boiler_heat_0_0)
 = 0
 
-c_e_TransformerBlock_relation(boiler_gas_heat_1)_:
--1 flow(boiler_heat_1)
-+1 flow(gas_boiler_1)
+c_e_TransformerBlock_relation(boiler_gas_heat_0_1)_:
++1 flow(gas_boiler_0_1)
+-1 flow(boiler_heat_0_1)
 = 0
 
-c_e_TransformerBlock_relation(boiler_gas_heat_2)_:
--1 flow(boiler_heat_2)
-+1 flow(gas_boiler_2)
+c_e_TransformerBlock_relation(boiler_gas_heat_0_2)_:
++1 flow(gas_boiler_0_2)
+-1 flow(boiler_heat_0_2)
 = 0
 
-c_e_TransformerBlock_relation(boiler_gas_heat_3)_:
--1 flow(boiler_heat_3)
-+1 flow(gas_boiler_3)
+c_e_TransformerBlock_relation(boiler_gas_heat_0_3)_:
++1 flow(gas_boiler_0_3)
+-1 flow(boiler_heat_0_3)
 = 0
 
-c_e_TransformerBlock_relation(boiler_gas_heat_4)_:
--1 flow(boiler_heat_4)
-+1 flow(gas_boiler_4)
+c_e_TransformerBlock_relation(boiler_gas_heat_0_4)_:
++1 flow(gas_boiler_0_4)
+-1 flow(boiler_heat_0_4)
 = 0
 
-c_e_TransformerBlock_relation(boiler_gas_heat_5)_:
--1 flow(boiler_heat_5)
-+1 flow(gas_boiler_5)
+c_e_TransformerBlock_relation(boiler_gas_heat_0_5)_:
++1 flow(gas_boiler_0_5)
+-1 flow(boiler_heat_0_5)
 = 0
 
-c_e_TransformerBlock_relation(boiler_gas_heat_6)_:
--1 flow(boiler_heat_6)
-+1 flow(gas_boiler_6)
+c_e_TransformerBlock_relation(boiler_gas_heat_0_6)_:
++1 flow(gas_boiler_0_6)
+-1 flow(boiler_heat_0_6)
 = 0
 
-c_e_TransformerBlock_relation(boiler_gas_heat_7)_:
--1 flow(boiler_heat_7)
-+1 flow(gas_boiler_7)
+c_e_TransformerBlock_relation(boiler_gas_heat_0_7)_:
++1 flow(gas_boiler_0_7)
+-1 flow(boiler_heat_0_7)
 = 0
 
-c_e_GenericStorageBlock_balance(storage_0)_:
+c_e_GenericStorageBlock_balance(storage_0_0)_:
+-1 flow(heat_storage_0_0)
++1 flow(storage_heat_0_0)
 +1 GenericStorageBlock_storage_content(storage_1)
--1 flow(heat_storage_0)
-+1 flow(storage_heat_0)
-= 270
+= 270.0
 
-c_e_GenericStorageBlock_balance(storage_1)_:
--0.90000000000000002 GenericStorageBlock_storage_content(storage_1)
+c_e_GenericStorageBlock_balance(storage_0_1)_:
+-1 flow(heat_storage_0_1)
++1 flow(storage_heat_0_1)
+-0.9 GenericStorageBlock_storage_content(storage_1)
 +1 GenericStorageBlock_storage_content(storage_2)
--1 flow(heat_storage_1)
-+1 flow(storage_heat_1)
 = 0
 
-c_e_GenericStorageBlock_balance(storage_2)_:
--0.90000000000000002 GenericStorageBlock_storage_content(storage_2)
+c_e_GenericStorageBlock_balance(storage_0_2)_:
+-1 flow(heat_storage_0_2)
++1 flow(storage_heat_0_2)
+-0.9 GenericStorageBlock_storage_content(storage_2)
 +1 GenericStorageBlock_storage_content(storage_3)
--1 flow(heat_storage_2)
-+1 flow(storage_heat_2)
 = 0
 
-c_e_GenericStorageBlock_balance(storage_3)_:
--0.81000000000000005 GenericStorageBlock_storage_content(storage_3)
+c_e_GenericStorageBlock_balance(storage_0_3)_:
+-2.0 flow(heat_storage_0_3)
++2.0 flow(storage_heat_0_3)
+-0.81 GenericStorageBlock_storage_content(storage_3)
 +1 GenericStorageBlock_storage_content(storage_4)
--2 flow(heat_storage_3)
-+2 flow(storage_heat_3)
 = 0
 
-c_e_GenericStorageBlock_balance(storage_4)_:
--0.81000000000000005 GenericStorageBlock_storage_content(storage_4)
+c_e_GenericStorageBlock_balance(storage_0_4)_:
+-2.0 flow(heat_storage_0_4)
++2.0 flow(storage_heat_0_4)
+-0.81 GenericStorageBlock_storage_content(storage_4)
 +1 GenericStorageBlock_storage_content(storage_5)
--2 flow(heat_storage_4)
-+2 flow(storage_heat_4)
 = 0
 
-c_e_GenericStorageBlock_balance(storage_5)_:
--0.94868329805051377 GenericStorageBlock_storage_content(storage_5)
+c_e_GenericStorageBlock_balance(storage_0_5)_:
+-0.5 flow(heat_storage_0_5)
++0.5 flow(storage_heat_0_5)
+-0.9486832980505138 GenericStorageBlock_storage_content(storage_5)
 +1 GenericStorageBlock_storage_content(storage_6)
--0.5 flow(heat_storage_5)
-+0.5 flow(storage_heat_5)
 = 0
 
-c_e_GenericStorageBlock_balance(storage_6)_:
--0.94868329805051377 GenericStorageBlock_storage_content(storage_6)
+c_e_GenericStorageBlock_balance(storage_0_6)_:
+-0.5 flow(heat_storage_0_6)
++0.5 flow(storage_heat_0_6)
+-0.9486832980505138 GenericStorageBlock_storage_content(storage_6)
 +1 GenericStorageBlock_storage_content(storage_7)
--0.5 flow(heat_storage_6)
-+0.5 flow(storage_heat_6)
 = 0
 
-c_e_GenericStorageBlock_balance(storage_7)_:
--0.94868329805051377 GenericStorageBlock_storage_content(storage_7)
+c_e_GenericStorageBlock_balance(storage_0_7)_:
+-0.5 flow(heat_storage_0_7)
++0.5 flow(storage_heat_0_7)
+-0.9486832980505138 GenericStorageBlock_storage_content(storage_7)
 +1 GenericStorageBlock_storage_content(storage_8)
--0.5 flow(heat_storage_7)
-+0.5 flow(storage_heat_7)
 = 0
 
 c_e_GenericStorageBlock_balanced_cstr(storage)_:
 +1 GenericStorageBlock_storage_content(storage_8)
 = 300
 
-c_e_ONE_VAR_CONSTANT:
-ONE_VAR_CONSTANT = 1.0
-
 bounds
-   0 <= flow(boiler_heat_0) <= 200
-   0 <= flow(boiler_heat_1) <= 200
-   0 <= flow(boiler_heat_2) <= 200
-   0 <= flow(boiler_heat_3) <= 200
-   0 <= flow(boiler_heat_4) <= 200
-   0 <= flow(boiler_heat_5) <= 200
-   0 <= flow(boiler_heat_6) <= 200
-   0 <= flow(boiler_heat_7) <= 200
-   0 <= flow(gas_boiler_0) <= +inf
-   0 <= flow(gas_boiler_1) <= +inf
-   0 <= flow(gas_boiler_2) <= +inf
-   0 <= flow(gas_boiler_3) <= +inf
-   0 <= flow(gas_boiler_4) <= +inf
-   0 <= flow(gas_boiler_5) <= +inf
-   0 <= flow(gas_boiler_6) <= +inf
-   0 <= flow(gas_boiler_7) <= +inf
-   0 <= flow(heat_storage_0) <= 100
-   0 <= flow(heat_storage_1) <= 100
-   0 <= flow(heat_storage_2) <= 100
-   0 <= flow(heat_storage_3) <= 100
-   0 <= flow(heat_storage_4) <= 100
-   0 <= flow(heat_storage_5) <= 100
-   0 <= flow(heat_storage_6) <= 100
-   0 <= flow(heat_storage_7) <= 100
-   0 <= flow(storage_heat_0) <= 100
-   0 <= flow(storage_heat_1) <= 100
-   0 <= flow(storage_heat_2) <= 100
-   0 <= flow(storage_heat_3) <= 100
-   0 <= flow(storage_heat_4) <= 100
-   0 <= flow(storage_heat_5) <= 100
-   0 <= flow(storage_heat_6) <= 100
-   0 <= flow(storage_heat_7) <= 100
+   0 <= flow(gas_boiler_0_0) <= +inf
+   0 <= flow(gas_boiler_0_1) <= +inf
+   0 <= flow(gas_boiler_0_2) <= +inf
+   0 <= flow(gas_boiler_0_3) <= +inf
+   0 <= flow(gas_boiler_0_4) <= +inf
+   0 <= flow(gas_boiler_0_5) <= +inf
+   0 <= flow(gas_boiler_0_6) <= +inf
+   0 <= flow(gas_boiler_0_7) <= +inf
+   0 <= flow(heat_storage_0_0) <= 100
+   0 <= flow(heat_storage_0_1) <= 100
+   0 <= flow(heat_storage_0_2) <= 100
+   0 <= flow(heat_storage_0_3) <= 100
+   0 <= flow(heat_storage_0_4) <= 100
+   0 <= flow(heat_storage_0_5) <= 100
+   0 <= flow(heat_storage_0_6) <= 100
+   0 <= flow(heat_storage_0_7) <= 100
+   0 <= flow(storage_heat_0_0) <= 100
+   0 <= flow(storage_heat_0_1) <= 100
+   0 <= flow(storage_heat_0_2) <= 100
+   0 <= flow(storage_heat_0_3) <= 100
+   0 <= flow(storage_heat_0_4) <= 100
+   0 <= flow(storage_heat_0_5) <= 100
+   0 <= flow(storage_heat_0_6) <= 100
+   0 <= flow(storage_heat_0_7) <= 100
+   0 <= flow(boiler_heat_0_0) <= 200
+   0 <= flow(boiler_heat_0_1) <= 200
+   0 <= flow(boiler_heat_0_2) <= 200
+   0 <= flow(boiler_heat_0_3) <= 200
+   0 <= flow(boiler_heat_0_4) <= 200
+   0 <= flow(boiler_heat_0_5) <= 200
+   0 <= flow(boiler_heat_0_6) <= 200
+   0 <= flow(boiler_heat_0_7) <= 200
    0 <= GenericStorageBlock_storage_content(storage_1) <= 300
    0 <= GenericStorageBlock_storage_content(storage_2) <= 300
    0 <= GenericStorageBlock_storage_content(storage_3) <= 300
    0 <= GenericStorageBlock_storage_content(storage_4) <= 300
    0 <= GenericStorageBlock_storage_content(storage_5) <= 300
    0 <= GenericStorageBlock_storage_content(storage_6) <= 300
    0 <= GenericStorageBlock_storage_content(storage_7) <= 300
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/piecewise_linear_transformer_cc.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/piecewise_linear_transformer_cc.lp`

 * *Files 12% similar despite different names*

```diff
@@ -1,69 +1,69 @@
 \* Source Pyomo model name=Model *\
 
-min
+min 
 objective:
-+1 flow(gasBus_pwltf_0)
-+1 flow(gasBus_pwltf_1)
-+1 flow(gasBus_pwltf_2)
++1 flow(gasBus_pwltf_0_0)
++1 flow(gasBus_pwltf_0_1)
++1 flow(gasBus_pwltf_0_2)
 
 s.t.
 
-c_e_BusBlock_balance(electricityBus_0)_:
-+1 flow(pwltf_electricityBus_0)
+c_e_BusBlock_balance(gasBus_0_0)_:
++1 flow(gasBus_pwltf_0_0)
 = 0
 
-c_e_BusBlock_balance(electricityBus_1)_:
-+1 flow(pwltf_electricityBus_1)
+c_e_BusBlock_balance(gasBus_0_1)_:
++1 flow(gasBus_pwltf_0_1)
 = 0
 
-c_e_BusBlock_balance(electricityBus_2)_:
-+1 flow(pwltf_electricityBus_2)
+c_e_BusBlock_balance(gasBus_0_2)_:
++1 flow(gasBus_pwltf_0_2)
 = 0
 
-c_e_BusBlock_balance(gasBus_0)_:
-+1 flow(gasBus_pwltf_0)
+c_e_BusBlock_balance(electricityBus_0_0)_:
++1 flow(pwltf_electricityBus_0_0)
 = 0
 
-c_e_BusBlock_balance(gasBus_1)_:
-+1 flow(gasBus_pwltf_1)
+c_e_BusBlock_balance(electricityBus_0_1)_:
++1 flow(pwltf_electricityBus_0_1)
 = 0
 
-c_e_BusBlock_balance(gasBus_2)_:
-+1 flow(gasBus_pwltf_2)
+c_e_BusBlock_balance(electricityBus_0_2)_:
++1 flow(pwltf_electricityBus_0_2)
 = 0
 
-c_e_PiecewiseLinearTransformerBlock_equate_in(pwltf_0)_:
+c_e_PiecewiseLinearTransformerBlock_equate_in(pwltf_0_0)_:
+-1 flow(gasBus_pwltf_0_0)
 +1 PiecewiseLinearTransformerBlock_inflow(pwltf_0)
--1 flow(gasBus_pwltf_0)
 = 0
 
-c_e_PiecewiseLinearTransformerBlock_equate_in(pwltf_1)_:
+c_e_PiecewiseLinearTransformerBlock_equate_in(pwltf_0_1)_:
+-1 flow(gasBus_pwltf_0_1)
 +1 PiecewiseLinearTransformerBlock_inflow(pwltf_1)
--1 flow(gasBus_pwltf_1)
 = 0
 
-c_e_PiecewiseLinearTransformerBlock_equate_in(pwltf_2)_:
+c_e_PiecewiseLinearTransformerBlock_equate_in(pwltf_0_2)_:
+-1 flow(gasBus_pwltf_0_2)
 +1 PiecewiseLinearTransformerBlock_inflow(pwltf_2)
--1 flow(gasBus_pwltf_2)
 = 0
 
-c_e_PiecewiseLinearTransformerBlock_equate_out(pwltf_0)_:
+c_e_PiecewiseLinearTransformerBlock_equate_out(pwltf_0_0)_:
+-1 flow(pwltf_electricityBus_0_0)
 +1 PiecewiseLinearTransformerBlock_outflow(pwltf_0)
--1 flow(pwltf_electricityBus_0)
 = 0
 
-c_e_PiecewiseLinearTransformerBlock_equate_out(pwltf_1)_:
+c_e_PiecewiseLinearTransformerBlock_equate_out(pwltf_0_1)_:
+-1 flow(pwltf_electricityBus_0_1)
 +1 PiecewiseLinearTransformerBlock_outflow(pwltf_1)
--1 flow(pwltf_electricityBus_1)
 = 0
 
-c_e_PiecewiseLinearTransformerBlock_equate_out(pwltf_2)_:
+c_e_PiecewiseLinearTransformerBlock_equate_out(pwltf_0_2)_:
+-1 flow(pwltf_electricityBus_0_2)
 +1 PiecewiseLinearTransformerBlock_outflow(pwltf_2)
--1 flow(pwltf_electricityBus_2)
 = 0
 
 c_e_PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_constraint1_:
 +1 PiecewiseLinearTransformerBlock_inflow(pwltf_0)
 -25 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_lambda(2)
 -50 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_lambda(3)
 -75 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_lambda(4)
@@ -75,47 +75,47 @@
 -625 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_lambda(2)
 -2500 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_lambda(3)
 -5625 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_lambda(4)
 -10000 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_lambda(5)
 = 0
 
 c_e_PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_constraint3_:
-+1 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_lambda(1)
 +1 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_lambda(2)
 +1 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_lambda(3)
 +1 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_lambda(4)
 +1 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_lambda(5)
++1 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_lambda(1)
 = 1
 
 c_u_PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_constraint4(1)_:
--1 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_bin_y(1)
 +1 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_lambda(1)
+-1 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_bin_y(1)
 <= 0
 
 c_u_PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_constraint4(2)_:
++1 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_lambda(2)
 -1 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_bin_y(1)
 -1 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_bin_y(2)
-+1 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_lambda(2)
 <= 0
 
 c_u_PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_constraint4(3)_:
++1 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_lambda(3)
 -1 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_bin_y(2)
 -1 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_bin_y(3)
-+1 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_lambda(3)
 <= 0
 
 c_u_PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_constraint4(4)_:
++1 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_lambda(4)
 -1 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_bin_y(3)
 -1 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_bin_y(4)
-+1 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_lambda(4)
 <= 0
 
 c_u_PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_constraint4(5)_:
--1 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_bin_y(4)
 +1 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_lambda(5)
+-1 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_bin_y(4)
 <= 0
 
 c_e_PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_constraint5_:
 +1 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_bin_y(1)
 +1 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_bin_y(2)
 +1 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_bin_y(3)
 +1 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_bin_y(4)
@@ -134,47 +134,47 @@
 -625 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_lambda(2)
 -2500 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_lambda(3)
 -5625 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_lambda(4)
 -10000 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_lambda(5)
 = 0
 
 c_e_PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_constraint3_:
-+1 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_lambda(1)
 +1 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_lambda(2)
 +1 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_lambda(3)
 +1 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_lambda(4)
 +1 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_lambda(5)
++1 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_lambda(1)
 = 1
 
 c_u_PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_constraint4(1)_:
--1 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_bin_y(1)
 +1 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_lambda(1)
+-1 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_bin_y(1)
 <= 0
 
 c_u_PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_constraint4(2)_:
++1 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_lambda(2)
 -1 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_bin_y(1)
 -1 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_bin_y(2)
-+1 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_lambda(2)
 <= 0
 
 c_u_PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_constraint4(3)_:
++1 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_lambda(3)
 -1 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_bin_y(2)
 -1 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_bin_y(3)
-+1 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_lambda(3)
 <= 0
 
 c_u_PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_constraint4(4)_:
++1 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_lambda(4)
 -1 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_bin_y(3)
 -1 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_bin_y(4)
-+1 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_lambda(4)
 <= 0
 
 c_u_PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_constraint4(5)_:
--1 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_bin_y(4)
 +1 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_lambda(5)
+-1 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_bin_y(4)
 <= 0
 
 c_e_PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_constraint5_:
 +1 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_bin_y(1)
 +1 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_bin_y(2)
 +1 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_bin_y(3)
 +1 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_bin_y(4)
@@ -193,95 +193,92 @@
 -625 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_lambda(2)
 -2500 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_lambda(3)
 -5625 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_lambda(4)
 -10000 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_lambda(5)
 = 0
 
 c_e_PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_constraint3_:
-+1 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_lambda(1)
 +1 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_lambda(2)
 +1 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_lambda(3)
 +1 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_lambda(4)
 +1 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_lambda(5)
++1 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_lambda(1)
 = 1
 
 c_u_PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_constraint4(1)_:
--1 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_bin_y(1)
 +1 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_lambda(1)
+-1 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_bin_y(1)
 <= 0
 
 c_u_PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_constraint4(2)_:
++1 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_lambda(2)
 -1 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_bin_y(1)
 -1 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_bin_y(2)
-+1 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_lambda(2)
 <= 0
 
 c_u_PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_constraint4(3)_:
++1 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_lambda(3)
 -1 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_bin_y(2)
 -1 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_bin_y(3)
-+1 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_lambda(3)
 <= 0
 
 c_u_PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_constraint4(4)_:
++1 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_lambda(4)
 -1 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_bin_y(3)
 -1 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_bin_y(4)
-+1 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_lambda(4)
 <= 0
 
 c_u_PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_constraint4(5)_:
--1 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_bin_y(4)
 +1 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_lambda(5)
+-1 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_bin_y(4)
 <= 0
 
 c_e_PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_constraint5_:
 +1 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_bin_y(1)
 +1 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_bin_y(2)
 +1 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_bin_y(3)
 +1 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_bin_y(4)
 = 1
 
-c_e_ONE_VAR_CONSTANT:
-ONE_VAR_CONSTANT = 1.0
-
 bounds
-   0 <= flow(gasBus_pwltf_0) <= 100
-   0 <= flow(gasBus_pwltf_1) <= 100
-   0 <= flow(gasBus_pwltf_2) <= 100
-   0 <= flow(pwltf_electricityBus_0) <= +inf
-   0 <= flow(pwltf_electricityBus_1) <= +inf
-   0 <= flow(pwltf_electricityBus_2) <= +inf
+   0 <= flow(gasBus_pwltf_0_0) <= 100
+   0 <= flow(gasBus_pwltf_0_1) <= 100
+   0 <= flow(gasBus_pwltf_0_2) <= 100
+   0 <= flow(pwltf_electricityBus_0_0) <= +inf
+   0 <= flow(pwltf_electricityBus_0_1) <= +inf
+   0 <= flow(pwltf_electricityBus_0_2) <= +inf
    0 <= PiecewiseLinearTransformerBlock_inflow(pwltf_0) <= 100
    0 <= PiecewiseLinearTransformerBlock_inflow(pwltf_1) <= 100
    0 <= PiecewiseLinearTransformerBlock_inflow(pwltf_2) <= 100
    0 <= PiecewiseLinearTransformerBlock_outflow(pwltf_0) <= 10000
    0 <= PiecewiseLinearTransformerBlock_outflow(pwltf_1) <= 10000
    0 <= PiecewiseLinearTransformerBlock_outflow(pwltf_2) <= 10000
-   0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_lambda(1) <= +inf
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_lambda(2) <= +inf
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_lambda(3) <= +inf
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_lambda(4) <= +inf
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_lambda(5) <= +inf
+   0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_lambda(1) <= +inf
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_bin_y(1) <= 1
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_bin_y(2) <= 1
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_bin_y(3) <= 1
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_bin_y(4) <= 1
-   0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_lambda(1) <= +inf
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_lambda(2) <= +inf
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_lambda(3) <= +inf
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_lambda(4) <= +inf
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_lambda(5) <= +inf
+   0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_lambda(1) <= +inf
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_bin_y(1) <= 1
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_bin_y(2) <= 1
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_bin_y(3) <= 1
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_CC_bin_y(4) <= 1
-   0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_lambda(1) <= +inf
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_lambda(2) <= +inf
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_lambda(3) <= +inf
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_lambda(4) <= +inf
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_lambda(5) <= +inf
+   0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_lambda(1) <= +inf
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_bin_y(1) <= 1
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_bin_y(2) <= 1
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_bin_y(3) <= 1
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_CC_bin_y(4) <= 1
 binary
   PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_bin_y(1)
   PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_CC_bin_y(2)
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/piecewise_linear_transformer_dcc.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/piecewise_linear_transformer_dcc.lp`

 * *Files 4% similar despite different names*

```diff
@@ -1,69 +1,69 @@
 \* Source Pyomo model name=Model *\
 
-min
+min 
 objective:
-+1 flow(gasBus_pwltf_0)
-+1 flow(gasBus_pwltf_1)
-+1 flow(gasBus_pwltf_2)
++1 flow(gasBus_pwltf_0_0)
++1 flow(gasBus_pwltf_0_1)
++1 flow(gasBus_pwltf_0_2)
 
 s.t.
 
-c_e_BusBlock_balance(electricityBus_0)_:
-+1 flow(pwltf_electricityBus_0)
+c_e_BusBlock_balance(gasBus_0_0)_:
++1 flow(gasBus_pwltf_0_0)
 = 0
 
-c_e_BusBlock_balance(electricityBus_1)_:
-+1 flow(pwltf_electricityBus_1)
+c_e_BusBlock_balance(gasBus_0_1)_:
++1 flow(gasBus_pwltf_0_1)
 = 0
 
-c_e_BusBlock_balance(electricityBus_2)_:
-+1 flow(pwltf_electricityBus_2)
+c_e_BusBlock_balance(gasBus_0_2)_:
++1 flow(gasBus_pwltf_0_2)
 = 0
 
-c_e_BusBlock_balance(gasBus_0)_:
-+1 flow(gasBus_pwltf_0)
+c_e_BusBlock_balance(electricityBus_0_0)_:
++1 flow(pwltf_electricityBus_0_0)
 = 0
 
-c_e_BusBlock_balance(gasBus_1)_:
-+1 flow(gasBus_pwltf_1)
+c_e_BusBlock_balance(electricityBus_0_1)_:
++1 flow(pwltf_electricityBus_0_1)
 = 0
 
-c_e_BusBlock_balance(gasBus_2)_:
-+1 flow(gasBus_pwltf_2)
+c_e_BusBlock_balance(electricityBus_0_2)_:
++1 flow(pwltf_electricityBus_0_2)
 = 0
 
-c_e_PiecewiseLinearTransformerBlock_equate_in(pwltf_0)_:
+c_e_PiecewiseLinearTransformerBlock_equate_in(pwltf_0_0)_:
+-1 flow(gasBus_pwltf_0_0)
 +1 PiecewiseLinearTransformerBlock_inflow(pwltf_0)
--1 flow(gasBus_pwltf_0)
 = 0
 
-c_e_PiecewiseLinearTransformerBlock_equate_in(pwltf_1)_:
+c_e_PiecewiseLinearTransformerBlock_equate_in(pwltf_0_1)_:
+-1 flow(gasBus_pwltf_0_1)
 +1 PiecewiseLinearTransformerBlock_inflow(pwltf_1)
--1 flow(gasBus_pwltf_1)
 = 0
 
-c_e_PiecewiseLinearTransformerBlock_equate_in(pwltf_2)_:
+c_e_PiecewiseLinearTransformerBlock_equate_in(pwltf_0_2)_:
+-1 flow(gasBus_pwltf_0_2)
 +1 PiecewiseLinearTransformerBlock_inflow(pwltf_2)
--1 flow(gasBus_pwltf_2)
 = 0
 
-c_e_PiecewiseLinearTransformerBlock_equate_out(pwltf_0)_:
+c_e_PiecewiseLinearTransformerBlock_equate_out(pwltf_0_0)_:
+-1 flow(pwltf_electricityBus_0_0)
 +1 PiecewiseLinearTransformerBlock_outflow(pwltf_0)
--1 flow(pwltf_electricityBus_0)
 = 0
 
-c_e_PiecewiseLinearTransformerBlock_equate_out(pwltf_1)_:
+c_e_PiecewiseLinearTransformerBlock_equate_out(pwltf_0_1)_:
+-1 flow(pwltf_electricityBus_0_1)
 +1 PiecewiseLinearTransformerBlock_outflow(pwltf_1)
--1 flow(pwltf_electricityBus_1)
 = 0
 
-c_e_PiecewiseLinearTransformerBlock_equate_out(pwltf_2)_:
+c_e_PiecewiseLinearTransformerBlock_equate_out(pwltf_0_2)_:
+-1 flow(pwltf_electricityBus_0_2)
 +1 PiecewiseLinearTransformerBlock_outflow(pwltf_2)
--1 flow(pwltf_electricityBus_2)
 = 0
 
 c_e_PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_constraint1_:
 +1 PiecewiseLinearTransformerBlock_inflow(pwltf_0)
 -25 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_lambda(1_2)
 -25 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_lambda(2_2)
 -50 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_lambda(2_3)
@@ -81,35 +81,35 @@
 -2500 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_lambda(3_3)
 -5625 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_lambda(3_4)
 -5625 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_lambda(4_4)
 -10000 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_lambda(4_5)
 = 0
 
 c_e_PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_constraint3(1)_:
+-1 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_lambda(1_2)
 +1 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_bin_y(1)
 -1 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_lambda(1_1)
--1 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_lambda(1_2)
 = 0
 
 c_e_PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_constraint3(2)_:
-+1 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_bin_y(2)
 -1 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_lambda(2_2)
 -1 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_lambda(2_3)
++1 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_bin_y(2)
 = 0
 
 c_e_PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_constraint3(3)_:
-+1 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_bin_y(3)
 -1 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_lambda(3_3)
 -1 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_lambda(3_4)
++1 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_bin_y(3)
 = 0
 
 c_e_PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_constraint3(4)_:
-+1 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_bin_y(4)
 -1 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_lambda(4_4)
 -1 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_lambda(4_5)
++1 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_bin_y(4)
 = 0
 
 c_e_PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_constraint4_:
 +1 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_bin_y(1)
 +1 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_bin_y(2)
 +1 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_bin_y(3)
 +1 PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_bin_y(4)
@@ -134,35 +134,35 @@
 -2500 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_DCC_lambda(3_3)
 -5625 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_DCC_lambda(3_4)
 -5625 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_DCC_lambda(4_4)
 -10000 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_DCC_lambda(4_5)
 = 0
 
 c_e_PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_DCC_constraint3(1)_:
+-1 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_DCC_lambda(1_2)
 +1 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_DCC_bin_y(1)
 -1 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_DCC_lambda(1_1)
--1 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_DCC_lambda(1_2)
 = 0
 
 c_e_PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_DCC_constraint3(2)_:
-+1 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_DCC_bin_y(2)
 -1 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_DCC_lambda(2_2)
 -1 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_DCC_lambda(2_3)
++1 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_DCC_bin_y(2)
 = 0
 
 c_e_PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_DCC_constraint3(3)_:
-+1 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_DCC_bin_y(3)
 -1 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_DCC_lambda(3_3)
 -1 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_DCC_lambda(3_4)
++1 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_DCC_bin_y(3)
 = 0
 
 c_e_PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_DCC_constraint3(4)_:
-+1 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_DCC_bin_y(4)
 -1 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_DCC_lambda(4_4)
 -1 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_DCC_lambda(4_5)
++1 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_DCC_bin_y(4)
 = 0
 
 c_e_PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_DCC_constraint4_:
 +1 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_DCC_bin_y(1)
 +1 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_DCC_bin_y(2)
 +1 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_DCC_bin_y(3)
 +1 PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_DCC_bin_y(4)
@@ -187,93 +187,90 @@
 -2500 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_DCC_lambda(3_3)
 -5625 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_DCC_lambda(3_4)
 -5625 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_DCC_lambda(4_4)
 -10000 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_DCC_lambda(4_5)
 = 0
 
 c_e_PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_DCC_constraint3(1)_:
+-1 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_DCC_lambda(1_2)
 +1 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_DCC_bin_y(1)
 -1 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_DCC_lambda(1_1)
--1 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_DCC_lambda(1_2)
 = 0
 
 c_e_PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_DCC_constraint3(2)_:
-+1 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_DCC_bin_y(2)
 -1 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_DCC_lambda(2_2)
 -1 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_DCC_lambda(2_3)
++1 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_DCC_bin_y(2)
 = 0
 
 c_e_PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_DCC_constraint3(3)_:
-+1 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_DCC_bin_y(3)
 -1 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_DCC_lambda(3_3)
 -1 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_DCC_lambda(3_4)
++1 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_DCC_bin_y(3)
 = 0
 
 c_e_PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_DCC_constraint3(4)_:
-+1 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_DCC_bin_y(4)
 -1 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_DCC_lambda(4_4)
 -1 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_DCC_lambda(4_5)
++1 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_DCC_bin_y(4)
 = 0
 
 c_e_PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_DCC_constraint4_:
 +1 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_DCC_bin_y(1)
 +1 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_DCC_bin_y(2)
 +1 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_DCC_bin_y(3)
 +1 PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_DCC_bin_y(4)
 = 1
 
-c_e_ONE_VAR_CONSTANT:
-ONE_VAR_CONSTANT = 1.0
-
 bounds
-   0 <= flow(gasBus_pwltf_0) <= 100
-   0 <= flow(gasBus_pwltf_1) <= 100
-   0 <= flow(gasBus_pwltf_2) <= 100
-   0 <= flow(pwltf_electricityBus_0) <= +inf
-   0 <= flow(pwltf_electricityBus_1) <= +inf
-   0 <= flow(pwltf_electricityBus_2) <= +inf
+   0 <= flow(gasBus_pwltf_0_0) <= 100
+   0 <= flow(gasBus_pwltf_0_1) <= 100
+   0 <= flow(gasBus_pwltf_0_2) <= 100
+   0 <= flow(pwltf_electricityBus_0_0) <= +inf
+   0 <= flow(pwltf_electricityBus_0_1) <= +inf
+   0 <= flow(pwltf_electricityBus_0_2) <= +inf
    0 <= PiecewiseLinearTransformerBlock_inflow(pwltf_0) <= 100
    0 <= PiecewiseLinearTransformerBlock_inflow(pwltf_1) <= 100
    0 <= PiecewiseLinearTransformerBlock_inflow(pwltf_2) <= 100
    0 <= PiecewiseLinearTransformerBlock_outflow(pwltf_0) <= 10000
    0 <= PiecewiseLinearTransformerBlock_outflow(pwltf_1) <= 10000
    0 <= PiecewiseLinearTransformerBlock_outflow(pwltf_2) <= 10000
-   0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_lambda(1_1) <= +inf
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_lambda(1_2) <= +inf
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_lambda(2_2) <= +inf
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_lambda(2_3) <= +inf
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_lambda(3_3) <= +inf
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_lambda(3_4) <= +inf
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_lambda(4_4) <= +inf
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_lambda(4_5) <= +inf
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_bin_y(1) <= 1
+   0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_lambda(1_1) <= +inf
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_bin_y(2) <= 1
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_bin_y(3) <= 1
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_bin_y(4) <= 1
-   0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_DCC_lambda(1_1) <= +inf
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_DCC_lambda(1_2) <= +inf
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_DCC_lambda(2_2) <= +inf
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_DCC_lambda(2_3) <= +inf
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_DCC_lambda(3_3) <= +inf
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_DCC_lambda(3_4) <= +inf
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_DCC_lambda(4_4) <= +inf
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_DCC_lambda(4_5) <= +inf
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_DCC_bin_y(1) <= 1
+   0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_DCC_lambda(1_1) <= +inf
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_DCC_bin_y(2) <= 1
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_DCC_bin_y(3) <= 1
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_1)_DCC_bin_y(4) <= 1
-   0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_DCC_lambda(1_1) <= +inf
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_DCC_lambda(1_2) <= +inf
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_DCC_lambda(2_2) <= +inf
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_DCC_lambda(2_3) <= +inf
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_DCC_lambda(3_3) <= +inf
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_DCC_lambda(3_4) <= +inf
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_DCC_lambda(4_4) <= +inf
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_DCC_lambda(4_5) <= +inf
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_DCC_bin_y(1) <= 1
+   0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_DCC_lambda(1_1) <= +inf
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_DCC_bin_y(2) <= 1
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_DCC_bin_y(3) <= 1
    0 <= PiecewiseLinearTransformerBlock_piecewise(pwltf_2)_DCC_bin_y(4) <= 1
 binary
   PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_bin_y(1)
   PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_bin_y(2)
   PiecewiseLinearTransformerBlock_piecewise(pwltf_0)_DCC_bin_y(3)
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/shared_limit.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/shared_limit.lp`

 * *Files 5% similar despite different names*

```diff
@@ -20,108 +20,106 @@
 
 c_e_limit_storage_constraint(2)_:
 +0.5 GenericStorageBlock_storage_content(storage1_2)
 +1.25 GenericStorageBlock_storage_content(storage2_2)
 -1 limit_storage(2)
 = 0
 
-c_e_BusBlock_balance(bus_0)_:
--1 flow(bus_storage1_0)
--1 flow(bus_storage2_0)
-+1 flow(storage1_bus_0)
-+1 flow(storage2_bus_0)
+c_e_BusBlock_balance(bus_0_0)_:
++1 flow(storage1_bus_0_0)
++1 flow(storage2_bus_0_0)
+-1 flow(bus_storage1_0_0)
+-1 flow(bus_storage2_0_0)
 = 0
 
-c_e_BusBlock_balance(bus_1)_:
--1 flow(bus_storage1_1)
--1 flow(bus_storage2_1)
-+1 flow(storage1_bus_1)
-+1 flow(storage2_bus_1)
+c_e_BusBlock_balance(bus_0_1)_:
++1 flow(storage1_bus_0_1)
++1 flow(storage2_bus_0_1)
+-1 flow(bus_storage1_0_1)
+-1 flow(bus_storage2_0_1)
 = 0
 
-c_e_BusBlock_balance(bus_2)_:
--1 flow(bus_storage1_2)
--1 flow(bus_storage2_2)
-+1 flow(storage1_bus_2)
-+1 flow(storage2_bus_2)
+c_e_BusBlock_balance(bus_0_2)_:
++1 flow(storage1_bus_0_2)
++1 flow(storage2_bus_0_2)
+-1 flow(bus_storage1_0_2)
+-1 flow(bus_storage2_0_2)
 = 0
 
-c_e_GenericStorageBlock_balance(storage1_0)_:
+c_e_GenericStorageBlock_balance(storage1_0_0)_:
 -1 GenericStorageBlock_storage_content(storage1_0)
 +1 GenericStorageBlock_storage_content(storage1_1)
--1 flow(bus_storage1_0)
-+1 flow(storage1_bus_0)
++1 flow(storage1_bus_0_0)
+-1 flow(bus_storage1_0_0)
 = 0
 
-c_e_GenericStorageBlock_balance(storage1_1)_:
+c_e_GenericStorageBlock_balance(storage1_0_1)_:
 -1 GenericStorageBlock_storage_content(storage1_1)
 +1 GenericStorageBlock_storage_content(storage1_2)
--1 flow(bus_storage1_1)
-+1 flow(storage1_bus_1)
++1 flow(storage1_bus_0_1)
+-1 flow(bus_storage1_0_1)
 = 0
 
-c_e_GenericStorageBlock_balance(storage1_2)_:
+c_e_GenericStorageBlock_balance(storage1_0_2)_:
 -1 GenericStorageBlock_storage_content(storage1_2)
++1 flow(storage1_bus_0_2)
+-1 flow(bus_storage1_0_2)
 +1 GenericStorageBlock_storage_content(storage1_3)
--1 flow(bus_storage1_2)
-+1 flow(storage1_bus_2)
 = 0
 
-c_e_GenericStorageBlock_balance(storage2_0)_:
+c_e_GenericStorageBlock_balance(storage2_0_0)_:
 -1 GenericStorageBlock_storage_content(storage2_0)
 +1 GenericStorageBlock_storage_content(storage2_1)
--1 flow(bus_storage2_0)
-+1 flow(storage2_bus_0)
++1 flow(storage2_bus_0_0)
+-1 flow(bus_storage2_0_0)
 = 0
 
-c_e_GenericStorageBlock_balance(storage2_1)_:
+c_e_GenericStorageBlock_balance(storage2_0_1)_:
 -1 GenericStorageBlock_storage_content(storage2_1)
 +1 GenericStorageBlock_storage_content(storage2_2)
--1 flow(bus_storage2_1)
-+1 flow(storage2_bus_1)
++1 flow(storage2_bus_0_1)
+-1 flow(bus_storage2_0_1)
 = 0
 
-c_e_GenericStorageBlock_balance(storage2_2)_:
+c_e_GenericStorageBlock_balance(storage2_0_2)_:
 -1 GenericStorageBlock_storage_content(storage2_2)
++1 flow(storage2_bus_0_2)
+-1 flow(bus_storage2_0_2)
 +1 GenericStorageBlock_storage_content(storage2_3)
--1 flow(bus_storage2_2)
-+1 flow(storage2_bus_2)
 = 0
 
 c_e_GenericStorageBlock_balanced_cstr(storage1)_:
 -1 GenericStorageBlock_storage_content(storage1_0)
 +1 GenericStorageBlock_storage_content(storage1_3)
 = 0
 
 c_e_GenericStorageBlock_balanced_cstr(storage2)_:
 -1 GenericStorageBlock_storage_content(storage2_0)
 +1 GenericStorageBlock_storage_content(storage2_3)
 = 0
 
-c_e_ONE_VAR_CONSTANT: 
-ONE_VAR_CONSTANT = 1.0
-
 bounds
-   0 <= flow(bus_storage1_0) <= +inf
-   0 <= flow(bus_storage1_1) <= +inf
-   0 <= flow(bus_storage1_2) <= +inf
-   0 <= flow(bus_storage2_0) <= +inf
-   0 <= flow(bus_storage2_1) <= +inf
-   0 <= flow(bus_storage2_2) <= +inf
-   0 <= flow(storage1_bus_0) <= +inf
-   0 <= flow(storage1_bus_1) <= +inf
-   0 <= flow(storage1_bus_2) <= +inf
-   0 <= flow(storage2_bus_0) <= +inf
-   0 <= flow(storage2_bus_1) <= +inf
-   0 <= flow(storage2_bus_2) <= +inf
-   0 <= limit_storage(0) <= 7
-   0 <= limit_storage(1) <= 7
-   0 <= limit_storage(2) <= 7
+   1 <= ONE_VAR_CONSTANT <= 1
    0 <= GenericStorageBlock_storage_content(storage1_0) <= 5
-   0 <= GenericStorageBlock_storage_content(storage1_1) <= 5
-   0 <= GenericStorageBlock_storage_content(storage1_2) <= 5
-   0 <= GenericStorageBlock_storage_content(storage1_3) <= 5
    0 <= GenericStorageBlock_storage_content(storage2_0) <= 5
+   0 <= limit_storage(0) <= 7
+   0 <= GenericStorageBlock_storage_content(storage1_1) <= 5
    0 <= GenericStorageBlock_storage_content(storage2_1) <= 5
+   0 <= limit_storage(1) <= 7
+   0 <= GenericStorageBlock_storage_content(storage1_2) <= 5
    0 <= GenericStorageBlock_storage_content(storage2_2) <= 5
+   0 <= limit_storage(2) <= 7
+   0 <= flow(storage1_bus_0_0) <= +inf
+   0 <= flow(storage2_bus_0_0) <= +inf
+   0 <= flow(bus_storage1_0_0) <= +inf
+   0 <= flow(bus_storage2_0_0) <= +inf
+   0 <= flow(storage1_bus_0_1) <= +inf
+   0 <= flow(storage2_bus_0_1) <= +inf
+   0 <= flow(bus_storage1_0_1) <= +inf
+   0 <= flow(bus_storage2_0_1) <= +inf
+   0 <= flow(storage1_bus_0_2) <= +inf
+   0 <= flow(storage2_bus_0_2) <= +inf
+   0 <= flow(bus_storage1_0_2) <= +inf
+   0 <= flow(bus_storage2_0_2) <= +inf
+   0 <= GenericStorageBlock_storage_content(storage1_3) <= 5
    0 <= GenericStorageBlock_storage_content(storage2_3) <= 5
 end
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/source_with_gradient.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/source_with_gradient.lp`

 * *Files 15% similar despite different names*

```diff
@@ -1,58 +1,65 @@
 \* Source Pyomo model name=Model *\
 
-min
+min 
 objective:
-+23 flow(powerplant_electricityBus_0)
-+23 flow(powerplant_electricityBus_1)
-+23 flow(powerplant_electricityBus_2)
++23 flow(powerplant_electricityBus_0_0)
++23 flow(powerplant_electricityBus_0_1)
++23 flow(powerplant_electricityBus_0_2)
 
 s.t.
 
-c_e_BusBlock_balance(electricityBus_0)_:
-+1 flow(powerplant_electricityBus_0)
+c_e_BusBlock_balance(electricityBus_0_0)_:
++1 flow(powerplant_electricityBus_0_0)
 = 0
 
-c_e_BusBlock_balance(electricityBus_1)_:
-+1 flow(powerplant_electricityBus_1)
+c_e_BusBlock_balance(electricityBus_0_1)_:
++1 flow(powerplant_electricityBus_0_1)
 = 0
 
-c_e_BusBlock_balance(electricityBus_2)_:
-+1 flow(powerplant_electricityBus_2)
+c_e_BusBlock_balance(electricityBus_0_2)_:
++1 flow(powerplant_electricityBus_0_2)
 = 0
 
-c_u_SimpleFlowBlock_positive_gradient_constr(powerplant_electricityBus_1)_:
+c_e_SimpleFlowBlock_positive_gradient_constr(powerplant_electricityBus_0_0)_:
++1 SimpleFlowBlock_positive_gradient(powerplant_electricityBus_0)
+= 0
+
+c_u_SimpleFlowBlock_positive_gradient_constr(powerplant_electricityBus_0_1)_:
+-1 flow(powerplant_electricityBus_0_0)
++1 flow(powerplant_electricityBus_0_1)
 -1 SimpleFlowBlock_positive_gradient(powerplant_electricityBus_1)
--1 flow(powerplant_electricityBus_0)
-+1 flow(powerplant_electricityBus_1)
 <= 0
 
-c_u_SimpleFlowBlock_positive_gradient_constr(powerplant_electricityBus_2)_:
+c_u_SimpleFlowBlock_positive_gradient_constr(powerplant_electricityBus_0_2)_:
+-1 flow(powerplant_electricityBus_0_1)
++1 flow(powerplant_electricityBus_0_2)
 -1 SimpleFlowBlock_positive_gradient(powerplant_electricityBus_2)
--1 flow(powerplant_electricityBus_1)
-+1 flow(powerplant_electricityBus_2)
 <= 0
 
-c_u_SimpleFlowBlock_negative_gradient_constr(powerplant_electricityBus_1)_:
+c_e_SimpleFlowBlock_negative_gradient_constr(powerplant_electricityBus_0_0)_:
++1 SimpleFlowBlock_negative_gradient(powerplant_electricityBus_0)
+= 0
+
+c_u_SimpleFlowBlock_negative_gradient_constr(powerplant_electricityBus_0_1)_:
++1 flow(powerplant_electricityBus_0_0)
+-1 flow(powerplant_electricityBus_0_1)
 -1 SimpleFlowBlock_negative_gradient(powerplant_electricityBus_1)
-+1 flow(powerplant_electricityBus_0)
--1 flow(powerplant_electricityBus_1)
 <= 0
 
-c_u_SimpleFlowBlock_negative_gradient_constr(powerplant_electricityBus_2)_:
+c_u_SimpleFlowBlock_negative_gradient_constr(powerplant_electricityBus_0_2)_:
++1 flow(powerplant_electricityBus_0_1)
+-1 flow(powerplant_electricityBus_0_2)
 -1 SimpleFlowBlock_negative_gradient(powerplant_electricityBus_2)
-+1 flow(powerplant_electricityBus_1)
--1 flow(powerplant_electricityBus_2)
 <= 0
 
-c_e_ONE_VAR_CONSTANT:
-ONE_VAR_CONSTANT = 1.0
-
 bounds
-   0 <= flow(powerplant_electricityBus_0) <= 999
-   0 <= flow(powerplant_electricityBus_1) <= 999
-   0 <= flow(powerplant_electricityBus_2) <= 999
-    -inf <= SimpleFlowBlock_positive_gradient(powerplant_electricityBus_1) <= 29.969999999999999
-    -inf <= SimpleFlowBlock_positive_gradient(powerplant_electricityBus_2) <= 29.969999999999999
-    -inf <= SimpleFlowBlock_negative_gradient(powerplant_electricityBus_1) <= 49.950000000000003
-    -inf <= SimpleFlowBlock_negative_gradient(powerplant_electricityBus_2) <= 49.950000000000003
+   0 <= flow(powerplant_electricityBus_0_0) <= 999
+   0 <= flow(powerplant_electricityBus_0_1) <= 999
+   0 <= flow(powerplant_electricityBus_0_2) <= 999
+   0 <= SimpleFlowBlock_positive_gradient(powerplant_electricityBus_0) <= 29.97
+   0 <= SimpleFlowBlock_positive_gradient(powerplant_electricityBus_1) <= 29.97
+   0 <= SimpleFlowBlock_positive_gradient(powerplant_electricityBus_2) <= 29.97
+   0 <= SimpleFlowBlock_negative_gradient(powerplant_electricityBus_0) <= 49.95
+   0 <= SimpleFlowBlock_negative_gradient(powerplant_electricityBus_1) <= 49.95
+   0 <= SimpleFlowBlock_negative_gradient(powerplant_electricityBus_2) <= 49.95
 end
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/source_with_nonconvex_gradient.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/source_with_nonconvex_gradient.lp`

 * *Files 5% similar despite different names*

```diff
@@ -1,118 +1,125 @@
 \* Source Pyomo model name=Model *\
 
-min
+min 
 objective:
-+23 flow(powerplant_electricityBus_0)
-+23 flow(powerplant_electricityBus_1)
-+23 flow(powerplant_electricityBus_2)
++23 flow(powerplant_electricityBus_0_0)
++23 flow(powerplant_electricityBus_0_1)
++23 flow(powerplant_electricityBus_0_2)
 
 s.t.
 
-c_e_BusBlock_balance(electricityBus_0)_:
-+1 flow(powerplant_electricityBus_0)
+c_e_BusBlock_balance(electricityBus_0_0)_:
++1 flow(powerplant_electricityBus_0_0)
 = 0
 
-c_e_BusBlock_balance(electricityBus_1)_:
-+1 flow(powerplant_electricityBus_1)
+c_e_BusBlock_balance(electricityBus_0_1)_:
++1 flow(powerplant_electricityBus_0_1)
 = 0
 
-c_e_BusBlock_balance(electricityBus_2)_:
-+1 flow(powerplant_electricityBus_2)
+c_e_BusBlock_balance(electricityBus_0_2)_:
++1 flow(powerplant_electricityBus_0_2)
 = 0
 
 c_e_NonConvexFlowBlock_status_nominal_constraint(powerplant_electricityBus_0)_:
--999 NonConvexFlowBlock_status(powerplant_electricityBus_0)
 +1 NonConvexFlowBlock_status_nominal(powerplant_electricityBus_0)
+-999 NonConvexFlowBlock_status(powerplant_electricityBus_0)
 = 0
 
 c_e_NonConvexFlowBlock_status_nominal_constraint(powerplant_electricityBus_1)_:
--999 NonConvexFlowBlock_status(powerplant_electricityBus_1)
 +1 NonConvexFlowBlock_status_nominal(powerplant_electricityBus_1)
+-999 NonConvexFlowBlock_status(powerplant_electricityBus_1)
 = 0
 
 c_e_NonConvexFlowBlock_status_nominal_constraint(powerplant_electricityBus_2)_:
--999 NonConvexFlowBlock_status(powerplant_electricityBus_2)
 +1 NonConvexFlowBlock_status_nominal(powerplant_electricityBus_2)
+-999 NonConvexFlowBlock_status(powerplant_electricityBus_2)
 = 0
 
-c_l_NonConvexFlowBlock_min(powerplant_electricityBus_0)_:
-+1 flow(powerplant_electricityBus_0)
->= 0
-
-c_l_NonConvexFlowBlock_min(powerplant_electricityBus_1)_:
-+1 flow(powerplant_electricityBus_1)
->= 0
-
-c_l_NonConvexFlowBlock_min(powerplant_electricityBus_2)_:
-+1 flow(powerplant_electricityBus_2)
->= 0
+c_u_NonConvexFlowBlock_min(powerplant_electricityBus_0_0)_:
+-1 flow(powerplant_electricityBus_0_0)
+<= 0
+
+c_u_NonConvexFlowBlock_min(powerplant_electricityBus_0_1)_:
+-1 flow(powerplant_electricityBus_0_1)
+<= 0
+
+c_u_NonConvexFlowBlock_min(powerplant_electricityBus_0_2)_:
+-1 flow(powerplant_electricityBus_0_2)
+<= 0
 
-c_u_NonConvexFlowBlock_max(powerplant_electricityBus_0)_:
+c_u_NonConvexFlowBlock_max(powerplant_electricityBus_0_0)_:
++1 flow(powerplant_electricityBus_0_0)
 -1 NonConvexFlowBlock_status_nominal(powerplant_electricityBus_0)
-+1 flow(powerplant_electricityBus_0)
 <= 0
 
-c_u_NonConvexFlowBlock_max(powerplant_electricityBus_1)_:
+c_u_NonConvexFlowBlock_max(powerplant_electricityBus_0_1)_:
++1 flow(powerplant_electricityBus_0_1)
 -1 NonConvexFlowBlock_status_nominal(powerplant_electricityBus_1)
-+1 flow(powerplant_electricityBus_1)
 <= 0
 
-c_u_NonConvexFlowBlock_max(powerplant_electricityBus_2)_:
+c_u_NonConvexFlowBlock_max(powerplant_electricityBus_0_2)_:
++1 flow(powerplant_electricityBus_0_2)
 -1 NonConvexFlowBlock_status_nominal(powerplant_electricityBus_2)
-+1 flow(powerplant_electricityBus_2)
 <= 0
 
-c_u_NonConvexFlowBlock_positive_gradient_constr(powerplant_electricityBus_1)_:
+c_e_NonConvexFlowBlock_positive_gradient_constr(powerplant_electricityBus_0_0)_:
++1 NonConvexFlowBlock_positive_gradient(powerplant_electricityBus_0)
+= 0
+
+c_u_NonConvexFlowBlock_positive_gradient_constr(powerplant_electricityBus_0_1)_:
 -1 NonConvexFlowBlock_positive_gradient(powerplant_electricityBus_1)
 + [
--1 NonConvexFlowBlock_status(powerplant_electricityBus_0) * flow(powerplant_electricityBus_0)
-+1 NonConvexFlowBlock_status(powerplant_electricityBus_1) * flow(powerplant_electricityBus_1)
+-1 flow(powerplant_electricityBus_0_0) * NonConvexFlowBlock_status(powerplant_electricityBus_0)
++1 flow(powerplant_electricityBus_0_1) * NonConvexFlowBlock_status(powerplant_electricityBus_1)
 ]
 <= 0
 
-c_u_NonConvexFlowBlock_positive_gradient_constr(powerplant_electricityBus_2)_:
+c_u_NonConvexFlowBlock_positive_gradient_constr(powerplant_electricityBus_0_2)_:
 -1 NonConvexFlowBlock_positive_gradient(powerplant_electricityBus_2)
 + [
--1 NonConvexFlowBlock_status(powerplant_electricityBus_1) * flow(powerplant_electricityBus_1)
-+1 NonConvexFlowBlock_status(powerplant_electricityBus_2) * flow(powerplant_electricityBus_2)
+-1 flow(powerplant_electricityBus_0_1) * NonConvexFlowBlock_status(powerplant_electricityBus_1)
++1 flow(powerplant_electricityBus_0_2) * NonConvexFlowBlock_status(powerplant_electricityBus_2)
 ]
 <= 0
 
-c_u_NonConvexFlowBlock_negative_gradient_constr(powerplant_electricityBus_1)_:
+c_e_NonConvexFlowBlock_negative_gradient_constr(powerplant_electricityBus_0_0)_:
++1 NonConvexFlowBlock_negative_gradient(powerplant_electricityBus_0)
+= 0
+
+c_u_NonConvexFlowBlock_negative_gradient_constr(powerplant_electricityBus_0_1)_:
 -1 NonConvexFlowBlock_negative_gradient(powerplant_electricityBus_1)
 + [
-+1 NonConvexFlowBlock_status(powerplant_electricityBus_0) * flow(powerplant_electricityBus_0)
--1 NonConvexFlowBlock_status(powerplant_electricityBus_1) * flow(powerplant_electricityBus_1)
++1 flow(powerplant_electricityBus_0_0) * NonConvexFlowBlock_status(powerplant_electricityBus_0)
+-1 flow(powerplant_electricityBus_0_1) * NonConvexFlowBlock_status(powerplant_electricityBus_1)
 ]
 <= 0
 
-c_u_NonConvexFlowBlock_negative_gradient_constr(powerplant_electricityBus_2)_:
+c_u_NonConvexFlowBlock_negative_gradient_constr(powerplant_electricityBus_0_2)_:
 -1 NonConvexFlowBlock_negative_gradient(powerplant_electricityBus_2)
 + [
-+1 NonConvexFlowBlock_status(powerplant_electricityBus_1) * flow(powerplant_electricityBus_1)
--1 NonConvexFlowBlock_status(powerplant_electricityBus_2) * flow(powerplant_electricityBus_2)
++1 flow(powerplant_electricityBus_0_1) * NonConvexFlowBlock_status(powerplant_electricityBus_1)
+-1 flow(powerplant_electricityBus_0_2) * NonConvexFlowBlock_status(powerplant_electricityBus_2)
 ]
 <= 0
 
-c_e_ONE_VAR_CONSTANT:
-ONE_VAR_CONSTANT = 1.0
-
 bounds
-   0 <= flow(powerplant_electricityBus_0) <= 999
-   0 <= flow(powerplant_electricityBus_1) <= 999
-   0 <= flow(powerplant_electricityBus_2) <= 999
-   0 <= NonConvexFlowBlock_status(powerplant_electricityBus_0) <= 1
-   0 <= NonConvexFlowBlock_status(powerplant_electricityBus_1) <= 1
-   0 <= NonConvexFlowBlock_status(powerplant_electricityBus_2) <= 1
+   0 <= flow(powerplant_electricityBus_0_0) <= 999
+   0 <= flow(powerplant_electricityBus_0_1) <= 999
+   0 <= flow(powerplant_electricityBus_0_2) <= 999
    0 <= NonConvexFlowBlock_status_nominal(powerplant_electricityBus_0) <= +inf
+   0 <= NonConvexFlowBlock_status(powerplant_electricityBus_0) <= 1
    0 <= NonConvexFlowBlock_status_nominal(powerplant_electricityBus_1) <= +inf
+   0 <= NonConvexFlowBlock_status(powerplant_electricityBus_1) <= 1
    0 <= NonConvexFlowBlock_status_nominal(powerplant_electricityBus_2) <= +inf
-    -inf <= NonConvexFlowBlock_positive_gradient(powerplant_electricityBus_1) <= +inf
-    -inf <= NonConvexFlowBlock_positive_gradient(powerplant_electricityBus_2) <= +inf
-    -inf <= NonConvexFlowBlock_negative_gradient(powerplant_electricityBus_1) <= +inf
-    -inf <= NonConvexFlowBlock_negative_gradient(powerplant_electricityBus_2) <= +inf
+   0 <= NonConvexFlowBlock_status(powerplant_electricityBus_2) <= 1
+   0 <= NonConvexFlowBlock_positive_gradient(powerplant_electricityBus_0) <= +inf
+   0 <= NonConvexFlowBlock_positive_gradient(powerplant_electricityBus_1) <= +inf
+   0 <= NonConvexFlowBlock_positive_gradient(powerplant_electricityBus_2) <= +inf
+   0 <= NonConvexFlowBlock_negative_gradient(powerplant_electricityBus_0) <= +inf
+   0 <= NonConvexFlowBlock_negative_gradient(powerplant_electricityBus_1) <= +inf
+   0 <= NonConvexFlowBlock_negative_gradient(powerplant_electricityBus_2) <= +inf
 binary
   NonConvexFlowBlock_status(powerplant_electricityBus_0)
   NonConvexFlowBlock_status(powerplant_electricityBus_1)
   NonConvexFlowBlock_status(powerplant_electricityBus_2)
 end
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/storage.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/storage_fixed_losses.lp`

 * *Files 16% similar despite different names*

```diff
@@ -1,66 +1,63 @@
 \* Source Pyomo model name=Model *\
 
-min
+min 
 objective:
-+56 flow(electricityBus_storage_no_invest_0)
-+56 flow(electricityBus_storage_no_invest_1)
-+56 flow(electricityBus_storage_no_invest_2)
-+24 flow(storage_no_invest_electricityBus_0)
-+24 flow(storage_no_invest_electricityBus_1)
-+24 flow(storage_no_invest_electricityBus_2)
++56 flow(electricityBus_storage_no_invest_0_0)
++56 flow(electricityBus_storage_no_invest_0_1)
++56 flow(electricityBus_storage_no_invest_0_2)
++24 flow(storage_no_invest_electricityBus_0_0)
++24 flow(storage_no_invest_electricityBus_0_1)
++24 flow(storage_no_invest_electricityBus_0_2)
 
 s.t.
 
-c_e_BusBlock_balance(electricityBus_0)_:
--1 flow(electricityBus_storage_no_invest_0)
-+1 flow(storage_no_invest_electricityBus_0)
+c_e_BusBlock_balance(electricityBus_0_0)_:
+-1 flow(electricityBus_storage_no_invest_0_0)
++1 flow(storage_no_invest_electricityBus_0_0)
 = 0
 
-c_e_BusBlock_balance(electricityBus_1)_:
--1 flow(electricityBus_storage_no_invest_1)
-+1 flow(storage_no_invest_electricityBus_1)
+c_e_BusBlock_balance(electricityBus_0_1)_:
+-1 flow(electricityBus_storage_no_invest_0_1)
++1 flow(storage_no_invest_electricityBus_0_1)
 = 0
 
-c_e_BusBlock_balance(electricityBus_2)_:
--1 flow(electricityBus_storage_no_invest_2)
-+1 flow(storage_no_invest_electricityBus_2)
+c_e_BusBlock_balance(electricityBus_0_2)_:
+-1 flow(electricityBus_storage_no_invest_0_2)
++1 flow(storage_no_invest_electricityBus_0_2)
 = 0
 
-c_e_GenericStorageBlock_balance(storage_no_invest_0)_:
+c_e_GenericStorageBlock_balance(storage_no_invest_0_0)_:
+-0.97 flow(electricityBus_storage_no_invest_0_0)
++1.1627906976744187 flow(storage_no_invest_electricityBus_0_0)
 +1 GenericStorageBlock_storage_content(storage_no_invest_1)
--0.96999999999999997 flow(electricityBus_storage_no_invest_0)
-+1.1627906976744187 flow(storage_no_invest_electricityBus_0)
-= 34800
+= 33797.0
 
-c_e_GenericStorageBlock_balance(storage_no_invest_1)_:
+c_e_GenericStorageBlock_balance(storage_no_invest_0_1)_:
+-0.97 flow(electricityBus_storage_no_invest_0_1)
++1.1627906976744187 flow(storage_no_invest_electricityBus_0_1)
 -0.87 GenericStorageBlock_storage_content(storage_no_invest_1)
 +1 GenericStorageBlock_storage_content(storage_no_invest_2)
--0.96999999999999997 flow(electricityBus_storage_no_invest_1)
-+1.1627906976744187 flow(storage_no_invest_electricityBus_1)
-= 0
+= -1003.0
 
-c_e_GenericStorageBlock_balance(storage_no_invest_2)_:
+c_e_GenericStorageBlock_balance(storage_no_invest_0_2)_:
+-0.97 flow(electricityBus_storage_no_invest_0_2)
++1.1627906976744187 flow(storage_no_invest_electricityBus_0_2)
 -0.87 GenericStorageBlock_storage_content(storage_no_invest_2)
 +1 GenericStorageBlock_storage_content(storage_no_invest_3)
--0.96999999999999997 flow(electricityBus_storage_no_invest_2)
-+1.1627906976744187 flow(storage_no_invest_electricityBus_2)
-= 0
+= -1003.0
 
 c_e_GenericStorageBlock_balanced_cstr(storage_no_invest)_:
 +1 GenericStorageBlock_storage_content(storage_no_invest_3)
-= 40000
-
-c_e_ONE_VAR_CONSTANT: 
-ONE_VAR_CONSTANT = 1.0
+= 40000.0
 
 bounds
-   0 <= flow(electricityBus_storage_no_invest_0) <= 16667
-   0 <= flow(electricityBus_storage_no_invest_1) <= 16667
-   0 <= flow(electricityBus_storage_no_invest_2) <= 16667
-   0 <= flow(storage_no_invest_electricityBus_0) <= 16667
-   0 <= flow(storage_no_invest_electricityBus_1) <= 16667
-   0 <= flow(storage_no_invest_electricityBus_2) <= 16667
-   0 <= GenericStorageBlock_storage_content(storage_no_invest_1) <= 100000
-   0 <= GenericStorageBlock_storage_content(storage_no_invest_2) <= 100000
-   0 <= GenericStorageBlock_storage_content(storage_no_invest_3) <= 100000
+   0 <= flow(electricityBus_storage_no_invest_0_0) <= 16667
+   0 <= flow(electricityBus_storage_no_invest_0_1) <= 16667
+   0 <= flow(electricityBus_storage_no_invest_0_2) <= 16667
+   0 <= flow(storage_no_invest_electricityBus_0_0) <= 16667
+   0 <= flow(storage_no_invest_electricityBus_0_1) <= 16667
+   0 <= flow(storage_no_invest_electricityBus_0_2) <= 16667
+   0.0 <= GenericStorageBlock_storage_content(storage_no_invest_1) <= 100000.0
+   0.0 <= GenericStorageBlock_storage_content(storage_no_invest_2) <= 100000.0
+   0.0 <= GenericStorageBlock_storage_content(storage_no_invest_3) <= 100000.0
 end
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/storage_fixed_losses.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/storage.lp`

 * *Files 24% similar despite different names*

```diff
@@ -1,66 +1,63 @@
 \* Source Pyomo model name=Model *\
 
 min 
 objective:
-+56 flow(electricityBus_storage_no_invest_0)
-+56 flow(electricityBus_storage_no_invest_1)
-+56 flow(electricityBus_storage_no_invest_2)
-+24 flow(storage_no_invest_electricityBus_0)
-+24 flow(storage_no_invest_electricityBus_1)
-+24 flow(storage_no_invest_electricityBus_2)
++56 flow(electricityBus_storage_no_invest_0_0)
++56 flow(electricityBus_storage_no_invest_0_1)
++56 flow(electricityBus_storage_no_invest_0_2)
++24 flow(storage_no_invest_electricityBus_0_0)
++24 flow(storage_no_invest_electricityBus_0_1)
++24 flow(storage_no_invest_electricityBus_0_2)
 
 s.t.
 
-c_e_BusBlock_balance(electricityBus_0)_:
--1 flow(electricityBus_storage_no_invest_0)
-+1 flow(storage_no_invest_electricityBus_0)
+c_e_BusBlock_balance(electricityBus_0_0)_:
+-1 flow(electricityBus_storage_no_invest_0_0)
++1 flow(storage_no_invest_electricityBus_0_0)
 = 0
 
-c_e_BusBlock_balance(electricityBus_1)_:
--1 flow(electricityBus_storage_no_invest_1)
-+1 flow(storage_no_invest_electricityBus_1)
+c_e_BusBlock_balance(electricityBus_0_1)_:
+-1 flow(electricityBus_storage_no_invest_0_1)
++1 flow(storage_no_invest_electricityBus_0_1)
 = 0
 
-c_e_BusBlock_balance(electricityBus_2)_:
--1 flow(electricityBus_storage_no_invest_2)
-+1 flow(storage_no_invest_electricityBus_2)
+c_e_BusBlock_balance(electricityBus_0_2)_:
+-1 flow(electricityBus_storage_no_invest_0_2)
++1 flow(storage_no_invest_electricityBus_0_2)
 = 0
 
-c_e_GenericStorageBlock_balance(storage_no_invest_0)_:
+c_e_GenericStorageBlock_balance(storage_no_invest_0_0)_:
+-0.97 flow(electricityBus_storage_no_invest_0_0)
++1.1627906976744187 flow(storage_no_invest_electricityBus_0_0)
 +1 GenericStorageBlock_storage_content(storage_no_invest_1)
--0.96999999999999997 flow(electricityBus_storage_no_invest_0)
-+1.1627906976744187 flow(storage_no_invest_electricityBus_0)
-= 33797
+= 34800.0
 
-c_e_GenericStorageBlock_balance(storage_no_invest_1)_:
+c_e_GenericStorageBlock_balance(storage_no_invest_0_1)_:
+-0.97 flow(electricityBus_storage_no_invest_0_1)
++1.1627906976744187 flow(storage_no_invest_electricityBus_0_1)
 -0.87 GenericStorageBlock_storage_content(storage_no_invest_1)
 +1 GenericStorageBlock_storage_content(storage_no_invest_2)
--0.96999999999999997 flow(electricityBus_storage_no_invest_1)
-+1.1627906976744187 flow(storage_no_invest_electricityBus_1)
-= -1003
+= 0
 
-c_e_GenericStorageBlock_balance(storage_no_invest_2)_:
+c_e_GenericStorageBlock_balance(storage_no_invest_0_2)_:
+-0.97 flow(electricityBus_storage_no_invest_0_2)
++1.1627906976744187 flow(storage_no_invest_electricityBus_0_2)
 -0.87 GenericStorageBlock_storage_content(storage_no_invest_2)
 +1 GenericStorageBlock_storage_content(storage_no_invest_3)
--0.96999999999999997 flow(electricityBus_storage_no_invest_2)
-+1.1627906976744187 flow(storage_no_invest_electricityBus_2)
-= -1003
+= 0
 
 c_e_GenericStorageBlock_balanced_cstr(storage_no_invest)_:
 +1 GenericStorageBlock_storage_content(storage_no_invest_3)
-= 40000
-
-c_e_ONE_VAR_CONSTANT: 
-ONE_VAR_CONSTANT = 1.0
+= 40000.0
 
 bounds
-   0 <= flow(electricityBus_storage_no_invest_0) <= 16667
-   0 <= flow(electricityBus_storage_no_invest_1) <= 16667
-   0 <= flow(electricityBus_storage_no_invest_2) <= 16667
-   0 <= flow(storage_no_invest_electricityBus_0) <= 16667
-   0 <= flow(storage_no_invest_electricityBus_1) <= 16667
-   0 <= flow(storage_no_invest_electricityBus_2) <= 16667
-   0 <= GenericStorageBlock_storage_content(storage_no_invest_1) <= 100000
-   0 <= GenericStorageBlock_storage_content(storage_no_invest_2) <= 100000
-   0 <= GenericStorageBlock_storage_content(storage_no_invest_3) <= 100000
+   0 <= flow(electricityBus_storage_no_invest_0_0) <= 16667
+   0 <= flow(electricityBus_storage_no_invest_0_1) <= 16667
+   0 <= flow(electricityBus_storage_no_invest_0_2) <= 16667
+   0 <= flow(storage_no_invest_electricityBus_0_0) <= 16667
+   0 <= flow(storage_no_invest_electricityBus_0_1) <= 16667
+   0 <= flow(storage_no_invest_electricityBus_0_2) <= 16667
+   0.0 <= GenericStorageBlock_storage_content(storage_no_invest_1) <= 100000.0
+   0.0 <= GenericStorageBlock_storage_content(storage_no_invest_2) <= 100000.0
+   0.0 <= GenericStorageBlock_storage_content(storage_no_invest_3) <= 100000.0
 end
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/storage_invest_1.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/storage_invest_1.lp`

 * *Files 13% similar despite different names*

```diff
@@ -1,148 +1,163 @@
 \* Source Pyomo model name=Model *\
 
-min
+min 
 objective:
-+145 GenericInvestmentStorageBlock_invest(storage1)
-+56 flow(electricityBus_storage1_0)
-+56 flow(electricityBus_storage1_1)
-+56 flow(electricityBus_storage1_2)
-+24 flow(storage1_electricityBus_0)
-+24 flow(storage1_electricityBus_1)
-+24 flow(storage1_electricityBus_2)
++56 flow(electricityBus_storage1_0_0)
++56 flow(electricityBus_storage1_0_1)
++56 flow(electricityBus_storage1_0_2)
++24 flow(storage1_electricityBus_0_0)
++24 flow(storage1_electricityBus_0_1)
++24 flow(storage1_electricityBus_0_2)
++145 GenericInvestmentStorageBlock_invest(storage1_0)
 
 s.t.
 
-c_e_BusBlock_balance(electricityBus_0)_:
--1 flow(electricityBus_storage1_0)
-+1 flow(storage1_electricityBus_0)
+c_e_BusBlock_balance(electricityBus_0_0)_:
+-1 flow(electricityBus_storage1_0_0)
++1 flow(storage1_electricityBus_0_0)
 = 0
 
-c_e_BusBlock_balance(electricityBus_1)_:
--1 flow(electricityBus_storage1_1)
-+1 flow(storage1_electricityBus_1)
+c_e_BusBlock_balance(electricityBus_0_1)_:
+-1 flow(electricityBus_storage1_0_1)
++1 flow(storage1_electricityBus_0_1)
 = 0
 
-c_e_BusBlock_balance(electricityBus_2)_:
--1 flow(electricityBus_storage1_2)
-+1 flow(storage1_electricityBus_2)
+c_e_BusBlock_balance(electricityBus_0_2)_:
+-1 flow(electricityBus_storage1_0_2)
++1 flow(storage1_electricityBus_0_2)
 = 0
 
-c_u_InvestmentFlowBlock_max(electricityBus_storage1_0)_:
--1 InvestmentFlowBlock_invest(electricityBus_storage1)
-+1 flow(electricityBus_storage1_0)
+c_e_InvestmentFlowBlock_total_rule(electricityBus_storage1_0)_:
++1 InvestmentFlowBlock_total(electricityBus_storage1_0)
+-1 InvestmentFlowBlock_invest(electricityBus_storage1_0)
+= 0
+
+c_e_InvestmentFlowBlock_total_rule(storage1_electricityBus_0)_:
++1 InvestmentFlowBlock_total(storage1_electricityBus_0)
+-1 InvestmentFlowBlock_invest(storage1_electricityBus_0)
+= 0
+
+c_u_InvestmentFlowBlock_max(electricityBus_storage1_0_0)_:
++1 flow(electricityBus_storage1_0_0)
+-1 InvestmentFlowBlock_total(electricityBus_storage1_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(electricityBus_storage1_1)_:
--1 InvestmentFlowBlock_invest(electricityBus_storage1)
-+1 flow(electricityBus_storage1_1)
+c_u_InvestmentFlowBlock_max(electricityBus_storage1_0_1)_:
++1 flow(electricityBus_storage1_0_1)
+-1 InvestmentFlowBlock_total(electricityBus_storage1_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(electricityBus_storage1_2)_:
--1 InvestmentFlowBlock_invest(electricityBus_storage1)
-+1 flow(electricityBus_storage1_2)
+c_u_InvestmentFlowBlock_max(electricityBus_storage1_0_2)_:
++1 flow(electricityBus_storage1_0_2)
+-1 InvestmentFlowBlock_total(electricityBus_storage1_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(storage1_electricityBus_0)_:
--1 InvestmentFlowBlock_invest(storage1_electricityBus)
-+1 flow(storage1_electricityBus_0)
+c_u_InvestmentFlowBlock_max(storage1_electricityBus_0_0)_:
++1 flow(storage1_electricityBus_0_0)
+-1 InvestmentFlowBlock_total(storage1_electricityBus_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(storage1_electricityBus_1)_:
--1 InvestmentFlowBlock_invest(storage1_electricityBus)
-+1 flow(storage1_electricityBus_1)
+c_u_InvestmentFlowBlock_max(storage1_electricityBus_0_1)_:
++1 flow(storage1_electricityBus_0_1)
+-1 InvestmentFlowBlock_total(storage1_electricityBus_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(storage1_electricityBus_2)_:
--1 InvestmentFlowBlock_invest(storage1_electricityBus)
-+1 flow(storage1_electricityBus_2)
+c_u_InvestmentFlowBlock_max(storage1_electricityBus_0_2)_:
++1 flow(storage1_electricityBus_0_2)
+-1 InvestmentFlowBlock_total(storage1_electricityBus_0)
 <= 0
 
+c_e_GenericInvestmentStorageBlock_total_storage_rule(storage1_0)_:
+-1 GenericInvestmentStorageBlock_invest(storage1_0)
++1 GenericInvestmentStorageBlock_total(storage1_0)
+= 0
+
 c_u_GenericInvestmentStorageBlock_init_content_limit(storage1)_:
+-1 GenericInvestmentStorageBlock_invest(storage1_0)
 +1 GenericInvestmentStorageBlock_init_content(storage1)
--1 GenericInvestmentStorageBlock_invest(storage1)
 <= 0
 
 c_e_GenericInvestmentStorageBlock_balance_first(storage1)_:
+-0.97 flow(electricityBus_storage1_0_0)
++1.1627906976744187 flow(storage1_electricityBus_0_0)
 -0.87 GenericInvestmentStorageBlock_init_content(storage1)
 +1 GenericInvestmentStorageBlock_storage_content(storage1_0)
--0.96999999999999997 flow(electricityBus_storage1_0)
-+1.1627906976744187 flow(storage1_electricityBus_0)
 = 0
 
-c_e_GenericInvestmentStorageBlock_balance(storage1_1)_:
+c_e_GenericInvestmentStorageBlock_balance(storage1_0_1)_:
+-0.97 flow(electricityBus_storage1_0_1)
++1.1627906976744187 flow(storage1_electricityBus_0_1)
 -0.87 GenericInvestmentStorageBlock_storage_content(storage1_0)
 +1 GenericInvestmentStorageBlock_storage_content(storage1_1)
--0.96999999999999997 flow(electricityBus_storage1_1)
-+1.1627906976744187 flow(storage1_electricityBus_1)
 = 0
 
-c_e_GenericInvestmentStorageBlock_balance(storage1_2)_:
+c_e_GenericInvestmentStorageBlock_balance(storage1_0_2)_:
+-0.97 flow(electricityBus_storage1_0_2)
++1.1627906976744187 flow(storage1_electricityBus_0_2)
 -0.87 GenericInvestmentStorageBlock_storage_content(storage1_1)
 +1 GenericInvestmentStorageBlock_storage_content(storage1_2)
--0.96999999999999997 flow(electricityBus_storage1_2)
-+1.1627906976744187 flow(storage1_electricityBus_2)
 = 0
 
 c_e_GenericInvestmentStorageBlock_balanced_cstr(storage1)_:
 -1 GenericInvestmentStorageBlock_init_content(storage1)
 +1 GenericInvestmentStorageBlock_storage_content(storage1_2)
 = 0
 
-c_e_GenericInvestmentStorageBlock_storage_capacity_inflow(storage1)_:
--0.16666666666666666 GenericInvestmentStorageBlock_invest(storage1)
-+1 InvestmentFlowBlock_invest(electricityBus_storage1)
+c_e_GenericInvestmentStorageBlock_storage_capacity_inflow(storage1_0)_:
++1 InvestmentFlowBlock_total(electricityBus_storage1_0)
+-0.16666666666666666 GenericInvestmentStorageBlock_total(storage1_0)
 = 0
 
-c_e_GenericInvestmentStorageBlock_storage_capacity_outflow(storage1)_:
--0.16666666666666666 GenericInvestmentStorageBlock_invest(storage1)
-+1 InvestmentFlowBlock_invest(storage1_electricityBus)
+c_e_GenericInvestmentStorageBlock_storage_capacity_outflow(storage1_0)_:
++1 InvestmentFlowBlock_total(storage1_electricityBus_0)
+-0.16666666666666666 GenericInvestmentStorageBlock_total(storage1_0)
 = 0
 
-c_u_GenericInvestmentStorageBlock_max_storage_content(storage1_0)_:
--0.90000000000000002 GenericInvestmentStorageBlock_invest(storage1)
+c_u_GenericInvestmentStorageBlock_max_storage_content(storage1_0_0)_:
+-0.9 GenericInvestmentStorageBlock_total(storage1_0)
 +1 GenericInvestmentStorageBlock_storage_content(storage1_0)
 <= 0
 
-c_u_GenericInvestmentStorageBlock_max_storage_content(storage1_1)_:
--0.90000000000000002 GenericInvestmentStorageBlock_invest(storage1)
+c_u_GenericInvestmentStorageBlock_max_storage_content(storage1_0_1)_:
+-0.9 GenericInvestmentStorageBlock_total(storage1_0)
 +1 GenericInvestmentStorageBlock_storage_content(storage1_1)
 <= 0
 
-c_u_GenericInvestmentStorageBlock_max_storage_content(storage1_2)_:
--0.90000000000000002 GenericInvestmentStorageBlock_invest(storage1)
+c_u_GenericInvestmentStorageBlock_max_storage_content(storage1_0_2)_:
+-0.9 GenericInvestmentStorageBlock_total(storage1_0)
 +1 GenericInvestmentStorageBlock_storage_content(storage1_2)
 <= 0
 
-c_u_GenericInvestmentStorageBlock_min_storage_content(storage1_0)_:
-+0.10000000000000001 GenericInvestmentStorageBlock_invest(storage1)
+c_u_GenericInvestmentStorageBlock_min_storage_content(storage1_0_0)_:
++0.1 GenericInvestmentStorageBlock_total(storage1_0)
 -1 GenericInvestmentStorageBlock_storage_content(storage1_0)
 <= 0
 
-c_u_GenericInvestmentStorageBlock_min_storage_content(storage1_1)_:
-+0.10000000000000001 GenericInvestmentStorageBlock_invest(storage1)
+c_u_GenericInvestmentStorageBlock_min_storage_content(storage1_0_1)_:
++0.1 GenericInvestmentStorageBlock_total(storage1_0)
 -1 GenericInvestmentStorageBlock_storage_content(storage1_1)
 <= 0
 
-c_u_GenericInvestmentStorageBlock_min_storage_content(storage1_2)_:
-+0.10000000000000001 GenericInvestmentStorageBlock_invest(storage1)
+c_u_GenericInvestmentStorageBlock_min_storage_content(storage1_0_2)_:
++0.1 GenericInvestmentStorageBlock_total(storage1_0)
 -1 GenericInvestmentStorageBlock_storage_content(storage1_2)
 <= 0
 
-c_e_ONE_VAR_CONSTANT:
-ONE_VAR_CONSTANT = 1.0
-
 bounds
-   0 <= flow(electricityBus_storage1_0) <= +inf
-   0 <= flow(electricityBus_storage1_1) <= +inf
-   0 <= flow(electricityBus_storage1_2) <= +inf
-   0 <= flow(storage1_electricityBus_0) <= +inf
-   0 <= flow(storage1_electricityBus_1) <= +inf
-   0 <= flow(storage1_electricityBus_2) <= +inf
-   0 <= InvestmentFlowBlock_invest(electricityBus_storage1) <= +inf
-   0 <= InvestmentFlowBlock_invest(storage1_electricityBus) <= +inf
+   0 <= flow(electricityBus_storage1_0_0) <= +inf
+   0 <= flow(electricityBus_storage1_0_1) <= +inf
+   0 <= flow(electricityBus_storage1_0_2) <= +inf
+   0 <= flow(storage1_electricityBus_0_0) <= +inf
+   0 <= flow(storage1_electricityBus_0_1) <= +inf
+   0 <= flow(storage1_electricityBus_0_2) <= +inf
+   0 <= GenericInvestmentStorageBlock_invest(storage1_0) <= 234
+   0 <= InvestmentFlowBlock_total(electricityBus_storage1_0) <= +inf
+   0 <= InvestmentFlowBlock_invest(electricityBus_storage1_0) <= +inf
+   0 <= InvestmentFlowBlock_total(storage1_electricityBus_0) <= +inf
+   0 <= InvestmentFlowBlock_invest(storage1_electricityBus_0) <= +inf
+   0 <= GenericInvestmentStorageBlock_total(storage1_0) <= +inf
+   0 <= GenericInvestmentStorageBlock_init_content(storage1) <= +inf
    0 <= GenericInvestmentStorageBlock_storage_content(storage1_0) <= +inf
    0 <= GenericInvestmentStorageBlock_storage_content(storage1_1) <= +inf
    0 <= GenericInvestmentStorageBlock_storage_content(storage1_2) <= +inf
-   0 <= GenericInvestmentStorageBlock_invest(storage1) <= 234
-   0 <= GenericInvestmentStorageBlock_init_content(storage1) <= +inf
 end
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/storage_invest_1_fixed_losses.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/storage_invest_2.lp`

 * *Files 12% similar despite different names*

```diff
@@ -1,151 +1,134 @@
 \* Source Pyomo model name=Model *\
 
-min
+min 
 objective:
-+145 GenericInvestmentStorageBlock_invest(storage1)
-+56 flow(electricityBus_storage1_0)
-+56 flow(electricityBus_storage1_1)
-+56 flow(electricityBus_storage1_2)
-+24 flow(storage1_electricityBus_0)
-+24 flow(storage1_electricityBus_1)
-+24 flow(storage1_electricityBus_2)
++99 InvestmentFlowBlock_invest(electricityBus_storage2_0)
++9 InvestmentFlowBlock_invest(storage2_electricityBus_0)
++145 GenericInvestmentStorageBlock_invest(storage2_0)
 
 s.t.
 
-c_e_BusBlock_balance(electricityBus_0)_:
--1 flow(electricityBus_storage1_0)
-+1 flow(storage1_electricityBus_0)
+c_e_BusBlock_balance(electricityBus_0_0)_:
++1 flow(storage2_electricityBus_0_0)
+-1 flow(electricityBus_storage2_0_0)
 = 0
 
-c_e_BusBlock_balance(electricityBus_1)_:
--1 flow(electricityBus_storage1_1)
-+1 flow(storage1_electricityBus_1)
+c_e_BusBlock_balance(electricityBus_0_1)_:
++1 flow(storage2_electricityBus_0_1)
+-1 flow(electricityBus_storage2_0_1)
 = 0
 
-c_e_BusBlock_balance(electricityBus_2)_:
--1 flow(electricityBus_storage1_2)
-+1 flow(storage1_electricityBus_2)
+c_e_BusBlock_balance(electricityBus_0_2)_:
++1 flow(storage2_electricityBus_0_2)
+-1 flow(electricityBus_storage2_0_2)
 = 0
 
-c_u_InvestmentFlowBlock_max(electricityBus_storage1_0)_:
--1 InvestmentFlowBlock_invest(electricityBus_storage1)
-+1 flow(electricityBus_storage1_0)
-<= 0
+c_e_InvestmentFlowBlock_total_rule(electricityBus_storage2_0)_:
+-1 InvestmentFlowBlock_invest(electricityBus_storage2_0)
++1 InvestmentFlowBlock_total(electricityBus_storage2_0)
+= 0
 
-c_u_InvestmentFlowBlock_max(electricityBus_storage1_1)_:
--1 InvestmentFlowBlock_invest(electricityBus_storage1)
-+1 flow(electricityBus_storage1_1)
-<= 0
+c_e_InvestmentFlowBlock_total_rule(storage2_electricityBus_0)_:
+-1 InvestmentFlowBlock_invest(storage2_electricityBus_0)
++1 InvestmentFlowBlock_total(storage2_electricityBus_0)
+= 0
 
-c_u_InvestmentFlowBlock_max(electricityBus_storage1_2)_:
--1 InvestmentFlowBlock_invest(electricityBus_storage1)
-+1 flow(electricityBus_storage1_2)
+c_u_InvestmentFlowBlock_max(electricityBus_storage2_0_0)_:
++1 flow(electricityBus_storage2_0_0)
+-1 InvestmentFlowBlock_total(electricityBus_storage2_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(storage1_electricityBus_0)_:
--1 InvestmentFlowBlock_invest(storage1_electricityBus)
-+1 flow(storage1_electricityBus_0)
+c_u_InvestmentFlowBlock_max(electricityBus_storage2_0_1)_:
++1 flow(electricityBus_storage2_0_1)
+-1 InvestmentFlowBlock_total(electricityBus_storage2_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(storage1_electricityBus_1)_:
--1 InvestmentFlowBlock_invest(storage1_electricityBus)
-+1 flow(storage1_electricityBus_1)
+c_u_InvestmentFlowBlock_max(electricityBus_storage2_0_2)_:
++1 flow(electricityBus_storage2_0_2)
+-1 InvestmentFlowBlock_total(electricityBus_storage2_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(storage1_electricityBus_2)_:
--1 InvestmentFlowBlock_invest(storage1_electricityBus)
-+1 flow(storage1_electricityBus_2)
+c_u_InvestmentFlowBlock_max(storage2_electricityBus_0_0)_:
++1 flow(storage2_electricityBus_0_0)
+-1 InvestmentFlowBlock_total(storage2_electricityBus_0)
 <= 0
 
-c_u_GenericInvestmentStorageBlock_init_content_limit(storage1)_:
-+1 GenericInvestmentStorageBlock_init_content(storage1)
--1 GenericInvestmentStorageBlock_invest(storage1)
+c_u_InvestmentFlowBlock_max(storage2_electricityBus_0_1)_:
++1 flow(storage2_electricityBus_0_1)
+-1 InvestmentFlowBlock_total(storage2_electricityBus_0)
 <= 0
 
-c_e_GenericInvestmentStorageBlock_balance_first(storage1)_:
--0.87 GenericInvestmentStorageBlock_init_content(storage1)
-+0.01 GenericInvestmentStorageBlock_invest(storage1)
-+1 GenericInvestmentStorageBlock_storage_content(storage1_0)
--0.96999999999999997 flow(electricityBus_storage1_0)
-+1.1627906976744187 flow(storage1_electricityBus_0)
-= -3
-
-c_e_GenericInvestmentStorageBlock_balance(storage1_1)_:
-+0.01 GenericInvestmentStorageBlock_invest(storage1)
--0.87 GenericInvestmentStorageBlock_storage_content(storage1_0)
-+1 GenericInvestmentStorageBlock_storage_content(storage1_1)
--0.96999999999999997 flow(electricityBus_storage1_1)
-+1.1627906976744187 flow(storage1_electricityBus_1)
-= -3
-
-c_e_GenericInvestmentStorageBlock_balance(storage1_2)_:
-+0.01 GenericInvestmentStorageBlock_invest(storage1)
--0.87 GenericInvestmentStorageBlock_storage_content(storage1_1)
-+1 GenericInvestmentStorageBlock_storage_content(storage1_2)
--0.96999999999999997 flow(electricityBus_storage1_2)
-+1.1627906976744187 flow(storage1_electricityBus_2)
-= -3
+c_u_InvestmentFlowBlock_max(storage2_electricityBus_0_2)_:
++1 flow(storage2_electricityBus_0_2)
+-1 InvestmentFlowBlock_total(storage2_electricityBus_0)
+<= 0
 
-c_e_GenericInvestmentStorageBlock_balanced_cstr(storage1)_:
--1 GenericInvestmentStorageBlock_init_content(storage1)
-+1 GenericInvestmentStorageBlock_storage_content(storage1_2)
+c_e_GenericInvestmentStorageBlock_total_storage_rule(storage2_0)_:
+-1 GenericInvestmentStorageBlock_invest(storage2_0)
++1 GenericInvestmentStorageBlock_total(storage2_0)
 = 0
 
-c_e_GenericInvestmentStorageBlock_storage_capacity_inflow(storage1)_:
--0.16666666666666666 GenericInvestmentStorageBlock_invest(storage1)
-+1 InvestmentFlowBlock_invest(electricityBus_storage1)
+c_e_GenericInvestmentStorageBlock_init_content_fix(storage2)_:
+-0.5 GenericInvestmentStorageBlock_invest(storage2_0)
++1 GenericInvestmentStorageBlock_init_content(storage2)
 = 0
 
-c_e_GenericInvestmentStorageBlock_storage_capacity_outflow(storage1)_:
--0.16666666666666666 GenericInvestmentStorageBlock_invest(storage1)
-+1 InvestmentFlowBlock_invest(storage1_electricityBus)
+c_e_GenericInvestmentStorageBlock_balance_first(storage2)_:
++1 flow(storage2_electricityBus_0_0)
+-1 flow(electricityBus_storage2_0_0)
+-1 GenericInvestmentStorageBlock_init_content(storage2)
++1 GenericInvestmentStorageBlock_storage_content(storage2_0)
 = 0
 
-c_u_GenericInvestmentStorageBlock_max_storage_content(storage1_0)_:
--0.90000000000000002 GenericInvestmentStorageBlock_invest(storage1)
-+1 GenericInvestmentStorageBlock_storage_content(storage1_0)
-<= 0
+c_e_GenericInvestmentStorageBlock_balance(storage2_0_1)_:
++1 flow(storage2_electricityBus_0_1)
+-1 flow(electricityBus_storage2_0_1)
+-1 GenericInvestmentStorageBlock_storage_content(storage2_0)
++1 GenericInvestmentStorageBlock_storage_content(storage2_1)
+= 0
 
-c_u_GenericInvestmentStorageBlock_max_storage_content(storage1_1)_:
--0.90000000000000002 GenericInvestmentStorageBlock_invest(storage1)
-+1 GenericInvestmentStorageBlock_storage_content(storage1_1)
-<= 0
+c_e_GenericInvestmentStorageBlock_balance(storage2_0_2)_:
++1 flow(storage2_electricityBus_0_2)
+-1 flow(electricityBus_storage2_0_2)
+-1 GenericInvestmentStorageBlock_storage_content(storage2_1)
++1 GenericInvestmentStorageBlock_storage_content(storage2_2)
+= 0
 
-c_u_GenericInvestmentStorageBlock_max_storage_content(storage1_2)_:
--0.90000000000000002 GenericInvestmentStorageBlock_invest(storage1)
-+1 GenericInvestmentStorageBlock_storage_content(storage1_2)
-<= 0
+c_e_GenericInvestmentStorageBlock_balanced_cstr(storage2)_:
+-1 GenericInvestmentStorageBlock_init_content(storage2)
++1 GenericInvestmentStorageBlock_storage_content(storage2_2)
+= 0
 
-c_u_GenericInvestmentStorageBlock_min_storage_content(storage1_0)_:
-+0.10000000000000001 GenericInvestmentStorageBlock_invest(storage1)
--1 GenericInvestmentStorageBlock_storage_content(storage1_0)
+c_u_GenericInvestmentStorageBlock_max_storage_content(storage2_0_0)_:
+-1 GenericInvestmentStorageBlock_total(storage2_0)
++1 GenericInvestmentStorageBlock_storage_content(storage2_0)
 <= 0
 
-c_u_GenericInvestmentStorageBlock_min_storage_content(storage1_1)_:
-+0.10000000000000001 GenericInvestmentStorageBlock_invest(storage1)
--1 GenericInvestmentStorageBlock_storage_content(storage1_1)
+c_u_GenericInvestmentStorageBlock_max_storage_content(storage2_0_1)_:
+-1 GenericInvestmentStorageBlock_total(storage2_0)
++1 GenericInvestmentStorageBlock_storage_content(storage2_1)
 <= 0
 
-c_u_GenericInvestmentStorageBlock_min_storage_content(storage1_2)_:
-+0.10000000000000001 GenericInvestmentStorageBlock_invest(storage1)
--1 GenericInvestmentStorageBlock_storage_content(storage1_2)
+c_u_GenericInvestmentStorageBlock_max_storage_content(storage2_0_2)_:
+-1 GenericInvestmentStorageBlock_total(storage2_0)
++1 GenericInvestmentStorageBlock_storage_content(storage2_2)
 <= 0
 
-c_e_ONE_VAR_CONSTANT:
-ONE_VAR_CONSTANT = 1.0
-
 bounds
-   0 <= flow(electricityBus_storage1_0) <= +inf
-   0 <= flow(electricityBus_storage1_1) <= +inf
-   0 <= flow(electricityBus_storage1_2) <= +inf
-   0 <= flow(storage1_electricityBus_0) <= +inf
-   0 <= flow(storage1_electricityBus_1) <= +inf
-   0 <= flow(storage1_electricityBus_2) <= +inf
-   0 <= InvestmentFlowBlock_invest(electricityBus_storage1) <= +inf
-   0 <= InvestmentFlowBlock_invest(storage1_electricityBus) <= +inf
-   0 <= GenericInvestmentStorageBlock_storage_content(storage1_0) <= +inf
-   0 <= GenericInvestmentStorageBlock_storage_content(storage1_1) <= +inf
-   0 <= GenericInvestmentStorageBlock_storage_content(storage1_2) <= +inf
-   0 <= GenericInvestmentStorageBlock_invest(storage1) <= 234
-   0 <= GenericInvestmentStorageBlock_init_content(storage1) <= +inf
+   0 <= InvestmentFlowBlock_invest(electricityBus_storage2_0) <= +inf
+   0 <= InvestmentFlowBlock_invest(storage2_electricityBus_0) <= +inf
+   0 <= GenericInvestmentStorageBlock_invest(storage2_0) <= +inf
+   0 <= flow(storage2_electricityBus_0_0) <= +inf
+   0 <= flow(electricityBus_storage2_0_0) <= +inf
+   0 <= flow(storage2_electricityBus_0_1) <= +inf
+   0 <= flow(electricityBus_storage2_0_1) <= +inf
+   0 <= flow(storage2_electricityBus_0_2) <= +inf
+   0 <= flow(electricityBus_storage2_0_2) <= +inf
+   0 <= InvestmentFlowBlock_total(electricityBus_storage2_0) <= +inf
+   0 <= InvestmentFlowBlock_total(storage2_electricityBus_0) <= +inf
+   0 <= GenericInvestmentStorageBlock_total(storage2_0) <= +inf
+   0 <= GenericInvestmentStorageBlock_init_content(storage2) <= +inf
+   0 <= GenericInvestmentStorageBlock_storage_content(storage2_0) <= +inf
+   0 <= GenericInvestmentStorageBlock_storage_content(storage2_1) <= +inf
+   0 <= GenericInvestmentStorageBlock_storage_content(storage2_2) <= +inf
 end
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/storage_invest_2.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/storage_invest_6.lp`

 * *Files 22% similar despite different names*

```diff
@@ -1,119 +1,138 @@
 \* Source Pyomo model name=Model *\
 
-min
+min 
 objective:
-+145 GenericInvestmentStorageBlock_invest(storage2)
-+99 InvestmentFlowBlock_invest(electricityBus_storage2)
-+9 InvestmentFlowBlock_invest(storage2_electricityBus)
++99 InvestmentFlowBlock_invest(electricityBus_storage6_0)
++145 GenericInvestmentStorageBlock_invest(storage6_0)
 
 s.t.
 
-c_e_BusBlock_balance(electricityBus_0)_:
--1 flow(electricityBus_storage2_0)
-+1 flow(storage2_electricityBus_0)
+c_e_BusBlock_balance(electricityBus_0_0)_:
++1 flow(storage6_electricityBus_0_0)
+-1 flow(electricityBus_storage6_0_0)
 = 0
 
-c_e_BusBlock_balance(electricityBus_1)_:
--1 flow(electricityBus_storage2_1)
-+1 flow(storage2_electricityBus_1)
+c_e_BusBlock_balance(electricityBus_0_1)_:
++1 flow(storage6_electricityBus_0_1)
+-1 flow(electricityBus_storage6_0_1)
 = 0
 
-c_e_BusBlock_balance(electricityBus_2)_:
--1 flow(electricityBus_storage2_2)
-+1 flow(storage2_electricityBus_2)
+c_e_BusBlock_balance(electricityBus_0_2)_:
++1 flow(storage6_electricityBus_0_2)
+-1 flow(electricityBus_storage6_0_2)
 = 0
 
-c_u_InvestmentFlowBlock_max(electricityBus_storage2_0)_:
--1 InvestmentFlowBlock_invest(electricityBus_storage2)
-+1 flow(electricityBus_storage2_0)
+c_e_InvestmentFlowBlock_total_rule(storage6_electricityBus_0)_:
++1 InvestmentFlowBlock_total(storage6_electricityBus_0)
+-1 InvestmentFlowBlock_invest(storage6_electricityBus_0)
+= 100
+
+c_e_InvestmentFlowBlock_total_rule(electricityBus_storage6_0)_:
+-1 InvestmentFlowBlock_invest(electricityBus_storage6_0)
++1 InvestmentFlowBlock_total(electricityBus_storage6_0)
+= 110
+
+c_u_InvestmentFlowBlock_max(storage6_electricityBus_0_0)_:
++1 flow(storage6_electricityBus_0_0)
+-1 InvestmentFlowBlock_total(storage6_electricityBus_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(electricityBus_storage2_1)_:
--1 InvestmentFlowBlock_invest(electricityBus_storage2)
-+1 flow(electricityBus_storage2_1)
+c_u_InvestmentFlowBlock_max(storage6_electricityBus_0_1)_:
++1 flow(storage6_electricityBus_0_1)
+-1 InvestmentFlowBlock_total(storage6_electricityBus_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(electricityBus_storage2_2)_:
--1 InvestmentFlowBlock_invest(electricityBus_storage2)
-+1 flow(electricityBus_storage2_2)
+c_u_InvestmentFlowBlock_max(storage6_electricityBus_0_2)_:
++1 flow(storage6_electricityBus_0_2)
+-1 InvestmentFlowBlock_total(storage6_electricityBus_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(storage2_electricityBus_0)_:
--1 InvestmentFlowBlock_invest(storage2_electricityBus)
-+1 flow(storage2_electricityBus_0)
+c_u_InvestmentFlowBlock_max(electricityBus_storage6_0_0)_:
++1 flow(electricityBus_storage6_0_0)
+-1 InvestmentFlowBlock_total(electricityBus_storage6_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(storage2_electricityBus_1)_:
--1 InvestmentFlowBlock_invest(storage2_electricityBus)
-+1 flow(storage2_electricityBus_1)
+c_u_InvestmentFlowBlock_max(electricityBus_storage6_0_1)_:
++1 flow(electricityBus_storage6_0_1)
+-1 InvestmentFlowBlock_total(electricityBus_storage6_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(storage2_electricityBus_2)_:
--1 InvestmentFlowBlock_invest(storage2_electricityBus)
-+1 flow(storage2_electricityBus_2)
+c_u_InvestmentFlowBlock_max(electricityBus_storage6_0_2)_:
++1 flow(electricityBus_storage6_0_2)
+-1 InvestmentFlowBlock_total(electricityBus_storage6_0)
 <= 0
 
-c_e_GenericInvestmentStorageBlock_init_content_fix(storage2)_:
-+1 GenericInvestmentStorageBlock_init_content(storage2)
--0.5 GenericInvestmentStorageBlock_invest(storage2)
+c_e_GenericInvestmentStorageBlock_total_storage_rule(storage6_0)_:
+-1 GenericInvestmentStorageBlock_invest(storage6_0)
++1 GenericInvestmentStorageBlock_total(storage6_0)
+= 10000
+
+c_u_GenericInvestmentStorageBlock_init_content_limit(storage6)_:
+-1 GenericInvestmentStorageBlock_invest(storage6_0)
++1 GenericInvestmentStorageBlock_init_content(storage6)
+<= 10000
+
+c_e_GenericInvestmentStorageBlock_balance_first(storage6)_:
++1 flow(storage6_electricityBus_0_0)
+-1 flow(electricityBus_storage6_0_0)
+-1 GenericInvestmentStorageBlock_init_content(storage6)
++1 GenericInvestmentStorageBlock_storage_content(storage6_0)
 = 0
 
-c_e_GenericInvestmentStorageBlock_balance_first(storage2)_:
--1 GenericInvestmentStorageBlock_init_content(storage2)
-+1 GenericInvestmentStorageBlock_storage_content(storage2_0)
--1 flow(electricityBus_storage2_0)
-+1 flow(storage2_electricityBus_0)
+c_e_GenericInvestmentStorageBlock_balance(storage6_0_1)_:
++1 flow(storage6_electricityBus_0_1)
+-1 flow(electricityBus_storage6_0_1)
+-1 GenericInvestmentStorageBlock_storage_content(storage6_0)
++1 GenericInvestmentStorageBlock_storage_content(storage6_1)
 = 0
 
-c_e_GenericInvestmentStorageBlock_balance(storage2_1)_:
--1 GenericInvestmentStorageBlock_storage_content(storage2_0)
-+1 GenericInvestmentStorageBlock_storage_content(storage2_1)
--1 flow(electricityBus_storage2_1)
-+1 flow(storage2_electricityBus_1)
+c_e_GenericInvestmentStorageBlock_balance(storage6_0_2)_:
++1 flow(storage6_electricityBus_0_2)
+-1 flow(electricityBus_storage6_0_2)
+-1 GenericInvestmentStorageBlock_storage_content(storage6_1)
++1 GenericInvestmentStorageBlock_storage_content(storage6_2)
 = 0
 
-c_e_GenericInvestmentStorageBlock_balance(storage2_2)_:
--1 GenericInvestmentStorageBlock_storage_content(storage2_1)
-+1 GenericInvestmentStorageBlock_storage_content(storage2_2)
--1 flow(electricityBus_storage2_2)
-+1 flow(storage2_electricityBus_2)
+c_e_GenericInvestmentStorageBlock_balanced_cstr(storage6)_:
+-1 GenericInvestmentStorageBlock_init_content(storage6)
++1 GenericInvestmentStorageBlock_storage_content(storage6_2)
 = 0
 
-c_e_GenericInvestmentStorageBlock_balanced_cstr(storage2)_:
--1 GenericInvestmentStorageBlock_init_content(storage2)
-+1 GenericInvestmentStorageBlock_storage_content(storage2_2)
+c_e_GenericInvestmentStorageBlock_power_coupled(storage6_0)_:
++1.1 InvestmentFlowBlock_total(storage6_electricityBus_0)
+-1 InvestmentFlowBlock_total(electricityBus_storage6_0)
 = 0
 
-c_u_GenericInvestmentStorageBlock_max_storage_content(storage2_0)_:
--1 GenericInvestmentStorageBlock_invest(storage2)
-+1 GenericInvestmentStorageBlock_storage_content(storage2_0)
+c_u_GenericInvestmentStorageBlock_max_storage_content(storage6_0_0)_:
+-1 GenericInvestmentStorageBlock_total(storage6_0)
++1 GenericInvestmentStorageBlock_storage_content(storage6_0)
 <= 0
 
-c_u_GenericInvestmentStorageBlock_max_storage_content(storage2_1)_:
--1 GenericInvestmentStorageBlock_invest(storage2)
-+1 GenericInvestmentStorageBlock_storage_content(storage2_1)
+c_u_GenericInvestmentStorageBlock_max_storage_content(storage6_0_1)_:
+-1 GenericInvestmentStorageBlock_total(storage6_0)
++1 GenericInvestmentStorageBlock_storage_content(storage6_1)
 <= 0
 
-c_u_GenericInvestmentStorageBlock_max_storage_content(storage2_2)_:
--1 GenericInvestmentStorageBlock_invest(storage2)
-+1 GenericInvestmentStorageBlock_storage_content(storage2_2)
+c_u_GenericInvestmentStorageBlock_max_storage_content(storage6_0_2)_:
+-1 GenericInvestmentStorageBlock_total(storage6_0)
++1 GenericInvestmentStorageBlock_storage_content(storage6_2)
 <= 0
 
-c_e_ONE_VAR_CONSTANT:
-ONE_VAR_CONSTANT = 1.0
-
 bounds
-   0 <= flow(electricityBus_storage2_0) <= +inf
-   0 <= flow(electricityBus_storage2_1) <= +inf
-   0 <= flow(electricityBus_storage2_2) <= +inf
-   0 <= flow(storage2_electricityBus_0) <= +inf
-   0 <= flow(storage2_electricityBus_1) <= +inf
-   0 <= flow(storage2_electricityBus_2) <= +inf
-   0 <= InvestmentFlowBlock_invest(electricityBus_storage2) <= +inf
-   0 <= InvestmentFlowBlock_invest(storage2_electricityBus) <= +inf
-   0 <= GenericInvestmentStorageBlock_storage_content(storage2_0) <= +inf
-   0 <= GenericInvestmentStorageBlock_storage_content(storage2_1) <= +inf
-   0 <= GenericInvestmentStorageBlock_storage_content(storage2_2) <= +inf
-   0 <= GenericInvestmentStorageBlock_invest(storage2) <= +inf
-   0 <= GenericInvestmentStorageBlock_init_content(storage2) <= +inf
+   0 <= InvestmentFlowBlock_invest(electricityBus_storage6_0) <= +inf
+   0 <= GenericInvestmentStorageBlock_invest(storage6_0) <= +inf
+   0 <= flow(storage6_electricityBus_0_0) <= +inf
+   0 <= flow(electricityBus_storage6_0_0) <= +inf
+   0 <= flow(storage6_electricityBus_0_1) <= +inf
+   0 <= flow(electricityBus_storage6_0_1) <= +inf
+   0 <= flow(storage6_electricityBus_0_2) <= +inf
+   0 <= flow(electricityBus_storage6_0_2) <= +inf
+   0 <= InvestmentFlowBlock_total(storage6_electricityBus_0) <= +inf
+   0 <= InvestmentFlowBlock_invest(storage6_electricityBus_0) <= +inf
+   0 <= InvestmentFlowBlock_total(electricityBus_storage6_0) <= +inf
+   0 <= GenericInvestmentStorageBlock_total(storage6_0) <= +inf
+   0 <= GenericInvestmentStorageBlock_init_content(storage6) <= +inf
+   0 <= GenericInvestmentStorageBlock_storage_content(storage6_0) <= +inf
+   0 <= GenericInvestmentStorageBlock_storage_content(storage6_1) <= +inf
+   0 <= GenericInvestmentStorageBlock_storage_content(storage6_2) <= +inf
 end
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/storage_invest_3.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/storage_invest_3.lp`

 * *Files 20% similar despite different names*

```diff
@@ -1,97 +1,106 @@
 \* Source Pyomo model name=Model *\
 
 min 
 objective:
-+99 InvestmentFlowBlock_invest(electricityBus_storage3)
-+9 InvestmentFlowBlock_invest(storage3_electricityBus)
++9 InvestmentFlowBlock_invest(storage3_electricityBus_0)
++99 InvestmentFlowBlock_invest(electricityBus_storage3_0)
 
 s.t.
 
-c_e_BusBlock_balance(electricityBus_0)_:
--1 flow(electricityBus_storage3_0)
-+1 flow(storage3_electricityBus_0)
+c_e_BusBlock_balance(electricityBus_0_0)_:
++1 flow(storage3_electricityBus_0_0)
+-1 flow(electricityBus_storage3_0_0)
 = 0
 
-c_e_BusBlock_balance(electricityBus_1)_:
--1 flow(electricityBus_storage3_1)
-+1 flow(storage3_electricityBus_1)
+c_e_BusBlock_balance(electricityBus_0_1)_:
++1 flow(storage3_electricityBus_0_1)
+-1 flow(electricityBus_storage3_0_1)
 = 0
 
-c_e_BusBlock_balance(electricityBus_2)_:
--1 flow(electricityBus_storage3_2)
-+1 flow(storage3_electricityBus_2)
+c_e_BusBlock_balance(electricityBus_0_2)_:
++1 flow(storage3_electricityBus_0_2)
+-1 flow(electricityBus_storage3_0_2)
 = 0
 
-c_u_InvestmentFlowBlock_max(electricityBus_storage3_0)_:
--1 InvestmentFlowBlock_invest(electricityBus_storage3)
-+1 flow(electricityBus_storage3_0)
+c_e_InvestmentFlowBlock_total_rule(storage3_electricityBus_0)_:
+-1 InvestmentFlowBlock_invest(storage3_electricityBus_0)
++1 InvestmentFlowBlock_total(storage3_electricityBus_0)
+= 0
+
+c_e_InvestmentFlowBlock_total_rule(electricityBus_storage3_0)_:
+-1 InvestmentFlowBlock_invest(electricityBus_storage3_0)
++1 InvestmentFlowBlock_total(electricityBus_storage3_0)
+= 0
+
+c_u_InvestmentFlowBlock_max(storage3_electricityBus_0_0)_:
++1 flow(storage3_electricityBus_0_0)
+-1 InvestmentFlowBlock_total(storage3_electricityBus_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(electricityBus_storage3_1)_:
--1 InvestmentFlowBlock_invest(electricityBus_storage3)
-+1 flow(electricityBus_storage3_1)
+c_u_InvestmentFlowBlock_max(storage3_electricityBus_0_1)_:
++1 flow(storage3_electricityBus_0_1)
+-1 InvestmentFlowBlock_total(storage3_electricityBus_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(electricityBus_storage3_2)_:
--1 InvestmentFlowBlock_invest(electricityBus_storage3)
-+1 flow(electricityBus_storage3_2)
+c_u_InvestmentFlowBlock_max(storage3_electricityBus_0_2)_:
++1 flow(storage3_electricityBus_0_2)
+-1 InvestmentFlowBlock_total(storage3_electricityBus_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(storage3_electricityBus_0)_:
--1 InvestmentFlowBlock_invest(storage3_electricityBus)
-+1 flow(storage3_electricityBus_0)
+c_u_InvestmentFlowBlock_max(electricityBus_storage3_0_0)_:
++1 flow(electricityBus_storage3_0_0)
+-1 InvestmentFlowBlock_total(electricityBus_storage3_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(storage3_electricityBus_1)_:
--1 InvestmentFlowBlock_invest(storage3_electricityBus)
-+1 flow(storage3_electricityBus_1)
+c_u_InvestmentFlowBlock_max(electricityBus_storage3_0_1)_:
++1 flow(electricityBus_storage3_0_1)
+-1 InvestmentFlowBlock_total(electricityBus_storage3_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(storage3_electricityBus_2)_:
--1 InvestmentFlowBlock_invest(storage3_electricityBus)
-+1 flow(storage3_electricityBus_2)
+c_u_InvestmentFlowBlock_max(electricityBus_storage3_0_2)_:
++1 flow(electricityBus_storage3_0_2)
+-1 InvestmentFlowBlock_total(electricityBus_storage3_0)
 <= 0
 
-c_e_GenericStorageBlock_balance(storage3_0)_:
--1 GenericStorageBlock_storage_content(storage3_0)
+c_e_GenericStorageBlock_balance(storage3_0_0)_:
++1 flow(storage3_electricityBus_0_0)
+-1 flow(electricityBus_storage3_0_0)
 +1 GenericStorageBlock_storage_content(storage3_1)
--1 flow(electricityBus_storage3_0)
-+1 flow(storage3_electricityBus_0)
+-1 GenericStorageBlock_storage_content(storage3_0)
 = 0
 
-c_e_GenericStorageBlock_balance(storage3_1)_:
+c_e_GenericStorageBlock_balance(storage3_0_1)_:
++1 flow(storage3_electricityBus_0_1)
+-1 flow(electricityBus_storage3_0_1)
 -1 GenericStorageBlock_storage_content(storage3_1)
 +1 GenericStorageBlock_storage_content(storage3_2)
--1 flow(electricityBus_storage3_1)
-+1 flow(storage3_electricityBus_1)
 = 0
 
-c_e_GenericStorageBlock_balance(storage3_2)_:
+c_e_GenericStorageBlock_balance(storage3_0_2)_:
++1 flow(storage3_electricityBus_0_2)
+-1 flow(electricityBus_storage3_0_2)
 -1 GenericStorageBlock_storage_content(storage3_2)
 +1 GenericStorageBlock_storage_content(storage3_3)
--1 flow(electricityBus_storage3_2)
-+1 flow(storage3_electricityBus_2)
 = 0
 
 c_e_GenericStorageBlock_balanced_cstr(storage3)_:
 -1 GenericStorageBlock_storage_content(storage3_0)
 +1 GenericStorageBlock_storage_content(storage3_3)
 = 0
 
-c_e_ONE_VAR_CONSTANT: 
-ONE_VAR_CONSTANT = 1.0
-
 bounds
-   0 <= flow(electricityBus_storage3_0) <= +inf
-   0 <= flow(electricityBus_storage3_1) <= +inf
-   0 <= flow(electricityBus_storage3_2) <= +inf
-   0 <= flow(storage3_electricityBus_0) <= +inf
-   0 <= flow(storage3_electricityBus_1) <= +inf
-   0 <= flow(storage3_electricityBus_2) <= +inf
-   0 <= InvestmentFlowBlock_invest(electricityBus_storage3) <= +inf
-   0 <= InvestmentFlowBlock_invest(storage3_electricityBus) <= +inf
-   0 <= GenericStorageBlock_storage_content(storage3_0) <= 5000
+   0 <= InvestmentFlowBlock_invest(storage3_electricityBus_0) <= +inf
+   0 <= InvestmentFlowBlock_invest(electricityBus_storage3_0) <= +inf
+   0 <= flow(storage3_electricityBus_0_0) <= +inf
+   0 <= flow(electricityBus_storage3_0_0) <= +inf
+   0 <= flow(storage3_electricityBus_0_1) <= +inf
+   0 <= flow(electricityBus_storage3_0_1) <= +inf
+   0 <= flow(storage3_electricityBus_0_2) <= +inf
+   0 <= flow(electricityBus_storage3_0_2) <= +inf
+   0 <= InvestmentFlowBlock_total(storage3_electricityBus_0) <= +inf
+   0 <= InvestmentFlowBlock_total(electricityBus_storage3_0) <= +inf
    0 <= GenericStorageBlock_storage_content(storage3_1) <= 5000
+   0 <= GenericStorageBlock_storage_content(storage3_0) <= 5000
    0 <= GenericStorageBlock_storage_content(storage3_2) <= 5000
    0 <= GenericStorageBlock_storage_content(storage3_3) <= 5000
 end
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/storage_invest_4.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/storage_invest_4.lp`

 * *Files 7% similar despite different names*

```diff
@@ -1,85 +1,88 @@
 \* Source Pyomo model name=Model *\
 
-min
+min 
 objective:
-+145 GenericInvestmentStorageBlock_invest(storage4)
++145 GenericInvestmentStorageBlock_invest(storage4_0)
 
 s.t.
 
-c_e_BusBlock_balance(electricityBus_0)_:
--1 flow(electricityBus_storage4_0)
-+1 flow(storage4_electricityBus_0)
+c_e_BusBlock_balance(electricityBus_0_0)_:
++1 flow(storage4_electricityBus_0_0)
+-1 flow(electricityBus_storage4_0_0)
 = 0
 
-c_e_BusBlock_balance(electricityBus_1)_:
--1 flow(electricityBus_storage4_1)
-+1 flow(storage4_electricityBus_1)
+c_e_BusBlock_balance(electricityBus_0_1)_:
++1 flow(storage4_electricityBus_0_1)
+-1 flow(electricityBus_storage4_0_1)
 = 0
 
-c_e_BusBlock_balance(electricityBus_2)_:
--1 flow(electricityBus_storage4_2)
-+1 flow(storage4_electricityBus_2)
+c_e_BusBlock_balance(electricityBus_0_2)_:
++1 flow(storage4_electricityBus_0_2)
+-1 flow(electricityBus_storage4_0_2)
+= 0
+
+c_e_GenericInvestmentStorageBlock_total_storage_rule(storage4_0)_:
+-1 GenericInvestmentStorageBlock_invest(storage4_0)
++1 GenericInvestmentStorageBlock_total(storage4_0)
 = 0
 
 c_u_GenericInvestmentStorageBlock_init_content_limit(storage4)_:
+-1 GenericInvestmentStorageBlock_invest(storage4_0)
 +1 GenericInvestmentStorageBlock_init_content(storage4)
--1 GenericInvestmentStorageBlock_invest(storage4)
 <= 0
 
 c_e_GenericInvestmentStorageBlock_balance_first(storage4)_:
++1 flow(storage4_electricityBus_0_0)
+-1 flow(electricityBus_storage4_0_0)
 -1 GenericInvestmentStorageBlock_init_content(storage4)
 +1 GenericInvestmentStorageBlock_storage_content(storage4_0)
--1 flow(electricityBus_storage4_0)
-+1 flow(storage4_electricityBus_0)
 = 0
 
-c_e_GenericInvestmentStorageBlock_balance(storage4_1)_:
+c_e_GenericInvestmentStorageBlock_balance(storage4_0_1)_:
++1 flow(storage4_electricityBus_0_1)
+-1 flow(electricityBus_storage4_0_1)
 -1 GenericInvestmentStorageBlock_storage_content(storage4_0)
 +1 GenericInvestmentStorageBlock_storage_content(storage4_1)
--1 flow(electricityBus_storage4_1)
-+1 flow(storage4_electricityBus_1)
 = 0
 
-c_e_GenericInvestmentStorageBlock_balance(storage4_2)_:
+c_e_GenericInvestmentStorageBlock_balance(storage4_0_2)_:
++1 flow(storage4_electricityBus_0_2)
+-1 flow(electricityBus_storage4_0_2)
 -1 GenericInvestmentStorageBlock_storage_content(storage4_1)
 +1 GenericInvestmentStorageBlock_storage_content(storage4_2)
--1 flow(electricityBus_storage4_2)
-+1 flow(storage4_electricityBus_2)
 = 0
 
 c_e_GenericInvestmentStorageBlock_balanced_cstr(storage4)_:
 -1 GenericInvestmentStorageBlock_init_content(storage4)
 +1 GenericInvestmentStorageBlock_storage_content(storage4_2)
 = 0
 
-c_u_GenericInvestmentStorageBlock_max_storage_content(storage4_0)_:
--1 GenericInvestmentStorageBlock_invest(storage4)
+c_u_GenericInvestmentStorageBlock_max_storage_content(storage4_0_0)_:
+-1 GenericInvestmentStorageBlock_total(storage4_0)
 +1 GenericInvestmentStorageBlock_storage_content(storage4_0)
 <= 0
 
-c_u_GenericInvestmentStorageBlock_max_storage_content(storage4_1)_:
--1 GenericInvestmentStorageBlock_invest(storage4)
+c_u_GenericInvestmentStorageBlock_max_storage_content(storage4_0_1)_:
+-1 GenericInvestmentStorageBlock_total(storage4_0)
 +1 GenericInvestmentStorageBlock_storage_content(storage4_1)
 <= 0
 
-c_u_GenericInvestmentStorageBlock_max_storage_content(storage4_2)_:
--1 GenericInvestmentStorageBlock_invest(storage4)
+c_u_GenericInvestmentStorageBlock_max_storage_content(storage4_0_2)_:
+-1 GenericInvestmentStorageBlock_total(storage4_0)
 +1 GenericInvestmentStorageBlock_storage_content(storage4_2)
 <= 0
 
-c_e_ONE_VAR_CONSTANT:
-ONE_VAR_CONSTANT = 1.0
-
 bounds
-   0 <= flow(electricityBus_storage4_0) <= 80
-   0 <= flow(electricityBus_storage4_1) <= 80
-   0 <= flow(electricityBus_storage4_2) <= 80
-   0 <= flow(storage4_electricityBus_0) <= 100
-   0 <= flow(storage4_electricityBus_1) <= 100
-   0 <= flow(storage4_electricityBus_2) <= 100
+   0 <= GenericInvestmentStorageBlock_invest(storage4_0) <= 500
+   0 <= flow(storage4_electricityBus_0_0) <= 100
+   0 <= flow(electricityBus_storage4_0_0) <= 80
+   0 <= flow(storage4_electricityBus_0_1) <= 100
+   0 <= flow(electricityBus_storage4_0_1) <= 80
+   0 <= flow(storage4_electricityBus_0_2) <= 100
+   0 <= flow(electricityBus_storage4_0_2) <= 80
+   0 <= GenericInvestmentStorageBlock_total(storage4_0) <= +inf
+   0 <= GenericInvestmentStorageBlock_init_content(storage4) <= +inf
    0 <= GenericInvestmentStorageBlock_storage_content(storage4_0) <= +inf
    0 <= GenericInvestmentStorageBlock_storage_content(storage4_1) <= +inf
    0 <= GenericInvestmentStorageBlock_storage_content(storage4_2) <= +inf
-   0 <= GenericInvestmentStorageBlock_invest(storage4) <= 500
-   0 <= GenericInvestmentStorageBlock_init_content(storage4) <= +inf
 end
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/storage_invest_6.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/storage_invest_5.lp`

 * *Files 16% similar despite different names*

```diff
@@ -1,123 +1,110 @@
 \* Source Pyomo model name=Model *\
 
-min
+min 
 objective:
-+145 GenericInvestmentStorageBlock_invest(storage6)
-+99 InvestmentFlowBlock_invest(electricityBus_storage6)
++99 InvestmentFlowBlock_invest(electricityBus_storage5_0)
 
 s.t.
 
-c_e_BusBlock_balance(electricityBus_0)_:
--1 flow(electricityBus_storage6_0)
-+1 flow(storage6_electricityBus_0)
+c_e_BusBlock_balance(electricityBus_0_0)_:
++1 flow(storage5_electricityBus_0_0)
+-1 flow(electricityBus_storage5_0_0)
 = 0
 
-c_e_BusBlock_balance(electricityBus_1)_:
--1 flow(electricityBus_storage6_1)
-+1 flow(storage6_electricityBus_1)
+c_e_BusBlock_balance(electricityBus_0_1)_:
++1 flow(storage5_electricityBus_0_1)
+-1 flow(electricityBus_storage5_0_1)
 = 0
 
-c_e_BusBlock_balance(electricityBus_2)_:
--1 flow(electricityBus_storage6_2)
-+1 flow(storage6_electricityBus_2)
+c_e_BusBlock_balance(electricityBus_0_2)_:
++1 flow(storage5_electricityBus_0_2)
+-1 flow(electricityBus_storage5_0_2)
 = 0
 
-c_u_InvestmentFlowBlock_max(electricityBus_storage6_0)_:
--1 InvestmentFlowBlock_invest(electricityBus_storage6)
-+1 flow(electricityBus_storage6_0)
-<= 110
+c_e_InvestmentFlowBlock_total_rule(storage5_electricityBus_0)_:
++1 InvestmentFlowBlock_total(storage5_electricityBus_0)
+-1 InvestmentFlowBlock_invest(storage5_electricityBus_0)
+= 100
 
-c_u_InvestmentFlowBlock_max(electricityBus_storage6_1)_:
--1 InvestmentFlowBlock_invest(electricityBus_storage6)
-+1 flow(electricityBus_storage6_1)
-<= 110
+c_e_InvestmentFlowBlock_total_rule(electricityBus_storage5_0)_:
+-1 InvestmentFlowBlock_invest(electricityBus_storage5_0)
++1 InvestmentFlowBlock_total(electricityBus_storage5_0)
+= 110
 
-c_u_InvestmentFlowBlock_max(electricityBus_storage6_2)_:
--1 InvestmentFlowBlock_invest(electricityBus_storage6)
-+1 flow(electricityBus_storage6_2)
-<= 110
+c_u_InvestmentFlowBlock_max(storage5_electricityBus_0_0)_:
++1 flow(storage5_electricityBus_0_0)
+-1 InvestmentFlowBlock_total(storage5_electricityBus_0)
+<= 0
 
-c_u_InvestmentFlowBlock_max(storage6_electricityBus_0)_:
--1 InvestmentFlowBlock_invest(storage6_electricityBus)
-+1 flow(storage6_electricityBus_0)
-<= 100
+c_u_InvestmentFlowBlock_max(storage5_electricityBus_0_1)_:
++1 flow(storage5_electricityBus_0_1)
+-1 InvestmentFlowBlock_total(storage5_electricityBus_0)
+<= 0
 
-c_u_InvestmentFlowBlock_max(storage6_electricityBus_1)_:
--1 InvestmentFlowBlock_invest(storage6_electricityBus)
-+1 flow(storage6_electricityBus_1)
-<= 100
+c_u_InvestmentFlowBlock_max(storage5_electricityBus_0_2)_:
++1 flow(storage5_electricityBus_0_2)
+-1 InvestmentFlowBlock_total(storage5_electricityBus_0)
+<= 0
 
-c_u_InvestmentFlowBlock_max(storage6_electricityBus_2)_:
--1 InvestmentFlowBlock_invest(storage6_electricityBus)
-+1 flow(storage6_electricityBus_2)
-<= 100
+c_u_InvestmentFlowBlock_max(electricityBus_storage5_0_0)_:
++1 flow(electricityBus_storage5_0_0)
+-1 InvestmentFlowBlock_total(electricityBus_storage5_0)
+<= 0
 
-c_u_GenericInvestmentStorageBlock_init_content_limit(storage6)_:
-+1 GenericInvestmentStorageBlock_init_content(storage6)
--1 GenericInvestmentStorageBlock_invest(storage6)
-<= 10000
+c_u_InvestmentFlowBlock_max(electricityBus_storage5_0_1)_:
++1 flow(electricityBus_storage5_0_1)
+-1 InvestmentFlowBlock_total(electricityBus_storage5_0)
+<= 0
 
-c_e_GenericInvestmentStorageBlock_balance_first(storage6)_:
--1 GenericInvestmentStorageBlock_init_content(storage6)
-+1 GenericInvestmentStorageBlock_storage_content(storage6_0)
--1 flow(electricityBus_storage6_0)
-+1 flow(storage6_electricityBus_0)
-= 0
+c_u_InvestmentFlowBlock_max(electricityBus_storage5_0_2)_:
++1 flow(electricityBus_storage5_0_2)
+-1 InvestmentFlowBlock_total(electricityBus_storage5_0)
+<= 0
 
-c_e_GenericInvestmentStorageBlock_balance(storage6_1)_:
--1 GenericInvestmentStorageBlock_storage_content(storage6_0)
-+1 GenericInvestmentStorageBlock_storage_content(storage6_1)
--1 flow(electricityBus_storage6_1)
-+1 flow(storage6_electricityBus_1)
+c_e_GenericStorageBlock_balance(storage5_0_0)_:
++1 flow(storage5_electricityBus_0_0)
+-1 flow(electricityBus_storage5_0_0)
++1 GenericStorageBlock_storage_content(storage5_1)
+-1 GenericStorageBlock_storage_content(storage5_0)
 = 0
 
-c_e_GenericInvestmentStorageBlock_balance(storage6_2)_:
--1 GenericInvestmentStorageBlock_storage_content(storage6_1)
-+1 GenericInvestmentStorageBlock_storage_content(storage6_2)
--1 flow(electricityBus_storage6_2)
-+1 flow(storage6_electricityBus_2)
+c_e_GenericStorageBlock_balance(storage5_0_1)_:
++1 flow(storage5_electricityBus_0_1)
+-1 flow(electricityBus_storage5_0_1)
+-1 GenericStorageBlock_storage_content(storage5_1)
++1 GenericStorageBlock_storage_content(storage5_2)
 = 0
 
-c_e_GenericInvestmentStorageBlock_balanced_cstr(storage6)_:
--1 GenericInvestmentStorageBlock_init_content(storage6)
-+1 GenericInvestmentStorageBlock_storage_content(storage6_2)
+c_e_GenericStorageBlock_balance(storage5_0_2)_:
++1 flow(storage5_electricityBus_0_2)
+-1 flow(electricityBus_storage5_0_2)
+-1 GenericStorageBlock_storage_content(storage5_2)
++1 GenericStorageBlock_storage_content(storage5_3)
 = 0
 
-c_e_GenericInvestmentStorageBlock_power_coupled(storage6)_:
--1 InvestmentFlowBlock_invest(electricityBus_storage6)
-+1.1000000000000001 InvestmentFlowBlock_invest(storage6_electricityBus)
-= -1.4210854715202004e-14
-
-c_u_GenericInvestmentStorageBlock_max_storage_content(storage6_0)_:
--1 GenericInvestmentStorageBlock_invest(storage6)
-+1 GenericInvestmentStorageBlock_storage_content(storage6_0)
-<= 10000
-
-c_u_GenericInvestmentStorageBlock_max_storage_content(storage6_1)_:
--1 GenericInvestmentStorageBlock_invest(storage6)
-+1 GenericInvestmentStorageBlock_storage_content(storage6_1)
-<= 10000
-
-c_u_GenericInvestmentStorageBlock_max_storage_content(storage6_2)_:
--1 GenericInvestmentStorageBlock_invest(storage6)
-+1 GenericInvestmentStorageBlock_storage_content(storage6_2)
-<= 10000
+c_e_GenericStorageBlock_balanced_cstr(storage5)_:
+-1 GenericStorageBlock_storage_content(storage5_0)
++1 GenericStorageBlock_storage_content(storage5_3)
+= 0
 
-c_e_ONE_VAR_CONSTANT:
-ONE_VAR_CONSTANT = 1.0
+c_e_GenericStorageBlock_power_coupled(storage5_0)_:
++1.1 InvestmentFlowBlock_total(storage5_electricityBus_0)
+-1 InvestmentFlowBlock_total(electricityBus_storage5_0)
+= 0
 
 bounds
-   0 <= flow(electricityBus_storage6_0) <= +inf
-   0 <= flow(electricityBus_storage6_1) <= +inf
-   0 <= flow(electricityBus_storage6_2) <= +inf
-   0 <= flow(storage6_electricityBus_0) <= +inf
-   0 <= flow(storage6_electricityBus_1) <= +inf
-   0 <= flow(storage6_electricityBus_2) <= +inf
-   0 <= InvestmentFlowBlock_invest(electricityBus_storage6) <= +inf
-   0 <= InvestmentFlowBlock_invest(storage6_electricityBus) <= +inf
-   0 <= GenericInvestmentStorageBlock_storage_content(storage6_0) <= +inf
-   0 <= GenericInvestmentStorageBlock_storage_content(storage6_1) <= +inf
-   0 <= GenericInvestmentStorageBlock_storage_content(storage6_2) <= +inf
-   0 <= GenericInvestmentStorageBlock_invest(storage6) <= +inf
-   0 <= GenericInvestmentStorageBlock_init_content(storage6) <= +inf
+   0 <= InvestmentFlowBlock_invest(electricityBus_storage5_0) <= +inf
+   0 <= flow(storage5_electricityBus_0_0) <= +inf
+   0 <= flow(electricityBus_storage5_0_0) <= +inf
+   0 <= flow(storage5_electricityBus_0_1) <= +inf
+   0 <= flow(electricityBus_storage5_0_1) <= +inf
+   0 <= flow(storage5_electricityBus_0_2) <= +inf
+   0 <= flow(electricityBus_storage5_0_2) <= +inf
+   0 <= InvestmentFlowBlock_total(storage5_electricityBus_0) <= +inf
+   0 <= InvestmentFlowBlock_invest(storage5_electricityBus_0) <= +inf
+   0 <= InvestmentFlowBlock_total(electricityBus_storage5_0) <= +inf
+   0 <= GenericStorageBlock_storage_content(storage5_1) <= 10000
+   0 <= GenericStorageBlock_storage_content(storage5_0) <= 10000
+   0 <= GenericStorageBlock_storage_content(storage5_2) <= 10000
+   0 <= GenericStorageBlock_storage_content(storage5_3) <= 10000
 end
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/storage_invest_all_nonconvex.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/storage_invest_all_nonconvex.lp`

 * *Files 7% similar despite different names*

```diff
@@ -1,159 +1,174 @@
 \* Source Pyomo model name=Model *\
 
-min
+min 
 objective:
-+20 GenericInvestmentStorageBlock_invest(storage_all_nonconvex)
-+30 GenericInvestmentStorageBlock_invest_status(storage_all_nonconvex)
-+10 InvestmentFlowBlock_invest(bus1_storage_all_nonconvex)
-+10 InvestmentFlowBlock_invest(storage_all_nonconvex_bus1)
-+10 InvestmentFlowBlock_invest_status(bus1_storage_all_nonconvex)
-+15 InvestmentFlowBlock_invest_status(storage_all_nonconvex_bus1)
++10 InvestmentFlowBlock_invest(storage_all_nonconvex_bus1_0)
++15 InvestmentFlowBlock_invest_status(storage_all_nonconvex_bus1_0)
++10 InvestmentFlowBlock_invest(bus1_storage_all_nonconvex_0)
++10 InvestmentFlowBlock_invest_status(bus1_storage_all_nonconvex_0)
++20 GenericInvestmentStorageBlock_invest(storage_all_nonconvex_0)
++30 GenericInvestmentStorageBlock_invest_status(storage_all_nonconvex_0)
 
 s.t.
 
-c_e_BusBlock_balance(bus1_0)_:
--1 flow(bus1_storage_all_nonconvex_0)
-+1 flow(storage_all_nonconvex_bus1_0)
+c_e_BusBlock_balance(bus1_0_0)_:
++1 flow(storage_all_nonconvex_bus1_0_0)
+-1 flow(bus1_storage_all_nonconvex_0_0)
 = 0
 
-c_e_BusBlock_balance(bus1_1)_:
--1 flow(bus1_storage_all_nonconvex_1)
-+1 flow(storage_all_nonconvex_bus1_1)
+c_e_BusBlock_balance(bus1_0_1)_:
++1 flow(storage_all_nonconvex_bus1_0_1)
+-1 flow(bus1_storage_all_nonconvex_0_1)
 = 0
 
-c_e_BusBlock_balance(bus1_2)_:
--1 flow(bus1_storage_all_nonconvex_2)
-+1 flow(storage_all_nonconvex_bus1_2)
+c_e_BusBlock_balance(bus1_0_2)_:
++1 flow(storage_all_nonconvex_bus1_0_2)
+-1 flow(bus1_storage_all_nonconvex_0_2)
 = 0
 
-c_u_InvestmentFlowBlock_minimum_rule(bus1_storage_all_nonconvex)_:
--1 InvestmentFlowBlock_invest(bus1_storage_all_nonconvex)
-+5 InvestmentFlowBlock_invest_status(bus1_storage_all_nonconvex)
+c_u_InvestmentFlowBlock_minimum_rule(storage_all_nonconvex_bus1_0)_:
+-1 InvestmentFlowBlock_invest(storage_all_nonconvex_bus1_0)
++8 InvestmentFlowBlock_invest_status(storage_all_nonconvex_bus1_0)
 <= 0
 
-c_u_InvestmentFlowBlock_minimum_rule(storage_all_nonconvex_bus1)_:
--1 InvestmentFlowBlock_invest(storage_all_nonconvex_bus1)
-+8 InvestmentFlowBlock_invest_status(storage_all_nonconvex_bus1)
+c_u_InvestmentFlowBlock_minimum_rule(bus1_storage_all_nonconvex_0)_:
+-1 InvestmentFlowBlock_invest(bus1_storage_all_nonconvex_0)
++5 InvestmentFlowBlock_invest_status(bus1_storage_all_nonconvex_0)
 <= 0
 
-c_u_InvestmentFlowBlock_maximum_rule(bus1_storage_all_nonconvex)_:
-+1 InvestmentFlowBlock_invest(bus1_storage_all_nonconvex)
--30 InvestmentFlowBlock_invest_status(bus1_storage_all_nonconvex)
+c_u_InvestmentFlowBlock_maximum_rule(storage_all_nonconvex_bus1_0)_:
++1 InvestmentFlowBlock_invest(storage_all_nonconvex_bus1_0)
+-20 InvestmentFlowBlock_invest_status(storage_all_nonconvex_bus1_0)
 <= 0
 
-c_u_InvestmentFlowBlock_maximum_rule(storage_all_nonconvex_bus1)_:
-+1 InvestmentFlowBlock_invest(storage_all_nonconvex_bus1)
--20 InvestmentFlowBlock_invest_status(storage_all_nonconvex_bus1)
+c_u_InvestmentFlowBlock_maximum_rule(bus1_storage_all_nonconvex_0)_:
++1 InvestmentFlowBlock_invest(bus1_storage_all_nonconvex_0)
+-30 InvestmentFlowBlock_invest_status(bus1_storage_all_nonconvex_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(bus1_storage_all_nonconvex_0)_:
--1 InvestmentFlowBlock_invest(bus1_storage_all_nonconvex)
-+1 flow(bus1_storage_all_nonconvex_0)
+c_e_InvestmentFlowBlock_total_rule(storage_all_nonconvex_bus1_0)_:
+-1 InvestmentFlowBlock_invest(storage_all_nonconvex_bus1_0)
++1 InvestmentFlowBlock_total(storage_all_nonconvex_bus1_0)
+= 0
+
+c_e_InvestmentFlowBlock_total_rule(bus1_storage_all_nonconvex_0)_:
+-1 InvestmentFlowBlock_invest(bus1_storage_all_nonconvex_0)
++1 InvestmentFlowBlock_total(bus1_storage_all_nonconvex_0)
+= 0
+
+c_u_InvestmentFlowBlock_max(storage_all_nonconvex_bus1_0_0)_:
++1 flow(storage_all_nonconvex_bus1_0_0)
+-1 InvestmentFlowBlock_total(storage_all_nonconvex_bus1_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(bus1_storage_all_nonconvex_1)_:
--1 InvestmentFlowBlock_invest(bus1_storage_all_nonconvex)
-+1 flow(bus1_storage_all_nonconvex_1)
+c_u_InvestmentFlowBlock_max(storage_all_nonconvex_bus1_0_1)_:
++1 flow(storage_all_nonconvex_bus1_0_1)
+-1 InvestmentFlowBlock_total(storage_all_nonconvex_bus1_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(bus1_storage_all_nonconvex_2)_:
--1 InvestmentFlowBlock_invest(bus1_storage_all_nonconvex)
-+1 flow(bus1_storage_all_nonconvex_2)
+c_u_InvestmentFlowBlock_max(storage_all_nonconvex_bus1_0_2)_:
++1 flow(storage_all_nonconvex_bus1_0_2)
+-1 InvestmentFlowBlock_total(storage_all_nonconvex_bus1_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(storage_all_nonconvex_bus1_0)_:
--1 InvestmentFlowBlock_invest(storage_all_nonconvex_bus1)
-+1 flow(storage_all_nonconvex_bus1_0)
+c_u_InvestmentFlowBlock_max(bus1_storage_all_nonconvex_0_0)_:
++1 flow(bus1_storage_all_nonconvex_0_0)
+-1 InvestmentFlowBlock_total(bus1_storage_all_nonconvex_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(storage_all_nonconvex_bus1_1)_:
--1 InvestmentFlowBlock_invest(storage_all_nonconvex_bus1)
-+1 flow(storage_all_nonconvex_bus1_1)
+c_u_InvestmentFlowBlock_max(bus1_storage_all_nonconvex_0_1)_:
++1 flow(bus1_storage_all_nonconvex_0_1)
+-1 InvestmentFlowBlock_total(bus1_storage_all_nonconvex_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(storage_all_nonconvex_bus1_2)_:
--1 InvestmentFlowBlock_invest(storage_all_nonconvex_bus1)
-+1 flow(storage_all_nonconvex_bus1_2)
+c_u_InvestmentFlowBlock_max(bus1_storage_all_nonconvex_0_2)_:
++1 flow(bus1_storage_all_nonconvex_0_2)
+-1 InvestmentFlowBlock_total(bus1_storage_all_nonconvex_0)
 <= 0
 
+c_e_GenericInvestmentStorageBlock_total_storage_rule(storage_all_nonconvex_0)_:
+-1 GenericInvestmentStorageBlock_invest(storage_all_nonconvex_0)
++1 GenericInvestmentStorageBlock_total(storage_all_nonconvex_0)
+= 0
+
 c_u_GenericInvestmentStorageBlock_init_content_limit(storage_all_nonconvex)_:
+-1 GenericInvestmentStorageBlock_invest(storage_all_nonconvex_0)
 +1 GenericInvestmentStorageBlock_init_content(storage_all_nonconvex)
--1 GenericInvestmentStorageBlock_invest(storage_all_nonconvex)
 <= 0
 
 c_e_GenericInvestmentStorageBlock_balance_first(storage_all_nonconvex)_:
++1 flow(storage_all_nonconvex_bus1_0_0)
+-1 flow(bus1_storage_all_nonconvex_0_0)
 -1 GenericInvestmentStorageBlock_init_content(storage_all_nonconvex)
 +1 GenericInvestmentStorageBlock_storage_content(storage_all_nonconvex_0)
--1 flow(bus1_storage_all_nonconvex_0)
-+1 flow(storage_all_nonconvex_bus1_0)
 = 0
 
-c_e_GenericInvestmentStorageBlock_balance(storage_all_nonconvex_1)_:
+c_e_GenericInvestmentStorageBlock_balance(storage_all_nonconvex_0_1)_:
++1 flow(storage_all_nonconvex_bus1_0_1)
+-1 flow(bus1_storage_all_nonconvex_0_1)
 -1 GenericInvestmentStorageBlock_storage_content(storage_all_nonconvex_0)
 +1 GenericInvestmentStorageBlock_storage_content(storage_all_nonconvex_1)
--1 flow(bus1_storage_all_nonconvex_1)
-+1 flow(storage_all_nonconvex_bus1_1)
 = 0
 
-c_e_GenericInvestmentStorageBlock_balance(storage_all_nonconvex_2)_:
+c_e_GenericInvestmentStorageBlock_balance(storage_all_nonconvex_0_2)_:
++1 flow(storage_all_nonconvex_bus1_0_2)
+-1 flow(bus1_storage_all_nonconvex_0_2)
 -1 GenericInvestmentStorageBlock_storage_content(storage_all_nonconvex_1)
 +1 GenericInvestmentStorageBlock_storage_content(storage_all_nonconvex_2)
--1 flow(bus1_storage_all_nonconvex_2)
-+1 flow(storage_all_nonconvex_bus1_2)
 = 0
 
 c_e_GenericInvestmentStorageBlock_balanced_cstr(storage_all_nonconvex)_:
 -1 GenericInvestmentStorageBlock_init_content(storage_all_nonconvex)
 +1 GenericInvestmentStorageBlock_storage_content(storage_all_nonconvex_2)
 = 0
 
-c_u_GenericInvestmentStorageBlock_max_storage_content(storage_all_nonconvex_0)_:
--1 GenericInvestmentStorageBlock_invest(storage_all_nonconvex)
+c_u_GenericInvestmentStorageBlock_max_storage_content(storage_all_nonconvex_0_0)_:
+-1 GenericInvestmentStorageBlock_total(storage_all_nonconvex_0)
 +1 GenericInvestmentStorageBlock_storage_content(storage_all_nonconvex_0)
 <= 0
 
-c_u_GenericInvestmentStorageBlock_max_storage_content(storage_all_nonconvex_1)_:
--1 GenericInvestmentStorageBlock_invest(storage_all_nonconvex)
+c_u_GenericInvestmentStorageBlock_max_storage_content(storage_all_nonconvex_0_1)_:
+-1 GenericInvestmentStorageBlock_total(storage_all_nonconvex_0)
 +1 GenericInvestmentStorageBlock_storage_content(storage_all_nonconvex_1)
 <= 0
 
-c_u_GenericInvestmentStorageBlock_max_storage_content(storage_all_nonconvex_2)_:
--1 GenericInvestmentStorageBlock_invest(storage_all_nonconvex)
+c_u_GenericInvestmentStorageBlock_max_storage_content(storage_all_nonconvex_0_2)_:
+-1 GenericInvestmentStorageBlock_total(storage_all_nonconvex_0)
 +1 GenericInvestmentStorageBlock_storage_content(storage_all_nonconvex_2)
 <= 0
 
-c_l_GenericInvestmentStorageBlock_limit_max(storage_all_nonconvex)_:
--1 GenericInvestmentStorageBlock_invest(storage_all_nonconvex)
-+100 GenericInvestmentStorageBlock_invest_status(storage_all_nonconvex)
+c_l_GenericInvestmentStorageBlock_limit_max(storage_all_nonconvex_0)_:
+-1 GenericInvestmentStorageBlock_invest(storage_all_nonconvex_0)
++100 GenericInvestmentStorageBlock_invest_status(storage_all_nonconvex_0)
 >= 0
 
-c_l_GenericInvestmentStorageBlock_limit_min(storage_all_nonconvex)_:
-+1 GenericInvestmentStorageBlock_invest(storage_all_nonconvex)
--20 GenericInvestmentStorageBlock_invest_status(storage_all_nonconvex)
+c_l_GenericInvestmentStorageBlock_limit_min(storage_all_nonconvex_0)_:
++1 GenericInvestmentStorageBlock_invest(storage_all_nonconvex_0)
+-20 GenericInvestmentStorageBlock_invest_status(storage_all_nonconvex_0)
 >= 0
 
-c_e_ONE_VAR_CONSTANT:
-ONE_VAR_CONSTANT = 1.0
-
 bounds
-   0 <= flow(bus1_storage_all_nonconvex_0) <= +inf
-   0 <= flow(bus1_storage_all_nonconvex_1) <= +inf
-   0 <= flow(bus1_storage_all_nonconvex_2) <= +inf
-   0 <= flow(storage_all_nonconvex_bus1_0) <= +inf
-   0 <= flow(storage_all_nonconvex_bus1_1) <= +inf
-   0 <= flow(storage_all_nonconvex_bus1_2) <= +inf
-   0 <= InvestmentFlowBlock_invest(bus1_storage_all_nonconvex) <= 30
-   0 <= InvestmentFlowBlock_invest(storage_all_nonconvex_bus1) <= 20
-   0 <= InvestmentFlowBlock_invest_status(bus1_storage_all_nonconvex) <= 1
-   0 <= InvestmentFlowBlock_invest_status(storage_all_nonconvex_bus1) <= 1
+   0 <= InvestmentFlowBlock_invest(storage_all_nonconvex_bus1_0) <= 20
+   0 <= InvestmentFlowBlock_invest_status(storage_all_nonconvex_bus1_0) <= 1
+   0 <= InvestmentFlowBlock_invest(bus1_storage_all_nonconvex_0) <= 30
+   0 <= InvestmentFlowBlock_invest_status(bus1_storage_all_nonconvex_0) <= 1
+   0 <= GenericInvestmentStorageBlock_invest(storage_all_nonconvex_0) <= 100
+   0 <= GenericInvestmentStorageBlock_invest_status(storage_all_nonconvex_0) <= 1
+   0 <= flow(storage_all_nonconvex_bus1_0_0) <= +inf
+   0 <= flow(bus1_storage_all_nonconvex_0_0) <= +inf
+   0 <= flow(storage_all_nonconvex_bus1_0_1) <= +inf
+   0 <= flow(bus1_storage_all_nonconvex_0_1) <= +inf
+   0 <= flow(storage_all_nonconvex_bus1_0_2) <= +inf
+   0 <= flow(bus1_storage_all_nonconvex_0_2) <= +inf
+   0 <= InvestmentFlowBlock_total(storage_all_nonconvex_bus1_0) <= +inf
+   0 <= InvestmentFlowBlock_total(bus1_storage_all_nonconvex_0) <= +inf
+   0 <= GenericInvestmentStorageBlock_total(storage_all_nonconvex_0) <= +inf
+   0 <= GenericInvestmentStorageBlock_init_content(storage_all_nonconvex) <= +inf
    0 <= GenericInvestmentStorageBlock_storage_content(storage_all_nonconvex_0) <= +inf
    0 <= GenericInvestmentStorageBlock_storage_content(storage_all_nonconvex_1) <= +inf
    0 <= GenericInvestmentStorageBlock_storage_content(storage_all_nonconvex_2) <= +inf
-   0 <= GenericInvestmentStorageBlock_invest(storage_all_nonconvex) <= 100
-   0 <= GenericInvestmentStorageBlock_init_content(storage_all_nonconvex) <= +inf
-   0 <= GenericInvestmentStorageBlock_invest_status(storage_all_nonconvex) <= 1
 binary
-  InvestmentFlowBlock_invest_status(bus1_storage_all_nonconvex)
-  InvestmentFlowBlock_invest_status(storage_all_nonconvex_bus1)
-  GenericInvestmentStorageBlock_invest_status(storage_all_nonconvex)
+  InvestmentFlowBlock_invest_status(storage_all_nonconvex_bus1_0)
+  InvestmentFlowBlock_invest_status(bus1_storage_all_nonconvex_0)
+  GenericInvestmentStorageBlock_invest_status(storage_all_nonconvex_0)
 end
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/storage_invest_minimum.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/storage_invest_minimum.lp`

 * *Files 11% similar despite different names*

```diff
@@ -1,85 +1,88 @@
 \* Source Pyomo model name=Model *\
 
-min
+min 
 objective:
-+145 GenericInvestmentStorageBlock_invest(storage1)
++145 GenericInvestmentStorageBlock_invest(storage1_0)
 
 s.t.
 
-c_e_BusBlock_balance(electricityBus_0)_:
--1 flow(electricityBus_storage1_0)
-+1 flow(storage1_electricityBus_0)
+c_e_BusBlock_balance(electricityBus_0_0)_:
++1 flow(storage1_electricityBus_0_0)
+-1 flow(electricityBus_storage1_0_0)
 = 0
 
-c_e_BusBlock_balance(electricityBus_1)_:
--1 flow(electricityBus_storage1_1)
-+1 flow(storage1_electricityBus_1)
+c_e_BusBlock_balance(electricityBus_0_1)_:
++1 flow(storage1_electricityBus_0_1)
+-1 flow(electricityBus_storage1_0_1)
 = 0
 
-c_e_BusBlock_balance(electricityBus_2)_:
--1 flow(electricityBus_storage1_2)
-+1 flow(storage1_electricityBus_2)
+c_e_BusBlock_balance(electricityBus_0_2)_:
++1 flow(storage1_electricityBus_0_2)
+-1 flow(electricityBus_storage1_0_2)
+= 0
+
+c_e_GenericInvestmentStorageBlock_total_storage_rule(storage1_0)_:
+-1 GenericInvestmentStorageBlock_invest(storage1_0)
++1 GenericInvestmentStorageBlock_total(storage1_0)
 = 0
 
 c_u_GenericInvestmentStorageBlock_init_content_limit(storage1)_:
+-1 GenericInvestmentStorageBlock_invest(storage1_0)
 +1 GenericInvestmentStorageBlock_init_content(storage1)
--1 GenericInvestmentStorageBlock_invest(storage1)
 <= 0
 
 c_e_GenericInvestmentStorageBlock_balance_first(storage1)_:
++1 flow(storage1_electricityBus_0_0)
+-1 flow(electricityBus_storage1_0_0)
 -1 GenericInvestmentStorageBlock_init_content(storage1)
 +1 GenericInvestmentStorageBlock_storage_content(storage1_0)
--1 flow(electricityBus_storage1_0)
-+1 flow(storage1_electricityBus_0)
 = 0
 
-c_e_GenericInvestmentStorageBlock_balance(storage1_1)_:
+c_e_GenericInvestmentStorageBlock_balance(storage1_0_1)_:
++1 flow(storage1_electricityBus_0_1)
+-1 flow(electricityBus_storage1_0_1)
 -1 GenericInvestmentStorageBlock_storage_content(storage1_0)
 +1 GenericInvestmentStorageBlock_storage_content(storage1_1)
--1 flow(electricityBus_storage1_1)
-+1 flow(storage1_electricityBus_1)
 = 0
 
-c_e_GenericInvestmentStorageBlock_balance(storage1_2)_:
+c_e_GenericInvestmentStorageBlock_balance(storage1_0_2)_:
++1 flow(storage1_electricityBus_0_2)
+-1 flow(electricityBus_storage1_0_2)
 -1 GenericInvestmentStorageBlock_storage_content(storage1_1)
 +1 GenericInvestmentStorageBlock_storage_content(storage1_2)
--1 flow(electricityBus_storage1_2)
-+1 flow(storage1_electricityBus_2)
 = 0
 
 c_e_GenericInvestmentStorageBlock_balanced_cstr(storage1)_:
 -1 GenericInvestmentStorageBlock_init_content(storage1)
 +1 GenericInvestmentStorageBlock_storage_content(storage1_2)
 = 0
 
-c_u_GenericInvestmentStorageBlock_max_storage_content(storage1_0)_:
--1 GenericInvestmentStorageBlock_invest(storage1)
+c_u_GenericInvestmentStorageBlock_max_storage_content(storage1_0_0)_:
+-1 GenericInvestmentStorageBlock_total(storage1_0)
 +1 GenericInvestmentStorageBlock_storage_content(storage1_0)
 <= 0
 
-c_u_GenericInvestmentStorageBlock_max_storage_content(storage1_1)_:
--1 GenericInvestmentStorageBlock_invest(storage1)
+c_u_GenericInvestmentStorageBlock_max_storage_content(storage1_0_1)_:
+-1 GenericInvestmentStorageBlock_total(storage1_0)
 +1 GenericInvestmentStorageBlock_storage_content(storage1_1)
 <= 0
 
-c_u_GenericInvestmentStorageBlock_max_storage_content(storage1_2)_:
--1 GenericInvestmentStorageBlock_invest(storage1)
+c_u_GenericInvestmentStorageBlock_max_storage_content(storage1_0_2)_:
+-1 GenericInvestmentStorageBlock_total(storage1_0)
 +1 GenericInvestmentStorageBlock_storage_content(storage1_2)
 <= 0
 
-c_e_ONE_VAR_CONSTANT:
-ONE_VAR_CONSTANT = 1.0
-
 bounds
-   0 <= flow(electricityBus_storage1_0) <= +inf
-   0 <= flow(electricityBus_storage1_1) <= +inf
-   0 <= flow(electricityBus_storage1_2) <= +inf
-   0 <= flow(storage1_electricityBus_0) <= +inf
-   0 <= flow(storage1_electricityBus_1) <= +inf
-   0 <= flow(storage1_electricityBus_2) <= +inf
+   100 <= GenericInvestmentStorageBlock_invest(storage1_0) <= 200
+   0 <= flow(storage1_electricityBus_0_0) <= +inf
+   0 <= flow(electricityBus_storage1_0_0) <= +inf
+   0 <= flow(storage1_electricityBus_0_1) <= +inf
+   0 <= flow(electricityBus_storage1_0_1) <= +inf
+   0 <= flow(storage1_electricityBus_0_2) <= +inf
+   0 <= flow(electricityBus_storage1_0_2) <= +inf
+   0 <= GenericInvestmentStorageBlock_total(storage1_0) <= +inf
+   0 <= GenericInvestmentStorageBlock_init_content(storage1) <= +inf
    0 <= GenericInvestmentStorageBlock_storage_content(storage1_0) <= +inf
    0 <= GenericInvestmentStorageBlock_storage_content(storage1_1) <= +inf
    0 <= GenericInvestmentStorageBlock_storage_content(storage1_2) <= +inf
-   100 <= GenericInvestmentStorageBlock_invest(storage1) <= 200
-   0 <= GenericInvestmentStorageBlock_init_content(storage1) <= +inf
 end
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/storage_invest_unbalanced.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/storage_invest_unbalanced.lp`

 * *Files 20% similar despite different names*

```diff
@@ -1,122 +1,137 @@
 \* Source Pyomo model name=Model *\
 
-min
+min 
 objective:
-+145 GenericInvestmentStorageBlock_invest(storage1)
++145 GenericInvestmentStorageBlock_invest(storage1_0)
 
 s.t.
 
-c_e_BusBlock_balance(electricityBus_0)_:
--1 flow(electricityBus_storage1_0)
-+1 flow(storage1_electricityBus_0)
+c_e_BusBlock_balance(electricityBus_0_0)_:
++1 flow(storage1_electricityBus_0_0)
+-1 flow(electricityBus_storage1_0_0)
 = 0
 
-c_e_BusBlock_balance(electricityBus_1)_:
--1 flow(electricityBus_storage1_1)
-+1 flow(storage1_electricityBus_1)
+c_e_BusBlock_balance(electricityBus_0_1)_:
++1 flow(storage1_electricityBus_0_1)
+-1 flow(electricityBus_storage1_0_1)
 = 0
 
-c_e_BusBlock_balance(electricityBus_2)_:
--1 flow(electricityBus_storage1_2)
-+1 flow(storage1_electricityBus_2)
+c_e_BusBlock_balance(electricityBus_0_2)_:
++1 flow(storage1_electricityBus_0_2)
+-1 flow(electricityBus_storage1_0_2)
 = 0
 
-c_u_InvestmentFlowBlock_max(electricityBus_storage1_0)_:
--1 InvestmentFlowBlock_invest(electricityBus_storage1)
-+1 flow(electricityBus_storage1_0)
+c_e_InvestmentFlowBlock_total_rule(electricityBus_storage1_0)_:
++1 InvestmentFlowBlock_total(electricityBus_storage1_0)
+-1 InvestmentFlowBlock_invest(electricityBus_storage1_0)
+= 0
+
+c_e_InvestmentFlowBlock_total_rule(storage1_electricityBus_0)_:
++1 InvestmentFlowBlock_total(storage1_electricityBus_0)
+-1 InvestmentFlowBlock_invest(storage1_electricityBus_0)
+= 0
+
+c_u_InvestmentFlowBlock_max(electricityBus_storage1_0_0)_:
++1 flow(electricityBus_storage1_0_0)
+-1 InvestmentFlowBlock_total(electricityBus_storage1_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(electricityBus_storage1_1)_:
--1 InvestmentFlowBlock_invest(electricityBus_storage1)
-+1 flow(electricityBus_storage1_1)
+c_u_InvestmentFlowBlock_max(electricityBus_storage1_0_1)_:
++1 flow(electricityBus_storage1_0_1)
+-1 InvestmentFlowBlock_total(electricityBus_storage1_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(electricityBus_storage1_2)_:
--1 InvestmentFlowBlock_invest(electricityBus_storage1)
-+1 flow(electricityBus_storage1_2)
+c_u_InvestmentFlowBlock_max(electricityBus_storage1_0_2)_:
++1 flow(electricityBus_storage1_0_2)
+-1 InvestmentFlowBlock_total(electricityBus_storage1_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(storage1_electricityBus_0)_:
--1 InvestmentFlowBlock_invest(storage1_electricityBus)
-+1 flow(storage1_electricityBus_0)
+c_u_InvestmentFlowBlock_max(storage1_electricityBus_0_0)_:
++1 flow(storage1_electricityBus_0_0)
+-1 InvestmentFlowBlock_total(storage1_electricityBus_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(storage1_electricityBus_1)_:
--1 InvestmentFlowBlock_invest(storage1_electricityBus)
-+1 flow(storage1_electricityBus_1)
+c_u_InvestmentFlowBlock_max(storage1_electricityBus_0_1)_:
++1 flow(storage1_electricityBus_0_1)
+-1 InvestmentFlowBlock_total(storage1_electricityBus_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(storage1_electricityBus_2)_:
--1 InvestmentFlowBlock_invest(storage1_electricityBus)
-+1 flow(storage1_electricityBus_2)
+c_u_InvestmentFlowBlock_max(storage1_electricityBus_0_2)_:
++1 flow(storage1_electricityBus_0_2)
+-1 InvestmentFlowBlock_total(storage1_electricityBus_0)
 <= 0
 
+c_e_GenericInvestmentStorageBlock_total_storage_rule(storage1_0)_:
+-1 GenericInvestmentStorageBlock_invest(storage1_0)
++1 GenericInvestmentStorageBlock_total(storage1_0)
+= 0
+
 c_e_GenericInvestmentStorageBlock_init_content_fix(storage1)_:
+-0.5 GenericInvestmentStorageBlock_invest(storage1_0)
 +1 GenericInvestmentStorageBlock_init_content(storage1)
--0.5 GenericInvestmentStorageBlock_invest(storage1)
 = 0
 
 c_e_GenericInvestmentStorageBlock_balance_first(storage1)_:
++1 flow(storage1_electricityBus_0_0)
+-1 flow(electricityBus_storage1_0_0)
 -1 GenericInvestmentStorageBlock_init_content(storage1)
 +1 GenericInvestmentStorageBlock_storage_content(storage1_0)
--1 flow(electricityBus_storage1_0)
-+1 flow(storage1_electricityBus_0)
 = 0
 
-c_e_GenericInvestmentStorageBlock_balance(storage1_1)_:
+c_e_GenericInvestmentStorageBlock_balance(storage1_0_1)_:
++1 flow(storage1_electricityBus_0_1)
+-1 flow(electricityBus_storage1_0_1)
 -1 GenericInvestmentStorageBlock_storage_content(storage1_0)
 +1 GenericInvestmentStorageBlock_storage_content(storage1_1)
--1 flow(electricityBus_storage1_1)
-+1 flow(storage1_electricityBus_1)
 = 0
 
-c_e_GenericInvestmentStorageBlock_balance(storage1_2)_:
+c_e_GenericInvestmentStorageBlock_balance(storage1_0_2)_:
++1 flow(storage1_electricityBus_0_2)
+-1 flow(electricityBus_storage1_0_2)
 -1 GenericInvestmentStorageBlock_storage_content(storage1_1)
 +1 GenericInvestmentStorageBlock_storage_content(storage1_2)
--1 flow(electricityBus_storage1_2)
-+1 flow(storage1_electricityBus_2)
 = 0
 
-c_e_GenericInvestmentStorageBlock_storage_capacity_inflow(storage1)_:
--1 GenericInvestmentStorageBlock_invest(storage1)
-+1 InvestmentFlowBlock_invest(electricityBus_storage1)
+c_e_GenericInvestmentStorageBlock_storage_capacity_inflow(storage1_0)_:
++1 InvestmentFlowBlock_total(electricityBus_storage1_0)
+-1 GenericInvestmentStorageBlock_total(storage1_0)
 = 0
 
-c_e_GenericInvestmentStorageBlock_storage_capacity_outflow(storage1)_:
--1 GenericInvestmentStorageBlock_invest(storage1)
-+1 InvestmentFlowBlock_invest(storage1_electricityBus)
+c_e_GenericInvestmentStorageBlock_storage_capacity_outflow(storage1_0)_:
++1 InvestmentFlowBlock_total(storage1_electricityBus_0)
+-1 GenericInvestmentStorageBlock_total(storage1_0)
 = 0
 
-c_u_GenericInvestmentStorageBlock_max_storage_content(storage1_0)_:
--1 GenericInvestmentStorageBlock_invest(storage1)
+c_u_GenericInvestmentStorageBlock_max_storage_content(storage1_0_0)_:
+-1 GenericInvestmentStorageBlock_total(storage1_0)
 +1 GenericInvestmentStorageBlock_storage_content(storage1_0)
 <= 0
 
-c_u_GenericInvestmentStorageBlock_max_storage_content(storage1_1)_:
--1 GenericInvestmentStorageBlock_invest(storage1)
+c_u_GenericInvestmentStorageBlock_max_storage_content(storage1_0_1)_:
+-1 GenericInvestmentStorageBlock_total(storage1_0)
 +1 GenericInvestmentStorageBlock_storage_content(storage1_1)
 <= 0
 
-c_u_GenericInvestmentStorageBlock_max_storage_content(storage1_2)_:
--1 GenericInvestmentStorageBlock_invest(storage1)
+c_u_GenericInvestmentStorageBlock_max_storage_content(storage1_0_2)_:
+-1 GenericInvestmentStorageBlock_total(storage1_0)
 +1 GenericInvestmentStorageBlock_storage_content(storage1_2)
 <= 0
 
-c_e_ONE_VAR_CONSTANT:
-ONE_VAR_CONSTANT = 1.0
-
 bounds
-   0 <= flow(electricityBus_storage1_0) <= +inf
-   0 <= flow(electricityBus_storage1_1) <= +inf
-   0 <= flow(electricityBus_storage1_2) <= +inf
-   0 <= flow(storage1_electricityBus_0) <= +inf
-   0 <= flow(storage1_electricityBus_1) <= +inf
-   0 <= flow(storage1_electricityBus_2) <= +inf
-   0 <= InvestmentFlowBlock_invest(electricityBus_storage1) <= +inf
-   0 <= InvestmentFlowBlock_invest(storage1_electricityBus) <= +inf
+   0 <= GenericInvestmentStorageBlock_invest(storage1_0) <= +inf
+   0 <= flow(storage1_electricityBus_0_0) <= +inf
+   0 <= flow(electricityBus_storage1_0_0) <= +inf
+   0 <= flow(storage1_electricityBus_0_1) <= +inf
+   0 <= flow(electricityBus_storage1_0_1) <= +inf
+   0 <= flow(storage1_electricityBus_0_2) <= +inf
+   0 <= flow(electricityBus_storage1_0_2) <= +inf
+   0 <= InvestmentFlowBlock_total(electricityBus_storage1_0) <= +inf
+   0 <= InvestmentFlowBlock_invest(electricityBus_storage1_0) <= +inf
+   0 <= InvestmentFlowBlock_total(storage1_electricityBus_0) <= +inf
+   0 <= InvestmentFlowBlock_invest(storage1_electricityBus_0) <= +inf
+   0 <= GenericInvestmentStorageBlock_total(storage1_0) <= +inf
+   0 <= GenericInvestmentStorageBlock_init_content(storage1) <= +inf
    0 <= GenericInvestmentStorageBlock_storage_content(storage1_0) <= +inf
    0 <= GenericInvestmentStorageBlock_storage_content(storage1_1) <= +inf
    0 <= GenericInvestmentStorageBlock_storage_content(storage1_2) <= +inf
-   0 <= GenericInvestmentStorageBlock_invest(storage1) <= +inf
-   0 <= GenericInvestmentStorageBlock_init_content(storage1) <= +inf
 end
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/storage_invest_with_offset.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/storage_invest_without_offset.lp`

 * *Files 18% similar despite different names*

```diff
@@ -1,162 +1,176 @@
 \* Source Pyomo model name=Model *\
 
-min
+min 
 objective:
-+145 GenericInvestmentStorageBlock_invest(storagenon_convex)
-+5 GenericInvestmentStorageBlock_invest_status(storagenon_convex)
-+56 flow(electricityBus_storagenon_convex_0)
-+56 flow(electricityBus_storagenon_convex_1)
-+56 flow(electricityBus_storagenon_convex_2)
-+24 flow(storagenon_convex_electricityBus_0)
-+24 flow(storagenon_convex_electricityBus_1)
-+24 flow(storagenon_convex_electricityBus_2)
++56 flow(electricityBus_storage_non_convex_0_0)
++56 flow(electricityBus_storage_non_convex_0_1)
++56 flow(electricityBus_storage_non_convex_0_2)
++24 flow(storage_non_convex_electricityBus_0_0)
++24 flow(storage_non_convex_electricityBus_0_1)
++24 flow(storage_non_convex_electricityBus_0_2)
++141 GenericInvestmentStorageBlock_invest(storage_non_convex_0)
 
 s.t.
 
-c_e_BusBlock_balance(electricityBus_0)_:
--1 flow(electricityBus_storagenon_convex_0)
-+1 flow(storagenon_convex_electricityBus_0)
+c_e_BusBlock_balance(electricityBus_0_0)_:
+-1 flow(electricityBus_storage_non_convex_0_0)
++1 flow(storage_non_convex_electricityBus_0_0)
 = 0
 
-c_e_BusBlock_balance(electricityBus_1)_:
--1 flow(electricityBus_storagenon_convex_1)
-+1 flow(storagenon_convex_electricityBus_1)
+c_e_BusBlock_balance(electricityBus_0_1)_:
+-1 flow(electricityBus_storage_non_convex_0_1)
++1 flow(storage_non_convex_electricityBus_0_1)
 = 0
 
-c_e_BusBlock_balance(electricityBus_2)_:
--1 flow(electricityBus_storagenon_convex_2)
-+1 flow(storagenon_convex_electricityBus_2)
+c_e_BusBlock_balance(electricityBus_0_2)_:
+-1 flow(electricityBus_storage_non_convex_0_2)
++1 flow(storage_non_convex_electricityBus_0_2)
 = 0
 
-c_u_InvestmentFlowBlock_max(electricityBus_storagenon_convex_0)_:
--1 InvestmentFlowBlock_invest(electricityBus_storagenon_convex)
-+1 flow(electricityBus_storagenon_convex_0)
+c_e_InvestmentFlowBlock_total_rule(storage_non_convex_electricityBus_0)_:
++1 InvestmentFlowBlock_total(storage_non_convex_electricityBus_0)
+-1 InvestmentFlowBlock_invest(storage_non_convex_electricityBus_0)
+= 0
+
+c_e_InvestmentFlowBlock_total_rule(electricityBus_storage_non_convex_0)_:
++1 InvestmentFlowBlock_total(electricityBus_storage_non_convex_0)
+-1 InvestmentFlowBlock_invest(electricityBus_storage_non_convex_0)
+= 0
+
+c_u_InvestmentFlowBlock_max(storage_non_convex_electricityBus_0_0)_:
++1 flow(storage_non_convex_electricityBus_0_0)
+-1 InvestmentFlowBlock_total(storage_non_convex_electricityBus_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(electricityBus_storagenon_convex_1)_:
--1 InvestmentFlowBlock_invest(electricityBus_storagenon_convex)
-+1 flow(electricityBus_storagenon_convex_1)
+c_u_InvestmentFlowBlock_max(storage_non_convex_electricityBus_0_1)_:
++1 flow(storage_non_convex_electricityBus_0_1)
+-1 InvestmentFlowBlock_total(storage_non_convex_electricityBus_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(electricityBus_storagenon_convex_2)_:
--1 InvestmentFlowBlock_invest(electricityBus_storagenon_convex)
-+1 flow(electricityBus_storagenon_convex_2)
+c_u_InvestmentFlowBlock_max(storage_non_convex_electricityBus_0_2)_:
++1 flow(storage_non_convex_electricityBus_0_2)
+-1 InvestmentFlowBlock_total(storage_non_convex_electricityBus_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(storagenon_convex_electricityBus_0)_:
--1 InvestmentFlowBlock_invest(storagenon_convex_electricityBus)
-+1 flow(storagenon_convex_electricityBus_0)
+c_u_InvestmentFlowBlock_max(electricityBus_storage_non_convex_0_0)_:
++1 flow(electricityBus_storage_non_convex_0_0)
+-1 InvestmentFlowBlock_total(electricityBus_storage_non_convex_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(storagenon_convex_electricityBus_1)_:
--1 InvestmentFlowBlock_invest(storagenon_convex_electricityBus)
-+1 flow(storagenon_convex_electricityBus_1)
+c_u_InvestmentFlowBlock_max(electricityBus_storage_non_convex_0_1)_:
++1 flow(electricityBus_storage_non_convex_0_1)
+-1 InvestmentFlowBlock_total(electricityBus_storage_non_convex_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(storagenon_convex_electricityBus_2)_:
--1 InvestmentFlowBlock_invest(storagenon_convex_electricityBus)
-+1 flow(storagenon_convex_electricityBus_2)
+c_u_InvestmentFlowBlock_max(electricityBus_storage_non_convex_0_2)_:
++1 flow(electricityBus_storage_non_convex_0_2)
+-1 InvestmentFlowBlock_total(electricityBus_storage_non_convex_0)
 <= 0
 
-c_u_GenericInvestmentStorageBlock_init_content_limit(storagenon_convex)_:
-+1 GenericInvestmentStorageBlock_init_content(storagenon_convex)
--1 GenericInvestmentStorageBlock_invest(storagenon_convex)
+c_e_GenericInvestmentStorageBlock_total_storage_rule(storage_non_convex_0)_:
+-1 GenericInvestmentStorageBlock_invest(storage_non_convex_0)
++1 GenericInvestmentStorageBlock_total(storage_non_convex_0)
+= 0
+
+c_u_GenericInvestmentStorageBlock_init_content_limit(storage_non_convex)_:
+-1 GenericInvestmentStorageBlock_invest(storage_non_convex_0)
++1 GenericInvestmentStorageBlock_init_content(storage_non_convex)
 <= 0
 
-c_e_GenericInvestmentStorageBlock_balance_first(storagenon_convex)_:
--0.87 GenericInvestmentStorageBlock_init_content(storagenon_convex)
-+1 GenericInvestmentStorageBlock_storage_content(storagenon_convex_0)
--0.96999999999999997 flow(electricityBus_storagenon_convex_0)
-+1.1627906976744187 flow(storagenon_convex_electricityBus_0)
+c_e_GenericInvestmentStorageBlock_balance_first(storage_non_convex)_:
+-0.97 flow(electricityBus_storage_non_convex_0_0)
++1.1627906976744187 flow(storage_non_convex_electricityBus_0_0)
+-0.87 GenericInvestmentStorageBlock_init_content(storage_non_convex)
++1 GenericInvestmentStorageBlock_storage_content(storage_non_convex_0)
 = 0
 
-c_e_GenericInvestmentStorageBlock_balance(storagenon_convex_1)_:
--0.87 GenericInvestmentStorageBlock_storage_content(storagenon_convex_0)
-+1 GenericInvestmentStorageBlock_storage_content(storagenon_convex_1)
--0.96999999999999997 flow(electricityBus_storagenon_convex_1)
-+1.1627906976744187 flow(storagenon_convex_electricityBus_1)
+c_e_GenericInvestmentStorageBlock_balance(storage_non_convex_0_1)_:
+-0.97 flow(electricityBus_storage_non_convex_0_1)
++1.1627906976744187 flow(storage_non_convex_electricityBus_0_1)
+-0.87 GenericInvestmentStorageBlock_storage_content(storage_non_convex_0)
++1 GenericInvestmentStorageBlock_storage_content(storage_non_convex_1)
 = 0
 
-c_e_GenericInvestmentStorageBlock_balance(storagenon_convex_2)_:
--0.87 GenericInvestmentStorageBlock_storage_content(storagenon_convex_1)
-+1 GenericInvestmentStorageBlock_storage_content(storagenon_convex_2)
--0.96999999999999997 flow(electricityBus_storagenon_convex_2)
-+1.1627906976744187 flow(storagenon_convex_electricityBus_2)
+c_e_GenericInvestmentStorageBlock_balance(storage_non_convex_0_2)_:
+-0.97 flow(electricityBus_storage_non_convex_0_2)
++1.1627906976744187 flow(storage_non_convex_electricityBus_0_2)
+-0.87 GenericInvestmentStorageBlock_storage_content(storage_non_convex_1)
++1 GenericInvestmentStorageBlock_storage_content(storage_non_convex_2)
 = 0
 
-c_e_GenericInvestmentStorageBlock_balanced_cstr(storagenon_convex)_:
--1 GenericInvestmentStorageBlock_init_content(storagenon_convex)
-+1 GenericInvestmentStorageBlock_storage_content(storagenon_convex_2)
+c_e_GenericInvestmentStorageBlock_balanced_cstr(storage_non_convex)_:
+-1 GenericInvestmentStorageBlock_init_content(storage_non_convex)
++1 GenericInvestmentStorageBlock_storage_content(storage_non_convex_2)
 = 0
 
-c_e_GenericInvestmentStorageBlock_storage_capacity_inflow(storagenon_convex)_:
--0.16666666666666666 GenericInvestmentStorageBlock_invest(storagenon_convex)
-+1 InvestmentFlowBlock_invest(electricityBus_storagenon_convex)
+c_e_GenericInvestmentStorageBlock_storage_capacity_inflow(storage_non_convex_0)_:
++1 InvestmentFlowBlock_total(electricityBus_storage_non_convex_0)
+-0.16666666666666666 GenericInvestmentStorageBlock_total(storage_non_convex_0)
 = 0
 
-c_e_GenericInvestmentStorageBlock_storage_capacity_outflow(storagenon_convex)_:
--0.16666666666666666 GenericInvestmentStorageBlock_invest(storagenon_convex)
-+1 InvestmentFlowBlock_invest(storagenon_convex_electricityBus)
+c_e_GenericInvestmentStorageBlock_storage_capacity_outflow(storage_non_convex_0)_:
++1 InvestmentFlowBlock_total(storage_non_convex_electricityBus_0)
+-0.16666666666666666 GenericInvestmentStorageBlock_total(storage_non_convex_0)
 = 0
 
-c_u_GenericInvestmentStorageBlock_max_storage_content(storagenon_convex_0)_:
--0.90000000000000002 GenericInvestmentStorageBlock_invest(storagenon_convex)
-+1 GenericInvestmentStorageBlock_storage_content(storagenon_convex_0)
+c_u_GenericInvestmentStorageBlock_max_storage_content(storage_non_convex_0_0)_:
+-0.9 GenericInvestmentStorageBlock_total(storage_non_convex_0)
++1 GenericInvestmentStorageBlock_storage_content(storage_non_convex_0)
 <= 0
 
-c_u_GenericInvestmentStorageBlock_max_storage_content(storagenon_convex_1)_:
--0.90000000000000002 GenericInvestmentStorageBlock_invest(storagenon_convex)
-+1 GenericInvestmentStorageBlock_storage_content(storagenon_convex_1)
+c_u_GenericInvestmentStorageBlock_max_storage_content(storage_non_convex_0_1)_:
+-0.9 GenericInvestmentStorageBlock_total(storage_non_convex_0)
++1 GenericInvestmentStorageBlock_storage_content(storage_non_convex_1)
 <= 0
 
-c_u_GenericInvestmentStorageBlock_max_storage_content(storagenon_convex_2)_:
--0.90000000000000002 GenericInvestmentStorageBlock_invest(storagenon_convex)
-+1 GenericInvestmentStorageBlock_storage_content(storagenon_convex_2)
+c_u_GenericInvestmentStorageBlock_max_storage_content(storage_non_convex_0_2)_:
+-0.9 GenericInvestmentStorageBlock_total(storage_non_convex_0)
++1 GenericInvestmentStorageBlock_storage_content(storage_non_convex_2)
 <= 0
 
-c_u_GenericInvestmentStorageBlock_min_storage_content(storagenon_convex_0)_:
-+0.10000000000000001 GenericInvestmentStorageBlock_invest(storagenon_convex)
--1 GenericInvestmentStorageBlock_storage_content(storagenon_convex_0)
+c_u_GenericInvestmentStorageBlock_min_storage_content(storage_non_convex_0_0)_:
++0.1 GenericInvestmentStorageBlock_total(storage_non_convex_0)
+-1 GenericInvestmentStorageBlock_storage_content(storage_non_convex_0)
 <= 0
 
-c_u_GenericInvestmentStorageBlock_min_storage_content(storagenon_convex_1)_:
-+0.10000000000000001 GenericInvestmentStorageBlock_invest(storagenon_convex)
--1 GenericInvestmentStorageBlock_storage_content(storagenon_convex_1)
+c_u_GenericInvestmentStorageBlock_min_storage_content(storage_non_convex_0_1)_:
++0.1 GenericInvestmentStorageBlock_total(storage_non_convex_0)
+-1 GenericInvestmentStorageBlock_storage_content(storage_non_convex_1)
 <= 0
 
-c_u_GenericInvestmentStorageBlock_min_storage_content(storagenon_convex_2)_:
-+0.10000000000000001 GenericInvestmentStorageBlock_invest(storagenon_convex)
--1 GenericInvestmentStorageBlock_storage_content(storagenon_convex_2)
+c_u_GenericInvestmentStorageBlock_min_storage_content(storage_non_convex_0_2)_:
++0.1 GenericInvestmentStorageBlock_total(storage_non_convex_0)
+-1 GenericInvestmentStorageBlock_storage_content(storage_non_convex_2)
 <= 0
 
-c_l_GenericInvestmentStorageBlock_limit_max(storagenon_convex)_:
--1 GenericInvestmentStorageBlock_invest(storagenon_convex)
-+1454 GenericInvestmentStorageBlock_invest_status(storagenon_convex)
+c_l_GenericInvestmentStorageBlock_limit_max(storage_non_convex_0)_:
+-1 GenericInvestmentStorageBlock_invest(storage_non_convex_0)
++244 GenericInvestmentStorageBlock_invest_status(storage_non_convex_0)
 >= 0
 
-c_l_GenericInvestmentStorageBlock_limit_min(storagenon_convex)_:
-+1 GenericInvestmentStorageBlock_invest(storagenon_convex)
--19 GenericInvestmentStorageBlock_invest_status(storagenon_convex)
+c_l_GenericInvestmentStorageBlock_limit_min(storage_non_convex_0)_:
++1 GenericInvestmentStorageBlock_invest(storage_non_convex_0)
+-12 GenericInvestmentStorageBlock_invest_status(storage_non_convex_0)
 >= 0
 
-c_e_ONE_VAR_CONSTANT:
-ONE_VAR_CONSTANT = 1.0
-
 bounds
-   0 <= flow(electricityBus_storagenon_convex_0) <= +inf
-   0 <= flow(electricityBus_storagenon_convex_1) <= +inf
-   0 <= flow(electricityBus_storagenon_convex_2) <= +inf
-   0 <= flow(storagenon_convex_electricityBus_0) <= +inf
-   0 <= flow(storagenon_convex_electricityBus_1) <= +inf
-   0 <= flow(storagenon_convex_electricityBus_2) <= +inf
-   0 <= InvestmentFlowBlock_invest(electricityBus_storagenon_convex) <= +inf
-   0 <= InvestmentFlowBlock_invest(storagenon_convex_electricityBus) <= +inf
-   0 <= GenericInvestmentStorageBlock_storage_content(storagenon_convex_0) <= +inf
-   0 <= GenericInvestmentStorageBlock_storage_content(storagenon_convex_1) <= +inf
-   0 <= GenericInvestmentStorageBlock_storage_content(storagenon_convex_2) <= +inf
-   0 <= GenericInvestmentStorageBlock_invest(storagenon_convex) <= 1454
-   0 <= GenericInvestmentStorageBlock_init_content(storagenon_convex) <= +inf
-   0 <= GenericInvestmentStorageBlock_invest_status(storagenon_convex) <= 1
+   0 <= flow(electricityBus_storage_non_convex_0_0) <= +inf
+   0 <= flow(electricityBus_storage_non_convex_0_1) <= +inf
+   0 <= flow(electricityBus_storage_non_convex_0_2) <= +inf
+   0 <= flow(storage_non_convex_electricityBus_0_0) <= +inf
+   0 <= flow(storage_non_convex_electricityBus_0_1) <= +inf
+   0 <= flow(storage_non_convex_electricityBus_0_2) <= +inf
+   0 <= GenericInvestmentStorageBlock_invest(storage_non_convex_0) <= 244
+   0 <= InvestmentFlowBlock_total(storage_non_convex_electricityBus_0) <= +inf
+   0 <= InvestmentFlowBlock_invest(storage_non_convex_electricityBus_0) <= +inf
+   0 <= InvestmentFlowBlock_total(electricityBus_storage_non_convex_0) <= +inf
+   0 <= InvestmentFlowBlock_invest(electricityBus_storage_non_convex_0) <= +inf
+   0 <= GenericInvestmentStorageBlock_total(storage_non_convex_0) <= +inf
+   0 <= GenericInvestmentStorageBlock_init_content(storage_non_convex) <= +inf
+   0 <= GenericInvestmentStorageBlock_storage_content(storage_non_convex_0) <= +inf
+   0 <= GenericInvestmentStorageBlock_storage_content(storage_non_convex_1) <= +inf
+   0 <= GenericInvestmentStorageBlock_storage_content(storage_non_convex_2) <= +inf
+   0 <= GenericInvestmentStorageBlock_invest_status(storage_non_convex_0) <= 1
 binary
-  GenericInvestmentStorageBlock_invest_status(storagenon_convex)
+  GenericInvestmentStorageBlock_invest_status(storage_non_convex_0)
 end
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/storage_invest_without_offset.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/storage_invest_with_offset.lp`

 * *Files 12% similar despite different names*

```diff
@@ -1,161 +1,177 @@
 \* Source Pyomo model name=Model *\
 
-min
+min 
 objective:
-+141 GenericInvestmentStorageBlock_invest(storage_non_convex)
-+56 flow(electricityBus_storage_non_convex_0)
-+56 flow(electricityBus_storage_non_convex_1)
-+56 flow(electricityBus_storage_non_convex_2)
-+24 flow(storage_non_convex_electricityBus_0)
-+24 flow(storage_non_convex_electricityBus_1)
-+24 flow(storage_non_convex_electricityBus_2)
++56 flow(electricityBus_storage_non_convex_0_0)
++56 flow(electricityBus_storage_non_convex_0_1)
++56 flow(electricityBus_storage_non_convex_0_2)
++24 flow(storage_non_convex_electricityBus_0_0)
++24 flow(storage_non_convex_electricityBus_0_1)
++24 flow(storage_non_convex_electricityBus_0_2)
++145 GenericInvestmentStorageBlock_invest(storage_non_convex_0)
++5 GenericInvestmentStorageBlock_invest_status(storage_non_convex_0)
 
 s.t.
 
-c_e_BusBlock_balance(electricityBus_0)_:
--1 flow(electricityBus_storage_non_convex_0)
-+1 flow(storage_non_convex_electricityBus_0)
+c_e_BusBlock_balance(electricityBus_0_0)_:
+-1 flow(electricityBus_storage_non_convex_0_0)
++1 flow(storage_non_convex_electricityBus_0_0)
 = 0
 
-c_e_BusBlock_balance(electricityBus_1)_:
--1 flow(electricityBus_storage_non_convex_1)
-+1 flow(storage_non_convex_electricityBus_1)
+c_e_BusBlock_balance(electricityBus_0_1)_:
+-1 flow(electricityBus_storage_non_convex_0_1)
++1 flow(storage_non_convex_electricityBus_0_1)
 = 0
 
-c_e_BusBlock_balance(electricityBus_2)_:
--1 flow(electricityBus_storage_non_convex_2)
-+1 flow(storage_non_convex_electricityBus_2)
+c_e_BusBlock_balance(electricityBus_0_2)_:
+-1 flow(electricityBus_storage_non_convex_0_2)
++1 flow(storage_non_convex_electricityBus_0_2)
 = 0
 
-c_u_InvestmentFlowBlock_max(electricityBus_storage_non_convex_0)_:
--1 InvestmentFlowBlock_invest(electricityBus_storage_non_convex)
-+1 flow(electricityBus_storage_non_convex_0)
+c_e_InvestmentFlowBlock_total_rule(storage_non_convex_electricityBus_0)_:
++1 InvestmentFlowBlock_total(storage_non_convex_electricityBus_0)
+-1 InvestmentFlowBlock_invest(storage_non_convex_electricityBus_0)
+= 0
+
+c_e_InvestmentFlowBlock_total_rule(electricityBus_storage_non_convex_0)_:
++1 InvestmentFlowBlock_total(electricityBus_storage_non_convex_0)
+-1 InvestmentFlowBlock_invest(electricityBus_storage_non_convex_0)
+= 0
+
+c_u_InvestmentFlowBlock_max(storage_non_convex_electricityBus_0_0)_:
++1 flow(storage_non_convex_electricityBus_0_0)
+-1 InvestmentFlowBlock_total(storage_non_convex_electricityBus_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(electricityBus_storage_non_convex_1)_:
--1 InvestmentFlowBlock_invest(electricityBus_storage_non_convex)
-+1 flow(electricityBus_storage_non_convex_1)
+c_u_InvestmentFlowBlock_max(storage_non_convex_electricityBus_0_1)_:
++1 flow(storage_non_convex_electricityBus_0_1)
+-1 InvestmentFlowBlock_total(storage_non_convex_electricityBus_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(electricityBus_storage_non_convex_2)_:
--1 InvestmentFlowBlock_invest(electricityBus_storage_non_convex)
-+1 flow(electricityBus_storage_non_convex_2)
+c_u_InvestmentFlowBlock_max(storage_non_convex_electricityBus_0_2)_:
++1 flow(storage_non_convex_electricityBus_0_2)
+-1 InvestmentFlowBlock_total(storage_non_convex_electricityBus_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(storage_non_convex_electricityBus_0)_:
--1 InvestmentFlowBlock_invest(storage_non_convex_electricityBus)
-+1 flow(storage_non_convex_electricityBus_0)
+c_u_InvestmentFlowBlock_max(electricityBus_storage_non_convex_0_0)_:
++1 flow(electricityBus_storage_non_convex_0_0)
+-1 InvestmentFlowBlock_total(electricityBus_storage_non_convex_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(storage_non_convex_electricityBus_1)_:
--1 InvestmentFlowBlock_invest(storage_non_convex_electricityBus)
-+1 flow(storage_non_convex_electricityBus_1)
+c_u_InvestmentFlowBlock_max(electricityBus_storage_non_convex_0_1)_:
++1 flow(electricityBus_storage_non_convex_0_1)
+-1 InvestmentFlowBlock_total(electricityBus_storage_non_convex_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(storage_non_convex_electricityBus_2)_:
--1 InvestmentFlowBlock_invest(storage_non_convex_electricityBus)
-+1 flow(storage_non_convex_electricityBus_2)
+c_u_InvestmentFlowBlock_max(electricityBus_storage_non_convex_0_2)_:
++1 flow(electricityBus_storage_non_convex_0_2)
+-1 InvestmentFlowBlock_total(electricityBus_storage_non_convex_0)
 <= 0
 
+c_e_GenericInvestmentStorageBlock_total_storage_rule(storage_non_convex_0)_:
+-1 GenericInvestmentStorageBlock_invest(storage_non_convex_0)
++1 GenericInvestmentStorageBlock_total(storage_non_convex_0)
+= 0
+
 c_u_GenericInvestmentStorageBlock_init_content_limit(storage_non_convex)_:
+-1 GenericInvestmentStorageBlock_invest(storage_non_convex_0)
 +1 GenericInvestmentStorageBlock_init_content(storage_non_convex)
--1 GenericInvestmentStorageBlock_invest(storage_non_convex)
 <= 0
 
 c_e_GenericInvestmentStorageBlock_balance_first(storage_non_convex)_:
+-0.97 flow(electricityBus_storage_non_convex_0_0)
++1.1627906976744187 flow(storage_non_convex_electricityBus_0_0)
 -0.87 GenericInvestmentStorageBlock_init_content(storage_non_convex)
 +1 GenericInvestmentStorageBlock_storage_content(storage_non_convex_0)
--0.96999999999999997 flow(electricityBus_storage_non_convex_0)
-+1.1627906976744187 flow(storage_non_convex_electricityBus_0)
 = 0
 
-c_e_GenericInvestmentStorageBlock_balance(storage_non_convex_1)_:
+c_e_GenericInvestmentStorageBlock_balance(storage_non_convex_0_1)_:
+-0.97 flow(electricityBus_storage_non_convex_0_1)
++1.1627906976744187 flow(storage_non_convex_electricityBus_0_1)
 -0.87 GenericInvestmentStorageBlock_storage_content(storage_non_convex_0)
 +1 GenericInvestmentStorageBlock_storage_content(storage_non_convex_1)
--0.96999999999999997 flow(electricityBus_storage_non_convex_1)
-+1.1627906976744187 flow(storage_non_convex_electricityBus_1)
 = 0
 
-c_e_GenericInvestmentStorageBlock_balance(storage_non_convex_2)_:
+c_e_GenericInvestmentStorageBlock_balance(storage_non_convex_0_2)_:
+-0.97 flow(electricityBus_storage_non_convex_0_2)
++1.1627906976744187 flow(storage_non_convex_electricityBus_0_2)
 -0.87 GenericInvestmentStorageBlock_storage_content(storage_non_convex_1)
 +1 GenericInvestmentStorageBlock_storage_content(storage_non_convex_2)
--0.96999999999999997 flow(electricityBus_storage_non_convex_2)
-+1.1627906976744187 flow(storage_non_convex_electricityBus_2)
 = 0
 
 c_e_GenericInvestmentStorageBlock_balanced_cstr(storage_non_convex)_:
 -1 GenericInvestmentStorageBlock_init_content(storage_non_convex)
 +1 GenericInvestmentStorageBlock_storage_content(storage_non_convex_2)
 = 0
 
-c_e_GenericInvestmentStorageBlock_storage_capacity_inflow(storage_non_convex)_:
--0.16666666666666666 GenericInvestmentStorageBlock_invest(storage_non_convex)
-+1 InvestmentFlowBlock_invest(electricityBus_storage_non_convex)
+c_e_GenericInvestmentStorageBlock_storage_capacity_inflow(storage_non_convex_0)_:
++1 InvestmentFlowBlock_total(electricityBus_storage_non_convex_0)
+-0.16666666666666666 GenericInvestmentStorageBlock_total(storage_non_convex_0)
 = 0
 
-c_e_GenericInvestmentStorageBlock_storage_capacity_outflow(storage_non_convex)_:
--0.16666666666666666 GenericInvestmentStorageBlock_invest(storage_non_convex)
-+1 InvestmentFlowBlock_invest(storage_non_convex_electricityBus)
+c_e_GenericInvestmentStorageBlock_storage_capacity_outflow(storage_non_convex_0)_:
++1 InvestmentFlowBlock_total(storage_non_convex_electricityBus_0)
+-0.16666666666666666 GenericInvestmentStorageBlock_total(storage_non_convex_0)
 = 0
 
-c_u_GenericInvestmentStorageBlock_max_storage_content(storage_non_convex_0)_:
--0.90000000000000002 GenericInvestmentStorageBlock_invest(storage_non_convex)
+c_u_GenericInvestmentStorageBlock_max_storage_content(storage_non_convex_0_0)_:
+-0.9 GenericInvestmentStorageBlock_total(storage_non_convex_0)
 +1 GenericInvestmentStorageBlock_storage_content(storage_non_convex_0)
 <= 0
 
-c_u_GenericInvestmentStorageBlock_max_storage_content(storage_non_convex_1)_:
--0.90000000000000002 GenericInvestmentStorageBlock_invest(storage_non_convex)
+c_u_GenericInvestmentStorageBlock_max_storage_content(storage_non_convex_0_1)_:
+-0.9 GenericInvestmentStorageBlock_total(storage_non_convex_0)
 +1 GenericInvestmentStorageBlock_storage_content(storage_non_convex_1)
 <= 0
 
-c_u_GenericInvestmentStorageBlock_max_storage_content(storage_non_convex_2)_:
--0.90000000000000002 GenericInvestmentStorageBlock_invest(storage_non_convex)
+c_u_GenericInvestmentStorageBlock_max_storage_content(storage_non_convex_0_2)_:
+-0.9 GenericInvestmentStorageBlock_total(storage_non_convex_0)
 +1 GenericInvestmentStorageBlock_storage_content(storage_non_convex_2)
 <= 0
 
-c_u_GenericInvestmentStorageBlock_min_storage_content(storage_non_convex_0)_:
-+0.10000000000000001 GenericInvestmentStorageBlock_invest(storage_non_convex)
+c_u_GenericInvestmentStorageBlock_min_storage_content(storage_non_convex_0_0)_:
++0.1 GenericInvestmentStorageBlock_total(storage_non_convex_0)
 -1 GenericInvestmentStorageBlock_storage_content(storage_non_convex_0)
 <= 0
 
-c_u_GenericInvestmentStorageBlock_min_storage_content(storage_non_convex_1)_:
-+0.10000000000000001 GenericInvestmentStorageBlock_invest(storage_non_convex)
+c_u_GenericInvestmentStorageBlock_min_storage_content(storage_non_convex_0_1)_:
++0.1 GenericInvestmentStorageBlock_total(storage_non_convex_0)
 -1 GenericInvestmentStorageBlock_storage_content(storage_non_convex_1)
 <= 0
 
-c_u_GenericInvestmentStorageBlock_min_storage_content(storage_non_convex_2)_:
-+0.10000000000000001 GenericInvestmentStorageBlock_invest(storage_non_convex)
+c_u_GenericInvestmentStorageBlock_min_storage_content(storage_non_convex_0_2)_:
++0.1 GenericInvestmentStorageBlock_total(storage_non_convex_0)
 -1 GenericInvestmentStorageBlock_storage_content(storage_non_convex_2)
 <= 0
 
-c_l_GenericInvestmentStorageBlock_limit_max(storage_non_convex)_:
--1 GenericInvestmentStorageBlock_invest(storage_non_convex)
-+244 GenericInvestmentStorageBlock_invest_status(storage_non_convex)
+c_l_GenericInvestmentStorageBlock_limit_max(storage_non_convex_0)_:
+-1 GenericInvestmentStorageBlock_invest(storage_non_convex_0)
++1454 GenericInvestmentStorageBlock_invest_status(storage_non_convex_0)
 >= 0
 
-c_l_GenericInvestmentStorageBlock_limit_min(storage_non_convex)_:
-+1 GenericInvestmentStorageBlock_invest(storage_non_convex)
--12 GenericInvestmentStorageBlock_invest_status(storage_non_convex)
+c_l_GenericInvestmentStorageBlock_limit_min(storage_non_convex_0)_:
++1 GenericInvestmentStorageBlock_invest(storage_non_convex_0)
+-19 GenericInvestmentStorageBlock_invest_status(storage_non_convex_0)
 >= 0
 
-c_e_ONE_VAR_CONSTANT:
-ONE_VAR_CONSTANT = 1.0
-
 bounds
-   0 <= flow(electricityBus_storage_non_convex_0) <= +inf
-   0 <= flow(electricityBus_storage_non_convex_1) <= +inf
-   0 <= flow(electricityBus_storage_non_convex_2) <= +inf
-   0 <= flow(storage_non_convex_electricityBus_0) <= +inf
-   0 <= flow(storage_non_convex_electricityBus_1) <= +inf
-   0 <= flow(storage_non_convex_electricityBus_2) <= +inf
-   0 <= InvestmentFlowBlock_invest(electricityBus_storage_non_convex) <= +inf
-   0 <= InvestmentFlowBlock_invest(storage_non_convex_electricityBus) <= +inf
+   0 <= flow(electricityBus_storage_non_convex_0_0) <= +inf
+   0 <= flow(electricityBus_storage_non_convex_0_1) <= +inf
+   0 <= flow(electricityBus_storage_non_convex_0_2) <= +inf
+   0 <= flow(storage_non_convex_electricityBus_0_0) <= +inf
+   0 <= flow(storage_non_convex_electricityBus_0_1) <= +inf
+   0 <= flow(storage_non_convex_electricityBus_0_2) <= +inf
+   0 <= GenericInvestmentStorageBlock_invest(storage_non_convex_0) <= 1454
+   0 <= GenericInvestmentStorageBlock_invest_status(storage_non_convex_0) <= 1
+   0 <= InvestmentFlowBlock_total(storage_non_convex_electricityBus_0) <= +inf
+   0 <= InvestmentFlowBlock_invest(storage_non_convex_electricityBus_0) <= +inf
+   0 <= InvestmentFlowBlock_total(electricityBus_storage_non_convex_0) <= +inf
+   0 <= InvestmentFlowBlock_invest(electricityBus_storage_non_convex_0) <= +inf
+   0 <= GenericInvestmentStorageBlock_total(storage_non_convex_0) <= +inf
+   0 <= GenericInvestmentStorageBlock_init_content(storage_non_convex) <= +inf
    0 <= GenericInvestmentStorageBlock_storage_content(storage_non_convex_0) <= +inf
    0 <= GenericInvestmentStorageBlock_storage_content(storage_non_convex_1) <= +inf
    0 <= GenericInvestmentStorageBlock_storage_content(storage_non_convex_2) <= +inf
-   0 <= GenericInvestmentStorageBlock_invest(storage_non_convex) <= 244
-   0 <= GenericInvestmentStorageBlock_init_content(storage_non_convex) <= +inf
-   0 <= GenericInvestmentStorageBlock_invest_status(storage_non_convex) <= 1
 binary
-  GenericInvestmentStorageBlock_invest_status(storage_non_convex)
+  GenericInvestmentStorageBlock_invest_status(storage_non_convex_0)
 end
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/storage_unbalanced.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/storage_unbalanced.lp`

 * *Files 21% similar despite different names*

```diff
@@ -2,58 +2,56 @@
 
 min 
 objective:
 +0 ONE_VAR_CONSTANT
 
 s.t.
 
-c_e_BusBlock_balance(electricityBus_0)_:
--1 flow(electricityBus_storage1_0)
-+1 flow(storage1_electricityBus_0)
+c_e_BusBlock_balance(electricityBus_0_0)_:
++1 flow(storage1_electricityBus_0_0)
+-1 flow(electricityBus_storage1_0_0)
 = 0
 
-c_e_BusBlock_balance(electricityBus_1)_:
--1 flow(electricityBus_storage1_1)
-+1 flow(storage1_electricityBus_1)
+c_e_BusBlock_balance(electricityBus_0_1)_:
++1 flow(storage1_electricityBus_0_1)
+-1 flow(electricityBus_storage1_0_1)
 = 0
 
-c_e_BusBlock_balance(electricityBus_2)_:
--1 flow(electricityBus_storage1_2)
-+1 flow(storage1_electricityBus_2)
+c_e_BusBlock_balance(electricityBus_0_2)_:
++1 flow(storage1_electricityBus_0_2)
+-1 flow(electricityBus_storage1_0_2)
 = 0
 
-c_e_GenericStorageBlock_balance(storage1_0)_:
--1 GenericStorageBlock_storage_content(storage1_0)
+c_e_GenericStorageBlock_balance(storage1_0_0)_:
++1 flow(storage1_electricityBus_0_0)
+-1 flow(electricityBus_storage1_0_0)
 +1 GenericStorageBlock_storage_content(storage1_1)
--1 flow(electricityBus_storage1_0)
-+1 flow(storage1_electricityBus_0)
+-1 GenericStorageBlock_storage_content(storage1_0)
 = 0
 
-c_e_GenericStorageBlock_balance(storage1_1)_:
+c_e_GenericStorageBlock_balance(storage1_0_1)_:
++1 flow(storage1_electricityBus_0_1)
+-1 flow(electricityBus_storage1_0_1)
 -1 GenericStorageBlock_storage_content(storage1_1)
 +1 GenericStorageBlock_storage_content(storage1_2)
--1 flow(electricityBus_storage1_1)
-+1 flow(storage1_electricityBus_1)
 = 0
 
-c_e_GenericStorageBlock_balance(storage1_2)_:
+c_e_GenericStorageBlock_balance(storage1_0_2)_:
++1 flow(storage1_electricityBus_0_2)
+-1 flow(electricityBus_storage1_0_2)
 -1 GenericStorageBlock_storage_content(storage1_2)
 +1 GenericStorageBlock_storage_content(storage1_3)
--1 flow(electricityBus_storage1_2)
-+1 flow(storage1_electricityBus_2)
 = 0
 
-c_e_ONE_VAR_CONSTANT: 
-ONE_VAR_CONSTANT = 1.0
-
 bounds
-   0 <= flow(electricityBus_storage1_0) <= +inf
-   0 <= flow(electricityBus_storage1_1) <= +inf
-   0 <= flow(electricityBus_storage1_2) <= +inf
-   0 <= flow(storage1_electricityBus_0) <= +inf
-   0 <= flow(storage1_electricityBus_1) <= +inf
-   0 <= flow(storage1_electricityBus_2) <= +inf
-   0 <= GenericStorageBlock_storage_content(storage1_0) <= 1111
+   1 <= ONE_VAR_CONSTANT <= 1
+   0 <= flow(storage1_electricityBus_0_0) <= +inf
+   0 <= flow(electricityBus_storage1_0_0) <= +inf
+   0 <= flow(storage1_electricityBus_0_1) <= +inf
+   0 <= flow(electricityBus_storage1_0_1) <= +inf
+   0 <= flow(storage1_electricityBus_0_2) <= +inf
+   0 <= flow(electricityBus_storage1_0_2) <= +inf
    0 <= GenericStorageBlock_storage_content(storage1_1) <= 1111
+   0 <= GenericStorageBlock_storage_content(storage1_0) <= 1111
    0 <= GenericStorageBlock_storage_content(storage1_2) <= 1111
    0 <= GenericStorageBlock_storage_content(storage1_3) <= 1111
 end
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/transformer_invest.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/transformer_invest.lp`

 * *Files 24% similar despite different names*

```diff
@@ -1,155 +1,158 @@
 \* Source Pyomo model name=Model *\
 
-min
+min 
 objective:
-+20 InvestmentFlowBlock_invest(powerplant_gas_coal_electricityBus)
-+50 flow(powerplant_gas_coal_electricityBus_0)
-+50 flow(powerplant_gas_coal_electricityBus_1)
-+50 flow(powerplant_gas_coal_electricityBus_2)
-+20 flow(powerplant_gas_coal_thermalBus_0)
-+20 flow(powerplant_gas_coal_thermalBus_1)
-+20 flow(powerplant_gas_coal_thermalBus_2)
++20 InvestmentFlowBlock_invest(powerplant_gas_coal_electricityBus_0)
++50 flow(powerplant_gas_coal_electricityBus_0_0)
++50 flow(powerplant_gas_coal_electricityBus_0_1)
++50 flow(powerplant_gas_coal_electricityBus_0_2)
++20 flow(powerplant_gas_coal_thermalBus_0_0)
++20 flow(powerplant_gas_coal_thermalBus_0_1)
++20 flow(powerplant_gas_coal_thermalBus_0_2)
 
 s.t.
 
-c_e_BusBlock_balance(coalBus_0)_:
-+1 flow(coalBus_powerplant_gas_coal_0)
+c_e_BusBlock_balance(coalBus_0_0)_:
++1 flow(coalBus_powerplant_gas_coal_0_0)
 = 0
 
-c_e_BusBlock_balance(coalBus_1)_:
-+1 flow(coalBus_powerplant_gas_coal_1)
+c_e_BusBlock_balance(coalBus_0_1)_:
++1 flow(coalBus_powerplant_gas_coal_0_1)
 = 0
 
-c_e_BusBlock_balance(coalBus_2)_:
-+1 flow(coalBus_powerplant_gas_coal_2)
+c_e_BusBlock_balance(coalBus_0_2)_:
++1 flow(coalBus_powerplant_gas_coal_0_2)
 = 0
 
-c_e_BusBlock_balance(electricityBus_0)_:
-+1 flow(powerplant_gas_coal_electricityBus_0)
+c_e_BusBlock_balance(gasBus_0_0)_:
++1 flow(gasBus_powerplant_gas_coal_0_0)
 = 0
 
-c_e_BusBlock_balance(electricityBus_1)_:
-+1 flow(powerplant_gas_coal_electricityBus_1)
+c_e_BusBlock_balance(gasBus_0_1)_:
++1 flow(gasBus_powerplant_gas_coal_0_1)
 = 0
 
-c_e_BusBlock_balance(electricityBus_2)_:
-+1 flow(powerplant_gas_coal_electricityBus_2)
+c_e_BusBlock_balance(gasBus_0_2)_:
++1 flow(gasBus_powerplant_gas_coal_0_2)
 = 0
 
-c_e_BusBlock_balance(gasBus_0)_:
-+1 flow(gasBus_powerplant_gas_coal_0)
+c_e_BusBlock_balance(electricityBus_0_0)_:
++1 flow(powerplant_gas_coal_electricityBus_0_0)
 = 0
 
-c_e_BusBlock_balance(gasBus_1)_:
-+1 flow(gasBus_powerplant_gas_coal_1)
+c_e_BusBlock_balance(electricityBus_0_1)_:
++1 flow(powerplant_gas_coal_electricityBus_0_1)
 = 0
 
-c_e_BusBlock_balance(gasBus_2)_:
-+1 flow(gasBus_powerplant_gas_coal_2)
+c_e_BusBlock_balance(electricityBus_0_2)_:
++1 flow(powerplant_gas_coal_electricityBus_0_2)
 = 0
 
-c_e_BusBlock_balance(thermalBus_0)_:
-+1 flow(powerplant_gas_coal_thermalBus_0)
+c_e_BusBlock_balance(thermalBus_0_0)_:
++1 flow(powerplant_gas_coal_thermalBus_0_0)
 = 0
 
-c_e_BusBlock_balance(thermalBus_1)_:
-+1 flow(powerplant_gas_coal_thermalBus_1)
+c_e_BusBlock_balance(thermalBus_0_1)_:
++1 flow(powerplant_gas_coal_thermalBus_0_1)
 = 0
 
-c_e_BusBlock_balance(thermalBus_2)_:
-+1 flow(powerplant_gas_coal_thermalBus_2)
+c_e_BusBlock_balance(thermalBus_0_2)_:
++1 flow(powerplant_gas_coal_thermalBus_0_2)
 = 0
 
-c_e_TransformerBlock_relation(powerplant_gas_coal_coalBus_electricityBus_0)_:
-+0.29999999999999999 flow(coalBus_powerplant_gas_coal_0)
--0.20000000000000001 flow(powerplant_gas_coal_electricityBus_0)
+c_e_TransformerBlock_relation(powerplant_gas_coal_coalBus_electricityBus_0_0)_:
+-0.2 flow(powerplant_gas_coal_electricityBus_0_0)
++0.3 flow(coalBus_powerplant_gas_coal_0_0)
 = 0
 
-c_e_TransformerBlock_relation(powerplant_gas_coal_coalBus_electricityBus_1)_:
-+0.29999999999999999 flow(coalBus_powerplant_gas_coal_1)
--0.20000000000000001 flow(powerplant_gas_coal_electricityBus_1)
+c_e_TransformerBlock_relation(powerplant_gas_coal_gasBus_electricityBus_0_0)_:
+-0.58 flow(powerplant_gas_coal_electricityBus_0_0)
++0.3 flow(gasBus_powerplant_gas_coal_0_0)
 = 0
 
-c_e_TransformerBlock_relation(powerplant_gas_coal_coalBus_electricityBus_2)_:
-+0.29999999999999999 flow(coalBus_powerplant_gas_coal_2)
--0.20000000000000001 flow(powerplant_gas_coal_electricityBus_2)
+c_e_TransformerBlock_relation(powerplant_gas_coal_coalBus_thermalBus_0_0)_:
+-0.2 flow(powerplant_gas_coal_thermalBus_0_0)
++0.5 flow(coalBus_powerplant_gas_coal_0_0)
 = 0
 
-c_e_TransformerBlock_relation(powerplant_gas_coal_coalBus_thermalBus_0)_:
-+0.5 flow(coalBus_powerplant_gas_coal_0)
--0.20000000000000001 flow(powerplant_gas_coal_thermalBus_0)
+c_e_TransformerBlock_relation(powerplant_gas_coal_gasBus_thermalBus_0_0)_:
+-0.58 flow(powerplant_gas_coal_thermalBus_0_0)
++0.5 flow(gasBus_powerplant_gas_coal_0_0)
 = 0
 
-c_e_TransformerBlock_relation(powerplant_gas_coal_coalBus_thermalBus_1)_:
-+0.5 flow(coalBus_powerplant_gas_coal_1)
--0.20000000000000001 flow(powerplant_gas_coal_thermalBus_1)
+c_e_TransformerBlock_relation(powerplant_gas_coal_coalBus_electricityBus_0_1)_:
+-0.2 flow(powerplant_gas_coal_electricityBus_0_1)
++0.3 flow(coalBus_powerplant_gas_coal_0_1)
 = 0
 
-c_e_TransformerBlock_relation(powerplant_gas_coal_coalBus_thermalBus_2)_:
-+0.5 flow(coalBus_powerplant_gas_coal_2)
--0.20000000000000001 flow(powerplant_gas_coal_thermalBus_2)
+c_e_TransformerBlock_relation(powerplant_gas_coal_gasBus_electricityBus_0_1)_:
+-0.58 flow(powerplant_gas_coal_electricityBus_0_1)
++0.3 flow(gasBus_powerplant_gas_coal_0_1)
 = 0
 
-c_e_TransformerBlock_relation(powerplant_gas_coal_gasBus_electricityBus_0)_:
-+0.29999999999999999 flow(gasBus_powerplant_gas_coal_0)
--0.57999999999999996 flow(powerplant_gas_coal_electricityBus_0)
+c_e_TransformerBlock_relation(powerplant_gas_coal_coalBus_thermalBus_0_1)_:
+-0.2 flow(powerplant_gas_coal_thermalBus_0_1)
++0.5 flow(coalBus_powerplant_gas_coal_0_1)
 = 0
 
-c_e_TransformerBlock_relation(powerplant_gas_coal_gasBus_electricityBus_1)_:
-+0.29999999999999999 flow(gasBus_powerplant_gas_coal_1)
--0.57999999999999996 flow(powerplant_gas_coal_electricityBus_1)
+c_e_TransformerBlock_relation(powerplant_gas_coal_gasBus_thermalBus_0_1)_:
+-0.58 flow(powerplant_gas_coal_thermalBus_0_1)
++0.5 flow(gasBus_powerplant_gas_coal_0_1)
 = 0
 
-c_e_TransformerBlock_relation(powerplant_gas_coal_gasBus_electricityBus_2)_:
-+0.29999999999999999 flow(gasBus_powerplant_gas_coal_2)
--0.57999999999999996 flow(powerplant_gas_coal_electricityBus_2)
+c_e_TransformerBlock_relation(powerplant_gas_coal_coalBus_electricityBus_0_2)_:
+-0.2 flow(powerplant_gas_coal_electricityBus_0_2)
++0.3 flow(coalBus_powerplant_gas_coal_0_2)
 = 0
 
-c_e_TransformerBlock_relation(powerplant_gas_coal_gasBus_thermalBus_0)_:
-+0.5 flow(gasBus_powerplant_gas_coal_0)
--0.57999999999999996 flow(powerplant_gas_coal_thermalBus_0)
+c_e_TransformerBlock_relation(powerplant_gas_coal_gasBus_electricityBus_0_2)_:
+-0.58 flow(powerplant_gas_coal_electricityBus_0_2)
++0.3 flow(gasBus_powerplant_gas_coal_0_2)
 = 0
 
-c_e_TransformerBlock_relation(powerplant_gas_coal_gasBus_thermalBus_1)_:
-+0.5 flow(gasBus_powerplant_gas_coal_1)
--0.57999999999999996 flow(powerplant_gas_coal_thermalBus_1)
+c_e_TransformerBlock_relation(powerplant_gas_coal_coalBus_thermalBus_0_2)_:
+-0.2 flow(powerplant_gas_coal_thermalBus_0_2)
++0.5 flow(coalBus_powerplant_gas_coal_0_2)
 = 0
 
-c_e_TransformerBlock_relation(powerplant_gas_coal_gasBus_thermalBus_2)_:
-+0.5 flow(gasBus_powerplant_gas_coal_2)
--0.57999999999999996 flow(powerplant_gas_coal_thermalBus_2)
+c_e_TransformerBlock_relation(powerplant_gas_coal_gasBus_thermalBus_0_2)_:
+-0.58 flow(powerplant_gas_coal_thermalBus_0_2)
++0.5 flow(gasBus_powerplant_gas_coal_0_2)
 = 0
 
-c_u_InvestmentFlowBlock_max(powerplant_gas_coal_electricityBus_0)_:
--1 InvestmentFlowBlock_invest(powerplant_gas_coal_electricityBus)
-+1 flow(powerplant_gas_coal_electricityBus_0)
-<= 0
+c_e_InvestmentFlowBlock_total_rule(powerplant_gas_coal_electricityBus_0)_:
+-1 InvestmentFlowBlock_invest(powerplant_gas_coal_electricityBus_0)
++1 InvestmentFlowBlock_total(powerplant_gas_coal_electricityBus_0)
+= 0
 
-c_u_InvestmentFlowBlock_max(powerplant_gas_coal_electricityBus_1)_:
--1 InvestmentFlowBlock_invest(powerplant_gas_coal_electricityBus)
-+1 flow(powerplant_gas_coal_electricityBus_1)
+c_u_InvestmentFlowBlock_max(powerplant_gas_coal_electricityBus_0_0)_:
++1 flow(powerplant_gas_coal_electricityBus_0_0)
+-1 InvestmentFlowBlock_total(powerplant_gas_coal_electricityBus_0)
 <= 0
 
-c_u_InvestmentFlowBlock_max(powerplant_gas_coal_electricityBus_2)_:
--1 InvestmentFlowBlock_invest(powerplant_gas_coal_electricityBus)
-+1 flow(powerplant_gas_coal_electricityBus_2)
+c_u_InvestmentFlowBlock_max(powerplant_gas_coal_electricityBus_0_1)_:
++1 flow(powerplant_gas_coal_electricityBus_0_1)
+-1 InvestmentFlowBlock_total(powerplant_gas_coal_electricityBus_0)
 <= 0
 
-c_e_ONE_VAR_CONSTANT:
-ONE_VAR_CONSTANT = 1.0
+c_u_InvestmentFlowBlock_max(powerplant_gas_coal_electricityBus_0_2)_:
++1 flow(powerplant_gas_coal_electricityBus_0_2)
+-1 InvestmentFlowBlock_total(powerplant_gas_coal_electricityBus_0)
+<= 0
 
 bounds
-   0 <= flow(coalBus_powerplant_gas_coal_0) <= +inf
-   0 <= flow(coalBus_powerplant_gas_coal_1) <= +inf
-   0 <= flow(coalBus_powerplant_gas_coal_2) <= +inf
-   0 <= flow(gasBus_powerplant_gas_coal_0) <= +inf
-   0 <= flow(gasBus_powerplant_gas_coal_1) <= +inf
-   0 <= flow(gasBus_powerplant_gas_coal_2) <= +inf
-   0 <= flow(powerplant_gas_coal_electricityBus_0) <= +inf
-   0 <= flow(powerplant_gas_coal_electricityBus_1) <= +inf
-   0 <= flow(powerplant_gas_coal_electricityBus_2) <= +inf
-   0 <= flow(powerplant_gas_coal_thermalBus_0) <= +inf
-   0 <= flow(powerplant_gas_coal_thermalBus_1) <= +inf
-   0 <= flow(powerplant_gas_coal_thermalBus_2) <= +inf
-   0 <= InvestmentFlowBlock_invest(powerplant_gas_coal_electricityBus) <= 1000
+   0 <= InvestmentFlowBlock_invest(powerplant_gas_coal_electricityBus_0) <= 1000
+   0 <= flow(powerplant_gas_coal_electricityBus_0_0) <= +inf
+   0 <= flow(powerplant_gas_coal_electricityBus_0_1) <= +inf
+   0 <= flow(powerplant_gas_coal_electricityBus_0_2) <= +inf
+   0 <= flow(powerplant_gas_coal_thermalBus_0_0) <= +inf
+   0 <= flow(powerplant_gas_coal_thermalBus_0_1) <= +inf
+   0 <= flow(powerplant_gas_coal_thermalBus_0_2) <= +inf
+   0 <= flow(coalBus_powerplant_gas_coal_0_0) <= +inf
+   0 <= flow(coalBus_powerplant_gas_coal_0_1) <= +inf
+   0 <= flow(coalBus_powerplant_gas_coal_0_2) <= +inf
+   0 <= flow(gasBus_powerplant_gas_coal_0_0) <= +inf
+   0 <= flow(gasBus_powerplant_gas_coal_0_1) <= +inf
+   0 <= flow(gasBus_powerplant_gas_coal_0_2) <= +inf
+   0 <= InvestmentFlowBlock_total(powerplant_gas_coal_electricityBus_0) <= +inf
 end
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/transformer_invest_with_existing.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/transformer_invest_with_existing.lp`

 * *Files 24% similar despite different names*

```diff
@@ -1,155 +1,158 @@
 \* Source Pyomo model name=Model *\
 
-min
+min 
 objective:
-+20 InvestmentFlowBlock_invest(powerplant_gas_coal_electricityBus)
-+50 flow(powerplant_gas_coal_electricityBus_0)
-+50 flow(powerplant_gas_coal_electricityBus_1)
-+50 flow(powerplant_gas_coal_electricityBus_2)
-+20 flow(powerplant_gas_coal_thermalBus_0)
-+20 flow(powerplant_gas_coal_thermalBus_1)
-+20 flow(powerplant_gas_coal_thermalBus_2)
++20 InvestmentFlowBlock_invest(powerplant_gas_coal_electricityBus_0)
++50 flow(powerplant_gas_coal_electricityBus_0_0)
++50 flow(powerplant_gas_coal_electricityBus_0_1)
++50 flow(powerplant_gas_coal_electricityBus_0_2)
++20 flow(powerplant_gas_coal_thermalBus_0_0)
++20 flow(powerplant_gas_coal_thermalBus_0_1)
++20 flow(powerplant_gas_coal_thermalBus_0_2)
 
 s.t.
 
-c_e_BusBlock_balance(coalBus_0)_:
-+1 flow(coalBus_powerplant_gas_coal_0)
+c_e_BusBlock_balance(coalBus_0_0)_:
++1 flow(coalBus_powerplant_gas_coal_0_0)
 = 0
 
-c_e_BusBlock_balance(coalBus_1)_:
-+1 flow(coalBus_powerplant_gas_coal_1)
+c_e_BusBlock_balance(coalBus_0_1)_:
++1 flow(coalBus_powerplant_gas_coal_0_1)
 = 0
 
-c_e_BusBlock_balance(coalBus_2)_:
-+1 flow(coalBus_powerplant_gas_coal_2)
+c_e_BusBlock_balance(coalBus_0_2)_:
++1 flow(coalBus_powerplant_gas_coal_0_2)
 = 0
 
-c_e_BusBlock_balance(electricityBus_0)_:
-+1 flow(powerplant_gas_coal_electricityBus_0)
+c_e_BusBlock_balance(gasBus_0_0)_:
++1 flow(gasBus_powerplant_gas_coal_0_0)
 = 0
 
-c_e_BusBlock_balance(electricityBus_1)_:
-+1 flow(powerplant_gas_coal_electricityBus_1)
+c_e_BusBlock_balance(gasBus_0_1)_:
++1 flow(gasBus_powerplant_gas_coal_0_1)
 = 0
 
-c_e_BusBlock_balance(electricityBus_2)_:
-+1 flow(powerplant_gas_coal_electricityBus_2)
+c_e_BusBlock_balance(gasBus_0_2)_:
++1 flow(gasBus_powerplant_gas_coal_0_2)
 = 0
 
-c_e_BusBlock_balance(gasBus_0)_:
-+1 flow(gasBus_powerplant_gas_coal_0)
+c_e_BusBlock_balance(electricityBus_0_0)_:
++1 flow(powerplant_gas_coal_electricityBus_0_0)
 = 0
 
-c_e_BusBlock_balance(gasBus_1)_:
-+1 flow(gasBus_powerplant_gas_coal_1)
+c_e_BusBlock_balance(electricityBus_0_1)_:
++1 flow(powerplant_gas_coal_electricityBus_0_1)
 = 0
 
-c_e_BusBlock_balance(gasBus_2)_:
-+1 flow(gasBus_powerplant_gas_coal_2)
+c_e_BusBlock_balance(electricityBus_0_2)_:
++1 flow(powerplant_gas_coal_electricityBus_0_2)
 = 0
 
-c_e_BusBlock_balance(thermalBus_0)_:
-+1 flow(powerplant_gas_coal_thermalBus_0)
+c_e_BusBlock_balance(thermalBus_0_0)_:
++1 flow(powerplant_gas_coal_thermalBus_0_0)
 = 0
 
-c_e_BusBlock_balance(thermalBus_1)_:
-+1 flow(powerplant_gas_coal_thermalBus_1)
+c_e_BusBlock_balance(thermalBus_0_1)_:
++1 flow(powerplant_gas_coal_thermalBus_0_1)
 = 0
 
-c_e_BusBlock_balance(thermalBus_2)_:
-+1 flow(powerplant_gas_coal_thermalBus_2)
+c_e_BusBlock_balance(thermalBus_0_2)_:
++1 flow(powerplant_gas_coal_thermalBus_0_2)
 = 0
 
-c_e_TransformerBlock_relation(powerplant_gas_coal_coalBus_electricityBus_0)_:
-+0.29999999999999999 flow(coalBus_powerplant_gas_coal_0)
--0.20000000000000001 flow(powerplant_gas_coal_electricityBus_0)
+c_e_TransformerBlock_relation(powerplant_gas_coal_coalBus_electricityBus_0_0)_:
+-0.2 flow(powerplant_gas_coal_electricityBus_0_0)
++0.3 flow(coalBus_powerplant_gas_coal_0_0)
 = 0
 
-c_e_TransformerBlock_relation(powerplant_gas_coal_coalBus_electricityBus_1)_:
-+0.29999999999999999 flow(coalBus_powerplant_gas_coal_1)
--0.20000000000000001 flow(powerplant_gas_coal_electricityBus_1)
+c_e_TransformerBlock_relation(powerplant_gas_coal_gasBus_electricityBus_0_0)_:
+-0.58 flow(powerplant_gas_coal_electricityBus_0_0)
++0.3 flow(gasBus_powerplant_gas_coal_0_0)
 = 0
 
-c_e_TransformerBlock_relation(powerplant_gas_coal_coalBus_electricityBus_2)_:
-+0.29999999999999999 flow(coalBus_powerplant_gas_coal_2)
--0.20000000000000001 flow(powerplant_gas_coal_electricityBus_2)
+c_e_TransformerBlock_relation(powerplant_gas_coal_coalBus_thermalBus_0_0)_:
+-0.2 flow(powerplant_gas_coal_thermalBus_0_0)
++0.5 flow(coalBus_powerplant_gas_coal_0_0)
 = 0
 
-c_e_TransformerBlock_relation(powerplant_gas_coal_coalBus_thermalBus_0)_:
-+0.5 flow(coalBus_powerplant_gas_coal_0)
--0.20000000000000001 flow(powerplant_gas_coal_thermalBus_0)
+c_e_TransformerBlock_relation(powerplant_gas_coal_gasBus_thermalBus_0_0)_:
+-0.58 flow(powerplant_gas_coal_thermalBus_0_0)
++0.5 flow(gasBus_powerplant_gas_coal_0_0)
 = 0
 
-c_e_TransformerBlock_relation(powerplant_gas_coal_coalBus_thermalBus_1)_:
-+0.5 flow(coalBus_powerplant_gas_coal_1)
--0.20000000000000001 flow(powerplant_gas_coal_thermalBus_1)
+c_e_TransformerBlock_relation(powerplant_gas_coal_coalBus_electricityBus_0_1)_:
+-0.2 flow(powerplant_gas_coal_electricityBus_0_1)
++0.3 flow(coalBus_powerplant_gas_coal_0_1)
 = 0
 
-c_e_TransformerBlock_relation(powerplant_gas_coal_coalBus_thermalBus_2)_:
-+0.5 flow(coalBus_powerplant_gas_coal_2)
--0.20000000000000001 flow(powerplant_gas_coal_thermalBus_2)
+c_e_TransformerBlock_relation(powerplant_gas_coal_gasBus_electricityBus_0_1)_:
+-0.58 flow(powerplant_gas_coal_electricityBus_0_1)
++0.3 flow(gasBus_powerplant_gas_coal_0_1)
 = 0
 
-c_e_TransformerBlock_relation(powerplant_gas_coal_gasBus_electricityBus_0)_:
-+0.29999999999999999 flow(gasBus_powerplant_gas_coal_0)
--0.57999999999999996 flow(powerplant_gas_coal_electricityBus_0)
+c_e_TransformerBlock_relation(powerplant_gas_coal_coalBus_thermalBus_0_1)_:
+-0.2 flow(powerplant_gas_coal_thermalBus_0_1)
++0.5 flow(coalBus_powerplant_gas_coal_0_1)
 = 0
 
-c_e_TransformerBlock_relation(powerplant_gas_coal_gasBus_electricityBus_1)_:
-+0.29999999999999999 flow(gasBus_powerplant_gas_coal_1)
--0.57999999999999996 flow(powerplant_gas_coal_electricityBus_1)
+c_e_TransformerBlock_relation(powerplant_gas_coal_gasBus_thermalBus_0_1)_:
+-0.58 flow(powerplant_gas_coal_thermalBus_0_1)
++0.5 flow(gasBus_powerplant_gas_coal_0_1)
 = 0
 
-c_e_TransformerBlock_relation(powerplant_gas_coal_gasBus_electricityBus_2)_:
-+0.29999999999999999 flow(gasBus_powerplant_gas_coal_2)
--0.57999999999999996 flow(powerplant_gas_coal_electricityBus_2)
+c_e_TransformerBlock_relation(powerplant_gas_coal_coalBus_electricityBus_0_2)_:
+-0.2 flow(powerplant_gas_coal_electricityBus_0_2)
++0.3 flow(coalBus_powerplant_gas_coal_0_2)
 = 0
 
-c_e_TransformerBlock_relation(powerplant_gas_coal_gasBus_thermalBus_0)_:
-+0.5 flow(gasBus_powerplant_gas_coal_0)
--0.57999999999999996 flow(powerplant_gas_coal_thermalBus_0)
+c_e_TransformerBlock_relation(powerplant_gas_coal_gasBus_electricityBus_0_2)_:
+-0.58 flow(powerplant_gas_coal_electricityBus_0_2)
++0.3 flow(gasBus_powerplant_gas_coal_0_2)
 = 0
 
-c_e_TransformerBlock_relation(powerplant_gas_coal_gasBus_thermalBus_1)_:
-+0.5 flow(gasBus_powerplant_gas_coal_1)
--0.57999999999999996 flow(powerplant_gas_coal_thermalBus_1)
+c_e_TransformerBlock_relation(powerplant_gas_coal_coalBus_thermalBus_0_2)_:
+-0.2 flow(powerplant_gas_coal_thermalBus_0_2)
++0.5 flow(coalBus_powerplant_gas_coal_0_2)
 = 0
 
-c_e_TransformerBlock_relation(powerplant_gas_coal_gasBus_thermalBus_2)_:
-+0.5 flow(gasBus_powerplant_gas_coal_2)
--0.57999999999999996 flow(powerplant_gas_coal_thermalBus_2)
+c_e_TransformerBlock_relation(powerplant_gas_coal_gasBus_thermalBus_0_2)_:
+-0.58 flow(powerplant_gas_coal_thermalBus_0_2)
++0.5 flow(gasBus_powerplant_gas_coal_0_2)
 = 0
 
-c_u_InvestmentFlowBlock_max(powerplant_gas_coal_electricityBus_0)_:
--1 InvestmentFlowBlock_invest(powerplant_gas_coal_electricityBus)
-+1 flow(powerplant_gas_coal_electricityBus_0)
-<= 200
+c_e_InvestmentFlowBlock_total_rule(powerplant_gas_coal_electricityBus_0)_:
+-1 InvestmentFlowBlock_invest(powerplant_gas_coal_electricityBus_0)
++1 InvestmentFlowBlock_total(powerplant_gas_coal_electricityBus_0)
+= 200
 
-c_u_InvestmentFlowBlock_max(powerplant_gas_coal_electricityBus_1)_:
--1 InvestmentFlowBlock_invest(powerplant_gas_coal_electricityBus)
-+1 flow(powerplant_gas_coal_electricityBus_1)
-<= 200
+c_u_InvestmentFlowBlock_max(powerplant_gas_coal_electricityBus_0_0)_:
++1 flow(powerplant_gas_coal_electricityBus_0_0)
+-1 InvestmentFlowBlock_total(powerplant_gas_coal_electricityBus_0)
+<= 0
 
-c_u_InvestmentFlowBlock_max(powerplant_gas_coal_electricityBus_2)_:
--1 InvestmentFlowBlock_invest(powerplant_gas_coal_electricityBus)
-+1 flow(powerplant_gas_coal_electricityBus_2)
-<= 200
+c_u_InvestmentFlowBlock_max(powerplant_gas_coal_electricityBus_0_1)_:
++1 flow(powerplant_gas_coal_electricityBus_0_1)
+-1 InvestmentFlowBlock_total(powerplant_gas_coal_electricityBus_0)
+<= 0
 
-c_e_ONE_VAR_CONSTANT:
-ONE_VAR_CONSTANT = 1.0
+c_u_InvestmentFlowBlock_max(powerplant_gas_coal_electricityBus_0_2)_:
++1 flow(powerplant_gas_coal_electricityBus_0_2)
+-1 InvestmentFlowBlock_total(powerplant_gas_coal_electricityBus_0)
+<= 0
 
 bounds
-   0 <= flow(coalBus_powerplant_gas_coal_0) <= +inf
-   0 <= flow(coalBus_powerplant_gas_coal_1) <= +inf
-   0 <= flow(coalBus_powerplant_gas_coal_2) <= +inf
-   0 <= flow(gasBus_powerplant_gas_coal_0) <= +inf
-   0 <= flow(gasBus_powerplant_gas_coal_1) <= +inf
-   0 <= flow(gasBus_powerplant_gas_coal_2) <= +inf
-   0 <= flow(powerplant_gas_coal_electricityBus_0) <= +inf
-   0 <= flow(powerplant_gas_coal_electricityBus_1) <= +inf
-   0 <= flow(powerplant_gas_coal_electricityBus_2) <= +inf
-   0 <= flow(powerplant_gas_coal_thermalBus_0) <= +inf
-   0 <= flow(powerplant_gas_coal_thermalBus_1) <= +inf
-   0 <= flow(powerplant_gas_coal_thermalBus_2) <= +inf
-   0 <= InvestmentFlowBlock_invest(powerplant_gas_coal_electricityBus) <= 1000
+   0 <= InvestmentFlowBlock_invest(powerplant_gas_coal_electricityBus_0) <= 1000
+   0 <= flow(powerplant_gas_coal_electricityBus_0_0) <= +inf
+   0 <= flow(powerplant_gas_coal_electricityBus_0_1) <= +inf
+   0 <= flow(powerplant_gas_coal_electricityBus_0_2) <= +inf
+   0 <= flow(powerplant_gas_coal_thermalBus_0_0) <= +inf
+   0 <= flow(powerplant_gas_coal_thermalBus_0_1) <= +inf
+   0 <= flow(powerplant_gas_coal_thermalBus_0_2) <= +inf
+   0 <= flow(coalBus_powerplant_gas_coal_0_0) <= +inf
+   0 <= flow(coalBus_powerplant_gas_coal_0_1) <= +inf
+   0 <= flow(coalBus_powerplant_gas_coal_0_2) <= +inf
+   0 <= flow(gasBus_powerplant_gas_coal_0_0) <= +inf
+   0 <= flow(gasBus_powerplant_gas_coal_0_1) <= +inf
+   0 <= flow(gasBus_powerplant_gas_coal_0_2) <= +inf
+   0 <= InvestmentFlowBlock_total(powerplant_gas_coal_electricityBus_0) <= +inf
 end
```

### Comparing `oemof.solph-0.5.1.dev0/tests/lp_files/variable_chp.lp` & `oemof.solph-0.5.1.dev1/tests/lp_files/variable_chp.lp`

 * *Files 22% similar despite different names*

```diff
@@ -1,142 +1,140 @@
 \* Source Pyomo model name=Model *\
 
-min
+min 
 objective:
 +0 ONE_VAR_CONSTANT
 
 s.t.
 
-c_e_BusBlock_balance(commodityBus_0)_:
-+1 flow(commodityBus_variable_chp_gas1_0)
-+1 flow(commodityBus_variable_chp_gas2_0)
+c_e_BusBlock_balance(commodityBus_0_0)_:
++1 flow(commodityBus_variable_chp_gas1_0_0)
++1 flow(commodityBus_variable_chp_gas2_0_0)
 = 0
 
-c_e_BusBlock_balance(commodityBus_1)_:
-+1 flow(commodityBus_variable_chp_gas1_1)
-+1 flow(commodityBus_variable_chp_gas2_1)
+c_e_BusBlock_balance(commodityBus_0_1)_:
++1 flow(commodityBus_variable_chp_gas1_0_1)
++1 flow(commodityBus_variable_chp_gas2_0_1)
 = 0
 
-c_e_BusBlock_balance(commodityBus_2)_:
-+1 flow(commodityBus_variable_chp_gas1_2)
-+1 flow(commodityBus_variable_chp_gas2_2)
+c_e_BusBlock_balance(commodityBus_0_2)_:
++1 flow(commodityBus_variable_chp_gas1_0_2)
++1 flow(commodityBus_variable_chp_gas2_0_2)
 = 0
 
-c_e_BusBlock_balance(electricityBus_0)_:
-+1 flow(variable_chp_gas1_electricityBus_0)
-+1 flow(variable_chp_gas2_electricityBus_0)
+c_e_BusBlock_balance(electricityBus_0_0)_:
++1 flow(variable_chp_gas1_electricityBus_0_0)
++1 flow(variable_chp_gas2_electricityBus_0_0)
 = 0
 
-c_e_BusBlock_balance(electricityBus_1)_:
-+1 flow(variable_chp_gas1_electricityBus_1)
-+1 flow(variable_chp_gas2_electricityBus_1)
+c_e_BusBlock_balance(electricityBus_0_1)_:
++1 flow(variable_chp_gas1_electricityBus_0_1)
++1 flow(variable_chp_gas2_electricityBus_0_1)
 = 0
 
-c_e_BusBlock_balance(electricityBus_2)_:
-+1 flow(variable_chp_gas1_electricityBus_2)
-+1 flow(variable_chp_gas2_electricityBus_2)
+c_e_BusBlock_balance(electricityBus_0_2)_:
++1 flow(variable_chp_gas1_electricityBus_0_2)
++1 flow(variable_chp_gas2_electricityBus_0_2)
 = 0
 
-c_e_BusBlock_balance(heatBus_0)_:
-+1 flow(variable_chp_gas1_heatBus_0)
-+1 flow(variable_chp_gas2_heatBus_0)
+c_e_BusBlock_balance(heatBus_0_0)_:
++1 flow(variable_chp_gas1_heatBus_0_0)
++1 flow(variable_chp_gas2_heatBus_0_0)
 = 0
 
-c_e_BusBlock_balance(heatBus_1)_:
-+1 flow(variable_chp_gas1_heatBus_1)
-+1 flow(variable_chp_gas2_heatBus_1)
+c_e_BusBlock_balance(heatBus_0_1)_:
++1 flow(variable_chp_gas1_heatBus_0_1)
++1 flow(variable_chp_gas2_heatBus_0_1)
 = 0
 
-c_e_BusBlock_balance(heatBus_2)_:
-+1 flow(variable_chp_gas1_heatBus_2)
-+1 flow(variable_chp_gas2_heatBus_2)
+c_e_BusBlock_balance(heatBus_0_2)_:
++1 flow(variable_chp_gas1_heatBus_0_2)
++1 flow(variable_chp_gas2_heatBus_0_2)
 = 0
 
-c_e_ExtractionTurbineCHPBlock_input_output_relation(variable_chp_gas1_0)_:
-+1 flow(commodityBus_variable_chp_gas1_0)
--2 flow(variable_chp_gas1_electricityBus_0)
--0.80000000000000004 flow(variable_chp_gas1_heatBus_0)
-= 0
+c_e_ExtractionTurbineCHPBlock_input_output_relation(variable_chp_gas1_0_0)_:
++1 flow(commodityBus_variable_chp_gas1_0_0)
+-2.0 flow(variable_chp_gas1_electricityBus_0_0)
+-0.8 flow(variable_chp_gas1_heatBus_0_0)
+= 0.0
 
-c_e_ExtractionTurbineCHPBlock_input_output_relation(variable_chp_gas1_1)_:
-+1 flow(commodityBus_variable_chp_gas1_1)
--2 flow(variable_chp_gas1_electricityBus_1)
--0.80000000000000004 flow(variable_chp_gas1_heatBus_1)
-= 0
+c_e_ExtractionTurbineCHPBlock_input_output_relation(variable_chp_gas1_0_1)_:
++1 flow(commodityBus_variable_chp_gas1_0_1)
+-2.0 flow(variable_chp_gas1_electricityBus_0_1)
+-0.8 flow(variable_chp_gas1_heatBus_0_1)
+= 0.0
 
-c_e_ExtractionTurbineCHPBlock_input_output_relation(variable_chp_gas1_2)_:
-+1 flow(commodityBus_variable_chp_gas1_2)
--2 flow(variable_chp_gas1_electricityBus_2)
--0.80000000000000004 flow(variable_chp_gas1_heatBus_2)
-= 0
+c_e_ExtractionTurbineCHPBlock_input_output_relation(variable_chp_gas1_0_2)_:
++1 flow(commodityBus_variable_chp_gas1_0_2)
+-2.0 flow(variable_chp_gas1_electricityBus_0_2)
+-0.8 flow(variable_chp_gas1_heatBus_0_2)
+= 0.0
 
-c_e_ExtractionTurbineCHPBlock_input_output_relation(variable_chp_gas2_0)_:
-+1 flow(commodityBus_variable_chp_gas2_0)
--2 flow(variable_chp_gas2_electricityBus_0)
--0.80000000000000004 flow(variable_chp_gas2_heatBus_0)
-= 0
+c_e_ExtractionTurbineCHPBlock_input_output_relation(variable_chp_gas2_0_0)_:
++1 flow(commodityBus_variable_chp_gas2_0_0)
+-2.0 flow(variable_chp_gas2_electricityBus_0_0)
+-0.8 flow(variable_chp_gas2_heatBus_0_0)
+= 0.0
 
-c_e_ExtractionTurbineCHPBlock_input_output_relation(variable_chp_gas2_1)_:
-+1 flow(commodityBus_variable_chp_gas2_1)
--2 flow(variable_chp_gas2_electricityBus_1)
--0.80000000000000004 flow(variable_chp_gas2_heatBus_1)
-= 0
+c_e_ExtractionTurbineCHPBlock_input_output_relation(variable_chp_gas2_0_1)_:
++1 flow(commodityBus_variable_chp_gas2_0_1)
+-2.0 flow(variable_chp_gas2_electricityBus_0_1)
+-0.8 flow(variable_chp_gas2_heatBus_0_1)
+= 0.0
 
-c_e_ExtractionTurbineCHPBlock_input_output_relation(variable_chp_gas2_2)_:
-+1 flow(commodityBus_variable_chp_gas2_2)
--2 flow(variable_chp_gas2_electricityBus_2)
--0.80000000000000004 flow(variable_chp_gas2_heatBus_2)
-= 0
+c_e_ExtractionTurbineCHPBlock_input_output_relation(variable_chp_gas2_0_2)_:
++1 flow(commodityBus_variable_chp_gas2_0_2)
+-2.0 flow(variable_chp_gas2_electricityBus_0_2)
+-0.8 flow(variable_chp_gas2_heatBus_0_2)
+= 0.0
 
-c_u_ExtractionTurbineCHPBlock_out_flow_relation(variable_chp_gas1_0)_:
--1 flow(variable_chp_gas1_electricityBus_0)
-+0.59999999999999998 flow(variable_chp_gas1_heatBus_0)
+c_u_ExtractionTurbineCHPBlock_out_flow_relation(variable_chp_gas1_0_0)_:
+-1 flow(variable_chp_gas1_electricityBus_0_0)
++0.6 flow(variable_chp_gas1_heatBus_0_0)
 <= 0
 
-c_u_ExtractionTurbineCHPBlock_out_flow_relation(variable_chp_gas1_1)_:
--1 flow(variable_chp_gas1_electricityBus_1)
-+0.59999999999999998 flow(variable_chp_gas1_heatBus_1)
+c_u_ExtractionTurbineCHPBlock_out_flow_relation(variable_chp_gas1_0_1)_:
+-1 flow(variable_chp_gas1_electricityBus_0_1)
++0.6 flow(variable_chp_gas1_heatBus_0_1)
 <= 0
 
-c_u_ExtractionTurbineCHPBlock_out_flow_relation(variable_chp_gas1_2)_:
--1 flow(variable_chp_gas1_electricityBus_2)
-+0.59999999999999998 flow(variable_chp_gas1_heatBus_2)
+c_u_ExtractionTurbineCHPBlock_out_flow_relation(variable_chp_gas1_0_2)_:
+-1 flow(variable_chp_gas1_electricityBus_0_2)
++0.6 flow(variable_chp_gas1_heatBus_0_2)
 <= 0
 
-c_u_ExtractionTurbineCHPBlock_out_flow_relation(variable_chp_gas2_0)_:
--1 flow(variable_chp_gas2_electricityBus_0)
-+0.59999999999999998 flow(variable_chp_gas2_heatBus_0)
+c_u_ExtractionTurbineCHPBlock_out_flow_relation(variable_chp_gas2_0_0)_:
+-1 flow(variable_chp_gas2_electricityBus_0_0)
++0.6 flow(variable_chp_gas2_heatBus_0_0)
 <= 0
 
-c_u_ExtractionTurbineCHPBlock_out_flow_relation(variable_chp_gas2_1)_:
--1 flow(variable_chp_gas2_electricityBus_1)
-+0.59999999999999998 flow(variable_chp_gas2_heatBus_1)
+c_u_ExtractionTurbineCHPBlock_out_flow_relation(variable_chp_gas2_0_1)_:
+-1 flow(variable_chp_gas2_electricityBus_0_1)
++0.6 flow(variable_chp_gas2_heatBus_0_1)
 <= 0
 
-c_u_ExtractionTurbineCHPBlock_out_flow_relation(variable_chp_gas2_2)_:
--1 flow(variable_chp_gas2_electricityBus_2)
-+0.59999999999999998 flow(variable_chp_gas2_heatBus_2)
+c_u_ExtractionTurbineCHPBlock_out_flow_relation(variable_chp_gas2_0_2)_:
+-1 flow(variable_chp_gas2_electricityBus_0_2)
++0.6 flow(variable_chp_gas2_heatBus_0_2)
 <= 0
 
-c_e_ONE_VAR_CONSTANT:
-ONE_VAR_CONSTANT = 1.0
-
 bounds
-   0 <= flow(commodityBus_variable_chp_gas1_0) <= 100
-   0 <= flow(commodityBus_variable_chp_gas1_1) <= 100
-   0 <= flow(commodityBus_variable_chp_gas1_2) <= 100
-   0 <= flow(commodityBus_variable_chp_gas2_0) <= 100
-   0 <= flow(commodityBus_variable_chp_gas2_1) <= 100
-   0 <= flow(commodityBus_variable_chp_gas2_2) <= 100
-   0 <= flow(variable_chp_gas1_electricityBus_0) <= +inf
-   0 <= flow(variable_chp_gas1_electricityBus_1) <= +inf
-   0 <= flow(variable_chp_gas1_electricityBus_2) <= +inf
-   0 <= flow(variable_chp_gas1_heatBus_0) <= +inf
-   0 <= flow(variable_chp_gas1_heatBus_1) <= +inf
-   0 <= flow(variable_chp_gas1_heatBus_2) <= +inf
-   0 <= flow(variable_chp_gas2_electricityBus_0) <= +inf
-   0 <= flow(variable_chp_gas2_electricityBus_1) <= +inf
-   0 <= flow(variable_chp_gas2_electricityBus_2) <= +inf
-   0 <= flow(variable_chp_gas2_heatBus_0) <= +inf
-   0 <= flow(variable_chp_gas2_heatBus_1) <= +inf
-   0 <= flow(variable_chp_gas2_heatBus_2) <= +inf
+   1 <= ONE_VAR_CONSTANT <= 1
+   0 <= flow(commodityBus_variable_chp_gas1_0_0) <= 100
+   0 <= flow(commodityBus_variable_chp_gas2_0_0) <= 100
+   0 <= flow(commodityBus_variable_chp_gas1_0_1) <= 100
+   0 <= flow(commodityBus_variable_chp_gas2_0_1) <= 100
+   0 <= flow(commodityBus_variable_chp_gas1_0_2) <= 100
+   0 <= flow(commodityBus_variable_chp_gas2_0_2) <= 100
+   0 <= flow(variable_chp_gas1_electricityBus_0_0) <= +inf
+   0 <= flow(variable_chp_gas2_electricityBus_0_0) <= +inf
+   0 <= flow(variable_chp_gas1_electricityBus_0_1) <= +inf
+   0 <= flow(variable_chp_gas2_electricityBus_0_1) <= +inf
+   0 <= flow(variable_chp_gas1_electricityBus_0_2) <= +inf
+   0 <= flow(variable_chp_gas2_electricityBus_0_2) <= +inf
+   0 <= flow(variable_chp_gas1_heatBus_0_0) <= +inf
+   0 <= flow(variable_chp_gas2_heatBus_0_0) <= +inf
+   0 <= flow(variable_chp_gas1_heatBus_0_1) <= +inf
+   0 <= flow(variable_chp_gas2_heatBus_0_1) <= +inf
+   0 <= flow(variable_chp_gas1_heatBus_0_2) <= +inf
+   0 <= flow(variable_chp_gas2_heatBus_0_2) <= +inf
 end
```

### Comparing `oemof.solph-0.5.1.dev0/tests/regression_tests.py` & `oemof.solph-0.5.1.dev1/tests/regression_tests.py`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/tests/test_components.py` & `oemof.solph-0.5.1.dev1/tests/test_components.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,18 @@
             outflow_conversion_factor=0.8,
         )
 
 
 def test_generic_storage_2():
     """Nominal value defined with investment model."""
     bel = Bus()
-    with pytest.raises(AttributeError, match="If an investment object"):
+    with pytest.raises(
+        AttributeError,
+        match="For backward compatibility, the option investment overwrites",
+    ):
         components.GenericStorage(
             label="storage3",
             nominal_storage_capacity=45,
             inputs={bel: Flow(variable_costs=10e10)},
             outputs={bel: Flow(variable_costs=10e10)},
             loss_rate=0.00,
             initial_storage_level=0,
@@ -112,15 +115,15 @@
             investment=Investment(nonconvex=True, existing=5, maximum=25),
         )
 
 
 def test_generic_storage_with_non_convex_invest_maximum():
     """No investment maximum at nonconvex investment."""
     with pytest.raises(
-        AttributeError, match=r"Please provide an maximum investment value"
+        AttributeError, match=r"Please provide a maximum investment value"
     ):
         bel = Bus()
         components.GenericStorage(
             label="storage6",
             inputs={bel: Flow()},
             outputs={bel: Flow()},
             invest_relation_input_capacity=1 / 6,
```

### Comparing `oemof.solph-0.5.1.dev0/tests/test_constraints_module.py` & `oemof.solph-0.5.1.dev1/tests/test_constraints_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,11 +53,11 @@
         )
     )
     om = solph.Model(energysystem)
     line12 = energysystem.groups["powerline_1_2"]
     line21 = energysystem.groups["powerline_2_1"]
     solph.constraints.equate_variables(
         om,
-        om.InvestmentFlowBlock.invest[line12, bel2],
-        om.InvestmentFlowBlock.invest[line21, bel1],
+        om.InvestmentFlowBlock.invest[line12, bel2, 0],
+        om.InvestmentFlowBlock.invest[line21, bel1, 0],
         name="my_name",
     )
```

### Comparing `oemof.solph-0.5.1.dev0/tests/test_grouping.py` & `oemof.solph-0.5.1.dev1/tests/test_grouping.py`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/tests/test_models.py` & `oemof.solph-0.5.1.dev1/tests/test_models.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 available from its original location oemof/tests/basic_tests.py
 
 SPDX-License-Identifier: MIT
 """
 
 import warnings
 
+import pandas as pd
 import pytest
 
 from oemof import solph
 
 
 def test_optimal_solution():
     es = solph.EnergySystem(timeincrement=[1])
@@ -61,7 +62,38 @@
                     }
                 )
             )
             m = solph.Model(es)
             m.solve(solver="cbc")
             assert "Optimization ended with status" in str(w[0].message)
             solph.processing.meta_results(m)
+
+
+def test_multi_period_default_discount_rate():
+    """Test error being thrown for default multi-period discount rate"""
+    warnings.filterwarnings("ignore", category=FutureWarning)
+    timeindex = pd.date_range(start="2017-01-01", periods=100, freq="D")
+    es = solph.EnergySystem(timeindex=timeindex, periods={0: timeindex})
+    bel = solph.buses.Bus(label="bus")
+    es.add(bel)
+    es.add(
+        solph.components.Sink(
+            label="sink",
+            inputs={
+                bel: solph.flows.Flow(
+                    nominal_value=5, fix=[1] * len(timeindex)
+                )
+            },
+        )
+    )
+    es.add(
+        solph.components.Source(
+            label="source",
+            outputs={bel: solph.flows.Flow(nominal_value=4, variable_costs=5)},
+        )
+    )
+    msg = (
+        "By default, a discount_rate of 0.02 is used for a multi-period model."
+    )
+    with warnings.catch_warnings(record=True) as w:
+        solph.Model(es)
+        assert msg in str(w[0].message)
```

### Comparing `oemof.solph-0.5.1.dev0/tests/test_non_equidistant_time_index.py` & `oemof.solph-0.5.1.dev1/tests/test_non_equidistant_time_index.py`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/tests/test_outputlib/__init__.py` & `oemof.solph-0.5.1.dev1/tests/test_outputlib/__init__.py`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/tests/test_outputlib/input_data.csv` & `oemof.solph-0.5.1.dev1/tests/test_outputlib/input_data.csv`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/tests/test_outputlib/test_views.py` & `oemof.solph-0.5.1.dev1/tests/test_outputlib/test_views.py`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/tests/test_processing.py` & `oemof.solph-0.5.1.dev1/tests/test_processing.py`

 * *Files 14% similar despite different names*

```diff
@@ -112,34 +112,37 @@
 
     def test_flows_without_none_exclusion(self):
         b_el2 = self.es.groups["b_el2"]
         demand = self.es.groups["demand_el"]
         param_results = processing.parameter_as_dict(
             self.es, exclude_none=False
         )
-        scalar_attributes = {
+        default_attributes = {
+            "age": None,
+            "lifetime": None,
             "integer": False,
             "investment": None,
             "nominal_value": 1,
             "nonconvex": None,
             "bidirectional": False,
             "full_load_time_max": None,
             "full_load_time_min": None,
             "max": 1,
             "min": 0,
             "negative_gradient_limit": None,
             "positive_gradient_limit": None,
             "variable_costs": 0,
+            "fixed_costs": None,
             "flow": None,
             "values": None,
             "label": str(b_el2.outputs[demand].label),
         }
         assert_series_equal(
             param_results[(b_el2, demand)]["scalars"].sort_index(),
-            pandas.Series(scalar_attributes).sort_index(),
+            pandas.Series(default_attributes).sort_index(),
         )
         sequences_attributes = {
             "fix": self.demand_values,
         }
 
         assert_frame_equal(
             param_results[(b_el2, demand)]["sequences"],
@@ -156,21 +159,25 @@
             param_results[("storage", "None")]["scalars"],
             pandas.Series(
                 {
                     "balanced": True,
                     "initial_storage_level": 0,
                     "invest_relation_input_capacity": 1 / 6,
                     "invest_relation_output_capacity": 1 / 6,
-                    "investment_ep_costs": 0.4,
+                    "investment_age": 0,
                     "investment_existing": 0,
+                    "investment_interest_rate": 0,
+                    "investment_nonconvex": False,
+                    "investment_ep_costs": 0.4,
                     "investment_maximum": float("inf"),
                     "investment_minimum": 0,
                     "investment_nonconvex": False,
                     "investment_offset": 0,
                     "label": "storage",
+                    "fixed_costs": 0,
                     "fixed_losses_absolute": 0,
                     "fixed_losses_relative": 0,
                     "inflow_conversion_factor": 1,
                     "loss_rate": 0,
                     "max_storage_level": 1,
                     "min_storage_level": 0,
                     "outflow_conversion_factor": 0.8,
@@ -192,21 +199,25 @@
             param_results[("storage", None)]["scalars"],
             pandas.Series(
                 {
                     "balanced": True,
                     "initial_storage_level": 0,
                     "invest_relation_input_capacity": 1 / 6,
                     "invest_relation_output_capacity": 1 / 6,
-                    "investment_ep_costs": 0.4,
+                    "investment_age": 0,
                     "investment_existing": 0,
+                    "investment_interest_rate": 0,
+                    "investment_nonconvex": False,
+                    "investment_ep_costs": 0.4,
                     "investment_maximum": float("inf"),
                     "investment_minimum": 0,
                     "investment_nonconvex": False,
                     "investment_offset": 0,
                     "label": "storage",
+                    "fixed_costs": 0,
                     "fixed_losses_absolute": 0,
                     "fixed_losses_relative": 0,
                     "inflow_conversion_factor": 1,
                     "loss_rate": 0,
                     "max_storage_level": 1,
                     "min_storage_level": 0,
                     "outflow_conversion_factor": 0.8,
@@ -272,29 +283,29 @@
         assert (
             int(bel1["sequences"][("diesel", "b_el1", "flow")].sum()) == 2875
         )
 
     def test_error_from_nan_values(self):
         trsf = self.es.groups["diesel"]
         bus = self.es.groups["b_el1"]
-        self.mod.flow[trsf, bus, 5] = float("nan")
+        self.mod.flow[trsf, bus, 0, 5] = float("nan")
         with pytest.raises(ValueError):
             processing.results(self.mod)
 
     def test_duals(self):
         results = processing.results(self.om)
         bel = views.node(results, "b_el1", multiindex=True)
         assert int(bel["sequences"]["b_el1", "None", "duals"].sum()) == 48
 
     def test_node_weight_by_type(self):
         results = processing.results(self.om)
         storage_content = views.node_weight_by_type(
             results, node_type=GenericStorage
         )
-        assert round(float(storage_content.sum()), 6) == 1437.500003
+        assert round(float(storage_content.sum()), 1) == 1437.5
 
     def test_output_by_type_view(self):
         results = processing.results(self.om)
         transformer_output = views.node_output_by_type(
             results, node_type=Transformer
         )
         compare = views.node(results, "diesel", multiindex=True)["sequences"][
```

### Comparing `oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_connect_invest/connect_invest.csv` & `oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_connect_invest/connect_invest.csv`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_connect_invest/test_connect_invest.py` & `oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_connect_invest/test_connect_invest.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,34 +96,42 @@
     )
     es.add(line21)
 
     om = Model(es)
 
     constraints.equate_variables(
         om,
-        om.InvestmentFlowBlock.invest[line12, bel2],
-        om.InvestmentFlowBlock.invest[line21, bel1],
+        om.InvestmentFlowBlock.invest[line12, bel2, 0],
+        om.InvestmentFlowBlock.invest[line21, bel1, 0],
         2,
     )
     constraints.equate_variables(
         om,
-        om.InvestmentFlowBlock.invest[line12, bel2],
-        om.GenericInvestmentStorageBlock.invest[storage],
+        om.InvestmentFlowBlock.invest[line12, bel2, 0],
+        om.GenericInvestmentStorageBlock.invest[storage, 0],
     )
 
     # if tee_switch is true solver messages will be displayed
     logging.info("Solve the optimization problem")
-    om.solve(solver="cbc")
+    om.solve(solver="cbc", tee=True)
 
     # check if the new result object is working for custom components
     results = processing.results(om)
 
     my_results = dict()
-    my_results["line12"] = float(views.node(results, "line12")["scalars"])
-    my_results["line21"] = float(views.node(results, "line21")["scalars"])
+    my_results["line12"] = float(
+        views.node(results, "line12")["scalars"].loc[
+            [(("line12", "electricity2"), "invest")]
+        ]
+    )
+    my_results["line21"] = float(
+        views.node(results, "line21")["scalars"].loc[
+            [(("line21", "electricity1"), "invest")]
+        ]
+    )
     stor_res = views.node(results, "storage")["scalars"]
     my_results["storage_in"] = stor_res[
         [(("electricity1", "storage"), "invest")]
     ]
     my_results["storage"] = stor_res[[(("storage", "None"), "invest")]]
     my_results["storage_out"] = stor_res[
         [(("storage", "electricity1"), "invest")]
```

### Comparing `oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_flexible_modelling/test_add_constraints.py` & `oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_flexible_modelling/test_add_constraints.py`

 * *Files 6% similar despite different names*

```diff
@@ -94,34 +94,34 @@
     myblock.COMMODITYFLOWS = [
         k for (k, v) in om.flows.items() if hasattr(v, "emission_factor")
     ]
 
     # add the sub-model to the oemof Model instance
     om.add_component("MyBlock", myblock)
 
-    def _inflow_share_rule(m, si, e, ti):
+    def _inflow_share_rule(m, si, e, p, ti):
         """pyomo rule definition: Here we can use all objects from the block or
         the om object, in this case we don't need anything from the block
         except the newly defined set MYFLOWS.
         """
-        expr = om.flow[si, e, ti] >= om.flows[si, e].outflow_share[ti] * sum(
-            om.flow[i, o, ti] for (i, o) in om.FLOWS if o == e
-        )
+        expr = om.flow[si, e, p, ti] >= om.flows[si, e].outflow_share[
+            ti
+        ] * sum(om.flow[i, o, p, ti] for (i, o) in om.FLOWS if o == e)
         return expr
 
     myblock.inflow_share = po.Constraint(
-        myblock.MYFLOWS, om.TIMESTEPS, rule=_inflow_share_rule
+        myblock.MYFLOWS, om.TIMEINDEX, rule=_inflow_share_rule
     )
     # add emission constraint
     myblock.emission_constr = po.Constraint(
         expr=(
             sum(
-                om.flow[i, o, t]
+                om.flow[i, o, p, t]
                 for (i, o) in myblock.COMMODITYFLOWS
-                for t in om.TIMESTEPS
+                for p, t in om.TIMEINDEX
             )
             <= emission_limit
         )
     )
 
     # solve and write results to dictionary
     # you may print the model with om.pprint()
```

### Comparing `oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_generic_caes/generic_caes.csv` & `oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_generic_caes/generic_caes.csv`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_generic_caes/test_generic_caes.py` & `oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_generic_caes/test_generic_caes.py`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_generic_chp/ccet.csv` & `oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_generic_chp/ccet.csv`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_generic_chp/test_generic_chp.py` & `oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_generic_chp/test_generic_chp.py`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_invest_fix_flow/test_simple_invest_fixed.py` & `oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_invest_fix_flow/test_simple_invest_fixed.py`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_lopf/test_lopf.py` & `oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_lopf/test_lopf.py`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_options/test_non_convex.py` & `oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_options/test_non_convex.py`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_piecewiselineartransformer/test_piecewiselineartransformer.py` & `oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_piecewiselineartransformer/test_piecewiselineartransformer.py`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_simple_model/input_data.csv` & `oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_simple_model/input_data.csv`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_simple_model/test_simple_dispatch.py` & `oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_simple_model/test_simple_dispatch.py`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_simple_model/test_simple_dispatch_one.py` & `oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_simple_model/test_simple_dispatch_one.py`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_simple_model/test_simple_dispatch_one_explicit_timemode.py` & `oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_simple_model/test_simple_dispatch_one_explicit_timemode.py`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_simple_model/test_simple_invest.py` & `oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_simple_model/test_simple_invest.py`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_storage_investment/storage_investment.csv` & `oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_storage_investment/storage_investment.csv`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_storage_investment/test_invest_storage_regression.py` & `oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_storage_investment/test_invest_storage_regression.py`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_storage_investment/test_storage_investment.py` & `oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_storage_investment/test_storage_investment.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,14 +147,15 @@
     es.results["meta"] = processing.meta_results(om)
 
     # Check dump and restore
     es.dump()
 
 
 def test_results_with_actual_dump():
+    test_optimise_storage_size()
     energysystem = solph.EnergySystem()
     energysystem.restore()
 
     # Results
     results = energysystem.results["main"]
     meta = energysystem.results["meta"]
 
@@ -184,27 +185,28 @@
     assert str(meta["solver"]["Termination condition"]) == "optimal"
     assert meta["solver"]["Error rc"] == 0
     assert str(meta["solver"]["Status"]) == "ok"
 
     # Problem results
     assert meta["problem"]["Lower bound"] == 4.231675777e17
     assert meta["problem"]["Upper bound"], 4.231675777e17
-    assert meta["problem"]["Number of variables"] == 2805
-    assert meta["problem"]["Number of constraints"] == 2806
+    assert meta["problem"]["Number of variables"] == 2807
+    assert meta["problem"]["Number of constraints"] == 2808
     assert meta["problem"]["Number of nonzeros"] == 1197
     assert meta["problem"]["Number of objectives"] == 1
     assert str(meta["problem"]["Sense"]) == "minimize"
 
     # Objective function
     assert round(meta["objective"]) == 423167578261115584
 
 
 def test_solph_transformer_attributes_before_dump_and_after_restore():
     """dump/restore should preserve all attributes
     of `solph.components.Transformer`"""
+    test_optimise_storage_size()
     energysystem = solph.EnergySystem()
     energysystem.restore()
 
     trsf_attr_before_dump = sorted([x for x in dir(PP_GAS) if "__" not in x])
 
     trsf_attr_after_restore = sorted(
         [x for x in dir(energysystem.groups["pp_gas"]) if "__" not in x]
```

### Comparing `oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_storage_investment/test_storage_with_tuple_label.py` & `oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_storage_investment/test_storage_with_tuple_label.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,15 +207,15 @@
     assert str(meta["solver"]["Termination condition"]) == "optimal"
     assert meta["solver"]["Error rc"] == 0
     assert str(meta["solver"]["Status"]) == "ok"
 
     # Problem results
     assert int(meta["problem"]["Lower bound"]) == 37819254
     assert int(meta["problem"]["Upper bound"]) == 37819254
-    assert meta["problem"]["Number of variables"] == 281
-    assert meta["problem"]["Number of constraints"] == 163
+    assert meta["problem"]["Number of variables"] == 280
+    assert meta["problem"]["Number of constraints"] == 162
     assert meta["problem"]["Number of nonzeros"] == 116
     assert meta["problem"]["Number of objectives"] == 1
     assert str(meta["problem"]["Sense"]) == "minimize"
 
     # Objective function
     assert round(meta["objective"]) == 37819254
```

### Comparing `oemof.solph-0.5.1.dev0/tests/test_scripts/test_solph/test_variable_chp/test_variable_chp.py` & `oemof.solph-0.5.1.dev1/tests/test_scripts/test_solph/test_variable_chp/test_variable_chp.py`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/tests/test_solph_network_classes.py` & `oemof.solph-0.5.1.dev1/tests/test_solph_network_classes.py`

 * *Files 20% similar despite different names*

```diff
@@ -67,19 +67,36 @@
 
     def test_transformer_missing_input_create_empty_dict(self):
         trfr = solph.components.Transformer(outputs={})
         assert trfr.inputs == {}
 
 
 def test_wrong_combination_invest_and_nominal_value():
-    msg = "Using the investment object the nominal_value"
-    with pytest.raises(ValueError, match=msg):
+    msg = "For backward compatibility, the option investment overwrites"
+    with pytest.raises(AttributeError, match=msg):
         solph.flows.Flow(investment=solph.Investment(), nominal_value=4)
 
 
+def test_fixed_costs_warning():
+    msg = (
+        "Be aware that the fixed costs attribute is only\n"
+        "meant to be used for multi-period models.\n"
+        "If you wish to set up a multi-period model, explicitly "
+        "set the `periods` attribute of your energy system.\n"
+        "It has been decided to remove the `fixed_costs` "
+        "attribute with v0.2 for regular uses.\n"
+        "If you specify `fixed_costs` for a regular model, "
+        "it will simply be ignored."
+    )
+    with warnings.catch_warnings(record=True) as w:
+        solph.flows.Flow(fixed_costs=34)
+        assert len(w) != 0
+        assert msg == str(w[-1].message)
+
+
 def test_flow_with_fix_and_min_max():
     msg = "It is not allowed to define `min`/`max` if `fix` is defined."
     with pytest.raises(AttributeError, match=msg):
         solph.flows.Flow(fix=[1, 3], min=[0, 5])
     with pytest.raises(AttributeError, match=msg):
         solph.flows.Flow(fix=[1, 3], max=[0, 5])
     with pytest.raises(AttributeError, match=msg):
```

### Comparing `oemof.solph-0.5.1.dev0/tests/test_time_index.py` & `oemof.solph-0.5.1.dev1/tests/test_time_index.py`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/tests/test_warnings.py` & `oemof.solph-0.5.1.dev1/tests/test_warnings.py`

 * *Files identical despite different names*

### Comparing `oemof.solph-0.5.1.dev0/tox.ini` & `oemof.solph-0.5.1.dev1/tox.ini`

 * *Files identical despite different names*

