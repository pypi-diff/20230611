# Comparing `tmp/mpltern-0.5.0.tar.gz` & `tmp/mpltern-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpltern-0.5.0.tar", last modified: Wed Feb 22 03:33:34 2023, max compression
+gzip compressed data, was "mpltern-1.0.0.tar", last modified: Sun Jun 11 14:32:31 2023, max compression
```

## Comparing `mpltern-0.5.0.tar` & `mpltern-1.0.0.tar`

### file list

```diff
@@ -1,527 +1,544 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 03:33:34.814236 mpltern-0.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 03:33:34.718235 mpltern-0.5.0/.circleci/
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-02-22 03:33:22.000000 mpltern-0.5.0/.circleci/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-22 03:33:22.000000 mpltern-0.5.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-22 03:33:22.000000 mpltern-0.5.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 03:33:34.710235 mpltern-0.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 03:33:34.718235 mpltern-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-02-22 03:33:22.000000 mpltern-0.5.0/.github/workflows/publish-to-test-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-02-22 03:33:22.000000 mpltern-0.5.0/.github/workflows/tests.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1203 2023-02-22 03:33:22.000000 mpltern-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-02-22 03:33:22.000000 mpltern-0.5.0/.lgtm.yml
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-02-22 03:33:22.000000 mpltern-0.5.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-02-22 03:33:22.000000 mpltern-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-02-22 03:33:22.000000 mpltern-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-02-22 03:33:34.814236 mpltern-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-02-22 03:33:22.000000 mpltern-0.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 03:33:34.718235 mpltern-0.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-02-22 03:33:22.000000 mpltern-0.5.0/docs/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 03:33:34.726235 mpltern-0.5.0/docsrc/
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-02-22 03:33:22.000000 mpltern-0.5.0/docsrc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 03:33:34.726235 mpltern-0.5.0/docsrc/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-02-22 03:33:22.000000 mpltern-0.5.0/docsrc/_static/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-02-22 03:33:22.000000 mpltern-0.5.0/docsrc/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-02-22 03:33:22.000000 mpltern-0.5.0/docsrc/_static/sphx_glr_logos0_002.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-02-22 03:33:22.000000 mpltern-0.5.0/docsrc/alternatives.rst
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-02-22 03:33:22.000000 mpltern-0.5.0/docsrc/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)    20478 2023-02-22 03:33:22.000000 mpltern-0.5.0/docsrc/basic_1.svg
--rw-r--r--   0 runner    (1001) docker     (123)    23805 2023-02-22 03:33:22.000000 mpltern-0.5.0/docsrc/basic_2.svg
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-02-22 03:33:22.000000 mpltern-0.5.0/docsrc/basic_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-02-22 03:33:22.000000 mpltern-0.5.0/docsrc/basic_usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-02-22 03:33:22.000000 mpltern-0.5.0/docsrc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-02-22 03:33:22.000000 mpltern-0.5.0/docsrc/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-02-22 03:33:22.000000 mpltern-0.5.0/docsrc/corner_based_1.py
--rw-r--r--   0 runner    (1001) docker     (123)    50242 2023-02-22 03:33:22.000000 mpltern-0.5.0/docsrc/corner_based_1.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-02-22 03:33:22.000000 mpltern-0.5.0/docsrc/corner_based_2.py
--rw-r--r--   0 runner    (1001) docker     (123)    52879 2023-02-22 03:33:22.000000 mpltern-0.5.0/docsrc/corner_based_2.svg
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-02-22 03:33:22.000000 mpltern-0.5.0/docsrc/create_favicon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-02-22 03:33:22.000000 mpltern-0.5.0/docsrc/implemented_methods.rst
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-02-22 03:33:22.000000 mpltern-0.5.0/docsrc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-02-22 03:33:22.000000 mpltern-0.5.0/docsrc/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-02-22 03:33:22.000000 mpltern-0.5.0/docsrc/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-22 03:33:22.000000 mpltern-0.5.0/docsrc/matplotlibrc
--rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-02-22 03:33:22.000000 mpltern-0.5.0/docsrc/notes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-02-22 03:33:22.000000 mpltern-0.5.0/docsrc/publications.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-02-22 03:33:22.000000 mpltern-0.5.0/docsrc/release_notes.rst
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-02-22 03:33:22.000000 mpltern-0.5.0/docsrc/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-02-22 03:33:22.000000 mpltern-0.5.0/docsrc/side_based_ccw.py
--rw-r--r--   0 runner    (1001) docker     (123)    54814 2023-02-22 03:33:22.000000 mpltern-0.5.0/docsrc/side_based_ccw.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-02-22 03:33:22.000000 mpltern-0.5.0/docsrc/side_based_cw.py
--rw-r--r--   0 runner    (1001) docker     (123)    53409 2023-02-22 03:33:22.000000 mpltern-0.5.0/docsrc/side_based_cw.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 03:33:34.726235 mpltern-0.5.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-02-22 03:33:22.000000 mpltern-0.5.0/examples/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 03:33:34.726235 mpltern-0.5.0/examples/advanced/
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-02-22 03:33:22.000000 mpltern-0.5.0/examples/advanced/00.colored_axes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-02-22 03:33:22.000000 mpltern-0.5.0/examples/advanced/01.arrows_along_axes.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-02-22 03:33:22.000000 mpltern-0.5.0/examples/advanced/02.minor_ticks.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-02-22 03:33:22.000000 mpltern-0.5.0/examples/advanced/03.manual_tick_positions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-02-22 03:33:22.000000 mpltern-0.5.0/examples/advanced/04.tick_labels_inside_triangle.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-02-22 03:33:22.000000 mpltern-0.5.0/examples/advanced/05.inset.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-02-22 03:33:22.000000 mpltern-0.5.0/examples/advanced/06.plot_fixed_onto_triangle.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-22 03:33:22.000000 mpltern-0.5.0/examples/advanced/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 03:33:34.730235 mpltern-0.5.0/examples/axis_and_tick/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-22 03:33:22.000000 mpltern-0.5.0/examples/axis_and_tick/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-02-22 03:33:22.000000 mpltern-0.5.0/examples/axis_and_tick/axis_label_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-02-22 03:33:22.000000 mpltern-0.5.0/examples/axis_and_tick/axis_label_rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-02-22 03:33:22.000000 mpltern-0.5.0/examples/axis_and_tick/tick_direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-02-22 03:33:22.000000 mpltern-0.5.0/examples/axis_and_tick/tick_position.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-02-22 03:33:22.000000 mpltern-0.5.0/examples/axis_and_tick/tick_rotation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 03:33:34.730235 mpltern-0.5.0/examples/intermediate/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-22 03:33:22.000000 mpltern-0.5.0/examples/intermediate/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-02-22 03:33:22.000000 mpltern-0.5.0/examples/intermediate/axline.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-02-22 03:33:22.000000 mpltern-0.5.0/examples/intermediate/legend.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-02-22 03:33:22.000000 mpltern-0.5.0/examples/intermediate/ternary_limits.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-02-22 03:33:22.000000 mpltern-0.5.0/examples/intermediate/with_normal_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-02-22 03:33:22.000000 mpltern-0.5.0/examples/intermediate/with_seaborn_styles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 03:33:34.730235 mpltern-0.5.0/examples/introductory/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-02-22 03:33:22.000000 mpltern-0.5.0/examples/introductory/00.line_and_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-02-22 03:33:22.000000 mpltern-0.5.0/examples/introductory/01.scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-02-22 03:33:22.000000 mpltern-0.5.0/examples/introductory/02.contour.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-02-22 03:33:22.000000 mpltern-0.5.0/examples/introductory/03.pseudocolor.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-02-22 03:33:22.000000 mpltern-0.5.0/examples/introductory/04.normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-02-22 03:33:22.000000 mpltern-0.5.0/examples/introductory/05.span.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-02-22 03:33:22.000000 mpltern-0.5.0/examples/introductory/06.text.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-02-22 03:33:22.000000 mpltern-0.5.0/examples/introductory/07.polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-02-22 03:33:22.000000 mpltern-0.5.0/examples/introductory/08.quiver.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-02-22 03:33:22.000000 mpltern-0.5.0/examples/introductory/09.grid.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-02-22 03:33:22.000000 mpltern-0.5.0/examples/introductory/10.axis_labels.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-02-22 03:33:22.000000 mpltern-0.5.0/examples/introductory/11.triangular_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-22 03:33:22.000000 mpltern-0.5.0/examples/introductory/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 03:33:34.734235 mpltern-0.5.0/examples/miscellaneous/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-22 03:33:22.000000 mpltern-0.5.0/examples/miscellaneous/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-02-22 03:33:22.000000 mpltern-0.5.0/examples/miscellaneous/dirichlet_pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-02-22 03:33:22.000000 mpltern-0.5.0/examples/miscellaneous/logos0.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 03:33:34.734235 mpltern-0.5.0/examples/statistics/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-22 03:33:22.000000 mpltern-0.5.0/examples/statistics/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-02-22 03:33:22.000000 mpltern-0.5.0/examples/statistics/hexbin.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-02-22 03:33:22.000000 mpltern-0.5.0/examples/statistics/tribin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-02-22 03:33:22.000000 mpltern-0.5.0/examples/statistics/with_scatter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 03:33:34.734235 mpltern-0.5.0/examples/triangle/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-02-22 03:33:22.000000 mpltern-0.5.0/examples/triangle/00.aspect.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-02-22 03:33:22.000000 mpltern-0.5.0/examples/triangle/01.triangle_rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-02-22 03:33:22.000000 mpltern-0.5.0/examples/triangle/02.arbitrary_triangle.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-22 03:33:22.000000 mpltern-0.5.0/examples/triangle/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 03:33:34.734235 mpltern-0.5.0/mpltern/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-02-22 03:33:22.000000 mpltern-0.5.0/mpltern/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-02-22 03:33:22.000000 mpltern-0.5.0/mpltern/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-02-22 03:33:22.000000 mpltern-0.5.0/mpltern/hexbin_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 03:33:34.738235 mpltern-0.5.0/mpltern/ternary/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-22 03:33:22.000000 mpltern-0.5.0/mpltern/ternary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28641 2023-02-22 03:33:22.000000 mpltern-0.5.0/mpltern/ternary/_axes.py
--rw-r--r--   0 runner    (1001) docker     (123)    25921 2023-02-22 03:33:22.000000 mpltern-0.5.0/mpltern/ternary/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    14129 2023-02-22 03:33:22.000000 mpltern-0.5.0/mpltern/ternary/axis.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-02-22 03:33:22.000000 mpltern-0.5.0/mpltern/ternary/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-02-22 03:33:22.000000 mpltern-0.5.0/mpltern/ternary/spines.py
--rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-02-22 03:33:22.000000 mpltern-0.5.0/mpltern/ternary/tick.py
--rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-02-22 03:33:22.000000 mpltern-0.5.0/mpltern/ternary/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-02-22 03:33:22.000000 mpltern-0.5.0/mpltern/ternary_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-02-22 03:33:22.000000 mpltern-0.5.0/mpltern/tribin_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 03:33:34.734235 mpltern-0.5.0/mpltern.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-02-22 03:33:34.000000 mpltern-0.5.0/mpltern.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27996 2023-02-22 03:33:34.000000 mpltern-0.5.0/mpltern.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 03:33:34.000000 mpltern-0.5.0/mpltern.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-22 03:33:34.000000 mpltern-0.5.0/mpltern.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-22 03:33:34.000000 mpltern-0.5.0/mpltern.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-02-22 03:33:22.000000 mpltern-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-22 03:33:22.000000 mpltern-0.5.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-22 03:33:34.814236 mpltern-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-02-22 03:33:22.000000 mpltern-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 03:33:34.742235 mpltern-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/Dirichlet_PDF_1.0_2.0_2.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/Dirichlet_PDF_1.5_1.5_1.5.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/Dirichlet_PDF_2.0_4.0_8.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/Dirichlet_PDF_5.0_5.0_5.0.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 03:33:34.718235 mpltern-0.5.0/tests/baseline_images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 03:33:34.742235 mpltern-0.5.0/tests/baseline_images/test_constrainedlayout/
--rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_constrainedlayout/constrained_layout1.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 03:33:34.746235 mpltern-0.5.0/tests/baseline_images/test_given_triangles/
--rw-r--r--   0 runner    (1001) docker     (123)    11382 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_given_triangles/given_triangles_axis_0.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_given_triangles/given_triangles_axis_180.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_given_triangles/given_triangles_axis_270.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_given_triangles/given_triangles_axis_90.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_given_triangles/given_triangles_horizontal_0.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_given_triangles/given_triangles_horizontal_180.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    11337 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_given_triangles/given_triangles_horizontal_270.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    11364 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_given_triangles/given_triangles_horizontal_90.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    11382 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_given_triangles/given_triangles_tick_0.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    11378 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_given_triangles/given_triangles_tick_180.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_given_triangles/given_triangles_tick_270.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_given_triangles/given_triangles_tick_90.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 03:33:34.746235 mpltern-0.5.0/tests/baseline_images/test_hexbin/
--rw-r--r--   0 runner    (1001) docker     (123)    18995 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_hexbin/base.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    11419 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_hexbin/extent.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    19493 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_hexbin/given_triangles.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    20041 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_hexbin/ternary_lim.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 03:33:34.754235 mpltern-0.5.0/tests/baseline_images/test_ternary/
--rw-r--r--   0 runner    (1001) docker     (123)    10189 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_ternary/arguments_6.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_ternary/arguments_7.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_ternary/arrow_axes.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_ternary/arrow_data.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_ternary/arrow_xy_axes.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6386 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_ternary/arrow_xy_data.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    11059 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_ternary/aspect.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     8826 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_ternary/axis_label_position_corner.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     8832 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_ternary/axis_label_position_tick1.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     8839 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_ternary/axis_label_position_tick2.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_ternary/legend.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    11150 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_ternary/manual_ticks.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_ternary/negative_ticks.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_ternary/opposite_ticks.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_ternary/plot.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_ternary/quiver.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    16075 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_ternary/quiver_color.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    13098 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_ternary/quiver_xy_axes.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    12916 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_ternary/quiver_xy_data.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     9473 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_ternary/scatter.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    19943 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_ternary/scatter_color.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    12043 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_ternary/test_ternary_lim-expected.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    65470 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_ternary/test_ternary_lim-expected.png
--rw-r--r--   0 runner    (1001) docker     (123)    38681 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_ternary/test_ternary_lim-expected.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_ternary/test_ternary_lim-expected_pdf.png
--rw-r--r--   0 runner    (1001) docker     (123)    63063 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_ternary/test_ternary_lim-expected_svg.png
--rw-r--r--   0 runner    (1001) docker     (123)    12043 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_ternary/test_ternary_lim.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    65470 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_ternary/test_ternary_lim.png
--rw-r--r--   0 runner    (1001) docker     (123)    38681 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_ternary/test_ternary_lim.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_ternary/test_ternary_lim_pdf.png
--rw-r--r--   0 runner    (1001) docker     (123)    63063 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_ternary/test_ternary_lim_svg.png
--rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_ternary/text.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_ternary/tick_direction_in.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_ternary/tick_direction_inout.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_ternary/tick_direction_out.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_ternary/tick_labels_inside_triangle.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_ternary/titie_center.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6887 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_ternary/titie_left.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_ternary/titie_right.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_ternary/transAxes.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 03:33:34.754235 mpltern-0.5.0/tests/baseline_images/test_tightlayout/
--rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_tightlayout/tight_layout1.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 03:33:34.774236 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/
--rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_0.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6693 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_105.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_120.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_135.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_15.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_150.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_165.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_180.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_195.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_210.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6693 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_225.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_240.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_255.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_270.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_285.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_30.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_300.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_315.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_330.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_345.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_360.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_45.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_60.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_75.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6473 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_90.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_0.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_105.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_120.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_135.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_15.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6476 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_150.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_165.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_180.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_195.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_210.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_225.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_240.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_255.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_270.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_285.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_30.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_300.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_315.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_330.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_345.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_360.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_45.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_60.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_75.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_90.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_0.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_105.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_120.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_135.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_15.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_150.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_165.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_180.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_195.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_210.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_225.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_240.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_255.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_270.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_285.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_30.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_300.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_315.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_330.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_345.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_360.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_45.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_60.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_75.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_90.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_0.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_105.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_120.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_135.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_15.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_150.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_165.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_180.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_195.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_210.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_225.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_240.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6688 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_255.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_270.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_285.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_30.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_300.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_315.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_330.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_345.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_360.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_45.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_60.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_75.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6480 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_90.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 03:33:34.794236 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/
--rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_0.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_105.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_120.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_135.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_15.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_150.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_165.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_180.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6636 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_195.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_210.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_225.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_240.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_255.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_270.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_285.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_30.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_300.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_315.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_330.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6644 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_345.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_360.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_45.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_60.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_75.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6414 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_90.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_0.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_105.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_120.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_135.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_15.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_150.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_165.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_180.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_195.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_210.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_225.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_240.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_255.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_270.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_285.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_30.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_300.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6644 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_315.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_330.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_345.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_360.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_45.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_60.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_75.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_90.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_0.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_105.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_120.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_135.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_15.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_150.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_165.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_180.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_195.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_210.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_225.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_240.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_255.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_270.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_285.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_30.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_300.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_315.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_330.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_345.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_360.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_45.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_60.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_75.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_90.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_0.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_105.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_120.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_135.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_15.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_150.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_165.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_180.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_195.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_210.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_225.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6387 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_240.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_255.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_270.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_285.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_30.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_300.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_315.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_330.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_345.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_360.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_45.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_60.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_75.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6415 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_90.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 03:33:34.814236 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/
--rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_0.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_105.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_120.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_135.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_15.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_150.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_165.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_180.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_195.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_210.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_225.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_240.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_255.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_270.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_285.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_30.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_300.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_315.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_330.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_345.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_360.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_45.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_60.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_75.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_90.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_0.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_105.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_120.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_135.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_15.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_150.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_165.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_180.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_195.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_210.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_225.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_240.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_255.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_270.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_285.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_30.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_300.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_315.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_330.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_345.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_360.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_45.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_60.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_75.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_90.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_0.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_105.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_120.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_135.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_15.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6453 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_150.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_165.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_180.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_195.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_210.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_225.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_240.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_255.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6456 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_270.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_285.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_30.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_300.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_315.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_330.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_345.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_360.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_45.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_60.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_75.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_90.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_0.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_105.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_120.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_135.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_15.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_150.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_165.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_180.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_195.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_210.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_225.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_240.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_255.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_270.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_285.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_30.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_300.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6688 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_315.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_330.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_345.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_360.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_45.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_60.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_75.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6456 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_90.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 03:33:34.814236 mpltern-0.5.0/tests/baseline_images/test_tribin/
--rw-r--r--   0 runner    (1001) docker     (123)   114587 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_tribin/base.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    27785 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_tribin/extent.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   121032 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_tribin/given_triangles.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   115121 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/baseline_images/test_tribin/ternary_lim.pdf
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/hexbin_indices.txt
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/make_references.py
--rw-r--r--   0 runner    (1001) docker     (123)    25306 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/test_axis.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/test_constrainedlayout.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/test_given_triangles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/test_hexbin.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/test_hexbin_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/test_scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    18067 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/test_ternary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/test_text.py
--rw-r--r--   0 runner    (1001) docker     (123)    25669 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/test_tick.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/test_tightlayout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/test_triangle_rotation_axis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/test_triangle_rotation_horizontal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/test_triangle_rotation_tick.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/test_tribin.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/test_tribin_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-02-22 03:33:22.000000 mpltern-0.5.0/tests/tribin_indices.txt
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-02-22 03:33:22.000000 mpltern-0.5.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:32:31.680461 mpltern-1.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:32:31.608460 mpltern-1.0.0/.circleci/
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-06-11 14:32:22.000000 mpltern-1.0.0/.circleci/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-11 14:32:22.000000 mpltern-1.0.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:32:31.604460 mpltern-1.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:32:31.608460 mpltern-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-11 14:32:22.000000 mpltern-1.0.0/.github/workflows/publish-to-test-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-11 14:32:22.000000 mpltern-1.0.0/.github/workflows/tests.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1203 2023-06-11 14:32:22.000000 mpltern-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-11 14:32:22.000000 mpltern-1.0.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-11 14:32:22.000000 mpltern-1.0.0/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-11 14:32:22.000000 mpltern-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-11 14:32:22.000000 mpltern-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7032 2023-06-11 14:32:31.680461 mpltern-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-06-11 14:32:22.000000 mpltern-1.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:32:31.608460 mpltern-1.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-11 14:32:22.000000 mpltern-1.0.0/docs/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:32:31.612460 mpltern-1.0.0/docsrc/
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-11 14:32:22.000000 mpltern-1.0.0/docsrc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:32:31.612460 mpltern-1.0.0/docsrc/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-06-11 14:32:22.000000 mpltern-1.0.0/docsrc/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    10129 2023-06-11 14:32:22.000000 mpltern-1.0.0/docsrc/_static/logo_dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10129 2023-06-11 14:32:22.000000 mpltern-1.0.0/docsrc/_static/logo_light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-11 14:32:22.000000 mpltern-1.0.0/docsrc/_static/mpl.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-06-11 14:32:22.000000 mpltern-1.0.0/docsrc/alternatives.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-11 14:32:22.000000 mpltern-1.0.0/docsrc/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-11 14:32:22.000000 mpltern-1.0.0/docsrc/basic_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-06-11 14:32:22.000000 mpltern-1.0.0/docsrc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-06-11 14:32:22.000000 mpltern-1.0.0/docsrc/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-11 14:32:22.000000 mpltern-1.0.0/docsrc/corner_based_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50242 2023-06-11 14:32:22.000000 mpltern-1.0.0/docsrc/corner_based_1.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-11 14:32:22.000000 mpltern-1.0.0/docsrc/corner_based_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52879 2023-06-11 14:32:22.000000 mpltern-1.0.0/docsrc/corner_based_2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-11 14:32:22.000000 mpltern-1.0.0/docsrc/create_favicon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-06-11 14:32:22.000000 mpltern-1.0.0/docsrc/implemented_methods.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-11 14:32:22.000000 mpltern-1.0.0/docsrc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-11 14:32:22.000000 mpltern-1.0.0/docsrc/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-11 14:32:22.000000 mpltern-1.0.0/docsrc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-11 14:32:22.000000 mpltern-1.0.0/docsrc/matplotlibrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-11 14:32:22.000000 mpltern-1.0.0/docsrc/publications.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-11 14:32:22.000000 mpltern-1.0.0/docsrc/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-11 14:32:22.000000 mpltern-1.0.0/docsrc/side_based_ccw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54814 2023-06-11 14:32:22.000000 mpltern-1.0.0/docsrc/side_based_ccw.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-11 14:32:22.000000 mpltern-1.0.0/docsrc/side_based_cw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53409 2023-06-11 14:32:22.000000 mpltern-1.0.0/docsrc/side_based_cw.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:32:31.612460 mpltern-1.0.0/docsrc/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 14:32:22.000000 mpltern-1.0.0/docsrc/sphinxext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-06-11 14:32:22.000000 mpltern-1.0.0/docsrc/sphinxext/custom_roles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:32:31.612460 mpltern-1.0.0/docsrc/users/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-11 14:32:22.000000 mpltern-1.0.0/docsrc/users/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-11 14:32:22.000000 mpltern-1.0.0/docsrc/users/mpltern_1.0.0.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-06-11 14:32:22.000000 mpltern-1.0.0/docsrc/users/release_notes.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:32:31.612460 mpltern-1.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:32:31.616460 mpltern-1.0.0/examples/axis_and_tick/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/axis_and_tick/00.axis_label_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/axis_and_tick/01.axis_label_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/axis_and_tick/10.tick_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/axis_and_tick/11.tick_direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/axis_and_tick/12.tick_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/axis_and_tick/20.tick-formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/axis_and_tick/21.tick-locators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/axis_and_tick/30.manual_tick_positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/axis_and_tick/31.manual_ticklabels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/axis_and_tick/98.colored_axes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/axis_and_tick/99.tick_labels_inside_triangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/axis_and_tick/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:32:31.616460 mpltern-1.0.0/examples/intermediate/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/intermediate/00.with_normal_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/intermediate/01.style_sheets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/intermediate/99.inset.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/intermediate/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:32:31.616460 mpltern-1.0.0/examples/introductory/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/introductory/00.line_and_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/introductory/01.scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/introductory/02.contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/introductory/03.pseudocolor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/introductory/04.normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/introductory/05.span.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/introductory/06.text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/introductory/07.polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/introductory/08.quiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/introductory/09.grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/introductory/10.axis_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/introductory/11.triangular_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/introductory/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/introductory/axline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/introductory/legend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:32:31.616460 mpltern-1.0.0/examples/limits/
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/limits/00.triangular_limits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/limits/01.hexagonal_limits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/limits/02.fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/limits/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:32:31.620460 mpltern-1.0.0/examples/miscellaneous/
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/miscellaneous/00.logos.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/miscellaneous/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/miscellaneous/dirichlet_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/miscellaneous/evolutionary_game_theory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/miscellaneous/soil_texture.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:32:31.620460 mpltern-1.0.0/examples/statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/statistics/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/statistics/hexbin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/statistics/tribin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/statistics/with_scatter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:32:31.620460 mpltern-1.0.0/examples/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/transforms/00.cartesian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/transforms/01.ticks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/transforms/06.plot_fixed_onto_triangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/transforms/99.arrows_along_axes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/transforms/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:32:31.620460 mpltern-1.0.0/examples/triangle/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/triangle/00.aspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/triangle/01.triangle_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/triangle/02.arbitrary_triangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-11 14:32:22.000000 mpltern-1.0.0/examples/triangle/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:32:31.620460 mpltern-1.0.0/mpltern/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-11 14:32:22.000000 mpltern-1.0.0/mpltern/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-06-11 14:32:22.000000 mpltern-1.0.0/mpltern/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-06-11 14:32:22.000000 mpltern-1.0.0/mpltern/hexbin_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:32:31.624460 mpltern-1.0.0/mpltern/ternary/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-11 14:32:22.000000 mpltern-1.0.0/mpltern/ternary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28783 2023-06-11 14:32:22.000000 mpltern-1.0.0/mpltern/ternary/_axes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32750 2023-06-11 14:32:22.000000 mpltern-1.0.0/mpltern/ternary/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15738 2023-06-11 14:32:22.000000 mpltern-1.0.0/mpltern/ternary/axis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-11 14:32:22.000000 mpltern-1.0.0/mpltern/ternary/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-11 14:32:22.000000 mpltern-1.0.0/mpltern/ternary/spines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8675 2023-06-11 14:32:22.000000 mpltern-1.0.0/mpltern/ternary/tick.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18090 2023-06-11 14:32:22.000000 mpltern-1.0.0/mpltern/ternary/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-06-11 14:32:22.000000 mpltern-1.0.0/mpltern/ternary_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-06-11 14:32:22.000000 mpltern-1.0.0/mpltern/tribin_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:32:31.620460 mpltern-1.0.0/mpltern.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7032 2023-06-11 14:32:31.000000 mpltern-1.0.0/mpltern.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28691 2023-06-11 14:32:31.000000 mpltern-1.0.0/mpltern.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 14:32:31.000000 mpltern-1.0.0/mpltern.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-11 14:32:31.000000 mpltern-1.0.0/mpltern.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-11 14:32:31.000000 mpltern-1.0.0/mpltern.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-11 14:32:22.000000 mpltern-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-11 14:32:22.000000 mpltern-1.0.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 14:32:31.680461 mpltern-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-06-11 14:32:22.000000 mpltern-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:32:31.624460 mpltern-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/Dirichlet_PDF_1.0_2.0_2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/Dirichlet_PDF_1.5_1.5_1.5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/Dirichlet_PDF_2.0_4.0_8.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/Dirichlet_PDF_5.0_5.0_5.0.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:32:31.608460 mpltern-1.0.0/tests/baseline_images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:32:31.624460 mpltern-1.0.0/tests/baseline_images/test_constrainedlayout/
+-rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_constrainedlayout/constrained_layout1.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:32:31.628460 mpltern-1.0.0/tests/baseline_images/test_given_triangles/
+-rw-r--r--   0 runner    (1001) docker     (123)    11382 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_given_triangles/given_triangles_axis_0.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_given_triangles/given_triangles_axis_180.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_given_triangles/given_triangles_axis_270.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_given_triangles/given_triangles_axis_90.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_given_triangles/given_triangles_horizontal_0.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_given_triangles/given_triangles_horizontal_180.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    11337 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_given_triangles/given_triangles_horizontal_270.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    11364 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_given_triangles/given_triangles_horizontal_90.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    11382 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_given_triangles/given_triangles_tick_0.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    11378 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_given_triangles/given_triangles_tick_180.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_given_triangles/given_triangles_tick_270.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_given_triangles/given_triangles_tick_90.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:32:31.628460 mpltern-1.0.0/tests/baseline_images/test_hexbin/
+-rw-r--r--   0 runner    (1001) docker     (123)    18995 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_hexbin/base.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    11419 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_hexbin/extent.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    19493 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_hexbin/given_triangles.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    20041 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_hexbin/ternary_lim.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:32:31.632460 mpltern-1.0.0/tests/baseline_images/test_ternary/
+-rw-r--r--   0 runner    (1001) docker     (123)    10189 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_ternary/arguments_6.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_ternary/arguments_7.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_ternary/arrow_axes.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_ternary/arrow_data.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_ternary/arrow_xy_axes.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6386 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_ternary/arrow_xy_data.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    11059 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_ternary/aspect.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     8826 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_ternary/axis_label_position_corner.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     8832 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_ternary/axis_label_position_tick1.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     8839 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_ternary/axis_label_position_tick2.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_ternary/fit_none.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_ternary/fit_rectangle.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    10796 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_ternary/fit_triangle.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_ternary/legend.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_ternary/manual_ticklabels.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    11150 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_ternary/manual_ticks.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_ternary/negative_ticks.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_ternary/opposite_ticks.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_ternary/plot.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_ternary/quiver.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    16075 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_ternary/quiver_color.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    13098 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_ternary/quiver_xy_axes.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    12916 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_ternary/quiver_xy_data.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     9473 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_ternary/scatter.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    19943 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_ternary/scatter_color.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_ternary/spans.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    12043 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_ternary/test_ternary_lim-expected.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    65470 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_ternary/test_ternary_lim-expected.png
+-rw-r--r--   0 runner    (1001) docker     (123)    38681 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_ternary/test_ternary_lim-expected.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_ternary/test_ternary_lim-expected_pdf.png
+-rw-r--r--   0 runner    (1001) docker     (123)    63063 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_ternary/test_ternary_lim-expected_svg.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12043 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_ternary/test_ternary_lim.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    65470 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_ternary/test_ternary_lim.png
+-rw-r--r--   0 runner    (1001) docker     (123)    38681 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_ternary/test_ternary_lim.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_ternary/test_ternary_lim_pdf.png
+-rw-r--r--   0 runner    (1001) docker     (123)    63063 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_ternary/test_ternary_lim_svg.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_ternary/text.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_ternary/tick_direction_in.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_ternary/tick_direction_inout.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_ternary/tick_direction_out.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_ternary/tick_labels_inside_triangle.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_ternary/titie_center.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6887 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_ternary/titie_left.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_ternary/titie_right.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_ternary/transAxes.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:32:31.636460 mpltern-1.0.0/tests/baseline_images/test_tightlayout/
+-rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_tightlayout/tight_layout1.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:32:31.648460 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/
+-rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_0.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6693 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_105.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_120.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_135.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_15.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_150.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_165.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_180.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_195.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_210.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6693 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_225.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_240.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_255.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_270.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_285.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_30.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_300.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_315.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_330.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_345.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_360.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_45.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_60.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_75.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6473 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_90.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_0.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_105.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_120.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_135.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_15.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6476 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_150.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_165.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_180.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_195.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_210.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_225.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_240.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_255.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_270.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_285.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_30.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_300.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_315.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_330.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_345.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_360.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_45.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_60.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_75.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_90.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_0.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_105.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_120.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_135.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_15.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_150.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_165.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_180.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_195.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_210.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_225.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_240.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_255.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_270.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_285.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_30.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_300.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_315.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_330.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_345.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_360.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_45.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_60.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_75.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_90.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_0.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_105.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_120.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_135.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_15.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_150.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_165.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_180.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_195.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_210.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_225.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_240.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6688 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_255.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_270.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_285.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_30.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_300.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_315.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_330.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_345.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_360.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_45.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_60.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_75.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6480 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_90.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:32:31.660461 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/
+-rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_0.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_105.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_120.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_135.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_15.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_150.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_165.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_180.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6636 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_195.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_210.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_225.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_240.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_255.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_270.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_285.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_30.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_300.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_315.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_330.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6644 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_345.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_360.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_45.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_60.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_75.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6414 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_90.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_0.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_105.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_120.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_135.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_15.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_150.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_165.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_180.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_195.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_210.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_225.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_240.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_255.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_270.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_285.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_30.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_300.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6644 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_315.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_330.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_345.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_360.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_45.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_60.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_75.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_90.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_0.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_105.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_120.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_135.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_15.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_150.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_165.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_180.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_195.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_210.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_225.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_240.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_255.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_270.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_285.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_30.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_300.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_315.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_330.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_345.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_360.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_45.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_60.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_75.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_90.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_0.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_105.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_120.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_135.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_15.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_150.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_165.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_180.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_195.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_210.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_225.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6387 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_240.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_255.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_270.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_285.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_30.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_300.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_315.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_330.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_345.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_360.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_45.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_60.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_75.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6415 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_90.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:32:31.676461 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_0.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_105.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_120.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_135.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_15.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_150.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_165.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_180.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_195.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_210.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_225.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_240.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_255.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_270.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_285.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_30.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_300.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_315.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_330.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_345.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_360.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_45.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_60.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_75.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_90.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_0.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_105.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_120.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_135.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_15.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_150.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_165.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_180.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_195.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_210.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_225.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_240.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_255.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_270.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_285.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_30.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_300.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_315.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_330.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_345.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_360.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_45.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_60.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_75.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_90.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_0.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_105.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_120.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_135.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_15.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6453 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_150.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_165.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_180.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_195.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_210.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_225.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_240.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_255.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6456 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_270.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_285.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_30.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_300.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_315.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_330.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_345.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_360.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_45.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_60.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_75.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_90.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_0.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_105.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_120.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_135.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_15.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_150.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_165.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_180.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_195.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_210.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_225.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_240.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_255.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_270.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_285.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_30.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_300.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6688 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_315.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_330.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_345.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_360.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_45.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_60.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_75.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6456 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_90.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:32:31.680461 mpltern-1.0.0/tests/baseline_images/test_tribin/
+-rw-r--r--   0 runner    (1001) docker     (123)   114587 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_tribin/base.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    27785 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_tribin/extent.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   121032 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_tribin/given_triangles.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   115121 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/baseline_images/test_tribin/ternary_lim.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/hexbin_indices.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/make_references.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25306 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/test_axis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/test_constrainedlayout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/test_given_triangles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/test_hexbin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/test_hexbin_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/test_spines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25877 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/test_ternary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25669 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/test_tick.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/test_tightlayout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/test_triangle_rotation_axis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/test_triangle_rotation_horizontal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/test_triangle_rotation_tick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/test_tribin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/test_tribin_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-11 14:32:22.000000 mpltern-1.0.0/tests/tribin_indices.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-11 14:32:22.000000 mpltern-1.0.0/tox.ini
```

### Comparing `mpltern-0.5.0/.circleci/config.yml` & `mpltern-1.0.0/.circleci/config.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Use the latest 2.1 version of CircleCI pipeline process engine.
 # See: https://circleci.com/docs/2.0/configuration-reference
 version: 2.1
 
 orbs:
-  python: circleci/python@1.5.0
+  python: circleci/python@2.1.1
 
 # Define a job to be invoked later in a workflow.
 # See: https://circleci.com/docs/2.0/configuration-reference/#jobs
 jobs:
   build-and-test: # This is the name of the job, feel free to change it to better match what you're trying to do!
     parameters:
       matplotlib-version:
@@ -29,14 +29,15 @@
           command: |
             sudo apt -qq update
             sudo apt-get -y install ghostscript inkscape
       - run:
           name: Install dependencies
           command: |
             python -m pip install --upgrade pip
+            python -m pip install setuptools==59.8.0 # Matplotlib 3.4
             python -m pip install pillow==9.0
             python -m pip install matplotlib==<< parameters.matplotlib-version >>
             python -m pip install pytest>=4.6
             python -m pip install pytest-cov
             python -m pip install codecov coverage
       - run:
           name: Test with pytest
```

### Comparing `mpltern-0.5.0/.github/workflows/publish-to-test-pypi.yml` & `mpltern-1.0.0/.github/workflows/publish-to-test-pypi.yml`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/.github/workflows/tests.yml` & `mpltern-1.0.0/.github/workflows/tests.yml`

 * *Files 14% similar despite different names*

```diff
@@ -30,7 +30,9 @@
         python -m pip install matplotlib==${{ matrix.matplotlib-version }}
         python -m pip install pytest>=4.6
         python -m pip install pytest-cov
         python -m pip install codecov coverage
     - name: Test with pytest
       run: |
         python -mpytest -ra --cov=./ --log-level=DEBUG
+    - name: Upload code coverage
+      uses: codecov/codecov-action@v3
```

### Comparing `mpltern-0.5.0/.gitignore` & `mpltern-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/LICENSE` & `mpltern-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/docsrc/Makefile` & `mpltern-1.0.0/docsrc/Makefile`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/docsrc/_static/favicon.ico` & `mpltern-1.0.0/docsrc/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/docsrc/alternatives.rst` & `mpltern-1.0.0/docsrc/alternatives.rst`

 * *Files 6% similar despite different names*

```diff
@@ -70,51 +70,40 @@
 
 .. _Statgraphics: http://www.statgraphics.com
 .. Ternary plots are not documented very much.
 
 Open-source
 ===========
 
-Python_
--------
+- Python_
         - `Plotly <https://plot.ly/python>`__
         - `python-ternary <https://github.com/marcharper/python-ternary>`_
-
-R_
---
+- R_
         - `Plotly <https://plot.ly/r>`__
         - ggtern_
         - Ternary_
         - vcd_
 
-JavaScript_
------------
+- JavaScript_
         - Plotly_
         - `d3-ternary (TypeScript) <https://github.com/davenquinn/d3-ternary>`__
-
-LaTeX_
-------
+- LaTeX_
         - PGFPlots_
 
-GUI
----
+- GUI
         - Veusz_
 
-Online
-------
+- Online
         - ternaryplot.com_ (based on d3-ternary)
 
 Proprietary
 ===========
 
-MATLAB_
--------
+- MATLAB_
         - ternary-plots_
         - alcheyst-ternplot_
-
-GUI
----
+- GUI
         - `DPlot <https://www.dplot.com/index.htm>`_
         - Grapher_
         - JMP_
         - Origin_
         - Statgraphics_
```

### Comparing `mpltern-0.5.0/docsrc/api.rst` & `mpltern-1.0.0/docsrc/api.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-###
-API
-###
+API Reference
+=============
 
 This page is under construction. Only a few available methods are shown.
 
 .. autoclass:: mpltern.ternary.TernaryAxes
 
    .. automethod:: mpltern.ternary.TernaryAxes.set_tlabel
    .. automethod:: mpltern.ternary.TernaryAxes.set_llabel
```

### Comparing `mpltern-0.5.0/docsrc/basic_usage.rst` & `mpltern-1.0.0/docsrc/basic_usage.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,59 +1,72 @@
 ###########
 Basic Usage
 ###########
 
-Import mpltern as well as Matplotlib as:
+Import mpltern together with Matplotlib as:
 
-.. code-block:: python
+.. plot::
 
     import matplotlib.pyplot as plt
     import mpltern
 
-By ``import mpltern``, a Matplotlib projection ``'ternary'`` is
-registered inside.
+With this, the projection ``"ternary"`` is registered.
+Then, make `TernaryAxes`;
 
-Then, make ``TernaryAxes`` e.g. as:
+.. plot::
 
-.. code-block:: python
+    ax = plt.subplot(projection="ternary")
 
-    ax = plt.subplot(projection='ternary')
+You can use another normalization constant e.g. 100 using `ternary_sum`.
+Ternary-axis labels can be given using e.g. `ax.set_tlabel`.
+You can also add grids with `ax.grid`.
 
-It is already possible to create ternary plots using the methods in ``ax``.
-For example:
+.. plot::
 
-.. code-block:: python
+    ax = plt.subplot(projection="ternary", ternary_sum=100.0)
 
-    from mpltern.ternary.datasets import get_spiral
+    ax.set_tlabel("Top (%)")
+    ax.set_llabel("Left (%)")
+    ax.set_rlabel("Right (%)")
 
-    t, l, r = mpltern.datasets.get_spiral()
+    ax.grid()
+
+    plt.show()
+
+You can make ternary plots using methods similar to Matplotlib.
+You can e.g. use `ax.plot`;
+the only difference from Matplotlib is that you give three variables i.e.
+`t` (top), `l` (left), `r` (right) instead of `x` and `y`.
+
+.. plot::
+
+    from mpltern.datasets import get_spiral
+
+    ax = plt.subplot(projection="ternary")
+
+    t, l, r = get_spiral()
     # t: [0.33333333 0.33357906 0.33430414 ...]
     # l: [0.33333333 0.33455407 0.33543547 ...]
     # r: [0.33333333 0.33186687 0.33026039 ...]
     ax.plot(t, l, r)
-    plt.show()
-
-You may see the following Archimedean spiral in the triangle.
 
-.. image:: basic_1.svg
+    plt.show()
 
-Contour-like plots are also possible in mpltern.
+You can also make filled contour plots using `ax.tricontourf`.
 
-.. code-block:: python
+.. plot::
 
-    ax = plt.subplot(projection='ternary')
+    from mpltern.datasets import get_shanon_entropies
 
-    from mpltern.ternary.datasets import get_shanon_entropies
+    ax = plt.subplot(projection="ternary")
 
-    t, l, r, v = get_shanon_entropies()
+    t, l, r, entropies = get_shanon_entropies()
     # t: [ 0. 0.  0.  0.  0.  0.  0.  0.  0.  0.  0.  0.1 0.1 0.1 ...]
     # l: [ 0. 0.1 0.2 0.3 0.4 0.5 0.6 0.7 0.8 0.9 1.  0.  0.1 0.2 ...]
     # r: [ 1. 0.9 0.8 0.7 0.6 0.5 0.4 0.3 0.2 0.1 0.  0.9 0.8 0.7 ...]
     # v: [-0. 0.32508297  0.50040242  ...]
-    ax.tricontourf(t, l, r, v)
-    plt.show()
-
-.. image:: basic_2.svg
+    ax.tricontourf(t, l, r, entropies)
 
-See `more examples in the gallery
-<https://mpltern.readthedocs.io/en/latest/gallery/index.html>`__.
+    plt.show()
 
+There are more plotting methods and controls.
+:doc:`See examples <gallery/index>`.
```

### Comparing `mpltern-0.5.0/docsrc/conf.py` & `mpltern-1.0.0/docsrc/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,147 +9,193 @@
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 import os
 import shutil
 import sys
+import warnings
 
 sys.path.insert(0, os.path.abspath(".."))
 
+import mpltern
+
+from datetime import datetime
+import time
+
 from sphinx.transforms import SphinxTransform
 
-import mpltern
+# Parse year using SOURCE_DATE_EPOCH, falling back to current time.
+# https://reproducible-builds.org/specs/source-date-epoch/
+sourceyear = datetime.utcfromtimestamp(
+    int(os.environ.get('SOURCE_DATE_EPOCH', time.time()))).year
 
 
 # General configuration
 # ---------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
 extensions = [
     'sphinx.ext.autodoc',
+    'IPython.sphinxext.ipython_console_highlighting',
     'numpydoc',  # Needs to be loaded *after* autodoc.
     'sphinx_gallery.gen_gallery',
+    'matplotlib.sphinxext.plot_directive',
+    'sphinxext.custom_roles',
     'sphinx_copybutton',
 ]
 
 
 def _check_dependencies():
     names = {
+        **{ext: ext.split(".")[0] for ext in extensions},
+        # Explicitly list deps that are not extensions, or whose PyPI package
+        # name does not match the (toplevel) module name.
         "colorspacious": 'colorspacious',
-        "IPython.sphinxext.ipython_console_highlighting": 'ipython',
+        "pydata_sphinx_theme": 'pydata_sphinx_theme',
         "matplotlib": 'matplotlib',
-        "numpydoc": 'numpydoc',
-        "sphinx_copybutton": 'sphinx_copybutton',
-        "sphinx_gallery": 'sphinx_gallery',
     }
     missing = []
     for name in names:
         try:
             __import__(name)
         except ImportError:
             missing.append(names[name])
     if missing:
         raise ImportError(
             "The following dependencies are missing to build the "
-            "documentation: {}".format(", ".join(missing)))
+            f"documentation: {', '.join(missing)}")
     if shutil.which('dot') is None:
         raise OSError(
             "No binary named dot - graphviz must be installed to build the "
             "documentation")
 
-
 _check_dependencies()
 
 
 # On Linux, prevent plt.show() from emitting a non-GUI backend warning.
 os.environ.pop("DISPLAY", None)
 
 intersphinx_mapping = {
     'matplotlib': ('https://matplotlib.org/stable/', None),
 }
 
 
+# Sphinx gallery configuration
+
 from sphinx_gallery.scrapers import matplotlib_scraper
 
 
 class matplotlib_svg_scraper(object):
     # To make the figures in the SVG format
     # https://sphinx-gallery.github.io/advanced.html#id9
 
     def __repr__(self):
         return self.__class__.__name__
 
     def __call__(self, *args, **kwargs):
         return matplotlib_scraper(*args, format='svg', **kwargs)
 
 
-# Sphinx gallery configuration
 from sphinx_gallery.sorting import ExplicitOrder
 from sphinx_gallery.sorting import FileNameSortKey
+
+gallery_dirs = ['gallery']
+
+example_dirs = ['../examples']
 sphinx_gallery_conf = {
-    'examples_dirs': ['../examples'],
-    'filename_pattern': '^((?!sgskip).)*$',
-    'gallery_dirs': ['gallery'],
     'doc_module': ('mpltern', ),
+    'examples_dirs': example_dirs,
+    'filename_pattern': '^((?!sgskip).)*$',
+    'gallery_dirs': gallery_dirs,
+    # The following is commented out because SVG does not work nicely yet
+    # for `ax.pcolormesh(shading='gouraud')
+    'image_scrapers': (matplotlib_svg_scraper(),),
     'subsection_order': ExplicitOrder(['../examples/introductory',
                                        '../examples/intermediate',
                                        '../examples/statistics',
                                        '../examples/axis_and_tick',
+                                       '../examples/limits',
+                                       '../examples/transforms',
                                        '../examples/triangle',
-                                       '../examples/advanced',
                                        '../examples/miscellaneous']),
-    'within_subsection_order': FileNameSortKey,
     'min_reported_time': 1,
-    # The following is commented out because SVG does not work nicely yet
-    # for `ax.pcolormesh(shading='gouraud')
-    'image_scrapers': (matplotlib_svg_scraper(),),
+    'plot_gallery': 'True',  # sphinx-gallery/913
+    'within_subsection_order': FileNameSortKey,
+    'capture_repr': (),
 }
 
-plot_gallery = True
-
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The suffix of source filenames.
 source_suffix = '.rst'
 
 # This is the default encoding, but it doesn't hurt to be explicit
 source_encoding = "utf-8"
 
-# The master toctree document.
-master_doc = 'index'  # default: 'contents'
+# The toplevel toctree document (renamed to root_doc in Sphinx 4.0)
+root_doc = master_doc = 'index'
 
 project = 'mpltern'
-copyright = '2019-2023, Yuji Ikeda'
+copyright = (
+    f'2019-{sourceyear} Yuji Ikeda'
+)
 author = 'Yuji Ikeda'
 
+
+# The default replacements for |version| and |release|, also used in various
+# other places throughout the built documents.
+#
+# The short X.Y version.
+
 version = mpltern.__version__
 # The full version, including alpha/beta/rc tags.
 release = version
 
+# The name of the Pygments (syntax highlighting) style to use.
+pygments_style = 'sphinx'
+
+default_role = 'obj'
+
 # Plot directive configuration
 # ----------------------------
 
-plot_formats = [('png', 100), ('pdf', 100)]
+# https://matplotlib.org/stable/api/sphinxext_plot_directive_api.html
+plot_include_source = True
+plot_html_show_source_link = False
+plot_formats = ['svg']
+plot_html_show_formats = False
 
 # GitHub extension
 
 github_project_url = "https://github.com/yuzie007/mpltern/"
 
-# The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
 
-# -- Options for HTML output -------------------------------------------------
+# Options for HTML output
+# -----------------------
 
-# The theme to use for HTML and HTML Help pages.  See the documentation for
-# a list of builtin themes.
-#
-# html_theme = 'alabaster'
+# The style sheet to use for HTML and HTML Help pages. A file of that name
+# must exist either in Sphinx' static/ path, or in one of the custom paths
+# given in html_static_path.
+html_css_files = [
+    "mpl.css",
+]
+
+html_theme = "pydata_sphinx_theme"
+
+html_theme_options = {
+    "github_url": "https://github.com/yuzie007/mpltern",
+    "logo": {
+       "image_light": "_static/logo_light.svg",
+       "image_dark": "_static/logo_dark.svg",
+    },
+    "header_links_before_dropdown": 10,
+}
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ['_static']
 
 
@@ -190,23 +236,20 @@
     # app.add_css_file("screenshots.css")
     app.add_transform(ReplaceMyBase)
 
 
 # Path to favicon
 html_favicon = '_static/favicon.ico'
 
-html_logo = '_static/sphx_glr_logos0_002.svg'
-
 # numpydoc config
 
 numpydoc_show_class_members = False
 
 # Workaround to remove matplotlib warning based on
 # https://github.com/sphinx-gallery/sphinx-gallery/pull/521
 
 
-import warnings
 
 # Remove matplotlib agg warnings from generated doc when using plt.show
 warnings.filterwarnings("ignore", category=UserWarning,
                         message='Matplotlib is currently using agg, which is a'
                                 ' non-GUI backend, so cannot show the figure.')
```

### Comparing `mpltern-0.5.0/docsrc/conventions.rst` & `mpltern-1.0.0/docsrc/conventions.rst`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Conventions in mpltern
 ######################
 
 Axes and Ticks
 ==============
 
 In a ternary plot, three variables which sum to a constant
-``t + l + r = ternary_scale`` (= 1 in mpltern by default) are projected onto
+``t + l + r = ternary_sum`` (= 1 in mpltern by default) are projected onto
 a two-dimensional triangle.
 Each variable is associated with each corner of the triangle, and the value is
 represented by the scaled distance to the corner from its opposite side.
 
 There may be two kinds of perspectives to read a ternary plot; the
 "corner-based" and the "side-based" perspectives.
 **Mpltern adopts the "corner-based" perspective.**
@@ -18,15 +18,17 @@
 the triangle, and the position in the triangle is given as the scaled distance
 to the corner from its opposite side, as already written above.
 In mpltern, the order of the variables is ``T (top) → L (left) → R (right)``
 (counterclockwise).
 
 In mpltern, by default, the ticks are shown to the right side of the triangle
 with seeing the corresponding corner upward.
-You can put the ticks to the opposite sides by ``ax.opposite_ticks(True)``.
+You can put the ticks to the opposite sides using
+``ax.taxis.set_ticks_position("tick2")`` etc.
+(:doc:`See here <gallery/axis_and_tick/10.tick_position>`.)
 Notice that, although the tick positions are changed, still a point in the
 triangle corresponds to the same composition (see the red point).
 
 .. image:: corner_based_1.svg
 
 .. image:: corner_based_2.svg
 
@@ -81,14 +83,14 @@
 - ``T → L → R`` (CCW) for the order of triangle corners
 - CCW for the ticks progress
 
 Normalization in Ternary Plots
 ==============================
 
 In most plotting methods in mpltern, the given three variables are
-automatically normalized by ``ternary_scale``.
+automatically normalized by ``ternary_sum``.
 By this convention, the three variables can be treated on an equal footing.
 The exceptions are the span-plots like ``ax.axtline``.
 Since in these methods only one of the variables is given, in principle it is
-not possible whether the given value is already normalized or not.
+not possible to know whether the given value is already normalized or not.
 **To avoid confusions, it is strongly suggested to normalize the three
-variables beforehand outside mpltern.**
+variables on the user side.**
```

### Comparing `mpltern-0.5.0/docsrc/corner_based_1.py` & `mpltern-1.0.0/docsrc/corner_based_1.py`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/docsrc/corner_based_1.svg` & `mpltern-1.0.0/docsrc/corner_based_1.svg`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/docsrc/corner_based_2.py` & `mpltern-1.0.0/docsrc/corner_based_2.py`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/docsrc/corner_based_2.svg` & `mpltern-1.0.0/docsrc/corner_based_2.svg`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/docsrc/implemented_methods.rst` & `mpltern-1.0.0/docsrc/implemented_methods.rst`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/docsrc/installation.rst` & `mpltern-1.0.0/docsrc/installation.rst`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/docsrc/make.bat` & `mpltern-1.0.0/docsrc/make.bat`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/docsrc/publications.rst` & `mpltern-1.0.0/docsrc/publications.rst`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/docsrc/release_notes.rst` & `mpltern-1.0.0/docsrc/users/release_notes.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,113 +1,123 @@
 #############
 Release notes
 #############
 
-mpltern 0.5.0
-=============
+.. include:: mpltern_1.0.0.rst
+
+mpltern 0.5.0 (2023-02-22)
+==========================
 
 **Matplotlib 3.4.0-3.7.x**
 
+What's new
+----------
+
 ``ax.hexbin``
--------------
+^^^^^^^^^^^^^
 
 .. |ax.hexbin| replace:: ``ax.hexbin``
 .. _ax.hexbin: https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.hexbin.html
 
-|ax.hexbin|_ can now be used.
-See `gallery <https://mpltern.readthedocs.io/en/latest/gallery/statistics/hexbin.html>`__.
+|ax.hexbin|_ is now available.
+See :doc:`gallery <../gallery/statistics/hexbin>`.
 
 ``ax.tribin``
--------------
+^^^^^^^^^^^^^
 
-``ax.tribin`` can now be used.
-See `gallery <https://mpltern.readthedocs.io/en/latest/gallery/statistics/tribin.html>`__.
+``ax.tribin`` is now available.
+See :doc:`gallery <../gallery/statistics/tribin>`.
 
-mpltern 0.4.0
-=============
+mpltern 0.4.0 (2022-12-07)
+==========================
 
 **Matplotlib 3.4.0-3.6.x**
 
+What's new
+----------
+
 ``ax.axline``
--------------
+^^^^^^^^^^^^^
 
 .. |ax.axline| replace:: ``ax.axline``
 .. _ax.axline: https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.axline.html
 
 .. |matplotlib330| replace:: ``matplotlib>=3.3.0``
 .. _matplotlib330: https://matplotlib.org/stable/users/prev_whats_new/whats_new_3.3.0.html#new-axes-axline-method
 
-|ax.axline|_ can now be used for |matplotlib330|_ and mpltern.
-See `gallery <https://mpltern.readthedocs.io/en/latest/gallery/intermediate/axline.html>`__.
+|ax.axline|_ is now available together with |matplotlib330|_.
+See :doc:`gallery <../gallery/introductory/axline>`.
 
 ``tight_layout`` and ``constrained_layout``
--------------------------------------------
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Previously ``tight_layout`` and ``constrained_layout`` did not work as
 expected, which is fixed in mpltern 0.4.0.
 
 No overlaps between titles and ternary axes
--------------------------------------------
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 As done in Matplotlib.
 
+API Changes
+-----------
+
 Removal of ``opposite_ticks``
------------------------------
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Instead, ``ax.taxis.set_ticks_position`` and ``ax.taxis.set_label_position``
 etc. should be used explicitly.
-See `gallery <https://mpltern.readthedocs.io/en/latest/gallery/axis_and_tick/tick_position.html>`__.
+See :doc:`gallery <../gallery/axis_and_tick/10.tick_position>`.
 
 Drop support of ``python<3.7`` and ``matplotlib<3.4.0``
--------------------------------------------------------
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Python 3.6 is not maintained anymore.
 With Python 3.7, Matplotlib 3.4.0 is available.
 
-mpltern 0.3.5
-=============
+mpltern 0.3.5 (2022-09-24)
+==========================
 
 **Matplotlib 3.2.0-3.6.x**
 
-mpltern 0.3.4
-=============
+mpltern 0.3.4 (2021-11-29)
+==========================
 
 **Matplotlib 3.2.0-3.5.x**
 
 While essentially mpltern still works with Matplotlib 3.1.1, I got difficulty
 to make it pass the tests and therefore dropped the support.
 
-mpltern 0.3.3
-=============
+mpltern 0.3.3 (2021-03-28)
+==========================
 
 **Matplotlib 3.1.1-3.4.x**
 
-mpltern 0.3.2
-=============
+mpltern 0.3.2 (2020-10-29)
+==========================
 
 **Matplotlib 3.1.1-3.3.x**
 
 Update for conda-forge
 
-mpltern 0.3.1
-===============
+mpltern 0.3.1 (2020-07-18)
+==========================
 
 **Matplotlib 3.1.1-3.3.x**
 
-mpltern 0.3.0
-=============
+mpltern 0.3.0 (2019-11-01)
+==========================
 
 **Matplotlib 3.1.1-3.2.x**
 
 The tick-label rotation in mpltern relies on the rotation of the ``Text``
 object in Matplotlib.
 In Matplotlib 3.0 or lower, however, there was a bug for the ``Text`` rotation
 in case ``va=='center_baseline'`` and ``rotation_mode=='anchor'``
 (https://github.com/matplotlib/matplotlib/issues/13028).
 If these Matplotlib versions are used, tick-label positions are not as
 expected.
 **When using mpltern, therefore, it is strongly discouraged to use these old
 Matplotlib versions and instead suggested to use higher versions.**
-I however also have to note that Matplotlib 3.1 may also have other serious
-bugs (e.g. https://github.com/matplotlib/matplotlib/issues/14751).
-Until the versions where both the bugs are fixed, the users of mpltern have to
-compromise with these issues.
+
+Note that Matplotlib 3.1 had also other bugs
+(e.g. https://github.com/matplotlib/matplotlib/issues/14751).
```

### Comparing `mpltern-0.5.0/docsrc/side_based_ccw.py` & `mpltern-1.0.0/docsrc/side_based_ccw.py`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/docsrc/side_based_ccw.svg` & `mpltern-1.0.0/docsrc/side_based_ccw.svg`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/docsrc/side_based_cw.py` & `mpltern-1.0.0/docsrc/side_based_cw.py`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/docsrc/side_based_cw.svg` & `mpltern-1.0.0/docsrc/side_based_cw.svg`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/examples/advanced/00.colored_axes.py` & `mpltern-1.0.0/examples/axis_and_tick/98.colored_axes.py`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/examples/advanced/01.arrows_along_axes.py` & `mpltern-1.0.0/examples/transforms/99.arrows_along_axes.py`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/examples/advanced/03.manual_tick_positions.py` & `mpltern-1.0.0/examples/axis_and_tick/30.manual_tick_positions.py`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/examples/advanced/04.tick_labels_inside_triangle.py` & `mpltern-1.0.0/examples/axis_and_tick/99.tick_labels_inside_triangle.py`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/examples/advanced/05.inset.py` & `mpltern-1.0.0/examples/intermediate/99.inset.py`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/examples/advanced/06.plot_fixed_onto_triangle.py` & `mpltern-1.0.0/examples/transforms/06.plot_fixed_onto_triangle.py`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/examples/axis_and_tick/axis_label_position.py` & `mpltern-1.0.0/examples/axis_and_tick/00.axis_label_position.py`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/examples/axis_and_tick/axis_label_rotation.py` & `mpltern-1.0.0/examples/axis_and_tick/01.axis_label_rotation.py`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/examples/axis_and_tick/tick_position.py` & `mpltern-1.0.0/examples/axis_and_tick/10.tick_position.py`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/examples/intermediate/axline.py` & `mpltern-1.0.0/examples/introductory/axline.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 ======
 
 An infinitely long straight line can be added using ``ax.axline`` in a similar
 way as Matplotlib. This may be helpful, e.g., for adding an isoproportion line.
 
 .. note::
 
-    This is available with ``matplotlib>=3.3``.
+    Available with ``matplotlib>=3.3`` and ``mpltern>=0.4.0``
 
 Unlike Matplotlib, ``slope`` is the displacement from the first argument and
 must be of length 3, whose sum should be zero. The sum of the first argument
-and ``slope`` is automatically scaled by ``ternary_scale``.
+and ``slope`` is automatically scaled by ``ternary_sum``.
 
 With ``matplotlib>=3.4``, a keyword argument ``transform`` can be given.
-Particularly when ``ax.transTernaryAxes`` is given, a line fixed to the
+Particularly when `ax.transTernaryAxes` is given, a line fixed to the
 triangle can be added by giving the first and the second arguments in the
 barycentric coordinates.
 """
 import matplotlib.pyplot as plt
 import mpltern
 
 ax = plt.subplot(projection="ternary")
```

### Comparing `mpltern-0.5.0/examples/intermediate/with_normal_plots.py` & `mpltern-1.0.0/examples/intermediate/00.with_normal_plots.py`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/examples/introductory/01.scatter.py` & `mpltern-1.0.0/examples/introductory/01.scatter.py`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/examples/introductory/02.contour.py` & `mpltern-1.0.0/examples/introductory/02.contour.py`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/examples/introductory/03.pseudocolor.py` & `mpltern-1.0.0/examples/introductory/03.pseudocolor.py`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/examples/introductory/04.normalization.py` & `mpltern-1.0.0/examples/introductory/04.normalization.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """
 =============
 Normalization
 =============
 
-The normalization of ternary plots can be modified using ``ternary_scale``.
+The normalization constant of ternary plots can be modified using
+``ternary_sum``.
+
+.. warning::
+    Prior to mpltern 1.0.0, the option name was ``ternary_scale``.
 
 .. note::
     The ternary data are automatically normalized with a few exceptions.
     See details in :doc:`../../conventions`.
 """
 import matplotlib.pyplot as plt
 from mpltern.datasets import get_spiral
 
 
 fig = plt.figure()
-
-ternary_scale = 0.5
-ax = fig.add_subplot(projection='ternary', ternary_scale=ternary_scale)
-
+ax = fig.add_subplot(projection='ternary', ternary_sum=100.0)
 t, l, r = get_spiral()
-
-ax.plot(t, l, r)  # Data are automatically normalized by `ternary_scale`.
-
+ax.plot(t, l, r)  # Data are automatically normalized by ``ternary_sum``.
 plt.show()
```

### Comparing `mpltern-0.5.0/examples/introductory/05.span.py` & `mpltern-1.0.0/examples/introductory/05.span.py`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/examples/introductory/07.polygon.py` & `mpltern-1.0.0/examples/introductory/07.polygon.py`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/examples/introductory/08.quiver.py` & `mpltern-1.0.0/examples/introductory/08.quiver.py`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/examples/miscellaneous/dirichlet_pdf.py` & `mpltern-1.0.0/examples/miscellaneous/dirichlet_pdf.py`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/examples/statistics/hexbin.py` & `mpltern-1.0.0/examples/statistics/hexbin.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,35 @@
 """
 ======
 HexBin
 ======
 
-``ax.hexbin`` is a 2D histogram plot, in which the bins are hexagons and
+`ax.hexbin` is a 2D histogram plot, in which the bins are hexagons and
 the color represents the number of data points within each bin.
+Unlike Matplotlib, `gridsize` (by default 100) can be only a single int.
 
-Unlike Matplotlib, `gridsize` can be only a single int.
+.. note::
+
+    Available with ``mpltern>=0.5.0``
 """
 import numpy as np
 
 import matplotlib.pyplot as plt
 import mpltern
 
 np.random.seed(19680801)
 t, l, r = np.random.dirichlet(alpha=(2.0, 4.0, 8.0), size=100000).T
+
+# %%
 ax = plt.subplot(projection="ternary")
-# If "face" (default), small hexagons look overlapping with each other.
+
+# If "edgecolors=face" (default), small hexagons look overlapping.
 ax.hexbin(t, l, r, edgecolors="none")
 
 plt.show()
+
+# %%
+ax = plt.subplot(projection="ternary")
+
+ax.hexbin(t, l, r, bins="log", edgecolors="none")
+
+plt.show()
```

### Comparing `mpltern-0.5.0/examples/statistics/with_scatter.py` & `mpltern-1.0.0/examples/statistics/with_scatter.py`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/examples/triangle/01.triangle_rotation.py` & `mpltern-1.0.0/examples/triangle/01.triangle_rotation.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 The triangle for a ternary plot can be rotated by `rotation`.
 Axis labels, tick labels, and tick markers are also automatically aligned.
 """
 import matplotlib.pyplot as plt
 from mpltern.datasets import get_spiral
 
 
-pad = 42
-
 t, l, r = get_spiral()
 
 fig = plt.figure(figsize=(10.8, 8.8))
 fig.subplots_adjust(
-    left=0.1, right=0.9, bottom=0.1, top=0.9, wspace=0.5, hspace=0.5)
+    left=0.1,
+    right=0.9,
+    hspace=0.75,
+)
 
 rotations = range(0, 360, 90)
 for i, rotation in enumerate(rotations):
     ax = fig.add_subplot(2, 2, i + 1, projection='ternary', rotation=rotation)
 
     ax.plot(t, l, r)
 
     ax.set_tlabel('Top')
     ax.set_llabel('Left')
     ax.set_rlabel('Right')
 
-    ax.set_title("rotation={}".format(rotation), pad=pad)
+    ax.set_title(f"rotation={rotation}")
 
 plt.show()
```

### Comparing `mpltern-0.5.0/mpltern/__init__.py` & `mpltern-1.0.0/mpltern/__init__.py`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/mpltern/hexbin_helpers.py` & `mpltern-1.0.0/mpltern/hexbin_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
-from typing import Tuple
+from typing import Sequence
 
 
-def calc_ternary_indices(t, l, r, gridsize: int, extent: Tuple[float]):
+def calc_ternary_indices(t, l, r, gridsize: int, extent: Sequence[float]):
     tmin, tmax, lmin, lmax, rmin, rmax = extent
 
     # side lengths along ternary axes
     st = (tmax - tmin) / gridsize
     sl = (lmax - lmin) / gridsize
     sr = (rmax - rmin) / gridsize
 
@@ -89,15 +89,15 @@
     tmpl = (0 <= il) & (il <= gridsize)
     tmpr = (0 <= ir) & (ir <= gridsize)
     is_inside = tmpt & tmpl & tmpr
     i = (gridsize - it) * (gridsize - it + 1) // 2 + ir
     return np.where(is_inside, i, -1)
 
 
-def serial_to_ternary(gridsize: int, i: int) -> Tuple[int]:
+def serial_to_ternary(gridsize: int, i: int) -> Sequence[int]:
     """Convert ternary indices of hexagons to serial index.
 
     Parameters
     ----------
     gridsize : int
         Grid size.
     i : int
```

### Comparing `mpltern-0.5.0/mpltern/ternary/_axes.py` & `mpltern-1.0.0/mpltern/ternary/_axes.py`

 * *Files 1% similar despite different names*

```diff
@@ -507,20 +507,20 @@
         polygon -= offsets[0]
 
         if True:
             # While `offset_transform` is introduced since `matplotlib>=3.6.0`,
             # here an alias `transOffset` is used for backword compatibility.
             # see matplotlib/matplotlib#21965
             collection = mcoll.PolyCollection(
-            [polygon],
-            edgecolors=edgecolors,
-            linewidths=linewidths,
-            offsets=offsets,
-            transOffset=mtransforms.AffineDeltaTransform(self.transData),
-        )
+                [polygon],
+                edgecolors=edgecolors,
+                linewidths=linewidths,
+                offsets=offsets,
+                transOffset=mtransforms.AffineDeltaTransform(self.transData),
+            )
 
         # Set normalizer if bins is 'log'
         if bins == 'log':
             if norm is not None:
                 _api.warn_external("Only one of 'bins' and 'norm' arguments "
                                    f"can be supplied, ignoring bins={bins}")
             else:
@@ -794,14 +794,18 @@
     def arrow(self, *args, **kwargs):
         return super().arrow(*args, **kwargs)
 
     @_parse_ternary_vector_field
     def quiver(self, *args, **kwargs):
         return super().quiver(*args, **kwargs)
 
+    @_parse_ternary_vector_field
+    def barbs(self, *args, **kwargs):
+        return super().barbs(*args, **kwargs)
+
     @_parse_ternary_multiple
     def fill(self, *args, **kwargs):
         return super().fill(*args, **kwargs)
 
     @_parse_ternary_single
     def hist2d(self, *args, **kwargs):
         return super().hist2d(*args, **kwargs)
```

### Comparing `mpltern-0.5.0/mpltern/ternary/_base.py` & `mpltern-1.0.0/mpltern/ternary/_base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import logging
-from collections import OrderedDict
+import warnings
 
 import numpy as np
 
 import matplotlib as mpl
 import matplotlib.cbook as cbook
 import matplotlib.patches as mpatches
 import matplotlib.transforms as mtransforms
 import matplotlib.axis as maxis
 from matplotlib.axes import Axes
 from matplotlib import _api
 from mpltern.ternary.spines import Spine
 from mpltern.ternary.transforms import (
-    TernaryTransform, TernaryPerpendicularTransform,
-    BarycentricTransform, TernaryScaleTransform, TernaryShift)
+    TernaryAxisTransform, TernaryTickLabelShift,
+    TernaryAxisLabelSTransform, TernaryAxisLabelCTransform,
+    H2THeightTransform, H2TWidthTransform,
+    BarycentricTransform, TernaryScaleTransform)
 from mpltern.ternary.axis import TAxis, LAxis, RAxis
 
 _log = logging.getLogger(__name__)
 
 
 def _create_corners(corners=None, rotation=None):
     if corners is None:
@@ -39,50 +41,62 @@
         corners = trans.transform(corners)
         # The following shift places the triangle inside the original
         # square `Axes` as much as possible.
         tmp = (np.min(corners, axis=0) + np.max(corners, axis=0)) * 0.5
         corners += (np.array([0.0, 0.5]) - tmp)
     return corners
 
+
 class TernaryAxesBase(Axes):
     _axis_names = ("x", "y", "t", "l", "r")
     _shared_axes = {name: cbook.Grouper() for name in _axis_names}
 
-    def __init__(self, *args, ternary_scale=1.0, corners=None, rotation=None,
-                 **kwargs):
+    def __init__(self, *args, ternary_sum: float = 1.0, corners=None,
+                 rotation: float = None, **kwargs):
         """Build an TernaryAxes in a figure.
 
         Parameters
         ----------
-        ternary_scale : float, optional
-            ``t + l + r``, by default 1.0
+        ternary_sum : float, optional
+            Constant to which ``t + l + r`` is normalized, by default 1.0
         corners : Sequence[float] or None, optional
             Corners of the triangle, by default None
         rotation : float or None, optional
             Rotation angle of the triangle, by default None
         """
+        if "ternary_scale" in kwargs:
+            warnings.warn(
+                "Since mpltern 1.0.0, the normalization constant for a "
+                "ternary plot has been renamed from `ternary_scale` to "
+                "`ternary_sum`. Use the latter."
+            )
+            ternary_sum = kwargs.pop("ternary_scale")
+
         # workaround for matplotlib>=3.6.0
         self._sharet = None
         self._sharel = None
         self._sharer = None
 
         # Triangle corners in the original data coordinates
         self.corners_data = _create_corners(corners, rotation)
         sx = np.sqrt(3.0) * 0.5  # Scale for x
         xmin = -1.0 / np.sqrt(3.0)
         v = xmin * sx
         trans = mtransforms.Affine2D().from_values(sx, 0.0, 0.0, 1.0, -v, 0.0)
         # Triangle corners in the original ``Axes`` coordinates
         self.corners_axes = trans.transform(self.corners_data)
 
-        self.ternary_scale = ternary_scale
+        self.ternary_sum = ternary_sum
         super().__init__(*args, **kwargs)
         self.set_aspect('equal', adjustable='box', anchor='C')
         self.set_ternary_lim(
-            0.0, ternary_scale, 0.0, ternary_scale, 0.0, ternary_scale)
+            0.0, ternary_sum,
+            0.0, ternary_sum,
+            0.0, ternary_sum,
+        )
 
     @property
     def callbacks(self):
         if tuple(int(_) for _ in mpl.__version__.split('.'))[:2] < (3, 6):
             return cbook.CallbackRegistry()
         else:
             return cbook.CallbackRegistry(
@@ -92,14 +106,17 @@
     def callbacks(self, value):
         pass
 
     def set_figure(self, fig):
         self.viewTLim = mtransforms.Bbox.unit()
         self.viewLLim = mtransforms.Bbox.unit()
         self.viewRLim = mtransforms.Bbox.unit()
+        self.viewOuterTLim = mtransforms.Bbox.unit()
+        self.viewOuterLLim = mtransforms.Bbox.unit()
+        self.viewOuterRLim = mtransforms.Bbox.unit()
         super().set_figure(fig)
 
     def _get_axis_list(self):
         return tuple(getattr(self, f"{name}axis") for name in self._axis_names)
 
     def _get_axis_map(self):
         # workaround for matplotlib>=3.4.0
@@ -122,137 +139,164 @@
         self.laxis = LAxis(self)
         self.raxis = RAxis(self)
 
         self.spines['tside'].register_axis(self.taxis)
         self.spines['lside'].register_axis(self.laxis)
         self.spines['rside'].register_axis(self.raxis)
 
+        self.spines['tcorner'].register_axis(self.taxis)
+        self.spines['lcorner'].register_axis(self.laxis)
+        self.spines['rcorner'].register_axis(self.raxis)
+
         self._update_transScale()
 
     def _set_lim_and_transforms(self):
         super()._set_lim_and_transforms()
-        transTernaryScale = TernaryScaleTransform(self.ternary_scale)
+        transTernaryScale = TernaryScaleTransform(self.ternary_sum)
         transTLimits = mtransforms.BboxTransformFrom(
-            mtransforms.TransformedBbox(self.viewTLim, self.transScale))
+            mtransforms.TransformedBbox(self.viewOuterTLim, self.transScale))
         transLLimits = mtransforms.BboxTransformFrom(
-            mtransforms.TransformedBbox(self.viewLLim, self.transScale))
+            mtransforms.TransformedBbox(self.viewOuterLLim, self.transScale))
         transRLimits = mtransforms.BboxTransformFrom(
-            mtransforms.TransformedBbox(self.viewRLim, self.transScale))
+            mtransforms.TransformedBbox(self.viewOuterRLim, self.transScale))
 
         corners_axes = self.corners_axes
 
-        taxis_transform = TernaryTransform(corners_axes, 0)
-        laxis_transform = TernaryTransform(corners_axes, 1)
-        raxis_transform = TernaryTransform(corners_axes, 2)
-
-        self._taxis_transform = transTLimits + taxis_transform + self.transAxes
-        self._laxis_transform = transLLimits + laxis_transform + self.transAxes
-        self._raxis_transform = transRLimits + raxis_transform + self.transAxes
-
-        # For axis labels
-        t_l_t = TernaryPerpendicularTransform(self.transAxes, corners_axes, 0)
-        l_l_t = TernaryPerpendicularTransform(self.transAxes, corners_axes, 1)
-        r_l_t = TernaryPerpendicularTransform(self.transAxes, corners_axes, 2)
-        self._taxis_label_transform = t_l_t
-        self._laxis_label_transform = l_l_t
-        self._raxis_label_transform = r_l_t
+        ternary_limits = [self.viewTLim, self.viewLLim, self.viewRLim]
+
+        h2t_h_t = H2THeightTransform(self.ternary_sum, ternary_limits, 0)
+        h2t_h_l = H2THeightTransform(self.ternary_sum, ternary_limits, 1)
+        h2t_h_r = H2THeightTransform(self.ternary_sum, ternary_limits, 2)
+
+        h2t_w_t = H2TWidthTransform(self.ternary_sum, ternary_limits, 0)
+        h2t_w_l = H2TWidthTransform(self.ternary_sum, ternary_limits, 1)
+        h2t_w_r = H2TWidthTransform(self.ternary_sum, ternary_limits, 2)
+
+        h2t_t = h2t_h_t + h2t_w_t
+        h2t_l = h2t_h_l + h2t_w_l
+        h2t_r = h2t_h_r + h2t_w_r
+
+        # From scaled ternary-axis coordinates to display coordinates
+        taxis_tr = TernaryAxisTransform(corners_axes, 0) + self.transAxes
+        laxis_tr = TernaryAxisTransform(corners_axes, 1) + self.transAxes
+        raxis_tr = TernaryAxisTransform(corners_axes, 2) + self.transAxes
+
+        # For ticks and spines
+        self._taxis_transform = transTLimits + h2t_w_t + taxis_tr
+        self._laxis_transform = transLLimits + h2t_w_l + laxis_tr
+        self._raxis_transform = transRLimits + h2t_w_r + raxis_tr
+
+        # For axis labels (to display coordinates)
+        self._tlabel_s_transform = TernaryAxisLabelSTransform(taxis_tr, h2t_t)
+        self._llabel_s_transform = TernaryAxisLabelSTransform(laxis_tr, h2t_l)
+        self._rlabel_s_transform = TernaryAxisLabelSTransform(raxis_tr, h2t_r)
+        self._tlabel_c_transform = TernaryAxisLabelCTransform(taxis_tr, h2t_t)
+        self._llabel_c_transform = TernaryAxisLabelCTransform(laxis_tr, h2t_l)
+        self._rlabel_c_transform = TernaryAxisLabelCTransform(raxis_tr, h2t_r)
 
         # From ternary coordinates to the original data coordinates
         self.transProjection = (transTernaryScale
                                 + BarycentricTransform(self.corners_data))
 
         # From ternary coordinates to the original Axes coordinates
         self._ternary_axes_transform = self.transProjection + self.transLimits
 
+        # From ternary coordinates to display coordinates
+        self._ternary2display_transform = self.transProjection + self.transData
+
         # From barycentric coordinates to the original Axes coordinates
-        self.transAxesProjection = BarycentricTransform(self.corners_axes)
+        self.transAxesProjection = BarycentricTransform(corners_axes.copy())
 
         # From barycentric coordinates to display coordinates
         self.transTernaryAxes = self.transAxesProjection + self.transAxes
 
+        # From outer Axes coordinates to display coordinates
+        self._outer_position = mtransforms.Bbox.unit()
+        self.transOuterAxes = (
+            mtransforms.BboxTransformTo(self._outer_position) + self.transAxes)
+
     def get_xaxis_transform(self, which='grid'):
         # Overridden not to call spines
         return self._xaxis_transform
 
     def get_yaxis_transform(self, which='grid'):
         # Overridden not to call spines
         return self._yaxis_transform
 
     def get_taxis_transform(self, which='grid'):
-        if which == 'label':
-            return self._taxis_label_transform
-        else:
-            return self._taxis_transform
+        """Get the transformation for drawing t-axis ticks and gridlines."""
+        return self._taxis_transform
 
     def get_laxis_transform(self, which='grid'):
-        if which == 'label':
-            return self._laxis_label_transform
-        else:
-            return self._laxis_transform
+        """Get the transformation for drawing l-axis ticks and gridlines."""
+        return self._laxis_transform
 
     def get_raxis_transform(self, which='grid'):
-        if which == 'label':
-            return self._raxis_label_transform
-        else:
-            return self._raxis_transform
+        """Get the transformation for drawing r-axis ticks and gridlines."""
+        return self._raxis_transform
 
     def _get_axis_text_transform(self, pad_points, trans, indices):
-        pad_shift = TernaryShift(indices, self.figure, self.axes, pad_points)
+        pad_shift = TernaryTickLabelShift(self, pad_points, indices)
         # `va` and `ha` are modified in `TernaryTick`
         return trans + pad_shift, 'top', 'center'
 
     def get_taxis_text1_transform(self, pad_points):
+        """Get the transformation for drawing t-axis tick-labels."""
         trans = self.get_taxis_transform(which='tick1')
         return self._get_axis_text_transform(pad_points, trans, [1, 2])
 
     def get_taxis_text2_transform(self, pad_points):
+        """Get the transformation for drawing t-axis tick-labels."""
         trans = self.get_taxis_transform(which='tick2')
         return self._get_axis_text_transform(pad_points, trans, [2, 1])
 
     def get_laxis_text1_transform(self, pad_points):
+        """Get the transformation for drawing l-axis tick-labels."""
         trans = self.get_laxis_transform(which='tick1')
         return self._get_axis_text_transform(pad_points, trans, [2, 0])
 
     def get_laxis_text2_transform(self, pad_points):
+        """Get the transformation for drawing l-axis tick-labels."""
         trans = self.get_laxis_transform(which='tick2')
         return self._get_axis_text_transform(pad_points, trans, [0, 2])
 
     def get_raxis_text1_transform(self, pad_points):
+        """Get the transformation for drawing r-axis tick-labels."""
         trans = self.get_raxis_transform(which='tick1')
         return self._get_axis_text_transform(pad_points, trans, [0, 1])
 
     def get_raxis_text2_transform(self, pad_points):
+        """Get the transformation for drawing r-axis tick-labels."""
         trans = self.get_raxis_transform(which='tick2')
         return self._get_axis_text_transform(pad_points, trans, [1, 0])
 
     def _gen_axes_patch(self):
-        return mpatches.Polygon(self.corners_axes)
+        return mpatches.Polygon(np.repeat(self.corners_axes, 2, axis=0))
 
     def _gen_axes_spines(self, locations=None, offset=0.0, units='inches'):
-        # Use `Spine` in `mpltern`
-        spines = OrderedDict((side, Spine.linear_spine(self, side))
-                             for side in ['tside', 'lside', 'rside'])
-        return spines
+        # overridden to use `Spine` in `mpltern`
+        return {side: Spine.linear_spine(self, side) for side in
+                ['tside', 'tcorner', 'lside', 'lcorner', 'rside', 'rcorner']}
 
     def get_taxis(self):
         """Return the TAxis instance"""
         return self.taxis
 
     def get_laxis(self):
         """Return the LAxis instance"""
         return self.laxis
 
     def get_raxis(self):
         """Return the RAxis instance"""
         return self.raxis
 
     def clear(self):
-        self.set_tlim(0.0, self.ternary_scale)
-        self.set_llim(0.0, self.ternary_scale)
-        self.set_rlim(0.0, self.ternary_scale)
+        self.viewTLim.intervalx = 0.0, self.ternary_sum
+        self.viewLLim.intervalx = 0.0, self.ternary_sum
+        self.viewRLim.intervalx = 0.0, self.ternary_sum
         if tuple(int(_) for _ in mpl.__version__.split('.'))[:2] < (3, 6):
             super().cla()
         else:
             super().clear()
         xmin = -1.0 / np.sqrt(3.0)
         xmax = +1.0 / np.sqrt(3.0)
         self.set_xlim(xmin, xmax)
@@ -571,95 +615,196 @@
                 'center': 0.5,
                 'right': 1,
             }[loc]
             kwargs.update(x=x, horizontalalignment=loc)
 
         return self.raxis.set_label_text(rlabel, fontdict, **kwargs)
 
-    def _create_bbox_from_ternary_lim(self):
+    def _get_hexagonal_vertices(self):
+        """Get vertices of the view-limit hexagon."""
         tmin, tmax = self.get_tlim()
         lmin, lmax = self.get_llim()
         rmin, rmax = self.get_rlim()
-        points = [[tmax, lmin, rmin], [tmin, lmax, rmin], [tmin, lmin, rmax]]
-        points = self.transProjection.transform(points)
+        return [
+            [tmax, lmin, self.ternary_sum - tmax - lmin],
+            [tmax, self.ternary_sum - tmax - rmin, rmin],
+            [self.ternary_sum - lmax - rmin, lmax, rmin],
+            [tmin, lmax, self.ternary_sum - lmax - tmin],
+            [tmin, self.ternary_sum - rmax - tmin, rmax],
+            [self.ternary_sum - rmax - lmin, lmin, rmax],
+        ]
+
+    def _get_triangular_vertices(self):
+        """Get vertices of the extrapolative triangle."""
+        tmin = self.get_tlim()[0]
+        lmin = self.get_llim()[0]
+        rmin = self.get_rlim()[0]
+        return [
+            [self.ternary_sum - lmin - rmin, lmin, rmin],
+            [tmin, self.ternary_sum - rmin - tmin, rmin],
+            [tmin, lmin, self.ternary_sum - tmin - lmin],
+        ]
+
+    def _create_bbox_from_ternary_lim(self, fit: str = "rectangle"):
+        if fit == "rectangle":
+            tlr = self._get_hexagonal_vertices()
+        elif fit == "triangle":
+            tlr = self._get_triangular_vertices()
+        elif fit == "none":
+            tlr = [
+                [self.ternary_sum, 0.0, 0.0],
+                [0.0, self.ternary_sum, 0.0],
+                [0.0, 0.0, self.ternary_sum],
+            ]
+        else:
+            raise ValueError(f'unknown fit: {fit}')
+        xy = self.transProjection.transform(tlr)
         bbox = mtransforms.Bbox.unit()
-        bbox.update_from_data_xy(points, ignore=True)
+        bbox.update_from_data_xy(xy, ignore=True)
         return bbox
 
-    def set_ternary_lim(self, tmin, tmax, lmin, lmax, rmin, rmax, *args, **kwargs):
-        """
+    def set_ternary_lim(
+        self, tmin, tmax, lmin, lmax, rmin, rmax, fit: str = "rectangle"
+    ):
+        """Set ternary limits.
 
-        Notes
-        -----
-        xmin, xmax : holizontal limits of the triangle
-        ymin, ymax : bottom and top of the triangle
-        """
-        t = tmax + lmin + rmin
-        l = tmin + lmax + rmin
-        r = tmin + lmin + rmax
-        s = self.ternary_scale
-        tol = 1e-12
-        if (abs(t - s) > tol) or (abs(l - s) > tol) or (abs(r - s) > tol):
-            raise ValueError(t, l, r, s)
-
-        boxin = self._create_bbox_from_ternary_lim()
-
-        self.set_tlim(tmin, tmax)
-        self.set_llim(lmin, lmax)
-        self.set_rlim(rmin, rmax)
+        Parameters
+        ----------
+        fit : {"rectangle", "triangle", "none"}
+            To what the plotting region is fitted.
+
+            - ``'rectangle'``: Fitted to the original rectangle.
+            - ``'triangle'``: Fitted to the original triangle.
+            - ``'none'``: The plotting region is simply cropped (or expanded).
+        """
+        _api.check_in_list(['rectangle', 'triangle', 'none'], fit=fit)
+        if np.sign(tmax - tmin) != np.sign(self.ternary_sum):
+            tmin, tmax = tmax, tmin
+        if np.sign(lmax - lmin) != np.sign(self.ternary_sum):
+            lmin, lmax = lmax, lmin
+        if np.sign(rmax - rmin) != np.sign(self.ternary_sum):
+            rmin, rmax = rmax, rmin
+
+        boxin = self._create_bbox_from_ternary_lim("none")
+
+        self._set_ternary_lim(tmin, tmax, lmin, lmax, rmin, rmax)
 
-        boxout = self._create_bbox_from_ternary_lim()
+        boxout = self._create_bbox_from_ternary_lim(fit)
 
         trans = mtransforms.BboxTransform(boxin, boxout)
 
-        xmin, xmax = self.get_xlim()
-        ymin, ymax = self.get_ylim()
-        points = [[xmin, ymin], [xmax, ymax]]
-        ((xmin, ymin), (xmax, ymax)) = trans.transform(points)
+        points = [[-0.5 / np.sqrt(3.0), 0.0], [+0.5 / np.sqrt(3.0), 1.0]]
 
-        self.set_xlim(xmin, xmax)
-        self.set_ylim(ymin, ymax)
+        # Expand xlim or ylim to keep:
+        # - the original Axes ratio
+        # - the same x/y aspect (by default equal, modified by set_aspect)
+        # - the position of the hexagon to the center of Axes
+        bbox = mtransforms.Bbox.unit()
+        bbox.update_from_data_xy(trans.transform(points))
+        aspect = 0.5 * np.sqrt(3.0)
+        if isinstance(self.get_aspect(), float):
+            aspect *= self.get_aspect()
+        tmp = aspect / (bbox.height / bbox.width)
+        if bbox.height / bbox.width < aspect:
+            bbox = bbox.expanded(1.0, tmp)
+        else:
+            bbox = bbox.expanded(1.0 / tmp, 1.0)
+        self.set_xlim(bbox.x0, bbox.x1)
+        self.set_ylim(bbox.y0, bbox.y1)
+
+        self._update_axes_patch()
+        self._update_triangular_vertices()
+
+    def _update_axes_patch(self):
+        tlr = self._get_hexagonal_vertices()
+        xy = self._ternary_axes_transform.transform(tlr)
+        self.patch.set_xy(xy)
+
+    def _update_triangular_vertices(self):
+        tlr = self._get_triangular_vertices()
+        xy = self._ternary_axes_transform.transform(tlr)
+        # Update the corner positions in axes coordinates.
+        # Indexing is necessary to keep the object ID.
+        self.corners_axes[:, :] = xy
+        self._outer_position.update_from_data_xy(xy)
+
+    def _set_ternary_lim(self, tmin, tmax, lmin, lmax, rmin, rmax):
+        """Set ternary limits.
+
+        Notes
+        -----
+        The given ternary limits may be further modified to show intersections
+        of (tmin, tmax), (lmin, lmax), (rmin, rmax).
+        """
+        tn_sum = self.ternary_sum
+
+        select_min, select_max = (max, min) if tn_sum > 0.0 else (min, max)
 
-    def set_ternary_min(self, tmin, lmin, rmin, *args, **kwargs):
-        s = self.ternary_scale
-        tmax = s - lmin - rmin
-        lmax = s - rmin - tmin
-        rmax = s - tmin - lmin
-        self.set_ternary_lim(tmin, tmax, lmin, lmax, rmin, rmax, *args, **kwargs)
-
-    def set_ternary_max(self, tmax, lmax, rmax, *args, **kwargs):
-        s = self.ternary_scale
-        tmin = (s + tmax - lmax - rmax) * 0.5
-        lmin = (s + lmax - rmax - tmax) * 0.5
-        rmin = (s + rmax - tmax - lmax) * 0.5
-        self.set_ternary_lim(tmin, tmax, lmin, lmax, rmin, rmax, *args, **kwargs)
+        tmin = select_min(tmin, tn_sum - lmax - rmax)
+        lmin = select_min(lmin, tn_sum - rmax - tmax)
+        rmin = select_min(rmin, tn_sum - tmax - lmax)
+
+        tmax = select_max(tmax, tn_sum - lmin - rmin)
+        lmax = select_max(lmax, tn_sum - rmin - tmin)
+        rmax = select_max(rmax, tn_sum - tmin - lmin)
+
+        self.viewTLim.intervalx = tmin, tmax
+        self.viewLLim.intervalx = lmin, lmax
+        self.viewRLim.intervalx = rmin, rmax
+
+        self.viewOuterTLim.intervalx = tmin, tn_sum - lmin - rmin
+        self.viewOuterLLim.intervalx = lmin, tn_sum - tmin - rmin
+        self.viewOuterRLim.intervalx = rmin, tn_sum - tmin - lmin
+
+    def set_ternary_min(self, tmin, lmin, rmin, fit: str = "rectangle"):
+        """Set the minimum values for ternary limits."""
+        tmax = self.ternary_sum - lmin - rmin
+        lmax = self.ternary_sum - rmin - tmin
+        rmax = self.ternary_sum - tmin - lmin
+        self.set_ternary_lim(tmin, tmax, lmin, lmax, rmin, rmax, fit)
+
+    def set_ternary_max(self, tmax, lmax, rmax, fit: str = "rectangle"):
+        """Set the maximum values for ternary limits."""
+        tmin = (self.ternary_sum + tmax - lmax - rmax) * 0.5
+        lmin = (self.ternary_sum + lmax - rmax - tmax) * 0.5
+        rmin = (self.ternary_sum + rmax - tmax - lmax) * 0.5
+        self.set_ternary_lim(tmin, tmax, lmin, lmax, rmin, rmax, fit)
 
     def get_tlim(self):
+        """Return the t-axis view limits."""
         return tuple(self.viewTLim.intervalx)
 
     def get_llim(self):
+        """Return the l-axis view limits."""
         return tuple(self.viewLLim.intervalx)
 
     def get_rlim(self):
+        """Return the r-axis view limits."""
         return tuple(self.viewRLim.intervalx)
 
-    def set_tlim(self, tmin, tmax):
-        self.viewTLim.intervalx = (tmin, tmax)
-        self.stale = True
-        return tmin, tmax
-
-    def set_llim(self, lmin, lmax):
-        self.viewLLim.intervalx = (lmin, lmax)
-        self.stale = True
-        return lmin, lmax
-
-    def set_rlim(self, rmin, rmax):
-        self.viewRLim.intervalx = (rmin, rmax)
-        self.stale = True
-        return rmin, rmax
+    def set_tlim(self, tmin, tmax, fit: str = "rectangle"):
+        """Set the t-axis view limits."""
+        lmin, lmax = self.get_llim()
+        rmin, rmax = self.get_rlim()
+        self.set_ternary_lim(tmin, tmax, lmin, lmax, rmin, rmax, fit)
+        return self.get_tlim()
+
+    def set_llim(self, lmin, lmax, fit: str = "rectangle"):
+        """Set the l-axis view limits."""
+        tmin, tmax = self.get_tlim()
+        rmin, rmax = self.get_rlim()
+        self.set_ternary_lim(tmin, tmax, lmin, lmax, rmin, rmax, fit)
+        return self.get_llim()
+
+    def set_rlim(self, rmin, rmax, fit: str = "rectangle"):
+        """Set the r-axis view limits."""
+        tmin, tmax = self.get_tlim()
+        lmin, lmax = self.get_llim()
+        self.set_ternary_lim(tmin, tmax, lmin, lmax, rmin, rmax, fit)
+        return self.get_rlim()
 
     # Interactive manipulation
 
     def can_zoom(self):
         """
         Return whether this Axes supports the zoom box button functionality.
 
@@ -686,19 +831,17 @@
         - _set_view (`Home`, `Forward`, `Backward`)
         - _set_view_from_bbox (`Zoom-to-rectangle`)
         - drag_pan (`Pan/Zoom`)
         (https://matplotlib.org/users/navigation_toolbar.html)
         """
         # points = self.transProjection.inverted().transform(self.corners)
         trans = self._ternary_axes_transform.inverted()
-        points = trans.transform(self.corners_axes)
+        points = trans.transform(self.patch.get_xy())
 
         tmax = points[0, 0]
-        tmin = points[1, 0]
-        lmax = points[1, 1]
-        lmin = points[2, 1]
-        rmax = points[2, 2]
-        rmin = points[0, 2]
-
-        self.set_tlim(tmin, tmax)
-        self.set_llim(lmin, lmax)
-        self.set_rlim(rmin, rmax)
+        tmin = points[3, 0]
+        lmax = points[2, 1]
+        lmin = points[5, 1]
+        rmax = points[4, 2]
+        rmin = points[1, 2]
+
+        self._set_ternary_lim(tmin, tmax, lmin, lmax, rmin, rmax)
```

### Comparing `mpltern-0.5.0/mpltern/ternary/axis.py` & `mpltern-1.0.0/mpltern/ternary/axis.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,84 +1,124 @@
+"""
+Classes for t-, l-, r-axis.
+"""
 import numpy as np
 
-import matplotlib as mpl
 from matplotlib import _api
-import matplotlib.cbook as cbook
 from matplotlib.axis import XAxis
 import matplotlib.text as mtext
 import matplotlib.ticker as mticker
 from matplotlib.transforms import Affine2D
 from mpltern.ternary.tick import TTick, LTick, RTick
 
 
 class TernaryAxis(XAxis):
+    """Ternary axis."""
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._init()
 
     def _init(self):
         # x : data coordinates in the axis direction
         # y : display (pixel) coordinates in the direction vertical to the
         #     axis direction, updated when drawn in `_update_label_positions`
         trans = {
-            't': self.axes.get_taxis_transform(which='label'),
-            'l': self.axes.get_laxis_transform(which='label'),
-            'r': self.axes.get_raxis_transform(which='label'),
+            't': self.axes._tlabel_c_transform,
+            'l': self.axes._llabel_c_transform,
+            'r': self.axes._rlabel_c_transform,
         }[self.axis_name]
         self.label.set_rotation(0)
         self.label.set_rotation_mode('anchor')
         self.label.set_transform(trans)
         self.label_position = 'corner'
         self._label_rotation_mode = 'axis'
 
     def _copy_tick_props(self, src, dest):
         super()._copy_tick_props(src, dest)
         dest.label1.set_y(src.label1.get_position()[1])
         dest.label2.set_y(src.label2.get_position()[1])
 
-    def set_ticks(self, ticks, minor=False):
-        """
-        Set the locations of the tick marks from sequence ticks
-
-        Parameters
-        ----------
-        ticks : sequence of floats
-        minor : bool
-        """
+    def _set_tick_locations(self, ticks, *, minor=False):
+        locator = mticker.FixedLocator(ticks)
         if minor:
-            self.set_minor_locator(mticker.FixedLocator(ticks))
+            self.set_minor_locator(locator)
             return self.get_minor_ticks(len(ticks))
         else:
-            self.set_major_locator(mticker.FixedLocator(ticks))
+            self.set_major_locator(locator)
             return self.get_major_ticks(len(ticks))
 
+    def set_ticks(self, ticks, labels=None, *, minor=False, **kwargs):
+        """
+        Set this Axis' tick locations and optionally labels.
+
+        If necessary, the view limits of the Axis are expanded so that all
+        given ticks are visible.
+
+        Parameters
+        ----------
+        ticks : list of floats
+            List of tick locations.  The axis `.Locator` is replaced by a
+            `~.ticker.FixedLocator`.
+
+            Some tick formatters will not label arbitrary tick positions;
+            e.g. log formatters only label decade ticks by default. In
+            such a case you can set a formatter explicitly on the axis
+            using `.Axis.set_major_formatter` or provide formatted
+            *labels* yourself.
+        labels : list of str, optional
+            List of tick labels. If not set, the labels are generated with
+            the axis tick `.Formatter`.
+        minor : bool, default: False
+            If ``False``, set the major ticks; if ``True``, the minor ticks.
+        **kwargs
+            `.Text` properties for the labels. These take effect only if you
+            pass *labels*. In other cases, please use `~.Axes.tick_params`.
+
+        Notes
+        -----
+        Unlike Matplotlib, the view limits are *not* expanded. To achieve this
+        behavior, `set_ticks` is implemented in the same way as Matplotlib,
+        while `_set_tick_locations` are modified.
+        """
+        if labels is None and kwargs:
+            raise ValueError('labels argument cannot be None when '
+                             'kwargs are passed')
+        result = self._set_tick_locations(ticks, minor=minor)
+        if labels is not None:
+            self.set_ticklabels(labels, minor=minor, **kwargs)
+        return result
+
     def _get_tick(self, major):
         if major:
             tick_kw = self._major_tick_kw
         else:
             tick_kw = self._minor_tick_kw
         tick = {
             't': TTick,
             'l': LTick,
             'r': RTick,
         }[self.axis_name]
-        try:
-            return tick(self.axes, 0, major=major, **tick_kw)
-        except TypeError:  # matplotlib<=3.2.2
-            return tick(self.axes, 0, '', major=major, **tick_kw)
+        return tick(self.axes, 0, major=major, **tick_kw)
 
     def set_label_position(self, position):
         """
         Set the label position (corner, tick1, or tick2)
 
         Parameters
         ----------
-        position : {'corner', 'tick1', 'tick2'}
+        position : {'corner', 'tick1', 'tick2', 'side'}
+
+        Notes
+        -----
+        'side', 'tick1b', 'tick2b' are practical only for hexagonal boundaries.
         """
-        _api.check_in_list(['corner', 'tick1', 'tick2'], position=position)
+        _api.check_in_list(
+            ['corner', 'tick1', 'tick2', 'side', 'tick1b', 'tick2b'],
+            position=position,
+        )
         self.label_position = position
         self.stale = True
 
     def _update_label_position(self, renderer):
         """
         Update the label position based on the bounding box enclosing
         all the ticklabels and axis spine
@@ -86,55 +126,24 @@
         Called from `get_tightbbox` and `draw`.
         """
         if not self._autolabelpos:
             return
 
         pad = self.labelpad * self.figure.dpi / 72
 
-        if self.label_position == 'tick1':
-            trans = {
-                't': self.axes.get_laxis_transform(which='label'),
-                'l': self.axes.get_raxis_transform(which='label'),
-                'r': self.axes.get_taxis_transform(which='label'),
-            }[self.axis_name]
-            sign = -1.0  # outward triangle
-            x = 0.5  # midpoint of the axis
-        elif self.label_position == 'tick2':
-            trans = {
-                't': self.axes.get_raxis_transform(which='label'),
-                'l': self.axes.get_taxis_transform(which='label'),
-                'r': self.axes.get_laxis_transform(which='label'),
-            }[self.axis_name]
-            sign = -1.0  # outward triangle
-            x = 0.5  # midpoint of the axis
-        else:  # self.label_position == 'corner'
-            trans = {
-                't': self.axes.get_taxis_transform(which='label'),
-                'l': self.axes.get_laxis_transform(which='label'),
-                'r': self.axes.get_raxis_transform(which='label'),
-            }[self.axis_name]
-            sign = 1.0  # inward triangle
-            # Get the corner in the display coordinates, and then get
-            # the *x* coordinates in the `trans` coordinates
-            corner_index = {'t': 0, 'l': 1, 'r': 2}[self.axis_name]
-            corners = [[1., 0., 0.], [0., 1., 0.], [0., 0., 1.]]
-            corners = self.axes.transTernaryAxes.transform(corners)
-            corner = corners[corner_index]
-            x = trans.inverted().transform(corner)[0]
+        trans = self._get_ternary_label_transform()
 
-        points = self._get_points_surrounding_triangle(renderer=renderer)
+        points = self._get_points_surrounding_hexagon(renderer=renderer)
         points = trans.inverted().transform(points)
-        y = max(sign * points[:, 1]) * sign
-        position = (x, y + sign * pad)
 
-        self.label.set_position(position)
+        self.label.set_position((0.5, max(points[:, 1]) + pad))
         self.label.set_transform(trans)
         angle, ha, va = self._get_label_rotation()
-        self.label.set_ha(ha)
-        self.label.set_va(va)
+        self.label.set_horizontalalignment(ha)
+        self.label.set_verticalalignment(va)
         self.label.set_rotation(angle)
 
     def set_ticks_position(self, position):
         """
         Set the ticks position.
 
         Parameters
@@ -162,45 +171,85 @@
         elif position == 'none':
             self.set_tick_params(which='both', tick1On=False,
                                  tick2On=False)
         else:
             assert False, "unhandled parameter not caught by _check_in_list"
         self.stale = True
 
+    def get_tick_space(self):
+        """Get tick space in data coordinates
+
+        This is overridden to get the proper number of ticks for ternary axes.
+        """
+        trans = {
+            't': self.axes._tlabel_s_transform,
+            'l': self.axes._llabel_s_transform,
+            'r': self.axes._rlabel_s_transform,
+        }[self.axis_name]
+        vertices = self.axes._get_hexagonal_vertices()
+        points = self.axes._ternary2display_transform.transform(vertices)
+        points = trans.inverted().transform(points)
+        # length in pixel
+        length = np.linalg.norm(max(points[:, 1]) - min(points[:, 1]))
+        # Having a spacing of at least 2 just looks good.
+        size = self._get_tick_label_size('y') * 2
+        if size > 0:
+            return int(np.floor(length / size))
+        else:
+            return 2**31 - 1
+
     def get_view_interval(self):
         'return the Interval instance for this axis view limits'
         return {
-            't': self.axes.get_tlim,
-            'l': self.axes.get_llim,
-            'r': self.axes.get_rlim,
-        }[self.axis_name]()
+            't': self.axes.viewTLim.intervalx,
+            'l': self.axes.viewLLim.intervalx,
+            'r': self.axes.viewRLim.intervalx,
+        }[self.axis_name]
 
     # Helper methods for `mpltern`
 
-    def _get_points_surrounding_triangle(self, renderer):
+    def _get_points_surrounding_hexagon(self, renderer):
         """Get the points of all tick labels in the pixel coordinates."""
         ticks = []
         # Only ticks to draw are added.
-        for axis in self.axes._get_axis_list():
-            if axis in [self.axes.xaxis, self.axes.yaxis]:
-                continue
-            try:
-                ticks.extend(axis._update_ticks())
-            except TypeError:  # For Matplotlib 3.0.3
-                ticks.extend(axis._update_ticks(renderer))
+        for axis in [self.axes.taxis, self.axes.laxis, self.axes.raxis]:
+            ticks.extend(axis._update_ticks())
         points = []
         for tick in ticks:
             for text in [tick.label1, tick.label2]:
                 if text.get_visible():
                     points.extend(_get_points_surrounding_text(text, renderer))
         # In case no tick labels exist, points of triangle corners are added.
-        corners = [[1., 0., 0.], [0., 1., 0.], [0., 0., 1.]]
-        points.extend(self.axes.transTernaryAxes.transform(corners))
+        vertices = self.axes._get_hexagonal_vertices()
+        points.extend(self.axes._ternary2display_transform.transform(vertices))
         return np.asarray(points)
 
+    def _get_ternary_label_transform(self):
+        i = ["t", "l", "r"].index(self.axis_name)
+
+        tmp = ["corner", "tick1b", "tick2b"]
+        if self.label_position in tmp:
+            j = tmp.index(self.label_position)
+            return [
+                self.axes._tlabel_c_transform,
+                self.axes._llabel_c_transform,
+                self.axes._rlabel_c_transform,
+            ][(i + j) % 3]
+
+        tmp = ["side", "tick1", "tick2"]
+        if self.label_position in tmp:
+            j = tmp.index(self.label_position)
+            return [
+                self.axes._tlabel_s_transform,
+                self.axes._llabel_s_transform,
+                self.axes._rlabel_s_transform,
+            ][(i + j) % 3]
+
+        raise ValueError
+
     def set_label_rotation_mode(self, mode):
         """
         Set the mode how to rotate and align the axis-label.
 
         Parameters
         ----------
         mode : {'axis', 'horizontal', 'manual'}
@@ -231,16 +280,16 @@
             label_rotation, ha, va = _get_label_rotation_along_axis(
                 corners, self.axis_name, self.label_position)
         elif mode == 'horizontal':
             label_rotation, ha, va = _get_label_rotation_horizontal(
                 corners, self.axis_name, self.label_position)
         else:
             label_rotation = self.label.get_rotation()
-            ha = self.label.get_ha()
-            va = self.label.get_va()
+            ha = self.label.get_horizontalalignment()
+            va = self.label.get_verticalalignment()
         return label_rotation, ha, va
 
 
 class TAxis(TernaryAxis):
     axis_name = 't'
 
 
@@ -248,38 +297,48 @@
     axis_name = 'l'
 
 
 class RAxis(TernaryAxis):
     axis_name = 'r'
 
 
+def _get_corners(corners, axis_name: str, label_position: str):
+    """Get corners to determine label rotation.
+
+    Returns
+    -------
+    c0, c1, c2 : corners
+        The axis label is given at c0 or at the side opposite to c0.
+    """
+    index = ['t', 'l', 'r'].index(axis_name)
+    if label_position in ['corner', 'side']:
+        return np.roll(corners, 0 - index, axis=0)
+    if label_position in ['tick2', 'tick2b']:
+        return np.roll(corners, 1 - index, axis=0)
+    if label_position in ['tick1', 'tick1b']:
+        return np.roll(corners, 2 - index, axis=0)
+    raise ValueError(label_position)
+
+
 def _get_label_rotation_along_axis(corners, axis_name, label_position):
-    # Index of the corner
-    index = {'t': 0, 'l': 1, 'r': 2}[axis_name]
-    if label_position == 'tick1':
-        c0, c1, c2 = np.roll(corners,  1 - index, axis=0)
-    elif label_position == 'tick2':
-        c0, c1, c2 = np.roll(corners,  0 - index, axis=0)
-    else:  # self.label_position == 'corner':
-        c0, c1, c2 = np.roll(corners, -1 - index, axis=0)
-
-    d01 = c1 - c0
-    d12 = c2 - c1
-    axis_angle = np.rad2deg(np.arctan2(d01[1], d01[0]))  # [-180, +180]
-    clockwise = ((d01[0] * d12[1] - d01[1] * d12[0]) < 0.0)
-    is_corner = (label_position not in ['tick1', 'tick2'])
+    c0, c1, c2 = _get_corners(corners, axis_name, label_position)
+    v01 = c1 - c0
+    v12 = c2 - c1
+    axis_angle = np.rad2deg(np.arctan2(v12[1], v12[0]))  # [-180, +180]
+    clockwise = ((v01[0] * v12[1] - v01[1] * v12[0]) < 0.0)
+    is_corner = (label_position in ['corner', 'tick1b', 'tick2b'])
 
     tol = 1e-6
     if abs(abs(axis_angle) - 90.0) < tol:  # axis_angle is -90 or 90.
         # `label_rotation` is determined by comparing the coordinates of
         # the midpoint of the axis with those of the other corner point.
-        midpoint = (c0 + c1) * 0.5
+        is_right = (c0[0] > 0.5 * (c1[0] + c2[0]))
         # (the other corner is on the right side) xor
         # (the label is at the other corner)
-        if (c2[0] > midpoint[0]) ^ is_corner:
+        if is_right ^ is_corner:
             label_rotation = 90.0
         else:
             label_rotation = -90.0
         va = 'bottom'  # Because the label faces to the axis.
     else:
         # For readability, the angle is adjusted to be in [-90, +90]
         label_rotation = (axis_angle + 90.0) % 180.0 - 90.0
@@ -291,28 +350,20 @@
         else:
             va = 'top'
 
     return label_rotation, 'center', va
 
 
 def _get_label_rotation_horizontal(corners, axis_name, label_position):
-    # Index of the corner
-    index = {'t': 0, 'l': 1, 'r': 2}[axis_name]
-    if label_position == 'tick1':
-        c0, c1, c2 = np.roll(corners,  1 - index, axis=0)
-    elif label_position == 'tick2':
-        c0, c1, c2 = np.roll(corners,  0 - index, axis=0)
-    else:  # elif label_position == 'corner':
-        c0, c1, c2 = np.roll(corners, -1 - index, axis=0)
-
-    d01 = c1 - c0
-    d12 = c2 - c1
-    axis_angle = np.rad2deg(np.arctan2(d01[1], d01[0]))  # [-180, +180]
-    clockwise = ((d01[0] * d12[1] - d01[1] * d12[0]) < 0.0)
-    is_corner = (label_position not in ['tick1', 'tick2'])
+    c0, c1, c2 = _get_corners(corners, axis_name, label_position)
+    v01 = c1 - c0
+    v12 = c2 - c1
+    axis_angle = np.rad2deg(np.arctan2(v12[1], v12[0]))  # [-180, +180]
+    clockwise = ((v01[0] * v12[1] - v01[1] * v12[0]) < 0.0)
+    is_corner = (label_position in ['corner', 'tick1b', 'tick2b'])
 
     tol = 1e-6
     b = clockwise ^ is_corner
 
     if abs(axis_angle) < 75.0 + tol:
         va = 'bottom' if b else 'top'
     elif abs(axis_angle) < 105.0 - tol:
```

### Comparing `mpltern-0.5.0/mpltern/ternary/spines.py` & `mpltern-1.0.0/mpltern/ternary/spines.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,51 +1,43 @@
-from matplotlib import rcParams
-import matplotlib.spines as mspines
+"""Spine"""
+import matplotlib as mpl
 import matplotlib.path as mpath
+import matplotlib.spines as mspines
 
 
 class Spine(mspines.Spine):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.set_transform(self.axes.transAxes)
+    """A ternary-axis spine."""
+    def __init__(self, axes, spine_type, path, **kwargs):
+        super().__init__(axes, spine_type, path, **kwargs)
+        if spine_type in ["tside", "tcorner"]:
+            self.set_transform(self.axes.get_taxis_transform())
+        elif spine_type in ["lside", "lcorner"]:
+            self.set_transform(self.axes.get_laxis_transform())
+        elif spine_type in ["rside", "rcorner"]:
+            self.set_transform(self.axes.get_raxis_transform())
+        else:
+            raise ValueError(f'unknown spine_type: {spine_type}')
 
     def _adjust_location(self):
-        corners = [[1., 0., 0.], [0., 1., 0.], [0., 0., 1.]]
-        corners_axes = self.axes.transAxesProjection.transform(corners)
-
-        v1 = self._path.vertices
-        assert v1.shape == (2, 2), 'unexpected vertices shape'
-        if self.spine_type in ['tside']:
-            v1[0] = corners_axes[1]
-            v1[1] = corners_axes[2]
-        elif self.spine_type in ['lside']:
-            v1[0] = corners_axes[2]
-            v1[1] = corners_axes[0]
-        elif self.spine_type in ['rside']:
-            v1[0] = corners_axes[0]
-            v1[1] = corners_axes[1]
-        else:
-            raise ValueError('unable to set bounds for spine "%s"' %
-                             self.spine_type)
+        """Automatically set spine bounds to the view interval."""
+        if self.spine_type in ["tside", "tcorner"]:
+            low, high = self.axes.get_tlim()
+        elif self.spine_type in ["lside", "lcorner"]:
+            low, high = self.axes.get_llim()
+        elif self.spine_type in ["rside", "rcorner"]:
+            low, high = self.axes.get_rlim()
+
+        if self.spine_type in ["tside", "lside", "rside"]:
+            self._path.vertices = [[low, 0.0], [low, 1.0]]
+        elif self.spine_type in ["tcorner", "lcorner", "rcorner"]:
+            self._path.vertices = [[high, 0.0], [high, 1.0]]
 
     def get_spine_transform(self):
-        return self.axes.transAxes
+        return self.get_transform()
 
     @classmethod
     def linear_spine(cls, axes, spine_type, **kwargs):
-        """
-        (staticmethod) Returns a linear :class:`Spine`.
-        """
-        # all values of 0.999 get replaced upon call to set_bounds()
-        if spine_type == 'tside':
-            path = mpath.Path([(0.0, 0.0), (1.0, 0.0)])
-        elif spine_type == 'lside':
-            path = mpath.Path([(0.5, 1.0), (0.0, 0.0)])
-        elif spine_type == 'rside':
-            path = mpath.Path([(1.0, 0.0), (0.5, 1.0)])
-        else:
-            raise ValueError('unable to make path for spine "%s"' % spine_type)
+        """Create and return a linear `Spine`."""
+        path = mpath.Path([(0.0, 0.0), (0.0, 1.0)])
         result = cls(axes, spine_type, path, **kwargs)
-        result.set_visible(rcParams['axes.spines.bottom'])
-
+        result.set_visible(mpl.rcParams['axes.spines.bottom'])
         return result
-
```

### Comparing `mpltern-0.5.0/mpltern/ternary/tick.py` & `mpltern-1.0.0/mpltern/ternary/tick.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,21 @@
+"""
+Classes for the ternary ticks.
+"""
 import numpy as np
 
-import matplotlib as mpl
 from matplotlib import _api
-import matplotlib.cbook as cbook
 import matplotlib.transforms as mtransforms
 from matplotlib.axis import XTick
 
 
 class TernaryTick(XTick):
+    """Ternary tick"""
+    tick_name = ""  # implemented in subclasses
+
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.tick1line.set_transform(self._get_axis_transform(which='tick1'))
         self.tick2line.set_transform(self._get_axis_transform(which='tick2'))
         self.gridline.set_transform(self._get_axis_transform(which='grid'))
 
     def _set_labelrotation(self, labelrotation):
@@ -21,16 +25,18 @@
             mode = labelrotation
             angle = 0
         elif isinstance(labelrotation, (tuple, list)):
             mode, angle = labelrotation
         else:
             mode = 'tick'
             angle = labelrotation
-        _api.check_in_list(['tick', 'axis', 'horizontal', 'manual'],
-                             labelrotation=mode)
+        _api.check_in_list(
+            ['tick', 'axis', 'horizontal', 'manual'],
+            labelrotation=mode,
+        )
         self._labelrotation = (mode, angle)
 
     def _get_text1_transform(self):
         return {
             'ttick': self.axes.get_taxis_text1_transform,
             'ltick': self.axes.get_laxis_text1_transform,
             'rtick': self.axes.get_raxis_text1_transform,
@@ -157,71 +163,72 @@
         if mode == 'manual':
             self.label1.set_rotation(user_angle)
             self.label2.set_rotation(user_angle)
             return
 
         ha1, va1, rotation1 = self._determine_anchor(
             mode, axis1_angle, tick1_angle)
-        self.label1.set_ha(ha1)
-        self.label1.set_va(va1)
+        self.label1.set_horizontalalignment(ha1)
+        self.label1.set_verticalalignment(va1)
         self.label1.set_rotation(rotation1 + user_angle)
         self.label1.set_rotation_mode('anchor')
 
         ha2, va2, rotation2 = self._determine_anchor(
             mode, axis2_angle, tick2_angle)
-        self.label2.set_ha(ha2)
-        self.label2.set_va(va2)
+        self.label2.set_horizontalalignment(ha2)
+        self.label2.set_verticalalignment(va2)
         self.label2.set_rotation(rotation2 + user_angle)
         self.label2.set_rotation_mode('anchor')
 
     # Helper methods for `mpltern`
 
     def get_tick_angle(self):
         # The angle here is for `direction='in'`
         name = self.tick_name
         indices = {'ttick': [2, 1], 'ltick': [0, 2], 'rtick': [1, 0]}[name]
         corners = [[1., 0., 0.], [0., 1., 0.], [0., 0., 1.]]
         points = self.axes.transTernaryAxes.transform(corners)[indices]
-        d = points[1] - points[0]
-        return np.rad2deg(np.arctan2(d[1], d[0]))
+        direction = points[1] - points[0]
+        return np.rad2deg(np.arctan2(direction[1], direction[0]))
 
     def get_axis1_angle(self):
         name = self.tick_name
         indices = {'ttick': [2, 0], 'ltick': [0, 1], 'rtick': [1, 2]}[name]
         corners = [[1., 0., 0.], [0., 1., 0.], [0., 0., 1.]]
         points = self.axes.transTernaryAxes.transform(corners)[indices]
-        d = points[1] - points[0]
-        return np.rad2deg(np.arctan2(d[1], d[0]))
+        direction = points[1] - points[0]
+        return np.rad2deg(np.arctan2(direction[1], direction[0]))
 
     def get_axis2_angle(self):
         name = self.tick_name
         indices = {'ttick': [1, 0], 'ltick': [2, 1], 'rtick': [0, 2]}[name]
         corners = [[1., 0., 0.], [0., 1., 0.], [0., 0., 1.]]
         points = self.axes.transTernaryAxes.transform(corners)[indices]
-        d = points[1] - points[0]
-        return np.rad2deg(np.arctan2(d[1], d[0]))
+        direction = points[1] - points[0]
+        return np.rad2deg(np.arctan2(direction[1], direction[0]))
 
     def _tilt_marker(self, line, angle):
         if self._tickdir == 'in':
             trans = mtransforms.Affine2D().scale(1.0).rotate(angle)
         elif self._tickdir == 'inout':
             trans = mtransforms.Affine2D().scale(0.5).rotate(angle)
         elif self._tickdir == 'out':
             trans = mtransforms.Affine2D().scale(-1.0).rotate(angle)
         else:
-            # Don't modify custom tick line markers.
+            # Not modify custom tick line markers.
             trans = line._marker._transform
         line._marker._transform = trans
 
 
 class TTick(TernaryTick):
+    """T tick"""
     tick_name = 'ttick'
 
 
 class LTick(TernaryTick):
+    """L tick"""
     tick_name = 'ltick'
 
 
 class RTick(TernaryTick):
+    """R tick"""
     tick_name = 'rtick'
-
-
```

### Comparing `mpltern-0.5.0/mpltern/ternary_parsers.py` & `mpltern-1.0.0/mpltern/ternary_parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import matplotlib as mpl
 
 
 def _get_xy(ax, this, trans):
     t, l, r = this
     tlr = np.column_stack((t, l, r))
     if trans == ax.transTernaryAxes:
-        trans_xy = ax.transAxes
+        trans_xy = ax.transOuterAxes
         x, y = ax.transAxesProjection.transform(tlr).T
     else:
         trans_xy = ax.transData
         x, y = ax.transProjection.transform(tlr).T
     return x, y, trans_xy
```

### Comparing `mpltern-0.5.0/mpltern/tribin_helpers.py` & `mpltern-1.0.0/mpltern/tribin_helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
-from typing import Tuple
+from typing import Sequence
 
 
-def calc_ternary_indices(t, l, r, gridsize: int, extent: Tuple[float]):
+def calc_ternary_indices(t, l, r, gridsize: int, extent: Sequence[float]):
     tmin, tmax, lmin, lmax, rmin, rmax = extent
 
     # side lengths along ternary axes
     st = (tmax - tmin) / gridsize
     sl = (lmax - lmin) / gridsize
     sr = (rmax - rmin) / gridsize
 
@@ -78,15 +78,15 @@
     i0 = (gridsize - it - 1) * (gridsize - it) // 2 + ir
     shift = gridsize * (gridsize + 1) // 2
     i1 = (gridsize - it - 2) * (gridsize - it - 1) // 2 + ir
     i = np.where(it + il + ir + 1 == gridsize, i0, i1 + shift)
     return np.where(is_inside, i, -1)
 
 
-def serial_to_ternary(gridsize: int, i: int) -> Tuple[int]:
+def serial_to_ternary(gridsize: int, i: int) -> Sequence[int]:
     """Convert ternary indices of triangles to serial index.
 
     Parameters
     ----------
     gridsize : int
         Grid size.
     i : int
```

### Comparing `mpltern-0.5.0/mpltern.egg-info/SOURCES.txt` & `mpltern-1.0.0/mpltern.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,94 +1,103 @@
 .coveragerc
-.gitattributes
 .gitignore
-.lgtm.yml
 .readthedocs.yml
+.zenodo.json
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
 pytest.ini
 setup.py
 tox.ini
 .circleci/config.yml
 .github/workflows/publish-to-test-pypi.yml
 .github/workflows/tests.yml
 docs/index.html
 docsrc/Makefile
 docsrc/alternatives.rst
 docsrc/api.rst
-docsrc/basic_1.svg
-docsrc/basic_2.svg
-docsrc/basic_usage.py
 docsrc/basic_usage.rst
 docsrc/conf.py
 docsrc/conventions.rst
 docsrc/corner_based_1.py
 docsrc/corner_based_1.svg
 docsrc/corner_based_2.py
 docsrc/corner_based_2.svg
 docsrc/create_favicon.py
 docsrc/implemented_methods.rst
 docsrc/index.rst
 docsrc/installation.rst
 docsrc/make.bat
 docsrc/matplotlibrc
-docsrc/notes.rst
 docsrc/publications.rst
-docsrc/release_notes.rst
 docsrc/requirements.txt
 docsrc/side_based_ccw.py
 docsrc/side_based_ccw.svg
 docsrc/side_based_cw.py
 docsrc/side_based_cw.svg
-docsrc/_static/.DS_Store
 docsrc/_static/favicon.ico
-docsrc/_static/sphx_glr_logos0_002.svg
+docsrc/_static/logo_dark.svg
+docsrc/_static/logo_light.svg
+docsrc/_static/mpl.css
+docsrc/sphinxext/__init__.py
+docsrc/sphinxext/custom_roles.py
+docsrc/users/index.rst
+docsrc/users/mpltern_1.0.0.rst
+docsrc/users/release_notes.rst
 examples/README.rst
-examples/advanced/00.colored_axes.py
-examples/advanced/01.arrows_along_axes.py
-examples/advanced/02.minor_ticks.py
-examples/advanced/03.manual_tick_positions.py
-examples/advanced/04.tick_labels_inside_triangle.py
-examples/advanced/05.inset.py
-examples/advanced/06.plot_fixed_onto_triangle.py
-examples/advanced/README.rst
+examples/axis_and_tick/00.axis_label_position.py
+examples/axis_and_tick/01.axis_label_rotation.py
+examples/axis_and_tick/10.tick_position.py
+examples/axis_and_tick/11.tick_direction.py
+examples/axis_and_tick/12.tick_rotation.py
+examples/axis_and_tick/20.tick-formatters.py
+examples/axis_and_tick/21.tick-locators.py
+examples/axis_and_tick/30.manual_tick_positions.py
+examples/axis_and_tick/31.manual_ticklabels.py
+examples/axis_and_tick/98.colored_axes.py
+examples/axis_and_tick/99.tick_labels_inside_triangle.py
 examples/axis_and_tick/README.rst
-examples/axis_and_tick/axis_label_position.py
-examples/axis_and_tick/axis_label_rotation.py
-examples/axis_and_tick/tick_direction.py
-examples/axis_and_tick/tick_position.py
-examples/axis_and_tick/tick_rotation.py
+examples/intermediate/00.with_normal_plots.py
+examples/intermediate/01.style_sheets.py
+examples/intermediate/99.inset.py
 examples/intermediate/README.rst
-examples/intermediate/axline.py
-examples/intermediate/legend.py
-examples/intermediate/ternary_limits.py
-examples/intermediate/with_normal_plots.py
-examples/intermediate/with_seaborn_styles.py
 examples/introductory/00.line_and_curve.py
 examples/introductory/01.scatter.py
 examples/introductory/02.contour.py
 examples/introductory/03.pseudocolor.py
 examples/introductory/04.normalization.py
 examples/introductory/05.span.py
 examples/introductory/06.text.py
 examples/introductory/07.polygon.py
 examples/introductory/08.quiver.py
 examples/introductory/09.grid.py
 examples/introductory/10.axis_labels.py
 examples/introductory/11.triangular_grid.py
 examples/introductory/README.rst
+examples/introductory/axline.py
+examples/introductory/legend.py
+examples/limits/00.triangular_limits.py
+examples/limits/01.hexagonal_limits.py
+examples/limits/02.fit.py
+examples/limits/README.rst
+examples/miscellaneous/00.logos.py
 examples/miscellaneous/README.rst
 examples/miscellaneous/dirichlet_pdf.py
-examples/miscellaneous/logos0.py
+examples/miscellaneous/evolutionary_game_theory.py
+examples/miscellaneous/soil_texture.py
 examples/statistics/README.rst
 examples/statistics/hexbin.py
 examples/statistics/tribin.py
 examples/statistics/with_scatter.py
+examples/transforms/00.cartesian.py
+examples/transforms/01.ticks.py
+examples/transforms/06.plot_fixed_onto_triangle.py
+examples/transforms/99.arrows_along_axes.py
+examples/transforms/README.rst
 examples/triangle/00.aspect.py
 examples/triangle/01.triangle_rotation.py
 examples/triangle/02.arbitrary_triangle.py
 examples/triangle/README.rst
 mpltern/__init__.py
 mpltern/datasets.py
 mpltern/hexbin_helpers.py
@@ -116,15 +125,15 @@
 tests/make_references.py
 tests/test_axis.py
 tests/test_constrainedlayout.py
 tests/test_datasets.py
 tests/test_given_triangles.py
 tests/test_hexbin.py
 tests/test_hexbin_helpers.py
-tests/test_scatter.py
+tests/test_spines.py
 tests/test_ternary.py
 tests/test_text.py
 tests/test_tick.py
 tests/test_tightlayout.py
 tests/test_transforms.py
 tests/test_triangle_rotation_axis.py
 tests/test_triangle_rotation_horizontal.py
@@ -155,25 +164,30 @@
 tests/baseline_images/test_ternary/arrow_data.pdf
 tests/baseline_images/test_ternary/arrow_xy_axes.pdf
 tests/baseline_images/test_ternary/arrow_xy_data.pdf
 tests/baseline_images/test_ternary/aspect.pdf
 tests/baseline_images/test_ternary/axis_label_position_corner.pdf
 tests/baseline_images/test_ternary/axis_label_position_tick1.pdf
 tests/baseline_images/test_ternary/axis_label_position_tick2.pdf
+tests/baseline_images/test_ternary/fit_none.pdf
+tests/baseline_images/test_ternary/fit_rectangle.pdf
+tests/baseline_images/test_ternary/fit_triangle.pdf
 tests/baseline_images/test_ternary/legend.pdf
+tests/baseline_images/test_ternary/manual_ticklabels.pdf
 tests/baseline_images/test_ternary/manual_ticks.pdf
 tests/baseline_images/test_ternary/negative_ticks.pdf
 tests/baseline_images/test_ternary/opposite_ticks.pdf
 tests/baseline_images/test_ternary/plot.pdf
 tests/baseline_images/test_ternary/quiver.pdf
 tests/baseline_images/test_ternary/quiver_color.pdf
 tests/baseline_images/test_ternary/quiver_xy_axes.pdf
 tests/baseline_images/test_ternary/quiver_xy_data.pdf
 tests/baseline_images/test_ternary/scatter.pdf
 tests/baseline_images/test_ternary/scatter_color.pdf
+tests/baseline_images/test_ternary/spans.pdf
 tests/baseline_images/test_ternary/test_ternary_lim-expected.pdf
 tests/baseline_images/test_ternary/test_ternary_lim-expected.png
 tests/baseline_images/test_ternary/test_ternary_lim-expected.svg
 tests/baseline_images/test_ternary/test_ternary_lim-expected_pdf.png
 tests/baseline_images/test_ternary/test_ternary_lim-expected_svg.png
 tests/baseline_images/test_ternary/test_ternary_lim.pdf
 tests/baseline_images/test_ternary/test_ternary_lim.png
```

### Comparing `mpltern-0.5.0/setup.py` & `mpltern-1.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,28 +84,21 @@
     #
     # For a list of valid classifiers, see https://pypi.org/classifiers/
     classifiers=[  # Optional
         # How mature is this project? Common values are
         #   3 - Alpha
         #   4 - Beta
         #   5 - Production/Stable
-        'Development Status :: 4 - Beta',
-
-        # Indicate who your project is intended for
-        'Intended Audience :: Developers',
-        'Topic :: Software Development :: Build Tools',
-
-        # Pick your license as you wish
+        'Development Status :: 5 - Production/Stable',
+        'Framework :: Matplotlib',
+        'Intended Audience :: Science/Research',
+        'Intended Audience :: Education',
         'License :: OSI Approved :: MIT License',
-
-        # Specify the Python versions you support here. In particular, ensure
-        # that you indicate whether you support Python 2, Python 3 or both.
-        # These classifiers are *not* checked by 'pip install'. See instead
-        # 'python_requires' below.
-        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3',
+        'Topic :: Scientific/Engineering :: Visualization',
     ],
 
     # This field adds keywords for your project which will appear on the
     # project page. What does your project relate to?
     #
     # Note that this is a string of words separated by whitespace, not a list.
     # keywords='sample setuptools development',  # Optional
```

### Comparing `mpltern-0.5.0/tests/Dirichlet_PDF_1.0_2.0_2.0.txt` & `mpltern-1.0.0/tests/Dirichlet_PDF_1.0_2.0_2.0.txt`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/Dirichlet_PDF_1.5_1.5_1.5.txt` & `mpltern-1.0.0/tests/Dirichlet_PDF_1.5_1.5_1.5.txt`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/Dirichlet_PDF_2.0_4.0_8.0.txt` & `mpltern-1.0.0/tests/Dirichlet_PDF_2.0_4.0_8.0.txt`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/Dirichlet_PDF_5.0_5.0_5.0.txt` & `mpltern-1.0.0/tests/Dirichlet_PDF_5.0_5.0_5.0.txt`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_constrainedlayout/constrained_layout1.pdf` & `mpltern-1.0.0/tests/baseline_images/test_constrainedlayout/constrained_layout1.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_given_triangles/given_triangles_axis_0.pdf` & `mpltern-1.0.0/tests/baseline_images/test_given_triangles/given_triangles_axis_0.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_given_triangles/given_triangles_axis_180.pdf` & `mpltern-1.0.0/tests/baseline_images/test_given_triangles/given_triangles_axis_180.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_given_triangles/given_triangles_axis_270.pdf` & `mpltern-1.0.0/tests/baseline_images/test_given_triangles/given_triangles_axis_270.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_given_triangles/given_triangles_axis_90.pdf` & `mpltern-1.0.0/tests/baseline_images/test_given_triangles/given_triangles_axis_90.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_given_triangles/given_triangles_horizontal_0.pdf` & `mpltern-1.0.0/tests/baseline_images/test_given_triangles/given_triangles_horizontal_0.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_given_triangles/given_triangles_horizontal_180.pdf` & `mpltern-1.0.0/tests/baseline_images/test_given_triangles/given_triangles_horizontal_180.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_given_triangles/given_triangles_horizontal_270.pdf` & `mpltern-1.0.0/tests/baseline_images/test_given_triangles/given_triangles_horizontal_270.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_given_triangles/given_triangles_horizontal_90.pdf` & `mpltern-1.0.0/tests/baseline_images/test_given_triangles/given_triangles_horizontal_90.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_given_triangles/given_triangles_tick_0.pdf` & `mpltern-1.0.0/tests/baseline_images/test_given_triangles/given_triangles_tick_0.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_given_triangles/given_triangles_tick_180.pdf` & `mpltern-1.0.0/tests/baseline_images/test_given_triangles/given_triangles_tick_180.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_given_triangles/given_triangles_tick_270.pdf` & `mpltern-1.0.0/tests/baseline_images/test_given_triangles/given_triangles_tick_270.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_given_triangles/given_triangles_tick_90.pdf` & `mpltern-1.0.0/tests/baseline_images/test_given_triangles/given_triangles_tick_90.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_hexbin/base.pdf` & `mpltern-1.0.0/tests/baseline_images/test_hexbin/base.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_hexbin/extent.pdf` & `mpltern-1.0.0/tests/baseline_images/test_hexbin/extent.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_hexbin/given_triangles.pdf` & `mpltern-1.0.0/tests/baseline_images/test_hexbin/given_triangles.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_hexbin/ternary_lim.pdf` & `mpltern-1.0.0/tests/baseline_images/test_hexbin/ternary_lim.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_ternary/arguments_6.pdf` & `mpltern-1.0.0/tests/baseline_images/test_ternary/arguments_6.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_ternary/arguments_7.pdf` & `mpltern-1.0.0/tests/baseline_images/test_ternary/arguments_7.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_ternary/arrow_axes.pdf` & `mpltern-1.0.0/tests/baseline_images/test_ternary/arrow_axes.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_ternary/arrow_data.pdf` & `mpltern-1.0.0/tests/baseline_images/test_ternary/arrow_data.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_ternary/arrow_xy_axes.pdf` & `mpltern-1.0.0/tests/baseline_images/test_ternary/arrow_xy_axes.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_ternary/arrow_xy_data.pdf` & `mpltern-1.0.0/tests/baseline_images/test_ternary/arrow_xy_data.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_ternary/aspect.pdf` & `mpltern-1.0.0/tests/baseline_images/test_ternary/aspect.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_ternary/axis_label_position_corner.pdf` & `mpltern-1.0.0/tests/baseline_images/test_ternary/axis_label_position_corner.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_ternary/axis_label_position_tick1.pdf` & `mpltern-1.0.0/tests/baseline_images/test_ternary/axis_label_position_tick1.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_ternary/axis_label_position_tick2.pdf` & `mpltern-1.0.0/tests/baseline_images/test_ternary/axis_label_position_tick2.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_ternary/legend.pdf` & `mpltern-1.0.0/tests/baseline_images/test_ternary/legend.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_ternary/manual_ticks.pdf` & `mpltern-1.0.0/tests/baseline_images/test_ternary/manual_ticks.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_ternary/negative_ticks.pdf` & `mpltern-1.0.0/tests/baseline_images/test_ternary/negative_ticks.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_ternary/opposite_ticks.pdf` & `mpltern-1.0.0/tests/baseline_images/test_ternary/opposite_ticks.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_ternary/plot.pdf` & `mpltern-1.0.0/tests/baseline_images/test_ternary/plot.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_ternary/quiver.pdf` & `mpltern-1.0.0/tests/baseline_images/test_ternary/quiver.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_ternary/quiver_color.pdf` & `mpltern-1.0.0/tests/baseline_images/test_ternary/quiver_color.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_ternary/quiver_xy_axes.pdf` & `mpltern-1.0.0/tests/baseline_images/test_ternary/quiver_xy_axes.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_ternary/quiver_xy_data.pdf` & `mpltern-1.0.0/tests/baseline_images/test_ternary/quiver_xy_data.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_ternary/scatter.pdf` & `mpltern-1.0.0/tests/baseline_images/test_ternary/scatter.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_ternary/scatter_color.pdf` & `mpltern-1.0.0/tests/baseline_images/test_ternary/scatter_color.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_ternary/test_ternary_lim-expected.pdf` & `mpltern-1.0.0/tests/baseline_images/test_ternary/test_ternary_lim-expected.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_ternary/test_ternary_lim-expected.png` & `mpltern-1.0.0/tests/baseline_images/test_ternary/test_ternary_lim-expected.png`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_ternary/test_ternary_lim-expected.svg` & `mpltern-1.0.0/tests/baseline_images/test_ternary/test_ternary_lim-expected.svg`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_ternary/test_ternary_lim-expected_pdf.png` & `mpltern-1.0.0/tests/baseline_images/test_ternary/test_ternary_lim-expected_pdf.png`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_ternary/test_ternary_lim-expected_svg.png` & `mpltern-1.0.0/tests/baseline_images/test_ternary/test_ternary_lim-expected_svg.png`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_ternary/test_ternary_lim.pdf` & `mpltern-1.0.0/tests/baseline_images/test_ternary/test_ternary_lim.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_ternary/test_ternary_lim.png` & `mpltern-1.0.0/tests/baseline_images/test_ternary/test_ternary_lim.png`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_ternary/test_ternary_lim.svg` & `mpltern-1.0.0/tests/baseline_images/test_ternary/test_ternary_lim.svg`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_ternary/test_ternary_lim_pdf.png` & `mpltern-1.0.0/tests/baseline_images/test_ternary/test_ternary_lim_pdf.png`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_ternary/test_ternary_lim_svg.png` & `mpltern-1.0.0/tests/baseline_images/test_ternary/test_ternary_lim_svg.png`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_ternary/text.pdf` & `mpltern-1.0.0/tests/baseline_images/test_ternary/text.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_ternary/tick_direction_in.pdf` & `mpltern-1.0.0/tests/baseline_images/test_ternary/tick_direction_in.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_ternary/tick_direction_inout.pdf` & `mpltern-1.0.0/tests/baseline_images/test_ternary/tick_direction_inout.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_ternary/tick_direction_out.pdf` & `mpltern-1.0.0/tests/baseline_images/test_ternary/tick_direction_out.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_ternary/tick_labels_inside_triangle.pdf` & `mpltern-1.0.0/tests/baseline_images/test_ternary/tick_labels_inside_triangle.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_ternary/titie_center.pdf` & `mpltern-1.0.0/tests/baseline_images/test_ternary/titie_center.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_ternary/titie_left.pdf` & `mpltern-1.0.0/tests/baseline_images/test_ternary/titie_left.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_ternary/titie_right.pdf` & `mpltern-1.0.0/tests/baseline_images/test_ternary/titie_right.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_ternary/transAxes.pdf` & `mpltern-1.0.0/tests/baseline_images/test_ternary/transAxes.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_tightlayout/tight_layout1.pdf` & `mpltern-1.0.0/tests/baseline_images/test_tightlayout/tight_layout1.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_0.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_0.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_105.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_105.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_120.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_120.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_135.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_135.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_15.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_15.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_150.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_150.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_165.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_165.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_180.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_180.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_195.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_195.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_210.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_210.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_225.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_225.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_240.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_240.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_255.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_255.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_270.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_270.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_285.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_285.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_30.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_30.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_300.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_300.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_315.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_315.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_330.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_330.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_345.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_345.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_360.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_360.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_45.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_45.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_60.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_60.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_75.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_75.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_90.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_False_90.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_0.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_0.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_105.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_105.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_120.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_120.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_135.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_135.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_15.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_15.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_150.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_150.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_165.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_165.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_180.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_180.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_195.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_195.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_210.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_210.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_225.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_225.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_240.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_240.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_255.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_255.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_270.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_270.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_285.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_285.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_30.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_30.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_300.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_300.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_315.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_315.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_330.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_330.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_345.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_345.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_360.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_360.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_45.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_45.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_60.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_60.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_75.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_75.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_90.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CCW_True_90.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_0.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_0.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_105.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_105.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_120.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_120.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_135.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_135.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_15.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_15.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_150.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_150.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_165.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_165.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_180.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_180.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_195.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_195.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_210.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_210.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_225.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_225.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_240.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_240.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_255.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_255.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_270.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_270.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_285.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_285.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_30.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_30.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_300.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_300.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_315.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_315.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_330.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_330.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_345.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_345.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_360.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_360.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_45.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_45.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_60.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_60.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_75.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_75.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_90.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_False_90.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_0.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_0.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_105.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_105.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_120.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_120.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_135.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_135.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_15.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_15.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_150.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_150.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_165.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_165.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_180.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_180.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_195.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_195.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_210.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_210.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_225.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_225.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_240.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_240.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_255.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_255.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_270.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_270.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_285.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_285.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_30.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_30.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_300.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_300.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_315.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_315.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_330.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_330.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_345.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_345.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_360.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_360.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_45.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_45.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_60.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_60.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_75.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_75.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_90.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_axis/CW_True_90.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_0.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_0.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_105.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_105.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_120.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_120.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_135.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_135.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_15.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_15.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_150.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_150.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_165.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_165.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_180.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_180.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_195.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_195.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_210.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_210.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_225.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_225.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_240.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_240.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_255.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_255.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_270.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_270.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_285.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_285.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_30.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_30.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_300.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_300.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_315.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_315.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_330.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_330.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_345.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_345.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_360.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_360.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_45.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_45.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_60.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_60.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_75.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_75.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_90.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_False_90.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_0.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_0.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_105.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_105.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_120.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_120.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_135.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_135.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_15.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_15.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_150.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_150.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_165.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_165.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_180.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_180.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_195.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_195.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_210.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_210.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_225.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_225.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_240.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_240.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_255.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_255.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_270.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_270.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_285.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_285.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_30.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_30.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_300.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_300.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_315.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_315.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_330.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_330.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_345.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_345.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_360.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_360.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_45.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_45.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_60.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_60.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_75.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_75.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_90.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CCW_True_90.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_0.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_0.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_105.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_105.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_120.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_120.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_135.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_135.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_15.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_15.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_150.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_150.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_165.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_165.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_180.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_180.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_195.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_195.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_210.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_210.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_225.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_225.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_240.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_240.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_255.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_255.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_270.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_270.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_285.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_285.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_30.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_30.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_300.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_300.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_315.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_315.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_330.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_330.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_345.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_345.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_360.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_360.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_45.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_45.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_60.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_60.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_75.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_75.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_90.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_False_90.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_0.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_0.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_105.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_105.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_120.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_120.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_135.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_135.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_15.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_15.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_150.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_150.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_165.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_165.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_180.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_180.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_195.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_195.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_210.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_210.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_225.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_225.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_240.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_240.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_255.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_255.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_270.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_270.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_285.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_285.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_30.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_30.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_300.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_300.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_315.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_315.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_330.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_330.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_345.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_345.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_360.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_360.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_45.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_45.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_60.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_60.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_75.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_75.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_90.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_horizontal/CW_True_90.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_0.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_0.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_105.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_105.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_120.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_120.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_135.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_135.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_15.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_15.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_150.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_150.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_165.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_165.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_180.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_180.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_195.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_195.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_210.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_210.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_225.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_225.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_240.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_240.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_255.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_255.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_270.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_270.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_285.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_285.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_30.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_30.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_300.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_300.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_315.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_315.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_330.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_330.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_345.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_345.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_360.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_360.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_45.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_45.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_60.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_60.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_75.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_75.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_90.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_False_90.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_0.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_0.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_105.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_105.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_120.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_120.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_135.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_135.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_15.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_15.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_150.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_150.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_165.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_165.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_180.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_180.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_195.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_195.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_210.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_210.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_225.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_225.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_240.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_240.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_255.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_255.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_270.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_270.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_285.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_285.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_30.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_30.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_300.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_300.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_315.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_315.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_330.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_330.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_345.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_345.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_360.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_360.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_45.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_45.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_60.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_60.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_75.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_75.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_90.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CCW_True_90.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_0.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_0.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_105.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_105.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_120.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_120.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_135.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_135.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_15.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_15.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_150.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_150.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_165.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_165.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_180.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_180.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_195.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_195.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_210.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_210.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_225.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_225.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_240.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_240.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_255.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_255.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_270.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_270.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_285.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_285.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_30.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_30.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_300.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_300.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_315.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_315.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_330.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_330.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_345.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_345.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_360.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_360.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_45.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_45.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_60.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_60.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_75.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_75.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_90.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_False_90.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_0.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_0.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_105.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_105.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_120.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_120.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_135.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_135.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_15.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_15.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_150.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_150.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_165.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_165.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_180.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_180.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_195.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_195.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_210.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_210.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_225.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_225.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_240.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_240.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_255.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_255.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_270.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_270.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_285.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_285.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_30.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_30.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_300.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_300.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_315.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_315.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_330.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_330.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_345.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_345.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_360.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_360.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_45.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_45.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_60.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_60.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_75.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_75.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_90.pdf` & `mpltern-1.0.0/tests/baseline_images/test_triangle_rotation_tick/CW_True_90.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_tribin/base.pdf` & `mpltern-1.0.0/tests/baseline_images/test_tribin/base.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_tribin/extent.pdf` & `mpltern-1.0.0/tests/baseline_images/test_tribin/extent.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_tribin/given_triangles.pdf` & `mpltern-1.0.0/tests/baseline_images/test_tribin/given_triangles.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/baseline_images/test_tribin/ternary_lim.pdf` & `mpltern-1.0.0/tests/baseline_images/test_tribin/ternary_lim.pdf`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/hexbin_indices.txt` & `mpltern-1.0.0/tests/hexbin_indices.txt`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/test_axis.py` & `mpltern-1.0.0/tests/test_axis.py`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/test_given_triangles.py` & `mpltern-1.0.0/tests/test_given_triangles.py`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/test_hexbin.py` & `mpltern-1.0.0/tests/test_hexbin.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 import numpy as np
 
 import matplotlib.pyplot as plt
-from matplotlib.testing.decorators import image_comparison
-import mpltern
+from matplotlib.testing.decorators import image_comparison, check_figures_equal
+from matplotlib.colors import LogNorm
+import mpltern  # noqa: F401
+
 
 @image_comparison(
     baseline_images=["base"],
     extensions=["pdf"],
     tol=0.1,
     style="mpl20",
 )
 def test_base():
     np.random.seed(19680801)
     t, l, r = np.random.dirichlet(alpha=(2.0, 4.0, 8.0), size=100000).T
     ax = plt.subplot(projection="ternary")
     # If "face" (default), small hexagons look overlapping with each other.
     ax.hexbin(t, l, r, edgecolors="none")
 
+
 @image_comparison(
     baseline_images=["ternary_lim"],
     extensions=["pdf"],
     style="mpl20",
 )
 def test_ternary_lim():
     np.random.seed(19680801)
@@ -30,32 +33,46 @@
     ax.hexbin(t, l, r, edgecolors="none")
     ax.set_ternary_lim(
         0.1, 0.5,  # tmin, tmax
         0.2, 0.6,  # lmin, lmax
         0.3, 0.7,  # rmin, rmax
     )
 
+
 @image_comparison(
     baseline_images=["extent"],
     extensions=["pdf"],
     style="mpl20",
 )
 def test_extent():
     np.random.seed(19680801)
     t, l, r = np.random.dirichlet(alpha=(2.0, 4.0, 8.0), size=100000).T
     ax = plt.subplot(projection="ternary")
     extent = (0.1, 0.5, 0.2, 0.6, 0.3, 0.7)
     # If "face" (default), small hexagons look overlapping with each other.
     ax.hexbin(t, l, r, gridsize=40, extent=extent, edgecolors="none")
 
+
 @image_comparison(
     baseline_images=["given_triangles"],
     extensions=["pdf"],
     style="mpl20",
 )
 def test_given_triangles():
     corners = ((0.5, 0.0), (1.0, 0.5), (0.0, 1.0))
     np.random.seed(19680801)
     t, l, r = np.random.dirichlet(alpha=(2.0, 4.0, 8.0), size=100000).T
     ax = plt.subplot(projection="ternary", corners=corners, rotation=0)
     # If "face" (default), small hexagons look overlapping with each other.
     ax.hexbin(t, l, r, edgecolors="none")
+
+
+@check_figures_equal(extensions=('pdf',))
+def test_bins_and_norm(fig_test, fig_ref):
+    np.random.seed(19680801)
+    t, l, r = np.random.dirichlet(alpha=(2.0, 4.0, 8.0), size=100000).T
+
+    ax = fig_test.add_subplot(projection="ternary")
+    ax.hexbin(t, l, r, bins="log")
+
+    ax = fig_ref.add_subplot(projection="ternary")
+    ax.hexbin(t, l, r, norm=LogNorm())
```

### Comparing `mpltern-0.5.0/tests/test_hexbin_helpers.py` & `mpltern-1.0.0/tests/test_hexbin_helpers.py`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/test_ternary.py` & `mpltern-1.0.0/tests/test_ternary.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 
 import pytest
+import matplotlib as mpl
 from matplotlib.testing.decorators import (
     image_comparison, check_figures_equal)
 import matplotlib.pyplot as plt
 from mpltern.datasets import (
     get_spiral, get_scatter_points, get_triangular_grid)
 
 
@@ -14,18 +15,19 @@
     # is restored.
     if 'text.kerning_factor' in plt.rcParams:
         plt.rcParams['text.kerning_factor'] = 6
 
 
 @image_comparison(baseline_images=['plot'], extensions=['pdf'], style='mpl20')
 def test_plot():
+    """Test if `plot` works as expected."""
     fig = plt.figure()
     ax = fig.add_subplot(projection='ternary')
-    t, l, r = get_spiral()
-    ax.plot(t, l, r)
+    tn0, tn1, tn2 = get_spiral()
+    ax.plot(tn0, tn1, tn2)
 
 
 # In Matplotlib, it is NOT allowed to exchange `x` and `y` in `ax.plot` even
 # when specifying them as keyword arguments. Following this behavior, in
 # `mpltern`, the order of `t`, `l`, `r` must not be able to exchange.
 # The following tests must, therefore, return errors.
 
@@ -49,73 +51,80 @@
 #         ax = fig_test.add_subplot(111, projection='ternary')
 #         ax.plot(c='C1', r=r, l=l, t=t)
 #         fig_ref = plt.figure()
 #         ax = fig_ref.add_subplot(111, projection='ternary')
 #         ax.plot(t, l, r, c='C1')
 
 
-def test_data():
-    fig = plt.figure()
-    ax = fig.add_subplot(projection='ternary')
-    t, l, r = get_spiral()
-    data = {'t': t, 'l': l, 'r': r}
-    ax.plot('t', 'l', 'r', data=data)
+@check_figures_equal(extensions=('pdf',))
+def test_data(fig_ref, fig_test):
+    """Test if the `data` argument works correctly."""
+    tn0, tn1, tn2 = get_spiral()
+
+    ax = fig_test.add_subplot(projection='ternary')
+    data = {'tn0': tn0, 'tn1': tn1, 'tn2': tn2}
+    ax.plot('tn0', 'tn1', 'tn2', data=data)
+
+    ax = fig_ref.add_subplot(projection='ternary')
+    ax.plot(tn0, tn1, tn2)
 
 
 def test_data_with_five_arguments():
-    # When with data, the number of positional arguments must be 3 or 4.
+    """Test if data with 5 arguments raise ValueError.
+
+    With data, the number of positional arguments must be 3 or 4.
+    """
     fig = plt.figure()
     ax = fig.add_subplot(projection='ternary')
-    t, l, r = get_spiral()
-    data = {'t': t, 'l': l, 'r': r}
+    tn0, tn1, tn2 = get_spiral()
+    data = {'tn0': tn0, 'tn1': tn1, 'tn2': tn2}
     with pytest.raises(ValueError):
-        ax.plot('t', 'l', 'r', 'foo', 'bar', data=data)
+        ax.plot('tn0', 'tn1', 'tn2', 'foo', 'bar', data=data)
 
 
 class TestArguments:
     @image_comparison(baseline_images=['arguments_6'], extensions=['pdf'],
                       style='mpl20')
     def test_arguments_6(self):
+        """Test if 6 arguments are parsed correctly."""
         fig = plt.figure()
         ax = fig.add_subplot(projection='ternary')
-        t, l, r = get_spiral()
-        ax.plot(t, l, r, l, r, t)
+        tn0, tn1, tn2 = get_spiral()
+        ax.plot(tn0, tn1, tn2, tn1, tn2, tn0)
 
     @image_comparison(baseline_images=['arguments_7'], extensions=['pdf'],
                       style='mpl20')
     def test_arguments_7(self):
+        """Test if 7 arguments are parsed correctly."""
         fig = plt.figure()
         ax = fig.add_subplot(projection='ternary')
-        t, l, r = get_spiral()
-        ax.plot(t, l, r, 'C3:', l, r, t)
+        tn0, tn1, tn2 = get_spiral()
+        ax.plot(tn0, tn1, tn2, 'C3:', tn1, tn2, tn0)
 
     def test_no_arguments(self):
-        # In Matplotlib, `ax.plot()` without any arguments returns an empty
-        # list. This test checks whether `mpltern` mimics this behavior.
+        """Test if `plot` with no arguments returns an empty list."""
         fig = plt.figure()
         ax = fig.add_subplot(projection='ternary')
         lines = ax.plot()
         assert lines == []
 
 
 class TestTransform:
-    # Confirm that `plot` can recognize `ax.transAxes` and handle data
-    # ax expected.
     @image_comparison(baseline_images=['transAxes'], extensions=['pdf'],
                       style='mpl20')
     def test_tranform_1(self):
+        """Test if `plot` recognizes and handle `ax.transAxes` as expected."""
         fig_test = plt.figure()
         ax = fig_test.add_subplot(111, projection='ternary')
         ax.plot([0, 1], [0, 1], transform=ax.transAxes)
 
 
 class TestAxisLabelPosition:
     positions = ['corner', 'tick1', 'tick2']
-    baseline_images_list = [
-        ['axis_label_position_{}'.format(p)] for p in positions]
+    baseline_images_list = [[f'axis_label_position_{p}'] for p in positions]
 
     @pytest.mark.parametrize('position, baseline_images',
                              zip(positions, baseline_images_list))
     @image_comparison(baseline_images=None, extensions=['pdf'], style='mpl20')
     def test_axis_label_position(self, position, baseline_images):
         fix_text_kerning_factor()
 
@@ -134,25 +143,26 @@
 class TestTitle:
     locs = ['center', 'left', 'right']
     baseline_images_list = [[f'titie_{loc}'] for loc in locs]
 
     @pytest.mark.parametrize('loc, baseline_images',
                              zip(locs, baseline_images_list),)
     @image_comparison(baseline_images=None, extensions=['pdf'], style='mpl20')
-    def test_tick_direction(self, loc, baseline_images):
+    def test_title_loc(self, loc, baseline_images):
         fix_text_kerning_factor()
 
         fig = plt.figure()
         ax = fig.add_subplot(projection='ternary')
         ax.set_title("Title", loc=loc)
 
 
 @image_comparison(baseline_images=['aspect'], extensions=['pdf'],
                   style='mpl20')
 def test_aspect():
+    """Test if `set_aspect` works."""
     fix_text_kerning_factor()
 
     fig = plt.figure()
     ax = fig.add_subplot(projection='ternary')
     ax.plot(*get_spiral())
 
     ax.set_aspect(1.5)
@@ -198,18 +208,19 @@
     [text.update(rkwargs) for text in ax.raxis.get_ticklabels()]
 
 
 class TestTicks:
     @image_comparison(baseline_images=['opposite_ticks'], extensions=['pdf'],
                       style='mpl20')
     def test_opposite_ticks(self):
-        # This changes only tick & label positions but does not change data
-        # visualizations.
-        # Check if the tick-markers, tick-labels, and axis-labels are shown as
-        # expected.
+        """Test if "tick2" works.
+
+        "tick2" should change the positions of tick-markers, tick-labels, and
+        axis-labels but should not change data points.
+        """
         fix_text_kerning_factor()
 
         fig = plt.figure()
         ax = fig.add_subplot(projection='ternary')
 
         ax.taxis.set_ticks_position('tick2')
         ax.laxis.set_ticks_position('tick2')
@@ -232,14 +243,15 @@
         fig = plt.figure()
         ax = fig.add_subplot(projection='ternary')
         ax.set_ternary_min(0, 3, -3)
 
     @image_comparison(baseline_images=['manual_ticks'],
                       extensions=['pdf'], style='mpl20')
     def test_manual_ticks(self):
+        """Test if ticks can be manually given."""
         fix_text_kerning_factor()
 
         fig = plt.figure()
         ax = fig.add_subplot(projection='ternary')
 
         ax.plot(*get_spiral())
 
@@ -250,73 +262,259 @@
         ax.set_rlabel('Right')
 
         # Specify tick positions manually.
         ax.taxis.set_ticks([0.2, 0.4, 0.6, 0.8, 1.0])
         ax.laxis.set_ticks([0.2, 0.4, 0.6, 0.8, 1.0])
         ax.raxis.set_ticks([0.2, 0.4, 0.6, 0.8, 1.0])
 
+    @image_comparison(baseline_images=['manual_ticklabels'],
+                      extensions=['pdf'], style='mpl20')
+    def test_manual_ticklabels(self):
+        """Test if tick-labels can be manually given."""
+        fix_text_kerning_factor()
+
+        fig = plt.figure()
+        ax = fig.add_subplot(projection='ternary')
+
+        # Specify tick positions manually.
+        ticks = [0.0, 0.2, 0.4, 0.6, 0.8, 1.0]
+        labels = ["0/5", "1/5", "2/5", "3/5", "4/5", "5/5"]
+        ax.taxis.set_ticks(ticks, labels=labels)
+        ax.laxis.set_ticks(ticks, labels=labels)
+        ax.raxis.set_ticks(ticks, labels=labels)
+
+    @mpl.style.context("default")
+    @check_figures_equal(extensions=('pdf',))
+    def test_number_of_ticks(self, fig_test, fig_ref):
+        """
+        Test if the number of ticks are automatically properly adjusted.
+
+        It is necessary to switch the style to "default" because the "classic"
+        style gives a different result.
+        """
+        ax = fig_test.add_subplot(projection="ternary")
+        ax.set_ternary_lim(0.0, 0.2, 0.0, 1.0, 0.0, 1.0)
+
+        ax = fig_ref.add_subplot(projection="ternary")
+        ax.set_ternary_lim(0.0, 0.2, 0.0, 1.0, 0.0, 1.0)
+        ax.taxis.set_ticks([0.0, 0.1, 0.2])
+
 
 @check_figures_equal(extensions=('pdf',))
-def test_ternary_lim(fig_test, fig_ref):
-    """
-    Check that the order of `plot` and `set_ternary_lim` does not affect
-    the result.
-    """
-    ax = fig_test.add_subplot(projection='ternary')
-    t, l, r = get_spiral()
-    ax.set_ternary_lim(
-        0.1, 0.5,  # tmin, tmax
-        0.2, 0.6,  # lmin, lmax
-        0.3, 0.7,  # rmin, rmax
-    )
-    ax.plot(t, l, r)
+def test_ternary_sum(fig_test, fig_ref):
+    """Test if the `ternary_sum` argument works correctly."""
+    ax = fig_test.add_subplot(projection='ternary', ternary_sum=0.5)
+    tn0, tn1, tn2 = get_spiral()
+    ax.plot(tn0, tn1, tn2)
     ax.set_tlabel('Top')
     ax.set_llabel('Left')
     ax.set_rlabel('Right')
 
     ax = fig_ref.add_subplot(projection='ternary')
-    t, l, r = get_spiral()
-    ax.plot(t, l, r)
-    ax.set_ternary_lim(
-        0.1, 0.5,  # tmin, tmax
-        0.2, 0.6,  # lmin, lmax
-        0.3, 0.7,  # rmin, rmax
-    )
+    tn0, tn1, tn2 = get_spiral()
+    ax.plot(tn0, tn1, tn2)
     ax.set_tlabel('Top')
     ax.set_llabel('Left')
     ax.set_rlabel('Right')
+    ticks = [0.0, 0.2, 0.4, 0.6, 0.8, 1.0]
+    ticklabels = [0.0, 0.1, 0.2, 0.3, 0.4, 0.5]
+    ax.taxis.set_ticks(ticks, ticklabels)
+    ax.laxis.set_ticks(ticks, ticklabels)
+    ax.raxis.set_ticks(ticks, ticklabels)
+
+
+class TestTernaryLim:
+    @check_figures_equal(extensions=('pdf',))
+    def test_order_data(self, fig_test, fig_ref):
+        """
+        Check that the order of `plot` and `set_ternary_lim` does not affect
+        the result.
+        """
+        tn0, tn1, tn2 = get_spiral()
+
+        ax = fig_test.add_subplot(projection="ternary")
+        ax.set_ternary_lim(
+            0.1, 0.5,  # tmin, tmax
+            0.2, 0.6,  # lmin, lmax
+            0.3, 0.7,  # rmin, rmax
+        )
+        ax.plot(tn0, tn1, tn2)
+
+        ax = fig_ref.add_subplot(projection="ternary")
+        ax.plot(tn0, tn1, tn2)
+        ax.set_ternary_lim(
+            0.1, 0.5,  # tmin, tmax
+            0.2, 0.6,  # lmin, lmax
+            0.3, 0.7,  # rmin, rmax
+        )
+
+    @check_figures_equal(extensions=('pdf',))
+    def test_order_axes(self, fig_test, fig_ref):
+        tn0, tn1, tn2 = get_spiral()
 
+        ax = fig_test.add_subplot(projection="ternary")
+        ax.set_ternary_lim(0.1, 0.7, 0.1, 0.6, 0.1, 0.5)
+        ax.plot(tn0, tn1, tn2)
+        ax.plot(tn0, tn1, tn2, "k", transform=ax.transTernaryAxes)
+
+        ax = fig_ref.add_subplot(projection="ternary")
+        ax.plot(tn0, tn1, tn2)
+        ax.plot(tn0, tn1, tn2, "k", transform=ax.transTernaryAxes)
+        ax.set_ternary_lim(0.1, 0.7, 0.1, 0.6, 0.1, 0.5)
 
-def set_spans(ax):
-    # "clip_on=False" is just for testing purpose
-    ax.axtline(0.2, c='C0', clip_on=False)  # line for equi-t values
-    ax.axlline(0.3, c='C1', clip_on=False)  # line for equi-l values
-    ax.axrline(0.4, c='C2', clip_on=False)  # line for equi-r values
-
-    # "clip_on=False" is just for testing purpose
-    kwargs = dict(alpha=0.2, clip_on=False)
-    ax.axtspan(0.3, 0.4, fc='C0', **kwargs)  # region between tmin and tmax
-    ax.axlspan(0.4, 0.5, fc='C1', **kwargs)  # region between lmin and lmax
-    ax.axrspan(0.5, 0.6, fc='C2', **kwargs)  # region between rmin and rmax
+    @check_figures_equal(extensions=('pdf',))
+    def test_order_limits(self, fig_test, fig_ref):
+        """Test if the plot is insensitive to the orders of limits."""
+        ax = fig_test.add_subplot(projection="ternary")
+        ax.set_ternary_lim(0.1, 0.7, 0.1, 0.6, 0.1, 0.5)
+
+        ax = fig_ref.add_subplot(projection="ternary")
+        ax.set_ternary_lim(0.7, 0.1, 0.6, 0.1, 0.5, 0.1)
+
+    @check_figures_equal(extensions=('pdf',))
+    def test_min_vs_max(self, fig_test, fig_ref):
+        """Test if ternary_min and ternary_max give the same result."""
+        ax = fig_test.add_subplot(projection="ternary")
+        ax.set_ternary_min(0.1, 0.2, 0.3)
+
+        ax = fig_ref.add_subplot(projection="ternary")
+        ax.set_ternary_max(0.5, 0.6, 0.7)
+
+    @pytest.mark.parametrize(
+        "fit, baseline_images", [
+            ["rectangle", ["fit_rectangle"]],
+            ["triangle", ["fit_triangle"]],
+            ["none", ["fit_none"]],
+        ],
+    )
+    @image_comparison(
+        baseline_images=None,
+        extensions=['pdf'],
+        remove_text=True,
+        style='mpl20',
+    )
+    def test_fit(self, fit: str, baseline_images):
+        """Test if hexagonal limits are properly plotted."""
+        fig = plt.figure()
+        ax = fig.add_subplot(projection="ternary")
+        tn0, tn1, tn2 = get_spiral()
+        ax.plot(tn0, tn1, tn2, "C0")
+        ax.plot(tn0, tn1, tn2, "k", transform=ax.transTernaryAxes)
+        ax.set_facecolor("0.9")
+        ax.grid(True)
+        ax.set_ternary_lim(0.1, 0.7, 0.1, 0.6, 0.1, 0.5, fit)
+
+    @pytest.mark.parametrize("fit", ["rectangle", "triangle", "none"])
+    @check_figures_equal(extensions=('pdf',))
+    def test_ternary_lim_vs_tlrlims_0(self, fig_test, fig_ref, fit):
+        """Test if the plot is insensitive to the orders of limits."""
+        ax = fig_test.add_subplot(projection="ternary")
+        ax.set_tlim(0.1, 0.5, fit)
+        ax.set_llim(0.2, 0.6, fit)
+        ax.set_rlim(0.3, 0.7, fit)
+
+        ax = fig_ref.add_subplot(projection="ternary")
+        ax.set_ternary_lim(0.1, 0.5, 0.2, 0.6, 0.3, 0.7, fit)
+
+    @pytest.mark.parametrize("fit", ["rectangle", "triangle", "none"])
+    @check_figures_equal(extensions=('pdf',))
+    def test_ternary_lim_vs_tlrlims_1(self, fig_test, fig_ref, fit):
+        """Test if the plot is insensitive to the orders of limits."""
+        ax = fig_test.add_subplot(projection="ternary")
+        ax.set_tlim(0.1, 0.7, fit)
+        ax.set_llim(0.1, 0.6, fit)
+        ax.set_rlim(0.1, 0.5, fit)
+
+        ax = fig_ref.add_subplot(projection="ternary")
+        ax.set_ternary_lim(0.1, 0.7, 0.1, 0.6, 0.1, 0.5, fit)
+
+
+class TestSpans:
+    """Tests related to spans."""
+    @image_comparison(
+        baseline_images=['spans'],
+        extensions=['pdf'],
+        remove_text=True,
+        style='mpl20',
+    )
+    def test_spans(self):
+        """Test if spans are plotted properly."""
+        fig = plt.figure()
+        ax = fig.add_subplot(projection="ternary")
+
+        ax.axtline(0.2, c='C0')
+        ax.axlline(0.3, c='C1')
+        ax.axrline(0.4, c='C2')
+
+        ax.axtspan(0.3, 0.5, fc='C0', alpha=0.2)
+        ax.axlspan(0.4, 0.6, fc='C1', alpha=0.2)
+        ax.axrspan(0.5, 0.7, fc='C2', alpha=0.2)
+
+    def test_axtline_transform(self):
+        """Test if `axtline` raises `ValueError` when getting `transform`"""
+        fig = plt.figure()
+        ax = fig.add_subplot(projection="ternary")
+        with pytest.raises(ValueError):
+            ax.axtline(0.5, transform=ax.transAxes)
+
+    def test_axlline_transform(self):
+        """Test if `axlline` raises `ValueError` when getting `transform`"""
+        fig = plt.figure()
+        ax = fig.add_subplot(projection="ternary")
+        with pytest.raises(ValueError):
+            ax.axlline(0.5, transform=ax.transAxes)
+
+    def test_axrline_transform(self):
+        """Test if `axrline` raises `ValueError` when getting `transform`"""
+        fig = plt.figure()
+        ax = fig.add_subplot(projection="ternary")
+        with pytest.raises(ValueError):
+            ax.axrline(0.5, transform=ax.transAxes)
 
 
 class TestTickDirection:
     directions = ['in', 'out', 'inout']
-    baseline_images_list = [
-        ['tick_direction_{}'.format(d)] for d in directions]
+    baseline_images_list = [[f'tick_direction_{d}'] for d in directions]
 
     @pytest.mark.parametrize('direction, baseline_images',
                              zip(directions, baseline_images_list))
     @image_comparison(baseline_images=None, extensions=['pdf'], style='mpl20')
     def test_tick_direction(self, direction, baseline_images):
         fig = plt.figure()
         ax = fig.add_subplot(projection='ternary')
         ax.tick_params(direction=direction)
 
 
+class TestAxisLabels:
+    """Test if ternary axis labels are assigned properly."""
+    def test_tlabel(self):
+        """Test if the t-axis label is assigned properly."""
+        fig = plt.figure()
+        ax = fig.add_subplot(projection='ternary')
+        label = "T"
+        ax.set_tlabel(label)
+        assert ax.get_tlabel() == label
+
+    def test_llabel(self):
+        """Test if the l-axis label is assigned properly."""
+        fig = plt.figure()
+        ax = fig.add_subplot(projection='ternary')
+        label = "L"
+        ax.set_llabel(label)
+        assert ax.get_llabel() == label
+
+    def test_rlabel(self):
+        """Test if the r-axis label is assigned properly."""
+        fig = plt.figure()
+        ax = fig.add_subplot(projection='ternary')
+        label = "R"
+        ax.set_rlabel(label)
+        assert ax.get_rlabel() == label
+
+
 class TestAxLine:
     @check_figures_equal(extensions=('pdf',))
     def test_axline(self, fig_test, fig_ref):
         ax = fig_test.add_subplot(projection='ternary')
         ax.axline((1.0, 0.0, 0.0), (0.0, 0.5, 0.5))
 
         ax = fig_ref.add_subplot(projection='ternary')
@@ -372,39 +570,40 @@
             # two identical points are not allowed
             ax.axline((1, 0, 0), (1, 0, 0))
             plt.draw()
 
 
 @image_comparison(baseline_images=['text'], extensions=['pdf'], style='mpl20')
 def test_text():
+    """Test if text is plotted correctly."""
     fig = plt.figure()
     ax = fig.add_subplot(projection='ternary')
     v = 1.0 / 3.0
     ax.text(v, v, v, 'center', ha='center', va='center')
 
 
 class TestScatter:
     @image_comparison(baseline_images=['scatter'], extensions=['pdf'],
                       tol=1.0, style='mpl20')
     def test_scatter(self):
-        t, l, r = get_scatter_points()
+        tn0, tn1, tn2 = get_scatter_points()
         fig = plt.figure()
         ax = fig.add_subplot(projection='ternary')
-        ax.scatter(t, l, r)
+        ax.scatter(tn0, tn1, tn2)
 
     @image_comparison(baseline_images=['scatter_color'], extensions=['pdf'],
                       tol=1.0, style='mpl20')
     def test_scatter_color(self):
         fix_text_kerning_factor()
 
-        t, l, r = get_scatter_points()
+        tn0, tn1, tn2 = get_scatter_points()
         fig = plt.figure()
         fig.subplots_adjust(left=0.075, right=0.85)
         ax = fig.add_subplot(111, projection='ternary')
-        sc = ax.scatter(t, l, r, c=range(len(t)))
+        sc = ax.scatter(tn0, tn1, tn2, c=range(len(tn0)))
         cax = ax.inset_axes([1.05, 0.1, 0.05, 0.9], transform=ax.transAxes)
         colorbar = fig.colorbar(sc, cax=cax)
         colorbar.set_label('Count', rotation=270, va='baseline')
 
         ax.set_tlabel('Top')
         ax.set_llabel('Left')
         ax.set_rlabel('Right')
@@ -444,36 +643,36 @@
         ax.arrow(0.2, 0.2, 0.6, 0.6, transform=ax.transAxes)
 
 
 class TestQuiver:
     @image_comparison(baseline_images=['quiver'], extensions=['pdf'],
                       style='mpl20')
     def test_quiver(self):
-        t, l, r = get_triangular_grid()
-        dt = 1.0 / 3.0 - t
-        dl = 1.0 / 3.0 - l
-        dr = 1.0 / 3.0 - r
+        tn0, tn1, tn2 = get_triangular_grid()
+        dtn0 = 1.0 / 3.0 - tn0
+        dtn1 = 1.0 / 3.0 - tn1
+        dtn2 = 1.0 / 3.0 - tn2
         fig = plt.figure()
         ax = fig.add_subplot(projection='ternary')
-        ax.quiver(t, l, r, dt, dl, dr)
+        ax.quiver(tn0, tn1, tn2, dtn0, dtn1, dtn2)
 
     @image_comparison(baseline_images=['quiver_color'], extensions=['pdf'],
                       tol=0.3, style='mpl20')
     def test_quiver_color(self):
         fix_text_kerning_factor()
 
-        t, l, r = get_triangular_grid()
-        dt = 1.0 / 3.0 - t
-        dl = 1.0 / 3.0 - l
-        dr = 1.0 / 3.0 - r
-        length = np.sqrt(dt ** 2 + dl ** 2 + dr ** 2)
+        tn0, tn1, tn2 = get_triangular_grid()
+        dtn0 = 1.0 / 3.0 - tn0
+        dtn1 = 1.0 / 3.0 - tn1
+        dtn2 = 1.0 / 3.0 - tn2
+        length = np.sqrt(dtn0**2 + dtn1**2 + dtn2**2)
         fig = plt.figure()
         fig.subplots_adjust(left=0.075, right=0.85)
         ax = fig.add_subplot(projection='ternary')
-        pc = ax.quiver(t, l, r, dt, dl, dr, length)
+        pc = ax.quiver(tn0, tn1, tn2, dtn0, dtn1, dtn2, length)
         cax = ax.inset_axes([1.05, 0.1, 0.05, 0.9], transform=ax.transAxes)
         colorbar = fig.colorbar(pc, cax=cax)
         colorbar.set_label('Length', rotation=270, va='baseline')
 
         ax.set_tlabel('Top')
         ax.set_llabel('Left')
         ax.set_rlabel('Right')
@@ -501,17 +700,30 @@
         dy = 0.5 - y
         fig = plt.figure()
         ax = fig.add_subplot(projection='ternary')
         ax.set_ternary_min(-0.2, -0.2, -0.2)
         ax.quiver(x, y, dx, dy, transform=ax.transAxes)
 
 
+@check_figures_equal(extensions=('pdf',))
+def test_grid_both(fig_test, fig_ref):
+    """Test if `grid("both")` gives the expected result."""
+    ax = fig_test.add_subplot(projection="ternary")
+    ax.grid(axis="both")
+
+    ax = fig_ref.add_subplot(projection="ternary")
+    ax.grid(axis="t")
+    ax.grid(axis="l")
+    ax.grid(axis="r")
+
+
 @image_comparison(baseline_images=['legend'], extensions=['pdf'],
                   tol=0.3, style='mpl20')
 def test_legend():
+    """Test if the legend is plotted correctly."""
     fig = plt.figure()
     ax = fig.add_subplot(projection='ternary')
 
     for seed in [1, 9, 6, 8]:
         ax.scatter(*get_scatter_points(11, seed=seed), alpha=0.5, label=seed)
 
     ax.legend()
```

### Comparing `mpltern-0.5.0/tests/test_text.py` & `mpltern-1.0.0/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/test_tick.py` & `mpltern-1.0.0/tests/test_tick.py`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/test_triangle_rotation_axis.py` & `mpltern-1.0.0/tests/test_triangle_rotation_axis.py`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/test_triangle_rotation_horizontal.py` & `mpltern-1.0.0/tests/test_triangle_rotation_horizontal.py`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/test_triangle_rotation_tick.py` & `mpltern-1.0.0/tests/test_triangle_rotation_tick.py`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/test_tribin.py` & `mpltern-1.0.0/tests/test_tribin.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import numpy as np
 
 import matplotlib.pyplot as plt
-from matplotlib.testing.decorators import image_comparison
-import mpltern
+from matplotlib.testing.decorators import image_comparison, check_figures_equal
+from matplotlib.colors import LogNorm
+import mpltern  # noqa: F401
+
 
 @image_comparison(
     baseline_images=["base"],
     extensions=["pdf"],
     style="mpl20",
 )
 def test_base():
     np.random.seed(19680801)
     t, l, r = np.random.dirichlet(alpha=(2.0, 4.0, 8.0), size=100000).T
     ax = plt.subplot(projection="ternary")
     # If "face" (default), small hexagons look overlapping with each other.
     ax.tribin(t, l, r, edgecolors="none")
 
+
 @image_comparison(
     baseline_images=["ternary_lim"],
     extensions=["pdf"],
     style="mpl20",
 )
 def test_ternary_lim():
     np.random.seed(19680801)
@@ -29,32 +32,46 @@
     ax.tribin(t, l, r, edgecolors="none")
     ax.set_ternary_lim(
         0.1, 0.5,  # tmin, tmax
         0.2, 0.6,  # lmin, lmax
         0.3, 0.7,  # rmin, rmax
     )
 
+
 @image_comparison(
     baseline_images=["extent"],
     extensions=["pdf"],
     style="mpl20",
 )
 def test_extent():
     np.random.seed(19680801)
     t, l, r = np.random.dirichlet(alpha=(2.0, 4.0, 8.0), size=100000).T
     ax = plt.subplot(projection="ternary")
     extent = (0.1, 0.5, 0.2, 0.6, 0.3, 0.7)
     # If "face" (default), small hexagons look overlapping with each other.
     ax.tribin(t, l, r, gridsize=40, extent=extent, edgecolors="none")
 
+
 @image_comparison(
     baseline_images=["given_triangles"],
     extensions=["pdf"],
     style="mpl20",
 )
 def test_given_triangles():
     corners = ((0.5, 0.0), (1.0, 0.5), (0.0, 1.0))
     np.random.seed(19680801)
     t, l, r = np.random.dirichlet(alpha=(2.0, 4.0, 8.0), size=100000).T
     ax = plt.subplot(projection="ternary", corners=corners, rotation=0)
     # If "face" (default), small hexagons look overlapping with each other.
     ax.tribin(t, l, r, edgecolors="none")
+
+
+@check_figures_equal(extensions=('pdf',))
+def test_bins_and_norm(fig_test, fig_ref):
+    np.random.seed(19680801)
+    t, l, r = np.random.dirichlet(alpha=(2.0, 4.0, 8.0), size=100000).T
+
+    ax = fig_test.add_subplot(projection="ternary")
+    ax.tribin(t, l, r, bins="log")
+
+    ax = fig_ref.add_subplot(projection="ternary")
+    ax.tribin(t, l, r, norm=LogNorm())
```

### Comparing `mpltern-0.5.0/tests/test_tribin_helpers.py` & `mpltern-1.0.0/tests/test_tribin_helpers.py`

 * *Files identical despite different names*

### Comparing `mpltern-0.5.0/tests/tribin_indices.txt` & `mpltern-1.0.0/tests/tribin_indices.txt`

 * *Files identical despite different names*

